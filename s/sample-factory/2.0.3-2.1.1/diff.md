# Comparing `tmp/sample-factory-2.0.3.tar.gz` & `tmp/sample-factory-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sample-factory-2.0.3.tar", last modified: Thu Feb  9 10:46:32 2023, max compression
+gzip compressed data, was "sample-factory-2.1.1.tar", last modified: Mon Jun 19 08:22:20 2023, max compression
```

## Comparing `sample-factory-2.0.3.tar` & `sample-factory-2.1.1.tar`

### file list

```diff
@@ -1,351 +1,350 @@
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-02-09 10:46:32.390088 sample-factory-2.0.3/
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-02-09 10:46:32.334090 sample-factory-2.0.3/.pytest_cache/
--rw-rw-r--   0 alex      (1000) alex      (1000)      302 2022-11-25 02:37:22.000000 sample-factory-2.0.3/.pytest_cache/README.md
--rw-rw-r--   0 alex      (1000) alex      (1000)     3193 2022-12-07 00:16:21.000000 sample-factory-2.0.3/CONTRIBUTING.md
--rw-rw-r--   0 alex      (1000) alex      (1000)     1073 2022-03-11 21:44:47.000000 sample-factory-2.0.3/LICENSE
--rw-rw-r--   0 alex      (1000) alex      (1000)      118 2022-12-07 00:16:21.000000 sample-factory-2.0.3/MANIFEST.in
--rw-rw-r--   0 alex      (1000) alex      (1000)    10876 2023-02-09 10:46:32.390088 sample-factory-2.0.3/PKG-INFO
--rw-rw-r--   0 alex      (1000) alex      (1000)    11167 2023-01-12 23:57:40.000000 sample-factory-2.0.3/README.md
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-02-09 10:46:32.334090 sample-factory-2.0.3/docs/
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-02-09 10:46:32.334090 sample-factory-2.0.3/docs/01-get-started/
--rw-rw-r--   0 alex      (1000) alex      (1000)     1412 2022-12-07 00:16:21.000000 sample-factory-2.0.3/docs/01-get-started/basic-usage.md
--rw-rw-r--   0 alex      (1000) alex      (1000)     1160 2022-12-07 00:16:21.000000 sample-factory-2.0.3/docs/01-get-started/installation.md
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-02-09 10:46:32.334090 sample-factory-2.0.3/docs/02-configuration/
--rw-rw-r--   0 alex      (1000) alex      (1000)    40759 2023-01-12 23:57:40.000000 sample-factory-2.0.3/docs/02-configuration/cfg-params.md
--rw-rw-r--   0 alex      (1000) alex      (1000)     5037 2022-12-07 00:16:21.000000 sample-factory-2.0.3/docs/02-configuration/configuration.md
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-02-09 10:46:32.334090 sample-factory-2.0.3/docs/03-customization/
--rw-rw-r--   0 alex      (1000) alex      (1000)     5640 2023-01-12 23:57:40.000000 sample-factory-2.0.3/docs/03-customization/custom-environments.md
--rw-rw-r--   0 alex      (1000) alex      (1000)     4194 2022-12-07 00:16:21.000000 sample-factory-2.0.3/docs/03-customization/custom-models.md
--rw-rw-r--   0 alex      (1000) alex      (1000)     2378 2022-12-07 00:16:21.000000 sample-factory-2.0.3/docs/03-customization/custom-multi-agent-environments.md
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-02-09 10:46:32.334090 sample-factory-2.0.3/docs/04-experiments/
--rw-rw-r--   0 alex      (1000) alex      (1000)    11233 2023-01-10 07:03:14.000000 sample-factory-2.0.3/docs/04-experiments/experiment-launcher.md
--rw-rw-r--   0 alex      (1000) alex      (1000)     3028 2022-12-07 00:16:21.000000 sample-factory-2.0.3/docs/04-experiments/slurm-details.md
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-02-09 10:46:32.334090 sample-factory-2.0.3/docs/05-monitoring/
--rw-rw-r--   0 alex      (1000) alex      (1000)      912 2022-12-07 00:16:21.000000 sample-factory-2.0.3/docs/05-monitoring/custom-metrics.md
--rw-rw-r--   0 alex      (1000) alex      (1000)     8412 2022-12-07 00:16:21.000000 sample-factory-2.0.3/docs/05-monitoring/metrics-reference.md
--rw-rw-r--   0 alex      (1000) alex      (1000)      922 2022-12-07 00:16:21.000000 sample-factory-2.0.3/docs/05-monitoring/tensorboard.md
--rw-rw-r--   0 alex      (1000) alex      (1000)     1309 2022-12-07 00:16:21.000000 sample-factory-2.0.3/docs/05-monitoring/wandb.md
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-02-09 10:46:32.334090 sample-factory-2.0.3/docs/06-architecture/
--rw-rw-r--   0 alex      (1000) alex      (1000)     3219 2022-12-07 00:16:21.000000 sample-factory-2.0.3/docs/06-architecture/message-passing.md
--rw-rw-r--   0 alex      (1000) alex      (1000)     6395 2022-12-07 00:16:21.000000 sample-factory-2.0.3/docs/06-architecture/overview.md
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-02-09 10:46:32.338090 sample-factory-2.0.3/docs/07-advanced-topics/
--rw-rw-r--   0 alex      (1000) alex      (1000)     2406 2022-12-07 00:16:21.000000 sample-factory-2.0.3/docs/07-advanced-topics/batched-non-batched.md
--rw-rw-r--   0 alex      (1000) alex      (1000)     1165 2022-12-07 00:16:21.000000 sample-factory-2.0.3/docs/07-advanced-topics/double-buffered.md
--rw-rw-r--   0 alex      (1000) alex      (1000)     1708 2022-12-07 00:16:21.000000 sample-factory-2.0.3/docs/07-advanced-topics/inactive-agents.md
--rw-rw-r--   0 alex      (1000) alex      (1000)     2875 2022-12-07 00:16:21.000000 sample-factory-2.0.3/docs/07-advanced-topics/multi-policy-training.md
--rw-rw-r--   0 alex      (1000) alex      (1000)     2122 2022-12-07 00:16:21.000000 sample-factory-2.0.3/docs/07-advanced-topics/normalizations.md
--rw-rw-r--   0 alex      (1000) alex      (1000)     1578 2022-12-07 00:16:21.000000 sample-factory-2.0.3/docs/07-advanced-topics/observer.md
--rw-rw-r--   0 alex      (1000) alex      (1000)     2710 2022-12-07 00:16:21.000000 sample-factory-2.0.3/docs/07-advanced-topics/passing-info.md
--rw-rw-r--   0 alex      (1000) alex      (1000)     7249 2022-12-07 00:16:21.000000 sample-factory-2.0.3/docs/07-advanced-topics/pbt.md
--rw-rw-r--   0 alex      (1000) alex      (1000)     4982 2022-12-07 00:16:21.000000 sample-factory-2.0.3/docs/07-advanced-topics/policy-lag.md
--rw-rw-r--   0 alex      (1000) alex      (1000)     9675 2022-12-07 00:16:21.000000 sample-factory-2.0.3/docs/07-advanced-topics/profiling.md
--rw-rw-r--   0 alex      (1000) alex      (1000)     1105 2022-12-07 00:16:21.000000 sample-factory-2.0.3/docs/07-advanced-topics/serial-mode.md
--rw-rw-r--   0 alex      (1000) alex      (1000)     3556 2022-12-07 00:16:21.000000 sample-factory-2.0.3/docs/07-advanced-topics/sync-async.md
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-02-09 10:46:32.338090 sample-factory-2.0.3/docs/08-miscellaneous/
--rw-rw-r--   0 alex      (1000) alex      (1000)     1098 2022-12-07 00:16:21.000000 sample-factory-2.0.3/docs/08-miscellaneous/tests.md
--rw-rw-r--   0 alex      (1000) alex      (1000)     1652 2022-12-07 00:16:21.000000 sample-factory-2.0.3/docs/08-miscellaneous/v1-to-v2.md
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-02-09 10:46:32.338090 sample-factory-2.0.3/docs/09-environment-integrations/
--rw-rw-r--   0 alex      (1000) alex      (1000)    12045 2022-12-07 00:16:21.000000 sample-factory-2.0.3/docs/09-environment-integrations/atari.md
--rw-rw-r--   0 alex      (1000) alex      (1000)     3951 2023-01-12 23:57:40.000000 sample-factory-2.0.3/docs/09-environment-integrations/brax.md
--rw-rw-r--   0 alex      (1000) alex      (1000)     3585 2022-12-07 00:16:21.000000 sample-factory-2.0.3/docs/09-environment-integrations/dmlab.md
--rw-rw-r--   0 alex      (1000) alex      (1000)     1857 2022-12-30 04:35:22.000000 sample-factory-2.0.3/docs/09-environment-integrations/envpool.md
--rw-rw-r--   0 alex      (1000) alex      (1000)     3008 2022-12-07 00:16:21.000000 sample-factory-2.0.3/docs/09-environment-integrations/isaacgym.md
--rw-rw-r--   0 alex      (1000) alex      (1000)     3305 2022-12-07 00:16:21.000000 sample-factory-2.0.3/docs/09-environment-integrations/megaverse.md
--rw-rw-r--   0 alex      (1000) alex      (1000)     5943 2022-12-07 00:16:21.000000 sample-factory-2.0.3/docs/09-environment-integrations/mujoco.md
--rw-rw-r--   0 alex      (1000) alex      (1000)     2587 2022-12-07 00:16:21.000000 sample-factory-2.0.3/docs/09-environment-integrations/swarm-rl.md
--rw-rw-r--   0 alex      (1000) alex      (1000)     9019 2022-12-07 00:16:21.000000 sample-factory-2.0.3/docs/09-environment-integrations/vizdoom.md
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-02-09 10:46:32.338090 sample-factory-2.0.3/docs/10-huggingface/
--rw-rw-r--   0 alex      (1000) alex      (1000)     4502 2023-01-12 04:15:35.000000 sample-factory-2.0.3/docs/10-huggingface/huggingface.md
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-02-09 10:46:32.338090 sample-factory-2.0.3/docs/11-release-notes/
--rw-rw-r--   0 alex      (1000) alex      (1000)     3612 2023-01-13 00:06:49.000000 sample-factory-2.0.3/docs/11-release-notes/release-notes.md
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-02-09 10:46:32.338090 sample-factory-2.0.3/docs/12-community/
--rw-rw-r--   0 alex      (1000) alex      (1000)     1081 2023-01-12 23:57:40.000000 sample-factory-2.0.3/docs/12-community/citation.md
--rw-rw-r--   0 alex      (1000) alex      (1000)     3181 2023-02-08 12:17:21.000000 sample-factory-2.0.3/docs/12-community/contribution.md
--rw-rw-r--   0 alex      (1000) alex      (1000)     1009 2022-12-07 00:16:21.000000 sample-factory-2.0.3/docs/12-community/doc-contribution.md
--rw-rw-r--   0 alex      (1000) alex      (1000)      680 2022-12-07 00:16:21.000000 sample-factory-2.0.3/docs/cfg-params.sh
--rw-rw-r--   0 alex      (1000) alex      (1000)     5203 2023-01-12 23:57:40.000000 sample-factory-2.0.3/docs/index.md
--rw-rw-r--   0 alex      (1000) alex      (1000)      279 2022-12-07 00:16:21.000000 sample-factory-2.0.3/pyproject.toml
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-02-09 10:46:32.338090 sample-factory-2.0.3/sample_factory/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-12-07 00:16:21.000000 sample-factory-2.0.3/sample_factory/__init__.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-02-09 10:46:32.338090 sample-factory-2.0.3/sample_factory/algo/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-12-07 00:16:21.000000 sample-factory-2.0.3/sample_factory/algo/__init__.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-02-09 10:46:32.338090 sample-factory-2.0.3/sample_factory/algo/learning/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-12-07 00:16:21.000000 sample-factory-2.0.3/sample_factory/algo/learning/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    11329 2022-12-07 00:16:21.000000 sample-factory-2.0.3/sample_factory/algo/learning/batcher.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    48171 2023-02-07 04:00:17.000000 sample-factory-2.0.3/sample_factory/algo/learning/learner.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     5747 2022-12-07 00:16:21.000000 sample-factory-2.0.3/sample_factory/algo/learning/learner_worker.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     6962 2022-12-07 00:16:21.000000 sample-factory-2.0.3/sample_factory/algo/learning/rnn_utils.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-02-09 10:46:32.342090 sample-factory-2.0.3/sample_factory/algo/runners/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-12-07 00:16:21.000000 sample-factory-2.0.3/sample_factory/algo/runners/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    32869 2022-12-30 04:35:22.000000 sample-factory-2.0.3/sample_factory/algo/runners/runner.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     2369 2022-12-07 00:16:21.000000 sample-factory-2.0.3/sample_factory/algo/runners/runner_parallel.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1154 2022-12-07 00:16:21.000000 sample-factory-2.0.3/sample_factory/algo/runners/runner_serial.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-02-09 10:46:32.342090 sample-factory-2.0.3/sample_factory/algo/sampling/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-12-07 00:16:21.000000 sample-factory-2.0.3/sample_factory/algo/sampling/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    17440 2022-12-07 00:16:21.000000 sample-factory-2.0.3/sample_factory/algo/sampling/batched_sampling.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    16896 2023-01-17 01:01:28.000000 sample-factory-2.0.3/sample_factory/algo/sampling/inference_worker.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    31340 2022-12-30 04:35:22.000000 sample-factory-2.0.3/sample_factory/algo/sampling/non_batched_sampling.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    14921 2022-12-07 00:16:21.000000 sample-factory-2.0.3/sample_factory/algo/sampling/rollout_worker.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    12946 2022-12-07 00:16:21.000000 sample-factory-2.0.3/sample_factory/algo/sampling/sampler.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     2773 2022-12-07 00:16:21.000000 sample-factory-2.0.3/sample_factory/algo/sampling/sampling_utils.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     8361 2022-12-07 00:16:21.000000 sample-factory-2.0.3/sample_factory/algo/sampling/simplified_sampling_api.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-02-09 10:46:32.342090 sample-factory-2.0.3/sample_factory/algo/utils/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-12-07 00:16:21.000000 sample-factory-2.0.3/sample_factory/algo/utils/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    10764 2022-12-30 04:27:45.000000 sample-factory-2.0.3/sample_factory/algo/utils/action_distributions.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     2839 2022-12-07 00:16:21.000000 sample-factory-2.0.3/sample_factory/algo/utils/agent_policy_mapping.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1022 2022-12-07 00:16:21.000000 sample-factory-2.0.3/sample_factory/algo/utils/context.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     4855 2022-12-07 00:16:21.000000 sample-factory-2.0.3/sample_factory/algo/utils/env_info.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1186 2022-12-07 00:16:21.000000 sample-factory-2.0.3/sample_factory/algo/utils/heartbeat.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    15434 2022-12-07 00:16:21.000000 sample-factory-2.0.3/sample_factory/algo/utils/make_env.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1086 2022-12-07 00:16:21.000000 sample-factory-2.0.3/sample_factory/algo/utils/misc.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     6051 2022-12-07 00:16:21.000000 sample-factory-2.0.3/sample_factory/algo/utils/model_sharing.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      886 2022-12-07 00:16:21.000000 sample-factory-2.0.3/sample_factory/algo/utils/multiprocessing_utils.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     6225 2022-12-07 00:16:21.000000 sample-factory-2.0.3/sample_factory/algo/utils/optimizers.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     3805 2022-12-30 04:27:45.000000 sample-factory-2.0.3/sample_factory/algo/utils/rl_utils.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     5893 2023-01-19 02:26:09.000000 sample-factory-2.0.3/sample_factory/algo/utils/running_mean_std.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    11118 2022-12-07 00:16:21.000000 sample-factory-2.0.3/sample_factory/algo/utils/shared_buffers.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-02-09 10:46:32.342090 sample-factory-2.0.3/sample_factory/algo/utils/spaces/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-12-07 00:16:21.000000 sample-factory-2.0.3/sample_factory/algo/utils/spaces/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      443 2022-12-07 00:16:21.000000 sample-factory-2.0.3/sample_factory/algo/utils/spaces/discretized.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     5277 2022-12-07 00:16:21.000000 sample-factory-2.0.3/sample_factory/algo/utils/tensor_dict.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1081 2022-12-07 00:16:21.000000 sample-factory-2.0.3/sample_factory/algo/utils/tensor_utils.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1741 2022-12-30 04:27:45.000000 sample-factory-2.0.3/sample_factory/algo/utils/torch_utils.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-02-09 10:46:32.342090 sample-factory-2.0.3/sample_factory/cfg/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-12-07 00:16:21.000000 sample-factory-2.0.3/sample_factory/cfg/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    10766 2023-01-12 04:15:35.000000 sample-factory-2.0.3/sample_factory/cfg/arguments.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    35663 2023-01-12 23:57:40.000000 sample-factory-2.0.3/sample_factory/cfg/cfg.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      146 2022-12-07 00:16:21.000000 sample-factory-2.0.3/sample_factory/cfg/configurable.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    11340 2023-01-12 23:57:40.000000 sample-factory-2.0.3/sample_factory/enjoy.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-02-09 10:46:32.342090 sample-factory-2.0.3/sample_factory/envs/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-12-07 00:16:21.000000 sample-factory-2.0.3/sample_factory/envs/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1400 2022-12-07 00:16:21.000000 sample-factory-2.0.3/sample_factory/envs/create_env.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     5247 2022-12-07 00:16:21.000000 sample-factory-2.0.3/sample_factory/envs/env_utils.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    15577 2022-12-07 00:16:21.000000 sample-factory-2.0.3/sample_factory/envs/env_wrappers.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-02-09 10:46:32.342090 sample-factory-2.0.3/sample_factory/huggingface/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-12-07 00:16:21.000000 sample-factory-2.0.3/sample_factory/huggingface/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     4762 2023-01-12 23:57:40.000000 sample-factory-2.0.3/sample_factory/huggingface/huggingface_utils.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      669 2022-12-07 00:16:21.000000 sample-factory-2.0.3/sample_factory/huggingface/load_from_hub.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1884 2023-01-12 04:15:35.000000 sample-factory-2.0.3/sample_factory/huggingface/push_to_hub.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-02-09 10:46:32.346090 sample-factory-2.0.3/sample_factory/launcher/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-12-07 00:16:21.000000 sample-factory-2.0.3/sample_factory/launcher/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      154 2022-12-07 00:16:21.000000 sample-factory-2.0.3/sample_factory/launcher/launcher_utils.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     2742 2022-12-07 00:16:21.000000 sample-factory-2.0.3/sample_factory/launcher/run.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     7490 2023-01-12 23:57:40.000000 sample-factory-2.0.3/sample_factory/launcher/run_description.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     2289 2022-12-07 00:16:21.000000 sample-factory-2.0.3/sample_factory/launcher/run_ngc.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     5474 2022-12-07 00:16:21.000000 sample-factory-2.0.3/sample_factory/launcher/run_processes.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     4558 2022-12-07 00:16:21.000000 sample-factory-2.0.3/sample_factory/launcher/run_slurm.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-02-09 10:46:32.346090 sample-factory-2.0.3/sample_factory/launcher/slurm/
--rw-rw-r--   0 alex      (1000) alex      (1000)      210 2022-12-07 00:16:21.000000 sample-factory-2.0.3/sample_factory/launcher/slurm/sbatch_timeout.sh
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-02-09 10:46:32.346090 sample-factory-2.0.3/sample_factory/model/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-12-07 00:16:21.000000 sample-factory-2.0.3/sample_factory/model/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     3046 2023-02-07 04:00:33.000000 sample-factory-2.0.3/sample_factory/model/action_parameterization.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    12744 2023-02-07 04:00:29.000000 sample-factory-2.0.3/sample_factory/model/actor_critic.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     2656 2022-12-07 00:16:21.000000 sample-factory-2.0.3/sample_factory/model/core.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1081 2022-12-30 04:27:45.000000 sample-factory-2.0.3/sample_factory/model/decoder.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     8946 2023-02-07 04:01:04.000000 sample-factory-2.0.3/sample_factory/model/encoder.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     2948 2022-12-07 00:16:21.000000 sample-factory-2.0.3/sample_factory/model/model_factory.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1886 2022-12-07 00:16:21.000000 sample-factory-2.0.3/sample_factory/model/model_utils.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-02-09 10:46:32.346090 sample-factory-2.0.3/sample_factory/pbt/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-12-07 00:16:21.000000 sample-factory-2.0.3/sample_factory/pbt/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    18221 2022-12-07 00:16:21.000000 sample-factory-2.0.3/sample_factory/pbt/population_based_training.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1342 2022-12-07 00:16:21.000000 sample-factory-2.0.3/sample_factory/train.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-02-09 10:46:32.346090 sample-factory-2.0.3/sample_factory/utils/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-12-07 00:16:21.000000 sample-factory-2.0.3/sample_factory/utils/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      208 2023-01-12 23:57:40.000000 sample-factory-2.0.3/sample_factory/utils/algo_version.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      215 2022-12-07 00:16:21.000000 sample-factory-2.0.3/sample_factory/utils/attr_dict.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1607 2022-12-07 00:16:21.000000 sample-factory-2.0.3/sample_factory/utils/decay.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     2983 2022-12-07 00:16:21.000000 sample-factory-2.0.3/sample_factory/utils/dicts.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      986 2022-12-07 00:16:21.000000 sample-factory-2.0.3/sample_factory/utils/get_available_gpus.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      953 2022-12-07 00:16:21.000000 sample-factory-2.0.3/sample_factory/utils/gifs.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     3428 2023-01-16 04:58:36.000000 sample-factory-2.0.3/sample_factory/utils/gpu_utils.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      361 2022-12-07 00:16:21.000000 sample-factory-2.0.3/sample_factory/utils/network.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     3115 2022-12-07 00:16:21.000000 sample-factory-2.0.3/sample_factory/utils/normalize.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)     2930 2022-12-07 00:16:21.000000 sample-factory-2.0.3/sample_factory/utils/tb.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     4970 2022-12-07 00:16:21.000000 sample-factory-2.0.3/sample_factory/utils/timing.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      771 2022-12-07 00:16:21.000000 sample-factory-2.0.3/sample_factory/utils/typing.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    13850 2023-01-12 04:15:35.000000 sample-factory-2.0.3/sample_factory/utils/utils.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1774 2022-12-07 00:16:21.000000 sample-factory-2.0.3/sample_factory/utils/wandb_utils.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-02-09 10:46:32.338090 sample-factory-2.0.3/sample_factory.egg-info/
--rw-rw-r--   0 alex      (1000) alex      (1000)    10876 2023-02-09 10:46:32.000000 sample-factory-2.0.3/sample_factory.egg-info/PKG-INFO
--rw-rw-r--   0 alex      (1000) alex      (1000)    12325 2023-02-09 10:46:32.000000 sample-factory-2.0.3/sample_factory.egg-info/SOURCES.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)        1 2023-02-09 10:46:32.000000 sample-factory-2.0.3/sample_factory.egg-info/dependency_links.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)      657 2023-02-09 10:46:32.000000 sample-factory-2.0.3/sample_factory.egg-info/requires.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)       27 2023-02-09 10:46:32.000000 sample-factory-2.0.3/sample_factory.egg-info/top_level.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)       38 2023-02-09 10:46:32.390088 sample-factory-2.0.3/setup.cfg
--rw-rw-r--   0 alex      (1000) alex      (1000)     2539 2023-02-07 04:22:17.000000 sample-factory-2.0.3/setup.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-02-09 10:46:32.346090 sample-factory-2.0.3/sf_examples/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-12-07 00:16:21.000000 sample-factory-2.0.3/sf_examples/__init__.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-02-09 10:46:32.350090 sample-factory-2.0.3/sf_examples/atari/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-12-07 00:16:21.000000 sample-factory-2.0.3/sf_examples/atari/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1554 2022-12-07 00:16:21.000000 sample-factory-2.0.3/sf_examples/atari/atari_params.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     4991 2022-12-07 00:16:21.000000 sample-factory-2.0.3/sf_examples/atari/atari_utils.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      350 2022-12-07 00:16:21.000000 sample-factory-2.0.3/sf_examples/atari/enjoy_atari.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-02-09 10:46:32.350090 sample-factory-2.0.3/sf_examples/atari/experiments/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-12-07 00:16:21.000000 sample-factory-2.0.3/sf_examples/atari/experiments/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      859 2022-12-07 00:16:21.000000 sample-factory-2.0.3/sf_examples/atari/experiments/atari_envs.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      922 2022-12-07 00:16:21.000000 sample-factory-2.0.3/sf_examples/atari/train_atari.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-02-09 10:46:32.350090 sample-factory-2.0.3/sf_examples/brax/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-01-12 23:57:40.000000 sample-factory-2.0.3/sf_examples/brax/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     6839 2023-01-12 23:57:40.000000 sample-factory-2.0.3/sf_examples/brax/brax_render.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      370 2023-01-12 23:57:40.000000 sample-factory-2.0.3/sf_examples/brax/enjoy_brax.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-02-09 10:46:32.350090 sample-factory-2.0.3/sf_examples/brax/experiments/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-01-12 23:57:40.000000 sample-factory-2.0.3/sf_examples/brax/experiments/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1270 2023-01-12 23:57:40.000000 sample-factory-2.0.3/sf_examples/brax/experiments/brax_basic_envs.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      324 2023-01-12 23:57:40.000000 sample-factory-2.0.3/sf_examples/brax/experiments/sbatch_timeout_brax.sh
--rw-rw-r--   0 alex      (1000) alex      (1000)     7827 2023-02-07 04:15:48.000000 sample-factory-2.0.3/sf_examples/brax/train_brax.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-02-09 10:46:32.350090 sample-factory-2.0.3/sf_examples/dmlab/
--rw-rw-r--   0 alex      (1000) alex      (1000)      166 2022-12-07 00:16:21.000000 sample-factory-2.0.3/sf_examples/dmlab/README.md
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-12-07 00:16:21.000000 sample-factory-2.0.3/sf_examples/dmlab/__init__.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-02-09 10:46:32.350090 sample-factory-2.0.3/sf_examples/dmlab/command_line/
--rwxrwxr-x   0 alex      (1000) alex      (1000)      666 2022-12-07 00:16:21.000000 sample-factory-2.0.3/sf_examples/dmlab/command_line/train_dmlab30.sh
--rwxrwxr-x   0 alex      (1000) alex      (1000)      829 2022-12-07 00:16:21.000000 sample-factory-2.0.3/sf_examples/dmlab/command_line/train_dmlab30_server_pbt.sh
--rw-rw-r--   0 alex      (1000) alex      (1000)     7874 2022-12-07 00:16:21.000000 sample-factory-2.0.3/sf_examples/dmlab/dmlab30.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    10329 2022-12-07 00:16:21.000000 sample-factory-2.0.3/sf_examples/dmlab/dmlab_env.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     9713 2022-12-07 00:16:21.000000 sample-factory-2.0.3/sf_examples/dmlab/dmlab_gym.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    10344 2022-12-07 00:16:21.000000 sample-factory-2.0.3/sf_examples/dmlab/dmlab_level_cache.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     3501 2022-12-07 00:16:21.000000 sample-factory-2.0.3/sf_examples/dmlab/dmlab_model.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     3261 2023-01-13 00:01:32.000000 sample-factory-2.0.3/sf_examples/dmlab/dmlab_params.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     6464 2022-12-07 00:16:21.000000 sample-factory-2.0.3/sf_examples/dmlab/dmlab_populate_cache.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      289 2022-12-07 00:16:21.000000 sample-factory-2.0.3/sf_examples/dmlab/dmlab_utils.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      349 2022-12-07 00:16:21.000000 sample-factory-2.0.3/sf_examples/dmlab/enjoy_dmlab.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-02-09 10:46:32.350090 sample-factory-2.0.3/sf_examples/dmlab/experiments/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-12-07 00:16:21.000000 sample-factory-2.0.3/sf_examples/dmlab/experiments/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1376 2023-01-10 07:03:14.000000 sample-factory-2.0.3/sf_examples/dmlab/experiments/dmlab30.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     3610 2022-12-07 00:16:21.000000 sample-factory-2.0.3/sf_examples/dmlab/train_dmlab.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-02-09 10:46:32.350090 sample-factory-2.0.3/sf_examples/dmlab/wrappers/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-12-07 00:16:21.000000 sample-factory-2.0.3/sf_examples/dmlab/wrappers/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1416 2022-12-07 00:16:21.000000 sample-factory-2.0.3/sf_examples/dmlab/wrappers/reward_shaping.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      365 2022-12-07 00:16:21.000000 sample-factory-2.0.3/sf_examples/enjoy_custom_env_custom_model.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      358 2022-12-07 00:16:21.000000 sample-factory-2.0.3/sf_examples/enjoy_custom_multi_env.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      349 2022-12-07 00:16:21.000000 sample-factory-2.0.3/sf_examples/enjoy_gym_env.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-02-09 10:46:32.350090 sample-factory-2.0.3/sf_examples/envpool/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-12-07 00:16:21.000000 sample-factory-2.0.3/sf_examples/envpool/__init__.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-02-09 10:46:32.350090 sample-factory-2.0.3/sf_examples/envpool/atari/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-12-07 00:16:21.000000 sample-factory-2.0.3/sf_examples/envpool/atari/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      350 2022-12-07 00:16:21.000000 sample-factory-2.0.3/sf_examples/envpool/atari/enjoy_envpool_atari.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     2045 2022-12-07 00:16:21.000000 sample-factory-2.0.3/sf_examples/envpool/atari/envpool_atari_params.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1774 2022-12-07 00:16:21.000000 sample-factory-2.0.3/sf_examples/envpool/atari/envpool_atari_utils.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1062 2022-12-07 00:16:21.000000 sample-factory-2.0.3/sf_examples/envpool/atari/train_envpool_atari.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      721 2022-12-07 00:16:21.000000 sample-factory-2.0.3/sf_examples/envpool/envpool_utils.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     2439 2022-12-07 00:16:21.000000 sample-factory-2.0.3/sf_examples/envpool/envpool_wrappers.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-02-09 10:46:32.354089 sample-factory-2.0.3/sf_examples/envpool/mujoco/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-12-07 00:16:21.000000 sample-factory-2.0.3/sf_examples/envpool/mujoco/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      323 2022-12-07 00:16:21.000000 sample-factory-2.0.3/sf_examples/envpool/mujoco/enjoy_envpool_mujoco.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     3599 2022-12-30 04:35:22.000000 sample-factory-2.0.3/sf_examples/envpool/mujoco/envpool_mujoco_params.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1623 2022-12-07 00:16:21.000000 sample-factory-2.0.3/sf_examples/envpool/mujoco/envpool_mujoco_utils.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-02-09 10:46:32.354089 sample-factory-2.0.3/sf_examples/envpool/mujoco/experiments/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-12-07 00:16:21.000000 sample-factory-2.0.3/sf_examples/envpool/mujoco/experiments/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1506 2023-01-10 07:03:14.000000 sample-factory-2.0.3/sf_examples/envpool/mujoco/experiments/mujoco_envpool.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1116 2022-12-07 00:16:21.000000 sample-factory-2.0.3/sf_examples/envpool/mujoco/train_envpool_mujoco.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-02-09 10:46:32.354089 sample-factory-2.0.3/sf_examples/isaacgym_examples/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-12-07 00:16:21.000000 sample-factory-2.0.3/sf_examples/isaacgym_examples/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      543 2022-12-07 00:16:21.000000 sample-factory-2.0.3/sf_examples/isaacgym_examples/enjoy_isaacgym.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-02-09 10:46:32.354089 sample-factory-2.0.3/sf_examples/isaacgym_examples/experiments/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-12-07 00:16:21.000000 sample-factory-2.0.3/sf_examples/isaacgym_examples/experiments/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1339 2023-01-10 07:03:14.000000 sample-factory-2.0.3/sf_examples/isaacgym_examples/experiments/isaacgym_allegrohand.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1353 2023-01-10 07:03:14.000000 sample-factory-2.0.3/sf_examples/isaacgym_examples/experiments/isaacgym_ant.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1351 2023-01-10 07:03:14.000000 sample-factory-2.0.3/sf_examples/isaacgym_examples/experiments/isaacgym_basic_envs.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1358 2023-01-10 07:03:14.000000 sample-factory-2.0.3/sf_examples/isaacgym_examples/experiments/isaacgym_humanoid.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      321 2022-12-07 00:16:21.000000 sample-factory-2.0.3/sf_examples/isaacgym_examples/experiments/isaacgym_runs.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    13612 2023-01-12 23:57:40.000000 sample-factory-2.0.3/sf_examples/isaacgym_examples/train_isaacgym.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-02-09 10:46:32.354089 sample-factory-2.0.3/sf_examples/mujoco/
--rw-rw-r--   0 alex      (1000) alex      (1000)     1647 2022-12-07 00:16:21.000000 sample-factory-2.0.3/sf_examples/mujoco/README.md
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-12-07 00:16:21.000000 sample-factory-2.0.3/sf_examples/mujoco/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      353 2022-12-07 00:16:21.000000 sample-factory-2.0.3/sf_examples/mujoco/enjoy_mujoco.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-02-09 10:46:32.354089 sample-factory-2.0.3/sf_examples/mujoco/experiments/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-12-07 00:16:21.000000 sample-factory-2.0.3/sf_examples/mujoco/experiments/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1074 2022-12-07 00:16:21.000000 sample-factory-2.0.3/sf_examples/mujoco/experiments/mujoco_all_envs.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1229 2022-12-07 00:16:21.000000 sample-factory-2.0.3/sf_examples/mujoco/mujoco_params.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1242 2022-12-07 00:16:21.000000 sample-factory-2.0.3/sf_examples/mujoco/mujoco_utils.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      949 2022-12-07 00:16:21.000000 sample-factory-2.0.3/sf_examples/mujoco/train_mujoco.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-02-09 10:46:32.354089 sample-factory-2.0.3/sf_examples/sampler/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-12-07 00:16:21.000000 sample-factory-2.0.3/sf_examples/sampler/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     2171 2022-12-07 00:16:21.000000 sample-factory-2.0.3/sf_examples/sampler/use_simplified_sampling_api.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     5349 2022-12-07 00:16:21.000000 sample-factory-2.0.3/sf_examples/train_custom_env_custom_model.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     5752 2022-12-07 00:16:21.000000 sample-factory-2.0.3/sf_examples/train_custom_multi_env.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1356 2022-12-07 00:16:21.000000 sample-factory-2.0.3/sf_examples/train_gym_env.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-02-09 10:46:32.354089 sample-factory-2.0.3/sf_examples/vizdoom/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-12-07 00:16:21.000000 sample-factory-2.0.3/sf_examples/vizdoom/__init__.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-02-09 10:46:32.354089 sample-factory-2.0.3/sf_examples/vizdoom/custom_env/
--rw-rw-r--   0 alex      (1000) alex      (1000)      984 2022-12-07 00:16:21.000000 sample-factory-2.0.3/sf_examples/vizdoom/custom_env/custom_doom_env.cfg
--rw-rw-r--   0 alex      (1000) alex      (1000)     2704 2022-12-07 00:16:21.000000 sample-factory-2.0.3/sf_examples/vizdoom/custom_env/custom_doom_env.wad
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-02-09 10:46:32.358089 sample-factory-2.0.3/sf_examples/vizdoom/doom/
--rw-rw-r--   0 alex      (1000) alex      (1000)      225 2022-12-07 00:16:21.000000 sample-factory-2.0.3/sf_examples/vizdoom/doom/README.md
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-12-07 00:16:21.000000 sample-factory-2.0.3/sf_examples/vizdoom/doom/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     4970 2022-12-07 00:16:21.000000 sample-factory-2.0.3/sf_examples/vizdoom/doom/action_space.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    25185 2022-12-07 00:16:21.000000 sample-factory-2.0.3/sf_examples/vizdoom/doom/doom_gym.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1718 2022-12-07 00:16:21.000000 sample-factory-2.0.3/sf_examples/vizdoom/doom/doom_model.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     2816 2022-12-07 00:16:21.000000 sample-factory-2.0.3/sf_examples/vizdoom/doom/doom_params.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1946 2022-12-07 00:16:21.000000 sample-factory-2.0.3/sf_examples/vizdoom/doom/doom_play_demo.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      927 2022-12-07 00:16:21.000000 sample-factory-2.0.3/sf_examples/vizdoom/doom/doom_render.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    13538 2022-12-07 00:16:21.000000 sample-factory-2.0.3/sf_examples/vizdoom/doom/doom_utils.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     8004 2022-12-07 00:16:21.000000 sample-factory-2.0.3/sf_examples/vizdoom/doom/multi_agent_match.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-02-09 10:46:32.358089 sample-factory-2.0.3/sf_examples/vizdoom/doom/multiplayer/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-12-07 00:16:21.000000 sample-factory-2.0.3/sf_examples/vizdoom/doom/multiplayer/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     9272 2022-12-07 00:16:21.000000 sample-factory-2.0.3/sf_examples/vizdoom/doom/multiplayer/doom_multiagent.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    14044 2022-12-07 00:16:21.000000 sample-factory-2.0.3/sf_examples/vizdoom/doom/multiplayer/doom_multiagent_wrapper.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      790 2022-12-07 00:16:21.000000 sample-factory-2.0.3/sf_examples/vizdoom/doom/play_doom.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      606 2022-12-07 00:16:21.000000 sample-factory-2.0.3/sf_examples/vizdoom/doom/sample_env.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-02-09 10:46:32.386088 sample-factory-2.0.3/sf_examples/vizdoom/doom/scenarios/
--rw-rw-r--   0 alex      (1000) alex      (1000)      924 2022-12-07 00:16:21.000000 sample-factory-2.0.3/sf_examples/vizdoom/doom/scenarios/basic.cfg
--rw-rw-r--   0 alex      (1000) alex      (1000)     2704 2022-12-07 00:16:21.000000 sample-factory-2.0.3/sf_examples/vizdoom/doom/scenarios/basic.wad
--rw-rw-r--   0 alex      (1000) alex      (1000)     1078 2022-12-07 00:16:21.000000 sample-factory-2.0.3/sf_examples/vizdoom/doom/scenarios/battle.cfg
--rw-rw-r--   0 alex      (1000) alex      (1000)    15496 2022-12-07 00:16:21.000000 sample-factory-2.0.3/sf_examples/vizdoom/doom/scenarios/battle.wad
--rw-rw-r--   0 alex      (1000) alex      (1000)    82549 2022-12-07 00:16:21.000000 sample-factory-2.0.3/sf_examples/vizdoom/doom/scenarios/battle2.wad
--rw-rw-r--   0 alex      (1000) alex      (1000)     1006 2022-12-07 00:16:21.000000 sample-factory-2.0.3/sf_examples/vizdoom/doom/scenarios/battle2_continuous_turning.cfg
--rw-rw-r--   0 alex      (1000) alex      (1000)     1071 2022-12-07 00:16:21.000000 sample-factory-2.0.3/sf_examples/vizdoom/doom/scenarios/battle_continuous_turning.cfg
--rw-rw-r--   0 alex      (1000) alex      (1000)     1052 2022-12-07 00:16:21.000000 sample-factory-2.0.3/sf_examples/vizdoom/doom/scenarios/cig.cfg
--rw-rw-r--   0 alex      (1000) alex      (1000)   214730 2022-12-07 00:16:21.000000 sample-factory-2.0.3/sf_examples/vizdoom/doom/scenarios/cig.wad
--rw-rw-r--   0 alex      (1000) alex      (1000)      891 2022-12-07 00:16:21.000000 sample-factory-2.0.3/sf_examples/vizdoom/doom/scenarios/deadly_corridor.cfg
--rw-rw-r--   0 alex      (1000) alex      (1000)    10048 2022-12-07 00:16:21.000000 sample-factory-2.0.3/sf_examples/vizdoom/doom/scenarios/deadly_corridor.wad
--rw-rw-r--   0 alex      (1000) alex      (1000)      901 2022-12-07 00:16:21.000000 sample-factory-2.0.3/sf_examples/vizdoom/doom/scenarios/defend_the_center.cfg
--rw-rw-r--   0 alex      (1000) alex      (1000)     6478 2022-12-07 00:16:21.000000 sample-factory-2.0.3/sf_examples/vizdoom/doom/scenarios/defend_the_center.wad
--rw-rw-r--   0 alex      (1000) alex      (1000)      825 2022-12-07 00:16:21.000000 sample-factory-2.0.3/sf_examples/vizdoom/doom/scenarios/defend_the_line.cfg
--rw-rw-r--   0 alex      (1000) alex      (1000)     4139 2022-12-07 00:16:21.000000 sample-factory-2.0.3/sf_examples/vizdoom/doom/scenarios/defend_the_line.wad
--rw-rw-r--   0 alex      (1000) alex      (1000)  2109396 2022-12-07 00:16:21.000000 sample-factory-2.0.3/sf_examples/vizdoom/doom/scenarios/dwango5.wad
--rw-rw-r--   0 alex      (1000) alex      (1000)     1469 2022-12-07 00:16:21.000000 sample-factory-2.0.3/sf_examples/vizdoom/doom/scenarios/dwango5_dm.cfg
--rw-rw-r--   0 alex      (1000) alex      (1000)     1569 2022-12-07 00:16:21.000000 sample-factory-2.0.3/sf_examples/vizdoom/doom/scenarios/dwango5_dm_continuous_weap.cfg
--rw-rw-r--   0 alex      (1000) alex      (1000)     1580 2022-12-07 00:16:21.000000 sample-factory-2.0.3/sf_examples/vizdoom/doom/scenarios/freedm.cfg
--rw-rw-r--   0 alex      (1000) alex      (1000) 21112116 2022-12-07 00:16:21.000000 sample-factory-2.0.3/sf_examples/vizdoom/doom/scenarios/freedm.wad
--rw-rw-r--   0 alex      (1000) alex      (1000)     1044 2022-12-07 00:16:21.000000 sample-factory-2.0.3/sf_examples/vizdoom/doom/scenarios/health_gathering.cfg
--rw-rw-r--   0 alex      (1000) alex      (1000)     2837 2022-12-07 00:16:21.000000 sample-factory-2.0.3/sf_examples/vizdoom/doom/scenarios/health_gathering.wad
--rw-rw-r--   0 alex      (1000) alex      (1000)      868 2022-12-07 00:16:21.000000 sample-factory-2.0.3/sf_examples/vizdoom/doom/scenarios/health_gathering_supreme.cfg
--rw-rw-r--   0 alex      (1000) alex      (1000)    23206 2022-12-07 00:16:21.000000 sample-factory-2.0.3/sf_examples/vizdoom/doom/scenarios/health_gathering_supreme.wad
--rw-rw-r--   0 alex      (1000) alex      (1000)      947 2022-12-07 00:16:21.000000 sample-factory-2.0.3/sf_examples/vizdoom/doom/scenarios/my_way_home.cfg
--rw-rw-r--   0 alex      (1000) alex      (1000)    28469 2022-12-07 00:16:21.000000 sample-factory-2.0.3/sf_examples/vizdoom/doom/scenarios/my_way_home.wad
--rw-rw-r--   0 alex      (1000) alex      (1000)     1578 2022-12-07 00:16:21.000000 sample-factory-2.0.3/sf_examples/vizdoom/doom/scenarios/ssl2.cfg
--rw-rw-r--   0 alex      (1000) alex      (1000)   330798 2022-12-07 00:16:21.000000 sample-factory-2.0.3/sf_examples/vizdoom/doom/scenarios/ssl2.wad
--rw-rw-r--   0 alex      (1000) alex      (1000)      864 2022-12-07 00:16:21.000000 sample-factory-2.0.3/sf_examples/vizdoom/doom/scenarios/two_colors_easy.cfg
--rw-rw-r--   0 alex      (1000) alex      (1000)     4810 2022-12-07 00:16:21.000000 sample-factory-2.0.3/sf_examples/vizdoom/doom/scenarios/two_colors_easy.wad
--rw-rw-r--   0 alex      (1000) alex      (1000)      864 2022-12-07 00:16:21.000000 sample-factory-2.0.3/sf_examples/vizdoom/doom/scenarios/two_colors_hard.cfg
--rw-rw-r--   0 alex      (1000) alex      (1000)     5096 2022-12-07 00:16:21.000000 sample-factory-2.0.3/sf_examples/vizdoom/doom/scenarios/two_colors_hard.wad
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-02-09 10:46:32.386088 sample-factory-2.0.3/sf_examples/vizdoom/doom/scripts/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-12-07 00:16:21.000000 sample-factory-2.0.3/sf_examples/vizdoom/doom/scripts/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1076 2022-12-07 00:16:21.000000 sample-factory-2.0.3/sf_examples/vizdoom/doom/scripts/generate_bots.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-02-09 10:46:32.390088 sample-factory-2.0.3/sf_examples/vizdoom/doom/wrappers/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-12-07 00:16:21.000000 sample-factory-2.0.3/sf_examples/vizdoom/doom/wrappers/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     3754 2022-12-07 00:16:21.000000 sample-factory-2.0.3/sf_examples/vizdoom/doom/wrappers/additional_input.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     2373 2022-12-07 00:16:21.000000 sample-factory-2.0.3/sf_examples/vizdoom/doom/wrappers/bot_difficulty.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1888 2022-12-07 00:16:21.000000 sample-factory-2.0.3/sf_examples/vizdoom/doom/wrappers/exploration.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     2335 2022-12-07 00:16:21.000000 sample-factory-2.0.3/sf_examples/vizdoom/doom/wrappers/multiplayer_stats.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1963 2022-12-07 00:16:21.000000 sample-factory-2.0.3/sf_examples/vizdoom/doom/wrappers/observation_space.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     9183 2022-12-07 00:16:21.000000 sample-factory-2.0.3/sf_examples/vizdoom/doom/wrappers/reward_shaping.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-02-09 10:46:32.390088 sample-factory-2.0.3/sf_examples/vizdoom/doom/wrappers/scenario_wrappers/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-12-07 00:16:21.000000 sample-factory-2.0.3/sf_examples/vizdoom/doom/wrappers/scenario_wrappers/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1194 2022-12-07 00:16:21.000000 sample-factory-2.0.3/sf_examples/vizdoom/doom/wrappers/scenario_wrappers/gathering_reward_shaping.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1116 2022-12-07 00:16:21.000000 sample-factory-2.0.3/sf_examples/vizdoom/doom/wrappers/step_human_input.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      860 2022-12-07 00:16:21.000000 sample-factory-2.0.3/sf_examples/vizdoom/enjoy_custom_vizdoom_env.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      814 2022-12-07 00:16:21.000000 sample-factory-2.0.3/sf_examples/vizdoom/enjoy_vizdoom.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     2362 2022-12-07 00:16:21.000000 sample-factory-2.0.3/sf_examples/vizdoom/train_custom_vizdoom_env.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1500 2022-12-07 00:16:21.000000 sample-factory-2.0.3/sf_examples/vizdoom/train_vizdoom.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-02-09 10:46:32.390088 sample-factory-2.0.3/tests/
--rw-rw-r--   0 alex      (1000) alex      (1000)     3811 2022-12-07 00:16:21.000000 sample-factory-2.0.3/tests/test_launcher.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      641 2022-12-07 00:16:21.000000 sample-factory-2.0.3/tests/test_precheck.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1982 2022-12-07 00:16:21.000000 sample-factory-2.0.3/tests/test_utils.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-02-09 10:46:32.334090 sample-factory-2.0.3/train_dir/
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-02-09 10:46:32.390088 sample-factory-2.0.3/train_dir/isaacgym_allegrohand/
--rw-rw-r--   0 alex      (1000) alex      (1000)     1804 2022-11-30 09:17:34.000000 sample-factory-2.0.3/train_dir/isaacgym_allegrohand/README.md
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-02-09 10:46:32.390088 sample-factory-2.0.3/train_dir/isaacgym_ant/
--rw-rw-r--   0 alex      (1000) alex      (1000)     1741 2022-11-30 09:12:41.000000 sample-factory-2.0.3/train_dir/isaacgym_ant/README.md
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-02-09 10:46:32.390088 sample-factory-2.0.3/train_dir/isaacgym_humanoid/
--rw-rw-r--   0 alex      (1000) alex      (1000)     1780 2022-11-30 09:15:44.000000 sample-factory-2.0.3/train_dir/isaacgym_humanoid/README.md
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-19 08:22:20.628728 sample-factory-2.1.1/
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-19 08:22:20.580728 sample-factory-2.1.1/.pytest_cache/
+-rw-rw-r--   0 alex      (1000) alex      (1000)      302 2023-02-26 04:17:32.000000 sample-factory-2.1.1/.pytest_cache/README.md
+-rw-rw-r--   0 alex      (1000) alex      (1000)     3193 2023-02-26 03:48:30.000000 sample-factory-2.1.1/CONTRIBUTING.md
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1073 2023-02-26 03:48:30.000000 sample-factory-2.1.1/LICENSE
+-rw-rw-r--   0 alex      (1000) alex      (1000)      118 2023-02-26 03:48:30.000000 sample-factory-2.1.1/MANIFEST.in
+-rw-rw-r--   0 alex      (1000) alex      (1000)    10876 2023-06-19 08:22:20.628728 sample-factory-2.1.1/PKG-INFO
+-rw-rw-r--   0 alex      (1000) alex      (1000)    11167 2023-05-02 05:55:36.000000 sample-factory-2.1.1/README.md
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-19 08:22:20.580728 sample-factory-2.1.1/docs/
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-19 08:22:20.580728 sample-factory-2.1.1/docs/01-get-started/
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1412 2023-02-26 03:48:30.000000 sample-factory-2.1.1/docs/01-get-started/basic-usage.md
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1160 2023-02-26 03:48:30.000000 sample-factory-2.1.1/docs/01-get-started/installation.md
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-19 08:22:20.584728 sample-factory-2.1.1/docs/02-configuration/
+-rw-rw-r--   0 alex      (1000) alex      (1000)    40945 2023-02-28 05:39:34.000000 sample-factory-2.1.1/docs/02-configuration/cfg-params.md
+-rw-rw-r--   0 alex      (1000) alex      (1000)     5037 2023-02-26 03:48:30.000000 sample-factory-2.1.1/docs/02-configuration/configuration.md
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-19 08:22:20.584728 sample-factory-2.1.1/docs/03-customization/
+-rw-rw-r--   0 alex      (1000) alex      (1000)     5640 2023-02-26 03:48:30.000000 sample-factory-2.1.1/docs/03-customization/custom-environments.md
+-rw-rw-r--   0 alex      (1000) alex      (1000)     4194 2023-02-26 03:48:30.000000 sample-factory-2.1.1/docs/03-customization/custom-models.md
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2378 2023-02-26 03:48:30.000000 sample-factory-2.1.1/docs/03-customization/custom-multi-agent-environments.md
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-19 08:22:20.584728 sample-factory-2.1.1/docs/04-experiments/
+-rw-rw-r--   0 alex      (1000) alex      (1000)    11233 2023-02-26 03:48:30.000000 sample-factory-2.1.1/docs/04-experiments/experiment-launcher.md
+-rw-rw-r--   0 alex      (1000) alex      (1000)     3028 2023-02-26 03:48:30.000000 sample-factory-2.1.1/docs/04-experiments/slurm-details.md
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-19 08:22:20.584728 sample-factory-2.1.1/docs/05-monitoring/
+-rw-rw-r--   0 alex      (1000) alex      (1000)      912 2023-02-26 03:48:30.000000 sample-factory-2.1.1/docs/05-monitoring/custom-metrics.md
+-rw-rw-r--   0 alex      (1000) alex      (1000)     8412 2023-02-26 03:48:30.000000 sample-factory-2.1.1/docs/05-monitoring/metrics-reference.md
+-rw-rw-r--   0 alex      (1000) alex      (1000)      922 2023-02-26 03:48:30.000000 sample-factory-2.1.1/docs/05-monitoring/tensorboard.md
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1309 2023-02-26 03:48:30.000000 sample-factory-2.1.1/docs/05-monitoring/wandb.md
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-19 08:22:20.584728 sample-factory-2.1.1/docs/05-troubleshooting/
+-rw-rw-r--   0 alex      (1000) alex      (1000)      771 2023-02-28 09:39:47.000000 sample-factory-2.1.1/docs/05-troubleshooting/troubleshooting.md
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-19 08:22:20.584728 sample-factory-2.1.1/docs/06-architecture/
+-rw-rw-r--   0 alex      (1000) alex      (1000)     3219 2023-02-26 03:48:30.000000 sample-factory-2.1.1/docs/06-architecture/message-passing.md
+-rw-rw-r--   0 alex      (1000) alex      (1000)     6395 2023-02-26 03:48:30.000000 sample-factory-2.1.1/docs/06-architecture/overview.md
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-19 08:22:20.584728 sample-factory-2.1.1/docs/07-advanced-topics/
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2406 2023-02-26 03:48:30.000000 sample-factory-2.1.1/docs/07-advanced-topics/batched-non-batched.md
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1165 2023-02-26 03:48:30.000000 sample-factory-2.1.1/docs/07-advanced-topics/double-buffered.md
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1708 2023-02-26 03:48:30.000000 sample-factory-2.1.1/docs/07-advanced-topics/inactive-agents.md
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2875 2023-02-26 03:48:30.000000 sample-factory-2.1.1/docs/07-advanced-topics/multi-policy-training.md
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2122 2023-02-26 03:48:30.000000 sample-factory-2.1.1/docs/07-advanced-topics/normalizations.md
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1578 2023-02-26 03:48:30.000000 sample-factory-2.1.1/docs/07-advanced-topics/observer.md
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2710 2023-02-26 03:48:30.000000 sample-factory-2.1.1/docs/07-advanced-topics/passing-info.md
+-rw-rw-r--   0 alex      (1000) alex      (1000)     7221 2023-05-02 05:55:45.000000 sample-factory-2.1.1/docs/07-advanced-topics/pbt.md
+-rw-rw-r--   0 alex      (1000) alex      (1000)     4982 2023-02-26 03:48:30.000000 sample-factory-2.1.1/docs/07-advanced-topics/policy-lag.md
+-rw-rw-r--   0 alex      (1000) alex      (1000)     9675 2023-02-26 03:48:30.000000 sample-factory-2.1.1/docs/07-advanced-topics/profiling.md
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1105 2023-02-26 03:48:30.000000 sample-factory-2.1.1/docs/07-advanced-topics/serial-mode.md
+-rw-rw-r--   0 alex      (1000) alex      (1000)     3556 2023-02-26 03:48:30.000000 sample-factory-2.1.1/docs/07-advanced-topics/sync-async.md
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-19 08:22:20.584728 sample-factory-2.1.1/docs/08-miscellaneous/
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1098 2023-02-26 03:48:30.000000 sample-factory-2.1.1/docs/08-miscellaneous/tests.md
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1652 2023-02-26 03:48:30.000000 sample-factory-2.1.1/docs/08-miscellaneous/v1-to-v2.md
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-19 08:22:20.584728 sample-factory-2.1.1/docs/09-environment-integrations/
+-rw-rw-r--   0 alex      (1000) alex      (1000)    12609 2023-05-02 07:07:32.000000 sample-factory-2.1.1/docs/09-environment-integrations/atari.md
+-rw-rw-r--   0 alex      (1000) alex      (1000)     3951 2023-02-26 03:48:30.000000 sample-factory-2.1.1/docs/09-environment-integrations/brax.md
+-rw-rw-r--   0 alex      (1000) alex      (1000)     3529 2023-05-02 05:55:45.000000 sample-factory-2.1.1/docs/09-environment-integrations/dmlab.md
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1857 2023-02-26 03:48:30.000000 sample-factory-2.1.1/docs/09-environment-integrations/envpool.md
+-rw-rw-r--   0 alex      (1000) alex      (1000)     3007 2023-02-26 03:48:30.000000 sample-factory-2.1.1/docs/09-environment-integrations/isaacgym.md
+-rw-rw-r--   0 alex      (1000) alex      (1000)     3305 2023-02-26 03:48:30.000000 sample-factory-2.1.1/docs/09-environment-integrations/megaverse.md
+-rw-rw-r--   0 alex      (1000) alex      (1000)     5943 2023-02-26 03:48:30.000000 sample-factory-2.1.1/docs/09-environment-integrations/mujoco.md
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2587 2023-02-26 03:48:30.000000 sample-factory-2.1.1/docs/09-environment-integrations/swarm-rl.md
+-rw-rw-r--   0 alex      (1000) alex      (1000)     9019 2023-02-26 03:48:30.000000 sample-factory-2.1.1/docs/09-environment-integrations/vizdoom.md
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-19 08:22:20.584728 sample-factory-2.1.1/docs/10-huggingface/
+-rw-rw-r--   0 alex      (1000) alex      (1000)     4502 2023-02-26 03:48:30.000000 sample-factory-2.1.1/docs/10-huggingface/huggingface.md
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-19 08:22:20.584728 sample-factory-2.1.1/docs/11-release-notes/
+-rw-rw-r--   0 alex      (1000) alex      (1000)     4209 2023-06-19 04:29:40.000000 sample-factory-2.1.1/docs/11-release-notes/release-notes.md
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-19 08:22:20.588728 sample-factory-2.1.1/docs/12-community/
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1081 2023-02-26 03:48:30.000000 sample-factory-2.1.1/docs/12-community/citation.md
+-rw-rw-r--   0 alex      (1000) alex      (1000)     3181 2023-02-26 03:48:30.000000 sample-factory-2.1.1/docs/12-community/contribution.md
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1006 2023-02-28 05:40:07.000000 sample-factory-2.1.1/docs/12-community/doc-contribution.md
+-rw-rw-r--   0 alex      (1000) alex      (1000)      680 2023-02-26 03:48:30.000000 sample-factory-2.1.1/docs/cfg-params.sh
+-rw-rw-r--   0 alex      (1000) alex      (1000)     5203 2023-05-02 05:55:36.000000 sample-factory-2.1.1/docs/index.md
+-rw-rw-r--   0 alex      (1000) alex      (1000)      321 2023-05-03 05:21:00.000000 sample-factory-2.1.1/pyproject.toml
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-19 08:22:20.588728 sample-factory-2.1.1/sample_factory/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-02-26 03:48:30.000000 sample-factory-2.1.1/sample_factory/__init__.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-19 08:22:20.588728 sample-factory-2.1.1/sample_factory/algo/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-02-26 03:48:30.000000 sample-factory-2.1.1/sample_factory/algo/__init__.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-19 08:22:20.588728 sample-factory-2.1.1/sample_factory/algo/evaluators/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-02-26 22:52:46.000000 sample-factory-2.1.1/sample_factory/algo/evaluators/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-05-02 05:55:36.000000 sample-factory-2.1.1/sample_factory/algo/evaluators/default_evaluator.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-19 08:22:20.588728 sample-factory-2.1.1/sample_factory/algo/learning/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-02-26 03:48:30.000000 sample-factory-2.1.1/sample_factory/algo/learning/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    11329 2023-02-26 03:48:30.000000 sample-factory-2.1.1/sample_factory/algo/learning/batcher.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    48320 2023-02-26 03:48:30.000000 sample-factory-2.1.1/sample_factory/algo/learning/learner.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     5747 2023-02-26 03:48:30.000000 sample-factory-2.1.1/sample_factory/algo/learning/learner_worker.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     6962 2023-02-26 03:48:30.000000 sample-factory-2.1.1/sample_factory/algo/learning/rnn_utils.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-19 08:22:20.588728 sample-factory-2.1.1/sample_factory/algo/runners/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-02-26 03:48:30.000000 sample-factory-2.1.1/sample_factory/algo/runners/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    32869 2023-02-26 03:48:30.000000 sample-factory-2.1.1/sample_factory/algo/runners/runner.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2369 2023-02-26 03:48:30.000000 sample-factory-2.1.1/sample_factory/algo/runners/runner_parallel.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1154 2023-02-26 03:48:30.000000 sample-factory-2.1.1/sample_factory/algo/runners/runner_serial.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-19 08:22:20.588728 sample-factory-2.1.1/sample_factory/algo/sampling/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-02-26 03:48:30.000000 sample-factory-2.1.1/sample_factory/algo/sampling/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    17453 2023-02-26 03:48:30.000000 sample-factory-2.1.1/sample_factory/algo/sampling/batched_sampling.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    16896 2023-02-26 03:48:30.000000 sample-factory-2.1.1/sample_factory/algo/sampling/inference_worker.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    31353 2023-05-02 06:30:38.000000 sample-factory-2.1.1/sample_factory/algo/sampling/non_batched_sampling.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    14921 2023-02-26 03:48:30.000000 sample-factory-2.1.1/sample_factory/algo/sampling/rollout_worker.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    12946 2023-02-26 03:48:30.000000 sample-factory-2.1.1/sample_factory/algo/sampling/sampler.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2773 2023-02-26 03:48:30.000000 sample-factory-2.1.1/sample_factory/algo/sampling/sampling_utils.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     8361 2023-02-26 03:48:30.000000 sample-factory-2.1.1/sample_factory/algo/sampling/simplified_sampling_api.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-19 08:22:20.592728 sample-factory-2.1.1/sample_factory/algo/utils/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-02-26 03:48:30.000000 sample-factory-2.1.1/sample_factory/algo/utils/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    10777 2023-02-26 03:48:30.000000 sample-factory-2.1.1/sample_factory/algo/utils/action_distributions.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2839 2023-02-26 03:48:30.000000 sample-factory-2.1.1/sample_factory/algo/utils/agent_policy_mapping.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1022 2023-02-26 03:48:30.000000 sample-factory-2.1.1/sample_factory/algo/utils/context.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     4868 2023-02-26 03:48:30.000000 sample-factory-2.1.1/sample_factory/algo/utils/env_info.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     4491 2023-02-26 03:48:30.000000 sample-factory-2.1.1/sample_factory/algo/utils/gymnasium_utils.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1186 2023-02-26 03:48:30.000000 sample-factory-2.1.1/sample_factory/algo/utils/heartbeat.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    15276 2023-06-19 04:04:06.000000 sample-factory-2.1.1/sample_factory/algo/utils/make_env.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1086 2023-02-26 03:48:30.000000 sample-factory-2.1.1/sample_factory/algo/utils/misc.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     6051 2023-02-26 03:48:30.000000 sample-factory-2.1.1/sample_factory/algo/utils/model_sharing.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      886 2023-02-26 03:48:30.000000 sample-factory-2.1.1/sample_factory/algo/utils/multiprocessing_utils.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     6270 2023-02-26 03:48:30.000000 sample-factory-2.1.1/sample_factory/algo/utils/optimizers.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     3805 2023-02-26 03:48:30.000000 sample-factory-2.1.1/sample_factory/algo/utils/rl_utils.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     5906 2023-02-26 03:48:30.000000 sample-factory-2.1.1/sample_factory/algo/utils/running_mean_std.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    11124 2023-02-26 03:48:30.000000 sample-factory-2.1.1/sample_factory/algo/utils/shared_buffers.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-19 08:22:20.592728 sample-factory-2.1.1/sample_factory/algo/utils/spaces/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-02-26 03:48:30.000000 sample-factory-2.1.1/sample_factory/algo/utils/spaces/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      449 2023-02-26 03:48:30.000000 sample-factory-2.1.1/sample_factory/algo/utils/spaces/discretized.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     5277 2023-02-26 03:48:30.000000 sample-factory-2.1.1/sample_factory/algo/utils/tensor_dict.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1081 2023-02-26 03:48:30.000000 sample-factory-2.1.1/sample_factory/algo/utils/tensor_utils.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1741 2023-02-26 03:48:30.000000 sample-factory-2.1.1/sample_factory/algo/utils/torch_utils.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-19 08:22:20.592728 sample-factory-2.1.1/sample_factory/cfg/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-02-26 03:48:30.000000 sample-factory-2.1.1/sample_factory/cfg/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    10766 2023-02-26 03:48:30.000000 sample-factory-2.1.1/sample_factory/cfg/arguments.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    35663 2023-02-26 03:48:30.000000 sample-factory-2.1.1/sample_factory/cfg/cfg.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      146 2023-02-26 03:48:30.000000 sample-factory-2.1.1/sample_factory/cfg/configurable.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    11353 2023-02-26 03:48:30.000000 sample-factory-2.1.1/sample_factory/enjoy.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-19 08:22:20.592728 sample-factory-2.1.1/sample_factory/envs/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-02-26 03:48:30.000000 sample-factory-2.1.1/sample_factory/envs/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1519 2023-02-26 03:48:30.000000 sample-factory-2.1.1/sample_factory/envs/create_env.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     5247 2023-02-26 03:48:30.000000 sample-factory-2.1.1/sample_factory/envs/env_utils.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    15562 2023-02-26 03:48:30.000000 sample-factory-2.1.1/sample_factory/envs/env_wrappers.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-19 08:22:20.592728 sample-factory-2.1.1/sample_factory/huggingface/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-02-26 03:48:30.000000 sample-factory-2.1.1/sample_factory/huggingface/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     4762 2023-02-26 03:48:30.000000 sample-factory-2.1.1/sample_factory/huggingface/huggingface_utils.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      669 2023-02-26 03:48:30.000000 sample-factory-2.1.1/sample_factory/huggingface/load_from_hub.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1884 2023-02-26 03:48:30.000000 sample-factory-2.1.1/sample_factory/huggingface/push_to_hub.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-19 08:22:20.592728 sample-factory-2.1.1/sample_factory/launcher/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-02-26 03:48:30.000000 sample-factory-2.1.1/sample_factory/launcher/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      154 2023-02-26 03:48:30.000000 sample-factory-2.1.1/sample_factory/launcher/launcher_utils.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2742 2023-02-26 03:48:30.000000 sample-factory-2.1.1/sample_factory/launcher/run.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     7490 2023-02-26 03:48:30.000000 sample-factory-2.1.1/sample_factory/launcher/run_description.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2289 2023-02-26 03:48:30.000000 sample-factory-2.1.1/sample_factory/launcher/run_ngc.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     5474 2023-02-26 03:48:30.000000 sample-factory-2.1.1/sample_factory/launcher/run_processes.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     4558 2023-02-26 03:48:30.000000 sample-factory-2.1.1/sample_factory/launcher/run_slurm.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-19 08:22:20.592728 sample-factory-2.1.1/sample_factory/launcher/slurm/
+-rw-rw-r--   0 alex      (1000) alex      (1000)      210 2023-02-26 03:48:30.000000 sample-factory-2.1.1/sample_factory/launcher/slurm/sbatch_timeout.sh
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-19 08:22:20.596728 sample-factory-2.1.1/sample_factory/model/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-02-26 03:48:30.000000 sample-factory-2.1.1/sample_factory/model/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     3046 2023-02-26 03:48:30.000000 sample-factory-2.1.1/sample_factory/model/action_parameterization.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    12744 2023-02-26 03:48:30.000000 sample-factory-2.1.1/sample_factory/model/actor_critic.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2656 2023-02-26 03:48:30.000000 sample-factory-2.1.1/sample_factory/model/core.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1081 2023-02-26 03:48:30.000000 sample-factory-2.1.1/sample_factory/model/decoder.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     8952 2023-02-26 03:48:30.000000 sample-factory-2.1.1/sample_factory/model/encoder.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2948 2023-02-26 03:48:30.000000 sample-factory-2.1.1/sample_factory/model/model_factory.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1861 2023-06-19 08:02:26.000000 sample-factory-2.1.1/sample_factory/model/model_utils.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-19 08:22:20.596728 sample-factory-2.1.1/sample_factory/pbt/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-02-26 03:48:30.000000 sample-factory-2.1.1/sample_factory/pbt/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    18221 2023-02-26 03:48:30.000000 sample-factory-2.1.1/sample_factory/pbt/population_based_training.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1342 2023-05-02 05:55:36.000000 sample-factory-2.1.1/sample_factory/train.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-19 08:22:20.596728 sample-factory-2.1.1/sample_factory/utils/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-02-26 03:48:30.000000 sample-factory-2.1.1/sample_factory/utils/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      208 2023-02-26 03:48:30.000000 sample-factory-2.1.1/sample_factory/utils/algo_version.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      215 2023-02-26 03:48:30.000000 sample-factory-2.1.1/sample_factory/utils/attr_dict.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1607 2023-02-26 03:48:30.000000 sample-factory-2.1.1/sample_factory/utils/decay.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2983 2023-02-26 03:48:30.000000 sample-factory-2.1.1/sample_factory/utils/dicts.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      986 2023-02-26 03:48:30.000000 sample-factory-2.1.1/sample_factory/utils/get_available_gpus.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      953 2023-02-26 03:48:30.000000 sample-factory-2.1.1/sample_factory/utils/gifs.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     3428 2023-02-26 03:48:30.000000 sample-factory-2.1.1/sample_factory/utils/gpu_utils.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      361 2023-02-26 03:48:30.000000 sample-factory-2.1.1/sample_factory/utils/network.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     3115 2023-02-26 03:48:30.000000 sample-factory-2.1.1/sample_factory/utils/normalize.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     2930 2023-02-26 03:48:30.000000 sample-factory-2.1.1/sample_factory/utils/tb.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     4970 2023-02-26 03:48:30.000000 sample-factory-2.1.1/sample_factory/utils/timing.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      777 2023-02-26 03:48:30.000000 sample-factory-2.1.1/sample_factory/utils/typing.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    13850 2023-02-26 03:48:30.000000 sample-factory-2.1.1/sample_factory/utils/utils.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1774 2023-02-26 03:48:30.000000 sample-factory-2.1.1/sample_factory/utils/wandb_utils.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-19 08:22:20.588728 sample-factory-2.1.1/sample_factory.egg-info/
+-rw-rw-r--   0 alex      (1000) alex      (1000)    10876 2023-06-19 08:22:20.000000 sample-factory-2.1.1/sample_factory.egg-info/PKG-INFO
+-rw-rw-r--   0 alex      (1000) alex      (1000)    12398 2023-06-19 08:22:20.000000 sample-factory-2.1.1/sample_factory.egg-info/SOURCES.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)        1 2023-06-19 08:22:20.000000 sample-factory-2.1.1/sample_factory.egg-info/dependency_links.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)      684 2023-06-19 08:22:20.000000 sample-factory-2.1.1/sample_factory.egg-info/requires.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)       27 2023-06-19 08:22:20.000000 sample-factory-2.1.1/sample_factory.egg-info/top_level.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)       38 2023-06-19 08:22:20.628728 sample-factory-2.1.1/setup.cfg
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2602 2023-06-19 04:09:10.000000 sample-factory-2.1.1/setup.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-19 08:22:20.596728 sample-factory-2.1.1/sf_examples/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-02-26 03:48:30.000000 sample-factory-2.1.1/sf_examples/__init__.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-19 08:22:20.596728 sample-factory-2.1.1/sf_examples/atari/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-02-26 03:48:30.000000 sample-factory-2.1.1/sf_examples/atari/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1554 2023-02-26 03:48:30.000000 sample-factory-2.1.1/sf_examples/atari/atari_params.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     5004 2023-02-26 03:48:30.000000 sample-factory-2.1.1/sf_examples/atari/atari_utils.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      350 2023-02-26 03:48:30.000000 sample-factory-2.1.1/sf_examples/atari/enjoy_atari.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-19 08:22:20.596728 sample-factory-2.1.1/sf_examples/atari/experiments/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-02-26 03:48:30.000000 sample-factory-2.1.1/sf_examples/atari/experiments/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      859 2023-02-26 03:48:30.000000 sample-factory-2.1.1/sf_examples/atari/experiments/atari_envs.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      962 2023-02-26 22:41:54.000000 sample-factory-2.1.1/sf_examples/atari/train_atari.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-19 08:22:20.596728 sample-factory-2.1.1/sf_examples/brax/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-02-26 03:48:30.000000 sample-factory-2.1.1/sf_examples/brax/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     6839 2023-02-26 03:48:30.000000 sample-factory-2.1.1/sf_examples/brax/brax_render.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      370 2023-02-26 03:48:30.000000 sample-factory-2.1.1/sf_examples/brax/enjoy_brax.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-19 08:22:20.596728 sample-factory-2.1.1/sf_examples/brax/experiments/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-02-26 03:48:30.000000 sample-factory-2.1.1/sf_examples/brax/experiments/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1270 2023-02-26 03:48:30.000000 sample-factory-2.1.1/sf_examples/brax/experiments/brax_basic_envs.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      324 2023-02-26 03:48:30.000000 sample-factory-2.1.1/sf_examples/brax/experiments/sbatch_timeout_brax.sh
+-rw-rw-r--   0 alex      (1000) alex      (1000)     7944 2023-02-26 03:48:30.000000 sample-factory-2.1.1/sf_examples/brax/train_brax.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-19 08:22:20.600728 sample-factory-2.1.1/sf_examples/dmlab/
+-rw-rw-r--   0 alex      (1000) alex      (1000)      166 2023-02-26 03:48:30.000000 sample-factory-2.1.1/sf_examples/dmlab/README.md
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-02-26 03:48:30.000000 sample-factory-2.1.1/sf_examples/dmlab/__init__.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-19 08:22:20.600728 sample-factory-2.1.1/sf_examples/dmlab/command_line/
+-rwxrwxr-x   0 alex      (1000) alex      (1000)      636 2023-05-02 05:55:45.000000 sample-factory-2.1.1/sf_examples/dmlab/command_line/train_dmlab30.sh
+-rwxrwxr-x   0 alex      (1000) alex      (1000)      799 2023-05-02 05:55:45.000000 sample-factory-2.1.1/sf_examples/dmlab/command_line/train_dmlab30_server_pbt.sh
+-rw-rw-r--   0 alex      (1000) alex      (1000)     7874 2023-02-26 03:48:30.000000 sample-factory-2.1.1/sf_examples/dmlab/dmlab30.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    10329 2023-02-26 03:48:30.000000 sample-factory-2.1.1/sf_examples/dmlab/dmlab_env.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     9751 2023-05-02 05:55:45.000000 sample-factory-2.1.1/sf_examples/dmlab/dmlab_gym.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    10344 2023-02-26 03:48:30.000000 sample-factory-2.1.1/sf_examples/dmlab/dmlab_level_cache.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     3501 2023-02-26 03:48:30.000000 sample-factory-2.1.1/sf_examples/dmlab/dmlab_model.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     3261 2023-02-26 03:48:30.000000 sample-factory-2.1.1/sf_examples/dmlab/dmlab_params.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     6464 2023-02-26 03:48:30.000000 sample-factory-2.1.1/sf_examples/dmlab/dmlab_populate_cache.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      289 2023-02-26 03:48:30.000000 sample-factory-2.1.1/sf_examples/dmlab/dmlab_utils.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      349 2023-02-26 03:48:30.000000 sample-factory-2.1.1/sf_examples/dmlab/enjoy_dmlab.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-19 08:22:20.600728 sample-factory-2.1.1/sf_examples/dmlab/experiments/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-02-26 03:48:30.000000 sample-factory-2.1.1/sf_examples/dmlab/experiments/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1376 2023-02-26 03:48:30.000000 sample-factory-2.1.1/sf_examples/dmlab/experiments/dmlab30.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     3610 2023-05-02 05:55:45.000000 sample-factory-2.1.1/sf_examples/dmlab/train_dmlab.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-19 08:22:20.600728 sample-factory-2.1.1/sf_examples/dmlab/wrappers/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-02-26 03:48:30.000000 sample-factory-2.1.1/sf_examples/dmlab/wrappers/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1429 2023-02-26 03:48:30.000000 sample-factory-2.1.1/sf_examples/dmlab/wrappers/reward_shaping.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      365 2023-02-26 03:48:30.000000 sample-factory-2.1.1/sf_examples/enjoy_custom_env_custom_model.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      358 2023-02-26 03:48:30.000000 sample-factory-2.1.1/sf_examples/enjoy_custom_multi_env.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      389 2023-02-26 22:42:16.000000 sample-factory-2.1.1/sf_examples/enjoy_gym_env.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-19 08:22:20.600728 sample-factory-2.1.1/sf_examples/envpool/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-02-26 03:48:30.000000 sample-factory-2.1.1/sf_examples/envpool/__init__.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-19 08:22:20.600728 sample-factory-2.1.1/sf_examples/envpool/atari/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-02-26 03:48:30.000000 sample-factory-2.1.1/sf_examples/envpool/atari/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      350 2023-02-26 03:48:30.000000 sample-factory-2.1.1/sf_examples/envpool/atari/enjoy_envpool_atari.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2045 2023-02-26 03:48:30.000000 sample-factory-2.1.1/sf_examples/envpool/atari/envpool_atari_params.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2080 2023-06-19 08:13:13.000000 sample-factory-2.1.1/sf_examples/envpool/atari/envpool_atari_utils.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1062 2023-02-26 03:48:30.000000 sample-factory-2.1.1/sf_examples/envpool/atari/train_envpool_atari.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      721 2023-02-26 03:48:30.000000 sample-factory-2.1.1/sf_examples/envpool/envpool_utils.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2496 2023-02-26 03:48:30.000000 sample-factory-2.1.1/sf_examples/envpool/envpool_wrappers.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-19 08:22:20.600728 sample-factory-2.1.1/sf_examples/envpool/mujoco/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-02-26 03:48:30.000000 sample-factory-2.1.1/sf_examples/envpool/mujoco/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      323 2023-02-26 03:48:30.000000 sample-factory-2.1.1/sf_examples/envpool/mujoco/enjoy_envpool_mujoco.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     3599 2023-02-26 03:48:30.000000 sample-factory-2.1.1/sf_examples/envpool/mujoco/envpool_mujoco_params.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1623 2023-02-26 03:48:30.000000 sample-factory-2.1.1/sf_examples/envpool/mujoco/envpool_mujoco_utils.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-19 08:22:20.600728 sample-factory-2.1.1/sf_examples/envpool/mujoco/experiments/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-02-26 03:48:30.000000 sample-factory-2.1.1/sf_examples/envpool/mujoco/experiments/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1506 2023-02-26 03:48:30.000000 sample-factory-2.1.1/sf_examples/envpool/mujoco/experiments/mujoco_envpool.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1116 2023-02-26 03:48:30.000000 sample-factory-2.1.1/sf_examples/envpool/mujoco/train_envpool_mujoco.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-19 08:22:20.600728 sample-factory-2.1.1/sf_examples/isaacgym_examples/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-02-26 03:48:30.000000 sample-factory-2.1.1/sf_examples/isaacgym_examples/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      543 2023-02-26 03:48:30.000000 sample-factory-2.1.1/sf_examples/isaacgym_examples/enjoy_isaacgym.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-19 08:22:20.600728 sample-factory-2.1.1/sf_examples/isaacgym_examples/experiments/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-02-26 03:48:30.000000 sample-factory-2.1.1/sf_examples/isaacgym_examples/experiments/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1339 2023-02-26 03:48:30.000000 sample-factory-2.1.1/sf_examples/isaacgym_examples/experiments/isaacgym_allegrohand.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1353 2023-02-26 03:48:30.000000 sample-factory-2.1.1/sf_examples/isaacgym_examples/experiments/isaacgym_ant.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1351 2023-02-26 03:48:30.000000 sample-factory-2.1.1/sf_examples/isaacgym_examples/experiments/isaacgym_basic_envs.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1358 2023-02-26 03:48:30.000000 sample-factory-2.1.1/sf_examples/isaacgym_examples/experiments/isaacgym_humanoid.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      321 2023-02-26 03:48:30.000000 sample-factory-2.1.1/sf_examples/isaacgym_examples/experiments/isaacgym_runs.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    13738 2023-02-26 03:48:30.000000 sample-factory-2.1.1/sf_examples/isaacgym_examples/train_isaacgym.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-19 08:22:20.604728 sample-factory-2.1.1/sf_examples/mujoco/
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1647 2023-02-26 03:48:30.000000 sample-factory-2.1.1/sf_examples/mujoco/README.md
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-02-26 03:48:30.000000 sample-factory-2.1.1/sf_examples/mujoco/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      353 2023-02-26 03:48:30.000000 sample-factory-2.1.1/sf_examples/mujoco/enjoy_mujoco.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-19 08:22:20.604728 sample-factory-2.1.1/sf_examples/mujoco/experiments/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-02-26 03:48:30.000000 sample-factory-2.1.1/sf_examples/mujoco/experiments/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1074 2023-02-26 03:48:30.000000 sample-factory-2.1.1/sf_examples/mujoco/experiments/mujoco_all_envs.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1229 2023-02-26 03:48:30.000000 sample-factory-2.1.1/sf_examples/mujoco/mujoco_params.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1255 2023-02-26 03:48:30.000000 sample-factory-2.1.1/sf_examples/mujoco/mujoco_utils.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      989 2023-02-26 22:42:54.000000 sample-factory-2.1.1/sf_examples/mujoco/train_mujoco.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-19 08:22:20.604728 sample-factory-2.1.1/sf_examples/sampler/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-02-26 03:48:30.000000 sample-factory-2.1.1/sf_examples/sampler/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2171 2023-02-26 03:48:30.000000 sample-factory-2.1.1/sf_examples/sampler/use_simplified_sampling_api.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     5362 2023-02-26 03:48:30.000000 sample-factory-2.1.1/sf_examples/train_custom_env_custom_model.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     5765 2023-02-26 03:48:30.000000 sample-factory-2.1.1/sf_examples/train_custom_multi_env.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1369 2023-02-26 03:48:30.000000 sample-factory-2.1.1/sf_examples/train_gym_env.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-19 08:22:20.604728 sample-factory-2.1.1/sf_examples/vizdoom/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-02-26 03:48:30.000000 sample-factory-2.1.1/sf_examples/vizdoom/__init__.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-19 08:22:20.604728 sample-factory-2.1.1/sf_examples/vizdoom/custom_env/
+-rw-rw-r--   0 alex      (1000) alex      (1000)      984 2023-02-26 03:48:30.000000 sample-factory-2.1.1/sf_examples/vizdoom/custom_env/custom_doom_env.cfg
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2704 2023-02-26 03:48:30.000000 sample-factory-2.1.1/sf_examples/vizdoom/custom_env/custom_doom_env.wad
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-19 08:22:20.604728 sample-factory-2.1.1/sf_examples/vizdoom/doom/
+-rw-rw-r--   0 alex      (1000) alex      (1000)      225 2023-02-26 03:48:30.000000 sample-factory-2.1.1/sf_examples/vizdoom/doom/README.md
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-02-26 03:48:30.000000 sample-factory-2.1.1/sf_examples/vizdoom/doom/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     4989 2023-02-26 03:48:30.000000 sample-factory-2.1.1/sf_examples/vizdoom/doom/action_space.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    25204 2023-02-26 03:48:30.000000 sample-factory-2.1.1/sf_examples/vizdoom/doom/doom_gym.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1718 2023-02-26 03:48:30.000000 sample-factory-2.1.1/sf_examples/vizdoom/doom/doom_model.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2816 2023-02-26 03:48:30.000000 sample-factory-2.1.1/sf_examples/vizdoom/doom/doom_params.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1946 2023-02-26 03:48:30.000000 sample-factory-2.1.1/sf_examples/vizdoom/doom/doom_play_demo.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      927 2023-02-26 03:48:30.000000 sample-factory-2.1.1/sf_examples/vizdoom/doom/doom_render.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    13544 2023-02-26 03:48:30.000000 sample-factory-2.1.1/sf_examples/vizdoom/doom/doom_utils.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     8004 2023-02-26 03:48:30.000000 sample-factory-2.1.1/sf_examples/vizdoom/doom/multi_agent_match.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-19 08:22:20.604728 sample-factory-2.1.1/sf_examples/vizdoom/doom/multiplayer/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-02-26 03:48:30.000000 sample-factory-2.1.1/sf_examples/vizdoom/doom/multiplayer/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     9272 2023-02-26 03:48:30.000000 sample-factory-2.1.1/sf_examples/vizdoom/doom/multiplayer/doom_multiagent.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    14057 2023-02-26 03:48:30.000000 sample-factory-2.1.1/sf_examples/vizdoom/doom/multiplayer/doom_multiagent_wrapper.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      790 2023-02-26 03:48:30.000000 sample-factory-2.1.1/sf_examples/vizdoom/doom/play_doom.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      606 2023-02-26 03:48:30.000000 sample-factory-2.1.1/sf_examples/vizdoom/doom/sample_env.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-19 08:22:20.628728 sample-factory-2.1.1/sf_examples/vizdoom/doom/scenarios/
+-rw-rw-r--   0 alex      (1000) alex      (1000)      924 2023-02-26 03:48:30.000000 sample-factory-2.1.1/sf_examples/vizdoom/doom/scenarios/basic.cfg
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2704 2023-02-26 03:48:30.000000 sample-factory-2.1.1/sf_examples/vizdoom/doom/scenarios/basic.wad
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1078 2023-02-26 03:48:30.000000 sample-factory-2.1.1/sf_examples/vizdoom/doom/scenarios/battle.cfg
+-rw-rw-r--   0 alex      (1000) alex      (1000)    15496 2023-02-26 03:48:30.000000 sample-factory-2.1.1/sf_examples/vizdoom/doom/scenarios/battle.wad
+-rw-rw-r--   0 alex      (1000) alex      (1000)    82549 2023-02-26 03:48:30.000000 sample-factory-2.1.1/sf_examples/vizdoom/doom/scenarios/battle2.wad
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1006 2023-02-26 03:48:30.000000 sample-factory-2.1.1/sf_examples/vizdoom/doom/scenarios/battle2_continuous_turning.cfg
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1071 2023-02-26 03:48:30.000000 sample-factory-2.1.1/sf_examples/vizdoom/doom/scenarios/battle_continuous_turning.cfg
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1052 2023-02-26 03:48:30.000000 sample-factory-2.1.1/sf_examples/vizdoom/doom/scenarios/cig.cfg
+-rw-rw-r--   0 alex      (1000) alex      (1000)   214730 2023-02-26 03:48:30.000000 sample-factory-2.1.1/sf_examples/vizdoom/doom/scenarios/cig.wad
+-rw-rw-r--   0 alex      (1000) alex      (1000)      891 2023-02-26 03:48:30.000000 sample-factory-2.1.1/sf_examples/vizdoom/doom/scenarios/deadly_corridor.cfg
+-rw-rw-r--   0 alex      (1000) alex      (1000)    10048 2023-02-26 03:48:30.000000 sample-factory-2.1.1/sf_examples/vizdoom/doom/scenarios/deadly_corridor.wad
+-rw-rw-r--   0 alex      (1000) alex      (1000)      901 2023-02-26 03:48:30.000000 sample-factory-2.1.1/sf_examples/vizdoom/doom/scenarios/defend_the_center.cfg
+-rw-rw-r--   0 alex      (1000) alex      (1000)     6478 2023-02-26 03:48:30.000000 sample-factory-2.1.1/sf_examples/vizdoom/doom/scenarios/defend_the_center.wad
+-rw-rw-r--   0 alex      (1000) alex      (1000)      825 2023-02-26 03:48:30.000000 sample-factory-2.1.1/sf_examples/vizdoom/doom/scenarios/defend_the_line.cfg
+-rw-rw-r--   0 alex      (1000) alex      (1000)     4139 2023-02-26 03:48:30.000000 sample-factory-2.1.1/sf_examples/vizdoom/doom/scenarios/defend_the_line.wad
+-rw-rw-r--   0 alex      (1000) alex      (1000)  2109396 2023-02-26 03:48:30.000000 sample-factory-2.1.1/sf_examples/vizdoom/doom/scenarios/dwango5.wad
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1469 2023-02-26 03:48:30.000000 sample-factory-2.1.1/sf_examples/vizdoom/doom/scenarios/dwango5_dm.cfg
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1569 2023-02-26 03:48:30.000000 sample-factory-2.1.1/sf_examples/vizdoom/doom/scenarios/dwango5_dm_continuous_weap.cfg
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1580 2023-02-26 03:48:30.000000 sample-factory-2.1.1/sf_examples/vizdoom/doom/scenarios/freedm.cfg
+-rw-rw-r--   0 alex      (1000) alex      (1000) 21112116 2023-02-26 03:48:30.000000 sample-factory-2.1.1/sf_examples/vizdoom/doom/scenarios/freedm.wad
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1044 2023-02-26 03:48:30.000000 sample-factory-2.1.1/sf_examples/vizdoom/doom/scenarios/health_gathering.cfg
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2837 2023-02-26 03:48:30.000000 sample-factory-2.1.1/sf_examples/vizdoom/doom/scenarios/health_gathering.wad
+-rw-rw-r--   0 alex      (1000) alex      (1000)      868 2023-02-26 03:48:30.000000 sample-factory-2.1.1/sf_examples/vizdoom/doom/scenarios/health_gathering_supreme.cfg
+-rw-rw-r--   0 alex      (1000) alex      (1000)    23206 2023-02-26 03:48:30.000000 sample-factory-2.1.1/sf_examples/vizdoom/doom/scenarios/health_gathering_supreme.wad
+-rw-rw-r--   0 alex      (1000) alex      (1000)      947 2023-02-26 03:48:30.000000 sample-factory-2.1.1/sf_examples/vizdoom/doom/scenarios/my_way_home.cfg
+-rw-rw-r--   0 alex      (1000) alex      (1000)    28469 2023-02-26 03:48:30.000000 sample-factory-2.1.1/sf_examples/vizdoom/doom/scenarios/my_way_home.wad
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1578 2023-02-26 03:48:30.000000 sample-factory-2.1.1/sf_examples/vizdoom/doom/scenarios/ssl2.cfg
+-rw-rw-r--   0 alex      (1000) alex      (1000)   330798 2023-02-26 03:48:30.000000 sample-factory-2.1.1/sf_examples/vizdoom/doom/scenarios/ssl2.wad
+-rw-rw-r--   0 alex      (1000) alex      (1000)      864 2023-02-26 03:48:30.000000 sample-factory-2.1.1/sf_examples/vizdoom/doom/scenarios/two_colors_easy.cfg
+-rw-rw-r--   0 alex      (1000) alex      (1000)     4810 2023-02-26 03:48:30.000000 sample-factory-2.1.1/sf_examples/vizdoom/doom/scenarios/two_colors_easy.wad
+-rw-rw-r--   0 alex      (1000) alex      (1000)      864 2023-02-26 03:48:30.000000 sample-factory-2.1.1/sf_examples/vizdoom/doom/scenarios/two_colors_hard.cfg
+-rw-rw-r--   0 alex      (1000) alex      (1000)     5096 2023-02-26 03:48:30.000000 sample-factory-2.1.1/sf_examples/vizdoom/doom/scenarios/two_colors_hard.wad
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-19 08:22:20.628728 sample-factory-2.1.1/sf_examples/vizdoom/doom/scripts/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-02-26 03:48:30.000000 sample-factory-2.1.1/sf_examples/vizdoom/doom/scripts/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1076 2023-02-26 03:48:30.000000 sample-factory-2.1.1/sf_examples/vizdoom/doom/scripts/generate_bots.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-19 08:22:20.628728 sample-factory-2.1.1/sf_examples/vizdoom/doom/wrappers/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-02-26 03:48:30.000000 sample-factory-2.1.1/sf_examples/vizdoom/doom/wrappers/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     3767 2023-02-26 03:48:30.000000 sample-factory-2.1.1/sf_examples/vizdoom/doom/wrappers/additional_input.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2386 2023-02-26 03:48:30.000000 sample-factory-2.1.1/sf_examples/vizdoom/doom/wrappers/bot_difficulty.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1901 2023-02-26 03:48:30.000000 sample-factory-2.1.1/sf_examples/vizdoom/doom/wrappers/exploration.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2348 2023-02-26 03:48:30.000000 sample-factory-2.1.1/sf_examples/vizdoom/doom/wrappers/multiplayer_stats.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1976 2023-02-26 03:48:30.000000 sample-factory-2.1.1/sf_examples/vizdoom/doom/wrappers/observation_space.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     9196 2023-02-26 03:48:30.000000 sample-factory-2.1.1/sf_examples/vizdoom/doom/wrappers/reward_shaping.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-19 08:22:20.628728 sample-factory-2.1.1/sf_examples/vizdoom/doom/wrappers/scenario_wrappers/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-02-26 03:48:30.000000 sample-factory-2.1.1/sf_examples/vizdoom/doom/wrappers/scenario_wrappers/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1207 2023-02-26 03:48:30.000000 sample-factory-2.1.1/sf_examples/vizdoom/doom/wrappers/scenario_wrappers/gathering_reward_shaping.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1129 2023-02-26 03:48:30.000000 sample-factory-2.1.1/sf_examples/vizdoom/doom/wrappers/step_human_input.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      860 2023-02-26 03:48:30.000000 sample-factory-2.1.1/sf_examples/vizdoom/enjoy_custom_vizdoom_env.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      814 2023-02-26 03:48:30.000000 sample-factory-2.1.1/sf_examples/vizdoom/enjoy_vizdoom.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2362 2023-02-26 03:48:30.000000 sample-factory-2.1.1/sf_examples/vizdoom/train_custom_vizdoom_env.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1538 2023-02-26 22:51:35.000000 sample-factory-2.1.1/sf_examples/vizdoom/train_vizdoom.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-19 08:22:20.628728 sample-factory-2.1.1/tests/
+-rw-rw-r--   0 alex      (1000) alex      (1000)     3811 2023-02-26 03:48:30.000000 sample-factory-2.1.1/tests/test_launcher.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      641 2023-02-26 03:48:30.000000 sample-factory-2.1.1/tests/test_precheck.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1982 2023-02-26 03:48:30.000000 sample-factory-2.1.1/tests/test_utils.py
```

### Comparing `sample-factory-2.0.3/CONTRIBUTING.md` & `sample-factory-2.1.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `sample-factory-2.0.3/LICENSE` & `sample-factory-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sample-factory-2.0.3/PKG-INFO` & `sample-factory-2.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sample-factory
-Version: 2.0.3
+Version: 2.1.1
 Summary: High throughput asynchronous reinforcement learning framework
 Home-page: https://github.com/alex-petrenko/sample-factory
 Author: Aleksei Petrenko
 License: MIT
 Project-URL: Github, https://github.com/alex-petrenko/sample-factory
 Project-URL: Videos, https://sites.google.com/view/sample-factory
 Keywords: asynchronous reinforcement learning policy gradient ppo appo impala ai
```

### Comparing `sample-factory-2.0.3/README.md` & `sample-factory-2.1.1/README.md`

 * *Files identical despite different names*

### Comparing `sample-factory-2.0.3/docs/01-get-started/basic-usage.md` & `sample-factory-2.1.1/docs/01-get-started/basic-usage.md`

 * *Files identical despite different names*

### Comparing `sample-factory-2.0.3/docs/01-get-started/installation.md` & `sample-factory-2.1.1/docs/01-get-started/installation.md`

 * *Files identical despite different names*

### Comparing `sample-factory-2.0.3/docs/02-configuration/cfg-params.md` & `sample-factory-2.1.1/docs/02-configuration/cfg-params.md`

 * *Files 2% similar despite different names*

```diff
@@ -120,15 +120,15 @@
                         experiment folder with this name aleady exists the
                         experiment will be RESUMED!Any parameters passed from
                         command line that do not match the parameters stored
                         in the experiment config.json file will be overridden.
                         (default: default_experiment)
   --train_dir TRAIN_DIR
                         Root for all experiments (default:
-                        /home/alex/all/projects/sf2/train_dir)
+                        /home/alex/all/projects/sample-factory/train_dir)
   --restart_behavior {resume,restart,overwrite}
                         How to handle the experiment if the directory with the
                         same name already exists. "resume" (default) will
                         resume the experiment, "restart" will preserve the
                         existing experiment folder under a different name
                         (with "old" suffix) and will start training from
                         scratch, "overwrite" will delete the existing
@@ -483,16 +483,18 @@
                         Start saving "best" policies after this many env steps
                         to filter lucky episodes that succeed and dominate the
                         statistics early on (default: 100000)
   --benchmark BENCHMARK
                         Benchmark mode (default: False)
   --encoder_mlp_layers [ENCODER_MLP_LAYERS [ENCODER_MLP_LAYERS ...]]
                         In case of MLP encoder, sizes of layers to use. This
-                        is ignored if observations are images. (default: [512,
-                        512])
+                        is ignored if observations are images. To use this
+                        parameter from command line, omit the = sign and
+                        separate values with spaces, e.g. --encoder_mlp_layers
+                        256 128 64 (default: [512, 512])
   --encoder_conv_architecture {convnet_simple,convnet_impala,convnet_atari,resnet_impala}
                         Architecture of the convolutional encoder. See
                         models.py for details. VizDoom and DMLab examples
                         demonstrate how to define custom architectures.
                         (default: convnet_simple)
   --encoder_conv_mlp_layers [ENCODER_CONV_MLP_LAYERS [ENCODER_CONV_MLP_LAYERS ...]]
                         Optional fully connected layers after the
```

### Comparing `sample-factory-2.0.3/docs/02-configuration/configuration.md` & `sample-factory-2.1.1/docs/02-configuration/configuration.md`

 * *Files identical despite different names*

### Comparing `sample-factory-2.0.3/docs/03-customization/custom-environments.md` & `sample-factory-2.1.1/docs/03-customization/custom-environments.md`

 * *Files identical despite different names*

### Comparing `sample-factory-2.0.3/docs/03-customization/custom-models.md` & `sample-factory-2.1.1/docs/03-customization/custom-models.md`

 * *Files identical despite different names*

### Comparing `sample-factory-2.0.3/docs/03-customization/custom-multi-agent-environments.md` & `sample-factory-2.1.1/docs/03-customization/custom-multi-agent-environments.md`

 * *Files identical despite different names*

### Comparing `sample-factory-2.0.3/docs/04-experiments/experiment-launcher.md` & `sample-factory-2.1.1/docs/04-experiments/experiment-launcher.md`

 * *Files identical despite different names*

### Comparing `sample-factory-2.0.3/docs/04-experiments/slurm-details.md` & `sample-factory-2.1.1/docs/04-experiments/slurm-details.md`

 * *Files identical despite different names*

### Comparing `sample-factory-2.0.3/docs/05-monitoring/custom-metrics.md` & `sample-factory-2.1.1/docs/05-monitoring/custom-metrics.md`

 * *Files identical despite different names*

### Comparing `sample-factory-2.0.3/docs/05-monitoring/metrics-reference.md` & `sample-factory-2.1.1/docs/05-monitoring/metrics-reference.md`

 * *Files identical despite different names*

### Comparing `sample-factory-2.0.3/docs/05-monitoring/tensorboard.md` & `sample-factory-2.1.1/docs/05-monitoring/tensorboard.md`

 * *Files identical despite different names*

### Comparing `sample-factory-2.0.3/docs/05-monitoring/wandb.md` & `sample-factory-2.1.1/docs/05-monitoring/wandb.md`

 * *Files identical despite different names*

### Comparing `sample-factory-2.0.3/docs/06-architecture/message-passing.md` & `sample-factory-2.1.1/docs/06-architecture/message-passing.md`

 * *Files identical despite different names*

### Comparing `sample-factory-2.0.3/docs/06-architecture/overview.md` & `sample-factory-2.1.1/docs/06-architecture/overview.md`

 * *Files identical despite different names*

### Comparing `sample-factory-2.0.3/docs/07-advanced-topics/batched-non-batched.md` & `sample-factory-2.1.1/docs/07-advanced-topics/batched-non-batched.md`

 * *Files identical despite different names*

### Comparing `sample-factory-2.0.3/docs/07-advanced-topics/double-buffered.md` & `sample-factory-2.1.1/docs/07-advanced-topics/double-buffered.md`

 * *Files identical despite different names*

### Comparing `sample-factory-2.0.3/docs/07-advanced-topics/inactive-agents.md` & `sample-factory-2.1.1/docs/07-advanced-topics/inactive-agents.md`

 * *Files identical despite different names*

### Comparing `sample-factory-2.0.3/docs/07-advanced-topics/multi-policy-training.md` & `sample-factory-2.1.1/docs/07-advanced-topics/multi-policy-training.md`

 * *Files identical despite different names*

### Comparing `sample-factory-2.0.3/docs/07-advanced-topics/normalizations.md` & `sample-factory-2.1.1/docs/07-advanced-topics/normalizations.md`

 * *Files identical despite different names*

### Comparing `sample-factory-2.0.3/docs/07-advanced-topics/observer.md` & `sample-factory-2.1.1/docs/07-advanced-topics/observer.md`

 * *Files identical despite different names*

### Comparing `sample-factory-2.0.3/docs/07-advanced-topics/passing-info.md` & `sample-factory-2.1.1/docs/07-advanced-topics/passing-info.md`

 * *Files identical despite different names*

### Comparing `sample-factory-2.0.3/docs/07-advanced-topics/pbt.md` & `sample-factory-2.1.1/docs/07-advanced-topics/pbt.md`

 * *Files 2% similar despite different names*

```diff
@@ -106,15 +106,15 @@
 Use `--with_pbt=True` to enable PBT. It is important also to set `--num_policies` to the number of agents in the population.
 
 ### Command-line examples
 
 Training on DMLab-30 with a 4-agent population on a 4-GPU machine:
 
 ```bash
-python -m sf_examples.dmlab.train_dmlab --env=dmlab_30 --train_for_env_steps=10000000000 --algo=APPO --gamma=0.99 --use_rnn=True --num_workers=90 --num_envs_per_worker=12 --num_epochs=1 --rollout=32 --recurrence=32 --batch_size=2048 --benchmark=False --max_grad_norm=0.0 --dmlab_renderer=software --decorrelate_experience_max_seconds=120 --reset_timeout_seconds=300 --encoder_conv_architecture=resnet_impala --encoder_conv_mlp_layers=512 --nonlinearity=relu --rnn_type=lstm --dmlab_extended_action_set=True --num_policies=4 --pbt_replace_reward_gap=0.05 --pbt_replace_reward_gap_absolute=5.0 --pbt_period_env_steps=10000000 --pbt_start_mutation=100000000 --with_pbt=True --experiment=dmlab_30_resnet_4pbt_w90_v12 --dmlab_one_task_per_worker=True --set_workers_cpu_affinity=True --max_policy_lag=35 --pbt_target_objective=dmlab_target_objective --dmlab30_dataset=~/datasets/brady_konkle_oliva2008 --dmlab_use_level_cache=True --dmlab_level_cache_path=/home/user/dmlab_cache
+python -m sf_examples.dmlab.train_dmlab --env=dmlab_30 --train_for_env_steps=10000000000 --algo=APPO --gamma=0.99 --use_rnn=True --num_workers=90 --num_envs_per_worker=12 --num_epochs=1 --rollout=32 --recurrence=32 --batch_size=2048 --benchmark=False --max_grad_norm=0.0 --dmlab_renderer=software --decorrelate_experience_max_seconds=120 --encoder_conv_architecture=resnet_impala --encoder_conv_mlp_layers=512 --nonlinearity=relu --rnn_type=lstm --dmlab_extended_action_set=True --num_policies=4 --pbt_replace_reward_gap=0.05 --pbt_replace_reward_gap_absolute=5.0 --pbt_period_env_steps=10000000 --pbt_start_mutation=100000000 --with_pbt=True --experiment=dmlab_30_resnet_4pbt_w90_v12 --dmlab_one_task_per_worker=True --set_workers_cpu_affinity=True --max_policy_lag=35 --pbt_target_objective=dmlab_target_objective --dmlab30_dataset=~/datasets/brady_konkle_oliva2008 --dmlab_use_level_cache=True --dmlab_level_cache_path=/home/user/dmlab_cache
 ```
 
 PBT for VizDoom (8 agents, 4-GPU machine):
 
 ```bash
 python -m sf_examples.vizdoom.train_vizdoom --env=doom_deathmatch_bots --train_for_seconds=3600000 --algo=APPO --use_rnn=True --gamma=0.995 --env_frameskip=2 --num_workers=80 --num_envs_per_worker=24 --num_policies=8 --batch_size=2048 --res_w=128 --res_h=72 --wide_aspect_ratio=False --with_pbt=True --pbt_period_env_steps=5000000 --experiment=doom_deathmatch_bots
 ```
```

### Comparing `sample-factory-2.0.3/docs/07-advanced-topics/policy-lag.md` & `sample-factory-2.1.1/docs/07-advanced-topics/policy-lag.md`

 * *Files identical despite different names*

### Comparing `sample-factory-2.0.3/docs/07-advanced-topics/profiling.md` & `sample-factory-2.1.1/docs/07-advanced-topics/profiling.md`

 * *Files identical despite different names*

### Comparing `sample-factory-2.0.3/docs/07-advanced-topics/serial-mode.md` & `sample-factory-2.1.1/docs/07-advanced-topics/serial-mode.md`

 * *Files identical despite different names*

### Comparing `sample-factory-2.0.3/docs/07-advanced-topics/sync-async.md` & `sample-factory-2.1.1/docs/07-advanced-topics/sync-async.md`

 * *Files identical despite different names*

### Comparing `sample-factory-2.0.3/docs/08-miscellaneous/tests.md` & `sample-factory-2.1.1/docs/08-miscellaneous/tests.md`

 * *Files identical despite different names*

### Comparing `sample-factory-2.0.3/docs/08-miscellaneous/v1-to-v2.md` & `sample-factory-2.1.1/docs/08-miscellaneous/v1-to-v2.md`

 * *Files identical despite different names*

### Comparing `sample-factory-2.0.3/docs/09-environment-integrations/atari.md` & `sample-factory-2.1.1/docs/09-environment-integrations/atari.md`

 * *Files 11% similar despite different names*

```diff
@@ -10,16 +10,15 @@
 ```
 
 ### Running Experiments
 
 Run Atari experiments with the scripts in `sf_examples.atari`.
 
 The default parameters have been chosen to match CleanRL's configuration (see reports below) and are not tuned for throughput.
-(TODO: also provide parameters that result in the fastest training).
- 
+(see some better parameters at the end of the document).
 
 To train a model in the `BreakoutNoFrameskip-v4` environment:
 
 ```
 python -m sf_examples.atari.train_atari --algo=APPO --env=atari_breakout --experiment="Experiment Name"
 ```
 
@@ -101,7 +100,31 @@
 | atari_zaxxon                 | ZaxxonNoFrameskip-v4           | [🤗 Hub Atari-2B checkpoints](https://huggingface.co/edbeeching/atari_2B_atari_zaxxon_1111)         |
 
 
 ### Reports
 
 - Sample Factory was benchmarked on Atari against CleanRL and Baselines. Sample Factory was able to achieve similar sample efficiency as CleanRL and Baselines using the same parameters.
     - https://wandb.ai/wmfrank/atari-benchmark/reports/Atari-Sample-Factory2-Baselines-CleanRL--VmlldzoyMzEyNjIw
+
+#### Better parameters (more envs, double buffering, async learning)
+
+```
+--experiment=breakout_faster
+--env=atari_breakout
+--summaries_use_frameskip=False
+--num_workers=16
+--num_envs_per_worker=8
+--worker_num_splits=2
+--train_for_env_steps=100000000
+--rollout=32
+--normalize_input=True
+--normalize_returns=True
+--serial_mode=False
+--async_rl=True
+--batch_size=1024
+--wandb_user=<user>
+--wandb_project=sf2_atari_breakout
+--wandb_group=breakout_w16v8r32
+--with_wandb=True
+```
+
+Report: https://wandb.ai/apetrenko/sf2_atari_breakout/reports/sf2-breakout-w16v8r32--Vmlldzo0MjM1MTQ4
```

### Comparing `sample-factory-2.0.3/docs/09-environment-integrations/brax.md` & `sample-factory-2.1.1/docs/09-environment-integrations/brax.md`

 * *Files identical despite different names*

### Comparing `sample-factory-2.0.3/docs/09-environment-integrations/dmlab.md` & `sample-factory-2.1.1/docs/09-environment-integrations/dmlab.md`

 * *Files 6% similar despite different names*

```diff
@@ -16,22 +16,22 @@
 ## Running Experiments
 
 Run DMLab experiments with the scripts in `sf_examples.dmlab`. 
 
 Example of training in the DMLab watermaze environment for 1B environment steps
 
 ```
-python -m sf_examples.dmlab.train_dmlab --env=dmlab_watermaze --train_for_env_steps=1000000000 --gamma=0.99 --use_rnn=True --num_workers=90 --num_envs_per_worker=12 --num_epochs=1 --rollout=32 --recurrence=32 --batch_size=2048 --benchmark=False --max_grad_norm=0.0 --dmlab_renderer=software --decorrelate_experience_max_seconds=120 --reset_timeout_seconds=300 --encoder_conv_architecture=resnet_impala --encoder_conv_mlp_layers=512 --nonlinearity=relu --rnn_type=lstm --dmlab_extended_action_set=True --num_policies=1 --experiment=dmlab_watermaze_resnet_w90_v12 --set_workers_cpu_affinity=True --max_policy_lag=35  --dmlab30_dataset=~/datasets/brady_konkle_oliva2008 --dmlab_use_level_cache=True --dmlab_level_cache_path=/home/user/dmlab_cache
+python -m sf_examples.dmlab.train_dmlab --env=dmlab_watermaze --train_for_env_steps=1000000000 --gamma=0.99 --use_rnn=True --num_workers=90 --num_envs_per_worker=12 --num_epochs=1 --rollout=32 --recurrence=32 --batch_size=2048 --benchmark=False --max_grad_norm=0.0 --dmlab_renderer=software --decorrelate_experience_max_seconds=120 --encoder_conv_architecture=resnet_impala --encoder_conv_mlp_layers=512 --nonlinearity=relu --rnn_type=lstm --dmlab_extended_action_set=True --num_policies=1 --experiment=dmlab_watermaze_resnet_w90_v12 --set_workers_cpu_affinity=True --max_policy_lag=35  --dmlab30_dataset=~/datasets/brady_konkle_oliva2008 --dmlab_use_level_cache=True --dmlab_level_cache_path=/home/user/dmlab_cache
 ```
 
 
 DMLab-30 run on a 36-core server with 4 GPUs using Population-Based Training with 4 agents:
 
 ```
-python -m sf_examples.dmlab.train_dmlab --env=dmlab_30 --train_for_env_steps=10000000000 --gamma=0.99 --use_rnn=True --num_workers=90 --num_envs_per_worker=12 --num_epochs=1 --rollout=32 --recurrence=32 --batch_size=2048 --benchmark=False --max_grad_norm=0.0 --dmlab_renderer=software --decorrelate_experience_max_seconds=120 --reset_timeout_seconds=300 --encoder_conv_architecture=resnet_impala --encoder_conv_mlp_layers=512 --nonlinearity=relu --rnn_type=lstm --dmlab_extended_action_set=True --num_policies=4 --pbt_replace_reward_gap=0.05 --pbt_replace_reward_gap_absolute=5.0 --pbt_period_env_steps=10000000 --pbt_start_mutation=100000000 --with_pbt=True --experiment=dmlab_30_resnet_4pbt_w90_v12 --dmlab_one_task_per_worker=True --set_workers_cpu_affinity=True --max_policy_lag=35 --pbt_target_objective=dmlab_target_objective --dmlab30_dataset=~/datasets/brady_konkle_oliva2008 --dmlab_use_level_cache=True --dmlab_level_cache_path=/home/user/dmlab_cache
+python -m sf_examples.dmlab.train_dmlab --env=dmlab_30 --train_for_env_steps=10000000000 --gamma=0.99 --use_rnn=True --num_workers=90 --num_envs_per_worker=12 --num_epochs=1 --rollout=32 --recurrence=32 --batch_size=2048 --benchmark=False --max_grad_norm=0.0 --dmlab_renderer=software --decorrelate_experience_max_seconds=120 --encoder_conv_architecture=resnet_impala --encoder_conv_mlp_layers=512 --nonlinearity=relu --rnn_type=lstm --dmlab_extended_action_set=True --num_policies=4 --pbt_replace_reward_gap=0.05 --pbt_replace_reward_gap_absolute=5.0 --pbt_period_env_steps=10000000 --pbt_start_mutation=100000000 --with_pbt=True --experiment=dmlab_30_resnet_4pbt_w90_v12 --dmlab_one_task_per_worker=True --set_workers_cpu_affinity=True --max_policy_lag=35 --pbt_target_objective=dmlab_target_objective --dmlab30_dataset=~/datasets/brady_konkle_oliva2008 --dmlab_use_level_cache=True --dmlab_level_cache_path=/home/user/dmlab_cache
 ```
 
 
 ## Models
 | DMLab Command Line Parameter | DMLab Environment name | Model Checkpooints                                                           |
 | ---------------------------- | ---------------------- | ---------------------------------------------------------------------------- |
 | dmlab_30                     | DMLab-30               | [🤗 Hub DMLab30 checkpoints](https://huggingface.co/edbeeching/dmlab_30_1111) |
```

### Comparing `sample-factory-2.0.3/docs/09-environment-integrations/envpool.md` & `sample-factory-2.1.1/docs/09-environment-integrations/envpool.md`

 * *Files identical despite different names*

### Comparing `sample-factory-2.0.3/docs/09-environment-integrations/isaacgym.md` & `sample-factory-2.1.1/docs/09-environment-integrations/isaacgym.md`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 
 ### Installation
 
 Install IsaacGym from NVIDIA at https://developer.nvidia.com/isaac-gym. Installation instructions can be found in the package's docs folder. Python 3.8 is compatable with both IsaacGym and Sample-Factory
 
 Install IsaacGymEnvs from https://github.com/NVIDIA-Omniverse/IsaacGymEnvs. 
 
-
 ### Running Experiments
 
 Run IsaacGym experiments using scripts from the `sf_examples.isaacgym_examples` folder. Currently, we support the AllegroHand, Ant, Anymal, AnymalTerrain, BallBalance, Cartpole , Humanoid, and ShadowHand  environments out of the box, and more environments can be added in `train_isaacgym.py`.
 
 To run an experiment in the Ant environment:
 ```
 python -m sf_examples.isaacgym_examples.train_isaacgym --actor_worker_gpus 0 --env=Ant --train_for_env_steps=100000000  --experiment=isaacgym_ant
```

### Comparing `sample-factory-2.0.3/docs/09-environment-integrations/megaverse.md` & `sample-factory-2.1.1/docs/09-environment-integrations/megaverse.md`

 * *Files identical despite different names*

### Comparing `sample-factory-2.0.3/docs/09-environment-integrations/mujoco.md` & `sample-factory-2.1.1/docs/09-environment-integrations/mujoco.md`

 * *Files identical despite different names*

### Comparing `sample-factory-2.0.3/docs/09-environment-integrations/swarm-rl.md` & `sample-factory-2.1.1/docs/09-environment-integrations/swarm-rl.md`

 * *Files identical despite different names*

### Comparing `sample-factory-2.0.3/docs/09-environment-integrations/vizdoom.md` & `sample-factory-2.1.1/docs/09-environment-integrations/vizdoom.md`

 * *Files identical despite different names*

### Comparing `sample-factory-2.0.3/docs/10-huggingface/huggingface.md` & `sample-factory-2.1.1/docs/10-huggingface/huggingface.md`

 * *Files identical despite different names*

### Comparing `sample-factory-2.0.3/docs/11-release-notes/release-notes.md` & `sample-factory-2.1.1/docs/11-release-notes/release-notes.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,9 +1,21 @@
 # Recent releases
 
+##### v2.1.1
+
+* Windows support in serial mode (do not require `faster-fifo` on Windows)
+* Allow Torch 2 (versions 2.0.1+ seem to work fine)
+
+##### v2.1.0
+
+* Use `gymnasium` instead of `gym` dependency. See https://gymnasium.farama.org/content/basic_usage/ New compatibility
+layer added to automatically convert legacy `gym` environments to `gymnasium` environments. Still, it is likely that
+some of the user code will need to be manually updated to use `gymnasium` instead of `gym`.
+Apologies for the inconvenience, but hopefully this is the last major change before Gym API finally stabilizes.
+
 ##### v2.0.3
 
 * Added cfg parameters `--lr_adaptive_min` and `--lr_adaptive_max` to control the minimum and maximum adaptive learning rate
 * Added Brax environment support + custom brax renderer for enjoy scripts
 * Automatically set `--recurrence` based on feed-forward vs RNN training
 * Added `--enjoy_script` and `--train_script` for generating the model card when uploading to the Hugging Face Hub (thank you Andrew!)
 * Fixed video name when generating Hugging Face model card
```

### Comparing `sample-factory-2.0.3/docs/12-community/citation.md` & `sample-factory-2.1.1/docs/12-community/citation.md`

 * *Files identical despite different names*

### Comparing `sample-factory-2.0.3/docs/12-community/contribution.md` & `sample-factory-2.1.1/docs/12-community/contribution.md`

 * *Files identical despite different names*

### Comparing `sample-factory-2.0.3/docs/12-community/doc-contribution.md` & `sample-factory-2.1.1/docs/12-community/doc-contribution.md`

 * *Files 12% similar despite different names*

```diff
@@ -7,22 +7,22 @@
 ```bash
 pip install -e .[dev]
 ```
 
 * Serve the website locally
 
 ```bash
-mkdocs docs-serve
+make docs-serve
 ```
 
 you should see the website on your localhost port now.
 
 * Modify or create markdown files
-- modify / create your markdown files in ‘docs’ folder.
-- add your markdown path in the ‘nav’ section of ‘mkdocs.yml’.
+* modify / create your markdown files in ‘docs’ folder.
+* add your markdown path in the ‘nav’ section of ‘mkdocs.yml’.
 
- Example folder-yml correspondence:
+Example folder-yml correspondence:
  
 <img src="https://user-images.githubusercontent.com/30235642/176805054-9d5f1c24-b8b6-49df-90c3-039acb741af3.png" alt="docs" width="300" height="300"/>
 <img src="https://user-images.githubusercontent.com/30235642/176805061-3da4b3b6-9a18-4d87-9d06-044dc863b6e4.png" alt="yml" width="400" height="300"/>
 
 * Commit and push your changes to remote repo. Github actions will automatically push your changes to your github pages website.
```

### Comparing `sample-factory-2.0.3/docs/cfg-params.sh` & `sample-factory-2.1.1/docs/cfg-params.sh`

 * *Files identical despite different names*

### Comparing `sample-factory-2.0.3/docs/index.md` & `sample-factory-2.1.1/docs/index.md`

 * *Files identical despite different names*

### Comparing `sample-factory-2.0.3/sample_factory/algo/learning/batcher.py` & `sample-factory-2.1.1/sample_factory/algo/learning/batcher.py`

 * *Files identical despite different names*

### Comparing `sample-factory-2.0.3/sample_factory/algo/learning/learner.py` & `sample-factory-2.1.1/sample_factory/algo/learning/learner.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from __future__ import annotations
 
 import glob
 import os
-import random
 import time
 from abc import ABC, abstractmethod
 from os.path import join
 from typing import Callable, Dict, Optional, Tuple
 
 import numpy as np
 import torch
@@ -229,21 +228,24 @@
         optimizer_cls = dict(adam=torch.optim.Adam, lamb=Lamb)
         if self.cfg.optimizer not in optimizer_cls:
             raise RuntimeError(f"Unknown optimizer {self.cfg.optimizer}")
 
         optimizer_cls = optimizer_cls[self.cfg.optimizer]
         log.debug(f"Using optimizer {optimizer_cls}")
 
-        self.optimizer = optimizer_cls(
-            params,
+        optimizer_kwargs = dict(
             lr=self.cfg.learning_rate,  # use default lr only in ctor, then we use the one loaded from the checkpoint
             betas=(self.cfg.adam_beta1, self.cfg.adam_beta2),
-            eps=self.cfg.adam_eps,
         )
 
+        if self.cfg.optimizer in ["adam", "lamb"]:
+            optimizer_kwargs["eps"] = self.cfg.adam_eps
+
+        self.optimizer = optimizer_cls(params, **optimizer_kwargs)
+
         self.load_from_checkpoint(self.policy_id)
         self.param_server.init(self.actor_critic, self.train_step, self.device)
         self.policy_versions_tensor[self.policy_id] = self.train_step
 
         self.lr_scheduler = get_lr_scheduler(self.cfg)
         self.curr_lr = self.cfg.learning_rate if self.curr_lr is None else self.curr_lr
         self._apply_lr(self.curr_lr)
@@ -896,15 +898,16 @@
             stats.ratio_min = ratio_min
             stats.ratio_max = ratio_max
             stats.num_sgd_steps = var.num_sgd_steps
 
         # this caused numerical issues on some versions of PyTorch with second moment reaching infinity
         adam_max_second_moment = 0.0
         for key, tensor_state in self.optimizer.state.items():
-            adam_max_second_moment = max(tensor_state["exp_avg_sq"].max().item(), adam_max_second_moment)
+            if "exp_avg_sq" in tensor_state:
+                adam_max_second_moment = max(tensor_state["exp_avg_sq"].max().item(), adam_max_second_moment)
         stats.adam_max_second_moment = adam_max_second_moment
 
         version_diff = (var.curr_policy_version - var.mb.policy_version)[var.mb.policy_id == self.policy_id]
         stats.version_diff_avg = version_diff.mean()
         stats.version_diff_min = version_diff.min()
         stats.version_diff_max = version_diff.max()
```

### Comparing `sample-factory-2.0.3/sample_factory/algo/learning/learner_worker.py` & `sample-factory-2.1.1/sample_factory/algo/learning/learner_worker.py`

 * *Files identical despite different names*

### Comparing `sample-factory-2.0.3/sample_factory/algo/learning/rnn_utils.py` & `sample-factory-2.1.1/sample_factory/algo/learning/rnn_utils.py`

 * *Files identical despite different names*

### Comparing `sample-factory-2.0.3/sample_factory/algo/runners/runner.py` & `sample-factory-2.1.1/sample_factory/algo/runners/runner.py`

 * *Files identical despite different names*

### Comparing `sample-factory-2.0.3/sample_factory/algo/runners/runner_parallel.py` & `sample-factory-2.1.1/sample_factory/algo/runners/runner_parallel.py`

 * *Files identical despite different names*

### Comparing `sample-factory-2.0.3/sample_factory/algo/runners/runner_serial.py` & `sample-factory-2.1.1/sample_factory/algo/runners/runner_serial.py`

 * *Files identical despite different names*

### Comparing `sample-factory-2.0.3/sample_factory/algo/sampling/batched_sampling.py` & `sample-factory-2.1.1/sample_factory/algo/sampling/batched_sampling.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 
 import numbers
 from queue import Empty
 from typing import Dict, List, Optional, Tuple
 
-import gym
+import gymnasium as gym
 import numpy as np
 import torch
 from torch import Tensor
 
 from sample_factory.algo.sampling.sampling_utils import VectorEnvRunner, record_episode_statistics_wrapper_stats
 from sample_factory.algo.utils.env_info import EnvInfo, check_env_info
 from sample_factory.algo.utils.make_env import BatchedVecEnv, SequentialVectorizeWrapper, make_env_func_batched
```

### Comparing `sample-factory-2.0.3/sample_factory/algo/sampling/inference_worker.py` & `sample-factory-2.1.1/sample_factory/algo/sampling/inference_worker.py`

 * *Files identical despite different names*

### Comparing `sample-factory-2.0.3/sample_factory/algo/sampling/non_batched_sampling.py` & `sample-factory-2.1.1/sample_factory/algo/sampling/non_batched_sampling.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 
 import random
 from queue import Empty
 from typing import Any, Dict, List, Optional, Tuple
 
-import gym
+import gymnasium as gym
 import numpy as np
 
 from sample_factory.algo.sampling.sampling_utils import VectorEnvRunner, record_episode_statistics_wrapper_stats
 from sample_factory.algo.utils.agent_policy_mapping import AgentPolicyMapping
 from sample_factory.algo.utils.env_info import EnvInfo, check_env_info
 from sample_factory.algo.utils.make_env import make_env_func_non_batched
 from sample_factory.algo.utils.misc import EPISODIC, POLICY_ID_KEY
```

### Comparing `sample-factory-2.0.3/sample_factory/algo/sampling/rollout_worker.py` & `sample-factory-2.1.1/sample_factory/algo/sampling/rollout_worker.py`

 * *Files identical despite different names*

### Comparing `sample-factory-2.0.3/sample_factory/algo/sampling/sampler.py` & `sample-factory-2.1.1/sample_factory/algo/sampling/sampler.py`

 * *Files identical despite different names*

### Comparing `sample-factory-2.0.3/sample_factory/algo/sampling/sampling_utils.py` & `sample-factory-2.1.1/sample_factory/algo/sampling/sampling_utils.py`

 * *Files identical despite different names*

### Comparing `sample-factory-2.0.3/sample_factory/algo/sampling/simplified_sampling_api.py` & `sample-factory-2.1.1/sample_factory/algo/sampling/simplified_sampling_api.py`

 * *Files identical despite different names*

### Comparing `sample-factory-2.0.3/sample_factory/algo/utils/action_distributions.py` & `sample-factory-2.1.1/sample_factory/algo/utils/action_distributions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import math
 
-import gym
+import gymnasium as gym
 import numpy as np
 import torch
 from torch import Tensor
 from torch.distributions import Independent, Normal
 from torch.nn import functional
 
 from sample_factory.utils.typing import ActionSpace
```

### Comparing `sample-factory-2.0.3/sample_factory/algo/utils/agent_policy_mapping.py` & `sample-factory-2.1.1/sample_factory/algo/utils/agent_policy_mapping.py`

 * *Files identical despite different names*

### Comparing `sample-factory-2.0.3/sample_factory/algo/utils/context.py` & `sample-factory-2.1.1/sample_factory/algo/utils/context.py`

 * *Files identical despite different names*

### Comparing `sample-factory-2.0.3/sample_factory/algo/utils/env_info.py` & `sample-factory-2.1.1/sample_factory/algo/utils/env_info.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import multiprocessing
 import os
 import pickle
 from dataclasses import dataclass
 from os.path import join
 from typing import Dict, List, Optional
 
-import gym
+import gymnasium as gym
 
 from sample_factory.algo.utils.action_distributions import calc_num_actions
 from sample_factory.algo.utils.context import set_global_context, sf_global_context
 from sample_factory.algo.utils.make_env import BatchedVecEnv, NonBatchedVecEnv, make_env_func_batched
 from sample_factory.envs.env_utils import get_default_reward_shaping
 from sample_factory.utils.typing import Config
 from sample_factory.utils.utils import log, project_tmp_dir
```

### Comparing `sample-factory-2.0.3/sample_factory/algo/utils/heartbeat.py` & `sample-factory-2.1.1/sample_factory/algo/utils/heartbeat.py`

 * *Files identical despite different names*

### Comparing `sample-factory-2.0.3/sample_factory/algo/utils/make_env.py` & `sample-factory-2.1.1/sample_factory/algo/utils/make_env.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from __future__ import annotations
 
 from typing import Any, Callable, Dict, List, Optional, Sequence, Tuple, Union
 
-import gym
+import gymnasium as gym
 import numpy as np
 import torch
-from gym import Wrapper, spaces
-from gym.core import ActType, ObsType
+from gymnasium import Wrapper, spaces
+from gymnasium.core import ActType, ObsType
 from torch import Tensor
 
 from sample_factory.algo.utils.tensor_utils import dict_of_lists_cat
 from sample_factory.envs.create_env import create_env
 from sample_factory.envs.env_utils import (
     RewardShapingInterface,
     TrainingInfoInterface,
@@ -41,36 +41,36 @@
 
 
 def is_multiagent_env(env: Any) -> bool:
     is_multiagent, num_agents = get_multiagent_info(env)
     return is_multiagent
 
 
-class _DictObservationsWrapper(Wrapper[ObsType, ActType]):
+class _DictObservationsWrapper(Wrapper):
     def __init__(self, env):
         super().__init__(env)
         is_multiagent, num_agents = get_multiagent_info(env)
         self.is_multiagent: bool = is_multiagent
         self.num_agents: int = num_agents
         self.observation_space: gym.spaces.Dict = gym.spaces.Dict(dict(obs=self.observation_space))
 
 
-class BatchedDictObservationsWrapper(_DictObservationsWrapper[DictObservations, Actions]):
+class BatchedDictObservationsWrapper(_DictObservationsWrapper):
     """Guarantees that the environment returns observations as dictionaries of lists (batches)."""
 
     def reset(self, **kwargs):
         obs, info = self.env.reset(**kwargs)
         return dict(obs=obs), info
 
     def step(self, action):
         obs, rew, terminated, truncated, info = self.env.step(action)
         return dict(obs=obs), rew, terminated, truncated, info
 
 
-class BatchedMultiAgentWrapper(Wrapper[DictOfListsObservations, Actions]):
+class BatchedMultiAgentWrapper(Wrapper):
     """Assumes wrapped environment has dictionary obs space."""
 
     def __init__(self, env):
         super().__init__(env)
         self.num_agents: int = 1
         self.is_multiagent: bool = True
         assert isinstance(env.observation_space, spaces.Dict), "Wrapped environment must have dictionary obs space."
@@ -90,15 +90,15 @@
         action = action[0]
         obs, rew, terminated, truncated, info = self.env.step(action)
         if terminated | truncated:  # auto-resetting
             obs, info["reset_info"] = self.env.reset()
         return self._obs(obs), [rew], [terminated], [truncated], [info]
 
 
-class NonBatchedMultiAgentWrapper(Wrapper[ListObservations, ListActions]):
+class NonBatchedMultiAgentWrapper(Wrapper):
     """
     This wrapper allows us to treat a single-agent environment as multi-agent with 1 agent.
     That is, the data (obs, rewards, etc.) is converted into lists of length 1
     """
 
     def __init__(self, env):
         super().__init__(env)
@@ -114,41 +114,41 @@
         action = action[0]
         obs, rew, terminated, truncated, info = self.env.step(action)
         if terminated or truncated:  # auto-resetting
             obs, info["reset_info"] = self.env.reset()
         return [obs], [rew], [terminated], [truncated], [info]
 
 
-class NonBatchedDictObservationsWrapper(_DictObservationsWrapper[ListOfDictObservations, ListActions]):
+class NonBatchedDictObservationsWrapper(_DictObservationsWrapper):
     """Guarantees that the environment returns observations as lists of dictionaries."""
 
     def reset(self, **kwargs) -> ListOfDictObservations:
         obs, info = self.env.reset(**kwargs)
         return [dict(obs=o) for o in obs], info
 
     def step(self, action: ListActions) -> Tuple[ListOfDictObservations, Any, Any, Any, Any]:
         obs, rew, terminated, truncated, info = self.env.step(action)
         return [dict(obs=o) for o in obs], rew, terminated, truncated, info
 
 
-class BatchedListToDictWrapper(Wrapper[DictOfListsObservations, Actions]):
+class BatchedListToDictWrapper(Wrapper):
     def reset(self, **kwargs):
         obs, info = self.env.reset(**kwargs)
         if isinstance(obs, list):
             return list_of_dicts_to_dict_of_lists(obs), info
         return obs, info
 
     def step(self, action):
         obs, rew, terminated, truncated, info = self.env.step(action)
         if isinstance(obs, list):
             return list_of_dicts_to_dict_of_lists(obs), rew, terminated, truncated, info
         return obs, rew, terminated, truncated, info
 
 
-class BatchedVecEnv(Wrapper[DictOfTensorObservations, TensorActions]):
+class BatchedVecEnv(Wrapper):
     """Ensures that the env returns a dictionary of tensors for observations, and tensors for rewards and dones."""
 
     ConvertFunc = Callable[[Any], Tensor]
 
     def __init__(self, env):
         if not isinstance(env.observation_space, spaces.Dict):
             env = BatchedDictObservationsWrapper(env)
@@ -307,14 +307,17 @@
 
             ofs += self.single_env_agents
             next_ofs += self.single_env_agents
 
         return self.obs, self.rew, self.terminated, self.truncated, infos
 
     def set_training_info(self, training_info: Dict) -> None:
+        if self.training_info_interfaces is None:
+            return
+
         for env_train_info in self.training_info_interfaces:
             env_train_info.set_training_info(training_info)
 
     def get_default_reward_shaping(self) -> Optional[Dict[str, Any]]:
         if self.reward_shaping_interfaces is not None:
             return self.reward_shaping_interfaces[0].get_default_reward_shaping()
         else:
@@ -344,15 +347,15 @@
     # Now we just want the environment to return a tensor dict for observations and tensors for rewards and dones.
     # We leave infos intact for now, because format of infos isn't really specified and can be inconsistent between
     # timesteps.
     env = BatchedVecEnv(env)
     return env
 
 
-class NonBatchedVecEnv(Wrapper[ListObservations, ListActions]):
+class NonBatchedVecEnv(Wrapper):
     """
     reset() returns a list of dict observations.
     step(action) returns a list of dict observations, list of rewards, list of dones, list of infos.
     """
 
     def __init__(self, env):
         if not is_multiagent_env(env):
```

### Comparing `sample-factory-2.0.3/sample_factory/algo/utils/misc.py` & `sample-factory-2.1.1/sample_factory/algo/utils/misc.py`

 * *Files identical despite different names*

### Comparing `sample-factory-2.0.3/sample_factory/algo/utils/model_sharing.py` & `sample-factory-2.1.1/sample_factory/algo/utils/model_sharing.py`

 * *Files identical despite different names*

### Comparing `sample-factory-2.0.3/sample_factory/algo/utils/multiprocessing_utils.py` & `sample-factory-2.1.1/sample_factory/algo/utils/multiprocessing_utils.py`

 * *Files identical despite different names*

### Comparing `sample-factory-2.0.3/sample_factory/algo/utils/optimizers.py` & `sample-factory-2.1.1/sample_factory/algo/utils/optimizers.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """
 Courtesy of https://github.com/shacklettbp/bps-nav
 See section 3.4 in https://arxiv.org/pdf/2103.07013.pdf
 
 """
 
 import math
+from typing import Callable, Optional, Tuple
 
 import torch
 from torch.optim import Optimizer
 
 
 class Lamb(Optimizer):
     def __init__(
```

### Comparing `sample-factory-2.0.3/sample_factory/algo/utils/rl_utils.py` & `sample-factory-2.1.1/sample_factory/algo/utils/rl_utils.py`

 * *Files identical despite different names*

### Comparing `sample-factory-2.0.3/sample_factory/algo/utils/running_mean_std.py` & `sample-factory-2.1.1/sample_factory/algo/utils/running_mean_std.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 PyTorch module that keeps track of tensor statistics and uses it to normalize data.
 All credit goes to https://github.com/Denys88/rl_games (only slightly changed here, mostly with in-place operations)
 Thanks a lot, great module!
 """
 from typing import Dict, Final, List, Optional, Union
 
-import gym
+import gymnasium as gym
 import torch
 import torch.nn as nn
 from torch import Tensor
 from torch.jit import RecursiveScriptModule, ScriptModule
 
 from sample_factory.utils.utils import log
```

### Comparing `sample-factory-2.0.3/sample_factory/algo/utils/shared_buffers.py` & `sample-factory-2.1.1/sample_factory/algo/utils/shared_buffers.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 
 import math
 from typing import Dict, List, Tuple
 
 import torch
-from gym import spaces
+from gymnasium import spaces
 from signal_slot.queue_utils import get_queue
 from torch import Tensor
 
 from sample_factory.algo.sampling.sampling_utils import rollout_worker_device
 from sample_factory.algo.utils.action_distributions import calc_num_action_parameters, calc_num_actions
 from sample_factory.algo.utils.env_info import EnvInfo
 from sample_factory.algo.utils.misc import MAGIC_FLOAT, MAGIC_INT
```

### Comparing `sample-factory-2.0.3/sample_factory/algo/utils/tensor_dict.py` & `sample-factory-2.1.1/sample_factory/algo/utils/tensor_dict.py`

 * *Files identical despite different names*

### Comparing `sample-factory-2.0.3/sample_factory/algo/utils/tensor_utils.py` & `sample-factory-2.1.1/sample_factory/algo/utils/tensor_utils.py`

 * *Files identical despite different names*

### Comparing `sample-factory-2.0.3/sample_factory/algo/utils/torch_utils.py` & `sample-factory-2.1.1/sample_factory/algo/utils/torch_utils.py`

 * *Files identical despite different names*

### Comparing `sample-factory-2.0.3/sample_factory/cfg/arguments.py` & `sample-factory-2.1.1/sample_factory/cfg/arguments.py`

 * *Files identical despite different names*

### Comparing `sample-factory-2.0.3/sample_factory/cfg/cfg.py` & `sample-factory-2.1.1/sample_factory/cfg/cfg.py`

 * *Files identical despite different names*

### Comparing `sample-factory-2.0.3/sample_factory/enjoy.py` & `sample-factory-2.1.1/sample_factory/enjoy.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import time
 from collections import deque
 from typing import Dict, Tuple
 
-import gym
+import gymnasium as gym
 import numpy as np
 import torch
 from torch import Tensor
 
 from sample_factory.algo.learning.learner import Learner
 from sample_factory.algo.sampling.batched_sampling import preprocess_actions
 from sample_factory.algo.utils.action_distributions import argmax_actions
```

### Comparing `sample-factory-2.0.3/sample_factory/envs/create_env.py` & `sample-factory-2.1.1/sample_factory/envs/create_env.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from __future__ import annotations
 
 from typing import Optional
 
 from sample_factory.algo.utils.context import global_env_registry
+from sample_factory.algo.utils.gymnasium_utils import patch_non_gymnasium_env
 from sample_factory.utils.attr_dict import AttrDict
 from sample_factory.utils.typing import Config
 from sample_factory.utils.utils import log
 
 
 def create_env(
     full_env_name: str,
@@ -31,8 +32,11 @@
         msg = f"Env name {full_env_name} is not registered. See register_env()!"
         log.error(msg)
         log.debug(f"Registered env names: {env_registry.keys()}")
         raise ValueError(msg)
 
     env_factory = env_registry[full_env_name]
     env = env_factory(full_env_name, cfg, env_config, render_mode)
+
+    env = patch_non_gymnasium_env(env)
+
     return env
```

### Comparing `sample-factory-2.0.3/sample_factory/envs/env_utils.py` & `sample-factory-2.1.1/sample_factory/envs/env_utils.py`

 * *Files identical despite different names*

### Comparing `sample-factory-2.0.3/sample_factory/envs/env_wrappers.py` & `sample-factory-2.1.1/sample_factory/envs/env_wrappers.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,19 +4,17 @@
 """
 import json
 import os
 from os.path import join
 from typing import Any, Dict, Tuple, Union
 
 import cv2
-import gym
+import gymnasium as gym
 import numpy as np
-
-# noinspection PyProtectedMember
-from gym import ObservationWrapper, RewardWrapper, spaces
+from gymnasium import ObservationWrapper, RewardWrapper, spaces
 
 from sample_factory.envs.env_utils import num_env_steps
 from sample_factory.utils.utils import ensure_dir_exists, log
 
 
 def has_image_observations(observation_space):
     """It's a heuristic."""
```

### Comparing `sample-factory-2.0.3/sample_factory/huggingface/huggingface_utils.py` & `sample-factory-2.1.1/sample_factory/huggingface/huggingface_utils.py`

 * *Files identical despite different names*

### Comparing `sample-factory-2.0.3/sample_factory/huggingface/load_from_hub.py` & `sample-factory-2.1.1/sample_factory/huggingface/load_from_hub.py`

 * *Files identical despite different names*

### Comparing `sample-factory-2.0.3/sample_factory/huggingface/push_to_hub.py` & `sample-factory-2.1.1/sample_factory/huggingface/push_to_hub.py`

 * *Files identical despite different names*

### Comparing `sample-factory-2.0.3/sample_factory/launcher/run.py` & `sample-factory-2.1.1/sample_factory/launcher/run.py`

 * *Files identical despite different names*

### Comparing `sample-factory-2.0.3/sample_factory/launcher/run_description.py` & `sample-factory-2.1.1/sample_factory/launcher/run_description.py`

 * *Files identical despite different names*

### Comparing `sample-factory-2.0.3/sample_factory/launcher/run_ngc.py` & `sample-factory-2.1.1/sample_factory/launcher/run_ngc.py`

 * *Files identical despite different names*

### Comparing `sample-factory-2.0.3/sample_factory/launcher/run_processes.py` & `sample-factory-2.1.1/sample_factory/launcher/run_processes.py`

 * *Files identical despite different names*

### Comparing `sample-factory-2.0.3/sample_factory/launcher/run_slurm.py` & `sample-factory-2.1.1/sample_factory/launcher/run_slurm.py`

 * *Files identical despite different names*

### Comparing `sample-factory-2.0.3/sample_factory/model/action_parameterization.py` & `sample-factory-2.1.1/sample_factory/model/action_parameterization.py`

 * *Files identical despite different names*

### Comparing `sample-factory-2.0.3/sample_factory/model/actor_critic.py` & `sample-factory-2.1.1/sample_factory/model/actor_critic.py`

 * *Files identical despite different names*

### Comparing `sample-factory-2.0.3/sample_factory/model/core.py` & `sample-factory-2.1.1/sample_factory/model/core.py`

 * *Files identical despite different names*

### Comparing `sample-factory-2.0.3/sample_factory/model/decoder.py` & `sample-factory-2.1.1/sample_factory/model/decoder.py`

 * *Files identical despite different names*

### Comparing `sample-factory-2.0.3/sample_factory/model/encoder.py` & `sample-factory-2.1.1/sample_factory/model/encoder.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import Dict, List, Optional
 
 import torch
-from gym import spaces
+from gymnasium import spaces
 from torch import Tensor, nn
 
 from sample_factory.algo.utils.torch_utils import calc_num_elements
 from sample_factory.model.model_utils import ModelModule, create_mlp, model_device, nonlinearity
 from sample_factory.utils.attr_dict import AttrDict
 from sample_factory.utils.typing import Config, ObsSpace
 from sample_factory.utils.utils import log
```

### Comparing `sample-factory-2.0.3/sample_factory/model/model_factory.py` & `sample-factory-2.1.1/sample_factory/model/model_factory.py`

 * *Files identical despite different names*

### Comparing `sample-factory-2.0.3/sample_factory/model/model_utils.py` & `sample-factory-2.1.1/sample_factory/model/model_utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 from typing import List, Optional
 
 import torch
 from torch import nn
 from torch.nn.utils import spectral_norm
 
 from sample_factory.cfg.configurable import Configurable
-from sample_factory.utils.attr_dict import AttrDict
-from sample_factory.utils.typing import Config, ObsSpace
+from sample_factory.utils.typing import Config
 
 
 def get_rnn_size(cfg):
     if cfg.use_rnn:
         size = cfg.rnn_size * cfg.rnn_num_layers
     else:
         size = 1
@@ -21,23 +20,23 @@
     if not cfg.actor_critic_share_weights:
         # actor and critic need separate states
         size *= 2
 
     return size
 
 
-def nonlinearity(cfg: Config) -> nn.Module:
+def nonlinearity(cfg: Config, inplace: bool = False) -> nn.Module:
     if cfg.nonlinearity == "elu":
-        return nn.ELU(inplace=True)
+        return nn.ELU(inplace=inplace)
     elif cfg.nonlinearity == "relu":
-        return nn.ReLU(inplace=True)
+        return nn.ReLU(inplace=inplace)
     elif cfg.nonlinearity == "tanh":
         return nn.Tanh()
     else:
-        raise Exception("Unknown nonlinearity")
+        raise Exception(f"Unknown {cfg.nonlinearity=}")
 
 
 def fc_layer(in_features: int, out_features: int, bias=True, spec_norm=False) -> nn.Module:
     layer = nn.Linear(in_features, out_features, bias)
     if spec_norm:
         layer = spectral_norm(layer)
```

### Comparing `sample-factory-2.0.3/sample_factory/pbt/population_based_training.py` & `sample-factory-2.1.1/sample_factory/pbt/population_based_training.py`

 * *Files identical despite different names*

### Comparing `sample-factory-2.0.3/sample_factory/train.py` & `sample-factory-2.1.1/sample_factory/train.py`

 * *Files identical despite different names*

### Comparing `sample-factory-2.0.3/sample_factory/utils/decay.py` & `sample-factory-2.1.1/sample_factory/utils/decay.py`

 * *Files identical despite different names*

### Comparing `sample-factory-2.0.3/sample_factory/utils/dicts.py` & `sample-factory-2.1.1/sample_factory/utils/dicts.py`

 * *Files identical despite different names*

### Comparing `sample-factory-2.0.3/sample_factory/utils/get_available_gpus.py` & `sample-factory-2.1.1/sample_factory/utils/get_available_gpus.py`

 * *Files identical despite different names*

### Comparing `sample-factory-2.0.3/sample_factory/utils/gifs.py` & `sample-factory-2.1.1/sample_factory/utils/gifs.py`

 * *Files identical despite different names*

### Comparing `sample-factory-2.0.3/sample_factory/utils/gpu_utils.py` & `sample-factory-2.1.1/sample_factory/utils/gpu_utils.py`

 * *Files identical despite different names*

### Comparing `sample-factory-2.0.3/sample_factory/utils/normalize.py` & `sample-factory-2.1.1/sample_factory/utils/normalize.py`

 * *Files identical despite different names*

### Comparing `sample-factory-2.0.3/sample_factory/utils/tb.py` & `sample-factory-2.1.1/sample_factory/utils/tb.py`

 * *Files identical despite different names*

### Comparing `sample-factory-2.0.3/sample_factory/utils/timing.py` & `sample-factory-2.1.1/sample_factory/utils/timing.py`

 * *Files identical despite different names*

### Comparing `sample-factory-2.0.3/sample_factory/utils/typing.py` & `sample-factory-2.1.1/sample_factory/utils/typing.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 
 import argparse
 from typing import Any, Callable, Dict, Optional, Tuple, Union
 
 import torch
-from gym import spaces
+from gymnasium import spaces
 
 from sample_factory.utils.attr_dict import AttrDict
 
 Config = Union[argparse.Namespace, AttrDict]
 
 StatusCode = int
```

### Comparing `sample-factory-2.0.3/sample_factory/utils/utils.py` & `sample-factory-2.1.1/sample_factory/utils/utils.py`

 * *Files identical despite different names*

### Comparing `sample-factory-2.0.3/sample_factory/utils/wandb_utils.py` & `sample-factory-2.1.1/sample_factory/utils/wandb_utils.py`

 * *Files identical despite different names*

### Comparing `sample-factory-2.0.3/sample_factory.egg-info/PKG-INFO` & `sample-factory-2.1.1/sample_factory.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sample-factory
-Version: 2.0.3
+Version: 2.1.1
 Summary: High throughput asynchronous reinforcement learning framework
 Home-page: https://github.com/alex-petrenko/sample-factory
 Author: Aleksei Petrenko
 License: MIT
 Project-URL: Github, https://github.com/alex-petrenko/sample-factory
 Project-URL: Videos, https://sites.google.com/view/sample-factory
 Keywords: asynchronous reinforcement learning policy gradient ppo appo impala ai
```

### Comparing `sample-factory-2.0.3/sample_factory.egg-info/SOURCES.txt` & `sample-factory-2.1.1/sample_factory.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 ./docs/03-customization/custom-multi-agent-environments.md
 ./docs/04-experiments/experiment-launcher.md
 ./docs/04-experiments/slurm-details.md
 ./docs/05-monitoring/custom-metrics.md
 ./docs/05-monitoring/metrics-reference.md
 ./docs/05-monitoring/tensorboard.md
 ./docs/05-monitoring/wandb.md
+./docs/05-troubleshooting/troubleshooting.md
 ./docs/06-architecture/message-passing.md
 ./docs/06-architecture/overview.md
 ./docs/07-advanced-topics/batched-non-batched.md
 ./docs/07-advanced-topics/double-buffered.md
 ./docs/07-advanced-topics/inactive-agents.md
 ./docs/07-advanced-topics/multi-policy-training.md
 ./docs/07-advanced-topics/normalizations.md
@@ -56,14 +57,16 @@
 ./sample_factory/train.py
 ./sample_factory.egg-info/PKG-INFO
 ./sample_factory.egg-info/SOURCES.txt
 ./sample_factory.egg-info/dependency_links.txt
 ./sample_factory.egg-info/requires.txt
 ./sample_factory.egg-info/top_level.txt
 ./sample_factory/algo/__init__.py
+./sample_factory/algo/evaluators/__init__.py
+./sample_factory/algo/evaluators/default_evaluator.py
 ./sample_factory/algo/learning/__init__.py
 ./sample_factory/algo/learning/batcher.py
 ./sample_factory/algo/learning/learner.py
 ./sample_factory/algo/learning/learner_worker.py
 ./sample_factory/algo/learning/rnn_utils.py
 ./sample_factory/algo/runners/__init__.py
 ./sample_factory/algo/runners/runner.py
@@ -78,14 +81,15 @@
 ./sample_factory/algo/sampling/sampling_utils.py
 ./sample_factory/algo/sampling/simplified_sampling_api.py
 ./sample_factory/algo/utils/__init__.py
 ./sample_factory/algo/utils/action_distributions.py
 ./sample_factory/algo/utils/agent_policy_mapping.py
 ./sample_factory/algo/utils/context.py
 ./sample_factory/algo/utils/env_info.py
+./sample_factory/algo/utils/gymnasium_utils.py
 ./sample_factory/algo/utils/heartbeat.py
 ./sample_factory/algo/utils/make_env.py
 ./sample_factory/algo/utils/misc.py
 ./sample_factory/algo/utils/model_sharing.py
 ./sample_factory/algo/utils/multiprocessing_utils.py
 ./sample_factory/algo/utils/optimizers.py
 ./sample_factory/algo/utils/rl_utils.py
@@ -276,13 +280,10 @@
 ./sf_examples/vizdoom/doom/wrappers/exploration.py
 ./sf_examples/vizdoom/doom/wrappers/multiplayer_stats.py
 ./sf_examples/vizdoom/doom/wrappers/observation_space.py
 ./sf_examples/vizdoom/doom/wrappers/reward_shaping.py
 ./sf_examples/vizdoom/doom/wrappers/step_human_input.py
 ./sf_examples/vizdoom/doom/wrappers/scenario_wrappers/__init__.py
 ./sf_examples/vizdoom/doom/wrappers/scenario_wrappers/gathering_reward_shaping.py
-./train_dir/isaacgym_allegrohand/README.md
-./train_dir/isaacgym_ant/README.md
-./train_dir/isaacgym_humanoid/README.md
 tests/test_launcher.py
 tests/test_precheck.py
 tests/test_utils.py
```

### Comparing `sample-factory-2.0.3/setup.py` & `sample-factory-2.1.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,16 +8,16 @@
     for dl in descr_lines:
         if not ("<img src=" in dl and "gif" in dl):
             descr_no_gifs.append(dl)
 
     long_description = "\n".join(descr_no_gifs)
 
 
-_atari_deps = ["gym[atari, accept-rom-license]"]
-_mujoco_deps = ["gym[mujoco]"]
+_atari_deps = ["gymnasium[atari, accept-rom-license]"]
+_mujoco_deps = ["gymnasium[mujoco]", "mujoco<=2.3.3"]
 _envpool_deps = ["envpool"]
 
 _docs_deps = [
     "mkdocs-material",
     "mkdocs-minify-plugin",
     "mkdocs-redirects",
     "mkdocs-git-revision-date-localized-plugin",
@@ -27,50 +27,50 @@
 
 setup(
     # Information
     name="sample-factory",
     description="High throughput asynchronous reinforcement learning framework",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    version="2.0.3",
+    version="2.1.1",
     url="https://github.com/alex-petrenko/sample-factory",
     author="Aleksei Petrenko",
     license="MIT",
     keywords="asynchronous reinforcement learning policy gradient ppo appo impala ai",
     project_urls={
         "Github": "https://github.com/alex-petrenko/sample-factory",
         "Videos": "https://sites.google.com/view/sample-factory",
     },
     install_requires=[
         "numpy>=1.18.1,<2.0",
-        "torch>=1.9,<2.0,!=1.13.0",
-        "gym>=0.26.1,<1.0",
+        "torch>=1.9,<3.0,!=1.13.0",
+        "gymnasium>=0.27,<1.0",
         "pyglet",  # gym dependency
         "tensorboard>=1.15.0",
         "tensorboardx>=2.0",
         "psutil>=5.7.0",
         "threadpoolctl>=2.0.0",
         "colorlog",
-        "faster-fifo>=1.4.2,<2.0",
+        # "faster-fifo>=1.4.2,<2.0",  <-- installed by signal-slot-mp
         "signal-slot-mp>=1.0.3,<2.0",
         "filelock",
-        "opencv-python!=3.4.18.65",
+        "opencv-python",
         "wandb>=0.12.9",
         "huggingface-hub>=0.10.0,<1.0",
     ],
     extras_require={
         # some tests require Atari and Mujoco so let's make sure dev environment has that
         "dev": ["black", "isort>=5.12", "pytest<8.0", "flake8", "pre-commit", "twine"]
         + _docs_deps
         + _atari_deps
         + _mujoco_deps,
         "atari": _atari_deps,
         "envpool": _envpool_deps,
         "mujoco": _mujoco_deps,
-        "vizdoom": ["vizdoom<2.0", "gym[classic_control]"],
+        "vizdoom": ["vizdoom<2.0", "gymnasium[classic_control]"],
         # "dmlab": ["dm_env"],  <-- these are just auxiliary packages, the main package has to be built from sources
     },
     package_dir={"": "./"},
     packages=setuptools.find_packages(where="./", include=["sample_factory*", "sf_examples*"]),
     include_package_data=True,
     python_requires=">=3.8",
 )
```

### Comparing `sample-factory-2.0.3/sf_examples/atari/atari_params.py` & `sample-factory-2.1.1/sf_examples/atari/atari_params.py`

 * *Files identical despite different names*

### Comparing `sample-factory-2.0.3/sf_examples/atari/atari_utils.py` & `sample-factory-2.1.1/sf_examples/atari/atari_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Optional
 
-import gym
+import gymnasium as gym
 
 from sample_factory.envs.env_wrappers import (
     ClipRewardEnv,
     EpisodicLifeEnv,
     FireResetEnv,
     MaxAndSkipEnv,
     NoopResetEnv,
```

### Comparing `sample-factory-2.0.3/sf_examples/atari/experiments/atari_envs.py` & `sample-factory-2.1.1/sf_examples/atari/experiments/atari_envs.py`

 * *Files identical despite different names*

### Comparing `sample-factory-2.0.3/sf_examples/atari/train_atari.py` & `sample-factory-2.1.1/sf_examples/atari/train_atari.py`

 * *Files 15% similar despite different names*

```diff
@@ -19,17 +19,17 @@
 def parse_atari_args(argv=None, evaluation=False):
     parser, partial_cfg = parse_sf_args(argv=argv, evaluation=evaluation)
     atari_override_defaults(partial_cfg.env, parser)
     final_cfg = parse_full_cfg(parser, argv)
     return final_cfg
 
 
-def main():
+def main():  # pragma: no cover
     """Script entry point."""
     register_atari_components()
     cfg = parse_atari_args()
     status = run_rl(cfg)
     return status
 
 
-if __name__ == "__main__":
+if __name__ == "__main__":  # pragma: no cover
     sys.exit(main())
```

### Comparing `sample-factory-2.0.3/sf_examples/brax/brax_render.py` & `sample-factory-2.1.1/sf_examples/brax/brax_render.py`

 * *Files identical despite different names*

### Comparing `sample-factory-2.0.3/sf_examples/brax/experiments/brax_basic_envs.py` & `sample-factory-2.1.1/sf_examples/brax/experiments/brax_basic_envs.py`

 * *Files identical despite different names*

### Comparing `sample-factory-2.0.3/sf_examples/brax/train_brax.py` & `sample-factory-2.1.1/sf_examples/brax/train_brax.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 """
 Brax env integration.
 """
 import sys
 from typing import Dict, List, Optional, Tuple, Union
 
-import gym
+import gymnasium as gym
 import numpy as np
 import torch
 import torch.utils.dlpack as tpack
-from gym.core import RenderFrame
+from gymnasium.core import RenderFrame
 from torch import Tensor
 
+from sample_factory.algo.utils.gymnasium_utils import convert_space
 from sample_factory.cfg.arguments import parse_full_cfg, parse_sf_args
 from sample_factory.envs.env_utils import register_env
 from sample_factory.train import run_rl
 from sample_factory.utils.typing import Config, Env
 from sample_factory.utils.utils import log, str2bool
 
 BRAX_EVALUATION = False
@@ -68,16 +69,16 @@
 
             obs_high = np.inf * np.ones(observation_size)
             self.observation_space = gym.spaces.Box(-obs_high, obs_high, dtype=np.float32)
 
             action_high = np.ones(action_size)
             self.action_space = gym.spaces.Box(-action_high, action_high, dtype=np.float32)
         else:
-            self.observation_space = self.env.observation_space
-            self.action_space = self.env.action_space
+            self.observation_space = convert_space(self.env.observation_space)
+            self.action_space = convert_space(self.env.action_space)
 
     def reset(self, *args, **kwargs) -> Tuple[Tensor, Dict]:
         log.debug(f"Resetting env {self.env} with {self.num_agents} parallel agents...")
         obs = self.env.reset()
         obs = jax_to_torch(obs)
         log.debug(f"reset() done, obs.shape={obs.shape}!")
         return obs, {}
```

### Comparing `sample-factory-2.0.3/sf_examples/dmlab/command_line/train_dmlab30_server_pbt.sh` & `sample-factory-2.1.1/sf_examples/dmlab/command_line/train_dmlab30_server_pbt.sh`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 #!/bin/bash
 python -m sf.algorithms.appo.train_appo \
 --env=dmlab_30 --train_for_seconds=3600000 --algo=APPO --gamma=0.99 --use_rnn=True --num_workers=72 --num_envs_per_worker=12 --ppo_epochs=1 --rollout=32 --recurrence=32 --macro_batch=2048 --batch_size=2048 --benchmark=False --ppo_epochs=1 \
 --max_grad_norm=0.0 \
 --dmlab_renderer=software \
 --decorrelate_experience_max_seconds=60 \
---reset_timeout_seconds=300 \
 --encoder_custom=dmlab_instructions --encoder_type=resnet --encoder_subtype=resnet_impala --encoder_extra_fc_layers=1 --hidden_size=256 --nonlinearity=relu --rnn_type=lstm \
 --dmlab_extended_action_set=True \
 --num_policies=4 --pbt_replace_reward_gap=0.1 --pbt_replace_reward_gap_absolute=5.0 --pbt_period_env_steps=10000000 --pbt_start_mutation=100000000 --with_pbt=True \
 --experiment=dmlab_30_resnet_4pbt_v84
```

### Comparing `sample-factory-2.0.3/sf_examples/dmlab/dmlab30.py` & `sample-factory-2.1.1/sf_examples/dmlab/dmlab30.py`

 * *Files identical despite different names*

### Comparing `sample-factory-2.0.3/sf_examples/dmlab/dmlab_env.py` & `sample-factory-2.1.1/sf_examples/dmlab/dmlab_env.py`

 * *Files identical despite different names*

### Comparing `sample-factory-2.0.3/sf_examples/dmlab/dmlab_gym.py` & `sample-factory-2.1.1/sf_examples/dmlab/dmlab_gym.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import shutil
 import time
 from os.path import join
 from typing import Dict, Optional
 
 import cv2
 import deepmind_lab
-import gym
+import gymnasium as gym
 import numpy as np
 
 from sample_factory.utils.typing import PolicyID
 from sample_factory.utils.utils import ensure_dir_exists, log
 from sf_examples.dmlab.dmlab30 import DMLAB_INSTRUCTIONS, DMLAB_MAX_INSTRUCTION_LEN, DMLAB_VOCABULARY_SIZE
 from sf_examples.dmlab.dmlab_level_cache import DmlabLevelCache
 from sf_examples.dmlab.dmlab_utils import string_to_hash_bucket
@@ -189,15 +189,15 @@
     def reset(self, **kwargs):
         if self.use_level_cache:
             self.curr_cache = self.dmlab_level_caches_per_policy[self.curr_policy_idx]
             self.last_reset_seed = self.curr_cache.get_unused_seed(self.level, self.random_state)
         else:
             self.last_reset_seed = self.random_state.randint(0, 2**31 - 1)
 
-        self.dmlab.reset()
+        self.dmlab.reset(seed=self.last_reset_seed)
         self.last_observation = self.format_obs_dict(self.dmlab.observations())
         return self.last_observation, {}
 
     def step(self, action):
         if self.benchmark_mode:
             # the performance of many DMLab environments heavily depends on what agent is actually doing
             # therefore for purposes of measuring throughput we ignore the actions, this way the agent executes
```

### Comparing `sample-factory-2.0.3/sf_examples/dmlab/dmlab_level_cache.py` & `sample-factory-2.1.1/sf_examples/dmlab/dmlab_level_cache.py`

 * *Files identical despite different names*

### Comparing `sample-factory-2.0.3/sf_examples/dmlab/dmlab_model.py` & `sample-factory-2.1.1/sf_examples/dmlab/dmlab_model.py`

 * *Files identical despite different names*

### Comparing `sample-factory-2.0.3/sf_examples/dmlab/dmlab_params.py` & `sample-factory-2.1.1/sf_examples/dmlab/dmlab_params.py`

 * *Files identical despite different names*

### Comparing `sample-factory-2.0.3/sf_examples/dmlab/dmlab_populate_cache.py` & `sample-factory-2.1.1/sf_examples/dmlab/dmlab_populate_cache.py`

 * *Files identical despite different names*

### Comparing `sample-factory-2.0.3/sf_examples/dmlab/experiments/dmlab30.py` & `sample-factory-2.1.1/sf_examples/dmlab/experiments/dmlab30.py`

 * *Files identical despite different names*

### Comparing `sample-factory-2.0.3/sf_examples/dmlab/train_dmlab.py` & `sample-factory-2.1.1/sf_examples/dmlab/train_dmlab.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 
 def register_dmlab_components(level_caches: Optional[DmlabLevelCaches] = None):
     register_dmlab_envs(level_caches)
     global_model_factory().register_encoder_factory(make_dmlab_encoder)
 
 
 class DmlabExtraSummariesObserver(AlgoObserver):
-    def extra_summaries(self, runner: Runner, policy_id: PolicyID, env_steps: int, writer: SummaryWriter) -> None:
+    def extra_summaries(self, runner: Runner, policy_id: PolicyID, writer: SummaryWriter, env_steps: int) -> None:
         dmlab_extra_summaries(runner, policy_id, env_steps, writer)
 
 
 def register_msg_handlers(cfg: Config, runner: Runner):
     if cfg.env == "dmlab_30":
         # extra functions to calculate human-normalized score etc.
         runner.register_episodic_stats_handler(dmlab_extra_episodic_stats_processing)
```

### Comparing `sample-factory-2.0.3/sf_examples/dmlab/wrappers/reward_shaping.py` & `sample-factory-2.1.1/sf_examples/dmlab/wrappers/reward_shaping.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from math import tanh
 
-import gym
+import gymnasium as gym
 
 RAW_SCORE_SUMMARY_KEY_SUFFIX = "dmlab_raw_score"
 
 
 class DmlabRewardShapingWrapper(gym.Wrapper):
     def __init__(self, env):
         super().__init__(env)
```

### Comparing `sample-factory-2.0.3/sf_examples/envpool/atari/envpool_atari_params.py` & `sample-factory-2.1.1/sf_examples/envpool/atari/envpool_atari_params.py`

 * *Files identical despite different names*

### Comparing `sample-factory-2.0.3/sf_examples/envpool/atari/envpool_atari_utils.py` & `sample-factory-2.1.1/sf_examples/envpool/atari/envpool_atari_utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 from typing import Optional
 
+from sample_factory.utils.utils import log
+
 try:
     import envpool
 except ImportError as e:
     print(e)
     print("Trying to import envpool when it is not installed. install with 'pip install envpool'")
 
 from sf_examples.atari.atari_utils import ATARI_ENVS, AtariSpec
@@ -24,15 +26,20 @@
     for cfg in ENVPOOL_ATARI_ENVS:
         if cfg.name == name:
             return cfg
     raise Exception("Unknown Atari env")
 
 
 def make_atari_env(env_name, cfg, env_config, render_mode: Optional[str] = None):
-    assert cfg.num_envs_per_worker == 1, "when using envpool, set num_envs_per_worker=1 and use --env_agents="
+    if cfg.num_envs_per_worker > 1:
+        log.warning(
+            "When using envpool, set num_envs_per_worker=1 and use --env_agents={desired number of envs}. "
+            f"Setting --num_envs_per_worker={cfg.num_envs_per_worker} will create multiple envpools per worker process "
+            f"which is not the desirable behavior in most configurations."
+        )
     atari_spec = atari_env_by_name(env_name)
 
     env_kwargs = dict()
 
     if atari_spec.default_timeout is not None:
         # envpool max_episode_steps does not take into account frameskip. see https://github.com/sail-sg/envpool/issues/195
         env_kwargs["max_episode_steps"] = atari_spec.default_timeout // 4
@@ -44,11 +51,13 @@
         env_type="gym",
         num_envs=cfg.env_agents,
         reward_clip=True,
         episodic_life=True,
         frame_skip=cfg.env_frameskip,
         **env_kwargs,
     )
+
     env = EnvPoolResetFixWrapper(env)
     env = BatchedRecordEpisodeStatistics(env, num_envs=cfg.env_agents)
     env.num_agents = cfg.env_agents
+
     return env
```

### Comparing `sample-factory-2.0.3/sf_examples/envpool/atari/train_envpool_atari.py` & `sample-factory-2.1.1/sf_examples/envpool/atari/train_envpool_atari.py`

 * *Files identical despite different names*

### Comparing `sample-factory-2.0.3/sf_examples/envpool/envpool_utils.py` & `sample-factory-2.1.1/sf_examples/envpool/envpool_utils.py`

 * *Files identical despite different names*

### Comparing `sample-factory-2.0.3/sf_examples/envpool/envpool_wrappers.py` & `sample-factory-2.1.1/sf_examples/envpool/envpool_wrappers.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Tuple, Union
 
-import gym
+import gymnasium as gym
 import numpy as np
-from gym.core import ObsType
+from gymnasium.core import ObsType
 
 DoneStepType = Tuple[
     Union[ObsType, np.ndarray],
     Union[float, np.ndarray],
     Union[bool, np.ndarray],
     Union[dict, list],
 ]
@@ -35,26 +35,27 @@
         needs_reset = np.nonzero(terminated | truncated)[0]
         obs[needs_reset], _ = self.env.reset(needs_reset)
 
         return obs, reward, terminated, truncated, info
 
     def reset(self, **kwargs):
         kwargs.pop("seed", None)  # envpool does not support the seed in reset, even with the updated API
-        return super().reset(**kwargs)
+        kwargs.pop("options", None)
+        return self.env.reset(**kwargs)
 
 
 class BatchedRecordEpisodeStatistics(gym.Wrapper):
     def __init__(self, env, num_envs, deque_size=100):
         super().__init__(env)
         self.num_envs = getattr(env, "num_envs", num_envs)
         self.episode_returns = None
         self.episode_lengths = None
 
     def reset(self, **kwargs):
-        observations, infos = super().reset(**kwargs)
+        observations, infos = self.env.reset(**kwargs)
         self.episode_returns = np.zeros(self.num_envs, dtype=np.float32)
         self.episode_lengths = np.zeros(self.num_envs, dtype=np.int32)
         self.lives = np.zeros(self.num_envs, dtype=np.int32)
         self.returned_episode_returns = np.zeros(self.num_envs, dtype=np.float32)
         self.returned_episode_lengths = np.zeros(self.num_envs, dtype=np.int32)
         return observations, infos
```

### Comparing `sample-factory-2.0.3/sf_examples/envpool/mujoco/envpool_mujoco_params.py` & `sample-factory-2.1.1/sf_examples/envpool/mujoco/envpool_mujoco_params.py`

 * *Files identical despite different names*

### Comparing `sample-factory-2.0.3/sf_examples/envpool/mujoco/envpool_mujoco_utils.py` & `sample-factory-2.1.1/sf_examples/envpool/mujoco/envpool_mujoco_utils.py`

 * *Files identical despite different names*

### Comparing `sample-factory-2.0.3/sf_examples/envpool/mujoco/experiments/mujoco_envpool.py` & `sample-factory-2.1.1/sf_examples/envpool/mujoco/experiments/mujoco_envpool.py`

 * *Files identical despite different names*

### Comparing `sample-factory-2.0.3/sf_examples/envpool/mujoco/train_envpool_mujoco.py` & `sample-factory-2.1.1/sf_examples/envpool/mujoco/train_envpool_mujoco.py`

 * *Files identical despite different names*

### Comparing `sample-factory-2.0.3/sf_examples/isaacgym_examples/enjoy_isaacgym.py` & `sample-factory-2.1.1/sf_examples/isaacgym_examples/enjoy_isaacgym.py`

 * *Files identical despite different names*

### Comparing `sample-factory-2.0.3/sf_examples/isaacgym_examples/experiments/isaacgym_allegrohand.py` & `sample-factory-2.1.1/sf_examples/isaacgym_examples/experiments/isaacgym_allegrohand.py`

 * *Files identical despite different names*

### Comparing `sample-factory-2.0.3/sf_examples/isaacgym_examples/experiments/isaacgym_ant.py` & `sample-factory-2.1.1/sf_examples/isaacgym_examples/experiments/isaacgym_ant.py`

 * *Files identical despite different names*

### Comparing `sample-factory-2.0.3/sf_examples/isaacgym_examples/experiments/isaacgym_basic_envs.py` & `sample-factory-2.1.1/sf_examples/isaacgym_examples/experiments/isaacgym_basic_envs.py`

 * *Files identical despite different names*

### Comparing `sample-factory-2.0.3/sf_examples/isaacgym_examples/experiments/isaacgym_humanoid.py` & `sample-factory-2.1.1/sf_examples/isaacgym_examples/experiments/isaacgym_humanoid.py`

 * *Files identical despite different names*

### Comparing `sample-factory-2.0.3/sf_examples/isaacgym_examples/train_isaacgym.py` & `sample-factory-2.1.1/sf_examples/isaacgym_examples/train_isaacgym.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,40 +6,41 @@
 # isort: on
 
 import os
 import sys
 from os.path import join
 from typing import Dict, List, Optional, Tuple
 
-import gym
+import gymnasium as gym
 import torch
 from isaacgymenvs.tasks import isaacgym_task_map
 from isaacgymenvs.utils.reformat import omegaconf_to_dict
 from torch import Tensor
 
+from sample_factory.algo.utils.gymnasium_utils import convert_space
 from sample_factory.cfg.arguments import parse_full_cfg, parse_sf_args
 from sample_factory.envs.env_utils import register_env
 from sample_factory.train import run_rl
 from sample_factory.utils.typing import Config, Env
 from sample_factory.utils.utils import str2bool
 
 
 class IsaacGymVecEnv(gym.Env):
     def __init__(self, isaacgym_env, obs_key):
         self.env = isaacgym_env
         # what about vectorized multi-agent envs? should we take num_agents into account also?
         self.num_agents = self.env.num_envs
-        self.action_space = self.env.action_space
+        self.action_space = convert_space(self.env.action_space)
 
         # isaacgym_examples environments actually return dicts
         if obs_key == "obs":
-            self.observation_space = gym.spaces.Dict(dict(obs=self.env.observation_space))
+            self.observation_space = gym.spaces.Dict(dict(obs=convert_space(self.env.observation_space)))
             self._proc_obs_func = lambda obs_dict: obs_dict
         elif obs_key == "states":
-            self.observation_space = gym.spaces.Dict(dict(obs=self.env.state_space))
+            self.observation_space = gym.spaces.Dict(dict(obs=convert_space(self.env.state_space)))
             self._proc_obs_func = self._use_states_as_obs
         else:
             raise ValueError(f"Unknown observation key: {obs_key}")
 
         self._truncated: Tensor = torch.zeros(self.num_agents, dtype=torch.bool)
 
     @staticmethod
```

### Comparing `sample-factory-2.0.3/sf_examples/mujoco/README.md` & `sample-factory-2.1.1/sf_examples/mujoco/README.md`

 * *Files identical despite different names*

### Comparing `sample-factory-2.0.3/sf_examples/mujoco/experiments/mujoco_all_envs.py` & `sample-factory-2.1.1/sf_examples/mujoco/experiments/mujoco_all_envs.py`

 * *Files identical despite different names*

### Comparing `sample-factory-2.0.3/sf_examples/mujoco/mujoco_params.py` & `sample-factory-2.1.1/sf_examples/mujoco/mujoco_params.py`

 * *Files identical despite different names*

### Comparing `sample-factory-2.0.3/sf_examples/mujoco/mujoco_utils.py` & `sample-factory-2.1.1/sf_examples/mujoco/mujoco_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Optional
 
-import gym
+import gymnasium as gym
 
 from sample_factory.utils.utils import is_module_available
 
 
 def mujoco_available():
     return is_module_available("mujoco")
```

### Comparing `sample-factory-2.0.3/sf_examples/mujoco/train_mujoco.py` & `sample-factory-2.1.1/sf_examples/mujoco/train_mujoco.py`

 * *Files 22% similar despite different names*

```diff
@@ -16,17 +16,17 @@
     parser, partial_cfg = parse_sf_args(argv=argv, evaluation=evaluation)
     add_mujoco_env_args(partial_cfg.env, parser)
     mujoco_override_defaults(partial_cfg.env, parser)
     final_cfg = parse_full_cfg(parser, argv)
     return final_cfg
 
 
-def main():
+def main():  # pragma: no cover
     """Script entry point."""
     register_mujoco_components()
     cfg = parse_mujoco_cfg()
     status = run_rl(cfg)
     return status
 
 
-if __name__ == "__main__":
+if __name__ == "__main__":  # pragma: no cover
     sys.exit(main())
```

### Comparing `sample-factory-2.0.3/sf_examples/sampler/use_simplified_sampling_api.py` & `sample-factory-2.1.1/sf_examples/sampler/use_simplified_sampling_api.py`

 * *Files identical despite different names*

### Comparing `sample-factory-2.0.3/sf_examples/train_custom_env_custom_model.py` & `sample-factory-2.1.1/sf_examples/train_custom_env_custom_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 """
 from __future__ import annotations
 
 import sys
 from typing import Any, Dict, Optional
 
-import gym
+import gymnasium as gym
 import numpy as np
 from torch import nn
 
 from sample_factory.algo.utils.context import global_model_factory
 from sample_factory.algo.utils.torch_utils import calc_num_elements
 from sample_factory.cfg.arguments import parse_full_cfg, parse_sf_args
 from sample_factory.envs.env_utils import RewardShapingInterface, TrainingInfoInterface, register_env
```

### Comparing `sample-factory-2.0.3/sf_examples/train_custom_multi_env.py` & `sample-factory-2.1.1/sf_examples/train_custom_multi_env.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 """
 from __future__ import annotations
 
 import random
 import sys
 from typing import Any, Dict, Optional
 
-import gym
+import gymnasium as gym
 import numpy as np
 
 from sample_factory.algo.utils.context import global_model_factory
 from sample_factory.cfg.arguments import parse_full_cfg, parse_sf_args
 from sample_factory.envs.env_utils import RewardShapingInterface, TrainingInfoInterface, register_env
 from sample_factory.train import run_rl
 from sf_examples.train_custom_env_custom_model import make_custom_encoder, override_default_params
```

### Comparing `sample-factory-2.0.3/sf_examples/train_gym_env.py` & `sample-factory-2.1.1/sf_examples/train_gym_env.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 python -m sf_examples.enjoy_gym_env --algo=APPO --experiment=example_gym_cartpole-v1 --env=CartPole-v1
 
 """
 
 import sys
 from typing import Optional
 
-import gym
+import gymnasium as gym
 
 from sample_factory.cfg.arguments import parse_full_cfg, parse_sf_args
 from sample_factory.envs.env_utils import register_env
 from sample_factory.train import run_rl
 
 
 def make_gym_env_func(full_env_name, cfg=None, env_config=None, render_mode: Optional[str] = None):
```

### Comparing `sample-factory-2.0.3/sf_examples/vizdoom/custom_env/custom_doom_env.cfg` & `sample-factory-2.1.1/sf_examples/vizdoom/custom_env/custom_doom_env.cfg`

 * *Files identical despite different names*

### Comparing `sample-factory-2.0.3/sf_examples/vizdoom/custom_env/custom_doom_env.wad` & `sample-factory-2.1.1/sf_examples/vizdoom/custom_env/custom_doom_env.wad`

 * *Files identical despite different names*

### Comparing `sample-factory-2.0.3/sf_examples/vizdoom/doom/action_space.py` & `sample-factory-2.1.1/sf_examples/vizdoom/doom/action_space.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-import gym
+import gymnasium as gym
 import numpy as np
-from gym.spaces import Box, Discrete
+from gymnasium.spaces import Box, Discrete
 
 from sample_factory.algo.utils.spaces.discretized import Discretized
 
 
 def key_to_action_basic(key):
     from pynput.keyboard import Key
```

### Comparing `sample-factory-2.0.3/sf_examples/vizdoom/doom/doom_gym.py` & `sample-factory-2.1.1/sf_examples/vizdoom/doom/doom_gym.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,18 +4,18 @@
 import re
 import time
 from os.path import join
 from threading import Thread
 from typing import Dict, Optional, Tuple
 
 import cv2
-import gym
+import gymnasium as gym
 import numpy as np
 from filelock import FileLock, Timeout
-from gym.utils import seeding
+from gymnasium.utils import seeding
 from vizdoom.vizdoom import AutomapMode, DoomGame, Mode, ScreenResolution
 
 from sample_factory.algo.utils.spaces.discretized import Discretized
 from sample_factory.utils.utils import log, project_tmp_dir
 
 
 def doom_lock_file(max_parallel):
```

### Comparing `sample-factory-2.0.3/sf_examples/vizdoom/doom/doom_model.py` & `sample-factory-2.1.1/sf_examples/vizdoom/doom/doom_model.py`

 * *Files identical despite different names*

### Comparing `sample-factory-2.0.3/sf_examples/vizdoom/doom/doom_params.py` & `sample-factory-2.1.1/sf_examples/vizdoom/doom/doom_params.py`

 * *Files identical despite different names*

### Comparing `sample-factory-2.0.3/sf_examples/vizdoom/doom/doom_play_demo.py` & `sample-factory-2.1.1/sf_examples/vizdoom/doom/doom_play_demo.py`

 * *Files identical despite different names*

### Comparing `sample-factory-2.0.3/sf_examples/vizdoom/doom/doom_render.py` & `sample-factory-2.1.1/sf_examples/vizdoom/doom/doom_render.py`

 * *Files identical despite different names*

### Comparing `sample-factory-2.0.3/sf_examples/vizdoom/doom/doom_utils.py` & `sample-factory-2.1.1/sf_examples/vizdoom/doom/doom_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import datetime
 import os
 from os.path import join
 from typing import Optional
 
-from gym.spaces import Discrete
+from gymnasium.spaces import Discrete
 
 from sample_factory.envs.env_wrappers import (
     PixelFormatChwWrapper,
     RecordingWrapper,
     ResizeWrapper,
     RewardScalingWrapper,
     TimeLimitWrapper,
```

### Comparing `sample-factory-2.0.3/sf_examples/vizdoom/doom/multi_agent_match.py` & `sample-factory-2.1.1/sf_examples/vizdoom/doom/multi_agent_match.py`

 * *Files identical despite different names*

### Comparing `sample-factory-2.0.3/sf_examples/vizdoom/doom/multiplayer/doom_multiagent.py` & `sample-factory-2.1.1/sf_examples/vizdoom/doom/multiplayer/doom_multiagent.py`

 * *Files identical despite different names*

### Comparing `sample-factory-2.0.3/sf_examples/vizdoom/doom/multiplayer/doom_multiagent_wrapper.py` & `sample-factory-2.1.1/sf_examples/vizdoom/doom/multiplayer/doom_multiagent_wrapper.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from queue import Empty, Queue
 from time import sleep
 from typing import Union
 
 import cv2
 import faster_fifo
 import filelock
-import gym
+import gymnasium as gym
 from filelock import FileLock
 
 from sample_factory.algo.utils.rl_utils import make_dones
 from sample_factory.envs.env_utils import RewardShapingInterface, get_default_reward_shaping
 from sample_factory.utils.utils import log
 from sf_examples.vizdoom.doom.doom_gym import doom_lock_file
 from sf_examples.vizdoom.doom.doom_render import concat_grid, cvt_doom_obs
```

### Comparing `sample-factory-2.0.3/sf_examples/vizdoom/doom/play_doom.py` & `sample-factory-2.1.1/sf_examples/vizdoom/doom/play_doom.py`

 * *Files identical despite different names*

### Comparing `sample-factory-2.0.3/sf_examples/vizdoom/doom/sample_env.py` & `sample-factory-2.1.1/sf_examples/vizdoom/doom/sample_env.py`

 * *Files identical despite different names*

### Comparing `sample-factory-2.0.3/sf_examples/vizdoom/doom/scenarios/basic.cfg` & `sample-factory-2.1.1/sf_examples/vizdoom/doom/scenarios/basic.cfg`

 * *Files identical despite different names*

### Comparing `sample-factory-2.0.3/sf_examples/vizdoom/doom/scenarios/basic.wad` & `sample-factory-2.1.1/sf_examples/vizdoom/doom/scenarios/basic.wad`

 * *Files identical despite different names*

### Comparing `sample-factory-2.0.3/sf_examples/vizdoom/doom/scenarios/battle.cfg` & `sample-factory-2.1.1/sf_examples/vizdoom/doom/scenarios/battle.cfg`

 * *Files identical despite different names*

### Comparing `sample-factory-2.0.3/sf_examples/vizdoom/doom/scenarios/battle.wad` & `sample-factory-2.1.1/sf_examples/vizdoom/doom/scenarios/battle.wad`

 * *Files identical despite different names*

### Comparing `sample-factory-2.0.3/sf_examples/vizdoom/doom/scenarios/battle2.wad` & `sample-factory-2.1.1/sf_examples/vizdoom/doom/scenarios/battle2.wad`

 * *Files identical despite different names*

### Comparing `sample-factory-2.0.3/sf_examples/vizdoom/doom/scenarios/battle2_continuous_turning.cfg` & `sample-factory-2.1.1/sf_examples/vizdoom/doom/scenarios/battle2_continuous_turning.cfg`

 * *Files identical despite different names*

### Comparing `sample-factory-2.0.3/sf_examples/vizdoom/doom/scenarios/battle_continuous_turning.cfg` & `sample-factory-2.1.1/sf_examples/vizdoom/doom/scenarios/battle_continuous_turning.cfg`

 * *Files identical despite different names*

### Comparing `sample-factory-2.0.3/sf_examples/vizdoom/doom/scenarios/cig.cfg` & `sample-factory-2.1.1/sf_examples/vizdoom/doom/scenarios/cig.cfg`

 * *Files identical despite different names*

### Comparing `sample-factory-2.0.3/sf_examples/vizdoom/doom/scenarios/cig.wad` & `sample-factory-2.1.1/sf_examples/vizdoom/doom/scenarios/cig.wad`

 * *Files identical despite different names*

### Comparing `sample-factory-2.0.3/sf_examples/vizdoom/doom/scenarios/deadly_corridor.cfg` & `sample-factory-2.1.1/sf_examples/vizdoom/doom/scenarios/deadly_corridor.cfg`

 * *Files identical despite different names*

### Comparing `sample-factory-2.0.3/sf_examples/vizdoom/doom/scenarios/deadly_corridor.wad` & `sample-factory-2.1.1/sf_examples/vizdoom/doom/scenarios/deadly_corridor.wad`

 * *Files identical despite different names*

### Comparing `sample-factory-2.0.3/sf_examples/vizdoom/doom/scenarios/defend_the_center.cfg` & `sample-factory-2.1.1/sf_examples/vizdoom/doom/scenarios/defend_the_center.cfg`

 * *Files identical despite different names*

### Comparing `sample-factory-2.0.3/sf_examples/vizdoom/doom/scenarios/defend_the_center.wad` & `sample-factory-2.1.1/sf_examples/vizdoom/doom/scenarios/defend_the_center.wad`

 * *Files identical despite different names*

### Comparing `sample-factory-2.0.3/sf_examples/vizdoom/doom/scenarios/defend_the_line.cfg` & `sample-factory-2.1.1/sf_examples/vizdoom/doom/scenarios/defend_the_line.cfg`

 * *Files identical despite different names*

### Comparing `sample-factory-2.0.3/sf_examples/vizdoom/doom/scenarios/defend_the_line.wad` & `sample-factory-2.1.1/sf_examples/vizdoom/doom/scenarios/defend_the_line.wad`

 * *Files identical despite different names*

### Comparing `sample-factory-2.0.3/sf_examples/vizdoom/doom/scenarios/dwango5.wad` & `sample-factory-2.1.1/sf_examples/vizdoom/doom/scenarios/dwango5.wad`

 * *Files identical despite different names*

### Comparing `sample-factory-2.0.3/sf_examples/vizdoom/doom/scenarios/dwango5_dm.cfg` & `sample-factory-2.1.1/sf_examples/vizdoom/doom/scenarios/dwango5_dm.cfg`

 * *Files identical despite different names*

### Comparing `sample-factory-2.0.3/sf_examples/vizdoom/doom/scenarios/dwango5_dm_continuous_weap.cfg` & `sample-factory-2.1.1/sf_examples/vizdoom/doom/scenarios/dwango5_dm_continuous_weap.cfg`

 * *Files identical despite different names*

### Comparing `sample-factory-2.0.3/sf_examples/vizdoom/doom/scenarios/freedm.cfg` & `sample-factory-2.1.1/sf_examples/vizdoom/doom/scenarios/freedm.cfg`

 * *Files identical despite different names*

### Comparing `sample-factory-2.0.3/sf_examples/vizdoom/doom/scenarios/freedm.wad` & `sample-factory-2.1.1/sf_examples/vizdoom/doom/scenarios/freedm.wad`

 * *Files identical despite different names*

### Comparing `sample-factory-2.0.3/sf_examples/vizdoom/doom/scenarios/health_gathering.cfg` & `sample-factory-2.1.1/sf_examples/vizdoom/doom/scenarios/health_gathering.cfg`

 * *Files identical despite different names*

### Comparing `sample-factory-2.0.3/sf_examples/vizdoom/doom/scenarios/health_gathering.wad` & `sample-factory-2.1.1/sf_examples/vizdoom/doom/scenarios/health_gathering.wad`

 * *Files identical despite different names*

### Comparing `sample-factory-2.0.3/sf_examples/vizdoom/doom/scenarios/health_gathering_supreme.cfg` & `sample-factory-2.1.1/sf_examples/vizdoom/doom/scenarios/health_gathering_supreme.cfg`

 * *Files identical despite different names*

### Comparing `sample-factory-2.0.3/sf_examples/vizdoom/doom/scenarios/health_gathering_supreme.wad` & `sample-factory-2.1.1/sf_examples/vizdoom/doom/scenarios/health_gathering_supreme.wad`

 * *Files identical despite different names*

### Comparing `sample-factory-2.0.3/sf_examples/vizdoom/doom/scenarios/my_way_home.cfg` & `sample-factory-2.1.1/sf_examples/vizdoom/doom/scenarios/my_way_home.cfg`

 * *Files identical despite different names*

### Comparing `sample-factory-2.0.3/sf_examples/vizdoom/doom/scenarios/my_way_home.wad` & `sample-factory-2.1.1/sf_examples/vizdoom/doom/scenarios/my_way_home.wad`

 * *Files identical despite different names*

### Comparing `sample-factory-2.0.3/sf_examples/vizdoom/doom/scenarios/ssl2.cfg` & `sample-factory-2.1.1/sf_examples/vizdoom/doom/scenarios/ssl2.cfg`

 * *Files identical despite different names*

### Comparing `sample-factory-2.0.3/sf_examples/vizdoom/doom/scenarios/ssl2.wad` & `sample-factory-2.1.1/sf_examples/vizdoom/doom/scenarios/ssl2.wad`

 * *Files identical despite different names*

### Comparing `sample-factory-2.0.3/sf_examples/vizdoom/doom/scenarios/two_colors_easy.cfg` & `sample-factory-2.1.1/sf_examples/vizdoom/doom/scenarios/two_colors_easy.cfg`

 * *Files identical despite different names*

### Comparing `sample-factory-2.0.3/sf_examples/vizdoom/doom/scenarios/two_colors_easy.wad` & `sample-factory-2.1.1/sf_examples/vizdoom/doom/scenarios/two_colors_easy.wad`

 * *Files identical despite different names*

### Comparing `sample-factory-2.0.3/sf_examples/vizdoom/doom/scenarios/two_colors_hard.cfg` & `sample-factory-2.1.1/sf_examples/vizdoom/doom/scenarios/two_colors_hard.cfg`

 * *Files identical despite different names*

### Comparing `sample-factory-2.0.3/sf_examples/vizdoom/doom/scenarios/two_colors_hard.wad` & `sample-factory-2.1.1/sf_examples/vizdoom/doom/scenarios/two_colors_hard.wad`

 * *Files identical despite different names*

### Comparing `sample-factory-2.0.3/sf_examples/vizdoom/doom/scripts/generate_bots.py` & `sample-factory-2.1.1/sf_examples/vizdoom/doom/scripts/generate_bots.py`

 * *Files identical despite different names*

### Comparing `sample-factory-2.0.3/sf_examples/vizdoom/doom/wrappers/additional_input.py` & `sample-factory-2.1.1/sf_examples/vizdoom/doom/wrappers/additional_input.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import gym
+import gymnasium as gym
 import numpy as np
 
 from sf_examples.vizdoom.doom.wrappers.reward_shaping import NUM_WEAPONS
 
 
 class DoomAdditionalInput(gym.Wrapper):
     """Add game variables to the observation space + reward shaping."""
```

### Comparing `sample-factory-2.0.3/sf_examples/vizdoom/doom/wrappers/bot_difficulty.py` & `sample-factory-2.1.1/sf_examples/vizdoom/doom/wrappers/bot_difficulty.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import gym
+import gymnasium as gym
 
 from sample_factory.utils.utils import log
 
 # Wrapper no longer in use
 
 
 class BotDifficultyWrapper(gym.Wrapper):
```

### Comparing `sample-factory-2.0.3/sf_examples/vizdoom/doom/wrappers/exploration.py` & `sample-factory-2.1.1/sf_examples/vizdoom/doom/wrappers/exploration.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import math
 from collections import deque
 
-import gym
+import gymnasium as gym
 import numpy as np
 
 
 class ExplorationWrapper(gym.Wrapper):
     def __init__(self, env):
         super().__init__(env)
         self.landmarks = deque([], maxlen=200)
```

### Comparing `sample-factory-2.0.3/sf_examples/vizdoom/doom/wrappers/multiplayer_stats.py` & `sample-factory-2.1.1/sf_examples/vizdoom/doom/wrappers/multiplayer_stats.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import gym
+import gymnasium as gym
 import numpy as np
 
 from sample_factory.algo.utils.rl_utils import make_dones
 
 
 class MultiplayerStatsWrapper(gym.Wrapper):
     """Add to info things like place in the match, gap to leader, kill-death ratio etc."""
```

### Comparing `sample-factory-2.0.3/sf_examples/vizdoom/doom/wrappers/observation_space.py` & `sample-factory-2.1.1/sf_examples/vizdoom/doom/wrappers/observation_space.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import gym
+import gymnasium as gym
 
 resolutions = [
     "160x120",
     "200x125",
     "200x150",
     "256x144",
     "256x160",
```

### Comparing `sample-factory-2.0.3/sf_examples/vizdoom/doom/wrappers/reward_shaping.py` & `sample-factory-2.1.1/sf_examples/vizdoom/doom/wrappers/reward_shaping.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import copy
 import operator
 from collections import deque
 from typing import Callable
 
-import gym
+import gymnasium as gym
 
 from sample_factory.algo.utils.misc import EPS
 from sample_factory.envs.env_utils import RewardShapingInterface
 from sample_factory.utils.utils import log
 
 NUM_WEAPONS = 8
```

### Comparing `sample-factory-2.0.3/sf_examples/vizdoom/doom/wrappers/scenario_wrappers/gathering_reward_shaping.py` & `sample-factory-2.1.1/sf_examples/vizdoom/doom/wrappers/scenario_wrappers/gathering_reward_shaping.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import gym
+import gymnasium as gym
 
 
 class DoomGatheringRewardShaping(gym.Wrapper):
     """Reward shaping specific for gathering scenarios."""
 
     def __init__(self, env):
         super().__init__(env)
```

### Comparing `sample-factory-2.0.3/sf_examples/vizdoom/doom/wrappers/step_human_input.py` & `sample-factory-2.1.1/sf_examples/vizdoom/doom/wrappers/step_human_input.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import gym
+import gymnasium as gym
 import numpy as np
 
 
 # noinspection PyProtectedMember
 class StepHumanInput(gym.Wrapper):
     """Doom wrapper that allows to play with human input."""
```

### Comparing `sample-factory-2.0.3/sf_examples/vizdoom/enjoy_custom_vizdoom_env.py` & `sample-factory-2.1.1/sf_examples/vizdoom/enjoy_custom_vizdoom_env.py`

 * *Files identical despite different names*

### Comparing `sample-factory-2.0.3/sf_examples/vizdoom/enjoy_vizdoom.py` & `sample-factory-2.1.1/sf_examples/vizdoom/enjoy_vizdoom.py`

 * *Files identical despite different names*

### Comparing `sample-factory-2.0.3/sf_examples/vizdoom/train_custom_vizdoom_env.py` & `sample-factory-2.1.1/sf_examples/vizdoom/train_custom_vizdoom_env.py`

 * *Files identical despite different names*

### Comparing `sample-factory-2.0.3/sf_examples/vizdoom/train_vizdoom.py` & `sample-factory-2.1.1/sf_examples/vizdoom/train_vizdoom.py`

 * *Files 7% similar despite different names*

```diff
@@ -32,19 +32,17 @@
     # override Doom default values for algo parameters
     doom_override_defaults(parser)
     # second parsing pass yields the final configuration
     final_cfg = parse_full_cfg(parser, argv)
     return final_cfg
 
 
-def main():
+def main():  # pragma: no cover
     """Script entry point."""
     register_vizdoom_components()
-
     cfg = parse_vizdoom_cfg()
-
     status = run_rl(cfg)
     return status
 
 
-if __name__ == "__main__":
+if __name__ == "__main__":  # pragma: no cover
     sys.exit(main())
```

### Comparing `sample-factory-2.0.3/tests/test_launcher.py` & `sample-factory-2.1.1/tests/test_launcher.py`

 * *Files identical despite different names*

### Comparing `sample-factory-2.0.3/tests/test_precheck.py` & `sample-factory-2.1.1/tests/test_precheck.py`

 * *Files identical despite different names*

### Comparing `sample-factory-2.0.3/tests/test_utils.py` & `sample-factory-2.1.1/tests/test_utils.py`

 * *Files identical despite different names*

