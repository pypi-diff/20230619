# Comparing `tmp/lightdash_client_python-0.618.0.tar.gz` & `tmp/lightdash_client_python-0.619.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lightdash_client_python-0.618.0.tar", last modified: Mon Jun 19 00:37:07 2023, max compression
+gzip compressed data, was "lightdash_client_python-0.619.1.tar", last modified: Mon Jun 19 12:41:42 2023, max compression
```

## Comparing `lightdash_client_python-0.618.0.tar` & `lightdash_client_python-0.619.1.tar`

### file list

```diff
@@ -1,287 +1,289 @@
--rw-r--r--   0        0        0      804 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/.github/CODEOWNERS
--rw-r--r--   0        0        0      402 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/.github/workflows/contributors-list.yml
--rw-r--r--   0        0        0     1849 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/.github/workflows/publish.yml
--rw-r--r--   0        0        0     2335 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/.github/workflows/test-publish.yml
--rw-r--r--   0        0        0     1115 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/.github/workflows/test.yml
--rw-r--r--   0        0        0     3078 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/.gitignore
--rw-r--r--   0        0        0     1040 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/.openapi-generator-ignore
--rw-r--r--   0        0        0     6821 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/.openapi-generator/FILES
--rw-r--r--   0        0        0        6 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/.openapi-generator/VERSION
--rw-r--r--   0        0        0     1375 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0    14088 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/.pylintrc
--rw-r--r--   0        0        0      150 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/.pypirc
--rw-r--r--   0        0        0        8 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/.python-version
--rw-r--r--   0        0        0       32 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/.style.yapf
--rw-r--r--   0        0        0    11357 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/LICENSE
--rw-r--r--   0        0        0      717 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/Makefile
--rw-r--r--   0        0        0     3258 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/README.md
--rwxr-xr-x   0        0        0     1121 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/dev/clean.sh
--rw-r--r--   0        0        0     2115 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/dev/generate_clients.sh
--rw-r--r--   0        0        0      974 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/dev/lint.sh
--rw-r--r--   0        0        0      211 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/dev/openapi-python-client.yml
--rwxr-xr-x   0        0        0     1391 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/dev/publish.sh
--rw-r--r--   0        0        0      152 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/dev/schemas/README.md
--rw-r--r--   0        0        0     1299 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/dev/schemas/download.sh
--rw-r--r--   0        0        0   233800 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/dev/schemas/swagger.json
--rwxr-xr-x   0        0        0     1023 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/dev/setup.sh
--rwxr-xr-x   0        0        0      958 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/dev/test_python.sh
--rw-r--r--   0        0        0      201 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/__init__.py
--rw-r--r--   0        0        0       47 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/api/__init__.py
--rw-r--r--   0        0        0        0 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/api/charts/__init__.py
--rw-r--r--   0        0        0     4680 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/api/charts/post_chart_results.py
--rw-r--r--   0        0        0        0 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/api/content/__init__.py
--rw-r--r--   0        0        0     4483 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/api/content/get_pinned_items.py
--rw-r--r--   0        0        0     5511 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/api/content/update_pinned_items_order.py
--rw-r--r--   0        0        0        0 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/api/exploring/__init__.py
--rw-r--r--   0        0        0     5017 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/api/exploring/post_run_query.py
--rw-r--r--   0        0        0     5095 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/api/exploring/post_run_underlying_data_query.py
--rw-r--r--   0        0        0        0 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/api/exports/__init__.py
--rw-r--r--   0        0        0     3848 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/api/exports/get_csv_url.py
--rw-r--r--   0        0        0        0 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/api/integrations/__init__.py
--rw-r--r--   0        0        0     4403 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/api/integrations/delete_dbt_cloud_integration_settings.py
--rw-r--r--   0        0        0     2743 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/api/integrations/get_dbt_cloud_integration_settings.py
--rw-r--r--   0        0        0     4847 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/api/integrations/get_dbt_cloud_metrics.py
--rw-r--r--   0        0        0     3651 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/api/integrations/get_slack_channels.py
--rw-r--r--   0        0        0     2734 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/api/integrations/update_dbt_cloud_integration_settings.py
--rw-r--r--   0        0        0        0 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/api/my_account/__init__.py
--rw-r--r--   0        0        0     2573 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/api/my_account/create_email_one_time_passcode.py
--rw-r--r--   0        0        0     3501 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/api/my_account/delete_me.py
--rw-r--r--   0        0        0     3021 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/api/my_account/get_email_verification_status.py
--rw-r--r--   0        0        0     4793 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/api/my_account/join_organization.py
--rw-r--r--   0        0        0     4349 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/api/my_account/list_my_available_organizations.py
--rw-r--r--   0        0        0        0 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/api/organizations/__init__.py
--rw-r--r--   0        0        0     4634 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/api/organizations/create_group_in_organization.py
--rw-r--r--   0        0        0     4256 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/api/organizations/delete_my_organization.py
--rw-r--r--   0        0        0     4057 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/api/organizations/delete_organization_member.py
--rw-r--r--   0        0        0     3589 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/api/organizations/get_my_organization.py
--rw-r--r--   0        0        0     3739 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/api/organizations/list_groups_in_organization.py
--rw-r--r--   0        0        0     3983 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/api/organizations/list_organization_email_domains.py
--rw-r--r--   0        0        0     3859 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/api/organizations/list_organization_members.py
--rw-r--r--   0        0        0     3771 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/api/organizations/list_organization_projects.py
--rw-r--r--   0        0        0        0 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/api/projects/__init__.py
--rw-r--r--   0        0        0     5756 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/api/projects/get_latest_validation_results.py
--rw-r--r--   0        0        0     2639 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/api/projects/get_project.py
--rw-r--r--   0        0        0     4187 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/api/projects/list_charts_in_project.py
--rw-r--r--   0        0        0     4187 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/api/projects/list_spaces_in_project.py
--rw-r--r--   0        0        0     6428 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/api/projects/validate_project.py
--rw-r--r--   0        0        0        0 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/api/roles_permissions/__init__.py
--rw-r--r--   0        0        0     2984 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/api/roles_permissions/create_space_in_project.py
--rw-r--r--   0        0        0     4928 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/api/roles_permissions/get_project_access_list.py
--rw-r--r--   0        0        0     4648 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/api/roles_permissions/grant_project_access_to_user.py
--rw-r--r--   0        0        0     4425 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/api/roles_permissions/revoke_project_access_for_user.py
--rw-r--r--   0        0        0     4794 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/api/roles_permissions/revoke_space_access_for_user.py
--rw-r--r--   0        0        0     5026 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/api/roles_permissions/update_project_access_for_user.py
--rw-r--r--   0        0        0        0 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/api/schedulers/__init__.py
--rw-r--r--   0        0        0     4176 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/api/schedulers/delete_scheduler.py
--rw-r--r--   0        0        0     4147 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/api/schedulers/get_scheduled_jobs.py
--rw-r--r--   0        0        0     2633 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/api/schedulers/get_scheduler.py
--rw-r--r--   0        0        0     4201 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/api/schedulers/get_scheduler_job_status.py
--rw-r--r--   0        0        0     2620 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/api/schedulers/get_scheduler_logs.py
--rw-r--r--   0        0        0     2919 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/api/schedulers/update_scheduler.py
--rw-r--r--   0        0        0        0 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/api/share_links/__init__.py
--rw-r--r--   0        0        0     3960 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/api/share_links/get_share_url.py
--rw-r--r--   0        0        0        0 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/api/spaces/__init__.py
--rw-r--r--   0        0        0     4429 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/api/spaces/delete_space.py
--rw-r--r--   0        0        0     2881 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/api/spaces/get_space.py
--rw-r--r--   0        0        0        0 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/api/ssh_keypairs/__init__.py
--rw-r--r--   0        0        0     3542 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/api/ssh_keypairs/create_ssh_key_pair.py
--rw-r--r--   0        0        0        0 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/api/user_groups/__init__.py
--rw-r--r--   0        0        0     4365 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/api/user_groups/add_user_to_group.py
--rw-r--r--   0        0        0     3927 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/api/user_groups/delete_group.py
--rw-r--r--   0        0        0     3949 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/api/user_groups/get_group.py
--rw-r--r--   0        0        0     4073 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/api/user_groups/get_group_members.py
--rw-r--r--   0        0        0     4348 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/api/user_groups/remove_user_from_group.py
--rw-r--r--   0        0        0     2906 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/client.py
--rw-r--r--   0        0        0      470 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/errors.py
--rw-r--r--   0        0        0    20640 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/__init__.py
--rw-r--r--   0        0        0     4166 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/additional_metric.py
--rw-r--r--   0        0        0     2422 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/allowed_email_domains.py
--rw-r--r--   0        0        0     2410 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/api_chart_summary_list_response.py
--rw-r--r--   0        0        0      152 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/api_chart_summary_list_response_status.py
--rw-r--r--   0        0        0     2106 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/api_csv_url_response.py
--rw-r--r--   0        0        0     1652 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/api_csv_url_response_results.py
--rw-r--r--   0        0        0      142 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/api_csv_url_response_status.py
--rw-r--r--   0        0        0     2254 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/api_dbt_cloud_metrics.py
--rw-r--r--   0        0        0      143 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/api_dbt_cloud_metrics_status.py
--rw-r--r--   0        0        0     2119 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/api_dbt_cloud_settings_delete_success.py
--rw-r--r--   0        0        0      157 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/api_dbt_cloud_settings_delete_success_status.py
--rw-r--r--   0        0        0      147 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/api_email_status_response_status.py
--rw-r--r--   0        0        0     2139 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/api_error_payload.py
--rw-r--r--   0        0        0     2386 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/api_error_payload_error.py
--rw-r--r--   0        0        0      146 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/api_error_payload_status.py
--rw-r--r--   0        0        0     2285 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/api_group_list_response.py
--rw-r--r--   0        0        0      145 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/api_group_list_response_status.py
--rw-r--r--   0        0        0     2359 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/api_group_members_response.py
--rw-r--r--   0        0        0      148 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/api_group_members_response_status.py
--rw-r--r--   0        0        0     1951 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/api_group_response.py
--rw-r--r--   0        0        0      141 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/api_group_response_status.py
--rw-r--r--   0        0        0     2208 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/api_job_scheduled_response.py
--rw-r--r--   0        0        0     1548 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/api_job_scheduled_response_results.py
--rw-r--r--   0        0        0      148 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/api_job_scheduled_response_status.py
--rw-r--r--   0        0        0     2157 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/api_job_status_response.py
--rw-r--r--   0        0        0     1535 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/api_job_status_response_results.py
--rw-r--r--   0        0        0      145 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/api_job_status_response_status.py
--rw-r--r--   0        0        0     2019 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/api_organization.py
--rw-r--r--   0        0        0     2241 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/api_organization_allowed_email_domains.py
--rw-r--r--   0        0        0      159 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/api_organization_allowed_email_domains_status.py
--rw-r--r--   0        0        0     2270 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/api_organization_member_profile.py
--rw-r--r--   0        0        0      153 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/api_organization_member_profile_status.py
--rw-r--r--   0        0        0     2519 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/api_organization_member_profiles.py
--rw-r--r--   0        0        0      154 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/api_organization_member_profiles_status.py
--rw-r--r--   0        0        0     2456 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/api_organization_projects.py
--rw-r--r--   0        0        0      148 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/api_organization_projects_status.py
--rw-r--r--   0        0        0      140 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/api_organization_status.py
--rw-r--r--   0        0        0     4825 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/api_pinned_items.py
--rw-r--r--   0        0        0      139 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/api_pinned_items_status.py
--rw-r--r--   0        0        0     2478 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/api_project_access_list_response.py
--rw-r--r--   0        0        0      153 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/api_project_access_list_response_status.py
--rw-r--r--   0        0        0      143 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/api_project_response_status.py
--rw-r--r--   0        0        0     2140 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/api_run_query_response.py
--rw-r--r--   0        0        0     2051 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/api_run_query_response_results.py
--rw-r--r--   0        0        0      144 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/api_run_query_response_status.py
--rw-r--r--   0        0        0     2383 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/api_scheduled_jobs_response.py
--rw-r--r--   0        0        0      149 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/api_scheduled_jobs_response_status.py
--rw-r--r--   0        0        0      155 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/api_scheduler_and_targets_response_status.py
--rw-r--r--   0        0        0      149 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/api_scheduler_logs_response_status.py
--rw-r--r--   0        0        0     2129 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/api_share_response.py
--rw-r--r--   0        0        0      141 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/api_share_response_status.py
--rw-r--r--   0        0        0     2376 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/api_slack_channels_response.py
--rw-r--r--   0        0        0      149 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/api_slack_channels_response_status.py
--rw-r--r--   0        0        0      141 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/api_space_response_status.py
--rw-r--r--   0        0        0     2410 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/api_space_summary_list_response.py
--rw-r--r--   0        0        0      152 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/api_space_summary_list_response_status.py
--rw-r--r--   0        0        0     2208 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/api_ssh_key_pair_response.py
--rw-r--r--   0        0        0      146 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/api_ssh_key_pair_response_status.py
--rw-r--r--   0        0        0     1937 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/api_success_empty.py
--rw-r--r--   0        0        0      140 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/api_success_empty_status.py
--rw-r--r--   0        0        0     2569 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/api_user_allowed_organizations_response.py
--rw-r--r--   0        0        0      160 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/api_user_allowed_organizations_response_status.py
--rw-r--r--   0        0        0     4732 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/api_validate_response.py
--rw-r--r--   0        0        0      144 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/api_validate_response_status.py
--rw-r--r--   0        0        0     1737 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/api_validation_dismiss_response.py
--rw-r--r--   0        0        0      153 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/api_validation_dismiss_response_status.py
--rw-r--r--   0        0        0      316 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/chart_kind.py
--rw-r--r--   0        0        0     3776 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/chart_summary.py
--rw-r--r--   0        0        0      192 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/chart_type.py
--rw-r--r--   0        0        0      220 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/compact.py
--rw-r--r--   0        0        0      272 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/compact_or_alias_type_1.py
--rw-r--r--   0        0        0     1937 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/create_project_member.py
--rw-r--r--   0        0        0     2646 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/create_space.py
--rw-r--r--   0        0        0     3745 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/dbt_azure_dev_ops_project_config.py
--rw-r--r--   0        0        0     3814 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/dbt_bit_bucket_project_config.py
--rw-r--r--   0        0        0     2425 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/dbt_cloud_ide_project_config.py
--rw-r--r--   0        0        0     2229 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/dbt_cloud_metadata_response_metrics.py
--rw-r--r--   0        0        0     2494 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/dbt_cloud_metric.py
--rw-r--r--   0        0        0     3603 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/dbt_github_project_config.py
--rw-r--r--   0        0        0     3603 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/dbt_gitlab_project_config.py
--rw-r--r--   0        0        0     2957 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/dbt_local_project_config.py
--rw-r--r--   0        0        0     2733 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/dbt_none_project_config.py
--rw-r--r--   0        0        0     1664 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/dbt_project_environment_variable.py
--rw-r--r--   0        0        0      295 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/dbt_project_type.py
--rw-r--r--   0        0        0      164 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/dbt_project_type_azuredevops.py
--rw-r--r--   0        0        0      156 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/dbt_project_type_bitbucket.py
--rw-r--r--   0        0        0      138 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/dbt_project_type_dbt.py
--rw-r--r--   0        0        0      166 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/dbt_project_type_dbtcloudide.py
--rw-r--r--   0        0        0      147 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/dbt_project_type_github.py
--rw-r--r--   0        0        0      147 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/dbt_project_type_gitlab.py
--rw-r--r--   0        0        0      141 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/dbt_project_type_none.py
--rw-r--r--   0        0        0     2051 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/delete_scheduler_response_201.py
--rw-r--r--   0        0        0      151 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/delete_scheduler_response_201_status.py
--rw-r--r--   0        0        0     2003 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/email_one_time_password.py
--rw-r--r--   0        0        0     2749 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/email_one_time_password_expiring.py
--rw-r--r--   0        0        0     2458 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/email_status.py
--rw-r--r--   0        0        0     1664 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/filter_group_response_type_0.py
--rw-r--r--   0        0        0     1674 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/filter_group_response_type_1.py
--rw-r--r--   0        0        0     4615 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/filters.py
--rw-r--r--   0        0        0     2247 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/group.py
--rw-r--r--   0        0        0     2163 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/group_member.py
--rw-r--r--   0        0        0     4963 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/metric_query_response.py
--rw-r--r--   0        0        0      383 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/metric_type.py
--rw-r--r--   0        0        0     2812 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/organization.py
--rw-r--r--   0        0        0     3539 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/organization_member_profile.py
--rw-r--r--   0        0        0      287 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/organization_member_role.py
--rw-r--r--   0        0        0     1991 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/organization_project.py
--rw-r--r--   0        0        0     2377 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/partial_omit_organization_organization_uuid_or_needs_project.py
--rw-r--r--   0        0        0     2120 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/partial_pick_organization_member_profile_role.py
--rw-r--r--   0        0        0     2628 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/partial_pick_space_is_private_or_access.py
--rw-r--r--   0        0        0     2493 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/pick_allowed_email_domains_exclude_keyof_allowed_email_domains_organization_uuid.py
--rw-r--r--   0        0        0     6235 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/pick_create_bigquery_credentials_exclude_keyof_create_bigquery_credentials_sensitive_credentials_field_names.py
--rw-r--r--   0        0        0      267 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/pick_create_bigquery_credentials_exclude_keyof_create_bigquery_credentials_sensitive_credentials_field_names_priority.py
--rw-r--r--   0        0        0     3905 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/pick_create_databricks_credentials_exclude_keyof_create_databricks_credentials_sensitive_credentials_field_names.py
--rw-r--r--   0        0        0     1841 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/pick_create_dbt_cloud_integration_metrics_job_id.py
--rw-r--r--   0        0        0     1565 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/pick_create_group_name.py
--rw-r--r--   0        0        0     6859 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/pick_create_postgres_credentials_exclude_keyof_create_postgres_credentials_sensitive_credentials_field_names.py
--rw-r--r--   0        0        0     6610 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/pick_create_redshift_credentials_exclude_keyof_create_redshift_credentials_sensitive_credentials_field_names.py
--rw-r--r--   0        0        0     5207 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/pick_create_snowflake_credentials_exclude_keyof_create_snowflake_credentials_sensitive_credentials_field_names.py
--rw-r--r--   0        0        0     3761 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/pick_create_trino_credentials_exclude_keyof_create_trino_credentials_sensitive_credentials_field_names.py
--rw-r--r--   0        0        0     6625 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/pick_dashboard_uuid_or_name_or_description_or_updated_at_or_project_uuid_or_updated_by_user_or_organization_uuid_or_space_uuid_or_views_or_first_viewed_at_or_pinned_list_uuid_or_pinned_list_order.py
--rw-r--r--   0        0        0     1532 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/pick_group_name.py
--rw-r--r--   0        0        0     1566 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/pick_organization_name.py
--rw-r--r--   0        0        0     2016 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/pick_resource_view_item_at_data_uuid_or_pinned_list_order.py
--rw-r--r--   0        0        0     3781 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/pick_saved_chart_uuid_or_name_or_description_or_space_name_or_space_uuid_or_project_uuid_or_organization_uuid_or_pinned_list_uuid.py
--rw-r--r--   0        0        0     4585 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/pick_saved_chart_uuid_or_name_or_updated_at_or_updated_by_user_or_description_or_space_uuid_or_pinned_list_uuid_or_pinned_list_order.py
--rw-r--r--   0        0        0     1757 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/pick_share_url_path_or_params.py
--rw-r--r--   0        0        0     1502 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/pick_space_name.py
--rw-r--r--   0        0        0     1768 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/pick_space_name_or_is_private.py
--rw-r--r--   0        0        0     2609 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/pick_space_organization_uuid_or_project_uuid_or_uuid_or_name_or_is_private.py
--rw-r--r--   0        0        0     3420 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/pick_space_project_uuid_or_uuid_or_name_or_is_private_or_pinned_list_uuid_or_pinned_list_order_or_organization_uuid.py
--rw-r--r--   0        0        0     1601 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/pick_space_share_user_uuid.py
--rw-r--r--   0        0        0     1619 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/pick_ssh_key_pair_public_key.py
--rw-r--r--   0        0        0     3860 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/pick_validation_response_base_exclude_keyof_validation_response_base_name.py
--rw-r--r--   0        0        0     2266 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/pick_validation_response_error_or_created_at_or_validation_id.py
--rw-r--r--   0        0        0     2095 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/post_chart_results_json_body.py
--rw-r--r--   0        0        0     2540 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/project_member_profile.py
--rw-r--r--   0        0        0      260 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/project_member_role.py
--rw-r--r--   0        0        0      164 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/project_type.py
--rw-r--r--   0        0        0     1294 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/record_string_any.py
--rw-r--r--   0        0        0      193 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/resource_view_item_type.py
--rw-r--r--   0        0        0      150 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/resource_view_item_type_chart.py
--rw-r--r--   0        0        0      162 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/resource_view_item_type_dashboard.py
--rw-r--r--   0        0        0      150 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/resource_view_item_type_space.py
--rw-r--r--   0        0        0     2093 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/resource_view_space_item.py
--rw-r--r--   0        0        0     3903 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/resource_view_space_item_data.py
--rw-r--r--   0        0        0     5334 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/run_query_request.py
--rw-r--r--   0        0        0     1933 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/run_query_request_filters.py
--rw-r--r--   0        0        0     1661 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/scheduled_jobs.py
--rw-r--r--   0        0        0     4958 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/scheduler_base.py
--rw-r--r--   0        0        0     2484 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/scheduler_csv_options.py
--rw-r--r--   0        0        0      170 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/scheduler_csv_options_limit_type_1.py
--rw-r--r--   0        0        0     2685 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/scheduler_email_target.py
--rw-r--r--   0        0        0      156 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/scheduler_format.py
--rw-r--r--   0        0        0     1272 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/scheduler_image_options.py
--rw-r--r--   0        0        0      223 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/scheduler_job_status.py
--rw-r--r--   0        0        0     5049 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/scheduler_log.py
--rw-r--r--   0        0        0      167 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/scheduler_log_target_type.py
--rw-r--r--   0        0        0      443 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/scheduler_log_task.py
--rw-r--r--   0        0        0     2665 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/scheduler_slack_target.py
--rw-r--r--   0        0        0     3505 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/share_url.py
--rw-r--r--   0        0        0     1553 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/slack_channel.py
--rw-r--r--   0        0        0     1658 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/sort_field.py
--rw-r--r--   0        0        0     2115 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/space_share.py
--rw-r--r--   0        0        0     2480 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/space_summary.py
--rw-r--r--   0        0        0     2119 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/table_calculation.py
--rw-r--r--   0        0        0     2350 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/update_pinned_item_order.py
--rw-r--r--   0        0        0     1582 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/update_project_member.py
--rw-r--r--   0        0        0     1173 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/updated_by_user.py
--rw-r--r--   0        0        0     1993 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/user_allowed_organization.py
--rw-r--r--   0        0        0     1964 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/validate_project_json_body.py
--rw-r--r--   0        0        0     6492 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/validation_error_chart_response.py
--rw-r--r--   0        0        0     5966 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/validation_error_dashboard_response.py
--rw-r--r--   0        0        0      260 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/validation_error_type.py
--rw-r--r--   0        0        0     3709 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/validation_response_base.py
--rw-r--r--   0        0        0      193 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/validation_source_type.py
--rw-r--r--   0        0        0     2633 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/view_statistics.py
--rw-r--r--   0        0        0      153 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/warehouse_types_bigquery.py
--rw-r--r--   0        0        0      159 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/warehouse_types_databricks.py
--rw-r--r--   0        0        0      153 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/warehouse_types_postgres.py
--rw-r--r--   0        0        0      153 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/warehouse_types_redshift.py
--rw-r--r--   0        0        0      156 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/warehouse_types_snowflake.py
--rw-r--r--   0        0        0      144 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/warehouse_types_trino.py
--rw-r--r--   0        0        0      225 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/week_day.py
--rw-r--r--   0        0        0       26 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/py.typed
--rw-r--r--   0        0        0     1101 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/types.py
--rw-r--r--   0        0        0     1624 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/pyproject.toml
--rw-r--r--   0        0        0      830 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/setup.py
--rw-r--r--   0        0        0      796 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/tests/__init__.py
--rw-r--r--   0        0        0      908 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/tests/test_dummy.py
--rw-r--r--   0        0        0     5168 1970-01-01 00:00:00.000000 lightdash_client_python-0.618.0/PKG-INFO
+-rw-r--r--   0        0        0      804 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/.github/CODEOWNERS
+-rw-r--r--   0        0        0      402 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/.github/workflows/contributors-list.yml
+-rw-r--r--   0        0        0     1849 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/.github/workflows/publish.yml
+-rw-r--r--   0        0        0     2335 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/.github/workflows/test-publish.yml
+-rw-r--r--   0        0        0     1115 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/.github/workflows/test.yml
+-rw-r--r--   0        0        0     3078 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/.gitignore
+-rw-r--r--   0        0        0     1040 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/.openapi-generator-ignore
+-rw-r--r--   0        0        0     6821 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/.openapi-generator/FILES
+-rw-r--r--   0        0        0        6 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/.openapi-generator/VERSION
+-rw-r--r--   0        0        0     1375 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    14088 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/.pylintrc
+-rw-r--r--   0        0        0      150 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/.pypirc
+-rw-r--r--   0        0        0        8 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/.python-version
+-rw-r--r--   0        0        0       32 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/.style.yapf
+-rw-r--r--   0        0        0    11357 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/LICENSE
+-rw-r--r--   0        0        0      717 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/Makefile
+-rw-r--r--   0        0        0     3258 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/README.md
+-rwxr-xr-x   0        0        0     1121 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/dev/clean.sh
+-rw-r--r--   0        0        0     2115 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/dev/generate_clients.sh
+-rw-r--r--   0        0        0      974 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/dev/lint.sh
+-rw-r--r--   0        0        0      211 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/dev/openapi-python-client.yml
+-rwxr-xr-x   0        0        0     1391 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/dev/publish.sh
+-rw-r--r--   0        0        0      152 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/dev/schemas/README.md
+-rw-r--r--   0        0        0     1299 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/dev/schemas/download.sh
+-rw-r--r--   0        0        0   233795 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/dev/schemas/swagger.json
+-rwxr-xr-x   0        0        0     1023 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/dev/setup.sh
+-rwxr-xr-x   0        0        0      958 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/dev/test_python.sh
+-rw-r--r--   0        0        0      201 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/__init__.py
+-rw-r--r--   0        0        0       47 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/api/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/api/charts/__init__.py
+-rw-r--r--   0        0        0     4680 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/api/charts/post_chart_results.py
+-rw-r--r--   0        0        0        0 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/api/content/__init__.py
+-rw-r--r--   0        0        0     4483 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/api/content/get_pinned_items.py
+-rw-r--r--   0        0        0     5511 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/api/content/update_pinned_items_order.py
+-rw-r--r--   0        0        0        0 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/api/exploring/__init__.py
+-rw-r--r--   0        0        0     5017 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/api/exploring/post_run_query.py
+-rw-r--r--   0        0        0     5095 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/api/exploring/post_run_underlying_data_query.py
+-rw-r--r--   0        0        0        0 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/api/exports/__init__.py
+-rw-r--r--   0        0        0     3848 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/api/exports/get_csv_url.py
+-rw-r--r--   0        0        0        0 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/api/integrations/__init__.py
+-rw-r--r--   0        0        0     4403 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/api/integrations/delete_dbt_cloud_integration_settings.py
+-rw-r--r--   0        0        0     2743 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/api/integrations/get_dbt_cloud_integration_settings.py
+-rw-r--r--   0        0        0     4847 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/api/integrations/get_dbt_cloud_metrics.py
+-rw-r--r--   0        0        0     3651 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/api/integrations/get_slack_channels.py
+-rw-r--r--   0        0        0     2734 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/api/integrations/update_dbt_cloud_integration_settings.py
+-rw-r--r--   0        0        0        0 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/api/my_account/__init__.py
+-rw-r--r--   0        0        0     2573 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/api/my_account/create_email_one_time_passcode.py
+-rw-r--r--   0        0        0     3501 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/api/my_account/delete_me.py
+-rw-r--r--   0        0        0     3021 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/api/my_account/get_email_verification_status.py
+-rw-r--r--   0        0        0     4793 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/api/my_account/join_organization.py
+-rw-r--r--   0        0        0     4349 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/api/my_account/list_my_available_organizations.py
+-rw-r--r--   0        0        0        0 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/api/organizations/__init__.py
+-rw-r--r--   0        0        0     4634 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/api/organizations/create_group_in_organization.py
+-rw-r--r--   0        0        0     4256 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/api/organizations/delete_my_organization.py
+-rw-r--r--   0        0        0     4057 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/api/organizations/delete_organization_member.py
+-rw-r--r--   0        0        0     3589 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/api/organizations/get_my_organization.py
+-rw-r--r--   0        0        0     3739 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/api/organizations/list_groups_in_organization.py
+-rw-r--r--   0        0        0     3983 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/api/organizations/list_organization_email_domains.py
+-rw-r--r--   0        0        0     3859 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/api/organizations/list_organization_members.py
+-rw-r--r--   0        0        0     3771 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/api/organizations/list_organization_projects.py
+-rw-r--r--   0        0        0        0 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/api/projects/__init__.py
+-rw-r--r--   0        0        0     4691 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/api/projects/delete_validation_dismiss.py
+-rw-r--r--   0        0        0     5756 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/api/projects/get_latest_validation_results.py
+-rw-r--r--   0        0        0     2639 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/api/projects/get_project.py
+-rw-r--r--   0        0        0     4187 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/api/projects/list_charts_in_project.py
+-rw-r--r--   0        0        0     4187 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/api/projects/list_spaces_in_project.py
+-rw-r--r--   0        0        0     6428 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/api/projects/validate_project.py
+-rw-r--r--   0        0        0        0 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/api/roles_permissions/__init__.py
+-rw-r--r--   0        0        0     2984 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/api/roles_permissions/create_space_in_project.py
+-rw-r--r--   0        0        0     4928 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/api/roles_permissions/get_project_access_list.py
+-rw-r--r--   0        0        0     4648 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/api/roles_permissions/grant_project_access_to_user.py
+-rw-r--r--   0        0        0     4425 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/api/roles_permissions/revoke_project_access_for_user.py
+-rw-r--r--   0        0        0     4794 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/api/roles_permissions/revoke_space_access_for_user.py
+-rw-r--r--   0        0        0     5062 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/api/roles_permissions/update_organization_member.py
+-rw-r--r--   0        0        0     5026 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/api/roles_permissions/update_project_access_for_user.py
+-rw-r--r--   0        0        0        0 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/api/schedulers/__init__.py
+-rw-r--r--   0        0        0     4176 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/api/schedulers/delete_scheduler.py
+-rw-r--r--   0        0        0     4147 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/api/schedulers/get_scheduled_jobs.py
+-rw-r--r--   0        0        0     2633 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/api/schedulers/get_scheduler.py
+-rw-r--r--   0        0        0     4201 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/api/schedulers/get_scheduler_job_status.py
+-rw-r--r--   0        0        0     2620 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/api/schedulers/get_scheduler_logs.py
+-rw-r--r--   0        0        0     2919 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/api/schedulers/update_scheduler.py
+-rw-r--r--   0        0        0        0 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/api/share_links/__init__.py
+-rw-r--r--   0        0        0     3960 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/api/share_links/get_share_url.py
+-rw-r--r--   0        0        0        0 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/api/spaces/__init__.py
+-rw-r--r--   0        0        0     4429 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/api/spaces/delete_space.py
+-rw-r--r--   0        0        0     2881 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/api/spaces/get_space.py
+-rw-r--r--   0        0        0        0 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/api/ssh_keypairs/__init__.py
+-rw-r--r--   0        0        0     3542 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/api/ssh_keypairs/create_ssh_key_pair.py
+-rw-r--r--   0        0        0        0 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/api/user_groups/__init__.py
+-rw-r--r--   0        0        0     4365 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/api/user_groups/add_user_to_group.py
+-rw-r--r--   0        0        0     3927 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/api/user_groups/delete_group.py
+-rw-r--r--   0        0        0     3949 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/api/user_groups/get_group.py
+-rw-r--r--   0        0        0     4073 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/api/user_groups/get_group_members.py
+-rw-r--r--   0        0        0     4348 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/api/user_groups/remove_user_from_group.py
+-rw-r--r--   0        0        0     2906 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/client.py
+-rw-r--r--   0        0        0      470 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/errors.py
+-rw-r--r--   0        0        0    20611 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/__init__.py
+-rw-r--r--   0        0        0     4166 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/additional_metric.py
+-rw-r--r--   0        0        0     2422 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/allowed_email_domains.py
+-rw-r--r--   0        0        0     2410 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/api_chart_summary_list_response.py
+-rw-r--r--   0        0        0      152 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/api_chart_summary_list_response_status.py
+-rw-r--r--   0        0        0     2106 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/api_csv_url_response.py
+-rw-r--r--   0        0        0     1652 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/api_csv_url_response_results.py
+-rw-r--r--   0        0        0      142 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/api_csv_url_response_status.py
+-rw-r--r--   0        0        0     2254 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/api_dbt_cloud_metrics.py
+-rw-r--r--   0        0        0      143 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/api_dbt_cloud_metrics_status.py
+-rw-r--r--   0        0        0     2119 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/api_dbt_cloud_settings_delete_success.py
+-rw-r--r--   0        0        0      157 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/api_dbt_cloud_settings_delete_success_status.py
+-rw-r--r--   0        0        0      147 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/api_email_status_response_status.py
+-rw-r--r--   0        0        0     2139 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/api_error_payload.py
+-rw-r--r--   0        0        0     2386 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/api_error_payload_error.py
+-rw-r--r--   0        0        0      146 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/api_error_payload_status.py
+-rw-r--r--   0        0        0     2285 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/api_group_list_response.py
+-rw-r--r--   0        0        0      145 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/api_group_list_response_status.py
+-rw-r--r--   0        0        0     2359 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/api_group_members_response.py
+-rw-r--r--   0        0        0      148 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/api_group_members_response_status.py
+-rw-r--r--   0        0        0     1951 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/api_group_response.py
+-rw-r--r--   0        0        0      141 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/api_group_response_status.py
+-rw-r--r--   0        0        0     2208 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/api_job_scheduled_response.py
+-rw-r--r--   0        0        0     1548 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/api_job_scheduled_response_results.py
+-rw-r--r--   0        0        0      148 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/api_job_scheduled_response_status.py
+-rw-r--r--   0        0        0     2157 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/api_job_status_response.py
+-rw-r--r--   0        0        0     1535 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/api_job_status_response_results.py
+-rw-r--r--   0        0        0      145 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/api_job_status_response_status.py
+-rw-r--r--   0        0        0     2019 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/api_organization.py
+-rw-r--r--   0        0        0     2241 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/api_organization_allowed_email_domains.py
+-rw-r--r--   0        0        0      159 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/api_organization_allowed_email_domains_status.py
+-rw-r--r--   0        0        0     2270 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/api_organization_member_profile.py
+-rw-r--r--   0        0        0      153 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/api_organization_member_profile_status.py
+-rw-r--r--   0        0        0     2519 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/api_organization_member_profiles.py
+-rw-r--r--   0        0        0      154 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/api_organization_member_profiles_status.py
+-rw-r--r--   0        0        0     2456 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/api_organization_projects.py
+-rw-r--r--   0        0        0      148 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/api_organization_projects_status.py
+-rw-r--r--   0        0        0      140 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/api_organization_status.py
+-rw-r--r--   0        0        0     4825 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/api_pinned_items.py
+-rw-r--r--   0        0        0      139 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/api_pinned_items_status.py
+-rw-r--r--   0        0        0     2478 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/api_project_access_list_response.py
+-rw-r--r--   0        0        0      153 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/api_project_access_list_response_status.py
+-rw-r--r--   0        0        0      143 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/api_project_response_status.py
+-rw-r--r--   0        0        0     2140 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/api_run_query_response.py
+-rw-r--r--   0        0        0     2051 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/api_run_query_response_results.py
+-rw-r--r--   0        0        0      144 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/api_run_query_response_status.py
+-rw-r--r--   0        0        0     2383 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/api_scheduled_jobs_response.py
+-rw-r--r--   0        0        0      149 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/api_scheduled_jobs_response_status.py
+-rw-r--r--   0        0        0      155 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/api_scheduler_and_targets_response_status.py
+-rw-r--r--   0        0        0      149 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/api_scheduler_logs_response_status.py
+-rw-r--r--   0        0        0     2129 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/api_share_response.py
+-rw-r--r--   0        0        0      141 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/api_share_response_status.py
+-rw-r--r--   0        0        0     2376 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/api_slack_channels_response.py
+-rw-r--r--   0        0        0      149 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/api_slack_channels_response_status.py
+-rw-r--r--   0        0        0      141 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/api_space_response_status.py
+-rw-r--r--   0        0        0     2410 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/api_space_summary_list_response.py
+-rw-r--r--   0        0        0      152 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/api_space_summary_list_response_status.py
+-rw-r--r--   0        0        0     2208 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/api_ssh_key_pair_response.py
+-rw-r--r--   0        0        0      146 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/api_ssh_key_pair_response_status.py
+-rw-r--r--   0        0        0     1937 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/api_success_empty.py
+-rw-r--r--   0        0        0      140 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/api_success_empty_status.py
+-rw-r--r--   0        0        0     2569 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/api_user_allowed_organizations_response.py
+-rw-r--r--   0        0        0      160 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/api_user_allowed_organizations_response_status.py
+-rw-r--r--   0        0        0     4732 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/api_validate_response.py
+-rw-r--r--   0        0        0      144 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/api_validate_response_status.py
+-rw-r--r--   0        0        0     1737 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/api_validation_dismiss_response.py
+-rw-r--r--   0        0        0      153 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/api_validation_dismiss_response_status.py
+-rw-r--r--   0        0        0      316 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/chart_kind.py
+-rw-r--r--   0        0        0     3776 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/chart_summary.py
+-rw-r--r--   0        0        0      192 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/chart_type.py
+-rw-r--r--   0        0        0      220 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/compact.py
+-rw-r--r--   0        0        0      272 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/compact_or_alias_type_1.py
+-rw-r--r--   0        0        0     1937 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/create_project_member.py
+-rw-r--r--   0        0        0     2646 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/create_space.py
+-rw-r--r--   0        0        0     3745 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/dbt_azure_dev_ops_project_config.py
+-rw-r--r--   0        0        0     3814 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/dbt_bit_bucket_project_config.py
+-rw-r--r--   0        0        0     2425 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/dbt_cloud_ide_project_config.py
+-rw-r--r--   0        0        0     2229 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/dbt_cloud_metadata_response_metrics.py
+-rw-r--r--   0        0        0     2494 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/dbt_cloud_metric.py
+-rw-r--r--   0        0        0     3603 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/dbt_github_project_config.py
+-rw-r--r--   0        0        0     3603 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/dbt_gitlab_project_config.py
+-rw-r--r--   0        0        0     2957 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/dbt_local_project_config.py
+-rw-r--r--   0        0        0     2733 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/dbt_none_project_config.py
+-rw-r--r--   0        0        0     1664 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/dbt_project_environment_variable.py
+-rw-r--r--   0        0        0      295 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/dbt_project_type.py
+-rw-r--r--   0        0        0      164 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/dbt_project_type_azuredevops.py
+-rw-r--r--   0        0        0      156 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/dbt_project_type_bitbucket.py
+-rw-r--r--   0        0        0      138 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/dbt_project_type_dbt.py
+-rw-r--r--   0        0        0      166 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/dbt_project_type_dbtcloudide.py
+-rw-r--r--   0        0        0      147 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/dbt_project_type_github.py
+-rw-r--r--   0        0        0      147 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/dbt_project_type_gitlab.py
+-rw-r--r--   0        0        0      141 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/dbt_project_type_none.py
+-rw-r--r--   0        0        0     2051 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/delete_scheduler_response_201.py
+-rw-r--r--   0        0        0      151 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/delete_scheduler_response_201_status.py
+-rw-r--r--   0        0        0     2003 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/email_one_time_password.py
+-rw-r--r--   0        0        0     2749 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/email_one_time_password_expiring.py
+-rw-r--r--   0        0        0     2458 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/email_status.py
+-rw-r--r--   0        0        0     1664 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/filter_group_response_type_0.py
+-rw-r--r--   0        0        0     1674 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/filter_group_response_type_1.py
+-rw-r--r--   0        0        0     4615 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/filters.py
+-rw-r--r--   0        0        0     2247 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/group.py
+-rw-r--r--   0        0        0     2163 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/group_member.py
+-rw-r--r--   0        0        0     4963 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/metric_query_response.py
+-rw-r--r--   0        0        0      383 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/metric_type.py
+-rw-r--r--   0        0        0     2812 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/organization.py
+-rw-r--r--   0        0        0     3539 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/organization_member_profile.py
+-rw-r--r--   0        0        0     1670 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/organization_member_profile_update.py
+-rw-r--r--   0        0        0      287 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/organization_member_role.py
+-rw-r--r--   0        0        0     1991 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/organization_project.py
+-rw-r--r--   0        0        0     2377 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/partial_omit_organization_organization_uuid_or_needs_project.py
+-rw-r--r--   0        0        0     2628 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/partial_pick_space_is_private_or_access.py
+-rw-r--r--   0        0        0     2493 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/pick_allowed_email_domains_exclude_keyof_allowed_email_domains_organization_uuid.py
+-rw-r--r--   0        0        0     6235 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/pick_create_bigquery_credentials_exclude_keyof_create_bigquery_credentials_sensitive_credentials_field_names.py
+-rw-r--r--   0        0        0      267 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/pick_create_bigquery_credentials_exclude_keyof_create_bigquery_credentials_sensitive_credentials_field_names_priority.py
+-rw-r--r--   0        0        0     3905 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/pick_create_databricks_credentials_exclude_keyof_create_databricks_credentials_sensitive_credentials_field_names.py
+-rw-r--r--   0        0        0     1841 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/pick_create_dbt_cloud_integration_metrics_job_id.py
+-rw-r--r--   0        0        0     1565 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/pick_create_group_name.py
+-rw-r--r--   0        0        0     6859 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/pick_create_postgres_credentials_exclude_keyof_create_postgres_credentials_sensitive_credentials_field_names.py
+-rw-r--r--   0        0        0     6610 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/pick_create_redshift_credentials_exclude_keyof_create_redshift_credentials_sensitive_credentials_field_names.py
+-rw-r--r--   0        0        0     5207 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/pick_create_snowflake_credentials_exclude_keyof_create_snowflake_credentials_sensitive_credentials_field_names.py
+-rw-r--r--   0        0        0     3761 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/pick_create_trino_credentials_exclude_keyof_create_trino_credentials_sensitive_credentials_field_names.py
+-rw-r--r--   0        0        0     6625 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/pick_dashboard_uuid_or_name_or_description_or_updated_at_or_project_uuid_or_updated_by_user_or_organization_uuid_or_space_uuid_or_views_or_first_viewed_at_or_pinned_list_uuid_or_pinned_list_order.py
+-rw-r--r--   0        0        0     1532 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/pick_group_name.py
+-rw-r--r--   0        0        0     1566 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/pick_organization_name.py
+-rw-r--r--   0        0        0     2016 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/pick_resource_view_item_at_data_uuid_or_pinned_list_order.py
+-rw-r--r--   0        0        0     3781 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/pick_saved_chart_uuid_or_name_or_description_or_space_name_or_space_uuid_or_project_uuid_or_organization_uuid_or_pinned_list_uuid.py
+-rw-r--r--   0        0        0     4585 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/pick_saved_chart_uuid_or_name_or_updated_at_or_updated_by_user_or_description_or_space_uuid_or_pinned_list_uuid_or_pinned_list_order.py
+-rw-r--r--   0        0        0     1757 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/pick_share_url_path_or_params.py
+-rw-r--r--   0        0        0     1502 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/pick_space_name.py
+-rw-r--r--   0        0        0     1768 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/pick_space_name_or_is_private.py
+-rw-r--r--   0        0        0     2609 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/pick_space_organization_uuid_or_project_uuid_or_uuid_or_name_or_is_private.py
+-rw-r--r--   0        0        0     3420 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/pick_space_project_uuid_or_uuid_or_name_or_is_private_or_pinned_list_uuid_or_pinned_list_order_or_organization_uuid.py
+-rw-r--r--   0        0        0     1601 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/pick_space_share_user_uuid.py
+-rw-r--r--   0        0        0     1619 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/pick_ssh_key_pair_public_key.py
+-rw-r--r--   0        0        0     3860 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/pick_validation_response_base_exclude_keyof_validation_response_base_name.py
+-rw-r--r--   0        0        0     2266 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/pick_validation_response_error_or_created_at_or_validation_id.py
+-rw-r--r--   0        0        0     2095 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/post_chart_results_json_body.py
+-rw-r--r--   0        0        0     2540 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/project_member_profile.py
+-rw-r--r--   0        0        0      260 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/project_member_role.py
+-rw-r--r--   0        0        0      164 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/project_type.py
+-rw-r--r--   0        0        0     1294 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/record_string_any.py
+-rw-r--r--   0        0        0      193 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/resource_view_item_type.py
+-rw-r--r--   0        0        0      150 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/resource_view_item_type_chart.py
+-rw-r--r--   0        0        0      162 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/resource_view_item_type_dashboard.py
+-rw-r--r--   0        0        0      150 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/resource_view_item_type_space.py
+-rw-r--r--   0        0        0     2093 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/resource_view_space_item.py
+-rw-r--r--   0        0        0     3903 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/resource_view_space_item_data.py
+-rw-r--r--   0        0        0     5334 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/run_query_request.py
+-rw-r--r--   0        0        0     1933 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/run_query_request_filters.py
+-rw-r--r--   0        0        0     1661 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/scheduled_jobs.py
+-rw-r--r--   0        0        0     4958 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/scheduler_base.py
+-rw-r--r--   0        0        0     2484 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/scheduler_csv_options.py
+-rw-r--r--   0        0        0      170 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/scheduler_csv_options_limit_type_1.py
+-rw-r--r--   0        0        0     2685 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/scheduler_email_target.py
+-rw-r--r--   0        0        0      156 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/scheduler_format.py
+-rw-r--r--   0        0        0     1272 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/scheduler_image_options.py
+-rw-r--r--   0        0        0      223 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/scheduler_job_status.py
+-rw-r--r--   0        0        0     5049 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/scheduler_log.py
+-rw-r--r--   0        0        0      167 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/scheduler_log_target_type.py
+-rw-r--r--   0        0        0      443 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/scheduler_log_task.py
+-rw-r--r--   0        0        0     2665 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/scheduler_slack_target.py
+-rw-r--r--   0        0        0     3505 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/share_url.py
+-rw-r--r--   0        0        0     1553 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/slack_channel.py
+-rw-r--r--   0        0        0     1658 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/sort_field.py
+-rw-r--r--   0        0        0     2115 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/space_share.py
+-rw-r--r--   0        0        0     2480 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/space_summary.py
+-rw-r--r--   0        0        0     2119 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/table_calculation.py
+-rw-r--r--   0        0        0     2350 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/update_pinned_item_order.py
+-rw-r--r--   0        0        0     1582 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/update_project_member.py
+-rw-r--r--   0        0        0     1173 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/updated_by_user.py
+-rw-r--r--   0        0        0     1993 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/user_allowed_organization.py
+-rw-r--r--   0        0        0     1964 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/validate_project_json_body.py
+-rw-r--r--   0        0        0     6492 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/validation_error_chart_response.py
+-rw-r--r--   0        0        0     5966 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/validation_error_dashboard_response.py
+-rw-r--r--   0        0        0      260 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/validation_error_type.py
+-rw-r--r--   0        0        0     3709 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/validation_response_base.py
+-rw-r--r--   0        0        0      193 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/validation_source_type.py
+-rw-r--r--   0        0        0     2633 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/view_statistics.py
+-rw-r--r--   0        0        0      153 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/warehouse_types_bigquery.py
+-rw-r--r--   0        0        0      159 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/warehouse_types_databricks.py
+-rw-r--r--   0        0        0      153 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/warehouse_types_postgres.py
+-rw-r--r--   0        0        0      153 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/warehouse_types_redshift.py
+-rw-r--r--   0        0        0      156 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/warehouse_types_snowflake.py
+-rw-r--r--   0        0        0      144 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/warehouse_types_trino.py
+-rw-r--r--   0        0        0      225 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/week_day.py
+-rw-r--r--   0        0        0       26 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/py.typed
+-rw-r--r--   0        0        0     1101 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/types.py
+-rw-r--r--   0        0        0     1624 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/pyproject.toml
+-rw-r--r--   0        0        0      830 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/setup.py
+-rw-r--r--   0        0        0      796 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/tests/__init__.py
+-rw-r--r--   0        0        0      908 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/tests/test_dummy.py
+-rw-r--r--   0        0        0     5168 1970-01-01 00:00:00.000000 lightdash_client_python-0.619.1/PKG-INFO
```

### Comparing `lightdash_client_python-0.618.0/.github/CODEOWNERS` & `lightdash_client_python-0.619.1/.github/CODEOWNERS`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.618.0/.github/workflows/publish.yml` & `lightdash_client_python-0.619.1/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.618.0/.github/workflows/test-publish.yml` & `lightdash_client_python-0.619.1/.github/workflows/test-publish.yml`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.618.0/.github/workflows/test.yml` & `lightdash_client_python-0.619.1/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.618.0/.gitignore` & `lightdash_client_python-0.619.1/.gitignore`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.618.0/.openapi-generator-ignore` & `lightdash_client_python-0.619.1/.openapi-generator-ignore`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.618.0/.openapi-generator/FILES` & `lightdash_client_python-0.619.1/.openapi-generator/FILES`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.618.0/.pre-commit-config.yaml` & `lightdash_client_python-0.619.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.618.0/.pylintrc` & `lightdash_client_python-0.619.1/.pylintrc`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.618.0/LICENSE` & `lightdash_client_python-0.619.1/LICENSE`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.618.0/Makefile` & `lightdash_client_python-0.619.1/Makefile`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.618.0/README.md` & `lightdash_client_python-0.619.1/README.md`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.618.0/dev/clean.sh` & `lightdash_client_python-0.619.1/dev/clean.sh`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.618.0/dev/generate_clients.sh` & `lightdash_client_python-0.619.1/dev/generate_clients.sh`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.618.0/dev/lint.sh` & `lightdash_client_python-0.619.1/dev/lint.sh`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.618.0/dev/publish.sh` & `lightdash_client_python-0.619.1/dev/publish.sh`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.618.0/dev/schemas/download.sh` & `lightdash_client_python-0.619.1/dev/schemas/download.sh`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.618.0/dev/schemas/swagger.json` & `lightdash_client_python-0.619.1/dev/schemas/swagger.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9915975168510075%*

 * *Differences: {"'components'": "{'schemas': {'OrganizationMemberProfileUpdate': {replace: "*

 * *                 "OrderedDict([('properties', OrderedDict([('role', OrderedDict([('$ref', "*

 * *                 "'#/components/schemas/OrganizationMemberRole')]))])), ('required', ['role']), "*

 * *                 "('type', 'object')])}, "*

 * *                 "'Pick_AllowedEmailDomains.Exclude_keyofAllowedEmailDomains.organizationUuid__': "*

 * *                 "{'required': {insert: [(1, 'role')], delete: [0]}}, delete: "*

 * *                 "['P […]*

```diff
@@ -1759,15 +1759,23 @@
                     "lastName",
                     "firstName",
                     "userUuid"
                 ],
                 "type": "object"
             },
             "OrganizationMemberProfileUpdate": {
-                "$ref": "#/components/schemas/Partial_Pick_OrganizationMemberProfile.role__"
+                "properties": {
+                    "role": {
+                        "$ref": "#/components/schemas/OrganizationMemberRole"
+                    }
+                },
+                "required": [
+                    "role"
+                ],
+                "type": "object"
             },
             "OrganizationMemberRole": {
                 "enum": [
                     "member",
                     "viewer",
                     "interactive_viewer",
                     "editor",
@@ -1811,24 +1819,14 @@
                     "name": {
                         "description": "The name of the organization",
                         "type": "string"
                     }
                 },
                 "type": "object"
             },
-            "Partial_Pick_OrganizationMemberProfile.role__": {
-                "description": "Make all properties in T optional",
-                "properties": {
-                    "role": {
-                        "$ref": "#/components/schemas/OrganizationMemberRole",
-                        "description": "The role of the user in the organization"
-                    }
-                },
-                "type": "object"
-            },
             "Partial_Pick_Space.isPrivate-or-access__": {
                 "description": "Make all properties in T optional",
                 "properties": {
                     "access": {
                         "items": {
                             "$ref": "#/components/schemas/SpaceShare"
                         },
@@ -1856,16 +1854,16 @@
                         "type": "array"
                     },
                     "role": {
                         "$ref": "#/components/schemas/OrganizationMemberRole"
                     }
                 },
                 "required": [
-                    "role",
                     "emailDomains",
+                    "role",
                     "projectUuids"
                 ],
                 "type": "object"
             },
             "Pick_CreateBigqueryCredentials.Exclude_keyofCreateBigqueryCredentials.SensitiveCredentialsFieldNames__": {
                 "description": "From T, pick a set of properties whose keys are in the union K",
                 "properties": {
@@ -3951,15 +3949,15 @@
             "url": "https://docs.lightdash.com/help-and-contact/contact/contact_info/"
         },
         "description": "Open API documentation for all public Lightdash API endpoints",
         "license": {
             "name": "MIT"
         },
         "title": "Lightdash API",
-        "version": "0.616.2"
+        "version": "0.618.1"
     },
     "openapi": "3.0.0",
     "paths": {
         "/api/v1/csv/{jobId}": {
             "get": {
                 "description": "Get a Csv",
                 "operationId": "getCsvUrl",
@@ -5961,14 +5959,22 @@
         },
         "/api/v1/projects/{projectUuid}/validate/{validationId}": {
             "delete": {
                 "description": "Deletes a single validation error.",
                 "operationId": "DeleteValidationDismiss",
                 "parameters": [
                     {
+                        "in": "path",
+                        "name": "projectUuid",
+                        "required": true,
+                        "schema": {
+                            "type": "string"
+                        }
+                    },
+                    {
                         "description": "the projectId for the validation",
                         "in": "path",
                         "name": "validationId",
                         "required": true,
                         "schema": {
                             "format": "double",
                             "type": "number"
```

### Comparing `lightdash_client_python-0.618.0/dev/setup.sh` & `lightdash_client_python-0.619.1/dev/setup.sh`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.618.0/dev/test_python.sh` & `lightdash_client_python-0.619.1/dev/test_python.sh`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.618.0/lightdash_client/api/charts/post_chart_results.py` & `lightdash_client_python-0.619.1/lightdash_client/api/charts/post_chart_results.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.618.0/lightdash_client/api/content/get_pinned_items.py` & `lightdash_client_python-0.619.1/lightdash_client/api/content/get_pinned_items.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.618.0/lightdash_client/api/content/update_pinned_items_order.py` & `lightdash_client_python-0.619.1/lightdash_client/api/content/update_pinned_items_order.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.618.0/lightdash_client/api/exploring/post_run_query.py` & `lightdash_client_python-0.619.1/lightdash_client/api/exploring/post_run_query.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.618.0/lightdash_client/api/exploring/post_run_underlying_data_query.py` & `lightdash_client_python-0.619.1/lightdash_client/api/exploring/post_run_underlying_data_query.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.618.0/lightdash_client/api/exports/get_csv_url.py` & `lightdash_client_python-0.619.1/lightdash_client/api/exports/get_csv_url.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.618.0/lightdash_client/api/integrations/delete_dbt_cloud_integration_settings.py` & `lightdash_client_python-0.619.1/lightdash_client/api/integrations/delete_dbt_cloud_integration_settings.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.618.0/lightdash_client/api/integrations/get_dbt_cloud_integration_settings.py` & `lightdash_client_python-0.619.1/lightdash_client/api/integrations/get_dbt_cloud_integration_settings.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.618.0/lightdash_client/api/integrations/get_dbt_cloud_metrics.py` & `lightdash_client_python-0.619.1/lightdash_client/api/integrations/get_dbt_cloud_metrics.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.618.0/lightdash_client/api/integrations/get_slack_channels.py` & `lightdash_client_python-0.619.1/lightdash_client/api/integrations/get_slack_channels.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.618.0/lightdash_client/api/integrations/update_dbt_cloud_integration_settings.py` & `lightdash_client_python-0.619.1/lightdash_client/api/integrations/update_dbt_cloud_integration_settings.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.618.0/lightdash_client/api/my_account/create_email_one_time_passcode.py` & `lightdash_client_python-0.619.1/lightdash_client/api/my_account/create_email_one_time_passcode.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.618.0/lightdash_client/api/my_account/delete_me.py` & `lightdash_client_python-0.619.1/lightdash_client/api/my_account/delete_me.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.618.0/lightdash_client/api/my_account/get_email_verification_status.py` & `lightdash_client_python-0.619.1/lightdash_client/api/my_account/get_email_verification_status.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.618.0/lightdash_client/api/my_account/join_organization.py` & `lightdash_client_python-0.619.1/lightdash_client/api/my_account/join_organization.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.618.0/lightdash_client/api/my_account/list_my_available_organizations.py` & `lightdash_client_python-0.619.1/lightdash_client/api/my_account/list_my_available_organizations.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.618.0/lightdash_client/api/organizations/create_group_in_organization.py` & `lightdash_client_python-0.619.1/lightdash_client/api/organizations/create_group_in_organization.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.618.0/lightdash_client/api/organizations/delete_my_organization.py` & `lightdash_client_python-0.619.1/lightdash_client/api/organizations/delete_my_organization.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.618.0/lightdash_client/api/organizations/delete_organization_member.py` & `lightdash_client_python-0.619.1/lightdash_client/api/organizations/delete_organization_member.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.618.0/lightdash_client/api/organizations/get_my_organization.py` & `lightdash_client_python-0.619.1/lightdash_client/api/organizations/get_my_organization.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.618.0/lightdash_client/api/organizations/list_groups_in_organization.py` & `lightdash_client_python-0.619.1/lightdash_client/api/organizations/list_groups_in_organization.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.618.0/lightdash_client/api/organizations/list_organization_email_domains.py` & `lightdash_client_python-0.619.1/lightdash_client/api/organizations/list_organization_email_domains.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.618.0/lightdash_client/api/organizations/list_organization_members.py` & `lightdash_client_python-0.619.1/lightdash_client/api/organizations/list_organization_members.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.618.0/lightdash_client/api/organizations/list_organization_projects.py` & `lightdash_client_python-0.619.1/lightdash_client/api/organizations/list_organization_projects.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.618.0/lightdash_client/api/projects/get_latest_validation_results.py` & `lightdash_client_python-0.619.1/lightdash_client/api/projects/get_latest_validation_results.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.618.0/lightdash_client/api/projects/get_project.py` & `lightdash_client_python-0.619.1/lightdash_client/api/projects/get_project.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.618.0/lightdash_client/api/projects/list_charts_in_project.py` & `lightdash_client_python-0.619.1/lightdash_client/api/projects/list_charts_in_project.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.618.0/lightdash_client/api/projects/list_spaces_in_project.py` & `lightdash_client_python-0.619.1/lightdash_client/api/projects/list_spaces_in_project.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.618.0/lightdash_client/api/projects/validate_project.py` & `lightdash_client_python-0.619.1/lightdash_client/api/projects/validate_project.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.618.0/lightdash_client/api/roles_permissions/create_space_in_project.py` & `lightdash_client_python-0.619.1/lightdash_client/api/roles_permissions/create_space_in_project.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.618.0/lightdash_client/api/roles_permissions/get_project_access_list.py` & `lightdash_client_python-0.619.1/lightdash_client/api/roles_permissions/get_project_access_list.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.618.0/lightdash_client/api/roles_permissions/grant_project_access_to_user.py` & `lightdash_client_python-0.619.1/lightdash_client/api/roles_permissions/grant_project_access_to_user.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.618.0/lightdash_client/api/roles_permissions/revoke_project_access_for_user.py` & `lightdash_client_python-0.619.1/lightdash_client/api/roles_permissions/revoke_project_access_for_user.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.618.0/lightdash_client/api/roles_permissions/revoke_space_access_for_user.py` & `lightdash_client_python-0.619.1/lightdash_client/api/roles_permissions/revoke_space_access_for_user.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.618.0/lightdash_client/api/roles_permissions/update_project_access_for_user.py` & `lightdash_client_python-0.619.1/lightdash_client/api/roles_permissions/update_project_access_for_user.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.618.0/lightdash_client/api/schedulers/delete_scheduler.py` & `lightdash_client_python-0.619.1/lightdash_client/api/schedulers/delete_scheduler.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.618.0/lightdash_client/api/schedulers/get_scheduled_jobs.py` & `lightdash_client_python-0.619.1/lightdash_client/api/schedulers/get_scheduled_jobs.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.618.0/lightdash_client/api/schedulers/get_scheduler.py` & `lightdash_client_python-0.619.1/lightdash_client/api/schedulers/get_scheduler.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.618.0/lightdash_client/api/schedulers/get_scheduler_job_status.py` & `lightdash_client_python-0.619.1/lightdash_client/api/schedulers/get_scheduler_job_status.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.618.0/lightdash_client/api/schedulers/get_scheduler_logs.py` & `lightdash_client_python-0.619.1/lightdash_client/api/schedulers/get_scheduler_logs.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.618.0/lightdash_client/api/schedulers/update_scheduler.py` & `lightdash_client_python-0.619.1/lightdash_client/api/schedulers/update_scheduler.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.618.0/lightdash_client/api/share_links/get_share_url.py` & `lightdash_client_python-0.619.1/lightdash_client/api/share_links/get_share_url.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.618.0/lightdash_client/api/spaces/delete_space.py` & `lightdash_client_python-0.619.1/lightdash_client/api/spaces/delete_space.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.618.0/lightdash_client/api/spaces/get_space.py` & `lightdash_client_python-0.619.1/lightdash_client/api/spaces/get_space.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.618.0/lightdash_client/api/ssh_keypairs/create_ssh_key_pair.py` & `lightdash_client_python-0.619.1/lightdash_client/api/ssh_keypairs/create_ssh_key_pair.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.618.0/lightdash_client/api/user_groups/add_user_to_group.py` & `lightdash_client_python-0.619.1/lightdash_client/api/user_groups/add_user_to_group.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.618.0/lightdash_client/api/user_groups/delete_group.py` & `lightdash_client_python-0.619.1/lightdash_client/api/user_groups/delete_group.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.618.0/lightdash_client/api/user_groups/get_group.py` & `lightdash_client_python-0.619.1/lightdash_client/api/user_groups/get_group.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.618.0/lightdash_client/api/user_groups/get_group_members.py` & `lightdash_client_python-0.619.1/lightdash_client/api/user_groups/get_group_members.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.618.0/lightdash_client/api/user_groups/remove_user_from_group.py` & `lightdash_client_python-0.619.1/lightdash_client/api/user_groups/remove_user_from_group.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.618.0/lightdash_client/client.py` & `lightdash_client_python-0.619.1/lightdash_client/client.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.618.0/lightdash_client/models/__init__.py` & `lightdash_client_python-0.619.1/lightdash_client/models/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -100,20 +100,20 @@
 from .filters import Filters
 from .group import Group
 from .group_member import GroupMember
 from .metric_query_response import MetricQueryResponse
 from .metric_type import MetricType
 from .organization import Organization
 from .organization_member_profile import OrganizationMemberProfile
+from .organization_member_profile_update import OrganizationMemberProfileUpdate
 from .organization_member_role import OrganizationMemberRole
 from .organization_project import OrganizationProject
 from .partial_omit_organization_organization_uuid_or_needs_project import (
     PartialOmitOrganizationOrganizationUuidOrNeedsProject,
 )
-from .partial_pick_organization_member_profile_role import PartialPickOrganizationMemberProfileRole
 from .partial_pick_space_is_private_or_access import PartialPickSpaceIsPrivateOrAccess
 from .pick_allowed_email_domains_exclude_keyof_allowed_email_domains_organization_uuid import (
     PickAllowedEmailDomainsExcludeKeyofAllowedEmailDomainsOrganizationUuid,
 )
 from .pick_create_bigquery_credentials_exclude_keyof_create_bigquery_credentials_sensitive_credentials_field_names import (
     PickCreateBigqueryCredentialsExcludeKeyofCreateBigqueryCredentialsSensitiveCredentialsFieldNames,
 )
@@ -318,18 +318,18 @@
     "Filters",
     "Group",
     "GroupMember",
     "MetricQueryResponse",
     "MetricType",
     "Organization",
     "OrganizationMemberProfile",
+    "OrganizationMemberProfileUpdate",
     "OrganizationMemberRole",
     "OrganizationProject",
     "PartialOmitOrganizationOrganizationUuidOrNeedsProject",
-    "PartialPickOrganizationMemberProfileRole",
     "PartialPickSpaceIsPrivateOrAccess",
     "PickAllowedEmailDomainsExcludeKeyofAllowedEmailDomainsOrganizationUuid",
     "PickCreateBigqueryCredentialsExcludeKeyofCreateBigqueryCredentialsSensitiveCredentialsFieldNames",
     "PickCreateBigqueryCredentialsExcludeKeyofCreateBigqueryCredentialsSensitiveCredentialsFieldNamesPriority",
     "PickCreateDatabricksCredentialsExcludeKeyofCreateDatabricksCredentialsSensitiveCredentialsFieldNames",
     "PickCreateDbtCloudIntegrationMetricsJobId",
     "PickCreateGroupName",
```

### Comparing `lightdash_client_python-0.618.0/lightdash_client/models/additional_metric.py` & `lightdash_client_python-0.619.1/lightdash_client/models/additional_metric.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.618.0/lightdash_client/models/allowed_email_domains.py` & `lightdash_client_python-0.619.1/lightdash_client/models/allowed_email_domains.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.618.0/lightdash_client/models/api_chart_summary_list_response.py` & `lightdash_client_python-0.619.1/lightdash_client/models/api_chart_summary_list_response.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.618.0/lightdash_client/models/api_csv_url_response.py` & `lightdash_client_python-0.619.1/lightdash_client/models/api_csv_url_response.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.618.0/lightdash_client/models/api_csv_url_response_results.py` & `lightdash_client_python-0.619.1/lightdash_client/models/api_csv_url_response_results.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.618.0/lightdash_client/models/api_dbt_cloud_metrics.py` & `lightdash_client_python-0.619.1/lightdash_client/models/api_dbt_cloud_metrics.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.618.0/lightdash_client/models/api_dbt_cloud_settings_delete_success.py` & `lightdash_client_python-0.619.1/lightdash_client/models/api_dbt_cloud_settings_delete_success.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.618.0/lightdash_client/models/api_error_payload.py` & `lightdash_client_python-0.619.1/lightdash_client/models/api_error_payload.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.618.0/lightdash_client/models/api_error_payload_error.py` & `lightdash_client_python-0.619.1/lightdash_client/models/api_error_payload_error.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.618.0/lightdash_client/models/api_group_list_response.py` & `lightdash_client_python-0.619.1/lightdash_client/models/api_group_list_response.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.618.0/lightdash_client/models/api_group_members_response.py` & `lightdash_client_python-0.619.1/lightdash_client/models/api_group_members_response.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.618.0/lightdash_client/models/api_group_response.py` & `lightdash_client_python-0.619.1/lightdash_client/models/api_group_response.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.618.0/lightdash_client/models/api_job_scheduled_response.py` & `lightdash_client_python-0.619.1/lightdash_client/models/api_job_scheduled_response.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.618.0/lightdash_client/models/api_job_scheduled_response_results.py` & `lightdash_client_python-0.619.1/lightdash_client/models/api_job_scheduled_response_results.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.618.0/lightdash_client/models/api_job_status_response.py` & `lightdash_client_python-0.619.1/lightdash_client/models/api_job_status_response.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.618.0/lightdash_client/models/api_job_status_response_results.py` & `lightdash_client_python-0.619.1/lightdash_client/models/api_job_status_response_results.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.618.0/lightdash_client/models/api_organization.py` & `lightdash_client_python-0.619.1/lightdash_client/models/api_organization.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.618.0/lightdash_client/models/api_organization_allowed_email_domains.py` & `lightdash_client_python-0.619.1/lightdash_client/models/api_organization_allowed_email_domains.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.618.0/lightdash_client/models/api_organization_member_profile.py` & `lightdash_client_python-0.619.1/lightdash_client/models/api_organization_member_profile.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.618.0/lightdash_client/models/api_organization_member_profiles.py` & `lightdash_client_python-0.619.1/lightdash_client/models/api_organization_member_profiles.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.618.0/lightdash_client/models/api_organization_projects.py` & `lightdash_client_python-0.619.1/lightdash_client/models/api_organization_projects.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.618.0/lightdash_client/models/api_pinned_items.py` & `lightdash_client_python-0.619.1/lightdash_client/models/api_pinned_items.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.618.0/lightdash_client/models/api_project_access_list_response.py` & `lightdash_client_python-0.619.1/lightdash_client/models/api_project_access_list_response.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.618.0/lightdash_client/models/api_run_query_response.py` & `lightdash_client_python-0.619.1/lightdash_client/models/api_run_query_response.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.618.0/lightdash_client/models/api_run_query_response_results.py` & `lightdash_client_python-0.619.1/lightdash_client/models/api_run_query_response_results.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.618.0/lightdash_client/models/api_scheduled_jobs_response.py` & `lightdash_client_python-0.619.1/lightdash_client/models/api_scheduled_jobs_response.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.618.0/lightdash_client/models/api_share_response.py` & `lightdash_client_python-0.619.1/lightdash_client/models/api_share_response.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.618.0/lightdash_client/models/api_slack_channels_response.py` & `lightdash_client_python-0.619.1/lightdash_client/models/api_slack_channels_response.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.618.0/lightdash_client/models/api_space_summary_list_response.py` & `lightdash_client_python-0.619.1/lightdash_client/models/api_space_summary_list_response.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.618.0/lightdash_client/models/api_ssh_key_pair_response.py` & `lightdash_client_python-0.619.1/lightdash_client/models/api_ssh_key_pair_response.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.618.0/lightdash_client/models/api_success_empty.py` & `lightdash_client_python-0.619.1/lightdash_client/models/api_success_empty.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.618.0/lightdash_client/models/api_user_allowed_organizations_response.py` & `lightdash_client_python-0.619.1/lightdash_client/models/api_user_allowed_organizations_response.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.618.0/lightdash_client/models/api_validate_response.py` & `lightdash_client_python-0.619.1/lightdash_client/models/api_validate_response.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.618.0/lightdash_client/models/api_validation_dismiss_response.py` & `lightdash_client_python-0.619.1/lightdash_client/models/api_validation_dismiss_response.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.618.0/lightdash_client/models/chart_summary.py` & `lightdash_client_python-0.619.1/lightdash_client/models/chart_summary.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.618.0/lightdash_client/models/create_project_member.py` & `lightdash_client_python-0.619.1/lightdash_client/models/create_project_member.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.618.0/lightdash_client/models/create_space.py` & `lightdash_client_python-0.619.1/lightdash_client/models/create_space.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.618.0/lightdash_client/models/dbt_azure_dev_ops_project_config.py` & `lightdash_client_python-0.619.1/lightdash_client/models/dbt_azure_dev_ops_project_config.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.618.0/lightdash_client/models/dbt_bit_bucket_project_config.py` & `lightdash_client_python-0.619.1/lightdash_client/models/dbt_bit_bucket_project_config.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.618.0/lightdash_client/models/dbt_cloud_ide_project_config.py` & `lightdash_client_python-0.619.1/lightdash_client/models/dbt_cloud_ide_project_config.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.618.0/lightdash_client/models/dbt_cloud_metadata_response_metrics.py` & `lightdash_client_python-0.619.1/lightdash_client/models/dbt_cloud_metadata_response_metrics.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.618.0/lightdash_client/models/dbt_cloud_metric.py` & `lightdash_client_python-0.619.1/lightdash_client/models/dbt_cloud_metric.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.618.0/lightdash_client/models/dbt_github_project_config.py` & `lightdash_client_python-0.619.1/lightdash_client/models/dbt_github_project_config.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.618.0/lightdash_client/models/dbt_gitlab_project_config.py` & `lightdash_client_python-0.619.1/lightdash_client/models/dbt_gitlab_project_config.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.618.0/lightdash_client/models/dbt_local_project_config.py` & `lightdash_client_python-0.619.1/lightdash_client/models/dbt_local_project_config.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.618.0/lightdash_client/models/dbt_none_project_config.py` & `lightdash_client_python-0.619.1/lightdash_client/models/dbt_none_project_config.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.618.0/lightdash_client/models/dbt_project_environment_variable.py` & `lightdash_client_python-0.619.1/lightdash_client/models/dbt_project_environment_variable.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.618.0/lightdash_client/models/delete_scheduler_response_201.py` & `lightdash_client_python-0.619.1/lightdash_client/models/delete_scheduler_response_201.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.618.0/lightdash_client/models/email_one_time_password.py` & `lightdash_client_python-0.619.1/lightdash_client/models/email_one_time_password.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.618.0/lightdash_client/models/email_one_time_password_expiring.py` & `lightdash_client_python-0.619.1/lightdash_client/models/email_one_time_password_expiring.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.618.0/lightdash_client/models/email_status.py` & `lightdash_client_python-0.619.1/lightdash_client/models/email_status.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.618.0/lightdash_client/models/filter_group_response_type_0.py` & `lightdash_client_python-0.619.1/lightdash_client/models/filter_group_response_type_0.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.618.0/lightdash_client/models/filter_group_response_type_1.py` & `lightdash_client_python-0.619.1/lightdash_client/models/filter_group_response_type_1.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.618.0/lightdash_client/models/filters.py` & `lightdash_client_python-0.619.1/lightdash_client/models/filters.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.618.0/lightdash_client/models/group.py` & `lightdash_client_python-0.619.1/lightdash_client/models/group.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.618.0/lightdash_client/models/group_member.py` & `lightdash_client_python-0.619.1/lightdash_client/models/group_member.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.618.0/lightdash_client/models/metric_query_response.py` & `lightdash_client_python-0.619.1/lightdash_client/models/metric_query_response.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.618.0/lightdash_client/models/organization.py` & `lightdash_client_python-0.619.1/lightdash_client/models/organization.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.618.0/lightdash_client/models/organization_member_profile.py` & `lightdash_client_python-0.619.1/lightdash_client/models/organization_member_profile.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.618.0/lightdash_client/models/organization_project.py` & `lightdash_client_python-0.619.1/lightdash_client/models/organization_project.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.618.0/lightdash_client/models/partial_omit_organization_organization_uuid_or_needs_project.py` & `lightdash_client_python-0.619.1/lightdash_client/models/partial_omit_organization_organization_uuid_or_needs_project.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.618.0/lightdash_client/models/partial_pick_organization_member_profile_role.py` & `lightdash_client_python-0.619.1/lightdash_client/models/partial_pick_space_is_private_or_access.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,63 +1,81 @@
 from typing import Any
 from typing import Dict
 from typing import List
 from typing import Type
+from typing import TYPE_CHECKING
 from typing import TypeVar
 from typing import Union
 
 import attr
 
-from ..models.organization_member_role import OrganizationMemberRole
 from ..types import UNSET
 from ..types import Unset
 
-T = TypeVar("T", bound="PartialPickOrganizationMemberProfileRole")
+if TYPE_CHECKING:
+    from ..models.space_share import SpaceShare
+
+
+T = TypeVar("T", bound="PartialPickSpaceIsPrivateOrAccess")
 
 
 @attr.s(auto_attribs=True)
-class PartialPickOrganizationMemberProfileRole:
+class PartialPickSpaceIsPrivateOrAccess:
     """Make all properties in T optional
 
     Attributes:
-        role (Union[Unset, OrganizationMemberRole]):
+        is_private (Union[Unset, bool]):
+        access (Union[Unset, List['SpaceShare']]):
     """
 
-    role: Union[Unset, OrganizationMemberRole] = UNSET
+    is_private: Union[Unset, bool] = UNSET
+    access: Union[Unset, List["SpaceShare"]] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
-        role: Union[Unset, str] = UNSET
-        if not isinstance(self.role, Unset):
-            role = self.role.value
+        is_private = self.is_private
+        access: Union[Unset, List[Dict[str, Any]]] = UNSET
+        if not isinstance(self.access, Unset):
+            access = []
+            for access_item_data in self.access:
+                access_item = access_item_data.to_dict()
+
+                access.append(access_item)
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({})
-        if role is not UNSET:
-            field_dict["role"] = role
+        if is_private is not UNSET:
+            field_dict["isPrivate"] = is_private
+        if access is not UNSET:
+            field_dict["access"] = access
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
+        from ..models.space_share import SpaceShare
+
         d = src_dict.copy()
-        _role = d.pop("role", UNSET)
-        role: Union[Unset, OrganizationMemberRole]
-        if isinstance(_role, Unset):
-            role = UNSET
-        else:
-            role = OrganizationMemberRole(_role)
+        is_private = d.pop("isPrivate", UNSET)
 
-        partial_pick_organization_member_profile_role = cls(
-            role=role,
+        access = []
+        _access = d.pop("access", UNSET)
+        for access_item_data in _access or []:
+            access_item = SpaceShare.from_dict(access_item_data)
+
+            access.append(access_item)
+
+        partial_pick_space_is_private_or_access = cls(
+            is_private=is_private,
+            access=access,
         )
 
-        partial_pick_organization_member_profile_role.additional_properties = d
-        return partial_pick_organization_member_profile_role
+        partial_pick_space_is_private_or_access.additional_properties = d
+        return partial_pick_space_is_private_or_access
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `lightdash_client_python-0.618.0/lightdash_client/models/partial_pick_space_is_private_or_access.py` & `lightdash_client_python-0.619.1/lightdash_client/models/post_chart_results_json_body.py`

 * *Files 27% similar despite different names*

```diff
@@ -8,74 +8,61 @@
 
 import attr
 
 from ..types import UNSET
 from ..types import Unset
 
 if TYPE_CHECKING:
-    from ..models.space_share import SpaceShare
+    from ..models.filters import Filters
 
 
-T = TypeVar("T", bound="PartialPickSpaceIsPrivateOrAccess")
+T = TypeVar("T", bound="PostChartResultsJsonBody")
 
 
 @attr.s(auto_attribs=True)
-class PartialPickSpaceIsPrivateOrAccess:
-    """Make all properties in T optional
-
+class PostChartResultsJsonBody:
+    """
     Attributes:
-        is_private (Union[Unset, bool]):
-        access (Union[Unset, List['SpaceShare']]):
+        filters (Union[Unset, Filters]):
     """
 
-    is_private: Union[Unset, bool] = UNSET
-    access: Union[Unset, List["SpaceShare"]] = UNSET
+    filters: Union[Unset, "Filters"] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
-        is_private = self.is_private
-        access: Union[Unset, List[Dict[str, Any]]] = UNSET
-        if not isinstance(self.access, Unset):
-            access = []
-            for access_item_data in self.access:
-                access_item = access_item_data.to_dict()
-
-                access.append(access_item)
+        filters: Union[Unset, Dict[str, Any]] = UNSET
+        if not isinstance(self.filters, Unset):
+            filters = self.filters.to_dict()
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({})
-        if is_private is not UNSET:
-            field_dict["isPrivate"] = is_private
-        if access is not UNSET:
-            field_dict["access"] = access
+        if filters is not UNSET:
+            field_dict["filters"] = filters
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        from ..models.space_share import SpaceShare
+        from ..models.filters import Filters
 
         d = src_dict.copy()
-        is_private = d.pop("isPrivate", UNSET)
+        _filters = d.pop("filters", UNSET)
+        filters: Union[Unset, Filters]
+        if isinstance(_filters, Unset):
+            filters = UNSET
+        else:
+            filters = Filters.from_dict(_filters)
 
-        access = []
-        _access = d.pop("access", UNSET)
-        for access_item_data in _access or []:
-            access_item = SpaceShare.from_dict(access_item_data)
-
-            access.append(access_item)
-
-        partial_pick_space_is_private_or_access = cls(
-            is_private=is_private,
-            access=access,
+        post_chart_results_json_body = cls(
+            filters=filters,
         )
 
-        partial_pick_space_is_private_or_access.additional_properties = d
-        return partial_pick_space_is_private_or_access
+        post_chart_results_json_body.additional_properties = d
+        return post_chart_results_json_body
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `lightdash_client_python-0.618.0/lightdash_client/models/pick_allowed_email_domains_exclude_keyof_allowed_email_domains_organization_uuid.py` & `lightdash_client_python-0.619.1/lightdash_client/models/pick_allowed_email_domains_exclude_keyof_allowed_email_domains_organization_uuid.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -13,55 +13,55 @@
 
 
 @attr.s(auto_attribs=True)
 class PickAllowedEmailDomainsExcludeKeyofAllowedEmailDomainsOrganizationUuid:
     """From T, pick a set of properties whose keys are in the union K
 
     Attributes:
-        role (OrganizationMemberRole):
         email_domains (List[str]):
+        role (OrganizationMemberRole):
         project_uuids (List[str]):
     """
 
-    role: OrganizationMemberRole
     email_domains: List[str]
+    role: OrganizationMemberRole
     project_uuids: List[str]
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
-        role = self.role.value
-
         email_domains = self.email_domains
 
+        role = self.role.value
+
         project_uuids = self.project_uuids
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update(
             {
-                "role": role,
                 "emailDomains": email_domains,
+                "role": role,
                 "projectUuids": project_uuids,
             }
         )
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
-        role = OrganizationMemberRole(d.pop("role"))
-
         email_domains = cast(List[str], d.pop("emailDomains"))
 
+        role = OrganizationMemberRole(d.pop("role"))
+
         project_uuids = cast(List[str], d.pop("projectUuids"))
 
         pick_allowed_email_domains_exclude_keyof_allowed_email_domains_organization_uuid = cls(
-            role=role,
             email_domains=email_domains,
+            role=role,
             project_uuids=project_uuids,
         )
 
         pick_allowed_email_domains_exclude_keyof_allowed_email_domains_organization_uuid.additional_properties = d
         return pick_allowed_email_domains_exclude_keyof_allowed_email_domains_organization_uuid
 
     @property
```

### Comparing `lightdash_client_python-0.618.0/lightdash_client/models/pick_create_bigquery_credentials_exclude_keyof_create_bigquery_credentials_sensitive_credentials_field_names.py` & `lightdash_client_python-0.619.1/lightdash_client/models/pick_create_bigquery_credentials_exclude_keyof_create_bigquery_credentials_sensitive_credentials_field_names.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.618.0/lightdash_client/models/pick_create_databricks_credentials_exclude_keyof_create_databricks_credentials_sensitive_credentials_field_names.py` & `lightdash_client_python-0.619.1/lightdash_client/models/pick_create_databricks_credentials_exclude_keyof_create_databricks_credentials_sensitive_credentials_field_names.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.618.0/lightdash_client/models/pick_create_dbt_cloud_integration_metrics_job_id.py` & `lightdash_client_python-0.619.1/lightdash_client/models/pick_create_dbt_cloud_integration_metrics_job_id.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.618.0/lightdash_client/models/pick_create_group_name.py` & `lightdash_client_python-0.619.1/lightdash_client/models/pick_create_group_name.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.618.0/lightdash_client/models/pick_create_postgres_credentials_exclude_keyof_create_postgres_credentials_sensitive_credentials_field_names.py` & `lightdash_client_python-0.619.1/lightdash_client/models/pick_create_postgres_credentials_exclude_keyof_create_postgres_credentials_sensitive_credentials_field_names.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.618.0/lightdash_client/models/pick_create_redshift_credentials_exclude_keyof_create_redshift_credentials_sensitive_credentials_field_names.py` & `lightdash_client_python-0.619.1/lightdash_client/models/pick_create_redshift_credentials_exclude_keyof_create_redshift_credentials_sensitive_credentials_field_names.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.618.0/lightdash_client/models/pick_create_snowflake_credentials_exclude_keyof_create_snowflake_credentials_sensitive_credentials_field_names.py` & `lightdash_client_python-0.619.1/lightdash_client/models/pick_create_snowflake_credentials_exclude_keyof_create_snowflake_credentials_sensitive_credentials_field_names.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.618.0/lightdash_client/models/pick_create_trino_credentials_exclude_keyof_create_trino_credentials_sensitive_credentials_field_names.py` & `lightdash_client_python-0.619.1/lightdash_client/models/pick_create_trino_credentials_exclude_keyof_create_trino_credentials_sensitive_credentials_field_names.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.618.0/lightdash_client/models/pick_dashboard_uuid_or_name_or_description_or_updated_at_or_project_uuid_or_updated_by_user_or_organization_uuid_or_space_uuid_or_views_or_first_viewed_at_or_pinned_list_uuid_or_pinned_list_order.py` & `lightdash_client_python-0.619.1/lightdash_client/models/pick_dashboard_uuid_or_name_or_description_or_updated_at_or_project_uuid_or_updated_by_user_or_organization_uuid_or_space_uuid_or_views_or_first_viewed_at_or_pinned_list_uuid_or_pinned_list_order.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.618.0/lightdash_client/models/pick_group_name.py` & `lightdash_client_python-0.619.1/lightdash_client/models/pick_group_name.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.618.0/lightdash_client/models/pick_organization_name.py` & `lightdash_client_python-0.619.1/lightdash_client/models/pick_organization_name.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.618.0/lightdash_client/models/pick_resource_view_item_at_data_uuid_or_pinned_list_order.py` & `lightdash_client_python-0.619.1/lightdash_client/models/pick_resource_view_item_at_data_uuid_or_pinned_list_order.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.618.0/lightdash_client/models/pick_saved_chart_uuid_or_name_or_description_or_space_name_or_space_uuid_or_project_uuid_or_organization_uuid_or_pinned_list_uuid.py` & `lightdash_client_python-0.619.1/lightdash_client/models/pick_saved_chart_uuid_or_name_or_description_or_space_name_or_space_uuid_or_project_uuid_or_organization_uuid_or_pinned_list_uuid.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.618.0/lightdash_client/models/pick_saved_chart_uuid_or_name_or_updated_at_or_updated_by_user_or_description_or_space_uuid_or_pinned_list_uuid_or_pinned_list_order.py` & `lightdash_client_python-0.619.1/lightdash_client/models/pick_saved_chart_uuid_or_name_or_updated_at_or_updated_by_user_or_description_or_space_uuid_or_pinned_list_uuid_or_pinned_list_order.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.618.0/lightdash_client/models/pick_share_url_path_or_params.py` & `lightdash_client_python-0.619.1/lightdash_client/models/pick_share_url_path_or_params.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.618.0/lightdash_client/models/pick_space_name.py` & `lightdash_client_python-0.619.1/lightdash_client/models/pick_space_name.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.618.0/lightdash_client/models/pick_space_name_or_is_private.py` & `lightdash_client_python-0.619.1/lightdash_client/models/pick_space_name_or_is_private.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.618.0/lightdash_client/models/pick_space_organization_uuid_or_project_uuid_or_uuid_or_name_or_is_private.py` & `lightdash_client_python-0.619.1/lightdash_client/models/pick_space_organization_uuid_or_project_uuid_or_uuid_or_name_or_is_private.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.618.0/lightdash_client/models/pick_space_project_uuid_or_uuid_or_name_or_is_private_or_pinned_list_uuid_or_pinned_list_order_or_organization_uuid.py` & `lightdash_client_python-0.619.1/lightdash_client/models/pick_space_project_uuid_or_uuid_or_name_or_is_private_or_pinned_list_uuid_or_pinned_list_order_or_organization_uuid.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.618.0/lightdash_client/models/pick_space_share_user_uuid.py` & `lightdash_client_python-0.619.1/lightdash_client/models/pick_space_share_user_uuid.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.618.0/lightdash_client/models/pick_ssh_key_pair_public_key.py` & `lightdash_client_python-0.619.1/lightdash_client/models/pick_ssh_key_pair_public_key.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.618.0/lightdash_client/models/pick_validation_response_base_exclude_keyof_validation_response_base_name.py` & `lightdash_client_python-0.619.1/lightdash_client/models/pick_validation_response_base_exclude_keyof_validation_response_base_name.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.618.0/lightdash_client/models/pick_validation_response_error_or_created_at_or_validation_id.py` & `lightdash_client_python-0.619.1/lightdash_client/models/pick_validation_response_error_or_created_at_or_validation_id.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.618.0/lightdash_client/models/post_chart_results_json_body.py` & `lightdash_client_python-0.619.1/lightdash_client/models/slack_channel.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,68 +1,59 @@
 from typing import Any
 from typing import Dict
 from typing import List
 from typing import Type
-from typing import TYPE_CHECKING
 from typing import TypeVar
-from typing import Union
 
 import attr
 
-from ..types import UNSET
-from ..types import Unset
-
-if TYPE_CHECKING:
-    from ..models.filters import Filters
-
-
-T = TypeVar("T", bound="PostChartResultsJsonBody")
+T = TypeVar("T", bound="SlackChannel")
 
 
 @attr.s(auto_attribs=True)
-class PostChartResultsJsonBody:
+class SlackChannel:
     """
     Attributes:
-        filters (Union[Unset, Filters]):
+        name (str):
+        id (str):
     """
 
-    filters: Union[Unset, "Filters"] = UNSET
+    name: str
+    id: str
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
-        filters: Union[Unset, Dict[str, Any]] = UNSET
-        if not isinstance(self.filters, Unset):
-            filters = self.filters.to_dict()
+        name = self.name
+        id = self.id
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
-        field_dict.update({})
-        if filters is not UNSET:
-            field_dict["filters"] = filters
+        field_dict.update(
+            {
+                "name": name,
+                "id": id,
+            }
+        )
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        from ..models.filters import Filters
-
         d = src_dict.copy()
-        _filters = d.pop("filters", UNSET)
-        filters: Union[Unset, Filters]
-        if isinstance(_filters, Unset):
-            filters = UNSET
-        else:
-            filters = Filters.from_dict(_filters)
+        name = d.pop("name")
+
+        id = d.pop("id")
 
-        post_chart_results_json_body = cls(
-            filters=filters,
+        slack_channel = cls(
+            name=name,
+            id=id,
         )
 
-        post_chart_results_json_body.additional_properties = d
-        return post_chart_results_json_body
+        slack_channel.additional_properties = d
+        return slack_channel
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `lightdash_client_python-0.618.0/lightdash_client/models/project_member_profile.py` & `lightdash_client_python-0.619.1/lightdash_client/models/project_member_profile.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.618.0/lightdash_client/models/record_string_any.py` & `lightdash_client_python-0.619.1/lightdash_client/models/record_string_any.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.618.0/lightdash_client/models/resource_view_space_item.py` & `lightdash_client_python-0.619.1/lightdash_client/models/resource_view_space_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.618.0/lightdash_client/models/resource_view_space_item_data.py` & `lightdash_client_python-0.619.1/lightdash_client/models/resource_view_space_item_data.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.618.0/lightdash_client/models/run_query_request.py` & `lightdash_client_python-0.619.1/lightdash_client/models/run_query_request.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.618.0/lightdash_client/models/run_query_request_filters.py` & `lightdash_client_python-0.619.1/lightdash_client/models/run_query_request_filters.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.618.0/lightdash_client/models/scheduled_jobs.py` & `lightdash_client_python-0.619.1/lightdash_client/models/scheduled_jobs.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.618.0/lightdash_client/models/scheduler_base.py` & `lightdash_client_python-0.619.1/lightdash_client/models/scheduler_base.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.618.0/lightdash_client/models/scheduler_csv_options.py` & `lightdash_client_python-0.619.1/lightdash_client/models/scheduler_csv_options.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.618.0/lightdash_client/models/scheduler_email_target.py` & `lightdash_client_python-0.619.1/lightdash_client/models/scheduler_email_target.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.618.0/lightdash_client/models/scheduler_image_options.py` & `lightdash_client_python-0.619.1/lightdash_client/models/scheduler_image_options.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.618.0/lightdash_client/models/scheduler_log.py` & `lightdash_client_python-0.619.1/lightdash_client/models/scheduler_log.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.618.0/lightdash_client/models/scheduler_slack_target.py` & `lightdash_client_python-0.619.1/lightdash_client/models/scheduler_slack_target.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.618.0/lightdash_client/models/share_url.py` & `lightdash_client_python-0.619.1/lightdash_client/models/share_url.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.618.0/lightdash_client/models/slack_channel.py` & `lightdash_client_python-0.619.1/lightdash_client/models/organization_member_profile_update.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,58 +2,53 @@
 from typing import Dict
 from typing import List
 from typing import Type
 from typing import TypeVar
 
 import attr
 
-T = TypeVar("T", bound="SlackChannel")
+from ..models.organization_member_role import OrganizationMemberRole
+
+T = TypeVar("T", bound="OrganizationMemberProfileUpdate")
 
 
 @attr.s(auto_attribs=True)
-class SlackChannel:
+class OrganizationMemberProfileUpdate:
     """
     Attributes:
-        name (str):
-        id (str):
+        role (OrganizationMemberRole):
     """
 
-    name: str
-    id: str
+    role: OrganizationMemberRole
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
-        name = self.name
-        id = self.id
+        role = self.role.value
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update(
             {
-                "name": name,
-                "id": id,
+                "role": role,
             }
         )
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
-        name = d.pop("name")
-
-        id = d.pop("id")
+        role = OrganizationMemberRole(d.pop("role"))
 
-        slack_channel = cls(
-            name=name,
-            id=id,
+        organization_member_profile_update = cls(
+            role=role,
         )
 
-        slack_channel.additional_properties = d
-        return slack_channel
+        organization_member_profile_update.additional_properties = d
+        return organization_member_profile_update
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `lightdash_client_python-0.618.0/lightdash_client/models/sort_field.py` & `lightdash_client_python-0.619.1/lightdash_client/models/sort_field.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.618.0/lightdash_client/models/space_share.py` & `lightdash_client_python-0.619.1/lightdash_client/models/space_share.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.618.0/lightdash_client/models/space_summary.py` & `lightdash_client_python-0.619.1/lightdash_client/models/space_summary.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.618.0/lightdash_client/models/table_calculation.py` & `lightdash_client_python-0.619.1/lightdash_client/models/table_calculation.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.618.0/lightdash_client/models/update_pinned_item_order.py` & `lightdash_client_python-0.619.1/lightdash_client/models/update_pinned_item_order.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.618.0/lightdash_client/models/update_project_member.py` & `lightdash_client_python-0.619.1/lightdash_client/models/update_project_member.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.618.0/lightdash_client/models/updated_by_user.py` & `lightdash_client_python-0.619.1/lightdash_client/models/updated_by_user.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.618.0/lightdash_client/models/user_allowed_organization.py` & `lightdash_client_python-0.619.1/lightdash_client/models/user_allowed_organization.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.618.0/lightdash_client/models/validate_project_json_body.py` & `lightdash_client_python-0.619.1/lightdash_client/models/validate_project_json_body.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.618.0/lightdash_client/models/validation_error_chart_response.py` & `lightdash_client_python-0.619.1/lightdash_client/models/validation_error_chart_response.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.618.0/lightdash_client/models/validation_error_dashboard_response.py` & `lightdash_client_python-0.619.1/lightdash_client/models/validation_error_dashboard_response.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.618.0/lightdash_client/models/validation_response_base.py` & `lightdash_client_python-0.619.1/lightdash_client/models/validation_response_base.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.618.0/lightdash_client/models/view_statistics.py` & `lightdash_client_python-0.619.1/lightdash_client/models/view_statistics.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.618.0/lightdash_client/types.py` & `lightdash_client_python-0.619.1/lightdash_client/types.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.618.0/pyproject.toml` & `lightdash_client_python-0.619.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.618.0/setup.py` & `lightdash_client_python-0.619.1/setup.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.618.0/tests/__init__.py` & `lightdash_client_python-0.619.1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.618.0/tests/test_dummy.py` & `lightdash_client_python-0.619.1/tests/test_dummy.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.618.0/PKG-INFO` & `lightdash_client_python-0.619.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lightdash-client-python
-Version: 0.618.0
+Version: 0.619.1
 Summary: A client library for accessing Lightdash API 
 Author: yu-iskw
 Requires-Python: >=3.8.0,<4
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
```

