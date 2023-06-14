# Comparing `tmp/xpanse-1.3.1.tar.gz` & `tmp/xpanse-2.0.0rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xpanse-1.3.1.tar", last modified: Mon May  2 21:04:36 2022, max compression
+gzip compressed data, was "xpanse-2.0.0rc3.tar", last modified: Tue May 30 19:38:20 2023, max compression
```

## Comparing `xpanse-1.3.1.tar` & `xpanse-2.0.0rc3.tar`

### file list

```diff
@@ -1,126 +1,80 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-02 21:04:36.698585 xpanse-1.3.1/
--rw-r--r--   0 runner    (1001) docker     (121)      754 2022-05-02 21:04:04.000000 xpanse-1.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      163 2022-05-02 21:04:04.000000 xpanse-1.3.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     3775 2022-05-02 21:04:36.698585 xpanse-1.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2975 2022-05-02 21:04:04.000000 xpanse-1.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-02 21:04:36.690585 xpanse-1.3.1/docs/
--rw-r--r--   0 runner    (1001) docker     (121)      640 2022-05-02 21:04:04.000000 xpanse-1.3.1/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (121)      459 2022-05-02 21:04:04.000000 xpanse-1.3.1/docs/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-02 21:04:36.690585 xpanse-1.3.1/docs/_source/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-02 21:04:36.690585 xpanse-1.3.1/docs/_source/_static/
--rw-r--r--   0 runner    (1001) docker     (121)     8940 2022-05-02 21:04:04.000000 xpanse-1.3.1/docs/_source/_static/expanse.png
--rw-r--r--   0 runner    (1001) docker     (121)    22679 2022-05-02 21:04:04.000000 xpanse-1.3.1/docs/_source/_static/expanse_banner.png
--rw-r--r--   0 runner    (1001) docker     (121)    17992 2022-05-02 21:04:04.000000 xpanse-1.3.1/docs/_source/_static/xpanse_banner.png
--rw-r--r--   0 runner    (1001) docker     (121)     3533 2022-05-02 21:04:04.000000 xpanse-1.3.1/docs/_source/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)     2009 2022-05-02 21:04:04.000000 xpanse-1.3.1/docs/_source/cover.rst
--rw-r--r--   0 runner    (1001) docker     (121)      264 2022-05-02 21:04:04.000000 xpanse-1.3.1/docs/_source/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)       55 2022-05-02 21:04:04.000000 xpanse-1.3.1/docs/_source/modules.rst
--rw-r--r--   0 runner    (1001) docker     (121)      229 2022-05-02 21:04:04.000000 xpanse-1.3.1/docs/_source/xpanse.api.annotations.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2546 2022-05-02 21:04:04.000000 xpanse-1.3.1/docs/_source/xpanse.api.assets.rst
--rw-r--r--   0 runner    (1001) docker     (121)      235 2022-05-02 21:04:04.000000 xpanse-1.3.1/docs/_source/xpanse.api.behavior.rst
--rw-r--r--   0 runner    (1001) docker     (121)      443 2022-05-02 21:04:04.000000 xpanse-1.3.1/docs/_source/xpanse.api.connectors.rst
--rw-r--r--   0 runner    (1001) docker     (121)      226 2022-05-02 21:04:04.000000 xpanse-1.3.1/docs/_source/xpanse.api.entities.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1140 2022-05-02 21:04:04.000000 xpanse-1.3.1/docs/_source/xpanse.api.issues.rst
--rw-r--r--   0 runner    (1001) docker     (121)      897 2022-05-02 21:04:04.000000 xpanse-1.3.1/docs/_source/xpanse.api.rst
--rw-r--r--   0 runner    (1001) docker     (121)      635 2022-05-02 21:04:04.000000 xpanse-1.3.1/docs/_source/xpanse.api.services.rst
--rw-r--r--   0 runner    (1001) docker     (121)      258 2022-05-02 21:04:04.000000 xpanse-1.3.1/docs/_source/xpanse.api.targeted_ips.rst
--rw-r--r--   0 runner    (1001) docker     (121)      875 2022-05-02 21:04:04.000000 xpanse-1.3.1/docs/_source/xpanse.rst
--rw-r--r--   0 runner    (1001) docker     (121)      620 2022-05-02 21:04:04.000000 xpanse-1.3.1/docs/requirements-docs.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-02 21:04:36.690585 xpanse-1.3.1/examples/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-02 21:04:36.690585 xpanse-1.3.1/examples/behavior_writer/
--rw-r--r--   0 runner    (1001) docker     (121)      524 2022-05-02 21:04:04.000000 xpanse-1.3.1/examples/behavior_writer/README.md
--rw-r--r--   0 runner    (1001) docker     (121)     2886 2022-05-02 21:04:04.000000 xpanse-1.3.1/examples/behavior_writer/export_behavior_to_csv.py
--rw-r--r--   0 runner    (1001) docker     (121)       26 2022-05-02 21:04:04.000000 xpanse-1.3.1/examples/behavior_writer/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-02 21:04:36.690585 xpanse-1.3.1/examples/bulk_issues_update/
--rw-r--r--   0 runner    (1001) docker     (121)      639 2022-05-02 21:04:04.000000 xpanse-1.3.1/examples/bulk_issues_update/README.md
--rw-r--r--   0 runner    (1001) docker     (121)     2586 2022-05-02 21:04:04.000000 xpanse-1.3.1/examples/bulk_issues_update/bulk_issues_update.py
--rw-r--r--   0 runner    (1001) docker     (121)       26 2022-05-02 21:04:04.000000 xpanse-1.3.1/examples/bulk_issues_update/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-02 21:04:36.690585 xpanse-1.3.1/examples/bulk_tagger/
--rw-r--r--   0 runner    (1001) docker     (121)      775 2022-05-02 21:04:04.000000 xpanse-1.3.1/examples/bulk_tagger/README.md
--rw-r--r--   0 runner    (1001) docker     (121)     2739 2022-05-02 21:04:04.000000 xpanse-1.3.1/examples/bulk_tagger/bulk_tagger.py
--rw-r--r--   0 runner    (1001) docker     (121)       26 2022-05-02 21:04:04.000000 xpanse-1.3.1/examples/bulk_tagger/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-02 21:04:36.694585 xpanse-1.3.1/examples/ip_range_writer/
--rw-r--r--   0 runner    (1001) docker     (121)      600 2022-05-02 21:04:04.000000 xpanse-1.3.1/examples/ip_range_writer/README.md
--rw-r--r--   0 runner    (1001) docker     (121)     3515 2022-05-02 21:04:04.000000 xpanse-1.3.1/examples/ip_range_writer/ip_range.py
--rw-r--r--   0 runner    (1001) docker     (121)       26 2022-05-02 21:04:04.000000 xpanse-1.3.1/examples/ip_range_writer/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-05-02 21:04:36.698585 xpanse-1.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1336 2022-05-02 21:04:04.000000 xpanse-1.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-02 21:04:36.694585 xpanse-1.3.1/xpanse/
--rw-r--r--   0 runner    (1001) docker     (121)      205 2022-05-02 21:04:04.000000 xpanse-1.3.1/xpanse/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-02 21:04:36.694585 xpanse-1.3.1/xpanse/api/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-02 21:04:04.000000 xpanse-1.3.1/xpanse/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-02 21:04:36.694585 xpanse-1.3.1/xpanse/api/annotations/
--rw-r--r--   0 runner    (1001) docker     (121)      432 2022-05-02 21:04:04.000000 xpanse-1.3.1/xpanse/api/annotations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-02 21:04:36.694585 xpanse-1.3.1/xpanse/api/annotations/v3/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-02 21:04:04.000000 xpanse-1.3.1/xpanse/api/annotations/v3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3858 2022-05-02 21:04:04.000000 xpanse-1.3.1/xpanse/api/annotations/v3/tags.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-02 21:04:36.694585 xpanse-1.3.1/xpanse/api/assets/
--rw-r--r--   0 runner    (1001) docker     (121)     5515 2022-05-02 21:04:04.000000 xpanse-1.3.1/xpanse/api/assets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-02 21:04:36.694585 xpanse-1.3.1/xpanse/api/assets/v2/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-02 21:04:04.000000 xpanse-1.3.1/xpanse/api/assets/v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1412 2022-05-02 21:04:04.000000 xpanse-1.3.1/xpanse/api/assets/v2/account_integrations.py
--rw-r--r--   0 runner    (1001) docker     (121)     7608 2022-05-02 21:04:04.000000 xpanse-1.3.1/xpanse/api/assets/v2/annotations.py
--rw-r--r--   0 runner    (1001) docker     (121)     1372 2022-05-02 21:04:04.000000 xpanse-1.3.1/xpanse/api/assets/v2/certificate_issuers.py
--rw-r--r--   0 runner    (1001) docker     (121)     1393 2022-05-02 21:04:04.000000 xpanse-1.3.1/xpanse/api/assets/v2/certificate_properties.py
--rw-r--r--   0 runner    (1001) docker     (121)    19797 2022-05-02 21:04:04.000000 xpanse-1.3.1/xpanse/api/assets/v2/certificates.py
--rw-r--r--   0 runner    (1001) docker     (121)    19024 2022-05-02 21:04:04.000000 xpanse-1.3.1/xpanse/api/assets/v2/cloud_resources.py
--rw-r--r--   0 runner    (1001) docker     (121)     1358 2022-05-02 21:04:04.000000 xpanse-1.3.1/xpanse/api/assets/v2/domain_registrars.py
--rw-r--r--   0 runner    (1001) docker     (121)    19722 2022-05-02 21:04:04.000000 xpanse-1.3.1/xpanse/api/assets/v2/domains.py
--rw-r--r--   0 runner    (1001) docker     (121)     1288 2022-05-02 21:04:04.000000 xpanse-1.3.1/xpanse/api/assets/v2/entities.py
--rw-r--r--   0 runner    (1001) docker     (121)     9512 2022-05-02 21:04:04.000000 xpanse-1.3.1/xpanse/api/assets/v2/ip_range.py
--rw-r--r--   0 runner    (1001) docker     (121)     4910 2022-05-02 21:04:04.000000 xpanse-1.3.1/xpanse/api/assets/v2/ips.py
--rw-r--r--   0 runner    (1001) docker     (121)     1298 2022-05-02 21:04:04.000000 xpanse-1.3.1/xpanse/api/assets/v2/providers.py
--rw-r--r--   0 runner    (1001) docker     (121)     1276 2022-05-02 21:04:04.000000 xpanse-1.3.1/xpanse/api/assets/v2/regions.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-02 21:04:36.694585 xpanse-1.3.1/xpanse/api/behavior/
--rw-r--r--   0 runner    (1001) docker     (121)      872 2022-05-02 21:04:04.000000 xpanse-1.3.1/xpanse/api/behavior/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-02 21:04:36.694585 xpanse-1.3.1/xpanse/api/behavior/v1/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-02 21:04:04.000000 xpanse-1.3.1/xpanse/api/behavior/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1939 2022-05-02 21:04:04.000000 xpanse-1.3.1/xpanse/api/behavior/v1/risk_rules.py
--rw-r--r--   0 runner    (1001) docker     (121)     3668 2022-05-02 21:04:04.000000 xpanse-1.3.1/xpanse/api/behavior/v1/risky_flows.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-02 21:04:36.694585 xpanse-1.3.1/xpanse/api/connectors/
--rw-r--r--   0 runner    (1001) docker     (121)      953 2022-05-02 21:04:04.000000 xpanse-1.3.1/xpanse/api/connectors/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-02 21:04:36.694585 xpanse-1.3.1/xpanse/api/connectors/v1/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-02 21:04:04.000000 xpanse-1.3.1/xpanse/api/connectors/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1866 2022-05-02 21:04:04.000000 xpanse-1.3.1/xpanse/api/connectors/v1/accounts.py
--rw-r--r--   0 runner    (1001) docker     (121)     1174 2022-05-02 21:04:04.000000 xpanse-1.3.1/xpanse/api/connectors/v1/services.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-02 21:04:36.698585 xpanse-1.3.1/xpanse/api/entities/
--rw-r--r--   0 runner    (1001) docker     (121)      464 2022-05-02 21:04:04.000000 xpanse-1.3.1/xpanse/api/entities/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-02 21:04:36.698585 xpanse-1.3.1/xpanse/api/entities/v1/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-02 21:04:04.000000 xpanse-1.3.1/xpanse/api/entities/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2841 2022-05-02 21:04:04.000000 xpanse-1.3.1/xpanse/api/entities/v1/entities.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-02 21:04:36.698585 xpanse-1.3.1/xpanse/api/issues/
--rw-r--r--   0 runner    (1001) docker     (121)     2926 2022-05-02 21:04:04.000000 xpanse-1.3.1/xpanse/api/issues/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-02 21:04:36.698585 xpanse-1.3.1/xpanse/api/issues/v1/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-02 21:04:04.000000 xpanse-1.3.1/xpanse/api/issues/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1135 2022-05-02 21:04:04.000000 xpanse-1.3.1/xpanse/api/issues/v1/assignees.py
--rw-r--r--   0 runner    (1001) docker     (121)     1160 2022-05-02 21:04:04.000000 xpanse-1.3.1/xpanse/api/issues/v1/business_units.py
--rw-r--r--   0 runner    (1001) docker     (121)     1121 2022-05-02 21:04:04.000000 xpanse-1.3.1/xpanse/api/issues/v1/issue_types.py
--rw-r--r--   0 runner    (1001) docker     (121)    27826 2022-05-02 21:04:04.000000 xpanse-1.3.1/xpanse/api/issues/v1/issues.py
--rw-r--r--   0 runner    (1001) docker     (121)     7097 2022-05-02 21:04:04.000000 xpanse-1.3.1/xpanse/api/issues/v1/policies.py
--rw-r--r--   0 runner    (1001) docker     (121)     1138 2022-05-02 21:04:04.000000 xpanse-1.3.1/xpanse/api/issues/v1/providers.py
--rw-r--r--   0 runner    (1001) docker     (121)     2157 2022-05-02 21:04:04.000000 xpanse-1.3.1/xpanse/api/issues/v1/updates.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-02 21:04:36.698585 xpanse-1.3.1/xpanse/api/services/
--rw-r--r--   0 runner    (1001) docker     (121)     1319 2022-05-02 21:04:04.000000 xpanse-1.3.1/xpanse/api/services/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-02 21:04:36.698585 xpanse-1.3.1/xpanse/api/services/v1/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-02 21:04:04.000000 xpanse-1.3.1/xpanse/api/services/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1203 2022-05-02 21:04:04.000000 xpanse-1.3.1/xpanse/api/services/v1/classifications.py
--rw-r--r--   0 runner    (1001) docker     (121)     1168 2022-05-02 21:04:04.000000 xpanse-1.3.1/xpanse/api/services/v1/country_codes.py
--rw-r--r--   0 runner    (1001) docker     (121)    29808 2022-05-02 21:04:04.000000 xpanse-1.3.1/xpanse/api/services/v1/services.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-02 21:04:36.698585 xpanse-1.3.1/xpanse/api/targeted_ips/
--rw-r--r--   0 runner    (1001) docker     (121)      494 2022-05-02 21:04:04.000000 xpanse-1.3.1/xpanse/api/targeted_ips/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-02 21:04:36.698585 xpanse-1.3.1/xpanse/api/targeted_ips/v1/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-02 21:04:04.000000 xpanse-1.3.1/xpanse/api/targeted_ips/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      920 2022-05-02 21:04:04.000000 xpanse-1.3.1/xpanse/api/targeted_ips/v1/targeted_ips.py
--rw-r--r--   0 runner    (1001) docker     (121)      149 2022-05-02 21:04:04.000000 xpanse-1.3.1/xpanse/base_api.py
--rw-r--r--   0 runner    (1001) docker     (121)    21058 2022-05-02 21:04:04.000000 xpanse-1.3.1/xpanse/client.py
--rw-r--r--   0 runner    (1001) docker     (121)     1106 2022-05-02 21:04:04.000000 xpanse-1.3.1/xpanse/const.py
--rw-r--r--   0 runner    (1001) docker     (121)      313 2022-05-02 21:04:04.000000 xpanse-1.3.1/xpanse/endpoint.py
--rw-r--r--   0 runner    (1001) docker     (121)     1010 2022-05-02 21:04:04.000000 xpanse-1.3.1/xpanse/error.py
--rw-r--r--   0 runner    (1001) docker     (121)     2378 2022-05-02 21:04:04.000000 xpanse-1.3.1/xpanse/iterator.py
--rw-r--r--   0 runner    (1001) docker     (121)      392 2022-05-02 21:04:04.000000 xpanse-1.3.1/xpanse/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-02 21:04:36.694585 xpanse-1.3.1/xpanse.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3775 2022-05-02 21:04:36.000000 xpanse-1.3.1/xpanse.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3090 2022-05-02 21:04:36.000000 xpanse-1.3.1/xpanse.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-02 21:04:36.000000 xpanse-1.3.1/xpanse.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       35 2022-05-02 21:04:36.000000 xpanse-1.3.1/xpanse.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       21 2022-05-02 21:04:36.000000 xpanse-1.3.1/xpanse.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:38:20.412516 xpanse-2.0.0rc3/
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-05-30 19:37:39.000000 xpanse-2.0.0rc3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-05-30 19:37:39.000000 xpanse-2.0.0rc3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4011 2023-05-30 19:38:20.412516 xpanse-2.0.0rc3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3119 2023-05-30 19:37:39.000000 xpanse-2.0.0rc3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:38:20.408517 xpanse-2.0.0rc3/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-05-30 19:37:39.000000 xpanse-2.0.0rc3/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-05-30 19:37:39.000000 xpanse-2.0.0rc3/docs/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:38:20.408517 xpanse-2.0.0rc3/docs/_source/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:38:20.408517 xpanse-2.0.0rc3/docs/_source/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)    17992 2023-05-30 19:37:39.000000 xpanse-2.0.0rc3/docs/_source/_static/xpanse_banner.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3531 2023-05-30 19:37:39.000000 xpanse-2.0.0rc3/docs/_source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2247 2023-05-30 19:37:39.000000 xpanse-2.0.0rc3/docs/_source/cover.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-05-30 19:37:39.000000 xpanse-2.0.0rc3/docs/_source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-05-30 19:37:39.000000 xpanse-2.0.0rc3/docs/_source/xpanse.api.asset_management.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-05-30 19:37:39.000000 xpanse-2.0.0rc3/docs/_source/xpanse.api.attack_surface_rules.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-05-30 19:37:39.000000 xpanse-2.0.0rc3/docs/_source/xpanse.api.incident_management.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-05-30 19:37:39.000000 xpanse-2.0.0rc3/docs/_source/xpanse.api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-30 19:37:39.000000 xpanse-2.0.0rc3/docs/_source/xpanse.api.tags.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-05-30 19:37:39.000000 xpanse-2.0.0rc3/docs/_source/xpanse.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-05-30 19:37:39.000000 xpanse-2.0.0rc3/docs/requirements-docs.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:38:20.408517 xpanse-2.0.0rc3/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:38:20.408517 xpanse-2.0.0rc3/examples/asset_management/
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-05-30 19:37:39.000000 xpanse-2.0.0rc3/examples/asset_management/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3418 2023-05-30 19:37:39.000000 xpanse-2.0.0rc3/examples/asset_management/get_services_by_asset.py
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-30 19:37:39.000000 xpanse-2.0.0rc3/examples/asset_management/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:38:20.412516 xpanse-2.0.0rc3/examples/incident_management/
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-05-30 19:37:39.000000 xpanse-2.0.0rc3/examples/incident_management/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-30 19:37:39.000000 xpanse-2.0.0rc3/examples/incident_management/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3442 2023-05-30 19:37:39.000000 xpanse-2.0.0rc3/examples/incident_management/update_incidents.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:38:20.412516 xpanse-2.0.0rc3/examples/tags/
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-05-30 19:37:39.000000 xpanse-2.0.0rc3/examples/tags/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-05-30 19:37:39.000000 xpanse-2.0.0rc3/examples/tags/assign_and_remove_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-30 19:37:39.000000 xpanse-2.0.0rc3/examples/tags/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 19:38:20.412516 xpanse-2.0.0rc3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-05-30 19:37:39.000000 xpanse-2.0.0rc3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:38:20.412516 xpanse-2.0.0rc3/xpanse/
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-05-30 19:37:39.000000 xpanse-2.0.0rc3/xpanse/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:38:20.412516 xpanse-2.0.0rc3/xpanse/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 19:37:39.000000 xpanse-2.0.0rc3/xpanse/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:38:20.412516 xpanse-2.0.0rc3/xpanse/api/asset_management/
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-05-30 19:37:39.000000 xpanse-2.0.0rc3/xpanse/api/asset_management/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4080 2023-05-30 19:37:39.000000 xpanse-2.0.0rc3/xpanse/api/asset_management/assets_management_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:38:20.412516 xpanse-2.0.0rc3/xpanse/api/asset_management/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 19:37:39.000000 xpanse-2.0.0rc3/xpanse/api/asset_management/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6859 2023-05-30 19:37:39.000000 xpanse-2.0.0rc3/xpanse/api/asset_management/v1/assets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5412 2023-05-30 19:37:39.000000 xpanse-2.0.0rc3/xpanse/api/asset_management/v1/owned_ip_ranges.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5230 2023-05-30 19:37:39.000000 xpanse-2.0.0rc3/xpanse/api/asset_management/v1/services.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:38:20.412516 xpanse-2.0.0rc3/xpanse/api/attack_surface_rules/
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-05-30 19:37:39.000000 xpanse-2.0.0rc3/xpanse/api/attack_surface_rules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:38:20.412516 xpanse-2.0.0rc3/xpanse/api/attack_surface_rules/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 19:37:39.000000 xpanse-2.0.0rc3/xpanse/api/attack_surface_rules/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6034 2023-05-30 19:37:39.000000 xpanse-2.0.0rc3/xpanse/api/attack_surface_rules/v1/attack_surface_rules.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:38:20.412516 xpanse-2.0.0rc3/xpanse/api/incident_management/
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-05-30 19:37:39.000000 xpanse-2.0.0rc3/xpanse/api/incident_management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:38:20.412516 xpanse-2.0.0rc3/xpanse/api/incident_management/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 19:37:39.000000 xpanse-2.0.0rc3/xpanse/api/incident_management/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7659 2023-05-30 19:37:39.000000 xpanse-2.0.0rc3/xpanse/api/incident_management/v1/incidents.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:38:20.412516 xpanse-2.0.0rc3/xpanse/api/incident_management/v2/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 19:37:39.000000 xpanse-2.0.0rc3/xpanse/api/incident_management/v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5239 2023-05-30 19:37:39.000000 xpanse-2.0.0rc3/xpanse/api/incident_management/v2/alerts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:38:20.412516 xpanse-2.0.0rc3/xpanse/api/tags/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-30 19:37:39.000000 xpanse-2.0.0rc3/xpanse/api/tags/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:38:20.412516 xpanse-2.0.0rc3/xpanse/api/tags/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 19:37:39.000000 xpanse-2.0.0rc3/xpanse/api/tags/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6754 2023-05-30 19:37:39.000000 xpanse-2.0.0rc3/xpanse/api/tags/v1/tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16292 2023-05-30 19:37:39.000000 xpanse-2.0.0rc3/xpanse/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3500 2023-05-30 19:37:39.000000 xpanse-2.0.0rc3/xpanse/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-05-30 19:37:39.000000 xpanse-2.0.0rc3/xpanse/endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-05-30 19:37:39.000000 xpanse-2.0.0rc3/xpanse/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6309 2023-05-30 19:37:39.000000 xpanse-2.0.0rc3/xpanse/iterator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-05-30 19:37:39.000000 xpanse-2.0.0rc3/xpanse/response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-05-30 19:37:39.000000 xpanse-2.0.0rc3/xpanse/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2947 2023-05-30 19:37:39.000000 xpanse-2.0.0rc3/xpanse/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:38:20.412516 xpanse-2.0.0rc3/xpanse.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4011 2023-05-30 19:38:20.000000 xpanse-2.0.0rc3/xpanse.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-05-30 19:38:20.000000 xpanse-2.0.0rc3/xpanse.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 19:38:20.000000 xpanse-2.0.0rc3/xpanse.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-30 19:38:20.000000 xpanse-2.0.0rc3/xpanse.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-30 19:38:20.000000 xpanse-2.0.0rc3/xpanse.egg-info/top_level.txt
```

### Comparing `xpanse-1.3.1/LICENSE` & `xpanse-2.0.0rc3/LICENSE`

 * *Files identical despite different names*

### Comparing `xpanse-1.3.1/PKG-INFO` & `xpanse-2.0.0rc3/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,236 +1,251 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 7870 616e  : 2.1.Name: xpan
-00000020: 7365 0a56 6572 7369 6f6e 3a20 312e 332e  se.Version: 1.3.
-00000030: 310a 5375 6d6d 6172 793a 2050 7974 686f  1.Summary: Pytho
-00000040: 6e20 6c69 6272 6172 7920 6973 2061 6e20  n library is an 
-00000050: 696e 7465 7266 6163 6520 746f 2074 6865  interface to the
-00000060: 2058 7061 6e73 6520 4578 7061 6e64 6572   Xpanse Expander
-00000070: 2041 5049 2e0a 486f 6d65 2d70 6167 653a   API..Home-page:
-00000080: 2055 4e4b 4e4f 574e 0a41 7574 686f 723a   UNKNOWN.Author:
-00000090: 2050 616c 6f20 416c 746f 2043 6f72 7465   Palo Alto Corte
-000000a0: 7820 5870 616e 7365 0a41 7574 686f 722d  x Xpanse.Author-
-000000b0: 656d 6169 6c3a 2078 7061 6e73 652d 696e  email: xpanse-in
-000000c0: 7465 6772 6174 696f 6e73 4070 616c 6f61  tegrations@paloa
-000000d0: 6c74 6f6e 6574 776f 726b 732e 636f 6d0a  ltonetworks.com.
-000000e0: 4c69 6365 6e73 653a 2049 5343 0a4b 6579  License: ISC.Key
-000000f0: 776f 7264 733a 2078 7061 6e73 6520 696f  words: xpanse io
-00000100: 6d0a 506c 6174 666f 726d 3a20 554e 4b4e  m.Platform: UNKN
-00000110: 4f57 4e0a 436c 6173 7369 6669 6572 3a20  OWN.Classifier: 
-00000120: 4465 7665 6c6f 706d 656e 7420 5374 6174  Development Stat
-00000130: 7573 203a 3a20 3520 2d20 5072 6f64 7563  us :: 5 - Produc
-00000140: 7469 6f6e 2f53 7461 626c 650a 436c 6173  tion/Stable.Clas
-00000150: 7369 6669 6572 3a20 496e 7465 6e64 6564  sifier: Intended
-00000160: 2041 7564 6965 6e63 6520 3a3a 2044 6576   Audience :: Dev
-00000170: 656c 6f70 6572 730a 436c 6173 7369 6669  elopers.Classifi
-00000180: 6572 3a20 546f 7069 6320 3a3a 2053 6f66  er: Topic :: Sof
-00000190: 7477 6172 6520 4465 7665 6c6f 706d 656e  tware Developmen
-000001a0: 740a 436c 6173 7369 6669 6572 3a20 546f  t.Classifier: To
-000001b0: 7069 6320 3a3a 2053 6f66 7477 6172 6520  pic :: Software 
-000001c0: 4465 7665 6c6f 706d 656e 7420 3a3a 204c  Development :: L
-000001d0: 6962 7261 7269 6573 0a43 6c61 7373 6966  ibraries.Classif
-000001e0: 6965 723a 2054 6f70 6963 203a 3a20 536f  ier: Topic :: So
-000001f0: 6674 7761 7265 2044 6576 656c 6f70 6d65  ftware Developme
-00000200: 6e74 203a 3a20 4c69 6272 6172 6965 7320  nt :: Libraries 
-00000210: 3a3a 2041 7070 6c69 6361 7469 6f6e 2046  :: Application F
-00000220: 7261 6d65 776f 726b 730a 436c 6173 7369  rameworks.Classi
-00000230: 6669 6572 3a20 5072 6f67 7261 6d6d 696e  fier: Programmin
-00000240: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
-00000250: 7468 6f6e 203a 3a20 330a 436c 6173 7369  thon :: 3.Classi
-00000260: 6669 6572 3a20 5072 6f67 7261 6d6d 696e  fier: Programmin
-00000270: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
-00000280: 7468 6f6e 203a 3a20 332e 360a 436c 6173  thon :: 3.6.Clas
-00000290: 7369 6669 6572 3a20 5072 6f67 7261 6d6d  sifier: Programm
-000002a0: 696e 6720 4c61 6e67 7561 6765 203a 3a20  ing Language :: 
-000002b0: 5079 7468 6f6e 203a 3a20 332e 370a 436c  Python :: 3.7.Cl
-000002c0: 6173 7369 6669 6572 3a20 5072 6f67 7261  assifier: Progra
-000002d0: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
-000002e0: 3a20 5079 7468 6f6e 203a 3a20 332e 380a  : Python :: 3.8.
-000002f0: 5265 7175 6972 6573 2d50 7974 686f 6e3a  Requires-Python:
-00000300: 203e 3d33 2e36 0a4c 6963 656e 7365 2d46   >=3.6.License-F
-00000310: 696c 653a 204c 4943 454e 5345 0a0a 5870  ile: LICENSE..Xp
-00000320: 616e 7365 2050 7974 686f 6e20 5344 4b0a  anse Python SDK.
-00000330: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00000340: 3d3d 0a2e 2e20 696d 6167 653a 3a20 6874  ==... image:: ht
-00000350: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00000360: 2f50 616c 6f41 6c74 6f4e 6574 776f 726b  /PaloAltoNetwork
-00000370: 732f 636f 7274 6578 2d78 7061 6e73 652d  s/cortex-xpanse-
-00000380: 7079 7468 6f6e 2d73 646b 2f62 6c6f 622f  python-sdk/blob/
-00000390: 6d61 696e 2f64 6f63 732f 5f73 6f75 7263  main/docs/_sourc
-000003a0: 652f 5f73 7461 7469 632f 7870 616e 7365  e/_static/xpanse
-000003b0: 5f62 616e 6e65 722e 706e 673f 7261 773d  _banner.png?raw=
-000003c0: 7472 7565 0a20 2020 3a77 6964 7468 3a20  true.   :width: 
-000003d0: 3830 300a 2020 203a 7461 7267 6574 3a20  800.   :target: 
-000003e0: 6874 7470 733a 2f2f 6578 7061 6e73 652e  https://expanse.
-000003f0: 636f 2f0a 0a2e 2e20 696d 6167 653a 3a20  co/.... image:: 
-00000400: 6874 7470 733a 2f2f 696d 672e 7368 6965  https://img.shie
-00000410: 6c64 732e 696f 2f62 6164 6765 2f63 6f64  lds.io/badge/cod
-00000420: 6525 3230 7374 796c 652d 626c 6163 6b2d  e%20style-black-
-00000430: 3030 3030 3030 2e73 7667 0a20 2020 3a74  000000.svg.   :t
-00000440: 6172 6765 743a 2068 7474 7073 3a2f 2f67  arget: https://g
-00000450: 6974 6875 622e 636f 6d2f 7073 662f 626c  ithub.com/psf/bl
-00000460: 6163 6b0a 0a2e 2e20 696d 6167 653a 3a20  ack.... image:: 
-00000470: 6874 7470 733a 2f2f 696d 672e 7368 6965  https://img.shie
-00000480: 6c64 732e 696f 2f62 6164 6765 2f70 7974  lds.io/badge/pyt
-00000490: 686f 6e2d 332e 3625 3230 2537 4325 3230  hon-3.6%20%7C%20
-000004a0: 332e 3725 3230 2537 4325 3230 332e 382d  3.7%20%7C%203.8-
-000004b0: 626c 7565 7669 6f6c 6574 0a20 2020 3a74  blueviolet.   :t
-000004c0: 6172 6765 743a 2068 7474 7073 3a2f 2f70  arget: https://p
-000004d0: 7970 692e 7079 7468 6f6e 2e6f 7267 2f70  ypi.python.org/p
-000004e0: 7970 692f 7870 616e 7365 0a0a 2e2e 2069  ypi/xpanse.... i
-000004f0: 6d61 6765 3a3a 2068 7474 7073 3a2f 2f69  mage:: https://i
-00000500: 6d67 2e73 6869 656c 6473 2e69 6f2f 6261  mg.shields.io/ba
-00000510: 6467 652f 636f 6465 2532 3073 7479 6c65  dge/code%20style
-00000520: 2d62 6c61 636b 2d30 3030 3030 302e 7376  -black-000000.sv
-00000530: 670a 2020 203a 7461 7267 6574 3a20 6874  g.   :target: ht
-00000540: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00000550: 2f70 7366 2f62 6c61 636b 0a0a 2e2e 2069  /psf/black.... i
-00000560: 6d61 6765 3a3a 2068 7474 7073 3a2f 2f69  mage:: https://i
-00000570: 6d67 2e73 6869 656c 6473 2e69 6f2f 7079  mg.shields.io/py
-00000580: 7069 2f6c 2f78 7061 6e73 650a 2020 203a  pi/l/xpanse.   :
-00000590: 7461 7267 6574 3a20 6874 7470 733a 2f2f  target: https://
-000005a0: 6769 7468 7562 2e63 6f6d 2f50 616c 6f41  github.com/PaloA
-000005b0: 6c74 6f4e 6574 776f 726b 732f 636f 7274  ltoNetworks/cort
-000005c0: 6578 2d78 7061 6e73 652d 7079 7468 6f6e  ex-xpanse-python
-000005d0: 2d73 646b 2f62 6c6f 622f 6d61 696e 2f4c  -sdk/blob/main/L
-000005e0: 4943 454e 5345 0a0a 2e2e 2069 6d61 6765  ICENSE.... image
-000005f0: 3a3a 2068 7474 7073 3a2f 2f69 6d67 2e73  :: https://img.s
-00000600: 6869 656c 6473 2e69 6f2f 6769 7468 7562  hields.io/github
-00000610: 2f63 6f6e 7472 6962 7574 6f72 732f 5061  /contributors/Pa
-00000620: 6c6f 416c 746f 4e65 7477 6f72 6b73 2f63  loAltoNetworks/c
-00000630: 6f72 7465 782d 7870 616e 7365 2d70 7974  ortex-xpanse-pyt
-00000640: 686f 6e2d 7364 6b0a 2020 203a 7461 7267  hon-sdk.   :targ
-00000650: 6574 3a20 6874 7470 733a 2f2f 6769 7468  et: https://gith
-00000660: 7562 2e63 6f6d 2f50 616c 6f41 6c74 6f4e  ub.com/PaloAltoN
-00000670: 6574 776f 726b 732f 636f 7274 6578 2d78  etworks/cortex-x
-00000680: 7061 6e73 652d 7079 7468 6f6e 2d73 646b  panse-python-sdk
-00000690: 2f67 7261 7068 732f 636f 6e74 7269 6275  /graphs/contribu
-000006a0: 746f 7273 0a0a 4f76 6572 7669 6577 0a2d  tors..Overview.-
-000006b0: 2d2d 2d2d 2d2d 2d0a 0a54 6869 7320 6c69  -------..This li
-000006c0: 6272 6172 7920 6973 2069 6e74 656e 6465  brary is intende
-000006d0: 6420 746f 2062 6520 616e 2069 6e74 6572  d to be an inter
-000006e0: 6661 6365 2074 6f20 7468 6520 6058 7061  face to the `Xpa
-000006f0: 6e73 6520 4578 7061 6e64 6572 2041 5049  nse Expander API
-00000700: 203c 6874 7470 733a 2f2f 6b6e 6f77 6c65   <https://knowle
-00000710: 6467 6562 6173 652e 7870 616e 7365 2e63  dgebase.xpanse.c
-00000720: 6f2f 6578 7061 6e64 6572 2d61 7069 732f  o/expander-apis/
-00000730: 3e60 5f2e 0a0a 496e 7374 616c 6c0a 2d2d  >`_...Install.--
-00000740: 2d2d 2d2d 2d0a 2e2e 2063 6f64 652d 626c  -----... code-bl
-00000750: 6f63 6b3a 3a20 7079 7468 6f6e 0a0a 2020  ock:: python..  
-00000760: 2020 7069 7020 696e 7374 616c 6c20 7870    pip install xp
-00000770: 616e 7365 0a0a 5265 7175 6972 656d 656e  anse..Requiremen
-00000780: 7473 0a2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a  ts.------------.
-00000790: 0a50 7974 686f 6e20 332e 362b 0a0a 5573  .Python 3.6+..Us
-000007a0: 6167 650a 2d2d 2d2d 2d0a 6044 6f63 756d  age.-----.`Docum
-000007b0: 656e 7461 7469 6f6e 203c 6874 7470 733a  entation <https:
-000007c0: 2f2f 636f 7274 6578 2d78 7061 6e73 652d  //cortex-xpanse-
-000007d0: 7079 7468 6f6e 2d73 646b 2e72 6561 6474  python-sdk.readt
-000007e0: 6865 646f 6373 2e69 6f2f 656e 2f6c 6174  hedocs.io/en/lat
-000007f0: 6573 742f 3e60 5f0a 0a2e 2e20 636f 6465  est/>`_.... code
-00000800: 2d62 6c6f 636b 3a3a 2070 7974 686f 6e0a  -block:: python.
-00000810: 0a20 2020 2023 2049 6d70 6f72 7420 636c  .    # Import cl
-00000820: 6965 6e74 0a20 2020 2066 726f 6d20 7870  ient.    from xp
-00000830: 616e 7365 2e63 6c69 656e 7420 696d 706f  anse.client impo
-00000840: 7274 2045 7843 6c69 656e 740a 0a20 2020  rt ExClient..   
-00000850: 2023 2069 6e69 7469 616c 697a 6520 636c   # initialize cl
-00000860: 6965 6e74 0a20 2020 2063 6c69 656e 7420  ient.    client 
-00000870: 3d20 4578 436c 6965 6e74 2829 0a0a 2020  = ExClient()..  
-00000880: 2020 2320 6765 7420 6970 5f72 616e 6765    # get ip_range
-00000890: 2069 7465 7261 746f 7220 6f62 6a65 6374   iterator object
-000008a0: 2061 6e64 2064 756d 7020 746f 2061 206c   and dump to a l
-000008b0: 6973 740a 2020 2020 7261 6e67 6573 203d  ist.    ranges =
-000008c0: 2063 6c69 656e 742e 6173 7365 7473 2e69   client.assets.i
-000008d0: 705f 7261 6e67 652e 6c69 7374 2829 2e64  p_range.list().d
-000008e0: 756d 7028 290a 0a59 6f75 2063 616e 2076  ump()..You can v
-000008f0: 6965 7720 6d6f 7265 2065 7861 6d70 6c65  iew more example
-00000900: 2063 6f64 6520 696e 2074 6865 2060 6578   code in the `ex
-00000910: 616d 706c 6573 203c 6874 7470 733a 2f2f  amples <https://
-00000920: 6769 7468 7562 2e63 6f6d 2f50 616c 6f41  github.com/PaloA
-00000930: 6c74 6f4e 6574 776f 726b 732f 636f 7274  ltoNetworks/cort
-00000940: 6578 2d78 7061 6e73 652d 7079 7468 6f6e  ex-xpanse-python
-00000950: 2d73 646b 2f74 7265 652f 6d61 696e 2f65  -sdk/tree/main/e
-00000960: 7861 6d70 6c65 733e 605f 2064 6972 6563  xamples>`_ direc
-00000970: 746f 7279 2e0a 0a43 6f6e 6669 6775 7261  tory...Configura
-00000980: 7469 6f6e 0a2d 2d2d 2d2d 2d2d 2d2d 2d2d  tion.-----------
-00000990: 2d2d 0a41 2076 616c 6964 2043 6c69 656e  --.A valid Clien
-000009a0: 7420 4944 2061 6e64 2053 6563 7265 7420  t ID and Secret 
-000009b0: 6973 2072 6571 7569 7265 6420 666f 7220  is required for 
-000009c0: 7573 652e 2054 6869 7320 6973 2072 6563  use. This is rec
-000009d0: 6f6d 6d65 6e64 6564 206f 7665 7220 7573  ommended over us
-000009e0: 696e 6720 6120 4a57 542c 2061 7320 7468  ing a JWT, as th
-000009f0: 6579 2068 6176 6520 6c69 6d69 7465 6420  ey have limited 
-00000a00: 6c69 6665 7370 616e 732e 0a57 6869 6c65  lifespans..While
-00000a10: 2061 2062 6561 7265 7220 746f 6b65 6e20   a bearer token 
-00000a20: 6973 2073 7570 706f 7274 6564 2069 6e20  is supported in 
-00000a30: 7468 6973 2076 6572 7369 6f6e 2c20 7468  this version, th
-00000a40: 6973 2061 7574 6820 666c 6f77 2069 7320  is auth flow is 
-00000a50: 6265 696e 6720 6465 7072 6563 6174 6564  being deprecated
-00000a60: 2e20 5468 6572 6566 6f72 652c 2069 7420  . Therefore, it 
-00000a70: 6973 2068 6967 686c 7920 7265 636f 6d6d  is highly recomm
-00000a80: 656e 6465 6420 746f 2075 7365 2043 6c69  ended to use Cli
-00000a90: 656e 7420 4372 6564 656e 7469 616c 732e  ent Credentials.
-00000aa0: 0a0a 5245 434f 4d4d 454e 4445 440a 2a2a  ..RECOMMENDED.**
-00000ab0: 2a2a 2a2a 2a2a 2a2a 2a0a 596f 7520 6361  *********.You ca
-00000ac0: 6e20 7375 7070 6c79 2074 6865 6d20 6173  n supply them as
-00000ad0: 2065 6e76 6972 6f6e 6d65 6e74 2076 6172   environment var
-00000ae0: 6961 626c 6573 2075 7369 6e67 2074 6865  iables using the
-00000af0: 2076 6172 6961 626c 6520 6e61 6d65 7320   variable names 
-00000b00: 6060 5850 414e 5345 5f43 4c49 454e 545f  ``XPANSE_CLIENT_
-00000b10: 4944 6060 2041 4e44 2060 6058 5041 4e53  ID`` AND ``XPANS
-00000b20: 455f 434c 4945 4e54 5f53 4543 5245 5460  E_CLIENT_SECRET`
-00000b30: 602e 0a0a 2e2e 2063 6f64 652d 626c 6f63  `..... code-bloc
-00000b40: 6b3a 3a20 7079 7468 6f6e 0a0a 2020 2020  k:: python..    
-00000b50: 6578 706f 7274 2058 5041 4e53 455f 434c  export XPANSE_CL
-00000b60: 4945 4e54 5f49 443d 3c43 6c69 656e 7420  IENT_ID=<Client 
-00000b70: 4944 3e0a 2020 2020 6578 706f 7274 2058  ID>.    export X
-00000b80: 5041 4e53 455f 434c 4945 4e54 5f53 4543  PANSE_CLIENT_SEC
-00000b90: 5245 543d 3c43 6c69 656e 7420 5365 6372  RET=<Client Secr
-00000ba0: 6574 3e0a 2020 2020 0a4e 4f54 2052 4543  et>.    .NOT REC
-00000bb0: 4f4d 4d45 4e44 4544 0a2a 2a2a 2a2a 2a2a  OMMENDED.*******
-00000bc0: 2a2a 2a2a 2a2a 2a2a 0a54 6f20 7573 6520  ********.To use 
-00000bd0: 6120 7368 6f72 7420 6c69 7665 6420 4a57  a short lived JW
-00000be0: 542c 2079 6f75 2063 616e 2073 7570 706c  T, you can suppl
-00000bf0: 7920 7468 6520 4a57 5420 6173 2061 6e20  y the JWT as an 
-00000c00: 656e 7669 726f 6e6d 656e 7461 6c20 7661  environmental va
-00000c10: 7269 6162 6c65 2075 7369 6e67 2074 6865  riable using the
-00000c20: 206e 616d 6520 6060 5850 414e 5345 5f4a   name ``XPANSE_J
-00000c30: 5754 5f54 4f4b 454e 6060 0a0a 2e2e 2063  WT_TOKEN``.... c
-00000c40: 6f64 652d 626c 6f63 6b3a 3a20 7079 7468  ode-block:: pyth
-00000c50: 6f6e 0a0a 2020 2020 6578 706f 7274 2058  on..    export X
-00000c60: 5041 4e53 455f 4a57 545f 544f 4b45 4e3d  PANSE_JWT_TOKEN=
-00000c70: 3c4a 5754 3e0a 0a5b 4465 7072 6563 6174  <JWT>..[Deprecat
-00000c80: 6564 5d0a 4120 7661 6c69 6420 4265 6172  ed].A valid Bear
-00000c90: 6572 2074 6f6b 656e 2063 616e 2062 6520  er token can be 
-00000ca0: 7375 7070 6c69 6564 2061 7320 616e 2065  supplied as an e
-00000cb0: 6e76 6972 6f6e 6d65 6e74 2076 6172 6961  nvironment varia
-00000cc0: 626c 650a 0a54 6f20 7375 7070 6c79 2061  ble..To supply a
-00000cd0: 2076 616c 6964 2062 6561 7265 7220 746f   valid bearer to
-00000ce0: 6b65 6e20 6173 2061 6e20 656e 7669 726f  ken as an enviro
-00000cf0: 6e6d 656e 7420 7661 7269 6162 6c65 2c20  nment variable, 
-00000d00: 796f 7520 6361 6e20 7573 6520 7468 6520  you can use the 
-00000d10: 7661 7269 6162 6c65 206e 616d 6573 2060  variable names `
-00000d20: 6058 5041 4e53 455f 4245 4152 4552 5f54  `XPANSE_BEARER_T
-00000d30: 4f4b 454e 6060 2e0a 0a2e 2e20 636f 6465  OKEN``..... code
-00000d40: 2d62 6c6f 636b 3a3a 2070 7974 686f 6e0a  -block:: python.
-00000d50: 0a20 2020 2065 7870 6f72 7420 5850 414e  .    export XPAN
-00000d60: 5345 5f42 4541 5245 525f 544f 4b45 4e3d  SE_BEARER_TOKEN=
-00000d70: 3c42 6561 7265 7220 546f 6b65 6e3e 0a0a  <Bearer Token>..
-00000d80: 4c6f 6767 696e 670a 2d2d 2d2d 2d2d 2d0a  Logging.-------.
-00000d90: 4c6f 6767 696e 6720 6973 2068 616e 646c  Logging is handl
-00000da0: 6564 2074 6872 6f75 6768 2074 6865 2070  ed through the p
-00000db0: 7974 686f 6e20 6c6f 6767 696e 6720 7061  ython logging pa
-00000dc0: 636b 6167 652e 2054 6f20 656e 6162 6c65  ckage. To enable
-00000dd0: 2064 6966 6665 7265 6e74 206c 6576 656c   different level
-00000de0: 7320 6f66 2076 6572 626f 7369 7479 2069  s of verbosity i
-00000df0: 6e20 796f 7572 2073 6372 6970 7473 2079  n your scripts y
-00000e00: 6f75 2063 616e 2064 6f20 7468 6520 666f  ou can do the fo
-00000e10: 6c6c 6f77 696e 673a 0a0a 2e2e 2063 6f64  llowing:.... cod
-00000e20: 652d 626c 6f63 6b3a 3a20 7079 7468 6f6e  e-block:: python
-00000e30: 0a0a 2020 2020 696d 706f 7274 206c 6f67  ..    import log
-00000e40: 6769 6e67 0a20 2020 206c 6f67 6769 6e67  ging.    logging
-00000e50: 2e62 6173 6963 436f 6e66 6967 286c 6576  .basicConfig(lev
-00000e60: 656c 3d6c 6f67 6769 6e67 2e44 4542 5547  el=logging.DEBUG
-00000e70: 290a 0a59 6f75 2063 616e 2072 6561 6420  )..You can read 
-00000e80: 6d6f 7265 2061 7420 603c 6874 7470 733a  more at `<https:
-00000e90: 2f2f 646f 6373 2e70 7974 686f 6e2e 6f72  //docs.python.or
-00000ea0: 672f 332f 6c69 6272 6172 792f 6c6f 6767  g/3/library/logg
-00000eb0: 696e 672e 6874 6d6c 3e60 5f2e 0a0a 0a    ing.html>`_....
+00000020: 7365 0a56 6572 7369 6f6e 3a20 322e 302e  se.Version: 2.0.
+00000030: 3072 6333 0a53 756d 6d61 7279 3a20 5079  0rc3.Summary: Py
+00000040: 7468 6f6e 206c 6962 7261 7279 2069 7320  thon library is 
+00000050: 616e 2069 6e74 6572 6661 6365 2074 6f20  an interface to 
+00000060: 7468 6520 436f 7274 6578 2058 7061 6e73  the Cortex Xpans
+00000070: 6520 4150 492e 0a48 6f6d 652d 7061 6765  e API..Home-page
+00000080: 3a20 554e 4b4e 4f57 4e0a 4175 7468 6f72  : UNKNOWN.Author
+00000090: 3a20 5061 6c6f 2041 6c74 6f20 436f 7274  : Palo Alto Cort
+000000a0: 6578 2058 7061 6e73 650a 4175 7468 6f72  ex Xpanse.Author
+000000b0: 2d65 6d61 696c 3a20 7870 616e 7365 2d69  -email: xpanse-i
+000000c0: 6e74 6567 7261 7469 6f6e 7340 7061 6c6f  ntegrations@palo
+000000d0: 616c 746f 6e65 7477 6f72 6b73 2e63 6f6d  altonetworks.com
+000000e0: 0a4c 6963 656e 7365 3a20 4953 430a 4b65  .License: ISC.Ke
+000000f0: 7977 6f72 6473 3a20 7870 616e 7365 2069  ywords: xpanse i
+00000100: 6f6d 0a50 6c61 7466 6f72 6d3a 2055 4e4b  om.Platform: UNK
+00000110: 4e4f 574e 0a43 6c61 7373 6966 6965 723a  NOWN.Classifier:
+00000120: 2044 6576 656c 6f70 6d65 6e74 2053 7461   Development Sta
+00000130: 7475 7320 3a3a 2035 202d 2050 726f 6475  tus :: 5 - Produ
+00000140: 6374 696f 6e2f 5374 6162 6c65 0a43 6c61  ction/Stable.Cla
+00000150: 7373 6966 6965 723a 2049 6e74 656e 6465  ssifier: Intende
+00000160: 6420 4175 6469 656e 6365 203a 3a20 4465  d Audience :: De
+00000170: 7665 6c6f 7065 7273 0a43 6c61 7373 6966  velopers.Classif
+00000180: 6965 723a 2054 6f70 6963 203a 3a20 536f  ier: Topic :: So
+00000190: 6674 7761 7265 2044 6576 656c 6f70 6d65  ftware Developme
+000001a0: 6e74 0a43 6c61 7373 6966 6965 723a 2054  nt.Classifier: T
+000001b0: 6f70 6963 203a 3a20 536f 6674 7761 7265  opic :: Software
+000001c0: 2044 6576 656c 6f70 6d65 6e74 203a 3a20   Development :: 
+000001d0: 4c69 6272 6172 6965 730a 436c 6173 7369  Libraries.Classi
+000001e0: 6669 6572 3a20 546f 7069 6320 3a3a 2053  fier: Topic :: S
+000001f0: 6f66 7477 6172 6520 4465 7665 6c6f 706d  oftware Developm
+00000200: 656e 7420 3a3a 204c 6962 7261 7269 6573  ent :: Libraries
+00000210: 203a 3a20 4170 706c 6963 6174 696f 6e20   :: Application 
+00000220: 4672 616d 6577 6f72 6b73 0a43 6c61 7373  Frameworks.Class
+00000230: 6966 6965 723a 2050 726f 6772 616d 6d69  ifier: Programmi
+00000240: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
+00000250: 7974 686f 6e20 3a3a 2033 0a43 6c61 7373  ython :: 3.Class
+00000260: 6966 6965 723a 2050 726f 6772 616d 6d69  ifier: Programmi
+00000270: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
+00000280: 7974 686f 6e20 3a3a 2033 2e37 0a43 6c61  ython :: 3.7.Cla
+00000290: 7373 6966 6965 723a 2050 726f 6772 616d  ssifier: Program
+000002a0: 6d69 6e67 204c 616e 6775 6167 6520 3a3a  ming Language ::
+000002b0: 2050 7974 686f 6e20 3a3a 2033 2e38 0a43   Python :: 3.8.C
+000002c0: 6c61 7373 6966 6965 723a 2050 726f 6772  lassifier: Progr
+000002d0: 616d 6d69 6e67 204c 616e 6775 6167 6520  amming Language 
+000002e0: 3a3a 2050 7974 686f 6e20 3a3a 2033 2e39  :: Python :: 3.9
+000002f0: 0a43 6c61 7373 6966 6965 723a 2050 726f  .Classifier: Pro
+00000300: 6772 616d 6d69 6e67 204c 616e 6775 6167  gramming Languag
+00000310: 6520 3a3a 2050 7974 686f 6e20 3a3a 2033  e :: Python :: 3
+00000320: 2e31 300a 5265 7175 6972 6573 2d50 7974  .10.Requires-Pyt
+00000330: 686f 6e3a 203e 3d33 2e37 0a44 6573 6372  hon: >=3.7.Descr
+00000340: 6970 7469 6f6e 2d43 6f6e 7465 6e74 2d54  iption-Content-T
+00000350: 7970 653a 2074 6578 742f 6d61 726b 646f  ype: text/markdo
+00000360: 776e 0a4c 6963 656e 7365 2d46 696c 653a  wn.License-File:
+00000370: 204c 4943 454e 5345 0a0a 436f 7274 6578   LICENSE..Cortex
+00000380: 2058 7061 6e73 6520 5079 7468 6f6e 2053   Xpanse Python S
+00000390: 444b 0a3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  DK.=============
+000003a0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d0a 3c70 2061  ===========.<p a
+000003b0: 6c69 676e 3d22 6365 6e74 6572 223e 0a20  lign="center">. 
+000003c0: 2020 203c 6120 6872 6566 3d22 6874 7470     <a href="http
+000003d0: 733a 2f2f 6578 7061 6e73 652e 636f 2f22  s://expanse.co/"
+000003e0: 3e0a 2020 2020 2020 2020 3c69 6d67 2073  >.        <img s
+000003f0: 7263 3d22 6874 7470 733a 2f2f 6769 7468  rc="https://gith
+00000400: 7562 2e63 6f6d 2f50 616c 6f41 6c74 6f4e  ub.com/PaloAltoN
+00000410: 6574 776f 726b 732f 636f 7274 6578 2d78  etworks/cortex-x
+00000420: 7061 6e73 652d 7079 7468 6f6e 2d73 646b  panse-python-sdk
+00000430: 2f62 6c6f 622f 6d61 696e 2f64 6f63 732f  /blob/main/docs/
+00000440: 5f73 6f75 7263 652f 5f73 7461 7469 632f  _source/_static/
+00000450: 7870 616e 7365 5f62 616e 6e65 722e 706e  xpanse_banner.pn
+00000460: 673f 7261 773d 7472 7565 222f 3e0a 2020  g?raw=true"/>.  
+00000470: 2020 3c2f 613e 0a3c 2f70 3e0a 0a3c 7020    </a>.</p>..<p 
+00000480: 616c 6967 6e3d 2263 656e 7465 7222 3e0a  align="center">.
+00000490: 2020 2020 3c61 2068 7265 663d 2268 7474      <a href="htt
+000004a0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+000004b0: 7073 662f 626c 6163 6b22 3e0a 2020 2020  psf/black">.    
+000004c0: 2020 2020 3c69 6d67 2073 7263 3d22 6874      <img src="ht
+000004d0: 7470 733a 2f2f 696d 672e 7368 6965 6c64  tps://img.shield
+000004e0: 732e 696f 2f62 6164 6765 2f63 6f64 6525  s.io/badge/code%
+000004f0: 3230 7374 796c 652d 626c 6163 6b2d 3030  20style-black-00
+00000500: 3030 3030 2e73 7667 222f 3e0a 2020 2020  0000.svg"/>.    
+00000510: 3c2f 613e 0a20 2020 203c 6120 6872 6566  </a>.    <a href
+00000520: 3d22 6874 7470 733a 2f2f 7079 7069 2e70  ="https://pypi.p
+00000530: 7974 686f 6e2e 6f72 672f 7079 7069 2f78  ython.org/pypi/x
+00000540: 7061 6e73 6522 3e0a 2020 2020 2020 2020  panse">.        
+00000550: 3c69 6d67 2073 7263 3d22 6874 7470 733a  <img src="https:
+00000560: 2f2f 696d 672e 7368 6965 6c64 732e 696f  //img.shields.io
+00000570: 2f62 6164 6765 2f70 7974 686f 6e2d 332e  /badge/python-3.
+00000580: 3725 3230 2537 4325 3230 332e 3825 3230  7%20%7C%203.8%20
+00000590: 2537 4325 3230 332e 3925 3230 2537 4325  %7C%203.9%20%7C%
+000005a0: 3230 332e 3130 2d62 6c75 6576 696f 6c65  203.10-blueviole
+000005b0: 7422 2f3e 0a20 2020 203c 2f61 3e0a 2020  t"/>.    </a>.  
+000005c0: 2020 3c61 2068 7265 663d 2268 7474 7073    <a href="https
+000005d0: 3a2f 2f67 6974 6875 622e 636f 6d2f 5061  ://github.com/Pa
+000005e0: 6c6f 416c 746f 4e65 7477 6f72 6b73 2f63  loAltoNetworks/c
+000005f0: 6f72 7465 782d 7870 616e 7365 2d70 7974  ortex-xpanse-pyt
+00000600: 686f 6e2d 7364 6b2f 626c 6f62 2f6d 6169  hon-sdk/blob/mai
+00000610: 6e2f 4c49 4345 4e53 4522 3e0a 2020 2020  n/LICENSE">.    
+00000620: 2020 2020 3c69 6d67 2073 7263 3d22 6874      <img src="ht
+00000630: 7470 733a 2f2f 696d 672e 7368 6965 6c64  tps://img.shield
+00000640: 732e 696f 2f70 7970 692f 6c2f 7870 616e  s.io/pypi/l/xpan
+00000650: 7365 222f 3e0a 2020 2020 3c2f 613e 0a20  se"/>.    </a>. 
+00000660: 2020 203c 6120 6872 6566 3d22 6874 7470     <a href="http
+00000670: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f50  s://github.com/P
+00000680: 616c 6f41 6c74 6f4e 6574 776f 726b 732f  aloAltoNetworks/
+00000690: 636f 7274 6578 2d78 7061 6e73 652d 7079  cortex-xpanse-py
+000006a0: 7468 6f6e 2d73 646b 2f67 7261 7068 732f  thon-sdk/graphs/
+000006b0: 636f 6e74 7269 6275 746f 7273 223e 0a20  contributors">. 
+000006c0: 2020 2020 2020 203c 696d 6720 7372 633d         <img src=
+000006d0: 2268 7474 7073 3a2f 2f69 6d67 2e73 6869  "https://img.shi
+000006e0: 656c 6473 2e69 6f2f 6769 7468 7562 2f63  elds.io/github/c
+000006f0: 6f6e 7472 6962 7574 6f72 732f 5061 6c6f  ontributors/Palo
+00000700: 416c 746f 4e65 7477 6f72 6b73 2f63 6f72  AltoNetworks/cor
+00000710: 7465 782d 7870 616e 7365 2d70 7974 686f  tex-xpanse-pytho
+00000720: 6e2d 7364 6b22 2f3e 0a20 2020 203c 2f61  n-sdk"/>.    </a
+00000730: 3e0a 3c2f 703e 0a0a 4f76 6572 7669 6577  >.</p>..Overview
+00000740: 0a2d 2d2d 2d2d 2d2d 2d0a 0a54 6869 7320  .--------..This 
+00000750: 6c69 6272 6172 7920 6973 2069 6e74 656e  library is inten
+00000760: 6465 6420 746f 2062 6520 616e 2069 6e74  ded to be an int
+00000770: 6572 6661 6365 2074 6f20 7468 650a 3c61  erface to the.<a
+00000780: 2068 7265 663d 2268 7474 7073 3a2f 2f64   href="https://d
+00000790: 6f63 732d 636f 7274 6578 2e70 616c 6f61  ocs-cortex.paloa
+000007a0: 6c74 6f6e 6574 776f 726b 732e 636f 6d2f  ltonetworks.com/
+000007b0: 722f 436f 7274 6578 2d58 5041 4e53 452f  r/Cortex-XPANSE/
+000007c0: 436f 7274 6578 2d58 7061 6e73 652d 4150  Cortex-Xpanse-AP
+000007d0: 492d 5265 6665 7265 6e63 6522 3e43 6f72  I-Reference">Cor
+000007e0: 7465 7820 5870 616e 7365 2050 7562 6c69  tex Xpanse Publi
+000007f0: 6320 4150 493c 2f61 3e2e 0a0a 496e 7374  c API</a>...Inst
+00000800: 616c 6c0a 2d2d 2d2d 2d2d 2d0a 6060 6070  all.-------.```p
+00000810: 7974 686f 6e0a 7069 7020 696e 7374 616c  ython.pip instal
+00000820: 6c20 7870 616e 7365 0a60 6060 0a0a 5265  l xpanse.```..Re
+00000830: 7175 6972 656d 656e 7473 0a2d 2d2d 2d2d  quirements.-----
+00000840: 2d2d 2d2d 2d2d 2d0a 0a60 5079 7468 6f6e  -------..`Python
+00000850: 2033 2e37 2b60 0a0a 5573 6167 650a 2d2d   3.7+`..Usage.--
+00000860: 2d2d 2d0a 3c61 2068 7265 663d 2268 7474  ---.<a href="htt
+00000870: 7073 3a2f 2f63 6f72 7465 782d 7870 616e  ps://cortex-xpan
+00000880: 7365 2d70 7974 686f 6e2d 7364 6b2e 7265  se-python-sdk.re
+00000890: 6164 7468 6564 6f63 732e 696f 2f65 6e2f  adthedocs.io/en/
+000008a0: 6c61 7465 7374 2f22 3e43 6f72 7465 7820  latest/">Cortex 
+000008b0: 5870 616e 7365 2050 7562 6c69 6320 4150  Xpanse Public AP
+000008c0: 4920 446f 6375 6d65 6e74 6174 696f 6e3c  I Documentation<
+000008d0: 2f61 3e0a 0a60 6060 7079 7468 6f6e 0a23  /a>..```python.#
+000008e0: 2049 6d70 6f72 7420 636c 6965 6e74 0a66   Import client.f
+000008f0: 726f 6d20 7870 616e 7365 2e63 6c69 656e  rom xpanse.clien
+00000900: 7420 696d 706f 7274 2058 7061 6e73 6543  t import XpanseC
+00000910: 6c69 656e 740a 0a23 2049 6e69 7469 616c  lient..# Initial
+00000920: 697a 6520 636c 6965 6e74 0a63 6c69 656e  ize client.clien
+00000930: 7420 3d20 5870 616e 7365 436c 6965 6e74  t = XpanseClient
+00000940: 2829 0a0a 2320 4765 7420 6173 7365 7473  ()..# Get assets
+00000950: 2069 7465 7261 746f 7220 6f62 6a65 6374   iterator object
+00000960: 2061 6e64 2064 756d 7020 746f 2061 206c   and dump to a l
+00000970: 6973 740a 6173 7365 7473 203d 2063 6c69  ist.assets = cli
+00000980: 656e 742e 6173 7365 7473 2e6c 6973 7428  ent.assets.list(
+00000990: 292e 6475 6d70 2829 0a60 6060 0a0a 596f  ).dump().```..Yo
+000009a0: 7520 6361 6e20 7669 6577 206d 6f72 6520  u can view more 
+000009b0: 6578 616d 706c 6520 636f 6465 2069 6e20  example code in 
+000009c0: 7468 6520 3c61 2068 7265 663d 2268 7474  the <a href="htt
+000009d0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+000009e0: 5061 6c6f 416c 746f 4e65 7477 6f72 6b73  PaloAltoNetworks
+000009f0: 2f63 6f72 7465 782d 7870 616e 7365 2d70  /cortex-xpanse-p
+00000a00: 7974 686f 6e2d 7364 6b2f 7472 6565 2f6d  ython-sdk/tree/m
+00000a10: 6169 6e2f 6578 616d 706c 6573 223e 6578  ain/examples">ex
+00000a20: 616d 706c 6573 3c2f 613e 2064 6972 6563  amples</a> direc
+00000a30: 746f 7279 2e0a 0a43 6f6e 6669 6775 7261  tory...Configura
+00000a40: 7469 6f6e 0a2d 2d2d 2d2d 2d2d 2d2d 2d2d  tion.-----------
+00000a50: 2d2d 0a41 2076 616c 6964 2060 4150 4920  --.A valid `API 
+00000a60: 4b65 7960 2c20 6041 5049 204b 6579 2049  Key`, `API Key I
+00000a70: 4460 2c20 616e 6420 6046 756c 6c79 2051  D`, and `Fully Q
+00000a80: 7561 6c69 6669 6564 2044 6f6d 6169 6e20  ualified Domain 
+00000a90: 4e61 6d65 2028 4651 444e 2960 2061 7265  Name (FQDN)` are
+00000aa0: 2072 6571 7569 7265 6420 666f 7220 7573   required for us
+00000ab0: 652e 0a0a 5265 6665 7265 6e63 6520 7468  e...Reference th
+00000ac0: 6520 646f 6373 2066 6f72 206d 6f72 6520  e docs for more 
+00000ad0: 696e 666f 726d 6174 696f 6e20 7769 7468  information with
+00000ae0: 203c 6120 6872 6566 3d22 6874 7470 733a   <a href="https:
+00000af0: 2f2f 646f 6373 2d63 6f72 7465 782e 7061  //docs-cortex.pa
+00000b00: 6c6f 616c 746f 6e65 7477 6f72 6b73 2e63  loaltonetworks.c
+00000b10: 6f6d 2f72 2f43 6f72 7465 782d 5850 414e  om/r/Cortex-XPAN
+00000b20: 5345 2f43 6f72 7465 782d 5870 616e 7365  SE/Cortex-Xpanse
+00000b30: 2d41 5049 2d52 6566 6572 656e 6365 2f47  -API-Reference/G
+00000b40: 6574 2d53 7461 7274 6564 2d77 6974 682d  et-Started-with-
+00000b50: 4150 4973 223e 4765 7474 696e 6720 5374  APIs">Getting St
+00000b60: 6172 7465 643c 2f61 3e2e 0a0a 2323 2323  arted</a>...####
+00000b70: 2052 4543 4f4d 4d45 4e44 4544 0a2a 2a2a   RECOMMENDED.***
+00000b80: 2a2a 2a2a 2a2a 2a2a 0a59 6f75 2063 616e  ********.You can
+00000b90: 2073 7570 706c 7920 7468 656d 2061 7320   supply them as 
+00000ba0: 656e 7669 726f 6e6d 656e 7420 7661 7269  environment vari
+00000bb0: 6162 6c65 732e 0a0a 6060 6073 6865 6c6c  ables...```shell
+00000bc0: 2073 6372 6970 740a 6578 706f 7274 2043   script.export C
+00000bd0: 4f52 5445 585f 4651 444e 3d3c 596f 7572  ORTEX_FQDN=<Your
+00000be0: 2058 7061 6e73 6520 496e 7374 616e 6365   Xpanse Instance
+00000bf0: 2055 524c 3e0a 6578 706f 7274 2043 4f52   URL>.export COR
+00000c00: 5445 585f 4150 495f 4b45 593d 3c41 5049  TEX_API_KEY=<API
+00000c10: 204b 6579 3e0a 6578 706f 7274 2043 4f52   Key>.export COR
+00000c20: 5445 585f 4150 495f 4b45 595f 4944 3d3c  TEX_API_KEY_ID=<
+00000c30: 4150 4920 4b65 7920 4944 3e0a 6060 600a  API Key ID>.```.
+00000c40: 2020 2020 0a23 2323 2320 4e4f 5420 5245      .#### NOT RE
+00000c50: 434f 4d4d 454e 4445 440a 2a2a 2a2a 2a2a  COMMENDED.******
+00000c60: 2a2a 2a2a 2a2a 2a2a 2a0a 5468 6520 666f  *********.The fo
+00000c70: 6c6c 6f77 696e 6720 7061 7261 6d65 7465  llowing paramete
+00000c80: 7273 2063 616e 2062 6520 7365 7420 696e  rs can be set in
+00000c90: 6c69 6e65 2075 7369 6e67 2074 6865 2060  line using the `
+00000ca0: 5870 616e 7365 436c 6965 6e74 6020 636f  XpanseClient` co
+00000cb0: 6e73 7472 7563 746f 722e 0a0a 5f54 6869  nstructor..._Thi
+00000cc0: 7320 6973 206e 6f74 2072 6563 6f6d 6d65  s is not recomme
+00000cd0: 6e64 6564 2c20 6173 2069 7420 6561 7369  nded, as it easi
+00000ce0: 6c79 2065 7870 6f73 6573 2073 656e 7369  ly exposes sensi
+00000cf0: 7469 7665 2063 7265 6465 6e74 6961 6c73  tive credentials
+00000d00: 2069 6e20 796f 7572 2073 6f75 7263 6520   in your source 
+00000d10: 636f 6465 2e5f 200a 0a60 6060 7079 7468  code._ ..```pyth
+00000d20: 6f6e 0a23 2049 6d70 6f72 7420 636c 6965  on.# Import clie
+00000d30: 6e74 0a66 726f 6d20 7870 616e 7365 2e63  nt.from xpanse.c
+00000d40: 6c69 656e 7420 696d 706f 7274 2058 7061  lient import Xpa
+00000d50: 6e73 6543 6c69 656e 740a 0a23 2049 6e69  nseClient..# Ini
+00000d60: 7469 616c 697a 6520 636c 6965 6e74 202d  tialize client -
+00000d70: 2054 4849 5320 4953 204e 4f54 2052 4543   THIS IS NOT REC
+00000d80: 4f4d 4d45 4e44 4544 2c20 5345 5420 454e  OMMENDED, SET EN
+00000d90: 5649 524f 4e4d 454e 5420 5641 5249 4142  VIRONMENT VARIAB
+00000da0: 4c45 5320 494e 5354 4541 440a 636c 6965  LES INSTEAD.clie
+00000db0: 6e74 203d 2058 7061 6e73 6543 6c69 656e  nt = XpanseClien
+00000dc0: 7428 7572 6c3d 2268 7474 7073 3a2f 2f6d  t(url="https://m
+00000dd0: 792d 636f 6d70 616e 792e 6372 7478 2e75  y-company.crtx.u
+00000de0: 732e 7061 6c6f 616c 746f 6e65 7477 6f72  s.paloaltonetwor
+00000df0: 6b73 2e63 6f6d 222c 0a20 2020 2020 2020  ks.com",.       
+00000e00: 2020 2020 2020 2020 2020 2020 2020 2061                 a
+00000e10: 7069 5f6b 6579 3d22 7878 7878 7878 7878  pi_key="xxxxxxxx
+00000e20: 7878 7878 7878 7841 7069 4b65 7978 7878  xxxxxxxApiKeyxxx
+00000e30: 7878 7878 7878 7878 7878 7878 222c 0a20  xxxxxxxxxxxx",. 
+00000e40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000e50: 2020 2020 2061 7069 5f6b 6579 5f69 643d       api_key_id=
+00000e60: 3129 0a60 6060 0a0a 4c6f 6767 696e 670a  1).```..Logging.
+00000e70: 2d2d 2d2d 2d2d 2d0a 4c6f 6767 696e 6720  -------.Logging 
+00000e80: 6973 2068 616e 646c 6564 2074 6872 6f75  is handled throu
+00000e90: 6768 2074 6865 2070 7974 686f 6e20 6c6f  gh the python lo
+00000ea0: 6767 696e 6720 7061 636b 6167 652e 2054  gging package. T
+00000eb0: 6f20 656e 6162 6c65 2064 6966 6665 7265  o enable differe
+00000ec0: 6e74 206c 6576 656c 7320 6f66 2076 6572  nt levels of ver
+00000ed0: 626f 7369 7479 2069 6e20 796f 7572 2073  bosity in your s
+00000ee0: 6372 6970 7473 2079 6f75 2063 616e 2064  cripts you can d
+00000ef0: 6f20 7468 6520 666f 6c6c 6f77 696e 673a  o the following:
+00000f00: 0a0a 6060 6070 7974 686f 6e0a 696d 706f  ..```python.impo
+00000f10: 7274 206c 6f67 6769 6e67 0a0a 2320 5365  rt logging..# Se
+00000f20: 7420 7468 6520 6c6f 6767 696e 6720 6c65  t the logging le
+00000f30: 7665 6c0a 6c6f 6767 696e 672e 6261 7369  vel.logging.basi
+00000f40: 6343 6f6e 6669 6728 6c65 7665 6c3d 6c6f  cConfig(level=lo
+00000f50: 6767 696e 672e 4445 4255 4729 0a60 6060  gging.DEBUG).```
+00000f60: 0a0a 596f 7520 6361 6e20 7265 6164 206d  ..You can read m
+00000f70: 6f72 6520 6174 203c 6874 7470 733a 2f2f  ore at <https://
+00000f80: 646f 6373 2e70 7974 686f 6e2e 6f72 672f  docs.python.org/
+00000f90: 332f 6c69 6272 6172 792f 6c6f 6767 696e  3/library/loggin
+00000fa0: 672e 6874 6d6c 3e2e 0a0a 0a              g.html>....
```

### Comparing `xpanse-1.3.1/README.md` & `xpanse-2.0.0rc3/docs/_source/cover.rst`

 * *Files 20% similar despite different names*

```diff
@@ -1,95 +1,83 @@
-Xpanse Python SDK
-==================
-.. image:: https://github.com/PaloAltoNetworks/cortex-xpanse-python-sdk/blob/main/docs/_source/_static/xpanse_banner.png?raw=true
-   :width: 800
+Cortex Xpanse Python SDK
+========================
+.. image:: _static/xpanse_banner.png
+   :width: 600
    :target: https://expanse.co/
 
-.. image:: https://img.shields.io/badge/code%20style-black-000000.svg
-   :target: https://github.com/psf/black
-
-.. image:: https://img.shields.io/badge/python-3.6%20%7C%203.7%20%7C%203.8-blueviolet
-   :target: https://pypi.python.org/pypi/xpanse
-
-.. image:: https://img.shields.io/badge/code%20style-black-000000.svg
-   :target: https://github.com/psf/black
-
-.. image:: https://img.shields.io/pypi/l/xpanse
-   :target: https://github.com/PaloAltoNetworks/cortex-xpanse-python-sdk/blob/main/LICENSE
-
-.. image:: https://img.shields.io/github/contributors/PaloAltoNetworks/cortex-xpanse-python-sdk
-   :target: https://github.com/PaloAltoNetworks/cortex-xpanse-python-sdk/graphs/contributors
-
 Overview
 --------
 
-This library is intended to be an interface to the `Xpanse Expander API <https://knowledgebase.xpanse.co/expander-apis/>`_.
+This library is intended to be an interface to the `Cortex Xpanse Public API <https://docs-cortex.paloaltonetworks.com/r/Cortex-XPANSE/Cortex-Xpanse-API-Reference>`_.
 
 Install
 -------
 .. code-block:: python
 
     pip install xpanse
 
+
 Requirements
 ------------
 
-Python 3.6+
+``Python 3.7+``
 
 Usage
 -----
-`Documentation <https://cortex-xpanse-python-sdk.readthedocs.io/en/latest/>`_
 
 .. code-block:: python
 
     # Import client
-    from xpanse.client import ExClient
+    from xpanse.client import XpanseClient
 
-    # initialize client
-    client = ExClient()
+    # Initialize client
+    client = XpanseClient()
 
-    # get ip_range iterator object and dump to a list
-    ranges = client.assets.ip_range.list().dump()
+    # Get assets iterator object and dump to a list
+    assets = client.assets.list().dump()
 
-You can view more example code in the `examples <https://github.com/PaloAltoNetworks/cortex-xpanse-python-sdk/tree/main/examples>`_ directory.
+You can view more example code in the `examples <https://github.com/PaloAltoNetworks/cortex-xpanse-python-sdk/tree/main/examples>`_.
 
 Configuration
 -------------
-A valid Client ID and Secret is required for use. This is recommended over using a JWT, as they have limited lifespans.
-While a bearer token is supported in this version, this auth flow is being deprecated. Therefore, it is highly recommended to use Client Credentials.
+A valid ``API Key``, ``API Key ID``, and ``Fully Qualified Domain Name (FQDN)`` are required for use.
 
-RECOMMENDED
-***********
-You can supply them as environment variables using the variable names ``XPANSE_CLIENT_ID`` AND ``XPANSE_CLIENT_SECRET``.
+Reference the docs for more information with `Getting Started <https://docs-cortex.paloaltonetworks.com/r/Cortex-XPANSE/Cortex-Xpanse-API-Reference/Get-Started-with-APIs>`_.
 
-.. code-block:: python
+**RECOMMENDED**
 
-    export XPANSE_CLIENT_ID=<Client ID>
-    export XPANSE_CLIENT_SECRET=<Client Secret>
-    
-NOT RECOMMENDED
-***************
-To use a short lived JWT, you can supply the JWT as an environmental variable using the name ``XPANSE_JWT_TOKEN``
+You can supply them as environment variables.
 
 .. code-block:: python
 
-    export XPANSE_JWT_TOKEN=<JWT>
+    export CORTEX_FQDN=<Your Xpanse Instance URL>
+    export CORTEX_API_KEY=<API Key>
+    export CORTEX_API_KEY_ID=<API Key ID>
+
+**NOT RECOMMENDED**
 
-[Deprecated]
-A valid Bearer token can be supplied as an environment variable
+The following parameters can be set inline using the ``XpanseClient`` constructor.
 
-To supply a valid bearer token as an environment variable, you can use the variable names ``XPANSE_BEARER_TOKEN``.
+*This is not recommended, as it easily exposes sensitive credentials in your source code.*
 
 .. code-block:: python
 
-    export XPANSE_BEARER_TOKEN=<Bearer Token>
+    # Import client
+    from xpanse.client import XpanseClient
+
+    # Initialize client - THIS IS NOT RECOMMENDED, SET ENVIRONMENT VARIABLES INSTEAD
+    client = XpanseClient(url="https://my-company.crtx.us.paloaltonetworks.com",
+                          api_key="xxxxxxxxxxxxxxxApiKeyxxxxxxxxxxxxxxx",
+                          api_key_id=1)
 
 Logging
 -------
 Logging is handled through the python logging package. To enable different levels of verbosity in your scripts you can do the following:
 
 .. code-block:: python
 
     import logging
+
+    # Set the logging level
     logging.basicConfig(level=logging.DEBUG)
 
-You can read more at `<https://docs.python.org/3/library/logging.html>`_.
+You can read more at `<https://docs.python.org/3/library/logging.html>`_.
```

### Comparing `xpanse-1.3.1/docs/_source/_static/xpanse_banner.png` & `xpanse-2.0.0rc3/docs/_source/_static/xpanse_banner.png`

 * *Files identical despite different names*

### Comparing `xpanse-1.3.1/docs/_source/conf.py` & `xpanse-2.0.0rc3/docs/_source/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,15 +73,15 @@
 add_module_names = False
 napoleon_google_docstring = True
 napoleon_numpy_docstring = False
 
 # -- Options for HTML output -------------------------------------------------
 
 html_theme_options = {
-    "description": "The Python interface to the Xpanse Expander API",
+    "description": "The Python interface to the Cortex Xpanse API",
     "fixed_sidebar": False,
     "logo": "xpanse_banner.png",
     "touch_icon": "xpanse_banner.png",
     "logo_name": "Xpanse",
 }
 
 # The theme to use for HTML and HTML Help pages.  See the documentation for
```

### Comparing `xpanse-1.3.1/docs/_source/xpanse.rst` & `xpanse-2.0.0rc3/docs/_source/xpanse.rst`

 * *Files 17% similar despite different names*

```diff
@@ -1,57 +1,77 @@
-Xpanse
-=======
+Cortex Xpanse Public API SDK
+============================
 
 Subpackages
 -----------
 
 .. toctree::
-    cover
-    xpanse.api
+   :maxdepth: 4
+
+   xpanse.api
+
+Submodules
+----------
 
 xpanse.client module
----------------------
+--------------------
 
 .. automodule:: xpanse.client
-    :members:
-    :undoc-members:
-    :show-inheritance:
+   :members:
+   :undoc-members:
+   :show-inheritance:
 
 xpanse.const module
---------------------
+-------------------
 
 .. automodule:: xpanse.const
-    :members:
-    :undoc-members:
-    :show-inheritance:
-
-xpanse.error module
----------------------
-
-.. automodule:: xpanse.error
-    :members:
-    :undoc-members:
-    :show-inheritance:
+   :members:
+   :undoc-members:
+   :show-inheritance:
 
 xpanse.endpoint module
------------------------
+----------------------
 
 .. automodule:: xpanse.endpoint
-    :members:
-    :undoc-members:
-    :show-inheritance:
+   :members:
+   :undoc-members:
+   :show-inheritance:
+
+xpanse.error module
+-------------------
+
+.. automodule:: xpanse.error
+   :members:
+   :undoc-members:
+   :show-inheritance:
 
 xpanse.iterator module
------------------------
+----------------------
 
 .. automodule:: xpanse.iterator
-    :members:
-    :undoc-members:
-    :show-inheritance:
+   :members:
+   :undoc-members:
+   :show-inheritance:
+
+xpanse.response module
+----------------------
+
+.. automodule:: xpanse.response
+   :members:
+   :undoc-members:
+   :show-inheritance:
+
+xpanse.types module
+-------------------
+
+.. automodule:: xpanse.types
+   :members:
+   :undoc-members:
+   :show-inheritance:
 
 xpanse.utils module
---------------------
+-------------------
 
 .. automodule:: xpanse.utils
-    :members:
-    :undoc-members:
-    :show-inheritance:
+   :members:
+   :undoc-members:
+   :show-inheritance:
```

### Comparing `xpanse-1.3.1/docs/requirements-docs.txt` & `xpanse-2.0.0rc3/docs/requirements-docs.txt`

 * *Files 18% similar despite different names*

```diff
@@ -24,9 +24,9 @@
 sphinx==3.1.2
 sphinxcontrib-applehelp==1.0.2
 sphinxcontrib-devhelp==1.0.2
 sphinxcontrib-htmlhelp==1.0.3
 sphinxcontrib-jsmath==1.0.1
 sphinxcontrib-qthelp==1.0.3
 sphinxcontrib-serializinghtml==1.1.4
-typing-extensions==3.7.4.2
+typing_extensions==4.5.0
 urllib3~=1.26.6
```

### Comparing `xpanse-1.3.1/setup.py` & `xpanse-2.0.0rc3/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,35 +4,37 @@
 from xpanse import __version__, __license__, __author__, __email__
 
 try:
     description = open(
         os.path.join(os.path.abspath(os.path.dirname(__file__)), "README.md")
     ).read()
 except:
-    description = "Please refer to https://knowledgebase.expanse.co/expander-apis/"
+    description = "Please refer to https://docs-cortex.paloaltonetworks.com/r/Cortex-XPANSE/Cortex-Xpanse-API-Reference"
     print("! could not read README.md file.")
 
 setup(
     name="xpanse",
     version=__version__,
-    description="Python library is an interface to the Xpanse Expander API.",
+    description="Python library is an interface to the Cortex Xpanse API.",
     author=__author__,
     long_description=description,
+    long_description_content_type="text/markdown",
     author_email=__email__,
     license=__license__,
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Topic :: Software Development",
         "Topic :: Software Development :: Libraries",
         "Topic :: Software Development :: Libraries :: Application Frameworks",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
     ],
     keywords="xpanse iom",
     packages=["docs", "examples", *find_packages(exclude=["tests"])],
-    install_requires=["requests>=2.25.1", "deprecated>=1.2.0"],
+    install_requires=["requests>=2.25.1", "deprecated>=1.2.0", "typing_extensions>=4.5.0"],
     include_package_data=True,
-    python_requires=">=3.6",
+    python_requires=">=3.7",
 )
```

### Comparing `xpanse-1.3.1/xpanse/api/services/__init__.py` & `xpanse-2.0.0rc3/xpanse/api/asset_management/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,57 +1,42 @@
-from xpanse.base_api import ExApi
-from xpanse.api.services.v1.classifications import ClassificationsEndpoint
-from xpanse.api.services.v1.country_codes import CountryCodesEndpoint
-from xpanse.api.services.v1.services import ServicesEndpoint
+from xpanse.api.asset_management.v1.assets import AssetsEndpoint
+from xpanse.api.asset_management.v1.owned_ip_ranges import OwnedIpRangesEndpoint
+from xpanse.api.asset_management.v1.services import ServicesEndpoint
 
 
-class ClassificationsAPI(ExApi, ClassificationsEndpoint):
+class AssetsApi(AssetsEndpoint):
     def __init__(self, session):
         super().__init__(session)
 
     @property
     def current_version(self):
         return "v1"
 
     @property
     def v1(self):
-        return ClassificationsEndpoint(self._api)
+        return AssetsEndpoint(self._api)
 
 
-class CountryCodesAPI(ExApi, CountryCodesEndpoint):
+class OwnedIpRangesApi(OwnedIpRangesEndpoint):
     def __init__(self, session):
         super().__init__(session)
 
     @property
     def current_version(self):
         return "v1"
 
     @property
     def v1(self):
-        return CountryCodesEndpoint(self._api)
+        return OwnedIpRangesEndpoint(self._api)
 
 
-class ServicesAPI(ExApi, ServicesEndpoint):
+class ServicesApi(ServicesEndpoint):
     def __init__(self, session):
         super().__init__(session)
 
     @property
     def current_version(self):
         return "v1"
 
     @property
     def v1(self):
         return ServicesEndpoint(self._api)
-
-
-class ServicesApi(ExApi):
-    @property
-    def classifications(self):
-        return ClassificationsAPI(self._api)
-
-    @property
-    def country_codes(self):
-        return CountryCodesAPI(self._api)
-
-    @property
-    def services(self):
-        return ServicesAPI(self._api)
```

### Comparing `xpanse-1.3.1/xpanse/client.py` & `xpanse-2.0.0rc3/xpanse/client.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,111 +1,96 @@
+import hashlib
 import logging
 import os
 import platform
-from typing import Any, List, MutableMapping, Optional
+import secrets
+import string
 import sys
-import json
+from datetime import datetime, timezone
+from typing import Any, List, Optional, Union, MutableMapping
+from urllib.parse import urlparse
 
 import requests
 from requests.exceptions import ConnectionError
 from urllib3.exceptions import NewConnectionError
 
 from . import __version__
 from xpanse.const import (
-    XPANSE_BEARER_TOKEN,
-    XPANSE_JWT_TOKEN,
     HTTPVerb,
-    ID_TOKEN_URL,
-    XPANSE_CLIENT_ID,
-    XPANSE_CLIENT_SECRET,
-    CLIENT_CREDENTIALS_SCOPE,
-    CLIENT_CREDENTIALS_GRANT_TYPE,
-    CLIENT_CREDENTIALS_TOKEN_URL,
+    CORTEX_FQDN,
+    CORTEX_API_KEY,
+    CORTEX_API_KEY_ID,
 )
 from xpanse.error import (
-    UnexpectedValueError,
-    JWTExpiredError,
     XpanseException,
+    InvalidApiCredentials,
 )
-from xpanse.api.annotations import AnnotationsApi
-from xpanse.api.assets import AssetsApi
-from xpanse.api.behavior import BehaviorApi
-from xpanse.api.entities import EntitiesApi
-from xpanse.api.issues import IssuesApi
-from xpanse.api.services import ServicesApi
-from xpanse.api.targeted_ips import TargetedIPsApi
-from xpanse.api.connectors import ConnectorsApi
+
 from xpanse.utils import normalize_param_names
+from xpanse.api.asset_management import ServicesApi, OwnedIpRangesApi, AssetsApi
+from xpanse.api.attack_surface_rules import AttackSurfaceRulesApi
+from xpanse.api.incident_management import AlertsApi, IncidentsApi
+from xpanse.api.tags import TagsApi
 
 
-class ExClient:
+class XpanseClient:
     """
-    Interface for Xpanse APIs.
+    Interface for Cortex Xpanse APIs.
 
     Args:
-        panw_url (str, optional):
-            The URL that the auth will go through.  The default
-            is ``https://api.paloaltonetworks.com``
-        url (str, optional):
-            The base URL that the paths will be appended onto.  The default
-            is ``https://api.expander.expanse.co``
-        client_id (str, optional):
-            The Client ID for the Xpanse API, which is used to request emphemeral JWT tokens.
-            More details at ``https://knowledgebase.expanse.co/expander-apis/#getting``
-        client_secret (str, optional):
-            The Client Secret for the Xpanse API, which is used to request emphemeral JWT tokens.
-            More details at ``https://knowledgebase.expanse.co/expander-apis/#getting``
-        bearer_token (str, optional):
-            The Bearer token for the Xpanse API, which is used to request emphemeral JWT tokens.
-            More details at ``https://knowledgebase.expanse.co/expander-apis/#getting``
-        jwt (str, optional):
-            The JWT for the Xpanse API. Note JWTs are temporary so they are not intended for use
-            with long-running applications.
-            More details at ``https://knowledgebase.expanse.co/expander-apis/#getting``
+        url (str, required):
+            The base URL that the paths will be appended onto. This field is required to be set either during
+            instantiation, or using the environment variable `CORTEX_FQDN`.
+        api_key_id (Union[str, int], required):
+            The API Key ID associated with the generated credentials. This can be located after generating
+            the credentials in the API Keys table under the 'ID' column. i.e. 1, 2, 3, etc. This field is required
+            to be set either during instantiation, or using the environment variable `CORTEX_API_KEY_ID`.
+        api_key (str, required):
+            The API Key generated when provisioning the credentials in your product. It is recommended that
+            the API Key defaults are kept (i.e. using Advanced keys). This field is required to be set either during
+            instantiation, or using the environment variable `CORTEX_API_KEY`.
+        use_advanced_auth (bool, optional):
+            A flag used to determine which type of API Key is being used. 'Advanced' is used when True,
+            'Standard' is used when False. This is configured when generating your API Keys is in the product.
+            The default is True.
+            See: https://docs-cortex.paloaltonetworks.com/r/Cortex-XPANSE/Cortex-Xpanse-API-Reference/Get-Started-with-APIs
         custom_ua (str, optional):
             A custom string can be provided that will be sent within the user-agent header on all
             requests to Xpanse. Final format will be `Xpanse SDK+<custom_ua>/__version__ ...`
-        proxies (dict, optional):
+        proxies (MutableMapping[str, str], optional):
             A dictionary detailing what proxy should be used for what transport protocol.
             This value will be passed to the session object after it has been either attached or
             created. For details on the structure of this dictionary, consult the
             :requests:`proxies <user/advanced/#proxies>` section of the Requests documentation.
         verify (bool, optional):
             Whether or not SSL verification should occur. This is `True` by default. Disabling certificate
             verification is strongly discouraged.
             See: https://urllib3.readthedocs.io/en/latest/advanced-usage.html#ssl-warnings InsecureRequestWarning
     """
 
-    """Xpanse URL"""
-    _url: str = "https://api.expander.expanse.co"
-
-    """Authentication URL for retrieving JWTs via Client Credentials"""
-    _panw_url: str = "https://api.paloaltonetworks.com"
-
-    """Client ID"""
-    _client_id: Optional[str] = None
+    """Xpanse URL - Default is set by the CORTEX_FQDN_URL environment variable"""
+    _url: str
 
-    """Client Secret"""
-    _client_secret: Optional[str] = None
+    """Public API Key ID"""
+    _api_key_id: str
 
-    """Bearer Token"""
-    _bt: Optional[str] = None
+    """Public API Key"""
+    _api_key: str
 
-    """JWT"""
-    _jwt: Optional[str] = None
+    """Uses a nonce and timestamp when true.
+       See: https://docs-cortex.paloaltonetworks.com/r/Cortex-XPANSE/Cortex-Xpanse-API-Reference/Get-Started-with-APIs
+    """
+    _use_advanced_auth: bool = True
 
     """Proxies"""
-    _proxies: Optional[str] = None
+    _proxies: Optional[MutableMapping[str, str]] = None
 
     """Verify SSL"""
     _verify = True
 
-    """JWT is valid"""
-    _jwt_valid: bool = False
-
     """Max Retry Count"""
     _max_retries: int = 1
 
     """Error Codes to Retry"""
     _retry_error_codes: List[int] = [503]
 
     """Vendor Name for UA"""
@@ -126,242 +111,185 @@
     """Active Session"""
     _session: requests.Session = requests.Session()
 
     """Class Methods"""
 
     def __init__(
         self,
-        url=None,
-        panw_url=None,
-        client_id=None,
-        client_secret=None,
-        bearer_token=None,
-        jwt=None,
-        custom_ua=None,
-        proxies=None,
-        verify=True,
+        url: Optional[str] = None,
+        api_key_id: Optional[Union[str, int]] = None,
+        api_key: Optional[str] = None,
+        use_advanced_auth: bool = True,
+        custom_ua: Optional[str] = None,
+        proxies: Optional[MutableMapping[str, str]] = None,
+        verify: bool = True,
     ):
-
         # Format logger
         self._log = logging.getLogger(
             "{}.{}".format(self.__module__, self.__class__.__name__)
         )
 
         # Get install details
         self._set_os()
         self._set_current_python_version()
 
         # If a custom UA product is desired, include that
         if custom_ua is not None:
             self._product += f"+{custom_ua}"
 
-        # Configure URL and Auth tokens
+        # Configure URL
+        env_url = os.getenv(CORTEX_FQDN)
         if url is not None:
             self._url = url
-
-        if panw_url is not None:
-            self._panw_url = panw_url
-
-        if client_id is not None and client_secret is not None:
-            self._client_id = client_id
-            self._client_secret = client_secret
-            self._auth_url = f"{self._panw_url}/{CLIENT_CREDENTIALS_TOKEN_URL}"
+        elif env_url is not None:
+            self._url = env_url
         else:
-            self._client_id = os.environ.get(XPANSE_CLIENT_ID, None)
-            self._client_secret = os.environ.get(XPANSE_CLIENT_SECRET, None)
+            raise ValueError(
+                "A 'url' must be provided. Set the 'url' client parameter or set the 'CORTEX_FQDN' "
+                "environment variable."
+            )
+
+        if not self._url.startswith("http"):
+            self._url = f"https://{self._url}"
 
-        if bearer_token is not None:
-            self._bt = bearer_token
-            self._auth_url = f"{self._url}/{ID_TOKEN_URL}"
+        host = urlparse(self._url).netloc
+        if host.startswith("api-"):
+            self._url = f"https://{host}"
         else:
-            self._bt = os.environ.get(XPANSE_BEARER_TOKEN, None)
+            self._url = f"https://api-{host}"
 
-        if proxies is not None:
-            self._proxies = proxies
+        # Configure Auth Session
+        self._proxies = proxies
 
         if isinstance(verify, bool):
             self._verify = verify
 
-        if jwt is not None:
-            self._jwt = jwt
-            self._jwt_valid = True
-        else:
-            env_jwt = os.environ.get(XPANSE_JWT_TOKEN, None)
-            if env_jwt is not None:
-                self._jwt = env_jwt
-                self._jwt_valid = True
-            else:
-                self._refresh_jwt()
+        if isinstance(use_advanced_auth, bool):
+            self._use_advanced_auth = use_advanced_auth
+        if not self._use_advanced_auth:
+            self._log.warning(
+                "'Advanced Authentication' is disabled, your requests may be vulnerable to replay attacks. "
+                "See https://docs-cortex.paloaltonetworks.com/r/Cortex-XPANSE/Cortex-Xpanse-API-Reference/Get-Started-with-APIs "
+                "for more information."
+            )
 
-        self._setup_auth()
+        self._setup_auth(api_key=api_key, api_key_id=api_key_id)
 
-        # create Session
-        self._create_session()
-
-    def _setup_auth(self):
+    def _setup_auth(
+        self, api_key: Optional[str], api_key_id: Optional[Union[str, int]]
+    ):
         """
         Check for a valid set of authentication inputs. This can be one of the following (in order of priority):
-        1. Client ID & Client Secret (needs both)
-        2. Bearer token (being deprecated)
-        3. JWT
-        """
-        if (
-            not self._bt
-            and not self._jwt_valid
-            and not self._client_id
-            and not self._client_secret
-        ):
-            raise UnexpectedValueError(
-                "A valid Xpanse Client credentials, Bearer token, or JWT token is required."
-            )
-        elif (self._client_id and not self._client_secret) or (
-            self._client_secret and not self._client_id
-        ):
-            raise UnexpectedValueError(
-                "A valid set of Xpanse Client credentials is required."
-            )
-        elif self._client_id and self._client_secret:
-            logging.debug("Using Client credential flow")
-        elif self._bt:
-            logging.warning(
-                "Bearer Token will be deprecated in a coming release of the Xpanse SDK"
-            )
-        else:
-            logging.error("We shouldn't get to this log line, something went wrong")
+            1. Setting api_key_id and api_key from the XpanseClient constructor
+            2. Setting the CORTEX_API_KEY_ID and CORTEX_API_KEY environment variables
 
-    def _refresh_jwt(self, is_retry: bool = False):
-        """
-        Refreshes JWT using Bearer token.
-        """
-        if self._client_id and self._client_secret:
-            self._refresh_client_credentials_jwt(is_retry)
-        elif self._bt is not None:
-            self._refresh_bearer_token_jwt(is_retry)
+        Args:
+            api_key (str, Optional):
+                The api_key provided from the constructor
+            api_key_id (str, Optional):
+                The api_key_id provided from the constructor
+        """
+        if api_key is not None:
+            self._api_key = api_key
+        elif os.getenv(CORTEX_API_KEY) is not None:
+            self._api_key = str(os.getenv(CORTEX_API_KEY))
         else:
-            raise UnexpectedValueError(
-                "A valid Xpanse Bearer token or client credentials is required."
+            raise ValueError(
+                "An 'api_key' must be provided. Set the 'api_key' parameter or set the 'CORTEX_API_KEY' "
+                "environment variable."
             )
 
-    def _refresh_client_credentials_jwt(self, is_retry):
-        try:
-            data = json.dumps(
-                {
-                    "client_id": self._client_id,
-                    "client_secret": self._client_secret,
-                    "grant_type": CLIENT_CREDENTIALS_GRANT_TYPE,
-                    "scope": CLIENT_CREDENTIALS_SCOPE,
-                }
+        if api_key_id is not None:
+            self._api_key_id = str(api_key_id)
+        elif os.getenv(CORTEX_API_KEY_ID) is not None:
+            self._api_key_id = str(os.getenv(CORTEX_API_KEY_ID))
+        else:
+            raise ValueError(
+                "An 'api_key_id' must be provided. Set the 'api_key_id' parameter or set the "
+                "'CORTEX_API_KEY_ID' environment variable."
             )
-            resp = requests.post(
-                self._auth_url,
-                headers={
-                    "Content-Type": "application/json",
-                },
-                data=data,
-                timeout=30,
-                proxies=self._proxies,
-                verify=self._verify,
+
+        self._create_session()
+
+        if not self._validate_auth():
+            key_type = "Advanced" if self._use_advanced_auth else "Standard"
+            raise InvalidApiCredentials(
+                "Failed to authenticate with the provided 'api_key' and 'api_key_id' using "
+                f"'{key_type}' authentication."
             )
-            if resp.status_code != 200:
-                raise UnexpectedValueError(
-                    f"API returned an error while refreshing JWT with client credentials: {resp.text}"
-                )
-            else:
-                self._jwt_valid = True
-                self._jwt = resp.json()["access_token"]
-        except ConnectionError as request_exception:
-            if is_retry:
-                raise UnexpectedValueError(
-                    "Request returned an exception"
-                ) from request_exception
-            logging.warn(f"ConnectionError encountered during JWT refresh, will retry.")
-            self._refresh_jwt(is_retry=True)
-        except requests.RequestException as request_exception:
-            raise UnexpectedValueError(
-                "Request returned an exception"
-            ) from request_exception
-
-    def _refresh_bearer_token_jwt(self, is_retry):
-        try:
-            resp = requests.get(
-                self._auth_url,
-                headers={
-                    "Authorization": f"Bearer {self._bt}",
-                    "Content-Type": "application/json",
-                },
-                timeout=30,
-                proxies=self._proxies,
-                verify=self._verify,
-            ).json()
-            if "error" in resp or "token" not in resp:
-                raise UnexpectedValueError(
-                    f"API returned an error while refreshing JWT: {resp['error']}"
-                )
-            else:
-                self._jwt_valid = True
-                self._jwt = resp["token"]
-        except ConnectionError as request_exception:
-            if is_retry:
-                raise UnexpectedValueError(
-                    "Request returned an exception"
-                ) from request_exception
-            logging.warn(f"ConnectionError encountered during JWT refresh, will retry.")
-            self._refresh_jwt(is_retry=True)
-        except requests.RequestException as request_exception:
-            raise UnexpectedValueError(
-                "Request returned an exception"
-            ) from request_exception
 
-    def _create_session(self, session: Optional[Any] = None):
+    def _validate_auth(self) -> bool:
         """
-        Add JWT auth to session.
+        Validates the provided API Keys
+
+        Returns:
+            :bool: True when the keys are valid, False when the keys are invalid or expired.
         """
-        if session is not None:
-            self._session = session
-        self._session = requests.Session()
-        self._session.headers.update(
-            {
-                "User-Agent": self._generate_user_agent(),
-                "Content-Type": "application/json",
-                "Authorization": f"Bearer {self._jwt}",
-            }
-        )
+        res = self.post("api_keys/validate/")
 
-        if self._proxies is not None:
-            self._session.proxies.update(self._proxies)  # type: ignore
+        if res is None or res.status_code == 401:
+            return False
 
-        self._session.verify = self._verify
+        return res.json()
 
-    def _refresh_session(self):
+    def _get_auth_headers(self) -> dict:
         """
-        Refresh JWT auth if the old token expires.
+        Generates authorization headers for both Standard and Advanced API Keys
+
+        Returns:
+            :dict: Authorization headers
         """
-        if not self._bt and not self._client_id and not self._client_secret:
-            raise UnexpectedValueError(
-                "No valid Xpanse Bearer token or client credential was found."
+        if self._use_advanced_auth:
+            # Generate a 64 bytes random string
+            nonce = "".join(
+                [
+                    secrets.choice(string.ascii_letters + string.digits)
+                    for _ in range(64)
+                ]
             )
-        self._refresh_jwt()
-        self._session.headers.update({"Authorization": f"Bearer {self._jwt}"})
+            # Get the current timestamp as milliseconds.
+            timestamp = int(datetime.now(timezone.utc).timestamp()) * 1000
+            # Generate the auth key
+            auth_key = "%s%s%s" % (self._api_key, nonce, timestamp)
+            # Convert to bytes object
+            auth_key_bytes = auth_key.encode("utf-8")
+            # Calculate sha256:
+            api_key_hash = hashlib.sha256(auth_key_bytes).hexdigest()
+            return {
+                "x-xdr-timestamp": str(timestamp),
+                "x-xdr-nonce": nonce,
+                "x-xdr-auth-id": str(self._api_key_id),
+                "Authorization": api_key_hash,
+            }
+        else:
+            return {
+                "x-xdr-auth-id": str(self._api_key_id),
+                "Authorization": self._api_key,
+            }
 
-    def _check_response_for_invalid_session(self, resp: requests.Response) -> bool:
+    def _refresh_auth(self):
         """
-        Check response for expired JWT.
+        Refresh auth in session.
         """
-        if resp.status_code == 401:
-            try:
-                resp_json = resp.json()
-                if (
-                    "detail" in resp_json
-                    and "Signature has expired." in resp_json["detail"]
-                ):
-                    return True
-            except ValueError:
-                # Some 401 responses are returned without a body
-                pass
-        return False
+        self._session.headers.pop("x-xdr-timestamp", None)
+        self._session.headers.pop("x-xdr-nonce", None)
+        self._session.headers.update(self._get_auth_headers())
+
+    def _create_session(self):
+        """
+        Creates a request session with auth.
+        """
+        self._session = requests.Session()
+
+        if self._proxies is not None:
+            self._session.proxies.update(self._proxies)
+
+        self._session.verify = self._verify
+
+        self._session.headers.update(self._get_auth_headers())
 
     def _set_current_python_version(self):
         """
         Get current installed python version.
         """
         self._python_version = ".".join([str(i) for i in sys.version_info][0:3])
 
@@ -382,59 +310,43 @@
     ) -> Optional[requests.Response]:
         """
         Request builder.
         """
         retries = 0
         while retries <= self._max_retries:
             try:
+                if self._use_advanced_auth:
+                    self._refresh_auth()
+
                 kwargs = normalize_param_names(kwargs)
                 self._log.debug(
                     f"REQUEST TO: {method} {self._url}/{path} WITH PAYLOAD: {kwargs}"
                 )
                 resp = self._session.request(method, f"{self._url}/{path}", **kwargs)
                 if resp.status_code < 400:
                     return resp
                 else:
-                    if self._check_response_for_invalid_session(resp):
-                        # JWT has expired, try to generare a new one if a bearer token exists
-                        # and retry the request without incrementing our retry counter.
-                        if self._bt is not None or (
-                            self._client_id is not None
-                            and self._client_secret is not None
-                        ):
-                            self._refresh_session()
-                            continue
-                        else:
-                            raise JWTExpiredError("JWT has expired", resp)
+                    if resp.status_code in self._retry_error_codes:
+                        retries += 1
+                        continue
                     else:
-                        if resp.status_code in self._retry_error_codes:
-                            retries += 1
-                            continue
-                        else:
-                            self._log.error(f"Error response: {resp.text}")
-                            return resp
+                        self._log.error(f"Error response: {resp.text}")
+                        return resp
             except (
                 ConnectionError,
                 NewConnectionError,
             ) as err:
                 self._log.error(err)
                 retries += 1
                 continue
             except XpanseException as err:
                 self._log.error(err)
                 break
         return None
 
-    def direct_get(self, url: str, **kwargs: Any) -> Optional[requests.Response]:
-        """
-        Fetches direct without url formatting.
-        """
-        resp = self._session.request(HTTPVerb.HTTP_GET.value, url, **kwargs)
-        return resp
-
     def get(self, path: str, **kwargs: Any) -> Optional[requests.Response]:
         """
         Initiates an HTTP GET request using the specified path.  Refer to
         :obj:`requests.request` for more detailed information on what
         keyword arguments can be passed:
 
         Args:
@@ -518,92 +430,45 @@
 
         Returns:
             :obj:`requests.Response`
 
         """
         return self._request(HTTPVerb.HTTP_DELETE.value, path)
 
-    def csv(self, path: str, file_: str, **kwargs: Any) -> bool:
-        """
-        Initiates an HTTP GET request using the specified path with special handling
-        for downloading a csv file. Refer to :obj:`requests.request` for more detailed
-        information on what keyword arguments can be passed:
-
-        Args:
-            path (str):
-                The path to be appended onto the base URL for the request.
-            file_ (str):
-                The file name with path where the resulting csv file should be saved.
-            **kwargs (dict):
-                Keyword arguments to be passed to the Requests Sessions request
-                method.
-
-        Returns:
-            :obj:`boolean`:
-                `True` if the download was successful, otherwise `False`.
-        """
-        try:
-            with requests.Session() as s:
-                s.headers.update(
-                    {
-                        "User-Agent": self._generate_user_agent(),
-                        "Accept": "text/csv",
-                        "Authorization": f"Bearer {self._jwt}",
-                    }
-                )
-                resp = s.get(f"{self._url}/{path}", params=kwargs, stream=True)
-                if resp.status_code < 400:
-                    with open(file_, "wb") as f:
-                        for chunk in resp.iter_content(1024 * 1024):
-                            f.write(chunk)
-                            self._log.debug(f"Writing {path} output to {file_}")
-                    return True
-                else:
-                    self._log.error(f"Error response: {resp.text}")
-                    return False
-        except requests.exceptions.RequestException:
-            self._log.exception(f"Error response")
-            return False
-
     ############################################
     # API Definitions
     ###########################################
 
     @property
-    def annotations(self):
-        """Annotations API"""
-        return AnnotationsApi(self)
-
-    @property
     def assets(self):
         """Assets API"""
         return AssetsApi(self)
 
     @property
-    def behavior(self):
-        """Behavior API"""
-        return BehaviorApi(self)
+    def owned_ip_ranges(self):
+        """Owned IP Ranges API"""
+        return OwnedIpRangesApi(self)
 
     @property
-    def entities(self):
-        """Entities API"""
-        return EntitiesApi(self)
+    def services(self):
+        """Services API"""
+        return ServicesApi(self)
 
     @property
-    def issues(self):
-        """Issues API"""
-        return IssuesApi(self)
+    def attack_surface_rules(self):
+        """Attack Surface Rules API"""
+        return AttackSurfaceRulesApi(self)
 
     @property
-    def services(self):
-        """Services API"""
-        return ServicesApi(self)
+    def incidents(self):
+        """Incidents API"""
+        return IncidentsApi(self)
 
     @property
-    def targeted_ips(self):
-        """Targeted IPs API"""
-        return TargetedIPsApi(self)
+    def alerts(self):
+        """Alerts V2 API"""
+        return AlertsApi(self)
 
     @property
-    def connectors(self):
-        """Connectors API"""
-        return ConnectorsApi(self)
+    def tags(self):
+        """Tags API"""
+        return TagsApi(self)
```

### Comparing `xpanse-1.3.1/xpanse/error.py` & `xpanse-2.0.0rc3/xpanse/error.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import logging
-from typing import Optional
 
 from requests import Response
 
 
 class XpanseException(Exception):
     """
     Base exception class.
@@ -37,13 +36,13 @@
     """
     Response from the server was unexpected and requires further investigation.
     """
 
     pass
 
 
-class JWTExpiredError(XpanseException):
+class InvalidApiCredentials(XpanseException):
     """
-    JWT has expired.
+    Thrown when credentials are invalid and need to be rotated.
     """
 
     pass
```

### Comparing `xpanse-1.3.1/xpanse.egg-info/PKG-INFO` & `xpanse-2.0.0rc3/xpanse.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,236 +1,251 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 7870 616e  : 2.1.Name: xpan
-00000020: 7365 0a56 6572 7369 6f6e 3a20 312e 332e  se.Version: 1.3.
-00000030: 310a 5375 6d6d 6172 793a 2050 7974 686f  1.Summary: Pytho
-00000040: 6e20 6c69 6272 6172 7920 6973 2061 6e20  n library is an 
-00000050: 696e 7465 7266 6163 6520 746f 2074 6865  interface to the
-00000060: 2058 7061 6e73 6520 4578 7061 6e64 6572   Xpanse Expander
-00000070: 2041 5049 2e0a 486f 6d65 2d70 6167 653a   API..Home-page:
-00000080: 2055 4e4b 4e4f 574e 0a41 7574 686f 723a   UNKNOWN.Author:
-00000090: 2050 616c 6f20 416c 746f 2043 6f72 7465   Palo Alto Corte
-000000a0: 7820 5870 616e 7365 0a41 7574 686f 722d  x Xpanse.Author-
-000000b0: 656d 6169 6c3a 2078 7061 6e73 652d 696e  email: xpanse-in
-000000c0: 7465 6772 6174 696f 6e73 4070 616c 6f61  tegrations@paloa
-000000d0: 6c74 6f6e 6574 776f 726b 732e 636f 6d0a  ltonetworks.com.
-000000e0: 4c69 6365 6e73 653a 2049 5343 0a4b 6579  License: ISC.Key
-000000f0: 776f 7264 733a 2078 7061 6e73 6520 696f  words: xpanse io
-00000100: 6d0a 506c 6174 666f 726d 3a20 554e 4b4e  m.Platform: UNKN
-00000110: 4f57 4e0a 436c 6173 7369 6669 6572 3a20  OWN.Classifier: 
-00000120: 4465 7665 6c6f 706d 656e 7420 5374 6174  Development Stat
-00000130: 7573 203a 3a20 3520 2d20 5072 6f64 7563  us :: 5 - Produc
-00000140: 7469 6f6e 2f53 7461 626c 650a 436c 6173  tion/Stable.Clas
-00000150: 7369 6669 6572 3a20 496e 7465 6e64 6564  sifier: Intended
-00000160: 2041 7564 6965 6e63 6520 3a3a 2044 6576   Audience :: Dev
-00000170: 656c 6f70 6572 730a 436c 6173 7369 6669  elopers.Classifi
-00000180: 6572 3a20 546f 7069 6320 3a3a 2053 6f66  er: Topic :: Sof
-00000190: 7477 6172 6520 4465 7665 6c6f 706d 656e  tware Developmen
-000001a0: 740a 436c 6173 7369 6669 6572 3a20 546f  t.Classifier: To
-000001b0: 7069 6320 3a3a 2053 6f66 7477 6172 6520  pic :: Software 
-000001c0: 4465 7665 6c6f 706d 656e 7420 3a3a 204c  Development :: L
-000001d0: 6962 7261 7269 6573 0a43 6c61 7373 6966  ibraries.Classif
-000001e0: 6965 723a 2054 6f70 6963 203a 3a20 536f  ier: Topic :: So
-000001f0: 6674 7761 7265 2044 6576 656c 6f70 6d65  ftware Developme
-00000200: 6e74 203a 3a20 4c69 6272 6172 6965 7320  nt :: Libraries 
-00000210: 3a3a 2041 7070 6c69 6361 7469 6f6e 2046  :: Application F
-00000220: 7261 6d65 776f 726b 730a 436c 6173 7369  rameworks.Classi
-00000230: 6669 6572 3a20 5072 6f67 7261 6d6d 696e  fier: Programmin
-00000240: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
-00000250: 7468 6f6e 203a 3a20 330a 436c 6173 7369  thon :: 3.Classi
-00000260: 6669 6572 3a20 5072 6f67 7261 6d6d 696e  fier: Programmin
-00000270: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
-00000280: 7468 6f6e 203a 3a20 332e 360a 436c 6173  thon :: 3.6.Clas
-00000290: 7369 6669 6572 3a20 5072 6f67 7261 6d6d  sifier: Programm
-000002a0: 696e 6720 4c61 6e67 7561 6765 203a 3a20  ing Language :: 
-000002b0: 5079 7468 6f6e 203a 3a20 332e 370a 436c  Python :: 3.7.Cl
-000002c0: 6173 7369 6669 6572 3a20 5072 6f67 7261  assifier: Progra
-000002d0: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
-000002e0: 3a20 5079 7468 6f6e 203a 3a20 332e 380a  : Python :: 3.8.
-000002f0: 5265 7175 6972 6573 2d50 7974 686f 6e3a  Requires-Python:
-00000300: 203e 3d33 2e36 0a4c 6963 656e 7365 2d46   >=3.6.License-F
-00000310: 696c 653a 204c 4943 454e 5345 0a0a 5870  ile: LICENSE..Xp
-00000320: 616e 7365 2050 7974 686f 6e20 5344 4b0a  anse Python SDK.
-00000330: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00000340: 3d3d 0a2e 2e20 696d 6167 653a 3a20 6874  ==... image:: ht
-00000350: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00000360: 2f50 616c 6f41 6c74 6f4e 6574 776f 726b  /PaloAltoNetwork
-00000370: 732f 636f 7274 6578 2d78 7061 6e73 652d  s/cortex-xpanse-
-00000380: 7079 7468 6f6e 2d73 646b 2f62 6c6f 622f  python-sdk/blob/
-00000390: 6d61 696e 2f64 6f63 732f 5f73 6f75 7263  main/docs/_sourc
-000003a0: 652f 5f73 7461 7469 632f 7870 616e 7365  e/_static/xpanse
-000003b0: 5f62 616e 6e65 722e 706e 673f 7261 773d  _banner.png?raw=
-000003c0: 7472 7565 0a20 2020 3a77 6964 7468 3a20  true.   :width: 
-000003d0: 3830 300a 2020 203a 7461 7267 6574 3a20  800.   :target: 
-000003e0: 6874 7470 733a 2f2f 6578 7061 6e73 652e  https://expanse.
-000003f0: 636f 2f0a 0a2e 2e20 696d 6167 653a 3a20  co/.... image:: 
-00000400: 6874 7470 733a 2f2f 696d 672e 7368 6965  https://img.shie
-00000410: 6c64 732e 696f 2f62 6164 6765 2f63 6f64  lds.io/badge/cod
-00000420: 6525 3230 7374 796c 652d 626c 6163 6b2d  e%20style-black-
-00000430: 3030 3030 3030 2e73 7667 0a20 2020 3a74  000000.svg.   :t
-00000440: 6172 6765 743a 2068 7474 7073 3a2f 2f67  arget: https://g
-00000450: 6974 6875 622e 636f 6d2f 7073 662f 626c  ithub.com/psf/bl
-00000460: 6163 6b0a 0a2e 2e20 696d 6167 653a 3a20  ack.... image:: 
-00000470: 6874 7470 733a 2f2f 696d 672e 7368 6965  https://img.shie
-00000480: 6c64 732e 696f 2f62 6164 6765 2f70 7974  lds.io/badge/pyt
-00000490: 686f 6e2d 332e 3625 3230 2537 4325 3230  hon-3.6%20%7C%20
-000004a0: 332e 3725 3230 2537 4325 3230 332e 382d  3.7%20%7C%203.8-
-000004b0: 626c 7565 7669 6f6c 6574 0a20 2020 3a74  blueviolet.   :t
-000004c0: 6172 6765 743a 2068 7474 7073 3a2f 2f70  arget: https://p
-000004d0: 7970 692e 7079 7468 6f6e 2e6f 7267 2f70  ypi.python.org/p
-000004e0: 7970 692f 7870 616e 7365 0a0a 2e2e 2069  ypi/xpanse.... i
-000004f0: 6d61 6765 3a3a 2068 7474 7073 3a2f 2f69  mage:: https://i
-00000500: 6d67 2e73 6869 656c 6473 2e69 6f2f 6261  mg.shields.io/ba
-00000510: 6467 652f 636f 6465 2532 3073 7479 6c65  dge/code%20style
-00000520: 2d62 6c61 636b 2d30 3030 3030 302e 7376  -black-000000.sv
-00000530: 670a 2020 203a 7461 7267 6574 3a20 6874  g.   :target: ht
-00000540: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00000550: 2f70 7366 2f62 6c61 636b 0a0a 2e2e 2069  /psf/black.... i
-00000560: 6d61 6765 3a3a 2068 7474 7073 3a2f 2f69  mage:: https://i
-00000570: 6d67 2e73 6869 656c 6473 2e69 6f2f 7079  mg.shields.io/py
-00000580: 7069 2f6c 2f78 7061 6e73 650a 2020 203a  pi/l/xpanse.   :
-00000590: 7461 7267 6574 3a20 6874 7470 733a 2f2f  target: https://
-000005a0: 6769 7468 7562 2e63 6f6d 2f50 616c 6f41  github.com/PaloA
-000005b0: 6c74 6f4e 6574 776f 726b 732f 636f 7274  ltoNetworks/cort
-000005c0: 6578 2d78 7061 6e73 652d 7079 7468 6f6e  ex-xpanse-python
-000005d0: 2d73 646b 2f62 6c6f 622f 6d61 696e 2f4c  -sdk/blob/main/L
-000005e0: 4943 454e 5345 0a0a 2e2e 2069 6d61 6765  ICENSE.... image
-000005f0: 3a3a 2068 7474 7073 3a2f 2f69 6d67 2e73  :: https://img.s
-00000600: 6869 656c 6473 2e69 6f2f 6769 7468 7562  hields.io/github
-00000610: 2f63 6f6e 7472 6962 7574 6f72 732f 5061  /contributors/Pa
-00000620: 6c6f 416c 746f 4e65 7477 6f72 6b73 2f63  loAltoNetworks/c
-00000630: 6f72 7465 782d 7870 616e 7365 2d70 7974  ortex-xpanse-pyt
-00000640: 686f 6e2d 7364 6b0a 2020 203a 7461 7267  hon-sdk.   :targ
-00000650: 6574 3a20 6874 7470 733a 2f2f 6769 7468  et: https://gith
-00000660: 7562 2e63 6f6d 2f50 616c 6f41 6c74 6f4e  ub.com/PaloAltoN
-00000670: 6574 776f 726b 732f 636f 7274 6578 2d78  etworks/cortex-x
-00000680: 7061 6e73 652d 7079 7468 6f6e 2d73 646b  panse-python-sdk
-00000690: 2f67 7261 7068 732f 636f 6e74 7269 6275  /graphs/contribu
-000006a0: 746f 7273 0a0a 4f76 6572 7669 6577 0a2d  tors..Overview.-
-000006b0: 2d2d 2d2d 2d2d 2d0a 0a54 6869 7320 6c69  -------..This li
-000006c0: 6272 6172 7920 6973 2069 6e74 656e 6465  brary is intende
-000006d0: 6420 746f 2062 6520 616e 2069 6e74 6572  d to be an inter
-000006e0: 6661 6365 2074 6f20 7468 6520 6058 7061  face to the `Xpa
-000006f0: 6e73 6520 4578 7061 6e64 6572 2041 5049  nse Expander API
-00000700: 203c 6874 7470 733a 2f2f 6b6e 6f77 6c65   <https://knowle
-00000710: 6467 6562 6173 652e 7870 616e 7365 2e63  dgebase.xpanse.c
-00000720: 6f2f 6578 7061 6e64 6572 2d61 7069 732f  o/expander-apis/
-00000730: 3e60 5f2e 0a0a 496e 7374 616c 6c0a 2d2d  >`_...Install.--
-00000740: 2d2d 2d2d 2d0a 2e2e 2063 6f64 652d 626c  -----... code-bl
-00000750: 6f63 6b3a 3a20 7079 7468 6f6e 0a0a 2020  ock:: python..  
-00000760: 2020 7069 7020 696e 7374 616c 6c20 7870    pip install xp
-00000770: 616e 7365 0a0a 5265 7175 6972 656d 656e  anse..Requiremen
-00000780: 7473 0a2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a  ts.------------.
-00000790: 0a50 7974 686f 6e20 332e 362b 0a0a 5573  .Python 3.6+..Us
-000007a0: 6167 650a 2d2d 2d2d 2d0a 6044 6f63 756d  age.-----.`Docum
-000007b0: 656e 7461 7469 6f6e 203c 6874 7470 733a  entation <https:
-000007c0: 2f2f 636f 7274 6578 2d78 7061 6e73 652d  //cortex-xpanse-
-000007d0: 7079 7468 6f6e 2d73 646b 2e72 6561 6474  python-sdk.readt
-000007e0: 6865 646f 6373 2e69 6f2f 656e 2f6c 6174  hedocs.io/en/lat
-000007f0: 6573 742f 3e60 5f0a 0a2e 2e20 636f 6465  est/>`_.... code
-00000800: 2d62 6c6f 636b 3a3a 2070 7974 686f 6e0a  -block:: python.
-00000810: 0a20 2020 2023 2049 6d70 6f72 7420 636c  .    # Import cl
-00000820: 6965 6e74 0a20 2020 2066 726f 6d20 7870  ient.    from xp
-00000830: 616e 7365 2e63 6c69 656e 7420 696d 706f  anse.client impo
-00000840: 7274 2045 7843 6c69 656e 740a 0a20 2020  rt ExClient..   
-00000850: 2023 2069 6e69 7469 616c 697a 6520 636c   # initialize cl
-00000860: 6965 6e74 0a20 2020 2063 6c69 656e 7420  ient.    client 
-00000870: 3d20 4578 436c 6965 6e74 2829 0a0a 2020  = ExClient()..  
-00000880: 2020 2320 6765 7420 6970 5f72 616e 6765    # get ip_range
-00000890: 2069 7465 7261 746f 7220 6f62 6a65 6374   iterator object
-000008a0: 2061 6e64 2064 756d 7020 746f 2061 206c   and dump to a l
-000008b0: 6973 740a 2020 2020 7261 6e67 6573 203d  ist.    ranges =
-000008c0: 2063 6c69 656e 742e 6173 7365 7473 2e69   client.assets.i
-000008d0: 705f 7261 6e67 652e 6c69 7374 2829 2e64  p_range.list().d
-000008e0: 756d 7028 290a 0a59 6f75 2063 616e 2076  ump()..You can v
-000008f0: 6965 7720 6d6f 7265 2065 7861 6d70 6c65  iew more example
-00000900: 2063 6f64 6520 696e 2074 6865 2060 6578   code in the `ex
-00000910: 616d 706c 6573 203c 6874 7470 733a 2f2f  amples <https://
-00000920: 6769 7468 7562 2e63 6f6d 2f50 616c 6f41  github.com/PaloA
-00000930: 6c74 6f4e 6574 776f 726b 732f 636f 7274  ltoNetworks/cort
-00000940: 6578 2d78 7061 6e73 652d 7079 7468 6f6e  ex-xpanse-python
-00000950: 2d73 646b 2f74 7265 652f 6d61 696e 2f65  -sdk/tree/main/e
-00000960: 7861 6d70 6c65 733e 605f 2064 6972 6563  xamples>`_ direc
-00000970: 746f 7279 2e0a 0a43 6f6e 6669 6775 7261  tory...Configura
-00000980: 7469 6f6e 0a2d 2d2d 2d2d 2d2d 2d2d 2d2d  tion.-----------
-00000990: 2d2d 0a41 2076 616c 6964 2043 6c69 656e  --.A valid Clien
-000009a0: 7420 4944 2061 6e64 2053 6563 7265 7420  t ID and Secret 
-000009b0: 6973 2072 6571 7569 7265 6420 666f 7220  is required for 
-000009c0: 7573 652e 2054 6869 7320 6973 2072 6563  use. This is rec
-000009d0: 6f6d 6d65 6e64 6564 206f 7665 7220 7573  ommended over us
-000009e0: 696e 6720 6120 4a57 542c 2061 7320 7468  ing a JWT, as th
-000009f0: 6579 2068 6176 6520 6c69 6d69 7465 6420  ey have limited 
-00000a00: 6c69 6665 7370 616e 732e 0a57 6869 6c65  lifespans..While
-00000a10: 2061 2062 6561 7265 7220 746f 6b65 6e20   a bearer token 
-00000a20: 6973 2073 7570 706f 7274 6564 2069 6e20  is supported in 
-00000a30: 7468 6973 2076 6572 7369 6f6e 2c20 7468  this version, th
-00000a40: 6973 2061 7574 6820 666c 6f77 2069 7320  is auth flow is 
-00000a50: 6265 696e 6720 6465 7072 6563 6174 6564  being deprecated
-00000a60: 2e20 5468 6572 6566 6f72 652c 2069 7420  . Therefore, it 
-00000a70: 6973 2068 6967 686c 7920 7265 636f 6d6d  is highly recomm
-00000a80: 656e 6465 6420 746f 2075 7365 2043 6c69  ended to use Cli
-00000a90: 656e 7420 4372 6564 656e 7469 616c 732e  ent Credentials.
-00000aa0: 0a0a 5245 434f 4d4d 454e 4445 440a 2a2a  ..RECOMMENDED.**
-00000ab0: 2a2a 2a2a 2a2a 2a2a 2a0a 596f 7520 6361  *********.You ca
-00000ac0: 6e20 7375 7070 6c79 2074 6865 6d20 6173  n supply them as
-00000ad0: 2065 6e76 6972 6f6e 6d65 6e74 2076 6172   environment var
-00000ae0: 6961 626c 6573 2075 7369 6e67 2074 6865  iables using the
-00000af0: 2076 6172 6961 626c 6520 6e61 6d65 7320   variable names 
-00000b00: 6060 5850 414e 5345 5f43 4c49 454e 545f  ``XPANSE_CLIENT_
-00000b10: 4944 6060 2041 4e44 2060 6058 5041 4e53  ID`` AND ``XPANS
-00000b20: 455f 434c 4945 4e54 5f53 4543 5245 5460  E_CLIENT_SECRET`
-00000b30: 602e 0a0a 2e2e 2063 6f64 652d 626c 6f63  `..... code-bloc
-00000b40: 6b3a 3a20 7079 7468 6f6e 0a0a 2020 2020  k:: python..    
-00000b50: 6578 706f 7274 2058 5041 4e53 455f 434c  export XPANSE_CL
-00000b60: 4945 4e54 5f49 443d 3c43 6c69 656e 7420  IENT_ID=<Client 
-00000b70: 4944 3e0a 2020 2020 6578 706f 7274 2058  ID>.    export X
-00000b80: 5041 4e53 455f 434c 4945 4e54 5f53 4543  PANSE_CLIENT_SEC
-00000b90: 5245 543d 3c43 6c69 656e 7420 5365 6372  RET=<Client Secr
-00000ba0: 6574 3e0a 2020 2020 0a4e 4f54 2052 4543  et>.    .NOT REC
-00000bb0: 4f4d 4d45 4e44 4544 0a2a 2a2a 2a2a 2a2a  OMMENDED.*******
-00000bc0: 2a2a 2a2a 2a2a 2a2a 0a54 6f20 7573 6520  ********.To use 
-00000bd0: 6120 7368 6f72 7420 6c69 7665 6420 4a57  a short lived JW
-00000be0: 542c 2079 6f75 2063 616e 2073 7570 706c  T, you can suppl
-00000bf0: 7920 7468 6520 4a57 5420 6173 2061 6e20  y the JWT as an 
-00000c00: 656e 7669 726f 6e6d 656e 7461 6c20 7661  environmental va
-00000c10: 7269 6162 6c65 2075 7369 6e67 2074 6865  riable using the
-00000c20: 206e 616d 6520 6060 5850 414e 5345 5f4a   name ``XPANSE_J
-00000c30: 5754 5f54 4f4b 454e 6060 0a0a 2e2e 2063  WT_TOKEN``.... c
-00000c40: 6f64 652d 626c 6f63 6b3a 3a20 7079 7468  ode-block:: pyth
-00000c50: 6f6e 0a0a 2020 2020 6578 706f 7274 2058  on..    export X
-00000c60: 5041 4e53 455f 4a57 545f 544f 4b45 4e3d  PANSE_JWT_TOKEN=
-00000c70: 3c4a 5754 3e0a 0a5b 4465 7072 6563 6174  <JWT>..[Deprecat
-00000c80: 6564 5d0a 4120 7661 6c69 6420 4265 6172  ed].A valid Bear
-00000c90: 6572 2074 6f6b 656e 2063 616e 2062 6520  er token can be 
-00000ca0: 7375 7070 6c69 6564 2061 7320 616e 2065  supplied as an e
-00000cb0: 6e76 6972 6f6e 6d65 6e74 2076 6172 6961  nvironment varia
-00000cc0: 626c 650a 0a54 6f20 7375 7070 6c79 2061  ble..To supply a
-00000cd0: 2076 616c 6964 2062 6561 7265 7220 746f   valid bearer to
-00000ce0: 6b65 6e20 6173 2061 6e20 656e 7669 726f  ken as an enviro
-00000cf0: 6e6d 656e 7420 7661 7269 6162 6c65 2c20  nment variable, 
-00000d00: 796f 7520 6361 6e20 7573 6520 7468 6520  you can use the 
-00000d10: 7661 7269 6162 6c65 206e 616d 6573 2060  variable names `
-00000d20: 6058 5041 4e53 455f 4245 4152 4552 5f54  `XPANSE_BEARER_T
-00000d30: 4f4b 454e 6060 2e0a 0a2e 2e20 636f 6465  OKEN``..... code
-00000d40: 2d62 6c6f 636b 3a3a 2070 7974 686f 6e0a  -block:: python.
-00000d50: 0a20 2020 2065 7870 6f72 7420 5850 414e  .    export XPAN
-00000d60: 5345 5f42 4541 5245 525f 544f 4b45 4e3d  SE_BEARER_TOKEN=
-00000d70: 3c42 6561 7265 7220 546f 6b65 6e3e 0a0a  <Bearer Token>..
-00000d80: 4c6f 6767 696e 670a 2d2d 2d2d 2d2d 2d0a  Logging.-------.
-00000d90: 4c6f 6767 696e 6720 6973 2068 616e 646c  Logging is handl
-00000da0: 6564 2074 6872 6f75 6768 2074 6865 2070  ed through the p
-00000db0: 7974 686f 6e20 6c6f 6767 696e 6720 7061  ython logging pa
-00000dc0: 636b 6167 652e 2054 6f20 656e 6162 6c65  ckage. To enable
-00000dd0: 2064 6966 6665 7265 6e74 206c 6576 656c   different level
-00000de0: 7320 6f66 2076 6572 626f 7369 7479 2069  s of verbosity i
-00000df0: 6e20 796f 7572 2073 6372 6970 7473 2079  n your scripts y
-00000e00: 6f75 2063 616e 2064 6f20 7468 6520 666f  ou can do the fo
-00000e10: 6c6c 6f77 696e 673a 0a0a 2e2e 2063 6f64  llowing:.... cod
-00000e20: 652d 626c 6f63 6b3a 3a20 7079 7468 6f6e  e-block:: python
-00000e30: 0a0a 2020 2020 696d 706f 7274 206c 6f67  ..    import log
-00000e40: 6769 6e67 0a20 2020 206c 6f67 6769 6e67  ging.    logging
-00000e50: 2e62 6173 6963 436f 6e66 6967 286c 6576  .basicConfig(lev
-00000e60: 656c 3d6c 6f67 6769 6e67 2e44 4542 5547  el=logging.DEBUG
-00000e70: 290a 0a59 6f75 2063 616e 2072 6561 6420  )..You can read 
-00000e80: 6d6f 7265 2061 7420 603c 6874 7470 733a  more at `<https:
-00000e90: 2f2f 646f 6373 2e70 7974 686f 6e2e 6f72  //docs.python.or
-00000ea0: 672f 332f 6c69 6272 6172 792f 6c6f 6767  g/3/library/logg
-00000eb0: 696e 672e 6874 6d6c 3e60 5f2e 0a0a 0a    ing.html>`_....
+00000020: 7365 0a56 6572 7369 6f6e 3a20 322e 302e  se.Version: 2.0.
+00000030: 3072 6333 0a53 756d 6d61 7279 3a20 5079  0rc3.Summary: Py
+00000040: 7468 6f6e 206c 6962 7261 7279 2069 7320  thon library is 
+00000050: 616e 2069 6e74 6572 6661 6365 2074 6f20  an interface to 
+00000060: 7468 6520 436f 7274 6578 2058 7061 6e73  the Cortex Xpans
+00000070: 6520 4150 492e 0a48 6f6d 652d 7061 6765  e API..Home-page
+00000080: 3a20 554e 4b4e 4f57 4e0a 4175 7468 6f72  : UNKNOWN.Author
+00000090: 3a20 5061 6c6f 2041 6c74 6f20 436f 7274  : Palo Alto Cort
+000000a0: 6578 2058 7061 6e73 650a 4175 7468 6f72  ex Xpanse.Author
+000000b0: 2d65 6d61 696c 3a20 7870 616e 7365 2d69  -email: xpanse-i
+000000c0: 6e74 6567 7261 7469 6f6e 7340 7061 6c6f  ntegrations@palo
+000000d0: 616c 746f 6e65 7477 6f72 6b73 2e63 6f6d  altonetworks.com
+000000e0: 0a4c 6963 656e 7365 3a20 4953 430a 4b65  .License: ISC.Ke
+000000f0: 7977 6f72 6473 3a20 7870 616e 7365 2069  ywords: xpanse i
+00000100: 6f6d 0a50 6c61 7466 6f72 6d3a 2055 4e4b  om.Platform: UNK
+00000110: 4e4f 574e 0a43 6c61 7373 6966 6965 723a  NOWN.Classifier:
+00000120: 2044 6576 656c 6f70 6d65 6e74 2053 7461   Development Sta
+00000130: 7475 7320 3a3a 2035 202d 2050 726f 6475  tus :: 5 - Produ
+00000140: 6374 696f 6e2f 5374 6162 6c65 0a43 6c61  ction/Stable.Cla
+00000150: 7373 6966 6965 723a 2049 6e74 656e 6465  ssifier: Intende
+00000160: 6420 4175 6469 656e 6365 203a 3a20 4465  d Audience :: De
+00000170: 7665 6c6f 7065 7273 0a43 6c61 7373 6966  velopers.Classif
+00000180: 6965 723a 2054 6f70 6963 203a 3a20 536f  ier: Topic :: So
+00000190: 6674 7761 7265 2044 6576 656c 6f70 6d65  ftware Developme
+000001a0: 6e74 0a43 6c61 7373 6966 6965 723a 2054  nt.Classifier: T
+000001b0: 6f70 6963 203a 3a20 536f 6674 7761 7265  opic :: Software
+000001c0: 2044 6576 656c 6f70 6d65 6e74 203a 3a20   Development :: 
+000001d0: 4c69 6272 6172 6965 730a 436c 6173 7369  Libraries.Classi
+000001e0: 6669 6572 3a20 546f 7069 6320 3a3a 2053  fier: Topic :: S
+000001f0: 6f66 7477 6172 6520 4465 7665 6c6f 706d  oftware Developm
+00000200: 656e 7420 3a3a 204c 6962 7261 7269 6573  ent :: Libraries
+00000210: 203a 3a20 4170 706c 6963 6174 696f 6e20   :: Application 
+00000220: 4672 616d 6577 6f72 6b73 0a43 6c61 7373  Frameworks.Class
+00000230: 6966 6965 723a 2050 726f 6772 616d 6d69  ifier: Programmi
+00000240: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
+00000250: 7974 686f 6e20 3a3a 2033 0a43 6c61 7373  ython :: 3.Class
+00000260: 6966 6965 723a 2050 726f 6772 616d 6d69  ifier: Programmi
+00000270: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
+00000280: 7974 686f 6e20 3a3a 2033 2e37 0a43 6c61  ython :: 3.7.Cla
+00000290: 7373 6966 6965 723a 2050 726f 6772 616d  ssifier: Program
+000002a0: 6d69 6e67 204c 616e 6775 6167 6520 3a3a  ming Language ::
+000002b0: 2050 7974 686f 6e20 3a3a 2033 2e38 0a43   Python :: 3.8.C
+000002c0: 6c61 7373 6966 6965 723a 2050 726f 6772  lassifier: Progr
+000002d0: 616d 6d69 6e67 204c 616e 6775 6167 6520  amming Language 
+000002e0: 3a3a 2050 7974 686f 6e20 3a3a 2033 2e39  :: Python :: 3.9
+000002f0: 0a43 6c61 7373 6966 6965 723a 2050 726f  .Classifier: Pro
+00000300: 6772 616d 6d69 6e67 204c 616e 6775 6167  gramming Languag
+00000310: 6520 3a3a 2050 7974 686f 6e20 3a3a 2033  e :: Python :: 3
+00000320: 2e31 300a 5265 7175 6972 6573 2d50 7974  .10.Requires-Pyt
+00000330: 686f 6e3a 203e 3d33 2e37 0a44 6573 6372  hon: >=3.7.Descr
+00000340: 6970 7469 6f6e 2d43 6f6e 7465 6e74 2d54  iption-Content-T
+00000350: 7970 653a 2074 6578 742f 6d61 726b 646f  ype: text/markdo
+00000360: 776e 0a4c 6963 656e 7365 2d46 696c 653a  wn.License-File:
+00000370: 204c 4943 454e 5345 0a0a 436f 7274 6578   LICENSE..Cortex
+00000380: 2058 7061 6e73 6520 5079 7468 6f6e 2053   Xpanse Python S
+00000390: 444b 0a3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  DK.=============
+000003a0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d0a 3c70 2061  ===========.<p a
+000003b0: 6c69 676e 3d22 6365 6e74 6572 223e 0a20  lign="center">. 
+000003c0: 2020 203c 6120 6872 6566 3d22 6874 7470     <a href="http
+000003d0: 733a 2f2f 6578 7061 6e73 652e 636f 2f22  s://expanse.co/"
+000003e0: 3e0a 2020 2020 2020 2020 3c69 6d67 2073  >.        <img s
+000003f0: 7263 3d22 6874 7470 733a 2f2f 6769 7468  rc="https://gith
+00000400: 7562 2e63 6f6d 2f50 616c 6f41 6c74 6f4e  ub.com/PaloAltoN
+00000410: 6574 776f 726b 732f 636f 7274 6578 2d78  etworks/cortex-x
+00000420: 7061 6e73 652d 7079 7468 6f6e 2d73 646b  panse-python-sdk
+00000430: 2f62 6c6f 622f 6d61 696e 2f64 6f63 732f  /blob/main/docs/
+00000440: 5f73 6f75 7263 652f 5f73 7461 7469 632f  _source/_static/
+00000450: 7870 616e 7365 5f62 616e 6e65 722e 706e  xpanse_banner.pn
+00000460: 673f 7261 773d 7472 7565 222f 3e0a 2020  g?raw=true"/>.  
+00000470: 2020 3c2f 613e 0a3c 2f70 3e0a 0a3c 7020    </a>.</p>..<p 
+00000480: 616c 6967 6e3d 2263 656e 7465 7222 3e0a  align="center">.
+00000490: 2020 2020 3c61 2068 7265 663d 2268 7474      <a href="htt
+000004a0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+000004b0: 7073 662f 626c 6163 6b22 3e0a 2020 2020  psf/black">.    
+000004c0: 2020 2020 3c69 6d67 2073 7263 3d22 6874      <img src="ht
+000004d0: 7470 733a 2f2f 696d 672e 7368 6965 6c64  tps://img.shield
+000004e0: 732e 696f 2f62 6164 6765 2f63 6f64 6525  s.io/badge/code%
+000004f0: 3230 7374 796c 652d 626c 6163 6b2d 3030  20style-black-00
+00000500: 3030 3030 2e73 7667 222f 3e0a 2020 2020  0000.svg"/>.    
+00000510: 3c2f 613e 0a20 2020 203c 6120 6872 6566  </a>.    <a href
+00000520: 3d22 6874 7470 733a 2f2f 7079 7069 2e70  ="https://pypi.p
+00000530: 7974 686f 6e2e 6f72 672f 7079 7069 2f78  ython.org/pypi/x
+00000540: 7061 6e73 6522 3e0a 2020 2020 2020 2020  panse">.        
+00000550: 3c69 6d67 2073 7263 3d22 6874 7470 733a  <img src="https:
+00000560: 2f2f 696d 672e 7368 6965 6c64 732e 696f  //img.shields.io
+00000570: 2f62 6164 6765 2f70 7974 686f 6e2d 332e  /badge/python-3.
+00000580: 3725 3230 2537 4325 3230 332e 3825 3230  7%20%7C%203.8%20
+00000590: 2537 4325 3230 332e 3925 3230 2537 4325  %7C%203.9%20%7C%
+000005a0: 3230 332e 3130 2d62 6c75 6576 696f 6c65  203.10-blueviole
+000005b0: 7422 2f3e 0a20 2020 203c 2f61 3e0a 2020  t"/>.    </a>.  
+000005c0: 2020 3c61 2068 7265 663d 2268 7474 7073    <a href="https
+000005d0: 3a2f 2f67 6974 6875 622e 636f 6d2f 5061  ://github.com/Pa
+000005e0: 6c6f 416c 746f 4e65 7477 6f72 6b73 2f63  loAltoNetworks/c
+000005f0: 6f72 7465 782d 7870 616e 7365 2d70 7974  ortex-xpanse-pyt
+00000600: 686f 6e2d 7364 6b2f 626c 6f62 2f6d 6169  hon-sdk/blob/mai
+00000610: 6e2f 4c49 4345 4e53 4522 3e0a 2020 2020  n/LICENSE">.    
+00000620: 2020 2020 3c69 6d67 2073 7263 3d22 6874      <img src="ht
+00000630: 7470 733a 2f2f 696d 672e 7368 6965 6c64  tps://img.shield
+00000640: 732e 696f 2f70 7970 692f 6c2f 7870 616e  s.io/pypi/l/xpan
+00000650: 7365 222f 3e0a 2020 2020 3c2f 613e 0a20  se"/>.    </a>. 
+00000660: 2020 203c 6120 6872 6566 3d22 6874 7470     <a href="http
+00000670: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f50  s://github.com/P
+00000680: 616c 6f41 6c74 6f4e 6574 776f 726b 732f  aloAltoNetworks/
+00000690: 636f 7274 6578 2d78 7061 6e73 652d 7079  cortex-xpanse-py
+000006a0: 7468 6f6e 2d73 646b 2f67 7261 7068 732f  thon-sdk/graphs/
+000006b0: 636f 6e74 7269 6275 746f 7273 223e 0a20  contributors">. 
+000006c0: 2020 2020 2020 203c 696d 6720 7372 633d         <img src=
+000006d0: 2268 7474 7073 3a2f 2f69 6d67 2e73 6869  "https://img.shi
+000006e0: 656c 6473 2e69 6f2f 6769 7468 7562 2f63  elds.io/github/c
+000006f0: 6f6e 7472 6962 7574 6f72 732f 5061 6c6f  ontributors/Palo
+00000700: 416c 746f 4e65 7477 6f72 6b73 2f63 6f72  AltoNetworks/cor
+00000710: 7465 782d 7870 616e 7365 2d70 7974 686f  tex-xpanse-pytho
+00000720: 6e2d 7364 6b22 2f3e 0a20 2020 203c 2f61  n-sdk"/>.    </a
+00000730: 3e0a 3c2f 703e 0a0a 4f76 6572 7669 6577  >.</p>..Overview
+00000740: 0a2d 2d2d 2d2d 2d2d 2d0a 0a54 6869 7320  .--------..This 
+00000750: 6c69 6272 6172 7920 6973 2069 6e74 656e  library is inten
+00000760: 6465 6420 746f 2062 6520 616e 2069 6e74  ded to be an int
+00000770: 6572 6661 6365 2074 6f20 7468 650a 3c61  erface to the.<a
+00000780: 2068 7265 663d 2268 7474 7073 3a2f 2f64   href="https://d
+00000790: 6f63 732d 636f 7274 6578 2e70 616c 6f61  ocs-cortex.paloa
+000007a0: 6c74 6f6e 6574 776f 726b 732e 636f 6d2f  ltonetworks.com/
+000007b0: 722f 436f 7274 6578 2d58 5041 4e53 452f  r/Cortex-XPANSE/
+000007c0: 436f 7274 6578 2d58 7061 6e73 652d 4150  Cortex-Xpanse-AP
+000007d0: 492d 5265 6665 7265 6e63 6522 3e43 6f72  I-Reference">Cor
+000007e0: 7465 7820 5870 616e 7365 2050 7562 6c69  tex Xpanse Publi
+000007f0: 6320 4150 493c 2f61 3e2e 0a0a 496e 7374  c API</a>...Inst
+00000800: 616c 6c0a 2d2d 2d2d 2d2d 2d0a 6060 6070  all.-------.```p
+00000810: 7974 686f 6e0a 7069 7020 696e 7374 616c  ython.pip instal
+00000820: 6c20 7870 616e 7365 0a60 6060 0a0a 5265  l xpanse.```..Re
+00000830: 7175 6972 656d 656e 7473 0a2d 2d2d 2d2d  quirements.-----
+00000840: 2d2d 2d2d 2d2d 2d0a 0a60 5079 7468 6f6e  -------..`Python
+00000850: 2033 2e37 2b60 0a0a 5573 6167 650a 2d2d   3.7+`..Usage.--
+00000860: 2d2d 2d0a 3c61 2068 7265 663d 2268 7474  ---.<a href="htt
+00000870: 7073 3a2f 2f63 6f72 7465 782d 7870 616e  ps://cortex-xpan
+00000880: 7365 2d70 7974 686f 6e2d 7364 6b2e 7265  se-python-sdk.re
+00000890: 6164 7468 6564 6f63 732e 696f 2f65 6e2f  adthedocs.io/en/
+000008a0: 6c61 7465 7374 2f22 3e43 6f72 7465 7820  latest/">Cortex 
+000008b0: 5870 616e 7365 2050 7562 6c69 6320 4150  Xpanse Public AP
+000008c0: 4920 446f 6375 6d65 6e74 6174 696f 6e3c  I Documentation<
+000008d0: 2f61 3e0a 0a60 6060 7079 7468 6f6e 0a23  /a>..```python.#
+000008e0: 2049 6d70 6f72 7420 636c 6965 6e74 0a66   Import client.f
+000008f0: 726f 6d20 7870 616e 7365 2e63 6c69 656e  rom xpanse.clien
+00000900: 7420 696d 706f 7274 2058 7061 6e73 6543  t import XpanseC
+00000910: 6c69 656e 740a 0a23 2049 6e69 7469 616c  lient..# Initial
+00000920: 697a 6520 636c 6965 6e74 0a63 6c69 656e  ize client.clien
+00000930: 7420 3d20 5870 616e 7365 436c 6965 6e74  t = XpanseClient
+00000940: 2829 0a0a 2320 4765 7420 6173 7365 7473  ()..# Get assets
+00000950: 2069 7465 7261 746f 7220 6f62 6a65 6374   iterator object
+00000960: 2061 6e64 2064 756d 7020 746f 2061 206c   and dump to a l
+00000970: 6973 740a 6173 7365 7473 203d 2063 6c69  ist.assets = cli
+00000980: 656e 742e 6173 7365 7473 2e6c 6973 7428  ent.assets.list(
+00000990: 292e 6475 6d70 2829 0a60 6060 0a0a 596f  ).dump().```..Yo
+000009a0: 7520 6361 6e20 7669 6577 206d 6f72 6520  u can view more 
+000009b0: 6578 616d 706c 6520 636f 6465 2069 6e20  example code in 
+000009c0: 7468 6520 3c61 2068 7265 663d 2268 7474  the <a href="htt
+000009d0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+000009e0: 5061 6c6f 416c 746f 4e65 7477 6f72 6b73  PaloAltoNetworks
+000009f0: 2f63 6f72 7465 782d 7870 616e 7365 2d70  /cortex-xpanse-p
+00000a00: 7974 686f 6e2d 7364 6b2f 7472 6565 2f6d  ython-sdk/tree/m
+00000a10: 6169 6e2f 6578 616d 706c 6573 223e 6578  ain/examples">ex
+00000a20: 616d 706c 6573 3c2f 613e 2064 6972 6563  amples</a> direc
+00000a30: 746f 7279 2e0a 0a43 6f6e 6669 6775 7261  tory...Configura
+00000a40: 7469 6f6e 0a2d 2d2d 2d2d 2d2d 2d2d 2d2d  tion.-----------
+00000a50: 2d2d 0a41 2076 616c 6964 2060 4150 4920  --.A valid `API 
+00000a60: 4b65 7960 2c20 6041 5049 204b 6579 2049  Key`, `API Key I
+00000a70: 4460 2c20 616e 6420 6046 756c 6c79 2051  D`, and `Fully Q
+00000a80: 7561 6c69 6669 6564 2044 6f6d 6169 6e20  ualified Domain 
+00000a90: 4e61 6d65 2028 4651 444e 2960 2061 7265  Name (FQDN)` are
+00000aa0: 2072 6571 7569 7265 6420 666f 7220 7573   required for us
+00000ab0: 652e 0a0a 5265 6665 7265 6e63 6520 7468  e...Reference th
+00000ac0: 6520 646f 6373 2066 6f72 206d 6f72 6520  e docs for more 
+00000ad0: 696e 666f 726d 6174 696f 6e20 7769 7468  information with
+00000ae0: 203c 6120 6872 6566 3d22 6874 7470 733a   <a href="https:
+00000af0: 2f2f 646f 6373 2d63 6f72 7465 782e 7061  //docs-cortex.pa
+00000b00: 6c6f 616c 746f 6e65 7477 6f72 6b73 2e63  loaltonetworks.c
+00000b10: 6f6d 2f72 2f43 6f72 7465 782d 5850 414e  om/r/Cortex-XPAN
+00000b20: 5345 2f43 6f72 7465 782d 5870 616e 7365  SE/Cortex-Xpanse
+00000b30: 2d41 5049 2d52 6566 6572 656e 6365 2f47  -API-Reference/G
+00000b40: 6574 2d53 7461 7274 6564 2d77 6974 682d  et-Started-with-
+00000b50: 4150 4973 223e 4765 7474 696e 6720 5374  APIs">Getting St
+00000b60: 6172 7465 643c 2f61 3e2e 0a0a 2323 2323  arted</a>...####
+00000b70: 2052 4543 4f4d 4d45 4e44 4544 0a2a 2a2a   RECOMMENDED.***
+00000b80: 2a2a 2a2a 2a2a 2a2a 0a59 6f75 2063 616e  ********.You can
+00000b90: 2073 7570 706c 7920 7468 656d 2061 7320   supply them as 
+00000ba0: 656e 7669 726f 6e6d 656e 7420 7661 7269  environment vari
+00000bb0: 6162 6c65 732e 0a0a 6060 6073 6865 6c6c  ables...```shell
+00000bc0: 2073 6372 6970 740a 6578 706f 7274 2043   script.export C
+00000bd0: 4f52 5445 585f 4651 444e 3d3c 596f 7572  ORTEX_FQDN=<Your
+00000be0: 2058 7061 6e73 6520 496e 7374 616e 6365   Xpanse Instance
+00000bf0: 2055 524c 3e0a 6578 706f 7274 2043 4f52   URL>.export COR
+00000c00: 5445 585f 4150 495f 4b45 593d 3c41 5049  TEX_API_KEY=<API
+00000c10: 204b 6579 3e0a 6578 706f 7274 2043 4f52   Key>.export COR
+00000c20: 5445 585f 4150 495f 4b45 595f 4944 3d3c  TEX_API_KEY_ID=<
+00000c30: 4150 4920 4b65 7920 4944 3e0a 6060 600a  API Key ID>.```.
+00000c40: 2020 2020 0a23 2323 2320 4e4f 5420 5245      .#### NOT RE
+00000c50: 434f 4d4d 454e 4445 440a 2a2a 2a2a 2a2a  COMMENDED.******
+00000c60: 2a2a 2a2a 2a2a 2a2a 2a0a 5468 6520 666f  *********.The fo
+00000c70: 6c6c 6f77 696e 6720 7061 7261 6d65 7465  llowing paramete
+00000c80: 7273 2063 616e 2062 6520 7365 7420 696e  rs can be set in
+00000c90: 6c69 6e65 2075 7369 6e67 2074 6865 2060  line using the `
+00000ca0: 5870 616e 7365 436c 6965 6e74 6020 636f  XpanseClient` co
+00000cb0: 6e73 7472 7563 746f 722e 0a0a 5f54 6869  nstructor..._Thi
+00000cc0: 7320 6973 206e 6f74 2072 6563 6f6d 6d65  s is not recomme
+00000cd0: 6e64 6564 2c20 6173 2069 7420 6561 7369  nded, as it easi
+00000ce0: 6c79 2065 7870 6f73 6573 2073 656e 7369  ly exposes sensi
+00000cf0: 7469 7665 2063 7265 6465 6e74 6961 6c73  tive credentials
+00000d00: 2069 6e20 796f 7572 2073 6f75 7263 6520   in your source 
+00000d10: 636f 6465 2e5f 200a 0a60 6060 7079 7468  code._ ..```pyth
+00000d20: 6f6e 0a23 2049 6d70 6f72 7420 636c 6965  on.# Import clie
+00000d30: 6e74 0a66 726f 6d20 7870 616e 7365 2e63  nt.from xpanse.c
+00000d40: 6c69 656e 7420 696d 706f 7274 2058 7061  lient import Xpa
+00000d50: 6e73 6543 6c69 656e 740a 0a23 2049 6e69  nseClient..# Ini
+00000d60: 7469 616c 697a 6520 636c 6965 6e74 202d  tialize client -
+00000d70: 2054 4849 5320 4953 204e 4f54 2052 4543   THIS IS NOT REC
+00000d80: 4f4d 4d45 4e44 4544 2c20 5345 5420 454e  OMMENDED, SET EN
+00000d90: 5649 524f 4e4d 454e 5420 5641 5249 4142  VIRONMENT VARIAB
+00000da0: 4c45 5320 494e 5354 4541 440a 636c 6965  LES INSTEAD.clie
+00000db0: 6e74 203d 2058 7061 6e73 6543 6c69 656e  nt = XpanseClien
+00000dc0: 7428 7572 6c3d 2268 7474 7073 3a2f 2f6d  t(url="https://m
+00000dd0: 792d 636f 6d70 616e 792e 6372 7478 2e75  y-company.crtx.u
+00000de0: 732e 7061 6c6f 616c 746f 6e65 7477 6f72  s.paloaltonetwor
+00000df0: 6b73 2e63 6f6d 222c 0a20 2020 2020 2020  ks.com",.       
+00000e00: 2020 2020 2020 2020 2020 2020 2020 2061                 a
+00000e10: 7069 5f6b 6579 3d22 7878 7878 7878 7878  pi_key="xxxxxxxx
+00000e20: 7878 7878 7878 7841 7069 4b65 7978 7878  xxxxxxxApiKeyxxx
+00000e30: 7878 7878 7878 7878 7878 7878 222c 0a20  xxxxxxxxxxxx",. 
+00000e40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000e50: 2020 2020 2061 7069 5f6b 6579 5f69 643d       api_key_id=
+00000e60: 3129 0a60 6060 0a0a 4c6f 6767 696e 670a  1).```..Logging.
+00000e70: 2d2d 2d2d 2d2d 2d0a 4c6f 6767 696e 6720  -------.Logging 
+00000e80: 6973 2068 616e 646c 6564 2074 6872 6f75  is handled throu
+00000e90: 6768 2074 6865 2070 7974 686f 6e20 6c6f  gh the python lo
+00000ea0: 6767 696e 6720 7061 636b 6167 652e 2054  gging package. T
+00000eb0: 6f20 656e 6162 6c65 2064 6966 6665 7265  o enable differe
+00000ec0: 6e74 206c 6576 656c 7320 6f66 2076 6572  nt levels of ver
+00000ed0: 626f 7369 7479 2069 6e20 796f 7572 2073  bosity in your s
+00000ee0: 6372 6970 7473 2079 6f75 2063 616e 2064  cripts you can d
+00000ef0: 6f20 7468 6520 666f 6c6c 6f77 696e 673a  o the following:
+00000f00: 0a0a 6060 6070 7974 686f 6e0a 696d 706f  ..```python.impo
+00000f10: 7274 206c 6f67 6769 6e67 0a0a 2320 5365  rt logging..# Se
+00000f20: 7420 7468 6520 6c6f 6767 696e 6720 6c65  t the logging le
+00000f30: 7665 6c0a 6c6f 6767 696e 672e 6261 7369  vel.logging.basi
+00000f40: 6343 6f6e 6669 6728 6c65 7665 6c3d 6c6f  cConfig(level=lo
+00000f50: 6767 696e 672e 4445 4255 4729 0a60 6060  gging.DEBUG).```
+00000f60: 0a0a 596f 7520 6361 6e20 7265 6164 206d  ..You can read m
+00000f70: 6f72 6520 6174 203c 6874 7470 733a 2f2f  ore at <https://
+00000f80: 646f 6373 2e70 7974 686f 6e2e 6f72 672f  docs.python.org/
+00000f90: 332f 6c69 6272 6172 792f 6c6f 6767 696e  3/library/loggin
+00000fa0: 672e 6874 6d6c 3e2e 0a0a 0a              g.html>....
```

