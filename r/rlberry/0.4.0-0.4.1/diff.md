# Comparing `tmp/rlberry-0.4.0.tar.gz` & `tmp/rlberry-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rlberry-0.4.0.tar", last modified: Wed Jan 18 10:01:12 2023, max compression
+gzip compressed data, was "rlberry-0.4.1.tar", last modified: Mon Jun 19 08:56:17 2023, max compression
```

## Comparing `rlberry-0.4.0.tar` & `rlberry-0.4.1.tar`

### file list

```diff
@@ -1,325 +1,319 @@
-drwxr-xr-x   0 frost     (1000) frost     (1000)        0 2023-01-18 10:01:12.098071 rlberry-0.4.0/
--rw-r--r--   0 frost     (1000) frost     (1000)     1067 2023-01-18 09:58:26.000000 rlberry-0.4.0/LICENSE
--rw-r--r--   0 frost     (1000) frost     (1000)       55 2023-01-18 09:58:26.000000 rlberry-0.4.0/MANIFEST.in
--rw-r--r--   0 frost     (1000) frost     (1000)     6802 2023-01-18 10:01:12.098071 rlberry-0.4.0/PKG-INFO
--rw-r--r--   0 frost     (1000) frost     (1000)     5938 2023-01-18 09:58:26.000000 rlberry-0.4.0/README.md
-drwxr-xr-x   0 frost     (1000) frost     (1000)        0 2023-01-18 10:01:12.071405 rlberry-0.4.0/assets/
--rw-r--r--   0 frost     (1000) frost     (1000)     5722 2023-01-18 09:58:26.000000 rlberry-0.4.0/assets/logo_square.svg
--rw-r--r--   0 frost     (1000) frost     (1000)     5541 2023-01-18 09:58:26.000000 rlberry-0.4.0/assets/logo_wide.svg
-drwxr-xr-x   0 frost     (1000) frost     (1000)        0 2023-01-18 10:01:12.074738 rlberry-0.4.0/rlberry/
--rw-r--r--   0 frost     (1000) frost     (1000)      335 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/__init__.py
--rw-r--r--   0 frost     (1000) frost     (1000)       23 2023-01-18 09:58:44.000000 rlberry-0.4.0/rlberry/_version.py
-drwxr-xr-x   0 frost     (1000) frost     (1000)        0 2023-01-18 10:01:12.074738 rlberry-0.4.0/rlberry/agents/
--rw-r--r--   0 frost     (1000) frost     (1000)      486 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/agents/__init__.py
-drwxr-xr-x   0 frost     (1000) frost     (1000)        0 2023-01-18 10:01:12.074738 rlberry-0.4.0/rlberry/agents/adaptiveql/
--rw-r--r--   0 frost     (1000) frost     (1000)       40 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/agents/adaptiveql/__init__.py
--rw-r--r--   0 frost     (1000) frost     (1000)     5468 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/agents/adaptiveql/adaptiveql.py
--rw-r--r--   0 frost     (1000) frost     (1000)     6237 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/agents/adaptiveql/tree.py
--rw-r--r--   0 frost     (1000) frost     (1000)     1691 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/agents/adaptiveql/utils.py
--rw-r--r--   0 frost     (1000) frost     (1000)    18382 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/agents/agent.py
-drwxr-xr-x   0 frost     (1000) frost     (1000)        0 2023-01-18 10:01:12.074738 rlberry-0.4.0/rlberry/agents/bandits/
--rw-r--r--   0 frost     (1000) frost     (1000)      479 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/agents/bandits/__init__.py
--rw-r--r--   0 frost     (1000) frost     (1000)     3361 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/agents/bandits/bandit_base.py
--rw-r--r--   0 frost     (1000) frost     (1000)     3300 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/agents/bandits/index_agents.py
--rw-r--r--   0 frost     (1000) frost     (1000)    12014 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/agents/bandits/indices.py
--rw-r--r--   0 frost     (1000) frost     (1000)     4472 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/agents/bandits/priors.py
--rw-r--r--   0 frost     (1000) frost     (1000)     4068 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/agents/bandits/randomized_agents.py
-drwxr-xr-x   0 frost     (1000) frost     (1000)        0 2023-01-18 10:01:12.074738 rlberry-0.4.0/rlberry/agents/bandits/tools/
--rw-r--r--   0 frost     (1000) frost     (1000)       35 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/agents/bandits/tools/__init__.py
--rw-r--r--   0 frost     (1000) frost     (1000)     8519 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/agents/bandits/tools/tracker.py
--rw-r--r--   0 frost     (1000) frost     (1000)     5110 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/agents/bandits/ts_agents.py
-drwxr-xr-x   0 frost     (1000) frost     (1000)        0 2023-01-18 10:01:12.074738 rlberry-0.4.0/rlberry/agents/dynprog/
--rw-r--r--   0 frost     (1000) frost     (1000)       49 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/agents/dynprog/__init__.py
--rw-r--r--   0 frost     (1000) frost     (1000)     8882 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/agents/dynprog/utils.py
--rw-r--r--   0 frost     (1000) frost     (1000)     2540 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/agents/dynprog/value_iteration.py
-drwxr-xr-x   0 frost     (1000) frost     (1000)        0 2023-01-18 10:01:12.074738 rlberry-0.4.0/rlberry/agents/experimental/
--rw-r--r--   0 frost     (1000) frost     (1000)        0 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/agents/experimental/__init__.py
-drwxr-xr-x   0 frost     (1000) frost     (1000)        0 2023-01-18 10:01:12.074738 rlberry-0.4.0/rlberry/agents/experimental/jax/
--rw-r--r--   0 frost     (1000) frost     (1000)       32 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/agents/experimental/jax/__init__.py
-drwxr-xr-x   0 frost     (1000) frost     (1000)        0 2023-01-18 10:01:12.078071 rlberry-0.4.0/rlberry/agents/experimental/jax/dqn/
--rw-r--r--   0 frost     (1000) frost     (1000)        0 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/agents/experimental/jax/dqn/__init__.py
--rw-r--r--   0 frost     (1000) frost     (1000)    16100 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/agents/experimental/jax/dqn/dqn.py
-drwxr-xr-x   0 frost     (1000) frost     (1000)        0 2023-01-18 10:01:12.078071 rlberry-0.4.0/rlberry/agents/experimental/jax/nets/
--rw-r--r--   0 frost     (1000) frost     (1000)        0 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/agents/experimental/jax/nets/__init__.py
--rw-r--r--   0 frost     (1000) frost     (1000)      728 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/agents/experimental/jax/nets/common.py
-drwxr-xr-x   0 frost     (1000) frost     (1000)        0 2023-01-18 10:01:12.078071 rlberry-0.4.0/rlberry/agents/experimental/jax/tests/
--rw-r--r--   0 frost     (1000) frost     (1000)        0 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/agents/experimental/jax/tests/__init__.py
--rw-r--r--   0 frost     (1000) frost     (1000)      906 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/agents/experimental/jax/tests/old_test_tqn.py
-drwxr-xr-x   0 frost     (1000) frost     (1000)        0 2023-01-18 10:01:12.078071 rlberry-0.4.0/rlberry/agents/experimental/jax/utils/
--rw-r--r--   0 frost     (1000) frost     (1000)        0 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/agents/experimental/jax/utils/__init__.py
--rw-r--r--   0 frost     (1000) frost     (1000)     5062 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/agents/experimental/jax/utils/replay_buffer.py
-drwxr-xr-x   0 frost     (1000) frost     (1000)        0 2023-01-18 10:01:12.078071 rlberry-0.4.0/rlberry/agents/experimental/tests/
--rw-r--r--   0 frost     (1000) frost     (1000)        0 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/agents/experimental/tests/__init__.py
--rw-r--r--   0 frost     (1000) frost     (1000)     1484 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/agents/experimental/tests/test_actor_critic.py
--rw-r--r--   0 frost     (1000) frost     (1000)     1324 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/agents/experimental/tests/test_sac.py
-drwxr-xr-x   0 frost     (1000) frost     (1000)        0 2023-01-18 10:01:12.078071 rlberry-0.4.0/rlberry/agents/experimental/torch/
--rw-r--r--   0 frost     (1000) frost     (1000)      101 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/agents/experimental/torch/__init__.py
-drwxr-xr-x   0 frost     (1000) frost     (1000)        0 2023-01-18 10:01:12.078071 rlberry-0.4.0/rlberry/agents/experimental/torch/avec/
--rw-r--r--   0 frost     (1000) frost     (1000)       35 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/agents/experimental/torch/avec/__init__.py
--rw-r--r--   0 frost     (1000) frost     (1000)    12259 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/agents/experimental/torch/avec/avec_ppo.py
-drwxr-xr-x   0 frost     (1000) frost     (1000)        0 2023-01-18 10:01:12.078071 rlberry-0.4.0/rlberry/agents/experimental/torch/sac/
--rw-r--r--   0 frost     (1000) frost     (1000)       26 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/agents/experimental/torch/sac/__init__.py
--rw-r--r--   0 frost     (1000) frost     (1000)    13122 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/agents/experimental/torch/sac/sac.py
--rw-r--r--   0 frost     (1000) frost     (1000)     2279 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/agents/experimental/torch/sac/utils.py
-drwxr-xr-x   0 frost     (1000) frost     (1000)        0 2023-01-18 10:01:12.078071 rlberry-0.4.0/rlberry/agents/features/
--rw-r--r--   0 frost     (1000) frost     (1000)       36 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/agents/features/__init__.py
--rw-r--r--   0 frost     (1000) frost     (1000)      580 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/agents/features/feature_map.py
-drwxr-xr-x   0 frost     (1000) frost     (1000)        0 2023-01-18 10:01:12.078071 rlberry-0.4.0/rlberry/agents/kernel_based/
--rw-r--r--   0 frost     (1000) frost     (1000)       83 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/agents/kernel_based/__init__.py
--rw-r--r--   0 frost     (1000) frost     (1000)      908 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/agents/kernel_based/common.py
--rw-r--r--   0 frost     (1000) frost     (1000)     1929 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/agents/kernel_based/kernels.py
--rw-r--r--   0 frost     (1000) frost     (1000)    12466 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/agents/kernel_based/rs_kernel_ucbvi.py
--rw-r--r--   0 frost     (1000) frost     (1000)    11254 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/agents/kernel_based/rs_ucbvi.py
-drwxr-xr-x   0 frost     (1000) frost     (1000)        0 2023-01-18 10:01:12.078071 rlberry-0.4.0/rlberry/agents/linear/
--rw-r--r--   0 frost     (1000) frost     (1000)       35 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/agents/linear/__init__.py
--rw-r--r--   0 frost     (1000) frost     (1000)    11184 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/agents/linear/lsvi_ucb.py
-drwxr-xr-x   0 frost     (1000) frost     (1000)        0 2023-01-18 10:01:12.078071 rlberry-0.4.0/rlberry/agents/mbqvi/
--rw-r--r--   0 frost     (1000) frost     (1000)       30 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/agents/mbqvi/__init__.py
--rw-r--r--   0 frost     (1000) frost     (1000)     4943 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/agents/mbqvi/mbqvi.py
-drwxr-xr-x   0 frost     (1000) frost     (1000)        0 2023-01-18 10:01:12.078071 rlberry-0.4.0/rlberry/agents/optql/
--rw-r--r--   0 frost     (1000) frost     (1000)       30 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/agents/optql/__init__.py
--rw-r--r--   0 frost     (1000) frost     (1000)     6595 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/agents/optql/optql.py
-drwxr-xr-x   0 frost     (1000) frost     (1000)        0 2023-01-18 10:01:12.078071 rlberry-0.4.0/rlberry/agents/psrl/
--rw-r--r--   0 frost     (1000) frost     (1000)       28 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/agents/psrl/__init__.py
--rw-r--r--   0 frost     (1000) frost     (1000)     8344 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/agents/psrl/psrl.py
-drwxr-xr-x   0 frost     (1000) frost     (1000)        0 2023-01-18 10:01:12.078071 rlberry-0.4.0/rlberry/agents/rlsvi/
--rw-r--r--   0 frost     (1000) frost     (1000)       30 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/agents/rlsvi/__init__.py
--rw-r--r--   0 frost     (1000) frost     (1000)     8502 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/agents/rlsvi/rlsvi.py
-drwxr-xr-x   0 frost     (1000) frost     (1000)        0 2023-01-18 10:01:12.081405 rlberry-0.4.0/rlberry/agents/stable_baselines/
--rw-r--r--   0 frost     (1000) frost     (1000)       51 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/agents/stable_baselines/__init__.py
--rw-r--r--   0 frost     (1000) frost     (1000)     8702 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/agents/stable_baselines/stable_baselines.py
-drwxr-xr-x   0 frost     (1000) frost     (1000)        0 2023-01-18 10:01:12.081405 rlberry-0.4.0/rlberry/agents/tests/
--rw-r--r--   0 frost     (1000) frost     (1000)        0 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/agents/tests/__init__.py
--rw-r--r--   0 frost     (1000) frost     (1000)      377 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/agents/tests/test_adaptiveql.py
--rw-r--r--   0 frost     (1000) frost     (1000)     3277 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/agents/tests/test_bandits.py
--rw-r--r--   0 frost     (1000) frost     (1000)     4902 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/agents/tests/test_dynprog.py
--rw-r--r--   0 frost     (1000) frost     (1000)     1558 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/agents/tests/test_kernel_based.py
--rw-r--r--   0 frost     (1000) frost     (1000)     6078 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/agents/tests/test_lsvi_ucb.py
--rw-r--r--   0 frost     (1000) frost     (1000)      808 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/agents/tests/test_mbqvi.py
--rw-r--r--   0 frost     (1000) frost     (1000)      304 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/agents/tests/test_optql.py
--rw-r--r--   0 frost     (1000) frost     (1000)      772 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/agents/tests/test_psrl.py
--rw-r--r--   0 frost     (1000) frost     (1000)     5707 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/agents/tests/test_replay.py
--rw-r--r--   0 frost     (1000) frost     (1000)      507 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/agents/tests/test_rlsvi.py
--rw-r--r--   0 frost     (1000) frost     (1000)     1058 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/agents/tests/test_stable_baselines.py
--rw-r--r--   0 frost     (1000) frost     (1000)      779 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/agents/tests/test_ucbvi.py
-drwxr-xr-x   0 frost     (1000) frost     (1000)        0 2023-01-18 10:01:12.081405 rlberry-0.4.0/rlberry/agents/torch/
--rw-r--r--   0 frost     (1000) frost     (1000)      191 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/agents/torch/__init__.py
-drwxr-xr-x   0 frost     (1000) frost     (1000)        0 2023-01-18 10:01:12.081405 rlberry-0.4.0/rlberry/agents/torch/a2c/
--rw-r--r--   0 frost     (1000) frost     (1000)       26 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/agents/torch/a2c/__init__.py
--rw-r--r--   0 frost     (1000) frost     (1000)    11433 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/agents/torch/a2c/a2c.py
-drwxr-xr-x   0 frost     (1000) frost     (1000)        0 2023-01-18 10:01:12.081405 rlberry-0.4.0/rlberry/agents/torch/dqn/
--rw-r--r--   0 frost     (1000) frost     (1000)       63 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/agents/torch/dqn/__init__.py
--rw-r--r--   0 frost     (1000) frost     (1000)    16491 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/agents/torch/dqn/dqn.py
--rw-r--r--   0 frost     (1000) frost     (1000)     4226 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/agents/torch/dqn/dqn_utils.py
--rw-r--r--   0 frost     (1000) frost     (1000)    17760 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/agents/torch/dqn/mdqn.py
-drwxr-xr-x   0 frost     (1000) frost     (1000)        0 2023-01-18 10:01:12.081405 rlberry-0.4.0/rlberry/agents/torch/ppo/
--rw-r--r--   0 frost     (1000) frost     (1000)       26 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/agents/torch/ppo/__init__.py
--rw-r--r--   0 frost     (1000) frost     (1000)    16349 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/agents/torch/ppo/ppo.py
-drwxr-xr-x   0 frost     (1000) frost     (1000)        0 2023-01-18 10:01:12.081405 rlberry-0.4.0/rlberry/agents/torch/reinforce/
--rw-r--r--   0 frost     (1000) frost     (1000)       38 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/agents/torch/reinforce/__init__.py
--rw-r--r--   0 frost     (1000) frost     (1000)     7169 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/agents/torch/reinforce/reinforce.py
-drwxr-xr-x   0 frost     (1000) frost     (1000)        0 2023-01-18 10:01:12.084738 rlberry-0.4.0/rlberry/agents/torch/tests/
--rw-r--r--   0 frost     (1000) frost     (1000)        0 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/agents/torch/tests/__init__.py
--rw-r--r--   0 frost     (1000) frost     (1000)     3389 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/agents/torch/tests/test_a2c.py
--rw-r--r--   0 frost     (1000) frost     (1000)     1140 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/agents/torch/tests/test_dqn.py
--rw-r--r--   0 frost     (1000) frost     (1000)      812 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/agents/torch/tests/test_factory.py
--rw-r--r--   0 frost     (1000) frost     (1000)     1134 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/agents/torch/tests/test_mdqn.py
--rw-r--r--   0 frost     (1000) frost     (1000)     5602 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/agents/torch/tests/test_ppo.py
--rw-r--r--   0 frost     (1000) frost     (1000)     1434 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/agents/torch/tests/test_reinforce.py
--rw-r--r--   0 frost     (1000) frost     (1000)     1496 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/agents/torch/tests/test_torch_models.py
--rw-r--r--   0 frost     (1000) frost     (1000)     1080 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/agents/torch/tests/test_torch_training.py
-drwxr-xr-x   0 frost     (1000) frost     (1000)        0 2023-01-18 10:01:12.084738 rlberry-0.4.0/rlberry/agents/torch/utils/
--rw-r--r--   0 frost     (1000) frost     (1000)        0 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/agents/torch/utils/__init__.py
--rw-r--r--   0 frost     (1000) frost     (1000)     7399 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/agents/torch/utils/attention_models.py
--rw-r--r--   0 frost     (1000) frost     (1000)    14007 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/agents/torch/utils/models.py
--rw-r--r--   0 frost     (1000) frost     (1000)     4762 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/agents/torch/utils/training.py
-drwxr-xr-x   0 frost     (1000) frost     (1000)        0 2023-01-18 10:01:12.084738 rlberry-0.4.0/rlberry/agents/ucbvi/
--rw-r--r--   0 frost     (1000) frost     (1000)       30 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/agents/ucbvi/__init__.py
--rw-r--r--   0 frost     (1000) frost     (1000)    10335 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/agents/ucbvi/ucbvi.py
--rw-r--r--   0 frost     (1000) frost     (1000)     1952 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/agents/ucbvi/utils.py
-drwxr-xr-x   0 frost     (1000) frost     (1000)        0 2023-01-18 10:01:12.084738 rlberry-0.4.0/rlberry/agents/utils/
--rw-r--r--   0 frost     (1000) frost     (1000)        0 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/agents/utils/__init__.py
--rw-r--r--   0 frost     (1000) frost     (1000)    11914 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/agents/utils/memories.py
--rw-r--r--   0 frost     (1000) frost     (1000)    14236 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/agents/utils/replay.py
--rw-r--r--   0 frost     (1000) frost     (1000)     5290 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/agents/utils/replay_utils.py
--rw-r--r--   0 frost     (1000) frost     (1000)      357 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/check_packages.py
-drwxr-xr-x   0 frost     (1000) frost     (1000)        0 2023-01-18 10:01:12.084738 rlberry-0.4.0/rlberry/colab_utils/
--rw-r--r--   0 frost     (1000) frost     (1000)        0 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/colab_utils/__init__.py
--rw-r--r--   0 frost     (1000) frost     (1000)     1053 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/colab_utils/display_setup.py
-drwxr-xr-x   0 frost     (1000) frost     (1000)        0 2023-01-18 10:01:12.084738 rlberry-0.4.0/rlberry/envs/
--rw-r--r--   0 frost     (1000) frost     (1000)      263 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/envs/__init__.py
-drwxr-xr-x   0 frost     (1000) frost     (1000)        0 2023-01-18 10:01:12.084738 rlberry-0.4.0/rlberry/envs/bandits/
--rw-r--r--   0 frost     (1000) frost     (1000)      181 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/envs/bandits/__init__.py
--rw-r--r--   0 frost     (1000) frost     (1000)     2240 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/envs/bandits/bandit_base.py
--rw-r--r--   0 frost     (1000) frost     (1000)     2533 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/envs/bandits/corrupted_bandits.py
--rw-r--r--   0 frost     (1000) frost     (1000)     1370 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/envs/bandits/stochastic_bandits.py
--rw-r--r--   0 frost     (1000) frost     (1000)     3817 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/envs/basewrapper.py
-drwxr-xr-x   0 frost     (1000) frost     (1000)        0 2023-01-18 10:01:12.084738 rlberry-0.4.0/rlberry/envs/benchmarks/
--rw-r--r--   0 frost     (1000) frost     (1000)        0 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/envs/benchmarks/__init__.py
-drwxr-xr-x   0 frost     (1000) frost     (1000)        0 2023-01-18 10:01:12.084738 rlberry-0.4.0/rlberry/envs/benchmarks/ball_exploration/
--rw-r--r--   0 frost     (1000) frost     (1000)       49 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/envs/benchmarks/ball_exploration/__init__.py
--rw-r--r--   0 frost     (1000) frost     (1000)     4995 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/envs/benchmarks/ball_exploration/ball2d.py
--rw-r--r--   0 frost     (1000) frost     (1000)    14237 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/envs/benchmarks/ball_exploration/pball.py
-drwxr-xr-x   0 frost     (1000) frost     (1000)        0 2023-01-18 10:01:12.084738 rlberry-0.4.0/rlberry/envs/benchmarks/generalization/
--rw-r--r--   0 frost     (1000) frost     (1000)        0 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/envs/benchmarks/generalization/__init__.py
--rw-r--r--   0 frost     (1000) frost     (1000)     5442 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/envs/benchmarks/generalization/twinrooms.py
-drwxr-xr-x   0 frost     (1000) frost     (1000)        0 2023-01-18 10:01:12.088071 rlberry-0.4.0/rlberry/envs/benchmarks/grid_exploration/
--rw-r--r--   0 frost     (1000) frost     (1000)        0 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/envs/benchmarks/grid_exploration/__init__.py
--rw-r--r--   0 frost     (1000) frost     (1000)     5296 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/envs/benchmarks/grid_exploration/apple_gold.py
--rw-r--r--   0 frost     (1000) frost     (1000)     3816 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/envs/benchmarks/grid_exploration/four_room.py
--rw-r--r--   0 frost     (1000) frost     (1000)    10495 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/envs/benchmarks/grid_exploration/nroom.py
--rw-r--r--   0 frost     (1000) frost     (1000)     4231 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/envs/benchmarks/grid_exploration/six_room.py
-drwxr-xr-x   0 frost     (1000) frost     (1000)        0 2023-01-18 10:01:12.088071 rlberry-0.4.0/rlberry/envs/classic_control/
--rw-r--r--   0 frost     (1000) frost     (1000)    18518 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/envs/classic_control/SpringCartPole.py
--rw-r--r--   0 frost     (1000) frost     (1000)      141 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/envs/classic_control/__init__.py
--rw-r--r--   0 frost     (1000) frost     (1000)    11984 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/envs/classic_control/acrobot.py
--rw-r--r--   0 frost     (1000) frost     (1000)     5938 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/envs/classic_control/mountain_car.py
--rw-r--r--   0 frost     (1000) frost     (1000)     3635 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/envs/classic_control/pendulum.py
-drwxr-xr-x   0 frost     (1000) frost     (1000)        0 2023-01-18 10:01:12.088071 rlberry-0.4.0/rlberry/envs/finite/
--rw-r--r--   0 frost     (1000) frost     (1000)       92 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/envs/finite/__init__.py
--rw-r--r--   0 frost     (1000) frost     (1000)     3956 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/envs/finite/chain.py
--rw-r--r--   0 frost     (1000) frost     (1000)     5594 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/envs/finite/finite_mdp.py
--rw-r--r--   0 frost     (1000) frost     (1000)    16182 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/envs/finite/gridworld.py
--rw-r--r--   0 frost     (1000) frost     (1000)     2011 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/envs/finite/gridworld_utils.py
--rw-r--r--   0 frost     (1000) frost     (1000)     1340 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/envs/gym_make.py
-drwxr-xr-x   0 frost     (1000) frost     (1000)        0 2023-01-18 10:01:12.088071 rlberry-0.4.0/rlberry/envs/interface/
--rw-r--r--   0 frost     (1000) frost     (1000)       25 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/envs/interface/__init__.py
--rw-r--r--   0 frost     (1000) frost     (1000)     4813 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/envs/interface/model.py
--rw-r--r--   0 frost     (1000) frost     (1000)     1227 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/envs/pipeline.py
-drwxr-xr-x   0 frost     (1000) frost     (1000)        0 2023-01-18 10:01:12.088071 rlberry-0.4.0/rlberry/envs/tests/
--rw-r--r--   0 frost     (1000) frost     (1000)        0 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/envs/tests/__init__.py
--rw-r--r--   0 frost     (1000) frost     (1000)     1268 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/envs/tests/test_bandits.py
--rw-r--r--   0 frost     (1000) frost     (1000)     2589 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/envs/tests/test_env_seeding.py
--rw-r--r--   0 frost     (1000) frost     (1000)     2225 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/envs/tests/test_gym_env_seeding.py
--rw-r--r--   0 frost     (1000) frost     (1000)     7440 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/envs/tests/test_instantiation.py
--rw-r--r--   0 frost     (1000) frost     (1000)     2635 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/envs/tests/test_spring_env.py
--rw-r--r--   0 frost     (1000) frost     (1000)      845 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/envs/utils.py
-drwxr-xr-x   0 frost     (1000) frost     (1000)        0 2023-01-18 10:01:12.088071 rlberry-0.4.0/rlberry/experiment/
--rw-r--r--   0 frost     (1000) frost     (1000)      142 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/experiment/__init__.py
--rw-r--r--   0 frost     (1000) frost     (1000)     1817 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/experiment/generator.py
--rw-r--r--   0 frost     (1000) frost     (1000)     3705 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/experiment/load_results.py
--rw-r--r--   0 frost     (1000) frost     (1000)     6285 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/experiment/yaml_utils.py
-drwxr-xr-x   0 frost     (1000) frost     (1000)        0 2023-01-18 10:01:12.091405 rlberry-0.4.0/rlberry/exploration_tools/
--rw-r--r--   0 frost     (1000) frost     (1000)        0 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/exploration_tools/__init__.py
--rw-r--r--   0 frost     (1000) frost     (1000)     3507 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/exploration_tools/discrete_counter.py
--rw-r--r--   0 frost     (1000) frost     (1000)     6179 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/exploration_tools/online_discretization_counter.py
-drwxr-xr-x   0 frost     (1000) frost     (1000)        0 2023-01-18 10:01:12.091405 rlberry-0.4.0/rlberry/exploration_tools/tests/
--rw-r--r--   0 frost     (1000) frost     (1000)        0 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/exploration_tools/tests/__init__.py
--rw-r--r--   0 frost     (1000) frost     (1000)     4326 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/exploration_tools/tests/test_discrete_counter.py
-drwxr-xr-x   0 frost     (1000) frost     (1000)        0 2023-01-18 10:01:12.091405 rlberry-0.4.0/rlberry/exploration_tools/torch/
--rw-r--r--   0 frost     (1000) frost     (1000)        0 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/exploration_tools/torch/__init__.py
--rw-r--r--   0 frost     (1000) frost     (1000)     7357 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/exploration_tools/torch/rnd.py
-drwxr-xr-x   0 frost     (1000) frost     (1000)        0 2023-01-18 10:01:12.091405 rlberry-0.4.0/rlberry/exploration_tools/torch/tests/
--rw-r--r--   0 frost     (1000) frost     (1000)        0 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/exploration_tools/torch/tests/__init__.py
--rw-r--r--   0 frost     (1000) frost     (1000)      711 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/exploration_tools/torch/tests/test_rnd.py
--rw-r--r--   0 frost     (1000) frost     (1000)     2341 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/exploration_tools/typing.py
--rw-r--r--   0 frost     (1000) frost     (1000)     1012 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/exploration_tools/uncertainty_estimator.py
-drwxr-xr-x   0 frost     (1000) frost     (1000)        0 2023-01-18 10:01:12.091405 rlberry-0.4.0/rlberry/manager/
--rw-r--r--   0 frost     (1000) frost     (1000)      164 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/manager/__init__.py
--rw-r--r--   0 frost     (1000) frost     (1000)    46496 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/manager/agent_manager.py
--rw-r--r--   0 frost     (1000) frost     (1000)    19902 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/manager/evaluation.py
--rw-r--r--   0 frost     (1000) frost     (1000)     2967 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/manager/multiple_managers.py
--rw-r--r--   0 frost     (1000) frost     (1000)     7863 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/manager/remote_agent_manager.py
-drwxr-xr-x   0 frost     (1000) frost     (1000)        0 2023-01-18 10:01:12.091405 rlberry-0.4.0/rlberry/manager/tests/
--rw-r--r--   0 frost     (1000) frost     (1000)        0 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/manager/tests/__init__.py
--rw-r--r--   0 frost     (1000) frost     (1000)     9443 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/manager/tests/test_agent_manager.py
--rw-r--r--   0 frost     (1000) frost     (1000)     2648 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/manager/tests/test_agent_manager_seeding.py
--rw-r--r--   0 frost     (1000) frost     (1000)     5052 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/manager/tests/test_hyperparam_optim.py
--rw-r--r--   0 frost     (1000) frost     (1000)     4460 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/manager/tests/test_plot.py
--rw-r--r--   0 frost     (1000) frost     (1000)     1249 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/manager/tests/test_shared_data.py
--rw-r--r--   0 frost     (1000) frost     (1000)      391 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/manager/utils.py
--rw-r--r--   0 frost     (1000) frost     (1000)     1947 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/metadata_utils.py
-drwxr-xr-x   0 frost     (1000) frost     (1000)        0 2023-01-18 10:01:12.091405 rlberry-0.4.0/rlberry/network/
--rw-r--r--   0 frost     (1000) frost     (1000)        0 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/network/__init__.py
--rw-r--r--   0 frost     (1000) frost     (1000)     1522 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/network/client.py
--rw-r--r--   0 frost     (1000) frost     (1000)     2836 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/network/interface.py
--rw-r--r--   0 frost     (1000) frost     (1000)     6408 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/network/server.py
--rw-r--r--   0 frost     (1000) frost     (1000)     5062 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/network/server_utils.py
--rw-r--r--   0 frost     (1000) frost     (1000)     2631 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/network/utils.py
-drwxr-xr-x   0 frost     (1000) frost     (1000)        0 2023-01-18 10:01:12.091405 rlberry-0.4.0/rlberry/rendering/
--rw-r--r--   0 frost     (1000) frost     (1000)      138 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/rendering/__init__.py
--rw-r--r--   0 frost     (1000) frost     (1000)     1001 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/rendering/common_shapes.py
--rw-r--r--   0 frost     (1000) frost     (1000)     1265 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/rendering/core.py
--rw-r--r--   0 frost     (1000) frost     (1000)     7710 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/rendering/opengl_render2d.py
--rw-r--r--   0 frost     (1000) frost     (1000)     5933 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/rendering/pygame_render2d.py
--rw-r--r--   0 frost     (1000) frost     (1000)     4428 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/rendering/render_interface.py
-drwxr-xr-x   0 frost     (1000) frost     (1000)        0 2023-01-18 10:01:12.094738 rlberry-0.4.0/rlberry/rendering/tests/
--rw-r--r--   0 frost     (1000) frost     (1000)        0 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/rendering/tests/__init__.py
--rw-r--r--   0 frost     (1000) frost     (1000)     2874 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/rendering/tests/test_rendering_interface.py
--rw-r--r--   0 frost     (1000) frost     (1000)     1864 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/rendering/utils.py
-drwxr-xr-x   0 frost     (1000) frost     (1000)        0 2023-01-18 10:01:12.094738 rlberry-0.4.0/rlberry/seeding/
--rw-r--r--   0 frost     (1000) frost     (1000)       99 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/seeding/__init__.py
--rw-r--r--   0 frost     (1000) frost     (1000)     3973 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/seeding/seeder.py
--rw-r--r--   0 frost     (1000) frost     (1000)     2105 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/seeding/seeding.py
-drwxr-xr-x   0 frost     (1000) frost     (1000)        0 2023-01-18 10:01:12.094738 rlberry-0.4.0/rlberry/seeding/tests/
--rw-r--r--   0 frost     (1000) frost     (1000)        0 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/seeding/tests/__init__.py
--rw-r--r--   0 frost     (1000) frost     (1000)     1728 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/seeding/tests/test_seeding.py
--rw-r--r--   0 frost     (1000) frost     (1000)      874 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/seeding/tests/test_threads.py
--rw-r--r--   0 frost     (1000) frost     (1000)     1072 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/seeding/tests/test_threads_torch.py
-drwxr-xr-x   0 frost     (1000) frost     (1000)        0 2023-01-18 10:01:12.094738 rlberry-0.4.0/rlberry/spaces/
--rw-r--r--   0 frost     (1000) frost     (1000)      180 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/spaces/__init__.py
--rw-r--r--   0 frost     (1000) frost     (1000)     3003 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/spaces/box.py
--rw-r--r--   0 frost     (1000) frost     (1000)      807 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/spaces/dict.py
--rw-r--r--   0 frost     (1000) frost     (1000)     1553 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/spaces/discrete.py
--rw-r--r--   0 frost     (1000) frost     (1000)     1429 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/spaces/from_gym.py
--rw-r--r--   0 frost     (1000) frost     (1000)     1261 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/spaces/multi_binary.py
--rw-r--r--   0 frost     (1000) frost     (1000)     1347 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/spaces/multi_discrete.py
-drwxr-xr-x   0 frost     (1000) frost     (1000)        0 2023-01-18 10:01:12.094738 rlberry-0.4.0/rlberry/spaces/tests/
--rw-r--r--   0 frost     (1000) frost     (1000)        0 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/spaces/tests/__init__.py
--rw-r--r--   0 frost     (1000) frost     (1000)     4724 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/spaces/tests/test_from_gym.py
--rw-r--r--   0 frost     (1000) frost     (1000)     3611 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/spaces/tests/test_spaces.py
--rw-r--r--   0 frost     (1000) frost     (1000)      763 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/spaces/tuple.py
-drwxr-xr-x   0 frost     (1000) frost     (1000)        0 2023-01-18 10:01:12.094738 rlberry-0.4.0/rlberry/tests/
--rw-r--r--   0 frost     (1000) frost     (1000)        0 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/tests/__init__.py
--rw-r--r--   0 frost     (1000) frost     (1000)     1734 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/tests/test_agent.py
--rw-r--r--   0 frost     (1000) frost     (1000)      724 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/tests/test_envs.py
--rw-r--r--   0 frost     (1000) frost     (1000)      283 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/types.py
-drwxr-xr-x   0 frost     (1000) frost     (1000)        0 2023-01-18 10:01:12.098071 rlberry-0.4.0/rlberry/utils/
--rw-r--r--   0 frost     (1000) frost     (1000)      228 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/utils/__init__.py
--rw-r--r--   0 frost     (1000) frost     (1000)     1177 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/utils/binsearch.py
--rw-r--r--   0 frost     (1000) frost     (1000)    10078 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/utils/check_agent.py
--rw-r--r--   0 frost     (1000) frost     (1000)     1771 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/utils/check_bandit_agent.py
--rw-r--r--   0 frost     (1000) frost     (1000)     1478 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/utils/check_env.py
--rw-r--r--   0 frost     (1000) frost     (1000)    10915 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/utils/check_gym_env.py
--rw-r--r--   0 frost     (1000) frost     (1000)      199 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/utils/factory.py
--rw-r--r--   0 frost     (1000) frost     (1000)      847 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/utils/io.py
--rw-r--r--   0 frost     (1000) frost     (1000)      395 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/utils/jit_setup.py
--rw-r--r--   0 frost     (1000) frost     (1000)     3453 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/utils/logging.py
--rw-r--r--   0 frost     (1000) frost     (1000)      326 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/utils/math.py
--rw-r--r--   0 frost     (1000) frost     (1000)      699 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/utils/metrics.py
--rw-r--r--   0 frost     (1000) frost     (1000)     2200 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/utils/space_discretizer.py
-drwxr-xr-x   0 frost     (1000) frost     (1000)        0 2023-01-18 10:01:12.098071 rlberry-0.4.0/rlberry/utils/tests/
--rw-r--r--   0 frost     (1000) frost     (1000)        0 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/utils/tests/__init__.py
--rw-r--r--   0 frost     (1000) frost     (1000)     1061 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/utils/tests/test_binsearch.py
--rw-r--r--   0 frost     (1000) frost     (1000)     2976 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/utils/tests/test_check.py
--rw-r--r--   0 frost     (1000) frost     (1000)      483 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/utils/tests/test_metrics.py
--rw-r--r--   0 frost     (1000) frost     (1000)     1410 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/utils/tests/test_writer.py
--rw-r--r--   0 frost     (1000) frost     (1000)     2517 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/utils/torch.py
--rw-r--r--   0 frost     (1000) frost     (1000)    13542 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/utils/writers.py
-drwxr-xr-x   0 frost     (1000) frost     (1000)        0 2023-01-18 10:01:12.098071 rlberry-0.4.0/rlberry/wrappers/
--rw-r--r--   0 frost     (1000) frost     (1000)      195 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/wrappers/__init__.py
--rw-r--r--   0 frost     (1000) frost     (1000)      890 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/wrappers/autoreset.py
--rw-r--r--   0 frost     (1000) frost     (1000)      962 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/wrappers/discrete2onehot.py
--rw-r--r--   0 frost     (1000) frost     (1000)     3273 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/wrappers/discretize_state.py
--rw-r--r--   0 frost     (1000) frost     (1000)     1217 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/wrappers/gym_utils.py
--rw-r--r--   0 frost     (1000) frost     (1000)     2064 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/wrappers/rescale_reward.py
--rw-r--r--   0 frost     (1000) frost     (1000)      505 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/wrappers/scalarize.py
-drwxr-xr-x   0 frost     (1000) frost     (1000)        0 2023-01-18 10:01:12.098071 rlberry-0.4.0/rlberry/wrappers/tests/
--rw-r--r--   0 frost     (1000) frost     (1000)        0 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/wrappers/tests/__init__.py
--rw-r--r--   0 frost     (1000) frost     (1000)      776 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/wrappers/tests/test_basewrapper.py
--rw-r--r--   0 frost     (1000) frost     (1000)     5701 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/wrappers/tests/test_common_wrappers.py
--rw-r--r--   0 frost     (1000) frost     (1000)     2988 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/wrappers/tests/test_gym_space_conversion.py
--rw-r--r--   0 frost     (1000) frost     (1000)     3981 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/wrappers/tests/test_wrapper_seeding.py
--rw-r--r--   0 frost     (1000) frost     (1000)     1114 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/wrappers/tests/test_writer_utils.py
--rw-r--r--   0 frost     (1000) frost     (1000)     3482 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/wrappers/uncertainty_estimator_wrapper.py
--rw-r--r--   0 frost     (1000) frost     (1000)    14355 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/wrappers/vis2d.py
--rw-r--r--   0 frost     (1000) frost     (1000)     1425 2023-01-18 09:58:26.000000 rlberry-0.4.0/rlberry/wrappers/writer_utils.py
-drwxr-xr-x   0 frost     (1000) frost     (1000)        0 2023-01-18 10:01:12.074738 rlberry-0.4.0/rlberry.egg-info/
--rw-r--r--   0 frost     (1000) frost     (1000)     6802 2023-01-18 10:01:11.000000 rlberry-0.4.0/rlberry.egg-info/PKG-INFO
--rw-r--r--   0 frost     (1000) frost     (1000)     9269 2023-01-18 10:01:12.000000 rlberry-0.4.0/rlberry.egg-info/SOURCES.txt
--rw-r--r--   0 frost     (1000) frost     (1000)        1 2023-01-18 10:01:11.000000 rlberry-0.4.0/rlberry.egg-info/dependency_links.txt
--rw-r--r--   0 frost     (1000) frost     (1000)        1 2023-01-18 10:00:11.000000 rlberry-0.4.0/rlberry.egg-info/not-zip-safe
--rw-r--r--   0 frost     (1000) frost     (1000)      457 2023-01-18 10:01:11.000000 rlberry-0.4.0/rlberry.egg-info/requires.txt
--rw-r--r--   0 frost     (1000) frost     (1000)        8 2023-01-18 10:01:11.000000 rlberry-0.4.0/rlberry.egg-info/top_level.txt
--rw-r--r--   0 frost     (1000) frost     (1000)       74 2023-01-18 10:01:12.098071 rlberry-0.4.0/setup.cfg
--rw-r--r--   0 frost     (1000) frost     (1000)     2181 2023-01-18 09:58:26.000000 rlberry-0.4.0/setup.py
+drwxrwxr-x   0 jteigny   (1000) jteigny   (1000)        0 2023-06-19 08:56:17.238106 rlberry-0.4.1/
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     1067 2022-05-09 08:37:51.000000 rlberry-0.4.1/LICENSE
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)       55 2022-05-09 08:37:51.000000 rlberry-0.4.1/MANIFEST.in
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     6752 2023-06-19 08:56:17.238106 rlberry-0.4.1/PKG-INFO
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     5868 2023-06-19 08:30:31.000000 rlberry-0.4.1/README.md
+drwxrwxr-x   0 jteigny   (1000) jteigny   (1000)        0 2023-06-19 08:56:17.230106 rlberry-0.4.1/assets/
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     5723 2023-06-19 08:30:31.000000 rlberry-0.4.1/assets/logo_square.svg
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     5542 2023-06-19 08:30:31.000000 rlberry-0.4.1/assets/logo_wide.svg
+drwxrwxr-x   0 jteigny   (1000) jteigny   (1000)        0 2023-06-19 08:56:17.230106 rlberry-0.4.1/rlberry/
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)      335 2022-09-26 08:44:24.000000 rlberry-0.4.1/rlberry/__init__.py
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)       23 2023-06-19 08:31:37.000000 rlberry-0.4.1/rlberry/_version.py
+drwxrwxr-x   0 jteigny   (1000) jteigny   (1000)        0 2023-06-19 08:56:17.230106 rlberry-0.4.1/rlberry/agents/
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)      530 2023-06-19 08:30:31.000000 rlberry-0.4.1/rlberry/agents/__init__.py
+drwxrwxr-x   0 jteigny   (1000) jteigny   (1000)        0 2023-06-19 08:56:17.230106 rlberry-0.4.1/rlberry/agents/adaptiveql/
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)       40 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/agents/adaptiveql/__init__.py
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     5479 2023-06-19 08:30:31.000000 rlberry-0.4.1/rlberry/agents/adaptiveql/adaptiveql.py
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     6237 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/agents/adaptiveql/tree.py
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     1691 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/agents/adaptiveql/utils.py
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)    18386 2023-06-19 08:30:31.000000 rlberry-0.4.1/rlberry/agents/agent.py
+drwxrwxr-x   0 jteigny   (1000) jteigny   (1000)        0 2023-06-19 08:56:17.230106 rlberry-0.4.1/rlberry/agents/bandits/
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)      479 2022-09-26 08:44:24.000000 rlberry-0.4.1/rlberry/agents/bandits/__init__.py
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     3361 2022-09-26 08:44:24.000000 rlberry-0.4.1/rlberry/agents/bandits/bandit_base.py
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     3300 2022-09-26 08:44:24.000000 rlberry-0.4.1/rlberry/agents/bandits/index_agents.py
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)    12014 2022-09-26 08:44:24.000000 rlberry-0.4.1/rlberry/agents/bandits/indices.py
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     4472 2022-09-26 08:44:24.000000 rlberry-0.4.1/rlberry/agents/bandits/priors.py
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     4068 2022-09-26 08:44:24.000000 rlberry-0.4.1/rlberry/agents/bandits/randomized_agents.py
+drwxrwxr-x   0 jteigny   (1000) jteigny   (1000)        0 2023-06-19 08:56:17.230106 rlberry-0.4.1/rlberry/agents/bandits/tools/
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)       35 2022-09-26 08:44:24.000000 rlberry-0.4.1/rlberry/agents/bandits/tools/__init__.py
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     8519 2022-09-26 08:44:24.000000 rlberry-0.4.1/rlberry/agents/bandits/tools/tracker.py
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     5109 2023-06-19 08:30:31.000000 rlberry-0.4.1/rlberry/agents/bandits/ts_agents.py
+drwxrwxr-x   0 jteigny   (1000) jteigny   (1000)        0 2023-06-19 08:56:17.230106 rlberry-0.4.1/rlberry/agents/dynprog/
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)       49 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/agents/dynprog/__init__.py
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     8882 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/agents/dynprog/utils.py
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     2540 2022-09-26 08:44:24.000000 rlberry-0.4.1/rlberry/agents/dynprog/value_iteration.py
+drwxrwxr-x   0 jteigny   (1000) jteigny   (1000)        0 2023-06-19 08:56:17.230106 rlberry-0.4.1/rlberry/agents/experimental/
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)        0 2022-09-26 08:44:24.000000 rlberry-0.4.1/rlberry/agents/experimental/__init__.py
+drwxrwxr-x   0 jteigny   (1000) jteigny   (1000)        0 2023-06-19 08:56:17.230106 rlberry-0.4.1/rlberry/agents/experimental/tests/
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)        0 2022-09-26 08:44:24.000000 rlberry-0.4.1/rlberry/agents/experimental/tests/__init__.py
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     1324 2022-09-26 08:44:24.000000 rlberry-0.4.1/rlberry/agents/experimental/tests/test_sac.py
+drwxrwxr-x   0 jteigny   (1000) jteigny   (1000)        0 2023-06-19 08:56:17.230106 rlberry-0.4.1/rlberry/agents/experimental/torch/
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)       26 2023-06-19 08:30:31.000000 rlberry-0.4.1/rlberry/agents/experimental/torch/__init__.py
+drwxrwxr-x   0 jteigny   (1000) jteigny   (1000)        0 2023-06-19 08:56:17.230106 rlberry-0.4.1/rlberry/agents/experimental/torch/sac/
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)       26 2022-09-26 08:44:24.000000 rlberry-0.4.1/rlberry/agents/experimental/torch/sac/__init__.py
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)    13132 2023-06-19 08:30:31.000000 rlberry-0.4.1/rlberry/agents/experimental/torch/sac/sac.py
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     2278 2023-06-19 08:30:31.000000 rlberry-0.4.1/rlberry/agents/experimental/torch/sac/utils.py
+drwxrwxr-x   0 jteigny   (1000) jteigny   (1000)        0 2023-06-19 08:56:17.230106 rlberry-0.4.1/rlberry/agents/features/
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)       36 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/agents/features/__init__.py
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)      580 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/agents/features/feature_map.py
+drwxrwxr-x   0 jteigny   (1000) jteigny   (1000)        0 2023-06-19 08:56:17.230106 rlberry-0.4.1/rlberry/agents/kernel_based/
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)       83 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/agents/kernel_based/__init__.py
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)      908 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/agents/kernel_based/common.py
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     1929 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/agents/kernel_based/kernels.py
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)    12466 2022-09-26 08:44:24.000000 rlberry-0.4.1/rlberry/agents/kernel_based/rs_kernel_ucbvi.py
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)    11254 2022-09-26 08:44:24.000000 rlberry-0.4.1/rlberry/agents/kernel_based/rs_ucbvi.py
+drwxrwxr-x   0 jteigny   (1000) jteigny   (1000)        0 2023-06-19 08:56:17.230106 rlberry-0.4.1/rlberry/agents/linear/
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)       35 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/agents/linear/__init__.py
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)    11184 2022-09-26 08:44:24.000000 rlberry-0.4.1/rlberry/agents/linear/lsvi_ucb.py
+drwxrwxr-x   0 jteigny   (1000) jteigny   (1000)        0 2023-06-19 08:56:17.230106 rlberry-0.4.1/rlberry/agents/mbqvi/
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)       30 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/agents/mbqvi/__init__.py
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     4943 2022-09-26 08:44:24.000000 rlberry-0.4.1/rlberry/agents/mbqvi/mbqvi.py
+drwxrwxr-x   0 jteigny   (1000) jteigny   (1000)        0 2023-06-19 08:56:17.230106 rlberry-0.4.1/rlberry/agents/optql/
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)       30 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/agents/optql/__init__.py
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     6595 2022-09-26 08:44:24.000000 rlberry-0.4.1/rlberry/agents/optql/optql.py
+drwxrwxr-x   0 jteigny   (1000) jteigny   (1000)        0 2023-06-19 08:56:17.230106 rlberry-0.4.1/rlberry/agents/psrl/
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)       28 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/agents/psrl/__init__.py
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     8344 2022-09-26 08:44:24.000000 rlberry-0.4.1/rlberry/agents/psrl/psrl.py
+drwxrwxr-x   0 jteigny   (1000) jteigny   (1000)        0 2023-06-19 08:56:17.230106 rlberry-0.4.1/rlberry/agents/rlsvi/
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)       30 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/agents/rlsvi/__init__.py
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     8502 2022-09-26 08:44:24.000000 rlberry-0.4.1/rlberry/agents/rlsvi/rlsvi.py
+drwxrwxr-x   0 jteigny   (1000) jteigny   (1000)        0 2023-06-19 08:56:17.234106 rlberry-0.4.1/rlberry/agents/stable_baselines/
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)       51 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/agents/stable_baselines/__init__.py
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     8702 2022-09-26 08:44:24.000000 rlberry-0.4.1/rlberry/agents/stable_baselines/stable_baselines.py
+drwxrwxr-x   0 jteigny   (1000) jteigny   (1000)        0 2023-06-19 08:56:17.234106 rlberry-0.4.1/rlberry/agents/tabular_rl/
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)       61 2023-06-19 08:30:31.000000 rlberry-0.4.1/rlberry/agents/tabular_rl/__init__.py
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     3991 2023-06-19 08:30:31.000000 rlberry-0.4.1/rlberry/agents/tabular_rl/qlearning.py
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     4042 2023-06-19 08:30:31.000000 rlberry-0.4.1/rlberry/agents/tabular_rl/sarsa.py
+drwxrwxr-x   0 jteigny   (1000) jteigny   (1000)        0 2023-06-19 08:56:17.234106 rlberry-0.4.1/rlberry/agents/tests/
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)        0 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/agents/tests/__init__.py
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)      377 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/agents/tests/test_adaptiveql.py
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     3509 2023-06-19 08:30:31.000000 rlberry-0.4.1/rlberry/agents/tests/test_bandits.py
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     4902 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/agents/tests/test_dynprog.py
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     1558 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/agents/tests/test_kernel_based.py
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     6078 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/agents/tests/test_lsvi_ucb.py
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)      808 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/agents/tests/test_mbqvi.py
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)      304 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/agents/tests/test_optql.py
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)      772 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/agents/tests/test_psrl.py
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     5707 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/agents/tests/test_replay.py
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)      507 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/agents/tests/test_rlsvi.py
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     1058 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/agents/tests/test_stable_baselines.py
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     1016 2023-06-19 08:30:31.000000 rlberry-0.4.1/rlberry/agents/tests/test_tabular_rl.py
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)      779 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/agents/tests/test_ucbvi.py
+drwxrwxr-x   0 jteigny   (1000) jteigny   (1000)        0 2023-06-19 08:56:17.234106 rlberry-0.4.1/rlberry/agents/torch/
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)      191 2023-06-19 08:30:31.000000 rlberry-0.4.1/rlberry/agents/torch/__init__.py
+drwxrwxr-x   0 jteigny   (1000) jteigny   (1000)        0 2023-06-19 08:56:17.234106 rlberry-0.4.1/rlberry/agents/torch/a2c/
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)       26 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/agents/torch/a2c/__init__.py
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)    11487 2023-06-19 08:30:31.000000 rlberry-0.4.1/rlberry/agents/torch/a2c/a2c.py
+drwxrwxr-x   0 jteigny   (1000) jteigny   (1000)        0 2023-06-19 08:56:17.234106 rlberry-0.4.1/rlberry/agents/torch/dqn/
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)       63 2023-06-19 08:30:31.000000 rlberry-0.4.1/rlberry/agents/torch/dqn/__init__.py
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)    16491 2023-06-19 08:30:31.000000 rlberry-0.4.1/rlberry/agents/torch/dqn/dqn.py
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     4226 2023-06-19 08:30:31.000000 rlberry-0.4.1/rlberry/agents/torch/dqn/dqn_utils.py
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)    17760 2023-06-19 08:30:31.000000 rlberry-0.4.1/rlberry/agents/torch/dqn/mdqn.py
+drwxrwxr-x   0 jteigny   (1000) jteigny   (1000)        0 2023-06-19 08:56:17.234106 rlberry-0.4.1/rlberry/agents/torch/ppo/
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)       26 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/agents/torch/ppo/__init__.py
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)    24870 2023-06-19 08:30:31.000000 rlberry-0.4.1/rlberry/agents/torch/ppo/ppo.py
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     5962 2023-06-19 08:30:31.000000 rlberry-0.4.1/rlberry/agents/torch/ppo/ppo_utils.py
+drwxrwxr-x   0 jteigny   (1000) jteigny   (1000)        0 2023-06-19 08:56:17.234106 rlberry-0.4.1/rlberry/agents/torch/reinforce/
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)       38 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/agents/torch/reinforce/__init__.py
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     7207 2023-06-19 08:30:31.000000 rlberry-0.4.1/rlberry/agents/torch/reinforce/reinforce.py
+drwxrwxr-x   0 jteigny   (1000) jteigny   (1000)        0 2023-06-19 08:56:17.234106 rlberry-0.4.1/rlberry/agents/torch/tests/
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)        0 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/agents/torch/tests/__init__.py
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     3388 2023-06-19 08:30:31.000000 rlberry-0.4.1/rlberry/agents/torch/tests/test_a2c.py
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     1140 2023-06-19 08:30:31.000000 rlberry-0.4.1/rlberry/agents/torch/tests/test_dqn.py
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)      692 2023-06-19 08:30:31.000000 rlberry-0.4.1/rlberry/agents/torch/tests/test_factory.py
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     1134 2023-06-19 08:30:31.000000 rlberry-0.4.1/rlberry/agents/torch/tests/test_mdqn.py
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     5752 2023-06-19 08:30:31.000000 rlberry-0.4.1/rlberry/agents/torch/tests/test_ppo.py
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     1434 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/agents/torch/tests/test_reinforce.py
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     3850 2023-06-19 08:30:31.000000 rlberry-0.4.1/rlberry/agents/torch/tests/test_torch_atari.py
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     1230 2023-06-19 08:30:31.000000 rlberry-0.4.1/rlberry/agents/torch/tests/test_torch_models.py
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     1080 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/agents/torch/tests/test_torch_training.py
+drwxrwxr-x   0 jteigny   (1000) jteigny   (1000)        0 2023-06-19 08:56:17.234106 rlberry-0.4.1/rlberry/agents/torch/utils/
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)        0 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/agents/torch/utils/__init__.py
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)    17133 2023-06-19 08:30:31.000000 rlberry-0.4.1/rlberry/agents/torch/utils/models.py
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     5201 2023-06-19 08:30:31.000000 rlberry-0.4.1/rlberry/agents/torch/utils/training.py
+drwxrwxr-x   0 jteigny   (1000) jteigny   (1000)        0 2023-06-19 08:56:17.234106 rlberry-0.4.1/rlberry/agents/ucbvi/
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)       30 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/agents/ucbvi/__init__.py
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)    10335 2022-09-26 08:44:24.000000 rlberry-0.4.1/rlberry/agents/ucbvi/ucbvi.py
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     1952 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/agents/ucbvi/utils.py
+drwxrwxr-x   0 jteigny   (1000) jteigny   (1000)        0 2023-06-19 08:56:17.234106 rlberry-0.4.1/rlberry/agents/utils/
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)        0 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/agents/utils/__init__.py
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     1525 2023-06-19 08:30:31.000000 rlberry-0.4.1/rlberry/agents/utils/memories.py
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)    14236 2023-06-19 08:30:31.000000 rlberry-0.4.1/rlberry/agents/utils/replay.py
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     5290 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/agents/utils/replay_utils.py
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)      357 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/check_packages.py
+drwxrwxr-x   0 jteigny   (1000) jteigny   (1000)        0 2023-06-19 08:56:17.234106 rlberry-0.4.1/rlberry/colab_utils/
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)        0 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/colab_utils/__init__.py
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     1053 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/colab_utils/display_setup.py
+drwxrwxr-x   0 jteigny   (1000) jteigny   (1000)        0 2023-06-19 08:56:17.234106 rlberry-0.4.1/rlberry/envs/
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)      263 2023-06-19 08:30:31.000000 rlberry-0.4.1/rlberry/envs/__init__.py
+drwxrwxr-x   0 jteigny   (1000) jteigny   (1000)        0 2023-06-19 08:56:17.234106 rlberry-0.4.1/rlberry/envs/bandits/
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)      181 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/envs/bandits/__init__.py
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     3392 2023-06-19 08:30:31.000000 rlberry-0.4.1/rlberry/envs/bandits/bandit_base.py
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     2614 2023-06-19 08:30:31.000000 rlberry-0.4.1/rlberry/envs/bandits/corrupted_bandits.py
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     1370 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/envs/bandits/stochastic_bandits.py
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     3817 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/envs/basewrapper.py
+drwxrwxr-x   0 jteigny   (1000) jteigny   (1000)        0 2023-06-19 08:56:17.234106 rlberry-0.4.1/rlberry/envs/benchmarks/
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)        0 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/envs/benchmarks/__init__.py
+drwxrwxr-x   0 jteigny   (1000) jteigny   (1000)        0 2023-06-19 08:56:17.234106 rlberry-0.4.1/rlberry/envs/benchmarks/ball_exploration/
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)       49 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/envs/benchmarks/ball_exploration/__init__.py
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     4995 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/envs/benchmarks/ball_exploration/ball2d.py
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)    14237 2022-09-26 08:44:24.000000 rlberry-0.4.1/rlberry/envs/benchmarks/ball_exploration/pball.py
+drwxrwxr-x   0 jteigny   (1000) jteigny   (1000)        0 2023-06-19 08:56:17.234106 rlberry-0.4.1/rlberry/envs/benchmarks/generalization/
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)        0 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/envs/benchmarks/generalization/__init__.py
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     5440 2023-06-19 08:30:31.000000 rlberry-0.4.1/rlberry/envs/benchmarks/generalization/twinrooms.py
+drwxrwxr-x   0 jteigny   (1000) jteigny   (1000)        0 2023-06-19 08:56:17.234106 rlberry-0.4.1/rlberry/envs/benchmarks/grid_exploration/
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)        0 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/envs/benchmarks/grid_exploration/__init__.py
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     5294 2023-06-19 08:30:31.000000 rlberry-0.4.1/rlberry/envs/benchmarks/grid_exploration/apple_gold.py
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     3816 2022-09-26 08:44:24.000000 rlberry-0.4.1/rlberry/envs/benchmarks/grid_exploration/four_room.py
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)    10490 2023-06-19 08:30:31.000000 rlberry-0.4.1/rlberry/envs/benchmarks/grid_exploration/nroom.py
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     4229 2023-06-19 08:30:31.000000 rlberry-0.4.1/rlberry/envs/benchmarks/grid_exploration/six_room.py
+drwxrwxr-x   0 jteigny   (1000) jteigny   (1000)        0 2023-06-19 08:56:17.234106 rlberry-0.4.1/rlberry/envs/classic_control/
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)    18518 2022-09-26 08:44:24.000000 rlberry-0.4.1/rlberry/envs/classic_control/SpringCartPole.py
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)      141 2022-09-26 08:44:24.000000 rlberry-0.4.1/rlberry/envs/classic_control/__init__.py
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)    11984 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/envs/classic_control/acrobot.py
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     5938 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/envs/classic_control/mountain_car.py
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     3635 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/envs/classic_control/pendulum.py
+drwxrwxr-x   0 jteigny   (1000) jteigny   (1000)        0 2023-06-19 08:56:17.234106 rlberry-0.4.1/rlberry/envs/finite/
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)       92 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/envs/finite/__init__.py
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     3956 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/envs/finite/chain.py
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     5594 2022-09-26 08:44:24.000000 rlberry-0.4.1/rlberry/envs/finite/finite_mdp.py
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)    16178 2023-06-19 08:30:31.000000 rlberry-0.4.1/rlberry/envs/finite/gridworld.py
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     2011 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/envs/finite/gridworld_utils.py
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     3776 2023-06-19 08:30:31.000000 rlberry-0.4.1/rlberry/envs/gym_make.py
+drwxrwxr-x   0 jteigny   (1000) jteigny   (1000)        0 2023-06-19 08:56:17.234106 rlberry-0.4.1/rlberry/envs/interface/
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)       25 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/envs/interface/__init__.py
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     4813 2022-09-26 08:44:24.000000 rlberry-0.4.1/rlberry/envs/interface/model.py
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     1227 2023-06-19 08:30:31.000000 rlberry-0.4.1/rlberry/envs/pipeline.py
+drwxrwxr-x   0 jteigny   (1000) jteigny   (1000)        0 2023-06-19 08:56:17.234106 rlberry-0.4.1/rlberry/envs/tests/
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)        0 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/envs/tests/__init__.py
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     1593 2023-06-19 08:30:31.000000 rlberry-0.4.1/rlberry/envs/tests/test_bandits.py
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     2589 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/envs/tests/test_env_seeding.py
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     2225 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/envs/tests/test_gym_env_seeding.py
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     7440 2023-06-19 08:30:31.000000 rlberry-0.4.1/rlberry/envs/tests/test_instantiation.py
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     2635 2023-06-19 08:30:31.000000 rlberry-0.4.1/rlberry/envs/tests/test_spring_env.py
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)      845 2022-09-26 08:44:24.000000 rlberry-0.4.1/rlberry/envs/utils.py
+drwxrwxr-x   0 jteigny   (1000) jteigny   (1000)        0 2023-06-19 08:56:17.234106 rlberry-0.4.1/rlberry/experiment/
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)      142 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/experiment/__init__.py
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     1815 2023-06-19 08:30:31.000000 rlberry-0.4.1/rlberry/experiment/generator.py
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     3705 2022-09-26 08:44:24.000000 rlberry-0.4.1/rlberry/experiment/load_results.py
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     6283 2023-06-19 08:30:31.000000 rlberry-0.4.1/rlberry/experiment/yaml_utils.py
+drwxrwxr-x   0 jteigny   (1000) jteigny   (1000)        0 2023-06-19 08:56:17.238106 rlberry-0.4.1/rlberry/exploration_tools/
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)        0 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/exploration_tools/__init__.py
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     3507 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/exploration_tools/discrete_counter.py
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     6179 2022-09-26 08:44:24.000000 rlberry-0.4.1/rlberry/exploration_tools/online_discretization_counter.py
+drwxrwxr-x   0 jteigny   (1000) jteigny   (1000)        0 2023-06-19 08:56:17.238106 rlberry-0.4.1/rlberry/exploration_tools/tests/
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)        0 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/exploration_tools/tests/__init__.py
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     4326 2023-06-19 08:30:31.000000 rlberry-0.4.1/rlberry/exploration_tools/tests/test_discrete_counter.py
+drwxrwxr-x   0 jteigny   (1000) jteigny   (1000)        0 2023-06-19 08:56:17.238106 rlberry-0.4.1/rlberry/exploration_tools/torch/
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)        0 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/exploration_tools/torch/__init__.py
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     7356 2023-06-19 08:30:31.000000 rlberry-0.4.1/rlberry/exploration_tools/torch/rnd.py
+drwxrwxr-x   0 jteigny   (1000) jteigny   (1000)        0 2023-06-19 08:56:17.238106 rlberry-0.4.1/rlberry/exploration_tools/torch/tests/
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)        0 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/exploration_tools/torch/tests/__init__.py
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)      711 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/exploration_tools/torch/tests/test_rnd.py
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     2341 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/exploration_tools/typing.py
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     1012 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/exploration_tools/uncertainty_estimator.py
+drwxrwxr-x   0 jteigny   (1000) jteigny   (1000)        0 2023-06-19 08:56:17.238106 rlberry-0.4.1/rlberry/manager/
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)      180 2023-06-19 08:30:31.000000 rlberry-0.4.1/rlberry/manager/__init__.py
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)    48007 2023-06-19 08:30:31.000000 rlberry-0.4.1/rlberry/manager/agent_manager.py
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)    19901 2023-06-19 08:30:31.000000 rlberry-0.4.1/rlberry/manager/evaluation.py
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     2967 2022-09-26 08:44:24.000000 rlberry-0.4.1/rlberry/manager/multiple_managers.py
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     7863 2022-09-26 08:44:24.000000 rlberry-0.4.1/rlberry/manager/remote_agent_manager.py
+drwxrwxr-x   0 jteigny   (1000) jteigny   (1000)        0 2023-06-19 08:56:17.238106 rlberry-0.4.1/rlberry/manager/tests/
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)        0 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/manager/tests/__init__.py
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)    10244 2023-06-19 08:30:31.000000 rlberry-0.4.1/rlberry/manager/tests/test_agent_manager.py
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     2648 2022-09-26 08:44:24.000000 rlberry-0.4.1/rlberry/manager/tests/test_agent_manager_seeding.py
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     5965 2023-06-19 08:30:31.000000 rlberry-0.4.1/rlberry/manager/tests/test_hyperparam_optim.py
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     4544 2023-06-19 08:30:31.000000 rlberry-0.4.1/rlberry/manager/tests/test_plot.py
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     1249 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/manager/tests/test_shared_data.py
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)      391 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/manager/utils.py
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     1947 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/metadata_utils.py
+drwxrwxr-x   0 jteigny   (1000) jteigny   (1000)        0 2023-06-19 08:56:17.238106 rlberry-0.4.1/rlberry/network/
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)        0 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/network/__init__.py
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     1522 2023-06-19 08:30:31.000000 rlberry-0.4.1/rlberry/network/client.py
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     2836 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/network/interface.py
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     6408 2022-09-26 08:44:24.000000 rlberry-0.4.1/rlberry/network/server.py
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     5062 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/network/server_utils.py
+drwxrwxr-x   0 jteigny   (1000) jteigny   (1000)        0 2023-06-19 08:56:17.238106 rlberry-0.4.1/rlberry/network/tests/
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)        0 2023-06-19 08:30:31.000000 rlberry-0.4.1/rlberry/network/tests/__init__.py
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     1393 2023-06-19 08:30:31.000000 rlberry-0.4.1/rlberry/network/tests/conftest.py
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     2792 2023-06-19 08:30:31.000000 rlberry-0.4.1/rlberry/network/tests/test_server.py
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     2631 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/network/utils.py
+drwxrwxr-x   0 jteigny   (1000) jteigny   (1000)        0 2023-06-19 08:56:17.238106 rlberry-0.4.1/rlberry/rendering/
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)      138 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/rendering/__init__.py
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     1001 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/rendering/common_shapes.py
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     1265 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/rendering/core.py
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     7709 2023-06-19 08:30:31.000000 rlberry-0.4.1/rlberry/rendering/opengl_render2d.py
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     5931 2023-06-19 08:30:31.000000 rlberry-0.4.1/rlberry/rendering/pygame_render2d.py
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     4427 2023-06-19 08:30:31.000000 rlberry-0.4.1/rlberry/rendering/render_interface.py
+drwxrwxr-x   0 jteigny   (1000) jteigny   (1000)        0 2023-06-19 08:56:17.238106 rlberry-0.4.1/rlberry/rendering/tests/
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)        0 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/rendering/tests/__init__.py
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     3049 2023-06-19 08:30:31.000000 rlberry-0.4.1/rlberry/rendering/tests/test_rendering_interface.py
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     1864 2022-09-26 08:44:24.000000 rlberry-0.4.1/rlberry/rendering/utils.py
+drwxrwxr-x   0 jteigny   (1000) jteigny   (1000)        0 2023-06-19 08:56:17.238106 rlberry-0.4.1/rlberry/seeding/
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)       99 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/seeding/__init__.py
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     3973 2022-09-26 08:44:24.000000 rlberry-0.4.1/rlberry/seeding/seeder.py
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     2105 2022-09-26 08:44:24.000000 rlberry-0.4.1/rlberry/seeding/seeding.py
+drwxrwxr-x   0 jteigny   (1000) jteigny   (1000)        0 2023-06-19 08:56:17.238106 rlberry-0.4.1/rlberry/seeding/tests/
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)        0 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/seeding/tests/__init__.py
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     1728 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/seeding/tests/test_seeding.py
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)      874 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/seeding/tests/test_threads.py
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     1072 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/seeding/tests/test_threads_torch.py
+drwxrwxr-x   0 jteigny   (1000) jteigny   (1000)        0 2023-06-19 08:56:17.238106 rlberry-0.4.1/rlberry/spaces/
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)      180 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/spaces/__init__.py
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     3003 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/spaces/box.py
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)      807 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/spaces/dict.py
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     1553 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/spaces/discrete.py
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     1429 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/spaces/from_gym.py
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     1261 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/spaces/multi_binary.py
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     1347 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/spaces/multi_discrete.py
+drwxrwxr-x   0 jteigny   (1000) jteigny   (1000)        0 2023-06-19 08:56:17.238106 rlberry-0.4.1/rlberry/spaces/tests/
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)        0 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/spaces/tests/__init__.py
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     4724 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/spaces/tests/test_from_gym.py
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     3611 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/spaces/tests/test_spaces.py
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)      763 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/spaces/tuple.py
+drwxrwxr-x   0 jteigny   (1000) jteigny   (1000)        0 2023-06-19 08:56:17.238106 rlberry-0.4.1/rlberry/tests/
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)        0 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/tests/__init__.py
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     2397 2023-06-19 08:30:31.000000 rlberry-0.4.1/rlberry/tests/test_agent_extra.py
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     1878 2023-06-19 08:30:31.000000 rlberry-0.4.1/rlberry/tests/test_agents_base.py
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)      760 2023-06-19 08:30:31.000000 rlberry-0.4.1/rlberry/tests/test_envs.py
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)      283 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/types.py
+drwxrwxr-x   0 jteigny   (1000) jteigny   (1000)        0 2023-06-19 08:56:17.238106 rlberry-0.4.1/rlberry/utils/
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)      228 2022-09-26 08:44:24.000000 rlberry-0.4.1/rlberry/utils/__init__.py
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     1177 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/utils/binsearch.py
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)    23015 2023-06-19 08:30:31.000000 rlberry-0.4.1/rlberry/utils/check_agent.py
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     1728 2023-06-19 08:30:31.000000 rlberry-0.4.1/rlberry/utils/check_bandit_agent.py
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     1478 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/utils/check_env.py
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)    10915 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/utils/check_gym_env.py
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)      199 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/utils/factory.py
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)      847 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/utils/io.py
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)      395 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/utils/jit_setup.py
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     3453 2022-09-26 08:44:24.000000 rlberry-0.4.1/rlberry/utils/logging.py
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)      326 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/utils/math.py
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)      699 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/utils/metrics.py
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     2200 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/utils/space_discretizer.py
+drwxrwxr-x   0 jteigny   (1000) jteigny   (1000)        0 2023-06-19 08:56:17.238106 rlberry-0.4.1/rlberry/utils/tests/
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)        0 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/utils/tests/__init__.py
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     1061 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/utils/tests/test_binsearch.py
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     2976 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/utils/tests/test_check.py
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)      483 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/utils/tests/test_metrics.py
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     1410 2022-09-26 08:44:24.000000 rlberry-0.4.1/rlberry/utils/tests/test_writer.py
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     2517 2022-09-26 08:44:24.000000 rlberry-0.4.1/rlberry/utils/torch.py
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)    17154 2023-06-19 08:30:31.000000 rlberry-0.4.1/rlberry/utils/writers.py
+drwxrwxr-x   0 jteigny   (1000) jteigny   (1000)        0 2023-06-19 08:56:17.238106 rlberry-0.4.1/rlberry/wrappers/
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)      195 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/wrappers/__init__.py
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     5812 2022-10-06 15:00:01.000000 rlberry-0.4.1/rlberry/wrappers/atari_utils.py
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)      890 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/wrappers/autoreset.py
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)      962 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/wrappers/discrete2onehot.py
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     3273 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/wrappers/discretize_state.py
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     1217 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/wrappers/gym_utils.py
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     2064 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/wrappers/rescale_reward.py
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)      551 2023-06-19 08:30:31.000000 rlberry-0.4.1/rlberry/wrappers/scalarize.py
+drwxrwxr-x   0 jteigny   (1000) jteigny   (1000)        0 2023-06-19 08:56:17.238106 rlberry-0.4.1/rlberry/wrappers/tests/
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)        0 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/wrappers/tests/__init__.py
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)      776 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/wrappers/tests/test_basewrapper.py
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     5701 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/wrappers/tests/test_common_wrappers.py
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     2988 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/wrappers/tests/test_gym_space_conversion.py
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     3981 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/wrappers/tests/test_wrapper_seeding.py
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     1114 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/wrappers/tests/test_writer_utils.py
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     3482 2022-09-26 08:44:24.000000 rlberry-0.4.1/rlberry/wrappers/uncertainty_estimator_wrapper.py
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)    14355 2022-09-26 08:44:24.000000 rlberry-0.4.1/rlberry/wrappers/vis2d.py
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     1425 2022-05-09 08:37:51.000000 rlberry-0.4.1/rlberry/wrappers/writer_utils.py
+drwxrwxr-x   0 jteigny   (1000) jteigny   (1000)        0 2023-06-19 08:56:17.230106 rlberry-0.4.1/rlberry.egg-info/
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     6752 2023-06-19 08:56:17.000000 rlberry-0.4.1/rlberry.egg-info/PKG-INFO
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     9039 2023-06-19 08:56:17.000000 rlberry-0.4.1/rlberry.egg-info/SOURCES.txt
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)        1 2023-06-19 08:56:17.000000 rlberry-0.4.1/rlberry.egg-info/dependency_links.txt
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)        1 2022-05-10 07:35:31.000000 rlberry-0.4.1/rlberry.egg-info/not-zip-safe
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)      514 2023-06-19 08:56:17.000000 rlberry-0.4.1/rlberry.egg-info/requires.txt
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)        8 2023-06-19 08:56:17.000000 rlberry-0.4.1/rlberry.egg-info/top_level.txt
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)       74 2023-06-19 08:56:17.238106 rlberry-0.4.1/setup.cfg
+-rw-rw-r--   0 jteigny   (1000) jteigny   (1000)     2332 2023-06-19 08:56:07.000000 rlberry-0.4.1/setup.py
```

### Comparing `rlberry-0.4.0/LICENSE` & `rlberry-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `rlberry-0.4.0/PKG-INFO` & `rlberry-0.4.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,54 +1,54 @@
 Metadata-Version: 2.1
 Name: rlberry
-Version: 0.4.0
+Version: 0.4.1
 Summary: An easy-to-use reinforcement learning library for research and education
 Home-page: https://github.com/rlberry-py
 Author: Omar Darwiche Domingues, Yannis Flet-Berliac, Edouard Leurent, Pierre Menard, Xuedong Shang
 License: MIT
+Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Education
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 Provides-Extra: default
+Provides-Extra: deploy
 Provides-Extra: jax_agents
 Provides-Extra: torch_agents
-Provides-Extra: deploy
 License-File: LICENSE
 
 <!-- Logo -->
 <p align="center">
    <img src="https://raw.githubusercontent.com/rlberry-py/rlberry/main/assets/logo_wide.svg" width="50%">
 </p>
 
 
+
 <!-- Short description -->
 <p align="center">
    A Reinforcement Learning Library for Research and Education
 </p>
 
+
 <!-- The badges -->
 <p align="center">
    <a href="https://github.com/rlberry-py/rlberry/workflows/test/badge.svg">
       <img alt="pytest" src="https://github.com/rlberry-py/rlberry/workflows/test/badge.svg">
    </a>
    <a href='https://rlberry.readthedocs.io/en/latest/?badge=latest'>
       <img alt="Documentation Status" src="https://readthedocs.org/projects/rlberry/badge/?version=latest">
    </a>
    <a href="https://img.shields.io/github/contributors/rlberry-py/rlberry">
       <img alt="contributors" src="https://img.shields.io/github/contributors/rlberry-py/rlberry">
    </a>
-   <a href="https://app.codacy.com/gh/rlberry-py/rlberry?utm_source=github.com&utm_medium=referral&utm_content=rlberry-py/rlberry&utm_campaign=Badge_Grade">
-      <img alt="Codacy" src="https://api.codacy.com/project/badge/Grade/27e91674d18a4ac49edf91c339af1502">
-   </a>
    <a href="https://codecov.io/gh/rlberry-py/rlberry">
       <img alt="codecov" src="https://codecov.io/gh/rlberry-py/rlberry/branch/main/graph/badge.svg?token=TIFP7RUD75">
      </a>
 </p>
 
 <p align="center">
    <!-- <a href="https://img.shields.io/pypi/pyversions/rlberry">
@@ -142,11 +142,18 @@
 
 The modules listed below are experimental at the moment, that is, they are not thoroughly tested and are susceptible to evolve.
 
 * `rlberry.network`: Allows communication between a server and client via sockets, and can be used to run agents remotely.
 * `rlberry.agents.experimental`: Experimental agents that are not thoroughly tested.
 
 
+## About us
+This project was initiated and is actively maintained by [INRIA SCOOL team](https://team.inria.fr/scool/).
+More information [here](https://rlberry.readthedocs.io/en/latest/about.html#).
+
+
 ## Contributing
 
 Want to contribute to `rlberry`? Please check [our contribution guidelines](https://rlberry.readthedocs.io/en/latest/contributing.html). **If you want to add any new agents or environments, do not hesitate
 to [open an issue](https://github.com/rlberry-py/rlberry/issues/new/choose)!**
+
+
```

#### html2text {}

```diff
@@ -1,23 +1,23 @@
-Metadata-Version: 2.1 Name: rlberry Version: 0.4.0 Summary: An easy-to-use
+Metadata-Version: 2.1 Name: rlberry Version: 0.4.1 Summary: An easy-to-use
 reinforcement learning library for research and education Home-page: https://
 github.com/rlberry-py Author: Omar Darwiche Domingues, Yannis Flet-Berliac,
-Edouard Leurent, Pierre Menard, Xuedong Shang License: MIT Classifier:
-Development Status :: 4 - Beta Classifier: Intended Audience :: Science/
-Research Classifier: Intended Audience :: Education Classifier: Topic ::
-Scientific/Engineering :: Artificial Intelligence Classifier: Programming
+Edouard Leurent, Pierre Menard, Xuedong Shang License: MIT Platform: UNKNOWN
+Classifier: Development Status :: 4 - Beta Classifier: Intended Audience ::
+Science/Research Classifier: Intended Audience :: Education Classifier: Topic
+:: Scientific/Engineering :: Artificial Intelligence Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3 ::
 Only Classifier: License :: OSI Approved :: MIT License Classifier: Operating
 System :: OS Independent Description-Content-Type: text/markdown Provides-
-Extra: default Provides-Extra: jax_agents Provides-Extra: torch_agents
-Provides-Extra: deploy License-File: LICENSE
+Extra: default Provides-Extra: deploy Provides-Extra: jax_agents Provides-
+Extra: torch_agents License-File: LICENSE
       [https://raw.githubusercontent.com/rlberry-py/rlberry/main/assets/
                                 logo_wide.svg]
           A Reinforcement Learning Library for Research and Education
-       [pytest] [Documentation_Status] [contributors] [Codacy] [codecov]
+           [pytest] [Documentation_Status] [contributors] [codecov]
 
                     Try_it_on_Google_Colab!_[Open_In_Colab]
 
 ===============================================================================
  ## What is `rlberry`? **Writing reinforcement learning algorithms is fun!**
 *But after the fun, we have lots of boring things to implement*: run our agents
 in parallel, average and plot results, optimize hyperparameters, compare to
@@ -48,12 +48,14 @@
 Valko, Michal}, doi = {10.5281/zenodo.5544540}, month = {10}, title = {{rlberry
 - A Reinforcement Learning Library for Research and Education}}, url = {https:/
 /github.com/rlberry-py/rlberry}, year = {2021} } ``` ## Development notes The
 modules listed below are experimental at the moment, that is, they are not
 thoroughly tested and are susceptible to evolve. * `rlberry.network`: Allows
 communication between a server and client via sockets, and can be used to run
 agents remotely. * `rlberry.agents.experimental`: Experimental agents that are
-not thoroughly tested. ## Contributing Want to contribute to `rlberry`? Please
-check [our contribution guidelines](https://rlberry.readthedocs.io/en/latest/
-contributing.html). **If you want to add any new agents or environments, do not
-hesitate to [open an issue](https://github.com/rlberry-py/rlberry/issues/new/
-choose)!**
+not thoroughly tested. ## About us This project was initiated and is actively
+maintained by [INRIA SCOOL team](https://team.inria.fr/scool/). More
+information [here](https://rlberry.readthedocs.io/en/latest/about.html#). ##
+Contributing Want to contribute to `rlberry`? Please check [our contribution
+guidelines](https://rlberry.readthedocs.io/en/latest/contributing.html). **If
+you want to add any new agents or environments, do not hesitate to [open an
+issue](https://github.com/rlberry-py/rlberry/issues/new/choose)!**
```

### Comparing `rlberry-0.4.0/README.md` & `rlberry-0.4.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,32 +1,31 @@
 <!-- Logo -->
 <p align="center">
    <img src="https://raw.githubusercontent.com/rlberry-py/rlberry/main/assets/logo_wide.svg" width="50%">
 </p>
 
 
+
 <!-- Short description -->
 <p align="center">
    A Reinforcement Learning Library for Research and Education
 </p>
 
+
 <!-- The badges -->
 <p align="center">
    <a href="https://github.com/rlberry-py/rlberry/workflows/test/badge.svg">
       <img alt="pytest" src="https://github.com/rlberry-py/rlberry/workflows/test/badge.svg">
    </a>
    <a href='https://rlberry.readthedocs.io/en/latest/?badge=latest'>
       <img alt="Documentation Status" src="https://readthedocs.org/projects/rlberry/badge/?version=latest">
    </a>
    <a href="https://img.shields.io/github/contributors/rlberry-py/rlberry">
       <img alt="contributors" src="https://img.shields.io/github/contributors/rlberry-py/rlberry">
    </a>
-   <a href="https://app.codacy.com/gh/rlberry-py/rlberry?utm_source=github.com&utm_medium=referral&utm_content=rlberry-py/rlberry&utm_campaign=Badge_Grade">
-      <img alt="Codacy" src="https://api.codacy.com/project/badge/Grade/27e91674d18a4ac49edf91c339af1502">
-   </a>
    <a href="https://codecov.io/gh/rlberry-py/rlberry">
       <img alt="codecov" src="https://codecov.io/gh/rlberry-py/rlberry/branch/main/graph/badge.svg?token=TIFP7RUD75">
      </a>
 </p>
 
 <p align="center">
    <!-- <a href="https://img.shields.io/pypi/pyversions/rlberry">
@@ -120,11 +119,16 @@
 
 The modules listed below are experimental at the moment, that is, they are not thoroughly tested and are susceptible to evolve.
 
 * `rlberry.network`: Allows communication between a server and client via sockets, and can be used to run agents remotely.
 * `rlberry.agents.experimental`: Experimental agents that are not thoroughly tested.
 
 
+## About us
+This project was initiated and is actively maintained by [INRIA SCOOL team](https://team.inria.fr/scool/).
+More information [here](https://rlberry.readthedocs.io/en/latest/about.html#).
+
+
 ## Contributing
 
 Want to contribute to `rlberry`? Please check [our contribution guidelines](https://rlberry.readthedocs.io/en/latest/contributing.html). **If you want to add any new agents or environments, do not hesitate
 to [open an issue](https://github.com/rlberry-py/rlberry/issues/new/choose)!**
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
       [https://raw.githubusercontent.com/rlberry-py/rlberry/main/assets/
                                 logo_wide.svg]
           A Reinforcement Learning Library for Research and Education
-       [pytest] [Documentation_Status] [contributors] [Codacy] [codecov]
+           [pytest] [Documentation_Status] [contributors] [codecov]
 
                     Try_it_on_Google_Colab!_[Open_In_Colab]
 
 ===============================================================================
  ## What is `rlberry`? **Writing reinforcement learning algorithms is fun!**
 *But after the fun, we have lots of boring things to implement*: run our agents
 in parallel, average and plot results, optimize hyperparameters, compare to
@@ -36,12 +36,14 @@
 Valko, Michal}, doi = {10.5281/zenodo.5544540}, month = {10}, title = {{rlberry
 - A Reinforcement Learning Library for Research and Education}}, url = {https:/
 /github.com/rlberry-py/rlberry}, year = {2021} } ``` ## Development notes The
 modules listed below are experimental at the moment, that is, they are not
 thoroughly tested and are susceptible to evolve. * `rlberry.network`: Allows
 communication between a server and client via sockets, and can be used to run
 agents remotely. * `rlberry.agents.experimental`: Experimental agents that are
-not thoroughly tested. ## Contributing Want to contribute to `rlberry`? Please
-check [our contribution guidelines](https://rlberry.readthedocs.io/en/latest/
-contributing.html). **If you want to add any new agents or environments, do not
-hesitate to [open an issue](https://github.com/rlberry-py/rlberry/issues/new/
-choose)!**
+not thoroughly tested. ## About us This project was initiated and is actively
+maintained by [INRIA SCOOL team](https://team.inria.fr/scool/). More
+information [here](https://rlberry.readthedocs.io/en/latest/about.html#). ##
+Contributing Want to contribute to `rlberry`? Please check [our contribution
+guidelines](https://rlberry.readthedocs.io/en/latest/contributing.html). **If
+you want to add any new agents or environments, do not hesitate to [open an
+issue](https://github.com/rlberry-py/rlberry/issues/new/choose)!**
```

### Comparing `rlberry-0.4.0/assets/logo_square.svg` & `rlberry-0.4.1/assets/logo_square.svg`

 * *Files 0% similar despite different names*

```diff
@@ -351,8 +351,8 @@
 000015e0: 2e33 392c 3135 362e 3836 5a22 2f3e 0a20  .39,156.86Z"/>. 
 000015f0: 2020 2020 2020 2020 2020 203c 656c 6c69             <elli
 00001600: 7073 6520 636c 6173 733d 2263 6c73 2d31  pse class="cls-1
 00001610: 2220 6378 3d22 3636 2220 6379 3d22 3137  " cx="66" cy="17
 00001620: 302e 3933 2220 7278 3d22 3133 2e33 3622  0.93" rx="13.36"
 00001630: 2072 793d 2231 362e 3139 222f 3e0a 2020   ry="16.19"/>.  
 00001640: 2020 2020 2020 3c2f 673e 0a20 2020 203c        </g>.    <
-00001650: 2f67 3e0a 3c2f 7376 673e                 /g>.</svg>
+00001650: 2f67 3e0a 3c2f 7376 673e 0a              /g>.</svg>.
```

### Comparing `rlberry-0.4.0/assets/logo_wide.svg` & `rlberry-0.4.1/assets/logo_wide.svg`

 * *Files 0% similar despite different names*

```diff
@@ -340,8 +340,8 @@
 00001530: 2e36 372c 3633 362e 3633 2c36 312e 3931  .67,636.63,61.91
 00001540: 5a22 2f3e 0a20 2020 2020 2020 2020 2020  Z"/>.           
 00001550: 203c 6369 7263 6c65 2063 6c61 7373 3d22   <circle class="
 00001560: 636c 732d 3122 2063 783d 2233 3433 2e33  cls-1" cx="343.3
 00001570: 3922 2063 793d 2239 312e 3122 2072 3d22  9" cy="91.1" r="
 00001580: 3237 2e33 3922 2f3e 0a20 2020 2020 2020  27.39"/>.       
 00001590: 203c 2f67 3e0a 2020 2020 3c2f 673e 0a3c   </g>.    </g>.<
-000015a0: 2f73 7667 3e                             /svg>
+000015a0: 2f73 7667 3e0a                           /svg>.
```

### Comparing `rlberry-0.4.0/rlberry/agents/adaptiveql/adaptiveql.py` & `rlberry-0.4.1/rlberry/agents/adaptiveql/adaptiveql.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     with continuous (Box) states and **discrete actions**.
 
     .. todo:: Handle continuous actios too.
 
     Parameters
     ----------
     env : gym.Env
-        Environment with discrete states and actions.
+        Environment with continuous states and discrete actions.
     gamma : double, default: 1.0
         Discount factor in [0, 1].
     horizon : int
         Horizon of the objective function.
     bonus_scale_factor : double, default: 1.0
         Constant by which to multiply the exploration bonus, controls
         the level of exploration.
```

### Comparing `rlberry-0.4.0/rlberry/agents/adaptiveql/tree.py` & `rlberry-0.4.1/rlberry/agents/adaptiveql/tree.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.4.0/rlberry/agents/adaptiveql/utils.py` & `rlberry-0.4.1/rlberry/agents/adaptiveql/utils.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.4.0/rlberry/agents/agent.py` & `rlberry-0.4.1/rlberry/agents/agent.py`

 * *Files 1% similar despite different names*

```diff
@@ -99,15 +99,15 @@
 
         self.seeder = Seeder(seeder)
         self.env = process_env(env, self.seeder, copy_env=copy_env)
 
         self.compress_pickle = compress_pickle
         # evaluation environment
         eval_env = eval_env or env
-        self.eval_env = process_env(eval_env, self.seeder, copy_env=True)
+        self.eval_env = process_env(eval_env, self.seeder, copy_env=copy_env)
 
         # metadata
         self._execution_metadata = (
             _execution_metadata or metadata_utils.ExecutionMetadata()
         )
         self._unique_id = metadata_utils.get_unique_id(self)
         if self.name:
```

### Comparing `rlberry-0.4.0/rlberry/agents/bandits/bandit_base.py` & `rlberry-0.4.1/rlberry/agents/bandits/bandit_base.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.4.0/rlberry/agents/bandits/index_agents.py` & `rlberry-0.4.1/rlberry/agents/bandits/index_agents.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.4.0/rlberry/agents/bandits/indices.py` & `rlberry-0.4.1/rlberry/agents/bandits/indices.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.4.0/rlberry/agents/bandits/priors.py` & `rlberry-0.4.1/rlberry/agents/bandits/priors.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.4.0/rlberry/agents/bandits/randomized_agents.py` & `rlberry-0.4.1/rlberry/agents/bandits/randomized_agents.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.4.0/rlberry/agents/bandits/tools/tracker.py` & `rlberry-0.4.1/rlberry/agents/bandits/tools/tracker.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.4.0/rlberry/agents/bandits/ts_agents.py` & `rlberry-0.4.1/rlberry/agents/bandits/ts_agents.py`

 * *Files 0% similar despite different names*

```diff
@@ -64,15 +64,14 @@
     """
 
     name = "TSAgent"
 
     def __init__(self, env, prior_info=None, **kwargs):
         BanditWithSimplePolicy.__init__(self, env, **kwargs)
         if prior_info is None:
-
             # Beta-Bernoulli prior by default
             def prior_params(tr):
                 """
                 The mean of a Bernoulli arm B(p) has prior distribution Beta(a, b),
                 where a is the number of success + 1, b the number of failures + 1.
                 """
                 return [
```

### Comparing `rlberry-0.4.0/rlberry/agents/dynprog/utils.py` & `rlberry-0.4.1/rlberry/agents/dynprog/utils.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.4.0/rlberry/agents/dynprog/value_iteration.py` & `rlberry-0.4.1/rlberry/agents/dynprog/value_iteration.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.4.0/rlberry/agents/experimental/jax/dqn/dqn.py` & `rlberry-0.4.1/rlberry/agents/torch/dqn/dqn.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,451 +1,451 @@
-"""
-Important
----------
-
-There is something very weird happening when using this agent with the optimize_hyperparams()
-method of AgentManager.
-If @functools.partial(jax.jit, static_argnums=(0,)) is used as a decorator to jit
-the learner_step() and actor_step() methods, the memory use increases a lot
-as the number of optuna trials increases.
-
-Using the following instead (in __init__):
-        self.actor_step = jax.jit(self._actor_step)
-        self.learner_step = jax.jit(self._learner_step)
-seems to solve the issue.
-
-However, if we jit the loss function before, as:
-        self._loss = jax.jit(self._loss)
-        self.actor_step = jax.jit(self._actor_step)
-        self.learner_step = jax.jit(self._learner_step)
-the memory issue comes back!
-
-It does not seem to be the same issue as this one: https://github.com/google/jax/issues/2072
-
-TODO: try to reproduce this issue with a simple example.
-"""
-
-import chex
-import functools
-import haiku as hk
-import jax
-import jax.numpy as jnp
+import inspect
+from typing import Callable, Optional, Union
 
+from gym import spaces
 import numpy as np
-import optax
-import dill
-import rlberry.agents.experimental.jax.nets.common as nets
-import rlax
+import torch
 
-from gym import spaces
-from pathlib import Path
 from rlberry import types
 from rlberry.agents import AgentWithSimplePolicy
-from rlberry.agents.experimental.jax.utils.replay_buffer import ReplayBuffer
-from typing import Any, Callable, Mapping, Optional
+from rlberry.agents.torch.utils.training import (
+    loss_function_factory,
+    model_factory,
+    optimizer_factory,
+    size_model_config,
+)
+from rlberry.agents.torch.dqn.dqn_utils import polynomial_schedule, lambda_returns
+from rlberry.agents.utils import replay
+from rlberry.utils.torch import choose_device
+from rlberry.utils.factory import load
+
 
 import rlberry
 
 logger = rlberry.logger
 
 
-@chex.dataclass
-class AllParams:
-    online: chex.ArrayTree
-    target: chex.ArrayTree
-
-
-@chex.dataclass
-class AllStates:
-    optimizer: chex.ArrayTree
-    learner_steps: int
-    actor_steps: int
-
-
-@chex.dataclass
-class ActorOutput:
-    actions: chex.Array
-    q_values: chex.Array
+def default_q_net_fn(env, **kwargs):
+    """
+    Returns a default Q value network.
+    """
+    del kwargs
+    model_config = {
+        "type": "MultiLayerPerceptron",
+        "layer_sizes": (64, 64),
+        "reshape": False,
+    }
+    model_config = size_model_config(env, **model_config)
+    return model_factory(**model_config)
 
 
 class DQNAgent(AgentWithSimplePolicy):
-    """
-    Implementation of Deep Q-Learning using JAX.
+    """DQN Agent based on PyTorch.
+
+    Notes
+    -----
+    Uses Q(lambda) for computing targets by default. To recover
+    the standard DQN, set :code:`lambda_ = 0.0` and :code:`chunk_size = 1`.
 
     Parameters
     ----------
-    env : types.Env
-        Environment.
-    gamma : float
+    env: :class:`~rlberry.types.Env`
+        Environment, can be a tuple (constructor, kwargs)
+    gamma: float, default = 0.99
         Discount factor.
-    batch_size : int
-        Batch size (in number of chunks).
-    chunk_size : int
-        Size of trajectory chunks to sample from the buffer.
-    online_update_interval : int
-        Interval (in number of transitions) between updates of the online network.
-    target_update_interval : int
-        Interval (in number total number of online updates) between updates of the target network.
-    learning_rate : float
+    batch_size: int, default=32
+        Batch size.
+    chunk_size: int, default=8
+        Length of sub-trajectories sampled from the replay buffer.
+    lambda_: float, default=0.5
+        Q(lambda) parameter.
+    target_update_parameter : int or float
+        If int: interval (in number total number of online updates) between updates of the target network.
+        If float: soft update coefficient
+    device: str
+        Torch device, see :func:`~rlberry.utils.torch.choose_device`
+    learning_rate : float, default = 1e-3
         Optimizer learning rate.
-    epsilon_init : float
-        Initial value of epsilon-greedy exploration.
-    epsilon_end : float
-        End value of epsilon-greedy exploration.
-    epsilon_steps : int
-        Number of steps over which annealing over epsilon takes place.
+    loss_function: {"l1", "l2", "smooth_l1"}, default: "l2"
+        Loss function used to compute Bellman error.
+    epsilon_init: float, default = 1.0
+        Initial epsilon value for epsilon-greedy exploration.
+    epsilon_final: float, default = 0.1
+        Final epsilon value for epsilon-greedy exploration.
+    epsilon_decay_interval : int
+        After :code:`epsilon_decay` timesteps, epsilon approaches :code:`epsilon_final`.
+    optimizer_type : {"ADAM", "RMS_PROP"}
+        Optimization algorithm.
+    q_net_constructor : Callable, str or None
+        Function/constructor that returns a torch module for the Q-network:
+        :code:`qnet = q_net_constructor(env, **kwargs)`.
+
+        Module (Q-network) requirements:
+
+        * Input shape = (batch_dim, chunk_size, obs_dims)
+
+        * Ouput shape = (batch_dim, chunk_size, number_of_actions)
+
+        Example: use `rlberry.agents.torch.utils.training.model_factory_from_env`,
+         and `q_net_kwargs`
+        parameter to modify the neural network::
+
+            model_configs = {
+                "type": "MultiLayerPerceptron",
+                "layer_sizes": (5, 5),
+                "reshape": False,
+            }
+
+            agent = DQNAgent(env,
+                q_net_constructor=model_factory_from_env,
+                q_net_kwargs=model_configs
+                )
+        If str then it should correspond to the full path to the constructor function,
+        e.g.::
+            agent = DQNAgent(env,
+                q_net_constructor='rlberry.agents.torch.utils.training.model_factory_from_env',
+                q_net_kwargs=model_configs
+                )
+
+        If None then it is set to MultiLayerPerceptron with 2 hidden layers
+        of size 64
+
+    q_net_kwargs : optional, dict
+        Parameters for q_net_constructor.
+    use_double_dqn : bool, default = False
+        If True, use Double DQN.
+    use_prioritized_replay : bool, default = False
+        If True, use Prioritized Experience Replay.
+    train_interval: int
+        Update the model every :code:`train_interval` steps.
+        If -1, train only at the end of the episodes.
+    gradient_steps: int
+        How many gradient steps to do at each update.
+        If -1, take the number of timesteps since last update.
     max_replay_size : int
         Maximum number of transitions in the replay buffer.
-    eval_interval : int
+    learning_starts : int
+        How many steps of the model to collect transitions for before learning starts
+    eval_interval : int, default = None
         Interval (in number of transitions) between agent evaluations in fit().
         If None, never evaluate.
-    max_episode_length : int
-        Maximum length of an episode. If None, episodes will only end if `done = True`
-        is returned by env.step().
-    lambda_ : float
-        Parameter for Peng's Q(lambda). If None, usual Q-learning is used.
-    net_constructor : callable
-        Constructor for Q network. If None, uses default MLP.
-    net_kwargs : dict
-        kwargs for network constructor (net_constructor).
-    max_gradient_norm : float, default: 100.0
-        Maximum gradient norm.
     """
 
-    name = "JaxDqnAgent"
+    name = "DQN"
 
     def __init__(
         self,
         env: types.Env,
         gamma: float = 0.99,
-        batch_size: int = 64,
+        batch_size: int = 32,
         chunk_size: int = 8,
-        online_update_interval: int = 1,
-        target_update_interval: int = 512,
-        learning_rate: float = 0.001,
+        lambda_: float = 0.5,
+        target_update_parameter: Union[int, float] = 0.005,
+        device: str = "cuda:best",
+        learning_rate: float = 1e-3,
         epsilon_init: float = 1.0,
-        epsilon_end: float = 0.05,
-        epsilon_steps: int = 5000,
-        max_replay_size: int = 100000,
+        epsilon_final: float = 0.1,
+        epsilon_decay_interval: int = 20_000,
+        loss_function: str = "l2",
+        optimizer_type: str = "ADAM",
+        q_net_constructor: Optional[Callable[..., torch.nn.Module]] = None,
+        q_net_kwargs: Optional[dict] = None,
+        use_double_dqn: bool = False,
+        use_prioritized_replay: bool = False,
+        train_interval: int = 10,
+        gradient_steps: int = -1,
+        max_replay_size: int = 200_000,
+        learning_starts: int = 5_000,
         eval_interval: Optional[int] = None,
-        max_episode_length: Optional[int] = None,
-        lambda_: Optional[float] = None,
-        net_constructor: Optional[Callable[..., hk.Module]] = None,
-        net_kwargs: Optional[Mapping[str, Any]] = None,
-        max_gradient_norm: float = 100.0,
-        **kwargs
+        **kwargs,
     ):
+        # For all parameters, define self.param = param
+        _, _, _, values = inspect.getargvalues(inspect.currentframe())
+        values.pop("self")
+        for arg, val in values.items():
+            setattr(self, arg, val)
+
         AgentWithSimplePolicy.__init__(self, env, **kwargs)
         env = self.env
-        self.rng_key = jax.random.PRNGKey(self.rng.integers(2**32).item())
+        assert isinstance(env.observation_space, spaces.Box)
+        assert isinstance(env.action_space, spaces.Discrete)
+
+        # DQN parameters
 
-        # checks
-        if not isinstance(self.env.observation_space, spaces.Box):
-            raise ValueError("DQN only implemented for Box observation spaces.")
-        if not isinstance(self.env.action_space, spaces.Discrete):
-            raise ValueError("DQN only implemented for Discrete action spaces.")
-
-        # params
-        self._gamma = gamma
-        self._batch_size = batch_size
-        self._chunk_size = chunk_size
-        self._online_update_interval = online_update_interval
-        self._target_update_interval = target_update_interval
-        self._max_replay_size = max_replay_size
+        # Online and target Q networks, torch device
+        self._device = choose_device(device)
+        if isinstance(q_net_constructor, str):
+            q_net_ctor = load(q_net_constructor)
+        elif q_net_constructor is None:
+            q_net_ctor = default_q_net_fn
+        else:
+            q_net_ctor = q_net_constructor
+        q_net_kwargs = q_net_kwargs or dict()
+        self._qnet_online = q_net_ctor(env, **q_net_kwargs).to(self._device)
+        self._qnet_target = q_net_ctor(env, **q_net_kwargs).to(self._device)
+
+        # Optimizer and loss
+        optimizer_kwargs = {"optimizer_type": optimizer_type, "lr": learning_rate}
+        self._optimizer = optimizer_factory(
+            self._qnet_online.parameters(), **optimizer_kwargs
+        )
+        self._loss_function = loss_function_factory(loss_function, reduction="none")
+
+        # Training params
+        self._train_interval = train_interval
+        self._gradient_steps = gradient_steps
+        self._learning_starts = learning_starts
+        self._learning_starts = learning_starts
         self._eval_interval = eval_interval
-        self._max_episode_length = max_episode_length or np.inf
-        self._lambda = lambda_
-        self._max_gradient_norm = max_gradient_norm
 
-        #
         # Setup replay buffer
-        #
-
-        # define specs
-        # TODO: generalize. Observation is taken from reset() because gym is
-        # mixing things up (returning double instead of float)
-        sample_obs = env.reset()
-        try:
-            obs_shape, obs_dtype = sample_obs.shape, sample_obs.dtype
-        except AttributeError:  # in case sample_obs has no .shape attribute
-            obs_shape, obs_dtype = (
-                env.observation_space.shape,
-                env.observation_space.dtype,
-            )
-        action_shape, action_dtype = env.action_space.shape, env.action_space.dtype
+        if hasattr(self.env, "_max_episode_steps"):
+            max_episode_steps = self.env._max_episode_steps
+        else:
+            max_episode_steps = np.inf
+        self._max_episode_steps = max_episode_steps
 
-        self._replay_buffer = ReplayBuffer(
-            self._batch_size,
-            self._chunk_size,
-            self._max_replay_size,
-        )
-        self._replay_buffer.setup_entry("actions", action_shape, action_dtype)
-        self._replay_buffer.setup_entry("observations", obs_shape, obs_dtype)
-        self._replay_buffer.setup_entry("next_observations", obs_shape, obs_dtype)
-        self._replay_buffer.setup_entry("rewards", (), np.float32)
-        self._replay_buffer.setup_entry("discounts", (), np.float32)
-        self._replay_buffer.build()
-
-        # initialize network and params
-        net_constructor = net_constructor or nets.MLPQNetwork
-        net_kwargs = net_kwargs or dict(
-            num_actions=self.env.action_space.n, hidden_sizes=(64, 64)
+        self._replay_buffer = replay.ReplayBuffer(
+            max_replay_size=max_replay_size,
+            rng=self.rng,
+            max_episode_steps=self._max_episode_steps,
+            enable_prioritized=use_prioritized_replay,
+        )
+        self._replay_buffer.setup_entry("observations", np.float32)
+        self._replay_buffer.setup_entry("next_observations", np.float32)
+        self._replay_buffer.setup_entry("actions", np.int32)
+        self._replay_buffer.setup_entry("rewards", np.float32)
+        self._replay_buffer.setup_entry("dones", bool)
+
+        # Counters
+        self._total_timesteps = 0
+        self._total_episodes = 0
+        self._total_updates = 0
+        self._timesteps_since_last_update = 0
+
+        # epsilon scheduling
+        self._epsilon_schedule = polynomial_schedule(
+            self.epsilon_init,
+            self.epsilon_final,
+            power=1.0,
+            transition_steps=self.epsilon_decay_interval,
+            transition_begin=0,
         )
-        net_ctor = functools.partial(net_constructor, **net_kwargs)
-        self._q_net = hk.without_apply_rng(hk.transform(lambda x: net_ctor()(x)))
 
-        self._dummy_obs = jnp.ones(self.env.observation_space.shape)
+    @property
+    def total_timesteps(self):
+        return self._total_timesteps
+
+    def _must_update(self, is_end_of_episode):
+        """Returns true if the model must be updated in the current timestep,
+        and the number of gradient steps to take"""
+        total_timesteps = self._total_timesteps
+        n_gradient_steps = self._gradient_steps
+
+        if total_timesteps < self._learning_starts:
+            return False, -1
+
+        if n_gradient_steps == -1:
+            n_gradient_steps = self._timesteps_since_last_update
+
+        run_update = False
+        if self._train_interval == -1:
+            run_update = is_end_of_episode
+        else:
+            run_update = total_timesteps % self._train_interval == 0
+        return run_update, n_gradient_steps
 
-        self.rng_key, subkey1 = jax.random.split(self.rng_key)
-        self.rng_key, subkey2 = jax.random.split(self.rng_key)
+    def _update(self, n_gradient_steps):
+        """Update networks."""
+        if self.use_prioritized_replay:
+            sampling_mode = "prioritized"
+        else:
+            sampling_mode = "uniform"
 
-        self._all_params = AllParams(
-            online=self._q_net.init(subkey1, self._dummy_obs),
-            target=self._q_net.init(subkey2, self._dummy_obs),
-        )
+        for _ in range(n_gradient_steps):
+            # Sample a batch
+            sampled = self._replay_buffer.sample(
+                self.batch_size, self.chunk_size, sampling_mode=sampling_mode
+            )
+            if not sampled:
+                return
 
-        # initialize optimizer and states
-        self._optimizer = optax.chain(
-            optax.clip_by_global_norm(self._max_gradient_norm),
-            optax.adam(learning_rate),
-        )
-        self._all_states = AllStates(
-            optimizer=self._optimizer.init(self._all_params.online),
-            learner_steps=jnp.array(0),
-            actor_steps=jnp.array(0),
-        )
+            # Update counters
+            self._timesteps_since_last_update = 0
+            self._total_updates += 1
+
+            batch = sampled.data
+            batch_info = sampled.info
+            assert batch["rewards"].shape == (self.batch_size, self.chunk_size)
+
+            # Compute targets
+            batch_observations = torch.FloatTensor(batch["observations"]).to(
+                self._device
+            )
+            batch_next_observations = torch.FloatTensor(batch["next_observations"]).to(
+                self._device
+            )
+            batch_actions = torch.LongTensor(batch["actions"]).to(self._device)
 
-        # epsilon decay
-        self._epsilon_schedule = optax.polynomial_schedule(
-            init_value=epsilon_init,
-            end_value=epsilon_end,
-            transition_steps=epsilon_steps,
-            transition_begin=0,
-            power=1.0,
-        )
+            target_q_values_tp1 = self._qnet_target(batch_next_observations).detach()
+            # Check if double DQN
+            if self.use_double_dqn:
+                online_q_values_tp1 = self._qnet_online(
+                    batch_next_observations
+                ).detach()
+                a_argmax = online_q_values_tp1.argmax(dim=-1).detach()
+            else:
+                a_argmax = target_q_values_tp1.argmax(dim=-1).detach()
+
+            v_tp1 = (
+                torch.gather(target_q_values_tp1, dim=-1, index=a_argmax[:, :, None])[
+                    :, :, 0
+                ]
+                .cpu()
+                .numpy()
+            )
 
-        # update functions (jit)
-        self.actor_step = jax.jit(self._actor_step)
-        self.learner_step = jax.jit(self._learner_step)
+            batch_lambda_returns = lambda_returns(
+                batch["rewards"],
+                self.gamma * (1.0 - np.array(batch["dones"], dtype=np.float32)),
+                v_tp1,
+                np.array(self.lambda_, dtype=np.float32),
+            )
+            targets = torch.tensor(batch_lambda_returns).to(self._device)
 
-    def policy(self, observation):
-        self.rng_key, subkey = jax.random.split(self.rng_key)
-        actor_out, _ = self.actor_step(
-            self._all_params,
-            self._all_states,
-            observation,
-            subkey,
-            evaluation=True,
-        )
-        action = actor_out.actions.item()
-        return action
+            # Compute loss
+            batch_q_values = self._qnet_online(batch_observations)
+            batch_values = torch.gather(
+                batch_q_values, dim=-1, index=batch_actions[:, :, None]
+            )[
+                :, :, 0
+            ]  # shape (batch, chunk)
+
+            assert batch_values.shape == targets.shape
+            per_element_loss = self._loss_function(batch_values, targets)
+            per_batch_element_loss = per_element_loss.mean(dim=1)
+            weights = torch.FloatTensor(batch_info["weights"]).to(self._device)
+            loss = torch.sum(per_batch_element_loss * weights) / torch.sum(weights)
+
+            self._optimizer.zero_grad()
+            loss.backward()
+            self._optimizer.step()
+
+            if self.writer:
+                self.writer.add_scalar(
+                    "losses/q_loss", loss.item(), self._total_updates
+                )
+
+            # update priorities
+            if self.use_prioritized_replay:
+                new_priorities = per_element_loss.abs().detach().cpu().numpy() + 1e-6
+                self._replay_buffer.update_priorities(
+                    batch_info["indices"], new_priorities
+                )
+
+            # target update
+            if self.target_update_parameter > 1:
+                if self._total_updates % self.target_update_parameter == 0:
+                    self._qnet_target.load_state_dict(self._qnet_online.state_dict())
+            else:
+                tau = self.target_update_parameter
+                for param, target_param in zip(
+                    self._qnet_online.parameters(), self._qnet_target.parameters()
+                ):
+                    target_param.data.copy_(
+                        tau * param.data + (1 - tau) * target_param.data
+                    )
 
     def fit(self, budget: int, **kwargs):
         """
-        Train DQN agent.
+        Train the agent using the provided environment.
 
         Parameters
         ----------
         budget: int
-            Number of timesteps to train the agent.
+            Number of timesteps to train the agent for.
+            One step = one transition in the environment.
         """
         del kwargs
         timesteps_counter = 0
         episode_rewards = 0.0
         episode_timesteps = 0
         observation = self.env.reset()
-        with self._replay_buffer.get_writer() as buffer_writer:
-            while timesteps_counter < budget:
-                self.rng_key, subkey = jax.random.split(self.rng_key)
-                actor_out, self._all_states = self.actor_step(
-                    self._all_params,
-                    self._all_states,
-                    observation,
-                    subkey,
-                    evaluation=False,
-                )
-                action = actor_out.actions.item()
-                next_obs, reward, done, _ = self.env.step(action)
-
-                # check max episode length
-                done = done and (episode_timesteps < self._max_episode_length)
+        while timesteps_counter < budget:
+            if self.total_timesteps < self._learning_starts:
+                action = self.env.action_space.sample()
+            else:
+                self._timesteps_since_last_update += 1
+                action = self._policy(observation, evaluation=False)
+            next_obs, reward, done, _ = self.env.step(action)
+
+            # store data
+            episode_rewards += reward
+            self._replay_buffer.append(
+                {
+                    "observations": observation,
+                    "actions": action,
+                    "rewards": reward,
+                    "dones": done,
+                    "next_observations": next_obs,
+                }
+            )
 
-                # store data
-                episode_rewards += reward
-                buffer_writer.append(
-                    {
-                        "actions": action,
-                        "observations": observation,
-                        "rewards": np.array(reward, dtype=np.float32),
-                        "discounts": np.array(
-                            self._gamma * (1.0 - done), dtype=np.float32
-                        ),
-                        "next_observations": next_obs,
-                    }
+            # counters and next obs
+            self._total_timesteps += 1
+            timesteps_counter += 1
+            episode_timesteps += 1
+            observation = next_obs
+
+            # update
+            run_update, n_gradient_steps = self._must_update(done)
+            if run_update:
+                self._update(n_gradient_steps)
+
+            # eval
+            total_timesteps = self._total_timesteps
+            if (
+                self._eval_interval is not None
+                and total_timesteps % self._eval_interval == 0
+            ):
+                eval_rewards = self.eval(
+                    eval_horizon=self._max_episode_steps, gamma=1.0
                 )
-
-                # counters and next obs
-                timesteps_counter += 1
-                episode_timesteps += 1
-                observation = next_obs
-
-                # update
-                total_timesteps = self._all_states.actor_steps.item()
-                if total_timesteps % self._online_update_interval == 0:
-                    sample = self._replay_buffer.sample()
-                    if sample:
-                        batch = sample.data
-                        self._all_params, self._all_states, info = self.learner_step(
-                            self._all_params, self._all_states, batch
-                        )
-                        if self.writer:
-                            self.writer.add_scalar(
-                                "q_loss", info["loss"].item(), total_timesteps
-                            )
-                            self.writer.add_scalar(
-                                "learner_steps",
-                                self._all_states.learner_steps.item(),
-                                total_timesteps,
-                            )
-
-                # eval
-                if (
-                    self._eval_interval is not None
-                    and total_timesteps % self._eval_interval == 0
-                ):
-                    eval_rewards = self.eval(
-                        eval_horizon=self._max_episode_length,
-                        n_simimulations=2,
-                        gamma=1.0,
-                    )
+                if self.writer:
+                    buffer_size = len(self._replay_buffer)
                     self.writer.add_scalar(
                         "eval_rewards", eval_rewards, total_timesteps
                     )
+                    self.writer.add_scalar("buffer_size", buffer_size, total_timesteps)
 
-                # check if episode ended
-                if done:
-                    if self.writer:
-                        self.writer.add_scalar(
-                            "episode_rewards", episode_rewards, total_timesteps
-                        )
-                    buffer_writer.end_episode()
-                    episode_rewards = 0.0
-                    episode_timesteps = 0
-                    observation = self.env.reset()
-
-    def _loss(self, all_params, batch):
-        obs_tm1 = batch["observations"]
-        a_tm1 = batch["actions"]
-        r_t = batch["rewards"]
-        discount_t = batch["discounts"]
-        obs_t = batch["next_observations"]
-
-        if self._lambda is None:
-            # remove time dim (batch has shape [batch, chunk_size, ...])
-            a_tm1 = a_tm1.flatten()
-            r_t = r_t.flatten()
-            discount_t = discount_t.flatten()
-            obs_tm1 = jnp.reshape(obs_tm1, (-1, obs_tm1.shape[-1]))
-            obs_t = jnp.reshape(obs_t, (-1, obs_t.shape[-1]))
-
-        q_tm1 = self._q_net.apply(all_params.online, obs_tm1)
-        q_t_val = self._q_net.apply(all_params.target, obs_t)
-        q_t_select = self._q_net.apply(all_params.online, obs_t)
-
-        if self._lambda is None:
-            batched_loss = jax.vmap(rlax.double_q_learning)
-            td_error = batched_loss(q_tm1, a_tm1, r_t, discount_t, q_t_val, q_t_select)
+            # check if episode ended
+            if done:
+                self._total_episodes += 1
+                self._replay_buffer.end_episode()
+                if self.writer:
+                    self.writer.add_scalar(
+                        "episode_rewards", episode_rewards, total_timesteps
+                    )
+                    self.writer.add_scalar(
+                        "total_episodes", self._total_episodes, total_timesteps
+                    )
+                episode_rewards = 0.0
+                episode_timesteps = 0
+                observation = self.env.reset()
+
+    def _policy(self, observation, evaluation=False):
+        epsilon = self._epsilon_schedule(self.total_timesteps)
+        if (not evaluation) and self.rng.uniform() < epsilon:
+            if self.writer:
+                self.writer.add_scalar("epsilon", epsilon, self.total_timesteps)
+            return self.env.action_space.sample()
         else:
-            batched_loss = jax.vmap(rlax.q_lambda)
-            batch_lambda = self._lambda * jnp.ones(r_t.shape)
-            td_error = batched_loss(
-                q_tm1, a_tm1, r_t, discount_t, q_t_val, batch_lambda
-            )
-
-        loss = jnp.mean(rlax.l2_loss(td_error))
-
-        info = dict(loss=loss)
-        return loss, info
-
-    def _actor_step(self, all_params, all_states, observation, rng_key, evaluation):
-        obs = jnp.expand_dims(observation, 0)  # dummy batch
-        q_val = self._q_net.apply(all_params.online, obs)[0]  # remove batch
-        epsilon = self._epsilon_schedule(all_states.actor_steps)
-        train_action = rlax.epsilon_greedy(epsilon).sample(rng_key, q_val)
-        eval_action = rlax.greedy().sample(rng_key, q_val)
-        action = jax.lax.select(evaluation, eval_action, train_action)
-        return (
-            ActorOutput(actions=action, q_values=q_val),
-            AllStates(
-                optimizer=all_states.optimizer,
-                learner_steps=all_states.learner_steps,
-                actor_steps=all_states.actor_steps + 1,
-            ),
-        )
-
-    def _learner_step(self, all_params, all_states, batch):
-        target_params = rlax.periodic_update(
-            all_params.online,
-            all_params.target,
-            all_states.learner_steps,
-            self._target_update_interval,
-        )
-        grad, info = jax.grad(self._loss, has_aux=True)(all_params, batch)
-        updates, optimizer_state = self._optimizer.update(
-            grad.online, all_states.optimizer
-        )
-        online_params = optax.apply_updates(all_params.online, updates)
-        return (
-            AllParams(online=online_params, target=target_params),
-            AllStates(
-                optimizer=optimizer_state,
-                learner_steps=all_states.learner_steps + 1,
-                actor_steps=all_states.actor_steps,
-            ),
-            info,
-        )
-
-    #
-    # Custom save/load methods.
-    #
-    def save(self, filename):
-        filename = Path(filename).with_suffix(".pickle")
-        filename.parent.mkdir(parents=True, exist_ok=True)
-
-        writer = None
-        if dill.pickles(self.writer):
-            writer = self.writer
-
-        agent_data = dict(
-            rng_key=self.rng_key,
-            params=self._all_params,
-            states=self._all_states,
-            writer=writer,
-        )
-        with filename.open("wb") as ff:
-            dill.dump(agent_data, ff)
-
-        return filename
+            with torch.no_grad():
+                observation = (
+                    torch.FloatTensor(observation).to(self._device).unsqueeze(0)
+                )
+                qvals_tensor = self._qnet_online(observation)[0]
+                action = qvals_tensor.argmax().item()
+                return action
 
-    @classmethod
-    def load(cls, filename, **kwargs):
-        filename = Path(filename).with_suffix(".pickle")
-        agent = cls(**kwargs)
-        with filename.open("rb") as ff:
-            agent_data = dill.load(ff)
-        agent.key = agent_data["rng_key"]
-        agent._all_params = agent_data["params"]
-        agent._all_states = agent_data["states"]
-        writer = agent_data["writer"]
-        if writer:
-            agent._writer = writer
-        return agent
-
-    #
-    # For hyperparameter optimization
-    #
-    @classmethod
-    def sample_parameters(cls, trial):
-        learning_rate = trial.suggest_loguniform("learning_rate", 1e-5, 1e-1)
-        gamma = trial.suggest_uniform("gamma", 0.95, 0.99)
-        lambda_ = trial.suggest_categorical("lambda_", [0.1, 0.5, 0.9, None])
-        return dict(learning_rate=learning_rate, gamma=gamma, lambda_=lambda_)
+    def policy(self, observation):
+        return self._policy(observation, evaluation=True)
```

### Comparing `rlberry-0.4.0/rlberry/agents/experimental/tests/test_actor_critic.py` & `rlberry-0.4.1/rlberry/agents/experimental/tests/test_sac.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,53 +1,47 @@
-from rlberry.agents.experimental.torch import AVECPPOAgent
+from rlberry.agents.experimental.torch import SACAgent
+
 from rlberry.envs.benchmarks.ball_exploration.ball2d import get_benchmark_env
 from rlberry.exploration_tools.discrete_counter import DiscreteCounter
 
 
-def test_avec_ppo_agent():
+def test_sac_agent():
     env = get_benchmark_env(level=1)
     n_episodes = 5
-    horizon = 30
 
-    #
     def uncertainty_estimator_fn(observation_space, action_space):
         counter = DiscreteCounter(observation_space, action_space, n_bins_obs=20)
         return counter
 
-    agent = AVECPPOAgent(
+    agent = SACAgent(
         env,
-        horizon=horizon,
         gamma=0.99,
         learning_rate=0.001,
-        eps_clip=0.2,
         k_epochs=4,
-        batch_size=1,
         use_bonus=True,
         uncertainty_estimator_kwargs=dict(
             uncertainty_estimator_fn=uncertainty_estimator_fn, bonus_scale_factor=1.0
         ),
+        device="cpu",
     )
-    agent.fit(budget=n_episodes // 2)
+    agent.fit(budget=n_episodes)
     agent.policy(env.observation_space.sample())
 
 
-def test_avec_ppo_agent_partial_fit():
+def test_sac_agent_partial_fit():
     env = get_benchmark_env(level=1)
     n_episodes = 10
-    horizon = 30
 
-    agent = AVECPPOAgent(
+    agent = SACAgent(
         env,
-        horizon=horizon,
         gamma=0.99,
         learning_rate=0.001,
-        eps_clip=0.2,
         k_epochs=4,
-        batch_size=1,
         use_bonus=False,
+        device="cpu",
     )
 
     agent.fit(budget=n_episodes // 2)
     agent.policy(env.observation_space.sample())
     assert agent.episode == 5
     agent.fit(budget=n_episodes // 2)
     assert agent.episode == 10
```

### Comparing `rlberry-0.4.0/rlberry/agents/experimental/tests/test_sac.py` & `rlberry-0.4.1/rlberry/agents/torch/tests/test_reinforce.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,48 +1,49 @@
-from rlberry.agents.experimental.torch import SACAgent
-
+from rlberry.agents.torch import REINFORCEAgent
 from rlberry.envs.benchmarks.ball_exploration.ball2d import get_benchmark_env
 from rlberry.exploration_tools.discrete_counter import DiscreteCounter
+from rlberry.wrappers.uncertainty_estimator_wrapper import UncertaintyEstimatorWrapper
 
 
-def test_sac_agent():
-    env = get_benchmark_env(level=1)
-    n_episodes = 5
+def test_reinforce_agent():
+    _env = get_benchmark_env(level=1)
+    n_episodes = 50
+    horizon = 30
 
+    #
     def uncertainty_estimator_fn(observation_space, action_space):
         counter = DiscreteCounter(observation_space, action_space, n_bins_obs=20)
         return counter
 
-    agent = SACAgent(
+    env = UncertaintyEstimatorWrapper(
+        _env, uncertainty_estimator_fn, bonus_scale_factor=1.0
+    )
+    #
+    agent = REINFORCEAgent(
         env,
+        horizon=horizon,
         gamma=0.99,
         learning_rate=0.001,
-        k_epochs=4,
-        use_bonus=True,
-        uncertainty_estimator_kwargs=dict(
-            uncertainty_estimator_fn=uncertainty_estimator_fn, bonus_scale_factor=1.0
-        ),
-        device="cpu",
+        use_bonus_if_available=True,
     )
     agent.fit(budget=n_episodes)
     agent.policy(env.observation_space.sample())
 
 
-def test_sac_agent_partial_fit():
+def test_reinforce_agent_partial_fit():
     env = get_benchmark_env(level=1)
     n_episodes = 10
+    horizon = 30
 
-    agent = SACAgent(
+    agent = REINFORCEAgent(
         env,
+        horizon=horizon,
         gamma=0.99,
         learning_rate=0.001,
-        k_epochs=4,
-        use_bonus=False,
-        device="cpu",
+        use_bonus_if_available=False,
     )
-
     agent.fit(budget=n_episodes // 2)
     agent.policy(env.observation_space.sample())
     assert agent.episode == 5
     agent.fit(budget=n_episodes // 2)
     assert agent.episode == 10
     agent.policy(env.observation_space.sample())
```

### Comparing `rlberry-0.4.0/rlberry/agents/experimental/torch/avec/avec_ppo.py` & `rlberry-0.4.1/rlberry/agents/torch/a2c/a2c.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,360 +1,335 @@
 import torch
-
 import torch.nn as nn
-import inspect
 
 import gym.spaces as spaces
+import numpy as np
 from rlberry.agents import AgentWithSimplePolicy
-from rlberry.agents.utils.memories import Memory
+from rlberry.agents.utils.replay import ReplayBuffer
 from rlberry.agents.torch.utils.training import optimizer_factory
 from rlberry.agents.torch.utils.models import default_policy_net_fn
 from rlberry.agents.torch.utils.models import default_value_net_fn
 from rlberry.utils.torch import choose_device
-from rlberry.wrappers.uncertainty_estimator_wrapper import UncertaintyEstimatorWrapper
+from rlberry.utils.factory import load
+from typing import Optional
 
 import rlberry
 
 logger = rlberry.logger
 
 
-class AVECPPOAgent(AgentWithSimplePolicy):
+class A2CAgent(AgentWithSimplePolicy):
     """
-    AVEC uses a modification of the training objective for the critic in
-    actor-critic algorithms to better approximate the value function (critic).
-    The new state-value function approximation learns the *relative* value of
-    the states rather than their *absolute* value as in conventional
-    actor-critic. This modification is:
-    - well-motivated by recent studies [1,2];
-    - theoretically sound;
-    - intuitively supported by the need to improve the approximation error
-    of the critic.
-
-    The application of Actor with Variance Estimated Critic (AVEC) to
-    state-of-the-art policy gradient methods produces considerable
-    gains in performance (on average +26% for SAC and +40% for PPO)
-    over the standard actor-critic training.
+    Advantage Actor Critic Agent.
+
+    A2C, or Advantage Actor Critic, is a synchronous version of the A3C policy
+    gradient method. As an alternative to the asynchronous implementation of
+    A3C, A2C is a synchronous, deterministic implementation that waits for each
+    actor to finish its segment of experience before updating, averaging over
+    all of the actors. This more effectively uses GPUs due to larger batch sizes.
 
     Parameters
     ----------
     env : Model
-        model with continuous (Box) state space and discrete actions
+        Online model with continuous (Box) state space and discrete actions
     batch_size : int
-        Number of episodes to wait before updating the policy.
-    horizon : int
-        Horizon of the objective function. If None and gamma<1,
-        set to 1/(1-gamma).
+        Number of timesteps to wait before updating the policy.
     gamma : double
-        Discount factor in [0, 1]. If gamma is 1.0, the problem is set
-        to be finite-horizon.
+        Discount factor in [0, 1].
     entr_coef : double
         Entropy coefficient.
-    vf_coef : double
-        Value function loss coefficient.
     learning_rate : double
         Learning rate.
     optimizer_type: str
         Type of optimizer. 'ADAM' by defaut.
-    eps_clip : double
-        PPO clipping range (epsilon).
-    k_epochs : int
-        Number of epochs per update.
     policy_net_fn : function(env, **kwargs)
         Function that returns an instance of a policy network (pytorch).
         If None, a default net is used.
     value_net_fn : function(env, **kwargs)
         Function that returns an instance of a value network (pytorch).
         If None, a default net is used.
     policy_net_kwargs : dict
         kwargs for policy_net_fn
     value_net_kwargs : dict
         kwargs for value_net_fn
-    use_bonus : bool, default = False
-        If true, compute an 'exploration_bonus' and add it to the reward.
-        See also UncertaintyEstimatorWrapper.
-    uncertainty_estimator_kwargs : dict
-        Arguments for the UncertaintyEstimatorWrapper
     device : str
         Device to put the tensors on
+    eval_interval : int, default = None
+        Interval (in number of transitions) between agent evaluations in fit().
+        If None, never evaluate.
 
     References
     ----------
-    Flet-Berliac, Y., Ouhamma, R., Maillard, O. A., & Preux, P. (2021).
-    "Is Standard Deviation the New Standard? Revisiting the Critic in Deep
-    Policy Gradients."
-    In International Conference on Learning Representations.
-
-    [1] Ilyas, A., Engstrom, L., Santurkar, S., Tsipras, D., Janoos, F.,
-    Rudolph, L. & Madry, A. (2020).
-    "A closer look at deep policy gradients."
-    In International Conference on Learning Representations.
-
-    [2] Tucker, G., Bhupatiraju, S., Gu, S., Turner, R., Ghahramani, Z. &
-    Levine, S. (2018).
-    "The mirage of action-dependent baselines in reinforcement learning."
-    In International Conference on Machine Learning, pp. 5015–5024.
+    Mnih, V., Badia, A.P., Mirza, M., Graves, A., Lillicrap, T., Harley, T.,
+    Silver, D. & Kavukcuoglu, K. (2016).
+    "Asynchronous methods for deep reinforcement learning."
+    In International Conference on Machine Learning (pp. 1928-1937).
     """
 
-    name = "AVECPPO"
+    name = "A2C"
 
     def __init__(
         self,
         env,
-        batch_size=8,
-        horizon=256,
+        batch_size=256,
         gamma=0.99,
         entr_coef=0.01,
-        vf_coef=0.0,
-        avec_coef=1.0,
-        learning_rate=0.0003,
+        learning_rate=0.01,
         optimizer_type="ADAM",
-        eps_clip=0.2,
-        k_epochs=10,
         policy_net_fn=None,
         value_net_fn=None,
         policy_net_kwargs=None,
         value_net_kwargs=None,
-        use_bonus=False,
-        uncertainty_estimator_kwargs=None,
         device="cuda:best",
+        eval_interval: Optional[int] = None,
         **kwargs
     ):
-        # For all parameters, define self.param = param
-        _, _, _, values = inspect.getargvalues(inspect.currentframe())
-        values.pop("self")
-        for arg, val in values.items():
-            setattr(self, arg, val)
-
         AgentWithSimplePolicy.__init__(self, env, **kwargs)
 
-        self.use_bonus = use_bonus
-        if self.use_bonus:
-            self.env = UncertaintyEstimatorWrapper(
-                self.env, **uncertainty_estimator_kwargs
-            )
-
+        self.batch_size = batch_size
+        self.gamma = gamma
+        self.entr_coef = entr_coef
+        self.learning_rate = learning_rate
         self.device = choose_device(device)
+        self.eval_interval = eval_interval
 
         self.policy_net_kwargs = policy_net_kwargs or {}
         self.value_net_kwargs = value_net_kwargs or {}
 
-        self.state_dim = self.env.observation_space.shape[0]
-        self.action_dim = self.env.action_space.n
-
-        #
-        self.policy_net_fn = policy_net_fn or default_policy_net_fn
-        self.value_net_fn = value_net_fn or default_value_net_fn
+        if isinstance(policy_net_fn, str):
+            self.policy_net_fn = load(policy_net_fn)
+        elif policy_net_fn is None:
+            self.policy_net_fn = default_policy_net_fn
+        else:
+            self.policy_net_fn = policy_net_fn
+
+        if isinstance(value_net_fn, str):
+            self.value_net_fn = load(value_net_fn)
+        elif value_net_fn is None:
+            self.value_net_fn = default_value_net_fn
+        else:
+            self.value_net_fn = value_net_fn
 
         self.optimizer_kwargs = {"optimizer_type": optimizer_type, "lr": learning_rate}
+        self.optimizer_type = optimizer_type
 
         # check environment
         assert isinstance(self.env.observation_space, spaces.Box)
-        assert isinstance(self.env.action_space, spaces.Discrete)
 
-        self.cat_policy = None  # categorical policy function
+        # get horizon
+        if hasattr(self.env, "_max_episode_steps"):
+            max_episode_steps = self.env._max_episode_steps
+        else:
+            max_episode_steps = np.inf
+        self._max_episode_steps = max_episode_steps
+
+        self._policy = None  # categorical policy function
 
         # initialize
         self.reset()
 
-    def reset(self, **kwargs):
-        self.cat_policy = self.policy_net_fn(self.env, **self.policy_net_kwargs).to(
+    def reset(self):
+        self._policy = self.policy_net_fn(self.env, **self.policy_net_kwargs).to(
             self.device
         )
-        self.policy_optimizer = optimizer_factory(
-            self.cat_policy.parameters(), **self.optimizer_kwargs
+        self._policy_optimizer = optimizer_factory(
+            self._policy.parameters(), **self.optimizer_kwargs
         )
 
         self.value_net = self.value_net_fn(self.env, **self.value_net_kwargs).to(
             self.device
         )
+
         self.value_optimizer = optimizer_factory(
             self.value_net.parameters(), **self.optimizer_kwargs
         )
 
-        self.cat_policy_old = self.policy_net_fn(self.env, **self.policy_net_kwargs).to(
+        self._policy_old = self.policy_net_fn(self.env, **self.policy_net_kwargs).to(
             self.device
         )
-        self.cat_policy_old.load_state_dict(self.cat_policy.state_dict())
+        self._policy_old.load_state_dict(self._policy.state_dict())
 
         self.MseLoss = nn.MSELoss()
 
-        self.memory = Memory()
+        self.memory = ReplayBuffer(max_replay_size=self.batch_size, rng=self.rng)
+        self.memory.setup_entry("states", dtype=np.float32)
+        if self._policy.ctns_actions:
+            self.memory.setup_entry("actions", dtype=np.float32)
+        else:
+            self.memory.setup_entry("actions", dtype=int)
+        self.memory.setup_entry("rewards", dtype=np.float32)
+        self.memory.setup_entry("dones", dtype=bool)
 
-        self.episode = 0
+        self.total_timesteps = 0
+        self.total_episodes = 0
 
     def policy(self, observation):
         state = observation
-        assert self.cat_policy is not None
+        assert self._policy is not None
         state = torch.from_numpy(state).float().to(self.device)
-        action_dist = self.cat_policy_old(state)
-        action = action_dist.sample().item()
-
+        action_dist = self._policy_old(state)
+        if self._policy.ctns_actions:
+            action = action_dist.sample().numpy()
+        else:
+            action = action_dist.sample().item()
         return action
 
     def fit(self, budget: int, **kwargs):
         """
         Train the agent using the provided environment.
 
         Parameters
         ----------
         budget: int
-            number of episodes. Each episode runs for self.horizon unless it
-            enconters a terminal state in which case it stops early.
+            Number of timesteps to train the agent for.
+            One step = one transition in the environment.
         """
-
         del kwargs
-        n_episodes_to_run = budget
-        count = 0
-        while count < n_episodes_to_run:
-            self._run_episode()
-            count += 1
-
-    def _select_action(self, state):
-        state = torch.from_numpy(state).float().to(self.device)
-        action_dist = self.cat_policy_old(state)
-        action = action_dist.sample()
-        action_logprob = action_dist.log_prob(action)
-
-        self.memory.states.append(state)
-        self.memory.actions.append(action)
-        self.memory.logprobs.append(action_logprob)
-
-        return action.item()
-
-    def _run_episode(self):
-        # interact for H steps
-        episode_rewards = 0
-        state = self.env.reset()
-        for _ in range(self.horizon):
-            # running policy_old
-            action = self._select_action(state)
-            next_state, reward, done, info = self.env.step(action)
-
-            # check whether to use bonus
-            bonus = 0.0
-            if self.use_bonus:
-                if info is not None and "exploration_bonus" in info:
-                    bonus = info["exploration_bonus"]
-
-            # save in batch
-            self.memory.rewards.append(reward + bonus)  # add bonus here
-            self.memory.is_terminals.append(done)
+        timesteps_counter = 0
+        episode_rewards = 0.0
+        episode_timesteps = 0
+        observation = self.env.reset()
+        while timesteps_counter < budget:
+            action = self._select_action(observation)
+            next_obs, reward, done, _ = self.env.step(action)
+            # if self._policy.ctns_actions:
+            #     action = torch.from_numpy(action).float().to(self.device)
+            # store data
             episode_rewards += reward
+            self.memory.append(
+                {
+                    "states": observation,
+                    "actions": action,
+                    "rewards": reward,
+                    "dones": done,
+                }
+            )
 
-            if done:
-                break
-
-            # update state
-            state = next_state
-
-        # update
-        self.episode += 1
-
-        #
-        if self.writer is not None:
-            self.writer.add_scalar("episode_rewards", episode_rewards, self.episode)
+            # counters and next obs
+            self.total_timesteps += 1
+            timesteps_counter += 1
+            episode_timesteps += 1
+            observation = next_obs
+
+            # update
+            if self.total_timesteps % self.batch_size == 0:
+                self._update()
+
+            # eval
+            total_timesteps = self.total_timesteps
+            if (
+                self.eval_interval is not None
+                and total_timesteps % self.eval_interval == 0
+            ):
+                eval_rewards = self.eval(
+                    eval_horizon=self._max_episode_steps, gamma=1.0
+                )
+                if self.writer:
+                    memory_size = len(self.memory)
+                    self.writer.add_scalar(
+                        "eval_rewards", eval_rewards, total_timesteps
+                    )
+                    self.writer.add_scalar("memory_size", memory_size, total_timesteps)
 
-        #
-        if self.episode % self.batch_size == 0:
-            self._update()
-            self.memory.clear_memory()
+            # check if episode ended
+            if done:
+                self.total_episodes += 1
+                self.memory.end_episode()
+                if self.writer:
+                    self.writer.add_scalar(
+                        "episode_rewards", episode_rewards, total_timesteps
+                    )
+                    self.writer.add_scalar(
+                        "total_episodes", self.total_episodes, total_timesteps
+                    )
+                episode_rewards = 0.0
+                episode_timesteps = 0
+                observation = self.env.reset()
 
-        return episode_rewards
+    def _select_action(self, state):
+        state = torch.from_numpy(state).float().to(self.device)
+        action_dist = self._policy_old(state)
+        action = action_dist.sample()
+        if self._policy.ctns_actions:
+            action = action.numpy()
+        else:
+            action = action.item()
+        return action
 
     def _update(self):
         # monte carlo estimate of rewards
         rewards = []
         discounted_reward = 0
+
+        memory_data = self.memory.data
+        memory_states = memory_data["states"]
+        memory_actions = memory_data["actions"]
+        memory_rewards = memory_data["rewards"]
+        memory_dones = memory_data["dones"]
+
         for reward, is_terminal in zip(
-            reversed(self.memory.rewards), reversed(self.memory.is_terminals)
+            reversed(memory_rewards), reversed(memory_dones)
         ):
             if is_terminal:
                 discounted_reward = 0
             discounted_reward = reward + (self.gamma * discounted_reward)
             rewards.insert(0, discounted_reward)
 
-        # normalizing the rewards
-        rewards = torch.tensor(rewards).to(self.device).float()
-        rewards = (rewards - rewards.mean()) / (rewards.std() + 1e-5)
+        # convert to tensor
+        rewards = torch.FloatTensor(rewards).to(self.device)
+        memory_states_tensors = [
+            torch.tensor(states).to(self.device).float() for states in memory_states
+        ]
+        memory_actions_tensors = [
+            torch.tensor(actions).to(self.device) for actions in memory_actions
+        ]
 
         # convert list to tensor
-        old_states = torch.stack(self.memory.states).to(self.device).detach()
-        old_actions = torch.stack(self.memory.actions).to(self.device).detach()
-        old_logprobs = torch.stack(self.memory.logprobs).to(self.device).detach()
-
-        # optimize policy for K epochs
-        for _ in range(self.k_epochs):
-            # evaluate old actions and values
-            action_dist = self.cat_policy(old_states)
-            logprobs = action_dist.log_prob(old_actions)
-            state_values = torch.squeeze(self.value_net(old_states))
-            dist_entropy = action_dist.entropy()
-
-            # find ratio (pi_theta / pi_theta__old)
-            ratios = torch.exp(logprobs - old_logprobs.detach())
-
-            # normalize the advantages
-            advantages = rewards - state_values.detach()
-            advantages = (advantages - advantages.mean()) / (advantages.std() + 1e-8)
-            # find surrogate loss
-            surr1 = ratios * advantages
-            surr2 = (
-                torch.clamp(ratios, 1 - self.eps_clip, 1 + self.eps_clip) * advantages
-            )
-            loss = (
-                -torch.min(surr1, surr2)
-                + self.avec_coef * self._avec_loss(state_values, rewards)
-                + self.vf_coef * self.MseLoss(state_values, rewards)
-                - self.entr_coef * dist_entropy
-            )
+        old_states = torch.stack(memory_states_tensors).to(self.device).detach()
+        old_actions = torch.stack(memory_actions_tensors).to(self.device).detach()
 
-            # take gradient step
-            self.policy_optimizer.zero_grad()
-            self.value_optimizer.zero_grad()
+        # evaluate old actions and values
+        action_dist = self._policy(old_states)
+        logprobs = action_dist.log_prob(old_actions)
+        state_values = torch.squeeze(self.value_net(old_states))
+        dist_entropy = action_dist.entropy()
+
+        # normalize the advantages
+        advantages = rewards - state_values.detach()
+        advantages = (advantages - advantages.mean()) / (advantages.std() + 1e-8)
+        # find pg loss
+        pg_loss = -logprobs * advantages
+        loss = (
+            pg_loss
+            + 0.5 * self.MseLoss(state_values, rewards)
+            - self.entr_coef * dist_entropy
+        )
 
-            loss.mean().backward()
+        # take gradient step
+        self._policy_optimizer.zero_grad()
+        self.value_optimizer.zero_grad()
 
-            self.policy_optimizer.step()
-            self.value_optimizer.step()
+        loss.mean().backward()
 
-        # copy new weights into old policy
-        self.cat_policy_old.load_state_dict(self.cat_policy.state_dict())
+        self._policy_optimizer.step()
+        self.value_optimizer.step()
 
-    def _avec_loss(self, y_pred, y_true):
-        """
-        Computes the objective function used in AVEC for the learning
-        of the value function:
-        the residual variance between the state-values and the
-        empirical returns.
-
-        Returns Var[y-ypred]
-        :param y_pred: (np.ndarray) the prediction
-        :param y_true: (np.ndarray) the expected value
-        :return: (float) residual variance of ypred and y
-        """
-        assert y_true.ndim == 1 and y_pred.ndim == 1
-
-        return torch.var(y_true - y_pred)
+        # copy new weights into old policy
+        self._policy_old.load_state_dict(self._policy.state_dict())
 
     #
     # For hyperparameter optimization
     #
     @classmethod
     def sample_parameters(cls, trial):
         batch_size = trial.suggest_categorical("batch_size", [1, 4, 8, 16, 32])
         gamma = trial.suggest_categorical("gamma", [0.9, 0.95, 0.99])
-        learning_rate = trial.suggest_loguniform("learning_rate", 1e-5, 1)
-
-        entr_coef = trial.suggest_loguniform("entr_coef", 1e-8, 0.1)
-
-        eps_clip = trial.suggest_categorical("eps_clip", [0.1, 0.2, 0.3])
+        learning_rate = trial.suggest_float("learning_rate", 1e-5, 1, log=True)
 
-        k_epochs = trial.suggest_categorical("k_epochs", [1, 5, 10, 20])
+        entr_coef = trial.suggest_float("entr_coef", 1e-8, 0.1, log=True)
 
         return {
             "batch_size": batch_size,
             "gamma": gamma,
             "learning_rate": learning_rate,
             "entr_coef": entr_coef,
-            "eps_clip": eps_clip,
-            "k_epochs": k_epochs,
         }
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `rlberry-0.4.0/rlberry/agents/experimental/torch/sac/sac.py` & `rlberry-0.4.1/rlberry/agents/experimental/torch/sac/sac.py`

 * *Files 1% similar despite different names*

```diff
@@ -92,15 +92,14 @@
         value_net_kwargs=None,
         twinq_net_kwargs=None,
         use_bonus=False,
         uncertainty_estimator_kwargs=None,
         device="cuda:best",
         **kwargs
     ):
-
         AgentWithSimplePolicy.__init__(self, env, **kwargs)
 
         self.use_bonus = use_bonus
         if self.use_bonus:
             self.env = UncertaintyEstimatorWrapper(
                 self.env, **uncertainty_estimator_kwargs
             )
@@ -360,16 +359,17 @@
     #
     # For hyperparameter optimization
     #
     @classmethod
     def sample_parameters(cls, trial):
         batch_size = trial.suggest_categorical("batch_size", [1, 4, 8, 16, 32])
         gamma = trial.suggest_categorical("gamma", [0.9, 0.95, 0.99])
-        learning_rate = trial.suggest_loguniform("learning_rate", 1e-5, 1)
-        entr_coef = trial.suggest_loguniform("entr_coef", 1e-8, 0.1)
+        learning_rate = trial.suggest_float("learning_rate", 1e-5, 1, log=True)
+        entr_coef = trial.suggest_float("entr_coef", 1e-8, 0.1, log=True)
+
         k_epochs = trial.suggest_categorical("k_epochs", [1, 5, 10, 20])
 
         return {
             "batch_size": batch_size,
             "gamma": gamma,
             "learning_rate": learning_rate,
             "entr_coef": entr_coef,
```

### Comparing `rlberry-0.4.0/rlberry/agents/experimental/torch/sac/utils.py` & `rlberry-0.4.1/rlberry/agents/experimental/torch/sac/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,15 +42,14 @@
 
     batch_target_val = rewards + (1 - dones) * gamma * val_next_states
     return batch_target_val
 
 
 @torch.no_grad()
 def get_vref(env, batch, twinq_net, policy_net, ent_alpha: float, device="cpu"):
-
     assert isinstance(twinq_net, tuple)
     assert isinstance(env.action_space, spaces.Discrete)
     num_actions = env.action_space.n
 
     states, _, _, _, _, _ = batch
     q1, q2 = twinq_net
     # references for the critic network
```

### Comparing `rlberry-0.4.0/rlberry/agents/features/feature_map.py` & `rlberry-0.4.1/rlberry/agents/features/feature_map.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.4.0/rlberry/agents/kernel_based/common.py` & `rlberry-0.4.1/rlberry/agents/kernel_based/common.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.4.0/rlberry/agents/kernel_based/kernels.py` & `rlberry-0.4.1/rlberry/agents/kernel_based/kernels.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.4.0/rlberry/agents/kernel_based/rs_kernel_ucbvi.py` & `rlberry-0.4.1/rlberry/agents/kernel_based/rs_kernel_ucbvi.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.4.0/rlberry/agents/kernel_based/rs_ucbvi.py` & `rlberry-0.4.1/rlberry/agents/kernel_based/rs_ucbvi.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.4.0/rlberry/agents/linear/lsvi_ucb.py` & `rlberry-0.4.1/rlberry/agents/linear/lsvi_ucb.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.4.0/rlberry/agents/mbqvi/mbqvi.py` & `rlberry-0.4.1/rlberry/agents/mbqvi/mbqvi.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.4.0/rlberry/agents/optql/optql.py` & `rlberry-0.4.1/rlberry/agents/optql/optql.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.4.0/rlberry/agents/psrl/psrl.py` & `rlberry-0.4.1/rlberry/agents/psrl/psrl.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.4.0/rlberry/agents/rlsvi/rlsvi.py` & `rlberry-0.4.1/rlberry/agents/rlsvi/rlsvi.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.4.0/rlberry/agents/stable_baselines/stable_baselines.py` & `rlberry-0.4.1/rlberry/agents/stable_baselines/stable_baselines.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.4.0/rlberry/agents/tests/test_dynprog.py` & `rlberry-0.4.1/rlberry/agents/tests/test_dynprog.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.4.0/rlberry/agents/tests/test_kernel_based.py` & `rlberry-0.4.1/rlberry/agents/tests/test_kernel_based.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.4.0/rlberry/agents/tests/test_lsvi_ucb.py` & `rlberry-0.4.1/rlberry/agents/tests/test_lsvi_ucb.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.4.0/rlberry/agents/tests/test_mbqvi.py` & `rlberry-0.4.1/rlberry/agents/tests/test_mbqvi.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.4.0/rlberry/agents/tests/test_psrl.py` & `rlberry-0.4.1/rlberry/agents/tests/test_psrl.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.4.0/rlberry/agents/tests/test_replay.py` & `rlberry-0.4.1/rlberry/agents/tests/test_replay.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.4.0/rlberry/agents/tests/test_stable_baselines.py` & `rlberry-0.4.1/rlberry/agents/tests/test_stable_baselines.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.4.0/rlberry/agents/tests/test_ucbvi.py` & `rlberry-0.4.1/rlberry/agents/tests/test_ucbvi.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.4.0/rlberry/agents/torch/dqn/dqn.py` & `rlberry-0.4.1/rlberry/agents/torch/dqn/mdqn.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,30 @@
 import inspect
-from typing import Callable, Optional, Union
 
-from gym import spaces
 import numpy as np
 import torch
-
+from gym import spaces
 from rlberry import types
 from rlberry.agents import AgentWithSimplePolicy
 from rlberry.agents.torch.utils.training import (
     loss_function_factory,
     model_factory,
     optimizer_factory,
     size_model_config,
 )
-from rlberry.agents.torch.dqn.dqn_utils import polynomial_schedule, lambda_returns
+from rlberry.agents.torch.dqn.dqn_utils import (
+    lambda_returns,
+    polynomial_schedule,
+    stable_scaled_log_softmax,
+    stable_softmax,
+)
 from rlberry.agents.utils import replay
 from rlberry.utils.torch import choose_device
 from rlberry.utils.factory import load
+from typing import Callable, Optional, Union
 
 
 import rlberry
 
 logger = rlberry.logger
 
 
@@ -34,41 +38,51 @@
         "layer_sizes": (64, 64),
         "reshape": False,
     }
     model_config = size_model_config(env, **model_config)
     return model_factory(**model_config)
 
 
-class DQNAgent(AgentWithSimplePolicy):
-    """DQN Agent based on PyTorch.
+class MunchausenDQNAgent(AgentWithSimplePolicy):
+    """Munchausen DQN Agent based on PyTorch.
 
     Notes
     -----
-    Uses Q(lambda) for computing targets by default. To recover
-    the standard DQN, set :code:`lambda_ = 0.0` and :code:`chunk_size = 1`.
+    Uses Munchausen trick for DQN for computing targets by default.
+    Compared to DQN, the scaled log-policy was added to the immediate
+    reward. Slightly modifying DQN in that way provides an agent that
+    is competitive with distributional methods on Atari games, without
+    making use of distributional RL, n-step returns or prioritized replay.
+    See more: https://arxiv.org/pdf/2007.14430.pdf
 
     Parameters
     ----------
     env: :class:`~rlberry.types.Env`
         Environment, can be a tuple (constructor, kwargs)
     gamma: float, default = 0.99
         Discount factor.
     batch_size: int, default=32
         Batch size.
     chunk_size: int, default=8
         Length of sub-trajectories sampled from the replay buffer.
     lambda_: float, default=0.5
         Q(lambda) parameter.
+    tau: float, default=0.03
+        softmax temperature for the policy
+    alpha: float, default=0.9
+        Munchausen coefficient
     target_update_parameter : int or float
         If int: interval (in number total number of online updates) between updates of the target network.
         If float: soft update coefficient
     device: str
         Torch device, see :func:`~rlberry.utils.torch.choose_device`
     learning_rate : float, default = 1e-3
         Optimizer learning rate.
+    clip_value_min: float, default = -1,
+        minimum value for munchausen term
     loss_function: {"l1", "l2", "smooth_l1"}, default: "l2"
         Loss function used to compute Bellman error.
     epsilon_init: float, default = 1.0
         Initial epsilon value for epsilon-greedy exploration.
     epsilon_final: float, default = 0.1
         Final epsilon value for epsilon-greedy exploration.
     epsilon_decay_interval : int
@@ -91,32 +105,30 @@
 
             model_configs = {
                 "type": "MultiLayerPerceptron",
                 "layer_sizes": (5, 5),
                 "reshape": False,
             }
 
-            agent = DQNAgent(env,
+            agent = MunchausenDQNAgent(env,
                 q_net_constructor=model_factory_from_env,
                 q_net_kwargs=model_configs
                 )
         If str then it should correspond to the full path to the constructor function,
         e.g.::
-            agent = DQNAgent(env,
+            agent = MunchausenDQNAgent(env,
                 q_net_constructor='rlberry.agents.torch.utils.training.model_factory_from_env',
                 q_net_kwargs=model_configs
                 )
 
         If None then it is set to MultiLayerPerceptron with 2 hidden layers
         of size 64
 
     q_net_kwargs : optional, dict
         Parameters for q_net_constructor.
-    use_double_dqn : bool, default = False
-        If True, use Double DQN.
     use_prioritized_replay : bool, default = False
         If True, use Prioritized Experience Replay.
     train_interval: int
         Update the model every :code:`train_interval` steps.
         If -1, train only at the end of the episodes.
     gradient_steps: int
         How many gradient steps to do at each update.
@@ -126,38 +138,41 @@
     learning_starts : int
         How many steps of the model to collect transitions for before learning starts
     eval_interval : int, default = None
         Interval (in number of transitions) between agent evaluations in fit().
         If None, never evaluate.
     """
 
-    name = "DQN"
+    name = "Munchausen DQN"
 
     def __init__(
         self,
         env: types.Env,
         gamma: float = 0.99,
         batch_size: int = 32,
         chunk_size: int = 8,
         lambda_: float = 0.5,
+        tau: float = 0.03,
+        alpha: float = 0.9,
         target_update_parameter: Union[int, float] = 0.005,
+        # tardet_update_freq: int = 8000,
         device: str = "cuda:best",
-        learning_rate: float = 1e-3,
+        learning_rate: float = 5e-5,
+        clip_value_min: float = -1.0,
         epsilon_init: float = 1.0,
         epsilon_final: float = 0.1,
         epsilon_decay_interval: int = 20_000,
         loss_function: str = "l2",
         optimizer_type: str = "ADAM",
         q_net_constructor: Optional[Callable[..., torch.nn.Module]] = None,
         q_net_kwargs: Optional[dict] = None,
-        use_double_dqn: bool = False,
         use_prioritized_replay: bool = False,
-        train_interval: int = 10,
+        train_interval: int = 4,
         gradient_steps: int = -1,
-        max_replay_size: int = 200_000,
+        max_replay_size: int = 1_000_000,
         learning_starts: int = 5_000,
         eval_interval: Optional[int] = None,
         **kwargs,
     ):
         # For all parameters, define self.param = param
         _, _, _, values = inspect.getargvalues(inspect.currentframe())
         values.pop("self")
@@ -165,15 +180,15 @@
             setattr(self, arg, val)
 
         AgentWithSimplePolicy.__init__(self, env, **kwargs)
         env = self.env
         assert isinstance(env.observation_space, spaces.Box)
         assert isinstance(env.action_space, spaces.Discrete)
 
-        # DQN parameters
+        # M-DQN parameters
 
         # Online and target Q networks, torch device
         self._device = choose_device(device)
         if isinstance(q_net_constructor, str):
             q_net_ctor = load(q_net_constructor)
         elif q_net_constructor is None:
             q_net_ctor = default_q_net_fn
@@ -273,48 +288,56 @@
             self._timesteps_since_last_update = 0
             self._total_updates += 1
 
             batch = sampled.data
             batch_info = sampled.info
             assert batch["rewards"].shape == (self.batch_size, self.chunk_size)
 
-            # Compute targets
+            # Get batched tensors
             batch_observations = torch.FloatTensor(batch["observations"]).to(
                 self._device
             )
+            batch_rewards = torch.FloatTensor(batch["rewards"]).to(self._device)
             batch_next_observations = torch.FloatTensor(batch["next_observations"]).to(
                 self._device
             )
             batch_actions = torch.LongTensor(batch["actions"]).to(self._device)
+            batch_dones = torch.LongTensor(batch["dones"]).to(self._device)
 
+            # Get target Q estimates
             target_q_values_tp1 = self._qnet_target(batch_next_observations).detach()
-            # Check if double DQN
-            if self.use_double_dqn:
-                online_q_values_tp1 = self._qnet_online(
-                    batch_next_observations
-                ).detach()
-                a_argmax = online_q_values_tp1.argmax(dim=-1).detach()
-            else:
-                a_argmax = target_q_values_tp1.argmax(dim=-1).detach()
+            target_q_values = self._qnet_target(batch_observations).detach()
 
-            v_tp1 = (
-                torch.gather(target_q_values_tp1, dim=-1, index=a_argmax[:, :, None])[
-                    :, :, 0
-                ]
-                .cpu()
-                .numpy()
+            # Compute softmax policies for the current and next step
+            log_pi = stable_scaled_log_softmax(target_q_values, self.tau, -1)
+            log_pi_tp1 = stable_scaled_log_softmax(target_q_values_tp1, self.tau, -1)
+            pi_tp1 = stable_softmax(target_q_values_tp1, self.tau, -1)
+
+            # Compute the "next step" part of the target
+            target_v_tp1 = (
+                torch.sum((target_q_values_tp1 - log_pi_tp1) * pi_tp1, -1).cpu().numpy()
             )
 
+            # Compute the Munchausen term
+            munchausen_term = torch.gather(
+                log_pi, dim=-1, index=batch_actions[:, :, None]
+            )[:, :, 0]
+            clipped_munchausen_term = torch.clip(
+                munchausen_term, self.clip_value_min, 0
+            )
+            final_munchausen_term = self.alpha * clipped_munchausen_term
+
+            # Compute the final target
             batch_lambda_returns = lambda_returns(
-                batch["rewards"],
+                (batch_rewards + final_munchausen_term).cpu().numpy(),
                 self.gamma * (1.0 - np.array(batch["dones"], dtype=np.float32)),
-                v_tp1,
+                target_v_tp1,
                 np.array(self.lambda_, dtype=np.float32),
             )
-            targets = torch.tensor(batch_lambda_returns).to(self._device)
+            targets = torch.tensor(batch_lambda_returns, device=self._device)
 
             # Compute loss
             batch_q_values = self._qnet_online(batch_observations)
             batch_values = torch.gather(
                 batch_q_values, dim=-1, index=batch_actions[:, :, None]
             )[
                 :, :, 0
@@ -339,14 +362,15 @@
             if self.use_prioritized_replay:
                 new_priorities = per_element_loss.abs().detach().cpu().numpy() + 1e-6
                 self._replay_buffer.update_priorities(
                     batch_info["indices"], new_priorities
                 )
 
             # target update
+
             if self.target_update_parameter > 1:
                 if self._total_updates % self.target_update_parameter == 0:
                     self._qnet_target.load_state_dict(self._qnet_online.state_dict())
             else:
                 tau = self.target_update_parameter
                 for param, target_param in zip(
                     self._qnet_online.parameters(), self._qnet_target.parameters()
```

### Comparing `rlberry-0.4.0/rlberry/agents/torch/dqn/dqn_utils.py` & `rlberry-0.4.1/rlberry/agents/torch/dqn/dqn_utils.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.4.0/rlberry/agents/torch/reinforce/reinforce.py` & `rlberry-0.4.1/rlberry/agents/torch/reinforce/reinforce.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import torch
 import inspect
+import numpy as np
 
 import gym.spaces as spaces
 from rlberry.agents import AgentWithSimplePolicy
 from rlberry.agents.utils.memories import Memory
 from rlberry.agents.torch.utils.training import optimizer_factory
 from rlberry.agents.torch.utils.models import default_policy_net_fn
 from rlberry.utils.torch import choose_device
@@ -68,15 +69,14 @@
         optimizer_type="ADAM",
         policy_net_fn=None,
         policy_net_kwargs=None,
         use_bonus_if_available=False,
         device="cuda:best",
         **kwargs
     ):
-
         # For all parameters, define self.param = param
         _, _, _, values = inspect.getargvalues(inspect.currentframe())
         values.pop("self")
         for arg, val in values.items():
             setattr(self, arg, val)
 
         AgentWithSimplePolicy.__init__(self, env, **kwargs)
@@ -194,15 +194,15 @@
         ):
             if is_terminal:
                 discounted_reward = 0
             discounted_reward = reward + (self.gamma * discounted_reward)
             rewards.insert(0, discounted_reward)
 
         # convert list to tensor
-        states = torch.FloatTensor(self.memory.states).to(self.device)
+        states = torch.FloatTensor(np.array(self.memory.states)).to(self.device)
         actions = torch.LongTensor(self.memory.actions).to(self.device)
         rewards = torch.FloatTensor(rewards).to(self.device)
         if self.normalize:
             rewards = self._normalize(rewards)
 
         # evaluate logprobs
         action_dist = self.policy_net(states)
@@ -222,17 +222,17 @@
     #
     # For hyperparameter optimization
     #
     @classmethod
     def sample_parameters(cls, trial):
         batch_size = trial.suggest_categorical("batch_size", [1, 4, 8, 16, 32])
         gamma = trial.suggest_categorical("gamma", [0.9, 0.95, 0.99])
-        learning_rate = trial.suggest_loguniform("learning_rate", 1e-5, 1)
+        learning_rate = trial.suggest_float("learning_rate", 1e-5, 1, log=True)
 
-        entr_coef = trial.suggest_loguniform("entr_coef", 1e-8, 0.1)
+        entr_coef = trial.suggest_float("entr_coef", 1e-8, 0.1, log=True)
 
         return {
             "batch_size": batch_size,
             "gamma": gamma,
             "learning_rate": learning_rate,
             "entr_coef": entr_coef,
         }
```

### Comparing `rlberry-0.4.0/rlberry/agents/torch/tests/test_a2c.py` & `rlberry-0.4.1/rlberry/agents/torch/tests/test_a2c.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,16 +2,15 @@
 from rlberry.agents.torch import A2CAgent
 from rlberry.manager import AgentManager, evaluate_agents
 from rlberry.envs.benchmarks.ball_exploration import PBall2D
 from gym import make
 
 
 def test_a2c():
-
-    env = "CartPole-v0"
+    env = "CartPole-v1"
     mdp = make(env)
     env_ctor = Wrapper
     env_kwargs = dict(env=mdp)
 
     a2crlberry_stats = AgentManager(
         A2CAgent,
         (env_ctor, env_kwargs),
@@ -81,15 +80,15 @@
 
     a2crlberry_stats.fit()
 
     output = evaluate_agents([a2crlberry_stats], n_simulations=2, plot=False)
     a2crlberry_stats.clear_output_dir()
 
     # test also non default
-    env = "CartPole-v0"
+    env = "CartPole-v1"
     mdp = make(env)
     env_ctor = Wrapper
     env_kwargs = dict(env=mdp)
 
     a2crlberry_stats = AgentManager(
         A2CAgent,
         (env_ctor, env_kwargs),
```

### Comparing `rlberry-0.4.0/rlberry/agents/torch/tests/test_dqn.py` & `rlberry-0.4.1/rlberry/agents/torch/tests/test_dqn.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from rlberry.agents.torch.utils.training import model_factory
 
 
 @pytest.mark.parametrize(
     "use_double_dqn, use_prioritized_replay", [(False, False), (True, True)]
 )
 def test_dqn_agent(use_double_dqn, use_prioritized_replay):
-    env = gym_make("CartPole-v0")
+    env = gym_make("CartPole-v1")
     agent = DQNAgent(
         env,
         learning_starts=5,
         eval_interval=75,
         train_interval=2,
         gradient_steps=-1,
         use_double_dqn=use_double_dqn,
```

### Comparing `rlberry-0.4.0/rlberry/agents/torch/tests/test_mdqn.py` & `rlberry-0.4.1/rlberry/agents/torch/tests/test_mdqn.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from rlberry.envs import gym_make
 from rlberry.agents.torch.dqn import MunchausenDQNAgent
 from rlberry.agents.torch.utils.training import model_factory
 
 
 @pytest.mark.parametrize("use_prioritized_replay", [(False), (True)])
 def test_mdqn_agent(use_prioritized_replay):
-    env = gym_make("CartPole-v0")
+    env = gym_make("CartPole-v1")
     agent = MunchausenDQNAgent(
         env,
         learning_starts=5,
         batch_size=5,
         eval_interval=2,
         train_interval=2,
         gradient_steps=-1,
```

### Comparing `rlberry-0.4.0/rlberry/agents/torch/tests/test_ppo.py` & `rlberry-0.4.1/rlberry/agents/torch/tests/test_ppo.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,35 +3,38 @@
 
 
 # env = (gym_make, dict(id="Acrobot-v1"))
 # # env = gym_make(id="Acrobot-v1")
 # ppo = PPOAgent(env)
 # ppo.fit(4096)
 
+import pytest
 from rlberry.envs import Wrapper
 from rlberry.agents.torch import PPOAgent
 from rlberry.manager import AgentManager, evaluate_agents
 from rlberry.envs.benchmarks.ball_exploration import PBall2D
 from gym import make
 from rlberry.agents.torch.utils.training import model_factory_from_env
+import sys
 
 
+@pytest.mark.timeout(300)
+@pytest.mark.xfail(sys.platform == "win32", reason="bug with windows???")
 def test_ppo():
-
-    env = "CartPole-v0"
+    env = "CartPole-v1"
     mdp = make(env)
     env_ctor = Wrapper
     env_kwargs = dict(env=mdp)
 
     pporlberry_stats = AgentManager(
         PPOAgent,
         (env_ctor, env_kwargs),
-        fit_budget=int(100),
+        fit_budget=int(132),
         eval_kwargs=dict(eval_horizon=2),
-        init_kwargs=dict(batch_size=24, n_steps=96),
+        init_kwargs=dict(batch_size=24, n_steps=96, device="cpu"),
         n_fit=1,
         agent_name="PPO_rlberry_" + env,
     )
 
     pporlberry_stats.fit()
 
     output = evaluate_agents([pporlberry_stats], n_simulations=2, plot=False)
@@ -41,17 +44,17 @@
     mdp = make(env)
     env_ctor = Wrapper
     env_kwargs = dict(env=mdp)
 
     pporlberry_stats = AgentManager(
         PPOAgent,
         (env_ctor, env_kwargs),
-        fit_budget=int(100),
+        fit_budget=int(132),
         eval_kwargs=dict(eval_horizon=2),
-        init_kwargs=dict(batch_size=24, n_steps=96),
+        init_kwargs=dict(batch_size=24, n_steps=96, device="cpu"),
         n_fit=1,
         agent_name="PPO_rlberry_" + env,
     )
 
     pporlberry_stats.fit()
 
     output = evaluate_agents([pporlberry_stats], n_simulations=2, plot=False)
@@ -61,59 +64,57 @@
     mdp = make(env)
     env_ctor = Wrapper
     env_kwargs = dict(env=mdp)
 
     pporlberry_stats = AgentManager(
         PPOAgent,
         (env_ctor, env_kwargs),
-        fit_budget=int(100),
+        fit_budget=int(132),
         eval_kwargs=dict(eval_horizon=2),
-        init_kwargs=dict(batch_size=24, n_steps=96),
+        init_kwargs=dict(batch_size=24, n_steps=96, device="cpu"),
         n_fit=1,
         agent_name="PPO_rlberry_" + env,
     )
 
     pporlberry_stats.fit()
 
     output = evaluate_agents([pporlberry_stats], n_simulations=2, plot=False)
     pporlberry_stats.clear_output_dir()
 
     env_ctor = PBall2D
     env_kwargs = dict()
-
     pporlberry_stats = AgentManager(
         PPOAgent,
         (env_ctor, env_kwargs),
-        fit_budget=int(100),
+        fit_budget=int(132),
         eval_kwargs=dict(eval_horizon=2),
-        init_kwargs=dict(batch_size=24, n_steps=96),
+        init_kwargs=dict(batch_size=24, n_steps=96, device="cpu"),
         n_fit=1,
         agent_name="PPO_rlberry_" + "PBall2D",
     )
 
     pporlberry_stats.fit()
 
     output = evaluate_agents([pporlberry_stats], n_simulations=2, plot=False)
     pporlberry_stats.clear_output_dir()
 
     # test also non default
-    env = "CartPole-v0"
+    env = "CartPole-v1"
     mdp = make(env)
     env_ctor = Wrapper
     env_kwargs = dict(env=mdp)
 
     pporlberry_stats = AgentManager(
         PPOAgent,
         (env_ctor, env_kwargs),
-        fit_budget=int(100),
+        fit_budget=int(132),
         eval_kwargs=dict(eval_horizon=2),
         init_kwargs=dict(
             batch_size=24,
             n_steps=96,
-            use_gae=False,
             policy_net_fn="rlberry.agents.torch.utils.training.model_factory_from_env",
             policy_net_kwargs=dict(
                 type="MultiLayerPerceptron",
                 layer_sizes=(256,),
                 reshape=False,
                 is_policy=True,
             ),
@@ -131,20 +132,19 @@
         agent_name="PPO_rlberry_" + env,
     )
     pporlberry_stats.fit()
 
     pporlberry_stats = AgentManager(
         PPOAgent,
         (env_ctor, env_kwargs),
-        fit_budget=int(100),
+        fit_budget=int(132),
         eval_kwargs=dict(eval_horizon=2),
         init_kwargs=dict(
             batch_size=24,
             n_steps=96,
-            use_gae=False,
             policy_net_fn=model_factory_from_env,
             policy_net_kwargs=dict(
                 type="MultiLayerPerceptron",
                 layer_sizes=(256,),
                 reshape=False,
                 is_policy=True,
             ),
@@ -164,36 +164,37 @@
     pporlberry_stats.fit()
 
     output = evaluate_agents([pporlberry_stats], n_simulations=2, plot=False)
     pporlberry_stats.clear_output_dir()
 
     env_ctor = PBall2D
     env_kwargs = dict()
-
     pporlberry_stats = AgentManager(
         PPOAgent,
         (env_ctor, env_kwargs),
-        fit_budget=int(100),
+        fit_budget=int(132),
         eval_kwargs=dict(eval_horizon=2),
-        init_kwargs=dict(batch_size=24, n_steps=96, normalize_rewards=True),
+        init_kwargs=dict(batch_size=24, n_steps=96, device="cpu"),
         n_fit=1,
         agent_name="PPO_rlberry_" + "PBall2D",
     )
 
     pporlberry_stats.fit()
 
     output = evaluate_agents([pporlberry_stats], n_simulations=2, plot=False)
     pporlberry_stats.clear_output_dir()
 
     pporlberry_stats = AgentManager(
         PPOAgent,
         (env_ctor, env_kwargs),
-        fit_budget=int(100),
+        fit_budget=int(132),
         eval_kwargs=dict(eval_horizon=2),
-        init_kwargs=dict(batch_size=24, n_steps=96, normalize_advantages=True),
+        init_kwargs=dict(
+            batch_size=24, n_steps=96, normalize_advantages=True, device="cpu"
+        ),
         n_fit=1,
         agent_name="PPO_rlberry_" + "PBall2D",
     )
 
     pporlberry_stats.fit()
 
     output = evaluate_agents([pporlberry_stats], n_simulations=2, plot=False)
```

### Comparing `rlberry-0.4.0/rlberry/agents/torch/tests/test_torch_training.py` & `rlberry-0.4.1/rlberry/agents/torch/tests/test_torch_training.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.4.0/rlberry/agents/torch/utils/models.py` & `rlberry-0.4.1/rlberry/agents/torch/utils/models.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 #
 # Simple MLP and CNN models
 #
+from functools import partial
 
-
+from gym import spaces
+from gym.vector.sync_vector_env import SyncVectorEnv
+import numpy as np
 import torch
 import torch.nn as nn
-from torch.distributions import Categorical, MultivariateNormal
-from gym import spaces
+import torch.nn.functional as F
+from torch.distributions import Categorical, Normal
 
-#
-# Utility functions
-#
 from rlberry.agents.torch.utils.training import model_factory, activation_factory
 
 
 def default_twinq_net_fn(env):
     """
     Returns a default Twinq network
     """
@@ -46,27 +46,30 @@
     q2 = model_factory(**model_config)
 
     return (q1, q2)
 
 
 def default_policy_net_fn(env):
     """
-    Returns a default value network.
+    Returns a default policy network.
     """
+    if type(env) is SyncVectorEnv:
+        env = env.envs[0]
+
     if isinstance(env.observation_space, spaces.Box):
         obs_shape = env.observation_space.shape
     elif isinstance(env.observation_space, spaces.Tuple):
         obs_shape = env.observation_space.spaces[0].shape
     else:
         raise ValueError(
             "Incompatible observation space: {}".format(env.observation_space)
         )
 
     if len(obs_shape) == 3:
-        if obs_shape[0] < obs_shape[1] and obs_shape[0] < obs_shape[1]:
+        if obs_shape[0] < obs_shape[1] and obs_shape[0] < obs_shape[2]:
             # Assume CHW observation space
             model_config = {
                 "type": "ConvolutionalNetwork",
                 "is_policy": True,
                 "in_channels": int(obs_shape[0]),
                 "in_height": int(obs_shape[1]),
                 "in_width": int(obs_shape[2]),
@@ -115,14 +118,18 @@
     return model_factory(**model_config)
 
 
 def default_value_net_fn(env):
     """
     Returns a default value network.
     """
+
+    if type(env) is SyncVectorEnv:
+        env = env.envs[0]
+
     if isinstance(env.observation_space, spaces.Box):
         obs_shape = env.observation_space.shape
     elif isinstance(env.observation_space, spaces.Tuple):
         obs_shape = env.observation_space.spaces[0].shape
     else:
         raise ValueError(
             "Incompatible observation space: {}".format(env.observation_space)
@@ -174,29 +181,32 @@
 class BaseModule(torch.nn.Module):
     """
     Base torch.nn.Module implementing basic features:
         - initialization factory
         - normalization parameters
     """
 
-    def __init__(self, activation_type="RELU", reset_type="XAVIER"):
+    def __init__(self, activation_type="RELU", reset_type="xavier"):
         super().__init__()
         self.activation = activation_factory(activation_type)
         self.reset_type = reset_type
 
-    def _init_weights(self, m):
+    def _init_weights(self, m, param=None, put_bias_to_zero=False):
         if hasattr(m, "weight"):
-            if self.reset_type == "XAVIER":
+            if self.reset_type == "xavier":
                 torch.nn.init.xavier_uniform_(m.weight.data)
-            elif self.reset_type == "ZEROS":
+            elif self.reset_type == "zeros":
                 torch.nn.init.constant_(m.weight.data, 0.0)
+            elif self.reset_type == "orthogonal":
+                torch.nn.init.orthogonal_(m.weight.data, gain=param)
             else:
                 raise ValueError("Unknown reset type")
-        if hasattr(m, "bias") and m.bias is not None:
-            torch.nn.init.constant_(m.bias.data, 0.0)
+        if put_bias_to_zero:
+            if hasattr(m, "bias") and m.bias is not None:
+                torch.nn.init.constant_(m.bias.data, 0.0)
 
     def reset(self):
         self.apply(self._init_weights)
 
 
 class Table(torch.nn.Module):
     """Torch module for a policy for discrete state-action spaces.
@@ -237,59 +247,97 @@
         If True, input tensors are reshaped to (batch_size, dim)
     out_size: int, optional
         Output size. If None, the output size is given by the last
         element of layer_sizes.
     activation: {"RELU", "TANH", "ELU"}
         Activation function.
     is_policy: bool, default=False
-        If true, the :meth:`forward` method returns a categorical
-        distribution corresponding to the softmax of the output.
+        If true, the :meth:`forward` method returns a distribution over the
+        output.
+    ctns_actions: bool, default=False
+        If true, the :meth:`forward` method returns a normal distribution
+        corresponding to the output. Otherwise, a categorical distribution
+        is returned.
+    std0: float, default=1.0
+        Initial standard deviation for the normal distribution. Only used
+        if ctns_actions and is_policy are True.
+    reset_type: {"xavier", "orthogonal", "zeros"}, default="orthogonal"
+        Type of weight initialization.
+    pred_init_scale: float, default="auto"
+        Scale of the initial weights of the output layer. If "auto", the
+        scale is set to 0.01 for policy networks and 1.0 otherwise.
     """
 
     def __init__(
         self,
         in_size=None,
         layer_sizes=None,
-        reshape=True,
+        reshape=False,
         out_size=None,
         activation="RELU",
         is_policy=False,
         ctns_actions=False,
+        std0=1.0,
+        reset_type="orthogonal",
+        pred_init_scale="auto",
         **kwargs
     ):
-        super().__init__(**kwargs)
+        super().__init__(reset_type=reset_type, **kwargs)
+
         self.reshape = reshape
         self.layer_sizes = layer_sizes or [64, 64]
         self.layer_sizes = list(self.layer_sizes)
         self.out_size = out_size
         self.activation = activation_factory(activation)
         self.is_policy = is_policy
         self.ctns_actions = ctns_actions
-        self.softmax = nn.Softmax(dim=-1)
+        self.std0 = std0
+
+        # Set pred_init_scale
+        if pred_init_scale == "auto":
+            self.pred_init_scale = 0.01 if is_policy else 1.0
+        else:
+            self.pred_init_scale = pred_init_scale
+
+        # Instantiate parameters
         sizes = [in_size] + self.layer_sizes
-        layers_list = [nn.Linear(sizes[i], sizes[i + 1]) for i in range(len(sizes) - 1)]
-        self.layers = nn.ModuleList(layers_list)
+        self.layers = nn.ModuleList(
+            [nn.Linear(sizes[i], sizes[i + 1]) for i in range(len(sizes) - 1)]
+        )
         if out_size:
+            if ctns_actions:
+                self.logstd = nn.Parameter(np.log(std0) * torch.ones(out_size))
             self.predict = nn.Linear(sizes[-1], out_size)
 
+        # Initialize parameters
+        self.reset()
+
+    def reset(self):
+        self.apply(partial(self._init_weights, param=np.log(2)))
+        if self.out_size:
+            if self.ctns_actions:
+                self.logstd.data.fill_(np.log(self.std0))
+                self.apply(
+                    partial(self._init_weights, param=np.log(2), put_bias_to_zero=True)
+                )
+            self._init_weights(self.predict, param=self.pred_init_scale)
+
     def forward(self, x):
         if self.reshape:
             x = x.reshape(x.shape[0], -1)  # We expect a batch of vectors
         for layer in self.layers:
             x = self.activation(layer(x.float()))
         if self.out_size:
             x = self.predict(x)
         if self.is_policy:
             if self.ctns_actions:
-                std = 2
-                dist = MultivariateNormal(
-                    x, covariance_matrix=torch.eye(self.out_size) * std
-                )
+                std = torch.exp(self.logstd.expand_as(x))
+                dist = Normal(x, std)
             else:
-                action_probs = self.softmax(x)
+                action_probs = F.softmax(x, dim=-1)
                 dist = Categorical(action_probs)
             return dist
         return x
 
     def action_scores(self, x):
         if self.is_policy:
             if self.reshape:
@@ -357,14 +405,16 @@
 
     Expects inputs of shape BCHW, where
     B = batch size;
     C = number of channels;
     H = height;
     W = width.
 
+    For the CNN forward, if the tensor has more than 4 dimensions (not BCHW), it keeps the 3 last dimension as CHW and merge all first ones into 1 (Batch). Go through the CNN + MLP, then split the first dimension as before.
+
     Parameters
     ----------
     activation: {"RELU", "TANH", "ELU"}
         Activation function.
     in_channels: int
         Number of input channels C
     in_height: int
@@ -394,48 +444,73 @@
         super().__init__()
         self.activation = activation_factory(activation)
         self.conv1 = nn.Conv2d(in_channels, 16, kernel_size=2, stride=2)
         self.conv2 = nn.Conv2d(16, 32, kernel_size=2, stride=2)
         self.conv3 = nn.Conv2d(32, 64, kernel_size=2, stride=2)
 
         # MLP Head
-        # Number of Linear input connections depends on output of conv2d layers
-        # and therefore the input image size, so compute it.
-        def conv2d_size_out(size, kernel_size=2, stride=2):
-            return (size - (kernel_size - 1) - 1) // stride + 1
-
-        convw = conv2d_size_out(conv2d_size_out(conv2d_size_out(in_width)))
-        convh = conv2d_size_out(conv2d_size_out(conv2d_size_out(in_height)))
-        assert convh > 0 and convw > 0
         self.head_mlp_kwargs = head_mlp_kwargs or {}
-        self.head_mlp_kwargs["in_size"] = convw * convh * 64
+        self.head_mlp_kwargs["in_size"] = self._get_conv_out_size(
+            [in_channels, in_height, in_width]
+        )  # Number of Linear input connections depends on output of conv layers
         self.head_mlp_kwargs["out_size"] = out_size
         self.head_mlp_kwargs["is_policy"] = is_policy
         self.head = model_factory(**self.head_mlp_kwargs)
 
         self.is_policy = is_policy
         self.transpose_obs = transpose_obs
 
+    def _get_conv_out_size(self, shape):
+        """
+        Computes the output dimensions of the convolution network.
+        Shape : dimension of the input of the CNN
+        """
+        conv_result = self.activation((self.conv1(torch.zeros(1, *shape))))
+        conv_result = self.activation((self.conv2(conv_result)))
+        conv_result = self.activation((self.conv3(conv_result)))
+        return int(np.prod(conv_result.size()))
+
     def convolutions(self, x):
         x = x.float()
+        # if there is no batch (CHW), add one dimension to specify batch of 1 (and get format BCHW)
         if len(x.shape) == 3:
             x = x.unsqueeze(0)
         if self.transpose_obs:
             x = torch.transpose(x, -1, -3)
         x = self.activation((self.conv1(x)))
         x = self.activation((self.conv2(x)))
         x = self.activation((self.conv3(x)))
+        x = x.view(x.size(0), -1)  # flatten
         return x
 
     def forward(self, x):
         """
         Forward convolutional network
 
         Parameters
         ----------
         x: torch.tensor
-            Tensor of shape BCHW
+            Tensor of shape BCHW (Batch,Chanel,Height,Width : if more than 4 dimensions, merge all the first in batch dimension)
         """
-        return self.head(self.convolutions(x))
+        flag_view_to_change = False
+
+        if len(x.shape) > 4:
+            flag_view_to_change = True
+            dim_to_retore = x.shape[:-3]
+            inputview_size = tuple((-1,)) + tuple(x.shape[-3:])
+            outputview_size = tuple(dim_to_retore) + tuple(
+                (self.head_mlp_kwargs["out_size"],)
+            )
+            x = x.view(inputview_size)
+
+        conv_result = self.convolutions(x)
+        output_result = self.head(
+            conv_result.view(conv_result.size()[0], -1)
+        )  # give the 'conv_result' flattenned in 2 dimensions (batch and other) to the MLP (head)
+
+        if flag_view_to_change:
+            output_result = output_result.view(outputview_size)
+
+        return output_result
 
     def action_scores(self, x):
         return self.head.action_scores(self.convolutions(x))
```

### Comparing `rlberry-0.4.0/rlberry/agents/torch/utils/training.py` & `rlberry-0.4.1/rlberry/agents/torch/utils/training.py`

 * *Files 12% similar despite different names*

```diff
@@ -45,46 +45,40 @@
     """Build a neural net of a given type.
 
     Parameters
     ----------
     type: {"MultiLayerPerceptron",
            "ConvolutionalNetwork",
            "DuelingNetwork",
-           "EgoAttentionNetwork",
            "Table"}, default = "MultiLayerPerceptron"
         Type of neural network.
     **kwargs: dict
         Parameters that vary according to each neural net type, see
 
         * :class:`~rlberry.agents.torch.utils.models.MultiLayerPerceptron`
 
         * :class:`~rlberry.agents.torch.utils.models.ConvolutionalNetwork`
 
         * :class:`~rlberry.agents.torch.utils.models.DuelingNetwork`
 
-        * :class:`~rlberry.agents.torch.utils.attention_models.EgoAttentionNetwork`
-
         * :class:`~rlberry.agents.torch.utils.models.Table`
     """
-    from rlberry.agents.torch.utils.attention_models import EgoAttentionNetwork
     from rlberry.agents.torch.utils.models import (
         MultiLayerPerceptron,
         DuelingNetwork,
         ConvolutionalNetwork,
         Table,
     )
 
     if type == "MultiLayerPerceptron":
         return MultiLayerPerceptron(**kwargs)
     elif type == "DuelingNetwork":
         return DuelingNetwork(**kwargs)
     elif type == "ConvolutionalNetwork":
         return ConvolutionalNetwork(**kwargs)
-    elif type == "EgoAttentionNetwork":
-        return EgoAttentionNetwork(**kwargs)
     elif type == "Table":
         return Table(**kwargs)
     else:
         raise ValueError("Unknown model type")
 
 
 def size_model_config(env, **model_config):
@@ -107,18 +101,31 @@
         obs_shape = env.observation_space.shape
     elif isinstance(env.observation_space, spaces.Tuple):
         obs_shape = env.observation_space.spaces[0].shape
     elif isinstance(env.observation_space, spaces.Discrete):
         return model_config
 
     # Assume CHW observation space
-    if model_config["type"] == "ConvolutionalNetwork":
-        model_config["in_channels"] = int(obs_shape[0])
-        model_config["in_height"] = int(obs_shape[1])
-        model_config["in_width"] = int(obs_shape[2])
+    if "type" in model_config and model_config["type"] == "ConvolutionalNetwork":
+        if "transpose_obs" in model_config and not model_config["transpose_obs"]:
+            # Assume CHW observation space
+            if "in_channels" not in model_config:
+                model_config["in_channels"] = int(obs_shape[0])
+            if "in_height" not in model_config:
+                model_config["in_height"] = int(obs_shape[1])
+            if "in_width" not in model_config:
+                model_config["in_width"] = int(obs_shape[2])
+        else:
+            # Assume WHC observation space to transpose
+            if "in_channels" not in model_config:
+                model_config["in_channels"] = int(obs_shape[2])
+            if "in_height" not in model_config:
+                model_config["in_height"] = int(obs_shape[1])
+            if "in_width" not in model_config:
+                model_config["in_width"] = int(obs_shape[0])
     else:
         model_config["in_size"] = int(np.prod(obs_shape))
 
     if "out_size" not in model_config:
         if isinstance(env.action_space, spaces.Discrete):
             model_config["out_size"] = env.action_space.n
         elif isinstance(env.action_space, spaces.Tuple):
```

### Comparing `rlberry-0.4.0/rlberry/agents/ucbvi/ucbvi.py` & `rlberry-0.4.1/rlberry/agents/ucbvi/ucbvi.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.4.0/rlberry/agents/ucbvi/utils.py` & `rlberry-0.4.1/rlberry/agents/ucbvi/utils.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.4.0/rlberry/agents/utils/replay.py` & `rlberry-0.4.1/rlberry/agents/utils/replay.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,15 +54,15 @@
     >>> rng = np.random.default_rng()
     >>> buffer = replay.ReplayBuffer(100_000, rng)
     >>> buffer.setup_entry("observations", np.float32)
     >>> buffer.setup_entry("actions", np.uint32)
     >>> buffer.setup_entry("rewards", np.float32)
     >>>
     >>> # Store data in the replay
-    >>> env = gym_make("CartPole-v0")
+    >>> env = gym_make("CartPole-v1")
     >>> for _ in range(500):
     >>>     done = False
     >>>     obs = env.reset()
     >>>     while not done:
     >>>         action = env.action_space.sample()
     >>>         next_obs, reward, done, info = env.step(action)
     >>>         buffer.append(
```

### Comparing `rlberry-0.4.0/rlberry/agents/utils/replay_utils.py` & `rlberry-0.4.1/rlberry/agents/utils/replay_utils.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.4.0/rlberry/colab_utils/display_setup.py` & `rlberry-0.4.1/rlberry/colab_utils/display_setup.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.4.0/rlberry/envs/bandits/bandit_base.py` & `rlberry-0.4.1/rlberry/envs/bandits/bandit_base.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from collections import deque
 
-
 from rlberry.envs.interface import Model
 import rlberry.spaces as spaces
-
+from rlberry.seeding import Seeder
 
 import rlberry
 
 logger = rlberry.logger
 
 
 class Bandit(Model):
@@ -29,26 +28,58 @@
 
     def __init__(self, laws=[], **kwargs):
         Model.__init__(self, **kwargs)
         self.laws = laws
         self.n_arms = len(self.laws)
         self.action_space = spaces.Discrete(self.n_arms)
 
+        # Pre-sample 10 samples
+        self.rewards = [
+            deque(self.laws[action].rvs(size=10, random_state=self.rng))
+            for action in range(self.n_arms)
+        ]
+        self.n_rewards = [10] * self.n_arms
+
     def step(self, action):
         """
         Sample the reward associated to the action.
         """
         # test that the action exists
         assert action < self.n_arms
 
-        reward = self.laws[action].rvs(random_state=self.rng)
+        # If the queue of reward for the action is empty, sample 2*size of old reward queue. Otherwise, pop from queue
+        if self.rewards[action]:
+            reward = self.rewards[action].pop()
+        else:
+            self.n_rewards[action] = 2 * self.n_rewards[action]
+            self.rewards[action] = deque(
+                self.laws[action].rvs(
+                    size=self.n_rewards[action], random_state=self.rng
+                )
+            )
+            reward = self.rewards[action].pop()
+
         done = True
 
         return 0, reward, done, {}
 
+    def reseed(self, seed_seq=None):
+        if seed_seq is None:
+            self.seeder = self.seeder.spawn()
+        else:
+            self.seeder = Seeder(seed_seq)
+        # spaces
+        self.action_space.reseed(self.seeder.seed_seq)
+
+        self.rewards = [
+            deque(self.laws[action].rvs(size=10, random_state=self.rng))
+            for action in range(self.n_arms)
+        ]
+        self.n_rewards = [10] * self.n_arms
+
     def reset(self):
         """
         Reset the environment to a default state.
         """
         return 0
```

### Comparing `rlberry-0.4.0/rlberry/envs/bandits/corrupted_bandits.py` & `rlberry-0.4.1/rlberry/envs/bandits/corrupted_bandits.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,32 +10,32 @@
 
     Parameters
     ----------
     law: law
         Can either be a frozen scipy law or any class that
         has a method .rvs() to sample according to the given law.
 
+
     cor_prop: float in (0,1/2)
         Proportion of corruption
 
     cor_law: law
         Laws of corruption.
     """
 
     def __init__(self, law, cor_prop, cor_law):
         self.law = law
         self.cor_prop = cor_prop
         self.cor_law = cor_law
 
-    def rvs(self, random_state):
-        is_corrupted = random_state.binomial(1, self.cor_prop)
-        if is_corrupted == 1:
-            return self.cor_law.rvs(random_state=random_state)
-        else:
-            return self.law.rvs(random_state=random_state)
+    def rvs(self, size, random_state):
+        is_corrupted = random_state.binomial(1, self.cor_prop, size=size)
+        cor_sample = self.cor_law.rvs(size=size, random_state=random_state)
+        noncor_sample = self.law.rvs(size=size, random_state=random_state)
+        return is_corrupted * cor_sample + (1 - is_corrupted) * noncor_sample
 
     def mean(self):
         return (
             1 - self.cor_prop
         ) * self.law.mean() + self.cor_prop * self.cor_law.mean()
```

### Comparing `rlberry-0.4.0/rlberry/envs/bandits/stochastic_bandits.py` & `rlberry-0.4.1/rlberry/envs/bandits/stochastic_bandits.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.4.0/rlberry/envs/basewrapper.py` & `rlberry-0.4.1/rlberry/envs/basewrapper.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.4.0/rlberry/envs/benchmarks/ball_exploration/ball2d.py` & `rlberry-0.4.1/rlberry/envs/benchmarks/ball_exploration/ball2d.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.4.0/rlberry/envs/benchmarks/ball_exploration/pball.py` & `rlberry-0.4.1/rlberry/envs/benchmarks/ball_exploration/pball.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.4.0/rlberry/envs/benchmarks/generalization/twinrooms.py` & `rlberry-0.4.1/rlberry/envs/benchmarks/generalization/twinrooms.py`

 * *Files 2% similar despite different names*

```diff
@@ -154,15 +154,15 @@
         shape.add_vertex((1 - eps, 0))
         shape.add_vertex((1 - eps, 1))
         shape.add_vertex((1 + eps, 1))
         shape.add_vertex((1 + eps, 0))
         bg.add_shape(shape)
 
         # rewards
-        for (x, y) in [
+        for x, y in [
             self.base_reward_pos,
             self.base_reward_pos + np.array([1.0, 0.0]),
         ]:
             reward = circle_shape((x, y), 0.1, n_points=50)
             reward.type = "POLYGON"
             reward.set_color((0.0, 0.5, 0.0))
             bg.add_shape(reward)
```

### Comparing `rlberry-0.4.0/rlberry/envs/benchmarks/grid_exploration/apple_gold.py` & `rlberry-0.4.1/rlberry/envs/benchmarks/grid_exploration/apple_gold.py`

 * *Files 1% similar despite different names*

```diff
@@ -144,15 +144,15 @@
             shape.add_vertex((x, y))
             shape.add_vertex((x + 1, y))
             shape.add_vertex((x + 1, y + 1))
             shape.add_vertex((x, y + 1))
             bg.add_shape(shape)
 
         # rewards
-        for (y, x) in self.reward_at:
+        for y, x in self.reward_at:
             rwd = self.reward_at[(y, x)]
             if rwd == -0.05:
                 rock = GeometricPrimitive("POLYGON")
                 rock.set_color((0.6, 0.6, 0.6))
                 rock.add_vertex((x, y))
                 rock.add_vertex((x + 1, y))
                 rock.add_vertex((x + 1, y + 1))
```

### Comparing `rlberry-0.4.0/rlberry/envs/benchmarks/grid_exploration/four_room.py` & `rlberry-0.4.1/rlberry/envs/benchmarks/grid_exploration/four_room.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.4.0/rlberry/envs/benchmarks/grid_exploration/nroom.py` & `rlberry-0.4.1/rlberry/envs/benchmarks/grid_exploration/nroom.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,15 +66,14 @@
         array_observation=False,
         room_size=5,
         success_probability=0.95,
         remove_walls=False,
         initial_state_distribution="center",
         include_traps=False,
     ):
-
         assert nrooms > 0, "nrooms must be > 0"
         assert initial_state_distribution in ("center", "uniform")
 
         self.reward_free = reward_free
         self.array_observation = array_observation
         self.nrooms = nrooms
         self.room_size = room_size
@@ -259,15 +258,15 @@
     def get_background(self):
         """
         Returne a scene (list of shapes) representing the background
         """
         bg = Scene()
 
         # traps
-        for (y, x) in self.traps:
+        for y, x in self.traps:
             shape = GeometricPrimitive("POLYGON")
             shape.set_color((0.5, 0.0, 0.0))
             shape.add_vertex((x, y))
             shape.add_vertex((x + 1, y))
             shape.add_vertex((x + 1, y + 1))
             shape.add_vertex((x, y + 1))
             bg.add_shape(shape)
@@ -280,15 +279,15 @@
             shape.add_vertex((x, y))
             shape.add_vertex((x + 1, y))
             shape.add_vertex((x + 1, y + 1))
             shape.add_vertex((x, y + 1))
             bg.add_shape(shape)
 
         # rewards
-        for (y, x) in self.reward_at:
+        for y, x in self.reward_at:
             flag = GeometricPrimitive("POLYGON")
             rwd = self.reward_at[(y, x)]
             if rwd == 1.0:
                 flag.set_color((0.0, 0.5, 0.0))
             elif rwd == 0.1:
                 flag.set_color((0.0, 0.0, 0.5))
             else:
```

### Comparing `rlberry-0.4.0/rlberry/envs/benchmarks/grid_exploration/six_room.py` & `rlberry-0.4.1/rlberry/envs/benchmarks/grid_exploration/six_room.py`

 * *Files 7% similar despite different names*

```diff
@@ -127,15 +127,15 @@
             shape.add_vertex((x, y))
             shape.add_vertex((x + 1, y))
             shape.add_vertex((x + 1, y + 1))
             shape.add_vertex((x, y + 1))
             bg.add_shape(shape)
 
         # rewards
-        for (y, x) in self.reward_at:
+        for y, x in self.reward_at:
             flag = GeometricPrimitive("POLYGON")
             rwd = self.reward_at[(y, x)]
             if rwd == 10:
                 flag.set_color((0.0, 0.5, 0.0))
             else:
                 flag.set_color((0.0, 0.0, 0.5))
```

### Comparing `rlberry-0.4.0/rlberry/envs/classic_control/SpringCartPole.py` & `rlberry-0.4.1/rlberry/envs/classic_control/SpringCartPole.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.4.0/rlberry/envs/classic_control/acrobot.py` & `rlberry-0.4.1/rlberry/envs/classic_control/acrobot.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.4.0/rlberry/envs/classic_control/mountain_car.py` & `rlberry-0.4.1/rlberry/envs/classic_control/mountain_car.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.4.0/rlberry/envs/classic_control/pendulum.py` & `rlberry-0.4.1/rlberry/envs/classic_control/pendulum.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.4.0/rlberry/envs/finite/chain.py` & `rlberry-0.4.1/rlberry/envs/finite/chain.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.4.0/rlberry/envs/finite/finite_mdp.py` & `rlberry-0.4.1/rlberry/envs/finite/finite_mdp.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.4.0/rlberry/envs/finite/gridworld.py` & `rlberry-0.4.1/rlberry/envs/finite/gridworld.py`

 * *Files 0% similar despite different names*

```diff
@@ -275,15 +275,15 @@
             for cc in range(self.ncols):
                 if (rr, cc) in self.walls:
                     grid[rr][cc] = "x "
                 else:
                     grid[rr][cc] = "o "
                 grid_idx[rr][cc] = str(self.coord2index[(rr, cc)]).zfill(3)
 
-        for (rr, cc) in self.reward_at:
+        for rr, cc in self.reward_at:
             rwd = self.reward_at[(rr, cc)]
             if rwd > 0:
                 grid[rr][cc] = "+ "
             if rwd < 0:
                 grid[rr][cc] = "-"
 
         grid[self.start_coord[0]][self.start_coord[1]] = "I "
@@ -448,15 +448,15 @@
             shape.add_vertex((x, y))
             shape.add_vertex((x + 1, y))
             shape.add_vertex((x + 1, y + 1))
             shape.add_vertex((x, y + 1))
             bg.add_shape(shape)
 
         # rewards
-        for (y, x) in self.reward_at:
+        for y, x in self.reward_at:
             flag = GeometricPrimitive("POLYGON")
             rwd = self.reward_at[(y, x)]
             color = 0.5 * np.abs(rwd) / self.reward_range[1]
             if rwd > 0:
                 flag.set_color((0.0, color, 0.0))
             if rwd < 0:
                 flag.set_color((color, 0.0, 0.0))
```

### Comparing `rlberry-0.4.0/rlberry/envs/finite/gridworld_utils.py` & `rlberry-0.4.1/rlberry/envs/finite/gridworld_utils.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.4.0/rlberry/envs/interface/model.py` & `rlberry-0.4.1/rlberry/envs/interface/model.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.4.0/rlberry/envs/pipeline.py` & `rlberry-0.4.1/rlberry/envs/pipeline.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.4.0/rlberry/envs/tests/test_bandits.py` & `rlberry-0.4.1/rlberry/envs/tests/test_bandits.py`

 * *Files 9% similar despite different names*

```diff
@@ -13,23 +13,34 @@
 
 
 def test_bernoulli():
     env = BernoulliBandit(p=[0.05, 0.95])
     safe_reseed(env, Seeder(TEST_SEED))
 
     sample = [env.step(1)[1] for f in range(1000)]
+
+    safe_reseed(env, Seeder(TEST_SEED))
+
+    sample2 = [env.step(1)[1] for f in range(1000)]
+
     assert np.abs(np.mean(sample) - 0.95) < 0.1
+    assert np.mean(sample) == np.mean(sample2), "Not reproducible"
 
 
 def test_normal():
     env = NormalBandit(means=[0, 1])
     safe_reseed(env, Seeder(TEST_SEED))
 
     sample = [env.step(1)[1] for f in range(1000)]
+    safe_reseed(env, Seeder(TEST_SEED))
+
+    sample2 = [env.step(1)[1] for f in range(1000)]
+
     assert np.abs(np.mean(sample) - 1) < 0.1
+    assert np.abs(sample[0] - sample2[0]) < 0.01, "Not reproducible"
 
 
 def test_cor_normal():
     env = CorruptedNormalBandit(means=[0, 1], cor_prop=0.1)
     safe_reseed(env, Seeder(TEST_SEED))
 
     sample = [env.step(1)[1] for f in range(1000)]
```

### Comparing `rlberry-0.4.0/rlberry/envs/tests/test_env_seeding.py` & `rlberry-0.4.1/rlberry/envs/tests/test_env_seeding.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.4.0/rlberry/envs/tests/test_gym_env_seeding.py` & `rlberry-0.4.1/rlberry/envs/tests/test_gym_env_seeding.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.4.0/rlberry/envs/tests/test_instantiation.py` & `rlberry-0.4.1/rlberry/envs/tests/test_instantiation.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.4.0/rlberry/envs/tests/test_spring_env.py` & `rlberry-0.4.1/rlberry/envs/tests/test_spring_env.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 # action_dict = {0: "LL", 1: "RR", 2: "LR", 3: "RL"}
 
 
 HORIZON = 20
 
 
 def test_spring_cartpole():
-
     # test 1 - default
     env = SpringCartPole()
 
     _ = env.reset()
     for _ in range(2):
         action = np.random.randint(0, env.action_space.n)
         next_state, _, done, _ = env.step(action)
@@ -80,14 +79,15 @@
     _ = env.get_video()
 
 
 def test_rk4():
     """
     Test of the rk4 utils defined in speingcartpole
     """
+
     ## 2D system
     def derivs6(x, t):
         d1 = x[0] + 2 * x[1]
         d2 = -3 * x[0] + 4 * x[1]
         return (d1, d2)
 
     dt = 0.0005
```

### Comparing `rlberry-0.4.0/rlberry/envs/utils.py` & `rlberry-0.4.1/rlberry/envs/utils.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.4.0/rlberry/experiment/generator.py` & `rlberry-0.4.1/rlberry/experiment/generator.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     """
     Parse command line arguments and yields AgentManager instances.
     """
     args = docopt(__doc__)
     max_workers = int(args["--max_workers"])
     if max_workers == -1:
         max_workers = None
-    for (_, agent_manager_kwargs) in parse_experiment_config(
+    for _, agent_manager_kwargs in parse_experiment_config(
         Path(args["<experiment_path>"]),
         n_fit=int(args["--n_fit"]),
         max_workers=max_workers,
         output_base_dir=args["--output_dir"],
         parallelization=args["--parallelization"],
     ):
         if args["--enable_tensorboard"]:
```

### Comparing `rlberry-0.4.0/rlberry/experiment/load_results.py` & `rlberry-0.4.1/rlberry/experiment/load_results.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.4.0/rlberry/experiment/yaml_utils.py` & `rlberry-0.4.1/rlberry/experiment/yaml_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -206,9 +206,9 @@
                 seed=seed,
                 outdir_id_style=None,
             )  # output_dir is already made unique above
 
 
 if __name__ == "__main__":
     filename = "examples/demo_experiment/params_experiment.yaml"
-    for (seed, agent_manager) in parse_experiment_config(Path(filename)):
+    for seed, agent_manager in parse_experiment_config(Path(filename)):
         print(seed)
```

### Comparing `rlberry-0.4.0/rlberry/exploration_tools/discrete_counter.py` & `rlberry-0.4.1/rlberry/exploration_tools/discrete_counter.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.4.0/rlberry/exploration_tools/online_discretization_counter.py` & `rlberry-0.4.1/rlberry/exploration_tools/online_discretization_counter.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.4.0/rlberry/exploration_tools/tests/test_discrete_counter.py` & `rlberry-0.4.1/rlberry/exploration_tools/tests/test_discrete_counter.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.4.0/rlberry/exploration_tools/torch/rnd.py` & `rlberry-0.4.1/rlberry/exploration_tools/torch/rnd.py`

 * *Files 0% similar despite different names*

```diff
@@ -142,15 +142,14 @@
                 )
                 random_embedding = random_embedding.gather(1, action).squeeze(1)
                 predicted_embedding = predicted_embedding.gather(1, action).squeeze(1)
         return random_embedding, predicted_embedding
 
     @preprocess_args(expected_type="torch")
     def update(self, state, action=None, next_state=None, reward=None, **kwargs):
-
         batch = [(state, action)]
         if self.batch_size > 0 and not self.memory.is_empty():
             batch += self.memory.sample(self.batch_size)
             self.memory.push((state, action))
         states, actions = zip(*batch)
         states = torch.stack(states)
         if self.with_action:
```

### Comparing `rlberry-0.4.0/rlberry/exploration_tools/torch/tests/test_rnd.py` & `rlberry-0.4.1/rlberry/exploration_tools/torch/tests/test_rnd.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.4.0/rlberry/exploration_tools/typing.py` & `rlberry-0.4.1/rlberry/exploration_tools/typing.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.4.0/rlberry/exploration_tools/uncertainty_estimator.py` & `rlberry-0.4.1/rlberry/exploration_tools/uncertainty_estimator.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.4.0/rlberry/manager/agent_manager.py` & `rlberry-0.4.1/rlberry/manager/agent_manager.py`

 * *Files 3% similar despite different names*

```diff
@@ -400,19 +400,19 @@
             self.tensorboard_dir = self.output_dir_ / "tensorboard"
             for idx, params in enumerate(self.agent_default_writer_kwargs):
                 params["tensorboard_kwargs"] = dict(
                     log_dir=self.tensorboard_dir / str(idx)
                 )
         # Update DefaultWriter according to user's settings.
         default_writer_kwargs = default_writer_kwargs or {}
-        if default_writer_kwargs:
-            logger.warning(
-                "(Re)defining the following DefaultWriter"
-                f" parameters in AgentManager: {list(default_writer_kwargs.keys())}"
-            )
+        # if default_writer_kwargs:
+        #     logger.warning(
+        #         "(Re)defining the following DefaultWriter"
+        #         f" parameters in AgentManager: {list(default_writer_kwargs.keys())}"
+        #     )
         for ii in range(n_fit):
             self.agent_default_writer_kwargs[ii].update(default_writer_kwargs)
 
         # agent handlers and init kwargs
         self._set_init_kwargs()  # init_kwargs for each agent
         self.agent_handlers = None
         self._reset_agent_handlers()
@@ -582,14 +582,16 @@
                 logger.info("  Evaluation finished \n")
                 logger.handlers = previous_handlers
 
         return values
 
     def clear_output_dir(self):
         """Delete output_dir and all its data."""
+        if self.optuna_study:
+            optuna.delete_study(self.optuna_study.study_name, self.optuna_storage_url)
         try:
             shutil.rmtree(self.output_dir_)
         except FileNotFoundError:
             logger.warning(f"No directory {self.output_dir_} found to be deleted.")
 
     def clear_handlers(self):
         """Delete files from output_dir/agent_handlers that are managed by this class."""
@@ -664,14 +666,15 @@
         budget: int or None
             Computational or sample complexity budget.
         """
         del kwargs
         budget = budget or self.fit_budget
 
         # If spawn, test that protected by if __name__ == "__main__"
+
         if self.mp_context == "spawn":
             try:
                 _check_not_importing_main()
             except RuntimeError as exc:
                 raise RuntimeError(
                     """Warning: in AgentManager, if mp_context='spawn' and
                         parallelization="process" then the script must be run
@@ -873,15 +876,14 @@
                     + str(obj.rlberry_version)
                     + "."
                 )
 
         return obj
 
     def __eq__(self, other):
-
         result = True
         self_init_kwargs = [_strip_seed_dir(kw) for kw in self.init_kwargs]
         other_init_kwargs = [_strip_seed_dir(kw) for kw in other.init_kwargs]
         result = result and all(
             [
                 self_init_kwargs[f] == other_init_kwargs[f]
                 for f in range(len(self_init_kwargs))
@@ -1029,15 +1031,14 @@
                 raise NotImplementedError(
                     "Pruner method %s is not implemented." % pruner_method
                 )
 
             # storage
             self._init_optuna_storage_url()
             storage = optuna.storages.RDBStorage(self.optuna_storage_url)
-
             # optuna study
             study = optuna.create_study(
                 sampler=sampler, pruner=pruner, storage=storage, direction="maximize"
             )
             self.optuna_study = study
 
         # save, to that optimization can be resumed later
@@ -1173,22 +1174,29 @@
         agent_handler.set_writer(None)
     elif (
         writer[0] != "default"
     ):  # 'default' corresponds to DefaultWriter created by Agent.__init__()
         writer_fn = writer[0]
         writer_kwargs = writer[1]
         agent_handler.set_writer(writer_fn(**writer_kwargs))
+
+    if agent_handler.writer._style_log == "progressbar":
+        agent_handler.writer.set_max_global_step(fit_budget)
     # fit agent
     agent_handler.fit(fit_budget, **fit_kwargs)
 
     # Remove writer after fit (prevent pickle problems),
     # unless the agent uses DefaultWriter
     if not isinstance(agent_handler.writer, DefaultWriter):
         agent_handler.set_writer(None)
 
+    if agent_handler.writer._style_log == "progressbar":
+        agent_handler.writer.pbar.close()
+        agent_handler.writer.pbar = None
+
     # remove from memory to avoid pickle issues
     agent_handler.dump()
 
     # garbage collector
     gc.collect()
 
     return agent_handler
@@ -1308,7 +1316,39 @@
     del res["output_dir"]
     return res
 
 
 def is_bz_file(filepath):
     with open(filepath, "rb") as test_f:
         return test_f.read(2) == b"BZ"
+
+
+def preset_manager(*args, **kwds):
+    """Preset an Agent Manager to some fixed keywords.
+
+    Examples
+    --------
+    >>> from rlberry.agents.torch import PPOAgent, DQNAgent
+    >>> from rlberry.manager import preset_manager
+    >>> from rlberry.envs import Acrobot
+    >>> env_ctor = Acrobot
+    >>> env_kwargs = {}
+    >>>
+    >>> manager_maker =  preset_manager(train_env=(env_ctor, env_kwargs),
+    >>>                                 eval_kwargs=dict(eval_horizon=500),
+    >>>                                 n_fit=4,
+    >>>                                 parallelization = "process",
+    >>>                                 mp_context="spawn",
+    >>>                                 seed=42,
+    >>>                                 max_workers=6
+    >>>                                 )
+    >>> ppo = manager_maker(PPOAgent, fit_budget = 100) # of type AgentManager
+    >>> dqn = manager_maker(DQNAgent, fit_budget = 200)
+    >>>
+    >>> ppo.fit()
+    >>> dqn.fit()
+    """
+
+    class Manager(AgentManager):
+        __init__ = functools.partialmethod(AgentManager.__init__, *args, **kwds)
+
+    return Manager
```

### Comparing `rlberry-0.4.0/rlberry/manager/evaluation.py` & `rlberry-0.4.1/rlberry/manager/evaluation.py`

 * *Files 0% similar despite different names*

```diff
@@ -275,15 +275,14 @@
                     # add column
                     data_list.append(processed_df)
     all_writer_data = pd.concat(data_list, ignore_index=True)
     return all_writer_data
 
 
 def _get_last_xp(input_dir, name):
-
     dir_name = Path(input_dir) / "manager_data"
 
     # list all of the experiments for this particular agent
     agent_xp = list(dir_name.glob(name + "*"))
 
     # get the times at which the experiment have been made
     times = [str(p).split("_")[-2] for p in agent_xp]
```

### Comparing `rlberry-0.4.0/rlberry/manager/multiple_managers.py` & `rlberry-0.4.1/rlberry/manager/multiple_managers.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.4.0/rlberry/manager/remote_agent_manager.py` & `rlberry-0.4.1/rlberry/manager/remote_agent_manager.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.4.0/rlberry/manager/tests/test_agent_manager.py` & `rlberry-0.4.1/rlberry/manager/tests/test_agent_manager.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,19 @@
 import pytest
 import numpy as np
+import sys
 import os
 from rlberry.envs import GridWorld
 from rlberry.agents import AgentWithSimplePolicy
-from rlberry.manager import AgentManager, plot_writer_data, evaluate_agents
+from rlberry.manager import (
+    AgentManager,
+    plot_writer_data,
+    evaluate_agents,
+    preset_manager,
+)
 
 
 class DummyAgent(AgentWithSimplePolicy):
     def __init__(self, env, hyperparameter1=0, hyperparameter2=0, **kwargs):
         AgentWithSimplePolicy.__init__(self, env, **kwargs)
         self.name = "DummyAgent"
         self.fitted = False
@@ -28,18 +34,19 @@
 
     def policy(self, observation):
         return 0
 
     @classmethod
     def sample_parameters(cls, trial):
         hyperparameter1 = trial.suggest_categorical("hyperparameter1", [1, 2, 3])
-        hyperparameter2 = trial.suggest_uniform("hyperparameter2", -10, 10)
+        hyperparameter2 = trial.suggest_float("hyperparameter2", -10, 10)
         return {"hyperparameter1": hyperparameter1, "hyperparameter2": hyperparameter2}
 
 
+@pytest.mark.xfail(sys.platform == "win32", reason="bug with windows???")
 def test_agent_manager_1():
     # Define train and evaluation envs
     train_env = (GridWorld, {})
 
     # Parameters
     params = dict(hyperparameter1=-1, hyperparameter2=100)
     eval_kwargs = dict(eval_horizon=10)
@@ -103,14 +110,15 @@
     loaded_stats.optimize_hyperparams(n_trials=3)
     loaded_stats.optimize_hyperparams(n_trials=3, continue_previous=True)
 
     for st in agent_manager_list:
         st.clear_output_dir()
 
 
+@pytest.mark.xfail(sys.platform == "win32", reason="bug with windows???")
 def test_agent_manager_2():
     # Define train and evaluation envs
     train_env = (GridWorld, {})
     eval_env = (GridWorld, {})
 
     # Parameters
     params = {}
@@ -321,14 +329,38 @@
         seed=123,
         init_kwargs_per_instance=params_per_instance,
     )
     stats_agent1.generate_profile(fname="profile.prof")
     assert os.path.getsize("profile.prof") > 100, "agent manager saved an empty profile"
 
 
+def test_preset():
+    # Define train and evaluation envs
+    train_env = (GridWorld, {})
+
+    # Parameters
+    params = dict(hyperparameter1=-1, hyperparameter2=100)
+    eval_kwargs = dict(eval_horizon=10)
+
+    # Run AgentManager
+    params_per_instance = [dict(hyperparameter2=ii) for ii in range(4)]
+
+    manager_maker = preset_manager(
+        train_env=train_env,
+        fit_budget=4,
+        eval_kwargs=eval_kwargs,
+        init_kwargs=params,
+        n_fit=4,
+        seed=123,
+        init_kwargs_per_instance=params_per_instance,
+    )
+    manager = manager_maker(DummyAgent)
+    manager.fit()
+
+
 def test_compress():
     # Define train and evaluation envs
     train_env = (GridWorld, {})
 
     # Parameters
     params = dict(
         hyperparameter1=-1, hyperparameter2=lambda x: 42, compress_pickle=True
```

### Comparing `rlberry-0.4.0/rlberry/manager/tests/test_agent_manager_seeding.py` & `rlberry-0.4.1/rlberry/manager/tests/test_agent_manager_seeding.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.4.0/rlberry/manager/tests/test_plot.py` & `rlberry-0.4.1/rlberry/manager/tests/test_plot.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import pytest
 import tempfile
 import os
 import numpy as np
 from pathlib import Path
-
+import sys
 
 from rlberry.wrappers import WriterWrapper
 from rlberry.envs import GridWorld
 from rlberry.manager import plot_writer_data, AgentManager, read_writer_data
 from rlberry.agents import UCBVIAgent
 
 
@@ -83,14 +83,15 @@
         )
         assert (
             os.path.getsize(tmpdirname + "/test.png") > 1000
         ), "plot_writer_data saved an empty image"
         assert len(output) > 1
 
 
+@pytest.mark.xfail(sys.platform == "win32", reason="bug with windows???")
 @pytest.mark.parametrize("outdir_id_style", ["timestamp"])
 def test_plot_writer_data_with_directory_input(outdir_id_style):
     with tempfile.TemporaryDirectory() as tmpdirname:
         output_dir = tmpdirname + "/rlberry_data"
         manager = _create_and_fit_agent_manager(output_dir, outdir_id_style)
         del manager
```

### Comparing `rlberry-0.4.0/rlberry/manager/tests/test_shared_data.py` & `rlberry-0.4.1/rlberry/manager/tests/test_shared_data.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.4.0/rlberry/metadata_utils.py` & `rlberry-0.4.1/rlberry/metadata_utils.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.4.0/rlberry/network/client.py` & `rlberry-0.4.1/rlberry/network/client.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.4.0/rlberry/network/interface.py` & `rlberry-0.4.1/rlberry/network/interface.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.4.0/rlberry/network/server.py` & `rlberry-0.4.1/rlberry/network/server.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.4.0/rlberry/network/server_utils.py` & `rlberry-0.4.1/rlberry/network/server_utils.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.4.0/rlberry/network/utils.py` & `rlberry-0.4.1/rlberry/network/utils.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.4.0/rlberry/rendering/common_shapes.py` & `rlberry-0.4.1/rlberry/rendering/common_shapes.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.4.0/rlberry/rendering/core.py` & `rlberry-0.4.1/rlberry/rendering/core.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.4.0/rlberry/rendering/opengl_render2d.py` & `rlberry-0.4.1/rlberry/rendering/opengl_render2d.py`

 * *Files 1% similar despite different names*

```diff
@@ -231,15 +231,15 @@
                 #
                 pg.display.flip()
 
                 #
                 # See https://stackoverflow.com/a/42754578/5691288
                 #
                 string_image = self.get_gl_image_str()
-                temp_surf = pg.image.fromstring(
+                temp_surf = pg.image.frombytes(
                     string_image, (self.window_width, self.window_height), "RGB"
                 )
                 tmp_arr = pg.surfarray.array3d(temp_surf)
                 imgdata = np.moveaxis(tmp_arr, 0, 1)
                 imgdata = np.flipud(imgdata)
                 video_data.append(imgdata)
```

### Comparing `rlberry-0.4.0/rlberry/rendering/pygame_render2d.py` & `rlberry-0.4.1/rlberry/rendering/pygame_render2d.py`

 * *Files 1% similar despite different names*

```diff
@@ -176,16 +176,16 @@
                 self.display()
                 #
                 pg.display.flip()
 
                 #
                 # See https://stackoverflow.com/a/42754578/5691288
                 #
-                string_image = pg.image.tostring(self.screen, "RGB")
-                temp_surf = pg.image.fromstring(
+                string_image = pg.image.tobytes(self.screen, "RGB")
+                temp_surf = pg.image.frombytes(
                     string_image, (self.window_width, self.window_height), "RGB"
                 )
                 tmp_arr = pg.surfarray.array3d(temp_surf)
                 imgdata = np.moveaxis(tmp_arr, 0, 1)
                 video_data.append(imgdata)
 
             pg.quit()
```

### Comparing `rlberry-0.4.0/rlberry/rendering/render_interface.py` & `rlberry-0.4.1/rlberry/rendering/render_interface.py`

 * *Files 0% similar despite different names*

```diff
@@ -136,15 +136,14 @@
             renderer.run_graphics(loop)
             return 0
         else:
             logger.info("Rendering not enabled for the environment.")
             return 1
 
     def get_video(self, framerate=25, **kwargs):
-
         # background and data
         background, data = self._get_background_and_scenes()
 
         if len(data) == 0:
             logger.info("No data to save.")
             return
```

### Comparing `rlberry-0.4.0/rlberry/rendering/tests/test_rendering_interface.py` & `rlberry-0.4.1/rlberry/rendering/tests/test_rendering_interface.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import os
 import pytest
+import sys
 
 from pyvirtualdisplay import Display
 from rlberry.envs.classic_control import MountainCar
 from rlberry.envs.classic_control import Acrobot
 from rlberry.envs.classic_control import Pendulum
 from rlberry.envs.finite import Chain
 from rlberry.envs.finite import GridWorld
@@ -44,14 +45,15 @@
     if isinstance(env, RenderInterface):
         env.disable_rendering()
         assert not env.is_render_enabled()
         env.enable_rendering()
         assert env.is_render_enabled()
 
 
+@pytest.mark.xfail(sys.platform != "linux", reason="bug with mac and windows???")
 @pytest.mark.parametrize("ModelClass", classes)
 def test_render2d_interface(ModelClass):
     env = ModelClass()
 
     if isinstance(env, RenderInterface2D):
         env.enable_rendering()
 
@@ -68,14 +70,15 @@
             env.clear_render_buffer()
         try:
             os.remove("test_video.mp4")
         except Exception:
             pass
 
 
+@pytest.mark.xfail(sys.platform != "linux", reason="bug with mac and windows???")
 @pytest.mark.parametrize("ModelClass", classes)
 def test_render2d_interface_wrapped(ModelClass):
     env = Wrapper(ModelClass())
 
     if isinstance(env.env, RenderInterface2D):
         env.enable_rendering()
         if env.is_online():
```

### Comparing `rlberry-0.4.0/rlberry/rendering/utils.py` & `rlberry-0.4.1/rlberry/rendering/utils.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.4.0/rlberry/seeding/seeder.py` & `rlberry-0.4.1/rlberry/seeding/seeder.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.4.0/rlberry/seeding/seeding.py` & `rlberry-0.4.1/rlberry/seeding/seeding.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.4.0/rlberry/seeding/tests/test_seeding.py` & `rlberry-0.4.1/rlberry/seeding/tests/test_seeding.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.4.0/rlberry/seeding/tests/test_threads.py` & `rlberry-0.4.1/rlberry/seeding/tests/test_threads.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.4.0/rlberry/seeding/tests/test_threads_torch.py` & `rlberry-0.4.1/rlberry/seeding/tests/test_threads_torch.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.4.0/rlberry/spaces/box.py` & `rlberry-0.4.1/rlberry/spaces/box.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.4.0/rlberry/spaces/dict.py` & `rlberry-0.4.1/rlberry/spaces/dict.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.4.0/rlberry/spaces/discrete.py` & `rlberry-0.4.1/rlberry/spaces/discrete.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.4.0/rlberry/spaces/from_gym.py` & `rlberry-0.4.1/rlberry/spaces/from_gym.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.4.0/rlberry/spaces/multi_binary.py` & `rlberry-0.4.1/rlberry/spaces/multi_binary.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.4.0/rlberry/spaces/multi_discrete.py` & `rlberry-0.4.1/rlberry/spaces/multi_discrete.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.4.0/rlberry/spaces/tests/test_from_gym.py` & `rlberry-0.4.1/rlberry/spaces/tests/test_from_gym.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.4.0/rlberry/spaces/tests/test_spaces.py` & `rlberry-0.4.1/rlberry/spaces/tests/test_spaces.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.4.0/rlberry/spaces/tuple.py` & `rlberry-0.4.1/rlberry/spaces/tuple.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.4.0/rlberry/tests/test_agent.py` & `rlberry-0.4.1/rlberry/tests/test_agents_base.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,14 +1,27 @@
+"""
+===============================================
+Tests for the installation without extra (StableBaselines3, torch, optuna, ...)
+===============================================
+tests based on test_agent.py and test_envs.py
+
+"""
+
+
 import pytest
+import numpy as np
+import sys
+
 import rlberry.agents as agents
-import rlberry.agents.torch as torch_agents
-from rlberry.agents.experimental import torch as torch_exp_agents
-from rlberry.utils.check_agent import check_rl_agent, check_rlberry_agent
 from rlberry.agents.features import FeatureMap
-import numpy as np
+
+from rlberry.utils.check_agent import (
+    check_rl_agent,
+    check_rlberry_agent,
+)
 
 
 class OneHotFeatureMap(FeatureMap):
     def __init__(self, S, A):
         self.S = S
         self.A = A
         self.shape = (S * A,)
@@ -27,37 +40,36 @@
 
         agents.LSVIUCBAgent.__init__(
             self, env, feature_map_fn=feature_map_fn, horizon=10, **kwargs
         )
 
 
 FINITE_MDP_AGENTS = [
+    agents.QLAgent,
+    agents.SARSAAgent,
     agents.ValueIterationAgent,
     agents.MBQVIAgent,
     agents.UCBVIAgent,
     agents.OptQLAgent,
     agents.PSRLAgent,
     agents.RLSVIAgent,
     OneHotLSVI,
 ]
 
 
 CONTINUOUS_STATE_AGENTS = [
     agents.RSUCBVIAgent,
     agents.RSKernelUCBVIAgent,
-    torch_agents.DQNAgent,
-    torch_agents.REINFORCEAgent,
-    torch_agents.PPOAgent,
-    torch_exp_agents.AVECPPOAgent,
 ]
 
 
 @pytest.mark.parametrize("agent", FINITE_MDP_AGENTS)
 def test_finite_state_agent(agent):
     check_rl_agent(agent, env="discrete_state")
     check_rlberry_agent(agent, env="discrete_state")
 
 
+@pytest.mark.xfail(sys.platform == "win32", reason="bug with windows???")
 @pytest.mark.parametrize("agent", CONTINUOUS_STATE_AGENTS)
 def test_continuous_state_agent(agent):
     check_rl_agent(agent, env="continuous_state")
     check_rlberry_agent(agent, env="continuous_state")
```

### Comparing `rlberry-0.4.0/rlberry/tests/test_envs.py` & `rlberry-0.4.1/rlberry/tests/test_envs.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 from rlberry.utils.check_env import check_env, check_rlberry_env
 from rlberry.envs import Acrobot
 from rlberry.envs.benchmarks.ball_exploration import PBall2D
 from rlberry.envs.benchmarks.generalization.twinrooms import TwinRooms
 from rlberry.envs.benchmarks.grid_exploration.apple_gold import AppleGold
 from rlberry.envs.benchmarks.grid_exploration.nroom import NRoom
-from rlberry.envs.classic_control import MountainCar
+from rlberry.envs.classic_control import MountainCar, SpringCartPole
 from rlberry.envs.finite import Chain, GridWorld
 import pytest
 
 ALL_ENVS = [
     Acrobot,
     PBall2D,
     TwinRooms,
     AppleGold,
     NRoom,
     MountainCar,
     Chain,
     GridWorld,
+    SpringCartPole,
 ]
 
 
 @pytest.mark.parametrize("Env", ALL_ENVS)
 def test_env(Env):
     check_env(Env())
     check_rlberry_env(Env())
```

### Comparing `rlberry-0.4.0/rlberry/utils/binsearch.py` & `rlberry-0.4.1/rlberry/utils/binsearch.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.4.0/rlberry/utils/check_bandit_agent.py` & `rlberry-0.4.1/rlberry/utils/check_bandit_agent.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,16 +45,15 @@
     )
     agent2 = AgentManager(
         Agent, (env_ctor, env_kwargs), fit_budget=10, n_fit=1, seed=seed
     )
 
     agent1.fit()
     agent2.fit()
-    env = env_ctor(**env_kwargs)
-    state = env.reset()
+    state = 0
     result = True
     for _ in range(5):
         # test reproducibility on 5 actions
         action1 = agent1.agent_handlers[0].policy(state)
         action2 = agent2.agent_handlers[0].policy(state)
         if action1 != action2:
             result = False
```

### Comparing `rlberry-0.4.0/rlberry/utils/check_env.py` & `rlberry-0.4.1/rlberry/utils/check_env.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.4.0/rlberry/utils/check_gym_env.py` & `rlberry-0.4.1/rlberry/utils/check_gym_env.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.4.0/rlberry/utils/io.py` & `rlberry-0.4.1/rlberry/utils/io.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.4.0/rlberry/utils/logging.py` & `rlberry-0.4.1/rlberry/utils/logging.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.4.0/rlberry/utils/metrics.py` & `rlberry-0.4.1/rlberry/utils/metrics.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.4.0/rlberry/utils/space_discretizer.py` & `rlberry-0.4.1/rlberry/utils/space_discretizer.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.4.0/rlberry/utils/tests/test_binsearch.py` & `rlberry-0.4.1/rlberry/utils/tests/test_binsearch.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.4.0/rlberry/utils/tests/test_check.py` & `rlberry-0.4.1/rlberry/utils/tests/test_check.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.4.0/rlberry/utils/tests/test_writer.py` & `rlberry-0.4.1/rlberry/utils/tests/test_writer.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.4.0/rlberry/utils/torch.py` & `rlberry-0.4.1/rlberry/utils/torch.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.4.0/rlberry/utils/writers.py` & `rlberry-0.4.1/rlberry/utils/writers.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,14 +2,18 @@
 import pandas as pd
 from collections import deque
 from typing import Optional
 from timeit import default_timer as timer
 from rlberry import check_packages
 from rlberry import metadata_utils
 import shutil
+from tqdm import tqdm
+from tqdm.utils import _screen_shape_wrapper
+import sys
+
 
 if check_packages.TENSORBOARD_INSTALLED:
     from torch.utils.tensorboard import SummaryWriter
 
 import rlberry
 
 logger = rlberry.logger
@@ -59,15 +63,19 @@
         self._name = name
         self._print_log = print_log
         self._log_interval = log_interval
         self._execution_metadata = execution_metadata
         self._data = None
         self._time_last_log = None
         self._log_time = True
-        assert style_log in ["multi_line", "one_line"], "Style log for writer unknown."
+        assert style_log in [
+            "multi_line",
+            "one_line",
+            "progressbar",
+        ], "Style log for writer unknown."
         self._style_log = style_log
         self._maxlen = maxlen
         self._maxlen_by_tag = maxlen_by_tag
         self.reset()
 
         # initialize tensorboard
         if (tensorboard_kwargs is not None) and (
@@ -96,14 +104,19 @@
     @property
     def data(self):
         df = pd.DataFrame(columns=("name", "tag", "value", "global_step"))
         for tag in self._data:
             df = pd.concat([df, pd.DataFrame(self._data[tag])], ignore_index=True)
         return df
 
+    def set_max_global_step(self, max_global_step):
+        self._max_global_step = max_global_step
+        self.pbar = extending_tqdm(total=int(max_global_step), desc=" ", leave=False)
+        self.progressbar_current_step = 0
+
     def read_tag_value(self, tag, main_tag: str = ""):
         """
         Reads the values for the tag `tag`.
         If a `main_tag` is given, the tag will be a concatenation of
         `main_tag`, underscore and `tag`.
 
         Parameters
@@ -285,15 +298,14 @@
     def _log(self):
         # time since last log
         t_now = timer()
         time_elapsed = t_now - self._time_last_log
         # log if enough time has passed since the last log
         max_global_step = 0
         if time_elapsed > self._log_interval:
-
             self._time_last_log = t_now
             size_term = shutil.get_terminal_size().columns
 
             if self._style_log == "multi_line":
                 df = pd.DataFrame()
                 df["agent_name"] = [self._name]
                 if self._execution_metadata:
@@ -311,14 +323,15 @@
                     len(data_message[1]) < size_term - 14
                 ):
                     message = data_message[0].center(size_term - 14).rstrip() + "\n"
                     message += (
                         " " * 14 + data_message[1].center(size_term - 14).rstrip()
                     )
                     # The -14 comes from the info  message
+                    logger.info(message)
                 else:
                     self._style_log = "one_line"
             if self._style_log == "one_line":
                 self._time_last_log = t_now
                 message = ""
                 for tag in self._data:
                     val = self._data[tag]["value"][-1]
@@ -329,16 +342,51 @@
 
                 header = self._name
                 if self._execution_metadata:
                     header += f"[worker: {self._execution_metadata.obj_worker_id}]"
                 message = (
                     f"[{header}] | max_global_step = {max_global_step} | " + message
                 )
+                logger.info(message)
+
+            elif self._style_log == "progressbar":
+                self._time_last_log = t_now
+                messages = []
+                for tag in self._data:
+                    val = self._data[tag]["value"][-1]
+                    gstep = self._data[tag]["global_step"][-1]
+                    my_data = np.array(self._data[tag]["value"])
+                    if len(my_data) > 20:
+                        improvement_lag = len(my_data) // 20
+                        improvement = np.mean(my_data[-improvement_lag:]) - np.mean(
+                            my_data[-2 * improvement_lag : -improvement_lag]
+                        )
+                        windowed_std = np.std(my_data[-2 * improvement_lag :])
+                    else:
+                        improvement = np.nan
+                        windowed_std = np.nan
+                    messages += [
+                        f"{tag} = {val} (improvement over last 10%: {np.round(improvement, 4)}, std over last 10%: {np.round(windowed_std,4)})"
+                    ]
+                    if not np.isnan(gstep):
+                        max_global_step = max(max_global_step, gstep)
 
-            logger.info(message)
+                header = self._name
+                if self._execution_metadata:
+                    header += f"[worker: {self._execution_metadata.obj_worker_id}]"
+                header_msg = f"[{header}] | max_global_step = {max_global_step} |"
+                messages = [
+                    "-" * len(header_msg),
+                    header_msg,
+                    "-" * len(header_msg),
+                ] + messages
+
+                self.pbar.set_description(messages)
+                self.pbar.update(max_global_step - self.progressbar_current_step)
+                self.progressbar_current_step = max_global_step
 
     def __getattr__(self, attr):
         """
         Calls SummaryWriter methods, if self._summary_writer is not None.
         Otherwise, does nothing.
         """
         if attr[:2] == "__":
@@ -368,7 +416,50 @@
             newstate["_tensorboard_kwargs"].update(
                 dict(log_dir=newstate["_tensorboard_logdir"])
             )
             newstate["_summary_writer"] = SummaryWriter(
                 **newstate["_tensorboard_kwargs"]
             )
         self.__dict__.update(newstate)
+
+
+class extending_tqdm(tqdm):
+    def __init__(self, *args, desc="", **kwargs):
+        super().__init__(*args, **kwargs)
+        self.subbar = None
+        self.set_description(desc)
+
+    def set_description(self, desc=None, refresh=True):
+        screen_width, _ = _screen_shape_wrapper()(sys.stdout)
+        max_len = screen_width
+        if len(desc) > 1:
+            if not self.subbar:
+                self.subbar = extending_tqdm(range(len(self)))
+                self.subbar.n = self.n
+                self.default_bar_format = self.bar_format
+                self.bar_format = "{desc}"
+            desc_now = desc.pop(0)
+            super().set_description_str(
+                desc=desc_now + " " * (screen_width - len(desc_now)), refresh=refresh
+            )
+            self.subbar.set_description(desc)
+        else:
+            if self.subbar:
+                self.bar_format = self.default_bar_format
+                self.subbar.leave = False
+                self.subbar.close()
+            super().set_description(desc=" ", refresh=refresh)
+
+    def update(self, n=1):
+        if self.subbar:
+            self.subbar.update(n)
+            self.last_print_n = self.subbar.last_print_n
+            self.n = self.subbar.n
+        else:
+            super().update(n)
+
+    def close(self):
+        if self.subbar:
+            self.subbar.leave = self.leave
+            self.subbar.close()
+
+        super().close()
```

### Comparing `rlberry-0.4.0/rlberry/wrappers/autoreset.py` & `rlberry-0.4.1/rlberry/wrappers/autoreset.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.4.0/rlberry/wrappers/discrete2onehot.py` & `rlberry-0.4.1/rlberry/wrappers/discrete2onehot.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.4.0/rlberry/wrappers/discretize_state.py` & `rlberry-0.4.1/rlberry/wrappers/discretize_state.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.4.0/rlberry/wrappers/gym_utils.py` & `rlberry-0.4.1/rlberry/wrappers/gym_utils.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.4.0/rlberry/wrappers/rescale_reward.py` & `rlberry-0.4.1/rlberry/wrappers/rescale_reward.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.4.0/rlberry/wrappers/tests/test_basewrapper.py` & `rlberry-0.4.1/rlberry/wrappers/tests/test_basewrapper.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.4.0/rlberry/wrappers/tests/test_common_wrappers.py` & `rlberry-0.4.1/rlberry/wrappers/tests/test_common_wrappers.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.4.0/rlberry/wrappers/tests/test_gym_space_conversion.py` & `rlberry-0.4.1/rlberry/wrappers/tests/test_gym_space_conversion.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.4.0/rlberry/wrappers/tests/test_wrapper_seeding.py` & `rlberry-0.4.1/rlberry/wrappers/tests/test_wrapper_seeding.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.4.0/rlberry/wrappers/tests/test_writer_utils.py` & `rlberry-0.4.1/rlberry/wrappers/tests/test_writer_utils.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.4.0/rlberry/wrappers/uncertainty_estimator_wrapper.py` & `rlberry-0.4.1/rlberry/wrappers/uncertainty_estimator_wrapper.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.4.0/rlberry/wrappers/vis2d.py` & `rlberry-0.4.1/rlberry/wrappers/vis2d.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.4.0/rlberry/wrappers/writer_utils.py` & `rlberry-0.4.1/rlberry/wrappers/writer_utils.py`

 * *Files identical despite different names*

### Comparing `rlberry-0.4.0/rlberry.egg-info/PKG-INFO` & `rlberry-0.4.1/rlberry.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,54 +1,54 @@
 Metadata-Version: 2.1
 Name: rlberry
-Version: 0.4.0
+Version: 0.4.1
 Summary: An easy-to-use reinforcement learning library for research and education
 Home-page: https://github.com/rlberry-py
 Author: Omar Darwiche Domingues, Yannis Flet-Berliac, Edouard Leurent, Pierre Menard, Xuedong Shang
 License: MIT
+Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Education
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 Provides-Extra: default
+Provides-Extra: deploy
 Provides-Extra: jax_agents
 Provides-Extra: torch_agents
-Provides-Extra: deploy
 License-File: LICENSE
 
 <!-- Logo -->
 <p align="center">
    <img src="https://raw.githubusercontent.com/rlberry-py/rlberry/main/assets/logo_wide.svg" width="50%">
 </p>
 
 
+
 <!-- Short description -->
 <p align="center">
    A Reinforcement Learning Library for Research and Education
 </p>
 
+
 <!-- The badges -->
 <p align="center">
    <a href="https://github.com/rlberry-py/rlberry/workflows/test/badge.svg">
       <img alt="pytest" src="https://github.com/rlberry-py/rlberry/workflows/test/badge.svg">
    </a>
    <a href='https://rlberry.readthedocs.io/en/latest/?badge=latest'>
       <img alt="Documentation Status" src="https://readthedocs.org/projects/rlberry/badge/?version=latest">
    </a>
    <a href="https://img.shields.io/github/contributors/rlberry-py/rlberry">
       <img alt="contributors" src="https://img.shields.io/github/contributors/rlberry-py/rlberry">
    </a>
-   <a href="https://app.codacy.com/gh/rlberry-py/rlberry?utm_source=github.com&utm_medium=referral&utm_content=rlberry-py/rlberry&utm_campaign=Badge_Grade">
-      <img alt="Codacy" src="https://api.codacy.com/project/badge/Grade/27e91674d18a4ac49edf91c339af1502">
-   </a>
    <a href="https://codecov.io/gh/rlberry-py/rlberry">
       <img alt="codecov" src="https://codecov.io/gh/rlberry-py/rlberry/branch/main/graph/badge.svg?token=TIFP7RUD75">
      </a>
 </p>
 
 <p align="center">
    <!-- <a href="https://img.shields.io/pypi/pyversions/rlberry">
@@ -142,11 +142,18 @@
 
 The modules listed below are experimental at the moment, that is, they are not thoroughly tested and are susceptible to evolve.
 
 * `rlberry.network`: Allows communication between a server and client via sockets, and can be used to run agents remotely.
 * `rlberry.agents.experimental`: Experimental agents that are not thoroughly tested.
 
 
+## About us
+This project was initiated and is actively maintained by [INRIA SCOOL team](https://team.inria.fr/scool/).
+More information [here](https://rlberry.readthedocs.io/en/latest/about.html#).
+
+
 ## Contributing
 
 Want to contribute to `rlberry`? Please check [our contribution guidelines](https://rlberry.readthedocs.io/en/latest/contributing.html). **If you want to add any new agents or environments, do not hesitate
 to [open an issue](https://github.com/rlberry-py/rlberry/issues/new/choose)!**
+
+
```

#### html2text {}

```diff
@@ -1,23 +1,23 @@
-Metadata-Version: 2.1 Name: rlberry Version: 0.4.0 Summary: An easy-to-use
+Metadata-Version: 2.1 Name: rlberry Version: 0.4.1 Summary: An easy-to-use
 reinforcement learning library for research and education Home-page: https://
 github.com/rlberry-py Author: Omar Darwiche Domingues, Yannis Flet-Berliac,
-Edouard Leurent, Pierre Menard, Xuedong Shang License: MIT Classifier:
-Development Status :: 4 - Beta Classifier: Intended Audience :: Science/
-Research Classifier: Intended Audience :: Education Classifier: Topic ::
-Scientific/Engineering :: Artificial Intelligence Classifier: Programming
+Edouard Leurent, Pierre Menard, Xuedong Shang License: MIT Platform: UNKNOWN
+Classifier: Development Status :: 4 - Beta Classifier: Intended Audience ::
+Science/Research Classifier: Intended Audience :: Education Classifier: Topic
+:: Scientific/Engineering :: Artificial Intelligence Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3 ::
 Only Classifier: License :: OSI Approved :: MIT License Classifier: Operating
 System :: OS Independent Description-Content-Type: text/markdown Provides-
-Extra: default Provides-Extra: jax_agents Provides-Extra: torch_agents
-Provides-Extra: deploy License-File: LICENSE
+Extra: default Provides-Extra: deploy Provides-Extra: jax_agents Provides-
+Extra: torch_agents License-File: LICENSE
       [https://raw.githubusercontent.com/rlberry-py/rlberry/main/assets/
                                 logo_wide.svg]
           A Reinforcement Learning Library for Research and Education
-       [pytest] [Documentation_Status] [contributors] [Codacy] [codecov]
+           [pytest] [Documentation_Status] [contributors] [codecov]
 
                     Try_it_on_Google_Colab!_[Open_In_Colab]
 
 ===============================================================================
  ## What is `rlberry`? **Writing reinforcement learning algorithms is fun!**
 *But after the fun, we have lots of boring things to implement*: run our agents
 in parallel, average and plot results, optimize hyperparameters, compare to
@@ -48,12 +48,14 @@
 Valko, Michal}, doi = {10.5281/zenodo.5544540}, month = {10}, title = {{rlberry
 - A Reinforcement Learning Library for Research and Education}}, url = {https:/
 /github.com/rlberry-py/rlberry}, year = {2021} } ``` ## Development notes The
 modules listed below are experimental at the moment, that is, they are not
 thoroughly tested and are susceptible to evolve. * `rlberry.network`: Allows
 communication between a server and client via sockets, and can be used to run
 agents remotely. * `rlberry.agents.experimental`: Experimental agents that are
-not thoroughly tested. ## Contributing Want to contribute to `rlberry`? Please
-check [our contribution guidelines](https://rlberry.readthedocs.io/en/latest/
-contributing.html). **If you want to add any new agents or environments, do not
-hesitate to [open an issue](https://github.com/rlberry-py/rlberry/issues/new/
-choose)!**
+not thoroughly tested. ## About us This project was initiated and is actively
+maintained by [INRIA SCOOL team](https://team.inria.fr/scool/). More
+information [here](https://rlberry.readthedocs.io/en/latest/about.html#). ##
+Contributing Want to contribute to `rlberry`? Please check [our contribution
+guidelines](https://rlberry.readthedocs.io/en/latest/contributing.html). **If
+you want to add any new agents or environments, do not hesitate to [open an
+issue](https://github.com/rlberry-py/rlberry/issues/new/choose)!**
```

### Comparing `rlberry-0.4.0/rlberry.egg-info/SOURCES.txt` & `rlberry-0.4.1/rlberry.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -31,29 +31,17 @@
 rlberry/agents/bandits/ts_agents.py
 rlberry/agents/bandits/tools/__init__.py
 rlberry/agents/bandits/tools/tracker.py
 rlberry/agents/dynprog/__init__.py
 rlberry/agents/dynprog/utils.py
 rlberry/agents/dynprog/value_iteration.py
 rlberry/agents/experimental/__init__.py
-rlberry/agents/experimental/jax/__init__.py
-rlberry/agents/experimental/jax/dqn/__init__.py
-rlberry/agents/experimental/jax/dqn/dqn.py
-rlberry/agents/experimental/jax/nets/__init__.py
-rlberry/agents/experimental/jax/nets/common.py
-rlberry/agents/experimental/jax/tests/__init__.py
-rlberry/agents/experimental/jax/tests/old_test_tqn.py
-rlberry/agents/experimental/jax/utils/__init__.py
-rlberry/agents/experimental/jax/utils/replay_buffer.py
 rlberry/agents/experimental/tests/__init__.py
-rlberry/agents/experimental/tests/test_actor_critic.py
 rlberry/agents/experimental/tests/test_sac.py
 rlberry/agents/experimental/torch/__init__.py
-rlberry/agents/experimental/torch/avec/__init__.py
-rlberry/agents/experimental/torch/avec/avec_ppo.py
 rlberry/agents/experimental/torch/sac/__init__.py
 rlberry/agents/experimental/torch/sac/sac.py
 rlberry/agents/experimental/torch/sac/utils.py
 rlberry/agents/features/__init__.py
 rlberry/agents/features/feature_map.py
 rlberry/agents/kernel_based/__init__.py
 rlberry/agents/kernel_based/common.py
@@ -68,49 +56,54 @@
 rlberry/agents/optql/optql.py
 rlberry/agents/psrl/__init__.py
 rlberry/agents/psrl/psrl.py
 rlberry/agents/rlsvi/__init__.py
 rlberry/agents/rlsvi/rlsvi.py
 rlberry/agents/stable_baselines/__init__.py
 rlberry/agents/stable_baselines/stable_baselines.py
+rlberry/agents/tabular_rl/__init__.py
+rlberry/agents/tabular_rl/qlearning.py
+rlberry/agents/tabular_rl/sarsa.py
 rlberry/agents/tests/__init__.py
 rlberry/agents/tests/test_adaptiveql.py
 rlberry/agents/tests/test_bandits.py
 rlberry/agents/tests/test_dynprog.py
 rlberry/agents/tests/test_kernel_based.py
 rlberry/agents/tests/test_lsvi_ucb.py
 rlberry/agents/tests/test_mbqvi.py
 rlberry/agents/tests/test_optql.py
 rlberry/agents/tests/test_psrl.py
 rlberry/agents/tests/test_replay.py
 rlberry/agents/tests/test_rlsvi.py
 rlberry/agents/tests/test_stable_baselines.py
+rlberry/agents/tests/test_tabular_rl.py
 rlberry/agents/tests/test_ucbvi.py
 rlberry/agents/torch/__init__.py
 rlberry/agents/torch/a2c/__init__.py
 rlberry/agents/torch/a2c/a2c.py
 rlberry/agents/torch/dqn/__init__.py
 rlberry/agents/torch/dqn/dqn.py
 rlberry/agents/torch/dqn/dqn_utils.py
 rlberry/agents/torch/dqn/mdqn.py
 rlberry/agents/torch/ppo/__init__.py
 rlberry/agents/torch/ppo/ppo.py
+rlberry/agents/torch/ppo/ppo_utils.py
 rlberry/agents/torch/reinforce/__init__.py
 rlberry/agents/torch/reinforce/reinforce.py
 rlberry/agents/torch/tests/__init__.py
 rlberry/agents/torch/tests/test_a2c.py
 rlberry/agents/torch/tests/test_dqn.py
 rlberry/agents/torch/tests/test_factory.py
 rlberry/agents/torch/tests/test_mdqn.py
 rlberry/agents/torch/tests/test_ppo.py
 rlberry/agents/torch/tests/test_reinforce.py
+rlberry/agents/torch/tests/test_torch_atari.py
 rlberry/agents/torch/tests/test_torch_models.py
 rlberry/agents/torch/tests/test_torch_training.py
 rlberry/agents/torch/utils/__init__.py
-rlberry/agents/torch/utils/attention_models.py
 rlberry/agents/torch/utils/models.py
 rlberry/agents/torch/utils/training.py
 rlberry/agents/ucbvi/__init__.py
 rlberry/agents/ucbvi/ucbvi.py
 rlberry/agents/ucbvi/utils.py
 rlberry/agents/utils/__init__.py
 rlberry/agents/utils/memories.py
@@ -185,14 +178,17 @@
 rlberry/manager/tests/test_shared_data.py
 rlberry/network/__init__.py
 rlberry/network/client.py
 rlberry/network/interface.py
 rlberry/network/server.py
 rlberry/network/server_utils.py
 rlberry/network/utils.py
+rlberry/network/tests/__init__.py
+rlberry/network/tests/conftest.py
+rlberry/network/tests/test_server.py
 rlberry/rendering/__init__.py
 rlberry/rendering/common_shapes.py
 rlberry/rendering/core.py
 rlberry/rendering/opengl_render2d.py
 rlberry/rendering/pygame_render2d.py
 rlberry/rendering/render_interface.py
 rlberry/rendering/utils.py
@@ -213,15 +209,16 @@
 rlberry/spaces/multi_binary.py
 rlberry/spaces/multi_discrete.py
 rlberry/spaces/tuple.py
 rlberry/spaces/tests/__init__.py
 rlberry/spaces/tests/test_from_gym.py
 rlberry/spaces/tests/test_spaces.py
 rlberry/tests/__init__.py
-rlberry/tests/test_agent.py
+rlberry/tests/test_agent_extra.py
+rlberry/tests/test_agents_base.py
 rlberry/tests/test_envs.py
 rlberry/utils/__init__.py
 rlberry/utils/binsearch.py
 rlberry/utils/check_agent.py
 rlberry/utils/check_bandit_agent.py
 rlberry/utils/check_env.py
 rlberry/utils/check_gym_env.py
@@ -236,14 +233,15 @@
 rlberry/utils/writers.py
 rlberry/utils/tests/__init__.py
 rlberry/utils/tests/test_binsearch.py
 rlberry/utils/tests/test_check.py
 rlberry/utils/tests/test_metrics.py
 rlberry/utils/tests/test_writer.py
 rlberry/wrappers/__init__.py
+rlberry/wrappers/atari_utils.py
 rlberry/wrappers/autoreset.py
 rlberry/wrappers/discrete2onehot.py
 rlberry/wrappers/discretize_state.py
 rlberry/wrappers/gym_utils.py
 rlberry/wrappers/rescale_reward.py
 rlberry/wrappers/scalarize.py
 rlberry/wrappers/uncertainty_estimator_wrapper.py
```

### Comparing `rlberry-0.4.0/setup.py` & `rlberry-0.4.1/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -10,19 +10,20 @@
 
 #
 # Base installation (interface only)
 #
 install_requires = [
     "numpy>=1.17",
     "scipy>=1.6",
-    "pygame",
+    "pygame-ce",
     "matplotlib",
     "seaborn",
     "pandas",
-    "gym",
+    #"gym[accept-rom-license] @ git+https://github.com/rlberry-py/gym_fix_021",
+    "gym[accept-rom-license]==0.21",
     "dill",
     "docopt",
     "pyyaml",
 ]
 
 #
 # Extras
@@ -38,14 +39,16 @@
     "pyvirtualdisplay",
 ]
 
 # tensorboard must be installed manually, due to conflicts with
 # dm-reverb-nightly[tensorflow] in jax_agents_requires
 torch_agents_requires = default_requires + [
     "torch>=1.6.0",
+    "opencv-python",
+    "ale-py==0.7.4",
     # 'tensorboard'
 ]
 
 jax_agents_requires = default_requires + [
     "jax[cpu]",
     "chex",
     "dm-haiku",
```

