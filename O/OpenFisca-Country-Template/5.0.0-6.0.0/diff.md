# Comparing `tmp/OpenFisca-Country-Template-5.0.0.tar.gz` & `tmp/OpenFisca-Country-Template-6.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/country-template/country-template/dist/.tmp-rky5rx33/OpenFisca-Country-Template-5.0.0.tar", last modified: Mon Dec 12 07:45:36 2022, max compression
+gzip compressed data, was "OpenFisca-Country-Template-6.0.0.tar", last modified: Thu Jun  8 15:23:50 2023, max compression
```

## Comparing `OpenFisca-Country-Template-5.0.0.tar` & `OpenFisca-Country-Template-6.0.0.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-12 07:45:36.000000 OpenFisca-Country-Template-5.0.0/
--rw-r--r--   0 runner    (1001) docker     (122)    17420 2022-12-12 07:45:17.000000 OpenFisca-Country-Template-5.0.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (122)    34519 2022-12-12 07:45:17.000000 OpenFisca-Country-Template-5.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)       47 2022-12-12 07:45:17.000000 OpenFisca-Country-Template-5.0.0/MANIFEST.in
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-12 07:45:36.000000 OpenFisca-Country-Template-5.0.0/OpenFisca_Country_Template.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     9498 2022-12-12 07:45:36.000000 OpenFisca-Country-Template-5.0.0/OpenFisca_Country_Template.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2720 2022-12-12 07:45:36.000000 OpenFisca-Country-Template-5.0.0/OpenFisca_Country_Template.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-12-12 07:45:36.000000 OpenFisca-Country-Template-5.0.0/OpenFisca_Country_Template.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      501 2022-12-12 07:45:36.000000 OpenFisca-Country-Template-5.0.0/OpenFisca_Country_Template.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       27 2022-12-12 07:45:36.000000 OpenFisca-Country-Template-5.0.0/OpenFisca_Country_Template.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)     9498 2022-12-12 07:45:36.000000 OpenFisca-Country-Template-5.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     8628 2022-12-12 07:45:17.000000 OpenFisca-Country-Template-5.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-12 07:45:36.000000 OpenFisca-Country-Template-5.0.0/openfisca_country_template/
--rw-r--r--   0 runner    (1001) docker     (122)     1770 2022-12-12 07:45:17.000000 OpenFisca-Country-Template-5.0.0/openfisca_country_template/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2697 2022-12-12 07:45:17.000000 OpenFisca-Country-Template-5.0.0/openfisca_country_template/entities.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-12 07:45:36.000000 OpenFisca-Country-Template-5.0.0/openfisca_country_template/parameters/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-12 07:45:36.000000 OpenFisca-Country-Template-5.0.0/openfisca_country_template/parameters/benefits/
--rw-r--r--   0 runner    (1001) docker     (122)      312 2022-12-12 07:45:17.000000 OpenFisca-Country-Template-5.0.0/openfisca_country_template/parameters/benefits/basic_income.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      411 2022-12-12 07:45:17.000000 OpenFisca-Country-Template-5.0.0/openfisca_country_template/parameters/benefits/housing_allowance.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      447 2022-12-12 07:45:17.000000 OpenFisca-Country-Template-5.0.0/openfisca_country_template/parameters/benefits/index.yaml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-12 07:45:36.000000 OpenFisca-Country-Template-5.0.0/openfisca_country_template/parameters/benefits/parenting_allowance/
--rw-r--r--   0 runner    (1001) docker     (122)      326 2022-12-12 07:45:17.000000 OpenFisca-Country-Template-5.0.0/openfisca_country_template/parameters/benefits/parenting_allowance/amount.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      356 2022-12-12 07:45:17.000000 OpenFisca-Country-Template-5.0.0/openfisca_country_template/parameters/benefits/parenting_allowance/income_threshold.yaml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-12 07:45:36.000000 OpenFisca-Country-Template-5.0.0/openfisca_country_template/parameters/general/
--rw-r--r--   0 runner    (1001) docker     (122)      191 2022-12-12 07:45:17.000000 OpenFisca-Country-Template-5.0.0/openfisca_country_template/parameters/general/age_of_majority.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      287 2022-12-12 07:45:17.000000 OpenFisca-Country-Template-5.0.0/openfisca_country_template/parameters/general/age_of_retirement.yaml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-12 07:45:36.000000 OpenFisca-Country-Template-5.0.0/openfisca_country_template/parameters/taxes/
--rw-r--r--   0 runner    (1001) docker     (122)      459 2022-12-12 07:45:17.000000 OpenFisca-Country-Template-5.0.0/openfisca_country_template/parameters/taxes/housing_tax.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      403 2022-12-12 07:45:17.000000 OpenFisca-Country-Template-5.0.0/openfisca_country_template/parameters/taxes/income_tax_rate.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      804 2022-12-12 07:45:17.000000 OpenFisca-Country-Template-5.0.0/openfisca_country_template/parameters/taxes/social_security_contribution.yaml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-12 07:45:36.000000 OpenFisca-Country-Template-5.0.0/openfisca_country_template/reforms/
--rw-r--r--   0 runner    (1001) docker     (122)      223 2022-12-12 07:45:17.000000 OpenFisca-Country-Template-5.0.0/openfisca_country_template/reforms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1795 2022-12-12 07:45:17.000000 OpenFisca-Country-Template-5.0.0/openfisca_country_template/reforms/add_dynamic_variable.py
--rw-r--r--   0 runner    (1001) docker     (122)     1779 2022-12-12 07:45:17.000000 OpenFisca-Country-Template-5.0.0/openfisca_country_template/reforms/add_new_tax.py
--rw-r--r--   0 runner    (1001) docker     (122)     1213 2022-12-12 07:45:17.000000 OpenFisca-Country-Template-5.0.0/openfisca_country_template/reforms/flat_social_security_contribution.py
--rw-r--r--   0 runner    (1001) docker     (122)     2082 2022-12-12 07:45:17.000000 OpenFisca-Country-Template-5.0.0/openfisca_country_template/reforms/modify_social_security_taxation.py
--rw-r--r--   0 runner    (1001) docker     (122)      866 2022-12-12 07:45:17.000000 OpenFisca-Country-Template-5.0.0/openfisca_country_template/reforms/removal_basic_income.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-12 07:45:36.000000 OpenFisca-Country-Template-5.0.0/openfisca_country_template/situation_examples/
--rw-r--r--   0 runner    (1001) docker     (122)      419 2022-12-12 07:45:17.000000 OpenFisca-Country-Template-5.0.0/openfisca_country_template/situation_examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      801 2022-12-12 07:45:17.000000 OpenFisca-Country-Template-5.0.0/openfisca_country_template/situation_examples/couple.json
--rw-r--r--   0 runner    (1001) docker     (122)      455 2022-12-12 07:45:17.000000 OpenFisca-Country-Template-5.0.0/openfisca_country_template/situation_examples/housing.json
--rw-r--r--   0 runner    (1001) docker     (122)      294 2022-12-12 07:45:17.000000 OpenFisca-Country-Template-5.0.0/openfisca_country_template/situation_examples/single.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-12 07:45:36.000000 OpenFisca-Country-Template-5.0.0/openfisca_country_template/tests/
--rw-r--r--   0 runner    (1001) docker     (122)      748 2022-12-12 07:45:17.000000 OpenFisca-Country-Template-5.0.0/openfisca_country_template/tests/age.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     1093 2022-12-12 07:45:17.000000 OpenFisca-Country-Template-5.0.0/openfisca_country_template/tests/basic_income.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     1268 2022-12-12 07:45:17.000000 OpenFisca-Country-Template-5.0.0/openfisca_country_template/tests/disposable_income.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      445 2022-12-12 07:45:17.000000 OpenFisca-Country-Template-5.0.0/openfisca_country_template/tests/housing_allowance.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      778 2022-12-12 07:45:17.000000 OpenFisca-Country-Template-5.0.0/openfisca_country_template/tests/housing_tax.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      278 2022-12-12 07:45:17.000000 OpenFisca-Country-Template-5.0.0/openfisca_country_template/tests/income_tax.yaml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-12 07:45:36.000000 OpenFisca-Country-Template-5.0.0/openfisca_country_template/tests/reforms/
--rw-r--r--   0 runner    (1001) docker     (122)      450 2022-12-12 07:45:17.000000 OpenFisca-Country-Template-5.0.0/openfisca_country_template/tests/reforms/add_dynamic_variable.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      681 2022-12-12 07:45:17.000000 OpenFisca-Country-Template-5.0.0/openfisca_country_template/tests/reforms/add_new_tax.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     1162 2022-12-12 07:45:17.000000 OpenFisca-Country-Template-5.0.0/openfisca_country_template/tests/reforms/modify_social_security_taxation.yaml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-12 07:45:36.000000 OpenFisca-Country-Template-5.0.0/openfisca_country_template/tests/situations/
--rw-r--r--   0 runner    (1001) docker     (122)      838 2022-12-12 07:45:17.000000 OpenFisca-Country-Template-5.0.0/openfisca_country_template/tests/situations/income_tax.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      915 2022-12-12 07:45:17.000000 OpenFisca-Country-Template-5.0.0/openfisca_country_template/tests/situations/parenting_allowance.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      961 2022-12-12 07:45:17.000000 OpenFisca-Country-Template-5.0.0/openfisca_country_template/tests/social_security_contribution.yaml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-12 07:45:36.000000 OpenFisca-Country-Template-5.0.0/openfisca_country_template/variables/
--rw-r--r--   0 runner    (1001) docker     (122)      185 2022-12-12 07:45:17.000000 OpenFisca-Country-Template-5.0.0/openfisca_country_template/variables/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5584 2022-12-12 07:45:17.000000 OpenFisca-Country-Template-5.0.0/openfisca_country_template/variables/benefits.py
--rw-r--r--   0 runner    (1001) docker     (122)     1949 2022-12-12 07:45:17.000000 OpenFisca-Country-Template-5.0.0/openfisca_country_template/variables/demographics.py
--rw-r--r--   0 runner    (1001) docker     (122)     1850 2022-12-12 07:45:17.000000 OpenFisca-Country-Template-5.0.0/openfisca_country_template/variables/housing.py
--rw-r--r--   0 runner    (1001) docker     (122)     1703 2022-12-12 07:45:17.000000 OpenFisca-Country-Template-5.0.0/openfisca_country_template/variables/income.py
--rw-r--r--   0 runner    (1001) docker     (122)     1766 2022-12-12 07:45:17.000000 OpenFisca-Country-Template-5.0.0/openfisca_country_template/variables/stats.py
--rw-r--r--   0 runner    (1001) docker     (122)     3426 2022-12-12 07:45:17.000000 OpenFisca-Country-Template-5.0.0/openfisca_country_template/variables/taxes.py
--rw-r--r--   0 runner    (1001) docker     (122)      645 2022-12-12 07:45:36.000000 OpenFisca-Country-Template-5.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     2467 2022-12-12 07:45:17.000000 OpenFisca-Country-Template-5.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-08 15:23:50.938693 OpenFisca-Country-Template-6.0.0/
+-rw-r--r--   0 runner    (1001) docker     (122)    17706 2023-06-08 15:23:27.000000 OpenFisca-Country-Template-6.0.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (122)    34519 2023-06-08 15:23:27.000000 OpenFisca-Country-Template-6.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)       47 2023-06-08 15:23:27.000000 OpenFisca-Country-Template-6.0.0/MANIFEST.in
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-08 15:23:50.934693 OpenFisca-Country-Template-6.0.0/OpenFisca_Country_Template.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     9398 2023-06-08 15:23:50.000000 OpenFisca-Country-Template-6.0.0/OpenFisca_Country_Template.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2720 2023-06-08 15:23:50.000000 OpenFisca-Country-Template-6.0.0/OpenFisca_Country_Template.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-08 15:23:50.000000 OpenFisca-Country-Template-6.0.0/OpenFisca_Country_Template.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      484 2023-06-08 15:23:50.000000 OpenFisca-Country-Template-6.0.0/OpenFisca_Country_Template.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       27 2023-06-08 15:23:50.000000 OpenFisca-Country-Template-6.0.0/OpenFisca_Country_Template.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     9398 2023-06-08 15:23:50.938693 OpenFisca-Country-Template-6.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     8527 2023-06-08 15:23:27.000000 OpenFisca-Country-Template-6.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-08 15:23:50.934693 OpenFisca-Country-Template-6.0.0/openfisca_country_template/
+-rw-r--r--   0 runner    (1001) docker     (122)     1770 2023-06-08 15:23:27.000000 OpenFisca-Country-Template-6.0.0/openfisca_country_template/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2697 2023-06-08 15:23:27.000000 OpenFisca-Country-Template-6.0.0/openfisca_country_template/entities.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-08 15:23:50.934693 OpenFisca-Country-Template-6.0.0/openfisca_country_template/parameters/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-08 15:23:50.934693 OpenFisca-Country-Template-6.0.0/openfisca_country_template/parameters/benefits/
+-rw-r--r--   0 runner    (1001) docker     (122)      312 2023-06-08 15:23:27.000000 OpenFisca-Country-Template-6.0.0/openfisca_country_template/parameters/benefits/basic_income.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      411 2023-06-08 15:23:27.000000 OpenFisca-Country-Template-6.0.0/openfisca_country_template/parameters/benefits/housing_allowance.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      447 2023-06-08 15:23:27.000000 OpenFisca-Country-Template-6.0.0/openfisca_country_template/parameters/benefits/index.yaml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-08 15:23:50.934693 OpenFisca-Country-Template-6.0.0/openfisca_country_template/parameters/benefits/parenting_allowance/
+-rw-r--r--   0 runner    (1001) docker     (122)      326 2023-06-08 15:23:27.000000 OpenFisca-Country-Template-6.0.0/openfisca_country_template/parameters/benefits/parenting_allowance/amount.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      356 2023-06-08 15:23:27.000000 OpenFisca-Country-Template-6.0.0/openfisca_country_template/parameters/benefits/parenting_allowance/income_threshold.yaml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-08 15:23:50.934693 OpenFisca-Country-Template-6.0.0/openfisca_country_template/parameters/general/
+-rw-r--r--   0 runner    (1001) docker     (122)      191 2023-06-08 15:23:27.000000 OpenFisca-Country-Template-6.0.0/openfisca_country_template/parameters/general/age_of_majority.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      287 2023-06-08 15:23:27.000000 OpenFisca-Country-Template-6.0.0/openfisca_country_template/parameters/general/age_of_retirement.yaml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-08 15:23:50.934693 OpenFisca-Country-Template-6.0.0/openfisca_country_template/parameters/taxes/
+-rw-r--r--   0 runner    (1001) docker     (122)      459 2023-06-08 15:23:27.000000 OpenFisca-Country-Template-6.0.0/openfisca_country_template/parameters/taxes/housing_tax.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      403 2023-06-08 15:23:27.000000 OpenFisca-Country-Template-6.0.0/openfisca_country_template/parameters/taxes/income_tax_rate.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      804 2023-06-08 15:23:27.000000 OpenFisca-Country-Template-6.0.0/openfisca_country_template/parameters/taxes/social_security_contribution.yaml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-08 15:23:50.938693 OpenFisca-Country-Template-6.0.0/openfisca_country_template/reforms/
+-rw-r--r--   0 runner    (1001) docker     (122)      223 2023-06-08 15:23:27.000000 OpenFisca-Country-Template-6.0.0/openfisca_country_template/reforms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1795 2023-06-08 15:23:27.000000 OpenFisca-Country-Template-6.0.0/openfisca_country_template/reforms/add_dynamic_variable.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1779 2023-06-08 15:23:27.000000 OpenFisca-Country-Template-6.0.0/openfisca_country_template/reforms/add_new_tax.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1213 2023-06-08 15:23:27.000000 OpenFisca-Country-Template-6.0.0/openfisca_country_template/reforms/flat_social_security_contribution.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2082 2023-06-08 15:23:27.000000 OpenFisca-Country-Template-6.0.0/openfisca_country_template/reforms/modify_social_security_taxation.py
+-rw-r--r--   0 runner    (1001) docker     (122)      866 2023-06-08 15:23:27.000000 OpenFisca-Country-Template-6.0.0/openfisca_country_template/reforms/removal_basic_income.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-08 15:23:50.938693 OpenFisca-Country-Template-6.0.0/openfisca_country_template/situation_examples/
+-rw-r--r--   0 runner    (1001) docker     (122)      419 2023-06-08 15:23:27.000000 OpenFisca-Country-Template-6.0.0/openfisca_country_template/situation_examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      801 2023-06-08 15:23:27.000000 OpenFisca-Country-Template-6.0.0/openfisca_country_template/situation_examples/couple.json
+-rw-r--r--   0 runner    (1001) docker     (122)      455 2023-06-08 15:23:27.000000 OpenFisca-Country-Template-6.0.0/openfisca_country_template/situation_examples/housing.json
+-rw-r--r--   0 runner    (1001) docker     (122)      294 2023-06-08 15:23:27.000000 OpenFisca-Country-Template-6.0.0/openfisca_country_template/situation_examples/single.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-08 15:23:50.938693 OpenFisca-Country-Template-6.0.0/openfisca_country_template/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)      748 2023-06-08 15:23:27.000000 OpenFisca-Country-Template-6.0.0/openfisca_country_template/tests/age.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     1093 2023-06-08 15:23:27.000000 OpenFisca-Country-Template-6.0.0/openfisca_country_template/tests/basic_income.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     1268 2023-06-08 15:23:27.000000 OpenFisca-Country-Template-6.0.0/openfisca_country_template/tests/disposable_income.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      445 2023-06-08 15:23:27.000000 OpenFisca-Country-Template-6.0.0/openfisca_country_template/tests/housing_allowance.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      778 2023-06-08 15:23:27.000000 OpenFisca-Country-Template-6.0.0/openfisca_country_template/tests/housing_tax.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      278 2023-06-08 15:23:27.000000 OpenFisca-Country-Template-6.0.0/openfisca_country_template/tests/income_tax.yaml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-08 15:23:50.938693 OpenFisca-Country-Template-6.0.0/openfisca_country_template/tests/reforms/
+-rw-r--r--   0 runner    (1001) docker     (122)      450 2023-06-08 15:23:27.000000 OpenFisca-Country-Template-6.0.0/openfisca_country_template/tests/reforms/add_dynamic_variable.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      681 2023-06-08 15:23:27.000000 OpenFisca-Country-Template-6.0.0/openfisca_country_template/tests/reforms/add_new_tax.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     1162 2023-06-08 15:23:27.000000 OpenFisca-Country-Template-6.0.0/openfisca_country_template/tests/reforms/modify_social_security_taxation.yaml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-08 15:23:50.938693 OpenFisca-Country-Template-6.0.0/openfisca_country_template/tests/situations/
+-rw-r--r--   0 runner    (1001) docker     (122)      838 2023-06-08 15:23:27.000000 OpenFisca-Country-Template-6.0.0/openfisca_country_template/tests/situations/income_tax.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      915 2023-06-08 15:23:27.000000 OpenFisca-Country-Template-6.0.0/openfisca_country_template/tests/situations/parenting_allowance.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      961 2023-06-08 15:23:27.000000 OpenFisca-Country-Template-6.0.0/openfisca_country_template/tests/social_security_contribution.yaml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-08 15:23:50.938693 OpenFisca-Country-Template-6.0.0/openfisca_country_template/variables/
+-rw-r--r--   0 runner    (1001) docker     (122)      185 2023-06-08 15:23:27.000000 OpenFisca-Country-Template-6.0.0/openfisca_country_template/variables/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5584 2023-06-08 15:23:27.000000 OpenFisca-Country-Template-6.0.0/openfisca_country_template/variables/benefits.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1949 2023-06-08 15:23:27.000000 OpenFisca-Country-Template-6.0.0/openfisca_country_template/variables/demographics.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1850 2023-06-08 15:23:27.000000 OpenFisca-Country-Template-6.0.0/openfisca_country_template/variables/housing.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1703 2023-06-08 15:23:27.000000 OpenFisca-Country-Template-6.0.0/openfisca_country_template/variables/income.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1766 2023-06-08 15:23:27.000000 OpenFisca-Country-Template-6.0.0/openfisca_country_template/variables/stats.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3422 2023-06-08 15:23:27.000000 OpenFisca-Country-Template-6.0.0/openfisca_country_template/variables/taxes.py
+-rw-r--r--   0 runner    (1001) docker     (122)      645 2023-06-08 15:23:50.938693 OpenFisca-Country-Template-6.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     2454 2023-06-08 15:23:27.000000 OpenFisca-Country-Template-6.0.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `OpenFisca-Country-Template-5.0.0/CHANGELOG.md` & `OpenFisca-Country-Template-6.0.0/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,17 @@
 # Changelog
 
+# 6.0.0 [#129](https://github.com/openfisca/country-template/pull/129)
+
+* Technical improvement.
+* Impacted periods: all.
+* Impacted areas: all.
+* Details:
+  - Upgrade every dependencies & use their latest versions to use Python 3.9 and 3.10 and drop support of Python versions < 3.9 .
+
 # 5.0.0 [#128](https://github.com/openfisca/country-template/pull/128)
 
 #### New features
 
 - Upgrade Web API specification to OpenAPI v3.
 
 #### Breaking changes
@@ -18,15 +26,15 @@
 * Technical improvement.
 * Details:
   - Expire deprecated class `Bracket`.
   - Functionality is now provided by `ParameterScaleBracket`
 
 ### 3.13.3 - [#122](https://github.com/openfisca/country-template/pull/122)
 
-* Technical improvement. 
+* Technical improvement.
 * Details:
   - Add pull request as GitHub Actions workflow trigger
 
 ### 3.13.2 - [#123](https://github.com/openfisca/country-template/pull/123)
 
 * Technical improvement.
 * Details:
```

### Comparing `OpenFisca-Country-Template-5.0.0/LICENSE` & `OpenFisca-Country-Template-6.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `OpenFisca-Country-Template-5.0.0/OpenFisca_Country_Template.egg-info/PKG-INFO` & `OpenFisca-Country-Template-6.0.0/OpenFisca_Country_Template.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: OpenFisca-Country-Template
-Version: 5.0.0
+Version: 6.0.0
 Summary: OpenFisca tax and benefit system for Country-Template
 Home-page: https://github.com/openfisca/country-template
 Author: OpenFisca Team
 Author-email: contact@openfisca.org
 License: http://www.fsf.org/licensing/licenses/agpl-3.0.html
 Keywords: benefit microsimulation social tax
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # OpenFisca Country-Template
 
@@ -71,17 +71,17 @@
 
 ## Packaging your Country Package for Distribution
 
 Country packages are python distributions. To distribute your package via `pip`, follow the steps given by the [Python Packaging Authority](https://python-packaging-user-guide.readthedocs.io/tutorials/distributing-packages/#packaging-your-project).
 
 ## Install Instructions for Users and Contributors
 
-This package requires [Python 3.7](https://www.python.org/downloads/release/python-370/). More recent versions should work, but are not tested.
+This package requires [Python 3.9](https://www.python.org/downloads/release/python-390/). More recent versions should work, but are not tested.
 
-All platforms that can execute Python are supported, which includes GNU/Linux, macOS and Microsoft Windows (in which case we recommend using [ConEmu](https://conemu.github.io/) instead of the default console).
+All platforms that can execute Python are supported, which includes GNU/Linux, macOS and Microsoft Windows.
 
 ### Setting-up a Virtual Environment with venv
 
 In order to limit dependencies conflicts, we recommend using a [virtual environment](https://www.python.org/dev/peps/pep-0405/) with [venv](https://docs.python.org/3/library/venv.html).
 
 - A [venv](https://docs.python.org/3/library/venv.html) is a project specific environment created to suit the needs of the project you are working on.
 
@@ -111,15 +111,15 @@
 For more advanced uses, head to the [Advanced Installation](#advanced-installation-git-clone).
 
 #### Install this Country Package with Pip Install
 
 Inside your venv, check the prerequisites:
 
 ```sh
-python --version  # should print "Python 3.7.xx".
+python --version  # should print "Python 3.9.xx".
 ```
 
 ```sh
 pip --version  # should print at least 9.0.
 # if not, run "pip install --upgrade pip"
 ```
 Install the Country Package:
@@ -153,15 +153,15 @@
 First, make sure [Git](https://www.git-scm.com/) is installed on your machine.
 
 Set your working directory to the location where you want this OpenFisca Country Package cloned.
 
 Inside your venv, check the prerequisites:
 
 ```sh
-python --version  # should print "Python 3.7.xx".
+python --version  # should print "Python 3.9.xx".
 ```
 
 ```sh
 pip --version  # should print at least 9.0.
 # if not, run "pip install --upgrade pip"
 ```
 Clone this Country Package on your machine:
```

### Comparing `OpenFisca-Country-Template-5.0.0/OpenFisca_Country_Template.egg-info/SOURCES.txt` & `OpenFisca-Country-Template-6.0.0/OpenFisca_Country_Template.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `OpenFisca-Country-Template-5.0.0/PKG-INFO` & `OpenFisca-Country-Template-6.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: OpenFisca-Country-Template
-Version: 5.0.0
+Version: 6.0.0
 Summary: OpenFisca tax and benefit system for Country-Template
 Home-page: https://github.com/openfisca/country-template
 Author: OpenFisca Team
 Author-email: contact@openfisca.org
 License: http://www.fsf.org/licensing/licenses/agpl-3.0.html
 Keywords: benefit microsimulation social tax
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # OpenFisca Country-Template
 
@@ -71,17 +71,17 @@
 
 ## Packaging your Country Package for Distribution
 
 Country packages are python distributions. To distribute your package via `pip`, follow the steps given by the [Python Packaging Authority](https://python-packaging-user-guide.readthedocs.io/tutorials/distributing-packages/#packaging-your-project).
 
 ## Install Instructions for Users and Contributors
 
-This package requires [Python 3.7](https://www.python.org/downloads/release/python-370/). More recent versions should work, but are not tested.
+This package requires [Python 3.9](https://www.python.org/downloads/release/python-390/). More recent versions should work, but are not tested.
 
-All platforms that can execute Python are supported, which includes GNU/Linux, macOS and Microsoft Windows (in which case we recommend using [ConEmu](https://conemu.github.io/) instead of the default console).
+All platforms that can execute Python are supported, which includes GNU/Linux, macOS and Microsoft Windows.
 
 ### Setting-up a Virtual Environment with venv
 
 In order to limit dependencies conflicts, we recommend using a [virtual environment](https://www.python.org/dev/peps/pep-0405/) with [venv](https://docs.python.org/3/library/venv.html).
 
 - A [venv](https://docs.python.org/3/library/venv.html) is a project specific environment created to suit the needs of the project you are working on.
 
@@ -111,15 +111,15 @@
 For more advanced uses, head to the [Advanced Installation](#advanced-installation-git-clone).
 
 #### Install this Country Package with Pip Install
 
 Inside your venv, check the prerequisites:
 
 ```sh
-python --version  # should print "Python 3.7.xx".
+python --version  # should print "Python 3.9.xx".
 ```
 
 ```sh
 pip --version  # should print at least 9.0.
 # if not, run "pip install --upgrade pip"
 ```
 Install the Country Package:
@@ -153,15 +153,15 @@
 First, make sure [Git](https://www.git-scm.com/) is installed on your machine.
 
 Set your working directory to the location where you want this OpenFisca Country Package cloned.
 
 Inside your venv, check the prerequisites:
 
 ```sh
-python --version  # should print "Python 3.7.xx".
+python --version  # should print "Python 3.9.xx".
 ```
 
 ```sh
 pip --version  # should print at least 9.0.
 # if not, run "pip install --upgrade pip"
 ```
 Clone this Country Package on your machine:
```

### Comparing `OpenFisca-Country-Template-5.0.0/README.md` & `OpenFisca-Country-Template-6.0.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -50,17 +50,17 @@
 
 ## Packaging your Country Package for Distribution
 
 Country packages are python distributions. To distribute your package via `pip`, follow the steps given by the [Python Packaging Authority](https://python-packaging-user-guide.readthedocs.io/tutorials/distributing-packages/#packaging-your-project).
 
 ## Install Instructions for Users and Contributors
 
-This package requires [Python 3.7](https://www.python.org/downloads/release/python-370/). More recent versions should work, but are not tested.
+This package requires [Python 3.9](https://www.python.org/downloads/release/python-390/). More recent versions should work, but are not tested.
 
-All platforms that can execute Python are supported, which includes GNU/Linux, macOS and Microsoft Windows (in which case we recommend using [ConEmu](https://conemu.github.io/) instead of the default console).
+All platforms that can execute Python are supported, which includes GNU/Linux, macOS and Microsoft Windows.
 
 ### Setting-up a Virtual Environment with venv
 
 In order to limit dependencies conflicts, we recommend using a [virtual environment](https://www.python.org/dev/peps/pep-0405/) with [venv](https://docs.python.org/3/library/venv.html).
 
 - A [venv](https://docs.python.org/3/library/venv.html) is a project specific environment created to suit the needs of the project you are working on.
 
@@ -90,15 +90,15 @@
 For more advanced uses, head to the [Advanced Installation](#advanced-installation-git-clone).
 
 #### Install this Country Package with Pip Install
 
 Inside your venv, check the prerequisites:
 
 ```sh
-python --version  # should print "Python 3.7.xx".
+python --version  # should print "Python 3.9.xx".
 ```
 
 ```sh
 pip --version  # should print at least 9.0.
 # if not, run "pip install --upgrade pip"
 ```
 Install the Country Package:
@@ -132,15 +132,15 @@
 First, make sure [Git](https://www.git-scm.com/) is installed on your machine.
 
 Set your working directory to the location where you want this OpenFisca Country Package cloned.
 
 Inside your venv, check the prerequisites:
 
 ```sh
-python --version  # should print "Python 3.7.xx".
+python --version  # should print "Python 3.9.xx".
 ```
 
 ```sh
 pip --version  # should print at least 9.0.
 # if not, run "pip install --upgrade pip"
 ```
 Clone this Country Package on your machine:
@@ -194,8 +194,8 @@
 
 Substitute your package's country name for `openfisca_country_template` below:
 
 ```sh
 curl -X POST -H "Content-Type: application/json" \
   -d @./openfisca_country_template/situation_examples/couple.json \
   http://localhost:5000/calculate
-```
+```
```

### Comparing `OpenFisca-Country-Template-5.0.0/openfisca_country_template/__init__.py` & `OpenFisca-Country-Template-6.0.0/openfisca_country_template/__init__.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Country-Template-5.0.0/openfisca_country_template/entities.py` & `OpenFisca-Country-Template-6.0.0/openfisca_country_template/entities.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Country-Template-5.0.0/openfisca_country_template/parameters/taxes/social_security_contribution.yaml` & `OpenFisca-Country-Template-6.0.0/openfisca_country_template/parameters/taxes/social_security_contribution.yaml`

 * *Files identical despite different names*

### Comparing `OpenFisca-Country-Template-5.0.0/openfisca_country_template/reforms/add_dynamic_variable.py` & `OpenFisca-Country-Template-6.0.0/openfisca_country_template/reforms/add_dynamic_variable.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Country-Template-5.0.0/openfisca_country_template/reforms/add_new_tax.py` & `OpenFisca-Country-Template-6.0.0/openfisca_country_template/reforms/add_new_tax.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Country-Template-5.0.0/openfisca_country_template/reforms/flat_social_security_contribution.py` & `OpenFisca-Country-Template-6.0.0/openfisca_country_template/reforms/flat_social_security_contribution.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Country-Template-5.0.0/openfisca_country_template/reforms/modify_social_security_taxation.py` & `OpenFisca-Country-Template-6.0.0/openfisca_country_template/reforms/modify_social_security_taxation.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Country-Template-5.0.0/openfisca_country_template/reforms/removal_basic_income.py` & `OpenFisca-Country-Template-6.0.0/openfisca_country_template/reforms/removal_basic_income.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Country-Template-5.0.0/openfisca_country_template/situation_examples/couple.json` & `OpenFisca-Country-Template-6.0.0/openfisca_country_template/situation_examples/couple.json`

 * *Files identical despite different names*

### Comparing `OpenFisca-Country-Template-5.0.0/openfisca_country_template/tests/age.yaml` & `OpenFisca-Country-Template-6.0.0/openfisca_country_template/tests/age.yaml`

 * *Files identical despite different names*

### Comparing `OpenFisca-Country-Template-5.0.0/openfisca_country_template/tests/basic_income.yaml` & `OpenFisca-Country-Template-6.0.0/openfisca_country_template/tests/basic_income.yaml`

 * *Files identical despite different names*

### Comparing `OpenFisca-Country-Template-5.0.0/openfisca_country_template/tests/disposable_income.yaml` & `OpenFisca-Country-Template-6.0.0/openfisca_country_template/tests/disposable_income.yaml`

 * *Files identical despite different names*

### Comparing `OpenFisca-Country-Template-5.0.0/openfisca_country_template/tests/housing_tax.yaml` & `OpenFisca-Country-Template-6.0.0/openfisca_country_template/tests/housing_tax.yaml`

 * *Files identical despite different names*

### Comparing `OpenFisca-Country-Template-5.0.0/openfisca_country_template/tests/reforms/add_new_tax.yaml` & `OpenFisca-Country-Template-6.0.0/openfisca_country_template/tests/reforms/add_new_tax.yaml`

 * *Files identical despite different names*

### Comparing `OpenFisca-Country-Template-5.0.0/openfisca_country_template/tests/reforms/modify_social_security_taxation.yaml` & `OpenFisca-Country-Template-6.0.0/openfisca_country_template/tests/reforms/modify_social_security_taxation.yaml`

 * *Files identical despite different names*

### Comparing `OpenFisca-Country-Template-5.0.0/openfisca_country_template/tests/situations/income_tax.yaml` & `OpenFisca-Country-Template-6.0.0/openfisca_country_template/tests/situations/income_tax.yaml`

 * *Files identical despite different names*

### Comparing `OpenFisca-Country-Template-5.0.0/openfisca_country_template/tests/situations/parenting_allowance.yaml` & `OpenFisca-Country-Template-6.0.0/openfisca_country_template/tests/situations/parenting_allowance.yaml`

 * *Files identical despite different names*

### Comparing `OpenFisca-Country-Template-5.0.0/openfisca_country_template/tests/social_security_contribution.yaml` & `OpenFisca-Country-Template-6.0.0/openfisca_country_template/tests/social_security_contribution.yaml`

 * *Files identical despite different names*

### Comparing `OpenFisca-Country-Template-5.0.0/openfisca_country_template/variables/benefits.py` & `OpenFisca-Country-Template-6.0.0/openfisca_country_template/variables/benefits.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Country-Template-5.0.0/openfisca_country_template/variables/demographics.py` & `OpenFisca-Country-Template-6.0.0/openfisca_country_template/variables/demographics.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Country-Template-5.0.0/openfisca_country_template/variables/housing.py` & `OpenFisca-Country-Template-6.0.0/openfisca_country_template/variables/housing.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Country-Template-5.0.0/openfisca_country_template/variables/income.py` & `OpenFisca-Country-Template-6.0.0/openfisca_country_template/variables/income.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Country-Template-5.0.0/openfisca_country_template/variables/stats.py` & `OpenFisca-Country-Template-6.0.0/openfisca_country_template/variables/stats.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Country-Template-5.0.0/openfisca_country_template/variables/taxes.py` & `OpenFisca-Country-Template-6.0.0/openfisca_country_template/variables/taxes.py`

 * *Files 4% similar despite different names*

```diff
@@ -72,12 +72,12 @@
         tax_params = parameters(period).taxes.housing_tax
         tax_amount = max_(accommodation_size * tax_params.rate, tax_params.minimal_amount)
 
         # `housing_occupancy_status` is an Enum variable
         occupancy_status = household("housing_occupancy_status", january)
         HousingOccupancyStatus = occupancy_status.possible_values  # Get the enum associated with the variable
         # To access an enum element, we use the `.` notation.
-        tenant = (occupancy_status == HousingOccupancyStatus.tenant)
-        owner = (occupancy_status == HousingOccupancyStatus.owner)
+        tenant = occupancy_status == HousingOccupancyStatus.tenant
+        owner = occupancy_status == HousingOccupancyStatus.owner
 
         # The tax is applied only if the household owns or rents its main residency
         return (owner + tenant) * tax_amount
```

### Comparing `OpenFisca-Country-Template-5.0.0/setup.cfg` & `OpenFisca-Country-Template-6.0.0/setup.cfg`

 * *Files identical despite different names*

