# Comparing `tmp/pulp-rpm-3.9.0.tar.gz` & `tmp/pulp-rpm-3.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pulp-rpm-3.9.0.tar", last modified: Thu Feb  4 22:09:55 2021, max compression
+gzip compressed data, was "dist/pulp-rpm-3.9.1.tar", last modified: Thu Mar 11 20:51:13 2021, max compression
```

## Comparing `pulp-rpm-3.9.0.tar` & `pulp-rpm-3.9.1.tar`

### file list

```diff
@@ -1,137 +1,137 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-04 22:09:55.000000 pulp-rpm-3.9.0/
--rw-r--r--   0 runner    (1001) docker     (116)    28871 2021-02-04 22:04:48.000000 pulp-rpm-3.9.0/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (116)     2095 2021-02-04 22:04:48.000000 pulp-rpm-3.9.0/COMMITMENT
--rw-r--r--   0 runner    (1001) docker     (116)      540 2021-02-04 22:04:48.000000 pulp-rpm-3.9.0/COPYRIGHT
--rw-r--r--   0 runner    (1001) docker     (116)    17988 2021-02-04 22:04:48.000000 pulp-rpm-3.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (116)      320 2021-02-04 22:04:48.000000 pulp-rpm-3.9.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (116)     2686 2021-02-04 22:09:55.000000 pulp-rpm-3.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     1612 2021-02-04 22:04:48.000000 pulp-rpm-3.9.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (116)     5692 2021-02-04 22:04:48.000000 pulp-rpm-3.9.0/coverage.md
--rw-r--r--   0 runner    (1001) docker     (116)      175 2021-02-04 22:04:48.000000 pulp-rpm-3.9.0/functest_requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-04 22:09:55.000000 pulp-rpm-3.9.0/pulp_rpm/
--rw-r--r--   0 runner    (1001) docker     (116)       59 2021-02-04 22:04:48.000000 pulp-rpm-3.9.0/pulp_rpm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-04 22:09:55.000000 pulp-rpm-3.9.0/pulp_rpm/app/
--rw-r--r--   0 runner    (1001) docker     (116)      221 2021-02-04 22:04:48.000000 pulp-rpm-3.9.0/pulp_rpm/app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    13477 2021-02-04 22:04:48.000000 pulp-rpm-3.9.0/pulp_rpm/app/advisory.py
--rw-r--r--   0 runner    (1001) docker     (116)     1364 2021-02-04 22:04:48.000000 pulp-rpm-3.9.0/pulp_rpm/app/comps.py
--rw-r--r--   0 runner    (1001) docker     (116)     6531 2021-02-04 22:04:48.000000 pulp-rpm-3.9.0/pulp_rpm/app/constants.py
--rw-r--r--   0 runner    (1001) docker     (116)    36032 2021-02-04 22:04:48.000000 pulp-rpm-3.9.0/pulp_rpm/app/depsolving.py
--rw-r--r--   0 runner    (1001) docker     (116)     3228 2021-02-04 22:04:48.000000 pulp-rpm-3.9.0/pulp_rpm/app/downloaders.py
--rw-r--r--   0 runner    (1001) docker     (116)     1071 2021-02-04 22:04:48.000000 pulp-rpm-3.9.0/pulp_rpm/app/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (116)     2384 2021-02-04 22:04:48.000000 pulp-rpm-3.9.0/pulp_rpm/app/fields.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-04 22:09:55.000000 pulp-rpm-3.9.0/pulp_rpm/app/kickstart/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2021-02-04 22:04:48.000000 pulp-rpm-3.9.0/pulp_rpm/app/kickstart/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    12313 2021-02-04 22:04:48.000000 pulp-rpm-3.9.0/pulp_rpm/app/kickstart/treeinfo.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-04 22:09:55.000000 pulp-rpm-3.9.0/pulp_rpm/app/migrations/
--rw-r--r--   0 runner    (1001) docker     (116)    23255 2021-02-04 22:04:48.000000 pulp-rpm-3.9.0/pulp_rpm/app/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (116)      388 2021-02-04 22:04:48.000000 pulp-rpm-3.9.0/pulp_rpm/app/migrations/0002_updaterecord_reboot_suggested.py
--rw-r--r--   0 runner    (1001) docker     (116)     2676 2021-02-04 22:04:48.000000 pulp-rpm-3.9.0/pulp_rpm/app/migrations/0003_DATA_incorrect_json.py
--rw-r--r--   0 runner    (1001) docker     (116)      609 2021-02-04 22:04:48.000000 pulp-rpm-3.9.0/pulp_rpm/app/migrations/0004_add_metadata_signing_service_fk.py
--rw-r--r--   0 runner    (1001) docker     (116)      954 2021-02-04 22:04:48.000000 pulp-rpm-3.9.0/pulp_rpm/app/migrations/0005_optimize_sync.py
--rw-r--r--   0 runner    (1001) docker     (116)      908 2021-02-04 22:04:48.000000 pulp-rpm-3.9.0/pulp_rpm/app/migrations/0006_opensuse_support.py
--rw-r--r--   0 runner    (1001) docker     (116)     1281 2021-02-04 22:04:48.000000 pulp-rpm-3.9.0/pulp_rpm/app/migrations/0007_checksum_types.py
--rw-r--r--   0 runner    (1001) docker     (116)     1532 2021-02-04 22:04:48.000000 pulp-rpm-3.9.0/pulp_rpm/app/migrations/0008_advisory_pkg_sumtype_as_int.py
--rw-r--r--   0 runner    (1001) docker     (116)      429 2021-02-04 22:04:48.000000 pulp-rpm-3.9.0/pulp_rpm/app/migrations/0009_revision_null.py
--rw-r--r--   0 runner    (1001) docker     (116)      415 2021-02-04 22:04:48.000000 pulp-rpm-3.9.0/pulp_rpm/app/migrations/0010_revision_null_redo.py
--rw-r--r--   0 runner    (1001) docker     (116)      405 2021-02-04 22:04:48.000000 pulp-rpm-3.9.0/pulp_rpm/app/migrations/0011_rpmremote_sles_auth_token.py
--rw-r--r--   0 runner    (1001) docker     (116)      712 2021-02-04 22:04:48.000000 pulp-rpm-3.9.0/pulp_rpm/app/migrations/0012_remove_pkg_group_env_cat_related_pkgs.py
--rw-r--r--   0 runner    (1001) docker     (116)     4734 2021-02-04 22:04:48.000000 pulp-rpm-3.9.0/pulp_rpm/app/migrations/0013_RAW_rpm_evr_extension.py
--rw-r--r--   0 runner    (1001) docker     (116)      415 2021-02-04 22:04:48.000000 pulp-rpm-3.9.0/pulp_rpm/app/migrations/0014_rpmrepository_package_retention_policy.py
--rw-r--r--   0 runner    (1001) docker     (116)      932 2021-02-04 22:04:48.000000 pulp-rpm-3.9.0/pulp_rpm/app/migrations/0015_repo_metadata.py
--rw-r--r--   0 runner    (1001) docker     (116)      882 2021-02-04 22:04:48.000000 pulp-rpm-3.9.0/pulp_rpm/app/migrations/0016_dist_tree_nofk.py
--rw-r--r--   0 runner    (1001) docker     (116)     1937 2021-02-04 22:04:48.000000 pulp-rpm-3.9.0/pulp_rpm/app/migrations/0017_merge_advisory_collections.py
--rw-r--r--   0 runner    (1001) docker     (116)      546 2021-02-04 22:04:48.000000 pulp-rpm-3.9.0/pulp_rpm/app/migrations/0018_updatecollection__update_record.py
--rw-r--r--   0 runner    (1001) docker     (116)     2630 2021-02-04 22:04:48.000000 pulp-rpm-3.9.0/pulp_rpm/app/migrations/0019_migrate_updatecollection_data.py
--rw-r--r--   0 runner    (1001) docker     (116)      353 2021-02-04 22:04:48.000000 pulp-rpm-3.9.0/pulp_rpm/app/migrations/0020_remove_updatecollection_m2m.py
--rw-r--r--   0 runner    (1001) docker     (116)      435 2021-02-04 22:04:48.000000 pulp-rpm-3.9.0/pulp_rpm/app/migrations/0021_rename_updatecollection_update_record.py
--rw-r--r--   0 runner    (1001) docker     (116)      679 2021-02-04 22:04:48.000000 pulp-rpm-3.9.0/pulp_rpm/app/migrations/0022_add_collections_related_name.py
--rw-r--r--   0 runner    (1001) docker     (116)      746 2021-02-04 22:04:48.000000 pulp-rpm-3.9.0/pulp_rpm/app/migrations/0023_increase_distribution_release_short.py
--rw-r--r--   0 runner    (1001) docker     (116)      527 2021-02-04 22:04:48.000000 pulp-rpm-3.9.0/pulp_rpm/app/migrations/0024_change_subrepo_relation_properties.py
--rw-r--r--   0 runner    (1001) docker     (116)      505 2021-02-04 22:04:48.000000 pulp-rpm-3.9.0/pulp_rpm/app/migrations/0025_remove_orphaned_subrepos.py
--rw-r--r--   0 runner    (1001) docker     (116)      613 2021-02-04 22:04:48.000000 pulp-rpm-3.9.0/pulp_rpm/app/migrations/0026_add_gpgcheck_options.py
--rw-r--r--   0 runner    (1001) docker     (116)     1510 2021-02-04 22:04:48.000000 pulp-rpm-3.9.0/pulp_rpm/app/migrations/0027_checksum_null.py
--rw-r--r--   0 runner    (1001) docker     (116)      413 2021-02-04 22:04:48.000000 pulp-rpm-3.9.0/pulp_rpm/app/migrations/0028_rpmrepository_last_sync_repomd_cheksum.py
--rw-r--r--   0 runner    (1001) docker     (116)      607 2021-02-04 22:04:48.000000 pulp-rpm-3.9.0/pulp_rpm/app/migrations/0029_rpmpublication_sqlite_metadata.py
--rw-r--r--   0 runner    (1001) docker     (116)      933 2021-02-04 22:04:48.000000 pulp-rpm-3.9.0/pulp_rpm/app/migrations/0030_DATA_fix_updaterecord.py
--rw-r--r--   0 runner    (1001) docker     (116)        0 2021-02-04 22:04:48.000000 pulp-rpm-3.9.0/pulp_rpm/app/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    14679 2021-02-04 22:04:48.000000 pulp-rpm-3.9.0/pulp_rpm/app/modelresource.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-04 22:09:55.000000 pulp-rpm-3.9.0/pulp_rpm/app/models/
--rw-r--r--   0 runner    (1001) docker     (116)      541 2021-02-04 22:04:48.000000 pulp-rpm-3.9.0/pulp_rpm/app/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    18288 2021-02-04 22:04:48.000000 pulp-rpm-3.9.0/pulp_rpm/app/models/advisory.py
--rw-r--r--   0 runner    (1001) docker     (116)    15139 2021-02-04 22:04:48.000000 pulp-rpm-3.9.0/pulp_rpm/app/models/comps.py
--rw-r--r--   0 runner    (1001) docker     (116)      838 2021-02-04 22:04:48.000000 pulp-rpm-3.9.0/pulp_rpm/app/models/custom_metadata.py
--rw-r--r--   0 runner    (1001) docker     (116)     9872 2021-02-04 22:04:48.000000 pulp-rpm-3.9.0/pulp_rpm/app/models/distribution.py
--rw-r--r--   0 runner    (1001) docker     (116)     2462 2021-02-04 22:04:48.000000 pulp-rpm-3.9.0/pulp_rpm/app/models/modulemd.py
--rw-r--r--   0 runner    (1001) docker     (116)    17275 2021-02-04 22:04:48.000000 pulp-rpm-3.9.0/pulp_rpm/app/models/package.py
--rw-r--r--   0 runner    (1001) docker     (116)    13590 2021-02-04 22:04:48.000000 pulp-rpm-3.9.0/pulp_rpm/app/models/repository.py
--rw-r--r--   0 runner    (1001) docker     (116)     5310 2021-02-04 22:04:48.000000 pulp-rpm-3.9.0/pulp_rpm/app/modulemd.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-04 22:09:55.000000 pulp-rpm-3.9.0/pulp_rpm/app/schema/
--rw-r--r--   0 runner    (1001) docker     (116)      207 2021-02-04 22:04:48.000000 pulp-rpm-3.9.0/pulp_rpm/app/schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      568 2021-02-04 22:04:48.000000 pulp-rpm-3.9.0/pulp_rpm/app/schema/copy_config.json
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-04 22:09:55.000000 pulp-rpm-3.9.0/pulp_rpm/app/serializers/
--rw-r--r--   0 runner    (1001) docker     (116)      865 2021-02-04 22:04:48.000000 pulp-rpm-3.9.0/pulp_rpm/app/serializers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     9048 2021-02-04 22:04:48.000000 pulp-rpm-3.9.0/pulp_rpm/app/serializers/advisory.py
--rw-r--r--   0 runner    (1001) docker     (116)     4857 2021-02-04 22:04:48.000000 pulp-rpm-3.9.0/pulp_rpm/app/serializers/comps.py
--rw-r--r--   0 runner    (1001) docker     (116)     1022 2021-02-04 22:04:48.000000 pulp-rpm-3.9.0/pulp_rpm/app/serializers/custom_metadata.py
--rw-r--r--   0 runner    (1001) docker     (116)     5336 2021-02-04 22:04:48.000000 pulp-rpm-3.9.0/pulp_rpm/app/serializers/distribution.py
--rw-r--r--   0 runner    (1001) docker     (116)     2688 2021-02-04 22:04:48.000000 pulp-rpm-3.9.0/pulp_rpm/app/serializers/modulemd.py
--rw-r--r--   0 runner    (1001) docker     (116)     9667 2021-02-04 22:04:48.000000 pulp-rpm-3.9.0/pulp_rpm/app/serializers/package.py
--rw-r--r--   0 runner    (1001) docker     (116)     6454 2021-02-04 22:04:48.000000 pulp-rpm-3.9.0/pulp_rpm/app/serializers/repository.py
--rw-r--r--   0 runner    (1001) docker     (116)      212 2021-02-04 22:04:48.000000 pulp-rpm-3.9.0/pulp_rpm/app/settings.py
--rw-r--r--   0 runner    (1001) docker     (116)     2383 2021-02-04 22:04:48.000000 pulp-rpm-3.9.0/pulp_rpm/app/shared_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-04 22:09:55.000000 pulp-rpm-3.9.0/pulp_rpm/app/tasks/
--rw-r--r--   0 runner    (1001) docker     (116)      126 2021-02-04 22:04:48.000000 pulp-rpm-3.9.0/pulp_rpm/app/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     9122 2021-02-04 22:04:48.000000 pulp-rpm-3.9.0/pulp_rpm/app/tasks/copy.py
--rw-r--r--   0 runner    (1001) docker     (116)    22308 2021-02-04 22:04:48.000000 pulp-rpm-3.9.0/pulp_rpm/app/tasks/publishing.py
--rw-r--r--   0 runner    (1001) docker     (116)    43724 2021-02-04 22:04:48.000000 pulp-rpm-3.9.0/pulp_rpm/app/tasks/synchronizing.py
--rw-r--r--   0 runner    (1001) docker     (116)      159 2021-02-04 22:04:48.000000 pulp-rpm-3.9.0/pulp_rpm/app/urls.py
--rw-r--r--   0 runner    (1001) docker     (116)    13161 2021-02-04 22:04:48.000000 pulp-rpm-3.9.0/pulp_rpm/app/viewsets.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-04 22:09:55.000000 pulp-rpm-3.9.0/pulp_rpm/tests/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2021-02-04 22:04:48.000000 pulp-rpm-3.9.0/pulp_rpm/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-04 22:09:55.000000 pulp-rpm-3.9.0/pulp_rpm/tests/functional/
--rw-r--r--   0 runner    (1001) docker     (116)       44 2021-02-04 22:04:48.000000 pulp-rpm-3.9.0/pulp_rpm/tests/functional/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-04 22:09:55.000000 pulp-rpm-3.9.0/pulp_rpm/tests/functional/api/
--rw-r--r--   0 runner    (1001) docker     (116)       77 2021-02-04 22:04:48.000000 pulp-rpm-3.9.0/pulp_rpm/tests/functional/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     2734 2021-02-04 22:04:48.000000 pulp-rpm-3.9.0/pulp_rpm/tests/functional/api/test_advisory_upload.py
--rw-r--r--   0 runner    (1001) docker     (116)     2686 2021-02-04 22:04:48.000000 pulp-rpm-3.9.0/pulp_rpm/tests/functional/api/test_character_encoding.py
--rw-r--r--   0 runner    (1001) docker     (116)     8955 2021-02-04 22:04:48.000000 pulp-rpm-3.9.0/pulp_rpm/tests/functional/api/test_consume_content.py
--rw-r--r--   0 runner    (1001) docker     (116)    22867 2021-02-04 22:04:48.000000 pulp-rpm-3.9.0/pulp_rpm/tests/functional/api/test_copy.py
--rw-r--r--   0 runner    (1001) docker     (116)     8729 2021-02-04 22:04:48.000000 pulp-rpm-3.9.0/pulp_rpm/tests/functional/api/test_crud_content_unit.py
--rw-r--r--   0 runner    (1001) docker     (116)     8037 2021-02-04 22:04:48.000000 pulp-rpm-3.9.0/pulp_rpm/tests/functional/api/test_crud_remotes.py
--rw-r--r--   0 runner    (1001) docker     (116)    10097 2021-02-04 22:04:48.000000 pulp-rpm-3.9.0/pulp_rpm/tests/functional/api/test_distribution_tree.py
--rw-r--r--   0 runner    (1001) docker     (116)     4218 2021-02-04 22:04:48.000000 pulp-rpm-3.9.0/pulp_rpm/tests/functional/api/test_download_content.py
--rw-r--r--   0 runner    (1001) docker     (116)     4281 2021-02-04 22:04:48.000000 pulp-rpm-3.9.0/pulp_rpm/tests/functional/api/test_download_policies.py
--rw-r--r--   0 runner    (1001) docker     (116)    29808 2021-02-04 22:04:48.000000 pulp-rpm-3.9.0/pulp_rpm/tests/functional/api/test_publish.py
--rw-r--r--   0 runner    (1001) docker     (116)     4817 2021-02-04 22:04:48.000000 pulp-rpm-3.9.0/pulp_rpm/tests/functional/api/test_pulp_to_pulp.py
--rw-r--r--   0 runner    (1001) docker     (116)     4683 2021-02-04 22:04:48.000000 pulp-rpm-3.9.0/pulp_rpm/tests/functional/api/test_pulpexport.py
--rw-r--r--   0 runner    (1001) docker     (116)     8977 2021-02-04 22:04:48.000000 pulp-rpm-3.9.0/pulp_rpm/tests/functional/api/test_pulpimport.py
--rw-r--r--   0 runner    (1001) docker     (116)     6475 2021-02-04 22:04:48.000000 pulp-rpm-3.9.0/pulp_rpm/tests/functional/api/test_retention_policy.py
--rw-r--r--   0 runner    (1001) docker     (116)    45871 2021-02-04 22:04:48.000000 pulp-rpm-3.9.0/pulp_rpm/tests/functional/api/test_sync.py
--rw-r--r--   0 runner    (1001) docker     (116)     2939 2021-02-04 22:04:48.000000 pulp-rpm-3.9.0/pulp_rpm/tests/functional/api/test_upload.py
--rw-r--r--   0 runner    (1001) docker     (116)    13754 2021-02-04 22:04:48.000000 pulp-rpm-3.9.0/pulp_rpm/tests/functional/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-04 22:09:55.000000 pulp-rpm-3.9.0/pulp_rpm/tests/functional/content_handler/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2021-02-04 22:04:48.000000 pulp-rpm-3.9.0/pulp_rpm/tests/functional/content_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     2740 2021-02-04 22:04:48.000000 pulp-rpm-3.9.0/pulp_rpm/tests/functional/content_handler/test_config_repo.py
--rwxr-xr-x   0 runner    (1001) docker     (116)      595 2021-02-04 22:04:48.000000 pulp-rpm-3.9.0/pulp_rpm/tests/functional/sign-metadata.sh
--rw-r--r--   0 runner    (1001) docker     (116)     8971 2021-02-04 22:04:48.000000 pulp-rpm-3.9.0/pulp_rpm/tests/functional/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-04 22:09:55.000000 pulp-rpm-3.9.0/pulp_rpm/tests/performance/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2021-02-04 22:04:48.000000 pulp-rpm-3.9.0/pulp_rpm/tests/performance/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     8153 2021-02-04 22:04:48.000000 pulp-rpm-3.9.0/pulp_rpm/tests/performance/test_publish.py
--rw-r--r--   0 runner    (1001) docker     (116)     5799 2021-02-04 22:04:48.000000 pulp-rpm-3.9.0/pulp_rpm/tests/performance/test_pulp_to_pulp.py
--rw-r--r--   0 runner    (1001) docker     (116)    11059 2021-02-04 22:04:48.000000 pulp-rpm-3.9.0/pulp_rpm/tests/performance/test_sync.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-04 22:09:55.000000 pulp-rpm-3.9.0/pulp_rpm/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2021-02-04 22:04:48.000000 pulp-rpm-3.9.0/pulp_rpm/tests/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      229 2021-02-04 22:04:48.000000 pulp-rpm-3.9.0/pulp_rpm/tests/unit/test_models.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-04 22:09:55.000000 pulp-rpm-3.9.0/pulp_rpm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     2686 2021-02-04 22:09:51.000000 pulp-rpm-3.9.0/pulp_rpm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     4750 2021-02-04 22:09:51.000000 pulp-rpm-3.9.0/pulp_rpm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2021-02-04 22:09:51.000000 pulp-rpm-3.9.0/pulp_rpm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)       58 2021-02-04 22:09:51.000000 pulp-rpm-3.9.0/pulp_rpm.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (116)      135 2021-02-04 22:09:51.000000 pulp-rpm-3.9.0/pulp_rpm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)        9 2021-02-04 22:09:51.000000 pulp-rpm-3.9.0/pulp_rpm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)      859 2021-02-04 22:04:48.000000 pulp-rpm-3.9.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (116)      135 2021-02-04 22:04:48.000000 pulp-rpm-3.9.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (116)       38 2021-02-04 22:09:55.000000 pulp-rpm-3.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     1194 2021-02-04 22:04:48.000000 pulp-rpm-3.9.0/setup.py
--rw-r--r--   0 runner    (1001) docker     (116)       82 2021-02-04 22:04:48.000000 pulp-rpm-3.9.0/test_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (116)        5 2021-02-04 22:04:48.000000 pulp-rpm-3.9.0/unittest_requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-11 20:51:13.000000 pulp-rpm-3.9.1/
+-rw-r--r--   0 runner    (1001) docker     (121)    29092 2021-03-11 20:45:43.000000 pulp-rpm-3.9.1/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     2095 2021-03-11 20:45:43.000000 pulp-rpm-3.9.1/COMMITMENT
+-rw-r--r--   0 runner    (1001) docker     (121)      540 2021-03-11 20:45:43.000000 pulp-rpm-3.9.1/COPYRIGHT
+-rw-r--r--   0 runner    (1001) docker     (121)    17988 2021-03-11 20:45:43.000000 pulp-rpm-3.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)      320 2021-03-11 20:45:43.000000 pulp-rpm-3.9.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     2686 2021-03-11 20:51:13.000000 pulp-rpm-3.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1612 2021-03-11 20:45:43.000000 pulp-rpm-3.9.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     5692 2021-03-11 20:45:43.000000 pulp-rpm-3.9.1/coverage.md
+-rw-r--r--   0 runner    (1001) docker     (121)      175 2021-03-11 20:45:43.000000 pulp-rpm-3.9.1/functest_requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-11 20:51:13.000000 pulp-rpm-3.9.1/pulp_rpm/
+-rw-r--r--   0 runner    (1001) docker     (121)       59 2021-03-11 20:45:43.000000 pulp-rpm-3.9.1/pulp_rpm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-11 20:51:13.000000 pulp-rpm-3.9.1/pulp_rpm/app/
+-rw-r--r--   0 runner    (1001) docker     (121)      221 2021-03-11 20:45:43.000000 pulp-rpm-3.9.1/pulp_rpm/app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13477 2021-03-11 20:45:43.000000 pulp-rpm-3.9.1/pulp_rpm/app/advisory.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1364 2021-03-11 20:45:43.000000 pulp-rpm-3.9.1/pulp_rpm/app/comps.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6531 2021-03-11 20:45:43.000000 pulp-rpm-3.9.1/pulp_rpm/app/constants.py
+-rw-r--r--   0 runner    (1001) docker     (121)    36032 2021-03-11 20:45:43.000000 pulp-rpm-3.9.1/pulp_rpm/app/depsolving.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3228 2021-03-11 20:45:43.000000 pulp-rpm-3.9.1/pulp_rpm/app/downloaders.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1071 2021-03-11 20:45:43.000000 pulp-rpm-3.9.1/pulp_rpm/app/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2384 2021-03-11 20:45:43.000000 pulp-rpm-3.9.1/pulp_rpm/app/fields.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-11 20:51:13.000000 pulp-rpm-3.9.1/pulp_rpm/app/kickstart/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-03-11 20:45:43.000000 pulp-rpm-3.9.1/pulp_rpm/app/kickstart/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12758 2021-03-11 20:45:43.000000 pulp-rpm-3.9.1/pulp_rpm/app/kickstart/treeinfo.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-11 20:51:13.000000 pulp-rpm-3.9.1/pulp_rpm/app/migrations/
+-rw-r--r--   0 runner    (1001) docker     (121)    23255 2021-03-11 20:45:43.000000 pulp-rpm-3.9.1/pulp_rpm/app/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (121)      388 2021-03-11 20:45:43.000000 pulp-rpm-3.9.1/pulp_rpm/app/migrations/0002_updaterecord_reboot_suggested.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2676 2021-03-11 20:45:43.000000 pulp-rpm-3.9.1/pulp_rpm/app/migrations/0003_DATA_incorrect_json.py
+-rw-r--r--   0 runner    (1001) docker     (121)      609 2021-03-11 20:45:43.000000 pulp-rpm-3.9.1/pulp_rpm/app/migrations/0004_add_metadata_signing_service_fk.py
+-rw-r--r--   0 runner    (1001) docker     (121)      954 2021-03-11 20:45:43.000000 pulp-rpm-3.9.1/pulp_rpm/app/migrations/0005_optimize_sync.py
+-rw-r--r--   0 runner    (1001) docker     (121)      908 2021-03-11 20:45:43.000000 pulp-rpm-3.9.1/pulp_rpm/app/migrations/0006_opensuse_support.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1281 2021-03-11 20:45:43.000000 pulp-rpm-3.9.1/pulp_rpm/app/migrations/0007_checksum_types.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1532 2021-03-11 20:45:43.000000 pulp-rpm-3.9.1/pulp_rpm/app/migrations/0008_advisory_pkg_sumtype_as_int.py
+-rw-r--r--   0 runner    (1001) docker     (121)      429 2021-03-11 20:45:43.000000 pulp-rpm-3.9.1/pulp_rpm/app/migrations/0009_revision_null.py
+-rw-r--r--   0 runner    (1001) docker     (121)      415 2021-03-11 20:45:43.000000 pulp-rpm-3.9.1/pulp_rpm/app/migrations/0010_revision_null_redo.py
+-rw-r--r--   0 runner    (1001) docker     (121)      405 2021-03-11 20:45:43.000000 pulp-rpm-3.9.1/pulp_rpm/app/migrations/0011_rpmremote_sles_auth_token.py
+-rw-r--r--   0 runner    (1001) docker     (121)      712 2021-03-11 20:45:43.000000 pulp-rpm-3.9.1/pulp_rpm/app/migrations/0012_remove_pkg_group_env_cat_related_pkgs.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4734 2021-03-11 20:45:43.000000 pulp-rpm-3.9.1/pulp_rpm/app/migrations/0013_RAW_rpm_evr_extension.py
+-rw-r--r--   0 runner    (1001) docker     (121)      415 2021-03-11 20:45:43.000000 pulp-rpm-3.9.1/pulp_rpm/app/migrations/0014_rpmrepository_package_retention_policy.py
+-rw-r--r--   0 runner    (1001) docker     (121)      932 2021-03-11 20:45:43.000000 pulp-rpm-3.9.1/pulp_rpm/app/migrations/0015_repo_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (121)      882 2021-03-11 20:45:43.000000 pulp-rpm-3.9.1/pulp_rpm/app/migrations/0016_dist_tree_nofk.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1937 2021-03-11 20:45:43.000000 pulp-rpm-3.9.1/pulp_rpm/app/migrations/0017_merge_advisory_collections.py
+-rw-r--r--   0 runner    (1001) docker     (121)      546 2021-03-11 20:45:43.000000 pulp-rpm-3.9.1/pulp_rpm/app/migrations/0018_updatecollection__update_record.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2630 2021-03-11 20:45:43.000000 pulp-rpm-3.9.1/pulp_rpm/app/migrations/0019_migrate_updatecollection_data.py
+-rw-r--r--   0 runner    (1001) docker     (121)      353 2021-03-11 20:45:43.000000 pulp-rpm-3.9.1/pulp_rpm/app/migrations/0020_remove_updatecollection_m2m.py
+-rw-r--r--   0 runner    (1001) docker     (121)      435 2021-03-11 20:45:43.000000 pulp-rpm-3.9.1/pulp_rpm/app/migrations/0021_rename_updatecollection_update_record.py
+-rw-r--r--   0 runner    (1001) docker     (121)      679 2021-03-11 20:45:43.000000 pulp-rpm-3.9.1/pulp_rpm/app/migrations/0022_add_collections_related_name.py
+-rw-r--r--   0 runner    (1001) docker     (121)      746 2021-03-11 20:45:43.000000 pulp-rpm-3.9.1/pulp_rpm/app/migrations/0023_increase_distribution_release_short.py
+-rw-r--r--   0 runner    (1001) docker     (121)      527 2021-03-11 20:45:43.000000 pulp-rpm-3.9.1/pulp_rpm/app/migrations/0024_change_subrepo_relation_properties.py
+-rw-r--r--   0 runner    (1001) docker     (121)      505 2021-03-11 20:45:43.000000 pulp-rpm-3.9.1/pulp_rpm/app/migrations/0025_remove_orphaned_subrepos.py
+-rw-r--r--   0 runner    (1001) docker     (121)      613 2021-03-11 20:45:43.000000 pulp-rpm-3.9.1/pulp_rpm/app/migrations/0026_add_gpgcheck_options.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1510 2021-03-11 20:45:43.000000 pulp-rpm-3.9.1/pulp_rpm/app/migrations/0027_checksum_null.py
+-rw-r--r--   0 runner    (1001) docker     (121)      413 2021-03-11 20:45:43.000000 pulp-rpm-3.9.1/pulp_rpm/app/migrations/0028_rpmrepository_last_sync_repomd_cheksum.py
+-rw-r--r--   0 runner    (1001) docker     (121)      607 2021-03-11 20:45:43.000000 pulp-rpm-3.9.1/pulp_rpm/app/migrations/0029_rpmpublication_sqlite_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (121)      933 2021-03-11 20:45:43.000000 pulp-rpm-3.9.1/pulp_rpm/app/migrations/0030_DATA_fix_updaterecord.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-03-11 20:45:43.000000 pulp-rpm-3.9.1/pulp_rpm/app/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14679 2021-03-11 20:45:43.000000 pulp-rpm-3.9.1/pulp_rpm/app/modelresource.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-11 20:51:13.000000 pulp-rpm-3.9.1/pulp_rpm/app/models/
+-rw-r--r--   0 runner    (1001) docker     (121)      541 2021-03-11 20:45:43.000000 pulp-rpm-3.9.1/pulp_rpm/app/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    18288 2021-03-11 20:45:43.000000 pulp-rpm-3.9.1/pulp_rpm/app/models/advisory.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15139 2021-03-11 20:45:43.000000 pulp-rpm-3.9.1/pulp_rpm/app/models/comps.py
+-rw-r--r--   0 runner    (1001) docker     (121)      838 2021-03-11 20:45:43.000000 pulp-rpm-3.9.1/pulp_rpm/app/models/custom_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9872 2021-03-11 20:45:43.000000 pulp-rpm-3.9.1/pulp_rpm/app/models/distribution.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2462 2021-03-11 20:45:43.000000 pulp-rpm-3.9.1/pulp_rpm/app/models/modulemd.py
+-rw-r--r--   0 runner    (1001) docker     (121)    17275 2021-03-11 20:45:43.000000 pulp-rpm-3.9.1/pulp_rpm/app/models/package.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13590 2021-03-11 20:45:43.000000 pulp-rpm-3.9.1/pulp_rpm/app/models/repository.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5310 2021-03-11 20:45:43.000000 pulp-rpm-3.9.1/pulp_rpm/app/modulemd.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-11 20:51:13.000000 pulp-rpm-3.9.1/pulp_rpm/app/schema/
+-rw-r--r--   0 runner    (1001) docker     (121)      207 2021-03-11 20:45:43.000000 pulp-rpm-3.9.1/pulp_rpm/app/schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      568 2021-03-11 20:45:43.000000 pulp-rpm-3.9.1/pulp_rpm/app/schema/copy_config.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-11 20:51:13.000000 pulp-rpm-3.9.1/pulp_rpm/app/serializers/
+-rw-r--r--   0 runner    (1001) docker     (121)      865 2021-03-11 20:45:43.000000 pulp-rpm-3.9.1/pulp_rpm/app/serializers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9048 2021-03-11 20:45:43.000000 pulp-rpm-3.9.1/pulp_rpm/app/serializers/advisory.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4857 2021-03-11 20:45:43.000000 pulp-rpm-3.9.1/pulp_rpm/app/serializers/comps.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1022 2021-03-11 20:45:43.000000 pulp-rpm-3.9.1/pulp_rpm/app/serializers/custom_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5336 2021-03-11 20:45:43.000000 pulp-rpm-3.9.1/pulp_rpm/app/serializers/distribution.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2688 2021-03-11 20:45:43.000000 pulp-rpm-3.9.1/pulp_rpm/app/serializers/modulemd.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9667 2021-03-11 20:45:43.000000 pulp-rpm-3.9.1/pulp_rpm/app/serializers/package.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6454 2021-03-11 20:45:43.000000 pulp-rpm-3.9.1/pulp_rpm/app/serializers/repository.py
+-rw-r--r--   0 runner    (1001) docker     (121)      212 2021-03-11 20:45:43.000000 pulp-rpm-3.9.1/pulp_rpm/app/settings.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2383 2021-03-11 20:45:43.000000 pulp-rpm-3.9.1/pulp_rpm/app/shared_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-11 20:51:13.000000 pulp-rpm-3.9.1/pulp_rpm/app/tasks/
+-rw-r--r--   0 runner    (1001) docker     (121)      126 2021-03-11 20:45:43.000000 pulp-rpm-3.9.1/pulp_rpm/app/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9122 2021-03-11 20:45:43.000000 pulp-rpm-3.9.1/pulp_rpm/app/tasks/copy.py
+-rw-r--r--   0 runner    (1001) docker     (121)    22308 2021-03-11 20:45:43.000000 pulp-rpm-3.9.1/pulp_rpm/app/tasks/publishing.py
+-rw-r--r--   0 runner    (1001) docker     (121)    43732 2021-03-11 20:45:43.000000 pulp-rpm-3.9.1/pulp_rpm/app/tasks/synchronizing.py
+-rw-r--r--   0 runner    (1001) docker     (121)      159 2021-03-11 20:45:43.000000 pulp-rpm-3.9.1/pulp_rpm/app/urls.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13161 2021-03-11 20:45:43.000000 pulp-rpm-3.9.1/pulp_rpm/app/viewsets.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-11 20:51:13.000000 pulp-rpm-3.9.1/pulp_rpm/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-03-11 20:45:43.000000 pulp-rpm-3.9.1/pulp_rpm/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-11 20:51:13.000000 pulp-rpm-3.9.1/pulp_rpm/tests/functional/
+-rw-r--r--   0 runner    (1001) docker     (121)       44 2021-03-11 20:45:43.000000 pulp-rpm-3.9.1/pulp_rpm/tests/functional/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-11 20:51:13.000000 pulp-rpm-3.9.1/pulp_rpm/tests/functional/api/
+-rw-r--r--   0 runner    (1001) docker     (121)       77 2021-03-11 20:45:43.000000 pulp-rpm-3.9.1/pulp_rpm/tests/functional/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2734 2021-03-11 20:45:43.000000 pulp-rpm-3.9.1/pulp_rpm/tests/functional/api/test_advisory_upload.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2686 2021-03-11 20:45:43.000000 pulp-rpm-3.9.1/pulp_rpm/tests/functional/api/test_character_encoding.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8955 2021-03-11 20:45:43.000000 pulp-rpm-3.9.1/pulp_rpm/tests/functional/api/test_consume_content.py
+-rw-r--r--   0 runner    (1001) docker     (121)    22867 2021-03-11 20:45:43.000000 pulp-rpm-3.9.1/pulp_rpm/tests/functional/api/test_copy.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8729 2021-03-11 20:45:43.000000 pulp-rpm-3.9.1/pulp_rpm/tests/functional/api/test_crud_content_unit.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8037 2021-03-11 20:45:43.000000 pulp-rpm-3.9.1/pulp_rpm/tests/functional/api/test_crud_remotes.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10097 2021-03-11 20:45:43.000000 pulp-rpm-3.9.1/pulp_rpm/tests/functional/api/test_distribution_tree.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4218 2021-03-11 20:45:43.000000 pulp-rpm-3.9.1/pulp_rpm/tests/functional/api/test_download_content.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4281 2021-03-11 20:45:43.000000 pulp-rpm-3.9.1/pulp_rpm/tests/functional/api/test_download_policies.py
+-rw-r--r--   0 runner    (1001) docker     (121)    29808 2021-03-11 20:45:43.000000 pulp-rpm-3.9.1/pulp_rpm/tests/functional/api/test_publish.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4817 2021-03-11 20:45:43.000000 pulp-rpm-3.9.1/pulp_rpm/tests/functional/api/test_pulp_to_pulp.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4683 2021-03-11 20:45:43.000000 pulp-rpm-3.9.1/pulp_rpm/tests/functional/api/test_pulpexport.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8977 2021-03-11 20:45:43.000000 pulp-rpm-3.9.1/pulp_rpm/tests/functional/api/test_pulpimport.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6475 2021-03-11 20:45:43.000000 pulp-rpm-3.9.1/pulp_rpm/tests/functional/api/test_retention_policy.py
+-rw-r--r--   0 runner    (1001) docker     (121)    45871 2021-03-11 20:45:43.000000 pulp-rpm-3.9.1/pulp_rpm/tests/functional/api/test_sync.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2939 2021-03-11 20:45:43.000000 pulp-rpm-3.9.1/pulp_rpm/tests/functional/api/test_upload.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13754 2021-03-11 20:45:43.000000 pulp-rpm-3.9.1/pulp_rpm/tests/functional/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-11 20:51:13.000000 pulp-rpm-3.9.1/pulp_rpm/tests/functional/content_handler/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-03-11 20:45:43.000000 pulp-rpm-3.9.1/pulp_rpm/tests/functional/content_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2740 2021-03-11 20:45:43.000000 pulp-rpm-3.9.1/pulp_rpm/tests/functional/content_handler/test_config_repo.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)      595 2021-03-11 20:45:43.000000 pulp-rpm-3.9.1/pulp_rpm/tests/functional/sign-metadata.sh
+-rw-r--r--   0 runner    (1001) docker     (121)     8971 2021-03-11 20:45:43.000000 pulp-rpm-3.9.1/pulp_rpm/tests/functional/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-11 20:51:13.000000 pulp-rpm-3.9.1/pulp_rpm/tests/performance/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-03-11 20:45:43.000000 pulp-rpm-3.9.1/pulp_rpm/tests/performance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8153 2021-03-11 20:45:43.000000 pulp-rpm-3.9.1/pulp_rpm/tests/performance/test_publish.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5799 2021-03-11 20:45:43.000000 pulp-rpm-3.9.1/pulp_rpm/tests/performance/test_pulp_to_pulp.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11059 2021-03-11 20:45:43.000000 pulp-rpm-3.9.1/pulp_rpm/tests/performance/test_sync.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-11 20:51:13.000000 pulp-rpm-3.9.1/pulp_rpm/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-03-11 20:45:43.000000 pulp-rpm-3.9.1/pulp_rpm/tests/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      229 2021-03-11 20:45:43.000000 pulp-rpm-3.9.1/pulp_rpm/tests/unit/test_models.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-11 20:51:13.000000 pulp-rpm-3.9.1/pulp_rpm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     2686 2021-03-11 20:51:13.000000 pulp-rpm-3.9.1/pulp_rpm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     4750 2021-03-11 20:51:13.000000 pulp-rpm-3.9.1/pulp_rpm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-03-11 20:51:13.000000 pulp-rpm-3.9.1/pulp_rpm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       58 2021-03-11 20:51:13.000000 pulp-rpm-3.9.1/pulp_rpm.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      141 2021-03-11 20:51:13.000000 pulp-rpm-3.9.1/pulp_rpm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        9 2021-03-11 20:51:13.000000 pulp-rpm-3.9.1/pulp_rpm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      859 2021-03-11 20:45:43.000000 pulp-rpm-3.9.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)      141 2021-03-11 20:45:43.000000 pulp-rpm-3.9.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2021-03-11 20:51:13.000000 pulp-rpm-3.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1194 2021-03-11 20:45:43.000000 pulp-rpm-3.9.1/setup.py
+-rw-r--r--   0 runner    (1001) docker     (121)       82 2021-03-11 20:45:43.000000 pulp-rpm-3.9.1/test_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        5 2021-03-11 20:45:43.000000 pulp-rpm-3.9.1/unittest_requirements.txt
```

### Comparing `pulp-rpm-3.9.0/CHANGES.rst` & `pulp-rpm-3.9.1/CHANGES.rst`

 * *Files 0% similar despite different names*

```diff
@@ -9,14 +9,28 @@
     To add a new change log entry, please see
     https://docs.pulpproject.org/contributing/git.html#changelog-update
 
     WARNING: Don't drop the next directive!
 
 .. towncrier release notes start
 
+3.9.1 (2021-03-11)
+==================
+
+
+Bugfixes
+--------
+
+- Fixed DistributionTree parsing for boolean fields which could cause a failure at sync or migration time.
+  `#8374 <https://pulp.plan.io/issues/8374>`_
+
+
+----
+
+
 3.9.0 (2021-02-04)
 ==================
 
 
 Features
 --------
```

### Comparing `pulp-rpm-3.9.0/COMMITMENT` & `pulp-rpm-3.9.1/COMMITMENT`

 * *Files identical despite different names*

### Comparing `pulp-rpm-3.9.0/COPYRIGHT` & `pulp-rpm-3.9.1/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `pulp-rpm-3.9.0/LICENSE` & `pulp-rpm-3.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pulp-rpm-3.9.0/PKG-INFO` & `pulp-rpm-3.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: pulp-rpm
-Version: 3.9.0
+Version: 3.9.1
 Summary: RPM plugin for the Pulp Project
 Home-page: http://www.pulpproject.org
 Author: Pulp Project Developers
 Author-email: pulp-list@redhat.com
 License: GPLv2+
 Description: ``pulp_rpm`` Plugin
         ===================
```

### Comparing `pulp-rpm-3.9.0/README.rst` & `pulp-rpm-3.9.1/README.rst`

 * *Files identical despite different names*

### Comparing `pulp-rpm-3.9.0/coverage.md` & `pulp-rpm-3.9.1/coverage.md`

 * *Files identical despite different names*

### Comparing `pulp-rpm-3.9.0/pulp_rpm/app/advisory.py` & `pulp-rpm-3.9.1/pulp_rpm/app/advisory.py`

 * *Files identical despite different names*

### Comparing `pulp-rpm-3.9.0/pulp_rpm/app/comps.py` & `pulp-rpm-3.9.1/pulp_rpm/app/comps.py`

 * *Files identical despite different names*

### Comparing `pulp-rpm-3.9.0/pulp_rpm/app/constants.py` & `pulp-rpm-3.9.1/pulp_rpm/app/constants.py`

 * *Files identical despite different names*

### Comparing `pulp-rpm-3.9.0/pulp_rpm/app/depsolving.py` & `pulp-rpm-3.9.1/pulp_rpm/app/depsolving.py`

 * *Files identical despite different names*

### Comparing `pulp-rpm-3.9.0/pulp_rpm/app/downloaders.py` & `pulp-rpm-3.9.1/pulp_rpm/app/downloaders.py`

 * *Files identical despite different names*

### Comparing `pulp-rpm-3.9.0/pulp_rpm/app/exceptions.py` & `pulp-rpm-3.9.1/pulp_rpm/app/exceptions.py`

 * *Files identical despite different names*

### Comparing `pulp-rpm-3.9.0/pulp_rpm/app/fields.py` & `pulp-rpm-3.9.1/pulp_rpm/app/fields.py`

 * *Files identical despite different names*

### Comparing `pulp-rpm-3.9.0/pulp_rpm/app/kickstart/treeinfo.py` & `pulp-rpm-3.9.1/pulp_rpm/app/kickstart/treeinfo.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import json
 from gettext import gettext as _
 from configparser import MissingSectionHeaderError
 from urllib.parse import urljoin
 
 from django.utils.timezone import now
 
 from productmd.common import SortedConfigParser
@@ -136,14 +137,19 @@
 
         if build_timestamp and parser._sections.get("general", {}).get("timestamp"):
             parser._sections["general"]["timestamp"] = build_timestamp
 
         if build_timestamp and parser._sections.get("tree", {}).get("build_timestamp"):
             parser._sections["tree"]["build_timestamp"] = build_timestamp
 
+        release = self.original_parser._sections.get("release", {})
+
+        if "is_layered" in release:
+            parser._sections["release"]["is_layered"] = json.loads(release["is_layered"])
+
         return parser._sections
 
 
 class TreeinfoData:
     """
     Treat parsed treeinfo data.
 
@@ -182,20 +188,26 @@
             )
 
         distribution_tree.update(
             {"header_version": self._data.get("header", {}).get("version", "1.2")}
         )
 
         if self._data.get("release"):
+            is_layered = self._data["release"].get("is_layered", False)
+
+            # If we get is_layered, but it's a string - let json turn it into a boolean
+            if is_layered and isinstance(is_layered, str):
+                is_layered = json.loads(is_layered)
+
             distribution_tree.update(
                 {
                     "release_name": self._data["release"]["name"],
                     "release_short": self._data["release"]["short"],
                     "release_version": self._data["release"]["version"],
-                    "release_is_layered": self._data["release"].get("is_layered", False),
+                    "release_is_layered": is_layered,
                 }
             )
 
         if self._data.get("tree"):
             distribution_tree.update(
                 {
                     "arch": self._data["tree"]["arch"],
```

### Comparing `pulp-rpm-3.9.0/pulp_rpm/app/migrations/0001_initial.py` & `pulp-rpm-3.9.1/pulp_rpm/app/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `pulp-rpm-3.9.0/pulp_rpm/app/migrations/0003_DATA_incorrect_json.py` & `pulp-rpm-3.9.1/pulp_rpm/app/migrations/0003_DATA_incorrect_json.py`

 * *Files identical despite different names*

### Comparing `pulp-rpm-3.9.0/pulp_rpm/app/migrations/0004_add_metadata_signing_service_fk.py` & `pulp-rpm-3.9.1/pulp_rpm/app/migrations/0004_add_metadata_signing_service_fk.py`

 * *Files identical despite different names*

### Comparing `pulp-rpm-3.9.0/pulp_rpm/app/migrations/0005_optimize_sync.py` & `pulp-rpm-3.9.1/pulp_rpm/app/migrations/0005_optimize_sync.py`

 * *Files identical despite different names*

### Comparing `pulp-rpm-3.9.0/pulp_rpm/app/migrations/0006_opensuse_support.py` & `pulp-rpm-3.9.1/pulp_rpm/app/migrations/0006_opensuse_support.py`

 * *Files identical despite different names*

### Comparing `pulp-rpm-3.9.0/pulp_rpm/app/migrations/0007_checksum_types.py` & `pulp-rpm-3.9.1/pulp_rpm/app/migrations/0007_checksum_types.py`

 * *Files identical despite different names*

### Comparing `pulp-rpm-3.9.0/pulp_rpm/app/migrations/0008_advisory_pkg_sumtype_as_int.py` & `pulp-rpm-3.9.1/pulp_rpm/app/migrations/0008_advisory_pkg_sumtype_as_int.py`

 * *Files identical despite different names*

### Comparing `pulp-rpm-3.9.0/pulp_rpm/app/migrations/0012_remove_pkg_group_env_cat_related_pkgs.py` & `pulp-rpm-3.9.1/pulp_rpm/app/migrations/0012_remove_pkg_group_env_cat_related_pkgs.py`

 * *Files identical despite different names*

### Comparing `pulp-rpm-3.9.0/pulp_rpm/app/migrations/0013_RAW_rpm_evr_extension.py` & `pulp-rpm-3.9.1/pulp_rpm/app/migrations/0013_RAW_rpm_evr_extension.py`

 * *Files identical despite different names*

### Comparing `pulp-rpm-3.9.0/pulp_rpm/app/migrations/0015_repo_metadata.py` & `pulp-rpm-3.9.1/pulp_rpm/app/migrations/0015_repo_metadata.py`

 * *Files identical despite different names*

### Comparing `pulp-rpm-3.9.0/pulp_rpm/app/migrations/0016_dist_tree_nofk.py` & `pulp-rpm-3.9.1/pulp_rpm/app/migrations/0016_dist_tree_nofk.py`

 * *Files identical despite different names*

### Comparing `pulp-rpm-3.9.0/pulp_rpm/app/migrations/0017_merge_advisory_collections.py` & `pulp-rpm-3.9.1/pulp_rpm/app/migrations/0017_merge_advisory_collections.py`

 * *Files identical despite different names*

### Comparing `pulp-rpm-3.9.0/pulp_rpm/app/migrations/0018_updatecollection__update_record.py` & `pulp-rpm-3.9.1/pulp_rpm/app/migrations/0018_updatecollection__update_record.py`

 * *Files identical despite different names*

### Comparing `pulp-rpm-3.9.0/pulp_rpm/app/migrations/0019_migrate_updatecollection_data.py` & `pulp-rpm-3.9.1/pulp_rpm/app/migrations/0019_migrate_updatecollection_data.py`

 * *Files identical despite different names*

### Comparing `pulp-rpm-3.9.0/pulp_rpm/app/migrations/0022_add_collections_related_name.py` & `pulp-rpm-3.9.1/pulp_rpm/app/migrations/0022_add_collections_related_name.py`

 * *Files identical despite different names*

### Comparing `pulp-rpm-3.9.0/pulp_rpm/app/migrations/0023_increase_distribution_release_short.py` & `pulp-rpm-3.9.1/pulp_rpm/app/migrations/0023_increase_distribution_release_short.py`

 * *Files identical despite different names*

### Comparing `pulp-rpm-3.9.0/pulp_rpm/app/migrations/0024_change_subrepo_relation_properties.py` & `pulp-rpm-3.9.1/pulp_rpm/app/migrations/0024_change_subrepo_relation_properties.py`

 * *Files identical despite different names*

### Comparing `pulp-rpm-3.9.0/pulp_rpm/app/migrations/0026_add_gpgcheck_options.py` & `pulp-rpm-3.9.1/pulp_rpm/app/migrations/0026_add_gpgcheck_options.py`

 * *Files identical despite different names*

### Comparing `pulp-rpm-3.9.0/pulp_rpm/app/migrations/0027_checksum_null.py` & `pulp-rpm-3.9.1/pulp_rpm/app/migrations/0027_checksum_null.py`

 * *Files identical despite different names*

### Comparing `pulp-rpm-3.9.0/pulp_rpm/app/migrations/0029_rpmpublication_sqlite_metadata.py` & `pulp-rpm-3.9.1/pulp_rpm/app/migrations/0029_rpmpublication_sqlite_metadata.py`

 * *Files identical despite different names*

### Comparing `pulp-rpm-3.9.0/pulp_rpm/app/migrations/0030_DATA_fix_updaterecord.py` & `pulp-rpm-3.9.1/pulp_rpm/app/migrations/0030_DATA_fix_updaterecord.py`

 * *Files identical despite different names*

### Comparing `pulp-rpm-3.9.0/pulp_rpm/app/modelresource.py` & `pulp-rpm-3.9.1/pulp_rpm/app/modelresource.py`

 * *Files identical despite different names*

### Comparing `pulp-rpm-3.9.0/pulp_rpm/app/models/__init__.py` & `pulp-rpm-3.9.1/pulp_rpm/app/models/__init__.py`

 * *Files identical despite different names*

### Comparing `pulp-rpm-3.9.0/pulp_rpm/app/models/advisory.py` & `pulp-rpm-3.9.1/pulp_rpm/app/models/advisory.py`

 * *Files identical despite different names*

### Comparing `pulp-rpm-3.9.0/pulp_rpm/app/models/comps.py` & `pulp-rpm-3.9.1/pulp_rpm/app/models/comps.py`

 * *Files identical despite different names*

### Comparing `pulp-rpm-3.9.0/pulp_rpm/app/models/custom_metadata.py` & `pulp-rpm-3.9.1/pulp_rpm/app/models/custom_metadata.py`

 * *Files identical despite different names*

### Comparing `pulp-rpm-3.9.0/pulp_rpm/app/models/distribution.py` & `pulp-rpm-3.9.1/pulp_rpm/app/models/distribution.py`

 * *Files identical despite different names*

### Comparing `pulp-rpm-3.9.0/pulp_rpm/app/models/modulemd.py` & `pulp-rpm-3.9.1/pulp_rpm/app/models/modulemd.py`

 * *Files identical despite different names*

### Comparing `pulp-rpm-3.9.0/pulp_rpm/app/models/package.py` & `pulp-rpm-3.9.1/pulp_rpm/app/models/package.py`

 * *Files identical despite different names*

### Comparing `pulp-rpm-3.9.0/pulp_rpm/app/models/repository.py` & `pulp-rpm-3.9.1/pulp_rpm/app/models/repository.py`

 * *Files identical despite different names*

### Comparing `pulp-rpm-3.9.0/pulp_rpm/app/modulemd.py` & `pulp-rpm-3.9.1/pulp_rpm/app/modulemd.py`

 * *Files identical despite different names*

### Comparing `pulp-rpm-3.9.0/pulp_rpm/app/schema/copy_config.json` & `pulp-rpm-3.9.1/pulp_rpm/app/schema/copy_config.json`

 * *Files identical despite different names*

### Comparing `pulp-rpm-3.9.0/pulp_rpm/app/serializers/__init__.py` & `pulp-rpm-3.9.1/pulp_rpm/app/serializers/__init__.py`

 * *Files identical despite different names*

### Comparing `pulp-rpm-3.9.0/pulp_rpm/app/serializers/advisory.py` & `pulp-rpm-3.9.1/pulp_rpm/app/serializers/advisory.py`

 * *Files identical despite different names*

### Comparing `pulp-rpm-3.9.0/pulp_rpm/app/serializers/comps.py` & `pulp-rpm-3.9.1/pulp_rpm/app/serializers/comps.py`

 * *Files identical despite different names*

### Comparing `pulp-rpm-3.9.0/pulp_rpm/app/serializers/custom_metadata.py` & `pulp-rpm-3.9.1/pulp_rpm/app/serializers/custom_metadata.py`

 * *Files identical despite different names*

### Comparing `pulp-rpm-3.9.0/pulp_rpm/app/serializers/distribution.py` & `pulp-rpm-3.9.1/pulp_rpm/app/serializers/distribution.py`

 * *Files identical despite different names*

### Comparing `pulp-rpm-3.9.0/pulp_rpm/app/serializers/modulemd.py` & `pulp-rpm-3.9.1/pulp_rpm/app/serializers/modulemd.py`

 * *Files identical despite different names*

### Comparing `pulp-rpm-3.9.0/pulp_rpm/app/serializers/package.py` & `pulp-rpm-3.9.1/pulp_rpm/app/serializers/package.py`

 * *Files identical despite different names*

### Comparing `pulp-rpm-3.9.0/pulp_rpm/app/serializers/repository.py` & `pulp-rpm-3.9.1/pulp_rpm/app/serializers/repository.py`

 * *Files identical despite different names*

### Comparing `pulp-rpm-3.9.0/pulp_rpm/app/shared_utils.py` & `pulp-rpm-3.9.1/pulp_rpm/app/shared_utils.py`

 * *Files identical despite different names*

### Comparing `pulp-rpm-3.9.0/pulp_rpm/app/tasks/copy.py` & `pulp-rpm-3.9.1/pulp_rpm/app/tasks/copy.py`

 * *Files identical despite different names*

### Comparing `pulp-rpm-3.9.0/pulp_rpm/app/tasks/publishing.py` & `pulp-rpm-3.9.1/pulp_rpm/app/tasks/publishing.py`

 * *Files identical despite different names*

### Comparing `pulp-rpm-3.9.0/pulp_rpm/app/tasks/synchronizing.py` & `pulp-rpm-3.9.1/pulp_rpm/app/tasks/synchronizing.py`

 * *Files 0% similar despite different names*

```diff
@@ -547,15 +547,15 @@
 
         while pending:
             done, pending = await asyncio.wait(pending, return_when=asyncio.FIRST_COMPLETED)
             for downloader in done:
                 try:
                     results = downloader.result()
                 except ClientResponseError as exc:
-                    raise HTTPNotFound(reason=_(f"File not found: {exc.request_info.url}"))
+                    raise HTTPNotFound(reason=_("File not found: {}".format(exc.request_info.url)))
                 else:
                     data_url = results[0].url
                     await data_type_handlers[data_url](results)
 
     async def parse_packages(self, results):
         """Parse packages from the remote repository."""
         primary_xml_path = results[0].path
```

### Comparing `pulp-rpm-3.9.0/pulp_rpm/app/viewsets.py` & `pulp-rpm-3.9.1/pulp_rpm/app/viewsets.py`

 * *Files identical despite different names*

### Comparing `pulp-rpm-3.9.0/pulp_rpm/tests/functional/api/test_advisory_upload.py` & `pulp-rpm-3.9.1/pulp_rpm/tests/functional/api/test_advisory_upload.py`

 * *Files identical despite different names*

### Comparing `pulp-rpm-3.9.0/pulp_rpm/tests/functional/api/test_character_encoding.py` & `pulp-rpm-3.9.1/pulp_rpm/tests/functional/api/test_character_encoding.py`

 * *Files identical despite different names*

### Comparing `pulp-rpm-3.9.0/pulp_rpm/tests/functional/api/test_consume_content.py` & `pulp-rpm-3.9.1/pulp_rpm/tests/functional/api/test_consume_content.py`

 * *Files identical despite different names*

### Comparing `pulp-rpm-3.9.0/pulp_rpm/tests/functional/api/test_copy.py` & `pulp-rpm-3.9.1/pulp_rpm/tests/functional/api/test_copy.py`

 * *Files identical despite different names*

### Comparing `pulp-rpm-3.9.0/pulp_rpm/tests/functional/api/test_crud_content_unit.py` & `pulp-rpm-3.9.1/pulp_rpm/tests/functional/api/test_crud_content_unit.py`

 * *Files identical despite different names*

### Comparing `pulp-rpm-3.9.0/pulp_rpm/tests/functional/api/test_crud_remotes.py` & `pulp-rpm-3.9.1/pulp_rpm/tests/functional/api/test_crud_remotes.py`

 * *Files identical despite different names*

### Comparing `pulp-rpm-3.9.0/pulp_rpm/tests/functional/api/test_distribution_tree.py` & `pulp-rpm-3.9.1/pulp_rpm/tests/functional/api/test_distribution_tree.py`

 * *Files identical despite different names*

### Comparing `pulp-rpm-3.9.0/pulp_rpm/tests/functional/api/test_download_content.py` & `pulp-rpm-3.9.1/pulp_rpm/tests/functional/api/test_download_content.py`

 * *Files identical despite different names*

### Comparing `pulp-rpm-3.9.0/pulp_rpm/tests/functional/api/test_download_policies.py` & `pulp-rpm-3.9.1/pulp_rpm/tests/functional/api/test_download_policies.py`

 * *Files identical despite different names*

### Comparing `pulp-rpm-3.9.0/pulp_rpm/tests/functional/api/test_publish.py` & `pulp-rpm-3.9.1/pulp_rpm/tests/functional/api/test_publish.py`

 * *Files identical despite different names*

### Comparing `pulp-rpm-3.9.0/pulp_rpm/tests/functional/api/test_pulp_to_pulp.py` & `pulp-rpm-3.9.1/pulp_rpm/tests/functional/api/test_pulp_to_pulp.py`

 * *Files identical despite different names*

### Comparing `pulp-rpm-3.9.0/pulp_rpm/tests/functional/api/test_pulpexport.py` & `pulp-rpm-3.9.1/pulp_rpm/tests/functional/api/test_pulpexport.py`

 * *Files identical despite different names*

### Comparing `pulp-rpm-3.9.0/pulp_rpm/tests/functional/api/test_pulpimport.py` & `pulp-rpm-3.9.1/pulp_rpm/tests/functional/api/test_pulpimport.py`

 * *Files identical despite different names*

### Comparing `pulp-rpm-3.9.0/pulp_rpm/tests/functional/api/test_retention_policy.py` & `pulp-rpm-3.9.1/pulp_rpm/tests/functional/api/test_retention_policy.py`

 * *Files identical despite different names*

### Comparing `pulp-rpm-3.9.0/pulp_rpm/tests/functional/api/test_sync.py` & `pulp-rpm-3.9.1/pulp_rpm/tests/functional/api/test_sync.py`

 * *Files identical despite different names*

### Comparing `pulp-rpm-3.9.0/pulp_rpm/tests/functional/api/test_upload.py` & `pulp-rpm-3.9.1/pulp_rpm/tests/functional/api/test_upload.py`

 * *Files identical despite different names*

### Comparing `pulp-rpm-3.9.0/pulp_rpm/tests/functional/constants.py` & `pulp-rpm-3.9.1/pulp_rpm/tests/functional/constants.py`

 * *Files identical despite different names*

### Comparing `pulp-rpm-3.9.0/pulp_rpm/tests/functional/content_handler/test_config_repo.py` & `pulp-rpm-3.9.1/pulp_rpm/tests/functional/content_handler/test_config_repo.py`

 * *Files identical despite different names*

### Comparing `pulp-rpm-3.9.0/pulp_rpm/tests/functional/sign-metadata.sh` & `pulp-rpm-3.9.1/pulp_rpm/tests/functional/sign-metadata.sh`

 * *Files identical despite different names*

### Comparing `pulp-rpm-3.9.0/pulp_rpm/tests/functional/utils.py` & `pulp-rpm-3.9.1/pulp_rpm/tests/functional/utils.py`

 * *Files identical despite different names*

### Comparing `pulp-rpm-3.9.0/pulp_rpm/tests/performance/test_publish.py` & `pulp-rpm-3.9.1/pulp_rpm/tests/performance/test_publish.py`

 * *Files identical despite different names*

### Comparing `pulp-rpm-3.9.0/pulp_rpm/tests/performance/test_pulp_to_pulp.py` & `pulp-rpm-3.9.1/pulp_rpm/tests/performance/test_pulp_to_pulp.py`

 * *Files identical despite different names*

### Comparing `pulp-rpm-3.9.0/pulp_rpm/tests/performance/test_sync.py` & `pulp-rpm-3.9.1/pulp_rpm/tests/performance/test_sync.py`

 * *Files identical despite different names*

### Comparing `pulp-rpm-3.9.0/pulp_rpm.egg-info/PKG-INFO` & `pulp-rpm-3.9.1/pulp_rpm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: pulp-rpm
-Version: 3.9.0
+Version: 3.9.1
 Summary: RPM plugin for the Pulp Project
 Home-page: http://www.pulpproject.org
 Author: Pulp Project Developers
 Author-email: pulp-list@redhat.com
 License: GPLv2+
 Description: ``pulp_rpm`` Plugin
         ===================
```

### Comparing `pulp-rpm-3.9.0/pulp_rpm.egg-info/SOURCES.txt` & `pulp-rpm-3.9.1/pulp_rpm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulp-rpm-3.9.0/pyproject.toml` & `pulp-rpm-3.9.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pulp-rpm-3.9.0/setup.py` & `pulp-rpm-3.9.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     requirements = requirements.readlines()
 
 with open("README.rst") as f:
     long_description = f.read()
 
 setup(
     name="pulp-rpm",
-    version="3.9.0",
+    version="3.9.1",
     description="RPM plugin for the Pulp Project",
     long_description=long_description,
     license="GPLv2+",
     author="Pulp Project Developers",
     author_email="pulp-list@redhat.com",
     url="http://www.pulpproject.org",
     python_requires=">=3.6",
```

