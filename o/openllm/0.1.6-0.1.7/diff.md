# Comparing `tmp/openllm-0.1.6.tar.gz` & `tmp/openllm-0.1.7.tar.gz`

## Comparing `openllm-0.1.6.tar` & `openllm-0.1.7.tar`

### file list

```diff
@@ -1,145 +1,149 @@
--rw-r--r--   0        0        0     2171 2020-02-02 00:00:00.000000 openllm-0.1.6/.pre-commit-config.yaml
--rw-r--r--   0        0        0     2938 2020-02-02 00:00:00.000000 openllm-0.1.6/ADDING_NEW_MODEL.md
--rw-r--r--   0        0        0     2116 2020-02-02 00:00:00.000000 openllm-0.1.6/CHANGELOG.md
--rw-r--r--   0        0        0     6492 2020-02-02 00:00:00.000000 openllm-0.1.6/DEVELOPMENT.md
--rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 openllm-0.1.6/package.json
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 openllm-0.1.6/taplo.toml
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 openllm-0.1.6/.github/CODEOWNERS
--rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 openllm-0.1.6/.github/SECURITY.md
--rw-r--r--   0        0        0      953 2020-02-02 00:00:00.000000 openllm-0.1.6/.github/dependabot.yml
--rw-r--r--   0        0        0     2765 2020-02-02 00:00:00.000000 openllm-0.1.6/.github/ISSUE_TEMPLATE/bug_report.yml
--rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 openllm-0.1.6/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 openllm-0.1.6/.github/ISSUE_TEMPLATE/feature_request.yml
--rwxr-xr-x   0        0        0     1428 2020-02-02 00:00:00.000000 openllm-0.1.6/.github/actions/create_release_and_archive.sh
--rwxr-xr-x   0        0        0     1853 2020-02-02 00:00:00.000000 openllm-0.1.6/.github/actions/release.sh
--rw-r--r--   0        0        0     2097 2020-02-02 00:00:00.000000 openllm-0.1.6/.github/actions/setup-repo/action.yml
--rw-r--r--   0        0        0     1571 2020-02-02 00:00:00.000000 openllm-0.1.6/.github/workflows/ci.yml
--rw-r--r--   0        0        0     2061 2020-02-02 00:00:00.000000 openllm-0.1.6/.github/workflows/create-releases.yml
--rw-r--r--   0        0        0     3502 2020-02-02 00:00:00.000000 openllm-0.1.6/.github/workflows/release-notes.yml
--rw-r--r--   0        0        0  1549838 2020-02-02 00:00:00.000000 openllm-0.1.6/assets/output.gif
--rw-r--r--   0        0        0      880 2020-02-02 00:00:00.000000 openllm-0.1.6/changelog.d/template.md.jinja
--rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 openllm-0.1.6/examples/bentoml-demo/bentofile.yaml
--rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 openllm-0.1.6/examples/bentoml-demo/service.py
--rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 openllm-0.1.6/examples/langchain-chains-demo/README.md
--rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 openllm-0.1.6/examples/langchain-chains-demo/bentofile.yaml
--rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 openllm-0.1.6/examples/langchain-chains-demo/download_model.py
--rw-r--r--   0        0        0     2230 2020-02-02 00:00:00.000000 openllm-0.1.6/examples/langchain-chains-demo/service.py
--rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 openllm-0.1.6/examples/langchain-tools-demo/README.md
--rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 openllm-0.1.6/examples/langchain-tools-demo/bentofile.yaml
--rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 openllm-0.1.6/examples/langchain-tools-demo/bentoml_configuration.yaml
--rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 openllm-0.1.6/examples/langchain-tools-demo/download_model.py
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 openllm-0.1.6/examples/langchain-tools-demo/requirements.txt
--rw-r--r--   0        0        0     1271 2020-02-02 00:00:00.000000 openllm-0.1.6/examples/langchain-tools-demo/service.py
--rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 openllm-0.1.6/src/openllm/__about__.py
--rw-r--r--   0        0        0     8880 2020-02-02 00:00:00.000000 openllm-0.1.6/src/openllm/__init__.py
--rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 openllm-0.1.6/src/openllm/__main__.py
--rw-r--r--   0        0        0    55304 2020-02-02 00:00:00.000000 openllm-0.1.6/src/openllm/_configuration.py
--rw-r--r--   0        0        0    42241 2020-02-02 00:00:00.000000 openllm-0.1.6/src/openllm/_llm.py
--rw-r--r--   0        0        0    12907 2020-02-02 00:00:00.000000 openllm-0.1.6/src/openllm/_package.py
--rw-r--r--   0        0        0     1636 2020-02-02 00:00:00.000000 openllm-0.1.6/src/openllm/_prompt.py
--rw-r--r--   0        0        0     2772 2020-02-02 00:00:00.000000 openllm-0.1.6/src/openllm/_schema.py
--rw-r--r--   0        0        0     2667 2020-02-02 00:00:00.000000 openllm-0.1.6/src/openllm/_service.py
--rw-r--r--   0        0        0     1459 2020-02-02 00:00:00.000000 openllm-0.1.6/src/openllm/_types.py
--rw-r--r--   0        0        0    43661 2020-02-02 00:00:00.000000 openllm-0.1.6/src/openllm/cli.py
--rw-r--r--   0        0        0     1881 2020-02-02 00:00:00.000000 openllm-0.1.6/src/openllm/client.py
--rw-r--r--   0        0        0     1390 2020-02-02 00:00:00.000000 openllm-0.1.6/src/openllm/exceptions.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openllm-0.1.6/src/openllm/py.typed
--rw-r--r--   0        0        0      855 2020-02-02 00:00:00.000000 openllm-0.1.6/src/openllm/models/__init__.py
--rw-r--r--   0        0        0     3366 2020-02-02 00:00:00.000000 openllm-0.1.6/src/openllm/models/auto/__init__.py
--rw-r--r--   0        0        0     4940 2020-02-02 00:00:00.000000 openllm-0.1.6/src/openllm/models/auto/configuration_auto.py
--rw-r--r--   0        0        0    12569 2020-02-02 00:00:00.000000 openllm-0.1.6/src/openllm/models/auto/factory.py
--rw-r--r--   0        0        0     1408 2020-02-02 00:00:00.000000 openllm-0.1.6/src/openllm/models/auto/modeling_auto.py
--rw-r--r--   0        0        0     1279 2020-02-02 00:00:00.000000 openllm-0.1.6/src/openllm/models/auto/modeling_flax_auto.py
--rw-r--r--   0        0        0     1263 2020-02-02 00:00:00.000000 openllm-0.1.6/src/openllm/models/auto/modeling_tf_auto.py
--rw-r--r--   0        0        0     1836 2020-02-02 00:00:00.000000 openllm-0.1.6/src/openllm/models/chatglm/__init__.py
--rw-r--r--   0        0        0     3071 2020-02-02 00:00:00.000000 openllm-0.1.6/src/openllm/models/chatglm/configuration_chatglm.py
--rw-r--r--   0        0        0     4783 2020-02-02 00:00:00.000000 openllm-0.1.6/src/openllm/models/chatglm/modeling_chatglm.py
--rw-r--r--   0        0        0     1749 2020-02-02 00:00:00.000000 openllm-0.1.6/src/openllm/models/dolly_v2/__init__.py
--rw-r--r--   0        0        0     3597 2020-02-02 00:00:00.000000 openllm-0.1.6/src/openllm/models/dolly_v2/configuration_dolly_v2.py
--rw-r--r--   0        0        0     4082 2020-02-02 00:00:00.000000 openllm-0.1.6/src/openllm/models/dolly_v2/modeling_dolly_v2.py
--rw-r--r--   0        0        0     1725 2020-02-02 00:00:00.000000 openllm-0.1.6/src/openllm/models/falcon/__init__.py
--rw-r--r--   0        0        0     2500 2020-02-02 00:00:00.000000 openllm-0.1.6/src/openllm/models/falcon/configuration_falcon.py
--rw-r--r--   0        0        0     5353 2020-02-02 00:00:00.000000 openllm-0.1.6/src/openllm/models/falcon/modeling_falcon.py
--rw-r--r--   0        0        0     2725 2020-02-02 00:00:00.000000 openllm-0.1.6/src/openllm/models/flan_t5/__init__.py
--rw-r--r--   0        0        0     2546 2020-02-02 00:00:00.000000 openllm-0.1.6/src/openllm/models/flan_t5/configuration_flan_t5.py
--rw-r--r--   0        0        0     3557 2020-02-02 00:00:00.000000 openllm-0.1.6/src/openllm/models/flan_t5/modeling_flan_t5.py
--rw-r--r--   0        0        0     3749 2020-02-02 00:00:00.000000 openllm-0.1.6/src/openllm/models/flan_t5/modeling_flax_flan_t5.py
--rw-r--r--   0        0        0     2853 2020-02-02 00:00:00.000000 openllm-0.1.6/src/openllm/models/flan_t5/modeling_tf_flan_t5.py
--rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 openllm-0.1.6/src/openllm/models/gpt_neox/__init__.py
--rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 openllm-0.1.6/src/openllm/models/llama/__init__.py
--rw-r--r--   0        0        0     2637 2020-02-02 00:00:00.000000 openllm-0.1.6/src/openllm/models/opt/__init__.py
--rw-r--r--   0        0        0     3067 2020-02-02 00:00:00.000000 openllm-0.1.6/src/openllm/models/opt/configuration_opt.py
--rw-r--r--   0        0        0     4733 2020-02-02 00:00:00.000000 openllm-0.1.6/src/openllm/models/opt/modeling_flax_opt.py
--rw-r--r--   0        0        0     5941 2020-02-02 00:00:00.000000 openllm-0.1.6/src/openllm/models/opt/modeling_opt.py
--rw-r--r--   0        0        0     4615 2020-02-02 00:00:00.000000 openllm-0.1.6/src/openllm/models/opt/modeling_tf_opt.py
--rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 openllm-0.1.6/src/openllm/models/roberta/__init__.py
--rw-r--r--   0        0        0     1755 2020-02-02 00:00:00.000000 openllm-0.1.6/src/openllm/models/stablelm/__init__.py
--rw-r--r--   0        0        0     3273 2020-02-02 00:00:00.000000 openllm-0.1.6/src/openllm/models/stablelm/configuration_stablelm.py
--rw-r--r--   0        0        0     4165 2020-02-02 00:00:00.000000 openllm-0.1.6/src/openllm/models/stablelm/modeling_stablelm.py
--rw-r--r--   0        0        0     1770 2020-02-02 00:00:00.000000 openllm-0.1.6/src/openllm/models/starcoder/__init__.py
--rw-r--r--   0        0        0     2566 2020-02-02 00:00:00.000000 openllm-0.1.6/src/openllm/models/starcoder/configuration_starcoder.py
--rw-r--r--   0        0        0     5285 2020-02-02 00:00:00.000000 openllm-0.1.6/src/openllm/models/starcoder/modeling_starcoder.py
--rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 openllm-0.1.6/src/openllm/playground/README
--rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 openllm-0.1.6/src/openllm/playground/__init__.py
--rw-r--r--   0        0        0     2194 2020-02-02 00:00:00.000000 openllm-0.1.6/src/openllm/playground/features.py
--rw-r--r--   0        0        0     4064 2020-02-02 00:00:00.000000 openllm-0.1.6/src/openllm/playground/ft_opt_lora.py
--rw-r--r--   0        0        0     5946 2020-02-02 00:00:00.000000 openllm-0.1.6/src/openllm/utils/__init__.py
--rw-r--r--   0        0        0     2754 2020-02-02 00:00:00.000000 openllm-0.1.6/src/openllm/utils/analytics.py
--rw-r--r--   0        0        0     5514 2020-02-02 00:00:00.000000 openllm-0.1.6/src/openllm/utils/codegen.py
--rw-r--r--   0        0        0    15415 2020-02-02 00:00:00.000000 openllm-0.1.6/src/openllm/utils/dantic.py
--rw-r--r--   0        0        0     1235 2020-02-02 00:00:00.000000 openllm-0.1.6/src/openllm/utils/dummy_flax_objects.py
--rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 openllm-0.1.6/src/openllm/utils/dummy_pt_and_cpm_kernels_objects.py
--rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 openllm-0.1.6/src/openllm/utils/dummy_pt_and_einops_objects.py
--rw-r--r--   0        0        0     1725 2020-02-02 00:00:00.000000 openllm-0.1.6/src/openllm/utils/dummy_pt_objects.py
--rw-r--r--   0        0        0     1215 2020-02-02 00:00:00.000000 openllm-0.1.6/src/openllm/utils/dummy_tf_objects.py
--rw-r--r--   0        0        0    11733 2020-02-02 00:00:00.000000 openllm-0.1.6/src/openllm/utils/import_utils.py
--rw-r--r--   0        0        0     5076 2020-02-02 00:00:00.000000 openllm-0.1.6/src/openllm/utils/lazy.py
--rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 openllm-0.1.6/src/openllm_client/__init__.py
--rw-r--r--   0        0        0     2273 2020-02-02 00:00:00.000000 openllm-0.1.6/src/openllm_client/_prompt.py
--rw-r--r--   0        0        0      685 2020-02-02 00:00:00.000000 openllm-0.1.6/src/openllm_client/runtimes/__init__.py
--rw-r--r--   0        0        0     7366 2020-02-02 00:00:00.000000 openllm-0.1.6/src/openllm_client/runtimes/base.py
--rw-r--r--   0        0        0     3503 2020-02-02 00:00:00.000000 openllm-0.1.6/src/openllm_client/runtimes/grpc.py
--rw-r--r--   0        0        0     2886 2020-02-02 00:00:00.000000 openllm-0.1.6/src/openllm_client/runtimes/http.py
--rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 openllm-0.1.6/src/openllm_js/package.json
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 openllm-0.1.6/src/openllm_js/tsconfig.cjs.json
--rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 openllm-0.1.6/src/openllm_js/tsconfig.json
--rw-r--r--   0        0        0      814 2020-02-02 00:00:00.000000 openllm-0.1.6/tests/__init__.py
--rw-r--r--   0        0        0     5566 2020-02-02 00:00:00.000000 openllm-0.1.6/tests/test_configuration.py
--rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 openllm-0.1.6/tests/_strategies/__init__.py
--rw-r--r--   0        0        0     3066 2020-02-02 00:00:00.000000 openllm-0.1.6/tests/_strategies/_configuration.py
--rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 openllm-0.1.6/tests/models/flan_t5/__init__.py
--rw-r--r--   0        0        0     1285 2020-02-02 00:00:00.000000 openllm-0.1.6/tests/models/flan_t5/test_modeling_flan_t5.py
--rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 openllm-0.1.6/tests/models/opt/__init__.py
--rw-r--r--   0        0        0     1216 2020-02-02 00:00:00.000000 openllm-0.1.6/tests/models/opt/test_modeling_opt.py
--rwxr-xr-x   0        0        0      489 2020-02-02 00:00:00.000000 openllm-0.1.6/tools/add-license-headers
--rwxr-xr-x   0        0        0      359 2020-02-02 00:00:00.000000 openllm-0.1.6/tools/assert-license-headers
--rwxr-xr-x   0        0        0      791 2020-02-02 00:00:00.000000 openllm-0.1.6/tools/assert-model-table-latest
--rwxr-xr-x   0        0        0     1901 2020-02-02 00:00:00.000000 openllm-0.1.6/tools/run-release-action
--rwxr-xr-x   0        0        0     2054 2020-02-02 00:00:00.000000 openllm-0.1.6/tools/update-optional-dependencies.py
--rwxr-xr-x   0        0        0     3575 2020-02-02 00:00:00.000000 openllm-0.1.6/tools/update-readme.py
--rw-r--r--   0        0        0    15605 2020-02-02 00:00:00.000000 openllm-0.1.6/typings/attr/__init__.pyi
--rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 openllm-0.1.6/typings/attr/_cmp.pyi
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 openllm-0.1.6/typings/attr/_compat.pyi
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 openllm-0.1.6/typings/attr/_typing_compat.pyi
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 openllm-0.1.6/typings/attr/_version_info.pyi
--rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 openllm-0.1.6/typings/attr/converters.pyi
--rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 openllm-0.1.6/typings/attr/exceptions.pyi
--rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 openllm-0.1.6/typings/attr/filters.pyi
--rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 openllm-0.1.6/typings/attr/setters.pyi
--rw-r--r--   0        0        0     2393 2020-02-02 00:00:00.000000 openllm-0.1.6/typings/attr/validators.pyi
--rw-r--r--   0        0        0      731 2020-02-02 00:00:00.000000 openllm-0.1.6/typings/click_option_group/__init__.pyi
--rw-r--r--   0        0        0     6084 2020-02-02 00:00:00.000000 openllm-0.1.6/typings/click_option_group/_core.pyi
--rw-r--r--   0        0        0     3451 2020-02-02 00:00:00.000000 openllm-0.1.6/typings/click_option_group/_decorators.pyi
--rw-r--r--   0        0        0      689 2020-02-02 00:00:00.000000 openllm-0.1.6/typings/click_option_group/_helpers.pyi
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 openllm-0.1.6/typings/click_option_group/_version.pyi
--rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 openllm-0.1.6/typings/deepmerge/__init__.pyi
--rw-r--r--   0        0        0      850 2020-02-02 00:00:00.000000 openllm-0.1.6/typings/deepmerge/merger.pyi
--rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 openllm-0.1.6/typings/deepmerge/strategy/core.pyi
--rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 openllm-0.1.6/typings/deepmerge/strategy/dict.pyi
--rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 openllm-0.1.6/typings/deepmerge/strategy/list.pyi
--rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 openllm-0.1.6/typings/deepmerge/strategy/set.pyi
--rw-r--r--   0        0        0     1858 2020-02-02 00:00:00.000000 openllm-0.1.6/.gitignore
--rw-r--r--   0        0        0    10470 2020-02-02 00:00:00.000000 openllm-0.1.6/LICENSE.md
--rw-r--r--   0        0        0    13859 2020-02-02 00:00:00.000000 openllm-0.1.6/README.md
--rw-r--r--   0        0        0     7146 2020-02-02 00:00:00.000000 openllm-0.1.6/pyproject.toml
--rw-r--r--   0        0        0    16980 2020-02-02 00:00:00.000000 openllm-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     2215 2020-02-02 00:00:00.000000 openllm-0.1.7/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     2938 2020-02-02 00:00:00.000000 openllm-0.1.7/ADDING_NEW_MODEL.md
+-rw-r--r--   0        0        0     3052 2020-02-02 00:00:00.000000 openllm-0.1.7/CHANGELOG.md
+-rw-r--r--   0        0        0     6496 2020-02-02 00:00:00.000000 openllm-0.1.7/DEVELOPMENT.md
+-rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 openllm-0.1.7/nightly-requirements.generated.txt
+-rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 openllm-0.1.7/package.json
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 openllm-0.1.7/taplo.toml
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 openllm-0.1.7/.github/CODEOWNERS
+-rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 openllm-0.1.7/.github/SECURITY.md
+-rw-r--r--   0        0        0      953 2020-02-02 00:00:00.000000 openllm-0.1.7/.github/dependabot.yml
+-rw-r--r--   0        0        0     2765 2020-02-02 00:00:00.000000 openllm-0.1.7/.github/ISSUE_TEMPLATE/bug_report.yml
+-rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 openllm-0.1.7/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 openllm-0.1.7/.github/ISSUE_TEMPLATE/feature_request.yml
+-rwxr-xr-x   0        0        0     1428 2020-02-02 00:00:00.000000 openllm-0.1.7/.github/actions/create_release_and_archive.sh
+-rwxr-xr-x   0        0        0     1853 2020-02-02 00:00:00.000000 openllm-0.1.7/.github/actions/release.sh
+-rw-r--r--   0        0        0     2081 2020-02-02 00:00:00.000000 openllm-0.1.7/.github/actions/setup-repo/action.yml
+-rw-r--r--   0        0        0     1487 2020-02-02 00:00:00.000000 openllm-0.1.7/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     2061 2020-02-02 00:00:00.000000 openllm-0.1.7/.github/workflows/create-releases.yml
+-rw-r--r--   0        0        0     3502 2020-02-02 00:00:00.000000 openllm-0.1.7/.github/workflows/release-notes.yml
+-rw-r--r--   0        0        0  1264669 2020-02-02 00:00:00.000000 openllm-0.1.7/assets/main-banner.png
+-rw-r--r--   0        0        0 10631249 2020-02-02 00:00:00.000000 openllm-0.1.7/assets/output.gif
+-rw-r--r--   0        0        0      881 2020-02-02 00:00:00.000000 openllm-0.1.7/changelog.d/template.md.jinja
+-rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 openllm-0.1.7/examples/bentoml-demo/bentofile.yaml
+-rw-r--r--   0        0        0     1002 2020-02-02 00:00:00.000000 openllm-0.1.7/examples/bentoml-demo/service.py
+-rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 openllm-0.1.7/examples/langchain-chains-demo/README.md
+-rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 openllm-0.1.7/examples/langchain-chains-demo/bentofile.yaml
+-rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 openllm-0.1.7/examples/langchain-chains-demo/download_model.py
+-rw-r--r--   0        0        0     2271 2020-02-02 00:00:00.000000 openllm-0.1.7/examples/langchain-chains-demo/service.py
+-rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 openllm-0.1.7/examples/langchain-tools-demo/README.md
+-rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 openllm-0.1.7/examples/langchain-tools-demo/bentofile.yaml
+-rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 openllm-0.1.7/examples/langchain-tools-demo/bentoml_configuration.yaml
+-rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 openllm-0.1.7/examples/langchain-tools-demo/download_model.py
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 openllm-0.1.7/examples/langchain-tools-demo/requirements.txt
+-rw-r--r--   0        0        0     1329 2020-02-02 00:00:00.000000 openllm-0.1.7/examples/langchain-tools-demo/service.py
+-rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 openllm-0.1.7/src/openllm/__about__.py
+-rw-r--r--   0        0        0     8872 2020-02-02 00:00:00.000000 openllm-0.1.7/src/openllm/__init__.py
+-rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 openllm-0.1.7/src/openllm/__main__.py
+-rw-r--r--   0        0        0    54358 2020-02-02 00:00:00.000000 openllm-0.1.7/src/openllm/_configuration.py
+-rw-r--r--   0        0        0     1637 2020-02-02 00:00:00.000000 openllm-0.1.7/src/openllm/_generation.py
+-rw-r--r--   0        0        0    43521 2020-02-02 00:00:00.000000 openllm-0.1.7/src/openllm/_llm.py
+-rw-r--r--   0        0        0    13551 2020-02-02 00:00:00.000000 openllm-0.1.7/src/openllm/_package.py
+-rw-r--r--   0        0        0     1636 2020-02-02 00:00:00.000000 openllm-0.1.7/src/openllm/_prompt.py
+-rw-r--r--   0        0        0     2773 2020-02-02 00:00:00.000000 openllm-0.1.7/src/openllm/_schema.py
+-rw-r--r--   0        0        0     3833 2020-02-02 00:00:00.000000 openllm-0.1.7/src/openllm/_service.py
+-rw-r--r--   0        0        0     1461 2020-02-02 00:00:00.000000 openllm-0.1.7/src/openllm/_types.py
+-rw-r--r--   0        0        0    48406 2020-02-02 00:00:00.000000 openllm-0.1.7/src/openllm/cli.py
+-rw-r--r--   0        0        0     1882 2020-02-02 00:00:00.000000 openllm-0.1.7/src/openllm/client.py
+-rw-r--r--   0        0        0     1390 2020-02-02 00:00:00.000000 openllm-0.1.7/src/openllm/exceptions.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openllm-0.1.7/src/openllm/py.typed
+-rw-r--r--   0        0        0      855 2020-02-02 00:00:00.000000 openllm-0.1.7/src/openllm/models/__init__.py
+-rw-r--r--   0        0        0     3367 2020-02-02 00:00:00.000000 openllm-0.1.7/src/openllm/models/auto/__init__.py
+-rw-r--r--   0        0        0     4995 2020-02-02 00:00:00.000000 openllm-0.1.7/src/openllm/models/auto/configuration_auto.py
+-rw-r--r--   0        0        0    12738 2020-02-02 00:00:00.000000 openllm-0.1.7/src/openllm/models/auto/factory.py
+-rw-r--r--   0        0        0     1428 2020-02-02 00:00:00.000000 openllm-0.1.7/src/openllm/models/auto/modeling_auto.py
+-rw-r--r--   0        0        0     1299 2020-02-02 00:00:00.000000 openllm-0.1.7/src/openllm/models/auto/modeling_flax_auto.py
+-rw-r--r--   0        0        0     1283 2020-02-02 00:00:00.000000 openllm-0.1.7/src/openllm/models/auto/modeling_tf_auto.py
+-rw-r--r--   0        0        0     1837 2020-02-02 00:00:00.000000 openllm-0.1.7/src/openllm/models/chatglm/__init__.py
+-rw-r--r--   0        0        0     3071 2020-02-02 00:00:00.000000 openllm-0.1.7/src/openllm/models/chatglm/configuration_chatglm.py
+-rw-r--r--   0        0        0     4783 2020-02-02 00:00:00.000000 openllm-0.1.7/src/openllm/models/chatglm/modeling_chatglm.py
+-rw-r--r--   0        0        0     1750 2020-02-02 00:00:00.000000 openllm-0.1.7/src/openllm/models/dolly_v2/__init__.py
+-rw-r--r--   0        0        0     3597 2020-02-02 00:00:00.000000 openllm-0.1.7/src/openllm/models/dolly_v2/configuration_dolly_v2.py
+-rw-r--r--   0        0        0     4091 2020-02-02 00:00:00.000000 openllm-0.1.7/src/openllm/models/dolly_v2/modeling_dolly_v2.py
+-rw-r--r--   0        0        0     1726 2020-02-02 00:00:00.000000 openllm-0.1.7/src/openllm/models/falcon/__init__.py
+-rw-r--r--   0        0        0     2500 2020-02-02 00:00:00.000000 openllm-0.1.7/src/openllm/models/falcon/configuration_falcon.py
+-rw-r--r--   0        0        0     5353 2020-02-02 00:00:00.000000 openllm-0.1.7/src/openllm/models/falcon/modeling_falcon.py
+-rw-r--r--   0        0        0     2726 2020-02-02 00:00:00.000000 openllm-0.1.7/src/openllm/models/flan_t5/__init__.py
+-rw-r--r--   0        0        0     2547 2020-02-02 00:00:00.000000 openllm-0.1.7/src/openllm/models/flan_t5/configuration_flan_t5.py
+-rw-r--r--   0        0        0     3559 2020-02-02 00:00:00.000000 openllm-0.1.7/src/openllm/models/flan_t5/modeling_flan_t5.py
+-rw-r--r--   0        0        0     3750 2020-02-02 00:00:00.000000 openllm-0.1.7/src/openllm/models/flan_t5/modeling_flax_flan_t5.py
+-rw-r--r--   0        0        0     2854 2020-02-02 00:00:00.000000 openllm-0.1.7/src/openllm/models/flan_t5/modeling_tf_flan_t5.py
+-rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 openllm-0.1.7/src/openllm/models/gpt_neox/__init__.py
+-rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 openllm-0.1.7/src/openllm/models/llama/__init__.py
+-rw-r--r--   0        0        0     2638 2020-02-02 00:00:00.000000 openllm-0.1.7/src/openllm/models/opt/__init__.py
+-rw-r--r--   0        0        0     3067 2020-02-02 00:00:00.000000 openllm-0.1.7/src/openllm/models/opt/configuration_opt.py
+-rw-r--r--   0        0        0     4733 2020-02-02 00:00:00.000000 openllm-0.1.7/src/openllm/models/opt/modeling_flax_opt.py
+-rw-r--r--   0        0        0     5942 2020-02-02 00:00:00.000000 openllm-0.1.7/src/openllm/models/opt/modeling_opt.py
+-rw-r--r--   0        0        0     4615 2020-02-02 00:00:00.000000 openllm-0.1.7/src/openllm/models/opt/modeling_tf_opt.py
+-rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 openllm-0.1.7/src/openllm/models/roberta/__init__.py
+-rw-r--r--   0        0        0     1756 2020-02-02 00:00:00.000000 openllm-0.1.7/src/openllm/models/stablelm/__init__.py
+-rw-r--r--   0        0        0     3273 2020-02-02 00:00:00.000000 openllm-0.1.7/src/openllm/models/stablelm/configuration_stablelm.py
+-rw-r--r--   0        0        0     4219 2020-02-02 00:00:00.000000 openllm-0.1.7/src/openllm/models/stablelm/modeling_stablelm.py
+-rw-r--r--   0        0        0     1771 2020-02-02 00:00:00.000000 openllm-0.1.7/src/openllm/models/starcoder/__init__.py
+-rw-r--r--   0        0        0     2566 2020-02-02 00:00:00.000000 openllm-0.1.7/src/openllm/models/starcoder/configuration_starcoder.py
+-rw-r--r--   0        0        0     6346 2020-02-02 00:00:00.000000 openllm-0.1.7/src/openllm/models/starcoder/modeling_starcoder.py
+-rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 openllm-0.1.7/src/openllm/playground/README
+-rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 openllm-0.1.7/src/openllm/playground/__init__.py
+-rw-r--r--   0        0        0     2195 2020-02-02 00:00:00.000000 openllm-0.1.7/src/openllm/playground/features.py
+-rw-r--r--   0        0        0     4099 2020-02-02 00:00:00.000000 openllm-0.1.7/src/openllm/playground/ft_opt_lora.py
+-rw-r--r--   0        0        0     7440 2020-02-02 00:00:00.000000 openllm-0.1.7/src/openllm/utils/__init__.py
+-rw-r--r--   0        0        0     2757 2020-02-02 00:00:00.000000 openllm-0.1.7/src/openllm/utils/analytics.py
+-rw-r--r--   0        0        0     5515 2020-02-02 00:00:00.000000 openllm-0.1.7/src/openllm/utils/codegen.py
+-rw-r--r--   0        0        0    15488 2020-02-02 00:00:00.000000 openllm-0.1.7/src/openllm/utils/dantic.py
+-rw-r--r--   0        0        0     1254 2020-02-02 00:00:00.000000 openllm-0.1.7/src/openllm/utils/dummy_flax_objects.py
+-rw-r--r--   0        0        0      923 2020-02-02 00:00:00.000000 openllm-0.1.7/src/openllm/utils/dummy_pt_and_cpm_kernels_objects.py
+-rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 openllm-0.1.7/src/openllm/utils/dummy_pt_and_einops_objects.py
+-rw-r--r--   0        0        0     1744 2020-02-02 00:00:00.000000 openllm-0.1.7/src/openllm/utils/dummy_pt_objects.py
+-rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 openllm-0.1.7/src/openllm/utils/dummy_tf_objects.py
+-rw-r--r--   0        0        0    12067 2020-02-02 00:00:00.000000 openllm-0.1.7/src/openllm/utils/import_utils.py
+-rw-r--r--   0        0        0     5190 2020-02-02 00:00:00.000000 openllm-0.1.7/src/openllm/utils/lazy.py
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 openllm-0.1.7/src/openllm_client/__init__.py
+-rw-r--r--   0        0        0     2274 2020-02-02 00:00:00.000000 openllm-0.1.7/src/openllm_client/_prompt.py
+-rw-r--r--   0        0        0      685 2020-02-02 00:00:00.000000 openllm-0.1.7/src/openllm_client/runtimes/__init__.py
+-rw-r--r--   0        0        0    11495 2020-02-02 00:00:00.000000 openllm-0.1.7/src/openllm_client/runtimes/base.py
+-rw-r--r--   0        0        0     3522 2020-02-02 00:00:00.000000 openllm-0.1.7/src/openllm_client/runtimes/grpc.py
+-rw-r--r--   0        0        0     2904 2020-02-02 00:00:00.000000 openllm-0.1.7/src/openllm_client/runtimes/http.py
+-rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 openllm-0.1.7/src/openllm_js/package.json
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 openllm-0.1.7/src/openllm_js/tsconfig.cjs.json
+-rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 openllm-0.1.7/src/openllm_js/tsconfig.json
+-rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 openllm-0.1.7/tests/__init__.py
+-rw-r--r--   0        0        0     5658 2020-02-02 00:00:00.000000 openllm-0.1.7/tests/test_configuration.py
+-rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 openllm-0.1.7/tests/_strategies/__init__.py
+-rw-r--r--   0        0        0     3094 2020-02-02 00:00:00.000000 openllm-0.1.7/tests/_strategies/_configuration.py
+-rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 openllm-0.1.7/tests/models/flan_t5/__init__.py
+-rw-r--r--   0        0        0     1308 2020-02-02 00:00:00.000000 openllm-0.1.7/tests/models/flan_t5/test_modeling_flan_t5.py
+-rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 openllm-0.1.7/tests/models/opt/__init__.py
+-rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 openllm-0.1.7/tests/models/opt/test_modeling_opt.py
+-rwxr-xr-x   0        0        0      489 2020-02-02 00:00:00.000000 openllm-0.1.7/tools/add-license-headers
+-rwxr-xr-x   0        0        0      359 2020-02-02 00:00:00.000000 openllm-0.1.7/tools/assert-license-headers
+-rwxr-xr-x   0        0        0      791 2020-02-02 00:00:00.000000 openllm-0.1.7/tools/assert-model-table-latest
+-rwxr-xr-x   0        0        0     1901 2020-02-02 00:00:00.000000 openllm-0.1.7/tools/run-release-action
+-rwxr-xr-x   0        0        0     5012 2020-02-02 00:00:00.000000 openllm-0.1.7/tools/update-optional-dependencies.py
+-rwxr-xr-x   0        0        0     3575 2020-02-02 00:00:00.000000 openllm-0.1.7/tools/update-readme.py
+-rw-r--r--   0        0        0    15821 2020-02-02 00:00:00.000000 openllm-0.1.7/typings/attr/__init__.pyi
+-rw-r--r--   0        0        0      435 2020-02-02 00:00:00.000000 openllm-0.1.7/typings/attr/_cmp.pyi
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 openllm-0.1.7/typings/attr/_compat.pyi
+-rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 openllm-0.1.7/typings/attr/_typing_compat.pyi
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 openllm-0.1.7/typings/attr/_version_info.pyi
+-rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 openllm-0.1.7/typings/attr/converters.pyi
+-rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 openllm-0.1.7/typings/attr/exceptions.pyi
+-rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 openllm-0.1.7/typings/attr/filters.pyi
+-rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 openllm-0.1.7/typings/attr/setters.pyi
+-rw-r--r--   0        0        0     2608 2020-02-02 00:00:00.000000 openllm-0.1.7/typings/attr/validators.pyi
+-rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 openllm-0.1.7/typings/click_option_group/__init__.pyi
+-rw-r--r--   0        0        0     6238 2020-02-02 00:00:00.000000 openllm-0.1.7/typings/click_option_group/_core.pyi
+-rw-r--r--   0        0        0     3691 2020-02-02 00:00:00.000000 openllm-0.1.7/typings/click_option_group/_decorators.pyi
+-rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 openllm-0.1.7/typings/click_option_group/_helpers.pyi
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 openllm-0.1.7/typings/click_option_group/_version.pyi
+-rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 openllm-0.1.7/typings/deepmerge/__init__.pyi
+-rw-r--r--   0        0        0      851 2020-02-02 00:00:00.000000 openllm-0.1.7/typings/deepmerge/merger.pyi
+-rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 openllm-0.1.7/typings/deepmerge/strategy/core.pyi
+-rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 openllm-0.1.7/typings/deepmerge/strategy/dict.pyi
+-rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 openllm-0.1.7/typings/deepmerge/strategy/list.pyi
+-rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 openllm-0.1.7/typings/deepmerge/strategy/set.pyi
+-rw-r--r--   0        0        0     1858 2020-02-02 00:00:00.000000 openllm-0.1.7/.gitignore
+-rw-r--r--   0        0        0    10470 2020-02-02 00:00:00.000000 openllm-0.1.7/LICENSE.md
+-rw-r--r--   0        0        0    14939 2020-02-02 00:00:00.000000 openllm-0.1.7/README.md
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 openllm-0.1.7/hatch.toml
+-rw-r--r--   0        0        0     5808 2020-02-02 00:00:00.000000 openllm-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0    18201 2020-02-02 00:00:00.000000 openllm-0.1.7/PKG-INFO
```

### Comparing `openllm-0.1.6/.pre-commit-config.yaml` & `openllm-0.1.7/.pre-commit-config.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -40,17 +40,19 @@
         name: check for license headers
         entry: ./tools/assert-license-headers
         language: script
         exclude_types:
           - 'markdown'
           - 'toml'
           - 'json'
+          - 'text'
         exclude: |
           (?x)^(
               tools/.*|
+              assets/.*|
               changelog.d/.*|
               typings/.*|
               .github/.*
           )$
       - id: check-models-table-update
         name: check if table in README.md is up-to-date
         entry: ./tools/assert-model-table-latest
```

### Comparing `openllm-0.1.6/ADDING_NEW_MODEL.md` & `openllm-0.1.7/ADDING_NEW_MODEL.md`

 * *Files identical despite different names*

### Comparing `openllm-0.1.6/DEVELOPMENT.md` & `openllm-0.1.7/DEVELOPMENT.md`

 * *Files 1% similar despite different names*

```diff
@@ -103,15 +103,15 @@
    hatch run fmt
    ```
 4. Write tests that verify your feature or fix (see
    [Writing Tests](#writing-tests) below).
 5. Run all tests to ensure your changes haven't broken anything:
 
    ```bash
-   hatch run test
+   hatch run test:p
    ```
 
 6. Commit your changes:
 
    ```bash
    git commit -m "Add my feature"
    ```
@@ -137,15 +137,15 @@
 
 We use `pytest` for our tests. Make sure your tests are in the `tests/`
 directory and their filenames start with `test_`.
 
 Run all tests with:
 
 ```bash
-hatch run test
+hatch run test:p
 ```
 
 ## Releasing a New Version
 
 To release a new version, use `./tools/run-release-action`. It requires `gh`,
 `jq` and `hatch`:
 
@@ -191,24 +191,23 @@
 - If you want to reference multiple issues, copy the news fragment to another
   filename. _Towncrier_ will merge all news fragments with identical contents
   into one entry with multiple links to the respective pull requests.
 
 Example entries:
 
 ```md
-Added `LLM.func()`.
-The feature really _is_ awesome.
+Added `LLM.func()`. The feature really _is_ awesome.
 ```
 
 or:
 
 ```md
-`openllm.utils.func()` now doesn't X.Y.Z anymore when passed the _foobar_ argument.
-The bug really _was_ nasty.
+`openllm.utils.func()` now doesn't X.Y.Z anymore when passed the _foobar_
+argument. The bug really _was_ nasty.
 ```
 
 ---
 
-`hatch run changelog` will render the current changelog to the terminal if you have
-any doubts.
+`hatch run changelog` will render the current changelog to the terminal if you
+have any doubts.
 
 [semantic newlines]: https://rhodesmill.org/brandon/2012/one-sentence-per-line/
```

### Comparing `openllm-0.1.6/package.json` & `openllm-0.1.7/package.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9545454545454546%*

 * *Differences: {"'version'": "'0.1.7'"}*

```diff
@@ -11,12 +11,12 @@
     "engines": {
         "node": ">=16"
     },
     "license": "Apache 2.0",
     "name": "openllm",
     "private": true,
     "repository": "git@github.com:llmsys/OpenLLM.git",
-    "version": "0.1.6",
+    "version": "0.1.7",
     "workspaces": [
         "src/openllm_js"
     ]
 }
```

### Comparing `openllm-0.1.6/.github/SECURITY.md` & `openllm-0.1.7/.github/SECURITY.md`

 * *Files identical despite different names*

### Comparing `openllm-0.1.6/.github/dependabot.yml` & `openllm-0.1.7/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `openllm-0.1.6/.github/ISSUE_TEMPLATE/bug_report.yml` & `openllm-0.1.7/.github/ISSUE_TEMPLATE/bug_report.yml`

 * *Files identical despite different names*

### Comparing `openllm-0.1.6/.github/ISSUE_TEMPLATE/config.yml` & `openllm-0.1.7/.github/ISSUE_TEMPLATE/config.yml`

 * *Files identical despite different names*

### Comparing `openllm-0.1.6/.github/ISSUE_TEMPLATE/feature_request.yml` & `openllm-0.1.7/.github/ISSUE_TEMPLATE/feature_request.yml`

 * *Files identical despite different names*

### Comparing `openllm-0.1.6/.github/actions/create_release_and_archive.sh` & `openllm-0.1.7/.github/actions/create_release_and_archive.sh`

 * *Files identical despite different names*

### Comparing `openllm-0.1.6/.github/actions/release.sh` & `openllm-0.1.7/.github/actions/release.sh`

 * *Files identical despite different names*

### Comparing `openllm-0.1.6/.github/actions/setup-repo/action.yml` & `openllm-0.1.7/.github/actions/setup-repo/action.yml`

 * *Files 4% similar despite different names*

```diff
@@ -49,15 +49,15 @@
       with:
         path: ${{ steps.pip-cache-dir.outputs.dir }}
         key: ${{ steps.get-cache-key-prefix.outputs.prefix }}-pypi
         restore-keys: |
           ${{ steps.get-cache-key-prefix.outputs.prefix }}-pypi-
     - name: Install dependencies
       shell: bash
-      run: pip install -e ".[all]" hatch towncrier -vv
+      run: pip install hatch towncrier
     - name: Install pyright
       shell: bash
       run: npm install -g npm@^7 pyright
     - name: Setup bufbuild/buf
       uses: bufbuild/buf-setup-action@v1.20.0
       with:
         github_token: ${{ github.token }}
```

### Comparing `openllm-0.1.6/.github/workflows/ci.yml` & `openllm-0.1.7/.github/workflows/ci.yml`

 * *Files 12% similar despite different names*

```diff
@@ -31,20 +31,19 @@
   tests:
     runs-on: ubuntu-latest
     if: ${{ github.event_name == 'pull_request' || github.event_name == 'push' }}
     strategy:
       fail-fast: false
       matrix:
         os: [ubuntu-latest, macos-latest]
-        python-version: ['3.8', '3.9', '3.10', '3.11']
-    name: tests (${{ matrix.os }}-${{ matrix.python-version }})
+    name: tests-${{ matrix.os }}
     steps:
       - uses: actions/checkout@v3
         with:
           fetch-depth: 0
       - name: Setup CI
         uses: ./.github/actions/setup-repo
       - name: Run tests
-        run: hatch run test
+        run: hatch run test:p
 concurrency:
   group: ci-${{ github.event.pull_request.number || github.sha }}
   cancel-in-progress: true
```

### Comparing `openllm-0.1.6/.github/workflows/create-releases.yml` & `openllm-0.1.7/.github/workflows/create-releases.yml`

 * *Files identical despite different names*

### Comparing `openllm-0.1.6/.github/workflows/release-notes.yml` & `openllm-0.1.7/.github/workflows/release-notes.yml`

 * *Files identical despite different names*

### Comparing `openllm-0.1.6/changelog.d/template.md.jinja` & `openllm-0.1.7/changelog.d/template.md.jinja`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 ## Changes for the Upcoming Release
 
 :::{warning}
 These changes reflect the current [development progress](https://github.com/bentoml/openllm/tree/main) and have **not** been part of a official PyPI release yet.
 To try out the latest change, one can do: `pip install -U git+https://github.com/bentoml/openllm.git@main`
 :::
 {% else -%}
-## [{{ versiondata["version"] }}](https://github.com/bentoml/openllm/tree/{{ versiondata["version"] }})
+## [{{ versiondata["version"] }}](https://github.com/bentoml/openllm/tree/v{{ versiondata["version"] }})
 {%- endif %}
 
 {% for section, _ in sections.items() %}
 {% if sections[section] %}
 {% for category, val in definitions.items() if category in sections[section] %}
 
 ### {{ definitions[category]['name'] }}
```

### Comparing `openllm-0.1.6/examples/bentoml-demo/bentofile.yaml` & `openllm-0.1.7/examples/bentoml-demo/bentofile.yaml`

 * *Files identical despite different names*

### Comparing `openllm-0.1.6/examples/bentoml-demo/service.py` & `openllm-0.1.7/examples/bentoml-demo/service.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import bentoml
 import openllm
 from bentoml.io import Text
 
+
 model = "dolly-v2"
 
 llm_config = openllm.AutoConfig.for_model(model)
 llm_runner = openllm.Runner(model, llm_config=llm_config)
 
 svc = bentoml.Service(name="llm-service", runners=[llm_runner])
```

### Comparing `openllm-0.1.6/examples/langchain-chains-demo/bentofile.yaml` & `openllm-0.1.7/examples/langchain-chains-demo/bentofile.yaml`

 * *Files identical despite different names*

### Comparing `openllm-0.1.6/examples/langchain-chains-demo/download_model.py` & `openllm-0.1.7/examples/langchain-chains-demo/download_model.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.6/examples/langchain-chains-demo/service.py` & `openllm-0.1.7/examples/langchain-chains-demo/service.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,22 +8,25 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from typing import Any, Dict
+from typing import Any
+from typing import Dict
 
-import bentoml
-from bentoml.io import Text, JSON
-from pydantic import BaseModel
-from langchain.prompts import PromptTemplate
 from langchain.chains import LLMChain
 from langchain.llms import OpenLLM
+from langchain.prompts import PromptTemplate
+from pydantic import BaseModel
+
+import bentoml
+from bentoml.io import JSON
+from bentoml.io import Text
 
 
 class Query(BaseModel):
     industry: str
     product_name: str
     keywords: list[str]
     llm_config: Dict[str, Any]
```

### Comparing `openllm-0.1.6/examples/langchain-tools-demo/bentofile.yaml` & `openllm-0.1.7/examples/langchain-tools-demo/bentofile.yaml`

 * *Files identical despite different names*

### Comparing `openllm-0.1.6/examples/langchain-tools-demo/bentoml_configuration.yaml` & `openllm-0.1.7/examples/langchain-tools-demo/bentoml_configuration.yaml`

 * *Files identical despite different names*

### Comparing `openllm-0.1.6/examples/langchain-tools-demo/download_model.py` & `openllm-0.1.7/examples/langchain-tools-demo/download_model.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.6/examples/langchain-tools-demo/service.py` & `openllm-0.1.7/examples/langchain-tools-demo/service.py`

 * *Files 11% similar despite different names*

```diff
@@ -8,18 +8,22 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+from langchain.agents import AgentType
+from langchain.agents import initialize_agent
+from langchain.agents import load_tools
+from langchain.llms import OpenLLM
+
 import bentoml
 from bentoml.io import Text
-from langchain.agents import AgentType, initialize_agent, load_tools
-from langchain.llms import OpenLLM
+
 
 SAMPLE_INPUT = "What is the weather in San Francisco?"
 
 llm = OpenLLM(
     model_name="dolly-v2",
     model_id="databricks/dolly-v2-7b",
     embedded=False,
```

### Comparing `openllm-0.1.6/src/openllm/__about__.py` & `openllm-0.1.7/src/openllm/models/gpt_neox/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,8 +7,9 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-__version__ = "0.1.6"
+
+raise NotImplementedError("This module is not implemented yet.")
```

### Comparing `openllm-0.1.6/src/openllm/__init__.py` & `openllm-0.1.7/src/openllm/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 import logging
 import typing as t
 
 from . import utils as utils
 from .__about__ import __version__ as __version__
 from .exceptions import MissingDependencyError
 
+
 if utils.DEBUG:
     utils.set_debug_mode(True)
     utils.set_quiet_mode(False)
 
     utils.configure_logging()
     logging.basicConfig(level=logging.NOTSET)
 
@@ -139,28 +140,28 @@
 # declaration for OpenLLM-related modules
 if t.TYPE_CHECKING:
     from . import cli as cli
     from . import client as client
     from . import exceptions as exceptions
     from . import models as models
     from . import playground as playground
+
     # Specific types import
     from ._configuration import LLMConfig as LLMConfig
     from ._llm import LLM as LLM
     from ._llm import LLMRunner as LLMRunner
     from ._llm import Runner as Runner
     from ._package import build as build
     from ._schema import GenerationInput as GenerationInput
     from ._schema import GenerationOutput as GenerationOutput
     from ._schema import MetadataOutput as MetadataOutput
     from .cli import start as start
     from .cli import start_grpc as start_grpc
     from .models.auto import CONFIG_MAPPING as CONFIG_MAPPING
-    from .models.auto import \
-        MODEL_FLAX_MAPPING_NAMES as MODEL_FLAX_MAPPING_NAMES
+    from .models.auto import MODEL_FLAX_MAPPING_NAMES as MODEL_FLAX_MAPPING_NAMES
     from .models.auto import MODEL_MAPPING_NAMES as MODEL_MAPPING_NAMES
     from .models.auto import MODEL_TF_MAPPING_NAMES as MODEL_TF_MAPPING_NAMES
     from .models.auto import AutoConfig as AutoConfig
     from .models.chatglm import ChatGLMConfig as ChatGLMConfig
     from .models.dolly_v2 import DollyV2Config as DollyV2Config
     from .models.falcon import FalconConfig as FalconConfig
     from .models.flan_t5 import FlanT5Config as FlanT5Config
```

### Comparing `openllm-0.1.6/src/openllm/__main__.py` & `openllm-0.1.7/src/openllm/__main__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.6/src/openllm/_configuration.py` & `openllm-0.1.7/src/openllm/_configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,24 +56,31 @@
 import typing as t
 from operator import itemgetter
 
 import attr
 import click_option_group as cog
 import inflection
 import orjson
-from cattr.gen import make_dict_unstructure_fn, override
+from cattr.gen import make_dict_unstructure_fn
+from cattr.gen import override
 from deepmerge.merger import Merger
 
 import openllm
 
-from .exceptions import (ForbiddenAttributeError, GpuNotAvailableError,
-                         OpenLLMException)
-from .utils import (DEBUG, ENV_VARS_TRUE_VALUES, LazyType, bentoml_cattr,
-                    codegen, dantic, first_not_none, lenient_issubclass,
-                    non_intrusive_setattr)
+from .exceptions import ForbiddenAttributeError
+from .utils import DEBUG
+from .utils import ENV_VARS_TRUE_VALUES
+from .utils import LazyType
+from .utils import bentoml_cattr
+from .utils import codegen
+from .utils import dantic
+from .utils import first_not_none
+from .utils import lenient_issubclass
+from .utils import non_intrusive_setattr
+
 
 if hasattr(t, "Required"):
     from typing import Required
 else:
     from typing_extensions import Required
 
 if hasattr(t, "NotRequired"):
@@ -86,42 +93,46 @@
 else:
     from typing_extensions import dataclass_transform
 
 _T = t.TypeVar("_T")
 
 
 if t.TYPE_CHECKING:
-    import tensorflow as tf
-    import torch
+    from attr import _CountingAttr  # type: ignore
+    from attr import _make_init  # type: ignore
+    from attr import _make_repr  # type: ignore
+    from attr import _transform_attrs  # type: ignore
+
     import transformers
-    from attr import (_CountingAttr, _make_init, _make_repr,  # type: ignore
-                      _transform_attrs)
     from transformers.generation.beam_constraints import Constraint
 
-    from ._types import ClickFunctionWrapper, F, O_co, P
+    from ._types import ClickFunctionWrapper
+    from ._types import F
+    from ._types import O_co
+    from ._types import P
 
     ReprArgs: t.TypeAlias = t.Iterable[tuple[str | None, t.Any]]
 
     DictStrAny = dict[str, t.Any]
     ListStr = list[str]
     ItemgetterAny = itemgetter[t.Any]
     FieldTransformers = t.Callable[[_T, list[attr.Attribute[t.Any]]], list[attr.Attribute[t.Any]]]
 else:
     Constraint = t.Any
     ListStr = list
     DictStrAny = dict
     ItemgetterAny = itemgetter
     # NOTE: Using internal API from attr here, since we are actually
     # allowing subclass of openllm.LLMConfig to become 'attrs'-ish
-    from attr._make import (_CountingAttr, _make_init, _make_repr,
-                            _transform_attrs)
+    from attr._make import _CountingAttr
+    from attr._make import _make_init
+    from attr._make import _make_repr
+    from attr._make import _transform_attrs
 
     transformers = openllm.utils.LazyLoader("transformers", globals(), "transformers")
-    torch = openllm.utils.LazyLoader("torch", globals(), "torch")
-    tf = openllm.utils.LazyLoader("tf", globals(), "tensorflow")
 
 __all__ = ["LLMConfig"]
 
 logger = logging.getLogger(__name__)
 
 config_merger = Merger(
     # merge dicts
@@ -476,15 +487,15 @@
             name_type="dasherize",
             requires_gpu=False,
             url="",
             use_pipeline=False,
             model_type="causal_lm",
             trust_remote_code=False,
             requirements=None,
-            timeout=3600,
+            timeout=int(36e6),
             service_name="",
             workers_per_resource=1,
             runtime="transformers",
         )
         return cls(**t.cast(DictStrAny, _))
 
 
@@ -848,15 +859,15 @@
 
         __openllm_start_name__: str = Field(None)
         """Default name to be used with `openllm start`"""
 
         __openllm_env__: openllm.utils.ModelEnv = Field(None, init=False)
         """A ModelEnv instance for this LLMConfig."""
 
-        __openllm_timeout__: int = Field(36000)
+        __openllm_timeout__: int = Field(36e6)
         """The default timeout to be set for this given LLM."""
 
         __openllm_workers_per_resource__: int | float = Field(1)
         """The number of workers per resource. This is used to determine the number of workers to use for this model.
         For example, if this is set to 0.5, then OpenLLM will use 1 worker per 2 resources. If this is set to 1, then
         OpenLLM will use 1 worker per resource. If this is set to 2, then OpenLLM will use 2 workers per resource.
 
@@ -958,15 +969,15 @@
                 attrs_init=True,  # whether to create __attrs_init__ instead of __init__
             ),
         )
         # __repr__ function with the updated fields.
         cls.__repr__ = codegen.add_method_dunders(cls, _make_repr(cls.__attrs_attrs__, None, cls))
         # Traverse the MRO to collect existing slots
         # and check for an existing __weakref__.
-        existing_slots: DictStrAny = dict()
+        existing_slots: DictStrAny = {}
         weakref_inherited = False
         for base_cls in cls.__mro__[1:-1]:
             if base_cls.__dict__.get("__weakref__", None) is not None:
                 weakref_inherited = True
             existing_slots.update({name: getattr(base_cls, name) for name in getattr(base_cls, "__slots__", [])})
 
         if (
@@ -980,15 +991,17 @@
         # We only add the names of attributes that aren't inherited.
         # Setting __slots__ to inherited attributes wastes memory.
         slot_names = [name for name in _attr_names if name not in _base_names]
         # There are slots for attributes from current class
         # that are defined in parent classes.
         # As their descriptors may be overridden by a child class,
         # we collect them here and update the class dict
-        reused_slots = {slot: slot_descriptor for slot, slot_descriptor in existing_slots.items() if slot in slot_names}
+        reused_slots = {
+            slot: slot_descriptor for slot, slot_descriptor in existing_slots.items() if slot in slot_names
+        }
         # __openllm_extras__ holds additional metadata that might be usefule for users, hence we add it to slots
         slot_names = [name for name in slot_names if name not in reused_slots] + ["__openllm_extras__"]
         cls.__slots__ = tuple(slot_names)
         # Finally, resolve the types
         if getattr(cls, "__attrs_types_resolved__", None) != cls:
             # NOTE: We will try to resolve type here, and cached it for faster use
             # It will be about 15-20ms slower comparing not resolving types.
@@ -1071,50 +1084,27 @@
             )
         internal_attributes = f"__openllm_{item}__"
         if hasattr(self, internal_attributes):
             return getattr(self, internal_attributes)
         elif hasattr(self, item):
             return getattr(self, item)
         elif hasattr(self.__openllm_generation_class__, item):
-            return getattr(self.__openllm_generation_class__, item)
+            return getattr(self.generation_config, item)
         elif item in self.__openllm_extras__:
             return self.__openllm_extras__[item]
         else:
             raise KeyError(item)
 
     def __getattribute__(self, item: str) -> t.Any:
         if item in _reserved_namespace:
             raise ForbiddenAttributeError(
                 f"'{item}' belongs to a private namespace for {self.__class__} and should not be access nor modified."
             )
         return _object_getattribute.__get__(self)(item)
 
-    @classmethod
-    def check_if_gpu_is_available(cls, implementation: str | None = None, force: bool = False):
-        if implementation is None:
-            implementation = cls.__openllm_env__["framework_value"]
-
-        try:
-            if cls.__openllm_requires_gpu__ or force:
-                if implementation in ("tf", "flax") and len(tf.config.list_physical_devices("GPU")) == 0:
-                    raise OpenLLMException("Required GPU for given model")
-                else:
-                    if not torch.cuda.is_available():
-                        raise OpenLLMException("Required GPU for given model")
-            else:
-                logger.debug(
-                    f"{cls} doesn't requires GPU by default. If you still want to check for GPU, set 'force=True'"
-                )
-        except OpenLLMException:
-            if force:
-                msg = "GPU is not available"
-            else:
-                msg = f"{cls} only supports running with GPU (None available)."
-            raise GpuNotAvailableError(msg) from None
-
     def model_dump(self, flatten: bool = False, **_: t.Any):
         dumped = bentoml_cattr.unstructure(self)
         if flatten:
             generation_config = dumped.pop("generation_config")
             dumped.update(generation_config)
         return dumped
 
@@ -1244,15 +1234,17 @@
     Otherwise, we will filter out all keys are first in LLMConfig, parse it in, then
     parse the remaining keys into LLMConfig.generation_config
     """
     if not LazyType(DictStrAny).isinstance(data):
         raise RuntimeError(f"Expected a dictionary, but got {type(data)}")
 
     generation_cls_fields = attr.fields_dict(cls.__openllm_generation_class__)
-    cls_attrs = {k: v for k, v in data.items() if k in cls.__openllm_accepted_keys__ and k not in generation_cls_fields}
+    cls_attrs = {
+        k: v for k, v in data.items() if k in cls.__openllm_accepted_keys__ and k not in generation_cls_fields
+    }
     if "generation_config" in data:
         generation_config = data.pop("generation_config")
         if not LazyType(DictStrAny).isinstance(generation_config):
             raise RuntimeError(f"Expected a dictionary, but got {type(generation_config)}")
         config_merger.merge(generation_config, {k: v for k, v in data.items() if k in generation_cls_fields})
     else:
         generation_config = {k: v for k, v in data.items() if k in generation_cls_fields}
```

### Comparing `openllm-0.1.6/src/openllm/_llm.py` & `openllm-0.1.7/src/openllm/_llm.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,32 +19,45 @@
 import logging
 import os
 import re
 import subprocess
 import sys
 import types
 import typing as t
-from abc import ABC, abstractmethod
+from abc import ABC
+from abc import abstractmethod
 
 import attr
-import bentoml
 import inflection
 import orjson
+
+import bentoml
+import openllm
 from bentoml._internal.models.model import ModelSignature
 from bentoml._internal.types import ModelSignatureDict
 
-import openllm
+from .exceptions import ForbiddenAttributeError
+from .exceptions import GpuNotAvailableError
+from .exceptions import OpenLLMException
+from .utils import DEBUG
+from .utils import LazyLoader
+from .utils import ModelEnv
+from .utils import bentoml_cattr
+from .utils import first_not_none
+from .utils import get_debug_mode
+from .utils import is_bitsandbytes_available
+from .utils import is_torch_available
+from .utils import is_transformers_supports_kbit
+from .utils import non_intrusive_setattr
+from .utils import pkg
 
-from .exceptions import ForbiddenAttributeError, OpenLLMException
-from .utils import (DEBUG, LazyLoader, ModelEnv, bentoml_cattr, first_not_none,
-                    get_debug_mode, is_bitsandbytes_available,
-                    is_torch_available, non_intrusive_setattr, pkg)
 
 if t.TYPE_CHECKING:
     import torch
+
     import transformers
     from bentoml._internal.runner.strategy import Strategy
 
     from .models.auto.factory import _BaseAutoLLMClass
 
     class LLMRunner(bentoml.Runner):
         __doc__: str
@@ -198,14 +211,25 @@
     def generate(self, prompt: str, **preprocess_generate_kwds: t.Any) -> t.Any:
         """The main function implementation for generating from given prompt.  It takes the prompt
         and the generation_kwargs from 'self.sanitize_parameters' and then
         pass it to 'self.model.generate'.
         """
         raise NotImplementedError
 
+    def generate_one(
+        self,
+        prompt: str,
+        stop: list[str],
+        **preprocess_generate_kwds: t.Any,
+    ) -> list[dict[t.Literal["generated_text"], str]]:
+        """The entrypoint for generating one prompt. This provides additional stop
+        tokens for generating per token level. This is useful when running with agents, or initial streaming support.
+        """
+        raise NotImplementedError
+
     def generate_iterator(self, prompt: str, **attrs: t.Any) -> t.Iterator[t.Any]:
         """An iterator version of generate function."""
         raise NotImplementedError(
             "Currently generate_iterator requires SSE (Server-side events) support, which is not yet implemented."
         )
 
     def sanitize_parameters(self, prompt: str, **attrs: t.Any) -> tuple[str, dict[str, t.Any], dict[str, t.Any]]:
@@ -297,15 +321,15 @@
                     "Missing required key 'config_class'. Make sure to define it within the LLM subclass."
                 )
 
         if cls.import_model is LLMInterface.import_model:
             # using the default import model
             setattr(cls, "import_model", functools.partial(import_model, _model_framework=implementation))
         else:
-            logger.debug("Custom 'import_model' will be used when loading modelj %s", cls.__name__)
+            logger.debug("Custom 'import_model' will be used when loading model %s", cls.__name__)
 
         cls.__llm_post_init__ = None if cls.llm_post_init is LLMInterface.llm_post_init else cls.llm_post_init
         cls.__llm_custom_load__ = None if cls.load_model is LLMInterface.load_model else cls.load_model
         cls.__llm_init_kwargs__ = None if cls.import_kwargs is LLMInterface.import_kwargs else cls.import_kwargs
 
         for at in {"bentomodel", "tag", "model", "tokenizer"}:
             setattr(cls, f"__llm_{at}__", None)
@@ -440,15 +464,15 @@
         int8_has_fp16_weight = attrs.pop("llm_int8_has_fp16_weight", False)
         # 4 bit configuration
         int4_compute_dtype = attrs.pop("llm_bnb_4bit_compute_dtype", torch.bfloat16)
         int4_quant_type = attrs.pop("llm_bnb_4bit_quant_type", "nf4")
         int4_use_double_quant = attrs.pop("llm_bnb_4bit_use_double_quant", True)
 
         if llm_config is not None:
-            logger.debug("Using given 'llm_config=(%s)' to initialize LLM.", llm_config)
+            logger.debug("Using provided LLMConfig to initialize LLM instead of from default.", llm_config)
             self.config = llm_config
         else:
             self.config = self.config_class.model_construct_env(**attrs)
             # The rests of the kwargs that is not used by the config class should be stored into __openllm_extras__.
             attrs = self.config["extras"]
 
         if quantization_config and quantize:
@@ -482,30 +506,28 @@
                         load_in_8bit=True,
                         llm_int8_enable_fp32_cpu_offload=cpu_offloading,
                         llm_int8_threshhold=int8_threshold,
                         llm_int8_skip_modules=int8_skip_modules,
                         llm_int8_has_fp16_weight=int8_has_fp16_weight,
                     )
                 elif quantize == "int4":
-                    trf_versions = pkg.pkg_version_info("transformers")
-                    supports_kbits = trf_versions[:2] >= (4, 30)
-                    if supports_kbits:
+                    if is_transformers_supports_kbit():
                         quantization_config = transformers.BitsAndBytesConfig(
                             load_in_4bit=True,
                             llm_bnb_4bit_compute_dtype=int4_compute_dtype,
                             llm_bnb_4bit_quant_type=int4_quant_type,
                             llm_bnb_4bit_use_double_quant=int4_use_double_quant,
                         )
                     else:
                         logger.warning(
                             "'quantize' is set to int4, while the current transformers version %s does not support "
                             "k-bit quantization. k-bit quantization is supported since transformers 4.30, therefore "
                             "make sure to install the latest version of transformers either via PyPI or "
                             "from git source: 'pip install git+https://github.com/huggingface/transformers'.",
-                            trf_versions,
+                            pkg.pkg_version_info("transformers"),
                         )
                 elif quantize == "gptq":
                     # TODO: support GPTQ loading quantization
                     if model_id is None:
                         raise RuntimeError(
                             "'quantize=%s' requires passing custom path to quantized weights as we are unable to load "
                             "the model on the fly. See https://github.com/qwopqwop200/GPTQ-for-LLaMa for "
@@ -712,15 +734,16 @@
             )
         return self.__llm_tag__
 
     @property
     def model(self) -> _M:
         """The model to use for this LLM. This shouldn't be set at runtime, rather let OpenLLM handle it."""
         # Run check for GPU
-        self.config.check_if_gpu_is_available(implementation=self.__llm_implementation__)
+        if self.config["requires_gpu"] and len(openllm.utils.gpu_count()) < 1:
+            raise GpuNotAvailableError(f"{self} only supports running with GPU (None available).") from None
 
         kwds = self._model_attrs
         kwds["trust_remote_code"] = self.__llm_trust_remote_code__
 
         is_pipeline = "_pretrained_class" in self._bentomodel.info.metadata
         # differentiate when saving tokenizer or other pretrained type.
         is_pretrained_model = is_pipeline and "_framework" in self._bentomodel.info.metadata
@@ -796,15 +819,19 @@
             from bentoml._internal.runner.strategy import DefaultStrategy
 
             scheduling_strategy = DefaultStrategy
 
         generate_sig = ModelSignature.from_dict(ModelSignatureDict(batchable=False))
         generate_iterator_sig = ModelSignature.from_dict(ModelSignatureDict(batchable=True))
         if method_configs is None:
-            method_configs = {"generate": generate_sig, "generate_iterator": generate_iterator_sig}
+            method_configs = {
+                "generate": generate_sig,
+                "generate_one": generate_sig,
+                "generate_iterator": generate_iterator_sig,
+            }
         else:
             signatures = ModelSignature.convert_signatures_dict(method_configs)
             generate_sig = first_not_none(signatures.get("generate"), default=generate_sig)
             generate_iterator_sig = first_not_none(signatures.get("generate_iterator"), default=generate_iterator_sig)
 
         class _Runnable(bentoml.Runnable):
             SUPPORTED_RESOURCES = ("nvidia.com/gpu", "cpu")
@@ -838,14 +865,25 @@
                 input_spec=generate_sig.input_spec,
                 output_spec=generate_sig.output_spec,
             )
             def generate(__self, prompt: str, **attrs: t.Any) -> list[t.Any]:
                 return self.generate(prompt, **attrs)
 
             @bentoml.Runnable.method(
+                batchable=generate_sig.batchable,
+                batch_dim=generate_sig.batch_dim,
+                input_spec=generate_sig.input_spec,
+                output_spec=generate_sig.output_spec,
+            )
+            def generate_one(
+                __self, prompt: str, stop: list[str], **attrs: t.Any
+            ) -> list[dict[t.Literal["generated_text"], str]]:
+                return self.generate_one(prompt, stop, **attrs)
+
+            @bentoml.Runnable.method(
                 batchable=generate_iterator_sig.batchable,
                 batch_dim=generate_iterator_sig.batch_dim,
                 input_spec=generate_iterator_sig.input_spec,
                 output_spec=generate_iterator_sig.output_spec,
             )
             def generate_iterator(__self, prompt: str, **attrs: t.Any) -> t.Iterator[t.Any]:
                 yield self.generate_iterator(prompt, **attrs)
```

### Comparing `openllm-0.1.6/src/openllm/_package.py` & `openllm-0.1.7/src/openllm/_package.py`

 * *Files 11% similar despite different names*

```diff
@@ -18,24 +18,31 @@
 
 import importlib.metadata
 import logging
 import os
 import typing as t
 from pathlib import Path
 
-import bentoml
 import fs
 import inflection
-from bentoml._internal.bento.build_config import DockerOptions, PythonOptions
-from bentoml._internal.configuration import get_debug_mode
 
+import bentoml
 import openllm
+from bentoml._internal.bento.build_config import DockerOptions
+from bentoml._internal.bento.build_config import PythonOptions
+from bentoml._internal.configuration import get_debug_mode
+
+from .utils import ModelEnv
+from .utils import codegen
+from .utils import first_not_none
+from .utils import is_flax_available
+from .utils import is_tf_available
+from .utils import is_torch_available
+from .utils import pkg
 
-from .utils import (ModelEnv, codegen, first_not_none, is_flax_available,
-                    is_tf_available, is_torch_available, pkg)
 
 if t.TYPE_CHECKING:
     from fs.base import FS
 
     from .models.auto.factory import _BaseAutoLLMClass
 
 logger = logging.getLogger(__name__)
@@ -68,20 +75,27 @@
             env.install(builder.build_system_requires)
             return builder.build("wheel", path, config_settings={"--global-option": "--quiet"})
     raise RuntimeError(
         "Custom OpenLLM build is currently not supported. Please install OpenLLM from PyPI or built it from Git source."
     )
 
 
-def construct_python_options(llm: openllm.LLM[t.Any, t.Any], llm_fs: FS) -> PythonOptions:
+def construct_python_options(
+    llm: openllm.LLM[t.Any, t.Any],
+    llm_fs: FS,
+    extra_dependencies: tuple[str, ...] | None = None,
+) -> PythonOptions:
     # NOTE: add openllm to the default dependencies
     # if users has openllm custom built wheels, it will still respect
     # that since bentoml will always install dependencies from requirements.txt
     # first, then proceed to install everything inside the wheels/ folder.
-    packages: list[str] = ["openllm"]
+    if extra_dependencies is not None:
+        packages = [f"openllm[{k}]" for k in extra_dependencies]
+    else:
+        packages = ["openllm"]
 
     if llm.config["requirements"] is not None:
         packages.extend(llm.config["requirements"])
 
     if not (str(os.environ.get("BENTOML_BUNDLE_LOCAL_BUILD", False)).lower() == "false"):
         packages.append(f"bentoml>={'.'.join([str(i) for i in pkg.pkg_version_info('bentoml')])}")
 
@@ -171,14 +185,15 @@
 @t.overload
 def build(
     model_name: str,
     *,
     model_id: str | None = ...,
     quantize: t.LiteralString | None = ...,
     bettertransformer: bool | None = ...,
+    _extra_dependencies: tuple[str, ...] | None = ...,
     _workers_per_resource: int | float | None = ...,
     _overwrite_existing_bento: bool = ...,
     __cli__: t.Literal[False] = ...,
     **attrs: t.Any,
 ) -> bentoml.Bento:
     ...
 
@@ -186,14 +201,15 @@
 @t.overload
 def build(
     model_name: str,
     *,
     model_id: str | None = ...,
     quantize: t.LiteralString | None = ...,
     bettertransformer: bool | None = ...,
+    _extra_dependencies: tuple[str, ...] | None = ...,
     _workers_per_resource: int | float | None = ...,
     _overwrite_existing_bento: bool = ...,
     __cli__: t.Literal[True] = ...,
     **attrs: t.Any,
 ) -> tuple[bentoml.Bento, bool]:
     ...
 
@@ -202,41 +218,41 @@
     bento_tag: bentoml.Tag,
     service_name: str,
     llm_fs: FS,
     llm: openllm.LLM[t.Any, t.Any],
     workers_per_resource: int | float,
     quantize: t.LiteralString | None,
     bettertransformer: bool | None,
+    extra_dependencies: tuple[str, ...] | None = None,
 ) -> bentoml.Bento:
     framework_envvar = llm.config["env"]["framework_value"]
     labels = dict(llm.identifying_params)
     labels.update({"_type": llm.llm_type, "_framework": framework_envvar})
     logger.info("Building Bento for LLM '%s'", llm.config["start_name"])
     return bentoml.bentos.build(
         f"{service_name}:svc",
         name=bento_tag.name,
         labels=labels,
         description=f"OpenLLM service for {llm.config['start_name']}",
-        include=[
-            f for f in llm_fs.walk.files(filter=["*.py"])
-        ],  # NOTE: By default, we are using _service.py as the default service, for now.
+        include=list(llm_fs.walk.files(filter=["*.py"])),  # NOTE: By default, we are using _service.py as the default service, for now.
         exclude=["/venv", "__pycache__/", "*.py[cod]", "*$py.class"],
-        python=construct_python_options(llm, llm_fs),
+        python=construct_python_options(llm, llm_fs, extra_dependencies),
         docker=construct_docker_options(llm, llm_fs, workers_per_resource, quantize, bettertransformer),
         version=bento_tag.version,
         build_ctx=llm_fs.getsyspath("/"),
     )
 
 
 def build(
     model_name: str,
     *,
     model_id: str | None = None,
     quantize: t.LiteralString | None = None,
     bettertransformer: bool | None = None,
+    _extra_dependencies: tuple[str, ...] | None = None,
     _workers_per_resource: int | float | None = None,
     _overwrite_existing_bento: bool = False,
     __cli__: bool = False,
     **attrs: t.Any,
 ) -> tuple[bentoml.Bento, bool] | bentoml.Bento:
     """Package a LLM into a Bento.
 
@@ -294,26 +310,28 @@
                         bento_tag,
                         service_name,
                         llm_fs,
                         llm,
                         workers_per_resource=workers_per_resource,
                         quantize=quantize,
                         bettertransformer=bettertransformer,
+                        extra_dependencies=_extra_dependencies,
                     )
                 _previously_built = True
             except bentoml.exceptions.NotFound:
                 logger.info("Building Bento for LLM '%s'", llm_config["start_name"])
                 bento = _build_bento(
                     bento_tag,
                     service_name,
                     llm_fs,
                     llm,
                     workers_per_resource=workers_per_resource,
                     quantize=quantize,
                     bettertransformer=bettertransformer,
+                    extra_dependencies=_extra_dependencies,
                 )
             return (bento, _previously_built) if __cli__ else bento
     except Exception as e:
         logger.error("\nException caught during building LLM %s: \n", model_name, exc_info=e)
         raise
     finally:
         del os.environ["OPENLLM_MODEL"]
```

### Comparing `openllm-0.1.6/src/openllm/_prompt.py` & `openllm-0.1.7/src/openllm/_prompt.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.6/src/openllm/_schema.py` & `openllm-0.1.7/src/openllm/_schema.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 import typing as t
 
 import attr
 import inflection
 
 import openllm
 
+
 if t.TYPE_CHECKING:
     DictStrAny = dict[str, t.Any]
 else:
     DictStrAny = dict
 
 
 @attr.frozen(slots=True)
```

### Comparing `openllm-0.1.6/src/openllm/_types.py` & `openllm-0.1.7/src/openllm/_types.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,19 +17,21 @@
 Note that this module SHOULD NOT BE IMPORTED DURING RUNTIME, as this serve only for typing purposes.
 It will raises a RuntimeError if this is imported eagerly.
 """
 from __future__ import annotations
 
 import typing as t
 
+
 if not t.TYPE_CHECKING:
     raise RuntimeError(f"{__name__} should not be imported during runtime")
 
 import click
 
+
 P = t.ParamSpec("P")
 O_co = t.TypeVar("O_co", covariant=True)
 
 
 class ClickFunctionWrapper(t.Protocol[P, O_co]):
     __name__: str
     __click_params__: list[click.Option]
```

### Comparing `openllm-0.1.6/src/openllm/cli.py` & `openllm-0.1.7/src/openllm/cli.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,46 +16,64 @@
 
 This extends BentoML's internal CLI CommandGroup.
 """
 from __future__ import annotations
 
 import functools
 import inspect
+import itertools
 import logging
 import os
 import re
 import sys
 import time
 import traceback
 import typing as t
 
-import bentoml
 import click
 import click_option_group as cog
 import inflection
 import orjson
 import psutil
-from bentoml._internal.configuration.containers import BentoMLContainer
 from bentoml_cli.utils import BentoMLCommandGroup
-from simple_di import Provide, inject
+from bentoml_cli.utils import opt_callback
+from simple_di import Provide
+from simple_di import inject
 
+import bentoml
 import openllm
+from bentoml._internal.configuration.containers import BentoMLContainer
 
 from .__about__ import __version__
 from .exceptions import OpenLLMException
-from .utils import (DEBUG, LazyLoader, LazyType, ModelEnv, analytics,
-                    bentoml_cattr, configure_logging, configure_server_logging,
-                    first_not_none, get_debug_mode, get_quiet_mode, gpu_count,
-                    is_torch_available, set_debug_mode, set_quiet_mode)
+from .utils import DEBUG
+from .utils import LazyLoader
+from .utils import LazyType
+from .utils import ModelEnv
+from .utils import analytics
+from .utils import bentoml_cattr
+from .utils import configure_logging
+from .utils import first_not_none
+from .utils import get_debug_mode
+from .utils import get_quiet_mode
+from .utils import gpu_count
+from .utils import is_torch_available
+from .utils import is_transformers_supports_agent
+from .utils import set_debug_mode
+from .utils import set_quiet_mode
+
 
 if t.TYPE_CHECKING:
     import torch
+
     from bentoml._internal.models import ModelStore
 
-    from ._types import ClickFunctionWrapper, F, P
+    from ._types import ClickFunctionWrapper
+    from ._types import F
+    from ._types import P
     from .models.auto.factory import _BaseAutoLLMClass
 
     ServeCommand = t.Literal["serve", "serve-grpc"]
     OutputLiteral = t.Literal["json", "pretty", "porcelain"]
 
     TupleStrAny = tuple[str, ...]
 else:
@@ -134,15 +152,15 @@
     if not LazyType(TupleStrAny).isinstance(value):
         raise RuntimeError(f"{params} only accept multiple values.")
 
     # NOTE: --device all is a special case
     if len(value) == 1 and value[0] == "all":
         return gpu_count()
 
-    parsed: tuple[str, ...] = tuple()
+    parsed: tuple[str, ...] = ()
     for v in value:
         if v == ",":
             # NOTE: This hits when CUDA_VISIBLE_DEVICES is set
             continue
         if "," in v:
             parsed += tuple(v.split(","))
         else:
@@ -240,16 +258,16 @@
     @staticmethod
     def common_params(f: F[P, t.Any]) -> ClickFunctionWrapper[..., t.Any]:
         """This is not supposed to be used with unprocessed click function.
         This should be used a the last currying from common_params -> usage_tracking -> exception_handling
         """
         # The following logics is similar to one of BentoMLCommandGroup
 
-        from bentoml._internal.configuration import (DEBUG_ENV_VAR,
-                                                     QUIET_ENV_VAR)
+        from bentoml._internal.configuration import DEBUG_ENV_VAR
+        from bentoml._internal.configuration import QUIET_ENV_VAR
 
         @click.option("-q", "--quiet", envvar=QUIET_ENV_VAR, is_flag=True, default=False, help="Suppress all output.")
         @click.option(
             "--debug", "--verbose", envvar=DEBUG_ENV_VAR, is_flag=True, default=False, help="Print out debug logs."
         )
         @click.option(
             "--do-not-track",
@@ -417,24 +435,30 @@
 
 
 @cli.group(cls=OpenLLMCommandGroup, context_settings=_CONTEXT_SETTINGS, name="start")
 def start_cli():
     """
     Start any LLM as a REST server.
 
+    \b
+    ```bash
     $ openllm start <model_name> --<options> ...
+    ```
     """
 
 
 @cli.group(cls=OpenLLMCommandGroup, context_settings=_CONTEXT_SETTINGS, name="start-grpc")
 def start_grpc_cli():
     """
     Start any LLM as a gRPC server.
 
+    \b
+    ```bash
     $ openllm start-grpc <model_name> --<options> ...
+    ```
     """
 
 
 # NOTE: A list of bentoml option that is not needed for parsing.
 # NOTE: User shouldn't set '--working-dir', as OpenLLM will setup this.
 # NOTE: production is also deprecated
 _IGNORED_OPTIONS = {"working_dir", "production", "protocol_version"}
@@ -558,31 +582,32 @@
         type=int,
         default=None,
         help="Server timeout in seconds",
     )
     @workers_per_resource_option(cog.optgroup)
     @model_id_option(cog.optgroup, model_env=env, click_type=click.Choice(llm_config["model_ids"]))
     @cog.optgroup.option(
+        "--fast",
+        is_flag=True,
+        default=False,
+        help="Bypass auto model checks and setup. This option is ahead-of-serving time.",
+    )
+    @cog.optgroup.group("LLM Optimization Options.")
+    @cog.optgroup.option(
         "--device",
         type=tuple,
         cls=NargsOptions,
         nargs=-1,
         envvar="CUDA_VISIBLE_DEVICES",
         callback=parse_device_callback,
         help=f"Assign GPU devices (if available) for {model_name}.",
         show_envvar=True,
     )
     @quantize_option(cog.optgroup)
     @bettertransformer_option(cog.optgroup, model_env=env)
-    @cog.optgroup.option(
-        "--fast",
-        is_flag=True,
-        default=False,
-        help="Bypass auto model checks and setup. This option is ahead-of-serving time.",
-    )
     @click.pass_context
     def model_start(
         ctx: click.Context,
         server_timeout: int | None,
         model_id: str | None,
         workers_per_resource: float | None,
         device: tuple[str, ...] | None,
@@ -655,14 +680,19 @@
                     f'runners."llm-{config["start_name"]}-runner".resources."nvidia.com/gpu"=[{device[0]}]'
                 )
 
         _bentoml_config_options_env += (
             " " if _bentoml_config_options_env else "" + " ".join(_bentoml_config_options_opts)
         )
 
+        if fast and not get_quiet_mode():
+            _echo(
+                f"Make sure to download the model before 'start': 'openllm download {model_name}{'--model-id ' + model_id if model_id else ''}'",
+                fg="yellow",
+            )
         automodel_attrs = {
             "model_id": model_id,
             "llm_config": config,
             "ensure_available": not fast,
         }
 
         if framework_envvar == "pt":
@@ -739,53 +769,72 @@
 
 
 start = functools.partial(_start, _serve_grpc=False)
 start_grpc = functools.partial(_start, _serve_grpc=True)
 
 
 @cli.command()
-@click.argument("model_name", type=click.Choice([inflection.dasherize(name) for name in openllm.CONFIG_MAPPING.keys()]))
+@click.argument(
+    "model_name", type=click.Choice([inflection.dasherize(name) for name in openllm.CONFIG_MAPPING.keys()])
+)
 @model_id_option(click)
 @output_option
 @click.option("--overwrite", is_flag=True, help="Overwrite existing Bento for given LLM if it already exists.")
 @workers_per_resource_option(click, build=True)
 @cog.optgroup.group(cls=cog.MutuallyExclusiveOptionGroup, name="Optimisation options.")
 @quantize_option(cog.optgroup, build=True)
 @bettertransformer_option(cog.optgroup)
+@click.option(
+    "--enable-features",
+    help="Enable additional features for building this LLM Bento. Available: {}".format(
+        ", ".join(openllm.utils.OPTIONAL_DEPENDENCIES)
+    ),
+    multiple=True,
+    nargs=1,
+    metavar="FEATURE[,FEATURE]",
+)
 def build(
     model_name: str,
     model_id: str | None,
     overwrite: bool,
     output: OutputLiteral,
     quantize: t.Literal["int8", "int4", "gptq"] | None,
+    enable_features: tuple[str] | None,
     bettertransformer: bool | None,
     workers_per_resource: float | None,
 ):
     """Package a given models into a Bento.
 
-    $ openllm build flan-t5
+    \b
+    ```bash
+    $ openllm build flan-t5 --model-id google/flan-t5-large
+    ```
 
     \b
-    NOTE: To run a container built from this Bento with GPU support, make sure
-    to have https://github.com/NVIDIA/nvidia-container-toolkit install locally.
+    > NOTE: To run a container built from this Bento with GPU support, make sure
+    > to have https://github.com/NVIDIA/nvidia-container-toolkit install locally.
     """
     if output == "porcelain":
         set_quiet_mode(True)
-        configure_server_logging()
+        configure_logging()
 
     if output == "pretty":
         if overwrite:
             _echo(f"Overwriting existing Bento for {model_name}.", fg="yellow")
 
+    if enable_features:
+        enable_features = tuple(itertools.chain.from_iterable((s.split(",") for s in enable_features)))
+
     bento, _previously_built = openllm.build(
         model_name,
         __cli__=True,
         model_id=model_id,
         quantize=quantize,
         bettertransformer=bettertransformer,
+        _extra_dependencies=enable_features,
         _workers_per_resource=workers_per_resource,
         _overwrite_existing_bento=overwrite,
     )
 
     if output == "pretty":
         if not get_quiet_mode():
             _echo("\n" + OPENLLM_FIGLET, fg="white")
@@ -822,15 +871,21 @@
     is_flag=True,
     default=False,
     help="Show available models in local store (mutually exclusive with '-o porcelain').",
 )
 def models(output: OutputLiteral, show_available: bool):
     """List all supported models.
 
-    NOTE: '--show-available' and '-o porcelain' are mutually exclusive.
+    \b
+    > NOTE: '--show-available' and '-o porcelain' are mutually exclusive.
+
+    \b
+    ```bash
+    openllm models --show-available
+    ```
     """
     from ._llm import convert_transformers_model_name
 
     models = tuple(inflection.dasherize(key) for key in openllm.CONFIG_MAPPING.keys())
     if output == "porcelain":
         if show_available:
             raise click.BadOptionUsage(
@@ -846,15 +901,15 @@
 
         # NOTE: Keep a sync list with ./tools/update-optional-dependencies.py
         extras = ["chatglm", "falcon", "flan-t5", "starcoder"]
 
         converted: list[str] = []
         for m in models:
             config = openllm.AutoConfig.for_model(m)
-            runtime_impl: tuple[t.Literal["pt", "flax", "tf"], ...] = tuple()
+            runtime_impl: tuple[t.Literal["pt", "flax", "tf"] | str, ...] = ()
             if config["model_name"] in openllm.MODEL_MAPPING_NAMES:
                 runtime_impl += ("pt",)
             if config["model_name"] in openllm.MODEL_FLAX_MAPPING_NAMES:
                 runtime_impl += ("flax",)
             if config["model_name"] in openllm.MODEL_TF_MAPPING_NAMES:
                 runtime_impl += ("tf",)
             json_data[m] = {
@@ -895,16 +950,16 @@
                             "✅" if v["requires_gpu"] else "❌",
                             v["runtime_impl"],
                         )
                     ]
                 )
             column_widths = [
                 int(COLUMNS / 6),
-                int(COLUMNS / 6),
                 int(COLUMNS / 3),
+                int(COLUMNS / 4),
                 int(COLUMNS / 6),
                 int(COLUMNS / 6),
                 int(COLUMNS / 9),
             ]
 
             if len(data) == 0 and len(failed_initialized) > 0:
                 _echo("Exception found while parsing models:\n", fg="yellow")
@@ -993,38 +1048,150 @@
             delete_confirmed = click.confirm(f"delete model {model.tag}?")
 
         if delete_confirmed:
             model_store.delete(model.tag)
             click.echo(f"{model} deleted.")
 
 
-@cli.command(name="query")
+# Can also support agent type such as langchain and other variants here.
+_AGENT_MAPPING = {"hf": "/hf/agent"}
+
+
+def parsing_instruction_callback(
+    ctx: click.Context, param: click.Parameter, value: list[str] | str | None
+) -> tuple[str, bool | str] | list[str] | str | None:
+    if value is None:
+        return value
+
+    if isinstance(value, list):
+        # we only parse --text foo bar -> --text foo and omit bar
+        value = value[-1]
+    if not isinstance(value, str):
+        raise click.BadParameter(f"Invalid option format: {value}")
+
+    key, *values = value.split("=")
+    if not key.startswith("--"):
+        raise click.BadParameter(f"Invalid option format: {value}")
+    key = key[2:]
+    if len(values) == 0:
+        return key, True
+    elif len(values) == 1:
+        return key, values[0]
+    else:
+        raise click.BadParameter(f"Invalid option format: {value}")
+
+
+def shared_client_options(f: t.Callable[..., t.Any]) -> t.Callable[..., t.Any]:
+    options = [
+        click.option(
+            "--endpoint",
+            type=click.STRING,
+            help="OpenLLM Server endpoint, i.e: http://localhost:3000",
+            envvar="OPENLLM_ENDPOINT",
+            default="http://localhost:3000",
+        ),
+        click.option("--timeout", type=click.INT, default=30, help="Default server timeout", show_default=True),
+        output_option,
+    ]
+    for opt in reversed(options):
+        f = opt(f)
+    return f
+
+
+@cli.command()
+@click.argument("task", type=click.STRING, metavar="TASK")
+@shared_client_options
 @click.option(
-    "--endpoint",
-    type=click.STRING,
-    help="OpenLLM Server endpoint, i.e: http://localhost:3000",
-    envvar="OPENLLM_ENDPOINT",
-    default="http://localhost:3000",
+    "--agent",
+    type=click.Choice(["hf"]),
+    default="hf",
+    help="Whether to interact with Agents from given Server endpoint.",
+    show_default=True,
 )
-@click.option("--timeout", type=click.INT, default=30, help="Default server timeout", show_default=True)
+@click.option(
+    "--remote",
+    is_flag=True,
+    default=False,
+    help="Whether or not to use remote tools (inference endpoints) instead of local ones.",
+    show_default=True,
+)
+@click.option(
+    "--opt",
+    help="Define prompt options. "
+    "(format: ``--opt text='I love this' --opt audio:./path/to/audio  --opt image:/path/to/file``)",
+    required=False,
+    multiple=True,
+    callback=opt_callback,
+    metavar="ARG=VALUE[,ARG=VALUE]",
+)
+def instruct(
+    endpoint: str,
+    timeout: int,
+    agent: t.LiteralString,
+    output: OutputLiteral,
+    remote: bool,
+    task: str,
+    _memoized: dict[str, t.Any],
+    **attrs: t.Any,
+):
+    """Instruct agents interactively for given tasks, from a terminal
+
+    \b
+    ```bash
+    $ openllm instruct --endpoint http://12.323.2.1:3000 \\
+        "Is the following `text` (in Spanish) positive or negative?" \\
+        --text "¡Este es un API muy agradable!"
+    ```
+    """
+    client = openllm.client.HTTPClient(endpoint, timeout=timeout)
+
+    breakpoint()
+
+    if agent == "hf":
+        if not is_transformers_supports_agent():
+            raise click.UsageError(
+                "Transformers version should be at least 4.29 to support HfAgent. "
+                "Upgrade with 'pip install -U transformers'"
+            )
+
+        _memoized = {k: v[0] for k, v in _memoized.items() if v}
+
+        client._hf_agent.set_stream(logger)
+        if output != "porcelain":
+            _echo(f"Sending the following prompt ('{task}') with the following vars: {_memoized}", fg="magenta")
+
+        result = client.agent(task, agent_type=agent, return_code=False, remote=remote, **_memoized)
+        if output == "json":
+            _echo(orjson.dumps(result, option=orjson.OPT_INDENT_2).decode(), fg="white")
+        else:
+            _echo(result, fg="white")
+        return result
+    else:
+        raise click.BadOptionUsage("agent", f"Unknown agent type {agent}")
+
+
+@cli.command()
+@shared_client_options
 @click.option(
     "--server-type", type=click.Choice(["grpc", "http"]), help="Server type", default="http", show_default=True
 )
-@output_option
-@click.argument("query", type=click.STRING)
-def query_(
-    query: str,
+@click.argument("prompt", type=click.STRING)
+def query(
+    prompt: str,
     endpoint: str,
     timeout: int,
     server_type: t.Literal["http", "grpc"],
     output: OutputLiteral,
 ):
     """Ask a LLM interactively, from a terminal.
 
+    \b
+    ```bash
     $ openllm query --endpoint http://12.323.2.1:3000 "What is the meaning of life?"
+    ```
     """
     if server_type == "grpc":
         endpoint = re.sub(r"http://", "", endpoint)
     client = (
         openllm.client.HTTPClient(endpoint, timeout=timeout)
         if server_type == "http"
         else openllm.client.GrpcClient(endpoint, timeout=timeout)
@@ -1032,20 +1199,20 @@
 
     model = t.cast(
         "_BaseAutoLLMClass",
         openllm[client.framework],  # type: ignore (internal API)
     ).for_model(client.model_name)
 
     if output != "porcelain":
-        _echo(f"Processing query: {query}\n", fg="white")
+        _echo(f"Processing query: {prompt}", fg="white")
 
-    res = client.query(query, return_raw_response=True)
+    res = client.query(prompt, return_raw_response=True)
 
     if output == "pretty":
-        formatted = model.postprocess_generate(query, res["responses"])
+        formatted = model.postprocess_generate(prompt, res["responses"])
         _echo("Responses: ", fg="white", nl=False)
         _echo(formatted, fg="cyan")
     elif output == "json":
         _echo(orjson.dumps(res, option=orjson.OPT_INDENT_2).decode(), fg="white")
     else:
         _echo(res["responses"], fg="white")
 
@@ -1056,15 +1223,21 @@
     type=click.Choice([inflection.dasherize(name) for name in openllm.CONFIG_MAPPING.keys()]),
 )
 @model_id_option(click)
 @output_option
 def download_models(model_name: str, model_id: str | None, output: OutputLiteral):
     """Setup LLM interactively.
 
+    \b
     Note: This is useful for development and setup for fine-tune.
+
+    \b
+    ```bash
+    $ openllm download opt --model-id facebook/opt-2.7b
+    ```
     """
     if output == "porcelain":
         set_quiet_mode(True)
         configure_logging()
 
     config = openllm.AutoConfig.for_model(model_name)
     envvar = config["env"]["framework_value"]
```

### Comparing `openllm-0.1.6/src/openllm/client.py` & `openllm-0.1.7/src/openllm/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 """
 from __future__ import annotations
 
 import importlib
 import itertools
 import typing as t
 
+
 _import_structure = {
     "runtimes.grpc": ["AsyncGrpcClient", "GrpcClient"],
     "runtimes.http": ["AsyncHTTPClient", "HTTPClient"],
 }
 
 if t.TYPE_CHECKING:
     from openllm_client import AsyncGrpcClient as AsyncGrpcClient
```

### Comparing `openllm-0.1.6/src/openllm/exceptions.py` & `openllm-0.1.7/src/openllm/exceptions.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.6/src/openllm/models/__init__.py` & `openllm-0.1.7/src/openllm/models/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.6/src/openllm/models/auto/__init__.py` & `openllm-0.1.7/src/openllm/models/auto/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 
 import typing as t
 
 import openllm
 
 from ... import utils
 
+
 _import_structure = {
     "configuration_auto": ["AutoConfig", "CONFIG_MAPPING", "CONFIG_MAPPING_NAMES"],
     "modeling_auto": ["MODEL_MAPPING_NAMES"],
     "modeling_flax_auto": ["MODEL_FLAX_MAPPING_NAMES"],
     "modeling_tf_auto": ["MODEL_TF_MAPPING_NAMES"],
 }
```

### Comparing `openllm-0.1.6/src/openllm/models/auto/configuration_auto.py` & `openllm-0.1.7/src/openllm/models/auto/configuration_auto.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,16 +18,19 @@
 import typing as t
 from collections import OrderedDict
 
 import inflection
 
 import openllm
 
+
 if t.TYPE_CHECKING:
-    from collections import _odict_items, _odict_keys, _odict_values
+    from collections import _odict_items
+    from collections import _odict_keys
+    from collections import _odict_values
 
     ConfigOrderedDict = OrderedDict[str, type[openllm.LLMConfig]]
 
     ConfigKeysView = _odict_keys[str, type[openllm.LLMConfig]]
     ConfigValuesView = _odict_values[str, type[openllm.LLMConfig]]
     ConfigItemsView = _odict_items[str, type[openllm.LLMConfig]]
 else:
```

### Comparing `openllm-0.1.6/src/openllm/models/auto/factory.py` & `openllm-0.1.7/src/openllm/models/auto/factory.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,16 +22,19 @@
 
 import inflection
 
 import openllm
 
 from .configuration_auto import AutoConfig
 
+
 if t.TYPE_CHECKING:
-    from collections import _odict_items, _odict_keys, _odict_values
+    from collections import _odict_items
+    from collections import _odict_keys
+    from collections import _odict_values
 
     from ..._llm import LLMRunner
 
     ConfigModelOrderedDict = OrderedDict[type[openllm.LLMConfig], type[openllm.LLM[t.Any, t.Any]]]
     ConfigModelKeysView = _odict_keys[type[openllm.LLMConfig], type[openllm.LLM[t.Any, t.Any]]]
     ConfigModelValuesView = _odict_values[type[openllm.LLMConfig], type[openllm.LLM[t.Any, t.Any]]]
     ConfigModelItemsView = _odict_items[type[openllm.LLMConfig], type[openllm.LLM[t.Any, t.Any]]]
@@ -112,15 +115,19 @@
             # the rest of attrs will be saved to __openllm_extras__
             llm = cls._model_mapping[type(llm_config)].from_pretrained(
                 model_id,
                 llm_config=llm_config,
                 **llm_config.__openllm_extras__,
             )
             if ensure_available:
-                logger.debug("'ensure_available=True', make sure model is available within local store.")
+                logger.debug(
+                    "'ensure_available=True', Downloading '%s' with 'model_id=%s' to local model store.",
+                    model_name,
+                    llm.model_id,
+                )
                 llm.ensure_model_id_exists()
             if not return_runner_kwargs:
                 return llm
             return llm, to_runner_attrs
         raise ValueError(
             f"Unrecognized configuration class {llm_config.__class__} for this kind of AutoLLM: {cls.__name__}.\n"
             f"LLM type should be one of {', '.join(c.__name__ for c in cls._model_mapping.keys())}."
```

### Comparing `openllm-0.1.6/src/openllm/models/auto/modeling_auto.py` & `openllm-0.1.7/src/openllm/models/auto/modeling_auto.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,20 +14,21 @@
 
 from __future__ import annotations
 
 import typing as t
 from collections import OrderedDict
 
 from .configuration_auto import CONFIG_MAPPING_NAMES
-from .factory import _BaseAutoLLMClass, _LazyAutoMapping
+from .factory import _BaseAutoLLMClass
+from .factory import _LazyAutoMapping
 
-if t.TYPE_CHECKING:
-    import transformers
 
+if t.TYPE_CHECKING:
     import openllm
+    import transformers
 
 MODEL_MAPPING_NAMES = OrderedDict(
     [
         ("flan_t5", "FlanT5"),
         ("dolly_v2", "DollyV2"),
         ("chatglm", "ChatGLM"),
         ("starcoder", "StarCoder"),
```

### Comparing `openllm-0.1.6/src/openllm/models/auto/modeling_flax_auto.py` & `openllm-0.1.7/src/openllm/models/auto/modeling_flax_auto.py`

 * *Files 9% similar despite different names*

```diff
@@ -14,20 +14,21 @@
 
 from __future__ import annotations
 
 import typing as t
 from collections import OrderedDict
 
 from .configuration_auto import CONFIG_MAPPING_NAMES
-from .factory import _BaseAutoLLMClass, _LazyAutoMapping
+from .factory import _BaseAutoLLMClass
+from .factory import _LazyAutoMapping
 
-if t.TYPE_CHECKING:
-    import transformers
 
+if t.TYPE_CHECKING:
     import openllm
+    import transformers
 
 MODEL_FLAX_MAPPING_NAMES = OrderedDict(
     [
         ("flan_t5", "FlaxFlanT5"),
         ("opt", "FlaxOPT"),
     ]
 )
```

### Comparing `openllm-0.1.6/src/openllm/models/auto/modeling_tf_auto.py` & `openllm-0.1.7/src/openllm/models/auto/modeling_tf_auto.py`

 * *Files 9% similar despite different names*

```diff
@@ -14,20 +14,21 @@
 
 from __future__ import annotations
 
 import typing as t
 from collections import OrderedDict
 
 from .configuration_auto import CONFIG_MAPPING_NAMES
-from .factory import _BaseAutoLLMClass, _LazyAutoMapping
+from .factory import _BaseAutoLLMClass
+from .factory import _LazyAutoMapping
 
-if t.TYPE_CHECKING:
-    import transformers
 
+if t.TYPE_CHECKING:
     import openllm
+    import transformers
 
 MODEL_TF_MAPPING_NAMES = OrderedDict(
     [
         ("flan_t5", "TFFlanT5"),
         ("opt", "TFOPT"),
     ]
 )
```

### Comparing `openllm-0.1.6/src/openllm/models/chatglm/__init__.py` & `openllm-0.1.7/src/openllm/models/chatglm/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 
 from __future__ import annotations
 
 import typing as t
 
 import openllm
 
+
 _import_structure = {
     "configuration_chatglm": ["ChatGLMConfig", "START_CHATGLM_COMMAND_DOCSTRING", "DEFAULT_PROMPT_TEMPLATE"],
 }
 
 try:
     if not openllm.utils.is_torch_available() or not openllm.utils.is_cpm_kernels_available():
         raise openllm.exceptions.MissingDependencyError
```

### Comparing `openllm-0.1.6/src/openllm/models/chatglm/configuration_chatglm.py` & `openllm-0.1.7/src/openllm/models/chatglm/configuration_chatglm.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.6/src/openllm/models/chatglm/modeling_chatglm.py` & `openllm-0.1.7/src/openllm/models/chatglm/modeling_chatglm.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -12,19 +12,19 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from __future__ import annotations
 
 import typing as t
 
 import bentoml
+import openllm
 import transformers
 from transformers.generation.logits_process import LogitsProcessor
 from transformers.generation.utils import LogitsProcessorList
 
-import openllm
 
 if t.TYPE_CHECKING:
     import torch
 else:
     torch = openllm.utils.LazyLoader("torch", globals(), "torch")
```

### Comparing `openllm-0.1.6/src/openllm/models/dolly_v2/__init__.py` & `openllm-0.1.7/src/openllm/models/dolly_v2/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 
 from __future__ import annotations
 
 import typing as t
 
 import openllm
 
+
 _import_structure = {
     "configuration_dolly_v2": ["DollyV2Config", "START_DOLLY_V2_COMMAND_DOCSTRING", "DEFAULT_PROMPT_TEMPLATE"],
 }
 
 try:
     if not openllm.utils.is_torch_available():
         raise openllm.exceptions.MissingDependencyError
```

### Comparing `openllm-0.1.6/src/openllm/models/dolly_v2/configuration_dolly_v2.py` & `openllm-0.1.7/src/openllm/models/dolly_v2/configuration_dolly_v2.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.6/src/openllm/models/dolly_v2/modeling_dolly_v2.py` & `openllm-0.1.7/src/openllm/models/dolly_v2/modeling_dolly_v2.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,35 +14,35 @@
 from __future__ import annotations
 
 import importlib
 import logging
 import typing as t
 
 import bentoml
-import transformers
-
 import openllm
+import transformers
 
 from .configuration_dolly_v2 import DEFAULT_PROMPT_TEMPLATE
 
+
 if t.TYPE_CHECKING:
     import torch
 else:
     torch = openllm.utils.LazyLoader("torch", globals(), "torch")
 
 logger = logging.getLogger(__name__)
 
 
 class DollyV2(openllm.LLM["transformers.Pipeline", "transformers.PreTrainedTokenizer"]):
     __openllm_internal__ = True
 
     @property
     def import_kwargs(self):
         model_kwds = {
-            "device_map": "auto" if torch.cuda.is_available() else None,
+            "device_map": "auto",
             "torch_dtype": torch.bfloat16,
         }
         tokenizer_kwds = {"padding_side": "left"}
         return model_kwds, tokenizer_kwds
 
     def llm_post_init(self):
         self.device = torch.device("cuda" if torch.cuda.is_available() else "cpu")
@@ -66,14 +66,17 @@
             return bentoml.transformers.save_model(
                 tag,
                 pipeline,
                 custom_objects={"tokenizer": tokenizer},
                 external_modules=[importlib.import_module(pipeline.__module__)],
             )
         finally:
+            import gc
+
+            gc.collect()
             if openllm.utils.is_torch_available() and torch.cuda.is_available():
                 torch.cuda.empty_cache()
 
     def sanitize_parameters(
         self,
         prompt: str,
         max_new_tokens: int | None = None,
```

### Comparing `openllm-0.1.6/src/openllm/models/falcon/__init__.py` & `openllm-0.1.7/src/openllm/models/falcon/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 
 from __future__ import annotations
 
 import typing as t
 
 import openllm
 
+
 _import_structure = {
     "configuration_falcon": ["FalconConfig", "START_FALCON_COMMAND_DOCSTRING", "DEFAULT_PROMPT_TEMPLATE"],
 }
 
 try:
     if not openllm.utils.is_torch_available():
         raise openllm.exceptions.MissingDependencyError
```

### Comparing `openllm-0.1.6/src/openllm/models/falcon/configuration_falcon.py` & `openllm-0.1.7/src/openllm/models/falcon/configuration_falcon.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.6/src/openllm/models/falcon/modeling_falcon.py` & `openllm-0.1.7/src/openllm/models/falcon/modeling_falcon.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -14,21 +14,21 @@
 
 from __future__ import annotations
 
 import importlib
 import typing as t
 
 import bentoml
-import transformers
-
 import openllm
+import transformers
 
 from ..._prompt import default_formatter
 from .configuration_falcon import DEFAULT_PROMPT_TEMPLATE
 
+
 if t.TYPE_CHECKING:
     import torch
 else:
     torch = openllm.utils.LazyLoader("torch", globals(), "torch")
 
 
 class Falcon(openllm.LLM["transformers.TextGenerationPipeline", "transformers.PreTrainedTokenizerFast"]):
```

### Comparing `openllm-0.1.6/src/openllm/models/flan_t5/__init__.py` & `openllm-0.1.7/src/openllm/models/flan_t5/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 
 from __future__ import annotations
 
 import typing as t
 
 import openllm
 
+
 _import_structure = {
     "configuration_flan_t5": ["FlanT5Config", "START_FLAN_T5_COMMAND_DOCSTRING", "DEFAULT_PROMPT_TEMPLATE"],
 }
 
 try:
     if not openllm.utils.is_torch_available():
         raise openllm.exceptions.MissingDependencyError
```

### Comparing `openllm-0.1.6/src/openllm/models/flan_t5/configuration_flan_t5.py` & `openllm-0.1.7/src/openllm/models/flan_t5/configuration_flan_t5.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from __future__ import annotations
 
 import openllm
 
+
 START_FLAN_T5_COMMAND_DOCSTRING = """\
 Run a LLMServer for FLAN-T5 model.
 
 \b
 > See more information about FLAN-T5 at [huggingface/transformers](https://huggingface.co/docs/transformers/model_doc/flan-t5)
 
 \b
```

### Comparing `openllm-0.1.6/src/openllm/models/flan_t5/modeling_flan_t5.py` & `openllm-0.1.7/src/openllm/models/flan_t5/modeling_flan_t5.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,16 +16,18 @@
 import typing as t
 
 import openllm
 
 from ..._prompt import default_formatter
 from .configuration_flan_t5 import DEFAULT_PROMPT_TEMPLATE
 
+
 if t.TYPE_CHECKING:
     import torch
+
     import transformers  # noqa
 else:
     torch = openllm.utils.LazyLoader("torch", globals(), "torch")
 
 
 class FlanT5(openllm.LLM["transformers.T5ForConditionalGeneration", "transformers.T5TokenizerFast"]):
     __openllm_internal__ = True
```

### Comparing `openllm-0.1.6/src/openllm/models/flan_t5/modeling_flax_flan_t5.py` & `openllm-0.1.7/src/openllm/models/flan_t5/modeling_flax_flan_t5.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 import typing as t
 
 import openllm
 
 from ..._prompt import default_formatter
 from .configuration_flan_t5 import DEFAULT_PROMPT_TEMPLATE
 
+
 if t.TYPE_CHECKING:
     import transformers  # noqa
 
 
 class FlaxFlanT5(openllm.LLM["transformers.FlaxT5ForConditionalGeneration", "transformers.T5TokenizerFast"]):
     __openllm_internal__ = True
```

### Comparing `openllm-0.1.6/src/openllm/models/flan_t5/modeling_tf_flan_t5.py` & `openllm-0.1.7/src/openllm/models/flan_t5/modeling_tf_flan_t5.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 import typing as t
 
 import openllm
 
 from ..._prompt import default_formatter
 from .configuration_flan_t5 import DEFAULT_PROMPT_TEMPLATE
 
+
 if t.TYPE_CHECKING:
     import transformers  # noqa
 
 
 class TFFlanT5(openllm.LLM["transformers.TFT5ForConditionalGeneration", "transformers.T5TokenizerFast"]):
     __openllm_internal__ = True
```

### Comparing `openllm-0.1.6/src/openllm/models/gpt_neox/__init__.py` & `openllm-0.1.7/src/openllm/models/llama/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.6/src/openllm/models/llama/__init__.py` & `openllm-0.1.7/src/openllm/models/roberta/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.6/src/openllm/models/opt/__init__.py` & `openllm-0.1.7/src/openllm/models/opt/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 
 from __future__ import annotations
 
 import typing as t
 
 import openllm
 
+
 _import_structure = {
     "configuration_opt": ["OPTConfig", "START_OPT_COMMAND_DOCSTRING", "DEFAULT_PROMPT_TEMPLATE"],
 }
 
 try:
     if not openllm.utils.is_torch_available():
         raise openllm.exceptions.MissingDependencyError
```

### Comparing `openllm-0.1.6/src/openllm/models/opt/configuration_opt.py` & `openllm-0.1.7/src/openllm/models/opt/configuration_opt.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.6/src/openllm/models/opt/modeling_flax_opt.py` & `openllm-0.1.7/src/openllm/models/opt/modeling_flax_opt.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -14,20 +14,20 @@
 
 from __future__ import annotations
 
 import logging
 import typing as t
 
 import bentoml
-
 import openllm
 
 from ..._prompt import default_formatter
 from .configuration_opt import DEFAULT_PROMPT_TEMPLATE
 
+
 if t.TYPE_CHECKING:
     import transformers
 else:
     transformers = openllm.utils.LazyLoader("transformers", globals(), "transformers")
 
 logger = logging.getLogger(__name__)
```

### Comparing `openllm-0.1.6/src/openllm/models/opt/modeling_opt.py` & `openllm-0.1.7/src/openllm/models/opt/modeling_opt.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,22 +14,23 @@
 
 from __future__ import annotations
 
 import logging
 import typing as t
 
 import bentoml
-
 import openllm
 
 from ..._prompt import default_formatter
 from .configuration_opt import DEFAULT_PROMPT_TEMPLATE
 
+
 if t.TYPE_CHECKING:
     import torch
+
     import transformers  # noqa
 else:
     torch = openllm.utils.LazyLoader("torch", globals(), "torch")
     transformers = openllm.utils.LazyLoader("transformers", globals(), "transformers")
 
 logger = logging.getLogger(__name__)
```

### Comparing `openllm-0.1.6/src/openllm/models/opt/modeling_tf_opt.py` & `openllm-0.1.7/src/openllm/models/opt/modeling_tf_opt.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -14,20 +14,20 @@
 
 from __future__ import annotations
 
 import logging
 import typing as t
 
 import bentoml
-
 import openllm
 
 from ..._prompt import default_formatter
 from .configuration_opt import DEFAULT_PROMPT_TEMPLATE
 
+
 if t.TYPE_CHECKING:
     import transformers
 else:
     transformers = openllm.utils.LazyLoader("transformers", globals(), "transformers")
 
 
 logger = logging.getLogger(__name__)
```

### Comparing `openllm-0.1.6/src/openllm/models/roberta/__init__.py` & `openllm-0.1.7/src/openllm_client/runtimes/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,8 +8,9 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-raise NotImplementedError("This module is not implemented yet.")
+from .grpc import GrpcClient as GrpcClient
+from .http import HTTPClient as HTTPClient
```

### Comparing `openllm-0.1.6/src/openllm/models/stablelm/__init__.py` & `openllm-0.1.7/src/openllm/models/stablelm/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 
 from __future__ import annotations
 
 import typing as t
 
 import openllm
 
+
 _import_structure = {
     "configuration_stablelm": ["StableLMConfig", "START_STABLELM_COMMAND_DOCSTRING", "DEFAULT_PROMPT_TEMPLATE"],
 }
 
 try:
     if not openllm.utils.is_torch_available():
         raise openllm.exceptions.MissingDependencyError
```

### Comparing `openllm-0.1.6/src/openllm/models/stablelm/configuration_stablelm.py` & `openllm-0.1.7/src/openllm/models/stablelm/configuration_stablelm.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.6/src/openllm/models/stablelm/modeling_stablelm.py` & `openllm-0.1.7/src/openllm/models/stablelm/modeling_stablelm.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,28 +12,30 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from __future__ import annotations
 
 import logging
 import typing as t
 
-from transformers import StoppingCriteria, StoppingCriteriaList
-
 import openllm
+from transformers import StoppingCriteria
+from transformers import StoppingCriteriaList
 
 from ..._prompt import default_formatter
-from .configuration_stablelm import DEFAULT_PROMPT_TEMPLATE, SYSTEM_PROMPT
+from .configuration_stablelm import DEFAULT_PROMPT_TEMPLATE
+from .configuration_stablelm import SYSTEM_PROMPT
+
 
 if t.TYPE_CHECKING:
     import transformers  # noqa
 
 
 class StopOnTokens(StoppingCriteria):
     def __call__(self, input_ids: torch.LongTensor, scores: torch.FloatTensor, **kwargs) -> bool:
-        stop_ids = set([50278, 50279, 50277, 1, 0])
+        stop_ids = {50278, 50279, 50277, 1, 0}
         return input_ids[0][-1] in stop_ids
 
 
 if t.TYPE_CHECKING:
     import torch
 else:
     torch = openllm.utils.LazyLoader("torch", globals(), "torch")
```

### Comparing `openllm-0.1.6/src/openllm/models/starcoder/__init__.py` & `openllm-0.1.7/src/openllm/models/starcoder/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 
 from __future__ import annotations
 
 import typing as t
 
 import openllm
 
+
 _import_structure = {
     "configuration_starcoder": ["StarCoderConfig", "START_STARCODER_COMMAND_DOCSTRING", "DEFAULT_PROMPT_TEMPLATE"],
 }
 
 try:
     if not openllm.utils.is_torch_available():
         raise openllm.exceptions.MissingDependencyError
```

### Comparing `openllm-0.1.6/src/openllm/models/starcoder/configuration_starcoder.py` & `openllm-0.1.7/src/openllm/models/starcoder/configuration_starcoder.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.6/src/openllm/models/starcoder/modeling_starcoder.py` & `openllm-0.1.7/src/openllm/models/starcoder/modeling_starcoder.py`

 * *Files 24% similar despite different names*

```diff
@@ -13,19 +13,22 @@
 # limitations under the License.
 from __future__ import annotations
 
 import logging
 import typing as t
 
 import bentoml
-
 import openllm
 
+from ..._generation import StopSequenceCriteria
+
+
 if t.TYPE_CHECKING:
     import torch
+
     import transformers
 else:
     torch = openllm.utils.LazyLoader("torch", globals(), "torch")
     transformers = openllm.utils.LazyLoader("transformers", globals(), "transformers")
 
 logger = logging.getLogger(__name__)
 
@@ -133,7 +136,26 @@
             # TODO: We will probably want to return the tokenizer here so that we can manually process this
             # return (skip_special_tokens=False, clean_up_tokenization_spaces=False))
             return self.tokenizer.batch_decode(
                 result_tensor[0],
                 skip_special_tokens=True,
                 clean_up_tokenization_spaces=True,
             )
+
+    def generate_one(
+        self, prompt: str, stop: list[str], **preprocess_generate_kwds: t.Any
+    ) -> list[dict[t.Literal["generated_text"], str]]:
+        max_new_tokens = preprocess_generate_kwds.pop("max_new_tokens", 200)
+        encoded_inputs = self.tokenizer(prompt, return_tensors="pt").to(self.device)
+        src_len = encoded_inputs["input_ids"].shape[1]
+        stopping_criteria = preprocess_generate_kwds.pop("stopping_criteria", transformers.StoppingCriteriaList([]))
+        stopping_criteria.append(StopSequenceCriteria(stop, self.tokenizer))
+        outputs = self.model.generate(
+            encoded_inputs["input_ids"], max_new_tokens=max_new_tokens, stopping_criteria=stopping_criteria
+        )
+
+        result = self.tokenizer.decode(outputs[0].tolist()[src_len:])
+        # Inference API returns the stop sequence
+        for stop_seq in stop:
+            if result.endswith(stop_seq):
+                result = result[: -len(stop_seq)]
+        return [{"generated_text": result}]
```

### Comparing `openllm-0.1.6/src/openllm/playground/__init__.py` & `openllm-0.1.7/src/openllm/playground/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.6/src/openllm/playground/features.py` & `openllm-0.1.7/src/openllm/playground/features.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 
 from __future__ import annotations
 
 import logging
 
 import openllm
 
+
 openllm.utils.configure_logging()
 
 logger = logging.getLogger(__name__)
 
 MAX_NEW_TOKENS = 384
 
 Q = "Answer the following question, step by step:\n{q}\nA:"
```

### Comparing `openllm-0.1.6/src/openllm/playground/ft_opt_lora.py` & `openllm-0.1.7/src/openllm/playground/ft_opt_lora.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 import logging
 import os
 import typing as t
 
 # import openllm here for OPENLLMDEVDEBUG
 import openllm
 
+
 openllm.utils.configure_logging()
 
 logger = logging.getLogger(__name__)
 
 if len(openllm.utils.gpu_count()) < 1:
     raise RuntimeError("This script can only be run with system that GPU is available.")
 
@@ -45,17 +46,21 @@
     logger.info("Installing dependencies to run this script: %s", _deps)
 
     if os.system(f"pip install -U {' '.join(_deps)}") != 0:
         raise SystemExit(1)
 
 os.environ["BITSANDBYTES_NOWELCOME"] = str(1)
 
-import transformers
 from datasets import load_dataset
-from peft import LoraConfig, get_peft_model, prepare_model_for_int8_training
+from peft import LoraConfig
+from peft import get_peft_model
+from peft import prepare_model_for_int8_training
+
+import transformers
+
 
 if t.TYPE_CHECKING:
     from peft import PeftModel
 
 DEFAULT_MODEL_ID = "facebook/opt-6.7b"
```

### Comparing `openllm-0.1.6/src/openllm/utils/__init__.py` & `openllm-0.1.7/src/openllm/utils/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -15,34 +15,36 @@
 Utilities function for OpenLLM. User can import these function for convenience, but
 we won't ensure backward compatibility for these functions. So use with caution.
 """
 from __future__ import annotations as _annotations
 
 import functools
 import logging
+import logging.config
 import os
 import sys
 import types
 import typing as t
 
-from bentoml._internal.configuration import (get_debug_mode, get_quiet_mode,
-                                             set_debug_mode, set_quiet_mode)
-from bentoml._internal.log import configure_logging, configure_server_logging
+from bentoml._internal.configuration import get_debug_mode
+from bentoml._internal.configuration import get_quiet_mode
+from bentoml._internal.configuration import set_debug_mode
+from bentoml._internal.configuration import set_quiet_mode
+from bentoml._internal.log import CLI_LOGGING_CONFIG as _CLI_LOGGING_CONFIG
 from bentoml._internal.types import LazyType
-from bentoml._internal.utils import (LazyLoader, bentoml_cattr,
-                                     copy_file_to_fs_folder, first_not_none,
-                                     pkg, reserve_free_port,
-                                     resolve_user_filepath)
+from bentoml._internal.utils import LazyLoader
+from bentoml._internal.utils import bentoml_cattr
+from bentoml._internal.utils import copy_file_to_fs_folder
+from bentoml._internal.utils import first_not_none
+from bentoml._internal.utils import pkg
+from bentoml._internal.utils import reserve_free_port
+from bentoml._internal.utils import resolve_user_filepath
 
 from .lazy import LazyModule
 
-# NOTE: The set marks contains a set of modules name
-# that are available above and are whitelisted
-# to be included in the extra_objects map.
-_whitelist_modules = {"pkg"}
 
 logger = logging.getLogger(__name__)
 
 try:
     from typing import GenericAlias as _TypingGenericAlias  # type: ignore
 except ImportError:
     # python < 3.9 does not have GenericAlias (list[int], tuple[str, ...] and so on)
@@ -84,73 +86,110 @@
     if not hasattr(obj, name):
         _setattr(name, value)
 
 
 DEBUG = sys.flags.dev_mode or (not sys.flags.ignore_environment and bool(os.environ.get("OPENLLMDEVDEBUG")))
 
 
+_LOGGING_CONFIG = _CLI_LOGGING_CONFIG.copy()
+_LOGGING_CONFIG["loggers"].update(
+    {
+        "openllm": {
+            "level": logging.INFO,
+            "handlers": ["bentomlhandler", "defaulthandler"],
+            "propagate": False,
+        }
+    }
+)
+
+
+def configure_logging() -> None:
+    if get_quiet_mode():
+        _LOGGING_CONFIG["loggers"]["openllm"]["level"] = logging.ERROR
+        _LOGGING_CONFIG["loggers"]["bentoml"]["level"] = logging.ERROR
+        _LOGGING_CONFIG["root"]["level"] = logging.ERROR
+    elif get_debug_mode() or DEBUG:
+        _LOGGING_CONFIG["loggers"]["openllm"]["level"] = logging.DEBUG
+        _LOGGING_CONFIG["loggers"]["bentoml"]["level"] = logging.DEBUG
+        _LOGGING_CONFIG["root"]["level"] = logging.DEBUG
+    else:
+        _LOGGING_CONFIG["loggers"]["openllm"]["level"] = logging.INFO
+        _LOGGING_CONFIG["loggers"]["bentoml"]["level"] = logging.INFO
+        _LOGGING_CONFIG["root"]["level"] = logging.INFO
+
+    logging.config.dictConfig(_LOGGING_CONFIG)
+
+
+# NOTE: The set marks contains a set of modules name
+# that are available above and are whitelisted
+# to be included in the extra_objects map.
+_whitelist_modules = {"pkg"}
+
 # XXX: define all classes, functions import above this line
 # since _extras will be the locals() import from this file.
 _extras: dict[str, t.Any] = {
     k: v
     for k, v in locals().items()
     if k in _whitelist_modules or (not isinstance(v, types.ModuleType) and not k.startswith("_"))
 }
 
 _import_structure = {
     "analytics": [],
     "codegen": [],
     "dantic": [],
     "import_utils": [
+        "OPTIONAL_DEPENDENCIES",
         "ENV_VARS_TRUE_VALUES",
         "DummyMetaclass",
         "ModelEnv",
         "is_cpm_kernels_available",
         "is_einops_available",
         "is_flax_available",
         "is_tf_available",
         "is_torch_available",
         "is_bitsandbytes_available",
+        "is_transformers_supports_kbit",
+        "is_transformers_supports_agent",
         "require_backends",
     ],
 }
 
 if t.TYPE_CHECKING:
     # NOTE: The following exports useful utils from bentoml
     from . import LazyLoader as LazyLoader
     from . import LazyType as LazyType
     from . import analytics as analytics
     from . import bentoml_cattr as bentoml_cattr
     from . import codegen as codegen
     from . import configure_logging as configure_logging
-    from . import configure_server_logging as configure_server_logging
     from . import copy_file_to_fs_folder as copy_file_to_fs_folder
     from . import dantic as dantic
     from . import first_not_none as first_not_none
     from . import get_debug_mode as get_debug_mode
     from . import get_quiet_mode as get_quiet_mode
     from . import gpu_count as gpu_count
     from . import lenient_issubclass as lenient_issubclass
     from . import non_intrusive_setattr as non_intrusive_setattr
     from . import pkg as pkg
     from . import reserve_free_port as reserve_free_port
     from . import resolve_user_filepath as resolve_user_filepath
     from . import set_debug_mode as set_debug_mode
     from . import set_quiet_mode as set_quiet_mode
     from .import_utils import ENV_VARS_TRUE_VALUES as ENV_VARS_TRUE_VALUES
+    from .import_utils import OPTIONAL_DEPENDENCIES as OPTIONAL_DEPENDENCIES
     from .import_utils import DummyMetaclass as DummyMetaclass
     from .import_utils import ModelEnv as ModelEnv
-    from .import_utils import \
-        is_bitsandbytes_available as is_bitsandbytes_available
-    from .import_utils import \
-        is_cpm_kernels_available as is_cpm_kernels_available
+    from .import_utils import is_bitsandbytes_available as is_bitsandbytes_available
+    from .import_utils import is_cpm_kernels_available as is_cpm_kernels_available
     from .import_utils import is_einops_available as is_einops_available
     from .import_utils import is_flax_available as is_flax_available
     from .import_utils import is_tf_available as is_tf_available
     from .import_utils import is_torch_available as is_torch_available
+    from .import_utils import is_transformers_supports_agent as is_transformers_supports_agent
+    from .import_utils import is_transformers_supports_kbit as is_transformers_supports_kbit
     from .import_utils import require_backends as require_backends
     from .lazy import LazyModule as LazyModule
 else:
     import sys
 
     sys.modules[__name__] = LazyModule(
         __name__,
```

### Comparing `openllm-0.1.6/src/openllm/utils/analytics.py` & `openllm-0.1.7/src/openllm/utils/analytics.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,22 +20,25 @@
 
 import contextlib
 import functools
 import os
 import typing as t
 
 import attr
+
 from bentoml._internal.utils import analytics as _internal_analytics
 from bentoml._internal.utils.analytics import usage_stats as _internal_usage
 
+
 if t.TYPE_CHECKING:
     import openllm
 
 from ..__about__ import __version__
 
+
 ENV_VARS_TRUE_VALUES = {"1", "ON", "YES", "TRUE"}
 
 # This variable is a proxy that will control BENTOML_DO_NOT_TRACK
 OPENLLM_DO_NOT_TRACK = "OPENLLM_DO_NOT_TRACK"
 
 DO_NOT_TRACK = os.environ.get(OPENLLM_DO_NOT_TRACK, str(False)).upper()
```

### Comparing `openllm-0.1.6/src/openllm/utils/codegen.py` & `openllm-0.1.7/src/openllm/utils/codegen.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 from __future__ import annotations
 
 import logging
 import string
 import typing as t
 from pathlib import Path
 
+
 if t.TYPE_CHECKING:
     from fs.base import FS
 
     DictStrAny = dict[str, t.Any]
 
     from attr import _make_method
 else:
```

### Comparing `openllm-0.1.6/src/openllm/utils/dantic.py` & `openllm-0.1.7/src/openllm/utils/dantic.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,18 +26,22 @@
 import click_option_group as cog
 import inflection
 import orjson
 from click import ParamType
 
 import openllm
 
+
 if t.TYPE_CHECKING:
     from attr import _ValidatorType
 
-    from .._types import ClickFunctionWrapper, F, O_co, P
+    from .._types import ClickFunctionWrapper
+    from .._types import F
+    from .._types import O_co
+    from .._types import P
 
 _T = t.TypeVar("_T")
 
 
 @t.overload
 def attrs_to_options(
     name: str,
```

### Comparing `openllm-0.1.6/src/openllm/utils/dummy_flax_objects.py` & `openllm-0.1.7/src/openllm/utils/dummy_flax_objects.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,15 +12,16 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from __future__ import annotations
 
 import typing as t
 
-from ..utils import DummyMetaclass, require_backends
+from ..utils import DummyMetaclass
+from ..utils import require_backends
 
 
 class FlaxFlanT5(metaclass=DummyMetaclass):
     _backends = ["flax"]
 
     def __init__(self, *args: t.Any, **attrs: t.Any):
         require_backends(self, ["flax"])
```

### Comparing `openllm-0.1.6/src/openllm/utils/dummy_pt_and_cpm_kernels_objects.py` & `openllm-0.1.7/src/openllm/utils/dummy_pt_and_einops_objects.py`

 * *Files 17% similar despite different names*

```diff
@@ -12,15 +12,16 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from __future__ import annotations
 
 import typing as t
 
-from ..utils import DummyMetaclass, require_backends
+from ..utils import DummyMetaclass
+from ..utils import require_backends
 
 
-class ChatGLM(metaclass=DummyMetaclass):
-    _backends = ["torch", "cpm_kernels"]
+class Falcon(metaclass=DummyMetaclass):
+    _backends = ["torch", "einops"]
 
     def __init__(self, *args: t.Any, **attrs: t.Any):
-        require_backends(self, ["torch", "cpm_kernels"])
+        require_backends(self, ["torch", "einops"])
```

### Comparing `openllm-0.1.6/src/openllm/utils/dummy_pt_and_einops_objects.py` & `openllm-0.1.7/src/openllm/utils/dummy_pt_and_cpm_kernels_objects.py`

 * *Files 16% similar despite different names*

```diff
@@ -12,15 +12,16 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from __future__ import annotations
 
 import typing as t
 
-from ..utils import DummyMetaclass, require_backends
+from ..utils import DummyMetaclass
+from ..utils import require_backends
 
 
-class Falcon(metaclass=DummyMetaclass):
-    _backends = ["torch", "einops"]
+class ChatGLM(metaclass=DummyMetaclass):
+    _backends = ["torch", "cpm_kernels"]
 
     def __init__(self, *args: t.Any, **attrs: t.Any):
-        require_backends(self, ["torch", "einops"])
+        require_backends(self, ["torch", "cpm_kernels"])
```

### Comparing `openllm-0.1.6/src/openllm/utils/dummy_pt_objects.py` & `openllm-0.1.7/src/openllm/utils/dummy_pt_objects.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,15 +12,16 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from __future__ import annotations
 
 import typing as t
 
-from ..utils import DummyMetaclass, require_backends
+from ..utils import DummyMetaclass
+from ..utils import require_backends
 
 
 class FlanT5(metaclass=DummyMetaclass):
     _backends = ["torch"]
 
     def __init__(self, *args: t.Any, **attrs: t.Any):
         require_backends(self, ["torch"])
```

### Comparing `openllm-0.1.6/src/openllm/utils/dummy_tf_objects.py` & `openllm-0.1.7/src/openllm/utils/dummy_tf_objects.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,16 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from __future__ import annotations
 
 import typing as t
 
-from ..utils import DummyMetaclass, require_backends
+from ..utils import DummyMetaclass
+from ..utils import require_backends
 
 
 class TFFlanT5(metaclass=DummyMetaclass):
     _backends = ["tf"]
 
     def __init__(self, *args: t.Any, **attrs: t.Any):
         require_backends(self, ["tf"])
```

### Comparing `openllm-0.1.6/src/openllm/utils/import_utils.py` & `openllm-0.1.7/src/openllm/utils/import_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,24 +23,28 @@
 import logging
 import os
 import typing as t
 from abc import ABCMeta
 from collections import OrderedDict
 
 import inflection
-from bentoml._internal.utils import LazyLoader
 from packaging import version
 
+from bentoml._internal.utils import LazyLoader
+from bentoml._internal.utils import pkg
+
+
 if t.TYPE_CHECKING:
     BackendOrderredDict = OrderedDict[str, tuple[t.Callable[[], bool], str]]
 else:
     BackendOrderredDict = OrderedDict
 
 logger = logging.getLogger(__name__)
 
+OPTIONAL_DEPENDENCIES = {"fine-tune", "flan-t5", "openai", "agents"}
 ENV_VARS_TRUE_VALUES = {"1", "ON", "YES", "TRUE"}
 ENV_VARS_TRUE_AND_AUTO_VALUES = ENV_VARS_TRUE_VALUES.union({"AUTO"})
 
 USE_TF = os.environ.get("USE_TF", "AUTO").upper()
 USE_TORCH = os.environ.get("USE_TORCH", "AUTO").upper()
 USE_JAX = os.environ.get("USE_FLAX", "AUTO").upper()
 
@@ -61,14 +65,22 @@
 _tf_available = importlib.util.find_spec("tensorflow") is not None
 _flax_available = importlib.util.find_spec("jax") is not None and importlib.util.find_spec("flax") is not None
 _einops_available = _is_package_available("einops")
 _cpm_kernel_available = _is_package_available("cpm_kernels")
 _bitsandbytes_available = _is_package_available("bitsandbytes")
 
 
+def is_transformers_supports_kbit() -> bool:
+    return pkg.pkg_version_info("transformers")[:2] >= (4, 30)
+
+
+def is_transformers_supports_agent() -> bool:
+    return pkg.pkg_version_info("transformers")[:2] >= (4, 29)
+
+
 def is_einops_available():
     return _einops_available
 
 
 def is_cpm_kernels_available():
     return _cpm_kernel_available
 
@@ -110,17 +122,17 @@
                     "intel-tensorflow-avx512",
                     "tensorflow-rocm",
                     "tensorflow-macos",
                     "tensorflow-aarch64",
                 )
                 _tf_version = None
                 # For the metadata, we have to look for both tensorflow and tensorflow-cpu
-                for pkg in candidates:
+                for _pkg in candidates:
                     try:
-                        _tf_version = importlib.metadata.version(pkg)
+                        _tf_version = importlib.metadata.version(_pkg)
                         break
                     except importlib.metadata.PackageNotFoundError:
                         pass
                 _tf_available = _tf_version is not None
             if _tf_available:
                 if _tf_version and version.parse(_tf_version) < version.parse("2"):
                     logger.info(f"TensorFlow found but with version {_tf_version}. OpenLLM only supports TF 2.x")
```

### Comparing `openllm-0.1.6/src/openllm/utils/lazy.py` & `openllm-0.1.7/src/openllm/utils/lazy.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,16 @@
 import importlib
 import importlib.machinery
 import itertools
 import os
 import types
 import typing as t
 
-from ..exceptions import ForbiddenAttributeError, OpenLLMException
+from ..exceptions import ForbiddenAttributeError
+from ..exceptions import OpenLLMException
 
 
 class UsageNotAllowedError(OpenLLMException):
     """Raised when LazyModule.__getitem__ is forbidden."""
 
 
 class MissingAttributesError(OpenLLMException):
@@ -79,14 +80,15 @@
         # elements of self.__all__ that are not already in the dir.
         for attribute in self.__all__:
             if attribute not in result:
                 result.append(attribute)
         return result
 
     def __getitem__(self, key: str) -> t.Any:
+        # currently, this is reserved to only internal uses and users shouldn't use this.
         if self._objects.get("__openllm_special__") is None:
             raise UsageNotAllowedError(f"'{self._name}' is not allowed to be used as a dict.")
         _special_mapping = self._objects.get("__openllm_special__", {})
         try:
             if key in _special_mapping:
                 return getattr(self, _special_mapping.__getitem__(key))
             raise MissingAttributesError(f"Requested '{key}' is not available in given mapping.")
```

### Comparing `openllm-0.1.6/src/openllm_client/__init__.py` & `openllm-0.1.7/src/openllm_client/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.6/src/openllm_client/_prompt.py` & `openllm-0.1.7/src/openllm_client/_prompt.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 import typing as t
 
 import attr
 
 import openllm
 from openllm._prompt import PromptFormatter
 
+
 if t.TYPE_CHECKING:
     DictStrStr = dict[str, str]
 else:
     DictStrStr = dict
 
 
 # TODO: Support jinja2 template, go template and possible other prompt template engine.
```

### Comparing `openllm-0.1.6/src/openllm_client/runtimes/__init__.py` & `openllm-0.1.7/src/openllm/__about__.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,10 +7,8 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-
-from .grpc import GrpcClient as GrpcClient
-from .http import HTTPClient as HTTPClient
+__version__ = "0.1.7"
```

### Comparing `openllm-0.1.6/src/openllm_client/runtimes/base.py` & `openllm-0.1.7/src/openllm_client/runtimes/base.py`

 * *Files 24% similar despite different names*

```diff
@@ -15,18 +15,20 @@
 from __future__ import annotations
 
 import asyncio
 import typing as t
 from abc import abstractmethod
 from urllib.parse import urljoin
 
-import bentoml
 import httpx
 
+import bentoml
 import openllm
+import transformers
+
 
 if t.TYPE_CHECKING:
     from openllm.models.auto.factory import _BaseAutoLLMClass
 
     class AnnotatedClient(bentoml.client.Client):
         def health(self, *args: t.Any, **attrs: t.Any) -> t.Any:
             ...
@@ -59,26 +61,38 @@
     _api_version: str
     _client_class: type[bentoml.client.Client]
 
     _host: str
     _port: str
 
     __client__: AnnotatedClient | None = None
+    __agent__: transformers.HfAgent | None = None
     __llm__: openllm.LLM[t.Any, t.Any] | None = None
 
     def __init__(self, address: str, timeout: int = 30):
         self._address = address
         self._timeout = timeout
         assert self._host and self._port, "Make sure to setup _host and _port based on your client implementation."
 
     def __init_subclass__(cls, *, client_type: t.Literal["http", "grpc"] = "http", api_version: str = "v1"):
         cls._client_class = bentoml.client.HTTPClient if client_type == "http" else bentoml.client.GrpcClient
         cls._api_version = api_version
 
     @property
+    def _hf_agent(self) -> transformers.HfAgent:
+        if self.__agent__ is None:
+            if not openllm.utils.is_transformers_supports_agent():
+                raise RuntimeError(
+                    "Current 'transformers' does not support Agent."
+                    " Make sure to upgrade to at least 4.29: 'pip install -U \"transformers>=4.29\"'"
+                )
+            self.__agent__ = transformers.HfAgent(urljoin(self._address, "/hf/agent"))
+        return self.__agent__
+
+    @property
     def _metadata(self) -> dict[str, t.Any]:
         if in_async_context():
             return httpx.post(urljoin(self._address, f"/{self._api_version}/metadata")).json()
         return self.call("metadata")
 
     @property
     @abstractmethod
@@ -135,14 +149,18 @@
         return_raw_response = attrs.pop("return_raw_response", False)
         return return_raw_response, *self.llm.sanitize_parameters(prompt, **attrs)
 
     @abstractmethod
     def postprocess(self, result: t.Any) -> openllm.GenerationOutput:
         ...
 
+    @abstractmethod
+    def _run_hf_agent(self, *args: t.Any, **kwargs: t.Any) -> t.Any:
+        ...
+
 
 class BaseClient(ClientMixin):
     def health(self) -> t.Any:
         raise NotImplementedError
 
     @t.overload
     def query(self, prompt: str, *, return_raw_response: t.Literal[False] = ..., **attrs: t.Any) -> str:
@@ -166,14 +184,36 @@
         r = self.postprocess(result)
 
         if return_raw_response:
             return openllm.utils.bentoml_cattr.unstructure(r)
 
         return self.llm.postprocess_generate(prompt, r.responses, **postprocess_kwargs)
 
+    def ask_agent(
+        self,
+        task: str,
+        *,
+        return_code: bool = False,
+        remote: bool = False,
+        agent_type: t.LiteralString = "hf",
+        **attrs: t.Any,
+    ) -> t.Any:
+        if agent_type == "hf":
+            return self._run_hf_agent(task, return_code=return_code, remote=remote, **attrs)
+        else:
+            raise RuntimeError(f"Unknown 'agent_type={agent_type}'")
+
+    def _run_hf_agent(self, *args: t.Any, **kwargs: t.Any) -> t.Any:
+        if len(args) > 1:
+            raise ValueError("'args' should only take one positional argument.")
+        task = kwargs.pop("task", args[0])
+        return_code = kwargs.pop("return_code", False)
+        remote = kwargs.pop("remote", False)
+        return self._hf_agent.run(task, return_code=return_code, remote=remote, **kwargs)
+
     # NOTE: Scikit interface
     def predict(self, prompt: str, **attrs: t.Any) -> t.Any:
         return self.query(prompt, **attrs)
 
     def chat(self, prompt: str, history: list[str], **attrs: t.Any) -> str:
         raise NotImplementedError
 
@@ -203,13 +243,78 @@
         r = self.postprocess(res)
 
         if return_raw_response:
             return openllm.utils.bentoml_cattr.unstructure(r)
 
         return self.llm.postprocess_generate(prompt, r.responses, **postprocess_kwargs)
 
+    async def ask_agent(
+        self,
+        task: str,
+        *,
+        return_code: bool = False,
+        remote: bool = False,
+        agent_type: t.LiteralString = "hf",
+        **attrs: t.Any,
+    ) -> t.Any:
+        """Async version of agent.run"""
+        if agent_type == "hf":
+            return await self._run_hf_agent(task, return_code=return_code, remote=remote, **attrs)
+        else:
+            raise RuntimeError(f"Unknown 'agent_type={agent_type}'")
+
+    async def _run_hf_agent(self, *args: t.Any, **kwargs: t.Any) -> t.Any:
+        if len(args) > 1:
+            raise ValueError("'args' should only take one positional argument.")
+        task = kwargs.pop("task", args[0])
+        return_code = kwargs.pop("return_code", False)
+        remote = kwargs.pop("remote", False)
+
+        from transformers.tools.agents import clean_code_for_run
+        from transformers.tools.agents import get_tool_creation_code
+        from transformers.tools.agents import resolve_tools
+        from transformers.tools.python_interpreter import evaluate
+
+        _hf_agent = self._hf_agent
+
+        prompt = _hf_agent.format_prompt(task)
+        stop = ["Task:"]
+        async with httpx.AsyncClient(timeout=httpx.Timeout(self.timeout)) as client:
+            response = await client.post(
+                _hf_agent.url_endpoint,
+                json={
+                    "inputs": prompt,
+                    "parameters": {"max_new_tokens": 200, "return_full_text": False, "stop": stop},
+                },
+            )
+            if response.status_code != 200:
+                raise ValueError(f"Error {response.status_code}: {response.json()}")
+
+        result = response.json()[0]["generated_text"]
+        # Inference API returns the stop sequence
+        for stop_seq in stop:
+            if result.endswith(stop_seq):
+                result = result[: -len(stop_seq)]
+                break
+
+        # the below have the same logic as agent.run API
+        explanation, code = clean_code_for_run(result)
+
+        _hf_agent.log(f"==Explanation from the agent==\n{explanation}")
+
+        _hf_agent.log(f"\n\n==Code generated by the agent==\n{code}")
+        if not return_code:
+            _hf_agent.log("\n\n==Result==")
+            _hf_agent.cached_tools = resolve_tools(
+                code, _hf_agent.toolbox, remote=remote, cached_tools=_hf_agent.cached_tools
+            )
+            return evaluate(code, _hf_agent.cached_tools, state=kwargs.copy())
+        else:
+            tool_code = get_tool_creation_code(code, _hf_agent.toolbox, remote=remote)
+            return f"{tool_code}\n{code}"
+
     # NOTE: Scikit interface
     async def predict(self, prompt: str, **attrs: t.Any) -> t.Any:
         return await self.query(prompt, **attrs)
 
     def chat(self, prompt: str, history: list[str], **attrs: t.Any) -> str:
         raise NotImplementedError
```

### Comparing `openllm-0.1.6/src/openllm_client/runtimes/grpc.py` & `openllm-0.1.7/src/openllm_client/runtimes/grpc.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,18 +18,21 @@
 import logging
 import typing as t
 
 import orjson
 
 import openllm
 
-from .base import BaseAsyncClient, BaseClient
+from .base import BaseAsyncClient
+from .base import BaseClient
+
 
 if t.TYPE_CHECKING:
     import grpc_health.v1.health_pb2 as health_pb2
+
     from bentoml.grpc.v1.service_pb2 import Response
 
 logger = logging.getLogger(__name__)
 
 
 class GrpcClientMixin:
     _metadata: Response
```

### Comparing `openllm-0.1.6/src/openllm_client/runtimes/http.py` & `openllm-0.1.7/src/openllm_client/runtimes/http.py`

 * *Files 7% similar despite different names*

```diff
@@ -18,15 +18,17 @@
 import typing as t
 from urllib.parse import urlparse
 
 import orjson
 
 import openllm
 
-from .base import BaseAsyncClient, BaseClient
+from .base import BaseAsyncClient
+from .base import BaseClient
+
 
 logger = logging.getLogger(__name__)
 
 
 class HTTPClientMixin:
     _metadata: dict[str, t.Any]
```

### Comparing `openllm-0.1.6/tests/__init__.py` & `openllm-0.1.7/tests/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,13 +9,15 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import os
 
-from hypothesis import HealthCheck, settings
+from hypothesis import HealthCheck
+from hypothesis import settings
+
 
 settings.register_profile("CI", settings(suppress_health_check=[HealthCheck.too_slow]), deadline=None)
 
 if "CI" in os.environ:
     settings.load_profile("CI")
```

### Comparing `openllm-0.1.6/tests/test_configuration.py` & `openllm-0.1.7/tests/test_configuration.py`

 * *Files 9% similar despite different names*

```diff
@@ -15,23 +15,27 @@
 """All configuration-related tests for openllm.LLMConfig. This will include testing
 for ModelEnv construction and parsing environment variables."""
 from __future__ import annotations
 
 import logging
 
 import pytest
-from hypothesis import assume, given
+from hypothesis import assume
+from hypothesis import given
 from hypothesis import strategies as st
 
 import openllm
-from openllm._configuration import (GenerationConfig, ModelSettings,
-                                    _field_env_key)
+from openllm._configuration import GenerationConfig
+from openllm._configuration import ModelSettings
+from openllm._configuration import _field_env_key
 from openllm.utils import DEBUG
 
-from ._strategies._configuration import make_llm_config, model_settings
+from ._strategies._configuration import make_llm_config
+from ._strategies._configuration import model_settings
+
 
 logger = logging.getLogger(__name__)
 
 
 def test_missing_default():
     with pytest.raises(ValueError, match="Either 'default_id' or 'model_ids'*"):
         make_llm_config("MissingDefaultId", {"name_type": "lowercase", "requirements": ["bentoml"]})
```

### Comparing `openllm-0.1.6/tests/_strategies/__init__.py` & `openllm-0.1.7/tests/_strategies/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.6/tests/_strategies/_configuration.py` & `openllm-0.1.7/tests/_strategies/_configuration.py`

 * *Files 19% similar despite different names*

```diff
@@ -18,36 +18,37 @@
 import typing as t
 
 from hypothesis import strategies as st
 
 import openllm
 from openllm._configuration import ModelSettings
 
+
 logger = logging.getLogger(__name__)
 
 env_strats = st.sampled_from([openllm.utils.ModelEnv(model_name) for model_name in openllm.CONFIG_MAPPING.keys()])
 
 
 @st.composite
 def model_settings(draw: st.DrawFn):
     """Strategy for generating ModelSettings objects."""
-    kwargs: dict[str, t.Any] = dict(
-        default_id=st.text(min_size=1),
-        model_ids=st.lists(st.text(), min_size=1),
-        url=st.text(),
-        requires_gpu=st.booleans(),
-        trust_remote_code=st.booleans(),
-        requirements=st.none() | st.lists(st.text(), min_size=1),
-        use_pipeline=st.booleans(),
-        model_type=st.sampled_from(["causal_lm", "seq2seq_lm"]),
-        runtime=st.sampled_from(["transformers", "cpp"]),
-        name_type=st.sampled_from(["dasherize", "lowercase"]),
-        timeout=st.integers(min_value=3600),
-        workers_per_resource=st.one_of(st.integers(min_value=1), st.floats(min_value=0.1, max_value=1.0)),
-    )
+    kwargs: dict[str, t.Any] = {
+        "default_id": st.text(min_size=1),
+        "model_ids": st.lists(st.text(), min_size=1),
+        "url": st.text(),
+        "requires_gpu": st.booleans(),
+        "trust_remote_code": st.booleans(),
+        "requirements": st.none() | st.lists(st.text(), min_size=1),
+        "use_pipeline": st.booleans(),
+        "model_type": st.sampled_from(["causal_lm", "seq2seq_lm"]),
+        "runtime": st.sampled_from(["transformers", "cpp"]),
+        "name_type": st.sampled_from(["dasherize", "lowercase"]),
+        "timeout": st.integers(min_value=3600),
+        "workers_per_resource": st.one_of(st.integers(min_value=1), st.floats(min_value=0.1, max_value=1.0)),
+    }
     return draw(st.builds(ModelSettings, **kwargs))
 
 
 def make_llm_config(
     cls_name: str,
     dunder_config: dict[str, t.Any] | ModelSettings,
     fields: tuple[tuple[t.LiteralString, str, t.Any], ...] | None = None,
@@ -63,15 +64,15 @@
     if fields is not None:
         for field, type_, default in fields:
             lines.append(f"    {field}: {type_} = {repr(default)}")
     if generation_fields is not None:
         generation_lines = ["class GenerationConfig:"]
         for field, default in generation_fields:
             generation_lines.append(f"    {field} = {repr(default)}")
-        lines.extend(map(lambda line: "    " + line, generation_lines))
+        lines.extend(("    " + line for line in generation_lines))
 
     script = "\n".join(lines)
 
     if openllm.utils.DEBUG:
         logger.info("Generated class %s:\n%s", cls_name, script)
 
     eval(compile(script, "name", "exec"), globs)
```

### Comparing `openllm-0.1.6/tests/models/flan_t5/__init__.py` & `openllm-0.1.7/tests/models/flan_t5/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.6/tests/models/flan_t5/test_modeling_flan_t5.py` & `openllm-0.1.7/tests/models/flan_t5/test_modeling_flan_t5.py`

 * *Files 12% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 
 @pytest.fixture
 def flan_t5_id() -> str:
     return "google/flan-t5-small"
 
 
 def test_small_flan(qa_prompt: str, flan_t5_id: str):
-    llm = openllm.AutoLLM.for_model("flan-t5", model_id=flan_t5_id)
+    llm = openllm.AutoLLM.for_model("flan-t5", model_id=flan_t5_id, ensure_available=True)
     generate = llm(qa_prompt)
     assert generate
 
 
 def test_small_runner_flan(qa_prompt: str, flan_t5_id: str):
     llm = openllm.Runner("flan-t5", model_id=flan_t5_id, init_local=True)
     generate = llm(qa_prompt)
```

### Comparing `openllm-0.1.6/tests/models/opt/__init__.py` & `openllm-0.1.7/tests/models/opt/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.6/tests/models/opt/test_modeling_opt.py` & `openllm-0.1.7/tests/models/opt/test_modeling_opt.py`

 * *Files 8% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
 @pytest.fixture
 def opt_id() -> str:
     return "facebook/opt-125m"
 
 
 def test_small_opt(qa_prompt: str, opt_id: str):
-    llm = openllm.AutoLLM.for_model("opt", model_id=opt_id)
+    llm = openllm.AutoLLM.for_model("opt", model_id=opt_id, ensure_available=True)
     generate = llm(qa_prompt)
     assert generate
 
 
 def test_small_runner_opt(qa_prompt: str, opt_id: str):
     llm = openllm.Runner("opt", model_id=opt_id, init_local=True)
     generate = llm(qa_prompt)
```

### Comparing `openllm-0.1.6/tools/assert-model-table-latest` & `openllm-0.1.7/tools/assert-model-table-latest`

 * *Files identical despite different names*

### Comparing `openllm-0.1.6/tools/run-release-action` & `openllm-0.1.7/tools/run-release-action`

 * *Files identical despite different names*

### Comparing `openllm-0.1.6/tools/update-readme.py` & `openllm-0.1.7/tools/update-readme.py`

 * *Files identical despite different names*

### Comparing `openllm-0.1.6/typings/attr/__init__.pyi` & `openllm-0.1.7/typings/attr/__init__.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -1,40 +1,39 @@
 from __future__ import annotations
 
 import enum
 import sys
-from typing import (
-    Any,
-    Callable,
-    Dict,
-    Generic,
-    List,
-    Literal,
-    Mapping,
-    Optional,
-    ParamSpec,
-    Protocol,
-    Sequence,
-    Tuple,
-    Type,
-    TypeGuard,
-    TypeVar,
-    Union,
-    overload,
-)
+from typing import Any
+from typing import Callable
+from typing import Dict
+from typing import Generic
+from typing import List
+from typing import Literal
+from typing import Mapping
+from typing import Optional
+from typing import ParamSpec
+from typing import Protocol
+from typing import Sequence
+from typing import Tuple
+from typing import Type
+from typing import TypeGuard
+from typing import TypeVar
+from typing import Union
+from typing import overload
 
 from . import converters as converters
 from . import exceptions as exceptions
 from . import filters as filters
 from . import setters as setters
 from . import validators as validators
 from ._cmp import cmp_using as cmp_using
 from ._typing_compat import AttrsInstance_
 from ._version_info import VersionInfo
 
+
 if sys.version_info >= (3, 10): ...
 else: ...
 __version__: str
 __version_info__: VersionInfo
 __title__: str
 __description__: str
 __url__: str
```

### Comparing `openllm-0.1.6/typings/attr/exceptions.pyi` & `openllm-0.1.7/typings/attr/exceptions.pyi`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from typing import Any
 
+
 class FrozenError(AttributeError):
     msg: str = ...
 
 class FrozenInstanceError(FrozenError): ...
 class FrozenAttributeError(FrozenError): ...
 class AttrsAttributeNotFoundError(ValueError): ...
 class NotAnAttrsClassError(ValueError): ...
```

### Comparing `openllm-0.1.6/typings/attr/validators.pyi` & `openllm-0.1.7/typings/attr/validators.pyi`

 * *Files 16% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-from typing import (
-    Any,
-    AnyStr,
-    Callable,
-    Container,
-    ContextManager,
-    Iterable,
-    List,
-    Mapping,
-    Match,
-    Optional,
-    Pattern,
-    Tuple,
-    Type,
-    TypeVar,
-    Union,
-    overload,
-)
+from typing import Any
+from typing import AnyStr
+from typing import Callable
+from typing import Container
+from typing import ContextManager
+from typing import Iterable
+from typing import List
+from typing import Mapping
+from typing import Match
+from typing import Optional
+from typing import Pattern
+from typing import Tuple
+from typing import Type
+from typing import TypeVar
+from typing import Union
+from typing import overload
+
+from . import _ValidatorArgType
+from . import _ValidatorType
 
-from . import _ValidatorArgType, _ValidatorType
 
 _T = TypeVar("_T")
 _T1 = TypeVar("_T1")
 _T2 = TypeVar("_T2")
 _T3 = TypeVar("_T3")
 _I = TypeVar("_I", bound=Iterable)
 _K = TypeVar("_K")
```

### Comparing `openllm-0.1.6/typings/click_option_group/__init__.pyi` & `openllm-0.1.7/typings/click_option_group/__init__.pyi`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,18 @@
-from ._core import (
-    AllOptionGroup,
-    GroupedOption,
-    MutuallyExclusiveOptionGroup,
-    OptionGroup,
-    RequiredAllOptionGroup,
-    RequiredAnyOptionGroup,
-    RequiredMutuallyExclusiveOptionGroup,
-)
+from ._core import AllOptionGroup
+from ._core import GroupedOption
+from ._core import MutuallyExclusiveOptionGroup
+from ._core import OptionGroup
+from ._core import RequiredAllOptionGroup
+from ._core import RequiredAnyOptionGroup
+from ._core import RequiredMutuallyExclusiveOptionGroup
 from ._decorators import optgroup
 from ._version import __version__
 
+
 """
 click-option-group
 ~~~~~~~~~~~~~~~~~~
 
 Option groups missing in Click
 
 :copyright: © 2019-2020 by Eugene Prilepin
```

### Comparing `openllm-0.1.6/typings/click_option_group/_core.pyi` & `openllm-0.1.7/typings/click_option_group/_core.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,21 @@
 from collections.abc import Callable
-from typing import Any, Dict, List, Mapping, Optional, Sequence, Set, Tuple, Union
+from typing import Any
+from typing import Dict
+from typing import List
+from typing import Mapping
+from typing import Optional
+from typing import Sequence
+from typing import Set
+from typing import Tuple
+from typing import Union
 
 import click
 
+
 FC = Union[Callable[..., Any], click.Command]
 
 class GroupedOption(click.Option):
     """Represents grouped (related) optional values
 
     The class should be used only with `OptionGroup` class for creating grouped options.
```

### Comparing `openllm-0.1.6/typings/click_option_group/_decorators.pyi` & `openllm-0.1.7/typings/click_option_group/_decorators.pyi`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,24 @@
-from typing import Any, Callable, Dict, NamedTuple, Optional, ParamSpec, Protocol, Tuple, Type, TypeVar
+from typing import Any
+from typing import Callable
+from typing import Dict
+from typing import Generic
+from typing import NamedTuple
+from typing import Optional
+from typing import ParamSpec
+from typing import Protocol
+from typing import Tuple
+from typing import Type
+from typing import TypeVar
 
 import click
 
-from ._core import FC, OptionGroup
+from ._core import FC
+from ._core import OptionGroup
+
 
 P = ParamSpec("P")
 O_co = TypeVar("O_co", covariant=True)
 
 F = Callable[P, O_co]
 
 class OptionStackItem(NamedTuple):
@@ -26,15 +38,15 @@
 
     Raises TypeError if not attached options exist.
     """
 
     def __init__(self, param_decls: Any = ..., *, all_not_attached_options: Any, **attrs: Any) -> None: ...
     def handle_parse_result(self, ctx: click.Context, opts: Any, args: tuple[Any]) -> Any: ...
 
-class _OptGroup:
+class _OptGroup(Generic[O_co]):
     """A helper class to manage creating groups and group options via decorators
 
     The class provides two decorator-methods: `group`/`__call__` and `option`.
     These decorators should be used for adding grouped options. The class have
     single global instance `optgroup` that should be used in most cases.
 
     The example of usage::
@@ -94,8 +106,8 @@
         All options will be registered by `group` decorator.
 
         :param param_decls: option declaration tuple
         :param attrs: additional option attributes and parameters
         """
         ...
 
-optgroup: _OptGroup = ...
+optgroup: _OptGroup[Any] = ...
```

### Comparing `openllm-0.1.6/typings/click_option_group/_helpers.pyi` & `openllm-0.1.7/typings/click_option_group/_helpers.pyi`

 * *Files 27% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 """
 This type stub file was generated by pyright.
 """
 
 import collections.abc as abc
-from typing import List, Tuple
+from typing import List
+from typing import Tuple
 
 import click
 
+
 FAKE_OPT_NAME_LEN = ...
 
 def get_callback_and_params(func) -> Tuple[abc.Callable, List[click.Option]]:
     """Returns callback function and its parameters list
 
     :param func: decorated function or click Command
     :return: (callback, params)
```

### Comparing `openllm-0.1.6/typings/deepmerge/merger.pyi` & `openllm-0.1.7/typings/deepmerge/merger.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 from typing import Any
 from typing import Dict
 from typing import List
 from typing import Tuple
 from typing import Union
 
-from .strategy.set import SetStrategies
 from .strategy.core import StrategyList
 from .strategy.dict import DictStrategies
 from .strategy.list import ListStrategies
+from .strategy.set import SetStrategies
+
 
 ConfigDictType = Dict[str, Any]
 
 class Merger:
     PROVIDED_TYPE_STRATEGIES: Dict[type, Union[ListStrategies, DictStrategies, SetStrategies]] = ...
 
     def __init__(
```

### Comparing `openllm-0.1.6/typings/deepmerge/strategy/core.pyi` & `openllm-0.1.7/typings/deepmerge/strategy/core.pyi`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from typing import Any
-from typing import List
-from typing import Union
 from typing import Callable
+from typing import List
 from typing import Optional
+from typing import Union
+
 
 _StringOrFunction = Union[str, Callable[..., Any]]
 STRATEGY_END: object = ...
 
 class StrategyList:
     NAME: Optional[str] = ...
     def __init__(self, strategy_list: Union[_StringOrFunction, List[_StringOrFunction]]) -> None: ...
```

### Comparing `openllm-0.1.6/typings/deepmerge/strategy/set.pyi` & `openllm-0.1.7/typings/deepmerge/strategy/set.pyi`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from typing import Any
 
-from .core import StrategyList
 from ..merger import Merger
+from .core import StrategyList
+
 
 class SetStrategies(StrategyList):
     NAME = ...
 
     @staticmethod
     def strategy_union(config: Any, path: str, base: StrategyList, nxt: StrategyList) -> StrategyList: ...
     @staticmethod
```

### Comparing `openllm-0.1.6/.gitignore` & `openllm-0.1.7/.gitignore`

 * *Files identical despite different names*

### Comparing `openllm-0.1.6/LICENSE.md` & `openllm-0.1.7/LICENSE.md`

 * *Files identical despite different names*

### Comparing `openllm-0.1.6/README.md` & `openllm-0.1.7/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+![Banner for OpenLLM](/assets/main-banner.png)
+
 <div align="center">
     <h1 align="center">🦾 OpenLLM</h1>
     <a href="https://pypi.org/project/openllm">
         <img src="https://img.shields.io/pypi/v/openllm.svg" alt="pypi_status" />
     </a><a href="https://github.com/bentoml/OpenLLM/actions/workflows/ci.yml">
         <img src="https://github.com/bentoml/OpenLLM/actions/workflows/ci.yml/badge.svg?branch=main" alt="ci" />
     </a><a href="https://twitter.com/bentomlai">
@@ -12,27 +14,27 @@
     <p>An open platform for operating large language models (LLMs) in production.</br>
     Fine-tune, serve, deploy, and monitor any LLMs with ease.</p>
     <i></i>
 </div>
 
 ## 📖 Introduction
 
-With OpenLLM, you can run inference with any open-source large-language
-models (LLMs), deploy to the cloud or on-premises, and build powerful AI apps.
+With OpenLLM, you can run inference with any open-source large-language models,
+deploy to the cloud or on-premises, and build powerful AI apps.
 
-🚂 **SOTA LLMs**: built-in supports a wide range of open-source LLMs and model
-runtime, including StableLM, Falcon, Dolly, Flan-T5, ChatGLM, StarCoder and
-more.
+🚂 **State-of-the-art LLMs**: built-in supports a wide range of open-source LLMs
+and model runtime, including StableLM, Falcon, Dolly, Flan-T5, ChatGLM,
+StarCoder and more.
 
 🔥 **Flexible APIs**: serve LLMs over RESTful API or gRPC with one command,
 query via WebUI, CLI, our Python/Javascript client, or any HTTP client.
 
-⛓️ **Freedom To Build**: First-class support for LangChain and BentoML allows you
-to easily create your own AI apps by composing LLMs with other models and
-services.
+⛓️ **Freedom To Build**: First-class support for LangChain, BentoML and
+HuggingFace that allows you to easily create your own AI apps by composing LLMs
+with other models and services.
 
 🎯 **Streamline Deployment**: Automatically generate your LLM server Docker
 Images or deploy as serverless endpoint via
 [☁️ BentoCloud](https://l.bentoml.com/bento-cloud).
 
 🤖️ **Bring your own LLM**: Fine-tune any LLM to suit your needs with
 `LLM.tuning()`. (Coming soon)
@@ -290,15 +292,15 @@
 For example, if you want to use the Tensorflow (`tf`) implementation for the
 `flan-t5` model, you can use the following command:
 
 ```bash
 OPENLLM_FLAN_T5_FRAMEWORK=tf openllm start flan-t5
 ```
 
-> For GPU support on Flax, refers to
+> **Note** For GPU support on Flax, refers to
 > [Jax's installation](https://github.com/google/jax#pip-installation-gpu-cuda-installed-via-pip-easier)
 > to make sure that you have Jax support for the corresponding CUDA version.
 
 ### Integrating a New Model
 
 OpenLLM encourages contributions by welcoming users to incorporate their custom
 LLMs into the ecosystem. Check out
@@ -335,14 +337,48 @@
 
 @svc.api(input=Text(), output=Text())
 async def prompt(input_text: str) -> str:
     answer = await llm_runner.generate(input_text)
     return answer
 ```
 
+### HuggingFace Agents
+
+OpenLLM seamlessly integrates with HuggingFace Agents.
+
+> **Warning** The HuggingFace Agent is still at experimental stage. It is
+> recommended to OpenLLM with
+> `pip install -r nightly-requirements.generated.txt` to get the latest API
+> update for HuggingFace agent.
+
+```python
+import transformers
+
+agent = transformers.HfAgent("http://localhost:3000/hf/agent")  # URL that runs the OpenLLM server
+
+agent.run("Is the following `text` positive or negative?", text="I don't like how this models is generate inputs")
+```
+
+> **Note** Only `starcoder` is currently supported with Agent integration. The
+> example aboved was also ran with four T4s on EC2 `g4dn.12xlarge`
+
+If you want to use OpenLLM client to ask questions to the running agent, you can
+also do so:
+
+```python
+import openllm
+
+client = openllm.client.HTTPClient("http://localhost:3000")
+
+client.ask_agent(
+    task="Is the following `text` positive or negative?",
+    text="What are you thinking about?",
+)
+```
+
 ### LangChain (⏳Coming Soon!)
 
 In future LangChain releases, you'll be able to effortlessly invoke OpenLLM
 models, like so:
 
 ```python
 from langchain.llms import OpenLLM
@@ -373,15 +409,15 @@
    A
    [Bento](https://docs.bentoml.org/en/latest/concepts/bento.html#what-is-a-bento),
    in BentoML, is the unit of distribution. It packages your program's source
    code, models, files, artifacts, and dependencies.
 
 2. **Containerize your Bento**
 
-   ```
+   ```bash
    bentoml containerize <name:version>
    ```
 
    BentoML offers a comprehensive set of options for deploying and hosting
    online ML services in production. To learn more, check out the
    [Deploying a Bento](https://docs.bentoml.org/en/latest/concepts/deploy.html)
    guide.
```

#### html2text {}

```diff
@@ -1,24 +1,25 @@
+![Banner for OpenLLM](/assets/main-banner.png)
                           ****** ð¦¾ OpenLLM ******
                       [pypi_status][ci][Twitter][Discord]
   An open platform for operating large language models (LLMs) in production.
            Fine-tune, serve, deploy, and monitor any LLMs with ease.
 ## ð Introduction With OpenLLM, you can run inference with any open-source
-large-language models (LLMs), deploy to the cloud or on-premises, and build
-powerful AI apps. ð **SOTA LLMs**: built-in supports a wide range of open-
-source LLMs and model runtime, including StableLM, Falcon, Dolly, Flan-T5,
+large-language models, deploy to the cloud or on-premises, and build powerful
+AI apps. ð **State-of-the-art LLMs**: built-in supports a wide range of
+open-source LLMs and model runtime, including StableLM, Falcon, Dolly, Flan-T5,
 ChatGLM, StarCoder and more. ð¥ **Flexible APIs**: serve LLMs over RESTful
 API or gRPC with one command, query via WebUI, CLI, our Python/Javascript
 client, or any HTTP client. âï¸ **Freedom To Build**: First-class support
-for LangChain and BentoML allows you to easily create your own AI apps by
-composing LLMs with other models and services. ð¯ **Streamline Deployment**:
-Automatically generate your LLM server Docker Images or deploy as serverless
-endpoint via [âï¸ BentoCloud](https://l.bentoml.com/bento-cloud). ð¤ï¸
-**Bring your own LLM**: Fine-tune any LLM to suit your needs with `LLM.tuning
-()`. (Coming soon) ![Gif showing OpenLLM Intro](/assets/output.gif)
+for LangChain, BentoML and HuggingFace that allows you to easily create your
+own AI apps by composing LLMs with other models and services. ð¯ **Streamline
+Deployment**: Automatically generate your LLM server Docker Images or deploy as
+serverless endpoint via [âï¸ BentoCloud](https://l.bentoml.com/bento-cloud).
+ð¤ï¸ **Bring your own LLM**: Fine-tune any LLM to suit your needs with
+`LLM.tuning()`. (Coming soon) ![Gif showing OpenLLM Intro](/assets/output.gif)
 ## ðâ Getting Started To use OpenLLM, you need to have Python 3.8 (or
 newer) and `pip` installed on your system. We highly recommend using a Virtual
 Environment to prevent package conflicts. You can install OpenLLM using pip as
 follows: ```bash pip install openllm ``` To verify if it's installed correctly,
 run: ``` $ openllm -h Usage: openllm [OPTIONS] COMMAND [ARGS]...
 âââââââ âââââââ
 ââââââââââââ ââââââ âââ ââââ
@@ -92,62 +93,75 @@
  ### Runtime Implementations (Experimental) Different LLMs may have multiple
 runtime implementations. For instance, they might use Pytorch (`pt`),
 Tensorflow (`tf`), or Flax (`flax`). If you wish to specify a particular
 runtime for a model, you can do so by setting the `OPENLLM_
 {MODEL_NAME}_FRAMEWORK={runtime}` environment variable before running `openllm
 start`. For example, if you want to use the Tensorflow (`tf`) implementation
 for the `flan-t5` model, you can use the following command: ```bash
-OPENLLM_FLAN_T5_FRAMEWORK=tf openllm start flan-t5 ``` > For GPU support on
-Flax, refers to > [Jax's installation](https://github.com/google/jax#pip-
-installation-gpu-cuda-installed-via-pip-easier) > to make sure that you have
-Jax support for the corresponding CUDA version. ### Integrating a New Model
-OpenLLM encourages contributions by welcoming users to incorporate their custom
-LLMs into the ecosystem. Check out [Adding a New Model Guide](https://
+OPENLLM_FLAN_T5_FRAMEWORK=tf openllm start flan-t5 ``` > **Note** For GPU
+support on Flax, refers to > [Jax's installation](https://github.com/google/
+jax#pip-installation-gpu-cuda-installed-via-pip-easier) > to make sure that you
+have Jax support for the corresponding CUDA version. ### Integrating a New
+Model OpenLLM encourages contributions by welcoming users to incorporate their
+custom LLMs into the ecosystem. Check out [Adding a New Model Guide](https://
 github.com/bentoml/OpenLLM/blob/main/ADDING_NEW_MODEL.md) to see how you can do
 it yourself. ## âï¸ Integrations OpenLLM is not just a standalone product;
 it's a building block designed to easily integrate with other powerful tools.
 We currently offer integration with [BentoML](https://github.com/bentoml/
 BentoML) and [LangChain](https://github.com/hwchase17/langchain). ### BentoML
 OpenLLM models can be integrated as a [Runner](https://docs.bentoml.org/en/
 latest/concepts/runner.html) in your BentoML service. These runners have a
 `generate` method that takes a string as a prompt and returns a corresponding
 output string. This will allow you to plug and play any OpenLLM models with
 your existing ML workflow. ```python import bentoml import openllm model =
 "dolly-v2" llm_config = openllm.AutoConfig.for_model(model) llm_runner =
 openllm.Runner(model, llm_config=llm_config) svc = bentoml.Service( name=f"llm-
 dolly-v2-service", runners=[llm_runner] ) @svc.api(input=Text(), output=Text())
 async def prompt(input_text: str) -> str: answer = await llm_runner.generate
-(input_text) return answer ``` ### LangChain (â³Coming Soon!) In future
-LangChain releases, you'll be able to effortlessly invoke OpenLLM models, like
-so: ```python from langchain.llms import OpenLLM llm = OpenLLM.for_model
-(model_name='flan-t5') llm("What is the difference between a duck and a
-goose?") ``` if you have an OpenLLM server deployed elsewhere, you can connect
-to it by specifying its URL: ```python from langchain.llms import OpenLLM llm =
-OpenLLM.for_model(server_url='http://localhost:8000', server_type='http') llm
-("What is the difference between a duck and a goose?") ``` ## ð Deploying to
-Production To deploy your LLMs into production: 1. **Building a Bento**: With
-OpenLLM, you can easily build a Bento for a specific model, like `dolly-v2`,
-using the `build` command.: ```bash openllm build dolly-v2 ``` A [Bento](https:
-//docs.bentoml.org/en/latest/concepts/bento.html#what-is-a-bento), in BentoML,
-is the unit of distribution. It packages your program's source code, models,
-files, artifacts, and dependencies. 2. **Containerize your Bento** ``` bentoml
-containerize  ``` BentoML offers a comprehensive set of options for deploying
-and hosting online ML services in production. To learn more, check out the
-[Deploying a Bento](https://docs.bentoml.org/en/latest/concepts/deploy.html)
-guide. ## ð Telemetry OpenLLM collects usage data to enhance user experience
-and improve the product. We only report OpenLLM's internal API calls and ensure
-maximum privacy by excluding sensitive information. We will never collect user
-code, model data, or stack traces. For usage tracking, check out the [code](./
-src/openllm/utils/analytics.py). You can opt-out of usage tracking by using the
-`--do-not-track` CLI option: ```bash openllm [command] --do-not-track ``` Or by
-setting environment variable `OPENLLM_DO_NOT_TRACK=True`: ```bash export
-OPENLLM_DO_NOT_TRACK=True ``` ## ð¥ Community Engage with like-minded
-individuals passionate about LLMs, AI, and more on our [Discord](https://
-l.bentoml.com/join-openllm-discord)! OpenLLM is actively maintained by the
-BentoML team. Feel free to reach out and join us in our pursuit to make LLMs
-more accessible and easy-to-useð [Join our Slack community!](https://
-l.bentoml.com/join-slack) ## ð Contributing We welcome contributions! If
-you're interested in enhancing OpenLLM's capabilities or have any questions,
-don't hesitate to reach out in our [discord channel](https://l.bentoml.com/
-join-openllm-discord). Checkout our [Developer Guide](https://github.com/
-bentoml/OpenLLM/blob/main/DEVELOPMENT.md) if you wish to contribute to
-OpenLLM's codebase.
+(input_text) return answer ``` ### HuggingFace Agents OpenLLM seamlessly
+integrates with HuggingFace Agents. > **Warning** The HuggingFace Agent is
+still at experimental stage. It is > recommended to OpenLLM with > `pip install
+-r nightly-requirements.generated.txt` to get the latest API > update for
+HuggingFace agent. ```python import transformers agent = transformers.HfAgent
+("http://localhost:3000/hf/agent") # URL that runs the OpenLLM server agent.run
+("Is the following `text` positive or negative?", text="I don't like how this
+models is generate inputs") ``` > **Note** Only `starcoder` is currently
+supported with Agent integration. The > example aboved was also ran with four
+T4s on EC2 `g4dn.12xlarge` If you want to use OpenLLM client to ask questions
+to the running agent, you can also do so: ```python import openllm client =
+openllm.client.HTTPClient("http://localhost:3000") client.ask_agent( task="Is
+the following `text` positive or negative?", text="What are you thinking
+about?", ) ``` ### LangChain (â³Coming Soon!) In future LangChain releases,
+you'll be able to effortlessly invoke OpenLLM models, like so: ```python from
+langchain.llms import OpenLLM llm = OpenLLM.for_model(model_name='flan-t5') llm
+("What is the difference between a duck and a goose?") ``` if you have an
+OpenLLM server deployed elsewhere, you can connect to it by specifying its URL:
+```python from langchain.llms import OpenLLM llm = OpenLLM.for_model
+(server_url='http://localhost:8000', server_type='http') llm("What is the
+difference between a duck and a goose?") ``` ## ð Deploying to Production To
+deploy your LLMs into production: 1. **Building a Bento**: With OpenLLM, you
+can easily build a Bento for a specific model, like `dolly-v2`, using the
+`build` command.: ```bash openllm build dolly-v2 ``` A [Bento](https://
+docs.bentoml.org/en/latest/concepts/bento.html#what-is-a-bento), in BentoML, is
+the unit of distribution. It packages your program's source code, models,
+files, artifacts, and dependencies. 2. **Containerize your Bento** ```bash
+bentoml containerize  ``` BentoML offers a comprehensive set of options for
+deploying and hosting online ML services in production. To learn more, check
+out the [Deploying a Bento](https://docs.bentoml.org/en/latest/concepts/
+deploy.html) guide. ## ð Telemetry OpenLLM collects usage data to enhance
+user experience and improve the product. We only report OpenLLM's internal API
+calls and ensure maximum privacy by excluding sensitive information. We will
+never collect user code, model data, or stack traces. For usage tracking, check
+out the [code](./src/openllm/utils/analytics.py). You can opt-out of usage
+tracking by using the `--do-not-track` CLI option: ```bash openllm [command] --
+do-not-track ``` Or by setting environment variable
+`OPENLLM_DO_NOT_TRACK=True`: ```bash export OPENLLM_DO_NOT_TRACK=True ``` ##
+ð¥ Community Engage with like-minded individuals passionate about LLMs, AI,
+and more on our [Discord](https://l.bentoml.com/join-openllm-discord)! OpenLLM
+is actively maintained by the BentoML team. Feel free to reach out and join us
+in our pursuit to make LLMs more accessible and easy-to-useð [Join our Slack
+community!](https://l.bentoml.com/join-slack) ## ð Contributing We welcome
+contributions! If you're interested in enhancing OpenLLM's capabilities or have
+any questions, don't hesitate to reach out in our [discord channel](https://
+l.bentoml.com/join-openllm-discord). Checkout our [Developer Guide](https://
+github.com/bentoml/OpenLLM/blob/main/DEVELOPMENT.md) if you wish to contribute
+to OpenLLM's codebase.
```

### Comparing `openllm-0.1.6/pyproject.toml` & `openllm-0.1.7/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,13 @@
 [build-system]
 build-backend = "hatchling.build"
 requires = ["hatchling"]
 
 [project]
-authors = [
-    { name = "Aaron Pham", email = "aarnphm@bentoml.com" },
-    { name = "BentoML Team", email = "contact@bentoml.com" },
-]
+authors = [{ name = "Aaron Pham", email = "aarnphm@bentoml.com" }]
 classifiers = [
     "Development Status :: 4 - Beta",
     "License :: OSI Approved :: Apache Software License",
     "Topic :: Scientific/Engineering :: Artificial Intelligence",
     "Topic :: Software Development :: Libraries",
     "Operating System :: OS Independent",
     "Programming Language :: Python",
@@ -19,33 +16,25 @@
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: PyPy",
 ]
+# NOTE: The below is managed by ./tools/update-optional-dependencies.py
 dependencies = [
-    # bentoml[io] includes pydantic, PIL, filetype, pandas and numpy
-    # bentoml[grpc,grpc-reflection] include grpcio, grpcio-reflection
     "bentoml[grpc,io]>=1.0.22",
+    "transformers[torch,tokenizers,accelerate]>=4.29.0",
+    "optimum",
     "attrs>=23.1.0",
     "cattrs>=23.1.0",
-    # transformers[torch] includes torch and transformers
-    "transformers[torch,tokenizers]>=4.29.0",
-    # BetterTransformer support for inference.
-    "optimum",
-    # Super fast JSON serialization
     "orjson",
     "inflection",
-    # tabulate for CLI with CJK support
-    # >=0.9.0 for some bug fixes
     "tabulate[widechars]>=0.9.0",
-    # httpx used within openllm.client
     "httpx",
-    # for typing support
     "typing_extensions",
 ]
 description = 'OpenLLM: REST/gRPC API server for running any open Large-Language Model - StableLM, Llama, Alpaca, Dolly, Flan-T5, Custom'
 dynamic = ["version"]
 keywords = [
     "MLOps",
     "AI",
@@ -65,25 +54,27 @@
 name = "openllm"
 readme = "README.md"
 requires-python = ">=3.8"
 
 # NOTE: Don't modify project.optional-dependencies
 # as it is managed by ./tools/update-optional-dependencies.py
 [project.optional-dependencies]
+agents = ["transformers[agents]", "diffusers", "soundfile"]
 all = [
     "openllm[chatglm]",
     "openllm[starcoder]",
     "openllm[falcon]",
+    "openllm[agents]",
     "openllm[fine-tune]",
-    "openllm[flan-t5]",
     "openllm[openai]",
+    "openllm[flan-t5]",
 ]
 chatglm = ["cpm_kernels", "sentencepiece"]
 falcon = ["einops", "xformers", "safetensors"]
-fine-tune = ["peft", "bitsandbytes", "datasets", "accelerate", "deepspeed", "auto-gptq"]
+fine-tune = ["peft", "bitsandbytes", "datasets", "accelerate", "deepspeed"]
 flan-t5 = ["flax", "jax", "jaxlib", "tensorflow", "keras"]
 openai = ["openai", "tiktoken"]
 starcoder = ["bitsandbytes"]
 
 [project.urls]
 Documentation = "https://github.com/bentoml/openllm#readme"
 Issues = "https://github.com/bentoml/openllm/issues"
@@ -97,48 +88,14 @@
 
 [tool.hatch.metadata]
 allow-direct-references = true
 
 [tool.hatch.build.targets.wheel]
 packages = ["src/openllm", "src/openllm_client"]
 
-[tool.hatch.envs.default]
-dependencies = [
-    "coverage[toml]>=6.5",
-    # NOTE: Tests strategies with Hypothesis and pytest, and snapshot testing with syrupy
-    "pytest",
-    "pytest-asyncio>=0.21.0",
-    "pytest-xdist[psutil]",
-    "pytest-cov",
-    "pytest-mock",
-    "pytest-randomly",
-    "pytest-rerunfailures",
-    "hypothesis",
-    "syrupy",
-    # NOTE: To run all hooks
-    "pre-commit",
-    # NOTE: Using under ./tools/update-optional-dependencies.py
-    "tomlkit",
-    # NOTE: Using under ./tools/update-readme.py
-    "markdown-it-py",
-    # NOTE: pyright for type
-    "pyright",
-    # NOTE: towncrier for changelog
-    "towncrier",
-]
-[tool.hatch.envs.default.scripts]
-changelog = "towncrier build --version main --draft"
-cov = ["cov-test", "cov-report"]
-cov-report = ["- coverage combine", "coverage report"]
-cov-test = "coverage run -m pytest {args:tests}"
-fmt = "pre-commit run --all-files"
-setup = "pre-commit install"
-test = "pytest {args:tests}"
-typing = "pyright {args:src/openllm tests}"
-
 [tool.towncrier]
 directory = "changelog.d"
 filename = "CHANGELOG.md"
 issue_format = "[#{issue}](https://github.com/bentoml/openllm/issues/{issue})"
 name = "openllm"
 start_string = "<!-- towncrier release notes start -->\n"
 template = "changelog.d/template.md.jinja"
@@ -192,39 +149,37 @@
     | _build
     | .build
     | bazel-*
     | build
     | venv
     | lib
     | dist
+    | tools
   )/
   | src/openllm/__about__.py
 )
 '''
-line-length = 120
+line-length = 119
 target-version = ["py311"]
 
 [tool.ruff]
+exclude = ["tools"]
 ignore = [
     # Allow non-abstract empty methods in abstract base classes
     "B027",
     # Allow boolean positional values in function calls, like `dict.get(... True)`
     "FBT003",
-    # Ignore checks for possible passwords
-    "S105",
-    "S106",
-    "S107",
     # Ignore complexity
     "C901",
-    "PLR0911",
-    "PLR0912",
-    "PLR0913",
-    "PLR0915",
+    # Never enforce `E501` (line length violations).
+    "E501",
+    "E741",
 ]
-line-length = 120
+line-length = 119
+select = ["C", "E", "F", "I", "W"]
 target-version = "py311"
 unfixable = [
     "F401", # Don't touch unused imports, just warn about it.
 ]
 
 [tool.ruff.pydocstyle]
 convention = "google"
```

### Comparing `openllm-0.1.6/PKG-INFO` & `openllm-0.1.7/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: openllm
-Version: 0.1.6
+Version: 0.1.7
 Summary: OpenLLM: REST/gRPC API server for running any open Large-Language Model - StableLM, Llama, Alpaca, Dolly, Flan-T5, Custom
 Project-URL: Documentation, https://github.com/bentoml/openllm#readme
 Project-URL: Issues, https://github.com/bentoml/openllm/issues
 Project-URL: Source, https://github.com/bentoml/openllm
-Author-email: Aaron Pham <aarnphm@bentoml.com>, BentoML Team <contact@bentoml.com>
+Author-email: Aaron Pham <aarnphm@bentoml.com>
 License-Expression: Apache-2.0
 License-File: LICENSE.md
 Keywords: AI,Alpaca,BentoML,Generative AI,LLMOps,Large Language Model,MLOps,Model Deployment,Model Serving,PyTorch,Stable Diffusion,StableLM,Transformers
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
@@ -28,17 +28,22 @@
 Requires-Dist: bentoml[grpc,io]>=1.0.22
 Requires-Dist: cattrs>=23.1.0
 Requires-Dist: httpx
 Requires-Dist: inflection
 Requires-Dist: optimum
 Requires-Dist: orjson
 Requires-Dist: tabulate[widechars]>=0.9.0
-Requires-Dist: transformers[tokenizers,torch]>=4.29.0
+Requires-Dist: transformers[accelerate,tokenizers,torch]>=4.29.0
 Requires-Dist: typing-extensions
+Provides-Extra: agents
+Requires-Dist: diffusers; extra == 'agents'
+Requires-Dist: soundfile; extra == 'agents'
+Requires-Dist: transformers[agents]; extra == 'agents'
 Provides-Extra: all
+Requires-Dist: openllm[agents]; extra == 'all'
 Requires-Dist: openllm[chatglm]; extra == 'all'
 Requires-Dist: openllm[falcon]; extra == 'all'
 Requires-Dist: openllm[fine-tune]; extra == 'all'
 Requires-Dist: openllm[flan-t5]; extra == 'all'
 Requires-Dist: openllm[openai]; extra == 'all'
 Requires-Dist: openllm[starcoder]; extra == 'all'
 Provides-Extra: chatglm
@@ -46,15 +51,14 @@
 Requires-Dist: sentencepiece; extra == 'chatglm'
 Provides-Extra: falcon
 Requires-Dist: einops; extra == 'falcon'
 Requires-Dist: safetensors; extra == 'falcon'
 Requires-Dist: xformers; extra == 'falcon'
 Provides-Extra: fine-tune
 Requires-Dist: accelerate; extra == 'fine-tune'
-Requires-Dist: auto-gptq; extra == 'fine-tune'
 Requires-Dist: bitsandbytes; extra == 'fine-tune'
 Requires-Dist: datasets; extra == 'fine-tune'
 Requires-Dist: deepspeed; extra == 'fine-tune'
 Requires-Dist: peft; extra == 'fine-tune'
 Provides-Extra: flan-t5
 Requires-Dist: flax; extra == 'flan-t5'
 Requires-Dist: jax; extra == 'flan-t5'
@@ -64,14 +68,16 @@
 Provides-Extra: openai
 Requires-Dist: openai; extra == 'openai'
 Requires-Dist: tiktoken; extra == 'openai'
 Provides-Extra: starcoder
 Requires-Dist: bitsandbytes; extra == 'starcoder'
 Description-Content-Type: text/markdown
 
+![Banner for OpenLLM](/assets/main-banner.png)
+
 <div align="center">
     <h1 align="center">🦾 OpenLLM</h1>
     <a href="https://pypi.org/project/openllm">
         <img src="https://img.shields.io/pypi/v/openllm.svg" alt="pypi_status" />
     </a><a href="https://github.com/bentoml/OpenLLM/actions/workflows/ci.yml">
         <img src="https://github.com/bentoml/OpenLLM/actions/workflows/ci.yml/badge.svg?branch=main" alt="ci" />
     </a><a href="https://twitter.com/bentomlai">
@@ -82,27 +88,27 @@
     <p>An open platform for operating large language models (LLMs) in production.</br>
     Fine-tune, serve, deploy, and monitor any LLMs with ease.</p>
     <i></i>
 </div>
 
 ## 📖 Introduction
 
-With OpenLLM, you can run inference with any open-source large-language
-models (LLMs), deploy to the cloud or on-premises, and build powerful AI apps.
+With OpenLLM, you can run inference with any open-source large-language models,
+deploy to the cloud or on-premises, and build powerful AI apps.
 
-🚂 **SOTA LLMs**: built-in supports a wide range of open-source LLMs and model
-runtime, including StableLM, Falcon, Dolly, Flan-T5, ChatGLM, StarCoder and
-more.
+🚂 **State-of-the-art LLMs**: built-in supports a wide range of open-source LLMs
+and model runtime, including StableLM, Falcon, Dolly, Flan-T5, ChatGLM,
+StarCoder and more.
 
 🔥 **Flexible APIs**: serve LLMs over RESTful API or gRPC with one command,
 query via WebUI, CLI, our Python/Javascript client, or any HTTP client.
 
-⛓️ **Freedom To Build**: First-class support for LangChain and BentoML allows you
-to easily create your own AI apps by composing LLMs with other models and
-services.
+⛓️ **Freedom To Build**: First-class support for LangChain, BentoML and
+HuggingFace that allows you to easily create your own AI apps by composing LLMs
+with other models and services.
 
 🎯 **Streamline Deployment**: Automatically generate your LLM server Docker
 Images or deploy as serverless endpoint via
 [☁️ BentoCloud](https://l.bentoml.com/bento-cloud).
 
 🤖️ **Bring your own LLM**: Fine-tune any LLM to suit your needs with
 `LLM.tuning()`. (Coming soon)
@@ -360,15 +366,15 @@
 For example, if you want to use the Tensorflow (`tf`) implementation for the
 `flan-t5` model, you can use the following command:
 
 ```bash
 OPENLLM_FLAN_T5_FRAMEWORK=tf openllm start flan-t5
 ```
 
-> For GPU support on Flax, refers to
+> **Note** For GPU support on Flax, refers to
 > [Jax's installation](https://github.com/google/jax#pip-installation-gpu-cuda-installed-via-pip-easier)
 > to make sure that you have Jax support for the corresponding CUDA version.
 
 ### Integrating a New Model
 
 OpenLLM encourages contributions by welcoming users to incorporate their custom
 LLMs into the ecosystem. Check out
@@ -405,14 +411,48 @@
 
 @svc.api(input=Text(), output=Text())
 async def prompt(input_text: str) -> str:
     answer = await llm_runner.generate(input_text)
     return answer
 ```
 
+### HuggingFace Agents
+
+OpenLLM seamlessly integrates with HuggingFace Agents.
+
+> **Warning** The HuggingFace Agent is still at experimental stage. It is
+> recommended to OpenLLM with
+> `pip install -r nightly-requirements.generated.txt` to get the latest API
+> update for HuggingFace agent.
+
+```python
+import transformers
+
+agent = transformers.HfAgent("http://localhost:3000/hf/agent")  # URL that runs the OpenLLM server
+
+agent.run("Is the following `text` positive or negative?", text="I don't like how this models is generate inputs")
+```
+
+> **Note** Only `starcoder` is currently supported with Agent integration. The
+> example aboved was also ran with four T4s on EC2 `g4dn.12xlarge`
+
+If you want to use OpenLLM client to ask questions to the running agent, you can
+also do so:
+
+```python
+import openllm
+
+client = openllm.client.HTTPClient("http://localhost:3000")
+
+client.ask_agent(
+    task="Is the following `text` positive or negative?",
+    text="What are you thinking about?",
+)
+```
+
 ### LangChain (⏳Coming Soon!)
 
 In future LangChain releases, you'll be able to effortlessly invoke OpenLLM
 models, like so:
 
 ```python
 from langchain.llms import OpenLLM
@@ -443,15 +483,15 @@
    A
    [Bento](https://docs.bentoml.org/en/latest/concepts/bento.html#what-is-a-bento),
    in BentoML, is the unit of distribution. It packages your program's source
    code, models, files, artifacts, and dependencies.
 
 2. **Containerize your Bento**
 
-   ```
+   ```bash
    bentoml containerize <name:version>
    ```
 
    BentoML offers a comprehensive set of options for deploying and hosting
    online ML services in production. To learn more, check out the
    [Deploying a Bento](https://docs.bentoml.org/en/latest/concepts/deploy.html)
    guide.
```

#### html2text {}

```diff
@@ -1,14 +1,13 @@
-Metadata-Version: 2.1 Name: openllm Version: 0.1.6 Summary: OpenLLM: REST/gRPC
+Metadata-Version: 2.1 Name: openllm Version: 0.1.7 Summary: OpenLLM: REST/gRPC
 API server for running any open Large-Language Model - StableLM, Llama, Alpaca,
 Dolly, Flan-T5, Custom Project-URL: Documentation, https://github.com/bentoml/
 openllm#readme Project-URL: Issues, https://github.com/bentoml/openllm/issues
 Project-URL: Source, https://github.com/bentoml/openllm Author-email: Aaron
 Pham
-bentoml.com>, BentoML Team
 bentoml.com> License-Expression: Apache-2.0 License-File: LICENSE.md Keywords:
 AI,Alpaca,BentoML,Generative AI,LLMOps,Large Language Model,MLOps,Model
 Deployment,Model Serving,PyTorch,Stable Diffusion,StableLM,Transformers
 Classifier: Development Status :: 4 - Beta Classifier: License :: OSI Approved
 :: Apache Software License Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3 :: Only Classifier:
@@ -18,50 +17,53 @@
 Python :: Implementation :: CPython Classifier: Programming Language :: Python
 :: Implementation :: PyPy Classifier: Topic :: Scientific/Engineering ::
 Artificial Intelligence Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3.8 Requires-Dist: attrs>=23.1.0 Requires-Dist: bentoml
 [grpc,io]>=1.0.22 Requires-Dist: cattrs>=23.1.0 Requires-Dist: httpx Requires-
 Dist: inflection Requires-Dist: optimum Requires-Dist: orjson Requires-Dist:
 tabulate[widechars]>=0.9.0 Requires-Dist: transformers
-[tokenizers,torch]>=4.29.0 Requires-Dist: typing-extensions Provides-Extra: all
+[accelerate,tokenizers,torch]>=4.29.0 Requires-Dist: typing-extensions
+Provides-Extra: agents Requires-Dist: diffusers; extra == 'agents' Requires-
+Dist: soundfile; extra == 'agents' Requires-Dist: transformers[agents]; extra
+== 'agents' Provides-Extra: all Requires-Dist: openllm[agents]; extra == 'all'
 Requires-Dist: openllm[chatglm]; extra == 'all' Requires-Dist: openllm[falcon];
 extra == 'all' Requires-Dist: openllm[fine-tune]; extra == 'all' Requires-Dist:
 openllm[flan-t5]; extra == 'all' Requires-Dist: openllm[openai]; extra == 'all'
 Requires-Dist: openllm[starcoder]; extra == 'all' Provides-Extra: chatglm
 Requires-Dist: cpm-kernels; extra == 'chatglm' Requires-Dist: sentencepiece;
 extra == 'chatglm' Provides-Extra: falcon Requires-Dist: einops; extra ==
 'falcon' Requires-Dist: safetensors; extra == 'falcon' Requires-Dist: xformers;
 extra == 'falcon' Provides-Extra: fine-tune Requires-Dist: accelerate; extra ==
-'fine-tune' Requires-Dist: auto-gptq; extra == 'fine-tune' Requires-Dist:
-bitsandbytes; extra == 'fine-tune' Requires-Dist: datasets; extra == 'fine-
-tune' Requires-Dist: deepspeed; extra == 'fine-tune' Requires-Dist: peft; extra
-== 'fine-tune' Provides-Extra: flan-t5 Requires-Dist: flax; extra == 'flan-t5'
-Requires-Dist: jax; extra == 'flan-t5' Requires-Dist: jaxlib; extra == 'flan-
-t5' Requires-Dist: keras; extra == 'flan-t5' Requires-Dist: tensorflow; extra
-== 'flan-t5' Provides-Extra: openai Requires-Dist: openai; extra == 'openai'
-Requires-Dist: tiktoken; extra == 'openai' Provides-Extra: starcoder Requires-
-Dist: bitsandbytes; extra == 'starcoder' Description-Content-Type: text/
-markdown
+'fine-tune' Requires-Dist: bitsandbytes; extra == 'fine-tune' Requires-Dist:
+datasets; extra == 'fine-tune' Requires-Dist: deepspeed; extra == 'fine-tune'
+Requires-Dist: peft; extra == 'fine-tune' Provides-Extra: flan-t5 Requires-
+Dist: flax; extra == 'flan-t5' Requires-Dist: jax; extra == 'flan-t5' Requires-
+Dist: jaxlib; extra == 'flan-t5' Requires-Dist: keras; extra == 'flan-t5'
+Requires-Dist: tensorflow; extra == 'flan-t5' Provides-Extra: openai Requires-
+Dist: openai; extra == 'openai' Requires-Dist: tiktoken; extra == 'openai'
+Provides-Extra: starcoder Requires-Dist: bitsandbytes; extra == 'starcoder'
+Description-Content-Type: text/markdown ![Banner for OpenLLM](/assets/main-
+banner.png)
                           ****** ð¦¾ OpenLLM ******
                       [pypi_status][ci][Twitter][Discord]
   An open platform for operating large language models (LLMs) in production.
            Fine-tune, serve, deploy, and monitor any LLMs with ease.
 ## ð Introduction With OpenLLM, you can run inference with any open-source
-large-language models (LLMs), deploy to the cloud or on-premises, and build
-powerful AI apps. ð **SOTA LLMs**: built-in supports a wide range of open-
-source LLMs and model runtime, including StableLM, Falcon, Dolly, Flan-T5,
+large-language models, deploy to the cloud or on-premises, and build powerful
+AI apps. ð **State-of-the-art LLMs**: built-in supports a wide range of
+open-source LLMs and model runtime, including StableLM, Falcon, Dolly, Flan-T5,
 ChatGLM, StarCoder and more. ð¥ **Flexible APIs**: serve LLMs over RESTful
 API or gRPC with one command, query via WebUI, CLI, our Python/Javascript
 client, or any HTTP client. âï¸ **Freedom To Build**: First-class support
-for LangChain and BentoML allows you to easily create your own AI apps by
-composing LLMs with other models and services. ð¯ **Streamline Deployment**:
-Automatically generate your LLM server Docker Images or deploy as serverless
-endpoint via [âï¸ BentoCloud](https://l.bentoml.com/bento-cloud). ð¤ï¸
-**Bring your own LLM**: Fine-tune any LLM to suit your needs with `LLM.tuning
-()`. (Coming soon) ![Gif showing OpenLLM Intro](/assets/output.gif)
+for LangChain, BentoML and HuggingFace that allows you to easily create your
+own AI apps by composing LLMs with other models and services. ð¯ **Streamline
+Deployment**: Automatically generate your LLM server Docker Images or deploy as
+serverless endpoint via [âï¸ BentoCloud](https://l.bentoml.com/bento-cloud).
+ð¤ï¸ **Bring your own LLM**: Fine-tune any LLM to suit your needs with
+`LLM.tuning()`. (Coming soon) ![Gif showing OpenLLM Intro](/assets/output.gif)
 ## ðâ Getting Started To use OpenLLM, you need to have Python 3.8 (or
 newer) and `pip` installed on your system. We highly recommend using a Virtual
 Environment to prevent package conflicts. You can install OpenLLM using pip as
 follows: ```bash pip install openllm ``` To verify if it's installed correctly,
 run: ``` $ openllm -h Usage: openllm [OPTIONS] COMMAND [ARGS]...
 âââââââ âââââââ
 ââââââââââââ ââââââ âââ ââââ
@@ -135,62 +137,75 @@
  ### Runtime Implementations (Experimental) Different LLMs may have multiple
 runtime implementations. For instance, they might use Pytorch (`pt`),
 Tensorflow (`tf`), or Flax (`flax`). If you wish to specify a particular
 runtime for a model, you can do so by setting the `OPENLLM_
 {MODEL_NAME}_FRAMEWORK={runtime}` environment variable before running `openllm
 start`. For example, if you want to use the Tensorflow (`tf`) implementation
 for the `flan-t5` model, you can use the following command: ```bash
-OPENLLM_FLAN_T5_FRAMEWORK=tf openllm start flan-t5 ``` > For GPU support on
-Flax, refers to > [Jax's installation](https://github.com/google/jax#pip-
-installation-gpu-cuda-installed-via-pip-easier) > to make sure that you have
-Jax support for the corresponding CUDA version. ### Integrating a New Model
-OpenLLM encourages contributions by welcoming users to incorporate their custom
-LLMs into the ecosystem. Check out [Adding a New Model Guide](https://
+OPENLLM_FLAN_T5_FRAMEWORK=tf openllm start flan-t5 ``` > **Note** For GPU
+support on Flax, refers to > [Jax's installation](https://github.com/google/
+jax#pip-installation-gpu-cuda-installed-via-pip-easier) > to make sure that you
+have Jax support for the corresponding CUDA version. ### Integrating a New
+Model OpenLLM encourages contributions by welcoming users to incorporate their
+custom LLMs into the ecosystem. Check out [Adding a New Model Guide](https://
 github.com/bentoml/OpenLLM/blob/main/ADDING_NEW_MODEL.md) to see how you can do
 it yourself. ## âï¸ Integrations OpenLLM is not just a standalone product;
 it's a building block designed to easily integrate with other powerful tools.
 We currently offer integration with [BentoML](https://github.com/bentoml/
 BentoML) and [LangChain](https://github.com/hwchase17/langchain). ### BentoML
 OpenLLM models can be integrated as a [Runner](https://docs.bentoml.org/en/
 latest/concepts/runner.html) in your BentoML service. These runners have a
 `generate` method that takes a string as a prompt and returns a corresponding
 output string. This will allow you to plug and play any OpenLLM models with
 your existing ML workflow. ```python import bentoml import openllm model =
 "dolly-v2" llm_config = openllm.AutoConfig.for_model(model) llm_runner =
 openllm.Runner(model, llm_config=llm_config) svc = bentoml.Service( name=f"llm-
 dolly-v2-service", runners=[llm_runner] ) @svc.api(input=Text(), output=Text())
 async def prompt(input_text: str) -> str: answer = await llm_runner.generate
-(input_text) return answer ``` ### LangChain (â³Coming Soon!) In future
-LangChain releases, you'll be able to effortlessly invoke OpenLLM models, like
-so: ```python from langchain.llms import OpenLLM llm = OpenLLM.for_model
-(model_name='flan-t5') llm("What is the difference between a duck and a
-goose?") ``` if you have an OpenLLM server deployed elsewhere, you can connect
-to it by specifying its URL: ```python from langchain.llms import OpenLLM llm =
-OpenLLM.for_model(server_url='http://localhost:8000', server_type='http') llm
-("What is the difference between a duck and a goose?") ``` ## ð Deploying to
-Production To deploy your LLMs into production: 1. **Building a Bento**: With
-OpenLLM, you can easily build a Bento for a specific model, like `dolly-v2`,
-using the `build` command.: ```bash openllm build dolly-v2 ``` A [Bento](https:
-//docs.bentoml.org/en/latest/concepts/bento.html#what-is-a-bento), in BentoML,
-is the unit of distribution. It packages your program's source code, models,
-files, artifacts, and dependencies. 2. **Containerize your Bento** ``` bentoml
-containerize  ``` BentoML offers a comprehensive set of options for deploying
-and hosting online ML services in production. To learn more, check out the
-[Deploying a Bento](https://docs.bentoml.org/en/latest/concepts/deploy.html)
-guide. ## ð Telemetry OpenLLM collects usage data to enhance user experience
-and improve the product. We only report OpenLLM's internal API calls and ensure
-maximum privacy by excluding sensitive information. We will never collect user
-code, model data, or stack traces. For usage tracking, check out the [code](./
-src/openllm/utils/analytics.py). You can opt-out of usage tracking by using the
-`--do-not-track` CLI option: ```bash openllm [command] --do-not-track ``` Or by
-setting environment variable `OPENLLM_DO_NOT_TRACK=True`: ```bash export
-OPENLLM_DO_NOT_TRACK=True ``` ## ð¥ Community Engage with like-minded
-individuals passionate about LLMs, AI, and more on our [Discord](https://
-l.bentoml.com/join-openllm-discord)! OpenLLM is actively maintained by the
-BentoML team. Feel free to reach out and join us in our pursuit to make LLMs
-more accessible and easy-to-useð [Join our Slack community!](https://
-l.bentoml.com/join-slack) ## ð Contributing We welcome contributions! If
-you're interested in enhancing OpenLLM's capabilities or have any questions,
-don't hesitate to reach out in our [discord channel](https://l.bentoml.com/
-join-openllm-discord). Checkout our [Developer Guide](https://github.com/
-bentoml/OpenLLM/blob/main/DEVELOPMENT.md) if you wish to contribute to
-OpenLLM's codebase.
+(input_text) return answer ``` ### HuggingFace Agents OpenLLM seamlessly
+integrates with HuggingFace Agents. > **Warning** The HuggingFace Agent is
+still at experimental stage. It is > recommended to OpenLLM with > `pip install
+-r nightly-requirements.generated.txt` to get the latest API > update for
+HuggingFace agent. ```python import transformers agent = transformers.HfAgent
+("http://localhost:3000/hf/agent") # URL that runs the OpenLLM server agent.run
+("Is the following `text` positive or negative?", text="I don't like how this
+models is generate inputs") ``` > **Note** Only `starcoder` is currently
+supported with Agent integration. The > example aboved was also ran with four
+T4s on EC2 `g4dn.12xlarge` If you want to use OpenLLM client to ask questions
+to the running agent, you can also do so: ```python import openllm client =
+openllm.client.HTTPClient("http://localhost:3000") client.ask_agent( task="Is
+the following `text` positive or negative?", text="What are you thinking
+about?", ) ``` ### LangChain (â³Coming Soon!) In future LangChain releases,
+you'll be able to effortlessly invoke OpenLLM models, like so: ```python from
+langchain.llms import OpenLLM llm = OpenLLM.for_model(model_name='flan-t5') llm
+("What is the difference between a duck and a goose?") ``` if you have an
+OpenLLM server deployed elsewhere, you can connect to it by specifying its URL:
+```python from langchain.llms import OpenLLM llm = OpenLLM.for_model
+(server_url='http://localhost:8000', server_type='http') llm("What is the
+difference between a duck and a goose?") ``` ## ð Deploying to Production To
+deploy your LLMs into production: 1. **Building a Bento**: With OpenLLM, you
+can easily build a Bento for a specific model, like `dolly-v2`, using the
+`build` command.: ```bash openllm build dolly-v2 ``` A [Bento](https://
+docs.bentoml.org/en/latest/concepts/bento.html#what-is-a-bento), in BentoML, is
+the unit of distribution. It packages your program's source code, models,
+files, artifacts, and dependencies. 2. **Containerize your Bento** ```bash
+bentoml containerize  ``` BentoML offers a comprehensive set of options for
+deploying and hosting online ML services in production. To learn more, check
+out the [Deploying a Bento](https://docs.bentoml.org/en/latest/concepts/
+deploy.html) guide. ## ð Telemetry OpenLLM collects usage data to enhance
+user experience and improve the product. We only report OpenLLM's internal API
+calls and ensure maximum privacy by excluding sensitive information. We will
+never collect user code, model data, or stack traces. For usage tracking, check
+out the [code](./src/openllm/utils/analytics.py). You can opt-out of usage
+tracking by using the `--do-not-track` CLI option: ```bash openllm [command] --
+do-not-track ``` Or by setting environment variable
+`OPENLLM_DO_NOT_TRACK=True`: ```bash export OPENLLM_DO_NOT_TRACK=True ``` ##
+ð¥ Community Engage with like-minded individuals passionate about LLMs, AI,
+and more on our [Discord](https://l.bentoml.com/join-openllm-discord)! OpenLLM
+is actively maintained by the BentoML team. Feel free to reach out and join us
+in our pursuit to make LLMs more accessible and easy-to-useð [Join our Slack
+community!](https://l.bentoml.com/join-slack) ## ð Contributing We welcome
+contributions! If you're interested in enhancing OpenLLM's capabilities or have
+any questions, don't hesitate to reach out in our [discord channel](https://
+l.bentoml.com/join-openllm-discord). Checkout our [Developer Guide](https://
+github.com/bentoml/OpenLLM/blob/main/DEVELOPMENT.md) if you wish to contribute
+to OpenLLM's codebase.
```

