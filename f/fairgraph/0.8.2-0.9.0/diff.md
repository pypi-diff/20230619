# Comparing `tmp/fairgraph-0.8.2.tar.gz` & `tmp/fairgraph-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fairgraph-0.8.2.tar", last modified: Tue Nov  8 10:15:40 2022, max compression
+gzip compressed data, was "fairgraph-0.9.0.tar", last modified: Tue Feb 28 20:36:45 2023, max compression
```

## Comparing `fairgraph-0.8.2.tar` & `fairgraph-0.9.0.tar`

### file list

```diff
@@ -1,277 +1,310 @@
-drwxr-xr-x   0 adavison   (502) staff       (20)        0 2022-11-08 10:15:40.804993 fairgraph-0.8.2/
--rw-r--r--   0 adavison   (502) staff       (20)    10174 2022-03-03 13:47:15.000000 fairgraph-0.8.2/LICENSE.txt
--rw-r--r--   0 adavison   (502) staff       (20)       45 2022-03-03 13:47:15.000000 fairgraph-0.8.2/MANIFEST.in
--rw-r--r--   0 adavison   (502) staff       (20)     6919 2022-11-08 10:15:40.804841 fairgraph-0.8.2/PKG-INFO
--rw-r--r--   0 adavison   (502) staff       (20)     6063 2022-11-08 09:52:09.000000 fairgraph-0.8.2/README.md
-drwxr-xr-x   0 adavison   (502) staff       (20)        0 2022-11-08 10:15:40.741390 fairgraph-0.8.2/fairgraph/
--rw-r--r--   0 adavison   (502) staff       (20)      984 2022-11-08 09:51:35.000000 fairgraph-0.8.2/fairgraph/__init__.py
--rw-r--r--   0 adavison   (502) staff       (20)    13195 2022-08-24 15:08:51.000000 fairgraph-0.8.2/fairgraph/analysis.py
--rw-r--r--   0 adavison   (502) staff       (20)    47469 2022-08-24 15:08:51.000000 fairgraph-0.8.2/fairgraph/base_v2.py
--rw-r--r--   0 adavison   (502) staff       (20)    53375 2022-11-07 09:39:53.000000 fairgraph-0.8.2/fairgraph/base_v3.py
--rw-r--r--   0 adavison   (502) staff       (20)    33890 2022-08-24 15:08:51.000000 fairgraph-0.8.2/fairgraph/brainsimulation.py
--rw-r--r--   0 adavison   (502) staff       (20)    16561 2022-08-24 15:08:51.000000 fairgraph-0.8.2/fairgraph/client_v2.py
--rw-r--r--   0 adavison   (502) staff       (20)    15352 2022-11-02 08:53:00.000000 fairgraph-0.8.2/fairgraph/client_v3.py
--rw-r--r--   0 adavison   (502) staff       (20)    32828 2022-08-24 15:08:51.000000 fairgraph-0.8.2/fairgraph/commons.py
--rw-r--r--   0 adavison   (502) staff       (20)     2419 2022-08-24 15:08:51.000000 fairgraph-0.8.2/fairgraph/computing.py
--rw-r--r--   0 adavison   (502) staff       (20)    17120 2022-08-24 15:08:51.000000 fairgraph-0.8.2/fairgraph/core.py
--rw-r--r--   0 adavison   (502) staff       (20)     2569 2022-08-24 15:08:51.000000 fairgraph-0.8.2/fairgraph/data.py
--rw-r--r--   0 adavison   (502) staff       (20)    58899 2022-08-24 15:08:51.000000 fairgraph-0.8.2/fairgraph/electrophysiology.py
--rw-r--r--   0 adavison   (502) staff       (20)      378 2022-08-24 15:08:51.000000 fairgraph-0.8.2/fairgraph/errors.py
--rw-r--r--   0 adavison   (502) staff       (20)    21203 2022-08-24 15:08:51.000000 fairgraph-0.8.2/fairgraph/experiment.py
--rw-r--r--   0 adavison   (502) staff       (20)    10312 2022-10-21 14:21:42.000000 fairgraph-0.8.2/fairgraph/fields.py
--rw-r--r--   0 adavison   (502) staff       (20)    18905 2022-08-24 15:08:51.000000 fairgraph-0.8.2/fairgraph/livepapers.py
--rw-r--r--   0 adavison   (502) staff       (20)    32171 2022-08-24 15:08:51.000000 fairgraph-0.8.2/fairgraph/minds.py
--rw-r--r--   0 adavison   (502) staff       (20)    11552 2022-08-24 15:08:51.000000 fairgraph-0.8.2/fairgraph/morphology.py
-drwxr-xr-x   0 adavison   (502) staff       (20)        0 2022-11-08 10:15:40.743517 fairgraph-0.8.2/fairgraph/openminds/
--rw-r--r--   0 adavison   (502) staff       (20)       88 2022-10-21 14:21:42.000000 fairgraph-0.8.2/fairgraph/openminds/__init__.py
-drwxr-xr-x   0 adavison   (502) staff       (20)        0 2022-11-08 10:15:40.745600 fairgraph-0.8.2/fairgraph/openminds/chemicals/
--rw-r--r--   0 adavison   (502) staff       (20)      505 2022-10-21 14:21:42.000000 fairgraph-0.8.2/fairgraph/openminds/chemicals/__init__.py
--rw-r--r--   0 adavison   (502) staff       (20)     1096 2022-10-21 14:21:42.000000 fairgraph-0.8.2/fairgraph/openminds/chemicals/amount_of_chemical.py
--rw-r--r--   0 adavison   (502) staff       (20)     1619 2022-10-21 14:21:42.000000 fairgraph-0.8.2/fairgraph/openminds/chemicals/chemical_mixture.py
--rw-r--r--   0 adavison   (502) staff       (20)     1540 2022-10-21 14:21:42.000000 fairgraph-0.8.2/fairgraph/openminds/chemicals/chemical_substance.py
--rw-r--r--   0 adavison   (502) staff       (20)     1540 2022-10-21 14:21:42.000000 fairgraph-0.8.2/fairgraph/openminds/chemicals/product_source.py
-drwxr-xr-x   0 adavison   (502) staff       (20)        0 2022-11-08 10:15:40.753557 fairgraph-0.8.2/fairgraph/openminds/computation/
--rw-r--r--   0 adavison   (502) staff       (20)      986 2022-10-21 14:21:42.000000 fairgraph-0.8.2/fairgraph/openminds/computation/__init__.py
--rw-r--r--   0 adavison   (502) staff       (20)     4651 2022-10-21 14:21:42.000000 fairgraph-0.8.2/fairgraph/openminds/computation/data_analysis.py
--rw-r--r--   0 adavison   (502) staff       (20)     1741 2022-10-21 14:21:42.000000 fairgraph-0.8.2/fairgraph/openminds/computation/environment.py
--rw-r--r--   0 adavison   (502) staff       (20)     1159 2022-10-21 14:19:55.000000 fairgraph-0.8.2/fairgraph/openminds/computation/hardware_system.py
--rw-r--r--   0 adavison   (502) staff       (20)     1511 2022-10-21 14:19:55.000000 fairgraph-0.8.2/fairgraph/openminds/computation/launch_configuration.py
--rw-r--r--   0 adavison   (502) staff       (20)     2141 2022-10-21 14:19:55.000000 fairgraph-0.8.2/fairgraph/openminds/computation/local_file.py
--rw-r--r--   0 adavison   (502) staff       (20)     4694 2022-10-21 14:21:42.000000 fairgraph-0.8.2/fairgraph/openminds/computation/model_validation.py
--rw-r--r--   0 adavison   (502) staff       (20)     4544 2022-10-21 14:21:42.000000 fairgraph-0.8.2/fairgraph/openminds/computation/optimization.py
--rw-r--r--   0 adavison   (502) staff       (20)     4507 2022-10-21 14:21:42.000000 fairgraph-0.8.2/fairgraph/openminds/computation/simulation.py
--rw-r--r--   0 adavison   (502) staff       (20)     1175 2022-10-21 14:19:55.000000 fairgraph-0.8.2/fairgraph/openminds/computation/software_agent.py
--rw-r--r--   0 adavison   (502) staff       (20)     3871 2022-10-21 14:21:42.000000 fairgraph-0.8.2/fairgraph/openminds/computation/validation_test.py
--rw-r--r--   0 adavison   (502) staff       (20)     9377 2022-10-21 14:21:42.000000 fairgraph-0.8.2/fairgraph/openminds/computation/validation_test_version.py
--rw-r--r--   0 adavison   (502) staff       (20)     4485 2022-10-21 14:21:42.000000 fairgraph-0.8.2/fairgraph/openminds/computation/visualization.py
--rw-r--r--   0 adavison   (502) staff       (20)     1344 2022-10-21 14:21:42.000000 fairgraph-0.8.2/fairgraph/openminds/computation/workflow_execution.py
--rw-r--r--   0 adavison   (502) staff       (20)     2419 2022-10-21 14:19:55.000000 fairgraph-0.8.2/fairgraph/openminds/computation/workflow_recipe.py
--rw-r--r--   0 adavison   (502) staff       (20)     8897 2022-10-21 14:21:42.000000 fairgraph-0.8.2/fairgraph/openminds/computation/workflow_recipe_version.py
-drwxr-xr-x   0 adavison   (502) staff       (20)        0 2022-11-08 10:15:40.774486 fairgraph-0.8.2/fairgraph/openminds/controlledterms/
--rw-r--r--   0 adavison   (502) staff       (20)     3051 2022-10-21 14:21:42.000000 fairgraph-0.8.2/fairgraph/openminds/controlledterms/__init__.py
--rw-r--r--   0 adavison   (502) staff       (20)     2044 2022-10-21 14:19:55.000000 fairgraph-0.8.2/fairgraph/openminds/controlledterms/action_status_type.py
--rw-r--r--   0 adavison   (502) staff       (20)     2188 2022-10-21 14:19:55.000000 fairgraph-0.8.2/fairgraph/openminds/controlledterms/age_category.py
--rw-r--r--   0 adavison   (502) staff       (20)     2236 2022-10-21 14:19:55.000000 fairgraph-0.8.2/fairgraph/openminds/controlledterms/anatomical_axes_orientation.py
--rw-r--r--   0 adavison   (502) staff       (20)     2038 2022-10-21 14:19:55.000000 fairgraph-0.8.2/fairgraph/openminds/controlledterms/anatomical_plane.py
--rw-r--r--   0 adavison   (502) staff       (20)     2034 2022-10-21 14:19:55.000000 fairgraph-0.8.2/fairgraph/openminds/controlledterms/annotation_type.py
--rw-r--r--   0 adavison   (502) staff       (20)     2014 2022-10-21 14:19:55.000000 fairgraph-0.8.2/fairgraph/openminds/controlledterms/atlas_type.py
--rw-r--r--   0 adavison   (502) staff       (20)     2038 2022-10-21 14:19:55.000000 fairgraph-0.8.2/fairgraph/openminds/controlledterms/biological_order.py
--rw-r--r--   0 adavison   (502) staff       (20)     2150 2022-10-21 14:19:55.000000 fairgraph-0.8.2/fairgraph/openminds/controlledterms/biological_sex.py
--rw-r--r--   0 adavison   (502) staff       (20)     2026 2022-10-21 14:19:55.000000 fairgraph-0.8.2/fairgraph/openminds/controlledterms/breeding_type.py
--rw-r--r--   0 adavison   (502) staff       (20)     2040 2022-10-21 14:19:55.000000 fairgraph-0.8.2/fairgraph/openminds/controlledterms/cell_culture_type.py
--rw-r--r--   0 adavison   (502) staff       (20)     2010 2022-10-21 14:19:55.000000 fairgraph-0.8.2/fairgraph/openminds/controlledterms/cell_type.py
--rw-r--r--   0 adavison   (502) staff       (20)     2056 2022-10-21 14:21:42.000000 fairgraph-0.8.2/fairgraph/openminds/controlledterms/chemical_mixture_type.py
--rw-r--r--   0 adavison   (502) staff       (20)     2218 2022-10-21 14:19:55.000000 fairgraph-0.8.2/fairgraph/openminds/controlledterms/contribution_type.py
--rw-r--r--   0 adavison   (502) staff       (20)     2048 2022-10-21 14:19:55.000000 fairgraph-0.8.2/fairgraph/openminds/controlledterms/cranial_window_type.py
--rw-r--r--   0 adavison   (502) staff       (20)     2230 2022-10-21 14:19:55.000000 fairgraph-0.8.2/fairgraph/openminds/controlledterms/criteria_quality_type.py
--rw-r--r--   0 adavison   (502) staff       (20)     2010 2022-10-21 14:19:55.000000 fairgraph-0.8.2/fairgraph/openminds/controlledterms/data_type.py
--rw-r--r--   0 adavison   (502) staff       (20)     2018 2022-10-21 14:19:55.000000 fairgraph-0.8.2/fairgraph/openminds/controlledterms/device_type.py
--rw-r--r--   0 adavison   (502) staff       (20)     2046 2022-10-21 14:21:42.000000 fairgraph-0.8.2/fairgraph/openminds/controlledterms/difference_measure.py
--rw-r--r--   0 adavison   (502) staff       (20)     2080 2022-10-21 14:19:55.000000 fairgraph-0.8.2/fairgraph/openminds/controlledterms/disease.py
--rw-r--r--   0 adavison   (502) staff       (20)     2026 2022-10-21 14:19:55.000000 fairgraph-0.8.2/fairgraph/openminds/controlledterms/disease_model.py
--rw-r--r--   0 adavison   (502) staff       (20)     2168 2022-10-21 14:19:55.000000 fairgraph-0.8.2/fairgraph/openminds/controlledterms/ethics_assessment.py
--rw-r--r--   0 adavison   (502) staff       (20)     2058 2022-10-21 14:19:55.000000 fairgraph-0.8.2/fairgraph/openminds/controlledterms/experimental_approach.py
--rw-r--r--   0 adavison   (502) staff       (20)     2188 2022-10-21 14:19:55.000000 fairgraph-0.8.2/fairgraph/openminds/controlledterms/file_bundle_grouping.py
--rw-r--r--   0 adavison   (502) staff       (20)     2052 2022-10-21 14:19:55.000000 fairgraph-0.8.2/fairgraph/openminds/controlledterms/file_repository_type.py
--rw-r--r--   0 adavison   (502) staff       (20)     2176 2022-10-21 14:19:55.000000 fairgraph-0.8.2/fairgraph/openminds/controlledterms/file_usage_role.py
--rw-r--r--   0 adavison   (502) staff       (20)     2048 2022-10-21 14:19:55.000000 fairgraph-0.8.2/fairgraph/openminds/controlledterms/genetic_strain_type.py
--rw-r--r--   0 adavison   (502) staff       (20)     2016 2022-10-21 14:19:55.000000 fairgraph-0.8.2/fairgraph/openminds/controlledterms/handedness.py
--rw-r--r--   0 adavison   (502) staff       (20)     2126 2022-10-21 14:19:55.000000 fairgraph-0.8.2/fairgraph/openminds/controlledterms/language.py
--rw-r--r--   0 adavison   (502) staff       (20)     2116 2022-10-21 14:19:55.000000 fairgraph-0.8.2/fairgraph/openminds/controlledterms/laterality.py
--rw-r--r--   0 adavison   (502) staff       (20)     2042 2022-10-21 14:19:55.000000 fairgraph-0.8.2/fairgraph/openminds/controlledterms/measured_quantity.py
--rw-r--r--   0 adavison   (502) staff       (20)     2050 2022-10-21 14:19:55.000000 fairgraph-0.8.2/fairgraph/openminds/controlledterms/meta_data_model_type.py
--rw-r--r--   0 adavison   (502) staff       (20)     2210 2022-10-21 14:19:55.000000 fairgraph-0.8.2/fairgraph/openminds/controlledterms/model_abstraction_level.py
--rw-r--r--   0 adavison   (502) staff       (20)     2148 2022-10-21 14:19:55.000000 fairgraph-0.8.2/fairgraph/openminds/controlledterms/model_scope.py
--rw-r--r--   0 adavison   (502) staff       (20)     2038 2022-10-21 14:19:55.000000 fairgraph-0.8.2/fairgraph/openminds/controlledterms/molecular_entity.py
--rw-r--r--   0 adavison   (502) staff       (20)     2136 2022-10-21 14:19:55.000000 fairgraph-0.8.2/fairgraph/openminds/controlledterms/operating_device.py
--rw-r--r--   0 adavison   (502) staff       (20)     2136 2022-10-21 14:19:55.000000 fairgraph-0.8.2/fairgraph/openminds/controlledterms/operating_system.py
--rw-r--r--   0 adavison   (502) staff       (20)     1996 2022-10-21 14:19:55.000000 fairgraph-0.8.2/fairgraph/openminds/controlledterms/organ.py
--rw-r--r--   0 adavison   (502) staff       (20)     2056 2022-10-21 14:19:55.000000 fairgraph-0.8.2/fairgraph/openminds/controlledterms/patch_clamp_variation.py
--rw-r--r--   0 adavison   (502) staff       (20)     2038 2022-10-21 14:19:55.000000 fairgraph-0.8.2/fairgraph/openminds/controlledterms/preparation_type.py
--rw-r--r--   0 adavison   (502) staff       (20)     2058 2022-10-21 14:19:55.000000 fairgraph-0.8.2/fairgraph/openminds/controlledterms/product_accessibility.py
--rw-r--r--   0 adavison   (502) staff       (20)     2160 2022-10-21 14:19:55.000000 fairgraph-0.8.2/fairgraph/openminds/controlledterms/programming_language.py
--rw-r--r--   0 adavison   (502) staff       (20)     2050 2022-10-21 14:19:55.000000 fairgraph-0.8.2/fairgraph/openminds/controlledterms/qualitative_overlap.py
--rw-r--r--   0 adavison   (502) staff       (20)     2044 2022-10-21 14:19:55.000000 fairgraph-0.8.2/fairgraph/openminds/controlledterms/semantic_data_type.py
--rw-r--r--   0 adavison   (502) staff       (20)     2004 2022-10-21 14:19:55.000000 fairgraph-0.8.2/fairgraph/openminds/controlledterms/service.py
--rw-r--r--   0 adavison   (502) staff       (20)     2014 2022-10-21 14:21:42.000000 fairgraph-0.8.2/fairgraph/openminds/controlledterms/setup_type.py
--rw-r--r--   0 adavison   (502) staff       (20)     2226 2022-10-21 14:19:55.000000 fairgraph-0.8.2/fairgraph/openminds/controlledterms/software_application_category.py
--rw-r--r--   0 adavison   (502) staff       (20)     2038 2022-10-21 14:19:55.000000 fairgraph-0.8.2/fairgraph/openminds/controlledterms/software_feature.py
--rw-r--r--   0 adavison   (502) staff       (20)     2084 2022-10-21 14:19:55.000000 fairgraph-0.8.2/fairgraph/openminds/controlledterms/species.py
--rw-r--r--   0 adavison   (502) staff       (20)     2054 2022-10-21 14:19:55.000000 fairgraph-0.8.2/fairgraph/openminds/controlledterms/stimulation_approach.py
--rw-r--r--   0 adavison   (502) staff       (20)     2026 2022-10-21 14:19:55.000000 fairgraph-0.8.2/fairgraph/openminds/controlledterms/stimulus_type.py
--rw-r--r--   0 adavison   (502) staff       (20)     2046 2022-10-21 14:19:55.000000 fairgraph-0.8.2/fairgraph/openminds/controlledterms/subcellular_entity.py
--rw-r--r--   0 adavison   (502) staff       (20)     2042 2022-10-21 14:19:55.000000 fairgraph-0.8.2/fairgraph/openminds/controlledterms/subject_attribute.py
--rw-r--r--   0 adavison   (502) staff       (20)     2096 2022-10-21 14:19:55.000000 fairgraph-0.8.2/fairgraph/openminds/controlledterms/technique.py
--rw-r--r--   0 adavison   (502) staff       (20)     2469 2022-10-21 14:19:55.000000 fairgraph-0.8.2/fairgraph/openminds/controlledterms/term_suggestion.py
--rw-r--r--   0 adavison   (502) staff       (20)     2020 2022-10-21 14:19:55.000000 fairgraph-0.8.2/fairgraph/openminds/controlledterms/terminology.py
--rw-r--r--   0 adavison   (502) staff       (20)     2064 2022-10-21 14:19:55.000000 fairgraph-0.8.2/fairgraph/openminds/controlledterms/tissue_sample_attribute.py
--rw-r--r--   0 adavison   (502) staff       (20)     2176 2022-10-21 14:19:55.000000 fairgraph-0.8.2/fairgraph/openminds/controlledterms/tissue_sample_type.py
--rw-r--r--   0 adavison   (502) staff       (20)     2048 2022-10-21 14:19:55.000000 fairgraph-0.8.2/fairgraph/openminds/controlledterms/type_of_uncertainty.py
--rw-r--r--   0 adavison   (502) staff       (20)     2060 2022-10-21 14:19:55.000000 fairgraph-0.8.2/fairgraph/openminds/controlledterms/uberon_parcellation.py
--rw-r--r--   0 adavison   (502) staff       (20)     2152 2022-10-21 14:19:55.000000 fairgraph-0.8.2/fairgraph/openminds/controlledterms/unit_of_measurement.py
-drwxr-xr-x   0 adavison   (502) staff       (20)        0 2022-11-08 10:15:40.774755 fairgraph-0.8.2/fairgraph/openminds/core/
--rw-r--r--   0 adavison   (502) staff       (20)     3351 2022-10-21 14:21:42.000000 fairgraph-0.8.2/fairgraph/openminds/core/__init__.py
-drwxr-xr-x   0 adavison   (502) staff       (20)        0 2022-11-08 10:15:40.776456 fairgraph-0.8.2/fairgraph/openminds/core/actors/
--rw-r--r--   0 adavison   (502) staff       (20)        0 2022-10-21 14:19:55.000000 fairgraph-0.8.2/fairgraph/openminds/core/actors/__init__.py
--rw-r--r--   0 adavison   (502) staff       (20)     1140 2022-10-21 14:19:55.000000 fairgraph-0.8.2/fairgraph/openminds/core/actors/affiliation.py
--rw-r--r--   0 adavison   (502) staff       (20)      827 2022-10-21 14:19:55.000000 fairgraph-0.8.2/fairgraph/openminds/core/actors/contact_information.py
--rw-r--r--   0 adavison   (502) staff       (20)     1194 2022-10-21 14:19:55.000000 fairgraph-0.8.2/fairgraph/openminds/core/actors/contribution.py
--rw-r--r--   0 adavison   (502) staff       (20)     1620 2022-10-21 14:19:55.000000 fairgraph-0.8.2/fairgraph/openminds/core/actors/organization.py
--rw-r--r--   0 adavison   (502) staff       (20)     2605 2022-10-25 09:05:47.000000 fairgraph-0.8.2/fairgraph/openminds/core/actors/person.py
-drwxr-xr-x   0 adavison   (502) staff       (20)        0 2022-11-08 10:15:40.780358 fairgraph-0.8.2/fairgraph/openminds/core/data/
--rw-r--r--   0 adavison   (502) staff       (20)        0 2022-10-21 14:19:55.000000 fairgraph-0.8.2/fairgraph/openminds/core/data/__init__.py
--rw-r--r--   0 adavison   (502) staff       (20)     2283 2022-10-21 14:19:55.000000 fairgraph-0.8.2/fairgraph/openminds/core/data/content_type.py
--rw-r--r--   0 adavison   (502) staff       (20)     1085 2022-10-21 14:19:55.000000 fairgraph-0.8.2/fairgraph/openminds/core/data/content_type_pattern.py
--rw-r--r--   0 adavison   (502) staff       (20)     1122 2022-10-21 14:19:55.000000 fairgraph-0.8.2/fairgraph/openminds/core/data/copyright.py
--rw-r--r--   0 adavison   (502) staff       (20)     4989 2022-10-21 14:21:42.000000 fairgraph-0.8.2/fairgraph/openminds/core/data/file.py
--rw-r--r--   0 adavison   (502) staff       (20)     1285 2022-10-21 14:19:55.000000 fairgraph-0.8.2/fairgraph/openminds/core/data/file_archive.py
--rw-r--r--   0 adavison   (502) staff       (20)     2733 2022-10-21 14:19:55.000000 fairgraph-0.8.2/fairgraph/openminds/core/data/file_bundle.py
--rw-r--r--   0 adavison   (502) staff       (20)      905 2022-10-21 14:19:55.000000 fairgraph-0.8.2/fairgraph/openminds/core/data/file_path_pattern.py
--rw-r--r--   0 adavison   (502) staff       (20)     2634 2022-10-21 14:19:55.000000 fairgraph-0.8.2/fairgraph/openminds/core/data/file_repository.py
--rw-r--r--   0 adavison   (502) staff       (20)      987 2022-10-21 14:19:55.000000 fairgraph-0.8.2/fairgraph/openminds/core/data/file_repository_structure.py
--rw-r--r--   0 adavison   (502) staff       (20)     1021 2022-10-21 14:19:55.000000 fairgraph-0.8.2/fairgraph/openminds/core/data/hash.py
--rw-r--r--   0 adavison   (502) staff       (20)     1427 2022-10-21 14:19:55.000000 fairgraph-0.8.2/fairgraph/openminds/core/data/license.py
--rw-r--r--   0 adavison   (502) staff       (20)     1527 2022-10-21 14:21:42.000000 fairgraph-0.8.2/fairgraph/openminds/core/data/measurement.py
--rw-r--r--   0 adavison   (502) staff       (20)     1631 2022-10-21 14:21:42.000000 fairgraph-0.8.2/fairgraph/openminds/core/data/service_link.py
-drwxr-xr-x   0 adavison   (502) staff       (20)        0 2022-11-08 10:15:40.784314 fairgraph-0.8.2/fairgraph/openminds/core/miscellaneous/
--rw-r--r--   0 adavison   (502) staff       (20)        0 2022-10-21 14:19:55.000000 fairgraph-0.8.2/fairgraph/openminds/core/miscellaneous/__init__.py
--rw-r--r--   0 adavison   (502) staff       (20)     1780 2022-10-21 14:21:42.000000 fairgraph-0.8.2/fairgraph/openminds/core/miscellaneous/comment.py
--rw-r--r--   0 adavison   (502) staff       (20)      785 2022-10-21 14:19:55.000000 fairgraph-0.8.2/fairgraph/openminds/core/miscellaneous/doi.py
--rw-r--r--   0 adavison   (502) staff       (20)     1546 2022-10-21 14:19:55.000000 fairgraph-0.8.2/fairgraph/openminds/core/miscellaneous/funding.py
--rw-r--r--   0 adavison   (502) staff       (20)      793 2022-10-21 14:19:55.000000 fairgraph-0.8.2/fairgraph/openminds/core/miscellaneous/gridid.py
--rw-r--r--   0 adavison   (502) staff       (20)      793 2022-10-21 14:19:55.000000 fairgraph-0.8.2/fairgraph/openminds/core/miscellaneous/handle.py
--rw-r--r--   0 adavison   (502) staff       (20)      788 2022-10-21 14:19:55.000000 fairgraph-0.8.2/fairgraph/openminds/core/miscellaneous/isbn.py
--rw-r--r--   0 adavison   (502) staff       (20)      788 2022-10-21 14:19:55.000000 fairgraph-0.8.2/fairgraph/openminds/core/miscellaneous/issn.py
--rw-r--r--   0 adavison   (502) staff       (20)      790 2022-10-21 14:19:55.000000 fairgraph-0.8.2/fairgraph/openminds/core/miscellaneous/orcid.py
--rw-r--r--   0 adavison   (502) staff       (20)     1438 2022-10-21 14:19:55.000000 fairgraph-0.8.2/fairgraph/openminds/core/miscellaneous/quantitative_value.py
--rw-r--r--   0 adavison   (502) staff       (20)     1541 2022-10-21 14:21:42.000000 fairgraph-0.8.2/fairgraph/openminds/core/miscellaneous/quantitative_value_array.py
--rw-r--r--   0 adavison   (502) staff       (20)     1267 2022-10-21 14:19:55.000000 fairgraph-0.8.2/fairgraph/openminds/core/miscellaneous/quantitative_value_range.py
--rw-r--r--   0 adavison   (502) staff       (20)      790 2022-10-21 14:19:55.000000 fairgraph-0.8.2/fairgraph/openminds/core/miscellaneous/rorid.py
--rw-r--r--   0 adavison   (502) staff       (20)      787 2022-10-21 14:19:55.000000 fairgraph-0.8.2/fairgraph/openminds/core/miscellaneous/rrid.py
--rw-r--r--   0 adavison   (502) staff       (20)      900 2022-10-21 14:19:55.000000 fairgraph-0.8.2/fairgraph/openminds/core/miscellaneous/stock_number.py
--rw-r--r--   0 adavison   (502) staff       (20)      792 2022-10-21 14:19:55.000000 fairgraph-0.8.2/fairgraph/openminds/core/miscellaneous/swhid.py
--rw-r--r--   0 adavison   (502) staff       (20)      749 2022-10-21 14:19:55.000000 fairgraph-0.8.2/fairgraph/openminds/core/miscellaneous/url.py
-drwxr-xr-x   0 adavison   (502) staff       (20)        0 2022-11-08 10:15:40.786171 fairgraph-0.8.2/fairgraph/openminds/core/products/
--rw-r--r--   0 adavison   (502) staff       (20)        0 2022-10-21 14:19:55.000000 fairgraph-0.8.2/fairgraph/openminds/core/products/__init__.py
--rw-r--r--   0 adavison   (502) staff       (20)     2524 2022-10-21 14:19:55.000000 fairgraph-0.8.2/fairgraph/openminds/core/products/dataset.py
--rw-r--r--   0 adavison   (502) staff       (20)    12274 2022-10-21 14:21:42.000000 fairgraph-0.8.2/fairgraph/openminds/core/products/dataset_version.py
--rw-r--r--   0 adavison   (502) staff       (20)     2431 2022-10-21 14:19:55.000000 fairgraph-0.8.2/fairgraph/openminds/core/products/meta_data_model.py
--rw-r--r--   0 adavison   (502) staff       (20)     9137 2022-10-21 14:21:42.000000 fairgraph-0.8.2/fairgraph/openminds/core/products/meta_data_model_version.py
--rw-r--r--   0 adavison   (502) staff       (20)     3852 2022-10-21 14:19:55.000000 fairgraph-0.8.2/fairgraph/openminds/core/products/model.py
--rw-r--r--   0 adavison   (502) staff       (20)     9534 2022-10-21 14:21:42.000000 fairgraph-0.8.2/fairgraph/openminds/core/products/model_version.py
--rw-r--r--   0 adavison   (502) staff       (20)     2322 2022-10-21 14:21:42.000000 fairgraph-0.8.2/fairgraph/openminds/core/products/project.py
--rw-r--r--   0 adavison   (502) staff       (20)     1768 2022-10-21 14:21:42.000000 fairgraph-0.8.2/fairgraph/openminds/core/products/setup.py
--rw-r--r--   0 adavison   (502) staff       (20)     2503 2022-10-21 14:19:55.000000 fairgraph-0.8.2/fairgraph/openminds/core/products/software.py
--rw-r--r--   0 adavison   (502) staff       (20)    10470 2022-10-21 14:21:42.000000 fairgraph-0.8.2/fairgraph/openminds/core/products/software_version.py
-drwxr-xr-x   0 adavison   (502) staff       (20)        0 2022-11-08 10:15:40.789743 fairgraph-0.8.2/fairgraph/openminds/core/research/
--rw-r--r--   0 adavison   (502) staff       (20)        0 2022-10-21 14:19:55.000000 fairgraph-0.8.2/fairgraph/openminds/core/research/__init__.py
--rw-r--r--   0 adavison   (502) staff       (20)     1615 2022-10-21 14:19:55.000000 fairgraph-0.8.2/fairgraph/openminds/core/research/behavioral_protocol.py
--rw-r--r--   0 adavison   (502) staff       (20)     1102 2022-10-21 14:19:55.000000 fairgraph-0.8.2/fairgraph/openminds/core/research/configuration.py
--rw-r--r--   0 adavison   (502) staff       (20)     1200 2022-10-25 14:39:51.000000 fairgraph-0.8.2/fairgraph/openminds/core/research/custom_property_set.py
--rw-r--r--   0 adavison   (502) staff       (20)     3449 2022-10-21 14:19:55.000000 fairgraph-0.8.2/fairgraph/openminds/core/research/experimental_activity.py
--rw-r--r--   0 adavison   (502) staff       (20)      982 2022-10-21 14:19:55.000000 fairgraph-0.8.2/fairgraph/openminds/core/research/numerical_property.py
--rw-r--r--   0 adavison   (502) staff       (20)     1018 2022-10-21 14:19:55.000000 fairgraph-0.8.2/fairgraph/openminds/core/research/property_value_list.py
--rw-r--r--   0 adavison   (502) staff       (20)     1425 2022-10-21 14:19:55.000000 fairgraph-0.8.2/fairgraph/openminds/core/research/protocol.py
--rw-r--r--   0 adavison   (502) staff       (20)     4017 2022-10-21 14:19:55.000000 fairgraph-0.8.2/fairgraph/openminds/core/research/protocol_execution.py
--rw-r--r--   0 adavison   (502) staff       (20)     1709 2022-10-21 14:19:55.000000 fairgraph-0.8.2/fairgraph/openminds/core/research/stimulation.py
--rw-r--r--   0 adavison   (502) staff       (20)     3325 2022-10-21 14:19:55.000000 fairgraph-0.8.2/fairgraph/openminds/core/research/strain.py
--rw-r--r--   0 adavison   (502) staff       (20)      899 2022-10-21 14:19:55.000000 fairgraph-0.8.2/fairgraph/openminds/core/research/string_property.py
--rw-r--r--   0 adavison   (502) staff       (20)     2155 2022-10-21 14:19:55.000000 fairgraph-0.8.2/fairgraph/openminds/core/research/subject.py
--rw-r--r--   0 adavison   (502) staff       (20)     2244 2022-10-21 14:19:55.000000 fairgraph-0.8.2/fairgraph/openminds/core/research/subject_group.py
--rw-r--r--   0 adavison   (502) staff       (20)     2859 2022-10-21 14:19:55.000000 fairgraph-0.8.2/fairgraph/openminds/core/research/subject_group_state.py
--rw-r--r--   0 adavison   (502) staff       (20)     2962 2022-10-21 14:19:55.000000 fairgraph-0.8.2/fairgraph/openminds/core/research/subject_state.py
--rw-r--r--   0 adavison   (502) staff       (20)     3225 2022-10-21 14:19:55.000000 fairgraph-0.8.2/fairgraph/openminds/core/research/tissue_sample.py
--rw-r--r--   0 adavison   (502) staff       (20)     3317 2022-10-21 14:19:55.000000 fairgraph-0.8.2/fairgraph/openminds/core/research/tissue_sample_collection.py
--rw-r--r--   0 adavison   (502) staff       (20)     2465 2022-10-21 14:19:55.000000 fairgraph-0.8.2/fairgraph/openminds/core/research/tissue_sample_collection_state.py
--rw-r--r--   0 adavison   (502) staff       (20)     2575 2022-10-21 14:19:55.000000 fairgraph-0.8.2/fairgraph/openminds/core/research/tissue_sample_state.py
-drwxr-xr-x   0 adavison   (502) staff       (20)        0 2022-11-08 10:15:40.789908 fairgraph-0.8.2/fairgraph/openminds/ephys/
--rw-r--r--   0 adavison   (502) staff       (20)      789 2022-10-21 14:21:42.000000 fairgraph-0.8.2/fairgraph/openminds/ephys/__init__.py
-drwxr-xr-x   0 adavison   (502) staff       (20)        0 2022-11-08 10:15:40.790626 fairgraph-0.8.2/fairgraph/openminds/ephys/activity/
--rw-r--r--   0 adavison   (502) staff       (20)        0 2022-10-21 14:19:55.000000 fairgraph-0.8.2/fairgraph/openminds/ephys/activity/__init__.py
--rw-r--r--   0 adavison   (502) staff       (20)     4639 2022-10-21 14:21:42.000000 fairgraph-0.8.2/fairgraph/openminds/ephys/activity/cell_patching.py
--rw-r--r--   0 adavison   (502) staff       (20)     4097 2022-10-21 14:21:42.000000 fairgraph-0.8.2/fairgraph/openminds/ephys/activity/electrode_placement.py
--rw-r--r--   0 adavison   (502) staff       (20)     3926 2022-10-21 14:21:42.000000 fairgraph-0.8.2/fairgraph/openminds/ephys/activity/recording_activity.py
-drwxr-xr-x   0 adavison   (502) staff       (20)        0 2022-11-08 10:15:40.792013 fairgraph-0.8.2/fairgraph/openminds/ephys/device/
--rw-r--r--   0 adavison   (502) staff       (20)        0 2022-10-21 14:21:42.000000 fairgraph-0.8.2/fairgraph/openminds/ephys/device/__init__.py
--rw-r--r--   0 adavison   (502) staff       (20)     2998 2022-10-21 14:21:42.000000 fairgraph-0.8.2/fairgraph/openminds/ephys/device/electrode.py
--rw-r--r--   0 adavison   (502) staff       (20)     2074 2022-10-21 14:21:42.000000 fairgraph-0.8.2/fairgraph/openminds/ephys/device/electrode_array.py
--rw-r--r--   0 adavison   (502) staff       (20)     2892 2022-10-21 14:21:42.000000 fairgraph-0.8.2/fairgraph/openminds/ephys/device/electrode_array_usage.py
--rw-r--r--   0 adavison   (502) staff       (20)     2796 2022-10-21 14:21:42.000000 fairgraph-0.8.2/fairgraph/openminds/ephys/device/electrode_usage.py
--rw-r--r--   0 adavison   (502) staff       (20)     2827 2022-10-21 14:21:42.000000 fairgraph-0.8.2/fairgraph/openminds/ephys/device/pipette.py
--rw-r--r--   0 adavison   (502) staff       (20)     3995 2022-10-21 14:21:42.000000 fairgraph-0.8.2/fairgraph/openminds/ephys/device/pipette_usage.py
-drwxr-xr-x   0 adavison   (502) staff       (20)        0 2022-11-08 10:15:40.792643 fairgraph-0.8.2/fairgraph/openminds/ephys/entity/
--rw-r--r--   0 adavison   (502) staff       (20)        0 2022-10-21 14:19:55.000000 fairgraph-0.8.2/fairgraph/openminds/ephys/entity/__init__.py
--rw-r--r--   0 adavison   (502) staff       (20)      972 2022-10-21 14:21:42.000000 fairgraph-0.8.2/fairgraph/openminds/ephys/entity/channel.py
--rw-r--r--   0 adavison   (502) staff       (20)     2182 2022-10-21 14:21:42.000000 fairgraph-0.8.2/fairgraph/openminds/ephys/entity/recording.py
-drwxr-xr-x   0 adavison   (502) staff       (20)        0 2022-11-08 10:15:40.795037 fairgraph-0.8.2/fairgraph/openminds/publications/
--rw-r--r--   0 adavison   (502) staff       (20)      743 2022-10-21 14:19:55.000000 fairgraph-0.8.2/fairgraph/openminds/publications/__init__.py
--rw-r--r--   0 adavison   (502) staff       (20)     4735 2022-10-21 14:21:42.000000 fairgraph-0.8.2/fairgraph/openminds/publications/book.py
--rw-r--r--   0 adavison   (502) staff       (20)     5064 2022-10-21 14:21:42.000000 fairgraph-0.8.2/fairgraph/openminds/publications/chapter.py
--rw-r--r--   0 adavison   (502) staff       (20)     2364 2022-10-21 14:21:42.000000 fairgraph-0.8.2/fairgraph/openminds/publications/live_paper.py
--rw-r--r--   0 adavison   (502) staff       (20)     1595 2022-10-21 14:21:42.000000 fairgraph-0.8.2/fairgraph/openminds/publications/live_paper_resource_item.py
--rw-r--r--   0 adavison   (502) staff       (20)     1534 2022-10-21 14:21:42.000000 fairgraph-0.8.2/fairgraph/openminds/publications/live_paper_section.py
--rw-r--r--   0 adavison   (502) staff       (20)     9083 2022-10-21 14:21:42.000000 fairgraph-0.8.2/fairgraph/openminds/publications/live_paper_version.py
--rw-r--r--   0 adavison   (502) staff       (20)     1154 2022-10-21 14:21:42.000000 fairgraph-0.8.2/fairgraph/openminds/publications/periodical.py
--rw-r--r--   0 adavison   (502) staff       (20)     1025 2022-10-21 14:21:42.000000 fairgraph-0.8.2/fairgraph/openminds/publications/publication_issue.py
--rw-r--r--   0 adavison   (502) staff       (20)     1023 2022-10-21 14:21:42.000000 fairgraph-0.8.2/fairgraph/openminds/publications/publication_volume.py
--rw-r--r--   0 adavison   (502) staff       (20)     7204 2022-10-21 14:21:42.000000 fairgraph-0.8.2/fairgraph/openminds/publications/scholarly_article.py
-drwxr-xr-x   0 adavison   (502) staff       (20)        0 2022-11-08 10:15:40.795256 fairgraph-0.8.2/fairgraph/openminds/sands/
--rw-r--r--   0 adavison   (502) staff       (20)     1479 2022-10-21 14:19:55.000000 fairgraph-0.8.2/fairgraph/openminds/sands/__init__.py
-drwxr-xr-x   0 adavison   (502) staff       (20)        0 2022-11-08 10:15:40.797009 fairgraph-0.8.2/fairgraph/openminds/sands/atlas/
--rw-r--r--   0 adavison   (502) staff       (20)        0 2022-10-21 14:19:55.000000 fairgraph-0.8.2/fairgraph/openminds/sands/atlas/__init__.py
--rw-r--r--   0 adavison   (502) staff       (20)     2348 2022-10-21 14:19:55.000000 fairgraph-0.8.2/fairgraph/openminds/sands/atlas/atlas_annotation.py
--rw-r--r--   0 adavison   (502) staff       (20)     2836 2022-10-21 14:19:55.000000 fairgraph-0.8.2/fairgraph/openminds/sands/atlas/brain_atlas.py
--rw-r--r--   0 adavison   (502) staff       (20)     9411 2022-10-21 14:21:42.000000 fairgraph-0.8.2/fairgraph/openminds/sands/atlas/brain_atlas_version.py
--rw-r--r--   0 adavison   (502) staff       (20)     3337 2022-10-21 14:19:55.000000 fairgraph-0.8.2/fairgraph/openminds/sands/atlas/common_coordinate_space.py
--rw-r--r--   0 adavison   (502) staff       (20)     2092 2022-10-21 14:19:55.000000 fairgraph-0.8.2/fairgraph/openminds/sands/atlas/parcellation_entity.py
--rw-r--r--   0 adavison   (502) staff       (20)     2745 2022-10-21 14:19:55.000000 fairgraph-0.8.2/fairgraph/openminds/sands/atlas/parcellation_entity_version.py
--rw-r--r--   0 adavison   (502) staff       (20)     1189 2022-10-21 14:19:55.000000 fairgraph-0.8.2/fairgraph/openminds/sands/atlas/parcellation_terminology.py
--rw-r--r--   0 adavison   (502) staff       (20)     1236 2022-10-21 14:19:55.000000 fairgraph-0.8.2/fairgraph/openminds/sands/atlas/parcellation_terminology_version.py
-drwxr-xr-x   0 adavison   (502) staff       (20)        0 2022-11-08 10:15:40.797788 fairgraph-0.8.2/fairgraph/openminds/sands/mathematicalShapes/
--rw-r--r--   0 adavison   (502) staff       (20)        0 2022-10-21 14:19:55.000000 fairgraph-0.8.2/fairgraph/openminds/sands/mathematicalShapes/__init__.py
--rw-r--r--   0 adavison   (502) staff       (20)      795 2022-10-21 14:19:55.000000 fairgraph-0.8.2/fairgraph/openminds/sands/mathematicalShapes/circle.py
--rw-r--r--   0 adavison   (502) staff       (20)     1010 2022-10-21 14:19:55.000000 fairgraph-0.8.2/fairgraph/openminds/sands/mathematicalShapes/ellipse.py
--rw-r--r--   0 adavison   (502) staff       (20)      961 2022-10-21 14:19:55.000000 fairgraph-0.8.2/fairgraph/openminds/sands/mathematicalShapes/rectangle.py
-drwxr-xr-x   0 adavison   (502) staff       (20)        0 2022-11-08 10:15:40.798773 fairgraph-0.8.2/fairgraph/openminds/sands/miscellaneous/
--rw-r--r--   0 adavison   (502) staff       (20)        0 2022-10-21 14:19:55.000000 fairgraph-0.8.2/fairgraph/openminds/sands/miscellaneous/__init__.py
--rw-r--r--   0 adavison   (502) staff       (20)     1778 2022-10-21 14:19:55.000000 fairgraph-0.8.2/fairgraph/openminds/sands/miscellaneous/anatomical_target_position.py
--rw-r--r--   0 adavison   (502) staff       (20)     1231 2022-10-21 14:19:55.000000 fairgraph-0.8.2/fairgraph/openminds/sands/miscellaneous/coordinate_point.py
--rw-r--r--   0 adavison   (502) staff       (20)     1336 2022-10-21 14:19:55.000000 fairgraph-0.8.2/fairgraph/openminds/sands/miscellaneous/qualitative_relation_assessment.py
--rw-r--r--   0 adavison   (502) staff       (20)     1290 2022-10-21 14:19:55.000000 fairgraph-0.8.2/fairgraph/openminds/sands/miscellaneous/quantitative_relation_assessment.py
-drwxr-xr-x   0 adavison   (502) staff       (20)        0 2022-11-08 10:15:40.799539 fairgraph-0.8.2/fairgraph/openminds/sands/non_atlas/
--rw-r--r--   0 adavison   (502) staff       (20)        0 2022-10-21 14:19:55.000000 fairgraph-0.8.2/fairgraph/openminds/sands/non_atlas/__init__.py
--rw-r--r--   0 adavison   (502) staff       (20)     1466 2022-10-21 14:19:55.000000 fairgraph-0.8.2/fairgraph/openminds/sands/non_atlas/custom_anatomical_entity.py
--rw-r--r--   0 adavison   (502) staff       (20)     2590 2022-10-21 14:19:55.000000 fairgraph-0.8.2/fairgraph/openminds/sands/non_atlas/custom_annotation.py
--rw-r--r--   0 adavison   (502) staff       (20)     1788 2022-10-21 14:19:55.000000 fairgraph-0.8.2/fairgraph/openminds/sands/non_atlas/custom_coordinate_space.py
--rw-r--r--   0 adavison   (502) staff       (20)    15651 2022-08-24 15:08:51.000000 fairgraph-0.8.2/fairgraph/optophysiology.py
--rw-r--r--   0 adavison   (502) staff       (20)     3725 2022-09-21 13:31:07.000000 fairgraph-0.8.2/fairgraph/queries.py
--rw-r--r--   0 adavison   (502) staff       (20)     5422 2022-09-13 12:54:33.000000 fairgraph-0.8.2/fairgraph/registry.py
--rw-r--r--   0 adavison   (502) staff       (20)     7555 2022-08-24 15:08:51.000000 fairgraph-0.8.2/fairgraph/software.py
--rw-r--r--   0 adavison   (502) staff       (20)    36886 2022-08-24 15:08:51.000000 fairgraph-0.8.2/fairgraph/uniminds.py
--rw-r--r--   0 adavison   (502) staff       (20)     9666 2022-08-24 15:08:51.000000 fairgraph-0.8.2/fairgraph/utility.py
-drwxr-xr-x   0 adavison   (502) staff       (20)        0 2022-11-08 10:15:40.743142 fairgraph-0.8.2/fairgraph.egg-info/
--rw-r--r--   0 adavison   (502) staff       (20)     6919 2022-11-08 10:15:40.000000 fairgraph-0.8.2/fairgraph.egg-info/PKG-INFO
--rw-r--r--   0 adavison   (502) staff       (20)    11681 2022-11-08 10:15:40.000000 fairgraph-0.8.2/fairgraph.egg-info/SOURCES.txt
--rw-r--r--   0 adavison   (502) staff       (20)        1 2022-11-08 10:15:40.000000 fairgraph-0.8.2/fairgraph.egg-info/dependency_links.txt
--rw-r--r--   0 adavison   (502) staff       (20)       80 2022-11-08 10:15:40.000000 fairgraph-0.8.2/fairgraph.egg-info/requires.txt
--rw-r--r--   0 adavison   (502) staff       (20)       21 2022-11-08 10:15:40.000000 fairgraph-0.8.2/fairgraph.egg-info/top_level.txt
--rw-r--r--   0 adavison   (502) staff       (20)      284 2022-08-26 12:52:49.000000 fairgraph-0.8.2/requirements.txt
--rw-r--r--   0 adavison   (502) staff       (20)       38 2022-11-08 10:15:40.805039 fairgraph-0.8.2/setup.cfg
--rw-r--r--   0 adavison   (502) staff       (20)     1580 2022-11-08 09:51:47.000000 fairgraph-0.8.2/setup.py
-drwxr-xr-x   0 adavison   (502) staff       (20)        0 2022-11-08 10:15:40.804425 fairgraph-0.8.2/test/
--rw-r--r--   0 adavison   (502) staff       (20)        0 2022-03-03 13:47:15.000000 fairgraph-0.8.2/test/__init__.py
--rw-r--r--   0 adavison   (502) staff       (20)     2647 2022-03-08 13:38:34.000000 fairgraph-0.8.2/test/test_analysis.py
--rw-r--r--   0 adavison   (502) staff       (20)    19996 2022-09-13 12:54:33.000000 fairgraph-0.8.2/test/test_base.py
--rw-r--r--   0 adavison   (502) staff       (20)    10991 2022-08-24 15:08:51.000000 fairgraph-0.8.2/test/test_brainsimulation.py
--rw-r--r--   0 adavison   (502) staff       (20)      938 2022-08-26 12:52:49.000000 fairgraph-0.8.2/test/test_client.py
--rw-r--r--   0 adavison   (502) staff       (20)     1700 2022-03-08 13:38:34.000000 fairgraph-0.8.2/test/test_commons.py
--rw-r--r--   0 adavison   (502) staff       (20)     7743 2022-08-24 15:08:51.000000 fairgraph-0.8.2/test/test_core.py
--rw-r--r--   0 adavison   (502) staff       (20)    36523 2022-08-24 15:08:51.000000 fairgraph-0.8.2/test/test_electrophysiology.py
--rw-r--r--   0 adavison   (502) staff       (20)    11901 2022-03-08 13:38:34.000000 fairgraph-0.8.2/test/test_minds.py
--rw-r--r--   0 adavison   (502) staff       (20)     3854 2022-08-26 12:52:49.000000 fairgraph-0.8.2/test/test_openminds_computation.py
--rw-r--r--   0 adavison   (502) staff       (20)     9151 2022-09-21 13:31:07.000000 fairgraph-0.8.2/test/test_openminds_core.py
--rw-r--r--   0 adavison   (502) staff       (20)     9896 2022-08-26 12:52:49.000000 fairgraph-0.8.2/test/test_queries.py
--rw-r--r--   0 adavison   (502) staff       (20)     9078 2022-03-08 13:38:34.000000 fairgraph-0.8.2/test/test_software.py
--rw-r--r--   0 adavison   (502) staff       (20)    16394 2022-03-08 13:38:34.000000 fairgraph-0.8.2/test/test_uniminds.py
--rw-r--r--   0 adavison   (502) staff       (20)    14494 2022-08-24 15:08:51.000000 fairgraph-0.8.2/test/utils.py
--rw-r--r--   0 adavison   (502) staff       (20)     3813 2022-09-21 13:31:07.000000 fairgraph-0.8.2/test/utils_v3.py
+drwxr-xr-x   0 adavison   (502) staff       (20)        0 2023-02-28 20:36:45.808407 fairgraph-0.9.0/
+-rw-r--r--   0 adavison   (502) staff       (20)    10174 2022-03-03 13:47:15.000000 fairgraph-0.9.0/LICENSE.txt
+-rw-r--r--   0 adavison   (502) staff       (20)     6745 2023-02-28 20:36:45.808234 fairgraph-0.9.0/PKG-INFO
+-rw-r--r--   0 adavison   (502) staff       (20)     6063 2022-11-08 09:52:09.000000 fairgraph-0.9.0/README.md
+drwxr-xr-x   0 adavison   (502) staff       (20)        0 2023-02-28 20:36:45.744367 fairgraph-0.9.0/fairgraph/
+-rw-r--r--   0 adavison   (502) staff       (20)      973 2023-02-28 20:29:46.000000 fairgraph-0.9.0/fairgraph/__init__.py
+-rw-r--r--   0 adavison   (502) staff       (20)    13195 2023-01-11 14:12:58.000000 fairgraph-0.9.0/fairgraph/analysis.py
+-rw-r--r--   0 adavison   (502) staff       (20)    47469 2023-01-11 14:12:58.000000 fairgraph-0.9.0/fairgraph/base_v2.py
+-rw-r--r--   0 adavison   (502) staff       (20)    56597 2023-02-28 20:20:22.000000 fairgraph-0.9.0/fairgraph/base_v3.py
+-rw-r--r--   0 adavison   (502) staff       (20)    33890 2023-01-11 14:12:58.000000 fairgraph-0.9.0/fairgraph/brainsimulation.py
+-rw-r--r--   0 adavison   (502) staff       (20)    16561 2023-01-11 14:12:58.000000 fairgraph-0.9.0/fairgraph/client_v2.py
+-rw-r--r--   0 adavison   (502) staff       (20)    17027 2023-02-28 20:30:00.000000 fairgraph-0.9.0/fairgraph/client_v3.py
+-rw-r--r--   0 adavison   (502) staff       (20)    32828 2023-01-11 14:12:58.000000 fairgraph-0.9.0/fairgraph/commons.py
+-rw-r--r--   0 adavison   (502) staff       (20)     2419 2023-01-11 14:12:58.000000 fairgraph-0.9.0/fairgraph/computing.py
+-rw-r--r--   0 adavison   (502) staff       (20)    17120 2023-01-11 14:12:58.000000 fairgraph-0.9.0/fairgraph/core.py
+-rw-r--r--   0 adavison   (502) staff       (20)     2569 2023-01-11 14:12:58.000000 fairgraph-0.9.0/fairgraph/data.py
+-rw-r--r--   0 adavison   (502) staff       (20)    58899 2023-01-11 14:12:58.000000 fairgraph-0.9.0/fairgraph/electrophysiology.py
+-rw-r--r--   0 adavison   (502) staff       (20)      486 2023-01-24 13:32:28.000000 fairgraph-0.9.0/fairgraph/errors.py
+-rw-r--r--   0 adavison   (502) staff       (20)    21203 2023-01-11 14:12:58.000000 fairgraph-0.9.0/fairgraph/experiment.py
+-rw-r--r--   0 adavison   (502) staff       (20)    10635 2023-01-11 14:12:58.000000 fairgraph-0.9.0/fairgraph/fields.py
+-rw-r--r--   0 adavison   (502) staff       (20)    18905 2023-01-11 14:12:58.000000 fairgraph-0.9.0/fairgraph/livepapers.py
+-rw-r--r--   0 adavison   (502) staff       (20)    32171 2023-01-11 14:12:58.000000 fairgraph-0.9.0/fairgraph/minds.py
+-rw-r--r--   0 adavison   (502) staff       (20)    11552 2023-01-11 14:12:58.000000 fairgraph-0.9.0/fairgraph/morphology.py
+drwxr-xr-x   0 adavison   (502) staff       (20)        0 2023-02-28 20:36:45.745507 fairgraph-0.9.0/fairgraph/openminds/
+-rw-r--r--   0 adavison   (502) staff       (20)      115 2022-12-22 17:48:40.000000 fairgraph-0.9.0/fairgraph/openminds/__init__.py
+drwxr-xr-x   0 adavison   (502) staff       (20)        0 2023-02-28 20:36:45.746672 fairgraph-0.9.0/fairgraph/openminds/chemicals/
+-rw-r--r--   0 adavison   (502) staff       (20)      505 2023-01-11 14:12:58.000000 fairgraph-0.9.0/fairgraph/openminds/chemicals/__init__.py
+-rw-r--r--   0 adavison   (502) staff       (20)     1249 2023-01-11 14:12:58.000000 fairgraph-0.9.0/fairgraph/openminds/chemicals/amount_of_chemical.py
+-rw-r--r--   0 adavison   (502) staff       (20)     1748 2023-01-11 14:12:58.000000 fairgraph-0.9.0/fairgraph/openminds/chemicals/chemical_mixture.py
+-rw-r--r--   0 adavison   (502) staff       (20)     1645 2023-01-11 14:12:58.000000 fairgraph-0.9.0/fairgraph/openminds/chemicals/chemical_substance.py
+-rw-r--r--   0 adavison   (502) staff       (20)     1724 2023-01-11 14:12:58.000000 fairgraph-0.9.0/fairgraph/openminds/chemicals/product_source.py
+drwxr-xr-x   0 adavison   (502) staff       (20)        0 2023-02-28 20:36:45.749893 fairgraph-0.9.0/fairgraph/openminds/computation/
+-rw-r--r--   0 adavison   (502) staff       (20)      986 2023-01-11 14:12:58.000000 fairgraph-0.9.0/fairgraph/openminds/computation/__init__.py
+-rw-r--r--   0 adavison   (502) staff       (20)     5196 2023-01-11 14:12:58.000000 fairgraph-0.9.0/fairgraph/openminds/computation/data_analysis.py
+-rw-r--r--   0 adavison   (502) staff       (20)     1741 2023-01-11 14:12:58.000000 fairgraph-0.9.0/fairgraph/openminds/computation/environment.py
+-rw-r--r--   0 adavison   (502) staff       (20)     1259 2023-01-11 14:12:58.000000 fairgraph-0.9.0/fairgraph/openminds/computation/hardware_system.py
+-rw-r--r--   0 adavison   (502) staff       (20)     1649 2023-01-11 14:12:58.000000 fairgraph-0.9.0/fairgraph/openminds/computation/launch_configuration.py
+-rw-r--r--   0 adavison   (502) staff       (20)     2283 2023-01-11 14:12:58.000000 fairgraph-0.9.0/fairgraph/openminds/computation/local_file.py
+-rw-r--r--   0 adavison   (502) staff       (20)     5393 2023-01-11 14:12:58.000000 fairgraph-0.9.0/fairgraph/openminds/computation/model_validation.py
+-rw-r--r--   0 adavison   (502) staff       (20)     5253 2023-01-11 14:12:58.000000 fairgraph-0.9.0/fairgraph/openminds/computation/optimization.py
+-rw-r--r--   0 adavison   (502) staff       (20)     5230 2023-01-11 14:12:58.000000 fairgraph-0.9.0/fairgraph/openminds/computation/simulation.py
+-rw-r--r--   0 adavison   (502) staff       (20)     1381 2023-01-11 14:12:58.000000 fairgraph-0.9.0/fairgraph/openminds/computation/software_agent.py
+-rw-r--r--   0 adavison   (502) staff       (20)     4471 2023-01-11 14:12:58.000000 fairgraph-0.9.0/fairgraph/openminds/computation/validation_test.py
+-rw-r--r--   0 adavison   (502) staff       (20)    10365 2023-01-11 14:12:58.000000 fairgraph-0.9.0/fairgraph/openminds/computation/validation_test_version.py
+-rw-r--r--   0 adavison   (502) staff       (20)     5264 2023-01-11 14:12:58.000000 fairgraph-0.9.0/fairgraph/openminds/computation/visualization.py
+-rw-r--r--   0 adavison   (502) staff       (20)     1488 2023-01-11 14:12:58.000000 fairgraph-0.9.0/fairgraph/openminds/computation/workflow_execution.py
+-rw-r--r--   0 adavison   (502) staff       (20)     2623 2023-01-11 14:12:58.000000 fairgraph-0.9.0/fairgraph/openminds/computation/workflow_recipe.py
+-rw-r--r--   0 adavison   (502) staff       (20)     9647 2023-01-11 14:12:58.000000 fairgraph-0.9.0/fairgraph/openminds/computation/workflow_recipe_version.py
+drwxr-xr-x   0 adavison   (502) staff       (20)        0 2023-02-28 20:36:45.766162 fairgraph-0.9.0/fairgraph/openminds/controlledterms/
+-rw-r--r--   0 adavison   (502) staff       (20)     3674 2023-01-11 14:12:58.000000 fairgraph-0.9.0/fairgraph/openminds/controlledterms/__init__.py
+-rw-r--r--   0 adavison   (502) staff       (20)     3752 2023-01-11 14:12:58.000000 fairgraph-0.9.0/fairgraph/openminds/controlledterms/action_status_type.py
+-rw-r--r--   0 adavison   (502) staff       (20)     6442 2023-01-11 14:12:58.000000 fairgraph-0.9.0/fairgraph/openminds/controlledterms/age_category.py
+-rw-r--r--   0 adavison   (502) staff       (20)     6720 2023-01-11 14:12:58.000000 fairgraph-0.9.0/fairgraph/openminds/controlledterms/anatomical_axes_orientation.py
+-rw-r--r--   0 adavison   (502) staff       (20)     3028 2023-01-11 14:12:58.000000 fairgraph-0.9.0/fairgraph/openminds/controlledterms/anatomical_plane.py
+-rw-r--r--   0 adavison   (502) staff       (20)     3104 2023-01-11 14:12:58.000000 fairgraph-0.9.0/fairgraph/openminds/controlledterms/annotation_type.py
+-rw-r--r--   0 adavison   (502) staff       (20)     3406 2023-01-11 14:12:58.000000 fairgraph-0.9.0/fairgraph/openminds/controlledterms/atlas_type.py
+-rw-r--r--   0 adavison   (502) staff       (20)     2810 2023-01-11 14:12:58.000000 fairgraph-0.9.0/fairgraph/openminds/controlledterms/auditory_stimulus_type.py
+-rw-r--r--   0 adavison   (502) staff       (20)     4184 2023-01-11 14:12:58.000000 fairgraph-0.9.0/fairgraph/openminds/controlledterms/biological_order.py
+-rw-r--r--   0 adavison   (502) staff       (20)     3390 2023-01-11 14:12:58.000000 fairgraph-0.9.0/fairgraph/openminds/controlledterms/biological_sex.py
+-rw-r--r--   0 adavison   (502) staff       (20)     4542 2023-01-11 14:12:58.000000 fairgraph-0.9.0/fairgraph/openminds/controlledterms/breeding_type.py
+-rw-r--r--   0 adavison   (502) staff       (20)     3008 2023-01-11 14:12:58.000000 fairgraph-0.9.0/fairgraph/openminds/controlledterms/cell_culture_type.py
+-rw-r--r--   0 adavison   (502) staff       (20)     8582 2023-01-11 14:12:58.000000 fairgraph-0.9.0/fairgraph/openminds/controlledterms/cell_type.py
+-rw-r--r--   0 adavison   (502) staff       (20)     3844 2023-01-11 14:12:58.000000 fairgraph-0.9.0/fairgraph/openminds/controlledterms/chemical_mixture_type.py
+-rw-r--r--   0 adavison   (502) staff       (20)     3032 2023-01-11 14:12:58.000000 fairgraph-0.9.0/fairgraph/openminds/controlledterms/contribution_type.py
+-rw-r--r--   0 adavison   (502) staff       (20)     3034 2023-01-11 14:12:58.000000 fairgraph-0.9.0/fairgraph/openminds/controlledterms/cranial_window_construction_type.py
+-rw-r--r--   0 adavison   (502) staff       (20)     3438 2023-01-11 14:12:58.000000 fairgraph-0.9.0/fairgraph/openminds/controlledterms/cranial_window_reinforcement_type.py
+-rw-r--r--   0 adavison   (502) staff       (20)     2890 2023-01-11 14:12:58.000000 fairgraph-0.9.0/fairgraph/openminds/controlledterms/criteria_quality_type.py
+-rw-r--r--   0 adavison   (502) staff       (20)     9720 2023-01-11 14:12:58.000000 fairgraph-0.9.0/fairgraph/openminds/controlledterms/data_type.py
+-rw-r--r--   0 adavison   (502) staff       (20)     5648 2023-01-11 14:12:58.000000 fairgraph-0.9.0/fairgraph/openminds/controlledterms/device_type.py
+-rw-r--r--   0 adavison   (502) staff       (20)     4026 2023-01-11 14:12:58.000000 fairgraph-0.9.0/fairgraph/openminds/controlledterms/difference_measure.py
+-rw-r--r--   0 adavison   (502) staff       (20)     8970 2023-01-11 14:12:58.000000 fairgraph-0.9.0/fairgraph/openminds/controlledterms/disease.py
+-rw-r--r--   0 adavison   (502) staff       (20)     5142 2023-01-11 14:12:58.000000 fairgraph-0.9.0/fairgraph/openminds/controlledterms/disease_model.py
+-rw-r--r--   0 adavison   (502) staff       (20)     2808 2023-01-11 14:12:58.000000 fairgraph-0.9.0/fairgraph/openminds/controlledterms/educational_level.py
+-rw-r--r--   0 adavison   (502) staff       (20)     2318 2023-01-11 14:12:58.000000 fairgraph-0.9.0/fairgraph/openminds/controlledterms/electrical_stimulus_type.py
+-rw-r--r--   0 adavison   (502) staff       (20)     4056 2023-01-11 14:12:58.000000 fairgraph-0.9.0/fairgraph/openminds/controlledterms/ethics_assessment.py
+-rw-r--r--   0 adavison   (502) staff       (20)    12186 2023-01-11 14:12:58.000000 fairgraph-0.9.0/fairgraph/openminds/controlledterms/experimental_approach.py
+-rw-r--r--   0 adavison   (502) staff       (20)     3096 2023-01-11 14:12:58.000000 fairgraph-0.9.0/fairgraph/openminds/controlledterms/file_bundle_grouping.py
+-rw-r--r--   0 adavison   (502) staff       (20)     4882 2023-01-11 14:12:58.000000 fairgraph-0.9.0/fairgraph/openminds/controlledterms/file_repository_type.py
+-rw-r--r--   0 adavison   (502) staff       (20)     3714 2023-01-11 14:12:58.000000 fairgraph-0.9.0/fairgraph/openminds/controlledterms/file_usage_role.py
+-rw-r--r--   0 adavison   (502) staff       (20)     2748 2023-01-11 14:12:58.000000 fairgraph-0.9.0/fairgraph/openminds/controlledterms/genetic_strain_type.py
+-rw-r--r--   0 adavison   (502) staff       (20)     2872 2023-01-11 14:12:58.000000 fairgraph-0.9.0/fairgraph/openminds/controlledterms/gustatory_stimulus_type.py
+-rw-r--r--   0 adavison   (502) staff       (20)     4162 2023-01-11 14:12:58.000000 fairgraph-0.9.0/fairgraph/openminds/controlledterms/handedness.py
+-rw-r--r--   0 adavison   (502) staff       (20)     2834 2023-01-11 14:12:58.000000 fairgraph-0.9.0/fairgraph/openminds/controlledterms/language.py
+-rw-r--r--   0 adavison   (502) staff       (20)     2402 2023-01-11 14:12:58.000000 fairgraph-0.9.0/fairgraph/openminds/controlledterms/laterality.py
+-rw-r--r--   0 adavison   (502) staff       (20)     3272 2023-01-11 14:12:58.000000 fairgraph-0.9.0/fairgraph/openminds/controlledterms/learning_resource_type.py
+-rw-r--r--   0 adavison   (502) staff       (20)     4544 2023-01-11 14:12:58.000000 fairgraph-0.9.0/fairgraph/openminds/controlledterms/measured_quantity.py
+-rw-r--r--   0 adavison   (502) staff       (20)     4036 2023-01-11 14:12:58.000000 fairgraph-0.9.0/fairgraph/openminds/controlledterms/meta_data_model_type.py
+-rw-r--r--   0 adavison   (502) staff       (20)     5788 2023-01-11 14:12:58.000000 fairgraph-0.9.0/fairgraph/openminds/controlledterms/model_abstraction_level.py
+-rw-r--r--   0 adavison   (502) staff       (20)     3964 2023-01-11 14:12:58.000000 fairgraph-0.9.0/fairgraph/openminds/controlledterms/model_scope.py
+-rw-r--r--   0 adavison   (502) staff       (20)    12376 2023-01-11 14:12:58.000000 fairgraph-0.9.0/fairgraph/openminds/controlledterms/molecular_entity.py
+-rw-r--r--   0 adavison   (502) staff       (20)     2392 2023-01-11 14:12:58.000000 fairgraph-0.9.0/fairgraph/openminds/controlledterms/olfactory_stimulus_type.py
+-rw-r--r--   0 adavison   (502) staff       (20)     4164 2023-01-11 14:12:58.000000 fairgraph-0.9.0/fairgraph/openminds/controlledterms/operating_device.py
+-rw-r--r--   0 adavison   (502) staff       (20)     4278 2023-01-11 14:12:58.000000 fairgraph-0.9.0/fairgraph/openminds/controlledterms/operating_system.py
+-rw-r--r--   0 adavison   (502) staff       (20)     2944 2023-01-11 14:12:58.000000 fairgraph-0.9.0/fairgraph/openminds/controlledterms/optical_stimulus_type.py
+-rw-r--r--   0 adavison   (502) staff       (20)     4350 2023-01-11 14:12:58.000000 fairgraph-0.9.0/fairgraph/openminds/controlledterms/organ.py
+-rw-r--r--   0 adavison   (502) staff       (20)     3904 2023-01-11 14:12:58.000000 fairgraph-0.9.0/fairgraph/openminds/controlledterms/patch_clamp_variation.py
+-rw-r--r--   0 adavison   (502) staff       (20)     4248 2023-01-11 14:12:58.000000 fairgraph-0.9.0/fairgraph/openminds/controlledterms/preparation_type.py
+-rw-r--r--   0 adavison   (502) staff       (20)     3580 2023-01-11 14:12:58.000000 fairgraph-0.9.0/fairgraph/openminds/controlledterms/product_accessibility.py
+-rw-r--r--   0 adavison   (502) staff       (20)     6454 2023-01-11 14:12:58.000000 fairgraph-0.9.0/fairgraph/openminds/controlledterms/programming_language.py
+-rw-r--r--   0 adavison   (502) staff       (20)     3574 2023-01-11 14:12:58.000000 fairgraph-0.9.0/fairgraph/openminds/controlledterms/qualitative_overlap.py
+-rw-r--r--   0 adavison   (502) staff       (20)     2506 2023-01-11 14:12:58.000000 fairgraph-0.9.0/fairgraph/openminds/controlledterms/semantic_data_type.py
+-rw-r--r--   0 adavison   (502) staff       (20)     5608 2023-01-11 14:12:58.000000 fairgraph-0.9.0/fairgraph/openminds/controlledterms/service.py
+-rw-r--r--   0 adavison   (502) staff       (20)     2916 2023-01-11 14:12:58.000000 fairgraph-0.9.0/fairgraph/openminds/controlledterms/setup_type.py
+-rw-r--r--   0 adavison   (502) staff       (20)     3762 2023-01-11 14:12:58.000000 fairgraph-0.9.0/fairgraph/openminds/controlledterms/software_application_category.py
+-rw-r--r--   0 adavison   (502) staff       (20)     6480 2023-01-11 14:12:58.000000 fairgraph-0.9.0/fairgraph/openminds/controlledterms/software_feature.py
+-rw-r--r--   0 adavison   (502) staff       (20)     8608 2023-01-11 14:12:58.000000 fairgraph-0.9.0/fairgraph/openminds/controlledterms/species.py
+-rw-r--r--   0 adavison   (502) staff       (20)     4124 2023-01-11 14:12:58.000000 fairgraph-0.9.0/fairgraph/openminds/controlledterms/stimulation_approach.py
+-rw-r--r--   0 adavison   (502) staff       (20)     6930 2023-01-11 14:12:58.000000 fairgraph-0.9.0/fairgraph/openminds/controlledterms/stimulation_technique.py
+-rw-r--r--   0 adavison   (502) staff       (20)     9440 2023-01-11 14:12:58.000000 fairgraph-0.9.0/fairgraph/openminds/controlledterms/subcellular_entity.py
+-rw-r--r--   0 adavison   (502) staff       (20)     7920 2023-01-11 14:12:58.000000 fairgraph-0.9.0/fairgraph/openminds/controlledterms/subject_attribute.py
+-rw-r--r--   0 adavison   (502) staff       (20)     2468 2023-01-11 14:12:58.000000 fairgraph-0.9.0/fairgraph/openminds/controlledterms/tactile_stimulus_type.py
+-rw-r--r--   0 adavison   (502) staff       (20)     8716 2023-01-11 14:12:58.000000 fairgraph-0.9.0/fairgraph/openminds/controlledterms/technique.py
+-rw-r--r--   0 adavison   (502) staff       (20)     2469 2023-01-11 14:12:58.000000 fairgraph-0.9.0/fairgraph/openminds/controlledterms/term_suggestion.py
+-rw-r--r--   0 adavison   (502) staff       (20)     4916 2023-01-11 14:12:58.000000 fairgraph-0.9.0/fairgraph/openminds/controlledterms/terminology.py
+-rw-r--r--   0 adavison   (502) staff       (20)     4804 2023-01-11 14:12:58.000000 fairgraph-0.9.0/fairgraph/openminds/controlledterms/tissue_sample_attribute.py
+-rw-r--r--   0 adavison   (502) staff       (20)     6008 2023-01-11 14:12:58.000000 fairgraph-0.9.0/fairgraph/openminds/controlledterms/tissue_sample_type.py
+-rw-r--r--   0 adavison   (502) staff       (20)     2380 2023-01-11 14:12:58.000000 fairgraph-0.9.0/fairgraph/openminds/controlledterms/type_of_uncertainty.py
+-rw-r--r--   0 adavison   (502) staff       (20)    10404 2023-01-11 14:12:58.000000 fairgraph-0.9.0/fairgraph/openminds/controlledterms/uberon_parcellation.py
+-rw-r--r--   0 adavison   (502) staff       (20)     7570 2023-01-11 14:12:58.000000 fairgraph-0.9.0/fairgraph/openminds/controlledterms/unit_of_measurement.py
+-rw-r--r--   0 adavison   (502) staff       (20)     2832 2023-01-11 14:12:58.000000 fairgraph-0.9.0/fairgraph/openminds/controlledterms/visual_stimulus_type.py
+drwxr-xr-x   0 adavison   (502) staff       (20)        0 2023-02-28 20:36:45.766356 fairgraph-0.9.0/fairgraph/openminds/core/
+-rw-r--r--   0 adavison   (502) staff       (20)     3511 2023-01-11 14:12:58.000000 fairgraph-0.9.0/fairgraph/openminds/core/__init__.py
+drwxr-xr-x   0 adavison   (502) staff       (20)        0 2023-02-28 20:36:45.767800 fairgraph-0.9.0/fairgraph/openminds/core/actors/
+-rw-r--r--   0 adavison   (502) staff       (20)        0 2022-12-22 17:48:40.000000 fairgraph-0.9.0/fairgraph/openminds/core/actors/__init__.py
+-rw-r--r--   0 adavison   (502) staff       (20)     1083 2023-01-11 14:12:58.000000 fairgraph-0.9.0/fairgraph/openminds/core/actors/account_information.py
+-rw-r--r--   0 adavison   (502) staff       (20)     1373 2023-01-11 14:12:58.000000 fairgraph-0.9.0/fairgraph/openminds/core/actors/affiliation.py
+-rw-r--r--   0 adavison   (502) staff       (20)     1651 2023-01-11 14:12:58.000000 fairgraph-0.9.0/fairgraph/openminds/core/actors/consortium.py
+-rw-r--r--   0 adavison   (502) staff       (20)      949 2023-01-11 14:12:58.000000 fairgraph-0.9.0/fairgraph/openminds/core/actors/contact_information.py
+-rw-r--r--   0 adavison   (502) staff       (20)     1223 2023-01-11 14:12:58.000000 fairgraph-0.9.0/fairgraph/openminds/core/actors/contribution.py
+-rw-r--r--   0 adavison   (502) staff       (20)     1823 2023-01-11 14:12:58.000000 fairgraph-0.9.0/fairgraph/openminds/core/actors/organization.py
+-rw-r--r--   0 adavison   (502) staff       (20)     2767 2023-01-12 10:59:37.000000 fairgraph-0.9.0/fairgraph/openminds/core/actors/person.py
+drwxr-xr-x   0 adavison   (502) staff       (20)        0 2023-02-28 20:36:45.772102 fairgraph-0.9.0/fairgraph/openminds/core/data/
+-rw-r--r--   0 adavison   (502) staff       (20)        0 2022-12-22 17:48:40.000000 fairgraph-0.9.0/fairgraph/openminds/core/data/__init__.py
+-rw-r--r--   0 adavison   (502) staff       (20)     2283 2023-01-11 14:12:58.000000 fairgraph-0.9.0/fairgraph/openminds/core/data/content_type.py
+-rw-r--r--   0 adavison   (502) staff       (20)     1085 2023-01-11 14:12:58.000000 fairgraph-0.9.0/fairgraph/openminds/core/data/content_type_pattern.py
+-rw-r--r--   0 adavison   (502) staff       (20)     1151 2023-01-11 14:12:58.000000 fairgraph-0.9.0/fairgraph/openminds/core/data/copyright.py
+-rw-r--r--   0 adavison   (502) staff       (20)     4987 2023-01-11 14:12:58.000000 fairgraph-0.9.0/fairgraph/openminds/core/data/file.py
+-rw-r--r--   0 adavison   (502) staff       (20)     1285 2023-01-11 14:12:58.000000 fairgraph-0.9.0/fairgraph/openminds/core/data/file_archive.py
+-rw-r--r--   0 adavison   (502) staff       (20)     2783 2023-01-11 14:12:58.000000 fairgraph-0.9.0/fairgraph/openminds/core/data/file_bundle.py
+-rw-r--r--   0 adavison   (502) staff       (20)      905 2023-01-11 14:12:58.000000 fairgraph-0.9.0/fairgraph/openminds/core/data/file_path_pattern.py
+-rw-r--r--   0 adavison   (502) staff       (20)     2634 2023-01-11 14:12:58.000000 fairgraph-0.9.0/fairgraph/openminds/core/data/file_repository.py
+-rw-r--r--   0 adavison   (502) staff       (20)      987 2023-01-11 14:12:58.000000 fairgraph-0.9.0/fairgraph/openminds/core/data/file_repository_structure.py
+-rw-r--r--   0 adavison   (502) staff       (20)     1021 2023-01-11 14:12:58.000000 fairgraph-0.9.0/fairgraph/openminds/core/data/hash.py
+-rw-r--r--   0 adavison   (502) staff       (20)     1427 2023-01-11 14:12:58.000000 fairgraph-0.9.0/fairgraph/openminds/core/data/license.py
+-rw-r--r--   0 adavison   (502) staff       (20)     1744 2023-01-11 14:12:58.000000 fairgraph-0.9.0/fairgraph/openminds/core/data/measurement.py
+-rw-r--r--   0 adavison   (502) staff       (20)     1662 2023-01-11 14:12:58.000000 fairgraph-0.9.0/fairgraph/openminds/core/data/service_link.py
+drwxr-xr-x   0 adavison   (502) staff       (20)        0 2023-02-28 20:36:45.775725 fairgraph-0.9.0/fairgraph/openminds/core/miscellaneous/
+-rw-r--r--   0 adavison   (502) staff       (20)        0 2022-12-22 17:48:40.000000 fairgraph-0.9.0/fairgraph/openminds/core/miscellaneous/__init__.py
+-rw-r--r--   0 adavison   (502) staff       (20)     1989 2023-01-11 14:12:58.000000 fairgraph-0.9.0/fairgraph/openminds/core/miscellaneous/comment.py
+-rw-r--r--   0 adavison   (502) staff       (20)     1045 2023-01-11 14:12:58.000000 fairgraph-0.9.0/fairgraph/openminds/core/miscellaneous/doi.py
+-rw-r--r--   0 adavison   (502) staff       (20)     1575 2023-01-11 14:12:58.000000 fairgraph-0.9.0/fairgraph/openminds/core/miscellaneous/funding.py
+-rw-r--r--   0 adavison   (502) staff       (20)      909 2023-01-11 14:12:58.000000 fairgraph-0.9.0/fairgraph/openminds/core/miscellaneous/gridid.py
+-rw-r--r--   0 adavison   (502) staff       (20)     1067 2023-01-11 14:12:58.000000 fairgraph-0.9.0/fairgraph/openminds/core/miscellaneous/handle.py
+-rw-r--r--   0 adavison   (502) staff       (20)      934 2023-01-11 14:12:58.000000 fairgraph-0.9.0/fairgraph/openminds/core/miscellaneous/isbn.py
+-rw-r--r--   0 adavison   (502) staff       (20)      938 2023-01-11 14:12:58.000000 fairgraph-0.9.0/fairgraph/openminds/core/miscellaneous/issn.py
+-rw-r--r--   0 adavison   (502) staff       (20)      980 2023-01-11 14:12:58.000000 fairgraph-0.9.0/fairgraph/openminds/core/miscellaneous/orcid.py
+-rw-r--r--   0 adavison   (502) staff       (20)     1438 2023-01-11 14:12:58.000000 fairgraph-0.9.0/fairgraph/openminds/core/miscellaneous/quantitative_value.py
+-rw-r--r--   0 adavison   (502) staff       (20)     1711 2023-01-11 14:12:58.000000 fairgraph-0.9.0/fairgraph/openminds/core/miscellaneous/quantitative_value_array.py
+-rw-r--r--   0 adavison   (502) staff       (20)     1373 2023-01-11 14:12:58.000000 fairgraph-0.9.0/fairgraph/openminds/core/miscellaneous/quantitative_value_range.py
+-rw-r--r--   0 adavison   (502) staff       (20)      994 2023-01-11 14:12:58.000000 fairgraph-0.9.0/fairgraph/openminds/core/miscellaneous/rorid.py
+-rw-r--r--   0 adavison   (502) staff       (20)      989 2023-01-11 14:12:58.000000 fairgraph-0.9.0/fairgraph/openminds/core/miscellaneous/rrid.py
+-rw-r--r--   0 adavison   (502) staff       (20)      900 2023-01-11 14:12:58.000000 fairgraph-0.9.0/fairgraph/openminds/core/miscellaneous/stock_number.py
+-rw-r--r--   0 adavison   (502) staff       (20)      792 2023-01-11 14:12:58.000000 fairgraph-0.9.0/fairgraph/openminds/core/miscellaneous/swhid.py
+-rw-r--r--   0 adavison   (502) staff       (20)      941 2023-01-11 14:12:58.000000 fairgraph-0.9.0/fairgraph/openminds/core/miscellaneous/url.py
+drwxr-xr-x   0 adavison   (502) staff       (20)        0 2023-02-28 20:36:45.778335 fairgraph-0.9.0/fairgraph/openminds/core/products/
+-rw-r--r--   0 adavison   (502) staff       (20)        0 2022-12-22 17:48:40.000000 fairgraph-0.9.0/fairgraph/openminds/core/products/__init__.py
+-rw-r--r--   0 adavison   (502) staff       (20)     2582 2023-01-11 14:12:58.000000 fairgraph-0.9.0/fairgraph/openminds/core/products/dataset.py
+-rw-r--r--   0 adavison   (502) staff       (20)    13234 2023-02-13 15:56:26.000000 fairgraph-0.9.0/fairgraph/openminds/core/products/dataset_version.py
+-rw-r--r--   0 adavison   (502) staff       (20)     2489 2023-01-11 14:12:58.000000 fairgraph-0.9.0/fairgraph/openminds/core/products/meta_data_model.py
+-rw-r--r--   0 adavison   (502) staff       (20)     9721 2023-01-11 14:12:58.000000 fairgraph-0.9.0/fairgraph/openminds/core/products/meta_data_model_version.py
+-rw-r--r--   0 adavison   (502) staff       (20)     4260 2023-01-11 14:12:58.000000 fairgraph-0.9.0/fairgraph/openminds/core/products/model.py
+-rw-r--r--   0 adavison   (502) staff       (20)    10118 2023-01-11 14:12:58.000000 fairgraph-0.9.0/fairgraph/openminds/core/products/model_version.py
+-rw-r--r--   0 adavison   (502) staff       (20)     2416 2023-01-11 14:12:58.000000 fairgraph-0.9.0/fairgraph/openminds/core/products/project.py
+-rw-r--r--   0 adavison   (502) staff       (20)     1837 2023-01-11 14:12:58.000000 fairgraph-0.9.0/fairgraph/openminds/core/products/setup.py
+-rw-r--r--   0 adavison   (502) staff       (20)     2561 2023-01-11 14:12:58.000000 fairgraph-0.9.0/fairgraph/openminds/core/products/software.py
+-rw-r--r--   0 adavison   (502) staff       (20)    11430 2023-01-25 10:12:43.000000 fairgraph-0.9.0/fairgraph/openminds/core/products/software_version.py
+-rw-r--r--   0 adavison   (502) staff       (20)     2291 2023-01-11 14:12:58.000000 fairgraph-0.9.0/fairgraph/openminds/core/products/web_service.py
+-rw-r--r--   0 adavison   (502) staff       (20)     9557 2023-01-25 10:13:33.000000 fairgraph-0.9.0/fairgraph/openminds/core/products/web_service_version.py
+drwxr-xr-x   0 adavison   (502) staff       (20)        0 2023-02-28 20:36:45.782160 fairgraph-0.9.0/fairgraph/openminds/core/research/
+-rw-r--r--   0 adavison   (502) staff       (20)        0 2022-12-22 17:48:40.000000 fairgraph-0.9.0/fairgraph/openminds/core/research/__init__.py
+-rw-r--r--   0 adavison   (502) staff       (20)     2366 2023-01-11 14:12:58.000000 fairgraph-0.9.0/fairgraph/openminds/core/research/behavioral_protocol.py
+-rw-r--r--   0 adavison   (502) staff       (20)     1271 2023-02-06 21:03:30.000000 fairgraph-0.9.0/fairgraph/openminds/core/research/configuration.py
+-rw-r--r--   0 adavison   (502) staff       (20)     1438 2023-01-11 14:12:58.000000 fairgraph-0.9.0/fairgraph/openminds/core/research/custom_property_set.py
+-rw-r--r--   0 adavison   (502) staff       (20)     4170 2023-01-11 14:12:58.000000 fairgraph-0.9.0/fairgraph/openminds/core/research/experimental_activity.py
+-rw-r--r--   0 adavison   (502) staff       (20)     1166 2023-01-11 14:12:58.000000 fairgraph-0.9.0/fairgraph/openminds/core/research/numerical_property.py
+-rw-r--r--   0 adavison   (502) staff       (20)     1110 2023-01-11 14:12:58.000000 fairgraph-0.9.0/fairgraph/openminds/core/research/property_value_list.py
+-rw-r--r--   0 adavison   (502) staff       (20)     2050 2023-01-11 14:12:58.000000 fairgraph-0.9.0/fairgraph/openminds/core/research/protocol.py
+-rw-r--r--   0 adavison   (502) staff       (20)     4562 2023-01-11 14:12:58.000000 fairgraph-0.9.0/fairgraph/openminds/core/research/protocol_execution.py
+-rw-r--r--   0 adavison   (502) staff       (20)     3325 2023-01-11 14:12:58.000000 fairgraph-0.9.0/fairgraph/openminds/core/research/strain.py
+-rw-r--r--   0 adavison   (502) staff       (20)      899 2023-01-11 14:12:58.000000 fairgraph-0.9.0/fairgraph/openminds/core/research/string_property.py
+-rw-r--r--   0 adavison   (502) staff       (20)     2155 2023-01-11 14:12:58.000000 fairgraph-0.9.0/fairgraph/openminds/core/research/subject.py
+-rw-r--r--   0 adavison   (502) staff       (20)     2244 2023-01-11 14:12:58.000000 fairgraph-0.9.0/fairgraph/openminds/core/research/subject_group.py
+-rw-r--r--   0 adavison   (502) staff       (20)     2859 2023-01-11 14:12:58.000000 fairgraph-0.9.0/fairgraph/openminds/core/research/subject_group_state.py
+-rw-r--r--   0 adavison   (502) staff       (20)     2962 2023-01-11 14:12:58.000000 fairgraph-0.9.0/fairgraph/openminds/core/research/subject_state.py
+-rw-r--r--   0 adavison   (502) staff       (20)     3225 2023-01-11 14:12:58.000000 fairgraph-0.9.0/fairgraph/openminds/core/research/tissue_sample.py
+-rw-r--r--   0 adavison   (502) staff       (20)     3317 2023-01-11 14:12:58.000000 fairgraph-0.9.0/fairgraph/openminds/core/research/tissue_sample_collection.py
+-rw-r--r--   0 adavison   (502) staff       (20)     2465 2023-01-11 14:12:58.000000 fairgraph-0.9.0/fairgraph/openminds/core/research/tissue_sample_collection_state.py
+-rw-r--r--   0 adavison   (502) staff       (20)     2575 2023-01-11 14:12:58.000000 fairgraph-0.9.0/fairgraph/openminds/core/research/tissue_sample_state.py
+drwxr-xr-x   0 adavison   (502) staff       (20)        0 2023-02-28 20:36:45.782418 fairgraph-0.9.0/fairgraph/openminds/ephys/
+-rw-r--r--   0 adavison   (502) staff       (20)      850 2023-01-11 14:12:58.000000 fairgraph-0.9.0/fairgraph/openminds/ephys/__init__.py
+drwxr-xr-x   0 adavison   (502) staff       (20)        0 2023-02-28 20:36:45.783151 fairgraph-0.9.0/fairgraph/openminds/ephys/activity/
+-rw-r--r--   0 adavison   (502) staff       (20)        0 2022-12-22 17:48:40.000000 fairgraph-0.9.0/fairgraph/openminds/ephys/activity/__init__.py
+-rw-r--r--   0 adavison   (502) staff       (20)     5079 2023-01-11 14:12:58.000000 fairgraph-0.9.0/fairgraph/openminds/ephys/activity/cell_patching.py
+-rw-r--r--   0 adavison   (502) staff       (20)     4555 2023-01-11 14:12:58.000000 fairgraph-0.9.0/fairgraph/openminds/ephys/activity/electrode_placement.py
+-rw-r--r--   0 adavison   (502) staff       (20)     4600 2023-01-11 14:12:58.000000 fairgraph-0.9.0/fairgraph/openminds/ephys/activity/recording_activity.py
+drwxr-xr-x   0 adavison   (502) staff       (20)        0 2023-02-28 20:36:45.784631 fairgraph-0.9.0/fairgraph/openminds/ephys/device/
+-rw-r--r--   0 adavison   (502) staff       (20)        0 2022-12-22 17:48:40.000000 fairgraph-0.9.0/fairgraph/openminds/ephys/device/__init__.py
+-rw-r--r--   0 adavison   (502) staff       (20)     3047 2023-01-11 14:12:58.000000 fairgraph-0.9.0/fairgraph/openminds/ephys/device/electrode.py
+-rw-r--r--   0 adavison   (502) staff       (20)     2065 2023-01-11 14:12:58.000000 fairgraph-0.9.0/fairgraph/openminds/ephys/device/electrode_array.py
+-rw-r--r--   0 adavison   (502) staff       (20)     2319 2023-01-11 14:12:58.000000 fairgraph-0.9.0/fairgraph/openminds/ephys/device/electrode_array_usage.py
+-rw-r--r--   0 adavison   (502) staff       (20)     2154 2023-01-11 14:12:58.000000 fairgraph-0.9.0/fairgraph/openminds/ephys/device/electrode_usage.py
+-rw-r--r--   0 adavison   (502) staff       (20)     2876 2023-01-11 14:12:58.000000 fairgraph-0.9.0/fairgraph/openminds/ephys/device/pipette.py
+-rw-r--r--   0 adavison   (502) staff       (20)     3986 2023-01-11 14:12:58.000000 fairgraph-0.9.0/fairgraph/openminds/ephys/device/pipette_usage.py
+drwxr-xr-x   0 adavison   (502) staff       (20)        0 2023-02-28 20:36:45.785253 fairgraph-0.9.0/fairgraph/openminds/ephys/entity/
+-rw-r--r--   0 adavison   (502) staff       (20)        0 2022-12-22 17:48:40.000000 fairgraph-0.9.0/fairgraph/openminds/ephys/entity/__init__.py
+-rw-r--r--   0 adavison   (502) staff       (20)      972 2023-01-11 14:12:58.000000 fairgraph-0.9.0/fairgraph/openminds/ephys/entity/channel.py
+-rw-r--r--   0 adavison   (502) staff       (20)     2218 2023-01-11 14:12:58.000000 fairgraph-0.9.0/fairgraph/openminds/ephys/entity/recording.py
+drwxr-xr-x   0 adavison   (502) staff       (20)        0 2023-02-28 20:36:45.789526 fairgraph-0.9.0/fairgraph/openminds/publications/
+-rw-r--r--   0 adavison   (502) staff       (20)      791 2023-01-11 14:12:58.000000 fairgraph-0.9.0/fairgraph/openminds/publications/__init__.py
+-rw-r--r--   0 adavison   (502) staff       (20)     5172 2023-01-11 14:12:58.000000 fairgraph-0.9.0/fairgraph/openminds/publications/book.py
+-rw-r--r--   0 adavison   (502) staff       (20)     5501 2023-01-11 14:12:58.000000 fairgraph-0.9.0/fairgraph/openminds/publications/chapter.py
+-rw-r--r--   0 adavison   (502) staff       (20)     6367 2023-01-11 14:12:58.000000 fairgraph-0.9.0/fairgraph/openminds/publications/learning_resource.py
+-rw-r--r--   0 adavison   (502) staff       (20)     2422 2023-01-11 14:12:58.000000 fairgraph-0.9.0/fairgraph/openminds/publications/live_paper.py
+-rw-r--r--   0 adavison   (502) staff       (20)     1655 2023-01-11 14:19:27.000000 fairgraph-0.9.0/fairgraph/openminds/publications/live_paper_resource_item.py
+-rw-r--r--   0 adavison   (502) staff       (20)     1534 2023-01-11 14:12:58.000000 fairgraph-0.9.0/fairgraph/openminds/publications/live_paper_section.py
+-rw-r--r--   0 adavison   (502) staff       (20)     9775 2023-02-15 14:00:35.000000 fairgraph-0.9.0/fairgraph/openminds/publications/live_paper_version.py
+-rw-r--r--   0 adavison   (502) staff       (20)     1154 2023-01-11 14:12:58.000000 fairgraph-0.9.0/fairgraph/openminds/publications/periodical.py
+-rw-r--r--   0 adavison   (502) staff       (20)     1025 2023-01-11 14:12:58.000000 fairgraph-0.9.0/fairgraph/openminds/publications/publication_issue.py
+-rw-r--r--   0 adavison   (502) staff       (20)     1023 2023-01-11 14:12:58.000000 fairgraph-0.9.0/fairgraph/openminds/publications/publication_volume.py
+-rw-r--r--   0 adavison   (502) staff       (20)     7629 2023-01-25 13:38:37.000000 fairgraph-0.9.0/fairgraph/openminds/publications/scholarly_article.py
+drwxr-xr-x   0 adavison   (502) staff       (20)        0 2023-02-28 20:36:45.789803 fairgraph-0.9.0/fairgraph/openminds/sands/
+-rw-r--r--   0 adavison   (502) staff       (20)     1479 2023-01-11 14:12:58.000000 fairgraph-0.9.0/fairgraph/openminds/sands/__init__.py
+drwxr-xr-x   0 adavison   (502) staff       (20)        0 2023-02-28 20:36:45.791800 fairgraph-0.9.0/fairgraph/openminds/sands/atlas/
+-rw-r--r--   0 adavison   (502) staff       (20)        0 2022-12-22 17:48:06.000000 fairgraph-0.9.0/fairgraph/openminds/sands/atlas/__init__.py
+-rw-r--r--   0 adavison   (502) staff       (20)     2348 2023-01-11 14:12:58.000000 fairgraph-0.9.0/fairgraph/openminds/sands/atlas/atlas_annotation.py
+-rw-r--r--   0 adavison   (502) staff       (20)     3105 2023-01-11 14:12:58.000000 fairgraph-0.9.0/fairgraph/openminds/sands/atlas/brain_atlas.py
+-rw-r--r--   0 adavison   (502) staff       (20)    10258 2023-01-11 14:12:58.000000 fairgraph-0.9.0/fairgraph/openminds/sands/atlas/brain_atlas_version.py
+-rw-r--r--   0 adavison   (502) staff       (20)     3600 2023-01-11 14:12:58.000000 fairgraph-0.9.0/fairgraph/openminds/sands/atlas/common_coordinate_space.py
+-rw-r--r--   0 adavison   (502) staff       (20)     2092 2023-01-11 14:12:58.000000 fairgraph-0.9.0/fairgraph/openminds/sands/atlas/parcellation_entity.py
+-rw-r--r--   0 adavison   (502) staff       (20)     2745 2023-01-11 14:12:58.000000 fairgraph-0.9.0/fairgraph/openminds/sands/atlas/parcellation_entity_version.py
+-rw-r--r--   0 adavison   (502) staff       (20)     1189 2023-01-11 14:12:58.000000 fairgraph-0.9.0/fairgraph/openminds/sands/atlas/parcellation_terminology.py
+-rw-r--r--   0 adavison   (502) staff       (20)     1236 2023-01-11 14:12:58.000000 fairgraph-0.9.0/fairgraph/openminds/sands/atlas/parcellation_terminology_version.py
+drwxr-xr-x   0 adavison   (502) staff       (20)        0 2023-02-28 20:36:45.792695 fairgraph-0.9.0/fairgraph/openminds/sands/mathematicalShapes/
+-rw-r--r--   0 adavison   (502) staff       (20)        0 2022-12-22 17:48:06.000000 fairgraph-0.9.0/fairgraph/openminds/sands/mathematicalShapes/__init__.py
+-rw-r--r--   0 adavison   (502) staff       (20)      742 2023-01-11 14:12:58.000000 fairgraph-0.9.0/fairgraph/openminds/sands/mathematicalShapes/circle.py
+-rw-r--r--   0 adavison   (502) staff       (20)      930 2023-01-11 14:12:58.000000 fairgraph-0.9.0/fairgraph/openminds/sands/mathematicalShapes/ellipse.py
+-rw-r--r--   0 adavison   (502) staff       (20)      900 2023-01-11 14:12:58.000000 fairgraph-0.9.0/fairgraph/openminds/sands/mathematicalShapes/rectangle.py
+drwxr-xr-x   0 adavison   (502) staff       (20)        0 2023-02-28 20:36:45.793605 fairgraph-0.9.0/fairgraph/openminds/sands/miscellaneous/
+-rw-r--r--   0 adavison   (502) staff       (20)        0 2022-12-22 17:48:06.000000 fairgraph-0.9.0/fairgraph/openminds/sands/miscellaneous/__init__.py
+-rw-r--r--   0 adavison   (502) staff       (20)     1719 2023-01-11 14:12:58.000000 fairgraph-0.9.0/fairgraph/openminds/sands/miscellaneous/anatomical_target_position.py
+-rw-r--r--   0 adavison   (502) staff       (20)     1154 2023-01-11 14:12:58.000000 fairgraph-0.9.0/fairgraph/openminds/sands/miscellaneous/coordinate_point.py
+-rw-r--r--   0 adavison   (502) staff       (20)     1336 2023-01-11 14:12:58.000000 fairgraph-0.9.0/fairgraph/openminds/sands/miscellaneous/qualitative_relation_assessment.py
+-rw-r--r--   0 adavison   (502) staff       (20)     1290 2023-01-11 14:12:58.000000 fairgraph-0.9.0/fairgraph/openminds/sands/miscellaneous/quantitative_relation_assessment.py
+drwxr-xr-x   0 adavison   (502) staff       (20)        0 2023-02-28 20:36:45.794505 fairgraph-0.9.0/fairgraph/openminds/sands/non_atlas/
+-rw-r--r--   0 adavison   (502) staff       (20)        0 2022-12-22 17:48:06.000000 fairgraph-0.9.0/fairgraph/openminds/sands/non_atlas/__init__.py
+-rw-r--r--   0 adavison   (502) staff       (20)     1466 2023-01-11 14:12:58.000000 fairgraph-0.9.0/fairgraph/openminds/sands/non_atlas/custom_anatomical_entity.py
+-rw-r--r--   0 adavison   (502) staff       (20)     2590 2023-01-11 14:12:58.000000 fairgraph-0.9.0/fairgraph/openminds/sands/non_atlas/custom_annotation.py
+-rw-r--r--   0 adavison   (502) staff       (20)     1788 2023-01-11 14:12:58.000000 fairgraph-0.9.0/fairgraph/openminds/sands/non_atlas/custom_coordinate_space.py
+drwxr-xr-x   0 adavison   (502) staff       (20)        0 2023-02-28 20:36:45.794748 fairgraph-0.9.0/fairgraph/openminds/specimenprep/
+-rw-r--r--   0 adavison   (502) staff       (20)      639 2023-01-11 14:12:58.000000 fairgraph-0.9.0/fairgraph/openminds/specimenprep/__init__.py
+drwxr-xr-x   0 adavison   (502) staff       (20)        0 2023-02-28 20:36:45.795786 fairgraph-0.9.0/fairgraph/openminds/specimenprep/activity/
+-rw-r--r--   0 adavison   (502) staff       (20)        0 2022-12-22 17:48:06.000000 fairgraph-0.9.0/fairgraph/openminds/specimenprep/activity/__init__.py
+-rw-r--r--   0 adavison   (502) staff       (20)     4579 2023-01-11 14:12:58.000000 fairgraph-0.9.0/fairgraph/openminds/specimenprep/activity/cranial_window_preparation.py
+-rw-r--r--   0 adavison   (502) staff       (20)     4441 2023-01-11 14:12:58.000000 fairgraph-0.9.0/fairgraph/openminds/specimenprep/activity/tissue_culture_preparation.py
+-rw-r--r--   0 adavison   (502) staff       (20)     4662 2023-01-11 14:12:58.000000 fairgraph-0.9.0/fairgraph/openminds/specimenprep/activity/tissue_sample_slicing.py
+drwxr-xr-x   0 adavison   (502) staff       (20)        0 2023-02-28 20:36:45.796348 fairgraph-0.9.0/fairgraph/openminds/specimenprep/device/
+-rw-r--r--   0 adavison   (502) staff       (20)        0 2022-12-22 17:48:06.000000 fairgraph-0.9.0/fairgraph/openminds/specimenprep/device/__init__.py
+-rw-r--r--   0 adavison   (502) staff       (20)     2113 2023-01-11 14:12:58.000000 fairgraph-0.9.0/fairgraph/openminds/specimenprep/device/slicing_device.py
+-rw-r--r--   0 adavison   (502) staff       (20)     2082 2023-01-11 14:12:58.000000 fairgraph-0.9.0/fairgraph/openminds/specimenprep/device/slicing_device_usage.py
+drwxr-xr-x   0 adavison   (502) staff       (20)        0 2023-02-28 20:36:45.796569 fairgraph-0.9.0/fairgraph/openminds/stimulation/
+-rw-r--r--   0 adavison   (502) staff       (20)      432 2023-01-11 14:12:58.000000 fairgraph-0.9.0/fairgraph/openminds/stimulation/__init__.py
+drwxr-xr-x   0 adavison   (502) staff       (20)        0 2023-02-28 20:36:45.796940 fairgraph-0.9.0/fairgraph/openminds/stimulation/activity/
+-rw-r--r--   0 adavison   (502) staff       (20)        0 2022-12-22 17:48:40.000000 fairgraph-0.9.0/fairgraph/openminds/stimulation/activity/__init__.py
+-rw-r--r--   0 adavison   (502) staff       (20)     4459 2023-01-11 14:12:58.000000 fairgraph-0.9.0/fairgraph/openminds/stimulation/activity/stimulation_activity.py
+drwxr-xr-x   0 adavison   (502) staff       (20)        0 2023-02-28 20:36:45.797289 fairgraph-0.9.0/fairgraph/openminds/stimulation/stimulus/
+-rw-r--r--   0 adavison   (502) staff       (20)        0 2022-12-22 17:48:40.000000 fairgraph-0.9.0/fairgraph/openminds/stimulation/stimulus/__init__.py
+-rw-r--r--   0 adavison   (502) staff       (20)      839 2023-01-11 14:12:58.000000 fairgraph-0.9.0/fairgraph/openminds/stimulation/stimulus/ephys_stimulus.py
+-rw-r--r--   0 adavison   (502) staff       (20)    15651 2023-01-11 14:12:58.000000 fairgraph-0.9.0/fairgraph/optophysiology.py
+-rw-r--r--   0 adavison   (502) staff       (20)     3725 2022-12-23 09:26:10.000000 fairgraph-0.9.0/fairgraph/queries.py
+-rw-r--r--   0 adavison   (502) staff       (20)     5422 2022-12-23 09:26:10.000000 fairgraph-0.9.0/fairgraph/registry.py
+-rw-r--r--   0 adavison   (502) staff       (20)     7555 2023-01-11 14:12:58.000000 fairgraph-0.9.0/fairgraph/software.py
+-rw-r--r--   0 adavison   (502) staff       (20)    36886 2023-01-11 14:12:58.000000 fairgraph-0.9.0/fairgraph/uniminds.py
+-rw-r--r--   0 adavison   (502) staff       (20)     9666 2022-12-23 09:26:10.000000 fairgraph-0.9.0/fairgraph/utility.py
+drwxr-xr-x   0 adavison   (502) staff       (20)        0 2023-02-28 20:36:45.745356 fairgraph-0.9.0/fairgraph.egg-info/
+-rw-r--r--   0 adavison   (502) staff       (20)     6745 2023-02-28 20:36:45.000000 fairgraph-0.9.0/fairgraph.egg-info/PKG-INFO
+-rw-r--r--   0 adavison   (502) staff       (20)    13307 2023-02-28 20:36:45.000000 fairgraph-0.9.0/fairgraph.egg-info/SOURCES.txt
+-rw-r--r--   0 adavison   (502) staff       (20)        1 2023-02-28 20:36:45.000000 fairgraph-0.9.0/fairgraph.egg-info/dependency_links.txt
+-rw-r--r--   0 adavison   (502) staff       (20)       80 2023-02-28 20:36:45.000000 fairgraph-0.9.0/fairgraph.egg-info/requires.txt
+-rw-r--r--   0 adavison   (502) staff       (20)       10 2023-02-28 20:36:45.000000 fairgraph-0.9.0/fairgraph.egg-info/top_level.txt
+-rw-r--r--   0 adavison   (502) staff       (20)     1234 2023-02-28 20:28:14.000000 fairgraph-0.9.0/pyproject.toml
+-rw-r--r--   0 adavison   (502) staff       (20)      284 2023-01-11 14:12:58.000000 fairgraph-0.9.0/requirements.txt
+-rw-r--r--   0 adavison   (502) staff       (20)       38 2023-02-28 20:36:45.808525 fairgraph-0.9.0/setup.cfg
+-rw-r--r--   0 adavison   (502) staff       (20)       39 2022-12-23 09:26:10.000000 fairgraph-0.9.0/setup.py
+drwxr-xr-x   0 adavison   (502) staff       (20)        0 2023-02-28 20:36:45.807940 fairgraph-0.9.0/test/
+-rw-r--r--   0 adavison   (502) staff       (20)        0 2022-03-03 13:47:15.000000 fairgraph-0.9.0/test/__init__.py
+-rw-r--r--   0 adavison   (502) staff       (20)     2647 2023-01-11 14:12:58.000000 fairgraph-0.9.0/test/test_analysis.py
+-rw-r--r--   0 adavison   (502) staff       (20)    19996 2023-01-11 14:12:58.000000 fairgraph-0.9.0/test/test_base.py
+-rw-r--r--   0 adavison   (502) staff       (20)    10991 2023-01-11 14:12:58.000000 fairgraph-0.9.0/test/test_brainsimulation.py
+-rw-r--r--   0 adavison   (502) staff       (20)     1503 2023-01-11 14:12:58.000000 fairgraph-0.9.0/test/test_client.py
+-rw-r--r--   0 adavison   (502) staff       (20)     1700 2023-01-11 14:12:58.000000 fairgraph-0.9.0/test/test_commons.py
+-rw-r--r--   0 adavison   (502) staff       (20)     7743 2023-01-11 14:12:58.000000 fairgraph-0.9.0/test/test_core.py
+-rw-r--r--   0 adavison   (502) staff       (20)    36523 2023-01-11 14:12:58.000000 fairgraph-0.9.0/test/test_electrophysiology.py
+-rw-r--r--   0 adavison   (502) staff       (20)     4402 2023-01-11 14:09:42.000000 fairgraph-0.9.0/test/test_fields.py
+-rw-r--r--   0 adavison   (502) staff       (20)    11901 2023-01-11 14:12:58.000000 fairgraph-0.9.0/test/test_minds.py
+-rw-r--r--   0 adavison   (502) staff       (20)     3854 2023-01-11 14:12:58.000000 fairgraph-0.9.0/test/test_openminds_computation.py
+-rw-r--r--   0 adavison   (502) staff       (20)    10848 2023-01-11 14:12:58.000000 fairgraph-0.9.0/test/test_openminds_core.py
+-rw-r--r--   0 adavison   (502) staff       (20)     9880 2023-01-11 14:45:44.000000 fairgraph-0.9.0/test/test_queries.py
+-rw-r--r--   0 adavison   (502) staff       (20)     9078 2023-01-11 14:12:58.000000 fairgraph-0.9.0/test/test_software.py
+-rw-r--r--   0 adavison   (502) staff       (20)    16394 2023-01-11 14:12:58.000000 fairgraph-0.9.0/test/test_uniminds.py
+-rw-r--r--   0 adavison   (502) staff       (20)     3813 2023-01-11 14:12:58.000000 fairgraph-0.9.0/test/utils_v3.py
```

### Comparing `fairgraph-0.8.2/LICENSE.txt` & `fairgraph-0.9.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `fairgraph-0.8.2/PKG-INFO` & `fairgraph-0.9.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,21 @@
 Metadata-Version: 2.1
 Name: fairgraph
-Version: 0.8.2
+Version: 0.9.0
 Summary: Python API for the Human Brain Project Knowledge Graph
-Home-page: https://github.com/HumanBrainProject/fairgraph
-Author: Andrew P. Davison
-Author-email: andrew.davison@cnrs.fr
-License: UNKNOWN
-Keywords: ebrains hbp metadata electrophysiology knowledge-graph
-Platform: UNKNOWN
+Author-email: "Andrew P. Davison" <andrew.davison@cnrs.fr>
+License: Apache Software License
+Project-URL: Homepage, https://github.com/HumanBrainProject/fairgraph
+Keywords: ebrains,hbp,metadata,electrophysiology,knowledge-graph
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # fairgraph: a Python API for the EBRAINS Knowledge Graph.
 
 Authors: Andrew P. Davison, Onur Ates, Nico Feld, Yann Zerlaut, Glynis Mattheisen
 
@@ -179,9 +174,7 @@
 please open a ticket in the [issue tracker](https://github.com/HumanBrainProject/fairgraph/issues).
 
 ## Acknowledgements
 
 <div><img src="https://www.braincouncil.eu/wp-content/uploads/2018/11/wsi-imageoptim-EU-Logo.jpg" alt="EU Logo" height="23%" width="15%" align="right" style="margin-left: 10px"></div>
 
 This open source software code was developed in part or in whole in the Human Brain Project, funded from the European Union's Horizon 2020 Framework Programme for Research and Innovation under Specific Grant Agreements No. 720270, No. 785907 and No. 945539 (Human Brain Project SGA1, SGA2 and SGA3).
-
-
```

### Comparing `fairgraph-0.8.2/README.md` & `fairgraph-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `fairgraph-0.8.2/fairgraph/__init__.py` & `fairgraph-0.9.0/fairgraph/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 Python client for the EBRAINS Knowledge Graph
 
-Authors: Andrew Davison et al., CNRS, 2018-2022 (see authors.rst)
+Authors: Andrew Davison et al., CNRS (see authors.rst)
 
 
-Copyright 2018-2022 CNRS
+Copyright 2018-2023 CNRS
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
 
@@ -18,13 +18,13 @@
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 import re
 from .client_v3 import KGv3Client as KGClient
 
-__version__ = "0.8.2"
+__version__ = "0.9.0"
 
 from . import (
     analysis, base_v2, base_v3, brainsimulation, client_v2, client_v3, commons, core, data,
     experiment, electrophysiology, errors, minds, optophysiology, software, uniminds, utility,
     livepapers, openminds)
```

### Comparing `fairgraph-0.8.2/fairgraph/analysis.py` & `fairgraph-0.9.0/fairgraph/analysis.py`

 * *Files identical despite different names*

### Comparing `fairgraph-0.8.2/fairgraph/base_v2.py` & `fairgraph-0.9.0/fairgraph/base_v2.py`

 * *Files identical despite different names*

### Comparing `fairgraph-0.8.2/fairgraph/base_v3.py` & `fairgraph-0.9.0/fairgraph/base_v3.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     from tabulate import tabulate
     have_tabulate = True
 except ImportError:
     have_tabulate = False
 from .utility import (compact_uri, expand_uri, as_list)
 from .registry import Registry, generate_cache_key, lookup, lookup_by_id, lookup_type, lookup_by_iri
 from .queries import QueryProperty, Query, Filter
-from .errors import ResolutionFailure
+from .errors import ResolutionFailure, AuthorizationError, ResourceExistsError
 
 
 logger = logging.getLogger("fairgraph")
 
 
 def get_filter_value(filters, field):
     value = filters[field.name]
@@ -172,15 +172,15 @@
 
         D = {
             compact_uri(key, cls.context): value
             for key, value in data.items() if key[0] != "@"
         }
         args = {}
         for field in cls.fields:
-            data_item = D.get(field.path)
+            data_item = D.get(field.path, D.get(field.alternate_path))
             args[field.name] = field.deserialize_v3(data_item, client, resolved=resolved)
         return cls(data=D, **args)
 
     def save(self, client, space=None, recursive=True, activity_log=None, replace=False):
         for field in self.fields:
             if field.intrinsic:
                 values = getattr(self, field.name)
@@ -343,14 +343,15 @@
             else:
                 raise NameError(f"""{self.__class__.__name__} does not have fields named "{'", "'.join(properties_copy)}".""")
 
         self.id = id
         self._space = space
         self.data = data
         self.scope = scope
+        self.allow_update = True
 
     def __repr__(self):
         template_parts = ("{}={{self.{}!r}}".format(field.name, field.name)
                             for field in self.fields if getattr(self, field.name) is not None)
         template = "{self.__class__.__name__}(" + ", ".join(template_parts) + ", space={self.space}, id={self.id})"
         return template.format(self=self)
 
@@ -388,15 +389,15 @@
         for otype in compact_uri(as_list(cls.type), cls.context):  # todo: update class generation to ensure classes are already compacted
             if otype not in D["@type"]:
                 #print("Warning: type mismatch {} - {}".format(otype, D["@type"]))
                 raise TypeError("type mismatch {} - {}".format(otype, D["@type"]))
         deserialized_data = {}
         for field in cls.fields:
             if field.intrinsic:
-                data_item = D.get(field.path)
+                data_item = D.get(field.path, D.get(field.alternate_path))
             else:
                 data_item = D["@id"]
             # sometimes queries put single items in a list, this removes the enclosing list
             if (not field.multiple) and isinstance(data_item, (list, tuple)) and len(data_item) == 1:
                 data_item = data_item[0]
             deserialized_data[field.name] = field.deserialize_v3(data_item, client, resolved=resolved)
         # if cls.__name__ == "ModelVersion":
@@ -513,14 +514,16 @@
                 api = "query"
             else:
                 api = "core"
 
         if api == "query":
             normalized_filters = normalize_filter(cls, filters) or None
             query = cls._get_query_definition(client, normalized_filters, space, resolved)
+            #if cls.__name__ == "DataAnalysis":
+            #    raise Exception()
             instances = client.query(
                 normalized_filters, query["@id"],
                 space=space,
                 from_index=from_index, size=size,
                 scope=scope
             ).data
             for instance in instances:
@@ -652,36 +655,48 @@
                     if cached_obj and cached_obj.data:
                         self.data = cached_obj.data  # copy or update needed?
                     return True
 
                 normalized_filters = normalize_filter(self.__class__, query_filter) or None
                 query = self.__class__._get_query_definition(client, normalized_filters, resolved=False)
                 instances = client.query(normalized_filters, query["@id"], size=1,
-                                         scope="in progress").data
+                                         scope="any").data
 
                 if instances:
                     self.id = instances[0]["@id"]
                     KGObject.save_cache[self.__class__][query_cache_key] = self.id
 
                     if self.data is None:
                         self.data = instances[0]
                     self._update(instances[0], client)
                 return bool(instances)
 
     def _updated_data(self, data):
         updated_data = {}
+        def _expand_key(key):
+            if key.startswith("@"):
+                return key
+            return expand_uri(key, {"vocab": "https://openminds.ebrains.eu/vocab/"})[0]
+
         for key, value in data.items():
-            if self.data is None or key not in self.data:
+            expanded_key = _expand_key(key)
+            if self.data is None or (key not in self.data and expanded_key not in self.data):
                 if value is not None:
                     logger.info(f"    - new field '{key}' with value {value}")  # todo: change to debug
                     updated_data[key] = value
             else:
-                existing = self.data[key]
+                existing = self.data.get(key, self.data.get(expanded_key))
                 if existing != value:
-                    if (isinstance(existing, list) and len(existing) == 0 and value is None):
+                    if (isinstance(existing, dict) and isinstance(value, dict)):
+                        expanded_value = {
+                            _expand_key(k): v for k, v in value.items()
+                        }
+                        if existing != expanded_value:
+                            updated_data[key] = value
+                    elif (isinstance(existing, list) and len(existing) == 0 and value is None):
                         # we treat empty list and None as equivalent
                         pass
                     elif (
                         isinstance(existing, list)
                         and len(existing) == 1
                         and isinstance(existing[0], dict)
                         and existing[0] == value
@@ -708,15 +723,15 @@
                                 data[field.path] = [data[field.path], serialized]
                         else:
                             data[field.path] = serialized
             return data
         else:
             raise NotImplementedError("to be implemented by child classes")
 
-    def save(self, client, space=None, recursive=True, activity_log=None, replace=False):
+    def save(self, client, space=None, recursive=True, activity_log=None, replace=False, ignore_auth_errors=False):
         if recursive:
             for field in self.fields:
                 if field.intrinsic:
                     values = getattr(self, field.name)
                     for value in as_list(values):
                         if isinstance(value, (KGObject, EmbeddedMetadata)):
                             if value.space:
@@ -737,78 +752,108 @@
         if space is None:
             if self.space is None:
                 space = self.__class__.default_space
             else:
                 space = self.space
         logger.info(f"Saving a {self.__class__.__name__} in space {space}")
         if self.exists(client):
-            # update
-            data = self._build_data(client, all_fields=True)
-            if replace:
-                logger.info(f"  - replacing - {self.__class__.__name__}(id={self.id})")
+            if not self.allow_update:
+                logger.info(f"  - not updating {self.__class__.__name__}(id={self.id}), update not allowed by user")
                 if activity_log:
-                    activity_log.update(item=self, delta=data, space=space, entry_type="replacement")
-                client.replace_instance(self.uuid, data)
+                    activity_log.update(item=self, delta=None, space=space, entry_type="no-op")
             else:
-                updated_data = self._updated_data(data)
-                if updated_data:
-                    logger.info(f"  - updating - {self.__class__.__name__}(id={self.id}) - fields changed: {updated_data.keys()}")
-                    if self.data is None:
-                        self.data = data
-                    else:
-                        self.data.update(data)
-
-                    skip_update = False
-                    if "vocab:storageSize" in updated_data:
-                        warn("Removing storage size from update because this field is currently locked by the KG")
-                        updated_data.pop("vocab:storageSize")
-                        skip_update = len(updated_data) == 0
+                # update
+                data = self._build_data(client, all_fields=True)
+                if replace:
+                    logger.info(f"  - replacing - {self.__class__.__name__}(id={self.id})")
+                    if activity_log:
+                        activity_log.update(item=self, delta=data, space=space, entry_type="replacement")
+                    try:
+                        client.replace_instance(self.uuid, data)
+                    except AuthorizationError as err:
+                        if ignore_auth_errors:
+                            logger.error(str(err))
+                        else:
+                            raise
+                else:
+                    updated_data = self._updated_data(data)
+                    if updated_data:
+                        logger.info(f"  - updating - {self.__class__.__name__}(id={self.id}) - fields changed: {updated_data.keys()}")
+                        if self.data is None:
+                            self.data = data
+                        else:
+                            self.data.update(data)
 
-                    if skip_update:
-                        if activity_log:
-                            activity_log.update(item=self, delta=None, space=space, entry_type="no-op")
+                        skip_update = False
+                        if "vocab:storageSize" in updated_data:
+                            warn("Removing storage size from update because this field is currently locked by the KG")
+                            updated_data.pop("vocab:storageSize")
+                            skip_update = len(updated_data) == 0
+
+                        if skip_update:
+                            if activity_log:
+                                activity_log.update(item=self, delta=None, space=space, entry_type="no-op")
+                        else:
+                            updated_data["@context"] = self.context
+                            try:
+                                client.update_instance(self.uuid, updated_data)
+                            except AuthorizationError as err:
+                                if ignore_auth_errors:
+                                    logger.error(str(err))
+                                else:
+                                    raise
+                            if activity_log:
+                                updated_data.pop("@context")
+                                activity_log.update(item=self, delta=updated_data, space=space, entry_type="update")
                     else:
-                        updated_data["@context"] = self.context
-                        client.update_instance(self.uuid, updated_data)
+                        logger.info(f"  - not updating {self.__class__.__name__}(id={self.id}), unchanged")
                         if activity_log:
-                            updated_data.pop("@context")
-                            activity_log.update(item=self, delta=updated_data, space=space, entry_type="update")
-                else:
-                    logger.info(f"  - not updating {self.__class__.__name__}(id={self.id}), unchanged")
-                    if activity_log:
-                        activity_log.update(item=self, delta=None, space=space, entry_type="no-op")
+                            activity_log.update(item=self, delta=None, space=space, entry_type="no-op")
         else:
             # create new
             data = self._build_data(client)
             logger.info("  - creating instance with data {}".format(data))
             data["@context"] = self.context
             data["@type"] = self.type
-            instance_data = client.create_new_instance(
-                data,
-                space or self.__class__.default_space,
-                instance_id=self.uuid)
-            self.id = instance_data["@id"]
-            self.data = instance_data
-            if activity_log:
-                activity_log.update(item=self, delta=data, space=self.space, entry_type="create")
+            try:
+                instance_data = client.create_new_instance(
+                    data,
+                    space or self.__class__.default_space,
+                    instance_id=self.uuid)
+            except (AuthorizationError, ResourceExistsError) as err:
+                if ignore_auth_errors:
+                    logger.error(str(err))
+                    if activity_log:
+                        activity_log.update(item=self, delta=data, space=self.space, entry_type="create-error")
+                else:
+                    raise
+            else:
+                self.id = instance_data["@id"]
+                self.data = instance_data
+                if activity_log:
+                    activity_log.update(item=self, delta=data, space=self.space, entry_type="create")
         # not handled yet: save existing object to new space - requires changing uuid
-        logger.debug("Updating cache for object {}. Current state: {}".format(self.id, self._build_data(client)))
-        KGObject.object_cache[self.id] = self
+        if self.id:
+            logger.debug("Updating cache for object {}. Current state: {}".format(self.id, self._build_data(client)))
+            KGObject.object_cache[self.id] = self
+        else:
+            logger.warning("Object has no id - see log for the underlying error")
 
     def delete(self, client, ignore_not_found=True):
         """Deprecate"""
         client.delete_instance(self.uuid, ignore_not_found=ignore_not_found)
         if self.id in KGObject.object_cache:
             KGObject.object_cache.pop(self.id)
 
     @classmethod
     def by_name(cls, name, client, match="equals", all=False,
                 space=None, scope="released", resolved=False):
-        # todo: implement 'match'
         objects = cls.list(client, space=space, scope=scope, resolved=resolved, api="query", name=name)
+        if match == "equals":
+            objects = [obj for obj in objects if obj.name == name]
         if len(objects) == 0:
             return None
         elif len(objects) == 1:
             return objects[0]
         elif all:
             return objects
         else:
@@ -1017,15 +1062,21 @@
                 if follow_links:
                     for child in children:
                         all_children.extend(child.children(client))
         return all_children
 
     def is_released(self, client, with_children=False):
         """Release status of the node"""
-        return client.is_released(self.id, with_children=with_children)
+        try:
+            return client.is_released(self.id, with_children=with_children)
+        except AuthorizationError:
+            # for unprivileged users
+            if "https://core.kg.ebrains.eu/vocab/meta/firstReleasedAt" in self.data:
+                return True
+            return False
 
     def release(self, client, with_children=False):
         """Release this node (make it available in public search)."""
         if not self.is_released(client, with_children=with_children):
             if with_children:
                 for child in self.children(client):
                     if not child.is_released(client, with_children=False):
@@ -1113,24 +1164,37 @@
 
     @property
     def uuid(self):
         return self.id.split("/")[-1]
 
     def delete(self, client, ignore_not_found=True):
         """Delete the instance which this proxy represents"""
-        obj = self.resolve(client, scope="in progress")
+        try:
+            obj = self.resolve(client, scope="in progress")
+        except ResolutionFailure as err:
+            logger.warning(str(err))
+            obj = None
         if obj:
             obj.delete(client, ignore_not_found=ignore_not_found)
         elif not ignore_not_found:
             raise ResolutionFailure("Couldn't resolve object to delete")
 
     def is_released(self, client, with_children=False):
         """Release status of the node"""
         return client.is_released(self.id, with_children=with_children)
 
+    def release(self, client, with_children=False):
+        """Release this node (make it available in public search)."""
+        if not self.is_released(client, with_children=with_children):
+            if with_children:
+                for child in self.children(client):
+                    if not child.is_released(client, with_children=False):
+                        client.release(child.id)
+            return client.release(self.id)
+
 
 class KGQuery(object):
     """docstring"""
 
     def __init__(self, classes, filter, preferred_scope="released"):
         self.classes = []
         for cls in as_list(classes):
```

### Comparing `fairgraph-0.8.2/fairgraph/brainsimulation.py` & `fairgraph-0.9.0/fairgraph/brainsimulation.py`

 * *Files identical despite different names*

### Comparing `fairgraph-0.8.2/fairgraph/client_v2.py` & `fairgraph-0.9.0/fairgraph/client_v2.py`

 * *Files identical despite different names*

### Comparing `fairgraph-0.8.2/fairgraph/client_v3.py` & `fairgraph-0.9.0/fairgraph/client_v3.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 define client
 """
 
-# Copyright 2018-2022 CNRS
+# Copyright 2018-2023 CNRS
 
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 
 #     http://www.apache.org/licenses/LICENSE-2.0
 
@@ -26,15 +26,15 @@
     from kg_core.kg import kg
     from kg_core.request import Stage, Pagination, ExtendedResponseConfiguration, ReleaseTreeScope
     from kg_core.response import ResultPage, JsonLdDocument
     have_v3 = True
 except ImportError:
     have_v3 = False
 
-from .errors import AuthenticationError
+from .errors import AuthenticationError, AuthorizationError, ResourceExistsError
 
 try:
     import clb_nb_utils.oauth as clb_oauth
 except ImportError:
     clb_oauth = None
 
 
@@ -97,38 +97,47 @@
 
     @property
     def _kg_admin_client(self):
         if self.__kg_admin_client is None:
             self.__kg_admin_client = self._kg_client_builder.build_admin()
         return self.__kg_admin_client
 
+    @property
+    def token(self):
+        return self._kg_client.instances._kg_config.token_handler._fetch_token()
+
     def _check_response(self, response, ignore_not_found=False, error_context=""):
         if response.error:
             # todo: handle "ignore_not_found"
             if response.error.code == 403:
-                raise AuthenticationError()
+                raise AuthorizationError(f"{response} {error_context}")
+            elif response.error.code == 401:
+                raise AuthenticationError(f"{response} {error_context}")
             elif response.error.code == 404 and ignore_not_found:
                 return response
+            elif response.error.code == 409:
+                raise ResourceExistsError(f"{response} {error_context}")
             else:
                 raise Exception(f"Error: {response.error} {error_context}")
         else:
             return response
 
     def query(self, filter, query_id, space=None, instance_id=None, from_index=0, size=100, scope="released", id_key="@id"):
 
         def _query(scope, from_index, size):
             response = self._kg_client.queries.execute_query_by_id(
                 query_id=self.uuid_from_uri(query_id),
                 additional_request_params=filter or {},
                 stage=STAGE_MAP[scope],
                 pagination=Pagination(start=from_index, size=size),
-                instance_id=instance_id
+                instance_id=instance_id,
                 #restrict_to_spaces=[space] if space else None,
             )
-            return self._check_response(response)
+            error_context = f"_query(scope={scope} space={space} query_id={query_id} filter={filter} instance_id={instance_id} size={size} from_index={from_index})"
+            return self._check_response(response, error_context=error_context)
 
         if scope == "any":
             # the following implementation is simple but very inefficient
             # because we retrieve _all_ instances and then apply the limits
             # from_index and size.
             # todo: make this more efficient, but be sure to clearly
             #       explain the algorithm
@@ -156,15 +165,16 @@
             response = self._kg_client.instances.list(
                 stage=STAGE_MAP[scope],
                 target_type=target_type,
                 space=space,
                 response_configuration=default_response_configuration,
                 pagination=Pagination(start=from_index, size=size)
             )
-            return self._check_response(response)
+            error_context = f"_list(scope={scope} space={space} target_type={target_type} size={size} from_index={from_index})"
+            return self._check_response(response, error_context=error_context)
 
         if scope == "any":
             # see comments in query() about this implementation
             instances = {}
             # first we get the released instances
             response = _list("released", 0, 100000)
             for instance in response.data:
@@ -199,20 +209,27 @@
                 except Exception as err:
                     if "404" in str(err):
                         data = None
                     else:
                         raise
                 else:
                     data = response.data
+                # in some circumstances, the KG returns "minimal" metadata,
+                # e.g. with just the id and fullName fields
+                # this means the user does not have full access, so we count this as no data
+                if data and "http://schema.org/identifier" not in data:
+                    data = None
                 return data
 
             if scope == "any":
-                data = _get_instance("in progress")
-                if data is None:
-                    data = _get_instance("released")
+                data_ip = _get_instance("in progress")
+                data_rel = _get_instance("released")
+                data = data_rel or data_ip
+                if data_ip is not None:
+                    data.update(data_ip)
             else:
                 data = _get_instance(scope)
         return data
 
     def create_new_instance(self, data, space, instance_id=None):
         if "'@id': None" in str(data):
             raise Exception("payload contains undefined ids")
@@ -234,23 +251,25 @@
 
     def update_instance(self, instance_id, data):
         response = self._kg_client.instances.contribute_to_partial_replacement(
             instance_id=instance_id,
             payload=data,
             extended_response_configuration=default_response_configuration
         )
-        return self._check_response(response).data
+        error_context = f"update_instance(data={data}, instance_id={instance_id})"
+        return self._check_response(response, error_context=error_context).data
 
     def replace_instance(self, instance_id, data):
         response = self._kg_client.instances.contribute_to_full_replacement(
             instance_id=instance_id,
             payload=data,
             extended_response_configuration=default_response_configuration
         )
-        return self._check_response(response).data
+        error_context = f"replace_instance(data={data}, instance_id={instance_id})"
+        return self._check_response(response, error_context=error_context).data
 
     def delete_instance(self, instance_id, ignore_not_found=True):
         response = self._kg_client.instances.delete(instance_id)
         # response is None if no errors
         return response
 
     def uri_from_uuid(self, uuid):
@@ -273,15 +292,15 @@
             response = self._check_response(
                 self._kg_client.queries.save_query(
                     query_id=query_id,
                     payload=query_definition,
                     space=space or "myspace"
                 )
             )
-        except AuthenticationError:
+        except AuthorizationError:
             response = self._check_response(
                 self._kg_client.queries.save_query(
                     query_id=query_id,
                     payload=query_definition,
                     space="myspace"
                 )
             )
@@ -348,19 +367,22 @@
                 return accessible_spaces
 
     @property
     def _private_space(self):
         # temporary workaround
         return f"private-{self.user_info().identifiers[0]}"
 
-    def configure_space(self, collab_id, types):
-        space_name = f"collab-{collab_id}"
+    def configure_space(self, space_name, types):
+        """
+
+        For a collab space, the space_name should be f"collab-{collab_id}"
+        """
         result = self._kg_admin_client.create_space_definition(space=space_name)
         if result:  # error
-            raise Exception(f"Unable to configure KG space for collab {collab_id}: {result}")
+            raise Exception(f"Unable to configure KG space for space '{space_name}': {result}")
         for cls in types:
             result = self._kg_admin_client.assign_type_to_space(space=space_name,
                                                                 target_type=cls.type[0])
             if result:  # error
                 raise Exception(f"Unable to assign {cls.__name__} to space {space_name}: {result}")
         return space_name
 
@@ -378,15 +400,20 @@
             release_tree_scope = ReleaseTreeScope.CHILDREN_ONLY
         else:
             release_tree_scope = ReleaseTreeScope.TOP_INSTANCE_ONLY
         response = self._kg_client.instances.get_release_status(
             instance_id=self.uuid_from_uri(uri),
             release_tree_scope=release_tree_scope
         )
-        return response.data in ("RELEASED", "HAS_CHANGED")
+        if response.data in ("RELEASED", "HAS_CHANGED"):
+            return True
+        elif response.data == "UNRELEASED":
+            return False
+        else:
+            raise AuthorizationError("You are not able to access the release status")
 
     def release(self, uri):
         """Release the node with the given uri"""
         response = self._kg_client.instances.release(self.uuid_from_uri(uri))
         if response:
             raise Exception(f"Can't release node with id {uri}. Error message: {response}")
```

### Comparing `fairgraph-0.8.2/fairgraph/commons.py` & `fairgraph-0.9.0/fairgraph/commons.py`

 * *Files identical despite different names*

### Comparing `fairgraph-0.8.2/fairgraph/computing.py` & `fairgraph-0.9.0/fairgraph/computing.py`

 * *Files identical despite different names*

### Comparing `fairgraph-0.8.2/fairgraph/core.py` & `fairgraph-0.9.0/fairgraph/core.py`

 * *Files identical despite different names*

### Comparing `fairgraph-0.8.2/fairgraph/data.py` & `fairgraph-0.9.0/fairgraph/data.py`

 * *Files identical despite different names*

### Comparing `fairgraph-0.8.2/fairgraph/electrophysiology.py` & `fairgraph-0.9.0/fairgraph/electrophysiology.py`

 * *Files identical despite different names*

### Comparing `fairgraph-0.8.2/fairgraph/experiment.py` & `fairgraph-0.9.0/fairgraph/experiment.py`

 * *Files identical despite different names*

### Comparing `fairgraph-0.8.2/fairgraph/fields.py` & `fairgraph-0.9.0/fairgraph/fields.py`

 * *Files 3% similar despite different names*

```diff
@@ -44,28 +44,29 @@
     IRI as IRIv3)
 
 
 class Field(object):
     """Representation of a metadata field"""
 
     def __init__(self, name, types, path, required=False, default=None, multiple=False,
-                 strict=False, reverse=None, doc=""):
+                 strict=False, reverse=None, doc="", alternate_path=None):
         self.name = name
         if isinstance(types, (type, str)):
             self._types = (types,)
         else:
             self._types = tuple(types)
         self._resolved_types = False
         # later, may need to use lookup() to turn strings into classes
         self.path = path
         self.required = required
         self.default = default
         self.multiple = multiple
         self.strict_mode = strict
         self.reverse = reverse
+        self.alternate_path = alternate_path  # for backwards compatibility when schemas are changed but KG not yet modified accordingly
         self.doc = doc
 
     def __repr__(self):
         return "Field(name='{}', types={}, path='{}', required={}, multiple={})".format(
             self.name, self._types, self.path, self.required, self.multiple)
 
     @property
@@ -141,22 +142,24 @@
             elif isinstance(value, (datetime, date)):
                 return value.isoformat()
             elif value is None:
                 return None
             else:
                 raise ValueError("don't know how to serialize this value")
         if isinstance(value, (list, tuple)):
-            if self.multiple:
+            if self.multiple or not self.strict_mode:
                 value = [serialize_single(item) for item in value]
                 if len(value) == 1:
                     return value[0]
                 else:
                     return value
             elif len(value) == 1:
                 return serialize_single(value[0])
+            elif self.strict_mode:
+                raise AttributeError(f"Single item expected for field {self.name} but received multiple")
             else:
                 return value
         else:
             return serialize_single(value)
 
     def deserialize(self, data, client, resolved=False):
```

### Comparing `fairgraph-0.8.2/fairgraph/livepapers.py` & `fairgraph-0.9.0/fairgraph/livepapers.py`

 * *Files identical despite different names*

### Comparing `fairgraph-0.8.2/fairgraph/minds.py` & `fairgraph-0.9.0/fairgraph/minds.py`

 * *Files identical despite different names*

### Comparing `fairgraph-0.8.2/fairgraph/morphology.py` & `fairgraph-0.9.0/fairgraph/morphology.py`

 * *Files identical despite different names*

### Comparing `fairgraph-0.8.2/fairgraph/openminds/chemicals/amount_of_chemical.py` & `fairgraph-0.9.0/fairgraph/openminds/core/data/file_archive.py`

 * *Files 21% similar despite different names*

```diff
@@ -7,28 +7,30 @@
 from datetime import date, datetime
 from fairgraph.base_v3 import KGObject, IRI
 from fairgraph.fields import Field
 
 
 
 
-class AmountOfChemical(KGObject):
+class FileArchive(KGObject):
     """
 
     """
     default_space = "dataset"
-    type = ["https://openminds.ebrains.eu/chemicals/AmountOfChemical"]
+    type = ["https://openminds.ebrains.eu/core/FileArchive"]
     context = {
         "schema": "http://schema.org/",
         "kg": "https://kg.ebrains.eu/api/instances/",
         "vocab": "https://openminds.ebrains.eu/vocab/",
         "terms": "https://openminds.ebrains.eu/controlledTerms/",
         "core": "https://openminds.ebrains.eu/core/"
     }
     fields = [
-        Field("amount", "openminds.core.QuantitativeValue", "vocab:amount", multiple=False, required=False,
-              doc="no description available"),
-        Field("chemical_product", ["openminds.chemicals.ChemicalMixture", "openminds.chemicals.ChemicalSubstance", "openminds.controlledterms.MolecularEntity"], "vocab:chemicalProduct", multiple=False, required=True,
+        Field("iri", IRI, "vocab:IRI", multiple=False, required=True,
+              doc="Stands for Internationalized Resource Identifier which is an internet protocol standard that builds on the URI protocol, extending the set of permitted characters to include Unicode/ISO 10646."),
+        Field("format", "openminds.core.ContentType", "vocab:format", multiple=False, required=True,
+              doc="Method of digitally organizing and structuring data or information."),
+        Field("source_datas", "openminds.core.File", "vocab:sourceData", multiple=True, required=False,
               doc="no description available"),
 
     ]
-    existence_query_fields = ('chemical_product',)
+    existence_query_fields = ('iri', 'format')
```

### Comparing `fairgraph-0.8.2/fairgraph/openminds/chemicals/chemical_mixture.py` & `fairgraph-0.9.0/fairgraph/openminds/chemicals/chemical_mixture.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 """
-
+Structured information about a mixture of chemical substances.
 """
 
 # this file was auto-generated
 
 from datetime import date, datetime
 from fairgraph.base_v3 import KGObject, IRI
 from fairgraph.fields import Field
 
 
 
 
 class ChemicalMixture(KGObject):
     """
-
+    Structured information about a mixture of chemical substances.
     """
-    default_space = "dataset"
+    default_space = "in-depth"
     type = ["https://openminds.ebrains.eu/chemicals/ChemicalMixture"]
     context = {
         "schema": "http://schema.org/",
         "kg": "https://kg.ebrains.eu/api/instances/",
         "vocab": "https://openminds.ebrains.eu/vocab/",
         "terms": "https://openminds.ebrains.eu/controlledTerms/",
         "core": "https://openminds.ebrains.eu/core/"
```

### Comparing `fairgraph-0.8.2/fairgraph/openminds/chemicals/chemical_substance.py` & `fairgraph-0.9.0/fairgraph/openminds/chemicals/chemical_substance.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 """
-
+Structured information about a chemical substance.
 """
 
 # this file was auto-generated
 
 from datetime import date, datetime
 from fairgraph.base_v3 import KGObject, IRI
 from fairgraph.fields import Field
 
 
 
 
 class ChemicalSubstance(KGObject):
     """
-
+    Structured information about a chemical substance.
     """
-    default_space = "dataset"
+    default_space = "in-depth"
     type = ["https://openminds.ebrains.eu/chemicals/ChemicalSubstance"]
     context = {
         "schema": "http://schema.org/",
         "kg": "https://kg.ebrains.eu/api/instances/",
         "vocab": "https://openminds.ebrains.eu/vocab/",
         "terms": "https://openminds.ebrains.eu/controlledTerms/",
         "core": "https://openminds.ebrains.eu/core/"
```

### Comparing `fairgraph-0.8.2/fairgraph/openminds/chemicals/product_source.py` & `fairgraph-0.9.0/fairgraph/openminds/chemicals/product_source.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 """
-
+Structured information about the source of a chemical substance or mixture.
 """
 
 # this file was auto-generated
 
 from datetime import date, datetime
 from fairgraph.base_v3 import KGObject, IRI
 from fairgraph.fields import Field
 
 
 
 
 class ProductSource(KGObject):
     """
-
+    Structured information about the source of a chemical substance or mixture.
     """
-    default_space = "dataset"
+    default_space = "in-depth"
     type = ["https://openminds.ebrains.eu/chemicals/ProductSource"]
     context = {
         "schema": "http://schema.org/",
         "kg": "https://kg.ebrains.eu/api/instances/",
         "vocab": "https://openminds.ebrains.eu/vocab/",
         "terms": "https://openminds.ebrains.eu/controlledTerms/",
         "core": "https://openminds.ebrains.eu/core/"
@@ -27,14 +27,14 @@
     fields = [
         Field("digital_identifier", "openminds.core.RRID", "vocab:digitalIdentifier", multiple=False, required=False,
               doc="Digital handle to identify objects or legal persons."),
         Field("identifier", str, "vocab:identifier", multiple=False, required=False,
               doc="Term or code used to identify the product source."),
         Field("product_name", str, "vocab:productName", multiple=False, required=True,
               doc="no description available"),
-        Field("provider", ["openminds.core.Organization", "openminds.core.Person"], "vocab:provider", multiple=False, required=True,
+        Field("provider", ["openminds.core.Consortium", "openminds.core.Organization", "openminds.core.Person"], "vocab:provider", multiple=False, required=True,
               doc="no description available"),
         Field("purity", ["openminds.core.QuantitativeValue", "openminds.core.QuantitativeValueRange"], "vocab:purity", multiple=False, required=False,
               doc="no description available"),
 
     ]
     existence_query_fields = ('product_name', 'provider')
```

### Comparing `fairgraph-0.8.2/fairgraph/openminds/computation/__init__.py` & `fairgraph-0.9.0/fairgraph/openminds/computation/__init__.py`

 * *Files identical despite different names*

### Comparing `fairgraph-0.8.2/fairgraph/openminds/computation/data_analysis.py` & `fairgraph-0.9.0/fairgraph/openminds/computation/model_validation.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,61 +1,65 @@
 """
-Structured information on inspecting, cleansing, transforming, and modelling data.
+Structured information about a process of validating a computational model.
 """
 
 # this file was auto-generated
 
 from datetime import date, datetime
 from fairgraph.base_v3 import KGObject, IRI
 from fairgraph.fields import Field
 
 
 
 
-class DataAnalysis(KGObject):
+class ModelValidation(KGObject):
     """
-    Structured information on inspecting, cleansing, transforming, and modelling data.
+    Structured information about a process of validating a computational model.
     """
     default_space = "computation"
-    type = ["https://openminds.ebrains.eu/computation/DataAnalysis"]
+    type = ["https://openminds.ebrains.eu/computation/ModelValidation"]
     context = {
         "schema": "http://schema.org/",
         "kg": "https://kg.ebrains.eu/api/instances/",
         "vocab": "https://openminds.ebrains.eu/vocab/",
         "terms": "https://openminds.ebrains.eu/controlledTerms/",
         "core": "https://openminds.ebrains.eu/core/"
     }
     fields = [
         Field("lookup_label", str, "vocab:lookupLabel", multiple=False, required=False,
               doc="no description available"),
         Field("custom_property_sets", "openminds.core.CustomPropertySet", "vocab:customPropertySet", multiple=True, required=False,
               doc="no description available"),
         Field("description", str, "vocab:description", multiple=False, required=False,
-              doc="Longer statement or account giving the characteristics of the data analysis."),
+              doc="Longer statement or account giving the characteristics of the model validation."),
         Field("ended_at_time", datetime, "vocab:endedAtTime", multiple=False, required=False,
               doc="no description available"),
         Field("environment", "openminds.computation.Environment", "vocab:environment", multiple=False, required=True,
               doc="no description available"),
-        Field("inputs", ["openminds.computation.LocalFile", "openminds.core.File", "openminds.core.FileBundle", "openminds.core.SoftwareVersion"], "vocab:input", multiple=True, required=True,
+        Field("inputs", ["openminds.computation.LocalFile", "openminds.computation.ValidationTestVersion", "openminds.core.File", "openminds.core.FileBundle", "openminds.core.ModelVersion", "openminds.core.SoftwareVersion"], "vocab:input", multiple=True, required=True,
               doc="Something or someone that is put into or participates in a process or machine."),
         Field("launch_configuration", "openminds.computation.LaunchConfiguration", "vocab:launchConfiguration", multiple=False, required=True,
               doc="no description available"),
         Field("outputs", ["openminds.computation.LocalFile", "openminds.core.File", "openminds.core.FileBundle"], "vocab:output", multiple=True, required=True,
               doc="Something or someone that comes out of, is delivered or produced by a process or machine."),
+        Field("performed_by", ["openminds.computation.SoftwareAgent", "openminds.core.Person"], "vocab:performedBy", multiple=True, required=False,
+              doc="no description available"),
         Field("recipe", "openminds.computation.WorkflowRecipeVersion", "vocab:recipe", multiple=False, required=False,
               doc="no description available"),
         Field("resource_usages", ["openminds.core.QuantitativeValue", "openminds.core.QuantitativeValueRange"], "vocab:resourceUsage", multiple=True, required=False,
               doc="no description available"),
+        Field("score", float, "vocab:score", multiple=False, required=False,
+              doc="no description available"),
         Field("started_at_time", datetime, "vocab:startedAtTime", multiple=False, required=True,
               doc="no description available"),
         Field("started_by", ["openminds.computation.SoftwareAgent", "openminds.core.Person"], "vocab:startedBy", multiple=False, required=False,
               doc="no description available"),
         Field("status", "openminds.controlledterms.ActionStatusType", "vocab:status", multiple=False, required=False,
               doc="no description available"),
-        Field("study_targets", ["openminds.controlledterms.BiologicalOrder", "openminds.controlledterms.BiologicalSex", "openminds.controlledterms.BreedingType", "openminds.controlledterms.CellCultureType", "openminds.controlledterms.CellType", "openminds.controlledterms.Disease", "openminds.controlledterms.DiseaseModel", "openminds.controlledterms.GeneticStrainType", "openminds.controlledterms.Handedness", "openminds.controlledterms.MolecularEntity", "openminds.controlledterms.Organ", "openminds.controlledterms.Species", "openminds.controlledterms.SubcellularEntity", "openminds.controlledterms.TermSuggestion", "openminds.controlledterms.UBERONParcellation", "openminds.sands.CustomAnatomicalEntity", "openminds.sands.ParcellationEntity", "openminds.sands.ParcellationEntityVersion"], "vocab:studyTarget", multiple=True, required=False,
+        Field("study_targets", ["openminds.controlledterms.AuditoryStimulusType", "openminds.controlledterms.BiologicalOrder", "openminds.controlledterms.BiologicalSex", "openminds.controlledterms.BreedingType", "openminds.controlledterms.CellCultureType", "openminds.controlledterms.CellType", "openminds.controlledterms.Disease", "openminds.controlledterms.DiseaseModel", "openminds.controlledterms.ElectricalStimulusType", "openminds.controlledterms.GeneticStrainType", "openminds.controlledterms.GustatoryStimulusType", "openminds.controlledterms.Handedness", "openminds.controlledterms.MolecularEntity", "openminds.controlledterms.OlfactoryStimulusType", "openminds.controlledterms.OpticalStimulusType", "openminds.controlledterms.Organ", "openminds.controlledterms.Species", "openminds.controlledterms.SubcellularEntity", "openminds.controlledterms.TactileStimulusType", "openminds.controlledterms.TermSuggestion", "openminds.controlledterms.UBERONParcellation", "openminds.controlledterms.VisualStimulusType", "openminds.sands.CustomAnatomicalEntity", "openminds.sands.ParcellationEntity", "openminds.sands.ParcellationEntityVersion"], "vocab:studyTarget", multiple=True, required=False,
               doc="Structure or function that was targeted within a study."),
         Field("tags", str, "vocab:tags", multiple=True, required=False,
               doc="no description available"),
         Field("was_informed_by", ["openminds.computation.DataAnalysis", "openminds.computation.ModelValidation", "openminds.computation.Optimization", "openminds.computation.Simulation", "openminds.computation.Visualization"], "vocab:wasInformedBy", multiple=False, required=False,
               doc="no description available"),
 
     ]
```

### Comparing `fairgraph-0.8.2/fairgraph/openminds/computation/environment.py` & `fairgraph-0.9.0/fairgraph/openminds/computation/environment.py`

 * *Files identical despite different names*

### Comparing `fairgraph-0.8.2/fairgraph/openminds/computation/hardware_system.py` & `fairgraph-0.9.0/fairgraph/openminds/computation/hardware_system.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 """
-
+Structured information about computing hardware.
 """
 
 # this file was auto-generated
 
 from datetime import date, datetime
 from fairgraph.base_v3 import KGObject, IRI
 from fairgraph.fields import Field
 
 
 
 
 class HardwareSystem(KGObject):
     """
-
+    Structured information about computing hardware.
     """
     default_space = "computation"
     type = ["https://openminds.ebrains.eu/computation/HardwareSystem"]
     context = {
         "schema": "http://schema.org/",
         "kg": "https://kg.ebrains.eu/api/instances/",
         "vocab": "https://openminds.ebrains.eu/vocab/",
```

### Comparing `fairgraph-0.8.2/fairgraph/openminds/computation/launch_configuration.py` & `fairgraph-0.9.0/fairgraph/openminds/sands/atlas/parcellation_entity.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,34 +7,40 @@
 from datetime import date, datetime
 from fairgraph.base_v3 import KGObject, IRI
 from fairgraph.fields import Field
 
 
 
 
-class LaunchConfiguration(KGObject):
+class ParcellationEntity(KGObject):
     """
 
     """
-    default_space = "computation"
-    type = ["https://openminds.ebrains.eu/computation/LaunchConfiguration"]
+    default_space = "atlas"
+    type = ["https://openminds.ebrains.eu/sands/ParcellationEntity"]
     context = {
         "schema": "http://schema.org/",
         "kg": "https://kg.ebrains.eu/api/instances/",
         "vocab": "https://openminds.ebrains.eu/vocab/",
         "terms": "https://openminds.ebrains.eu/controlledTerms/",
         "core": "https://openminds.ebrains.eu/core/"
     }
     fields = [
-        Field("name", str, "vocab:name", multiple=False, required=False,
-              doc="Word or phrase that constitutes the distinctive designation of the launch configuration."),
-        Field("arguments", str, "vocab:arguments", multiple=True, required=False,
+        Field("name", str, "vocab:name", multiple=False, required=True,
+              doc="Word or phrase that constitutes the distinctive designation of the parcellation entity."),
+        Field("lookup_label", str, "vocab:lookupLabel", multiple=False, required=False,
               doc="no description available"),
-        Field("description", str, "vocab:description", multiple=False, required=False,
-              doc="Longer statement or account giving the characteristics of the launch configuration."),
-        Field("environment_variables", "openminds.core.PropertyValueList", "vocab:environmentVariables", multiple=False, required=False,
+        Field("alternative_names", str, "vocab:alternativeName", multiple=True, required=False,
               doc="no description available"),
-        Field("executable", str, "vocab:executable", multiple=False, required=True,
+        Field("definition", str, "vocab:definition", multiple=False, required=False,
+              doc="Short, but precise statement of the meaning of a word, word group, sign or a symbol."),
+        Field("has_parents", "openminds.sands.ParcellationEntity", "vocab:hasParent", multiple=True, required=False,
+              doc="Reference to a parent object or legal person."),
+        Field("versions", "openminds.sands.ParcellationEntityVersion", "vocab:hasVersion", multiple=True, required=False,
+              doc="Reference to variants of an original."),
+        Field("ontology_identifiers", str, "vocab:ontologyIdentifier", multiple=True, required=False,
+              doc="Term or code used to identify the parcellation entity registered within a particular ontology."),
+        Field("related_uberon_term", "openminds.controlledterms.UBERONParcellation", "vocab:relatedUBERONTerm", multiple=False, required=False,
               doc="no description available"),
 
     ]
-    existence_query_fields = ('executable', 'name')
+    existence_query_fields = ('name',)
```

### Comparing `fairgraph-0.8.2/fairgraph/openminds/computation/local_file.py` & `fairgraph-0.9.0/fairgraph/openminds/computation/local_file.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 """
-
+Structured information about a file that is not accessible via a URL.
 """
 
 # this file was auto-generated
 
 from datetime import date, datetime
 from fairgraph.base_v3 import KGObject, IRI
 from fairgraph.fields import Field
 
 
 
 
 class LocalFile(KGObject):
     """
-
+    Structured information about a file that is not accessible via a URL.
     """
     default_space = "computation"
     type = ["https://openminds.ebrains.eu/computation/LocalFile"]
     context = {
         "schema": "http://schema.org/",
         "kg": "https://kg.ebrains.eu/api/instances/",
         "vocab": "https://openminds.ebrains.eu/vocab/",
```

### Comparing `fairgraph-0.8.2/fairgraph/openminds/computation/model_validation.py` & `fairgraph-0.9.0/fairgraph/openminds/computation/data_analysis.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,63 +1,63 @@
 """
-
+Structured information on inspecting, cleansing, transforming, and modelling data.
 """
 
 # this file was auto-generated
 
 from datetime import date, datetime
 from fairgraph.base_v3 import KGObject, IRI
 from fairgraph.fields import Field
 
 
 
 
-class ModelValidation(KGObject):
+class DataAnalysis(KGObject):
     """
-
+    Structured information on inspecting, cleansing, transforming, and modelling data.
     """
     default_space = "computation"
-    type = ["https://openminds.ebrains.eu/computation/ModelValidation"]
+    type = ["https://openminds.ebrains.eu/computation/DataAnalysis"]
     context = {
         "schema": "http://schema.org/",
         "kg": "https://kg.ebrains.eu/api/instances/",
         "vocab": "https://openminds.ebrains.eu/vocab/",
         "terms": "https://openminds.ebrains.eu/controlledTerms/",
         "core": "https://openminds.ebrains.eu/core/"
     }
     fields = [
         Field("lookup_label", str, "vocab:lookupLabel", multiple=False, required=False,
               doc="no description available"),
         Field("custom_property_sets", "openminds.core.CustomPropertySet", "vocab:customPropertySet", multiple=True, required=False,
               doc="no description available"),
         Field("description", str, "vocab:description", multiple=False, required=False,
-              doc="Longer statement or account giving the characteristics of the model validation."),
+              doc="Longer statement or account giving the characteristics of the data analysis."),
         Field("ended_at_time", datetime, "vocab:endedAtTime", multiple=False, required=False,
               doc="no description available"),
         Field("environment", "openminds.computation.Environment", "vocab:environment", multiple=False, required=True,
               doc="no description available"),
-        Field("inputs", ["openminds.computation.LocalFile", "openminds.computation.ValidationTestVersion", "openminds.core.File", "openminds.core.FileBundle", "openminds.core.ModelVersion", "openminds.core.SoftwareVersion"], "vocab:input", multiple=True, required=True,
+        Field("inputs", ["openminds.computation.LocalFile", "openminds.core.File", "openminds.core.FileBundle", "openminds.core.SoftwareVersion"], "vocab:input", multiple=True, required=True,
               doc="Something or someone that is put into or participates in a process or machine."),
         Field("launch_configuration", "openminds.computation.LaunchConfiguration", "vocab:launchConfiguration", multiple=False, required=True,
               doc="no description available"),
         Field("outputs", ["openminds.computation.LocalFile", "openminds.core.File", "openminds.core.FileBundle"], "vocab:output", multiple=True, required=True,
               doc="Something or someone that comes out of, is delivered or produced by a process or machine."),
+        Field("performed_by", ["openminds.computation.SoftwareAgent", "openminds.core.Person"], "vocab:performedBy", multiple=True, required=False,
+              doc="no description available"),
         Field("recipe", "openminds.computation.WorkflowRecipeVersion", "vocab:recipe", multiple=False, required=False,
               doc="no description available"),
         Field("resource_usages", ["openminds.core.QuantitativeValue", "openminds.core.QuantitativeValueRange"], "vocab:resourceUsage", multiple=True, required=False,
               doc="no description available"),
-        Field("score", float, "vocab:score", multiple=False, required=False,
-              doc="no description available"),
         Field("started_at_time", datetime, "vocab:startedAtTime", multiple=False, required=True,
               doc="no description available"),
         Field("started_by", ["openminds.computation.SoftwareAgent", "openminds.core.Person"], "vocab:startedBy", multiple=False, required=False,
               doc="no description available"),
         Field("status", "openminds.controlledterms.ActionStatusType", "vocab:status", multiple=False, required=False,
               doc="no description available"),
-        Field("study_targets", ["openminds.controlledterms.BiologicalOrder", "openminds.controlledterms.BiologicalSex", "openminds.controlledterms.BreedingType", "openminds.controlledterms.CellCultureType", "openminds.controlledterms.CellType", "openminds.controlledterms.Disease", "openminds.controlledterms.DiseaseModel", "openminds.controlledterms.GeneticStrainType", "openminds.controlledterms.Handedness", "openminds.controlledterms.MolecularEntity", "openminds.controlledterms.Organ", "openminds.controlledterms.Species", "openminds.controlledterms.SubcellularEntity", "openminds.controlledterms.TermSuggestion", "openminds.controlledterms.UBERONParcellation", "openminds.sands.CustomAnatomicalEntity", "openminds.sands.ParcellationEntity", "openminds.sands.ParcellationEntityVersion"], "vocab:studyTarget", multiple=True, required=False,
+        Field("study_targets", ["openminds.controlledterms.AuditoryStimulusType", "openminds.controlledterms.BiologicalOrder", "openminds.controlledterms.BiologicalSex", "openminds.controlledterms.BreedingType", "openminds.controlledterms.CellCultureType", "openminds.controlledterms.CellType", "openminds.controlledterms.Disease", "openminds.controlledterms.DiseaseModel", "openminds.controlledterms.ElectricalStimulusType", "openminds.controlledterms.GeneticStrainType", "openminds.controlledterms.GustatoryStimulusType", "openminds.controlledterms.Handedness", "openminds.controlledterms.MolecularEntity", "openminds.controlledterms.OlfactoryStimulusType", "openminds.controlledterms.OpticalStimulusType", "openminds.controlledterms.Organ", "openminds.controlledterms.Species", "openminds.controlledterms.SubcellularEntity", "openminds.controlledterms.TactileStimulusType", "openminds.controlledterms.TermSuggestion", "openminds.controlledterms.UBERONParcellation", "openminds.controlledterms.VisualStimulusType", "openminds.sands.CustomAnatomicalEntity", "openminds.sands.ParcellationEntity", "openminds.sands.ParcellationEntityVersion"], "vocab:studyTarget", multiple=True, required=False,
               doc="Structure or function that was targeted within a study."),
         Field("tags", str, "vocab:tags", multiple=True, required=False,
               doc="no description available"),
         Field("was_informed_by", ["openminds.computation.DataAnalysis", "openminds.computation.ModelValidation", "openminds.computation.Optimization", "openminds.computation.Simulation", "openminds.computation.Visualization"], "vocab:wasInformedBy", multiple=False, required=False,
               doc="no description available"),
 
     ]
```

### Comparing `fairgraph-0.8.2/fairgraph/openminds/computation/optimization.py` & `fairgraph-0.9.0/fairgraph/openminds/computation/validation_test.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,62 +1,56 @@
 """
-
+Structured information about the definition of a process for validating a computational model.
 """
 
 # this file was auto-generated
 
 from datetime import date, datetime
 from fairgraph.base_v3 import KGObject, IRI
 from fairgraph.fields import Field
 
 
 
 
-class Optimization(KGObject):
+class ValidationTest(KGObject):
     """
-
+    Structured information about the definition of a process for validating a computational model.
     """
     default_space = "computation"
-    type = ["https://openminds.ebrains.eu/computation/Optimization"]
+    type = ["https://openminds.ebrains.eu/computation/ValidationTest"]
     context = {
         "schema": "http://schema.org/",
         "kg": "https://kg.ebrains.eu/api/instances/",
         "vocab": "https://openminds.ebrains.eu/vocab/",
         "terms": "https://openminds.ebrains.eu/controlledTerms/",
         "core": "https://openminds.ebrains.eu/core/"
     }
     fields = [
-        Field("lookup_label", str, "vocab:lookupLabel", multiple=False, required=False,
-              doc="no description available"),
-        Field("custom_property_sets", "openminds.core.CustomPropertySet", "vocab:customPropertySet", multiple=True, required=False,
-              doc="no description available"),
-        Field("description", str, "vocab:description", multiple=False, required=False,
-              doc="Longer statement or account giving the characteristics of the optimization."),
-        Field("ended_at_time", datetime, "vocab:endedAtTime", multiple=False, required=False,
-              doc="no description available"),
-        Field("environment", "openminds.computation.Environment", "vocab:environment", multiple=False, required=True,
-              doc="no description available"),
-        Field("inputs", ["openminds.computation.LocalFile", "openminds.core.File", "openminds.core.FileBundle", "openminds.core.ModelVersion", "openminds.core.SoftwareVersion"], "vocab:input", multiple=True, required=True,
-              doc="Something or someone that is put into or participates in a process or machine."),
-        Field("launch_configuration", "openminds.computation.LaunchConfiguration", "vocab:launchConfiguration", multiple=False, required=True,
-              doc="no description available"),
-        Field("outputs", ["openminds.computation.LocalFile", "openminds.core.File", "openminds.core.FileBundle", "openminds.core.ModelVersion"], "vocab:output", multiple=True, required=True,
-              doc="Something or someone that comes out of, is delivered or produced by a process or machine."),
-        Field("recipe", "openminds.computation.WorkflowRecipeVersion", "vocab:recipe", multiple=False, required=False,
+        Field("name", str, "vocab:fullName", multiple=False, required=True,
+              doc="Whole, non-abbreviated name of the validation test."),
+        Field("alias", str, "vocab:shortName", multiple=False, required=True,
+              doc="Shortened or fully abbreviated name of the validation test."),
+        Field("custodians", ["openminds.core.Consortium", "openminds.core.Organization", "openminds.core.Person"], "vocab:custodian", multiple=True, required=False,
+              doc="The 'custodian' is a legal person who is responsible for the content and quality of the data, metadata, and/or code of a research product."),
+        Field("description", str, "vocab:description", multiple=False, required=True,
+              doc="Longer statement or account giving the characteristics of the validation test."),
+        Field("developers", ["openminds.core.Consortium", "openminds.core.Organization", "openminds.core.Person"], "vocab:developer", multiple=True, required=True,
+              doc="Legal person that creates or improves products or services (e.g., software, applications, etc.)."),
+        Field("digital_identifier", "openminds.core.DOI", "vocab:digitalIdentifier", multiple=False, required=False,
+              doc="Digital handle to identify objects or legal persons."),
+        Field("experimental_technique", "openminds.controlledterms.Technique", "vocab:experimentalTechnique", multiple=False, required=False,
+              doc="no description available"),
+        Field("versions", "openminds.computation.ValidationTestVersion", "vocab:hasVersion", multiple=True, required=True,
+              doc="Reference to variants of an original."),
+        Field("homepage", "openminds.core.URL", "vocab:homepage", multiple=False, required=False,
+              doc="Main website of the validation test."),
+        Field("how_to_cite", str, "vocab:howToCite", multiple=False, required=False,
+              doc="Preferred format for citing a particular object or legal person."),
+        Field("model_scope", "openminds.controlledterms.ModelScope", "vocab:scope", multiple=False, required=False,
+              doc="Extent of something."),
+        Field("score_type", "openminds.controlledterms.DifferenceMeasure", "vocab:scoreType", multiple=False, required=False,
               doc="no description available"),
-        Field("resource_usages", ["openminds.core.QuantitativeValue", "openminds.core.QuantitativeValueRange"], "vocab:resourceUsage", multiple=True, required=False,
-              doc="no description available"),
-        Field("started_at_time", datetime, "vocab:startedAtTime", multiple=False, required=True,
-              doc="no description available"),
-        Field("started_by", ["openminds.computation.SoftwareAgent", "openminds.core.Person"], "vocab:startedBy", multiple=False, required=False,
-              doc="no description available"),
-        Field("status", "openminds.controlledterms.ActionStatusType", "vocab:status", multiple=False, required=False,
-              doc="no description available"),
-        Field("study_targets", ["openminds.controlledterms.BiologicalOrder", "openminds.controlledterms.BiologicalSex", "openminds.controlledterms.BreedingType", "openminds.controlledterms.CellCultureType", "openminds.controlledterms.CellType", "openminds.controlledterms.Disease", "openminds.controlledterms.DiseaseModel", "openminds.controlledterms.GeneticStrainType", "openminds.controlledterms.Handedness", "openminds.controlledterms.MolecularEntity", "openminds.controlledterms.Organ", "openminds.controlledterms.Species", "openminds.controlledterms.SubcellularEntity", "openminds.controlledterms.TermSuggestion", "openminds.controlledterms.UBERONParcellation", "openminds.sands.CustomAnatomicalEntity", "openminds.sands.ParcellationEntity", "openminds.sands.ParcellationEntityVersion"], "vocab:studyTarget", multiple=True, required=False,
+        Field("study_targets", ["openminds.controlledterms.AuditoryStimulusType", "openminds.controlledterms.BiologicalOrder", "openminds.controlledterms.BiologicalSex", "openminds.controlledterms.BreedingType", "openminds.controlledterms.CellCultureType", "openminds.controlledterms.CellType", "openminds.controlledterms.Disease", "openminds.controlledterms.DiseaseModel", "openminds.controlledterms.ElectricalStimulusType", "openminds.controlledterms.GeneticStrainType", "openminds.controlledterms.GustatoryStimulusType", "openminds.controlledterms.Handedness", "openminds.controlledterms.MolecularEntity", "openminds.controlledterms.OlfactoryStimulusType", "openminds.controlledterms.OpticalStimulusType", "openminds.controlledterms.Organ", "openminds.controlledterms.Species", "openminds.controlledterms.SubcellularEntity", "openminds.controlledterms.TactileStimulusType", "openminds.controlledterms.TermSuggestion", "openminds.controlledterms.UBERONParcellation", "openminds.controlledterms.VisualStimulusType", "openminds.sands.CustomAnatomicalEntity", "openminds.sands.ParcellationEntity", "openminds.sands.ParcellationEntityVersion"], "vocab:studyTarget", multiple=True, required=False,
               doc="Structure or function that was targeted within a study."),
-        Field("tags", str, "vocab:tags", multiple=True, required=False,
-              doc="no description available"),
-        Field("was_informed_by", ["openminds.computation.DataAnalysis", "openminds.computation.ModelValidation", "openminds.computation.Optimization", "openminds.computation.Simulation", "openminds.computation.Visualization"], "vocab:wasInformedBy", multiple=False, required=False,
-              doc="no description available"),
 
     ]
-    existence_query_fields = ('lookup_label',)
+    existence_query_fields = ('name', 'alias')
```

### Comparing `fairgraph-0.8.2/fairgraph/openminds/computation/simulation.py` & `fairgraph-0.9.0/fairgraph/openminds/ephys/activity/electrode_placement.py`

 * *Files 24% similar despite different names*

```diff
@@ -7,56 +7,52 @@
 from datetime import date, datetime
 from fairgraph.base_v3 import KGObject, IRI
 from fairgraph.fields import Field
 
 
 
 
-class Simulation(KGObject):
+class ElectrodePlacement(KGObject):
     """
 
     """
-    default_space = "computation"
-    type = ["https://openminds.ebrains.eu/computation/Simulation"]
+    default_space = "in-depth"
+    type = ["https://openminds.ebrains.eu/ephys/ElectrodePlacement"]
     context = {
         "schema": "http://schema.org/",
         "kg": "https://kg.ebrains.eu/api/instances/",
         "vocab": "https://openminds.ebrains.eu/vocab/",
         "terms": "https://openminds.ebrains.eu/controlledTerms/",
         "core": "https://openminds.ebrains.eu/core/"
     }
     fields = [
         Field("lookup_label", str, "vocab:lookupLabel", multiple=False, required=False,
               doc="no description available"),
         Field("custom_property_sets", "openminds.core.CustomPropertySet", "vocab:customPropertySet", multiple=True, required=False,
               doc="no description available"),
         Field("description", str, "vocab:description", multiple=False, required=False,
-              doc="Longer statement or account giving the characteristics of the simulation."),
+              doc="Longer statement or account giving the characteristics of the electrode placement."),
+        Field("device", ["openminds.ephys.ElectrodeArrayUsage", "openminds.ephys.ElectrodeUsage", "openminds.ephys.PipetteUsage", "openminds.specimenprep.SlicingDeviceUsage"], "vocab:device", multiple=False, required=True,
+              doc="Piece of equipment or mechanism (hardware) designed to serve a special purpose or perform a special function."),
         Field("ended_at_time", datetime, "vocab:endedAtTime", multiple=False, required=False,
               doc="no description available"),
-        Field("environment", "openminds.computation.Environment", "vocab:environment", multiple=False, required=True,
-              doc="no description available"),
-        Field("inputs", ["openminds.computation.LocalFile", "openminds.core.File", "openminds.core.FileBundle", "openminds.core.ModelVersion", "openminds.core.SoftwareVersion"], "vocab:input", multiple=True, required=True,
+        Field("inputs", ["openminds.core.SubjectState", "openminds.core.TissueSampleState"], "vocab:input", multiple=True, required=True,
               doc="Something or someone that is put into or participates in a process or machine."),
-        Field("launch_configuration", "openminds.computation.LaunchConfiguration", "vocab:launchConfiguration", multiple=False, required=True,
-              doc="no description available"),
-        Field("outputs", ["openminds.computation.LocalFile", "openminds.core.File", "openminds.core.FileBundle"], "vocab:output", multiple=True, required=True,
+        Field("is_part_of", "openminds.core.DatasetVersion", "vocab:isPartOf", multiple=False, required=True,
+              doc="Reference to the ensemble of multiple things or beings."),
+        Field("outputs", ["openminds.core.SubjectState", "openminds.core.TissueSampleState"], "vocab:output", multiple=True, required=True,
               doc="Something or someone that comes out of, is delivered or produced by a process or machine."),
-        Field("recipe", "openminds.computation.WorkflowRecipeVersion", "vocab:recipe", multiple=False, required=False,
-              doc="no description available"),
-        Field("resource_usages", ["openminds.core.QuantitativeValue", "openminds.core.QuantitativeValueRange"], "vocab:resourceUsage", multiple=True, required=False,
+        Field("performed_by", ["openminds.computation.SoftwareAgent", "openminds.core.Person"], "vocab:performedBy", multiple=True, required=False,
               doc="no description available"),
-        Field("started_at_time", datetime, "vocab:startedAtTime", multiple=False, required=True,
+        Field("preparation_design", "openminds.controlledterms.PreparationType", "vocab:preparationDesign", multiple=False, required=False,
               doc="no description available"),
-        Field("started_by", ["openminds.computation.SoftwareAgent", "openminds.core.Person"], "vocab:startedBy", multiple=False, required=False,
+        Field("protocols", "openminds.core.Protocol", "vocab:protocol", multiple=True, required=True,
+              doc="Plan that describes the process of a scientific or medical experiment, treatment, or procedure."),
+        Field("started_at_time", datetime, "vocab:startedAtTime", multiple=False, required=False,
               doc="no description available"),
-        Field("status", "openminds.controlledterms.ActionStatusType", "vocab:status", multiple=False, required=False,
-              doc="no description available"),
-        Field("study_targets", ["openminds.controlledterms.BiologicalOrder", "openminds.controlledterms.BiologicalSex", "openminds.controlledterms.BreedingType", "openminds.controlledterms.CellCultureType", "openminds.controlledterms.CellType", "openminds.controlledterms.Disease", "openminds.controlledterms.DiseaseModel", "openminds.controlledterms.GeneticStrainType", "openminds.controlledterms.Handedness", "openminds.controlledterms.MolecularEntity", "openminds.controlledterms.Organ", "openminds.controlledterms.Species", "openminds.controlledterms.SubcellularEntity", "openminds.controlledterms.TermSuggestion", "openminds.controlledterms.UBERONParcellation", "openminds.sands.CustomAnatomicalEntity", "openminds.sands.ParcellationEntity", "openminds.sands.ParcellationEntityVersion"], "vocab:studyTarget", multiple=True, required=False,
+        Field("study_targets", ["openminds.controlledterms.AuditoryStimulusType", "openminds.controlledterms.BiologicalOrder", "openminds.controlledterms.BiologicalSex", "openminds.controlledterms.BreedingType", "openminds.controlledterms.CellCultureType", "openminds.controlledterms.CellType", "openminds.controlledterms.Disease", "openminds.controlledterms.DiseaseModel", "openminds.controlledterms.ElectricalStimulusType", "openminds.controlledterms.GeneticStrainType", "openminds.controlledterms.GustatoryStimulusType", "openminds.controlledterms.Handedness", "openminds.controlledterms.MolecularEntity", "openminds.controlledterms.OlfactoryStimulusType", "openminds.controlledterms.OpticalStimulusType", "openminds.controlledterms.Organ", "openminds.controlledterms.Species", "openminds.controlledterms.SubcellularEntity", "openminds.controlledterms.TactileStimulusType", "openminds.controlledterms.TermSuggestion", "openminds.controlledterms.UBERONParcellation", "openminds.controlledterms.VisualStimulusType", "openminds.sands.CustomAnatomicalEntity", "openminds.sands.ParcellationEntity", "openminds.sands.ParcellationEntityVersion"], "vocab:studyTarget", multiple=True, required=False,
               doc="Structure or function that was targeted within a study."),
-        Field("tags", str, "vocab:tags", multiple=True, required=False,
-              doc="no description available"),
-        Field("was_informed_by", ["openminds.computation.DataAnalysis", "openminds.computation.ModelValidation", "openminds.computation.Optimization", "openminds.computation.Simulation", "openminds.computation.Visualization"], "vocab:wasInformedBy", multiple=False, required=False,
+        Field("target_position", "openminds.sands.AnatomicalTargetPosition", "vocab:targetPosition", multiple=False, required=False,
               doc="no description available"),
 
     ]
     existence_query_fields = ('lookup_label',)
```

### Comparing `fairgraph-0.8.2/fairgraph/openminds/computation/software_agent.py` & `fairgraph-0.9.0/fairgraph/openminds/computation/software_agent.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 """
-
+Structured information about a piece of software or web service that can perform a task autonomously.
 """
 
 # this file was auto-generated
 
 from datetime import date, datetime
 from fairgraph.base_v3 import KGObject, IRI
 from fairgraph.fields import Field
 
 
 
 
 class SoftwareAgent(KGObject):
     """
-
+    Structured information about a piece of software or web service that can perform a task autonomously.
     """
     default_space = "computation"
     type = ["https://openminds.ebrains.eu/computation/SoftwareAgent"]
     context = {
         "schema": "http://schema.org/",
         "kg": "https://kg.ebrains.eu/api/instances/",
         "vocab": "https://openminds.ebrains.eu/vocab/",
```

### Comparing `fairgraph-0.8.2/fairgraph/openminds/computation/validation_test.py` & `fairgraph-0.9.0/fairgraph/openminds/publications/chapter.py`

 * *Files 22% similar despite different names*

```diff
@@ -7,50 +7,62 @@
 from datetime import date, datetime
 from fairgraph.base_v3 import KGObject, IRI
 from fairgraph.fields import Field
 
 
 
 
-class ValidationTest(KGObject):
+class Chapter(KGObject):
     """
 
     """
-    default_space = "computation"
-    type = ["https://openminds.ebrains.eu/computation/ValidationTest"]
+    default_space = "livepapers"
+    type = ["https://openminds.ebrains.eu/publications/Chapter"]
     context = {
         "schema": "http://schema.org/",
         "kg": "https://kg.ebrains.eu/api/instances/",
         "vocab": "https://openminds.ebrains.eu/vocab/",
         "terms": "https://openminds.ebrains.eu/controlledTerms/",
         "core": "https://openminds.ebrains.eu/core/"
     }
     fields = [
-        Field("name", str, "vocab:fullName", multiple=False, required=True,
-              doc="Whole, non-abbreviated name of the validation test."),
-        Field("alias", str, "vocab:shortName", multiple=False, required=True,
-              doc="Shortened or fully abbreviated name of the validation test."),
-        Field("custodians", ["openminds.core.Organization", "openminds.core.Person"], "vocab:custodian", multiple=True, required=False,
+        Field("name", str, "vocab:name", multiple=False, required=True,
+              doc="Word or phrase that constitutes the distinctive designation of the chapter."),
+        Field("iri", IRI, "vocab:IRI", multiple=False, required=False,
+              doc="Stands for Internationalized Resource Identifier which is an internet protocol standard that builds on the URI protocol, extending the set of permitted characters to include Unicode/ISO 10646."),
+        Field("abstract", str, "vocab:abstract", multiple=False, required=False,
+              doc="no description available"),
+        Field("authors", ["openminds.core.Consortium", "openminds.core.Organization", "openminds.core.Person"], "vocab:author", multiple=True, required=True,
+              doc="Creator of a literary or creative work, as well as a dataset publication."),
+        Field("cited_publications", ["openminds.core.DOI", "openminds.core.ISBN"], "vocab:citedPublication", multiple=True, required=False,
+              doc="no description available"),
+        Field("copyright", "openminds.core.Copyright", "vocab:copyright", multiple=False, required=False,
+              doc="Exclusive and assignable legal right of an originator to reproduce, publish, sell, or distribute the matter and form of a creative work for a defined time period."),
+        Field("custodians", ["openminds.core.Consortium", "openminds.core.Organization", "openminds.core.Person"], "vocab:custodian", multiple=True, required=False,
               doc="The 'custodian' is a legal person who is responsible for the content and quality of the data, metadata, and/or code of a research product."),
-        Field("description", str, "vocab:description", multiple=False, required=True,
-              doc="Longer statement or account giving the characteristics of the validation test."),
-        Field("developers", ["openminds.core.Organization", "openminds.core.Person"], "vocab:developer", multiple=True, required=True,
-              doc="Legal person that creates or improves products or services (e.g., software, applications, etc.)."),
+        Field("date_created", date, "vocab:dateCreated", multiple=False, required=False,
+              doc="no description available"),
+        Field("date_modified", date, "vocab:dateModified", multiple=False, required=False,
+              doc="no description available"),
+        Field("date_published", date, "vocab:datePublished", multiple=False, required=True,
+              doc="no description available"),
         Field("digital_identifier", "openminds.core.DOI", "vocab:digitalIdentifier", multiple=False, required=False,
               doc="Digital handle to identify objects or legal persons."),
-        Field("experimental_technique", "openminds.controlledterms.Technique", "vocab:experimentalTechnique", multiple=False, required=False,
+        Field("editors", "openminds.core.Person", "vocab:editor", multiple=True, required=False,
+              doc="no description available"),
+        Field("funding", "openminds.core.Funding", "vocab:funding", multiple=True, required=False,
+              doc="Money provided by a legal person for a particular purpose."),
+        Field("is_part_of", "openminds.publications.Book", "vocab:isPartOf", multiple=False, required=True,
+              doc="Reference to the ensemble of multiple things or beings."),
+        Field("keywords", ["openminds.controlledterms.AuditoryStimulusType", "openminds.controlledterms.BiologicalOrder", "openminds.controlledterms.BiologicalSex", "openminds.controlledterms.BreedingType", "openminds.controlledterms.CellCultureType", "openminds.controlledterms.CellType", "openminds.controlledterms.Disease", "openminds.controlledterms.DiseaseModel", "openminds.controlledterms.ElectricalStimulusType", "openminds.controlledterms.GeneticStrainType", "openminds.controlledterms.GustatoryStimulusType", "openminds.controlledterms.Handedness", "openminds.controlledterms.MolecularEntity", "openminds.controlledterms.OlfactoryStimulusType", "openminds.controlledterms.OpticalStimulusType", "openminds.controlledterms.Organ", "openminds.controlledterms.Species", "openminds.controlledterms.SubcellularEntity", "openminds.controlledterms.TactileStimulusType", "openminds.controlledterms.TermSuggestion", "openminds.controlledterms.UBERONParcellation", "openminds.controlledterms.VisualStimulusType", "openminds.sands.CustomAnatomicalEntity", "openminds.sands.ParcellationEntity", "openminds.sands.ParcellationEntityVersion"], "vocab:keyword", multiple=True, required=False,
+              doc="Significant word or concept that are representative of the chapter."),
+        Field("license", "openminds.core.License", "vocab:license", multiple=False, required=False,
+              doc="Grant by a party to another party as an element of an agreement between those parties that permits to do, use, or own something."),
+        Field("pagination", str, "vocab:pagination", multiple=False, required=False,
               doc="no description available"),
-        Field("versions", "openminds.computation.ValidationTestVersion", "vocab:hasVersion", multiple=True, required=True,
-              doc="Reference to variants of an original."),
-        Field("homepage", "openminds.core.URL", "vocab:homepage", multiple=False, required=False,
-              doc="Main website of the validation test."),
-        Field("how_to_cite", str, "vocab:howToCite", multiple=False, required=False,
-              doc="Preferred format for citing a particular object or legal person."),
-        Field("model_scope", "openminds.controlledterms.ModelScope", "vocab:scope", multiple=False, required=False,
-              doc="Extent of something."),
-        Field("score_type", "openminds.controlledterms.DifferenceMeasure", "vocab:scoreType", multiple=False, required=False,
+        Field("publisher", ["openminds.core.Consortium", "openminds.core.Organization", "openminds.core.Person"], "vocab:publisher", multiple=False, required=False,
               doc="no description available"),
-        Field("study_targets", ["openminds.controlledterms.BiologicalOrder", "openminds.controlledterms.BiologicalSex", "openminds.controlledterms.BreedingType", "openminds.controlledterms.CellCultureType", "openminds.controlledterms.CellType", "openminds.controlledterms.Disease", "openminds.controlledterms.DiseaseModel", "openminds.controlledterms.GeneticStrainType", "openminds.controlledterms.Handedness", "openminds.controlledterms.MolecularEntity", "openminds.controlledterms.Organ", "openminds.controlledterms.Species", "openminds.controlledterms.SubcellularEntity", "openminds.controlledterms.TermSuggestion", "openminds.controlledterms.UBERONParcellation", "openminds.sands.CustomAnatomicalEntity", "openminds.sands.ParcellationEntity", "openminds.sands.ParcellationEntityVersion"], "vocab:studyTarget", multiple=True, required=False,
-              doc="Structure or function that was targeted within a study."),
+        Field("version_identifier", str, "vocab:versionIdentifier", multiple=False, required=False,
+              doc="Term or code used to identify the version of something."),
 
     ]
-    existence_query_fields = ('name', 'alias')
+    existence_query_fields = ('name', 'authors', 'date_published', 'is_part_of')
```

### Comparing `fairgraph-0.8.2/fairgraph/openminds/computation/validation_test_version.py` & `fairgraph-0.9.0/fairgraph/openminds/computation/validation_test_version.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 """
-
+Structured information about a specific implementation of a validation test.
 """
 
 # this file was auto-generated
 
 from datetime import date, datetime
 from fairgraph.base_v3 import KGObject, IRI
 from fairgraph.fields import Field
 
 from fairgraph.errors import ResolutionFailure
 from .validation_test import ValidationTest
 
 
 class ValidationTestVersion(KGObject):
     """
-
+    Structured information about a specific implementation of a validation test.
     """
     default_space = "computation"
     type = ["https://openminds.ebrains.eu/computation/ValidationTestVersion"]
     context = {
         "schema": "http://schema.org/",
         "kg": "https://kg.ebrains.eu/api/instances/",
         "vocab": "https://openminds.ebrains.eu/vocab/",
@@ -28,21 +28,23 @@
     fields = [
         Field("name", str, "vocab:fullName", multiple=False, required=False,
               doc="Whole, non-abbreviated name of the validation test version."),
         Field("alias", str, "vocab:shortName", multiple=False, required=True,
               doc="Shortened or fully abbreviated name of the validation test version."),
         Field("accessibility", "openminds.controlledterms.ProductAccessibility", "vocab:accessibility", multiple=False, required=True,
               doc="Level to which something is accessible to the validation test version."),
+        Field("configuration", ["openminds.core.Configuration", "openminds.core.File", "openminds.core.PropertyValueList", "openminds.core.URL"], "vocab:configuration", multiple=False, required=False,
+              doc="no description available"),
         Field("copyright", "openminds.core.Copyright", "vocab:copyright", multiple=False, required=False,
               doc="Exclusive and assignable legal right of an originator to reproduce, publish, sell, or distribute the matter and form of a creative work for a defined time period."),
-        Field("custodians", ["openminds.core.Organization", "openminds.core.Person"], "vocab:custodian", multiple=True, required=False,
+        Field("custodians", ["openminds.core.Consortium", "openminds.core.Organization", "openminds.core.Person"], "vocab:custodian", multiple=True, required=False,
               doc="The 'custodian' is a legal person who is responsible for the content and quality of the data, metadata, and/or code of a research product."),
         Field("description", str, "vocab:description", multiple=False, required=False,
               doc="Longer statement or account giving the characteristics of the validation test version."),
-        Field("developers", ["openminds.core.Organization", "openminds.core.Person"], "vocab:developer", multiple=True, required=False,
+        Field("developers", ["openminds.core.Consortium", "openminds.core.Organization", "openminds.core.Person"], "vocab:developer", multiple=True, required=False,
               doc="Legal person that creates or improves products or services (e.g., software, applications, etc.)."),
         Field("digital_identifier", "openminds.core.DOI", "vocab:digitalIdentifier", multiple=False, required=False,
               doc="Digital handle to identify objects or legal persons."),
         Field("entry_point", str, "vocab:entryPoint", multiple=False, required=False,
               doc="no description available"),
         Field("format", "openminds.core.ContentType", "vocab:format", multiple=False, required=True,
               doc="Method of digitally organizing and structuring data or information."),
@@ -54,15 +56,15 @@
               doc="Main website of the validation test version."),
         Field("how_to_cite", str, "vocab:howToCite", multiple=False, required=False,
               doc="Preferred format for citing a particular object or legal person."),
         Field("is_alternative_version_of", "openminds.computation.ValidationTestVersion", "vocab:isAlternativeVersionOf", multiple=True, required=False,
               doc="Reference to an original form where the essence was preserved, but presented in an alternative form."),
         Field("is_new_version_of", "openminds.computation.ValidationTestVersion", "vocab:isNewVersionOf", multiple=False, required=False,
               doc="Reference to a previous (potentially outdated) particular form of something."),
-        Field("keywords", ["openminds.controlledterms.ActionStatusType", "openminds.controlledterms.AgeCategory", "openminds.controlledterms.AnatomicalAxesOrientation", "openminds.controlledterms.AnatomicalPlane", "openminds.controlledterms.AnnotationType", "openminds.controlledterms.AtlasType", "openminds.controlledterms.BiologicalOrder", "openminds.controlledterms.BiologicalSex", "openminds.controlledterms.BreedingType", "openminds.controlledterms.CellCultureType", "openminds.controlledterms.CellType", "openminds.controlledterms.ChemicalMixtureType", "openminds.controlledterms.ContributionType", "openminds.controlledterms.CranialWindowType", "openminds.controlledterms.CriteriaQualityType", "openminds.controlledterms.DataType", "openminds.controlledterms.DeviceType", "openminds.controlledterms.DifferenceMeasure", "openminds.controlledterms.Disease", "openminds.controlledterms.DiseaseModel", "openminds.controlledterms.EthicsAssessment", "openminds.controlledterms.ExperimentalApproach", "openminds.controlledterms.FileBundleGrouping", "openminds.controlledterms.FileRepositoryType", "openminds.controlledterms.FileUsageRole", "openminds.controlledterms.GeneticStrainType", "openminds.controlledterms.Handedness", "openminds.controlledterms.Language", "openminds.controlledterms.Laterality", "openminds.controlledterms.MeasuredQuantity", "openminds.controlledterms.MetaDataModelType", "openminds.controlledterms.ModelAbstractionLevel", "openminds.controlledterms.ModelScope", "openminds.controlledterms.MolecularEntity", "openminds.controlledterms.OperatingDevice", "openminds.controlledterms.OperatingSystem", "openminds.controlledterms.Organ", "openminds.controlledterms.PatchClampVariation", "openminds.controlledterms.PreparationType", "openminds.controlledterms.ProductAccessibility", "openminds.controlledterms.ProgrammingLanguage", "openminds.controlledterms.QualitativeOverlap", "openminds.controlledterms.SemanticDataType", "openminds.controlledterms.Service", "openminds.controlledterms.SetupType", "openminds.controlledterms.SoftwareApplicationCategory", "openminds.controlledterms.SoftwareFeature", "openminds.controlledterms.Species", "openminds.controlledterms.StimulationApproach", "openminds.controlledterms.StimulusType", "openminds.controlledterms.SubcellularEntity", "openminds.controlledterms.SubjectAttribute", "openminds.controlledterms.Technique", "openminds.controlledterms.TermSuggestion", "openminds.controlledterms.Terminology", "openminds.controlledterms.TissueSampleAttribute", "openminds.controlledterms.TissueSampleType", "openminds.controlledterms.TypeOfUncertainty", "openminds.controlledterms.UBERONParcellation", "openminds.controlledterms.UnitOfMeasurement"], "vocab:keyword", multiple=True, required=False,
+        Field("keywords", ["openminds.controlledterms.ActionStatusType", "openminds.controlledterms.AgeCategory", "openminds.controlledterms.AnatomicalAxesOrientation", "openminds.controlledterms.AnatomicalPlane", "openminds.controlledterms.AnnotationType", "openminds.controlledterms.AtlasType", "openminds.controlledterms.AuditoryStimulusType", "openminds.controlledterms.BiologicalOrder", "openminds.controlledterms.BiologicalSex", "openminds.controlledterms.BreedingType", "openminds.controlledterms.CellCultureType", "openminds.controlledterms.CellType", "openminds.controlledterms.ChemicalMixtureType", "openminds.controlledterms.ContributionType", "openminds.controlledterms.CranialWindowConstructionType", "openminds.controlledterms.CranialWindowReinforcementType", "openminds.controlledterms.CriteriaQualityType", "openminds.controlledterms.DataType", "openminds.controlledterms.DeviceType", "openminds.controlledterms.DifferenceMeasure", "openminds.controlledterms.Disease", "openminds.controlledterms.DiseaseModel", "openminds.controlledterms.EducationalLevel", "openminds.controlledterms.ElectricalStimulusType", "openminds.controlledterms.EthicsAssessment", "openminds.controlledterms.ExperimentalApproach", "openminds.controlledterms.FileBundleGrouping", "openminds.controlledterms.FileRepositoryType", "openminds.controlledterms.FileUsageRole", "openminds.controlledterms.GeneticStrainType", "openminds.controlledterms.GustatoryStimulusType", "openminds.controlledterms.Handedness", "openminds.controlledterms.Language", "openminds.controlledterms.Laterality", "openminds.controlledterms.LearningResourceType", "openminds.controlledterms.MeasuredQuantity", "openminds.controlledterms.MetaDataModelType", "openminds.controlledterms.ModelAbstractionLevel", "openminds.controlledterms.ModelScope", "openminds.controlledterms.MolecularEntity", "openminds.controlledterms.OlfactoryStimulusType", "openminds.controlledterms.OperatingDevice", "openminds.controlledterms.OperatingSystem", "openminds.controlledterms.OpticalStimulusType", "openminds.controlledterms.Organ", "openminds.controlledterms.PatchClampVariation", "openminds.controlledterms.PreparationType", "openminds.controlledterms.ProductAccessibility", "openminds.controlledterms.ProgrammingLanguage", "openminds.controlledterms.QualitativeOverlap", "openminds.controlledterms.SemanticDataType", "openminds.controlledterms.Service", "openminds.controlledterms.SetupType", "openminds.controlledterms.SoftwareApplicationCategory", "openminds.controlledterms.SoftwareFeature", "openminds.controlledterms.Species", "openminds.controlledterms.StimulationApproach", "openminds.controlledterms.StimulationTechnique", "openminds.controlledterms.SubcellularEntity", "openminds.controlledterms.SubjectAttribute", "openminds.controlledterms.TactileStimulusType", "openminds.controlledterms.Technique", "openminds.controlledterms.TermSuggestion", "openminds.controlledterms.Terminology", "openminds.controlledterms.TissueSampleAttribute", "openminds.controlledterms.TissueSampleType", "openminds.controlledterms.TypeOfUncertainty", "openminds.controlledterms.UBERONParcellation", "openminds.controlledterms.UnitOfMeasurement", "openminds.controlledterms.VisualStimulusType"], "vocab:keyword", multiple=True, required=False,
               doc="Significant word or concept that are representative of the validation test version."),
         Field("licenses", "openminds.core.License", "vocab:license", multiple=True, required=False,
               doc="Grant by a party to another party as an element of an agreement between those parties that permits to do, use, or own something."),
         Field("other_contributions", "openminds.core.Contribution", "vocab:otherContribution", multiple=True, required=False,
               doc="Giving or supplying of something (such as money or time) as a part or share other than what is covered elsewhere."),
         Field("reference_data", ["openminds.core.DOI", "openminds.core.File", "openminds.core.FileBundle", "openminds.core.URL"], "vocab:referenceData", multiple=True, required=False,
               doc="no description available"),
```

### Comparing `fairgraph-0.8.2/fairgraph/openminds/computation/visualization.py` & `fairgraph-0.9.0/fairgraph/openminds/core/research/tissue_sample.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,62 +1,50 @@
 """
-
+Structured information on a tissue sample.
 """
 
 # this file was auto-generated
 
 from datetime import date, datetime
 from fairgraph.base_v3 import KGObject, IRI
 from fairgraph.fields import Field
 
 
 
 
-class Visualization(KGObject):
+class TissueSample(KGObject):
     """
-
+    Structured information on a tissue sample.
     """
-    default_space = "computation"
-    type = ["https://openminds.ebrains.eu/computation/Visualization"]
+    default_space = "dataset"
+    type = ["https://openminds.ebrains.eu/core/TissueSample"]
     context = {
         "schema": "http://schema.org/",
         "kg": "https://kg.ebrains.eu/api/instances/",
         "vocab": "https://openminds.ebrains.eu/vocab/",
         "terms": "https://openminds.ebrains.eu/controlledTerms/",
         "core": "https://openminds.ebrains.eu/core/"
     }
     fields = [
         Field("lookup_label", str, "vocab:lookupLabel", multiple=False, required=False,
               doc="no description available"),
-        Field("custom_property_sets", "openminds.core.CustomPropertySet", "vocab:customPropertySet", multiple=True, required=False,
-              doc="no description available"),
-        Field("description", str, "vocab:description", multiple=False, required=False,
-              doc="Longer statement or account giving the characteristics of the visualization."),
-        Field("ended_at_time", datetime, "vocab:endedAtTime", multiple=False, required=False,
-              doc="no description available"),
-        Field("environment", "openminds.computation.Environment", "vocab:environment", multiple=False, required=True,
-              doc="no description available"),
-        Field("inputs", ["openminds.computation.LocalFile", "openminds.core.File", "openminds.core.FileBundle", "openminds.core.SoftwareVersion"], "vocab:input", multiple=True, required=True,
-              doc="Something or someone that is put into or participates in a process or machine."),
-        Field("launch_configuration", "openminds.computation.LaunchConfiguration", "vocab:launchConfiguration", multiple=False, required=True,
-              doc="no description available"),
-        Field("outputs", ["openminds.computation.LocalFile", "openminds.core.File", "openminds.core.FileBundle"], "vocab:output", multiple=True, required=True,
-              doc="Something or someone that comes out of, is delivered or produced by a process or machine."),
-        Field("recipe", "openminds.computation.WorkflowRecipeVersion", "vocab:recipe", multiple=False, required=False,
-              doc="no description available"),
-        Field("resource_usages", ["openminds.core.QuantitativeValue", "openminds.core.QuantitativeValueRange"], "vocab:resourceUsage", multiple=True, required=False,
-              doc="no description available"),
-        Field("started_at_time", datetime, "vocab:startedAtTime", multiple=False, required=True,
-              doc="no description available"),
-        Field("started_by", ["openminds.computation.SoftwareAgent", "openminds.core.Person"], "vocab:startedBy", multiple=False, required=False,
-              doc="no description available"),
-        Field("status", "openminds.controlledterms.ActionStatusType", "vocab:status", multiple=False, required=False,
-              doc="no description available"),
-        Field("study_targets", ["openminds.controlledterms.BiologicalOrder", "openminds.controlledterms.BiologicalSex", "openminds.controlledterms.BreedingType", "openminds.controlledterms.CellCultureType", "openminds.controlledterms.CellType", "openminds.controlledterms.Disease", "openminds.controlledterms.DiseaseModel", "openminds.controlledterms.GeneticStrainType", "openminds.controlledterms.Handedness", "openminds.controlledterms.MolecularEntity", "openminds.controlledterms.Organ", "openminds.controlledterms.Species", "openminds.controlledterms.SubcellularEntity", "openminds.controlledterms.TermSuggestion", "openminds.controlledterms.UBERONParcellation", "openminds.sands.CustomAnatomicalEntity", "openminds.sands.ParcellationEntity", "openminds.sands.ParcellationEntityVersion"], "vocab:studyTarget", multiple=True, required=False,
-              doc="Structure or function that was targeted within a study."),
-        Field("tags", str, "vocab:tags", multiple=True, required=False,
-              doc="no description available"),
-        Field("was_informed_by", ["openminds.computation.DataAnalysis", "openminds.computation.ModelValidation", "openminds.computation.Optimization", "openminds.computation.Simulation", "openminds.computation.Visualization"], "vocab:wasInformedBy", multiple=False, required=False,
+        Field("anatomical_locations", ["openminds.controlledterms.UBERONParcellation", "openminds.sands.CustomAnatomicalEntity", "openminds.sands.ParcellationEntity", "openminds.sands.ParcellationEntityVersion"], "vocab:anatomicalLocation", multiple=True, required=False,
               doc="no description available"),
+        Field("biological_sex", "openminds.controlledterms.BiologicalSex", "vocab:biologicalSex", multiple=False, required=False,
+              doc="Differentiation of individuals of most species (animals and plants) based on the type of gametes they produce."),
+        Field("internal_identifier", str, "vocab:internalIdentifier", multiple=False, required=False,
+              doc="Term or code that identifies the tissue sample within a particular product."),
+        Field("is_part_of", "openminds.core.TissueSampleCollection", "vocab:isPartOf", multiple=True, required=False,
+              doc="Reference to the ensemble of multiple things or beings."),
+        Field("laterality", "openminds.controlledterms.Laterality", "vocab:laterality", multiple=True, required=False,
+              doc="Differentiation between a pair of lateral homologous parts of the body."),
+        Field("origin", ["openminds.controlledterms.CellType", "openminds.controlledterms.Organ"], "vocab:origin", multiple=False, required=True,
+              doc="Source at which something begins or rises, or from which something derives."),
+        Field("species", ["openminds.controlledterms.Species", "openminds.core.Strain"], "vocab:species", multiple=False, required=True,
+              doc="Category of biological classification comprising related organisms or populations potentially capable of interbreeding, and being designated by a binomial that consists of the name of a genus followed by a Latin or latinized uncapitalized noun or adjective."),
+        Field("studied_states", "openminds.core.TissueSampleState", "vocab:studiedState", multiple=True, required=True,
+              doc="Reference to a point in time at which the tissue sample was studied in a particular mode or condition."),
+        Field("type", "openminds.controlledterms.TissueSampleType", "vocab:type", multiple=False, required=True,
+              doc="Distinct class to which a group of entities or concepts with similar characteristics or attributes belong to."),
 
     ]
     existence_query_fields = ('lookup_label',)
```

### Comparing `fairgraph-0.8.2/fairgraph/openminds/computation/workflow_execution.py` & `fairgraph-0.9.0/fairgraph/openminds/core/data/service_link.py`

 * *Files 24% similar despite different names*

```diff
@@ -7,30 +7,34 @@
 from datetime import date, datetime
 from fairgraph.base_v3 import KGObject, IRI
 from fairgraph.fields import Field
 
 
 
 
-class WorkflowExecution(KGObject):
+class ServiceLink(KGObject):
     """
 
     """
-    default_space = "computation"
-    type = ["https://openminds.ebrains.eu/computation/WorkflowExecution"]
+    default_space = "dataset"
+    type = ["https://openminds.ebrains.eu/core/ServiceLink"]
     context = {
         "schema": "http://schema.org/",
         "kg": "https://kg.ebrains.eu/api/instances/",
         "vocab": "https://openminds.ebrains.eu/vocab/",
         "terms": "https://openminds.ebrains.eu/controlledTerms/",
         "core": "https://openminds.ebrains.eu/core/"
     }
     fields = [
-        Field("recipe", "openminds.computation.WorkflowRecipeVersion", "vocab:recipe", multiple=False, required=False,
+        Field("name", str, "vocab:name", multiple=False, required=False,
+              doc="Word or phrase that constitutes the distinctive designation of the service link."),
+        Field("data_location", ["openminds.core.File", "openminds.core.FileArchive", "openminds.core.FileBundle", "openminds.core.ModelVersion", "openminds.publications.LivePaperResourceItem", "openminds.sands.ParcellationEntityVersion"], "vocab:dataLocation", multiple=False, required=True,
               doc="no description available"),
-        Field("stages", ["openminds.computation.DataAnalysis", "openminds.computation.ModelValidation", "openminds.computation.Optimization", "openminds.computation.Simulation", "openminds.computation.Visualization"], "vocab:stages", multiple=True, required=True,
+        Field("open_data_in", "openminds.core.URL", "vocab:openDataIn", multiple=False, required=True,
               doc="no description available"),
-        Field("started_by", ["openminds.computation.SoftwareAgent", "openminds.core.Person"], "vocab:startedBy", multiple=False, required=False,
+        Field("preview_image", "openminds.core.File", "vocab:previewImage", multiple=False, required=False,
+              doc="no description available"),
+        Field("service", "openminds.controlledterms.Service", "vocab:service", multiple=False, required=True,
               doc="no description available"),
 
     ]
-    existence_query_fields = ('stages',)
+    existence_query_fields = ('data_location', 'open_data_in', 'service')
```

### Comparing `fairgraph-0.8.2/fairgraph/openminds/computation/workflow_recipe.py` & `fairgraph-0.9.0/fairgraph/openminds/computation/workflow_recipe.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 """
-
+Structured information about the description of a prospective workflow.
 """
 
 # this file was auto-generated
 
 from datetime import date, datetime
 from fairgraph.base_v3 import KGObject, IRI
 from fairgraph.fields import Field
 
 
 
 
 class WorkflowRecipe(KGObject):
     """
-
+    Structured information about the description of a prospective workflow.
     """
     default_space = "computation"
     type = ["https://openminds.ebrains.eu/computation/WorkflowRecipe"]
     context = {
         "schema": "http://schema.org/",
         "kg": "https://kg.ebrains.eu/api/instances/",
         "vocab": "https://openminds.ebrains.eu/vocab/",
@@ -25,19 +25,19 @@
         "core": "https://openminds.ebrains.eu/core/"
     }
     fields = [
         Field("name", str, "vocab:fullName", multiple=False, required=True,
               doc="Whole, non-abbreviated name of the workflow recipe."),
         Field("alias", str, "vocab:shortName", multiple=False, required=True,
               doc="Shortened or fully abbreviated name of the workflow recipe."),
-        Field("custodians", ["openminds.core.Organization", "openminds.core.Person"], "vocab:custodian", multiple=True, required=False,
+        Field("custodians", ["openminds.core.Consortium", "openminds.core.Organization", "openminds.core.Person"], "vocab:custodian", multiple=True, required=False,
               doc="The 'custodian' is a legal person who is responsible for the content and quality of the data, metadata, and/or code of a research product."),
         Field("description", str, "vocab:description", multiple=False, required=True,
               doc="Longer statement or account giving the characteristics of the workflow recipe."),
-        Field("developers", ["openminds.core.Organization", "openminds.core.Person"], "vocab:developer", multiple=True, required=True,
+        Field("developers", ["openminds.core.Consortium", "openminds.core.Organization", "openminds.core.Person"], "vocab:developer", multiple=True, required=True,
               doc="Legal person that creates or improves products or services (e.g., software, applications, etc.)."),
         Field("digital_identifier", "openminds.core.DOI", "vocab:digitalIdentifier", multiple=False, required=False,
               doc="Digital handle to identify objects or legal persons."),
         Field("versions", "openminds.computation.WorkflowRecipeVersion", "vocab:hasVersion", multiple=True, required=True,
               doc="Reference to variants of an original."),
         Field("homepage", "openminds.core.URL", "vocab:homepage", multiple=False, required=False,
               doc="Main website of the workflow recipe."),
```

### Comparing `fairgraph-0.8.2/fairgraph/openminds/computation/workflow_recipe_version.py` & `fairgraph-0.9.0/fairgraph/openminds/computation/workflow_recipe_version.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 """
-
+Structured information about a specific implemented version of a workflow recipe.
 """
 
 # this file was auto-generated
 
 from datetime import date, datetime
 from fairgraph.base_v3 import KGObject, IRI
 from fairgraph.fields import Field
 
 
 
 
 class WorkflowRecipeVersion(KGObject):
     """
-
+    Structured information about a specific implemented version of a workflow recipe.
     """
     default_space = "computation"
     type = ["https://openminds.ebrains.eu/computation/WorkflowRecipeVersion"]
     context = {
         "schema": "http://schema.org/",
         "kg": "https://kg.ebrains.eu/api/instances/",
         "vocab": "https://openminds.ebrains.eu/vocab/",
@@ -29,19 +29,19 @@
               doc="Whole, non-abbreviated name of the workflow recipe version."),
         Field("alias", str, "vocab:shortName", multiple=False, required=True,
               doc="Shortened or fully abbreviated name of the workflow recipe version."),
         Field("accessibility", "openminds.controlledterms.ProductAccessibility", "vocab:accessibility", multiple=False, required=True,
               doc="Level to which something is accessible to the workflow recipe version."),
         Field("copyright", "openminds.core.Copyright", "vocab:copyright", multiple=False, required=False,
               doc="Exclusive and assignable legal right of an originator to reproduce, publish, sell, or distribute the matter and form of a creative work for a defined time period."),
-        Field("custodians", ["openminds.core.Organization", "openminds.core.Person"], "vocab:custodian", multiple=True, required=False,
+        Field("custodians", ["openminds.core.Consortium", "openminds.core.Organization", "openminds.core.Person"], "vocab:custodian", multiple=True, required=False,
               doc="The 'custodian' is a legal person who is responsible for the content and quality of the data, metadata, and/or code of a research product."),
         Field("description", str, "vocab:description", multiple=False, required=False,
               doc="Longer statement or account giving the characteristics of the workflow recipe version."),
-        Field("developers", ["openminds.core.Organization", "openminds.core.Person"], "vocab:developer", multiple=True, required=False,
+        Field("developers", ["openminds.core.Consortium", "openminds.core.Organization", "openminds.core.Person"], "vocab:developer", multiple=True, required=False,
               doc="Legal person that creates or improves products or services (e.g., software, applications, etc.)."),
         Field("digital_identifier", "openminds.core.DOI", "vocab:digitalIdentifier", multiple=False, required=False,
               doc="Digital handle to identify objects or legal persons."),
         Field("format", "openminds.core.ContentType", "vocab:format", multiple=False, required=True,
               doc="Method of digitally organizing and structuring data or information."),
         Field("full_documentation", ["openminds.core.DOI", "openminds.core.File", "openminds.core.URL"], "vocab:fullDocumentation", multiple=False, required=True,
               doc="Non-abridged instructions, comments, and information for using a particular product."),
@@ -53,15 +53,15 @@
               doc="Main website of the workflow recipe version."),
         Field("how_to_cite", str, "vocab:howToCite", multiple=False, required=False,
               doc="Preferred format for citing a particular object or legal person."),
         Field("is_alternative_version_of", "openminds.computation.WorkflowRecipeVersion", "vocab:isAlternativeVersionOf", multiple=True, required=False,
               doc="Reference to an original form where the essence was preserved, but presented in an alternative form."),
         Field("is_new_version_of", "openminds.computation.WorkflowRecipeVersion", "vocab:isNewVersionOf", multiple=False, required=False,
               doc="Reference to a previous (potentially outdated) particular form of something."),
-        Field("keywords", ["openminds.controlledterms.ActionStatusType", "openminds.controlledterms.AgeCategory", "openminds.controlledterms.AnatomicalAxesOrientation", "openminds.controlledterms.AnatomicalPlane", "openminds.controlledterms.AnnotationType", "openminds.controlledterms.AtlasType", "openminds.controlledterms.BiologicalOrder", "openminds.controlledterms.BiologicalSex", "openminds.controlledterms.BreedingType", "openminds.controlledterms.CellCultureType", "openminds.controlledterms.CellType", "openminds.controlledterms.ChemicalMixtureType", "openminds.controlledterms.ContributionType", "openminds.controlledterms.CranialWindowType", "openminds.controlledterms.CriteriaQualityType", "openminds.controlledterms.DataType", "openminds.controlledterms.DeviceType", "openminds.controlledterms.DifferenceMeasure", "openminds.controlledterms.Disease", "openminds.controlledterms.DiseaseModel", "openminds.controlledterms.EthicsAssessment", "openminds.controlledterms.ExperimentalApproach", "openminds.controlledterms.FileBundleGrouping", "openminds.controlledterms.FileRepositoryType", "openminds.controlledterms.FileUsageRole", "openminds.controlledterms.GeneticStrainType", "openminds.controlledterms.Handedness", "openminds.controlledterms.Language", "openminds.controlledterms.Laterality", "openminds.controlledterms.MeasuredQuantity", "openminds.controlledterms.MetaDataModelType", "openminds.controlledterms.ModelAbstractionLevel", "openminds.controlledterms.ModelScope", "openminds.controlledterms.MolecularEntity", "openminds.controlledterms.OperatingDevice", "openminds.controlledterms.OperatingSystem", "openminds.controlledterms.Organ", "openminds.controlledterms.PatchClampVariation", "openminds.controlledterms.PreparationType", "openminds.controlledterms.ProductAccessibility", "openminds.controlledterms.ProgrammingLanguage", "openminds.controlledterms.QualitativeOverlap", "openminds.controlledterms.SemanticDataType", "openminds.controlledterms.Service", "openminds.controlledterms.SetupType", "openminds.controlledterms.SoftwareApplicationCategory", "openminds.controlledterms.SoftwareFeature", "openminds.controlledterms.Species", "openminds.controlledterms.StimulationApproach", "openminds.controlledterms.StimulusType", "openminds.controlledterms.SubcellularEntity", "openminds.controlledterms.SubjectAttribute", "openminds.controlledterms.Technique", "openminds.controlledterms.TermSuggestion", "openminds.controlledterms.Terminology", "openminds.controlledterms.TissueSampleAttribute", "openminds.controlledterms.TissueSampleType", "openminds.controlledterms.TypeOfUncertainty", "openminds.controlledterms.UBERONParcellation", "openminds.controlledterms.UnitOfMeasurement"], "vocab:keyword", multiple=True, required=False,
+        Field("keywords", ["openminds.controlledterms.ActionStatusType", "openminds.controlledterms.AgeCategory", "openminds.controlledterms.AnatomicalAxesOrientation", "openminds.controlledterms.AnatomicalPlane", "openminds.controlledterms.AnnotationType", "openminds.controlledterms.AtlasType", "openminds.controlledterms.AuditoryStimulusType", "openminds.controlledterms.BiologicalOrder", "openminds.controlledterms.BiologicalSex", "openminds.controlledterms.BreedingType", "openminds.controlledterms.CellCultureType", "openminds.controlledterms.CellType", "openminds.controlledterms.ChemicalMixtureType", "openminds.controlledterms.ContributionType", "openminds.controlledterms.CranialWindowConstructionType", "openminds.controlledterms.CranialWindowReinforcementType", "openminds.controlledterms.CriteriaQualityType", "openminds.controlledterms.DataType", "openminds.controlledterms.DeviceType", "openminds.controlledterms.DifferenceMeasure", "openminds.controlledterms.Disease", "openminds.controlledterms.DiseaseModel", "openminds.controlledterms.EducationalLevel", "openminds.controlledterms.ElectricalStimulusType", "openminds.controlledterms.EthicsAssessment", "openminds.controlledterms.ExperimentalApproach", "openminds.controlledterms.FileBundleGrouping", "openminds.controlledterms.FileRepositoryType", "openminds.controlledterms.FileUsageRole", "openminds.controlledterms.GeneticStrainType", "openminds.controlledterms.GustatoryStimulusType", "openminds.controlledterms.Handedness", "openminds.controlledterms.Language", "openminds.controlledterms.Laterality", "openminds.controlledterms.LearningResourceType", "openminds.controlledterms.MeasuredQuantity", "openminds.controlledterms.MetaDataModelType", "openminds.controlledterms.ModelAbstractionLevel", "openminds.controlledterms.ModelScope", "openminds.controlledterms.MolecularEntity", "openminds.controlledterms.OlfactoryStimulusType", "openminds.controlledterms.OperatingDevice", "openminds.controlledterms.OperatingSystem", "openminds.controlledterms.OpticalStimulusType", "openminds.controlledterms.Organ", "openminds.controlledterms.PatchClampVariation", "openminds.controlledterms.PreparationType", "openminds.controlledterms.ProductAccessibility", "openminds.controlledterms.ProgrammingLanguage", "openminds.controlledterms.QualitativeOverlap", "openminds.controlledterms.SemanticDataType", "openminds.controlledterms.Service", "openminds.controlledterms.SetupType", "openminds.controlledterms.SoftwareApplicationCategory", "openminds.controlledterms.SoftwareFeature", "openminds.controlledterms.Species", "openminds.controlledterms.StimulationApproach", "openminds.controlledterms.StimulationTechnique", "openminds.controlledterms.SubcellularEntity", "openminds.controlledterms.SubjectAttribute", "openminds.controlledterms.TactileStimulusType", "openminds.controlledterms.Technique", "openminds.controlledterms.TermSuggestion", "openminds.controlledterms.Terminology", "openminds.controlledterms.TissueSampleAttribute", "openminds.controlledterms.TissueSampleType", "openminds.controlledterms.TypeOfUncertainty", "openminds.controlledterms.UBERONParcellation", "openminds.controlledterms.UnitOfMeasurement", "openminds.controlledterms.VisualStimulusType"], "vocab:keyword", multiple=True, required=False,
               doc="Significant word or concept that are representative of the workflow recipe version."),
         Field("licenses", "openminds.core.License", "vocab:license", multiple=True, required=False,
               doc="Grant by a party to another party as an element of an agreement between those parties that permits to do, use, or own something."),
         Field("other_contributions", "openminds.core.Contribution", "vocab:otherContribution", multiple=True, required=False,
               doc="Giving or supplying of something (such as money or time) as a part or share other than what is covered elsewhere."),
         Field("related_publications", ["openminds.core.DOI", "openminds.core.HANDLE", "openminds.core.ISBN"], "vocab:relatedPublication", multiple=True, required=False,
               doc="Reference to something that was made available for the general public to see or buy."),
```

### Comparing `fairgraph-0.8.2/fairgraph/openminds/controlledterms/__init__.py` & `fairgraph-0.9.0/fairgraph/openminds/controlledterms/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 import sys
 import inspect
 from ...base_v3 import KGObject
 
 from .difference_measure import DifferenceMeasure
 from .programming_language import ProgrammingLanguage
+from .stimulation_technique import StimulationTechnique
 from .measured_quantity import MeasuredQuantity
 from .laterality import Laterality
+from .auditory_stimulus_type import AuditoryStimulusType
 from .software_application_category import SoftwareApplicationCategory
 from .service import Service
 from .age_category import AgeCategory
 from .semantic_data_type import SemanticDataType
 from .preparation_type import PreparationType
 from .criteria_quality_type import CriteriaQualityType
 from .operating_system import OperatingSystem
@@ -19,52 +21,60 @@
 from .subject_attribute import SubjectAttribute
 from .device_type import DeviceType
 from .uberon_parcellation import UBERONParcellation
 from .software_feature import SoftwareFeature
 from .cell_type import CellType
 from .type_of_uncertainty import TypeOfUncertainty
 from .genetic_strain_type import GeneticStrainType
+from .electrical_stimulus_type import ElectricalStimulusType
 from .model_abstraction_level import ModelAbstractionLevel
+from .olfactory_stimulus_type import OlfactoryStimulusType
+from .learning_resource_type import LearningResourceType
 from .ethics_assessment import EthicsAssessment
 from .organ import Organ
 from .technique import Technique
+from .tactile_stimulus_type import TactileStimulusType
 from .chemical_mixture_type import ChemicalMixtureType
 from .qualitative_overlap import QualitativeOverlap
 from .anatomical_axes_orientation import AnatomicalAxesOrientation
 from .molecular_entity import MolecularEntity
 from .meta_data_model_type import MetaDataModelType
 from .species import Species
 from .file_usage_role import FileUsageRole
 from .anatomical_plane import AnatomicalPlane
 from .biological_sex import BiologicalSex
 from .data_type import DataType
 from .stimulation_approach import StimulationApproach
 from .model_scope import ModelScope
-from .stimulus_type import StimulusType
+from .optical_stimulus_type import OpticalStimulusType
+from .cranial_window_reinforcement_type import CranialWindowReinforcementType
 from .term_suggestion import TermSuggestion
 from .disease import Disease
 from .setup_type import SetupType
 from .terminology import Terminology
 from .handedness import Handedness
 from .tissue_sample_type import TissueSampleType
 from .contribution_type import ContributionType
 from .product_accessibility import ProductAccessibility
+from .cranial_window_construction_type import CranialWindowConstructionType
 from .biological_order import BiologicalOrder
-from .cranial_window_type import CranialWindowType
+from .educational_level import EducationalLevel
+from .visual_stimulus_type import VisualStimulusType
 from .language import Language
 from .cell_culture_type import CellCultureType
 from .action_status_type import ActionStatusType
 from .unit_of_measurement import UnitOfMeasurement
 from .file_bundle_grouping import FileBundleGrouping
 from .disease_model import DiseaseModel
 from .patch_clamp_variation import PatchClampVariation
 from .file_repository_type import FileRepositoryType
 from .atlas_type import AtlasType
 from .subcellular_entity import SubcellularEntity
 from .annotation_type import AnnotationType
+from .gustatory_stimulus_type import GustatoryStimulusType
 from .tissue_sample_attribute import TissueSampleAttribute
 
 
 def list_kg_classes():
     """List all KG classes defined in this module"""
     return [obj for name, obj in inspect.getmembers(sys.modules[__name__])
            if inspect.isclass(obj) and issubclass(obj, KGObject) and obj.__module__.startswith(__name__)]
```

### Comparing `fairgraph-0.8.2/fairgraph/openminds/controlledterms/action_status_type.py` & `fairgraph-0.9.0/fairgraph/openminds/controlledterms/laterality.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,40 +1,60 @@
 """
+Structured information on the lateral direction.
+
+    .. list-table:: **Possible values**
+       :widths: 20 80
+       :header-rows: 0
+
+       * - left
+         -
+       * - right
+         -
 
 """
 
 # this file was auto-generated
 
 from datetime import date, datetime
 from fairgraph.base_v3 import KGObject, IRI
 from fairgraph.fields import Field
 
 
 
 
-class ActionStatusType(KGObject):
+class Laterality(KGObject):
     """
+    Structured information on the lateral direction.
+
+    .. list-table:: **Possible values**
+       :widths: 20 80
+       :header-rows: 0
+
+       * - left
+         -
+       * - right
+         -
 
     """
     default_space = "controlled"
-    type = ["https://openminds.ebrains.eu/controlledTerms/ActionStatusType"]
+    type = ["https://openminds.ebrains.eu/controlledTerms/Laterality"]
     context = {
         "schema": "http://schema.org/",
         "kg": "https://kg.ebrains.eu/api/instances/",
         "vocab": "https://openminds.ebrains.eu/vocab/",
         "terms": "https://openminds.ebrains.eu/controlledTerms/",
         "core": "https://openminds.ebrains.eu/core/"
     }
     fields = [
         Field("name", str, "vocab:name", multiple=False, required=True,
-              doc="Word or phrase that constitutes the distinctive designation of the action status type."),
+              doc="Word or phrase that constitutes the distinctive designation of the laterality."),
         Field("definition", str, "vocab:definition", multiple=False, required=False,
               doc="Short, but precise statement of the meaning of a word, word group, sign or a symbol."),
         Field("description", str, "vocab:description", multiple=False, required=False,
-              doc="Longer statement or account giving the characteristics of the action status type."),
+              doc="Longer statement or account giving the characteristics of the laterality."),
         Field("interlex_identifier", IRI, "vocab:interlexIdentifier", multiple=False, required=False,
               doc="Persistent identifier for a term registered in the InterLex project."),
         Field("knowledge_space_link", IRI, "vocab:knowledgeSpaceLink", multiple=False, required=False,
               doc="Persistent link to an encyclopedia entry in the Knowledge Space project."),
         Field("preferred_ontology_identifier", IRI, "vocab:preferredOntologyIdentifier", multiple=False, required=False,
               doc="Persistent identifier of a preferred ontological term."),
         Field("synonyms", str, "vocab:synonym", multiple=True, required=False,
```

### Comparing `fairgraph-0.8.2/fairgraph/openminds/controlledterms/age_category.py` & `fairgraph-0.9.0/fairgraph/openminds/controlledterms/type_of_uncertainty.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,40 +1,60 @@
 """
-Structured information on the life cycle (semantic term) of a specific age group.
+
+
+    .. list-table:: **Possible values**
+       :widths: 20 80
+       :header-rows: 0
+
+       * - standard deviation
+         -
+       * - standard error
+         -
+
 """
 
 # this file was auto-generated
 
 from datetime import date, datetime
 from fairgraph.base_v3 import KGObject, IRI
 from fairgraph.fields import Field
 
 
 
 
-class AgeCategory(KGObject):
+class TypeOfUncertainty(KGObject):
     """
-    Structured information on the life cycle (semantic term) of a specific age group.
+
+
+    .. list-table:: **Possible values**
+       :widths: 20 80
+       :header-rows: 0
+
+       * - standard deviation
+         -
+       * - standard error
+         -
+
     """
     default_space = "controlled"
-    type = ["https://openminds.ebrains.eu/controlledTerms/AgeCategory"]
+    type = ["https://openminds.ebrains.eu/controlledTerms/TypeOfUncertainty"]
     context = {
         "schema": "http://schema.org/",
         "kg": "https://kg.ebrains.eu/api/instances/",
         "vocab": "https://openminds.ebrains.eu/vocab/",
         "terms": "https://openminds.ebrains.eu/controlledTerms/",
         "core": "https://openminds.ebrains.eu/core/"
     }
     fields = [
         Field("name", str, "vocab:name", multiple=False, required=True,
-              doc="Word or phrase that constitutes the distinctive designation of the age category."),
+              doc="Word or phrase that constitutes the distinctive designation of the type of uncertainty."),
         Field("definition", str, "vocab:definition", multiple=False, required=False,
               doc="Short, but precise statement of the meaning of a word, word group, sign or a symbol."),
         Field("description", str, "vocab:description", multiple=False, required=False,
-              doc="Longer statement or account giving the characteristics of the age category."),
+              doc="Longer statement or account giving the characteristics of the type of uncertainty."),
         Field("interlex_identifier", IRI, "vocab:interlexIdentifier", multiple=False, required=False,
               doc="Persistent identifier for a term registered in the InterLex project."),
         Field("knowledge_space_link", IRI, "vocab:knowledgeSpaceLink", multiple=False, required=False,
               doc="Persistent link to an encyclopedia entry in the Knowledge Space project."),
         Field("preferred_ontology_identifier", IRI, "vocab:preferredOntologyIdentifier", multiple=False, required=False,
               doc="Persistent identifier of a preferred ontological term."),
         Field("synonyms", str, "vocab:synonym", multiple=True, required=False,
```

### Comparing `fairgraph-0.8.2/fairgraph/openminds/controlledterms/anatomical_axes_orientation.py` & `fairgraph-0.9.0/fairgraph/openminds/controlledterms/semantic_data_type.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,40 +1,68 @@
 """
-Structured information on the anatomical directions of the X, Y, and Z axis.
+
+
+    .. list-table:: **Possible values**
+       :widths: 20 80
+       :header-rows: 0
+
+       * - raw data
+         -
+       * - derived data
+         -
+       * - simulated data
+         -
+       * - experimental data
+         -
+
 """
 
 # this file was auto-generated
 
 from datetime import date, datetime
 from fairgraph.base_v3 import KGObject, IRI
 from fairgraph.fields import Field
 
 
 
 
-class AnatomicalAxesOrientation(KGObject):
+class SemanticDataType(KGObject):
     """
-    Structured information on the anatomical directions of the X, Y, and Z axis.
+
+
+    .. list-table:: **Possible values**
+       :widths: 20 80
+       :header-rows: 0
+
+       * - raw data
+         -
+       * - derived data
+         -
+       * - simulated data
+         -
+       * - experimental data
+         -
+
     """
     default_space = "controlled"
-    type = ["https://openminds.ebrains.eu/controlledTerms/AnatomicalAxesOrientation"]
+    type = ["https://openminds.ebrains.eu/controlledTerms/SemanticDataType"]
     context = {
         "schema": "http://schema.org/",
         "kg": "https://kg.ebrains.eu/api/instances/",
         "vocab": "https://openminds.ebrains.eu/vocab/",
         "terms": "https://openminds.ebrains.eu/controlledTerms/",
         "core": "https://openminds.ebrains.eu/core/"
     }
     fields = [
         Field("name", str, "vocab:name", multiple=False, required=True,
-              doc="Word or phrase that constitutes the distinctive designation of the anatomical axes orientation."),
+              doc="Word or phrase that constitutes the distinctive designation of the semantic data type."),
         Field("definition", str, "vocab:definition", multiple=False, required=False,
               doc="Short, but precise statement of the meaning of a word, word group, sign or a symbol."),
         Field("description", str, "vocab:description", multiple=False, required=False,
-              doc="Longer statement or account giving the characteristics of the anatomical axes orientation."),
+              doc="Longer statement or account giving the characteristics of the semantic data type."),
         Field("interlex_identifier", IRI, "vocab:interlexIdentifier", multiple=False, required=False,
               doc="Persistent identifier for a term registered in the InterLex project."),
         Field("knowledge_space_link", IRI, "vocab:knowledgeSpaceLink", multiple=False, required=False,
               doc="Persistent link to an encyclopedia entry in the Knowledge Space project."),
         Field("preferred_ontology_identifier", IRI, "vocab:preferredOntologyIdentifier", multiple=False, required=False,
               doc="Persistent identifier of a preferred ontological term."),
         Field("synonyms", str, "vocab:synonym", multiple=True, required=False,
```

### Comparing `fairgraph-0.8.2/fairgraph/openminds/controlledterms/anatomical_plane.py` & `fairgraph-0.9.0/fairgraph/openminds/controlledterms/term_suggestion.py`

 * *Files 15% similar despite different names*

```diff
@@ -7,38 +7,42 @@
 from datetime import date, datetime
 from fairgraph.base_v3 import KGObject, IRI
 from fairgraph.fields import Field
 
 
 
 
-class AnatomicalPlane(KGObject):
+class TermSuggestion(KGObject):
     """
 
     """
     default_space = "controlled"
-    type = ["https://openminds.ebrains.eu/controlledTerms/AnatomicalPlane"]
+    type = ["https://openminds.ebrains.eu/controlledTerms/TermSuggestion"]
     context = {
         "schema": "http://schema.org/",
         "kg": "https://kg.ebrains.eu/api/instances/",
         "vocab": "https://openminds.ebrains.eu/vocab/",
         "terms": "https://openminds.ebrains.eu/controlledTerms/",
         "core": "https://openminds.ebrains.eu/core/"
     }
     fields = [
         Field("name", str, "vocab:name", multiple=False, required=True,
-              doc="Word or phrase that constitutes the distinctive designation of the anatomical plane."),
+              doc="Word or phrase that constitutes the distinctive designation of the term suggestion."),
+        Field("add_existing_terminology", "openminds.controlledterms.Terminology", "vocab:addExistingTerminology", multiple=False, required=False,
+              doc="Reference to an existing terminology (distinct class to group related terms)."),
         Field("definition", str, "vocab:definition", multiple=False, required=False,
               doc="Short, but precise statement of the meaning of a word, word group, sign or a symbol."),
         Field("description", str, "vocab:description", multiple=False, required=False,
-              doc="Longer statement or account giving the characteristics of the anatomical plane."),
+              doc="Longer statement or account giving the characteristics of the term suggestion."),
         Field("interlex_identifier", IRI, "vocab:interlexIdentifier", multiple=False, required=False,
               doc="Persistent identifier for a term registered in the InterLex project."),
         Field("knowledge_space_link", IRI, "vocab:knowledgeSpaceLink", multiple=False, required=False,
               doc="Persistent link to an encyclopedia entry in the Knowledge Space project."),
         Field("preferred_ontology_identifier", IRI, "vocab:preferredOntologyIdentifier", multiple=False, required=False,
               doc="Persistent identifier of a preferred ontological term."),
+        Field("suggest_new_terminology", str, "vocab:suggestNewTerminology", multiple=False, required=False,
+              doc="Proposal of a new distinct class to group related terms."),
         Field("synonyms", str, "vocab:synonym", multiple=True, required=False,
               doc="Words or expressions used in the same language that have the same or nearly the same meaning in some or all senses."),
 
     ]
     existence_query_fields = ('name',)
```

### Comparing `fairgraph-0.8.2/fairgraph/openminds/controlledterms/annotation_type.py` & `fairgraph-0.9.0/fairgraph/openminds/controlledterms/language.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,40 +1,88 @@
 """
+Structured information on the available language setting.
+
+    .. list-table:: **Possible values**
+       :widths: 20 80
+       :header-rows: 0
+
+       * - French
+         -
+       * - English
+         -
+       * - Dutch
+         -
+       * - Norwegian
+         -
+       * - German
+         -
+       * - Greek
+         -
+       * - Italian
+         -
+       * - Spanish
+         -
+       * - Swedish
+         -
 
 """
 
 # this file was auto-generated
 
 from datetime import date, datetime
 from fairgraph.base_v3 import KGObject, IRI
 from fairgraph.fields import Field
 
 
 
 
-class AnnotationType(KGObject):
+class Language(KGObject):
     """
+    Structured information on the available language setting.
+
+    .. list-table:: **Possible values**
+       :widths: 20 80
+       :header-rows: 0
+
+       * - French
+         -
+       * - English
+         -
+       * - Dutch
+         -
+       * - Norwegian
+         -
+       * - German
+         -
+       * - Greek
+         -
+       * - Italian
+         -
+       * - Spanish
+         -
+       * - Swedish
+         -
 
     """
     default_space = "controlled"
-    type = ["https://openminds.ebrains.eu/controlledTerms/AnnotationType"]
+    type = ["https://openminds.ebrains.eu/controlledTerms/Language"]
     context = {
         "schema": "http://schema.org/",
         "kg": "https://kg.ebrains.eu/api/instances/",
         "vocab": "https://openminds.ebrains.eu/vocab/",
         "terms": "https://openminds.ebrains.eu/controlledTerms/",
         "core": "https://openminds.ebrains.eu/core/"
     }
     fields = [
         Field("name", str, "vocab:name", multiple=False, required=True,
-              doc="Word or phrase that constitutes the distinctive designation of the annotation type."),
+              doc="Word or phrase that constitutes the distinctive designation of the language."),
         Field("definition", str, "vocab:definition", multiple=False, required=False,
               doc="Short, but precise statement of the meaning of a word, word group, sign or a symbol."),
         Field("description", str, "vocab:description", multiple=False, required=False,
-              doc="Longer statement or account giving the characteristics of the annotation type."),
+              doc="Longer statement or account giving the characteristics of the language."),
         Field("interlex_identifier", IRI, "vocab:interlexIdentifier", multiple=False, required=False,
               doc="Persistent identifier for a term registered in the InterLex project."),
         Field("knowledge_space_link", IRI, "vocab:knowledgeSpaceLink", multiple=False, required=False,
               doc="Persistent link to an encyclopedia entry in the Knowledge Space project."),
         Field("preferred_ontology_identifier", IRI, "vocab:preferredOntologyIdentifier", multiple=False, required=False,
               doc="Persistent identifier of a preferred ontological term."),
         Field("synonyms", str, "vocab:synonym", multiple=True, required=False,
```

### Comparing `fairgraph-0.8.2/fairgraph/openminds/controlledterms/atlas_type.py` & `fairgraph-0.9.0/fairgraph/openminds/core/research/subject_group.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,38 +7,38 @@
 from datetime import date, datetime
 from fairgraph.base_v3 import KGObject, IRI
 from fairgraph.fields import Field
 
 
 
 
-class AtlasType(KGObject):
+class SubjectGroup(KGObject):
     """
 
     """
-    default_space = "controlled"
-    type = ["https://openminds.ebrains.eu/controlledTerms/AtlasType"]
+    default_space = "dataset"
+    type = ["https://openminds.ebrains.eu/core/SubjectGroup"]
     context = {
         "schema": "http://schema.org/",
         "kg": "https://kg.ebrains.eu/api/instances/",
         "vocab": "https://openminds.ebrains.eu/vocab/",
         "terms": "https://openminds.ebrains.eu/controlledTerms/",
         "core": "https://openminds.ebrains.eu/core/"
     }
     fields = [
-        Field("name", str, "vocab:name", multiple=False, required=True,
-              doc="Word or phrase that constitutes the distinctive designation of the atlas type."),
-        Field("definition", str, "vocab:definition", multiple=False, required=False,
-              doc="Short, but precise statement of the meaning of a word, word group, sign or a symbol."),
-        Field("description", str, "vocab:description", multiple=False, required=False,
-              doc="Longer statement or account giving the characteristics of the atlas type."),
-        Field("interlex_identifier", IRI, "vocab:interlexIdentifier", multiple=False, required=False,
-              doc="Persistent identifier for a term registered in the InterLex project."),
-        Field("knowledge_space_link", IRI, "vocab:knowledgeSpaceLink", multiple=False, required=False,
-              doc="Persistent link to an encyclopedia entry in the Knowledge Space project."),
-        Field("preferred_ontology_identifier", IRI, "vocab:preferredOntologyIdentifier", multiple=False, required=False,
-              doc="Persistent identifier of a preferred ontological term."),
-        Field("synonyms", str, "vocab:synonym", multiple=True, required=False,
-              doc="Words or expressions used in the same language that have the same or nearly the same meaning in some or all senses."),
+        Field("lookup_label", str, "vocab:lookupLabel", multiple=False, required=False,
+              doc="no description available"),
+        Field("additional_remarks", str, "vocab:additionalRemarks", multiple=False, required=False,
+              doc="Mention of what deserves additional attention or notice."),
+        Field("biological_sex", "openminds.controlledterms.BiologicalSex", "vocab:biologicalSex", multiple=True, required=False,
+              doc="Differentiation of individuals of most species (animals and plants) based on the type of gametes they produce."),
+        Field("internal_identifier", str, "vocab:internalIdentifier", multiple=False, required=False,
+              doc="Term or code that identifies the subject group within a particular product."),
+        Field("quantity", int, "vocab:quantity", multiple=False, required=False,
+              doc="Total amount or number of things or beings."),
+        Field("species", ["openminds.controlledterms.Species", "openminds.core.Strain"], "vocab:species", multiple=True, required=True,
+              doc="Category of biological classification comprising related organisms or populations potentially capable of interbreeding, and being designated by a binomial that consists of the name of a genus followed by a Latin or latinized uncapitalized noun or adjective."),
+        Field("studied_states", "openminds.core.SubjectGroupState", "vocab:studiedState", multiple=True, required=True,
+              doc="Reference to a point in time at which the subject group was studied in a particular mode or condition."),
 
     ]
-    existence_query_fields = ('name',)
+    existence_query_fields = ('lookup_label',)
```

### Comparing `fairgraph-0.8.2/fairgraph/openminds/controlledterms/biological_order.py` & `fairgraph-0.9.0/fairgraph/openminds/controlledterms/tactile_stimulus_type.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,40 +1,64 @@
 """
 
+
+    .. list-table:: **Possible values**
+       :widths: 20 80
+       :header-rows: 0
+
+       * - vibrating surface
+         -
+       * - textured surface
+         -
+       * - vibrating object
+         -
+
 """
 
 # this file was auto-generated
 
 from datetime import date, datetime
 from fairgraph.base_v3 import KGObject, IRI
 from fairgraph.fields import Field
 
 
 
 
-class BiologicalOrder(KGObject):
+class TactileStimulusType(KGObject):
     """
 
+
+    .. list-table:: **Possible values**
+       :widths: 20 80
+       :header-rows: 0
+
+       * - vibrating surface
+         -
+       * - textured surface
+         -
+       * - vibrating object
+         -
+
     """
     default_space = "controlled"
-    type = ["https://openminds.ebrains.eu/controlledTerms/BiologicalOrder"]
+    type = ["https://openminds.ebrains.eu/controlledTerms/TactileStimulusType"]
     context = {
         "schema": "http://schema.org/",
         "kg": "https://kg.ebrains.eu/api/instances/",
         "vocab": "https://openminds.ebrains.eu/vocab/",
         "terms": "https://openminds.ebrains.eu/controlledTerms/",
         "core": "https://openminds.ebrains.eu/core/"
     }
     fields = [
         Field("name", str, "vocab:name", multiple=False, required=True,
-              doc="Word or phrase that constitutes the distinctive designation of the biological order."),
+              doc="Word or phrase that constitutes the distinctive designation of the tactile stimulus type."),
         Field("definition", str, "vocab:definition", multiple=False, required=False,
               doc="Short, but precise statement of the meaning of a word, word group, sign or a symbol."),
         Field("description", str, "vocab:description", multiple=False, required=False,
-              doc="Longer statement or account giving the characteristics of the biological order."),
+              doc="Longer statement or account giving the characteristics of the tactile stimulus type."),
         Field("interlex_identifier", IRI, "vocab:interlexIdentifier", multiple=False, required=False,
               doc="Persistent identifier for a term registered in the InterLex project."),
         Field("knowledge_space_link", IRI, "vocab:knowledgeSpaceLink", multiple=False, required=False,
               doc="Persistent link to an encyclopedia entry in the Knowledge Space project."),
         Field("preferred_ontology_identifier", IRI, "vocab:preferredOntologyIdentifier", multiple=False, required=False,
               doc="Persistent identifier of a preferred ontological term."),
         Field("synonyms", str, "vocab:synonym", multiple=True, required=False,
```

### Comparing `fairgraph-0.8.2/fairgraph/openminds/controlledterms/biological_sex.py` & `fairgraph-0.9.0/fairgraph/openminds/controlledterms/cell_culture_type.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,40 +1,60 @@
 """
-Structured information on the biological sex of a subject.
+
+
+    .. list-table:: **Possible values**
+       :widths: 20 80
+       :header-rows: 0
+
+       * - `primary cell culture <http://id.nlm.nih.gov/mesh/2018/M0452904>`_
+         - A cell culture comprised of primary cultured cells and the media in which they are being actively propaged or quiescently stored.
+       * - `secondary cell culture <http://purl.obolibrary.org/obo/OBI_0001905>`_
+         - A cultured cell population that is derived through one or more passages in culture.
+
 """
 
 # this file was auto-generated
 
 from datetime import date, datetime
 from fairgraph.base_v3 import KGObject, IRI
 from fairgraph.fields import Field
 
 
 
 
-class BiologicalSex(KGObject):
+class CellCultureType(KGObject):
     """
-    Structured information on the biological sex of a subject.
+
+
+    .. list-table:: **Possible values**
+       :widths: 20 80
+       :header-rows: 0
+
+       * - `primary cell culture <http://id.nlm.nih.gov/mesh/2018/M0452904>`_
+         - A cell culture comprised of primary cultured cells and the media in which they are being actively propaged or quiescently stored.
+       * - `secondary cell culture <http://purl.obolibrary.org/obo/OBI_0001905>`_
+         - A cultured cell population that is derived through one or more passages in culture.
+
     """
     default_space = "controlled"
-    type = ["https://openminds.ebrains.eu/controlledTerms/BiologicalSex"]
+    type = ["https://openminds.ebrains.eu/controlledTerms/CellCultureType"]
     context = {
         "schema": "http://schema.org/",
         "kg": "https://kg.ebrains.eu/api/instances/",
         "vocab": "https://openminds.ebrains.eu/vocab/",
         "terms": "https://openminds.ebrains.eu/controlledTerms/",
         "core": "https://openminds.ebrains.eu/core/"
     }
     fields = [
         Field("name", str, "vocab:name", multiple=False, required=True,
-              doc="Word or phrase that constitutes the distinctive designation of the biological sex."),
+              doc="Word or phrase that constitutes the distinctive designation of the cell culture type."),
         Field("definition", str, "vocab:definition", multiple=False, required=False,
               doc="Short, but precise statement of the meaning of a word, word group, sign or a symbol."),
         Field("description", str, "vocab:description", multiple=False, required=False,
-              doc="Longer statement or account giving the characteristics of the biological sex."),
+              doc="Longer statement or account giving the characteristics of the cell culture type."),
         Field("interlex_identifier", IRI, "vocab:interlexIdentifier", multiple=False, required=False,
               doc="Persistent identifier for a term registered in the InterLex project."),
         Field("knowledge_space_link", IRI, "vocab:knowledgeSpaceLink", multiple=False, required=False,
               doc="Persistent link to an encyclopedia entry in the Knowledge Space project."),
         Field("preferred_ontology_identifier", IRI, "vocab:preferredOntologyIdentifier", multiple=False, required=False,
               doc="Persistent identifier of a preferred ontological term."),
         Field("synonyms", str, "vocab:synonym", multiple=True, required=False,
```

### Comparing `fairgraph-0.8.2/fairgraph/openminds/controlledterms/breeding_type.py` & `fairgraph-0.9.0/fairgraph/openminds/publications/live_paper.py`

 * *Files 15% similar despite different names*

```diff
@@ -7,38 +7,42 @@
 from datetime import date, datetime
 from fairgraph.base_v3 import KGObject, IRI
 from fairgraph.fields import Field
 
 
 
 
-class BreedingType(KGObject):
+class LivePaper(KGObject):
     """
 
     """
-    default_space = "controlled"
-    type = ["https://openminds.ebrains.eu/controlledTerms/BreedingType"]
+    default_space = "livepapers"
+    type = ["https://openminds.ebrains.eu/publications/LivePaper"]
     context = {
         "schema": "http://schema.org/",
         "kg": "https://kg.ebrains.eu/api/instances/",
         "vocab": "https://openminds.ebrains.eu/vocab/",
         "terms": "https://openminds.ebrains.eu/controlledTerms/",
         "core": "https://openminds.ebrains.eu/core/"
     }
     fields = [
-        Field("name", str, "vocab:name", multiple=False, required=True,
-              doc="Word or phrase that constitutes the distinctive designation of the breeding type."),
-        Field("definition", str, "vocab:definition", multiple=False, required=False,
-              doc="Short, but precise statement of the meaning of a word, word group, sign or a symbol."),
-        Field("description", str, "vocab:description", multiple=False, required=False,
-              doc="Longer statement or account giving the characteristics of the breeding type."),
-        Field("interlex_identifier", IRI, "vocab:interlexIdentifier", multiple=False, required=False,
-              doc="Persistent identifier for a term registered in the InterLex project."),
-        Field("knowledge_space_link", IRI, "vocab:knowledgeSpaceLink", multiple=False, required=False,
-              doc="Persistent link to an encyclopedia entry in the Knowledge Space project."),
-        Field("preferred_ontology_identifier", IRI, "vocab:preferredOntologyIdentifier", multiple=False, required=False,
-              doc="Persistent identifier of a preferred ontological term."),
-        Field("synonyms", str, "vocab:synonym", multiple=True, required=False,
-              doc="Words or expressions used in the same language that have the same or nearly the same meaning in some or all senses."),
+        Field("name", str, "vocab:fullName", multiple=False, required=True,
+              doc="Whole, non-abbreviated name of the live paper."),
+        Field("alias", str, "vocab:shortName", multiple=False, required=True,
+              doc="Shortened or fully abbreviated name of the live paper."),
+        Field("authors", ["openminds.core.Consortium", "openminds.core.Organization", "openminds.core.Person"], "vocab:author", multiple=True, required=True,
+              doc="Creator of a literary or creative work, as well as a dataset publication."),
+        Field("custodians", ["openminds.core.Consortium", "openminds.core.Organization", "openminds.core.Person"], "vocab:custodian", multiple=True, required=False,
+              doc="The 'custodian' is a legal person who is responsible for the content and quality of the data, metadata, and/or code of a research product."),
+        Field("description", str, "vocab:description", multiple=False, required=True,
+              doc="Longer statement or account giving the characteristics of the live paper."),
+        Field("digital_identifier", "openminds.core.DOI", "vocab:digitalIdentifier", multiple=False, required=False,
+              doc="Digital handle to identify objects or legal persons."),
+        Field("versions", "openminds.publications.LivePaperVersion", "vocab:hasVersion", multiple=True, required=True,
+              doc="Reference to variants of an original."),
+        Field("homepage", "openminds.core.URL", "vocab:homepage", multiple=False, required=False,
+              doc="Main website of the live paper."),
+        Field("how_to_cite", str, "vocab:howToCite", multiple=False, required=False,
+              doc="Preferred format for citing a particular object or legal person."),
 
     ]
-    existence_query_fields = ('name',)
+    existence_query_fields = ('name', 'alias')
```

### Comparing `fairgraph-0.8.2/fairgraph/openminds/controlledterms/cell_culture_type.py` & `fairgraph-0.9.0/fairgraph/openminds/controlledterms/visual_stimulus_type.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,40 +1,84 @@
 """
 
+
+    .. list-table:: **Possible values**
+       :widths: 20 80
+       :header-rows: 0
+
+       * - moving checkerboard
+         -
+       * - natural movie
+         -
+       * - moving symbol
+         -
+       * - static symbol
+         -
+       * - static grating
+         -
+       * - natural scene
+         -
+       * - moving grating
+         -
+       * - static checkerboard
+         -
+
 """
 
 # this file was auto-generated
 
 from datetime import date, datetime
 from fairgraph.base_v3 import KGObject, IRI
 from fairgraph.fields import Field
 
 
 
 
-class CellCultureType(KGObject):
+class VisualStimulusType(KGObject):
     """
 
+
+    .. list-table:: **Possible values**
+       :widths: 20 80
+       :header-rows: 0
+
+       * - moving checkerboard
+         -
+       * - natural movie
+         -
+       * - moving symbol
+         -
+       * - static symbol
+         -
+       * - static grating
+         -
+       * - natural scene
+         -
+       * - moving grating
+         -
+       * - static checkerboard
+         -
+
     """
     default_space = "controlled"
-    type = ["https://openminds.ebrains.eu/controlledTerms/CellCultureType"]
+    type = ["https://openminds.ebrains.eu/controlledTerms/VisualStimulusType"]
     context = {
         "schema": "http://schema.org/",
         "kg": "https://kg.ebrains.eu/api/instances/",
         "vocab": "https://openminds.ebrains.eu/vocab/",
         "terms": "https://openminds.ebrains.eu/controlledTerms/",
         "core": "https://openminds.ebrains.eu/core/"
     }
     fields = [
         Field("name", str, "vocab:name", multiple=False, required=True,
-              doc="Word or phrase that constitutes the distinctive designation of the cell culture type."),
+              doc="Word or phrase that constitutes the distinctive designation of the visual stimulus type."),
         Field("definition", str, "vocab:definition", multiple=False, required=False,
               doc="Short, but precise statement of the meaning of a word, word group, sign or a symbol."),
         Field("description", str, "vocab:description", multiple=False, required=False,
-              doc="Longer statement or account giving the characteristics of the cell culture type."),
+              doc="Longer statement or account giving the characteristics of the visual stimulus type."),
         Field("interlex_identifier", IRI, "vocab:interlexIdentifier", multiple=False, required=False,
               doc="Persistent identifier for a term registered in the InterLex project."),
         Field("knowledge_space_link", IRI, "vocab:knowledgeSpaceLink", multiple=False, required=False,
               doc="Persistent link to an encyclopedia entry in the Knowledge Space project."),
         Field("preferred_ontology_identifier", IRI, "vocab:preferredOntologyIdentifier", multiple=False, required=False,
               doc="Persistent identifier of a preferred ontological term."),
         Field("synonyms", str, "vocab:synonym", multiple=True, required=False,
```

### Comparing `fairgraph-0.8.2/fairgraph/openminds/controlledterms/cell_type.py` & `fairgraph-0.9.0/fairgraph/openminds/sands/atlas/brain_atlas.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,44 +1,54 @@
 """
-
+Structured information on a brain atlas (concept level).
 """
 
 # this file was auto-generated
 
 from datetime import date, datetime
 from fairgraph.base_v3 import KGObject, IRI
 from fairgraph.fields import Field
 
 
 
 
-class CellType(KGObject):
+class BrainAtlas(KGObject):
     """
-
+    Structured information on a brain atlas (concept level).
     """
-    default_space = "controlled"
-    type = ["https://openminds.ebrains.eu/controlledTerms/CellType"]
+    default_space = "atlas"
+    type = ["https://openminds.ebrains.eu/sands/BrainAtlas"]
     context = {
         "schema": "http://schema.org/",
         "kg": "https://kg.ebrains.eu/api/instances/",
         "vocab": "https://openminds.ebrains.eu/vocab/",
         "terms": "https://openminds.ebrains.eu/controlledTerms/",
         "core": "https://openminds.ebrains.eu/core/"
     }
     fields = [
-        Field("name", str, "vocab:name", multiple=False, required=True,
-              doc="Word or phrase that constitutes the distinctive designation of the cell type."),
-        Field("definition", str, "vocab:definition", multiple=False, required=False,
-              doc="Short, but precise statement of the meaning of a word, word group, sign or a symbol."),
-        Field("description", str, "vocab:description", multiple=False, required=False,
-              doc="Longer statement or account giving the characteristics of the cell type."),
-        Field("interlex_identifier", IRI, "vocab:interlexIdentifier", multiple=False, required=False,
-              doc="Persistent identifier for a term registered in the InterLex project."),
-        Field("knowledge_space_link", IRI, "vocab:knowledgeSpaceLink", multiple=False, required=False,
-              doc="Persistent link to an encyclopedia entry in the Knowledge Space project."),
-        Field("preferred_ontology_identifier", IRI, "vocab:preferredOntologyIdentifier", multiple=False, required=False,
-              doc="Persistent identifier of a preferred ontological term."),
-        Field("synonyms", str, "vocab:synonym", multiple=True, required=False,
-              doc="Words or expressions used in the same language that have the same or nearly the same meaning in some or all senses."),
+        Field("name", str, "vocab:fullName", multiple=False, required=True,
+              doc="Whole, non-abbreviated name of the brain atlas."),
+        Field("alias", str, "vocab:shortName", multiple=False, required=True,
+              doc="Shortened or fully abbreviated name of the brain atlas."),
+        Field("abbreviation", str, "vocab:abbreviation", multiple=False, required=False,
+              doc="no description available"),
+        Field("authors", ["openminds.core.Consortium", "openminds.core.Organization", "openminds.core.Person"], "vocab:author", multiple=True, required=True,
+              doc="Creator of a literary or creative work, as well as a dataset publication."),
+        Field("custodians", ["openminds.core.Consortium", "openminds.core.Organization", "openminds.core.Person"], "vocab:custodian", multiple=True, required=False,
+              doc="The 'custodian' is a legal person who is responsible for the content and quality of the data, metadata, and/or code of a research product."),
+        Field("description", str, "vocab:description", multiple=False, required=True,
+              doc="Longer statement or account giving the characteristics of the brain atlas."),
+        Field("digital_identifier", ["openminds.core.DOI", "openminds.core.ISBN", "openminds.core.RRID"], "vocab:digitalIdentifier", multiple=False, required=False,
+              doc="Digital handle to identify objects or legal persons."),
+        Field("has_terminology", "openminds.sands.ParcellationTerminology", "vocab:hasTerminology", multiple=False, required=True,
+              doc="no description available"),
+        Field("versions", "openminds.sands.BrainAtlasVersion", "vocab:hasVersion", multiple=True, required=True,
+              doc="Reference to variants of an original."),
+        Field("homepage", "openminds.core.URL", "vocab:homepage", multiple=False, required=False,
+              doc="Main website of the brain atlas."),
+        Field("how_to_cite", str, "vocab:howToCite", multiple=False, required=False,
+              doc="Preferred format for citing a particular object or legal person."),
+        Field("ontology_identifier", IRI, "vocab:ontologyIdentifier", multiple=False, required=False,
+              doc="Term or code used to identify the brain atlas registered within a particular ontology."),
 
     ]
-    existence_query_fields = ('name',)
+    existence_query_fields = ('digital_identifier',)
```

### Comparing `fairgraph-0.8.2/fairgraph/openminds/controlledterms/chemical_mixture_type.py` & `fairgraph-0.9.0/fairgraph/openminds/sands/non_atlas/custom_coordinate_space.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,38 +7,34 @@
 from datetime import date, datetime
 from fairgraph.base_v3 import KGObject, IRI
 from fairgraph.fields import Field
 
 
 
 
-class ChemicalMixtureType(KGObject):
+class CustomCoordinateSpace(KGObject):
     """
 
     """
-    default_space = "controlled"
-    type = ["https://openminds.ebrains.eu/controlledTerms/ChemicalMixtureType"]
+    default_space = "spatial"
+    type = ["https://openminds.ebrains.eu/sands/CustomCoordinateSpace"]
     context = {
         "schema": "http://schema.org/",
         "kg": "https://kg.ebrains.eu/api/instances/",
         "vocab": "https://openminds.ebrains.eu/vocab/",
         "terms": "https://openminds.ebrains.eu/controlledTerms/",
         "core": "https://openminds.ebrains.eu/core/"
     }
     fields = [
         Field("name", str, "vocab:name", multiple=False, required=True,
-              doc="Word or phrase that constitutes the distinctive designation of the chemical mixture type."),
-        Field("definition", str, "vocab:definition", multiple=False, required=False,
-              doc="Short, but precise statement of the meaning of a word, word group, sign or a symbol."),
-        Field("description", str, "vocab:description", multiple=False, required=False,
-              doc="Longer statement or account giving the characteristics of the chemical mixture type."),
-        Field("interlex_identifier", IRI, "vocab:interlexIdentifier", multiple=False, required=False,
-              doc="Persistent identifier for a term registered in the InterLex project."),
-        Field("knowledge_space_link", IRI, "vocab:knowledgeSpaceLink", multiple=False, required=False,
-              doc="Persistent link to an encyclopedia entry in the Knowledge Space project."),
-        Field("preferred_ontology_identifier", IRI, "vocab:preferredOntologyIdentifier", multiple=False, required=False,
-              doc="Persistent identifier of a preferred ontological term."),
-        Field("synonyms", str, "vocab:synonym", multiple=True, required=False,
-              doc="Words or expressions used in the same language that have the same or nearly the same meaning in some or all senses."),
+              doc="Word or phrase that constitutes the distinctive designation of the custom coordinate space."),
+        Field("anatomical_axes_orientation", "openminds.controlledterms.AnatomicalAxesOrientation", "vocab:anatomicalAxesOrientation", multiple=False, required=True,
+              doc="Relation between reference planes used in anatomy and mathematics."),
+        Field("axes_origins", "openminds.core.QuantitativeValue", "vocab:axesOrigin", multiple=True, required=True,
+              doc="Special point in a coordinate system used as a fixed point of reference for the geometry of the surrounding space."),
+        Field("default_images", "openminds.core.File", "vocab:defaultImage", multiple=True, required=False,
+              doc="Two or three dimensional image that particluarly represents a specific coordinate space."),
+        Field("native_unit", "openminds.controlledterms.UnitOfMeasurement", "vocab:nativeUnit", multiple=False, required=True,
+              doc="Determinate quantity used in the original measurement."),
 
     ]
     existence_query_fields = ('name',)
```

### Comparing `fairgraph-0.8.2/fairgraph/openminds/controlledterms/contribution_type.py` & `fairgraph-0.9.0/fairgraph/openminds/core/data/content_type.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,44 +1,46 @@
 """
-Structured information on the type of contribution a person or organization performed.
+Structured information on the content type of a file instance, bundle or repository.
 """
 
 # this file was auto-generated
 
 from datetime import date, datetime
 from fairgraph.base_v3 import KGObject, IRI
 from fairgraph.fields import Field
 
 
 
 
-class ContributionType(KGObject):
+class ContentType(KGObject):
     """
-    Structured information on the type of contribution a person or organization performed.
+    Structured information on the content type of a file instance, bundle or repository.
     """
     default_space = "controlled"
-    type = ["https://openminds.ebrains.eu/controlledTerms/ContributionType"]
+    type = ["https://openminds.ebrains.eu/core/ContentType"]
     context = {
         "schema": "http://schema.org/",
         "kg": "https://kg.ebrains.eu/api/instances/",
         "vocab": "https://openminds.ebrains.eu/vocab/",
         "terms": "https://openminds.ebrains.eu/controlledTerms/",
         "core": "https://openminds.ebrains.eu/core/"
     }
     fields = [
         Field("name", str, "vocab:name", multiple=False, required=True,
-              doc="Word or phrase that constitutes the distinctive designation of the contribution type."),
-        Field("definition", str, "vocab:definition", multiple=False, required=False,
-              doc="Short, but precise statement of the meaning of a word, word group, sign or a symbol."),
+              doc="Word or phrase that constitutes the distinctive designation of the content type."),
+        Field("data_types", "openminds.controlledterms.DataType", "vocab:dataType", multiple=True, required=False,
+              doc="no description available"),
         Field("description", str, "vocab:description", multiple=False, required=False,
-              doc="Longer statement or account giving the characteristics of the contribution type."),
-        Field("interlex_identifier", IRI, "vocab:interlexIdentifier", multiple=False, required=False,
-              doc="Persistent identifier for a term registered in the InterLex project."),
-        Field("knowledge_space_link", IRI, "vocab:knowledgeSpaceLink", multiple=False, required=False,
-              doc="Persistent link to an encyclopedia entry in the Knowledge Space project."),
-        Field("preferred_ontology_identifier", IRI, "vocab:preferredOntologyIdentifier", multiple=False, required=False,
-              doc="Persistent identifier of a preferred ontological term."),
+              doc="Longer statement or account giving the characteristics of the content type."),
+        Field("display_label", str, "vocab:displayLabel", multiple=False, required=False,
+              doc="no description available"),
+        Field("file_extensions", str, "vocab:fileExtension", multiple=True, required=False,
+              doc="String of characters attached as suffix to the names of files of a particular format."),
+        Field("related_media_type", IRI, "vocab:relatedMediaType", multiple=False, required=False,
+              doc="Reference to an official two-part identifier for file formats and format contents."),
+        Field("specification", IRI, "vocab:specification", multiple=False, required=False,
+              doc="Detailed and precise presentation of, or proposal for something."),
         Field("synonyms", str, "vocab:synonym", multiple=True, required=False,
               doc="Words or expressions used in the same language that have the same or nearly the same meaning in some or all senses."),
 
     ]
     existence_query_fields = ('name',)
```

### Comparing `fairgraph-0.8.2/fairgraph/openminds/controlledterms/cranial_window_type.py` & `fairgraph-0.9.0/fairgraph/openminds/core/products/dataset.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,44 +1,48 @@
 """
-
+Structured information on data originating from human/animal studies or simulations (concept level).
 """
 
 # this file was auto-generated
 
 from datetime import date, datetime
 from fairgraph.base_v3 import KGObject, IRI
 from fairgraph.fields import Field
 
 
 
 
-class CranialWindowType(KGObject):
+class Dataset(KGObject):
     """
-
+    Structured information on data originating from human/animal studies or simulations (concept level).
     """
-    default_space = "controlled"
-    type = ["https://openminds.ebrains.eu/controlledTerms/CranialWindowType"]
+    default_space = "dataset"
+    type = ["https://openminds.ebrains.eu/core/Dataset"]
     context = {
         "schema": "http://schema.org/",
         "kg": "https://kg.ebrains.eu/api/instances/",
         "vocab": "https://openminds.ebrains.eu/vocab/",
         "terms": "https://openminds.ebrains.eu/controlledTerms/",
         "core": "https://openminds.ebrains.eu/core/"
     }
     fields = [
-        Field("name", str, "vocab:name", multiple=False, required=True,
-              doc="Word or phrase that constitutes the distinctive designation of the cranial window type."),
-        Field("definition", str, "vocab:definition", multiple=False, required=False,
-              doc="Short, but precise statement of the meaning of a word, word group, sign or a symbol."),
-        Field("description", str, "vocab:description", multiple=False, required=False,
-              doc="Longer statement or account giving the characteristics of the cranial window type."),
-        Field("interlex_identifier", IRI, "vocab:interlexIdentifier", multiple=False, required=False,
-              doc="Persistent identifier for a term registered in the InterLex project."),
-        Field("knowledge_space_link", IRI, "vocab:knowledgeSpaceLink", multiple=False, required=False,
-              doc="Persistent link to an encyclopedia entry in the Knowledge Space project."),
-        Field("preferred_ontology_identifier", IRI, "vocab:preferredOntologyIdentifier", multiple=False, required=False,
-              doc="Persistent identifier of a preferred ontological term."),
-        Field("synonyms", str, "vocab:synonym", multiple=True, required=False,
-              doc="Words or expressions used in the same language that have the same or nearly the same meaning in some or all senses."),
+        Field("name", str, "vocab:fullName", multiple=False, required=True,
+              doc="Whole, non-abbreviated name of the dataset."),
+        Field("alias", str, "vocab:shortName", multiple=False, required=True,
+              doc="Shortened or fully abbreviated name of the dataset."),
+        Field("authors", ["openminds.core.Consortium", "openminds.core.Organization", "openminds.core.Person"], "vocab:author", multiple=True, required=True,
+              doc="Creator of a literary or creative work, as well as a dataset publication."),
+        Field("custodians", ["openminds.core.Consortium", "openminds.core.Organization", "openminds.core.Person"], "vocab:custodian", multiple=True, required=False,
+              doc="The 'custodian' is a legal person who is responsible for the content and quality of the data, metadata, and/or code of a research product."),
+        Field("description", str, "vocab:description", multiple=False, required=True,
+              doc="Longer statement or account giving the characteristics of the dataset."),
+        Field("digital_identifier", "openminds.core.DOI", "vocab:digitalIdentifier", multiple=False, required=False,
+              doc="Digital handle to identify objects or legal persons."),
+        Field("versions", "openminds.core.DatasetVersion", "vocab:hasVersion", multiple=True, required=True,
+              doc="Reference to variants of an original."),
+        Field("homepage", "openminds.core.URL", "vocab:homepage", multiple=False, required=False,
+              doc="Main website of the dataset."),
+        Field("how_to_cite", str, "vocab:howToCite", multiple=False, required=False,
+              doc="Preferred format for citing a particular object or legal person."),
 
     ]
-    existence_query_fields = ('name',)
+    existence_query_fields = ('alias',)
```

### Comparing `fairgraph-0.8.2/fairgraph/openminds/controlledterms/criteria_quality_type.py` & `fairgraph-0.9.0/fairgraph/openminds/controlledterms/electrical_stimulus_type.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,40 +1,56 @@
 """
-Structured information on the quality type of the defined criteria for a measurement.
+
+
+    .. list-table:: **Possible values**
+       :widths: 20 80
+       :header-rows: 0
+
+       * - direct current
+         -
+
 """
 
 # this file was auto-generated
 
 from datetime import date, datetime
 from fairgraph.base_v3 import KGObject, IRI
 from fairgraph.fields import Field
 
 
 
 
-class CriteriaQualityType(KGObject):
+class ElectricalStimulusType(KGObject):
     """
-    Structured information on the quality type of the defined criteria for a measurement.
+
+
+    .. list-table:: **Possible values**
+       :widths: 20 80
+       :header-rows: 0
+
+       * - direct current
+         -
+
     """
     default_space = "controlled"
-    type = ["https://openminds.ebrains.eu/controlledTerms/CriteriaQualityType"]
+    type = ["https://openminds.ebrains.eu/controlledTerms/ElectricalStimulusType"]
     context = {
         "schema": "http://schema.org/",
         "kg": "https://kg.ebrains.eu/api/instances/",
         "vocab": "https://openminds.ebrains.eu/vocab/",
         "terms": "https://openminds.ebrains.eu/controlledTerms/",
         "core": "https://openminds.ebrains.eu/core/"
     }
     fields = [
         Field("name", str, "vocab:name", multiple=False, required=True,
-              doc="Word or phrase that constitutes the distinctive designation of the criteria quality type."),
+              doc="Word or phrase that constitutes the distinctive designation of the electrical stimulus type."),
         Field("definition", str, "vocab:definition", multiple=False, required=False,
               doc="Short, but precise statement of the meaning of a word, word group, sign or a symbol."),
         Field("description", str, "vocab:description", multiple=False, required=False,
-              doc="Longer statement or account giving the characteristics of the criteria quality type."),
+              doc="Longer statement or account giving the characteristics of the electrical stimulus type."),
         Field("interlex_identifier", IRI, "vocab:interlexIdentifier", multiple=False, required=False,
               doc="Persistent identifier for a term registered in the InterLex project."),
         Field("knowledge_space_link", IRI, "vocab:knowledgeSpaceLink", multiple=False, required=False,
               doc="Persistent link to an encyclopedia entry in the Knowledge Space project."),
         Field("preferred_ontology_identifier", IRI, "vocab:preferredOntologyIdentifier", multiple=False, required=False,
               doc="Persistent identifier of a preferred ontological term."),
         Field("synonyms", str, "vocab:synonym", multiple=True, required=False,
```

### Comparing `fairgraph-0.8.2/fairgraph/openminds/controlledterms/data_type.py` & `fairgraph-0.9.0/fairgraph/openminds/sands/atlas/parcellation_entity_version.py`

 * *Files 15% similar despite different names*

```diff
@@ -7,38 +7,46 @@
 from datetime import date, datetime
 from fairgraph.base_v3 import KGObject, IRI
 from fairgraph.fields import Field
 
 
 
 
-class DataType(KGObject):
+class ParcellationEntityVersion(KGObject):
     """
 
     """
-    default_space = "controlled"
-    type = ["https://openminds.ebrains.eu/controlledTerms/DataType"]
+    default_space = "atlas"
+    type = ["https://openminds.ebrains.eu/sands/ParcellationEntityVersion"]
     context = {
         "schema": "http://schema.org/",
         "kg": "https://kg.ebrains.eu/api/instances/",
         "vocab": "https://openminds.ebrains.eu/vocab/",
         "terms": "https://openminds.ebrains.eu/controlledTerms/",
         "core": "https://openminds.ebrains.eu/core/"
     }
     fields = [
         Field("name", str, "vocab:name", multiple=False, required=True,
-              doc="Word or phrase that constitutes the distinctive designation of the data type."),
-        Field("definition", str, "vocab:definition", multiple=False, required=False,
-              doc="Short, but precise statement of the meaning of a word, word group, sign or a symbol."),
-        Field("description", str, "vocab:description", multiple=False, required=False,
-              doc="Longer statement or account giving the characteristics of the data type."),
-        Field("interlex_identifier", IRI, "vocab:interlexIdentifier", multiple=False, required=False,
-              doc="Persistent identifier for a term registered in the InterLex project."),
-        Field("knowledge_space_link", IRI, "vocab:knowledgeSpaceLink", multiple=False, required=False,
-              doc="Persistent link to an encyclopedia entry in the Knowledge Space project."),
-        Field("preferred_ontology_identifier", IRI, "vocab:preferredOntologyIdentifier", multiple=False, required=False,
-              doc="Persistent identifier of a preferred ontological term."),
-        Field("synonyms", str, "vocab:synonym", multiple=True, required=False,
-              doc="Words or expressions used in the same language that have the same or nearly the same meaning in some or all senses."),
+              doc="Word or phrase that constitutes the distinctive designation of the parcellation entity version."),
+        Field("lookup_label", str, "vocab:lookupLabel", multiple=False, required=False,
+              doc="no description available"),
+        Field("additional_remarks", str, "vocab:additionalRemarks", multiple=False, required=False,
+              doc="Mention of what deserves additional attention or notice."),
+        Field("alternative_names", str, "vocab:alternativeName", multiple=True, required=False,
+              doc="no description available"),
+        Field("corrected_name", str, "vocab:correctedName", multiple=False, required=False,
+              doc="no description available"),
+        Field("has_annotations", "openminds.sands.AtlasAnnotation", "vocab:hasAnnotation", multiple=True, required=False,
+              doc="no description available"),
+        Field("has_parents", ["openminds.sands.ParcellationEntity", "openminds.sands.ParcellationEntityVersion"], "vocab:hasParent", multiple=True, required=False,
+              doc="Reference to a parent object or legal person."),
+        Field("ontology_identifiers", str, "vocab:ontologyIdentifier", multiple=True, required=False,
+              doc="Term or code used to identify the parcellation entity version registered within a particular ontology."),
+        Field("relation_assessments", ["openminds.sands.QualitativeRelationAssessment", "openminds.sands.QuantitativeRelationAssessment"], "vocab:relationAssessment", multiple=True, required=False,
+              doc="no description available"),
+        Field("version_identifier", str, "vocab:versionIdentifier", multiple=False, required=True,
+              doc="Term or code used to identify the version of something."),
+        Field("version_innovation", str, "vocab:versionInnovation", multiple=False, required=False,
+              doc="Documentation on what changed in comparison to a previously published form of something."),
 
     ]
-    existence_query_fields = ('name',)
+    existence_query_fields = ('name', 'version_identifier')
```

### Comparing `fairgraph-0.8.2/fairgraph/openminds/controlledterms/device_type.py` & `fairgraph-0.9.0/fairgraph/openminds/controlledterms/contribution_type.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,40 +1,84 @@
 """
+Structured information on the type of contribution a person or organization performed.
+
+    .. list-table:: **Possible values**
+       :widths: 20 80
+       :header-rows: 0
+
+       * - marketing
+         -
+       * - information technology support
+         -
+       * - metadata managment
+         -
+       * - coordination
+         -
+       * - data processing
+         -
+       * - data collection
+         -
+       * - laboratory assistance
+         -
+       * - data management
+         -
 
 """
 
 # this file was auto-generated
 
 from datetime import date, datetime
 from fairgraph.base_v3 import KGObject, IRI
 from fairgraph.fields import Field
 
 
 
 
-class DeviceType(KGObject):
+class ContributionType(KGObject):
     """
+    Structured information on the type of contribution a person or organization performed.
+
+    .. list-table:: **Possible values**
+       :widths: 20 80
+       :header-rows: 0
+
+       * - marketing
+         -
+       * - information technology support
+         -
+       * - metadata managment
+         -
+       * - coordination
+         -
+       * - data processing
+         -
+       * - data collection
+         -
+       * - laboratory assistance
+         -
+       * - data management
+         -
 
     """
     default_space = "controlled"
-    type = ["https://openminds.ebrains.eu/controlledTerms/DeviceType"]
+    type = ["https://openminds.ebrains.eu/controlledTerms/ContributionType"]
     context = {
         "schema": "http://schema.org/",
         "kg": "https://kg.ebrains.eu/api/instances/",
         "vocab": "https://openminds.ebrains.eu/vocab/",
         "terms": "https://openminds.ebrains.eu/controlledTerms/",
         "core": "https://openminds.ebrains.eu/core/"
     }
     fields = [
         Field("name", str, "vocab:name", multiple=False, required=True,
-              doc="Word or phrase that constitutes the distinctive designation of the device type."),
+              doc="Word or phrase that constitutes the distinctive designation of the contribution type."),
         Field("definition", str, "vocab:definition", multiple=False, required=False,
               doc="Short, but precise statement of the meaning of a word, word group, sign or a symbol."),
         Field("description", str, "vocab:description", multiple=False, required=False,
-              doc="Longer statement or account giving the characteristics of the device type."),
+              doc="Longer statement or account giving the characteristics of the contribution type."),
         Field("interlex_identifier", IRI, "vocab:interlexIdentifier", multiple=False, required=False,
               doc="Persistent identifier for a term registered in the InterLex project."),
         Field("knowledge_space_link", IRI, "vocab:knowledgeSpaceLink", multiple=False, required=False,
               doc="Persistent link to an encyclopedia entry in the Knowledge Space project."),
         Field("preferred_ontology_identifier", IRI, "vocab:preferredOntologyIdentifier", multiple=False, required=False,
               doc="Persistent identifier of a preferred ontological term."),
         Field("synonyms", str, "vocab:synonym", multiple=True, required=False,
```

### Comparing `fairgraph-0.8.2/fairgraph/openminds/controlledterms/difference_measure.py` & `fairgraph-0.9.0/fairgraph/openminds/publications/live_paper_section.py`

 * *Files 15% similar despite different names*

```diff
@@ -7,38 +7,34 @@
 from datetime import date, datetime
 from fairgraph.base_v3 import KGObject, IRI
 from fairgraph.fields import Field
 
 
 
 
-class DifferenceMeasure(KGObject):
+class LivePaperSection(KGObject):
     """
 
     """
-    default_space = "controlled"
-    type = ["https://openminds.ebrains.eu/controlledTerms/DifferenceMeasure"]
+    default_space = "livepapers"
+    type = ["https://openminds.ebrains.eu/publications/LivePaperSection"]
     context = {
         "schema": "http://schema.org/",
         "kg": "https://kg.ebrains.eu/api/instances/",
         "vocab": "https://openminds.ebrains.eu/vocab/",
         "terms": "https://openminds.ebrains.eu/controlledTerms/",
         "core": "https://openminds.ebrains.eu/core/"
     }
     fields = [
         Field("name", str, "vocab:name", multiple=False, required=True,
-              doc="Word or phrase that constitutes the distinctive designation of the difference measure."),
-        Field("definition", str, "vocab:definition", multiple=False, required=False,
-              doc="Short, but precise statement of the meaning of a word, word group, sign or a symbol."),
+              doc="Word or phrase that constitutes the distinctive designation of the live paper section."),
         Field("description", str, "vocab:description", multiple=False, required=False,
-              doc="Longer statement or account giving the characteristics of the difference measure."),
-        Field("interlex_identifier", IRI, "vocab:interlexIdentifier", multiple=False, required=False,
-              doc="Persistent identifier for a term registered in the InterLex project."),
-        Field("knowledge_space_link", IRI, "vocab:knowledgeSpaceLink", multiple=False, required=False,
-              doc="Persistent link to an encyclopedia entry in the Knowledge Space project."),
-        Field("preferred_ontology_identifier", IRI, "vocab:preferredOntologyIdentifier", multiple=False, required=False,
-              doc="Persistent identifier of a preferred ontological term."),
-        Field("synonyms", str, "vocab:synonym", multiple=True, required=False,
-              doc="Words or expressions used in the same language that have the same or nearly the same meaning in some or all senses."),
+              doc="Longer statement or account giving the characteristics of the live paper section."),
+        Field("is_part_of", "openminds.publications.LivePaperVersion", "vocab:isPartOf", multiple=False, required=True,
+              doc="Reference to the ensemble of multiple things or beings."),
+        Field("order", int, "vocab:order", multiple=False, required=True,
+              doc="no description available"),
+        Field("section_type", str, "vocab:sectionType", multiple=False, required=True,
+              doc="no description available"),
 
     ]
-    existence_query_fields = ('name',)
+    existence_query_fields = ('name', 'is_part_of', 'order', 'section_type')
```

### Comparing `fairgraph-0.8.2/fairgraph/openminds/controlledterms/disease.py` & `fairgraph-0.9.0/fairgraph/openminds/sands/non_atlas/custom_annotation.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,44 +1,48 @@
 """
-Structured information on a disease.
+
 """
 
 # this file was auto-generated
 
 from datetime import date, datetime
-from fairgraph.base_v3 import KGObject, IRI
+from fairgraph.base_v3 import EmbeddedMetadata, IRI
 from fairgraph.fields import Field
 
 
 
 
-class Disease(KGObject):
+class CustomAnnotation(EmbeddedMetadata):
     """
-    Structured information on a disease.
+
     """
-    default_space = "controlled"
-    type = ["https://openminds.ebrains.eu/controlledTerms/Disease"]
+    type = ["https://openminds.ebrains.eu/sands/CustomAnnotation"]
     context = {
         "schema": "http://schema.org/",
         "kg": "https://kg.ebrains.eu/api/instances/",
         "vocab": "https://openminds.ebrains.eu/vocab/",
         "terms": "https://openminds.ebrains.eu/controlledTerms/",
         "core": "https://openminds.ebrains.eu/core/"
     }
     fields = [
-        Field("name", str, "vocab:name", multiple=False, required=True,
-              doc="Word or phrase that constitutes the distinctive designation of the disease."),
-        Field("definition", str, "vocab:definition", multiple=False, required=False,
-              doc="Short, but precise statement of the meaning of a word, word group, sign or a symbol."),
-        Field("description", str, "vocab:description", multiple=False, required=False,
-              doc="Longer statement or account giving the characteristics of the disease."),
-        Field("interlex_identifier", IRI, "vocab:interlexIdentifier", multiple=False, required=False,
-              doc="Persistent identifier for a term registered in the InterLex project."),
-        Field("knowledge_space_link", IRI, "vocab:knowledgeSpaceLink", multiple=False, required=False,
-              doc="Persistent link to an encyclopedia entry in the Knowledge Space project."),
-        Field("preferred_ontology_identifier", IRI, "vocab:preferredOntologyIdentifier", multiple=False, required=False,
-              doc="Persistent identifier of a preferred ontological term."),
-        Field("synonyms", str, "vocab:synonym", multiple=True, required=False,
-              doc="Words or expressions used in the same language that have the same or nearly the same meaning in some or all senses."),
+        Field("annotation_type", "openminds.controlledterms.AnnotationType", "vocab:annotationType", multiple=False, required=False,
+              doc="no description available"),
+        Field("best_view_point", "openminds.sands.CoordinatePoint", "vocab:bestViewPoint", multiple=False, required=False,
+              doc="Coordinate point from which you get the best view of something."),
+        Field("coordinate_space", ["openminds.sands.CommonCoordinateSpace", "openminds.sands.CustomCoordinateSpace"], "vocab:coordinateSpace", multiple=False, required=True,
+              doc="Two or three dimensional geometric setting."),
+        Field("criteria", "openminds.core.ProtocolExecution", "vocab:criteria", multiple=False, required=False,
+              doc="Aspects or standards on which a judgement or decision is based."),
+        Field("criteria_quality_type", "openminds.controlledterms.CriteriaQualityType", "vocab:criteriaQualityType", multiple=False, required=True,
+              doc="Distinct class that defines how the judgement or decision was made for a particular criteria."),
+        Field("display_color", str, "vocab:displayColor", multiple=False, required=False,
+              doc="Preferred coloring."),
+        Field("inspired_bys", "openminds.core.File", "vocab:inspiredBy", multiple=True, required=False,
+              doc="Reference to an inspiring element."),
+        Field("internal_identifier", str, "vocab:internalIdentifier", multiple=False, required=True,
+              doc="Term or code that identifies the custom annotation within a particular product."),
+        Field("laterality", "openminds.controlledterms.Laterality", "vocab:laterality", multiple=True, required=False,
+              doc="Differentiation between a pair of lateral homologous parts of the body."),
+        Field("visualized_in", "openminds.core.File", "vocab:visualizedIn", multiple=False, required=True,
+              doc="Reference to an image in which something is visible."),
 
     ]
-    existence_query_fields = ('name',)
```

### Comparing `fairgraph-0.8.2/fairgraph/openminds/controlledterms/disease_model.py` & `fairgraph-0.9.0/fairgraph/openminds/core/research/subject.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,44 +1,42 @@
 """
-
+Structured information on a subject.
 """
 
 # this file was auto-generated
 
 from datetime import date, datetime
 from fairgraph.base_v3 import KGObject, IRI
 from fairgraph.fields import Field
 
 
 
 
-class DiseaseModel(KGObject):
+class Subject(KGObject):
     """
-
+    Structured information on a subject.
     """
-    default_space = "controlled"
-    type = ["https://openminds.ebrains.eu/controlledTerms/DiseaseModel"]
+    default_space = "dataset"
+    type = ["https://openminds.ebrains.eu/core/Subject"]
     context = {
         "schema": "http://schema.org/",
         "kg": "https://kg.ebrains.eu/api/instances/",
         "vocab": "https://openminds.ebrains.eu/vocab/",
         "terms": "https://openminds.ebrains.eu/controlledTerms/",
         "core": "https://openminds.ebrains.eu/core/"
     }
     fields = [
-        Field("name", str, "vocab:name", multiple=False, required=True,
-              doc="Word or phrase that constitutes the distinctive designation of the disease model."),
-        Field("definition", str, "vocab:definition", multiple=False, required=False,
-              doc="Short, but precise statement of the meaning of a word, word group, sign or a symbol."),
-        Field("description", str, "vocab:description", multiple=False, required=False,
-              doc="Longer statement or account giving the characteristics of the disease model."),
-        Field("interlex_identifier", IRI, "vocab:interlexIdentifier", multiple=False, required=False,
-              doc="Persistent identifier for a term registered in the InterLex project."),
-        Field("knowledge_space_link", IRI, "vocab:knowledgeSpaceLink", multiple=False, required=False,
-              doc="Persistent link to an encyclopedia entry in the Knowledge Space project."),
-        Field("preferred_ontology_identifier", IRI, "vocab:preferredOntologyIdentifier", multiple=False, required=False,
-              doc="Persistent identifier of a preferred ontological term."),
-        Field("synonyms", str, "vocab:synonym", multiple=True, required=False,
-              doc="Words or expressions used in the same language that have the same or nearly the same meaning in some or all senses."),
+        Field("lookup_label", str, "vocab:lookupLabel", multiple=False, required=False,
+              doc="no description available"),
+        Field("biological_sex", "openminds.controlledterms.BiologicalSex", "vocab:biologicalSex", multiple=False, required=False,
+              doc="Differentiation of individuals of most species (animals and plants) based on the type of gametes they produce."),
+        Field("internal_identifier", str, "vocab:internalIdentifier", multiple=False, required=False,
+              doc="Term or code that identifies the subject within a particular product."),
+        Field("is_part_of", "openminds.core.SubjectGroup", "vocab:isPartOf", multiple=True, required=False,
+              doc="Reference to the ensemble of multiple things or beings."),
+        Field("species", ["openminds.controlledterms.Species", "openminds.core.Strain"], "vocab:species", multiple=False, required=True,
+              doc="Category of biological classification comprising related organisms or populations potentially capable of interbreeding, and being designated by a binomial that consists of the name of a genus followed by a Latin or latinized uncapitalized noun or adjective."),
+        Field("studied_states", "openminds.core.SubjectState", "vocab:studiedState", multiple=True, required=True,
+              doc="Reference to a point in time at which the subject was studied in a particular mode or condition."),
 
     ]
-    existence_query_fields = ('name',)
+    existence_query_fields = ('lookup_label',)
```

### Comparing `fairgraph-0.8.2/fairgraph/openminds/controlledterms/ethics_assessment.py` & `fairgraph-0.9.0/fairgraph/openminds/controlledterms/olfactory_stimulus_type.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,40 +1,56 @@
 """
-Structured information on the ethics assessment of a dataset.
+
+
+    .. list-table:: **Possible values**
+       :widths: 20 80
+       :header-rows: 0
+
+       * - floral odor
+         - Any chemical compound that smells floral.
+
 """
 
 # this file was auto-generated
 
 from datetime import date, datetime
 from fairgraph.base_v3 import KGObject, IRI
 from fairgraph.fields import Field
 
 
 
 
-class EthicsAssessment(KGObject):
+class OlfactoryStimulusType(KGObject):
     """
-    Structured information on the ethics assessment of a dataset.
+
+
+    .. list-table:: **Possible values**
+       :widths: 20 80
+       :header-rows: 0
+
+       * - floral odor
+         - Any chemical compound that smells floral.
+
     """
     default_space = "controlled"
-    type = ["https://openminds.ebrains.eu/controlledTerms/EthicsAssessment"]
+    type = ["https://openminds.ebrains.eu/controlledTerms/OlfactoryStimulusType"]
     context = {
         "schema": "http://schema.org/",
         "kg": "https://kg.ebrains.eu/api/instances/",
         "vocab": "https://openminds.ebrains.eu/vocab/",
         "terms": "https://openminds.ebrains.eu/controlledTerms/",
         "core": "https://openminds.ebrains.eu/core/"
     }
     fields = [
         Field("name", str, "vocab:name", multiple=False, required=True,
-              doc="Word or phrase that constitutes the distinctive designation of the ethics assessment."),
+              doc="Word or phrase that constitutes the distinctive designation of the olfactory stimulus type."),
         Field("definition", str, "vocab:definition", multiple=False, required=False,
               doc="Short, but precise statement of the meaning of a word, word group, sign or a symbol."),
         Field("description", str, "vocab:description", multiple=False, required=False,
-              doc="Longer statement or account giving the characteristics of the ethics assessment."),
+              doc="Longer statement or account giving the characteristics of the olfactory stimulus type."),
         Field("interlex_identifier", IRI, "vocab:interlexIdentifier", multiple=False, required=False,
               doc="Persistent identifier for a term registered in the InterLex project."),
         Field("knowledge_space_link", IRI, "vocab:knowledgeSpaceLink", multiple=False, required=False,
               doc="Persistent link to an encyclopedia entry in the Knowledge Space project."),
         Field("preferred_ontology_identifier", IRI, "vocab:preferredOntologyIdentifier", multiple=False, required=False,
               doc="Persistent identifier of a preferred ontological term."),
         Field("synonyms", str, "vocab:synonym", multiple=True, required=False,
```

### Comparing `fairgraph-0.8.2/fairgraph/openminds/controlledterms/experimental_approach.py` & `fairgraph-0.9.0/fairgraph/openminds/ephys/device/pipette.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,38 +7,48 @@
 from datetime import date, datetime
 from fairgraph.base_v3 import KGObject, IRI
 from fairgraph.fields import Field
 
 
 
 
-class ExperimentalApproach(KGObject):
+class Pipette(KGObject):
     """
 
     """
-    default_space = "controlled"
-    type = ["https://openminds.ebrains.eu/controlledTerms/ExperimentalApproach"]
+    default_space = "in-depth"
+    type = ["https://openminds.ebrains.eu/ephys/Pipette"]
     context = {
         "schema": "http://schema.org/",
         "kg": "https://kg.ebrains.eu/api/instances/",
         "vocab": "https://openminds.ebrains.eu/vocab/",
         "terms": "https://openminds.ebrains.eu/controlledTerms/",
         "core": "https://openminds.ebrains.eu/core/"
     }
     fields = [
         Field("name", str, "vocab:name", multiple=False, required=True,
-              doc="Word or phrase that constitutes the distinctive designation of the experimental approach."),
-        Field("definition", str, "vocab:definition", multiple=False, required=False,
-              doc="Short, but precise statement of the meaning of a word, word group, sign or a symbol."),
+              doc="Word or phrase that constitutes the distinctive designation of the pipette."),
+        Field("lookup_label", str, "vocab:lookupLabel", multiple=False, required=False,
+              doc="no description available"),
         Field("description", str, "vocab:description", multiple=False, required=False,
-              doc="Longer statement or account giving the characteristics of the experimental approach."),
-        Field("interlex_identifier", IRI, "vocab:interlexIdentifier", multiple=False, required=False,
-              doc="Persistent identifier for a term registered in the InterLex project."),
-        Field("knowledge_space_link", IRI, "vocab:knowledgeSpaceLink", multiple=False, required=False,
-              doc="Persistent link to an encyclopedia entry in the Knowledge Space project."),
-        Field("preferred_ontology_identifier", IRI, "vocab:preferredOntologyIdentifier", multiple=False, required=False,
-              doc="Persistent identifier of a preferred ontological term."),
-        Field("synonyms", str, "vocab:synonym", multiple=True, required=False,
-              doc="Words or expressions used in the same language that have the same or nearly the same meaning in some or all senses."),
+              doc="Longer statement or account giving the characteristics of the pipette."),
+        Field("device_type", "openminds.controlledterms.DeviceType", "vocab:deviceType", multiple=False, required=False,
+              doc="no description available"),
+        Field("digital_identifier", ["openminds.core.DOI", "openminds.core.RRID"], "vocab:digitalIdentifier", multiple=False, required=False,
+              doc="Digital handle to identify objects or legal persons."),
+        Field("external_diameter", "openminds.core.QuantitativeValue", "vocab:externalDiameter", multiple=False, required=False,
+              doc="no description available"),
+        Field("internal_diameter", "openminds.core.QuantitativeValue", "vocab:internalDiameter", multiple=False, required=False,
+              doc="no description available"),
+        Field("internal_identifier", str, "vocab:internalIdentifier", multiple=False, required=False,
+              doc="Term or code that identifies the pipette within a particular product."),
+        Field("manufacturers", ["openminds.core.Consortium", "openminds.core.Organization", "openminds.core.Person"], "vocab:manufacturer", multiple=True, required=True,
+              doc="no description available"),
+        Field("material", ["openminds.chemicals.ChemicalMixture", "openminds.chemicals.ChemicalSubstance", "openminds.controlledterms.MolecularEntity"], "vocab:material", multiple=False, required=False,
+              doc="no description available"),
+        Field("owners", ["openminds.core.Consortium", "openminds.core.Organization", "openminds.core.Person"], "vocab:owner", multiple=True, required=False,
+              doc="no description available"),
+        Field("serial_number", str, "vocab:serialNumber", multiple=False, required=False,
+              doc="no description available"),
 
     ]
-    existence_query_fields = ('name',)
+    existence_query_fields = ('lookup_label',)
```

### Comparing `fairgraph-0.8.2/fairgraph/openminds/controlledterms/file_bundle_grouping.py` & `fairgraph-0.9.0/fairgraph/openminds/sands/atlas/atlas_annotation.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,44 +1,46 @@
 """
-Structured information on the grouping mechanism of a file bundle.
+
 """
 
 # this file was auto-generated
 
 from datetime import date, datetime
-from fairgraph.base_v3 import KGObject, IRI
+from fairgraph.base_v3 import EmbeddedMetadata, IRI
 from fairgraph.fields import Field
 
 
 
 
-class FileBundleGrouping(KGObject):
+class AtlasAnnotation(EmbeddedMetadata):
     """
-    Structured information on the grouping mechanism of a file bundle.
+
     """
-    default_space = "controlled"
-    type = ["https://openminds.ebrains.eu/controlledTerms/FileBundleGrouping"]
+    type = ["https://openminds.ebrains.eu/sands/AtlasAnnotation"]
     context = {
         "schema": "http://schema.org/",
         "kg": "https://kg.ebrains.eu/api/instances/",
         "vocab": "https://openminds.ebrains.eu/vocab/",
         "terms": "https://openminds.ebrains.eu/controlledTerms/",
         "core": "https://openminds.ebrains.eu/core/"
     }
     fields = [
-        Field("name", str, "vocab:name", multiple=False, required=True,
-              doc="Word or phrase that constitutes the distinctive designation of the file bundle grouping."),
-        Field("definition", str, "vocab:definition", multiple=False, required=False,
-              doc="Short, but precise statement of the meaning of a word, word group, sign or a symbol."),
-        Field("description", str, "vocab:description", multiple=False, required=False,
-              doc="Longer statement or account giving the characteristics of the file bundle grouping."),
-        Field("interlex_identifier", IRI, "vocab:interlexIdentifier", multiple=False, required=False,
-              doc="Persistent identifier for a term registered in the InterLex project."),
-        Field("knowledge_space_link", IRI, "vocab:knowledgeSpaceLink", multiple=False, required=False,
-              doc="Persistent link to an encyclopedia entry in the Knowledge Space project."),
-        Field("preferred_ontology_identifier", IRI, "vocab:preferredOntologyIdentifier", multiple=False, required=False,
-              doc="Persistent identifier of a preferred ontological term."),
-        Field("synonyms", str, "vocab:synonym", multiple=True, required=False,
-              doc="Words or expressions used in the same language that have the same or nearly the same meaning in some or all senses."),
+        Field("annotation_type", "openminds.controlledterms.AnnotationType", "vocab:annotationType", multiple=False, required=False,
+              doc="no description available"),
+        Field("best_view_point", "openminds.sands.CoordinatePoint", "vocab:bestViewPoint", multiple=False, required=False,
+              doc="Coordinate point from which you get the best view of something."),
+        Field("criteria", "openminds.core.ProtocolExecution", "vocab:criteria", multiple=False, required=False,
+              doc="Aspects or standards on which a judgement or decision is based."),
+        Field("criteria_quality_type", "openminds.controlledterms.CriteriaQualityType", "vocab:criteriaQualityType", multiple=False, required=True,
+              doc="Distinct class that defines how the judgement or decision was made for a particular criteria."),
+        Field("display_color", str, "vocab:displayColor", multiple=False, required=False,
+              doc="Preferred coloring."),
+        Field("inspired_bys", "openminds.core.File", "vocab:inspiredBy", multiple=True, required=False,
+              doc="Reference to an inspiring element."),
+        Field("internal_identifier", str, "vocab:internalIdentifier", multiple=False, required=True,
+              doc="Term or code that identifies the atlas annotation within a particular product."),
+        Field("laterality", "openminds.controlledterms.Laterality", "vocab:laterality", multiple=True, required=False,
+              doc="Differentiation between a pair of lateral homologous parts of the body."),
+        Field("visualized_in", "openminds.core.File", "vocab:visualizedIn", multiple=False, required=False,
+              doc="Reference to an image in which something is visible."),
 
     ]
-    existence_query_fields = ('name',)
```

### Comparing `fairgraph-0.8.2/fairgraph/openminds/controlledterms/file_repository_type.py` & `fairgraph-0.9.0/fairgraph/openminds/controlledterms/file_bundle_grouping.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,40 +1,92 @@
 """
+Structured information on the grouping mechanism of a file bundle.
+
+    .. list-table:: **Possible values**
+       :widths: 20 80
+       :header-rows: 0
+
+       * - technique
+         -
+       * - subject group
+         -
+       * - tissue sample
+         -
+       * - behavioral task
+         -
+       * - coordinate space
+         -
+       * - protocol
+         -
+       * - behavioral protocol
+         -
+       * - study target
+         -
+       * - subject
+         -
+       * - tissue sample collection
+         -
 
 """
 
 # this file was auto-generated
 
 from datetime import date, datetime
 from fairgraph.base_v3 import KGObject, IRI
 from fairgraph.fields import Field
 
 
 
 
-class FileRepositoryType(KGObject):
+class FileBundleGrouping(KGObject):
     """
+    Structured information on the grouping mechanism of a file bundle.
+
+    .. list-table:: **Possible values**
+       :widths: 20 80
+       :header-rows: 0
+
+       * - technique
+         -
+       * - subject group
+         -
+       * - tissue sample
+         -
+       * - behavioral task
+         -
+       * - coordinate space
+         -
+       * - protocol
+         -
+       * - behavioral protocol
+         -
+       * - study target
+         -
+       * - subject
+         -
+       * - tissue sample collection
+         -
 
     """
     default_space = "controlled"
-    type = ["https://openminds.ebrains.eu/controlledTerms/FileRepositoryType"]
+    type = ["https://openminds.ebrains.eu/controlledTerms/FileBundleGrouping"]
     context = {
         "schema": "http://schema.org/",
         "kg": "https://kg.ebrains.eu/api/instances/",
         "vocab": "https://openminds.ebrains.eu/vocab/",
         "terms": "https://openminds.ebrains.eu/controlledTerms/",
         "core": "https://openminds.ebrains.eu/core/"
     }
     fields = [
         Field("name", str, "vocab:name", multiple=False, required=True,
-              doc="Word or phrase that constitutes the distinctive designation of the file repository type."),
+              doc="Word or phrase that constitutes the distinctive designation of the file bundle grouping."),
         Field("definition", str, "vocab:definition", multiple=False, required=False,
               doc="Short, but precise statement of the meaning of a word, word group, sign or a symbol."),
         Field("description", str, "vocab:description", multiple=False, required=False,
-              doc="Longer statement or account giving the characteristics of the file repository type."),
+              doc="Longer statement or account giving the characteristics of the file bundle grouping."),
         Field("interlex_identifier", IRI, "vocab:interlexIdentifier", multiple=False, required=False,
               doc="Persistent identifier for a term registered in the InterLex project."),
         Field("knowledge_space_link", IRI, "vocab:knowledgeSpaceLink", multiple=False, required=False,
               doc="Persistent link to an encyclopedia entry in the Knowledge Space project."),
         Field("preferred_ontology_identifier", IRI, "vocab:preferredOntologyIdentifier", multiple=False, required=False,
               doc="Persistent identifier of a preferred ontological term."),
         Field("synonyms", str, "vocab:synonym", multiple=True, required=False,
```

### Comparing `fairgraph-0.8.2/fairgraph/openminds/controlledterms/file_usage_role.py` & `fairgraph-0.9.0/fairgraph/openminds/core/products/meta_data_model.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,44 +1,48 @@
 """
-Structured information on the usage role of a file instance or bundle.
+
 """
 
 # this file was auto-generated
 
 from datetime import date, datetime
 from fairgraph.base_v3 import KGObject, IRI
 from fairgraph.fields import Field
 
 
 
 
-class FileUsageRole(KGObject):
+class MetaDataModel(KGObject):
     """
-    Structured information on the usage role of a file instance or bundle.
+
     """
-    default_space = "controlled"
-    type = ["https://openminds.ebrains.eu/controlledTerms/FileUsageRole"]
+    default_space = "metadatamodel"
+    type = ["https://openminds.ebrains.eu/core/MetaDataModel"]
     context = {
         "schema": "http://schema.org/",
         "kg": "https://kg.ebrains.eu/api/instances/",
         "vocab": "https://openminds.ebrains.eu/vocab/",
         "terms": "https://openminds.ebrains.eu/controlledTerms/",
         "core": "https://openminds.ebrains.eu/core/"
     }
     fields = [
-        Field("name", str, "vocab:name", multiple=False, required=True,
-              doc="Word or phrase that constitutes the distinctive designation of the file usage role."),
-        Field("definition", str, "vocab:definition", multiple=False, required=False,
-              doc="Short, but precise statement of the meaning of a word, word group, sign or a symbol."),
-        Field("description", str, "vocab:description", multiple=False, required=False,
-              doc="Longer statement or account giving the characteristics of the file usage role."),
-        Field("interlex_identifier", IRI, "vocab:interlexIdentifier", multiple=False, required=False,
-              doc="Persistent identifier for a term registered in the InterLex project."),
-        Field("knowledge_space_link", IRI, "vocab:knowledgeSpaceLink", multiple=False, required=False,
-              doc="Persistent link to an encyclopedia entry in the Knowledge Space project."),
-        Field("preferred_ontology_identifier", IRI, "vocab:preferredOntologyIdentifier", multiple=False, required=False,
-              doc="Persistent identifier of a preferred ontological term."),
-        Field("synonyms", str, "vocab:synonym", multiple=True, required=False,
-              doc="Words or expressions used in the same language that have the same or nearly the same meaning in some or all senses."),
+        Field("name", str, "vocab:fullName", multiple=False, required=True,
+              doc="Whole, non-abbreviated name of the meta data model."),
+        Field("alias", str, "vocab:shortName", multiple=False, required=True,
+              doc="Shortened or fully abbreviated name of the meta data model."),
+        Field("custodians", ["openminds.core.Consortium", "openminds.core.Organization", "openminds.core.Person"], "vocab:custodian", multiple=True, required=False,
+              doc="The 'custodian' is a legal person who is responsible for the content and quality of the data, metadata, and/or code of a research product."),
+        Field("description", str, "vocab:description", multiple=False, required=True,
+              doc="Longer statement or account giving the characteristics of the meta data model."),
+        Field("developers", ["openminds.core.Consortium", "openminds.core.Organization", "openminds.core.Person"], "vocab:developer", multiple=True, required=True,
+              doc="Legal person that creates or improves products or services (e.g., software, applications, etc.)."),
+        Field("digital_identifier", ["openminds.core.DOI", "openminds.core.SWHID"], "vocab:digitalIdentifier", multiple=False, required=False,
+              doc="Digital handle to identify objects or legal persons."),
+        Field("versions", "openminds.core.MetaDataModelVersion", "vocab:hasVersion", multiple=True, required=True,
+              doc="Reference to variants of an original."),
+        Field("homepage", "openminds.core.URL", "vocab:homepage", multiple=False, required=False,
+              doc="Main website of the meta data model."),
+        Field("how_to_cite", str, "vocab:howToCite", multiple=False, required=False,
+              doc="Preferred format for citing a particular object or legal person."),
 
     ]
-    existence_query_fields = ('name',)
+    existence_query_fields = ('alias',)
```

### Comparing `fairgraph-0.8.2/fairgraph/openminds/controlledterms/genetic_strain_type.py` & `fairgraph-0.9.0/fairgraph/openminds/publications/live_paper_resource_item.py`

 * *Files 17% similar despite different names*

```diff
@@ -7,38 +7,33 @@
 from datetime import date, datetime
 from fairgraph.base_v3 import KGObject, IRI
 from fairgraph.fields import Field
 
 
 
 
-class GeneticStrainType(KGObject):
+class LivePaperResourceItem(KGObject):
     """
 
     """
-    default_space = "controlled"
-    type = ["https://openminds.ebrains.eu/controlledTerms/GeneticStrainType"]
+    default_space = "livepapers"
+    type = ["https://openminds.ebrains.eu/publications/LivePaperResourceItem"]
     context = {
         "schema": "http://schema.org/",
         "kg": "https://kg.ebrains.eu/api/instances/",
         "vocab": "https://openminds.ebrains.eu/vocab/",
         "terms": "https://openminds.ebrains.eu/controlledTerms/",
         "core": "https://openminds.ebrains.eu/core/"
     }
     fields = [
         Field("name", str, "vocab:name", multiple=False, required=True,
-              doc="Word or phrase that constitutes the distinctive designation of the genetic strain type."),
-        Field("definition", str, "vocab:definition", multiple=False, required=False,
-              doc="Short, but precise statement of the meaning of a word, word group, sign or a symbol."),
-        Field("description", str, "vocab:description", multiple=False, required=False,
-              doc="Longer statement or account giving the characteristics of the genetic strain type."),
-        Field("interlex_identifier", IRI, "vocab:interlexIdentifier", multiple=False, required=False,
-              doc="Persistent identifier for a term registered in the InterLex project."),
-        Field("knowledge_space_link", IRI, "vocab:knowledgeSpaceLink", multiple=False, required=False,
-              doc="Persistent link to an encyclopedia entry in the Knowledge Space project."),
-        Field("preferred_ontology_identifier", IRI, "vocab:preferredOntologyIdentifier", multiple=False, required=False,
-              doc="Persistent identifier of a preferred ontological term."),
-        Field("synonyms", str, "vocab:synonym", multiple=True, required=False,
-              doc="Words or expressions used in the same language that have the same or nearly the same meaning in some or all senses."),
+              doc="Word or phrase that constitutes the distinctive designation of the live paper resource item."),
+        Field("iri", IRI, "vocab:IRI", multiple=False, required=True,
+              doc="Stands for Internationalized Resource Identifier which is an internet protocol standard that builds on the URI protocol, extending the set of permitted characters to include Unicode/ISO 10646."),
+        Field("hosted_by", "openminds.core.Organization", "vocab:hostedBy", multiple=False, required=True,
+              doc="Reference to an organization that provides facilities and services for something."),
+        Field("is_part_of", "openminds.publications.LivePaperSection", "vocab:isPartOf", multiple=False, required=True,
+              doc="Reference to the ensemble of multiple things or beings."),
 
     ]
-    existence_query_fields = ('name',)
+    #existence_query_fields = ('name', 'iri', 'hosted_by', 'is_part_of')
+    existence_query_fields = ('name', 'iri', 'is_part_of')
```

### Comparing `fairgraph-0.8.2/fairgraph/openminds/controlledterms/handedness.py` & `fairgraph-0.9.0/fairgraph/openminds/ephys/device/electrode.py`

 * *Files 18% similar despite different names*

```diff
@@ -7,38 +7,48 @@
 from datetime import date, datetime
 from fairgraph.base_v3 import KGObject, IRI
 from fairgraph.fields import Field
 
 
 
 
-class Handedness(KGObject):
+class Electrode(KGObject):
     """
 
     """
-    default_space = "controlled"
-    type = ["https://openminds.ebrains.eu/controlledTerms/Handedness"]
+    default_space = "in-depth"
+    type = ["https://openminds.ebrains.eu/ephys/Electrode"]
     context = {
         "schema": "http://schema.org/",
         "kg": "https://kg.ebrains.eu/api/instances/",
         "vocab": "https://openminds.ebrains.eu/vocab/",
         "terms": "https://openminds.ebrains.eu/controlledTerms/",
         "core": "https://openminds.ebrains.eu/core/"
     }
     fields = [
         Field("name", str, "vocab:name", multiple=False, required=True,
-              doc="Word or phrase that constitutes the distinctive designation of the handedness."),
-        Field("definition", str, "vocab:definition", multiple=False, required=False,
-              doc="Short, but precise statement of the meaning of a word, word group, sign or a symbol."),
+              doc="Word or phrase that constitutes the distinctive designation of the electrode."),
+        Field("lookup_label", str, "vocab:lookupLabel", multiple=False, required=False,
+              doc="no description available"),
+        Field("conductor_material", ["openminds.chemicals.ChemicalMixture", "openminds.chemicals.ChemicalSubstance", "openminds.controlledterms.MolecularEntity"], "vocab:conductorMaterial", multiple=False, required=False,
+              doc="no description available"),
         Field("description", str, "vocab:description", multiple=False, required=False,
-              doc="Longer statement or account giving the characteristics of the handedness."),
-        Field("interlex_identifier", IRI, "vocab:interlexIdentifier", multiple=False, required=False,
-              doc="Persistent identifier for a term registered in the InterLex project."),
-        Field("knowledge_space_link", IRI, "vocab:knowledgeSpaceLink", multiple=False, required=False,
-              doc="Persistent link to an encyclopedia entry in the Knowledge Space project."),
-        Field("preferred_ontology_identifier", IRI, "vocab:preferredOntologyIdentifier", multiple=False, required=False,
-              doc="Persistent identifier of a preferred ontological term."),
-        Field("synonyms", str, "vocab:synonym", multiple=True, required=False,
-              doc="Words or expressions used in the same language that have the same or nearly the same meaning in some or all senses."),
+              doc="Longer statement or account giving the characteristics of the electrode."),
+        Field("device_type", "openminds.controlledterms.DeviceType", "vocab:deviceType", multiple=False, required=False,
+              doc="no description available"),
+        Field("digital_identifier", ["openminds.core.DOI", "openminds.core.RRID"], "vocab:digitalIdentifier", multiple=False, required=False,
+              doc="Digital handle to identify objects or legal persons."),
+        Field("insulator_material", ["openminds.chemicals.ChemicalMixture", "openminds.chemicals.ChemicalSubstance", "openminds.controlledterms.MolecularEntity"], "vocab:insulatorMaterial", multiple=False, required=False,
+              doc="no description available"),
+        Field("internal_identifier", str, "vocab:internalIdentifier", multiple=False, required=False,
+              doc="Term or code that identifies the electrode within a particular product."),
+        Field("intrinsic_resistance", ["openminds.core.QuantitativeValue", "openminds.core.QuantitativeValueRange"], "vocab:intrinsicResistance", multiple=False, required=False,
+              doc="no description available"),
+        Field("manufacturers", ["openminds.core.Consortium", "openminds.core.Organization", "openminds.core.Person"], "vocab:manufacturer", multiple=True, required=True,
+              doc="no description available"),
+        Field("owners", ["openminds.core.Consortium", "openminds.core.Organization", "openminds.core.Person"], "vocab:owner", multiple=True, required=False,
+              doc="no description available"),
+        Field("serial_number", str, "vocab:serialNumber", multiple=False, required=False,
+              doc="no description available"),
 
     ]
-    existence_query_fields = ('name',)
+    existence_query_fields = ('lookup_label',)
```

### Comparing `fairgraph-0.8.2/fairgraph/openminds/controlledterms/language.py` & `fairgraph-0.9.0/fairgraph/openminds/core/data/file_repository.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,44 +1,48 @@
 """
-Structured information on the available language setting.
+Structured information on a file repository.
 """
 
 # this file was auto-generated
 
 from datetime import date, datetime
 from fairgraph.base_v3 import KGObject, IRI
 from fairgraph.fields import Field
 
 
 
 
-class Language(KGObject):
+class FileRepository(KGObject):
     """
-    Structured information on the available language setting.
+    Structured information on a file repository.
     """
-    default_space = "controlled"
-    type = ["https://openminds.ebrains.eu/controlledTerms/Language"]
+    default_space = "dataset"
+    type = ["https://openminds.ebrains.eu/core/FileRepository"]
     context = {
         "schema": "http://schema.org/",
         "kg": "https://kg.ebrains.eu/api/instances/",
         "vocab": "https://openminds.ebrains.eu/vocab/",
         "terms": "https://openminds.ebrains.eu/controlledTerms/",
         "core": "https://openminds.ebrains.eu/core/"
     }
     fields = [
         Field("name", str, "vocab:name", multiple=False, required=True,
-              doc="Word or phrase that constitutes the distinctive designation of the language."),
-        Field("definition", str, "vocab:definition", multiple=False, required=False,
-              doc="Short, but precise statement of the meaning of a word, word group, sign or a symbol."),
-        Field("description", str, "vocab:description", multiple=False, required=False,
-              doc="Longer statement or account giving the characteristics of the language."),
-        Field("interlex_identifier", IRI, "vocab:interlexIdentifier", multiple=False, required=False,
-              doc="Persistent identifier for a term registered in the InterLex project."),
-        Field("knowledge_space_link", IRI, "vocab:knowledgeSpaceLink", multiple=False, required=False,
-              doc="Persistent link to an encyclopedia entry in the Knowledge Space project."),
-        Field("preferred_ontology_identifier", IRI, "vocab:preferredOntologyIdentifier", multiple=False, required=False,
-              doc="Persistent identifier of a preferred ontological term."),
-        Field("synonyms", str, "vocab:synonym", multiple=True, required=False,
-              doc="Words or expressions used in the same language that have the same or nearly the same meaning in some or all senses."),
+              doc="Word or phrase that constitutes the distinctive designation of the file repository."),
+        Field("iri", IRI, "vocab:IRI", multiple=False, required=True,
+              doc="Stands for Internationalized Resource Identifier which is an internet protocol standard that builds on the URI protocol, extending the set of permitted characters to include Unicode/ISO 10646."),
+        Field("content_type_patterns", "openminds.core.ContentTypePattern", "vocab:contentTypePattern", multiple=True, required=False,
+              doc="no description available"),
+        Field("format", "openminds.core.ContentType", "vocab:format", multiple=False, required=False,
+              doc="Method of digitally organizing and structuring data or information."),
+        Field("hash", "openminds.core.Hash", "vocab:hash", multiple=False, required=False,
+              doc="Term used for the process of converting any data into a single value. Often also directly refers to the resulting single value."),
+        Field("hosted_by", "openminds.core.Organization", "vocab:hostedBy", multiple=False, required=True,
+              doc="Reference to an organization that provides facilities and services for something."),
+        Field("repository_type", "openminds.controlledterms.FileRepositoryType", "vocab:repositoryType", multiple=False, required=False,
+              doc="no description available"),
+        Field("storage_size", "openminds.core.QuantitativeValue", "vocab:storageSize", multiple=False, required=False,
+              doc="Quantitative value defining how much disk space is used by an object on a computer system."),
+        Field("structure_pattern", "openminds.core.FileRepositoryStructure", "vocab:structurePattern", multiple=False, required=False,
+              doc="no description available"),
 
     ]
-    existence_query_fields = ('name',)
+    existence_query_fields = ('iri',)
```

### Comparing `fairgraph-0.8.2/fairgraph/openminds/controlledterms/laterality.py` & `fairgraph-0.9.0/fairgraph/openminds/ephys/device/electrode_usage.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,44 +1,44 @@
 """
-Structured information on the lateral direction.
+
 """
 
 # this file was auto-generated
 
 from datetime import date, datetime
 from fairgraph.base_v3 import KGObject, IRI
 from fairgraph.fields import Field
 
 
 
 
-class Laterality(KGObject):
+class ElectrodeUsage(KGObject):
     """
-    Structured information on the lateral direction.
+
     """
-    default_space = "controlled"
-    type = ["https://openminds.ebrains.eu/controlledTerms/Laterality"]
+    default_space = "in-depth"
+    type = ["https://openminds.ebrains.eu/ephys/ElectrodeUsage"]
     context = {
         "schema": "http://schema.org/",
         "kg": "https://kg.ebrains.eu/api/instances/",
         "vocab": "https://openminds.ebrains.eu/vocab/",
         "terms": "https://openminds.ebrains.eu/controlledTerms/",
         "core": "https://openminds.ebrains.eu/core/"
     }
     fields = [
-        Field("name", str, "vocab:name", multiple=False, required=True,
-              doc="Word or phrase that constitutes the distinctive designation of the laterality."),
-        Field("definition", str, "vocab:definition", multiple=False, required=False,
-              doc="Short, but precise statement of the meaning of a word, word group, sign or a symbol."),
-        Field("description", str, "vocab:description", multiple=False, required=False,
-              doc="Longer statement or account giving the characteristics of the laterality."),
-        Field("interlex_identifier", IRI, "vocab:interlexIdentifier", multiple=False, required=False,
-              doc="Persistent identifier for a term registered in the InterLex project."),
-        Field("knowledge_space_link", IRI, "vocab:knowledgeSpaceLink", multiple=False, required=False,
-              doc="Persistent link to an encyclopedia entry in the Knowledge Space project."),
-        Field("preferred_ontology_identifier", IRI, "vocab:preferredOntologyIdentifier", multiple=False, required=False,
-              doc="Persistent identifier of a preferred ontological term."),
-        Field("synonyms", str, "vocab:synonym", multiple=True, required=False,
-              doc="Words or expressions used in the same language that have the same or nearly the same meaning in some or all senses."),
+        Field("lookup_label", str, "vocab:lookupLabel", multiple=False, required=False,
+              doc="no description available"),
+        Field("additional_informations", ["openminds.core.File", "openminds.core.FileBundle"], "vocab:additionalInformation", multiple=True, required=False,
+              doc="no description available"),
+        Field("anatomical_location", ["openminds.controlledterms.UBERONParcellation", "openminds.sands.CustomAnatomicalEntity", "openminds.sands.ParcellationEntity", "openminds.sands.ParcellationEntityVersion"], "vocab:anatomicalLocation", multiple=False, required=False,
+              doc="no description available"),
+        Field("contact_resistance", ["openminds.core.QuantitativeValue", "openminds.core.QuantitativeValueRange"], "vocab:contactResistance", multiple=False, required=False,
+              doc="no description available"),
+        Field("coordinate_point", "openminds.sands.CoordinatePoint", "vocab:coordinatePoint", multiple=False, required=False,
+              doc="Pair or triplet of numbers defining the position in a particular two- or three dimensional plane or space."),
+        Field("electrode", "openminds.ephys.Electrode", "vocab:electrode", multiple=False, required=True,
+              doc="no description available"),
+        Field("used_specimen", ["openminds.core.SubjectState", "openminds.core.TissueSampleState"], "vocab:usedSpecimen", multiple=False, required=False,
+              doc="no description available"),
 
     ]
-    existence_query_fields = ('name',)
+    existence_query_fields = ('lookup_label',)
```

### Comparing `fairgraph-0.8.2/fairgraph/openminds/controlledterms/measured_quantity.py` & `fairgraph-0.9.0/fairgraph/openminds/core/actors/consortium.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,44 +1,38 @@
 """
-
+Structured information about an association of two or more persons or organizations, with the objective of participating in a common activity.
 """
 
 # this file was auto-generated
 
 from datetime import date, datetime
 from fairgraph.base_v3 import KGObject, IRI
 from fairgraph.fields import Field
 
 
 
 
-class MeasuredQuantity(KGObject):
+class Consortium(KGObject):
     """
-
+    Structured information about an association of two or more persons or organizations, with the objective of participating in a common activity.
     """
-    default_space = "controlled"
-    type = ["https://openminds.ebrains.eu/controlledTerms/MeasuredQuantity"]
+    default_space = "common"
+    type = ["https://openminds.ebrains.eu/core/Consortium"]
     context = {
         "schema": "http://schema.org/",
         "kg": "https://kg.ebrains.eu/api/instances/",
         "vocab": "https://openminds.ebrains.eu/vocab/",
         "terms": "https://openminds.ebrains.eu/controlledTerms/",
         "core": "https://openminds.ebrains.eu/core/"
     }
     fields = [
-        Field("name", str, "vocab:name", multiple=False, required=True,
-              doc="Word or phrase that constitutes the distinctive designation of the measured quantity."),
-        Field("definition", str, "vocab:definition", multiple=False, required=False,
-              doc="Short, but precise statement of the meaning of a word, word group, sign or a symbol."),
-        Field("description", str, "vocab:description", multiple=False, required=False,
-              doc="Longer statement or account giving the characteristics of the measured quantity."),
-        Field("interlex_identifier", IRI, "vocab:interlexIdentifier", multiple=False, required=False,
-              doc="Persistent identifier for a term registered in the InterLex project."),
-        Field("knowledge_space_link", IRI, "vocab:knowledgeSpaceLink", multiple=False, required=False,
-              doc="Persistent link to an encyclopedia entry in the Knowledge Space project."),
-        Field("preferred_ontology_identifier", IRI, "vocab:preferredOntologyIdentifier", multiple=False, required=False,
-              doc="Persistent identifier of a preferred ontological term."),
-        Field("synonyms", str, "vocab:synonym", multiple=True, required=False,
-              doc="Words or expressions used in the same language that have the same or nearly the same meaning in some or all senses."),
+        Field("name", str, "vocab:fullName", multiple=False, required=True,
+              doc="Whole, non-abbreviated name of the consortium."),
+        Field("alias", str, "vocab:shortName", multiple=False, required=False,
+              doc="Shortened or fully abbreviated name of the consortium."),
+        Field("contact_information", "openminds.core.ContactInformation", "vocab:contactInformation", multiple=False, required=False,
+              doc="Any available way used to contact a person or business (e.g., address, phone number, email address, etc.)."),
+        Field("homepage", "openminds.core.URL", "vocab:homepage", multiple=False, required=False,
+              doc="Main website of the consortium."),
 
     ]
     existence_query_fields = ('name',)
```

### Comparing `fairgraph-0.8.2/fairgraph/openminds/controlledterms/meta_data_model_type.py` & `fairgraph-0.9.0/fairgraph/openminds/controlledterms/educational_level.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,40 +1,64 @@
 """
 
+
+    .. list-table:: **Possible values**
+       :widths: 20 80
+       :header-rows: 0
+
+       * - beginner
+         - The learner has no or minimal knowledge or experience of the given topic.
+       * - advanced
+         - The learner has extensive knowledge of the given topic.
+       * - intermediate
+         - The learner has knowledge of the given topic, but is not an expert.
+
 """
 
 # this file was auto-generated
 
 from datetime import date, datetime
 from fairgraph.base_v3 import KGObject, IRI
 from fairgraph.fields import Field
 
 
 
 
-class MetaDataModelType(KGObject):
+class EducationalLevel(KGObject):
     """
 
+
+    .. list-table:: **Possible values**
+       :widths: 20 80
+       :header-rows: 0
+
+       * - beginner
+         - The learner has no or minimal knowledge or experience of the given topic.
+       * - advanced
+         - The learner has extensive knowledge of the given topic.
+       * - intermediate
+         - The learner has knowledge of the given topic, but is not an expert.
+
     """
     default_space = "controlled"
-    type = ["https://openminds.ebrains.eu/controlledTerms/MetaDataModelType"]
+    type = ["https://openminds.ebrains.eu/controlledTerms/EducationalLevel"]
     context = {
         "schema": "http://schema.org/",
         "kg": "https://kg.ebrains.eu/api/instances/",
         "vocab": "https://openminds.ebrains.eu/vocab/",
         "terms": "https://openminds.ebrains.eu/controlledTerms/",
         "core": "https://openminds.ebrains.eu/core/"
     }
     fields = [
         Field("name", str, "vocab:name", multiple=False, required=True,
-              doc="Word or phrase that constitutes the distinctive designation of the meta data model type."),
+              doc="Word or phrase that constitutes the distinctive designation of the educational level."),
         Field("definition", str, "vocab:definition", multiple=False, required=False,
               doc="Short, but precise statement of the meaning of a word, word group, sign or a symbol."),
         Field("description", str, "vocab:description", multiple=False, required=False,
-              doc="Longer statement or account giving the characteristics of the meta data model type."),
+              doc="Longer statement or account giving the characteristics of the educational level."),
         Field("interlex_identifier", IRI, "vocab:interlexIdentifier", multiple=False, required=False,
               doc="Persistent identifier for a term registered in the InterLex project."),
         Field("knowledge_space_link", IRI, "vocab:knowledgeSpaceLink", multiple=False, required=False,
               doc="Persistent link to an encyclopedia entry in the Knowledge Space project."),
         Field("preferred_ontology_identifier", IRI, "vocab:preferredOntologyIdentifier", multiple=False, required=False,
               doc="Persistent identifier of a preferred ontological term."),
         Field("synonyms", str, "vocab:synonym", multiple=True, required=False,
```

### Comparing `fairgraph-0.8.2/fairgraph/openminds/controlledterms/model_abstraction_level.py` & `fairgraph-0.9.0/fairgraph/openminds/controlledterms/annotation_type.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,40 +1,60 @@
 """
-Structured information on abstraction level of the computational model.
+
+
+    .. list-table:: **Possible values**
+       :widths: 20 80
+       :header-rows: 0
+
+       * - deterministic annotation
+         - A 'deterministic annotation' provides an exact assignment of an entity or a list of entities to a defined annotation. The assingment itself can be based on a deterministic or maximum probability assumption.
+       * - probabalistic annotation
+         - A 'probabalistic annotation' provides the probability or probabilites to which an entity or a list of entities belong(s) to a defined annotation.
+
 """
 
 # this file was auto-generated
 
 from datetime import date, datetime
 from fairgraph.base_v3 import KGObject, IRI
 from fairgraph.fields import Field
 
 
 
 
-class ModelAbstractionLevel(KGObject):
+class AnnotationType(KGObject):
     """
-    Structured information on abstraction level of the computational model.
+
+
+    .. list-table:: **Possible values**
+       :widths: 20 80
+       :header-rows: 0
+
+       * - deterministic annotation
+         - A 'deterministic annotation' provides an exact assignment of an entity or a list of entities to a defined annotation. The assingment itself can be based on a deterministic or maximum probability assumption.
+       * - probabalistic annotation
+         - A 'probabalistic annotation' provides the probability or probabilites to which an entity or a list of entities belong(s) to a defined annotation.
+
     """
     default_space = "controlled"
-    type = ["https://openminds.ebrains.eu/controlledTerms/ModelAbstractionLevel"]
+    type = ["https://openminds.ebrains.eu/controlledTerms/AnnotationType"]
     context = {
         "schema": "http://schema.org/",
         "kg": "https://kg.ebrains.eu/api/instances/",
         "vocab": "https://openminds.ebrains.eu/vocab/",
         "terms": "https://openminds.ebrains.eu/controlledTerms/",
         "core": "https://openminds.ebrains.eu/core/"
     }
     fields = [
         Field("name", str, "vocab:name", multiple=False, required=True,
-              doc="Word or phrase that constitutes the distinctive designation of the model abstraction level."),
+              doc="Word or phrase that constitutes the distinctive designation of the annotation type."),
         Field("definition", str, "vocab:definition", multiple=False, required=False,
               doc="Short, but precise statement of the meaning of a word, word group, sign or a symbol."),
         Field("description", str, "vocab:description", multiple=False, required=False,
-              doc="Longer statement or account giving the characteristics of the model abstraction level."),
+              doc="Longer statement or account giving the characteristics of the annotation type."),
         Field("interlex_identifier", IRI, "vocab:interlexIdentifier", multiple=False, required=False,
               doc="Persistent identifier for a term registered in the InterLex project."),
         Field("knowledge_space_link", IRI, "vocab:knowledgeSpaceLink", multiple=False, required=False,
               doc="Persistent link to an encyclopedia entry in the Knowledge Space project."),
         Field("preferred_ontology_identifier", IRI, "vocab:preferredOntologyIdentifier", multiple=False, required=False,
               doc="Persistent identifier of a preferred ontological term."),
         Field("synonyms", str, "vocab:synonym", multiple=True, required=False,
```

### Comparing `fairgraph-0.8.2/fairgraph/openminds/controlledterms/model_scope.py` & `fairgraph-0.9.0/fairgraph/openminds/controlledterms/criteria_quality_type.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,40 +1,60 @@
 """
-Structured information on the scope of the computational model.
+Structured information on the quality type of the defined criteria for a measurement.
+
+    .. list-table:: **Possible values**
+       :widths: 20 80
+       :header-rows: 0
+
+       * - processive
+         - If a criteria is 'processive' it is based on a repeatable and often automated process.
+       * - asserted
+         - If a criteria is 'asserted' it is based on an opinion or claim, usually made by an expert.
+
 """
 
 # this file was auto-generated
 
 from datetime import date, datetime
 from fairgraph.base_v3 import KGObject, IRI
 from fairgraph.fields import Field
 
 
 
 
-class ModelScope(KGObject):
+class CriteriaQualityType(KGObject):
     """
-    Structured information on the scope of the computational model.
+    Structured information on the quality type of the defined criteria for a measurement.
+
+    .. list-table:: **Possible values**
+       :widths: 20 80
+       :header-rows: 0
+
+       * - processive
+         - If a criteria is 'processive' it is based on a repeatable and often automated process.
+       * - asserted
+         - If a criteria is 'asserted' it is based on an opinion or claim, usually made by an expert.
+
     """
     default_space = "controlled"
-    type = ["https://openminds.ebrains.eu/controlledTerms/ModelScope"]
+    type = ["https://openminds.ebrains.eu/controlledTerms/CriteriaQualityType"]
     context = {
         "schema": "http://schema.org/",
         "kg": "https://kg.ebrains.eu/api/instances/",
         "vocab": "https://openminds.ebrains.eu/vocab/",
         "terms": "https://openminds.ebrains.eu/controlledTerms/",
         "core": "https://openminds.ebrains.eu/core/"
     }
     fields = [
         Field("name", str, "vocab:name", multiple=False, required=True,
-              doc="Word or phrase that constitutes the distinctive designation of the model scope."),
+              doc="Word or phrase that constitutes the distinctive designation of the criteria quality type."),
         Field("definition", str, "vocab:definition", multiple=False, required=False,
               doc="Short, but precise statement of the meaning of a word, word group, sign or a symbol."),
         Field("description", str, "vocab:description", multiple=False, required=False,
-              doc="Longer statement or account giving the characteristics of the model scope."),
+              doc="Longer statement or account giving the characteristics of the criteria quality type."),
         Field("interlex_identifier", IRI, "vocab:interlexIdentifier", multiple=False, required=False,
               doc="Persistent identifier for a term registered in the InterLex project."),
         Field("knowledge_space_link", IRI, "vocab:knowledgeSpaceLink", multiple=False, required=False,
               doc="Persistent link to an encyclopedia entry in the Knowledge Space project."),
         Field("preferred_ontology_identifier", IRI, "vocab:preferredOntologyIdentifier", multiple=False, required=False,
               doc="Persistent identifier of a preferred ontological term."),
         Field("synonyms", str, "vocab:synonym", multiple=True, required=False,
```

### Comparing `fairgraph-0.8.2/fairgraph/openminds/controlledterms/molecular_entity.py` & `fairgraph-0.9.0/fairgraph/openminds/ephys/entity/recording.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,38 +7,40 @@
 from datetime import date, datetime
 from fairgraph.base_v3 import KGObject, IRI
 from fairgraph.fields import Field
 
 
 
 
-class MolecularEntity(KGObject):
+class Recording(KGObject):
     """
 
     """
-    default_space = "controlled"
-    type = ["https://openminds.ebrains.eu/controlledTerms/MolecularEntity"]
+    default_space = "in-depth"
+    type = ["https://openminds.ebrains.eu/ephys/Recording"]
     context = {
         "schema": "http://schema.org/",
         "kg": "https://kg.ebrains.eu/api/instances/",
         "vocab": "https://openminds.ebrains.eu/vocab/",
         "terms": "https://openminds.ebrains.eu/controlledTerms/",
         "core": "https://openminds.ebrains.eu/core/"
     }
     fields = [
-        Field("name", str, "vocab:name", multiple=False, required=True,
-              doc="Word or phrase that constitutes the distinctive designation of the molecular entity."),
-        Field("definition", str, "vocab:definition", multiple=False, required=False,
-              doc="Short, but precise statement of the meaning of a word, word group, sign or a symbol."),
-        Field("description", str, "vocab:description", multiple=False, required=False,
-              doc="Longer statement or account giving the characteristics of the molecular entity."),
-        Field("interlex_identifier", IRI, "vocab:interlexIdentifier", multiple=False, required=False,
-              doc="Persistent identifier for a term registered in the InterLex project."),
-        Field("knowledge_space_link", IRI, "vocab:knowledgeSpaceLink", multiple=False, required=False,
-              doc="Persistent link to an encyclopedia entry in the Knowledge Space project."),
-        Field("preferred_ontology_identifier", IRI, "vocab:preferredOntologyIdentifier", multiple=False, required=False,
-              doc="Persistent identifier of a preferred ontological term."),
-        Field("synonyms", str, "vocab:synonym", multiple=True, required=False,
-              doc="Words or expressions used in the same language that have the same or nearly the same meaning in some or all senses."),
+        Field("name", str, "vocab:name", multiple=False, required=False,
+              doc="Word or phrase that constitutes the distinctive designation of the recording."),
+        Field("additional_remarks", str, "vocab:additionalRemarks", multiple=False, required=False,
+              doc="Mention of what deserves additional attention or notice."),
+        Field("channels", "openminds.ephys.Channel", "vocab:channel", multiple=True, required=True,
+              doc="no description available"),
+        Field("data_location", ["openminds.core.File", "openminds.core.FileBundle"], "vocab:dataLocation", multiple=False, required=True,
+              doc="no description available"),
+        Field("internal_identifier", str, "vocab:internalIdentifier", multiple=False, required=False,
+              doc="Term or code that identifies the recording within a particular product."),
+        Field("previous_recording", "openminds.ephys.Recording", "vocab:previousRecording", multiple=False, required=False,
+              doc="no description available"),
+        Field("recorded_with", ["openminds.ephys.ElectrodeArrayUsage", "openminds.ephys.ElectrodeUsage", "openminds.ephys.PipetteUsage", "openminds.specimenprep.SlicingDeviceUsage"], "vocab:recordedWith", multiple=False, required=True,
+              doc="no description available"),
+        Field("sampling_frequency", "openminds.core.QuantitativeValue", "vocab:samplingFrequency", multiple=False, required=True,
+              doc="no description available"),
 
     ]
-    existence_query_fields = ('name',)
+    existence_query_fields = ('channels', 'data_location', 'recorded_with', 'sampling_frequency')
```

### Comparing `fairgraph-0.8.2/fairgraph/openminds/controlledterms/operating_device.py` & `fairgraph-0.9.0/fairgraph/openminds/core/miscellaneous/quantitative_value_array.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,44 +1,40 @@
 """
-Structured information on the operating device.
+A representation of an array of quantitative values, optionally with uncertainties.
 """
 
 # this file was auto-generated
 
 from datetime import date, datetime
 from fairgraph.base_v3 import KGObject, IRI
 from fairgraph.fields import Field
 
 
 
 
-class OperatingDevice(KGObject):
+class QuantitativeValueArray(KGObject):
     """
-    Structured information on the operating device.
+    A representation of an array of quantitative values, optionally with uncertainties.
     """
-    default_space = "controlled"
-    type = ["https://openminds.ebrains.eu/controlledTerms/OperatingDevice"]
+    default_space = "dataset"
+    type = ["https://openminds.ebrains.eu/core/QuantitativeValueArray"]
     context = {
         "schema": "http://schema.org/",
         "kg": "https://kg.ebrains.eu/api/instances/",
         "vocab": "https://openminds.ebrains.eu/vocab/",
         "terms": "https://openminds.ebrains.eu/controlledTerms/",
         "core": "https://openminds.ebrains.eu/core/"
     }
     fields = [
-        Field("name", str, "vocab:name", multiple=False, required=True,
-              doc="Word or phrase that constitutes the distinctive designation of the operating device."),
-        Field("definition", str, "vocab:definition", multiple=False, required=False,
-              doc="Short, but precise statement of the meaning of a word, word group, sign or a symbol."),
-        Field("description", str, "vocab:description", multiple=False, required=False,
-              doc="Longer statement or account giving the characteristics of the operating device."),
-        Field("interlex_identifier", IRI, "vocab:interlexIdentifier", multiple=False, required=False,
-              doc="Persistent identifier for a term registered in the InterLex project."),
-        Field("knowledge_space_link", IRI, "vocab:knowledgeSpaceLink", multiple=False, required=False,
-              doc="Persistent link to an encyclopedia entry in the Knowledge Space project."),
-        Field("preferred_ontology_identifier", IRI, "vocab:preferredOntologyIdentifier", multiple=False, required=False,
-              doc="Persistent identifier of a preferred ontological term."),
-        Field("synonyms", str, "vocab:synonym", multiple=True, required=False,
-              doc="Words or expressions used in the same language that have the same or nearly the same meaning in some or all senses."),
+        Field("negative_uncertainties", float, "vocab:negativeUncertainties", multiple=True, required=False,
+              doc="no description available"),
+        Field("positive_uncertainties", float, "vocab:positiveUncertainties", multiple=True, required=False,
+              doc="no description available"),
+        Field("type_of_uncertainty", "openminds.controlledterms.TypeOfUncertainty", "vocab:typeOfUncertainty", multiple=False, required=False,
+              doc="Distinct technique used to quantify the uncertainty of a measurement."),
+        Field("unit", "openminds.controlledterms.UnitOfMeasurement", "vocab:unit", multiple=False, required=False,
+              doc="Determinate quantity adopted as a standard of measurement."),
+        Field("values", float, "vocab:values", multiple=True, required=True,
+              doc="no description available"),
 
     ]
-    existence_query_fields = ('name',)
+    existence_query_fields = ('values',)
```

### Comparing `fairgraph-0.8.2/fairgraph/openminds/controlledterms/operating_system.py` & `fairgraph-0.9.0/fairgraph/openminds/computation/launch_configuration.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,44 +1,40 @@
 """
-Structured information on the operating system.
+Structured information about the launch of a computational process.
 """
 
 # this file was auto-generated
 
 from datetime import date, datetime
 from fairgraph.base_v3 import KGObject, IRI
 from fairgraph.fields import Field
 
 
 
 
-class OperatingSystem(KGObject):
+class LaunchConfiguration(KGObject):
     """
-    Structured information on the operating system.
+    Structured information about the launch of a computational process.
     """
-    default_space = "controlled"
-    type = ["https://openminds.ebrains.eu/controlledTerms/OperatingSystem"]
+    default_space = "computation"
+    type = ["https://openminds.ebrains.eu/computation/LaunchConfiguration"]
     context = {
         "schema": "http://schema.org/",
         "kg": "https://kg.ebrains.eu/api/instances/",
         "vocab": "https://openminds.ebrains.eu/vocab/",
         "terms": "https://openminds.ebrains.eu/controlledTerms/",
         "core": "https://openminds.ebrains.eu/core/"
     }
     fields = [
-        Field("name", str, "vocab:name", multiple=False, required=True,
-              doc="Word or phrase that constitutes the distinctive designation of the operating system."),
-        Field("definition", str, "vocab:definition", multiple=False, required=False,
-              doc="Short, but precise statement of the meaning of a word, word group, sign or a symbol."),
+        Field("name", str, "vocab:name", multiple=False, required=False,
+              doc="Word or phrase that constitutes the distinctive designation of the launch configuration."),
+        Field("arguments", str, "vocab:arguments", multiple=True, required=False,
+              doc="no description available"),
         Field("description", str, "vocab:description", multiple=False, required=False,
-              doc="Longer statement or account giving the characteristics of the operating system."),
-        Field("interlex_identifier", IRI, "vocab:interlexIdentifier", multiple=False, required=False,
-              doc="Persistent identifier for a term registered in the InterLex project."),
-        Field("knowledge_space_link", IRI, "vocab:knowledgeSpaceLink", multiple=False, required=False,
-              doc="Persistent link to an encyclopedia entry in the Knowledge Space project."),
-        Field("preferred_ontology_identifier", IRI, "vocab:preferredOntologyIdentifier", multiple=False, required=False,
-              doc="Persistent identifier of a preferred ontological term."),
-        Field("synonyms", str, "vocab:synonym", multiple=True, required=False,
-              doc="Words or expressions used in the same language that have the same or nearly the same meaning in some or all senses."),
+              doc="Longer statement or account giving the characteristics of the launch configuration."),
+        Field("environment_variables", "openminds.core.PropertyValueList", "vocab:environmentVariables", multiple=False, required=False,
+              doc="no description available"),
+        Field("executable", str, "vocab:executable", multiple=False, required=True,
+              doc="no description available"),
 
     ]
-    existence_query_fields = ('name',)
+    existence_query_fields = ('executable', 'name')
```

### Comparing `fairgraph-0.8.2/fairgraph/openminds/controlledterms/organ.py` & `fairgraph-0.9.0/fairgraph/openminds/core/products/web_service.py`

 * *Files 23% similar despite different names*

```diff
@@ -7,38 +7,40 @@
 from datetime import date, datetime
 from fairgraph.base_v3 import KGObject, IRI
 from fairgraph.fields import Field
 
 
 
 
-class Organ(KGObject):
+class WebService(KGObject):
     """
 
     """
-    default_space = "controlled"
-    type = ["https://openminds.ebrains.eu/controlledTerms/Organ"]
+    default_space = "webservice"
+    type = ["https://openminds.ebrains.eu/core/WebService"]
     context = {
         "schema": "http://schema.org/",
         "kg": "https://kg.ebrains.eu/api/instances/",
         "vocab": "https://openminds.ebrains.eu/vocab/",
         "terms": "https://openminds.ebrains.eu/controlledTerms/",
         "core": "https://openminds.ebrains.eu/core/"
     }
     fields = [
-        Field("name", str, "vocab:name", multiple=False, required=True,
-              doc="Word or phrase that constitutes the distinctive designation of the organ."),
-        Field("definition", str, "vocab:definition", multiple=False, required=False,
-              doc="Short, but precise statement of the meaning of a word, word group, sign or a symbol."),
-        Field("description", str, "vocab:description", multiple=False, required=False,
-              doc="Longer statement or account giving the characteristics of the organ."),
-        Field("interlex_identifier", IRI, "vocab:interlexIdentifier", multiple=False, required=False,
-              doc="Persistent identifier for a term registered in the InterLex project."),
-        Field("knowledge_space_link", IRI, "vocab:knowledgeSpaceLink", multiple=False, required=False,
-              doc="Persistent link to an encyclopedia entry in the Knowledge Space project."),
-        Field("preferred_ontology_identifier", IRI, "vocab:preferredOntologyIdentifier", multiple=False, required=False,
-              doc="Persistent identifier of a preferred ontological term."),
-        Field("synonyms", str, "vocab:synonym", multiple=True, required=False,
-              doc="Words or expressions used in the same language that have the same or nearly the same meaning in some or all senses."),
+        Field("name", str, "vocab:fullName", multiple=False, required=True,
+              doc="Whole, non-abbreviated name of the web service."),
+        Field("alias", str, "vocab:shortName", multiple=False, required=True,
+              doc="Shortened or fully abbreviated name of the web service."),
+        Field("custodians", ["openminds.core.Consortium", "openminds.core.Organization", "openminds.core.Person"], "vocab:custodian", multiple=True, required=False,
+              doc="The 'custodian' is a legal person who is responsible for the content and quality of the data, metadata, and/or code of a research product."),
+        Field("description", str, "vocab:description", multiple=False, required=True,
+              doc="Longer statement or account giving the characteristics of the web service."),
+        Field("developers", ["openminds.core.Consortium", "openminds.core.Organization", "openminds.core.Person"], "vocab:developer", multiple=True, required=True,
+              doc="Legal person that creates or improves products or services (e.g., software, applications, etc.)."),
+        Field("versions", "openminds.core.WebServiceVersion", "vocab:hasVersion", multiple=True, required=True,
+              doc="Reference to variants of an original."),
+        Field("homepage", "openminds.core.URL", "vocab:homepage", multiple=False, required=False,
+              doc="Main website of the web service."),
+        Field("how_to_cite", str, "vocab:howToCite", multiple=False, required=False,
+              doc="Preferred format for citing a particular object or legal person."),
 
     ]
-    existence_query_fields = ('name',)
+    existence_query_fields = ('name', 'alias', 'description', 'developers', 'versions')
```

### Comparing `fairgraph-0.8.2/fairgraph/openminds/controlledterms/patch_clamp_variation.py` & `fairgraph-0.9.0/fairgraph/openminds/core/research/strain.py`

 * *Files 20% similar despite different names*

```diff
@@ -7,38 +7,52 @@
 from datetime import date, datetime
 from fairgraph.base_v3 import KGObject, IRI
 from fairgraph.fields import Field
 
 
 
 
-class PatchClampVariation(KGObject):
+class Strain(KGObject):
     """
 
     """
-    default_space = "controlled"
-    type = ["https://openminds.ebrains.eu/controlledTerms/PatchClampVariation"]
+    default_space = "dataset"
+    type = ["https://openminds.ebrains.eu/core/Strain"]
     context = {
         "schema": "http://schema.org/",
         "kg": "https://kg.ebrains.eu/api/instances/",
         "vocab": "https://openminds.ebrains.eu/vocab/",
         "terms": "https://openminds.ebrains.eu/controlledTerms/",
         "core": "https://openminds.ebrains.eu/core/"
     }
     fields = [
         Field("name", str, "vocab:name", multiple=False, required=True,
-              doc="Word or phrase that constitutes the distinctive designation of the patch clamp variation."),
-        Field("definition", str, "vocab:definition", multiple=False, required=False,
-              doc="Short, but precise statement of the meaning of a word, word group, sign or a symbol."),
+              doc="Word or phrase that constitutes the distinctive designation of the strain."),
+        Field("rrid", "openminds.core.RRID", "vocab:RRID", multiple=False, required=False,
+              doc="no description available"),
+        Field("background_strains", "openminds.core.Strain", "vocab:backgroundStrain", multiple=True, required=False,
+              doc="no description available"),
+        Field("breeding_type", "openminds.controlledterms.BreedingType", "vocab:breedingType", multiple=False, required=False,
+              doc="no description available"),
         Field("description", str, "vocab:description", multiple=False, required=False,
-              doc="Longer statement or account giving the characteristics of the patch clamp variation."),
-        Field("interlex_identifier", IRI, "vocab:interlexIdentifier", multiple=False, required=False,
-              doc="Persistent identifier for a term registered in the InterLex project."),
-        Field("knowledge_space_link", IRI, "vocab:knowledgeSpaceLink", multiple=False, required=False,
-              doc="Persistent link to an encyclopedia entry in the Knowledge Space project."),
-        Field("preferred_ontology_identifier", IRI, "vocab:preferredOntologyIdentifier", multiple=False, required=False,
-              doc="Persistent identifier of a preferred ontological term."),
+              doc="Longer statement or account giving the characteristics of the strain."),
+        Field("disease_models", ["openminds.controlledterms.Disease", "openminds.controlledterms.DiseaseModel"], "vocab:diseaseModel", multiple=True, required=False,
+              doc="no description available"),
+        Field("genetic_strain_type", "openminds.controlledterms.GeneticStrainType", "vocab:geneticStrainType", multiple=False, required=True,
+              doc="no description available"),
+        Field("identifiers", str, "vocab:identifier", multiple=True, required=False,
+              doc="Term or code used to identify the strain."),
+        Field("laboratory_code", str, "vocab:laboratoryCode", multiple=False, required=False,
+              doc="no description available"),
+        Field("ontology_identifiers", str, "vocab:ontologyIdentifier", multiple=True, required=False,
+              doc="Term or code used to identify the strain registered within a particular ontology."),
+        Field("phenotype", str, "vocab:phenotype", multiple=False, required=False,
+              doc="Physical expression of one or more genes of an organism."),
+        Field("species", "openminds.controlledterms.Species", "vocab:species", multiple=False, required=True,
+              doc="Category of biological classification comprising related organisms or populations potentially capable of interbreeding, and being designated by a binomial that consists of the name of a genus followed by a Latin or latinized uncapitalized noun or adjective."),
+        Field("stock_number", "openminds.core.StockNumber", "vocab:stockNumber", multiple=False, required=False,
+              doc="no description available"),
         Field("synonyms", str, "vocab:synonym", multiple=True, required=False,
               doc="Words or expressions used in the same language that have the same or nearly the same meaning in some or all senses."),
 
     ]
-    existence_query_fields = ('name',)
+    existence_query_fields = ('name', 'genetic_strain_type', 'species')
```

### Comparing `fairgraph-0.8.2/fairgraph/openminds/controlledterms/preparation_type.py` & `fairgraph-0.9.0/fairgraph/openminds/controlledterms/gustatory_stimulus_type.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,40 +1,68 @@
 """
 
+
+    .. list-table:: **Possible values**
+       :widths: 20 80
+       :header-rows: 0
+
+       * - sweet substance
+         - Any chemical compound that tastes sweet.
+       * - salty substance
+         - Any chemical compound that tastes salty.
+       * - bitter substance
+         - Any chemical compound that tastes bitter.
+       * - sour substance
+         - Any chemical compound that tastes sour.
+
 """
 
 # this file was auto-generated
 
 from datetime import date, datetime
 from fairgraph.base_v3 import KGObject, IRI
 from fairgraph.fields import Field
 
 
 
 
-class PreparationType(KGObject):
+class GustatoryStimulusType(KGObject):
     """
 
+
+    .. list-table:: **Possible values**
+       :widths: 20 80
+       :header-rows: 0
+
+       * - sweet substance
+         - Any chemical compound that tastes sweet.
+       * - salty substance
+         - Any chemical compound that tastes salty.
+       * - bitter substance
+         - Any chemical compound that tastes bitter.
+       * - sour substance
+         - Any chemical compound that tastes sour.
+
     """
     default_space = "controlled"
-    type = ["https://openminds.ebrains.eu/controlledTerms/PreparationType"]
+    type = ["https://openminds.ebrains.eu/controlledTerms/GustatoryStimulusType"]
     context = {
         "schema": "http://schema.org/",
         "kg": "https://kg.ebrains.eu/api/instances/",
         "vocab": "https://openminds.ebrains.eu/vocab/",
         "terms": "https://openminds.ebrains.eu/controlledTerms/",
         "core": "https://openminds.ebrains.eu/core/"
     }
     fields = [
         Field("name", str, "vocab:name", multiple=False, required=True,
-              doc="Word or phrase that constitutes the distinctive designation of the preparation type."),
+              doc="Word or phrase that constitutes the distinctive designation of the gustatory stimulus type."),
         Field("definition", str, "vocab:definition", multiple=False, required=False,
               doc="Short, but precise statement of the meaning of a word, word group, sign or a symbol."),
         Field("description", str, "vocab:description", multiple=False, required=False,
-              doc="Longer statement or account giving the characteristics of the preparation type."),
+              doc="Longer statement or account giving the characteristics of the gustatory stimulus type."),
         Field("interlex_identifier", IRI, "vocab:interlexIdentifier", multiple=False, required=False,
               doc="Persistent identifier for a term registered in the InterLex project."),
         Field("knowledge_space_link", IRI, "vocab:knowledgeSpaceLink", multiple=False, required=False,
               doc="Persistent link to an encyclopedia entry in the Knowledge Space project."),
         Field("preferred_ontology_identifier", IRI, "vocab:preferredOntologyIdentifier", multiple=False, required=False,
               doc="Persistent identifier of a preferred ontological term."),
         Field("synonyms", str, "vocab:synonym", multiple=True, required=False,
```

### Comparing `fairgraph-0.8.2/fairgraph/openminds/controlledterms/product_accessibility.py` & `fairgraph-0.9.0/fairgraph/openminds/controlledterms/genetic_strain_type.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,40 +1,80 @@
 """
 
+
+    .. list-table:: **Possible values**
+       :widths: 20 80
+       :header-rows: 0
+
+       * - wildtype
+         -
+       * - transgenic
+         -
+       * - knockout
+         -
+       * - knockin
+         -
+       * - conditional knockout ready
+         -
+       * - conditional ready
+         -
+       * - conditional knockin ready
+         -
+
 """
 
 # this file was auto-generated
 
 from datetime import date, datetime
 from fairgraph.base_v3 import KGObject, IRI
 from fairgraph.fields import Field
 
 
 
 
-class ProductAccessibility(KGObject):
+class GeneticStrainType(KGObject):
     """
 
+
+    .. list-table:: **Possible values**
+       :widths: 20 80
+       :header-rows: 0
+
+       * - wildtype
+         -
+       * - transgenic
+         -
+       * - knockout
+         -
+       * - knockin
+         -
+       * - conditional knockout ready
+         -
+       * - conditional ready
+         -
+       * - conditional knockin ready
+         -
+
     """
     default_space = "controlled"
-    type = ["https://openminds.ebrains.eu/controlledTerms/ProductAccessibility"]
+    type = ["https://openminds.ebrains.eu/controlledTerms/GeneticStrainType"]
     context = {
         "schema": "http://schema.org/",
         "kg": "https://kg.ebrains.eu/api/instances/",
         "vocab": "https://openminds.ebrains.eu/vocab/",
         "terms": "https://openminds.ebrains.eu/controlledTerms/",
         "core": "https://openminds.ebrains.eu/core/"
     }
     fields = [
         Field("name", str, "vocab:name", multiple=False, required=True,
-              doc="Word or phrase that constitutes the distinctive designation of the product accessibility."),
+              doc="Word or phrase that constitutes the distinctive designation of the genetic strain type."),
         Field("definition", str, "vocab:definition", multiple=False, required=False,
               doc="Short, but precise statement of the meaning of a word, word group, sign or a symbol."),
         Field("description", str, "vocab:description", multiple=False, required=False,
-              doc="Longer statement or account giving the characteristics of the product accessibility."),
+              doc="Longer statement or account giving the characteristics of the genetic strain type."),
         Field("interlex_identifier", IRI, "vocab:interlexIdentifier", multiple=False, required=False,
               doc="Persistent identifier for a term registered in the InterLex project."),
         Field("knowledge_space_link", IRI, "vocab:knowledgeSpaceLink", multiple=False, required=False,
               doc="Persistent link to an encyclopedia entry in the Knowledge Space project."),
         Field("preferred_ontology_identifier", IRI, "vocab:preferredOntologyIdentifier", multiple=False, required=False,
               doc="Persistent identifier of a preferred ontological term."),
         Field("synonyms", str, "vocab:synonym", multiple=True, required=False,
```

### Comparing `fairgraph-0.8.2/fairgraph/openminds/controlledterms/programming_language.py` & `fairgraph-0.9.0/fairgraph/openminds/core/miscellaneous/funding.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,44 +1,38 @@
 """
-Structured information on the programming language.
+Structured information on used funding.
 """
 
 # this file was auto-generated
 
 from datetime import date, datetime
 from fairgraph.base_v3 import KGObject, IRI
 from fairgraph.fields import Field
 
 
 
 
-class ProgrammingLanguage(KGObject):
+class Funding(KGObject):
     """
-    Structured information on the programming language.
+    Structured information on used funding.
     """
-    default_space = "controlled"
-    type = ["https://openminds.ebrains.eu/controlledTerms/ProgrammingLanguage"]
+    default_space = "common"
+    type = ["https://openminds.ebrains.eu/core/Funding"]
     context = {
         "schema": "http://schema.org/",
         "kg": "https://kg.ebrains.eu/api/instances/",
         "vocab": "https://openminds.ebrains.eu/vocab/",
         "terms": "https://openminds.ebrains.eu/controlledTerms/",
         "core": "https://openminds.ebrains.eu/core/"
     }
     fields = [
-        Field("name", str, "vocab:name", multiple=False, required=True,
-              doc="Word or phrase that constitutes the distinctive designation of the programming language."),
-        Field("definition", str, "vocab:definition", multiple=False, required=False,
-              doc="Short, but precise statement of the meaning of a word, word group, sign or a symbol."),
-        Field("description", str, "vocab:description", multiple=False, required=False,
-              doc="Longer statement or account giving the characteristics of the programming language."),
-        Field("interlex_identifier", IRI, "vocab:interlexIdentifier", multiple=False, required=False,
-              doc="Persistent identifier for a term registered in the InterLex project."),
-        Field("knowledge_space_link", IRI, "vocab:knowledgeSpaceLink", multiple=False, required=False,
-              doc="Persistent link to an encyclopedia entry in the Knowledge Space project."),
-        Field("preferred_ontology_identifier", IRI, "vocab:preferredOntologyIdentifier", multiple=False, required=False,
-              doc="Persistent identifier of a preferred ontological term."),
-        Field("synonyms", str, "vocab:synonym", multiple=True, required=False,
-              doc="Words or expressions used in the same language that have the same or nearly the same meaning in some or all senses."),
+        Field("acknowledgement", str, "vocab:acknowledgement", multiple=False, required=False,
+              doc="Offical declaration or avowal of appreciation of an act or achievement."),
+        Field("award_number", str, "vocab:awardNumber", multiple=False, required=False,
+              doc="Machine-readable identifier for a benefit that is conferred or bestowed on the basis of merit or need."),
+        Field("award_title", str, "vocab:awardTitle", multiple=False, required=False,
+              doc="Human-readable identifier for a benefit that is conferred or bestowed on the basis of merit or need."),
+        Field("funder", ["openminds.core.Consortium", "openminds.core.Organization", "openminds.core.Person"], "vocab:funder", multiple=False, required=True,
+              doc="Legal person that provides money for a particular purpose."),
 
     ]
-    existence_query_fields = ('name',)
+    existence_query_fields = ('funder',)
```

### Comparing `fairgraph-0.8.2/fairgraph/openminds/controlledterms/qualitative_overlap.py` & `fairgraph-0.9.0/fairgraph/openminds/ephys/device/electrode_array_usage.py`

 * *Files 20% similar despite different names*

```diff
@@ -7,38 +7,40 @@
 from datetime import date, datetime
 from fairgraph.base_v3 import KGObject, IRI
 from fairgraph.fields import Field
 
 
 
 
-class QualitativeOverlap(KGObject):
+class ElectrodeArrayUsage(KGObject):
     """
 
     """
-    default_space = "controlled"
-    type = ["https://openminds.ebrains.eu/controlledTerms/QualitativeOverlap"]
+    default_space = "in-depth"
+    type = ["https://openminds.ebrains.eu/ephys/ElectrodeArrayUsage"]
     context = {
         "schema": "http://schema.org/",
         "kg": "https://kg.ebrains.eu/api/instances/",
         "vocab": "https://openminds.ebrains.eu/vocab/",
         "terms": "https://openminds.ebrains.eu/controlledTerms/",
         "core": "https://openminds.ebrains.eu/core/"
     }
     fields = [
-        Field("name", str, "vocab:name", multiple=False, required=True,
-              doc="Word or phrase that constitutes the distinctive designation of the qualitative overlap."),
-        Field("definition", str, "vocab:definition", multiple=False, required=False,
-              doc="Short, but precise statement of the meaning of a word, word group, sign or a symbol."),
-        Field("description", str, "vocab:description", multiple=False, required=False,
-              doc="Longer statement or account giving the characteristics of the qualitative overlap."),
-        Field("interlex_identifier", IRI, "vocab:interlexIdentifier", multiple=False, required=False,
-              doc="Persistent identifier for a term registered in the InterLex project."),
-        Field("knowledge_space_link", IRI, "vocab:knowledgeSpaceLink", multiple=False, required=False,
-              doc="Persistent link to an encyclopedia entry in the Knowledge Space project."),
-        Field("preferred_ontology_identifier", IRI, "vocab:preferredOntologyIdentifier", multiple=False, required=False,
-              doc="Persistent identifier of a preferred ontological term."),
-        Field("synonyms", str, "vocab:synonym", multiple=True, required=False,
-              doc="Words or expressions used in the same language that have the same or nearly the same meaning in some or all senses."),
+        Field("lookup_label", str, "vocab:lookupLabel", multiple=False, required=False,
+              doc="no description available"),
+        Field("additional_informations", ["openminds.core.File", "openminds.core.FileBundle"], "vocab:additionalInformation", multiple=True, required=False,
+              doc="no description available"),
+        Field("anatomical_locations", ["openminds.controlledterms.UBERONParcellation", "openminds.sands.CustomAnatomicalEntity", "openminds.sands.ParcellationEntity", "openminds.sands.ParcellationEntityVersion"], "vocab:anatomicalLocation", multiple=True, required=False,
+              doc="no description available"),
+        Field("contact_resistances", ["openminds.core.QuantitativeValue", "openminds.core.QuantitativeValueRange"], "vocab:contactResistance", multiple=True, required=False,
+              doc="no description available"),
+        Field("coordinate_points", "openminds.sands.CoordinatePoint", "vocab:coordinatePoint", multiple=True, required=False,
+              doc="Pair or triplet of numbers defining the position in a particular two- or three dimensional plane or space."),
+        Field("electrode_array", "openminds.ephys.ElectrodeArray", "vocab:electrodeArray", multiple=False, required=True,
+              doc="no description available"),
+        Field("used_electrodes", str, "vocab:usedElectrode", multiple=True, required=False,
+              doc="no description available"),
+        Field("used_specimen", ["openminds.core.SubjectState", "openminds.core.TissueSampleState"], "vocab:usedSpecimen", multiple=False, required=False,
+              doc="no description available"),
 
     ]
-    existence_query_fields = ('name',)
+    existence_query_fields = ('lookup_label',)
```

### Comparing `fairgraph-0.8.2/fairgraph/openminds/controlledterms/semantic_data_type.py` & `fairgraph-0.9.0/fairgraph/openminds/controlledterms/cranial_window_construction_type.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,40 +1,64 @@
 """
 
+
+    .. list-table:: **Possible values**
+       :widths: 20 80
+       :header-rows: 0
+
+       * - cleared skull cranial window
+         - A cranial window that is constructed by clearing a small region of the skull.
+       * - transcranial window
+         - A cranial window that is constructed by removal of a small region of the skull.
+       * - thinned skull cranial window
+         - A cranial window that is constructed by thinning a small region of the skull.
+
 """
 
 # this file was auto-generated
 
 from datetime import date, datetime
 from fairgraph.base_v3 import KGObject, IRI
 from fairgraph.fields import Field
 
 
 
 
-class SemanticDataType(KGObject):
+class CranialWindowConstructionType(KGObject):
     """
 
+
+    .. list-table:: **Possible values**
+       :widths: 20 80
+       :header-rows: 0
+
+       * - cleared skull cranial window
+         - A cranial window that is constructed by clearing a small region of the skull.
+       * - transcranial window
+         - A cranial window that is constructed by removal of a small region of the skull.
+       * - thinned skull cranial window
+         - A cranial window that is constructed by thinning a small region of the skull.
+
     """
     default_space = "controlled"
-    type = ["https://openminds.ebrains.eu/controlledTerms/SemanticDataType"]
+    type = ["https://openminds.ebrains.eu/controlledTerms/CranialWindowConstructionType"]
     context = {
         "schema": "http://schema.org/",
         "kg": "https://kg.ebrains.eu/api/instances/",
         "vocab": "https://openminds.ebrains.eu/vocab/",
         "terms": "https://openminds.ebrains.eu/controlledTerms/",
         "core": "https://openminds.ebrains.eu/core/"
     }
     fields = [
         Field("name", str, "vocab:name", multiple=False, required=True,
-              doc="Word or phrase that constitutes the distinctive designation of the semantic data type."),
+              doc="Word or phrase that constitutes the distinctive designation of the cranial window construction type."),
         Field("definition", str, "vocab:definition", multiple=False, required=False,
               doc="Short, but precise statement of the meaning of a word, word group, sign or a symbol."),
         Field("description", str, "vocab:description", multiple=False, required=False,
-              doc="Longer statement or account giving the characteristics of the semantic data type."),
+              doc="Longer statement or account giving the characteristics of the cranial window construction type."),
         Field("interlex_identifier", IRI, "vocab:interlexIdentifier", multiple=False, required=False,
               doc="Persistent identifier for a term registered in the InterLex project."),
         Field("knowledge_space_link", IRI, "vocab:knowledgeSpaceLink", multiple=False, required=False,
               doc="Persistent link to an encyclopedia entry in the Knowledge Space project."),
         Field("preferred_ontology_identifier", IRI, "vocab:preferredOntologyIdentifier", multiple=False, required=False,
               doc="Persistent identifier of a preferred ontological term."),
         Field("synonyms", str, "vocab:synonym", multiple=True, required=False,
```

### Comparing `fairgraph-0.8.2/fairgraph/openminds/controlledterms/setup_type.py` & `fairgraph-0.9.0/fairgraph/openminds/specimenprep/device/slicing_device.py`

 * *Files 17% similar despite different names*

```diff
@@ -7,38 +7,40 @@
 from datetime import date, datetime
 from fairgraph.base_v3 import KGObject, IRI
 from fairgraph.fields import Field
 
 
 
 
-class SetupType(KGObject):
+class SlicingDevice(KGObject):
     """
 
     """
-    default_space = "controlled"
-    type = ["https://openminds.ebrains.eu/controlledTerms/SetupType"]
+    default_space = "in-depth"
+    type = ["https://openminds.ebrains.eu/specimenPrep/SlicingDevice"]
     context = {
         "schema": "http://schema.org/",
         "kg": "https://kg.ebrains.eu/api/instances/",
         "vocab": "https://openminds.ebrains.eu/vocab/",
         "terms": "https://openminds.ebrains.eu/controlledTerms/",
         "core": "https://openminds.ebrains.eu/core/"
     }
     fields = [
         Field("name", str, "vocab:name", multiple=False, required=True,
-              doc="Word or phrase that constitutes the distinctive designation of the setup type."),
-        Field("definition", str, "vocab:definition", multiple=False, required=False,
-              doc="Short, but precise statement of the meaning of a word, word group, sign or a symbol."),
+              doc="Word or phrase that constitutes the distinctive designation of the slicing device."),
+        Field("lookup_label", str, "vocab:lookupLabel", multiple=False, required=False,
+              doc="no description available"),
         Field("description", str, "vocab:description", multiple=False, required=False,
-              doc="Longer statement or account giving the characteristics of the setup type."),
-        Field("interlex_identifier", IRI, "vocab:interlexIdentifier", multiple=False, required=False,
-              doc="Persistent identifier for a term registered in the InterLex project."),
-        Field("knowledge_space_link", IRI, "vocab:knowledgeSpaceLink", multiple=False, required=False,
-              doc="Persistent link to an encyclopedia entry in the Knowledge Space project."),
-        Field("preferred_ontology_identifier", IRI, "vocab:preferredOntologyIdentifier", multiple=False, required=False,
-              doc="Persistent identifier of a preferred ontological term."),
-        Field("synonyms", str, "vocab:synonym", multiple=True, required=False,
-              doc="Words or expressions used in the same language that have the same or nearly the same meaning in some or all senses."),
+              doc="Longer statement or account giving the characteristics of the slicing device."),
+        Field("device_type", "openminds.controlledterms.DeviceType", "vocab:deviceType", multiple=False, required=False,
+              doc="no description available"),
+        Field("digital_identifier", ["openminds.core.DOI", "openminds.core.RRID"], "vocab:digitalIdentifier", multiple=False, required=False,
+              doc="Digital handle to identify objects or legal persons."),
+        Field("manufacturers", ["openminds.core.Consortium", "openminds.core.Organization", "openminds.core.Person"], "vocab:manufacturer", multiple=True, required=True,
+              doc="no description available"),
+        Field("owners", ["openminds.core.Consortium", "openminds.core.Organization", "openminds.core.Person"], "vocab:owner", multiple=True, required=False,
+              doc="no description available"),
+        Field("serial_number", str, "vocab:serialNumber", multiple=False, required=False,
+              doc="no description available"),
 
     ]
-    existence_query_fields = ('name',)
+    existence_query_fields = ('lookup_label',)
```

### Comparing `fairgraph-0.8.2/fairgraph/openminds/controlledterms/software_application_category.py` & `fairgraph-0.9.0/fairgraph/openminds/controlledterms/optical_stimulus_type.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,40 +1,56 @@
 """
-Structured information on the category of the software application.
+
+
+    .. list-table:: **Possible values**
+       :widths: 20 80
+       :header-rows: 0
+
+       * - infrared neural stimulus
+         - An 'infrared neural stimulus' is a pulsed IR light (between the wavelength of 1400–2100 nm) used to generate a highly controlled temperature transients in neurons (dT/dz or dT/dt), leading them to fire action potentials. [adapted from [Horváth et al., (2020)](https://doi.org/10.1038/s41378-020-0153-3)]
+
 """
 
 # this file was auto-generated
 
 from datetime import date, datetime
 from fairgraph.base_v3 import KGObject, IRI
 from fairgraph.fields import Field
 
 
 
 
-class SoftwareApplicationCategory(KGObject):
+class OpticalStimulusType(KGObject):
     """
-    Structured information on the category of the software application.
+
+
+    .. list-table:: **Possible values**
+       :widths: 20 80
+       :header-rows: 0
+
+       * - infrared neural stimulus
+         - An 'infrared neural stimulus' is a pulsed IR light (between the wavelength of 1400–2100 nm) used to generate a highly controlled temperature transients in neurons (dT/dz or dT/dt), leading them to fire action potentials. [adapted from [Horváth et al., (2020)](https://doi.org/10.1038/s41378-020-0153-3)]
+
     """
     default_space = "controlled"
-    type = ["https://openminds.ebrains.eu/controlledTerms/SoftwareApplicationCategory"]
+    type = ["https://openminds.ebrains.eu/controlledTerms/OpticalStimulusType"]
     context = {
         "schema": "http://schema.org/",
         "kg": "https://kg.ebrains.eu/api/instances/",
         "vocab": "https://openminds.ebrains.eu/vocab/",
         "terms": "https://openminds.ebrains.eu/controlledTerms/",
         "core": "https://openminds.ebrains.eu/core/"
     }
     fields = [
         Field("name", str, "vocab:name", multiple=False, required=True,
-              doc="Word or phrase that constitutes the distinctive designation of the software application category."),
+              doc="Word or phrase that constitutes the distinctive designation of the optical stimulus type."),
         Field("definition", str, "vocab:definition", multiple=False, required=False,
               doc="Short, but precise statement of the meaning of a word, word group, sign or a symbol."),
         Field("description", str, "vocab:description", multiple=False, required=False,
-              doc="Longer statement or account giving the characteristics of the software application category."),
+              doc="Longer statement or account giving the characteristics of the optical stimulus type."),
         Field("interlex_identifier", IRI, "vocab:interlexIdentifier", multiple=False, required=False,
               doc="Persistent identifier for a term registered in the InterLex project."),
         Field("knowledge_space_link", IRI, "vocab:knowledgeSpaceLink", multiple=False, required=False,
               doc="Persistent link to an encyclopedia entry in the Knowledge Space project."),
         Field("preferred_ontology_identifier", IRI, "vocab:preferredOntologyIdentifier", multiple=False, required=False,
               doc="Persistent identifier of a preferred ontological term."),
         Field("synonyms", str, "vocab:synonym", multiple=True, required=False,
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `fairgraph-0.8.2/fairgraph/openminds/controlledterms/software_feature.py` & `fairgraph-0.9.0/fairgraph/openminds/core/products/software.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,44 +1,48 @@
 """
-
+Structured information on a software tool (concept level).
 """
 
 # this file was auto-generated
 
 from datetime import date, datetime
 from fairgraph.base_v3 import KGObject, IRI
 from fairgraph.fields import Field
 
 
 
 
-class SoftwareFeature(KGObject):
+class Software(KGObject):
     """
-
+    Structured information on a software tool (concept level).
     """
-    default_space = "controlled"
-    type = ["https://openminds.ebrains.eu/controlledTerms/SoftwareFeature"]
+    default_space = "software"
+    type = ["https://openminds.ebrains.eu/core/Software"]
     context = {
         "schema": "http://schema.org/",
         "kg": "https://kg.ebrains.eu/api/instances/",
         "vocab": "https://openminds.ebrains.eu/vocab/",
         "terms": "https://openminds.ebrains.eu/controlledTerms/",
         "core": "https://openminds.ebrains.eu/core/"
     }
     fields = [
-        Field("name", str, "vocab:name", multiple=False, required=True,
-              doc="Word or phrase that constitutes the distinctive designation of the software feature."),
-        Field("definition", str, "vocab:definition", multiple=False, required=False,
-              doc="Short, but precise statement of the meaning of a word, word group, sign or a symbol."),
-        Field("description", str, "vocab:description", multiple=False, required=False,
-              doc="Longer statement or account giving the characteristics of the software feature."),
-        Field("interlex_identifier", IRI, "vocab:interlexIdentifier", multiple=False, required=False,
-              doc="Persistent identifier for a term registered in the InterLex project."),
-        Field("knowledge_space_link", IRI, "vocab:knowledgeSpaceLink", multiple=False, required=False,
-              doc="Persistent link to an encyclopedia entry in the Knowledge Space project."),
-        Field("preferred_ontology_identifier", IRI, "vocab:preferredOntologyIdentifier", multiple=False, required=False,
-              doc="Persistent identifier of a preferred ontological term."),
-        Field("synonyms", str, "vocab:synonym", multiple=True, required=False,
-              doc="Words or expressions used in the same language that have the same or nearly the same meaning in some or all senses."),
+        Field("name", str, "vocab:fullName", multiple=False, required=True,
+              doc="Whole, non-abbreviated name of the software."),
+        Field("alias", str, "vocab:shortName", multiple=False, required=True,
+              doc="Shortened or fully abbreviated name of the software."),
+        Field("custodians", ["openminds.core.Consortium", "openminds.core.Organization", "openminds.core.Person"], "vocab:custodian", multiple=True, required=False,
+              doc="The 'custodian' is a legal person who is responsible for the content and quality of the data, metadata, and/or code of a research product."),
+        Field("description", str, "vocab:description", multiple=False, required=True,
+              doc="Longer statement or account giving the characteristics of the software."),
+        Field("developers", ["openminds.core.Consortium", "openminds.core.Organization", "openminds.core.Person"], "vocab:developer", multiple=True, required=True,
+              doc="Legal person that creates or improves products or services (e.g., software, applications, etc.)."),
+        Field("digital_identifier", ["openminds.core.DOI", "openminds.core.SWHID"], "vocab:digitalIdentifier", multiple=False, required=False,
+              doc="Digital handle to identify objects or legal persons."),
+        Field("versions", "openminds.core.SoftwareVersion", "vocab:hasVersion", multiple=True, required=True,
+              doc="Reference to variants of an original."),
+        Field("homepage", "openminds.core.URL", "vocab:homepage", multiple=False, required=False,
+              doc="Main website of the software."),
+        Field("how_to_cite", str, "vocab:howToCite", multiple=False, required=False,
+              doc="Preferred format for citing a particular object or legal person."),
 
     ]
-    existence_query_fields = ('name',)
+    existence_query_fields = ('alias',)
```

### Comparing `fairgraph-0.8.2/fairgraph/openminds/controlledterms/species.py` & `fairgraph-0.9.0/fairgraph/openminds/core/research/tissue_sample_collection.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,44 +1,52 @@
 """
-Structured information on the species.
+
 """
 
 # this file was auto-generated
 
 from datetime import date, datetime
 from fairgraph.base_v3 import KGObject, IRI
 from fairgraph.fields import Field
 
 
 
 
-class Species(KGObject):
+class TissueSampleCollection(KGObject):
     """
-    Structured information on the species.
+
     """
-    default_space = "controlled"
-    type = ["https://openminds.ebrains.eu/controlledTerms/Species"]
+    default_space = "dataset"
+    type = ["https://openminds.ebrains.eu/core/TissueSampleCollection"]
     context = {
         "schema": "http://schema.org/",
         "kg": "https://kg.ebrains.eu/api/instances/",
         "vocab": "https://openminds.ebrains.eu/vocab/",
         "terms": "https://openminds.ebrains.eu/controlledTerms/",
         "core": "https://openminds.ebrains.eu/core/"
     }
     fields = [
-        Field("name", str, "vocab:name", multiple=False, required=True,
-              doc="Word or phrase that constitutes the distinctive designation of the species."),
-        Field("definition", str, "vocab:definition", multiple=False, required=False,
-              doc="Short, but precise statement of the meaning of a word, word group, sign or a symbol."),
-        Field("description", str, "vocab:description", multiple=False, required=False,
-              doc="Longer statement or account giving the characteristics of the species."),
-        Field("interlex_identifier", IRI, "vocab:interlexIdentifier", multiple=False, required=False,
-              doc="Persistent identifier for a term registered in the InterLex project."),
-        Field("knowledge_space_link", IRI, "vocab:knowledgeSpaceLink", multiple=False, required=False,
-              doc="Persistent link to an encyclopedia entry in the Knowledge Space project."),
-        Field("preferred_ontology_identifier", IRI, "vocab:preferredOntologyIdentifier", multiple=False, required=False,
-              doc="Persistent identifier of a preferred ontological term."),
-        Field("synonyms", str, "vocab:synonym", multiple=True, required=False,
-              doc="Words or expressions used in the same language that have the same or nearly the same meaning in some or all senses."),
+        Field("lookup_label", str, "vocab:lookupLabel", multiple=False, required=False,
+              doc="no description available"),
+        Field("additional_remarks", str, "vocab:additionalRemarks", multiple=False, required=False,
+              doc="Mention of what deserves additional attention or notice."),
+        Field("anatomical_locations", ["openminds.controlledterms.UBERONParcellation", "openminds.sands.CustomAnatomicalEntity", "openminds.sands.ParcellationEntity", "openminds.sands.ParcellationEntityVersion"], "vocab:anatomicalLocation", multiple=True, required=False,
+              doc="no description available"),
+        Field("biological_sex", "openminds.controlledterms.BiologicalSex", "vocab:biologicalSex", multiple=True, required=False,
+              doc="Differentiation of individuals of most species (animals and plants) based on the type of gametes they produce."),
+        Field("internal_identifier", str, "vocab:internalIdentifier", multiple=False, required=False,
+              doc="Term or code that identifies the tissue sample collection within a particular product."),
+        Field("laterality", "openminds.controlledterms.Laterality", "vocab:laterality", multiple=True, required=False,
+              doc="Differentiation between a pair of lateral homologous parts of the body."),
+        Field("origins", ["openminds.controlledterms.CellType", "openminds.controlledterms.Organ"], "vocab:origin", multiple=True, required=True,
+              doc="Source at which something begins or rises, or from which something derives."),
+        Field("quantity", int, "vocab:quantity", multiple=False, required=False,
+              doc="Total amount or number of things or beings."),
+        Field("species", ["openminds.controlledterms.Species", "openminds.core.Strain"], "vocab:species", multiple=True, required=True,
+              doc="Category of biological classification comprising related organisms or populations potentially capable of interbreeding, and being designated by a binomial that consists of the name of a genus followed by a Latin or latinized uncapitalized noun or adjective."),
+        Field("studied_states", "openminds.core.TissueSampleCollectionState", "vocab:studiedState", multiple=True, required=True,
+              doc="Reference to a point in time at which the tissue sample collection was studied in a particular mode or condition."),
+        Field("types", "openminds.controlledterms.TissueSampleType", "vocab:type", multiple=True, required=True,
+              doc="Distinct class to which a group of entities or concepts with similar characteristics or attributes belong to."),
 
     ]
-    existence_query_fields = ('name',)
+    existence_query_fields = ('lookup_label',)
```

### Comparing `fairgraph-0.8.2/fairgraph/openminds/controlledterms/stimulation_approach.py` & `fairgraph-0.9.0/fairgraph/openminds/core/data/license.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,44 +1,38 @@
 """
-
+Structured information on a used license.
 """
 
 # this file was auto-generated
 
 from datetime import date, datetime
 from fairgraph.base_v3 import KGObject, IRI
 from fairgraph.fields import Field
 
 
 
 
-class StimulationApproach(KGObject):
+class License(KGObject):
     """
-
+    Structured information on a used license.
     """
     default_space = "controlled"
-    type = ["https://openminds.ebrains.eu/controlledTerms/StimulationApproach"]
+    type = ["https://openminds.ebrains.eu/core/License"]
     context = {
         "schema": "http://schema.org/",
         "kg": "https://kg.ebrains.eu/api/instances/",
         "vocab": "https://openminds.ebrains.eu/vocab/",
         "terms": "https://openminds.ebrains.eu/controlledTerms/",
         "core": "https://openminds.ebrains.eu/core/"
     }
     fields = [
-        Field("name", str, "vocab:name", multiple=False, required=True,
-              doc="Word or phrase that constitutes the distinctive designation of the stimulation approach."),
-        Field("definition", str, "vocab:definition", multiple=False, required=False,
-              doc="Short, but precise statement of the meaning of a word, word group, sign or a symbol."),
-        Field("description", str, "vocab:description", multiple=False, required=False,
-              doc="Longer statement or account giving the characteristics of the stimulation approach."),
-        Field("interlex_identifier", IRI, "vocab:interlexIdentifier", multiple=False, required=False,
-              doc="Persistent identifier for a term registered in the InterLex project."),
-        Field("knowledge_space_link", IRI, "vocab:knowledgeSpaceLink", multiple=False, required=False,
-              doc="Persistent link to an encyclopedia entry in the Knowledge Space project."),
-        Field("preferred_ontology_identifier", IRI, "vocab:preferredOntologyIdentifier", multiple=False, required=False,
-              doc="Persistent identifier of a preferred ontological term."),
-        Field("synonyms", str, "vocab:synonym", multiple=True, required=False,
-              doc="Words or expressions used in the same language that have the same or nearly the same meaning in some or all senses."),
+        Field("name", str, "vocab:fullName", multiple=False, required=True,
+              doc="Whole, non-abbreviated name of the license."),
+        Field("alias", str, "vocab:shortName", multiple=False, required=True,
+              doc="Shortened or fully abbreviated name of the license."),
+        Field("legal_code", IRI, "vocab:legalCode", multiple=False, required=True,
+              doc="Type of legislation that claims to cover the law system (complete or parts) as it existed at the time the code was enacted."),
+        Field("webpages", str, "vocab:webpage", multiple=True, required=False,
+              doc="Hypertext document (block of information) found on the World Wide Web."),
 
     ]
-    existence_query_fields = ('name',)
+    existence_query_fields = ('alias',)
```

### Comparing `fairgraph-0.8.2/fairgraph/openminds/controlledterms/stimulus_type.py` & `fairgraph-0.9.0/fairgraph/openminds/publications/periodical.py`

 * *Files 23% similar despite different names*

```diff
@@ -7,38 +7,30 @@
 from datetime import date, datetime
 from fairgraph.base_v3 import KGObject, IRI
 from fairgraph.fields import Field
 
 
 
 
-class StimulusType(KGObject):
+class Periodical(KGObject):
     """
 
     """
-    default_space = "controlled"
-    type = ["https://openminds.ebrains.eu/controlledTerms/StimulusType"]
+    default_space = "livepapers"
+    type = ["https://openminds.ebrains.eu/publications/Periodical"]
     context = {
         "schema": "http://schema.org/",
         "kg": "https://kg.ebrains.eu/api/instances/",
         "vocab": "https://openminds.ebrains.eu/vocab/",
         "terms": "https://openminds.ebrains.eu/controlledTerms/",
         "core": "https://openminds.ebrains.eu/core/"
     }
     fields = [
-        Field("name", str, "vocab:name", multiple=False, required=True,
-              doc="Word or phrase that constitutes the distinctive designation of the stimulus type."),
-        Field("definition", str, "vocab:definition", multiple=False, required=False,
-              doc="Short, but precise statement of the meaning of a word, word group, sign or a symbol."),
-        Field("description", str, "vocab:description", multiple=False, required=False,
-              doc="Longer statement or account giving the characteristics of the stimulus type."),
-        Field("interlex_identifier", IRI, "vocab:interlexIdentifier", multiple=False, required=False,
-              doc="Persistent identifier for a term registered in the InterLex project."),
-        Field("knowledge_space_link", IRI, "vocab:knowledgeSpaceLink", multiple=False, required=False,
-              doc="Persistent link to an encyclopedia entry in the Knowledge Space project."),
-        Field("preferred_ontology_identifier", IRI, "vocab:preferredOntologyIdentifier", multiple=False, required=False,
-              doc="Persistent identifier of a preferred ontological term."),
-        Field("synonyms", str, "vocab:synonym", multiple=True, required=False,
-              doc="Words or expressions used in the same language that have the same or nearly the same meaning in some or all senses."),
+        Field("name", str, "vocab:fullName", multiple=False, required=False,
+              doc="Whole, non-abbreviated name of the periodical."),
+        Field("alias", str, "vocab:shortName", multiple=False, required=True,
+              doc="Shortened or fully abbreviated name of the periodical."),
+        Field("digital_identifier", "openminds.core.ISSN", "vocab:digitalIdentifier", multiple=False, required=False,
+              doc="Digital handle to identify objects or legal persons."),
 
     ]
-    existence_query_fields = ('name',)
+    existence_query_fields = ('alias',)
```

### Comparing `fairgraph-0.8.2/fairgraph/openminds/controlledterms/subcellular_entity.py` & `fairgraph-0.9.0/fairgraph/openminds/sands/non_atlas/custom_anatomical_entity.py`

 * *Files 26% similar despite different names*

```diff
@@ -7,38 +7,32 @@
 from datetime import date, datetime
 from fairgraph.base_v3 import KGObject, IRI
 from fairgraph.fields import Field
 
 
 
 
-class SubcellularEntity(KGObject):
+class CustomAnatomicalEntity(KGObject):
     """
 
     """
-    default_space = "controlled"
-    type = ["https://openminds.ebrains.eu/controlledTerms/SubcellularEntity"]
+    default_space = "spatial"
+    type = ["https://openminds.ebrains.eu/sands/CustomAnatomicalEntity"]
     context = {
         "schema": "http://schema.org/",
         "kg": "https://kg.ebrains.eu/api/instances/",
         "vocab": "https://openminds.ebrains.eu/vocab/",
         "terms": "https://openminds.ebrains.eu/controlledTerms/",
         "core": "https://openminds.ebrains.eu/core/"
     }
     fields = [
         Field("name", str, "vocab:name", multiple=False, required=True,
-              doc="Word or phrase that constitutes the distinctive designation of the subcellular entity."),
-        Field("definition", str, "vocab:definition", multiple=False, required=False,
-              doc="Short, but precise statement of the meaning of a word, word group, sign or a symbol."),
-        Field("description", str, "vocab:description", multiple=False, required=False,
-              doc="Longer statement or account giving the characteristics of the subcellular entity."),
-        Field("interlex_identifier", IRI, "vocab:interlexIdentifier", multiple=False, required=False,
-              doc="Persistent identifier for a term registered in the InterLex project."),
-        Field("knowledge_space_link", IRI, "vocab:knowledgeSpaceLink", multiple=False, required=False,
-              doc="Persistent link to an encyclopedia entry in the Knowledge Space project."),
-        Field("preferred_ontology_identifier", IRI, "vocab:preferredOntologyIdentifier", multiple=False, required=False,
-              doc="Persistent identifier of a preferred ontological term."),
-        Field("synonyms", str, "vocab:synonym", multiple=True, required=False,
-              doc="Words or expressions used in the same language that have the same or nearly the same meaning in some or all senses."),
+              doc="Word or phrase that constitutes the distinctive designation of the custom anatomical entity."),
+        Field("has_annotations", "openminds.sands.CustomAnnotation", "vocab:hasAnnotation", multiple=True, required=False,
+              doc="no description available"),
+        Field("related_uberon_term", "openminds.controlledterms.UBERONParcellation", "vocab:relatedUBERONTerm", multiple=False, required=False,
+              doc="no description available"),
+        Field("relation_assessments", ["openminds.sands.QualitativeRelationAssessment", "openminds.sands.QuantitativeRelationAssessment"], "vocab:relationAssessment", multiple=True, required=False,
+              doc="no description available"),
 
     ]
     existence_query_fields = ('name',)
```

### Comparing `fairgraph-0.8.2/fairgraph/openminds/controlledterms/subject_attribute.py` & `fairgraph-0.9.0/fairgraph/openminds/controlledterms/setup_type.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,40 +1,64 @@
 """
 
+
+    .. list-table:: **Possible values**
+       :widths: 20 80
+       :header-rows: 0
+
+       * - acquisition system
+         - An 'acquisition system' is a setup type with the purpose of collecting data.
+       * - computing system
+         - A 'computing system' is a setup type with the purpose of performing computations.
+       * - stimulation system
+         - A 'stimulation system' is a setup type with the purpose of stimulating a specimen.
+
 """
 
 # this file was auto-generated
 
 from datetime import date, datetime
 from fairgraph.base_v3 import KGObject, IRI
 from fairgraph.fields import Field
 
 
 
 
-class SubjectAttribute(KGObject):
+class SetupType(KGObject):
     """
 
+
+    .. list-table:: **Possible values**
+       :widths: 20 80
+       :header-rows: 0
+
+       * - acquisition system
+         - An 'acquisition system' is a setup type with the purpose of collecting data.
+       * - computing system
+         - A 'computing system' is a setup type with the purpose of performing computations.
+       * - stimulation system
+         - A 'stimulation system' is a setup type with the purpose of stimulating a specimen.
+
     """
     default_space = "controlled"
-    type = ["https://openminds.ebrains.eu/controlledTerms/SubjectAttribute"]
+    type = ["https://openminds.ebrains.eu/controlledTerms/SetupType"]
     context = {
         "schema": "http://schema.org/",
         "kg": "https://kg.ebrains.eu/api/instances/",
         "vocab": "https://openminds.ebrains.eu/vocab/",
         "terms": "https://openminds.ebrains.eu/controlledTerms/",
         "core": "https://openminds.ebrains.eu/core/"
     }
     fields = [
         Field("name", str, "vocab:name", multiple=False, required=True,
-              doc="Word or phrase that constitutes the distinctive designation of the subject attribute."),
+              doc="Word or phrase that constitutes the distinctive designation of the setup type."),
         Field("definition", str, "vocab:definition", multiple=False, required=False,
               doc="Short, but precise statement of the meaning of a word, word group, sign or a symbol."),
         Field("description", str, "vocab:description", multiple=False, required=False,
-              doc="Longer statement or account giving the characteristics of the subject attribute."),
+              doc="Longer statement or account giving the characteristics of the setup type."),
         Field("interlex_identifier", IRI, "vocab:interlexIdentifier", multiple=False, required=False,
               doc="Persistent identifier for a term registered in the InterLex project."),
         Field("knowledge_space_link", IRI, "vocab:knowledgeSpaceLink", multiple=False, required=False,
               doc="Persistent link to an encyclopedia entry in the Knowledge Space project."),
         Field("preferred_ontology_identifier", IRI, "vocab:preferredOntologyIdentifier", multiple=False, required=False,
               doc="Persistent identifier of a preferred ontological term."),
         Field("synonyms", str, "vocab:synonym", multiple=True, required=False,
```

### Comparing `fairgraph-0.8.2/fairgraph/openminds/controlledterms/technique.py` & `fairgraph-0.9.0/fairgraph/openminds/core/research/tissue_sample_state.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,44 +1,46 @@
 """
-Structured information on the technique.
+Structured information on a temporary state of a tissue sample.
 """
 
 # this file was auto-generated
 
 from datetime import date, datetime
 from fairgraph.base_v3 import KGObject, IRI
 from fairgraph.fields import Field
 
 
 
 
-class Technique(KGObject):
+class TissueSampleState(KGObject):
     """
-    Structured information on the technique.
+    Structured information on a temporary state of a tissue sample.
     """
-    default_space = "controlled"
-    type = ["https://openminds.ebrains.eu/controlledTerms/Technique"]
+    default_space = "dataset"
+    type = ["https://openminds.ebrains.eu/core/TissueSampleState"]
     context = {
         "schema": "http://schema.org/",
         "kg": "https://kg.ebrains.eu/api/instances/",
         "vocab": "https://openminds.ebrains.eu/vocab/",
         "terms": "https://openminds.ebrains.eu/controlledTerms/",
         "core": "https://openminds.ebrains.eu/core/"
     }
     fields = [
-        Field("name", str, "vocab:name", multiple=False, required=True,
-              doc="Word or phrase that constitutes the distinctive designation of the technique."),
-        Field("definition", str, "vocab:definition", multiple=False, required=False,
-              doc="Short, but precise statement of the meaning of a word, word group, sign or a symbol."),
-        Field("description", str, "vocab:description", multiple=False, required=False,
-              doc="Longer statement or account giving the characteristics of the technique."),
-        Field("interlex_identifier", IRI, "vocab:interlexIdentifier", multiple=False, required=False,
-              doc="Persistent identifier for a term registered in the InterLex project."),
-        Field("knowledge_space_link", IRI, "vocab:knowledgeSpaceLink", multiple=False, required=False,
-              doc="Persistent link to an encyclopedia entry in the Knowledge Space project."),
-        Field("preferred_ontology_identifier", IRI, "vocab:preferredOntologyIdentifier", multiple=False, required=False,
-              doc="Persistent identifier of a preferred ontological term."),
-        Field("synonyms", str, "vocab:synonym", multiple=True, required=False,
-              doc="Words or expressions used in the same language that have the same or nearly the same meaning in some or all senses."),
+        Field("lookup_label", str, "vocab:lookupLabel", multiple=False, required=False,
+              doc="no description available"),
+        Field("additional_remarks", str, "vocab:additionalRemarks", multiple=False, required=False,
+              doc="Mention of what deserves additional attention or notice."),
+        Field("age", ["openminds.core.QuantitativeValue", "openminds.core.QuantitativeValueRange"], "vocab:age", multiple=False, required=False,
+              doc="Time of life or existence at which some particular qualification, capacity or event arises."),
+        Field("attributes", "openminds.controlledterms.TissueSampleAttribute", "vocab:attribute", multiple=True, required=False,
+              doc="no description available"),
+        Field("descended_from", ["openminds.core.SubjectGroupState", "openminds.core.SubjectState", "openminds.core.TissueSampleCollectionState", "openminds.core.TissueSampleState"], "vocab:descendedFrom", multiple=True, required=False,
+              doc="no description available"),
+        Field("pathologies", ["openminds.controlledterms.Disease", "openminds.controlledterms.DiseaseModel"], "vocab:pathology", multiple=True, required=False,
+              doc="Structural and functional deviation from the normal that constitutes a disease or characterizes a particular disease."),
+        Field("relative_time_indication", ["openminds.core.QuantitativeValue", "openminds.core.QuantitativeValueRange"], "vocab:relativeTimeIndication", multiple=False, required=False,
+              doc="no description available"),
+        Field("weight", ["openminds.core.QuantitativeValue", "openminds.core.QuantitativeValueRange"], "vocab:weight", multiple=False, required=False,
+              doc="Amount that a thing or being weighs."),
 
     ]
-    existence_query_fields = ('name',)
+    existence_query_fields = ('lookup_label',)
```

### Comparing `fairgraph-0.8.2/fairgraph/openminds/controlledterms/tissue_sample_attribute.py` & `fairgraph-0.9.0/fairgraph/openminds/sands/atlas/common_coordinate_space.py`

 * *Files 23% similar despite different names*

```diff
@@ -7,38 +7,52 @@
 from datetime import date, datetime
 from fairgraph.base_v3 import KGObject, IRI
 from fairgraph.fields import Field
 
 
 
 
-class TissueSampleAttribute(KGObject):
+class CommonCoordinateSpace(KGObject):
     """
 
     """
-    default_space = "controlled"
-    type = ["https://openminds.ebrains.eu/controlledTerms/TissueSampleAttribute"]
+    default_space = "atlas"
+    type = ["https://openminds.ebrains.eu/sands/CommonCoordinateSpace"]
     context = {
         "schema": "http://schema.org/",
         "kg": "https://kg.ebrains.eu/api/instances/",
         "vocab": "https://openminds.ebrains.eu/vocab/",
         "terms": "https://openminds.ebrains.eu/controlledTerms/",
         "core": "https://openminds.ebrains.eu/core/"
     }
     fields = [
-        Field("name", str, "vocab:name", multiple=False, required=True,
-              doc="Word or phrase that constitutes the distinctive designation of the tissue sample attribute."),
-        Field("definition", str, "vocab:definition", multiple=False, required=False,
-              doc="Short, but precise statement of the meaning of a word, word group, sign or a symbol."),
+        Field("name", str, "vocab:fullName", multiple=False, required=True,
+              doc="Whole, non-abbreviated name of the common coordinate space."),
+        Field("alias", str, "vocab:shortName", multiple=False, required=True,
+              doc="Shortened or fully abbreviated name of the common coordinate space."),
+        Field("anatomical_axes_orientation", "openminds.controlledterms.AnatomicalAxesOrientation", "vocab:anatomicalAxesOrientation", multiple=False, required=True,
+              doc="Relation between reference planes used in anatomy and mathematics."),
+        Field("axes_origins", "openminds.core.QuantitativeValue", "vocab:axesOrigin", multiple=True, required=True,
+              doc="Special point in a coordinate system used as a fixed point of reference for the geometry of the surrounding space."),
+        Field("default_images", "openminds.core.File", "vocab:defaultImage", multiple=True, required=False,
+              doc="Two or three dimensional image that particluarly represents a specific coordinate space."),
         Field("description", str, "vocab:description", multiple=False, required=False,
-              doc="Longer statement or account giving the characteristics of the tissue sample attribute."),
-        Field("interlex_identifier", IRI, "vocab:interlexIdentifier", multiple=False, required=False,
-              doc="Persistent identifier for a term registered in the InterLex project."),
-        Field("knowledge_space_link", IRI, "vocab:knowledgeSpaceLink", multiple=False, required=False,
-              doc="Persistent link to an encyclopedia entry in the Knowledge Space project."),
-        Field("preferred_ontology_identifier", IRI, "vocab:preferredOntologyIdentifier", multiple=False, required=False,
-              doc="Persistent identifier of a preferred ontological term."),
-        Field("synonyms", str, "vocab:synonym", multiple=True, required=False,
-              doc="Words or expressions used in the same language that have the same or nearly the same meaning in some or all senses."),
+              doc="Longer statement or account giving the characteristics of the common coordinate space."),
+        Field("digital_identifier", ["openminds.core.DOI", "openminds.core.ISBN", "openminds.core.RRID"], "vocab:digitalIdentifier", multiple=False, required=False,
+              doc="Digital handle to identify objects or legal persons."),
+        Field("homepage", "openminds.core.URL", "vocab:homepage", multiple=False, required=False,
+              doc="Main website of the common coordinate space."),
+        Field("how_to_cite", str, "vocab:howToCite", multiple=False, required=False,
+              doc="Preferred format for citing a particular object or legal person."),
+        Field("native_unit", "openminds.controlledterms.UnitOfMeasurement", "vocab:nativeUnit", multiple=False, required=True,
+              doc="Determinate quantity used in the original measurement."),
+        Field("ontology_identifiers", str, "vocab:ontologyIdentifier", multiple=True, required=False,
+              doc="Term or code used to identify the common coordinate space registered within a particular ontology."),
+        Field("release_date", date, "vocab:releaseDate", multiple=False, required=True,
+              doc="Fixed date on which a product is due to become or was made available for the general public to see or buy"),
+        Field("used_specimens", ["openminds.core.Subject", "openminds.core.SubjectGroup", "openminds.core.TissueSample", "openminds.core.TissueSampleCollection"], "vocab:usedSpecimen", multiple=True, required=False,
+              doc="no description available"),
+        Field("version_identifier", str, "vocab:versionIdentifier", multiple=False, required=True,
+              doc="Term or code used to identify the version of something."),
 
     ]
-    existence_query_fields = ('name',)
+    existence_query_fields = ('alias', 'version_identifier')
```

### Comparing `fairgraph-0.8.2/fairgraph/openminds/controlledterms/tissue_sample_type.py` & `fairgraph-0.9.0/fairgraph/openminds/ephys/device/electrode_array.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,44 +1,44 @@
 """
-Structured information on the general type of the tissue sample.
+
 """
 
 # this file was auto-generated
 
 from datetime import date, datetime
 from fairgraph.base_v3 import KGObject, IRI
 from fairgraph.fields import Field
 
 
 
 
-class TissueSampleType(KGObject):
+class ElectrodeArray(KGObject):
     """
-    Structured information on the general type of the tissue sample.
+
     """
-    default_space = "controlled"
-    type = ["https://openminds.ebrains.eu/controlledTerms/TissueSampleType"]
+    default_space = "in-depth"
+    type = ["https://openminds.ebrains.eu/ephys/ElectrodeArray"]
     context = {
         "schema": "http://schema.org/",
         "kg": "https://kg.ebrains.eu/api/instances/",
         "vocab": "https://openminds.ebrains.eu/vocab/",
         "terms": "https://openminds.ebrains.eu/controlledTerms/",
         "core": "https://openminds.ebrains.eu/core/"
     }
     fields = [
-        Field("name", str, "vocab:name", multiple=False, required=True,
-              doc="Word or phrase that constitutes the distinctive designation of the tissue sample type."),
-        Field("definition", str, "vocab:definition", multiple=False, required=False,
-              doc="Short, but precise statement of the meaning of a word, word group, sign or a symbol."),
-        Field("description", str, "vocab:description", multiple=False, required=False,
-              doc="Longer statement or account giving the characteristics of the tissue sample type."),
-        Field("interlex_identifier", IRI, "vocab:interlexIdentifier", multiple=False, required=False,
-              doc="Persistent identifier for a term registered in the InterLex project."),
-        Field("knowledge_space_link", IRI, "vocab:knowledgeSpaceLink", multiple=False, required=False,
-              doc="Persistent link to an encyclopedia entry in the Knowledge Space project."),
-        Field("preferred_ontology_identifier", IRI, "vocab:preferredOntologyIdentifier", multiple=False, required=False,
-              doc="Persistent identifier of a preferred ontological term."),
-        Field("synonyms", str, "vocab:synonym", multiple=True, required=False,
-              doc="Words or expressions used in the same language that have the same or nearly the same meaning in some or all senses."),
+        Field("lookup_label", str, "vocab:lookupLabel", multiple=False, required=False,
+              doc="no description available"),
+        Field("conductor_material", ["openminds.chemicals.ChemicalMixture", "openminds.chemicals.ChemicalSubstance", "openminds.controlledterms.MolecularEntity"], "vocab:conductorMaterial", multiple=False, required=False,
+              doc="no description available"),
+        Field("electrode_identifiers", str, "vocab:electrodeIdentifier", multiple=True, required=True,
+              doc="no description available"),
+        Field("insulator_material", ["openminds.chemicals.ChemicalMixture", "openminds.chemicals.ChemicalSubstance", "openminds.controlledterms.MolecularEntity"], "vocab:insulatorMaterial", multiple=False, required=False,
+              doc="no description available"),
+        Field("internal_identifier", str, "vocab:internalIdentifier", multiple=False, required=False,
+              doc="Term or code that identifies the electrode array within a particular product."),
+        Field("intrinsic_resistance", ["openminds.core.QuantitativeValue", "openminds.core.QuantitativeValueRange"], "vocab:intrinsicResistance", multiple=False, required=False,
+              doc="no description available"),
+        Field("number_of_electrodes", int, "vocab:numberOfElectrodes", multiple=False, required=True,
+              doc="no description available"),
 
     ]
-    existence_query_fields = ('name',)
+    existence_query_fields = ('lookup_label',)
```

### Comparing `fairgraph-0.8.2/fairgraph/openminds/controlledterms/type_of_uncertainty.py` & `fairgraph-0.9.0/fairgraph/openminds/specimenprep/device/slicing_device_usage.py`

 * *Files 26% similar despite different names*

```diff
@@ -7,38 +7,38 @@
 from datetime import date, datetime
 from fairgraph.base_v3 import KGObject, IRI
 from fairgraph.fields import Field
 
 
 
 
-class TypeOfUncertainty(KGObject):
+class SlicingDeviceUsage(KGObject):
     """
 
     """
-    default_space = "controlled"
-    type = ["https://openminds.ebrains.eu/controlledTerms/TypeOfUncertainty"]
+    default_space = "in-depth"
+    type = ["https://openminds.ebrains.eu/specimenPrep/SlicingDeviceUsage"]
     context = {
         "schema": "http://schema.org/",
         "kg": "https://kg.ebrains.eu/api/instances/",
         "vocab": "https://openminds.ebrains.eu/vocab/",
         "terms": "https://openminds.ebrains.eu/controlledTerms/",
         "core": "https://openminds.ebrains.eu/core/"
     }
     fields = [
-        Field("name", str, "vocab:name", multiple=False, required=True,
-              doc="Word or phrase that constitutes the distinctive designation of the type of uncertainty."),
-        Field("definition", str, "vocab:definition", multiple=False, required=False,
-              doc="Short, but precise statement of the meaning of a word, word group, sign or a symbol."),
-        Field("description", str, "vocab:description", multiple=False, required=False,
-              doc="Longer statement or account giving the characteristics of the type of uncertainty."),
-        Field("interlex_identifier", IRI, "vocab:interlexIdentifier", multiple=False, required=False,
-              doc="Persistent identifier for a term registered in the InterLex project."),
-        Field("knowledge_space_link", IRI, "vocab:knowledgeSpaceLink", multiple=False, required=False,
-              doc="Persistent link to an encyclopedia entry in the Knowledge Space project."),
-        Field("preferred_ontology_identifier", IRI, "vocab:preferredOntologyIdentifier", multiple=False, required=False,
-              doc="Persistent identifier of a preferred ontological term."),
-        Field("synonyms", str, "vocab:synonym", multiple=True, required=False,
-              doc="Words or expressions used in the same language that have the same or nearly the same meaning in some or all senses."),
+        Field("device", "openminds.specimenprep.SlicingDevice", "vocab:device", multiple=False, required=True,
+              doc="Piece of equipment or mechanism (hardware) designed to serve a special purpose or perform a special function."),
+        Field("oscillation_amplitude", "openminds.core.QuantitativeValue", "vocab:oscillationAmplitude", multiple=False, required=False,
+              doc="no description available"),
+        Field("slice_thickness", ["openminds.core.QuantitativeValue", "openminds.core.QuantitativeValueRange"], "vocab:sliceThickness", multiple=False, required=True,
+              doc="no description available"),
+        Field("slicing_angles", ["openminds.core.NumericalParameter", "openminds.core.QuantitativeValue"], "vocab:slicingAngle", multiple=True, required=False,
+              doc="no description available"),
+        Field("slicing_plane", "openminds.controlledterms.AnatomicalPlane", "vocab:slicingPlane", multiple=False, required=True,
+              doc="no description available"),
+        Field("slicing_speed", "openminds.core.QuantitativeValue", "vocab:slicingSpeed", multiple=False, required=False,
+              doc="no description available"),
+        Field("vibration_frequency", "openminds.core.QuantitativeValue", "vocab:vibrationFrequency", multiple=False, required=False,
+              doc="no description available"),
 
     ]
-    existence_query_fields = ('name',)
+    existence_query_fields = ('device', 'slice_thickness', 'slicing_plane')
```

### Comparing `fairgraph-0.8.2/fairgraph/openminds/controlledterms/uberon_parcellation.py` & `fairgraph-0.9.0/fairgraph/openminds/core/research/tissue_sample_collection_state.py`

 * *Files 25% similar despite different names*

```diff
@@ -7,38 +7,40 @@
 from datetime import date, datetime
 from fairgraph.base_v3 import KGObject, IRI
 from fairgraph.fields import Field
 
 
 
 
-class UBERONParcellation(KGObject):
+class TissueSampleCollectionState(KGObject):
     """
 
     """
-    default_space = "controlled"
-    type = ["https://openminds.ebrains.eu/controlledTerms/UBERONParcellation"]
+    default_space = "dataset"
+    type = ["https://openminds.ebrains.eu/core/TissueSampleCollectionState"]
     context = {
         "schema": "http://schema.org/",
         "kg": "https://kg.ebrains.eu/api/instances/",
         "vocab": "https://openminds.ebrains.eu/vocab/",
         "terms": "https://openminds.ebrains.eu/controlledTerms/",
         "core": "https://openminds.ebrains.eu/core/"
     }
     fields = [
-        Field("name", str, "vocab:name", multiple=False, required=True,
-              doc="Word or phrase that constitutes the distinctive designation of the u b e r o n parcellation."),
-        Field("definition", str, "vocab:definition", multiple=False, required=False,
-              doc="Short, but precise statement of the meaning of a word, word group, sign or a symbol."),
-        Field("description", str, "vocab:description", multiple=False, required=False,
-              doc="Longer statement or account giving the characteristics of the u b e r o n parcellation."),
-        Field("interlex_identifier", IRI, "vocab:interlexIdentifier", multiple=False, required=False,
-              doc="Persistent identifier for a term registered in the InterLex project."),
-        Field("knowledge_space_link", IRI, "vocab:knowledgeSpaceLink", multiple=False, required=False,
-              doc="Persistent link to an encyclopedia entry in the Knowledge Space project."),
-        Field("preferred_ontology_identifier", IRI, "vocab:preferredOntologyIdentifier", multiple=False, required=False,
-              doc="Persistent identifier of a preferred ontological term."),
-        Field("synonyms", str, "vocab:synonym", multiple=True, required=False,
-              doc="Words or expressions used in the same language that have the same or nearly the same meaning in some or all senses."),
+        Field("lookup_label", str, "vocab:lookupLabel", multiple=False, required=False,
+              doc="no description available"),
+        Field("additional_remarks", str, "vocab:additionalRemarks", multiple=False, required=False,
+              doc="Mention of what deserves additional attention or notice."),
+        Field("age", ["openminds.core.QuantitativeValue", "openminds.core.QuantitativeValueRange"], "vocab:age", multiple=False, required=False,
+              doc="Time of life or existence at which some particular qualification, capacity or event arises."),
+        Field("attributes", "openminds.controlledterms.TissueSampleAttribute", "vocab:attribute", multiple=True, required=False,
+              doc="no description available"),
+        Field("descended_from", ["openminds.core.SubjectGroupState", "openminds.core.SubjectState", "openminds.core.TissueSampleCollectionState", "openminds.core.TissueSampleState"], "vocab:descendedFrom", multiple=True, required=False,
+              doc="no description available"),
+        Field("pathologies", ["openminds.controlledterms.Disease", "openminds.controlledterms.DiseaseModel"], "vocab:pathology", multiple=True, required=False,
+              doc="Structural and functional deviation from the normal that constitutes a disease or characterizes a particular disease."),
+        Field("relative_time_indication", ["openminds.core.QuantitativeValue", "openminds.core.QuantitativeValueRange"], "vocab:relativeTimeIndication", multiple=False, required=False,
+              doc="no description available"),
+        Field("weight", ["openminds.core.QuantitativeValue", "openminds.core.QuantitativeValueRange"], "vocab:weight", multiple=False, required=False,
+              doc="Amount that a thing or being weighs."),
 
     ]
-    existence_query_fields = ('name',)
+    existence_query_fields = ('lookup_label',)
```

### Comparing `fairgraph-0.8.2/fairgraph/openminds/controlledterms/unit_of_measurement.py` & `fairgraph-0.9.0/fairgraph/openminds/core/actors/person.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,44 +1,67 @@
 """
-Structured information on the unit of measurement.
+Structured information on a person.
 """
 
 # this file was auto-generated
 
 from datetime import date, datetime
 from fairgraph.base_v3 import KGObject, IRI
 from fairgraph.fields import Field
 
 
 
 
-class UnitOfMeasurement(KGObject):
+class Person(KGObject):
     """
-    Structured information on the unit of measurement.
+    Structured information on a person.
     """
-    default_space = "controlled"
-    type = ["https://openminds.ebrains.eu/controlledTerms/UnitOfMeasurement"]
+    default_space = "common"
+    type = ["https://openminds.ebrains.eu/core/Person"]
     context = {
         "schema": "http://schema.org/",
         "kg": "https://kg.ebrains.eu/api/instances/",
         "vocab": "https://openminds.ebrains.eu/vocab/",
         "terms": "https://openminds.ebrains.eu/controlledTerms/",
         "core": "https://openminds.ebrains.eu/core/"
     }
     fields = [
-        Field("name", str, "vocab:name", multiple=False, required=True,
-              doc="Word or phrase that constitutes the distinctive designation of the unit of measurement."),
-        Field("definition", str, "vocab:definition", multiple=False, required=False,
-              doc="Short, but precise statement of the meaning of a word, word group, sign or a symbol."),
-        Field("description", str, "vocab:description", multiple=False, required=False,
-              doc="Longer statement or account giving the characteristics of the unit of measurement."),
-        Field("interlex_identifier", IRI, "vocab:interlexIdentifier", multiple=False, required=False,
-              doc="Persistent identifier for a term registered in the InterLex project."),
-        Field("knowledge_space_link", IRI, "vocab:knowledgeSpaceLink", multiple=False, required=False,
-              doc="Persistent link to an encyclopedia entry in the Knowledge Space project."),
-        Field("preferred_ontology_identifier", IRI, "vocab:preferredOntologyIdentifier", multiple=False, required=False,
-              doc="Persistent identifier of a preferred ontological term."),
-        Field("synonyms", str, "vocab:synonym", multiple=True, required=False,
-              doc="Words or expressions used in the same language that have the same or nearly the same meaning in some or all senses."),
+        Field("affiliations", "openminds.core.Affiliation", "vocab:affiliation", multiple=True, required=False,
+              doc="Declaration of a person being closely associated to an organization."),
+        Field("associated_accounts", "openminds.core.AccountInformation", "vocab:associatedAccount", multiple=True, required=False,
+              doc="no description available"),
+        Field("contact_information", "openminds.core.ContactInformation", "vocab:contactInformation", multiple=False, required=False,
+              doc="Any available way used to contact a person or business (e.g., address, phone number, email address, etc.)."),
+        Field("digital_identifiers", "openminds.core.ORCID", "vocab:digitalIdentifier", multiple=True, required=False,
+              doc="Digital handle to identify objects or legal persons."),
+        Field("family_name", str, "vocab:familyName", multiple=False, required=False,
+              doc="Name borne in common by members of a family."),
+        Field("given_name", str, "vocab:givenName", multiple=False, required=True,
+              doc="Name given to a person, including all potential middle names, but excluding the family name."),
 
     ]
-    existence_query_fields = ('name',)
+    existence_query_fields = ('given_name', 'family_name')
+
+
+    @property
+    def full_name(self):
+        return f"{self.given_name} {self.family_name}"
+
+    @classmethod
+    def me(cls, client, allow_multiple=False, resolved=False):
+        user_info = client.user_info()
+        possible_matches = cls.list(
+            client, scope="in progress", space="common",
+            resolved=resolved,
+            family_name=user_info.family_name,
+            given_name=user_info.given_name
+        )
+        if len(possible_matches) == 0:
+            person = Person(family_name=user_info.family_name,
+                            given_name=user_info.given_name)
+        elif len(possible_matches) == 1:
+            person = possible_matches[0]
+        elif allow_multiple:
+            person = possible_matches
+        else:
+            raise Exception("Found multiple matches")
+        return person
```

### Comparing `fairgraph-0.8.2/fairgraph/openminds/core/__init__.py` & `fairgraph-0.9.0/fairgraph/openminds/core/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 from .research.protocol_execution import ProtocolExecution
 from .research.behavioral_protocol import BehavioralProtocol
 from .research.string_property import StringProperty
 from .research.custom_property_set import CustomPropertySet
 from .research.subject import Subject
 from .research.strain import Strain
 from .research.tissue_sample_collection import TissueSampleCollection
-from .research.stimulation import Stimulation
 from .research.configuration import Configuration
 from .research.tissue_sample_state import TissueSampleState
 from .research.subject_state import SubjectState
 from .research.experimental_activity import ExperimentalActivity
 from .research.tissue_sample import TissueSample
 from .research.tissue_sample_collection_state import TissueSampleCollectionState
 from .research.protocol import Protocol
@@ -26,15 +25,17 @@
 from .products.software_version import SoftwareVersion
 from .products.dataset_version import DatasetVersion
 from .products.meta_data_model_version import MetaDataModelVersion
 from .products.setup import Setup
 from .products.model import Model
 from .products.software import Software
 from .products.meta_data_model import MetaDataModel
+from .products.web_service_version import WebServiceVersion
 from .products.model_version import ModelVersion
+from .products.web_service import WebService
 from .miscellaneous.doi import DOI
 from .miscellaneous.rorid import RORID
 from .miscellaneous.issn import ISSN
 from .miscellaneous.isbn import ISBN
 from .miscellaneous.quantitative_value import QuantitativeValue
 from .miscellaneous.rrid import RRID
 from .miscellaneous.orcid import ORCID
@@ -43,15 +44,17 @@
 from .miscellaneous.stock_number import StockNumber
 from .miscellaneous.comment import Comment
 from .miscellaneous.quantitative_value_range import QuantitativeValueRange
 from .miscellaneous.quantitative_value_array import QuantitativeValueArray
 from .miscellaneous.handle import HANDLE
 from .miscellaneous.swhid import SWHID
 from .miscellaneous.url import URL
+from .actors.account_information import AccountInformation
 from .actors.contribution import Contribution
+from .actors.consortium import Consortium
 from .actors.organization import Organization
 from .actors.contact_information import ContactInformation
 from .actors.affiliation import Affiliation
 from .actors.person import Person
 from .data.service_link import ServiceLink
 from .data.copyright import Copyright
 from .data.content_type_pattern import ContentTypePattern
```

### Comparing `fairgraph-0.8.2/fairgraph/openminds/core/actors/affiliation.py` & `fairgraph-0.9.0/fairgraph/openminds/core/research/configuration.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,34 +1,36 @@
 """
-
+Structured information about the properties or parameters of an entity or process.
 """
 
 # this file was auto-generated
 
 from datetime import date, datetime
-from fairgraph.base_v3 import EmbeddedMetadata, IRI
+from fairgraph.base_v3 import KGObject, IRI
 from fairgraph.fields import Field
 
 
 
 
-class Affiliation(EmbeddedMetadata):
+class Configuration(KGObject):
     """
-
+    Structured information about the properties or parameters of an entity or process.
     """
-    type = ["https://openminds.ebrains.eu/core/Affiliation"]
+    default_space = "common"
+    type = ["https://openminds.ebrains.eu/core/Configuration"]
     context = {
         "schema": "http://schema.org/",
         "kg": "https://kg.ebrains.eu/api/instances/",
         "vocab": "https://openminds.ebrains.eu/vocab/",
         "terms": "https://openminds.ebrains.eu/controlledTerms/",
         "core": "https://openminds.ebrains.eu/core/"
     }
     fields = [
-        Field("end_date", date, "vocab:endDate", multiple=False, required=False,
-              doc="Date in the Gregorian calendar at which something terminates in time."),
-        Field("organization", "openminds.core.Organization", "vocab:organization", multiple=False, required=True,
-              doc="Legally accountable, administrative and functional structure."),
-        Field("start_date", date, "vocab:startDate", multiple=False, required=False,
-              doc="Date in the Gregorian calendar at which something begins in time"),
+        Field("lookup_label", str, "vocab:lookupLabel", multiple=False, required=False,
+              doc="no description available"),
+        Field("configuration", str, "vocab:configuration", multiple=False, required=True,
+              doc="no description available"),
+        Field("definition_format", "openminds.core.ContentType", "vocab:definitionFormat", multiple=False, required=True,
+              doc="no description available"),
 
     ]
+    existence_query_fields = ('configuration',)
```

### Comparing `fairgraph-0.8.2/fairgraph/openminds/core/actors/contact_information.py` & `fairgraph-0.9.0/fairgraph/openminds/core/actors/contact_information.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 """
-
+Structured information about how to contact a given person.
 """
 
 # this file was auto-generated
 
 from datetime import date, datetime
 from fairgraph.base_v3 import KGObject, IRI
 from fairgraph.fields import Field
 
 
 
 
 class ContactInformation(KGObject):
     """
-
+    Structured information about how to contact a given person.
     """
     default_space = "restricted"
     type = ["https://openminds.ebrains.eu/core/ContactInformation"]
     context = {
         "schema": "http://schema.org/",
         "kg": "https://kg.ebrains.eu/api/instances/",
         "vocab": "https://openminds.ebrains.eu/vocab/",
```

### Comparing `fairgraph-0.8.2/fairgraph/openminds/core/actors/contribution.py` & `fairgraph-0.9.0/fairgraph/openminds/core/actors/contribution.py`

 * *Files 7% similar despite different names*

```diff
@@ -22,11 +22,11 @@
         "vocab": "https://openminds.ebrains.eu/vocab/",
         "terms": "https://openminds.ebrains.eu/controlledTerms/",
         "core": "https://openminds.ebrains.eu/core/"
     }
     fields = [
         Field("contribution_types", "openminds.controlledterms.ContributionType", "vocab:contributionType", multiple=True, required=True,
               doc="Distinct class of what was given or supplied as a part or share."),
-        Field("contributor", ["openminds.core.Organization", "openminds.core.Person"], "vocab:contributor", multiple=False, required=True,
+        Field("contributor", ["openminds.core.Consortium", "openminds.core.Organization", "openminds.core.Person"], "vocab:contributor", multiple=False, required=True,
               doc="Legal person that gave or supplied something as a part or share."),
 
     ]
```

### Comparing `fairgraph-0.8.2/fairgraph/openminds/core/actors/organization.py` & `fairgraph-0.9.0/fairgraph/openminds/core/miscellaneous/quantitative_value.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,40 +1,36 @@
 """
-Structured information on an organization.
+Structured information on a quantitative value.
 """
 
 # this file was auto-generated
 
 from datetime import date, datetime
-from fairgraph.base_v3 import KGObject, IRI
+from fairgraph.base_v3 import EmbeddedMetadata, IRI
 from fairgraph.fields import Field
 
 
 
 
-class Organization(KGObject):
+class QuantitativeValue(EmbeddedMetadata):
     """
-    Structured information on an organization.
+    Structured information on a quantitative value.
     """
-    default_space = "common"
-    type = ["https://openminds.ebrains.eu/core/Organization"]
+    type = ["https://openminds.ebrains.eu/core/QuantitativeValue"]
     context = {
         "schema": "http://schema.org/",
         "kg": "https://kg.ebrains.eu/api/instances/",
         "vocab": "https://openminds.ebrains.eu/vocab/",
         "terms": "https://openminds.ebrains.eu/controlledTerms/",
         "core": "https://openminds.ebrains.eu/core/"
     }
     fields = [
-        Field("name", str, "vocab:fullName", multiple=False, required=True,
-              doc="Whole, non-abbreviated name of the organization."),
-        Field("alias", str, "vocab:shortName", multiple=False, required=False,
-              doc="Shortened or fully abbreviated name of the organization."),
-        Field("digital_identifiers", ["openminds.core.GRIDID", "openminds.core.RORID", "openminds.core.RRID"], "vocab:digitalIdentifier", multiple=True, required=False,
-              doc="Digital handle to identify objects or legal persons."),
-        Field("has_parent", "openminds.core.Organization", "vocab:hasParent", multiple=False, required=False,
-              doc="Reference to a parent object or legal person."),
-        Field("homepage", "openminds.core.URL", "vocab:homepage", multiple=False, required=False,
-              doc="Main website of the organization."),
+        Field("type_of_uncertainty", "openminds.controlledterms.TypeOfUncertainty", "vocab:typeOfUncertainty", multiple=False, required=False,
+              doc="Distinct technique used to quantify the uncertainty of a measurement."),
+        Field("uncertainties", float, "vocab:uncertainty", multiple=True, required=False,
+              doc="Quantitative value range defining the uncertainty of a measurement."),
+        Field("unit", "openminds.controlledterms.UnitOfMeasurement", "vocab:unit", multiple=False, required=False,
+              doc="Determinate quantity adopted as a standard of measurement."),
+        Field("value", float, "vocab:value", multiple=False, required=True,
+              doc="Entry for a property."),
 
     ]
-    existence_query_fields = ('name',)
```

### Comparing `fairgraph-0.8.2/fairgraph/openminds/core/data/content_type.py` & `fairgraph-0.9.0/fairgraph/openminds/core/miscellaneous/quantitative_value_range.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,46 +1,36 @@
 """
-Structured information on the content type of a file instance, bundle or repository.
+A representation of a range of quantitative values.
 """
 
 # this file was auto-generated
 
 from datetime import date, datetime
-from fairgraph.base_v3 import KGObject, IRI
+from fairgraph.base_v3 import EmbeddedMetadata, IRI
 from fairgraph.fields import Field
 
 
 
 
-class ContentType(KGObject):
+class QuantitativeValueRange(EmbeddedMetadata):
     """
-    Structured information on the content type of a file instance, bundle or repository.
+    A representation of a range of quantitative values.
     """
-    default_space = "controlled"
-    type = ["https://openminds.ebrains.eu/core/ContentType"]
+    type = ["https://openminds.ebrains.eu/core/QuantitativeValueRange"]
     context = {
         "schema": "http://schema.org/",
         "kg": "https://kg.ebrains.eu/api/instances/",
         "vocab": "https://openminds.ebrains.eu/vocab/",
         "terms": "https://openminds.ebrains.eu/controlledTerms/",
         "core": "https://openminds.ebrains.eu/core/"
     }
     fields = [
-        Field("name", str, "vocab:name", multiple=False, required=True,
-              doc="Word or phrase that constitutes the distinctive designation of the content type."),
-        Field("data_types", "openminds.controlledterms.DataType", "vocab:dataType", multiple=True, required=False,
+        Field("max_value", float, "vocab:maxValue", multiple=False, required=True,
+              doc="Greatest quantity attained or allowed."),
+        Field("max_value_unit", "openminds.controlledterms.UnitOfMeasurement", "vocab:maxValueUnit", multiple=False, required=False,
               doc="no description available"),
-        Field("description", str, "vocab:description", multiple=False, required=False,
-              doc="Longer statement or account giving the characteristics of the content type."),
-        Field("display_label", str, "vocab:displayLabel", multiple=False, required=False,
+        Field("min_value", float, "vocab:minValue", multiple=False, required=True,
+              doc="Smallest quantity attained or allowed."),
+        Field("min_value_unit", "openminds.controlledterms.UnitOfMeasurement", "vocab:minValueUnit", multiple=False, required=False,
               doc="no description available"),
-        Field("file_extensions", str, "vocab:fileExtension", multiple=True, required=False,
-              doc="String of characters attached as suffix to the names of files of a particular format."),
-        Field("related_media_type", IRI, "vocab:relatedMediaType", multiple=False, required=False,
-              doc="Reference to an official two-part identifier for file formats and format contents."),
-        Field("specification", IRI, "vocab:specification", multiple=False, required=False,
-              doc="Detailed and precise presentation of, or proposal for something."),
-        Field("synonyms", str, "vocab:synonym", multiple=True, required=False,
-              doc="Words or expressions used in the same language that have the same or nearly the same meaning in some or all senses."),
 
     ]
-    existence_query_fields = ('name',)
```

### Comparing `fairgraph-0.8.2/fairgraph/openminds/core/data/content_type_pattern.py` & `fairgraph-0.9.0/fairgraph/openminds/core/data/content_type_pattern.py`

 * *Files identical despite different names*

### Comparing `fairgraph-0.8.2/fairgraph/openminds/core/data/copyright.py` & `fairgraph-0.9.0/fairgraph/openminds/core/data/copyright.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,13 +20,13 @@
         "schema": "http://schema.org/",
         "kg": "https://kg.ebrains.eu/api/instances/",
         "vocab": "https://openminds.ebrains.eu/vocab/",
         "terms": "https://openminds.ebrains.eu/controlledTerms/",
         "core": "https://openminds.ebrains.eu/core/"
     }
     fields = [
-        Field("holders", ["openminds.core.Organization", "openminds.core.Person"], "vocab:holder", multiple=True, required=True,
+        Field("holders", ["openminds.core.Consortium", "openminds.core.Organization", "openminds.core.Person"], "vocab:holder", multiple=True, required=True,
               doc="Legal person in possession of something."),
         Field("year", str, "vocab:year", multiple=False, required=True,
               doc="Cycle in the Gregorian calendar specified by a number and comprised of 365 or 366 days divided into 12 months beginning with January and ending with December."),
 
     ]
```

### Comparing `fairgraph-0.8.2/fairgraph/openminds/core/data/file.py` & `fairgraph-0.9.0/fairgraph/openminds/core/data/file.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Structured information on a file instances.
+Structured information on a file instance.
 """
 
 # this file was auto-generated
 
 from datetime import date, datetime
 from fairgraph.base_v3 import KGObject, IRI
 from fairgraph.fields import Field
@@ -33,15 +33,15 @@
             h.update(data)
     return h.hexdigest()
 
 
 
 class File(KGObject):
     """
-    Structured information on a file instances.
+    Structured information on a file instance.
     """
     default_space = "files"
     type = ["https://openminds.ebrains.eu/core/File"]
     context = {
         "schema": "http://schema.org/",
         "kg": "https://kg.ebrains.eu/api/instances/",
         "vocab": "https://openminds.ebrains.eu/vocab/",
```

### Comparing `fairgraph-0.8.2/fairgraph/openminds/core/data/file_archive.py` & `fairgraph-0.9.0/fairgraph/openminds/core/miscellaneous/isbn.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,36 +1,32 @@
 """
-
+An International Standard Book Number of the International ISBN Agency.
 """
 
 # this file was auto-generated
 
 from datetime import date, datetime
 from fairgraph.base_v3 import KGObject, IRI
 from fairgraph.fields import Field
 
 
 
 
-class FileArchive(KGObject):
+class ISBN(KGObject):
     """
-
+    An International Standard Book Number of the International ISBN Agency.
     """
     default_space = "dataset"
-    type = ["https://openminds.ebrains.eu/core/FileArchive"]
+    type = ["https://openminds.ebrains.eu/core/ISBN"]
     context = {
         "schema": "http://schema.org/",
         "kg": "https://kg.ebrains.eu/api/instances/",
         "vocab": "https://openminds.ebrains.eu/vocab/",
         "terms": "https://openminds.ebrains.eu/controlledTerms/",
         "core": "https://openminds.ebrains.eu/core/"
     }
     fields = [
-        Field("iri", IRI, "vocab:IRI", multiple=False, required=True,
-              doc="Stands for Internationalized Resource Identifier which is an internet protocol standard that builds on the URI protocol, extending the set of permitted characters to include Unicode/ISO 10646."),
-        Field("format", "openminds.core.ContentType", "vocab:format", multiple=False, required=True,
-              doc="Method of digitally organizing and structuring data or information."),
-        Field("source_datas", "openminds.core.File", "vocab:sourceData", multiple=True, required=False,
-              doc="no description available"),
+        Field("identifier", str, "vocab:identifier", multiple=False, required=True,
+              doc="Term or code used to identify the ISBN."),
 
     ]
-    existence_query_fields = ('iri', 'format')
+    existence_query_fields = ('identifier',)
```

### Comparing `fairgraph-0.8.2/fairgraph/openminds/core/data/file_bundle.py` & `fairgraph-0.9.0/fairgraph/openminds/core/data/file_bundle.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,15 +25,15 @@
         "core": "https://openminds.ebrains.eu/core/"
     }
     fields = [
         Field("name", str, "vocab:name", multiple=False, required=True,
               doc="Word or phrase that constitutes the distinctive designation of the file bundle."),
         Field("content_description", str, "vocab:contentDescription", multiple=False, required=False,
               doc="no description available"),
-        Field("descended_from", ["openminds.computation.LocalFile", "openminds.controlledterms.Technique", "openminds.core.BehavioralProtocol", "openminds.core.File", "openminds.core.FileBundle", "openminds.core.Subject", "openminds.core.SubjectGroup", "openminds.core.SubjectGroupState", "openminds.core.SubjectState", "openminds.core.TissueSample", "openminds.core.TissueSampleCollection", "openminds.core.TissueSampleCollectionState", "openminds.core.TissueSampleState"], "vocab:descendedFrom", multiple=False, required=False,
+        Field("descended_from", ["openminds.computation.LocalFile", "openminds.controlledterms.StimulationTechnique", "openminds.controlledterms.Technique", "openminds.core.BehavioralProtocol", "openminds.core.File", "openminds.core.FileBundle", "openminds.core.Subject", "openminds.core.SubjectGroup", "openminds.core.SubjectGroupState", "openminds.core.SubjectState", "openminds.core.TissueSample", "openminds.core.TissueSampleCollection", "openminds.core.TissueSampleCollectionState", "openminds.core.TissueSampleState"], "vocab:descendedFrom", multiple=False, required=False,
               doc="no description available"),
         Field("format", "openminds.core.ContentType", "vocab:format", multiple=False, required=False,
               doc="Method of digitally organizing and structuring data or information."),
         Field("grouping_type", "openminds.controlledterms.FileBundleGrouping", "vocab:groupingType", multiple=False, required=False,
               doc="no description available"),
         Field("hash", "openminds.core.Hash", "vocab:hash", multiple=False, required=False,
               doc="Term used for the process of converting any data into a single value. Often also directly refers to the resulting single value."),
```

### Comparing `fairgraph-0.8.2/fairgraph/openminds/core/data/file_path_pattern.py` & `fairgraph-0.9.0/fairgraph/openminds/core/data/file_path_pattern.py`

 * *Files identical despite different names*

### Comparing `fairgraph-0.8.2/fairgraph/openminds/core/data/file_repository_structure.py` & `fairgraph-0.9.0/fairgraph/openminds/core/data/file_repository_structure.py`

 * *Files identical despite different names*

### Comparing `fairgraph-0.8.2/fairgraph/openminds/core/data/hash.py` & `fairgraph-0.9.0/fairgraph/openminds/core/data/hash.py`

 * *Files identical despite different names*

### Comparing `fairgraph-0.8.2/fairgraph/openminds/core/data/license.py` & `fairgraph-0.9.0/fairgraph/openminds/core/research/numerical_property.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,38 +1,32 @@
 """
-Structured information on a used license.
+Structured information about a property of some entity or process whose value is a number.
 """
 
 # this file was auto-generated
 
 from datetime import date, datetime
-from fairgraph.base_v3 import KGObject, IRI
+from fairgraph.base_v3 import EmbeddedMetadata, IRI
 from fairgraph.fields import Field
 
 
 
 
-class License(KGObject):
+class NumericalProperty(EmbeddedMetadata):
     """
-    Structured information on a used license.
+    Structured information about a property of some entity or process whose value is a number.
     """
-    default_space = "controlled"
-    type = ["https://openminds.ebrains.eu/core/License"]
+    type = ["https://openminds.ebrains.eu/core/NumericalProperty"]
     context = {
         "schema": "http://schema.org/",
         "kg": "https://kg.ebrains.eu/api/instances/",
         "vocab": "https://openminds.ebrains.eu/vocab/",
         "terms": "https://openminds.ebrains.eu/controlledTerms/",
         "core": "https://openminds.ebrains.eu/core/"
     }
     fields = [
-        Field("name", str, "vocab:fullName", multiple=False, required=True,
-              doc="Whole, non-abbreviated name of the license."),
-        Field("alias", str, "vocab:shortName", multiple=False, required=True,
-              doc="Shortened or fully abbreviated name of the license."),
-        Field("legal_code", IRI, "vocab:legalCode", multiple=False, required=True,
-              doc="Type of legislation that claims to cover the law system (complete or parts) as it existed at the time the code was enacted."),
-        Field("webpages", str, "vocab:webpage", multiple=True, required=False,
-              doc="Hypertext document (block of information) found on the World Wide Web."),
+        Field("name", str, "vocab:name", multiple=False, required=True,
+              doc="Word or phrase that constitutes the distinctive designation of the numerical property."),
+        Field("values", ["openminds.core.QuantitativeValue", "openminds.core.QuantitativeValueRange"], "vocab:value", multiple=True, required=True,
+              doc="Entry for a property."),
 
     ]
-    existence_query_fields = ('alias',)
```

### Comparing `fairgraph-0.8.2/fairgraph/openminds/core/data/measurement.py` & `fairgraph-0.9.0/fairgraph/openminds/core/data/measurement.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 """
-
+Structured information about a measurement performed during a scientific experiment.
 """
 
 # this file was auto-generated
 
 from datetime import date, datetime
 from fairgraph.base_v3 import EmbeddedMetadata, IRI
 from fairgraph.fields import Field
 
 
 
 
 class Measurement(EmbeddedMetadata):
     """
-
+    Structured information about a measurement performed during a scientific experiment.
     """
     type = ["https://openminds.ebrains.eu/core/Measurement"]
     context = {
         "schema": "http://schema.org/",
         "kg": "https://kg.ebrains.eu/api/instances/",
         "vocab": "https://openminds.ebrains.eu/vocab/",
         "terms": "https://openminds.ebrains.eu/controlledTerms/",
         "core": "https://openminds.ebrains.eu/core/"
     }
     fields = [
         Field("additional_remarks", str, "vocab:additionalRemarks", multiple=False, required=False,
               doc="Mention of what deserves additional attention or notice."),
         Field("measured_quantity", "openminds.controlledterms.MeasuredQuantity", "vocab:measuredQuantity", multiple=False, required=True,
               doc="no description available"),
-        Field("measured_with", ["openminds.ephys.ElectrodeArrayUsage", "openminds.ephys.ElectrodeUsage", "openminds.ephys.PipetteUsage"], "vocab:measuredWith", multiple=False, required=False,
+        Field("measured_with", ["openminds.ephys.ElectrodeArrayUsage", "openminds.ephys.ElectrodeUsage", "openminds.ephys.PipetteUsage", "openminds.specimenprep.SlicingDeviceUsage"], "vocab:measuredWith", multiple=False, required=False,
               doc="no description available"),
         Field("timestamp", datetime, "vocab:timestamp", multiple=False, required=False,
               doc="no description available"),
         Field("values", ["openminds.core.QuantitativeValue", "openminds.core.QuantitativeValueRange"], "vocab:value", multiple=True, required=True,
               doc="Entry for a property."),
 
     ]
```

### Comparing `fairgraph-0.8.2/fairgraph/openminds/core/data/service_link.py` & `fairgraph-0.9.0/fairgraph/openminds/sands/atlas/parcellation_terminology.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,40 +1,34 @@
 """
 
 """
 
 # this file was auto-generated
 
 from datetime import date, datetime
-from fairgraph.base_v3 import KGObject, IRI
+from fairgraph.base_v3 import EmbeddedMetadata, IRI
 from fairgraph.fields import Field
 
 
 
 
-class ServiceLink(KGObject):
+class ParcellationTerminology(EmbeddedMetadata):
     """
 
     """
-    default_space = "dataset"
-    type = ["https://openminds.ebrains.eu/core/ServiceLink"]
+    type = ["https://openminds.ebrains.eu/sands/ParcellationTerminology"]
     context = {
         "schema": "http://schema.org/",
         "kg": "https://kg.ebrains.eu/api/instances/",
         "vocab": "https://openminds.ebrains.eu/vocab/",
         "terms": "https://openminds.ebrains.eu/controlledTerms/",
         "core": "https://openminds.ebrains.eu/core/"
     }
     fields = [
-        Field("name", str, "vocab:name", multiple=False, required=False,
-              doc="Word or phrase that constitutes the distinctive designation of the service link."),
-        Field("data_location", ["openminds.core.File", "openminds.core.FileArchive", "openminds.core.FileBundle", "openminds.publications.LivePaperResourceItem", "openminds.sands.ParcellationEntityVersion"], "vocab:dataLocation", multiple=False, required=True,
-              doc="no description available"),
-        Field("open_data_in", "openminds.core.URL", "vocab:openDataIn", multiple=False, required=True,
-              doc="no description available"),
-        Field("preview_image", "openminds.core.File", "vocab:previewImage", multiple=False, required=False,
-              doc="no description available"),
-        Field("service", "openminds.controlledterms.Service", "vocab:service", multiple=False, required=True,
+        Field("defined_ins", "openminds.core.File", "vocab:definedIn", multiple=True, required=False,
+              doc="Reference to a file instance in which something is stored."),
+        Field("entities", "openminds.sands.ParcellationEntity", "vocab:hasEntity", multiple=True, required=True,
               doc="no description available"),
+        Field("ontology_identifiers", str, "vocab:ontologyIdentifier", multiple=True, required=False,
+              doc="Term or code used to identify the parcellation terminology registered within a particular ontology."),
 
     ]
-    existence_query_fields = ('data_location', 'open_data_in', 'service')
```

### Comparing `fairgraph-0.8.2/fairgraph/openminds/core/miscellaneous/comment.py` & `fairgraph-0.9.0/fairgraph/openminds/core/miscellaneous/comment.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 """
-
+Structured information about a short text associated with some entity.
 """
 
 # this file was auto-generated
 
 from datetime import date, datetime
 from fairgraph.base_v3 import KGObject, IRI
 from fairgraph.fields import Field
 
 
 
 
 class Comment(KGObject):
     """
-
+    Structured information about a short text associated with some entity.
     """
     default_space = "common"
     type = ["https://openminds.ebrains.eu/core/Comment"]
     context = {
         "schema": "http://schema.org/",
         "kg": "https://kg.ebrains.eu/api/instances/",
         "vocab": "https://openminds.ebrains.eu/vocab/",
@@ -25,14 +25,14 @@
         "core": "https://openminds.ebrains.eu/core/"
     }
     fields = [
         Field("commenter", "openminds.core.Person", "vocab:commenter", multiple=False, required=True,
               doc="no description available"),
         Field("content", str, "vocab:content", multiple=False, required=True,
               doc="Something that is contained."),
-        Field("subject", ["openminds.computation.ValidationTest", "openminds.computation.ValidationTestVersion", "openminds.computation.WorkflowRecipe", "openminds.computation.WorkflowRecipeVersion", "openminds.core.Dataset", "openminds.core.DatasetVersion", "openminds.core.MetaDataModel", "openminds.core.MetaDataModelVersion", "openminds.core.Model", "openminds.core.ModelVersion", "openminds.core.Software", "openminds.core.SoftwareVersion", "openminds.publications.LivePaper", "openminds.publications.LivePaperVersion", "openminds.sands.BrainAtlas", "openminds.sands.BrainAtlasVersion"], "vocab:subject", multiple=False, required=True,
+        Field("subject", ["openminds.computation.ValidationTest", "openminds.computation.ValidationTestVersion", "openminds.computation.WorkflowRecipe", "openminds.computation.WorkflowRecipeVersion", "openminds.core.Dataset", "openminds.core.DatasetVersion", "openminds.core.MetaDataModel", "openminds.core.MetaDataModelVersion", "openminds.core.Model", "openminds.core.ModelVersion", "openminds.core.Software", "openminds.core.SoftwareVersion", "openminds.core.WebService", "openminds.core.WebServiceVersion", "openminds.publications.LivePaper", "openminds.publications.LivePaperVersion", "openminds.sands.BrainAtlas", "openminds.sands.BrainAtlasVersion"], "vocab:subject", multiple=False, required=True,
               doc="no description available"),
         Field("timestamp", datetime, "vocab:timestamp", multiple=False, required=True,
               doc="no description available"),
 
     ]
     existence_query_fields = ('commenter', 'content', 'subject', 'timestamp')
```

### Comparing `fairgraph-0.8.2/fairgraph/openminds/core/miscellaneous/doi.py` & `fairgraph-0.9.0/fairgraph/openminds/core/miscellaneous/stock_number.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 """
 
 """
 
 # this file was auto-generated
 
 from datetime import date, datetime
-from fairgraph.base_v3 import KGObject, IRI
+from fairgraph.base_v3 import EmbeddedMetadata, IRI
 from fairgraph.fields import Field
 
 
 
 
-class DOI(KGObject):
+class StockNumber(EmbeddedMetadata):
     """
 
     """
-    default_space = "dataset"
-    type = ["https://openminds.ebrains.eu/core/DOI"]
+    type = ["https://openminds.ebrains.eu/core/StockNumber"]
     context = {
         "schema": "http://schema.org/",
         "kg": "https://kg.ebrains.eu/api/instances/",
         "vocab": "https://openminds.ebrains.eu/vocab/",
         "terms": "https://openminds.ebrains.eu/controlledTerms/",
         "core": "https://openminds.ebrains.eu/core/"
     }
     fields = [
         Field("identifier", str, "vocab:identifier", multiple=False, required=True,
-              doc="Term or code used to identify the DOI."),
+              doc="Term or code used to identify the stock number."),
+        Field("vendor", "openminds.core.Organization", "vocab:vendor", multiple=False, required=True,
+              doc="no description available"),
 
     ]
-    existence_query_fields = ('identifier',)
```

### Comparing `fairgraph-0.8.2/fairgraph/openminds/core/miscellaneous/funding.py` & `fairgraph-0.9.0/fairgraph/openminds/core/research/custom_property_set.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,38 +1,34 @@
 """
-Structured information on used funding.
+Structured information about properties of an entity that cannot be represented with a more general openMINDS schema.
 """
 
 # this file was auto-generated
 
 from datetime import date, datetime
-from fairgraph.base_v3 import KGObject, IRI
+from fairgraph.base_v3 import EmbeddedMetadata, IRI
 from fairgraph.fields import Field
 
 
 
 
-class Funding(KGObject):
+class CustomPropertySet(EmbeddedMetadata):
     """
-    Structured information on used funding.
+    Structured information about properties of an entity that cannot be represented with a more general openMINDS schema.
     """
-    default_space = "common"
-    type = ["https://openminds.ebrains.eu/core/Funding"]
+    type = ["https://openminds.ebrains.eu/core/CustomPropertySet"]
     context = {
         "schema": "http://schema.org/",
         "kg": "https://kg.ebrains.eu/api/instances/",
         "vocab": "https://openminds.ebrains.eu/vocab/",
         "terms": "https://openminds.ebrains.eu/controlledTerms/",
         "core": "https://openminds.ebrains.eu/core/"
     }
     fields = [
-        Field("acknowledgement", str, "vocab:acknowledgement", multiple=False, required=False,
-              doc="Offical declaration or avowal of appreciation of an act or achievement."),
-        Field("award_number", str, "vocab:awardNumber", multiple=False, required=False,
-              doc="Machine-readable identifier for a benefit that is conferred or bestowed on the basis of merit or need."),
-        Field("award_title", str, "vocab:awardTitle", multiple=False, required=False,
-              doc="Human-readable identifier for a benefit that is conferred or bestowed on the basis of merit or need."),
-        Field("funder", ["openminds.core.Organization", "openminds.core.Person"], "vocab:funder", multiple=False, required=True,
-              doc="Legal person that provides money for a particular purpose."),
+        Field("context", str, "vocab:context", multiple=False, required=True,
+              doc="no description available"),
+        Field("defined_in", ["openminds.core.Configuration", "openminds.core.File", "openminds.core.PropertyValueList"], "vocab:definedIn", multiple=False, required=True,
+              doc="Reference to a file instance in which something is stored."),
+        Field("relevant_for", "openminds.controlledterms.Technique", "vocab:relevantFor", multiple=False, required=True,
+              doc="Reference to what or whom the custom property set bears siginificance."),
 
     ]
-    existence_query_fields = ('funder',)
```

### Comparing `fairgraph-0.8.2/fairgraph/openminds/core/miscellaneous/gridid.py` & `fairgraph-0.9.0/fairgraph/openminds/core/miscellaneous/rorid.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 """
-
+A persistent identifier for a research organization, provided by the Research Organization Registry.
 """
 
 # this file was auto-generated
 
 from datetime import date, datetime
 from fairgraph.base_v3 import KGObject, IRI
 from fairgraph.fields import Field
 
 
 
 
-class GRIDID(KGObject):
+class RORID(KGObject):
     """
-
+    A persistent identifier for a research organization, provided by the Research Organization Registry.
     """
     default_space = "common"
-    type = ["https://openminds.ebrains.eu/core/GRIDID"]
+    type = ["https://openminds.ebrains.eu/core/RORID"]
     context = {
         "schema": "http://schema.org/",
         "kg": "https://kg.ebrains.eu/api/instances/",
         "vocab": "https://openminds.ebrains.eu/vocab/",
         "terms": "https://openminds.ebrains.eu/controlledTerms/",
         "core": "https://openminds.ebrains.eu/core/"
     }
     fields = [
         Field("identifier", str, "vocab:identifier", multiple=False, required=True,
-              doc="Term or code used to identify the GRIDID."),
+              doc="Term or code used to identify the RORID."),
 
     ]
     existence_query_fields = ('identifier',)
```

### Comparing `fairgraph-0.8.2/fairgraph/openminds/core/miscellaneous/handle.py` & `fairgraph-0.9.0/fairgraph/openminds/core/miscellaneous/swhid.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,26 +7,26 @@
 from datetime import date, datetime
 from fairgraph.base_v3 import KGObject, IRI
 from fairgraph.fields import Field
 
 
 
 
-class HANDLE(KGObject):
+class SWHID(KGObject):
     """
 
     """
-    default_space = "common"
-    type = ["https://openminds.ebrains.eu/core/HANDLE"]
+    default_space = "software"
+    type = ["https://openminds.ebrains.eu/core/SWHID"]
     context = {
         "schema": "http://schema.org/",
         "kg": "https://kg.ebrains.eu/api/instances/",
         "vocab": "https://openminds.ebrains.eu/vocab/",
         "terms": "https://openminds.ebrains.eu/controlledTerms/",
         "core": "https://openminds.ebrains.eu/core/"
     }
     fields = [
         Field("identifier", str, "vocab:identifier", multiple=False, required=True,
-              doc="Term or code used to identify the HANDLE."),
+              doc="Term or code used to identify the SWHID."),
 
     ]
     existence_query_fields = ('identifier',)
```

### Comparing `fairgraph-0.8.2/fairgraph/openminds/core/miscellaneous/isbn.py` & `fairgraph-0.9.0/fairgraph/openminds/ephys/entity/channel.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 """
 
 """
 
 # this file was auto-generated
 
 from datetime import date, datetime
-from fairgraph.base_v3 import KGObject, IRI
+from fairgraph.base_v3 import EmbeddedMetadata, IRI
 from fairgraph.fields import Field
 
 
 
 
-class ISBN(KGObject):
+class Channel(EmbeddedMetadata):
     """
 
     """
-    default_space = "dataset"
-    type = ["https://openminds.ebrains.eu/core/ISBN"]
+    type = ["https://openminds.ebrains.eu/ephys/Channel"]
     context = {
         "schema": "http://schema.org/",
         "kg": "https://kg.ebrains.eu/api/instances/",
         "vocab": "https://openminds.ebrains.eu/vocab/",
         "terms": "https://openminds.ebrains.eu/controlledTerms/",
         "core": "https://openminds.ebrains.eu/core/"
     }
     fields = [
-        Field("identifier", str, "vocab:identifier", multiple=False, required=True,
-              doc="Term or code used to identify the ISBN."),
+        Field("internal_identifier", str, "vocab:internalIdentifier", multiple=False, required=True,
+              doc="Term or code that identifies the channel within a particular product."),
+        Field("unit_of_measurement", "openminds.controlledterms.UnitOfMeasurement", "vocab:unitOfMeasurement", multiple=False, required=True,
+              doc="no description available"),
 
     ]
-    existence_query_fields = ('identifier',)
```

### Comparing `fairgraph-0.8.2/fairgraph/openminds/core/miscellaneous/issn.py` & `fairgraph-0.9.0/fairgraph/openminds/core/miscellaneous/url.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,26 +7,28 @@
 from datetime import date, datetime
 from fairgraph.base_v3 import KGObject, IRI
 from fairgraph.fields import Field
 
 
 
 
-class ISSN(KGObject):
+class URL(KGObject):
     """
 
     """
-    default_space = "dataset"
-    type = ["https://openminds.ebrains.eu/core/ISSN"]
+    default_space = "common"
+    type = ["https://openminds.ebrains.eu/core/URL"]
     context = {
         "schema": "http://schema.org/",
         "kg": "https://kg.ebrains.eu/api/instances/",
         "vocab": "https://openminds.ebrains.eu/vocab/",
         "terms": "https://openminds.ebrains.eu/controlledTerms/",
         "core": "https://openminds.ebrains.eu/core/"
     }
     fields = [
-        Field("identifier", str, "vocab:identifier", multiple=False, required=True,
-              doc="Term or code used to identify the ISSN."),
+        Field("url", IRI, "vocab:URL", multiple=False, required=True,
+              doc="no description available"),
+        Field("format", "openminds.core.ContentType", "vocab:format", multiple=False, required=False,
+              doc="Method of digitally organizing and structuring data or information."),
 
     ]
-    existence_query_fields = ('identifier',)
+    existence_query_fields = ('url',)
```

### Comparing `fairgraph-0.8.2/fairgraph/openminds/core/miscellaneous/orcid.py` & `fairgraph-0.9.0/fairgraph/openminds/core/miscellaneous/rrid.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 """
-
+A persistent identifier for a research resource provided by the Resource Identification Initiative.
 """
 
 # this file was auto-generated
 
 from datetime import date, datetime
 from fairgraph.base_v3 import KGObject, IRI
 from fairgraph.fields import Field
 
 
 
 
-class ORCID(KGObject):
+class RRID(KGObject):
     """
-
+    A persistent identifier for a research resource provided by the Resource Identification Initiative.
     """
     default_space = "common"
-    type = ["https://openminds.ebrains.eu/core/ORCID"]
+    type = ["https://openminds.ebrains.eu/core/RRID"]
     context = {
         "schema": "http://schema.org/",
         "kg": "https://kg.ebrains.eu/api/instances/",
         "vocab": "https://openminds.ebrains.eu/vocab/",
         "terms": "https://openminds.ebrains.eu/controlledTerms/",
         "core": "https://openminds.ebrains.eu/core/"
     }
     fields = [
         Field("identifier", str, "vocab:identifier", multiple=False, required=True,
-              doc="Term or code used to identify the ORCID."),
+              doc="Term or code used to identify the RRID."),
 
     ]
     existence_query_fields = ('identifier',)
```

### Comparing `fairgraph-0.8.2/fairgraph/openminds/core/miscellaneous/quantitative_value.py` & `fairgraph-0.9.0/fairgraph/openminds/core/research/string_property.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,36 +1,32 @@
 """
-Structured information on a quantitative value.
+
 """
 
 # this file was auto-generated
 
 from datetime import date, datetime
 from fairgraph.base_v3 import EmbeddedMetadata, IRI
 from fairgraph.fields import Field
 
 
 
 
-class QuantitativeValue(EmbeddedMetadata):
+class StringProperty(EmbeddedMetadata):
     """
-    Structured information on a quantitative value.
+
     """
-    type = ["https://openminds.ebrains.eu/core/QuantitativeValue"]
+    type = ["https://openminds.ebrains.eu/core/StringProperty"]
     context = {
         "schema": "http://schema.org/",
         "kg": "https://kg.ebrains.eu/api/instances/",
         "vocab": "https://openminds.ebrains.eu/vocab/",
         "terms": "https://openminds.ebrains.eu/controlledTerms/",
         "core": "https://openminds.ebrains.eu/core/"
     }
     fields = [
-        Field("type_of_uncertainty", "openminds.controlledterms.TypeOfUncertainty", "vocab:typeOfUncertainty", multiple=False, required=False,
-              doc="Distinct technique used to quantify the uncertainty of a measurement."),
-        Field("uncertainties", float, "vocab:uncertainty", multiple=True, required=False,
-              doc="Quantitative value range defining the uncertainty of a measurement."),
-        Field("unit", "openminds.controlledterms.UnitOfMeasurement", "vocab:unit", multiple=False, required=False,
-              doc="Determinate quantity adopted as a standard of measurement."),
-        Field("value", float, "vocab:value", multiple=False, required=True,
+        Field("name", str, "vocab:name", multiple=False, required=True,
+              doc="Word or phrase that constitutes the distinctive designation of the string property."),
+        Field("value", str, "vocab:value", multiple=False, required=True,
               doc="Entry for a property."),
 
     ]
```

### Comparing `fairgraph-0.8.2/fairgraph/openminds/core/miscellaneous/quantitative_value_array.py` & `fairgraph-0.9.0/fairgraph/openminds/core/products/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -7,34 +7,36 @@
 from datetime import date, datetime
 from fairgraph.base_v3 import KGObject, IRI
 from fairgraph.fields import Field
 
 
 
 
-class QuantitativeValueArray(KGObject):
+class Setup(KGObject):
     """
 
     """
     default_space = "dataset"
-    type = ["https://openminds.ebrains.eu/core/QuantitativeValueArray"]
+    type = ["https://openminds.ebrains.eu/core/Setup"]
     context = {
         "schema": "http://schema.org/",
         "kg": "https://kg.ebrains.eu/api/instances/",
         "vocab": "https://openminds.ebrains.eu/vocab/",
         "terms": "https://openminds.ebrains.eu/controlledTerms/",
         "core": "https://openminds.ebrains.eu/core/"
     }
     fields = [
-        Field("negative_uncertainties", float, "vocab:negativeUncertainties", multiple=True, required=False,
+        Field("name", str, "vocab:name", multiple=False, required=True,
+              doc="Word or phrase that constitutes the distinctive designation of the setup."),
+        Field("components", ["openminds.core.Setup", "openminds.core.SoftwareVersion", "openminds.ephys.Electrode", "openminds.ephys.ElectrodeArray", "openminds.ephys.Pipette", "openminds.specimenprep.SlicingDevice"], "vocab:components", multiple=True, required=True,
               doc="no description available"),
-        Field("positive_uncertainties", float, "vocab:positiveUncertainties", multiple=True, required=False,
+        Field("description", str, "vocab:description", multiple=False, required=True,
+              doc="Longer statement or account giving the characteristics of the setup."),
+        Field("location", str, "vocab:location", multiple=False, required=False,
               doc="no description available"),
-        Field("type_of_uncertainty", "openminds.controlledterms.TypeOfUncertainty", "vocab:typeOfUncertainty", multiple=False, required=False,
-              doc="Distinct technique used to quantify the uncertainty of a measurement."),
-        Field("unit", "openminds.controlledterms.UnitOfMeasurement", "vocab:unit", multiple=False, required=False,
-              doc="Determinate quantity adopted as a standard of measurement."),
-        Field("values", float, "vocab:values", multiple=True, required=True,
+        Field("manufacturers", ["openminds.core.Consortium", "openminds.core.Organization", "openminds.core.Person"], "vocab:manufacturer", multiple=True, required=False,
+              doc="no description available"),
+        Field("setup_types", "openminds.controlledterms.SetupType", "vocab:setupType", multiple=True, required=False,
               doc="no description available"),
 
     ]
-    existence_query_fields = ('values',)
+    existence_query_fields = ('name', 'components', 'description')
```

### Comparing `fairgraph-0.8.2/fairgraph/openminds/core/miscellaneous/quantitative_value_range.py` & `fairgraph-0.9.0/fairgraph/openminds/sands/miscellaneous/anatomical_target_position.py`

 * *Files 22% similar despite different names*

```diff
@@ -7,30 +7,32 @@
 from datetime import date, datetime
 from fairgraph.base_v3 import EmbeddedMetadata, IRI
 from fairgraph.fields import Field
 
 
 
 
-class QuantitativeValueRange(EmbeddedMetadata):
+class AnatomicalTargetPosition(EmbeddedMetadata):
     """
 
     """
-    type = ["https://openminds.ebrains.eu/core/QuantitativeValueRange"]
+    type = ["https://openminds.ebrains.eu/sands/AnatomicalTargetPosition"]
     context = {
         "schema": "http://schema.org/",
         "kg": "https://kg.ebrains.eu/api/instances/",
         "vocab": "https://openminds.ebrains.eu/vocab/",
         "terms": "https://openminds.ebrains.eu/controlledTerms/",
         "core": "https://openminds.ebrains.eu/core/"
     }
     fields = [
-        Field("max_value", float, "vocab:maxValue", multiple=False, required=True,
-              doc="Greatest quantity attained or allowed."),
-        Field("max_value_unit", "openminds.controlledterms.UnitOfMeasurement", "vocab:maxValueUnit", multiple=False, required=False,
+        Field("lookup_label", str, "vocab:lookupLabel", multiple=False, required=False,
               doc="no description available"),
-        Field("min_value", float, "vocab:minValue", multiple=False, required=True,
-              doc="Smallest quantity attained or allowed."),
-        Field("min_value_unit", "openminds.controlledterms.UnitOfMeasurement", "vocab:minValueUnit", multiple=False, required=False,
+        Field("additional_remarks", str, "vocab:additionalRemarks", multiple=False, required=False,
+              doc="Mention of what deserves additional attention or notice."),
+        Field("anatomical_targets", ["openminds.controlledterms.CellType", "openminds.controlledterms.UBERONParcellation", "openminds.sands.CustomAnatomicalEntity", "openminds.sands.ParcellationEntity", "openminds.sands.ParcellationEntityVersion"], "vocab:anatomicalTarget", multiple=True, required=True,
+              doc="no description available"),
+        Field("coordinates", "openminds.sands.CoordinatePoint", "vocab:coordinates", multiple=False, required=False,
+              doc="Pair or triplet of numbers defining a location in a given coordinate space."),
+        Field("target_identification_type", "openminds.controlledterms.AnatomicalIdentificationType", "vocab:targetIdentificationType", multiple=False, required=True,
               doc="no description available"),
 
     ]
```

### Comparing `fairgraph-0.8.2/fairgraph/openminds/core/miscellaneous/rorid.py` & `fairgraph-0.9.0/fairgraph/openminds/publications/publication_issue.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,26 +7,28 @@
 from datetime import date, datetime
 from fairgraph.base_v3 import KGObject, IRI
 from fairgraph.fields import Field
 
 
 
 
-class RORID(KGObject):
+class PublicationIssue(KGObject):
     """
 
     """
-    default_space = "common"
-    type = ["https://openminds.ebrains.eu/core/RORID"]
+    default_space = "livepapers"
+    type = ["https://openminds.ebrains.eu/publications/PublicationIssue"]
     context = {
         "schema": "http://schema.org/",
         "kg": "https://kg.ebrains.eu/api/instances/",
         "vocab": "https://openminds.ebrains.eu/vocab/",
         "terms": "https://openminds.ebrains.eu/controlledTerms/",
         "core": "https://openminds.ebrains.eu/core/"
     }
     fields = [
-        Field("identifier", str, "vocab:identifier", multiple=False, required=True,
-              doc="Term or code used to identify the RORID."),
+        Field("is_part_of", "openminds.publications.PublicationVolume", "vocab:isPartOf", multiple=False, required=True,
+              doc="Reference to the ensemble of multiple things or beings."),
+        Field("issue_number", str, "vocab:issueNumber", multiple=False, required=True,
+              doc="no description available"),
 
     ]
-    existence_query_fields = ('identifier',)
+    existence_query_fields = ('is_part_of', 'issue_number')
```

### Comparing `fairgraph-0.8.2/fairgraph/openminds/core/miscellaneous/rrid.py` & `fairgraph-0.9.0/fairgraph/openminds/publications/publication_volume.py`

 * *Files 13% similar despite different names*

```diff
@@ -7,26 +7,28 @@
 from datetime import date, datetime
 from fairgraph.base_v3 import KGObject, IRI
 from fairgraph.fields import Field
 
 
 
 
-class RRID(KGObject):
+class PublicationVolume(KGObject):
     """
 
     """
-    default_space = "common"
-    type = ["https://openminds.ebrains.eu/core/RRID"]
+    default_space = "livepapers"
+    type = ["https://openminds.ebrains.eu/publications/PublicationVolume"]
     context = {
         "schema": "http://schema.org/",
         "kg": "https://kg.ebrains.eu/api/instances/",
         "vocab": "https://openminds.ebrains.eu/vocab/",
         "terms": "https://openminds.ebrains.eu/controlledTerms/",
         "core": "https://openminds.ebrains.eu/core/"
     }
     fields = [
-        Field("identifier", str, "vocab:identifier", multiple=False, required=True,
-              doc="Term or code used to identify the RRID."),
+        Field("is_part_of", "openminds.publications.Periodical", "vocab:isPartOf", multiple=False, required=True,
+              doc="Reference to the ensemble of multiple things or beings."),
+        Field("volume_number", str, "vocab:volumeNumber", multiple=False, required=True,
+              doc="no description available"),
 
     ]
-    existence_query_fields = ('identifier',)
+    existence_query_fields = ('is_part_of', 'volume_number')
```

### Comparing `fairgraph-0.8.2/fairgraph/openminds/core/miscellaneous/stock_number.py` & `fairgraph-0.9.0/fairgraph/openminds/sands/mathematicalShapes/circle.py`

 * *Files 18% similar despite different names*

```diff
@@ -7,26 +7,24 @@
 from datetime import date, datetime
 from fairgraph.base_v3 import EmbeddedMetadata, IRI
 from fairgraph.fields import Field
 
 
 
 
-class StockNumber(EmbeddedMetadata):
+class Circle(EmbeddedMetadata):
     """
 
     """
-    type = ["https://openminds.ebrains.eu/core/StockNumber"]
+    type = ["https://openminds.ebrains.eu/sands/Circle"]
     context = {
         "schema": "http://schema.org/",
         "kg": "https://kg.ebrains.eu/api/instances/",
         "vocab": "https://openminds.ebrains.eu/vocab/",
         "terms": "https://openminds.ebrains.eu/controlledTerms/",
         "core": "https://openminds.ebrains.eu/core/"
     }
     fields = [
-        Field("identifier", str, "vocab:identifier", multiple=False, required=True,
-              doc="Term or code used to identify the stock number."),
-        Field("vendor", "openminds.core.Organization", "vocab:vendor", multiple=False, required=True,
+        Field("radius", "openminds.core.QuantitativeValue", "vocab:radius", multiple=False, required=True,
               doc="no description available"),
 
     ]
```

### Comparing `fairgraph-0.8.2/fairgraph/openminds/core/miscellaneous/swhid.py` & `fairgraph-0.9.0/fairgraph/openminds/core/research/property_value_list.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,32 +1,34 @@
 """
-
+An identifiable list of property-value pairs
 """
 
 # this file was auto-generated
 
 from datetime import date, datetime
 from fairgraph.base_v3 import KGObject, IRI
 from fairgraph.fields import Field
 
 
 
 
-class SWHID(KGObject):
+class PropertyValueList(KGObject):
     """
-
+    An identifiable list of property-value pairs
     """
-    default_space = "software"
-    type = ["https://openminds.ebrains.eu/core/SWHID"]
+    default_space = "dataset"
+    type = ["https://openminds.ebrains.eu/core/PropertyValueList"]
     context = {
         "schema": "http://schema.org/",
         "kg": "https://kg.ebrains.eu/api/instances/",
         "vocab": "https://openminds.ebrains.eu/vocab/",
         "terms": "https://openminds.ebrains.eu/controlledTerms/",
         "core": "https://openminds.ebrains.eu/core/"
     }
     fields = [
-        Field("identifier", str, "vocab:identifier", multiple=False, required=True,
-              doc="Term or code used to identify the SWHID."),
+        Field("lookup_label", str, "vocab:lookupLabel", multiple=False, required=False,
+              doc="no description available"),
+        Field("property_value_pairs", ["openminds.core.NumericalProperty", "openminds.core.StringProperty"], "vocab:propertyValuePair", multiple=True, required=True,
+              doc="no description available"),
 
     ]
-    existence_query_fields = ('identifier',)
+    existence_query_fields = ('lookup_label',)
```

### Comparing `fairgraph-0.8.2/fairgraph/openminds/core/miscellaneous/url.py` & `fairgraph-0.9.0/fairgraph/openminds/sands/mathematicalShapes/ellipse.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 """
 
 """
 
 # this file was auto-generated
 
 from datetime import date, datetime
-from fairgraph.base_v3 import KGObject, IRI
+from fairgraph.base_v3 import EmbeddedMetadata, IRI
 from fairgraph.fields import Field
 
 
 
 
-class URL(KGObject):
+class Ellipse(EmbeddedMetadata):
     """
 
     """
-    default_space = "common"
-    type = ["https://openminds.ebrains.eu/core/URL"]
+    type = ["https://openminds.ebrains.eu/sands/Ellipse"]
     context = {
         "schema": "http://schema.org/",
         "kg": "https://kg.ebrains.eu/api/instances/",
         "vocab": "https://openminds.ebrains.eu/vocab/",
         "terms": "https://openminds.ebrains.eu/controlledTerms/",
         "core": "https://openminds.ebrains.eu/core/"
     }
     fields = [
-        Field("url", IRI, "vocab:URL", multiple=False, required=True,
+        Field("semi_major_axis", "openminds.core.QuantitativeValue", "vocab:semiMajorAxis", multiple=False, required=True,
+              doc="no description available"),
+        Field("semi_minor_axis", "openminds.core.QuantitativeValue", "vocab:semiMinorAxis", multiple=False, required=True,
               doc="no description available"),
 
     ]
-    existence_query_fields = ('url',)
```

### Comparing `fairgraph-0.8.2/fairgraph/openminds/core/products/dataset_version.py` & `fairgraph-0.9.0/fairgraph/openminds/core/products/software_version.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,114 +1,102 @@
 """
-Structured information on data originating from human/animal studies or simulations (version level).
+
 """
 
 # this file was auto-generated
 
 from datetime import date, datetime
 from fairgraph.base_v3 import KGObject, IRI
 from fairgraph.fields import Field
-
-from urllib.request import urlretrieve
-from pathlib import Path
-from fairgraph.utility import accepted_terms_of_use
+from fairgraph.errors import ResolutionFailure
+from .software import Software
 
 
-class DatasetVersion(KGObject):
+class SoftwareVersion(KGObject):
     """
-    Structured information on data originating from human/animal studies or simulations (version level).
+
     """
-    default_space = "dataset"
-    type = ["https://openminds.ebrains.eu/core/DatasetVersion"]
+    default_space = "software"
+    type = ["https://openminds.ebrains.eu/core/SoftwareVersion"]
     context = {
         "schema": "http://schema.org/",
         "kg": "https://kg.ebrains.eu/api/instances/",
         "vocab": "https://openminds.ebrains.eu/vocab/",
         "terms": "https://openminds.ebrains.eu/controlledTerms/",
         "core": "https://openminds.ebrains.eu/core/"
     }
     fields = [
         Field("name", str, "vocab:fullName", multiple=False, required=False,
-              doc="Whole, non-abbreviated name of the dataset version."),
+              doc="Whole, non-abbreviated name of the software version."),
         Field("alias", str, "vocab:shortName", multiple=False, required=True,
-              doc="Shortened or fully abbreviated name of the dataset version."),
+              doc="Shortened or fully abbreviated name of the software version."),
         Field("accessibility", "openminds.controlledterms.ProductAccessibility", "vocab:accessibility", multiple=False, required=True,
-              doc="Level to which something is accessible to the dataset version."),
-        Field("authors", ["openminds.core.Organization", "openminds.core.Person"], "vocab:author", multiple=True, required=False,
-              doc="Creator of a literary or creative work, as well as a dataset publication."),
-        Field("behavioral_protocols", "openminds.core.BehavioralProtocol", "vocab:behavioralProtocol", multiple=True, required=False,
-              doc="no description available"),
+              doc="Level to which something is accessible to the software version."),
+        Field("application_categories", "openminds.controlledterms.SoftwareApplicationCategory", "vocab:applicationCategory", multiple=True, required=True,
+              doc="Distinct class that groups software programs which perform a similar task or set of tasks."),
         Field("copyright", "openminds.core.Copyright", "vocab:copyright", multiple=False, required=False,
               doc="Exclusive and assignable legal right of an originator to reproduce, publish, sell, or distribute the matter and form of a creative work for a defined time period."),
-        Field("custodians", ["openminds.core.Organization", "openminds.core.Person"], "vocab:custodian", multiple=True, required=False,
+        Field("custodians", ["openminds.core.Consortium", "openminds.core.Organization", "openminds.core.Person"], "vocab:custodian", multiple=True, required=False,
               doc="The 'custodian' is a legal person who is responsible for the content and quality of the data, metadata, and/or code of a research product."),
-        Field("data_types", "openminds.controlledterms.SemanticDataType", "vocab:dataType", multiple=True, required=True,
-              doc="no description available"),
         Field("description", str, "vocab:description", multiple=False, required=False,
-              doc="Longer statement or account giving the characteristics of the dataset version."),
-        Field("digital_identifier", "openminds.core.DOI", "vocab:digitalIdentifier", multiple=False, required=True,
+              doc="Longer statement or account giving the characteristics of the software version."),
+        Field("developers", ["openminds.core.Consortium", "openminds.core.Organization", "openminds.core.Person"], "vocab:developer", multiple=True, required=False,
+              doc="Legal person that creates or improves products or services (e.g., software, applications, etc.)."),
+        Field("devices", "openminds.controlledterms.OperatingDevice", "vocab:device", multiple=True, required=True,
+              doc="Piece of equipment or mechanism (hardware) designed to serve a special purpose or perform a special function."),
+        Field("digital_identifier", ["openminds.core.DOI", "openminds.core.SWHID"], "vocab:digitalIdentifier", multiple=False, required=False,
               doc="Digital handle to identify objects or legal persons."),
-        Field("ethics_assessment", "openminds.controlledterms.EthicsAssessment", "vocab:ethicsAssessment", multiple=False, required=True,
-              doc="Judgment about the applied principles of conduct governing an individual or a group."),
-        Field("experimental_approaches", "openminds.controlledterms.ExperimentalApproach", "vocab:experimentalApproach", multiple=True, required=True,
-              doc="no description available"),
+        Field("features", "openminds.controlledterms.SoftwareFeature", "vocab:feature", multiple=True, required=True,
+              doc="Structure, form, or appearance that characterizes the software version."),
         Field("full_documentation", ["openminds.core.DOI", "openminds.core.File", "openminds.core.URL"], "vocab:fullDocumentation", multiple=False, required=True,
               doc="Non-abridged instructions, comments, and information for using a particular product."),
         Field("funding", "openminds.core.Funding", "vocab:funding", multiple=True, required=False,
               doc="Money provided by a legal person for a particular purpose."),
         Field("homepage", "openminds.core.URL", "vocab:homepage", multiple=False, required=False,
-              doc="Main website of the dataset version."),
+              doc="Main website of the software version."),
         Field("how_to_cite", str, "vocab:howToCite", multiple=False, required=False,
               doc="Preferred format for citing a particular object or legal person."),
-        Field("input_data", ["openminds.core.DOI", "openminds.core.File", "openminds.core.FileBundle", "openminds.core.URL", "openminds.sands.BrainAtlasVersion", "openminds.sands.CommonCoordinateSpace"], "vocab:inputData", multiple=True, required=False,
-              doc="Data that is put into a process or machine."),
-        Field("is_alternative_version_of", "openminds.core.DatasetVersion", "vocab:isAlternativeVersionOf", multiple=True, required=False,
+        Field("input_formats", "openminds.core.ContentType", "vocab:inputFormat", multiple=True, required=False,
+              doc="Format of data that is put into a process or machine."),
+        Field("is_alternative_version_of", "openminds.core.SoftwareVersion", "vocab:isAlternativeVersionOf", multiple=True, required=False,
               doc="Reference to an original form where the essence was preserved, but presented in an alternative form."),
-        Field("is_new_version_of", "openminds.core.DatasetVersion", "vocab:isNewVersionOf", multiple=False, required=False,
+        Field("is_new_version_of", "openminds.core.SoftwareVersion", "vocab:isNewVersionOf", multiple=False, required=False,
               doc="Reference to a previous (potentially outdated) particular form of something."),
-        Field("keywords", ["openminds.controlledterms.ActionStatusType", "openminds.controlledterms.AgeCategory", "openminds.controlledterms.AnatomicalAxesOrientation", "openminds.controlledterms.AnatomicalPlane", "openminds.controlledterms.AnnotationType", "openminds.controlledterms.AtlasType", "openminds.controlledterms.BiologicalOrder", "openminds.controlledterms.BiologicalSex", "openminds.controlledterms.BreedingType", "openminds.controlledterms.CellCultureType", "openminds.controlledterms.CellType", "openminds.controlledterms.ChemicalMixtureType", "openminds.controlledterms.ContributionType", "openminds.controlledterms.CranialWindowType", "openminds.controlledterms.CriteriaQualityType", "openminds.controlledterms.DataType", "openminds.controlledterms.DeviceType", "openminds.controlledterms.DifferenceMeasure", "openminds.controlledterms.Disease", "openminds.controlledterms.DiseaseModel", "openminds.controlledterms.EthicsAssessment", "openminds.controlledterms.ExperimentalApproach", "openminds.controlledterms.FileBundleGrouping", "openminds.controlledterms.FileRepositoryType", "openminds.controlledterms.FileUsageRole", "openminds.controlledterms.GeneticStrainType", "openminds.controlledterms.Handedness", "openminds.controlledterms.Language", "openminds.controlledterms.Laterality", "openminds.controlledterms.MeasuredQuantity", "openminds.controlledterms.MetaDataModelType", "openminds.controlledterms.ModelAbstractionLevel", "openminds.controlledterms.ModelScope", "openminds.controlledterms.MolecularEntity", "openminds.controlledterms.OperatingDevice", "openminds.controlledterms.OperatingSystem", "openminds.controlledterms.Organ", "openminds.controlledterms.PatchClampVariation", "openminds.controlledterms.PreparationType", "openminds.controlledterms.ProductAccessibility", "openminds.controlledterms.ProgrammingLanguage", "openminds.controlledterms.QualitativeOverlap", "openminds.controlledterms.SemanticDataType", "openminds.controlledterms.Service", "openminds.controlledterms.SetupType", "openminds.controlledterms.SoftwareApplicationCategory", "openminds.controlledterms.SoftwareFeature", "openminds.controlledterms.Species", "openminds.controlledterms.StimulationApproach", "openminds.controlledterms.StimulusType", "openminds.controlledterms.SubcellularEntity", "openminds.controlledterms.SubjectAttribute", "openminds.controlledterms.Technique", "openminds.controlledterms.TermSuggestion", "openminds.controlledterms.Terminology", "openminds.controlledterms.TissueSampleAttribute", "openminds.controlledterms.TissueSampleType", "openminds.controlledterms.TypeOfUncertainty", "openminds.controlledterms.UBERONParcellation", "openminds.controlledterms.UnitOfMeasurement"], "vocab:keyword", multiple=True, required=False,
-              doc="Significant word or concept that are representative of the dataset version."),
-        Field("license", "openminds.core.License", "vocab:license", multiple=False, required=True,
+        Field("keywords", ["openminds.controlledterms.ActionStatusType", "openminds.controlledterms.AgeCategory", "openminds.controlledterms.AnatomicalAxesOrientation", "openminds.controlledterms.AnatomicalPlane", "openminds.controlledterms.AnnotationType", "openminds.controlledterms.AtlasType", "openminds.controlledterms.AuditoryStimulusType", "openminds.controlledterms.BiologicalOrder", "openminds.controlledterms.BiologicalSex", "openminds.controlledterms.BreedingType", "openminds.controlledterms.CellCultureType", "openminds.controlledterms.CellType", "openminds.controlledterms.ChemicalMixtureType", "openminds.controlledterms.ContributionType", "openminds.controlledterms.CranialWindowConstructionType", "openminds.controlledterms.CranialWindowReinforcementType", "openminds.controlledterms.CriteriaQualityType", "openminds.controlledterms.DataType", "openminds.controlledterms.DeviceType", "openminds.controlledterms.DifferenceMeasure", "openminds.controlledterms.Disease", "openminds.controlledterms.DiseaseModel", "openminds.controlledterms.EducationalLevel", "openminds.controlledterms.ElectricalStimulusType", "openminds.controlledterms.EthicsAssessment", "openminds.controlledterms.ExperimentalApproach", "openminds.controlledterms.FileBundleGrouping", "openminds.controlledterms.FileRepositoryType", "openminds.controlledterms.FileUsageRole", "openminds.controlledterms.GeneticStrainType", "openminds.controlledterms.GustatoryStimulusType", "openminds.controlledterms.Handedness", "openminds.controlledterms.Language", "openminds.controlledterms.Laterality", "openminds.controlledterms.LearningResourceType", "openminds.controlledterms.MeasuredQuantity", "openminds.controlledterms.MetaDataModelType", "openminds.controlledterms.ModelAbstractionLevel", "openminds.controlledterms.ModelScope", "openminds.controlledterms.MolecularEntity", "openminds.controlledterms.OlfactoryStimulusType", "openminds.controlledterms.OperatingDevice", "openminds.controlledterms.OperatingSystem", "openminds.controlledterms.OpticalStimulusType", "openminds.controlledterms.Organ", "openminds.controlledterms.PatchClampVariation", "openminds.controlledterms.PreparationType", "openminds.controlledterms.ProductAccessibility", "openminds.controlledterms.ProgrammingLanguage", "openminds.controlledterms.QualitativeOverlap", "openminds.controlledterms.SemanticDataType", "openminds.controlledterms.Service", "openminds.controlledterms.SetupType", "openminds.controlledterms.SoftwareApplicationCategory", "openminds.controlledterms.SoftwareFeature", "openminds.controlledterms.Species", "openminds.controlledterms.StimulationApproach", "openminds.controlledterms.StimulationTechnique", "openminds.controlledterms.SubcellularEntity", "openminds.controlledterms.SubjectAttribute", "openminds.controlledterms.TactileStimulusType", "openminds.controlledterms.Technique", "openminds.controlledterms.TermSuggestion", "openminds.controlledterms.Terminology", "openminds.controlledterms.TissueSampleAttribute", "openminds.controlledterms.TissueSampleType", "openminds.controlledterms.TypeOfUncertainty", "openminds.controlledterms.UBERONParcellation", "openminds.controlledterms.UnitOfMeasurement", "openminds.controlledterms.VisualStimulusType"], "vocab:keyword", multiple=True, required=False,
+              doc="Significant word or concept that are representative of the software version."),
+        Field("languages", "openminds.controlledterms.Language", "vocab:language", multiple=True, required=True,
+              doc="System of communication (words, their pronunciation, and the methods of combining them) used and understood by a particular community."),
+        Field("licenses", "openminds.core.License", "vocab:license", multiple=True, required=True,
               doc="Grant by a party to another party as an element of an agreement between those parties that permits to do, use, or own something."),
+        Field("operating_systems", "openminds.controlledterms.OperatingSystem", "vocab:operatingSystem", multiple=True, required=True,
+              doc="Software that controls the operation of a computer and directs the processing of programs."),
         Field("other_contributions", "openminds.core.Contribution", "vocab:otherContribution", multiple=True, required=False,
               doc="Giving or supplying of something (such as money or time) as a part or share other than what is covered elsewhere."),
-        Field("preparation_designs", "openminds.controlledterms.PreparationType", "vocab:preparationDesign", multiple=True, required=False,
-              doc="no description available"),
+        Field("output_formats", "openminds.core.ContentType", "vocab:outputFormat", multiple=True, required=False,
+              doc="Format of data that comes out of, is delivered or produced by a process or machine."),
+        Field("programming_languages", "openminds.controlledterms.ProgrammingLanguage", "vocab:programmingLanguage", multiple=True, required=True,
+              doc="Distinct set of instructions for computer programs in order to produce various kinds of output."),
         Field("related_publications", ["openminds.core.DOI", "openminds.core.HANDLE", "openminds.core.ISBN"], "vocab:relatedPublication", multiple=True, required=False,
               doc="Reference to something that was made available for the general public to see or buy."),
         Field("release_date", date, "vocab:releaseDate", multiple=False, required=True,
               doc="Fixed date on which a product is due to become or was made available for the general public to see or buy"),
         Field("repository", "openminds.core.FileRepository", "vocab:repository", multiple=False, required=False,
               doc="Place, room, or container where something is deposited or stored."),
-        Field("studied_specimens", ["openminds.core.Subject", "openminds.core.SubjectGroup", "openminds.core.TissueSample", "openminds.core.TissueSampleCollection"], "vocab:studiedSpecimen", multiple=True, required=False,
-              doc="no description available"),
-        Field("study_targets", ["openminds.controlledterms.BiologicalOrder", "openminds.controlledterms.BiologicalSex", "openminds.controlledterms.BreedingType", "openminds.controlledterms.CellCultureType", "openminds.controlledterms.CellType", "openminds.controlledterms.Disease", "openminds.controlledterms.DiseaseModel", "openminds.controlledterms.GeneticStrainType", "openminds.controlledterms.Handedness", "openminds.controlledterms.MolecularEntity", "openminds.controlledterms.Organ", "openminds.controlledterms.Species", "openminds.controlledterms.SubcellularEntity", "openminds.controlledterms.TermSuggestion", "openminds.controlledterms.UBERONParcellation", "openminds.sands.CustomAnatomicalEntity", "openminds.sands.ParcellationEntity", "openminds.sands.ParcellationEntityVersion"], "vocab:studyTarget", multiple=True, required=False,
-              doc="Structure or function that was targeted within a study."),
+        Field("requirements", str, "vocab:requirement", multiple=True, required=False,
+              doc="Something essential to the existence, occurrence or function of something else."),
         Field("support_channels", str, "vocab:supportChannel", multiple=True, required=False,
               doc="Way of communication used to interact with users or customers."),
-        Field("techniques", "openminds.controlledterms.Technique", "vocab:technique", multiple=True, required=True,
-              doc="Method of accomplishing a desired aim."),
         Field("version_identifier", str, "vocab:versionIdentifier", multiple=False, required=True,
               doc="Term or code used to identify the version of something."),
         Field("version_innovation", str, "vocab:versionInnovation", multiple=False, required=True,
               doc="Documentation on what changed in comparison to a previously published form of something."),
 
     ]
     existence_query_fields = ('alias', 'version_identifier')
 
-
-    def download(self, local_path, client, accept_terms_of_use=False):
-        if accepted_terms_of_use(client, accept_terms_of_use=accept_terms_of_use):
-            repo = self.repository.resolve(client)
-            if (repo.iri.value.startswith("https://object.cscs.ch/v1/AUTH")
-                or repo.iri.value.startswith("https://data-proxy.ebrains.eu/api/v1/public")
-            ):
-                zip_archive_url = f"https://data.kg.ebrains.eu/zip?container={repo.iri.value}"
-            else:
-                raise NotImplementedError("Download not yet implemented for this repository type")
-            if local_path.endswith(".zip"):
-                local_filename = Path(local_path)
-            else:
-                local_filename = Path(local_path) / (zip_archive_url.split("/")[-1] + ".zip")
-            local_filename.parent.mkdir(parents=True, exist_ok=True)
-            local_filename, headers = urlretrieve(zip_archive_url, local_filename)
-            return local_filename
+    def is_version_of(self, client):
+        parents = Software.list(client, scope=self.scope, space=self.space, versions=self)
+        if len(parents) == 0:
+            raise ResolutionFailure("Unable to find parent")
+        else:
+            assert len(parents) == 1
+            return parents[0]
```

### Comparing `fairgraph-0.8.2/fairgraph/openminds/core/products/meta_data_model.py` & `fairgraph-0.9.0/fairgraph/openminds/core/actors/organization.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,48 +1,42 @@
 """
-
+Structured information on an organization.
 """
 
 # this file was auto-generated
 
 from datetime import date, datetime
 from fairgraph.base_v3 import KGObject, IRI
 from fairgraph.fields import Field
 
 
 
 
-class MetaDataModel(KGObject):
+class Organization(KGObject):
     """
-
+    Structured information on an organization.
     """
-    default_space = "metadatamodel"
-    type = ["https://openminds.ebrains.eu/core/MetaDataModel"]
+    default_space = "common"
+    type = ["https://openminds.ebrains.eu/core/Organization"]
     context = {
         "schema": "http://schema.org/",
         "kg": "https://kg.ebrains.eu/api/instances/",
         "vocab": "https://openminds.ebrains.eu/vocab/",
         "terms": "https://openminds.ebrains.eu/controlledTerms/",
         "core": "https://openminds.ebrains.eu/core/"
     }
     fields = [
         Field("name", str, "vocab:fullName", multiple=False, required=True,
-              doc="Whole, non-abbreviated name of the meta data model."),
-        Field("alias", str, "vocab:shortName", multiple=False, required=True,
-              doc="Shortened or fully abbreviated name of the meta data model."),
-        Field("custodians", ["openminds.core.Organization", "openminds.core.Person"], "vocab:custodian", multiple=True, required=False,
-              doc="The 'custodian' is a legal person who is responsible for the content and quality of the data, metadata, and/or code of a research product."),
-        Field("description", str, "vocab:description", multiple=False, required=True,
-              doc="Longer statement or account giving the characteristics of the meta data model."),
-        Field("developers", ["openminds.core.Organization", "openminds.core.Person"], "vocab:developer", multiple=True, required=True,
-              doc="Legal person that creates or improves products or services (e.g., software, applications, etc.)."),
-        Field("digital_identifier", ["openminds.core.DOI", "openminds.core.SWHID"], "vocab:digitalIdentifier", multiple=False, required=False,
+              doc="Whole, non-abbreviated name of the organization."),
+        Field("alias", str, "vocab:shortName", multiple=False, required=False,
+              doc="Shortened or fully abbreviated name of the organization."),
+        Field("affiliations", "openminds.core.Affiliation", "vocab:affiliation", multiple=True, required=False,
+              doc="Declaration of a person being closely associated to an organization."),
+        Field("digital_identifiers", ["openminds.core.GRIDID", "openminds.core.RORID", "openminds.core.RRID"], "vocab:digitalIdentifier", multiple=True, required=False,
               doc="Digital handle to identify objects or legal persons."),
-        Field("versions", "openminds.core.MetaDataModelVersion", "vocab:hasVersion", multiple=True, required=True,
-              doc="Reference to variants of an original."),
+        Field("has_parents", "openminds.core.Organization", "vocab:hasParent", multiple=True, required=False,
+              doc="Reference to a parent object or legal person."),
         Field("homepage", "openminds.core.URL", "vocab:homepage", multiple=False, required=False,
-              doc="Main website of the meta data model."),
-        Field("how_to_cite", str, "vocab:howToCite", multiple=False, required=False,
-              doc="Preferred format for citing a particular object or legal person."),
+              doc="Main website of the organization."),
 
     ]
-    existence_query_fields = ('alias',)
+    existence_query_fields = ('name',)
```

### Comparing `fairgraph-0.8.2/fairgraph/openminds/core/products/meta_data_model_version.py` & `fairgraph-0.9.0/fairgraph/openminds/core/products/model_version.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,82 +1,92 @@
 """
-
+Structured information on a computational model (version level).
 """
 
 # this file was auto-generated
 
 from datetime import date, datetime
 from fairgraph.base_v3 import KGObject, IRI
 from fairgraph.fields import Field
 
+from fairgraph.errors import ResolutionFailure
+from .model import Model
 
 
-
-class MetaDataModelVersion(KGObject):
+class ModelVersion(KGObject):
     """
-
+    Structured information on a computational model (version level).
     """
-    default_space = "metadatamodel"
-    type = ["https://openminds.ebrains.eu/core/MetaDataModelVersion"]
+    default_space = "model"
+    type = ["https://openminds.ebrains.eu/core/ModelVersion"]
     context = {
         "schema": "http://schema.org/",
         "kg": "https://kg.ebrains.eu/api/instances/",
         "vocab": "https://openminds.ebrains.eu/vocab/",
         "terms": "https://openminds.ebrains.eu/controlledTerms/",
         "core": "https://openminds.ebrains.eu/core/"
     }
     fields = [
         Field("name", str, "vocab:fullName", multiple=False, required=False,
-              doc="Whole, non-abbreviated name of the meta data model version."),
+              doc="Whole, non-abbreviated name of the model version."),
         Field("alias", str, "vocab:shortName", multiple=False, required=True,
-              doc="Shortened or fully abbreviated name of the meta data model version."),
+              doc="Shortened or fully abbreviated name of the model version."),
         Field("accessibility", "openminds.controlledterms.ProductAccessibility", "vocab:accessibility", multiple=False, required=True,
-              doc="Level to which something is accessible to the meta data model version."),
+              doc="Level to which something is accessible to the model version."),
         Field("copyright", "openminds.core.Copyright", "vocab:copyright", multiple=False, required=False,
               doc="Exclusive and assignable legal right of an originator to reproduce, publish, sell, or distribute the matter and form of a creative work for a defined time period."),
-        Field("custodians", ["openminds.core.Organization", "openminds.core.Person"], "vocab:custodian", multiple=True, required=False,
+        Field("custodians", ["openminds.core.Consortium", "openminds.core.Organization", "openminds.core.Person"], "vocab:custodian", multiple=True, required=False,
               doc="The 'custodian' is a legal person who is responsible for the content and quality of the data, metadata, and/or code of a research product."),
         Field("description", str, "vocab:description", multiple=False, required=False,
-              doc="Longer statement or account giving the characteristics of the meta data model version."),
-        Field("developers", ["openminds.core.Organization", "openminds.core.Person"], "vocab:developer", multiple=True, required=False,
+              doc="Longer statement or account giving the characteristics of the model version."),
+        Field("developers", ["openminds.core.Consortium", "openminds.core.Organization", "openminds.core.Person"], "vocab:developer", multiple=True, required=False,
               doc="Legal person that creates or improves products or services (e.g., software, applications, etc.)."),
         Field("digital_identifier", ["openminds.core.DOI", "openminds.core.SWHID"], "vocab:digitalIdentifier", multiple=False, required=False,
               doc="Digital handle to identify objects or legal persons."),
+        Field("formats", "openminds.core.ContentType", "vocab:format", multiple=True, required=True,
+              doc="Method of digitally organizing and structuring data or information."),
         Field("full_documentation", ["openminds.core.DOI", "openminds.core.File", "openminds.core.URL"], "vocab:fullDocumentation", multiple=False, required=True,
               doc="Non-abridged instructions, comments, and information for using a particular product."),
         Field("funding", "openminds.core.Funding", "vocab:funding", multiple=True, required=False,
               doc="Money provided by a legal person for a particular purpose."),
         Field("homepage", "openminds.core.URL", "vocab:homepage", multiple=False, required=False,
-              doc="Main website of the meta data model version."),
+              doc="Main website of the model version."),
         Field("how_to_cite", str, "vocab:howToCite", multiple=False, required=False,
               doc="Preferred format for citing a particular object or legal person."),
-        Field("is_alternative_version_of", "openminds.core.MetaDataModelVersion", "vocab:isAlternativeVersionOf", multiple=True, required=False,
+        Field("input_data", ["openminds.core.DOI", "openminds.core.File", "openminds.core.FileBundle", "openminds.core.URL"], "vocab:inputData", multiple=True, required=False,
+              doc="Data that is put into a process or machine."),
+        Field("is_alternative_version_of", "openminds.core.ModelVersion", "vocab:isAlternativeVersionOf", multiple=True, required=False,
               doc="Reference to an original form where the essence was preserved, but presented in an alternative form."),
-        Field("is_new_version_of", "openminds.core.MetaDataModelVersion", "vocab:isNewVersionOf", multiple=False, required=False,
+        Field("is_new_version_of", "openminds.core.ModelVersion", "vocab:isNewVersionOf", multiple=False, required=False,
               doc="Reference to a previous (potentially outdated) particular form of something."),
-        Field("keywords", ["openminds.controlledterms.ActionStatusType", "openminds.controlledterms.AgeCategory", "openminds.controlledterms.AnatomicalAxesOrientation", "openminds.controlledterms.AnatomicalPlane", "openminds.controlledterms.AnnotationType", "openminds.controlledterms.AtlasType", "openminds.controlledterms.BiologicalOrder", "openminds.controlledterms.BiologicalSex", "openminds.controlledterms.BreedingType", "openminds.controlledterms.CellCultureType", "openminds.controlledterms.CellType", "openminds.controlledterms.ChemicalMixtureType", "openminds.controlledterms.ContributionType", "openminds.controlledterms.CranialWindowType", "openminds.controlledterms.CriteriaQualityType", "openminds.controlledterms.DataType", "openminds.controlledterms.DeviceType", "openminds.controlledterms.DifferenceMeasure", "openminds.controlledterms.Disease", "openminds.controlledterms.DiseaseModel", "openminds.controlledterms.EthicsAssessment", "openminds.controlledterms.ExperimentalApproach", "openminds.controlledterms.FileBundleGrouping", "openminds.controlledterms.FileRepositoryType", "openminds.controlledterms.FileUsageRole", "openminds.controlledterms.GeneticStrainType", "openminds.controlledterms.Handedness", "openminds.controlledterms.Language", "openminds.controlledterms.Laterality", "openminds.controlledterms.MeasuredQuantity", "openminds.controlledterms.MetaDataModelType", "openminds.controlledterms.ModelAbstractionLevel", "openminds.controlledterms.ModelScope", "openminds.controlledterms.MolecularEntity", "openminds.controlledterms.OperatingDevice", "openminds.controlledterms.OperatingSystem", "openminds.controlledterms.Organ", "openminds.controlledterms.PatchClampVariation", "openminds.controlledterms.PreparationType", "openminds.controlledterms.ProductAccessibility", "openminds.controlledterms.ProgrammingLanguage", "openminds.controlledterms.QualitativeOverlap", "openminds.controlledterms.SemanticDataType", "openminds.controlledterms.Service", "openminds.controlledterms.SetupType", "openminds.controlledterms.SoftwareApplicationCategory", "openminds.controlledterms.SoftwareFeature", "openminds.controlledterms.Species", "openminds.controlledterms.StimulationApproach", "openminds.controlledterms.StimulusType", "openminds.controlledterms.SubcellularEntity", "openminds.controlledterms.SubjectAttribute", "openminds.controlledterms.Technique", "openminds.controlledterms.TermSuggestion", "openminds.controlledterms.Terminology", "openminds.controlledterms.TissueSampleAttribute", "openminds.controlledterms.TissueSampleType", "openminds.controlledterms.TypeOfUncertainty", "openminds.controlledterms.UBERONParcellation", "openminds.controlledterms.UnitOfMeasurement"], "vocab:keyword", multiple=True, required=False,
-              doc="Significant word or concept that are representative of the meta data model version."),
-        Field("license", "openminds.core.License", "vocab:license", multiple=False, required=True,
+        Field("keywords", ["openminds.controlledterms.ActionStatusType", "openminds.controlledterms.AgeCategory", "openminds.controlledterms.AnatomicalAxesOrientation", "openminds.controlledterms.AnatomicalPlane", "openminds.controlledterms.AnnotationType", "openminds.controlledterms.AtlasType", "openminds.controlledterms.AuditoryStimulusType", "openminds.controlledterms.BiologicalOrder", "openminds.controlledterms.BiologicalSex", "openminds.controlledterms.BreedingType", "openminds.controlledterms.CellCultureType", "openminds.controlledterms.CellType", "openminds.controlledterms.ChemicalMixtureType", "openminds.controlledterms.ContributionType", "openminds.controlledterms.CranialWindowConstructionType", "openminds.controlledterms.CranialWindowReinforcementType", "openminds.controlledterms.CriteriaQualityType", "openminds.controlledterms.DataType", "openminds.controlledterms.DeviceType", "openminds.controlledterms.DifferenceMeasure", "openminds.controlledterms.Disease", "openminds.controlledterms.DiseaseModel", "openminds.controlledterms.EducationalLevel", "openminds.controlledterms.ElectricalStimulusType", "openminds.controlledterms.EthicsAssessment", "openminds.controlledterms.ExperimentalApproach", "openminds.controlledterms.FileBundleGrouping", "openminds.controlledterms.FileRepositoryType", "openminds.controlledterms.FileUsageRole", "openminds.controlledterms.GeneticStrainType", "openminds.controlledterms.GustatoryStimulusType", "openminds.controlledterms.Handedness", "openminds.controlledterms.Language", "openminds.controlledterms.Laterality", "openminds.controlledterms.LearningResourceType", "openminds.controlledterms.MeasuredQuantity", "openminds.controlledterms.MetaDataModelType", "openminds.controlledterms.ModelAbstractionLevel", "openminds.controlledterms.ModelScope", "openminds.controlledterms.MolecularEntity", "openminds.controlledterms.OlfactoryStimulusType", "openminds.controlledterms.OperatingDevice", "openminds.controlledterms.OperatingSystem", "openminds.controlledterms.OpticalStimulusType", "openminds.controlledterms.Organ", "openminds.controlledterms.PatchClampVariation", "openminds.controlledterms.PreparationType", "openminds.controlledterms.ProductAccessibility", "openminds.controlledterms.ProgrammingLanguage", "openminds.controlledterms.QualitativeOverlap", "openminds.controlledterms.SemanticDataType", "openminds.controlledterms.Service", "openminds.controlledterms.SetupType", "openminds.controlledterms.SoftwareApplicationCategory", "openminds.controlledterms.SoftwareFeature", "openminds.controlledterms.Species", "openminds.controlledterms.StimulationApproach", "openminds.controlledterms.StimulationTechnique", "openminds.controlledterms.SubcellularEntity", "openminds.controlledterms.SubjectAttribute", "openminds.controlledterms.TactileStimulusType", "openminds.controlledterms.Technique", "openminds.controlledterms.TermSuggestion", "openminds.controlledterms.Terminology", "openminds.controlledterms.TissueSampleAttribute", "openminds.controlledterms.TissueSampleType", "openminds.controlledterms.TypeOfUncertainty", "openminds.controlledterms.UBERONParcellation", "openminds.controlledterms.UnitOfMeasurement", "openminds.controlledterms.VisualStimulusType"], "vocab:keyword", multiple=True, required=False,
+              doc="Significant word or concept that are representative of the model version."),
+        Field("licenses", "openminds.core.License", "vocab:license", multiple=True, required=True,
               doc="Grant by a party to another party as an element of an agreement between those parties that permits to do, use, or own something."),
         Field("other_contributions", "openminds.core.Contribution", "vocab:otherContribution", multiple=True, required=False,
               doc="Giving or supplying of something (such as money or time) as a part or share other than what is covered elsewhere."),
+        Field("output_data", ["openminds.core.DOI", "openminds.core.File", "openminds.core.FileBundle", "openminds.core.URL"], "vocab:outputData", multiple=True, required=False,
+              doc="Data that comes out of, is delivered or produced by a process or machine."),
         Field("related_publications", ["openminds.core.DOI", "openminds.core.HANDLE", "openminds.core.ISBN"], "vocab:relatedPublication", multiple=True, required=False,
               doc="Reference to something that was made available for the general public to see or buy."),
         Field("release_date", date, "vocab:releaseDate", multiple=False, required=True,
               doc="Fixed date on which a product is due to become or was made available for the general public to see or buy"),
         Field("repository", "openminds.core.FileRepository", "vocab:repository", multiple=False, required=False,
               doc="Place, room, or container where something is deposited or stored."),
-        Field("serialization_formats", "openminds.core.ContentType", "vocab:serializationFormat", multiple=True, required=False,
-              doc="Form in which a particular data structure or object state is translated to for storage."),
-        Field("specification_formats", "openminds.core.ContentType", "vocab:specificationFormat", multiple=True, required=False,
-              doc="Form in which a particular data structure or object state is specified in."),
         Field("support_channels", str, "vocab:supportChannel", multiple=True, required=False,
               doc="Way of communication used to interact with users or customers."),
-        Field("type", "openminds.controlledterms.MetaDataModelType", "vocab:type", multiple=False, required=True,
-              doc="Distinct class to which a group of entities or concepts with similar characteristics or attributes belong to."),
         Field("version_identifier", str, "vocab:versionIdentifier", multiple=False, required=True,
               doc="Term or code used to identify the version of something."),
         Field("version_innovation", str, "vocab:versionInnovation", multiple=False, required=True,
               doc="Documentation on what changed in comparison to a previously published form of something."),
 
     ]
-    existence_query_fields = ('alias', 'version_identifier')
+    existence_query_fields = ('name', 'version_identifier')
+
+
+    def is_version_of(self, client):
+        parents = Model.list(client, scope=self.scope, space=self.space, versions=self)
+        if len(parents) == 0:
+            raise ResolutionFailure("Unable to find parent")
+        else:
+            assert len(parents) == 1
+            return parents[0]
```

### Comparing `fairgraph-0.8.2/fairgraph/openminds/core/products/model.py` & `fairgraph-0.9.0/fairgraph/openminds/core/products/model.py`

 * *Files 21% similar despite different names*

```diff
@@ -27,28 +27,28 @@
     fields = [
         Field("name", str, "vocab:fullName", multiple=False, required=True,
               doc="Whole, non-abbreviated name of the model."),
         Field("alias", str, "vocab:shortName", multiple=False, required=True,
               doc="Shortened or fully abbreviated name of the model."),
         Field("abstraction_level", "openminds.controlledterms.ModelAbstractionLevel", "vocab:abstractionLevel", multiple=False, required=True,
               doc="Extent of simplification of physical, spatial, or temporal details or attributes in the study of objects or systems."),
-        Field("custodians", ["openminds.core.Organization", "openminds.core.Person"], "vocab:custodian", multiple=True, required=False,
+        Field("custodians", ["openminds.core.Consortium", "openminds.core.Organization", "openminds.core.Person"], "vocab:custodian", multiple=True, required=False,
               doc="The 'custodian' is a legal person who is responsible for the content and quality of the data, metadata, and/or code of a research product."),
         Field("description", str, "vocab:description", multiple=False, required=True,
               doc="Longer statement or account giving the characteristics of the model."),
-        Field("developers", ["openminds.core.Organization", "openminds.core.Person"], "vocab:developer", multiple=True, required=True,
+        Field("developers", ["openminds.core.Consortium", "openminds.core.Organization", "openminds.core.Person"], "vocab:developer", multiple=True, required=True,
               doc="Legal person that creates or improves products or services (e.g., software, applications, etc.)."),
         Field("digital_identifier", ["openminds.core.DOI", "openminds.core.SWHID"], "vocab:digitalIdentifier", multiple=False, required=False,
               doc="Digital handle to identify objects or legal persons."),
         Field("versions", "openminds.core.ModelVersion", "vocab:hasVersion", multiple=True, required=True,
               doc="Reference to variants of an original."),
         Field("homepage", "openminds.core.URL", "vocab:homepage", multiple=False, required=False,
               doc="Main website of the model."),
         Field("how_to_cite", str, "vocab:howToCite", multiple=False, required=False,
               doc="Preferred format for citing a particular object or legal person."),
         Field("model_scope", "openminds.controlledterms.ModelScope", "vocab:scope", multiple=False, required=True,
               doc="Extent of something."),
-        Field("study_targets", ["openminds.controlledterms.BiologicalOrder", "openminds.controlledterms.BiologicalSex", "openminds.controlledterms.BreedingType", "openminds.controlledterms.CellCultureType", "openminds.controlledterms.CellType", "openminds.controlledterms.Disease", "openminds.controlledterms.DiseaseModel", "openminds.controlledterms.GeneticStrainType", "openminds.controlledterms.Handedness", "openminds.controlledterms.MolecularEntity", "openminds.controlledterms.Organ", "openminds.controlledterms.Species", "openminds.controlledterms.SubcellularEntity", "openminds.controlledterms.TermSuggestion", "openminds.controlledterms.UBERONParcellation", "openminds.sands.CustomAnatomicalEntity", "openminds.sands.ParcellationEntity", "openminds.sands.ParcellationEntityVersion"], "vocab:studyTarget", multiple=True, required=True,
+        Field("study_targets", ["openminds.controlledterms.AuditoryStimulusType", "openminds.controlledterms.BiologicalOrder", "openminds.controlledterms.BiologicalSex", "openminds.controlledterms.BreedingType", "openminds.controlledterms.CellCultureType", "openminds.controlledterms.CellType", "openminds.controlledterms.Disease", "openminds.controlledterms.DiseaseModel", "openminds.controlledterms.ElectricalStimulusType", "openminds.controlledterms.GeneticStrainType", "openminds.controlledterms.GustatoryStimulusType", "openminds.controlledterms.Handedness", "openminds.controlledterms.MolecularEntity", "openminds.controlledterms.OlfactoryStimulusType", "openminds.controlledterms.OpticalStimulusType", "openminds.controlledterms.Organ", "openminds.controlledterms.Species", "openminds.controlledterms.SubcellularEntity", "openminds.controlledterms.TactileStimulusType", "openminds.controlledterms.TermSuggestion", "openminds.controlledterms.UBERONParcellation", "openminds.controlledterms.VisualStimulusType", "openminds.sands.CustomAnatomicalEntity", "openminds.sands.ParcellationEntity", "openminds.sands.ParcellationEntityVersion"], "vocab:studyTarget", multiple=True, required=True,
               doc="Structure or function that was targeted within a study."),
 
     ]
     existence_query_fields = ('name',)
```

### Comparing `fairgraph-0.8.2/fairgraph/openminds/core/products/model_version.py` & `fairgraph-0.9.0/fairgraph/openminds/sands/atlas/brain_atlas_version.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,92 +1,88 @@
 """
-Structured information on a computational model (version level).
+Structured information on a brain atlas (version level).
 """
 
 # this file was auto-generated
 
 from datetime import date, datetime
 from fairgraph.base_v3 import KGObject, IRI
 from fairgraph.fields import Field
 
-from fairgraph.errors import ResolutionFailure
-from .model import Model
 
 
-class ModelVersion(KGObject):
+
+class BrainAtlasVersion(KGObject):
     """
-    Structured information on a computational model (version level).
+    Structured information on a brain atlas (version level).
     """
-    default_space = "model"
-    type = ["https://openminds.ebrains.eu/core/ModelVersion"]
+    default_space = "atlas"
+    type = ["https://openminds.ebrains.eu/sands/BrainAtlasVersion"]
     context = {
         "schema": "http://schema.org/",
         "kg": "https://kg.ebrains.eu/api/instances/",
         "vocab": "https://openminds.ebrains.eu/vocab/",
         "terms": "https://openminds.ebrains.eu/controlledTerms/",
         "core": "https://openminds.ebrains.eu/core/"
     }
     fields = [
         Field("name", str, "vocab:fullName", multiple=False, required=False,
-              doc="Whole, non-abbreviated name of the model version."),
+              doc="Whole, non-abbreviated name of the brain atlas version."),
         Field("alias", str, "vocab:shortName", multiple=False, required=True,
-              doc="Shortened or fully abbreviated name of the model version."),
+              doc="Shortened or fully abbreviated name of the brain atlas version."),
+        Field("abbreviation", str, "vocab:abbreviation", multiple=False, required=False,
+              doc="no description available"),
         Field("accessibility", "openminds.controlledterms.ProductAccessibility", "vocab:accessibility", multiple=False, required=True,
-              doc="Level to which something is accessible to the model version."),
+              doc="Level to which something is accessible to the brain atlas version."),
+        Field("atlas_type", "openminds.controlledterms.AtlasType", "vocab:atlasType", multiple=False, required=False,
+              doc="no description available"),
+        Field("authors", ["openminds.core.Consortium", "openminds.core.Organization", "openminds.core.Person"], "vocab:author", multiple=True, required=False,
+              doc="Creator of a literary or creative work, as well as a dataset publication."),
+        Field("coordinate_space", "openminds.sands.CommonCoordinateSpace", "vocab:coordinateSpace", multiple=False, required=True,
+              doc="Two or three dimensional geometric setting."),
         Field("copyright", "openminds.core.Copyright", "vocab:copyright", multiple=False, required=False,
               doc="Exclusive and assignable legal right of an originator to reproduce, publish, sell, or distribute the matter and form of a creative work for a defined time period."),
-        Field("custodians", ["openminds.core.Organization", "openminds.core.Person"], "vocab:custodian", multiple=True, required=False,
+        Field("custodians", ["openminds.core.Consortium", "openminds.core.Organization", "openminds.core.Person"], "vocab:custodian", multiple=True, required=False,
               doc="The 'custodian' is a legal person who is responsible for the content and quality of the data, metadata, and/or code of a research product."),
         Field("description", str, "vocab:description", multiple=False, required=False,
-              doc="Longer statement or account giving the characteristics of the model version."),
-        Field("developers", ["openminds.core.Organization", "openminds.core.Person"], "vocab:developer", multiple=True, required=False,
-              doc="Legal person that creates or improves products or services (e.g., software, applications, etc.)."),
-        Field("digital_identifier", ["openminds.core.DOI", "openminds.core.SWHID"], "vocab:digitalIdentifier", multiple=False, required=False,
+              doc="Longer statement or account giving the characteristics of the brain atlas version."),
+        Field("digital_identifier", ["openminds.core.DOI", "openminds.core.ISBN", "openminds.core.RRID"], "vocab:digitalIdentifier", multiple=False, required=False,
               doc="Digital handle to identify objects or legal persons."),
-        Field("formats", "openminds.core.ContentType", "vocab:format", multiple=True, required=True,
-              doc="Method of digitally organizing and structuring data or information."),
         Field("full_documentation", ["openminds.core.DOI", "openminds.core.File", "openminds.core.URL"], "vocab:fullDocumentation", multiple=False, required=True,
               doc="Non-abridged instructions, comments, and information for using a particular product."),
         Field("funding", "openminds.core.Funding", "vocab:funding", multiple=True, required=False,
               doc="Money provided by a legal person for a particular purpose."),
+        Field("has_terminology_version", "openminds.sands.ParcellationTerminologyVersion", "vocab:hasTerminologyVersion", multiple=False, required=True,
+              doc="no description available"),
         Field("homepage", "openminds.core.URL", "vocab:homepage", multiple=False, required=False,
-              doc="Main website of the model version."),
+              doc="Main website of the brain atlas version."),
         Field("how_to_cite", str, "vocab:howToCite", multiple=False, required=False,
               doc="Preferred format for citing a particular object or legal person."),
-        Field("input_data", ["openminds.core.DOI", "openminds.core.File", "openminds.core.FileBundle", "openminds.core.URL"], "vocab:inputData", multiple=True, required=False,
-              doc="Data that is put into a process or machine."),
-        Field("is_alternative_version_of", "openminds.core.ModelVersion", "vocab:isAlternativeVersionOf", multiple=True, required=False,
+        Field("is_alternative_version_of", "openminds.sands.BrainAtlasVersion", "vocab:isAlternativeVersionOf", multiple=True, required=False,
               doc="Reference to an original form where the essence was preserved, but presented in an alternative form."),
-        Field("is_new_version_of", "openminds.core.ModelVersion", "vocab:isNewVersionOf", multiple=False, required=False,
+        Field("is_new_version_of", "openminds.sands.BrainAtlasVersion", "vocab:isNewVersionOf", multiple=False, required=False,
               doc="Reference to a previous (potentially outdated) particular form of something."),
-        Field("keywords", ["openminds.controlledterms.ActionStatusType", "openminds.controlledterms.AgeCategory", "openminds.controlledterms.AnatomicalAxesOrientation", "openminds.controlledterms.AnatomicalPlane", "openminds.controlledterms.AnnotationType", "openminds.controlledterms.AtlasType", "openminds.controlledterms.BiologicalOrder", "openminds.controlledterms.BiologicalSex", "openminds.controlledterms.BreedingType", "openminds.controlledterms.CellCultureType", "openminds.controlledterms.CellType", "openminds.controlledterms.ChemicalMixtureType", "openminds.controlledterms.ContributionType", "openminds.controlledterms.CranialWindowType", "openminds.controlledterms.CriteriaQualityType", "openminds.controlledterms.DataType", "openminds.controlledterms.DeviceType", "openminds.controlledterms.DifferenceMeasure", "openminds.controlledterms.Disease", "openminds.controlledterms.DiseaseModel", "openminds.controlledterms.EthicsAssessment", "openminds.controlledterms.ExperimentalApproach", "openminds.controlledterms.FileBundleGrouping", "openminds.controlledterms.FileRepositoryType", "openminds.controlledterms.FileUsageRole", "openminds.controlledterms.GeneticStrainType", "openminds.controlledterms.Handedness", "openminds.controlledterms.Language", "openminds.controlledterms.Laterality", "openminds.controlledterms.MeasuredQuantity", "openminds.controlledterms.MetaDataModelType", "openminds.controlledterms.ModelAbstractionLevel", "openminds.controlledterms.ModelScope", "openminds.controlledterms.MolecularEntity", "openminds.controlledterms.OperatingDevice", "openminds.controlledterms.OperatingSystem", "openminds.controlledterms.Organ", "openminds.controlledterms.PatchClampVariation", "openminds.controlledterms.PreparationType", "openminds.controlledterms.ProductAccessibility", "openminds.controlledterms.ProgrammingLanguage", "openminds.controlledterms.QualitativeOverlap", "openminds.controlledterms.SemanticDataType", "openminds.controlledterms.Service", "openminds.controlledterms.SetupType", "openminds.controlledterms.SoftwareApplicationCategory", "openminds.controlledterms.SoftwareFeature", "openminds.controlledterms.Species", "openminds.controlledterms.StimulationApproach", "openminds.controlledterms.StimulusType", "openminds.controlledterms.SubcellularEntity", "openminds.controlledterms.SubjectAttribute", "openminds.controlledterms.Technique", "openminds.controlledterms.TermSuggestion", "openminds.controlledterms.Terminology", "openminds.controlledterms.TissueSampleAttribute", "openminds.controlledterms.TissueSampleType", "openminds.controlledterms.TypeOfUncertainty", "openminds.controlledterms.UBERONParcellation", "openminds.controlledterms.UnitOfMeasurement"], "vocab:keyword", multiple=True, required=False,
-              doc="Significant word or concept that are representative of the model version."),
-        Field("licenses", "openminds.core.License", "vocab:license", multiple=True, required=True,
+        Field("keywords", ["openminds.controlledterms.ActionStatusType", "openminds.controlledterms.AgeCategory", "openminds.controlledterms.AnatomicalAxesOrientation", "openminds.controlledterms.AnatomicalPlane", "openminds.controlledterms.AnnotationType", "openminds.controlledterms.AtlasType", "openminds.controlledterms.AuditoryStimulusType", "openminds.controlledterms.BiologicalOrder", "openminds.controlledterms.BiologicalSex", "openminds.controlledterms.BreedingType", "openminds.controlledterms.CellCultureType", "openminds.controlledterms.CellType", "openminds.controlledterms.ChemicalMixtureType", "openminds.controlledterms.ContributionType", "openminds.controlledterms.CranialWindowConstructionType", "openminds.controlledterms.CranialWindowReinforcementType", "openminds.controlledterms.CriteriaQualityType", "openminds.controlledterms.DataType", "openminds.controlledterms.DeviceType", "openminds.controlledterms.DifferenceMeasure", "openminds.controlledterms.Disease", "openminds.controlledterms.DiseaseModel", "openminds.controlledterms.EducationalLevel", "openminds.controlledterms.ElectricalStimulusType", "openminds.controlledterms.EthicsAssessment", "openminds.controlledterms.ExperimentalApproach", "openminds.controlledterms.FileBundleGrouping", "openminds.controlledterms.FileRepositoryType", "openminds.controlledterms.FileUsageRole", "openminds.controlledterms.GeneticStrainType", "openminds.controlledterms.GustatoryStimulusType", "openminds.controlledterms.Handedness", "openminds.controlledterms.Language", "openminds.controlledterms.Laterality", "openminds.controlledterms.LearningResourceType", "openminds.controlledterms.MeasuredQuantity", "openminds.controlledterms.MetaDataModelType", "openminds.controlledterms.ModelAbstractionLevel", "openminds.controlledterms.ModelScope", "openminds.controlledterms.MolecularEntity", "openminds.controlledterms.OlfactoryStimulusType", "openminds.controlledterms.OperatingDevice", "openminds.controlledterms.OperatingSystem", "openminds.controlledterms.OpticalStimulusType", "openminds.controlledterms.Organ", "openminds.controlledterms.PatchClampVariation", "openminds.controlledterms.PreparationType", "openminds.controlledterms.ProductAccessibility", "openminds.controlledterms.ProgrammingLanguage", "openminds.controlledterms.QualitativeOverlap", "openminds.controlledterms.SemanticDataType", "openminds.controlledterms.Service", "openminds.controlledterms.SetupType", "openminds.controlledterms.SoftwareApplicationCategory", "openminds.controlledterms.SoftwareFeature", "openminds.controlledterms.Species", "openminds.controlledterms.StimulationApproach", "openminds.controlledterms.StimulationTechnique", "openminds.controlledterms.SubcellularEntity", "openminds.controlledterms.SubjectAttribute", "openminds.controlledterms.TactileStimulusType", "openminds.controlledterms.Technique", "openminds.controlledterms.TermSuggestion", "openminds.controlledterms.Terminology", "openminds.controlledterms.TissueSampleAttribute", "openminds.controlledterms.TissueSampleType", "openminds.controlledterms.TypeOfUncertainty", "openminds.controlledterms.UBERONParcellation", "openminds.controlledterms.UnitOfMeasurement", "openminds.controlledterms.VisualStimulusType"], "vocab:keyword", multiple=True, required=False,
+              doc="Significant word or concept that are representative of the brain atlas version."),
+        Field("license", "openminds.core.License", "vocab:license", multiple=False, required=True,
               doc="Grant by a party to another party as an element of an agreement between those parties that permits to do, use, or own something."),
+        Field("ontology_identifier", IRI, "vocab:ontologyIdentifier", multiple=False, required=False,
+              doc="Term or code used to identify the brain atlas version registered within a particular ontology."),
         Field("other_contributions", "openminds.core.Contribution", "vocab:otherContribution", multiple=True, required=False,
               doc="Giving or supplying of something (such as money or time) as a part or share other than what is covered elsewhere."),
-        Field("output_data", ["openminds.core.DOI", "openminds.core.File", "openminds.core.FileBundle", "openminds.core.URL"], "vocab:outputData", multiple=True, required=False,
-              doc="Data that comes out of, is delivered or produced by a process or machine."),
         Field("related_publications", ["openminds.core.DOI", "openminds.core.HANDLE", "openminds.core.ISBN"], "vocab:relatedPublication", multiple=True, required=False,
               doc="Reference to something that was made available for the general public to see or buy."),
         Field("release_date", date, "vocab:releaseDate", multiple=False, required=True,
               doc="Fixed date on which a product is due to become or was made available for the general public to see or buy"),
         Field("repository", "openminds.core.FileRepository", "vocab:repository", multiple=False, required=False,
               doc="Place, room, or container where something is deposited or stored."),
         Field("support_channels", str, "vocab:supportChannel", multiple=True, required=False,
               doc="Way of communication used to interact with users or customers."),
+        Field("used_specimens", ["openminds.core.Subject", "openminds.core.SubjectGroup", "openminds.core.TissueSample", "openminds.core.TissueSampleCollection"], "vocab:usedSpecimen", multiple=True, required=False,
+              doc="no description available"),
         Field("version_identifier", str, "vocab:versionIdentifier", multiple=False, required=True,
               doc="Term or code used to identify the version of something."),
         Field("version_innovation", str, "vocab:versionInnovation", multiple=False, required=True,
               doc="Documentation on what changed in comparison to a previously published form of something."),
 
     ]
-    existence_query_fields = ('name', 'version_identifier')
-
-
-    def is_version_of(self, client):
-        parents = Model.list(client, scope=self.scope, space=self.space, versions=self)
-        if len(parents) == 0:
-            raise ResolutionFailure("Unable to find parent")
-        else:
-            assert len(parents) == 1
-            return parents[0]
+    existence_query_fields = ('alias', 'version_identifier')
```

### Comparing `fairgraph-0.8.2/fairgraph/openminds/core/products/project.py` & `fairgraph-0.9.0/fairgraph/openminds/core/products/project.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,18 +25,18 @@
         "core": "https://openminds.ebrains.eu/core/"
     }
     fields = [
         Field("name", str, "vocab:fullName", multiple=False, required=True,
               doc="Whole, non-abbreviated name of the project."),
         Field("alias", str, "vocab:shortName", multiple=False, required=True,
               doc="Shortened or fully abbreviated name of the project."),
-        Field("coordinators", ["openminds.core.Organization", "openminds.core.Person"], "vocab:coordinator", multiple=True, required=False,
+        Field("coordinators", ["openminds.core.Consortium", "openminds.core.Organization", "openminds.core.Person"], "vocab:coordinator", multiple=True, required=False,
               doc="Legal person who organizes the collaborative work of people or groups."),
         Field("description", str, "vocab:description", multiple=False, required=True,
               doc="Longer statement or account giving the characteristics of the project."),
-        Field("has_research_products", ["openminds.computation.ValidationTest", "openminds.computation.ValidationTestVersion", "openminds.computation.WorkflowRecipe", "openminds.computation.WorkflowRecipeVersion", "openminds.core.Dataset", "openminds.core.DatasetVersion", "openminds.core.MetaDataModel", "openminds.core.MetaDataModelVersion", "openminds.core.Model", "openminds.core.ModelVersion", "openminds.core.Software", "openminds.core.SoftwareVersion", "openminds.publications.LivePaper", "openminds.publications.LivePaperVersion", "openminds.sands.BrainAtlas", "openminds.sands.BrainAtlasVersion"], "vocab:hasResearchProducts", multiple=True, required=True,
+        Field("has_research_products", ["openminds.computation.ValidationTest", "openminds.computation.ValidationTestVersion", "openminds.computation.WorkflowRecipe", "openminds.computation.WorkflowRecipeVersion", "openminds.core.Dataset", "openminds.core.DatasetVersion", "openminds.core.MetaDataModel", "openminds.core.MetaDataModelVersion", "openminds.core.Model", "openminds.core.ModelVersion", "openminds.core.Software", "openminds.core.SoftwareVersion", "openminds.core.WebService", "openminds.core.WebServiceVersion", "openminds.publications.LivePaper", "openminds.publications.LivePaperVersion", "openminds.sands.BrainAtlas", "openminds.sands.BrainAtlasVersion"], "vocab:hasResearchProducts", multiple=True, required=True,
               doc="Reference to subsidiary research products."),
         Field("homepage", "openminds.core.URL", "vocab:homepage", multiple=False, required=False,
               doc="Main website of the project."),
 
     ]
     existence_query_fields = ('alias',)
```

### Comparing `fairgraph-0.8.2/fairgraph/openminds/core/products/setup.py` & `fairgraph-0.9.0/fairgraph/openminds/sands/atlas/parcellation_terminology_version.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,42 +1,34 @@
 """
 
 """
 
 # this file was auto-generated
 
 from datetime import date, datetime
-from fairgraph.base_v3 import KGObject, IRI
+from fairgraph.base_v3 import EmbeddedMetadata, IRI
 from fairgraph.fields import Field
 
 
 
 
-class Setup(KGObject):
+class ParcellationTerminologyVersion(EmbeddedMetadata):
     """
 
     """
-    default_space = "dataset"
-    type = ["https://openminds.ebrains.eu/core/Setup"]
+    type = ["https://openminds.ebrains.eu/sands/ParcellationTerminologyVersion"]
     context = {
         "schema": "http://schema.org/",
         "kg": "https://kg.ebrains.eu/api/instances/",
         "vocab": "https://openminds.ebrains.eu/vocab/",
         "terms": "https://openminds.ebrains.eu/controlledTerms/",
         "core": "https://openminds.ebrains.eu/core/"
     }
     fields = [
-        Field("name", str, "vocab:name", multiple=False, required=True,
-              doc="Word or phrase that constitutes the distinctive designation of the setup."),
-        Field("components", ["openminds.core.Setup", "openminds.core.SoftwareVersion", "openminds.ephys.Electrode", "openminds.ephys.ElectrodeArray", "openminds.ephys.Pipette"], "vocab:components", multiple=True, required=True,
-              doc="no description available"),
-        Field("description", str, "vocab:description", multiple=False, required=True,
-              doc="Longer statement or account giving the characteristics of the setup."),
-        Field("location", str, "vocab:location", multiple=False, required=False,
-              doc="no description available"),
-        Field("manufacturers", ["openminds.core.Organization", "openminds.core.Person"], "vocab:manufacturer", multiple=True, required=False,
-              doc="no description available"),
-        Field("setup_types", "openminds.controlledterms.SetupType", "vocab:setupType", multiple=True, required=False,
+        Field("defined_ins", "openminds.core.File", "vocab:definedIn", multiple=True, required=False,
+              doc="Reference to a file instance in which something is stored."),
+        Field("has_entity_versions", "openminds.sands.ParcellationEntityVersion", "vocab:hasEntityVersion", multiple=True, required=True,
               doc="no description available"),
+        Field("ontology_identifiers", str, "vocab:ontologyIdentifier", multiple=True, required=False,
+              doc="Term or code used to identify the parcellation terminology version registered within a particular ontology."),
 
     ]
-    existence_query_fields = ('name', 'components', 'description')
```

### Comparing `fairgraph-0.8.2/fairgraph/openminds/core/products/software.py` & `fairgraph-0.9.0/fairgraph/openminds/core/research/behavioral_protocol.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,48 +1,42 @@
 """
-Structured information on a software tool (concept level).
+Structured information about a protocol used in an experiment studying human or animal behavior.
 """
 
 # this file was auto-generated
 
 from datetime import date, datetime
 from fairgraph.base_v3 import KGObject, IRI
 from fairgraph.fields import Field
 
 
 
 
-class Software(KGObject):
+class BehavioralProtocol(KGObject):
     """
-    Structured information on a software tool (concept level).
+    Structured information about a protocol used in an experiment studying human or animal behavior.
     """
-    default_space = "software"
-    type = ["https://openminds.ebrains.eu/core/Software"]
+    default_space = "dataset"
+    type = ["https://openminds.ebrains.eu/core/BehavioralProtocol"]
     context = {
         "schema": "http://schema.org/",
         "kg": "https://kg.ebrains.eu/api/instances/",
         "vocab": "https://openminds.ebrains.eu/vocab/",
         "terms": "https://openminds.ebrains.eu/controlledTerms/",
         "core": "https://openminds.ebrains.eu/core/"
     }
     fields = [
-        Field("name", str, "vocab:fullName", multiple=False, required=True,
-              doc="Whole, non-abbreviated name of the software."),
-        Field("alias", str, "vocab:shortName", multiple=False, required=True,
-              doc="Shortened or fully abbreviated name of the software."),
-        Field("custodians", ["openminds.core.Organization", "openminds.core.Person"], "vocab:custodian", multiple=True, required=False,
-              doc="The 'custodian' is a legal person who is responsible for the content and quality of the data, metadata, and/or code of a research product."),
+        Field("name", str, "vocab:name", multiple=False, required=True,
+              doc="Word or phrase that constitutes the distinctive designation of the behavioral protocol."),
+        Field("described_in", ["openminds.core.DOI", "openminds.core.File", "openminds.core.URL"], "vocab:describedIn", multiple=False, required=False,
+              doc="no description available"),
         Field("description", str, "vocab:description", multiple=False, required=True,
-              doc="Longer statement or account giving the characteristics of the software."),
-        Field("developers", ["openminds.core.Organization", "openminds.core.Person"], "vocab:developer", multiple=True, required=True,
-              doc="Legal person that creates or improves products or services (e.g., software, applications, etc.)."),
-        Field("digital_identifier", ["openminds.core.DOI", "openminds.core.SWHID"], "vocab:digitalIdentifier", multiple=False, required=False,
-              doc="Digital handle to identify objects or legal persons."),
-        Field("versions", "openminds.core.SoftwareVersion", "vocab:hasVersion", multiple=True, required=True,
-              doc="Reference to variants of an original."),
-        Field("homepage", "openminds.core.URL", "vocab:homepage", multiple=False, required=False,
-              doc="Main website of the software."),
-        Field("how_to_cite", str, "vocab:howToCite", multiple=False, required=False,
-              doc="Preferred format for citing a particular object or legal person."),
+              doc="Longer statement or account giving the characteristics of the behavioral protocol."),
+        Field("internal_identifier", str, "vocab:internalIdentifier", multiple=False, required=False,
+              doc="Term or code that identifies the behavioral protocol within a particular product."),
+        Field("stimulations", ["openminds.controlledterms.StimulationApproach", "openminds.controlledterms.StimulationTechnique"], "vocab:stimulation", multiple=True, required=False,
+              doc="no description available"),
+        Field("stimulus_types", ["openminds.controlledterms.AuditoryStimulusType", "openminds.controlledterms.ElectricalStimulusType", "openminds.controlledterms.GustatoryStimulusType", "openminds.controlledterms.OlfactoryStimulusType", "openminds.controlledterms.OpticalStimulusType", "openminds.controlledterms.TactileStimulusType", "openminds.controlledterms.VisualStimulusType"], "vocab:stimulusType", multiple=True, required=False,
+              doc="no description available"),
 
     ]
-    existence_query_fields = ('alias',)
+    existence_query_fields = ('name', 'description')
```

### Comparing `fairgraph-0.8.2/fairgraph/openminds/core/products/software_version.py` & `fairgraph-0.9.0/fairgraph/openminds/core/products/dataset_version.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,94 +1,114 @@
 """
-
+Structured information on data originating from human/animal studies or simulations (version level).
 """
 
 # this file was auto-generated
 
 from datetime import date, datetime
 from fairgraph.base_v3 import KGObject, IRI
 from fairgraph.fields import Field
 
+from urllib.request import urlretrieve
+from pathlib import Path
+from fairgraph.utility import accepted_terms_of_use
 
 
-
-class SoftwareVersion(KGObject):
+class DatasetVersion(KGObject):
     """
-
+    Structured information on data originating from human/animal studies or simulations (version level).
     """
-    default_space = "software"
-    type = ["https://openminds.ebrains.eu/core/SoftwareVersion"]
+    default_space = "dataset"
+    type = ["https://openminds.ebrains.eu/core/DatasetVersion"]
     context = {
         "schema": "http://schema.org/",
         "kg": "https://kg.ebrains.eu/api/instances/",
         "vocab": "https://openminds.ebrains.eu/vocab/",
         "terms": "https://openminds.ebrains.eu/controlledTerms/",
         "core": "https://openminds.ebrains.eu/core/"
     }
     fields = [
         Field("name", str, "vocab:fullName", multiple=False, required=False,
-              doc="Whole, non-abbreviated name of the software version."),
+              doc="Whole, non-abbreviated name of the dataset version."),
         Field("alias", str, "vocab:shortName", multiple=False, required=True,
-              doc="Shortened or fully abbreviated name of the software version."),
+              doc="Shortened or fully abbreviated name of the dataset version."),
         Field("accessibility", "openminds.controlledterms.ProductAccessibility", "vocab:accessibility", multiple=False, required=True,
-              doc="Level to which something is accessible to the software version."),
-        Field("application_categories", "openminds.controlledterms.SoftwareApplicationCategory", "vocab:applicationCategory", multiple=True, required=True,
-              doc="Distinct class that groups software programs which perform a similar task or set of tasks."),
+              doc="Level to which something is accessible to the dataset version."),
+        Field("authors", ["openminds.core.Consortium", "openminds.core.Organization", "openminds.core.Person"], "vocab:author", multiple=True, required=False,
+              doc="Creator of a literary or creative work, as well as a dataset publication."),
+        Field("behavioral_protocols", "openminds.core.BehavioralProtocol", "vocab:behavioralProtocol", multiple=True, required=False,
+              doc="no description available"),
         Field("copyright", "openminds.core.Copyright", "vocab:copyright", multiple=False, required=False,
               doc="Exclusive and assignable legal right of an originator to reproduce, publish, sell, or distribute the matter and form of a creative work for a defined time period."),
-        Field("custodians", ["openminds.core.Organization", "openminds.core.Person"], "vocab:custodian", multiple=True, required=False,
+        Field("custodians", ["openminds.core.Consortium", "openminds.core.Organization", "openminds.core.Person"], "vocab:custodian", multiple=True, required=False,
               doc="The 'custodian' is a legal person who is responsible for the content and quality of the data, metadata, and/or code of a research product."),
+        Field("data_types", "openminds.controlledterms.SemanticDataType", "vocab:dataType", multiple=True, required=True,
+              doc="no description available"),
         Field("description", str, "vocab:description", multiple=False, required=False,
-              doc="Longer statement or account giving the characteristics of the software version."),
-        Field("developers", ["openminds.core.Organization", "openminds.core.Person"], "vocab:developer", multiple=True, required=False,
-              doc="Legal person that creates or improves products or services (e.g., software, applications, etc.)."),
-        Field("devices", "openminds.controlledterms.OperatingDevice", "vocab:device", multiple=True, required=True,
-              doc="Piece of equipment or mechanism (hardware) designed to serve a special purpose or perform a special function."),
-        Field("digital_identifier", ["openminds.core.DOI", "openminds.core.SWHID"], "vocab:digitalIdentifier", multiple=False, required=False,
+              doc="Longer statement or account giving the characteristics of the dataset version."),
+        Field("digital_identifier", "openminds.core.DOI", "vocab:digitalIdentifier", multiple=False, required=True,
               doc="Digital handle to identify objects or legal persons."),
-        Field("features", "openminds.controlledterms.SoftwareFeature", "vocab:feature", multiple=True, required=True,
-              doc="Structure, form, or appearance that characterizes the software version."),
+        Field("ethics_assessment", "openminds.controlledterms.EthicsAssessment", "vocab:ethicsAssessment", multiple=False, required=True,
+              doc="Judgment about the applied principles of conduct governing an individual or a group."),
+        Field("experimental_approaches", "openminds.controlledterms.ExperimentalApproach", "vocab:experimentalApproach", multiple=True, required=True,
+              doc="no description available"),
         Field("full_documentation", ["openminds.core.DOI", "openminds.core.File", "openminds.core.URL"], "vocab:fullDocumentation", multiple=False, required=True,
               doc="Non-abridged instructions, comments, and information for using a particular product."),
         Field("funding", "openminds.core.Funding", "vocab:funding", multiple=True, required=False,
               doc="Money provided by a legal person for a particular purpose."),
         Field("homepage", "openminds.core.URL", "vocab:homepage", multiple=False, required=False,
-              doc="Main website of the software version."),
+              doc="Main website of the dataset version."),
         Field("how_to_cite", str, "vocab:howToCite", multiple=False, required=False,
               doc="Preferred format for citing a particular object or legal person."),
-        Field("input_formats", "openminds.core.ContentType", "vocab:inputFormat", multiple=True, required=False,
-              doc="Format of data that is put into a process or machine."),
-        Field("is_alternative_version_of", "openminds.core.SoftwareVersion", "vocab:isAlternativeVersionOf", multiple=True, required=False,
+        Field("input_data", ["openminds.core.DOI", "openminds.core.File", "openminds.core.FileBundle", "openminds.core.URL", "openminds.sands.BrainAtlasVersion", "openminds.sands.CommonCoordinateSpace"], "vocab:inputData", multiple=True, required=False,
+              doc="Data that is put into a process or machine."),
+        Field("is_alternative_version_of", "openminds.core.DatasetVersion", "vocab:isAlternativeVersionOf", multiple=True, required=False,
               doc="Reference to an original form where the essence was preserved, but presented in an alternative form."),
-        Field("is_new_version_of", "openminds.core.SoftwareVersion", "vocab:isNewVersionOf", multiple=False, required=False,
+        Field("is_new_version_of", "openminds.core.DatasetVersion", "vocab:isNewVersionOf", multiple=False, required=False,
               doc="Reference to a previous (potentially outdated) particular form of something."),
-        Field("keywords", ["openminds.controlledterms.ActionStatusType", "openminds.controlledterms.AgeCategory", "openminds.controlledterms.AnatomicalAxesOrientation", "openminds.controlledterms.AnatomicalPlane", "openminds.controlledterms.AnnotationType", "openminds.controlledterms.AtlasType", "openminds.controlledterms.BiologicalOrder", "openminds.controlledterms.BiologicalSex", "openminds.controlledterms.BreedingType", "openminds.controlledterms.CellCultureType", "openminds.controlledterms.CellType", "openminds.controlledterms.ChemicalMixtureType", "openminds.controlledterms.ContributionType", "openminds.controlledterms.CranialWindowType", "openminds.controlledterms.CriteriaQualityType", "openminds.controlledterms.DataType", "openminds.controlledterms.DeviceType", "openminds.controlledterms.DifferenceMeasure", "openminds.controlledterms.Disease", "openminds.controlledterms.DiseaseModel", "openminds.controlledterms.EthicsAssessment", "openminds.controlledterms.ExperimentalApproach", "openminds.controlledterms.FileBundleGrouping", "openminds.controlledterms.FileRepositoryType", "openminds.controlledterms.FileUsageRole", "openminds.controlledterms.GeneticStrainType", "openminds.controlledterms.Handedness", "openminds.controlledterms.Language", "openminds.controlledterms.Laterality", "openminds.controlledterms.MeasuredQuantity", "openminds.controlledterms.MetaDataModelType", "openminds.controlledterms.ModelAbstractionLevel", "openminds.controlledterms.ModelScope", "openminds.controlledterms.MolecularEntity", "openminds.controlledterms.OperatingDevice", "openminds.controlledterms.OperatingSystem", "openminds.controlledterms.Organ", "openminds.controlledterms.PatchClampVariation", "openminds.controlledterms.PreparationType", "openminds.controlledterms.ProductAccessibility", "openminds.controlledterms.ProgrammingLanguage", "openminds.controlledterms.QualitativeOverlap", "openminds.controlledterms.SemanticDataType", "openminds.controlledterms.Service", "openminds.controlledterms.SetupType", "openminds.controlledterms.SoftwareApplicationCategory", "openminds.controlledterms.SoftwareFeature", "openminds.controlledterms.Species", "openminds.controlledterms.StimulationApproach", "openminds.controlledterms.StimulusType", "openminds.controlledterms.SubcellularEntity", "openminds.controlledterms.SubjectAttribute", "openminds.controlledterms.Technique", "openminds.controlledterms.TermSuggestion", "openminds.controlledterms.Terminology", "openminds.controlledterms.TissueSampleAttribute", "openminds.controlledterms.TissueSampleType", "openminds.controlledterms.TypeOfUncertainty", "openminds.controlledterms.UBERONParcellation", "openminds.controlledterms.UnitOfMeasurement"], "vocab:keyword", multiple=True, required=False,
-              doc="Significant word or concept that are representative of the software version."),
-        Field("languages", "openminds.controlledterms.Language", "vocab:language", multiple=True, required=True,
-              doc="System of communication (words, their pronunciation, and the methods of combining them) used and understood by a particular community."),
-        Field("licenses", "openminds.core.License", "vocab:license", multiple=True, required=True,
+        Field("keywords", ["openminds.controlledterms.ActionStatusType", "openminds.controlledterms.AgeCategory", "openminds.controlledterms.AnatomicalAxesOrientation", "openminds.controlledterms.AnatomicalPlane", "openminds.controlledterms.AnnotationType", "openminds.controlledterms.AtlasType", "openminds.controlledterms.AuditoryStimulusType", "openminds.controlledterms.BiologicalOrder", "openminds.controlledterms.BiologicalSex", "openminds.controlledterms.BreedingType", "openminds.controlledterms.CellCultureType", "openminds.controlledterms.CellType", "openminds.controlledterms.ChemicalMixtureType", "openminds.controlledterms.ContributionType", "openminds.controlledterms.CranialWindowConstructionType", "openminds.controlledterms.CranialWindowReinforcementType", "openminds.controlledterms.CriteriaQualityType", "openminds.controlledterms.DataType", "openminds.controlledterms.DeviceType", "openminds.controlledterms.DifferenceMeasure", "openminds.controlledterms.Disease", "openminds.controlledterms.DiseaseModel", "openminds.controlledterms.EducationalLevel", "openminds.controlledterms.ElectricalStimulusType", "openminds.controlledterms.EthicsAssessment", "openminds.controlledterms.ExperimentalApproach", "openminds.controlledterms.FileBundleGrouping", "openminds.controlledterms.FileRepositoryType", "openminds.controlledterms.FileUsageRole", "openminds.controlledterms.GeneticStrainType", "openminds.controlledterms.GustatoryStimulusType", "openminds.controlledterms.Handedness", "openminds.controlledterms.Language", "openminds.controlledterms.Laterality", "openminds.controlledterms.LearningResourceType", "openminds.controlledterms.MeasuredQuantity", "openminds.controlledterms.MetaDataModelType", "openminds.controlledterms.ModelAbstractionLevel", "openminds.controlledterms.ModelScope", "openminds.controlledterms.MolecularEntity", "openminds.controlledterms.OlfactoryStimulusType", "openminds.controlledterms.OperatingDevice", "openminds.controlledterms.OperatingSystem", "openminds.controlledterms.OpticalStimulusType", "openminds.controlledterms.Organ", "openminds.controlledterms.PatchClampVariation", "openminds.controlledterms.PreparationType", "openminds.controlledterms.ProductAccessibility", "openminds.controlledterms.ProgrammingLanguage", "openminds.controlledterms.QualitativeOverlap", "openminds.controlledterms.SemanticDataType", "openminds.controlledterms.Service", "openminds.controlledterms.SetupType", "openminds.controlledterms.SoftwareApplicationCategory", "openminds.controlledterms.SoftwareFeature", "openminds.controlledterms.Species", "openminds.controlledterms.StimulationApproach", "openminds.controlledterms.StimulationTechnique", "openminds.controlledterms.SubcellularEntity", "openminds.controlledterms.SubjectAttribute", "openminds.controlledterms.TactileStimulusType", "openminds.controlledterms.Technique", "openminds.controlledterms.TermSuggestion", "openminds.controlledterms.Terminology", "openminds.controlledterms.TissueSampleAttribute", "openminds.controlledterms.TissueSampleType", "openminds.controlledterms.TypeOfUncertainty", "openminds.controlledterms.UBERONParcellation", "openminds.controlledterms.UnitOfMeasurement", "openminds.controlledterms.VisualStimulusType"], "vocab:keyword", multiple=True, required=False,
+              doc="Significant word or concept that are representative of the dataset version."),
+        Field("license", "openminds.core.License", "vocab:license", multiple=False, required=True,
               doc="Grant by a party to another party as an element of an agreement between those parties that permits to do, use, or own something."),
-        Field("operating_systems", "openminds.controlledterms.OperatingSystem", "vocab:operatingSystem", multiple=True, required=True,
-              doc="Software that controls the operation of a computer and directs the processing of programs."),
         Field("other_contributions", "openminds.core.Contribution", "vocab:otherContribution", multiple=True, required=False,
               doc="Giving or supplying of something (such as money or time) as a part or share other than what is covered elsewhere."),
-        Field("output_formats", "openminds.core.ContentType", "vocab:outputFormat", multiple=True, required=False,
-              doc="Format of data that comes out of, is delivered or produced by a process or machine."),
-        Field("programming_languages", "openminds.controlledterms.ProgrammingLanguage", "vocab:programmingLanguage", multiple=True, required=True,
-              doc="Distinct set of instructions for computer programs in order to produce various kinds of output."),
+        Field("preparation_designs", "openminds.controlledterms.PreparationType", "vocab:preparationDesign", multiple=True, required=False,
+              doc="no description available"),
         Field("related_publications", ["openminds.core.DOI", "openminds.core.HANDLE", "openminds.core.ISBN"], "vocab:relatedPublication", multiple=True, required=False,
               doc="Reference to something that was made available for the general public to see or buy."),
         Field("release_date", date, "vocab:releaseDate", multiple=False, required=True,
               doc="Fixed date on which a product is due to become or was made available for the general public to see or buy"),
         Field("repository", "openminds.core.FileRepository", "vocab:repository", multiple=False, required=False,
               doc="Place, room, or container where something is deposited or stored."),
-        Field("requirements", str, "vocab:requirement", multiple=True, required=False,
-              doc="Something essential to the existence, occurrence or function of something else."),
+        Field("studied_specimens", ["openminds.core.Subject", "openminds.core.SubjectGroup", "openminds.core.TissueSample", "openminds.core.TissueSampleCollection"], "vocab:studiedSpecimen", multiple=True, required=False,
+              doc="no description available"),
+        Field("study_targets", ["openminds.controlledterms.AuditoryStimulusType", "openminds.controlledterms.BiologicalOrder", "openminds.controlledterms.BiologicalSex", "openminds.controlledterms.BreedingType", "openminds.controlledterms.CellCultureType", "openminds.controlledterms.CellType", "openminds.controlledterms.Disease", "openminds.controlledterms.DiseaseModel", "openminds.controlledterms.ElectricalStimulusType", "openminds.controlledterms.GeneticStrainType", "openminds.controlledterms.GustatoryStimulusType", "openminds.controlledterms.Handedness", "openminds.controlledterms.MolecularEntity", "openminds.controlledterms.OlfactoryStimulusType", "openminds.controlledterms.OpticalStimulusType", "openminds.controlledterms.Organ", "openminds.controlledterms.Species", "openminds.controlledterms.SubcellularEntity", "openminds.controlledterms.TactileStimulusType", "openminds.controlledterms.TermSuggestion", "openminds.controlledterms.UBERONParcellation", "openminds.controlledterms.VisualStimulusType", "openminds.sands.CustomAnatomicalEntity", "openminds.sands.ParcellationEntity", "openminds.sands.ParcellationEntityVersion"], "vocab:studyTarget", multiple=True, required=False,
+              doc="Structure or function that was targeted within a study."),
         Field("support_channels", str, "vocab:supportChannel", multiple=True, required=False,
               doc="Way of communication used to interact with users or customers."),
+        Field("techniques", "openminds.controlledterms.Technique", "vocab:technique", multiple=True, required=True,
+              doc="Method of accomplishing a desired aim."),
         Field("version_identifier", str, "vocab:versionIdentifier", multiple=False, required=True,
               doc="Term or code used to identify the version of something."),
         Field("version_innovation", str, "vocab:versionInnovation", multiple=False, required=True,
               doc="Documentation on what changed in comparison to a previously published form of something."),
 
     ]
     existence_query_fields = ('alias', 'version_identifier')
+
+
+    def download(self, local_path, client, accept_terms_of_use=False):
+        if accepted_terms_of_use(client, accept_terms_of_use=accept_terms_of_use):
+            repo = self.repository.resolve(client, scope=self.scope or None)
+            if (repo.iri.value.startswith("https://object.cscs.ch/v1/AUTH")
+                or repo.iri.value.startswith("https://data-proxy.ebrains.eu/api/v1/public")
+            ):
+                zip_archive_url = f"https://data.kg.ebrains.eu/zip?container={repo.iri.value}"
+            else:
+                raise NotImplementedError("Download not yet implemented for this repository type")
+            if local_path.endswith(".zip"):
+                local_filename = Path(local_path)
+            else:
+                local_filename = Path(local_path) / (zip_archive_url.split("/")[-1] + ".zip")
+            local_filename.parent.mkdir(parents=True, exist_ok=True)
+            local_filename, headers = urlretrieve(zip_archive_url, local_filename)
+            return local_filename
```

### Comparing `fairgraph-0.8.2/fairgraph/openminds/core/research/behavioral_protocol.py` & `fairgraph-0.9.0/fairgraph/openminds/core/miscellaneous/orcid.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,40 +1,32 @@
 """
-
+A persistent identifier for a researcher provided by Open Researcher and Contributor ID, Inc.
 """
 
 # this file was auto-generated
 
 from datetime import date, datetime
 from fairgraph.base_v3 import KGObject, IRI
 from fairgraph.fields import Field
 
 
 
 
-class BehavioralProtocol(KGObject):
+class ORCID(KGObject):
     """
-
+    A persistent identifier for a researcher provided by Open Researcher and Contributor ID, Inc.
     """
-    default_space = "dataset"
-    type = ["https://openminds.ebrains.eu/core/BehavioralProtocol"]
+    default_space = "common"
+    type = ["https://openminds.ebrains.eu/core/ORCID"]
     context = {
         "schema": "http://schema.org/",
         "kg": "https://kg.ebrains.eu/api/instances/",
         "vocab": "https://openminds.ebrains.eu/vocab/",
         "terms": "https://openminds.ebrains.eu/controlledTerms/",
         "core": "https://openminds.ebrains.eu/core/"
     }
     fields = [
-        Field("name", str, "vocab:name", multiple=False, required=True,
-              doc="Word or phrase that constitutes the distinctive designation of the behavioral protocol."),
-        Field("described_in", ["openminds.core.DOI", "openminds.core.File", "openminds.core.URL"], "vocab:describedIn", multiple=False, required=False,
-              doc="no description available"),
-        Field("description", str, "vocab:description", multiple=False, required=True,
-              doc="Longer statement or account giving the characteristics of the behavioral protocol."),
-        Field("internal_identifier", str, "vocab:internalIdentifier", multiple=False, required=False,
-              doc="Term or code that identifies the behavioral protocol within a particular product."),
-        Field("stimulations", "openminds.core.Stimulation", "vocab:stimulation", multiple=True, required=False,
-              doc="no description available"),
+        Field("identifier", str, "vocab:identifier", multiple=False, required=True,
+              doc="Term or code used to identify the ORCID."),
 
     ]
-    existence_query_fields = ('name', 'description')
+    existence_query_fields = ('identifier',)
```

### Comparing `fairgraph-0.8.2/fairgraph/openminds/core/research/configuration.py` & `fairgraph-0.9.0/fairgraph/openminds/core/miscellaneous/gridid.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,36 +1,32 @@
 """
-
+A GRID (Global Research Identifier Database) identifier.
 """
 
 # this file was auto-generated
 
 from datetime import date, datetime
 from fairgraph.base_v3 import KGObject, IRI
 from fairgraph.fields import Field
 
 
 
 
-class Configuration(KGObject):
+class GRIDID(KGObject):
     """
-
+    A GRID (Global Research Identifier Database) identifier.
     """
     default_space = "common"
-    type = ["https://openminds.ebrains.eu/core/Configuration"]
+    type = ["https://openminds.ebrains.eu/core/GRIDID"]
     context = {
         "schema": "http://schema.org/",
         "kg": "https://kg.ebrains.eu/api/instances/",
         "vocab": "https://openminds.ebrains.eu/vocab/",
         "terms": "https://openminds.ebrains.eu/controlledTerms/",
         "core": "https://openminds.ebrains.eu/core/"
     }
     fields = [
-        Field("lookup_label", str, "vocab:lookupLabel", multiple=False, required=False,
-              doc="no description available"),
-        Field("configuration", str, "vocab:configuration", multiple=False, required=True,
-              doc="no description available"),
-        Field("definition_format", "openminds.core.ContentType", "vocab:definitionFormat", multiple=False, required=True,
-              doc="no description available"),
+        Field("identifier", str, "vocab:identifier", multiple=False, required=True,
+              doc="Term or code used to identify the GRIDID."),
 
     ]
-    existence_query_fields = ('lookup_label',)
+    existence_query_fields = ('identifier',)
```

### Comparing `fairgraph-0.8.2/fairgraph/openminds/core/research/experimental_activity.py` & `fairgraph-0.9.0/fairgraph/openminds/core/research/experimental_activity.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 """
-
+Structured information about an activity performed as part of a scientific experiment.
 """
 
 # this file was auto-generated
 
 from datetime import date, datetime
 from fairgraph.base_v3 import KGObject, IRI
 from fairgraph.fields import Field
 
 
 
 
 class ExperimentalActivity(KGObject):
     """
-
+    Structured information about an activity performed as part of a scientific experiment.
     """
     default_space = "dataset"
     type = ["https://openminds.ebrains.eu/core/ExperimentalActivity"]
     context = {
         "schema": "http://schema.org/",
         "kg": "https://kg.ebrains.eu/api/instances/",
         "vocab": "https://openminds.ebrains.eu/vocab/",
@@ -35,18 +35,20 @@
               doc="no description available"),
         Field("inputs", ["openminds.core.File", "openminds.core.FileBundle"], "vocab:input", multiple=True, required=True,
               doc="Something or someone that is put into or participates in a process or machine."),
         Field("is_part_of", "openminds.core.DatasetVersion", "vocab:isPartOf", multiple=False, required=True,
               doc="Reference to the ensemble of multiple things or beings."),
         Field("outputs", ["openminds.core.File", "openminds.core.FileBundle"], "vocab:output", multiple=True, required=True,
               doc="Something or someone that comes out of, is delivered or produced by a process or machine."),
+        Field("performed_by", ["openminds.computation.SoftwareAgent", "openminds.core.Person"], "vocab:performedBy", multiple=True, required=False,
+              doc="no description available"),
         Field("preparation_design", "openminds.controlledterms.PreparationType", "vocab:preparationDesign", multiple=False, required=False,
               doc="no description available"),
         Field("protocols", "openminds.core.Protocol", "vocab:protocol", multiple=True, required=True,
               doc="Plan that describes the process of a scientific or medical experiment, treatment, or procedure."),
         Field("started_at_time", datetime, "vocab:startedAtTime", multiple=False, required=False,
               doc="no description available"),
-        Field("study_targets", ["openminds.controlledterms.BiologicalOrder", "openminds.controlledterms.BiologicalSex", "openminds.controlledterms.BreedingType", "openminds.controlledterms.CellCultureType", "openminds.controlledterms.CellType", "openminds.controlledterms.Disease", "openminds.controlledterms.DiseaseModel", "openminds.controlledterms.GeneticStrainType", "openminds.controlledterms.Handedness", "openminds.controlledterms.MolecularEntity", "openminds.controlledterms.Organ", "openminds.controlledterms.Species", "openminds.controlledterms.SubcellularEntity", "openminds.controlledterms.TermSuggestion", "openminds.controlledterms.UBERONParcellation", "openminds.sands.CustomAnatomicalEntity", "openminds.sands.ParcellationEntity", "openminds.sands.ParcellationEntityVersion"], "vocab:studyTarget", multiple=True, required=False,
+        Field("study_targets", ["openminds.controlledterms.AuditoryStimulusType", "openminds.controlledterms.BiologicalOrder", "openminds.controlledterms.BiologicalSex", "openminds.controlledterms.BreedingType", "openminds.controlledterms.CellCultureType", "openminds.controlledterms.CellType", "openminds.controlledterms.Disease", "openminds.controlledterms.DiseaseModel", "openminds.controlledterms.ElectricalStimulusType", "openminds.controlledterms.GeneticStrainType", "openminds.controlledterms.GustatoryStimulusType", "openminds.controlledterms.Handedness", "openminds.controlledterms.MolecularEntity", "openminds.controlledterms.OlfactoryStimulusType", "openminds.controlledterms.OpticalStimulusType", "openminds.controlledterms.Organ", "openminds.controlledterms.Species", "openminds.controlledterms.SubcellularEntity", "openminds.controlledterms.TactileStimulusType", "openminds.controlledterms.TermSuggestion", "openminds.controlledterms.UBERONParcellation", "openminds.controlledterms.VisualStimulusType", "openminds.sands.CustomAnatomicalEntity", "openminds.sands.ParcellationEntity", "openminds.sands.ParcellationEntityVersion"], "vocab:studyTarget", multiple=True, required=False,
               doc="Structure or function that was targeted within a study."),
 
     ]
     existence_query_fields = ('lookup_label',)
```

### Comparing `fairgraph-0.8.2/fairgraph/openminds/core/research/numerical_property.py` & `fairgraph-0.9.0/fairgraph/openminds/core/miscellaneous/doi.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 """
-
+Structured information about a digital object identifier, as standardized by the International Organization for Standardization.
 """
 
 # this file was auto-generated
 
 from datetime import date, datetime
-from fairgraph.base_v3 import EmbeddedMetadata, IRI
+from fairgraph.base_v3 import KGObject, IRI
 from fairgraph.fields import Field
 
 
 
 
-class NumericalProperty(EmbeddedMetadata):
+class DOI(KGObject):
     """
-
+    Structured information about a digital object identifier, as standardized by the International Organization for Standardization.
     """
-    type = ["https://openminds.ebrains.eu/core/NumericalProperty"]
+    default_space = "dataset"
+    type = ["https://openminds.ebrains.eu/core/DOI"]
     context = {
         "schema": "http://schema.org/",
         "kg": "https://kg.ebrains.eu/api/instances/",
         "vocab": "https://openminds.ebrains.eu/vocab/",
         "terms": "https://openminds.ebrains.eu/controlledTerms/",
         "core": "https://openminds.ebrains.eu/core/"
     }
     fields = [
-        Field("name", str, "vocab:name", multiple=False, required=True,
-              doc="Word or phrase that constitutes the distinctive designation of the numerical property."),
-        Field("values", ["openminds.core.QuantitativeValue", "openminds.core.QuantitativeValueRange"], "vocab:value", multiple=True, required=True,
-              doc="Entry for a property."),
+        Field("identifier", str, "vocab:identifier", multiple=False, required=True,
+              doc="Term or code used to identify the DOI."),
 
     ]
+    existence_query_fields = ('identifier',)
```

### Comparing `fairgraph-0.8.2/fairgraph/openminds/core/research/protocol_execution.py` & `fairgraph-0.9.0/fairgraph/openminds/ephys/activity/recording_activity.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,54 +1,58 @@
 """
-Structured information on a protocol execution.
+
 """
 
 # this file was auto-generated
 
 from datetime import date, datetime
 from fairgraph.base_v3 import KGObject, IRI
 from fairgraph.fields import Field
 
 
 
 
-class ProtocolExecution(KGObject):
+class RecordingActivity(KGObject):
     """
-    Structured information on a protocol execution.
+
     """
-    default_space = "dataset"
-    type = ["https://openminds.ebrains.eu/core/ProtocolExecution"]
+    default_space = "in-depth"
+    type = ["https://openminds.ebrains.eu/ephys/RecordingActivity"]
     context = {
         "schema": "http://schema.org/",
         "kg": "https://kg.ebrains.eu/api/instances/",
         "vocab": "https://openminds.ebrains.eu/vocab/",
         "terms": "https://openminds.ebrains.eu/controlledTerms/",
         "core": "https://openminds.ebrains.eu/core/"
     }
     fields = [
         Field("lookup_label", str, "vocab:lookupLabel", multiple=False, required=False,
               doc="no description available"),
-        Field("behavioral_protocols", "openminds.core.BehavioralProtocol", "vocab:behavioralProtocol", multiple=True, required=False,
-              doc="no description available"),
         Field("custom_property_sets", "openminds.core.CustomPropertySet", "vocab:customPropertySet", multiple=True, required=False,
               doc="no description available"),
         Field("description", str, "vocab:description", multiple=False, required=False,
-              doc="Longer statement or account giving the characteristics of the protocol execution."),
+              doc="Longer statement or account giving the characteristics of the recording activity."),
+        Field("devices", ["openminds.ephys.ElectrodeArrayUsage", "openminds.ephys.ElectrodeUsage", "openminds.ephys.PipetteUsage"], "vocab:device", multiple=True, required=False,
+              doc="Piece of equipment or mechanism (hardware) designed to serve a special purpose or perform a special function."),
         Field("ended_at_time", datetime, "vocab:endedAtTime", multiple=False, required=False,
               doc="no description available"),
-        Field("inputs", ["openminds.core.File", "openminds.core.FileBundle", "openminds.core.SubjectGroupState", "openminds.core.SubjectState", "openminds.core.TissueSampleCollectionState", "openminds.core.TissueSampleState"], "vocab:input", multiple=True, required=True,
+        Field("inputs", ["openminds.core.SubjectGroupState", "openminds.core.SubjectState", "openminds.core.TissueSampleCollectionState", "openminds.core.TissueSampleState"], "vocab:input", multiple=True, required=True,
               doc="Something or someone that is put into or participates in a process or machine."),
+        Field("internal_identifier", str, "vocab:internalIdentifier", multiple=False, required=False,
+              doc="Term or code that identifies the recording activity within a particular product."),
         Field("is_part_of", "openminds.core.DatasetVersion", "vocab:isPartOf", multiple=False, required=True,
               doc="Reference to the ensemble of multiple things or beings."),
-        Field("outputs", ["openminds.core.File", "openminds.core.FileBundle", "openminds.core.SubjectGroupState", "openminds.core.SubjectState", "openminds.core.TissueSampleCollectionState", "openminds.core.TissueSampleState"], "vocab:output", multiple=True, required=True,
+        Field("outputs", ["openminds.core.File", "openminds.core.FileBundle"], "vocab:output", multiple=True, required=True,
               doc="Something or someone that comes out of, is delivered or produced by a process or machine."),
+        Field("performed_by", ["openminds.computation.SoftwareAgent", "openminds.core.Person"], "vocab:performedBy", multiple=True, required=False,
+              doc="no description available"),
         Field("preparation_design", "openminds.controlledterms.PreparationType", "vocab:preparationDesign", multiple=False, required=False,
               doc="no description available"),
         Field("protocols", "openminds.core.Protocol", "vocab:protocol", multiple=True, required=True,
               doc="Plan that describes the process of a scientific or medical experiment, treatment, or procedure."),
         Field("started_at_time", datetime, "vocab:startedAtTime", multiple=False, required=False,
               doc="no description available"),
-        Field("study_targets", ["openminds.controlledterms.BiologicalOrder", "openminds.controlledterms.BiologicalSex", "openminds.controlledterms.BreedingType", "openminds.controlledterms.CellCultureType", "openminds.controlledterms.CellType", "openminds.controlledterms.Disease", "openminds.controlledterms.DiseaseModel", "openminds.controlledterms.GeneticStrainType", "openminds.controlledterms.Handedness", "openminds.controlledterms.MolecularEntity", "openminds.controlledterms.Organ", "openminds.controlledterms.Species", "openminds.controlledterms.SubcellularEntity", "openminds.controlledterms.TermSuggestion", "openminds.controlledterms.UBERONParcellation", "openminds.sands.CustomAnatomicalEntity", "openminds.sands.ParcellationEntity", "openminds.sands.ParcellationEntityVersion"], "vocab:studyTarget", multiple=True, required=False,
+        Field("study_targets", ["openminds.controlledterms.AuditoryStimulusType", "openminds.controlledterms.BiologicalOrder", "openminds.controlledterms.BiologicalSex", "openminds.controlledterms.BreedingType", "openminds.controlledterms.CellCultureType", "openminds.controlledterms.CellType", "openminds.controlledterms.Disease", "openminds.controlledterms.DiseaseModel", "openminds.controlledterms.ElectricalStimulusType", "openminds.controlledterms.GeneticStrainType", "openminds.controlledterms.GustatoryStimulusType", "openminds.controlledterms.Handedness", "openminds.controlledterms.MolecularEntity", "openminds.controlledterms.OlfactoryStimulusType", "openminds.controlledterms.OpticalStimulusType", "openminds.controlledterms.Organ", "openminds.controlledterms.Species", "openminds.controlledterms.SubcellularEntity", "openminds.controlledterms.TactileStimulusType", "openminds.controlledterms.TermSuggestion", "openminds.controlledterms.UBERONParcellation", "openminds.controlledterms.VisualStimulusType", "openminds.sands.CustomAnatomicalEntity", "openminds.sands.ParcellationEntity", "openminds.sands.ParcellationEntityVersion"], "vocab:studyTarget", multiple=True, required=False,
               doc="Structure or function that was targeted within a study."),
 
     ]
     existence_query_fields = ('lookup_label',)
```

### Comparing `fairgraph-0.8.2/fairgraph/openminds/core/research/subject.py` & `fairgraph-0.9.0/fairgraph/openminds/computation/workflow_execution.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,42 +1,36 @@
 """
-Structured information on a subject.
+Structured information about an execution of a computational workflow.
 """
 
 # this file was auto-generated
 
 from datetime import date, datetime
 from fairgraph.base_v3 import KGObject, IRI
 from fairgraph.fields import Field
 
 
 
 
-class Subject(KGObject):
+class WorkflowExecution(KGObject):
     """
-    Structured information on a subject.
+    Structured information about an execution of a computational workflow.
     """
-    default_space = "dataset"
-    type = ["https://openminds.ebrains.eu/core/Subject"]
+    default_space = "computation"
+    type = ["https://openminds.ebrains.eu/computation/WorkflowExecution"]
     context = {
         "schema": "http://schema.org/",
         "kg": "https://kg.ebrains.eu/api/instances/",
         "vocab": "https://openminds.ebrains.eu/vocab/",
         "terms": "https://openminds.ebrains.eu/controlledTerms/",
         "core": "https://openminds.ebrains.eu/core/"
     }
     fields = [
-        Field("lookup_label", str, "vocab:lookupLabel", multiple=False, required=False,
+        Field("recipe", "openminds.computation.WorkflowRecipeVersion", "vocab:recipe", multiple=False, required=False,
+              doc="no description available"),
+        Field("stages", ["openminds.computation.DataAnalysis", "openminds.computation.ModelValidation", "openminds.computation.Optimization", "openminds.computation.Simulation", "openminds.computation.Visualization"], "vocab:stages", multiple=True, required=True,
+              doc="no description available"),
+        Field("started_by", ["openminds.computation.SoftwareAgent", "openminds.core.Person"], "vocab:startedBy", multiple=False, required=False,
               doc="no description available"),
-        Field("biological_sex", "openminds.controlledterms.BiologicalSex", "vocab:biologicalSex", multiple=False, required=False,
-              doc="Differentiation of individuals of most species (animals and plants) based on the type of gametes they produce."),
-        Field("internal_identifier", str, "vocab:internalIdentifier", multiple=False, required=False,
-              doc="Term or code that identifies the subject within a particular product."),
-        Field("is_part_of", "openminds.core.SubjectGroup", "vocab:isPartOf", multiple=True, required=False,
-              doc="Reference to the ensemble of multiple things or beings."),
-        Field("species", ["openminds.controlledterms.Species", "openminds.core.Strain"], "vocab:species", multiple=False, required=True,
-              doc="Category of biological classification comprising related organisms or populations potentially capable of interbreeding, and being designated by a binomial that consists of the name of a genus followed by a Latin or latinized uncapitalized noun or adjective."),
-        Field("studied_states", "openminds.core.SubjectState", "vocab:studiedState", multiple=True, required=True,
-              doc="Reference to a point in time at which the subject was studied in a particular mode or condition."),
 
     ]
-    existence_query_fields = ('lookup_label',)
+    existence_query_fields = ('stages',)
```

### Comparing `fairgraph-0.8.2/fairgraph/openminds/core/research/subject_group.py` & `fairgraph-0.9.0/fairgraph/openminds/core/actors/affiliation.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,44 +1,34 @@
 """
-
+Structured information about a relationship between two entities, such as a person and their employer.
 """
 
 # this file was auto-generated
 
 from datetime import date, datetime
-from fairgraph.base_v3 import KGObject, IRI
+from fairgraph.base_v3 import EmbeddedMetadata, IRI
 from fairgraph.fields import Field
 
 
 
 
-class SubjectGroup(KGObject):
+class Affiliation(EmbeddedMetadata):
     """
-
+    Structured information about a relationship between two entities, such as a person and their employer.
     """
-    default_space = "dataset"
-    type = ["https://openminds.ebrains.eu/core/SubjectGroup"]
+    type = ["https://openminds.ebrains.eu/core/Affiliation"]
     context = {
         "schema": "http://schema.org/",
         "kg": "https://kg.ebrains.eu/api/instances/",
         "vocab": "https://openminds.ebrains.eu/vocab/",
         "terms": "https://openminds.ebrains.eu/controlledTerms/",
         "core": "https://openminds.ebrains.eu/core/"
     }
     fields = [
-        Field("lookup_label", str, "vocab:lookupLabel", multiple=False, required=False,
-              doc="no description available"),
-        Field("additional_remarks", str, "vocab:additionalRemarks", multiple=False, required=False,
-              doc="Mention of what deserves additional attention or notice."),
-        Field("biological_sex", "openminds.controlledterms.BiologicalSex", "vocab:biologicalSex", multiple=True, required=False,
-              doc="Differentiation of individuals of most species (animals and plants) based on the type of gametes they produce."),
-        Field("internal_identifier", str, "vocab:internalIdentifier", multiple=False, required=False,
-              doc="Term or code that identifies the subject group within a particular product."),
-        Field("quantity", int, "vocab:quantity", multiple=False, required=False,
-              doc="Total amount or number of things or beings."),
-        Field("species", ["openminds.controlledterms.Species", "openminds.core.Strain"], "vocab:species", multiple=True, required=True,
-              doc="Category of biological classification comprising related organisms or populations potentially capable of interbreeding, and being designated by a binomial that consists of the name of a genus followed by a Latin or latinized uncapitalized noun or adjective."),
-        Field("studied_states", "openminds.core.SubjectGroupState", "vocab:studiedState", multiple=True, required=True,
-              doc="Reference to a point in time at which the subject group was studied in a particular mode or condition."),
+        Field("end_date", date, "vocab:endDate", multiple=False, required=False,
+              doc="Date in the Gregorian calendar at which something terminates in time."),
+        Field("member_of", ["openminds.core.Consortium", "openminds.core.Organization"], "vocab:memberOf", multiple=False, required=False,
+              doc="no description available", alternate_path="vocab:organization"),
+        Field("start_date", date, "vocab:startDate", multiple=False, required=False,
+              doc="Date in the Gregorian calendar at which something begins in time"),
 
     ]
-    existence_query_fields = ('lookup_label',)
```

### Comparing `fairgraph-0.8.2/fairgraph/openminds/core/research/subject_group_state.py` & `fairgraph-0.9.0/fairgraph/openminds/core/research/subject_group_state.py`

 * *Files identical despite different names*

### Comparing `fairgraph-0.8.2/fairgraph/openminds/core/research/subject_state.py` & `fairgraph-0.9.0/fairgraph/openminds/core/research/subject_state.py`

 * *Files identical despite different names*

### Comparing `fairgraph-0.8.2/fairgraph/openminds/core/research/tissue_sample.py` & `fairgraph-0.9.0/fairgraph/openminds/controlledterms/action_status_type.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,50 +1,84 @@
 """
-Structured information on a tissue sample.
+The status of an action.
+
+    .. list-table:: **Possible values**
+       :widths: 20 80
+       :header-rows: 0
+
+       * - `active <https://schema.org/ActiveActionStatus>`_
+         - An in-progress action.
+       * - `completed <https://schema.org/CompletedActionStatus>`_
+         - An action that has already taken place with a successful outcome.
+       * - inactive
+         - A pending or suspended action.
+       * - `failed <https://schema.org/FailedActionStatus>`_
+         - An action that failed to complete or completed but produced an error.
+       * - paused
+         - A temporarily stopped action that can be resumed at a later point in time.
+       * - `potential <https://schema.org/PotentialActionStatus>`_
+         - A description of an action that is supported.
+       * - pending
+         - An action which is awaiting execution.
+
 """
 
 # this file was auto-generated
 
 from datetime import date, datetime
 from fairgraph.base_v3 import KGObject, IRI
 from fairgraph.fields import Field
 
 
 
 
-class TissueSample(KGObject):
+class ActionStatusType(KGObject):
     """
-    Structured information on a tissue sample.
+    The status of an action.
+
+    .. list-table:: **Possible values**
+       :widths: 20 80
+       :header-rows: 0
+
+       * - `active <https://schema.org/ActiveActionStatus>`_
+         - An in-progress action.
+       * - `completed <https://schema.org/CompletedActionStatus>`_
+         - An action that has already taken place with a successful outcome.
+       * - inactive
+         - A pending or suspended action.
+       * - `failed <https://schema.org/FailedActionStatus>`_
+         - An action that failed to complete or completed but produced an error.
+       * - paused
+         - A temporarily stopped action that can be resumed at a later point in time.
+       * - `potential <https://schema.org/PotentialActionStatus>`_
+         - A description of an action that is supported.
+       * - pending
+         - An action which is awaiting execution.
+
     """
-    default_space = "dataset"
-    type = ["https://openminds.ebrains.eu/core/TissueSample"]
+    default_space = "controlled"
+    type = ["https://openminds.ebrains.eu/controlledTerms/ActionStatusType"]
     context = {
         "schema": "http://schema.org/",
         "kg": "https://kg.ebrains.eu/api/instances/",
         "vocab": "https://openminds.ebrains.eu/vocab/",
         "terms": "https://openminds.ebrains.eu/controlledTerms/",
         "core": "https://openminds.ebrains.eu/core/"
     }
     fields = [
-        Field("lookup_label", str, "vocab:lookupLabel", multiple=False, required=False,
-              doc="no description available"),
-        Field("anatomical_locations", ["openminds.controlledterms.UBERONParcellation", "openminds.sands.CustomAnatomicalEntity", "openminds.sands.ParcellationEntity", "openminds.sands.ParcellationEntityVersion"], "vocab:anatomicalLocation", multiple=True, required=False,
-              doc="no description available"),
-        Field("biological_sex", "openminds.controlledterms.BiologicalSex", "vocab:biologicalSex", multiple=False, required=False,
-              doc="Differentiation of individuals of most species (animals and plants) based on the type of gametes they produce."),
-        Field("internal_identifier", str, "vocab:internalIdentifier", multiple=False, required=False,
-              doc="Term or code that identifies the tissue sample within a particular product."),
-        Field("is_part_of", "openminds.core.TissueSampleCollection", "vocab:isPartOf", multiple=True, required=False,
-              doc="Reference to the ensemble of multiple things or beings."),
-        Field("laterality", "openminds.controlledterms.Laterality", "vocab:laterality", multiple=True, required=False,
-              doc="Differentiation between a pair of lateral homologous parts of the body."),
-        Field("origin", ["openminds.controlledterms.CellType", "openminds.controlledterms.Organ"], "vocab:origin", multiple=False, required=True,
-              doc="Source at which something begins or rises, or from which something derives."),
-        Field("species", ["openminds.controlledterms.Species", "openminds.core.Strain"], "vocab:species", multiple=False, required=True,
-              doc="Category of biological classification comprising related organisms or populations potentially capable of interbreeding, and being designated by a binomial that consists of the name of a genus followed by a Latin or latinized uncapitalized noun or adjective."),
-        Field("studied_states", "openminds.core.TissueSampleState", "vocab:studiedState", multiple=True, required=True,
-              doc="Reference to a point in time at which the tissue sample was studied in a particular mode or condition."),
-        Field("type", "openminds.controlledterms.TissueSampleType", "vocab:type", multiple=False, required=True,
-              doc="Distinct class to which a group of entities or concepts with similar characteristics or attributes belong to."),
+        Field("name", str, "vocab:name", multiple=False, required=True,
+              doc="Word or phrase that constitutes the distinctive designation of the action status type."),
+        Field("definition", str, "vocab:definition", multiple=False, required=False,
+              doc="Short, but precise statement of the meaning of a word, word group, sign or a symbol."),
+        Field("description", str, "vocab:description", multiple=False, required=False,
+              doc="Longer statement or account giving the characteristics of the action status type."),
+        Field("interlex_identifier", IRI, "vocab:interlexIdentifier", multiple=False, required=False,
+              doc="Persistent identifier for a term registered in the InterLex project."),
+        Field("knowledge_space_link", IRI, "vocab:knowledgeSpaceLink", multiple=False, required=False,
+              doc="Persistent link to an encyclopedia entry in the Knowledge Space project."),
+        Field("preferred_ontology_identifier", IRI, "vocab:preferredOntologyIdentifier", multiple=False, required=False,
+              doc="Persistent identifier of a preferred ontological term."),
+        Field("synonyms", str, "vocab:synonym", multiple=True, required=False,
+              doc="Words or expressions used in the same language that have the same or nearly the same meaning in some or all senses."),
 
     ]
-    existence_query_fields = ('lookup_label',)
+    existence_query_fields = ('name',)
```

### Comparing `fairgraph-0.8.2/fairgraph/openminds/core/research/tissue_sample_collection.py` & `fairgraph-0.9.0/fairgraph/openminds/controlledterms/auditory_stimulus_type.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,52 +1,60 @@
 """
 
+
+    .. list-table:: **Possible values**
+       :widths: 20 80
+       :header-rows: 0
+
+       * - real spoken word
+         - A speech sound or series of speech sounds that symbolizes and communicates a meaning (usually) without being divisible into smaller units capable of independent use. [adapted from [Merriam-Webster](https://www.merriam-webster.com/dictionary/word)]
+
 """
 
 # this file was auto-generated
 
 from datetime import date, datetime
 from fairgraph.base_v3 import KGObject, IRI
 from fairgraph.fields import Field
 
 
 
 
-class TissueSampleCollection(KGObject):
+class AuditoryStimulusType(KGObject):
     """
 
+
+    .. list-table:: **Possible values**
+       :widths: 20 80
+       :header-rows: 0
+
+       * - real spoken word
+         - A speech sound or series of speech sounds that symbolizes and communicates a meaning (usually) without being divisible into smaller units capable of independent use. [adapted from [Merriam-Webster](https://www.merriam-webster.com/dictionary/word)]
+
     """
-    default_space = "dataset"
-    type = ["https://openminds.ebrains.eu/core/TissueSampleCollection"]
+    default_space = "controlled"
+    type = ["https://openminds.ebrains.eu/controlledTerms/AuditoryStimulusType"]
     context = {
         "schema": "http://schema.org/",
         "kg": "https://kg.ebrains.eu/api/instances/",
         "vocab": "https://openminds.ebrains.eu/vocab/",
         "terms": "https://openminds.ebrains.eu/controlledTerms/",
         "core": "https://openminds.ebrains.eu/core/"
     }
     fields = [
-        Field("lookup_label", str, "vocab:lookupLabel", multiple=False, required=False,
-              doc="no description available"),
-        Field("additional_remarks", str, "vocab:additionalRemarks", multiple=False, required=False,
-              doc="Mention of what deserves additional attention or notice."),
-        Field("anatomical_locations", ["openminds.controlledterms.UBERONParcellation", "openminds.sands.CustomAnatomicalEntity", "openminds.sands.ParcellationEntity", "openminds.sands.ParcellationEntityVersion"], "vocab:anatomicalLocation", multiple=True, required=False,
-              doc="no description available"),
-        Field("biological_sex", "openminds.controlledterms.BiologicalSex", "vocab:biologicalSex", multiple=True, required=False,
-              doc="Differentiation of individuals of most species (animals and plants) based on the type of gametes they produce."),
-        Field("internal_identifier", str, "vocab:internalIdentifier", multiple=False, required=False,
-              doc="Term or code that identifies the tissue sample collection within a particular product."),
-        Field("laterality", "openminds.controlledterms.Laterality", "vocab:laterality", multiple=True, required=False,
-              doc="Differentiation between a pair of lateral homologous parts of the body."),
-        Field("origins", ["openminds.controlledterms.CellType", "openminds.controlledterms.Organ"], "vocab:origin", multiple=True, required=True,
-              doc="Source at which something begins or rises, or from which something derives."),
-        Field("quantity", int, "vocab:quantity", multiple=False, required=False,
-              doc="Total amount or number of things or beings."),
-        Field("species", ["openminds.controlledterms.Species", "openminds.core.Strain"], "vocab:species", multiple=True, required=True,
-              doc="Category of biological classification comprising related organisms or populations potentially capable of interbreeding, and being designated by a binomial that consists of the name of a genus followed by a Latin or latinized uncapitalized noun or adjective."),
-        Field("studied_states", "openminds.core.TissueSampleCollectionState", "vocab:studiedState", multiple=True, required=True,
-              doc="Reference to a point in time at which the tissue sample collection was studied in a particular mode or condition."),
-        Field("types", "openminds.controlledterms.TissueSampleType", "vocab:type", multiple=True, required=True,
-              doc="Distinct class to which a group of entities or concepts with similar characteristics or attributes belong to."),
+        Field("name", str, "vocab:name", multiple=False, required=True,
+              doc="Word or phrase that constitutes the distinctive designation of the auditory stimulus type."),
+        Field("definition", str, "vocab:definition", multiple=False, required=False,
+              doc="Short, but precise statement of the meaning of a word, word group, sign or a symbol."),
+        Field("description", str, "vocab:description", multiple=False, required=False,
+              doc="Longer statement or account giving the characteristics of the auditory stimulus type."),
+        Field("interlex_identifier", IRI, "vocab:interlexIdentifier", multiple=False, required=False,
+              doc="Persistent identifier for a term registered in the InterLex project."),
+        Field("knowledge_space_link", IRI, "vocab:knowledgeSpaceLink", multiple=False, required=False,
+              doc="Persistent link to an encyclopedia entry in the Knowledge Space project."),
+        Field("preferred_ontology_identifier", IRI, "vocab:preferredOntologyIdentifier", multiple=False, required=False,
+              doc="Persistent identifier of a preferred ontological term."),
+        Field("synonyms", str, "vocab:synonym", multiple=True, required=False,
+              doc="Words or expressions used in the same language that have the same or nearly the same meaning in some or all senses."),
 
     ]
-    existence_query_fields = ('lookup_label',)
+    existence_query_fields = ('name',)
```

### Comparing `fairgraph-0.8.2/fairgraph/openminds/ephys/__init__.py` & `fairgraph-0.9.0/fairgraph/openminds/ephys/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import sys
 import inspect
 from ...base_v3 import KGObject
 
 from .activity.recording_activity import RecordingActivity
+from .activity.electrode_placement import ElectrodePlacement
 from .activity.cell_patching import CellPatching
 from .entity.channel import Channel
 from .entity.recording import Recording
 from .device.electrode_array import ElectrodeArray
 from .device.pipette_usage import PipetteUsage
 from .device.pipette import Pipette
 from .device.electrode import Electrode
```

### Comparing `fairgraph-0.8.2/fairgraph/openminds/ephys/activity/cell_patching.py` & `fairgraph-0.9.0/fairgraph/openminds/publications/book.py`

 * *Files 18% similar despite different names*

```diff
@@ -7,58 +7,58 @@
 from datetime import date, datetime
 from fairgraph.base_v3 import KGObject, IRI
 from fairgraph.fields import Field
 
 
 
 
-class CellPatching(KGObject):
+class Book(KGObject):
     """
 
     """
-    default_space = "electrophysiology"
-    type = ["https://openminds.ebrains.eu/ephys/CellPatching"]
+    default_space = "livepapers"
+    type = ["https://openminds.ebrains.eu/publications/Book"]
     context = {
         "schema": "http://schema.org/",
         "kg": "https://kg.ebrains.eu/api/instances/",
         "vocab": "https://openminds.ebrains.eu/vocab/",
         "terms": "https://openminds.ebrains.eu/controlledTerms/",
         "core": "https://openminds.ebrains.eu/core/"
     }
     fields = [
-        Field("lookup_label", str, "vocab:lookupLabel", multiple=False, required=False,
-              doc="no description available"),
-        Field("bath_temperature", ["openminds.core.QuantitativeValue", "openminds.core.QuantitativeValueRange"], "vocab:bathTemperature", multiple=False, required=False,
-              doc="no description available"),
-        Field("custom_property_sets", "openminds.core.CustomPropertySet", "vocab:customPropertySet", multiple=True, required=False,
-              doc="no description available"),
-        Field("description", str, "vocab:description", multiple=False, required=False,
-              doc="Longer statement or account giving the characteristics of the cell patching."),
-        Field("devices", ["openminds.ephys.ElectrodeArrayUsage", "openminds.ephys.ElectrodeUsage", "openminds.ephys.PipetteUsage"], "vocab:device", multiple=True, required=True,
-              doc="Piece of equipment or mechanism (hardware) designed to serve a special purpose or perform a special function."),
-        Field("ended_at_time", datetime, "vocab:endedAtTime", multiple=False, required=False,
-              doc="no description available"),
-        Field("inputs", ["openminds.core.SubjectState", "openminds.core.TissueSampleState"], "vocab:input", multiple=True, required=True,
-              doc="Something or someone that is put into or participates in a process or machine."),
-        Field("is_part_of", "openminds.core.DatasetVersion", "vocab:isPartOf", multiple=False, required=True,
-              doc="Reference to the ensemble of multiple things or beings."),
-        Field("outputs", "openminds.core.TissueSampleState", "vocab:output", multiple=True, required=True,
-              doc="Something or someone that comes out of, is delivered or produced by a process or machine."),
-        Field("preparation_design", "openminds.controlledterms.PreparationType", "vocab:preparationDesign", multiple=False, required=False,
-              doc="no description available"),
-        Field("protocols", "openminds.core.Protocol", "vocab:protocol", multiple=True, required=True,
-              doc="Plan that describes the process of a scientific or medical experiment, treatment, or procedure."),
-        Field("setup", "openminds.core.Setup", "vocab:setup", multiple=False, required=False,
-              doc="no description available"),
-        Field("started_at_time", datetime, "vocab:startedAtTime", multiple=False, required=False,
-              doc="no description available"),
-        Field("study_targets", ["openminds.controlledterms.BiologicalOrder", "openminds.controlledterms.BiologicalSex", "openminds.controlledterms.BreedingType", "openminds.controlledterms.CellCultureType", "openminds.controlledterms.CellType", "openminds.controlledterms.Disease", "openminds.controlledterms.DiseaseModel", "openminds.controlledterms.GeneticStrainType", "openminds.controlledterms.Handedness", "openminds.controlledterms.MolecularEntity", "openminds.controlledterms.Organ", "openminds.controlledterms.Species", "openminds.controlledterms.SubcellularEntity", "openminds.controlledterms.TermSuggestion", "openminds.controlledterms.UBERONParcellation", "openminds.sands.CustomAnatomicalEntity", "openminds.sands.ParcellationEntity", "openminds.sands.ParcellationEntityVersion"], "vocab:studyTarget", multiple=True, required=False,
-              doc="Structure or function that was targeted within a study."),
-        Field("target_position", "openminds.sands.AnatomicalTargetPosition", "vocab:targetPosition", multiple=False, required=False,
-              doc="no description available"),
-        Field("tissue_bath_solution", "openminds.chemicals.ChemicalMixture", "vocab:tissueBathSolution", multiple=False, required=False,
-              doc="no description available"),
-        Field("variation", "openminds.controlledterms.PatchClampVariation", "vocab:variation", multiple=False, required=False,
+        Field("name", str, "vocab:name", multiple=False, required=True,
+              doc="Word or phrase that constitutes the distinctive designation of the book."),
+        Field("iri", IRI, "vocab:IRI", multiple=False, required=False,
+              doc="Stands for Internationalized Resource Identifier which is an internet protocol standard that builds on the URI protocol, extending the set of permitted characters to include Unicode/ISO 10646."),
+        Field("abstract", str, "vocab:abstract", multiple=False, required=False,
+              doc="no description available"),
+        Field("authors", ["openminds.core.Consortium", "openminds.core.Organization", "openminds.core.Person"], "vocab:author", multiple=True, required=False,
+              doc="Creator of a literary or creative work, as well as a dataset publication."),
+        Field("cited_publications", ["openminds.core.DOI", "openminds.core.ISBN"], "vocab:citedPublication", multiple=True, required=False,
+              doc="no description available"),
+        Field("copyright", "openminds.core.Copyright", "vocab:copyright", multiple=False, required=False,
+              doc="Exclusive and assignable legal right of an originator to reproduce, publish, sell, or distribute the matter and form of a creative work for a defined time period."),
+        Field("custodians", ["openminds.core.Consortium", "openminds.core.Organization", "openminds.core.Person"], "vocab:custodian", multiple=True, required=False,
+              doc="The 'custodian' is a legal person who is responsible for the content and quality of the data, metadata, and/or code of a research product."),
+        Field("date_created", date, "vocab:dateCreated", multiple=False, required=False,
+              doc="no description available"),
+        Field("date_modified", date, "vocab:dateModified", multiple=False, required=False,
+              doc="no description available"),
+        Field("date_published", date, "vocab:datePublished", multiple=False, required=True,
+              doc="no description available"),
+        Field("digital_identifier", ["openminds.core.DOI", "openminds.core.ISBN"], "vocab:digitalIdentifier", multiple=False, required=False,
+              doc="Digital handle to identify objects or legal persons."),
+        Field("editors", "openminds.core.Person", "vocab:editor", multiple=True, required=False,
+              doc="no description available"),
+        Field("funding", "openminds.core.Funding", "vocab:funding", multiple=True, required=False,
+              doc="Money provided by a legal person for a particular purpose."),
+        Field("keywords", ["openminds.controlledterms.AuditoryStimulusType", "openminds.controlledterms.BiologicalOrder", "openminds.controlledterms.BiologicalSex", "openminds.controlledterms.BreedingType", "openminds.controlledterms.CellCultureType", "openminds.controlledterms.CellType", "openminds.controlledterms.Disease", "openminds.controlledterms.DiseaseModel", "openminds.controlledterms.ElectricalStimulusType", "openminds.controlledterms.GeneticStrainType", "openminds.controlledterms.GustatoryStimulusType", "openminds.controlledterms.Handedness", "openminds.controlledterms.MolecularEntity", "openminds.controlledterms.OlfactoryStimulusType", "openminds.controlledterms.OpticalStimulusType", "openminds.controlledterms.Organ", "openminds.controlledterms.Species", "openminds.controlledterms.SubcellularEntity", "openminds.controlledterms.TactileStimulusType", "openminds.controlledterms.TermSuggestion", "openminds.controlledterms.UBERONParcellation", "openminds.controlledterms.VisualStimulusType", "openminds.sands.CustomAnatomicalEntity", "openminds.sands.ParcellationEntity", "openminds.sands.ParcellationEntityVersion"], "vocab:keyword", multiple=True, required=False,
+              doc="Significant word or concept that are representative of the book."),
+        Field("license", "openminds.core.License", "vocab:license", multiple=False, required=False,
+              doc="Grant by a party to another party as an element of an agreement between those parties that permits to do, use, or own something."),
+        Field("publisher", ["openminds.core.Consortium", "openminds.core.Organization", "openminds.core.Person"], "vocab:publisher", multiple=False, required=False,
               doc="no description available"),
+        Field("version_identifier", str, "vocab:versionIdentifier", multiple=False, required=False,
+              doc="Term or code used to identify the version of something."),
 
     ]
-    existence_query_fields = ('lookup_label',)
+    existence_query_fields = ('name', 'date_published')
```

### Comparing `fairgraph-0.8.2/fairgraph/openminds/ephys/activity/electrode_placement.py` & `fairgraph-0.9.0/fairgraph/openminds/ephys/activity/cell_patching.py`

 * *Files 18% similar despite different names*

```diff
@@ -11,48 +11,54 @@
 
 
 
 class CellPatching(KGObject):
     """
 
     """
-    default_space = "electrophysiology"
+    default_space = "in-depth"
     type = ["https://openminds.ebrains.eu/ephys/CellPatching"]
     context = {
         "schema": "http://schema.org/",
         "kg": "https://kg.ebrains.eu/api/instances/",
         "vocab": "https://openminds.ebrains.eu/vocab/",
         "terms": "https://openminds.ebrains.eu/controlledTerms/",
         "core": "https://openminds.ebrains.eu/core/"
     }
     fields = [
         Field("lookup_label", str, "vocab:lookupLabel", multiple=False, required=False,
               doc="no description available"),
+        Field("bath_temperature", ["openminds.core.QuantitativeValue", "openminds.core.QuantitativeValueRange"], "vocab:bathTemperature", multiple=False, required=False,
+              doc="no description available"),
         Field("custom_property_sets", "openminds.core.CustomPropertySet", "vocab:customPropertySet", multiple=True, required=False,
               doc="no description available"),
         Field("description", str, "vocab:description", multiple=False, required=False,
               doc="Longer statement or account giving the characteristics of the cell patching."),
-        Field("devices", ["openminds.ephys.ElectrodeArrayUsage", "openminds.ephys.ElectrodeUsage", "openminds.ephys.PipetteUsage"], "vocab:device", multiple=True, required=True,
+        Field("devices", ["openminds.ephys.ElectrodeArrayUsage", "openminds.ephys.ElectrodeUsage", "openminds.ephys.PipetteUsage", "openminds.specimenprep.SlicingDeviceUsage"], "vocab:device", multiple=True, required=True,
               doc="Piece of equipment or mechanism (hardware) designed to serve a special purpose or perform a special function."),
         Field("ended_at_time", datetime, "vocab:endedAtTime", multiple=False, required=False,
               doc="no description available"),
         Field("inputs", ["openminds.core.SubjectState", "openminds.core.TissueSampleState"], "vocab:input", multiple=True, required=True,
               doc="Something or someone that is put into or participates in a process or machine."),
         Field("is_part_of", "openminds.core.DatasetVersion", "vocab:isPartOf", multiple=False, required=True,
               doc="Reference to the ensemble of multiple things or beings."),
-        Field("outputs", ["openminds.core.SubjectState", "openminds.core.TissueSampleState"], "vocab:output", multiple=True, required=True,
+        Field("outputs", "openminds.core.TissueSampleState", "vocab:output", multiple=True, required=True,
               doc="Something or someone that comes out of, is delivered or produced by a process or machine."),
+        Field("performed_by", ["openminds.computation.SoftwareAgent", "openminds.core.Person"], "vocab:performedBy", multiple=True, required=False,
+              doc="no description available"),
         Field("preparation_design", "openminds.controlledterms.PreparationType", "vocab:preparationDesign", multiple=False, required=False,
               doc="no description available"),
         Field("protocols", "openminds.core.Protocol", "vocab:protocol", multiple=True, required=True,
               doc="Plan that describes the process of a scientific or medical experiment, treatment, or procedure."),
-        Field("setup", "openminds.core.Setup", "vocab:setup", multiple=False, required=False,
-              doc="no description available"),
         Field("started_at_time", datetime, "vocab:startedAtTime", multiple=False, required=False,
               doc="no description available"),
-        Field("study_targets", ["openminds.controlledterms.BiologicalOrder", "openminds.controlledterms.BiologicalSex", "openminds.controlledterms.BreedingType", "openminds.controlledterms.CellCultureType", "openminds.controlledterms.CellType", "openminds.controlledterms.Disease", "openminds.controlledterms.DiseaseModel", "openminds.controlledterms.GeneticStrainType", "openminds.controlledterms.Handedness", "openminds.controlledterms.MolecularEntity", "openminds.controlledterms.Organ", "openminds.controlledterms.Species", "openminds.controlledterms.SubcellularEntity", "openminds.controlledterms.TermSuggestion", "openminds.controlledterms.UBERONParcellation", "openminds.sands.CustomAnatomicalEntity", "openminds.sands.ParcellationEntity", "openminds.sands.ParcellationEntityVersion"], "vocab:studyTarget", multiple=True, required=False,
+        Field("study_targets", ["openminds.controlledterms.AuditoryStimulusType", "openminds.controlledterms.BiologicalOrder", "openminds.controlledterms.BiologicalSex", "openminds.controlledterms.BreedingType", "openminds.controlledterms.CellCultureType", "openminds.controlledterms.CellType", "openminds.controlledterms.Disease", "openminds.controlledterms.DiseaseModel", "openminds.controlledterms.ElectricalStimulusType", "openminds.controlledterms.GeneticStrainType", "openminds.controlledterms.GustatoryStimulusType", "openminds.controlledterms.Handedness", "openminds.controlledterms.MolecularEntity", "openminds.controlledterms.OlfactoryStimulusType", "openminds.controlledterms.OpticalStimulusType", "openminds.controlledterms.Organ", "openminds.controlledterms.Species", "openminds.controlledterms.SubcellularEntity", "openminds.controlledterms.TactileStimulusType", "openminds.controlledterms.TermSuggestion", "openminds.controlledterms.UBERONParcellation", "openminds.controlledterms.VisualStimulusType", "openminds.sands.CustomAnatomicalEntity", "openminds.sands.ParcellationEntity", "openminds.sands.ParcellationEntityVersion"], "vocab:studyTarget", multiple=True, required=False,
               doc="Structure or function that was targeted within a study."),
         Field("target_position", "openminds.sands.AnatomicalTargetPosition", "vocab:targetPosition", multiple=False, required=False,
               doc="no description available"),
+        Field("tissue_bath_solution", "openminds.chemicals.ChemicalMixture", "vocab:tissueBathSolution", multiple=False, required=False,
+              doc="no description available"),
+        Field("variation", "openminds.controlledterms.PatchClampVariation", "vocab:variation", multiple=False, required=False,
+              doc="no description available"),
 
     ]
     existence_query_fields = ('lookup_label',)
```

### Comparing `fairgraph-0.8.2/fairgraph/openminds/ephys/activity/recording_activity.py` & `fairgraph-0.9.0/fairgraph/openminds/specimenprep/activity/tissue_culture_preparation.py`

 * *Files 23% similar despite different names*

```diff
@@ -7,50 +7,52 @@
 from datetime import date, datetime
 from fairgraph.base_v3 import KGObject, IRI
 from fairgraph.fields import Field
 
 
 
 
-class RecordingActivity(KGObject):
+class TissueCulturePreparation(KGObject):
     """
 
     """
-    default_space = "electrophysiology"
-    type = ["https://openminds.ebrains.eu/ephys/RecordingActivity"]
+    default_space = "in-depth"
+    type = ["https://openminds.ebrains.eu/specimenPrep/TissueCulturePreparation"]
     context = {
         "schema": "http://schema.org/",
         "kg": "https://kg.ebrains.eu/api/instances/",
         "vocab": "https://openminds.ebrains.eu/vocab/",
         "terms": "https://openminds.ebrains.eu/controlledTerms/",
         "core": "https://openminds.ebrains.eu/core/"
     }
     fields = [
         Field("lookup_label", str, "vocab:lookupLabel", multiple=False, required=False,
               doc="no description available"),
+        Field("culture_medium", "openminds.chemicals.ChemicalMixture", "vocab:cultureMedium", multiple=False, required=True,
+              doc="no description available"),
+        Field("culture_type", "openminds.controlledterms.CellCultureType", "vocab:cultureType", multiple=False, required=True,
+              doc="no description available"),
         Field("custom_property_sets", "openminds.core.CustomPropertySet", "vocab:customPropertySet", multiple=True, required=False,
               doc="no description available"),
         Field("description", str, "vocab:description", multiple=False, required=False,
-              doc="Longer statement or account giving the characteristics of the recording activity."),
+              doc="Longer statement or account giving the characteristics of the tissue culture preparation."),
         Field("ended_at_time", datetime, "vocab:endedAtTime", multiple=False, required=False,
               doc="no description available"),
         Field("inputs", ["openminds.core.SubjectGroupState", "openminds.core.SubjectState", "openminds.core.TissueSampleCollectionState", "openminds.core.TissueSampleState"], "vocab:input", multiple=True, required=True,
               doc="Something or someone that is put into or participates in a process or machine."),
-        Field("internal_identifier", str, "vocab:internalIdentifier", multiple=False, required=False,
-              doc="Term or code that identifies the recording activity within a particular product."),
         Field("is_part_of", "openminds.core.DatasetVersion", "vocab:isPartOf", multiple=False, required=True,
               doc="Reference to the ensemble of multiple things or beings."),
-        Field("outputs", ["openminds.core.File", "openminds.core.FileBundle"], "vocab:output", multiple=True, required=True,
+        Field("outputs", "openminds.core.TissueSampleState", "vocab:output", multiple=True, required=True,
               doc="Something or someone that comes out of, is delivered or produced by a process or machine."),
+        Field("performed_by", ["openminds.computation.SoftwareAgent", "openminds.core.Person"], "vocab:performedBy", multiple=True, required=False,
+              doc="no description available"),
         Field("preparation_design", "openminds.controlledterms.PreparationType", "vocab:preparationDesign", multiple=False, required=False,
               doc="no description available"),
         Field("protocols", "openminds.core.Protocol", "vocab:protocol", multiple=True, required=True,
               doc="Plan that describes the process of a scientific or medical experiment, treatment, or procedure."),
         Field("started_at_time", datetime, "vocab:startedAtTime", multiple=False, required=False,
               doc="no description available"),
-        Field("stimulation", "openminds.stimulation.StimulationActivity", "vocab:stimulation", multiple=False, required=True,
-              doc="no description available"),
-        Field("study_targets", ["openminds.controlledterms.BiologicalOrder", "openminds.controlledterms.BiologicalSex", "openminds.controlledterms.BreedingType", "openminds.controlledterms.CellCultureType", "openminds.controlledterms.CellType", "openminds.controlledterms.Disease", "openminds.controlledterms.DiseaseModel", "openminds.controlledterms.GeneticStrainType", "openminds.controlledterms.Handedness", "openminds.controlledterms.MolecularEntity", "openminds.controlledterms.Organ", "openminds.controlledterms.Species", "openminds.controlledterms.SubcellularEntity", "openminds.controlledterms.TermSuggestion", "openminds.controlledterms.UBERONParcellation", "openminds.sands.CustomAnatomicalEntity", "openminds.sands.ParcellationEntity", "openminds.sands.ParcellationEntityVersion"], "vocab:studyTarget", multiple=True, required=False,
+        Field("study_targets", ["openminds.controlledterms.AuditoryStimulusType", "openminds.controlledterms.BiologicalOrder", "openminds.controlledterms.BiologicalSex", "openminds.controlledterms.BreedingType", "openminds.controlledterms.CellCultureType", "openminds.controlledterms.CellType", "openminds.controlledterms.Disease", "openminds.controlledterms.DiseaseModel", "openminds.controlledterms.ElectricalStimulusType", "openminds.controlledterms.GeneticStrainType", "openminds.controlledterms.GustatoryStimulusType", "openminds.controlledterms.Handedness", "openminds.controlledterms.MolecularEntity", "openminds.controlledterms.OlfactoryStimulusType", "openminds.controlledterms.OpticalStimulusType", "openminds.controlledterms.Organ", "openminds.controlledterms.Species", "openminds.controlledterms.SubcellularEntity", "openminds.controlledterms.TactileStimulusType", "openminds.controlledterms.TermSuggestion", "openminds.controlledterms.UBERONParcellation", "openminds.controlledterms.VisualStimulusType", "openminds.sands.CustomAnatomicalEntity", "openminds.sands.ParcellationEntity", "openminds.sands.ParcellationEntityVersion"], "vocab:studyTarget", multiple=True, required=False,
               doc="Structure or function that was targeted within a study."),
 
     ]
     existence_query_fields = ('lookup_label',)
```

### Comparing `fairgraph-0.8.2/fairgraph/openminds/ephys/device/pipette_usage.py` & `fairgraph-0.9.0/fairgraph/openminds/ephys/device/pipette_usage.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 
 
 class PipetteUsage(KGObject):
     """
 
     """
-    default_space = "electrophysiology"
+    default_space = "in-depth"
     type = ["https://openminds.ebrains.eu/ephys/PipetteUsage"]
     context = {
         "schema": "http://schema.org/",
         "kg": "https://kg.ebrains.eu/api/instances/",
         "vocab": "https://openminds.ebrains.eu/vocab/",
         "terms": "https://openminds.ebrains.eu/controlledTerms/",
         "core": "https://openminds.ebrains.eu/core/"
```

### Comparing `fairgraph-0.8.2/fairgraph/openminds/publications/__init__.py` & `fairgraph-0.9.0/fairgraph/openminds/publications/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from .publication_issue import PublicationIssue
 from .book import Book
 from .live_paper_section import LivePaperSection
 from .periodical import Periodical
 from .chapter import Chapter
 from .live_paper_version import LivePaperVersion
 from .publication_volume import PublicationVolume
+from .learning_resource import LearningResource
 from .live_paper_resource_item import LivePaperResourceItem
 from .live_paper import LivePaper
 from .scholarly_article import ScholarlyArticle
 
 
 def list_kg_classes():
     """List all KG classes defined in this module"""
```

### Comparing `fairgraph-0.8.2/fairgraph/openminds/publications/book.py` & `fairgraph-0.9.0/fairgraph/openminds/publications/scholarly_article.py`

 * *Files 24% similar despite different names*

```diff
@@ -4,61 +4,109 @@
 
 # this file was auto-generated
 
 from datetime import date, datetime
 from fairgraph.base_v3 import KGObject, IRI
 from fairgraph.fields import Field
 
+from fairgraph.base_v3 import as_list
+from .publication_issue import PublicationIssue
+from .periodical import Periodical
 
 
-
-class Book(KGObject):
+class ScholarlyArticle(KGObject):
     """
 
     """
     default_space = "livepapers"
-    type = ["https://openminds.ebrains.eu/publications/Book"]
+    type = ["https://openminds.ebrains.eu/publications/ScholarlyArticle"]
     context = {
         "schema": "http://schema.org/",
         "kg": "https://kg.ebrains.eu/api/instances/",
         "vocab": "https://openminds.ebrains.eu/vocab/",
         "terms": "https://openminds.ebrains.eu/controlledTerms/",
         "core": "https://openminds.ebrains.eu/core/"
     }
     fields = [
         Field("name", str, "vocab:name", multiple=False, required=True,
-              doc="Word or phrase that constitutes the distinctive designation of the book."),
+              doc="Word or phrase that constitutes the distinctive designation of the scholarly article."),
         Field("iri", IRI, "vocab:IRI", multiple=False, required=False,
               doc="Stands for Internationalized Resource Identifier which is an internet protocol standard that builds on the URI protocol, extending the set of permitted characters to include Unicode/ISO 10646."),
         Field("abstract", str, "vocab:abstract", multiple=False, required=False,
               doc="no description available"),
-        Field("authors", ["openminds.core.Organization", "openminds.core.Person"], "vocab:author", multiple=True, required=False,
+        Field("authors", ["openminds.core.Consortium", "openminds.core.Organization", "openminds.core.Person"], "vocab:author", multiple=True, required=True,
               doc="Creator of a literary or creative work, as well as a dataset publication."),
         Field("cited_publications", ["openminds.core.DOI", "openminds.core.ISBN"], "vocab:citedPublication", multiple=True, required=False,
               doc="no description available"),
         Field("copyright", "openminds.core.Copyright", "vocab:copyright", multiple=False, required=False,
               doc="Exclusive and assignable legal right of an originator to reproduce, publish, sell, or distribute the matter and form of a creative work for a defined time period."),
-        Field("custodians", ["openminds.core.Organization", "openminds.core.Person"], "vocab:custodian", multiple=True, required=False,
+        Field("custodians", ["openminds.core.Consortium", "openminds.core.Organization", "openminds.core.Person"], "vocab:custodian", multiple=True, required=False,
               doc="The 'custodian' is a legal person who is responsible for the content and quality of the data, metadata, and/or code of a research product."),
         Field("date_created", date, "vocab:dateCreated", multiple=False, required=False,
               doc="no description available"),
         Field("date_modified", date, "vocab:dateModified", multiple=False, required=False,
               doc="no description available"),
         Field("date_published", date, "vocab:datePublished", multiple=False, required=True,
               doc="no description available"),
-        Field("digital_identifier", ["openminds.core.DOI", "openminds.core.ISBN"], "vocab:digitalIdentifier", multiple=False, required=False,
+        Field("digital_identifier", "openminds.core.DOI", "vocab:digitalIdentifier", multiple=False, required=False,
               doc="Digital handle to identify objects or legal persons."),
         Field("editors", "openminds.core.Person", "vocab:editor", multiple=True, required=False,
               doc="no description available"),
         Field("funding", "openminds.core.Funding", "vocab:funding", multiple=True, required=False,
               doc="Money provided by a legal person for a particular purpose."),
-        Field("keywords", ["openminds.controlledterms.BiologicalOrder", "openminds.controlledterms.BiologicalSex", "openminds.controlledterms.BreedingType", "openminds.controlledterms.CellCultureType", "openminds.controlledterms.CellType", "openminds.controlledterms.Disease", "openminds.controlledterms.DiseaseModel", "openminds.controlledterms.GeneticStrainType", "openminds.controlledterms.Handedness", "openminds.controlledterms.MolecularEntity", "openminds.controlledterms.Organ", "openminds.controlledterms.Species", "openminds.controlledterms.SubcellularEntity", "openminds.controlledterms.TermSuggestion", "openminds.controlledterms.UBERONParcellation", "openminds.sands.CustomAnatomicalEntity", "openminds.sands.ParcellationEntity", "openminds.sands.ParcellationEntityVersion"], "vocab:keyword", multiple=True, required=False,
-              doc="Significant word or concept that are representative of the book."),
+        Field("is_part_of", ["openminds.publications.PublicationIssue", "openminds.publications.PublicationVolume"], "vocab:isPartOf", multiple=False, required=True,
+              doc="Reference to the ensemble of multiple things or beings."),
+        Field("keywords", ["openminds.controlledterms.AuditoryStimulusType", "openminds.controlledterms.BiologicalOrder", "openminds.controlledterms.BiologicalSex", "openminds.controlledterms.BreedingType", "openminds.controlledterms.CellCultureType", "openminds.controlledterms.CellType", "openminds.controlledterms.Disease", "openminds.controlledterms.DiseaseModel", "openminds.controlledterms.ElectricalStimulusType", "openminds.controlledterms.GeneticStrainType", "openminds.controlledterms.GustatoryStimulusType", "openminds.controlledterms.Handedness", "openminds.controlledterms.MolecularEntity", "openminds.controlledterms.OlfactoryStimulusType", "openminds.controlledterms.OpticalStimulusType", "openminds.controlledterms.Organ", "openminds.controlledterms.Species", "openminds.controlledterms.SubcellularEntity", "openminds.controlledterms.TactileStimulusType", "openminds.controlledterms.TermSuggestion", "openminds.controlledterms.UBERONParcellation", "openminds.controlledterms.VisualStimulusType", "openminds.sands.CustomAnatomicalEntity", "openminds.sands.ParcellationEntity", "openminds.sands.ParcellationEntityVersion"], "vocab:keyword", multiple=True, required=False,
+              doc="Significant word or concept that are representative of the scholarly article."),
         Field("license", "openminds.core.License", "vocab:license", multiple=False, required=False,
               doc="Grant by a party to another party as an element of an agreement between those parties that permits to do, use, or own something."),
-        Field("publisher", ["openminds.core.Organization", "openminds.core.Person"], "vocab:publisher", multiple=False, required=False,
+        Field("pagination", str, "vocab:pagination", multiple=False, required=False,
+              doc="no description available"),
+        Field("publisher", ["openminds.core.Consortium", "openminds.core.Organization", "openminds.core.Person"], "vocab:publisher", multiple=False, required=False,
               doc="no description available"),
         Field("version_identifier", str, "vocab:versionIdentifier", multiple=False, required=False,
               doc="Term or code used to identify the version of something."),
 
     ]
-    existence_query_fields = ('name', 'date_published')
+    existence_query_fields = ('name',)
+
+    def get_journal(self, client, with_volume=False, with_issue=False):
+        journal = volume = issue = None
+        if self.is_part_of:
+            issue_or_volume = self.is_part_of.resolve(client, scope=self.scope, follow_links=1)
+            if isinstance(issue_or_volume, PublicationIssue):
+                volume = issue_or_volume.is_part_of
+                issue = issue_or_volume
+            else:
+                volume = issue_or_volume
+                issue = None
+            journal = volume.is_part_of
+            assert isinstance(journal, Periodical)
+        retval = [journal]
+        if with_volume:
+            retval.append(volume)
+        if with_issue:
+            retval.append(issue)
+        if not with_volume and not with_issue:
+            return journal
+        else:
+            return tuple(retval)
+
+    def get_citation_string(self, client):
+        #Eyal, G., Verhoog, M. B., Testa-Silva, G., Deitcher, Y., Lodder, '
+        #     -              'J. C., Benavides-Piccione, R., ... & Segev, I. (2016). Unique '
+        #     -              'membrane properties and enhanced signal processing in human '
+        #     -              'neocortical neurons. Elife, 5, e16553.
+        self.resolve(client, follow_links=1)
+        authors = as_list(self.authors)
+        if len(authors) == 1:
+            author_str = authors[0].full_name
+        elif len(authors) > 1:
+            author_str = ", ".join(au.full_name for au in authors[:-1])
+            author_str += " & " + self.authors[-1].full_name
+        journal, volume, issue = self.get_journal(client, with_volume=True, with_issue=True)
+        title = self.name
+        if title and title[-1] != ".":
+            title += "."
+        journal_name = journal.name if journal else ""
+        volume_number = volume.volume_number if volume else ""
+        return f"{author_str} ({self.date_published.year}). {title} {journal_name}, {volume_number}: {self.pagination}."
```

### Comparing `fairgraph-0.8.2/fairgraph/openminds/publications/chapter.py` & `fairgraph-0.9.0/fairgraph/openminds/publications/learning_resource.py`

 * *Files 20% similar despite different names*

```diff
@@ -7,62 +7,70 @@
 from datetime import date, datetime
 from fairgraph.base_v3 import KGObject, IRI
 from fairgraph.fields import Field
 
 
 
 
-class Chapter(KGObject):
+class LearningResource(KGObject):
     """
 
     """
     default_space = "livepapers"
-    type = ["https://openminds.ebrains.eu/publications/Chapter"]
+    type = ["https://openminds.ebrains.eu/publications/LearningResource"]
     context = {
         "schema": "http://schema.org/",
         "kg": "https://kg.ebrains.eu/api/instances/",
         "vocab": "https://openminds.ebrains.eu/vocab/",
         "terms": "https://openminds.ebrains.eu/controlledTerms/",
         "core": "https://openminds.ebrains.eu/core/"
     }
     fields = [
         Field("name", str, "vocab:name", multiple=False, required=True,
-              doc="Word or phrase that constitutes the distinctive designation of the chapter."),
+              doc="Word or phrase that constitutes the distinctive designation of the learning resource."),
         Field("iri", IRI, "vocab:IRI", multiple=False, required=False,
               doc="Stands for Internationalized Resource Identifier which is an internet protocol standard that builds on the URI protocol, extending the set of permitted characters to include Unicode/ISO 10646."),
+        Field("about", ["openminds.core.DatasetVersion", "openminds.core.MetaDataModelVersion", "openminds.core.ModelVersion", "openminds.core.SoftwareVersion", "openminds.core.WebServiceVersion"], "vocab:about", multiple=True, required=True,
+              doc="no description available"),
         Field("abstract", str, "vocab:abstract", multiple=False, required=False,
               doc="no description available"),
-        Field("authors", ["openminds.core.Organization", "openminds.core.Person"], "vocab:author", multiple=True, required=True,
+        Field("authors", ["openminds.core.Consortium", "openminds.core.Organization", "openminds.core.Person"], "vocab:author", multiple=True, required=False,
               doc="Creator of a literary or creative work, as well as a dataset publication."),
         Field("cited_publications", ["openminds.core.DOI", "openminds.core.ISBN"], "vocab:citedPublication", multiple=True, required=False,
               doc="no description available"),
+        Field("competency_required", str, "vocab:competencyRequired", multiple=False, required=False,
+              doc="no description available"),
         Field("copyright", "openminds.core.Copyright", "vocab:copyright", multiple=False, required=False,
               doc="Exclusive and assignable legal right of an originator to reproduce, publish, sell, or distribute the matter and form of a creative work for a defined time period."),
-        Field("custodians", ["openminds.core.Organization", "openminds.core.Person"], "vocab:custodian", multiple=True, required=False,
+        Field("custodians", ["openminds.core.Consortium", "openminds.core.Organization", "openminds.core.Person"], "vocab:custodian", multiple=True, required=False,
               doc="The 'custodian' is a legal person who is responsible for the content and quality of the data, metadata, and/or code of a research product."),
         Field("date_created", date, "vocab:dateCreated", multiple=False, required=False,
               doc="no description available"),
         Field("date_modified", date, "vocab:dateModified", multiple=False, required=False,
               doc="no description available"),
         Field("date_published", date, "vocab:datePublished", multiple=False, required=True,
               doc="no description available"),
         Field("digital_identifier", "openminds.core.DOI", "vocab:digitalIdentifier", multiple=False, required=False,
               doc="Digital handle to identify objects or legal persons."),
         Field("editors", "openminds.core.Person", "vocab:editor", multiple=True, required=False,
               doc="no description available"),
+        Field("educational_level", "openminds.controlledterms.EducationalLevel", "vocab:educationalLevel", multiple=False, required=False,
+              doc="no description available"),
         Field("funding", "openminds.core.Funding", "vocab:funding", multiple=True, required=False,
               doc="Money provided by a legal person for a particular purpose."),
-        Field("is_part_of", "openminds.publications.Book", "vocab:isPartOf", multiple=False, required=True,
-              doc="Reference to the ensemble of multiple things or beings."),
-        Field("keywords", ["openminds.controlledterms.BiologicalOrder", "openminds.controlledterms.BiologicalSex", "openminds.controlledterms.BreedingType", "openminds.controlledterms.CellCultureType", "openminds.controlledterms.CellType", "openminds.controlledterms.Disease", "openminds.controlledterms.DiseaseModel", "openminds.controlledterms.GeneticStrainType", "openminds.controlledterms.Handedness", "openminds.controlledterms.MolecularEntity", "openminds.controlledterms.Organ", "openminds.controlledterms.Species", "openminds.controlledterms.SubcellularEntity", "openminds.controlledterms.TermSuggestion", "openminds.controlledterms.UBERONParcellation", "openminds.sands.CustomAnatomicalEntity", "openminds.sands.ParcellationEntity", "openminds.sands.ParcellationEntityVersion"], "vocab:keyword", multiple=True, required=False,
-              doc="Significant word or concept that are representative of the chapter."),
+        Field("keywords", ["openminds.controlledterms.AuditoryStimulusType", "openminds.controlledterms.BiologicalOrder", "openminds.controlledterms.BiologicalSex", "openminds.controlledterms.BreedingType", "openminds.controlledterms.CellCultureType", "openminds.controlledterms.CellType", "openminds.controlledterms.Disease", "openminds.controlledterms.DiseaseModel", "openminds.controlledterms.ElectricalStimulusType", "openminds.controlledterms.GeneticStrainType", "openminds.controlledterms.GustatoryStimulusType", "openminds.controlledterms.Handedness", "openminds.controlledterms.MolecularEntity", "openminds.controlledterms.OlfactoryStimulusType", "openminds.controlledterms.OpticalStimulusType", "openminds.controlledterms.Organ", "openminds.controlledterms.Species", "openminds.controlledterms.SubcellularEntity", "openminds.controlledterms.TactileStimulusType", "openminds.controlledterms.TermSuggestion", "openminds.controlledterms.UBERONParcellation", "openminds.controlledterms.VisualStimulusType", "openminds.sands.CustomAnatomicalEntity", "openminds.sands.ParcellationEntity", "openminds.sands.ParcellationEntityVersion"], "vocab:keyword", multiple=True, required=False,
+              doc="Significant word or concept that are representative of the learning resource."),
+        Field("learning_resource_type", "openminds.controlledterms.LearningResourceType", "vocab:learningResourceType", multiple=False, required=False,
+              doc="no description available"),
         Field("license", "openminds.core.License", "vocab:license", multiple=False, required=False,
               doc="Grant by a party to another party as an element of an agreement between those parties that permits to do, use, or own something."),
-        Field("pagination", str, "vocab:pagination", multiple=False, required=False,
+        Field("publisher", ["openminds.core.Consortium", "openminds.core.Organization", "openminds.core.Person"], "vocab:publisher", multiple=False, required=False,
+              doc="no description available"),
+        Field("teaches", str, "vocab:teaches", multiple=False, required=False,
               doc="no description available"),
-        Field("publisher", ["openminds.core.Organization", "openminds.core.Person"], "vocab:publisher", multiple=False, required=False,
+        Field("time_required", ["openminds.core.QuantitativeValue", "openminds.core.QuantitativeValueRange"], "vocab:timeRequired", multiple=False, required=False,
               doc="no description available"),
         Field("version_identifier", str, "vocab:versionIdentifier", multiple=False, required=False,
               doc="Term or code used to identify the version of something."),
 
     ]
-    existence_query_fields = ('name', 'authors', 'date_published', 'is_part_of')
+    existence_query_fields = ('name', 'about', 'date_published')
```

### Comparing `fairgraph-0.8.2/fairgraph/openminds/publications/live_paper_resource_item.py` & `fairgraph-0.9.0/fairgraph/openminds/sands/miscellaneous/quantitative_relation_assessment.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,38 +1,34 @@
 """
 
 """
 
 # this file was auto-generated
 
 from datetime import date, datetime
-from fairgraph.base_v3 import KGObject, IRI
+from fairgraph.base_v3 import EmbeddedMetadata, IRI
 from fairgraph.fields import Field
 
 
 
 
-class LivePaperResourceItem(KGObject):
+class QuantitativeRelationAssessment(EmbeddedMetadata):
     """
 
     """
-    default_space = "livepapers"
-    type = ["https://openminds.ebrains.eu/publications/LivePaperResourceItem"]
+    type = ["https://openminds.ebrains.eu/sands/QuantitativeRelationAssessment"]
     context = {
         "schema": "http://schema.org/",
         "kg": "https://kg.ebrains.eu/api/instances/",
         "vocab": "https://openminds.ebrains.eu/vocab/",
         "terms": "https://openminds.ebrains.eu/controlledTerms/",
         "core": "https://openminds.ebrains.eu/core/"
     }
     fields = [
-        Field("name", str, "vocab:name", multiple=False, required=True,
-              doc="Word or phrase that constitutes the distinctive designation of the live paper resource item."),
-        Field("iri", IRI, "vocab:IRI", multiple=False, required=True,
-              doc="Stands for Internationalized Resource Identifier which is an internet protocol standard that builds on the URI protocol, extending the set of permitted characters to include Unicode/ISO 10646."),
-        Field("hosted_by", "openminds.core.Organization", "vocab:hostedBy", multiple=False, required=True,
-              doc="Reference to an organization that provides facilities and services for something."),
-        Field("is_part_of", "openminds.publications.LivePaperSection", "vocab:isPartOf", multiple=False, required=True,
-              doc="Reference to the ensemble of multiple things or beings."),
+        Field("criteria", "openminds.core.ProtocolExecution", "vocab:criteria", multiple=False, required=False,
+              doc="Aspects or standards on which a judgement or decision is based."),
+        Field("in_relation_to", "openminds.sands.ParcellationEntityVersion", "vocab:inRelationTo", multiple=False, required=True,
+              doc="Reference to a related element."),
+        Field("quantitative_overlap", ["openminds.core.QuantitativeValue", "openminds.core.QuantitativeValueRange"], "vocab:quantitativeOverlap", multiple=False, required=True,
+              doc="Numerical characterization of how much two things occupy the same space."),
 
     ]
-    existence_query_fields = ('name', 'iri', 'hosted_by', 'is_part_of')
```

### Comparing `fairgraph-0.8.2/fairgraph/openminds/publications/live_paper_version.py` & `fairgraph-0.9.0/fairgraph/openminds/core/products/web_service_version.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,87 +3,86 @@
 """
 
 # this file was auto-generated
 
 from datetime import date, datetime
 from fairgraph.base_v3 import KGObject, IRI
 from fairgraph.fields import Field
-
 from fairgraph.errors import ResolutionFailure
-from .live_paper import LivePaper
+from .web_service import WebService
+
+
 
 
-class LivePaperVersion(KGObject):
+class WebServiceVersion(KGObject):
     """
 
     """
-    default_space = "livepapers"
-    type = ["https://openminds.ebrains.eu/publications/LivePaperVersion"]
+    default_space = "webservice"
+    type = ["https://openminds.ebrains.eu/core/WebServiceVersion"]
     context = {
         "schema": "http://schema.org/",
         "kg": "https://kg.ebrains.eu/api/instances/",
         "vocab": "https://openminds.ebrains.eu/vocab/",
         "terms": "https://openminds.ebrains.eu/controlledTerms/",
         "core": "https://openminds.ebrains.eu/core/"
     }
     fields = [
         Field("name", str, "vocab:fullName", multiple=False, required=False,
-              doc="Whole, non-abbreviated name of the live paper version."),
+              doc="Whole, non-abbreviated name of the web service version."),
         Field("alias", str, "vocab:shortName", multiple=False, required=True,
-              doc="Shortened or fully abbreviated name of the live paper version."),
-        Field("about", ["openminds.core.DatasetVersion", "openminds.core.ModelVersion", "openminds.core.SoftwareVersion"], "vocab:about", multiple=True, required=False,
-              doc="no description available"),
+              doc="Shortened or fully abbreviated name of the web service version."),
         Field("accessibility", "openminds.controlledterms.ProductAccessibility", "vocab:accessibility", multiple=False, required=True,
-              doc="Level to which something is accessible to the live paper version."),
-        Field("authors", ["openminds.core.Organization", "openminds.core.Person"], "vocab:author", multiple=True, required=False,
-              doc="Creator of a literary or creative work, as well as a dataset publication."),
+              doc="Level to which something is accessible to the web service version."),
         Field("copyright", "openminds.core.Copyright", "vocab:copyright", multiple=False, required=False,
               doc="Exclusive and assignable legal right of an originator to reproduce, publish, sell, or distribute the matter and form of a creative work for a defined time period."),
-        Field("custodians", ["openminds.core.Organization", "openminds.core.Person"], "vocab:custodian", multiple=True, required=False,
+        Field("custodians", ["openminds.core.Consortium", "openminds.core.Organization", "openminds.core.Person"], "vocab:custodian", multiple=True, required=False,
               doc="The 'custodian' is a legal person who is responsible for the content and quality of the data, metadata, and/or code of a research product."),
         Field("description", str, "vocab:description", multiple=False, required=False,
-              doc="Longer statement or account giving the characteristics of the live paper version."),
-        Field("digital_identifier", "openminds.core.DOI", "vocab:digitalIdentifier", multiple=False, required=True,
-              doc="Digital handle to identify objects or legal persons."),
+              doc="Longer statement or account giving the characteristics of the web service version."),
+        Field("developers", ["openminds.core.Consortium", "openminds.core.Organization", "openminds.core.Person"], "vocab:developer", multiple=True, required=False,
+              doc="Legal person that creates or improves products or services (e.g., software, applications, etc.)."),
         Field("full_documentation", ["openminds.core.DOI", "openminds.core.File", "openminds.core.URL"], "vocab:fullDocumentation", multiple=False, required=True,
               doc="Non-abridged instructions, comments, and information for using a particular product."),
         Field("funding", "openminds.core.Funding", "vocab:funding", multiple=True, required=False,
               doc="Money provided by a legal person for a particular purpose."),
+        Field("has_components", "openminds.core.SoftwareVersion", "vocab:hasComponent", multiple=True, required=False,
+              doc="Reference to an element of a collection."),
         Field("homepage", "openminds.core.URL", "vocab:homepage", multiple=False, required=False,
-              doc="Main website of the live paper version."),
+              doc="Main website of the web service version."),
         Field("how_to_cite", str, "vocab:howToCite", multiple=False, required=False,
               doc="Preferred format for citing a particular object or legal person."),
-        Field("is_alternative_version_of", "openminds.publications.LivePaperVersion", "vocab:isAlternativeVersionOf", multiple=True, required=False,
+        Field("input_formats", "openminds.core.ContentType", "vocab:inputFormat", multiple=True, required=False,
+              doc="Format of data that is put into a process or machine."),
+        Field("is_alternative_version_of", "openminds.core.WebServiceVersion", "vocab:isAlternativeVersionOf", multiple=True, required=False,
               doc="Reference to an original form where the essence was preserved, but presented in an alternative form."),
-        Field("is_new_version_of", "openminds.publications.LivePaperVersion", "vocab:isNewVersionOf", multiple=False, required=False,
+        Field("is_new_version_of", "openminds.core.WebServiceVersion", "vocab:isNewVersionOf", multiple=False, required=False,
               doc="Reference to a previous (potentially outdated) particular form of something."),
-        Field("keywords", ["openminds.controlledterms.ActionStatusType", "openminds.controlledterms.AgeCategory", "openminds.controlledterms.AnatomicalAxesOrientation", "openminds.controlledterms.AnatomicalPlane", "openminds.controlledterms.AnnotationType", "openminds.controlledterms.AtlasType", "openminds.controlledterms.BiologicalOrder", "openminds.controlledterms.BiologicalSex", "openminds.controlledterms.BreedingType", "openminds.controlledterms.CellCultureType", "openminds.controlledterms.CellType", "openminds.controlledterms.ChemicalMixtureType", "openminds.controlledterms.ContributionType", "openminds.controlledterms.CranialWindowType", "openminds.controlledterms.CriteriaQualityType", "openminds.controlledterms.DataType", "openminds.controlledterms.DeviceType", "openminds.controlledterms.DifferenceMeasure", "openminds.controlledterms.Disease", "openminds.controlledterms.DiseaseModel", "openminds.controlledterms.EthicsAssessment", "openminds.controlledterms.ExperimentalApproach", "openminds.controlledterms.FileBundleGrouping", "openminds.controlledterms.FileRepositoryType", "openminds.controlledterms.FileUsageRole", "openminds.controlledterms.GeneticStrainType", "openminds.controlledterms.Handedness", "openminds.controlledterms.Language", "openminds.controlledterms.Laterality", "openminds.controlledterms.MeasuredQuantity", "openminds.controlledterms.MetaDataModelType", "openminds.controlledterms.ModelAbstractionLevel", "openminds.controlledterms.ModelScope", "openminds.controlledterms.MolecularEntity", "openminds.controlledterms.OperatingDevice", "openminds.controlledterms.OperatingSystem", "openminds.controlledterms.Organ", "openminds.controlledterms.PatchClampVariation", "openminds.controlledterms.PreparationType", "openminds.controlledterms.ProductAccessibility", "openminds.controlledterms.ProgrammingLanguage", "openminds.controlledterms.QualitativeOverlap", "openminds.controlledterms.SemanticDataType", "openminds.controlledterms.Service", "openminds.controlledterms.SetupType", "openminds.controlledterms.SoftwareApplicationCategory", "openminds.controlledterms.SoftwareFeature", "openminds.controlledterms.Species", "openminds.controlledterms.StimulationApproach", "openminds.controlledterms.StimulusType", "openminds.controlledterms.SubcellularEntity", "openminds.controlledterms.SubjectAttribute", "openminds.controlledterms.Technique", "openminds.controlledterms.TermSuggestion", "openminds.controlledterms.Terminology", "openminds.controlledterms.TissueSampleAttribute", "openminds.controlledterms.TissueSampleType", "openminds.controlledterms.TypeOfUncertainty", "openminds.controlledterms.UBERONParcellation", "openminds.controlledterms.UnitOfMeasurement"], "vocab:keyword", multiple=True, required=False,
-              doc="Significant word or concept that are representative of the live paper version."),
-        Field("last_modified", datetime, "vocab:lastModified", multiple=False, required=False,
-              doc="no description available"),
-        Field("license", "openminds.core.License", "vocab:license", multiple=False, required=True,
-              doc="Grant by a party to another party as an element of an agreement between those parties that permits to do, use, or own something."),
+        Field("keywords", ["openminds.controlledterms.ActionStatusType", "openminds.controlledterms.AgeCategory", "openminds.controlledterms.AnatomicalAxesOrientation", "openminds.controlledterms.AnatomicalPlane", "openminds.controlledterms.AnnotationType", "openminds.controlledterms.AtlasType", "openminds.controlledterms.AuditoryStimulusType", "openminds.controlledterms.BiologicalOrder", "openminds.controlledterms.BiologicalSex", "openminds.controlledterms.BreedingType", "openminds.controlledterms.CellCultureType", "openminds.controlledterms.CellType", "openminds.controlledterms.ChemicalMixtureType", "openminds.controlledterms.ContributionType", "openminds.controlledterms.CranialWindowConstructionType", "openminds.controlledterms.CranialWindowReinforcementType", "openminds.controlledterms.CriteriaQualityType", "openminds.controlledterms.DataType", "openminds.controlledterms.DeviceType", "openminds.controlledterms.DifferenceMeasure", "openminds.controlledterms.Disease", "openminds.controlledterms.DiseaseModel", "openminds.controlledterms.EducationalLevel", "openminds.controlledterms.ElectricalStimulusType", "openminds.controlledterms.EthicsAssessment", "openminds.controlledterms.ExperimentalApproach", "openminds.controlledterms.FileBundleGrouping", "openminds.controlledterms.FileRepositoryType", "openminds.controlledterms.FileUsageRole", "openminds.controlledterms.GeneticStrainType", "openminds.controlledterms.GustatoryStimulusType", "openminds.controlledterms.Handedness", "openminds.controlledterms.Language", "openminds.controlledterms.Laterality", "openminds.controlledterms.LearningResourceType", "openminds.controlledterms.MeasuredQuantity", "openminds.controlledterms.MetaDataModelType", "openminds.controlledterms.ModelAbstractionLevel", "openminds.controlledterms.ModelScope", "openminds.controlledterms.MolecularEntity", "openminds.controlledterms.OlfactoryStimulusType", "openminds.controlledterms.OperatingDevice", "openminds.controlledterms.OperatingSystem", "openminds.controlledterms.OpticalStimulusType", "openminds.controlledterms.Organ", "openminds.controlledterms.PatchClampVariation", "openminds.controlledterms.PreparationType", "openminds.controlledterms.ProductAccessibility", "openminds.controlledterms.ProgrammingLanguage", "openminds.controlledterms.QualitativeOverlap", "openminds.controlledterms.SemanticDataType", "openminds.controlledterms.Service", "openminds.controlledterms.SetupType", "openminds.controlledterms.SoftwareApplicationCategory", "openminds.controlledterms.SoftwareFeature", "openminds.controlledterms.Species", "openminds.controlledterms.StimulationApproach", "openminds.controlledterms.StimulationTechnique", "openminds.controlledterms.SubcellularEntity", "openminds.controlledterms.SubjectAttribute", "openminds.controlledterms.TactileStimulusType", "openminds.controlledterms.Technique", "openminds.controlledterms.TermSuggestion", "openminds.controlledterms.Terminology", "openminds.controlledterms.TissueSampleAttribute", "openminds.controlledterms.TissueSampleType", "openminds.controlledterms.TypeOfUncertainty", "openminds.controlledterms.UBERONParcellation", "openminds.controlledterms.UnitOfMeasurement", "openminds.controlledterms.VisualStimulusType"], "vocab:keyword", multiple=True, required=False,
+              doc="Significant word or concept that are representative of the web service version."),
         Field("other_contributions", "openminds.core.Contribution", "vocab:otherContribution", multiple=True, required=False,
               doc="Giving or supplying of something (such as money or time) as a part or share other than what is covered elsewhere."),
-        Field("related_publications", ["openminds.core.DOI", "openminds.core.ISBN", "openminds.core.ISSN"], "vocab:relatedPublication", multiple=True, required=False,
+        Field("output_formats", "openminds.core.ContentType", "vocab:outputFormat", multiple=True, required=False,
+              doc="Format of data that comes out of, is delivered or produced by a process or machine."),
+        Field("related_publications", ["openminds.core.DOI", "openminds.core.HANDLE", "openminds.core.ISBN"], "vocab:relatedPublication", multiple=True, required=False,
               doc="Reference to something that was made available for the general public to see or buy."),
         Field("release_date", date, "vocab:releaseDate", multiple=False, required=True,
               doc="Fixed date on which a product is due to become or was made available for the general public to see or buy"),
         Field("repository", "openminds.core.FileRepository", "vocab:repository", multiple=False, required=False,
               doc="Place, room, or container where something is deposited or stored."),
         Field("support_channels", str, "vocab:supportChannel", multiple=True, required=False,
               doc="Way of communication used to interact with users or customers."),
         Field("version_identifier", str, "vocab:versionIdentifier", multiple=False, required=True,
               doc="Term or code used to identify the version of something."),
         Field("version_innovation", str, "vocab:versionInnovation", multiple=False, required=True,
               doc="Documentation on what changed in comparison to a previously published form of something."),
 
     ]
-    existence_query_fields = ('alias', 'version_identifier')
+    existence_query_fields = ('alias', 'accessibility', 'full_documentation', 'release_date', 'version_identifier', 'version_innovation')
 
     def is_version_of(self, client):
-        parents = LivePaper.list(client, scope=self.scope, space=self.space, versions=self)
+        parents = WebService.list(client, scope=self.scope, space=self.space, versions=self)
         if len(parents) == 0:
             raise ResolutionFailure("Unable to find parent")
         else:
             assert len(parents) == 1
-            return parents[0]
+            return parents[0]
```

### Comparing `fairgraph-0.8.2/fairgraph/openminds/publications/publication_issue.py` & `fairgraph-0.9.0/fairgraph/openminds/core/actors/account_information.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 """
-
+Structured information about a user account for a web service.
 """
 
 # this file was auto-generated
 
 from datetime import date, datetime
 from fairgraph.base_v3 import KGObject, IRI
 from fairgraph.fields import Field
 
 
 
 
-class PublicationIssue(KGObject):
+class AccountInformation(KGObject):
     """
-
+    Structured information about a user account for a web service.
     """
-    default_space = "livepapers"
-    type = ["https://openminds.ebrains.eu/publications/PublicationIssue"]
+    default_space = "common"
+    type = ["https://openminds.ebrains.eu/core/AccountInformation"]
     context = {
         "schema": "http://schema.org/",
         "kg": "https://kg.ebrains.eu/api/instances/",
         "vocab": "https://openminds.ebrains.eu/vocab/",
         "terms": "https://openminds.ebrains.eu/controlledTerms/",
         "core": "https://openminds.ebrains.eu/core/"
     }
     fields = [
-        Field("is_part_of", "openminds.publications.PublicationVolume", "vocab:isPartOf", multiple=False, required=True,
-              doc="Reference to the ensemble of multiple things or beings."),
-        Field("issue_number", str, "vocab:issueNumber", multiple=False, required=True,
+        Field("service", "openminds.core.WebService", "vocab:service", multiple=False, required=True,
+              doc="no description available"),
+        Field("user_name", str, "vocab:userName", multiple=False, required=True,
               doc="no description available"),
 
     ]
-    existence_query_fields = ('is_part_of', 'issue_number')
+    existence_query_fields = ('service', 'user_name')
```

### Comparing `fairgraph-0.8.2/fairgraph/openminds/sands/__init__.py` & `fairgraph-0.9.0/fairgraph/openminds/sands/__init__.py`

 * *Files identical despite different names*

### Comparing `fairgraph-0.8.2/fairgraph/openminds/sands/atlas/brain_atlas_version.py` & `fairgraph-0.9.0/fairgraph/openminds/core/products/meta_data_model_version.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,86 +1,82 @@
 """
-Structured information on a brain atlas (version level).
+
 """
 
 # this file was auto-generated
 
 from datetime import date, datetime
 from fairgraph.base_v3 import KGObject, IRI
 from fairgraph.fields import Field
 
 
 
 
-class BrainAtlasVersion(KGObject):
+class MetaDataModelVersion(KGObject):
     """
-    Structured information on a brain atlas (version level).
+
     """
-    default_space = "atlas"
-    type = ["https://openminds.ebrains.eu/sands/BrainAtlasVersion"]
+    default_space = "metadatamodel"
+    type = ["https://openminds.ebrains.eu/core/MetaDataModelVersion"]
     context = {
         "schema": "http://schema.org/",
         "kg": "https://kg.ebrains.eu/api/instances/",
         "vocab": "https://openminds.ebrains.eu/vocab/",
         "terms": "https://openminds.ebrains.eu/controlledTerms/",
         "core": "https://openminds.ebrains.eu/core/"
     }
     fields = [
         Field("name", str, "vocab:fullName", multiple=False, required=False,
-              doc="Whole, non-abbreviated name of the brain atlas version."),
+              doc="Whole, non-abbreviated name of the meta data model version."),
         Field("alias", str, "vocab:shortName", multiple=False, required=True,
-              doc="Shortened or fully abbreviated name of the brain atlas version."),
-        Field("abbreviation", str, "vocab:abbreviation", multiple=False, required=False,
-              doc="no description available"),
+              doc="Shortened or fully abbreviated name of the meta data model version."),
         Field("accessibility", "openminds.controlledterms.ProductAccessibility", "vocab:accessibility", multiple=False, required=True,
-              doc="Level to which something is accessible to the brain atlas version."),
-        Field("atlas_type", "openminds.controlledterms.AtlasType", "vocab:atlasType", multiple=False, required=False,
-              doc="no description available"),
-        Field("authors", ["openminds.core.Organization", "openminds.core.Person"], "vocab:author", multiple=True, required=False,
-              doc="Creator of a literary or creative work, as well as a dataset publication."),
-        Field("coordinate_space", "openminds.sands.CommonCoordinateSpace", "vocab:coordinateSpace", multiple=False, required=True,
-              doc="Two or three dimensional geometric setting."),
+              doc="Level to which something is accessible to the meta data model version."),
         Field("copyright", "openminds.core.Copyright", "vocab:copyright", multiple=False, required=False,
               doc="Exclusive and assignable legal right of an originator to reproduce, publish, sell, or distribute the matter and form of a creative work for a defined time period."),
-        Field("custodians", ["openminds.core.Organization", "openminds.core.Person"], "vocab:custodian", multiple=True, required=False,
+        Field("custodians", ["openminds.core.Consortium", "openminds.core.Organization", "openminds.core.Person"], "vocab:custodian", multiple=True, required=False,
               doc="The 'custodian' is a legal person who is responsible for the content and quality of the data, metadata, and/or code of a research product."),
         Field("description", str, "vocab:description", multiple=False, required=False,
-              doc="Longer statement or account giving the characteristics of the brain atlas version."),
-        Field("digital_identifier", ["openminds.core.DOI", "openminds.core.ISBN", "openminds.core.RRID"], "vocab:digitalIdentifier", multiple=False, required=False,
+              doc="Longer statement or account giving the characteristics of the meta data model version."),
+        Field("developers", ["openminds.core.Consortium", "openminds.core.Organization", "openminds.core.Person"], "vocab:developer", multiple=True, required=False,
+              doc="Legal person that creates or improves products or services (e.g., software, applications, etc.)."),
+        Field("digital_identifier", ["openminds.core.DOI", "openminds.core.SWHID"], "vocab:digitalIdentifier", multiple=False, required=False,
               doc="Digital handle to identify objects or legal persons."),
         Field("full_documentation", ["openminds.core.DOI", "openminds.core.File", "openminds.core.URL"], "vocab:fullDocumentation", multiple=False, required=True,
               doc="Non-abridged instructions, comments, and information for using a particular product."),
         Field("funding", "openminds.core.Funding", "vocab:funding", multiple=True, required=False,
               doc="Money provided by a legal person for a particular purpose."),
-        Field("has_terminology_version", "openminds.sands.ParcellationTerminologyVersion", "vocab:hasTerminologyVersion", multiple=False, required=True,
-              doc="no description available"),
         Field("homepage", "openminds.core.URL", "vocab:homepage", multiple=False, required=False,
-              doc="Main website of the brain atlas version."),
+              doc="Main website of the meta data model version."),
         Field("how_to_cite", str, "vocab:howToCite", multiple=False, required=False,
               doc="Preferred format for citing a particular object or legal person."),
-        Field("is_alternative_version_of", "openminds.sands.BrainAtlasVersion", "vocab:isAlternativeVersionOf", multiple=True, required=False,
+        Field("is_alternative_version_of", "openminds.core.MetaDataModelVersion", "vocab:isAlternativeVersionOf", multiple=True, required=False,
               doc="Reference to an original form where the essence was preserved, but presented in an alternative form."),
-        Field("is_new_version_of", "openminds.sands.BrainAtlasVersion", "vocab:isNewVersionOf", multiple=False, required=False,
+        Field("is_new_version_of", "openminds.core.MetaDataModelVersion", "vocab:isNewVersionOf", multiple=False, required=False,
               doc="Reference to a previous (potentially outdated) particular form of something."),
-        Field("keywords", ["openminds.controlledterms.ActionStatusType", "openminds.controlledterms.AgeCategory", "openminds.controlledterms.AnatomicalAxesOrientation", "openminds.controlledterms.AnatomicalPlane", "openminds.controlledterms.AnnotationType", "openminds.controlledterms.AtlasType", "openminds.controlledterms.BiologicalOrder", "openminds.controlledterms.BiologicalSex", "openminds.controlledterms.BreedingType", "openminds.controlledterms.CellCultureType", "openminds.controlledterms.CellType", "openminds.controlledterms.ChemicalMixtureType", "openminds.controlledterms.ContributionType", "openminds.controlledterms.CranialWindowType", "openminds.controlledterms.CriteriaQualityType", "openminds.controlledterms.DataType", "openminds.controlledterms.DeviceType", "openminds.controlledterms.DifferenceMeasure", "openminds.controlledterms.Disease", "openminds.controlledterms.DiseaseModel", "openminds.controlledterms.EthicsAssessment", "openminds.controlledterms.ExperimentalApproach", "openminds.controlledterms.FileBundleGrouping", "openminds.controlledterms.FileRepositoryType", "openminds.controlledterms.FileUsageRole", "openminds.controlledterms.GeneticStrainType", "openminds.controlledterms.Handedness", "openminds.controlledterms.Language", "openminds.controlledterms.Laterality", "openminds.controlledterms.MeasuredQuantity", "openminds.controlledterms.MetaDataModelType", "openminds.controlledterms.ModelAbstractionLevel", "openminds.controlledterms.ModelScope", "openminds.controlledterms.MolecularEntity", "openminds.controlledterms.OperatingDevice", "openminds.controlledterms.OperatingSystem", "openminds.controlledterms.Organ", "openminds.controlledterms.PatchClampVariation", "openminds.controlledterms.PreparationType", "openminds.controlledterms.ProductAccessibility", "openminds.controlledterms.ProgrammingLanguage", "openminds.controlledterms.QualitativeOverlap", "openminds.controlledterms.SemanticDataType", "openminds.controlledterms.Service", "openminds.controlledterms.SetupType", "openminds.controlledterms.SoftwareApplicationCategory", "openminds.controlledterms.SoftwareFeature", "openminds.controlledterms.Species", "openminds.controlledterms.StimulationApproach", "openminds.controlledterms.StimulusType", "openminds.controlledterms.SubcellularEntity", "openminds.controlledterms.SubjectAttribute", "openminds.controlledterms.Technique", "openminds.controlledterms.TermSuggestion", "openminds.controlledterms.Terminology", "openminds.controlledterms.TissueSampleAttribute", "openminds.controlledterms.TissueSampleType", "openminds.controlledterms.TypeOfUncertainty", "openminds.controlledterms.UBERONParcellation", "openminds.controlledterms.UnitOfMeasurement"], "vocab:keyword", multiple=True, required=False,
-              doc="Significant word or concept that are representative of the brain atlas version."),
+        Field("keywords", ["openminds.controlledterms.ActionStatusType", "openminds.controlledterms.AgeCategory", "openminds.controlledterms.AnatomicalAxesOrientation", "openminds.controlledterms.AnatomicalPlane", "openminds.controlledterms.AnnotationType", "openminds.controlledterms.AtlasType", "openminds.controlledterms.AuditoryStimulusType", "openminds.controlledterms.BiologicalOrder", "openminds.controlledterms.BiologicalSex", "openminds.controlledterms.BreedingType", "openminds.controlledterms.CellCultureType", "openminds.controlledterms.CellType", "openminds.controlledterms.ChemicalMixtureType", "openminds.controlledterms.ContributionType", "openminds.controlledterms.CranialWindowConstructionType", "openminds.controlledterms.CranialWindowReinforcementType", "openminds.controlledterms.CriteriaQualityType", "openminds.controlledterms.DataType", "openminds.controlledterms.DeviceType", "openminds.controlledterms.DifferenceMeasure", "openminds.controlledterms.Disease", "openminds.controlledterms.DiseaseModel", "openminds.controlledterms.EducationalLevel", "openminds.controlledterms.ElectricalStimulusType", "openminds.controlledterms.EthicsAssessment", "openminds.controlledterms.ExperimentalApproach", "openminds.controlledterms.FileBundleGrouping", "openminds.controlledterms.FileRepositoryType", "openminds.controlledterms.FileUsageRole", "openminds.controlledterms.GeneticStrainType", "openminds.controlledterms.GustatoryStimulusType", "openminds.controlledterms.Handedness", "openminds.controlledterms.Language", "openminds.controlledterms.Laterality", "openminds.controlledterms.LearningResourceType", "openminds.controlledterms.MeasuredQuantity", "openminds.controlledterms.MetaDataModelType", "openminds.controlledterms.ModelAbstractionLevel", "openminds.controlledterms.ModelScope", "openminds.controlledterms.MolecularEntity", "openminds.controlledterms.OlfactoryStimulusType", "openminds.controlledterms.OperatingDevice", "openminds.controlledterms.OperatingSystem", "openminds.controlledterms.OpticalStimulusType", "openminds.controlledterms.Organ", "openminds.controlledterms.PatchClampVariation", "openminds.controlledterms.PreparationType", "openminds.controlledterms.ProductAccessibility", "openminds.controlledterms.ProgrammingLanguage", "openminds.controlledterms.QualitativeOverlap", "openminds.controlledterms.SemanticDataType", "openminds.controlledterms.Service", "openminds.controlledterms.SetupType", "openminds.controlledterms.SoftwareApplicationCategory", "openminds.controlledterms.SoftwareFeature", "openminds.controlledterms.Species", "openminds.controlledterms.StimulationApproach", "openminds.controlledterms.StimulationTechnique", "openminds.controlledterms.SubcellularEntity", "openminds.controlledterms.SubjectAttribute", "openminds.controlledterms.TactileStimulusType", "openminds.controlledterms.Technique", "openminds.controlledterms.TermSuggestion", "openminds.controlledterms.Terminology", "openminds.controlledterms.TissueSampleAttribute", "openminds.controlledterms.TissueSampleType", "openminds.controlledterms.TypeOfUncertainty", "openminds.controlledterms.UBERONParcellation", "openminds.controlledterms.UnitOfMeasurement", "openminds.controlledterms.VisualStimulusType"], "vocab:keyword", multiple=True, required=False,
+              doc="Significant word or concept that are representative of the meta data model version."),
         Field("license", "openminds.core.License", "vocab:license", multiple=False, required=True,
               doc="Grant by a party to another party as an element of an agreement between those parties that permits to do, use, or own something."),
-        Field("ontology_identifiers", str, "vocab:ontologyIdentifier", multiple=True, required=False,
-              doc="Term or code used to identify the brain atlas version registered within a particular ontology."),
         Field("other_contributions", "openminds.core.Contribution", "vocab:otherContribution", multiple=True, required=False,
               doc="Giving or supplying of something (such as money or time) as a part or share other than what is covered elsewhere."),
         Field("related_publications", ["openminds.core.DOI", "openminds.core.HANDLE", "openminds.core.ISBN"], "vocab:relatedPublication", multiple=True, required=False,
               doc="Reference to something that was made available for the general public to see or buy."),
         Field("release_date", date, "vocab:releaseDate", multiple=False, required=True,
               doc="Fixed date on which a product is due to become or was made available for the general public to see or buy"),
         Field("repository", "openminds.core.FileRepository", "vocab:repository", multiple=False, required=False,
               doc="Place, room, or container where something is deposited or stored."),
+        Field("serialization_formats", "openminds.core.ContentType", "vocab:serializationFormat", multiple=True, required=False,
+              doc="Form in which a particular data structure or object state is translated to for storage."),
+        Field("specification_formats", "openminds.core.ContentType", "vocab:specificationFormat", multiple=True, required=False,
+              doc="Form in which a particular data structure or object state is specified in."),
         Field("support_channels", str, "vocab:supportChannel", multiple=True, required=False,
               doc="Way of communication used to interact with users or customers."),
+        Field("type", "openminds.controlledterms.MetaDataModelType", "vocab:type", multiple=False, required=True,
+              doc="Distinct class to which a group of entities or concepts with similar characteristics or attributes belong to."),
         Field("version_identifier", str, "vocab:versionIdentifier", multiple=False, required=True,
               doc="Term or code used to identify the version of something."),
         Field("version_innovation", str, "vocab:versionInnovation", multiple=False, required=True,
               doc="Documentation on what changed in comparison to a previously published form of something."),
 
     ]
     existence_query_fields = ('alias', 'version_identifier')
```

### Comparing `fairgraph-0.8.2/fairgraph/openminds/sands/atlas/common_coordinate_space.py` & `fairgraph-0.9.0/fairgraph/openminds/controlledterms/cranial_window_reinforcement_type.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,56 +1,76 @@
 """
 
+
+    .. list-table:: **Possible values**
+       :widths: 20 80
+       :header-rows: 0
+
+       * - GRIN lens-based cranial window
+         - A cranial window reinforced by an implanted GRIN lens.
+       * - crystalline-based cranial window
+         - A cranial window reinforced by an implantation of a crystalline material.
+       * - prism-based cranial window
+         - A cranial window reinforced by an implanted prism.
+       * - glass coverslip cranial window
+         - A cranial window reinforced by an implantation of a glass coverslip.
+       * - polymer-based cranial window
+         - A cranial window reinforced by an implantation of a polymer material.
+
 """
 
 # this file was auto-generated
 
 from datetime import date, datetime
 from fairgraph.base_v3 import KGObject, IRI
 from fairgraph.fields import Field
 
 
 
 
-class CommonCoordinateSpace(KGObject):
+class CranialWindowReinforcementType(KGObject):
     """
 
+
+    .. list-table:: **Possible values**
+       :widths: 20 80
+       :header-rows: 0
+
+       * - GRIN lens-based cranial window
+         - A cranial window reinforced by an implanted GRIN lens.
+       * - crystalline-based cranial window
+         - A cranial window reinforced by an implantation of a crystalline material.
+       * - prism-based cranial window
+         - A cranial window reinforced by an implanted prism.
+       * - glass coverslip cranial window
+         - A cranial window reinforced by an implantation of a glass coverslip.
+       * - polymer-based cranial window
+         - A cranial window reinforced by an implantation of a polymer material.
+
     """
-    default_space = "atlas"
-    type = ["https://openminds.ebrains.eu/sands/CommonCoordinateSpace"]
+    default_space = "controlled"
+    type = ["https://openminds.ebrains.eu/controlledTerms/CranialWindowReinforcementType"]
     context = {
         "schema": "http://schema.org/",
         "kg": "https://kg.ebrains.eu/api/instances/",
         "vocab": "https://openminds.ebrains.eu/vocab/",
         "terms": "https://openminds.ebrains.eu/controlledTerms/",
         "core": "https://openminds.ebrains.eu/core/"
     }
     fields = [
-        Field("name", str, "vocab:fullName", multiple=False, required=True,
-              doc="Whole, non-abbreviated name of the common coordinate space."),
-        Field("alias", str, "vocab:shortName", multiple=False, required=True,
-              doc="Shortened or fully abbreviated name of the common coordinate space."),
-        Field("anatomical_axes_orientation", "openminds.controlledterms.AnatomicalAxesOrientation", "vocab:anatomicalAxesOrientation", multiple=False, required=True,
-              doc="Relation between reference planes used in anatomy and mathematics."),
-        Field("axes_origins", "openminds.core.QuantitativeValue", "vocab:axesOrigin", multiple=True, required=True,
-              doc="Special point in a coordinate system used as a fixed point of reference for the geometry of the surrounding space."),
-        Field("default_images", "openminds.core.File", "vocab:defaultImage", multiple=True, required=False,
-              doc="Two or three dimensional image that particluarly represents a specific coordinate space."),
+        Field("name", str, "vocab:name", multiple=False, required=True,
+              doc="Word or phrase that constitutes the distinctive designation of the cranial window reinforcement type."),
+        Field("definition", str, "vocab:definition", multiple=False, required=False,
+              doc="Short, but precise statement of the meaning of a word, word group, sign or a symbol."),
         Field("description", str, "vocab:description", multiple=False, required=False,
-              doc="Longer statement or account giving the characteristics of the common coordinate space."),
-        Field("digital_identifier", ["openminds.core.DOI", "openminds.core.ISBN", "openminds.core.RRID"], "vocab:digitalIdentifier", multiple=False, required=False,
-              doc="Digital handle to identify objects or legal persons."),
-        Field("homepage", "openminds.core.URL", "vocab:homepage", multiple=False, required=False,
-              doc="Main website of the common coordinate space."),
-        Field("how_to_cite", str, "vocab:howToCite", multiple=False, required=False,
-              doc="Preferred format for citing a particular object or legal person."),
-        Field("native_unit", "openminds.controlledterms.UnitOfMeasurement", "vocab:nativeUnit", multiple=False, required=True,
-              doc="Determinate quantity used in the original measurement."),
-        Field("ontology_identifiers", str, "vocab:ontologyIdentifier", multiple=True, required=False,
-              doc="Term or code used to identify the common coordinate space registered within a particular ontology."),
-        Field("release_date", date, "vocab:releaseDate", multiple=False, required=True,
-              doc="Fixed date on which a product is due to become or was made available for the general public to see or buy"),
-        Field("version_identifier", str, "vocab:versionIdentifier", multiple=False, required=True,
-              doc="Term or code used to identify the version of something."),
+              doc="Longer statement or account giving the characteristics of the cranial window reinforcement type."),
+        Field("interlex_identifier", IRI, "vocab:interlexIdentifier", multiple=False, required=False,
+              doc="Persistent identifier for a term registered in the InterLex project."),
+        Field("knowledge_space_link", IRI, "vocab:knowledgeSpaceLink", multiple=False, required=False,
+              doc="Persistent link to an encyclopedia entry in the Knowledge Space project."),
+        Field("preferred_ontology_identifier", IRI, "vocab:preferredOntologyIdentifier", multiple=False, required=False,
+              doc="Persistent identifier of a preferred ontological term."),
+        Field("synonyms", str, "vocab:synonym", multiple=True, required=False,
+              doc="Words or expressions used in the same language that have the same or nearly the same meaning in some or all senses."),
 
     ]
-    existence_query_fields = ('alias', 'version_identifier')
+    existence_query_fields = ('name',)
```

### Comparing `fairgraph-0.8.2/fairgraph/openminds/sands/mathematicalShapes/circle.py` & `fairgraph-0.9.0/fairgraph/openminds/stimulation/stimulus/ephys_stimulus.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,26 +7,26 @@
 from datetime import date, datetime
 from fairgraph.base_v3 import KGObject, IRI
 from fairgraph.fields import Field
 
 
 
 
-class Circle(KGObject):
+class EphysStimulus(KGObject):
     """
 
     """
-    default_space = "atlas"
-    type = ["https://openminds.ebrains.eu/sands/Circle"]
+    default_space = "in-depth"
+    type = ["https://openminds.ebrains.eu/stimulation/EphysStimulus"]
     context = {
         "schema": "http://schema.org/",
         "kg": "https://kg.ebrains.eu/api/instances/",
         "vocab": "https://openminds.ebrains.eu/vocab/",
         "terms": "https://openminds.ebrains.eu/controlledTerms/",
         "core": "https://openminds.ebrains.eu/core/"
     }
     fields = [
-        Field("radius", "openminds.core.QuantitativeValue", "vocab:radius", multiple=False, required=True,
+        Field("stimulus_type", "openminds.controlledterms.ElectricalStimulusType", "vocab:stimulusType", multiple=False, required=False,
               doc="no description available"),
 
     ]
-    existence_query_fields = ('radius',)
+    existence_query_fields = ()
```

### Comparing `fairgraph-0.8.2/fairgraph/openminds/sands/miscellaneous/coordinate_point.py` & `fairgraph-0.9.0/fairgraph/openminds/sands/miscellaneous/coordinate_point.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 """
 Structured information on a coordinate point.
 """
 
 # this file was auto-generated
 
 from datetime import date, datetime
-from fairgraph.base_v3 import KGObject, IRI
+from fairgraph.base_v3 import EmbeddedMetadata, IRI
 from fairgraph.fields import Field
 
 
 
 
-class CoordinatePoint(KGObject):
+class CoordinatePoint(EmbeddedMetadata):
     """
     Structured information on a coordinate point.
     """
-    default_space = "atlas"
     type = ["https://openminds.ebrains.eu/sands/CoordinatePoint"]
     context = {
         "schema": "http://schema.org/",
         "kg": "https://kg.ebrains.eu/api/instances/",
         "vocab": "https://openminds.ebrains.eu/vocab/",
         "terms": "https://openminds.ebrains.eu/controlledTerms/",
         "core": "https://openminds.ebrains.eu/core/"
@@ -27,8 +26,7 @@
     fields = [
         Field("coordinate_space", ["openminds.sands.CommonCoordinateSpace", "openminds.sands.CustomCoordinateSpace"], "vocab:coordinateSpace", multiple=False, required=True,
               doc="Two or three dimensional geometric setting."),
         Field("coordinates", "openminds.core.QuantitativeValue", "vocab:coordinates", multiple=True, required=True,
               doc="Pair or triplet of numbers defining a location in a given coordinate space."),
 
     ]
-    existence_query_fields = ('coordinate_space', 'coordinates')
```

### Comparing `fairgraph-0.8.2/fairgraph/openminds/sands/miscellaneous/qualitative_relation_assessment.py` & `fairgraph-0.9.0/fairgraph/openminds/sands/miscellaneous/qualitative_relation_assessment.py`

 * *Files identical despite different names*

### Comparing `fairgraph-0.8.2/fairgraph/openminds/sands/miscellaneous/quantitative_relation_assessment.py` & `fairgraph-0.9.0/fairgraph/openminds/core/miscellaneous/handle.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,34 +1,32 @@
 """
-
+A persistent identifier for an information resource provided by the Handle System of the Corporation for National Research Initiatives.
 """
 
 # this file was auto-generated
 
 from datetime import date, datetime
-from fairgraph.base_v3 import EmbeddedMetadata, IRI
+from fairgraph.base_v3 import KGObject, IRI
 from fairgraph.fields import Field
 
 
 
 
-class QuantitativeRelationAssessment(EmbeddedMetadata):
+class HANDLE(KGObject):
     """
-
+    A persistent identifier for an information resource provided by the Handle System of the Corporation for National Research Initiatives.
     """
-    type = ["https://openminds.ebrains.eu/sands/QuantitativeRelationAssessment"]
+    default_space = "common"
+    type = ["https://openminds.ebrains.eu/core/HANDLE"]
     context = {
         "schema": "http://schema.org/",
         "kg": "https://kg.ebrains.eu/api/instances/",
         "vocab": "https://openminds.ebrains.eu/vocab/",
         "terms": "https://openminds.ebrains.eu/controlledTerms/",
         "core": "https://openminds.ebrains.eu/core/"
     }
     fields = [
-        Field("criteria", "openminds.core.ProtocolExecution", "vocab:criteria", multiple=False, required=False,
-              doc="Aspects or standards on which a judgement or decision is based."),
-        Field("in_relation_to", "openminds.sands.ParcellationEntityVersion", "vocab:inRelationTo", multiple=False, required=True,
-              doc="Reference to a related element."),
-        Field("quantitative_overlap", ["openminds.core.QuantitativeValue", "openminds.core.QuantitativeValueRange"], "vocab:quantitativeOverlap", multiple=False, required=True,
-              doc="Numerical characterization of how much two things occupy the same space."),
+        Field("identifier", str, "vocab:identifier", multiple=False, required=True,
+              doc="Term or code used to identify the HANDLE."),
 
     ]
+    existence_query_fields = ('identifier',)
```

### Comparing `fairgraph-0.8.2/fairgraph/optophysiology.py` & `fairgraph-0.9.0/fairgraph/optophysiology.py`

 * *Files identical despite different names*

### Comparing `fairgraph-0.8.2/fairgraph/queries.py` & `fairgraph-0.9.0/fairgraph/queries.py`

 * *Files identical despite different names*

### Comparing `fairgraph-0.8.2/fairgraph/registry.py` & `fairgraph-0.9.0/fairgraph/registry.py`

 * *Files identical despite different names*

### Comparing `fairgraph-0.8.2/fairgraph/software.py` & `fairgraph-0.9.0/fairgraph/software.py`

 * *Files identical despite different names*

### Comparing `fairgraph-0.8.2/fairgraph/uniminds.py` & `fairgraph-0.9.0/fairgraph/uniminds.py`

 * *Files identical despite different names*

### Comparing `fairgraph-0.8.2/fairgraph/utility.py` & `fairgraph-0.9.0/fairgraph/utility.py`

 * *Files identical despite different names*

### Comparing `fairgraph-0.8.2/fairgraph.egg-info/PKG-INFO` & `fairgraph-0.9.0/fairgraph.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,21 @@
 Metadata-Version: 2.1
 Name: fairgraph
-Version: 0.8.2
+Version: 0.9.0
 Summary: Python API for the Human Brain Project Knowledge Graph
-Home-page: https://github.com/HumanBrainProject/fairgraph
-Author: Andrew P. Davison
-Author-email: andrew.davison@cnrs.fr
-License: UNKNOWN
-Keywords: ebrains hbp metadata electrophysiology knowledge-graph
-Platform: UNKNOWN
+Author-email: "Andrew P. Davison" <andrew.davison@cnrs.fr>
+License: Apache Software License
+Project-URL: Homepage, https://github.com/HumanBrainProject/fairgraph
+Keywords: ebrains,hbp,metadata,electrophysiology,knowledge-graph
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # fairgraph: a Python API for the EBRAINS Knowledge Graph.
 
 Authors: Andrew P. Davison, Onur Ates, Nico Feld, Yann Zerlaut, Glynis Mattheisen
 
@@ -179,9 +174,7 @@
 please open a ticket in the [issue tracker](https://github.com/HumanBrainProject/fairgraph/issues).
 
 ## Acknowledgements
 
 <div><img src="https://www.braincouncil.eu/wp-content/uploads/2018/11/wsi-imageoptim-EU-Logo.jpg" alt="EU Logo" height="23%" width="15%" align="right" style="margin-left: 10px"></div>
 
 This open source software code was developed in part or in whole in the Human Brain Project, funded from the European Union's Horizon 2020 Framework Programme for Research and Innovation under Specific Grant Agreements No. 720270, No. 785907 and No. 945539 (Human Brain Project SGA1, SGA2 and SGA3).
-
-
```

### Comparing `fairgraph-0.8.2/fairgraph.egg-info/SOURCES.txt` & `fairgraph-0.9.0/fairgraph.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 LICENSE.txt
-MANIFEST.in
 README.md
+pyproject.toml
 requirements.txt
 setup.py
 fairgraph/__init__.py
 fairgraph/analysis.py
 fairgraph/base_v2.py
 fairgraph/base_v3.py
 fairgraph/brainsimulation.py
@@ -57,71 +57,83 @@
 fairgraph/openminds/controlledterms/__init__.py
 fairgraph/openminds/controlledterms/action_status_type.py
 fairgraph/openminds/controlledterms/age_category.py
 fairgraph/openminds/controlledterms/anatomical_axes_orientation.py
 fairgraph/openminds/controlledterms/anatomical_plane.py
 fairgraph/openminds/controlledterms/annotation_type.py
 fairgraph/openminds/controlledterms/atlas_type.py
+fairgraph/openminds/controlledterms/auditory_stimulus_type.py
 fairgraph/openminds/controlledterms/biological_order.py
 fairgraph/openminds/controlledterms/biological_sex.py
 fairgraph/openminds/controlledterms/breeding_type.py
 fairgraph/openminds/controlledterms/cell_culture_type.py
 fairgraph/openminds/controlledterms/cell_type.py
 fairgraph/openminds/controlledterms/chemical_mixture_type.py
 fairgraph/openminds/controlledterms/contribution_type.py
-fairgraph/openminds/controlledterms/cranial_window_type.py
+fairgraph/openminds/controlledterms/cranial_window_construction_type.py
+fairgraph/openminds/controlledterms/cranial_window_reinforcement_type.py
 fairgraph/openminds/controlledterms/criteria_quality_type.py
 fairgraph/openminds/controlledterms/data_type.py
 fairgraph/openminds/controlledterms/device_type.py
 fairgraph/openminds/controlledterms/difference_measure.py
 fairgraph/openminds/controlledterms/disease.py
 fairgraph/openminds/controlledterms/disease_model.py
+fairgraph/openminds/controlledterms/educational_level.py
+fairgraph/openminds/controlledterms/electrical_stimulus_type.py
 fairgraph/openminds/controlledterms/ethics_assessment.py
 fairgraph/openminds/controlledterms/experimental_approach.py
 fairgraph/openminds/controlledterms/file_bundle_grouping.py
 fairgraph/openminds/controlledterms/file_repository_type.py
 fairgraph/openminds/controlledterms/file_usage_role.py
 fairgraph/openminds/controlledterms/genetic_strain_type.py
+fairgraph/openminds/controlledterms/gustatory_stimulus_type.py
 fairgraph/openminds/controlledterms/handedness.py
 fairgraph/openminds/controlledterms/language.py
 fairgraph/openminds/controlledterms/laterality.py
+fairgraph/openminds/controlledterms/learning_resource_type.py
 fairgraph/openminds/controlledterms/measured_quantity.py
 fairgraph/openminds/controlledterms/meta_data_model_type.py
 fairgraph/openminds/controlledterms/model_abstraction_level.py
 fairgraph/openminds/controlledterms/model_scope.py
 fairgraph/openminds/controlledterms/molecular_entity.py
+fairgraph/openminds/controlledterms/olfactory_stimulus_type.py
 fairgraph/openminds/controlledterms/operating_device.py
 fairgraph/openminds/controlledterms/operating_system.py
+fairgraph/openminds/controlledterms/optical_stimulus_type.py
 fairgraph/openminds/controlledterms/organ.py
 fairgraph/openminds/controlledterms/patch_clamp_variation.py
 fairgraph/openminds/controlledterms/preparation_type.py
 fairgraph/openminds/controlledterms/product_accessibility.py
 fairgraph/openminds/controlledterms/programming_language.py
 fairgraph/openminds/controlledterms/qualitative_overlap.py
 fairgraph/openminds/controlledterms/semantic_data_type.py
 fairgraph/openminds/controlledterms/service.py
 fairgraph/openminds/controlledterms/setup_type.py
 fairgraph/openminds/controlledterms/software_application_category.py
 fairgraph/openminds/controlledterms/software_feature.py
 fairgraph/openminds/controlledterms/species.py
 fairgraph/openminds/controlledterms/stimulation_approach.py
-fairgraph/openminds/controlledterms/stimulus_type.py
+fairgraph/openminds/controlledterms/stimulation_technique.py
 fairgraph/openminds/controlledterms/subcellular_entity.py
 fairgraph/openminds/controlledterms/subject_attribute.py
+fairgraph/openminds/controlledterms/tactile_stimulus_type.py
 fairgraph/openminds/controlledterms/technique.py
 fairgraph/openminds/controlledterms/term_suggestion.py
 fairgraph/openminds/controlledterms/terminology.py
 fairgraph/openminds/controlledterms/tissue_sample_attribute.py
 fairgraph/openminds/controlledterms/tissue_sample_type.py
 fairgraph/openminds/controlledterms/type_of_uncertainty.py
 fairgraph/openminds/controlledterms/uberon_parcellation.py
 fairgraph/openminds/controlledterms/unit_of_measurement.py
+fairgraph/openminds/controlledterms/visual_stimulus_type.py
 fairgraph/openminds/core/__init__.py
 fairgraph/openminds/core/actors/__init__.py
+fairgraph/openminds/core/actors/account_information.py
 fairgraph/openminds/core/actors/affiliation.py
+fairgraph/openminds/core/actors/consortium.py
 fairgraph/openminds/core/actors/contact_information.py
 fairgraph/openminds/core/actors/contribution.py
 fairgraph/openminds/core/actors/organization.py
 fairgraph/openminds/core/actors/person.py
 fairgraph/openminds/core/data/__init__.py
 fairgraph/openminds/core/data/content_type.py
 fairgraph/openminds/core/data/content_type_pattern.py
@@ -160,24 +172,25 @@
 fairgraph/openminds/core/products/meta_data_model_version.py
 fairgraph/openminds/core/products/model.py
 fairgraph/openminds/core/products/model_version.py
 fairgraph/openminds/core/products/project.py
 fairgraph/openminds/core/products/setup.py
 fairgraph/openminds/core/products/software.py
 fairgraph/openminds/core/products/software_version.py
+fairgraph/openminds/core/products/web_service.py
+fairgraph/openminds/core/products/web_service_version.py
 fairgraph/openminds/core/research/__init__.py
 fairgraph/openminds/core/research/behavioral_protocol.py
 fairgraph/openminds/core/research/configuration.py
 fairgraph/openminds/core/research/custom_property_set.py
 fairgraph/openminds/core/research/experimental_activity.py
 fairgraph/openminds/core/research/numerical_property.py
 fairgraph/openminds/core/research/property_value_list.py
 fairgraph/openminds/core/research/protocol.py
 fairgraph/openminds/core/research/protocol_execution.py
-fairgraph/openminds/core/research/stimulation.py
 fairgraph/openminds/core/research/strain.py
 fairgraph/openminds/core/research/string_property.py
 fairgraph/openminds/core/research/subject.py
 fairgraph/openminds/core/research/subject_group.py
 fairgraph/openminds/core/research/subject_group_state.py
 fairgraph/openminds/core/research/subject_state.py
 fairgraph/openminds/core/research/tissue_sample.py
@@ -198,14 +211,15 @@
 fairgraph/openminds/ephys/device/pipette_usage.py
 fairgraph/openminds/ephys/entity/__init__.py
 fairgraph/openminds/ephys/entity/channel.py
 fairgraph/openminds/ephys/entity/recording.py
 fairgraph/openminds/publications/__init__.py
 fairgraph/openminds/publications/book.py
 fairgraph/openminds/publications/chapter.py
+fairgraph/openminds/publications/learning_resource.py
 fairgraph/openminds/publications/live_paper.py
 fairgraph/openminds/publications/live_paper_resource_item.py
 fairgraph/openminds/publications/live_paper_section.py
 fairgraph/openminds/publications/live_paper_version.py
 fairgraph/openminds/publications/periodical.py
 fairgraph/openminds/publications/publication_issue.py
 fairgraph/openminds/publications/publication_volume.py
@@ -229,23 +243,36 @@
 fairgraph/openminds/sands/miscellaneous/coordinate_point.py
 fairgraph/openminds/sands/miscellaneous/qualitative_relation_assessment.py
 fairgraph/openminds/sands/miscellaneous/quantitative_relation_assessment.py
 fairgraph/openminds/sands/non_atlas/__init__.py
 fairgraph/openminds/sands/non_atlas/custom_anatomical_entity.py
 fairgraph/openminds/sands/non_atlas/custom_annotation.py
 fairgraph/openminds/sands/non_atlas/custom_coordinate_space.py
+fairgraph/openminds/specimenprep/__init__.py
+fairgraph/openminds/specimenprep/activity/__init__.py
+fairgraph/openminds/specimenprep/activity/cranial_window_preparation.py
+fairgraph/openminds/specimenprep/activity/tissue_culture_preparation.py
+fairgraph/openminds/specimenprep/activity/tissue_sample_slicing.py
+fairgraph/openminds/specimenprep/device/__init__.py
+fairgraph/openminds/specimenprep/device/slicing_device.py
+fairgraph/openminds/specimenprep/device/slicing_device_usage.py
+fairgraph/openminds/stimulation/__init__.py
+fairgraph/openminds/stimulation/activity/__init__.py
+fairgraph/openminds/stimulation/activity/stimulation_activity.py
+fairgraph/openminds/stimulation/stimulus/__init__.py
+fairgraph/openminds/stimulation/stimulus/ephys_stimulus.py
 test/__init__.py
 test/test_analysis.py
 test/test_base.py
 test/test_brainsimulation.py
 test/test_client.py
 test/test_commons.py
 test/test_core.py
 test/test_electrophysiology.py
+test/test_fields.py
 test/test_minds.py
 test/test_openminds_computation.py
 test/test_openminds_core.py
 test/test_queries.py
 test/test_software.py
 test/test_uniminds.py
-test/utils.py
 test/utils_v3.py
```

### Comparing `fairgraph-0.8.2/setup.py` & `fairgraph-0.9.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,45 +1,43 @@
+[project]
+name = "fairgraph"
+version = "0.9.0"
+description = "Python API for the Human Brain Project Knowledge Graph"
+readme = "README.md"
+authors = [
+    { name="Andrew P. Davison", email="andrew.davison@cnrs.fr" }
+]
+requires-python = ">=3.7"
+license = {text = "Apache Software License"}
+classifiers = [
+    "Development Status :: 4 - Beta",
+    "Intended Audience :: Science/Research",
+    "Topic :: Scientific/Engineering",
+    "License :: OSI Approved :: Apache Software License",
+    "Programming Language :: Python :: 3"
+]
+keywords = ["ebrains", "hbp", "metadata", "electrophysiology", "knowledge-graph"]
+dependencies=[
+    #"openid_http_client @ git+https://github.com/HumanBrainProject/openid_http_client.git#subdirectory=openid_http_client",
+    #"pyxus @ git+https://github.com/apdavison/pyxus.git@pystache-jinja2#egg=pyxus&subdirectory=pyxus",
+    "ebrains-kg-core",
+    "pathlib2",
+    "python-dateutil",
+    "six",
+    "tabulate",
+    "requests",
+    "tqdm",
+    "pyld==0.8.2"
+]
 
-from setuptools import setup, find_packages
-from codecs import open
-from os import path
+[project.urls]
+"Homepage" = "https://github.com/HumanBrainProject/fairgraph"
 
-here = path.abspath(path.dirname(__file__))
+[tool.setuptools.packages.find]
+include = ["fairgraph*"]
 
-with open(path.join(here, 'README.md'), encoding='utf-8') as f:
-    long_description = f.read()
-
-setup(
-    name='fairgraph',
-    version='0.8.2',
-    description='Python API for the Human Brain Project Knowledge Graph',
-    long_description=long_description,
-    long_description_content_type="text/markdown",
-    url='https://github.com/HumanBrainProject/fairgraph',
-    author='Andrew P. Davison',
-    author_email='andrew.davison@cnrs.fr',
-    classifiers=[
-        'Development Status :: 4 - Beta',
-        'Intended Audience :: Science/Research',
-        'Topic :: Scientific/Engineering',
-        'License :: OSI Approved :: Apache Software License',
-        'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.7',
-        'Programming Language :: Python :: 3.8',
-        'Programming Language :: Python :: 3.9',
-        'Programming Language :: Python :: 3.10',
-    ],
-    keywords='ebrains hbp metadata electrophysiology knowledge-graph',
-    packages=find_packages(),
-    install_requires=[
-        #"openid_http_client @ git+https://github.com/HumanBrainProject/openid_http_client.git#subdirectory=openid_http_client",
-        #"pyxus @ git+https://github.com/apdavison/pyxus.git@pystache-jinja2#egg=pyxus&subdirectory=pyxus",
-        "ebrains-kg-core",
-        "pathlib2",
-        "python-dateutil",
-        "six",
-        "tabulate",
-        "requests",
-        "tqdm",
-        "pyld==0.8.2"
-    ]
-)
+[build-system]
+ requires = [
+     "setuptools",
+     "wheel",
+ ]
+ build-backend = "setuptools.build_meta"
```

### Comparing `fairgraph-0.8.2/test/test_analysis.py` & `fairgraph-0.9.0/test/test_analysis.py`

 * *Files identical despite different names*

### Comparing `fairgraph-0.8.2/test/test_base.py` & `fairgraph-0.9.0/test/test_base.py`

 * *Files identical despite different names*

### Comparing `fairgraph-0.8.2/test/test_brainsimulation.py` & `fairgraph-0.9.0/test/test_brainsimulation.py`

 * *Files identical despite different names*

### Comparing `fairgraph-0.8.2/test/test_commons.py` & `fairgraph-0.9.0/test/test_commons.py`

 * *Files identical despite different names*

### Comparing `fairgraph-0.8.2/test/test_core.py` & `fairgraph-0.9.0/test/test_core.py`

 * *Files identical despite different names*

### Comparing `fairgraph-0.8.2/test/test_electrophysiology.py` & `fairgraph-0.9.0/test/test_electrophysiology.py`

 * *Files identical despite different names*

### Comparing `fairgraph-0.8.2/test/test_minds.py` & `fairgraph-0.9.0/test/test_minds.py`

 * *Files identical despite different names*

### Comparing `fairgraph-0.8.2/test/test_openminds_computation.py` & `fairgraph-0.9.0/test/test_openminds_computation.py`

 * *Files identical despite different names*

### Comparing `fairgraph-0.8.2/test/test_openminds_core.py` & `fairgraph-0.9.0/test/test_openminds_core.py`

 * *Files 10% similar despite different names*

```diff
@@ -88,18 +88,18 @@
 @skip_if_no_connection
 def test_resolve_model(kg_client):
     model = omcore.Model.from_id("708024f7-9dd7-4c92-ae95-936db23c6d99", kg_client)
     assert model.name == "Scaffold Model of Cerebellum microcircuit version 2.0"
     assert isinstance(model.versions, KGProxy)
     resolved_model2 = deepcopy(model).resolve(kg_client, scope="in progress", follow_links=2)
     assert isinstance(resolved_model2.versions, omcore.ModelVersion)
-    assert isinstance(resolved_model2.custodians[0].affiliations[0].organization, KGProxy)
+    assert isinstance(resolved_model2.custodians[0].affiliations[0].member_of, KGProxy)
 
     resolved_model4 = deepcopy(model).resolve(kg_client, scope="in progress", follow_links=3)
-    assert isinstance(resolved_model4.custodians[0].affiliations[0].organization, omcore.Organization)
+    assert isinstance(resolved_model4.custodians[0].affiliations[0].member_of, omcore.Organization)
 
 
 @skip_if_no_connection
 def test_count_released_models(kg_client):
     models = omcore.Model.list(kg_client, scope="released", space="model", api="core", size=1000)
     n_models = omcore.Model.count(kg_client, scope="released", space="model", api="core")
     assert len(models) == n_models
@@ -136,14 +136,47 @@
 
     new_model = omcore.Model(name=model.name)
     assert new_model != model
     assert new_model.exists(kg_client)
     assert new_model == model
 
 
+def test__update():
+    example_data = {
+        '@id': 'https://kg.ebrains.eu/api/instances/e90fc25a-fc35-4066-9ff2-ca3583a2d008',
+        '@type': ['https://openminds.ebrains.eu/core/Person'],
+        'http://schema.org/identifier': [
+            'ba78ffe138e3a79a7514f26441fba6ff',
+            'https://nexus.humanbrainproject.org/v0/data/uniminds/core/person/v1.0.0/e90fc25a-fc35-4066-9ff2-ca3583a2d008',
+            'https://kg.ebrains.eu/api/instances/e90fc25a-fc35-4066-9ff2-ca3583a2d008'
+        ],
+        'https://core.kg.ebrains.eu/vocab/meta/revision': '_fCLxIMC---',
+        'https://core.kg.ebrains.eu/vocab/meta/space': 'common',
+        'https://openminds.ebrains.eu/vocab/affiliation': {
+            '@type': ['https://openminds.ebrains.eu/core/Affiliation'],
+            'https://openminds.ebrains.eu/vocab/memberOf': {
+                '@id': 'https://kg.ebrains.eu/api/instances/05c23d56-b27e-4cf2-8c47-ed12c1a441e7'
+            }
+        },
+        'https://openminds.ebrains.eu/vocab/contactInformation': [
+            {'@id': 'https://kg.ebrains.eu/api/instances/4b88cd1e-e222-47e9-9b4a-32b648bddbca'},
+            {'@id': 'https://kg.ebrains.eu/api/instances/bc036c71-084b-4ffa-8430-4543095660f2'}
+        ],
+        'https://openminds.ebrains.eu/vocab/familyName': 'Bianchi',
+        'https://openminds.ebrains.eu/vocab/givenName': 'Daniela'
+    }
+    client = None
+    person = omcore.Person.from_kg_instance(example_data, client=client, scope="in progress")
+    assert person.data == example_data
+    # this follows the sequence in person.save()
+    data = person._build_data(client, all_fields=True)
+    updated_data = person._updated_data(data)
+    assert len(updated_data) == 0
+
+
 @skip_if_no_connection
 def test_KGQuery_resolve(kg_client):
     ca1 = omterms.UBERONParcellation.by_name("CA1 field of hippocampus", kg_client)
     single_cell = omterms.ModelScope.by_name("single cell", kg_client)
     filters = {"study_targets": ca1, "model_scope": single_cell}
     q = KGQuery(omcore.Model, filters)
     models_q = q.resolve(kg_client, scope="released")
@@ -190,25 +223,25 @@
 
 
 def test_save_new_recursive_mock(mock_client):
     new_person = omcore.Person(
         given_name="Thorin",
         family_name="Oakenshield",
         affiliations=omcore.Affiliation(
-            organization=omcore.Organization(name="The Lonely Mountain")
+            member_of=omcore.Organization(name="The Lonely Mountain")
         )
     )
     log = ActivityLog()
     new_person.save(mock_client, space="myspace", recursive=True, activity_log=log)
     assert len(log.entries) == 2
     assert log.entries[0].cls == "Organization"
     assert log.entries[0].space == "myspace"
     assert log.entries[0].type == "create"
     assert log.entries[1].cls == "Person"
     assert log.entries[1].space == "myspace"
     assert log.entries[1].type == "create"
     assert UUID(new_person.uuid)
-    assert UUID(new_person.affiliations.organization.uuid)
+    assert UUID(new_person.affiliations.member_of.uuid)
 
 
 #def test_save_existing_with_id_mock(mock_client):
 #    existing_model = mock_client.instances[]
```

### Comparing `fairgraph-0.8.2/test/test_queries.py` & `fairgraph-0.9.0/test/test_queries.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,16 +37,16 @@
                       type_filter="https://openminds.ebrains.eu/core/Person",
                       properties=[
                           QueryProperty("@id", filter=Filter("EQUALS", parameter="custodian")),
                           QueryProperty("https://openminds.ebrains.eu/vocab/affiliation",
                                     name="vocab:affiliation",
                                     properties=[
                                         QueryProperty("@type"),
-                                        QueryProperty("https://openminds.ebrains.eu/vocab/organization",
-                                                  name="vocab:organization",
+                                        QueryProperty("https://openminds.ebrains.eu/vocab/memberOf",
+                                                  name="vocab:memberOf",
                                                   properties=[QueryProperty("@id")]),
                                         QueryProperty("https://openminds.ebrains.eu/vocab/startDate",
                                                   name="vocab:startDate")
                                     ])
                       ])
         ]
     )
@@ -148,16 +148,16 @@
                     },
                     {
                         'path': 'https://openminds.ebrains.eu/vocab/affiliation',
                         'propertyName': 'vocab:affiliation',
                         'structure': [
                             {'path': '@type'},
                             {
-                                'path': 'https://openminds.ebrains.eu/vocab/organization',
-                                'propertyName': 'vocab:organization',
+                                'path': 'https://openminds.ebrains.eu/vocab/memberOf',
+                                'propertyName': 'vocab:memberOf',
                                 'structure': [
                                     {'path': '@id'}
                                 ]
                             },
                             {
                                 'path': 'https://openminds.ebrains.eu/vocab/startDate',
                                 'propertyName': 'vocab:startDate'
```

### Comparing `fairgraph-0.8.2/test/test_software.py` & `fairgraph-0.9.0/test/test_software.py`

 * *Files identical despite different names*

### Comparing `fairgraph-0.8.2/test/test_uniminds.py` & `fairgraph-0.9.0/test/test_uniminds.py`

 * *Files identical despite different names*

### Comparing `fairgraph-0.8.2/test/utils_v3.py` & `fairgraph-0.9.0/test/utils_v3.py`

 * *Files identical despite different names*

