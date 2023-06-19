# Comparing `tmp/RIFT-0.0.15.9rc3.tar.gz` & `tmp/RIFT-0.0.15.9rc4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RIFT-0.0.15.9rc3.tar", last modified: Wed Jun  7 15:16:47 2023, max compression
+gzip compressed data, was "RIFT-0.0.15.9rc4.tar", last modified: Mon Jun 19 13:22:14 2023, max compression
```

## Comparing `RIFT-0.0.15.9rc3.tar` & `RIFT-0.0.15.9rc4.tar`

### file list

```diff
@@ -1,193 +1,193 @@
-drwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)        0 2023-06-07 15:16:47.300335 RIFT-0.0.15.9rc3/
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1042 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc3/AUTOMATED_OR_ONLINE.md
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1755 2023-04-20 10:32:56.000000 RIFT-0.0.15.9rc3/Dockerfile
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    22146 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc3/GETTING_STARTED.md
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     3557 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc3/INSTALL.md
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1364 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc3/INSTALL_OPTIONAL_DEPENDENCIES.md
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1118 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc3/LICENSE.md
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)      204 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc3/MANIFEST.in
-drwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)        0 2023-06-07 15:16:47.003334 RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/
-drwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)        0 2023-06-07 15:16:47.007334 RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/
-drwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)        0 2023-06-07 15:16:47.029334 RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/RIFT/
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)      173 2023-05-24 11:46:08.000000 RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/RIFT/__init__.py
-drwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)        0 2023-06-07 15:16:47.038334 RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/RIFT/calmarg/
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)       22 2023-05-24 11:46:08.000000 RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/RIFT/calmarg/__init__.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     6265 2023-05-24 11:46:08.000000 RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/RIFT/calmarg/rift_source.py
-drwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)        0 2023-06-07 15:16:47.053334 RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/RIFT/integrators/
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    18724 2023-04-16 18:23:39.000000 RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/RIFT/integrators/MonteCarloEnsemble.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)        0 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/RIFT/integrators/__init__.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     2592 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/RIFT/integrators/direct_quadrature.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    20255 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/RIFT/integrators/gaussian_mixture_model.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    53572 2023-05-30 17:28:25.000000 RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/RIFT/integrators/mcsampler.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    28350 2023-05-24 11:46:08.000000 RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/RIFT/integrators/mcsamplerEnsemble.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    69057 2023-05-30 17:28:25.000000 RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/RIFT/integrators/mcsamplerGPU.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     2901 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/RIFT/integrators/multivariate_truncnorm.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     7235 2022-10-24 14:00:10.000000 RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/RIFT/integrators/statutils.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    33113 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/RIFT/integrators/weighted_gmm.py
-drwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)        0 2023-06-07 15:16:47.066334 RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/RIFT/interpolators/
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     9944 2022-10-23 22:26:00.000000 RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/RIFT/interpolators/BayesianLeastSquares.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     3835 2022-10-23 22:26:00.000000 RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/RIFT/interpolators/ConstrainedQuadraticLikelihood.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)        0 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/RIFT/interpolators/__init__.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     2658 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/RIFT/interpolators/efficient_save_sklearn_gp.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1655 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/RIFT/interpolators/gp.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     2518 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/RIFT/interpolators/gpytorch_wrapper.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     5558 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/RIFT/interpolators/internal_GP.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     3488 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/RIFT/interpolators/interp_gpu.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    26826 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/RIFT/interpolators/senni.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)   249715 2023-06-07 15:16:25.000000 RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/RIFT/lalsimutils.py
-drwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)        0 2023-06-07 15:16:47.079334 RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/RIFT/likelihood/
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1643 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/RIFT/likelihood/Q_inner_product.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    33438 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/RIFT/likelihood/SphericalHarmonics_gpu.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)        0 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/RIFT/likelihood/__init__.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1525 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/RIFT/likelihood/cuda_Q_inner_product.cu
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    94316 2023-06-07 15:16:25.000000 RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/RIFT/likelihood/factored_likelihood.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     5269 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/RIFT/likelihood/optimized_gpu_tools.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1451 2023-05-30 17:28:25.000000 RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/RIFT/likelihood/priors_utils.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     4616 2023-06-07 15:16:25.000000 RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/RIFT/likelihood/vectorized_general_tools.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     4706 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/RIFT/likelihood/vectorized_lal_tools.py
-drwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)        0 2023-06-07 15:16:47.111334 RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/RIFT/misc/
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    70947 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/RIFT/misc/ModifiedScikitFit.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)       65 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/RIFT/misc/__init__.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    29427 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/RIFT/misc/amrlib.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     7367 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/RIFT/misc/bounded_kde.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)      229 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/RIFT/misc/common_cl.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)   109345 2023-05-24 11:46:08.000000 RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/RIFT/misc/dag_utils.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     9324 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/RIFT/misc/modules.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    23083 2022-10-11 14:57:54.000000 RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/RIFT/misc/our_corner.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    30542 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/RIFT/misc/ourparams.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    10915 2023-03-24 18:44:03.000000 RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/RIFT/misc/samples_utils.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     2901 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/RIFT/misc/sky_rotations.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    10623 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/RIFT/misc/spokes.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     6975 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/RIFT/misc/tools.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     2641 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/RIFT/misc/weight_simulations.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     8651 2023-05-30 17:28:25.000000 RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/RIFT/misc/xmlutils.py
-drwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)        0 2023-06-07 15:16:47.125334 RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/RIFT/physics/
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    26126 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/RIFT/physics/EOBTidalExternal.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    31276 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/RIFT/physics/EOBTidalExternalC.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    63089 2023-04-07 18:24:37.000000 RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/RIFT/physics/EOSManager.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     4664 2023-03-12 13:15:08.000000 RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/RIFT/physics/GWSignal.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     2654 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/RIFT/physics/MonotonicSpline.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    19507 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/RIFT/physics/PrecessingFisherMatrix.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    52302 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/RIFT/physics/ROMWaveformManager.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)       68 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/RIFT/physics/__init__.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    23733 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/RIFT/physics/effectiveFisher.py
-drwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)        0 2023-06-07 15:16:47.036334 RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/RIFT.egg-info/
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     6360 2023-06-07 15:16:44.000000 RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/RIFT.egg-info/PKG-INFO
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    10749 2023-06-07 15:16:45.000000 RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/RIFT.egg-info/SOURCES.txt
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)        1 2023-06-07 15:16:44.000000 RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/RIFT.egg-info/dependency_links.txt
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)      142 2023-06-07 15:16:44.000000 RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/RIFT.egg-info/requires.txt
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)        5 2023-06-07 15:16:44.000000 RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/RIFT.egg-info/top_level.txt
-drwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)        0 2023-06-07 15:16:47.298335 RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/bin/
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     8723 2022-10-11 14:57:54.000000 RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/bin/assess_propose_CIP_convergence_sequence.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    13848 2023-05-24 11:46:08.000000 RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/bin/calibration_reweighting.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     2371 2023-04-22 14:25:02.000000 RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/bin/combine_weights_and_rejection_sample.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     2800 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/bin/config_yank.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     6140 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/bin/convergence_test_amr.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     9039 2023-06-07 15:16:25.000000 RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/bin/convergence_test_samples.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     2239 2023-04-20 10:32:56.000000 RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/bin/convert_ascii_framechange_xphm.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1224 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/bin/convert_dat_to_hdf5.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1920 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/bin/convert_output_format_allnet2xml
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)      541 2023-03-24 18:44:03.000000 RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/bin/convert_output_format_ascii2h5.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    11799 2023-03-12 13:15:08.000000 RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/bin/convert_output_format_ile2inference
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     8166 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/bin/convert_output_format_inference2ile
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     2013 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/bin/convert_psd_ascii2xml
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     9065 2022-10-11 14:57:54.000000 RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/bin/create_CIP_convergence_sequence.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    33506 2023-04-07 18:24:37.000000 RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/bin/create_eos_posterior_pipeline
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    14569 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/bin/create_event_dag_via_grid
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    88335 2022-10-11 14:57:54.000000 RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/bin/create_event_parameter_pipeline_AlternateIteration
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)   120192 2023-04-25 00:19:30.000000 RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/bin/create_event_parameter_pipeline_BasicIteration
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    71601 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/bin/create_event_parameter_pipeline_BasicMultiApproxIteration
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     2768 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/bin/create_ile_sub_dag.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    13979 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/bin/create_postprocessing_event_dag.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    97555 2023-06-07 15:16:25.000000 RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/bin/helper_LDG_Events.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1886 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/bin/helper_OnlinePSDCleanup.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    20152 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/bin/ile_postproc_add_time
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    83560 2023-03-12 13:15:08.000000 RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/bin/integrate_likelihood_extrinsic
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)   103590 2023-06-07 15:16:25.000000 RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/bin/integrate_likelihood_extrinsic_batchmode
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    18630 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/bin/integrate_likelihood_extrinsic_no-op
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     5408 2023-03-24 18:44:03.000000 RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/bin/make_uni_comov_skymap.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    37925 2023-05-24 11:46:08.000000 RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/bin/plot_posterior_corner.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     3746 2023-03-24 18:44:03.000000 RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/bin/resample_uniform_comoving.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)      354 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/bin/switcheroo
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    34265 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/bin/util_AMRGrid.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     3696 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/bin/util_AdaptiveExponent.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    18544 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/bin/util_AnalyticFisherGrid.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     7130 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/bin/util_BatchConvertResampleILEOutput.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1028 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/bin/util_CIPdagPostprocess.sh
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)      219 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/bin/util_CacheFileConvert.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1436 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/bin/util_CharacterizePosterior.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     3934 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/bin/util_CleanILE.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)      876 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/bin/util_CoincIFOUtility.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    15127 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/bin/util_CompareWaveformsInDetectors.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)      853 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/bin/util_ConsolidateDAGsUnderMaster.sh
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    10380 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/bin/util_ConstructBNSMarginalEOSRank.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    33198 2023-04-07 18:24:37.000000 RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/bin/util_ConstructEOSPosterior.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    55368 2022-11-28 22:41:57.000000 RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/bin/util_ConstructIntrinsicPosterior_GaussianResampling.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)   164109 2023-06-07 15:16:25.000000 RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/bin/util_ConstructIntrinsicPosterior_GenericCoordinates.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     2314 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/bin/util_CoordinateNamesAngularToCartesianSpins.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     9633 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/bin/util_EOBTideWriteFrame.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)      389 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/bin/util_EstimateWaveformDuration.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     3250 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/bin/util_FetchExternalGrid.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    27796 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/bin/util_FitAndEvaluate_GenericCoordinates.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)      256 2022-10-11 14:57:54.000000 RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/bin/util_ForOSG_MakeLocalFramesDir.sh
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1640 2023-03-12 13:15:08.000000 RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/bin/util_ForOSG_MakeTruncatedLocalFramesDir.sh
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     3266 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/bin/util_FrameZeroNoiseSNR.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    11553 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/bin/util_GenerateMaxlnLWaveform.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     6162 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/bin/util_GenerateMaxlnLWaveform_NRFromIndex.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     2223 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/bin/util_GridRecenter.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    13919 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/bin/util_GridSubsetOfTemplateBank.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     2778 2023-04-07 18:24:37.000000 RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/bin/util_HyperCombine.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1590 2023-04-07 18:24:37.000000 RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/bin/util_HyperparameterGrid.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     5156 2023-04-07 18:24:37.000000 RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/bin/util_HyperparameterPuffball.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)      829 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/bin/util_ILENextGeneration.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1018 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/bin/util_ILEROMdagPostprocess.sh
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1597 2022-10-11 14:57:54.000000 RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/bin/util_ILEdagPostprocess.sh
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     6780 2023-03-24 18:44:03.000000 RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/bin/util_InitMargTable
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     4553 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/bin/util_IntermediateEOSIntegralFromFit.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    40228 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/bin/util_IterativeFisher.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     2698 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/bin/util_JoinXML.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     8109 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/bin/util_LALCompareApproximantsOnSamples.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     7660 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/bin/util_LALWriteFrame.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    50356 2022-10-11 14:57:54.000000 RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/bin/util_ManualOverlapGrid.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     7195 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/bin/util_MarginalizedLikelihoodEOSIntegralFromIntermediate.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1214 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/bin/util_MassGrid.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     2450 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/bin/util_MassGridCoalesce.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     8821 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/bin/util_NRBestOfIndex.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     6671 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/bin/util_NRDumpDetectorResponse.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    20394 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/bin/util_NRExtrudeOverlapGrid.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     5672 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/bin/util_NRIndexedFminCutToILE.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    10752 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/bin/util_NRNearestSimulationTo.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     4794 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/bin/util_NRRelabelILE.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     9830 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/bin/util_NRWriteFrame.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     3377 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/bin/util_NR_GWMemory.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1490 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/bin/util_NRdagPostprocess.sh
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     2349 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/bin/util_ParameterFilter.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    12414 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/bin/util_ParameterPuffball.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     3665 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/bin/util_ParameterRandomize.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1087 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/bin/util_PosteriorPostprocess.sh
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     3302 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/bin/util_PrintInjection.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     5424 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/bin/util_RIFT_MultiMetaPipe.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    79435 2023-06-07 15:16:25.000000 RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/bin/util_RIFT_pseudo_pipe.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    35804 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/bin/util_RIFT_pseudo_pipe_lowlatency.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     6293 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/bin/util_ROMWriteFrame.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1675 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/bin/util_RandomizeOverlapOrder.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     3080 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/bin/util_ResampleILEOutputWithExtrinsic.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     3792 2023-03-24 18:44:03.000000 RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/bin/util_SimInspiralToCoinc.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     7587 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/bin/util_TEOBResumSWriteFrame.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     4982 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/bin/util_TestSpokesIO.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)      814 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/bin/util_TestXMLParameterStorage.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    11254 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/bin/util_TidalPlotSimulationStrain.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)      457 2022-10-15 00:56:03.000000 RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/bin/util_TruncateMergeFrames.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     3430 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/bin/util_WriteFrameAndCacheFromXML.sh
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     2784 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/bin/util_WriteInjectionFile.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1955 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/bin/util_WriteXMLWithEOS.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)      276 2023-04-22 14:25:02.000000 RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/bin/util_shuffle_file.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     3488 2022-09-24 12:18:48.000000 RIFT-0.0.15.9rc3/PACKAGING.md
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     6360 2023-06-07 15:16:47.300335 RIFT-0.0.15.9rc3/PKG-INFO
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     5821 2023-04-07 18:24:37.000000 RIFT-0.0.15.9rc3/README.md
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     6132 2022-09-24 12:18:48.000000 RIFT-0.0.15.9rc3/TROUBLESHOOTING.md
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     6136 2022-09-24 12:18:48.000000 RIFT-0.0.15.9rc3/howto.md
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)       96 2023-04-24 19:45:36.000000 RIFT-0.0.15.9rc3/pyproject.toml
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)      184 2023-03-24 18:44:03.000000 RIFT-0.0.15.9rc3/requirements.txt
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)       38 2023-06-07 15:16:47.300335 RIFT-0.0.15.9rc3/setup.cfg
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     2934 2023-06-07 15:16:25.000000 RIFT-0.0.15.9rc3/setup.py
+drwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)        0 2023-06-19 13:22:14.535797 RIFT-0.0.15.9rc4/
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1042 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc4/AUTOMATED_OR_ONLINE.md
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1755 2023-04-20 10:32:56.000000 RIFT-0.0.15.9rc4/Dockerfile
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    22146 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc4/GETTING_STARTED.md
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     3557 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc4/INSTALL.md
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1364 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc4/INSTALL_OPTIONAL_DEPENDENCIES.md
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1118 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc4/LICENSE.md
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)      204 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc4/MANIFEST.in
+drwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)        0 2023-06-19 13:22:12.049787 RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/
+drwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)        0 2023-06-19 13:22:12.214788 RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/
+drwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)        0 2023-06-19 13:22:12.770790 RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/RIFT/
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)      173 2023-05-24 11:46:08.000000 RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/RIFT/__init__.py
+drwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)        0 2023-06-19 13:22:12.830790 RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/RIFT/calmarg/
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)       22 2023-05-24 11:46:08.000000 RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/RIFT/calmarg/__init__.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     6265 2023-05-24 11:46:08.000000 RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/RIFT/calmarg/rift_source.py
+drwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)        0 2023-06-19 13:22:13.192791 RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/RIFT/integrators/
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    18724 2023-04-16 18:23:39.000000 RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/RIFT/integrators/MonteCarloEnsemble.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)        0 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/RIFT/integrators/__init__.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     2592 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/RIFT/integrators/direct_quadrature.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    20255 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/RIFT/integrators/gaussian_mixture_model.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    53572 2023-05-30 17:28:25.000000 RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/RIFT/integrators/mcsampler.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    28350 2023-05-24 11:46:08.000000 RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/RIFT/integrators/mcsamplerEnsemble.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    69417 2023-06-19 13:21:23.000000 RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/RIFT/integrators/mcsamplerGPU.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     2901 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/RIFT/integrators/multivariate_truncnorm.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     7235 2022-10-24 14:00:10.000000 RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/RIFT/integrators/statutils.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    33113 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/RIFT/integrators/weighted_gmm.py
+drwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)        0 2023-06-19 13:22:13.211791 RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/RIFT/interpolators/
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     9944 2022-10-23 22:26:00.000000 RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/RIFT/interpolators/BayesianLeastSquares.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     3835 2022-10-23 22:26:00.000000 RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/RIFT/interpolators/ConstrainedQuadraticLikelihood.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)        0 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/RIFT/interpolators/__init__.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     2658 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/RIFT/interpolators/efficient_save_sklearn_gp.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1655 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/RIFT/interpolators/gp.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     2518 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/RIFT/interpolators/gpytorch_wrapper.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     5558 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/RIFT/interpolators/internal_GP.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     3488 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/RIFT/interpolators/interp_gpu.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    26826 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/RIFT/interpolators/senni.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)   249727 2023-06-19 13:21:23.000000 RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/RIFT/lalsimutils.py
+drwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)        0 2023-06-19 13:22:13.230791 RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/RIFT/likelihood/
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1643 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/RIFT/likelihood/Q_inner_product.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    33438 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/RIFT/likelihood/SphericalHarmonics_gpu.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)        0 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/RIFT/likelihood/__init__.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1525 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/RIFT/likelihood/cuda_Q_inner_product.cu
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    94340 2023-06-19 13:21:23.000000 RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/RIFT/likelihood/factored_likelihood.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     5269 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/RIFT/likelihood/optimized_gpu_tools.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1451 2023-05-30 17:28:25.000000 RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/RIFT/likelihood/priors_utils.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     4616 2023-06-07 15:16:25.000000 RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/RIFT/likelihood/vectorized_general_tools.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     4706 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/RIFT/likelihood/vectorized_lal_tools.py
+drwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)        0 2023-06-19 13:22:13.790794 RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/RIFT/misc/
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    70947 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/RIFT/misc/ModifiedScikitFit.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)       65 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/RIFT/misc/__init__.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    29427 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/RIFT/misc/amrlib.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     7367 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/RIFT/misc/bounded_kde.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)      229 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/RIFT/misc/common_cl.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)   109345 2023-05-24 11:46:08.000000 RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/RIFT/misc/dag_utils.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     9324 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/RIFT/misc/modules.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    23083 2022-10-11 14:57:54.000000 RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/RIFT/misc/our_corner.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    30542 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/RIFT/misc/ourparams.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    10915 2023-03-24 18:44:03.000000 RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/RIFT/misc/samples_utils.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     2901 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/RIFT/misc/sky_rotations.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    10623 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/RIFT/misc/spokes.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     6975 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/RIFT/misc/tools.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     2641 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/RIFT/misc/weight_simulations.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     8651 2023-05-30 17:28:25.000000 RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/RIFT/misc/xmlutils.py
+drwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)        0 2023-06-19 13:22:13.824794 RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/RIFT/physics/
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    26126 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/RIFT/physics/EOBTidalExternal.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    31276 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/RIFT/physics/EOBTidalExternalC.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    63809 2023-06-19 13:21:23.000000 RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/RIFT/physics/EOSManager.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     4776 2023-06-19 13:21:23.000000 RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/RIFT/physics/GWSignal.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     2654 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/RIFT/physics/MonotonicSpline.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    19507 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/RIFT/physics/PrecessingFisherMatrix.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    52302 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/RIFT/physics/ROMWaveformManager.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)       68 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/RIFT/physics/__init__.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    23733 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/RIFT/physics/effectiveFisher.py
+drwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)        0 2023-06-19 13:22:12.781790 RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/RIFT.egg-info/
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     6360 2023-06-19 13:22:09.000000 RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/RIFT.egg-info/PKG-INFO
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    10749 2023-06-19 13:22:09.000000 RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/RIFT.egg-info/SOURCES.txt
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)        1 2023-06-19 13:22:09.000000 RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/RIFT.egg-info/dependency_links.txt
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)      142 2023-06-19 13:22:09.000000 RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/RIFT.egg-info/requires.txt
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)        5 2023-06-19 13:22:09.000000 RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/RIFT.egg-info/top_level.txt
+drwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)        0 2023-06-19 13:22:14.526797 RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/bin/
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     8723 2022-10-11 14:57:54.000000 RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/bin/assess_propose_CIP_convergence_sequence.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    13848 2023-05-24 11:46:08.000000 RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/bin/calibration_reweighting.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     2371 2023-04-22 14:25:02.000000 RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/bin/combine_weights_and_rejection_sample.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     2800 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/bin/config_yank.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     6140 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/bin/convergence_test_amr.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     9039 2023-06-07 15:16:25.000000 RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/bin/convergence_test_samples.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     2239 2023-04-20 10:32:56.000000 RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/bin/convert_ascii_framechange_xphm.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1224 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/bin/convert_dat_to_hdf5.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1920 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/bin/convert_output_format_allnet2xml
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)      541 2023-03-24 18:44:03.000000 RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/bin/convert_output_format_ascii2h5.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    11799 2023-03-12 13:15:08.000000 RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/bin/convert_output_format_ile2inference
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     8166 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/bin/convert_output_format_inference2ile
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     2013 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/bin/convert_psd_ascii2xml
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     9065 2022-10-11 14:57:54.000000 RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/bin/create_CIP_convergence_sequence.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    33506 2023-04-07 18:24:37.000000 RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/bin/create_eos_posterior_pipeline
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    14569 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/bin/create_event_dag_via_grid
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    88335 2022-10-11 14:57:54.000000 RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/bin/create_event_parameter_pipeline_AlternateIteration
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)   120192 2023-04-25 00:19:30.000000 RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/bin/create_event_parameter_pipeline_BasicIteration
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    71601 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/bin/create_event_parameter_pipeline_BasicMultiApproxIteration
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     2768 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/bin/create_ile_sub_dag.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    13979 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/bin/create_postprocessing_event_dag.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    98022 2023-06-19 13:21:23.000000 RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/bin/helper_LDG_Events.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1886 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/bin/helper_OnlinePSDCleanup.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    20152 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/bin/ile_postproc_add_time
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    83560 2023-03-12 13:15:08.000000 RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/bin/integrate_likelihood_extrinsic
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)   103850 2023-06-19 13:21:23.000000 RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/bin/integrate_likelihood_extrinsic_batchmode
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    18630 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/bin/integrate_likelihood_extrinsic_no-op
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     5408 2023-03-24 18:44:03.000000 RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/bin/make_uni_comov_skymap.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    37925 2023-05-24 11:46:08.000000 RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/bin/plot_posterior_corner.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     3746 2023-03-24 18:44:03.000000 RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/bin/resample_uniform_comoving.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)      354 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/bin/switcheroo
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    34265 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/bin/util_AMRGrid.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     3696 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/bin/util_AdaptiveExponent.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    18544 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/bin/util_AnalyticFisherGrid.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     7348 2023-06-19 13:21:23.000000 RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/bin/util_BatchConvertResampleILEOutput.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1028 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/bin/util_CIPdagPostprocess.sh
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)      219 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/bin/util_CacheFileConvert.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1436 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/bin/util_CharacterizePosterior.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     3934 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/bin/util_CleanILE.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)      876 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/bin/util_CoincIFOUtility.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    15127 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/bin/util_CompareWaveformsInDetectors.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)      853 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/bin/util_ConsolidateDAGsUnderMaster.sh
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    10380 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/bin/util_ConstructBNSMarginalEOSRank.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    33198 2023-04-07 18:24:37.000000 RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/bin/util_ConstructEOSPosterior.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    55368 2022-11-28 22:41:57.000000 RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/bin/util_ConstructIntrinsicPosterior_GaussianResampling.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)   164113 2023-06-19 13:21:23.000000 RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/bin/util_ConstructIntrinsicPosterior_GenericCoordinates.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     2314 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/bin/util_CoordinateNamesAngularToCartesianSpins.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     9633 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/bin/util_EOBTideWriteFrame.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)      389 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/bin/util_EstimateWaveformDuration.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     3250 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/bin/util_FetchExternalGrid.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    27796 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/bin/util_FitAndEvaluate_GenericCoordinates.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)      256 2022-10-11 14:57:54.000000 RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/bin/util_ForOSG_MakeLocalFramesDir.sh
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1640 2023-03-12 13:15:08.000000 RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/bin/util_ForOSG_MakeTruncatedLocalFramesDir.sh
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     3266 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/bin/util_FrameZeroNoiseSNR.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    11553 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/bin/util_GenerateMaxlnLWaveform.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     6162 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/bin/util_GenerateMaxlnLWaveform_NRFromIndex.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     2223 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/bin/util_GridRecenter.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    13919 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/bin/util_GridSubsetOfTemplateBank.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     2778 2023-04-07 18:24:37.000000 RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/bin/util_HyperCombine.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1590 2023-04-07 18:24:37.000000 RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/bin/util_HyperparameterGrid.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     5156 2023-04-07 18:24:37.000000 RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/bin/util_HyperparameterPuffball.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)      829 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/bin/util_ILENextGeneration.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1018 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/bin/util_ILEROMdagPostprocess.sh
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1597 2022-10-11 14:57:54.000000 RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/bin/util_ILEdagPostprocess.sh
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     6780 2023-03-24 18:44:03.000000 RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/bin/util_InitMargTable
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     4553 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/bin/util_IntermediateEOSIntegralFromFit.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    40228 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/bin/util_IterativeFisher.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     2698 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/bin/util_JoinXML.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     8109 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/bin/util_LALCompareApproximantsOnSamples.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     7660 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/bin/util_LALWriteFrame.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    50356 2022-10-11 14:57:54.000000 RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/bin/util_ManualOverlapGrid.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     7195 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/bin/util_MarginalizedLikelihoodEOSIntegralFromIntermediate.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1214 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/bin/util_MassGrid.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     2450 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/bin/util_MassGridCoalesce.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     8821 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/bin/util_NRBestOfIndex.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     6671 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/bin/util_NRDumpDetectorResponse.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    20394 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/bin/util_NRExtrudeOverlapGrid.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     5672 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/bin/util_NRIndexedFminCutToILE.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    10752 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/bin/util_NRNearestSimulationTo.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     4794 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/bin/util_NRRelabelILE.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     9830 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/bin/util_NRWriteFrame.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     3377 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/bin/util_NR_GWMemory.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1490 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/bin/util_NRdagPostprocess.sh
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     2349 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/bin/util_ParameterFilter.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    12414 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/bin/util_ParameterPuffball.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     3665 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/bin/util_ParameterRandomize.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1087 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/bin/util_PosteriorPostprocess.sh
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     3302 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/bin/util_PrintInjection.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     5424 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/bin/util_RIFT_MultiMetaPipe.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    79435 2023-06-07 15:16:25.000000 RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/bin/util_RIFT_pseudo_pipe.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    35804 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/bin/util_RIFT_pseudo_pipe_lowlatency.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     6293 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/bin/util_ROMWriteFrame.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1675 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/bin/util_RandomizeOverlapOrder.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     3080 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/bin/util_ResampleILEOutputWithExtrinsic.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     3792 2023-03-24 18:44:03.000000 RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/bin/util_SimInspiralToCoinc.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     7587 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/bin/util_TEOBResumSWriteFrame.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     4982 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/bin/util_TestSpokesIO.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)      814 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/bin/util_TestXMLParameterStorage.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    11254 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/bin/util_TidalPlotSimulationStrain.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)      457 2022-10-15 00:56:03.000000 RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/bin/util_TruncateMergeFrames.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     3430 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/bin/util_WriteFrameAndCacheFromXML.sh
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     2784 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/bin/util_WriteInjectionFile.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1955 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/bin/util_WriteXMLWithEOS.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)      276 2023-04-22 14:25:02.000000 RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/bin/util_shuffle_file.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     3488 2022-09-24 12:18:48.000000 RIFT-0.0.15.9rc4/PACKAGING.md
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     6360 2023-06-19 13:22:14.534797 RIFT-0.0.15.9rc4/PKG-INFO
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     5821 2023-04-07 18:24:37.000000 RIFT-0.0.15.9rc4/README.md
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     6132 2022-09-24 12:18:48.000000 RIFT-0.0.15.9rc4/TROUBLESHOOTING.md
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     6136 2022-09-24 12:18:48.000000 RIFT-0.0.15.9rc4/howto.md
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)       96 2023-04-24 19:45:36.000000 RIFT-0.0.15.9rc4/pyproject.toml
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)      184 2023-03-24 18:44:03.000000 RIFT-0.0.15.9rc4/requirements.txt
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)       38 2023-06-19 13:22:14.535797 RIFT-0.0.15.9rc4/setup.cfg
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     2934 2023-06-19 13:21:23.000000 RIFT-0.0.15.9rc4/setup.py
```

### Comparing `RIFT-0.0.15.9rc3/AUTOMATED_OR_ONLINE.md` & `RIFT-0.0.15.9rc4/AUTOMATED_OR_ONLINE.md`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc3/Dockerfile` & `RIFT-0.0.15.9rc4/Dockerfile`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc3/GETTING_STARTED.md` & `RIFT-0.0.15.9rc4/GETTING_STARTED.md`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc3/INSTALL.md` & `RIFT-0.0.15.9rc4/INSTALL.md`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc3/INSTALL_OPTIONAL_DEPENDENCIES.md` & `RIFT-0.0.15.9rc4/INSTALL_OPTIONAL_DEPENDENCIES.md`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc3/LICENSE.md` & `RIFT-0.0.15.9rc4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/RIFT/calmarg/rift_source.py` & `RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/RIFT/calmarg/rift_source.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/RIFT/integrators/MonteCarloEnsemble.py` & `RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/RIFT/integrators/MonteCarloEnsemble.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/RIFT/integrators/direct_quadrature.py` & `RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/RIFT/integrators/direct_quadrature.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/RIFT/integrators/gaussian_mixture_model.py` & `RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/RIFT/integrators/gaussian_mixture_model.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/RIFT/integrators/mcsampler.py` & `RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/RIFT/integrators/mcsampler.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/RIFT/integrators/mcsamplerEnsemble.py` & `RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/RIFT/integrators/mcsamplerEnsemble.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/RIFT/integrators/mcsamplerGPU.py` & `RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/RIFT/integrators/mcsamplerGPU.py`

 * *Files 1% similar despite different names*

```diff
@@ -1363,24 +1363,29 @@
 
 def pseudo_dist_samp(r0,r):
         return r*r*numpy.exp( - (r0/r)*(r0/r)/2. + r0/r)+0.01  # put a floor on probability, so we converge. Note this floor only cuts out NEARBY distances
 
 #pseudo_dist_samp_vector = numpy.vectorize(pseudo_dist_samp,excluded=['r0'],otypes=[numpy.float64])
 pseudo_dist_samp_vector = numpy.vectorize(pseudo_dist_samp,otypes=[numpy.float64])
 
-def delta_func_pdf(x_0, x):
-    return 1.0 if x == x_0 else 0.0
-
-delta_func_pdf_vector = numpy.vectorize(delta_func_pdf, otypes=[numpy.float64])
-
-def delta_func_samp(x_0, x):
-    return x_0
-
-delta_func_samp_vector = numpy.vectorize(delta_func_samp, otypes=[numpy.float64])
-
+if xpy_default == numpy:
+  def delta_func_pdf(x_0, x):
+     return 1.0 if x == x_0 else 0.0
+  delta_func_pdf_vector = xpy_default.vectorize(delta_func_pdf, otypes=[xpy_default.float64])
+else:
+   # only called on data which already satisfies the constraint, so return 1
+   delta_func_pdf_vector = lambda x,y: xpy_default.ones(y.shape)
+
+if xpy_default==numpy:
+ def delta_func_samp(x_0, x):
+     return x_0
+ delta_func_samp_vector = xpy_default.vectorize(delta_func_samp, otypes=[xpy_default.float64])
+else:
+ # return value equal to the requested floating point constant
+ delta_func_samp_vector = lambda x,y: x*xpy_default.ones(y.shape)
 
 
 def sanityCheckSamplerIntegrateUnity(sampler,*args,**kwargs):
         return sampler.integrate(lambda *args: 1,*args,**kwargs)
 
 ###
 ### CONVERGENCE TESTS
```

### Comparing `RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/RIFT/integrators/multivariate_truncnorm.py` & `RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/RIFT/integrators/multivariate_truncnorm.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/RIFT/integrators/statutils.py` & `RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/RIFT/integrators/statutils.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/RIFT/integrators/weighted_gmm.py` & `RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/RIFT/integrators/weighted_gmm.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/RIFT/interpolators/BayesianLeastSquares.py` & `RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/RIFT/interpolators/BayesianLeastSquares.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/RIFT/interpolators/ConstrainedQuadraticLikelihood.py` & `RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/RIFT/interpolators/ConstrainedQuadraticLikelihood.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/RIFT/interpolators/efficient_save_sklearn_gp.py` & `RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/RIFT/interpolators/efficient_save_sklearn_gp.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/RIFT/interpolators/gp.py` & `RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/RIFT/interpolators/gp.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/RIFT/interpolators/gpytorch_wrapper.py` & `RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/RIFT/interpolators/gpytorch_wrapper.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/RIFT/interpolators/internal_GP.py` & `RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/RIFT/interpolators/internal_GP.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/RIFT/interpolators/interp_gpu.py` & `RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/RIFT/interpolators/interp_gpu.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/RIFT/interpolators/senni.py` & `RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/RIFT/interpolators/senni.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/RIFT/lalsimutils.py` & `RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/RIFT/lalsimutils.py`

 * *Files 0% similar despite different names*

```diff
@@ -2405,15 +2405,15 @@
 
 def CreateCompatibleComplexOverlap(hlmf,**kwargs):
     """
     CreateCompatibleComplexOverlap: accepts dictionary or single instance of COMPLEX16FrequencySeries
     """
     if isinstance(hlmf, dict):
         modes = hlmf.keys()
-        hbase = hlmf[modes[0]]
+        hbase = hlmf[list(modes)[0]]
     else:
         hbase =hlmf
     deltaF = hbase.deltaF
     fNyq = hbase.deltaF*hbase.data.length/2 # np.max(evaluate_fvals(hbase))
     if rosDebugMessagesContainer[0]:
         print( kwargs)
         print( "dF, fNyq, npts = ",deltaF, fNyq, len(hbase.data.data))
@@ -2422,15 +2422,15 @@
 
 def CreateCompatibleComplexIP(hlmf,**kwargs):
     """
     Creates complex IP (no maximization)
     """
     if isinstance(hlmf, dict):
         modes = hlmf.keys()
-        hbase = hlmf[modes[0]]
+        hbase = hlmf[list(modes)[0]]
     else:
         hbase =hlmf
     deltaF = hbase.deltaF
     fNyq = hbase.deltaF*hbase.data.length/2 # np.max(evaluate_fvals(hbase))
     if rosDebugMessagesContainer[0]:
         print( kwargs)
         print( "dF, fNyq, npts = ",deltaF, fNyq, len(hbase.data.data))
```

### Comparing `RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/RIFT/likelihood/Q_inner_product.py` & `RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/RIFT/likelihood/Q_inner_product.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/RIFT/likelihood/SphericalHarmonics_gpu.py` & `RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/RIFT/likelihood/SphericalHarmonics_gpu.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/RIFT/likelihood/cuda_Q_inner_product.cu` & `RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/RIFT/likelihood/cuda_Q_inner_product.cu`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/RIFT/likelihood/factored_likelihood.py` & `RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/RIFT/likelihood/factored_likelihood.py`

 * *Files 0% similar despite different names*

```diff
@@ -191,15 +191,15 @@
                         del hlms_conj[mode]
                         continue
 
 
     elif use_gwsignal and (has_GWS):  # this MUST be called first, so the P.approx is never tested
         if not quiet:
             print( "  FACTORED LIKELIHOOD WITH hlmoff (GWsignal) " )            
-        hlms, hlms_conj = rgws.std_and_conj_hlmoff(P,Lmax,approx_string=use_gwsignal_approx)
+        hlms, hlms_conj = rgws.std_and_conj_hlmoff(P,Lmax,approx_string=use_gwsignal_approx,**extra_waveform_kwargs)
 
     elif (not nr_lookup) and (not NR_group) and ( P.approx ==lalsim.SEOBNRv2 or P.approx == lalsim.SEOBNRv1 or P.approx==lalsim.SEOBNRv3 or P.approx == lsu.lalSEOBv4 or P.approx ==lsu.lalSEOBNRv4HM or P.approx == lalsim.EOBNRv2 or P.approx == lsu.lalTEOBv2 or P.approx==lsu.lalTEOBv4 ):
         # note: alternative to this branch is to call hlmoff, which will actually *work* if ChooseTDModes is propertly implemented for that model
         #   or P.approx == lsu.lalSEOBNRv4PHM or P.approx == lsu.lalSEOBNRv4P  
         if not quiet:
                 print("  FACTORED LIKELIHOOD WITH SEOB ")
         hlmsT = {}
```

### Comparing `RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/RIFT/likelihood/optimized_gpu_tools.py` & `RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/RIFT/likelihood/optimized_gpu_tools.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/RIFT/likelihood/priors_utils.py` & `RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/RIFT/likelihood/priors_utils.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/RIFT/likelihood/vectorized_general_tools.py` & `RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/RIFT/likelihood/vectorized_general_tools.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/RIFT/likelihood/vectorized_lal_tools.py` & `RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/RIFT/likelihood/vectorized_lal_tools.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/RIFT/misc/ModifiedScikitFit.py` & `RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/RIFT/misc/ModifiedScikitFit.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/RIFT/misc/amrlib.py` & `RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/RIFT/misc/amrlib.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/RIFT/misc/bounded_kde.py` & `RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/RIFT/misc/bounded_kde.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/RIFT/misc/dag_utils.py` & `RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/RIFT/misc/dag_utils.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/RIFT/misc/modules.py` & `RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/RIFT/misc/modules.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/RIFT/misc/our_corner.py` & `RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/RIFT/misc/our_corner.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/RIFT/misc/ourparams.py` & `RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/RIFT/misc/ourparams.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/RIFT/misc/samples_utils.py` & `RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/RIFT/misc/samples_utils.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/RIFT/misc/sky_rotations.py` & `RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/RIFT/misc/sky_rotations.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/RIFT/misc/spokes.py` & `RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/RIFT/misc/spokes.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/RIFT/misc/tools.py` & `RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/RIFT/misc/tools.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/RIFT/misc/weight_simulations.py` & `RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/RIFT/misc/weight_simulations.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/RIFT/misc/xmlutils.py` & `RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/RIFT/misc/xmlutils.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/RIFT/physics/EOBTidalExternal.py` & `RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/RIFT/physics/EOBTidalExternal.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/RIFT/physics/EOBTidalExternalC.py` & `RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/RIFT/physics/EOBTidalExternalC.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/RIFT/physics/EOSManager.py` & `RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/RIFT/physics/EOSManager.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,16 +31,16 @@
     import pyreprimand as pyr
     has_reprimand=True
 except:
     has_reprimand=False
 
 #import gwemlightcurves.table as gw_eos_table
 
-from . import MonotonicSpline as ms
-#from RIFT.physics import MonotonicSpline as ms
+try:    from .            import MonotonicSpline as ms
+except: from RIFT.physics import MonotonicSpline as ms
 
 C_CGS=lal.C_SI*100
 DENSITY_CGS_IN_MSQUARED=1000*lal.G_SI/lal.C_SI**2  # g/cm^3 -> 1/m^2 //GRUnits. Multiply by this to convert from CGS -> 1/m^2 units (_geom). lal.G_SI/lal.C_SI**2 takes kg/m^3 -> 1/m^2  ||  https://lscsoft.docs.ligo.org/lalsuite/lalsimulation/_l_a_l_sim_neutron_star_8h_source.html
 PRESSURE_CGS_IN_MSQUARED = DENSITY_CGS_IN_MSQUARED/(lal.C_SI*100)**2
 
 
 def make_compactness_from_lambda_approximate(lambda_vals):
@@ -634,15 +634,15 @@
         
         self.spec_params = spec_params
         
         if use_lal_spec_eos:
             try:
                 self.eos = lalsim.SimNeutronStarEOS4ParamCausalSpectralDecomposition(spec_params['gamma1'], spec_params['gamma2'], spec_params['gamma3'], spec_params['gamma4'])
             except:
-                raise Exception("Did not send spec_params along. Please do, or turn 'use_lal_spec_eos' = False and expect a table to be read.")
+                raise Exception("A reasonable spec_params was not provided by the user. Please provide spec_params, or turn 'use_lal_spec_eos' = False and the code will expect an EoS table to be read.")
         else:
             # Create data file
             self.make_spec_param_eos(500,save_dat=True,ligo_units=True,verbose=verbose)
             # Use data file
             #print " Trying to load ",name+"_geom.dat"
             import os; #print os.listdir('.')
             cwd = os.getcwd()
@@ -707,26 +707,26 @@
 
 # https://github.com/oshaughn/RIT-matters/blob/master/communications/20230130-ROSKediaYelikar-EOSManagerSpectralUpdates/demo_reprimand.py
 class EOSReprimand(EOSConcrete):
     """Pass param_dict as the dictionary of 'pseudo_enthalpy','rest_mass_density','energy_density','pressure','sound_speed_over_c' for being resolved into a TOV sequence. CGS Units only except sound_speed_over_c.
     Instead you can send a lalsim_eos which processes lalsim eos object type and produces a TOV sequence.
     load_eos takes a 2D array with pressure, energy_density and rest_mass_density (not tested).
     """
-    def __init__(self,name=None,param_dict=None,lalsim_eos=None,load_eos = None, specific_internal_energy = True, m_b_units = lal.MP_SI):
+    def __init__(self,name=None,param_dict=None,lalsim_eos=None,load_eos = None, specific_internal_energy = True, m_b_units = lal.MP_SI, RePrimAnd_scale = 1e-6):
         self.name              = name
         self.pyr_eos           = None # REQUIRED, new name for reprimand structure. Provided so we can also back-port converting between two
         self.tov_seq_reprimand = None   # Stores RePrimAnd eos object
         self.eos_lal           = lalsim_eos  # NOT required, only would be useful for talking to lalsim
         self.mMaxMsun          = None  # required
         self._pyr_mrL_dat      = None # internal data for M_g, R, lambda, M_b
-        self.m_b_units         = m_b_units # Base units for baryon mass for the EOS. Leave this as it is unless you want tune mass of nucleons from 1.66e-27 to 1.67e-27 kg.
+        self.m_b_units         = m_b_units # Base units for baryon mass for the EOS. To see why it was added in the first place, see RIFT v 0.0.15.8 and https://git.ligo.org/rapidpe-rift/rapidpe_rift_review_o4/-/wikis/Review:20230509.
         if self.eos_lal is None and load_eos is not None: self.eos_lal = EOSFromTabularData(eos_data=load_eos).eos
         
         if param_dict:
-            self.update(param_dict,specific_internal_energy)
+            self.update(param_dict,specific_internal_energy, RePrimAnd_scale)
         elif self.eos_lal is not None: # process LALSim EOS object
             min_pseudo_enthalpy = 0.005
             max_pseudo_enthalpy = lalsim.SimNeutronStarEOSMaxPseudoEnthalpy(self.eos_lal)
             hvals = max_pseudo_enthalpy* 10**np.linspace( np.log10(min_pseudo_enthalpy/max_pseudo_enthalpy),  0,num=500)
             qry_object = QueryLS_EOS(self.eos_lal)
             
             param_dict = dict()
@@ -734,68 +734,70 @@
             param_dict['rest_mass_density'] = qry_object.extract_param('rest_mass_density',hvals)
             param_dict['energy_density'] = qry_object.extract_param('energy_density',hvals)
             param_dict['pressure'] = qry_object.extract_param('pressure',hvals)
             param_dict['sound_speed_over_c'] = qry_object.extract_param('sound_speed_over_c',hvals)
             
             #just_check_monotonicity_and_causality(param_dict)
             #param_dict = eos_monotonic_parts_and_causal_sound_speed(param_dict,preserve_same_length = False) # Don't enable by default. First check if monotonicity or causality is violated indeed, and document if it does.
-            self.update(param_dict,specific_internal_energy)
+            self.update(param_dict,specific_internal_energy, RePrimAnd_scale)
         else:
             print(" Warning: Empty EOS object created")
         return None
     
-    def update(self,param_dict,specific_internal_energy):
+    def update(self,param_dict,specific_internal_energy, RePrimAnd_scale = 1e-6):
         # minimum required input, cgs units like everything else above
         # for example, you could get this from QueryLS_EOS.extract_param(name, xvals) for xvals your parameter
         #p_enthalpy = param_dict['pseudo_enthalpy']
         rho    = param_dict['rest_mass_density']
         edens  = param_dict['energy_density']
         press  = param_dict['pressure']
         cs     = param_dict['sound_speed_over_c']
         
         unew = pyr.units.geom_solar(msun_si=lal.MSUN_SI) # the argument normalizes to our units.
         spec_int_energy = edens/(rho*1.66e-27/self.m_b_units) -1  # 1.66e-27 kg is the baryon mass used in reprimand. 
         
         # 1000, and 0.1 are converting cgs quantities to SI.
         spec_int_energy_unew = spec_int_energy
-        rho_unew = rho*1000/unew.density
+        rho_unew = rho*1.66e-27/self.m_b_units*1000/unew.density # 1.66e-27/self.m_b_units is multiplied to convert rho to RePrimAnd's mass scale.
         press_unew = press*0.1/unew.pressure
         
         temp, efrac= [], []
         n_poly=1.7115960633290546  # polytropic index below lowest tabular data. Not good, should have full range.
         eps_0 = 0.0  # energy density at zero pressure
-        pts_per_mag =1000  # points log spaced per decaded in some parameter
+        pts_per_mag =800  # points log spaced per decaded in some parameter
         isentropic = True
         rgrho = pyr.range(min(rho_unew)*1.0000001, max(rho_unew) / 1.0000001)
         
         # Instantiate EOS
         if specific_internal_energy: self.pyr_eos = pyr.make_eos_barotr_spline(rho_unew, spec_int_energy_unew, press_unew, cs, temp, efrac, isentropic, rgrho, n_poly, unew, pts_per_mag)
         else: self.pyr_eos = pyr.make_eos_barotr_spline(rho_unew, press_unew, cs, temp, efrac, rgrho, n_poly, eps_0, unew, pts_per_mag)
         # pyr.make_eos_barotr_spline(gm1, rho_unew, spec_int_energy_unew, press_unew, cs, temp, efrac, isentropic, rgrho, n_poly, unew, pts_per_mag)
         
-        self._pyr_mrL_dat, self.tov_seq_reprimand = make_mr_lambda_reprimand(self.pyr_eos,return_eos_object=True, m_b_units = self.m_b_units)
+        self._pyr_mrL_dat, self.tov_seq_reprimand = make_mr_lambda_reprimand(self.pyr_eos,return_eos_object=True, m_b_units = self.m_b_units, RePrimAnd_scale = RePrimAnd_scale)
         self.mMaxMsun = max(self._pyr_mrL_dat[:,0])
         
         return None
     
     def baryon_mass_from_mg(self,mg):
         return self.tov_seq_reprimand.bary_mass_from_grav_mass(mg)*self.m_b_units/1.66e-27
     
     def lambda_from_m(self,mg):
         try:    # single element
+            # If mg is in solar mass units(~2), it is << 1e15
             if mg <1e15: return self.tov_seq_reprimand.lambda_tidal_from_grav_mass(mg)
+            # If mg is in SI units (~4e30), it is >> 1e15            
             return self.tov_seq_reprimand.lambda_tidal_from_grav_mass(mg/lal.MSUN_SI)
-        except: # multi element
+        except: # multi element array
             mg = np.array(mg)
             if mg[0] <1e15: return self.tov_seq_reprimand.lambda_tidal_from_grav_mass(mg)
             return self.tov_seq_reprimand.lambda_tidal_from_grav_mass(mg/lal.MSUN_SI)
 
 
 # RePrimAnd
-def make_mr_lambda_reprimand(eos,n_bins=800,save_tov_sequence=False,read_tov_sequence=False,return_eos_object=False, m_b_units = lal.MP_SI):
+def make_mr_lambda_reprimand(eos,n_bins=800,save_tov_sequence=False,read_tov_sequence=False,return_eos_object=False, m_b_units = lal.MP_SI, RePrimAnd_scale = 1e-6):
     """
     Construct mass-radius curve from EOS using RePrimAnd (https://wokast.github.io/RePrimAnd/tov_solver.html).
     Parameter `eos` should be in RePrimAnd's eos object format, made with something like `make_eos_barotr_spline` (https://wokast.github.io/RePrimAnd/eos_barotr_ref.html).
     By default this returns the Mass_g-Radius-Lambda-Mass_b. But if `return_eos_object` is True, this will also return the RePrimAnd EOS object.
     Wolfgang Kastaun, Jay Vijay Kalinani, and Riccardo Ciolfi. Robust recovery of primitive variables in relativistic ideal magnetohydrodynamics. Phys. Rev. D, 103(2):023018, 2021. doi:10.1103/PhysRevD.103.023018.
     Roland Haas and Wolfgang Kastaun. (2023). wokast/RePrimAnd: Release 1.6 (v1.6). Zenodo. https://doi.org/10.5281/zenodo.7700296
     """
@@ -813,15 +815,15 @@
     geom_umass(umass, g_si) : divides everything such that mass = umass given. DID NOT CHECK g_si dependence.
     # Units of quantities
     density is in SI/6.1758e+20 i.e. 1.98841e+30/1476.625**3 = pyr.units.geom_solar().mass / pyr.units.geom_solar().length**3
     """
     assert has_reprimand
     
     #Make TOV sequence
-    acc_tov=1e-10; acc_deform=1e-8; minsteps=500; num_samp=2500; mgrav_min=0.3
+    acc_tov=RePrimAnd_scale*1e-2; acc_deform=RePrimAnd_scale; minsteps=500; num_samp=2000; mgrav_min=0.3
     acc = pyr.tov_acc_simple(acc_tov, acc_deform, minsteps)
     try: seq = pyr.make_tov_branch_stable(eos, acc, num_samp=num_samp, mgrav_min=mgrav_min)
     except:
         if read_tov_sequence:
             sol_units = pyr.units.geom_solar(msun_si=lal.MSUN_SI)
             seq = pyr.load_star_branch(eos, sol_units)
         else: raise Exception("No EOS supplied.")
@@ -910,14 +912,16 @@
                       'pressure': param_dict['pressure'][below_speed_of_light],
                       'sound_speed_over_c': param_dict['sound_speed_over_c'][below_speed_of_light]}
     else: param_dict['sound_speed_over_c'][np.where(param_dict['sound_speed_over_c']> 1)[0]] = 1
     return param_dict
 
 
 def eos_monotonic_parts_and_causal_sound_speed(param_dict, preserve_same_length = False):
+    """rest_mass_density , energy_density, pressure, pseudo_enthalpy, and sound_speed_over_c are the dictionary parameters that this function expects.
+    """
     param_dict_main = {'rest_mass_density': param_dict['rest_mass_density'], 'energy_density': param_dict['energy_density'],'pressure': param_dict['pressure']}
     param_dict_others = {'pseudo_enthalpy': param_dict['pseudo_enthalpy'], 'sound_speed_over_c': param_dict['sound_speed_over_c']}
     
     check_monotonic(param_dict_main, param_dict_others, preserve_same_length=preserve_same_length)
     
     param_dict = {'pseudo_enthalpy': param_dict_others['pseudo_enthalpy'],
                   'rest_mass_density': param_dict_main['rest_mass_density'],
@@ -1307,15 +1311,15 @@
         Den_SI_to_CGS = 0.001 # kg m^-3 -> g cm^-3
         Energy_SI_to_CGS = 10/(lal.C_SI*100)**2 # J m^-3 *10 -> erg/cm^3 /c^2 -> g cm^-3
         Press_SI_to_CGS = 10 # Pa -> Ba ~ g cm^-1 s^-2
         
         extraction_dict_lalsim_raw = {
             'pseudo_enthalpy'   : lambda x: x,
             'rest_mass_density' : lambda x: lalsim.SimNeutronStarEOSRestMassDensityOfPseudoEnthalpy(x, eos)*Den_SI_to_CGS,
-            'baryon_density'    : lambda x: lalsim.SimNeutronStarEOSRestMassDensityOfPseudoEnthalpy(x, eos)*Den_SI_to_CGS/(lal.AMU_SI*1e3),  #  cm^-3
+            'baryon_density'    : lambda x: lalsim.SimNeutronStarEOSRestMassDensityOfPseudoEnthalpy(x, eos)*Den_SI_to_CGS/(lal.MP_SI*1e3),  #  cm^-3
             'pressure'          : lambda x: lalsim.SimNeutronStarEOSPressureOfPseudoEnthalpy(x, eos)*Press_SI_to_CGS,
             'energy_density'    : lambda x: lalsim.SimNeutronStarEOSEnergyDensityOfPseudoEnthalpy(x,eos)*Energy_SI_to_CGS,
             'sound_speed_over_c': lambda x: lalsim.SimNeutronStarEOSSpeedOfSound(x,eos)/lal.C_SI
             }
         self.extraction_dict_lalsim = {}
         for name in         extraction_dict_lalsim_raw:
             self.extraction_dict_lalsim[name] = np.vectorize(extraction_dict_lalsim_raw[name])
@@ -1325,16 +1329,16 @@
             raise Exception("Variable required to convert.")
         if var_name == 'rest_mass_density':
             return var*lal.C_SI**2/(lal.QE_SI*1e48) # MeV fm^-3    ## c**2/(coulomb charge) * 1/(10**39 * 10**3 * 10**6) See https://en.wikipedia.org/wiki/Electronvolt#Mass for a handy conversion. lal.C_SI**2/(lal.QE_SI*10**48) = 5.6096*10**-13
         if var_name == 'energy_density':
             return var*lal.C_SI**2/(lal.QE_SI*1e48) # MeV fm^-3
         if var_name == 'energy_density_n_sat':
             return var/(2.7e14) # nuclear saturation density in cgs = 2.7*10**14. ~ 0.16 fm^-3
-        if var_name == 'sound_speed_over_c':
-            return var*lal.C_SI*100   # cm s-1
+        if var_name == 'sound_speed_to_cm_s':
+            return var*lal.C_SI*1e2   # cm s-1
         if var_name == 'pressure':
             raise Exception('not yet implemented')
             return ##Check this conversion. possibly same as density with or without c**2. [MeV fm^-3]
         
         # IN PROGRESS
         #   - adiabatic index
         #Gamma = (self.extraction_dict_lalsim['energy_density']()*(lal.C_SI*100)**2 + self.extraction_dict_lalsim['pressure']())/(self.extraction_dict_lalsim['pressure']()) *np.square(self.extraction_dict_lalsim['sound_speed_over_c']())
```

### Comparing `RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/RIFT/physics/GWSignal.py` & `RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/RIFT/physics/GWSignal.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,25 +29,25 @@
     has_gws=True
 except:
     has_gws=False
     print("GWsignal import failed")
 
 
 def std_and_conj_hlmoff(P, Lmax=2,approx_string=None,**kwargs):
-    hlms = hlmoft(P, Lmax,approx_string=approx_string)
+    hlms = hlmoft(P, Lmax,approx_string=approx_string,**kwargs)
     hlmsF = {}
     hlms_conj_F = {}
     for mode in hlms:
         hlmsF[mode] = lalsimutils.DataFourier(hlms[mode])
         hlms[mode].data.data = np.conj(hlms[mode].data.data)
         hlms_conj_F[mode] = lalsimutils.DataFourier(hlms[mode])
     return hlmsF, hlms_conj_F
 
 def hlmoff(P, Lmax=2,approx_string=None,**kwargs):
-    hlms = hlmoft(P, Lmax,approx_string=approx_string)
+    hlms = hlmoft(P, Lmax,approx_string=approx_string,**kwargs)
     hlmsF = {}
     for mode in hlms:
         hlmsF[mode] = lalsimutils.DataFourier(hlms[mode])
     return hlmsF
 
 
 def hlmoft(P, Lmax=2,approx_string=None,**kwargs):
@@ -76,14 +76,16 @@
               'phi_ref' : P.phiref*u.rad,
               'distance' : P.dist/(1e6*lal.PC_SI)*u.Mpc,
               'inclination' : P.incl*u.rad,
               'eccentricity' : P.eccentricity*u.dimensionless_unscaled,
               'longAscNodes' : P.psi*u.rad,
               'meanPerAno' : P.meanPerAno*u.rad,
               'condition' : taper}
+    if 'lmax_nyquist' in kwargs:
+        python_dict['lmax_nyquist'] = kwargs['lmax_nyquist']
 
     # if needed
 #    lal_dict = gws.core.utils.to_lal_dict(python_dict)
 
     approx_string_here = approx_string
     if not(approx_string):
         approx_string_here = lalsim.GetStringFromApproximant(P.approx)
```

### Comparing `RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/RIFT/physics/MonotonicSpline.py` & `RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/RIFT/physics/MonotonicSpline.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/RIFT/physics/PrecessingFisherMatrix.py` & `RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/RIFT/physics/PrecessingFisherMatrix.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/RIFT/physics/ROMWaveformManager.py` & `RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/RIFT/physics/ROMWaveformManager.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/RIFT/physics/effectiveFisher.py` & `RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/RIFT/physics/effectiveFisher.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/RIFT.egg-info/PKG-INFO` & `RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/RIFT.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RIFT
-Version: 0.0.15.9rc3
+Version: 0.0.15.9rc4
 Summary: RIFT parameter estimation pipeline. Note branch used is temp-RIT-Tides-port_python3_restructure_package (which will become master shortly)!
 Home-page: https://git.ligo.org/rapidpe-rift/rift
 Author: Richard O'Shaughnessy
 Author-email: richard.oshaughnessy@ligo.org
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/RIFT.egg-info/SOURCES.txt` & `RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/RIFT.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/bin/assess_propose_CIP_convergence_sequence.py` & `RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/bin/assess_propose_CIP_convergence_sequence.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/bin/calibration_reweighting.py` & `RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/bin/calibration_reweighting.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/bin/combine_weights_and_rejection_sample.py` & `RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/bin/combine_weights_and_rejection_sample.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/bin/config_yank.py` & `RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/bin/config_yank.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/bin/convergence_test_amr.py` & `RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/bin/convergence_test_amr.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/bin/convergence_test_samples.py` & `RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/bin/convergence_test_samples.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/bin/convert_ascii_framechange_xphm.py` & `RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/bin/convert_ascii_framechange_xphm.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/bin/convert_dat_to_hdf5.py` & `RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/bin/convert_dat_to_hdf5.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/bin/convert_output_format_allnet2xml` & `RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/bin/convert_output_format_allnet2xml`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/bin/convert_output_format_ascii2h5.py` & `RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/bin/convert_output_format_ascii2h5.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/bin/convert_output_format_ile2inference` & `RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/bin/convert_output_format_ile2inference`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/bin/convert_output_format_inference2ile` & `RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/bin/convert_output_format_inference2ile`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/bin/convert_psd_ascii2xml` & `RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/bin/convert_psd_ascii2xml`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/bin/create_CIP_convergence_sequence.py` & `RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/bin/create_CIP_convergence_sequence.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/bin/create_eos_posterior_pipeline` & `RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/bin/create_eos_posterior_pipeline`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/bin/create_event_dag_via_grid` & `RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/bin/create_event_dag_via_grid`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/bin/create_event_parameter_pipeline_AlternateIteration` & `RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/bin/create_event_parameter_pipeline_AlternateIteration`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/bin/create_event_parameter_pipeline_BasicIteration` & `RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/bin/create_event_parameter_pipeline_BasicIteration`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/bin/create_event_parameter_pipeline_BasicMultiApproxIteration` & `RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/bin/create_event_parameter_pipeline_BasicMultiApproxIteration`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/bin/create_ile_sub_dag.py` & `RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/bin/create_ile_sub_dag.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/bin/create_postprocessing_event_dag.py` & `RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/bin/create_postprocessing_event_dag.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/bin/helper_LDG_Events.py` & `RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/bin/helper_LDG_Events.py`

 * *Files 1% similar despite different names*

```diff
@@ -824,14 +824,15 @@
 tmp1,tmp2 = lalsimutils.m1m2(1,eta_min)
 delta_max_tight= delta_max =(tmp1-tmp2)/(tmp1+tmp2)  # about 0.8
 delta_min_tight = delta_min =1e-4  # Some approximants like SEOBNRv3 can hard fail if m1=m2
 if not(opts.force_eta_range is None):
     tmp = opts.force_eta_range 
     eta_range_parsed = list(map(float,tmp.replace('[','').replace(']','').split(',')))
     delta_min_tight = np.sqrt(1 - 4*eta_range_parsed[1]) + 1e-4
+    delta_max_tight = np.sqrt(1 - 4*eta_range_parsed[0])
 if mc_center < 2.6 and opts.propose_initial_grid:  # BNS scale, need to constraint eta to satisfy mc > 1
     import scipy.optimize
     # solution to equation with m2 -> 1 is  1 == mc delta 2^(1/5)/(1-delta^2)^(3/5), which is annoying to solve
     def crit_m2(delta):
         eta_val = 0.25*(1-delta*delta)
         return 0.5*mc_center*(eta_val**(-3./5.))*(1-delta) - 1.
     res = scipy.optimize.brentq(crit_m2, 0.001,0.999) # critical value of delta: largest possible for this mc value
@@ -1506,23 +1507,28 @@
         helper_cip_arg_list.append(helper_cip_arg_list[-1]) 
         helper_cip_arg_list[-1] +=  " --parameter-implied DeltaLambdaTilde "
 
         n_its = map(lambda x: float(x.split()[0]), helper_cip_arg_list)
         puff_max_it= np.sum(n_its) # puff all the way to the end
     elif opts.internal_tabular_eos_file:
         helper_cip_args = " --tabular-eos-file {} ".format(opts.internal_tabular_eos_file)
+        helper_cip_args+= " --parameter-implied LambdaTilde "
         for indx in np.arange(len(helper_cip_arg_list)):
-            helper_cip_arg_list[indx] += " --tabular-eos-file {} ".format(opts.internal_tabular_eos_file)
+            helper_cip_arg_list[indx] += " --parameter-implied LambdaTilde --tabular-eos-file {} ".format(opts.internal_tabular_eos_file)
+        helper_cip_arg_list[-1] += "  --parameter-implied DeltaLambdaTilde "
     elif opts.assume_matter_eos:
         helper_cip_args += "  --input-tides --using-eos {} ".format(opts.assume_matter_eos)
+        helper_cip_args+= " --parameter-implied LambdaTilde "
         if opts.assume_matter_but_primary_bh:
             helper_cip_args += " --assume-eos-but-primary-bh "
         for indx in np.arange(len(helper_cip_arg_list)):
-            helper_cip_arg_list[indx] += " --using-eos {} ".format(opts.assume_matter_eos)
-            helper_cip_args_list[indx] += " --assume-eos-but-primary-bh "
+            helper_cip_arg_list[indx] += " --input-tides  --parameter-implied LambdaTilde --using-eos {} ".format(opts.assume_matter_eos)
+            if opts.assume_matter_but_primary_bh:
+                helper_cip_arg_list[indx] += " --assume-eos-but-primary-bh "
+        helper_cip_arg_list[-1] += "  --parameter-implied DeltaLambdaTilde "
 # lnL-offset was already enforced
 #    if opts.internal_fit_strategy_enforces_cut:
 #        for indx in np.arange(len(helper_cip_arg_list))[1:]:
 #            helper_cip_arg_list[indx] += " --lnL-offset 20 "  # enforce lnL cutoff past the first iteration. Focuses fit on high-likelihood points as in O1/O2
 
 
 with open("helper_cip_args.txt",'w') as f:
```

### Comparing `RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/bin/helper_OnlinePSDCleanup.py` & `RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/bin/helper_OnlinePSDCleanup.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/bin/ile_postproc_add_time` & `RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/bin/ile_postproc_add_time`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/bin/integrate_likelihood_extrinsic` & `RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/bin/integrate_likelihood_extrinsic`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/bin/integrate_likelihood_extrinsic_batchmode` & `RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/bin/integrate_likelihood_extrinsic_batchmode`

 * *Files 1% similar despite different names*

```diff
@@ -191,14 +191,15 @@
 optp.add_option("--rom-integrate-intrinsic",default=False,action='store_true',help='Integrate over intrinsic variables. REQUIRES rom_use_basis at present. ONLY integrates in mass ratio as present')
 optp.add_option("--nr-perturbative-extraction",default=False,action='store_true')
 optp.add_option("--nr-perturbative-extraction-full",default=False,action='store_true')
 optp.add_option("--nr-use-provided-strain",default=False,action='store_true')
 optp.add_option("--no-memory",default=False,action='store_true', help="At present, turns off m=0 modes. Use with EXTREME caution only if requested by model developer")
 optp.add_option("--restricted-mode-list-file",default=None,help="A list of ALL modes to use in likelihood. Incredibly dangerous. Only use when comparing with models which provide restricted mode sets, or otherwise to isolate the effect of subsets of modes on the whole")
 optp.add_option("--use-gwsignal",default=False,action='store_true',help='Use gwsignal. In this case the approx name is passed as a string to the lalsimulation.gwsignal interface')
+optp.add_option("--use-gwsignal-lmax-nyquist",default=None,type=int,help='Passes lmax_nyquist integer to the gwsignal waveform interface')
 optp.add_option("--use-external-EOB",default=False,action='store_true')
 optp.add_option("--maximize-only",default=False, action='store_true',help="After integrating, attempts to find the single best fitting point")
 optp.add_option("--dump-lnL-time-series",default=False, action='store_true',help="(requires --sim-xml) Dump lnL(t) at the injected parameters")
 optp.add_option("-a", "--approximant", default="TaylorT4", help="Waveform family to use for templates. Any approximant implemented in LALSimulation is valid.")
 optp.add_option("-A", "--amp-order", type=int, default=0, help="Include amplitude corrections in template waveforms up to this e.g. (e.g. 5 <==> 2.5PN), default is Newtonian order.")
 optp.add_option("--l-max", type=int, default=2, help="Include all (l,m) modes with l less than or equal to this value.")
 optp.add_option("-s", "--data-start-time", type=float, default=None, help="GPS start time of data segment. If given, must also give --data-end-time. If not given, sane start and end time will automatically be chosen.")
@@ -1136,14 +1137,16 @@
     extra_waveform_kwargs = {}
     if opts.internal_waveform_fd_L_frame:
       extra_waveform_kwargs = {'fd_L_frame':True}
     if opts.internal_waveform_fd_no_condition:
       extra_waveform_kwargs['no_condition'] = True
     if opts.rom_group:
       extra_waveform_kwargs['rom_taper_start'] = True  # really for NRHyb3dq8 given discussion with Aasim for high-SNR sources, but valuable generally
+    if opts.use_gwsignal_lmax_nyquist:
+      extra_waveform_kwargs['lmax_nyquist'] = int(opts.use_gwsignal_lmax_nyquist)
     # Precompute
     t_window = 0.15
     rholms_intp, cross_terms, cross_terms_V,  rholms,  guess_snr, rest=factored_likelihood.PrecomputeLikelihoodTerms(
             fiducial_epoch, t_window, P, data_dict, psd_dict, opts.l_max, fmax,
             False, inv_spec_trunc_Q, T_spec,
             NR_group=NR_template_group,NR_param=NR_template_param,
             use_gwsignal=opts.use_gwsignal,
```

### Comparing `RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/bin/integrate_likelihood_extrinsic_no-op` & `RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/bin/integrate_likelihood_extrinsic_no-op`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/bin/make_uni_comov_skymap.py` & `RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/bin/make_uni_comov_skymap.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/bin/plot_posterior_corner.py` & `RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/bin/plot_posterior_corner.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/bin/resample_uniform_comoving.py` & `RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/bin/resample_uniform_comoving.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/bin/util_AMRGrid.py` & `RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/bin/util_AMRGrid.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/bin/util_AdaptiveExponent.py` & `RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/bin/util_AdaptiveExponent.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/bin/util_AnalyticFisherGrid.py` & `RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/bin/util_AnalyticFisherGrid.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/bin/util_BatchConvertResampleILEOutput.py` & `RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/bin/util_BatchConvertResampleILEOutput.py`

 * *Files 6% similar despite different names*

```diff
@@ -70,29 +70,34 @@
 if True: #opts.convention == 'LI':
   print("# m1 m2 a1x a1y a1z a2x a2y a2z mc eta  ra dec time phiorb incl psi  distance Npts lnL p ps neff  mtotal q chi_eff chi_p",end=' ')
   if opts.export_extra_spins:
       print( 'theta_jn phi_jl tilt1 tilt2 costilt1 costilt2 phi12 a1 a2 psiJ',end=' ')
   if opts.export_tides:
       print( "lambda1 lambda2 lam_tilde",end=' ')
   if opts.export_cosmology:
-      print( " m1_source m2_source mc_source mtotal_source redshift ",end=' ')
+      print( " m1_source m2_source mc_source mtotal_source redshift",end=' ')
   if opts.export_weights:
-      print( " weights ", )
+      print( " weights", )
+  if opts.export_eccentricity:
+      print( " eccentricity", )
   print('')
 
 
 for fname in args:
     points = lsctables.SimInspiralTable.get_table(utils.load_filename(fname,contenthandler=ligolw.LIGOLWContentHandler), lsctables.SimInspiralTable.tableName)
 
     # Stage 1: downselect samples (reduces overhead to do this first)
     lnL = np.array([row.alpha1 for row in points])  # hardcoded name
     p = np.array([row.alpha2 for row in points])
     ps = np.array([row.alpha3 for row in points])
     Nmax = np.max([int(row.simulation_id) for row in points])+1    # Nmax. Assumes NOT mixed samples.
 
+    if opts.export_eccentricity:
+        ecc = [row.alpha4 for row in points]
+        
     lnLmax = np.max(lnL)
     weights = np.exp(lnL - lnLmax) * (p/ps)
     # replace weights if nan
     weights=np.nan_to_num(weights,nan=1e-2)
     neff_here = np.sum(weights)/np.max(weights)  # neff for this file.  Assumes NOT mixed samples: dangerous
     p_threshold_size = opts.n_output_samples_per_file
     indx_list = np.random.choice(np.arange(len(weights)), size=p_threshold_size, p=weights/np.sum(weights))
@@ -114,14 +119,16 @@
         P.s1x = pt.spin1x
         P.s1y = pt.spin1y
         P.s1z = pt.spin1z
         P.s2x = pt.spin2x
         P.s2y = pt.spin2y
         P.s2z = pt.spin2z
         P.fmin=opts.fref
+        if opts.export_eccentricity:
+            P.eccentricity = ecc
         try:
             P.fmin = pt.f_lower  # should use this first
         except:
             True
         chieff_here =P.extract_param('xi')
         chip_here = P.extract_param('chi_p')
         mc_here = mc(pt.mass1,pt.mass2)
```

### Comparing `RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/bin/util_CIPdagPostprocess.sh` & `RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/bin/util_CIPdagPostprocess.sh`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/bin/util_CharacterizePosterior.py` & `RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/bin/util_CharacterizePosterior.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/bin/util_CleanILE.py` & `RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/bin/util_CleanILE.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/bin/util_CoincIFOUtility.py` & `RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/bin/util_CoincIFOUtility.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/bin/util_CompareWaveformsInDetectors.py` & `RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/bin/util_CompareWaveformsInDetectors.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/bin/util_ConsolidateDAGsUnderMaster.sh` & `RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/bin/util_ConsolidateDAGsUnderMaster.sh`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/bin/util_ConstructBNSMarginalEOSRank.py` & `RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/bin/util_ConstructBNSMarginalEOSRank.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/bin/util_ConstructEOSPosterior.py` & `RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/bin/util_ConstructEOSPosterior.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/bin/util_ConstructIntrinsicPosterior_GaussianResampling.py` & `RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/bin/util_ConstructIntrinsicPosterior_GaussianResampling.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/bin/util_ConstructIntrinsicPosterior_GenericCoordinates.py` & `RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/bin/util_ConstructIntrinsicPosterior_GenericCoordinates.py`

 * *Files 0% similar despite different names*

```diff
@@ -2885,18 +2885,18 @@
             Pgrid.assign_param(coord_to_assign, line[indx]*fac)
 #            print indx_here, coord_to_assign, line[indx]
         # Test for downselect
         # Perform tabular EOS calculations: compute reference index, lambda1, lambda2
         if my_eos:
             # only define lambda1, lambda2 as parameters if they are used in sampling! Otherwise may cause problems (e.g.,we are assuming it is zero for a BH)
             if not(opts.assume_eos_but_primary_bh):
-                Pgrid.lambda1 = my_eos.lambda_of_m(Pgrid.m1/lal.MSUN_SI)
+                Pgrid.lambda1 = my_eos.lambda_from_m(Pgrid.m1/lal.MSUN_SI)
             else:
                 Pgrid.lambda1 = 0 # BH
-            Pgrid.lambda2 = my_eos.lambda_of_m(Pgrid.m2/lal.MSUN_SI)
+            Pgrid.lambda2 = my_eos.lambda_from_m(Pgrid.m2/lal.MSUN_SI)
         elif opts.tabular_eos_file:
             # save the index of the SORTED SIMULATION (because that's how I'll be accessing it!)
             eos_indx_here = my_eos_sequence.lookup_closest(samples['ordering'][indx_here])
             Pgrid.eos_table_index = eos_indx_here
             # Compute lambda1, lambda2 for output for this EOS, using ASSUMED source redshift (not currently with consistent/flexible distances)
             Pgrid.lambda1 = my_eos_sequence.lambda_of_m_indx(Pgrid.m1/lal.MSUN_SI/(1+source_redshift), eos_indx_here)
             Pgrid.lambda2 = my_eos_sequence.lambda_of_m_indx(Pgrid.m2/lal.MSUN_SI/(1+source_redshift), eos_indx_here)
```

### Comparing `RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/bin/util_CoordinateNamesAngularToCartesianSpins.py` & `RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/bin/util_CoordinateNamesAngularToCartesianSpins.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/bin/util_EOBTideWriteFrame.py` & `RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/bin/util_EOBTideWriteFrame.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/bin/util_FetchExternalGrid.py` & `RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/bin/util_FetchExternalGrid.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/bin/util_FitAndEvaluate_GenericCoordinates.py` & `RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/bin/util_FitAndEvaluate_GenericCoordinates.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/bin/util_ForOSG_MakeTruncatedLocalFramesDir.sh` & `RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/bin/util_ForOSG_MakeTruncatedLocalFramesDir.sh`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/bin/util_FrameZeroNoiseSNR.py` & `RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/bin/util_FrameZeroNoiseSNR.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/bin/util_GenerateMaxlnLWaveform.py` & `RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/bin/util_GenerateMaxlnLWaveform.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/bin/util_GenerateMaxlnLWaveform_NRFromIndex.py` & `RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/bin/util_GenerateMaxlnLWaveform_NRFromIndex.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/bin/util_GridRecenter.py` & `RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/bin/util_GridRecenter.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/bin/util_GridSubsetOfTemplateBank.py` & `RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/bin/util_GridSubsetOfTemplateBank.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/bin/util_HyperCombine.py` & `RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/bin/util_HyperCombine.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/bin/util_HyperparameterGrid.py` & `RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/bin/util_HyperparameterGrid.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/bin/util_HyperparameterPuffball.py` & `RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/bin/util_HyperparameterPuffball.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/bin/util_ILENextGeneration.py` & `RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/bin/util_ILENextGeneration.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/bin/util_ILEROMdagPostprocess.sh` & `RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/bin/util_ILEROMdagPostprocess.sh`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/bin/util_ILEdagPostprocess.sh` & `RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/bin/util_ILEdagPostprocess.sh`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/bin/util_InitMargTable` & `RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/bin/util_InitMargTable`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/bin/util_IntermediateEOSIntegralFromFit.py` & `RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/bin/util_IntermediateEOSIntegralFromFit.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/bin/util_IterativeFisher.py` & `RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/bin/util_IterativeFisher.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/bin/util_JoinXML.py` & `RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/bin/util_JoinXML.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/bin/util_LALCompareApproximantsOnSamples.py` & `RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/bin/util_LALCompareApproximantsOnSamples.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/bin/util_LALWriteFrame.py` & `RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/bin/util_LALWriteFrame.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/bin/util_ManualOverlapGrid.py` & `RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/bin/util_ManualOverlapGrid.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/bin/util_MarginalizedLikelihoodEOSIntegralFromIntermediate.py` & `RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/bin/util_MarginalizedLikelihoodEOSIntegralFromIntermediate.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/bin/util_MassGrid.py` & `RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/bin/util_MassGrid.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/bin/util_MassGridCoalesce.py` & `RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/bin/util_MassGridCoalesce.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/bin/util_NRBestOfIndex.py` & `RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/bin/util_NRBestOfIndex.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/bin/util_NRDumpDetectorResponse.py` & `RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/bin/util_NRDumpDetectorResponse.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/bin/util_NRExtrudeOverlapGrid.py` & `RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/bin/util_NRExtrudeOverlapGrid.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/bin/util_NRIndexedFminCutToILE.py` & `RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/bin/util_NRIndexedFminCutToILE.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/bin/util_NRNearestSimulationTo.py` & `RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/bin/util_NRNearestSimulationTo.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/bin/util_NRRelabelILE.py` & `RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/bin/util_NRRelabelILE.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/bin/util_NRWriteFrame.py` & `RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/bin/util_NRWriteFrame.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/bin/util_NR_GWMemory.py` & `RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/bin/util_NR_GWMemory.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/bin/util_NRdagPostprocess.sh` & `RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/bin/util_NRdagPostprocess.sh`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/bin/util_ParameterFilter.py` & `RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/bin/util_ParameterFilter.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/bin/util_ParameterPuffball.py` & `RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/bin/util_ParameterPuffball.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/bin/util_ParameterRandomize.py` & `RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/bin/util_ParameterRandomize.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/bin/util_PosteriorPostprocess.sh` & `RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/bin/util_PosteriorPostprocess.sh`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/bin/util_PrintInjection.py` & `RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/bin/util_PrintInjection.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/bin/util_RIFT_MultiMetaPipe.py` & `RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/bin/util_RIFT_MultiMetaPipe.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/bin/util_RIFT_pseudo_pipe.py` & `RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/bin/util_RIFT_pseudo_pipe.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/bin/util_RIFT_pseudo_pipe_lowlatency.py` & `RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/bin/util_RIFT_pseudo_pipe_lowlatency.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/bin/util_ROMWriteFrame.py` & `RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/bin/util_ROMWriteFrame.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/bin/util_RandomizeOverlapOrder.py` & `RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/bin/util_RandomizeOverlapOrder.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/bin/util_ResampleILEOutputWithExtrinsic.py` & `RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/bin/util_ResampleILEOutputWithExtrinsic.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/bin/util_SimInspiralToCoinc.py` & `RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/bin/util_SimInspiralToCoinc.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/bin/util_TEOBResumSWriteFrame.py` & `RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/bin/util_TEOBResumSWriteFrame.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/bin/util_TestSpokesIO.py` & `RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/bin/util_TestSpokesIO.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/bin/util_TestXMLParameterStorage.py` & `RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/bin/util_TestXMLParameterStorage.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/bin/util_TidalPlotSimulationStrain.py` & `RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/bin/util_TidalPlotSimulationStrain.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/bin/util_WriteFrameAndCacheFromXML.sh` & `RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/bin/util_WriteFrameAndCacheFromXML.sh`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/bin/util_WriteInjectionFile.py` & `RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/bin/util_WriteInjectionFile.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc3/MonteCarloMarginalizeCode/Code/bin/util_WriteXMLWithEOS.py` & `RIFT-0.0.15.9rc4/MonteCarloMarginalizeCode/Code/bin/util_WriteXMLWithEOS.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc3/PACKAGING.md` & `RIFT-0.0.15.9rc4/PACKAGING.md`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc3/PKG-INFO` & `RIFT-0.0.15.9rc4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RIFT
-Version: 0.0.15.9rc3
+Version: 0.0.15.9rc4
 Summary: RIFT parameter estimation pipeline. Note branch used is temp-RIT-Tides-port_python3_restructure_package (which will become master shortly)!
 Home-page: https://git.ligo.org/rapidpe-rift/rift
 Author: Richard O'Shaughnessy
 Author-email: richard.oshaughnessy@ligo.org
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `RIFT-0.0.15.9rc3/README.md` & `RIFT-0.0.15.9rc4/README.md`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc3/TROUBLESHOOTING.md` & `RIFT-0.0.15.9rc4/TROUBLESHOOTING.md`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc3/howto.md` & `RIFT-0.0.15.9rc4/howto.md`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc3/setup.py` & `RIFT-0.0.15.9rc4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 #  - ourio.py, ourparams.py
 #  - anything with 'test'
 #print " Identified scripts ", my_scripts\
 #print setuptools.find_packages('MonteCarloMarginalizeCode/Code')
 
 setuptools.setup(
     name="RIFT",
-    version="0.0.15.9rc3", # do not build on OSX machine, side effects
+    version="0.0.15.9rc4", # do not build on OSX machine, side effects
     author="Richard O'Shaughnessy",
     author_email="richard.oshaughnessy@ligo.org",
     description="RIFT parameter estimation pipeline. Note branch used is temp-RIT-Tides-port_python3_restructure_package (which will become master shortly)!",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://git.ligo.org/rapidpe-rift/rift",
     package_dir = {'':'MonteCarloMarginalizeCode/Code'},
```

