# Comparing `tmp/morph_kgc-2.5.0.tar.gz` & `tmp/morph_kgc-2.5.1.tar.gz`

## Comparing `morph_kgc-2.5.0.tar` & `morph_kgc-2.5.1.tar`

### file list

```diff
@@ -1,1365 +1,1365 @@
--rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/.zenodo.json
--rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/CITATION.cff
--rw-r--r--   0        0        0      882 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/CONTRIBUTING.md
--rw-r--r--   0        0        0     1744 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/mkdocs.yml
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/readthedocs.yml
--rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/.github/ISSUE_TEMPLATE/bug-report.md
--rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/.github/ISSUE_TEMPLATE/documentation-improvement.md
--rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/.github/ISSUE_TEMPLATE/feature-request.md
--rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/.github/ISSUE_TEMPLATE/installation-issue.md
--rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/.github/ISSUE_TEMPLATE/submit-quesion.md
--rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/.github/workflows/ci.yml
--rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/.github/workflows/pypi-publish.yml
--rw-r--r--   0        0        0    25137 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/docs/documentation.md
--rw-r--r--   0        0        0     2553 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/docs/faq.md
--rw-r--r--   0        0        0     3848 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/docs/index.md
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/docs/requirements.txt
--rw-r--r--   0        0        0     2516 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/docs/research.md
--rw-r--r--   0        0        0     5055 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/docs/why-morph-kgc.md
--rw-r--r--   0        0        0    58421 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/docs/assets/BASF.png
--rw-r--r--   0        0        0   172672 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/docs/assets/BASF.tif
--rw-r--r--   0        0        0    44456 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/docs/assets/datos40.png
--rw-r--r--   0        0        0    40106 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/docs/assets/entente.png
--rw-r--r--   0        0        0    33187 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/docs/assets/knowledgespaces.png
--rw-r--r--   0        0        0   299520 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/docs/assets/logo-oeg.png
--rw-r--r--   0        0        0   133582 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/docs/assets/logo-upm.png
--rw-r--r--   0        0        0    50123 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/docs/assets/logo.png
--rw-r--r--   0        0        0    60779 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/docs/assets/sigtrans.png
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/docs/stylesheets/extra.css
--rw-r--r--   0        0        0     3702 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/examples/README.md
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/examples/configuration-file/basic_config.ini
--rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/examples/configuration-file/default_config.ini
--rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/examples/configuration-file/oracle_config.ini
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/examples/csv/config.ini
--rw-r--r--   0        0        0    33628 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/examples/csv/mapping.csv.ttl
--rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/examples/csv/data/AGENCY.csv
--rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/examples/csv/data/CALENDAR.csv
--rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/examples/csv/data/CALENDAR_DATES.csv
--rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/examples/csv/data/FEED_INFO.csv
--rw-r--r--   0        0        0     3503 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/examples/csv/data/FREQUENCIES.csv
--rw-r--r--   0        0        0     2924 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/examples/csv/data/ROUTES.csv
--rw-r--r--   0        0        0     3171 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/examples/csv/data/SHAPES.csv
--rw-r--r--   0        0        0     4379 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/examples/csv/data/STOPS.csv
--rw-r--r--   0        0        0     4700 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/examples/csv/data/STOP_TIMES.csv
--rw-r--r--   0        0        0     6000 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/examples/csv/data/TRIPS.csv
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/examples/dataframe/config.ini
--rw-r--r--   0        0        0      859 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/examples/dataframe/kg_generation.py
--rw-r--r--   0        0        0     2319 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/examples/dataframe/mapping_rml.ttl
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/examples/dict/config.ini
--rw-r--r--   0        0        0     1512 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/examples/dict/kg_generation.py
--rw-r--r--   0        0        0     2330 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/examples/dict/mapping_rml.ttl
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/examples/json/config.ini
--rw-r--r--   0        0        0     3464 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/examples/json/data.json
--rw-r--r--   0        0        0     9731 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/examples/json/mapping.json.ttl
--rw-r--r--   0        0        0     1791 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/examples/json/mapping.json.yaml
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/examples/rdb/config.ini
--rw-r--r--   0        0        0    29169 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/examples/rdb/gtfs-rdb.r2rml.ttl
--rw-r--r--   0        0        0    13238 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/examples/tutorial/Morph-KGC.ipynb
--rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/examples/tutorial/README.md
--rw-r--r--   0        0        0    34542 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/examples/tutorial/mapping.gtfs.ttl
--rw-r--r--   0        0        0    26514 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/examples/tutorial/mapping.somef.ttl
--rw-r--r--   0        0        0    35086 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/examples/tutorial/oeg-upm_morph-kgc.json
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/examples/xml/config.ini
--rw-r--r--   0        0        0     3656 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/examples/xml/data.xml
--rw-r--r--   0        0        0     1756 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/examples/xml/mapping.xml.yaml
--rw-r--r--   0        0        0     9696 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/examples/xml/mappingOA.xml.ttl
--rw-r--r--   0        0        0     2978 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/src/morph_kgc/__init__.py
--rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/src/morph_kgc/__main__.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/src/morph_kgc/_version.py
--rw-r--r--   0        0        0     2205 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/src/morph_kgc/args_parser.py
--rw-r--r--   0        0        0    14497 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/src/morph_kgc/config.py
--rw-r--r--   0        0        0     8596 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/src/morph_kgc/constants.py
--rw-r--r--   0        0        0    25984 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/src/morph_kgc/materializer.py
--rw-r--r--   0        0        0     8924 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/src/morph_kgc/utils.py
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/src/morph_kgc/data_source/__init__.py
--rw-r--r--   0        0        0     8867 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/src/morph_kgc/data_source/data_file.py
--rw-r--r--   0        0        0     2406 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/src/morph_kgc/data_source/python_data.py
--rw-r--r--   0        0        0     7485 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/src/morph_kgc/data_source/relational_database.py
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/src/morph_kgc/fno/__init__.py
--rw-r--r--   0        0        0     8530 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/src/morph_kgc/fno/built_in_functions.py
--rw-r--r--   0        0        0     4636 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/src/morph_kgc/fno/fno_executer.py
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/src/morph_kgc/mapping/__init__.py
--rw-r--r--   0        0        0     6477 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/src/morph_kgc/mapping/mapping_constants.py
--rw-r--r--   0        0        0    37748 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/src/morph_kgc/mapping/mapping_parser.py
--rw-r--r--   0        0        0    20297 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/src/morph_kgc/mapping/mapping_partitioner.py
--rw-r--r--   0        0        0     1033 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/fno/RMLFNOTC0000-CSV/mapping.ttl
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/fno/RMLFNOTC0000-CSV/output.nq
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/fno/RMLFNOTC0000-CSV/student.csv
--rw-r--r--   0        0        0      841 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/fno/RMLFNOTC0000-CSV/test_RMLFNOTC0000-CSV.py
--rw-r--r--   0        0        0     1198 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/fno/RMLFNOTC0001-CSV/mapping.ttl
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/fno/RMLFNOTC0001-CSV/output.nq
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/fno/RMLFNOTC0001-CSV/student.csv
--rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/fno/RMLFNOTC0001-CSV/test_RMLFNOTC0001-CSV.py
--rw-r--r--   0        0        0     1196 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/fno/RMLFNOTC0002-CSV/mapping.ttl
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/fno/RMLFNOTC0002-CSV/output.nq
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/fno/RMLFNOTC0002-CSV/student.csv
--rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/fno/RMLFNOTC0002-CSV/test_RMLFNOTC0002-CSV.py
--rw-r--r--   0        0        0     1291 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/fno/RMLFNOTC0003-CSV/mapping.ttl
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/fno/RMLFNOTC0003-CSV/output.nq
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/fno/RMLFNOTC0003-CSV/student.csv
--rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/fno/RMLFNOTC0003-CSV/test_RMLFNOTC0003-CSV.py
--rw-r--r--   0        0        0     1202 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/fno/RMLFNOTC0004-CSV/mapping.ttl
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/fno/RMLFNOTC0004-CSV/output.nq
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/fno/RMLFNOTC0004-CSV/student.csv
--rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/fno/RMLFNOTC0004-CSV/test_RMLFNOTC0004-CSV.py
--rw-r--r--   0        0        0     1160 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/fno/RMLFNOTC0005-CSV/mapping.ttl
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/fno/RMLFNOTC0005-CSV/output.nq
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/fno/RMLFNOTC0005-CSV/student.csv
--rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/fno/RMLFNOTC0005-CSV/test_RMLFNOTC0005-CSV.py
--rw-r--r--   0        0        0     1233 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/fno/RMLFNOTC0006-CSV/mapping.ttl
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/fno/RMLFNOTC0006-CSV/output.nq
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/fno/RMLFNOTC0006-CSV/student.csv
--rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/fno/RMLFNOTC0006-CSV/test_RMLFNOTC0006-CSV.py
--rw-r--r--   0        0        0     1183 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/fno/RMLFNOTC0008-CSV/mapping.ttl
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/fno/RMLFNOTC0008-CSV/output.nq
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/fno/RMLFNOTC0008-CSV/student.csv
--rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/fno/RMLFNOTC0008-CSV/test_RMLFNOTC0008-CSV.py
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/fno/array_get_slice/article.tsv
--rw-r--r--   0        0        0     1766 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/fno/array_get_slice/mapping.ttl
--rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/fno/array_get_slice/output.nq
--rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/fno/array_get_slice/test_array_get_slice.py
--rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/fno/controls_if/calendar.csv
--rw-r--r--   0        0        0     2024 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/fno/controls_if/mapping.ttl
--rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/fno/controls_if/output.nq
--rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/fno/controls_if/test_controls_if.py
--rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/fno/controls_if_cast/calendar.csv
--rw-r--r--   0        0        0     2031 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/fno/controls_if_cast/mapping.ttl
--rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/fno/controls_if_cast/output.nq
--rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/fno/controls_if_cast/test_controls_if_cast.py
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/fno/date_to_date/calendar.csv
--rw-r--r--   0        0        0     1489 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/fno/date_to_date/mapping.ttl
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/fno/date_to_date/output.nq
--rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/fno/date_to_date/test_date_to_date.py
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/fno/math_round/distances.tsv
--rw-r--r--   0        0        0     1246 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/fno/math_round/mapping.ttl
--rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/fno/math_round/output.nq
--rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/fno/math_round/test_math_round.py
--rw-r--r--   0        0        0     1817 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/fno/nested_function/mapping.ttl
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/fno/nested_function/output.nq
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/fno/nested_function/student.csv
--rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/fno/nested_function/test_nested_function.py
--rw-r--r--   0        0        0     1312 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/fno/split_explode/mapping.ttl
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/fno/split_explode/mixed_content_list.csv
--rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/fno/split_explode/output.nq
--rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/fno/split_explode/test_split_explode.py
--rw-r--r--   0        0        0     1317 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/fno/split_explode_null/mapping.ttl
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/fno/split_explode_null/mixed_content_list.csv
--rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/fno/split_explode_null/output.nq
--rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/fno/split_explode_null/test_split_explode_null.py
--rw-r--r--   0        0        0     1183 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/fno/udf/mapping.ttl
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/fno/udf/output.nq
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/fno/udf/student.csv
--rw-r--r--   0        0        0      781 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/fno/udf/test_udf.py
--rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/fno/udf/udf.py
--rw-r--r--   0        0        0     1540 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/issues/issue_118/mapping.ttl
--rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/issues/issue_118/output.nq
--rw-r--r--   0        0        0     1500 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/issues/issue_118/premis.xml
--rw-r--r--   0        0        0      689 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/issues/issue_118/test_issue_118.py
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/issues/issue_124/data.csv
--rw-r--r--   0        0        0     1724 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/issues/issue_124/mapping.ttl
--rw-r--r--   0        0        0      838 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/issues/issue_124/output.nq
--rw-r--r--   0        0        0      758 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/issues/issue_124/test_issue_124.py
--rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/issues/issue_145/data.csv
--rw-r--r--   0        0        0     1630 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/issues/issue_145/mapping.ttl
--rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/issues/issue_145/output.nq
--rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/issues/issue_145/test_issue_145.py
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/issues/issue_62/data1.csv
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/issues/issue_62/data2.csv
--rw-r--r--   0        0        0     1043 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/issues/issue_62/mapping.ttl
--rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/issues/issue_62/output.nq
--rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/issues/issue_62/test_issue_62.py
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/issues/issue_67/data.csv
--rw-r--r--   0        0        0      978 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/issues/issue_67/mapping.ttl
--rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/issues/issue_67/output.nq
--rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/issues/issue_67/test_issue_67.py
--rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/issues/issue_80/mapping.rml
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/issues/issue_80/output.nq
--rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/issues/issue_80/student.csv
--rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/issues/issue_80/test_issue_80.py
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/issues/issue_81/country_info.csv
--rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/issues/issue_81/mapping.ttl
--rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/issues/issue_81/output.nq
--rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/issues/issue_81/test_issue_81.py
--rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0000/mapping.ttl
--rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0000/output.nq
--rw-r--r--   0        0        0     8192 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0000/resource.db
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0000/resource.sql
--rw-r--r--   0        0        0      829 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0000/test_R2RMLTC0000_SQLITE.py
--rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0001a/mapping.ttl
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0001a/output.nq
--rw-r--r--   0        0        0     8192 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0001a/resource.db
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0001a/resource.sql
--rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0001a/test_R2RMLTC0001a_SQLITE.py
--rw-r--r--   0        0        0      489 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0001b/mapping.ttl
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0001b/output.nq
--rw-r--r--   0        0        0     8192 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0001b/resource.db
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0001b/resource.sql
--rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0001b/test_R2RMLTC0001b_SQLITE.py
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0002a/mapping.ttl
--rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0002a/output.nq
--rw-r--r--   0        0        0     8192 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0002a/resource.db
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0002a/resource.sql
--rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0002a/test_R2RMLTC0002a_SQLITE.py
--rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0002b/mapping.ttl
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0002b/output.nq
--rw-r--r--   0        0        0     8192 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0002b/resource.db
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0002b/resource.sql
--rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0002b/test_R2RMLTC0002b_SQLITE.py
--rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0002c/mapping.ttl
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0002c/output.nq
--rw-r--r--   0        0        0     8192 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0002c/resource.db
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0002c/resource.sql
--rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0002c/test_R2RMLTC0002c_SQLITE.py
--rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0002d/mapping.ttl
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0002d/output.nq
--rw-r--r--   0        0        0     8192 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0002d/resource.db
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0002d/resource.sql
--rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0002d/test_R2RMLTC0002d_SQLITE.py
--rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0002e/mapping.ttl
--rw-r--r--   0        0        0     8192 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0002e/resource.db
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0002e/resource.sql
--rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0002e/test_R2RMLTC0002e_SQLITE.py
--rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0002f/mapping.ttl
--rw-r--r--   0        0        0     8192 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0002f/resource.db
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0002f/resource.sql
--rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0002f/test_R2RMLTC0002f_SQLITE.py
--rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0002g/mapping.ttl
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0002g/output.nq
--rw-r--r--   0        0        0     8192 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0002g/resource.db
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0002g/resource.sql
--rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0002g/test_R2RMLTC0002g_SQLITE.py
--rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0002h/mapping.ttl
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0002h/output.nq
--rw-r--r--   0        0        0     8192 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0002h/resource.db
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0002h/resource.sql
--rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0002h/test_R2RMLTC0002h_SQLITE.py
--rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0002i/mapping.ttl
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0002i/output.nq
--rw-r--r--   0        0        0     8192 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0002i/resource.db
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0002i/resource.sql
--rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0002i/test_R2RMLTC0002i_SQLITE.py
--rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0002j/mapping.ttl
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0002j/output.nq
--rw-r--r--   0        0        0     8192 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0002j/resource.db
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0002j/resource.sql
--rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0002j/test_R2RMLTC0002j_SQLITE.py
--rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0003a/R2RMLTC0003a_SQLITE.py
--rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0003a/mapping.ttl
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0003a/output.nq
--rw-r--r--   0        0        0     8192 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0003a/resource.db
--rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0003a/resource.sql
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0003b/mapping.ttl
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0003b/output.nq
--rw-r--r--   0        0        0     8192 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0003b/resource.db
--rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0003b/resource.sql
--rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0003b/test_R2RMLTC0003b_SQLITE.py
--rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0003c/mapping.ttl
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0003c/output.nq
--rw-r--r--   0        0        0     8192 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0003c/resource.db
--rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0003c/resource.sql
--rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0003c/test_R2RMLTC0003c_SQLITE.py
--rw-r--r--   0        0        0      839 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0004a/mapping.ttl
--rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0004a/output.nq
--rw-r--r--   0        0        0     8192 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0004a/resource.db
--rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0004a/resource.sql
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0004a/student_sport.csv
--rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0004a/test_R2RMLTC0004a_SQLITE.py
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0004b/mapping.ttl
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0004b/output.nq
--rw-r--r--   0        0        0     8192 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0004b/resource.db
--rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0004b/resource.sql
--rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0004b/test_R2RMLTC0004b_SQLITE.py
--rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0005a/mapping.ttl
--rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0005a/output.nq
--rw-r--r--   0        0        0     8192 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0005a/resource.db
--rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0005a/resource.sql
--rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0005a/test_R2RMLTC0005a_SQLITE.py
--rw-r--r--   0        0        0      817 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0005b/mapping.ttl
--rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0005b/output.nq
--rw-r--r--   0        0        0     8192 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0005b/resource.db
--rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0005b/resource.sql
--rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0005b/test_R2RMLTC0005b_SQLITE.py
--rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0006a/mapping.ttl
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0006a/output.nq
--rw-r--r--   0        0        0     8192 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0006a/resource.db
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0006a/resource.sql
--rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0006a/test_R2RMLTC0006a_SQLITE.py
--rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0007a/mapping.ttl
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0007a/output.nq
--rw-r--r--   0        0        0     8192 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0007a/resource.db
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0007a/resource.sql
--rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0007a/test_R2RMLTC0007a_SQLITE.py
--rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0007b/mapping.ttl
--rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0007b/output.nq
--rw-r--r--   0        0        0     8192 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0007b/resource.db
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0007b/resource.sql
--rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0007b/test_R2RMLTC0007b_SQLITE.py
--rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0007c/mapping.ttl
--rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0007c/output.nq
--rw-r--r--   0        0        0     8192 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0007c/resource.db
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0007c/resource.sql
--rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0007c/test_R2RMLTC0007c_SQLITE.py
--rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0007d/mapping.ttl
--rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0007d/output.nq
--rw-r--r--   0        0        0     8192 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0007d/resource.db
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0007d/resource.sql
--rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0007d/test_R2RMLTC0007d_SQLITE.py
--rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0007e/mapping.ttl
--rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0007e/output.nq
--rw-r--r--   0        0        0     8192 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0007e/resource.db
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0007e/resource.sql
--rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0007e/test_R2RMLTC0007e_SQLITE.py
--rw-r--r--   0        0        0      763 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0007f/mapping.ttl
--rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0007f/output.nq
--rw-r--r--   0        0        0     8192 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0007f/resource.db
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0007f/resource.sql
--rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0007f/test_R2RMLTC0007f_SQLITE.py
--rw-r--r--   0        0        0      676 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0007g/mapping.ttl
--rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0007g/output.nq
--rw-r--r--   0        0        0     8192 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0007g/resource.db
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0007g/resource.sql
--rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0007g/test_R2RMLTC0007g_SQLITE.py
--rw-r--r--   0        0        0      708 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0007h/mapping.ttl
--rw-r--r--   0        0        0     8192 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0007h/resource.db
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0007h/resource.sql
--rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0007h/test_R2RMLTC0007h_SQLITE.py
--rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0008a/mapping.ttl
--rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0008a/output.nq
--rw-r--r--   0        0        0     8192 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0008a/resource.db
--rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0008a/resource.sql
--rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0008a/test_R2RMLTC0008a_SQLITE.py
--rw-r--r--   0        0        0     1235 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0008b/mapping.ttl
--rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0008b/output.nq
--rw-r--r--   0        0        0     8192 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0008b/resource.db
--rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0008b/resource.sql
--rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0008b/test_R2RMLTC0008b_SQLITE.py
--rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0008c/mapping.ttl
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0008c/output.nq
--rw-r--r--   0        0        0     8192 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0008c/resource.db
--rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0008c/resource.sql
--rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0008c/test_R2RMLTC0008c_SQLITE.py
--rw-r--r--   0        0        0     1129 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0009a/mapping.ttl
--rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0009a/output.nq
--rw-r--r--   0        0        0    12288 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0009a/resource.db
--rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0009a/resource.sql
--rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0009a/test_R2RMLTC0009a_SQLITE.py
--rw-r--r--   0        0        0     1495 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0009b/mapping.ttl
--rw-r--r--   0        0        0     1198 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0009b/output.nq
--rw-r--r--   0        0        0    12288 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0009b/resource.db
--rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0009b/resource.sql
--rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0009b/test_R2RMLTC0009b_SQLITE.py
--rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0009c/mapping.ttl
--rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0009c/output.nq
--rw-r--r--   0        0        0    12288 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0009c/resource.db
--rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0009c/resource.sql
--rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0009c/test_R2RMLTC0009c_SQLITE.py
--rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0009d/mapping.ttl
--rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0009d/output.nq
--rw-r--r--   0        0        0    12288 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0009d/resource.db
--rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0009d/resource.sql
--rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0009d/test_R2RMLTC0009d_SQLITE.py
--rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0010a/mapping.ttl
--rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0010a/output.nq
--rw-r--r--   0        0        0     8192 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0010a/resource.db
--rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0010a/resource.sql
--rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0010a/test_R2RMLTC0010a_SQLITE.py
--rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0010b/mapping.ttl
--rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0010b/output.nq
--rw-r--r--   0        0        0     8192 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0010b/resource.db
--rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0010b/resource.sql
--rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0010b/test_R2RMLTC0010b_SQLITE.py
--rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0010c/mapping.ttl
--rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0010c/output.nq
--rw-r--r--   0        0        0     8192 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0010c/resource.db
--rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0010c/resource.sql
--rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0010c/test_R2RMLTC0010c_SQLITE.py
--rw-r--r--   0        0        0     1660 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0011a/mapping.ttl
--rw-r--r--   0        0        0     1525 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0011a/output.nq
--rw-r--r--   0        0        0    20480 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0011a/resource.db
--rw-r--r--   0        0        0     1143 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0011a/resource.sql
--rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0011a/test_R2RMLTC0011a_SQLITE.py
--rw-r--r--   0        0        0     1248 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0011b/mapping.ttl
--rw-r--r--   0        0        0     1228 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0011b/output.nq
--rw-r--r--   0        0        0    20480 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0011b/resource.db
--rw-r--r--   0        0        0     1143 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0011b/resource.sql
--rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0011b/test_R2RMLTC0011b_SQLITE.py
--rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0012a/mapping.ttl
--rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0012a/output.nq
--rw-r--r--   0        0        0    12288 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0012a/resource.db
--rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0012a/resource.sql
--rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0012a/test_R2RMLTC0012a_SQLITE.py
--rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0012b/mapping.ttl
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0012b/output.nq
--rw-r--r--   0        0        0    12288 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0012b/resource.db
--rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0012b/resource.sql
--rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0012b/test_R2RMLTC0012b_SQLITE.py
--rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0012c/mapping.ttl
--rw-r--r--   0        0        0    12288 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0012c/resource.db
--rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0012c/resource.sql
--rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0012c/test_R2RMLTC0012c_SQLITE.py
--rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0012d/mapping.ttl
--rw-r--r--   0        0        0    12288 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0012d/resource.db
--rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0012d/resource.sql
--rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0012d/test_R2RMLTC0012d_SQLITE.py
--rw-r--r--   0        0        0     1500 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0012e/mapping.ttl
--rw-r--r--   0        0        0     1252 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0012e/output.nq
--rw-r--r--   0        0        0    12288 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0012e/resource.db
--rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0012e/resource.sql
--rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0012e/test_R2RMLTC0012e_SQLITE.py
--rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0013a/mapping.ttl
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0013a/output.nq
--rw-r--r--   0        0        0     8192 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0013a/resource.db
--rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0013a/resource.sql
--rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0013a/test_R2RMLTC0013a_SQLITE.py
--rw-r--r--   0        0        0      843 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0014d/mapping.ttl
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0014d/output.nq
--rw-r--r--   0        0        0    20480 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0014d/resource.db
--rw-r--r--   0        0        0      775 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0014d/resource.sql
--rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0014d/test_R2RMLTC0014d_SQLITE.py
--rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0015a/mapping.ttl
--rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0015a/output.nq
--rw-r--r--   0        0        0    12288 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0015a/resource.db
--rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0015a/resource.sql
--rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0015a/test_R2RMLTC0015a_SQLITE.py
--rw-r--r--   0        0        0     1122 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0015b/mapping.ttl
--rw-r--r--   0        0        0    12288 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0015b/resource.db
--rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0015b/resource.sql
--rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0015b/test_R2RMLTC0015b_SQLITE.py
--rw-r--r--   0        0        0      974 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0016a/mapping.ttl
--rw-r--r--   0        0        0     1197 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0016a/output.nq
--rw-r--r--   0        0        0     8192 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0016a/resource.db
--rw-r--r--   0        0        0     1435 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0016a/resource.sql
--rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0016a/test_R2RMLTC0016a_SQLITE.py
--rw-r--r--   0        0        0      910 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0016b/R2RMLTC0016b_SQLITE.py
--rw-r--r--   0        0        0      751 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0016b/mapping.ttl
--rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0016b/output.nq
--rw-r--r--   0        0        0     8192 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0016b/resource.db
--rw-r--r--   0        0        0     1435 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0016b/resource.sql
--rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0016c/R2RMLTC0016c_SQLITE.py
--rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0016c/mapping.ttl
--rw-r--r--   0        0        0     1110 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0016c/output.nq
--rw-r--r--   0        0        0     8192 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0016c/resource.db
--rw-r--r--   0        0        0     1435 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0016c/resource.sql
--rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0016d/R2RMLTC0016d_SQLITE.py
--rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0016d/mapping.ttl
--rw-r--r--   0        0        0      685 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0016d/output.nq
--rw-r--r--   0        0        0     8192 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0016d/resource.db
--rw-r--r--   0        0        0     1435 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0016d/resource.sql
--rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0016e/R2RMLTC0016e_SQLITE.py
--rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0016e/mapping.ttl
--rw-r--r--   0        0        0     1110 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0016e/output.nq
--rw-r--r--   0        0        0     8192 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0016e/resource.db
--rw-r--r--   0        0        0     1435 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0016e/resource.sql
--rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0018a/mapping.ttl
--rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0018a/output.nq
--rw-r--r--   0        0        0     8192 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0018a/resource.db
--rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0018a/resource.sql
--rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0018a/test_R2RMLTC0018a_SQLITE.py
--rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0019a/R2RMLTC0019a_SQLITE.py
--rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0019a/mapping.ttl
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0019a/output.nq
--rw-r--r--   0        0        0     8192 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0019a/resource.db
--rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0019a/resource.sql
--rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0019b/R2RMLTC0019b_SQLITE.py
--rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0019b/mapping.ttl
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0019b/output.nq
--rw-r--r--   0        0        0     8192 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0019b/resource.db
--rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0019b/resource.sql
--rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0020a/R2RMLTC0020a_SQLITE.py
--rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0020a/mapping.ttl
--rw-r--r--   0        0        0      658 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0020a/output.nq
--rw-r--r--   0        0        0     8192 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0020a/resource.db
--rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0020a/resource.sql
--rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0020b/R2RMLTC0020b_SQLITE.py
--rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0020b/mapping.ttl
--rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0020b/output.nq
--rw-r--r--   0        0        0     8192 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0020b/resource.db
--rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/r2rml/R2RMLTC0020b/resource.sql
--rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/csv/RMLTC0000/mapping.ttl
--rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/csv/RMLTC0000/output.nq
--rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/csv/RMLTC0000/student.csv
--rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/csv/RMLTC0000/test_RMLTC0000_CSV.py
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/csv/RMLTC0001a/mapping.ttl
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/csv/RMLTC0001a/output.nq
--rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/csv/RMLTC0001a/student.csv
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/csv/RMLTC0001a/test_RMLTC0001a_CSV.py
--rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/csv/RMLTC0001b/mapping.ttl
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/csv/RMLTC0001b/output.nq
--rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/csv/RMLTC0001b/student.csv
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/csv/RMLTC0001b/test_RMLTC0001b_CSV.py
--rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/csv/RMLTC0002a/mapping.ttl
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/csv/RMLTC0002a/output.nq
--rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/csv/RMLTC0002a/student.csv
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/csv/RMLTC0002a/test_RMLTC0002a_CSV.py
--rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/csv/RMLTC0002b/mapping.ttl
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/csv/RMLTC0002b/output.nq
--rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/csv/RMLTC0002b/student.csv
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/csv/RMLTC0002b/test_RMLTC0002b_CSV.py
--rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/csv/RMLTC0002c/mapping.ttl
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/csv/RMLTC0002c/output.nq
--rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/csv/RMLTC0002c/student.csv
--rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/csv/RMLTC0002c/test_RMLTC0002c_CSV.py
--rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/csv/RMLTC0002e/mapping.ttl
--rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/csv/RMLTC0002e/student.csv
--rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/csv/RMLTC0002e/test_RMLTC0002e_CSV.py
--rw-r--r--   0        0        0      689 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/csv/RMLTC0003c/mapping.ttl
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/csv/RMLTC0003c/output.nq
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/csv/RMLTC0003c/student.csv
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/csv/RMLTC0003c/test_RMLTC0003c_CSV.py
--rw-r--r--   0        0        0     1035 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/csv/RMLTC0004a/mapping.ttl
--rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/csv/RMLTC0004a/output.nq
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/csv/RMLTC0004a/student_sport.csv
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/csv/RMLTC0004a/test_RMLTC0004a_CSV.py
--rw-r--r--   0        0        0      666 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/csv/RMLTC0004b/mapping.ttl
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/csv/RMLTC0004b/output.nq
--rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/csv/RMLTC0004b/student.csv
--rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/csv/RMLTC0004b/test_RMLTC0004b_CSV.py
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/csv/RMLTC0005a/ious.csv
--rw-r--r--   0        0        0      659 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/csv/RMLTC0005a/mapping.ttl
--rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/csv/RMLTC0005a/output.nq
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/csv/RMLTC0005a/test_RMLTC0005a_CSV.py
--rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/csv/RMLTC0006a/mapping.ttl
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/csv/RMLTC0006a/output.nq
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/csv/RMLTC0006a/student.csv
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/csv/RMLTC0006a/test_RMLTC0006a_CSV.py
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/csv/RMLTC0007a/mapping.ttl
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/csv/RMLTC0007a/output.nq
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/csv/RMLTC0007a/student.csv
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/csv/RMLTC0007a/test_RMLTC0007a_CSV.py
--rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/csv/RMLTC0007b/mapping.ttl
--rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/csv/RMLTC0007b/output.nq
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/csv/RMLTC0007b/student.csv
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/csv/RMLTC0007b/test_RMLTC0007b_CSV.py
--rw-r--r--   0        0        0      785 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/csv/RMLTC0007c/mapping.ttl
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/csv/RMLTC0007c/output.nq
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/csv/RMLTC0007c/student.csv
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/csv/RMLTC0007c/test_RMLTC0007c_CSV.py
--rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/csv/RMLTC0007d/mapping.ttl
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/csv/RMLTC0007d/output.nq
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/csv/RMLTC0007d/student.csv
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/csv/RMLTC0007d/test_RMLTC0007d_CSV.py
--rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/csv/RMLTC0007e/mapping.ttl
--rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/csv/RMLTC0007e/output.nq
--rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/csv/RMLTC0007e/student.csv
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/csv/RMLTC0007e/test_RMLTC0007e_CSV.py
--rw-r--r--   0        0        0      923 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/csv/RMLTC0007f/mapping.ttl
--rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/csv/RMLTC0007f/output.nq
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/csv/RMLTC0007f/student.csv
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/csv/RMLTC0007f/test_RMLTC0007f_CSV.py
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/csv/RMLTC0007g/mapping.ttl
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/csv/RMLTC0007g/output.nq
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/csv/RMLTC0007g/student.csv
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/csv/RMLTC0007g/test_RMLTC0007g_CSV.py
--rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/csv/RMLTC0007h/mapping.ttl
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/csv/RMLTC0007h/student.csv
--rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/csv/RMLTC0007h/test_RMLTC0007h_CSV.py
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/csv/RMLTC0008a/mapping.ttl
--rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/csv/RMLTC0008a/output.nq
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/csv/RMLTC0008a/student.csv
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/csv/RMLTC0008a/test_RMLTC0008a_CSV.py
--rw-r--r--   0        0        0     1410 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/csv/RMLTC0008b/mapping.ttl
--rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/csv/RMLTC0008b/output.nq
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/csv/RMLTC0008b/student.csv
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/csv/RMLTC0008b/test_RMLTC0008b_CSV.py
--rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/csv/RMLTC0008c/mapping.ttl
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/csv/RMLTC0008c/output.nq
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/csv/RMLTC0008c/student.csv
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/csv/RMLTC0008c/test_RMLTC0008c_CSV.py
--rw-r--r--   0        0        0     1344 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/csv/RMLTC0009a/mapping.ttl
--rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/csv/RMLTC0009a/output.nq
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/csv/RMLTC0009a/sport.csv
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/csv/RMLTC0009a/student.csv
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/csv/RMLTC0009a/test_RMLTC0009a_CSV.py
--rw-r--r--   0        0        0     1665 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/csv/RMLTC0009b/mapping.ttl
--rw-r--r--   0        0        0     1198 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/csv/RMLTC0009b/output.nq
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/csv/RMLTC0009b/sport.csv
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/csv/RMLTC0009b/student.csv
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/csv/RMLTC0009b/test_RMLTC0009b_CSV.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/csv/RMLTC0010a/country_info.csv
--rw-r--r--   0        0        0      685 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/csv/RMLTC0010a/mapping.ttl
--rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/csv/RMLTC0010a/output.nq
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/csv/RMLTC0010a/test_RMLTC0010a_CSV.py
--rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/csv/RMLTC0010b/country_info.csv
--rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/csv/RMLTC0010b/mapping.ttl
--rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/csv/RMLTC0010b/output.nq
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/csv/RMLTC0010b/test_RMLTC0010b_CSV.py
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/csv/RMLTC0010c/country_info.csv
--rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/csv/RMLTC0010c/mapping.ttl
--rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/csv/RMLTC0010c/output.nq
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/csv/RMLTC0010c/test_RMLTC0010c_CSV.py
--rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/csv/RMLTC0011b/mapping.ttl
--rw-r--r--   0        0        0     1229 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/csv/RMLTC0011b/output.nq
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/csv/RMLTC0011b/sport.csv
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/csv/RMLTC0011b/student.csv
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/csv/RMLTC0011b/student_sport.csv
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/csv/RMLTC0011b/test_RMLTC0011b_CSV.py
--rw-r--r--   0        0        0      817 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/csv/RMLTC0012a/mapping.ttl
--rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/csv/RMLTC0012a/output.nq
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/csv/RMLTC0012a/persons.csv
--rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/csv/RMLTC0012a/test_RMLTC0012a_CSV.py
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/csv/RMLTC0012b/lives.csv
--rw-r--r--   0        0        0     1058 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/csv/RMLTC0012b/mapping.ttl
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/csv/RMLTC0012b/output.nq
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/csv/RMLTC0012b/persons.csv
--rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/csv/RMLTC0012b/test_RMLTC0012b_CSV.py
--rw-r--r--   0        0        0      731 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/csv/RMLTC0012c/mapping.ttl
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/csv/RMLTC0012c/persons.csv
--rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/csv/RMLTC0012c/test_RMLTC0012c_CSV.py
--rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/csv/RMLTC0012d/mapping.ttl
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/csv/RMLTC0012d/persons.csv
--rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/csv/RMLTC0012d/test_RMLTC0012d_CSV.py
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/csv/RMLTC0015a/country_en.csv
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/csv/RMLTC0015a/country_es.csv
--rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/csv/RMLTC0015a/mapping.ttl
--rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/csv/RMLTC0015a/output.nq
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/csv/RMLTC0015a/test_RMLTC0015a_CSV.py
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/csv/RMLTC0015b/country_en.csv
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/csv/RMLTC0015b/country_es.csv
--rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/csv/RMLTC0015b/mapping.ttl
--rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/csv/RMLTC0015b/test_RMLTC0015b_CSV.py
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/csv/RMLTC0019a/RMLTC0019a_CSV.py
--rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/csv/RMLTC0019a/mapping.ttl
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/csv/RMLTC0019a/output.nq
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/csv/RMLTC0019a/persons.csv
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/csv/RMLTC0019b/RMLTC0019b_CSV.py
--rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/csv/RMLTC0019b/mapping.ttl
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/csv/RMLTC0019b/output.nq
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/csv/RMLTC0019b/persons.csv
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/csv/RMLTC0020a/RMLTC0020a_CSV.py
--rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/csv/RMLTC0020a/mapping.ttl
--rw-r--r--   0        0        0      658 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/csv/RMLTC0020a/output.nq
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/csv/RMLTC0020a/student.csv
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/csv/RMLTC0020b/RMLTC0020b_CSV.py
--rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/csv/RMLTC0020b/mapping.ttl
--rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/csv/RMLTC0020b/output.nq
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/csv/RMLTC0020b/student.csv
--rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/csv/null_filter/mapping.ttl
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/csv/null_filter/output.nq
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/csv/null_filter/student.csv
--rw-r--r--   0        0        0      689 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/csv/null_filter/test_null_filter_CSV.py
--rw-r--r--   0        0        0     1161 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/csv/triples_map_without_pom/mapping.ttl
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/csv/triples_map_without_pom/output.nq
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/csv/triples_map_without_pom/sport.csv
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/csv/triples_map_without_pom/student.csv
--rw-r--r--   0        0        0      701 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/csv/triples_map_without_pom/test_triples_map_without_pom_CSV.py
--rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/json/RMLTC0000/mapping.ttl
--rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/json/RMLTC0000/output.nq
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/json/RMLTC0000/student.json
--rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/json/RMLTC0000/test_RMLTC0000_JSON.py
--rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/json/RMLTC0001a/mapping.ttl
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/json/RMLTC0001a/output.nq
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/json/RMLTC0001a/student.json
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/json/RMLTC0001a/test_RMLTC0001a_JSON.py
--rw-r--r--   0        0        0      689 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/json/RMLTC0001b/mapping.ttl
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/json/RMLTC0001b/output.nq
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/json/RMLTC0001b/student.json
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/json/RMLTC0001b/test_RMLTC0001b_JSON.py
--rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/json/RMLTC0002a/mapping.ttl
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/json/RMLTC0002a/output.nq
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/json/RMLTC0002a/student.json
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/json/RMLTC0002a/test_RMLTC0002a_JSON.py
--rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/json/RMLTC0002b/mapping.ttl
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/json/RMLTC0002b/output.nq
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/json/RMLTC0002b/student.json
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/json/RMLTC0002b/test_RMLTC0002b_JSON.py
--rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/json/RMLTC0002c/mapping.ttl
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/json/RMLTC0002c/output.nq
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/json/RMLTC0002c/student.json
--rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/json/RMLTC0002c/test_RMLTC0002c_JSON.py
--rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/json/RMLTC0002e/mapping.ttl
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/json/RMLTC0002e/student.json
--rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/json/RMLTC0002e/test_RMLTC0002e_JSON.py
--rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/json/RMLTC0003c/mapping.ttl
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/json/RMLTC0003c/output.nq
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/json/RMLTC0003c/student.json
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/json/RMLTC0003c/test_RMLTC0003c_JSON.py
--rw-r--r--   0        0        0     1117 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/json/RMLTC0004a/mapping.ttl
--rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/json/RMLTC0004a/output.nq
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/json/RMLTC0004a/student_sport.json
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/json/RMLTC0004a/test_RMLTC0004a_JSON.py
--rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/json/RMLTC0004b/mapping.ttl
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/json/RMLTC0004b/output.nq
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/json/RMLTC0004b/student.json
--rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/json/RMLTC0004b/test_RMLTC0004b_JSON.py
--rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/json/RMLTC0005a/ious.json
--rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/json/RMLTC0005a/mapping.ttl
--rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/json/RMLTC0005a/output.nq
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/json/RMLTC0005a/test_RMLTC0005a_JSON.py
--rw-r--r--   0        0        0      751 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/json/RMLTC0006a/mapping.ttl
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/json/RMLTC0006a/output.nq
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/json/RMLTC0006a/student.json
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/json/RMLTC0006a/test_RMLTC0006a_JSON.py
--rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/json/RMLTC0007a/mapping.ttl
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/json/RMLTC0007a/output.nq
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/json/RMLTC0007a/student.json
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/json/RMLTC0007a/test_RMLTC0007a_JSON.py
--rw-r--r--   0        0        0      865 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/json/RMLTC0007b/mapping.ttl
--rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/json/RMLTC0007b/output.nq
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/json/RMLTC0007b/student.json
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/json/RMLTC0007b/test_RMLTC0007b_JSON.py
--rw-r--r--   0        0        0      826 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/json/RMLTC0007c/mapping.ttl
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/json/RMLTC0007c/output.nq
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/json/RMLTC0007c/student.json
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/json/RMLTC0007c/test_RMLTC0007c_JSON.py
--rw-r--r--   0        0        0     1015 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/json/RMLTC0007d/mapping.ttl
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/json/RMLTC0007d/output.nq
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/json/RMLTC0007d/student.json
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/json/RMLTC0007d/test_RMLTC0007d_JSON.py
--rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/json/RMLTC0007e/mapping.ttl
--rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/json/RMLTC0007e/output.nq
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/json/RMLTC0007e/student.json
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/json/RMLTC0007e/test_RMLTC0007e_JSON.py
--rw-r--r--   0        0        0      964 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/json/RMLTC0007f/mapping.ttl
--rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/json/RMLTC0007f/output.nq
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/json/RMLTC0007f/student.json
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/json/RMLTC0007f/test_RMLTC0007f_JSON.py
--rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/json/RMLTC0007g/mapping.ttl
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/json/RMLTC0007g/output.nq
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/json/RMLTC0007g/student.json
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/json/RMLTC0007g/test_RMLTC0007g_JSON.py
--rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/json/RMLTC0007h/mapping.ttl
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/json/RMLTC0007h/student.json
--rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/json/RMLTC0007h/test_RMLTC0007h_JSON.py
--rw-r--r--   0        0        0     1111 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/json/RMLTC0008a/mapping.ttl
--rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/json/RMLTC0008a/output.nq
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/json/RMLTC0008a/student.json
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/json/RMLTC0008a/test_RMLTC0008a_JSON.py
--rw-r--r--   0        0        0     1492 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/json/RMLTC0008b/mapping.ttl
--rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/json/RMLTC0008b/output.nq
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/json/RMLTC0008b/student.json
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/json/RMLTC0008b/test_RMLTC0008b_JSON.py
--rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/json/RMLTC0008c/mapping.ttl
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/json/RMLTC0008c/output.nq
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/json/RMLTC0008c/student.json
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/json/RMLTC0008c/test_RMLTC0008c_JSON.py
--rw-r--r--   0        0        0     1424 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/json/RMLTC0009a/mapping.ttl
--rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/json/RMLTC0009a/output.nq
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/json/RMLTC0009a/sport.json
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/json/RMLTC0009a/student.json
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/json/RMLTC0009a/test_RMLTC0009a_JSON.py
--rw-r--r--   0        0        0     1735 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/json/RMLTC0009b/mapping.ttl
--rw-r--r--   0        0        0     1198 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/json/RMLTC0009b/output.nq
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/json/RMLTC0009b/sport.json
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/json/RMLTC0009b/student.json
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/json/RMLTC0009b/test_RMLTC0009b_JSON.py
--rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/json/RMLTC0010a/country_info.json
--rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/json/RMLTC0010a/mapping.ttl
--rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/json/RMLTC0010a/output.nq
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/json/RMLTC0010a/test_RMLTC0010a_JSON.py
--rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/json/RMLTC0010b/country_info.json
--rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/json/RMLTC0010b/mapping.ttl
--rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/json/RMLTC0010b/output.nq
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/json/RMLTC0010b/test_RMLTC0010b_JSON.py
--rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/json/RMLTC0010c/country_info.json
--rw-r--r--   0        0        0      781 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/json/RMLTC0010c/mapping.ttl
--rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/json/RMLTC0010c/output.nq
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/json/RMLTC0010c/test_RMLTC0010c_JSON.py
--rw-r--r--   0        0        0     1723 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/json/RMLTC0011b/mapping.ttl
--rw-r--r--   0        0        0     1229 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/json/RMLTC0011b/output.nq
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/json/RMLTC0011b/sport.json
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/json/RMLTC0011b/student.json
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/json/RMLTC0011b/student_sport.json
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/json/RMLTC0011b/test_RMLTC0011b_JSON.py
--rw-r--r--   0        0        0      857 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/json/RMLTC0012a/mapping.ttl
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/json/RMLTC0012a/output.nq
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/json/RMLTC0012a/persons.json
--rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/json/RMLTC0012a/test_RMLTC0012a_JSON.py
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/json/RMLTC0012b/lives.json
--rw-r--r--   0        0        0     1136 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/json/RMLTC0012b/mapping.ttl
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/json/RMLTC0012b/output.nq
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/json/RMLTC0012b/persons.json
--rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/json/RMLTC0012b/test_RMLTC0012b_JSON.py
--rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/json/RMLTC0012c/mapping.ttl
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/json/RMLTC0012c/persons.json
--rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/json/RMLTC0012c/test_RMLTC0012c_JSON.py
--rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/json/RMLTC0012d/mapping.ttl
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/json/RMLTC0012d/persons.json
--rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/json/RMLTC0012d/test_RMLTC0012d_JSON.py
--rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/json/RMLTC0013a/mapping.ttl
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/json/RMLTC0013a/output.nq
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/json/RMLTC0013a/persons.json
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/json/RMLTC0013a/test_RMLTC0013a_JSON.py
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/json/RMLTC0015a/country_en.json
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/json/RMLTC0015a/country_es.json
--rw-r--r--   0        0        0     1167 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/json/RMLTC0015a/mapping.ttl
--rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/json/RMLTC0015a/output.nq
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/json/RMLTC0015a/test_RMLTC0015a_JSON.py
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/json/RMLTC0015b/country_en.json
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/json/RMLTC0015b/country_es.json
--rw-r--r--   0        0        0     1165 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/json/RMLTC0015b/mapping.ttl
--rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/json/RMLTC0015b/test_RMLTC0015b_JSON.py
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/json/RMLTC0019a/RMLTC0019a_JSON.py
--rw-r--r--   0        0        0      720 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/json/RMLTC0019a/mapping.ttl
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/json/RMLTC0019a/output.nq
--rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/json/RMLTC0019a/persons.json
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/json/RMLTC0019b/RMLTC0019b_JSON.py
--rw-r--r--   0        0        0      720 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/json/RMLTC0019b/mapping.ttl
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/json/RMLTC0019b/output.nq
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/json/RMLTC0019b/persons.json
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/json/RMLTC0020a/RMLTC0020a_JSON.py
--rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/json/RMLTC0020a/mapping.ttl
--rw-r--r--   0        0        0      658 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/json/RMLTC0020a/output.nq
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/json/RMLTC0020a/student.json
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/json/RMLTC0020b/RMLTC0020b_JSON.py
--rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/json/RMLTC0020b/mapping.ttl
--rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/json/RMLTC0020b/output.nq
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/json/RMLTC0020b/student.json
--rw-r--r--   0        0        0     3464 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/json/complex/data.json
--rw-r--r--   0        0        0     9797 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/json/complex/mapping.ttl
--rw-r--r--   0        0        0     1791 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/json/complex/mapping.yaml
--rw-r--r--   0        0        0     3729 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/json/complex/output.nq
--rw-r--r--   0        0        0     2021 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/json/complex/test_complex_JSON.py
--rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/tabular/RMLTC0002a_EXCEL/mapping.ttl
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/tabular/RMLTC0002a_EXCEL/output.nq
--rw-r--r--   0        0        0     4925 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/tabular/RMLTC0002a_EXCEL/student.xlsx
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/tabular/RMLTC0002a_EXCEL/test_RMLTC0002a_EXCEL.py
--rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/tabular/RMLTC0002a_FEATHER/mapping.ttl
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/tabular/RMLTC0002a_FEATHER/output.nq
--rw-r--r--   0        0        0     1538 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/tabular/RMLTC0002a_FEATHER/student.feather
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/tabular/RMLTC0002a_FEATHER/test_RMLTC0002a_FEATHER.py
--rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/tabular/RMLTC0002a_ODS/mapping.ttl
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/tabular/RMLTC0002a_ODS/output.nq
--rw-r--r--   0        0        0     5269 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/tabular/RMLTC0002a_ODS/student.ods
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/tabular/RMLTC0002a_ODS/test_RMLTC0002a_ODS.py
--rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/tabular/RMLTC0002a_PARQUET/mapping.ttl
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/tabular/RMLTC0002a_PARQUET/output.nq
--rw-r--r--   0        0        0     1746 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/tabular/RMLTC0002a_PARQUET/student.parquet
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/tabular/RMLTC0002a_PARQUET/test_RMLTC0002a_PARQUET.py
--rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/tabular/RMLTC0002a_STATA/mapping.ttl
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/tabular/RMLTC0002a_STATA/output.nq
--rw-r--r--   0        0        0     1844 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/tabular/RMLTC0002a_STATA/student.dta
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/tabular/RMLTC0002a_STATA/test_RMLTC0002a_STATA.py
--rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/tabular/RMLTC0002a_TSV/mapping.ttl
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/tabular/RMLTC0002a_TSV/output.nq
--rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/tabular/RMLTC0002a_TSV/student.tsv
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/tabular/RMLTC0002a_TSV/test_RMLTC0002a_TSV.py
--rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/xml/RMLTC0000/mapping.ttl
--rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/xml/RMLTC0000/output.nq
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/xml/RMLTC0000/student.xml
--rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/xml/RMLTC0000/test_RMLTC0000_XML.py
--rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/xml/RMLTC0001a/mapping.ttl
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/xml/RMLTC0001a/output.nq
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/xml/RMLTC0001a/student.xml
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/xml/RMLTC0001a/test_RMLTC0001a_XML.py
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/xml/RMLTC0001b/mapping.ttl
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/xml/RMLTC0001b/output.nq
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/xml/RMLTC0001b/student.xml
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/xml/RMLTC0001b/test_RMLTC0001b_XML.py
--rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/xml/RMLTC0002a/mapping.ttl
--rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/xml/RMLTC0002a/output.nq
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/xml/RMLTC0002a/student.xml
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/xml/RMLTC0002a/test_RMLTC0002a_XML.py
--rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/xml/RMLTC0002b/mapping.ttl
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/xml/RMLTC0002b/output.nq
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/xml/RMLTC0002b/student.xml
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/xml/RMLTC0002b/test_RMLTC0002b_XML.py
--rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/xml/RMLTC0002c/mapping.ttl
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/xml/RMLTC0002c/output.nq
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/xml/RMLTC0002c/student.xml
--rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/xml/RMLTC0002c/test_RMLTC0002c_XML.py
--rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/xml/RMLTC0002e/mapping.ttl
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/xml/RMLTC0002e/student.xml
--rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/xml/RMLTC0002e/test_RMLTC0002e_XML.py
--rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/xml/RMLTC0003c/mapping.ttl
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/xml/RMLTC0003c/output.nq
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/xml/RMLTC0003c/student.xml
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/xml/RMLTC0003c/test_RMLTC0003c_XML.py
--rw-r--r--   0        0        0     1115 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/xml/RMLTC0004a/mapping.ttl
--rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/xml/RMLTC0004a/output.nq
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/xml/RMLTC0004a/student_sport.xml
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/xml/RMLTC0004a/test_RMLTC0004a_XML.py
--rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/xml/RMLTC0004b/mapping.ttl
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/xml/RMLTC0004b/output.nq
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/xml/RMLTC0004b/student.xml
--rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/xml/RMLTC0004b/test_RMLTC0004b_XML.py
--rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/xml/RMLTC0005a/ious.xml
--rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/xml/RMLTC0005a/mapping.ttl
--rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/xml/RMLTC0005a/output.nq
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/xml/RMLTC0005a/test_RMLTC0005a_XML.py
--rw-r--r--   0        0        0      750 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/xml/RMLTC0006a/mapping.ttl
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/xml/RMLTC0006a/output.nq
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/xml/RMLTC0006a/student.xml
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/xml/RMLTC0006a/test_RMLTC0006a_XML.py
--rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/xml/RMLTC0007a/mapping.ttl
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/xml/RMLTC0007a/output.nq
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/xml/RMLTC0007a/student.xml
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/xml/RMLTC0007a/test_RMLTC0007a_XML.py
--rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/xml/RMLTC0007b/mapping.ttl
--rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/xml/RMLTC0007b/output.nq
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/xml/RMLTC0007b/student.xml
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/xml/RMLTC0007b/test_RMLTC0007b_XML.py
--rw-r--r--   0        0        0      825 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/xml/RMLTC0007c/mapping.ttl
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/xml/RMLTC0007c/output.nq
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/xml/RMLTC0007c/student.xml
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/xml/RMLTC0007c/test_RMLTC0007c_XML.py
--rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/xml/RMLTC0007d/mapping.ttl
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/xml/RMLTC0007d/output.nq
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/xml/RMLTC0007d/student.xml
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/xml/RMLTC0007d/test_RMLTC0007d_XML.py
--rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/xml/RMLTC0007e/mapping.ttl
--rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/xml/RMLTC0007e/output.nq
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/xml/RMLTC0007e/student.xml
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/xml/RMLTC0007e/test_RMLTC0007e_XML.py
--rw-r--r--   0        0        0      963 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/xml/RMLTC0007f/mapping.ttl
--rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/xml/RMLTC0007f/output.nq
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/xml/RMLTC0007f/student.xml
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/xml/RMLTC0007f/test_RMLTC0007f_XML.py
--rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/xml/RMLTC0007g/mapping.ttl
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/xml/RMLTC0007g/output.nq
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/xml/RMLTC0007g/student.xml
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/xml/RMLTC0007g/test_RMLTC0007g_XML.py
--rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/xml/RMLTC0007h/mapping.ttl
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/xml/RMLTC0007h/student.xml
--rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/xml/RMLTC0007h/test_RMLTC0007h_XML.py
--rw-r--r--   0        0        0     1110 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/xml/RMLTC0008a/mapping.ttl
--rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/xml/RMLTC0008a/output.nq
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/xml/RMLTC0008a/student.xml
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/xml/RMLTC0008a/test_RMLTC0008a_XML.py
--rw-r--r--   0        0        0     1490 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/xml/RMLTC0008b/mapping.ttl
--rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/xml/RMLTC0008b/output.nq
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/xml/RMLTC0008b/student.xml
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/xml/RMLTC0008b/test_RMLTC0008b_XML.py
--rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/xml/RMLTC0008c/mapping.ttl
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/xml/RMLTC0008c/output.nq
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/xml/RMLTC0008c/student.xml
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/xml/RMLTC0008c/test_RMLTC0008c_XML.py
--rw-r--r--   0        0        0     1420 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/xml/RMLTC0009a/mapping.ttl
--rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/xml/RMLTC0009a/output.nq
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/xml/RMLTC0009a/sport.xml
--rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/xml/RMLTC0009a/student.xml
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/xml/RMLTC0009a/test_RMLTC0009a_XML.py
--rw-r--r--   0        0        0     1740 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/xml/RMLTC0009b/mapping.ttl
--rw-r--r--   0        0        0     1198 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/xml/RMLTC0009b/output.nq
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/xml/RMLTC0009b/sport.xml
--rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/xml/RMLTC0009b/student.xml
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/xml/RMLTC0009b/test_RMLTC0009b_XML.py
--rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/xml/RMLTC0010b/country_info.xml
--rw-r--r--   0        0        0      732 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/xml/RMLTC0010b/mapping.ttl
--rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/xml/RMLTC0010b/output.nq
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/xml/RMLTC0010b/test_RMLTC0010b_XML.py
--rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/xml/RMLTC0010c/country_info.xml
--rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/xml/RMLTC0010c/mapping.ttl
--rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/xml/RMLTC0010c/output.nq
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/xml/RMLTC0010c/test_RMLTC0010c_XML.py
--rw-r--r--   0        0        0     1715 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/xml/RMLTC0011b/mapping.ttl
--rw-r--r--   0        0        0     1229 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/xml/RMLTC0011b/output.nq
--rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/xml/RMLTC0011b/sport.xml
--rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/xml/RMLTC0011b/student.xml
--rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/xml/RMLTC0011b/student_sport.xml
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/xml/RMLTC0011b/test_RMLTC0011b_XML.py
--rw-r--r--   0        0        0      855 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/xml/RMLTC0012a/mapping.ttl
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/xml/RMLTC0012a/output.nq
--rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/xml/RMLTC0012a/persons.xml
--rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/xml/RMLTC0012a/test_RMLTC0012a_XML.py
--rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/xml/RMLTC0012b/lives.xml
--rw-r--r--   0        0        0     1132 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/xml/RMLTC0012b/mapping.ttl
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/xml/RMLTC0012b/output.nq
--rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/xml/RMLTC0012b/persons.xml
--rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/xml/RMLTC0012b/test_RMLTC0012b_XML.py
--rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/xml/RMLTC0012c/mapping.ttl
--rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/xml/RMLTC0012c/persons.xml
--rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/xml/RMLTC0012c/test_RMLTC0012c_XML.py
--rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/xml/RMLTC0012d/mapping.ttl
--rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/xml/RMLTC0012d/persons.xml
--rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/xml/RMLTC0012d/test_RMLTC0012d_XML.py
--rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/xml/RMLTC0015a/country_en.xml
--rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/xml/RMLTC0015a/country_es.xml
--rw-r--r--   0        0        0     1165 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/xml/RMLTC0015a/mapping.ttl
--rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/xml/RMLTC0015a/output.nq
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/xml/RMLTC0015a/test_RMLTC0015a_XML.py
--rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/xml/RMLTC0015b/country_en.xml
--rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/xml/RMLTC0015b/country_es.xml
--rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/xml/RMLTC0015b/mapping.ttl
--rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/xml/RMLTC0015b/test_RMLTC0015b_XML.py
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/xml/RMLTC0019a/RMLTC0019a_XML.py
--rw-r--r--   0        0        0      718 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/xml/RMLTC0019a/mapping.ttl
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/xml/RMLTC0019a/output.nq
--rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/xml/RMLTC0019a/persons.xml
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/xml/RMLTC0019b/RMLTC0019b_XML.py
--rw-r--r--   0        0        0      718 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/xml/RMLTC0019b/mapping.ttl
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/xml/RMLTC0019b/output.nq
--rw-r--r--   0        0        0      432 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/xml/RMLTC0019b/persons.xml
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/xml/RMLTC0020a/RMLTC0020a_XML.py
--rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/xml/RMLTC0020a/mapping.ttl
--rw-r--r--   0        0        0      658 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/xml/RMLTC0020a/output.nq
--rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/xml/RMLTC0020a/student.xml
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/xml/RMLTC0020b/RMLTC0020b_XML.py
--rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/xml/RMLTC0020b/mapping.ttl
--rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/xml/RMLTC0020b/output.nq
--rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/xml/RMLTC0020b/student.xml
--rw-r--r--   0        0        0      859 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/xml/attributes/data.xml
--rw-r--r--   0        0        0     1516 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/xml/attributes/mapping.ttl
--rw-r--r--   0        0        0     1532 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/xml/attributes/output.nq
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/xml/attributes/test_attributes_XML.py
--rw-r--r--   0        0        0     3656 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/xml/complex/data.xml
--rw-r--r--   0        0        0     9759 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/xml/complex/mapping.ttl
--rw-r--r--   0        0        0     1756 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/xml/complex/mapping.yaml
--rw-r--r--   0        0        0     4539 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/xml/complex/output.nq
--rw-r--r--   0        0        0     2020 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/xml/complex/test_complex_XML.py
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/xml/rml_spec_example_section_3/Transport.xml
--rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/xml/rml_spec_example_section_3/mapping.ttl
--rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/xml/rml_spec_example_section_3/output.nq
--rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/xml/rml_spec_example_section_3/test_rml_spec_example_section_3_XML.py
--rw-r--r--   0        0        0      435 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/xml/rml_spec_example_section_5/Transport.xml
--rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/xml/rml_spec_example_section_5/mapping.ttl
--rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/xml/rml_spec_example_section_5/output.nq
--rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml/xml/rml_spec_example_section_5/test_rml_spec_example_section_5_XML.py
--rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-in-memory/json_dictionary/RMLIMTC0000/mapping.ttl
--rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-in-memory/json_dictionary/RMLIMTC0000/output.nq
--rw-r--r--   0        0        0      900 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-in-memory/json_dictionary/RMLIMTC0000/test_RMLTC0000_DICT.py
--rw-r--r--   0        0        0      998 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-in-memory/json_dictionary/RMLIMTC0001a/mapping.ttl
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-in-memory/json_dictionary/RMLIMTC0001a/output.nq
--rw-r--r--   0        0        0      803 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-in-memory/json_dictionary/RMLIMTC0001a/test_RMLTC0001a_DICT.py
--rw-r--r--   0        0        0      979 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-in-memory/json_dictionary/RMLIMTC0001b/mapping.ttl
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-in-memory/json_dictionary/RMLIMTC0001b/output.nq
--rw-r--r--   0        0        0      803 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-in-memory/json_dictionary/RMLIMTC0001b/test_RMLTC0001b_DICT.py
--rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-in-memory/json_dictionary/RMLIMTC0002a/mapping.ttl
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-in-memory/json_dictionary/RMLIMTC0002a/output.nq
--rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-in-memory/json_dictionary/RMLIMTC0002a/test_RMLTC0002a_DICT.py
--rw-r--r--   0        0        0      973 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-in-memory/json_dictionary/RMLIMTC0002b/mapping.ttl
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-in-memory/json_dictionary/RMLIMTC0002b/output.nq
--rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-in-memory/json_dictionary/RMLIMTC0002b/test_RMLTC0002b_DICT.py
--rw-r--r--   0        0        0      958 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-in-memory/json_dictionary/RMLIMTC0002c/mapping.ttl
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-in-memory/json_dictionary/RMLIMTC0002c/output.nq
--rw-r--r--   0        0        0      751 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-in-memory/json_dictionary/RMLIMTC0002c/test_RMLTC0002c_DICT.py
--rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-in-memory/json_dictionary/RMLIMTC0002e/mapping.ttl
--rw-r--r--   0        0        0      751 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-in-memory/json_dictionary/RMLIMTC0002e/test_RMLTC0002e_DICT.py
--rw-r--r--   0        0        0     1021 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-in-memory/json_dictionary/RMLIMTC0003c/mapping.ttl
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-in-memory/json_dictionary/RMLIMTC0003c/output.nq
--rw-r--r--   0        0        0      857 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-in-memory/json_dictionary/RMLIMTC0003c/test_RMLTC0003c_DICT.py
--rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-in-memory/json_dictionary/RMLIMTC0004a/mapping.ttl
--rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-in-memory/json_dictionary/RMLIMTC0004a/output.nq
--rw-r--r--   0        0        0      833 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-in-memory/json_dictionary/RMLIMTC0004a/test_RMLTC0004a_DICT.py
--rw-r--r--   0        0        0      996 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-in-memory/json_dictionary/RMLIMTC0004b/mapping.ttl
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-in-memory/json_dictionary/RMLIMTC0004b/output.nq
--rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-in-memory/json_dictionary/RMLIMTC0004b/test_RMLTC0004b_DICT.py
--rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-in-memory/json_dictionary/RMLIMTC0005a/mapping.ttl
--rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-in-memory/json_dictionary/RMLIMTC0005a/output.nq
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-in-memory/json_dictionary/RMLIMTC0005a/test_RMLTC0005a_DICT.py
--rw-r--r--   0        0        0     1040 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-in-memory/json_dictionary/RMLIMTC0006a/mapping.ttl
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-in-memory/json_dictionary/RMLIMTC0006a/output.nq
--rw-r--r--   0        0        0      857 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-in-memory/json_dictionary/RMLIMTC0006a/test_RMLTC0006a_DICT.py
--rw-r--r--   0        0        0     1019 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-in-memory/json_dictionary/RMLIMTC0007a/mapping.ttl
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-in-memory/json_dictionary/RMLIMTC0007a/output.nq
--rw-r--r--   0        0        0      857 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-in-memory/json_dictionary/RMLIMTC0007a/test_RMLTC0007a_DICT.py
--rw-r--r--   0        0        0     1155 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-in-memory/json_dictionary/RMLIMTC0007b/mapping.ttl
--rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-in-memory/json_dictionary/RMLIMTC0007b/output.nq
--rw-r--r--   0        0        0      857 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-in-memory/json_dictionary/RMLIMTC0007b/test_RMLTC0007b_DICT.py
--rw-r--r--   0        0        0     1116 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-in-memory/json_dictionary/RMLIMTC0007c/mapping.ttl
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-in-memory/json_dictionary/RMLIMTC0007c/output.nq
--rw-r--r--   0        0        0      857 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-in-memory/json_dictionary/RMLIMTC0007c/test_RMLTC0007c_DICT.py
--rw-r--r--   0        0        0     1305 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-in-memory/json_dictionary/RMLIMTC0007d/mapping.ttl
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-in-memory/json_dictionary/RMLIMTC0007d/output.nq
--rw-r--r--   0        0        0      857 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-in-memory/json_dictionary/RMLIMTC0007d/test_RMLTC0007d_DICT.py
--rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-in-memory/json_dictionary/RMLIMTC0007e/mapping.ttl
--rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-in-memory/json_dictionary/RMLIMTC0007e/output.nq
--rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-in-memory/json_dictionary/RMLIMTC0007e/test_RMLTC0007e_DICT.py
--rw-r--r--   0        0        0     1254 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-in-memory/json_dictionary/RMLIMTC0007f/mapping.ttl
--rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-in-memory/json_dictionary/RMLIMTC0007f/output.nq
--rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-in-memory/json_dictionary/RMLIMTC0007f/test_RMLTC0007f_DICT.py
--rw-r--r--   0        0        0     1019 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-in-memory/json_dictionary/RMLIMTC0007g/mapping.ttl
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-in-memory/json_dictionary/RMLIMTC0007g/output.nq
--rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-in-memory/json_dictionary/RMLIMTC0007g/test_RMLTC0007g_DICT.py
--rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-in-memory/json_dictionary/RMLIMTC0007h/mapping.ttl
--rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-in-memory/json_dictionary/RMLIMTC0007h/test_RMLTC0007h_DICT.py
--rw-r--r--   0        0        0     1401 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-in-memory/json_dictionary/RMLIMTC0008a/mapping.ttl
--rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-in-memory/json_dictionary/RMLIMTC0008a/output.nq
--rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-in-memory/json_dictionary/RMLIMTC0008a/test_RMLTC0008a_DICT.py
--rw-r--r--   0        0        0     1909 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-in-memory/json_dictionary/RMLIMTC0008b/mapping.ttl
--rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-in-memory/json_dictionary/RMLIMTC0008b/output.nq
--rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-in-memory/json_dictionary/RMLIMTC0008b/test_RMLTC0008b_DICT.py
--rw-r--r--   0        0        0     1045 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-in-memory/json_dictionary/RMLIMTC0008c/mapping.ttl
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-in-memory/json_dictionary/RMLIMTC0008c/output.nq
--rw-r--r--   0        0        0      857 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-in-memory/json_dictionary/RMLIMTC0008c/test_RMLTC0008c_DICT.py
--rw-r--r--   0        0        0     1843 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-in-memory/json_dictionary/RMLIMTC0009a/mapping.ttl
--rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-in-memory/json_dictionary/RMLIMTC0009a/output.nq
--rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-in-memory/json_dictionary/RMLIMTC0009a/test_RMLTC0009a_DICT.py
--rw-r--r--   0        0        0     2153 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-in-memory/json_dictionary/RMLIMTC0009b/mapping.ttl
--rw-r--r--   0        0        0     1198 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-in-memory/json_dictionary/RMLIMTC0009b/output.nq
--rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-in-memory/json_dictionary/RMLIMTC0009b/test_RMLTC0009b_DICT.py
--rw-r--r--   0        0        0     1011 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-in-memory/json_dictionary/RMLIMTC0010a/mapping.ttl
--rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-in-memory/json_dictionary/RMLIMTC0010a/output.nq
--rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-in-memory/json_dictionary/RMLIMTC0010a/test_RMLTC0010a_DICT.py
--rw-r--r--   0        0        0     1018 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-in-memory/json_dictionary/RMLIMTC0010b/mapping.ttl
--rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-in-memory/json_dictionary/RMLIMTC0010b/output.nq
--rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-in-memory/json_dictionary/RMLIMTC0010b/test_RMLTC0010b_DICT.py
--rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-in-memory/json_dictionary/RMLIMTC0010c/mapping.ttl
--rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-in-memory/json_dictionary/RMLIMTC0010c/output.nq
--rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-in-memory/json_dictionary/RMLIMTC0010c/test_RMLTC0010c_DICT.py
--rw-r--r--   0        0        0     2261 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-in-memory/json_dictionary/RMLIMTC0011b/mapping.ttl
--rw-r--r--   0        0        0     1229 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-in-memory/json_dictionary/RMLIMTC0011b/output.nq
--rw-r--r--   0        0        0     1391 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-in-memory/json_dictionary/RMLIMTC0011b/test_RMLTC0011b_DICT.py
--rw-r--r--   0        0        0     1146 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-in-memory/json_dictionary/RMLIMTC0012a/mapping.ttl
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-in-memory/json_dictionary/RMLIMTC0012a/output.nq
--rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-in-memory/json_dictionary/RMLIMTC0012a/test_RMLTC0012a_DICT.py
--rw-r--r--   0        0        0     1553 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-in-memory/json_dictionary/RMLIMTC0012b/mapping.ttl
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-in-memory/json_dictionary/RMLIMTC0012b/output.nq
--rw-r--r--   0        0        0     1129 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-in-memory/json_dictionary/RMLIMTC0012b/test_RMLTC0012b_DICT.py
--rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-in-memory/json_dictionary/RMLIMTC0012c/mapping.ttl
--rw-r--r--   0        0        0      865 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-in-memory/json_dictionary/RMLIMTC0012c/test_RMLTC0012c_DICT.py
--rw-r--r--   0        0        0     1235 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-in-memory/json_dictionary/RMLIMTC0012d/mapping.ttl
--rw-r--r--   0        0        0      865 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-in-memory/json_dictionary/RMLIMTC0012d/test_RMLTC0012d_DICT.py
--rw-r--r--   0        0        0      997 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-in-memory/json_dictionary/RMLIMTC0013a/mapping.ttl
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-in-memory/json_dictionary/RMLIMTC0013a/output.nq
--rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-in-memory/json_dictionary/RMLIMTC0013a/test_RMLTC0013a_DICT.py
--rw-r--r--   0        0        0     1577 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-in-memory/json_dictionary/RMLIMTC0015a/mapping.ttl
--rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-in-memory/json_dictionary/RMLIMTC0015a/output.nq
--rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-in-memory/json_dictionary/RMLIMTC0015a/test_RMLTC0015a_DICT.py
--rw-r--r--   0        0        0     1574 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-in-memory/json_dictionary/RMLIMTC0015b/mapping.ttl
--rw-r--r--   0        0        0      991 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-in-memory/json_dictionary/RMLIMTC0015b/test_RMLTC0015b_DICT.py
--rw-r--r--   0        0        0      984 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0000/mapping.ttl
--rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0000/output.nq
--rw-r--r--   0        0        0      790 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0000/test_RMLIMTC0000_DF.py
--rw-r--r--   0        0        0      983 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0001a/mapping.ttl
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0001a/output.nq
--rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0001a/student.csv
--rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0001a/test_RMLTC0001a_DF.py
--rw-r--r--   0        0        0      994 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0001b/mapping.ttl
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0001b/output.nq
--rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0001b/test_RMLIMTC0001b_DF.py
--rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0002a/mapping.ttl
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0002a/output.nq
--rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0002a/test_RMLIMTC0002a_DF.py
--rw-r--r--   0        0        0      988 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0002b/mapping.ttl
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0002b/output.nq
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0002b/test_RMLIMTC0002b_DF.py
--rw-r--r--   0        0        0      973 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0002c/mapping.ttl
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0002c/output.nq
--rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0002c/test_RMLIMTC0002c_DF.py
--rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0002e/mapping.ttl
--rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0002e/test_RMLIMTC0002e_DF.py
--rw-r--r--   0        0        0     1034 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0003c/mapping.ttl
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0003c/output.nq
--rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0003c/test_RMLIMTC0003c_DF.py
--rw-r--r--   0        0        0     1552 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0004a/mapping.ttl
--rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0004a/output.nq
--rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0004a/test_RMLIMTC0004a_DF.py
--rw-r--r--   0        0        0     1005 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0004b/mapping.ttl
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0004b/output.nq
--rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0004b/test_RMLIMTC0004b_DF.py
--rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0005a/mapping.ttl
--rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0005a/output.nq
--rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0005a/test_RMLIMTC0005a_DF.py
--rw-r--r--   0        0        0     1056 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0006a/mapping.ttl
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0006a/output.nq
--rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0006a/test_RMLIMTC0006a_DF.py
--rw-r--r--   0        0        0     1034 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0007a/mapping.ttl
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0007a/output.nq
--rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0007a/test_RMLIMTC0007a_DF.py
--rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0007b/mapping.ttl
--rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0007b/output.nq
--rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0007b/test_RMLIMTC0007b_DF.py
--rw-r--r--   0        0        0     1131 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0007c/mapping.ttl
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0007c/output.nq
--rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0007c/test_RMLIMTC0007c_DF.py
--rw-r--r--   0        0        0     1322 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0007d/mapping.ttl
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0007d/output.nq
--rw-r--r--   0        0        0      835 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0007d/test_RMLTC0007d_DF.py
--rw-r--r--   0        0        0     1151 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0007e/mapping.ttl
--rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0007e/output.nq
--rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0007e/test_RMLIMTC0007e_DF.py
--rw-r--r--   0        0        0     1269 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0007f/mapping.ttl
--rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0007f/output.nq
--rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0007f/test_RMLIMTC0007f_DF.py
--rw-r--r--   0        0        0     1034 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0007g/mapping.ttl
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0007g/output.nq
--rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0007g/test_RMLIMTC0007g_DF.py
--rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0007h/mapping.ttl
--rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0007h/test_RMLIMTC0007h_DF.py
--rw-r--r--   0        0        0     1416 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0008a/mapping.ttl
--rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0008a/output.nq
--rw-r--r--   0        0        0      835 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0008a/test_RMLIMTC0008a_DF.py
--rw-r--r--   0        0        0     1933 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0008b/mapping.ttl
--rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0008b/output.nq
--rw-r--r--   0        0        0      835 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0008b/test_RMLIMTC0008b_DF.py
--rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0008c/mapping.ttl
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0008c/output.nq
--rw-r--r--   0        0        0      835 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0008c/test_RMLIMTC0008c_DF.py
--rw-r--r--   0        0        0     1875 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0009a/mapping.ttl
--rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0009a/output.nq
--rw-r--r--   0        0        0      925 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0009a/test_RMLIMTC0009a_DF.py
--rw-r--r--   0        0        0     2190 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0009b/mapping.ttl
--rw-r--r--   0        0        0     1198 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0009b/output.nq
--rw-r--r--   0        0        0      925 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0009b/test_RMLIMTC0009b_DF.py
--rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0010a/mapping.ttl
--rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0010a/output.nq
--rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0010a/test_RMLIMTC0010a_DF.py
--rw-r--r--   0        0        0     1033 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0010b/mapping.ttl
--rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0010b/output.nq
--rw-r--r--   0        0        0      930 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0010b/test_RMLIMTC0010b_DF.py
--rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0010c/mapping.ttl
--rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0010c/output.nq
--rw-r--r--   0        0        0      930 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0010c/test_RMLIMTC0010c_DF.py
--rw-r--r--   0        0        0     2315 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0011b/mapping.ttl
--rw-r--r--   0        0        0     1229 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0011b/output.nq
--rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0011b/test_RMLIMTC0011b_DF.py
--rw-r--r--   0        0        0     1162 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0012a/mapping.ttl
--rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0012a/output.nq
--rw-r--r--   0        0        0      831 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0012a/test_RMLIMTC0012a_DF.py
--rw-r--r--   0        0        0     1589 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0012b/mapping.ttl
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0012b/output.nq
--rw-r--r--   0        0        0      987 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0012b/test_RMLIMTC0012b_DF.py
--rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0012c/mapping.ttl
--rw-r--r--   0        0        0      796 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0012c/test_RMLIMTC0012c_DF.py
--rw-r--r--   0        0        0     1252 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0012d/mapping.ttl
--rw-r--r--   0        0        0      797 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0012d/test_RMLIMTC0012d_DF.py
--rw-r--r--   0        0        0     1607 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0015a/mapping.ttl
--rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0015a/output.nq
--rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0015a/test_RMLIMTC0015a_DF.py
--rw-r--r--   0        0        0     1604 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0015b/mapping.ttl
--rw-r--r--   0        0        0      922 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0015b/test_RMLIMTC0015b_DF.py
--rw-r--r--   0        0        0     1662 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-in-memory/pandas_dataframe/triples_map_without_pom/mapping.ttl
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-in-memory/pandas_dataframe/triples_map_without_pom/output.nq
--rw-r--r--   0        0        0      937 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-in-memory/pandas_dataframe/triples_map_without_pom/test_triples_map_without_pom_DF.py
--rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-star/RMLSTARTC001a/data.csv
--rw-r--r--   0        0        0     1041 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-star/RMLSTARTC001a/mapping.ttl
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-star/RMLSTARTC001a/output.nq
--rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-star/RMLSTARTC001a/test_RMLSTARTC001a_CSV.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-star/RMLSTARTC001b/data1.csv
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-star/RMLSTARTC001b/data2.csv
--rw-r--r--   0        0        0     1146 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-star/RMLSTARTC001b/mapping.ttl
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-star/RMLSTARTC001b/output.nq
--rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-star/RMLSTARTC001b/test_RMLSTARTC001b_CSV.py
--rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-star/RMLSTARTC002a/data.csv
--rw-r--r--   0        0        0     1132 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-star/RMLSTARTC002a/mapping.ttl
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-star/RMLSTARTC002a/output.nq
--rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-star/RMLSTARTC002a/test_RMLSTARTC002a_CSV.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-star/RMLSTARTC002b/data1.csv
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-star/RMLSTARTC002b/data2.csv
--rw-r--r--   0        0        0     1238 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-star/RMLSTARTC002b/mapping.ttl
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-star/RMLSTARTC002b/output.nq
--rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-star/RMLSTARTC002b/test_RMLSTARTC002b_CSV.py
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-star/RMLSTARTC003a/data.csv
--rw-r--r--   0        0        0     1478 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-star/RMLSTARTC003a/mapping.ttl
--rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-star/RMLSTARTC003a/output.nq
--rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-star/RMLSTARTC003a/test_RMLSTARTC003a_CSV.py
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-star/RMLSTARTC003b/data1.csv
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-star/RMLSTARTC003b/data2.csv
--rw-r--r--   0        0        0     1585 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-star/RMLSTARTC003b/mapping.ttl
--rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-star/RMLSTARTC003b/output.nq
--rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-star/RMLSTARTC003b/test_RMLSTARTC003b_CSV.py
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-star/RMLSTARTC004a/data.csv
--rw-r--r--   0        0        0     1455 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-star/RMLSTARTC004a/mapping.ttl
--rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-star/RMLSTARTC004a/output.nq
--rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-star/RMLSTARTC004a/test_RMLSTARTC004a_CSV.py
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-star/RMLSTARTC004b/data1.csv
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-star/RMLSTARTC004b/data2.csv
--rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-star/RMLSTARTC004b/mapping.ttl
--rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-star/RMLSTARTC004b/output.nq
--rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-star/RMLSTARTC004b/test_RMLSTARTC004b_CSV.py
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-star/RMLSTARTC005a/data.csv
--rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-star/RMLSTARTC005a/mapping.ttl
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-star/RMLSTARTC005a/output.nq
--rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-star/RMLSTARTC005a/test_RMLSTARTC005a_CSV.py
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-star/RMLSTARTC005b/data1.csv
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-star/RMLSTARTC005b/data2.csv
--rw-r--r--   0        0        0     1223 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-star/RMLSTARTC005b/mapping.ttl
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-star/RMLSTARTC005b/output.nq
--rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-star/RMLSTARTC005b/test_RMLSTARTC005b_CSV.py
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-star/RMLSTARTC006a/data.csv
--rw-r--r--   0        0        0     1201 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-star/RMLSTARTC006a/mapping.ttl
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-star/RMLSTARTC006a/output.nq
--rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-star/RMLSTARTC006a/test_RMLSTARTC006a_CSV.py
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-star/RMLSTARTC006b/data1.csv
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-star/RMLSTARTC006b/data2.csv
--rw-r--r--   0        0        0     1323 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-star/RMLSTARTC006b/mapping.ttl
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-star/RMLSTARTC006b/output.nq
--rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-star/RMLSTARTC006b/test_RMLSTARTC006b_CSV.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-star/RMLSTARTC007a/data.csv
--rw-r--r--   0        0        0     1485 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-star/RMLSTARTC007a/mapping.ttl
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-star/RMLSTARTC007a/output.nq
--rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-star/RMLSTARTC007a/test_RMLSTARTC007a_CSV.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-star/RMLSTARTC007b/data1.csv
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-star/RMLSTARTC007b/data2.csv
--rw-r--r--   0        0        0     1609 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-star/RMLSTARTC007b/mapping.ttl
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-star/RMLSTARTC007b/output.nq
--rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-star/RMLSTARTC007b/test_RMLSTARTC007b_CSV.py
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-star/RMLSTARTC008a/data.csv
--rw-r--r--   0        0        0     3089 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-star/RMLSTARTC008a/mapping.ttl
--rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-star/RMLSTARTC008a/output.nq
--rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-star/RMLSTARTC008a/test_RMLSTARTC008a_CSV.py
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-star/RMLSTARTC008b/data1.csv
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-star/RMLSTARTC008b/data2.csv
--rw-r--r--   0        0        0     3225 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-star/RMLSTARTC008b/mapping.ttl
--rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-star/RMLSTARTC008b/output.nq
--rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rml-star/RMLSTARTC008b/test_RMLSTARTC008b_CSV.py
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rmltv/RMLTVTC0002d/mapping.ttl
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rmltv/RMLTVTC0002d/output.nq
--rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rmltv/RMLTVTC0002d/student.csv
--rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rmltv/RMLTVTC0002d/test_RMLTVTC0002d_CSV.py
--rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rmltv/RMLTVTC0002g/mapping.ttl
--rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rmltv/RMLTVTC0002g/student.csv
--rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rmltv/RMLTVTC0002g/test_RMLTVTC0002g_CSV.py
--rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rmltv/RMLTVTC0002h/mapping.ttl
--rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rmltv/RMLTVTC0002h/student.csv
--rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rmltv/RMLTVTC0002h/test_RMLTVTC0002h_CSV.py
--rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rmltv/RMLTVTC0002i/mapping.ttl
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rmltv/RMLTVTC0002i/output.nq
--rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rmltv/RMLTVTC0002i/student.csv
--rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rmltv/RMLTVTC0002i/test_RMLTVTC0002i_CSV.py
--rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rmltv/RMLTVTC0002j/mapping.ttl
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rmltv/RMLTVTC0002j/output.nq
--rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rmltv/RMLTVTC0002j/student.csv
--rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rmltv/RMLTVTC0002j/test_RMLTVTC0002j_CSV.py
--rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rmltv/RMLTVTC0003b/mapping.ttl
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rmltv/RMLTVTC0003b/output.nq
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rmltv/RMLTVTC0003b/student.csv
--rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rmltv/RMLTVTC0003b/test_RMLTVTC0003b_CSV.py
--rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rmltv/RMLTVTC0009c/mapping.ttl
--rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rmltv/RMLTVTC0009c/output.nq
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rmltv/RMLTVTC0009c/sport.csv
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rmltv/RMLTVTC0009c/student.csv
--rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rmltv/RMLTVTC0009c/test_RMLTVTC0009c_CSV.py
--rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rmltv/RMLTVTC0009d/mapping.ttl
--rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rmltv/RMLTVTC0009d/output.nq
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rmltv/RMLTVTC0009d/sport.csv
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rmltv/RMLTVTC0009d/student.csv
--rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rmltv/RMLTVTC0009d/test_RMLTVTC0009d_CSV.py
--rw-r--r--   0        0        0     1753 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rmltv/RMLTVTC0011a/mapping.ttl
--rw-r--r--   0        0        0     1525 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rmltv/RMLTVTC0011a/output.nq
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rmltv/RMLTVTC0011a/sport.csv
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rmltv/RMLTVTC0011a/student.csv
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rmltv/RMLTVTC0011a/student_sport.csv
--rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rmltv/RMLTVTC0011a/test_RMLTVTC0011a_CSV.py
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rmltv/RMLTVTC0014d/dept.csv
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rmltv/RMLTVTC0014d/emp.csv
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rmltv/RMLTVTC0014d/likes.csv
--rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rmltv/RMLTVTC0014d/mapping.ttl
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rmltv/RMLTVTC0014d/output.nq
--rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rmltv/RMLTVTC0014d/test_RMLTVTC0014d_CSV.py
--rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rmltv/RMLTVTC0015a/country.csv
--rw-r--r--   0        0        0     1012 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rmltv/RMLTVTC0015a/mapping.ttl
--rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rmltv/RMLTVTC0015a/output.nq
--rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rmltv/RMLTVTC0015a/test_RMLTVTC0015a_CSV.py
--rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rmltv/RMLTVTC0015b/country.csv
--rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rmltv/RMLTVTC0015b/mapping.ttl
--rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rmltv/RMLTVTC0015b/test_RMLTVTC0015b_CSV.py
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rmltv/RMLTVTC0019a/employee.csv
--rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rmltv/RMLTVTC0019a/mapping.ttl
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rmltv/RMLTVTC0019a/output.nq
--rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rmltv/RMLTVTC0019a/test_RMLTVTC0019a_CSV.py
--rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rmltv/RMLTVTC0026a/mapping.ttl
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rmltv/RMLTVTC0026a/mixed_content_list.csv
--rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rmltv/RMLTVTC0026a/output.nq
--rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rmltv/RMLTVTC0026a/test_RMLTVTC0026a_CSV.py
--rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rmltv/RMLTVTC0027a/mapping.ttl
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rmltv/RMLTVTC0027a/mixed_content_json.csv
--rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rmltv/RMLTVTC0027a/output.nq
--rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rmltv/RMLTVTC0027a/test_RMLTVTC0027a_CSV.py
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rmltv/RMLTVTC0028a/aka_title.csv
--rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rmltv/RMLTVTC0028a/mapping.ttl
--rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rmltv/RMLTVTC0028a/output.nq
--rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rmltv/RMLTVTC0028a/test_RMLTVTC0028a_CSV.py
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rmltv/RMLTVTC0028a/title.csv
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rmltv/RMLTVTC0029a/department.csv
--rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rmltv/RMLTVTC0029a/faculty.csv
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rmltv/RMLTVTC0029a/graduatecourse.csv
--rw-r--r--   0        0        0      965 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rmltv/RMLTVTC0029a/mapping.ttl
--rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rmltv/RMLTVTC0029a/output.nq
--rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/test/rmltv/RMLTVTC0029a/test_RMLTVTC0029a_CSV.py
--rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/LICENSE
--rw-r--r--   0        0        0     6860 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/README.md
--rw-r--r--   0        0        0     2660 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/pyproject.toml
--rw-r--r--   0        0        0    10290 2020-02-02 00:00:00.000000 morph_kgc-2.5.0/PKG-INFO
+-rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/.zenodo.json
+-rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/CITATION.cff
+-rw-r--r--   0        0        0      882 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1744 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/mkdocs.yml
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/readthedocs.yml
+-rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/.github/ISSUE_TEMPLATE/bug-report.md
+-rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/.github/ISSUE_TEMPLATE/documentation-improvement.md
+-rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/.github/ISSUE_TEMPLATE/feature-request.md
+-rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/.github/ISSUE_TEMPLATE/installation-issue.md
+-rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/.github/ISSUE_TEMPLATE/submit-quesion.md
+-rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/.github/workflows/pypi-publish.yml
+-rw-r--r--   0        0        0    25137 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/docs/documentation.md
+-rw-r--r--   0        0        0     2553 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/docs/faq.md
+-rw-r--r--   0        0        0     3848 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/docs/index.md
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/docs/requirements.txt
+-rw-r--r--   0        0        0     2516 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/docs/research.md
+-rw-r--r--   0        0        0     5055 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/docs/why-morph-kgc.md
+-rw-r--r--   0        0        0    58421 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/docs/assets/BASF.png
+-rw-r--r--   0        0        0   172672 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/docs/assets/BASF.tif
+-rw-r--r--   0        0        0    44456 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/docs/assets/datos40.png
+-rw-r--r--   0        0        0    40106 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/docs/assets/entente.png
+-rw-r--r--   0        0        0    33187 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/docs/assets/knowledgespaces.png
+-rw-r--r--   0        0        0   299520 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/docs/assets/logo-oeg.png
+-rw-r--r--   0        0        0   133582 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/docs/assets/logo-upm.png
+-rw-r--r--   0        0        0    50123 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/docs/assets/logo.png
+-rw-r--r--   0        0        0    60779 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/docs/assets/sigtrans.png
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/docs/stylesheets/extra.css
+-rw-r--r--   0        0        0     3702 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/examples/README.md
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/examples/configuration-file/basic_config.ini
+-rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/examples/configuration-file/default_config.ini
+-rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/examples/configuration-file/oracle_config.ini
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/examples/csv/config.ini
+-rw-r--r--   0        0        0    33628 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/examples/csv/mapping.csv.ttl
+-rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/examples/csv/data/AGENCY.csv
+-rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/examples/csv/data/CALENDAR.csv
+-rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/examples/csv/data/CALENDAR_DATES.csv
+-rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/examples/csv/data/FEED_INFO.csv
+-rw-r--r--   0        0        0     3503 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/examples/csv/data/FREQUENCIES.csv
+-rw-r--r--   0        0        0     2924 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/examples/csv/data/ROUTES.csv
+-rw-r--r--   0        0        0     3171 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/examples/csv/data/SHAPES.csv
+-rw-r--r--   0        0        0     4379 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/examples/csv/data/STOPS.csv
+-rw-r--r--   0        0        0     4700 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/examples/csv/data/STOP_TIMES.csv
+-rw-r--r--   0        0        0     6000 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/examples/csv/data/TRIPS.csv
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/examples/dataframe/config.ini
+-rw-r--r--   0        0        0      859 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/examples/dataframe/kg_generation.py
+-rw-r--r--   0        0        0     2319 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/examples/dataframe/mapping_rml.ttl
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/examples/dict/config.ini
+-rw-r--r--   0        0        0     1512 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/examples/dict/kg_generation.py
+-rw-r--r--   0        0        0     2330 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/examples/dict/mapping_rml.ttl
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/examples/json/config.ini
+-rw-r--r--   0        0        0     3464 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/examples/json/data.json
+-rw-r--r--   0        0        0     9731 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/examples/json/mapping.json.ttl
+-rw-r--r--   0        0        0     1791 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/examples/json/mapping.json.yaml
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/examples/rdb/config.ini
+-rw-r--r--   0        0        0    29169 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/examples/rdb/gtfs-rdb.r2rml.ttl
+-rw-r--r--   0        0        0    13238 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/examples/tutorial/Morph-KGC.ipynb
+-rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/examples/tutorial/README.md
+-rw-r--r--   0        0        0    34542 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/examples/tutorial/mapping.gtfs.ttl
+-rw-r--r--   0        0        0    26514 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/examples/tutorial/mapping.somef.ttl
+-rw-r--r--   0        0        0    35086 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/examples/tutorial/oeg-upm_morph-kgc.json
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/examples/xml/config.ini
+-rw-r--r--   0        0        0     3656 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/examples/xml/data.xml
+-rw-r--r--   0        0        0     1756 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/examples/xml/mapping.xml.yaml
+-rw-r--r--   0        0        0     9696 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/examples/xml/mappingOA.xml.ttl
+-rw-r--r--   0        0        0     2978 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/src/morph_kgc/__init__.py
+-rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/src/morph_kgc/__main__.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/src/morph_kgc/_version.py
+-rw-r--r--   0        0        0     2205 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/src/morph_kgc/args_parser.py
+-rw-r--r--   0        0        0    14497 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/src/morph_kgc/config.py
+-rw-r--r--   0        0        0     8622 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/src/morph_kgc/constants.py
+-rw-r--r--   0        0        0    25984 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/src/morph_kgc/materializer.py
+-rw-r--r--   0        0        0     8924 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/src/morph_kgc/utils.py
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/src/morph_kgc/data_source/__init__.py
+-rw-r--r--   0        0        0     8867 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/src/morph_kgc/data_source/data_file.py
+-rw-r--r--   0        0        0     2406 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/src/morph_kgc/data_source/python_data.py
+-rw-r--r--   0        0        0     7606 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/src/morph_kgc/data_source/relational_database.py
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/src/morph_kgc/fno/__init__.py
+-rw-r--r--   0        0        0     8530 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/src/morph_kgc/fno/built_in_functions.py
+-rw-r--r--   0        0        0     4636 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/src/morph_kgc/fno/fno_executer.py
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/src/morph_kgc/mapping/__init__.py
+-rw-r--r--   0        0        0     6477 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/src/morph_kgc/mapping/mapping_constants.py
+-rw-r--r--   0        0        0    37748 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/src/morph_kgc/mapping/mapping_parser.py
+-rw-r--r--   0        0        0    20297 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/src/morph_kgc/mapping/mapping_partitioner.py
+-rw-r--r--   0        0        0     1033 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/fno/RMLFNOTC0000-CSV/mapping.ttl
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/fno/RMLFNOTC0000-CSV/output.nq
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/fno/RMLFNOTC0000-CSV/student.csv
+-rw-r--r--   0        0        0      841 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/fno/RMLFNOTC0000-CSV/test_RMLFNOTC0000-CSV.py
+-rw-r--r--   0        0        0     1198 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/fno/RMLFNOTC0001-CSV/mapping.ttl
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/fno/RMLFNOTC0001-CSV/output.nq
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/fno/RMLFNOTC0001-CSV/student.csv
+-rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/fno/RMLFNOTC0001-CSV/test_RMLFNOTC0001-CSV.py
+-rw-r--r--   0        0        0     1196 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/fno/RMLFNOTC0002-CSV/mapping.ttl
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/fno/RMLFNOTC0002-CSV/output.nq
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/fno/RMLFNOTC0002-CSV/student.csv
+-rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/fno/RMLFNOTC0002-CSV/test_RMLFNOTC0002-CSV.py
+-rw-r--r--   0        0        0     1291 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/fno/RMLFNOTC0003-CSV/mapping.ttl
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/fno/RMLFNOTC0003-CSV/output.nq
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/fno/RMLFNOTC0003-CSV/student.csv
+-rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/fno/RMLFNOTC0003-CSV/test_RMLFNOTC0003-CSV.py
+-rw-r--r--   0        0        0     1202 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/fno/RMLFNOTC0004-CSV/mapping.ttl
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/fno/RMLFNOTC0004-CSV/output.nq
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/fno/RMLFNOTC0004-CSV/student.csv
+-rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/fno/RMLFNOTC0004-CSV/test_RMLFNOTC0004-CSV.py
+-rw-r--r--   0        0        0     1160 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/fno/RMLFNOTC0005-CSV/mapping.ttl
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/fno/RMLFNOTC0005-CSV/output.nq
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/fno/RMLFNOTC0005-CSV/student.csv
+-rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/fno/RMLFNOTC0005-CSV/test_RMLFNOTC0005-CSV.py
+-rw-r--r--   0        0        0     1233 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/fno/RMLFNOTC0006-CSV/mapping.ttl
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/fno/RMLFNOTC0006-CSV/output.nq
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/fno/RMLFNOTC0006-CSV/student.csv
+-rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/fno/RMLFNOTC0006-CSV/test_RMLFNOTC0006-CSV.py
+-rw-r--r--   0        0        0     1183 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/fno/RMLFNOTC0008-CSV/mapping.ttl
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/fno/RMLFNOTC0008-CSV/output.nq
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/fno/RMLFNOTC0008-CSV/student.csv
+-rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/fno/RMLFNOTC0008-CSV/test_RMLFNOTC0008-CSV.py
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/fno/array_get_slice/article.tsv
+-rw-r--r--   0        0        0     1766 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/fno/array_get_slice/mapping.ttl
+-rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/fno/array_get_slice/output.nq
+-rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/fno/array_get_slice/test_array_get_slice.py
+-rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/fno/controls_if/calendar.csv
+-rw-r--r--   0        0        0     2024 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/fno/controls_if/mapping.ttl
+-rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/fno/controls_if/output.nq
+-rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/fno/controls_if/test_controls_if.py
+-rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/fno/controls_if_cast/calendar.csv
+-rw-r--r--   0        0        0     2031 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/fno/controls_if_cast/mapping.ttl
+-rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/fno/controls_if_cast/output.nq
+-rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/fno/controls_if_cast/test_controls_if_cast.py
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/fno/date_to_date/calendar.csv
+-rw-r--r--   0        0        0     1489 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/fno/date_to_date/mapping.ttl
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/fno/date_to_date/output.nq
+-rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/fno/date_to_date/test_date_to_date.py
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/fno/math_round/distances.tsv
+-rw-r--r--   0        0        0     1246 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/fno/math_round/mapping.ttl
+-rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/fno/math_round/output.nq
+-rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/fno/math_round/test_math_round.py
+-rw-r--r--   0        0        0     1817 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/fno/nested_function/mapping.ttl
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/fno/nested_function/output.nq
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/fno/nested_function/student.csv
+-rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/fno/nested_function/test_nested_function.py
+-rw-r--r--   0        0        0     1312 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/fno/split_explode/mapping.ttl
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/fno/split_explode/mixed_content_list.csv
+-rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/fno/split_explode/output.nq
+-rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/fno/split_explode/test_split_explode.py
+-rw-r--r--   0        0        0     1317 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/fno/split_explode_null/mapping.ttl
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/fno/split_explode_null/mixed_content_list.csv
+-rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/fno/split_explode_null/output.nq
+-rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/fno/split_explode_null/test_split_explode_null.py
+-rw-r--r--   0        0        0     1183 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/fno/udf/mapping.ttl
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/fno/udf/output.nq
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/fno/udf/student.csv
+-rw-r--r--   0        0        0      781 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/fno/udf/test_udf.py
+-rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/fno/udf/udf.py
+-rw-r--r--   0        0        0     1540 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/issues/issue_118/mapping.ttl
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/issues/issue_118/output.nq
+-rw-r--r--   0        0        0     1500 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/issues/issue_118/premis.xml
+-rw-r--r--   0        0        0      689 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/issues/issue_118/test_issue_118.py
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/issues/issue_124/data.csv
+-rw-r--r--   0        0        0     1724 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/issues/issue_124/mapping.ttl
+-rw-r--r--   0        0        0      838 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/issues/issue_124/output.nq
+-rw-r--r--   0        0        0      758 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/issues/issue_124/test_issue_124.py
+-rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/issues/issue_145/data.csv
+-rw-r--r--   0        0        0     1630 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/issues/issue_145/mapping.ttl
+-rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/issues/issue_145/output.nq
+-rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/issues/issue_145/test_issue_145.py
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/issues/issue_62/data1.csv
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/issues/issue_62/data2.csv
+-rw-r--r--   0        0        0     1043 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/issues/issue_62/mapping.ttl
+-rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/issues/issue_62/output.nq
+-rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/issues/issue_62/test_issue_62.py
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/issues/issue_67/data.csv
+-rw-r--r--   0        0        0      978 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/issues/issue_67/mapping.ttl
+-rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/issues/issue_67/output.nq
+-rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/issues/issue_67/test_issue_67.py
+-rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/issues/issue_80/mapping.rml
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/issues/issue_80/output.nq
+-rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/issues/issue_80/student.csv
+-rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/issues/issue_80/test_issue_80.py
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/issues/issue_81/country_info.csv
+-rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/issues/issue_81/mapping.ttl
+-rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/issues/issue_81/output.nq
+-rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/issues/issue_81/test_issue_81.py
+-rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0000/mapping.ttl
+-rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0000/output.nq
+-rw-r--r--   0        0        0     8192 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0000/resource.db
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0000/resource.sql
+-rw-r--r--   0        0        0      829 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0000/test_R2RMLTC0000_SQLITE.py
+-rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0001a/mapping.ttl
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0001a/output.nq
+-rw-r--r--   0        0        0     8192 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0001a/resource.db
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0001a/resource.sql
+-rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0001a/test_R2RMLTC0001a_SQLITE.py
+-rw-r--r--   0        0        0      489 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0001b/mapping.ttl
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0001b/output.nq
+-rw-r--r--   0        0        0     8192 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0001b/resource.db
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0001b/resource.sql
+-rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0001b/test_R2RMLTC0001b_SQLITE.py
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0002a/mapping.ttl
+-rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0002a/output.nq
+-rw-r--r--   0        0        0     8192 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0002a/resource.db
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0002a/resource.sql
+-rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0002a/test_R2RMLTC0002a_SQLITE.py
+-rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0002b/mapping.ttl
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0002b/output.nq
+-rw-r--r--   0        0        0     8192 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0002b/resource.db
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0002b/resource.sql
+-rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0002b/test_R2RMLTC0002b_SQLITE.py
+-rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0002c/mapping.ttl
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0002c/output.nq
+-rw-r--r--   0        0        0     8192 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0002c/resource.db
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0002c/resource.sql
+-rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0002c/test_R2RMLTC0002c_SQLITE.py
+-rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0002d/mapping.ttl
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0002d/output.nq
+-rw-r--r--   0        0        0     8192 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0002d/resource.db
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0002d/resource.sql
+-rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0002d/test_R2RMLTC0002d_SQLITE.py
+-rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0002e/mapping.ttl
+-rw-r--r--   0        0        0     8192 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0002e/resource.db
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0002e/resource.sql
+-rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0002e/test_R2RMLTC0002e_SQLITE.py
+-rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0002f/mapping.ttl
+-rw-r--r--   0        0        0     8192 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0002f/resource.db
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0002f/resource.sql
+-rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0002f/test_R2RMLTC0002f_SQLITE.py
+-rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0002g/mapping.ttl
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0002g/output.nq
+-rw-r--r--   0        0        0     8192 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0002g/resource.db
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0002g/resource.sql
+-rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0002g/test_R2RMLTC0002g_SQLITE.py
+-rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0002h/mapping.ttl
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0002h/output.nq
+-rw-r--r--   0        0        0     8192 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0002h/resource.db
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0002h/resource.sql
+-rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0002h/test_R2RMLTC0002h_SQLITE.py
+-rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0002i/mapping.ttl
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0002i/output.nq
+-rw-r--r--   0        0        0     8192 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0002i/resource.db
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0002i/resource.sql
+-rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0002i/test_R2RMLTC0002i_SQLITE.py
+-rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0002j/mapping.ttl
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0002j/output.nq
+-rw-r--r--   0        0        0     8192 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0002j/resource.db
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0002j/resource.sql
+-rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0002j/test_R2RMLTC0002j_SQLITE.py
+-rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0003a/R2RMLTC0003a_SQLITE.py
+-rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0003a/mapping.ttl
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0003a/output.nq
+-rw-r--r--   0        0        0     8192 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0003a/resource.db
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0003a/resource.sql
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0003b/mapping.ttl
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0003b/output.nq
+-rw-r--r--   0        0        0     8192 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0003b/resource.db
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0003b/resource.sql
+-rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0003b/test_R2RMLTC0003b_SQLITE.py
+-rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0003c/mapping.ttl
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0003c/output.nq
+-rw-r--r--   0        0        0     8192 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0003c/resource.db
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0003c/resource.sql
+-rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0003c/test_R2RMLTC0003c_SQLITE.py
+-rw-r--r--   0        0        0      839 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0004a/mapping.ttl
+-rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0004a/output.nq
+-rw-r--r--   0        0        0     8192 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0004a/resource.db
+-rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0004a/resource.sql
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0004a/student_sport.csv
+-rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0004a/test_R2RMLTC0004a_SQLITE.py
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0004b/mapping.ttl
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0004b/output.nq
+-rw-r--r--   0        0        0     8192 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0004b/resource.db
+-rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0004b/resource.sql
+-rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0004b/test_R2RMLTC0004b_SQLITE.py
+-rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0005a/mapping.ttl
+-rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0005a/output.nq
+-rw-r--r--   0        0        0     8192 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0005a/resource.db
+-rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0005a/resource.sql
+-rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0005a/test_R2RMLTC0005a_SQLITE.py
+-rw-r--r--   0        0        0      817 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0005b/mapping.ttl
+-rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0005b/output.nq
+-rw-r--r--   0        0        0     8192 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0005b/resource.db
+-rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0005b/resource.sql
+-rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0005b/test_R2RMLTC0005b_SQLITE.py
+-rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0006a/mapping.ttl
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0006a/output.nq
+-rw-r--r--   0        0        0     8192 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0006a/resource.db
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0006a/resource.sql
+-rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0006a/test_R2RMLTC0006a_SQLITE.py
+-rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0007a/mapping.ttl
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0007a/output.nq
+-rw-r--r--   0        0        0     8192 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0007a/resource.db
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0007a/resource.sql
+-rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0007a/test_R2RMLTC0007a_SQLITE.py
+-rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0007b/mapping.ttl
+-rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0007b/output.nq
+-rw-r--r--   0        0        0     8192 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0007b/resource.db
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0007b/resource.sql
+-rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0007b/test_R2RMLTC0007b_SQLITE.py
+-rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0007c/mapping.ttl
+-rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0007c/output.nq
+-rw-r--r--   0        0        0     8192 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0007c/resource.db
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0007c/resource.sql
+-rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0007c/test_R2RMLTC0007c_SQLITE.py
+-rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0007d/mapping.ttl
+-rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0007d/output.nq
+-rw-r--r--   0        0        0     8192 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0007d/resource.db
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0007d/resource.sql
+-rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0007d/test_R2RMLTC0007d_SQLITE.py
+-rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0007e/mapping.ttl
+-rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0007e/output.nq
+-rw-r--r--   0        0        0     8192 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0007e/resource.db
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0007e/resource.sql
+-rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0007e/test_R2RMLTC0007e_SQLITE.py
+-rw-r--r--   0        0        0      763 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0007f/mapping.ttl
+-rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0007f/output.nq
+-rw-r--r--   0        0        0     8192 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0007f/resource.db
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0007f/resource.sql
+-rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0007f/test_R2RMLTC0007f_SQLITE.py
+-rw-r--r--   0        0        0      676 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0007g/mapping.ttl
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0007g/output.nq
+-rw-r--r--   0        0        0     8192 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0007g/resource.db
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0007g/resource.sql
+-rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0007g/test_R2RMLTC0007g_SQLITE.py
+-rw-r--r--   0        0        0      708 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0007h/mapping.ttl
+-rw-r--r--   0        0        0     8192 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0007h/resource.db
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0007h/resource.sql
+-rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0007h/test_R2RMLTC0007h_SQLITE.py
+-rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0008a/mapping.ttl
+-rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0008a/output.nq
+-rw-r--r--   0        0        0     8192 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0008a/resource.db
+-rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0008a/resource.sql
+-rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0008a/test_R2RMLTC0008a_SQLITE.py
+-rw-r--r--   0        0        0     1235 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0008b/mapping.ttl
+-rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0008b/output.nq
+-rw-r--r--   0        0        0     8192 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0008b/resource.db
+-rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0008b/resource.sql
+-rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0008b/test_R2RMLTC0008b_SQLITE.py
+-rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0008c/mapping.ttl
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0008c/output.nq
+-rw-r--r--   0        0        0     8192 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0008c/resource.db
+-rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0008c/resource.sql
+-rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0008c/test_R2RMLTC0008c_SQLITE.py
+-rw-r--r--   0        0        0     1129 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0009a/mapping.ttl
+-rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0009a/output.nq
+-rw-r--r--   0        0        0    12288 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0009a/resource.db
+-rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0009a/resource.sql
+-rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0009a/test_R2RMLTC0009a_SQLITE.py
+-rw-r--r--   0        0        0     1495 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0009b/mapping.ttl
+-rw-r--r--   0        0        0     1198 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0009b/output.nq
+-rw-r--r--   0        0        0    12288 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0009b/resource.db
+-rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0009b/resource.sql
+-rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0009b/test_R2RMLTC0009b_SQLITE.py
+-rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0009c/mapping.ttl
+-rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0009c/output.nq
+-rw-r--r--   0        0        0    12288 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0009c/resource.db
+-rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0009c/resource.sql
+-rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0009c/test_R2RMLTC0009c_SQLITE.py
+-rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0009d/mapping.ttl
+-rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0009d/output.nq
+-rw-r--r--   0        0        0    12288 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0009d/resource.db
+-rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0009d/resource.sql
+-rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0009d/test_R2RMLTC0009d_SQLITE.py
+-rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0010a/mapping.ttl
+-rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0010a/output.nq
+-rw-r--r--   0        0        0     8192 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0010a/resource.db
+-rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0010a/resource.sql
+-rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0010a/test_R2RMLTC0010a_SQLITE.py
+-rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0010b/mapping.ttl
+-rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0010b/output.nq
+-rw-r--r--   0        0        0     8192 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0010b/resource.db
+-rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0010b/resource.sql
+-rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0010b/test_R2RMLTC0010b_SQLITE.py
+-rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0010c/mapping.ttl
+-rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0010c/output.nq
+-rw-r--r--   0        0        0     8192 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0010c/resource.db
+-rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0010c/resource.sql
+-rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0010c/test_R2RMLTC0010c_SQLITE.py
+-rw-r--r--   0        0        0     1660 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0011a/mapping.ttl
+-rw-r--r--   0        0        0     1525 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0011a/output.nq
+-rw-r--r--   0        0        0    20480 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0011a/resource.db
+-rw-r--r--   0        0        0     1143 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0011a/resource.sql
+-rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0011a/test_R2RMLTC0011a_SQLITE.py
+-rw-r--r--   0        0        0     1248 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0011b/mapping.ttl
+-rw-r--r--   0        0        0     1228 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0011b/output.nq
+-rw-r--r--   0        0        0    20480 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0011b/resource.db
+-rw-r--r--   0        0        0     1143 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0011b/resource.sql
+-rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0011b/test_R2RMLTC0011b_SQLITE.py
+-rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0012a/mapping.ttl
+-rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0012a/output.nq
+-rw-r--r--   0        0        0    12288 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0012a/resource.db
+-rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0012a/resource.sql
+-rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0012a/test_R2RMLTC0012a_SQLITE.py
+-rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0012b/mapping.ttl
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0012b/output.nq
+-rw-r--r--   0        0        0    12288 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0012b/resource.db
+-rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0012b/resource.sql
+-rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0012b/test_R2RMLTC0012b_SQLITE.py
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0012c/mapping.ttl
+-rw-r--r--   0        0        0    12288 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0012c/resource.db
+-rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0012c/resource.sql
+-rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0012c/test_R2RMLTC0012c_SQLITE.py
+-rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0012d/mapping.ttl
+-rw-r--r--   0        0        0    12288 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0012d/resource.db
+-rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0012d/resource.sql
+-rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0012d/test_R2RMLTC0012d_SQLITE.py
+-rw-r--r--   0        0        0     1500 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0012e/mapping.ttl
+-rw-r--r--   0        0        0     1252 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0012e/output.nq
+-rw-r--r--   0        0        0    12288 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0012e/resource.db
+-rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0012e/resource.sql
+-rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0012e/test_R2RMLTC0012e_SQLITE.py
+-rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0013a/mapping.ttl
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0013a/output.nq
+-rw-r--r--   0        0        0     8192 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0013a/resource.db
+-rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0013a/resource.sql
+-rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0013a/test_R2RMLTC0013a_SQLITE.py
+-rw-r--r--   0        0        0      843 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0014d/mapping.ttl
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0014d/output.nq
+-rw-r--r--   0        0        0    20480 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0014d/resource.db
+-rw-r--r--   0        0        0      775 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0014d/resource.sql
+-rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0014d/test_R2RMLTC0014d_SQLITE.py
+-rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0015a/mapping.ttl
+-rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0015a/output.nq
+-rw-r--r--   0        0        0    12288 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0015a/resource.db
+-rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0015a/resource.sql
+-rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0015a/test_R2RMLTC0015a_SQLITE.py
+-rw-r--r--   0        0        0     1122 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0015b/mapping.ttl
+-rw-r--r--   0        0        0    12288 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0015b/resource.db
+-rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0015b/resource.sql
+-rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0015b/test_R2RMLTC0015b_SQLITE.py
+-rw-r--r--   0        0        0      974 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0016a/mapping.ttl
+-rw-r--r--   0        0        0     1197 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0016a/output.nq
+-rw-r--r--   0        0        0     8192 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0016a/resource.db
+-rw-r--r--   0        0        0     1435 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0016a/resource.sql
+-rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0016a/test_R2RMLTC0016a_SQLITE.py
+-rw-r--r--   0        0        0      910 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0016b/R2RMLTC0016b_SQLITE.py
+-rw-r--r--   0        0        0      751 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0016b/mapping.ttl
+-rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0016b/output.nq
+-rw-r--r--   0        0        0     8192 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0016b/resource.db
+-rw-r--r--   0        0        0     1435 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0016b/resource.sql
+-rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0016c/R2RMLTC0016c_SQLITE.py
+-rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0016c/mapping.ttl
+-rw-r--r--   0        0        0     1110 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0016c/output.nq
+-rw-r--r--   0        0        0     8192 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0016c/resource.db
+-rw-r--r--   0        0        0     1435 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0016c/resource.sql
+-rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0016d/R2RMLTC0016d_SQLITE.py
+-rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0016d/mapping.ttl
+-rw-r--r--   0        0        0      685 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0016d/output.nq
+-rw-r--r--   0        0        0     8192 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0016d/resource.db
+-rw-r--r--   0        0        0     1435 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0016d/resource.sql
+-rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0016e/R2RMLTC0016e_SQLITE.py
+-rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0016e/mapping.ttl
+-rw-r--r--   0        0        0     1110 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0016e/output.nq
+-rw-r--r--   0        0        0     8192 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0016e/resource.db
+-rw-r--r--   0        0        0     1435 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0016e/resource.sql
+-rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0018a/mapping.ttl
+-rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0018a/output.nq
+-rw-r--r--   0        0        0     8192 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0018a/resource.db
+-rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0018a/resource.sql
+-rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0018a/test_R2RMLTC0018a_SQLITE.py
+-rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0019a/R2RMLTC0019a_SQLITE.py
+-rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0019a/mapping.ttl
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0019a/output.nq
+-rw-r--r--   0        0        0     8192 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0019a/resource.db
+-rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0019a/resource.sql
+-rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0019b/R2RMLTC0019b_SQLITE.py
+-rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0019b/mapping.ttl
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0019b/output.nq
+-rw-r--r--   0        0        0     8192 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0019b/resource.db
+-rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0019b/resource.sql
+-rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0020a/R2RMLTC0020a_SQLITE.py
+-rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0020a/mapping.ttl
+-rw-r--r--   0        0        0      658 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0020a/output.nq
+-rw-r--r--   0        0        0     8192 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0020a/resource.db
+-rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0020a/resource.sql
+-rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0020b/R2RMLTC0020b_SQLITE.py
+-rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0020b/mapping.ttl
+-rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0020b/output.nq
+-rw-r--r--   0        0        0     8192 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0020b/resource.db
+-rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/r2rml/R2RMLTC0020b/resource.sql
+-rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/csv/RMLTC0000/mapping.ttl
+-rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/csv/RMLTC0000/output.nq
+-rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/csv/RMLTC0000/student.csv
+-rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/csv/RMLTC0000/test_RMLTC0000_CSV.py
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/csv/RMLTC0001a/mapping.ttl
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/csv/RMLTC0001a/output.nq
+-rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/csv/RMLTC0001a/student.csv
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/csv/RMLTC0001a/test_RMLTC0001a_CSV.py
+-rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/csv/RMLTC0001b/mapping.ttl
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/csv/RMLTC0001b/output.nq
+-rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/csv/RMLTC0001b/student.csv
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/csv/RMLTC0001b/test_RMLTC0001b_CSV.py
+-rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/csv/RMLTC0002a/mapping.ttl
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/csv/RMLTC0002a/output.nq
+-rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/csv/RMLTC0002a/student.csv
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/csv/RMLTC0002a/test_RMLTC0002a_CSV.py
+-rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/csv/RMLTC0002b/mapping.ttl
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/csv/RMLTC0002b/output.nq
+-rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/csv/RMLTC0002b/student.csv
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/csv/RMLTC0002b/test_RMLTC0002b_CSV.py
+-rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/csv/RMLTC0002c/mapping.ttl
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/csv/RMLTC0002c/output.nq
+-rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/csv/RMLTC0002c/student.csv
+-rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/csv/RMLTC0002c/test_RMLTC0002c_CSV.py
+-rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/csv/RMLTC0002e/mapping.ttl
+-rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/csv/RMLTC0002e/student.csv
+-rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/csv/RMLTC0002e/test_RMLTC0002e_CSV.py
+-rw-r--r--   0        0        0      689 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/csv/RMLTC0003c/mapping.ttl
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/csv/RMLTC0003c/output.nq
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/csv/RMLTC0003c/student.csv
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/csv/RMLTC0003c/test_RMLTC0003c_CSV.py
+-rw-r--r--   0        0        0     1035 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/csv/RMLTC0004a/mapping.ttl
+-rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/csv/RMLTC0004a/output.nq
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/csv/RMLTC0004a/student_sport.csv
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/csv/RMLTC0004a/test_RMLTC0004a_CSV.py
+-rw-r--r--   0        0        0      666 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/csv/RMLTC0004b/mapping.ttl
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/csv/RMLTC0004b/output.nq
+-rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/csv/RMLTC0004b/student.csv
+-rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/csv/RMLTC0004b/test_RMLTC0004b_CSV.py
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/csv/RMLTC0005a/ious.csv
+-rw-r--r--   0        0        0      659 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/csv/RMLTC0005a/mapping.ttl
+-rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/csv/RMLTC0005a/output.nq
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/csv/RMLTC0005a/test_RMLTC0005a_CSV.py
+-rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/csv/RMLTC0006a/mapping.ttl
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/csv/RMLTC0006a/output.nq
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/csv/RMLTC0006a/student.csv
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/csv/RMLTC0006a/test_RMLTC0006a_CSV.py
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/csv/RMLTC0007a/mapping.ttl
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/csv/RMLTC0007a/output.nq
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/csv/RMLTC0007a/student.csv
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/csv/RMLTC0007a/test_RMLTC0007a_CSV.py
+-rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/csv/RMLTC0007b/mapping.ttl
+-rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/csv/RMLTC0007b/output.nq
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/csv/RMLTC0007b/student.csv
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/csv/RMLTC0007b/test_RMLTC0007b_CSV.py
+-rw-r--r--   0        0        0      785 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/csv/RMLTC0007c/mapping.ttl
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/csv/RMLTC0007c/output.nq
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/csv/RMLTC0007c/student.csv
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/csv/RMLTC0007c/test_RMLTC0007c_CSV.py
+-rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/csv/RMLTC0007d/mapping.ttl
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/csv/RMLTC0007d/output.nq
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/csv/RMLTC0007d/student.csv
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/csv/RMLTC0007d/test_RMLTC0007d_CSV.py
+-rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/csv/RMLTC0007e/mapping.ttl
+-rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/csv/RMLTC0007e/output.nq
+-rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/csv/RMLTC0007e/student.csv
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/csv/RMLTC0007e/test_RMLTC0007e_CSV.py
+-rw-r--r--   0        0        0      923 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/csv/RMLTC0007f/mapping.ttl
+-rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/csv/RMLTC0007f/output.nq
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/csv/RMLTC0007f/student.csv
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/csv/RMLTC0007f/test_RMLTC0007f_CSV.py
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/csv/RMLTC0007g/mapping.ttl
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/csv/RMLTC0007g/output.nq
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/csv/RMLTC0007g/student.csv
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/csv/RMLTC0007g/test_RMLTC0007g_CSV.py
+-rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/csv/RMLTC0007h/mapping.ttl
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/csv/RMLTC0007h/student.csv
+-rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/csv/RMLTC0007h/test_RMLTC0007h_CSV.py
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/csv/RMLTC0008a/mapping.ttl
+-rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/csv/RMLTC0008a/output.nq
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/csv/RMLTC0008a/student.csv
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/csv/RMLTC0008a/test_RMLTC0008a_CSV.py
+-rw-r--r--   0        0        0     1410 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/csv/RMLTC0008b/mapping.ttl
+-rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/csv/RMLTC0008b/output.nq
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/csv/RMLTC0008b/student.csv
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/csv/RMLTC0008b/test_RMLTC0008b_CSV.py
+-rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/csv/RMLTC0008c/mapping.ttl
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/csv/RMLTC0008c/output.nq
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/csv/RMLTC0008c/student.csv
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/csv/RMLTC0008c/test_RMLTC0008c_CSV.py
+-rw-r--r--   0        0        0     1344 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/csv/RMLTC0009a/mapping.ttl
+-rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/csv/RMLTC0009a/output.nq
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/csv/RMLTC0009a/sport.csv
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/csv/RMLTC0009a/student.csv
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/csv/RMLTC0009a/test_RMLTC0009a_CSV.py
+-rw-r--r--   0        0        0     1665 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/csv/RMLTC0009b/mapping.ttl
+-rw-r--r--   0        0        0     1198 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/csv/RMLTC0009b/output.nq
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/csv/RMLTC0009b/sport.csv
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/csv/RMLTC0009b/student.csv
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/csv/RMLTC0009b/test_RMLTC0009b_CSV.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/csv/RMLTC0010a/country_info.csv
+-rw-r--r--   0        0        0      685 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/csv/RMLTC0010a/mapping.ttl
+-rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/csv/RMLTC0010a/output.nq
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/csv/RMLTC0010a/test_RMLTC0010a_CSV.py
+-rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/csv/RMLTC0010b/country_info.csv
+-rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/csv/RMLTC0010b/mapping.ttl
+-rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/csv/RMLTC0010b/output.nq
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/csv/RMLTC0010b/test_RMLTC0010b_CSV.py
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/csv/RMLTC0010c/country_info.csv
+-rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/csv/RMLTC0010c/mapping.ttl
+-rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/csv/RMLTC0010c/output.nq
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/csv/RMLTC0010c/test_RMLTC0010c_CSV.py
+-rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/csv/RMLTC0011b/mapping.ttl
+-rw-r--r--   0        0        0     1229 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/csv/RMLTC0011b/output.nq
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/csv/RMLTC0011b/sport.csv
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/csv/RMLTC0011b/student.csv
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/csv/RMLTC0011b/student_sport.csv
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/csv/RMLTC0011b/test_RMLTC0011b_CSV.py
+-rw-r--r--   0        0        0      817 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/csv/RMLTC0012a/mapping.ttl
+-rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/csv/RMLTC0012a/output.nq
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/csv/RMLTC0012a/persons.csv
+-rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/csv/RMLTC0012a/test_RMLTC0012a_CSV.py
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/csv/RMLTC0012b/lives.csv
+-rw-r--r--   0        0        0     1058 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/csv/RMLTC0012b/mapping.ttl
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/csv/RMLTC0012b/output.nq
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/csv/RMLTC0012b/persons.csv
+-rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/csv/RMLTC0012b/test_RMLTC0012b_CSV.py
+-rw-r--r--   0        0        0      731 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/csv/RMLTC0012c/mapping.ttl
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/csv/RMLTC0012c/persons.csv
+-rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/csv/RMLTC0012c/test_RMLTC0012c_CSV.py
+-rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/csv/RMLTC0012d/mapping.ttl
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/csv/RMLTC0012d/persons.csv
+-rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/csv/RMLTC0012d/test_RMLTC0012d_CSV.py
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/csv/RMLTC0015a/country_en.csv
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/csv/RMLTC0015a/country_es.csv
+-rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/csv/RMLTC0015a/mapping.ttl
+-rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/csv/RMLTC0015a/output.nq
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/csv/RMLTC0015a/test_RMLTC0015a_CSV.py
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/csv/RMLTC0015b/country_en.csv
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/csv/RMLTC0015b/country_es.csv
+-rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/csv/RMLTC0015b/mapping.ttl
+-rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/csv/RMLTC0015b/test_RMLTC0015b_CSV.py
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/csv/RMLTC0019a/RMLTC0019a_CSV.py
+-rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/csv/RMLTC0019a/mapping.ttl
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/csv/RMLTC0019a/output.nq
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/csv/RMLTC0019a/persons.csv
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/csv/RMLTC0019b/RMLTC0019b_CSV.py
+-rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/csv/RMLTC0019b/mapping.ttl
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/csv/RMLTC0019b/output.nq
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/csv/RMLTC0019b/persons.csv
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/csv/RMLTC0020a/RMLTC0020a_CSV.py
+-rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/csv/RMLTC0020a/mapping.ttl
+-rw-r--r--   0        0        0      658 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/csv/RMLTC0020a/output.nq
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/csv/RMLTC0020a/student.csv
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/csv/RMLTC0020b/RMLTC0020b_CSV.py
+-rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/csv/RMLTC0020b/mapping.ttl
+-rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/csv/RMLTC0020b/output.nq
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/csv/RMLTC0020b/student.csv
+-rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/csv/null_filter/mapping.ttl
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/csv/null_filter/output.nq
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/csv/null_filter/student.csv
+-rw-r--r--   0        0        0      689 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/csv/null_filter/test_null_filter_CSV.py
+-rw-r--r--   0        0        0     1161 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/csv/triples_map_without_pom/mapping.ttl
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/csv/triples_map_without_pom/output.nq
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/csv/triples_map_without_pom/sport.csv
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/csv/triples_map_without_pom/student.csv
+-rw-r--r--   0        0        0      701 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/csv/triples_map_without_pom/test_triples_map_without_pom_CSV.py
+-rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/json/RMLTC0000/mapping.ttl
+-rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/json/RMLTC0000/output.nq
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/json/RMLTC0000/student.json
+-rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/json/RMLTC0000/test_RMLTC0000_JSON.py
+-rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/json/RMLTC0001a/mapping.ttl
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/json/RMLTC0001a/output.nq
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/json/RMLTC0001a/student.json
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/json/RMLTC0001a/test_RMLTC0001a_JSON.py
+-rw-r--r--   0        0        0      689 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/json/RMLTC0001b/mapping.ttl
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/json/RMLTC0001b/output.nq
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/json/RMLTC0001b/student.json
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/json/RMLTC0001b/test_RMLTC0001b_JSON.py
+-rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/json/RMLTC0002a/mapping.ttl
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/json/RMLTC0002a/output.nq
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/json/RMLTC0002a/student.json
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/json/RMLTC0002a/test_RMLTC0002a_JSON.py
+-rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/json/RMLTC0002b/mapping.ttl
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/json/RMLTC0002b/output.nq
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/json/RMLTC0002b/student.json
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/json/RMLTC0002b/test_RMLTC0002b_JSON.py
+-rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/json/RMLTC0002c/mapping.ttl
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/json/RMLTC0002c/output.nq
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/json/RMLTC0002c/student.json
+-rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/json/RMLTC0002c/test_RMLTC0002c_JSON.py
+-rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/json/RMLTC0002e/mapping.ttl
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/json/RMLTC0002e/student.json
+-rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/json/RMLTC0002e/test_RMLTC0002e_JSON.py
+-rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/json/RMLTC0003c/mapping.ttl
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/json/RMLTC0003c/output.nq
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/json/RMLTC0003c/student.json
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/json/RMLTC0003c/test_RMLTC0003c_JSON.py
+-rw-r--r--   0        0        0     1117 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/json/RMLTC0004a/mapping.ttl
+-rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/json/RMLTC0004a/output.nq
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/json/RMLTC0004a/student_sport.json
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/json/RMLTC0004a/test_RMLTC0004a_JSON.py
+-rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/json/RMLTC0004b/mapping.ttl
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/json/RMLTC0004b/output.nq
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/json/RMLTC0004b/student.json
+-rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/json/RMLTC0004b/test_RMLTC0004b_JSON.py
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/json/RMLTC0005a/ious.json
+-rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/json/RMLTC0005a/mapping.ttl
+-rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/json/RMLTC0005a/output.nq
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/json/RMLTC0005a/test_RMLTC0005a_JSON.py
+-rw-r--r--   0        0        0      751 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/json/RMLTC0006a/mapping.ttl
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/json/RMLTC0006a/output.nq
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/json/RMLTC0006a/student.json
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/json/RMLTC0006a/test_RMLTC0006a_JSON.py
+-rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/json/RMLTC0007a/mapping.ttl
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/json/RMLTC0007a/output.nq
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/json/RMLTC0007a/student.json
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/json/RMLTC0007a/test_RMLTC0007a_JSON.py
+-rw-r--r--   0        0        0      865 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/json/RMLTC0007b/mapping.ttl
+-rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/json/RMLTC0007b/output.nq
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/json/RMLTC0007b/student.json
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/json/RMLTC0007b/test_RMLTC0007b_JSON.py
+-rw-r--r--   0        0        0      826 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/json/RMLTC0007c/mapping.ttl
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/json/RMLTC0007c/output.nq
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/json/RMLTC0007c/student.json
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/json/RMLTC0007c/test_RMLTC0007c_JSON.py
+-rw-r--r--   0        0        0     1015 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/json/RMLTC0007d/mapping.ttl
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/json/RMLTC0007d/output.nq
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/json/RMLTC0007d/student.json
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/json/RMLTC0007d/test_RMLTC0007d_JSON.py
+-rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/json/RMLTC0007e/mapping.ttl
+-rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/json/RMLTC0007e/output.nq
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/json/RMLTC0007e/student.json
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/json/RMLTC0007e/test_RMLTC0007e_JSON.py
+-rw-r--r--   0        0        0      964 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/json/RMLTC0007f/mapping.ttl
+-rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/json/RMLTC0007f/output.nq
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/json/RMLTC0007f/student.json
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/json/RMLTC0007f/test_RMLTC0007f_JSON.py
+-rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/json/RMLTC0007g/mapping.ttl
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/json/RMLTC0007g/output.nq
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/json/RMLTC0007g/student.json
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/json/RMLTC0007g/test_RMLTC0007g_JSON.py
+-rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/json/RMLTC0007h/mapping.ttl
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/json/RMLTC0007h/student.json
+-rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/json/RMLTC0007h/test_RMLTC0007h_JSON.py
+-rw-r--r--   0        0        0     1111 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/json/RMLTC0008a/mapping.ttl
+-rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/json/RMLTC0008a/output.nq
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/json/RMLTC0008a/student.json
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/json/RMLTC0008a/test_RMLTC0008a_JSON.py
+-rw-r--r--   0        0        0     1492 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/json/RMLTC0008b/mapping.ttl
+-rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/json/RMLTC0008b/output.nq
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/json/RMLTC0008b/student.json
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/json/RMLTC0008b/test_RMLTC0008b_JSON.py
+-rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/json/RMLTC0008c/mapping.ttl
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/json/RMLTC0008c/output.nq
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/json/RMLTC0008c/student.json
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/json/RMLTC0008c/test_RMLTC0008c_JSON.py
+-rw-r--r--   0        0        0     1424 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/json/RMLTC0009a/mapping.ttl
+-rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/json/RMLTC0009a/output.nq
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/json/RMLTC0009a/sport.json
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/json/RMLTC0009a/student.json
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/json/RMLTC0009a/test_RMLTC0009a_JSON.py
+-rw-r--r--   0        0        0     1735 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/json/RMLTC0009b/mapping.ttl
+-rw-r--r--   0        0        0     1198 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/json/RMLTC0009b/output.nq
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/json/RMLTC0009b/sport.json
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/json/RMLTC0009b/student.json
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/json/RMLTC0009b/test_RMLTC0009b_JSON.py
+-rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/json/RMLTC0010a/country_info.json
+-rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/json/RMLTC0010a/mapping.ttl
+-rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/json/RMLTC0010a/output.nq
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/json/RMLTC0010a/test_RMLTC0010a_JSON.py
+-rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/json/RMLTC0010b/country_info.json
+-rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/json/RMLTC0010b/mapping.ttl
+-rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/json/RMLTC0010b/output.nq
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/json/RMLTC0010b/test_RMLTC0010b_JSON.py
+-rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/json/RMLTC0010c/country_info.json
+-rw-r--r--   0        0        0      781 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/json/RMLTC0010c/mapping.ttl
+-rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/json/RMLTC0010c/output.nq
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/json/RMLTC0010c/test_RMLTC0010c_JSON.py
+-rw-r--r--   0        0        0     1723 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/json/RMLTC0011b/mapping.ttl
+-rw-r--r--   0        0        0     1229 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/json/RMLTC0011b/output.nq
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/json/RMLTC0011b/sport.json
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/json/RMLTC0011b/student.json
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/json/RMLTC0011b/student_sport.json
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/json/RMLTC0011b/test_RMLTC0011b_JSON.py
+-rw-r--r--   0        0        0      857 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/json/RMLTC0012a/mapping.ttl
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/json/RMLTC0012a/output.nq
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/json/RMLTC0012a/persons.json
+-rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/json/RMLTC0012a/test_RMLTC0012a_JSON.py
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/json/RMLTC0012b/lives.json
+-rw-r--r--   0        0        0     1136 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/json/RMLTC0012b/mapping.ttl
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/json/RMLTC0012b/output.nq
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/json/RMLTC0012b/persons.json
+-rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/json/RMLTC0012b/test_RMLTC0012b_JSON.py
+-rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/json/RMLTC0012c/mapping.ttl
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/json/RMLTC0012c/persons.json
+-rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/json/RMLTC0012c/test_RMLTC0012c_JSON.py
+-rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/json/RMLTC0012d/mapping.ttl
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/json/RMLTC0012d/persons.json
+-rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/json/RMLTC0012d/test_RMLTC0012d_JSON.py
+-rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/json/RMLTC0013a/mapping.ttl
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/json/RMLTC0013a/output.nq
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/json/RMLTC0013a/persons.json
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/json/RMLTC0013a/test_RMLTC0013a_JSON.py
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/json/RMLTC0015a/country_en.json
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/json/RMLTC0015a/country_es.json
+-rw-r--r--   0        0        0     1167 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/json/RMLTC0015a/mapping.ttl
+-rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/json/RMLTC0015a/output.nq
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/json/RMLTC0015a/test_RMLTC0015a_JSON.py
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/json/RMLTC0015b/country_en.json
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/json/RMLTC0015b/country_es.json
+-rw-r--r--   0        0        0     1165 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/json/RMLTC0015b/mapping.ttl
+-rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/json/RMLTC0015b/test_RMLTC0015b_JSON.py
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/json/RMLTC0019a/RMLTC0019a_JSON.py
+-rw-r--r--   0        0        0      720 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/json/RMLTC0019a/mapping.ttl
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/json/RMLTC0019a/output.nq
+-rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/json/RMLTC0019a/persons.json
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/json/RMLTC0019b/RMLTC0019b_JSON.py
+-rw-r--r--   0        0        0      720 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/json/RMLTC0019b/mapping.ttl
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/json/RMLTC0019b/output.nq
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/json/RMLTC0019b/persons.json
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/json/RMLTC0020a/RMLTC0020a_JSON.py
+-rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/json/RMLTC0020a/mapping.ttl
+-rw-r--r--   0        0        0      658 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/json/RMLTC0020a/output.nq
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/json/RMLTC0020a/student.json
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/json/RMLTC0020b/RMLTC0020b_JSON.py
+-rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/json/RMLTC0020b/mapping.ttl
+-rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/json/RMLTC0020b/output.nq
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/json/RMLTC0020b/student.json
+-rw-r--r--   0        0        0     3464 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/json/complex/data.json
+-rw-r--r--   0        0        0     9797 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/json/complex/mapping.ttl
+-rw-r--r--   0        0        0     1791 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/json/complex/mapping.yaml
+-rw-r--r--   0        0        0     3729 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/json/complex/output.nq
+-rw-r--r--   0        0        0     2021 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/json/complex/test_complex_JSON.py
+-rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/tabular/RMLTC0002a_EXCEL/mapping.ttl
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/tabular/RMLTC0002a_EXCEL/output.nq
+-rw-r--r--   0        0        0     4925 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/tabular/RMLTC0002a_EXCEL/student.xlsx
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/tabular/RMLTC0002a_EXCEL/test_RMLTC0002a_EXCEL.py
+-rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/tabular/RMLTC0002a_FEATHER/mapping.ttl
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/tabular/RMLTC0002a_FEATHER/output.nq
+-rw-r--r--   0        0        0     1538 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/tabular/RMLTC0002a_FEATHER/student.feather
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/tabular/RMLTC0002a_FEATHER/test_RMLTC0002a_FEATHER.py
+-rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/tabular/RMLTC0002a_ODS/mapping.ttl
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/tabular/RMLTC0002a_ODS/output.nq
+-rw-r--r--   0        0        0     5269 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/tabular/RMLTC0002a_ODS/student.ods
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/tabular/RMLTC0002a_ODS/test_RMLTC0002a_ODS.py
+-rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/tabular/RMLTC0002a_PARQUET/mapping.ttl
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/tabular/RMLTC0002a_PARQUET/output.nq
+-rw-r--r--   0        0        0     1746 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/tabular/RMLTC0002a_PARQUET/student.parquet
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/tabular/RMLTC0002a_PARQUET/test_RMLTC0002a_PARQUET.py
+-rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/tabular/RMLTC0002a_STATA/mapping.ttl
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/tabular/RMLTC0002a_STATA/output.nq
+-rw-r--r--   0        0        0     1844 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/tabular/RMLTC0002a_STATA/student.dta
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/tabular/RMLTC0002a_STATA/test_RMLTC0002a_STATA.py
+-rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/tabular/RMLTC0002a_TSV/mapping.ttl
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/tabular/RMLTC0002a_TSV/output.nq
+-rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/tabular/RMLTC0002a_TSV/student.tsv
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/tabular/RMLTC0002a_TSV/test_RMLTC0002a_TSV.py
+-rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/xml/RMLTC0000/mapping.ttl
+-rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/xml/RMLTC0000/output.nq
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/xml/RMLTC0000/student.xml
+-rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/xml/RMLTC0000/test_RMLTC0000_XML.py
+-rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/xml/RMLTC0001a/mapping.ttl
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/xml/RMLTC0001a/output.nq
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/xml/RMLTC0001a/student.xml
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/xml/RMLTC0001a/test_RMLTC0001a_XML.py
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/xml/RMLTC0001b/mapping.ttl
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/xml/RMLTC0001b/output.nq
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/xml/RMLTC0001b/student.xml
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/xml/RMLTC0001b/test_RMLTC0001b_XML.py
+-rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/xml/RMLTC0002a/mapping.ttl
+-rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/xml/RMLTC0002a/output.nq
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/xml/RMLTC0002a/student.xml
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/xml/RMLTC0002a/test_RMLTC0002a_XML.py
+-rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/xml/RMLTC0002b/mapping.ttl
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/xml/RMLTC0002b/output.nq
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/xml/RMLTC0002b/student.xml
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/xml/RMLTC0002b/test_RMLTC0002b_XML.py
+-rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/xml/RMLTC0002c/mapping.ttl
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/xml/RMLTC0002c/output.nq
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/xml/RMLTC0002c/student.xml
+-rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/xml/RMLTC0002c/test_RMLTC0002c_XML.py
+-rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/xml/RMLTC0002e/mapping.ttl
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/xml/RMLTC0002e/student.xml
+-rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/xml/RMLTC0002e/test_RMLTC0002e_XML.py
+-rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/xml/RMLTC0003c/mapping.ttl
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/xml/RMLTC0003c/output.nq
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/xml/RMLTC0003c/student.xml
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/xml/RMLTC0003c/test_RMLTC0003c_XML.py
+-rw-r--r--   0        0        0     1115 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/xml/RMLTC0004a/mapping.ttl
+-rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/xml/RMLTC0004a/output.nq
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/xml/RMLTC0004a/student_sport.xml
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/xml/RMLTC0004a/test_RMLTC0004a_XML.py
+-rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/xml/RMLTC0004b/mapping.ttl
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/xml/RMLTC0004b/output.nq
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/xml/RMLTC0004b/student.xml
+-rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/xml/RMLTC0004b/test_RMLTC0004b_XML.py
+-rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/xml/RMLTC0005a/ious.xml
+-rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/xml/RMLTC0005a/mapping.ttl
+-rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/xml/RMLTC0005a/output.nq
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/xml/RMLTC0005a/test_RMLTC0005a_XML.py
+-rw-r--r--   0        0        0      750 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/xml/RMLTC0006a/mapping.ttl
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/xml/RMLTC0006a/output.nq
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/xml/RMLTC0006a/student.xml
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/xml/RMLTC0006a/test_RMLTC0006a_XML.py
+-rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/xml/RMLTC0007a/mapping.ttl
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/xml/RMLTC0007a/output.nq
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/xml/RMLTC0007a/student.xml
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/xml/RMLTC0007a/test_RMLTC0007a_XML.py
+-rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/xml/RMLTC0007b/mapping.ttl
+-rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/xml/RMLTC0007b/output.nq
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/xml/RMLTC0007b/student.xml
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/xml/RMLTC0007b/test_RMLTC0007b_XML.py
+-rw-r--r--   0        0        0      825 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/xml/RMLTC0007c/mapping.ttl
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/xml/RMLTC0007c/output.nq
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/xml/RMLTC0007c/student.xml
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/xml/RMLTC0007c/test_RMLTC0007c_XML.py
+-rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/xml/RMLTC0007d/mapping.ttl
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/xml/RMLTC0007d/output.nq
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/xml/RMLTC0007d/student.xml
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/xml/RMLTC0007d/test_RMLTC0007d_XML.py
+-rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/xml/RMLTC0007e/mapping.ttl
+-rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/xml/RMLTC0007e/output.nq
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/xml/RMLTC0007e/student.xml
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/xml/RMLTC0007e/test_RMLTC0007e_XML.py
+-rw-r--r--   0        0        0      963 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/xml/RMLTC0007f/mapping.ttl
+-rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/xml/RMLTC0007f/output.nq
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/xml/RMLTC0007f/student.xml
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/xml/RMLTC0007f/test_RMLTC0007f_XML.py
+-rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/xml/RMLTC0007g/mapping.ttl
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/xml/RMLTC0007g/output.nq
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/xml/RMLTC0007g/student.xml
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/xml/RMLTC0007g/test_RMLTC0007g_XML.py
+-rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/xml/RMLTC0007h/mapping.ttl
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/xml/RMLTC0007h/student.xml
+-rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/xml/RMLTC0007h/test_RMLTC0007h_XML.py
+-rw-r--r--   0        0        0     1110 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/xml/RMLTC0008a/mapping.ttl
+-rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/xml/RMLTC0008a/output.nq
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/xml/RMLTC0008a/student.xml
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/xml/RMLTC0008a/test_RMLTC0008a_XML.py
+-rw-r--r--   0        0        0     1490 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/xml/RMLTC0008b/mapping.ttl
+-rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/xml/RMLTC0008b/output.nq
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/xml/RMLTC0008b/student.xml
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/xml/RMLTC0008b/test_RMLTC0008b_XML.py
+-rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/xml/RMLTC0008c/mapping.ttl
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/xml/RMLTC0008c/output.nq
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/xml/RMLTC0008c/student.xml
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/xml/RMLTC0008c/test_RMLTC0008c_XML.py
+-rw-r--r--   0        0        0     1420 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/xml/RMLTC0009a/mapping.ttl
+-rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/xml/RMLTC0009a/output.nq
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/xml/RMLTC0009a/sport.xml
+-rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/xml/RMLTC0009a/student.xml
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/xml/RMLTC0009a/test_RMLTC0009a_XML.py
+-rw-r--r--   0        0        0     1740 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/xml/RMLTC0009b/mapping.ttl
+-rw-r--r--   0        0        0     1198 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/xml/RMLTC0009b/output.nq
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/xml/RMLTC0009b/sport.xml
+-rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/xml/RMLTC0009b/student.xml
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/xml/RMLTC0009b/test_RMLTC0009b_XML.py
+-rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/xml/RMLTC0010b/country_info.xml
+-rw-r--r--   0        0        0      732 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/xml/RMLTC0010b/mapping.ttl
+-rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/xml/RMLTC0010b/output.nq
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/xml/RMLTC0010b/test_RMLTC0010b_XML.py
+-rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/xml/RMLTC0010c/country_info.xml
+-rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/xml/RMLTC0010c/mapping.ttl
+-rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/xml/RMLTC0010c/output.nq
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/xml/RMLTC0010c/test_RMLTC0010c_XML.py
+-rw-r--r--   0        0        0     1715 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/xml/RMLTC0011b/mapping.ttl
+-rw-r--r--   0        0        0     1229 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/xml/RMLTC0011b/output.nq
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/xml/RMLTC0011b/sport.xml
+-rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/xml/RMLTC0011b/student.xml
+-rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/xml/RMLTC0011b/student_sport.xml
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/xml/RMLTC0011b/test_RMLTC0011b_XML.py
+-rw-r--r--   0        0        0      855 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/xml/RMLTC0012a/mapping.ttl
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/xml/RMLTC0012a/output.nq
+-rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/xml/RMLTC0012a/persons.xml
+-rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/xml/RMLTC0012a/test_RMLTC0012a_XML.py
+-rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/xml/RMLTC0012b/lives.xml
+-rw-r--r--   0        0        0     1132 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/xml/RMLTC0012b/mapping.ttl
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/xml/RMLTC0012b/output.nq
+-rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/xml/RMLTC0012b/persons.xml
+-rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/xml/RMLTC0012b/test_RMLTC0012b_XML.py
+-rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/xml/RMLTC0012c/mapping.ttl
+-rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/xml/RMLTC0012c/persons.xml
+-rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/xml/RMLTC0012c/test_RMLTC0012c_XML.py
+-rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/xml/RMLTC0012d/mapping.ttl
+-rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/xml/RMLTC0012d/persons.xml
+-rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/xml/RMLTC0012d/test_RMLTC0012d_XML.py
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/xml/RMLTC0015a/country_en.xml
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/xml/RMLTC0015a/country_es.xml
+-rw-r--r--   0        0        0     1165 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/xml/RMLTC0015a/mapping.ttl
+-rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/xml/RMLTC0015a/output.nq
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/xml/RMLTC0015a/test_RMLTC0015a_XML.py
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/xml/RMLTC0015b/country_en.xml
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/xml/RMLTC0015b/country_es.xml
+-rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/xml/RMLTC0015b/mapping.ttl
+-rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/xml/RMLTC0015b/test_RMLTC0015b_XML.py
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/xml/RMLTC0019a/RMLTC0019a_XML.py
+-rw-r--r--   0        0        0      718 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/xml/RMLTC0019a/mapping.ttl
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/xml/RMLTC0019a/output.nq
+-rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/xml/RMLTC0019a/persons.xml
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/xml/RMLTC0019b/RMLTC0019b_XML.py
+-rw-r--r--   0        0        0      718 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/xml/RMLTC0019b/mapping.ttl
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/xml/RMLTC0019b/output.nq
+-rw-r--r--   0        0        0      432 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/xml/RMLTC0019b/persons.xml
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/xml/RMLTC0020a/RMLTC0020a_XML.py
+-rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/xml/RMLTC0020a/mapping.ttl
+-rw-r--r--   0        0        0      658 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/xml/RMLTC0020a/output.nq
+-rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/xml/RMLTC0020a/student.xml
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/xml/RMLTC0020b/RMLTC0020b_XML.py
+-rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/xml/RMLTC0020b/mapping.ttl
+-rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/xml/RMLTC0020b/output.nq
+-rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/xml/RMLTC0020b/student.xml
+-rw-r--r--   0        0        0      859 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/xml/attributes/data.xml
+-rw-r--r--   0        0        0     1516 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/xml/attributes/mapping.ttl
+-rw-r--r--   0        0        0     1532 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/xml/attributes/output.nq
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/xml/attributes/test_attributes_XML.py
+-rw-r--r--   0        0        0     3656 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/xml/complex/data.xml
+-rw-r--r--   0        0        0     9759 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/xml/complex/mapping.ttl
+-rw-r--r--   0        0        0     1756 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/xml/complex/mapping.yaml
+-rw-r--r--   0        0        0     4539 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/xml/complex/output.nq
+-rw-r--r--   0        0        0     2020 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/xml/complex/test_complex_XML.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/xml/rml_spec_example_section_3/Transport.xml
+-rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/xml/rml_spec_example_section_3/mapping.ttl
+-rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/xml/rml_spec_example_section_3/output.nq
+-rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/xml/rml_spec_example_section_3/test_rml_spec_example_section_3_XML.py
+-rw-r--r--   0        0        0      435 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/xml/rml_spec_example_section_5/Transport.xml
+-rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/xml/rml_spec_example_section_5/mapping.ttl
+-rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/xml/rml_spec_example_section_5/output.nq
+-rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml/xml/rml_spec_example_section_5/test_rml_spec_example_section_5_XML.py
+-rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-in-memory/json_dictionary/RMLIMTC0000/mapping.ttl
+-rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-in-memory/json_dictionary/RMLIMTC0000/output.nq
+-rw-r--r--   0        0        0      900 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-in-memory/json_dictionary/RMLIMTC0000/test_RMLTC0000_DICT.py
+-rw-r--r--   0        0        0      998 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-in-memory/json_dictionary/RMLIMTC0001a/mapping.ttl
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-in-memory/json_dictionary/RMLIMTC0001a/output.nq
+-rw-r--r--   0        0        0      803 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-in-memory/json_dictionary/RMLIMTC0001a/test_RMLTC0001a_DICT.py
+-rw-r--r--   0        0        0      979 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-in-memory/json_dictionary/RMLIMTC0001b/mapping.ttl
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-in-memory/json_dictionary/RMLIMTC0001b/output.nq
+-rw-r--r--   0        0        0      803 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-in-memory/json_dictionary/RMLIMTC0001b/test_RMLTC0001b_DICT.py
+-rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-in-memory/json_dictionary/RMLIMTC0002a/mapping.ttl
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-in-memory/json_dictionary/RMLIMTC0002a/output.nq
+-rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-in-memory/json_dictionary/RMLIMTC0002a/test_RMLTC0002a_DICT.py
+-rw-r--r--   0        0        0      973 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-in-memory/json_dictionary/RMLIMTC0002b/mapping.ttl
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-in-memory/json_dictionary/RMLIMTC0002b/output.nq
+-rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-in-memory/json_dictionary/RMLIMTC0002b/test_RMLTC0002b_DICT.py
+-rw-r--r--   0        0        0      958 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-in-memory/json_dictionary/RMLIMTC0002c/mapping.ttl
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-in-memory/json_dictionary/RMLIMTC0002c/output.nq
+-rw-r--r--   0        0        0      751 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-in-memory/json_dictionary/RMLIMTC0002c/test_RMLTC0002c_DICT.py
+-rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-in-memory/json_dictionary/RMLIMTC0002e/mapping.ttl
+-rw-r--r--   0        0        0      751 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-in-memory/json_dictionary/RMLIMTC0002e/test_RMLTC0002e_DICT.py
+-rw-r--r--   0        0        0     1021 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-in-memory/json_dictionary/RMLIMTC0003c/mapping.ttl
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-in-memory/json_dictionary/RMLIMTC0003c/output.nq
+-rw-r--r--   0        0        0      857 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-in-memory/json_dictionary/RMLIMTC0003c/test_RMLTC0003c_DICT.py
+-rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-in-memory/json_dictionary/RMLIMTC0004a/mapping.ttl
+-rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-in-memory/json_dictionary/RMLIMTC0004a/output.nq
+-rw-r--r--   0        0        0      833 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-in-memory/json_dictionary/RMLIMTC0004a/test_RMLTC0004a_DICT.py
+-rw-r--r--   0        0        0      996 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-in-memory/json_dictionary/RMLIMTC0004b/mapping.ttl
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-in-memory/json_dictionary/RMLIMTC0004b/output.nq
+-rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-in-memory/json_dictionary/RMLIMTC0004b/test_RMLTC0004b_DICT.py
+-rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-in-memory/json_dictionary/RMLIMTC0005a/mapping.ttl
+-rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-in-memory/json_dictionary/RMLIMTC0005a/output.nq
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-in-memory/json_dictionary/RMLIMTC0005a/test_RMLTC0005a_DICT.py
+-rw-r--r--   0        0        0     1040 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-in-memory/json_dictionary/RMLIMTC0006a/mapping.ttl
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-in-memory/json_dictionary/RMLIMTC0006a/output.nq
+-rw-r--r--   0        0        0      857 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-in-memory/json_dictionary/RMLIMTC0006a/test_RMLTC0006a_DICT.py
+-rw-r--r--   0        0        0     1019 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-in-memory/json_dictionary/RMLIMTC0007a/mapping.ttl
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-in-memory/json_dictionary/RMLIMTC0007a/output.nq
+-rw-r--r--   0        0        0      857 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-in-memory/json_dictionary/RMLIMTC0007a/test_RMLTC0007a_DICT.py
+-rw-r--r--   0        0        0     1155 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-in-memory/json_dictionary/RMLIMTC0007b/mapping.ttl
+-rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-in-memory/json_dictionary/RMLIMTC0007b/output.nq
+-rw-r--r--   0        0        0      857 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-in-memory/json_dictionary/RMLIMTC0007b/test_RMLTC0007b_DICT.py
+-rw-r--r--   0        0        0     1116 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-in-memory/json_dictionary/RMLIMTC0007c/mapping.ttl
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-in-memory/json_dictionary/RMLIMTC0007c/output.nq
+-rw-r--r--   0        0        0      857 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-in-memory/json_dictionary/RMLIMTC0007c/test_RMLTC0007c_DICT.py
+-rw-r--r--   0        0        0     1305 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-in-memory/json_dictionary/RMLIMTC0007d/mapping.ttl
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-in-memory/json_dictionary/RMLIMTC0007d/output.nq
+-rw-r--r--   0        0        0      857 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-in-memory/json_dictionary/RMLIMTC0007d/test_RMLTC0007d_DICT.py
+-rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-in-memory/json_dictionary/RMLIMTC0007e/mapping.ttl
+-rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-in-memory/json_dictionary/RMLIMTC0007e/output.nq
+-rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-in-memory/json_dictionary/RMLIMTC0007e/test_RMLTC0007e_DICT.py
+-rw-r--r--   0        0        0     1254 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-in-memory/json_dictionary/RMLIMTC0007f/mapping.ttl
+-rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-in-memory/json_dictionary/RMLIMTC0007f/output.nq
+-rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-in-memory/json_dictionary/RMLIMTC0007f/test_RMLTC0007f_DICT.py
+-rw-r--r--   0        0        0     1019 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-in-memory/json_dictionary/RMLIMTC0007g/mapping.ttl
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-in-memory/json_dictionary/RMLIMTC0007g/output.nq
+-rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-in-memory/json_dictionary/RMLIMTC0007g/test_RMLTC0007g_DICT.py
+-rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-in-memory/json_dictionary/RMLIMTC0007h/mapping.ttl
+-rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-in-memory/json_dictionary/RMLIMTC0007h/test_RMLTC0007h_DICT.py
+-rw-r--r--   0        0        0     1401 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-in-memory/json_dictionary/RMLIMTC0008a/mapping.ttl
+-rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-in-memory/json_dictionary/RMLIMTC0008a/output.nq
+-rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-in-memory/json_dictionary/RMLIMTC0008a/test_RMLTC0008a_DICT.py
+-rw-r--r--   0        0        0     1909 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-in-memory/json_dictionary/RMLIMTC0008b/mapping.ttl
+-rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-in-memory/json_dictionary/RMLIMTC0008b/output.nq
+-rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-in-memory/json_dictionary/RMLIMTC0008b/test_RMLTC0008b_DICT.py
+-rw-r--r--   0        0        0     1045 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-in-memory/json_dictionary/RMLIMTC0008c/mapping.ttl
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-in-memory/json_dictionary/RMLIMTC0008c/output.nq
+-rw-r--r--   0        0        0      857 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-in-memory/json_dictionary/RMLIMTC0008c/test_RMLTC0008c_DICT.py
+-rw-r--r--   0        0        0     1843 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-in-memory/json_dictionary/RMLIMTC0009a/mapping.ttl
+-rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-in-memory/json_dictionary/RMLIMTC0009a/output.nq
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-in-memory/json_dictionary/RMLIMTC0009a/test_RMLTC0009a_DICT.py
+-rw-r--r--   0        0        0     2153 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-in-memory/json_dictionary/RMLIMTC0009b/mapping.ttl
+-rw-r--r--   0        0        0     1198 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-in-memory/json_dictionary/RMLIMTC0009b/output.nq
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-in-memory/json_dictionary/RMLIMTC0009b/test_RMLTC0009b_DICT.py
+-rw-r--r--   0        0        0     1011 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-in-memory/json_dictionary/RMLIMTC0010a/mapping.ttl
+-rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-in-memory/json_dictionary/RMLIMTC0010a/output.nq
+-rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-in-memory/json_dictionary/RMLIMTC0010a/test_RMLTC0010a_DICT.py
+-rw-r--r--   0        0        0     1018 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-in-memory/json_dictionary/RMLIMTC0010b/mapping.ttl
+-rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-in-memory/json_dictionary/RMLIMTC0010b/output.nq
+-rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-in-memory/json_dictionary/RMLIMTC0010b/test_RMLTC0010b_DICT.py
+-rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-in-memory/json_dictionary/RMLIMTC0010c/mapping.ttl
+-rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-in-memory/json_dictionary/RMLIMTC0010c/output.nq
+-rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-in-memory/json_dictionary/RMLIMTC0010c/test_RMLTC0010c_DICT.py
+-rw-r--r--   0        0        0     2261 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-in-memory/json_dictionary/RMLIMTC0011b/mapping.ttl
+-rw-r--r--   0        0        0     1229 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-in-memory/json_dictionary/RMLIMTC0011b/output.nq
+-rw-r--r--   0        0        0     1391 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-in-memory/json_dictionary/RMLIMTC0011b/test_RMLTC0011b_DICT.py
+-rw-r--r--   0        0        0     1146 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-in-memory/json_dictionary/RMLIMTC0012a/mapping.ttl
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-in-memory/json_dictionary/RMLIMTC0012a/output.nq
+-rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-in-memory/json_dictionary/RMLIMTC0012a/test_RMLTC0012a_DICT.py
+-rw-r--r--   0        0        0     1553 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-in-memory/json_dictionary/RMLIMTC0012b/mapping.ttl
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-in-memory/json_dictionary/RMLIMTC0012b/output.nq
+-rw-r--r--   0        0        0     1129 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-in-memory/json_dictionary/RMLIMTC0012b/test_RMLTC0012b_DICT.py
+-rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-in-memory/json_dictionary/RMLIMTC0012c/mapping.ttl
+-rw-r--r--   0        0        0      865 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-in-memory/json_dictionary/RMLIMTC0012c/test_RMLTC0012c_DICT.py
+-rw-r--r--   0        0        0     1235 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-in-memory/json_dictionary/RMLIMTC0012d/mapping.ttl
+-rw-r--r--   0        0        0      865 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-in-memory/json_dictionary/RMLIMTC0012d/test_RMLTC0012d_DICT.py
+-rw-r--r--   0        0        0      997 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-in-memory/json_dictionary/RMLIMTC0013a/mapping.ttl
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-in-memory/json_dictionary/RMLIMTC0013a/output.nq
+-rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-in-memory/json_dictionary/RMLIMTC0013a/test_RMLTC0013a_DICT.py
+-rw-r--r--   0        0        0     1577 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-in-memory/json_dictionary/RMLIMTC0015a/mapping.ttl
+-rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-in-memory/json_dictionary/RMLIMTC0015a/output.nq
+-rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-in-memory/json_dictionary/RMLIMTC0015a/test_RMLTC0015a_DICT.py
+-rw-r--r--   0        0        0     1574 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-in-memory/json_dictionary/RMLIMTC0015b/mapping.ttl
+-rw-r--r--   0        0        0      991 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-in-memory/json_dictionary/RMLIMTC0015b/test_RMLTC0015b_DICT.py
+-rw-r--r--   0        0        0      984 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-in-memory/pandas_dataframe/RMLIMTC0000/mapping.ttl
+-rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-in-memory/pandas_dataframe/RMLIMTC0000/output.nq
+-rw-r--r--   0        0        0      790 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-in-memory/pandas_dataframe/RMLIMTC0000/test_RMLIMTC0000_DF.py
+-rw-r--r--   0        0        0      983 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-in-memory/pandas_dataframe/RMLIMTC0001a/mapping.ttl
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-in-memory/pandas_dataframe/RMLIMTC0001a/output.nq
+-rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-in-memory/pandas_dataframe/RMLIMTC0001a/student.csv
+-rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-in-memory/pandas_dataframe/RMLIMTC0001a/test_RMLTC0001a_DF.py
+-rw-r--r--   0        0        0      994 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-in-memory/pandas_dataframe/RMLIMTC0001b/mapping.ttl
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-in-memory/pandas_dataframe/RMLIMTC0001b/output.nq
+-rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-in-memory/pandas_dataframe/RMLIMTC0001b/test_RMLIMTC0001b_DF.py
+-rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-in-memory/pandas_dataframe/RMLIMTC0002a/mapping.ttl
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-in-memory/pandas_dataframe/RMLIMTC0002a/output.nq
+-rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-in-memory/pandas_dataframe/RMLIMTC0002a/test_RMLIMTC0002a_DF.py
+-rw-r--r--   0        0        0      988 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-in-memory/pandas_dataframe/RMLIMTC0002b/mapping.ttl
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-in-memory/pandas_dataframe/RMLIMTC0002b/output.nq
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-in-memory/pandas_dataframe/RMLIMTC0002b/test_RMLIMTC0002b_DF.py
+-rw-r--r--   0        0        0      973 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-in-memory/pandas_dataframe/RMLIMTC0002c/mapping.ttl
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-in-memory/pandas_dataframe/RMLIMTC0002c/output.nq
+-rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-in-memory/pandas_dataframe/RMLIMTC0002c/test_RMLIMTC0002c_DF.py
+-rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-in-memory/pandas_dataframe/RMLIMTC0002e/mapping.ttl
+-rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-in-memory/pandas_dataframe/RMLIMTC0002e/test_RMLIMTC0002e_DF.py
+-rw-r--r--   0        0        0     1034 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-in-memory/pandas_dataframe/RMLIMTC0003c/mapping.ttl
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-in-memory/pandas_dataframe/RMLIMTC0003c/output.nq
+-rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-in-memory/pandas_dataframe/RMLIMTC0003c/test_RMLIMTC0003c_DF.py
+-rw-r--r--   0        0        0     1552 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-in-memory/pandas_dataframe/RMLIMTC0004a/mapping.ttl
+-rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-in-memory/pandas_dataframe/RMLIMTC0004a/output.nq
+-rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-in-memory/pandas_dataframe/RMLIMTC0004a/test_RMLIMTC0004a_DF.py
+-rw-r--r--   0        0        0     1005 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-in-memory/pandas_dataframe/RMLIMTC0004b/mapping.ttl
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-in-memory/pandas_dataframe/RMLIMTC0004b/output.nq
+-rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-in-memory/pandas_dataframe/RMLIMTC0004b/test_RMLIMTC0004b_DF.py
+-rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-in-memory/pandas_dataframe/RMLIMTC0005a/mapping.ttl
+-rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-in-memory/pandas_dataframe/RMLIMTC0005a/output.nq
+-rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-in-memory/pandas_dataframe/RMLIMTC0005a/test_RMLIMTC0005a_DF.py
+-rw-r--r--   0        0        0     1056 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-in-memory/pandas_dataframe/RMLIMTC0006a/mapping.ttl
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-in-memory/pandas_dataframe/RMLIMTC0006a/output.nq
+-rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-in-memory/pandas_dataframe/RMLIMTC0006a/test_RMLIMTC0006a_DF.py
+-rw-r--r--   0        0        0     1034 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-in-memory/pandas_dataframe/RMLIMTC0007a/mapping.ttl
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-in-memory/pandas_dataframe/RMLIMTC0007a/output.nq
+-rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-in-memory/pandas_dataframe/RMLIMTC0007a/test_RMLIMTC0007a_DF.py
+-rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-in-memory/pandas_dataframe/RMLIMTC0007b/mapping.ttl
+-rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-in-memory/pandas_dataframe/RMLIMTC0007b/output.nq
+-rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-in-memory/pandas_dataframe/RMLIMTC0007b/test_RMLIMTC0007b_DF.py
+-rw-r--r--   0        0        0     1131 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-in-memory/pandas_dataframe/RMLIMTC0007c/mapping.ttl
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-in-memory/pandas_dataframe/RMLIMTC0007c/output.nq
+-rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-in-memory/pandas_dataframe/RMLIMTC0007c/test_RMLIMTC0007c_DF.py
+-rw-r--r--   0        0        0     1322 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-in-memory/pandas_dataframe/RMLIMTC0007d/mapping.ttl
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-in-memory/pandas_dataframe/RMLIMTC0007d/output.nq
+-rw-r--r--   0        0        0      835 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-in-memory/pandas_dataframe/RMLIMTC0007d/test_RMLTC0007d_DF.py
+-rw-r--r--   0        0        0     1151 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-in-memory/pandas_dataframe/RMLIMTC0007e/mapping.ttl
+-rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-in-memory/pandas_dataframe/RMLIMTC0007e/output.nq
+-rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-in-memory/pandas_dataframe/RMLIMTC0007e/test_RMLIMTC0007e_DF.py
+-rw-r--r--   0        0        0     1269 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-in-memory/pandas_dataframe/RMLIMTC0007f/mapping.ttl
+-rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-in-memory/pandas_dataframe/RMLIMTC0007f/output.nq
+-rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-in-memory/pandas_dataframe/RMLIMTC0007f/test_RMLIMTC0007f_DF.py
+-rw-r--r--   0        0        0     1034 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-in-memory/pandas_dataframe/RMLIMTC0007g/mapping.ttl
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-in-memory/pandas_dataframe/RMLIMTC0007g/output.nq
+-rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-in-memory/pandas_dataframe/RMLIMTC0007g/test_RMLIMTC0007g_DF.py
+-rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-in-memory/pandas_dataframe/RMLIMTC0007h/mapping.ttl
+-rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-in-memory/pandas_dataframe/RMLIMTC0007h/test_RMLIMTC0007h_DF.py
+-rw-r--r--   0        0        0     1416 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-in-memory/pandas_dataframe/RMLIMTC0008a/mapping.ttl
+-rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-in-memory/pandas_dataframe/RMLIMTC0008a/output.nq
+-rw-r--r--   0        0        0      835 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-in-memory/pandas_dataframe/RMLIMTC0008a/test_RMLIMTC0008a_DF.py
+-rw-r--r--   0        0        0     1933 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-in-memory/pandas_dataframe/RMLIMTC0008b/mapping.ttl
+-rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-in-memory/pandas_dataframe/RMLIMTC0008b/output.nq
+-rw-r--r--   0        0        0      835 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-in-memory/pandas_dataframe/RMLIMTC0008b/test_RMLIMTC0008b_DF.py
+-rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-in-memory/pandas_dataframe/RMLIMTC0008c/mapping.ttl
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-in-memory/pandas_dataframe/RMLIMTC0008c/output.nq
+-rw-r--r--   0        0        0      835 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-in-memory/pandas_dataframe/RMLIMTC0008c/test_RMLIMTC0008c_DF.py
+-rw-r--r--   0        0        0     1875 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-in-memory/pandas_dataframe/RMLIMTC0009a/mapping.ttl
+-rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-in-memory/pandas_dataframe/RMLIMTC0009a/output.nq
+-rw-r--r--   0        0        0      925 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-in-memory/pandas_dataframe/RMLIMTC0009a/test_RMLIMTC0009a_DF.py
+-rw-r--r--   0        0        0     2190 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-in-memory/pandas_dataframe/RMLIMTC0009b/mapping.ttl
+-rw-r--r--   0        0        0     1198 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-in-memory/pandas_dataframe/RMLIMTC0009b/output.nq
+-rw-r--r--   0        0        0      925 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-in-memory/pandas_dataframe/RMLIMTC0009b/test_RMLIMTC0009b_DF.py
+-rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-in-memory/pandas_dataframe/RMLIMTC0010a/mapping.ttl
+-rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-in-memory/pandas_dataframe/RMLIMTC0010a/output.nq
+-rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-in-memory/pandas_dataframe/RMLIMTC0010a/test_RMLIMTC0010a_DF.py
+-rw-r--r--   0        0        0     1033 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-in-memory/pandas_dataframe/RMLIMTC0010b/mapping.ttl
+-rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-in-memory/pandas_dataframe/RMLIMTC0010b/output.nq
+-rw-r--r--   0        0        0      930 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-in-memory/pandas_dataframe/RMLIMTC0010b/test_RMLIMTC0010b_DF.py
+-rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-in-memory/pandas_dataframe/RMLIMTC0010c/mapping.ttl
+-rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-in-memory/pandas_dataframe/RMLIMTC0010c/output.nq
+-rw-r--r--   0        0        0      930 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-in-memory/pandas_dataframe/RMLIMTC0010c/test_RMLIMTC0010c_DF.py
+-rw-r--r--   0        0        0     2315 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-in-memory/pandas_dataframe/RMLIMTC0011b/mapping.ttl
+-rw-r--r--   0        0        0     1229 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-in-memory/pandas_dataframe/RMLIMTC0011b/output.nq
+-rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-in-memory/pandas_dataframe/RMLIMTC0011b/test_RMLIMTC0011b_DF.py
+-rw-r--r--   0        0        0     1162 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-in-memory/pandas_dataframe/RMLIMTC0012a/mapping.ttl
+-rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-in-memory/pandas_dataframe/RMLIMTC0012a/output.nq
+-rw-r--r--   0        0        0      831 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-in-memory/pandas_dataframe/RMLIMTC0012a/test_RMLIMTC0012a_DF.py
+-rw-r--r--   0        0        0     1589 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-in-memory/pandas_dataframe/RMLIMTC0012b/mapping.ttl
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-in-memory/pandas_dataframe/RMLIMTC0012b/output.nq
+-rw-r--r--   0        0        0      987 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-in-memory/pandas_dataframe/RMLIMTC0012b/test_RMLIMTC0012b_DF.py
+-rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-in-memory/pandas_dataframe/RMLIMTC0012c/mapping.ttl
+-rw-r--r--   0        0        0      796 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-in-memory/pandas_dataframe/RMLIMTC0012c/test_RMLIMTC0012c_DF.py
+-rw-r--r--   0        0        0     1252 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-in-memory/pandas_dataframe/RMLIMTC0012d/mapping.ttl
+-rw-r--r--   0        0        0      797 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-in-memory/pandas_dataframe/RMLIMTC0012d/test_RMLIMTC0012d_DF.py
+-rw-r--r--   0        0        0     1607 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-in-memory/pandas_dataframe/RMLIMTC0015a/mapping.ttl
+-rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-in-memory/pandas_dataframe/RMLIMTC0015a/output.nq
+-rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-in-memory/pandas_dataframe/RMLIMTC0015a/test_RMLIMTC0015a_DF.py
+-rw-r--r--   0        0        0     1604 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-in-memory/pandas_dataframe/RMLIMTC0015b/mapping.ttl
+-rw-r--r--   0        0        0      922 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-in-memory/pandas_dataframe/RMLIMTC0015b/test_RMLIMTC0015b_DF.py
+-rw-r--r--   0        0        0     1662 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-in-memory/pandas_dataframe/triples_map_without_pom/mapping.ttl
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-in-memory/pandas_dataframe/triples_map_without_pom/output.nq
+-rw-r--r--   0        0        0      937 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-in-memory/pandas_dataframe/triples_map_without_pom/test_triples_map_without_pom_DF.py
+-rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-star/RMLSTARTC001a/data.csv
+-rw-r--r--   0        0        0     1041 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-star/RMLSTARTC001a/mapping.ttl
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-star/RMLSTARTC001a/output.nq
+-rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-star/RMLSTARTC001a/test_RMLSTARTC001a_CSV.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-star/RMLSTARTC001b/data1.csv
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-star/RMLSTARTC001b/data2.csv
+-rw-r--r--   0        0        0     1146 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-star/RMLSTARTC001b/mapping.ttl
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-star/RMLSTARTC001b/output.nq
+-rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-star/RMLSTARTC001b/test_RMLSTARTC001b_CSV.py
+-rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-star/RMLSTARTC002a/data.csv
+-rw-r--r--   0        0        0     1132 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-star/RMLSTARTC002a/mapping.ttl
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-star/RMLSTARTC002a/output.nq
+-rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-star/RMLSTARTC002a/test_RMLSTARTC002a_CSV.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-star/RMLSTARTC002b/data1.csv
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-star/RMLSTARTC002b/data2.csv
+-rw-r--r--   0        0        0     1238 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-star/RMLSTARTC002b/mapping.ttl
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-star/RMLSTARTC002b/output.nq
+-rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-star/RMLSTARTC002b/test_RMLSTARTC002b_CSV.py
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-star/RMLSTARTC003a/data.csv
+-rw-r--r--   0        0        0     1478 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-star/RMLSTARTC003a/mapping.ttl
+-rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-star/RMLSTARTC003a/output.nq
+-rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-star/RMLSTARTC003a/test_RMLSTARTC003a_CSV.py
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-star/RMLSTARTC003b/data1.csv
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-star/RMLSTARTC003b/data2.csv
+-rw-r--r--   0        0        0     1585 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-star/RMLSTARTC003b/mapping.ttl
+-rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-star/RMLSTARTC003b/output.nq
+-rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-star/RMLSTARTC003b/test_RMLSTARTC003b_CSV.py
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-star/RMLSTARTC004a/data.csv
+-rw-r--r--   0        0        0     1455 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-star/RMLSTARTC004a/mapping.ttl
+-rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-star/RMLSTARTC004a/output.nq
+-rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-star/RMLSTARTC004a/test_RMLSTARTC004a_CSV.py
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-star/RMLSTARTC004b/data1.csv
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-star/RMLSTARTC004b/data2.csv
+-rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-star/RMLSTARTC004b/mapping.ttl
+-rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-star/RMLSTARTC004b/output.nq
+-rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-star/RMLSTARTC004b/test_RMLSTARTC004b_CSV.py
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-star/RMLSTARTC005a/data.csv
+-rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-star/RMLSTARTC005a/mapping.ttl
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-star/RMLSTARTC005a/output.nq
+-rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-star/RMLSTARTC005a/test_RMLSTARTC005a_CSV.py
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-star/RMLSTARTC005b/data1.csv
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-star/RMLSTARTC005b/data2.csv
+-rw-r--r--   0        0        0     1223 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-star/RMLSTARTC005b/mapping.ttl
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-star/RMLSTARTC005b/output.nq
+-rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-star/RMLSTARTC005b/test_RMLSTARTC005b_CSV.py
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-star/RMLSTARTC006a/data.csv
+-rw-r--r--   0        0        0     1201 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-star/RMLSTARTC006a/mapping.ttl
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-star/RMLSTARTC006a/output.nq
+-rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-star/RMLSTARTC006a/test_RMLSTARTC006a_CSV.py
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-star/RMLSTARTC006b/data1.csv
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-star/RMLSTARTC006b/data2.csv
+-rw-r--r--   0        0        0     1323 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-star/RMLSTARTC006b/mapping.ttl
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-star/RMLSTARTC006b/output.nq
+-rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-star/RMLSTARTC006b/test_RMLSTARTC006b_CSV.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-star/RMLSTARTC007a/data.csv
+-rw-r--r--   0        0        0     1485 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-star/RMLSTARTC007a/mapping.ttl
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-star/RMLSTARTC007a/output.nq
+-rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-star/RMLSTARTC007a/test_RMLSTARTC007a_CSV.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-star/RMLSTARTC007b/data1.csv
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-star/RMLSTARTC007b/data2.csv
+-rw-r--r--   0        0        0     1609 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-star/RMLSTARTC007b/mapping.ttl
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-star/RMLSTARTC007b/output.nq
+-rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-star/RMLSTARTC007b/test_RMLSTARTC007b_CSV.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-star/RMLSTARTC008a/data.csv
+-rw-r--r--   0        0        0     3089 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-star/RMLSTARTC008a/mapping.ttl
+-rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-star/RMLSTARTC008a/output.nq
+-rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-star/RMLSTARTC008a/test_RMLSTARTC008a_CSV.py
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-star/RMLSTARTC008b/data1.csv
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-star/RMLSTARTC008b/data2.csv
+-rw-r--r--   0        0        0     3225 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-star/RMLSTARTC008b/mapping.ttl
+-rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-star/RMLSTARTC008b/output.nq
+-rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rml-star/RMLSTARTC008b/test_RMLSTARTC008b_CSV.py
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rmltv/RMLTVTC0002d/mapping.ttl
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rmltv/RMLTVTC0002d/output.nq
+-rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rmltv/RMLTVTC0002d/student.csv
+-rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rmltv/RMLTVTC0002d/test_RMLTVTC0002d_CSV.py
+-rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rmltv/RMLTVTC0002g/mapping.ttl
+-rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rmltv/RMLTVTC0002g/student.csv
+-rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rmltv/RMLTVTC0002g/test_RMLTVTC0002g_CSV.py
+-rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rmltv/RMLTVTC0002h/mapping.ttl
+-rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rmltv/RMLTVTC0002h/student.csv
+-rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rmltv/RMLTVTC0002h/test_RMLTVTC0002h_CSV.py
+-rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rmltv/RMLTVTC0002i/mapping.ttl
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rmltv/RMLTVTC0002i/output.nq
+-rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rmltv/RMLTVTC0002i/student.csv
+-rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rmltv/RMLTVTC0002i/test_RMLTVTC0002i_CSV.py
+-rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rmltv/RMLTVTC0002j/mapping.ttl
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rmltv/RMLTVTC0002j/output.nq
+-rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rmltv/RMLTVTC0002j/student.csv
+-rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rmltv/RMLTVTC0002j/test_RMLTVTC0002j_CSV.py
+-rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rmltv/RMLTVTC0003b/mapping.ttl
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rmltv/RMLTVTC0003b/output.nq
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rmltv/RMLTVTC0003b/student.csv
+-rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rmltv/RMLTVTC0003b/test_RMLTVTC0003b_CSV.py
+-rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rmltv/RMLTVTC0009c/mapping.ttl
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rmltv/RMLTVTC0009c/output.nq
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rmltv/RMLTVTC0009c/sport.csv
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rmltv/RMLTVTC0009c/student.csv
+-rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rmltv/RMLTVTC0009c/test_RMLTVTC0009c_CSV.py
+-rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rmltv/RMLTVTC0009d/mapping.ttl
+-rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rmltv/RMLTVTC0009d/output.nq
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rmltv/RMLTVTC0009d/sport.csv
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rmltv/RMLTVTC0009d/student.csv
+-rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rmltv/RMLTVTC0009d/test_RMLTVTC0009d_CSV.py
+-rw-r--r--   0        0        0     1753 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rmltv/RMLTVTC0011a/mapping.ttl
+-rw-r--r--   0        0        0     1525 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rmltv/RMLTVTC0011a/output.nq
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rmltv/RMLTVTC0011a/sport.csv
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rmltv/RMLTVTC0011a/student.csv
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rmltv/RMLTVTC0011a/student_sport.csv
+-rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rmltv/RMLTVTC0011a/test_RMLTVTC0011a_CSV.py
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rmltv/RMLTVTC0014d/dept.csv
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rmltv/RMLTVTC0014d/emp.csv
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rmltv/RMLTVTC0014d/likes.csv
+-rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rmltv/RMLTVTC0014d/mapping.ttl
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rmltv/RMLTVTC0014d/output.nq
+-rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rmltv/RMLTVTC0014d/test_RMLTVTC0014d_CSV.py
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rmltv/RMLTVTC0015a/country.csv
+-rw-r--r--   0        0        0     1012 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rmltv/RMLTVTC0015a/mapping.ttl
+-rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rmltv/RMLTVTC0015a/output.nq
+-rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rmltv/RMLTVTC0015a/test_RMLTVTC0015a_CSV.py
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rmltv/RMLTVTC0015b/country.csv
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rmltv/RMLTVTC0015b/mapping.ttl
+-rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rmltv/RMLTVTC0015b/test_RMLTVTC0015b_CSV.py
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rmltv/RMLTVTC0019a/employee.csv
+-rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rmltv/RMLTVTC0019a/mapping.ttl
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rmltv/RMLTVTC0019a/output.nq
+-rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rmltv/RMLTVTC0019a/test_RMLTVTC0019a_CSV.py
+-rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rmltv/RMLTVTC0026a/mapping.ttl
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rmltv/RMLTVTC0026a/mixed_content_list.csv
+-rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rmltv/RMLTVTC0026a/output.nq
+-rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rmltv/RMLTVTC0026a/test_RMLTVTC0026a_CSV.py
+-rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rmltv/RMLTVTC0027a/mapping.ttl
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rmltv/RMLTVTC0027a/mixed_content_json.csv
+-rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rmltv/RMLTVTC0027a/output.nq
+-rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rmltv/RMLTVTC0027a/test_RMLTVTC0027a_CSV.py
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rmltv/RMLTVTC0028a/aka_title.csv
+-rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rmltv/RMLTVTC0028a/mapping.ttl
+-rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rmltv/RMLTVTC0028a/output.nq
+-rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rmltv/RMLTVTC0028a/test_RMLTVTC0028a_CSV.py
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rmltv/RMLTVTC0028a/title.csv
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rmltv/RMLTVTC0029a/department.csv
+-rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rmltv/RMLTVTC0029a/faculty.csv
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rmltv/RMLTVTC0029a/graduatecourse.csv
+-rw-r--r--   0        0        0      965 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rmltv/RMLTVTC0029a/mapping.ttl
+-rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rmltv/RMLTVTC0029a/output.nq
+-rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/test/rmltv/RMLTVTC0029a/test_RMLTVTC0029a_CSV.py
+-rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/LICENSE
+-rw-r--r--   0        0        0     6860 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/README.md
+-rw-r--r--   0        0        0     2660 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/pyproject.toml
+-rw-r--r--   0        0        0    10290 2020-02-02 00:00:00.000000 morph_kgc-2.5.1/PKG-INFO
```

### Comparing `morph_kgc-2.5.0/.zenodo.json` & `morph_kgc-2.5.1/.zenodo.json`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/CITATION.cff` & `morph_kgc-2.5.1/CITATION.cff`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/CODE_OF_CONDUCT.md` & `morph_kgc-2.5.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/CONTRIBUTING.md` & `morph_kgc-2.5.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/mkdocs.yml` & `morph_kgc-2.5.1/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/.github/ISSUE_TEMPLATE/documentation-improvement.md` & `morph_kgc-2.5.1/.github/ISSUE_TEMPLATE/documentation-improvement.md`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/.github/ISSUE_TEMPLATE/feature-request.md` & `morph_kgc-2.5.1/.github/ISSUE_TEMPLATE/feature-request.md`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/.github/ISSUE_TEMPLATE/installation-issue.md` & `morph_kgc-2.5.1/.github/ISSUE_TEMPLATE/installation-issue.md`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/.github/workflows/ci.yml` & `morph_kgc-2.5.1/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/.github/workflows/pypi-publish.yml` & `morph_kgc-2.5.1/.github/workflows/pypi-publish.yml`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/docs/documentation.md` & `morph_kgc-2.5.1/docs/documentation.md`

 * *Files 1% similar despite different names*

```diff
@@ -187,18 +187,18 @@
 #### Relational Databases
 
 The properties to be specified for **relational databases** are listed below. All of the properties are **required**.
 
 |<div style="width:100px">Property</div>|Description|<div style="width:475px">Values</div>|
 |-------|-------|-------|
 |**`mappings`**|Specifies the mapping file(s) or URL(s) for the relational database.|**[REQUIRED]**<br>**Valid:**<br>- The path to a mapping file or URL.<br>- The paths to multiple mapping files or URLs separated by commas.<br>- The path to a directory containing all the mapping files.|
-|**`db_url`**|It is a URL that configures the database engine (username, password, hostname, database name). See **[here](https://docs.sqlalchemy.org/en/14/core/engines.html#database-urls)** how to create the database URLs.|**[REQUIRED]**<br>**Example:** _dialect+driver://username:password@host:port/db_name_|
+|**`db_url`**|It is a URL that configures the database engine (username, password, hostname, database name). See **[here](https://docs.sqlalchemy.org/en/20/core/engines.html#database-urls)** how to create the database URLs.|**[REQUIRED]**<br>**Example:** _dialect+driver://username:password@host:port/db_name_|
 |**`connect_args`**|A dictionary string of options for [SQLAlchemy](https://www.sqlalchemy.org/). See [here](https://docs.sqlalchemy.org/en/20/core/engines.html#sqlalchemy.create_engine.params.connect_args) the [SQLAlchemy](https://www.sqlalchemy.org/) documentation.|**Example:** _{"http_path": "<cluster_http_path>"}_|
 
-Example **`db_url`** values (see **[here](https://docs.sqlalchemy.org/en/14/core/engines.html#database-urls)** all the information):
+Example **`db_url`** values (see **[here](https://docs.sqlalchemy.org/en/20/core/engines.html#database-urls)** all the information):
 
 - **[MySQL](https://www.mysql.com/)**: _mysql+pymysql://username:password@host:port/db_name_
 - **[PostgreSQL](https://www.postgresql.org/)**: _postgresql+psycopg2://username:password@host:port/db_name_
 - **[Oracle](https://www.oracle.com/database/)**: _oracle+cx_oracle://username:password@host:port/db_name_
 - **[Microsoft SQL Server](https://www.microsoft.com/sql-server)**: _mssql+pymssql://username:password@host:port/db_name_
 - **[MariaDB](https://mariadb.org/)**: _mariadb+pymysql://username:password@host:port/db_name_
 - **[SQLite](https://www.sqlite.org)**: _sqlite:///db_path/db_name.db_
```

### Comparing `morph_kgc-2.5.0/docs/faq.md` & `morph_kgc-2.5.1/docs/faq.md`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/docs/index.md` & `morph_kgc-2.5.1/docs/index.md`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/docs/research.md` & `morph_kgc-2.5.1/docs/research.md`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/docs/why-morph-kgc.md` & `morph_kgc-2.5.1/docs/why-morph-kgc.md`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/docs/assets/BASF.png` & `morph_kgc-2.5.1/docs/assets/BASF.png`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/docs/assets/BASF.tif` & `morph_kgc-2.5.1/docs/assets/BASF.tif`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/docs/assets/datos40.png` & `morph_kgc-2.5.1/docs/assets/datos40.png`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/docs/assets/entente.png` & `morph_kgc-2.5.1/docs/assets/entente.png`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/docs/assets/knowledgespaces.png` & `morph_kgc-2.5.1/docs/assets/knowledgespaces.png`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/docs/assets/logo-oeg.png` & `morph_kgc-2.5.1/docs/assets/logo-oeg.png`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/docs/assets/logo-upm.png` & `morph_kgc-2.5.1/docs/assets/logo-upm.png`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/docs/assets/logo.png` & `morph_kgc-2.5.1/docs/assets/logo.png`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/docs/assets/sigtrans.png` & `morph_kgc-2.5.1/docs/assets/sigtrans.png`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/examples/README.md` & `morph_kgc-2.5.1/examples/README.md`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/examples/configuration-file/default_config.ini` & `morph_kgc-2.5.1/examples/configuration-file/default_config.ini`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/examples/csv/mapping.csv.ttl` & `morph_kgc-2.5.1/examples/csv/mapping.csv.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/examples/csv/data/FREQUENCIES.csv` & `morph_kgc-2.5.1/examples/csv/data/FREQUENCIES.csv`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/examples/csv/data/ROUTES.csv` & `morph_kgc-2.5.1/examples/csv/data/ROUTES.csv`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/examples/csv/data/SHAPES.csv` & `morph_kgc-2.5.1/examples/csv/data/SHAPES.csv`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/examples/csv/data/STOPS.csv` & `morph_kgc-2.5.1/examples/csv/data/STOPS.csv`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/examples/csv/data/STOP_TIMES.csv` & `morph_kgc-2.5.1/examples/csv/data/STOP_TIMES.csv`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/examples/csv/data/TRIPS.csv` & `morph_kgc-2.5.1/examples/csv/data/TRIPS.csv`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/examples/dataframe/kg_generation.py` & `morph_kgc-2.5.1/examples/dataframe/kg_generation.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/examples/dataframe/mapping_rml.ttl` & `morph_kgc-2.5.1/examples/dataframe/mapping_rml.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/examples/dict/kg_generation.py` & `morph_kgc-2.5.1/examples/dict/kg_generation.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/examples/dict/mapping_rml.ttl` & `morph_kgc-2.5.1/examples/dict/mapping_rml.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/examples/json/data.json` & `morph_kgc-2.5.1/examples/json/data.json`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/examples/json/mapping.json.ttl` & `morph_kgc-2.5.1/examples/json/mapping.json.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/examples/json/mapping.json.yaml` & `morph_kgc-2.5.1/examples/json/mapping.json.yaml`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/examples/rdb/gtfs-rdb.r2rml.ttl` & `morph_kgc-2.5.1/examples/rdb/gtfs-rdb.r2rml.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/examples/tutorial/Morph-KGC.ipynb` & `morph_kgc-2.5.1/examples/tutorial/Morph-KGC.ipynb`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/examples/tutorial/mapping.gtfs.ttl` & `morph_kgc-2.5.1/examples/tutorial/mapping.gtfs.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/examples/tutorial/mapping.somef.ttl` & `morph_kgc-2.5.1/examples/tutorial/mapping.somef.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/examples/tutorial/oeg-upm_morph-kgc.json` & `morph_kgc-2.5.1/examples/tutorial/oeg-upm_morph-kgc.json`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/examples/xml/data.xml` & `morph_kgc-2.5.1/examples/xml/data.xml`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/examples/xml/mapping.xml.yaml` & `morph_kgc-2.5.1/examples/xml/mapping.xml.yaml`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/examples/xml/mappingOA.xml.ttl` & `morph_kgc-2.5.1/examples/xml/mappingOA.xml.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/src/morph_kgc/__init__.py` & `morph_kgc-2.5.1/src/morph_kgc/__init__.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/src/morph_kgc/__main__.py` & `morph_kgc-2.5.1/src/morph_kgc/__main__.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/src/morph_kgc/args_parser.py` & `morph_kgc-2.5.1/src/morph_kgc/args_parser.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/src/morph_kgc/config.py` & `morph_kgc-2.5.1/src/morph_kgc/config.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/src/morph_kgc/constants.py` & `morph_kgc-2.5.1/src/morph_kgc/constants.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,14 +37,15 @@
 RDB = 'RDB'
 MYSQL = 'MYSQL'
 MARIADB = 'MARIADB'
 MSSQL = 'MSSQL'
 ORACLE = 'ORACLE'
 POSTGRESQL = 'POSTGRESQL'
 SQLITE = 'SQLITE'
+DATABRICKS = 'DATABRICKS'
 
 # in-memory data
 PYTHON_SOURCE = 'PYTHON_SOURCE'
 DATAFRAME = 'DATAFRAME'
 DICTIONARY = 'DICTIONARY'
 JSON_STRING = 'JSON_STRING'
```

### Comparing `morph_kgc-2.5.0/src/morph_kgc/materializer.py` & `morph_kgc-2.5.1/src/morph_kgc/materializer.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/src/morph_kgc/utils.py` & `morph_kgc-2.5.1/src/morph_kgc/utils.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/src/morph_kgc/data_source/data_file.py` & `morph_kgc-2.5.1/src/morph_kgc/data_source/data_file.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/src/morph_kgc/data_source/python_data.py` & `morph_kgc-2.5.1/src/morph_kgc/data_source/python_data.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/src/morph_kgc/data_source/relational_database.py` & `morph_kgc-2.5.1/src/morph_kgc/data_source/relational_database.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,14 +71,17 @@
         num_enclosing_char = 0
         for char in sql_query:
             if char == '`':
                 dialect_sql_query = dialect_sql_query + square_brackets[num_enclosing_char % 2]
                 num_enclosing_char += 1
             else:
                 dialect_sql_query = dialect_sql_query + char
+    elif db_dialect == DATABRICKS:
+        # remove all backticks
+        dialect_sql_query = sql_query.replace('`', '')
     else:
         # replace backticks with double quotes
         dialect_sql_query = sql_query.replace('`', '"')
 
     return dialect_sql_query
```

### Comparing `morph_kgc-2.5.0/src/morph_kgc/fno/built_in_functions.py` & `morph_kgc-2.5.1/src/morph_kgc/fno/built_in_functions.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/src/morph_kgc/fno/fno_executer.py` & `morph_kgc-2.5.1/src/morph_kgc/fno/fno_executer.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/src/morph_kgc/mapping/mapping_constants.py` & `morph_kgc-2.5.1/src/morph_kgc/mapping/mapping_constants.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/src/morph_kgc/mapping/mapping_parser.py` & `morph_kgc-2.5.1/src/morph_kgc/mapping/mapping_parser.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/src/morph_kgc/mapping/mapping_partitioner.py` & `morph_kgc-2.5.1/src/morph_kgc/mapping/mapping_partitioner.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/fno/RMLFNOTC0000-CSV/mapping.ttl` & `morph_kgc-2.5.1/test/fno/RMLFNOTC0000-CSV/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/fno/RMLFNOTC0000-CSV/test_RMLFNOTC0000-CSV.py` & `morph_kgc-2.5.1/test/fno/RMLFNOTC0000-CSV/test_RMLFNOTC0000-CSV.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/fno/RMLFNOTC0001-CSV/mapping.ttl` & `morph_kgc-2.5.1/test/fno/RMLFNOTC0001-CSV/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/fno/RMLFNOTC0001-CSV/test_RMLFNOTC0001-CSV.py` & `morph_kgc-2.5.1/test/fno/RMLFNOTC0001-CSV/test_RMLFNOTC0001-CSV.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/fno/RMLFNOTC0002-CSV/mapping.ttl` & `morph_kgc-2.5.1/test/fno/RMLFNOTC0002-CSV/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/fno/RMLFNOTC0002-CSV/test_RMLFNOTC0002-CSV.py` & `morph_kgc-2.5.1/test/fno/RMLFNOTC0002-CSV/test_RMLFNOTC0002-CSV.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/fno/RMLFNOTC0003-CSV/mapping.ttl` & `morph_kgc-2.5.1/test/fno/RMLFNOTC0003-CSV/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/fno/RMLFNOTC0003-CSV/test_RMLFNOTC0003-CSV.py` & `morph_kgc-2.5.1/test/fno/RMLFNOTC0003-CSV/test_RMLFNOTC0003-CSV.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/fno/RMLFNOTC0004-CSV/mapping.ttl` & `morph_kgc-2.5.1/test/fno/RMLFNOTC0004-CSV/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/fno/RMLFNOTC0004-CSV/test_RMLFNOTC0004-CSV.py` & `morph_kgc-2.5.1/test/fno/RMLFNOTC0004-CSV/test_RMLFNOTC0004-CSV.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/fno/RMLFNOTC0005-CSV/mapping.ttl` & `morph_kgc-2.5.1/test/fno/RMLFNOTC0005-CSV/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/fno/RMLFNOTC0005-CSV/test_RMLFNOTC0005-CSV.py` & `morph_kgc-2.5.1/test/fno/RMLFNOTC0005-CSV/test_RMLFNOTC0005-CSV.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/fno/RMLFNOTC0006-CSV/mapping.ttl` & `morph_kgc-2.5.1/test/fno/RMLFNOTC0006-CSV/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/fno/RMLFNOTC0006-CSV/test_RMLFNOTC0006-CSV.py` & `morph_kgc-2.5.1/test/fno/RMLFNOTC0006-CSV/test_RMLFNOTC0006-CSV.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/fno/RMLFNOTC0008-CSV/mapping.ttl` & `morph_kgc-2.5.1/test/fno/RMLFNOTC0008-CSV/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/fno/RMLFNOTC0008-CSV/test_RMLFNOTC0008-CSV.py` & `morph_kgc-2.5.1/test/fno/RMLFNOTC0008-CSV/test_RMLFNOTC0008-CSV.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/fno/array_get_slice/mapping.ttl` & `morph_kgc-2.5.1/test/fno/array_get_slice/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/fno/array_get_slice/test_array_get_slice.py` & `morph_kgc-2.5.1/test/fno/array_get_slice/test_array_get_slice.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/fno/controls_if/mapping.ttl` & `morph_kgc-2.5.1/test/fno/controls_if/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/fno/controls_if/output.nq` & `morph_kgc-2.5.1/test/fno/controls_if/output.nq`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/fno/controls_if/test_controls_if.py` & `morph_kgc-2.5.1/test/fno/controls_if/test_controls_if.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/fno/controls_if_cast/mapping.ttl` & `morph_kgc-2.5.1/test/fno/controls_if_cast/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/fno/controls_if_cast/output.nq` & `morph_kgc-2.5.1/test/fno/controls_if_cast/output.nq`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/fno/controls_if_cast/test_controls_if_cast.py` & `morph_kgc-2.5.1/test/fno/controls_if_cast/test_controls_if_cast.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/fno/date_to_date/mapping.ttl` & `morph_kgc-2.5.1/test/fno/date_to_date/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/fno/date_to_date/test_date_to_date.py` & `morph_kgc-2.5.1/test/fno/date_to_date/test_date_to_date.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/fno/math_round/mapping.ttl` & `morph_kgc-2.5.1/test/fno/math_round/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/fno/math_round/test_math_round.py` & `morph_kgc-2.5.1/test/fno/math_round/test_math_round.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/fno/nested_function/mapping.ttl` & `morph_kgc-2.5.1/test/fno/nested_function/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/fno/nested_function/test_nested_function.py` & `morph_kgc-2.5.1/test/fno/nested_function/test_nested_function.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/fno/split_explode/mapping.ttl` & `morph_kgc-2.5.1/test/fno/split_explode/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/fno/split_explode/test_split_explode.py` & `morph_kgc-2.5.1/test/fno/split_explode/test_split_explode.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/fno/split_explode_null/mapping.ttl` & `morph_kgc-2.5.1/test/fno/split_explode_null/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/fno/split_explode_null/test_split_explode_null.py` & `morph_kgc-2.5.1/test/fno/split_explode_null/test_split_explode_null.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/fno/udf/mapping.ttl` & `morph_kgc-2.5.1/test/fno/udf/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/fno/udf/test_udf.py` & `morph_kgc-2.5.1/test/fno/udf/test_udf.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/issues/issue_118/mapping.ttl` & `morph_kgc-2.5.1/test/issues/issue_118/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/issues/issue_118/premis.xml` & `morph_kgc-2.5.1/test/issues/issue_118/premis.xml`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/issues/issue_118/test_issue_118.py` & `morph_kgc-2.5.1/test/issues/issue_118/test_issue_118.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/issues/issue_124/mapping.ttl` & `morph_kgc-2.5.1/test/issues/issue_124/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/issues/issue_124/output.nq` & `morph_kgc-2.5.1/test/issues/issue_124/output.nq`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/issues/issue_124/test_issue_124.py` & `morph_kgc-2.5.1/test/issues/issue_124/test_issue_124.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/issues/issue_145/mapping.ttl` & `morph_kgc-2.5.1/test/issues/issue_145/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/issues/issue_145/test_issue_145.py` & `morph_kgc-2.5.1/test/issues/issue_145/test_issue_145.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/issues/issue_62/mapping.ttl` & `morph_kgc-2.5.1/test/issues/issue_62/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/issues/issue_62/output.nq` & `morph_kgc-2.5.1/test/issues/issue_62/output.nq`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/issues/issue_62/test_issue_62.py` & `morph_kgc-2.5.1/test/issues/issue_62/test_issue_62.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/issues/issue_67/mapping.ttl` & `morph_kgc-2.5.1/test/issues/issue_67/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/issues/issue_67/test_issue_67.py` & `morph_kgc-2.5.1/test/issues/issue_67/test_issue_67.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/issues/issue_80/mapping.rml` & `morph_kgc-2.5.1/test/issues/issue_80/mapping.rml`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/issues/issue_80/test_issue_80.py` & `morph_kgc-2.5.1/test/issues/issue_80/test_issue_80.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/issues/issue_81/mapping.ttl` & `morph_kgc-2.5.1/test/issues/issue_81/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/issues/issue_81/test_issue_81.py` & `morph_kgc-2.5.1/test/issues/issue_81/test_issue_81.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/r2rml/R2RMLTC0000/resource.db` & `morph_kgc-2.5.1/test/r2rml/R2RMLTC0000/resource.db`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/r2rml/R2RMLTC0000/test_R2RMLTC0000_SQLITE.py` & `morph_kgc-2.5.1/test/r2rml/R2RMLTC0000/test_R2RMLTC0000_SQLITE.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/r2rml/R2RMLTC0001a/resource.db` & `morph_kgc-2.5.1/test/r2rml/R2RMLTC0001a/resource.db`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/r2rml/R2RMLTC0001a/test_R2RMLTC0001a_SQLITE.py` & `morph_kgc-2.5.1/test/r2rml/R2RMLTC0001a/test_R2RMLTC0001a_SQLITE.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/r2rml/R2RMLTC0001b/resource.db` & `morph_kgc-2.5.1/test/r2rml/R2RMLTC0001b/resource.db`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/r2rml/R2RMLTC0001b/test_R2RMLTC0001b_SQLITE.py` & `morph_kgc-2.5.1/test/r2rml/R2RMLTC0001b/test_R2RMLTC0001b_SQLITE.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/r2rml/R2RMLTC0002a/mapping.ttl` & `morph_kgc-2.5.1/test/r2rml/R2RMLTC0002a/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/r2rml/R2RMLTC0002a/resource.db` & `morph_kgc-2.5.1/test/r2rml/R2RMLTC0002a/resource.db`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/r2rml/R2RMLTC0002a/test_R2RMLTC0002a_SQLITE.py` & `morph_kgc-2.5.1/test/r2rml/R2RMLTC0002a/test_R2RMLTC0002a_SQLITE.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/r2rml/R2RMLTC0002b/resource.db` & `morph_kgc-2.5.1/test/r2rml/R2RMLTC0002b/resource.db`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/r2rml/R2RMLTC0002b/test_R2RMLTC0002b_SQLITE.py` & `morph_kgc-2.5.1/test/r2rml/R2RMLTC0002b/test_R2RMLTC0002b_SQLITE.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/r2rml/R2RMLTC0002c/resource.db` & `morph_kgc-2.5.1/test/r2rml/R2RMLTC0002c/resource.db`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/r2rml/R2RMLTC0002c/test_R2RMLTC0002c_SQLITE.py` & `morph_kgc-2.5.1/test/r2rml/R2RMLTC0002c/test_R2RMLTC0002c_SQLITE.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/r2rml/R2RMLTC0002d/mapping.ttl` & `morph_kgc-2.5.1/test/r2rml/R2RMLTC0002d/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/r2rml/R2RMLTC0002d/resource.db` & `morph_kgc-2.5.1/test/r2rml/R2RMLTC0002d/resource.db`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/r2rml/R2RMLTC0002d/test_R2RMLTC0002d_SQLITE.py` & `morph_kgc-2.5.1/test/r2rml/R2RMLTC0002d/test_R2RMLTC0002d_SQLITE.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/r2rml/R2RMLTC0002e/resource.db` & `morph_kgc-2.5.1/test/r2rml/R2RMLTC0002e/resource.db`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/r2rml/R2RMLTC0002e/test_R2RMLTC0002e_SQLITE.py` & `morph_kgc-2.5.1/test/r2rml/R2RMLTC0002e/test_R2RMLTC0002e_SQLITE.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/r2rml/R2RMLTC0002f/mapping.ttl` & `morph_kgc-2.5.1/test/r2rml/R2RMLTC0002f/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/r2rml/R2RMLTC0002f/resource.db` & `morph_kgc-2.5.1/test/r2rml/R2RMLTC0002f/resource.db`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/r2rml/R2RMLTC0002f/test_R2RMLTC0002f_SQLITE.py` & `morph_kgc-2.5.1/test/r2rml/R2RMLTC0002f/test_R2RMLTC0002f_SQLITE.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/r2rml/R2RMLTC0002g/mapping.ttl` & `morph_kgc-2.5.1/test/r2rml/R2RMLTC0002g/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/r2rml/R2RMLTC0002g/resource.db` & `morph_kgc-2.5.1/test/r2rml/R2RMLTC0002g/resource.db`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/r2rml/R2RMLTC0002g/test_R2RMLTC0002g_SQLITE.py` & `morph_kgc-2.5.1/test/r2rml/R2RMLTC0002g/test_R2RMLTC0002g_SQLITE.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/r2rml/R2RMLTC0002h/mapping.ttl` & `morph_kgc-2.5.1/test/r2rml/R2RMLTC0002h/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/r2rml/R2RMLTC0002h/resource.db` & `morph_kgc-2.5.1/test/r2rml/R2RMLTC0002h/resource.db`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/r2rml/R2RMLTC0002h/test_R2RMLTC0002h_SQLITE.py` & `morph_kgc-2.5.1/test/r2rml/R2RMLTC0002h/test_R2RMLTC0002h_SQLITE.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/r2rml/R2RMLTC0002i/mapping.ttl` & `morph_kgc-2.5.1/test/r2rml/R2RMLTC0002i/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/r2rml/R2RMLTC0002i/resource.db` & `morph_kgc-2.5.1/test/r2rml/R2RMLTC0002i/resource.db`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/r2rml/R2RMLTC0002i/test_R2RMLTC0002i_SQLITE.py` & `morph_kgc-2.5.1/test/r2rml/R2RMLTC0002i/test_R2RMLTC0002i_SQLITE.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/r2rml/R2RMLTC0002j/mapping.ttl` & `morph_kgc-2.5.1/test/r2rml/R2RMLTC0002j/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/r2rml/R2RMLTC0002j/resource.db` & `morph_kgc-2.5.1/test/r2rml/R2RMLTC0002j/resource.db`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/r2rml/R2RMLTC0002j/test_R2RMLTC0002j_SQLITE.py` & `morph_kgc-2.5.1/test/r2rml/R2RMLTC0002j/test_R2RMLTC0002j_SQLITE.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/r2rml/R2RMLTC0003a/R2RMLTC0003a_SQLITE.py` & `morph_kgc-2.5.1/test/r2rml/R2RMLTC0003a/R2RMLTC0003a_SQLITE.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/r2rml/R2RMLTC0003a/mapping.ttl` & `morph_kgc-2.5.1/test/r2rml/R2RMLTC0003a/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/r2rml/R2RMLTC0003a/resource.db` & `morph_kgc-2.5.1/test/r2rml/R2RMLTC0003a/resource.db`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/r2rml/R2RMLTC0003b/mapping.ttl` & `morph_kgc-2.5.1/test/r2rml/R2RMLTC0003b/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/r2rml/R2RMLTC0003b/resource.db` & `morph_kgc-2.5.1/test/r2rml/R2RMLTC0003b/resource.db`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/r2rml/R2RMLTC0003b/test_R2RMLTC0003b_SQLITE.py` & `morph_kgc-2.5.1/test/r2rml/R2RMLTC0003b/test_R2RMLTC0003b_SQLITE.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/r2rml/R2RMLTC0003c/mapping.ttl` & `morph_kgc-2.5.1/test/r2rml/R2RMLTC0003c/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/r2rml/R2RMLTC0003c/resource.db` & `morph_kgc-2.5.1/test/r2rml/R2RMLTC0003c/resource.db`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/r2rml/R2RMLTC0003c/test_R2RMLTC0003c_SQLITE.py` & `morph_kgc-2.5.1/test/r2rml/R2RMLTC0003c/test_R2RMLTC0003c_SQLITE.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/r2rml/R2RMLTC0004a/mapping.ttl` & `morph_kgc-2.5.1/test/r2rml/R2RMLTC0004a/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/r2rml/R2RMLTC0004a/resource.db` & `morph_kgc-2.5.1/test/r2rml/R2RMLTC0004a/resource.db`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/r2rml/R2RMLTC0004a/test_R2RMLTC0004a_SQLITE.py` & `morph_kgc-2.5.1/test/r2rml/R2RMLTC0004a/test_R2RMLTC0004a_SQLITE.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/r2rml/R2RMLTC0004b/mapping.ttl` & `morph_kgc-2.5.1/test/r2rml/R2RMLTC0004b/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/r2rml/R2RMLTC0004b/resource.db` & `morph_kgc-2.5.1/test/r2rml/R2RMLTC0004b/resource.db`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/r2rml/R2RMLTC0004b/test_R2RMLTC0004b_SQLITE.py` & `morph_kgc-2.5.1/test/r2rml/R2RMLTC0004b/test_R2RMLTC0004b_SQLITE.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/r2rml/R2RMLTC0005a/mapping.ttl` & `morph_kgc-2.5.1/test/r2rml/R2RMLTC0005a/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/r2rml/R2RMLTC0005a/resource.db` & `morph_kgc-2.5.1/test/r2rml/R2RMLTC0005a/resource.db`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/r2rml/R2RMLTC0005a/test_R2RMLTC0005a_SQLITE.py` & `morph_kgc-2.5.1/test/r2rml/R2RMLTC0005a/test_R2RMLTC0005a_SQLITE.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/r2rml/R2RMLTC0005b/mapping.ttl` & `morph_kgc-2.5.1/test/r2rml/R2RMLTC0005b/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/r2rml/R2RMLTC0005b/output.nq` & `morph_kgc-2.5.1/test/r2rml/R2RMLTC0005b/output.nq`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/r2rml/R2RMLTC0005b/resource.db` & `morph_kgc-2.5.1/test/r2rml/R2RMLTC0005b/resource.db`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/r2rml/R2RMLTC0005b/test_R2RMLTC0005b_SQLITE.py` & `morph_kgc-2.5.1/test/r2rml/R2RMLTC0005b/test_R2RMLTC0005b_SQLITE.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/r2rml/R2RMLTC0006a/mapping.ttl` & `morph_kgc-2.5.1/test/r2rml/R2RMLTC0006a/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/r2rml/R2RMLTC0006a/resource.db` & `morph_kgc-2.5.1/test/r2rml/R2RMLTC0006a/resource.db`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/r2rml/R2RMLTC0006a/test_R2RMLTC0006a_SQLITE.py` & `morph_kgc-2.5.1/test/r2rml/R2RMLTC0006a/test_R2RMLTC0006a_SQLITE.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/r2rml/R2RMLTC0007a/mapping.ttl` & `morph_kgc-2.5.1/test/r2rml/R2RMLTC0007a/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/r2rml/R2RMLTC0007a/resource.db` & `morph_kgc-2.5.1/test/r2rml/R2RMLTC0007a/resource.db`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/r2rml/R2RMLTC0007a/test_R2RMLTC0007a_SQLITE.py` & `morph_kgc-2.5.1/test/r2rml/R2RMLTC0007a/test_R2RMLTC0007a_SQLITE.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/r2rml/R2RMLTC0007b/mapping.ttl` & `morph_kgc-2.5.1/test/r2rml/R2RMLTC0007b/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/r2rml/R2RMLTC0007b/resource.db` & `morph_kgc-2.5.1/test/r2rml/R2RMLTC0007b/resource.db`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/r2rml/R2RMLTC0007b/test_R2RMLTC0007b_SQLITE.py` & `morph_kgc-2.5.1/test/r2rml/R2RMLTC0007b/test_R2RMLTC0007b_SQLITE.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/r2rml/R2RMLTC0007c/mapping.ttl` & `morph_kgc-2.5.1/test/r2rml/R2RMLTC0007c/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/r2rml/R2RMLTC0007c/resource.db` & `morph_kgc-2.5.1/test/r2rml/R2RMLTC0007c/resource.db`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/r2rml/R2RMLTC0007c/test_R2RMLTC0007c_SQLITE.py` & `morph_kgc-2.5.1/test/r2rml/R2RMLTC0007c/test_R2RMLTC0007c_SQLITE.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/r2rml/R2RMLTC0007d/mapping.ttl` & `morph_kgc-2.5.1/test/r2rml/R2RMLTC0007d/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/r2rml/R2RMLTC0007d/resource.db` & `morph_kgc-2.5.1/test/r2rml/R2RMLTC0007d/resource.db`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/r2rml/R2RMLTC0007d/test_R2RMLTC0007d_SQLITE.py` & `morph_kgc-2.5.1/test/r2rml/R2RMLTC0007d/test_R2RMLTC0007d_SQLITE.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/r2rml/R2RMLTC0007e/mapping.ttl` & `morph_kgc-2.5.1/test/r2rml/R2RMLTC0007e/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/r2rml/R2RMLTC0007e/resource.db` & `morph_kgc-2.5.1/test/r2rml/R2RMLTC0007e/resource.db`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/r2rml/R2RMLTC0007e/test_R2RMLTC0007e_SQLITE.py` & `morph_kgc-2.5.1/test/r2rml/R2RMLTC0007e/test_R2RMLTC0007e_SQLITE.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/r2rml/R2RMLTC0007f/mapping.ttl` & `morph_kgc-2.5.1/test/r2rml/R2RMLTC0007f/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/r2rml/R2RMLTC0007f/resource.db` & `morph_kgc-2.5.1/test/r2rml/R2RMLTC0007f/resource.db`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/r2rml/R2RMLTC0007f/test_R2RMLTC0007f_SQLITE.py` & `morph_kgc-2.5.1/test/r2rml/R2RMLTC0007f/test_R2RMLTC0007f_SQLITE.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/r2rml/R2RMLTC0007g/mapping.ttl` & `morph_kgc-2.5.1/test/r2rml/R2RMLTC0007g/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/r2rml/R2RMLTC0007g/resource.db` & `morph_kgc-2.5.1/test/r2rml/R2RMLTC0007g/resource.db`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/r2rml/R2RMLTC0007g/test_R2RMLTC0007g_SQLITE.py` & `morph_kgc-2.5.1/test/r2rml/R2RMLTC0007g/test_R2RMLTC0007g_SQLITE.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/r2rml/R2RMLTC0007h/mapping.ttl` & `morph_kgc-2.5.1/test/r2rml/R2RMLTC0007h/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/r2rml/R2RMLTC0007h/resource.db` & `morph_kgc-2.5.1/test/r2rml/R2RMLTC0007h/resource.db`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/r2rml/R2RMLTC0007h/test_R2RMLTC0007h_SQLITE.py` & `morph_kgc-2.5.1/test/r2rml/R2RMLTC0007h/test_R2RMLTC0007h_SQLITE.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/r2rml/R2RMLTC0008a/mapping.ttl` & `morph_kgc-2.5.1/test/r2rml/R2RMLTC0008a/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/r2rml/R2RMLTC0008a/output.nq` & `morph_kgc-2.5.1/test/r2rml/R2RMLTC0008a/output.nq`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/r2rml/R2RMLTC0008a/resource.db` & `morph_kgc-2.5.1/test/r2rml/R2RMLTC0008a/resource.db`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/r2rml/R2RMLTC0008a/test_R2RMLTC0008a_SQLITE.py` & `morph_kgc-2.5.1/test/r2rml/R2RMLTC0008a/test_R2RMLTC0008a_SQLITE.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/r2rml/R2RMLTC0008b/mapping.ttl` & `morph_kgc-2.5.1/test/r2rml/R2RMLTC0008b/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/r2rml/R2RMLTC0008b/output.nq` & `morph_kgc-2.5.1/test/r2rml/R2RMLTC0008b/output.nq`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/r2rml/R2RMLTC0008b/resource.db` & `morph_kgc-2.5.1/test/r2rml/R2RMLTC0008b/resource.db`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/r2rml/R2RMLTC0008b/test_R2RMLTC0008b_SQLITE.py` & `morph_kgc-2.5.1/test/r2rml/R2RMLTC0008b/test_R2RMLTC0008b_SQLITE.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/r2rml/R2RMLTC0008c/mapping.ttl` & `morph_kgc-2.5.1/test/r2rml/R2RMLTC0008c/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/r2rml/R2RMLTC0008c/resource.db` & `morph_kgc-2.5.1/test/r2rml/R2RMLTC0008c/resource.db`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/r2rml/R2RMLTC0008c/test_R2RMLTC0008c_SQLITE.py` & `morph_kgc-2.5.1/test/r2rml/R2RMLTC0008c/test_R2RMLTC0008c_SQLITE.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/r2rml/R2RMLTC0009a/mapping.ttl` & `morph_kgc-2.5.1/test/r2rml/R2RMLTC0009a/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/r2rml/R2RMLTC0009a/resource.db` & `morph_kgc-2.5.1/test/r2rml/R2RMLTC0009a/resource.db`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/r2rml/R2RMLTC0009a/test_R2RMLTC0009a_SQLITE.py` & `morph_kgc-2.5.1/test/r2rml/R2RMLTC0009a/test_R2RMLTC0009a_SQLITE.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/r2rml/R2RMLTC0009b/mapping.ttl` & `morph_kgc-2.5.1/test/r2rml/R2RMLTC0009b/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/r2rml/R2RMLTC0009b/output.nq` & `morph_kgc-2.5.1/test/r2rml/R2RMLTC0009b/output.nq`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/r2rml/R2RMLTC0009b/resource.db` & `morph_kgc-2.5.1/test/r2rml/R2RMLTC0009b/resource.db`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/r2rml/R2RMLTC0009b/test_R2RMLTC0009b_SQLITE.py` & `morph_kgc-2.5.1/test/r2rml/R2RMLTC0009b/test_R2RMLTC0009b_SQLITE.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/r2rml/R2RMLTC0009c/mapping.ttl` & `morph_kgc-2.5.1/test/r2rml/R2RMLTC0009c/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/r2rml/R2RMLTC0009c/resource.db` & `morph_kgc-2.5.1/test/r2rml/R2RMLTC0009c/resource.db`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/r2rml/R2RMLTC0009c/test_R2RMLTC0009c_SQLITE.py` & `morph_kgc-2.5.1/test/r2rml/R2RMLTC0009c/test_R2RMLTC0009c_SQLITE.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/r2rml/R2RMLTC0009d/mapping.ttl` & `morph_kgc-2.5.1/test/r2rml/R2RMLTC0009d/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/r2rml/R2RMLTC0009d/resource.db` & `morph_kgc-2.5.1/test/r2rml/R2RMLTC0009d/resource.db`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/r2rml/R2RMLTC0009d/test_R2RMLTC0009d_SQLITE.py` & `morph_kgc-2.5.1/test/r2rml/R2RMLTC0009d/test_R2RMLTC0009d_SQLITE.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/r2rml/R2RMLTC0010a/resource.db` & `morph_kgc-2.5.1/test/r2rml/R2RMLTC0010a/resource.db`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/r2rml/R2RMLTC0010a/test_R2RMLTC0010a_SQLITE.py` & `morph_kgc-2.5.1/test/r2rml/R2RMLTC0010a/test_R2RMLTC0010a_SQLITE.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/r2rml/R2RMLTC0010b/resource.db` & `morph_kgc-2.5.1/test/r2rml/R2RMLTC0010b/resource.db`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/r2rml/R2RMLTC0010b/test_R2RMLTC0010b_SQLITE.py` & `morph_kgc-2.5.1/test/r2rml/R2RMLTC0010b/test_R2RMLTC0010b_SQLITE.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/r2rml/R2RMLTC0010c/mapping.ttl` & `morph_kgc-2.5.1/test/r2rml/R2RMLTC0010c/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/r2rml/R2RMLTC0010c/resource.db` & `morph_kgc-2.5.1/test/r2rml/R2RMLTC0010c/resource.db`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/r2rml/R2RMLTC0010c/test_R2RMLTC0010c_SQLITE.py` & `morph_kgc-2.5.1/test/r2rml/R2RMLTC0010c/test_R2RMLTC0010c_SQLITE.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/r2rml/R2RMLTC0011a/mapping.ttl` & `morph_kgc-2.5.1/test/r2rml/R2RMLTC0011a/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/r2rml/R2RMLTC0011a/output.nq` & `morph_kgc-2.5.1/test/r2rml/R2RMLTC0011a/output.nq`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/r2rml/R2RMLTC0011a/resource.db` & `morph_kgc-2.5.1/test/r2rml/R2RMLTC0011a/resource.db`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/r2rml/R2RMLTC0011a/resource.sql` & `morph_kgc-2.5.1/test/r2rml/R2RMLTC0011a/resource.sql`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/r2rml/R2RMLTC0011a/test_R2RMLTC0011a_SQLITE.py` & `morph_kgc-2.5.1/test/r2rml/R2RMLTC0011a/test_R2RMLTC0011a_SQLITE.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/r2rml/R2RMLTC0011b/mapping.ttl` & `morph_kgc-2.5.1/test/r2rml/R2RMLTC0011b/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/r2rml/R2RMLTC0011b/output.nq` & `morph_kgc-2.5.1/test/r2rml/R2RMLTC0011b/output.nq`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/r2rml/R2RMLTC0011b/resource.db` & `morph_kgc-2.5.1/test/r2rml/R2RMLTC0011b/resource.db`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/r2rml/R2RMLTC0011b/resource.sql` & `morph_kgc-2.5.1/test/r2rml/R2RMLTC0011b/resource.sql`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/r2rml/R2RMLTC0011b/test_R2RMLTC0011b_SQLITE.py` & `morph_kgc-2.5.1/test/r2rml/R2RMLTC0011b/test_R2RMLTC0011b_SQLITE.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/r2rml/R2RMLTC0012a/mapping.ttl` & `morph_kgc-2.5.1/test/r2rml/R2RMLTC0012a/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/r2rml/R2RMLTC0012a/resource.db` & `morph_kgc-2.5.1/test/r2rml/R2RMLTC0012a/resource.db`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/r2rml/R2RMLTC0012a/resource.sql` & `morph_kgc-2.5.1/test/r2rml/R2RMLTC0012a/resource.sql`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/r2rml/R2RMLTC0012a/test_R2RMLTC0012a_SQLITE.py` & `morph_kgc-2.5.1/test/r2rml/R2RMLTC0012a/test_R2RMLTC0012a_SQLITE.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/r2rml/R2RMLTC0012b/mapping.ttl` & `morph_kgc-2.5.1/test/r2rml/R2RMLTC0012b/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/r2rml/R2RMLTC0012b/resource.db` & `morph_kgc-2.5.1/test/r2rml/R2RMLTC0012b/resource.db`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/r2rml/R2RMLTC0012b/resource.sql` & `morph_kgc-2.5.1/test/r2rml/R2RMLTC0012b/resource.sql`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/r2rml/R2RMLTC0012b/test_R2RMLTC0012b_SQLITE.py` & `morph_kgc-2.5.1/test/r2rml/R2RMLTC0012b/test_R2RMLTC0012b_SQLITE.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/r2rml/R2RMLTC0012c/mapping.ttl` & `morph_kgc-2.5.1/test/r2rml/R2RMLTC0012c/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/r2rml/R2RMLTC0012c/resource.db` & `morph_kgc-2.5.1/test/r2rml/R2RMLTC0012c/resource.db`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/r2rml/R2RMLTC0012c/resource.sql` & `morph_kgc-2.5.1/test/r2rml/R2RMLTC0012c/resource.sql`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/r2rml/R2RMLTC0012c/test_R2RMLTC0012c_SQLITE.py` & `morph_kgc-2.5.1/test/r2rml/R2RMLTC0012c/test_R2RMLTC0012c_SQLITE.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/r2rml/R2RMLTC0012d/mapping.ttl` & `morph_kgc-2.5.1/test/r2rml/R2RMLTC0012d/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/r2rml/R2RMLTC0012d/resource.db` & `morph_kgc-2.5.1/test/r2rml/R2RMLTC0012d/resource.db`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/r2rml/R2RMLTC0012d/resource.sql` & `morph_kgc-2.5.1/test/r2rml/R2RMLTC0012d/resource.sql`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/r2rml/R2RMLTC0012d/test_R2RMLTC0012d_SQLITE.py` & `morph_kgc-2.5.1/test/r2rml/R2RMLTC0012d/test_R2RMLTC0012d_SQLITE.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/r2rml/R2RMLTC0012e/mapping.ttl` & `morph_kgc-2.5.1/test/r2rml/R2RMLTC0012e/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/r2rml/R2RMLTC0012e/output.nq` & `morph_kgc-2.5.1/test/r2rml/R2RMLTC0012e/output.nq`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/r2rml/R2RMLTC0012e/resource.db` & `morph_kgc-2.5.1/test/r2rml/R2RMLTC0012e/resource.db`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/r2rml/R2RMLTC0012e/resource.sql` & `morph_kgc-2.5.1/test/r2rml/R2RMLTC0012e/resource.sql`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/r2rml/R2RMLTC0012e/test_R2RMLTC0012e_SQLITE.py` & `morph_kgc-2.5.1/test/r2rml/R2RMLTC0012e/test_R2RMLTC0012e_SQLITE.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/r2rml/R2RMLTC0013a/mapping.ttl` & `morph_kgc-2.5.1/test/r2rml/R2RMLTC0013a/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/r2rml/R2RMLTC0013a/resource.db` & `morph_kgc-2.5.1/test/r2rml/R2RMLTC0013a/resource.db`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/r2rml/R2RMLTC0013a/test_R2RMLTC0013a_SQLITE.py` & `morph_kgc-2.5.1/test/r2rml/R2RMLTC0013a/test_R2RMLTC0013a_SQLITE.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/r2rml/R2RMLTC0014d/mapping.ttl` & `morph_kgc-2.5.1/test/r2rml/R2RMLTC0014d/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/r2rml/R2RMLTC0014d/resource.db` & `morph_kgc-2.5.1/test/r2rml/R2RMLTC0014d/resource.db`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/r2rml/R2RMLTC0014d/resource.sql` & `morph_kgc-2.5.1/test/r2rml/R2RMLTC0014d/resource.sql`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/r2rml/R2RMLTC0014d/test_R2RMLTC0014d_SQLITE.py` & `morph_kgc-2.5.1/test/r2rml/R2RMLTC0014d/test_R2RMLTC0014d_SQLITE.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/r2rml/R2RMLTC0015a/mapping.ttl` & `morph_kgc-2.5.1/test/r2rml/R2RMLTC0015a/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/r2rml/R2RMLTC0015a/resource.db` & `morph_kgc-2.5.1/test/r2rml/R2RMLTC0015a/resource.db`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/r2rml/R2RMLTC0015a/test_R2RMLTC0015a_SQLITE.py` & `morph_kgc-2.5.1/test/r2rml/R2RMLTC0015a/test_R2RMLTC0015a_SQLITE.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/r2rml/R2RMLTC0015b/mapping.ttl` & `morph_kgc-2.5.1/test/r2rml/R2RMLTC0015b/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/r2rml/R2RMLTC0015b/resource.db` & `morph_kgc-2.5.1/test/r2rml/R2RMLTC0015b/resource.db`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/r2rml/R2RMLTC0015b/test_R2RMLTC0015b_SQLITE.py` & `morph_kgc-2.5.1/test/r2rml/R2RMLTC0015b/test_R2RMLTC0015b_SQLITE.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/r2rml/R2RMLTC0016a/mapping.ttl` & `morph_kgc-2.5.1/test/r2rml/R2RMLTC0016a/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/r2rml/R2RMLTC0016a/output.nq` & `morph_kgc-2.5.1/test/r2rml/R2RMLTC0016a/output.nq`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/r2rml/R2RMLTC0016a/resource.db` & `morph_kgc-2.5.1/test/r2rml/R2RMLTC0016a/resource.db`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/r2rml/R2RMLTC0016a/resource.sql` & `morph_kgc-2.5.1/test/r2rml/R2RMLTC0016a/resource.sql`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/r2rml/R2RMLTC0016a/test_R2RMLTC0016a_SQLITE.py` & `morph_kgc-2.5.1/test/r2rml/R2RMLTC0016a/test_R2RMLTC0016a_SQLITE.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/r2rml/R2RMLTC0016b/R2RMLTC0016b_SQLITE.py` & `morph_kgc-2.5.1/test/r2rml/R2RMLTC0016b/R2RMLTC0016b_SQLITE.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/r2rml/R2RMLTC0016b/mapping.ttl` & `morph_kgc-2.5.1/test/r2rml/R2RMLTC0016b/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/r2rml/R2RMLTC0016b/output.nq` & `morph_kgc-2.5.1/test/r2rml/R2RMLTC0016b/output.nq`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/r2rml/R2RMLTC0016b/resource.db` & `morph_kgc-2.5.1/test/r2rml/R2RMLTC0016b/resource.db`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/r2rml/R2RMLTC0016b/resource.sql` & `morph_kgc-2.5.1/test/r2rml/R2RMLTC0016b/resource.sql`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/r2rml/R2RMLTC0016c/R2RMLTC0016c_SQLITE.py` & `morph_kgc-2.5.1/test/r2rml/R2RMLTC0016c/R2RMLTC0016c_SQLITE.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/r2rml/R2RMLTC0016c/mapping.ttl` & `morph_kgc-2.5.1/test/r2rml/R2RMLTC0016c/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/r2rml/R2RMLTC0016c/output.nq` & `morph_kgc-2.5.1/test/r2rml/R2RMLTC0016c/output.nq`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/r2rml/R2RMLTC0016c/resource.db` & `morph_kgc-2.5.1/test/r2rml/R2RMLTC0016c/resource.db`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/r2rml/R2RMLTC0016c/resource.sql` & `morph_kgc-2.5.1/test/r2rml/R2RMLTC0016c/resource.sql`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/r2rml/R2RMLTC0016d/R2RMLTC0016d_SQLITE.py` & `morph_kgc-2.5.1/test/r2rml/R2RMLTC0016d/R2RMLTC0016d_SQLITE.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/r2rml/R2RMLTC0016d/mapping.ttl` & `morph_kgc-2.5.1/test/r2rml/R2RMLTC0016d/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/r2rml/R2RMLTC0016d/output.nq` & `morph_kgc-2.5.1/test/r2rml/R2RMLTC0016d/output.nq`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/r2rml/R2RMLTC0016d/resource.db` & `morph_kgc-2.5.1/test/r2rml/R2RMLTC0016d/resource.db`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/r2rml/R2RMLTC0016d/resource.sql` & `morph_kgc-2.5.1/test/r2rml/R2RMLTC0016d/resource.sql`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/r2rml/R2RMLTC0016e/R2RMLTC0016e_SQLITE.py` & `morph_kgc-2.5.1/test/r2rml/R2RMLTC0016e/R2RMLTC0016e_SQLITE.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/r2rml/R2RMLTC0016e/mapping.ttl` & `morph_kgc-2.5.1/test/r2rml/R2RMLTC0016e/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/r2rml/R2RMLTC0016e/output.nq` & `morph_kgc-2.5.1/test/r2rml/R2RMLTC0016e/output.nq`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/r2rml/R2RMLTC0016e/resource.db` & `morph_kgc-2.5.1/test/r2rml/R2RMLTC0016e/resource.db`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/r2rml/R2RMLTC0016e/resource.sql` & `morph_kgc-2.5.1/test/r2rml/R2RMLTC0016e/resource.sql`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/r2rml/R2RMLTC0018a/mapping.ttl` & `morph_kgc-2.5.1/test/r2rml/R2RMLTC0018a/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/r2rml/R2RMLTC0018a/output.nq` & `morph_kgc-2.5.1/test/r2rml/R2RMLTC0018a/output.nq`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/r2rml/R2RMLTC0018a/resource.db` & `morph_kgc-2.5.1/test/r2rml/R2RMLTC0018a/resource.db`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/r2rml/R2RMLTC0018a/test_R2RMLTC0018a_SQLITE.py` & `morph_kgc-2.5.1/test/r2rml/R2RMLTC0018a/test_R2RMLTC0018a_SQLITE.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/r2rml/R2RMLTC0019a/R2RMLTC0019a_SQLITE.py` & `morph_kgc-2.5.1/test/r2rml/R2RMLTC0019a/R2RMLTC0019a_SQLITE.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/r2rml/R2RMLTC0019a/mapping.ttl` & `morph_kgc-2.5.1/test/r2rml/R2RMLTC0019a/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/r2rml/R2RMLTC0019a/resource.db` & `morph_kgc-2.5.1/test/r2rml/R2RMLTC0019a/resource.db`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/r2rml/R2RMLTC0019b/R2RMLTC0019b_SQLITE.py` & `morph_kgc-2.5.1/test/r2rml/R2RMLTC0019b/R2RMLTC0019b_SQLITE.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/r2rml/R2RMLTC0019b/resource.db` & `morph_kgc-2.5.1/test/r2rml/R2RMLTC0019b/resource.db`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/r2rml/R2RMLTC0020a/R2RMLTC0020a_SQLITE.py` & `morph_kgc-2.5.1/test/r2rml/R2RMLTC0020a/R2RMLTC0020a_SQLITE.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/r2rml/R2RMLTC0020a/mapping.ttl` & `morph_kgc-2.5.1/test/r2rml/R2RMLTC0020a/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/r2rml/R2RMLTC0020a/output.nq` & `morph_kgc-2.5.1/test/r2rml/R2RMLTC0020a/output.nq`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/r2rml/R2RMLTC0020a/resource.db` & `morph_kgc-2.5.1/test/r2rml/R2RMLTC0020a/resource.db`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/r2rml/R2RMLTC0020b/R2RMLTC0020b_SQLITE.py` & `morph_kgc-2.5.1/test/r2rml/R2RMLTC0020b/R2RMLTC0020b_SQLITE.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/r2rml/R2RMLTC0020b/mapping.ttl` & `morph_kgc-2.5.1/test/r2rml/R2RMLTC0020b/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/r2rml/R2RMLTC0020b/resource.db` & `morph_kgc-2.5.1/test/r2rml/R2RMLTC0020b/resource.db`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/csv/RMLTC0000/mapping.ttl` & `morph_kgc-2.5.1/test/rml/csv/RMLTC0000/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/csv/RMLTC0000/test_RMLTC0000_CSV.py` & `morph_kgc-2.5.1/test/rml/csv/RMLTC0000/test_RMLTC0000_CSV.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/csv/RMLTC0001a/mapping.ttl` & `morph_kgc-2.5.1/test/rml/csv/RMLTC0001a/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/csv/RMLTC0001a/test_RMLTC0001a_CSV.py` & `morph_kgc-2.5.1/test/rml/csv/RMLTC0001a/test_RMLTC0001a_CSV.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/csv/RMLTC0001b/mapping.ttl` & `morph_kgc-2.5.1/test/rml/csv/RMLTC0001b/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/csv/RMLTC0001b/test_RMLTC0001b_CSV.py` & `morph_kgc-2.5.1/test/rml/csv/RMLTC0001b/test_RMLTC0001b_CSV.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/csv/RMLTC0002a/mapping.ttl` & `morph_kgc-2.5.1/test/rml/csv/RMLTC0002a/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/csv/RMLTC0002a/test_RMLTC0002a_CSV.py` & `morph_kgc-2.5.1/test/rml/csv/RMLTC0002a/test_RMLTC0002a_CSV.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/csv/RMLTC0002b/mapping.ttl` & `morph_kgc-2.5.1/test/rml/csv/RMLTC0002b/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/csv/RMLTC0002b/test_RMLTC0002b_CSV.py` & `morph_kgc-2.5.1/test/rml/csv/RMLTC0002b/test_RMLTC0002b_CSV.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/csv/RMLTC0002c/mapping.ttl` & `morph_kgc-2.5.1/test/rml/csv/RMLTC0002c/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/csv/RMLTC0002c/test_RMLTC0002c_CSV.py` & `morph_kgc-2.5.1/test/rml/csv/RMLTC0002c/test_RMLTC0002c_CSV.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/csv/RMLTC0002e/mapping.ttl` & `morph_kgc-2.5.1/test/rml/csv/RMLTC0002e/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/csv/RMLTC0002e/test_RMLTC0002e_CSV.py` & `morph_kgc-2.5.1/test/rml/csv/RMLTC0002e/test_RMLTC0002e_CSV.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/csv/RMLTC0003c/mapping.ttl` & `morph_kgc-2.5.1/test/rml/csv/RMLTC0003c/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/csv/RMLTC0003c/test_RMLTC0003c_CSV.py` & `morph_kgc-2.5.1/test/rml/csv/RMLTC0003c/test_RMLTC0003c_CSV.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/csv/RMLTC0004a/mapping.ttl` & `morph_kgc-2.5.1/test/rml/csv/RMLTC0004a/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/csv/RMLTC0004a/test_RMLTC0004a_CSV.py` & `morph_kgc-2.5.1/test/rml/csv/RMLTC0004a/test_RMLTC0004a_CSV.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/csv/RMLTC0004b/mapping.ttl` & `morph_kgc-2.5.1/test/rml/csv/RMLTC0004b/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/csv/RMLTC0004b/test_RMLTC0004b_CSV.py` & `morph_kgc-2.5.1/test/rml/csv/RMLTC0004b/test_RMLTC0004b_CSV.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/csv/RMLTC0005a/mapping.ttl` & `morph_kgc-2.5.1/test/rml/csv/RMLTC0005a/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/csv/RMLTC0005a/test_RMLTC0005a_CSV.py` & `morph_kgc-2.5.1/test/rml/csv/RMLTC0005a/test_RMLTC0005a_CSV.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/csv/RMLTC0006a/mapping.ttl` & `morph_kgc-2.5.1/test/rml/csv/RMLTC0006a/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/csv/RMLTC0006a/test_RMLTC0006a_CSV.py` & `morph_kgc-2.5.1/test/rml/csv/RMLTC0006a/test_RMLTC0006a_CSV.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/csv/RMLTC0007a/mapping.ttl` & `morph_kgc-2.5.1/test/rml/csv/RMLTC0007a/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/csv/RMLTC0007a/test_RMLTC0007a_CSV.py` & `morph_kgc-2.5.1/test/rml/csv/RMLTC0007a/test_RMLTC0007a_CSV.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/csv/RMLTC0007b/mapping.ttl` & `morph_kgc-2.5.1/test/rml/csv/RMLTC0007b/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/csv/RMLTC0007b/test_RMLTC0007b_CSV.py` & `morph_kgc-2.5.1/test/rml/csv/RMLTC0007b/test_RMLTC0007b_CSV.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/csv/RMLTC0007c/mapping.ttl` & `morph_kgc-2.5.1/test/rml/csv/RMLTC0007c/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/csv/RMLTC0007c/test_RMLTC0007c_CSV.py` & `morph_kgc-2.5.1/test/rml/csv/RMLTC0007c/test_RMLTC0007c_CSV.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/csv/RMLTC0007d/mapping.ttl` & `morph_kgc-2.5.1/test/rml/csv/RMLTC0007d/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/csv/RMLTC0007d/test_RMLTC0007d_CSV.py` & `morph_kgc-2.5.1/test/rml/csv/RMLTC0007d/test_RMLTC0007d_CSV.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/csv/RMLTC0007e/mapping.ttl` & `morph_kgc-2.5.1/test/rml/csv/RMLTC0007e/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/csv/RMLTC0007e/test_RMLTC0007e_CSV.py` & `morph_kgc-2.5.1/test/rml/csv/RMLTC0007e/test_RMLTC0007e_CSV.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/csv/RMLTC0007f/mapping.ttl` & `morph_kgc-2.5.1/test/rml/csv/RMLTC0007f/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/csv/RMLTC0007f/test_RMLTC0007f_CSV.py` & `morph_kgc-2.5.1/test/rml/csv/RMLTC0007f/test_RMLTC0007f_CSV.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/csv/RMLTC0007g/mapping.ttl` & `morph_kgc-2.5.1/test/rml/csv/RMLTC0007g/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/csv/RMLTC0007g/test_RMLTC0007g_CSV.py` & `morph_kgc-2.5.1/test/rml/csv/RMLTC0007g/test_RMLTC0007g_CSV.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/csv/RMLTC0007h/mapping.ttl` & `morph_kgc-2.5.1/test/rml/csv/RMLTC0007h/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/csv/RMLTC0007h/test_RMLTC0007h_CSV.py` & `morph_kgc-2.5.1/test/rml/csv/RMLTC0007h/test_RMLTC0007h_CSV.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/csv/RMLTC0008a/mapping.ttl` & `morph_kgc-2.5.1/test/rml/csv/RMLTC0008a/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/csv/RMLTC0008a/output.nq` & `morph_kgc-2.5.1/test/rml/csv/RMLTC0008a/output.nq`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/csv/RMLTC0008a/test_RMLTC0008a_CSV.py` & `morph_kgc-2.5.1/test/rml/csv/RMLTC0008a/test_RMLTC0008a_CSV.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/csv/RMLTC0008b/mapping.ttl` & `morph_kgc-2.5.1/test/rml/csv/RMLTC0008b/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/csv/RMLTC0008b/output.nq` & `morph_kgc-2.5.1/test/rml/csv/RMLTC0008b/output.nq`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/csv/RMLTC0008b/test_RMLTC0008b_CSV.py` & `morph_kgc-2.5.1/test/rml/csv/RMLTC0008b/test_RMLTC0008b_CSV.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/csv/RMLTC0008c/mapping.ttl` & `morph_kgc-2.5.1/test/rml/csv/RMLTC0008c/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/csv/RMLTC0008c/test_RMLTC0008c_CSV.py` & `morph_kgc-2.5.1/test/rml/csv/RMLTC0008c/test_RMLTC0008c_CSV.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/csv/RMLTC0009a/mapping.ttl` & `morph_kgc-2.5.1/test/rml/csv/RMLTC0009a/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/csv/RMLTC0009a/test_RMLTC0009a_CSV.py` & `morph_kgc-2.5.1/test/rml/csv/RMLTC0009a/test_RMLTC0009a_CSV.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/csv/RMLTC0009b/mapping.ttl` & `morph_kgc-2.5.1/test/rml/csv/RMLTC0009b/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/csv/RMLTC0009b/output.nq` & `morph_kgc-2.5.1/test/rml/csv/RMLTC0009b/output.nq`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/csv/RMLTC0009b/test_RMLTC0009b_CSV.py` & `morph_kgc-2.5.1/test/rml/csv/RMLTC0009b/test_RMLTC0009b_CSV.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/csv/RMLTC0010a/mapping.ttl` & `morph_kgc-2.5.1/test/rml/csv/RMLTC0010a/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/csv/RMLTC0010a/test_RMLTC0010a_CSV.py` & `morph_kgc-2.5.1/test/rml/csv/RMLTC0010a/test_RMLTC0010a_CSV.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/csv/RMLTC0010b/mapping.ttl` & `morph_kgc-2.5.1/test/rml/csv/RMLTC0010b/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/csv/RMLTC0010b/test_RMLTC0010b_CSV.py` & `morph_kgc-2.5.1/test/rml/csv/RMLTC0010b/test_RMLTC0010b_CSV.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/csv/RMLTC0010c/mapping.ttl` & `morph_kgc-2.5.1/test/rml/csv/RMLTC0010c/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/csv/RMLTC0010c/test_RMLTC0010c_CSV.py` & `morph_kgc-2.5.1/test/rml/csv/RMLTC0010c/test_RMLTC0010c_CSV.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/csv/RMLTC0011b/mapping.ttl` & `morph_kgc-2.5.1/test/rml/csv/RMLTC0011b/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/csv/RMLTC0011b/output.nq` & `morph_kgc-2.5.1/test/rml/csv/RMLTC0011b/output.nq`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/csv/RMLTC0011b/test_RMLTC0011b_CSV.py` & `morph_kgc-2.5.1/test/rml/csv/RMLTC0011b/test_RMLTC0011b_CSV.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/csv/RMLTC0012a/mapping.ttl` & `morph_kgc-2.5.1/test/rml/csv/RMLTC0012a/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/csv/RMLTC0012a/test_RMLTC0012a_CSV.py` & `morph_kgc-2.5.1/test/rml/csv/RMLTC0012a/test_RMLTC0012a_CSV.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/csv/RMLTC0012b/mapping.ttl` & `morph_kgc-2.5.1/test/rml/csv/RMLTC0012b/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/csv/RMLTC0012b/test_RMLTC0012b_CSV.py` & `morph_kgc-2.5.1/test/rml/csv/RMLTC0012b/test_RMLTC0012b_CSV.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/csv/RMLTC0012c/mapping.ttl` & `morph_kgc-2.5.1/test/rml/csv/RMLTC0012c/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/csv/RMLTC0012c/test_RMLTC0012c_CSV.py` & `morph_kgc-2.5.1/test/rml/csv/RMLTC0012c/test_RMLTC0012c_CSV.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/csv/RMLTC0012d/mapping.ttl` & `morph_kgc-2.5.1/test/rml/csv/RMLTC0012d/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/csv/RMLTC0012d/test_RMLTC0012d_CSV.py` & `morph_kgc-2.5.1/test/rml/csv/RMLTC0012d/test_RMLTC0012d_CSV.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/csv/RMLTC0015a/mapping.ttl` & `morph_kgc-2.5.1/test/rml/csv/RMLTC0015a/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/csv/RMLTC0015a/test_RMLTC0015a_CSV.py` & `morph_kgc-2.5.1/test/rml/csv/RMLTC0015a/test_RMLTC0015a_CSV.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/csv/RMLTC0015b/mapping.ttl` & `morph_kgc-2.5.1/test/rml/csv/RMLTC0015b/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/csv/RMLTC0015b/test_RMLTC0015b_CSV.py` & `morph_kgc-2.5.1/test/rml/csv/RMLTC0015b/test_RMLTC0015b_CSV.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/csv/RMLTC0019a/RMLTC0019a_CSV.py` & `morph_kgc-2.5.1/test/rml/csv/RMLTC0019a/RMLTC0019a_CSV.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/csv/RMLTC0019a/mapping.ttl` & `morph_kgc-2.5.1/test/rml/csv/RMLTC0019a/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/csv/RMLTC0019b/RMLTC0019b_CSV.py` & `morph_kgc-2.5.1/test/rml/csv/RMLTC0019b/RMLTC0019b_CSV.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/csv/RMLTC0019b/mapping.ttl` & `morph_kgc-2.5.1/test/rml/csv/RMLTC0019b/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/csv/RMLTC0020a/RMLTC0020a_CSV.py` & `morph_kgc-2.5.1/test/rml/csv/RMLTC0020a/RMLTC0020a_CSV.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/csv/RMLTC0020a/mapping.ttl` & `morph_kgc-2.5.1/test/rml/csv/RMLTC0020a/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/csv/RMLTC0020a/output.nq` & `morph_kgc-2.5.1/test/rml/csv/RMLTC0020a/output.nq`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/csv/RMLTC0020b/RMLTC0020b_CSV.py` & `morph_kgc-2.5.1/test/rml/csv/RMLTC0020b/RMLTC0020b_CSV.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/csv/RMLTC0020b/mapping.ttl` & `morph_kgc-2.5.1/test/rml/csv/RMLTC0020b/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/csv/null_filter/mapping.ttl` & `morph_kgc-2.5.1/test/rml/csv/null_filter/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/csv/null_filter/test_null_filter_CSV.py` & `morph_kgc-2.5.1/test/rml/csv/null_filter/test_null_filter_CSV.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/csv/triples_map_without_pom/mapping.ttl` & `morph_kgc-2.5.1/test/rml/csv/triples_map_without_pom/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/csv/triples_map_without_pom/test_triples_map_without_pom_CSV.py` & `morph_kgc-2.5.1/test/rml/csv/triples_map_without_pom/test_triples_map_without_pom_CSV.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/json/RMLTC0000/mapping.ttl` & `morph_kgc-2.5.1/test/rml/json/RMLTC0000/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/json/RMLTC0000/test_RMLTC0000_JSON.py` & `morph_kgc-2.5.1/test/rml/json/RMLTC0000/test_RMLTC0000_JSON.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/json/RMLTC0001a/mapping.ttl` & `morph_kgc-2.5.1/test/rml/json/RMLTC0001a/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/json/RMLTC0001a/test_RMLTC0001a_JSON.py` & `morph_kgc-2.5.1/test/rml/json/RMLTC0001a/test_RMLTC0001a_JSON.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/json/RMLTC0001b/mapping.ttl` & `morph_kgc-2.5.1/test/rml/json/RMLTC0001b/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/json/RMLTC0001b/test_RMLTC0001b_JSON.py` & `morph_kgc-2.5.1/test/rml/json/RMLTC0001b/test_RMLTC0001b_JSON.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/json/RMLTC0002a/mapping.ttl` & `morph_kgc-2.5.1/test/rml/json/RMLTC0002a/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/json/RMLTC0002a/test_RMLTC0002a_JSON.py` & `morph_kgc-2.5.1/test/rml/json/RMLTC0002a/test_RMLTC0002a_JSON.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/json/RMLTC0002b/mapping.ttl` & `morph_kgc-2.5.1/test/rml/json/RMLTC0002b/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/json/RMLTC0002b/test_RMLTC0002b_JSON.py` & `morph_kgc-2.5.1/test/rml/json/RMLTC0002b/test_RMLTC0002b_JSON.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/json/RMLTC0002c/mapping.ttl` & `morph_kgc-2.5.1/test/rml/json/RMLTC0002c/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/json/RMLTC0002c/test_RMLTC0002c_JSON.py` & `morph_kgc-2.5.1/test/rml/json/RMLTC0002c/test_RMLTC0002c_JSON.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/json/RMLTC0002e/mapping.ttl` & `morph_kgc-2.5.1/test/rml/json/RMLTC0002e/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/json/RMLTC0002e/test_RMLTC0002e_JSON.py` & `morph_kgc-2.5.1/test/rml/json/RMLTC0002e/test_RMLTC0002e_JSON.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/json/RMLTC0003c/mapping.ttl` & `morph_kgc-2.5.1/test/rml/json/RMLTC0003c/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/json/RMLTC0003c/test_RMLTC0003c_JSON.py` & `morph_kgc-2.5.1/test/rml/json/RMLTC0003c/test_RMLTC0003c_JSON.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/json/RMLTC0004a/mapping.ttl` & `morph_kgc-2.5.1/test/rml/json/RMLTC0004a/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/json/RMLTC0004a/test_RMLTC0004a_JSON.py` & `morph_kgc-2.5.1/test/rml/json/RMLTC0004a/test_RMLTC0004a_JSON.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/json/RMLTC0004b/mapping.ttl` & `morph_kgc-2.5.1/test/rml/json/RMLTC0004b/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/json/RMLTC0004b/test_RMLTC0004b_JSON.py` & `morph_kgc-2.5.1/test/rml/json/RMLTC0004b/test_RMLTC0004b_JSON.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/json/RMLTC0005a/mapping.ttl` & `morph_kgc-2.5.1/test/rml/json/RMLTC0005a/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/json/RMLTC0005a/test_RMLTC0005a_JSON.py` & `morph_kgc-2.5.1/test/rml/json/RMLTC0005a/test_RMLTC0005a_JSON.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/json/RMLTC0006a/mapping.ttl` & `morph_kgc-2.5.1/test/rml/json/RMLTC0006a/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/json/RMLTC0006a/test_RMLTC0006a_JSON.py` & `morph_kgc-2.5.1/test/rml/json/RMLTC0006a/test_RMLTC0006a_JSON.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/json/RMLTC0007a/mapping.ttl` & `morph_kgc-2.5.1/test/rml/json/RMLTC0007a/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/json/RMLTC0007a/test_RMLTC0007a_JSON.py` & `morph_kgc-2.5.1/test/rml/json/RMLTC0007a/test_RMLTC0007a_JSON.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/json/RMLTC0007b/mapping.ttl` & `morph_kgc-2.5.1/test/rml/json/RMLTC0007b/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/json/RMLTC0007b/test_RMLTC0007b_JSON.py` & `morph_kgc-2.5.1/test/rml/json/RMLTC0007b/test_RMLTC0007b_JSON.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/json/RMLTC0007c/mapping.ttl` & `morph_kgc-2.5.1/test/rml/json/RMLTC0007c/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/json/RMLTC0007c/test_RMLTC0007c_JSON.py` & `morph_kgc-2.5.1/test/rml/json/RMLTC0007c/test_RMLTC0007c_JSON.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/json/RMLTC0007d/mapping.ttl` & `morph_kgc-2.5.1/test/rml/json/RMLTC0007d/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/json/RMLTC0007d/test_RMLTC0007d_JSON.py` & `morph_kgc-2.5.1/test/rml/json/RMLTC0007d/test_RMLTC0007d_JSON.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/json/RMLTC0007e/mapping.ttl` & `morph_kgc-2.5.1/test/rml/json/RMLTC0007e/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/json/RMLTC0007e/test_RMLTC0007e_JSON.py` & `morph_kgc-2.5.1/test/rml/json/RMLTC0007e/test_RMLTC0007e_JSON.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/json/RMLTC0007f/mapping.ttl` & `morph_kgc-2.5.1/test/rml/json/RMLTC0007f/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/json/RMLTC0007f/test_RMLTC0007f_JSON.py` & `morph_kgc-2.5.1/test/rml/json/RMLTC0007f/test_RMLTC0007f_JSON.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/json/RMLTC0007g/mapping.ttl` & `morph_kgc-2.5.1/test/rml/json/RMLTC0007g/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/json/RMLTC0007g/test_RMLTC0007g_JSON.py` & `morph_kgc-2.5.1/test/rml/json/RMLTC0007g/test_RMLTC0007g_JSON.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/json/RMLTC0007h/mapping.ttl` & `morph_kgc-2.5.1/test/rml/json/RMLTC0007h/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/json/RMLTC0007h/test_RMLTC0007h_JSON.py` & `morph_kgc-2.5.1/test/rml/json/RMLTC0007h/test_RMLTC0007h_JSON.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/json/RMLTC0008a/mapping.ttl` & `morph_kgc-2.5.1/test/rml/json/RMLTC0008a/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/json/RMLTC0008a/output.nq` & `morph_kgc-2.5.1/test/rml/json/RMLTC0008a/output.nq`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/json/RMLTC0008a/test_RMLTC0008a_JSON.py` & `morph_kgc-2.5.1/test/rml/json/RMLTC0008a/test_RMLTC0008a_JSON.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/json/RMLTC0008b/mapping.ttl` & `morph_kgc-2.5.1/test/rml/json/RMLTC0008b/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/json/RMLTC0008b/output.nq` & `morph_kgc-2.5.1/test/rml/json/RMLTC0008b/output.nq`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/json/RMLTC0008b/test_RMLTC0008b_JSON.py` & `morph_kgc-2.5.1/test/rml/json/RMLTC0008b/test_RMLTC0008b_JSON.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/json/RMLTC0008c/mapping.ttl` & `morph_kgc-2.5.1/test/rml/json/RMLTC0008c/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/json/RMLTC0008c/test_RMLTC0008c_JSON.py` & `morph_kgc-2.5.1/test/rml/json/RMLTC0008c/test_RMLTC0008c_JSON.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/json/RMLTC0009a/mapping.ttl` & `morph_kgc-2.5.1/test/rml/json/RMLTC0009a/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/json/RMLTC0009a/test_RMLTC0009a_JSON.py` & `morph_kgc-2.5.1/test/rml/json/RMLTC0009a/test_RMLTC0009a_JSON.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/json/RMLTC0009b/mapping.ttl` & `morph_kgc-2.5.1/test/rml/json/RMLTC0009b/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/json/RMLTC0009b/output.nq` & `morph_kgc-2.5.1/test/rml/json/RMLTC0009b/output.nq`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/json/RMLTC0009b/test_RMLTC0009b_JSON.py` & `morph_kgc-2.5.1/test/rml/json/RMLTC0009b/test_RMLTC0009b_JSON.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/json/RMLTC0010a/mapping.ttl` & `morph_kgc-2.5.1/test/rml/json/RMLTC0010a/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/json/RMLTC0010a/test_RMLTC0010a_JSON.py` & `morph_kgc-2.5.1/test/rml/json/RMLTC0010a/test_RMLTC0010a_JSON.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/json/RMLTC0010b/mapping.ttl` & `morph_kgc-2.5.1/test/rml/json/RMLTC0010b/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/json/RMLTC0010b/test_RMLTC0010b_JSON.py` & `morph_kgc-2.5.1/test/rml/json/RMLTC0010b/test_RMLTC0010b_JSON.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/json/RMLTC0010c/mapping.ttl` & `morph_kgc-2.5.1/test/rml/json/RMLTC0010c/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/json/RMLTC0010c/test_RMLTC0010c_JSON.py` & `morph_kgc-2.5.1/test/rml/json/RMLTC0010c/test_RMLTC0010c_JSON.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/json/RMLTC0011b/mapping.ttl` & `morph_kgc-2.5.1/test/rml/json/RMLTC0011b/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/json/RMLTC0011b/output.nq` & `morph_kgc-2.5.1/test/rml/json/RMLTC0011b/output.nq`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/json/RMLTC0011b/test_RMLTC0011b_JSON.py` & `morph_kgc-2.5.1/test/rml/json/RMLTC0011b/test_RMLTC0011b_JSON.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/json/RMLTC0012a/mapping.ttl` & `morph_kgc-2.5.1/test/rml/json/RMLTC0012a/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/json/RMLTC0012a/test_RMLTC0012a_JSON.py` & `morph_kgc-2.5.1/test/rml/json/RMLTC0012a/test_RMLTC0012a_JSON.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/json/RMLTC0012b/mapping.ttl` & `morph_kgc-2.5.1/test/rml/json/RMLTC0012b/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/json/RMLTC0012b/test_RMLTC0012b_JSON.py` & `morph_kgc-2.5.1/test/rml/json/RMLTC0012b/test_RMLTC0012b_JSON.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/json/RMLTC0012c/mapping.ttl` & `morph_kgc-2.5.1/test/rml/json/RMLTC0012c/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/json/RMLTC0012c/test_RMLTC0012c_JSON.py` & `morph_kgc-2.5.1/test/rml/json/RMLTC0012c/test_RMLTC0012c_JSON.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/json/RMLTC0012d/mapping.ttl` & `morph_kgc-2.5.1/test/rml/json/RMLTC0012d/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/json/RMLTC0012d/test_RMLTC0012d_JSON.py` & `morph_kgc-2.5.1/test/rml/json/RMLTC0012d/test_RMLTC0012d_JSON.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/json/RMLTC0013a/mapping.ttl` & `morph_kgc-2.5.1/test/rml/json/RMLTC0013a/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/json/RMLTC0013a/test_RMLTC0013a_JSON.py` & `morph_kgc-2.5.1/test/rml/json/RMLTC0013a/test_RMLTC0013a_JSON.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/json/RMLTC0015a/mapping.ttl` & `morph_kgc-2.5.1/test/rml/json/RMLTC0015a/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/json/RMLTC0015a/test_RMLTC0015a_JSON.py` & `morph_kgc-2.5.1/test/rml/json/RMLTC0015a/test_RMLTC0015a_JSON.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/json/RMLTC0015b/mapping.ttl` & `morph_kgc-2.5.1/test/rml/json/RMLTC0015b/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/json/RMLTC0015b/test_RMLTC0015b_JSON.py` & `morph_kgc-2.5.1/test/rml/json/RMLTC0015b/test_RMLTC0015b_JSON.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/json/RMLTC0019a/RMLTC0019a_JSON.py` & `morph_kgc-2.5.1/test/rml/json/RMLTC0019a/RMLTC0019a_JSON.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/json/RMLTC0019a/mapping.ttl` & `morph_kgc-2.5.1/test/rml/json/RMLTC0019a/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/json/RMLTC0019b/RMLTC0019b_JSON.py` & `morph_kgc-2.5.1/test/rml/json/RMLTC0019b/RMLTC0019b_JSON.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/json/RMLTC0019b/mapping.ttl` & `morph_kgc-2.5.1/test/rml/json/RMLTC0019b/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/json/RMLTC0020a/RMLTC0020a_JSON.py` & `morph_kgc-2.5.1/test/rml/json/RMLTC0020a/RMLTC0020a_JSON.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/json/RMLTC0020a/mapping.ttl` & `morph_kgc-2.5.1/test/rml/json/RMLTC0020a/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/json/RMLTC0020a/output.nq` & `morph_kgc-2.5.1/test/rml/json/RMLTC0020a/output.nq`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/json/RMLTC0020b/RMLTC0020b_JSON.py` & `morph_kgc-2.5.1/test/rml/json/RMLTC0020b/RMLTC0020b_JSON.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/json/RMLTC0020b/mapping.ttl` & `morph_kgc-2.5.1/test/rml/json/RMLTC0020b/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/json/complex/data.json` & `morph_kgc-2.5.1/test/rml/json/complex/data.json`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/json/complex/mapping.ttl` & `morph_kgc-2.5.1/test/rml/json/complex/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/json/complex/mapping.yaml` & `morph_kgc-2.5.1/test/rml/json/complex/mapping.yaml`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/json/complex/output.nq` & `morph_kgc-2.5.1/test/rml/json/complex/output.nq`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/json/complex/test_complex_JSON.py` & `morph_kgc-2.5.1/test/rml/json/complex/test_complex_JSON.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/tabular/RMLTC0002a_EXCEL/mapping.ttl` & `morph_kgc-2.5.1/test/rml/tabular/RMLTC0002a_EXCEL/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/tabular/RMLTC0002a_EXCEL/student.xlsx` & `morph_kgc-2.5.1/test/rml/tabular/RMLTC0002a_EXCEL/student.xlsx`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/tabular/RMLTC0002a_EXCEL/test_RMLTC0002a_EXCEL.py` & `morph_kgc-2.5.1/test/rml/tabular/RMLTC0002a_EXCEL/test_RMLTC0002a_EXCEL.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/tabular/RMLTC0002a_FEATHER/mapping.ttl` & `morph_kgc-2.5.1/test/rml/tabular/RMLTC0002a_FEATHER/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/tabular/RMLTC0002a_FEATHER/student.feather` & `morph_kgc-2.5.1/test/rml/tabular/RMLTC0002a_FEATHER/student.feather`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/tabular/RMLTC0002a_FEATHER/test_RMLTC0002a_FEATHER.py` & `morph_kgc-2.5.1/test/rml/tabular/RMLTC0002a_FEATHER/test_RMLTC0002a_FEATHER.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/tabular/RMLTC0002a_ODS/mapping.ttl` & `morph_kgc-2.5.1/test/rml/tabular/RMLTC0002a_ODS/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/tabular/RMLTC0002a_ODS/student.ods` & `morph_kgc-2.5.1/test/rml/tabular/RMLTC0002a_ODS/student.ods`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/tabular/RMLTC0002a_ODS/test_RMLTC0002a_ODS.py` & `morph_kgc-2.5.1/test/rml/tabular/RMLTC0002a_ODS/test_RMLTC0002a_ODS.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/tabular/RMLTC0002a_PARQUET/mapping.ttl` & `morph_kgc-2.5.1/test/rml/tabular/RMLTC0002a_PARQUET/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/tabular/RMLTC0002a_PARQUET/student.parquet` & `morph_kgc-2.5.1/test/rml/tabular/RMLTC0002a_PARQUET/student.parquet`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/tabular/RMLTC0002a_PARQUET/test_RMLTC0002a_PARQUET.py` & `morph_kgc-2.5.1/test/rml/tabular/RMLTC0002a_PARQUET/test_RMLTC0002a_PARQUET.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/tabular/RMLTC0002a_STATA/mapping.ttl` & `morph_kgc-2.5.1/test/rml/tabular/RMLTC0002a_STATA/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/tabular/RMLTC0002a_STATA/student.dta` & `morph_kgc-2.5.1/test/rml/tabular/RMLTC0002a_STATA/student.dta`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/tabular/RMLTC0002a_STATA/test_RMLTC0002a_STATA.py` & `morph_kgc-2.5.1/test/rml/tabular/RMLTC0002a_STATA/test_RMLTC0002a_STATA.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/tabular/RMLTC0002a_TSV/mapping.ttl` & `morph_kgc-2.5.1/test/rml/tabular/RMLTC0002a_TSV/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/tabular/RMLTC0002a_TSV/test_RMLTC0002a_TSV.py` & `morph_kgc-2.5.1/test/rml/tabular/RMLTC0002a_TSV/test_RMLTC0002a_TSV.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/xml/RMLTC0000/mapping.ttl` & `morph_kgc-2.5.1/test/rml/xml/RMLTC0000/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/xml/RMLTC0000/test_RMLTC0000_XML.py` & `morph_kgc-2.5.1/test/rml/xml/RMLTC0000/test_RMLTC0000_XML.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/xml/RMLTC0001a/mapping.ttl` & `morph_kgc-2.5.1/test/rml/xml/RMLTC0001a/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/xml/RMLTC0001a/test_RMLTC0001a_XML.py` & `morph_kgc-2.5.1/test/rml/xml/RMLTC0001a/test_RMLTC0001a_XML.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/xml/RMLTC0001b/mapping.ttl` & `morph_kgc-2.5.1/test/rml/xml/RMLTC0001b/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/xml/RMLTC0001b/test_RMLTC0001b_XML.py` & `morph_kgc-2.5.1/test/rml/xml/RMLTC0001b/test_RMLTC0001b_XML.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/xml/RMLTC0002a/mapping.ttl` & `morph_kgc-2.5.1/test/rml/xml/RMLTC0002a/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/xml/RMLTC0002a/test_RMLTC0002a_XML.py` & `morph_kgc-2.5.1/test/rml/xml/RMLTC0002a/test_RMLTC0002a_XML.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/xml/RMLTC0002b/mapping.ttl` & `morph_kgc-2.5.1/test/rml/xml/RMLTC0002b/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/xml/RMLTC0002b/test_RMLTC0002b_XML.py` & `morph_kgc-2.5.1/test/rml/xml/RMLTC0002b/test_RMLTC0002b_XML.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/xml/RMLTC0002c/mapping.ttl` & `morph_kgc-2.5.1/test/rml/xml/RMLTC0002c/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/xml/RMLTC0002c/test_RMLTC0002c_XML.py` & `morph_kgc-2.5.1/test/rml/xml/RMLTC0002c/test_RMLTC0002c_XML.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/xml/RMLTC0002e/mapping.ttl` & `morph_kgc-2.5.1/test/rml/xml/RMLTC0002e/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/xml/RMLTC0002e/test_RMLTC0002e_XML.py` & `morph_kgc-2.5.1/test/rml/xml/RMLTC0002e/test_RMLTC0002e_XML.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/xml/RMLTC0003c/mapping.ttl` & `morph_kgc-2.5.1/test/rml/xml/RMLTC0003c/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/xml/RMLTC0003c/test_RMLTC0003c_XML.py` & `morph_kgc-2.5.1/test/rml/xml/RMLTC0003c/test_RMLTC0003c_XML.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/xml/RMLTC0004a/mapping.ttl` & `morph_kgc-2.5.1/test/rml/xml/RMLTC0004a/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/xml/RMLTC0004a/test_RMLTC0004a_XML.py` & `morph_kgc-2.5.1/test/rml/xml/RMLTC0004a/test_RMLTC0004a_XML.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/xml/RMLTC0004b/mapping.ttl` & `morph_kgc-2.5.1/test/rml/xml/RMLTC0004b/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/xml/RMLTC0004b/test_RMLTC0004b_XML.py` & `morph_kgc-2.5.1/test/rml/xml/RMLTC0004b/test_RMLTC0004b_XML.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/xml/RMLTC0005a/mapping.ttl` & `morph_kgc-2.5.1/test/rml/xml/RMLTC0005a/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/xml/RMLTC0005a/test_RMLTC0005a_XML.py` & `morph_kgc-2.5.1/test/rml/xml/RMLTC0005a/test_RMLTC0005a_XML.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/xml/RMLTC0006a/mapping.ttl` & `morph_kgc-2.5.1/test/rml/xml/RMLTC0006a/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/xml/RMLTC0006a/test_RMLTC0006a_XML.py` & `morph_kgc-2.5.1/test/rml/xml/RMLTC0006a/test_RMLTC0006a_XML.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/xml/RMLTC0007a/mapping.ttl` & `morph_kgc-2.5.1/test/rml/xml/RMLTC0007a/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/xml/RMLTC0007a/test_RMLTC0007a_XML.py` & `morph_kgc-2.5.1/test/rml/xml/RMLTC0007a/test_RMLTC0007a_XML.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/xml/RMLTC0007b/mapping.ttl` & `morph_kgc-2.5.1/test/rml/xml/RMLTC0007b/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/xml/RMLTC0007b/test_RMLTC0007b_XML.py` & `morph_kgc-2.5.1/test/rml/xml/RMLTC0007b/test_RMLTC0007b_XML.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/xml/RMLTC0007c/mapping.ttl` & `morph_kgc-2.5.1/test/rml/xml/RMLTC0007c/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/xml/RMLTC0007c/test_RMLTC0007c_XML.py` & `morph_kgc-2.5.1/test/rml/xml/RMLTC0007c/test_RMLTC0007c_XML.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/xml/RMLTC0007d/mapping.ttl` & `morph_kgc-2.5.1/test/rml/xml/RMLTC0007d/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/xml/RMLTC0007d/test_RMLTC0007d_XML.py` & `morph_kgc-2.5.1/test/rml/xml/RMLTC0007d/test_RMLTC0007d_XML.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/xml/RMLTC0007e/mapping.ttl` & `morph_kgc-2.5.1/test/rml/xml/RMLTC0007e/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/xml/RMLTC0007e/test_RMLTC0007e_XML.py` & `morph_kgc-2.5.1/test/rml/xml/RMLTC0007e/test_RMLTC0007e_XML.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/xml/RMLTC0007f/mapping.ttl` & `morph_kgc-2.5.1/test/rml/xml/RMLTC0007f/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/xml/RMLTC0007f/test_RMLTC0007f_XML.py` & `morph_kgc-2.5.1/test/rml/xml/RMLTC0007f/test_RMLTC0007f_XML.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/xml/RMLTC0007g/mapping.ttl` & `morph_kgc-2.5.1/test/rml/xml/RMLTC0007g/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/xml/RMLTC0007g/test_RMLTC0007g_XML.py` & `morph_kgc-2.5.1/test/rml/xml/RMLTC0007g/test_RMLTC0007g_XML.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/xml/RMLTC0007h/mapping.ttl` & `morph_kgc-2.5.1/test/rml/xml/RMLTC0007h/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/xml/RMLTC0007h/test_RMLTC0007h_XML.py` & `morph_kgc-2.5.1/test/rml/xml/RMLTC0007h/test_RMLTC0007h_XML.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/xml/RMLTC0008a/mapping.ttl` & `morph_kgc-2.5.1/test/rml/xml/RMLTC0008a/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/xml/RMLTC0008a/output.nq` & `morph_kgc-2.5.1/test/rml/xml/RMLTC0008a/output.nq`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/xml/RMLTC0008a/test_RMLTC0008a_XML.py` & `morph_kgc-2.5.1/test/rml/xml/RMLTC0008a/test_RMLTC0008a_XML.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/xml/RMLTC0008b/mapping.ttl` & `morph_kgc-2.5.1/test/rml/xml/RMLTC0008b/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/xml/RMLTC0008b/output.nq` & `morph_kgc-2.5.1/test/rml/xml/RMLTC0008b/output.nq`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/xml/RMLTC0008b/test_RMLTC0008b_XML.py` & `morph_kgc-2.5.1/test/rml/xml/RMLTC0008b/test_RMLTC0008b_XML.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/xml/RMLTC0008c/mapping.ttl` & `morph_kgc-2.5.1/test/rml/xml/RMLTC0008c/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/xml/RMLTC0008c/test_RMLTC0008c_XML.py` & `morph_kgc-2.5.1/test/rml/xml/RMLTC0008c/test_RMLTC0008c_XML.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/xml/RMLTC0009a/mapping.ttl` & `morph_kgc-2.5.1/test/rml/xml/RMLTC0009a/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/xml/RMLTC0009a/test_RMLTC0009a_XML.py` & `morph_kgc-2.5.1/test/rml/xml/RMLTC0009a/test_RMLTC0009a_XML.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/xml/RMLTC0009b/mapping.ttl` & `morph_kgc-2.5.1/test/rml/xml/RMLTC0009b/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/xml/RMLTC0009b/output.nq` & `morph_kgc-2.5.1/test/rml/xml/RMLTC0009b/output.nq`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/xml/RMLTC0009b/test_RMLTC0009b_XML.py` & `morph_kgc-2.5.1/test/rml/xml/RMLTC0009b/test_RMLTC0009b_XML.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/xml/RMLTC0010b/mapping.ttl` & `morph_kgc-2.5.1/test/rml/xml/RMLTC0010b/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/xml/RMLTC0010b/test_RMLTC0010b_XML.py` & `morph_kgc-2.5.1/test/rml/xml/RMLTC0010b/test_RMLTC0010b_XML.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/xml/RMLTC0010c/mapping.ttl` & `morph_kgc-2.5.1/test/rml/xml/RMLTC0010c/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/xml/RMLTC0010c/test_RMLTC0010c_XML.py` & `morph_kgc-2.5.1/test/rml/xml/RMLTC0010c/test_RMLTC0010c_XML.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/xml/RMLTC0011b/mapping.ttl` & `morph_kgc-2.5.1/test/rml/xml/RMLTC0011b/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/xml/RMLTC0011b/output.nq` & `morph_kgc-2.5.1/test/rml/xml/RMLTC0011b/output.nq`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/xml/RMLTC0011b/test_RMLTC0011b_XML.py` & `morph_kgc-2.5.1/test/rml/xml/RMLTC0011b/test_RMLTC0011b_XML.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/xml/RMLTC0012a/mapping.ttl` & `morph_kgc-2.5.1/test/rml/xml/RMLTC0012a/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/xml/RMLTC0012a/test_RMLTC0012a_XML.py` & `morph_kgc-2.5.1/test/rml/xml/RMLTC0012a/test_RMLTC0012a_XML.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/xml/RMLTC0012b/mapping.ttl` & `morph_kgc-2.5.1/test/rml/xml/RMLTC0012b/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/xml/RMLTC0012b/test_RMLTC0012b_XML.py` & `morph_kgc-2.5.1/test/rml/xml/RMLTC0012b/test_RMLTC0012b_XML.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/xml/RMLTC0012c/mapping.ttl` & `morph_kgc-2.5.1/test/rml/xml/RMLTC0012c/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/xml/RMLTC0012c/test_RMLTC0012c_XML.py` & `morph_kgc-2.5.1/test/rml/xml/RMLTC0012c/test_RMLTC0012c_XML.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/xml/RMLTC0012d/mapping.ttl` & `morph_kgc-2.5.1/test/rml/xml/RMLTC0012d/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/xml/RMLTC0012d/test_RMLTC0012d_XML.py` & `morph_kgc-2.5.1/test/rml/xml/RMLTC0012d/test_RMLTC0012d_XML.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/xml/RMLTC0015a/mapping.ttl` & `morph_kgc-2.5.1/test/rml/xml/RMLTC0015a/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/xml/RMLTC0015a/test_RMLTC0015a_XML.py` & `morph_kgc-2.5.1/test/rml/xml/RMLTC0015a/test_RMLTC0015a_XML.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/xml/RMLTC0015b/mapping.ttl` & `morph_kgc-2.5.1/test/rml/xml/RMLTC0015b/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/xml/RMLTC0015b/test_RMLTC0015b_XML.py` & `morph_kgc-2.5.1/test/rml/xml/RMLTC0015b/test_RMLTC0015b_XML.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/xml/RMLTC0019a/RMLTC0019a_XML.py` & `morph_kgc-2.5.1/test/rml/xml/RMLTC0019a/RMLTC0019a_XML.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/xml/RMLTC0019a/mapping.ttl` & `morph_kgc-2.5.1/test/rml/xml/RMLTC0019a/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/xml/RMLTC0019b/RMLTC0019b_XML.py` & `morph_kgc-2.5.1/test/rml/xml/RMLTC0019b/RMLTC0019b_XML.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/xml/RMLTC0019b/mapping.ttl` & `morph_kgc-2.5.1/test/rml/xml/RMLTC0019b/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/xml/RMLTC0020a/RMLTC0020a_XML.py` & `morph_kgc-2.5.1/test/rml/xml/RMLTC0020a/RMLTC0020a_XML.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/xml/RMLTC0020a/mapping.ttl` & `morph_kgc-2.5.1/test/rml/xml/RMLTC0020a/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/xml/RMLTC0020a/output.nq` & `morph_kgc-2.5.1/test/rml/xml/RMLTC0020a/output.nq`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/xml/RMLTC0020b/RMLTC0020b_XML.py` & `morph_kgc-2.5.1/test/rml/xml/RMLTC0020b/RMLTC0020b_XML.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/xml/RMLTC0020b/mapping.ttl` & `morph_kgc-2.5.1/test/rml/xml/RMLTC0020b/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/xml/attributes/data.xml` & `morph_kgc-2.5.1/test/rml/xml/attributes/data.xml`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/xml/attributes/mapping.ttl` & `morph_kgc-2.5.1/test/rml/xml/attributes/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/xml/attributes/output.nq` & `morph_kgc-2.5.1/test/rml/xml/attributes/output.nq`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/xml/attributes/test_attributes_XML.py` & `morph_kgc-2.5.1/test/rml/xml/attributes/test_attributes_XML.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/xml/complex/data.xml` & `morph_kgc-2.5.1/test/rml/xml/complex/data.xml`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/xml/complex/mapping.ttl` & `morph_kgc-2.5.1/test/rml/xml/complex/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/xml/complex/mapping.yaml` & `morph_kgc-2.5.1/test/rml/xml/complex/mapping.yaml`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/xml/complex/output.nq` & `morph_kgc-2.5.1/test/rml/xml/complex/output.nq`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/xml/complex/test_complex_XML.py` & `morph_kgc-2.5.1/test/rml/xml/complex/test_complex_XML.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/xml/rml_spec_example_section_3/mapping.ttl` & `morph_kgc-2.5.1/test/rml/xml/rml_spec_example_section_3/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/xml/rml_spec_example_section_3/output.nq` & `morph_kgc-2.5.1/test/rml/xml/rml_spec_example_section_3/output.nq`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/xml/rml_spec_example_section_3/test_rml_spec_example_section_3_XML.py` & `morph_kgc-2.5.1/test/rml/xml/rml_spec_example_section_3/test_rml_spec_example_section_3_XML.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/xml/rml_spec_example_section_5/mapping.ttl` & `morph_kgc-2.5.1/test/rml/xml/rml_spec_example_section_5/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/xml/rml_spec_example_section_5/output.nq` & `morph_kgc-2.5.1/test/rml/xml/rml_spec_example_section_5/output.nq`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml/xml/rml_spec_example_section_5/test_rml_spec_example_section_5_XML.py` & `morph_kgc-2.5.1/test/rml/xml/rml_spec_example_section_5/test_rml_spec_example_section_5_XML.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml-in-memory/json_dictionary/RMLIMTC0000/mapping.ttl` & `morph_kgc-2.5.1/test/rml-in-memory/json_dictionary/RMLIMTC0000/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml-in-memory/json_dictionary/RMLIMTC0000/test_RMLTC0000_DICT.py` & `morph_kgc-2.5.1/test/rml-in-memory/json_dictionary/RMLIMTC0000/test_RMLTC0000_DICT.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml-in-memory/json_dictionary/RMLIMTC0001a/mapping.ttl` & `morph_kgc-2.5.1/test/rml-in-memory/json_dictionary/RMLIMTC0001a/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml-in-memory/json_dictionary/RMLIMTC0001a/test_RMLTC0001a_DICT.py` & `morph_kgc-2.5.1/test/rml-in-memory/json_dictionary/RMLIMTC0001a/test_RMLTC0001a_DICT.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml-in-memory/json_dictionary/RMLIMTC0001b/mapping.ttl` & `morph_kgc-2.5.1/test/rml-in-memory/json_dictionary/RMLIMTC0001b/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml-in-memory/json_dictionary/RMLIMTC0001b/test_RMLTC0001b_DICT.py` & `morph_kgc-2.5.1/test/rml-in-memory/json_dictionary/RMLIMTC0001b/test_RMLTC0001b_DICT.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml-in-memory/json_dictionary/RMLIMTC0002a/mapping.ttl` & `morph_kgc-2.5.1/test/rml-in-memory/json_dictionary/RMLIMTC0002a/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml-in-memory/json_dictionary/RMLIMTC0002a/test_RMLTC0002a_DICT.py` & `morph_kgc-2.5.1/test/rml-in-memory/json_dictionary/RMLIMTC0002a/test_RMLTC0002a_DICT.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml-in-memory/json_dictionary/RMLIMTC0002b/mapping.ttl` & `morph_kgc-2.5.1/test/rml-in-memory/json_dictionary/RMLIMTC0002b/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml-in-memory/json_dictionary/RMLIMTC0002b/test_RMLTC0002b_DICT.py` & `morph_kgc-2.5.1/test/rml-in-memory/json_dictionary/RMLIMTC0002b/test_RMLTC0002b_DICT.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml-in-memory/json_dictionary/RMLIMTC0002c/mapping.ttl` & `morph_kgc-2.5.1/test/rml-in-memory/json_dictionary/RMLIMTC0002c/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml-in-memory/json_dictionary/RMLIMTC0002c/test_RMLTC0002c_DICT.py` & `morph_kgc-2.5.1/test/rml-in-memory/json_dictionary/RMLIMTC0002c/test_RMLTC0002c_DICT.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml-in-memory/json_dictionary/RMLIMTC0002e/mapping.ttl` & `morph_kgc-2.5.1/test/rml-in-memory/json_dictionary/RMLIMTC0002e/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml-in-memory/json_dictionary/RMLIMTC0002e/test_RMLTC0002e_DICT.py` & `morph_kgc-2.5.1/test/rml-in-memory/json_dictionary/RMLIMTC0002e/test_RMLTC0002e_DICT.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml-in-memory/json_dictionary/RMLIMTC0003c/mapping.ttl` & `morph_kgc-2.5.1/test/rml-in-memory/json_dictionary/RMLIMTC0003c/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml-in-memory/json_dictionary/RMLIMTC0003c/test_RMLTC0003c_DICT.py` & `morph_kgc-2.5.1/test/rml-in-memory/json_dictionary/RMLIMTC0003c/test_RMLTC0003c_DICT.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml-in-memory/json_dictionary/RMLIMTC0004a/mapping.ttl` & `morph_kgc-2.5.1/test/rml-in-memory/json_dictionary/RMLIMTC0004a/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml-in-memory/json_dictionary/RMLIMTC0004a/test_RMLTC0004a_DICT.py` & `morph_kgc-2.5.1/test/rml-in-memory/json_dictionary/RMLIMTC0004a/test_RMLTC0004a_DICT.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml-in-memory/json_dictionary/RMLIMTC0004b/mapping.ttl` & `morph_kgc-2.5.1/test/rml-in-memory/json_dictionary/RMLIMTC0004b/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml-in-memory/json_dictionary/RMLIMTC0004b/test_RMLTC0004b_DICT.py` & `morph_kgc-2.5.1/test/rml-in-memory/json_dictionary/RMLIMTC0004b/test_RMLTC0004b_DICT.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml-in-memory/json_dictionary/RMLIMTC0005a/mapping.ttl` & `morph_kgc-2.5.1/test/rml-in-memory/json_dictionary/RMLIMTC0005a/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml-in-memory/json_dictionary/RMLIMTC0005a/test_RMLTC0005a_DICT.py` & `morph_kgc-2.5.1/test/rml-in-memory/json_dictionary/RMLIMTC0005a/test_RMLTC0005a_DICT.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml-in-memory/json_dictionary/RMLIMTC0006a/mapping.ttl` & `morph_kgc-2.5.1/test/rml-in-memory/json_dictionary/RMLIMTC0006a/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml-in-memory/json_dictionary/RMLIMTC0006a/test_RMLTC0006a_DICT.py` & `morph_kgc-2.5.1/test/rml-in-memory/json_dictionary/RMLIMTC0006a/test_RMLTC0006a_DICT.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml-in-memory/json_dictionary/RMLIMTC0007a/mapping.ttl` & `morph_kgc-2.5.1/test/rml-in-memory/json_dictionary/RMLIMTC0007a/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml-in-memory/json_dictionary/RMLIMTC0007a/test_RMLTC0007a_DICT.py` & `morph_kgc-2.5.1/test/rml-in-memory/json_dictionary/RMLIMTC0007a/test_RMLTC0007a_DICT.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml-in-memory/json_dictionary/RMLIMTC0007b/mapping.ttl` & `morph_kgc-2.5.1/test/rml-in-memory/json_dictionary/RMLIMTC0007b/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml-in-memory/json_dictionary/RMLIMTC0007b/test_RMLTC0007b_DICT.py` & `morph_kgc-2.5.1/test/rml-in-memory/json_dictionary/RMLIMTC0007b/test_RMLTC0007b_DICT.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml-in-memory/json_dictionary/RMLIMTC0007c/mapping.ttl` & `morph_kgc-2.5.1/test/rml-in-memory/json_dictionary/RMLIMTC0007c/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml-in-memory/json_dictionary/RMLIMTC0007c/test_RMLTC0007c_DICT.py` & `morph_kgc-2.5.1/test/rml-in-memory/json_dictionary/RMLIMTC0007c/test_RMLTC0007c_DICT.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml-in-memory/json_dictionary/RMLIMTC0007d/mapping.ttl` & `morph_kgc-2.5.1/test/rml-in-memory/json_dictionary/RMLIMTC0007d/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml-in-memory/json_dictionary/RMLIMTC0007d/test_RMLTC0007d_DICT.py` & `morph_kgc-2.5.1/test/rml-in-memory/json_dictionary/RMLIMTC0007d/test_RMLTC0007d_DICT.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml-in-memory/json_dictionary/RMLIMTC0007e/mapping.ttl` & `morph_kgc-2.5.1/test/rml-in-memory/json_dictionary/RMLIMTC0007e/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml-in-memory/json_dictionary/RMLIMTC0007e/test_RMLTC0007e_DICT.py` & `morph_kgc-2.5.1/test/rml-in-memory/json_dictionary/RMLIMTC0007e/test_RMLTC0007e_DICT.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml-in-memory/json_dictionary/RMLIMTC0007f/mapping.ttl` & `morph_kgc-2.5.1/test/rml-in-memory/json_dictionary/RMLIMTC0007f/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml-in-memory/json_dictionary/RMLIMTC0007f/test_RMLTC0007f_DICT.py` & `morph_kgc-2.5.1/test/rml-in-memory/json_dictionary/RMLIMTC0007f/test_RMLTC0007f_DICT.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml-in-memory/json_dictionary/RMLIMTC0007g/mapping.ttl` & `morph_kgc-2.5.1/test/rml-in-memory/json_dictionary/RMLIMTC0007g/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml-in-memory/json_dictionary/RMLIMTC0007g/test_RMLTC0007g_DICT.py` & `morph_kgc-2.5.1/test/rml-in-memory/json_dictionary/RMLIMTC0007g/test_RMLTC0007g_DICT.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml-in-memory/json_dictionary/RMLIMTC0007h/mapping.ttl` & `morph_kgc-2.5.1/test/rml-in-memory/json_dictionary/RMLIMTC0007h/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml-in-memory/json_dictionary/RMLIMTC0007h/test_RMLTC0007h_DICT.py` & `morph_kgc-2.5.1/test/rml-in-memory/json_dictionary/RMLIMTC0007h/test_RMLTC0007h_DICT.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml-in-memory/json_dictionary/RMLIMTC0008a/mapping.ttl` & `morph_kgc-2.5.1/test/rml-in-memory/json_dictionary/RMLIMTC0008a/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml-in-memory/json_dictionary/RMLIMTC0008a/output.nq` & `morph_kgc-2.5.1/test/rml-in-memory/json_dictionary/RMLIMTC0008a/output.nq`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml-in-memory/json_dictionary/RMLIMTC0008a/test_RMLTC0008a_DICT.py` & `morph_kgc-2.5.1/test/rml-in-memory/json_dictionary/RMLIMTC0008a/test_RMLTC0008a_DICT.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml-in-memory/json_dictionary/RMLIMTC0008b/mapping.ttl` & `morph_kgc-2.5.1/test/rml-in-memory/json_dictionary/RMLIMTC0008b/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml-in-memory/json_dictionary/RMLIMTC0008b/output.nq` & `morph_kgc-2.5.1/test/rml-in-memory/json_dictionary/RMLIMTC0008b/output.nq`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml-in-memory/json_dictionary/RMLIMTC0008b/test_RMLTC0008b_DICT.py` & `morph_kgc-2.5.1/test/rml-in-memory/json_dictionary/RMLIMTC0008b/test_RMLTC0008b_DICT.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml-in-memory/json_dictionary/RMLIMTC0008c/mapping.ttl` & `morph_kgc-2.5.1/test/rml-in-memory/json_dictionary/RMLIMTC0008c/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml-in-memory/json_dictionary/RMLIMTC0008c/test_RMLTC0008c_DICT.py` & `morph_kgc-2.5.1/test/rml-in-memory/json_dictionary/RMLIMTC0008c/test_RMLTC0008c_DICT.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml-in-memory/json_dictionary/RMLIMTC0009a/mapping.ttl` & `morph_kgc-2.5.1/test/rml-in-memory/json_dictionary/RMLIMTC0009a/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml-in-memory/json_dictionary/RMLIMTC0009a/test_RMLTC0009a_DICT.py` & `morph_kgc-2.5.1/test/rml-in-memory/json_dictionary/RMLIMTC0009a/test_RMLTC0009a_DICT.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml-in-memory/json_dictionary/RMLIMTC0009b/mapping.ttl` & `morph_kgc-2.5.1/test/rml-in-memory/json_dictionary/RMLIMTC0009b/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml-in-memory/json_dictionary/RMLIMTC0009b/output.nq` & `morph_kgc-2.5.1/test/rml-in-memory/json_dictionary/RMLIMTC0009b/output.nq`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml-in-memory/json_dictionary/RMLIMTC0009b/test_RMLTC0009b_DICT.py` & `morph_kgc-2.5.1/test/rml-in-memory/json_dictionary/RMLIMTC0009b/test_RMLTC0009b_DICT.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml-in-memory/json_dictionary/RMLIMTC0010a/mapping.ttl` & `morph_kgc-2.5.1/test/rml-in-memory/json_dictionary/RMLIMTC0010a/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml-in-memory/json_dictionary/RMLIMTC0010a/test_RMLTC0010a_DICT.py` & `morph_kgc-2.5.1/test/rml-in-memory/json_dictionary/RMLIMTC0010a/test_RMLTC0010a_DICT.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml-in-memory/json_dictionary/RMLIMTC0010b/mapping.ttl` & `morph_kgc-2.5.1/test/rml-in-memory/json_dictionary/RMLIMTC0010b/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml-in-memory/json_dictionary/RMLIMTC0010b/test_RMLTC0010b_DICT.py` & `morph_kgc-2.5.1/test/rml-in-memory/json_dictionary/RMLIMTC0010b/test_RMLTC0010b_DICT.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml-in-memory/json_dictionary/RMLIMTC0010c/mapping.ttl` & `morph_kgc-2.5.1/test/rml-in-memory/json_dictionary/RMLIMTC0010c/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml-in-memory/json_dictionary/RMLIMTC0010c/test_RMLTC0010c_DICT.py` & `morph_kgc-2.5.1/test/rml-in-memory/json_dictionary/RMLIMTC0010c/test_RMLTC0010c_DICT.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml-in-memory/json_dictionary/RMLIMTC0011b/mapping.ttl` & `morph_kgc-2.5.1/test/rml-in-memory/json_dictionary/RMLIMTC0011b/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml-in-memory/json_dictionary/RMLIMTC0011b/output.nq` & `morph_kgc-2.5.1/test/rml-in-memory/json_dictionary/RMLIMTC0011b/output.nq`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml-in-memory/json_dictionary/RMLIMTC0011b/test_RMLTC0011b_DICT.py` & `morph_kgc-2.5.1/test/rml-in-memory/json_dictionary/RMLIMTC0011b/test_RMLTC0011b_DICT.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml-in-memory/json_dictionary/RMLIMTC0012a/mapping.ttl` & `morph_kgc-2.5.1/test/rml-in-memory/json_dictionary/RMLIMTC0012a/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml-in-memory/json_dictionary/RMLIMTC0012a/test_RMLTC0012a_DICT.py` & `morph_kgc-2.5.1/test/rml-in-memory/json_dictionary/RMLIMTC0012a/test_RMLTC0012a_DICT.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml-in-memory/json_dictionary/RMLIMTC0012b/mapping.ttl` & `morph_kgc-2.5.1/test/rml-in-memory/json_dictionary/RMLIMTC0012b/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml-in-memory/json_dictionary/RMLIMTC0012b/test_RMLTC0012b_DICT.py` & `morph_kgc-2.5.1/test/rml-in-memory/json_dictionary/RMLIMTC0012b/test_RMLTC0012b_DICT.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml-in-memory/json_dictionary/RMLIMTC0012c/mapping.ttl` & `morph_kgc-2.5.1/test/rml-in-memory/json_dictionary/RMLIMTC0012c/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml-in-memory/json_dictionary/RMLIMTC0012c/test_RMLTC0012c_DICT.py` & `morph_kgc-2.5.1/test/rml-in-memory/json_dictionary/RMLIMTC0012c/test_RMLTC0012c_DICT.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml-in-memory/json_dictionary/RMLIMTC0012d/mapping.ttl` & `morph_kgc-2.5.1/test/rml-in-memory/json_dictionary/RMLIMTC0012d/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml-in-memory/json_dictionary/RMLIMTC0012d/test_RMLTC0012d_DICT.py` & `morph_kgc-2.5.1/test/rml-in-memory/json_dictionary/RMLIMTC0012d/test_RMLTC0012d_DICT.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml-in-memory/json_dictionary/RMLIMTC0013a/mapping.ttl` & `morph_kgc-2.5.1/test/rml-in-memory/json_dictionary/RMLIMTC0013a/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml-in-memory/json_dictionary/RMLIMTC0013a/test_RMLTC0013a_DICT.py` & `morph_kgc-2.5.1/test/rml-in-memory/json_dictionary/RMLIMTC0013a/test_RMLTC0013a_DICT.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml-in-memory/json_dictionary/RMLIMTC0015a/mapping.ttl` & `morph_kgc-2.5.1/test/rml-in-memory/json_dictionary/RMLIMTC0015a/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml-in-memory/json_dictionary/RMLIMTC0015a/test_RMLTC0015a_DICT.py` & `morph_kgc-2.5.1/test/rml-in-memory/json_dictionary/RMLIMTC0015a/test_RMLTC0015a_DICT.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml-in-memory/json_dictionary/RMLIMTC0015b/mapping.ttl` & `morph_kgc-2.5.1/test/rml-in-memory/json_dictionary/RMLIMTC0015b/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml-in-memory/json_dictionary/RMLIMTC0015b/test_RMLTC0015b_DICT.py` & `morph_kgc-2.5.1/test/rml-in-memory/json_dictionary/RMLIMTC0015b/test_RMLTC0015b_DICT.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0000/mapping.ttl` & `morph_kgc-2.5.1/test/rml-in-memory/pandas_dataframe/RMLIMTC0000/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0000/test_RMLIMTC0000_DF.py` & `morph_kgc-2.5.1/test/rml-in-memory/pandas_dataframe/RMLIMTC0000/test_RMLIMTC0000_DF.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0001a/mapping.ttl` & `morph_kgc-2.5.1/test/rml-in-memory/pandas_dataframe/RMLIMTC0001a/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0001a/test_RMLTC0001a_DF.py` & `morph_kgc-2.5.1/test/rml-in-memory/pandas_dataframe/RMLIMTC0001a/test_RMLTC0001a_DF.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0001b/mapping.ttl` & `morph_kgc-2.5.1/test/rml-in-memory/pandas_dataframe/RMLIMTC0001b/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0001b/test_RMLIMTC0001b_DF.py` & `morph_kgc-2.5.1/test/rml-in-memory/pandas_dataframe/RMLIMTC0001b/test_RMLIMTC0001b_DF.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0002a/mapping.ttl` & `morph_kgc-2.5.1/test/rml-in-memory/pandas_dataframe/RMLIMTC0002a/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0002a/test_RMLIMTC0002a_DF.py` & `morph_kgc-2.5.1/test/rml-in-memory/pandas_dataframe/RMLIMTC0002a/test_RMLIMTC0002a_DF.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0002b/mapping.ttl` & `morph_kgc-2.5.1/test/rml-in-memory/pandas_dataframe/RMLIMTC0002b/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0002b/test_RMLIMTC0002b_DF.py` & `morph_kgc-2.5.1/test/rml-in-memory/pandas_dataframe/RMLIMTC0002b/test_RMLIMTC0002b_DF.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0002c/mapping.ttl` & `morph_kgc-2.5.1/test/rml-in-memory/pandas_dataframe/RMLIMTC0002c/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0002c/test_RMLIMTC0002c_DF.py` & `morph_kgc-2.5.1/test/rml-in-memory/pandas_dataframe/RMLIMTC0002c/test_RMLIMTC0002c_DF.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0002e/mapping.ttl` & `morph_kgc-2.5.1/test/rml-in-memory/pandas_dataframe/RMLIMTC0002e/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0002e/test_RMLIMTC0002e_DF.py` & `morph_kgc-2.5.1/test/rml-in-memory/pandas_dataframe/RMLIMTC0002e/test_RMLIMTC0002e_DF.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0003c/mapping.ttl` & `morph_kgc-2.5.1/test/rml-in-memory/pandas_dataframe/RMLIMTC0003c/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0003c/test_RMLIMTC0003c_DF.py` & `morph_kgc-2.5.1/test/rml-in-memory/pandas_dataframe/RMLIMTC0003c/test_RMLIMTC0003c_DF.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0004a/mapping.ttl` & `morph_kgc-2.5.1/test/rml-in-memory/pandas_dataframe/RMLIMTC0004a/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0004a/test_RMLIMTC0004a_DF.py` & `morph_kgc-2.5.1/test/rml-in-memory/pandas_dataframe/RMLIMTC0004a/test_RMLIMTC0004a_DF.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0004b/mapping.ttl` & `morph_kgc-2.5.1/test/rml-in-memory/pandas_dataframe/RMLIMTC0004b/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0004b/test_RMLIMTC0004b_DF.py` & `morph_kgc-2.5.1/test/rml-in-memory/pandas_dataframe/RMLIMTC0004b/test_RMLIMTC0004b_DF.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0005a/mapping.ttl` & `morph_kgc-2.5.1/test/rml-in-memory/pandas_dataframe/RMLIMTC0005a/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0005a/test_RMLIMTC0005a_DF.py` & `morph_kgc-2.5.1/test/rml-in-memory/pandas_dataframe/RMLIMTC0005a/test_RMLIMTC0005a_DF.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0006a/mapping.ttl` & `morph_kgc-2.5.1/test/rml-in-memory/pandas_dataframe/RMLIMTC0006a/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0006a/test_RMLIMTC0006a_DF.py` & `morph_kgc-2.5.1/test/rml-in-memory/pandas_dataframe/RMLIMTC0006a/test_RMLIMTC0006a_DF.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0007a/mapping.ttl` & `morph_kgc-2.5.1/test/rml-in-memory/pandas_dataframe/RMLIMTC0007a/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0007a/test_RMLIMTC0007a_DF.py` & `morph_kgc-2.5.1/test/rml-in-memory/pandas_dataframe/RMLIMTC0007a/test_RMLIMTC0007a_DF.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0007b/mapping.ttl` & `morph_kgc-2.5.1/test/rml-in-memory/pandas_dataframe/RMLIMTC0007b/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0007b/test_RMLIMTC0007b_DF.py` & `morph_kgc-2.5.1/test/rml-in-memory/pandas_dataframe/RMLIMTC0007b/test_RMLIMTC0007b_DF.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0007c/mapping.ttl` & `morph_kgc-2.5.1/test/rml-in-memory/pandas_dataframe/RMLIMTC0007c/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0007c/test_RMLIMTC0007c_DF.py` & `morph_kgc-2.5.1/test/rml-in-memory/pandas_dataframe/RMLIMTC0007c/test_RMLIMTC0007c_DF.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0007d/mapping.ttl` & `morph_kgc-2.5.1/test/rml-in-memory/pandas_dataframe/RMLIMTC0007d/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0007d/test_RMLTC0007d_DF.py` & `morph_kgc-2.5.1/test/rml-in-memory/pandas_dataframe/RMLIMTC0007d/test_RMLTC0007d_DF.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0007e/mapping.ttl` & `morph_kgc-2.5.1/test/rml-in-memory/pandas_dataframe/RMLIMTC0007e/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0007e/test_RMLIMTC0007e_DF.py` & `morph_kgc-2.5.1/test/rml-in-memory/pandas_dataframe/RMLIMTC0007e/test_RMLIMTC0007e_DF.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0007f/mapping.ttl` & `morph_kgc-2.5.1/test/rml-in-memory/pandas_dataframe/RMLIMTC0007f/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0007f/test_RMLIMTC0007f_DF.py` & `morph_kgc-2.5.1/test/rml-in-memory/pandas_dataframe/RMLIMTC0007f/test_RMLIMTC0007f_DF.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0007g/mapping.ttl` & `morph_kgc-2.5.1/test/rml-in-memory/pandas_dataframe/RMLIMTC0007g/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0007g/test_RMLIMTC0007g_DF.py` & `morph_kgc-2.5.1/test/rml-in-memory/pandas_dataframe/RMLIMTC0007g/test_RMLIMTC0007g_DF.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0007h/mapping.ttl` & `morph_kgc-2.5.1/test/rml-in-memory/pandas_dataframe/RMLIMTC0007h/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0007h/test_RMLIMTC0007h_DF.py` & `morph_kgc-2.5.1/test/rml-in-memory/pandas_dataframe/RMLIMTC0007h/test_RMLIMTC0007h_DF.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0008a/mapping.ttl` & `morph_kgc-2.5.1/test/rml-in-memory/pandas_dataframe/RMLIMTC0008a/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0008a/output.nq` & `morph_kgc-2.5.1/test/rml-in-memory/pandas_dataframe/RMLIMTC0008a/output.nq`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0008a/test_RMLIMTC0008a_DF.py` & `morph_kgc-2.5.1/test/rml-in-memory/pandas_dataframe/RMLIMTC0008a/test_RMLIMTC0008a_DF.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0008b/mapping.ttl` & `morph_kgc-2.5.1/test/rml-in-memory/pandas_dataframe/RMLIMTC0008b/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0008b/output.nq` & `morph_kgc-2.5.1/test/rml-in-memory/pandas_dataframe/RMLIMTC0008b/output.nq`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0008b/test_RMLIMTC0008b_DF.py` & `morph_kgc-2.5.1/test/rml-in-memory/pandas_dataframe/RMLIMTC0008b/test_RMLIMTC0008b_DF.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0008c/mapping.ttl` & `morph_kgc-2.5.1/test/rml-in-memory/pandas_dataframe/RMLIMTC0008c/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0008c/test_RMLIMTC0008c_DF.py` & `morph_kgc-2.5.1/test/rml-in-memory/pandas_dataframe/RMLIMTC0008c/test_RMLIMTC0008c_DF.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0009a/mapping.ttl` & `morph_kgc-2.5.1/test/rml-in-memory/pandas_dataframe/RMLIMTC0009a/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0009a/test_RMLIMTC0009a_DF.py` & `morph_kgc-2.5.1/test/rml-in-memory/pandas_dataframe/RMLIMTC0009a/test_RMLIMTC0009a_DF.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0009b/mapping.ttl` & `morph_kgc-2.5.1/test/rml-in-memory/pandas_dataframe/RMLIMTC0009b/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0009b/output.nq` & `morph_kgc-2.5.1/test/rml-in-memory/pandas_dataframe/RMLIMTC0009b/output.nq`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0009b/test_RMLIMTC0009b_DF.py` & `morph_kgc-2.5.1/test/rml-in-memory/pandas_dataframe/RMLIMTC0009b/test_RMLIMTC0009b_DF.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0010a/mapping.ttl` & `morph_kgc-2.5.1/test/rml-in-memory/pandas_dataframe/RMLIMTC0010a/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0010a/test_RMLIMTC0010a_DF.py` & `morph_kgc-2.5.1/test/rml-in-memory/pandas_dataframe/RMLIMTC0010a/test_RMLIMTC0010a_DF.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0010b/mapping.ttl` & `morph_kgc-2.5.1/test/rml-in-memory/pandas_dataframe/RMLIMTC0010b/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0010b/test_RMLIMTC0010b_DF.py` & `morph_kgc-2.5.1/test/rml-in-memory/pandas_dataframe/RMLIMTC0010b/test_RMLIMTC0010b_DF.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0010c/mapping.ttl` & `morph_kgc-2.5.1/test/rml-in-memory/pandas_dataframe/RMLIMTC0010c/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0010c/test_RMLIMTC0010c_DF.py` & `morph_kgc-2.5.1/test/rml-in-memory/pandas_dataframe/RMLIMTC0010c/test_RMLIMTC0010c_DF.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0011b/mapping.ttl` & `morph_kgc-2.5.1/test/rml-in-memory/pandas_dataframe/RMLIMTC0011b/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0011b/output.nq` & `morph_kgc-2.5.1/test/rml-in-memory/pandas_dataframe/RMLIMTC0011b/output.nq`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0011b/test_RMLIMTC0011b_DF.py` & `morph_kgc-2.5.1/test/rml-in-memory/pandas_dataframe/RMLIMTC0011b/test_RMLIMTC0011b_DF.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0012a/mapping.ttl` & `morph_kgc-2.5.1/test/rml-in-memory/pandas_dataframe/RMLIMTC0012a/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0012a/test_RMLIMTC0012a_DF.py` & `morph_kgc-2.5.1/test/rml-in-memory/pandas_dataframe/RMLIMTC0012a/test_RMLIMTC0012a_DF.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0012b/mapping.ttl` & `morph_kgc-2.5.1/test/rml-in-memory/pandas_dataframe/RMLIMTC0012b/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0012b/test_RMLIMTC0012b_DF.py` & `morph_kgc-2.5.1/test/rml-in-memory/pandas_dataframe/RMLIMTC0012b/test_RMLIMTC0012b_DF.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0012c/mapping.ttl` & `morph_kgc-2.5.1/test/rml-in-memory/pandas_dataframe/RMLIMTC0012c/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0012c/test_RMLIMTC0012c_DF.py` & `morph_kgc-2.5.1/test/rml-in-memory/pandas_dataframe/RMLIMTC0012c/test_RMLIMTC0012c_DF.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0012d/mapping.ttl` & `morph_kgc-2.5.1/test/rml-in-memory/pandas_dataframe/RMLIMTC0012d/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0012d/test_RMLIMTC0012d_DF.py` & `morph_kgc-2.5.1/test/rml-in-memory/pandas_dataframe/RMLIMTC0012d/test_RMLIMTC0012d_DF.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0015a/mapping.ttl` & `morph_kgc-2.5.1/test/rml-in-memory/pandas_dataframe/RMLIMTC0015a/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0015a/test_RMLIMTC0015a_DF.py` & `morph_kgc-2.5.1/test/rml-in-memory/pandas_dataframe/RMLIMTC0015a/test_RMLIMTC0015a_DF.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0015b/mapping.ttl` & `morph_kgc-2.5.1/test/rml-in-memory/pandas_dataframe/RMLIMTC0015b/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml-in-memory/pandas_dataframe/RMLIMTC0015b/test_RMLIMTC0015b_DF.py` & `morph_kgc-2.5.1/test/rml-in-memory/pandas_dataframe/RMLIMTC0015b/test_RMLIMTC0015b_DF.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml-in-memory/pandas_dataframe/triples_map_without_pom/mapping.ttl` & `morph_kgc-2.5.1/test/rml-in-memory/pandas_dataframe/triples_map_without_pom/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml-in-memory/pandas_dataframe/triples_map_without_pom/test_triples_map_without_pom_DF.py` & `morph_kgc-2.5.1/test/rml-in-memory/pandas_dataframe/triples_map_without_pom/test_triples_map_without_pom_DF.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml-star/RMLSTARTC001a/mapping.ttl` & `morph_kgc-2.5.1/test/rml-star/RMLSTARTC001a/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml-star/RMLSTARTC001a/test_RMLSTARTC001a_CSV.py` & `morph_kgc-2.5.1/test/rml-star/RMLSTARTC001a/test_RMLSTARTC001a_CSV.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml-star/RMLSTARTC001b/mapping.ttl` & `morph_kgc-2.5.1/test/rml-star/RMLSTARTC001b/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml-star/RMLSTARTC001b/test_RMLSTARTC001b_CSV.py` & `morph_kgc-2.5.1/test/rml-star/RMLSTARTC001b/test_RMLSTARTC001b_CSV.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml-star/RMLSTARTC002a/mapping.ttl` & `morph_kgc-2.5.1/test/rml-star/RMLSTARTC002a/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml-star/RMLSTARTC002a/test_RMLSTARTC002a_CSV.py` & `morph_kgc-2.5.1/test/rml-star/RMLSTARTC002a/test_RMLSTARTC002a_CSV.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml-star/RMLSTARTC002b/mapping.ttl` & `morph_kgc-2.5.1/test/rml-star/RMLSTARTC002b/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml-star/RMLSTARTC002b/test_RMLSTARTC002b_CSV.py` & `morph_kgc-2.5.1/test/rml-star/RMLSTARTC002b/test_RMLSTARTC002b_CSV.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml-star/RMLSTARTC003a/mapping.ttl` & `morph_kgc-2.5.1/test/rml-star/RMLSTARTC003a/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml-star/RMLSTARTC003a/test_RMLSTARTC003a_CSV.py` & `morph_kgc-2.5.1/test/rml-star/RMLSTARTC003a/test_RMLSTARTC003a_CSV.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml-star/RMLSTARTC003b/mapping.ttl` & `morph_kgc-2.5.1/test/rml-star/RMLSTARTC003b/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml-star/RMLSTARTC003b/test_RMLSTARTC003b_CSV.py` & `morph_kgc-2.5.1/test/rml-star/RMLSTARTC003b/test_RMLSTARTC003b_CSV.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml-star/RMLSTARTC004a/mapping.ttl` & `morph_kgc-2.5.1/test/rml-star/RMLSTARTC004a/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml-star/RMLSTARTC004a/test_RMLSTARTC004a_CSV.py` & `morph_kgc-2.5.1/test/rml-star/RMLSTARTC004a/test_RMLSTARTC004a_CSV.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml-star/RMLSTARTC004b/mapping.ttl` & `morph_kgc-2.5.1/test/rml-star/RMLSTARTC004b/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml-star/RMLSTARTC004b/test_RMLSTARTC004b_CSV.py` & `morph_kgc-2.5.1/test/rml-star/RMLSTARTC004b/test_RMLSTARTC004b_CSV.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml-star/RMLSTARTC005a/mapping.ttl` & `morph_kgc-2.5.1/test/rml-star/RMLSTARTC005a/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml-star/RMLSTARTC005a/test_RMLSTARTC005a_CSV.py` & `morph_kgc-2.5.1/test/rml-star/RMLSTARTC005a/test_RMLSTARTC005a_CSV.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml-star/RMLSTARTC005b/mapping.ttl` & `morph_kgc-2.5.1/test/rml-star/RMLSTARTC005b/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml-star/RMLSTARTC005b/test_RMLSTARTC005b_CSV.py` & `morph_kgc-2.5.1/test/rml-star/RMLSTARTC005b/test_RMLSTARTC005b_CSV.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml-star/RMLSTARTC006a/mapping.ttl` & `morph_kgc-2.5.1/test/rml-star/RMLSTARTC006a/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml-star/RMLSTARTC006a/test_RMLSTARTC006a_CSV.py` & `morph_kgc-2.5.1/test/rml-star/RMLSTARTC006a/test_RMLSTARTC006a_CSV.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml-star/RMLSTARTC006b/mapping.ttl` & `morph_kgc-2.5.1/test/rml-star/RMLSTARTC006b/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml-star/RMLSTARTC006b/test_RMLSTARTC006b_CSV.py` & `morph_kgc-2.5.1/test/rml-star/RMLSTARTC006b/test_RMLSTARTC006b_CSV.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml-star/RMLSTARTC007a/mapping.ttl` & `morph_kgc-2.5.1/test/rml-star/RMLSTARTC007a/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml-star/RMLSTARTC007a/test_RMLSTARTC007a_CSV.py` & `morph_kgc-2.5.1/test/rml-star/RMLSTARTC007a/test_RMLSTARTC007a_CSV.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml-star/RMLSTARTC007b/mapping.ttl` & `morph_kgc-2.5.1/test/rml-star/RMLSTARTC007b/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml-star/RMLSTARTC007b/test_RMLSTARTC007b_CSV.py` & `morph_kgc-2.5.1/test/rml-star/RMLSTARTC007b/test_RMLSTARTC007b_CSV.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml-star/RMLSTARTC008a/mapping.ttl` & `morph_kgc-2.5.1/test/rml-star/RMLSTARTC008a/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml-star/RMLSTARTC008a/test_RMLSTARTC008a_CSV.py` & `morph_kgc-2.5.1/test/rml-star/RMLSTARTC008a/test_RMLSTARTC008a_CSV.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml-star/RMLSTARTC008b/mapping.ttl` & `morph_kgc-2.5.1/test/rml-star/RMLSTARTC008b/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rml-star/RMLSTARTC008b/test_RMLSTARTC008b_CSV.py` & `morph_kgc-2.5.1/test/rml-star/RMLSTARTC008b/test_RMLSTARTC008b_CSV.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rmltv/RMLTVTC0002d/mapping.ttl` & `morph_kgc-2.5.1/test/rmltv/RMLTVTC0002d/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rmltv/RMLTVTC0002d/test_RMLTVTC0002d_CSV.py` & `morph_kgc-2.5.1/test/rmltv/RMLTVTC0002d/test_RMLTVTC0002d_CSV.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rmltv/RMLTVTC0002g/mapping.ttl` & `morph_kgc-2.5.1/test/rmltv/RMLTVTC0002g/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rmltv/RMLTVTC0002g/test_RMLTVTC0002g_CSV.py` & `morph_kgc-2.5.1/test/rmltv/RMLTVTC0002g/test_RMLTVTC0002g_CSV.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rmltv/RMLTVTC0002h/mapping.ttl` & `morph_kgc-2.5.1/test/rmltv/RMLTVTC0002h/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rmltv/RMLTVTC0002h/test_RMLTVTC0002h_CSV.py` & `morph_kgc-2.5.1/test/rmltv/RMLTVTC0002h/test_RMLTVTC0002h_CSV.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rmltv/RMLTVTC0002i/test_RMLTVTC0002i_CSV.py` & `morph_kgc-2.5.1/test/rmltv/RMLTVTC0002i/test_RMLTVTC0002i_CSV.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rmltv/RMLTVTC0002j/mapping.ttl` & `morph_kgc-2.5.1/test/rmltv/RMLTVTC0002j/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rmltv/RMLTVTC0002j/test_RMLTVTC0002j_CSV.py` & `morph_kgc-2.5.1/test/rmltv/RMLTVTC0002j/test_RMLTVTC0002j_CSV.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rmltv/RMLTVTC0003b/mapping.ttl` & `morph_kgc-2.5.1/test/rmltv/RMLTVTC0003b/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rmltv/RMLTVTC0003b/test_RMLTVTC0003b_CSV.py` & `morph_kgc-2.5.1/test/rmltv/RMLTVTC0003b/test_RMLTVTC0003b_CSV.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rmltv/RMLTVTC0009c/mapping.ttl` & `morph_kgc-2.5.1/test/rmltv/RMLTVTC0009c/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rmltv/RMLTVTC0009c/test_RMLTVTC0009c_CSV.py` & `morph_kgc-2.5.1/test/rmltv/RMLTVTC0009c/test_RMLTVTC0009c_CSV.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rmltv/RMLTVTC0009d/mapping.ttl` & `morph_kgc-2.5.1/test/rmltv/RMLTVTC0009d/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rmltv/RMLTVTC0009d/test_RMLTVTC0009d_CSV.py` & `morph_kgc-2.5.1/test/rmltv/RMLTVTC0009d/test_RMLTVTC0009d_CSV.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rmltv/RMLTVTC0011a/mapping.ttl` & `morph_kgc-2.5.1/test/rmltv/RMLTVTC0011a/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rmltv/RMLTVTC0011a/output.nq` & `morph_kgc-2.5.1/test/rmltv/RMLTVTC0011a/output.nq`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rmltv/RMLTVTC0011a/test_RMLTVTC0011a_CSV.py` & `morph_kgc-2.5.1/test/rmltv/RMLTVTC0011a/test_RMLTVTC0011a_CSV.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rmltv/RMLTVTC0014d/mapping.ttl` & `morph_kgc-2.5.1/test/rmltv/RMLTVTC0014d/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rmltv/RMLTVTC0014d/test_RMLTVTC0014d_CSV.py` & `morph_kgc-2.5.1/test/rmltv/RMLTVTC0014d/test_RMLTVTC0014d_CSV.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rmltv/RMLTVTC0015a/mapping.ttl` & `morph_kgc-2.5.1/test/rmltv/RMLTVTC0015a/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rmltv/RMLTVTC0015a/test_RMLTVTC0015a_CSV.py` & `morph_kgc-2.5.1/test/rmltv/RMLTVTC0015a/test_RMLTVTC0015a_CSV.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rmltv/RMLTVTC0015b/mapping.ttl` & `morph_kgc-2.5.1/test/rmltv/RMLTVTC0015b/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rmltv/RMLTVTC0015b/test_RMLTVTC0015b_CSV.py` & `morph_kgc-2.5.1/test/rmltv/RMLTVTC0015b/test_RMLTVTC0015b_CSV.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rmltv/RMLTVTC0019a/mapping.ttl` & `morph_kgc-2.5.1/test/rmltv/RMLTVTC0019a/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rmltv/RMLTVTC0019a/test_RMLTVTC0019a_CSV.py` & `morph_kgc-2.5.1/test/rmltv/RMLTVTC0019a/test_RMLTVTC0019a_CSV.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rmltv/RMLTVTC0026a/mapping.ttl` & `morph_kgc-2.5.1/test/rmltv/RMLTVTC0026a/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rmltv/RMLTVTC0026a/test_RMLTVTC0026a_CSV.py` & `morph_kgc-2.5.1/test/rmltv/RMLTVTC0026a/test_RMLTVTC0026a_CSV.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rmltv/RMLTVTC0027a/mapping.ttl` & `morph_kgc-2.5.1/test/rmltv/RMLTVTC0027a/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rmltv/RMLTVTC0027a/test_RMLTVTC0027a_CSV.py` & `morph_kgc-2.5.1/test/rmltv/RMLTVTC0027a/test_RMLTVTC0027a_CSV.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rmltv/RMLTVTC0028a/mapping.ttl` & `morph_kgc-2.5.1/test/rmltv/RMLTVTC0028a/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rmltv/RMLTVTC0028a/test_RMLTVTC0028a_CSV.py` & `morph_kgc-2.5.1/test/rmltv/RMLTVTC0028a/test_RMLTVTC0028a_CSV.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rmltv/RMLTVTC0029a/mapping.ttl` & `morph_kgc-2.5.1/test/rmltv/RMLTVTC0029a/mapping.ttl`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/test/rmltv/RMLTVTC0029a/test_RMLTVTC0029a_CSV.py` & `morph_kgc-2.5.1/test/rmltv/RMLTVTC0029a/test_RMLTVTC0029a_CSV.py`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/LICENSE` & `morph_kgc-2.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/README.md` & `morph_kgc-2.5.1/README.md`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/pyproject.toml` & `morph_kgc-2.5.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `morph_kgc-2.5.0/PKG-INFO` & `morph_kgc-2.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: morph_kgc
-Version: 2.5.0
+Version: 2.5.1
 Summary: Powerful [R2]RML engine to create RDF knowledge graphs from heterogeneous data sources.
 Project-URL: Documentation, https://morph-kgc.readthedocs.io/en/latest/documentation/
 Project-URL: Source, https://github.com/morph-kgc/morph-kgc
 Project-URL: Tracker, https://github.com/morph-kgc/morph-kgc/issues
 Project-URL: CI, https://github.com/morph-kgc/morph-kgc/actions
 Project-URL: Homepage, https://morph-kgc.readthedocs.io/en/latest/
 Project-URL: History, https://github.com/morph-kgc/morph-kgc/releases
```

