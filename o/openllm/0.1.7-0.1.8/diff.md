# Comparing `tmp/openllm-0.1.7.tar.gz` & `tmp/openllm-0.1.8.tar.gz`

## Comparing `openllm-0.1.7.tar` & `openllm-0.1.8.tar`

### file list

```diff
@@ -1,149 +1,149 @@
--rw-r--r--   0        0        0     2215 2020-02-02 00:00:00.000000 openllm-0.1.7/.pre-commit-config.yaml
--rw-r--r--   0        0        0     2938 2020-02-02 00:00:00.000000 openllm-0.1.7/ADDING_NEW_MODEL.md
--rw-r--r--   0        0        0     3052 2020-02-02 00:00:00.000000 openllm-0.1.7/CHANGELOG.md
--rw-r--r--   0        0        0     6496 2020-02-02 00:00:00.000000 openllm-0.1.7/DEVELOPMENT.md
--rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 openllm-0.1.7/nightly-requirements.generated.txt
--rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 openllm-0.1.7/package.json
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 openllm-0.1.7/taplo.toml
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 openllm-0.1.7/.github/CODEOWNERS
--rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 openllm-0.1.7/.github/SECURITY.md
--rw-r--r--   0        0        0      953 2020-02-02 00:00:00.000000 openllm-0.1.7/.github/dependabot.yml
--rw-r--r--   0        0        0     2765 2020-02-02 00:00:00.000000 openllm-0.1.7/.github/ISSUE_TEMPLATE/bug_report.yml
--rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 openllm-0.1.7/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 openllm-0.1.7/.github/ISSUE_TEMPLATE/feature_request.yml
--rwxr-xr-x   0        0        0     1428 2020-02-02 00:00:00.000000 openllm-0.1.7/.github/actions/create_release_and_archive.sh
--rwxr-xr-x   0        0        0     1853 2020-02-02 00:00:00.000000 openllm-0.1.7/.github/actions/release.sh
--rw-r--r--   0        0        0     2081 2020-02-02 00:00:00.000000 openllm-0.1.7/.github/actions/setup-repo/action.yml
--rw-r--r--   0        0        0     1487 2020-02-02 00:00:00.000000 openllm-0.1.7/.github/workflows/ci.yml
--rw-r--r--   0        0        0     2061 2020-02-02 00:00:00.000000 openllm-0.1.7/.github/workflows/create-releases.yml
--rw-r--r--   0        0        0     3502 2020-02-02 00:00:00.000000 openllm-0.1.7/.github/workflows/release-notes.yml
--rw-r--r--   0        0        0  1264669 2020-02-02 00:00:00.000000 openllm-0.1.7/assets/main-banner.png
--rw-r--r--   0        0        0 10631249 2020-02-02 00:00:00.000000 openllm-0.1.7/assets/output.gif
--rw-r--r--   0        0        0      881 2020-02-02 00:00:00.000000 openllm-0.1.7/changelog.d/template.md.jinja
--rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 openllm-0.1.7/examples/bentoml-demo/bentofile.yaml
--rw-r--r--   0        0        0     1002 2020-02-02 00:00:00.000000 openllm-0.1.7/examples/bentoml-demo/service.py
--rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 openllm-0.1.7/examples/langchain-chains-demo/README.md
--rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 openllm-0.1.7/examples/langchain-chains-demo/bentofile.yaml
--rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 openllm-0.1.7/examples/langchain-chains-demo/download_model.py
--rw-r--r--   0        0        0     2271 2020-02-02 00:00:00.000000 openllm-0.1.7/examples/langchain-chains-demo/service.py
--rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 openllm-0.1.7/examples/langchain-tools-demo/README.md
--rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 openllm-0.1.7/examples/langchain-tools-demo/bentofile.yaml
--rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 openllm-0.1.7/examples/langchain-tools-demo/bentoml_configuration.yaml
--rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 openllm-0.1.7/examples/langchain-tools-demo/download_model.py
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 openllm-0.1.7/examples/langchain-tools-demo/requirements.txt
--rw-r--r--   0        0        0     1329 2020-02-02 00:00:00.000000 openllm-0.1.7/examples/langchain-tools-demo/service.py
--rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 openllm-0.1.7/src/openllm/__about__.py
--rw-r--r--   0        0        0     8872 2020-02-02 00:00:00.000000 openllm-0.1.7/src/openllm/__init__.py
--rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 openllm-0.1.7/src/openllm/__main__.py
--rw-r--r--   0        0        0    54358 2020-02-02 00:00:00.000000 openllm-0.1.7/src/openllm/_configuration.py
--rw-r--r--   0        0        0     1637 2020-02-02 00:00:00.000000 openllm-0.1.7/src/openllm/_generation.py
--rw-r--r--   0        0        0    43521 2020-02-02 00:00:00.000000 openllm-0.1.7/src/openllm/_llm.py
--rw-r--r--   0        0        0    13551 2020-02-02 00:00:00.000000 openllm-0.1.7/src/openllm/_package.py
--rw-r--r--   0        0        0     1636 2020-02-02 00:00:00.000000 openllm-0.1.7/src/openllm/_prompt.py
--rw-r--r--   0        0        0     2773 2020-02-02 00:00:00.000000 openllm-0.1.7/src/openllm/_schema.py
--rw-r--r--   0        0        0     3833 2020-02-02 00:00:00.000000 openllm-0.1.7/src/openllm/_service.py
--rw-r--r--   0        0        0     1461 2020-02-02 00:00:00.000000 openllm-0.1.7/src/openllm/_types.py
--rw-r--r--   0        0        0    48406 2020-02-02 00:00:00.000000 openllm-0.1.7/src/openllm/cli.py
--rw-r--r--   0        0        0     1882 2020-02-02 00:00:00.000000 openllm-0.1.7/src/openllm/client.py
--rw-r--r--   0        0        0     1390 2020-02-02 00:00:00.000000 openllm-0.1.7/src/openllm/exceptions.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openllm-0.1.7/src/openllm/py.typed
--rw-r--r--   0        0        0      855 2020-02-02 00:00:00.000000 openllm-0.1.7/src/openllm/models/__init__.py
--rw-r--r--   0        0        0     3367 2020-02-02 00:00:00.000000 openllm-0.1.7/src/openllm/models/auto/__init__.py
--rw-r--r--   0        0        0     4995 2020-02-02 00:00:00.000000 openllm-0.1.7/src/openllm/models/auto/configuration_auto.py
--rw-r--r--   0        0        0    12738 2020-02-02 00:00:00.000000 openllm-0.1.7/src/openllm/models/auto/factory.py
--rw-r--r--   0        0        0     1428 2020-02-02 00:00:00.000000 openllm-0.1.7/src/openllm/models/auto/modeling_auto.py
--rw-r--r--   0        0        0     1299 2020-02-02 00:00:00.000000 openllm-0.1.7/src/openllm/models/auto/modeling_flax_auto.py
--rw-r--r--   0        0        0     1283 2020-02-02 00:00:00.000000 openllm-0.1.7/src/openllm/models/auto/modeling_tf_auto.py
--rw-r--r--   0        0        0     1837 2020-02-02 00:00:00.000000 openllm-0.1.7/src/openllm/models/chatglm/__init__.py
--rw-r--r--   0        0        0     3071 2020-02-02 00:00:00.000000 openllm-0.1.7/src/openllm/models/chatglm/configuration_chatglm.py
--rw-r--r--   0        0        0     4783 2020-02-02 00:00:00.000000 openllm-0.1.7/src/openllm/models/chatglm/modeling_chatglm.py
--rw-r--r--   0        0        0     1750 2020-02-02 00:00:00.000000 openllm-0.1.7/src/openllm/models/dolly_v2/__init__.py
--rw-r--r--   0        0        0     3597 2020-02-02 00:00:00.000000 openllm-0.1.7/src/openllm/models/dolly_v2/configuration_dolly_v2.py
--rw-r--r--   0        0        0     4091 2020-02-02 00:00:00.000000 openllm-0.1.7/src/openllm/models/dolly_v2/modeling_dolly_v2.py
--rw-r--r--   0        0        0     1726 2020-02-02 00:00:00.000000 openllm-0.1.7/src/openllm/models/falcon/__init__.py
--rw-r--r--   0        0        0     2500 2020-02-02 00:00:00.000000 openllm-0.1.7/src/openllm/models/falcon/configuration_falcon.py
--rw-r--r--   0        0        0     5353 2020-02-02 00:00:00.000000 openllm-0.1.7/src/openllm/models/falcon/modeling_falcon.py
--rw-r--r--   0        0        0     2726 2020-02-02 00:00:00.000000 openllm-0.1.7/src/openllm/models/flan_t5/__init__.py
--rw-r--r--   0        0        0     2547 2020-02-02 00:00:00.000000 openllm-0.1.7/src/openllm/models/flan_t5/configuration_flan_t5.py
--rw-r--r--   0        0        0     3559 2020-02-02 00:00:00.000000 openllm-0.1.7/src/openllm/models/flan_t5/modeling_flan_t5.py
--rw-r--r--   0        0        0     3750 2020-02-02 00:00:00.000000 openllm-0.1.7/src/openllm/models/flan_t5/modeling_flax_flan_t5.py
--rw-r--r--   0        0        0     2854 2020-02-02 00:00:00.000000 openllm-0.1.7/src/openllm/models/flan_t5/modeling_tf_flan_t5.py
--rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 openllm-0.1.7/src/openllm/models/gpt_neox/__init__.py
--rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 openllm-0.1.7/src/openllm/models/llama/__init__.py
--rw-r--r--   0        0        0     2638 2020-02-02 00:00:00.000000 openllm-0.1.7/src/openllm/models/opt/__init__.py
--rw-r--r--   0        0        0     3067 2020-02-02 00:00:00.000000 openllm-0.1.7/src/openllm/models/opt/configuration_opt.py
--rw-r--r--   0        0        0     4733 2020-02-02 00:00:00.000000 openllm-0.1.7/src/openllm/models/opt/modeling_flax_opt.py
--rw-r--r--   0        0        0     5942 2020-02-02 00:00:00.000000 openllm-0.1.7/src/openllm/models/opt/modeling_opt.py
--rw-r--r--   0        0        0     4615 2020-02-02 00:00:00.000000 openllm-0.1.7/src/openllm/models/opt/modeling_tf_opt.py
--rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 openllm-0.1.7/src/openllm/models/roberta/__init__.py
--rw-r--r--   0        0        0     1756 2020-02-02 00:00:00.000000 openllm-0.1.7/src/openllm/models/stablelm/__init__.py
--rw-r--r--   0        0        0     3273 2020-02-02 00:00:00.000000 openllm-0.1.7/src/openllm/models/stablelm/configuration_stablelm.py
--rw-r--r--   0        0        0     4219 2020-02-02 00:00:00.000000 openllm-0.1.7/src/openllm/models/stablelm/modeling_stablelm.py
--rw-r--r--   0        0        0     1771 2020-02-02 00:00:00.000000 openllm-0.1.7/src/openllm/models/starcoder/__init__.py
--rw-r--r--   0        0        0     2566 2020-02-02 00:00:00.000000 openllm-0.1.7/src/openllm/models/starcoder/configuration_starcoder.py
--rw-r--r--   0        0        0     6346 2020-02-02 00:00:00.000000 openllm-0.1.7/src/openllm/models/starcoder/modeling_starcoder.py
--rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 openllm-0.1.7/src/openllm/playground/README
--rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 openllm-0.1.7/src/openllm/playground/__init__.py
--rw-r--r--   0        0        0     2195 2020-02-02 00:00:00.000000 openllm-0.1.7/src/openllm/playground/features.py
--rw-r--r--   0        0        0     4099 2020-02-02 00:00:00.000000 openllm-0.1.7/src/openllm/playground/ft_opt_lora.py
--rw-r--r--   0        0        0     7440 2020-02-02 00:00:00.000000 openllm-0.1.7/src/openllm/utils/__init__.py
--rw-r--r--   0        0        0     2757 2020-02-02 00:00:00.000000 openllm-0.1.7/src/openllm/utils/analytics.py
--rw-r--r--   0        0        0     5515 2020-02-02 00:00:00.000000 openllm-0.1.7/src/openllm/utils/codegen.py
--rw-r--r--   0        0        0    15488 2020-02-02 00:00:00.000000 openllm-0.1.7/src/openllm/utils/dantic.py
--rw-r--r--   0        0        0     1254 2020-02-02 00:00:00.000000 openllm-0.1.7/src/openllm/utils/dummy_flax_objects.py
--rw-r--r--   0        0        0      923 2020-02-02 00:00:00.000000 openllm-0.1.7/src/openllm/utils/dummy_pt_and_cpm_kernels_objects.py
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 openllm-0.1.7/src/openllm/utils/dummy_pt_and_einops_objects.py
--rw-r--r--   0        0        0     1744 2020-02-02 00:00:00.000000 openllm-0.1.7/src/openllm/utils/dummy_pt_objects.py
--rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 openllm-0.1.7/src/openllm/utils/dummy_tf_objects.py
--rw-r--r--   0        0        0    12067 2020-02-02 00:00:00.000000 openllm-0.1.7/src/openllm/utils/import_utils.py
--rw-r--r--   0        0        0     5190 2020-02-02 00:00:00.000000 openllm-0.1.7/src/openllm/utils/lazy.py
--rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 openllm-0.1.7/src/openllm_client/__init__.py
--rw-r--r--   0        0        0     2274 2020-02-02 00:00:00.000000 openllm-0.1.7/src/openllm_client/_prompt.py
--rw-r--r--   0        0        0      685 2020-02-02 00:00:00.000000 openllm-0.1.7/src/openllm_client/runtimes/__init__.py
--rw-r--r--   0        0        0    11495 2020-02-02 00:00:00.000000 openllm-0.1.7/src/openllm_client/runtimes/base.py
--rw-r--r--   0        0        0     3522 2020-02-02 00:00:00.000000 openllm-0.1.7/src/openllm_client/runtimes/grpc.py
--rw-r--r--   0        0        0     2904 2020-02-02 00:00:00.000000 openllm-0.1.7/src/openllm_client/runtimes/http.py
--rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 openllm-0.1.7/src/openllm_js/package.json
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 openllm-0.1.7/src/openllm_js/tsconfig.cjs.json
--rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 openllm-0.1.7/src/openllm_js/tsconfig.json
--rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 openllm-0.1.7/tests/__init__.py
--rw-r--r--   0        0        0     5658 2020-02-02 00:00:00.000000 openllm-0.1.7/tests/test_configuration.py
--rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 openllm-0.1.7/tests/_strategies/__init__.py
--rw-r--r--   0        0        0     3094 2020-02-02 00:00:00.000000 openllm-0.1.7/tests/_strategies/_configuration.py
--rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 openllm-0.1.7/tests/models/flan_t5/__init__.py
--rw-r--r--   0        0        0     1308 2020-02-02 00:00:00.000000 openllm-0.1.7/tests/models/flan_t5/test_modeling_flan_t5.py
--rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 openllm-0.1.7/tests/models/opt/__init__.py
--rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 openllm-0.1.7/tests/models/opt/test_modeling_opt.py
--rwxr-xr-x   0        0        0      489 2020-02-02 00:00:00.000000 openllm-0.1.7/tools/add-license-headers
--rwxr-xr-x   0        0        0      359 2020-02-02 00:00:00.000000 openllm-0.1.7/tools/assert-license-headers
--rwxr-xr-x   0        0        0      791 2020-02-02 00:00:00.000000 openllm-0.1.7/tools/assert-model-table-latest
--rwxr-xr-x   0        0        0     1901 2020-02-02 00:00:00.000000 openllm-0.1.7/tools/run-release-action
--rwxr-xr-x   0        0        0     5012 2020-02-02 00:00:00.000000 openllm-0.1.7/tools/update-optional-dependencies.py
--rwxr-xr-x   0        0        0     3575 2020-02-02 00:00:00.000000 openllm-0.1.7/tools/update-readme.py
--rw-r--r--   0        0        0    15821 2020-02-02 00:00:00.000000 openllm-0.1.7/typings/attr/__init__.pyi
--rw-r--r--   0        0        0      435 2020-02-02 00:00:00.000000 openllm-0.1.7/typings/attr/_cmp.pyi
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 openllm-0.1.7/typings/attr/_compat.pyi
--rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 openllm-0.1.7/typings/attr/_typing_compat.pyi
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 openllm-0.1.7/typings/attr/_version_info.pyi
--rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 openllm-0.1.7/typings/attr/converters.pyi
--rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 openllm-0.1.7/typings/attr/exceptions.pyi
--rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 openllm-0.1.7/typings/attr/filters.pyi
--rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 openllm-0.1.7/typings/attr/setters.pyi
--rw-r--r--   0        0        0     2608 2020-02-02 00:00:00.000000 openllm-0.1.7/typings/attr/validators.pyi
--rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 openllm-0.1.7/typings/click_option_group/__init__.pyi
--rw-r--r--   0        0        0     6238 2020-02-02 00:00:00.000000 openllm-0.1.7/typings/click_option_group/_core.pyi
--rw-r--r--   0        0        0     3691 2020-02-02 00:00:00.000000 openllm-0.1.7/typings/click_option_group/_decorators.pyi
--rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 openllm-0.1.7/typings/click_option_group/_helpers.pyi
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 openllm-0.1.7/typings/click_option_group/_version.pyi
--rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 openllm-0.1.7/typings/deepmerge/__init__.pyi
--rw-r--r--   0        0        0      851 2020-02-02 00:00:00.000000 openllm-0.1.7/typings/deepmerge/merger.pyi
--rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 openllm-0.1.7/typings/deepmerge/strategy/core.pyi
--rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 openllm-0.1.7/typings/deepmerge/strategy/dict.pyi
--rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 openllm-0.1.7/typings/deepmerge/strategy/list.pyi
--rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 openllm-0.1.7/typings/deepmerge/strategy/set.pyi
--rw-r--r--   0        0        0     1858 2020-02-02 00:00:00.000000 openllm-0.1.7/.gitignore
--rw-r--r--   0        0        0    10470 2020-02-02 00:00:00.000000 openllm-0.1.7/LICENSE.md
--rw-r--r--   0        0        0    14939 2020-02-02 00:00:00.000000 openllm-0.1.7/README.md
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 openllm-0.1.7/hatch.toml
--rw-r--r--   0        0        0     5808 2020-02-02 00:00:00.000000 openllm-0.1.7/pyproject.toml
--rw-r--r--   0        0        0    18201 2020-02-02 00:00:00.000000 openllm-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0     2215 2020-02-02 00:00:00.000000 openllm-0.1.8/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     2938 2020-02-02 00:00:00.000000 openllm-0.1.8/ADDING_NEW_MODEL.md
+-rw-r--r--   0        0        0     3137 2020-02-02 00:00:00.000000 openllm-0.1.8/CHANGELOG.md
+-rw-r--r--   0        0        0     6496 2020-02-02 00:00:00.000000 openllm-0.1.8/DEVELOPMENT.md
+-rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 openllm-0.1.8/nightly-requirements.generated.txt
+-rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 openllm-0.1.8/package.json
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 openllm-0.1.8/taplo.toml
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 openllm-0.1.8/.github/CODEOWNERS
+-rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 openllm-0.1.8/.github/SECURITY.md
+-rw-r--r--   0        0        0      953 2020-02-02 00:00:00.000000 openllm-0.1.8/.github/dependabot.yml
+-rw-r--r--   0        0        0     2765 2020-02-02 00:00:00.000000 openllm-0.1.8/.github/ISSUE_TEMPLATE/bug_report.yml
+-rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 openllm-0.1.8/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 openllm-0.1.8/.github/ISSUE_TEMPLATE/feature_request.yml
+-rwxr-xr-x   0        0        0     1428 2020-02-02 00:00:00.000000 openllm-0.1.8/.github/actions/create_release_and_archive.sh
+-rwxr-xr-x   0        0        0     1853 2020-02-02 00:00:00.000000 openllm-0.1.8/.github/actions/release.sh
+-rw-r--r--   0        0        0     2081 2020-02-02 00:00:00.000000 openllm-0.1.8/.github/actions/setup-repo/action.yml
+-rw-r--r--   0        0        0     1487 2020-02-02 00:00:00.000000 openllm-0.1.8/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     2061 2020-02-02 00:00:00.000000 openllm-0.1.8/.github/workflows/create-releases.yml
+-rw-r--r--   0        0        0     3502 2020-02-02 00:00:00.000000 openllm-0.1.8/.github/workflows/release-notes.yml
+-rw-r--r--   0        0        0  1264669 2020-02-02 00:00:00.000000 openllm-0.1.8/assets/main-banner.png
+-rw-r--r--   0        0        0 10631249 2020-02-02 00:00:00.000000 openllm-0.1.8/assets/output.gif
+-rw-r--r--   0        0        0      881 2020-02-02 00:00:00.000000 openllm-0.1.8/changelog.d/template.md.jinja
+-rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 openllm-0.1.8/examples/bentoml-demo/bentofile.yaml
+-rw-r--r--   0        0        0     1002 2020-02-02 00:00:00.000000 openllm-0.1.8/examples/bentoml-demo/service.py
+-rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 openllm-0.1.8/examples/langchain-chains-demo/README.md
+-rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 openllm-0.1.8/examples/langchain-chains-demo/bentofile.yaml
+-rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 openllm-0.1.8/examples/langchain-chains-demo/download_model.py
+-rw-r--r--   0        0        0     2271 2020-02-02 00:00:00.000000 openllm-0.1.8/examples/langchain-chains-demo/service.py
+-rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 openllm-0.1.8/examples/langchain-tools-demo/README.md
+-rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 openllm-0.1.8/examples/langchain-tools-demo/bentofile.yaml
+-rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 openllm-0.1.8/examples/langchain-tools-demo/bentoml_configuration.yaml
+-rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 openllm-0.1.8/examples/langchain-tools-demo/download_model.py
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 openllm-0.1.8/examples/langchain-tools-demo/requirements.txt
+-rw-r--r--   0        0        0     1329 2020-02-02 00:00:00.000000 openllm-0.1.8/examples/langchain-tools-demo/service.py
+-rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 openllm-0.1.8/src/openllm/__about__.py
+-rw-r--r--   0        0        0     8872 2020-02-02 00:00:00.000000 openllm-0.1.8/src/openllm/__init__.py
+-rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 openllm-0.1.8/src/openllm/__main__.py
+-rw-r--r--   0        0        0    54358 2020-02-02 00:00:00.000000 openllm-0.1.8/src/openllm/_configuration.py
+-rw-r--r--   0        0        0     1637 2020-02-02 00:00:00.000000 openllm-0.1.8/src/openllm/_generation.py
+-rw-r--r--   0        0        0    43521 2020-02-02 00:00:00.000000 openllm-0.1.8/src/openllm/_llm.py
+-rw-r--r--   0        0        0    13551 2020-02-02 00:00:00.000000 openllm-0.1.8/src/openllm/_package.py
+-rw-r--r--   0        0        0     1636 2020-02-02 00:00:00.000000 openllm-0.1.8/src/openllm/_prompt.py
+-rw-r--r--   0        0        0     2773 2020-02-02 00:00:00.000000 openllm-0.1.8/src/openllm/_schema.py
+-rw-r--r--   0        0        0     3833 2020-02-02 00:00:00.000000 openllm-0.1.8/src/openllm/_service.py
+-rw-r--r--   0        0        0     1461 2020-02-02 00:00:00.000000 openllm-0.1.8/src/openllm/_types.py
+-rw-r--r--   0        0        0    48388 2020-02-02 00:00:00.000000 openllm-0.1.8/src/openllm/cli.py
+-rw-r--r--   0        0        0     1882 2020-02-02 00:00:00.000000 openllm-0.1.8/src/openllm/client.py
+-rw-r--r--   0        0        0     1390 2020-02-02 00:00:00.000000 openllm-0.1.8/src/openllm/exceptions.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openllm-0.1.8/src/openllm/py.typed
+-rw-r--r--   0        0        0      855 2020-02-02 00:00:00.000000 openllm-0.1.8/src/openllm/models/__init__.py
+-rw-r--r--   0        0        0     3367 2020-02-02 00:00:00.000000 openllm-0.1.8/src/openllm/models/auto/__init__.py
+-rw-r--r--   0        0        0     4995 2020-02-02 00:00:00.000000 openllm-0.1.8/src/openllm/models/auto/configuration_auto.py
+-rw-r--r--   0        0        0    12738 2020-02-02 00:00:00.000000 openllm-0.1.8/src/openllm/models/auto/factory.py
+-rw-r--r--   0        0        0     1428 2020-02-02 00:00:00.000000 openllm-0.1.8/src/openllm/models/auto/modeling_auto.py
+-rw-r--r--   0        0        0     1299 2020-02-02 00:00:00.000000 openllm-0.1.8/src/openllm/models/auto/modeling_flax_auto.py
+-rw-r--r--   0        0        0     1283 2020-02-02 00:00:00.000000 openllm-0.1.8/src/openllm/models/auto/modeling_tf_auto.py
+-rw-r--r--   0        0        0     1837 2020-02-02 00:00:00.000000 openllm-0.1.8/src/openllm/models/chatglm/__init__.py
+-rw-r--r--   0        0        0     3071 2020-02-02 00:00:00.000000 openllm-0.1.8/src/openllm/models/chatglm/configuration_chatglm.py
+-rw-r--r--   0        0        0     4783 2020-02-02 00:00:00.000000 openllm-0.1.8/src/openllm/models/chatglm/modeling_chatglm.py
+-rw-r--r--   0        0        0     1750 2020-02-02 00:00:00.000000 openllm-0.1.8/src/openllm/models/dolly_v2/__init__.py
+-rw-r--r--   0        0        0     3597 2020-02-02 00:00:00.000000 openllm-0.1.8/src/openllm/models/dolly_v2/configuration_dolly_v2.py
+-rw-r--r--   0        0        0     4091 2020-02-02 00:00:00.000000 openllm-0.1.8/src/openllm/models/dolly_v2/modeling_dolly_v2.py
+-rw-r--r--   0        0        0     1726 2020-02-02 00:00:00.000000 openllm-0.1.8/src/openllm/models/falcon/__init__.py
+-rw-r--r--   0        0        0     2500 2020-02-02 00:00:00.000000 openllm-0.1.8/src/openllm/models/falcon/configuration_falcon.py
+-rw-r--r--   0        0        0     5353 2020-02-02 00:00:00.000000 openllm-0.1.8/src/openllm/models/falcon/modeling_falcon.py
+-rw-r--r--   0        0        0     2726 2020-02-02 00:00:00.000000 openllm-0.1.8/src/openllm/models/flan_t5/__init__.py
+-rw-r--r--   0        0        0     2547 2020-02-02 00:00:00.000000 openllm-0.1.8/src/openllm/models/flan_t5/configuration_flan_t5.py
+-rw-r--r--   0        0        0     3559 2020-02-02 00:00:00.000000 openllm-0.1.8/src/openllm/models/flan_t5/modeling_flan_t5.py
+-rw-r--r--   0        0        0     3750 2020-02-02 00:00:00.000000 openllm-0.1.8/src/openllm/models/flan_t5/modeling_flax_flan_t5.py
+-rw-r--r--   0        0        0     2854 2020-02-02 00:00:00.000000 openllm-0.1.8/src/openllm/models/flan_t5/modeling_tf_flan_t5.py
+-rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 openllm-0.1.8/src/openllm/models/gpt_neox/__init__.py
+-rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 openllm-0.1.8/src/openllm/models/llama/__init__.py
+-rw-r--r--   0        0        0     2638 2020-02-02 00:00:00.000000 openllm-0.1.8/src/openllm/models/opt/__init__.py
+-rw-r--r--   0        0        0     3067 2020-02-02 00:00:00.000000 openllm-0.1.8/src/openllm/models/opt/configuration_opt.py
+-rw-r--r--   0        0        0     4733 2020-02-02 00:00:00.000000 openllm-0.1.8/src/openllm/models/opt/modeling_flax_opt.py
+-rw-r--r--   0        0        0     5942 2020-02-02 00:00:00.000000 openllm-0.1.8/src/openllm/models/opt/modeling_opt.py
+-rw-r--r--   0        0        0     4615 2020-02-02 00:00:00.000000 openllm-0.1.8/src/openllm/models/opt/modeling_tf_opt.py
+-rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 openllm-0.1.8/src/openllm/models/roberta/__init__.py
+-rw-r--r--   0        0        0     1756 2020-02-02 00:00:00.000000 openllm-0.1.8/src/openllm/models/stablelm/__init__.py
+-rw-r--r--   0        0        0     3273 2020-02-02 00:00:00.000000 openllm-0.1.8/src/openllm/models/stablelm/configuration_stablelm.py
+-rw-r--r--   0        0        0     4219 2020-02-02 00:00:00.000000 openllm-0.1.8/src/openllm/models/stablelm/modeling_stablelm.py
+-rw-r--r--   0        0        0     1771 2020-02-02 00:00:00.000000 openllm-0.1.8/src/openllm/models/starcoder/__init__.py
+-rw-r--r--   0        0        0     2566 2020-02-02 00:00:00.000000 openllm-0.1.8/src/openllm/models/starcoder/configuration_starcoder.py
+-rw-r--r--   0        0        0     6346 2020-02-02 00:00:00.000000 openllm-0.1.8/src/openllm/models/starcoder/modeling_starcoder.py
+-rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 openllm-0.1.8/src/openllm/playground/README
+-rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 openllm-0.1.8/src/openllm/playground/__init__.py
+-rw-r--r--   0        0        0     2195 2020-02-02 00:00:00.000000 openllm-0.1.8/src/openllm/playground/features.py
+-rw-r--r--   0        0        0     4099 2020-02-02 00:00:00.000000 openllm-0.1.8/src/openllm/playground/ft_opt_lora.py
+-rw-r--r--   0        0        0     7440 2020-02-02 00:00:00.000000 openllm-0.1.8/src/openllm/utils/__init__.py
+-rw-r--r--   0        0        0     2757 2020-02-02 00:00:00.000000 openllm-0.1.8/src/openllm/utils/analytics.py
+-rw-r--r--   0        0        0     5515 2020-02-02 00:00:00.000000 openllm-0.1.8/src/openllm/utils/codegen.py
+-rw-r--r--   0        0        0    15488 2020-02-02 00:00:00.000000 openllm-0.1.8/src/openllm/utils/dantic.py
+-rw-r--r--   0        0        0     1254 2020-02-02 00:00:00.000000 openllm-0.1.8/src/openllm/utils/dummy_flax_objects.py
+-rw-r--r--   0        0        0      923 2020-02-02 00:00:00.000000 openllm-0.1.8/src/openllm/utils/dummy_pt_and_cpm_kernels_objects.py
+-rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 openllm-0.1.8/src/openllm/utils/dummy_pt_and_einops_objects.py
+-rw-r--r--   0        0        0     1744 2020-02-02 00:00:00.000000 openllm-0.1.8/src/openllm/utils/dummy_pt_objects.py
+-rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 openllm-0.1.8/src/openllm/utils/dummy_tf_objects.py
+-rw-r--r--   0        0        0    12067 2020-02-02 00:00:00.000000 openllm-0.1.8/src/openllm/utils/import_utils.py
+-rw-r--r--   0        0        0     5190 2020-02-02 00:00:00.000000 openllm-0.1.8/src/openllm/utils/lazy.py
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 openllm-0.1.8/src/openllm_client/__init__.py
+-rw-r--r--   0        0        0     2274 2020-02-02 00:00:00.000000 openllm-0.1.8/src/openllm_client/_prompt.py
+-rw-r--r--   0        0        0      685 2020-02-02 00:00:00.000000 openllm-0.1.8/src/openllm_client/runtimes/__init__.py
+-rw-r--r--   0        0        0    11495 2020-02-02 00:00:00.000000 openllm-0.1.8/src/openllm_client/runtimes/base.py
+-rw-r--r--   0        0        0     3522 2020-02-02 00:00:00.000000 openllm-0.1.8/src/openllm_client/runtimes/grpc.py
+-rw-r--r--   0        0        0     2904 2020-02-02 00:00:00.000000 openllm-0.1.8/src/openllm_client/runtimes/http.py
+-rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 openllm-0.1.8/src/openllm_js/package.json
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 openllm-0.1.8/src/openllm_js/tsconfig.cjs.json
+-rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 openllm-0.1.8/src/openllm_js/tsconfig.json
+-rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 openllm-0.1.8/tests/__init__.py
+-rw-r--r--   0        0        0     5658 2020-02-02 00:00:00.000000 openllm-0.1.8/tests/test_configuration.py
+-rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 openllm-0.1.8/tests/_strategies/__init__.py
+-rw-r--r--   0        0        0     3094 2020-02-02 00:00:00.000000 openllm-0.1.8/tests/_strategies/_configuration.py
+-rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 openllm-0.1.8/tests/models/flan_t5/__init__.py
+-rw-r--r--   0        0        0     1308 2020-02-02 00:00:00.000000 openllm-0.1.8/tests/models/flan_t5/test_modeling_flan_t5.py
+-rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 openllm-0.1.8/tests/models/opt/__init__.py
+-rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 openllm-0.1.8/tests/models/opt/test_modeling_opt.py
+-rwxr-xr-x   0        0        0      489 2020-02-02 00:00:00.000000 openllm-0.1.8/tools/add-license-headers
+-rwxr-xr-x   0        0        0      359 2020-02-02 00:00:00.000000 openllm-0.1.8/tools/assert-license-headers
+-rwxr-xr-x   0        0        0      791 2020-02-02 00:00:00.000000 openllm-0.1.8/tools/assert-model-table-latest
+-rwxr-xr-x   0        0        0     1901 2020-02-02 00:00:00.000000 openllm-0.1.8/tools/run-release-action
+-rwxr-xr-x   0        0        0     5012 2020-02-02 00:00:00.000000 openllm-0.1.8/tools/update-optional-dependencies.py
+-rwxr-xr-x   0        0        0     3575 2020-02-02 00:00:00.000000 openllm-0.1.8/tools/update-readme.py
+-rw-r--r--   0        0        0    15821 2020-02-02 00:00:00.000000 openllm-0.1.8/typings/attr/__init__.pyi
+-rw-r--r--   0        0        0      435 2020-02-02 00:00:00.000000 openllm-0.1.8/typings/attr/_cmp.pyi
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 openllm-0.1.8/typings/attr/_compat.pyi
+-rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 openllm-0.1.8/typings/attr/_typing_compat.pyi
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 openllm-0.1.8/typings/attr/_version_info.pyi
+-rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 openllm-0.1.8/typings/attr/converters.pyi
+-rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 openllm-0.1.8/typings/attr/exceptions.pyi
+-rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 openllm-0.1.8/typings/attr/filters.pyi
+-rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 openllm-0.1.8/typings/attr/setters.pyi
+-rw-r--r--   0        0        0     2608 2020-02-02 00:00:00.000000 openllm-0.1.8/typings/attr/validators.pyi
+-rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 openllm-0.1.8/typings/click_option_group/__init__.pyi
+-rw-r--r--   0        0        0     6238 2020-02-02 00:00:00.000000 openllm-0.1.8/typings/click_option_group/_core.pyi
+-rw-r--r--   0        0        0     3691 2020-02-02 00:00:00.000000 openllm-0.1.8/typings/click_option_group/_decorators.pyi
+-rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 openllm-0.1.8/typings/click_option_group/_helpers.pyi
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 openllm-0.1.8/typings/click_option_group/_version.pyi
+-rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 openllm-0.1.8/typings/deepmerge/__init__.pyi
+-rw-r--r--   0        0        0      851 2020-02-02 00:00:00.000000 openllm-0.1.8/typings/deepmerge/merger.pyi
+-rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 openllm-0.1.8/typings/deepmerge/strategy/core.pyi
+-rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 openllm-0.1.8/typings/deepmerge/strategy/dict.pyi
+-rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 openllm-0.1.8/typings/deepmerge/strategy/list.pyi
+-rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 openllm-0.1.8/typings/deepmerge/strategy/set.pyi
+-rw-r--r--   0        0        0     1858 2020-02-02 00:00:00.000000 openllm-0.1.8/.gitignore
+-rw-r--r--   0        0        0    10470 2020-02-02 00:00:00.000000 openllm-0.1.8/LICENSE.md
+-rw-r--r--   0        0        0    14995 2020-02-02 00:00:00.000000 openllm-0.1.8/README.md
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 openllm-0.1.8/hatch.toml
+-rw-r--r--   0        0        0     5808 2020-02-02 00:00:00.000000 openllm-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0    18257 2020-02-02 00:00:00.000000 openllm-0.1.8/PKG-INFO
```

### Comparing `openllm-0.1.7/.pre-commit-config.yaml` & `openllm-0.1.8/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `openllm-0.1.7/ADDING_NEW_MODEL.md` & `openllm-0.1.8/ADDING_NEW_MODEL.md`

 * *Files identical despite different names*

### Comparing `openllm-0.1.7/CHANGELOG.md` & `openllm-0.1.8/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -14,14 +14,18 @@
 Do *NOT* add changelog entries here!
 
 This changelog is managed by towncrier and is compiled at release time.
 -->
 
 <!-- towncrier release notes start -->
 
+## [0.1.8](https://github.com/bentoml/openllm/tree/v0.1.8)
+No significant changes.
+
+
 ## [0.1.7](https://github.com/bentoml/openllm/tree/v0.1.7)
 
 ### Features
 
 - OpenLLM now seamlessly integrates with HuggingFace Agents.
   Replace the HfAgent endpoint with a running remote server.
```

### Comparing `openllm-0.1.7/DEVELOPMENT.md` & `openllm-0.1.8/DEVELOPMENT.md`

 * *Files identical despite different names*

### Comparing `openllm-0.1.7/nightly-requirements.generated.txt` & `openllm-0.1.8/nightly-requirements.generated.txt`

 * *Files identical despite different names*

### Comparing `openllm-0.1.7/package.json` & `openllm-0.1.8/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9545454545454546%*

 * *Differences: {"'version'": "'0.1.8'"}*

```diff
@@ -11,12 +11,12 @@
     "engines": {
         "node": ">=16"
     },
     "license": "Apache 2.0",
     "name": "openllm",
     "private": true,
     "repository": "git@github.com:llmsys/OpenLLM.git",
-    "version": "0.1.7",
+    "version": "0.1.8",
     "workspaces": [
         "src/openllm_js"
     ]
 }
```

### Comparing `openllm-0.1.7/.github/SECURITY.md` & `openllm-0.1.8/.github/SECURITY.md`

 * *Files identical despite different names*

### Comparing `openllm-0.1.7/.github/dependabot.yml` & `openllm-0.1.8/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `openllm-0.1.7/.github/ISSUE_TEMPLATE/bug_report.yml` & `openllm-0.1.8/.github/ISSUE_TEMPLATE/bug_report.yml`

 * *Files identical despite different names*

### Comparing `openllm-0.1.7/.github/ISSUE_TEMPLATE/config.yml` & `openllm-0.1.8/.github/ISSUE_TEMPLATE/config.yml`

 * *Files identical despite different names*

### Comparing `openllm-0.1.7/.github/ISSUE_TEMPLATE/feature_request.yml` & `openllm-0.1.8/.github/ISSUE_TEMPLATE/feature_request.yml`

 * *Files identical despite different names*

### Comparing `openllm-0.1.7/.github/actions/create_release_and_archive.sh` & `openllm-0.1.8/.github/actions/create_release_and_archive.sh`

 * *Files identical despite different names*

### Comparing `openllm-0.1.7/.github/actions/release.sh` & `openllm-0.1.8/.github/actions/release.sh`

 * *Files identical despite different names*

### Comparing `openllm-0.1.7/.github/actions/setup-repo/action.yml` & `openllm-0.1.8/.github/actions/setup-repo/action.yml`

 * *Files identical despite different names*

### Comparing `openllm-0.1.7/.github/workflows/ci.yml` & `openllm-0.1.8/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `openllm-0.1.7/.github/workflows/create-releases.yml` & `openllm-0.1.8/.github/workflows/create-releases.yml`

 * *Files identical despite different names*

### Comparing `openllm-0.1.7/.github/workflows/release-notes.yml` & `openllm-0.1.8/.github/workflows/release-notes.yml`

 * *Files identical despite different names*

### Comparing `openllm-0.1.7/assets/main-banner.png` & `openllm-0.1.8/assets/main-banner.png`

 * *Files identical despite different names*

### Comparing `openllm-0.1.7/assets/output.gif` & `openllm-0.1.8/assets/output.gif`

 * *Files identical despite different names*

### Comparing `openllm-0.1.7/changelog.d/template.md.jinja` & `openllm-0.1.8/changelog.d/template.md.jinja`

 * *Files identical despite different names*

### Comparing `openllm-0.1.7/examples/bentoml-demo/bentofile.yaml` & `openllm-0.1.8/examples/bentoml-demo/bentofile.yaml`

 * *Files identical despite different names*

### Comparing `openllm-0.1.7/examples/bentoml-demo/service.py` & `openllm-0.1.8/examples/bentoml-demo/service.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.7/examples/langchain-chains-demo/bentofile.yaml` & `openllm-0.1.8/examples/langchain-chains-demo/bentofile.yaml`

 * *Files identical despite different names*

### Comparing `openllm-0.1.7/examples/langchain-chains-demo/download_model.py` & `openllm-0.1.8/examples/langchain-chains-demo/download_model.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.7/examples/langchain-chains-demo/service.py` & `openllm-0.1.8/examples/langchain-chains-demo/service.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.7/examples/langchain-tools-demo/bentofile.yaml` & `openllm-0.1.8/examples/langchain-tools-demo/bentofile.yaml`

 * *Files identical despite different names*

### Comparing `openllm-0.1.7/examples/langchain-tools-demo/bentoml_configuration.yaml` & `openllm-0.1.8/examples/langchain-tools-demo/bentoml_configuration.yaml`

 * *Files identical despite different names*

### Comparing `openllm-0.1.7/examples/langchain-tools-demo/download_model.py` & `openllm-0.1.8/examples/langchain-tools-demo/download_model.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.7/examples/langchain-tools-demo/service.py` & `openllm-0.1.8/examples/langchain-tools-demo/service.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.7/src/openllm/__about__.py` & `openllm-0.1.8/src/openllm/playground/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,8 +7,7 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-__version__ = "0.1.7"
```

### Comparing `openllm-0.1.7/src/openllm/__init__.py` & `openllm-0.1.8/src/openllm/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.7/src/openllm/__main__.py` & `openllm-0.1.8/src/openllm/__main__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.7/src/openllm/_configuration.py` & `openllm-0.1.8/src/openllm/_configuration.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.7/src/openllm/_generation.py` & `openllm-0.1.8/src/openllm/_generation.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.7/src/openllm/_llm.py` & `openllm-0.1.8/src/openllm/_llm.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.7/src/openllm/_package.py` & `openllm-0.1.8/src/openllm/_package.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.7/src/openllm/_prompt.py` & `openllm-0.1.8/src/openllm/_prompt.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.7/src/openllm/_schema.py` & `openllm-0.1.8/src/openllm/_schema.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.7/src/openllm/_service.py` & `openllm-0.1.8/src/openllm/_service.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.7/src/openllm/_types.py` & `openllm-0.1.8/src/openllm/_types.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.7/src/openllm/cli.py` & `openllm-0.1.8/src/openllm/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -1140,16 +1140,14 @@
     $ openllm instruct --endpoint http://12.323.2.1:3000 \\
         "Is the following `text` (in Spanish) positive or negative?" \\
         --text "¡Este es un API muy agradable!"
     ```
     """
     client = openllm.client.HTTPClient(endpoint, timeout=timeout)
 
-    breakpoint()
-
     if agent == "hf":
         if not is_transformers_supports_agent():
             raise click.UsageError(
                 "Transformers version should be at least 4.29 to support HfAgent. "
                 "Upgrade with 'pip install -U transformers'"
             )
```

### Comparing `openllm-0.1.7/src/openllm/client.py` & `openllm-0.1.8/src/openllm/client.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.7/src/openllm/exceptions.py` & `openllm-0.1.8/src/openllm/exceptions.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.7/src/openllm/models/__init__.py` & `openllm-0.1.8/src/openllm/models/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.7/src/openllm/models/auto/__init__.py` & `openllm-0.1.8/src/openllm/models/auto/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.7/src/openllm/models/auto/configuration_auto.py` & `openllm-0.1.8/src/openllm/models/auto/configuration_auto.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.7/src/openllm/models/auto/factory.py` & `openllm-0.1.8/src/openllm/models/auto/factory.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.7/src/openllm/models/auto/modeling_auto.py` & `openllm-0.1.8/src/openllm/models/auto/modeling_auto.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.7/src/openllm/models/auto/modeling_flax_auto.py` & `openllm-0.1.8/src/openllm/models/auto/modeling_flax_auto.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.7/src/openllm/models/auto/modeling_tf_auto.py` & `openllm-0.1.8/src/openllm/models/auto/modeling_tf_auto.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.7/src/openllm/models/chatglm/__init__.py` & `openllm-0.1.8/src/openllm/models/chatglm/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.7/src/openllm/models/chatglm/configuration_chatglm.py` & `openllm-0.1.8/src/openllm/models/chatglm/configuration_chatglm.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.7/src/openllm/models/chatglm/modeling_chatglm.py` & `openllm-0.1.8/src/openllm/models/chatglm/modeling_chatglm.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.7/src/openllm/models/dolly_v2/__init__.py` & `openllm-0.1.8/src/openllm/models/dolly_v2/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.7/src/openllm/models/dolly_v2/configuration_dolly_v2.py` & `openllm-0.1.8/src/openllm/models/dolly_v2/configuration_dolly_v2.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.7/src/openllm/models/dolly_v2/modeling_dolly_v2.py` & `openllm-0.1.8/src/openllm/models/dolly_v2/modeling_dolly_v2.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.7/src/openllm/models/falcon/__init__.py` & `openllm-0.1.8/src/openllm/models/falcon/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.7/src/openllm/models/falcon/configuration_falcon.py` & `openllm-0.1.8/src/openllm/models/falcon/configuration_falcon.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.7/src/openllm/models/falcon/modeling_falcon.py` & `openllm-0.1.8/src/openllm/models/falcon/modeling_falcon.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.7/src/openllm/models/flan_t5/__init__.py` & `openllm-0.1.8/src/openllm/models/flan_t5/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.7/src/openllm/models/flan_t5/configuration_flan_t5.py` & `openllm-0.1.8/src/openllm/models/flan_t5/configuration_flan_t5.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.7/src/openllm/models/flan_t5/modeling_flan_t5.py` & `openllm-0.1.8/src/openllm/models/flan_t5/modeling_flan_t5.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.7/src/openllm/models/flan_t5/modeling_flax_flan_t5.py` & `openllm-0.1.8/src/openllm/models/flan_t5/modeling_flax_flan_t5.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.7/src/openllm/models/flan_t5/modeling_tf_flan_t5.py` & `openllm-0.1.8/src/openllm/models/flan_t5/modeling_tf_flan_t5.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.7/src/openllm/models/gpt_neox/__init__.py` & `openllm-0.1.8/src/openllm/models/gpt_neox/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.7/src/openllm/models/llama/__init__.py` & `openllm-0.1.8/src/openllm/models/llama/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.7/src/openllm/models/opt/__init__.py` & `openllm-0.1.8/src/openllm/models/opt/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.7/src/openllm/models/opt/configuration_opt.py` & `openllm-0.1.8/src/openllm/models/opt/configuration_opt.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.7/src/openllm/models/opt/modeling_flax_opt.py` & `openllm-0.1.8/src/openllm/models/opt/modeling_flax_opt.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.7/src/openllm/models/opt/modeling_opt.py` & `openllm-0.1.8/src/openllm/models/opt/modeling_opt.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.7/src/openllm/models/opt/modeling_tf_opt.py` & `openllm-0.1.8/src/openllm/models/opt/modeling_tf_opt.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.7/src/openllm/models/roberta/__init__.py` & `openllm-0.1.8/src/openllm/models/roberta/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.7/src/openllm/models/stablelm/__init__.py` & `openllm-0.1.8/src/openllm/models/stablelm/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.7/src/openllm/models/stablelm/configuration_stablelm.py` & `openllm-0.1.8/src/openllm/models/stablelm/configuration_stablelm.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.7/src/openllm/models/stablelm/modeling_stablelm.py` & `openllm-0.1.8/src/openllm/models/stablelm/modeling_stablelm.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.7/src/openllm/models/starcoder/__init__.py` & `openllm-0.1.8/src/openllm/models/starcoder/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.7/src/openllm/models/starcoder/configuration_starcoder.py` & `openllm-0.1.8/src/openllm/models/starcoder/configuration_starcoder.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.7/src/openllm/models/starcoder/modeling_starcoder.py` & `openllm-0.1.8/src/openllm/models/starcoder/modeling_starcoder.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.7/src/openllm/playground/__init__.py` & `openllm-0.1.8/tests/_strategies/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.7/src/openllm/playground/features.py` & `openllm-0.1.8/src/openllm/playground/features.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.7/src/openllm/playground/ft_opt_lora.py` & `openllm-0.1.8/src/openllm/playground/ft_opt_lora.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.7/src/openllm/utils/__init__.py` & `openllm-0.1.8/src/openllm/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.7/src/openllm/utils/analytics.py` & `openllm-0.1.8/src/openllm/utils/analytics.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.7/src/openllm/utils/codegen.py` & `openllm-0.1.8/src/openllm/utils/codegen.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.7/src/openllm/utils/dantic.py` & `openllm-0.1.8/src/openllm/utils/dantic.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.7/src/openllm/utils/dummy_flax_objects.py` & `openllm-0.1.8/src/openllm/utils/dummy_flax_objects.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.7/src/openllm/utils/dummy_pt_and_cpm_kernels_objects.py` & `openllm-0.1.8/src/openllm/utils/dummy_pt_and_cpm_kernels_objects.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.7/src/openllm/utils/dummy_pt_and_einops_objects.py` & `openllm-0.1.8/src/openllm/utils/dummy_pt_and_einops_objects.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.7/src/openllm/utils/dummy_pt_objects.py` & `openllm-0.1.8/src/openllm/utils/dummy_pt_objects.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.7/src/openllm/utils/dummy_tf_objects.py` & `openllm-0.1.8/src/openllm/utils/dummy_tf_objects.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.7/src/openllm/utils/import_utils.py` & `openllm-0.1.8/src/openllm/utils/import_utils.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.7/src/openllm/utils/lazy.py` & `openllm-0.1.8/src/openllm/utils/lazy.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.7/src/openllm_client/__init__.py` & `openllm-0.1.8/src/openllm_client/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.7/src/openllm_client/_prompt.py` & `openllm-0.1.8/src/openllm_client/_prompt.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.7/src/openllm_client/runtimes/__init__.py` & `openllm-0.1.8/src/openllm_client/runtimes/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.7/src/openllm_client/runtimes/base.py` & `openllm-0.1.8/src/openllm_client/runtimes/base.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.7/src/openllm_client/runtimes/grpc.py` & `openllm-0.1.8/src/openllm_client/runtimes/grpc.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.7/src/openllm_client/runtimes/http.py` & `openllm-0.1.8/src/openllm_client/runtimes/http.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.7/tests/__init__.py` & `openllm-0.1.8/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.7/tests/test_configuration.py` & `openllm-0.1.8/tests/test_configuration.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.7/tests/_strategies/__init__.py` & `openllm-0.1.8/tests/models/flan_t5/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.7/tests/_strategies/_configuration.py` & `openllm-0.1.8/tests/_strategies/_configuration.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.7/tests/models/flan_t5/__init__.py` & `openllm-0.1.8/tests/models/opt/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.7/tests/models/flan_t5/test_modeling_flan_t5.py` & `openllm-0.1.8/tests/models/flan_t5/test_modeling_flan_t5.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.7/tests/models/opt/__init__.py` & `openllm-0.1.8/src/openllm/__about__.py`

 * *Files 20% similar despite different names*

```diff
@@ -7,7 +7,8 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+__version__ = "0.1.8"
```

### Comparing `openllm-0.1.7/tests/models/opt/test_modeling_opt.py` & `openllm-0.1.8/tests/models/opt/test_modeling_opt.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.7/tools/assert-model-table-latest` & `openllm-0.1.8/tools/assert-model-table-latest`

 * *Files identical despite different names*

### Comparing `openllm-0.1.7/tools/run-release-action` & `openllm-0.1.8/tools/run-release-action`

 * *Files identical despite different names*

### Comparing `openllm-0.1.7/tools/update-optional-dependencies.py` & `openllm-0.1.8/tools/update-optional-dependencies.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.7/tools/update-readme.py` & `openllm-0.1.8/tools/update-readme.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.7/typings/attr/__init__.pyi` & `openllm-0.1.8/typings/attr/__init__.pyi`

 * *Files identical despite different names*

### Comparing `openllm-0.1.7/typings/attr/exceptions.pyi` & `openllm-0.1.8/typings/attr/exceptions.pyi`

 * *Files identical despite different names*

### Comparing `openllm-0.1.7/typings/attr/setters.pyi` & `openllm-0.1.8/typings/attr/setters.pyi`

 * *Files identical despite different names*

### Comparing `openllm-0.1.7/typings/attr/validators.pyi` & `openllm-0.1.8/typings/attr/validators.pyi`

 * *Files identical despite different names*

### Comparing `openllm-0.1.7/typings/click_option_group/__init__.pyi` & `openllm-0.1.8/typings/click_option_group/__init__.pyi`

 * *Files identical despite different names*

### Comparing `openllm-0.1.7/typings/click_option_group/_core.pyi` & `openllm-0.1.8/typings/click_option_group/_core.pyi`

 * *Files identical despite different names*

### Comparing `openllm-0.1.7/typings/click_option_group/_decorators.pyi` & `openllm-0.1.8/typings/click_option_group/_decorators.pyi`

 * *Files identical despite different names*

### Comparing `openllm-0.1.7/typings/click_option_group/_helpers.pyi` & `openllm-0.1.8/typings/click_option_group/_helpers.pyi`

 * *Files identical despite different names*

### Comparing `openllm-0.1.7/typings/deepmerge/merger.pyi` & `openllm-0.1.8/typings/deepmerge/merger.pyi`

 * *Files identical despite different names*

### Comparing `openllm-0.1.7/typings/deepmerge/strategy/core.pyi` & `openllm-0.1.8/typings/deepmerge/strategy/core.pyi`

 * *Files identical despite different names*

### Comparing `openllm-0.1.7/typings/deepmerge/strategy/set.pyi` & `openllm-0.1.8/typings/deepmerge/strategy/set.pyi`

 * *Files identical despite different names*

### Comparing `openllm-0.1.7/.gitignore` & `openllm-0.1.8/.gitignore`

 * *Files identical despite different names*

### Comparing `openllm-0.1.7/LICENSE.md` & `openllm-0.1.8/LICENSE.md`

 * *Files identical despite different names*

### Comparing `openllm-0.1.7/README.md` & `openllm-0.1.8/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -70,19 +70,20 @@
 
   An open platform for operating large language models in production.
   Fine-tune, serve, deploy, and monitor any LLMs with ease.
 ```
 
 ### Starting an LLM Server
 
-To start an LLM server, use `openllm start`. For example, to start a `dolly-v2`
-server:
+To start an LLM server, use `openllm start`. For example, to start a
+[`OPT`](https://huggingface.co/docs/transformers/model_doc/opt) server, do the
+following:
 
 ```bash
-openllm start dolly-v2
+openllm start opt
 ```
 
 Following this, a Web UI will be accessible at http://localhost:3000 where you
 can experiment with the endpoints and sample input prompts.
 
 OpenLLM provides a built-in Python client, allowing you to interact with the
 model. In a different terminal window or a Jupyter notebook, create a client to
@@ -322,21 +323,21 @@
 prompt and returns a corresponding output string. This will allow you to plug
 and play any OpenLLM models with your existing ML workflow.
 
 ```python
 import bentoml
 import openllm
 
-model = "dolly-v2"
+model = "opt"
 
 llm_config = openllm.AutoConfig.for_model(model)
 llm_runner = openllm.Runner(model, llm_config=llm_config)
 
 svc = bentoml.Service(
-    name=f"llm-dolly-v2-service", runners=[llm_runner]
+    name=f"llm-opt-service", runners=[llm_runner]
 )
 
 @svc.api(input=Text(), output=Text())
 async def prompt(input_text: str) -> str:
     answer = await llm_runner.generate(input_text)
     return answer
 ```
```

#### html2text {}

```diff
@@ -35,32 +35,33 @@
 âââââââââââââââââââââââââ
 âââ âââ âââââââ âââ
 âââââââââââ
 ââââââââââââââââââââââââ
 âââ An open platform for operating large language models in production.
 Fine-tune, serve, deploy, and monitor any LLMs with ease. ``` ### Starting an
 LLM Server To start an LLM server, use `openllm start`. For example, to start a
-`dolly-v2` server: ```bash openllm start dolly-v2 ``` Following this, a Web UI
-will be accessible at http://localhost:3000 where you can experiment with the
-endpoints and sample input prompts. OpenLLM provides a built-in Python client,
-allowing you to interact with the model. In a different terminal window or a
-Jupyter notebook, create a client to start interacting with the model:
-```python >>> import openllm >>> client = openllm.client.HTTPClient('http://
-localhost:3000') >>> client.query('Explain to me the difference between
-"further" and "farther"') ``` You can also use the `openllm query` command to
-query the model from the terminal: ```bash export OPENLLM_ENDPOINT=http://
-localhost:3000 openllm query 'Explain to me the difference between "further"
-and "farther"' ``` Visit `http://localhost:3000/docs.json` for OpenLLM's API
-specification. Users can also specify different variants of the model to be
-served, by providing the `--model-id` argument, e.g.: ```bash openllm start
-flan-t5 --model-id google/flan-t5-large ``` Use the `openllm models` command to
-see the list of models and their variants supported in OpenLLM. ## ð§©
-Supported Models The following models are currently supported in OpenLLM. By
-default, OpenLLM doesn't include dependencies to run all models. The extra
-model-specific dependencies can be installed with the instructions below:
+[`OPT`](https://huggingface.co/docs/transformers/model_doc/opt) server, do the
+following: ```bash openllm start opt ``` Following this, a Web UI will be
+accessible at http://localhost:3000 where you can experiment with the endpoints
+and sample input prompts. OpenLLM provides a built-in Python client, allowing
+you to interact with the model. In a different terminal window or a Jupyter
+notebook, create a client to start interacting with the model: ```python >>>
+import openllm >>> client = openllm.client.HTTPClient('http://localhost:3000')
+>>> client.query('Explain to me the difference between "further" and
+"farther"') ``` You can also use the `openllm query` command to query the model
+from the terminal: ```bash export OPENLLM_ENDPOINT=http://localhost:3000
+openllm query 'Explain to me the difference between "further" and "farther"'
+``` Visit `http://localhost:3000/docs.json` for OpenLLM's API specification.
+Users can also specify different variants of the model to be served, by
+providing the `--model-id` argument, e.g.: ```bash openllm start flan-t5 --
+model-id google/flan-t5-large ``` Use the `openllm models` command to see the
+list of models and their variants supported in OpenLLM. ## ð§© Supported
+Models The following models are currently supported in OpenLLM. By default,
+OpenLLM doesn't include dependencies to run all models. The extra model-
+specific dependencies can be installed with the instructions below:
 Model     CPU GPU Installation                 Model Ids
                                                    * google/flan-t5-small
                   ```bash pip install "openllm     * google/flan-t5-base
 flan-t5   ââ[flan-t5]" ```                   * google/flan-t5-large
                                                    * google/flan-t5-xl
                                                    * google/flan-t5-xxl
                   ```bash pip install openllm      * databricks/dolly-v2-3b
@@ -109,17 +110,17 @@
 We currently offer integration with [BentoML](https://github.com/bentoml/
 BentoML) and [LangChain](https://github.com/hwchase17/langchain). ### BentoML
 OpenLLM models can be integrated as a [Runner](https://docs.bentoml.org/en/
 latest/concepts/runner.html) in your BentoML service. These runners have a
 `generate` method that takes a string as a prompt and returns a corresponding
 output string. This will allow you to plug and play any OpenLLM models with
 your existing ML workflow. ```python import bentoml import openllm model =
-"dolly-v2" llm_config = openllm.AutoConfig.for_model(model) llm_runner =
+"opt" llm_config = openllm.AutoConfig.for_model(model) llm_runner =
 openllm.Runner(model, llm_config=llm_config) svc = bentoml.Service( name=f"llm-
-dolly-v2-service", runners=[llm_runner] ) @svc.api(input=Text(), output=Text())
+opt-service", runners=[llm_runner] ) @svc.api(input=Text(), output=Text())
 async def prompt(input_text: str) -> str: answer = await llm_runner.generate
 (input_text) return answer ``` ### HuggingFace Agents OpenLLM seamlessly
 integrates with HuggingFace Agents. > **Warning** The HuggingFace Agent is
 still at experimental stage. It is > recommended to OpenLLM with > `pip install
 -r nightly-requirements.generated.txt` to get the latest API > update for
 HuggingFace agent. ```python import transformers agent = transformers.HfAgent
 ("http://localhost:3000/hf/agent") # URL that runs the OpenLLM server agent.run
```

### Comparing `openllm-0.1.7/hatch.toml` & `openllm-0.1.8/hatch.toml`

 * *Files identical despite different names*

### Comparing `openllm-0.1.7/pyproject.toml` & `openllm-0.1.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `openllm-0.1.7/PKG-INFO` & `openllm-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openllm
-Version: 0.1.7
+Version: 0.1.8
 Summary: OpenLLM: REST/gRPC API server for running any open Large-Language Model - StableLM, Llama, Alpaca, Dolly, Flan-T5, Custom
 Project-URL: Documentation, https://github.com/bentoml/openllm#readme
 Project-URL: Issues, https://github.com/bentoml/openllm/issues
 Project-URL: Source, https://github.com/bentoml/openllm
 Author-email: Aaron Pham <aarnphm@bentoml.com>
 License-Expression: Apache-2.0
 License-File: LICENSE.md
@@ -144,19 +144,20 @@
 
   An open platform for operating large language models in production.
   Fine-tune, serve, deploy, and monitor any LLMs with ease.
 ```
 
 ### Starting an LLM Server
 
-To start an LLM server, use `openllm start`. For example, to start a `dolly-v2`
-server:
+To start an LLM server, use `openllm start`. For example, to start a
+[`OPT`](https://huggingface.co/docs/transformers/model_doc/opt) server, do the
+following:
 
 ```bash
-openllm start dolly-v2
+openllm start opt
 ```
 
 Following this, a Web UI will be accessible at http://localhost:3000 where you
 can experiment with the endpoints and sample input prompts.
 
 OpenLLM provides a built-in Python client, allowing you to interact with the
 model. In a different terminal window or a Jupyter notebook, create a client to
@@ -396,21 +397,21 @@
 prompt and returns a corresponding output string. This will allow you to plug
 and play any OpenLLM models with your existing ML workflow.
 
 ```python
 import bentoml
 import openllm
 
-model = "dolly-v2"
+model = "opt"
 
 llm_config = openllm.AutoConfig.for_model(model)
 llm_runner = openllm.Runner(model, llm_config=llm_config)
 
 svc = bentoml.Service(
-    name=f"llm-dolly-v2-service", runners=[llm_runner]
+    name=f"llm-opt-service", runners=[llm_runner]
 )
 
 @svc.api(input=Text(), output=Text())
 async def prompt(input_text: str) -> str:
     answer = await llm_runner.generate(input_text)
     return answer
 ```
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: openllm Version: 0.1.7 Summary: OpenLLM: REST/gRPC
+Metadata-Version: 2.1 Name: openllm Version: 0.1.8 Summary: OpenLLM: REST/gRPC
 API server for running any open Large-Language Model - StableLM, Llama, Alpaca,
 Dolly, Flan-T5, Custom Project-URL: Documentation, https://github.com/bentoml/
 openllm#readme Project-URL: Issues, https://github.com/bentoml/openllm/issues
 Project-URL: Source, https://github.com/bentoml/openllm Author-email: Aaron
 Pham
 bentoml.com> License-Expression: Apache-2.0 License-File: LICENSE.md Keywords:
 AI,Alpaca,BentoML,Generative AI,LLMOps,Large Language Model,MLOps,Model
@@ -79,32 +79,33 @@
 âââââââââââââââââââââââââ
 âââ âââ âââââââ âââ
 âââââââââââ
 ââââââââââââââââââââââââ
 âââ An open platform for operating large language models in production.
 Fine-tune, serve, deploy, and monitor any LLMs with ease. ``` ### Starting an
 LLM Server To start an LLM server, use `openllm start`. For example, to start a
-`dolly-v2` server: ```bash openllm start dolly-v2 ``` Following this, a Web UI
-will be accessible at http://localhost:3000 where you can experiment with the
-endpoints and sample input prompts. OpenLLM provides a built-in Python client,
-allowing you to interact with the model. In a different terminal window or a
-Jupyter notebook, create a client to start interacting with the model:
-```python >>> import openllm >>> client = openllm.client.HTTPClient('http://
-localhost:3000') >>> client.query('Explain to me the difference between
-"further" and "farther"') ``` You can also use the `openllm query` command to
-query the model from the terminal: ```bash export OPENLLM_ENDPOINT=http://
-localhost:3000 openllm query 'Explain to me the difference between "further"
-and "farther"' ``` Visit `http://localhost:3000/docs.json` for OpenLLM's API
-specification. Users can also specify different variants of the model to be
-served, by providing the `--model-id` argument, e.g.: ```bash openllm start
-flan-t5 --model-id google/flan-t5-large ``` Use the `openllm models` command to
-see the list of models and their variants supported in OpenLLM. ## ð§©
-Supported Models The following models are currently supported in OpenLLM. By
-default, OpenLLM doesn't include dependencies to run all models. The extra
-model-specific dependencies can be installed with the instructions below:
+[`OPT`](https://huggingface.co/docs/transformers/model_doc/opt) server, do the
+following: ```bash openllm start opt ``` Following this, a Web UI will be
+accessible at http://localhost:3000 where you can experiment with the endpoints
+and sample input prompts. OpenLLM provides a built-in Python client, allowing
+you to interact with the model. In a different terminal window or a Jupyter
+notebook, create a client to start interacting with the model: ```python >>>
+import openllm >>> client = openllm.client.HTTPClient('http://localhost:3000')
+>>> client.query('Explain to me the difference between "further" and
+"farther"') ``` You can also use the `openllm query` command to query the model
+from the terminal: ```bash export OPENLLM_ENDPOINT=http://localhost:3000
+openllm query 'Explain to me the difference between "further" and "farther"'
+``` Visit `http://localhost:3000/docs.json` for OpenLLM's API specification.
+Users can also specify different variants of the model to be served, by
+providing the `--model-id` argument, e.g.: ```bash openllm start flan-t5 --
+model-id google/flan-t5-large ``` Use the `openllm models` command to see the
+list of models and their variants supported in OpenLLM. ## ð§© Supported
+Models The following models are currently supported in OpenLLM. By default,
+OpenLLM doesn't include dependencies to run all models. The extra model-
+specific dependencies can be installed with the instructions below:
 Model     CPU GPU Installation                 Model Ids
                                                    * google/flan-t5-small
                   ```bash pip install "openllm     * google/flan-t5-base
 flan-t5   ââ[flan-t5]" ```                   * google/flan-t5-large
                                                    * google/flan-t5-xl
                                                    * google/flan-t5-xxl
                   ```bash pip install openllm      * databricks/dolly-v2-3b
@@ -153,17 +154,17 @@
 We currently offer integration with [BentoML](https://github.com/bentoml/
 BentoML) and [LangChain](https://github.com/hwchase17/langchain). ### BentoML
 OpenLLM models can be integrated as a [Runner](https://docs.bentoml.org/en/
 latest/concepts/runner.html) in your BentoML service. These runners have a
 `generate` method that takes a string as a prompt and returns a corresponding
 output string. This will allow you to plug and play any OpenLLM models with
 your existing ML workflow. ```python import bentoml import openllm model =
-"dolly-v2" llm_config = openllm.AutoConfig.for_model(model) llm_runner =
+"opt" llm_config = openllm.AutoConfig.for_model(model) llm_runner =
 openllm.Runner(model, llm_config=llm_config) svc = bentoml.Service( name=f"llm-
-dolly-v2-service", runners=[llm_runner] ) @svc.api(input=Text(), output=Text())
+opt-service", runners=[llm_runner] ) @svc.api(input=Text(), output=Text())
 async def prompt(input_text: str) -> str: answer = await llm_runner.generate
 (input_text) return answer ``` ### HuggingFace Agents OpenLLM seamlessly
 integrates with HuggingFace Agents. > **Warning** The HuggingFace Agent is
 still at experimental stage. It is > recommended to OpenLLM with > `pip install
 -r nightly-requirements.generated.txt` to get the latest API > update for
 HuggingFace agent. ```python import transformers agent = transformers.HfAgent
 ("http://localhost:3000/hf/agent") # URL that runs the OpenLLM server agent.run
```

