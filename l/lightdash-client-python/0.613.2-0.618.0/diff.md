# Comparing `tmp/lightdash_client_python-0.613.2.tar.gz` & `tmp/lightdash_client_python-0.618.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lightdash_client_python-0.613.2.tar", last modified: Thu Jun 15 08:00:02 2023, max compression
+gzip compressed data, was "lightdash_client_python-0.618.0.tar", last modified: Mon Jun 19 00:37:07 2023, max compression
```

## Comparing `lightdash_client_python-0.613.2.tar` & `lightdash_client_python-0.618.0.tar`

### file list

```diff
@@ -1,250 +1,287 @@
--rw-r--r--   0        0        0      804 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/.github/CODEOWNERS
--rw-r--r--   0        0        0      402 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/.github/workflows/contributors-list.yml
--rw-r--r--   0        0        0     1849 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/.github/workflows/publish.yml
--rw-r--r--   0        0        0     2335 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/.github/workflows/test-publish.yml
--rw-r--r--   0        0        0     1115 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/.github/workflows/test.yml
--rw-r--r--   0        0        0     3078 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/.gitignore
--rw-r--r--   0        0        0     1040 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/.openapi-generator-ignore
--rw-r--r--   0        0        0     6821 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/.openapi-generator/FILES
--rw-r--r--   0        0        0        6 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/.openapi-generator/VERSION
--rw-r--r--   0        0        0     1266 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0    14088 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/.pylintrc
--rw-r--r--   0        0        0      150 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/.pypirc
--rw-r--r--   0        0        0        8 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/.python-version
--rw-r--r--   0        0        0       32 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/.style.yapf
--rw-r--r--   0        0        0    11357 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/LICENSE
--rw-r--r--   0        0        0      717 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/Makefile
--rw-r--r--   0        0        0     3258 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/README.md
--rwxr-xr-x   0        0        0     1121 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/dev/clean.sh
--rw-r--r--   0        0        0     2115 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/dev/generate_clients.sh
--rw-r--r--   0        0        0      974 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/dev/lint.sh
--rw-r--r--   0        0        0      211 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/dev/openapi-python-client.yml
--rwxr-xr-x   0        0        0     1391 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/dev/publish.sh
--rw-r--r--   0        0        0      152 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/dev/schemas/README.md
--rw-r--r--   0        0        0     1249 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/dev/schemas/download.sh
--rw-r--r--   0        0        0   200027 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/dev/schemas/swagger.json
--rwxr-xr-x   0        0        0     1023 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/dev/setup.sh
--rwxr-xr-x   0        0        0      958 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/dev/test_python.sh
--rw-r--r--   0        0        0      201 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/__init__.py
--rw-r--r--   0        0        0       47 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/api/__init__.py
--rw-r--r--   0        0        0        0 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/api/charts/__init__.py
--rw-r--r--   0        0        0     4680 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/api/charts/post_chart_results.py
--rw-r--r--   0        0        0        0 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/api/content/__init__.py
--rw-r--r--   0        0        0     4483 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/api/content/get_pinned_items.py
--rw-r--r--   0        0        0     5511 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/api/content/update_pinned_items_order.py
--rw-r--r--   0        0        0        0 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/api/exploring/__init__.py
--rw-r--r--   0        0        0     5017 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/api/exploring/post_run_query.py
--rw-r--r--   0        0        0     5095 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/api/exploring/post_run_underlying_data_query.py
--rw-r--r--   0        0        0        0 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/api/exports/__init__.py
--rw-r--r--   0        0        0     3848 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/api/exports/get_csv_url.py
--rw-r--r--   0        0        0        0 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/api/integrations/__init__.py
--rw-r--r--   0        0        0     4403 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/api/integrations/delete_dbt_cloud_integration_settings.py
--rw-r--r--   0        0        0     2743 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/api/integrations/get_dbt_cloud_integration_settings.py
--rw-r--r--   0        0        0     4847 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/api/integrations/get_dbt_cloud_metrics.py
--rw-r--r--   0        0        0     3651 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/api/integrations/get_slack_channels.py
--rw-r--r--   0        0        0     2734 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/api/integrations/update_dbt_cloud_integration_settings.py
--rw-r--r--   0        0        0        0 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/api/my_account/__init__.py
--rw-r--r--   0        0        0     2573 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/api/my_account/create_email_one_time_passcode.py
--rw-r--r--   0        0        0     3501 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/api/my_account/delete_me.py
--rw-r--r--   0        0        0     3021 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/api/my_account/get_email_verification_status.py
--rw-r--r--   0        0        0     4793 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/api/my_account/join_organization.py
--rw-r--r--   0        0        0     4349 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/api/my_account/list_my_available_organizations.py
--rw-r--r--   0        0        0        0 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/api/organizations/__init__.py
--rw-r--r--   0        0        0     4634 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/api/organizations/create_group_in_organization.py
--rw-r--r--   0        0        0     4256 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/api/organizations/delete_my_organization.py
--rw-r--r--   0        0        0     4057 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/api/organizations/delete_organization_member.py
--rw-r--r--   0        0        0     3589 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/api/organizations/get_my_organization.py
--rw-r--r--   0        0        0     3739 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/api/organizations/list_groups_in_organization.py
--rw-r--r--   0        0        0     3983 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/api/organizations/list_organization_email_domains.py
--rw-r--r--   0        0        0     3859 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/api/organizations/list_organization_members.py
--rw-r--r--   0        0        0        0 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/api/projects/__init__.py
--rw-r--r--   0        0        0     5756 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/api/projects/get_latest_validation_results.py
--rw-r--r--   0        0        0     4187 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/api/projects/list_charts_in_project.py
--rw-r--r--   0        0        0     4187 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/api/projects/list_spaces_in_project.py
--rw-r--r--   0        0        0     6428 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/api/projects/validate_project.py
--rw-r--r--   0        0        0        0 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/api/roles_permissions/__init__.py
--rw-r--r--   0        0        0     2984 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/api/roles_permissions/create_space_in_project.py
--rw-r--r--   0        0        0     4928 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/api/roles_permissions/get_project_access_list.py
--rw-r--r--   0        0        0     4648 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/api/roles_permissions/grant_project_access_to_user.py
--rw-r--r--   0        0        0     4425 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/api/roles_permissions/revoke_project_access_for_user.py
--rw-r--r--   0        0        0     4794 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/api/roles_permissions/revoke_space_access_for_user.py
--rw-r--r--   0        0        0     5026 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/api/roles_permissions/update_project_access_for_user.py
--rw-r--r--   0        0        0        0 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/api/schedulers/__init__.py
--rw-r--r--   0        0        0     4176 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/api/schedulers/delete_scheduler.py
--rw-r--r--   0        0        0     4147 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/api/schedulers/get_scheduled_jobs.py
--rw-r--r--   0        0        0     2633 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/api/schedulers/get_scheduler.py
--rw-r--r--   0        0        0     4201 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/api/schedulers/get_scheduler_job_status.py
--rw-r--r--   0        0        0     2620 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/api/schedulers/get_scheduler_logs.py
--rw-r--r--   0        0        0     2919 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/api/schedulers/update_scheduler.py
--rw-r--r--   0        0        0        0 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/api/share_links/__init__.py
--rw-r--r--   0        0        0     3960 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/api/share_links/get_share_url.py
--rw-r--r--   0        0        0        0 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/api/spaces/__init__.py
--rw-r--r--   0        0        0     4429 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/api/spaces/delete_space.py
--rw-r--r--   0        0        0     2881 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/api/spaces/get_space.py
--rw-r--r--   0        0        0        0 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/api/ssh_keypairs/__init__.py
--rw-r--r--   0        0        0     3542 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/api/ssh_keypairs/create_ssh_key_pair.py
--rw-r--r--   0        0        0        0 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/api/user_groups/__init__.py
--rw-r--r--   0        0        0     4365 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/api/user_groups/add_user_to_group.py
--rw-r--r--   0        0        0     3927 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/api/user_groups/delete_group.py
--rw-r--r--   0        0        0     3949 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/api/user_groups/get_group.py
--rw-r--r--   0        0        0     4073 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/api/user_groups/get_group_members.py
--rw-r--r--   0        0        0     4348 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/api/user_groups/remove_user_from_group.py
--rw-r--r--   0        0        0     2906 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/client.py
--rw-r--r--   0        0        0      470 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/errors.py
--rw-r--r--   0        0        0    15782 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/__init__.py
--rw-r--r--   0        0        0     4166 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/additional_metric.py
--rw-r--r--   0        0        0     2422 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/allowed_email_domains.py
--rw-r--r--   0        0        0     2410 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/api_chart_summary_list_response.py
--rw-r--r--   0        0        0      152 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/api_chart_summary_list_response_status.py
--rw-r--r--   0        0        0     2106 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/api_csv_url_response.py
--rw-r--r--   0        0        0     1652 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/api_csv_url_response_results.py
--rw-r--r--   0        0        0      142 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/api_csv_url_response_status.py
--rw-r--r--   0        0        0     2254 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/api_dbt_cloud_metrics.py
--rw-r--r--   0        0        0      143 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/api_dbt_cloud_metrics_status.py
--rw-r--r--   0        0        0     2119 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/api_dbt_cloud_settings_delete_success.py
--rw-r--r--   0        0        0      157 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/api_dbt_cloud_settings_delete_success_status.py
--rw-r--r--   0        0        0      147 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/api_email_status_response_status.py
--rw-r--r--   0        0        0     2139 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/api_error_payload.py
--rw-r--r--   0        0        0     2386 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/api_error_payload_error.py
--rw-r--r--   0        0        0      146 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/api_error_payload_status.py
--rw-r--r--   0        0        0     2285 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/api_group_list_response.py
--rw-r--r--   0        0        0      145 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/api_group_list_response_status.py
--rw-r--r--   0        0        0     2359 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/api_group_members_response.py
--rw-r--r--   0        0        0      148 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/api_group_members_response_status.py
--rw-r--r--   0        0        0     1951 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/api_group_response.py
--rw-r--r--   0        0        0      141 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/api_group_response_status.py
--rw-r--r--   0        0        0     2208 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/api_job_scheduled_response.py
--rw-r--r--   0        0        0     1548 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/api_job_scheduled_response_results.py
--rw-r--r--   0        0        0      148 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/api_job_scheduled_response_status.py
--rw-r--r--   0        0        0     2157 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/api_job_status_response.py
--rw-r--r--   0        0        0     1535 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/api_job_status_response_results.py
--rw-r--r--   0        0        0      145 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/api_job_status_response_status.py
--rw-r--r--   0        0        0     2019 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/api_organization.py
--rw-r--r--   0        0        0     2241 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/api_organization_allowed_email_domains.py
--rw-r--r--   0        0        0      159 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/api_organization_allowed_email_domains_status.py
--rw-r--r--   0        0        0     2270 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/api_organization_member_profile.py
--rw-r--r--   0        0        0      153 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/api_organization_member_profile_status.py
--rw-r--r--   0        0        0     2519 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/api_organization_member_profiles.py
--rw-r--r--   0        0        0      154 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/api_organization_member_profiles_status.py
--rw-r--r--   0        0        0      140 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/api_organization_status.py
--rw-r--r--   0        0        0     4825 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/api_pinned_items.py
--rw-r--r--   0        0        0      139 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/api_pinned_items_status.py
--rw-r--r--   0        0        0     2478 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/api_project_access_list_response.py
--rw-r--r--   0        0        0      153 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/api_project_access_list_response_status.py
--rw-r--r--   0        0        0     2140 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/api_run_query_response.py
--rw-r--r--   0        0        0     2051 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/api_run_query_response_results.py
--rw-r--r--   0        0        0      144 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/api_run_query_response_status.py
--rw-r--r--   0        0        0     2383 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/api_scheduled_jobs_response.py
--rw-r--r--   0        0        0      149 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/api_scheduled_jobs_response_status.py
--rw-r--r--   0        0        0      155 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/api_scheduler_and_targets_response_status.py
--rw-r--r--   0        0        0      149 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/api_scheduler_logs_response_status.py
--rw-r--r--   0        0        0     2129 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/api_share_response.py
--rw-r--r--   0        0        0      141 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/api_share_response_status.py
--rw-r--r--   0        0        0     2376 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/api_slack_channels_response.py
--rw-r--r--   0        0        0      149 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/api_slack_channels_response_status.py
--rw-r--r--   0        0        0      141 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/api_space_response_status.py
--rw-r--r--   0        0        0     2410 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/api_space_summary_list_response.py
--rw-r--r--   0        0        0      152 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/api_space_summary_list_response_status.py
--rw-r--r--   0        0        0     2208 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/api_ssh_key_pair_response.py
--rw-r--r--   0        0        0      146 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/api_ssh_key_pair_response_status.py
--rw-r--r--   0        0        0     1937 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/api_success_empty.py
--rw-r--r--   0        0        0      140 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/api_success_empty_status.py
--rw-r--r--   0        0        0     2569 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/api_user_allowed_organizations_response.py
--rw-r--r--   0        0        0      160 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/api_user_allowed_organizations_response_status.py
--rw-r--r--   0        0        0     4732 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/api_validate_response.py
--rw-r--r--   0        0        0      144 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/api_validate_response_status.py
--rw-r--r--   0        0        0     1737 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/api_validation_dismiss_response.py
--rw-r--r--   0        0        0      153 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/api_validation_dismiss_response_status.py
--rw-r--r--   0        0        0      316 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/chart_kind.py
--rw-r--r--   0        0        0     3776 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/chart_summary.py
--rw-r--r--   0        0        0      192 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/chart_type.py
--rw-r--r--   0        0        0      220 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/compact.py
--rw-r--r--   0        0        0      272 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/compact_or_alias_type_1.py
--rw-r--r--   0        0        0     1937 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/create_project_member.py
--rw-r--r--   0        0        0     2646 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/create_space.py
--rw-r--r--   0        0        0     2229 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/dbt_cloud_metadata_response_metrics.py
--rw-r--r--   0        0        0     2494 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/dbt_cloud_metric.py
--rw-r--r--   0        0        0     2051 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/delete_scheduler_response_201.py
--rw-r--r--   0        0        0      151 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/delete_scheduler_response_201_status.py
--rw-r--r--   0        0        0     2003 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/email_one_time_password.py
--rw-r--r--   0        0        0     2749 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/email_one_time_password_expiring.py
--rw-r--r--   0        0        0     2458 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/email_status.py
--rw-r--r--   0        0        0     1664 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/filter_group_response_type_0.py
--rw-r--r--   0        0        0     1674 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/filter_group_response_type_1.py
--rw-r--r--   0        0        0     4615 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/filters.py
--rw-r--r--   0        0        0     2247 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/group.py
--rw-r--r--   0        0        0     2163 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/group_member.py
--rw-r--r--   0        0        0     4963 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/metric_query_response.py
--rw-r--r--   0        0        0      383 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/metric_type.py
--rw-r--r--   0        0        0     2812 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/organization.py
--rw-r--r--   0        0        0     3539 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/organization_member_profile.py
--rw-r--r--   0        0        0      287 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/organization_member_role.py
--rw-r--r--   0        0        0     2377 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/partial_omit_organization_organization_uuid_or_needs_project.py
--rw-r--r--   0        0        0     2120 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/partial_pick_organization_member_profile_role.py
--rw-r--r--   0        0        0     2628 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/partial_pick_space_is_private_or_access.py
--rw-r--r--   0        0        0     2493 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/pick_allowed_email_domains_exclude_keyof_allowed_email_domains_organization_uuid.py
--rw-r--r--   0        0        0     1841 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/pick_create_dbt_cloud_integration_metrics_job_id.py
--rw-r--r--   0        0        0     1565 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/pick_create_group_name.py
--rw-r--r--   0        0        0     6625 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/pick_dashboard_uuid_or_name_or_description_or_updated_at_or_project_uuid_or_updated_by_user_or_organization_uuid_or_space_uuid_or_views_or_first_viewed_at_or_pinned_list_uuid_or_pinned_list_order.py
--rw-r--r--   0        0        0     1532 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/pick_group_name.py
--rw-r--r--   0        0        0     1566 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/pick_organization_name.py
--rw-r--r--   0        0        0     2016 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/pick_resource_view_item_at_data_uuid_or_pinned_list_order.py
--rw-r--r--   0        0        0     3781 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/pick_saved_chart_uuid_or_name_or_description_or_space_name_or_space_uuid_or_project_uuid_or_organization_uuid_or_pinned_list_uuid.py
--rw-r--r--   0        0        0     4585 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/pick_saved_chart_uuid_or_name_or_updated_at_or_updated_by_user_or_description_or_space_uuid_or_pinned_list_uuid_or_pinned_list_order.py
--rw-r--r--   0        0        0     1757 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/pick_share_url_path_or_params.py
--rw-r--r--   0        0        0     1502 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/pick_space_name.py
--rw-r--r--   0        0        0     1768 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/pick_space_name_or_is_private.py
--rw-r--r--   0        0        0     2609 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/pick_space_organization_uuid_or_project_uuid_or_uuid_or_name_or_is_private.py
--rw-r--r--   0        0        0     3420 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/pick_space_project_uuid_or_uuid_or_name_or_is_private_or_pinned_list_uuid_or_pinned_list_order_or_organization_uuid.py
--rw-r--r--   0        0        0     1601 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/pick_space_share_user_uuid.py
--rw-r--r--   0        0        0     1619 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/pick_ssh_key_pair_public_key.py
--rw-r--r--   0        0        0     3860 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/pick_validation_response_base_exclude_keyof_validation_response_base_name.py
--rw-r--r--   0        0        0     2266 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/pick_validation_response_error_or_created_at_or_validation_id.py
--rw-r--r--   0        0        0     2095 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/post_chart_results_json_body.py
--rw-r--r--   0        0        0     2540 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/project_member_profile.py
--rw-r--r--   0        0        0      260 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/project_member_role.py
--rw-r--r--   0        0        0     1294 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/record_string_any.py
--rw-r--r--   0        0        0      193 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/resource_view_item_type.py
--rw-r--r--   0        0        0      150 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/resource_view_item_type_chart.py
--rw-r--r--   0        0        0      162 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/resource_view_item_type_dashboard.py
--rw-r--r--   0        0        0      150 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/resource_view_item_type_space.py
--rw-r--r--   0        0        0     2093 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/resource_view_space_item.py
--rw-r--r--   0        0        0     3903 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/resource_view_space_item_data.py
--rw-r--r--   0        0        0     5334 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/run_query_request.py
--rw-r--r--   0        0        0     1933 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/run_query_request_filters.py
--rw-r--r--   0        0        0     1661 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/scheduled_jobs.py
--rw-r--r--   0        0        0     4958 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/scheduler_base.py
--rw-r--r--   0        0        0     2484 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/scheduler_csv_options.py
--rw-r--r--   0        0        0      170 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/scheduler_csv_options_limit_type_1.py
--rw-r--r--   0        0        0     2685 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/scheduler_email_target.py
--rw-r--r--   0        0        0      156 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/scheduler_format.py
--rw-r--r--   0        0        0     1272 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/scheduler_image_options.py
--rw-r--r--   0        0        0      223 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/scheduler_job_status.py
--rw-r--r--   0        0        0     5049 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/scheduler_log.py
--rw-r--r--   0        0        0      167 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/scheduler_log_target_type.py
--rw-r--r--   0        0        0      443 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/scheduler_log_task.py
--rw-r--r--   0        0        0     2665 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/scheduler_slack_target.py
--rw-r--r--   0        0        0     3505 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/share_url.py
--rw-r--r--   0        0        0     1553 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/slack_channel.py
--rw-r--r--   0        0        0     1658 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/sort_field.py
--rw-r--r--   0        0        0     2115 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/space_share.py
--rw-r--r--   0        0        0     2480 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/space_summary.py
--rw-r--r--   0        0        0     2119 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/table_calculation.py
--rw-r--r--   0        0        0     2350 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/update_pinned_item_order.py
--rw-r--r--   0        0        0     1582 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/update_project_member.py
--rw-r--r--   0        0        0     1173 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/updated_by_user.py
--rw-r--r--   0        0        0     1993 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/user_allowed_organization.py
--rw-r--r--   0        0        0     1964 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/validate_project_json_body.py
--rw-r--r--   0        0        0     6492 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/validation_error_chart_response.py
--rw-r--r--   0        0        0     5966 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/validation_error_dashboard_response.py
--rw-r--r--   0        0        0      260 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/validation_error_type.py
--rw-r--r--   0        0        0     3709 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/validation_response_base.py
--rw-r--r--   0        0        0      193 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/validation_source_type.py
--rw-r--r--   0        0        0     2633 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/view_statistics.py
--rw-r--r--   0        0        0       26 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/py.typed
--rw-r--r--   0        0        0     1101 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/types.py
--rw-r--r--   0        0        0     1624 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/pyproject.toml
--rw-r--r--   0        0        0      830 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/setup.py
--rw-r--r--   0        0        0      796 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/tests/__init__.py
--rw-r--r--   0        0        0      908 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/tests/test_dummy.py
--rw-r--r--   0        0        0     5168 1970-01-01 00:00:00.000000 lightdash_client_python-0.613.2/PKG-INFO
+-rw-r--r--   0        0        0      804 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/.github/CODEOWNERS
+-rw-r--r--   0        0        0      402 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/.github/workflows/contributors-list.yml
+-rw-r--r--   0        0        0     1849 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/.github/workflows/publish.yml
+-rw-r--r--   0        0        0     2335 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/.github/workflows/test-publish.yml
+-rw-r--r--   0        0        0     1115 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/.github/workflows/test.yml
+-rw-r--r--   0        0        0     3078 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/.gitignore
+-rw-r--r--   0        0        0     1040 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/.openapi-generator-ignore
+-rw-r--r--   0        0        0     6821 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/.openapi-generator/FILES
+-rw-r--r--   0        0        0        6 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/.openapi-generator/VERSION
+-rw-r--r--   0        0        0     1375 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    14088 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/.pylintrc
+-rw-r--r--   0        0        0      150 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/.pypirc
+-rw-r--r--   0        0        0        8 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/.python-version
+-rw-r--r--   0        0        0       32 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/.style.yapf
+-rw-r--r--   0        0        0    11357 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/LICENSE
+-rw-r--r--   0        0        0      717 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/Makefile
+-rw-r--r--   0        0        0     3258 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/README.md
+-rwxr-xr-x   0        0        0     1121 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/dev/clean.sh
+-rw-r--r--   0        0        0     2115 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/dev/generate_clients.sh
+-rw-r--r--   0        0        0      974 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/dev/lint.sh
+-rw-r--r--   0        0        0      211 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/dev/openapi-python-client.yml
+-rwxr-xr-x   0        0        0     1391 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/dev/publish.sh
+-rw-r--r--   0        0        0      152 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/dev/schemas/README.md
+-rw-r--r--   0        0        0     1299 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/dev/schemas/download.sh
+-rw-r--r--   0        0        0   233800 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/dev/schemas/swagger.json
+-rwxr-xr-x   0        0        0     1023 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/dev/setup.sh
+-rwxr-xr-x   0        0        0      958 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/dev/test_python.sh
+-rw-r--r--   0        0        0      201 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/__init__.py
+-rw-r--r--   0        0        0       47 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/api/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/api/charts/__init__.py
+-rw-r--r--   0        0        0     4680 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/api/charts/post_chart_results.py
+-rw-r--r--   0        0        0        0 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/api/content/__init__.py
+-rw-r--r--   0        0        0     4483 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/api/content/get_pinned_items.py
+-rw-r--r--   0        0        0     5511 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/api/content/update_pinned_items_order.py
+-rw-r--r--   0        0        0        0 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/api/exploring/__init__.py
+-rw-r--r--   0        0        0     5017 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/api/exploring/post_run_query.py
+-rw-r--r--   0        0        0     5095 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/api/exploring/post_run_underlying_data_query.py
+-rw-r--r--   0        0        0        0 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/api/exports/__init__.py
+-rw-r--r--   0        0        0     3848 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/api/exports/get_csv_url.py
+-rw-r--r--   0        0        0        0 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/api/integrations/__init__.py
+-rw-r--r--   0        0        0     4403 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/api/integrations/delete_dbt_cloud_integration_settings.py
+-rw-r--r--   0        0        0     2743 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/api/integrations/get_dbt_cloud_integration_settings.py
+-rw-r--r--   0        0        0     4847 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/api/integrations/get_dbt_cloud_metrics.py
+-rw-r--r--   0        0        0     3651 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/api/integrations/get_slack_channels.py
+-rw-r--r--   0        0        0     2734 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/api/integrations/update_dbt_cloud_integration_settings.py
+-rw-r--r--   0        0        0        0 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/api/my_account/__init__.py
+-rw-r--r--   0        0        0     2573 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/api/my_account/create_email_one_time_passcode.py
+-rw-r--r--   0        0        0     3501 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/api/my_account/delete_me.py
+-rw-r--r--   0        0        0     3021 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/api/my_account/get_email_verification_status.py
+-rw-r--r--   0        0        0     4793 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/api/my_account/join_organization.py
+-rw-r--r--   0        0        0     4349 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/api/my_account/list_my_available_organizations.py
+-rw-r--r--   0        0        0        0 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/api/organizations/__init__.py
+-rw-r--r--   0        0        0     4634 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/api/organizations/create_group_in_organization.py
+-rw-r--r--   0        0        0     4256 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/api/organizations/delete_my_organization.py
+-rw-r--r--   0        0        0     4057 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/api/organizations/delete_organization_member.py
+-rw-r--r--   0        0        0     3589 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/api/organizations/get_my_organization.py
+-rw-r--r--   0        0        0     3739 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/api/organizations/list_groups_in_organization.py
+-rw-r--r--   0        0        0     3983 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/api/organizations/list_organization_email_domains.py
+-rw-r--r--   0        0        0     3859 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/api/organizations/list_organization_members.py
+-rw-r--r--   0        0        0     3771 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/api/organizations/list_organization_projects.py
+-rw-r--r--   0        0        0        0 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/api/projects/__init__.py
+-rw-r--r--   0        0        0     5756 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/api/projects/get_latest_validation_results.py
+-rw-r--r--   0        0        0     2639 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/api/projects/get_project.py
+-rw-r--r--   0        0        0     4187 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/api/projects/list_charts_in_project.py
+-rw-r--r--   0        0        0     4187 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/api/projects/list_spaces_in_project.py
+-rw-r--r--   0        0        0     6428 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/api/projects/validate_project.py
+-rw-r--r--   0        0        0        0 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/api/roles_permissions/__init__.py
+-rw-r--r--   0        0        0     2984 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/api/roles_permissions/create_space_in_project.py
+-rw-r--r--   0        0        0     4928 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/api/roles_permissions/get_project_access_list.py
+-rw-r--r--   0        0        0     4648 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/api/roles_permissions/grant_project_access_to_user.py
+-rw-r--r--   0        0        0     4425 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/api/roles_permissions/revoke_project_access_for_user.py
+-rw-r--r--   0        0        0     4794 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/api/roles_permissions/revoke_space_access_for_user.py
+-rw-r--r--   0        0        0     5026 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/api/roles_permissions/update_project_access_for_user.py
+-rw-r--r--   0        0        0        0 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/api/schedulers/__init__.py
+-rw-r--r--   0        0        0     4176 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/api/schedulers/delete_scheduler.py
+-rw-r--r--   0        0        0     4147 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/api/schedulers/get_scheduled_jobs.py
+-rw-r--r--   0        0        0     2633 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/api/schedulers/get_scheduler.py
+-rw-r--r--   0        0        0     4201 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/api/schedulers/get_scheduler_job_status.py
+-rw-r--r--   0        0        0     2620 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/api/schedulers/get_scheduler_logs.py
+-rw-r--r--   0        0        0     2919 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/api/schedulers/update_scheduler.py
+-rw-r--r--   0        0        0        0 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/api/share_links/__init__.py
+-rw-r--r--   0        0        0     3960 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/api/share_links/get_share_url.py
+-rw-r--r--   0        0        0        0 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/api/spaces/__init__.py
+-rw-r--r--   0        0        0     4429 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/api/spaces/delete_space.py
+-rw-r--r--   0        0        0     2881 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/api/spaces/get_space.py
+-rw-r--r--   0        0        0        0 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/api/ssh_keypairs/__init__.py
+-rw-r--r--   0        0        0     3542 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/api/ssh_keypairs/create_ssh_key_pair.py
+-rw-r--r--   0        0        0        0 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/api/user_groups/__init__.py
+-rw-r--r--   0        0        0     4365 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/api/user_groups/add_user_to_group.py
+-rw-r--r--   0        0        0     3927 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/api/user_groups/delete_group.py
+-rw-r--r--   0        0        0     3949 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/api/user_groups/get_group.py
+-rw-r--r--   0        0        0     4073 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/api/user_groups/get_group_members.py
+-rw-r--r--   0        0        0     4348 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/api/user_groups/remove_user_from_group.py
+-rw-r--r--   0        0        0     2906 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/client.py
+-rw-r--r--   0        0        0      470 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/errors.py
+-rw-r--r--   0        0        0    20640 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/__init__.py
+-rw-r--r--   0        0        0     4166 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/additional_metric.py
+-rw-r--r--   0        0        0     2422 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/allowed_email_domains.py
+-rw-r--r--   0        0        0     2410 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/api_chart_summary_list_response.py
+-rw-r--r--   0        0        0      152 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/api_chart_summary_list_response_status.py
+-rw-r--r--   0        0        0     2106 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/api_csv_url_response.py
+-rw-r--r--   0        0        0     1652 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/api_csv_url_response_results.py
+-rw-r--r--   0        0        0      142 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/api_csv_url_response_status.py
+-rw-r--r--   0        0        0     2254 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/api_dbt_cloud_metrics.py
+-rw-r--r--   0        0        0      143 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/api_dbt_cloud_metrics_status.py
+-rw-r--r--   0        0        0     2119 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/api_dbt_cloud_settings_delete_success.py
+-rw-r--r--   0        0        0      157 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/api_dbt_cloud_settings_delete_success_status.py
+-rw-r--r--   0        0        0      147 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/api_email_status_response_status.py
+-rw-r--r--   0        0        0     2139 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/api_error_payload.py
+-rw-r--r--   0        0        0     2386 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/api_error_payload_error.py
+-rw-r--r--   0        0        0      146 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/api_error_payload_status.py
+-rw-r--r--   0        0        0     2285 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/api_group_list_response.py
+-rw-r--r--   0        0        0      145 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/api_group_list_response_status.py
+-rw-r--r--   0        0        0     2359 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/api_group_members_response.py
+-rw-r--r--   0        0        0      148 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/api_group_members_response_status.py
+-rw-r--r--   0        0        0     1951 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/api_group_response.py
+-rw-r--r--   0        0        0      141 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/api_group_response_status.py
+-rw-r--r--   0        0        0     2208 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/api_job_scheduled_response.py
+-rw-r--r--   0        0        0     1548 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/api_job_scheduled_response_results.py
+-rw-r--r--   0        0        0      148 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/api_job_scheduled_response_status.py
+-rw-r--r--   0        0        0     2157 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/api_job_status_response.py
+-rw-r--r--   0        0        0     1535 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/api_job_status_response_results.py
+-rw-r--r--   0        0        0      145 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/api_job_status_response_status.py
+-rw-r--r--   0        0        0     2019 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/api_organization.py
+-rw-r--r--   0        0        0     2241 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/api_organization_allowed_email_domains.py
+-rw-r--r--   0        0        0      159 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/api_organization_allowed_email_domains_status.py
+-rw-r--r--   0        0        0     2270 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/api_organization_member_profile.py
+-rw-r--r--   0        0        0      153 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/api_organization_member_profile_status.py
+-rw-r--r--   0        0        0     2519 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/api_organization_member_profiles.py
+-rw-r--r--   0        0        0      154 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/api_organization_member_profiles_status.py
+-rw-r--r--   0        0        0     2456 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/api_organization_projects.py
+-rw-r--r--   0        0        0      148 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/api_organization_projects_status.py
+-rw-r--r--   0        0        0      140 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/api_organization_status.py
+-rw-r--r--   0        0        0     4825 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/api_pinned_items.py
+-rw-r--r--   0        0        0      139 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/api_pinned_items_status.py
+-rw-r--r--   0        0        0     2478 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/api_project_access_list_response.py
+-rw-r--r--   0        0        0      153 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/api_project_access_list_response_status.py
+-rw-r--r--   0        0        0      143 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/api_project_response_status.py
+-rw-r--r--   0        0        0     2140 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/api_run_query_response.py
+-rw-r--r--   0        0        0     2051 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/api_run_query_response_results.py
+-rw-r--r--   0        0        0      144 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/api_run_query_response_status.py
+-rw-r--r--   0        0        0     2383 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/api_scheduled_jobs_response.py
+-rw-r--r--   0        0        0      149 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/api_scheduled_jobs_response_status.py
+-rw-r--r--   0        0        0      155 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/api_scheduler_and_targets_response_status.py
+-rw-r--r--   0        0        0      149 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/api_scheduler_logs_response_status.py
+-rw-r--r--   0        0        0     2129 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/api_share_response.py
+-rw-r--r--   0        0        0      141 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/api_share_response_status.py
+-rw-r--r--   0        0        0     2376 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/api_slack_channels_response.py
+-rw-r--r--   0        0        0      149 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/api_slack_channels_response_status.py
+-rw-r--r--   0        0        0      141 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/api_space_response_status.py
+-rw-r--r--   0        0        0     2410 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/api_space_summary_list_response.py
+-rw-r--r--   0        0        0      152 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/api_space_summary_list_response_status.py
+-rw-r--r--   0        0        0     2208 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/api_ssh_key_pair_response.py
+-rw-r--r--   0        0        0      146 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/api_ssh_key_pair_response_status.py
+-rw-r--r--   0        0        0     1937 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/api_success_empty.py
+-rw-r--r--   0        0        0      140 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/api_success_empty_status.py
+-rw-r--r--   0        0        0     2569 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/api_user_allowed_organizations_response.py
+-rw-r--r--   0        0        0      160 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/api_user_allowed_organizations_response_status.py
+-rw-r--r--   0        0        0     4732 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/api_validate_response.py
+-rw-r--r--   0        0        0      144 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/api_validate_response_status.py
+-rw-r--r--   0        0        0     1737 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/api_validation_dismiss_response.py
+-rw-r--r--   0        0        0      153 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/api_validation_dismiss_response_status.py
+-rw-r--r--   0        0        0      316 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/chart_kind.py
+-rw-r--r--   0        0        0     3776 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/chart_summary.py
+-rw-r--r--   0        0        0      192 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/chart_type.py
+-rw-r--r--   0        0        0      220 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/compact.py
+-rw-r--r--   0        0        0      272 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/compact_or_alias_type_1.py
+-rw-r--r--   0        0        0     1937 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/create_project_member.py
+-rw-r--r--   0        0        0     2646 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/create_space.py
+-rw-r--r--   0        0        0     3745 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/dbt_azure_dev_ops_project_config.py
+-rw-r--r--   0        0        0     3814 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/dbt_bit_bucket_project_config.py
+-rw-r--r--   0        0        0     2425 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/dbt_cloud_ide_project_config.py
+-rw-r--r--   0        0        0     2229 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/dbt_cloud_metadata_response_metrics.py
+-rw-r--r--   0        0        0     2494 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/dbt_cloud_metric.py
+-rw-r--r--   0        0        0     3603 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/dbt_github_project_config.py
+-rw-r--r--   0        0        0     3603 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/dbt_gitlab_project_config.py
+-rw-r--r--   0        0        0     2957 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/dbt_local_project_config.py
+-rw-r--r--   0        0        0     2733 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/dbt_none_project_config.py
+-rw-r--r--   0        0        0     1664 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/dbt_project_environment_variable.py
+-rw-r--r--   0        0        0      295 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/dbt_project_type.py
+-rw-r--r--   0        0        0      164 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/dbt_project_type_azuredevops.py
+-rw-r--r--   0        0        0      156 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/dbt_project_type_bitbucket.py
+-rw-r--r--   0        0        0      138 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/dbt_project_type_dbt.py
+-rw-r--r--   0        0        0      166 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/dbt_project_type_dbtcloudide.py
+-rw-r--r--   0        0        0      147 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/dbt_project_type_github.py
+-rw-r--r--   0        0        0      147 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/dbt_project_type_gitlab.py
+-rw-r--r--   0        0        0      141 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/dbt_project_type_none.py
+-rw-r--r--   0        0        0     2051 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/delete_scheduler_response_201.py
+-rw-r--r--   0        0        0      151 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/delete_scheduler_response_201_status.py
+-rw-r--r--   0        0        0     2003 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/email_one_time_password.py
+-rw-r--r--   0        0        0     2749 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/email_one_time_password_expiring.py
+-rw-r--r--   0        0        0     2458 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/email_status.py
+-rw-r--r--   0        0        0     1664 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/filter_group_response_type_0.py
+-rw-r--r--   0        0        0     1674 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/filter_group_response_type_1.py
+-rw-r--r--   0        0        0     4615 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/filters.py
+-rw-r--r--   0        0        0     2247 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/group.py
+-rw-r--r--   0        0        0     2163 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/group_member.py
+-rw-r--r--   0        0        0     4963 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/metric_query_response.py
+-rw-r--r--   0        0        0      383 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/metric_type.py
+-rw-r--r--   0        0        0     2812 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/organization.py
+-rw-r--r--   0        0        0     3539 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/organization_member_profile.py
+-rw-r--r--   0        0        0      287 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/organization_member_role.py
+-rw-r--r--   0        0        0     1991 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/organization_project.py
+-rw-r--r--   0        0        0     2377 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/partial_omit_organization_organization_uuid_or_needs_project.py
+-rw-r--r--   0        0        0     2120 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/partial_pick_organization_member_profile_role.py
+-rw-r--r--   0        0        0     2628 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/partial_pick_space_is_private_or_access.py
+-rw-r--r--   0        0        0     2493 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/pick_allowed_email_domains_exclude_keyof_allowed_email_domains_organization_uuid.py
+-rw-r--r--   0        0        0     6235 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/pick_create_bigquery_credentials_exclude_keyof_create_bigquery_credentials_sensitive_credentials_field_names.py
+-rw-r--r--   0        0        0      267 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/pick_create_bigquery_credentials_exclude_keyof_create_bigquery_credentials_sensitive_credentials_field_names_priority.py
+-rw-r--r--   0        0        0     3905 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/pick_create_databricks_credentials_exclude_keyof_create_databricks_credentials_sensitive_credentials_field_names.py
+-rw-r--r--   0        0        0     1841 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/pick_create_dbt_cloud_integration_metrics_job_id.py
+-rw-r--r--   0        0        0     1565 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/pick_create_group_name.py
+-rw-r--r--   0        0        0     6859 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/pick_create_postgres_credentials_exclude_keyof_create_postgres_credentials_sensitive_credentials_field_names.py
+-rw-r--r--   0        0        0     6610 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/pick_create_redshift_credentials_exclude_keyof_create_redshift_credentials_sensitive_credentials_field_names.py
+-rw-r--r--   0        0        0     5207 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/pick_create_snowflake_credentials_exclude_keyof_create_snowflake_credentials_sensitive_credentials_field_names.py
+-rw-r--r--   0        0        0     3761 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/pick_create_trino_credentials_exclude_keyof_create_trino_credentials_sensitive_credentials_field_names.py
+-rw-r--r--   0        0        0     6625 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/pick_dashboard_uuid_or_name_or_description_or_updated_at_or_project_uuid_or_updated_by_user_or_organization_uuid_or_space_uuid_or_views_or_first_viewed_at_or_pinned_list_uuid_or_pinned_list_order.py
+-rw-r--r--   0        0        0     1532 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/pick_group_name.py
+-rw-r--r--   0        0        0     1566 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/pick_organization_name.py
+-rw-r--r--   0        0        0     2016 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/pick_resource_view_item_at_data_uuid_or_pinned_list_order.py
+-rw-r--r--   0        0        0     3781 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/pick_saved_chart_uuid_or_name_or_description_or_space_name_or_space_uuid_or_project_uuid_or_organization_uuid_or_pinned_list_uuid.py
+-rw-r--r--   0        0        0     4585 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/pick_saved_chart_uuid_or_name_or_updated_at_or_updated_by_user_or_description_or_space_uuid_or_pinned_list_uuid_or_pinned_list_order.py
+-rw-r--r--   0        0        0     1757 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/pick_share_url_path_or_params.py
+-rw-r--r--   0        0        0     1502 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/pick_space_name.py
+-rw-r--r--   0        0        0     1768 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/pick_space_name_or_is_private.py
+-rw-r--r--   0        0        0     2609 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/pick_space_organization_uuid_or_project_uuid_or_uuid_or_name_or_is_private.py
+-rw-r--r--   0        0        0     3420 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/pick_space_project_uuid_or_uuid_or_name_or_is_private_or_pinned_list_uuid_or_pinned_list_order_or_organization_uuid.py
+-rw-r--r--   0        0        0     1601 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/pick_space_share_user_uuid.py
+-rw-r--r--   0        0        0     1619 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/pick_ssh_key_pair_public_key.py
+-rw-r--r--   0        0        0     3860 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/pick_validation_response_base_exclude_keyof_validation_response_base_name.py
+-rw-r--r--   0        0        0     2266 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/pick_validation_response_error_or_created_at_or_validation_id.py
+-rw-r--r--   0        0        0     2095 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/post_chart_results_json_body.py
+-rw-r--r--   0        0        0     2540 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/project_member_profile.py
+-rw-r--r--   0        0        0      260 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/project_member_role.py
+-rw-r--r--   0        0        0      164 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/project_type.py
+-rw-r--r--   0        0        0     1294 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/record_string_any.py
+-rw-r--r--   0        0        0      193 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/resource_view_item_type.py
+-rw-r--r--   0        0        0      150 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/resource_view_item_type_chart.py
+-rw-r--r--   0        0        0      162 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/resource_view_item_type_dashboard.py
+-rw-r--r--   0        0        0      150 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/resource_view_item_type_space.py
+-rw-r--r--   0        0        0     2093 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/resource_view_space_item.py
+-rw-r--r--   0        0        0     3903 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/resource_view_space_item_data.py
+-rw-r--r--   0        0        0     5334 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/run_query_request.py
+-rw-r--r--   0        0        0     1933 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/run_query_request_filters.py
+-rw-r--r--   0        0        0     1661 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/scheduled_jobs.py
+-rw-r--r--   0        0        0     4958 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/scheduler_base.py
+-rw-r--r--   0        0        0     2484 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/scheduler_csv_options.py
+-rw-r--r--   0        0        0      170 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/scheduler_csv_options_limit_type_1.py
+-rw-r--r--   0        0        0     2685 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/scheduler_email_target.py
+-rw-r--r--   0        0        0      156 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/scheduler_format.py
+-rw-r--r--   0        0        0     1272 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/scheduler_image_options.py
+-rw-r--r--   0        0        0      223 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/scheduler_job_status.py
+-rw-r--r--   0        0        0     5049 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/scheduler_log.py
+-rw-r--r--   0        0        0      167 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/scheduler_log_target_type.py
+-rw-r--r--   0        0        0      443 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/scheduler_log_task.py
+-rw-r--r--   0        0        0     2665 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/scheduler_slack_target.py
+-rw-r--r--   0        0        0     3505 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/share_url.py
+-rw-r--r--   0        0        0     1553 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/slack_channel.py
+-rw-r--r--   0        0        0     1658 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/sort_field.py
+-rw-r--r--   0        0        0     2115 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/space_share.py
+-rw-r--r--   0        0        0     2480 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/space_summary.py
+-rw-r--r--   0        0        0     2119 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/table_calculation.py
+-rw-r--r--   0        0        0     2350 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/update_pinned_item_order.py
+-rw-r--r--   0        0        0     1582 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/update_project_member.py
+-rw-r--r--   0        0        0     1173 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/updated_by_user.py
+-rw-r--r--   0        0        0     1993 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/user_allowed_organization.py
+-rw-r--r--   0        0        0     1964 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/validate_project_json_body.py
+-rw-r--r--   0        0        0     6492 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/validation_error_chart_response.py
+-rw-r--r--   0        0        0     5966 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/validation_error_dashboard_response.py
+-rw-r--r--   0        0        0      260 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/validation_error_type.py
+-rw-r--r--   0        0        0     3709 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/validation_response_base.py
+-rw-r--r--   0        0        0      193 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/validation_source_type.py
+-rw-r--r--   0        0        0     2633 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/view_statistics.py
+-rw-r--r--   0        0        0      153 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/warehouse_types_bigquery.py
+-rw-r--r--   0        0        0      159 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/warehouse_types_databricks.py
+-rw-r--r--   0        0        0      153 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/warehouse_types_postgres.py
+-rw-r--r--   0        0        0      153 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/warehouse_types_redshift.py
+-rw-r--r--   0        0        0      156 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/warehouse_types_snowflake.py
+-rw-r--r--   0        0        0      144 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/warehouse_types_trino.py
+-rw-r--r--   0        0        0      225 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/models/week_day.py
+-rw-r--r--   0        0        0       26 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/py.typed
+-rw-r--r--   0        0        0     1101 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/lightdash_client/types.py
+-rw-r--r--   0        0        0     1624 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/pyproject.toml
+-rw-r--r--   0        0        0      830 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/setup.py
+-rw-r--r--   0        0        0      796 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/tests/__init__.py
+-rw-r--r--   0        0        0      908 2023-06-19 00:37:07.000000 lightdash_client_python-0.618.0/tests/test_dummy.py
+-rw-r--r--   0        0        0     5168 1970-01-01 00:00:00.000000 lightdash_client_python-0.618.0/PKG-INFO
```

### Comparing `lightdash_client_python-0.613.2/.github/CODEOWNERS` & `lightdash_client_python-0.618.0/.github/CODEOWNERS`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.613.2/.github/workflows/publish.yml` & `lightdash_client_python-0.618.0/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.613.2/.github/workflows/test-publish.yml` & `lightdash_client_python-0.618.0/.github/workflows/test-publish.yml`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.613.2/.github/workflows/test.yml` & `lightdash_client_python-0.618.0/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.613.2/.gitignore` & `lightdash_client_python-0.618.0/.gitignore`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.613.2/.openapi-generator-ignore` & `lightdash_client_python-0.618.0/.openapi-generator-ignore`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.613.2/.openapi-generator/FILES` & `lightdash_client_python-0.618.0/.openapi-generator/FILES`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.613.2/.pre-commit-config.yaml` & `lightdash_client_python-0.618.0/.pre-commit-config.yaml`

 * *Files 15% similar despite different names*

```diff
@@ -27,7 +27,11 @@
     rev: v1.6.24
     hooks:
       - id: actionlint
   - repo: https://github.com/asottile/reorder_python_imports
     rev: v3.9.0
     hooks:
       - id: reorder-python-imports
+  - repo: https://github.com/shellcheck-py/shellcheck-py
+    rev: v0.9.0.2
+    hooks:
+      - id: shellcheck
```

### Comparing `lightdash_client_python-0.613.2/.pylintrc` & `lightdash_client_python-0.618.0/.pylintrc`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.613.2/LICENSE` & `lightdash_client_python-0.618.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.613.2/Makefile` & `lightdash_client_python-0.618.0/Makefile`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.613.2/README.md` & `lightdash_client_python-0.618.0/README.md`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.613.2/dev/clean.sh` & `lightdash_client_python-0.618.0/dev/clean.sh`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.613.2/dev/generate_clients.sh` & `lightdash_client_python-0.618.0/dev/generate_clients.sh`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.613.2/dev/lint.sh` & `lightdash_client_python-0.618.0/dev/lint.sh`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.613.2/dev/publish.sh` & `lightdash_client_python-0.618.0/dev/publish.sh`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.613.2/dev/schemas/download.sh` & `lightdash_client_python-0.618.0/dev/schemas/download.sh`

 * *Files 6% similar despite different names*

```diff
@@ -30,8 +30,9 @@
     echo "WARN: unrecognized argument ${1}" >&2
     shift 1
   fi
 done
 
 
 # Download swagger.json from the GitHub repository
-curl -O "https://raw.githubusercontent.com/lightdash/lightdash/${lightdash_version:?}/packages/backend/src/generated/swagger.json"
+url="https://raw.githubusercontent.com/lightdash/lightdash/${lightdash_version:?}/packages/backend/src/generated/swagger.json"
+curl "${url:?}" --output "${SCRIPT_DIR}/swagger.json"
```

### Comparing `lightdash_client_python-0.613.2/dev/schemas/swagger.json` & `lightdash_client_python-0.618.0/dev/schemas/swagger.json`

 * *Files 9% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9861786558595069%*

 * *Differences: {"'components'": "{'schemas': {'ProjectType': OrderedDict([('enum', ['DEFAULT', 'PREVIEW']), "*

 * *                 "('type', 'string')]), 'OrganizationProject': OrderedDict([('properties', "*

 * *                 "OrderedDict([('type', OrderedDict([('$ref', "*

 * *                 "'#/components/schemas/ProjectType')])), ('name', OrderedDict([('type', "*

 * *                 "'string')])), ('projectUuid', OrderedDict([('type', 'string'), ('description', "*

 * *                 "'The unique identifier of the project'), ('format',  […]*

```diff
@@ -445,14 +445,37 @@
                 },
                 "required": [
                     "results",
                     "status"
                 ],
                 "type": "object"
             },
+            "ApiOrganizationProjects": {
+                "description": "List of projects in the current organization",
+                "properties": {
+                    "results": {
+                        "items": {
+                            "$ref": "#/components/schemas/OrganizationProject"
+                        },
+                        "type": "array"
+                    },
+                    "status": {
+                        "enum": [
+                            "ok"
+                        ],
+                        "nullable": false,
+                        "type": "string"
+                    }
+                },
+                "required": [
+                    "results",
+                    "status"
+                ],
+                "type": "object"
+            },
             "ApiPinnedItems": {
                 "properties": {
                     "results": {
                         "$ref": "#/components/schemas/PinnedItems"
                     },
                     "status": {
                         "enum": [
@@ -486,14 +509,33 @@
                 },
                 "required": [
                     "results",
                     "status"
                 ],
                 "type": "object"
             },
+            "ApiProjectResponse": {
+                "properties": {
+                    "results": {
+                        "$ref": "#/components/schemas/Project"
+                    },
+                    "status": {
+                        "enum": [
+                            "ok"
+                        ],
+                        "nullable": false,
+                        "type": "string"
+                    }
+                },
+                "required": [
+                    "results",
+                    "status"
+                ],
+                "type": "object"
+            },
             "ApiRunQueryResponse": {
                 "properties": {
                     "results": {
                         "properties": {
                             "metricQuery": {
                                 "$ref": "#/components/schemas/MetricQueryResponse"
                             },
@@ -754,14 +796,17 @@
                     }
                 },
                 "required": [
                     "status"
                 ],
                 "type": "object"
             },
+            "BigqueryCredentials": {
+                "$ref": "#/components/schemas/Omit_CreateBigqueryCredentials.SensitiveCredentialsFieldNames_"
+            },
             "ChartKind": {
                 "enum": [
                     "line",
                     "horizontal_bar",
                     "vertical_bar",
                     "scatter",
                     "area",
@@ -925,14 +970,158 @@
                             "dashboardUuid",
                             "savedChartUuid"
                         ],
                         "type": "object"
                     }
                 ]
             },
+            "DatabricksCredentials": {
+                "$ref": "#/components/schemas/Omit_CreateDatabricksCredentials.SensitiveCredentialsFieldNames_"
+            },
+            "DbtAzureDevOpsProjectConfig": {
+                "additionalProperties": false,
+                "properties": {
+                    "branch": {
+                        "type": "string"
+                    },
+                    "environment": {
+                        "items": {
+                            "$ref": "#/components/schemas/DbtProjectEnvironmentVariable"
+                        },
+                        "type": "array"
+                    },
+                    "organization": {
+                        "type": "string"
+                    },
+                    "personal_access_token": {
+                        "type": "string"
+                    },
+                    "project": {
+                        "type": "string"
+                    },
+                    "project_sub_path": {
+                        "type": "string"
+                    },
+                    "repository": {
+                        "type": "string"
+                    },
+                    "target": {
+                        "type": "string"
+                    },
+                    "type": {
+                        "$ref": "#/components/schemas/DbtProjectType.AZURE_DEVOPS"
+                    }
+                },
+                "required": [
+                    "type",
+                    "personal_access_token",
+                    "organization",
+                    "project",
+                    "repository",
+                    "branch",
+                    "project_sub_path"
+                ],
+                "type": "object"
+            },
+            "DbtBitBucketProjectConfig": {
+                "additionalProperties": false,
+                "properties": {
+                    "branch": {
+                        "type": "string"
+                    },
+                    "environment": {
+                        "items": {
+                            "$ref": "#/components/schemas/DbtProjectEnvironmentVariable"
+                        },
+                        "type": "array"
+                    },
+                    "host_domain": {
+                        "type": "string"
+                    },
+                    "personal_access_token": {
+                        "type": "string"
+                    },
+                    "project_sub_path": {
+                        "type": "string"
+                    },
+                    "repository": {
+                        "type": "string"
+                    },
+                    "target": {
+                        "type": "string"
+                    },
+                    "type": {
+                        "$ref": "#/components/schemas/DbtProjectType.BITBUCKET"
+                    },
+                    "username": {
+                        "type": "string"
+                    }
+                },
+                "required": [
+                    "type",
+                    "username",
+                    "personal_access_token",
+                    "repository",
+                    "branch",
+                    "project_sub_path"
+                ],
+                "type": "object"
+            },
+            "DbtCloudIDEProjectConfig": {
+                "additionalProperties": false,
+                "properties": {
+                    "account_id": {
+                        "anyOf": [
+                            {
+                                "type": "string"
+                            },
+                            {
+                                "format": "double",
+                                "type": "number"
+                            }
+                        ]
+                    },
+                    "api_key": {
+                        "type": "string"
+                    },
+                    "environment_id": {
+                        "anyOf": [
+                            {
+                                "type": "string"
+                            },
+                            {
+                                "format": "double",
+                                "type": "number"
+                            }
+                        ]
+                    },
+                    "project_id": {
+                        "anyOf": [
+                            {
+                                "type": "string"
+                            },
+                            {
+                                "format": "double",
+                                "type": "number"
+                            }
+                        ]
+                    },
+                    "type": {
+                        "$ref": "#/components/schemas/DbtProjectType.DBT_CLOUD_IDE"
+                    }
+                },
+                "required": [
+                    "type",
+                    "api_key",
+                    "account_id",
+                    "environment_id",
+                    "project_id"
+                ],
+                "type": "object"
+            },
             "DbtCloudIntegration": {
                 "$ref": "#/components/schemas/Pick_CreateDbtCloudIntegration.metricsJobId_",
                 "description": "Configuration for a Lightdash integration with dbt Cloud"
             },
             "DbtCloudMetadataResponseMetrics": {
                 "description": "Response from dbt cloud metadata api containing a list of metric definitions",
                 "properties": {
@@ -982,14 +1171,239 @@
                     "description",
                     "dimensions",
                     "name",
                     "uniqueId"
                 ],
                 "type": "object"
             },
+            "DbtGithubProjectConfig": {
+                "additionalProperties": false,
+                "properties": {
+                    "branch": {
+                        "type": "string"
+                    },
+                    "environment": {
+                        "items": {
+                            "$ref": "#/components/schemas/DbtProjectEnvironmentVariable"
+                        },
+                        "type": "array"
+                    },
+                    "host_domain": {
+                        "type": "string"
+                    },
+                    "personal_access_token": {
+                        "type": "string"
+                    },
+                    "project_sub_path": {
+                        "type": "string"
+                    },
+                    "repository": {
+                        "type": "string"
+                    },
+                    "target": {
+                        "type": "string"
+                    },
+                    "type": {
+                        "$ref": "#/components/schemas/DbtProjectType.GITHUB"
+                    }
+                },
+                "required": [
+                    "type",
+                    "personal_access_token",
+                    "repository",
+                    "branch",
+                    "project_sub_path"
+                ],
+                "type": "object"
+            },
+            "DbtGitlabProjectConfig": {
+                "additionalProperties": false,
+                "properties": {
+                    "branch": {
+                        "type": "string"
+                    },
+                    "environment": {
+                        "items": {
+                            "$ref": "#/components/schemas/DbtProjectEnvironmentVariable"
+                        },
+                        "type": "array"
+                    },
+                    "host_domain": {
+                        "type": "string"
+                    },
+                    "personal_access_token": {
+                        "type": "string"
+                    },
+                    "project_sub_path": {
+                        "type": "string"
+                    },
+                    "repository": {
+                        "type": "string"
+                    },
+                    "target": {
+                        "type": "string"
+                    },
+                    "type": {
+                        "$ref": "#/components/schemas/DbtProjectType.GITLAB"
+                    }
+                },
+                "required": [
+                    "type",
+                    "personal_access_token",
+                    "repository",
+                    "branch",
+                    "project_sub_path"
+                ],
+                "type": "object"
+            },
+            "DbtLocalProjectConfig": {
+                "additionalProperties": false,
+                "properties": {
+                    "environment": {
+                        "items": {
+                            "$ref": "#/components/schemas/DbtProjectEnvironmentVariable"
+                        },
+                        "type": "array"
+                    },
+                    "profiles_dir": {
+                        "type": "string"
+                    },
+                    "project_dir": {
+                        "type": "string"
+                    },
+                    "target": {
+                        "type": "string"
+                    },
+                    "type": {
+                        "$ref": "#/components/schemas/DbtProjectType.DBT"
+                    }
+                },
+                "required": [
+                    "type"
+                ],
+                "type": "object"
+            },
+            "DbtNoneProjectConfig": {
+                "additionalProperties": false,
+                "properties": {
+                    "environment": {
+                        "items": {
+                            "$ref": "#/components/schemas/DbtProjectEnvironmentVariable"
+                        },
+                        "type": "array"
+                    },
+                    "hideRefreshButton": {
+                        "type": "boolean"
+                    },
+                    "target": {
+                        "type": "string"
+                    },
+                    "type": {
+                        "$ref": "#/components/schemas/DbtProjectType.NONE"
+                    }
+                },
+                "required": [
+                    "type"
+                ],
+                "type": "object"
+            },
+            "DbtProjectConfig": {
+                "anyOf": [
+                    {
+                        "$ref": "#/components/schemas/DbtLocalProjectConfig"
+                    },
+                    {
+                        "$ref": "#/components/schemas/DbtCloudIDEProjectConfig"
+                    },
+                    {
+                        "$ref": "#/components/schemas/DbtGithubProjectConfig"
+                    },
+                    {
+                        "$ref": "#/components/schemas/DbtBitBucketProjectConfig"
+                    },
+                    {
+                        "$ref": "#/components/schemas/DbtGitlabProjectConfig"
+                    },
+                    {
+                        "$ref": "#/components/schemas/DbtAzureDevOpsProjectConfig"
+                    },
+                    {
+                        "$ref": "#/components/schemas/DbtNoneProjectConfig"
+                    }
+                ]
+            },
+            "DbtProjectEnvironmentVariable": {
+                "properties": {
+                    "key": {
+                        "type": "string"
+                    },
+                    "value": {
+                        "type": "string"
+                    }
+                },
+                "required": [
+                    "value",
+                    "key"
+                ],
+                "type": "object"
+            },
+            "DbtProjectType": {
+                "enum": [
+                    "dbt",
+                    "dbt_cloud_ide",
+                    "github",
+                    "gitlab",
+                    "bitbucket",
+                    "azure_devops",
+                    "none"
+                ],
+                "type": "string"
+            },
+            "DbtProjectType.AZURE_DEVOPS": {
+                "enum": [
+                    "azure_devops"
+                ],
+                "type": "string"
+            },
+            "DbtProjectType.BITBUCKET": {
+                "enum": [
+                    "bitbucket"
+                ],
+                "type": "string"
+            },
+            "DbtProjectType.DBT": {
+                "enum": [
+                    "dbt"
+                ],
+                "type": "string"
+            },
+            "DbtProjectType.DBT_CLOUD_IDE": {
+                "enum": [
+                    "dbt_cloud_ide"
+                ],
+                "type": "string"
+            },
+            "DbtProjectType.GITHUB": {
+                "enum": [
+                    "github"
+                ],
+                "type": "string"
+            },
+            "DbtProjectType.GITLAB": {
+                "enum": [
+                    "gitlab"
+                ],
+                "type": "string"
+            },
+            "DbtProjectType.NONE": {
+                "enum": [
+                    "none"
+                ],
+                "type": "string"
+            },
             "EmailOneTimePassword": {
                 "properties": {
                     "createdAt": {
                         "description": "Time that the passcode was created",
                         "format": "date-time",
                         "type": "string"
                     },
@@ -1241,14 +1655,38 @@
                 ],
                 "type": "string"
             },
             "Omit_AllowedEmailDomains.organizationUuid_": {
                 "$ref": "#/components/schemas/Pick_AllowedEmailDomains.Exclude_keyofAllowedEmailDomains.organizationUuid__",
                 "description": "Construct a type with the properties of T except for those in type K."
             },
+            "Omit_CreateBigqueryCredentials.SensitiveCredentialsFieldNames_": {
+                "$ref": "#/components/schemas/Pick_CreateBigqueryCredentials.Exclude_keyofCreateBigqueryCredentials.SensitiveCredentialsFieldNames__",
+                "description": "Construct a type with the properties of T except for those in type K."
+            },
+            "Omit_CreateDatabricksCredentials.SensitiveCredentialsFieldNames_": {
+                "$ref": "#/components/schemas/Pick_CreateDatabricksCredentials.Exclude_keyofCreateDatabricksCredentials.SensitiveCredentialsFieldNames__",
+                "description": "Construct a type with the properties of T except for those in type K."
+            },
+            "Omit_CreatePostgresCredentials.SensitiveCredentialsFieldNames_": {
+                "$ref": "#/components/schemas/Pick_CreatePostgresCredentials.Exclude_keyofCreatePostgresCredentials.SensitiveCredentialsFieldNames__",
+                "description": "Construct a type with the properties of T except for those in type K."
+            },
+            "Omit_CreateRedshiftCredentials.SensitiveCredentialsFieldNames_": {
+                "$ref": "#/components/schemas/Pick_CreateRedshiftCredentials.Exclude_keyofCreateRedshiftCredentials.SensitiveCredentialsFieldNames__",
+                "description": "Construct a type with the properties of T except for those in type K."
+            },
+            "Omit_CreateSnowflakeCredentials.SensitiveCredentialsFieldNames_": {
+                "$ref": "#/components/schemas/Pick_CreateSnowflakeCredentials.Exclude_keyofCreateSnowflakeCredentials.SensitiveCredentialsFieldNames__",
+                "description": "Construct a type with the properties of T except for those in type K."
+            },
+            "Omit_CreateTrinoCredentials.SensitiveCredentialsFieldNames_": {
+                "$ref": "#/components/schemas/Pick_CreateTrinoCredentials.Exclude_keyofCreateTrinoCredentials.SensitiveCredentialsFieldNames__",
+                "description": "Construct a type with the properties of T except for those in type K."
+            },
             "Omit_ValidationResponseBase.name_": {
                 "$ref": "#/components/schemas/Pick_ValidationResponseBase.Exclude_keyofValidationResponseBase.name__",
                 "description": "Construct a type with the properties of T except for those in type K."
             },
             "Organization": {
                 "description": "Details of a user's Organization",
                 "properties": {
@@ -1334,14 +1772,36 @@
                     "interactive_viewer",
                     "editor",
                     "developer",
                     "admin"
                 ],
                 "type": "string"
             },
+            "OrganizationProject": {
+                "description": "Summary of a project under an organization",
+                "properties": {
+                    "name": {
+                        "type": "string"
+                    },
+                    "projectUuid": {
+                        "description": "The unique identifier of the project",
+                        "format": "uuid",
+                        "type": "string"
+                    },
+                    "type": {
+                        "$ref": "#/components/schemas/ProjectType"
+                    }
+                },
+                "required": [
+                    "type",
+                    "name",
+                    "projectUuid"
+                ],
+                "type": "object"
+            },
             "Partial_Omit_Organization.organizationUuid-or-needsProject__": {
                 "description": "Make all properties in T optional",
                 "properties": {
                     "chartColors": {
                         "description": "The default color palette for all projects in the organization",
                         "items": {
                             "type": "string"
@@ -1402,14 +1862,103 @@
                 "required": [
                     "role",
                     "emailDomains",
                     "projectUuids"
                 ],
                 "type": "object"
             },
+            "Pick_CreateBigqueryCredentials.Exclude_keyofCreateBigqueryCredentials.SensitiveCredentialsFieldNames__": {
+                "description": "From T, pick a set of properties whose keys are in the union K",
+                "properties": {
+                    "dataset": {
+                        "type": "string"
+                    },
+                    "location": {
+                        "type": "string"
+                    },
+                    "maximumBytesBilled": {
+                        "format": "double",
+                        "type": "number"
+                    },
+                    "priority": {
+                        "enum": [
+                            "interactive",
+                            "batch"
+                        ],
+                        "type": "string"
+                    },
+                    "project": {
+                        "type": "string"
+                    },
+                    "retries": {
+                        "format": "double",
+                        "type": "number"
+                    },
+                    "startOfWeek": {
+                        "allOf": [
+                            {
+                                "$ref": "#/components/schemas/WeekDay"
+                            }
+                        ],
+                        "nullable": true
+                    },
+                    "threads": {
+                        "format": "double",
+                        "type": "number"
+                    },
+                    "timeoutSeconds": {
+                        "format": "double",
+                        "type": "number"
+                    },
+                    "type": {
+                        "$ref": "#/components/schemas/WarehouseTypes.BIGQUERY"
+                    }
+                },
+                "required": [
+                    "type",
+                    "project",
+                    "dataset"
+                ],
+                "type": "object"
+            },
+            "Pick_CreateDatabricksCredentials.Exclude_keyofCreateDatabricksCredentials.SensitiveCredentialsFieldNames__": {
+                "description": "From T, pick a set of properties whose keys are in the union K",
+                "properties": {
+                    "catalog": {
+                        "type": "string"
+                    },
+                    "database": {
+                        "type": "string"
+                    },
+                    "httpPath": {
+                        "type": "string"
+                    },
+                    "serverHostName": {
+                        "type": "string"
+                    },
+                    "startOfWeek": {
+                        "allOf": [
+                            {
+                                "$ref": "#/components/schemas/WeekDay"
+                            }
+                        ],
+                        "nullable": true
+                    },
+                    "type": {
+                        "$ref": "#/components/schemas/WarehouseTypes.DATABRICKS"
+                    }
+                },
+                "required": [
+                    "type",
+                    "database",
+                    "serverHostName",
+                    "httpPath"
+                ],
+                "type": "object"
+            },
             "Pick_CreateDbtCloudIntegration.metricsJobId_": {
                 "description": "From T, pick a set of properties whose keys are in the union K",
                 "properties": {
                     "metricsJobId": {
                         "description": "Job id for a dbt cloud job containing a compiled dbt project with available dbt metrics",
                         "type": "string"
                     }
@@ -1428,14 +1977,244 @@
                     }
                 },
                 "required": [
                     "name"
                 ],
                 "type": "object"
             },
+            "Pick_CreatePostgresCredentials.Exclude_keyofCreatePostgresCredentials.SensitiveCredentialsFieldNames__": {
+                "description": "From T, pick a set of properties whose keys are in the union K",
+                "properties": {
+                    "dbname": {
+                        "type": "string"
+                    },
+                    "host": {
+                        "type": "string"
+                    },
+                    "keepalivesIdle": {
+                        "format": "double",
+                        "type": "number"
+                    },
+                    "port": {
+                        "format": "double",
+                        "type": "number"
+                    },
+                    "role": {
+                        "type": "string"
+                    },
+                    "schema": {
+                        "type": "string"
+                    },
+                    "searchPath": {
+                        "type": "string"
+                    },
+                    "sshTunnelHost": {
+                        "type": "string"
+                    },
+                    "sshTunnelPort": {
+                        "format": "double",
+                        "type": "number"
+                    },
+                    "sshTunnelPublicKey": {
+                        "type": "string"
+                    },
+                    "sshTunnelUser": {
+                        "type": "string"
+                    },
+                    "sslmode": {
+                        "type": "string"
+                    },
+                    "startOfWeek": {
+                        "allOf": [
+                            {
+                                "$ref": "#/components/schemas/WeekDay"
+                            }
+                        ],
+                        "nullable": true
+                    },
+                    "threads": {
+                        "format": "double",
+                        "type": "number"
+                    },
+                    "type": {
+                        "$ref": "#/components/schemas/WarehouseTypes.POSTGRES"
+                    },
+                    "useSshTunnel": {
+                        "type": "boolean"
+                    }
+                },
+                "required": [
+                    "type",
+                    "schema",
+                    "host",
+                    "port",
+                    "dbname"
+                ],
+                "type": "object"
+            },
+            "Pick_CreateRedshiftCredentials.Exclude_keyofCreateRedshiftCredentials.SensitiveCredentialsFieldNames__": {
+                "description": "From T, pick a set of properties whose keys are in the union K",
+                "properties": {
+                    "dbname": {
+                        "type": "string"
+                    },
+                    "host": {
+                        "type": "string"
+                    },
+                    "keepalivesIdle": {
+                        "format": "double",
+                        "type": "number"
+                    },
+                    "port": {
+                        "format": "double",
+                        "type": "number"
+                    },
+                    "ra3Node": {
+                        "type": "boolean"
+                    },
+                    "schema": {
+                        "type": "string"
+                    },
+                    "sshTunnelHost": {
+                        "type": "string"
+                    },
+                    "sshTunnelPort": {
+                        "format": "double",
+                        "type": "number"
+                    },
+                    "sshTunnelPublicKey": {
+                        "type": "string"
+                    },
+                    "sshTunnelUser": {
+                        "type": "string"
+                    },
+                    "sslmode": {
+                        "type": "string"
+                    },
+                    "startOfWeek": {
+                        "allOf": [
+                            {
+                                "$ref": "#/components/schemas/WeekDay"
+                            }
+                        ],
+                        "nullable": true
+                    },
+                    "threads": {
+                        "format": "double",
+                        "type": "number"
+                    },
+                    "type": {
+                        "$ref": "#/components/schemas/WarehouseTypes.REDSHIFT"
+                    },
+                    "useSshTunnel": {
+                        "type": "boolean"
+                    }
+                },
+                "required": [
+                    "type",
+                    "schema",
+                    "host",
+                    "port",
+                    "dbname"
+                ],
+                "type": "object"
+            },
+            "Pick_CreateSnowflakeCredentials.Exclude_keyofCreateSnowflakeCredentials.SensitiveCredentialsFieldNames__": {
+                "description": "From T, pick a set of properties whose keys are in the union K",
+                "properties": {
+                    "accessUrl": {
+                        "type": "string"
+                    },
+                    "account": {
+                        "type": "string"
+                    },
+                    "clientSessionKeepAlive": {
+                        "type": "boolean"
+                    },
+                    "database": {
+                        "type": "string"
+                    },
+                    "queryTag": {
+                        "type": "string"
+                    },
+                    "role": {
+                        "type": "string"
+                    },
+                    "schema": {
+                        "type": "string"
+                    },
+                    "startOfWeek": {
+                        "allOf": [
+                            {
+                                "$ref": "#/components/schemas/WeekDay"
+                            }
+                        ],
+                        "nullable": true
+                    },
+                    "threads": {
+                        "format": "double",
+                        "type": "number"
+                    },
+                    "type": {
+                        "$ref": "#/components/schemas/WarehouseTypes.SNOWFLAKE"
+                    },
+                    "warehouse": {
+                        "type": "string"
+                    }
+                },
+                "required": [
+                    "type",
+                    "account",
+                    "database",
+                    "warehouse",
+                    "schema"
+                ],
+                "type": "object"
+            },
+            "Pick_CreateTrinoCredentials.Exclude_keyofCreateTrinoCredentials.SensitiveCredentialsFieldNames__": {
+                "description": "From T, pick a set of properties whose keys are in the union K",
+                "properties": {
+                    "dbname": {
+                        "type": "string"
+                    },
+                    "host": {
+                        "type": "string"
+                    },
+                    "http_scheme": {
+                        "type": "string"
+                    },
+                    "port": {
+                        "format": "double",
+                        "type": "number"
+                    },
+                    "schema": {
+                        "type": "string"
+                    },
+                    "startOfWeek": {
+                        "allOf": [
+                            {
+                                "$ref": "#/components/schemas/WeekDay"
+                            }
+                        ],
+                        "nullable": true
+                    },
+                    "type": {
+                        "$ref": "#/components/schemas/WarehouseTypes.TRINO"
+                    }
+                },
+                "required": [
+                    "type",
+                    "schema",
+                    "host",
+                    "port",
+                    "dbname",
+                    "http_scheme"
+                ],
+                "type": "object"
+            },
             "Pick_Dashboard.uuid-or-name-or-description-or-updatedAt-or-projectUuid-or-updatedByUser-or-organizationUuid-or-spaceUuid-or-views-or-firstViewedAt-or-pinnedListUuid-or-pinnedListOrder_": {
                 "description": "From T, pick a set of properties whose keys are in the union K",
                 "properties": {
                     "description": {
                         "type": "string"
                     },
                     "firstViewedAt": {
@@ -1967,14 +2746,53 @@
                         {
                             "$ref": "#/components/schemas/ResourceViewSpaceItem"
                         }
                     ]
                 },
                 "type": "array"
             },
+            "PostgresCredentials": {
+                "$ref": "#/components/schemas/Omit_CreatePostgresCredentials.SensitiveCredentialsFieldNames_"
+            },
+            "Project": {
+                "properties": {
+                    "copiedFromProjectUuid": {
+                        "type": "string"
+                    },
+                    "dbtConnection": {
+                        "$ref": "#/components/schemas/DbtProjectConfig"
+                    },
+                    "name": {
+                        "type": "string"
+                    },
+                    "organizationUuid": {
+                        "type": "string"
+                    },
+                    "pinnedListUuid": {
+                        "type": "string"
+                    },
+                    "projectUuid": {
+                        "type": "string"
+                    },
+                    "type": {
+                        "$ref": "#/components/schemas/ProjectType"
+                    },
+                    "warehouseConnection": {
+                        "$ref": "#/components/schemas/WarehouseCredentials"
+                    }
+                },
+                "required": [
+                    "dbtConnection",
+                    "type",
+                    "name",
+                    "projectUuid",
+                    "organizationUuid"
+                ],
+                "type": "object"
+            },
             "ProjectMemberProfile": {
                 "properties": {
                     "email": {
                         "type": "string"
                     },
                     "firstName": {
                         "type": "string"
@@ -2008,19 +2826,29 @@
                     "interactive_viewer",
                     "editor",
                     "developer",
                     "admin"
                 ],
                 "type": "string"
             },
+            "ProjectType": {
+                "enum": [
+                    "DEFAULT",
+                    "PREVIEW"
+                ],
+                "type": "string"
+            },
             "Record_string.any_": {
                 "description": "Construct a type with a set of properties K of type T",
                 "properties": {},
                 "type": "object"
             },
+            "RedshiftCredentials": {
+                "$ref": "#/components/schemas/Omit_CreateRedshiftCredentials.SensitiveCredentialsFieldNames_"
+            },
             "ResourceViewChartItem": {
                 "properties": {
                     "data": {
                         "$ref": "#/components/schemas/Pick_SpaceQuery.uuid-or-name-or-chartType-or-firstViewedAt-or-views-or-pinnedListUuid-or-pinnedListOrder-or-spaceUuid-or-description-or-updatedAt-or-updatedByUser-or-validationErrors_"
                     },
                     "type": {
                         "$ref": "#/components/schemas/ResourceViewItemType.CHART"
@@ -2588,14 +3416,17 @@
                 },
                 "required": [
                     "name",
                     "id"
                 ],
                 "type": "object"
             },
+            "SnowflakeCredentials": {
+                "$ref": "#/components/schemas/Omit_CreateSnowflakeCredentials.SensitiveCredentialsFieldNames_"
+            },
             "SortField": {
                 "properties": {
                     "descending": {
                         "type": "boolean"
                     },
                     "fieldId": {
                         "type": "string"
@@ -2756,14 +3587,17 @@
                 "required": [
                     "sql",
                     "displayName",
                     "name"
                 ],
                 "type": "object"
             },
+            "TrinoCredentials": {
+                "$ref": "#/components/schemas/Omit_CreateTrinoCredentials.SensitiveCredentialsFieldNames_"
+            },
             "UpdateAllowedEmailDomains": {
                 "$ref": "#/components/schemas/Omit_AllowedEmailDomains.organizationUuid_"
             },
             "UpdateGroup": {
                 "$ref": "#/components/schemas/Pick_Group.name_"
             },
             "UpdateOrganization": {
@@ -3020,14 +3854,84 @@
                     }
                 },
                 "required": [
                     "firstViewedAt",
                     "views"
                 ],
                 "type": "object"
+            },
+            "WarehouseCredentials": {
+                "anyOf": [
+                    {
+                        "$ref": "#/components/schemas/SnowflakeCredentials"
+                    },
+                    {
+                        "$ref": "#/components/schemas/RedshiftCredentials"
+                    },
+                    {
+                        "$ref": "#/components/schemas/PostgresCredentials"
+                    },
+                    {
+                        "$ref": "#/components/schemas/BigqueryCredentials"
+                    },
+                    {
+                        "$ref": "#/components/schemas/DatabricksCredentials"
+                    },
+                    {
+                        "$ref": "#/components/schemas/TrinoCredentials"
+                    }
+                ]
+            },
+            "WarehouseTypes.BIGQUERY": {
+                "enum": [
+                    "bigquery"
+                ],
+                "type": "string"
+            },
+            "WarehouseTypes.DATABRICKS": {
+                "enum": [
+                    "databricks"
+                ],
+                "type": "string"
+            },
+            "WarehouseTypes.POSTGRES": {
+                "enum": [
+                    "postgres"
+                ],
+                "type": "string"
+            },
+            "WarehouseTypes.REDSHIFT": {
+                "enum": [
+                    "redshift"
+                ],
+                "type": "string"
+            },
+            "WarehouseTypes.SNOWFLAKE": {
+                "enum": [
+                    "snowflake"
+                ],
+                "type": "string"
+            },
+            "WarehouseTypes.TRINO": {
+                "enum": [
+                    "trino"
+                ],
+                "type": "string"
+            },
+            "WeekDay": {
+                "enum": [
+                    0,
+                    1,
+                    2,
+                    3,
+                    4,
+                    5,
+                    6
+                ],
+                "type": "number"
             }
         },
         "securitySchemes": {
             "api_key": {
                 "description": "Value should be 'ApiKey <your key>'",
                 "in": "header",
                 "name": "Authorization",
@@ -3047,15 +3951,15 @@
             "url": "https://docs.lightdash.com/help-and-contact/contact/contact_info/"
         },
         "description": "Open API documentation for all public Lightdash API endpoints",
         "license": {
             "name": "MIT"
         },
         "title": "Lightdash API",
-        "version": "0.613.1"
+        "version": "0.616.2"
     },
     "openapi": "3.0.0",
     "paths": {
         "/api/v1/csv/{jobId}": {
             "get": {
                 "description": "Get a Csv",
                 "operationId": "getCsvUrl",
@@ -3639,14 +4543,47 @@
                 },
                 "security": [],
                 "tags": [
                     "Organizations"
                 ]
             }
         },
+        "/api/v1/org/projects": {
+            "get": {
+                "description": "Gets all projects of the current user's organization",
+                "operationId": "ListOrganizationProjects",
+                "parameters": [],
+                "responses": {
+                    "200": {
+                        "content": {
+                            "application/json": {
+                                "schema": {
+                                    "$ref": "#/components/schemas/ApiOrganizationProjects"
+                                }
+                            }
+                        },
+                        "description": "Ok"
+                    },
+                    "default": {
+                        "content": {
+                            "application/json": {
+                                "schema": {
+                                    "$ref": "#/components/schemas/ApiErrorPayload"
+                                }
+                            }
+                        },
+                        "description": "Error"
+                    }
+                },
+                "security": [],
+                "tags": [
+                    "Organizations"
+                ]
+            }
+        },
         "/api/v1/org/user/{userUuid}": {
             "delete": {
                 "description": "Deletes a user from the current user's organization",
                 "operationId": "DeleteOrganizationMember",
                 "parameters": [
                     {
                         "description": "the uuid of the user to delete",
@@ -3814,14 +4751,56 @@
                 },
                 "security": [],
                 "tags": [
                     "Organizations"
                 ]
             }
         },
+        "/api/v1/projects/{projectUuid}": {
+            "get": {
+                "description": "Get a project of an organiztion",
+                "operationId": "GetProject",
+                "parameters": [
+                    {
+                        "in": "path",
+                        "name": "projectUuid",
+                        "required": true,
+                        "schema": {
+                            "type": "string"
+                        }
+                    }
+                ],
+                "responses": {
+                    "200": {
+                        "content": {
+                            "application/json": {
+                                "schema": {
+                                    "$ref": "#/components/schemas/ApiProjectResponse"
+                                }
+                            }
+                        },
+                        "description": "Success"
+                    },
+                    "default": {
+                        "content": {
+                            "application/json": {
+                                "schema": {
+                                    "$ref": "#/components/schemas/ApiErrorPayload"
+                                }
+                            }
+                        },
+                        "description": "Error"
+                    }
+                },
+                "security": [],
+                "tags": [
+                    "Projects"
+                ]
+            }
+        },
         "/api/v1/projects/{projectUuid}/access": {
             "get": {
                 "description": "Get access list for a project. This is a list of users that have been explictly granted access to the project.\nThere may be other users that have access to the project via their organization membership.",
                 "operationId": "GetProjectAccessList",
                 "parameters": [
                     {
                         "in": "path",
```

### Comparing `lightdash_client_python-0.613.2/dev/setup.sh` & `lightdash_client_python-0.618.0/dev/setup.sh`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.613.2/dev/test_python.sh` & `lightdash_client_python-0.618.0/dev/test_python.sh`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.613.2/lightdash_client/api/charts/post_chart_results.py` & `lightdash_client_python-0.618.0/lightdash_client/api/charts/post_chart_results.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.613.2/lightdash_client/api/content/get_pinned_items.py` & `lightdash_client_python-0.618.0/lightdash_client/api/content/get_pinned_items.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.613.2/lightdash_client/api/content/update_pinned_items_order.py` & `lightdash_client_python-0.618.0/lightdash_client/api/content/update_pinned_items_order.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.613.2/lightdash_client/api/exploring/post_run_query.py` & `lightdash_client_python-0.618.0/lightdash_client/api/exploring/post_run_query.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.613.2/lightdash_client/api/exploring/post_run_underlying_data_query.py` & `lightdash_client_python-0.618.0/lightdash_client/api/exploring/post_run_underlying_data_query.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.613.2/lightdash_client/api/exports/get_csv_url.py` & `lightdash_client_python-0.618.0/lightdash_client/api/exports/get_csv_url.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.613.2/lightdash_client/api/integrations/delete_dbt_cloud_integration_settings.py` & `lightdash_client_python-0.618.0/lightdash_client/api/integrations/delete_dbt_cloud_integration_settings.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.613.2/lightdash_client/api/integrations/get_dbt_cloud_integration_settings.py` & `lightdash_client_python-0.618.0/lightdash_client/api/integrations/get_dbt_cloud_integration_settings.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.613.2/lightdash_client/api/integrations/get_dbt_cloud_metrics.py` & `lightdash_client_python-0.618.0/lightdash_client/api/integrations/get_dbt_cloud_metrics.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.613.2/lightdash_client/api/integrations/get_slack_channels.py` & `lightdash_client_python-0.618.0/lightdash_client/api/integrations/get_slack_channels.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.613.2/lightdash_client/api/integrations/update_dbt_cloud_integration_settings.py` & `lightdash_client_python-0.618.0/lightdash_client/api/integrations/update_dbt_cloud_integration_settings.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.613.2/lightdash_client/api/my_account/create_email_one_time_passcode.py` & `lightdash_client_python-0.618.0/lightdash_client/api/my_account/create_email_one_time_passcode.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.613.2/lightdash_client/api/my_account/delete_me.py` & `lightdash_client_python-0.618.0/lightdash_client/api/my_account/delete_me.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.613.2/lightdash_client/api/my_account/get_email_verification_status.py` & `lightdash_client_python-0.618.0/lightdash_client/api/my_account/get_email_verification_status.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.613.2/lightdash_client/api/my_account/join_organization.py` & `lightdash_client_python-0.618.0/lightdash_client/api/my_account/join_organization.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.613.2/lightdash_client/api/my_account/list_my_available_organizations.py` & `lightdash_client_python-0.618.0/lightdash_client/api/my_account/list_my_available_organizations.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.613.2/lightdash_client/api/organizations/create_group_in_organization.py` & `lightdash_client_python-0.618.0/lightdash_client/api/organizations/create_group_in_organization.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.613.2/lightdash_client/api/organizations/delete_my_organization.py` & `lightdash_client_python-0.618.0/lightdash_client/api/organizations/delete_my_organization.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.613.2/lightdash_client/api/organizations/delete_organization_member.py` & `lightdash_client_python-0.618.0/lightdash_client/api/organizations/delete_organization_member.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.613.2/lightdash_client/api/organizations/get_my_organization.py` & `lightdash_client_python-0.618.0/lightdash_client/api/organizations/get_my_organization.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.613.2/lightdash_client/api/organizations/list_groups_in_organization.py` & `lightdash_client_python-0.618.0/lightdash_client/api/organizations/list_groups_in_organization.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.613.2/lightdash_client/api/organizations/list_organization_email_domains.py` & `lightdash_client_python-0.618.0/lightdash_client/api/organizations/list_organization_email_domains.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.613.2/lightdash_client/api/organizations/list_organization_members.py` & `lightdash_client_python-0.618.0/lightdash_client/api/organizations/list_organization_members.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.613.2/lightdash_client/api/projects/get_latest_validation_results.py` & `lightdash_client_python-0.618.0/lightdash_client/api/projects/get_latest_validation_results.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.613.2/lightdash_client/api/projects/list_charts_in_project.py` & `lightdash_client_python-0.618.0/lightdash_client/api/projects/list_charts_in_project.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.613.2/lightdash_client/api/projects/list_spaces_in_project.py` & `lightdash_client_python-0.618.0/lightdash_client/api/projects/list_spaces_in_project.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.613.2/lightdash_client/api/projects/validate_project.py` & `lightdash_client_python-0.618.0/lightdash_client/api/projects/validate_project.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.613.2/lightdash_client/api/roles_permissions/create_space_in_project.py` & `lightdash_client_python-0.618.0/lightdash_client/api/roles_permissions/create_space_in_project.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.613.2/lightdash_client/api/roles_permissions/get_project_access_list.py` & `lightdash_client_python-0.618.0/lightdash_client/api/roles_permissions/get_project_access_list.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.613.2/lightdash_client/api/roles_permissions/grant_project_access_to_user.py` & `lightdash_client_python-0.618.0/lightdash_client/api/roles_permissions/grant_project_access_to_user.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.613.2/lightdash_client/api/roles_permissions/revoke_project_access_for_user.py` & `lightdash_client_python-0.618.0/lightdash_client/api/roles_permissions/revoke_project_access_for_user.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.613.2/lightdash_client/api/roles_permissions/revoke_space_access_for_user.py` & `lightdash_client_python-0.618.0/lightdash_client/api/roles_permissions/revoke_space_access_for_user.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.613.2/lightdash_client/api/roles_permissions/update_project_access_for_user.py` & `lightdash_client_python-0.618.0/lightdash_client/api/roles_permissions/update_project_access_for_user.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.613.2/lightdash_client/api/schedulers/delete_scheduler.py` & `lightdash_client_python-0.618.0/lightdash_client/api/schedulers/delete_scheduler.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.613.2/lightdash_client/api/schedulers/get_scheduled_jobs.py` & `lightdash_client_python-0.618.0/lightdash_client/api/schedulers/get_scheduled_jobs.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.613.2/lightdash_client/api/schedulers/get_scheduler.py` & `lightdash_client_python-0.618.0/lightdash_client/api/schedulers/get_scheduler.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.613.2/lightdash_client/api/schedulers/get_scheduler_job_status.py` & `lightdash_client_python-0.618.0/lightdash_client/api/schedulers/get_scheduler_job_status.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.613.2/lightdash_client/api/schedulers/get_scheduler_logs.py` & `lightdash_client_python-0.618.0/lightdash_client/api/schedulers/get_scheduler_logs.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.613.2/lightdash_client/api/schedulers/update_scheduler.py` & `lightdash_client_python-0.618.0/lightdash_client/api/schedulers/update_scheduler.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.613.2/lightdash_client/api/share_links/get_share_url.py` & `lightdash_client_python-0.618.0/lightdash_client/api/share_links/get_share_url.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.613.2/lightdash_client/api/spaces/delete_space.py` & `lightdash_client_python-0.618.0/lightdash_client/api/spaces/delete_space.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.613.2/lightdash_client/api/spaces/get_space.py` & `lightdash_client_python-0.618.0/lightdash_client/api/spaces/get_space.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.613.2/lightdash_client/api/ssh_keypairs/create_ssh_key_pair.py` & `lightdash_client_python-0.618.0/lightdash_client/api/ssh_keypairs/create_ssh_key_pair.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.613.2/lightdash_client/api/user_groups/add_user_to_group.py` & `lightdash_client_python-0.618.0/lightdash_client/api/user_groups/add_user_to_group.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.613.2/lightdash_client/api/user_groups/delete_group.py` & `lightdash_client_python-0.618.0/lightdash_client/api/user_groups/delete_group.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.613.2/lightdash_client/api/user_groups/get_group.py` & `lightdash_client_python-0.618.0/lightdash_client/api/user_groups/get_group.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.613.2/lightdash_client/api/user_groups/get_group_members.py` & `lightdash_client_python-0.618.0/lightdash_client/api/user_groups/get_group_members.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.613.2/lightdash_client/api/user_groups/remove_user_from_group.py` & `lightdash_client_python-0.618.0/lightdash_client/api/user_groups/remove_user_from_group.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.613.2/lightdash_client/client.py` & `lightdash_client_python-0.618.0/lightdash_client/client.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.613.2/lightdash_client/models/__init__.py` & `lightdash_client_python-0.618.0/lightdash_client/models/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -29,19 +29,22 @@
 from .api_organization import ApiOrganization
 from .api_organization_allowed_email_domains import ApiOrganizationAllowedEmailDomains
 from .api_organization_allowed_email_domains_status import ApiOrganizationAllowedEmailDomainsStatus
 from .api_organization_member_profile import ApiOrganizationMemberProfile
 from .api_organization_member_profile_status import ApiOrganizationMemberProfileStatus
 from .api_organization_member_profiles import ApiOrganizationMemberProfiles
 from .api_organization_member_profiles_status import ApiOrganizationMemberProfilesStatus
+from .api_organization_projects import ApiOrganizationProjects
+from .api_organization_projects_status import ApiOrganizationProjectsStatus
 from .api_organization_status import ApiOrganizationStatus
 from .api_pinned_items import ApiPinnedItems
 from .api_pinned_items_status import ApiPinnedItemsStatus
 from .api_project_access_list_response import ApiProjectAccessListResponse
 from .api_project_access_list_response_status import ApiProjectAccessListResponseStatus
+from .api_project_response_status import ApiProjectResponseStatus
 from .api_run_query_response import ApiRunQueryResponse
 from .api_run_query_response_results import ApiRunQueryResponseResults
 from .api_run_query_response_status import ApiRunQueryResponseStatus
 from .api_scheduled_jobs_response import ApiScheduledJobsResponse
 from .api_scheduled_jobs_response_status import ApiScheduledJobsResponseStatus
 from .api_scheduler_and_targets_response_status import ApiSchedulerAndTargetsResponseStatus
 from .api_scheduler_logs_response_status import ApiSchedulerLogsResponseStatus
@@ -65,16 +68,32 @@
 from .chart_kind import ChartKind
 from .chart_summary import ChartSummary
 from .chart_type import ChartType
 from .compact import Compact
 from .compact_or_alias_type_1 import CompactOrAliasType1
 from .create_project_member import CreateProjectMember
 from .create_space import CreateSpace
+from .dbt_azure_dev_ops_project_config import DbtAzureDevOpsProjectConfig
+from .dbt_bit_bucket_project_config import DbtBitBucketProjectConfig
+from .dbt_cloud_ide_project_config import DbtCloudIDEProjectConfig
 from .dbt_cloud_metadata_response_metrics import DbtCloudMetadataResponseMetrics
 from .dbt_cloud_metric import DbtCloudMetric
+from .dbt_github_project_config import DbtGithubProjectConfig
+from .dbt_gitlab_project_config import DbtGitlabProjectConfig
+from .dbt_local_project_config import DbtLocalProjectConfig
+from .dbt_none_project_config import DbtNoneProjectConfig
+from .dbt_project_environment_variable import DbtProjectEnvironmentVariable
+from .dbt_project_type import DbtProjectType
+from .dbt_project_type_azuredevops import DbtProjectTypeAZUREDEVOPS
+from .dbt_project_type_bitbucket import DbtProjectTypeBITBUCKET
+from .dbt_project_type_dbt import DbtProjectTypeDBT
+from .dbt_project_type_dbtcloudide import DbtProjectTypeDBTCLOUDIDE
+from .dbt_project_type_github import DbtProjectTypeGITHUB
+from .dbt_project_type_gitlab import DbtProjectTypeGITLAB
+from .dbt_project_type_none import DbtProjectTypeNONE
 from .delete_scheduler_response_201 import DeleteSchedulerResponse201
 from .delete_scheduler_response_201_status import DeleteSchedulerResponse201Status
 from .email_one_time_password import EmailOneTimePassword
 from .email_one_time_password_expiring import EmailOneTimePasswordExpiring
 from .email_status import EmailStatus
 from .filter_group_response_type_0 import FilterGroupResponseType0
 from .filter_group_response_type_1 import FilterGroupResponseType1
@@ -82,24 +101,46 @@
 from .group import Group
 from .group_member import GroupMember
 from .metric_query_response import MetricQueryResponse
 from .metric_type import MetricType
 from .organization import Organization
 from .organization_member_profile import OrganizationMemberProfile
 from .organization_member_role import OrganizationMemberRole
+from .organization_project import OrganizationProject
 from .partial_omit_organization_organization_uuid_or_needs_project import (
     PartialOmitOrganizationOrganizationUuidOrNeedsProject,
 )
 from .partial_pick_organization_member_profile_role import PartialPickOrganizationMemberProfileRole
 from .partial_pick_space_is_private_or_access import PartialPickSpaceIsPrivateOrAccess
 from .pick_allowed_email_domains_exclude_keyof_allowed_email_domains_organization_uuid import (
     PickAllowedEmailDomainsExcludeKeyofAllowedEmailDomainsOrganizationUuid,
 )
+from .pick_create_bigquery_credentials_exclude_keyof_create_bigquery_credentials_sensitive_credentials_field_names import (
+    PickCreateBigqueryCredentialsExcludeKeyofCreateBigqueryCredentialsSensitiveCredentialsFieldNames,
+)
+from .pick_create_bigquery_credentials_exclude_keyof_create_bigquery_credentials_sensitive_credentials_field_names_priority import (
+    PickCreateBigqueryCredentialsExcludeKeyofCreateBigqueryCredentialsSensitiveCredentialsFieldNamesPriority,
+)
+from .pick_create_databricks_credentials_exclude_keyof_create_databricks_credentials_sensitive_credentials_field_names import (
+    PickCreateDatabricksCredentialsExcludeKeyofCreateDatabricksCredentialsSensitiveCredentialsFieldNames,
+)
 from .pick_create_dbt_cloud_integration_metrics_job_id import PickCreateDbtCloudIntegrationMetricsJobId
 from .pick_create_group_name import PickCreateGroupName
+from .pick_create_postgres_credentials_exclude_keyof_create_postgres_credentials_sensitive_credentials_field_names import (
+    PickCreatePostgresCredentialsExcludeKeyofCreatePostgresCredentialsSensitiveCredentialsFieldNames,
+)
+from .pick_create_redshift_credentials_exclude_keyof_create_redshift_credentials_sensitive_credentials_field_names import (
+    PickCreateRedshiftCredentialsExcludeKeyofCreateRedshiftCredentialsSensitiveCredentialsFieldNames,
+)
+from .pick_create_snowflake_credentials_exclude_keyof_create_snowflake_credentials_sensitive_credentials_field_names import (
+    PickCreateSnowflakeCredentialsExcludeKeyofCreateSnowflakeCredentialsSensitiveCredentialsFieldNames,
+)
+from .pick_create_trino_credentials_exclude_keyof_create_trino_credentials_sensitive_credentials_field_names import (
+    PickCreateTrinoCredentialsExcludeKeyofCreateTrinoCredentialsSensitiveCredentialsFieldNames,
+)
 from .pick_dashboard_uuid_or_name_or_description_or_updated_at_or_project_uuid_or_updated_by_user_or_organization_uuid_or_space_uuid_or_views_or_first_viewed_at_or_pinned_list_uuid_or_pinned_list_order import (
     PickDashboardUuidOrNameOrDescriptionOrUpdatedAtOrProjectUuidOrUpdatedByUserOrOrganizationUuidOrSpaceUuidOrViewsOrFirstViewedAtOrPinnedListUuidOrPinnedListOrder,
 )
 from .pick_group_name import PickGroupName
 from .pick_organization_name import PickOrganizationName
 from .pick_resource_view_item_at_data_uuid_or_pinned_list_order import PickResourceViewItemAtDataUuidOrPinnedListOrder
 from .pick_saved_chart_uuid_or_name_or_description_or_space_name_or_space_uuid_or_project_uuid_or_organization_uuid_or_pinned_list_uuid import (
@@ -124,14 +165,15 @@
 )
 from .pick_validation_response_error_or_created_at_or_validation_id import (
     PickValidationResponseErrorOrCreatedAtOrValidationId,
 )
 from .post_chart_results_json_body import PostChartResultsJsonBody
 from .project_member_profile import ProjectMemberProfile
 from .project_member_role import ProjectMemberRole
+from .project_type import ProjectType
 from .record_string_any import RecordStringAny
 from .resource_view_item_type import ResourceViewItemType
 from .resource_view_item_type_chart import ResourceViewItemTypeCHART
 from .resource_view_item_type_dashboard import ResourceViewItemTypeDASHBOARD
 from .resource_view_item_type_space import ResourceViewItemTypeSPACE
 from .resource_view_space_item import ResourceViewSpaceItem
 from .resource_view_space_item_data import ResourceViewSpaceItemData
@@ -162,14 +204,21 @@
 from .validate_project_json_body import ValidateProjectJsonBody
 from .validation_error_chart_response import ValidationErrorChartResponse
 from .validation_error_dashboard_response import ValidationErrorDashboardResponse
 from .validation_error_type import ValidationErrorType
 from .validation_response_base import ValidationResponseBase
 from .validation_source_type import ValidationSourceType
 from .view_statistics import ViewStatistics
+from .warehouse_types_bigquery import WarehouseTypesBIGQUERY
+from .warehouse_types_databricks import WarehouseTypesDATABRICKS
+from .warehouse_types_postgres import WarehouseTypesPOSTGRES
+from .warehouse_types_redshift import WarehouseTypesREDSHIFT
+from .warehouse_types_snowflake import WarehouseTypesSNOWFLAKE
+from .warehouse_types_trino import WarehouseTypesTRINO
+from .week_day import WeekDay
 
 __all__ = (
     "AdditionalMetric",
     "AllowedEmailDomains",
     "ApiChartSummaryListResponse",
     "ApiChartSummaryListResponseStatus",
     "ApiCsvUrlResponse",
@@ -198,19 +247,22 @@
     "ApiOrganization",
     "ApiOrganizationAllowedEmailDomains",
     "ApiOrganizationAllowedEmailDomainsStatus",
     "ApiOrganizationMemberProfile",
     "ApiOrganizationMemberProfiles",
     "ApiOrganizationMemberProfilesStatus",
     "ApiOrganizationMemberProfileStatus",
+    "ApiOrganizationProjects",
+    "ApiOrganizationProjectsStatus",
     "ApiOrganizationStatus",
     "ApiPinnedItems",
     "ApiPinnedItemsStatus",
     "ApiProjectAccessListResponse",
     "ApiProjectAccessListResponseStatus",
+    "ApiProjectResponseStatus",
     "ApiRunQueryResponse",
     "ApiRunQueryResponseResults",
     "ApiRunQueryResponseStatus",
     "ApiScheduledJobsResponse",
     "ApiScheduledJobsResponseStatus",
     "ApiSchedulerAndTargetsResponseStatus",
     "ApiSchedulerLogsResponseStatus",
@@ -234,16 +286,32 @@
     "ChartKind",
     "ChartSummary",
     "ChartType",
     "Compact",
     "CompactOrAliasType1",
     "CreateProjectMember",
     "CreateSpace",
+    "DbtAzureDevOpsProjectConfig",
+    "DbtBitBucketProjectConfig",
+    "DbtCloudIDEProjectConfig",
     "DbtCloudMetadataResponseMetrics",
     "DbtCloudMetric",
+    "DbtGithubProjectConfig",
+    "DbtGitlabProjectConfig",
+    "DbtLocalProjectConfig",
+    "DbtNoneProjectConfig",
+    "DbtProjectEnvironmentVariable",
+    "DbtProjectType",
+    "DbtProjectTypeAZUREDEVOPS",
+    "DbtProjectTypeBITBUCKET",
+    "DbtProjectTypeDBT",
+    "DbtProjectTypeDBTCLOUDIDE",
+    "DbtProjectTypeGITHUB",
+    "DbtProjectTypeGITLAB",
+    "DbtProjectTypeNONE",
     "DeleteSchedulerResponse201",
     "DeleteSchedulerResponse201Status",
     "EmailOneTimePassword",
     "EmailOneTimePasswordExpiring",
     "EmailStatus",
     "FilterGroupResponseType0",
     "FilterGroupResponseType1",
@@ -251,20 +319,28 @@
     "Group",
     "GroupMember",
     "MetricQueryResponse",
     "MetricType",
     "Organization",
     "OrganizationMemberProfile",
     "OrganizationMemberRole",
+    "OrganizationProject",
     "PartialOmitOrganizationOrganizationUuidOrNeedsProject",
     "PartialPickOrganizationMemberProfileRole",
     "PartialPickSpaceIsPrivateOrAccess",
     "PickAllowedEmailDomainsExcludeKeyofAllowedEmailDomainsOrganizationUuid",
+    "PickCreateBigqueryCredentialsExcludeKeyofCreateBigqueryCredentialsSensitiveCredentialsFieldNames",
+    "PickCreateBigqueryCredentialsExcludeKeyofCreateBigqueryCredentialsSensitiveCredentialsFieldNamesPriority",
+    "PickCreateDatabricksCredentialsExcludeKeyofCreateDatabricksCredentialsSensitiveCredentialsFieldNames",
     "PickCreateDbtCloudIntegrationMetricsJobId",
     "PickCreateGroupName",
+    "PickCreatePostgresCredentialsExcludeKeyofCreatePostgresCredentialsSensitiveCredentialsFieldNames",
+    "PickCreateRedshiftCredentialsExcludeKeyofCreateRedshiftCredentialsSensitiveCredentialsFieldNames",
+    "PickCreateSnowflakeCredentialsExcludeKeyofCreateSnowflakeCredentialsSensitiveCredentialsFieldNames",
+    "PickCreateTrinoCredentialsExcludeKeyofCreateTrinoCredentialsSensitiveCredentialsFieldNames",
     "PickDashboardUuidOrNameOrDescriptionOrUpdatedAtOrProjectUuidOrUpdatedByUserOrOrganizationUuidOrSpaceUuidOrViewsOrFirstViewedAtOrPinnedListUuidOrPinnedListOrder",
     "PickGroupName",
     "PickOrganizationName",
     "PickResourceViewItemAtDataUuidOrPinnedListOrder",
     "PickSavedChartUuidOrNameOrDescriptionOrSpaceNameOrSpaceUuidOrProjectUuidOrOrganizationUuidOrPinnedListUuid",
     "PickSavedChartUuidOrNameOrUpdatedAtOrUpdatedByUserOrDescriptionOrSpaceUuidOrPinnedListUuidOrPinnedListOrder",
     "PickShareUrlPathOrParams",
@@ -275,14 +351,15 @@
     "PickSpaceShareUserUuid",
     "PickSshKeyPairPublicKey",
     "PickValidationResponseBaseExcludeKeyofValidationResponseBaseName",
     "PickValidationResponseErrorOrCreatedAtOrValidationId",
     "PostChartResultsJsonBody",
     "ProjectMemberProfile",
     "ProjectMemberRole",
+    "ProjectType",
     "RecordStringAny",
     "ResourceViewItemType",
     "ResourceViewItemTypeCHART",
     "ResourceViewItemTypeDASHBOARD",
     "ResourceViewItemTypeSPACE",
     "ResourceViewSpaceItem",
     "ResourceViewSpaceItemData",
@@ -313,8 +390,15 @@
     "ValidateProjectJsonBody",
     "ValidationErrorChartResponse",
     "ValidationErrorDashboardResponse",
     "ValidationErrorType",
     "ValidationResponseBase",
     "ValidationSourceType",
     "ViewStatistics",
+    "WarehouseTypesBIGQUERY",
+    "WarehouseTypesDATABRICKS",
+    "WarehouseTypesPOSTGRES",
+    "WarehouseTypesREDSHIFT",
+    "WarehouseTypesSNOWFLAKE",
+    "WarehouseTypesTRINO",
+    "WeekDay",
 )
```

### Comparing `lightdash_client_python-0.613.2/lightdash_client/models/additional_metric.py` & `lightdash_client_python-0.618.0/lightdash_client/models/additional_metric.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.613.2/lightdash_client/models/allowed_email_domains.py` & `lightdash_client_python-0.618.0/lightdash_client/models/allowed_email_domains.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.613.2/lightdash_client/models/api_chart_summary_list_response.py` & `lightdash_client_python-0.618.0/lightdash_client/models/api_chart_summary_list_response.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.613.2/lightdash_client/models/api_csv_url_response.py` & `lightdash_client_python-0.618.0/lightdash_client/models/api_csv_url_response.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.613.2/lightdash_client/models/api_csv_url_response_results.py` & `lightdash_client_python-0.618.0/lightdash_client/models/api_csv_url_response_results.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.613.2/lightdash_client/models/api_dbt_cloud_metrics.py` & `lightdash_client_python-0.618.0/lightdash_client/models/api_dbt_cloud_metrics.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.613.2/lightdash_client/models/api_dbt_cloud_settings_delete_success.py` & `lightdash_client_python-0.618.0/lightdash_client/models/api_dbt_cloud_settings_delete_success.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.613.2/lightdash_client/models/api_error_payload.py` & `lightdash_client_python-0.618.0/lightdash_client/models/api_error_payload.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.613.2/lightdash_client/models/api_error_payload_error.py` & `lightdash_client_python-0.618.0/lightdash_client/models/api_error_payload_error.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.613.2/lightdash_client/models/api_group_list_response.py` & `lightdash_client_python-0.618.0/lightdash_client/models/api_group_list_response.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.613.2/lightdash_client/models/api_group_members_response.py` & `lightdash_client_python-0.618.0/lightdash_client/models/api_group_members_response.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.613.2/lightdash_client/models/api_group_response.py` & `lightdash_client_python-0.618.0/lightdash_client/models/api_group_response.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.613.2/lightdash_client/models/api_job_scheduled_response.py` & `lightdash_client_python-0.618.0/lightdash_client/models/api_job_scheduled_response.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.613.2/lightdash_client/models/api_job_scheduled_response_results.py` & `lightdash_client_python-0.618.0/lightdash_client/models/api_job_scheduled_response_results.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.613.2/lightdash_client/models/api_job_status_response.py` & `lightdash_client_python-0.618.0/lightdash_client/models/api_job_status_response.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.613.2/lightdash_client/models/api_job_status_response_results.py` & `lightdash_client_python-0.618.0/lightdash_client/models/api_job_status_response_results.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.613.2/lightdash_client/models/api_organization.py` & `lightdash_client_python-0.618.0/lightdash_client/models/api_organization.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.613.2/lightdash_client/models/api_organization_allowed_email_domains.py` & `lightdash_client_python-0.618.0/lightdash_client/models/api_organization_allowed_email_domains.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.613.2/lightdash_client/models/api_organization_member_profile.py` & `lightdash_client_python-0.618.0/lightdash_client/models/api_organization_member_profile.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.613.2/lightdash_client/models/api_organization_member_profiles.py` & `lightdash_client_python-0.618.0/lightdash_client/models/api_organization_member_profiles.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.613.2/lightdash_client/models/api_pinned_items.py` & `lightdash_client_python-0.618.0/lightdash_client/models/api_pinned_items.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.613.2/lightdash_client/models/api_project_access_list_response.py` & `lightdash_client_python-0.618.0/lightdash_client/models/api_project_access_list_response.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.613.2/lightdash_client/models/api_run_query_response.py` & `lightdash_client_python-0.618.0/lightdash_client/models/api_run_query_response.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.613.2/lightdash_client/models/api_run_query_response_results.py` & `lightdash_client_python-0.618.0/lightdash_client/models/api_run_query_response_results.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.613.2/lightdash_client/models/api_scheduled_jobs_response.py` & `lightdash_client_python-0.618.0/lightdash_client/models/api_scheduled_jobs_response.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.613.2/lightdash_client/models/api_share_response.py` & `lightdash_client_python-0.618.0/lightdash_client/models/api_share_response.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.613.2/lightdash_client/models/api_slack_channels_response.py` & `lightdash_client_python-0.618.0/lightdash_client/models/api_slack_channels_response.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.613.2/lightdash_client/models/api_space_summary_list_response.py` & `lightdash_client_python-0.618.0/lightdash_client/models/api_space_summary_list_response.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.613.2/lightdash_client/models/api_ssh_key_pair_response.py` & `lightdash_client_python-0.618.0/lightdash_client/models/api_ssh_key_pair_response.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.613.2/lightdash_client/models/api_success_empty.py` & `lightdash_client_python-0.618.0/lightdash_client/models/api_success_empty.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.613.2/lightdash_client/models/api_user_allowed_organizations_response.py` & `lightdash_client_python-0.618.0/lightdash_client/models/api_user_allowed_organizations_response.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.613.2/lightdash_client/models/api_validate_response.py` & `lightdash_client_python-0.618.0/lightdash_client/models/api_validate_response.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.613.2/lightdash_client/models/api_validation_dismiss_response.py` & `lightdash_client_python-0.618.0/lightdash_client/models/api_validation_dismiss_response.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.613.2/lightdash_client/models/chart_summary.py` & `lightdash_client_python-0.618.0/lightdash_client/models/chart_summary.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.613.2/lightdash_client/models/create_project_member.py` & `lightdash_client_python-0.618.0/lightdash_client/models/create_project_member.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.613.2/lightdash_client/models/create_space.py` & `lightdash_client_python-0.618.0/lightdash_client/models/create_space.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.613.2/lightdash_client/models/dbt_cloud_metadata_response_metrics.py` & `lightdash_client_python-0.618.0/lightdash_client/models/dbt_cloud_metadata_response_metrics.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.613.2/lightdash_client/models/dbt_cloud_metric.py` & `lightdash_client_python-0.618.0/lightdash_client/models/dbt_cloud_metric.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.613.2/lightdash_client/models/delete_scheduler_response_201.py` & `lightdash_client_python-0.618.0/lightdash_client/models/delete_scheduler_response_201.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.613.2/lightdash_client/models/email_one_time_password.py` & `lightdash_client_python-0.618.0/lightdash_client/models/email_one_time_password.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.613.2/lightdash_client/models/email_one_time_password_expiring.py` & `lightdash_client_python-0.618.0/lightdash_client/models/email_one_time_password_expiring.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.613.2/lightdash_client/models/email_status.py` & `lightdash_client_python-0.618.0/lightdash_client/models/email_status.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.613.2/lightdash_client/models/filter_group_response_type_0.py` & `lightdash_client_python-0.618.0/lightdash_client/models/filter_group_response_type_0.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.613.2/lightdash_client/models/filter_group_response_type_1.py` & `lightdash_client_python-0.618.0/lightdash_client/models/filter_group_response_type_1.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.613.2/lightdash_client/models/filters.py` & `lightdash_client_python-0.618.0/lightdash_client/models/filters.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.613.2/lightdash_client/models/group.py` & `lightdash_client_python-0.618.0/lightdash_client/models/group.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.613.2/lightdash_client/models/group_member.py` & `lightdash_client_python-0.618.0/lightdash_client/models/group_member.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.613.2/lightdash_client/models/metric_query_response.py` & `lightdash_client_python-0.618.0/lightdash_client/models/metric_query_response.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.613.2/lightdash_client/models/organization.py` & `lightdash_client_python-0.618.0/lightdash_client/models/organization.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.613.2/lightdash_client/models/organization_member_profile.py` & `lightdash_client_python-0.618.0/lightdash_client/models/organization_member_profile.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.613.2/lightdash_client/models/partial_omit_organization_organization_uuid_or_needs_project.py` & `lightdash_client_python-0.618.0/lightdash_client/models/partial_omit_organization_organization_uuid_or_needs_project.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.613.2/lightdash_client/models/partial_pick_organization_member_profile_role.py` & `lightdash_client_python-0.618.0/lightdash_client/models/partial_pick_organization_member_profile_role.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.613.2/lightdash_client/models/partial_pick_space_is_private_or_access.py` & `lightdash_client_python-0.618.0/lightdash_client/models/partial_pick_space_is_private_or_access.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.613.2/lightdash_client/models/pick_allowed_email_domains_exclude_keyof_allowed_email_domains_organization_uuid.py` & `lightdash_client_python-0.618.0/lightdash_client/models/pick_allowed_email_domains_exclude_keyof_allowed_email_domains_organization_uuid.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.613.2/lightdash_client/models/pick_create_dbt_cloud_integration_metrics_job_id.py` & `lightdash_client_python-0.618.0/lightdash_client/models/pick_create_dbt_cloud_integration_metrics_job_id.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.613.2/lightdash_client/models/pick_create_group_name.py` & `lightdash_client_python-0.618.0/lightdash_client/models/pick_create_group_name.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.613.2/lightdash_client/models/pick_dashboard_uuid_or_name_or_description_or_updated_at_or_project_uuid_or_updated_by_user_or_organization_uuid_or_space_uuid_or_views_or_first_viewed_at_or_pinned_list_uuid_or_pinned_list_order.py` & `lightdash_client_python-0.618.0/lightdash_client/models/pick_dashboard_uuid_or_name_or_description_or_updated_at_or_project_uuid_or_updated_by_user_or_organization_uuid_or_space_uuid_or_views_or_first_viewed_at_or_pinned_list_uuid_or_pinned_list_order.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.613.2/lightdash_client/models/pick_group_name.py` & `lightdash_client_python-0.618.0/lightdash_client/models/pick_group_name.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.613.2/lightdash_client/models/pick_organization_name.py` & `lightdash_client_python-0.618.0/lightdash_client/models/pick_organization_name.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.613.2/lightdash_client/models/pick_resource_view_item_at_data_uuid_or_pinned_list_order.py` & `lightdash_client_python-0.618.0/lightdash_client/models/pick_resource_view_item_at_data_uuid_or_pinned_list_order.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.613.2/lightdash_client/models/pick_saved_chart_uuid_or_name_or_description_or_space_name_or_space_uuid_or_project_uuid_or_organization_uuid_or_pinned_list_uuid.py` & `lightdash_client_python-0.618.0/lightdash_client/models/pick_saved_chart_uuid_or_name_or_description_or_space_name_or_space_uuid_or_project_uuid_or_organization_uuid_or_pinned_list_uuid.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.613.2/lightdash_client/models/pick_saved_chart_uuid_or_name_or_updated_at_or_updated_by_user_or_description_or_space_uuid_or_pinned_list_uuid_or_pinned_list_order.py` & `lightdash_client_python-0.618.0/lightdash_client/models/pick_saved_chart_uuid_or_name_or_updated_at_or_updated_by_user_or_description_or_space_uuid_or_pinned_list_uuid_or_pinned_list_order.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.613.2/lightdash_client/models/pick_share_url_path_or_params.py` & `lightdash_client_python-0.618.0/lightdash_client/models/pick_share_url_path_or_params.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.613.2/lightdash_client/models/pick_space_name.py` & `lightdash_client_python-0.618.0/lightdash_client/models/pick_space_name.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.613.2/lightdash_client/models/pick_space_name_or_is_private.py` & `lightdash_client_python-0.618.0/lightdash_client/models/pick_space_name_or_is_private.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.613.2/lightdash_client/models/pick_space_organization_uuid_or_project_uuid_or_uuid_or_name_or_is_private.py` & `lightdash_client_python-0.618.0/lightdash_client/models/pick_space_organization_uuid_or_project_uuid_or_uuid_or_name_or_is_private.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.613.2/lightdash_client/models/pick_space_project_uuid_or_uuid_or_name_or_is_private_or_pinned_list_uuid_or_pinned_list_order_or_organization_uuid.py` & `lightdash_client_python-0.618.0/lightdash_client/models/pick_space_project_uuid_or_uuid_or_name_or_is_private_or_pinned_list_uuid_or_pinned_list_order_or_organization_uuid.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.613.2/lightdash_client/models/pick_space_share_user_uuid.py` & `lightdash_client_python-0.618.0/lightdash_client/models/pick_space_share_user_uuid.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.613.2/lightdash_client/models/pick_ssh_key_pair_public_key.py` & `lightdash_client_python-0.618.0/lightdash_client/models/pick_ssh_key_pair_public_key.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.613.2/lightdash_client/models/pick_validation_response_base_exclude_keyof_validation_response_base_name.py` & `lightdash_client_python-0.618.0/lightdash_client/models/pick_validation_response_base_exclude_keyof_validation_response_base_name.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.613.2/lightdash_client/models/pick_validation_response_error_or_created_at_or_validation_id.py` & `lightdash_client_python-0.618.0/lightdash_client/models/pick_validation_response_error_or_created_at_or_validation_id.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.613.2/lightdash_client/models/post_chart_results_json_body.py` & `lightdash_client_python-0.618.0/lightdash_client/models/post_chart_results_json_body.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.613.2/lightdash_client/models/project_member_profile.py` & `lightdash_client_python-0.618.0/lightdash_client/models/project_member_profile.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.613.2/lightdash_client/models/record_string_any.py` & `lightdash_client_python-0.618.0/lightdash_client/models/record_string_any.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.613.2/lightdash_client/models/resource_view_space_item.py` & `lightdash_client_python-0.618.0/lightdash_client/models/resource_view_space_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.613.2/lightdash_client/models/resource_view_space_item_data.py` & `lightdash_client_python-0.618.0/lightdash_client/models/resource_view_space_item_data.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.613.2/lightdash_client/models/run_query_request.py` & `lightdash_client_python-0.618.0/lightdash_client/models/run_query_request.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.613.2/lightdash_client/models/run_query_request_filters.py` & `lightdash_client_python-0.618.0/lightdash_client/models/run_query_request_filters.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.613.2/lightdash_client/models/scheduled_jobs.py` & `lightdash_client_python-0.618.0/lightdash_client/models/scheduled_jobs.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.613.2/lightdash_client/models/scheduler_base.py` & `lightdash_client_python-0.618.0/lightdash_client/models/scheduler_base.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.613.2/lightdash_client/models/scheduler_csv_options.py` & `lightdash_client_python-0.618.0/lightdash_client/models/scheduler_csv_options.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.613.2/lightdash_client/models/scheduler_email_target.py` & `lightdash_client_python-0.618.0/lightdash_client/models/scheduler_email_target.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.613.2/lightdash_client/models/scheduler_image_options.py` & `lightdash_client_python-0.618.0/lightdash_client/models/scheduler_image_options.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.613.2/lightdash_client/models/scheduler_log.py` & `lightdash_client_python-0.618.0/lightdash_client/models/scheduler_log.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.613.2/lightdash_client/models/scheduler_slack_target.py` & `lightdash_client_python-0.618.0/lightdash_client/models/scheduler_slack_target.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.613.2/lightdash_client/models/share_url.py` & `lightdash_client_python-0.618.0/lightdash_client/models/share_url.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.613.2/lightdash_client/models/slack_channel.py` & `lightdash_client_python-0.618.0/lightdash_client/models/slack_channel.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.613.2/lightdash_client/models/sort_field.py` & `lightdash_client_python-0.618.0/lightdash_client/models/sort_field.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.613.2/lightdash_client/models/space_share.py` & `lightdash_client_python-0.618.0/lightdash_client/models/space_share.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.613.2/lightdash_client/models/space_summary.py` & `lightdash_client_python-0.618.0/lightdash_client/models/space_summary.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.613.2/lightdash_client/models/table_calculation.py` & `lightdash_client_python-0.618.0/lightdash_client/models/table_calculation.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.613.2/lightdash_client/models/update_pinned_item_order.py` & `lightdash_client_python-0.618.0/lightdash_client/models/update_pinned_item_order.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.613.2/lightdash_client/models/update_project_member.py` & `lightdash_client_python-0.618.0/lightdash_client/models/update_project_member.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.613.2/lightdash_client/models/updated_by_user.py` & `lightdash_client_python-0.618.0/lightdash_client/models/updated_by_user.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.613.2/lightdash_client/models/user_allowed_organization.py` & `lightdash_client_python-0.618.0/lightdash_client/models/user_allowed_organization.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.613.2/lightdash_client/models/validate_project_json_body.py` & `lightdash_client_python-0.618.0/lightdash_client/models/validate_project_json_body.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.613.2/lightdash_client/models/validation_error_chart_response.py` & `lightdash_client_python-0.618.0/lightdash_client/models/validation_error_chart_response.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.613.2/lightdash_client/models/validation_error_dashboard_response.py` & `lightdash_client_python-0.618.0/lightdash_client/models/validation_error_dashboard_response.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.613.2/lightdash_client/models/validation_response_base.py` & `lightdash_client_python-0.618.0/lightdash_client/models/validation_response_base.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.613.2/lightdash_client/models/view_statistics.py` & `lightdash_client_python-0.618.0/lightdash_client/models/view_statistics.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.613.2/lightdash_client/types.py` & `lightdash_client_python-0.618.0/lightdash_client/types.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.613.2/pyproject.toml` & `lightdash_client_python-0.618.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.613.2/setup.py` & `lightdash_client_python-0.618.0/setup.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.613.2/tests/__init__.py` & `lightdash_client_python-0.618.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.613.2/tests/test_dummy.py` & `lightdash_client_python-0.618.0/tests/test_dummy.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.613.2/PKG-INFO` & `lightdash_client_python-0.618.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lightdash-client-python
-Version: 0.613.2
+Version: 0.618.0
 Summary: A client library for accessing Lightdash API 
 Author: yu-iskw
 Requires-Python: >=3.8.0,<4
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
```

