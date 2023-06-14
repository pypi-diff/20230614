# Comparing `tmp/lightdash_client_python-0.1.2.tar.gz` & `tmp/lightdash_client_python-0.611.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lightdash_client_python-0.1.2.tar", last modified: Thu May 25 04:23:15 2023, max compression
+gzip compressed data, was "lightdash_client_python-0.611.0.tar", last modified: Wed Jun 14 04:54:50 2023, max compression
```

## Comparing `lightdash_client_python-0.1.2.tar` & `lightdash_client_python-0.611.0.tar`

### file list

```diff
@@ -1,161 +1,248 @@
--rw-r--r--   0        0        0      804 2023-05-25 04:23:15.000000 lightdash_client_python-0.1.2/.github/CODEOWNERS
--rw-r--r--   0        0        0      402 2023-05-25 04:23:15.000000 lightdash_client_python-0.1.2/.github/workflows/contributors-list.yml
--rw-r--r--   0        0        0     1849 2023-05-25 04:23:15.000000 lightdash_client_python-0.1.2/.github/workflows/publish.yml
--rw-r--r--   0        0        0     2335 2023-05-25 04:23:15.000000 lightdash_client_python-0.1.2/.github/workflows/test-publish.yml
--rw-r--r--   0        0        0     1115 2023-05-25 04:23:15.000000 lightdash_client_python-0.1.2/.github/workflows/test.yml
--rw-r--r--   0        0        0     3078 2023-05-25 04:23:15.000000 lightdash_client_python-0.1.2/.gitignore
--rw-r--r--   0        0        0     1040 2023-05-25 04:23:15.000000 lightdash_client_python-0.1.2/.openapi-generator-ignore
--rw-r--r--   0        0        0     6821 2023-05-25 04:23:15.000000 lightdash_client_python-0.1.2/.openapi-generator/FILES
--rw-r--r--   0        0        0        6 2023-05-25 04:23:15.000000 lightdash_client_python-0.1.2/.openapi-generator/VERSION
--rw-r--r--   0        0        0     1266 2023-05-25 04:23:15.000000 lightdash_client_python-0.1.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0    14088 2023-05-25 04:23:15.000000 lightdash_client_python-0.1.2/.pylintrc
--rw-r--r--   0        0        0      150 2023-05-25 04:23:15.000000 lightdash_client_python-0.1.2/.pypirc
--rw-r--r--   0        0        0        8 2023-05-25 04:23:15.000000 lightdash_client_python-0.1.2/.python-version
--rw-r--r--   0        0        0       32 2023-05-25 04:23:15.000000 lightdash_client_python-0.1.2/.style.yapf
--rw-r--r--   0        0        0    11357 2023-05-25 04:23:15.000000 lightdash_client_python-0.1.2/LICENSE
--rw-r--r--   0        0        0      587 2023-05-25 04:23:15.000000 lightdash_client_python-0.1.2/Makefile
--rw-r--r--   0        0        0     3258 2023-05-25 04:23:15.000000 lightdash_client_python-0.1.2/README.md
--rwxr-xr-x   0        0        0     1121 2023-05-25 04:23:15.000000 lightdash_client_python-0.1.2/dev/clean.sh
--rw-r--r--   0        0        0     2004 2023-05-25 04:23:15.000000 lightdash_client_python-0.1.2/dev/generate_clients.sh
--rw-r--r--   0        0        0      974 2023-05-25 04:23:15.000000 lightdash_client_python-0.1.2/dev/lint.sh
--rw-r--r--   0        0        0      193 2023-05-25 04:23:15.000000 lightdash_client_python-0.1.2/dev/openapi-python-client.yml
--rwxr-xr-x   0        0        0     1391 2023-05-25 04:23:15.000000 lightdash_client_python-0.1.2/dev/publish.sh
--rw-r--r--   0        0        0    69729 2023-05-25 04:23:15.000000 lightdash_client_python-0.1.2/dev/schemas/lightdash-api.json
--rwxr-xr-x   0        0        0     1023 2023-05-25 04:23:15.000000 lightdash_client_python-0.1.2/dev/setup.sh
--rwxr-xr-x   0        0        0      958 2023-05-25 04:23:15.000000 lightdash_client_python-0.1.2/dev/test_python.sh
--rw-r--r--   0        0        0      199 2023-05-25 04:23:15.000000 lightdash_client_python-0.1.2/lightdash_client/__init__.py
--rw-r--r--   0        0        0       47 2023-05-25 04:23:15.000000 lightdash_client_python-0.1.2/lightdash_client/api/__init__.py
--rw-r--r--   0        0        0        0 2023-05-25 04:23:15.000000 lightdash_client_python-0.1.2/lightdash_client/api/dashboard/__init__.py
--rw-r--r--   0        0        0     2793 2023-05-25 04:23:15.000000 lightdash_client_python-0.1.2/lightdash_client/api/dashboard/delete_dashboard.py
--rw-r--r--   0        0        0     2736 2023-05-25 04:23:15.000000 lightdash_client_python-0.1.2/lightdash_client/api/dashboard/get_dashboard.py
--rw-r--r--   0        0        0     5064 2023-05-25 04:23:15.000000 lightdash_client_python-0.1.2/lightdash_client/api/dashboard/get_dashboards.py
--rw-r--r--   0        0        0     3689 2023-05-25 04:23:15.000000 lightdash_client_python-0.1.2/lightdash_client/api/dashboard/patch_dashboard.py
--rw-r--r--   0        0        0        0 2023-05-25 04:23:15.000000 lightdash_client_python-0.1.2/lightdash_client/api/job/__init__.py
--rw-r--r--   0        0        0     3926 2023-05-25 04:23:15.000000 lightdash_client_python-0.1.2/lightdash_client/api/job/get_job.py
--rw-r--r--   0        0        0        0 2023-05-25 04:23:15.000000 lightdash_client_python-0.1.2/lightdash_client/api/organization/__init__.py
--rw-r--r--   0        0        0     2697 2023-05-25 04:23:15.000000 lightdash_client_python-0.1.2/lightdash_client/api/organization/delete_organization_project.py
--rw-r--r--   0        0        0     2652 2023-05-25 04:23:15.000000 lightdash_client_python-0.1.2/lightdash_client/api/organization/delete_organization_user.py
--rw-r--r--   0        0        0     4585 2023-05-25 04:23:15.000000 lightdash_client_python-0.1.2/lightdash_client/api/organization/get_organization_projects.py
--rw-r--r--   0        0        0     3747 2023-05-25 04:23:15.000000 lightdash_client_python-0.1.2/lightdash_client/api/organization/get_organization_users.py
--rw-r--r--   0        0        0     2414 2023-05-25 04:23:15.000000 lightdash_client_python-0.1.2/lightdash_client/api/organization/update_organization.py
--rw-r--r--   0        0        0     4959 2023-05-25 04:23:15.000000 lightdash_client_python-0.1.2/lightdash_client/api/organization/update_organization_member.py
--rw-r--r--   0        0        0        0 2023-05-25 04:23:15.000000 lightdash_client_python-0.1.2/lightdash_client/api/project/__init__.py
--rw-r--r--   0        0        0     4350 2023-05-25 04:23:15.000000 lightdash_client_python-0.1.2/lightdash_client/api/project/get_project_catalog.py
--rw-r--r--   0        0        0     4535 2023-05-25 04:23:15.000000 lightdash_client_python-0.1.2/lightdash_client/api/project/get_project_tables_configuration.py
--rw-r--r--   0        0        0     4794 2023-05-25 04:23:15.000000 lightdash_client_python-0.1.2/lightdash_client/api/project/run_sql_query.py
--rw-r--r--   0        0        0     5296 2023-05-25 04:23:15.000000 lightdash_client_python-0.1.2/lightdash_client/api/project/update_project_tables_configuration.py
--rw-r--r--   0        0        0        0 2023-05-25 04:23:15.000000 lightdash_client_python-0.1.2/lightdash_client/api/saved/__init__.py
--rw-r--r--   0        0        0     5012 2023-05-25 04:23:15.000000 lightdash_client_python-0.1.2/lightdash_client/api/saved/create_saved_chart_version.py
--rw-r--r--   0        0        0     3955 2023-05-25 04:23:15.000000 lightdash_client_python-0.1.2/lightdash_client/api/saved/delete_saved_chart.py
--rw-r--r--   0        0        0     4165 2023-05-25 04:23:15.000000 lightdash_client_python-0.1.2/lightdash_client/api/saved/get_saved_chart.py
--rw-r--r--   0        0        0     4774 2023-05-25 04:23:15.000000 lightdash_client_python-0.1.2/lightdash_client/api/saved/patch_saved_chart.py
--rw-r--r--   0        0        0     5106 2023-05-25 04:23:15.000000 lightdash_client_python-0.1.2/lightdash_client/api/saved/patch_saved_charts.py
--rw-r--r--   0        0        0     5619 2023-05-25 04:23:15.000000 lightdash_client_python-0.1.2/lightdash_client/api/saved/post_saved_chart.py
--rw-r--r--   0        0        0        0 2023-05-25 04:23:15.000000 lightdash_client_python-0.1.2/lightdash_client/api/saved_chart/__init__.py
--rw-r--r--   0        0        0     4414 2023-05-25 04:23:15.000000 lightdash_client_python-0.1.2/lightdash_client/api/saved_chart/get_available_chart_filters.py
--rw-r--r--   0        0        0        0 2023-05-25 04:23:15.000000 lightdash_client_python-0.1.2/lightdash_client/api/user/__init__.py
--rw-r--r--   0        0        0     4325 2023-05-25 04:23:15.000000 lightdash_client_python-0.1.2/lightdash_client/api/user/create_invite_link.py
--rw-r--r--   0        0        0     4580 2023-05-25 04:23:15.000000 lightdash_client_python-0.1.2/lightdash_client/api/user/create_personal_access_token.py
--rw-r--r--   0        0        0     4119 2023-05-25 04:23:15.000000 lightdash_client_python-0.1.2/lightdash_client/api/user/create_user.py
--rw-r--r--   0        0        0     2432 2023-05-25 04:23:15.000000 lightdash_client_python-0.1.2/lightdash_client/api/user/delete_invite_links.py
--rw-r--r--   0        0        0     4136 2023-05-25 04:23:15.000000 lightdash_client_python-0.1.2/lightdash_client/api/user/get_invite_link.py
--rw-r--r--   0        0        0     4028 2023-05-25 04:23:15.000000 lightdash_client_python-0.1.2/lightdash_client/api/user/get_personal_access_tokens.py
--rw-r--r--   0        0        0     3548 2023-05-25 04:23:15.000000 lightdash_client_python-0.1.2/lightdash_client/api/user/get_user.py
--rw-r--r--   0        0        0     3946 2023-05-25 04:23:15.000000 lightdash_client_python-0.1.2/lightdash_client/api/user/login_with_password.py
--rw-r--r--   0        0        0     2835 2023-05-25 04:23:15.000000 lightdash_client_python-0.1.2/lightdash_client/client.py
--rw-r--r--   0        0        0      470 2023-05-25 04:23:15.000000 lightdash_client_python-0.1.2/lightdash_client/errors.py
--rw-r--r--   0        0        0     7851 2023-05-25 04:23:15.000000 lightdash_client_python-0.1.2/lightdash_client/models/__init__.py
--rw-r--r--   0        0        0     2890 2023-05-25 04:23:15.000000 lightdash_client_python-0.1.2/lightdash_client/models/chart_config.py
--rw-r--r--   0        0        0      203 2023-05-25 04:23:15.000000 lightdash_client_python-0.1.2/lightdash_client/models/chart_config_chart_type.py
--rw-r--r--   0        0        0     1252 2023-05-25 04:23:15.000000 lightdash_client_python-0.1.2/lightdash_client/models/chart_config_config.py
--rw-r--r--   0        0        0     4530 2023-05-25 04:23:15.000000 lightdash_client_python-0.1.2/lightdash_client/models/create_dashboard_tile.py
--rw-r--r--   0        0        0      204 2023-05-25 04:23:15.000000 lightdash_client_python-0.1.2/lightdash_client/models/create_dashboard_tile_type.py
--rw-r--r--   0        0        0     1615 2023-05-25 04:23:15.000000 lightdash_client_python-0.1.2/lightdash_client/models/create_invite_link.py
--rw-r--r--   0        0        0     2409 2023-05-25 04:23:15.000000 lightdash_client_python-0.1.2/lightdash_client/models/create_invite_link_response_201.py
--rw-r--r--   0        0        0     2319 2023-05-25 04:23:15.000000 lightdash_client_python-0.1.2/lightdash_client/models/create_personal_access_token.py
--rw-r--r--   0        0        0     2596 2023-05-25 04:23:15.000000 lightdash_client_python-0.1.2/lightdash_client/models/create_personal_access_token_response_200.py
--rw-r--r--   0        0        0     5672 2023-05-25 04:23:15.000000 lightdash_client_python-0.1.2/lightdash_client/models/create_saved_chart.py
--rw-r--r--   0        0        0     1308 2023-05-25 04:23:15.000000 lightdash_client_python-0.1.2/lightdash_client/models/create_saved_chart_metric_query.py
--rw-r--r--   0        0        0     1598 2023-05-25 04:23:15.000000 lightdash_client_python-0.1.2/lightdash_client/models/create_saved_chart_pivot_config.py
--rw-r--r--   0        0        0      950 2023-05-25 04:23:15.000000 lightdash_client_python-0.1.2/lightdash_client/models/create_saved_chart_table_config.py
--rw-r--r--   0        0        0     3387 2023-05-25 04:23:15.000000 lightdash_client_python-0.1.2/lightdash_client/models/create_saved_chart_version.py
--rw-r--r--   0        0        0     1346 2023-05-25 04:23:15.000000 lightdash_client_python-0.1.2/lightdash_client/models/create_saved_chart_version_metric_query.py
--rw-r--r--   0        0        0     1636 2023-05-25 04:23:15.000000 lightdash_client_python-0.1.2/lightdash_client/models/create_saved_chart_version_pivot_config.py
--rw-r--r--   0        0        0     2447 2023-05-25 04:23:15.000000 lightdash_client_python-0.1.2/lightdash_client/models/create_saved_chart_version_response_200.py
--rw-r--r--   0        0        0      980 2023-05-25 04:23:15.000000 lightdash_client_python-0.1.2/lightdash_client/models/create_saved_chart_version_table_config.py
--rw-r--r--   0        0        0     2213 2023-05-25 04:23:15.000000 lightdash_client_python-0.1.2/lightdash_client/models/create_user.py
--rw-r--r--   0        0        0     2397 2023-05-25 04:23:15.000000 lightdash_client_python-0.1.2/lightdash_client/models/create_user_response_201.py
--rw-r--r--   0        0        0     2295 2023-05-25 04:23:15.000000 lightdash_client_python-0.1.2/lightdash_client/models/dashboard_list_item.py
--rw-r--r--   0        0        0     4364 2023-05-25 04:23:15.000000 lightdash_client_python-0.1.2/lightdash_client/models/dashboard_tile.py
--rw-r--r--   0        0        0     1850 2023-05-25 04:23:15.000000 lightdash_client_python-0.1.2/lightdash_client/models/error.py
--rw-r--r--   0        0        0     2585 2023-05-25 04:23:15.000000 lightdash_client_python-0.1.2/lightdash_client/models/error_error.py
--rw-r--r--   0        0        0     1237 2023-05-25 04:23:15.000000 lightdash_client_python-0.1.2/lightdash_client/models/error_error_data.py
--rw-r--r--   0        0        0      136 2023-05-25 04:23:15.000000 lightdash_client_python-0.1.2/lightdash_client/models/error_status.py
--rw-r--r--   0        0        0     2759 2023-05-25 04:23:15.000000 lightdash_client_python-0.1.2/lightdash_client/models/field.py
--rw-r--r--   0        0        0     3020 2023-05-25 04:23:15.000000 lightdash_client_python-0.1.2/lightdash_client/models/get_available_chart_filters_response_200.py
--rw-r--r--   0        0        0     2732 2023-05-25 04:23:15.000000 lightdash_client_python-0.1.2/lightdash_client/models/get_dashboards_response_200.py
--rw-r--r--   0        0        0     2394 2023-05-25 04:23:15.000000 lightdash_client_python-0.1.2/lightdash_client/models/get_invite_link_response_200.py
--rw-r--r--   0        0        0     2305 2023-05-25 04:23:15.000000 lightdash_client_python-0.1.2/lightdash_client/models/get_job_response_200.py
--rw-r--r--   0        0        0      935 2023-05-25 04:23:15.000000 lightdash_client_python-0.1.2/lightdash_client/models/get_organization_projects_json_body.py
--rw-r--r--   0        0        0     2711 2023-05-25 04:23:15.000000 lightdash_client_python-0.1.2/lightdash_client/models/get_organization_projects_response_200.py
--rw-r--r--   0        0        0     2761 2023-05-25 04:23:15.000000 lightdash_client_python-0.1.2/lightdash_client/models/get_organization_users_response_200.py
--rw-r--r--   0        0        0     2802 2023-05-25 04:23:15.000000 lightdash_client_python-0.1.2/lightdash_client/models/get_personal_access_tokens_response_200.py
--rw-r--r--   0        0        0     2442 2023-05-25 04:23:15.000000 lightdash_client_python-0.1.2/lightdash_client/models/get_project_catalog_response_200.py
--rw-r--r--   0        0        0     2591 2023-05-25 04:23:15.000000 lightdash_client_python-0.1.2/lightdash_client/models/get_project_tables_configuration_response_200.py
--rw-r--r--   0        0        0     2394 2023-05-25 04:23:15.000000 lightdash_client_python-0.1.2/lightdash_client/models/get_saved_chart_response_200.py
--rw-r--r--   0        0        0     2382 2023-05-25 04:23:15.000000 lightdash_client_python-0.1.2/lightdash_client/models/get_user_response_200.py
--rw-r--r--   0        0        0     1993 2023-05-25 04:23:15.000000 lightdash_client_python-0.1.2/lightdash_client/models/invite_link.py
--rw-r--r--   0        0        0     4619 2023-05-25 04:23:15.000000 lightdash_client_python-0.1.2/lightdash_client/models/job.py
--rw-r--r--   0        0        0     1232 2023-05-25 04:23:15.000000 lightdash_client_python-0.1.2/lightdash_client/models/job_job_results.py
--rw-r--r--   0        0        0      203 2023-05-25 04:23:15.000000 lightdash_client_python-0.1.2/lightdash_client/models/job_job_status.py
--rw-r--r--   0        0        0      193 2023-05-25 04:23:15.000000 lightdash_client_python-0.1.2/lightdash_client/models/job_job_type.py
--rw-r--r--   0        0        0     5154 2023-05-25 04:23:15.000000 lightdash_client_python-0.1.2/lightdash_client/models/lightdash_user.py
--rw-r--r--   0        0        0     1318 2023-05-25 04:23:15.000000 lightdash_client_python-0.1.2/lightdash_client/models/lightdash_user_ability_rules_item.py
--rw-r--r--   0        0        0     1585 2023-05-25 04:23:15.000000 lightdash_client_python-0.1.2/lightdash_client/models/login.py
--rw-r--r--   0        0        0     1606 2023-05-25 04:23:15.000000 lightdash_client_python-0.1.2/lightdash_client/models/loom_tile_properties.py
--rw-r--r--   0        0        0     1875 2023-05-25 04:23:15.000000 lightdash_client_python-0.1.2/lightdash_client/models/markdown_tile_properties.py
--rw-r--r--   0        0        0     2201 2023-05-25 04:23:15.000000 lightdash_client_python-0.1.2/lightdash_client/models/organization_user.py
--rw-r--r--   0        0        0     2404 2023-05-25 04:23:15.000000 lightdash_client_python-0.1.2/lightdash_client/models/patch_saved_chart_response_200.py
--rw-r--r--   0        0        0     2699 2023-05-25 04:23:15.000000 lightdash_client_python-0.1.2/lightdash_client/models/patch_saved_charts_response_200.py
--rw-r--r--   0        0        0     3111 2023-05-25 04:23:15.000000 lightdash_client_python-0.1.2/lightdash_client/models/personal_access_token.py
--rw-r--r--   0        0        0     3085 2023-05-25 04:23:15.000000 lightdash_client_python-0.1.2/lightdash_client/models/personal_access_token_with_secret.py
--rw-r--r--   0        0        0     2399 2023-05-25 04:23:15.000000 lightdash_client_python-0.1.2/lightdash_client/models/post_saved_chart_response_200.py
--rw-r--r--   0        0        0     1924 2023-05-25 04:23:15.000000 lightdash_client_python-0.1.2/lightdash_client/models/project.py
--rw-r--r--   0        0        0     1829 2023-05-25 04:23:15.000000 lightdash_client_python-0.1.2/lightdash_client/models/project_catalog.py
--rw-r--r--   0        0        0     1922 2023-05-25 04:23:15.000000 lightdash_client_python-0.1.2/lightdash_client/models/project_catalog_database.py
--rw-r--r--   0        0        0     1997 2023-05-25 04:23:15.000000 lightdash_client_python-0.1.2/lightdash_client/models/project_catalog_database_schema.py
--rw-r--r--   0        0        0     1971 2023-05-25 04:23:15.000000 lightdash_client_python-0.1.2/lightdash_client/models/project_catalog_database_schema_table.py
--rw-r--r--   0        0        0     2030 2023-05-25 04:23:15.000000 lightdash_client_python-0.1.2/lightdash_client/models/project_tables_configuration.py
--rw-r--r--   0        0        0     2159 2023-05-25 04:23:15.000000 lightdash_client_python-0.1.2/lightdash_client/models/project_tables_configuration_table_selection.py
--rw-r--r--   0        0        0      223 2023-05-25 04:23:15.000000 lightdash_client_python-0.1.2/lightdash_client/models/project_tables_configuration_table_selection_type.py
--rw-r--r--   0        0        0     1792 2023-05-25 04:23:15.000000 lightdash_client_python-0.1.2/lightdash_client/models/query_result.py
--rw-r--r--   0        0        0     2175 2023-05-25 04:23:15.000000 lightdash_client_python-0.1.2/lightdash_client/models/query_result_column_id.py
--rw-r--r--   0        0        0     1891 2023-05-25 04:23:15.000000 lightdash_client_python-0.1.2/lightdash_client/models/query_result_column_id_value.py
--rw-r--r--   0        0        0     2484 2023-05-25 04:23:15.000000 lightdash_client_python-0.1.2/lightdash_client/models/run_query_response_200.py
--rw-r--r--   0        0        0     2221 2023-05-25 04:23:15.000000 lightdash_client_python-0.1.2/lightdash_client/models/run_query_response_200_results.py
--rw-r--r--   0        0        0     1465 2023-05-25 04:23:15.000000 lightdash_client_python-0.1.2/lightdash_client/models/run_sql_query_json_body.py
--rw-r--r--   0        0        0     2205 2023-05-25 04:23:15.000000 lightdash_client_python-0.1.2/lightdash_client/models/run_sql_query_response_200.py
--rw-r--r--   0        0        0     5738 2023-05-25 04:23:15.000000 lightdash_client_python-0.1.2/lightdash_client/models/saved_chart.py
--rw-r--r--   0        0        0     1275 2023-05-25 04:23:15.000000 lightdash_client_python-0.1.2/lightdash_client/models/saved_chart_metric_query.py
--rw-r--r--   0        0        0     1565 2023-05-25 04:23:15.000000 lightdash_client_python-0.1.2/lightdash_client/models/saved_chart_pivot_config.py
--rw-r--r--   0        0        0      924 2023-05-25 04:23:15.000000 lightdash_client_python-0.1.2/lightdash_client/models/saved_chart_table_config.py
--rw-r--r--   0        0        0     4025 2023-05-25 04:23:15.000000 lightdash_client_python-0.1.2/lightdash_client/models/step.py
--rw-r--r--   0        0        0     1796 2023-05-25 04:23:15.000000 lightdash_client_python-0.1.2/lightdash_client/models/step_error.py
--rw-r--r--   0        0        0      229 2023-05-25 04:23:15.000000 lightdash_client_python-0.1.2/lightdash_client/models/step_step_status.py
--rw-r--r--   0        0        0     1887 2023-05-25 04:23:15.000000 lightdash_client_python-0.1.2/lightdash_client/models/success.py
--rw-r--r--   0        0        0      132 2023-05-25 04:23:15.000000 lightdash_client_python-0.1.2/lightdash_client/models/success_status.py
--rw-r--r--   0        0        0     1633 2023-05-25 04:23:15.000000 lightdash_client_python-0.1.2/lightdash_client/models/tile_properties_chart.py
--rw-r--r--   0        0        0     1484 2023-05-25 04:23:15.000000 lightdash_client_python-0.1.2/lightdash_client/models/unversioned_fields.py
--rw-r--r--   0        0        0     1727 2023-05-25 04:23:15.000000 lightdash_client_python-0.1.2/lightdash_client/models/update_multiple_saved_chart.py
--rw-r--r--   0        0        0      939 2023-05-25 04:23:15.000000 lightdash_client_python-0.1.2/lightdash_client/models/update_organization_member_json_body.py
--rw-r--r--   0        0        0     2889 2023-05-25 04:23:15.000000 lightdash_client_python-0.1.2/lightdash_client/models/update_organization_member_response_200.py
--rw-r--r--   0        0        0     2606 2023-05-25 04:23:15.000000 lightdash_client_python-0.1.2/lightdash_client/models/update_project_tables_configuration_response_201.py
--rw-r--r--   0        0        0     1470 2023-05-25 04:23:15.000000 lightdash_client_python-0.1.2/lightdash_client/models/update_saved_chart.py
--rw-r--r--   0        0        0     1877 2023-05-25 04:23:15.000000 lightdash_client_python-0.1.2/lightdash_client/models/updated_by_user.py
--rw-r--r--   0        0        0       26 2023-05-25 04:23:15.000000 lightdash_client_python-0.1.2/lightdash_client/py.typed
--rw-r--r--   0        0        0     1101 2023-05-25 04:23:15.000000 lightdash_client_python-0.1.2/lightdash_client/types.py
--rw-r--r--   0        0        0     1580 2023-05-25 04:23:15.000000 lightdash_client_python-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      830 2023-05-25 04:23:15.000000 lightdash_client_python-0.1.2/setup.py
--rw-r--r--   0        0        0      796 2023-05-25 04:23:15.000000 lightdash_client_python-0.1.2/tests/__init__.py
--rw-r--r--   0        0        0      908 2023-05-25 04:23:15.000000 lightdash_client_python-0.1.2/tests/test_dummy.py
--rw-r--r--   0        0        0     5097 1970-01-01 00:00:00.000000 lightdash_client_python-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      804 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/.github/CODEOWNERS
+-rw-r--r--   0        0        0      402 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/.github/workflows/contributors-list.yml
+-rw-r--r--   0        0        0     1849 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/.github/workflows/publish.yml
+-rw-r--r--   0        0        0     2335 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/.github/workflows/test-publish.yml
+-rw-r--r--   0        0        0     1115 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/.github/workflows/test.yml
+-rw-r--r--   0        0        0     3078 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/.gitignore
+-rw-r--r--   0        0        0     1040 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/.openapi-generator-ignore
+-rw-r--r--   0        0        0     6821 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/.openapi-generator/FILES
+-rw-r--r--   0        0        0        6 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/.openapi-generator/VERSION
+-rw-r--r--   0        0        0     1266 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    14088 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/.pylintrc
+-rw-r--r--   0        0        0      150 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/.pypirc
+-rw-r--r--   0        0        0        8 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/.python-version
+-rw-r--r--   0        0        0       32 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/.style.yapf
+-rw-r--r--   0        0        0    11357 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/LICENSE
+-rw-r--r--   0        0        0      717 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/Makefile
+-rw-r--r--   0        0        0     3258 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/README.md
+-rwxr-xr-x   0        0        0     1121 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/dev/clean.sh
+-rw-r--r--   0        0        0     2115 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/dev/generate_clients.sh
+-rw-r--r--   0        0        0      974 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/dev/lint.sh
+-rw-r--r--   0        0        0      211 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/dev/openapi-python-client.yml
+-rwxr-xr-x   0        0        0     1391 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/dev/publish.sh
+-rw-r--r--   0        0        0      152 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/dev/schemas/README.md
+-rw-r--r--   0        0        0   199906 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/dev/schemas/swagger.json
+-rwxr-xr-x   0        0        0     1023 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/dev/setup.sh
+-rwxr-xr-x   0        0        0      958 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/dev/test_python.sh
+-rw-r--r--   0        0        0      201 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/__init__.py
+-rw-r--r--   0        0        0       47 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/api/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/api/charts/__init__.py
+-rw-r--r--   0        0        0     4680 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/api/charts/post_chart_results.py
+-rw-r--r--   0        0        0        0 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/api/content/__init__.py
+-rw-r--r--   0        0        0     4483 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/api/content/get_pinned_items.py
+-rw-r--r--   0        0        0     5511 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/api/content/update_pinned_items_order.py
+-rw-r--r--   0        0        0        0 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/api/exploring/__init__.py
+-rw-r--r--   0        0        0     5017 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/api/exploring/post_run_query.py
+-rw-r--r--   0        0        0     5095 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/api/exploring/post_run_underlying_data_query.py
+-rw-r--r--   0        0        0        0 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/api/exports/__init__.py
+-rw-r--r--   0        0        0     3848 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/api/exports/get_csv_url.py
+-rw-r--r--   0        0        0        0 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/api/integrations/__init__.py
+-rw-r--r--   0        0        0     4403 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/api/integrations/delete_dbt_cloud_integration_settings.py
+-rw-r--r--   0        0        0     2743 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/api/integrations/get_dbt_cloud_integration_settings.py
+-rw-r--r--   0        0        0     4847 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/api/integrations/get_dbt_cloud_metrics.py
+-rw-r--r--   0        0        0     3651 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/api/integrations/get_slack_channels.py
+-rw-r--r--   0        0        0     2734 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/api/integrations/update_dbt_cloud_integration_settings.py
+-rw-r--r--   0        0        0        0 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/api/my_account/__init__.py
+-rw-r--r--   0        0        0     2573 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/api/my_account/create_email_one_time_passcode.py
+-rw-r--r--   0        0        0     3501 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/api/my_account/delete_me.py
+-rw-r--r--   0        0        0     3021 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/api/my_account/get_email_verification_status.py
+-rw-r--r--   0        0        0     4793 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/api/my_account/join_organization.py
+-rw-r--r--   0        0        0     4349 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/api/my_account/list_my_available_organizations.py
+-rw-r--r--   0        0        0        0 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/api/organizations/__init__.py
+-rw-r--r--   0        0        0     4634 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/api/organizations/create_group_in_organization.py
+-rw-r--r--   0        0        0     4256 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/api/organizations/delete_my_organization.py
+-rw-r--r--   0        0        0     4057 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/api/organizations/delete_organization_member.py
+-rw-r--r--   0        0        0     3589 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/api/organizations/get_my_organization.py
+-rw-r--r--   0        0        0     3739 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/api/organizations/list_groups_in_organization.py
+-rw-r--r--   0        0        0     3983 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/api/organizations/list_organization_email_domains.py
+-rw-r--r--   0        0        0     3859 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/api/organizations/list_organization_members.py
+-rw-r--r--   0        0        0        0 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/api/projects/__init__.py
+-rw-r--r--   0        0        0     5756 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/api/projects/get_latest_validation_results.py
+-rw-r--r--   0        0        0     4187 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/api/projects/list_charts_in_project.py
+-rw-r--r--   0        0        0     4187 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/api/projects/list_spaces_in_project.py
+-rw-r--r--   0        0        0     6428 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/api/projects/validate_project.py
+-rw-r--r--   0        0        0        0 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/api/roles_permissions/__init__.py
+-rw-r--r--   0        0        0     2984 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/api/roles_permissions/create_space_in_project.py
+-rw-r--r--   0        0        0     4928 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/api/roles_permissions/get_project_access_list.py
+-rw-r--r--   0        0        0     4648 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/api/roles_permissions/grant_project_access_to_user.py
+-rw-r--r--   0        0        0     4794 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/api/roles_permissions/revoke_project_access_for_user.py
+-rw-r--r--   0        0        0     5026 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/api/roles_permissions/update_project_access_for_user.py
+-rw-r--r--   0        0        0        0 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/api/schedulers/__init__.py
+-rw-r--r--   0        0        0     4176 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/api/schedulers/delete_scheduler.py
+-rw-r--r--   0        0        0     4147 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/api/schedulers/get_scheduled_jobs.py
+-rw-r--r--   0        0        0     2633 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/api/schedulers/get_scheduler.py
+-rw-r--r--   0        0        0     4201 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/api/schedulers/get_scheduler_job_status.py
+-rw-r--r--   0        0        0     2620 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/api/schedulers/get_scheduler_logs.py
+-rw-r--r--   0        0        0     2919 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/api/schedulers/update_scheduler.py
+-rw-r--r--   0        0        0        0 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/api/share_links/__init__.py
+-rw-r--r--   0        0        0     3960 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/api/share_links/get_share_url.py
+-rw-r--r--   0        0        0        0 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/api/spaces/__init__.py
+-rw-r--r--   0        0        0     4429 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/api/spaces/delete_space.py
+-rw-r--r--   0        0        0     2881 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/api/spaces/get_space.py
+-rw-r--r--   0        0        0        0 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/api/ssh_keypairs/__init__.py
+-rw-r--r--   0        0        0     3542 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/api/ssh_keypairs/create_ssh_key_pair.py
+-rw-r--r--   0        0        0        0 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/api/user_groups/__init__.py
+-rw-r--r--   0        0        0     4365 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/api/user_groups/add_user_to_group.py
+-rw-r--r--   0        0        0     3927 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/api/user_groups/delete_group.py
+-rw-r--r--   0        0        0     3949 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/api/user_groups/get_group.py
+-rw-r--r--   0        0        0     4073 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/api/user_groups/get_group_members.py
+-rw-r--r--   0        0        0     4348 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/api/user_groups/remove_user_from_group.py
+-rw-r--r--   0        0        0     2906 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/client.py
+-rw-r--r--   0        0        0      470 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/errors.py
+-rw-r--r--   0        0        0    15782 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/__init__.py
+-rw-r--r--   0        0        0     4166 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/additional_metric.py
+-rw-r--r--   0        0        0     2422 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/allowed_email_domains.py
+-rw-r--r--   0        0        0     2410 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/api_chart_summary_list_response.py
+-rw-r--r--   0        0        0      152 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/api_chart_summary_list_response_status.py
+-rw-r--r--   0        0        0     2106 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/api_csv_url_response.py
+-rw-r--r--   0        0        0     1652 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/api_csv_url_response_results.py
+-rw-r--r--   0        0        0      142 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/api_csv_url_response_status.py
+-rw-r--r--   0        0        0     2254 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/api_dbt_cloud_metrics.py
+-rw-r--r--   0        0        0      143 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/api_dbt_cloud_metrics_status.py
+-rw-r--r--   0        0        0     2119 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/api_dbt_cloud_settings_delete_success.py
+-rw-r--r--   0        0        0      157 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/api_dbt_cloud_settings_delete_success_status.py
+-rw-r--r--   0        0        0      147 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/api_email_status_response_status.py
+-rw-r--r--   0        0        0     2139 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/api_error_payload.py
+-rw-r--r--   0        0        0     2386 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/api_error_payload_error.py
+-rw-r--r--   0        0        0      146 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/api_error_payload_status.py
+-rw-r--r--   0        0        0     2285 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/api_group_list_response.py
+-rw-r--r--   0        0        0      145 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/api_group_list_response_status.py
+-rw-r--r--   0        0        0     2359 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/api_group_members_response.py
+-rw-r--r--   0        0        0      148 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/api_group_members_response_status.py
+-rw-r--r--   0        0        0     1951 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/api_group_response.py
+-rw-r--r--   0        0        0      141 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/api_group_response_status.py
+-rw-r--r--   0        0        0     2208 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/api_job_scheduled_response.py
+-rw-r--r--   0        0        0     1548 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/api_job_scheduled_response_results.py
+-rw-r--r--   0        0        0      148 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/api_job_scheduled_response_status.py
+-rw-r--r--   0        0        0     2157 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/api_job_status_response.py
+-rw-r--r--   0        0        0     1535 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/api_job_status_response_results.py
+-rw-r--r--   0        0        0      145 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/api_job_status_response_status.py
+-rw-r--r--   0        0        0     2019 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/api_organization.py
+-rw-r--r--   0        0        0     2241 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/api_organization_allowed_email_domains.py
+-rw-r--r--   0        0        0      159 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/api_organization_allowed_email_domains_status.py
+-rw-r--r--   0        0        0     2270 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/api_organization_member_profile.py
+-rw-r--r--   0        0        0      153 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/api_organization_member_profile_status.py
+-rw-r--r--   0        0        0     2519 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/api_organization_member_profiles.py
+-rw-r--r--   0        0        0      154 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/api_organization_member_profiles_status.py
+-rw-r--r--   0        0        0      140 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/api_organization_status.py
+-rw-r--r--   0        0        0     4825 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/api_pinned_items.py
+-rw-r--r--   0        0        0      139 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/api_pinned_items_status.py
+-rw-r--r--   0        0        0     2478 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/api_project_access_list_response.py
+-rw-r--r--   0        0        0      153 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/api_project_access_list_response_status.py
+-rw-r--r--   0        0        0     2140 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/api_run_query_response.py
+-rw-r--r--   0        0        0     2051 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/api_run_query_response_results.py
+-rw-r--r--   0        0        0      144 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/api_run_query_response_status.py
+-rw-r--r--   0        0        0     2383 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/api_scheduled_jobs_response.py
+-rw-r--r--   0        0        0      149 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/api_scheduled_jobs_response_status.py
+-rw-r--r--   0        0        0      155 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/api_scheduler_and_targets_response_status.py
+-rw-r--r--   0        0        0      149 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/api_scheduler_logs_response_status.py
+-rw-r--r--   0        0        0     2129 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/api_share_response.py
+-rw-r--r--   0        0        0      141 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/api_share_response_status.py
+-rw-r--r--   0        0        0     2376 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/api_slack_channels_response.py
+-rw-r--r--   0        0        0      149 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/api_slack_channels_response_status.py
+-rw-r--r--   0        0        0      141 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/api_space_response_status.py
+-rw-r--r--   0        0        0     2410 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/api_space_summary_list_response.py
+-rw-r--r--   0        0        0      152 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/api_space_summary_list_response_status.py
+-rw-r--r--   0        0        0     2208 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/api_ssh_key_pair_response.py
+-rw-r--r--   0        0        0      146 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/api_ssh_key_pair_response_status.py
+-rw-r--r--   0        0        0     1937 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/api_success_empty.py
+-rw-r--r--   0        0        0      140 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/api_success_empty_status.py
+-rw-r--r--   0        0        0     2569 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/api_user_allowed_organizations_response.py
+-rw-r--r--   0        0        0      160 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/api_user_allowed_organizations_response_status.py
+-rw-r--r--   0        0        0     4732 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/api_validate_response.py
+-rw-r--r--   0        0        0      144 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/api_validate_response_status.py
+-rw-r--r--   0        0        0     1737 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/api_validation_dismiss_response.py
+-rw-r--r--   0        0        0      153 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/api_validation_dismiss_response_status.py
+-rw-r--r--   0        0        0      316 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/chart_kind.py
+-rw-r--r--   0        0        0     3776 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/chart_summary.py
+-rw-r--r--   0        0        0      192 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/chart_type.py
+-rw-r--r--   0        0        0      220 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/compact.py
+-rw-r--r--   0        0        0      272 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/compact_or_alias_type_1.py
+-rw-r--r--   0        0        0     1937 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/create_project_member.py
+-rw-r--r--   0        0        0     2646 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/create_space.py
+-rw-r--r--   0        0        0     2229 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/dbt_cloud_metadata_response_metrics.py
+-rw-r--r--   0        0        0     2494 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/dbt_cloud_metric.py
+-rw-r--r--   0        0        0     2051 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/delete_scheduler_response_201.py
+-rw-r--r--   0        0        0      151 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/delete_scheduler_response_201_status.py
+-rw-r--r--   0        0        0     2003 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/email_one_time_password.py
+-rw-r--r--   0        0        0     2749 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/email_one_time_password_expiring.py
+-rw-r--r--   0        0        0     2458 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/email_status.py
+-rw-r--r--   0        0        0     1664 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/filter_group_response_type_0.py
+-rw-r--r--   0        0        0     1674 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/filter_group_response_type_1.py
+-rw-r--r--   0        0        0     4615 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/filters.py
+-rw-r--r--   0        0        0     2247 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/group.py
+-rw-r--r--   0        0        0     2163 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/group_member.py
+-rw-r--r--   0        0        0     4963 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/metric_query_response.py
+-rw-r--r--   0        0        0      383 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/metric_type.py
+-rw-r--r--   0        0        0     2812 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/organization.py
+-rw-r--r--   0        0        0     3539 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/organization_member_profile.py
+-rw-r--r--   0        0        0      287 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/organization_member_role.py
+-rw-r--r--   0        0        0     2377 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/partial_omit_organization_organization_uuid_or_needs_project.py
+-rw-r--r--   0        0        0     2120 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/partial_pick_organization_member_profile_role.py
+-rw-r--r--   0        0        0     2628 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/partial_pick_space_is_private_or_access.py
+-rw-r--r--   0        0        0     2493 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/pick_allowed_email_domains_exclude_keyof_allowed_email_domains_organization_uuid.py
+-rw-r--r--   0        0        0     1841 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/pick_create_dbt_cloud_integration_metrics_job_id.py
+-rw-r--r--   0        0        0     1565 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/pick_create_group_name.py
+-rw-r--r--   0        0        0     6625 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/pick_dashboard_uuid_or_name_or_description_or_updated_at_or_project_uuid_or_updated_by_user_or_organization_uuid_or_space_uuid_or_views_or_first_viewed_at_or_pinned_list_uuid_or_pinned_list_order.py
+-rw-r--r--   0        0        0     1532 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/pick_group_name.py
+-rw-r--r--   0        0        0     1566 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/pick_organization_name.py
+-rw-r--r--   0        0        0     2016 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/pick_resource_view_item_at_data_uuid_or_pinned_list_order.py
+-rw-r--r--   0        0        0     3781 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/pick_saved_chart_uuid_or_name_or_description_or_space_name_or_space_uuid_or_project_uuid_or_organization_uuid_or_pinned_list_uuid.py
+-rw-r--r--   0        0        0     4585 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/pick_saved_chart_uuid_or_name_or_updated_at_or_updated_by_user_or_description_or_space_uuid_or_pinned_list_uuid_or_pinned_list_order.py
+-rw-r--r--   0        0        0     1757 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/pick_share_url_path_or_params.py
+-rw-r--r--   0        0        0     1502 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/pick_space_name.py
+-rw-r--r--   0        0        0     1768 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/pick_space_name_or_is_private.py
+-rw-r--r--   0        0        0     2609 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/pick_space_organization_uuid_or_project_uuid_or_uuid_or_name_or_is_private.py
+-rw-r--r--   0        0        0     3420 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/pick_space_project_uuid_or_uuid_or_name_or_is_private_or_pinned_list_uuid_or_pinned_list_order_or_organization_uuid.py
+-rw-r--r--   0        0        0     1601 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/pick_space_share_user_uuid.py
+-rw-r--r--   0        0        0     1619 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/pick_ssh_key_pair_public_key.py
+-rw-r--r--   0        0        0     3860 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/pick_validation_response_base_exclude_keyof_validation_response_base_name.py
+-rw-r--r--   0        0        0     2266 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/pick_validation_response_error_or_created_at_or_validation_id.py
+-rw-r--r--   0        0        0     2095 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/post_chart_results_json_body.py
+-rw-r--r--   0        0        0     2540 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/project_member_profile.py
+-rw-r--r--   0        0        0      260 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/project_member_role.py
+-rw-r--r--   0        0        0     1294 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/record_string_any.py
+-rw-r--r--   0        0        0      193 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/resource_view_item_type.py
+-rw-r--r--   0        0        0      150 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/resource_view_item_type_chart.py
+-rw-r--r--   0        0        0      162 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/resource_view_item_type_dashboard.py
+-rw-r--r--   0        0        0      150 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/resource_view_item_type_space.py
+-rw-r--r--   0        0        0     2093 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/resource_view_space_item.py
+-rw-r--r--   0        0        0     3903 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/resource_view_space_item_data.py
+-rw-r--r--   0        0        0     5334 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/run_query_request.py
+-rw-r--r--   0        0        0     1933 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/run_query_request_filters.py
+-rw-r--r--   0        0        0     1661 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/scheduled_jobs.py
+-rw-r--r--   0        0        0     4958 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/scheduler_base.py
+-rw-r--r--   0        0        0     2484 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/scheduler_csv_options.py
+-rw-r--r--   0        0        0      170 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/scheduler_csv_options_limit_type_1.py
+-rw-r--r--   0        0        0     2685 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/scheduler_email_target.py
+-rw-r--r--   0        0        0      156 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/scheduler_format.py
+-rw-r--r--   0        0        0     1272 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/scheduler_image_options.py
+-rw-r--r--   0        0        0      223 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/scheduler_job_status.py
+-rw-r--r--   0        0        0     5049 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/scheduler_log.py
+-rw-r--r--   0        0        0      167 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/scheduler_log_target_type.py
+-rw-r--r--   0        0        0      443 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/scheduler_log_task.py
+-rw-r--r--   0        0        0     2665 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/scheduler_slack_target.py
+-rw-r--r--   0        0        0     3505 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/share_url.py
+-rw-r--r--   0        0        0     1553 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/slack_channel.py
+-rw-r--r--   0        0        0     1658 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/sort_field.py
+-rw-r--r--   0        0        0     2115 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/space_share.py
+-rw-r--r--   0        0        0     2480 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/space_summary.py
+-rw-r--r--   0        0        0     2119 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/table_calculation.py
+-rw-r--r--   0        0        0     2350 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/update_pinned_item_order.py
+-rw-r--r--   0        0        0     1582 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/update_project_member.py
+-rw-r--r--   0        0        0     1173 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/updated_by_user.py
+-rw-r--r--   0        0        0     1993 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/user_allowed_organization.py
+-rw-r--r--   0        0        0     1964 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/validate_project_json_body.py
+-rw-r--r--   0        0        0     6205 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/validation_error_chart_response.py
+-rw-r--r--   0        0        0     5966 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/validation_error_dashboard_response.py
+-rw-r--r--   0        0        0      260 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/validation_error_type.py
+-rw-r--r--   0        0        0     3709 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/validation_response_base.py
+-rw-r--r--   0        0        0      193 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/validation_source_type.py
+-rw-r--r--   0        0        0     2633 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/view_statistics.py
+-rw-r--r--   0        0        0       26 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/py.typed
+-rw-r--r--   0        0        0     1101 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/types.py
+-rw-r--r--   0        0        0     1624 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/pyproject.toml
+-rw-r--r--   0        0        0      830 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/setup.py
+-rw-r--r--   0        0        0      796 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/tests/__init__.py
+-rw-r--r--   0        0        0      908 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/tests/test_dummy.py
+-rw-r--r--   0        0        0     5168 1970-01-01 00:00:00.000000 lightdash_client_python-0.611.0/PKG-INFO
```

### Comparing `lightdash_client_python-0.1.2/.github/CODEOWNERS` & `lightdash_client_python-0.611.0/.github/CODEOWNERS`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.1.2/.github/workflows/publish.yml` & `lightdash_client_python-0.611.0/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.1.2/.github/workflows/test-publish.yml` & `lightdash_client_python-0.611.0/.github/workflows/test-publish.yml`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.1.2/.github/workflows/test.yml` & `lightdash_client_python-0.611.0/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.1.2/.gitignore` & `lightdash_client_python-0.611.0/.gitignore`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.1.2/.openapi-generator-ignore` & `lightdash_client_python-0.611.0/.openapi-generator-ignore`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.1.2/.openapi-generator/FILES` & `lightdash_client_python-0.611.0/.openapi-generator/FILES`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.1.2/.pre-commit-config.yaml` & `lightdash_client_python-0.611.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.1.2/.pylintrc` & `lightdash_client_python-0.611.0/.pylintrc`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.1.2/LICENSE` & `lightdash_client_python-0.611.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.1.2/README.md` & `lightdash_client_python-0.611.0/README.md`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.1.2/dev/clean.sh` & `lightdash_client_python-0.611.0/dev/clean.sh`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.1.2/dev/generate_clients.sh` & `lightdash_client_python-0.611.0/dev/generate_clients.sh`

 * *Files 5% similar despite different names*

```diff
@@ -18,39 +18,43 @@
 #
 
 # Constants
 SCRIPT_DIR="$(dirname "$(readlink -f "$0")")"
 PROJECT_DIR="$(dirname "$SCRIPT_DIR")"
 
 # Arguments
-schema_json="${PROJECT_DIR}/dev/schemas/lightdash-api.json"
+schema_json="${PROJECT_DIR}/dev/schemas/swagger.json"
 config_yaml="${PROJECT_DIR}/dev/openapi-python-client.yml"
 output_dir="${PROJECT_DIR}"
 meta="setup"
+skip_validate_spec=1
 while (($# > 0)); do
   if [[ "$1" == "--schema-json" ]]; then
     schema_json="${2:?}"
     shift 2
   elif [[ "$1" == "--output" ]]; then
     output_dir="${2:?}"
     shift 2
   elif [[ "$1" == "--config" ]]; then
     config_yaml="${2:?}"
     shift 2
   elif [[ "$1" == "--meta" ]]; then
     meta="${2:?}"
     shift 2
+  elif [[ "$1" == "--skip-validate-spec" ]]; then
+    skip_validate_spec="${2:?}"
+    shift 2
   else
     echo "ERROR: Unrecognized argument ${1}" >&2
     exit 1
   fi
 done
 
 options=()
-if [[ "${skip_validate_spec}" == "1" ]]; then
+if [[ "${skip_validate_spec:?}" == "1" ]]; then
   options+=("--skip-validate-spec")
 fi
 
 # Generate the client in the temporary directory.
 temp_dir="$(mktemp -d -t openapi-python-client-XXXXXXXXXX)"
 cd "${temp_dir:?}" || exit 1
 openapi-python-client generate \
```

### Comparing `lightdash_client_python-0.1.2/dev/lint.sh` & `lightdash_client_python-0.611.0/dev/lint.sh`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.1.2/dev/publish.sh` & `lightdash_client_python-0.611.0/dev/publish.sh`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.1.2/dev/setup.sh` & `lightdash_client_python-0.611.0/dev/setup.sh`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.1.2/dev/test_python.sh` & `lightdash_client_python-0.611.0/dev/test_python.sh`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.1.2/lightdash_client/api/dashboard/delete_dashboard.py` & `lightdash_client_python-0.611.0/lightdash_client/api/roles_permissions/create_space_in_project.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,40 +3,43 @@
 from typing import Dict
 from typing import Optional
 
 import httpx
 
 from ... import errors
 from ...client import Client
+from ...models.create_space import CreateSpace
 from ...types import Response
 
 
 def _get_kwargs(
-    dashboard_uuid: str,
+    project_uuid: str,
     *,
     client: Client,
+    json_body: CreateSpace,
 ) -> Dict[str, Any]:
-    url = "{}/dashboards/{dashboardUuid}".format(client.base_url, dashboardUuid=dashboard_uuid)
+    url = "{}/api/v1/projects/{projectUuid}/spaces".format(client.base_url, projectUuid=project_uuid)
 
     headers: Dict[str, str] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
+    json_json_body = json_body.to_dict()
+
     return {
-        "method": "delete",
+        "method": "post",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
         "follow_redirects": client.follow_redirects,
+        "json": json_json_body,
     }
 
 
 def _parse_response(*, client: Client, response: httpx.Response) -> Optional[Any]:
-    if response.status_code == HTTPStatus.OK:
-        return None
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
 def _build_response(*, client: Client, response: httpx.Response) -> Response[Any]:
@@ -45,68 +48,70 @@
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
-    dashboard_uuid: str,
+    project_uuid: str,
     *,
     client: Client,
+    json_body: CreateSpace,
 ) -> Response[Any]:
-    """Delete dashboard
-
-     Delete a single dashboard by dashboard_id
+    """Create a new space inside a project
 
     Args:
-        dashboard_uuid (str):
+        project_uuid (str):
+        json_body (CreateSpace):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Response[Any]
     """
 
     kwargs = _get_kwargs(
-        dashboard_uuid=dashboard_uuid,
+        project_uuid=project_uuid,
         client=client,
+        json_body=json_body,
     )
 
     response = httpx.request(
         verify=client.verify_ssl,
         **kwargs,
     )
 
     return _build_response(client=client, response=response)
 
 
 async def asyncio_detailed(
-    dashboard_uuid: str,
+    project_uuid: str,
     *,
     client: Client,
+    json_body: CreateSpace,
 ) -> Response[Any]:
-    """Delete dashboard
-
-     Delete a single dashboard by dashboard_id
+    """Create a new space inside a project
 
     Args:
-        dashboard_uuid (str):
+        project_uuid (str):
+        json_body (CreateSpace):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Response[Any]
     """
 
     kwargs = _get_kwargs(
-        dashboard_uuid=dashboard_uuid,
+        project_uuid=project_uuid,
         client=client,
+        json_body=json_body,
     )
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
         response = await _client.request(**kwargs)
 
     return _build_response(client=client, response=response)
```

### Comparing `lightdash_client_python-0.1.2/lightdash_client/api/dashboard/get_dashboard.py` & `lightdash_client_python-0.611.0/lightdash_client/api/my_account/create_email_one_time_passcode.py`

 * *Files 13% similar despite different names*

```diff
@@ -7,25 +7,24 @@
 
 from ... import errors
 from ...client import Client
 from ...types import Response
 
 
 def _get_kwargs(
-    dashboard_uuid: str,
     *,
     client: Client,
 ) -> Dict[str, Any]:
-    url = "{}/dashboards/{dashboardUuid}".format(client.base_url, dashboardUuid=dashboard_uuid)
+    url = "{}/api/v1/user/me/email/otp".format(client.base_url)
 
     headers: Dict[str, str] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     return {
-        "method": "get",
+        "method": "put",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
         "follow_redirects": client.follow_redirects,
     }
 
@@ -43,68 +42,56 @@
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
-    dashboard_uuid: str,
     *,
     client: Client,
 ) -> Response[Any]:
-    """Get dashboard
-
-     Get details for a single dashboard by dashboard_id
-
-    Args:
-        dashboard_uuid (str):
+    """Create a new one-time passcode for the current user's primary email.
+    The user will receive an email with the passcode.
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Response[Any]
     """
 
     kwargs = _get_kwargs(
-        dashboard_uuid=dashboard_uuid,
         client=client,
     )
 
     response = httpx.request(
         verify=client.verify_ssl,
         **kwargs,
     )
 
     return _build_response(client=client, response=response)
 
 
 async def asyncio_detailed(
-    dashboard_uuid: str,
     *,
     client: Client,
 ) -> Response[Any]:
-    """Get dashboard
-
-     Get details for a single dashboard by dashboard_id
-
-    Args:
-        dashboard_uuid (str):
+    """Create a new one-time passcode for the current user's primary email.
+    The user will receive an email with the passcode.
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Response[Any]
     """
 
     kwargs = _get_kwargs(
-        dashboard_uuid=dashboard_uuid,
         client=client,
     )
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
         response = await _client.request(**kwargs)
 
     return _build_response(client=client, response=response)
```

### Comparing `lightdash_client_python-0.1.2/lightdash_client/api/dashboard/get_dashboards.py` & `lightdash_client_python-0.611.0/lightdash_client/api/roles_permissions/update_project_access_for_user.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,191 +1,193 @@
 from http import HTTPStatus
 from typing import Any
 from typing import Dict
 from typing import Optional
-from typing import Union
 
 import httpx
 
 from ... import errors
 from ...client import Client
-from ...models.get_dashboards_response_200 import GetDashboardsResponse200
+from ...models.api_success_empty import ApiSuccessEmpty
+from ...models.update_project_member import UpdateProjectMember
 from ...types import Response
-from ...types import UNSET
-from ...types import Unset
 
 
 def _get_kwargs(
     project_uuid: str,
+    user_uuid: str,
     *,
     client: Client,
-    chart_uuid: Union[Unset, None, str] = UNSET,
+    json_body: UpdateProjectMember,
 ) -> Dict[str, Any]:
-    url = "{}/projects/{projectUuid}/dashboards".format(client.base_url, projectUuid=project_uuid)
+    url = "{}/api/v1/projects/{projectUuid}/access/{userUuid}".format(
+        client.base_url, projectUuid=project_uuid, userUuid=user_uuid
+    )
 
     headers: Dict[str, str] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
-    params: Dict[str, Any] = {}
-    params["chartUuid"] = chart_uuid
-
-    params = {k: v for k, v in params.items() if v is not UNSET and v is not None}
+    json_json_body = json_body.to_dict()
 
     return {
-        "method": "get",
+        "method": "patch",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
         "follow_redirects": client.follow_redirects,
-        "params": params,
+        "json": json_json_body,
     }
 
 
-def _parse_response(*, client: Client, response: httpx.Response) -> Optional[GetDashboardsResponse200]:
+def _parse_response(*, client: Client, response: httpx.Response) -> Optional[ApiSuccessEmpty]:
     if response.status_code == HTTPStatus.OK:
-        response_200 = GetDashboardsResponse200.from_dict(response.json())
+        response_200 = ApiSuccessEmpty.from_dict(response.json())
 
         return response_200
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
-def _build_response(*, client: Client, response: httpx.Response) -> Response[GetDashboardsResponse200]:
+def _build_response(*, client: Client, response: httpx.Response) -> Response[ApiSuccessEmpty]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
     project_uuid: str,
+    user_uuid: str,
     *,
     client: Client,
-    chart_uuid: Union[Unset, None, str] = UNSET,
-) -> Response[GetDashboardsResponse200]:
-    """List dashboards
-
-     List all dashboards in a project
+    json_body: UpdateProjectMember,
+) -> Response[ApiSuccessEmpty]:
+    """Update a user's access to a project
 
     Args:
         project_uuid (str):
-        chart_uuid (Union[Unset, None, str]):
+        user_uuid (str):
+        json_body (UpdateProjectMember):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[GetDashboardsResponse200]
+        Response[ApiSuccessEmpty]
     """
 
     kwargs = _get_kwargs(
         project_uuid=project_uuid,
+        user_uuid=user_uuid,
         client=client,
-        chart_uuid=chart_uuid,
+        json_body=json_body,
     )
 
     response = httpx.request(
         verify=client.verify_ssl,
         **kwargs,
     )
 
     return _build_response(client=client, response=response)
 
 
 def sync(
     project_uuid: str,
+    user_uuid: str,
     *,
     client: Client,
-    chart_uuid: Union[Unset, None, str] = UNSET,
-) -> Optional[GetDashboardsResponse200]:
-    """List dashboards
-
-     List all dashboards in a project
+    json_body: UpdateProjectMember,
+) -> Optional[ApiSuccessEmpty]:
+    """Update a user's access to a project
 
     Args:
         project_uuid (str):
-        chart_uuid (Union[Unset, None, str]):
+        user_uuid (str):
+        json_body (UpdateProjectMember):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        GetDashboardsResponse200
+        ApiSuccessEmpty
     """
 
     return sync_detailed(
         project_uuid=project_uuid,
+        user_uuid=user_uuid,
         client=client,
-        chart_uuid=chart_uuid,
+        json_body=json_body,
     ).parsed
 
 
 async def asyncio_detailed(
     project_uuid: str,
+    user_uuid: str,
     *,
     client: Client,
-    chart_uuid: Union[Unset, None, str] = UNSET,
-) -> Response[GetDashboardsResponse200]:
-    """List dashboards
-
-     List all dashboards in a project
+    json_body: UpdateProjectMember,
+) -> Response[ApiSuccessEmpty]:
+    """Update a user's access to a project
 
     Args:
         project_uuid (str):
-        chart_uuid (Union[Unset, None, str]):
+        user_uuid (str):
+        json_body (UpdateProjectMember):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[GetDashboardsResponse200]
+        Response[ApiSuccessEmpty]
     """
 
     kwargs = _get_kwargs(
         project_uuid=project_uuid,
+        user_uuid=user_uuid,
         client=client,
-        chart_uuid=chart_uuid,
+        json_body=json_body,
     )
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
         response = await _client.request(**kwargs)
 
     return _build_response(client=client, response=response)
 
 
 async def asyncio(
     project_uuid: str,
+    user_uuid: str,
     *,
     client: Client,
-    chart_uuid: Union[Unset, None, str] = UNSET,
-) -> Optional[GetDashboardsResponse200]:
-    """List dashboards
-
-     List all dashboards in a project
+    json_body: UpdateProjectMember,
+) -> Optional[ApiSuccessEmpty]:
+    """Update a user's access to a project
 
     Args:
         project_uuid (str):
-        chart_uuid (Union[Unset, None, str]):
+        user_uuid (str):
+        json_body (UpdateProjectMember):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        GetDashboardsResponse200
+        ApiSuccessEmpty
     """
 
     return (
         await asyncio_detailed(
             project_uuid=project_uuid,
+            user_uuid=user_uuid,
             client=client,
-            chart_uuid=chart_uuid,
+            json_body=json_body,
         )
     ).parsed
```

### Comparing `lightdash_client_python-0.1.2/lightdash_client/api/dashboard/patch_dashboard.py` & `lightdash_client_python-0.611.0/lightdash_client/api/schedulers/get_scheduled_jobs.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,133 +1,161 @@
 from http import HTTPStatus
 from typing import Any
 from typing import Dict
 from typing import Optional
-from typing import Union
 
 import httpx
 
 from ... import errors
 from ...client import Client
-from ...models.all_fields import AllFields
-from ...models.unversioned_fields import UnversionedFields
-from ...models.versioned_fields import VersionedFields
+from ...models.api_scheduled_jobs_response import ApiScheduledJobsResponse
 from ...types import Response
 
 
 def _get_kwargs(
-    dashboard_uuid: str,
+    scheduler_uuid: str,
     *,
     client: Client,
-    json_body: Union["AllFields", "UnversionedFields", "VersionedFields"],
 ) -> Dict[str, Any]:
-    url = "{}/dashboards/{dashboardUuid}".format(client.base_url, dashboardUuid=dashboard_uuid)
+    url = "{}/api/v1/schedulers/{schedulerUuid}/jobs".format(client.base_url, schedulerUuid=scheduler_uuid)
 
     headers: Dict[str, str] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
-    json_json_body: Dict[str, Any]
-
-    if isinstance(json_body, UnversionedFields):
-        json_json_body = json_body.to_dict()
-
-    elif isinstance(json_body, VersionedFields):
-        json_json_body = json_body.to_dict()
-
-    else:
-        json_json_body = json_body.to_dict()
-
     return {
-        "method": "patch",
+        "method": "get",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
         "follow_redirects": client.follow_redirects,
-        "json": json_json_body,
     }
 
 
-def _parse_response(*, client: Client, response: httpx.Response) -> Optional[Any]:
+def _parse_response(*, client: Client, response: httpx.Response) -> Optional[ApiScheduledJobsResponse]:
+    if response.status_code == HTTPStatus.OK:
+        response_200 = ApiScheduledJobsResponse.from_dict(response.json())
+
+        return response_200
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
-def _build_response(*, client: Client, response: httpx.Response) -> Response[Any]:
+def _build_response(*, client: Client, response: httpx.Response) -> Response[ApiScheduledJobsResponse]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
-    dashboard_uuid: str,
+    scheduler_uuid: str,
     *,
     client: Client,
-    json_body: Union["AllFields", "UnversionedFields", "VersionedFields"],
-) -> Response[Any]:
-    """Update dashboard
-
-     Update details for a single dashboard by dashboard_id
+) -> Response[ApiScheduledJobsResponse]:
+    """Get scheduled jobs
 
     Args:
-        dashboard_uuid (str):
-        json_body (Union['AllFields', 'UnversionedFields', 'VersionedFields']):
+        scheduler_uuid (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Any]
+        Response[ApiScheduledJobsResponse]
     """
 
     kwargs = _get_kwargs(
-        dashboard_uuid=dashboard_uuid,
+        scheduler_uuid=scheduler_uuid,
         client=client,
-        json_body=json_body,
     )
 
     response = httpx.request(
         verify=client.verify_ssl,
         **kwargs,
     )
 
     return _build_response(client=client, response=response)
 
 
-async def asyncio_detailed(
-    dashboard_uuid: str,
+def sync(
+    scheduler_uuid: str,
     *,
     client: Client,
-    json_body: Union["AllFields", "UnversionedFields", "VersionedFields"],
-) -> Response[Any]:
-    """Update dashboard
+) -> Optional[ApiScheduledJobsResponse]:
+    """Get scheduled jobs
+
+    Args:
+        scheduler_uuid (str):
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
+    Returns:
+        ApiScheduledJobsResponse
+    """
+
+    return sync_detailed(
+        scheduler_uuid=scheduler_uuid,
+        client=client,
+    ).parsed
 
-     Update details for a single dashboard by dashboard_id
+
+async def asyncio_detailed(
+    scheduler_uuid: str,
+    *,
+    client: Client,
+) -> Response[ApiScheduledJobsResponse]:
+    """Get scheduled jobs
 
     Args:
-        dashboard_uuid (str):
-        json_body (Union['AllFields', 'UnversionedFields', 'VersionedFields']):
+        scheduler_uuid (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Any]
+        Response[ApiScheduledJobsResponse]
     """
 
     kwargs = _get_kwargs(
-        dashboard_uuid=dashboard_uuid,
+        scheduler_uuid=scheduler_uuid,
         client=client,
-        json_body=json_body,
     )
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
         response = await _client.request(**kwargs)
 
     return _build_response(client=client, response=response)
+
+
+async def asyncio(
+    scheduler_uuid: str,
+    *,
+    client: Client,
+) -> Optional[ApiScheduledJobsResponse]:
+    """Get scheduled jobs
+
+    Args:
+        scheduler_uuid (str):
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
+    Returns:
+        ApiScheduledJobsResponse
+    """
+
+    return (
+        await asyncio_detailed(
+            scheduler_uuid=scheduler_uuid,
+            client=client,
+        )
+    ).parsed
```

### Comparing `lightdash_client_python-0.1.2/lightdash_client/api/job/get_job.py` & `lightdash_client_python-0.611.0/lightdash_client/api/share_links/get_share_url.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,159 +3,159 @@
 from typing import Dict
 from typing import Optional
 
 import httpx
 
 from ... import errors
 from ...client import Client
-from ...models.get_job_response_200 import GetJobResponse200
+from ...models.api_share_response import ApiShareResponse
 from ...types import Response
 
 
 def _get_kwargs(
-    job_uuid: str,
+    nano_id: str,
     *,
     client: Client,
 ) -> Dict[str, Any]:
-    url = "{}/jobs/{jobUuid}".format(client.base_url, jobUuid=job_uuid)
+    url = "{}/api/v1/share/{nanoId}".format(client.base_url, nanoId=nano_id)
 
     headers: Dict[str, str] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     return {
         "method": "get",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
         "follow_redirects": client.follow_redirects,
     }
 
 
-def _parse_response(*, client: Client, response: httpx.Response) -> Optional[GetJobResponse200]:
+def _parse_response(*, client: Client, response: httpx.Response) -> Optional[ApiShareResponse]:
     if response.status_code == HTTPStatus.OK:
-        response_200 = GetJobResponse200.from_dict(response.json())
+        response_200 = ApiShareResponse.from_dict(response.json())
 
         return response_200
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
-def _build_response(*, client: Client, response: httpx.Response) -> Response[GetJobResponse200]:
+def _build_response(*, client: Client, response: httpx.Response) -> Response[ApiShareResponse]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
-    job_uuid: str,
+    nano_id: str,
     *,
     client: Client,
-) -> Response[GetJobResponse200]:
-    """List status of a job
+) -> Response[ApiShareResponse]:
+    """Get a share url from a short url id
 
     Args:
-        job_uuid (str):
+        nano_id (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[GetJobResponse200]
+        Response[ApiShareResponse]
     """
 
     kwargs = _get_kwargs(
-        job_uuid=job_uuid,
+        nano_id=nano_id,
         client=client,
     )
 
     response = httpx.request(
         verify=client.verify_ssl,
         **kwargs,
     )
 
     return _build_response(client=client, response=response)
 
 
 def sync(
-    job_uuid: str,
+    nano_id: str,
     *,
     client: Client,
-) -> Optional[GetJobResponse200]:
-    """List status of a job
+) -> Optional[ApiShareResponse]:
+    """Get a share url from a short url id
 
     Args:
-        job_uuid (str):
+        nano_id (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        GetJobResponse200
+        ApiShareResponse
     """
 
     return sync_detailed(
-        job_uuid=job_uuid,
+        nano_id=nano_id,
         client=client,
     ).parsed
 
 
 async def asyncio_detailed(
-    job_uuid: str,
+    nano_id: str,
     *,
     client: Client,
-) -> Response[GetJobResponse200]:
-    """List status of a job
+) -> Response[ApiShareResponse]:
+    """Get a share url from a short url id
 
     Args:
-        job_uuid (str):
+        nano_id (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[GetJobResponse200]
+        Response[ApiShareResponse]
     """
 
     kwargs = _get_kwargs(
-        job_uuid=job_uuid,
+        nano_id=nano_id,
         client=client,
     )
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
         response = await _client.request(**kwargs)
 
     return _build_response(client=client, response=response)
 
 
 async def asyncio(
-    job_uuid: str,
+    nano_id: str,
     *,
     client: Client,
-) -> Optional[GetJobResponse200]:
-    """List status of a job
+) -> Optional[ApiShareResponse]:
+    """Get a share url from a short url id
 
     Args:
-        job_uuid (str):
+        nano_id (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        GetJobResponse200
+        ApiShareResponse
     """
 
     return (
         await asyncio_detailed(
-            job_uuid=job_uuid,
+            nano_id=nano_id,
             client=client,
         )
     ).parsed
```

### Comparing `lightdash_client_python-0.1.2/lightdash_client/api/organization/delete_organization_project.py` & `lightdash_client_python-0.611.0/lightdash_client/api/integrations/update_dbt_cloud_integration_settings.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,32 +11,32 @@
 
 
 def _get_kwargs(
     project_uuid: str,
     *,
     client: Client,
 ) -> Dict[str, Any]:
-    url = "{}/org/projects/{projectUuid}".format(client.base_url, projectUuid=project_uuid)
+    url = "{}/api/v1/projects/{projectUuid}/integrations/dbt-cloud/settings".format(
+        client.base_url, projectUuid=project_uuid
+    )
 
     headers: Dict[str, str] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     return {
-        "method": "delete",
+        "method": "post",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
         "follow_redirects": client.follow_redirects,
     }
 
 
 def _parse_response(*, client: Client, response: httpx.Response) -> Optional[Any]:
-    if response.status_code == HTTPStatus.OK:
-        return None
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
 def _build_response(*, client: Client, response: httpx.Response) -> Response[Any]:
@@ -49,15 +49,15 @@
 
 
 def sync_detailed(
     project_uuid: str,
     *,
     client: Client,
 ) -> Response[Any]:
-    """Delete organization project
+    """Update the dbt Cloud integration settings for a project
 
     Args:
         project_uuid (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
@@ -80,15 +80,15 @@
 
 
 async def asyncio_detailed(
     project_uuid: str,
     *,
     client: Client,
 ) -> Response[Any]:
-    """Delete organization project
+    """Update the dbt Cloud integration settings for a project
 
     Args:
         project_uuid (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
```

### Comparing `lightdash_client_python-0.1.2/lightdash_client/api/organization/delete_organization_user.py` & `lightdash_client_python-0.611.0/lightdash_client/api/integrations/get_dbt_cloud_integration_settings.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,36 +7,36 @@
 
 from ... import errors
 from ...client import Client
 from ...types import Response
 
 
 def _get_kwargs(
-    user_uuid: str,
+    project_uuid: str,
     *,
     client: Client,
 ) -> Dict[str, Any]:
-    url = "{}/org/users/{userUuid}".format(client.base_url, userUuid=user_uuid)
+    url = "{}/api/v1/projects/{projectUuid}/integrations/dbt-cloud/settings".format(
+        client.base_url, projectUuid=project_uuid
+    )
 
     headers: Dict[str, str] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     return {
-        "method": "delete",
+        "method": "get",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
         "follow_redirects": client.follow_redirects,
     }
 
 
 def _parse_response(*, client: Client, response: httpx.Response) -> Optional[Any]:
-    if response.status_code == HTTPStatus.OK:
-        return None
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
 def _build_response(*, client: Client, response: httpx.Response) -> Response[Any]:
@@ -45,64 +45,64 @@
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
-    user_uuid: str,
+    project_uuid: str,
     *,
     client: Client,
 ) -> Response[Any]:
-    """Delete organization user
+    """Get the current dbt Cloud integration settings for a project
 
     Args:
-        user_uuid (str):
+        project_uuid (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Response[Any]
     """
 
     kwargs = _get_kwargs(
-        user_uuid=user_uuid,
+        project_uuid=project_uuid,
         client=client,
     )
 
     response = httpx.request(
         verify=client.verify_ssl,
         **kwargs,
     )
 
     return _build_response(client=client, response=response)
 
 
 async def asyncio_detailed(
-    user_uuid: str,
+    project_uuid: str,
     *,
     client: Client,
 ) -> Response[Any]:
-    """Delete organization user
+    """Get the current dbt Cloud integration settings for a project
 
     Args:
-        user_uuid (str):
+        project_uuid (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Response[Any]
     """
 
     kwargs = _get_kwargs(
-        user_uuid=user_uuid,
+        project_uuid=project_uuid,
         client=client,
     )
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
         response = await _client.request(**kwargs)
 
     return _build_response(client=client, response=response)
```

### Comparing `lightdash_client_python-0.1.2/lightdash_client/api/organization/get_organization_projects.py` & `lightdash_client_python-0.611.0/lightdash_client/api/organizations/create_group_in_organization.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,78 +3,79 @@
 from typing import Dict
 from typing import Optional
 
 import httpx
 
 from ... import errors
 from ...client import Client
-from ...models.get_organization_projects_json_body import GetOrganizationProjectsJsonBody
-from ...models.get_organization_projects_response_200 import GetOrganizationProjectsResponse200
+from ...models.api_group_response import ApiGroupResponse
+from ...models.pick_create_group_name import PickCreateGroupName
 from ...types import Response
 
 
 def _get_kwargs(
     *,
     client: Client,
-    json_body: GetOrganizationProjectsJsonBody,
+    json_body: PickCreateGroupName,
 ) -> Dict[str, Any]:
-    url = "{}/org/projects".format(client.base_url)
+    url = "{}/api/v1/org/groups".format(client.base_url)
 
     headers: Dict[str, str] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     json_json_body = json_body.to_dict()
 
     return {
-        "method": "get",
+        "method": "post",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
         "follow_redirects": client.follow_redirects,
         "json": json_json_body,
     }
 
 
-def _parse_response(*, client: Client, response: httpx.Response) -> Optional[GetOrganizationProjectsResponse200]:
+def _parse_response(*, client: Client, response: httpx.Response) -> Optional[ApiGroupResponse]:
     if response.status_code == HTTPStatus.OK:
-        response_200 = GetOrganizationProjectsResponse200.from_dict(response.json())
+        response_200 = ApiGroupResponse.from_dict(response.json())
 
         return response_200
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
-def _build_response(*, client: Client, response: httpx.Response) -> Response[GetOrganizationProjectsResponse200]:
+def _build_response(*, client: Client, response: httpx.Response) -> Response[ApiGroupResponse]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
     *,
     client: Client,
-    json_body: GetOrganizationProjectsJsonBody,
-) -> Response[GetOrganizationProjectsResponse200]:
-    """List organization projects
+    json_body: PickCreateGroupName,
+) -> Response[ApiGroupResponse]:
+    """Creates a new group in the current user's organization
 
     Args:
-        json_body (GetOrganizationProjectsJsonBody):
+        json_body (PickCreateGroupName): From T, pick a set of properties whose keys are in the
+            union K
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[GetOrganizationProjectsResponse200]
+        Response[ApiGroupResponse]
     """
 
     kwargs = _get_kwargs(
         client=client,
         json_body=json_body,
     )
 
@@ -85,51 +86,53 @@
 
     return _build_response(client=client, response=response)
 
 
 def sync(
     *,
     client: Client,
-    json_body: GetOrganizationProjectsJsonBody,
-) -> Optional[GetOrganizationProjectsResponse200]:
-    """List organization projects
+    json_body: PickCreateGroupName,
+) -> Optional[ApiGroupResponse]:
+    """Creates a new group in the current user's organization
 
     Args:
-        json_body (GetOrganizationProjectsJsonBody):
+        json_body (PickCreateGroupName): From T, pick a set of properties whose keys are in the
+            union K
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        GetOrganizationProjectsResponse200
+        ApiGroupResponse
     """
 
     return sync_detailed(
         client=client,
         json_body=json_body,
     ).parsed
 
 
 async def asyncio_detailed(
     *,
     client: Client,
-    json_body: GetOrganizationProjectsJsonBody,
-) -> Response[GetOrganizationProjectsResponse200]:
-    """List organization projects
+    json_body: PickCreateGroupName,
+) -> Response[ApiGroupResponse]:
+    """Creates a new group in the current user's organization
 
     Args:
-        json_body (GetOrganizationProjectsJsonBody):
+        json_body (PickCreateGroupName): From T, pick a set of properties whose keys are in the
+            union K
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[GetOrganizationProjectsResponse200]
+        Response[ApiGroupResponse]
     """
 
     kwargs = _get_kwargs(
         client=client,
         json_body=json_body,
     )
 
@@ -138,27 +141,28 @@
 
     return _build_response(client=client, response=response)
 
 
 async def asyncio(
     *,
     client: Client,
-    json_body: GetOrganizationProjectsJsonBody,
-) -> Optional[GetOrganizationProjectsResponse200]:
-    """List organization projects
+    json_body: PickCreateGroupName,
+) -> Optional[ApiGroupResponse]:
+    """Creates a new group in the current user's organization
 
     Args:
-        json_body (GetOrganizationProjectsJsonBody):
+        json_body (PickCreateGroupName): From T, pick a set of properties whose keys are in the
+            union K
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        GetOrganizationProjectsResponse200
+        ApiGroupResponse
     """
 
     return (
         await asyncio_detailed(
             client=client,
             json_body=json_body,
         )
```

### Comparing `lightdash_client_python-0.1.2/lightdash_client/api/organization/get_organization_users.py` & `lightdash_client_python-0.611.0/lightdash_client/api/organizations/list_groups_in_organization.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,69 +3,69 @@
 from typing import Dict
 from typing import Optional
 
 import httpx
 
 from ... import errors
 from ...client import Client
-from ...models.get_organization_users_response_200 import GetOrganizationUsersResponse200
+from ...models.api_group_list_response import ApiGroupListResponse
 from ...types import Response
 
 
 def _get_kwargs(
     *,
     client: Client,
 ) -> Dict[str, Any]:
-    url = "{}/org/users".format(client.base_url)
+    url = "{}/api/v1/org/groups".format(client.base_url)
 
     headers: Dict[str, str] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     return {
         "method": "get",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
         "follow_redirects": client.follow_redirects,
     }
 
 
-def _parse_response(*, client: Client, response: httpx.Response) -> Optional[GetOrganizationUsersResponse200]:
+def _parse_response(*, client: Client, response: httpx.Response) -> Optional[ApiGroupListResponse]:
     if response.status_code == HTTPStatus.OK:
-        response_200 = GetOrganizationUsersResponse200.from_dict(response.json())
+        response_200 = ApiGroupListResponse.from_dict(response.json())
 
         return response_200
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
-def _build_response(*, client: Client, response: httpx.Response) -> Response[GetOrganizationUsersResponse200]:
+def _build_response(*, client: Client, response: httpx.Response) -> Response[ApiGroupListResponse]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
     *,
     client: Client,
-) -> Response[GetOrganizationUsersResponse200]:
-    """Get organization users
+) -> Response[ApiGroupListResponse]:
+    """Gets all the groups in the current user's organization
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[GetOrganizationUsersResponse200]
+        Response[ApiGroupListResponse]
     """
 
     kwargs = _get_kwargs(
         client=client,
     )
 
     response = httpx.request(
@@ -75,42 +75,42 @@
 
     return _build_response(client=client, response=response)
 
 
 def sync(
     *,
     client: Client,
-) -> Optional[GetOrganizationUsersResponse200]:
-    """Get organization users
+) -> Optional[ApiGroupListResponse]:
+    """Gets all the groups in the current user's organization
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        GetOrganizationUsersResponse200
+        ApiGroupListResponse
     """
 
     return sync_detailed(
         client=client,
     ).parsed
 
 
 async def asyncio_detailed(
     *,
     client: Client,
-) -> Response[GetOrganizationUsersResponse200]:
-    """Get organization users
+) -> Response[ApiGroupListResponse]:
+    """Gets all the groups in the current user's organization
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[GetOrganizationUsersResponse200]
+        Response[ApiGroupListResponse]
     """
 
     kwargs = _get_kwargs(
         client=client,
     )
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
@@ -118,23 +118,23 @@
 
     return _build_response(client=client, response=response)
 
 
 async def asyncio(
     *,
     client: Client,
-) -> Optional[GetOrganizationUsersResponse200]:
-    """Get organization users
+) -> Optional[ApiGroupListResponse]:
+    """Gets all the groups in the current user's organization
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        GetOrganizationUsersResponse200
+        ApiGroupListResponse
     """
 
     return (
         await asyncio_detailed(
             client=client,
         )
     ).parsed
```

### Comparing `lightdash_client_python-0.1.2/lightdash_client/api/organization/update_organization.py` & `lightdash_client_python-0.611.0/lightdash_client/api/my_account/get_email_verification_status.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,41 +1,49 @@
 from http import HTTPStatus
 from typing import Any
 from typing import Dict
 from typing import Optional
+from typing import Union
 
 import httpx
 
 from ... import errors
 from ...client import Client
 from ...types import Response
+from ...types import UNSET
+from ...types import Unset
 
 
 def _get_kwargs(
     *,
     client: Client,
+    passcode: Union[Unset, None, str] = UNSET,
 ) -> Dict[str, Any]:
-    url = "{}/org".format(client.base_url)
+    url = "{}/api/v1/user/me/email/status".format(client.base_url)
 
     headers: Dict[str, str] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
+    params: Dict[str, Any] = {}
+    params["passcode"] = passcode
+
+    params = {k: v for k, v in params.items() if v is not UNSET and v is not None}
+
     return {
-        "method": "patch",
+        "method": "get",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
         "follow_redirects": client.follow_redirects,
+        "params": params,
     }
 
 
 def _parse_response(*, client: Client, response: httpx.Response) -> Optional[Any]:
-    if response.status_code == HTTPStatus.OK:
-        return None
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
 def _build_response(*, client: Client, response: httpx.Response) -> Response[Any]:
@@ -46,52 +54,62 @@
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
     *,
     client: Client,
+    passcode: Union[Unset, None, str] = UNSET,
 ) -> Response[Any]:
-    """Update organization
+    """Get the verification status for the current user's primary email
+
+    Args:
+        passcode (Union[Unset, None, str]):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Response[Any]
     """
 
     kwargs = _get_kwargs(
         client=client,
+        passcode=passcode,
     )
 
     response = httpx.request(
         verify=client.verify_ssl,
         **kwargs,
     )
 
     return _build_response(client=client, response=response)
 
 
 async def asyncio_detailed(
     *,
     client: Client,
+    passcode: Union[Unset, None, str] = UNSET,
 ) -> Response[Any]:
-    """Update organization
+    """Get the verification status for the current user's primary email
+
+    Args:
+        passcode (Union[Unset, None, str]):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Response[Any]
     """
 
     kwargs = _get_kwargs(
         client=client,
+        passcode=passcode,
     )
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
         response = await _client.request(**kwargs)
 
     return _build_response(client=client, response=response)
```

### Comparing `lightdash_client_python-0.1.2/lightdash_client/api/organization/update_organization_member.py` & `lightdash_client_python-0.611.0/lightdash_client/api/exploring/post_run_query.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,176 +3,191 @@
 from typing import Dict
 from typing import Optional
 
 import httpx
 
 from ... import errors
 from ...client import Client
-from ...models.update_organization_member_json_body import UpdateOrganizationMemberJsonBody
-from ...models.update_organization_member_response_200 import UpdateOrganizationMemberResponse200
+from ...models.api_run_query_response import ApiRunQueryResponse
+from ...models.run_query_request import RunQueryRequest
 from ...types import Response
 
 
 def _get_kwargs(
-    user_uuid: str,
+    project_uuid: str,
+    explore_id: str,
     *,
     client: Client,
-    json_body: UpdateOrganizationMemberJsonBody,
+    json_body: RunQueryRequest,
 ) -> Dict[str, Any]:
-    url = "{}/org/users/{userUuid}".format(client.base_url, userUuid=user_uuid)
+    url = "{}/api/v1/projects/{projectUuid}/explores/{exploreId}/runQuery".format(
+        client.base_url, projectUuid=project_uuid, exploreId=explore_id
+    )
 
     headers: Dict[str, str] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     json_json_body = json_body.to_dict()
 
     return {
-        "method": "patch",
+        "method": "post",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
         "follow_redirects": client.follow_redirects,
         "json": json_json_body,
     }
 
 
-def _parse_response(*, client: Client, response: httpx.Response) -> Optional[UpdateOrganizationMemberResponse200]:
+def _parse_response(*, client: Client, response: httpx.Response) -> Optional[ApiRunQueryResponse]:
     if response.status_code == HTTPStatus.OK:
-        response_200 = UpdateOrganizationMemberResponse200.from_dict(response.json())
+        response_200 = ApiRunQueryResponse.from_dict(response.json())
 
         return response_200
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
-def _build_response(*, client: Client, response: httpx.Response) -> Response[UpdateOrganizationMemberResponse200]:
+def _build_response(*, client: Client, response: httpx.Response) -> Response[ApiRunQueryResponse]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
-    user_uuid: str,
+    project_uuid: str,
+    explore_id: str,
     *,
     client: Client,
-    json_body: UpdateOrganizationMemberJsonBody,
-) -> Response[UpdateOrganizationMemberResponse200]:
-    """Update organization member
+    json_body: RunQueryRequest,
+) -> Response[ApiRunQueryResponse]:
+    """Run a query for explore
 
     Args:
-        user_uuid (str):
-        json_body (UpdateOrganizationMemberJsonBody):
+        project_uuid (str):
+        explore_id (str):
+        json_body (RunQueryRequest):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[UpdateOrganizationMemberResponse200]
+        Response[ApiRunQueryResponse]
     """
 
     kwargs = _get_kwargs(
-        user_uuid=user_uuid,
+        project_uuid=project_uuid,
+        explore_id=explore_id,
         client=client,
         json_body=json_body,
     )
 
     response = httpx.request(
         verify=client.verify_ssl,
         **kwargs,
     )
 
     return _build_response(client=client, response=response)
 
 
 def sync(
-    user_uuid: str,
+    project_uuid: str,
+    explore_id: str,
     *,
     client: Client,
-    json_body: UpdateOrganizationMemberJsonBody,
-) -> Optional[UpdateOrganizationMemberResponse200]:
-    """Update organization member
+    json_body: RunQueryRequest,
+) -> Optional[ApiRunQueryResponse]:
+    """Run a query for explore
 
     Args:
-        user_uuid (str):
-        json_body (UpdateOrganizationMemberJsonBody):
+        project_uuid (str):
+        explore_id (str):
+        json_body (RunQueryRequest):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        UpdateOrganizationMemberResponse200
+        ApiRunQueryResponse
     """
 
     return sync_detailed(
-        user_uuid=user_uuid,
+        project_uuid=project_uuid,
+        explore_id=explore_id,
         client=client,
         json_body=json_body,
     ).parsed
 
 
 async def asyncio_detailed(
-    user_uuid: str,
+    project_uuid: str,
+    explore_id: str,
     *,
     client: Client,
-    json_body: UpdateOrganizationMemberJsonBody,
-) -> Response[UpdateOrganizationMemberResponse200]:
-    """Update organization member
+    json_body: RunQueryRequest,
+) -> Response[ApiRunQueryResponse]:
+    """Run a query for explore
 
     Args:
-        user_uuid (str):
-        json_body (UpdateOrganizationMemberJsonBody):
+        project_uuid (str):
+        explore_id (str):
+        json_body (RunQueryRequest):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[UpdateOrganizationMemberResponse200]
+        Response[ApiRunQueryResponse]
     """
 
     kwargs = _get_kwargs(
-        user_uuid=user_uuid,
+        project_uuid=project_uuid,
+        explore_id=explore_id,
         client=client,
         json_body=json_body,
     )
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
         response = await _client.request(**kwargs)
 
     return _build_response(client=client, response=response)
 
 
 async def asyncio(
-    user_uuid: str,
+    project_uuid: str,
+    explore_id: str,
     *,
     client: Client,
-    json_body: UpdateOrganizationMemberJsonBody,
-) -> Optional[UpdateOrganizationMemberResponse200]:
-    """Update organization member
+    json_body: RunQueryRequest,
+) -> Optional[ApiRunQueryResponse]:
+    """Run a query for explore
 
     Args:
-        user_uuid (str):
-        json_body (UpdateOrganizationMemberJsonBody):
+        project_uuid (str):
+        explore_id (str):
+        json_body (RunQueryRequest):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        UpdateOrganizationMemberResponse200
+        ApiRunQueryResponse
     """
 
     return (
         await asyncio_detailed(
-            user_uuid=user_uuid,
+            project_uuid=project_uuid,
+            explore_id=explore_id,
             client=client,
             json_body=json_body,
         )
     ).parsed
```

### Comparing `lightdash_client_python-0.1.2/lightdash_client/api/project/get_project_catalog.py` & `lightdash_client_python-0.611.0/lightdash_client/api/spaces/delete_space.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,167 +3,174 @@
 from typing import Dict
 from typing import Optional
 
 import httpx
 
 from ... import errors
 from ...client import Client
-from ...models.get_project_catalog_response_200 import GetProjectCatalogResponse200
+from ...models.api_success_empty import ApiSuccessEmpty
 from ...types import Response
 
 
 def _get_kwargs(
     project_uuid: str,
+    space_uuid: str,
     *,
     client: Client,
 ) -> Dict[str, Any]:
-    url = "{}/projects/{projectUuid}/catalog".format(client.base_url, projectUuid=project_uuid)
+    url = "{}/api/v1/projects/{projectUuid}/spaces/{spaceUuid}".format(
+        client.base_url, projectUuid=project_uuid, spaceUuid=space_uuid
+    )
 
     headers: Dict[str, str] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     return {
-        "method": "get",
+        "method": "delete",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
         "follow_redirects": client.follow_redirects,
     }
 
 
-def _parse_response(*, client: Client, response: httpx.Response) -> Optional[GetProjectCatalogResponse200]:
-    if response.status_code == HTTPStatus.OK:
-        response_200 = GetProjectCatalogResponse200.from_dict(response.json())
+def _parse_response(*, client: Client, response: httpx.Response) -> Optional[ApiSuccessEmpty]:
+    if response.status_code == HTTPStatus.NO_CONTENT:
+        response_204 = ApiSuccessEmpty.from_dict(response.json())
 
-        return response_200
+        return response_204
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
-def _build_response(*, client: Client, response: httpx.Response) -> Response[GetProjectCatalogResponse200]:
+def _build_response(*, client: Client, response: httpx.Response) -> Response[ApiSuccessEmpty]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
     project_uuid: str,
+    space_uuid: str,
     *,
     client: Client,
-) -> Response[GetProjectCatalogResponse200]:
-    """Get project catalog
-
-     Get project catalog with all valid tables
+) -> Response[ApiSuccessEmpty]:
+    """Delete a space from a project
 
     Args:
         project_uuid (str):
+        space_uuid (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[GetProjectCatalogResponse200]
+        Response[ApiSuccessEmpty]
     """
 
     kwargs = _get_kwargs(
         project_uuid=project_uuid,
+        space_uuid=space_uuid,
         client=client,
     )
 
     response = httpx.request(
         verify=client.verify_ssl,
         **kwargs,
     )
 
     return _build_response(client=client, response=response)
 
 
 def sync(
     project_uuid: str,
+    space_uuid: str,
     *,
     client: Client,
-) -> Optional[GetProjectCatalogResponse200]:
-    """Get project catalog
-
-     Get project catalog with all valid tables
+) -> Optional[ApiSuccessEmpty]:
+    """Delete a space from a project
 
     Args:
         project_uuid (str):
+        space_uuid (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        GetProjectCatalogResponse200
+        ApiSuccessEmpty
     """
 
     return sync_detailed(
         project_uuid=project_uuid,
+        space_uuid=space_uuid,
         client=client,
     ).parsed
 
 
 async def asyncio_detailed(
     project_uuid: str,
+    space_uuid: str,
     *,
     client: Client,
-) -> Response[GetProjectCatalogResponse200]:
-    """Get project catalog
-
-     Get project catalog with all valid tables
+) -> Response[ApiSuccessEmpty]:
+    """Delete a space from a project
 
     Args:
         project_uuid (str):
+        space_uuid (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[GetProjectCatalogResponse200]
+        Response[ApiSuccessEmpty]
     """
 
     kwargs = _get_kwargs(
         project_uuid=project_uuid,
+        space_uuid=space_uuid,
         client=client,
     )
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
         response = await _client.request(**kwargs)
 
     return _build_response(client=client, response=response)
 
 
 async def asyncio(
     project_uuid: str,
+    space_uuid: str,
     *,
     client: Client,
-) -> Optional[GetProjectCatalogResponse200]:
-    """Get project catalog
-
-     Get project catalog with all valid tables
+) -> Optional[ApiSuccessEmpty]:
+    """Delete a space from a project
 
     Args:
         project_uuid (str):
+        space_uuid (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        GetProjectCatalogResponse200
+        ApiSuccessEmpty
     """
 
     return (
         await asyncio_detailed(
             project_uuid=project_uuid,
+            space_uuid=space_uuid,
             client=client,
         )
     ).parsed
```

### Comparing `lightdash_client_python-0.1.2/lightdash_client/api/project/get_project_tables_configuration.py` & `lightdash_client_python-0.611.0/lightdash_client/api/roles_permissions/revoke_project_access_for_user.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,167 +3,187 @@
 from typing import Dict
 from typing import Optional
 
 import httpx
 
 from ... import errors
 from ...client import Client
-from ...models.get_project_tables_configuration_response_200 import GetProjectTablesConfigurationResponse200
+from ...models.api_success_empty import ApiSuccessEmpty
 from ...types import Response
 
 
 def _get_kwargs(
     project_uuid: str,
+    space_uuid: str,
+    user_uuid: str,
     *,
     client: Client,
 ) -> Dict[str, Any]:
-    url = "{}/projects/{projectUuid}/tablesConfiguration".format(client.base_url, projectUuid=project_uuid)
+    url = "{}/api/v1/projects/{projectUuid}/spaces/{spaceUuid}/share/{userUuid}".format(
+        client.base_url, projectUuid=project_uuid, spaceUuid=space_uuid, userUuid=user_uuid
+    )
 
     headers: Dict[str, str] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     return {
-        "method": "get",
+        "method": "delete",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
         "follow_redirects": client.follow_redirects,
     }
 
 
-def _parse_response(*, client: Client, response: httpx.Response) -> Optional[GetProjectTablesConfigurationResponse200]:
+def _parse_response(*, client: Client, response: httpx.Response) -> Optional[ApiSuccessEmpty]:
     if response.status_code == HTTPStatus.OK:
-        response_200 = GetProjectTablesConfigurationResponse200.from_dict(response.json())
+        response_200 = ApiSuccessEmpty.from_dict(response.json())
 
         return response_200
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
-def _build_response(*, client: Client, response: httpx.Response) -> Response[GetProjectTablesConfigurationResponse200]:
+def _build_response(*, client: Client, response: httpx.Response) -> Response[ApiSuccessEmpty]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
     project_uuid: str,
+    space_uuid: str,
+    user_uuid: str,
     *,
     client: Client,
-) -> Response[GetProjectTablesConfigurationResponse200]:
-    """Get project tables configuration
-
-     Get project tables configuration
+) -> Response[ApiSuccessEmpty]:
+    """Remove a user's access to a space
 
     Args:
         project_uuid (str):
+        space_uuid (str):
+        user_uuid (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[GetProjectTablesConfigurationResponse200]
+        Response[ApiSuccessEmpty]
     """
 
     kwargs = _get_kwargs(
         project_uuid=project_uuid,
+        space_uuid=space_uuid,
+        user_uuid=user_uuid,
         client=client,
     )
 
     response = httpx.request(
         verify=client.verify_ssl,
         **kwargs,
     )
 
     return _build_response(client=client, response=response)
 
 
 def sync(
     project_uuid: str,
+    space_uuid: str,
+    user_uuid: str,
     *,
     client: Client,
-) -> Optional[GetProjectTablesConfigurationResponse200]:
-    """Get project tables configuration
-
-     Get project tables configuration
+) -> Optional[ApiSuccessEmpty]:
+    """Remove a user's access to a space
 
     Args:
         project_uuid (str):
+        space_uuid (str):
+        user_uuid (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        GetProjectTablesConfigurationResponse200
+        ApiSuccessEmpty
     """
 
     return sync_detailed(
         project_uuid=project_uuid,
+        space_uuid=space_uuid,
+        user_uuid=user_uuid,
         client=client,
     ).parsed
 
 
 async def asyncio_detailed(
     project_uuid: str,
+    space_uuid: str,
+    user_uuid: str,
     *,
     client: Client,
-) -> Response[GetProjectTablesConfigurationResponse200]:
-    """Get project tables configuration
-
-     Get project tables configuration
+) -> Response[ApiSuccessEmpty]:
+    """Remove a user's access to a space
 
     Args:
         project_uuid (str):
+        space_uuid (str):
+        user_uuid (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[GetProjectTablesConfigurationResponse200]
+        Response[ApiSuccessEmpty]
     """
 
     kwargs = _get_kwargs(
         project_uuid=project_uuid,
+        space_uuid=space_uuid,
+        user_uuid=user_uuid,
         client=client,
     )
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
         response = await _client.request(**kwargs)
 
     return _build_response(client=client, response=response)
 
 
 async def asyncio(
     project_uuid: str,
+    space_uuid: str,
+    user_uuid: str,
     *,
     client: Client,
-) -> Optional[GetProjectTablesConfigurationResponse200]:
-    """Get project tables configuration
-
-     Get project tables configuration
+) -> Optional[ApiSuccessEmpty]:
+    """Remove a user's access to a space
 
     Args:
         project_uuid (str):
+        space_uuid (str):
+        user_uuid (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        GetProjectTablesConfigurationResponse200
+        ApiSuccessEmpty
     """
 
     return (
         await asyncio_detailed(
             project_uuid=project_uuid,
+            space_uuid=space_uuid,
+            user_uuid=user_uuid,
             client=client,
         )
     ).parsed
```

### Comparing `lightdash_client_python-0.1.2/lightdash_client/api/project/update_project_tables_configuration.py` & `lightdash_client_python-0.611.0/lightdash_client/api/exploring/post_run_underlying_data_query.py`

 * *Files 17% similar despite different names*

```diff
@@ -3,188 +3,191 @@
 from typing import Dict
 from typing import Optional
 
 import httpx
 
 from ... import errors
 from ...client import Client
-from ...models.project_tables_configuration import ProjectTablesConfiguration
-from ...models.update_project_tables_configuration_response_201 import UpdateProjectTablesConfigurationResponse201
+from ...models.api_run_query_response import ApiRunQueryResponse
+from ...models.run_query_request import RunQueryRequest
 from ...types import Response
 
 
 def _get_kwargs(
     project_uuid: str,
+    explore_id: str,
     *,
     client: Client,
-    json_body: ProjectTablesConfiguration,
+    json_body: RunQueryRequest,
 ) -> Dict[str, Any]:
-    url = "{}/projects/{projectUuid}/tablesConfiguration".format(client.base_url, projectUuid=project_uuid)
+    url = "{}/api/v1/projects/{projectUuid}/explores/{exploreId}/runUnderlyingDataQuery".format(
+        client.base_url, projectUuid=project_uuid, exploreId=explore_id
+    )
 
     headers: Dict[str, str] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     json_json_body = json_body.to_dict()
 
     return {
-        "method": "patch",
+        "method": "post",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
         "follow_redirects": client.follow_redirects,
         "json": json_json_body,
     }
 
 
-def _parse_response(
-    *, client: Client, response: httpx.Response
-) -> Optional[UpdateProjectTablesConfigurationResponse201]:
-    if response.status_code == HTTPStatus.CREATED:
-        response_201 = UpdateProjectTablesConfigurationResponse201.from_dict(response.json())
+def _parse_response(*, client: Client, response: httpx.Response) -> Optional[ApiRunQueryResponse]:
+    if response.status_code == HTTPStatus.OK:
+        response_200 = ApiRunQueryResponse.from_dict(response.json())
 
-        return response_201
+        return response_200
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
-def _build_response(
-    *, client: Client, response: httpx.Response
-) -> Response[UpdateProjectTablesConfigurationResponse201]:
+def _build_response(*, client: Client, response: httpx.Response) -> Response[ApiRunQueryResponse]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
     project_uuid: str,
+    explore_id: str,
     *,
     client: Client,
-    json_body: ProjectTablesConfiguration,
-) -> Response[UpdateProjectTablesConfigurationResponse201]:
-    """Update project tables configuration
-
-     Update project tables configuration
+    json_body: RunQueryRequest,
+) -> Response[ApiRunQueryResponse]:
+    """Run a query for underlying data results
 
     Args:
         project_uuid (str):
-        json_body (ProjectTablesConfiguration):
+        explore_id (str):
+        json_body (RunQueryRequest):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[UpdateProjectTablesConfigurationResponse201]
+        Response[ApiRunQueryResponse]
     """
 
     kwargs = _get_kwargs(
         project_uuid=project_uuid,
+        explore_id=explore_id,
         client=client,
         json_body=json_body,
     )
 
     response = httpx.request(
         verify=client.verify_ssl,
         **kwargs,
     )
 
     return _build_response(client=client, response=response)
 
 
 def sync(
     project_uuid: str,
+    explore_id: str,
     *,
     client: Client,
-    json_body: ProjectTablesConfiguration,
-) -> Optional[UpdateProjectTablesConfigurationResponse201]:
-    """Update project tables configuration
-
-     Update project tables configuration
+    json_body: RunQueryRequest,
+) -> Optional[ApiRunQueryResponse]:
+    """Run a query for underlying data results
 
     Args:
         project_uuid (str):
-        json_body (ProjectTablesConfiguration):
+        explore_id (str):
+        json_body (RunQueryRequest):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        UpdateProjectTablesConfigurationResponse201
+        ApiRunQueryResponse
     """
 
     return sync_detailed(
         project_uuid=project_uuid,
+        explore_id=explore_id,
         client=client,
         json_body=json_body,
     ).parsed
 
 
 async def asyncio_detailed(
     project_uuid: str,
+    explore_id: str,
     *,
     client: Client,
-    json_body: ProjectTablesConfiguration,
-) -> Response[UpdateProjectTablesConfigurationResponse201]:
-    """Update project tables configuration
-
-     Update project tables configuration
+    json_body: RunQueryRequest,
+) -> Response[ApiRunQueryResponse]:
+    """Run a query for underlying data results
 
     Args:
         project_uuid (str):
-        json_body (ProjectTablesConfiguration):
+        explore_id (str):
+        json_body (RunQueryRequest):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[UpdateProjectTablesConfigurationResponse201]
+        Response[ApiRunQueryResponse]
     """
 
     kwargs = _get_kwargs(
         project_uuid=project_uuid,
+        explore_id=explore_id,
         client=client,
         json_body=json_body,
     )
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
         response = await _client.request(**kwargs)
 
     return _build_response(client=client, response=response)
 
 
 async def asyncio(
     project_uuid: str,
+    explore_id: str,
     *,
     client: Client,
-    json_body: ProjectTablesConfiguration,
-) -> Optional[UpdateProjectTablesConfigurationResponse201]:
-    """Update project tables configuration
-
-     Update project tables configuration
+    json_body: RunQueryRequest,
+) -> Optional[ApiRunQueryResponse]:
+    """Run a query for underlying data results
 
     Args:
         project_uuid (str):
-        json_body (ProjectTablesConfiguration):
+        explore_id (str):
+        json_body (RunQueryRequest):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        UpdateProjectTablesConfigurationResponse201
+        ApiRunQueryResponse
     """
 
     return (
         await asyncio_detailed(
             project_uuid=project_uuid,
+            explore_id=explore_id,
             client=client,
             json_body=json_body,
         )
     ).parsed
```

### Comparing `lightdash_client_python-0.1.2/lightdash_client/api/saved/create_saved_chart_version.py` & `lightdash_client_python-0.611.0/lightdash_client/api/charts/post_chart_results.py`

 * *Files 25% similar despite different names*

```diff
@@ -3,26 +3,26 @@
 from typing import Dict
 from typing import Optional
 
 import httpx
 
 from ... import errors
 from ...client import Client
-from ...models.create_saved_chart_version import CreateSavedChartVersion
-from ...models.create_saved_chart_version_response_200 import CreateSavedChartVersionResponse200
+from ...models.api_run_query_response import ApiRunQueryResponse
+from ...models.post_chart_results_json_body import PostChartResultsJsonBody
 from ...types import Response
 
 
 def _get_kwargs(
-    saved_chart_uuid: str,
+    chart_uuid: str,
     *,
     client: Client,
-    json_body: CreateSavedChartVersion,
+    json_body: PostChartResultsJsonBody,
 ) -> Dict[str, Any]:
-    url = "{}/saved/{savedChartUuid}/version".format(client.base_url, savedChartUuid=saved_chart_uuid)
+    url = "{}/api/v1/saved/{chartUuid}/results".format(client.base_url, chartUuid=chart_uuid)
 
     headers: Dict[str, str] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     json_json_body = json_body.to_dict()
 
     return {
@@ -32,147 +32,147 @@
         "cookies": cookies,
         "timeout": client.get_timeout(),
         "follow_redirects": client.follow_redirects,
         "json": json_json_body,
     }
 
 
-def _parse_response(*, client: Client, response: httpx.Response) -> Optional[CreateSavedChartVersionResponse200]:
+def _parse_response(*, client: Client, response: httpx.Response) -> Optional[ApiRunQueryResponse]:
     if response.status_code == HTTPStatus.OK:
-        response_200 = CreateSavedChartVersionResponse200.from_dict(response.json())
+        response_200 = ApiRunQueryResponse.from_dict(response.json())
 
         return response_200
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
-def _build_response(*, client: Client, response: httpx.Response) -> Response[CreateSavedChartVersionResponse200]:
+def _build_response(*, client: Client, response: httpx.Response) -> Response[ApiRunQueryResponse]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
-    saved_chart_uuid: str,
+    chart_uuid: str,
     *,
     client: Client,
-    json_body: CreateSavedChartVersion,
-) -> Response[CreateSavedChartVersionResponse200]:
-    """Create a new saved chart version
+    json_body: PostChartResultsJsonBody,
+) -> Response[ApiRunQueryResponse]:
+    """Run a query for a chart
 
     Args:
-        saved_chart_uuid (str):
-        json_body (CreateSavedChartVersion):
+        chart_uuid (str):
+        json_body (PostChartResultsJsonBody):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[CreateSavedChartVersionResponse200]
+        Response[ApiRunQueryResponse]
     """
 
     kwargs = _get_kwargs(
-        saved_chart_uuid=saved_chart_uuid,
+        chart_uuid=chart_uuid,
         client=client,
         json_body=json_body,
     )
 
     response = httpx.request(
         verify=client.verify_ssl,
         **kwargs,
     )
 
     return _build_response(client=client, response=response)
 
 
 def sync(
-    saved_chart_uuid: str,
+    chart_uuid: str,
     *,
     client: Client,
-    json_body: CreateSavedChartVersion,
-) -> Optional[CreateSavedChartVersionResponse200]:
-    """Create a new saved chart version
+    json_body: PostChartResultsJsonBody,
+) -> Optional[ApiRunQueryResponse]:
+    """Run a query for a chart
 
     Args:
-        saved_chart_uuid (str):
-        json_body (CreateSavedChartVersion):
+        chart_uuid (str):
+        json_body (PostChartResultsJsonBody):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        CreateSavedChartVersionResponse200
+        ApiRunQueryResponse
     """
 
     return sync_detailed(
-        saved_chart_uuid=saved_chart_uuid,
+        chart_uuid=chart_uuid,
         client=client,
         json_body=json_body,
     ).parsed
 
 
 async def asyncio_detailed(
-    saved_chart_uuid: str,
+    chart_uuid: str,
     *,
     client: Client,
-    json_body: CreateSavedChartVersion,
-) -> Response[CreateSavedChartVersionResponse200]:
-    """Create a new saved chart version
+    json_body: PostChartResultsJsonBody,
+) -> Response[ApiRunQueryResponse]:
+    """Run a query for a chart
 
     Args:
-        saved_chart_uuid (str):
-        json_body (CreateSavedChartVersion):
+        chart_uuid (str):
+        json_body (PostChartResultsJsonBody):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[CreateSavedChartVersionResponse200]
+        Response[ApiRunQueryResponse]
     """
 
     kwargs = _get_kwargs(
-        saved_chart_uuid=saved_chart_uuid,
+        chart_uuid=chart_uuid,
         client=client,
         json_body=json_body,
     )
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
         response = await _client.request(**kwargs)
 
     return _build_response(client=client, response=response)
 
 
 async def asyncio(
-    saved_chart_uuid: str,
+    chart_uuid: str,
     *,
     client: Client,
-    json_body: CreateSavedChartVersion,
-) -> Optional[CreateSavedChartVersionResponse200]:
-    """Create a new saved chart version
+    json_body: PostChartResultsJsonBody,
+) -> Optional[ApiRunQueryResponse]:
+    """Run a query for a chart
 
     Args:
-        saved_chart_uuid (str):
-        json_body (CreateSavedChartVersion):
+        chart_uuid (str):
+        json_body (PostChartResultsJsonBody):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        CreateSavedChartVersionResponse200
+        ApiRunQueryResponse
     """
 
     return (
         await asyncio_detailed(
-            saved_chart_uuid=saved_chart_uuid,
+            chart_uuid=chart_uuid,
             client=client,
             json_body=json_body,
         )
     ).parsed
```

### Comparing `lightdash_client_python-0.1.2/lightdash_client/api/saved/delete_saved_chart.py` & `lightdash_client_python-0.611.0/lightdash_client/api/schedulers/delete_scheduler.py`

 * *Files 21% similar despite different names*

```diff
@@ -3,159 +3,159 @@
 from typing import Dict
 from typing import Optional
 
 import httpx
 
 from ... import errors
 from ...client import Client
-from ...models.success import Success
+from ...models.delete_scheduler_response_201 import DeleteSchedulerResponse201
 from ...types import Response
 
 
 def _get_kwargs(
-    saved_chart_uuid: str,
+    scheduler_uuid: str,
     *,
     client: Client,
 ) -> Dict[str, Any]:
-    url = "{}/saved/{savedChartUuid}".format(client.base_url, savedChartUuid=saved_chart_uuid)
+    url = "{}/api/v1/schedulers/{schedulerUuid}".format(client.base_url, schedulerUuid=scheduler_uuid)
 
     headers: Dict[str, str] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     return {
         "method": "delete",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
         "follow_redirects": client.follow_redirects,
     }
 
 
-def _parse_response(*, client: Client, response: httpx.Response) -> Optional[Success]:
-    if response.status_code == HTTPStatus.OK:
-        response_200 = Success.from_dict(response.json())
+def _parse_response(*, client: Client, response: httpx.Response) -> Optional[DeleteSchedulerResponse201]:
+    if response.status_code == HTTPStatus.CREATED:
+        response_201 = DeleteSchedulerResponse201.from_dict(response.json())
 
-        return response_200
+        return response_201
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
-def _build_response(*, client: Client, response: httpx.Response) -> Response[Success]:
+def _build_response(*, client: Client, response: httpx.Response) -> Response[DeleteSchedulerResponse201]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
-    saved_chart_uuid: str,
+    scheduler_uuid: str,
     *,
     client: Client,
-) -> Response[Success]:
-    """Delete a saved chart
+) -> Response[DeleteSchedulerResponse201]:
+    """Delete a scheduler
 
     Args:
-        saved_chart_uuid (str):
+        scheduler_uuid (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Success]
+        Response[DeleteSchedulerResponse201]
     """
 
     kwargs = _get_kwargs(
-        saved_chart_uuid=saved_chart_uuid,
+        scheduler_uuid=scheduler_uuid,
         client=client,
     )
 
     response = httpx.request(
         verify=client.verify_ssl,
         **kwargs,
     )
 
     return _build_response(client=client, response=response)
 
 
 def sync(
-    saved_chart_uuid: str,
+    scheduler_uuid: str,
     *,
     client: Client,
-) -> Optional[Success]:
-    """Delete a saved chart
+) -> Optional[DeleteSchedulerResponse201]:
+    """Delete a scheduler
 
     Args:
-        saved_chart_uuid (str):
+        scheduler_uuid (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Success
+        DeleteSchedulerResponse201
     """
 
     return sync_detailed(
-        saved_chart_uuid=saved_chart_uuid,
+        scheduler_uuid=scheduler_uuid,
         client=client,
     ).parsed
 
 
 async def asyncio_detailed(
-    saved_chart_uuid: str,
+    scheduler_uuid: str,
     *,
     client: Client,
-) -> Response[Success]:
-    """Delete a saved chart
+) -> Response[DeleteSchedulerResponse201]:
+    """Delete a scheduler
 
     Args:
-        saved_chart_uuid (str):
+        scheduler_uuid (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Success]
+        Response[DeleteSchedulerResponse201]
     """
 
     kwargs = _get_kwargs(
-        saved_chart_uuid=saved_chart_uuid,
+        scheduler_uuid=scheduler_uuid,
         client=client,
     )
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
         response = await _client.request(**kwargs)
 
     return _build_response(client=client, response=response)
 
 
 async def asyncio(
-    saved_chart_uuid: str,
+    scheduler_uuid: str,
     *,
     client: Client,
-) -> Optional[Success]:
-    """Delete a saved chart
+) -> Optional[DeleteSchedulerResponse201]:
+    """Delete a scheduler
 
     Args:
-        saved_chart_uuid (str):
+        scheduler_uuid (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Success
+        DeleteSchedulerResponse201
     """
 
     return (
         await asyncio_detailed(
-            saved_chart_uuid=saved_chart_uuid,
+            scheduler_uuid=scheduler_uuid,
             client=client,
         )
     ).parsed
```

### Comparing `lightdash_client_python-0.1.2/lightdash_client/api/saved/get_saved_chart.py` & `lightdash_client_python-0.611.0/lightdash_client/api/user_groups/get_group.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,159 +3,159 @@
 from typing import Dict
 from typing import Optional
 
 import httpx
 
 from ... import errors
 from ...client import Client
-from ...models.get_saved_chart_response_200 import GetSavedChartResponse200
+from ...models.api_group_response import ApiGroupResponse
 from ...types import Response
 
 
 def _get_kwargs(
-    saved_chart_uuid: str,
+    group_uuid: str,
     *,
     client: Client,
 ) -> Dict[str, Any]:
-    url = "{}/saved/{savedChartUuid}".format(client.base_url, savedChartUuid=saved_chart_uuid)
+    url = "{}/api/v1/groups/{groupUuid}".format(client.base_url, groupUuid=group_uuid)
 
     headers: Dict[str, str] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     return {
         "method": "get",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
         "follow_redirects": client.follow_redirects,
     }
 
 
-def _parse_response(*, client: Client, response: httpx.Response) -> Optional[GetSavedChartResponse200]:
+def _parse_response(*, client: Client, response: httpx.Response) -> Optional[ApiGroupResponse]:
     if response.status_code == HTTPStatus.OK:
-        response_200 = GetSavedChartResponse200.from_dict(response.json())
+        response_200 = ApiGroupResponse.from_dict(response.json())
 
         return response_200
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
-def _build_response(*, client: Client, response: httpx.Response) -> Response[GetSavedChartResponse200]:
+def _build_response(*, client: Client, response: httpx.Response) -> Response[ApiGroupResponse]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
-    saved_chart_uuid: str,
+    group_uuid: str,
     *,
     client: Client,
-) -> Response[GetSavedChartResponse200]:
-    """Get a saved chart
+) -> Response[ApiGroupResponse]:
+    """Get group details
 
     Args:
-        saved_chart_uuid (str):
+        group_uuid (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[GetSavedChartResponse200]
+        Response[ApiGroupResponse]
     """
 
     kwargs = _get_kwargs(
-        saved_chart_uuid=saved_chart_uuid,
+        group_uuid=group_uuid,
         client=client,
     )
 
     response = httpx.request(
         verify=client.verify_ssl,
         **kwargs,
     )
 
     return _build_response(client=client, response=response)
 
 
 def sync(
-    saved_chart_uuid: str,
+    group_uuid: str,
     *,
     client: Client,
-) -> Optional[GetSavedChartResponse200]:
-    """Get a saved chart
+) -> Optional[ApiGroupResponse]:
+    """Get group details
 
     Args:
-        saved_chart_uuid (str):
+        group_uuid (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        GetSavedChartResponse200
+        ApiGroupResponse
     """
 
     return sync_detailed(
-        saved_chart_uuid=saved_chart_uuid,
+        group_uuid=group_uuid,
         client=client,
     ).parsed
 
 
 async def asyncio_detailed(
-    saved_chart_uuid: str,
+    group_uuid: str,
     *,
     client: Client,
-) -> Response[GetSavedChartResponse200]:
-    """Get a saved chart
+) -> Response[ApiGroupResponse]:
+    """Get group details
 
     Args:
-        saved_chart_uuid (str):
+        group_uuid (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[GetSavedChartResponse200]
+        Response[ApiGroupResponse]
     """
 
     kwargs = _get_kwargs(
-        saved_chart_uuid=saved_chart_uuid,
+        group_uuid=group_uuid,
         client=client,
     )
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
         response = await _client.request(**kwargs)
 
     return _build_response(client=client, response=response)
 
 
 async def asyncio(
-    saved_chart_uuid: str,
+    group_uuid: str,
     *,
     client: Client,
-) -> Optional[GetSavedChartResponse200]:
-    """Get a saved chart
+) -> Optional[ApiGroupResponse]:
+    """Get group details
 
     Args:
-        saved_chart_uuid (str):
+        group_uuid (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        GetSavedChartResponse200
+        ApiGroupResponse
     """
 
     return (
         await asyncio_detailed(
-            saved_chart_uuid=saved_chart_uuid,
+            group_uuid=group_uuid,
             client=client,
         )
     ).parsed
```

### Comparing `lightdash_client_python-0.1.2/lightdash_client/api/saved/patch_saved_chart.py` & `lightdash_client_python-0.611.0/lightdash_client/api/content/update_pinned_items_order.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,178 +1,198 @@
 from http import HTTPStatus
 from typing import Any
 from typing import Dict
+from typing import List
 from typing import Optional
 
 import httpx
 
 from ... import errors
 from ...client import Client
-from ...models.patch_saved_chart_response_200 import PatchSavedChartResponse200
-from ...models.update_saved_chart import UpdateSavedChart
+from ...models.api_pinned_items import ApiPinnedItems
+from ...models.update_pinned_item_order import UpdatePinnedItemOrder
 from ...types import Response
 
 
 def _get_kwargs(
-    saved_chart_uuid: str,
+    project_uuid: str,
+    pinned_list_uuid: str,
     *,
     client: Client,
-    json_body: UpdateSavedChart,
+    json_body: List["UpdatePinnedItemOrder"],
 ) -> Dict[str, Any]:
-    url = "{}/saved/{savedChartUuid}".format(client.base_url, savedChartUuid=saved_chart_uuid)
+    url = "{}/api/v1/projects/{projectUuid}/pinned-lists/{pinnedListUuid}/items/order".format(
+        client.base_url, projectUuid=project_uuid, pinnedListUuid=pinned_list_uuid
+    )
 
     headers: Dict[str, str] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
-    json_json_body = json_body.to_dict()
+    json_json_body = []
+    for json_body_item_data in json_body:
+        json_body_item = json_body_item_data.to_dict()
+
+        json_json_body.append(json_body_item)
 
     return {
         "method": "patch",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
         "follow_redirects": client.follow_redirects,
         "json": json_json_body,
     }
 
 
-def _parse_response(*, client: Client, response: httpx.Response) -> Optional[PatchSavedChartResponse200]:
+def _parse_response(*, client: Client, response: httpx.Response) -> Optional[ApiPinnedItems]:
     if response.status_code == HTTPStatus.OK:
-        response_200 = PatchSavedChartResponse200.from_dict(response.json())
+        response_200 = ApiPinnedItems.from_dict(response.json())
 
         return response_200
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
-def _build_response(*, client: Client, response: httpx.Response) -> Response[PatchSavedChartResponse200]:
+def _build_response(*, client: Client, response: httpx.Response) -> Response[ApiPinnedItems]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
-    saved_chart_uuid: str,
+    project_uuid: str,
+    pinned_list_uuid: str,
     *,
     client: Client,
-    json_body: UpdateSavedChart,
-) -> Response[PatchSavedChartResponse200]:
-    """Update a saved chart
+    json_body: List["UpdatePinnedItemOrder"],
+) -> Response[ApiPinnedItems]:
+    """Update pinned items order
 
     Args:
-        saved_chart_uuid (str):
-        json_body (UpdateSavedChart):
+        project_uuid (str):
+        pinned_list_uuid (str):
+        json_body (List['UpdatePinnedItemOrder']): the new order of the pinned items
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[PatchSavedChartResponse200]
+        Response[ApiPinnedItems]
     """
 
     kwargs = _get_kwargs(
-        saved_chart_uuid=saved_chart_uuid,
+        project_uuid=project_uuid,
+        pinned_list_uuid=pinned_list_uuid,
         client=client,
         json_body=json_body,
     )
 
     response = httpx.request(
         verify=client.verify_ssl,
         **kwargs,
     )
 
     return _build_response(client=client, response=response)
 
 
 def sync(
-    saved_chart_uuid: str,
+    project_uuid: str,
+    pinned_list_uuid: str,
     *,
     client: Client,
-    json_body: UpdateSavedChart,
-) -> Optional[PatchSavedChartResponse200]:
-    """Update a saved chart
+    json_body: List["UpdatePinnedItemOrder"],
+) -> Optional[ApiPinnedItems]:
+    """Update pinned items order
 
     Args:
-        saved_chart_uuid (str):
-        json_body (UpdateSavedChart):
+        project_uuid (str):
+        pinned_list_uuid (str):
+        json_body (List['UpdatePinnedItemOrder']): the new order of the pinned items
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        PatchSavedChartResponse200
+        ApiPinnedItems
     """
 
     return sync_detailed(
-        saved_chart_uuid=saved_chart_uuid,
+        project_uuid=project_uuid,
+        pinned_list_uuid=pinned_list_uuid,
         client=client,
         json_body=json_body,
     ).parsed
 
 
 async def asyncio_detailed(
-    saved_chart_uuid: str,
+    project_uuid: str,
+    pinned_list_uuid: str,
     *,
     client: Client,
-    json_body: UpdateSavedChart,
-) -> Response[PatchSavedChartResponse200]:
-    """Update a saved chart
+    json_body: List["UpdatePinnedItemOrder"],
+) -> Response[ApiPinnedItems]:
+    """Update pinned items order
 
     Args:
-        saved_chart_uuid (str):
-        json_body (UpdateSavedChart):
+        project_uuid (str):
+        pinned_list_uuid (str):
+        json_body (List['UpdatePinnedItemOrder']): the new order of the pinned items
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[PatchSavedChartResponse200]
+        Response[ApiPinnedItems]
     """
 
     kwargs = _get_kwargs(
-        saved_chart_uuid=saved_chart_uuid,
+        project_uuid=project_uuid,
+        pinned_list_uuid=pinned_list_uuid,
         client=client,
         json_body=json_body,
     )
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
         response = await _client.request(**kwargs)
 
     return _build_response(client=client, response=response)
 
 
 async def asyncio(
-    saved_chart_uuid: str,
+    project_uuid: str,
+    pinned_list_uuid: str,
     *,
     client: Client,
-    json_body: UpdateSavedChart,
-) -> Optional[PatchSavedChartResponse200]:
-    """Update a saved chart
+    json_body: List["UpdatePinnedItemOrder"],
+) -> Optional[ApiPinnedItems]:
+    """Update pinned items order
 
     Args:
-        saved_chart_uuid (str):
-        json_body (UpdateSavedChart):
+        project_uuid (str):
+        pinned_list_uuid (str):
+        json_body (List['UpdatePinnedItemOrder']): the new order of the pinned items
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        PatchSavedChartResponse200
+        ApiPinnedItems
     """
 
     return (
         await asyncio_detailed(
-            saved_chart_uuid=saved_chart_uuid,
+            project_uuid=project_uuid,
+            pinned_list_uuid=pinned_list_uuid,
             client=client,
             json_body=json_body,
         )
     ).parsed
```

### Comparing `lightdash_client_python-0.1.2/lightdash_client/api/saved/patch_saved_charts.py` & `lightdash_client_python-0.611.0/lightdash_client/api/exports/get_csv_url.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,183 +1,161 @@
 from http import HTTPStatus
 from typing import Any
 from typing import Dict
-from typing import List
 from typing import Optional
 
 import httpx
 
 from ... import errors
 from ...client import Client
-from ...models.patch_saved_charts_response_200 import PatchSavedChartsResponse200
-from ...models.update_multiple_saved_chart import UpdateMultipleSavedChart
+from ...models.api_csv_url_response import ApiCsvUrlResponse
 from ...types import Response
 
 
 def _get_kwargs(
-    project_uuid: str,
+    job_id: str,
     *,
     client: Client,
-    json_body: List["UpdateMultipleSavedChart"],
 ) -> Dict[str, Any]:
-    url = "{}/projects/{projectUuid}/saved".format(client.base_url, projectUuid=project_uuid)
+    url = "{}/api/v1/csv/{jobId}".format(client.base_url, jobId=job_id)
 
     headers: Dict[str, str] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
-    json_json_body = []
-    for json_body_item_data in json_body:
-        json_body_item = json_body_item_data.to_dict()
-
-        json_json_body.append(json_body_item)
-
     return {
-        "method": "patch",
+        "method": "get",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
         "follow_redirects": client.follow_redirects,
-        "json": json_json_body,
     }
 
 
-def _parse_response(*, client: Client, response: httpx.Response) -> Optional[PatchSavedChartsResponse200]:
+def _parse_response(*, client: Client, response: httpx.Response) -> Optional[ApiCsvUrlResponse]:
     if response.status_code == HTTPStatus.OK:
-        response_200 = PatchSavedChartsResponse200.from_dict(response.json())
+        response_200 = ApiCsvUrlResponse.from_dict(response.json())
 
         return response_200
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
-def _build_response(*, client: Client, response: httpx.Response) -> Response[PatchSavedChartsResponse200]:
+def _build_response(*, client: Client, response: httpx.Response) -> Response[ApiCsvUrlResponse]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
-    project_uuid: str,
+    job_id: str,
     *,
     client: Client,
-    json_body: List["UpdateMultipleSavedChart"],
-) -> Response[PatchSavedChartsResponse200]:
-    """Update multiple saved charts in project
+) -> Response[ApiCsvUrlResponse]:
+    """Get a Csv
 
     Args:
-        project_uuid (str):
-        json_body (List['UpdateMultipleSavedChart']):
+        job_id (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[PatchSavedChartsResponse200]
+        Response[ApiCsvUrlResponse]
     """
 
     kwargs = _get_kwargs(
-        project_uuid=project_uuid,
+        job_id=job_id,
         client=client,
-        json_body=json_body,
     )
 
     response = httpx.request(
         verify=client.verify_ssl,
         **kwargs,
     )
 
     return _build_response(client=client, response=response)
 
 
 def sync(
-    project_uuid: str,
+    job_id: str,
     *,
     client: Client,
-    json_body: List["UpdateMultipleSavedChart"],
-) -> Optional[PatchSavedChartsResponse200]:
-    """Update multiple saved charts in project
+) -> Optional[ApiCsvUrlResponse]:
+    """Get a Csv
 
     Args:
-        project_uuid (str):
-        json_body (List['UpdateMultipleSavedChart']):
+        job_id (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        PatchSavedChartsResponse200
+        ApiCsvUrlResponse
     """
 
     return sync_detailed(
-        project_uuid=project_uuid,
+        job_id=job_id,
         client=client,
-        json_body=json_body,
     ).parsed
 
 
 async def asyncio_detailed(
-    project_uuid: str,
+    job_id: str,
     *,
     client: Client,
-    json_body: List["UpdateMultipleSavedChart"],
-) -> Response[PatchSavedChartsResponse200]:
-    """Update multiple saved charts in project
+) -> Response[ApiCsvUrlResponse]:
+    """Get a Csv
 
     Args:
-        project_uuid (str):
-        json_body (List['UpdateMultipleSavedChart']):
+        job_id (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[PatchSavedChartsResponse200]
+        Response[ApiCsvUrlResponse]
     """
 
     kwargs = _get_kwargs(
-        project_uuid=project_uuid,
+        job_id=job_id,
         client=client,
-        json_body=json_body,
     )
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
         response = await _client.request(**kwargs)
 
     return _build_response(client=client, response=response)
 
 
 async def asyncio(
-    project_uuid: str,
+    job_id: str,
     *,
     client: Client,
-    json_body: List["UpdateMultipleSavedChart"],
-) -> Optional[PatchSavedChartsResponse200]:
-    """Update multiple saved charts in project
+) -> Optional[ApiCsvUrlResponse]:
+    """Get a Csv
 
     Args:
-        project_uuid (str):
-        json_body (List['UpdateMultipleSavedChart']):
+        job_id (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        PatchSavedChartsResponse200
+        ApiCsvUrlResponse
     """
 
     return (
         await asyncio_detailed(
-            project_uuid=project_uuid,
+            job_id=job_id,
             client=client,
-            json_body=json_body,
         )
     ).parsed
```

### Comparing `lightdash_client_python-0.1.2/lightdash_client/api/saved/post_saved_chart.py` & `lightdash_client_python-0.611.0/lightdash_client/api/projects/validate_project.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,200 +1,194 @@
 from http import HTTPStatus
 from typing import Any
 from typing import Dict
 from typing import Optional
-from typing import Union
 
 import httpx
 
 from ... import errors
 from ...client import Client
-from ...models.create_saved_chart import CreateSavedChart
-from ...models.post_saved_chart_response_200 import PostSavedChartResponse200
+from ...models.api_job_scheduled_response import ApiJobScheduledResponse
+from ...models.validate_project_json_body import ValidateProjectJsonBody
 from ...types import Response
-from ...types import UNSET
-from ...types import Unset
 
 
 def _get_kwargs(
     project_uuid: str,
     *,
     client: Client,
-    json_body: CreateSavedChart,
-    duplicate_from: Union[Unset, None, str] = UNSET,
+    json_body: ValidateProjectJsonBody,
 ) -> Dict[str, Any]:
-    url = "{}/projects/{projectUuid}/saved".format(client.base_url, projectUuid=project_uuid)
+    url = "{}/api/v1/projects/{projectUuid}/validate".format(client.base_url, projectUuid=project_uuid)
 
     headers: Dict[str, str] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
-    params: Dict[str, Any] = {}
-    params["duplicateFrom"] = duplicate_from
-
-    params = {k: v for k, v in params.items() if v is not UNSET and v is not None}
-
     json_json_body = json_body.to_dict()
 
     return {
         "method": "post",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
         "follow_redirects": client.follow_redirects,
         "json": json_json_body,
-        "params": params,
     }
 
 
-def _parse_response(*, client: Client, response: httpx.Response) -> Optional[PostSavedChartResponse200]:
+def _parse_response(*, client: Client, response: httpx.Response) -> Optional[ApiJobScheduledResponse]:
     if response.status_code == HTTPStatus.OK:
-        response_200 = PostSavedChartResponse200.from_dict(response.json())
+        response_200 = ApiJobScheduledResponse.from_dict(response.json())
 
         return response_200
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
-def _build_response(*, client: Client, response: httpx.Response) -> Response[PostSavedChartResponse200]:
+def _build_response(*, client: Client, response: httpx.Response) -> Response[ApiJobScheduledResponse]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
     project_uuid: str,
     *,
     client: Client,
-    json_body: CreateSavedChart,
-    duplicate_from: Union[Unset, None, str] = UNSET,
-) -> Response[PostSavedChartResponse200]:
-    """Create saved chart in project
+    json_body: ValidateProjectJsonBody,
+) -> Response[ApiJobScheduledResponse]:
+    """Validate content inside a project. This will start a validation job and return the job id.
+
+    Validation jobs scan all charts and dashboards inside a project to find any broken references
+    to metrics or dimensions that aren't available. Results are available after the job is completed.
 
     Args:
         project_uuid (str):
-        duplicate_from (Union[Unset, None, str]):
-        json_body (CreateSavedChart):
+        json_body (ValidateProjectJsonBody): the compiled explores to validate against an existing
+            project, this is used in the CLI to validate a project without creating a preview
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[PostSavedChartResponse200]
+        Response[ApiJobScheduledResponse]
     """
 
     kwargs = _get_kwargs(
         project_uuid=project_uuid,
         client=client,
         json_body=json_body,
-        duplicate_from=duplicate_from,
     )
 
     response = httpx.request(
         verify=client.verify_ssl,
         **kwargs,
     )
 
     return _build_response(client=client, response=response)
 
 
 def sync(
     project_uuid: str,
     *,
     client: Client,
-    json_body: CreateSavedChart,
-    duplicate_from: Union[Unset, None, str] = UNSET,
-) -> Optional[PostSavedChartResponse200]:
-    """Create saved chart in project
+    json_body: ValidateProjectJsonBody,
+) -> Optional[ApiJobScheduledResponse]:
+    """Validate content inside a project. This will start a validation job and return the job id.
+
+    Validation jobs scan all charts and dashboards inside a project to find any broken references
+    to metrics or dimensions that aren't available. Results are available after the job is completed.
 
     Args:
         project_uuid (str):
-        duplicate_from (Union[Unset, None, str]):
-        json_body (CreateSavedChart):
+        json_body (ValidateProjectJsonBody): the compiled explores to validate against an existing
+            project, this is used in the CLI to validate a project without creating a preview
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        PostSavedChartResponse200
+        ApiJobScheduledResponse
     """
 
     return sync_detailed(
         project_uuid=project_uuid,
         client=client,
         json_body=json_body,
-        duplicate_from=duplicate_from,
     ).parsed
 
 
 async def asyncio_detailed(
     project_uuid: str,
     *,
     client: Client,
-    json_body: CreateSavedChart,
-    duplicate_from: Union[Unset, None, str] = UNSET,
-) -> Response[PostSavedChartResponse200]:
-    """Create saved chart in project
+    json_body: ValidateProjectJsonBody,
+) -> Response[ApiJobScheduledResponse]:
+    """Validate content inside a project. This will start a validation job and return the job id.
+
+    Validation jobs scan all charts and dashboards inside a project to find any broken references
+    to metrics or dimensions that aren't available. Results are available after the job is completed.
 
     Args:
         project_uuid (str):
-        duplicate_from (Union[Unset, None, str]):
-        json_body (CreateSavedChart):
+        json_body (ValidateProjectJsonBody): the compiled explores to validate against an existing
+            project, this is used in the CLI to validate a project without creating a preview
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[PostSavedChartResponse200]
+        Response[ApiJobScheduledResponse]
     """
 
     kwargs = _get_kwargs(
         project_uuid=project_uuid,
         client=client,
         json_body=json_body,
-        duplicate_from=duplicate_from,
     )
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
         response = await _client.request(**kwargs)
 
     return _build_response(client=client, response=response)
 
 
 async def asyncio(
     project_uuid: str,
     *,
     client: Client,
-    json_body: CreateSavedChart,
-    duplicate_from: Union[Unset, None, str] = UNSET,
-) -> Optional[PostSavedChartResponse200]:
-    """Create saved chart in project
+    json_body: ValidateProjectJsonBody,
+) -> Optional[ApiJobScheduledResponse]:
+    """Validate content inside a project. This will start a validation job and return the job id.
+
+    Validation jobs scan all charts and dashboards inside a project to find any broken references
+    to metrics or dimensions that aren't available. Results are available after the job is completed.
 
     Args:
         project_uuid (str):
-        duplicate_from (Union[Unset, None, str]):
-        json_body (CreateSavedChart):
+        json_body (ValidateProjectJsonBody): the compiled explores to validate against an existing
+            project, this is used in the CLI to validate a project without creating a preview
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        PostSavedChartResponse200
+        ApiJobScheduledResponse
     """
 
     return (
         await asyncio_detailed(
             project_uuid=project_uuid,
             client=client,
             json_body=json_body,
-            duplicate_from=duplicate_from,
         )
     ).parsed
```

### Comparing `lightdash_client_python-0.1.2/lightdash_client/api/saved_chart/get_available_chart_filters.py` & `lightdash_client_python-0.611.0/lightdash_client/api/integrations/get_dbt_cloud_metrics.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,159 +3,169 @@
 from typing import Dict
 from typing import Optional
 
 import httpx
 
 from ... import errors
 from ...client import Client
-from ...models.get_available_chart_filters_response_200 import GetAvailableChartFiltersResponse200
+from ...models.api_dbt_cloud_metrics import ApiDbtCloudMetrics
 from ...types import Response
 
 
 def _get_kwargs(
-    saved_chart_uuid: str,
+    project_uuid: str,
     *,
     client: Client,
 ) -> Dict[str, Any]:
-    url = "{}/saved/{savedChartUuid}/availableFilters".format(client.base_url, savedChartUuid=saved_chart_uuid)
+    url = "{}/api/v1/projects/{projectUuid}/integrations/dbt-cloud/metrics".format(
+        client.base_url, projectUuid=project_uuid
+    )
 
     headers: Dict[str, str] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     return {
         "method": "get",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
         "follow_redirects": client.follow_redirects,
     }
 
 
-def _parse_response(*, client: Client, response: httpx.Response) -> Optional[GetAvailableChartFiltersResponse200]:
+def _parse_response(*, client: Client, response: httpx.Response) -> Optional[ApiDbtCloudMetrics]:
     if response.status_code == HTTPStatus.OK:
-        response_200 = GetAvailableChartFiltersResponse200.from_dict(response.json())
+        response_200 = ApiDbtCloudMetrics.from_dict(response.json())
 
         return response_200
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
-def _build_response(*, client: Client, response: httpx.Response) -> Response[GetAvailableChartFiltersResponse200]:
+def _build_response(*, client: Client, response: httpx.Response) -> Response[ApiDbtCloudMetrics]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
-    saved_chart_uuid: str,
+    project_uuid: str,
     *,
     client: Client,
-) -> Response[GetAvailableChartFiltersResponse200]:
-    """Get available filters for a saved chart
+) -> Response[ApiDbtCloudMetrics]:
+    """Get a list of dbt metric definitions from the dbt Cloud metadata api.
+    The metrics are taken from the metadata from a single dbt Cloud job configured
+    with the dbt Cloud integration settings for the project.
 
     Args:
-        saved_chart_uuid (str):
+        project_uuid (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[GetAvailableChartFiltersResponse200]
+        Response[ApiDbtCloudMetrics]
     """
 
     kwargs = _get_kwargs(
-        saved_chart_uuid=saved_chart_uuid,
+        project_uuid=project_uuid,
         client=client,
     )
 
     response = httpx.request(
         verify=client.verify_ssl,
         **kwargs,
     )
 
     return _build_response(client=client, response=response)
 
 
 def sync(
-    saved_chart_uuid: str,
+    project_uuid: str,
     *,
     client: Client,
-) -> Optional[GetAvailableChartFiltersResponse200]:
-    """Get available filters for a saved chart
+) -> Optional[ApiDbtCloudMetrics]:
+    """Get a list of dbt metric definitions from the dbt Cloud metadata api.
+    The metrics are taken from the metadata from a single dbt Cloud job configured
+    with the dbt Cloud integration settings for the project.
 
     Args:
-        saved_chart_uuid (str):
+        project_uuid (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        GetAvailableChartFiltersResponse200
+        ApiDbtCloudMetrics
     """
 
     return sync_detailed(
-        saved_chart_uuid=saved_chart_uuid,
+        project_uuid=project_uuid,
         client=client,
     ).parsed
 
 
 async def asyncio_detailed(
-    saved_chart_uuid: str,
+    project_uuid: str,
     *,
     client: Client,
-) -> Response[GetAvailableChartFiltersResponse200]:
-    """Get available filters for a saved chart
+) -> Response[ApiDbtCloudMetrics]:
+    """Get a list of dbt metric definitions from the dbt Cloud metadata api.
+    The metrics are taken from the metadata from a single dbt Cloud job configured
+    with the dbt Cloud integration settings for the project.
 
     Args:
-        saved_chart_uuid (str):
+        project_uuid (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[GetAvailableChartFiltersResponse200]
+        Response[ApiDbtCloudMetrics]
     """
 
     kwargs = _get_kwargs(
-        saved_chart_uuid=saved_chart_uuid,
+        project_uuid=project_uuid,
         client=client,
     )
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
         response = await _client.request(**kwargs)
 
     return _build_response(client=client, response=response)
 
 
 async def asyncio(
-    saved_chart_uuid: str,
+    project_uuid: str,
     *,
     client: Client,
-) -> Optional[GetAvailableChartFiltersResponse200]:
-    """Get available filters for a saved chart
+) -> Optional[ApiDbtCloudMetrics]:
+    """Get a list of dbt metric definitions from the dbt Cloud metadata api.
+    The metrics are taken from the metadata from a single dbt Cloud job configured
+    with the dbt Cloud integration settings for the project.
 
     Args:
-        saved_chart_uuid (str):
+        project_uuid (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        GetAvailableChartFiltersResponse200
+        ApiDbtCloudMetrics
     """
 
     return (
         await asyncio_detailed(
-            saved_chart_uuid=saved_chart_uuid,
+            project_uuid=project_uuid,
             client=client,
         )
     ).parsed
```

### Comparing `lightdash_client_python-0.1.2/lightdash_client/api/user/create_invite_link.py` & `lightdash_client_python-0.611.0/lightdash_client/api/roles_permissions/grant_project_access_to_user.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,25 +3,26 @@
 from typing import Dict
 from typing import Optional
 
 import httpx
 
 from ... import errors
 from ...client import Client
-from ...models.create_invite_link import CreateInviteLink
-from ...models.create_invite_link_response_201 import CreateInviteLinkResponse201
+from ...models.api_success_empty import ApiSuccessEmpty
+from ...models.create_project_member import CreateProjectMember
 from ...types import Response
 
 
 def _get_kwargs(
+    project_uuid: str,
     *,
     client: Client,
-    json_body: CreateInviteLink,
+    json_body: CreateProjectMember,
 ) -> Dict[str, Any]:
-    url = "{}/invite-links".format(client.base_url)
+    url = "{}/api/v1/projects/{projectUuid}/access".format(client.base_url, projectUuid=project_uuid)
 
     headers: Dict[str, str] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     json_json_body = json_body.to_dict()
 
     return {
@@ -31,135 +32,147 @@
         "cookies": cookies,
         "timeout": client.get_timeout(),
         "follow_redirects": client.follow_redirects,
         "json": json_json_body,
     }
 
 
-def _parse_response(*, client: Client, response: httpx.Response) -> Optional[CreateInviteLinkResponse201]:
-    if response.status_code == HTTPStatus.CREATED:
-        response_201 = CreateInviteLinkResponse201.from_dict(response.json())
+def _parse_response(*, client: Client, response: httpx.Response) -> Optional[ApiSuccessEmpty]:
+    if response.status_code == HTTPStatus.OK:
+        response_200 = ApiSuccessEmpty.from_dict(response.json())
 
-        return response_201
+        return response_200
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
-def _build_response(*, client: Client, response: httpx.Response) -> Response[CreateInviteLinkResponse201]:
+def _build_response(*, client: Client, response: httpx.Response) -> Response[ApiSuccessEmpty]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
+    project_uuid: str,
     *,
     client: Client,
-    json_body: CreateInviteLink,
-) -> Response[CreateInviteLinkResponse201]:
-    """Create a new invite link
+    json_body: CreateProjectMember,
+) -> Response[ApiSuccessEmpty]:
+    """Grant a user access to a project
 
     Args:
-        json_body (CreateInviteLink):
+        project_uuid (str):
+        json_body (CreateProjectMember):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[CreateInviteLinkResponse201]
+        Response[ApiSuccessEmpty]
     """
 
     kwargs = _get_kwargs(
+        project_uuid=project_uuid,
         client=client,
         json_body=json_body,
     )
 
     response = httpx.request(
         verify=client.verify_ssl,
         **kwargs,
     )
 
     return _build_response(client=client, response=response)
 
 
 def sync(
+    project_uuid: str,
     *,
     client: Client,
-    json_body: CreateInviteLink,
-) -> Optional[CreateInviteLinkResponse201]:
-    """Create a new invite link
+    json_body: CreateProjectMember,
+) -> Optional[ApiSuccessEmpty]:
+    """Grant a user access to a project
 
     Args:
-        json_body (CreateInviteLink):
+        project_uuid (str):
+        json_body (CreateProjectMember):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        CreateInviteLinkResponse201
+        ApiSuccessEmpty
     """
 
     return sync_detailed(
+        project_uuid=project_uuid,
         client=client,
         json_body=json_body,
     ).parsed
 
 
 async def asyncio_detailed(
+    project_uuid: str,
     *,
     client: Client,
-    json_body: CreateInviteLink,
-) -> Response[CreateInviteLinkResponse201]:
-    """Create a new invite link
+    json_body: CreateProjectMember,
+) -> Response[ApiSuccessEmpty]:
+    """Grant a user access to a project
 
     Args:
-        json_body (CreateInviteLink):
+        project_uuid (str):
+        json_body (CreateProjectMember):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[CreateInviteLinkResponse201]
+        Response[ApiSuccessEmpty]
     """
 
     kwargs = _get_kwargs(
+        project_uuid=project_uuid,
         client=client,
         json_body=json_body,
     )
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
         response = await _client.request(**kwargs)
 
     return _build_response(client=client, response=response)
 
 
 async def asyncio(
+    project_uuid: str,
     *,
     client: Client,
-    json_body: CreateInviteLink,
-) -> Optional[CreateInviteLinkResponse201]:
-    """Create a new invite link
+    json_body: CreateProjectMember,
+) -> Optional[ApiSuccessEmpty]:
+    """Grant a user access to a project
 
     Args:
-        json_body (CreateInviteLink):
+        project_uuid (str):
+        json_body (CreateProjectMember):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        CreateInviteLinkResponse201
+        ApiSuccessEmpty
     """
 
     return (
         await asyncio_detailed(
+            project_uuid=project_uuid,
             client=client,
             json_body=json_body,
         )
     ).parsed
```

### Comparing `lightdash_client_python-0.1.2/lightdash_client/api/user/create_personal_access_token.py` & `lightdash_client_python-0.611.0/lightdash_client/api/my_account/list_my_available_organizations.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,163 +3,142 @@
 from typing import Dict
 from typing import Optional
 
 import httpx
 
 from ... import errors
 from ...client import Client
-from ...models.create_personal_access_token import CreatePersonalAccessToken
-from ...models.create_personal_access_token_response_200 import CreatePersonalAccessTokenResponse200
+from ...models.api_user_allowed_organizations_response import ApiUserAllowedOrganizationsResponse
 from ...types import Response
 
 
 def _get_kwargs(
     *,
     client: Client,
-    json_body: CreatePersonalAccessToken,
 ) -> Dict[str, Any]:
-    url = "{}/user/me/personal-access-tokens".format(client.base_url)
+    url = "{}/api/v1/user/me/allowedOrganizations".format(client.base_url)
 
     headers: Dict[str, str] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
-    json_json_body = json_body.to_dict()
-
     return {
-        "method": "post",
+        "method": "get",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
         "follow_redirects": client.follow_redirects,
-        "json": json_json_body,
     }
 
 
-def _parse_response(*, client: Client, response: httpx.Response) -> Optional[CreatePersonalAccessTokenResponse200]:
+def _parse_response(*, client: Client, response: httpx.Response) -> Optional[ApiUserAllowedOrganizationsResponse]:
     if response.status_code == HTTPStatus.OK:
-        response_200 = CreatePersonalAccessTokenResponse200.from_dict(response.json())
+        response_200 = ApiUserAllowedOrganizationsResponse.from_dict(response.json())
 
         return response_200
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
-def _build_response(*, client: Client, response: httpx.Response) -> Response[CreatePersonalAccessTokenResponse200]:
+def _build_response(*, client: Client, response: httpx.Response) -> Response[ApiUserAllowedOrganizationsResponse]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
     *,
     client: Client,
-    json_body: CreatePersonalAccessToken,
-) -> Response[CreatePersonalAccessTokenResponse200]:
-    """Create a personal access token
-
-    Args:
-        json_body (CreatePersonalAccessToken):
+) -> Response[ApiUserAllowedOrganizationsResponse]:
+    """List the organizations that the current user can join.
+    This is based on the user's primary email domain and the organization's allowed email domains.
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[CreatePersonalAccessTokenResponse200]
+        Response[ApiUserAllowedOrganizationsResponse]
     """
 
     kwargs = _get_kwargs(
         client=client,
-        json_body=json_body,
     )
 
     response = httpx.request(
         verify=client.verify_ssl,
         **kwargs,
     )
 
     return _build_response(client=client, response=response)
 
 
 def sync(
     *,
     client: Client,
-    json_body: CreatePersonalAccessToken,
-) -> Optional[CreatePersonalAccessTokenResponse200]:
-    """Create a personal access token
-
-    Args:
-        json_body (CreatePersonalAccessToken):
+) -> Optional[ApiUserAllowedOrganizationsResponse]:
+    """List the organizations that the current user can join.
+    This is based on the user's primary email domain and the organization's allowed email domains.
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        CreatePersonalAccessTokenResponse200
+        ApiUserAllowedOrganizationsResponse
     """
 
     return sync_detailed(
         client=client,
-        json_body=json_body,
     ).parsed
 
 
 async def asyncio_detailed(
     *,
     client: Client,
-    json_body: CreatePersonalAccessToken,
-) -> Response[CreatePersonalAccessTokenResponse200]:
-    """Create a personal access token
-
-    Args:
-        json_body (CreatePersonalAccessToken):
+) -> Response[ApiUserAllowedOrganizationsResponse]:
+    """List the organizations that the current user can join.
+    This is based on the user's primary email domain and the organization's allowed email domains.
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[CreatePersonalAccessTokenResponse200]
+        Response[ApiUserAllowedOrganizationsResponse]
     """
 
     kwargs = _get_kwargs(
         client=client,
-        json_body=json_body,
     )
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
         response = await _client.request(**kwargs)
 
     return _build_response(client=client, response=response)
 
 
 async def asyncio(
     *,
     client: Client,
-    json_body: CreatePersonalAccessToken,
-) -> Optional[CreatePersonalAccessTokenResponse200]:
-    """Create a personal access token
-
-    Args:
-        json_body (CreatePersonalAccessToken):
+) -> Optional[ApiUserAllowedOrganizationsResponse]:
+    """List the organizations that the current user can join.
+    This is based on the user's primary email domain and the organization's allowed email domains.
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        CreatePersonalAccessTokenResponse200
+        ApiUserAllowedOrganizationsResponse
     """
 
     return (
         await asyncio_detailed(
             client=client,
-            json_body=json_body,
         )
     ).parsed
```

### Comparing `lightdash_client_python-0.1.2/lightdash_client/api/user/create_user.py` & `lightdash_client_python-0.611.0/lightdash_client/api/schedulers/get_scheduler_job_status.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,163 +3,163 @@
 from typing import Dict
 from typing import Optional
 
 import httpx
 
 from ... import errors
 from ...client import Client
-from ...models.create_user import CreateUser
-from ...models.create_user_response_201 import CreateUserResponse201
+from ...models.api_job_status_response import ApiJobStatusResponse
 from ...types import Response
 
 
 def _get_kwargs(
+    job_id: str,
     *,
     client: Client,
-    json_body: CreateUser,
 ) -> Dict[str, Any]:
-    url = "{}/user".format(client.base_url)
+    url = "{}/api/v1/schedulers/job/{jobId}/status".format(client.base_url, jobId=job_id)
 
     headers: Dict[str, str] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
-    json_json_body = json_body.to_dict()
-
     return {
-        "method": "post",
+        "method": "get",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
         "follow_redirects": client.follow_redirects,
-        "json": json_json_body,
     }
 
 
-def _parse_response(*, client: Client, response: httpx.Response) -> Optional[CreateUserResponse201]:
-    if response.status_code == HTTPStatus.CREATED:
-        response_201 = CreateUserResponse201.from_dict(response.json())
+def _parse_response(*, client: Client, response: httpx.Response) -> Optional[ApiJobStatusResponse]:
+    if response.status_code == HTTPStatus.OK:
+        response_200 = ApiJobStatusResponse.from_dict(response.json())
 
-        return response_201
+        return response_200
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
-def _build_response(*, client: Client, response: httpx.Response) -> Response[CreateUserResponse201]:
+def _build_response(*, client: Client, response: httpx.Response) -> Response[ApiJobStatusResponse]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
+    job_id: str,
     *,
     client: Client,
-    json_body: CreateUser,
-) -> Response[CreateUserResponse201]:
-    """Create user
+) -> Response[ApiJobStatusResponse]:
+    """Get a generic job status
+    This method can be used when polling from the frontend
 
     Args:
-        json_body (CreateUser):
+        job_id (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[CreateUserResponse201]
+        Response[ApiJobStatusResponse]
     """
 
     kwargs = _get_kwargs(
+        job_id=job_id,
         client=client,
-        json_body=json_body,
     )
 
     response = httpx.request(
         verify=client.verify_ssl,
         **kwargs,
     )
 
     return _build_response(client=client, response=response)
 
 
 def sync(
+    job_id: str,
     *,
     client: Client,
-    json_body: CreateUser,
-) -> Optional[CreateUserResponse201]:
-    """Create user
+) -> Optional[ApiJobStatusResponse]:
+    """Get a generic job status
+    This method can be used when polling from the frontend
 
     Args:
-        json_body (CreateUser):
+        job_id (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        CreateUserResponse201
+        ApiJobStatusResponse
     """
 
     return sync_detailed(
+        job_id=job_id,
         client=client,
-        json_body=json_body,
     ).parsed
 
 
 async def asyncio_detailed(
+    job_id: str,
     *,
     client: Client,
-    json_body: CreateUser,
-) -> Response[CreateUserResponse201]:
-    """Create user
+) -> Response[ApiJobStatusResponse]:
+    """Get a generic job status
+    This method can be used when polling from the frontend
 
     Args:
-        json_body (CreateUser):
+        job_id (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[CreateUserResponse201]
+        Response[ApiJobStatusResponse]
     """
 
     kwargs = _get_kwargs(
+        job_id=job_id,
         client=client,
-        json_body=json_body,
     )
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
         response = await _client.request(**kwargs)
 
     return _build_response(client=client, response=response)
 
 
 async def asyncio(
+    job_id: str,
     *,
     client: Client,
-    json_body: CreateUser,
-) -> Optional[CreateUserResponse201]:
-    """Create user
+) -> Optional[ApiJobStatusResponse]:
+    """Get a generic job status
+    This method can be used when polling from the frontend
 
     Args:
-        json_body (CreateUser):
+        job_id (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        CreateUserResponse201
+        ApiJobStatusResponse
     """
 
     return (
         await asyncio_detailed(
+            job_id=job_id,
             client=client,
-            json_body=json_body,
         )
     ).parsed
```

### Comparing `lightdash_client_python-0.1.2/lightdash_client/api/user/delete_invite_links.py` & `lightdash_client_python-0.611.0/lightdash_client/api/integrations/get_slack_channels.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,95 +3,138 @@
 from typing import Dict
 from typing import Optional
 
 import httpx
 
 from ... import errors
 from ...client import Client
+from ...models.api_slack_channels_response import ApiSlackChannelsResponse
 from ...types import Response
 
 
 def _get_kwargs(
     *,
     client: Client,
 ) -> Dict[str, Any]:
-    url = "{}/invite-links".format(client.base_url)
+    url = "{}/api/v1/slack/channels".format(client.base_url)
 
     headers: Dict[str, str] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     return {
-        "method": "delete",
+        "method": "get",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
         "follow_redirects": client.follow_redirects,
     }
 
 
-def _parse_response(*, client: Client, response: httpx.Response) -> Optional[Any]:
+def _parse_response(*, client: Client, response: httpx.Response) -> Optional[ApiSlackChannelsResponse]:
     if response.status_code == HTTPStatus.OK:
-        return None
+        response_200 = ApiSlackChannelsResponse.from_dict(response.json())
+
+        return response_200
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
-def _build_response(*, client: Client, response: httpx.Response) -> Response[Any]:
+def _build_response(*, client: Client, response: httpx.Response) -> Response[ApiSlackChannelsResponse]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
     *,
     client: Client,
-) -> Response[Any]:
-    """Delete all invite links
+) -> Response[ApiSlackChannelsResponse]:
+    """Get slack channels
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Any]
+        Response[ApiSlackChannelsResponse]
     """
 
     kwargs = _get_kwargs(
         client=client,
     )
 
     response = httpx.request(
         verify=client.verify_ssl,
         **kwargs,
     )
 
     return _build_response(client=client, response=response)
 
 
+def sync(
+    *,
+    client: Client,
+) -> Optional[ApiSlackChannelsResponse]:
+    """Get slack channels
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
+    Returns:
+        ApiSlackChannelsResponse
+    """
+
+    return sync_detailed(
+        client=client,
+    ).parsed
+
+
 async def asyncio_detailed(
     *,
     client: Client,
-) -> Response[Any]:
-    """Delete all invite links
+) -> Response[ApiSlackChannelsResponse]:
+    """Get slack channels
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Any]
+        Response[ApiSlackChannelsResponse]
     """
 
     kwargs = _get_kwargs(
         client=client,
     )
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
         response = await _client.request(**kwargs)
 
     return _build_response(client=client, response=response)
+
+
+async def asyncio(
+    *,
+    client: Client,
+) -> Optional[ApiSlackChannelsResponse]:
+    """Get slack channels
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
+    Returns:
+        ApiSlackChannelsResponse
+    """
+
+    return (
+        await asyncio_detailed(
+            client=client,
+        )
+    ).parsed
```

### Comparing `lightdash_client_python-0.1.2/lightdash_client/api/user/get_invite_link.py` & `lightdash_client_python-0.611.0/lightdash_client/api/ssh_keypairs/create_ssh_key_pair.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,159 +3,134 @@
 from typing import Dict
 from typing import Optional
 
 import httpx
 
 from ... import errors
 from ...client import Client
-from ...models.get_invite_link_response_200 import GetInviteLinkResponse200
+from ...models.api_ssh_key_pair_response import ApiSshKeyPairResponse
 from ...types import Response
 
 
 def _get_kwargs(
-    invite_link_id: str,
     *,
     client: Client,
 ) -> Dict[str, Any]:
-    url = "{}/invite-links/{inviteLinkId}".format(client.base_url, inviteLinkId=invite_link_id)
+    url = "{}/api/v1/ssh/key-pairs".format(client.base_url)
 
     headers: Dict[str, str] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     return {
-        "method": "get",
+        "method": "post",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
         "follow_redirects": client.follow_redirects,
     }
 
 
-def _parse_response(*, client: Client, response: httpx.Response) -> Optional[GetInviteLinkResponse200]:
-    if response.status_code == HTTPStatus.OK:
-        response_200 = GetInviteLinkResponse200.from_dict(response.json())
+def _parse_response(*, client: Client, response: httpx.Response) -> Optional[ApiSshKeyPairResponse]:
+    if response.status_code == HTTPStatus.CREATED:
+        response_201 = ApiSshKeyPairResponse.from_dict(response.json())
 
-        return response_200
+        return response_201
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
-def _build_response(*, client: Client, response: httpx.Response) -> Response[GetInviteLinkResponse200]:
+def _build_response(*, client: Client, response: httpx.Response) -> Response[ApiSshKeyPairResponse]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
-    invite_link_id: str,
     *,
     client: Client,
-) -> Response[GetInviteLinkResponse200]:
-    """Get an invite link
-
-    Args:
-        invite_link_id (str):
-
+) -> Response[ApiSshKeyPairResponse]:
+    """
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[GetInviteLinkResponse200]
+        Response[ApiSshKeyPairResponse]
     """
 
     kwargs = _get_kwargs(
-        invite_link_id=invite_link_id,
         client=client,
     )
 
     response = httpx.request(
         verify=client.verify_ssl,
         **kwargs,
     )
 
     return _build_response(client=client, response=response)
 
 
 def sync(
-    invite_link_id: str,
     *,
     client: Client,
-) -> Optional[GetInviteLinkResponse200]:
-    """Get an invite link
-
-    Args:
-        invite_link_id (str):
-
+) -> Optional[ApiSshKeyPairResponse]:
+    """
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        GetInviteLinkResponse200
+        ApiSshKeyPairResponse
     """
 
     return sync_detailed(
-        invite_link_id=invite_link_id,
         client=client,
     ).parsed
 
 
 async def asyncio_detailed(
-    invite_link_id: str,
     *,
     client: Client,
-) -> Response[GetInviteLinkResponse200]:
-    """Get an invite link
-
-    Args:
-        invite_link_id (str):
-
+) -> Response[ApiSshKeyPairResponse]:
+    """
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[GetInviteLinkResponse200]
+        Response[ApiSshKeyPairResponse]
     """
 
     kwargs = _get_kwargs(
-        invite_link_id=invite_link_id,
         client=client,
     )
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
         response = await _client.request(**kwargs)
 
     return _build_response(client=client, response=response)
 
 
 async def asyncio(
-    invite_link_id: str,
     *,
     client: Client,
-) -> Optional[GetInviteLinkResponse200]:
-    """Get an invite link
-
-    Args:
-        invite_link_id (str):
-
+) -> Optional[ApiSshKeyPairResponse]:
+    """
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        GetInviteLinkResponse200
+        ApiSshKeyPairResponse
     """
 
     return (
         await asyncio_detailed(
-            invite_link_id=invite_link_id,
             client=client,
         )
     ).parsed
```

### Comparing `lightdash_client_python-0.1.2/lightdash_client/api/user/get_personal_access_tokens.py` & `lightdash_client_python-0.611.0/lightdash_client/api/projects/list_spaces_in_project.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,146 +3,159 @@
 from typing import Dict
 from typing import Optional
 
 import httpx
 
 from ... import errors
 from ...client import Client
-from ...models.get_personal_access_tokens_response_200 import GetPersonalAccessTokensResponse200
+from ...models.api_space_summary_list_response import ApiSpaceSummaryListResponse
 from ...types import Response
 
 
 def _get_kwargs(
+    project_uuid: str,
     *,
     client: Client,
 ) -> Dict[str, Any]:
-    url = "{}/user/me/personal-access-tokens".format(client.base_url)
+    url = "{}/api/v1/projects/{projectUuid}/spaces".format(client.base_url, projectUuid=project_uuid)
 
     headers: Dict[str, str] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     return {
         "method": "get",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
         "follow_redirects": client.follow_redirects,
     }
 
 
-def _parse_response(*, client: Client, response: httpx.Response) -> Optional[GetPersonalAccessTokensResponse200]:
+def _parse_response(*, client: Client, response: httpx.Response) -> Optional[ApiSpaceSummaryListResponse]:
     if response.status_code == HTTPStatus.OK:
-        response_200 = GetPersonalAccessTokensResponse200.from_dict(response.json())
+        response_200 = ApiSpaceSummaryListResponse.from_dict(response.json())
 
         return response_200
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
-def _build_response(*, client: Client, response: httpx.Response) -> Response[GetPersonalAccessTokensResponse200]:
+def _build_response(*, client: Client, response: httpx.Response) -> Response[ApiSpaceSummaryListResponse]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
+    project_uuid: str,
     *,
     client: Client,
-) -> Response[GetPersonalAccessTokensResponse200]:
-    """Get all personal access tokens
+) -> Response[ApiSpaceSummaryListResponse]:
+    """List all spaces in a project
 
-     List all personal access tokens for user
+    Args:
+        project_uuid (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[GetPersonalAccessTokensResponse200]
+        Response[ApiSpaceSummaryListResponse]
     """
 
     kwargs = _get_kwargs(
+        project_uuid=project_uuid,
         client=client,
     )
 
     response = httpx.request(
         verify=client.verify_ssl,
         **kwargs,
     )
 
     return _build_response(client=client, response=response)
 
 
 def sync(
+    project_uuid: str,
     *,
     client: Client,
-) -> Optional[GetPersonalAccessTokensResponse200]:
-    """Get all personal access tokens
+) -> Optional[ApiSpaceSummaryListResponse]:
+    """List all spaces in a project
 
-     List all personal access tokens for user
+    Args:
+        project_uuid (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        GetPersonalAccessTokensResponse200
+        ApiSpaceSummaryListResponse
     """
 
     return sync_detailed(
+        project_uuid=project_uuid,
         client=client,
     ).parsed
 
 
 async def asyncio_detailed(
+    project_uuid: str,
     *,
     client: Client,
-) -> Response[GetPersonalAccessTokensResponse200]:
-    """Get all personal access tokens
+) -> Response[ApiSpaceSummaryListResponse]:
+    """List all spaces in a project
 
-     List all personal access tokens for user
+    Args:
+        project_uuid (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[GetPersonalAccessTokensResponse200]
+        Response[ApiSpaceSummaryListResponse]
     """
 
     kwargs = _get_kwargs(
+        project_uuid=project_uuid,
         client=client,
     )
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
         response = await _client.request(**kwargs)
 
     return _build_response(client=client, response=response)
 
 
 async def asyncio(
+    project_uuid: str,
     *,
     client: Client,
-) -> Optional[GetPersonalAccessTokensResponse200]:
-    """Get all personal access tokens
+) -> Optional[ApiSpaceSummaryListResponse]:
+    """List all spaces in a project
 
-     List all personal access tokens for user
+    Args:
+        project_uuid (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        GetPersonalAccessTokensResponse200
+        ApiSpaceSummaryListResponse
     """
 
     return (
         await asyncio_detailed(
+            project_uuid=project_uuid,
             client=client,
         )
     ).parsed
```

### Comparing `lightdash_client_python-0.1.2/lightdash_client/api/user/get_user.py` & `lightdash_client_python-0.611.0/lightdash_client/api/schedulers/get_scheduler.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,138 +3,104 @@
 from typing import Dict
 from typing import Optional
 
 import httpx
 
 from ... import errors
 from ...client import Client
-from ...models.get_user_response_200 import GetUserResponse200
 from ...types import Response
 
 
 def _get_kwargs(
+    scheduler_uuid: str,
     *,
     client: Client,
 ) -> Dict[str, Any]:
-    url = "{}/user".format(client.base_url)
+    url = "{}/api/v1/schedulers/{schedulerUuid}".format(client.base_url, schedulerUuid=scheduler_uuid)
 
     headers: Dict[str, str] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     return {
         "method": "get",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
         "follow_redirects": client.follow_redirects,
     }
 
 
-def _parse_response(*, client: Client, response: httpx.Response) -> Optional[GetUserResponse200]:
-    if response.status_code == HTTPStatus.OK:
-        response_200 = GetUserResponse200.from_dict(response.json())
-
-        return response_200
+def _parse_response(*, client: Client, response: httpx.Response) -> Optional[Any]:
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
-def _build_response(*, client: Client, response: httpx.Response) -> Response[GetUserResponse200]:
+def _build_response(*, client: Client, response: httpx.Response) -> Response[Any]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
+    scheduler_uuid: str,
     *,
     client: Client,
-) -> Response[GetUserResponse200]:
-    """Get user profile
+) -> Response[Any]:
+    """Get a scheduler
+
+    Args:
+        scheduler_uuid (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[GetUserResponse200]
+        Response[Any]
     """
 
     kwargs = _get_kwargs(
+        scheduler_uuid=scheduler_uuid,
         client=client,
     )
 
     response = httpx.request(
         verify=client.verify_ssl,
         **kwargs,
     )
 
     return _build_response(client=client, response=response)
 
 
-def sync(
-    *,
-    client: Client,
-) -> Optional[GetUserResponse200]:
-    """Get user profile
-
-    Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
-        httpx.TimeoutException: If the request takes longer than Client.timeout.
-
-    Returns:
-        GetUserResponse200
-    """
-
-    return sync_detailed(
-        client=client,
-    ).parsed
-
-
 async def asyncio_detailed(
+    scheduler_uuid: str,
     *,
     client: Client,
-) -> Response[GetUserResponse200]:
-    """Get user profile
+) -> Response[Any]:
+    """Get a scheduler
+
+    Args:
+        scheduler_uuid (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[GetUserResponse200]
+        Response[Any]
     """
 
     kwargs = _get_kwargs(
+        scheduler_uuid=scheduler_uuid,
         client=client,
     )
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
         response = await _client.request(**kwargs)
 
     return _build_response(client=client, response=response)
-
-
-async def asyncio(
-    *,
-    client: Client,
-) -> Optional[GetUserResponse200]:
-    """Get user profile
-
-    Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
-        httpx.TimeoutException: If the request takes longer than Client.timeout.
-
-    Returns:
-        GetUserResponse200
-    """
-
-    return (
-        await asyncio_detailed(
-            client=client,
-        )
-    ).parsed
```

### Comparing `lightdash_client_python-0.1.2/lightdash_client/api/user/login_with_password.py` & `lightdash_client_python-0.611.0/lightdash_client/api/projects/list_charts_in_project.py`

 * *Files 19% similar despite different names*

```diff
@@ -3,163 +3,159 @@
 from typing import Dict
 from typing import Optional
 
 import httpx
 
 from ... import errors
 from ...client import Client
-from ...models.login import Login
-from ...models.success import Success
+from ...models.api_chart_summary_list_response import ApiChartSummaryListResponse
 from ...types import Response
 
 
 def _get_kwargs(
+    project_uuid: str,
     *,
     client: Client,
-    json_body: Login,
 ) -> Dict[str, Any]:
-    url = "{}/login".format(client.base_url)
+    url = "{}/api/v1/projects/{projectUuid}/charts".format(client.base_url, projectUuid=project_uuid)
 
     headers: Dict[str, str] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
-    json_json_body = json_body.to_dict()
-
     return {
-        "method": "post",
+        "method": "get",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
         "follow_redirects": client.follow_redirects,
-        "json": json_json_body,
     }
 
 
-def _parse_response(*, client: Client, response: httpx.Response) -> Optional[Success]:
+def _parse_response(*, client: Client, response: httpx.Response) -> Optional[ApiChartSummaryListResponse]:
     if response.status_code == HTTPStatus.OK:
-        response_200 = Success.from_dict(response.json())
+        response_200 = ApiChartSummaryListResponse.from_dict(response.json())
 
         return response_200
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
-def _build_response(*, client: Client, response: httpx.Response) -> Response[Success]:
+def _build_response(*, client: Client, response: httpx.Response) -> Response[ApiChartSummaryListResponse]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
+    project_uuid: str,
     *,
     client: Client,
-    json_body: Login,
-) -> Response[Success]:
-    """Login with email and password
+) -> Response[ApiChartSummaryListResponse]:
+    """List all charts in a project
 
     Args:
-        json_body (Login):
+        project_uuid (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Success]
+        Response[ApiChartSummaryListResponse]
     """
 
     kwargs = _get_kwargs(
+        project_uuid=project_uuid,
         client=client,
-        json_body=json_body,
     )
 
     response = httpx.request(
         verify=client.verify_ssl,
         **kwargs,
     )
 
     return _build_response(client=client, response=response)
 
 
 def sync(
+    project_uuid: str,
     *,
     client: Client,
-    json_body: Login,
-) -> Optional[Success]:
-    """Login with email and password
+) -> Optional[ApiChartSummaryListResponse]:
+    """List all charts in a project
 
     Args:
-        json_body (Login):
+        project_uuid (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Success
+        ApiChartSummaryListResponse
     """
 
     return sync_detailed(
+        project_uuid=project_uuid,
         client=client,
-        json_body=json_body,
     ).parsed
 
 
 async def asyncio_detailed(
+    project_uuid: str,
     *,
     client: Client,
-    json_body: Login,
-) -> Response[Success]:
-    """Login with email and password
+) -> Response[ApiChartSummaryListResponse]:
+    """List all charts in a project
 
     Args:
-        json_body (Login):
+        project_uuid (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Success]
+        Response[ApiChartSummaryListResponse]
     """
 
     kwargs = _get_kwargs(
+        project_uuid=project_uuid,
         client=client,
-        json_body=json_body,
     )
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
         response = await _client.request(**kwargs)
 
     return _build_response(client=client, response=response)
 
 
 async def asyncio(
+    project_uuid: str,
     *,
     client: Client,
-    json_body: Login,
-) -> Optional[Success]:
-    """Login with email and password
+) -> Optional[ApiChartSummaryListResponse]:
+    """List all charts in a project
 
     Args:
-        json_body (Login):
+        project_uuid (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Success
+        ApiChartSummaryListResponse
     """
 
     return (
         await asyncio_detailed(
+            project_uuid=project_uuid,
             client=client,
-            json_body=json_body,
         )
     ).parsed
```

### Comparing `lightdash_client_python-0.1.2/lightdash_client/client.py` & `lightdash_client_python-0.611.0/lightdash_client/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,14 +54,15 @@
 
 
 @attr.s(auto_attribs=True)
 class AuthenticatedClient(Client):
     """A Client which has been authenticated for use on secured endpoints"""
 
     token: str
+    # The prefix was manually changed from the default value 'Bearer'.
     prefix: str = "ApiKey"
     auth_header_name: str = "Authorization"
 
     def get_headers(self) -> Dict[str, str]:
         """Get headers to be used in authenticated endpoints"""
         auth_header_value = f"{self.prefix} {self.token}" if self.prefix else self.token
         return {self.auth_header_name: auth_header_value, **self.headers}
```

### Comparing `lightdash_client_python-0.1.2/lightdash_client/models/chart_config.py` & `lightdash_client_python-0.611.0/lightdash_client/models/api_organization_allowed_email_domains.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,87 +1,69 @@
 from typing import Any
 from typing import Dict
 from typing import List
 from typing import Type
 from typing import TYPE_CHECKING
 from typing import TypeVar
-from typing import Union
 
 import attr
 
-from ..models.chart_config_chart_type import ChartConfigChartType
-from ..types import UNSET
-from ..types import Unset
+from ..models.api_organization_allowed_email_domains_status import ApiOrganizationAllowedEmailDomainsStatus
 
 if TYPE_CHECKING:
-    from ..models.chart_config_config import ChartConfigConfig
+    from ..models.allowed_email_domains import AllowedEmailDomains
 
 
-T = TypeVar("T", bound="ChartConfig")
+T = TypeVar("T", bound="ApiOrganizationAllowedEmailDomains")
 
 
 @attr.s(auto_attribs=True)
-class ChartConfig:
+class ApiOrganizationAllowedEmailDomains:
     """
     Attributes:
-        chart_type (Union[Unset, ChartConfigChartType]):
-        config (Union[Unset, None, ChartConfigConfig]):
+        results (AllowedEmailDomains):
+        status (ApiOrganizationAllowedEmailDomainsStatus):
     """
 
-    chart_type: Union[Unset, ChartConfigChartType] = UNSET
-    config: Union[Unset, None, "ChartConfigConfig"] = UNSET
+    results: "AllowedEmailDomains"
+    status: ApiOrganizationAllowedEmailDomainsStatus
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
-        chart_type: Union[Unset, str] = UNSET
-        if not isinstance(self.chart_type, Unset):
-            chart_type = self.chart_type.value
-
-        config: Union[Unset, None, Dict[str, Any]] = UNSET
-        if not isinstance(self.config, Unset):
-            config = self.config.to_dict() if self.config else None
+        results = self.results.to_dict()
+
+        status = self.status.value
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
-        field_dict.update({})
-        if chart_type is not UNSET:
-            field_dict["chartType"] = chart_type
-        if config is not UNSET:
-            field_dict["config"] = config
+        field_dict.update(
+            {
+                "results": results,
+                "status": status,
+            }
+        )
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        from ..models.chart_config_config import ChartConfigConfig
+        from ..models.allowed_email_domains import AllowedEmailDomains
 
         d = src_dict.copy()
-        _chart_type = d.pop("chartType", UNSET)
-        chart_type: Union[Unset, ChartConfigChartType]
-        if isinstance(_chart_type, Unset):
-            chart_type = UNSET
-        else:
-            chart_type = ChartConfigChartType(_chart_type)
-
-        _config = d.pop("config", UNSET)
-        config: Union[Unset, None, ChartConfigConfig]
-        if _config is None:
-            config = None
-        elif isinstance(_config, Unset):
-            config = UNSET
-        else:
-            config = ChartConfigConfig.from_dict(_config)
-
-        chart_config = cls(
-            chart_type=chart_type,
-            config=config,
+        results = AllowedEmailDomains.from_dict(d.pop("results"))
+
+        status = ApiOrganizationAllowedEmailDomainsStatus(d.pop("status"))
+
+        api_organization_allowed_email_domains = cls(
+            results=results,
+            status=status,
         )
 
-        chart_config.additional_properties = d
-        return chart_config
+        api_organization_allowed_email_domains.additional_properties = d
+        return api_organization_allowed_email_domains
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `lightdash_client_python-0.1.2/lightdash_client/models/chart_config_config.py` & `lightdash_client_python-0.611.0/lightdash_client/models/record_string_any.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,37 +2,37 @@
 from typing import Dict
 from typing import List
 from typing import Type
 from typing import TypeVar
 
 import attr
 
-T = TypeVar("T", bound="ChartConfigConfig")
+T = TypeVar("T", bound="RecordStringAny")
 
 
 @attr.s(auto_attribs=True)
-class ChartConfigConfig:
-    """ """
+class RecordStringAny:
+    """Construct a type with a set of properties K of type T"""
 
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({})
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
-        chart_config_config = cls()
+        record_string_any = cls()
 
-        chart_config_config.additional_properties = d
-        return chart_config_config
+        record_string_any.additional_properties = d
+        return record_string_any
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `lightdash_client_python-0.1.2/lightdash_client/models/create_invite_link.py` & `lightdash_client_python-0.611.0/lightdash_client/models/scheduled_jobs.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,51 +4,58 @@
 from typing import List
 from typing import Type
 from typing import TypeVar
 
 import attr
 from dateutil.parser import isoparse
 
-T = TypeVar("T", bound="CreateInviteLink")
+T = TypeVar("T", bound="ScheduledJobs")
 
 
 @attr.s(auto_attribs=True)
-class CreateInviteLink:
+class ScheduledJobs:
     """
     Attributes:
-        expires_at (datetime.datetime):
+        id (str):
+        date (datetime.datetime):
     """
 
-    expires_at: datetime.datetime
+    id: str
+    date: datetime.datetime
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
-        expires_at = self.expires_at.isoformat()
+        id = self.id
+        date = self.date.isoformat()
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update(
             {
-                "expiresAt": expires_at,
+                "id": id,
+                "date": date,
             }
         )
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
-        expires_at = isoparse(d.pop("expiresAt"))
+        id = d.pop("id")
 
-        create_invite_link = cls(
-            expires_at=expires_at,
+        date = isoparse(d.pop("date"))
+
+        scheduled_jobs = cls(
+            id=id,
+            date=date,
         )
 
-        create_invite_link.additional_properties = d
-        return create_invite_link
+        scheduled_jobs.additional_properties = d
+        return scheduled_jobs
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `lightdash_client_python-0.1.2/lightdash_client/models/create_invite_link_response_201.py` & `lightdash_client_python-0.611.0/lightdash_client/models/api_dbt_cloud_settings_delete_success.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,80 +1,66 @@
 from typing import Any
 from typing import Dict
 from typing import List
 from typing import Type
-from typing import TYPE_CHECKING
 from typing import TypeVar
 from typing import Union
 
 import attr
 
-from ..models.success_status import SuccessStatus
+from ..models.api_dbt_cloud_settings_delete_success_status import ApiDbtCloudSettingsDeleteSuccessStatus
 from ..types import UNSET
 from ..types import Unset
 
-if TYPE_CHECKING:
-    from ..models.invite_link import InviteLink
-
-
-T = TypeVar("T", bound="CreateInviteLinkResponse201")
+T = TypeVar("T", bound="ApiDbtCloudSettingsDeleteSuccess")
 
 
 @attr.s(auto_attribs=True)
-class CreateInviteLinkResponse201:
+class ApiDbtCloudSettingsDeleteSuccess:
     """
     Attributes:
-        results (InviteLink):
-        status (Union[Unset, SuccessStatus]):
+        status (ApiDbtCloudSettingsDeleteSuccessStatus):
+        results (Union[Unset, Any]):
     """
 
-    results: "InviteLink"
-    status: Union[Unset, SuccessStatus] = UNSET
+    status: ApiDbtCloudSettingsDeleteSuccessStatus
+    results: Union[Unset, Any] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
-        results = self.results.to_dict()
+        status = self.status.value
 
-        status: Union[Unset, str] = UNSET
-        if not isinstance(self.status, Unset):
-            status = self.status.value
+        results = self.results
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update(
             {
-                "results": results,
+                "status": status,
             }
         )
-        if status is not UNSET:
-            field_dict["status"] = status
+        if results is not UNSET:
+            field_dict["results"] = results
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        from ..models.invite_link import InviteLink
-
         d = src_dict.copy()
-        results = InviteLink.from_dict(d.pop("results"))
+        status = ApiDbtCloudSettingsDeleteSuccessStatus(d.pop("status"))
 
-        _status = d.pop("status", UNSET)
-        status: Union[Unset, SuccessStatus]
-        if isinstance(_status, Unset):
-            status = UNSET
-        else:
-            status = SuccessStatus(_status)
+        results = d.pop("results", UNSET)
 
-        create_invite_link_response_201 = cls(
-            results=results,
+        api_dbt_cloud_settings_delete_success = cls(
             status=status,
+            results=results,
         )
 
-        create_invite_link_response_201.additional_properties = d
-        return create_invite_link_response_201
+        api_dbt_cloud_settings_delete_success.additional_properties = d
+        return api_dbt_cloud_settings_delete_success
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `lightdash_client_python-0.1.2/lightdash_client/models/create_personal_access_token.py` & `lightdash_client_python-0.611.0/lightdash_client/models/partial_pick_organization_member_profile_role.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,73 +1,63 @@
-import datetime
 from typing import Any
 from typing import Dict
 from typing import List
 from typing import Type
 from typing import TypeVar
 from typing import Union
 
 import attr
-from dateutil.parser import isoparse
 
+from ..models.organization_member_role import OrganizationMemberRole
 from ..types import UNSET
 from ..types import Unset
 
-T = TypeVar("T", bound="CreatePersonalAccessToken")
+T = TypeVar("T", bound="PartialPickOrganizationMemberProfileRole")
 
 
 @attr.s(auto_attribs=True)
-class CreatePersonalAccessToken:
-    """
+class PartialPickOrganizationMemberProfileRole:
+    """Make all properties in T optional
+
     Attributes:
-        description (str):
-        expires_at (Union[Unset, datetime.datetime]):
+        role (Union[Unset, OrganizationMemberRole]):
     """
 
-    description: str
-    expires_at: Union[Unset, datetime.datetime] = UNSET
+    role: Union[Unset, OrganizationMemberRole] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
-        description = self.description
-        expires_at: Union[Unset, str] = UNSET
-        if not isinstance(self.expires_at, Unset):
-            expires_at = self.expires_at.isoformat()
+        role: Union[Unset, str] = UNSET
+        if not isinstance(self.role, Unset):
+            role = self.role.value
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
-        field_dict.update(
-            {
-                "description": description,
-            }
-        )
-        if expires_at is not UNSET:
-            field_dict["expiresAt"] = expires_at
+        field_dict.update({})
+        if role is not UNSET:
+            field_dict["role"] = role
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
-        description = d.pop("description")
-
-        _expires_at = d.pop("expiresAt", UNSET)
-        expires_at: Union[Unset, datetime.datetime]
-        if isinstance(_expires_at, Unset):
-            expires_at = UNSET
+        _role = d.pop("role", UNSET)
+        role: Union[Unset, OrganizationMemberRole]
+        if isinstance(_role, Unset):
+            role = UNSET
         else:
-            expires_at = isoparse(_expires_at)
+            role = OrganizationMemberRole(_role)
 
-        create_personal_access_token = cls(
-            description=description,
-            expires_at=expires_at,
+        partial_pick_organization_member_profile_role = cls(
+            role=role,
         )
 
-        create_personal_access_token.additional_properties = d
-        return create_personal_access_token
+        partial_pick_organization_member_profile_role.additional_properties = d
+        return partial_pick_organization_member_profile_role
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `lightdash_client_python-0.1.2/lightdash_client/models/create_personal_access_token_response_200.py` & `lightdash_client_python-0.611.0/lightdash_client/models/api_ssh_key_pair_response.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,80 +1,69 @@
 from typing import Any
 from typing import Dict
 from typing import List
 from typing import Type
 from typing import TYPE_CHECKING
 from typing import TypeVar
-from typing import Union
 
 import attr
 
-from ..models.success_status import SuccessStatus
-from ..types import UNSET
-from ..types import Unset
+from ..models.api_ssh_key_pair_response_status import ApiSshKeyPairResponseStatus
 
 if TYPE_CHECKING:
-    from ..models.personal_access_token_with_secret import PersonalAccessTokenWithSecret
+    from ..models.pick_ssh_key_pair_public_key import PickSshKeyPairPublicKey
 
 
-T = TypeVar("T", bound="CreatePersonalAccessTokenResponse200")
+T = TypeVar("T", bound="ApiSshKeyPairResponse")
 
 
 @attr.s(auto_attribs=True)
-class CreatePersonalAccessTokenResponse200:
+class ApiSshKeyPairResponse:
     """
     Attributes:
-        results (PersonalAccessTokenWithSecret):
-        status (Union[Unset, SuccessStatus]):
+        results (PickSshKeyPairPublicKey): From T, pick a set of properties whose keys are in the union K
+        status (ApiSshKeyPairResponseStatus):
     """
 
-    results: "PersonalAccessTokenWithSecret"
-    status: Union[Unset, SuccessStatus] = UNSET
+    results: "PickSshKeyPairPublicKey"
+    status: ApiSshKeyPairResponseStatus
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         results = self.results.to_dict()
 
-        status: Union[Unset, str] = UNSET
-        if not isinstance(self.status, Unset):
-            status = self.status.value
+        status = self.status.value
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update(
             {
                 "results": results,
+                "status": status,
             }
         )
-        if status is not UNSET:
-            field_dict["status"] = status
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        from ..models.personal_access_token_with_secret import PersonalAccessTokenWithSecret
+        from ..models.pick_ssh_key_pair_public_key import PickSshKeyPairPublicKey
 
         d = src_dict.copy()
-        results = PersonalAccessTokenWithSecret.from_dict(d.pop("results"))
+        results = PickSshKeyPairPublicKey.from_dict(d.pop("results"))
 
-        _status = d.pop("status", UNSET)
-        status: Union[Unset, SuccessStatus]
-        if isinstance(_status, Unset):
-            status = UNSET
-        else:
-            status = SuccessStatus(_status)
+        status = ApiSshKeyPairResponseStatus(d.pop("status"))
 
-        create_personal_access_token_response_200 = cls(
+        api_ssh_key_pair_response = cls(
             results=results,
             status=status,
         )
 
-        create_personal_access_token_response_200.additional_properties = d
-        return create_personal_access_token_response_200
+        api_ssh_key_pair_response.additional_properties = d
+        return api_ssh_key_pair_response
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `lightdash_client_python-0.1.2/lightdash_client/models/create_saved_chart_metric_query.py` & `lightdash_client_python-0.611.0/lightdash_client/models/scheduler_image_options.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,37 +2,37 @@
 from typing import Dict
 from typing import List
 from typing import Type
 from typing import TypeVar
 
 import attr
 
-T = TypeVar("T", bound="CreateSavedChartMetricQuery")
+T = TypeVar("T", bound="SchedulerImageOptions")
 
 
 @attr.s(auto_attribs=True)
-class CreateSavedChartMetricQuery:
+class SchedulerImageOptions:
     """ """
 
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({})
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
-        create_saved_chart_metric_query = cls()
+        scheduler_image_options = cls()
 
-        create_saved_chart_metric_query.additional_properties = d
-        return create_saved_chart_metric_query
+        scheduler_image_options.additional_properties = d
+        return scheduler_image_options
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `lightdash_client_python-0.1.2/lightdash_client/models/create_saved_chart_pivot_config.py` & `lightdash_client_python-0.611.0/lightdash_client/models/api_job_scheduled_response_results.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,53 +1,52 @@
 from typing import Any
-from typing import cast
 from typing import Dict
 from typing import List
 from typing import Type
 from typing import TypeVar
 
 import attr
 
-T = TypeVar("T", bound="CreateSavedChartPivotConfig")
+T = TypeVar("T", bound="ApiJobScheduledResponseResults")
 
 
 @attr.s(auto_attribs=True)
-class CreateSavedChartPivotConfig:
+class ApiJobScheduledResponseResults:
     """
     Attributes:
-        columns (List[str]):
+        job_id (str):
     """
 
-    columns: List[str]
+    job_id: str
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
-        columns = self.columns
+        job_id = self.job_id
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update(
             {
-                "columns": columns,
+                "jobId": job_id,
             }
         )
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
-        columns = cast(List[str], d.pop("columns"))
+        job_id = d.pop("jobId")
 
-        create_saved_chart_pivot_config = cls(
-            columns=columns,
+        api_job_scheduled_response_results = cls(
+            job_id=job_id,
         )
 
-        create_saved_chart_pivot_config.additional_properties = d
-        return create_saved_chart_pivot_config
+        api_job_scheduled_response_results.additional_properties = d
+        return api_job_scheduled_response_results
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `lightdash_client_python-0.1.2/lightdash_client/models/create_saved_chart_version_metric_query.py` & `lightdash_client_python-0.611.0/lightdash_client/models/api_validation_dismiss_response.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,37 +2,53 @@
 from typing import Dict
 from typing import List
 from typing import Type
 from typing import TypeVar
 
 import attr
 
-T = TypeVar("T", bound="CreateSavedChartVersionMetricQuery")
+from ..models.api_validation_dismiss_response_status import ApiValidationDismissResponseStatus
+
+T = TypeVar("T", bound="ApiValidationDismissResponse")
 
 
 @attr.s(auto_attribs=True)
-class CreateSavedChartVersionMetricQuery:
-    """ """
+class ApiValidationDismissResponse:
+    """
+    Attributes:
+        status (ApiValidationDismissResponseStatus):
+    """
 
+    status: ApiValidationDismissResponseStatus
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
+        status = self.status.value
+
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
-        field_dict.update({})
+        field_dict.update(
+            {
+                "status": status,
+            }
+        )
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
-        create_saved_chart_version_metric_query = cls()
+        status = ApiValidationDismissResponseStatus(d.pop("status"))
+
+        api_validation_dismiss_response = cls(
+            status=status,
+        )
 
-        create_saved_chart_version_metric_query.additional_properties = d
-        return create_saved_chart_version_metric_query
+        api_validation_dismiss_response.additional_properties = d
+        return api_validation_dismiss_response
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `lightdash_client_python-0.1.2/lightdash_client/models/create_saved_chart_version_pivot_config.py` & `lightdash_client_python-0.611.0/lightdash_client/models/sort_field.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,53 +1,59 @@
 from typing import Any
-from typing import cast
 from typing import Dict
 from typing import List
 from typing import Type
 from typing import TypeVar
 
 import attr
 
-T = TypeVar("T", bound="CreateSavedChartVersionPivotConfig")
+T = TypeVar("T", bound="SortField")
 
 
 @attr.s(auto_attribs=True)
-class CreateSavedChartVersionPivotConfig:
+class SortField:
     """
     Attributes:
-        columns (List[str]):
+        descending (bool):
+        field_id (str):
     """
 
-    columns: List[str]
+    descending: bool
+    field_id: str
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
-        columns = self.columns
+        descending = self.descending
+        field_id = self.field_id
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update(
             {
-                "columns": columns,
+                "descending": descending,
+                "fieldId": field_id,
             }
         )
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
-        columns = cast(List[str], d.pop("columns"))
+        descending = d.pop("descending")
 
-        create_saved_chart_version_pivot_config = cls(
-            columns=columns,
+        field_id = d.pop("fieldId")
+
+        sort_field = cls(
+            descending=descending,
+            field_id=field_id,
         )
 
-        create_saved_chart_version_pivot_config.additional_properties = d
-        return create_saved_chart_version_pivot_config
+        sort_field.additional_properties = d
+        return sort_field
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `lightdash_client_python-0.1.2/lightdash_client/models/create_saved_chart_version_response_200.py` & `lightdash_client_python-0.611.0/lightdash_client/models/api_csv_url_response.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,80 +1,69 @@
 from typing import Any
 from typing import Dict
 from typing import List
 from typing import Type
 from typing import TYPE_CHECKING
 from typing import TypeVar
-from typing import Union
 
 import attr
 
-from ..models.success_status import SuccessStatus
-from ..types import UNSET
-from ..types import Unset
+from ..models.api_csv_url_response_status import ApiCsvUrlResponseStatus
 
 if TYPE_CHECKING:
-    from ..models.saved_chart import SavedChart
+    from ..models.api_csv_url_response_results import ApiCsvUrlResponseResults
 
 
-T = TypeVar("T", bound="CreateSavedChartVersionResponse200")
+T = TypeVar("T", bound="ApiCsvUrlResponse")
 
 
 @attr.s(auto_attribs=True)
-class CreateSavedChartVersionResponse200:
+class ApiCsvUrlResponse:
     """
     Attributes:
-        results (SavedChart):
-        status (Union[Unset, SuccessStatus]):
+        results (ApiCsvUrlResponseResults):
+        status (ApiCsvUrlResponseStatus):
     """
 
-    results: "SavedChart"
-    status: Union[Unset, SuccessStatus] = UNSET
+    results: "ApiCsvUrlResponseResults"
+    status: ApiCsvUrlResponseStatus
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         results = self.results.to_dict()
 
-        status: Union[Unset, str] = UNSET
-        if not isinstance(self.status, Unset):
-            status = self.status.value
+        status = self.status.value
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update(
             {
                 "results": results,
+                "status": status,
             }
         )
-        if status is not UNSET:
-            field_dict["status"] = status
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        from ..models.saved_chart import SavedChart
+        from ..models.api_csv_url_response_results import ApiCsvUrlResponseResults
 
         d = src_dict.copy()
-        results = SavedChart.from_dict(d.pop("results"))
+        results = ApiCsvUrlResponseResults.from_dict(d.pop("results"))
 
-        _status = d.pop("status", UNSET)
-        status: Union[Unset, SuccessStatus]
-        if isinstance(_status, Unset):
-            status = UNSET
-        else:
-            status = SuccessStatus(_status)
+        status = ApiCsvUrlResponseStatus(d.pop("status"))
 
-        create_saved_chart_version_response_200 = cls(
+        api_csv_url_response = cls(
             results=results,
             status=status,
         )
 
-        create_saved_chart_version_response_200.additional_properties = d
-        return create_saved_chart_version_response_200
+        api_csv_url_response.additional_properties = d
+        return api_csv_url_response
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `lightdash_client_python-0.1.2/lightdash_client/models/create_user.py` & `lightdash_client_python-0.611.0/lightdash_client/models/pick_space_name.py`

 * *Files 21% similar despite different names*

```diff
@@ -2,79 +2,52 @@
 from typing import Dict
 from typing import List
 from typing import Type
 from typing import TypeVar
 
 import attr
 
-T = TypeVar("T", bound="CreateUser")
+T = TypeVar("T", bound="PickSpaceName")
 
 
 @attr.s(auto_attribs=True)
-class CreateUser:
-    """
+class PickSpaceName:
+    """From T, pick a set of properties whose keys are in the union K
+
     Attributes:
-        invite_code (str):
-        first_name (str):
-        last_name (str):
-        email (str):
-        password (str):
+        name (str):
     """
 
-    invite_code: str
-    first_name: str
-    last_name: str
-    email: str
-    password: str
+    name: str
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
-        invite_code = self.invite_code
-        first_name = self.first_name
-        last_name = self.last_name
-        email = self.email
-        password = self.password
+        name = self.name
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update(
             {
-                "inviteCode": invite_code,
-                "firstName": first_name,
-                "lastName": last_name,
-                "email": email,
-                "password": password,
+                "name": name,
             }
         )
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
-        invite_code = d.pop("inviteCode")
-
-        first_name = d.pop("firstName")
-
-        last_name = d.pop("lastName")
-
-        email = d.pop("email")
-
-        password = d.pop("password")
+        name = d.pop("name")
 
-        create_user = cls(
-            invite_code=invite_code,
-            first_name=first_name,
-            last_name=last_name,
-            email=email,
-            password=password,
+        pick_space_name = cls(
+            name=name,
         )
 
-        create_user.additional_properties = d
-        return create_user
+        pick_space_name.additional_properties = d
+        return pick_space_name
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `lightdash_client_python-0.1.2/lightdash_client/models/create_user_response_201.py` & `lightdash_client_python-0.611.0/lightdash_client/models/api_group_response.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,80 +1,69 @@
 from typing import Any
 from typing import Dict
 from typing import List
 from typing import Type
 from typing import TYPE_CHECKING
 from typing import TypeVar
-from typing import Union
 
 import attr
 
-from ..models.success_status import SuccessStatus
-from ..types import UNSET
-from ..types import Unset
+from ..models.api_group_response_status import ApiGroupResponseStatus
 
 if TYPE_CHECKING:
-    from ..models.lightdash_user import LightdashUser
+    from ..models.group import Group
 
 
-T = TypeVar("T", bound="CreateUserResponse201")
+T = TypeVar("T", bound="ApiGroupResponse")
 
 
 @attr.s(auto_attribs=True)
-class CreateUserResponse201:
+class ApiGroupResponse:
     """
     Attributes:
-        results (LightdashUser):
-        status (Union[Unset, SuccessStatus]):
+        results (Group):
+        status (ApiGroupResponseStatus):
     """
 
-    results: "LightdashUser"
-    status: Union[Unset, SuccessStatus] = UNSET
+    results: "Group"
+    status: ApiGroupResponseStatus
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         results = self.results.to_dict()
 
-        status: Union[Unset, str] = UNSET
-        if not isinstance(self.status, Unset):
-            status = self.status.value
+        status = self.status.value
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update(
             {
                 "results": results,
+                "status": status,
             }
         )
-        if status is not UNSET:
-            field_dict["status"] = status
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        from ..models.lightdash_user import LightdashUser
+        from ..models.group import Group
 
         d = src_dict.copy()
-        results = LightdashUser.from_dict(d.pop("results"))
+        results = Group.from_dict(d.pop("results"))
 
-        _status = d.pop("status", UNSET)
-        status: Union[Unset, SuccessStatus]
-        if isinstance(_status, Unset):
-            status = UNSET
-        else:
-            status = SuccessStatus(_status)
+        status = ApiGroupResponseStatus(d.pop("status"))
 
-        create_user_response_201 = cls(
+        api_group_response = cls(
             results=results,
             status=status,
         )
 
-        create_user_response_201.additional_properties = d
-        return create_user_response_201
+        api_group_response.additional_properties = d
+        return api_group_response
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `lightdash_client_python-0.1.2/lightdash_client/models/dashboard_list_item.py` & `lightdash_client_python-0.611.0/lightdash_client/models/partial_pick_space_is_private_or_access.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,81 +1,81 @@
-import datetime
 from typing import Any
 from typing import Dict
 from typing import List
 from typing import Type
+from typing import TYPE_CHECKING
 from typing import TypeVar
 from typing import Union
 
 import attr
-from dateutil.parser import isoparse
 
 from ..types import UNSET
 from ..types import Unset
 
-T = TypeVar("T", bound="DashboardListItem")
+if TYPE_CHECKING:
+    from ..models.space_share import SpaceShare
+
+
+T = TypeVar("T", bound="PartialPickSpaceIsPrivateOrAccess")
 
 
 @attr.s(auto_attribs=True)
-class DashboardListItem:
-    """
+class PartialPickSpaceIsPrivateOrAccess:
+    """Make all properties in T optional
+
     Attributes:
-        uuid (str):
-        name (str):
-        updated_at (datetime.datetime):
-        description (Union[Unset, None, str]):
+        is_private (Union[Unset, bool]):
+        access (Union[Unset, List['SpaceShare']]):
     """
 
-    uuid: str
-    name: str
-    updated_at: datetime.datetime
-    description: Union[Unset, None, str] = UNSET
+    is_private: Union[Unset, bool] = UNSET
+    access: Union[Unset, List["SpaceShare"]] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
-        uuid = self.uuid
-        name = self.name
-        updated_at = self.updated_at.isoformat()
+        is_private = self.is_private
+        access: Union[Unset, List[Dict[str, Any]]] = UNSET
+        if not isinstance(self.access, Unset):
+            access = []
+            for access_item_data in self.access:
+                access_item = access_item_data.to_dict()
 
-        description = self.description
+                access.append(access_item)
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
-        field_dict.update(
-            {
-                "uuid": uuid,
-                "name": name,
-                "updatedAt": updated_at,
-            }
-        )
-        if description is not UNSET:
-            field_dict["description"] = description
+        field_dict.update({})
+        if is_private is not UNSET:
+            field_dict["isPrivate"] = is_private
+        if access is not UNSET:
+            field_dict["access"] = access
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        d = src_dict.copy()
-        uuid = d.pop("uuid")
-
-        name = d.pop("name")
+        from ..models.space_share import SpaceShare
 
-        updated_at = isoparse(d.pop("updatedAt"))
-
-        description = d.pop("description", UNSET)
+        d = src_dict.copy()
+        is_private = d.pop("isPrivate", UNSET)
 
-        dashboard_list_item = cls(
-            uuid=uuid,
-            name=name,
-            updated_at=updated_at,
-            description=description,
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
 
-        dashboard_list_item.additional_properties = d
-        return dashboard_list_item
+        partial_pick_space_is_private_or_access.additional_properties = d
+        return partial_pick_space_is_private_or_access
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `lightdash_client_python-0.1.2/lightdash_client/models/error.py` & `lightdash_client_python-0.611.0/lightdash_client/models/pick_group_name.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,69 +1,53 @@
 from typing import Any
 from typing import Dict
 from typing import List
 from typing import Type
-from typing import TYPE_CHECKING
 from typing import TypeVar
 
 import attr
 
-from ..models.error_status import ErrorStatus
-
-if TYPE_CHECKING:
-    from ..models.error_error import ErrorError
-
-
-T = TypeVar("T", bound="Error")
+T = TypeVar("T", bound="PickGroupName")
 
 
 @attr.s(auto_attribs=True)
-class Error:
-    """
+class PickGroupName:
+    """From T, pick a set of properties whose keys are in the union K
+
     Attributes:
-        status (ErrorStatus):
-        error (ErrorError):
+        name (str): A friendly name for the group
     """
 
-    status: ErrorStatus
-    error: "ErrorError"
+    name: str
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
-        status = self.status.value
-
-        error = self.error.to_dict()
+        name = self.name
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update(
             {
-                "status": status,
-                "error": error,
+                "name": name,
             }
         )
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        from ..models.error_error import ErrorError
-
         d = src_dict.copy()
-        status = ErrorStatus(d.pop("status"))
-
-        error = ErrorError.from_dict(d.pop("error"))
+        name = d.pop("name")
 
-        error = cls(
-            status=status,
-            error=error,
+        pick_group_name = cls(
+            name=name,
         )
 
-        error.additional_properties = d
-        return error
+        pick_group_name.additional_properties = d
+        return pick_group_name
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `lightdash_client_python-0.1.2/lightdash_client/models/error_error.py` & `lightdash_client_python-0.611.0/lightdash_client/models/api_error_payload_error.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,92 +1,79 @@
 from typing import Any
 from typing import Dict
 from typing import List
 from typing import Type
-from typing import TYPE_CHECKING
 from typing import TypeVar
 from typing import Union
 
 import attr
 
 from ..types import UNSET
 from ..types import Unset
 
-if TYPE_CHECKING:
-    from ..models.error_error_data import ErrorErrorData
-
-
-T = TypeVar("T", bound="ErrorError")
+T = TypeVar("T", bound="ApiErrorPayloadError")
 
 
 @attr.s(auto_attribs=True)
-class ErrorError:
+class ApiErrorPayloadError:
     """
     Attributes:
-        name (str):
-        status_code (float):
-        message (str):
-        data (Union[Unset, ErrorErrorData]):
+        name (str): Unique name for the type of error
+        status_code (float): HTTP status code
+        data (Union[Unset, Any]): Optional data containing details of the error
+        message (Union[Unset, str]): A friendly message summarising the error
     """
 
     name: str
     status_code: float
-    message: str
-    data: Union[Unset, "ErrorErrorData"] = UNSET
+    data: Union[Unset, Any] = UNSET
+    message: Union[Unset, str] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         name = self.name
         status_code = self.status_code
+        data = self.data
         message = self.message
-        data: Union[Unset, Dict[str, Any]] = UNSET
-        if not isinstance(self.data, Unset):
-            data = self.data.to_dict()
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update(
             {
                 "name": name,
                 "statusCode": status_code,
-                "message": message,
             }
         )
         if data is not UNSET:
             field_dict["data"] = data
+        if message is not UNSET:
+            field_dict["message"] = message
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        from ..models.error_error_data import ErrorErrorData
-
         d = src_dict.copy()
         name = d.pop("name")
 
         status_code = d.pop("statusCode")
 
-        message = d.pop("message")
+        data = d.pop("data", UNSET)
 
-        _data = d.pop("data", UNSET)
-        data: Union[Unset, ErrorErrorData]
-        if isinstance(_data, Unset):
-            data = UNSET
-        else:
-            data = ErrorErrorData.from_dict(_data)
+        message = d.pop("message", UNSET)
 
-        error_error = cls(
+        api_error_payload_error = cls(
             name=name,
             status_code=status_code,
-            message=message,
             data=data,
+            message=message,
         )
 
-        error_error.additional_properties = d
-        return error_error
+        api_error_payload_error.additional_properties = d
+        return api_error_payload_error
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `lightdash_client_python-0.1.2/lightdash_client/models/error_error_data.py` & `lightdash_client_python-0.611.0/lightdash_client/models/pick_space_name_or_is_private.py`

 * *Files 27% similar despite different names*

```diff
@@ -2,37 +2,59 @@
 from typing import Dict
 from typing import List
 from typing import Type
 from typing import TypeVar
 
 import attr
 
-T = TypeVar("T", bound="ErrorErrorData")
+T = TypeVar("T", bound="PickSpaceNameOrIsPrivate")
 
 
 @attr.s(auto_attribs=True)
-class ErrorErrorData:
-    """ """
+class PickSpaceNameOrIsPrivate:
+    """From T, pick a set of properties whose keys are in the union K
 
+    Attributes:
+        name (str):
+        is_private (bool):
+    """
+
+    name: str
+    is_private: bool
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
+        name = self.name
+        is_private = self.is_private
+
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
-        field_dict.update({})
+        field_dict.update(
+            {
+                "name": name,
+                "isPrivate": is_private,
+            }
+        )
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
-        error_error_data = cls()
+        name = d.pop("name")
+
+        is_private = d.pop("isPrivate")
+
+        pick_space_name_or_is_private = cls(
+            name=name,
+            is_private=is_private,
+        )
 
-        error_error_data.additional_properties = d
-        return error_error_data
+        pick_space_name_or_is_private.additional_properties = d
+        return pick_space_name_or_is_private
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `lightdash_client_python-0.1.2/lightdash_client/models/field.py` & `lightdash_client_python-0.611.0/lightdash_client/models/run_query_request_filters.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,101 +6,57 @@
 from typing import Union
 
 import attr
 
 from ..types import UNSET
 from ..types import Unset
 
-T = TypeVar("T", bound="Field")
+T = TypeVar("T", bound="RunQueryRequestFilters")
 
 
 @attr.s(auto_attribs=True)
-class Field:
+class RunQueryRequestFilters:
     """
     Attributes:
-        field_type (str):
-        type (str):
-        name (str):
-        label (str):
-        table (str):
-        table_label (str):
-        sql (str):
-        description (Union[Unset, str]):
+        metrics (Union[Unset, Any]):
+        dimensions (Union[Unset, Any]):
     """
 
-    field_type: str
-    type: str
-    name: str
-    label: str
-    table: str
-    table_label: str
-    sql: str
-    description: Union[Unset, str] = UNSET
+    metrics: Union[Unset, Any] = UNSET
+    dimensions: Union[Unset, Any] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
-        field_type = self.field_type
-        type = self.type
-        name = self.name
-        label = self.label
-        table = self.table
-        table_label = self.table_label
-        sql = self.sql
-        description = self.description
+        metrics = self.metrics
+        dimensions = self.dimensions
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
-        field_dict.update(
-            {
-                "fieldType": field_type,
-                "type": type,
-                "name": name,
-                "label": label,
-                "table": table,
-                "tableLabel": table_label,
-                "sql": sql,
-            }
-        )
-        if description is not UNSET:
-            field_dict["description"] = description
+        field_dict.update({})
+        if metrics is not UNSET:
+            field_dict["metrics"] = metrics
+        if dimensions is not UNSET:
+            field_dict["dimensions"] = dimensions
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
-        field_type = d.pop("fieldType")
-
-        type = d.pop("type")
-
-        name = d.pop("name")
-
-        label = d.pop("label")
-
-        table = d.pop("table")
-
-        table_label = d.pop("tableLabel")
-
-        sql = d.pop("sql")
+        metrics = d.pop("metrics", UNSET)
 
-        description = d.pop("description", UNSET)
+        dimensions = d.pop("dimensions", UNSET)
 
-        field = cls(
-            field_type=field_type,
-            type=type,
-            name=name,
-            label=label,
-            table=table,
-            table_label=table_label,
-            sql=sql,
-            description=description,
+        run_query_request_filters = cls(
+            metrics=metrics,
+            dimensions=dimensions,
         )
 
-        field.additional_properties = d
-        return field
+        run_query_request_filters.additional_properties = d
+        return run_query_request_filters
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `lightdash_client_python-0.1.2/lightdash_client/models/get_available_chart_filters_response_200.py` & `lightdash_client_python-0.611.0/lightdash_client/models/create_space.py`

 * *Files 21% similar despite different names*

```diff
@@ -4,86 +4,87 @@
 from typing import Type
 from typing import TYPE_CHECKING
 from typing import TypeVar
 from typing import Union
 
 import attr
 
-from ..models.success_status import SuccessStatus
 from ..types import UNSET
 from ..types import Unset
 
 if TYPE_CHECKING:
-    from ..models.field import Field
+    from ..models.space_share import SpaceShare
 
 
-T = TypeVar("T", bound="GetAvailableChartFiltersResponse200")
+T = TypeVar("T", bound="CreateSpace")
 
 
 @attr.s(auto_attribs=True)
-class GetAvailableChartFiltersResponse200:
+class CreateSpace:
     """
     Attributes:
-        status (Union[Unset, SuccessStatus]):
-        results (Union[Unset, List['Field']]):
+        name (str):
+        is_private (Union[Unset, bool]):
+        access (Union[Unset, List['SpaceShare']]):
     """
 
-    status: Union[Unset, SuccessStatus] = UNSET
-    results: Union[Unset, List["Field"]] = UNSET
+    name: str
+    is_private: Union[Unset, bool] = UNSET
+    access: Union[Unset, List["SpaceShare"]] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
-        status: Union[Unset, str] = UNSET
-        if not isinstance(self.status, Unset):
-            status = self.status.value
-
-        results: Union[Unset, List[Dict[str, Any]]] = UNSET
-        if not isinstance(self.results, Unset):
-            results = []
-            for componentsschemas_fields_item_data in self.results:
-                componentsschemas_fields_item = componentsschemas_fields_item_data.to_dict()
+        name = self.name
+        is_private = self.is_private
+        access: Union[Unset, List[Dict[str, Any]]] = UNSET
+        if not isinstance(self.access, Unset):
+            access = []
+            for access_item_data in self.access:
+                access_item = access_item_data.to_dict()
 
-                results.append(componentsschemas_fields_item)
+                access.append(access_item)
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
-        field_dict.update({})
-        if status is not UNSET:
-            field_dict["status"] = status
-        if results is not UNSET:
-            field_dict["results"] = results
+        field_dict.update(
+            {
+                "name": name,
+            }
+        )
+        if is_private is not UNSET:
+            field_dict["isPrivate"] = is_private
+        if access is not UNSET:
+            field_dict["access"] = access
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        from ..models.field import Field
+        from ..models.space_share import SpaceShare
 
         d = src_dict.copy()
-        _status = d.pop("status", UNSET)
-        status: Union[Unset, SuccessStatus]
-        if isinstance(_status, Unset):
-            status = UNSET
-        else:
-            status = SuccessStatus(_status)
-
-        results = []
-        _results = d.pop("results", UNSET)
-        for componentsschemas_fields_item_data in _results or []:
-            componentsschemas_fields_item = Field.from_dict(componentsschemas_fields_item_data)
-
-            results.append(componentsschemas_fields_item)
-
-        get_available_chart_filters_response_200 = cls(
-            status=status,
-            results=results,
+        name = d.pop("name")
+
+        is_private = d.pop("isPrivate", UNSET)
+
+        access = []
+        _access = d.pop("access", UNSET)
+        for access_item_data in _access or []:
+            access_item = SpaceShare.from_dict(access_item_data)
+
+            access.append(access_item)
+
+        create_space = cls(
+            name=name,
+            is_private=is_private,
+            access=access,
         )
 
-        get_available_chart_filters_response_200.additional_properties = d
-        return get_available_chart_filters_response_200
+        create_space.additional_properties = d
+        return create_space
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `lightdash_client_python-0.1.2/lightdash_client/models/get_dashboards_response_200.py` & `lightdash_client_python-0.611.0/lightdash_client/models/email_status.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,86 +4,82 @@
 from typing import Type
 from typing import TYPE_CHECKING
 from typing import TypeVar
 from typing import Union
 
 import attr
 
-from ..models.success_status import SuccessStatus
 from ..types import UNSET
 from ..types import Unset
 
 if TYPE_CHECKING:
-    from ..models.dashboard_list_item import DashboardListItem
+    from ..models.email_one_time_password import EmailOneTimePassword
 
 
-T = TypeVar("T", bound="GetDashboardsResponse200")
+T = TypeVar("T", bound="EmailStatus")
 
 
 @attr.s(auto_attribs=True)
-class GetDashboardsResponse200:
+class EmailStatus:
     """
     Attributes:
-        results (List['DashboardListItem']):
-        status (Union[Unset, SuccessStatus]):
+        is_verified (bool):
+        email (str):
+        otp (Union[Unset, EmailOneTimePassword]):
     """
 
-    results: List["DashboardListItem"]
-    status: Union[Unset, SuccessStatus] = UNSET
+    is_verified: bool
+    email: str
+    otp: Union[Unset, "EmailOneTimePassword"] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
-        results = []
-        for results_item_data in self.results:
-            results_item = results_item_data.to_dict()
-
-            results.append(results_item)
-
-        status: Union[Unset, str] = UNSET
-        if not isinstance(self.status, Unset):
-            status = self.status.value
+        is_verified = self.is_verified
+        email = self.email
+        otp: Union[Unset, Dict[str, Any]] = UNSET
+        if not isinstance(self.otp, Unset):
+            otp = self.otp.to_dict()
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update(
             {
-                "results": results,
+                "isVerified": is_verified,
+                "email": email,
             }
         )
-        if status is not UNSET:
-            field_dict["status"] = status
+        if otp is not UNSET:
+            field_dict["otp"] = otp
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        from ..models.dashboard_list_item import DashboardListItem
+        from ..models.email_one_time_password import EmailOneTimePassword
 
         d = src_dict.copy()
-        results = []
-        _results = d.pop("results")
-        for results_item_data in _results:
-            results_item = DashboardListItem.from_dict(results_item_data)
-
-            results.append(results_item)
-
-        _status = d.pop("status", UNSET)
-        status: Union[Unset, SuccessStatus]
-        if isinstance(_status, Unset):
-            status = UNSET
+        is_verified = d.pop("isVerified")
+
+        email = d.pop("email")
+
+        _otp = d.pop("otp", UNSET)
+        otp: Union[Unset, EmailOneTimePassword]
+        if isinstance(_otp, Unset):
+            otp = UNSET
         else:
-            status = SuccessStatus(_status)
+            otp = EmailOneTimePassword.from_dict(_otp)
 
-        get_dashboards_response_200 = cls(
-            results=results,
-            status=status,
+        email_status = cls(
+            is_verified=is_verified,
+            email=email,
+            otp=otp,
         )
 
-        get_dashboards_response_200.additional_properties = d
-        return get_dashboards_response_200
+        email_status.additional_properties = d
+        return email_status
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `lightdash_client_python-0.1.2/lightdash_client/models/get_invite_link_response_200.py` & `lightdash_client_python-0.611.0/lightdash_client/models/delete_scheduler_response_201.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,80 +1,66 @@
 from typing import Any
 from typing import Dict
 from typing import List
 from typing import Type
-from typing import TYPE_CHECKING
 from typing import TypeVar
 from typing import Union
 
 import attr
 
-from ..models.success_status import SuccessStatus
+from ..models.delete_scheduler_response_201_status import DeleteSchedulerResponse201Status
 from ..types import UNSET
 from ..types import Unset
 
-if TYPE_CHECKING:
-    from ..models.invite_link import InviteLink
-
-
-T = TypeVar("T", bound="GetInviteLinkResponse200")
+T = TypeVar("T", bound="DeleteSchedulerResponse201")
 
 
 @attr.s(auto_attribs=True)
-class GetInviteLinkResponse200:
+class DeleteSchedulerResponse201:
     """
     Attributes:
-        results (InviteLink):
-        status (Union[Unset, SuccessStatus]):
+        status (DeleteSchedulerResponse201Status):
+        results (Union[Unset, Any]):
     """
 
-    results: "InviteLink"
-    status: Union[Unset, SuccessStatus] = UNSET
+    status: DeleteSchedulerResponse201Status
+    results: Union[Unset, Any] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
-        results = self.results.to_dict()
+        status = self.status.value
 
-        status: Union[Unset, str] = UNSET
-        if not isinstance(self.status, Unset):
-            status = self.status.value
+        results = self.results
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update(
             {
-                "results": results,
+                "status": status,
             }
         )
-        if status is not UNSET:
-            field_dict["status"] = status
+        if results is not UNSET:
+            field_dict["results"] = results
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        from ..models.invite_link import InviteLink
-
         d = src_dict.copy()
-        results = InviteLink.from_dict(d.pop("results"))
+        status = DeleteSchedulerResponse201Status(d.pop("status"))
 
-        _status = d.pop("status", UNSET)
-        status: Union[Unset, SuccessStatus]
-        if isinstance(_status, Unset):
-            status = UNSET
-        else:
-            status = SuccessStatus(_status)
+        results = d.pop("results", UNSET)
 
-        get_invite_link_response_200 = cls(
-            results=results,
+        delete_scheduler_response_201 = cls(
             status=status,
+            results=results,
         )
 
-        get_invite_link_response_200.additional_properties = d
-        return get_invite_link_response_200
+        delete_scheduler_response_201.additional_properties = d
+        return delete_scheduler_response_201
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `lightdash_client_python-0.1.2/lightdash_client/models/get_job_response_200.py` & `lightdash_client_python-0.611.0/lightdash_client/models/api_success_empty.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,80 +1,66 @@
 from typing import Any
 from typing import Dict
 from typing import List
 from typing import Type
-from typing import TYPE_CHECKING
 from typing import TypeVar
 from typing import Union
 
 import attr
 
-from ..models.success_status import SuccessStatus
+from ..models.api_success_empty_status import ApiSuccessEmptyStatus
 from ..types import UNSET
 from ..types import Unset
 
-if TYPE_CHECKING:
-    from ..models.job import Job
-
-
-T = TypeVar("T", bound="GetJobResponse200")
+T = TypeVar("T", bound="ApiSuccessEmpty")
 
 
 @attr.s(auto_attribs=True)
-class GetJobResponse200:
+class ApiSuccessEmpty:
     """
     Attributes:
-        results (Job):
-        status (Union[Unset, SuccessStatus]):
+        status (ApiSuccessEmptyStatus):
+        results (Union[Unset, Any]):
     """
 
-    results: "Job"
-    status: Union[Unset, SuccessStatus] = UNSET
+    status: ApiSuccessEmptyStatus
+    results: Union[Unset, Any] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
-        results = self.results.to_dict()
+        status = self.status.value
 
-        status: Union[Unset, str] = UNSET
-        if not isinstance(self.status, Unset):
-            status = self.status.value
+        results = self.results
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update(
             {
-                "results": results,
+                "status": status,
             }
         )
-        if status is not UNSET:
-            field_dict["status"] = status
+        if results is not UNSET:
+            field_dict["results"] = results
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        from ..models.job import Job
-
         d = src_dict.copy()
-        results = Job.from_dict(d.pop("results"))
+        status = ApiSuccessEmptyStatus(d.pop("status"))
 
-        _status = d.pop("status", UNSET)
-        status: Union[Unset, SuccessStatus]
-        if isinstance(_status, Unset):
-            status = UNSET
-        else:
-            status = SuccessStatus(_status)
+        results = d.pop("results", UNSET)
 
-        get_job_response_200 = cls(
-            results=results,
+        api_success_empty = cls(
             status=status,
+            results=results,
         )
 
-        get_job_response_200.additional_properties = d
-        return get_job_response_200
+        api_success_empty.additional_properties = d
+        return api_success_empty
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `lightdash_client_python-0.1.2/lightdash_client/models/get_organization_projects_response_200.py` & `lightdash_client_python-0.611.0/lightdash_client/models/api_user_allowed_organizations_response.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,89 +1,78 @@
 from typing import Any
 from typing import Dict
 from typing import List
 from typing import Type
 from typing import TYPE_CHECKING
 from typing import TypeVar
-from typing import Union
 
 import attr
 
-from ..models.success_status import SuccessStatus
-from ..types import UNSET
-from ..types import Unset
+from ..models.api_user_allowed_organizations_response_status import ApiUserAllowedOrganizationsResponseStatus
 
 if TYPE_CHECKING:
-    from ..models.project import Project
+    from ..models.user_allowed_organization import UserAllowedOrganization
 
 
-T = TypeVar("T", bound="GetOrganizationProjectsResponse200")
+T = TypeVar("T", bound="ApiUserAllowedOrganizationsResponse")
 
 
 @attr.s(auto_attribs=True)
-class GetOrganizationProjectsResponse200:
+class ApiUserAllowedOrganizationsResponse:
     """
     Attributes:
-        results (List['Project']):
-        status (Union[Unset, SuccessStatus]):
+        results (List['UserAllowedOrganization']):
+        status (ApiUserAllowedOrganizationsResponseStatus):
     """
 
-    results: List["Project"]
-    status: Union[Unset, SuccessStatus] = UNSET
+    results: List["UserAllowedOrganization"]
+    status: ApiUserAllowedOrganizationsResponseStatus
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         results = []
         for results_item_data in self.results:
             results_item = results_item_data.to_dict()
 
             results.append(results_item)
 
-        status: Union[Unset, str] = UNSET
-        if not isinstance(self.status, Unset):
-            status = self.status.value
+        status = self.status.value
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update(
             {
                 "results": results,
+                "status": status,
             }
         )
-        if status is not UNSET:
-            field_dict["status"] = status
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        from ..models.project import Project
+        from ..models.user_allowed_organization import UserAllowedOrganization
 
         d = src_dict.copy()
         results = []
         _results = d.pop("results")
         for results_item_data in _results:
-            results_item = Project.from_dict(results_item_data)
+            results_item = UserAllowedOrganization.from_dict(results_item_data)
 
             results.append(results_item)
 
-        _status = d.pop("status", UNSET)
-        status: Union[Unset, SuccessStatus]
-        if isinstance(_status, Unset):
-            status = UNSET
-        else:
-            status = SuccessStatus(_status)
+        status = ApiUserAllowedOrganizationsResponseStatus(d.pop("status"))
 
-        get_organization_projects_response_200 = cls(
+        api_user_allowed_organizations_response = cls(
             results=results,
             status=status,
         )
 
-        get_organization_projects_response_200.additional_properties = d
-        return get_organization_projects_response_200
+        api_user_allowed_organizations_response.additional_properties = d
+        return api_user_allowed_organizations_response
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `lightdash_client_python-0.1.2/lightdash_client/models/get_organization_users_response_200.py` & `lightdash_client_python-0.611.0/lightdash_client/models/api_organization.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,89 +1,69 @@
 from typing import Any
 from typing import Dict
 from typing import List
 from typing import Type
 from typing import TYPE_CHECKING
 from typing import TypeVar
-from typing import Union
 
 import attr
 
-from ..models.success_status import SuccessStatus
-from ..types import UNSET
-from ..types import Unset
+from ..models.api_organization_status import ApiOrganizationStatus
 
 if TYPE_CHECKING:
-    from ..models.organization_user import OrganizationUser
+    from ..models.organization import Organization
 
 
-T = TypeVar("T", bound="GetOrganizationUsersResponse200")
+T = TypeVar("T", bound="ApiOrganization")
 
 
 @attr.s(auto_attribs=True)
-class GetOrganizationUsersResponse200:
+class ApiOrganization:
     """
     Attributes:
-        results (List['OrganizationUser']):
-        status (Union[Unset, SuccessStatus]):
+        results (Organization): Details of a user's Organization
+        status (ApiOrganizationStatus):
     """
 
-    results: List["OrganizationUser"]
-    status: Union[Unset, SuccessStatus] = UNSET
+    results: "Organization"
+    status: ApiOrganizationStatus
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
-        results = []
-        for results_item_data in self.results:
-            results_item = results_item_data.to_dict()
-
-            results.append(results_item)
-
-        status: Union[Unset, str] = UNSET
-        if not isinstance(self.status, Unset):
-            status = self.status.value
+        results = self.results.to_dict()
+
+        status = self.status.value
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update(
             {
                 "results": results,
+                "status": status,
             }
         )
-        if status is not UNSET:
-            field_dict["status"] = status
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        from ..models.organization_user import OrganizationUser
+        from ..models.organization import Organization
 
         d = src_dict.copy()
-        results = []
-        _results = d.pop("results")
-        for results_item_data in _results:
-            results_item = OrganizationUser.from_dict(results_item_data)
-
-            results.append(results_item)
-
-        _status = d.pop("status", UNSET)
-        status: Union[Unset, SuccessStatus]
-        if isinstance(_status, Unset):
-            status = UNSET
-        else:
-            status = SuccessStatus(_status)
+        results = Organization.from_dict(d.pop("results"))
+
+        status = ApiOrganizationStatus(d.pop("status"))
 
-        get_organization_users_response_200 = cls(
+        api_organization = cls(
             results=results,
             status=status,
         )
 
-        get_organization_users_response_200.additional_properties = d
-        return get_organization_users_response_200
+        api_organization.additional_properties = d
+        return api_organization
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `lightdash_client_python-0.1.2/lightdash_client/models/get_personal_access_tokens_response_200.py` & `lightdash_client_python-0.611.0/lightdash_client/models/group_member.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,89 +1,74 @@
 from typing import Any
 from typing import Dict
 from typing import List
 from typing import Type
-from typing import TYPE_CHECKING
 from typing import TypeVar
-from typing import Union
 
 import attr
 
-from ..models.success_status import SuccessStatus
-from ..types import UNSET
-from ..types import Unset
-
-if TYPE_CHECKING:
-    from ..models.personal_access_token import PersonalAccessToken
-
-
-T = TypeVar("T", bound="GetPersonalAccessTokensResponse200")
+T = TypeVar("T", bound="GroupMember")
 
 
 @attr.s(auto_attribs=True)
-class GetPersonalAccessTokensResponse200:
-    """
+class GroupMember:
+    """A summary for a Lightdash user within a group
+
     Attributes:
-        results (List['PersonalAccessToken']):
-        status (Union[Unset, SuccessStatus]):
+        last_name (str): The user's last name
+        first_name (str): The user's first name
+        email (str): Primary email address for the user
+        user_uuid (str): Unique id for the user
     """
 
-    results: List["PersonalAccessToken"]
-    status: Union[Unset, SuccessStatus] = UNSET
+    last_name: str
+    first_name: str
+    email: str
+    user_uuid: str
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
-        results = []
-        for results_item_data in self.results:
-            results_item = results_item_data.to_dict()
-
-            results.append(results_item)
-
-        status: Union[Unset, str] = UNSET
-        if not isinstance(self.status, Unset):
-            status = self.status.value
+        last_name = self.last_name
+        first_name = self.first_name
+        email = self.email
+        user_uuid = self.user_uuid
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update(
             {
-                "results": results,
+                "lastName": last_name,
+                "firstName": first_name,
+                "email": email,
+                "userUuid": user_uuid,
             }
         )
-        if status is not UNSET:
-            field_dict["status"] = status
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        from ..models.personal_access_token import PersonalAccessToken
-
         d = src_dict.copy()
-        results = []
-        _results = d.pop("results")
-        for results_item_data in _results:
-            results_item = PersonalAccessToken.from_dict(results_item_data)
-
-            results.append(results_item)
-
-        _status = d.pop("status", UNSET)
-        status: Union[Unset, SuccessStatus]
-        if isinstance(_status, Unset):
-            status = UNSET
-        else:
-            status = SuccessStatus(_status)
-
-        get_personal_access_tokens_response_200 = cls(
-            results=results,
-            status=status,
+        last_name = d.pop("lastName")
+
+        first_name = d.pop("firstName")
+
+        email = d.pop("email")
+
+        user_uuid = d.pop("userUuid")
+
+        group_member = cls(
+            last_name=last_name,
+            first_name=first_name,
+            email=email,
+            user_uuid=user_uuid,
         )
 
-        get_personal_access_tokens_response_200.additional_properties = d
-        return get_personal_access_tokens_response_200
+        group_member.additional_properties = d
+        return group_member
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `lightdash_client_python-0.1.2/lightdash_client/models/get_project_catalog_response_200.py` & `lightdash_client_python-0.611.0/lightdash_client/models/api_job_scheduled_response.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,80 +1,69 @@
 from typing import Any
 from typing import Dict
 from typing import List
 from typing import Type
 from typing import TYPE_CHECKING
 from typing import TypeVar
-from typing import Union
 
 import attr
 
-from ..models.success_status import SuccessStatus
-from ..types import UNSET
-from ..types import Unset
+from ..models.api_job_scheduled_response_status import ApiJobScheduledResponseStatus
 
 if TYPE_CHECKING:
-    from ..models.project_catalog import ProjectCatalog
+    from ..models.api_job_scheduled_response_results import ApiJobScheduledResponseResults
 
 
-T = TypeVar("T", bound="GetProjectCatalogResponse200")
+T = TypeVar("T", bound="ApiJobScheduledResponse")
 
 
 @attr.s(auto_attribs=True)
-class GetProjectCatalogResponse200:
+class ApiJobScheduledResponse:
     """
     Attributes:
-        results (ProjectCatalog):
-        status (Union[Unset, SuccessStatus]):
+        results (ApiJobScheduledResponseResults):
+        status (ApiJobScheduledResponseStatus):
     """
 
-    results: "ProjectCatalog"
-    status: Union[Unset, SuccessStatus] = UNSET
+    results: "ApiJobScheduledResponseResults"
+    status: ApiJobScheduledResponseStatus
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         results = self.results.to_dict()
 
-        status: Union[Unset, str] = UNSET
-        if not isinstance(self.status, Unset):
-            status = self.status.value
+        status = self.status.value
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update(
             {
                 "results": results,
+                "status": status,
             }
         )
-        if status is not UNSET:
-            field_dict["status"] = status
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        from ..models.project_catalog import ProjectCatalog
+        from ..models.api_job_scheduled_response_results import ApiJobScheduledResponseResults
 
         d = src_dict.copy()
-        results = ProjectCatalog.from_dict(d.pop("results"))
+        results = ApiJobScheduledResponseResults.from_dict(d.pop("results"))
 
-        _status = d.pop("status", UNSET)
-        status: Union[Unset, SuccessStatus]
-        if isinstance(_status, Unset):
-            status = UNSET
-        else:
-            status = SuccessStatus(_status)
+        status = ApiJobScheduledResponseStatus(d.pop("status"))
 
-        get_project_catalog_response_200 = cls(
+        api_job_scheduled_response = cls(
             results=results,
             status=status,
         )
 
-        get_project_catalog_response_200.additional_properties = d
-        return get_project_catalog_response_200
+        api_job_scheduled_response.additional_properties = d
+        return api_job_scheduled_response
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `lightdash_client_python-0.1.2/lightdash_client/models/get_project_tables_configuration_response_200.py` & `lightdash_client_python-0.611.0/lightdash_client/models/api_organization_member_profile.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,80 +1,69 @@
 from typing import Any
 from typing import Dict
 from typing import List
 from typing import Type
 from typing import TYPE_CHECKING
 from typing import TypeVar
-from typing import Union
 
 import attr
 
-from ..models.success_status import SuccessStatus
-from ..types import UNSET
-from ..types import Unset
+from ..models.api_organization_member_profile_status import ApiOrganizationMemberProfileStatus
 
 if TYPE_CHECKING:
-    from ..models.project_tables_configuration import ProjectTablesConfiguration
+    from ..models.organization_member_profile import OrganizationMemberProfile
 
 
-T = TypeVar("T", bound="GetProjectTablesConfigurationResponse200")
+T = TypeVar("T", bound="ApiOrganizationMemberProfile")
 
 
 @attr.s(auto_attribs=True)
-class GetProjectTablesConfigurationResponse200:
+class ApiOrganizationMemberProfile:
     """
     Attributes:
-        results (ProjectTablesConfiguration):
-        status (Union[Unset, SuccessStatus]):
+        results (OrganizationMemberProfile): Profile for a user's membership in an organization
+        status (ApiOrganizationMemberProfileStatus):
     """
 
-    results: "ProjectTablesConfiguration"
-    status: Union[Unset, SuccessStatus] = UNSET
+    results: "OrganizationMemberProfile"
+    status: ApiOrganizationMemberProfileStatus
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         results = self.results.to_dict()
 
-        status: Union[Unset, str] = UNSET
-        if not isinstance(self.status, Unset):
-            status = self.status.value
+        status = self.status.value
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update(
             {
                 "results": results,
+                "status": status,
             }
         )
-        if status is not UNSET:
-            field_dict["status"] = status
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        from ..models.project_tables_configuration import ProjectTablesConfiguration
+        from ..models.organization_member_profile import OrganizationMemberProfile
 
         d = src_dict.copy()
-        results = ProjectTablesConfiguration.from_dict(d.pop("results"))
+        results = OrganizationMemberProfile.from_dict(d.pop("results"))
 
-        _status = d.pop("status", UNSET)
-        status: Union[Unset, SuccessStatus]
-        if isinstance(_status, Unset):
-            status = UNSET
-        else:
-            status = SuccessStatus(_status)
+        status = ApiOrganizationMemberProfileStatus(d.pop("status"))
 
-        get_project_tables_configuration_response_200 = cls(
+        api_organization_member_profile = cls(
             results=results,
             status=status,
         )
 
-        get_project_tables_configuration_response_200.additional_properties = d
-        return get_project_tables_configuration_response_200
+        api_organization_member_profile.additional_properties = d
+        return api_organization_member_profile
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `lightdash_client_python-0.1.2/lightdash_client/models/get_saved_chart_response_200.py` & `lightdash_client_python-0.611.0/lightdash_client/models/api_share_response.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,80 +1,71 @@
 from typing import Any
 from typing import Dict
 from typing import List
 from typing import Type
 from typing import TYPE_CHECKING
 from typing import TypeVar
-from typing import Union
 
 import attr
 
-from ..models.success_status import SuccessStatus
-from ..types import UNSET
-from ..types import Unset
+from ..models.api_share_response_status import ApiShareResponseStatus
 
 if TYPE_CHECKING:
-    from ..models.saved_chart import SavedChart
+    from ..models.share_url import ShareUrl
 
 
-T = TypeVar("T", bound="GetSavedChartResponse200")
+T = TypeVar("T", bound="ApiShareResponse")
 
 
 @attr.s(auto_attribs=True)
-class GetSavedChartResponse200:
+class ApiShareResponse:
     """
     Attributes:
-        results (SavedChart):
-        status (Union[Unset, SuccessStatus]):
+        results (ShareUrl): A ShareUrl maps a short shareable id to a full URL
+            in the Lightdash UI. This allows very long URLs
+            to be represented by short ids.
+        status (ApiShareResponseStatus):
     """
 
-    results: "SavedChart"
-    status: Union[Unset, SuccessStatus] = UNSET
+    results: "ShareUrl"
+    status: ApiShareResponseStatus
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         results = self.results.to_dict()
 
-        status: Union[Unset, str] = UNSET
-        if not isinstance(self.status, Unset):
-            status = self.status.value
+        status = self.status.value
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update(
             {
                 "results": results,
+                "status": status,
             }
         )
-        if status is not UNSET:
-            field_dict["status"] = status
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        from ..models.saved_chart import SavedChart
+        from ..models.share_url import ShareUrl
 
         d = src_dict.copy()
-        results = SavedChart.from_dict(d.pop("results"))
+        results = ShareUrl.from_dict(d.pop("results"))
 
-        _status = d.pop("status", UNSET)
-        status: Union[Unset, SuccessStatus]
-        if isinstance(_status, Unset):
-            status = UNSET
-        else:
-            status = SuccessStatus(_status)
+        status = ApiShareResponseStatus(d.pop("status"))
 
-        get_saved_chart_response_200 = cls(
+        api_share_response = cls(
             results=results,
             status=status,
         )
 
-        get_saved_chart_response_200.additional_properties = d
-        return get_saved_chart_response_200
+        api_share_response.additional_properties = d
+        return api_share_response
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `lightdash_client_python-0.1.2/lightdash_client/models/get_user_response_200.py` & `lightdash_client_python-0.611.0/lightdash_client/models/api_group_list_response.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,80 +1,78 @@
 from typing import Any
 from typing import Dict
 from typing import List
 from typing import Type
 from typing import TYPE_CHECKING
 from typing import TypeVar
-from typing import Union
 
 import attr
 
-from ..models.success_status import SuccessStatus
-from ..types import UNSET
-from ..types import Unset
+from ..models.api_group_list_response_status import ApiGroupListResponseStatus
 
 if TYPE_CHECKING:
-    from ..models.lightdash_user import LightdashUser
+    from ..models.group import Group
 
 
-T = TypeVar("T", bound="GetUserResponse200")
+T = TypeVar("T", bound="ApiGroupListResponse")
 
 
 @attr.s(auto_attribs=True)
-class GetUserResponse200:
+class ApiGroupListResponse:
     """
     Attributes:
-        results (LightdashUser):
-        status (Union[Unset, SuccessStatus]):
+        results (List['Group']):
+        status (ApiGroupListResponseStatus):
     """
 
-    results: "LightdashUser"
-    status: Union[Unset, SuccessStatus] = UNSET
+    results: List["Group"]
+    status: ApiGroupListResponseStatus
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
-        results = self.results.to_dict()
+        results = []
+        for results_item_data in self.results:
+            results_item = results_item_data.to_dict()
 
-        status: Union[Unset, str] = UNSET
-        if not isinstance(self.status, Unset):
-            status = self.status.value
+            results.append(results_item)
+
+        status = self.status.value
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update(
             {
                 "results": results,
+                "status": status,
             }
         )
-        if status is not UNSET:
-            field_dict["status"] = status
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        from ..models.lightdash_user import LightdashUser
+        from ..models.group import Group
 
         d = src_dict.copy()
-        results = LightdashUser.from_dict(d.pop("results"))
+        results = []
+        _results = d.pop("results")
+        for results_item_data in _results:
+            results_item = Group.from_dict(results_item_data)
+
+            results.append(results_item)
 
-        _status = d.pop("status", UNSET)
-        status: Union[Unset, SuccessStatus]
-        if isinstance(_status, Unset):
-            status = UNSET
-        else:
-            status = SuccessStatus(_status)
+        status = ApiGroupListResponseStatus(d.pop("status"))
 
-        get_user_response_200 = cls(
+        api_group_list_response = cls(
             results=results,
             status=status,
         )
 
-        get_user_response_200.additional_properties = d
-        return get_user_response_200
+        api_group_list_response.additional_properties = d
+        return api_group_list_response
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `lightdash_client_python-0.1.2/lightdash_client/models/invite_link.py` & `lightdash_client_python-0.611.0/lightdash_client/models/space_share.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,69 +1,76 @@
-import datetime
 from typing import Any
 from typing import Dict
 from typing import List
 from typing import Type
 from typing import TypeVar
 
 import attr
-from dateutil.parser import isoparse
 
-T = TypeVar("T", bound="InviteLink")
+from ..models.project_member_role import ProjectMemberRole
+
+T = TypeVar("T", bound="SpaceShare")
 
 
 @attr.s(auto_attribs=True)
-class InviteLink:
+class SpaceShare:
     """
     Attributes:
-        expires_at (datetime.datetime):
-        invite_code (str):
-        invite_url (str):
+        role (ProjectMemberRole):
+        last_name (str):
+        first_name (str):
+        user_uuid (str):
     """
 
-    expires_at: datetime.datetime
-    invite_code: str
-    invite_url: str
+    role: ProjectMemberRole
+    last_name: str
+    first_name: str
+    user_uuid: str
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
-        expires_at = self.expires_at.isoformat()
+        role = self.role.value
 
-        invite_code = self.invite_code
-        invite_url = self.invite_url
+        last_name = self.last_name
+        first_name = self.first_name
+        user_uuid = self.user_uuid
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update(
             {
-                "expiresAt": expires_at,
-                "inviteCode": invite_code,
-                "inviteUrl": invite_url,
+                "role": role,
+                "lastName": last_name,
+                "firstName": first_name,
+                "userUuid": user_uuid,
             }
         )
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
-        expires_at = isoparse(d.pop("expiresAt"))
+        role = ProjectMemberRole(d.pop("role"))
+
+        last_name = d.pop("lastName")
 
-        invite_code = d.pop("inviteCode")
+        first_name = d.pop("firstName")
 
-        invite_url = d.pop("inviteUrl")
+        user_uuid = d.pop("userUuid")
 
-        invite_link = cls(
-            expires_at=expires_at,
-            invite_code=invite_code,
-            invite_url=invite_url,
+        space_share = cls(
+            role=role,
+            last_name=last_name,
+            first_name=first_name,
+            user_uuid=user_uuid,
         )
 
-        invite_link.additional_properties = d
-        return invite_link
+        space_share.additional_properties = d
+        return space_share
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `lightdash_client_python-0.1.2/lightdash_client/models/job_job_results.py` & `lightdash_client_python-0.611.0/lightdash_client/models/api_job_status_response_results.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,37 +2,51 @@
 from typing import Dict
 from typing import List
 from typing import Type
 from typing import TypeVar
 
 import attr
 
-T = TypeVar("T", bound="JobJobResults")
+T = TypeVar("T", bound="ApiJobStatusResponseResults")
 
 
 @attr.s(auto_attribs=True)
-class JobJobResults:
-    """ """
+class ApiJobStatusResponseResults:
+    """
+    Attributes:
+        status (str):
+    """
 
+    status: str
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
+        status = self.status
+
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
-        field_dict.update({})
+        field_dict.update(
+            {
+                "status": status,
+            }
+        )
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
-        job_job_results = cls()
+        status = d.pop("status")
+
+        api_job_status_response_results = cls(
+            status=status,
+        )
 
-        job_job_results.additional_properties = d
-        return job_job_results
+        api_job_status_response_results.additional_properties = d
+        return api_job_status_response_results
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `lightdash_client_python-0.1.2/lightdash_client/models/lightdash_user_ability_rules_item.py` & `lightdash_client_python-0.611.0/lightdash_client/models/dbt_cloud_metadata_response_metrics.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,38 +1,69 @@
 from typing import Any
 from typing import Dict
 from typing import List
 from typing import Type
+from typing import TYPE_CHECKING
 from typing import TypeVar
 
 import attr
 
-T = TypeVar("T", bound="LightdashUserAbilityRulesItem")
+if TYPE_CHECKING:
+    from ..models.dbt_cloud_metric import DbtCloudMetric
+
+
+T = TypeVar("T", bound="DbtCloudMetadataResponseMetrics")
 
 
 @attr.s(auto_attribs=True)
-class LightdashUserAbilityRulesItem:
-    """ """
+class DbtCloudMetadataResponseMetrics:
+    """Response from dbt cloud metadata api containing a list of metric definitions
+
+    Attributes:
+        metrics (List['DbtCloudMetric']): A list of dbt metric definitions from the dbt cloud metadata api
+    """
 
+    metrics: List["DbtCloudMetric"]
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
+        metrics = []
+        for metrics_item_data in self.metrics:
+            metrics_item = metrics_item_data.to_dict()
+
+            metrics.append(metrics_item)
+
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
-        field_dict.update({})
+        field_dict.update(
+            {
+                "metrics": metrics,
+            }
+        )
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
+        from ..models.dbt_cloud_metric import DbtCloudMetric
+
         d = src_dict.copy()
-        lightdash_user_ability_rules_item = cls()
+        metrics = []
+        _metrics = d.pop("metrics")
+        for metrics_item_data in _metrics:
+            metrics_item = DbtCloudMetric.from_dict(metrics_item_data)
+
+            metrics.append(metrics_item)
+
+        dbt_cloud_metadata_response_metrics = cls(
+            metrics=metrics,
+        )
 
-        lightdash_user_ability_rules_item.additional_properties = d
-        return lightdash_user_ability_rules_item
+        dbt_cloud_metadata_response_metrics.additional_properties = d
+        return dbt_cloud_metadata_response_metrics
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `lightdash_client_python-0.1.2/lightdash_client/models/login.py` & `lightdash_client_python-0.611.0/lightdash_client/models/allowed_email_domains.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,59 +1,79 @@
 from typing import Any
+from typing import cast
 from typing import Dict
 from typing import List
 from typing import Type
 from typing import TypeVar
 
 import attr
 
-T = TypeVar("T", bound="Login")
+from ..models.organization_member_role import OrganizationMemberRole
+
+T = TypeVar("T", bound="AllowedEmailDomains")
 
 
 @attr.s(auto_attribs=True)
-class Login:
+class AllowedEmailDomains:
     """
     Attributes:
-        email (str):
-        password (str):
+        project_uuids (List[str]):
+        role (OrganizationMemberRole):
+        email_domains (List[str]):
+        organization_uuid (str):
     """
 
-    email: str
-    password: str
+    project_uuids: List[str]
+    role: OrganizationMemberRole
+    email_domains: List[str]
+    organization_uuid: str
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
-        email = self.email
-        password = self.password
+        project_uuids = self.project_uuids
+
+        role = self.role.value
+
+        email_domains = self.email_domains
+
+        organization_uuid = self.organization_uuid
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update(
             {
-                "email": email,
-                "password": password,
+                "projectUuids": project_uuids,
+                "role": role,
+                "emailDomains": email_domains,
+                "organizationUuid": organization_uuid,
             }
         )
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
-        email = d.pop("email")
+        project_uuids = cast(List[str], d.pop("projectUuids"))
+
+        role = OrganizationMemberRole(d.pop("role"))
+
+        email_domains = cast(List[str], d.pop("emailDomains"))
 
-        password = d.pop("password")
+        organization_uuid = d.pop("organizationUuid")
 
-        login = cls(
-            email=email,
-            password=password,
+        allowed_email_domains = cls(
+            project_uuids=project_uuids,
+            role=role,
+            email_domains=email_domains,
+            organization_uuid=organization_uuid,
         )
 
-        login.additional_properties = d
-        return login
+        allowed_email_domains.additional_properties = d
+        return allowed_email_domains
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `lightdash_client_python-0.1.2/lightdash_client/models/loom_tile_properties.py` & `lightdash_client_python-0.611.0/lightdash_client/models/filter_group_response_type_0.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,59 +1,61 @@
 from typing import Any
+from typing import cast
 from typing import Dict
 from typing import List
 from typing import Type
 from typing import TypeVar
 
 import attr
 
-T = TypeVar("T", bound="LoomTileProperties")
+T = TypeVar("T", bound="FilterGroupResponseType0")
 
 
 @attr.s(auto_attribs=True)
-class LoomTileProperties:
+class FilterGroupResponseType0:
     """
     Attributes:
-        title (str):
-        url (str):
+        or_ (List[Any]):
+        id (str):
     """
 
-    title: str
-    url: str
+    or_: List[Any]
+    id: str
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
-        title = self.title
-        url = self.url
+        or_ = self.or_
+
+        id = self.id
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update(
             {
-                "title": title,
-                "url": url,
+                "or": or_,
+                "id": id,
             }
         )
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
-        title = d.pop("title")
+        or_ = cast(List[Any], d.pop("or"))
 
-        url = d.pop("url")
+        id = d.pop("id")
 
-        loom_tile_properties = cls(
-            title=title,
-            url=url,
+        filter_group_response_type_0 = cls(
+            or_=or_,
+            id=id,
         )
 
-        loom_tile_properties.additional_properties = d
-        return loom_tile_properties
+        filter_group_response_type_0.additional_properties = d
+        return filter_group_response_type_0
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `lightdash_client_python-0.1.2/lightdash_client/models/markdown_tile_properties.py` & `lightdash_client_python-0.611.0/lightdash_client/models/slack_channel.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,62 +1,59 @@
 from typing import Any
 from typing import Dict
 from typing import List
 from typing import Type
 from typing import TypeVar
-from typing import Union
 
 import attr
 
-from ..types import UNSET
-from ..types import Unset
-
-T = TypeVar("T", bound="MarkdownTileProperties")
+T = TypeVar("T", bound="SlackChannel")
 
 
 @attr.s(auto_attribs=True)
-class MarkdownTileProperties:
+class SlackChannel:
     """
     Attributes:
-        title (Union[Unset, str]):
-        content (Union[Unset, str]):
+        name (str):
+        id (str):
     """
 
-    title: Union[Unset, str] = UNSET
-    content: Union[Unset, str] = UNSET
+    name: str
+    id: str
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
-        title = self.title
-        content = self.content
+        name = self.name
+        id = self.id
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
-        field_dict.update({})
-        if title is not UNSET:
-            field_dict["title"] = title
-        if content is not UNSET:
-            field_dict["content"] = content
+        field_dict.update(
+            {
+                "name": name,
+                "id": id,
+            }
+        )
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
-        title = d.pop("title", UNSET)
+        name = d.pop("name")
 
-        content = d.pop("content", UNSET)
+        id = d.pop("id")
 
-        markdown_tile_properties = cls(
-            title=title,
-            content=content,
+        slack_channel = cls(
+            name=name,
+            id=id,
         )
 
-        markdown_tile_properties.additional_properties = d
-        return markdown_tile_properties
+        slack_channel.additional_properties = d
+        return slack_channel
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `lightdash_client_python-0.1.2/lightdash_client/models/organization_user.py` & `lightdash_client_python-0.611.0/lightdash_client/models/group.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,78 +1,76 @@
+import datetime
 from typing import Any
 from typing import Dict
 from typing import List
 from typing import Type
 from typing import TypeVar
-from typing import Union
 
 import attr
+from dateutil.parser import isoparse
 
-from ..types import UNSET
-from ..types import Unset
-
-T = TypeVar("T", bound="OrganizationUser")
+T = TypeVar("T", bound="Group")
 
 
 @attr.s(auto_attribs=True)
-class OrganizationUser:
+class Group:
     """
     Attributes:
-        user_uuid (str):
-        first_name (str):
-        last_name (str):
-        email (Union[Unset, str]):
+        organization_uuid (str): The UUID of the organization that the group belongs to
+        created_at (datetime.datetime): The time that the group was created
+        name (str): A friendly name for the group
+        uuid (str): The group's UUID
     """
 
-    user_uuid: str
-    first_name: str
-    last_name: str
-    email: Union[Unset, str] = UNSET
+    organization_uuid: str
+    created_at: datetime.datetime
+    name: str
+    uuid: str
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
-        user_uuid = self.user_uuid
-        first_name = self.first_name
-        last_name = self.last_name
-        email = self.email
+        organization_uuid = self.organization_uuid
+        created_at = self.created_at.isoformat()
+
+        name = self.name
+        uuid = self.uuid
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update(
             {
-                "userUuid": user_uuid,
-                "firstName": first_name,
-                "lastName": last_name,
+                "organizationUuid": organization_uuid,
+                "createdAt": created_at,
+                "name": name,
+                "uuid": uuid,
             }
         )
-        if email is not UNSET:
-            field_dict["email"] = email
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
-        user_uuid = d.pop("userUuid")
+        organization_uuid = d.pop("organizationUuid")
 
-        first_name = d.pop("firstName")
+        created_at = isoparse(d.pop("createdAt"))
 
-        last_name = d.pop("lastName")
+        name = d.pop("name")
 
-        email = d.pop("email", UNSET)
+        uuid = d.pop("uuid")
 
-        organization_user = cls(
-            user_uuid=user_uuid,
-            first_name=first_name,
-            last_name=last_name,
-            email=email,
+        group = cls(
+            organization_uuid=organization_uuid,
+            created_at=created_at,
+            name=name,
+            uuid=uuid,
         )
 
-        organization_user.additional_properties = d
-        return organization_user
+        group.additional_properties = d
+        return group
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `lightdash_client_python-0.1.2/lightdash_client/models/patch_saved_chart_response_200.py` & `lightdash_client_python-0.611.0/lightdash_client/models/post_chart_results_json_body.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,77 +4,65 @@
 from typing import Type
 from typing import TYPE_CHECKING
 from typing import TypeVar
 from typing import Union
 
 import attr
 
-from ..models.success_status import SuccessStatus
 from ..types import UNSET
 from ..types import Unset
 
 if TYPE_CHECKING:
-    from ..models.saved_chart import SavedChart
+    from ..models.filters import Filters
 
 
-T = TypeVar("T", bound="PatchSavedChartResponse200")
+T = TypeVar("T", bound="PostChartResultsJsonBody")
 
 
 @attr.s(auto_attribs=True)
-class PatchSavedChartResponse200:
+class PostChartResultsJsonBody:
     """
     Attributes:
-        results (SavedChart):
-        status (Union[Unset, SuccessStatus]):
+        filters (Union[Unset, Filters]):
     """
 
-    results: "SavedChart"
-    status: Union[Unset, SuccessStatus] = UNSET
+    filters: Union[Unset, "Filters"] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
-        results = self.results.to_dict()
-
-        status: Union[Unset, str] = UNSET
-        if not isinstance(self.status, Unset):
-            status = self.status.value
+        filters: Union[Unset, Dict[str, Any]] = UNSET
+        if not isinstance(self.filters, Unset):
+            filters = self.filters.to_dict()
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
-        field_dict.update(
-            {
-                "results": results,
-            }
-        )
-        if status is not UNSET:
-            field_dict["status"] = status
+        field_dict.update({})
+        if filters is not UNSET:
+            field_dict["filters"] = filters
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        from ..models.saved_chart import SavedChart
+        from ..models.filters import Filters
 
         d = src_dict.copy()
-        results = SavedChart.from_dict(d.pop("results"))
-
-        _status = d.pop("status", UNSET)
-        status: Union[Unset, SuccessStatus]
-        if isinstance(_status, Unset):
-            status = UNSET
+        _filters = d.pop("filters", UNSET)
+        filters: Union[Unset, Filters]
+        if isinstance(_filters, Unset):
+            filters = UNSET
         else:
-            status = SuccessStatus(_status)
+            filters = Filters.from_dict(_filters)
 
-        patch_saved_chart_response_200 = cls(
-            results=results,
-            status=status,
+        post_chart_results_json_body = cls(
+            filters=filters,
         )
 
-        patch_saved_chart_response_200.additional_properties = d
-        return patch_saved_chart_response_200
+        post_chart_results_json_body.additional_properties = d
+        return post_chart_results_json_body
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `lightdash_client_python-0.1.2/lightdash_client/models/patch_saved_charts_response_200.py` & `lightdash_client_python-0.611.0/lightdash_client/models/api_scheduled_jobs_response.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,89 +1,78 @@
 from typing import Any
 from typing import Dict
 from typing import List
 from typing import Type
 from typing import TYPE_CHECKING
 from typing import TypeVar
-from typing import Union
 
 import attr
 
-from ..models.success_status import SuccessStatus
-from ..types import UNSET
-from ..types import Unset
+from ..models.api_scheduled_jobs_response_status import ApiScheduledJobsResponseStatus
 
 if TYPE_CHECKING:
-    from ..models.saved_chart import SavedChart
+    from ..models.scheduled_jobs import ScheduledJobs
 
 
-T = TypeVar("T", bound="PatchSavedChartsResponse200")
+T = TypeVar("T", bound="ApiScheduledJobsResponse")
 
 
 @attr.s(auto_attribs=True)
-class PatchSavedChartsResponse200:
+class ApiScheduledJobsResponse:
     """
     Attributes:
-        results (List['SavedChart']):
-        status (Union[Unset, SuccessStatus]):
+        results (List['ScheduledJobs']):
+        status (ApiScheduledJobsResponseStatus):
     """
 
-    results: List["SavedChart"]
-    status: Union[Unset, SuccessStatus] = UNSET
+    results: List["ScheduledJobs"]
+    status: ApiScheduledJobsResponseStatus
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         results = []
         for results_item_data in self.results:
             results_item = results_item_data.to_dict()
 
             results.append(results_item)
 
-        status: Union[Unset, str] = UNSET
-        if not isinstance(self.status, Unset):
-            status = self.status.value
+        status = self.status.value
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update(
             {
                 "results": results,
+                "status": status,
             }
         )
-        if status is not UNSET:
-            field_dict["status"] = status
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        from ..models.saved_chart import SavedChart
+        from ..models.scheduled_jobs import ScheduledJobs
 
         d = src_dict.copy()
         results = []
         _results = d.pop("results")
         for results_item_data in _results:
-            results_item = SavedChart.from_dict(results_item_data)
+            results_item = ScheduledJobs.from_dict(results_item_data)
 
             results.append(results_item)
 
-        _status = d.pop("status", UNSET)
-        status: Union[Unset, SuccessStatus]
-        if isinstance(_status, Unset):
-            status = UNSET
-        else:
-            status = SuccessStatus(_status)
+        status = ApiScheduledJobsResponseStatus(d.pop("status"))
 
-        patch_saved_charts_response_200 = cls(
+        api_scheduled_jobs_response = cls(
             results=results,
             status=status,
         )
 
-        patch_saved_charts_response_200.additional_properties = d
-        return patch_saved_charts_response_200
+        api_scheduled_jobs_response.additional_properties = d
+        return api_scheduled_jobs_response
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `lightdash_client_python-0.1.2/lightdash_client/models/post_saved_chart_response_200.py` & `lightdash_client_python-0.611.0/lightdash_client/models/update_project_member.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,80 +1,54 @@
 from typing import Any
 from typing import Dict
 from typing import List
 from typing import Type
-from typing import TYPE_CHECKING
 from typing import TypeVar
-from typing import Union
 
 import attr
 
-from ..models.success_status import SuccessStatus
-from ..types import UNSET
-from ..types import Unset
+from ..models.project_member_role import ProjectMemberRole
 
-if TYPE_CHECKING:
-    from ..models.saved_chart import SavedChart
-
-
-T = TypeVar("T", bound="PostSavedChartResponse200")
+T = TypeVar("T", bound="UpdateProjectMember")
 
 
 @attr.s(auto_attribs=True)
-class PostSavedChartResponse200:
+class UpdateProjectMember:
     """
     Attributes:
-        results (SavedChart):
-        status (Union[Unset, SuccessStatus]):
+        role (ProjectMemberRole):
     """
 
-    results: "SavedChart"
-    status: Union[Unset, SuccessStatus] = UNSET
+    role: ProjectMemberRole
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
-        results = self.results.to_dict()
-
-        status: Union[Unset, str] = UNSET
-        if not isinstance(self.status, Unset):
-            status = self.status.value
+        role = self.role.value
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update(
             {
-                "results": results,
+                "role": role,
             }
         )
-        if status is not UNSET:
-            field_dict["status"] = status
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        from ..models.saved_chart import SavedChart
-
         d = src_dict.copy()
-        results = SavedChart.from_dict(d.pop("results"))
+        role = ProjectMemberRole(d.pop("role"))
 
-        _status = d.pop("status", UNSET)
-        status: Union[Unset, SuccessStatus]
-        if isinstance(_status, Unset):
-            status = UNSET
-        else:
-            status = SuccessStatus(_status)
-
-        post_saved_chart_response_200 = cls(
-            results=results,
-            status=status,
+        update_project_member = cls(
+            role=role,
         )
 
-        post_saved_chart_response_200.additional_properties = d
-        return post_saved_chart_response_200
+        update_project_member.additional_properties = d
+        return update_project_member
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `lightdash_client_python-0.1.2/lightdash_client/models/project.py` & `lightdash_client_python-0.611.0/lightdash_client/models/validate_project_json_body.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,71 +1,59 @@
 from typing import Any
+from typing import cast
 from typing import Dict
 from typing import List
 from typing import Type
 from typing import TypeVar
 from typing import Union
 
 import attr
 
 from ..types import UNSET
 from ..types import Unset
 
-T = TypeVar("T", bound="Project")
+T = TypeVar("T", bound="ValidateProjectJsonBody")
 
 
 @attr.s(auto_attribs=True)
-class Project:
-    """
-    Attributes:
-        name (str):
-        project_uuid (str):
-        type (Union[Unset, str]):
+class ValidateProjectJsonBody:
+    """the compiled explores to validate against an existing project, this is used in the CLI to validate a project without
+    creating a preview
+
+        Attributes:
+            explores (Union[Unset, List[Any]]):
     """
 
-    name: str
-    project_uuid: str
-    type: Union[Unset, str] = UNSET
+    explores: Union[Unset, List[Any]] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
-        name = self.name
-        project_uuid = self.project_uuid
-        type = self.type
+        explores: Union[Unset, List[Any]] = UNSET
+        if not isinstance(self.explores, Unset):
+            explores = self.explores
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
-        field_dict.update(
-            {
-                "name": name,
-                "projectUuid": project_uuid,
-            }
-        )
-        if type is not UNSET:
-            field_dict["type"] = type
+        field_dict.update({})
+        if explores is not UNSET:
+            field_dict["explores"] = explores
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
-        name = d.pop("name")
-
-        project_uuid = d.pop("projectUuid")
-
-        type = d.pop("type", UNSET)
+        explores = cast(List[Any], d.pop("explores", UNSET))
 
-        project = cls(
-            name=name,
-            project_uuid=project_uuid,
-            type=type,
+        validate_project_json_body = cls(
+            explores=explores,
         )
 
-        project.additional_properties = d
-        return project
+        validate_project_json_body.additional_properties = d
+        return validate_project_json_body
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `lightdash_client_python-0.1.2/lightdash_client/models/project_catalog_database.py` & `lightdash_client_python-0.611.0/lightdash_client/models/api_run_query_response.py`

 * *Files 26% similar despite different names*

```diff
@@ -3,62 +3,76 @@
 from typing import List
 from typing import Type
 from typing import TYPE_CHECKING
 from typing import TypeVar
 
 import attr
 
+from ..models.api_run_query_response_status import ApiRunQueryResponseStatus
+
 if TYPE_CHECKING:
-    from ..models.project_catalog_database_schema import ProjectCatalogDatabaseSchema
+    from ..models.api_run_query_response_results import ApiRunQueryResponseResults
 
 
-T = TypeVar("T", bound="ProjectCatalogDatabase")
+T = TypeVar("T", bound="ApiRunQueryResponse")
 
 
 @attr.s(auto_attribs=True)
-class ProjectCatalogDatabase:
-    """ """
-
-    additional_properties: Dict[str, "ProjectCatalogDatabaseSchema"] = attr.ib(init=False, factory=dict)
+class ApiRunQueryResponse:
+    """
+    Attributes:
+        results (ApiRunQueryResponseResults):
+        status (ApiRunQueryResponseStatus):
+    """
+
+    results: "ApiRunQueryResponseResults"
+    status: ApiRunQueryResponseStatus
+    additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
-        pass
+        results = self.results.to_dict()
 
-        field_dict: Dict[str, Any] = {}
-        for prop_name, prop in self.additional_properties.items():
-            field_dict[prop_name] = prop.to_dict()
+        status = self.status.value
 
-        field_dict.update({})
+        field_dict: Dict[str, Any] = {}
+        field_dict.update(self.additional_properties)
+        field_dict.update(
+            {
+                "results": results,
+                "status": status,
+            }
+        )
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        from ..models.project_catalog_database_schema import ProjectCatalogDatabaseSchema
+        from ..models.api_run_query_response_results import ApiRunQueryResponseResults
 
         d = src_dict.copy()
-        project_catalog_database = cls()
+        results = ApiRunQueryResponseResults.from_dict(d.pop("results"))
 
-        additional_properties = {}
-        for prop_name, prop_dict in d.items():
-            additional_property = ProjectCatalogDatabaseSchema.from_dict(prop_dict)
+        status = ApiRunQueryResponseStatus(d.pop("status"))
 
-            additional_properties[prop_name] = additional_property
+        api_run_query_response = cls(
+            results=results,
+            status=status,
+        )
 
-        project_catalog_database.additional_properties = additional_properties
-        return project_catalog_database
+        api_run_query_response.additional_properties = d
+        return api_run_query_response
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
-    def __getitem__(self, key: str) -> "ProjectCatalogDatabaseSchema":
+    def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
 
-    def __setitem__(self, key: str, value: "ProjectCatalogDatabaseSchema") -> None:
+    def __setitem__(self, key: str, value: Any) -> None:
         self.additional_properties[key] = value
 
     def __delitem__(self, key: str) -> None:
         del self.additional_properties[key]
 
     def __contains__(self, key: str) -> bool:
         return key in self.additional_properties
```

### Comparing `lightdash_client_python-0.1.2/lightdash_client/models/project_catalog_database_schema.py` & `lightdash_client_python-0.611.0/lightdash_client/models/api_job_status_response.py`

 * *Files 23% similar despite different names*

```diff
@@ -3,62 +3,76 @@
 from typing import List
 from typing import Type
 from typing import TYPE_CHECKING
 from typing import TypeVar
 
 import attr
 
+from ..models.api_job_status_response_status import ApiJobStatusResponseStatus
+
 if TYPE_CHECKING:
-    from ..models.project_catalog_database_schema_table import ProjectCatalogDatabaseSchemaTable
+    from ..models.api_job_status_response_results import ApiJobStatusResponseResults
 
 
-T = TypeVar("T", bound="ProjectCatalogDatabaseSchema")
+T = TypeVar("T", bound="ApiJobStatusResponse")
 
 
 @attr.s(auto_attribs=True)
-class ProjectCatalogDatabaseSchema:
-    """ """
-
-    additional_properties: Dict[str, "ProjectCatalogDatabaseSchemaTable"] = attr.ib(init=False, factory=dict)
+class ApiJobStatusResponse:
+    """
+    Attributes:
+        results (ApiJobStatusResponseResults):
+        status (ApiJobStatusResponseStatus):
+    """
+
+    results: "ApiJobStatusResponseResults"
+    status: ApiJobStatusResponseStatus
+    additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
-        pass
+        results = self.results.to_dict()
 
-        field_dict: Dict[str, Any] = {}
-        for prop_name, prop in self.additional_properties.items():
-            field_dict[prop_name] = prop.to_dict()
+        status = self.status.value
 
-        field_dict.update({})
+        field_dict: Dict[str, Any] = {}
+        field_dict.update(self.additional_properties)
+        field_dict.update(
+            {
+                "results": results,
+                "status": status,
+            }
+        )
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        from ..models.project_catalog_database_schema_table import ProjectCatalogDatabaseSchemaTable
+        from ..models.api_job_status_response_results import ApiJobStatusResponseResults
 
         d = src_dict.copy()
-        project_catalog_database_schema = cls()
+        results = ApiJobStatusResponseResults.from_dict(d.pop("results"))
 
-        additional_properties = {}
-        for prop_name, prop_dict in d.items():
-            additional_property = ProjectCatalogDatabaseSchemaTable.from_dict(prop_dict)
+        status = ApiJobStatusResponseStatus(d.pop("status"))
 
-            additional_properties[prop_name] = additional_property
+        api_job_status_response = cls(
+            results=results,
+            status=status,
+        )
 
-        project_catalog_database_schema.additional_properties = additional_properties
-        return project_catalog_database_schema
+        api_job_status_response.additional_properties = d
+        return api_job_status_response
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
-    def __getitem__(self, key: str) -> "ProjectCatalogDatabaseSchemaTable":
+    def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
 
-    def __setitem__(self, key: str, value: "ProjectCatalogDatabaseSchemaTable") -> None:
+    def __setitem__(self, key: str, value: Any) -> None:
         self.additional_properties[key] = value
 
     def __delitem__(self, key: str) -> None:
         del self.additional_properties[key]
 
     def __contains__(self, key: str) -> bool:
         return key in self.additional_properties
```

### Comparing `lightdash_client_python-0.1.2/lightdash_client/models/project_catalog_database_schema_table.py` & `lightdash_client_python-0.611.0/lightdash_client/models/api_run_query_response_results.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,64 +1,68 @@
 from typing import Any
+from typing import cast
 from typing import Dict
 from typing import List
 from typing import Type
+from typing import TYPE_CHECKING
 from typing import TypeVar
-from typing import Union
 
 import attr
 
-from ..types import UNSET
-from ..types import Unset
+if TYPE_CHECKING:
+    from ..models.metric_query_response import MetricQueryResponse
 
-T = TypeVar("T", bound="ProjectCatalogDatabaseSchemaTable")
+
+T = TypeVar("T", bound="ApiRunQueryResponseResults")
 
 
 @attr.s(auto_attribs=True)
-class ProjectCatalogDatabaseSchemaTable:
+class ApiRunQueryResponseResults:
     """
     Attributes:
-        sql_table (str):
-        description (Union[Unset, str]):
+        rows (List[Any]):
+        metric_query (MetricQueryResponse):
     """
 
-    sql_table: str
-    description: Union[Unset, str] = UNSET
+    rows: List[Any]
+    metric_query: "MetricQueryResponse"
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
-        sql_table = self.sql_table
-        description = self.description
+        rows = self.rows
+
+        metric_query = self.metric_query.to_dict()
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update(
             {
-                "sqlTable": sql_table,
+                "rows": rows,
+                "metricQuery": metric_query,
             }
         )
-        if description is not UNSET:
-            field_dict["description"] = description
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
+        from ..models.metric_query_response import MetricQueryResponse
+
         d = src_dict.copy()
-        sql_table = d.pop("sqlTable")
+        rows = cast(List[Any], d.pop("rows"))
 
-        description = d.pop("description", UNSET)
+        metric_query = MetricQueryResponse.from_dict(d.pop("metricQuery"))
 
-        project_catalog_database_schema_table = cls(
-            sql_table=sql_table,
-            description=description,
+        api_run_query_response_results = cls(
+            rows=rows,
+            metric_query=metric_query,
         )
 
-        project_catalog_database_schema_table.additional_properties = d
-        return project_catalog_database_schema_table
+        api_run_query_response_results.additional_properties = d
+        return api_run_query_response_results
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `lightdash_client_python-0.1.2/lightdash_client/models/project_tables_configuration.py` & `lightdash_client_python-0.611.0/lightdash_client/models/email_one_time_password.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,59 +1,61 @@
+import datetime
 from typing import Any
 from typing import Dict
 from typing import List
 from typing import Type
-from typing import TYPE_CHECKING
 from typing import TypeVar
 
 import attr
+from dateutil.parser import isoparse
 
-if TYPE_CHECKING:
-    from ..models.project_tables_configuration_table_selection import ProjectTablesConfigurationTableSelection
-
-
-T = TypeVar("T", bound="ProjectTablesConfiguration")
+T = TypeVar("T", bound="EmailOneTimePassword")
 
 
 @attr.s(auto_attribs=True)
-class ProjectTablesConfiguration:
+class EmailOneTimePassword:
     """
     Attributes:
-        table_selection (ProjectTablesConfigurationTableSelection):
+        number_of_attempts (float): Number of times the passcode has been attempted
+        created_at (datetime.datetime): Time that the passcode was created
     """
 
-    table_selection: "ProjectTablesConfigurationTableSelection"
+    number_of_attempts: float
+    created_at: datetime.datetime
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
-        table_selection = self.table_selection.to_dict()
+        number_of_attempts = self.number_of_attempts
+        created_at = self.created_at.isoformat()
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update(
             {
-                "tableSelection": table_selection,
+                "numberOfAttempts": number_of_attempts,
+                "createdAt": created_at,
             }
         )
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        from ..models.project_tables_configuration_table_selection import ProjectTablesConfigurationTableSelection
-
         d = src_dict.copy()
-        table_selection = ProjectTablesConfigurationTableSelection.from_dict(d.pop("tableSelection"))
+        number_of_attempts = d.pop("numberOfAttempts")
+
+        created_at = isoparse(d.pop("createdAt"))
 
-        project_tables_configuration = cls(
-            table_selection=table_selection,
+        email_one_time_password = cls(
+            number_of_attempts=number_of_attempts,
+            created_at=created_at,
         )
 
-        project_tables_configuration.additional_properties = d
-        return project_tables_configuration
+        email_one_time_password.additional_properties = d
+        return email_one_time_password
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `lightdash_client_python-0.1.2/lightdash_client/models/project_tables_configuration_table_selection.py` & `lightdash_client_python-0.611.0/lightdash_client/models/space_summary.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,67 +1,88 @@
 from typing import Any
 from typing import cast
 from typing import Dict
 from typing import List
-from typing import Optional
 from typing import Type
 from typing import TypeVar
 
 import attr
 
-from ..models.project_tables_configuration_table_selection_type import ProjectTablesConfigurationTableSelectionType
-
-T = TypeVar("T", bound="ProjectTablesConfigurationTableSelection")
+T = TypeVar("T", bound="SpaceSummary")
 
 
 @attr.s(auto_attribs=True)
-class ProjectTablesConfigurationTableSelection:
+class SpaceSummary:
     """
     Attributes:
-        type (ProjectTablesConfigurationTableSelectionType):
-        value (Optional[List[str]]):
+        name (str):
+        organization_uuid (str):
+        uuid (str):
+        project_uuid (str):
+        is_private (bool):
+        access (List[str]):
     """
 
-    type: ProjectTablesConfigurationTableSelectionType
-    value: Optional[List[str]]
+    name: str
+    organization_uuid: str
+    uuid: str
+    project_uuid: str
+    is_private: bool
+    access: List[str]
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
-        type = self.type.value
-
-        if self.value is None:
-            value = None
-        else:
-            value = self.value
+        name = self.name
+        organization_uuid = self.organization_uuid
+        uuid = self.uuid
+        project_uuid = self.project_uuid
+        is_private = self.is_private
+        access = self.access
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update(
             {
-                "type": type,
-                "value": value,
+                "name": name,
+                "organizationUuid": organization_uuid,
+                "uuid": uuid,
+                "projectUuid": project_uuid,
+                "isPrivate": is_private,
+                "access": access,
             }
         )
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
-        type = ProjectTablesConfigurationTableSelectionType(d.pop("type"))
+        name = d.pop("name")
+
+        organization_uuid = d.pop("organizationUuid")
+
+        uuid = d.pop("uuid")
+
+        project_uuid = d.pop("projectUuid")
+
+        is_private = d.pop("isPrivate")
 
-        value = cast(List[str], d.pop("value"))
+        access = cast(List[str], d.pop("access"))
 
-        project_tables_configuration_table_selection = cls(
-            type=type,
-            value=value,
+        space_summary = cls(
+            name=name,
+            organization_uuid=organization_uuid,
+            uuid=uuid,
+            project_uuid=project_uuid,
+            is_private=is_private,
+            access=access,
         )
 
-        project_tables_configuration_table_selection.additional_properties = d
-        return project_tables_configuration_table_selection
+        space_summary.additional_properties = d
+        return space_summary
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `lightdash_client_python-0.1.2/lightdash_client/models/query_result_column_id.py` & `lightdash_client_python-0.611.0/lightdash_client/models/scheduler_csv_options.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,68 +1,82 @@
 from typing import Any
+from typing import cast
 from typing import Dict
 from typing import List
 from typing import Type
-from typing import TYPE_CHECKING
 from typing import TypeVar
 from typing import Union
 
 import attr
 
-from ..types import UNSET
-from ..types import Unset
+from ..models.scheduler_csv_options_limit_type_1 import SchedulerCsvOptionsLimitType1
 
-if TYPE_CHECKING:
-    from ..models.query_result_column_id_value import QueryResultColumnIdValue
-
-
-T = TypeVar("T", bound="QueryResultColumnId")
+T = TypeVar("T", bound="SchedulerCsvOptions")
 
 
 @attr.s(auto_attribs=True)
-class QueryResultColumnId:
+class SchedulerCsvOptions:
     """
     Attributes:
-        value (Union[Unset, QueryResultColumnIdValue]):
+        limit (Union[SchedulerCsvOptionsLimitType1, float]):
+        formatted (bool):
     """
 
-    value: Union[Unset, "QueryResultColumnIdValue"] = UNSET
+    limit: Union[SchedulerCsvOptionsLimitType1, float]
+    formatted: bool
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
-        value: Union[Unset, Dict[str, Any]] = UNSET
-        if not isinstance(self.value, Unset):
-            value = self.value.to_dict()
+        limit: Union[float, str]
+
+        if isinstance(self.limit, SchedulerCsvOptionsLimitType1):
+            limit = self.limit.value
+
+        else:
+            limit = self.limit
+
+        formatted = self.formatted
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
-        field_dict.update({})
-        if value is not UNSET:
-            field_dict["value"] = value
+        field_dict.update(
+            {
+                "limit": limit,
+                "formatted": formatted,
+            }
+        )
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        from ..models.query_result_column_id_value import QueryResultColumnIdValue
-
         d = src_dict.copy()
-        _value = d.pop("value", UNSET)
-        value: Union[Unset, QueryResultColumnIdValue]
-        if isinstance(_value, Unset):
-            value = UNSET
-        else:
-            value = QueryResultColumnIdValue.from_dict(_value)
 
-        query_result_column_id = cls(
-            value=value,
+        def _parse_limit(data: object) -> Union[SchedulerCsvOptionsLimitType1, float]:
+            try:
+                if not isinstance(data, str):
+                    raise TypeError()
+                limit_type_1 = SchedulerCsvOptionsLimitType1(data)
+
+                return limit_type_1
+            except:  # noqa: E722
+                pass
+            return cast(Union[SchedulerCsvOptionsLimitType1, float], data)
+
+        limit = _parse_limit(d.pop("limit"))
+
+        formatted = d.pop("formatted")
+
+        scheduler_csv_options = cls(
+            limit=limit,
+            formatted=formatted,
         )
 
-        query_result_column_id.additional_properties = d
-        return query_result_column_id
+        scheduler_csv_options.additional_properties = d
+        return scheduler_csv_options
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `lightdash_client_python-0.1.2/lightdash_client/models/query_result_column_id_value.py` & `lightdash_client_python-0.611.0/lightdash_client/models/user_allowed_organization.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,62 +1,66 @@
 from typing import Any
 from typing import Dict
 from typing import List
 from typing import Type
 from typing import TypeVar
-from typing import Union
 
 import attr
 
-from ..types import UNSET
-from ..types import Unset
-
-T = TypeVar("T", bound="QueryResultColumnIdValue")
+T = TypeVar("T", bound="UserAllowedOrganization")
 
 
 @attr.s(auto_attribs=True)
-class QueryResultColumnIdValue:
+class UserAllowedOrganization:
     """
     Attributes:
-        raw (Union[Unset, Any]):
-        formatted (Union[Unset, Any]):
+        members_count (float):
+        name (str):
+        organization_uuid (str):
     """
 
-    raw: Union[Unset, Any] = UNSET
-    formatted: Union[Unset, Any] = UNSET
+    members_count: float
+    name: str
+    organization_uuid: str
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
-        raw = self.raw
-        formatted = self.formatted
+        members_count = self.members_count
+        name = self.name
+        organization_uuid = self.organization_uuid
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
-        field_dict.update({})
-        if raw is not UNSET:
-            field_dict["raw"] = raw
-        if formatted is not UNSET:
-            field_dict["formatted"] = formatted
+        field_dict.update(
+            {
+                "membersCount": members_count,
+                "name": name,
+                "organizationUuid": organization_uuid,
+            }
+        )
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
-        raw = d.pop("raw", UNSET)
+        members_count = d.pop("membersCount")
+
+        name = d.pop("name")
 
-        formatted = d.pop("formatted", UNSET)
+        organization_uuid = d.pop("organizationUuid")
 
-        query_result_column_id_value = cls(
-            raw=raw,
-            formatted=formatted,
+        user_allowed_organization = cls(
+            members_count=members_count,
+            name=name,
+            organization_uuid=organization_uuid,
         )
 
-        query_result_column_id_value.additional_properties = d
-        return query_result_column_id_value
+        user_allowed_organization.additional_properties = d
+        return user_allowed_organization
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `lightdash_client_python-0.1.2/lightdash_client/models/run_query_response_200.py` & `lightdash_client_python-0.611.0/lightdash_client/models/partial_omit_organization_organization_uuid_or_needs_project.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,80 +1,66 @@
 from typing import Any
+from typing import cast
 from typing import Dict
 from typing import List
 from typing import Type
-from typing import TYPE_CHECKING
 from typing import TypeVar
 from typing import Union
 
 import attr
 
-from ..models.success_status import SuccessStatus
 from ..types import UNSET
 from ..types import Unset
 
-if TYPE_CHECKING:
-    from ..models.run_query_response_200_results import RunQueryResponse200Results
-
-
-T = TypeVar("T", bound="RunQueryResponse200")
+T = TypeVar("T", bound="PartialOmitOrganizationOrganizationUuidOrNeedsProject")
 
 
 @attr.s(auto_attribs=True)
-class RunQueryResponse200:
-    """
+class PartialOmitOrganizationOrganizationUuidOrNeedsProject:
+    """Make all properties in T optional
+
     Attributes:
-        results (RunQueryResponse200Results):
-        status (Union[Unset, SuccessStatus]):
+        name (Union[Unset, str]): The name of the organization
+        chart_colors (Union[Unset, List[str]]): The default color palette for all projects in the organization
     """
 
-    results: "RunQueryResponse200Results"
-    status: Union[Unset, SuccessStatus] = UNSET
+    name: Union[Unset, str] = UNSET
+    chart_colors: Union[Unset, List[str]] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
-        results = self.results.to_dict()
-
-        status: Union[Unset, str] = UNSET
-        if not isinstance(self.status, Unset):
-            status = self.status.value
+        name = self.name
+        chart_colors: Union[Unset, List[str]] = UNSET
+        if not isinstance(self.chart_colors, Unset):
+            chart_colors = self.chart_colors
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
-        field_dict.update(
-            {
-                "results": results,
-            }
-        )
-        if status is not UNSET:
-            field_dict["status"] = status
+        field_dict.update({})
+        if name is not UNSET:
+            field_dict["name"] = name
+        if chart_colors is not UNSET:
+            field_dict["chartColors"] = chart_colors
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        from ..models.run_query_response_200_results import RunQueryResponse200Results
-
         d = src_dict.copy()
-        results = RunQueryResponse200Results.from_dict(d.pop("results"))
+        name = d.pop("name", UNSET)
+
+        chart_colors = cast(List[str], d.pop("chartColors", UNSET))
 
-        _status = d.pop("status", UNSET)
-        status: Union[Unset, SuccessStatus]
-        if isinstance(_status, Unset):
-            status = UNSET
-        else:
-            status = SuccessStatus(_status)
-
-        run_query_response_200 = cls(
-            results=results,
-            status=status,
+        partial_omit_organization_organization_uuid_or_needs_project = cls(
+            name=name,
+            chart_colors=chart_colors,
         )
 
-        run_query_response_200.additional_properties = d
-        return run_query_response_200
+        partial_omit_organization_organization_uuid_or_needs_project.additional_properties = d
+        return partial_omit_organization_organization_uuid_or_needs_project
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `lightdash_client_python-0.1.2/lightdash_client/models/run_query_response_200_results.py` & `lightdash_client_python-0.611.0/lightdash_client/models/filter_group_response_type_1.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,72 +1,61 @@
 from typing import Any
+from typing import cast
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
-    from ..models.query_result import QueryResult
-
-
-T = TypeVar("T", bound="RunQueryResponse200Results")
+T = TypeVar("T", bound="FilterGroupResponseType1")
 
 
 @attr.s(auto_attribs=True)
-class RunQueryResponse200Results:
+class FilterGroupResponseType1:
     """
     Attributes:
-        rows (Union[Unset, List['QueryResult']]):
+        and_ (List[Any]):
+        id (str):
     """
 
-    rows: Union[Unset, List["QueryResult"]] = UNSET
+    and_: List[Any]
+    id: str
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
-        rows: Union[Unset, List[Dict[str, Any]]] = UNSET
-        if not isinstance(self.rows, Unset):
-            rows = []
-            for rows_item_data in self.rows:
-                rows_item = rows_item_data.to_dict()
+        and_ = self.and_
 
-                rows.append(rows_item)
+        id = self.id
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
-        field_dict.update({})
-        if rows is not UNSET:
-            field_dict["rows"] = rows
+        field_dict.update(
+            {
+                "and": and_,
+                "id": id,
+            }
+        )
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        from ..models.query_result import QueryResult
-
         d = src_dict.copy()
-        rows = []
-        _rows = d.pop("rows", UNSET)
-        for rows_item_data in _rows or []:
-            rows_item = QueryResult.from_dict(rows_item_data)
+        and_ = cast(List[Any], d.pop("and"))
 
-            rows.append(rows_item)
+        id = d.pop("id")
 
-        run_query_response_200_results = cls(
-            rows=rows,
+        filter_group_response_type_1 = cls(
+            and_=and_,
+            id=id,
         )
 
-        run_query_response_200_results.additional_properties = d
-        return run_query_response_200_results
+        filter_group_response_type_1.additional_properties = d
+        return filter_group_response_type_1
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `lightdash_client_python-0.1.2/lightdash_client/models/run_sql_query_response_200.py` & `lightdash_client_python-0.611.0/lightdash_client/models/pick_ssh_key_pair_public_key.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,74 +1,53 @@
 from typing import Any
-from typing import cast
 from typing import Dict
 from typing import List
 from typing import Type
 from typing import TypeVar
-from typing import Union
 
 import attr
 
-from ..models.success_status import SuccessStatus
-from ..types import UNSET
-from ..types import Unset
-
-T = TypeVar("T", bound="RunSqlQueryResponse200")
+T = TypeVar("T", bound="PickSshKeyPairPublicKey")
 
 
 @attr.s(auto_attribs=True)
-class RunSqlQueryResponse200:
-    """
+class PickSshKeyPairPublicKey:
+    """From T, pick a set of properties whose keys are in the union K
+
     Attributes:
-        rows (List[Any]):
-        status (Union[Unset, SuccessStatus]):
+        public_key (str):
     """
 
-    rows: List[Any]
-    status: Union[Unset, SuccessStatus] = UNSET
+    public_key: str
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
-        rows = self.rows
-
-        status: Union[Unset, str] = UNSET
-        if not isinstance(self.status, Unset):
-            status = self.status.value
+        public_key = self.public_key
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update(
             {
-                "rows": rows,
+                "publicKey": public_key,
             }
         )
-        if status is not UNSET:
-            field_dict["status"] = status
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
-        rows = cast(List[Any], d.pop("rows"))
+        public_key = d.pop("publicKey")
 
-        _status = d.pop("status", UNSET)
-        status: Union[Unset, SuccessStatus]
-        if isinstance(_status, Unset):
-            status = UNSET
-        else:
-            status = SuccessStatus(_status)
-
-        run_sql_query_response_200 = cls(
-            rows=rows,
-            status=status,
+        pick_ssh_key_pair_public_key = cls(
+            public_key=public_key,
         )
 
-        run_sql_query_response_200.additional_properties = d
-        return run_sql_query_response_200
+        pick_ssh_key_pair_public_key.additional_properties = d
+        return pick_ssh_key_pair_public_key
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `lightdash_client_python-0.1.2/lightdash_client/models/saved_chart_metric_query.py` & `lightdash_client_python-0.611.0/lightdash_client/models/pick_space_share_user_uuid.py`

 * *Files 19% similar despite different names*

```diff
@@ -2,37 +2,52 @@
 from typing import Dict
 from typing import List
 from typing import Type
 from typing import TypeVar
 
 import attr
 
-T = TypeVar("T", bound="SavedChartMetricQuery")
+T = TypeVar("T", bound="PickSpaceShareUserUuid")
 
 
 @attr.s(auto_attribs=True)
-class SavedChartMetricQuery:
-    """ """
+class PickSpaceShareUserUuid:
+    """From T, pick a set of properties whose keys are in the union K
 
+    Attributes:
+        user_uuid (str):
+    """
+
+    user_uuid: str
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
+        user_uuid = self.user_uuid
+
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
-        field_dict.update({})
+        field_dict.update(
+            {
+                "userUuid": user_uuid,
+            }
+        )
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
-        saved_chart_metric_query = cls()
+        user_uuid = d.pop("userUuid")
+
+        pick_space_share_user_uuid = cls(
+            user_uuid=user_uuid,
+        )
 
-        saved_chart_metric_query.additional_properties = d
-        return saved_chart_metric_query
+        pick_space_share_user_uuid.additional_properties = d
+        return pick_space_share_user_uuid
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `lightdash_client_python-0.1.2/lightdash_client/models/saved_chart_pivot_config.py` & `lightdash_client_python-0.611.0/lightdash_client/models/pick_share_url_path_or_params.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,53 +1,60 @@
 from typing import Any
-from typing import cast
 from typing import Dict
 from typing import List
 from typing import Type
 from typing import TypeVar
 
 import attr
 
-T = TypeVar("T", bound="SavedChartPivotConfig")
+T = TypeVar("T", bound="PickShareUrlPathOrParams")
 
 
 @attr.s(auto_attribs=True)
-class SavedChartPivotConfig:
-    """
+class PickShareUrlPathOrParams:
+    """From T, pick a set of properties whose keys are in the union K
+
     Attributes:
-        columns (List[str]):
+        path (str): The URL path of the full URL
+        params (str):
     """
 
-    columns: List[str]
+    path: str
+    params: str
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
-        columns = self.columns
+        path = self.path
+        params = self.params
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update(
             {
-                "columns": columns,
+                "path": path,
+                "params": params,
             }
         )
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
-        columns = cast(List[str], d.pop("columns"))
+        path = d.pop("path")
+
+        params = d.pop("params")
 
-        saved_chart_pivot_config = cls(
-            columns=columns,
+        pick_share_url_path_or_params = cls(
+            path=path,
+            params=params,
         )
 
-        saved_chart_pivot_config.additional_properties = d
-        return saved_chart_pivot_config
+        pick_share_url_path_or_params.additional_properties = d
+        return pick_share_url_path_or_params
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `lightdash_client_python-0.1.2/lightdash_client/models/step.py` & `lightdash_client_python-0.611.0/lightdash_client/models/validation_response_base.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,135 +1,121 @@
 import datetime
 from typing import Any
 from typing import Dict
 from typing import List
-from typing import Optional
 from typing import Type
-from typing import TYPE_CHECKING
 from typing import TypeVar
 from typing import Union
 
 import attr
 from dateutil.parser import isoparse
 
-from ..models.step_step_status import StepStepStatus
+from ..models.validation_error_type import ValidationErrorType
+from ..models.validation_source_type import ValidationSourceType
 from ..types import UNSET
 from ..types import Unset
 
-if TYPE_CHECKING:
-    from ..models.step_error import StepError
-
-
-T = TypeVar("T", bound="Step")
+T = TypeVar("T", bound="ValidationResponseBase")
 
 
 @attr.s(auto_attribs=True)
-class Step:
+class ValidationResponseBase:
     """
     Attributes:
-        job_uuid (str):
+        project_uuid (str):
+        error_type (ValidationErrorType):
+        error (str):
+        name (str):
         created_at (datetime.datetime):
-        updated_at (datetime.datetime):
-        step_status (StepStepStatus):
-        step_type (str):
-        step_label (str):
-        started_at (Optional[datetime.datetime]):
-        error (Union[Unset, None, StepError]):
+        validation_id (float):
+        source (Union[Unset, ValidationSourceType]):
+        space_uuid (Union[Unset, str]):
     """
 
-    job_uuid: str
+    project_uuid: str
+    error_type: ValidationErrorType
+    error: str
+    name: str
     created_at: datetime.datetime
-    updated_at: datetime.datetime
-    step_status: StepStepStatus
-    step_type: str
-    step_label: str
-    started_at: Optional[datetime.datetime]
-    error: Union[Unset, None, "StepError"] = UNSET
+    validation_id: float
+    source: Union[Unset, ValidationSourceType] = UNSET
+    space_uuid: Union[Unset, str] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
-        job_uuid = self.job_uuid
-        created_at = self.created_at.isoformat()
+        project_uuid = self.project_uuid
+        error_type = self.error_type.value
 
-        updated_at = self.updated_at.isoformat()
-
-        step_status = self.step_status.value
+        error = self.error
+        name = self.name
+        created_at = self.created_at.isoformat()
 
-        step_type = self.step_type
-        step_label = self.step_label
-        started_at = self.started_at.isoformat() if self.started_at else None
+        validation_id = self.validation_id
+        source: Union[Unset, str] = UNSET
+        if not isinstance(self.source, Unset):
+            source = self.source.value
 
-        error: Union[Unset, None, Dict[str, Any]] = UNSET
-        if not isinstance(self.error, Unset):
-            error = self.error.to_dict() if self.error else None
+        space_uuid = self.space_uuid
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update(
             {
-                "jobUuid": job_uuid,
+                "projectUuid": project_uuid,
+                "errorType": error_type,
+                "error": error,
+                "name": name,
                 "createdAt": created_at,
-                "updatedAt": updated_at,
-                "stepStatus": step_status,
-                "stepType": step_type,
-                "stepLabel": step_label,
-                "startedAt": started_at,
+                "validationId": validation_id,
             }
         )
-        if error is not UNSET:
-            field_dict["error"] = error
+        if source is not UNSET:
+            field_dict["source"] = source
+        if space_uuid is not UNSET:
+            field_dict["spaceUuid"] = space_uuid
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        from ..models.step_error import StepError
-
         d = src_dict.copy()
-        job_uuid = d.pop("jobUuid")
+        project_uuid = d.pop("projectUuid")
 
-        created_at = isoparse(d.pop("createdAt"))
+        error_type = ValidationErrorType(d.pop("errorType"))
 
-        updated_at = isoparse(d.pop("updatedAt"))
+        error = d.pop("error")
 
-        step_status = StepStepStatus(d.pop("stepStatus"))
+        name = d.pop("name")
 
-        step_type = d.pop("stepType")
+        created_at = isoparse(d.pop("createdAt"))
 
-        step_label = d.pop("stepLabel")
+        validation_id = d.pop("validationId")
 
-        _started_at = d.pop("startedAt")
-        started_at: Optional[datetime.datetime]
-        if _started_at is None:
-            started_at = None
+        _source = d.pop("source", UNSET)
+        source: Union[Unset, ValidationSourceType]
+        if isinstance(_source, Unset):
+            source = UNSET
         else:
-            started_at = isoparse(_started_at)
+            source = ValidationSourceType(_source)
 
-        _error = d.pop("error", UNSET)
-        error: Union[Unset, None, StepError]
-        if _error is None:
-            error = None
-        elif isinstance(_error, Unset):
-            error = UNSET
-        else:
-            error = StepError.from_dict(_error)
+        space_uuid = d.pop("spaceUuid", UNSET)
 
-        step = cls(
-            job_uuid=job_uuid,
-            created_at=created_at,
-            updated_at=updated_at,
-            step_status=step_status,
-            step_type=step_type,
-            step_label=step_label,
-            started_at=started_at,
+        validation_response_base = cls(
+            project_uuid=project_uuid,
+            error_type=error_type,
             error=error,
+            name=name,
+            created_at=created_at,
+            validation_id=validation_id,
+            source=source,
+            space_uuid=space_uuid,
         )
 
-        step.additional_properties = d
-        return step
+        validation_response_base.additional_properties = d
+        return validation_response_base
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `lightdash_client_python-0.1.2/lightdash_client/models/step_error.py` & `lightdash_client_python-0.611.0/lightdash_client/models/table_calculation.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,57 +6,73 @@
 from typing import Union
 
 import attr
 
 from ..types import UNSET
 from ..types import Unset
 
-T = TypeVar("T", bound="StepError")
+T = TypeVar("T", bound="TableCalculation")
 
 
 @attr.s(auto_attribs=True)
-class StepError:
+class TableCalculation:
     """
     Attributes:
-        name (Union[Unset, str]):
-        message (Union[Unset, str]):
+        sql (str):
+        display_name (str):
+        name (str):
+        index (Union[Unset, float]):
     """
 
-    name: Union[Unset, str] = UNSET
-    message: Union[Unset, str] = UNSET
+    sql: str
+    display_name: str
+    name: str
+    index: Union[Unset, float] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
+        sql = self.sql
+        display_name = self.display_name
         name = self.name
-        message = self.message
+        index = self.index
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
-        field_dict.update({})
-        if name is not UNSET:
-            field_dict["name"] = name
-        if message is not UNSET:
-            field_dict["message"] = message
+        field_dict.update(
+            {
+                "sql": sql,
+                "displayName": display_name,
+                "name": name,
+            }
+        )
+        if index is not UNSET:
+            field_dict["index"] = index
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
-        name = d.pop("name", UNSET)
+        sql = d.pop("sql")
+
+        display_name = d.pop("displayName")
+
+        name = d.pop("name")
 
-        message = d.pop("message", UNSET)
+        index = d.pop("index", UNSET)
 
-        step_error = cls(
+        table_calculation = cls(
+            sql=sql,
+            display_name=display_name,
             name=name,
-            message=message,
+            index=index,
         )
 
-        step_error.additional_properties = d
-        return step_error
+        table_calculation.additional_properties = d
+        return table_calculation
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `lightdash_client_python-0.1.2/lightdash_client/models/success.py` & `lightdash_client_python-0.611.0/lightdash_client/models/organization.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,62 +1,83 @@
 from typing import Any
+from typing import cast
 from typing import Dict
 from typing import List
 from typing import Type
 from typing import TypeVar
 from typing import Union
 
 import attr
 
-from ..models.success_status import SuccessStatus
 from ..types import UNSET
 from ..types import Unset
 
-T = TypeVar("T", bound="Success")
+T = TypeVar("T", bound="Organization")
 
 
 @attr.s(auto_attribs=True)
-class Success:
-    """
+class Organization:
+    """Details of a user's Organization
+
     Attributes:
-        status (Union[Unset, SuccessStatus]):
+        name (str): The name of the organization
+        organization_uuid (str): The unique identifier of the organization
+        needs_project (Union[Unset, bool]): The organization needs a project if it doesn't have at least one project.
+        chart_colors (Union[Unset, List[str]]): The default color palette for all projects in the organization
     """
 
-    status: Union[Unset, SuccessStatus] = UNSET
+    name: str
+    organization_uuid: str
+    needs_project: Union[Unset, bool] = UNSET
+    chart_colors: Union[Unset, List[str]] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
-        status: Union[Unset, str] = UNSET
-        if not isinstance(self.status, Unset):
-            status = self.status.value
+        name = self.name
+        organization_uuid = self.organization_uuid
+        needs_project = self.needs_project
+        chart_colors: Union[Unset, List[str]] = UNSET
+        if not isinstance(self.chart_colors, Unset):
+            chart_colors = self.chart_colors
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
-        field_dict.update({})
-        if status is not UNSET:
-            field_dict["status"] = status
+        field_dict.update(
+            {
+                "name": name,
+                "organizationUuid": organization_uuid,
+            }
+        )
+        if needs_project is not UNSET:
+            field_dict["needsProject"] = needs_project
+        if chart_colors is not UNSET:
+            field_dict["chartColors"] = chart_colors
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
-        _status = d.pop("status", UNSET)
-        status: Union[Unset, SuccessStatus]
-        if isinstance(_status, Unset):
-            status = UNSET
-        else:
-            status = SuccessStatus(_status)
+        name = d.pop("name")
+
+        organization_uuid = d.pop("organizationUuid")
+
+        needs_project = d.pop("needsProject", UNSET)
+
+        chart_colors = cast(List[str], d.pop("chartColors", UNSET))
 
-        success = cls(
-            status=status,
+        organization = cls(
+            name=name,
+            organization_uuid=organization_uuid,
+            needs_project=needs_project,
+            chart_colors=chart_colors,
         )
 
-        success.additional_properties = d
-        return success
+        organization.additional_properties = d
+        return organization
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `lightdash_client_python-0.1.2/lightdash_client/models/update_organization_member_response_200.py` & `lightdash_client_python-0.611.0/lightdash_client/models/pick_validation_response_error_or_created_at_or_validation_id.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,95 +1,70 @@
+import datetime
 from typing import Any
 from typing import Dict
 from typing import List
 from typing import Type
 from typing import TypeVar
-from typing import Union
 
 import attr
+from dateutil.parser import isoparse
 
-from ..models.success_status import SuccessStatus
-from ..types import UNSET
-from ..types import Unset
-
-T = TypeVar("T", bound="UpdateOrganizationMemberResponse200")
+T = TypeVar("T", bound="PickValidationResponseErrorOrCreatedAtOrValidationId")
 
 
 @attr.s(auto_attribs=True)
-class UpdateOrganizationMemberResponse200:
-    """
+class PickValidationResponseErrorOrCreatedAtOrValidationId:
+    """From T, pick a set of properties whose keys are in the union K
+
     Attributes:
-        user_uuid (str):
-        first_name (str):
-        last_name (str):
-        status (Union[Unset, SuccessStatus]):
-        email (Union[Unset, str]):
+        validation_id (float):
+        created_at (datetime.datetime):
+        error (str):
     """
 
-    user_uuid: str
-    first_name: str
-    last_name: str
-    status: Union[Unset, SuccessStatus] = UNSET
-    email: Union[Unset, str] = UNSET
+    validation_id: float
+    created_at: datetime.datetime
+    error: str
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
-        user_uuid = self.user_uuid
-        first_name = self.first_name
-        last_name = self.last_name
-        status: Union[Unset, str] = UNSET
-        if not isinstance(self.status, Unset):
-            status = self.status.value
+        validation_id = self.validation_id
+        created_at = self.created_at.isoformat()
 
-        email = self.email
+        error = self.error
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update(
             {
-                "userUuid": user_uuid,
-                "firstName": first_name,
-                "lastName": last_name,
+                "validationId": validation_id,
+                "createdAt": created_at,
+                "error": error,
             }
         )
-        if status is not UNSET:
-            field_dict["status"] = status
-        if email is not UNSET:
-            field_dict["email"] = email
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
-        user_uuid = d.pop("userUuid")
+        validation_id = d.pop("validationId")
 
-        first_name = d.pop("firstName")
+        created_at = isoparse(d.pop("createdAt"))
 
-        last_name = d.pop("lastName")
+        error = d.pop("error")
 
-        _status = d.pop("status", UNSET)
-        status: Union[Unset, SuccessStatus]
-        if isinstance(_status, Unset):
-            status = UNSET
-        else:
-            status = SuccessStatus(_status)
-
-        email = d.pop("email", UNSET)
-
-        update_organization_member_response_200 = cls(
-            user_uuid=user_uuid,
-            first_name=first_name,
-            last_name=last_name,
-            status=status,
-            email=email,
+        pick_validation_response_error_or_created_at_or_validation_id = cls(
+            validation_id=validation_id,
+            created_at=created_at,
+            error=error,
         )
 
-        update_organization_member_response_200.additional_properties = d
-        return update_organization_member_response_200
+        pick_validation_response_error_or_created_at_or_validation_id.additional_properties = d
+        return pick_validation_response_error_or_created_at_or_validation_id
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `lightdash_client_python-0.1.2/lightdash_client/models/update_project_tables_configuration_response_201.py` & `lightdash_client_python-0.611.0/lightdash_client/models/api_organization_member_profiles.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,80 +1,78 @@
 from typing import Any
 from typing import Dict
 from typing import List
 from typing import Type
 from typing import TYPE_CHECKING
 from typing import TypeVar
-from typing import Union
 
 import attr
 
-from ..models.success_status import SuccessStatus
-from ..types import UNSET
-from ..types import Unset
+from ..models.api_organization_member_profiles_status import ApiOrganizationMemberProfilesStatus
 
 if TYPE_CHECKING:
-    from ..models.project_tables_configuration import ProjectTablesConfiguration
+    from ..models.organization_member_profile import OrganizationMemberProfile
 
 
-T = TypeVar("T", bound="UpdateProjectTablesConfigurationResponse201")
+T = TypeVar("T", bound="ApiOrganizationMemberProfiles")
 
 
 @attr.s(auto_attribs=True)
-class UpdateProjectTablesConfigurationResponse201:
+class ApiOrganizationMemberProfiles:
     """
     Attributes:
-        results (ProjectTablesConfiguration):
-        status (Union[Unset, SuccessStatus]):
+        results (List['OrganizationMemberProfile']):
+        status (ApiOrganizationMemberProfilesStatus):
     """
 
-    results: "ProjectTablesConfiguration"
-    status: Union[Unset, SuccessStatus] = UNSET
+    results: List["OrganizationMemberProfile"]
+    status: ApiOrganizationMemberProfilesStatus
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
-        results = self.results.to_dict()
+        results = []
+        for results_item_data in self.results:
+            results_item = results_item_data.to_dict()
 
-        status: Union[Unset, str] = UNSET
-        if not isinstance(self.status, Unset):
-            status = self.status.value
+            results.append(results_item)
+
+        status = self.status.value
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update(
             {
                 "results": results,
+                "status": status,
             }
         )
-        if status is not UNSET:
-            field_dict["status"] = status
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        from ..models.project_tables_configuration import ProjectTablesConfiguration
+        from ..models.organization_member_profile import OrganizationMemberProfile
 
         d = src_dict.copy()
-        results = ProjectTablesConfiguration.from_dict(d.pop("results"))
+        results = []
+        _results = d.pop("results")
+        for results_item_data in _results:
+            results_item = OrganizationMemberProfile.from_dict(results_item_data)
+
+            results.append(results_item)
 
-        _status = d.pop("status", UNSET)
-        status: Union[Unset, SuccessStatus]
-        if isinstance(_status, Unset):
-            status = UNSET
-        else:
-            status = SuccessStatus(_status)
+        status = ApiOrganizationMemberProfilesStatus(d.pop("status"))
 
-        update_project_tables_configuration_response_201 = cls(
+        api_organization_member_profiles = cls(
             results=results,
             status=status,
         )
 
-        update_project_tables_configuration_response_201.additional_properties = d
-        return update_project_tables_configuration_response_201
+        api_organization_member_profiles.additional_properties = d
+        return api_organization_member_profiles
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `lightdash_client_python-0.1.2/lightdash_client/models/updated_by_user.py` & `lightdash_client_python-0.611.0/lightdash_client/models/project_member_profile.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,65 +2,89 @@
 from typing import Dict
 from typing import List
 from typing import Type
 from typing import TypeVar
 
 import attr
 
-T = TypeVar("T", bound="UpdatedByUser")
+from ..models.project_member_role import ProjectMemberRole
+
+T = TypeVar("T", bound="ProjectMemberProfile")
 
 
 @attr.s(auto_attribs=True)
-class UpdatedByUser:
+class ProjectMemberProfile:
     """
     Attributes:
-        user_uuid (str):
-        first_name (str):
         last_name (str):
+        first_name (str):
+        email (str):
+        role (ProjectMemberRole):
+        project_uuid (str):
+        user_uuid (str):
     """
 
-    user_uuid: str
-    first_name: str
     last_name: str
+    first_name: str
+    email: str
+    role: ProjectMemberRole
+    project_uuid: str
+    user_uuid: str
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
-        user_uuid = self.user_uuid
-        first_name = self.first_name
         last_name = self.last_name
+        first_name = self.first_name
+        email = self.email
+        role = self.role.value
+
+        project_uuid = self.project_uuid
+        user_uuid = self.user_uuid
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update(
             {
-                "userUuid": user_uuid,
-                "firstName": first_name,
                 "lastName": last_name,
+                "firstName": first_name,
+                "email": email,
+                "role": role,
+                "projectUuid": project_uuid,
+                "userUuid": user_uuid,
             }
         )
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
-        user_uuid = d.pop("userUuid")
+        last_name = d.pop("lastName")
 
         first_name = d.pop("firstName")
 
-        last_name = d.pop("lastName")
+        email = d.pop("email")
 
-        updated_by_user = cls(
-            user_uuid=user_uuid,
-            first_name=first_name,
+        role = ProjectMemberRole(d.pop("role"))
+
+        project_uuid = d.pop("projectUuid")
+
+        user_uuid = d.pop("userUuid")
+
+        project_member_profile = cls(
             last_name=last_name,
+            first_name=first_name,
+            email=email,
+            role=role,
+            project_uuid=project_uuid,
+            user_uuid=user_uuid,
         )
 
-        updated_by_user.additional_properties = d
-        return updated_by_user
+        project_member_profile.additional_properties = d
+        return project_member_profile
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `lightdash_client_python-0.1.2/lightdash_client/types.py` & `lightdash_client_python-0.611.0/lightdash_client/types.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.1.2/pyproject.toml` & `lightdash_client_python-0.611.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -38,21 +38,22 @@
 [project.urls]
 Home = "https://github.com/yu-iskw/lightdash-client-python"
 
 [project.optional-dependencies]
 test = [
     "pytest >=6.2.4,<7.0.0",
     "pylint >=2.12.0",
-    "mypy ==0.910",
+    "mypy >=0.910,<1.0",
     "flake8 >=3.8.3,<4.0.0",
-    "black ==21.9b0",
+    "black >=20.0",
     "isort >=5.0.6,<6.0.0",
     "yapf >=0.29.0",
 ]
 dev = [
     "flit ==3.7.1",
     "build ==0.7.0",
     "yapf >=0.29.0",
     "pyyaml >=5.3",
     "pdoc3 >=0.9.2",
     "pre-commit >=2.15.0",
+    "openapi-python-client >=0.14,<1.0",
 ]
```

### Comparing `lightdash_client_python-0.1.2/setup.py` & `lightdash_client_python-0.611.0/setup.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.1.2/tests/__init__.py` & `lightdash_client_python-0.611.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.1.2/tests/test_dummy.py` & `lightdash_client_python-0.611.0/tests/test_dummy.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.1.2/PKG-INFO` & `lightdash_client_python-0.611.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lightdash-client-python
-Version: 0.1.2
+Version: 0.611.0
 Summary: A client library for accessing Lightdash API 
 Author: yu-iskw
 Requires-Python: >=3.8.0,<4
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
@@ -25,19 +25,20 @@
 Requires-Dist: python-dateutil >= 2.8.0, < 3
 Requires-Dist: flit ==3.7.1 ; extra == "dev"
 Requires-Dist: build ==0.7.0 ; extra == "dev"
 Requires-Dist: yapf >=0.29.0 ; extra == "dev"
 Requires-Dist: pyyaml >=5.3 ; extra == "dev"
 Requires-Dist: pdoc3 >=0.9.2 ; extra == "dev"
 Requires-Dist: pre-commit >=2.15.0 ; extra == "dev"
+Requires-Dist: openapi-python-client >=0.14,<1.0 ; extra == "dev"
 Requires-Dist: pytest >=6.2.4,<7.0.0 ; extra == "test"
 Requires-Dist: pylint >=2.12.0 ; extra == "test"
-Requires-Dist: mypy ==0.910 ; extra == "test"
+Requires-Dist: mypy >=0.910,<1.0 ; extra == "test"
 Requires-Dist: flake8 >=3.8.3,<4.0.0 ; extra == "test"
-Requires-Dist: black ==21.9b0 ; extra == "test"
+Requires-Dist: black >=20.0 ; extra == "test"
 Requires-Dist: isort >=5.0.6,<6.0.0 ; extra == "test"
 Requires-Dist: yapf >=0.29.0 ; extra == "test"
 Project-URL: Home, https://github.com/yu-iskw/lightdash-client-python
 Provides-Extra: dev
 Provides-Extra: test
 
 # lightdash-client-python
```

