# Comparing `tmp/pulp_rpm-client-3.9.0.dev1611548779.tar.gz` & `tmp/pulp_rpm-client-3.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pulp_rpm-client-3.9.0.dev1611548779.tar", last modified: Mon Jan 25 04:26:26 2021, max compression
+gzip compressed data, was "dist/pulp_rpm-client-3.9.1.tar", last modified: Thu Mar 11 20:51:37 2021, max compression
```

## Comparing `pulp_rpm-client-3.9.0.dev1611548779.tar` & `pulp_rpm-client-3.9.1.tar`

### file list

```diff
@@ -1,174 +1,174 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-25 04:26:26.000000 pulp_rpm-client-3.9.0.dev1611548779/
--rw-r--r--   0 runner    (1001) docker     (116)      366 2021-01-25 04:26:26.000000 pulp_rpm-client-3.9.0.dev1611548779/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)    14816 2021-01-25 04:26:25.000000 pulp_rpm-client-3.9.0.dev1611548779/README.md
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-25 04:26:26.000000 pulp_rpm-client-3.9.0.dev1611548779/pulp_rpm_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)      366 2021-01-25 04:26:26.000000 pulp_rpm-client-3.9.0.dev1611548779/pulp_rpm_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     8092 2021-01-25 04:26:26.000000 pulp_rpm-client-3.9.0.dev1611548779/pulp_rpm_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2021-01-25 04:26:26.000000 pulp_rpm-client-3.9.0.dev1611548779/pulp_rpm_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)       48 2021-01-25 04:26:26.000000 pulp_rpm-client-3.9.0.dev1611548779/pulp_rpm_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)        9 2021-01-25 04:26:26.000000 pulp_rpm-client-3.9.0.dev1611548779/pulp_rpm_client.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-25 04:26:26.000000 pulp_rpm-client-3.9.0.dev1611548779/pulpcore/
--rw-r--r--   0 runner    (1001) docker     (116)       75 2021-01-25 04:26:25.000000 pulp_rpm-client-3.9.0.dev1611548779/pulpcore/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-25 04:26:26.000000 pulp_rpm-client-3.9.0.dev1611548779/pulpcore/client/
--rw-r--r--   0 runner    (1001) docker     (116)       75 2021-01-25 04:26:25.000000 pulp_rpm-client-3.9.0.dev1611548779/pulpcore/client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-25 04:26:26.000000 pulp_rpm-client-3.9.0.dev1611548779/pulpcore/client/pulp_rpm/
--rw-r--r--   0 runner    (1001) docker     (116)     7920 2021-01-25 04:26:25.000000 pulp_rpm-client-3.9.0.dev1611548779/pulpcore/client/pulp_rpm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-25 04:26:26.000000 pulp_rpm-client-3.9.0.dev1611548779/pulpcore/client/pulp_rpm/api/
--rw-r--r--   0 runner    (1001) docker     (116)     1504 2021-01-25 04:26:25.000000 pulp_rpm-client-3.9.0.dev1611548779/pulpcore/client/pulp_rpm/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    23621 2021-01-25 04:26:25.000000 pulp_rpm-client-3.9.0.dev1611548779/pulpcore/client/pulp_rpm/api/content_advisories_api.py
--rw-r--r--   0 runner    (1001) docker     (116)    14315 2021-01-25 04:26:25.000000 pulp_rpm-client-3.9.0.dev1611548779/pulpcore/client/pulp_rpm/api/content_distribution_trees_api.py
--rw-r--r--   0 runner    (1001) docker     (116)    24428 2021-01-25 04:26:25.000000 pulp_rpm-client-3.9.0.dev1611548779/pulpcore/client/pulp_rpm/api/content_modulemd_defaults_api.py
--rw-r--r--   0 runner    (1001) docker     (116)    26435 2021-01-25 04:26:25.000000 pulp_rpm-client-3.9.0.dev1611548779/pulpcore/client/pulp_rpm/api/content_modulemds_api.py
--rw-r--r--   0 runner    (1001) docker     (116)    14280 2021-01-25 04:26:25.000000 pulp_rpm-client-3.9.0.dev1611548779/pulpcore/client/pulp_rpm/api/content_packagecategories_api.py
--rw-r--r--   0 runner    (1001) docker     (116)    14374 2021-01-25 04:26:25.000000 pulp_rpm-client-3.9.0.dev1611548779/pulpcore/client/pulp_rpm/api/content_packageenvironments_api.py
--rw-r--r--   0 runner    (1001) docker     (116)    14182 2021-01-25 04:26:25.000000 pulp_rpm-client-3.9.0.dev1611548779/pulpcore/client/pulp_rpm/api/content_packagegroups_api.py
--rw-r--r--   0 runner    (1001) docker     (116)    14308 2021-01-25 04:26:25.000000 pulp_rpm-client-3.9.0.dev1611548779/pulpcore/client/pulp_rpm/api/content_packagelangpacks_api.py
--rw-r--r--   0 runner    (1001) docker     (116)    27731 2021-01-25 04:26:25.000000 pulp_rpm-client-3.9.0.dev1611548779/pulpcore/client/pulp_rpm/api/content_packages_api.py
--rw-r--r--   0 runner    (1001) docker     (116)    14332 2021-01-25 04:26:25.000000 pulp_rpm-client-3.9.0.dev1611548779/pulpcore/client/pulp_rpm/api/content_repo_metadata_files_api.py
--rw-r--r--   0 runner    (1001) docker     (116)    39535 2021-01-25 04:26:25.000000 pulp_rpm-client-3.9.0.dev1611548779/pulpcore/client/pulp_rpm/api/distributions_rpm_api.py
--rw-r--r--   0 runner    (1001) docker     (116)    25967 2021-01-25 04:26:25.000000 pulp_rpm-client-3.9.0.dev1611548779/pulpcore/client/pulp_rpm/api/publications_rpm_api.py
--rw-r--r--   0 runner    (1001) docker     (116)    39719 2021-01-25 04:26:25.000000 pulp_rpm-client-3.9.0.dev1611548779/pulpcore/client/pulp_rpm/api/remotes_rpm_api.py
--rw-r--r--   0 runner    (1001) docker     (116)    50653 2021-01-25 04:26:25.000000 pulp_rpm-client-3.9.0.dev1611548779/pulpcore/client/pulp_rpm/api/repositories_rpm_api.py
--rw-r--r--   0 runner    (1001) docker     (116)    30602 2021-01-25 04:26:25.000000 pulp_rpm-client-3.9.0.dev1611548779/pulpcore/client/pulp_rpm/api/repositories_rpm_versions_api.py
--rw-r--r--   0 runner    (1001) docker     (116)     6171 2021-01-25 04:26:25.000000 pulp_rpm-client-3.9.0.dev1611548779/pulpcore/client/pulp_rpm/api/rpm_copy_api.py
--rw-r--r--   0 runner    (1001) docker     (116)    26289 2021-01-25 04:26:25.000000 pulp_rpm-client-3.9.0.dev1611548779/pulpcore/client/pulp_rpm/api_client.py
--rw-r--r--   0 runner    (1001) docker     (116)    13967 2021-01-25 04:26:25.000000 pulp_rpm-client-3.9.0.dev1611548779/pulpcore/client/pulp_rpm/configuration.py
--rw-r--r--   0 runner    (1001) docker     (116)     3769 2021-01-25 04:26:25.000000 pulp_rpm-client-3.9.0.dev1611548779/pulpcore/client/pulp_rpm/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-25 04:26:26.000000 pulp_rpm-client-3.9.0.dev1611548779/pulpcore/client/pulp_rpm/models/
--rw-r--r--   0 runner    (1001) docker     (116)     5982 2021-01-25 04:26:25.000000 pulp_rpm-client-3.9.0.dev1611548779/pulpcore/client/pulp_rpm/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     6899 2021-01-25 04:26:24.000000 pulp_rpm-client-3.9.0.dev1611548779/pulpcore/client/pulp_rpm/models/addon_response.py
--rw-r--r--   0 runner    (1001) docker     (116)    10073 2021-01-25 04:26:24.000000 pulp_rpm-client-3.9.0.dev1611548779/pulpcore/client/pulp_rpm/models/artifact_response.py
--rw-r--r--   0 runner    (1001) docker     (116)     3572 2021-01-25 04:26:24.000000 pulp_rpm-client-3.9.0.dev1611548779/pulpcore/client/pulp_rpm/models/async_operation_response.py
--rw-r--r--   0 runner    (1001) docker     (116)     4423 2021-01-25 04:26:24.000000 pulp_rpm-client-3.9.0.dev1611548779/pulpcore/client/pulp_rpm/models/checksum_response.py
--rw-r--r--   0 runner    (1001) docker     (116)     5072 2021-01-25 04:26:24.000000 pulp_rpm-client-3.9.0.dev1611548779/pulpcore/client/pulp_rpm/models/content_summary.py
--rw-r--r--   0 runner    (1001) docker     (116)     5200 2021-01-25 04:26:24.000000 pulp_rpm-client-3.9.0.dev1611548779/pulpcore/client/pulp_rpm/models/content_summary_response.py
--rw-r--r--   0 runner    (1001) docker     (116)     4561 2021-01-25 04:26:24.000000 pulp_rpm-client-3.9.0.dev1611548779/pulpcore/client/pulp_rpm/models/copy.py
--rw-r--r--   0 runner    (1001) docker     (116)     5870 2021-01-25 04:26:24.000000 pulp_rpm-client-3.9.0.dev1611548779/pulpcore/client/pulp_rpm/models/image_response.py
--rw-r--r--   0 runner    (1001) docker     (116)     2999 2021-01-25 04:26:24.000000 pulp_rpm-client-3.9.0.dev1611548779/pulpcore/client/pulp_rpm/models/metadata_checksum_type_enum.py
--rw-r--r--   0 runner    (1001) docker     (116)     2995 2021-01-25 04:26:24.000000 pulp_rpm-client-3.9.0.dev1611548779/pulpcore/client/pulp_rpm/models/package_checksum_type_enum.py
--rw-r--r--   0 runner    (1001) docker     (116)     5675 2021-01-25 04:26:24.000000 pulp_rpm-client-3.9.0.dev1611548779/pulpcore/client/pulp_rpm/models/paginated_repository_version_response_list.py
--rw-r--r--   0 runner    (1001) docker     (116)     5721 2021-01-25 04:26:24.000000 pulp_rpm-client-3.9.0.dev1611548779/pulpcore/client/pulp_rpm/models/paginatedrpm_distribution_tree_response_list.py
--rw-r--r--   0 runner    (1001) docker     (116)     5721 2021-01-25 04:26:24.000000 pulp_rpm-client-3.9.0.dev1611548779/pulpcore/client/pulp_rpm/models/paginatedrpm_modulemd_defaults_response_list.py
--rw-r--r--   0 runner    (1001) docker     (116)     5537 2021-01-25 04:26:24.000000 pulp_rpm-client-3.9.0.dev1611548779/pulpcore/client/pulp_rpm/models/paginatedrpm_modulemd_response_list.py
--rw-r--r--   0 runner    (1001) docker     (116)     5698 2021-01-25 04:26:24.000000 pulp_rpm-client-3.9.0.dev1611548779/pulpcore/client/pulp_rpm/models/paginatedrpm_package_category_response_list.py
--rw-r--r--   0 runner    (1001) docker     (116)     5767 2021-01-25 04:26:24.000000 pulp_rpm-client-3.9.0.dev1611548779/pulpcore/client/pulp_rpm/models/paginatedrpm_package_environment_response_list.py
--rw-r--r--   0 runner    (1001) docker     (116)     5629 2021-01-25 04:26:24.000000 pulp_rpm-client-3.9.0.dev1611548779/pulpcore/client/pulp_rpm/models/paginatedrpm_package_group_response_list.py
--rw-r--r--   0 runner    (1001) docker     (116)     5721 2021-01-25 04:26:24.000000 pulp_rpm-client-3.9.0.dev1611548779/pulpcore/client/pulp_rpm/models/paginatedrpm_package_langpacks_response_list.py
--rw-r--r--   0 runner    (1001) docker     (116)     5514 2021-01-25 04:26:24.000000 pulp_rpm-client-3.9.0.dev1611548779/pulpcore/client/pulp_rpm/models/paginatedrpm_package_response_list.py
--rw-r--r--   0 runner    (1001) docker     (116)     5721 2021-01-25 04:26:24.000000 pulp_rpm-client-3.9.0.dev1611548779/pulpcore/client/pulp_rpm/models/paginatedrpm_repo_metadata_file_response_list.py
--rw-r--r--   0 runner    (1001) docker     (116)     5698 2021-01-25 04:26:24.000000 pulp_rpm-client-3.9.0.dev1611548779/pulpcore/client/pulp_rpm/models/paginatedrpm_rpm_distribution_response_list.py
--rw-r--r--   0 runner    (1001) docker     (116)     5675 2021-01-25 04:26:24.000000 pulp_rpm-client-3.9.0.dev1611548779/pulpcore/client/pulp_rpm/models/paginatedrpm_rpm_publication_response_list.py
--rw-r--r--   0 runner    (1001) docker     (116)     5560 2021-01-25 04:26:24.000000 pulp_rpm-client-3.9.0.dev1611548779/pulpcore/client/pulp_rpm/models/paginatedrpm_rpm_remote_response_list.py
--rw-r--r--   0 runner    (1001) docker     (116)     5652 2021-01-25 04:26:24.000000 pulp_rpm-client-3.9.0.dev1611548779/pulpcore/client/pulp_rpm/models/paginatedrpm_rpm_repository_response_list.py
--rw-r--r--   0 runner    (1001) docker     (116)     5629 2021-01-25 04:26:24.000000 pulp_rpm-client-3.9.0.dev1611548779/pulpcore/client/pulp_rpm/models/paginatedrpm_update_record_response_list.py
--rw-r--r--   0 runner    (1001) docker     (116)     6281 2021-01-25 04:26:24.000000 pulp_rpm-client-3.9.0.dev1611548779/pulpcore/client/pulp_rpm/models/patchedrpm_rpm_distribution.py
--rw-r--r--   0 runner    (1001) docker     (116)    18420 2021-01-25 04:26:24.000000 pulp_rpm-client-3.9.0.dev1611548779/pulpcore/client/pulp_rpm/models/patchedrpm_rpm_remote.py
--rw-r--r--   0 runner    (1001) docker     (116)     7723 2021-01-25 04:26:24.000000 pulp_rpm-client-3.9.0.dev1611548779/pulpcore/client/pulp_rpm/models/patchedrpm_rpm_repository.py
--rw-r--r--   0 runner    (1001) docker     (116)     2859 2021-01-25 04:26:24.000000 pulp_rpm-client-3.9.0.dev1611548779/pulpcore/client/pulp_rpm/models/policy_enum.py
--rw-r--r--   0 runner    (1001) docker     (116)     6396 2021-01-25 04:26:24.000000 pulp_rpm-client-3.9.0.dev1611548779/pulpcore/client/pulp_rpm/models/repository_add_remove_content.py
--rw-r--r--   0 runner    (1001) docker     (116)     3698 2021-01-25 04:26:24.000000 pulp_rpm-client-3.9.0.dev1611548779/pulpcore/client/pulp_rpm/models/repository_version.py
--rw-r--r--   0 runner    (1001) docker     (116)     7166 2021-01-25 04:26:24.000000 pulp_rpm-client-3.9.0.dev1611548779/pulpcore/client/pulp_rpm/models/repository_version_response.py
--rw-r--r--   0 runner    (1001) docker     (116)    20723 2021-01-25 04:26:24.000000 pulp_rpm-client-3.9.0.dev1611548779/pulpcore/client/pulp_rpm/models/rpm_distribution_tree_response.py
--rw-r--r--   0 runner    (1001) docker     (116)    12702 2021-01-25 04:26:24.000000 pulp_rpm-client-3.9.0.dev1611548779/pulpcore/client/pulp_rpm/models/rpm_modulemd.py
--rw-r--r--   0 runner    (1001) docker     (116)     9115 2021-01-25 04:26:24.000000 pulp_rpm-client-3.9.0.dev1611548779/pulpcore/client/pulp_rpm/models/rpm_modulemd_defaults.py
--rw-r--r--   0 runner    (1001) docker     (116)    12703 2021-01-25 04:26:24.000000 pulp_rpm-client-3.9.0.dev1611548779/pulpcore/client/pulp_rpm/models/rpm_modulemd_defaults_response.py
--rw-r--r--   0 runner    (1001) docker     (116)    16290 2021-01-25 04:26:24.000000 pulp_rpm-client-3.9.0.dev1611548779/pulpcore/client/pulp_rpm/models/rpm_modulemd_response.py
--rw-r--r--   0 runner    (1001) docker     (116)     6191 2021-01-25 04:26:24.000000 pulp_rpm-client-3.9.0.dev1611548779/pulpcore/client/pulp_rpm/models/rpm_package.py
--rw-r--r--   0 runner    (1001) docker     (116)    11350 2021-01-25 04:26:24.000000 pulp_rpm-client-3.9.0.dev1611548779/pulpcore/client/pulp_rpm/models/rpm_package_category_response.py
--rw-r--r--   0 runner    (1001) docker     (116)    12355 2021-01-25 04:26:24.000000 pulp_rpm-client-3.9.0.dev1611548779/pulpcore/client/pulp_rpm/models/rpm_package_environment_response.py
--rw-r--r--   0 runner    (1001) docker     (116)    13787 2021-01-25 04:26:24.000000 pulp_rpm-client-3.9.0.dev1611548779/pulpcore/client/pulp_rpm/models/rpm_package_group_response.py
--rw-r--r--   0 runner    (1001) docker     (116)     5846 2021-01-25 04:26:24.000000 pulp_rpm-client-3.9.0.dev1611548779/pulpcore/client/pulp_rpm/models/rpm_package_langpacks_response.py
--rw-r--r--   0 runner    (1001) docker     (116)    40009 2021-01-25 04:26:24.000000 pulp_rpm-client-3.9.0.dev1611548779/pulpcore/client/pulp_rpm/models/rpm_package_response.py
--rw-r--r--   0 runner    (1001) docker     (116)    13956 2021-01-25 04:26:24.000000 pulp_rpm-client-3.9.0.dev1611548779/pulpcore/client/pulp_rpm/models/rpm_repo_metadata_file_response.py
--rw-r--r--   0 runner    (1001) docker     (116)     6693 2021-01-25 04:26:24.000000 pulp_rpm-client-3.9.0.dev1611548779/pulpcore/client/pulp_rpm/models/rpm_repository_sync_url.py
--rw-r--r--   0 runner    (1001) docker     (116)     6454 2021-01-25 04:26:24.000000 pulp_rpm-client-3.9.0.dev1611548779/pulpcore/client/pulp_rpm/models/rpm_rpm_distribution.py
--rw-r--r--   0 runner    (1001) docker     (116)     9144 2021-01-25 04:26:24.000000 pulp_rpm-client-3.9.0.dev1611548779/pulpcore/client/pulp_rpm/models/rpm_rpm_distribution_response.py
--rw-r--r--   0 runner    (1001) docker     (116)    10605 2021-01-25 04:26:24.000000 pulp_rpm-client-3.9.0.dev1611548779/pulpcore/client/pulp_rpm/models/rpm_rpm_publication.py
--rw-r--r--   0 runner    (1001) docker     (116)    12484 2021-01-25 04:26:24.000000 pulp_rpm-client-3.9.0.dev1611548779/pulpcore/client/pulp_rpm/models/rpm_rpm_publication_response.py
--rw-r--r--   0 runner    (1001) docker     (116)    18251 2021-01-25 04:26:24.000000 pulp_rpm-client-3.9.0.dev1611548779/pulpcore/client/pulp_rpm/models/rpm_rpm_remote.py
--rw-r--r--   0 runner    (1001) docker     (116)    21408 2021-01-25 04:26:24.000000 pulp_rpm-client-3.9.0.dev1611548779/pulpcore/client/pulp_rpm/models/rpm_rpm_remote_response.py
--rw-r--r--   0 runner    (1001) docker     (116)     7709 2021-01-25 04:26:24.000000 pulp_rpm-client-3.9.0.dev1611548779/pulpcore/client/pulp_rpm/models/rpm_rpm_repository.py
--rw-r--r--   0 runner    (1001) docker     (116)    11246 2021-01-25 04:26:24.000000 pulp_rpm-client-3.9.0.dev1611548779/pulpcore/client/pulp_rpm/models/rpm_rpm_repository_response.py
--rw-r--r--   0 runner    (1001) docker     (116)     4823 2021-01-25 04:26:24.000000 pulp_rpm-client-3.9.0.dev1611548779/pulpcore/client/pulp_rpm/models/rpm_update_collection.py
--rw-r--r--   0 runner    (1001) docker     (116)     5773 2021-01-25 04:26:24.000000 pulp_rpm-client-3.9.0.dev1611548779/pulpcore/client/pulp_rpm/models/rpm_update_collection_response.py
--rw-r--r--   0 runner    (1001) docker     (116)     4364 2021-01-25 04:26:24.000000 pulp_rpm-client-3.9.0.dev1611548779/pulpcore/client/pulp_rpm/models/rpm_update_record.py
--rw-r--r--   0 runner    (1001) docker     (116)    18830 2021-01-25 04:26:24.000000 pulp_rpm-client-3.9.0.dev1611548779/pulpcore/client/pulp_rpm/models/rpm_update_record_response.py
--rw-r--r--   0 runner    (1001) docker     (116)    11441 2021-01-25 04:26:25.000000 pulp_rpm-client-3.9.0.dev1611548779/pulpcore/client/pulp_rpm/models/variant_response.py
--rw-r--r--   0 runner    (1001) docker     (116)    12311 2021-01-25 04:26:25.000000 pulp_rpm-client-3.9.0.dev1611548779/pulpcore/client/pulp_rpm/rest.py
--rw-r--r--   0 runner    (1001) docker     (116)       69 2021-01-25 04:26:26.000000 pulp_rpm-client-3.9.0.dev1611548779/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     1114 2021-01-25 04:26:25.000000 pulp_rpm-client-3.9.0.dev1611548779/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-25 04:26:26.000000 pulp_rpm-client-3.9.0.dev1611548779/test/
--rw-r--r--   0 runner    (1001) docker     (116)     1688 2021-01-25 04:26:24.000000 pulp_rpm-client-3.9.0.dev1611548779/test/test_addon_response.py
--rw-r--r--   0 runner    (1001) docker     (116)     1832 2021-01-25 04:26:24.000000 pulp_rpm-client-3.9.0.dev1611548779/test/test_artifact_response.py
--rw-r--r--   0 runner    (1001) docker     (116)     1547 2021-01-25 04:26:24.000000 pulp_rpm-client-3.9.0.dev1611548779/test/test_async_operation_response.py
--rw-r--r--   0 runner    (1001) docker     (116)     1544 2021-01-25 04:26:24.000000 pulp_rpm-client-3.9.0.dev1611548779/test/test_checksum_response.py
--rw-r--r--   0 runner    (1001) docker     (116)     1192 2021-01-25 04:26:25.000000 pulp_rpm-client-3.9.0.dev1611548779/test/test_content_advisories_api.py
--rw-r--r--   0 runner    (1001) docker     (116)     1111 2021-01-25 04:26:25.000000 pulp_rpm-client-3.9.0.dev1611548779/test/test_content_distribution_trees_api.py
--rw-r--r--   0 runner    (1001) docker     (116)     1240 2021-01-25 04:26:25.000000 pulp_rpm-client-3.9.0.dev1611548779/test/test_content_modulemd_defaults_api.py
--rw-r--r--   0 runner    (1001) docker     (116)     1169 2021-01-25 04:26:25.000000 pulp_rpm-client-3.9.0.dev1611548779/test/test_content_modulemds_api.py
--rw-r--r--   0 runner    (1001) docker     (116)     1107 2021-01-25 04:26:25.000000 pulp_rpm-client-3.9.0.dev1611548779/test/test_content_packagecategories_api.py
--rw-r--r--   0 runner    (1001) docker     (116)     1125 2021-01-25 04:26:25.000000 pulp_rpm-client-3.9.0.dev1611548779/test/test_content_packageenvironments_api.py
--rw-r--r--   0 runner    (1001) docker     (116)     1077 2021-01-25 04:26:25.000000 pulp_rpm-client-3.9.0.dev1611548779/test/test_content_packagegroups_api.py
--rw-r--r--   0 runner    (1001) docker     (116)     1103 2021-01-25 04:26:25.000000 pulp_rpm-client-3.9.0.dev1611548779/test/test_content_packagelangpacks_api.py
--rw-r--r--   0 runner    (1001) docker     (116)     1160 2021-01-25 04:26:25.000000 pulp_rpm-client-3.9.0.dev1611548779/test/test_content_packages_api.py
--rw-r--r--   0 runner    (1001) docker     (116)     1115 2021-01-25 04:26:25.000000 pulp_rpm-client-3.9.0.dev1611548779/test/test_content_repo_metadata_files_api.py
--rw-r--r--   0 runner    (1001) docker     (116)     1591 2021-01-25 04:26:24.000000 pulp_rpm-client-3.9.0.dev1611548779/test/test_content_summary.py
--rw-r--r--   0 runner    (1001) docker     (116)     1681 2021-01-25 04:26:24.000000 pulp_rpm-client-3.9.0.dev1611548779/test/test_content_summary_response.py
--rw-r--r--   0 runner    (1001) docker     (116)     1395 2021-01-25 04:26:24.000000 pulp_rpm-client-3.9.0.dev1611548779/test/test_copy.py
--rw-r--r--   0 runner    (1001) docker     (116)     1611 2021-01-25 04:26:25.000000 pulp_rpm-client-3.9.0.dev1611548779/test/test_distributions_rpm_api.py
--rw-r--r--   0 runner    (1001) docker     (116)     1637 2021-01-25 04:26:24.000000 pulp_rpm-client-3.9.0.dev1611548779/test/test_image_response.py
--rw-r--r--   0 runner    (1001) docker     (116)     1516 2021-01-25 04:26:24.000000 pulp_rpm-client-3.9.0.dev1611548779/test/test_metadata_checksum_type_enum.py
--rw-r--r--   0 runner    (1001) docker     (116)     1505 2021-01-25 04:26:24.000000 pulp_rpm-client-3.9.0.dev1611548779/test/test_package_checksum_type_enum.py
--rw-r--r--   0 runner    (1001) docker     (116)     2318 2021-01-25 04:26:24.000000 pulp_rpm-client-3.9.0.dev1611548779/test/test_paginated_repository_version_response_list.py
--rw-r--r--   0 runner    (1001) docker     (116)     4412 2021-01-25 04:26:24.000000 pulp_rpm-client-3.9.0.dev1611548779/test/test_paginatedrpm_distribution_tree_response_list.py
--rw-r--r--   0 runner    (1001) docker     (116)     2651 2021-01-25 04:26:24.000000 pulp_rpm-client-3.9.0.dev1611548779/test/test_paginatedrpm_modulemd_defaults_response_list.py
--rw-r--r--   0 runner    (1001) docker     (116)     2864 2021-01-25 04:26:24.000000 pulp_rpm-client-3.9.0.dev1611548779/test/test_paginatedrpm_modulemd_response_list.py
--rw-r--r--   0 runner    (1001) docker     (116)     2695 2021-01-25 04:26:24.000000 pulp_rpm-client-3.9.0.dev1611548779/test/test_paginatedrpm_package_category_response_list.py
--rw-r--r--   0 runner    (1001) docker     (116)     2829 2021-01-25 04:26:24.000000 pulp_rpm-client-3.9.0.dev1611548779/test/test_paginatedrpm_package_environment_response_list.py
--rw-r--r--   0 runner    (1001) docker     (116)     2785 2021-01-25 04:26:24.000000 pulp_rpm-client-3.9.0.dev1611548779/test/test_paginatedrpm_package_group_response_list.py
--rw-r--r--   0 runner    (1001) docker     (116)     2339 2021-01-25 04:26:24.000000 pulp_rpm-client-3.9.0.dev1611548779/test/test_paginatedrpm_package_langpacks_response_list.py
--rw-r--r--   0 runner    (1001) docker     (116)     4382 2021-01-25 04:26:24.000000 pulp_rpm-client-3.9.0.dev1611548779/test/test_paginatedrpm_package_response_list.py
--rw-r--r--   0 runner    (1001) docker     (116)     2662 2021-01-25 04:26:24.000000 pulp_rpm-client-3.9.0.dev1611548779/test/test_paginatedrpm_repo_metadata_file_response_list.py
--rw-r--r--   0 runner    (1001) docker     (116)     2411 2021-01-25 04:26:24.000000 pulp_rpm-client-3.9.0.dev1611548779/test/test_paginatedrpm_rpm_distribution_response_list.py
--rw-r--r--   0 runner    (1001) docker     (116)     2525 2021-01-25 04:26:24.000000 pulp_rpm-client-3.9.0.dev1611548779/test/test_paginatedrpm_rpm_publication_response_list.py
--rw-r--r--   0 runner    (1001) docker     (116)     2954 2021-01-25 04:26:24.000000 pulp_rpm-client-3.9.0.dev1611548779/test/test_paginatedrpm_rpm_remote_response_list.py
--rw-r--r--   0 runner    (1001) docker     (116)     2504 2021-01-25 04:26:24.000000 pulp_rpm-client-3.9.0.dev1611548779/test/test_paginatedrpm_rpm_repository_response_list.py
--rw-r--r--   0 runner    (1001) docker     (116)     3423 2021-01-25 04:26:24.000000 pulp_rpm-client-3.9.0.dev1611548779/test/test_paginatedrpm_update_record_response_list.py
--rw-r--r--   0 runner    (1001) docker     (116)     1660 2021-01-25 04:26:24.000000 pulp_rpm-client-3.9.0.dev1611548779/test/test_patchedrpm_rpm_distribution.py
--rw-r--r--   0 runner    (1001) docker     (116)     2037 2021-01-25 04:26:24.000000 pulp_rpm-client-3.9.0.dev1611548779/test/test_patchedrpm_rpm_remote.py
--rw-r--r--   0 runner    (1001) docker     (116)     1692 2021-01-25 04:26:24.000000 pulp_rpm-client-3.9.0.dev1611548779/test/test_patchedrpm_rpm_repository.py
--rw-r--r--   0 runner    (1001) docker     (116)     1358 2021-01-25 04:26:24.000000 pulp_rpm-client-3.9.0.dev1611548779/test/test_policy_enum.py
--rw-r--r--   0 runner    (1001) docker     (116)     1317 2021-01-25 04:26:25.000000 pulp_rpm-client-3.9.0.dev1611548779/test/test_publications_rpm_api.py
--rw-r--r--   0 runner    (1001) docker     (116)     1539 2021-01-25 04:26:25.000000 pulp_rpm-client-3.9.0.dev1611548779/test/test_remotes_rpm_api.py
--rw-r--r--   0 runner    (1001) docker     (116)     1848 2021-01-25 04:26:25.000000 pulp_rpm-client-3.9.0.dev1611548779/test/test_repositories_rpm_api.py
--rw-r--r--   0 runner    (1001) docker     (116)     1329 2021-01-25 04:26:25.000000 pulp_rpm-client-3.9.0.dev1611548779/test/test_repositories_rpm_versions_api.py
--rw-r--r--   0 runner    (1001) docker     (116)     1750 2021-01-25 04:26:24.000000 pulp_rpm-client-3.9.0.dev1611548779/test/test_repository_add_remove_content.py
--rw-r--r--   0 runner    (1001) docker     (116)     1470 2021-01-25 04:26:24.000000 pulp_rpm-client-3.9.0.dev1611548779/test/test_repository_version.py
--rw-r--r--   0 runner    (1001) docker     (116)     1775 2021-01-25 04:26:24.000000 pulp_rpm-client-3.9.0.dev1611548779/test/test_repository_version_response.py
--rw-r--r--   0 runner    (1001) docker     (116)      880 2021-01-25 04:26:25.000000 pulp_rpm-client-3.9.0.dev1611548779/test/test_rpm_copy_api.py
--rw-r--r--   0 runner    (1001) docker     (116)     5443 2021-01-25 04:26:24.000000 pulp_rpm-client-3.9.0.dev1611548779/test/test_rpm_distribution_tree_response.py
--rw-r--r--   0 runner    (1001) docker     (116)     2072 2021-01-25 04:26:24.000000 pulp_rpm-client-3.9.0.dev1611548779/test/test_rpm_modulemd.py
--rw-r--r--   0 runner    (1001) docker     (116)     1829 2021-01-25 04:26:24.000000 pulp_rpm-client-3.9.0.dev1611548779/test/test_rpm_modulemd_defaults.py
--rw-r--r--   0 runner    (1001) docker     (116)     2188 2021-01-25 04:26:24.000000 pulp_rpm-client-3.9.0.dev1611548779/test/test_rpm_modulemd_defaults_response.py
--rw-r--r--   0 runner    (1001) docker     (116)     2545 2021-01-25 04:26:24.000000 pulp_rpm-client-3.9.0.dev1611548779/test/test_rpm_modulemd_response.py
--rw-r--r--   0 runner    (1001) docker     (116)     1539 2021-01-25 04:26:24.000000 pulp_rpm-client-3.9.0.dev1611548779/test/test_rpm_package.py
--rw-r--r--   0 runner    (1001) docker     (116)     2532 2021-01-25 04:26:24.000000 pulp_rpm-client-3.9.0.dev1611548779/test/test_rpm_package_category_response.py
--rw-r--r--   0 runner    (1001) docker     (116)     2738 2021-01-25 04:26:24.000000 pulp_rpm-client-3.9.0.dev1611548779/test/test_rpm_package_environment_response.py
--rw-r--r--   0 runner    (1001) docker     (116)     2601 2021-01-25 04:26:24.000000 pulp_rpm-client-3.9.0.dev1611548779/test/test_rpm_package_group_response.py
--rw-r--r--   0 runner    (1001) docker     (116)     1907 2021-01-25 04:26:24.000000 pulp_rpm-client-3.9.0.dev1611548779/test/test_rpm_package_langpacks_response.py
--rw-r--r--   0 runner    (1001) docker     (116)     3534 2021-01-25 04:26:24.000000 pulp_rpm-client-3.9.0.dev1611548779/test/test_rpm_package_response.py
--rw-r--r--   0 runner    (1001) docker     (116)     2189 2021-01-25 04:26:24.000000 pulp_rpm-client-3.9.0.dev1611548779/test/test_rpm_repo_metadata_file_response.py
--rw-r--r--   0 runner    (1001) docker     (116)     1649 2021-01-25 04:26:24.000000 pulp_rpm-client-3.9.0.dev1611548779/test/test_rpm_repository_sync_url.py
--rw-r--r--   0 runner    (1001) docker     (116)     1644 2021-01-25 04:26:24.000000 pulp_rpm-client-3.9.0.dev1611548779/test/test_rpm_rpm_distribution.py
--rw-r--r--   0 runner    (1001) docker     (116)     1911 2021-01-25 04:26:24.000000 pulp_rpm-client-3.9.0.dev1611548779/test/test_rpm_rpm_distribution_response.py
--rw-r--r--   0 runner    (1001) docker     (116)     1716 2021-01-25 04:26:24.000000 pulp_rpm-client-3.9.0.dev1611548779/test/test_rpm_rpm_publication.py
--rw-r--r--   0 runner    (1001) docker     (116)     1950 2021-01-25 04:26:24.000000 pulp_rpm-client-3.9.0.dev1611548779/test/test_rpm_rpm_publication_response.py
--rw-r--r--   0 runner    (1001) docker     (116)     2015 2021-01-25 04:26:24.000000 pulp_rpm-client-3.9.0.dev1611548779/test/test_rpm_rpm_remote.py
--rw-r--r--   0 runner    (1001) docker     (116)     2364 2021-01-25 04:26:24.000000 pulp_rpm-client-3.9.0.dev1611548779/test/test_rpm_rpm_remote_response.py
--rw-r--r--   0 runner    (1001) docker     (116)     1643 2021-01-25 04:26:24.000000 pulp_rpm-client-3.9.0.dev1611548779/test/test_rpm_rpm_repository.py
--rw-r--r--   0 runner    (1001) docker     (116)     1959 2021-01-25 04:26:24.000000 pulp_rpm-client-3.9.0.dev1611548779/test/test_rpm_rpm_repository_response.py
--rw-r--r--   0 runner    (1001) docker     (116)     1644 2021-01-25 04:26:24.000000 pulp_rpm-client-3.9.0.dev1611548779/test/test_rpm_update_collection.py
--rw-r--r--   0 runner    (1001) docker     (116)     1898 2021-01-25 04:26:24.000000 pulp_rpm-client-3.9.0.dev1611548779/test/test_rpm_update_collection_response.py
--rw-r--r--   0 runner    (1001) docker     (116)     1488 2021-01-25 04:26:24.000000 pulp_rpm-client-3.9.0.dev1611548779/test/test_rpm_update_record.py
--rw-r--r--   0 runner    (1001) docker     (116)     2684 2021-01-25 04:26:24.000000 pulp_rpm-client-3.9.0.dev1611548779/test/test_rpm_update_record_response.py
--rw-r--r--   0 runner    (1001) docker     (116)     2099 2021-01-25 04:26:25.000000 pulp_rpm-client-3.9.0.dev1611548779/test/test_variant_response.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-11 20:51:37.000000 pulp_rpm-client-3.9.1/
+-rw-r--r--   0 runner    (1001) docker     (121)      352 2021-03-11 20:51:37.000000 pulp_rpm-client-3.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)    14801 2021-03-11 20:51:36.000000 pulp_rpm-client-3.9.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-11 20:51:37.000000 pulp_rpm-client-3.9.1/pulp_rpm_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)      352 2021-03-11 20:51:37.000000 pulp_rpm-client-3.9.1/pulp_rpm_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     8092 2021-03-11 20:51:37.000000 pulp_rpm-client-3.9.1/pulp_rpm_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-03-11 20:51:37.000000 pulp_rpm-client-3.9.1/pulp_rpm_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       48 2021-03-11 20:51:37.000000 pulp_rpm-client-3.9.1/pulp_rpm_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        9 2021-03-11 20:51:37.000000 pulp_rpm-client-3.9.1/pulp_rpm_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-11 20:51:37.000000 pulp_rpm-client-3.9.1/pulpcore/
+-rw-r--r--   0 runner    (1001) docker     (121)       75 2021-03-11 20:51:36.000000 pulp_rpm-client-3.9.1/pulpcore/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-11 20:51:37.000000 pulp_rpm-client-3.9.1/pulpcore/client/
+-rw-r--r--   0 runner    (1001) docker     (121)       75 2021-03-11 20:51:36.000000 pulp_rpm-client-3.9.1/pulpcore/client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-11 20:51:37.000000 pulp_rpm-client-3.9.1/pulpcore/client/pulp_rpm/
+-rw-r--r--   0 runner    (1001) docker     (121)     7905 2021-03-11 20:51:36.000000 pulp_rpm-client-3.9.1/pulpcore/client/pulp_rpm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-11 20:51:37.000000 pulp_rpm-client-3.9.1/pulpcore/client/pulp_rpm/api/
+-rw-r--r--   0 runner    (1001) docker     (121)     1504 2021-03-11 20:51:36.000000 pulp_rpm-client-3.9.1/pulpcore/client/pulp_rpm/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    23621 2021-03-11 20:51:36.000000 pulp_rpm-client-3.9.1/pulpcore/client/pulp_rpm/api/content_advisories_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14315 2021-03-11 20:51:36.000000 pulp_rpm-client-3.9.1/pulpcore/client/pulp_rpm/api/content_distribution_trees_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)    24428 2021-03-11 20:51:36.000000 pulp_rpm-client-3.9.1/pulpcore/client/pulp_rpm/api/content_modulemd_defaults_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)    26435 2021-03-11 20:51:36.000000 pulp_rpm-client-3.9.1/pulpcore/client/pulp_rpm/api/content_modulemds_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14280 2021-03-11 20:51:36.000000 pulp_rpm-client-3.9.1/pulpcore/client/pulp_rpm/api/content_packagecategories_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14374 2021-03-11 20:51:36.000000 pulp_rpm-client-3.9.1/pulpcore/client/pulp_rpm/api/content_packageenvironments_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14182 2021-03-11 20:51:36.000000 pulp_rpm-client-3.9.1/pulpcore/client/pulp_rpm/api/content_packagegroups_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14308 2021-03-11 20:51:36.000000 pulp_rpm-client-3.9.1/pulpcore/client/pulp_rpm/api/content_packagelangpacks_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)    27731 2021-03-11 20:51:36.000000 pulp_rpm-client-3.9.1/pulpcore/client/pulp_rpm/api/content_packages_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14332 2021-03-11 20:51:36.000000 pulp_rpm-client-3.9.1/pulpcore/client/pulp_rpm/api/content_repo_metadata_files_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)    39908 2021-03-11 20:51:36.000000 pulp_rpm-client-3.9.1/pulpcore/client/pulp_rpm/api/distributions_rpm_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)    25967 2021-03-11 20:51:36.000000 pulp_rpm-client-3.9.1/pulpcore/client/pulp_rpm/api/publications_rpm_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)    40092 2021-03-11 20:51:36.000000 pulp_rpm-client-3.9.1/pulpcore/client/pulp_rpm/api/remotes_rpm_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)    51026 2021-03-11 20:51:36.000000 pulp_rpm-client-3.9.1/pulpcore/client/pulp_rpm/api/repositories_rpm_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)    30602 2021-03-11 20:51:36.000000 pulp_rpm-client-3.9.1/pulpcore/client/pulp_rpm/api/repositories_rpm_versions_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6171 2021-03-11 20:51:36.000000 pulp_rpm-client-3.9.1/pulpcore/client/pulp_rpm/api/rpm_copy_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)    26274 2021-03-11 20:51:36.000000 pulp_rpm-client-3.9.1/pulpcore/client/pulp_rpm/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13952 2021-03-11 20:51:36.000000 pulp_rpm-client-3.9.1/pulpcore/client/pulp_rpm/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3769 2021-03-11 20:51:36.000000 pulp_rpm-client-3.9.1/pulpcore/client/pulp_rpm/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-11 20:51:37.000000 pulp_rpm-client-3.9.1/pulpcore/client/pulp_rpm/models/
+-rw-r--r--   0 runner    (1001) docker     (121)     5982 2021-03-11 20:51:36.000000 pulp_rpm-client-3.9.1/pulpcore/client/pulp_rpm/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6899 2021-03-11 20:51:35.000000 pulp_rpm-client-3.9.1/pulpcore/client/pulp_rpm/models/addon_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10073 2021-03-11 20:51:35.000000 pulp_rpm-client-3.9.1/pulpcore/client/pulp_rpm/models/artifact_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3572 2021-03-11 20:51:35.000000 pulp_rpm-client-3.9.1/pulpcore/client/pulp_rpm/models/async_operation_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4423 2021-03-11 20:51:35.000000 pulp_rpm-client-3.9.1/pulpcore/client/pulp_rpm/models/checksum_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5072 2021-03-11 20:51:35.000000 pulp_rpm-client-3.9.1/pulpcore/client/pulp_rpm/models/content_summary.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5200 2021-03-11 20:51:35.000000 pulp_rpm-client-3.9.1/pulpcore/client/pulp_rpm/models/content_summary_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4561 2021-03-11 20:51:35.000000 pulp_rpm-client-3.9.1/pulpcore/client/pulp_rpm/models/copy.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5870 2021-03-11 20:51:35.000000 pulp_rpm-client-3.9.1/pulpcore/client/pulp_rpm/models/image_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2999 2021-03-11 20:51:35.000000 pulp_rpm-client-3.9.1/pulpcore/client/pulp_rpm/models/metadata_checksum_type_enum.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2995 2021-03-11 20:51:35.000000 pulp_rpm-client-3.9.1/pulpcore/client/pulp_rpm/models/package_checksum_type_enum.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5675 2021-03-11 20:51:35.000000 pulp_rpm-client-3.9.1/pulpcore/client/pulp_rpm/models/paginated_repository_version_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5721 2021-03-11 20:51:35.000000 pulp_rpm-client-3.9.1/pulpcore/client/pulp_rpm/models/paginatedrpm_distribution_tree_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5721 2021-03-11 20:51:35.000000 pulp_rpm-client-3.9.1/pulpcore/client/pulp_rpm/models/paginatedrpm_modulemd_defaults_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5537 2021-03-11 20:51:35.000000 pulp_rpm-client-3.9.1/pulpcore/client/pulp_rpm/models/paginatedrpm_modulemd_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5698 2021-03-11 20:51:35.000000 pulp_rpm-client-3.9.1/pulpcore/client/pulp_rpm/models/paginatedrpm_package_category_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5767 2021-03-11 20:51:35.000000 pulp_rpm-client-3.9.1/pulpcore/client/pulp_rpm/models/paginatedrpm_package_environment_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5629 2021-03-11 20:51:35.000000 pulp_rpm-client-3.9.1/pulpcore/client/pulp_rpm/models/paginatedrpm_package_group_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5721 2021-03-11 20:51:35.000000 pulp_rpm-client-3.9.1/pulpcore/client/pulp_rpm/models/paginatedrpm_package_langpacks_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5514 2021-03-11 20:51:35.000000 pulp_rpm-client-3.9.1/pulpcore/client/pulp_rpm/models/paginatedrpm_package_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5721 2021-03-11 20:51:35.000000 pulp_rpm-client-3.9.1/pulpcore/client/pulp_rpm/models/paginatedrpm_repo_metadata_file_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5698 2021-03-11 20:51:35.000000 pulp_rpm-client-3.9.1/pulpcore/client/pulp_rpm/models/paginatedrpm_rpm_distribution_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5675 2021-03-11 20:51:35.000000 pulp_rpm-client-3.9.1/pulpcore/client/pulp_rpm/models/paginatedrpm_rpm_publication_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5560 2021-03-11 20:51:35.000000 pulp_rpm-client-3.9.1/pulpcore/client/pulp_rpm/models/paginatedrpm_rpm_remote_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5652 2021-03-11 20:51:35.000000 pulp_rpm-client-3.9.1/pulpcore/client/pulp_rpm/models/paginatedrpm_rpm_repository_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5629 2021-03-11 20:51:35.000000 pulp_rpm-client-3.9.1/pulpcore/client/pulp_rpm/models/paginatedrpm_update_record_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7059 2021-03-11 20:51:35.000000 pulp_rpm-client-3.9.1/pulpcore/client/pulp_rpm/models/patchedrpm_rpm_distribution.py
+-rw-r--r--   0 runner    (1001) docker     (121)    20004 2021-03-11 20:51:35.000000 pulp_rpm-client-3.9.1/pulpcore/client/pulp_rpm/models/patchedrpm_rpm_remote.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8493 2021-03-11 20:51:35.000000 pulp_rpm-client-3.9.1/pulpcore/client/pulp_rpm/models/patchedrpm_rpm_repository.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2859 2021-03-11 20:51:35.000000 pulp_rpm-client-3.9.1/pulpcore/client/pulp_rpm/models/policy_enum.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6396 2021-03-11 20:51:35.000000 pulp_rpm-client-3.9.1/pulpcore/client/pulp_rpm/models/repository_add_remove_content.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3698 2021-03-11 20:51:35.000000 pulp_rpm-client-3.9.1/pulpcore/client/pulp_rpm/models/repository_version.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7166 2021-03-11 20:51:35.000000 pulp_rpm-client-3.9.1/pulpcore/client/pulp_rpm/models/repository_version_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)    20723 2021-03-11 20:51:35.000000 pulp_rpm-client-3.9.1/pulpcore/client/pulp_rpm/models/rpm_distribution_tree_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12702 2021-03-11 20:51:35.000000 pulp_rpm-client-3.9.1/pulpcore/client/pulp_rpm/models/rpm_modulemd.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9115 2021-03-11 20:51:35.000000 pulp_rpm-client-3.9.1/pulpcore/client/pulp_rpm/models/rpm_modulemd_defaults.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12703 2021-03-11 20:51:35.000000 pulp_rpm-client-3.9.1/pulpcore/client/pulp_rpm/models/rpm_modulemd_defaults_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16290 2021-03-11 20:51:35.000000 pulp_rpm-client-3.9.1/pulpcore/client/pulp_rpm/models/rpm_modulemd_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6191 2021-03-11 20:51:35.000000 pulp_rpm-client-3.9.1/pulpcore/client/pulp_rpm/models/rpm_package.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11350 2021-03-11 20:51:35.000000 pulp_rpm-client-3.9.1/pulpcore/client/pulp_rpm/models/rpm_package_category_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12355 2021-03-11 20:51:35.000000 pulp_rpm-client-3.9.1/pulpcore/client/pulp_rpm/models/rpm_package_environment_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13787 2021-03-11 20:51:35.000000 pulp_rpm-client-3.9.1/pulpcore/client/pulp_rpm/models/rpm_package_group_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5846 2021-03-11 20:51:35.000000 pulp_rpm-client-3.9.1/pulpcore/client/pulp_rpm/models/rpm_package_langpacks_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)    40009 2021-03-11 20:51:35.000000 pulp_rpm-client-3.9.1/pulpcore/client/pulp_rpm/models/rpm_package_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13956 2021-03-11 20:51:35.000000 pulp_rpm-client-3.9.1/pulpcore/client/pulp_rpm/models/rpm_repo_metadata_file_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6693 2021-03-11 20:51:36.000000 pulp_rpm-client-3.9.1/pulpcore/client/pulp_rpm/models/rpm_repository_sync_url.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7204 2021-03-11 20:51:36.000000 pulp_rpm-client-3.9.1/pulpcore/client/pulp_rpm/models/rpm_rpm_distribution.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9926 2021-03-11 20:51:36.000000 pulp_rpm-client-3.9.1/pulpcore/client/pulp_rpm/models/rpm_rpm_distribution_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10605 2021-03-11 20:51:36.000000 pulp_rpm-client-3.9.1/pulpcore/client/pulp_rpm/models/rpm_rpm_publication.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12484 2021-03-11 20:51:36.000000 pulp_rpm-client-3.9.1/pulpcore/client/pulp_rpm/models/rpm_rpm_publication_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)    19779 2021-03-11 20:51:36.000000 pulp_rpm-client-3.9.1/pulpcore/client/pulp_rpm/models/rpm_rpm_remote.py
+-rw-r--r--   0 runner    (1001) docker     (121)    23000 2021-03-11 20:51:36.000000 pulp_rpm-client-3.9.1/pulpcore/client/pulp_rpm/models/rpm_rpm_remote_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8451 2021-03-11 20:51:36.000000 pulp_rpm-client-3.9.1/pulpcore/client/pulp_rpm/models/rpm_rpm_repository.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12020 2021-03-11 20:51:36.000000 pulp_rpm-client-3.9.1/pulpcore/client/pulp_rpm/models/rpm_rpm_repository_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4823 2021-03-11 20:51:36.000000 pulp_rpm-client-3.9.1/pulpcore/client/pulp_rpm/models/rpm_update_collection.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5773 2021-03-11 20:51:36.000000 pulp_rpm-client-3.9.1/pulpcore/client/pulp_rpm/models/rpm_update_collection_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4364 2021-03-11 20:51:36.000000 pulp_rpm-client-3.9.1/pulpcore/client/pulp_rpm/models/rpm_update_record.py
+-rw-r--r--   0 runner    (1001) docker     (121)    18830 2021-03-11 20:51:36.000000 pulp_rpm-client-3.9.1/pulpcore/client/pulp_rpm/models/rpm_update_record_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11441 2021-03-11 20:51:36.000000 pulp_rpm-client-3.9.1/pulpcore/client/pulp_rpm/models/variant_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12311 2021-03-11 20:51:36.000000 pulp_rpm-client-3.9.1/pulpcore/client/pulp_rpm/rest.py
+-rw-r--r--   0 runner    (1001) docker     (121)       69 2021-03-11 20:51:37.000000 pulp_rpm-client-3.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1099 2021-03-11 20:51:36.000000 pulp_rpm-client-3.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-11 20:51:37.000000 pulp_rpm-client-3.9.1/test/
+-rw-r--r--   0 runner    (1001) docker     (121)     1688 2021-03-11 20:51:35.000000 pulp_rpm-client-3.9.1/test/test_addon_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1832 2021-03-11 20:51:35.000000 pulp_rpm-client-3.9.1/test/test_artifact_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1547 2021-03-11 20:51:35.000000 pulp_rpm-client-3.9.1/test/test_async_operation_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1544 2021-03-11 20:51:35.000000 pulp_rpm-client-3.9.1/test/test_checksum_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1192 2021-03-11 20:51:36.000000 pulp_rpm-client-3.9.1/test/test_content_advisories_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1111 2021-03-11 20:51:36.000000 pulp_rpm-client-3.9.1/test/test_content_distribution_trees_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1240 2021-03-11 20:51:36.000000 pulp_rpm-client-3.9.1/test/test_content_modulemd_defaults_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1169 2021-03-11 20:51:36.000000 pulp_rpm-client-3.9.1/test/test_content_modulemds_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1107 2021-03-11 20:51:36.000000 pulp_rpm-client-3.9.1/test/test_content_packagecategories_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1125 2021-03-11 20:51:36.000000 pulp_rpm-client-3.9.1/test/test_content_packageenvironments_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1077 2021-03-11 20:51:36.000000 pulp_rpm-client-3.9.1/test/test_content_packagegroups_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1103 2021-03-11 20:51:36.000000 pulp_rpm-client-3.9.1/test/test_content_packagelangpacks_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1160 2021-03-11 20:51:36.000000 pulp_rpm-client-3.9.1/test/test_content_packages_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1115 2021-03-11 20:51:36.000000 pulp_rpm-client-3.9.1/test/test_content_repo_metadata_files_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1591 2021-03-11 20:51:35.000000 pulp_rpm-client-3.9.1/test/test_content_summary.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1681 2021-03-11 20:51:35.000000 pulp_rpm-client-3.9.1/test/test_content_summary_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1395 2021-03-11 20:51:35.000000 pulp_rpm-client-3.9.1/test/test_copy.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1611 2021-03-11 20:51:36.000000 pulp_rpm-client-3.9.1/test/test_distributions_rpm_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1637 2021-03-11 20:51:35.000000 pulp_rpm-client-3.9.1/test/test_image_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1516 2021-03-11 20:51:35.000000 pulp_rpm-client-3.9.1/test/test_metadata_checksum_type_enum.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1505 2021-03-11 20:51:35.000000 pulp_rpm-client-3.9.1/test/test_package_checksum_type_enum.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2318 2021-03-11 20:51:35.000000 pulp_rpm-client-3.9.1/test/test_paginated_repository_version_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4412 2021-03-11 20:51:35.000000 pulp_rpm-client-3.9.1/test/test_paginatedrpm_distribution_tree_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2651 2021-03-11 20:51:35.000000 pulp_rpm-client-3.9.1/test/test_paginatedrpm_modulemd_defaults_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2864 2021-03-11 20:51:35.000000 pulp_rpm-client-3.9.1/test/test_paginatedrpm_modulemd_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2695 2021-03-11 20:51:35.000000 pulp_rpm-client-3.9.1/test/test_paginatedrpm_package_category_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2829 2021-03-11 20:51:35.000000 pulp_rpm-client-3.9.1/test/test_paginatedrpm_package_environment_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2785 2021-03-11 20:51:35.000000 pulp_rpm-client-3.9.1/test/test_paginatedrpm_package_group_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2339 2021-03-11 20:51:35.000000 pulp_rpm-client-3.9.1/test/test_paginatedrpm_package_langpacks_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4382 2021-03-11 20:51:35.000000 pulp_rpm-client-3.9.1/test/test_paginatedrpm_package_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2662 2021-03-11 20:51:35.000000 pulp_rpm-client-3.9.1/test/test_paginatedrpm_repo_metadata_file_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2509 2021-03-11 20:51:35.000000 pulp_rpm-client-3.9.1/test/test_paginatedrpm_rpm_distribution_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2525 2021-03-11 20:51:35.000000 pulp_rpm-client-3.9.1/test/test_paginatedrpm_rpm_publication_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3094 2021-03-11 20:51:35.000000 pulp_rpm-client-3.9.1/test/test_paginatedrpm_rpm_remote_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2602 2021-03-11 20:51:35.000000 pulp_rpm-client-3.9.1/test/test_paginatedrpm_rpm_repository_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3423 2021-03-11 20:51:35.000000 pulp_rpm-client-3.9.1/test/test_paginatedrpm_update_record_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1697 2021-03-11 20:51:35.000000 pulp_rpm-client-3.9.1/test/test_patchedrpm_rpm_distribution.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2108 2021-03-11 20:51:35.000000 pulp_rpm-client-3.9.1/test/test_patchedrpm_rpm_remote.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1729 2021-03-11 20:51:35.000000 pulp_rpm-client-3.9.1/test/test_patchedrpm_rpm_repository.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1358 2021-03-11 20:51:35.000000 pulp_rpm-client-3.9.1/test/test_policy_enum.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1317 2021-03-11 20:51:36.000000 pulp_rpm-client-3.9.1/test/test_publications_rpm_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1539 2021-03-11 20:51:36.000000 pulp_rpm-client-3.9.1/test/test_remotes_rpm_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1848 2021-03-11 20:51:36.000000 pulp_rpm-client-3.9.1/test/test_repositories_rpm_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1329 2021-03-11 20:51:36.000000 pulp_rpm-client-3.9.1/test/test_repositories_rpm_versions_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1750 2021-03-11 20:51:35.000000 pulp_rpm-client-3.9.1/test/test_repository_add_remove_content.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1470 2021-03-11 20:51:35.000000 pulp_rpm-client-3.9.1/test/test_repository_version.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1775 2021-03-11 20:51:35.000000 pulp_rpm-client-3.9.1/test/test_repository_version_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)      880 2021-03-11 20:51:36.000000 pulp_rpm-client-3.9.1/test/test_rpm_copy_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5443 2021-03-11 20:51:35.000000 pulp_rpm-client-3.9.1/test/test_rpm_distribution_tree_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2072 2021-03-11 20:51:35.000000 pulp_rpm-client-3.9.1/test/test_rpm_modulemd.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1829 2021-03-11 20:51:35.000000 pulp_rpm-client-3.9.1/test/test_rpm_modulemd_defaults.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2188 2021-03-11 20:51:35.000000 pulp_rpm-client-3.9.1/test/test_rpm_modulemd_defaults_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2545 2021-03-11 20:51:35.000000 pulp_rpm-client-3.9.1/test/test_rpm_modulemd_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1539 2021-03-11 20:51:35.000000 pulp_rpm-client-3.9.1/test/test_rpm_package.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2532 2021-03-11 20:51:35.000000 pulp_rpm-client-3.9.1/test/test_rpm_package_category_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2738 2021-03-11 20:51:35.000000 pulp_rpm-client-3.9.1/test/test_rpm_package_environment_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2601 2021-03-11 20:51:35.000000 pulp_rpm-client-3.9.1/test/test_rpm_package_group_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1907 2021-03-11 20:51:35.000000 pulp_rpm-client-3.9.1/test/test_rpm_package_langpacks_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3534 2021-03-11 20:51:35.000000 pulp_rpm-client-3.9.1/test/test_rpm_package_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2189 2021-03-11 20:51:35.000000 pulp_rpm-client-3.9.1/test/test_rpm_repo_metadata_file_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1649 2021-03-11 20:51:36.000000 pulp_rpm-client-3.9.1/test/test_rpm_repository_sync_url.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1681 2021-03-11 20:51:36.000000 pulp_rpm-client-3.9.1/test/test_rpm_rpm_distribution.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2001 2021-03-11 20:51:36.000000 pulp_rpm-client-3.9.1/test/test_rpm_rpm_distribution_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1716 2021-03-11 20:51:36.000000 pulp_rpm-client-3.9.1/test/test_rpm_rpm_publication.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1950 2021-03-11 20:51:36.000000 pulp_rpm-client-3.9.1/test/test_rpm_rpm_publication_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2086 2021-03-11 20:51:36.000000 pulp_rpm-client-3.9.1/test/test_rpm_rpm_remote.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2488 2021-03-11 20:51:36.000000 pulp_rpm-client-3.9.1/test/test_rpm_rpm_remote_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1680 2021-03-11 20:51:36.000000 pulp_rpm-client-3.9.1/test/test_rpm_rpm_repository.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2049 2021-03-11 20:51:36.000000 pulp_rpm-client-3.9.1/test/test_rpm_rpm_repository_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1644 2021-03-11 20:51:36.000000 pulp_rpm-client-3.9.1/test/test_rpm_update_collection.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1898 2021-03-11 20:51:36.000000 pulp_rpm-client-3.9.1/test/test_rpm_update_collection_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1488 2021-03-11 20:51:36.000000 pulp_rpm-client-3.9.1/test/test_rpm_update_record.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2684 2021-03-11 20:51:36.000000 pulp_rpm-client-3.9.1/test/test_rpm_update_record_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2099 2021-03-11 20:51:36.000000 pulp_rpm-client-3.9.1/test/test_variant_response.py
```

### Comparing `pulp_rpm-client-3.9.0.dev1611548779/README.md` & `pulp_rpm-client-3.9.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # pulp_rpm-client
 Fetch, Upload, Organize, and Distribute Software Packages
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
 - API version: v3
-- Package version: 3.9.0.dev01611548779
+- Package version: 3.9.1
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 For more information, please visit [https://pulpproject.org](https://pulpproject.org)
 
 ## Requirements.
 
 Python 2.7 and 3.4+
```

### Comparing `pulp_rpm-client-3.9.0.dev1611548779/pulp_rpm_client.egg-info/SOURCES.txt` & `pulp_rpm-client-3.9.1/pulp_rpm_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulp_rpm-client-3.9.0.dev1611548779/pulpcore/client/pulp_rpm/__init__.py` & `pulp_rpm-client-3.9.1/pulpcore/client/pulp_rpm/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     Contact: pulp-list@redhat.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
-__version__ = "3.9.0.dev01611548779"
+__version__ = "3.9.1"
 
 # import apis into sdk package
 from pulpcore.client.pulp_rpm.api.content_advisories_api import ContentAdvisoriesApi
 from pulpcore.client.pulp_rpm.api.content_distribution_trees_api import ContentDistributionTreesApi
 from pulpcore.client.pulp_rpm.api.content_modulemd_defaults_api import ContentModulemdDefaultsApi
 from pulpcore.client.pulp_rpm.api.content_modulemds_api import ContentModulemdsApi
 from pulpcore.client.pulp_rpm.api.content_packagecategories_api import ContentPackagecategoriesApi
```

### Comparing `pulp_rpm-client-3.9.0.dev1611548779/pulpcore/client/pulp_rpm/api/__init__.py` & `pulp_rpm-client-3.9.1/pulpcore/client/pulp_rpm/api/__init__.py`

 * *Files identical despite different names*

### Comparing `pulp_rpm-client-3.9.0.dev1611548779/pulpcore/client/pulp_rpm/api/content_advisories_api.py` & `pulp_rpm-client-3.9.1/pulpcore/client/pulp_rpm/api/content_advisories_api.py`

 * *Files identical despite different names*

### Comparing `pulp_rpm-client-3.9.0.dev1611548779/pulpcore/client/pulp_rpm/api/content_distribution_trees_api.py` & `pulp_rpm-client-3.9.1/pulpcore/client/pulp_rpm/api/content_distribution_trees_api.py`

 * *Files identical despite different names*

### Comparing `pulp_rpm-client-3.9.0.dev1611548779/pulpcore/client/pulp_rpm/api/content_modulemd_defaults_api.py` & `pulp_rpm-client-3.9.1/pulpcore/client/pulp_rpm/api/content_modulemd_defaults_api.py`

 * *Files identical despite different names*

### Comparing `pulp_rpm-client-3.9.0.dev1611548779/pulpcore/client/pulp_rpm/api/content_modulemds_api.py` & `pulp_rpm-client-3.9.1/pulpcore/client/pulp_rpm/api/content_modulemds_api.py`

 * *Files identical despite different names*

### Comparing `pulp_rpm-client-3.9.0.dev1611548779/pulpcore/client/pulp_rpm/api/content_packagecategories_api.py` & `pulp_rpm-client-3.9.1/pulpcore/client/pulp_rpm/api/content_packagecategories_api.py`

 * *Files identical despite different names*

### Comparing `pulp_rpm-client-3.9.0.dev1611548779/pulpcore/client/pulp_rpm/api/content_packageenvironments_api.py` & `pulp_rpm-client-3.9.1/pulpcore/client/pulp_rpm/api/content_packageenvironments_api.py`

 * *Files identical despite different names*

### Comparing `pulp_rpm-client-3.9.0.dev1611548779/pulpcore/client/pulp_rpm/api/content_packagegroups_api.py` & `pulp_rpm-client-3.9.1/pulpcore/client/pulp_rpm/api/content_packagegroups_api.py`

 * *Files identical despite different names*

### Comparing `pulp_rpm-client-3.9.0.dev1611548779/pulpcore/client/pulp_rpm/api/content_packagelangpacks_api.py` & `pulp_rpm-client-3.9.1/pulpcore/client/pulp_rpm/api/content_packagelangpacks_api.py`

 * *Files identical despite different names*

### Comparing `pulp_rpm-client-3.9.0.dev1611548779/pulpcore/client/pulp_rpm/api/content_packages_api.py` & `pulp_rpm-client-3.9.1/pulpcore/client/pulp_rpm/api/content_packages_api.py`

 * *Files identical despite different names*

### Comparing `pulp_rpm-client-3.9.0.dev1611548779/pulpcore/client/pulp_rpm/api/content_repo_metadata_files_api.py` & `pulp_rpm-client-3.9.1/pulpcore/client/pulp_rpm/api/content_repo_metadata_files_api.py`

 * *Files identical despite different names*

### Comparing `pulp_rpm-client-3.9.0.dev1611548779/pulpcore/client/pulp_rpm/api/distributions_rpm_api.py` & `pulp_rpm-client-3.9.1/pulpcore/client/pulp_rpm/api/distributions_rpm_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -287,14 +287,15 @@
         :param str name: name
         :param str name__contains: name__contains
         :param str name__icontains: name__icontains
         :param str name__in: name__in
         :param str name__startswith: name__startswith
         :param int offset: The initial index from which to return the results.
         :param str ordering: Which field to use when ordering the results.
+        :param str pulp_label_select: pulp_label_select
         :param str fields: A list of fields to include in the response.
         :param str exclude_fields: A list of fields to exclude from the response.
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
@@ -325,14 +326,15 @@
         :param str name: name
         :param str name__contains: name__contains
         :param str name__icontains: name__icontains
         :param str name__in: name__in
         :param str name__startswith: name__startswith
         :param int offset: The initial index from which to return the results.
         :param str ordering: Which field to use when ordering the results.
+        :param str pulp_label_select: pulp_label_select
         :param str fields: A list of fields to include in the response.
         :param str exclude_fields: A list of fields to exclude from the response.
         :param _return_http_data_only: response data without head status code
                                        and headers
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
@@ -356,14 +358,15 @@
             'name',
             'name__contains',
             'name__icontains',
             'name__in',
             'name__startswith',
             'offset',
             'ordering',
+            'pulp_label_select',
             'fields',
             'exclude_fields'
         ]
         all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
@@ -406,14 +409,16 @@
             query_params.append(('name__in', local_var_params['name__in']))  # noqa: E501
         if 'name__startswith' in local_var_params and local_var_params['name__startswith'] is not None:  # noqa: E501
             query_params.append(('name__startswith', local_var_params['name__startswith']))  # noqa: E501
         if 'offset' in local_var_params and local_var_params['offset'] is not None:  # noqa: E501
             query_params.append(('offset', local_var_params['offset']))  # noqa: E501
         if 'ordering' in local_var_params and local_var_params['ordering'] is not None:  # noqa: E501
             query_params.append(('ordering', local_var_params['ordering']))  # noqa: E501
+        if 'pulp_label_select' in local_var_params and local_var_params['pulp_label_select'] is not None:  # noqa: E501
+            query_params.append(('pulp_label_select', local_var_params['pulp_label_select']))  # noqa: E501
         if 'fields' in local_var_params and local_var_params['fields'] is not None:  # noqa: E501
             query_params.append(('fields', local_var_params['fields']))  # noqa: E501
         if 'exclude_fields' in local_var_params and local_var_params['exclude_fields'] is not None:  # noqa: E501
             query_params.append(('exclude_fields', local_var_params['exclude_fields']))  # noqa: E501
 
         header_params = {}
```

### Comparing `pulp_rpm-client-3.9.0.dev1611548779/pulpcore/client/pulp_rpm/api/publications_rpm_api.py` & `pulp_rpm-client-3.9.1/pulpcore/client/pulp_rpm/api/publications_rpm_api.py`

 * *Files identical despite different names*

### Comparing `pulp_rpm-client-3.9.0.dev1611548779/pulpcore/client/pulp_rpm/api/remotes_rpm_api.py` & `pulp_rpm-client-3.9.1/pulpcore/client/pulp_rpm/api/remotes_rpm_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -283,14 +283,15 @@
         :param str name: name
         :param str name__contains: name__contains
         :param str name__icontains: name__icontains
         :param str name__in: name__in
         :param str name__startswith: name__startswith
         :param int offset: The initial index from which to return the results.
         :param str ordering: Which field to use when ordering the results.
+        :param str pulp_label_select: pulp_label_select
         :param str pulp_last_updated: pulp_last_updated
         :param str pulp_last_updated__gt: pulp_last_updated__gt
         :param str pulp_last_updated__gte: pulp_last_updated__gte
         :param str pulp_last_updated__lt: pulp_last_updated__lt
         :param str pulp_last_updated__lte: pulp_last_updated__lte
         :param str pulp_last_updated__range: pulp_last_updated__range
         :param str fields: A list of fields to include in the response.
@@ -323,14 +324,15 @@
         :param str name: name
         :param str name__contains: name__contains
         :param str name__icontains: name__icontains
         :param str name__in: name__in
         :param str name__startswith: name__startswith
         :param int offset: The initial index from which to return the results.
         :param str ordering: Which field to use when ordering the results.
+        :param str pulp_label_select: pulp_label_select
         :param str pulp_last_updated: pulp_last_updated
         :param str pulp_last_updated__gt: pulp_last_updated__gt
         :param str pulp_last_updated__gte: pulp_last_updated__gte
         :param str pulp_last_updated__lt: pulp_last_updated__lt
         :param str pulp_last_updated__lte: pulp_last_updated__lte
         :param str pulp_last_updated__range: pulp_last_updated__range
         :param str fields: A list of fields to include in the response.
@@ -356,14 +358,15 @@
             'name',
             'name__contains',
             'name__icontains',
             'name__in',
             'name__startswith',
             'offset',
             'ordering',
+            'pulp_label_select',
             'pulp_last_updated',
             'pulp_last_updated__gt',
             'pulp_last_updated__gte',
             'pulp_last_updated__lt',
             'pulp_last_updated__lte',
             'pulp_last_updated__range',
             'fields',
@@ -404,14 +407,16 @@
             query_params.append(('name__in', local_var_params['name__in']))  # noqa: E501
         if 'name__startswith' in local_var_params and local_var_params['name__startswith'] is not None:  # noqa: E501
             query_params.append(('name__startswith', local_var_params['name__startswith']))  # noqa: E501
         if 'offset' in local_var_params and local_var_params['offset'] is not None:  # noqa: E501
             query_params.append(('offset', local_var_params['offset']))  # noqa: E501
         if 'ordering' in local_var_params and local_var_params['ordering'] is not None:  # noqa: E501
             query_params.append(('ordering', local_var_params['ordering']))  # noqa: E501
+        if 'pulp_label_select' in local_var_params and local_var_params['pulp_label_select'] is not None:  # noqa: E501
+            query_params.append(('pulp_label_select', local_var_params['pulp_label_select']))  # noqa: E501
         if 'pulp_last_updated' in local_var_params and local_var_params['pulp_last_updated'] is not None:  # noqa: E501
             query_params.append(('pulp_last_updated', local_var_params['pulp_last_updated']))  # noqa: E501
         if 'pulp_last_updated__gt' in local_var_params and local_var_params['pulp_last_updated__gt'] is not None:  # noqa: E501
             query_params.append(('pulp_last_updated__gt', local_var_params['pulp_last_updated__gt']))  # noqa: E501
         if 'pulp_last_updated__gte' in local_var_params and local_var_params['pulp_last_updated__gte'] is not None:  # noqa: E501
             query_params.append(('pulp_last_updated__gte', local_var_params['pulp_last_updated__gte']))  # noqa: E501
         if 'pulp_last_updated__lt' in local_var_params and local_var_params['pulp_last_updated__lt'] is not None:  # noqa: E501
```

### Comparing `pulp_rpm-client-3.9.0.dev1611548779/pulpcore/client/pulp_rpm/api/repositories_rpm_api.py` & `pulp_rpm-client-3.9.1/pulpcore/client/pulp_rpm/api/repositories_rpm_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -283,14 +283,15 @@
         :param str name: name
         :param str name__contains: name__contains
         :param str name__icontains: name__icontains
         :param str name__in: name__in
         :param str name__startswith: name__startswith
         :param int offset: The initial index from which to return the results.
         :param str ordering: Which field to use when ordering the results.
+        :param str pulp_label_select: pulp_label_select
         :param str fields: A list of fields to include in the response.
         :param str exclude_fields: A list of fields to exclude from the response.
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
@@ -317,14 +318,15 @@
         :param str name: name
         :param str name__contains: name__contains
         :param str name__icontains: name__icontains
         :param str name__in: name__in
         :param str name__startswith: name__startswith
         :param int offset: The initial index from which to return the results.
         :param str ordering: Which field to use when ordering the results.
+        :param str pulp_label_select: pulp_label_select
         :param str fields: A list of fields to include in the response.
         :param str exclude_fields: A list of fields to exclude from the response.
         :param _return_http_data_only: response data without head status code
                                        and headers
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
@@ -344,14 +346,15 @@
             'name',
             'name__contains',
             'name__icontains',
             'name__in',
             'name__startswith',
             'offset',
             'ordering',
+            'pulp_label_select',
             'fields',
             'exclude_fields'
         ]
         all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
@@ -386,14 +389,16 @@
             query_params.append(('name__in', local_var_params['name__in']))  # noqa: E501
         if 'name__startswith' in local_var_params and local_var_params['name__startswith'] is not None:  # noqa: E501
             query_params.append(('name__startswith', local_var_params['name__startswith']))  # noqa: E501
         if 'offset' in local_var_params and local_var_params['offset'] is not None:  # noqa: E501
             query_params.append(('offset', local_var_params['offset']))  # noqa: E501
         if 'ordering' in local_var_params and local_var_params['ordering'] is not None:  # noqa: E501
             query_params.append(('ordering', local_var_params['ordering']))  # noqa: E501
+        if 'pulp_label_select' in local_var_params and local_var_params['pulp_label_select'] is not None:  # noqa: E501
+            query_params.append(('pulp_label_select', local_var_params['pulp_label_select']))  # noqa: E501
         if 'fields' in local_var_params and local_var_params['fields'] is not None:  # noqa: E501
             query_params.append(('fields', local_var_params['fields']))  # noqa: E501
         if 'exclude_fields' in local_var_params and local_var_params['exclude_fields'] is not None:  # noqa: E501
             query_params.append(('exclude_fields', local_var_params['exclude_fields']))  # noqa: E501
 
         header_params = {}
```

### Comparing `pulp_rpm-client-3.9.0.dev1611548779/pulpcore/client/pulp_rpm/api/repositories_rpm_versions_api.py` & `pulp_rpm-client-3.9.1/pulpcore/client/pulp_rpm/api/repositories_rpm_versions_api.py`

 * *Files identical despite different names*

### Comparing `pulp_rpm-client-3.9.0.dev1611548779/pulpcore/client/pulp_rpm/api/rpm_copy_api.py` & `pulp_rpm-client-3.9.1/pulpcore/client/pulp_rpm/api/rpm_copy_api.py`

 * *Files identical despite different names*

### Comparing `pulp_rpm-client-3.9.0.dev1611548779/pulpcore/client/pulp_rpm/api_client.py` & `pulp_rpm-client-3.9.1/pulpcore/client/pulp_rpm/api_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -75,15 +75,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/3.9.0.dev01611548779/python'
+        self.user_agent = 'OpenAPI-Generator/3.9.1/python'
         self.client_side_validation = configuration.client_side_validation
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
```

### Comparing `pulp_rpm-client-3.9.0.dev1611548779/pulpcore/client/pulp_rpm/configuration.py` & `pulp_rpm-client-3.9.1/pulpcore/client/pulp_rpm/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -372,15 +372,15 @@
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: v3\n"\
-               "SDK Package Version: 3.9.0.dev01611548779".\
+               "SDK Package Version: 3.9.1".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `pulp_rpm-client-3.9.0.dev1611548779/pulpcore/client/pulp_rpm/exceptions.py` & `pulp_rpm-client-3.9.1/pulpcore/client/pulp_rpm/exceptions.py`

 * *Files identical despite different names*

### Comparing `pulp_rpm-client-3.9.0.dev1611548779/pulpcore/client/pulp_rpm/models/__init__.py` & `pulp_rpm-client-3.9.1/pulpcore/client/pulp_rpm/models/__init__.py`

 * *Files identical despite different names*

### Comparing `pulp_rpm-client-3.9.0.dev1611548779/pulpcore/client/pulp_rpm/models/addon_response.py` & `pulp_rpm-client-3.9.1/pulpcore/client/pulp_rpm/models/addon_response.py`

 * *Files identical despite different names*

### Comparing `pulp_rpm-client-3.9.0.dev1611548779/pulpcore/client/pulp_rpm/models/artifact_response.py` & `pulp_rpm-client-3.9.1/pulpcore/client/pulp_rpm/models/artifact_response.py`

 * *Files identical despite different names*

### Comparing `pulp_rpm-client-3.9.0.dev1611548779/pulpcore/client/pulp_rpm/models/async_operation_response.py` & `pulp_rpm-client-3.9.1/pulpcore/client/pulp_rpm/models/async_operation_response.py`

 * *Files identical despite different names*

### Comparing `pulp_rpm-client-3.9.0.dev1611548779/pulpcore/client/pulp_rpm/models/checksum_response.py` & `pulp_rpm-client-3.9.1/pulpcore/client/pulp_rpm/models/checksum_response.py`

 * *Files identical despite different names*

### Comparing `pulp_rpm-client-3.9.0.dev1611548779/pulpcore/client/pulp_rpm/models/content_summary.py` & `pulp_rpm-client-3.9.1/pulpcore/client/pulp_rpm/models/content_summary.py`

 * *Files identical despite different names*

### Comparing `pulp_rpm-client-3.9.0.dev1611548779/pulpcore/client/pulp_rpm/models/content_summary_response.py` & `pulp_rpm-client-3.9.1/pulpcore/client/pulp_rpm/models/content_summary_response.py`

 * *Files identical despite different names*

### Comparing `pulp_rpm-client-3.9.0.dev1611548779/pulpcore/client/pulp_rpm/models/copy.py` & `pulp_rpm-client-3.9.1/pulpcore/client/pulp_rpm/models/copy.py`

 * *Files identical despite different names*

### Comparing `pulp_rpm-client-3.9.0.dev1611548779/pulpcore/client/pulp_rpm/models/image_response.py` & `pulp_rpm-client-3.9.1/pulpcore/client/pulp_rpm/models/image_response.py`

 * *Files identical despite different names*

### Comparing `pulp_rpm-client-3.9.0.dev1611548779/pulpcore/client/pulp_rpm/models/metadata_checksum_type_enum.py` & `pulp_rpm-client-3.9.1/pulpcore/client/pulp_rpm/models/metadata_checksum_type_enum.py`

 * *Files identical despite different names*

### Comparing `pulp_rpm-client-3.9.0.dev1611548779/pulpcore/client/pulp_rpm/models/package_checksum_type_enum.py` & `pulp_rpm-client-3.9.1/pulpcore/client/pulp_rpm/models/package_checksum_type_enum.py`

 * *Files identical despite different names*

### Comparing `pulp_rpm-client-3.9.0.dev1611548779/pulpcore/client/pulp_rpm/models/paginated_repository_version_response_list.py` & `pulp_rpm-client-3.9.1/pulpcore/client/pulp_rpm/models/paginated_repository_version_response_list.py`

 * *Files identical despite different names*

### Comparing `pulp_rpm-client-3.9.0.dev1611548779/pulpcore/client/pulp_rpm/models/paginatedrpm_distribution_tree_response_list.py` & `pulp_rpm-client-3.9.1/pulpcore/client/pulp_rpm/models/paginatedrpm_distribution_tree_response_list.py`

 * *Files identical despite different names*

### Comparing `pulp_rpm-client-3.9.0.dev1611548779/pulpcore/client/pulp_rpm/models/paginatedrpm_modulemd_defaults_response_list.py` & `pulp_rpm-client-3.9.1/pulpcore/client/pulp_rpm/models/paginatedrpm_modulemd_defaults_response_list.py`

 * *Files identical despite different names*

### Comparing `pulp_rpm-client-3.9.0.dev1611548779/pulpcore/client/pulp_rpm/models/paginatedrpm_modulemd_response_list.py` & `pulp_rpm-client-3.9.1/pulpcore/client/pulp_rpm/models/paginatedrpm_modulemd_response_list.py`

 * *Files identical despite different names*

### Comparing `pulp_rpm-client-3.9.0.dev1611548779/pulpcore/client/pulp_rpm/models/paginatedrpm_package_category_response_list.py` & `pulp_rpm-client-3.9.1/pulpcore/client/pulp_rpm/models/paginatedrpm_package_category_response_list.py`

 * *Files identical despite different names*

### Comparing `pulp_rpm-client-3.9.0.dev1611548779/pulpcore/client/pulp_rpm/models/paginatedrpm_package_environment_response_list.py` & `pulp_rpm-client-3.9.1/pulpcore/client/pulp_rpm/models/paginatedrpm_package_environment_response_list.py`

 * *Files identical despite different names*

### Comparing `pulp_rpm-client-3.9.0.dev1611548779/pulpcore/client/pulp_rpm/models/paginatedrpm_package_group_response_list.py` & `pulp_rpm-client-3.9.1/pulpcore/client/pulp_rpm/models/paginatedrpm_package_group_response_list.py`

 * *Files identical despite different names*

### Comparing `pulp_rpm-client-3.9.0.dev1611548779/pulpcore/client/pulp_rpm/models/paginatedrpm_package_langpacks_response_list.py` & `pulp_rpm-client-3.9.1/pulpcore/client/pulp_rpm/models/paginatedrpm_package_langpacks_response_list.py`

 * *Files identical despite different names*

### Comparing `pulp_rpm-client-3.9.0.dev1611548779/pulpcore/client/pulp_rpm/models/paginatedrpm_package_response_list.py` & `pulp_rpm-client-3.9.1/pulpcore/client/pulp_rpm/models/paginatedrpm_package_response_list.py`

 * *Files identical despite different names*

### Comparing `pulp_rpm-client-3.9.0.dev1611548779/pulpcore/client/pulp_rpm/models/paginatedrpm_repo_metadata_file_response_list.py` & `pulp_rpm-client-3.9.1/pulpcore/client/pulp_rpm/models/paginatedrpm_repo_metadata_file_response_list.py`

 * *Files identical despite different names*

### Comparing `pulp_rpm-client-3.9.0.dev1611548779/pulpcore/client/pulp_rpm/models/paginatedrpm_rpm_distribution_response_list.py` & `pulp_rpm-client-3.9.1/pulpcore/client/pulp_rpm/models/paginatedrpm_rpm_distribution_response_list.py`

 * *Files identical despite different names*

### Comparing `pulp_rpm-client-3.9.0.dev1611548779/pulpcore/client/pulp_rpm/models/paginatedrpm_rpm_publication_response_list.py` & `pulp_rpm-client-3.9.1/pulpcore/client/pulp_rpm/models/paginatedrpm_rpm_publication_response_list.py`

 * *Files identical despite different names*

### Comparing `pulp_rpm-client-3.9.0.dev1611548779/pulpcore/client/pulp_rpm/models/paginatedrpm_rpm_remote_response_list.py` & `pulp_rpm-client-3.9.1/pulpcore/client/pulp_rpm/models/paginatedrpm_rpm_remote_response_list.py`

 * *Files identical despite different names*

### Comparing `pulp_rpm-client-3.9.0.dev1611548779/pulpcore/client/pulp_rpm/models/paginatedrpm_rpm_repository_response_list.py` & `pulp_rpm-client-3.9.1/pulpcore/client/pulp_rpm/models/paginatedrpm_rpm_repository_response_list.py`

 * *Files identical despite different names*

### Comparing `pulp_rpm-client-3.9.0.dev1611548779/pulpcore/client/pulp_rpm/models/paginatedrpm_update_record_response_list.py` & `pulp_rpm-client-3.9.1/pulpcore/client/pulp_rpm/models/paginatedrpm_update_record_response_list.py`

 * *Files identical despite different names*

### Comparing `pulp_rpm-client-3.9.0.dev1611548779/pulpcore/client/pulp_rpm/models/patchedrpm_rpm_distribution.py` & `pulp_rpm-client-3.9.1/pulpcore/client/pulp_rpm/models/patchedrpm_rpm_distribution.py`

 * *Files 13% similar despite different names*

```diff
@@ -32,40 +32,45 @@
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
         'base_path': 'str',
         'content_guard': 'str',
+        'pulp_labels': 'object',
         'name': 'str',
         'publication': 'str'
     }
 
     attribute_map = {
         'base_path': 'base_path',
         'content_guard': 'content_guard',
+        'pulp_labels': 'pulp_labels',
         'name': 'name',
         'publication': 'publication'
     }
 
-    def __init__(self, base_path=None, content_guard=None, name=None, publication=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, base_path=None, content_guard=None, pulp_labels=None, name=None, publication=None, local_vars_configuration=None):  # noqa: E501
         """PatchedrpmRpmDistribution - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._base_path = None
         self._content_guard = None
+        self._pulp_labels = None
         self._name = None
         self._publication = None
         self.discriminator = None
 
         if base_path is not None:
             self.base_path = base_path
         self.content_guard = content_guard
+        if pulp_labels is not None:
+            self.pulp_labels = pulp_labels
         if name is not None:
             self.name = name
         self.publication = publication
 
     @property
     def base_path(self):
         """Gets the base_path of this PatchedrpmRpmDistribution.  # noqa: E501
@@ -109,14 +114,35 @@
         :param content_guard: The content_guard of this PatchedrpmRpmDistribution.  # noqa: E501
         :type: str
         """
 
         self._content_guard = content_guard
 
     @property
+    def pulp_labels(self):
+        """Gets the pulp_labels of this PatchedrpmRpmDistribution.  # noqa: E501
+
+
+        :return: The pulp_labels of this PatchedrpmRpmDistribution.  # noqa: E501
+        :rtype: object
+        """
+        return self._pulp_labels
+
+    @pulp_labels.setter
+    def pulp_labels(self, pulp_labels):
+        """Sets the pulp_labels of this PatchedrpmRpmDistribution.
+
+
+        :param pulp_labels: The pulp_labels of this PatchedrpmRpmDistribution.  # noqa: E501
+        :type: object
+        """
+
+        self._pulp_labels = pulp_labels
+
+    @property
     def name(self):
         """Gets the name of this PatchedrpmRpmDistribution.  # noqa: E501
 
         A unique name. Ex, `rawhide` and `stable`.  # noqa: E501
 
         :return: The name of this PatchedrpmRpmDistribution.  # noqa: E501
         :rtype: str
```

### Comparing `pulp_rpm-client-3.9.0.dev1611548779/pulpcore/client/pulp_rpm/models/patchedrpm_rpm_remote.py` & `pulp_rpm-client-3.9.1/pulpcore/client/pulp_rpm/models/patchedrpm_rpm_remote.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,63 +39,69 @@
         'ca_cert': 'str',
         'client_cert': 'str',
         'client_key': 'str',
         'tls_validation': 'bool',
         'proxy_url': 'str',
         'username': 'str',
         'password': 'str',
+        'pulp_labels': 'object',
         'download_concurrency': 'int',
         'policy': 'PolicyEnum',
         'total_timeout': 'float',
         'connect_timeout': 'float',
         'sock_connect_timeout': 'float',
         'sock_read_timeout': 'float',
+        'rate_limit': 'int',
         'sles_auth_token': 'str'
     }
 
     attribute_map = {
         'name': 'name',
         'url': 'url',
         'ca_cert': 'ca_cert',
         'client_cert': 'client_cert',
         'client_key': 'client_key',
         'tls_validation': 'tls_validation',
         'proxy_url': 'proxy_url',
         'username': 'username',
         'password': 'password',
+        'pulp_labels': 'pulp_labels',
         'download_concurrency': 'download_concurrency',
         'policy': 'policy',
         'total_timeout': 'total_timeout',
         'connect_timeout': 'connect_timeout',
         'sock_connect_timeout': 'sock_connect_timeout',
         'sock_read_timeout': 'sock_read_timeout',
+        'rate_limit': 'rate_limit',
         'sles_auth_token': 'sles_auth_token'
     }
 
-    def __init__(self, name=None, url=None, ca_cert=None, client_cert=None, client_key=None, tls_validation=None, proxy_url=None, username=None, password=None, download_concurrency=None, policy=None, total_timeout=None, connect_timeout=None, sock_connect_timeout=None, sock_read_timeout=None, sles_auth_token=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, name=None, url=None, ca_cert=None, client_cert=None, client_key=None, tls_validation=None, proxy_url=None, username=None, password=None, pulp_labels=None, download_concurrency=None, policy=None, total_timeout=None, connect_timeout=None, sock_connect_timeout=None, sock_read_timeout=None, rate_limit=None, sles_auth_token=None, local_vars_configuration=None):  # noqa: E501
         """PatchedrpmRpmRemote - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._name = None
         self._url = None
         self._ca_cert = None
         self._client_cert = None
         self._client_key = None
         self._tls_validation = None
         self._proxy_url = None
         self._username = None
         self._password = None
+        self._pulp_labels = None
         self._download_concurrency = None
         self._policy = None
         self._total_timeout = None
         self._connect_timeout = None
         self._sock_connect_timeout = None
         self._sock_read_timeout = None
+        self._rate_limit = None
         self._sles_auth_token = None
         self.discriminator = None
 
         if name is not None:
             self.name = name
         if url is not None:
             self.url = url
@@ -103,22 +109,25 @@
         self.client_cert = client_cert
         self.client_key = client_key
         if tls_validation is not None:
             self.tls_validation = tls_validation
         self.proxy_url = proxy_url
         self.username = username
         self.password = password
+        if pulp_labels is not None:
+            self.pulp_labels = pulp_labels
         if download_concurrency is not None:
             self.download_concurrency = download_concurrency
         if policy is not None:
             self.policy = policy
         self.total_timeout = total_timeout
         self.connect_timeout = connect_timeout
         self.sock_connect_timeout = sock_connect_timeout
         self.sock_read_timeout = sock_read_timeout
+        self.rate_limit = rate_limit
         self.sles_auth_token = sles_auth_token
 
     @property
     def name(self):
         """Gets the name of this PatchedrpmRpmRemote.  # noqa: E501
 
         A unique name for this remote.  # noqa: E501
@@ -321,14 +330,35 @@
         :param password: The password of this PatchedrpmRpmRemote.  # noqa: E501
         :type: str
         """
 
         self._password = password
 
     @property
+    def pulp_labels(self):
+        """Gets the pulp_labels of this PatchedrpmRpmRemote.  # noqa: E501
+
+
+        :return: The pulp_labels of this PatchedrpmRpmRemote.  # noqa: E501
+        :rtype: object
+        """
+        return self._pulp_labels
+
+    @pulp_labels.setter
+    def pulp_labels(self, pulp_labels):
+        """Sets the pulp_labels of this PatchedrpmRpmRemote.
+
+
+        :param pulp_labels: The pulp_labels of this PatchedrpmRpmRemote.  # noqa: E501
+        :type: object
+        """
+
+        self._pulp_labels = pulp_labels
+
+    @property
     def download_concurrency(self):
         """Gets the download_concurrency of this PatchedrpmRpmRemote.  # noqa: E501
 
         Total number of simultaneous connections.  # noqa: E501
 
         :return: The download_concurrency of this PatchedrpmRpmRemote.  # noqa: E501
         :rtype: int
@@ -474,14 +504,37 @@
         if (self.local_vars_configuration.client_side_validation and
                 sock_read_timeout is not None and sock_read_timeout < 0.0):  # noqa: E501
             raise ValueError("Invalid value for `sock_read_timeout`, must be a value greater than or equal to `0.0`")  # noqa: E501
 
         self._sock_read_timeout = sock_read_timeout
 
     @property
+    def rate_limit(self):
+        """Gets the rate_limit of this PatchedrpmRpmRemote.  # noqa: E501
+
+        Limits total download rate in requests per second  # noqa: E501
+
+        :return: The rate_limit of this PatchedrpmRpmRemote.  # noqa: E501
+        :rtype: int
+        """
+        return self._rate_limit
+
+    @rate_limit.setter
+    def rate_limit(self, rate_limit):
+        """Sets the rate_limit of this PatchedrpmRpmRemote.
+
+        Limits total download rate in requests per second  # noqa: E501
+
+        :param rate_limit: The rate_limit of this PatchedrpmRpmRemote.  # noqa: E501
+        :type: int
+        """
+
+        self._rate_limit = rate_limit
+
+    @property
     def sles_auth_token(self):
         """Gets the sles_auth_token of this PatchedrpmRpmRemote.  # noqa: E501
 
         Authentication token for SLES repositories.  # noqa: E501
 
         :return: The sles_auth_token of this PatchedrpmRpmRemote.  # noqa: E501
         :rtype: str
```

### Comparing `pulp_rpm-client-3.9.0.dev1611548779/pulpcore/client/pulp_rpm/models/patchedrpm_rpm_repository.py` & `pulp_rpm-client-3.9.1/pulpcore/client/pulp_rpm/models/patchedrpm_rpm_repository.py`

 * *Files 9% similar despite different names*

```diff
@@ -30,51 +30,77 @@
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
+        'pulp_labels': 'object',
         'name': 'str',
         'description': 'str',
         'remote': 'str',
         'metadata_signing_service': 'str',
         'retain_package_versions': 'int'
     }
 
     attribute_map = {
+        'pulp_labels': 'pulp_labels',
         'name': 'name',
         'description': 'description',
         'remote': 'remote',
         'metadata_signing_service': 'metadata_signing_service',
         'retain_package_versions': 'retain_package_versions'
     }
 
-    def __init__(self, name=None, description=None, remote=None, metadata_signing_service=None, retain_package_versions=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, pulp_labels=None, name=None, description=None, remote=None, metadata_signing_service=None, retain_package_versions=None, local_vars_configuration=None):  # noqa: E501
         """PatchedrpmRpmRepository - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
+        self._pulp_labels = None
         self._name = None
         self._description = None
         self._remote = None
         self._metadata_signing_service = None
         self._retain_package_versions = None
         self.discriminator = None
 
+        if pulp_labels is not None:
+            self.pulp_labels = pulp_labels
         if name is not None:
             self.name = name
         self.description = description
         self.remote = remote
         self.metadata_signing_service = metadata_signing_service
         if retain_package_versions is not None:
             self.retain_package_versions = retain_package_versions
 
     @property
+    def pulp_labels(self):
+        """Gets the pulp_labels of this PatchedrpmRpmRepository.  # noqa: E501
+
+
+        :return: The pulp_labels of this PatchedrpmRpmRepository.  # noqa: E501
+        :rtype: object
+        """
+        return self._pulp_labels
+
+    @pulp_labels.setter
+    def pulp_labels(self, pulp_labels):
+        """Sets the pulp_labels of this PatchedrpmRpmRepository.
+
+
+        :param pulp_labels: The pulp_labels of this PatchedrpmRpmRepository.  # noqa: E501
+        :type: object
+        """
+
+        self._pulp_labels = pulp_labels
+
+    @property
     def name(self):
         """Gets the name of this PatchedrpmRpmRepository.  # noqa: E501
 
         A unique name for this repository.  # noqa: E501
 
         :return: The name of this PatchedrpmRpmRepository.  # noqa: E501
         :rtype: str
```

### Comparing `pulp_rpm-client-3.9.0.dev1611548779/pulpcore/client/pulp_rpm/models/policy_enum.py` & `pulp_rpm-client-3.9.1/pulpcore/client/pulp_rpm/models/policy_enum.py`

 * *Files identical despite different names*

### Comparing `pulp_rpm-client-3.9.0.dev1611548779/pulpcore/client/pulp_rpm/models/repository_add_remove_content.py` & `pulp_rpm-client-3.9.1/pulpcore/client/pulp_rpm/models/repository_add_remove_content.py`

 * *Files identical despite different names*

### Comparing `pulp_rpm-client-3.9.0.dev1611548779/pulpcore/client/pulp_rpm/models/repository_version.py` & `pulp_rpm-client-3.9.1/pulpcore/client/pulp_rpm/models/repository_version.py`

 * *Files identical despite different names*

### Comparing `pulp_rpm-client-3.9.0.dev1611548779/pulpcore/client/pulp_rpm/models/repository_version_response.py` & `pulp_rpm-client-3.9.1/pulpcore/client/pulp_rpm/models/repository_version_response.py`

 * *Files identical despite different names*

### Comparing `pulp_rpm-client-3.9.0.dev1611548779/pulpcore/client/pulp_rpm/models/rpm_distribution_tree_response.py` & `pulp_rpm-client-3.9.1/pulpcore/client/pulp_rpm/models/rpm_distribution_tree_response.py`

 * *Files identical despite different names*

### Comparing `pulp_rpm-client-3.9.0.dev1611548779/pulpcore/client/pulp_rpm/models/rpm_modulemd.py` & `pulp_rpm-client-3.9.1/pulpcore/client/pulp_rpm/models/rpm_modulemd.py`

 * *Files identical despite different names*

### Comparing `pulp_rpm-client-3.9.0.dev1611548779/pulpcore/client/pulp_rpm/models/rpm_modulemd_defaults.py` & `pulp_rpm-client-3.9.1/pulpcore/client/pulp_rpm/models/rpm_modulemd_defaults.py`

 * *Files identical despite different names*

### Comparing `pulp_rpm-client-3.9.0.dev1611548779/pulpcore/client/pulp_rpm/models/rpm_modulemd_defaults_response.py` & `pulp_rpm-client-3.9.1/pulpcore/client/pulp_rpm/models/rpm_modulemd_defaults_response.py`

 * *Files identical despite different names*

### Comparing `pulp_rpm-client-3.9.0.dev1611548779/pulpcore/client/pulp_rpm/models/rpm_modulemd_response.py` & `pulp_rpm-client-3.9.1/pulpcore/client/pulp_rpm/models/rpm_modulemd_response.py`

 * *Files identical despite different names*

### Comparing `pulp_rpm-client-3.9.0.dev1611548779/pulpcore/client/pulp_rpm/models/rpm_package.py` & `pulp_rpm-client-3.9.1/pulpcore/client/pulp_rpm/models/rpm_package.py`

 * *Files identical despite different names*

### Comparing `pulp_rpm-client-3.9.0.dev1611548779/pulpcore/client/pulp_rpm/models/rpm_package_category_response.py` & `pulp_rpm-client-3.9.1/pulpcore/client/pulp_rpm/models/rpm_package_category_response.py`

 * *Files identical despite different names*

### Comparing `pulp_rpm-client-3.9.0.dev1611548779/pulpcore/client/pulp_rpm/models/rpm_package_environment_response.py` & `pulp_rpm-client-3.9.1/pulpcore/client/pulp_rpm/models/rpm_package_environment_response.py`

 * *Files identical despite different names*

### Comparing `pulp_rpm-client-3.9.0.dev1611548779/pulpcore/client/pulp_rpm/models/rpm_package_group_response.py` & `pulp_rpm-client-3.9.1/pulpcore/client/pulp_rpm/models/rpm_package_group_response.py`

 * *Files identical despite different names*

### Comparing `pulp_rpm-client-3.9.0.dev1611548779/pulpcore/client/pulp_rpm/models/rpm_package_langpacks_response.py` & `pulp_rpm-client-3.9.1/pulpcore/client/pulp_rpm/models/rpm_package_langpacks_response.py`

 * *Files identical despite different names*

### Comparing `pulp_rpm-client-3.9.0.dev1611548779/pulpcore/client/pulp_rpm/models/rpm_package_response.py` & `pulp_rpm-client-3.9.1/pulpcore/client/pulp_rpm/models/rpm_package_response.py`

 * *Files identical despite different names*

### Comparing `pulp_rpm-client-3.9.0.dev1611548779/pulpcore/client/pulp_rpm/models/rpm_repo_metadata_file_response.py` & `pulp_rpm-client-3.9.1/pulpcore/client/pulp_rpm/models/rpm_repo_metadata_file_response.py`

 * *Files identical despite different names*

### Comparing `pulp_rpm-client-3.9.0.dev1611548779/pulpcore/client/pulp_rpm/models/rpm_repository_sync_url.py` & `pulp_rpm-client-3.9.1/pulpcore/client/pulp_rpm/models/rpm_repository_sync_url.py`

 * *Files identical despite different names*

### Comparing `pulp_rpm-client-3.9.0.dev1611548779/pulpcore/client/pulp_rpm/models/rpm_rpm_distribution.py` & `pulp_rpm-client-3.9.1/pulpcore/client/pulp_rpm/models/rpm_rpm_distribution.py`

 * *Files 14% similar despite different names*

```diff
@@ -32,39 +32,44 @@
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
         'base_path': 'str',
         'content_guard': 'str',
+        'pulp_labels': 'object',
         'name': 'str',
         'publication': 'str'
     }
 
     attribute_map = {
         'base_path': 'base_path',
         'content_guard': 'content_guard',
+        'pulp_labels': 'pulp_labels',
         'name': 'name',
         'publication': 'publication'
     }
 
-    def __init__(self, base_path=None, content_guard=None, name=None, publication=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, base_path=None, content_guard=None, pulp_labels=None, name=None, publication=None, local_vars_configuration=None):  # noqa: E501
         """RpmRpmDistribution - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._base_path = None
         self._content_guard = None
+        self._pulp_labels = None
         self._name = None
         self._publication = None
         self.discriminator = None
 
         self.base_path = base_path
         self.content_guard = content_guard
+        if pulp_labels is not None:
+            self.pulp_labels = pulp_labels
         self.name = name
         self.publication = publication
 
     @property
     def base_path(self):
         """Gets the base_path of this RpmRpmDistribution.  # noqa: E501
 
@@ -109,14 +114,35 @@
         :param content_guard: The content_guard of this RpmRpmDistribution.  # noqa: E501
         :type: str
         """
 
         self._content_guard = content_guard
 
     @property
+    def pulp_labels(self):
+        """Gets the pulp_labels of this RpmRpmDistribution.  # noqa: E501
+
+
+        :return: The pulp_labels of this RpmRpmDistribution.  # noqa: E501
+        :rtype: object
+        """
+        return self._pulp_labels
+
+    @pulp_labels.setter
+    def pulp_labels(self, pulp_labels):
+        """Sets the pulp_labels of this RpmRpmDistribution.
+
+
+        :param pulp_labels: The pulp_labels of this RpmRpmDistribution.  # noqa: E501
+        :type: object
+        """
+
+        self._pulp_labels = pulp_labels
+
+    @property
     def name(self):
         """Gets the name of this RpmRpmDistribution.  # noqa: E501
 
         A unique name. Ex, `rawhide` and `stable`.  # noqa: E501
 
         :return: The name of this RpmRpmDistribution.  # noqa: E501
         :rtype: str
```

### Comparing `pulp_rpm-client-3.9.0.dev1611548779/pulpcore/client/pulp_rpm/models/rpm_rpm_distribution_response.py` & `pulp_rpm-client-3.9.1/pulpcore/client/pulp_rpm/models/rpm_rpm_distribution_response.py`

 * *Files 16% similar despite different names*

```diff
@@ -35,51 +35,56 @@
     """
     openapi_types = {
         'pulp_href': 'str',
         'pulp_created': 'datetime',
         'base_path': 'str',
         'base_url': 'str',
         'content_guard': 'str',
+        'pulp_labels': 'object',
         'name': 'str',
         'publication': 'str'
     }
 
     attribute_map = {
         'pulp_href': 'pulp_href',
         'pulp_created': 'pulp_created',
         'base_path': 'base_path',
         'base_url': 'base_url',
         'content_guard': 'content_guard',
+        'pulp_labels': 'pulp_labels',
         'name': 'name',
         'publication': 'publication'
     }
 
-    def __init__(self, pulp_href=None, pulp_created=None, base_path=None, base_url=None, content_guard=None, name=None, publication=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, pulp_href=None, pulp_created=None, base_path=None, base_url=None, content_guard=None, pulp_labels=None, name=None, publication=None, local_vars_configuration=None):  # noqa: E501
         """RpmRpmDistributionResponse - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._pulp_href = None
         self._pulp_created = None
         self._base_path = None
         self._base_url = None
         self._content_guard = None
+        self._pulp_labels = None
         self._name = None
         self._publication = None
         self.discriminator = None
 
         if pulp_href is not None:
             self.pulp_href = pulp_href
         if pulp_created is not None:
             self.pulp_created = pulp_created
         self.base_path = base_path
         if base_url is not None:
             self.base_url = base_url
         self.content_guard = content_guard
+        if pulp_labels is not None:
+            self.pulp_labels = pulp_labels
         self.name = name
         self.publication = publication
 
     @property
     def pulp_href(self):
         """Gets the pulp_href of this RpmRpmDistributionResponse.  # noqa: E501
 
@@ -191,14 +196,35 @@
         :param content_guard: The content_guard of this RpmRpmDistributionResponse.  # noqa: E501
         :type: str
         """
 
         self._content_guard = content_guard
 
     @property
+    def pulp_labels(self):
+        """Gets the pulp_labels of this RpmRpmDistributionResponse.  # noqa: E501
+
+
+        :return: The pulp_labels of this RpmRpmDistributionResponse.  # noqa: E501
+        :rtype: object
+        """
+        return self._pulp_labels
+
+    @pulp_labels.setter
+    def pulp_labels(self, pulp_labels):
+        """Sets the pulp_labels of this RpmRpmDistributionResponse.
+
+
+        :param pulp_labels: The pulp_labels of this RpmRpmDistributionResponse.  # noqa: E501
+        :type: object
+        """
+
+        self._pulp_labels = pulp_labels
+
+    @property
     def name(self):
         """Gets the name of this RpmRpmDistributionResponse.  # noqa: E501
 
         A unique name. Ex, `rawhide` and `stable`.  # noqa: E501
 
         :return: The name of this RpmRpmDistributionResponse.  # noqa: E501
         :rtype: str
```

### Comparing `pulp_rpm-client-3.9.0.dev1611548779/pulpcore/client/pulp_rpm/models/rpm_rpm_publication.py` & `pulp_rpm-client-3.9.1/pulpcore/client/pulp_rpm/models/rpm_rpm_publication.py`

 * *Files identical despite different names*

### Comparing `pulp_rpm-client-3.9.0.dev1611548779/pulpcore/client/pulp_rpm/models/rpm_rpm_publication_response.py` & `pulp_rpm-client-3.9.1/pulpcore/client/pulp_rpm/models/rpm_rpm_publication_response.py`

 * *Files identical despite different names*

### Comparing `pulp_rpm-client-3.9.0.dev1611548779/pulpcore/client/pulp_rpm/models/rpm_rpm_remote.py` & `pulp_rpm-client-3.9.1/pulpcore/client/pulp_rpm/models/rpm_rpm_remote.py`

 * *Files 3% similar despite different names*

```diff
@@ -39,84 +39,93 @@
         'ca_cert': 'str',
         'client_cert': 'str',
         'client_key': 'str',
         'tls_validation': 'bool',
         'proxy_url': 'str',
         'username': 'str',
         'password': 'str',
+        'pulp_labels': 'object',
         'download_concurrency': 'int',
         'policy': 'PolicyEnum',
         'total_timeout': 'float',
         'connect_timeout': 'float',
         'sock_connect_timeout': 'float',
         'sock_read_timeout': 'float',
+        'rate_limit': 'int',
         'sles_auth_token': 'str'
     }
 
     attribute_map = {
         'name': 'name',
         'url': 'url',
         'ca_cert': 'ca_cert',
         'client_cert': 'client_cert',
         'client_key': 'client_key',
         'tls_validation': 'tls_validation',
         'proxy_url': 'proxy_url',
         'username': 'username',
         'password': 'password',
+        'pulp_labels': 'pulp_labels',
         'download_concurrency': 'download_concurrency',
         'policy': 'policy',
         'total_timeout': 'total_timeout',
         'connect_timeout': 'connect_timeout',
         'sock_connect_timeout': 'sock_connect_timeout',
         'sock_read_timeout': 'sock_read_timeout',
+        'rate_limit': 'rate_limit',
         'sles_auth_token': 'sles_auth_token'
     }
 
-    def __init__(self, name=None, url=None, ca_cert=None, client_cert=None, client_key=None, tls_validation=None, proxy_url=None, username=None, password=None, download_concurrency=None, policy=None, total_timeout=None, connect_timeout=None, sock_connect_timeout=None, sock_read_timeout=None, sles_auth_token=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, name=None, url=None, ca_cert=None, client_cert=None, client_key=None, tls_validation=None, proxy_url=None, username=None, password=None, pulp_labels=None, download_concurrency=None, policy=None, total_timeout=None, connect_timeout=None, sock_connect_timeout=None, sock_read_timeout=None, rate_limit=None, sles_auth_token=None, local_vars_configuration=None):  # noqa: E501
         """RpmRpmRemote - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._name = None
         self._url = None
         self._ca_cert = None
         self._client_cert = None
         self._client_key = None
         self._tls_validation = None
         self._proxy_url = None
         self._username = None
         self._password = None
+        self._pulp_labels = None
         self._download_concurrency = None
         self._policy = None
         self._total_timeout = None
         self._connect_timeout = None
         self._sock_connect_timeout = None
         self._sock_read_timeout = None
+        self._rate_limit = None
         self._sles_auth_token = None
         self.discriminator = None
 
         self.name = name
         self.url = url
         self.ca_cert = ca_cert
         self.client_cert = client_cert
         self.client_key = client_key
         if tls_validation is not None:
             self.tls_validation = tls_validation
         self.proxy_url = proxy_url
         self.username = username
         self.password = password
+        if pulp_labels is not None:
+            self.pulp_labels = pulp_labels
         if download_concurrency is not None:
             self.download_concurrency = download_concurrency
         if policy is not None:
             self.policy = policy
         self.total_timeout = total_timeout
         self.connect_timeout = connect_timeout
         self.sock_connect_timeout = sock_connect_timeout
         self.sock_read_timeout = sock_read_timeout
+        self.rate_limit = rate_limit
         self.sles_auth_token = sles_auth_token
 
     @property
     def name(self):
         """Gets the name of this RpmRpmRemote.  # noqa: E501
 
         A unique name for this remote.  # noqa: E501
@@ -323,14 +332,35 @@
         :param password: The password of this RpmRpmRemote.  # noqa: E501
         :type: str
         """
 
         self._password = password
 
     @property
+    def pulp_labels(self):
+        """Gets the pulp_labels of this RpmRpmRemote.  # noqa: E501
+
+
+        :return: The pulp_labels of this RpmRpmRemote.  # noqa: E501
+        :rtype: object
+        """
+        return self._pulp_labels
+
+    @pulp_labels.setter
+    def pulp_labels(self, pulp_labels):
+        """Sets the pulp_labels of this RpmRpmRemote.
+
+
+        :param pulp_labels: The pulp_labels of this RpmRpmRemote.  # noqa: E501
+        :type: object
+        """
+
+        self._pulp_labels = pulp_labels
+
+    @property
     def download_concurrency(self):
         """Gets the download_concurrency of this RpmRpmRemote.  # noqa: E501
 
         Total number of simultaneous connections.  # noqa: E501
 
         :return: The download_concurrency of this RpmRpmRemote.  # noqa: E501
         :rtype: int
@@ -476,14 +506,37 @@
         if (self.local_vars_configuration.client_side_validation and
                 sock_read_timeout is not None and sock_read_timeout < 0.0):  # noqa: E501
             raise ValueError("Invalid value for `sock_read_timeout`, must be a value greater than or equal to `0.0`")  # noqa: E501
 
         self._sock_read_timeout = sock_read_timeout
 
     @property
+    def rate_limit(self):
+        """Gets the rate_limit of this RpmRpmRemote.  # noqa: E501
+
+        Limits total download rate in requests per second  # noqa: E501
+
+        :return: The rate_limit of this RpmRpmRemote.  # noqa: E501
+        :rtype: int
+        """
+        return self._rate_limit
+
+    @rate_limit.setter
+    def rate_limit(self, rate_limit):
+        """Sets the rate_limit of this RpmRpmRemote.
+
+        Limits total download rate in requests per second  # noqa: E501
+
+        :param rate_limit: The rate_limit of this RpmRpmRemote.  # noqa: E501
+        :type: int
+        """
+
+        self._rate_limit = rate_limit
+
+    @property
     def sles_auth_token(self):
         """Gets the sles_auth_token of this RpmRpmRemote.  # noqa: E501
 
         Authentication token for SLES repositories.  # noqa: E501
 
         :return: The sles_auth_token of this RpmRpmRemote.  # noqa: E501
         :rtype: str
```

### Comparing `pulp_rpm-client-3.9.0.dev1611548779/pulpcore/client/pulp_rpm/models/rpm_rpm_remote_response.py` & `pulp_rpm-client-3.9.1/pulpcore/client/pulp_rpm/models/rpm_rpm_remote_response.py`

 * *Files 6% similar despite different names*

```diff
@@ -41,21 +41,23 @@
         'ca_cert': 'str',
         'client_cert': 'str',
         'client_key': 'str',
         'tls_validation': 'bool',
         'proxy_url': 'str',
         'username': 'str',
         'password': 'str',
+        'pulp_labels': 'object',
         'pulp_last_updated': 'datetime',
         'download_concurrency': 'int',
         'policy': 'PolicyEnum',
         'total_timeout': 'float',
         'connect_timeout': 'float',
         'sock_connect_timeout': 'float',
         'sock_read_timeout': 'float',
+        'rate_limit': 'int',
         'sles_auth_token': 'str'
     }
 
     attribute_map = {
         'pulp_href': 'pulp_href',
         'pulp_created': 'pulp_created',
         'name': 'name',
@@ -63,25 +65,27 @@
         'ca_cert': 'ca_cert',
         'client_cert': 'client_cert',
         'client_key': 'client_key',
         'tls_validation': 'tls_validation',
         'proxy_url': 'proxy_url',
         'username': 'username',
         'password': 'password',
+        'pulp_labels': 'pulp_labels',
         'pulp_last_updated': 'pulp_last_updated',
         'download_concurrency': 'download_concurrency',
         'policy': 'policy',
         'total_timeout': 'total_timeout',
         'connect_timeout': 'connect_timeout',
         'sock_connect_timeout': 'sock_connect_timeout',
         'sock_read_timeout': 'sock_read_timeout',
+        'rate_limit': 'rate_limit',
         'sles_auth_token': 'sles_auth_token'
     }
 
-    def __init__(self, pulp_href=None, pulp_created=None, name=None, url=None, ca_cert=None, client_cert=None, client_key=None, tls_validation=None, proxy_url=None, username=None, password=None, pulp_last_updated=None, download_concurrency=None, policy=None, total_timeout=None, connect_timeout=None, sock_connect_timeout=None, sock_read_timeout=None, sles_auth_token=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, pulp_href=None, pulp_created=None, name=None, url=None, ca_cert=None, client_cert=None, client_key=None, tls_validation=None, proxy_url=None, username=None, password=None, pulp_labels=None, pulp_last_updated=None, download_concurrency=None, policy=None, total_timeout=None, connect_timeout=None, sock_connect_timeout=None, sock_read_timeout=None, rate_limit=None, sles_auth_token=None, local_vars_configuration=None):  # noqa: E501
         """RpmRpmRemoteResponse - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._pulp_href = None
         self._pulp_created = None
@@ -90,21 +94,23 @@
         self._ca_cert = None
         self._client_cert = None
         self._client_key = None
         self._tls_validation = None
         self._proxy_url = None
         self._username = None
         self._password = None
+        self._pulp_labels = None
         self._pulp_last_updated = None
         self._download_concurrency = None
         self._policy = None
         self._total_timeout = None
         self._connect_timeout = None
         self._sock_connect_timeout = None
         self._sock_read_timeout = None
+        self._rate_limit = None
         self._sles_auth_token = None
         self.discriminator = None
 
         if pulp_href is not None:
             self.pulp_href = pulp_href
         if pulp_created is not None:
             self.pulp_created = pulp_created
@@ -114,24 +120,27 @@
         self.client_cert = client_cert
         self.client_key = client_key
         if tls_validation is not None:
             self.tls_validation = tls_validation
         self.proxy_url = proxy_url
         self.username = username
         self.password = password
+        if pulp_labels is not None:
+            self.pulp_labels = pulp_labels
         if pulp_last_updated is not None:
             self.pulp_last_updated = pulp_last_updated
         if download_concurrency is not None:
             self.download_concurrency = download_concurrency
         if policy is not None:
             self.policy = policy
         self.total_timeout = total_timeout
         self.connect_timeout = connect_timeout
         self.sock_connect_timeout = sock_connect_timeout
         self.sock_read_timeout = sock_read_timeout
+        self.rate_limit = rate_limit
         self.sles_auth_token = sles_auth_token
 
     @property
     def pulp_href(self):
         """Gets the pulp_href of this RpmRpmRemoteResponse.  # noqa: E501
 
 
@@ -382,14 +391,35 @@
         :param password: The password of this RpmRpmRemoteResponse.  # noqa: E501
         :type: str
         """
 
         self._password = password
 
     @property
+    def pulp_labels(self):
+        """Gets the pulp_labels of this RpmRpmRemoteResponse.  # noqa: E501
+
+
+        :return: The pulp_labels of this RpmRpmRemoteResponse.  # noqa: E501
+        :rtype: object
+        """
+        return self._pulp_labels
+
+    @pulp_labels.setter
+    def pulp_labels(self, pulp_labels):
+        """Sets the pulp_labels of this RpmRpmRemoteResponse.
+
+
+        :param pulp_labels: The pulp_labels of this RpmRpmRemoteResponse.  # noqa: E501
+        :type: object
+        """
+
+        self._pulp_labels = pulp_labels
+
+    @property
     def pulp_last_updated(self):
         """Gets the pulp_last_updated of this RpmRpmRemoteResponse.  # noqa: E501
 
         Timestamp of the most recent update of the remote.  # noqa: E501
 
         :return: The pulp_last_updated of this RpmRpmRemoteResponse.  # noqa: E501
         :rtype: datetime
@@ -558,14 +588,37 @@
         if (self.local_vars_configuration.client_side_validation and
                 sock_read_timeout is not None and sock_read_timeout < 0.0):  # noqa: E501
             raise ValueError("Invalid value for `sock_read_timeout`, must be a value greater than or equal to `0.0`")  # noqa: E501
 
         self._sock_read_timeout = sock_read_timeout
 
     @property
+    def rate_limit(self):
+        """Gets the rate_limit of this RpmRpmRemoteResponse.  # noqa: E501
+
+        Limits total download rate in requests per second  # noqa: E501
+
+        :return: The rate_limit of this RpmRpmRemoteResponse.  # noqa: E501
+        :rtype: int
+        """
+        return self._rate_limit
+
+    @rate_limit.setter
+    def rate_limit(self, rate_limit):
+        """Sets the rate_limit of this RpmRpmRemoteResponse.
+
+        Limits total download rate in requests per second  # noqa: E501
+
+        :param rate_limit: The rate_limit of this RpmRpmRemoteResponse.  # noqa: E501
+        :type: int
+        """
+
+        self._rate_limit = rate_limit
+
+    @property
     def sles_auth_token(self):
         """Gets the sles_auth_token of this RpmRpmRemoteResponse.  # noqa: E501
 
         Authentication token for SLES repositories.  # noqa: E501
 
         :return: The sles_auth_token of this RpmRpmRemoteResponse.  # noqa: E501
         :rtype: str
```

### Comparing `pulp_rpm-client-3.9.0.dev1611548779/pulpcore/client/pulp_rpm/models/rpm_rpm_repository.py` & `pulp_rpm-client-3.9.1/pulpcore/client/pulp_rpm/models/rpm_rpm_repository.py`

 * *Files 7% similar despite different names*

```diff
@@ -30,50 +30,76 @@
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
+        'pulp_labels': 'object',
         'name': 'str',
         'description': 'str',
         'remote': 'str',
         'metadata_signing_service': 'str',
         'retain_package_versions': 'int'
     }
 
     attribute_map = {
+        'pulp_labels': 'pulp_labels',
         'name': 'name',
         'description': 'description',
         'remote': 'remote',
         'metadata_signing_service': 'metadata_signing_service',
         'retain_package_versions': 'retain_package_versions'
     }
 
-    def __init__(self, name=None, description=None, remote=None, metadata_signing_service=None, retain_package_versions=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, pulp_labels=None, name=None, description=None, remote=None, metadata_signing_service=None, retain_package_versions=None, local_vars_configuration=None):  # noqa: E501
         """RpmRpmRepository - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
+        self._pulp_labels = None
         self._name = None
         self._description = None
         self._remote = None
         self._metadata_signing_service = None
         self._retain_package_versions = None
         self.discriminator = None
 
+        if pulp_labels is not None:
+            self.pulp_labels = pulp_labels
         self.name = name
         self.description = description
         self.remote = remote
         self.metadata_signing_service = metadata_signing_service
         if retain_package_versions is not None:
             self.retain_package_versions = retain_package_versions
 
     @property
+    def pulp_labels(self):
+        """Gets the pulp_labels of this RpmRpmRepository.  # noqa: E501
+
+
+        :return: The pulp_labels of this RpmRpmRepository.  # noqa: E501
+        :rtype: object
+        """
+        return self._pulp_labels
+
+    @pulp_labels.setter
+    def pulp_labels(self, pulp_labels):
+        """Sets the pulp_labels of this RpmRpmRepository.
+
+
+        :param pulp_labels: The pulp_labels of this RpmRpmRepository.  # noqa: E501
+        :type: object
+        """
+
+        self._pulp_labels = pulp_labels
+
+    @property
     def name(self):
         """Gets the name of this RpmRpmRepository.  # noqa: E501
 
         A unique name for this repository.  # noqa: E501
 
         :return: The name of this RpmRpmRepository.  # noqa: E501
         :rtype: str
```

### Comparing `pulp_rpm-client-3.9.0.dev1611548779/pulpcore/client/pulp_rpm/models/rpm_rpm_repository_response.py` & `pulp_rpm-client-3.9.1/pulpcore/client/pulp_rpm/models/rpm_rpm_repository_response.py`

 * *Files 6% similar despite different names*

```diff
@@ -33,57 +33,62 @@
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
         'pulp_href': 'str',
         'pulp_created': 'datetime',
         'versions_href': 'str',
+        'pulp_labels': 'object',
         'latest_version_href': 'str',
         'name': 'str',
         'description': 'str',
         'remote': 'str',
         'metadata_signing_service': 'str',
         'retain_package_versions': 'int'
     }
 
     attribute_map = {
         'pulp_href': 'pulp_href',
         'pulp_created': 'pulp_created',
         'versions_href': 'versions_href',
+        'pulp_labels': 'pulp_labels',
         'latest_version_href': 'latest_version_href',
         'name': 'name',
         'description': 'description',
         'remote': 'remote',
         'metadata_signing_service': 'metadata_signing_service',
         'retain_package_versions': 'retain_package_versions'
     }
 
-    def __init__(self, pulp_href=None, pulp_created=None, versions_href=None, latest_version_href=None, name=None, description=None, remote=None, metadata_signing_service=None, retain_package_versions=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, pulp_href=None, pulp_created=None, versions_href=None, pulp_labels=None, latest_version_href=None, name=None, description=None, remote=None, metadata_signing_service=None, retain_package_versions=None, local_vars_configuration=None):  # noqa: E501
         """RpmRpmRepositoryResponse - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._pulp_href = None
         self._pulp_created = None
         self._versions_href = None
+        self._pulp_labels = None
         self._latest_version_href = None
         self._name = None
         self._description = None
         self._remote = None
         self._metadata_signing_service = None
         self._retain_package_versions = None
         self.discriminator = None
 
         if pulp_href is not None:
             self.pulp_href = pulp_href
         if pulp_created is not None:
             self.pulp_created = pulp_created
         if versions_href is not None:
             self.versions_href = versions_href
+        if pulp_labels is not None:
+            self.pulp_labels = pulp_labels
         if latest_version_href is not None:
             self.latest_version_href = latest_version_href
         self.name = name
         self.description = description
         self.remote = remote
         self.metadata_signing_service = metadata_signing_service
         if retain_package_versions is not None:
@@ -151,14 +156,35 @@
         :param versions_href: The versions_href of this RpmRpmRepositoryResponse.  # noqa: E501
         :type: str
         """
 
         self._versions_href = versions_href
 
     @property
+    def pulp_labels(self):
+        """Gets the pulp_labels of this RpmRpmRepositoryResponse.  # noqa: E501
+
+
+        :return: The pulp_labels of this RpmRpmRepositoryResponse.  # noqa: E501
+        :rtype: object
+        """
+        return self._pulp_labels
+
+    @pulp_labels.setter
+    def pulp_labels(self, pulp_labels):
+        """Sets the pulp_labels of this RpmRpmRepositoryResponse.
+
+
+        :param pulp_labels: The pulp_labels of this RpmRpmRepositoryResponse.  # noqa: E501
+        :type: object
+        """
+
+        self._pulp_labels = pulp_labels
+
+    @property
     def latest_version_href(self):
         """Gets the latest_version_href of this RpmRpmRepositoryResponse.  # noqa: E501
 
 
         :return: The latest_version_href of this RpmRpmRepositoryResponse.  # noqa: E501
         :rtype: str
         """
```

### Comparing `pulp_rpm-client-3.9.0.dev1611548779/pulpcore/client/pulp_rpm/models/rpm_update_collection.py` & `pulp_rpm-client-3.9.1/pulpcore/client/pulp_rpm/models/rpm_update_collection.py`

 * *Files identical despite different names*

### Comparing `pulp_rpm-client-3.9.0.dev1611548779/pulpcore/client/pulp_rpm/models/rpm_update_collection_response.py` & `pulp_rpm-client-3.9.1/pulpcore/client/pulp_rpm/models/rpm_update_collection_response.py`

 * *Files identical despite different names*

### Comparing `pulp_rpm-client-3.9.0.dev1611548779/pulpcore/client/pulp_rpm/models/rpm_update_record.py` & `pulp_rpm-client-3.9.1/pulpcore/client/pulp_rpm/models/rpm_update_record.py`

 * *Files identical despite different names*

### Comparing `pulp_rpm-client-3.9.0.dev1611548779/pulpcore/client/pulp_rpm/models/rpm_update_record_response.py` & `pulp_rpm-client-3.9.1/pulpcore/client/pulp_rpm/models/rpm_update_record_response.py`

 * *Files identical despite different names*

### Comparing `pulp_rpm-client-3.9.0.dev1611548779/pulpcore/client/pulp_rpm/models/variant_response.py` & `pulp_rpm-client-3.9.1/pulpcore/client/pulp_rpm/models/variant_response.py`

 * *Files identical despite different names*

### Comparing `pulp_rpm-client-3.9.0.dev1611548779/pulpcore/client/pulp_rpm/rest.py` & `pulp_rpm-client-3.9.1/pulpcore/client/pulp_rpm/rest.py`

 * *Files identical despite different names*

### Comparing `pulp_rpm-client-3.9.0.dev1611548779/setup.py` & `pulp_rpm-client-3.9.1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 from setuptools import setup, find_packages  # noqa: H301
 
 NAME = "pulp_rpm-client"
-VERSION = "3.9.0.dev01611548779"
+VERSION = "3.9.1"
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
```

### Comparing `pulp_rpm-client-3.9.0.dev1611548779/test/test_addon_response.py` & `pulp_rpm-client-3.9.1/test/test_addon_response.py`

 * *Files identical despite different names*

### Comparing `pulp_rpm-client-3.9.0.dev1611548779/test/test_artifact_response.py` & `pulp_rpm-client-3.9.1/test/test_artifact_response.py`

 * *Files identical despite different names*

### Comparing `pulp_rpm-client-3.9.0.dev1611548779/test/test_async_operation_response.py` & `pulp_rpm-client-3.9.1/test/test_async_operation_response.py`

 * *Files identical despite different names*

### Comparing `pulp_rpm-client-3.9.0.dev1611548779/test/test_checksum_response.py` & `pulp_rpm-client-3.9.1/test/test_checksum_response.py`

 * *Files identical despite different names*

### Comparing `pulp_rpm-client-3.9.0.dev1611548779/test/test_content_advisories_api.py` & `pulp_rpm-client-3.9.1/test/test_content_advisories_api.py`

 * *Files identical despite different names*

### Comparing `pulp_rpm-client-3.9.0.dev1611548779/test/test_content_distribution_trees_api.py` & `pulp_rpm-client-3.9.1/test/test_content_distribution_trees_api.py`

 * *Files identical despite different names*

### Comparing `pulp_rpm-client-3.9.0.dev1611548779/test/test_content_modulemd_defaults_api.py` & `pulp_rpm-client-3.9.1/test/test_content_modulemd_defaults_api.py`

 * *Files identical despite different names*

### Comparing `pulp_rpm-client-3.9.0.dev1611548779/test/test_content_modulemds_api.py` & `pulp_rpm-client-3.9.1/test/test_content_modulemds_api.py`

 * *Files identical despite different names*

### Comparing `pulp_rpm-client-3.9.0.dev1611548779/test/test_content_packagecategories_api.py` & `pulp_rpm-client-3.9.1/test/test_content_packagecategories_api.py`

 * *Files identical despite different names*

### Comparing `pulp_rpm-client-3.9.0.dev1611548779/test/test_content_packageenvironments_api.py` & `pulp_rpm-client-3.9.1/test/test_content_packageenvironments_api.py`

 * *Files identical despite different names*

### Comparing `pulp_rpm-client-3.9.0.dev1611548779/test/test_content_packagegroups_api.py` & `pulp_rpm-client-3.9.1/test/test_content_packagegroups_api.py`

 * *Files identical despite different names*

### Comparing `pulp_rpm-client-3.9.0.dev1611548779/test/test_content_packagelangpacks_api.py` & `pulp_rpm-client-3.9.1/test/test_content_packagelangpacks_api.py`

 * *Files identical despite different names*

### Comparing `pulp_rpm-client-3.9.0.dev1611548779/test/test_content_packages_api.py` & `pulp_rpm-client-3.9.1/test/test_content_packages_api.py`

 * *Files identical despite different names*

### Comparing `pulp_rpm-client-3.9.0.dev1611548779/test/test_content_repo_metadata_files_api.py` & `pulp_rpm-client-3.9.1/test/test_content_repo_metadata_files_api.py`

 * *Files identical despite different names*

### Comparing `pulp_rpm-client-3.9.0.dev1611548779/test/test_content_summary.py` & `pulp_rpm-client-3.9.1/test/test_content_summary.py`

 * *Files identical despite different names*

### Comparing `pulp_rpm-client-3.9.0.dev1611548779/test/test_content_summary_response.py` & `pulp_rpm-client-3.9.1/test/test_content_summary_response.py`

 * *Files identical despite different names*

### Comparing `pulp_rpm-client-3.9.0.dev1611548779/test/test_copy.py` & `pulp_rpm-client-3.9.1/test/test_copy.py`

 * *Files identical despite different names*

### Comparing `pulp_rpm-client-3.9.0.dev1611548779/test/test_distributions_rpm_api.py` & `pulp_rpm-client-3.9.1/test/test_distributions_rpm_api.py`

 * *Files identical despite different names*

### Comparing `pulp_rpm-client-3.9.0.dev1611548779/test/test_image_response.py` & `pulp_rpm-client-3.9.1/test/test_image_response.py`

 * *Files identical despite different names*

### Comparing `pulp_rpm-client-3.9.0.dev1611548779/test/test_metadata_checksum_type_enum.py` & `pulp_rpm-client-3.9.1/test/test_metadata_checksum_type_enum.py`

 * *Files identical despite different names*

### Comparing `pulp_rpm-client-3.9.0.dev1611548779/test/test_package_checksum_type_enum.py` & `pulp_rpm-client-3.9.1/test/test_package_checksum_type_enum.py`

 * *Files identical despite different names*

### Comparing `pulp_rpm-client-3.9.0.dev1611548779/test/test_paginated_repository_version_response_list.py` & `pulp_rpm-client-3.9.1/test/test_paginated_repository_version_response_list.py`

 * *Files identical despite different names*

### Comparing `pulp_rpm-client-3.9.0.dev1611548779/test/test_paginatedrpm_distribution_tree_response_list.py` & `pulp_rpm-client-3.9.1/test/test_paginatedrpm_distribution_tree_response_list.py`

 * *Files identical despite different names*

### Comparing `pulp_rpm-client-3.9.0.dev1611548779/test/test_paginatedrpm_modulemd_defaults_response_list.py` & `pulp_rpm-client-3.9.1/test/test_paginatedrpm_modulemd_defaults_response_list.py`

 * *Files identical despite different names*

### Comparing `pulp_rpm-client-3.9.0.dev1611548779/test/test_paginatedrpm_modulemd_response_list.py` & `pulp_rpm-client-3.9.1/test/test_paginatedrpm_modulemd_response_list.py`

 * *Files identical despite different names*

### Comparing `pulp_rpm-client-3.9.0.dev1611548779/test/test_paginatedrpm_package_category_response_list.py` & `pulp_rpm-client-3.9.1/test/test_paginatedrpm_package_category_response_list.py`

 * *Files identical despite different names*

### Comparing `pulp_rpm-client-3.9.0.dev1611548779/test/test_paginatedrpm_package_environment_response_list.py` & `pulp_rpm-client-3.9.1/test/test_paginatedrpm_package_environment_response_list.py`

 * *Files identical despite different names*

### Comparing `pulp_rpm-client-3.9.0.dev1611548779/test/test_paginatedrpm_package_group_response_list.py` & `pulp_rpm-client-3.9.1/test/test_paginatedrpm_package_group_response_list.py`

 * *Files identical despite different names*

### Comparing `pulp_rpm-client-3.9.0.dev1611548779/test/test_paginatedrpm_package_langpacks_response_list.py` & `pulp_rpm-client-3.9.1/test/test_paginatedrpm_package_langpacks_response_list.py`

 * *Files identical despite different names*

### Comparing `pulp_rpm-client-3.9.0.dev1611548779/test/test_paginatedrpm_package_response_list.py` & `pulp_rpm-client-3.9.1/test/test_paginatedrpm_package_response_list.py`

 * *Files identical despite different names*

### Comparing `pulp_rpm-client-3.9.0.dev1611548779/test/test_paginatedrpm_repo_metadata_file_response_list.py` & `pulp_rpm-client-3.9.1/test/test_paginatedrpm_repo_metadata_file_response_list.py`

 * *Files identical despite different names*

### Comparing `pulp_rpm-client-3.9.0.dev1611548779/test/test_paginatedrpm_rpm_distribution_response_list.py` & `pulp_rpm-client-3.9.1/test/test_paginatedrpm_rpm_distribution_response_list.py`

 * *Files 9% similar despite different names*

```diff
@@ -43,14 +43,15 @@
                 results = [
                     pulpcore.client.pulp_rpm.models.rpm/rpm_distribution_response.rpm.RpmDistributionResponse(
                         pulp_href = '0', 
                         pulp_created = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
                         base_path = '0', 
                         base_url = '0', 
                         content_guard = '0', 
+                        pulp_labels = pulpcore.client.pulp_rpm.models.pulp_labels.pulp_labels(), 
                         name = '0', 
                         publication = '0', )
                     ]
             )
         else :
             return PaginatedrpmRpmDistributionResponseList(
         )
```

### Comparing `pulp_rpm-client-3.9.0.dev1611548779/test/test_paginatedrpm_rpm_publication_response_list.py` & `pulp_rpm-client-3.9.1/test/test_paginatedrpm_rpm_publication_response_list.py`

 * *Files identical despite different names*

### Comparing `pulp_rpm-client-3.9.0.dev1611548779/test/test_paginatedrpm_rpm_remote_response_list.py` & `pulp_rpm-client-3.9.1/test/test_paginatedrpm_rpm_remote_response_list.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,21 +49,23 @@
                         ca_cert = '0', 
                         client_cert = '0', 
                         client_key = '0', 
                         tls_validation = True, 
                         proxy_url = '0', 
                         username = '0', 
                         password = '0', 
+                        pulp_labels = pulpcore.client.pulp_rpm.models.pulp_labels.pulp_labels(), 
                         pulp_last_updated = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
                         download_concurrency = 1, 
                         policy = null, 
                         total_timeout = 0.0, 
                         connect_timeout = 0.0, 
                         sock_connect_timeout = 0.0, 
                         sock_read_timeout = 0.0, 
+                        rate_limit = 56, 
                         sles_auth_token = '0', )
                     ]
             )
         else :
             return PaginatedrpmRpmRemoteResponseList(
         )
```

### Comparing `pulp_rpm-client-3.9.0.dev1611548779/test/test_paginatedrpm_rpm_repository_response_list.py` & `pulp_rpm-client-3.9.1/test/test_paginatedrpm_rpm_repository_response_list.py`

 * *Files 13% similar despite different names*

```diff
@@ -41,14 +41,15 @@
                 next = 'http://api.example.org/accounts/?offset=400&limit=100', 
                 previous = 'http://api.example.org/accounts/?offset=200&limit=100', 
                 results = [
                     pulpcore.client.pulp_rpm.models.rpm/rpm_repository_response.rpm.RpmRepositoryResponse(
                         pulp_href = '0', 
                         pulp_created = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
                         versions_href = '0', 
+                        pulp_labels = pulpcore.client.pulp_rpm.models.pulp_labels.pulp_labels(), 
                         latest_version_href = '0', 
                         name = '0', 
                         description = '0', 
                         remote = '0', 
                         metadata_signing_service = '0', 
                         retain_package_versions = 0, )
                     ]
```

### Comparing `pulp_rpm-client-3.9.0.dev1611548779/test/test_paginatedrpm_update_record_response_list.py` & `pulp_rpm-client-3.9.1/test/test_paginatedrpm_update_record_response_list.py`

 * *Files identical despite different names*

### Comparing `pulp_rpm-client-3.9.0.dev1611548779/test/test_patchedrpm_rpm_distribution.py` & `pulp_rpm-client-3.9.1/test/test_rpm_rpm_distribution.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,44 +13,47 @@
 
 from __future__ import absolute_import
 
 import unittest
 import datetime
 
 import pulpcore.client.pulp_rpm
-from pulpcore.client.pulp_rpm.models.patchedrpm_rpm_distribution import PatchedrpmRpmDistribution  # noqa: E501
+from pulpcore.client.pulp_rpm.models.rpm_rpm_distribution import RpmRpmDistribution  # noqa: E501
 from pulpcore.client.pulp_rpm.rest import ApiException
 
-class TestPatchedrpmRpmDistribution(unittest.TestCase):
-    """PatchedrpmRpmDistribution unit test stubs"""
+class TestRpmRpmDistribution(unittest.TestCase):
+    """RpmRpmDistribution unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test PatchedrpmRpmDistribution
+        """Test RpmRpmDistribution
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # model = pulpcore.client.pulp_rpm.models.patchedrpm_rpm_distribution.PatchedrpmRpmDistribution()  # noqa: E501
+        # model = pulpcore.client.pulp_rpm.models.rpm_rpm_distribution.RpmRpmDistribution()  # noqa: E501
         if include_optional :
-            return PatchedrpmRpmDistribution(
+            return RpmRpmDistribution(
                 base_path = '0', 
                 content_guard = '0', 
+                pulp_labels = None, 
                 name = '0', 
                 publication = '0'
             )
         else :
-            return PatchedrpmRpmDistribution(
+            return RpmRpmDistribution(
+                base_path = '0',
+                name = '0',
         )
 
-    def testPatchedrpmRpmDistribution(self):
-        """Test PatchedrpmRpmDistribution"""
+    def testRpmRpmDistribution(self):
+        """Test RpmRpmDistribution"""
         inst_req_only = self.make_instance(include_optional=False)
         inst_req_and_optional = self.make_instance(include_optional=True)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `pulp_rpm-client-3.9.0.dev1611548779/test/test_patchedrpm_rpm_remote.py` & `pulp_rpm-client-3.9.1/test/test_patchedrpm_rpm_remote.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,20 +42,22 @@
                 ca_cert = '0', 
                 client_cert = '0', 
                 client_key = '0', 
                 tls_validation = True, 
                 proxy_url = '0', 
                 username = '0', 
                 password = '0', 
+                pulp_labels = None, 
                 download_concurrency = 1, 
                 policy = null, 
                 total_timeout = 0.0, 
                 connect_timeout = 0.0, 
                 sock_connect_timeout = 0.0, 
                 sock_read_timeout = 0.0, 
+                rate_limit = 56, 
                 sles_auth_token = '0'
             )
         else :
             return PatchedrpmRpmRemote(
         )
 
     def testPatchedrpmRpmRemote(self):
```

### Comparing `pulp_rpm-client-3.9.0.dev1611548779/test/test_patchedrpm_rpm_repository.py` & `pulp_rpm-client-3.9.1/test/test_patchedrpm_rpm_repository.py`

 * *Files 5% similar despite different names*

```diff
@@ -33,14 +33,15 @@
         """Test PatchedrpmRpmRepository
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
         # model = pulpcore.client.pulp_rpm.models.patchedrpm_rpm_repository.PatchedrpmRpmRepository()  # noqa: E501
         if include_optional :
             return PatchedrpmRpmRepository(
+                pulp_labels = None, 
                 name = '0', 
                 description = '0', 
                 remote = '0', 
                 metadata_signing_service = '0', 
                 retain_package_versions = 0
             )
         else :
```

### Comparing `pulp_rpm-client-3.9.0.dev1611548779/test/test_policy_enum.py` & `pulp_rpm-client-3.9.1/test/test_policy_enum.py`

 * *Files identical despite different names*

### Comparing `pulp_rpm-client-3.9.0.dev1611548779/test/test_publications_rpm_api.py` & `pulp_rpm-client-3.9.1/test/test_publications_rpm_api.py`

 * *Files identical despite different names*

### Comparing `pulp_rpm-client-3.9.0.dev1611548779/test/test_remotes_rpm_api.py` & `pulp_rpm-client-3.9.1/test/test_remotes_rpm_api.py`

 * *Files identical despite different names*

### Comparing `pulp_rpm-client-3.9.0.dev1611548779/test/test_repositories_rpm_api.py` & `pulp_rpm-client-3.9.1/test/test_repositories_rpm_api.py`

 * *Files identical despite different names*

### Comparing `pulp_rpm-client-3.9.0.dev1611548779/test/test_repositories_rpm_versions_api.py` & `pulp_rpm-client-3.9.1/test/test_repositories_rpm_versions_api.py`

 * *Files identical despite different names*

### Comparing `pulp_rpm-client-3.9.0.dev1611548779/test/test_repository_add_remove_content.py` & `pulp_rpm-client-3.9.1/test/test_repository_add_remove_content.py`

 * *Files identical despite different names*

### Comparing `pulp_rpm-client-3.9.0.dev1611548779/test/test_repository_version.py` & `pulp_rpm-client-3.9.1/test/test_repository_version.py`

 * *Files identical despite different names*

### Comparing `pulp_rpm-client-3.9.0.dev1611548779/test/test_repository_version_response.py` & `pulp_rpm-client-3.9.1/test/test_repository_version_response.py`

 * *Files identical despite different names*

### Comparing `pulp_rpm-client-3.9.0.dev1611548779/test/test_rpm_copy_api.py` & `pulp_rpm-client-3.9.1/test/test_rpm_copy_api.py`

 * *Files identical despite different names*

### Comparing `pulp_rpm-client-3.9.0.dev1611548779/test/test_rpm_distribution_tree_response.py` & `pulp_rpm-client-3.9.1/test/test_rpm_distribution_tree_response.py`

 * *Files identical despite different names*

### Comparing `pulp_rpm-client-3.9.0.dev1611548779/test/test_rpm_modulemd.py` & `pulp_rpm-client-3.9.1/test/test_rpm_modulemd.py`

 * *Files identical despite different names*

### Comparing `pulp_rpm-client-3.9.0.dev1611548779/test/test_rpm_modulemd_defaults.py` & `pulp_rpm-client-3.9.1/test/test_rpm_modulemd_defaults.py`

 * *Files identical despite different names*

### Comparing `pulp_rpm-client-3.9.0.dev1611548779/test/test_rpm_modulemd_defaults_response.py` & `pulp_rpm-client-3.9.1/test/test_rpm_modulemd_defaults_response.py`

 * *Files identical despite different names*

### Comparing `pulp_rpm-client-3.9.0.dev1611548779/test/test_rpm_modulemd_response.py` & `pulp_rpm-client-3.9.1/test/test_rpm_modulemd_response.py`

 * *Files identical despite different names*

### Comparing `pulp_rpm-client-3.9.0.dev1611548779/test/test_rpm_package.py` & `pulp_rpm-client-3.9.1/test/test_rpm_package.py`

 * *Files identical despite different names*

### Comparing `pulp_rpm-client-3.9.0.dev1611548779/test/test_rpm_package_category_response.py` & `pulp_rpm-client-3.9.1/test/test_rpm_package_category_response.py`

 * *Files identical despite different names*

### Comparing `pulp_rpm-client-3.9.0.dev1611548779/test/test_rpm_package_environment_response.py` & `pulp_rpm-client-3.9.1/test/test_rpm_package_environment_response.py`

 * *Files identical despite different names*

### Comparing `pulp_rpm-client-3.9.0.dev1611548779/test/test_rpm_package_group_response.py` & `pulp_rpm-client-3.9.1/test/test_rpm_package_group_response.py`

 * *Files identical despite different names*

### Comparing `pulp_rpm-client-3.9.0.dev1611548779/test/test_rpm_package_langpacks_response.py` & `pulp_rpm-client-3.9.1/test/test_rpm_package_langpacks_response.py`

 * *Files identical despite different names*

### Comparing `pulp_rpm-client-3.9.0.dev1611548779/test/test_rpm_package_response.py` & `pulp_rpm-client-3.9.1/test/test_rpm_package_response.py`

 * *Files identical despite different names*

### Comparing `pulp_rpm-client-3.9.0.dev1611548779/test/test_rpm_repo_metadata_file_response.py` & `pulp_rpm-client-3.9.1/test/test_rpm_repo_metadata_file_response.py`

 * *Files identical despite different names*

### Comparing `pulp_rpm-client-3.9.0.dev1611548779/test/test_rpm_repository_sync_url.py` & `pulp_rpm-client-3.9.1/test/test_rpm_repository_sync_url.py`

 * *Files identical despite different names*

### Comparing `pulp_rpm-client-3.9.0.dev1611548779/test/test_rpm_rpm_distribution.py` & `pulp_rpm-client-3.9.1/test/test_patchedrpm_rpm_distribution.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,46 +13,45 @@
 
 from __future__ import absolute_import
 
 import unittest
 import datetime
 
 import pulpcore.client.pulp_rpm
-from pulpcore.client.pulp_rpm.models.rpm_rpm_distribution import RpmRpmDistribution  # noqa: E501
+from pulpcore.client.pulp_rpm.models.patchedrpm_rpm_distribution import PatchedrpmRpmDistribution  # noqa: E501
 from pulpcore.client.pulp_rpm.rest import ApiException
 
-class TestRpmRpmDistribution(unittest.TestCase):
-    """RpmRpmDistribution unit test stubs"""
+class TestPatchedrpmRpmDistribution(unittest.TestCase):
+    """PatchedrpmRpmDistribution unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test RpmRpmDistribution
+        """Test PatchedrpmRpmDistribution
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # model = pulpcore.client.pulp_rpm.models.rpm_rpm_distribution.RpmRpmDistribution()  # noqa: E501
+        # model = pulpcore.client.pulp_rpm.models.patchedrpm_rpm_distribution.PatchedrpmRpmDistribution()  # noqa: E501
         if include_optional :
-            return RpmRpmDistribution(
+            return PatchedrpmRpmDistribution(
                 base_path = '0', 
                 content_guard = '0', 
+                pulp_labels = None, 
                 name = '0', 
                 publication = '0'
             )
         else :
-            return RpmRpmDistribution(
-                base_path = '0',
-                name = '0',
+            return PatchedrpmRpmDistribution(
         )
 
-    def testRpmRpmDistribution(self):
-        """Test RpmRpmDistribution"""
+    def testPatchedrpmRpmDistribution(self):
+        """Test PatchedrpmRpmDistribution"""
         inst_req_only = self.make_instance(include_optional=False)
         inst_req_and_optional = self.make_instance(include_optional=True)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `pulp_rpm-client-3.9.0.dev1611548779/test/test_rpm_rpm_distribution_response.py` & `pulp_rpm-client-3.9.1/test/test_rpm_rpm_distribution_response.py`

 * *Files 10% similar despite different names*

```diff
@@ -38,14 +38,15 @@
         if include_optional :
             return RpmRpmDistributionResponse(
                 pulp_href = '0', 
                 pulp_created = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
                 base_path = '0', 
                 base_url = '0', 
                 content_guard = '0', 
+                pulp_labels = pulpcore.client.pulp_rpm.models.pulp_labels.pulp_labels(), 
                 name = '0', 
                 publication = '0'
             )
         else :
             return RpmRpmDistributionResponse(
                 base_path = '0',
                 name = '0',
```

### Comparing `pulp_rpm-client-3.9.0.dev1611548779/test/test_rpm_rpm_publication.py` & `pulp_rpm-client-3.9.1/test/test_rpm_rpm_publication.py`

 * *Files identical despite different names*

### Comparing `pulp_rpm-client-3.9.0.dev1611548779/test/test_rpm_rpm_publication_response.py` & `pulp_rpm-client-3.9.1/test/test_rpm_rpm_publication_response.py`

 * *Files identical despite different names*

### Comparing `pulp_rpm-client-3.9.0.dev1611548779/test/test_rpm_rpm_remote.py` & `pulp_rpm-client-3.9.1/test/test_rpm_rpm_remote.py`

 * *Files 3% similar despite different names*

```diff
@@ -42,20 +42,22 @@
                 ca_cert = '0', 
                 client_cert = '0', 
                 client_key = '0', 
                 tls_validation = True, 
                 proxy_url = '0', 
                 username = '0', 
                 password = '0', 
+                pulp_labels = None, 
                 download_concurrency = 1, 
                 policy = null, 
                 total_timeout = 0.0, 
                 connect_timeout = 0.0, 
                 sock_connect_timeout = 0.0, 
                 sock_read_timeout = 0.0, 
+                rate_limit = 56, 
                 sles_auth_token = '0'
             )
         else :
             return RpmRpmRemote(
                 name = '0',
                 url = '0',
         )
```

### Comparing `pulp_rpm-client-3.9.0.dev1611548779/test/test_rpm_rpm_remote_response.py` & `pulp_rpm-client-3.9.1/test/test_rpm_rpm_remote_response.py`

 * *Files 4% similar despite different names*

```diff
@@ -44,21 +44,23 @@
                 ca_cert = '0', 
                 client_cert = '0', 
                 client_key = '0', 
                 tls_validation = True, 
                 proxy_url = '0', 
                 username = '0', 
                 password = '0', 
+                pulp_labels = pulpcore.client.pulp_rpm.models.pulp_labels.pulp_labels(), 
                 pulp_last_updated = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
                 download_concurrency = 1, 
                 policy = null, 
                 total_timeout = 0.0, 
                 connect_timeout = 0.0, 
                 sock_connect_timeout = 0.0, 
                 sock_read_timeout = 0.0, 
+                rate_limit = 56, 
                 sles_auth_token = '0'
             )
         else :
             return RpmRpmRemoteResponse(
                 name = '0',
                 url = '0',
         )
```

### Comparing `pulp_rpm-client-3.9.0.dev1611548779/test/test_rpm_rpm_repository.py` & `pulp_rpm-client-3.9.1/test/test_rpm_rpm_repository.py`

 * *Files 8% similar despite different names*

```diff
@@ -33,14 +33,15 @@
         """Test RpmRpmRepository
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
         # model = pulpcore.client.pulp_rpm.models.rpm_rpm_repository.RpmRpmRepository()  # noqa: E501
         if include_optional :
             return RpmRpmRepository(
+                pulp_labels = None, 
                 name = '0', 
                 description = '0', 
                 remote = '0', 
                 metadata_signing_service = '0', 
                 retain_package_versions = 0
             )
         else :
```

### Comparing `pulp_rpm-client-3.9.0.dev1611548779/test/test_rpm_rpm_repository_response.py` & `pulp_rpm-client-3.9.1/test/test_rpm_rpm_repository_response.py`

 * *Files 10% similar despite different names*

```diff
@@ -36,14 +36,15 @@
             optional params are included """
         # model = pulpcore.client.pulp_rpm.models.rpm_rpm_repository_response.RpmRpmRepositoryResponse()  # noqa: E501
         if include_optional :
             return RpmRpmRepositoryResponse(
                 pulp_href = '0', 
                 pulp_created = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
                 versions_href = '0', 
+                pulp_labels = pulpcore.client.pulp_rpm.models.pulp_labels.pulp_labels(), 
                 latest_version_href = '0', 
                 name = '0', 
                 description = '0', 
                 remote = '0', 
                 metadata_signing_service = '0', 
                 retain_package_versions = 0
             )
```

### Comparing `pulp_rpm-client-3.9.0.dev1611548779/test/test_rpm_update_collection.py` & `pulp_rpm-client-3.9.1/test/test_rpm_update_collection.py`

 * *Files identical despite different names*

### Comparing `pulp_rpm-client-3.9.0.dev1611548779/test/test_rpm_update_collection_response.py` & `pulp_rpm-client-3.9.1/test/test_rpm_update_collection_response.py`

 * *Files identical despite different names*

### Comparing `pulp_rpm-client-3.9.0.dev1611548779/test/test_rpm_update_record.py` & `pulp_rpm-client-3.9.1/test/test_rpm_update_record.py`

 * *Files identical despite different names*

### Comparing `pulp_rpm-client-3.9.0.dev1611548779/test/test_rpm_update_record_response.py` & `pulp_rpm-client-3.9.1/test/test_rpm_update_record_response.py`

 * *Files identical despite different names*

### Comparing `pulp_rpm-client-3.9.0.dev1611548779/test/test_variant_response.py` & `pulp_rpm-client-3.9.1/test/test_variant_response.py`

 * *Files identical despite different names*

