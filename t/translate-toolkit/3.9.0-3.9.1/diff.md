# Comparing `tmp/translate-toolkit-3.9.0.tar.gz` & `tmp/translate-toolkit-3.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "translate-toolkit-3.9.0.tar", last modified: Mon May 15 15:14:10 2023, max compression
+gzip compressed data, was "translate-toolkit-3.9.1.tar", last modified: Wed Jun 14 06:36:35 2023, max compression
```

## Comparing `translate-toolkit-3.9.0.tar` & `translate-toolkit-3.9.1.tar`

### file list

```diff
@@ -1,1001 +1,983 @@
-drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-05-15 15:14:10.629689 translate-toolkit-3.9.0/
--rw-r--r--   0 nijel     (1000) nijel     (1000)      135 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/.deepsource.toml
-drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-05-15 15:14:10.481689 translate-toolkit-3.9.0/.github/
--rw-r--r--   0 nijel     (1000) nijel     (1000)      349 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/.github/dependabot.yml
-drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-05-15 15:14:10.481689 translate-toolkit-3.9.0/.github/matchers/
--rw-r--r--   0 nijel     (1000) nijel     (1000)      292 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/.github/matchers/flake8.json
-drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-05-15 15:14:10.481689 translate-toolkit-3.9.0/.github/workflows/
--rw-r--r--   0 nijel     (1000) nijel     (1000)      815 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/.github/workflows/docs.yml
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1905 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/.github/workflows/linux.yml
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1361 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/.github/workflows/osx.yml
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1764 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/.github/workflows/pre-commit.yml
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1774 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/.github/workflows/setup.yml
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1145 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/.github/workflows/win.yml
--rw-r--r--   0 nijel     (1000) nijel     (1000)      724 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/.gitignore
--rw-r--r--   0 nijel     (1000) nijel     (1000)      102 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/.gitmodules
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1265 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/.pre-commit-config.yaml
--rw-r--r--   0 nijel     (1000) nijel     (1000)      569 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/.readthedocs.yml
--rw-r--r--   0 nijel     (1000) nijel     (1000)    17992 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/COPYING
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1768 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/CREDITS
--rw-r--r--   0 nijel     (1000) nijel     (1000)      171 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/LICENSES
--rw-r--r--   0 nijel     (1000) nijel     (1000)      305 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/MANIFEST.in
--rw-r--r--   0 nijel     (1000) nijel     (1000)     2925 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/Makefile
--rw-r--r--   0 nijel     (1000) nijel     (1000)    10835 2023-05-15 15:14:10.629689 translate-toolkit-3.9.0/PKG-INFO
--rw-r--r--   0 nijel     (1000) nijel     (1000)     8810 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/README.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)       15 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/codecov.yml
-drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-05-15 15:14:10.481689 translate-toolkit-3.9.0/docs/
--rw-r--r--   0 nijel     (1000) nijel     (1000)     5743 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/Makefile
-drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-05-15 15:14:10.481689 translate-toolkit-3.9.0/docs/_ext/
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1016 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/_ext/translate_docs.py
-drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-05-15 15:14:10.485689 translate-toolkit-3.9.0/docs/_static/
--rw-r--r--   0 nijel     (1000) nijel     (1000)       55 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/_static/README.txt
-drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-05-15 15:14:10.485689 translate-toolkit-3.9.0/docs/_themes/
--rw-r--r--   0 nijel     (1000) nijel     (1000)      703 2023-05-15 15:13:17.000000 translate-toolkit-3.9.0/docs/_themes/README.rst
-drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-05-15 15:14:10.485689 translate-toolkit-3.9.0/docs/_themes/sphinx-bootstrap/
--rw-r--r--   0 nijel     (1000) nijel     (1000)      200 2023-05-15 15:13:17.000000 translate-toolkit-3.9.0/docs/_themes/sphinx-bootstrap/globaltoc.html
--rw-r--r--   0 nijel     (1000) nijel     (1000)     2628 2023-05-15 15:13:17.000000 translate-toolkit-3.9.0/docs/_themes/sphinx-bootstrap/layout.html
--rw-r--r--   0 nijel     (1000) nijel     (1000)      227 2023-05-15 15:13:17.000000 translate-toolkit-3.9.0/docs/_themes/sphinx-bootstrap/localtoc.html
--rw-r--r--   0 nijel     (1000) nijel     (1000)      304 2023-05-15 15:13:17.000000 translate-toolkit-3.9.0/docs/_themes/sphinx-bootstrap/relations.html
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1085 2023-05-15 15:13:17.000000 translate-toolkit-3.9.0/docs/_themes/sphinx-bootstrap/search.html
--rw-r--r--   0 nijel     (1000) nijel     (1000)      305 2023-05-15 15:13:17.000000 translate-toolkit-3.9.0/docs/_themes/sphinx-bootstrap/searchbox.html
--rw-r--r--   0 nijel     (1000) nijel     (1000)      420 2023-05-15 15:13:17.000000 translate-toolkit-3.9.0/docs/_themes/sphinx-bootstrap/sourcelink.html
-drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-05-15 15:14:10.485689 translate-toolkit-3.9.0/docs/_themes/sphinx-bootstrap/static/
--rw-r--r--   0 nijel     (1000) nijel     (1000)    10518 2023-05-15 15:13:17.000000 translate-toolkit-3.9.0/docs/_themes/sphinx-bootstrap/static/bootstrap-responsive.css
--rw-r--r--   0 nijel     (1000) nijel     (1000)      374 2023-05-15 15:13:17.000000 translate-toolkit-3.9.0/docs/_themes/sphinx-bootstrap/static/bootstrap-sphinx.css_t
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1727 2023-05-15 15:13:17.000000 translate-toolkit-3.9.0/docs/_themes/sphinx-bootstrap/static/bootstrap-sphinx.js
--rw-r--r--   0 nijel     (1000) nijel     (1000)    97055 2023-05-15 15:13:17.000000 translate-toolkit-3.9.0/docs/_themes/sphinx-bootstrap/static/bootstrap.css
--rw-r--r--   0 nijel     (1000) nijel     (1000)    22323 2023-05-15 15:13:17.000000 translate-toolkit-3.9.0/docs/_themes/sphinx-bootstrap/static/bootstrap.js
-drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-05-15 15:14:10.485689 translate-toolkit-3.9.0/docs/_themes/sphinx-bootstrap/static/font/
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)    38708 2023-05-15 15:13:17.000000 translate-toolkit-3.9.0/docs/_themes/sphinx-bootstrap/static/font/fontawesome-webfont.eot
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)   130151 2023-05-15 15:13:17.000000 translate-toolkit-3.9.0/docs/_themes/sphinx-bootstrap/static/font/fontawesome-webfont.svg
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)    68476 2023-05-15 15:13:17.000000 translate-toolkit-3.9.0/docs/_themes/sphinx-bootstrap/static/font/fontawesome-webfont.ttf
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)    41752 2023-05-15 15:13:17.000000 translate-toolkit-3.9.0/docs/_themes/sphinx-bootstrap/static/font/fontawesome-webfont.woff
--rw-r--r--   0 nijel     (1000) nijel     (1000)    93436 2023-05-15 15:13:17.000000 translate-toolkit-3.9.0/docs/_themes/sphinx-bootstrap/static/jquery.js
-drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-05-15 15:14:10.485689 translate-toolkit-3.9.0/docs/_themes/sphinx-bootstrap/static/less/
--rw-r--r--   0 nijel     (1000) nijel     (1000)    14766 2023-05-15 15:13:17.000000 translate-toolkit-3.9.0/docs/_themes/sphinx-bootstrap/static/less/font-awesome.less
--rw-r--r--   0 nijel     (1000) nijel     (1000)     4514 2023-05-15 15:13:17.000000 translate-toolkit-3.9.0/docs/_themes/sphinx-bootstrap/static/less/theme.less
--rw-r--r--   0 nijel     (1000) nijel     (1000)     8431 2023-05-15 15:13:17.000000 translate-toolkit-3.9.0/docs/_themes/sphinx-bootstrap/static/less/variables.less
--rw-r--r--   0 nijel     (1000) nijel     (1000)      114 2023-05-15 15:13:17.000000 translate-toolkit-3.9.0/docs/_themes/sphinx-bootstrap/theme.conf
-drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-05-15 15:14:10.485689 translate-toolkit-3.9.0/docs/api/
--rw-r--r--   0 nijel     (1000) nijel     (1000)     5427 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/api/convert.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)      786 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/api/filters.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)      912 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/api/index.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     3317 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/api/lang.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)      964 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/api/misc.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)      364 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/api/search.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)      177 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/api/services.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     6573 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/api/storage.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1680 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/api/tools.rst
-drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-05-15 15:14:10.493689 translate-toolkit-3.9.0/docs/commands/
--rw-r--r--   0 nijel     (1000) nijel     (1000)     5021 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/commands/csv2po.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     3362 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/commands/csv2tbx.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     5091 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/commands/flatxml2po.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     2063 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/commands/general_usage.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     5138 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/commands/html2po.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     4287 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/commands/ical2po.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     6234 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/commands/index.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     5482 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/commands/ini2po.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     4106 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/commands/json2po.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)      356 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/commands/junitmsgfmt.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     2631 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/commands/levenshtein_distance.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     4456 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/commands/moz-l10n-builder.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     7496 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/commands/moz2po.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     9695 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/commands/mozilla_l10n_scripts.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     3699 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/commands/odf2xliff.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     7685 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/commands/oo2po.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1157 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/commands/option_accelerator.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     2411 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/commands/option_duplicates.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1704 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/commands/option_errorlevel.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)      599 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/commands/option_filteraction.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)      613 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/commands/option_multifile.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1562 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/commands/option_personality.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     2719 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/commands/option_progress.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     4073 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/commands/option_rewrite.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     4377 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/commands/phase.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     4172 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/commands/php2po.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     3396 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/commands/po2tmx.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1659 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/commands/po2wordfast.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1804 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/commands/poclean.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)      968 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/commands/pocommentclean.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     3485 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/commands/pocompendium.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1847 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/commands/pocompile.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     3790 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/commands/poconflicts.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     5658 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/commands/pocount.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     7176 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/commands/podebug.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     4972 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/commands/pofilter.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)    25812 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/commands/pofilter_tests.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     3789 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/commands/pogrep.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     4091 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/commands/pomerge.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     2544 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/commands/pomigrate2.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1746 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/commands/popuretext.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1367 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/commands/poreencode.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     2046 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/commands/porestructure.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     3586 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/commands/posegment.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)      848 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/commands/posplit.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     3354 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/commands/poswap.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     4111 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/commands/pot2po.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)    16451 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/commands/poterminology.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     8052 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/commands/poterminology_stopword_file.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     3214 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/commands/pretranslate.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     7629 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/commands/prop2po.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     4925 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/commands/rc2po.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     4019 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/commands/resx2po.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     3908 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/commands/sub2po.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     5754 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/commands/symb2po.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1638 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/commands/tbx2po.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     2375 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/commands/tiki2po.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     2544 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/commands/tmserver.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     3864 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/commands/ts2po.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     7056 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/commands/txt2po.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     3727 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/commands/web2py2po.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     3213 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/commands/xliff2po.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     4357 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/commands/yaml2po.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     6572 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/conf.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1028 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/contents.rst.inc
-drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-05-15 15:14:10.497689 translate-toolkit-3.9.0/docs/developers/
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1299 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/developers/building.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     3679 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/developers/contributing.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     2146 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/developers/deprecation.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     9692 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/developers/developers.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)    11047 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/developers/releasing.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     3174 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/developers/reporting_bugs.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)    19038 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/developers/styleguide.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     9434 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/developers/testing.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     2499 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/features.rst
-drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-05-15 15:14:10.501689 translate-toolkit-3.9.0/docs/formats/
--rw-r--r--   0 nijel     (1000) nijel     (1000)      736 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/formats/android.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     7698 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/formats/base_classes.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     2041 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/formats/catkeys.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)      707 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/formats/conformance.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1973 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/formats/csv.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1006 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/formats/dtd.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     3043 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/formats/flatxml.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)      451 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/formats/flex.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)      493 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/formats/gsi.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1160 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/formats/html.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     2090 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/formats/ical.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     7893 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/formats/index.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)      769 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/formats/ini.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)      923 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/formats/json.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)      998 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/formats/mo.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)      452 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/formats/mozilla_lang.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1549 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/formats/odf.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)      962 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/formats/omegat_glossary.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     7761 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/formats/php.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1210 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/formats/po.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1579 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/formats/properties.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)      888 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/formats/qm.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1233 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/formats/qt_phrase_book.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     2078 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/formats/quoting_and_escaping.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1281 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/formats/rc.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1412 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/formats/resx.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)      979 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/formats/strings.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1360 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/formats/subtitles.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     2026 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/formats/tbx.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)      800 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/formats/text.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)      810 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/formats/tmx.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1964 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/formats/ts.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1216 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/formats/utx.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1821 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/formats/wiki.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)      316 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/formats/wml.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)      777 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/formats/wordfast.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     2160 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/formats/xliff.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)      495 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/formats/yaml.rst
-drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-05-15 15:14:10.501689 translate-toolkit-3.9.0/docs/guides/
--rw-r--r--   0 nijel     (1000) nijel     (1000)     6603 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/guides/checking_for_inconsistencies.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1736 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/guides/cleanup_translator_comments.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     7490 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/guides/creating_a_terminology_list_from_your_existing_translations.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     2161 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/guides/creating_mozilla_pot_files.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1960 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/guides/document_translation.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1297 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/guides/index.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     6258 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/guides/migrating_translations.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1524 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/guides/running_the_tools_on_microsoft_windows.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     7596 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/guides/using_csv2po.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     2230 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/guides/using_oo2po.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     7736 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/guides/using_pofilter.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     4864 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/history.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)      237 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/index.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     5263 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/installation.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)      233 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/license.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     5116 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/make.bat
-drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-05-15 15:14:10.509689 translate-toolkit-3.9.0/docs/releases/
--rw-r--r--   0 nijel     (1000) nijel     (1000)      225 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/releases/0.10.1.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     2200 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/releases/0.10.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1170 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/releases/0.11.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)      220 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/releases/0.7.1.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)      219 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/releases/0.8.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)      219 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/releases/0.9.1.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)      221 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/releases/0.9.2.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     4422 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/releases/0.9.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)      655 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/releases/1.0.1.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     6959 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/releases/1.0.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     4071 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/releases/1.1.0.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)      680 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/releases/1.1.1.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     4368 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/releases/1.10.0.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     4975 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/releases/1.11.0.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     5431 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/releases/1.12.0.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     4151 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/releases/1.13.0.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     2206 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/releases/1.2.0.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)      223 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/releases/1.2.1.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)      273 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/releases/1.3.0.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)      713 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/releases/1.4.0.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)      961 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/releases/1.4.1.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)      223 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/releases/1.5.0.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)      222 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/releases/1.5.1.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)      222 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/releases/1.5.2.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)      222 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/releases/1.5.3.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)      589 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/releases/1.6.0.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)      218 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/releases/1.7.0.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)      221 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/releases/1.8.0.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     3162 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/releases/1.8.1.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     2325 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/releases/1.9.0.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     8012 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/releases/2.0.0.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     2153 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/releases/2.1.0.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1621 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/releases/2.2.0.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1310 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/releases/2.2.1.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)      376 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/releases/2.2.2.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)      384 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/releases/2.2.3.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1018 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/releases/2.2.4.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)      557 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/releases/2.2.5.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1683 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/releases/2.3.0.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     2341 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/releases/2.3.1.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     2357 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/releases/2.4.0.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1465 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/releases/2.5.0.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1416 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/releases/2.5.1.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1563 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/releases/3.0.0.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1211 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/releases/3.1.0.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)      378 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/releases/3.1.1.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)      639 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/releases/3.2.0.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1490 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/releases/3.3.0.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)      503 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/releases/3.3.1.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)      604 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/releases/3.3.2.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)      692 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/releases/3.3.3.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)      438 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/releases/3.3.4.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)      490 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/releases/3.3.5.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)      452 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/releases/3.3.6.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)      563 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/releases/3.4.0.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)      573 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/releases/3.4.1.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)      481 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/releases/3.5.0.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)      367 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/releases/3.5.1.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)      482 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/releases/3.5.2.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)      394 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/releases/3.5.3.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)      765 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/releases/3.6.0.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)      533 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/releases/3.6.1.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)      508 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/releases/3.6.2.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)      869 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/releases/3.7.0.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)      477 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/releases/3.7.1.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)      387 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/releases/3.7.2.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)      602 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/releases/3.7.3.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)      536 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/releases/3.7.4.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)      701 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/releases/3.8.0.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)      529 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/releases/3.8.1.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)      348 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/releases/3.8.2.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)      398 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/releases/3.8.3.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)      403 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/releases/3.8.4.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)      347 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/releases/3.8.5.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)      447 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/releases/3.8.6.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)      776 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/releases/3.9.0.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1246 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/releases/README.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1683 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/releases/index.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)      306 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/pyproject.toml
--rw-r--r--   0 nijel     (1000) nijel     (1000)       41 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/pytest.ini
-drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-05-15 15:14:10.509689 translate-toolkit-3.9.0/requirements/
--rw-r--r--   0 nijel     (1000) nijel     (1000)       47 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/requirements/dev.txt
--rw-r--r--   0 nijel     (1000) nijel     (1000)      114 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/requirements/dist.txt
--rw-r--r--   0 nijel     (1000) nijel     (1000)       18 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/requirements/lint.txt
--rw-r--r--   0 nijel     (1000) nijel     (1000)      735 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/requirements/optional.txt
--rw-r--r--   0 nijel     (1000) nijel     (1000)       71 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/requirements/required.txt
--rw-r--r--   0 nijel     (1000) nijel     (1000)      107 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/requirements/test.txt
--rw-r--r--   0 nijel     (1000) nijel     (1000)     5951 2023-05-15 15:14:10.633689 translate-toolkit-3.9.0/setup.cfg
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)     2385 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/setup.py
-drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-05-15 15:14:10.473689 translate-toolkit-3.9.0/tests/
-drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-05-15 15:14:10.517689 translate-toolkit-3.9.0/tests/cli/
-drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-05-15 15:14:10.473689 translate-toolkit-3.9.0/tests/cli/data/
-drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-05-15 15:14:10.517689 translate-toolkit-3.9.0/tests/cli/data/test_flatxml2po/
--rw-r--r--   0 nijel     (1000) nijel     (1000)      460 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/data/test_flatxml2po/one.xml
--rw-r--r--   0 nijel     (1000) nijel     (1000)      813 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/data/test_flatxml2po/out.po
-drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-05-15 15:14:10.521689 translate-toolkit-3.9.0/tests/cli/data/test_flatxml2po_wrongkey/
--rw-r--r--   0 nijel     (1000) nijel     (1000)       57 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/data/test_flatxml2po_wrongkey/one.xml
--rw-r--r--   0 nijel     (1000) nijel     (1000)      212 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/data/test_flatxml2po_wrongkey/stderr.txt
-drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-05-15 15:14:10.521689 translate-toolkit-3.9.0/tests/cli/data/test_flatxml2po_wrongns/
--rw-r--r--   0 nijel     (1000) nijel     (1000)       57 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/data/test_flatxml2po_wrongns/one.xml
--rw-r--r--   0 nijel     (1000) nijel     (1000)      200 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/data/test_flatxml2po_wrongns/stderr.txt
-drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-05-15 15:14:10.521689 translate-toolkit-3.9.0/tests/cli/data/test_flatxml2po_wrongroot/
--rw-r--r--   0 nijel     (1000) nijel     (1000)       57 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/data/test_flatxml2po_wrongroot/one.xml
--rw-r--r--   0 nijel     (1000) nijel     (1000)      198 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/data/test_flatxml2po_wrongroot/stderr.txt
-drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-05-15 15:14:10.521689 translate-toolkit-3.9.0/tests/cli/data/test_flatxml2po_wrongvalue/
--rw-r--r--   0 nijel     (1000) nijel     (1000)       57 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/data/test_flatxml2po_wrongvalue/one.xml
--rw-r--r--   0 nijel     (1000) nijel     (1000)      210 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/data/test_flatxml2po_wrongvalue/stderr.txt
-drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-05-15 15:14:10.521689 translate-toolkit-3.9.0/tests/cli/data/test_junitmsgfmt_failure/
--rw-r--r--   0 nijel     (1000) nijel     (1000)      238 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/data/test_junitmsgfmt_failure/one.po
--rw-r--r--   0 nijel     (1000) nijel     (1000)      846 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/data/test_junitmsgfmt_failure/stdout.txt
-drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-05-15 15:14:10.521689 translate-toolkit-3.9.0/tests/cli/data/test_junitmsgfmt_untranslated/
--rw-r--r--   0 nijel     (1000) nijel     (1000)      207 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/data/test_junitmsgfmt_untranslated/one.po
--rw-r--r--   0 nijel     (1000) nijel     (1000)      808 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/data/test_junitmsgfmt_untranslated/stdout.txt
-drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-05-15 15:14:10.521689 translate-toolkit-3.9.0/tests/cli/data/test_po2csv/
--rw-r--r--   0 nijel     (1000) nijel     (1000)       85 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/data/test_po2csv/one.po
--rw-r--r--   0 nijel     (1000) nijel     (1000)       88 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/data/test_po2csv/out.txt
-drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-05-15 15:14:10.521689 translate-toolkit-3.9.0/tests/cli/data/test_po2flatxml/
--rw-r--r--   0 nijel     (1000) nijel     (1000)       61 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/data/test_po2flatxml/one.po
--rw-r--r--   0 nijel     (1000) nijel     (1000)      118 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/data/test_po2flatxml/out.xml
-drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-05-15 15:14:10.521689 translate-toolkit-3.9.0/tests/cli/data/test_po2flatxml_params/
--rw-r--r--   0 nijel     (1000) nijel     (1000)       82 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/data/test_po2flatxml_params/one.po
--rw-r--r--   0 nijel     (1000) nijel     (1000)      318 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/data/test_po2flatxml_params/out.xml
-drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-05-15 15:14:10.525689 translate-toolkit-3.9.0/tests/cli/data/test_po2flatxml_preserve/
--rw-r--r--   0 nijel     (1000) nijel     (1000)       89 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/data/test_po2flatxml_preserve/one.po
--rw-r--r--   0 nijel     (1000) nijel     (1000)      292 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/data/test_po2flatxml_preserve/out.xml
--rw-r--r--   0 nijel     (1000) nijel     (1000)      264 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/data/test_po2flatxml_preserve/two.xml
-drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-05-15 15:14:10.525689 translate-toolkit-3.9.0/tests/cli/data/test_po2flatxml_template/
--rw-r--r--   0 nijel     (1000) nijel     (1000)       82 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/data/test_po2flatxml_template/one.po
--rw-r--r--   0 nijel     (1000) nijel     (1000)      270 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/data/test_po2flatxml_template/out.xml
--rw-r--r--   0 nijel     (1000) nijel     (1000)      115 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/data/test_po2flatxml_template/two.xml
-drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-05-15 15:14:10.525689 translate-toolkit-3.9.0/tests/cli/data/test_po2html/
--rw-r--r--   0 nijel     (1000) nijel     (1000)       85 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/data/test_po2html/one.po
--rw-r--r--   0 nijel     (1000) nijel     (1000)       79 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/data/test_po2html/out.txt
--rw-r--r--   0 nijel     (1000) nijel     (1000)       78 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/data/test_po2html/template.html
-drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-05-15 15:14:10.525689 translate-toolkit-3.9.0/tests/cli/data/test_po2json_files_removeuntranslated/
--rw-r--r--   0 nijel     (1000) nijel     (1000)       42 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/data/test_po2json_files_removeuntranslated/out.json
--rw-r--r--   0 nijel     (1000) nijel     (1000)       83 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/data/test_po2json_files_removeuntranslated/template.json
--rw-r--r--   0 nijel     (1000) nijel     (1000)      161 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/data/test_po2json_files_removeuntranslated/translations.po
-drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-05-15 15:14:10.525689 translate-toolkit-3.9.0/tests/cli/data/test_po2prop_mozilla_files/
--rw-r--r--   0 nijel     (1000) nijel     (1000)      145 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/data/test_po2prop_mozilla_files/out.properties
--rw-r--r--   0 nijel     (1000) nijel     (1000)      141 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/data/test_po2prop_mozilla_files/template.properties
--rw-r--r--   0 nijel     (1000) nijel     (1000)      198 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/data/test_po2prop_mozilla_files/translations.po
-drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-05-15 15:14:10.525689 translate-toolkit-3.9.0/tests/cli/data/test_po2ts/
--rw-r--r--   0 nijel     (1000) nijel     (1000)       85 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/data/test_po2ts/one.po
--rw-r--r--   0 nijel     (1000) nijel     (1000)      362 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/data/test_po2ts/out.txt
-drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-05-15 15:14:10.529689 translate-toolkit-3.9.0/tests/cli/data/test_po2txt/
--rw-r--r--   0 nijel     (1000) nijel     (1000)      151 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/data/test_po2txt/one.po
--rw-r--r--   0 nijel     (1000) nijel     (1000)       32 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/data/test_po2txt/out.txt
-drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-05-15 15:14:10.529689 translate-toolkit-3.9.0/tests/cli/data/test_po2txt_threshold/
--rw-r--r--   0 nijel     (1000) nijel     (1000)      151 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/data/test_po2txt_threshold/one.po
--rw-r--r--   0 nijel     (1000) nijel     (1000)        0 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/data/test_po2txt_threshold/out.txt
-drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-05-15 15:14:10.529689 translate-toolkit-3.9.0/tests/cli/data/test_pocount/
--rw-r--r--   0 nijel     (1000) nijel     (1000)      206 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/data/test_pocount/stderr.txt
-drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-05-15 15:14:10.529689 translate-toolkit-3.9.0/tests/cli/data/test_pocount_mutually_exclusive/
--rw-r--r--   0 nijel     (1000) nijel     (1000)      238 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/data/test_pocount_mutually_exclusive/stderr.txt
-drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-05-15 15:14:10.529689 translate-toolkit-3.9.0/tests/cli/data/test_pocount_nonexistant/
--rw-r--r--   0 nijel     (1000) nijel     (1000)       74 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/data/test_pocount_nonexistant/stderr.txt
-drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-05-15 15:14:10.529689 translate-toolkit-3.9.0/tests/cli/data/test_pocount_po_csv/
--rw-r--r--   0 nijel     (1000) nijel     (1000)       43 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/data/test_pocount_po_csv/one.po
-drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-05-15 15:14:10.529689 translate-toolkit-3.9.0/tests/cli/data/test_pocount_po_file/
--rw-r--r--   0 nijel     (1000) nijel     (1000)       43 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/data/test_pocount_po_file/one.po
--rw-r--r--   0 nijel     (1000) nijel     (1000)      430 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/data/test_pocount_po_file/stdout.txt
-drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-05-15 15:14:10.529689 translate-toolkit-3.9.0/tests/cli/data/test_pocount_po_fuzzy/
--rw-r--r--   0 nijel     (1000) nijel     (1000)      121 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/data/test_pocount_po_fuzzy/one.po
--rw-r--r--   0 nijel     (1000) nijel     (1000)      492 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/data/test_pocount_po_fuzzy/stdout.txt
-drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-05-15 15:14:10.529689 translate-toolkit-3.9.0/tests/cli/data/test_pocount_po_plurals/
--rw-r--r--   0 nijel     (1000) nijel     (1000)      101 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/data/test_pocount_po_plurals/plural.po
--rw-r--r--   0 nijel     (1000) nijel     (1000)      420 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/data/test_pocount_po_plurals/stdout.txt
-drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-05-15 15:14:10.529689 translate-toolkit-3.9.0/tests/cli/data/test_pocount_xliff_states_no/
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1505 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/data/test_pocount_xliff_states_no/states.xlf
--rw-r--r--   0 nijel     (1000) nijel     (1000)      503 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/data/test_pocount_xliff_states_no/stdout.txt
-drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-05-15 15:14:10.529689 translate-toolkit-3.9.0/tests/cli/data/test_pocount_xliff_states_yes/
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1513 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/data/test_pocount_xliff_states_yes/states.xlf
--rw-r--r--   0 nijel     (1000) nijel     (1000)      504 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/data/test_pocount_xliff_states_yes/stdout.txt
-drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-05-15 15:14:10.533689 translate-toolkit-3.9.0/tests/cli/data/test_pofilter_listfilters/
--rw-r--r--   0 nijel     (1000) nijel     (1000)     3337 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/data/test_pofilter_listfilters/stdout.txt
-drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-05-15 15:14:10.533689 translate-toolkit-3.9.0/tests/cli/data/test_pofilter_manpage/
--rw-r--r--   0 nijel     (1000) nijel     (1000)     3421 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/data/test_pofilter_manpage/stdout.txt
-drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-05-15 15:14:10.533689 translate-toolkit-3.9.0/tests/cli/data/test_posegment/
--rw-r--r--   0 nijel     (1000) nijel     (1000)      370 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/data/test_posegment/one.po
--rw-r--r--   0 nijel     (1000) nijel     (1000)      388 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/data/test_posegment/out.po
-drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-05-15 15:14:10.533689 translate-toolkit-3.9.0/tests/cli/data/test_poswap_comments/
--rw-r--r--   0 nijel     (1000) nijel     (1000)      133 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/data/test_poswap_comments/af.po
--rw-r--r--   0 nijel     (1000) nijel     (1000)      130 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/data/test_poswap_comments/fr.po
--rw-r--r--   0 nijel     (1000) nijel     (1000)      133 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/data/test_poswap_comments/out.po
-drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-05-15 15:14:10.533689 translate-toolkit-3.9.0/tests/cli/data/test_poswap_fr_af/
--rw-r--r--   0 nijel     (1000) nijel     (1000)       86 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/data/test_poswap_fr_af/af.po
--rw-r--r--   0 nijel     (1000) nijel     (1000)       81 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/data/test_poswap_fr_af/fr.po
--rw-r--r--   0 nijel     (1000) nijel     (1000)       86 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/data/test_poswap_fr_af/out.po
-drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-05-15 15:14:10.533689 translate-toolkit-3.9.0/tests/cli/data/test_poswap_fr_af_reverse/
--rw-r--r--   0 nijel     (1000) nijel     (1000)       81 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/data/test_poswap_fr_af_reverse/fr.po
--rw-r--r--   0 nijel     (1000) nijel     (1000)       81 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/data/test_poswap_fr_af_reverse/fr_af.po
--rw-r--r--   0 nijel     (1000) nijel     (1000)       81 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/data/test_poswap_fr_af_reverse/out.po
-drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-05-15 15:14:10.533689 translate-toolkit-3.9.0/tests/cli/data/test_poswap_missing_units/
--rw-r--r--   0 nijel     (1000) nijel     (1000)       52 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/data/test_poswap_missing_units/af.po
--rw-r--r--   0 nijel     (1000) nijel     (1000)       54 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/data/test_poswap_missing_units/fr.po
--rw-r--r--   0 nijel     (1000) nijel     (1000)       49 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/data/test_poswap_missing_units/out.po
-drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-05-15 15:14:10.533689 translate-toolkit-3.9.0/tests/cli/data/test_prop2po/
--rw-r--r--   0 nijel     (1000) nijel     (1000)      322 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/data/test_prop2po/stderr.txt
-drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-05-15 15:14:10.533689 translate-toolkit-3.9.0/tests/cli/data/test_prop2po_dirs/
-drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-05-15 15:14:10.537689 translate-toolkit-3.9.0/tests/cli/data/test_prop2po_dirs/one/
--rw-r--r--   0 nijel     (1000) nijel     (1000)       10 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/data/test_prop2po_dirs/one/a.properties
-drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-05-15 15:14:10.537689 translate-toolkit-3.9.0/tests/cli/data/test_prop2po_dirs/out/
--rw-r--r--   0 nijel     (1000) nijel     (1000)      498 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/data/test_prop2po_dirs/out/a.po
--rw-r--r--   0 nijel     (1000) nijel     (1000)      144 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/data/test_prop2po_dirs/stderr.txt
-drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-05-15 15:14:10.537689 translate-toolkit-3.9.0/tests/cli/data/test_prop2po_files/
--rw-r--r--   0 nijel     (1000) nijel     (1000)       10 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/data/test_prop2po_files/one.properties
--rw-r--r--   0 nijel     (1000) nijel     (1000)      506 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/data/test_prop2po_files/out.po
-drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-05-15 15:14:10.537689 translate-toolkit-3.9.0/tests/cli/data/test_prop2po_files_templates/
--rw-r--r--   0 nijel     (1000) nijel     (1000)       10 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/data/test_prop2po_files_templates/one.properties
--rw-r--r--   0 nijel     (1000) nijel     (1000)      574 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/data/test_prop2po_files_templates/out.po
--rw-r--r--   0 nijel     (1000) nijel     (1000)       11 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/data/test_prop2po_files_templates/two.properties
-drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-05-15 15:14:10.537689 translate-toolkit-3.9.0/tests/cli/data/test_rc2po/
--rw-r--r--   0 nijel     (1000) nijel     (1000)     3564 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/data/test_rc2po/one.rc
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1882 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/data/test_rc2po/out.po
--rw-r--r--   0 nijel     (1000) nijel     (1000)      727 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/example_test.sh
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)      226 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/run_tests.sh
--rw-r--r--   0 nijel     (1000) nijel     (1000)     4775 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/test.inc.sh
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)      127 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/test_flatxml2po.sh
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)      141 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/test_flatxml2po_wrongkey.sh
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)      147 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/test_flatxml2po_wrongns.sh
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)      142 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/test_flatxml2po_wrongroot.sh
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)      143 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/test_flatxml2po_wrongvalue.sh
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)      107 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/test_junitmsgfmt_failure.sh
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)      122 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/test_junitmsgfmt_untranslated.sh
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)      123 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/test_po2csv.sh
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)      127 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/test_po2flatxml.sh
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)      252 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/test_po2flatxml_params.sh
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)      141 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/test_po2flatxml_preserve.sh
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)      266 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/test_po2flatxml_template.sh
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)      137 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/test_po2html.sh
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)      167 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/test_po2json_files_removeuntranslated.sh
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)      168 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/test_po2prop_mozilla_files.sh
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)      122 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/test_po2ts.sh
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)      123 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/test_po2txt.sh
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)      194 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/test_po2txt_threshold.sh
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)      135 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/test_pocount.sh
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)      114 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/test_pocount_mutually_exclusive.sh
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)      109 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/test_pocount_nonexistant.sh
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)      114 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/test_pocount_po_file.sh
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)      114 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/test_pocount_po_fuzzy.sh
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)      117 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/test_pocount_xliff_states_no.sh
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)      117 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/test_pocount_xliff_states_yes.sh
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)      113 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/test_pofilter_listfilters.sh
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)      182 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/test_pofilter_manpage.sh
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)      126 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/test_posegment.sh
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)      147 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/test_poswap_comments.sh
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)      147 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/test_poswap_fr_af.sh
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)      160 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/test_poswap_fr_af_reverse.sh
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)      147 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/test_poswap_missing_units.sh
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)       98 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/test_prop2po.sh
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)      108 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/test_prop2po_dirs.sh
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)      124 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/test_prop2po_files.sh
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)      132 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/test_prop2po_files_templates.sh
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)      128 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/test_rc2po.sh
-drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-05-15 15:14:10.537689 translate-toolkit-3.9.0/tests/odf_xliff/
--rw-r--r--   0 nijel     (1000) nijel     (1000)     3085 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/odf_xliff/test_2-test_odf2xliff-reference.xlf
--rw-r--r--   0 nijel     (1000) nijel     (1000)   133081 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/odf_xliff/test_2.odt
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1864 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/odf_xliff/test_inline-test_odf2xliff_inline-reference.xlf
--rw-r--r--   0 nijel     (1000) nijel     (1000)     7300 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/odf_xliff/test_inline.odt
--rw-r--r--   0 nijel     (1000) nijel     (1000)     5466 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/odf_xliff/test_odf_xliff.py
-drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-05-15 15:14:10.541689 translate-toolkit-3.9.0/tests/xliff_conformance/
--rw-r--r--   0 nijel     (1000) nijel     (1000)    36103 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/xliff_conformance/af-pootle.po
--rw-r--r--   0 nijel     (1000) nijel     (1000)    30075 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/xliff_conformance/en-US.sdf
--rw-r--r--   0 nijel     (1000) nijel     (1000)     2257 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/xliff_conformance/test_xliff_conformance.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)    96911 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/xliff_conformance/xliff-core-1.1.xsd
-drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-05-15 15:14:10.541689 translate-toolkit-3.9.0/tools/
-drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-05-15 15:14:10.545689 translate-toolkit-3.9.0/tools/mozilla/
--rw-r--r--   0 nijel     (1000) nijel     (1000)     7012 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tools/mozilla/README.firefox_build_instructions.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     4102 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tools/mozilla/Vagrantfile
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)     3429 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tools/mozilla/accesskey_checker
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)     2546 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tools/mozilla/accesskey_checker_PO
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)    12855 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tools/mozilla/build_firefox.sh
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)     7178 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tools/mozilla/build_tb3_langs.sh
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)     9665 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tools/mozilla/buildxpi.py
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)      158 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tools/mozilla/compare-locales.sh
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)     4495 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tools/mozilla/get_moz_enUS.py
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)    11342 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tools/mozilla/moz-l10n-builder
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)    23575 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tools/mozilla/moz_l10n_builder.py
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)     2257 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tools/mozilla/mozcronbuild.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1487 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tools/mozilla/mozilla-l10n.patch
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)    12089 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tools/mozilla/mozzy.sh
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)     3208 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tools/mozilla/postinstall.sh
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)      497 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tools/mozilla/setup_mozilla.sh
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)    18996 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tools/phase
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)      626 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tools/phaselist2goals
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)     1041 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tools/pocommentclean
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)     4683 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tools/pocompendium
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)     5288 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tools/pomigrate2
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)     1852 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tools/popuretext
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)     1121 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tools/poreencode
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)     1526 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tools/posplit
-drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-05-15 15:14:10.545689 translate-toolkit-3.9.0/translate/
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1816 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/__init__.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1406 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/__version__.py
-drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-05-15 15:14:10.565689 translate-toolkit-3.9.0/translate/convert/
--rw-r--r--   0 nijel     (1000) nijel     (1000)      790 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/convert/__init__.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     8225 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/convert/accesskey.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)    20603 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/convert/convert.py
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)    10171 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/convert/csv2po.py
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)     3325 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/convert/csv2tbx.py
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)    13191 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/convert/dtd2po.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     7541 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/convert/factory.py
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)     3663 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/convert/flatxml2po.py
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)     5523 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/convert/html2po.py
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)     4527 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/convert/ical2po.py
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)     1902 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/convert/idml2po.py
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)     5078 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/convert/ini2po.py
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)     5180 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/convert/json2po.py
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)     2358 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/convert/moz2po.py
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)     4922 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/convert/mozfunny2prop.py
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)     3981 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/convert/mozlang2po.py
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)     3839 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/convert/odf2xliff.py
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)      357 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/convert/odfxml
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)     7936 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/convert/oo2po.py
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)     7286 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/convert/oo2xliff.py
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)     4536 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/convert/php2po.py
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)     3950 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/convert/po2csv.py
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)     8688 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/convert/po2dtd.py
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)     5083 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/convert/po2flatxml.py
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)     6792 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/convert/po2html.py
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)     3617 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/convert/po2ical.py
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)     6806 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/convert/po2idml.py
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)     4107 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/convert/po2ini.py
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)     3682 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/convert/po2json.py
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)     3490 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/convert/po2moz.py
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)     3702 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/convert/po2mozlang.py
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)    11233 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/convert/po2oo.py
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)     3374 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/convert/po2php.py
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)    12940 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/convert/po2prop.py
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)    13213 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/convert/po2rc.py
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)     3195 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/convert/po2resx.py
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)     2821 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/convert/po2sub.py
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)     4085 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/convert/po2symb.py
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)     3227 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/convert/po2tiki.py
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)     5569 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/convert/po2tmx.py
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)     3228 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/convert/po2ts.py
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)     5171 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/convert/po2txt.py
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)     2559 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/convert/po2web2py.py
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)     4185 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/convert/po2wordfast.py
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)     4287 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/convert/po2xliff.py
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)     3949 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/convert/po2yaml.py
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)    12222 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/convert/pot2po.py
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)     6230 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/convert/prop2mozfunny.py
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)    18818 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/convert/prop2po.py
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)     5941 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/convert/rc2po.py
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)     6038 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/convert/resx2po.py
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)     1730 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/convert/roundtrip-OOo
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)     1629 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/convert/roundtrip-gaia
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)     1589 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/convert/roundtrip-mozilla
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)     4776 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/convert/sub2po.py
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)     4101 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/convert/symb2po.py
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)     2352 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/convert/tbx2po.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)   189411 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/convert/test.idml
--rw-r--r--   0 nijel     (1000) nijel     (1000)    11608 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/convert/test.odt
--rw-r--r--   0 nijel     (1000) nijel     (1000)     4655 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/convert/test_accesskey.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     5372 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/convert/test_convert.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     6225 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/convert/test_csv2po.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)    19205 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/convert/test_dtd2po.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     4744 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/convert/test_flatxml2po.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)    27945 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/convert/test_html2po.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)    12076 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/convert/test_ical2po.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)      449 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/convert/test_idml2po.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     4543 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/convert/test_ini2po.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     2472 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/convert/test_json2po.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)      414 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/convert/test_moz2po.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     2179 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/convert/test_mozfunny2prop.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     4733 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/convert/test_mozlang2po.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)      446 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/convert/test_ods2xliff.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)    13063 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/convert/test_oo2po.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     2989 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/convert/test_oo2xliff.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)    11579 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/convert/test_php2po.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     5969 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/convert/test_po2csv.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)    22148 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/convert/test_po2dtd.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     4617 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/convert/test_po2flatxml.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)    11889 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/convert/test_po2html.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)    10814 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/convert/test_po2ical.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)      826 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/convert/test_po2idml.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     8117 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/convert/test_po2ini.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     3853 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/convert/test_po2json.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)      494 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/convert/test_po2moz.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     5024 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/convert/test_po2mozlang.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     9663 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/convert/test_po2oo.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)    10874 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/convert/test_po2php.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)    17564 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/convert/test_po2prop.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     9084 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/convert/test_po2rc.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)    18992 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/convert/test_po2resx.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     2151 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/convert/test_po2sub.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     2097 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/convert/test_po2tiki.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     6522 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/convert/test_po2tmx.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     4373 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/convert/test_po2ts.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     5238 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/convert/test_po2txt.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1967 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/convert/test_po2web2py.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)    10413 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/convert/test_po2xliff.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     6837 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/convert/test_po2yaml.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)    27471 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/convert/test_pot2po.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     2201 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/convert/test_prop2mozfunny.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)    14486 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/convert/test_prop2po.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     4827 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/convert/test_rc2po.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)    10049 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/convert/test_resx2po.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     2362 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/convert/test_tiki2po.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     4628 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/convert/test_ts2po.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     8333 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/convert/test_txt2po.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1823 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/convert/test_web2py2po.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)      942 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/convert/test_xliff2odf.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)    12996 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/convert/test_xliff2po.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     5143 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/convert/test_yaml2po.py
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)     3144 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/convert/tiki2po.py
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)     3774 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/convert/ts2po.py
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)     4682 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/convert/txt2po.py
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)     2757 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/convert/web2py2po.py
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)     5947 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/convert/xliff2odf.py
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)    11230 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/convert/xliff2oo.py
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)     4049 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/convert/xliff2po.py
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)     4458 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/convert/yaml2po.py
-drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-05-15 15:14:10.569689 translate-toolkit-3.9.0/translate/filters/
--rw-r--r--   0 nijel     (1000) nijel     (1000)      766 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/filters/__init__.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     2440 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/filters/autocorrect.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)   101819 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/filters/checks.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)    10481 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/filters/decoration.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1940 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/filters/decorators.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     2796 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/filters/helpers.py
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)    13302 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/filters/pofilter.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     6133 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/filters/prefilters.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     2153 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/filters/spelling.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     2531 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/filters/test_autocorrect.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)   108937 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/filters/test_checks.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     4060 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/filters/test_decoration.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)    13635 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/filters/test_pofilter.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1065 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/filters/test_prefilters.py
-drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-05-15 15:14:10.585689 translate-toolkit-3.9.0/translate/lang/
--rw-r--r--   0 nijel     (1000) nijel     (1000)      969 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/lang/__init__.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     3868 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/lang/af.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)      925 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/lang/ak.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1513 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/lang/am.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     2090 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/lang/ar.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)      974 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/lang/az.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     2096 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/lang/bn.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)      973 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/lang/bo.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1458 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/lang/code_as.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1551 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/lang/code_or.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)    13174 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/lang/common.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1081 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/lang/da.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)    27413 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/lang/data.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)      976 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/lang/de.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)      976 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/lang/dz.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1949 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/lang/el.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1782 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/lang/es.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     3632 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/lang/fa.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     2488 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/lang/factory.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)      985 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/lang/fi.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     2849 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/lang/fr.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)      969 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/lang/gd.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)      983 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/lang/gu.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)      983 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/lang/he.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)      974 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/lang/hi.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1821 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/lang/hy.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     4934 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/lang/identify.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1699 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/lang/ja.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1977 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/lang/km.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)      980 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/lang/kn.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)      971 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/lang/ko.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)      973 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/lang/kw.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)      967 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/lang/lo.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)      986 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/lang/ml.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)      980 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/lang/mr.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)      967 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/lang/ms.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1042 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/lang/my.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1637 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/lang/ne.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     4893 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/lang/ngram.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1413 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/lang/nqo.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)      952 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/lang/nso.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1614 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/lang/pa.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1079 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/lang/pl.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     5968 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/lang/poedit.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1100 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/lang/pt_BR.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     2828 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/lang/ro.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     5382 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/lang/scn.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)      992 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/lang/si.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)      963 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/lang/son.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)      940 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/lang/st.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)      979 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/lang/su.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1080 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/lang/sv.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)      978 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/lang/ta.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)      971 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/lang/te.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)    21016 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/lang/team.py
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)      707 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/lang/test-language-teams.sh
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1690 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/lang/test_af.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1119 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/lang/test_am.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1388 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/lang/test_ar.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     5162 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/lang/test_common.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     4131 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/lang/test_data.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1417 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/lang/test_el.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1273 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/lang/test_es.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     2815 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/lang/test_fa.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1918 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/lang/test_factory.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     3107 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/lang/test_fr.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1448 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/lang/test_hy.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     6480 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/lang/test_identify.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1116 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/lang/test_ja.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1829 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/lang/test_km.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1094 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/lang/test_ko.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     2963 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/lang/test_ne.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1751 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/lang/test_nqo.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1639 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/lang/test_or.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)      705 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/lang/test_poedit.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1737 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/lang/test_ro.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1869 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/lang/test_scn.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)      775 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/lang/test_team.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)      632 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/lang/test_th.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)      405 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/lang/test_tr.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)      328 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/lang/test_uk.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1426 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/lang/test_vi.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1008 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/lang/test_zh.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1181 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/lang/th.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1025 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/lang/tr.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1091 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/lang/ug.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1186 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/lang/ur.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)      952 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/lang/ve.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1532 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/lang/vi.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1655 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/lang/wo.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     2367 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/lang/zh.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1016 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/lang/zh_cn.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1029 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/lang/zh_hk.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1029 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/lang/zh_tw.py
-drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-05-15 15:14:10.589689 translate-toolkit-3.9.0/translate/misc/
--rw-r--r--   0 nijel     (1000) nijel     (1000)      838 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/misc/__init__.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1610 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/misc/deprecation.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     2733 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/misc/dictutils.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     2580 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/misc/file_discovery.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     3010 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/misc/multistring.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)    33419 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/misc/optrecurse.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)    10453 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/misc/ourdom.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     4655 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/misc/progressbar.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)    17756 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/misc/quote.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)    17681 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/misc/selector.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)      465 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/misc/test_deprecation.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)      234 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/misc/test_dictutils.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     3052 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/misc/test_multistring.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1133 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/misc/test_optrecurse.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)      419 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/misc/test_progressbar.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     7634 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/misc/test_quote.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1209 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/misc/test_xml_helpers.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1424 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/misc/wStringIO.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1138 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/misc/wsgi.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     6869 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/misc/xml_helpers.py
-drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-05-15 15:14:10.589689 translate-toolkit-3.9.0/translate/search/
--rw-r--r--   0 nijel     (1000) nijel     (1000)      772 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/search/__init__.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     6056 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/search/lshtein.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)    15948 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/search/match.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1754 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/search/terminology.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1866 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/search/test_lshtein.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     5705 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/search/test_match.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)      307 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/search/test_terminology.py
-drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-05-15 15:14:10.589689 translate-toolkit-3.9.0/translate/services/
--rw-r--r--   0 nijel     (1000) nijel     (1000)      833 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/services/__init__.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1855 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/services/test_tmserver.py
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)     8293 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/services/tmserver.py
-drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-05-15 15:14:10.589689 translate-toolkit-3.9.0/translate/share/
-drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-05-15 15:14:10.601689 translate-toolkit-3.9.0/translate/share/langmodels/
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1449 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/share/langmodels/Ndebele.lm
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1481 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/share/langmodels/NorthernSotho.lm
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1071 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/share/langmodels/README
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1463 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/share/langmodels/Sotho.lm
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1463 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/share/langmodels/Swati.lm
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1447 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/share/langmodels/Tsonga.lm
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1475 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/share/langmodels/Tswana.lm
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1457 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/share/langmodels/Venda.lm
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1421 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/share/langmodels/Xhosa.lm
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1464 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/share/langmodels/Zulu.lm
--rw-r--r--   0 nijel     (1000) nijel     (1000)     3387 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/share/langmodels/afrikaans.lm
--rw-r--r--   0 nijel     (1000) nijel     (1000)     3355 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/share/langmodels/albanian.lm
--rw-r--r--   0 nijel     (1000) nijel     (1000)     2325 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/share/langmodels/arabic.lm
--rw-r--r--   0 nijel     (1000) nijel     (1000)     3243 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/share/langmodels/basque.lm
--rw-r--r--   0 nijel     (1000) nijel     (1000)     2195 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/share/langmodels/belarus.lm
--rw-r--r--   0 nijel     (1000) nijel     (1000)     3131 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/share/langmodels/bosnian.lm
--rw-r--r--   0 nijel     (1000) nijel     (1000)     3287 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/share/langmodels/breton.lm
--rw-r--r--   0 nijel     (1000) nijel     (1000)     3223 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/share/langmodels/catalan.lm
--rw-r--r--   0 nijel     (1000) nijel     (1000)     2089 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/share/langmodels/chinese_simplified.lm
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1991 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/share/langmodels/chinese_traditional.lm
--rw-r--r--   0 nijel     (1000) nijel     (1000)     3428 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/share/langmodels/croatian.lm
--rw-r--r--   0 nijel     (1000) nijel     (1000)     3369 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/share/langmodels/czech.lm
--rw-r--r--   0 nijel     (1000) nijel     (1000)     3375 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/share/langmodels/danish.lm
--rw-r--r--   0 nijel     (1000) nijel     (1000)     3384 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/share/langmodels/dutch.lm
--rw-r--r--   0 nijel     (1000) nijel     (1000)     3317 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/share/langmodels/english.lm
--rw-r--r--   0 nijel     (1000) nijel     (1000)     3427 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/share/langmodels/esperanto.lm
--rw-r--r--   0 nijel     (1000) nijel     (1000)     3315 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/share/langmodels/estonian.lm
--rw-r--r--   0 nijel     (1000) nijel     (1000)     3425 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/share/langmodels/finnish.lm
--rw-r--r--   0 nijel     (1000) nijel     (1000)     3687 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/share/langmodels/fpdb.conf
--rw-r--r--   0 nijel     (1000) nijel     (1000)     3355 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/share/langmodels/french.lm
--rw-r--r--   0 nijel     (1000) nijel     (1000)     3443 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/share/langmodels/frisian.lm
--rw-r--r--   0 nijel     (1000) nijel     (1000)     3444 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/share/langmodels/german.lm
--rw-r--r--   0 nijel     (1000) nijel     (1000)     4266 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/share/langmodels/greek.lm
--rw-r--r--   0 nijel     (1000) nijel     (1000)     4187 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/share/langmodels/hebrew.lm
--rw-r--r--   0 nijel     (1000) nijel     (1000)     3353 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/share/langmodels/hungarian.lm
--rw-r--r--   0 nijel     (1000) nijel     (1000)     3475 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/share/langmodels/icelandic.lm
--rw-r--r--   0 nijel     (1000) nijel     (1000)     3359 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/share/langmodels/indonesian.lm
--rw-r--r--   0 nijel     (1000) nijel     (1000)     3178 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/share/langmodels/irish_gaelic.lm
--rw-r--r--   0 nijel     (1000) nijel     (1000)     3426 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/share/langmodels/italian.lm
--rw-r--r--   0 nijel     (1000) nijel     (1000)     2309 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/share/langmodels/japanese.lm
--rw-r--r--   0 nijel     (1000) nijel     (1000)     3324 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/share/langmodels/latin.lm
--rw-r--r--   0 nijel     (1000) nijel     (1000)     3500 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/share/langmodels/latvian.lm
--rw-r--r--   0 nijel     (1000) nijel     (1000)     3350 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/share/langmodels/lithuanian.lm
--rw-r--r--   0 nijel     (1000) nijel     (1000)     3597 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/share/langmodels/malay.lm
--rw-r--r--   0 nijel     (1000) nijel     (1000)     3462 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/share/langmodels/manx_gaelic.lm
--rw-r--r--   0 nijel     (1000) nijel     (1000)     3408 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/share/langmodels/norwegian.lm
--rw-r--r--   0 nijel     (1000) nijel     (1000)     3416 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/share/langmodels/polish.lm
--rw-r--r--   0 nijel     (1000) nijel     (1000)     3467 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/share/langmodels/portuguese.lm
--rw-r--r--   0 nijel     (1000) nijel     (1000)     3205 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/share/langmodels/quechua.lm
--rw-r--r--   0 nijel     (1000) nijel     (1000)     3297 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/share/langmodels/romanian.lm
--rw-r--r--   0 nijel     (1000) nijel     (1000)     3117 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/share/langmodels/romansh.lm
--rw-r--r--   0 nijel     (1000) nijel     (1000)     4146 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/share/langmodels/russian.lm
--rw-r--r--   0 nijel     (1000) nijel     (1000)     3131 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/share/langmodels/scots.lm
--rw-r--r--   0 nijel     (1000) nijel     (1000)     3323 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/share/langmodels/scots_gaelic.lm
--rw-r--r--   0 nijel     (1000) nijel     (1000)     3420 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/share/langmodels/serbian_ascii.lm
--rw-r--r--   0 nijel     (1000) nijel     (1000)     3239 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/share/langmodels/slovak_ascii.lm
--rw-r--r--   0 nijel     (1000) nijel     (1000)     3152 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/share/langmodels/slovenian.lm
--rw-r--r--   0 nijel     (1000) nijel     (1000)     3417 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/share/langmodels/spanish.lm
--rw-r--r--   0 nijel     (1000) nijel     (1000)     3314 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/share/langmodels/swahili.lm
--rw-r--r--   0 nijel     (1000) nijel     (1000)     3484 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/share/langmodels/swedish.lm
--rw-r--r--   0 nijel     (1000) nijel     (1000)     3261 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/share/langmodels/tagalog.lm
--rw-r--r--   0 nijel     (1000) nijel     (1000)     3539 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/share/langmodels/turkish.lm
--rw-r--r--   0 nijel     (1000) nijel     (1000)     2172 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/share/langmodels/ukrainian.lm
--rw-r--r--   0 nijel     (1000) nijel     (1000)     3689 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/share/langmodels/vietnamese.lm
--rw-r--r--   0 nijel     (1000) nijel     (1000)     3535 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/share/langmodels/welsh.lm
--rw-r--r--   0 nijel     (1000) nijel     (1000)     8740 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/share/stoplist-en
-drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-05-15 15:14:10.621689 translate-toolkit-3.9.0/translate/storage/
--rw-r--r--   0 nijel     (1000) nijel     (1000)      786 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/storage/__init__.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1324 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/storage/_factory_classes.py
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)    22457 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/storage/aresource.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)    34064 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/storage/base.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     7514 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/storage/benchmark.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)    10410 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/storage/bundleprojstore.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)    10970 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/storage/catkeys.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)    37641 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/storage/cpo.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)    11481 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/storage/csvl10n.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)      338 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/storage/debug.properties
--rw-r--r--   0 nijel     (1000) nijel     (1000)     2383 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/storage/directory.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)    24352 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/storage/dtd.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     8762 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/storage/factory.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     8204 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/storage/flatxml.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)    24555 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/storage/fluent.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)    19719 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/storage/fpo.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)    17147 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/storage/html.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     4972 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/storage/ical.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     2846 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/storage/idml.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     4515 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/storage/ini.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)    25065 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/storage/jsonl10n.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)    13083 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/storage/lisa.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)    10982 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/storage/mo.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     5500 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/storage/mozilla_lang.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1165 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/storage/odf_io.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     5390 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/storage/odf_shared.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     6139 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/storage/omegat.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)    15688 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/storage/oo.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)    18547 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/storage/php.py
-drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-05-15 15:14:10.621689 translate-toolkit-3.9.0/translate/storage/placeables/
--rw-r--r--   0 nijel     (1000) nijel     (1000)     2004 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/storage/placeables/__init__.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     2962 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/storage/placeables/base.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)    13901 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/storage/placeables/general.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1241 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/storage/placeables/interfaces.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     7195 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/storage/placeables/lisa.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     3269 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/storage/placeables/parse.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)    35646 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/storage/placeables/strelem.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     3297 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/storage/placeables/terminology.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     8107 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/storage/placeables/test_base.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)    10622 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/storage/placeables/test_general.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     6121 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/storage/placeables/test_lisa.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     2029 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/storage/placeables/test_terminology.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     3991 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/storage/placeables/xliff.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1693 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/storage/po.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     7092 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/storage/pocommon.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)    16276 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/storage/poheader.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)    13215 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/storage/poparser.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)    12932 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/storage/poxliff.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     9143 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/storage/project.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)    14695 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/storage/projstore.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)      753 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/storage/properties.java
--rw-r--r--   0 nijel     (1000) nijel     (1000)    43632 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/storage/properties.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)    37283 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/storage/pypo.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     8559 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/storage/qm.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     5127 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/storage/qph.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)    16053 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/storage/rc.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1649 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/storage/resourcedictionary.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     8538 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/storage/resx.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     7567 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/storage/statistics.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     6662 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/storage/stringsdict.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     7652 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/storage/subtitles.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     2234 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/storage/symbian.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     4531 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/storage/tbx.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)    30744 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/storage/test_aresource.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)    14765 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/storage/test_base.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     2492 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/storage/test_catkeys.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     9086 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/storage/test_cpo.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     5570 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/storage/test_csvl10n.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     2798 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/storage/test_directory.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)    21418 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/storage/test_dtd.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     6704 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/storage/test_factory.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     3869 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/storage/test_flatxml.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)    71615 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/storage/test_fluent.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     9820 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/storage/test_html.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)      483 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/storage/test_ini.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)    28694 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/storage/test_jsonl10n.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     8420 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/storage/test_mo.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1296 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/storage/test_monolingual.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)    10207 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/storage/test_mozilla_lang.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)      501 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/storage/test_omegat.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     6658 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/storage/test_oo.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)    44427 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/storage/test_php.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)    38517 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/storage/test_po.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)      675 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/storage/test_pocommon.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)    11275 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/storage/test_poheader.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     5392 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/storage/test_poxliff.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)    64201 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/storage/test_properties.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)    22936 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/storage/test_pypo.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1198 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/storage/test_qm.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     3239 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/storage/test_qph.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)    18737 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/storage/test_rc.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1928 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/storage/test_resourcedictionary.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     5022 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/storage/test_resx.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     6114 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/storage/test_stringsdict.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)      743 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/storage/test_subtitles.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     3558 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/storage/test_tbx.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     3146 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/storage/test_tiki.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     3916 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/storage/test_tmx.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)      882 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/storage/test_trados.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)      211 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/storage/test_ts.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)    13697 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/storage/test_ts2.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     2002 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/storage/test_txt.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)      207 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/storage/test_utx.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     2847 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/storage/test_wordfast.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)    25248 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/storage/test_xliff.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)    15664 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/storage/test_yaml.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     2697 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/storage/test_zip.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     6986 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/storage/tiki.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)    13004 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/storage/tmdb.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     5845 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/storage/tmx.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     6409 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/storage/trados.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     6935 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/storage/ts.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)    17854 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/storage/ts2.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     4994 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/storage/txt.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     9488 2023-05-15 15:11:38.000000 translate-toolkit-3.9.0/translate/storage/utx.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)    15187 2023-05-15 15:11:38.000000 translate-toolkit-3.9.0/translate/storage/wordfast.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     8786 2023-05-15 15:11:38.000000 translate-toolkit-3.9.0/translate/storage/workflow.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)    33543 2023-05-15 15:11:38.000000 translate-toolkit-3.9.0/translate/storage/xliff.py
-drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-05-15 15:14:10.625689 translate-toolkit-3.9.0/translate/storage/xml_extract/
--rw-r--r--   0 nijel     (1000) nijel     (1000)      716 2023-05-15 15:11:38.000000 translate-toolkit-3.9.0/translate/storage/xml_extract/__init__.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)    14635 2023-05-15 15:11:38.000000 translate-toolkit-3.9.0/translate/storage/xml_extract/extract.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)    11240 2023-05-15 15:11:38.000000 translate-toolkit-3.9.0/translate/storage/xml_extract/generate.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     2825 2023-05-15 15:11:38.000000 translate-toolkit-3.9.0/translate/storage/xml_extract/misc.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     2166 2023-05-15 15:11:38.000000 translate-toolkit-3.9.0/translate/storage/xml_extract/test_misc.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     2955 2023-05-15 15:11:38.000000 translate-toolkit-3.9.0/translate/storage/xml_extract/test_unit_tree.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1205 2023-05-15 15:11:38.000000 translate-toolkit-3.9.0/translate/storage/xml_extract/test_xpath_breadcrumb.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     4854 2023-05-15 15:11:38.000000 translate-toolkit-3.9.0/translate/storage/xml_extract/unit_tree.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     2230 2023-05-15 15:11:38.000000 translate-toolkit-3.9.0/translate/storage/xml_extract/xpath_breadcrumb.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     2677 2023-05-15 15:11:38.000000 translate-toolkit-3.9.0/translate/storage/xml_name.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     7211 2023-05-15 15:11:38.000000 translate-toolkit-3.9.0/translate/storage/yaml.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     2276 2023-05-15 15:11:38.000000 translate-toolkit-3.9.0/translate/storage/zip.py
-drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-05-15 15:14:10.629689 translate-toolkit-3.9.0/translate/tools/
--rw-r--r--   0 nijel     (1000) nijel     (1000)      777 2023-05-15 15:11:38.000000 translate-toolkit-3.9.0/translate/tools/__init__.py
-drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-05-15 15:14:10.629689 translate-toolkit-3.9.0/translate/tools/__snapshots__/
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1871 2023-05-15 15:11:38.000000 translate-toolkit-3.9.0/translate/tools/__snapshots__/test_junitmsgfmt.ambr
--rw-r--r--   0 nijel     (1000) nijel     (1000)    10626 2023-05-15 15:11:38.000000 translate-toolkit-3.9.0/translate/tools/__snapshots__/test_pocount.ambr
--rw-r--r--   0 nijel     (1000) nijel     (1000)      301 2023-05-15 15:11:38.000000 translate-toolkit-3.9.0/translate/tools/_test_utils.py
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)     3350 2023-05-15 15:11:38.000000 translate-toolkit-3.9.0/translate/tools/build_tmdb.py
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)     2844 2023-05-15 15:11:38.000000 translate-toolkit-3.9.0/translate/tools/junitmsgfmt.py
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)     3415 2023-05-15 15:11:38.000000 translate-toolkit-3.9.0/translate/tools/phppo2pypo.py
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)     2363 2023-05-15 15:11:38.000000 translate-toolkit-3.9.0/translate/tools/poclean.py
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)     3408 2023-05-15 15:11:38.000000 translate-toolkit-3.9.0/translate/tools/pocompile.py
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)     8679 2023-05-15 15:11:38.000000 translate-toolkit-3.9.0/translate/tools/poconflicts.py
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)    19130 2023-05-15 15:11:38.000000 translate-toolkit-3.9.0/translate/tools/pocount.py
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)    16454 2023-05-15 15:11:38.000000 translate-toolkit-3.9.0/translate/tools/podebug.py
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)    14678 2023-05-15 15:11:38.000000 translate-toolkit-3.9.0/translate/tools/pogrep.py
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)     5292 2023-05-15 15:11:38.000000 translate-toolkit-3.9.0/translate/tools/pomerge.py
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)     5643 2023-05-15 15:11:38.000000 translate-toolkit-3.9.0/translate/tools/porestructure.py
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)     4954 2023-05-15 15:11:38.000000 translate-toolkit-3.9.0/translate/tools/posegment.py
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)     3720 2023-05-15 15:11:38.000000 translate-toolkit-3.9.0/translate/tools/poswap.py
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)    25251 2023-05-15 15:11:38.000000 translate-toolkit-3.9.0/translate/tools/poterminology.py
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)     9213 2023-05-15 15:11:38.000000 translate-toolkit-3.9.0/translate/tools/pretranslate.py
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)    12659 2023-05-15 15:11:38.000000 translate-toolkit-3.9.0/translate/tools/pydiff.py
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)     3384 2023-05-15 15:11:38.000000 translate-toolkit-3.9.0/translate/tools/pypo2phppo.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)      714 2023-05-15 15:11:38.000000 translate-toolkit-3.9.0/translate/tools/test_help.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)      548 2023-05-15 15:11:38.000000 translate-toolkit-3.9.0/translate/tools/test_junitmsgfmt.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1710 2023-05-15 15:11:38.000000 translate-toolkit-3.9.0/translate/tools/test_phppo2pypo.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     5751 2023-05-15 15:11:38.000000 translate-toolkit-3.9.0/translate/tools/test_pocount.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)    11912 2023-05-15 15:11:38.000000 translate-toolkit-3.9.0/translate/tools/test_podebug.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     8182 2023-05-15 15:11:38.000000 translate-toolkit-3.9.0/translate/tools/test_pogrep.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)    23743 2023-05-15 15:11:38.000000 translate-toolkit-3.9.0/translate/tools/test_pomerge.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     3529 2023-05-15 15:11:38.000000 translate-toolkit-3.9.0/translate/tools/test_posegment.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)      945 2023-05-15 15:11:38.000000 translate-toolkit-3.9.0/translate/tools/test_poterminology.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)    14618 2023-05-15 15:11:38.000000 translate-toolkit-3.9.0/translate/tools/test_pretranslate.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1709 2023-05-15 15:11:38.000000 translate-toolkit-3.9.0/translate/tools/test_pypo2phppo.py
-drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-05-15 15:14:10.629689 translate-toolkit-3.9.0/translate_toolkit.egg-info/
--rw-r--r--   0 nijel     (1000) nijel     (1000)    10835 2023-05-15 15:14:10.000000 translate-toolkit-3.9.0/translate_toolkit.egg-info/PKG-INFO
--rw-r--r--   0 nijel     (1000) nijel     (1000)    28961 2023-05-15 15:14:10.000000 translate-toolkit-3.9.0/translate_toolkit.egg-info/SOURCES.txt
--rw-r--r--   0 nijel     (1000) nijel     (1000)        1 2023-05-15 15:14:10.000000 translate-toolkit-3.9.0/translate_toolkit.egg-info/dependency_links.txt
--rw-r--r--   0 nijel     (1000) nijel     (1000)     3197 2023-05-15 15:14:10.000000 translate-toolkit-3.9.0/translate_toolkit.egg-info/entry_points.txt
--rw-r--r--   0 nijel     (1000) nijel     (1000)        1 2023-05-15 15:14:10.000000 translate-toolkit-3.9.0/translate_toolkit.egg-info/not-zip-safe
--rw-r--r--   0 nijel     (1000) nijel     (1000)      629 2023-05-15 15:14:10.000000 translate-toolkit-3.9.0/translate_toolkit.egg-info/requires.txt
--rw-r--r--   0 nijel     (1000) nijel     (1000)       10 2023-05-15 15:14:10.000000 translate-toolkit-3.9.0/translate_toolkit.egg-info/top_level.txt
+drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-06-14 06:36:35.085624 translate-toolkit-3.9.1/
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      135 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/.deepsource.toml
+drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-06-14 06:36:34.941624 translate-toolkit-3.9.1/.github/
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      349 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/.github/dependabot.yml
+drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-06-14 06:36:34.941624 translate-toolkit-3.9.1/.github/matchers/
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      292 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/.github/matchers/flake8.json
+drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-06-14 06:36:34.941624 translate-toolkit-3.9.1/.github/workflows/
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      734 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/.github/workflows/docs.yml
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1808 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/.github/workflows/linux.yml
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1345 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/.github/workflows/osx.yml
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1764 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/.github/workflows/pre-commit.yml
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1693 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/.github/workflows/setup.yml
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1129 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/.github/workflows/win.yml
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      724 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/.gitignore
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      102 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/.gitmodules
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1166 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/.pre-commit-config.yaml
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      569 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/.readthedocs.yml
+-rw-r--r--   0 nijel     (1000) nijel     (1000)    17992 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/COPYING
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1768 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/CREDITS
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      171 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/LICENSES
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      305 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/MANIFEST.in
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     2925 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/Makefile
+-rw-r--r--   0 nijel     (1000) nijel     (1000)    10785 2023-06-14 06:36:35.085624 translate-toolkit-3.9.1/PKG-INFO
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     8810 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/README.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)       15 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/codecov.yml
+drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-06-14 06:36:34.945624 translate-toolkit-3.9.1/docs/
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     5743 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/docs/Makefile
+drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-06-14 06:36:34.945624 translate-toolkit-3.9.1/docs/_ext/
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1016 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/docs/_ext/translate_docs.py
+drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-06-14 06:36:34.945624 translate-toolkit-3.9.1/docs/_static/
+-rw-r--r--   0 nijel     (1000) nijel     (1000)       55 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/docs/_static/README.txt
+drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-06-14 06:36:34.945624 translate-toolkit-3.9.1/docs/_themes/
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      703 2023-06-14 06:35:43.000000 translate-toolkit-3.9.1/docs/_themes/README.rst
+drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-06-14 06:36:34.945624 translate-toolkit-3.9.1/docs/_themes/sphinx-bootstrap/
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      200 2023-06-14 06:35:43.000000 translate-toolkit-3.9.1/docs/_themes/sphinx-bootstrap/globaltoc.html
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     2628 2023-06-14 06:35:43.000000 translate-toolkit-3.9.1/docs/_themes/sphinx-bootstrap/layout.html
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      227 2023-06-14 06:35:43.000000 translate-toolkit-3.9.1/docs/_themes/sphinx-bootstrap/localtoc.html
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      304 2023-06-14 06:35:43.000000 translate-toolkit-3.9.1/docs/_themes/sphinx-bootstrap/relations.html
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1085 2023-06-14 06:35:43.000000 translate-toolkit-3.9.1/docs/_themes/sphinx-bootstrap/search.html
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      305 2023-06-14 06:35:43.000000 translate-toolkit-3.9.1/docs/_themes/sphinx-bootstrap/searchbox.html
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      420 2023-06-14 06:35:43.000000 translate-toolkit-3.9.1/docs/_themes/sphinx-bootstrap/sourcelink.html
+drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-06-14 06:36:34.945624 translate-toolkit-3.9.1/docs/_themes/sphinx-bootstrap/static/
+-rw-r--r--   0 nijel     (1000) nijel     (1000)    10518 2023-06-14 06:35:43.000000 translate-toolkit-3.9.1/docs/_themes/sphinx-bootstrap/static/bootstrap-responsive.css
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      374 2023-06-14 06:35:43.000000 translate-toolkit-3.9.1/docs/_themes/sphinx-bootstrap/static/bootstrap-sphinx.css_t
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1727 2023-06-14 06:35:43.000000 translate-toolkit-3.9.1/docs/_themes/sphinx-bootstrap/static/bootstrap-sphinx.js
+-rw-r--r--   0 nijel     (1000) nijel     (1000)    97055 2023-06-14 06:35:43.000000 translate-toolkit-3.9.1/docs/_themes/sphinx-bootstrap/static/bootstrap.css
+-rw-r--r--   0 nijel     (1000) nijel     (1000)    22323 2023-06-14 06:35:43.000000 translate-toolkit-3.9.1/docs/_themes/sphinx-bootstrap/static/bootstrap.js
+drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-06-14 06:36:34.945624 translate-toolkit-3.9.1/docs/_themes/sphinx-bootstrap/static/font/
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)    38708 2023-06-14 06:35:43.000000 translate-toolkit-3.9.1/docs/_themes/sphinx-bootstrap/static/font/fontawesome-webfont.eot
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)   130151 2023-06-14 06:35:43.000000 translate-toolkit-3.9.1/docs/_themes/sphinx-bootstrap/static/font/fontawesome-webfont.svg
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)    68476 2023-06-14 06:35:43.000000 translate-toolkit-3.9.1/docs/_themes/sphinx-bootstrap/static/font/fontawesome-webfont.ttf
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)    41752 2023-06-14 06:35:43.000000 translate-toolkit-3.9.1/docs/_themes/sphinx-bootstrap/static/font/fontawesome-webfont.woff
+-rw-r--r--   0 nijel     (1000) nijel     (1000)    93436 2023-06-14 06:35:43.000000 translate-toolkit-3.9.1/docs/_themes/sphinx-bootstrap/static/jquery.js
+drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-06-14 06:36:34.949624 translate-toolkit-3.9.1/docs/_themes/sphinx-bootstrap/static/less/
+-rw-r--r--   0 nijel     (1000) nijel     (1000)    14766 2023-06-14 06:35:43.000000 translate-toolkit-3.9.1/docs/_themes/sphinx-bootstrap/static/less/font-awesome.less
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     4514 2023-06-14 06:35:43.000000 translate-toolkit-3.9.1/docs/_themes/sphinx-bootstrap/static/less/theme.less
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     8431 2023-06-14 06:35:43.000000 translate-toolkit-3.9.1/docs/_themes/sphinx-bootstrap/static/less/variables.less
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      114 2023-06-14 06:35:43.000000 translate-toolkit-3.9.1/docs/_themes/sphinx-bootstrap/theme.conf
+drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-06-14 06:36:34.949624 translate-toolkit-3.9.1/docs/api/
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     5427 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/docs/api/convert.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      786 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/docs/api/filters.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      912 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/docs/api/index.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     3317 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/docs/api/lang.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      964 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/docs/api/misc.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      364 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/docs/api/search.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      177 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/docs/api/services.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     6573 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/docs/api/storage.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1680 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/docs/api/tools.rst
+drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-06-14 06:36:34.953624 translate-toolkit-3.9.1/docs/commands/
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     5177 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/docs/commands/csv2po.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     3362 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/docs/commands/csv2tbx.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     5091 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/docs/commands/flatxml2po.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     2063 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/docs/commands/general_usage.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     5138 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/docs/commands/html2po.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     4287 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/docs/commands/ical2po.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     6234 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/docs/commands/index.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     5482 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/docs/commands/ini2po.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     4106 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/docs/commands/json2po.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      356 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/docs/commands/junitmsgfmt.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     2631 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/docs/commands/levenshtein_distance.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     4456 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/docs/commands/moz-l10n-builder.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     7496 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/docs/commands/moz2po.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     9695 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/docs/commands/mozilla_l10n_scripts.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     3699 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/docs/commands/odf2xliff.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     7685 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/docs/commands/oo2po.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1157 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/docs/commands/option_accelerator.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     2411 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/docs/commands/option_duplicates.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1704 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/docs/commands/option_errorlevel.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      599 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/docs/commands/option_filteraction.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      613 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/docs/commands/option_multifile.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1562 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/docs/commands/option_personality.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     2719 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/docs/commands/option_progress.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     4073 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/docs/commands/option_rewrite.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     4377 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/docs/commands/phase.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     4172 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/docs/commands/php2po.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     3396 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/docs/commands/po2tmx.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1659 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/docs/commands/po2wordfast.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1804 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/docs/commands/poclean.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      968 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/docs/commands/pocommentclean.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     3485 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/docs/commands/pocompendium.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1847 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/docs/commands/pocompile.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     3790 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/docs/commands/poconflicts.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     5658 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/docs/commands/pocount.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     7176 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/docs/commands/podebug.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     4972 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/docs/commands/pofilter.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)    25812 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/docs/commands/pofilter_tests.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     3789 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/docs/commands/pogrep.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     4091 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/docs/commands/pomerge.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     2544 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/docs/commands/pomigrate2.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1746 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/docs/commands/popuretext.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1367 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/docs/commands/poreencode.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     2046 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/docs/commands/porestructure.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     3586 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/docs/commands/posegment.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      848 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/docs/commands/posplit.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     3354 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/docs/commands/poswap.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     4111 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/docs/commands/pot2po.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)    16451 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/docs/commands/poterminology.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     8052 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/docs/commands/poterminology_stopword_file.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     3214 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/docs/commands/pretranslate.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     7629 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/docs/commands/prop2po.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     4925 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/docs/commands/rc2po.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     4019 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/docs/commands/resx2po.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     3908 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/docs/commands/sub2po.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     5754 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/docs/commands/symb2po.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1638 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/docs/commands/tbx2po.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     2375 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/docs/commands/tiki2po.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     2544 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/docs/commands/tmserver.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     3864 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/docs/commands/ts2po.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     7056 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/docs/commands/txt2po.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     3727 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/docs/commands/web2py2po.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     3213 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/docs/commands/xliff2po.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     4357 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/docs/commands/yaml2po.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     6572 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/docs/conf.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1028 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/docs/contents.rst.inc
+drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-06-14 06:36:34.957624 translate-toolkit-3.9.1/docs/developers/
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1299 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/docs/developers/building.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     3679 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/docs/developers/contributing.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     2146 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/docs/developers/deprecation.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     9692 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/docs/developers/developers.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)    11047 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/docs/developers/releasing.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     3174 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/docs/developers/reporting_bugs.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)    19038 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/docs/developers/styleguide.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     9434 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/docs/developers/testing.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     2499 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/docs/features.rst
+drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-06-14 06:36:34.957624 translate-toolkit-3.9.1/docs/formats/
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      736 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/docs/formats/android.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     7698 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/docs/formats/base_classes.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     2041 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/docs/formats/catkeys.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      707 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/docs/formats/conformance.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1973 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/docs/formats/csv.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1006 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/docs/formats/dtd.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     3043 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/docs/formats/flatxml.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      451 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/docs/formats/flex.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      493 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/docs/formats/gsi.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1160 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/docs/formats/html.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     2090 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/docs/formats/ical.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     7893 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/docs/formats/index.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      769 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/docs/formats/ini.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      923 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/docs/formats/json.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      998 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/docs/formats/mo.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      452 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/docs/formats/mozilla_lang.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1549 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/docs/formats/odf.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      962 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/docs/formats/omegat_glossary.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     7761 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/docs/formats/php.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1210 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/docs/formats/po.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1579 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/docs/formats/properties.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      888 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/docs/formats/qm.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1233 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/docs/formats/qt_phrase_book.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     2078 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/docs/formats/quoting_and_escaping.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1281 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/docs/formats/rc.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1412 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/docs/formats/resx.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      979 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/docs/formats/strings.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1360 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/docs/formats/subtitles.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     2026 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/docs/formats/tbx.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      800 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/docs/formats/text.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      810 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/docs/formats/tmx.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1964 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/docs/formats/ts.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1216 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/docs/formats/utx.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1821 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/docs/formats/wiki.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      316 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/docs/formats/wml.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      777 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/docs/formats/wordfast.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     2160 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/docs/formats/xliff.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      495 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/docs/formats/yaml.rst
+drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-06-14 06:36:34.961624 translate-toolkit-3.9.1/docs/guides/
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     6603 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/docs/guides/checking_for_inconsistencies.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1736 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/docs/guides/cleanup_translator_comments.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     7490 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/docs/guides/creating_a_terminology_list_from_your_existing_translations.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     2161 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/docs/guides/creating_mozilla_pot_files.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1960 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/docs/guides/document_translation.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1297 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/docs/guides/index.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     6258 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/docs/guides/migrating_translations.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1524 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/docs/guides/running_the_tools_on_microsoft_windows.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     7596 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/docs/guides/using_csv2po.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     2230 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/docs/guides/using_oo2po.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     7736 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/docs/guides/using_pofilter.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     4864 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/docs/history.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      237 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/docs/index.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     5263 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/docs/installation.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      233 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/docs/license.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     5116 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/docs/make.bat
+drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-06-14 06:36:34.969624 translate-toolkit-3.9.1/docs/releases/
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      225 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/docs/releases/0.10.1.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     2200 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/docs/releases/0.10.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1170 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/docs/releases/0.11.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      220 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/docs/releases/0.7.1.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      219 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/docs/releases/0.8.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      219 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/docs/releases/0.9.1.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      221 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/docs/releases/0.9.2.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     4422 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/docs/releases/0.9.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      655 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/docs/releases/1.0.1.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     6959 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/docs/releases/1.0.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     4071 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/docs/releases/1.1.0.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      680 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/docs/releases/1.1.1.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     4368 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/docs/releases/1.10.0.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     4975 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/docs/releases/1.11.0.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     5431 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/docs/releases/1.12.0.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     4151 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/docs/releases/1.13.0.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     2206 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/docs/releases/1.2.0.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      223 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/docs/releases/1.2.1.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      273 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/docs/releases/1.3.0.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      713 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/docs/releases/1.4.0.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      961 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/docs/releases/1.4.1.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      223 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/docs/releases/1.5.0.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      222 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/docs/releases/1.5.1.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      222 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/docs/releases/1.5.2.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      222 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/docs/releases/1.5.3.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      589 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/docs/releases/1.6.0.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      218 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/docs/releases/1.7.0.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      221 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/docs/releases/1.8.0.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     3162 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/docs/releases/1.8.1.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     2325 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/docs/releases/1.9.0.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     8012 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/docs/releases/2.0.0.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     2153 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/docs/releases/2.1.0.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1621 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/docs/releases/2.2.0.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1310 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/docs/releases/2.2.1.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      376 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/docs/releases/2.2.2.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      384 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/docs/releases/2.2.3.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1018 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/docs/releases/2.2.4.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      557 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/docs/releases/2.2.5.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1683 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/docs/releases/2.3.0.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     2341 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/docs/releases/2.3.1.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     2357 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/docs/releases/2.4.0.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1465 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/docs/releases/2.5.0.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1416 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/docs/releases/2.5.1.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1563 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/docs/releases/3.0.0.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1211 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/docs/releases/3.1.0.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      378 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/docs/releases/3.1.1.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      639 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/docs/releases/3.2.0.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1490 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/docs/releases/3.3.0.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      503 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/docs/releases/3.3.1.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      604 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/docs/releases/3.3.2.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      692 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/docs/releases/3.3.3.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      438 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/docs/releases/3.3.4.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      490 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/docs/releases/3.3.5.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      452 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/docs/releases/3.3.6.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      563 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/docs/releases/3.4.0.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      573 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/docs/releases/3.4.1.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      481 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/docs/releases/3.5.0.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      367 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/docs/releases/3.5.1.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      482 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/docs/releases/3.5.2.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      394 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/docs/releases/3.5.3.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      765 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/docs/releases/3.6.0.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      533 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/docs/releases/3.6.1.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      508 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/docs/releases/3.6.2.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      869 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/docs/releases/3.7.0.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      477 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/docs/releases/3.7.1.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      387 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/docs/releases/3.7.2.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      602 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/docs/releases/3.7.3.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      536 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/docs/releases/3.7.4.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      701 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/docs/releases/3.8.0.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      529 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/docs/releases/3.8.1.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      348 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/docs/releases/3.8.2.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      398 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/docs/releases/3.8.3.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      403 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/docs/releases/3.8.4.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      347 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/docs/releases/3.8.5.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      447 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/docs/releases/3.8.6.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      776 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/docs/releases/3.9.0.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      536 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/docs/releases/3.9.1.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1246 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/docs/releases/README.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1700 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/docs/releases/index.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      306 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/pyproject.toml
+-rw-r--r--   0 nijel     (1000) nijel     (1000)       41 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/pytest.ini
+drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-06-14 06:36:34.969624 translate-toolkit-3.9.1/requirements/
+-rw-r--r--   0 nijel     (1000) nijel     (1000)       47 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/requirements/dev.txt
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      114 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/requirements/dist.txt
+-rw-r--r--   0 nijel     (1000) nijel     (1000)       18 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/requirements/lint.txt
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      736 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/requirements/optional.txt
+-rw-r--r--   0 nijel     (1000) nijel     (1000)       71 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/requirements/required.txt
+-rw-r--r--   0 nijel     (1000) nijel     (1000)       82 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/requirements/test.txt
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     5912 2023-06-14 06:36:35.089624 translate-toolkit-3.9.1/setup.cfg
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)     2385 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/setup.py
+drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-06-14 06:36:34.937624 translate-toolkit-3.9.1/tests/
+drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-06-14 06:36:34.973624 translate-toolkit-3.9.1/tests/cli/
+drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-06-14 06:36:34.937624 translate-toolkit-3.9.1/tests/cli/data/
+drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-06-14 06:36:34.973624 translate-toolkit-3.9.1/tests/cli/data/test_flatxml2po/
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      460 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/tests/cli/data/test_flatxml2po/one.xml
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      813 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/tests/cli/data/test_flatxml2po/out.po
+drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-06-14 06:36:34.977624 translate-toolkit-3.9.1/tests/cli/data/test_flatxml2po_wrongkey/
+-rw-r--r--   0 nijel     (1000) nijel     (1000)       57 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/tests/cli/data/test_flatxml2po_wrongkey/one.xml
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      212 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/tests/cli/data/test_flatxml2po_wrongkey/stderr.txt
+drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-06-14 06:36:34.977624 translate-toolkit-3.9.1/tests/cli/data/test_flatxml2po_wrongns/
+-rw-r--r--   0 nijel     (1000) nijel     (1000)       57 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/tests/cli/data/test_flatxml2po_wrongns/one.xml
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      200 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/tests/cli/data/test_flatxml2po_wrongns/stderr.txt
+drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-06-14 06:36:34.977624 translate-toolkit-3.9.1/tests/cli/data/test_flatxml2po_wrongroot/
+-rw-r--r--   0 nijel     (1000) nijel     (1000)       57 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/tests/cli/data/test_flatxml2po_wrongroot/one.xml
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      198 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/tests/cli/data/test_flatxml2po_wrongroot/stderr.txt
+drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-06-14 06:36:34.977624 translate-toolkit-3.9.1/tests/cli/data/test_flatxml2po_wrongvalue/
+-rw-r--r--   0 nijel     (1000) nijel     (1000)       57 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/tests/cli/data/test_flatxml2po_wrongvalue/one.xml
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      210 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/tests/cli/data/test_flatxml2po_wrongvalue/stderr.txt
+drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-06-14 06:36:34.977624 translate-toolkit-3.9.1/tests/cli/data/test_junitmsgfmt_failure/
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      238 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/tests/cli/data/test_junitmsgfmt_failure/one.po
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      846 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/tests/cli/data/test_junitmsgfmt_failure/stdout.txt
+drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-06-14 06:36:34.977624 translate-toolkit-3.9.1/tests/cli/data/test_junitmsgfmt_untranslated/
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      207 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/tests/cli/data/test_junitmsgfmt_untranslated/one.po
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      808 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/tests/cli/data/test_junitmsgfmt_untranslated/stdout.txt
+drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-06-14 06:36:34.977624 translate-toolkit-3.9.1/tests/cli/data/test_po2csv/
+-rw-r--r--   0 nijel     (1000) nijel     (1000)       85 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/tests/cli/data/test_po2csv/one.po
+-rw-r--r--   0 nijel     (1000) nijel     (1000)       88 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/tests/cli/data/test_po2csv/out.txt
+drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-06-14 06:36:34.977624 translate-toolkit-3.9.1/tests/cli/data/test_po2flatxml/
+-rw-r--r--   0 nijel     (1000) nijel     (1000)       61 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/tests/cli/data/test_po2flatxml/one.po
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      118 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/tests/cli/data/test_po2flatxml/out.xml
+drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-06-14 06:36:34.977624 translate-toolkit-3.9.1/tests/cli/data/test_po2flatxml_params/
+-rw-r--r--   0 nijel     (1000) nijel     (1000)       82 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/tests/cli/data/test_po2flatxml_params/one.po
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      318 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/tests/cli/data/test_po2flatxml_params/out.xml
+drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-06-14 06:36:34.977624 translate-toolkit-3.9.1/tests/cli/data/test_po2flatxml_preserve/
+-rw-r--r--   0 nijel     (1000) nijel     (1000)       89 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/tests/cli/data/test_po2flatxml_preserve/one.po
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      292 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/tests/cli/data/test_po2flatxml_preserve/out.xml
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      264 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/tests/cli/data/test_po2flatxml_preserve/two.xml
+drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-06-14 06:36:34.981624 translate-toolkit-3.9.1/tests/cli/data/test_po2flatxml_template/
+-rw-r--r--   0 nijel     (1000) nijel     (1000)       82 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/tests/cli/data/test_po2flatxml_template/one.po
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      270 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/tests/cli/data/test_po2flatxml_template/out.xml
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      115 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/tests/cli/data/test_po2flatxml_template/two.xml
+drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-06-14 06:36:34.981624 translate-toolkit-3.9.1/tests/cli/data/test_po2html/
+-rw-r--r--   0 nijel     (1000) nijel     (1000)       85 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/tests/cli/data/test_po2html/one.po
+-rw-r--r--   0 nijel     (1000) nijel     (1000)       79 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/tests/cli/data/test_po2html/out.txt
+-rw-r--r--   0 nijel     (1000) nijel     (1000)       78 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/tests/cli/data/test_po2html/template.html
+drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-06-14 06:36:34.981624 translate-toolkit-3.9.1/tests/cli/data/test_po2json_files_removeuntranslated/
+-rw-r--r--   0 nijel     (1000) nijel     (1000)       42 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/tests/cli/data/test_po2json_files_removeuntranslated/out.json
+-rw-r--r--   0 nijel     (1000) nijel     (1000)       83 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/tests/cli/data/test_po2json_files_removeuntranslated/template.json
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      161 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/tests/cli/data/test_po2json_files_removeuntranslated/translations.po
+drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-06-14 06:36:34.981624 translate-toolkit-3.9.1/tests/cli/data/test_po2prop_mozilla_files/
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      145 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/tests/cli/data/test_po2prop_mozilla_files/out.properties
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      141 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/tests/cli/data/test_po2prop_mozilla_files/template.properties
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      198 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/tests/cli/data/test_po2prop_mozilla_files/translations.po
+drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-06-14 06:36:34.981624 translate-toolkit-3.9.1/tests/cli/data/test_po2ts/
+-rw-r--r--   0 nijel     (1000) nijel     (1000)       85 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/tests/cli/data/test_po2ts/one.po
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      362 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/tests/cli/data/test_po2ts/out.txt
+drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-06-14 06:36:34.981624 translate-toolkit-3.9.1/tests/cli/data/test_po2txt/
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      151 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/tests/cli/data/test_po2txt/one.po
+-rw-r--r--   0 nijel     (1000) nijel     (1000)       32 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/tests/cli/data/test_po2txt/out.txt
+drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-06-14 06:36:34.981624 translate-toolkit-3.9.1/tests/cli/data/test_po2txt_threshold/
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      151 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/tests/cli/data/test_po2txt_threshold/one.po
+-rw-r--r--   0 nijel     (1000) nijel     (1000)        0 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/tests/cli/data/test_po2txt_threshold/out.txt
+drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-06-14 06:36:34.981624 translate-toolkit-3.9.1/tests/cli/data/test_pocount_po_csv/
+-rw-r--r--   0 nijel     (1000) nijel     (1000)       43 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/tests/cli/data/test_pocount_po_csv/one.po
+drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-06-14 06:36:34.981624 translate-toolkit-3.9.1/tests/cli/data/test_pocount_po_file/
+-rw-r--r--   0 nijel     (1000) nijel     (1000)       43 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/tests/cli/data/test_pocount_po_file/one.po
+drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-06-14 06:36:34.981624 translate-toolkit-3.9.1/tests/cli/data/test_pocount_po_fuzzy/
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      121 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/tests/cli/data/test_pocount_po_fuzzy/one.po
+drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-06-14 06:36:34.981624 translate-toolkit-3.9.1/tests/cli/data/test_pocount_po_plurals/
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      101 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/tests/cli/data/test_pocount_po_plurals/plural.po
+drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-06-14 06:36:34.981624 translate-toolkit-3.9.1/tests/cli/data/test_pocount_xliff_states_no/
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1505 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/tests/cli/data/test_pocount_xliff_states_no/states.xlf
+drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-06-14 06:36:34.981624 translate-toolkit-3.9.1/tests/cli/data/test_pocount_xliff_states_yes/
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1513 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/tests/cli/data/test_pocount_xliff_states_yes/states.xlf
+drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-06-14 06:36:34.981624 translate-toolkit-3.9.1/tests/cli/data/test_pofilter_listfilters/
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     3337 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/tests/cli/data/test_pofilter_listfilters/stdout.txt
+drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-06-14 06:36:34.981624 translate-toolkit-3.9.1/tests/cli/data/test_pofilter_manpage/
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     3421 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/tests/cli/data/test_pofilter_manpage/stdout.txt
+drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-06-14 06:36:34.981624 translate-toolkit-3.9.1/tests/cli/data/test_posegment/
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      370 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/tests/cli/data/test_posegment/one.po
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      388 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/tests/cli/data/test_posegment/out.po
+drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-06-14 06:36:34.985624 translate-toolkit-3.9.1/tests/cli/data/test_poswap_comments/
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      133 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/tests/cli/data/test_poswap_comments/af.po
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      130 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/tests/cli/data/test_poswap_comments/fr.po
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      133 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/tests/cli/data/test_poswap_comments/out.po
+drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-06-14 06:36:34.985624 translate-toolkit-3.9.1/tests/cli/data/test_poswap_fr_af/
+-rw-r--r--   0 nijel     (1000) nijel     (1000)       86 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/tests/cli/data/test_poswap_fr_af/af.po
+-rw-r--r--   0 nijel     (1000) nijel     (1000)       81 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/tests/cli/data/test_poswap_fr_af/fr.po
+-rw-r--r--   0 nijel     (1000) nijel     (1000)       86 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/tests/cli/data/test_poswap_fr_af/out.po
+drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-06-14 06:36:34.985624 translate-toolkit-3.9.1/tests/cli/data/test_poswap_fr_af_reverse/
+-rw-r--r--   0 nijel     (1000) nijel     (1000)       81 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/tests/cli/data/test_poswap_fr_af_reverse/fr.po
+-rw-r--r--   0 nijel     (1000) nijel     (1000)       81 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/tests/cli/data/test_poswap_fr_af_reverse/fr_af.po
+-rw-r--r--   0 nijel     (1000) nijel     (1000)       81 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/tests/cli/data/test_poswap_fr_af_reverse/out.po
+drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-06-14 06:36:34.985624 translate-toolkit-3.9.1/tests/cli/data/test_poswap_missing_units/
+-rw-r--r--   0 nijel     (1000) nijel     (1000)       52 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/tests/cli/data/test_poswap_missing_units/af.po
+-rw-r--r--   0 nijel     (1000) nijel     (1000)       54 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/tests/cli/data/test_poswap_missing_units/fr.po
+-rw-r--r--   0 nijel     (1000) nijel     (1000)       49 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/tests/cli/data/test_poswap_missing_units/out.po
+drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-06-14 06:36:34.985624 translate-toolkit-3.9.1/tests/cli/data/test_prop2po/
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      322 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/tests/cli/data/test_prop2po/stderr.txt
+drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-06-14 06:36:34.985624 translate-toolkit-3.9.1/tests/cli/data/test_prop2po_dirs/
+drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-06-14 06:36:34.985624 translate-toolkit-3.9.1/tests/cli/data/test_prop2po_dirs/one/
+-rw-r--r--   0 nijel     (1000) nijel     (1000)       10 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/tests/cli/data/test_prop2po_dirs/one/a.properties
+drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-06-14 06:36:34.985624 translate-toolkit-3.9.1/tests/cli/data/test_prop2po_dirs/out/
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      498 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/tests/cli/data/test_prop2po_dirs/out/a.po
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      144 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/tests/cli/data/test_prop2po_dirs/stderr.txt
+drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-06-14 06:36:34.985624 translate-toolkit-3.9.1/tests/cli/data/test_prop2po_files/
+-rw-r--r--   0 nijel     (1000) nijel     (1000)       10 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/tests/cli/data/test_prop2po_files/one.properties
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      506 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/tests/cli/data/test_prop2po_files/out.po
+drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-06-14 06:36:34.989624 translate-toolkit-3.9.1/tests/cli/data/test_prop2po_files_templates/
+-rw-r--r--   0 nijel     (1000) nijel     (1000)       10 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/tests/cli/data/test_prop2po_files_templates/one.properties
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      574 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/tests/cli/data/test_prop2po_files_templates/out.po
+-rw-r--r--   0 nijel     (1000) nijel     (1000)       11 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/tests/cli/data/test_prop2po_files_templates/two.properties
+drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-06-14 06:36:34.989624 translate-toolkit-3.9.1/tests/cli/data/test_rc2po/
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     3564 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/tests/cli/data/test_rc2po/one.rc
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1882 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/tests/cli/data/test_rc2po/out.po
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      727 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/tests/cli/example_test.sh
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)      226 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/tests/cli/run_tests.sh
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     4775 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/tests/cli/test.inc.sh
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)      127 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/tests/cli/test_flatxml2po.sh
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)      141 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/tests/cli/test_flatxml2po_wrongkey.sh
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)      147 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/tests/cli/test_flatxml2po_wrongns.sh
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)      142 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/tests/cli/test_flatxml2po_wrongroot.sh
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)      143 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/tests/cli/test_flatxml2po_wrongvalue.sh
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)      107 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/tests/cli/test_junitmsgfmt_failure.sh
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)      122 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/tests/cli/test_junitmsgfmt_untranslated.sh
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)      123 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/tests/cli/test_po2csv.sh
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)      127 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/tests/cli/test_po2flatxml.sh
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)      252 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/tests/cli/test_po2flatxml_params.sh
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)      141 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/tests/cli/test_po2flatxml_preserve.sh
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)      266 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/tests/cli/test_po2flatxml_template.sh
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)      137 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/tests/cli/test_po2html.sh
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)      167 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/tests/cli/test_po2json_files_removeuntranslated.sh
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)      168 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/tests/cli/test_po2prop_mozilla_files.sh
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)      122 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/tests/cli/test_po2ts.sh
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)      123 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/tests/cli/test_po2txt.sh
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)      194 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/tests/cli/test_po2txt_threshold.sh
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)      113 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/tests/cli/test_pofilter_listfilters.sh
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)      182 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/tests/cli/test_pofilter_manpage.sh
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)      126 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/tests/cli/test_posegment.sh
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)      147 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/tests/cli/test_poswap_comments.sh
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)      147 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/tests/cli/test_poswap_fr_af.sh
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)      160 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/tests/cli/test_poswap_fr_af_reverse.sh
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)      147 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/tests/cli/test_poswap_missing_units.sh
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)       98 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/tests/cli/test_prop2po.sh
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)      108 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/tests/cli/test_prop2po_dirs.sh
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)      124 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/tests/cli/test_prop2po_files.sh
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)      132 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/tests/cli/test_prop2po_files_templates.sh
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)      128 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/tests/cli/test_rc2po.sh
+drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-06-14 06:36:34.989624 translate-toolkit-3.9.1/tests/odf_xliff/
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     3085 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/tests/odf_xliff/test_2-test_odf2xliff-reference.xlf
+-rw-r--r--   0 nijel     (1000) nijel     (1000)   133081 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/tests/odf_xliff/test_2.odt
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1864 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/tests/odf_xliff/test_inline-test_odf2xliff_inline-reference.xlf
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     7300 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/tests/odf_xliff/test_inline.odt
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     5466 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/tests/odf_xliff/test_odf_xliff.py
+drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-06-14 06:36:34.989624 translate-toolkit-3.9.1/tests/xliff_conformance/
+-rw-r--r--   0 nijel     (1000) nijel     (1000)    36103 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/tests/xliff_conformance/af-pootle.po
+-rw-r--r--   0 nijel     (1000) nijel     (1000)    30075 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/tests/xliff_conformance/en-US.sdf
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     2257 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/tests/xliff_conformance/test_xliff_conformance.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)    96911 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/tests/xliff_conformance/xliff-core-1.1.xsd
+drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-06-14 06:36:34.993624 translate-toolkit-3.9.1/tools/
+drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-06-14 06:36:34.997624 translate-toolkit-3.9.1/tools/mozilla/
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     7012 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/tools/mozilla/README.firefox_build_instructions.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     4102 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/tools/mozilla/Vagrantfile
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)     3429 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/tools/mozilla/accesskey_checker
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)     2546 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/tools/mozilla/accesskey_checker_PO
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)    12855 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/tools/mozilla/build_firefox.sh
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)     7178 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/tools/mozilla/build_tb3_langs.sh
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)     9665 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/tools/mozilla/buildxpi.py
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)      158 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/tools/mozilla/compare-locales.sh
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)     4495 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/tools/mozilla/get_moz_enUS.py
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)    11342 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/tools/mozilla/moz-l10n-builder
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)    23575 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/tools/mozilla/moz_l10n_builder.py
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)     2257 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/tools/mozilla/mozcronbuild.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1487 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/tools/mozilla/mozilla-l10n.patch
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)    12089 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/tools/mozilla/mozzy.sh
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)     3208 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/tools/mozilla/postinstall.sh
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)      497 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/tools/mozilla/setup_mozilla.sh
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)    18996 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/tools/phase
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)      626 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/tools/phaselist2goals
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)     1041 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/tools/pocommentclean
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)     4683 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/tools/pocompendium
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)     5288 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/tools/pomigrate2
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)     1852 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/tools/popuretext
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)     1121 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/tools/poreencode
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)     1526 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/tools/posplit
+drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-06-14 06:36:34.997624 translate-toolkit-3.9.1/translate/
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1816 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/__init__.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1406 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/__version__.py
+drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-06-14 06:36:35.021624 translate-toolkit-3.9.1/translate/convert/
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      790 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/convert/__init__.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     8225 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/convert/accesskey.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)    20603 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/convert/convert.py
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)    10219 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/convert/csv2po.py
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)     3325 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/convert/csv2tbx.py
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)    13191 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/convert/dtd2po.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     7541 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/convert/factory.py
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)     3663 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/convert/flatxml2po.py
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)     5523 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/convert/html2po.py
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)     4527 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/convert/ical2po.py
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)     1902 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/convert/idml2po.py
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)     5078 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/convert/ini2po.py
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)     5180 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/convert/json2po.py
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)     2358 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/convert/moz2po.py
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)     4922 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/convert/mozfunny2prop.py
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)     3981 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/convert/mozlang2po.py
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)     3839 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/convert/odf2xliff.py
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)      357 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/convert/odfxml
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)     7936 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/convert/oo2po.py
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)     7286 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/convert/oo2xliff.py
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)     4536 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/convert/php2po.py
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)     4005 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/convert/po2csv.py
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)     8688 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/convert/po2dtd.py
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)     5083 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/convert/po2flatxml.py
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)     6792 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/convert/po2html.py
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)     3617 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/convert/po2ical.py
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)     6806 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/convert/po2idml.py
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)     4107 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/convert/po2ini.py
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)     3682 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/convert/po2json.py
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)     3490 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/convert/po2moz.py
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)     3702 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/convert/po2mozlang.py
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)    11233 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/convert/po2oo.py
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)     3374 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/convert/po2php.py
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)    12940 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/convert/po2prop.py
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)    13967 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/convert/po2rc.py
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)     3195 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/convert/po2resx.py
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)     2821 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/convert/po2sub.py
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)     4085 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/convert/po2symb.py
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)     3227 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/convert/po2tiki.py
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)     5569 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/convert/po2tmx.py
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)     3228 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/convert/po2ts.py
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)     5171 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/convert/po2txt.py
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)     2559 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/convert/po2web2py.py
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)     4185 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/convert/po2wordfast.py
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)     4287 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/convert/po2xliff.py
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)     3949 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/convert/po2yaml.py
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)    12222 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/convert/pot2po.py
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)     6230 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/convert/prop2mozfunny.py
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)    18818 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/convert/prop2po.py
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)     5941 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/convert/rc2po.py
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)     6038 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/convert/resx2po.py
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)     1730 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/convert/roundtrip-OOo
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)     1629 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/convert/roundtrip-gaia
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)     1589 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/convert/roundtrip-mozilla
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)     4776 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/convert/sub2po.py
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)     4101 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/convert/symb2po.py
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)     2352 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/convert/tbx2po.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)   189411 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/convert/test.idml
+-rw-r--r--   0 nijel     (1000) nijel     (1000)    11608 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/convert/test.odt
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     4655 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/convert/test_accesskey.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     5372 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/convert/test_convert.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     6225 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/convert/test_csv2po.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)    19205 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/convert/test_dtd2po.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     4744 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/convert/test_flatxml2po.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)    27945 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/convert/test_html2po.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)    12076 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/convert/test_ical2po.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      449 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/convert/test_idml2po.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     4543 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/convert/test_ini2po.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     2472 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/convert/test_json2po.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      414 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/convert/test_moz2po.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     2179 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/convert/test_mozfunny2prop.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     4733 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/convert/test_mozlang2po.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      446 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/convert/test_ods2xliff.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)    13063 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/convert/test_oo2po.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     2989 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/convert/test_oo2xliff.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)    11579 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/convert/test_php2po.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     6405 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/convert/test_po2csv.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)    22148 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/convert/test_po2dtd.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     4617 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/convert/test_po2flatxml.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)    11889 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/convert/test_po2html.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)    10814 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/convert/test_po2ical.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      826 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/convert/test_po2idml.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     8117 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/convert/test_po2ini.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     3853 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/convert/test_po2json.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      494 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/convert/test_po2moz.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     5024 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/convert/test_po2mozlang.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     9663 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/convert/test_po2oo.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)    10874 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/convert/test_po2php.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)    17564 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/convert/test_po2prop.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)    11622 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/convert/test_po2rc.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)    18992 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/convert/test_po2resx.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     2151 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/convert/test_po2sub.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     2097 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/convert/test_po2tiki.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     6522 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/convert/test_po2tmx.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     4373 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/convert/test_po2ts.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     5238 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/convert/test_po2txt.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1967 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/convert/test_po2web2py.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)    10413 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/convert/test_po2xliff.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     6837 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/convert/test_po2yaml.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)    27471 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/convert/test_pot2po.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     2201 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/convert/test_prop2mozfunny.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)    14486 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/convert/test_prop2po.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     4827 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/convert/test_rc2po.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)    10049 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/convert/test_resx2po.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     2362 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/convert/test_tiki2po.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     4628 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/convert/test_ts2po.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     8333 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/convert/test_txt2po.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1823 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/convert/test_web2py2po.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      942 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/convert/test_xliff2odf.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)    12996 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/convert/test_xliff2po.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     5143 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/convert/test_yaml2po.py
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)     3144 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/convert/tiki2po.py
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)     3774 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/convert/ts2po.py
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)     4682 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/convert/txt2po.py
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)     2757 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/convert/web2py2po.py
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)     5947 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/convert/xliff2odf.py
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)    11230 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/convert/xliff2oo.py
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)     4049 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/convert/xliff2po.py
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)     4458 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/convert/yaml2po.py
+drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-06-14 06:36:35.025624 translate-toolkit-3.9.1/translate/filters/
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      766 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/filters/__init__.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     2440 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/filters/autocorrect.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)   101819 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/filters/checks.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)    10481 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/filters/decoration.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1940 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/filters/decorators.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     2796 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/filters/helpers.py
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)    13302 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/filters/pofilter.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     6133 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/filters/prefilters.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     2153 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/filters/spelling.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     2531 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/filters/test_autocorrect.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)   108937 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/filters/test_checks.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     4060 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/filters/test_decoration.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)    13635 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/filters/test_pofilter.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1065 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/filters/test_prefilters.py
+drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-06-14 06:36:35.041624 translate-toolkit-3.9.1/translate/lang/
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      969 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/lang/__init__.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     3868 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/lang/af.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      925 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/lang/ak.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1513 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/lang/am.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     2090 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/lang/ar.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      974 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/lang/az.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     2096 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/lang/bn.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      973 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/lang/bo.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1458 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/lang/code_as.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1551 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/lang/code_or.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)    13174 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/lang/common.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1081 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/lang/da.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)    27413 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/lang/data.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      976 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/lang/de.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      976 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/lang/dz.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1949 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/lang/el.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1782 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/lang/es.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     3632 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/lang/fa.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     2488 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/lang/factory.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      985 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/lang/fi.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     2849 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/lang/fr.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      969 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/lang/gd.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      983 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/lang/gu.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      983 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/lang/he.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      974 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/lang/hi.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1821 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/lang/hy.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     4934 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/lang/identify.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1699 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/lang/ja.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1977 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/lang/km.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      980 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/lang/kn.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      971 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/lang/ko.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      973 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/lang/kw.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      967 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/lang/lo.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      986 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/lang/ml.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      980 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/lang/mr.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      967 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/lang/ms.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1042 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/lang/my.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1637 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/lang/ne.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     4893 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/lang/ngram.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1413 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/lang/nqo.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      952 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/lang/nso.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1614 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/lang/pa.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1079 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/lang/pl.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     5968 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/lang/poedit.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1100 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/lang/pt_BR.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     2828 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/lang/ro.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     5382 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/lang/scn.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      992 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/lang/si.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      963 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/lang/son.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      940 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/lang/st.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      979 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/lang/su.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1080 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/lang/sv.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      978 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/lang/ta.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      971 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/lang/te.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)    21016 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/lang/team.py
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)      707 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/lang/test-language-teams.sh
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1690 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/lang/test_af.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1119 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/lang/test_am.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1388 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/lang/test_ar.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     5162 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/lang/test_common.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     4131 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/lang/test_data.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1417 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/lang/test_el.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1273 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/lang/test_es.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     2815 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/lang/test_fa.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1918 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/lang/test_factory.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     3107 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/lang/test_fr.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1448 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/lang/test_hy.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     6480 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/lang/test_identify.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1116 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/lang/test_ja.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1829 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/lang/test_km.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1094 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/lang/test_ko.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     2963 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/lang/test_ne.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1751 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/lang/test_nqo.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1639 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/lang/test_or.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      705 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/lang/test_poedit.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1737 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/lang/test_ro.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1869 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/lang/test_scn.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      775 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/lang/test_team.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      632 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/lang/test_th.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      405 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/lang/test_tr.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      328 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/lang/test_uk.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1426 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/lang/test_vi.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1008 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/lang/test_zh.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1181 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/lang/th.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1025 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/lang/tr.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1091 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/lang/ug.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1186 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/lang/ur.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      952 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/lang/ve.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1532 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/lang/vi.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1655 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/lang/wo.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     2367 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/lang/zh.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1016 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/lang/zh_cn.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1029 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/lang/zh_hk.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1029 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/lang/zh_tw.py
+drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-06-14 06:36:35.045624 translate-toolkit-3.9.1/translate/misc/
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      838 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/misc/__init__.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1610 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/misc/deprecation.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     2733 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/misc/dictutils.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     2580 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/misc/file_discovery.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     3010 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/misc/multistring.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)    33419 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/misc/optrecurse.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)    10453 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/misc/ourdom.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     4655 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/misc/progressbar.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)    17756 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/misc/quote.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)    17681 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/misc/selector.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      465 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/misc/test_deprecation.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      234 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/misc/test_dictutils.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     3052 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/misc/test_multistring.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1133 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/misc/test_optrecurse.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      419 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/misc/test_progressbar.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     7634 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/misc/test_quote.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1209 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/misc/test_xml_helpers.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1424 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/misc/wStringIO.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1138 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/misc/wsgi.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     6869 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/misc/xml_helpers.py
+drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-06-14 06:36:35.045624 translate-toolkit-3.9.1/translate/search/
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      772 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/search/__init__.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     6056 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/search/lshtein.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)    15948 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/search/match.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1754 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/search/terminology.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1866 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/search/test_lshtein.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     5705 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/search/test_match.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      307 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/search/test_terminology.py
+drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-06-14 06:36:35.045624 translate-toolkit-3.9.1/translate/services/
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      833 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/services/__init__.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1855 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/services/test_tmserver.py
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)     8293 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/services/tmserver.py
+drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-06-14 06:36:35.045624 translate-toolkit-3.9.1/translate/share/
+drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-06-14 06:36:35.057624 translate-toolkit-3.9.1/translate/share/langmodels/
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1449 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/share/langmodels/Ndebele.lm
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1481 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/share/langmodels/NorthernSotho.lm
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1071 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/share/langmodels/README
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1463 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/share/langmodels/Sotho.lm
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1463 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/share/langmodels/Swati.lm
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1447 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/share/langmodels/Tsonga.lm
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1475 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/share/langmodels/Tswana.lm
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1457 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/share/langmodels/Venda.lm
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1421 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/share/langmodels/Xhosa.lm
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1464 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/share/langmodels/Zulu.lm
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     3387 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/share/langmodels/afrikaans.lm
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     3355 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/share/langmodels/albanian.lm
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     2325 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/share/langmodels/arabic.lm
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     3243 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/share/langmodels/basque.lm
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     2195 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/share/langmodels/belarus.lm
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     3131 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/share/langmodels/bosnian.lm
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     3287 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/share/langmodels/breton.lm
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     3223 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/share/langmodels/catalan.lm
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     2089 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/share/langmodels/chinese_simplified.lm
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1991 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/share/langmodels/chinese_traditional.lm
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     3428 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/share/langmodels/croatian.lm
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     3369 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/share/langmodels/czech.lm
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     3375 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/share/langmodels/danish.lm
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     3384 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/share/langmodels/dutch.lm
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     3317 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/share/langmodels/english.lm
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     3427 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/share/langmodels/esperanto.lm
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     3315 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/share/langmodels/estonian.lm
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     3425 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/share/langmodels/finnish.lm
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     3687 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/share/langmodels/fpdb.conf
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     3355 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/share/langmodels/french.lm
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     3443 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/share/langmodels/frisian.lm
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     3444 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/share/langmodels/german.lm
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     4266 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/share/langmodels/greek.lm
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     4187 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/share/langmodels/hebrew.lm
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     3353 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/share/langmodels/hungarian.lm
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     3475 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/share/langmodels/icelandic.lm
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     3359 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/share/langmodels/indonesian.lm
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     3178 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/share/langmodels/irish_gaelic.lm
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     3426 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/share/langmodels/italian.lm
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     2309 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/share/langmodels/japanese.lm
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     3324 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/share/langmodels/latin.lm
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     3500 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/share/langmodels/latvian.lm
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     3350 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/share/langmodels/lithuanian.lm
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     3597 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/share/langmodels/malay.lm
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     3462 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/share/langmodels/manx_gaelic.lm
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     3408 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/share/langmodels/norwegian.lm
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     3416 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/share/langmodels/polish.lm
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     3467 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/share/langmodels/portuguese.lm
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     3205 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/share/langmodels/quechua.lm
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     3297 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/share/langmodels/romanian.lm
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     3117 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/share/langmodels/romansh.lm
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     4146 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/share/langmodels/russian.lm
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     3131 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/share/langmodels/scots.lm
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     3323 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/share/langmodels/scots_gaelic.lm
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     3420 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/share/langmodels/serbian_ascii.lm
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     3239 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/share/langmodels/slovak_ascii.lm
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     3152 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/share/langmodels/slovenian.lm
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     3417 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/share/langmodels/spanish.lm
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     3314 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/share/langmodels/swahili.lm
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     3484 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/share/langmodels/swedish.lm
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     3261 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/share/langmodels/tagalog.lm
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     3539 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/share/langmodels/turkish.lm
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     2172 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/share/langmodels/ukrainian.lm
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     3689 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/share/langmodels/vietnamese.lm
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     3535 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/share/langmodels/welsh.lm
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     8740 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/share/stoplist-en
+drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-06-14 06:36:35.077624 translate-toolkit-3.9.1/translate/storage/
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      786 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/storage/__init__.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1324 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/storage/_factory_classes.py
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)    22457 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/storage/aresource.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)    34064 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/storage/base.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     7514 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/storage/benchmark.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)    10410 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/storage/bundleprojstore.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)    10970 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/storage/catkeys.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)    37641 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/storage/cpo.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)    11481 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/storage/csvl10n.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      338 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/storage/debug.properties
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     2383 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/storage/directory.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)    24352 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/storage/dtd.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     8762 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/storage/factory.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     8204 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/storage/flatxml.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)    24555 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/storage/fluent.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)    19719 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/storage/fpo.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)    17147 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/storage/html.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     4972 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/storage/ical.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     2846 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/storage/idml.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     4515 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/storage/ini.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)    25065 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/storage/jsonl10n.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)    13083 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/storage/lisa.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)    10982 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/storage/mo.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     5500 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/storage/mozilla_lang.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1165 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/storage/odf_io.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     5390 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/storage/odf_shared.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     6139 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/storage/omegat.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)    15688 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/storage/oo.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)    18547 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/storage/php.py
+drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-06-14 06:36:35.081624 translate-toolkit-3.9.1/translate/storage/placeables/
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     2004 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/storage/placeables/__init__.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     2962 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/storage/placeables/base.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)    13901 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/storage/placeables/general.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1241 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/storage/placeables/interfaces.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     7195 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/storage/placeables/lisa.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     3269 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/storage/placeables/parse.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)    35646 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/storage/placeables/strelem.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     3297 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/storage/placeables/terminology.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     8107 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/storage/placeables/test_base.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)    10622 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/storage/placeables/test_general.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     6121 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/storage/placeables/test_lisa.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     2029 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/storage/placeables/test_terminology.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     3991 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/storage/placeables/xliff.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1693 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/storage/po.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     7092 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/storage/pocommon.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)    16276 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/storage/poheader.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)    13215 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/storage/poparser.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)    12932 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/storage/poxliff.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     9143 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/storage/project.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)    14695 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/storage/projstore.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      753 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/storage/properties.java
+-rw-r--r--   0 nijel     (1000) nijel     (1000)    43632 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/storage/properties.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)    37283 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/storage/pypo.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     8559 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/storage/qm.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     5127 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/storage/qph.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)    16000 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/storage/rc.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1649 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/storage/resourcedictionary.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     8538 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/storage/resx.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     7567 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/storage/statistics.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     6662 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/storage/stringsdict.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     7652 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/storage/subtitles.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     2234 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/storage/symbian.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     4531 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/storage/tbx.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)    30744 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/storage/test_aresource.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)    14765 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/storage/test_base.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     2492 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/storage/test_catkeys.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     9086 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/storage/test_cpo.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     5570 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/storage/test_csvl10n.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     2798 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/storage/test_directory.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)    21418 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/storage/test_dtd.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     6704 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/storage/test_factory.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     3869 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/storage/test_flatxml.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)    71615 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/storage/test_fluent.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     9820 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/storage/test_html.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      483 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/storage/test_ini.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)    28694 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/storage/test_jsonl10n.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     8420 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/storage/test_mo.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1296 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/storage/test_monolingual.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)    10207 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/storage/test_mozilla_lang.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      501 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/storage/test_omegat.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     6658 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/storage/test_oo.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)    44427 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/storage/test_php.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)    38517 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/storage/test_po.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      675 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/storage/test_pocommon.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)    11275 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/storage/test_poheader.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     5392 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/storage/test_poxliff.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)    64201 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/storage/test_properties.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)    22936 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/storage/test_pypo.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1198 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/storage/test_qm.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     3239 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/storage/test_qph.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)    19149 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/storage/test_rc.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1928 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/storage/test_resourcedictionary.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     5022 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/storage/test_resx.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     6114 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/storage/test_stringsdict.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      743 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/storage/test_subtitles.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     3558 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/storage/test_tbx.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     3146 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/storage/test_tiki.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     3916 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/storage/test_tmx.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      882 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/storage/test_trados.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      211 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/storage/test_ts.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)    13697 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/storage/test_ts2.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     2002 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/storage/test_txt.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      207 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/storage/test_utx.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     2847 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/storage/test_wordfast.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)    25248 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/storage/test_xliff.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)    15664 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/storage/test_yaml.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     2697 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/storage/test_zip.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     6986 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/storage/tiki.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)    13004 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/storage/tmdb.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     5845 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/storage/tmx.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     6409 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/storage/trados.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     6935 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/storage/ts.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)    17854 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/storage/ts2.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     4994 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/storage/txt.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     9488 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/storage/utx.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)    15187 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/storage/wordfast.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     8786 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/storage/workflow.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)    33543 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/storage/xliff.py
+drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-06-14 06:36:35.081624 translate-toolkit-3.9.1/translate/storage/xml_extract/
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      716 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/storage/xml_extract/__init__.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)    14635 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/storage/xml_extract/extract.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)    11240 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/storage/xml_extract/generate.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     2825 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/storage/xml_extract/misc.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     2166 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/storage/xml_extract/test_misc.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     2955 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/storage/xml_extract/test_unit_tree.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1205 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/storage/xml_extract/test_xpath_breadcrumb.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     4854 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/storage/xml_extract/unit_tree.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     2230 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/storage/xml_extract/xpath_breadcrumb.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     2677 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/storage/xml_name.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     7211 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/storage/yaml.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     2276 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/storage/zip.py
+drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-06-14 06:36:35.085624 translate-toolkit-3.9.1/translate/tools/
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      777 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/tools/__init__.py
+drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-06-14 06:36:35.085624 translate-toolkit-3.9.1/translate/tools/__snapshots__/
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1871 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/tools/__snapshots__/test_junitmsgfmt.ambr
+-rw-r--r--   0 nijel     (1000) nijel     (1000)    13607 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/tools/__snapshots__/test_pocount.ambr
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)     3350 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/tools/build_tmdb.py
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)     2844 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/tools/junitmsgfmt.py
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)     3415 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/tools/phppo2pypo.py
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)     2363 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/tools/poclean.py
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)     3408 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/tools/pocompile.py
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)     8679 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/tools/poconflicts.py
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)    19044 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/tools/pocount.py
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)    16454 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/tools/podebug.py
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)    14678 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/tools/pogrep.py
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)     5292 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/tools/pomerge.py
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)     5643 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/tools/porestructure.py
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)     4954 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/tools/posegment.py
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)     3720 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/tools/poswap.py
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)    25251 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/tools/poterminology.py
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)     9213 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/tools/pretranslate.py
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)    12659 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/tools/pydiff.py
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)     3384 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/tools/pypo2phppo.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      714 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/tools/test_help.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      483 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/tools/test_junitmsgfmt.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1710 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/tools/test_phppo2pypo.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     7557 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/tools/test_pocount.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)    11912 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/tools/test_podebug.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     8182 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/tools/test_pogrep.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)    23743 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/tools/test_pomerge.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     3529 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/tools/test_posegment.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      945 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/tools/test_poterminology.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)    14618 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/tools/test_pretranslate.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1709 2023-06-14 06:34:21.000000 translate-toolkit-3.9.1/translate/tools/test_pypo2phppo.py
+drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-06-14 06:36:35.085624 translate-toolkit-3.9.1/translate_toolkit.egg-info/
+-rw-r--r--   0 nijel     (1000) nijel     (1000)    10785 2023-06-14 06:36:34.000000 translate-toolkit-3.9.1/translate_toolkit.egg-info/PKG-INFO
+-rw-r--r--   0 nijel     (1000) nijel     (1000)    28287 2023-06-14 06:36:34.000000 translate-toolkit-3.9.1/translate_toolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 nijel     (1000) nijel     (1000)        1 2023-06-14 06:36:34.000000 translate-toolkit-3.9.1/translate_toolkit.egg-info/dependency_links.txt
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     3197 2023-06-14 06:36:34.000000 translate-toolkit-3.9.1/translate_toolkit.egg-info/entry_points.txt
+-rw-r--r--   0 nijel     (1000) nijel     (1000)        1 2023-06-14 06:36:34.000000 translate-toolkit-3.9.1/translate_toolkit.egg-info/not-zip-safe
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      631 2023-06-14 06:36:34.000000 translate-toolkit-3.9.1/translate_toolkit.egg-info/requires.txt
+-rw-r--r--   0 nijel     (1000) nijel     (1000)       10 2023-06-14 06:36:34.000000 translate-toolkit-3.9.1/translate_toolkit.egg-info/top_level.txt
```

### Comparing `translate-toolkit-3.9.0/.github/workflows/docs.yml` & `translate-toolkit-3.9.1/.github/workflows/docs.yml`

 * *Files 18% similar despite different names*

```diff
@@ -21,16 +21,14 @@
         submodules: recursive
     - name: Setup Python
       uses: actions/setup-python@v4
       with:
         python-version: '3.11'
         cache: pip
         cache-dependency-path: requirements/*.txt
-    - name: Configure Fast APT Mirror
-      uses: vegardit/fast-apt-mirror.sh@v1
     - name: Install apt dependencies
       run: |
         sudo apt-get update
         sudo apt-get install -y libgettextpo-dev
     - name: Install dependencies
       run: |
         pip install --upgrade pip wheel
```

### Comparing `translate-toolkit-3.9.0/.github/workflows/linux.yml` & `translate-toolkit-3.9.1/.github/workflows/linux.yml`

 * *Files 12% similar despite different names*

```diff
@@ -18,33 +18,30 @@
   test:
 
     runs-on: ubuntu-latest
     strategy:
       matrix:
         requirements: [latest]
         python-version:
-        - '3.7'
         - '3.8'
         - '3.9'
         - '3.10'
         - '3.11'
         include:
         - requirements: minimal
-          python-version: '3.7'
+          python-version: '3.8'
 
     steps:
     - uses: actions/checkout@v3
     - name: Set up Python ${{ matrix.python-version }}
       uses: actions/setup-python@v4
       with:
         python-version: ${{ matrix.python-version }}
         cache: pip
         cache-dependency-path: requirements/*.txt
-    - name: Configure Fast APT Mirror
-      uses: vegardit/fast-apt-mirror.sh@v1
     - name: Install apt dependencies
       run: |
         sudo apt-get update
         sudo apt-get install -y libgettextpo-dev libxml2-dev libxmlsec1-dev gettext hunspell-af
     - name: Update pip
       run: pip install --upgrade pip wheel
     - name: Install pip dependencies
```

### Comparing `translate-toolkit-3.9.0/.github/workflows/osx.yml` & `translate-toolkit-3.9.1/.github/workflows/osx.yml`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,14 @@
   test-osx:
 
     runs-on: macos-latest
     strategy:
       matrix:
         requirements: [latest]
         python-version:
-        - '3.7'
         - '3.8'
         - '3.9'
         - '3.10'
         - '3.11'
 
     steps:
     - uses: actions/checkout@v3
```

### Comparing `translate-toolkit-3.9.0/.github/workflows/pre-commit.yml` & `translate-toolkit-3.9.1/.github/workflows/pre-commit.yml`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/.github/workflows/win.yml` & `translate-toolkit-3.9.1/.github/workflows/win.yml`

 * *Files 9% similar despite different names*

```diff
@@ -18,15 +18,14 @@
   test-win:
 
     runs-on: windows-latest
     strategy:
       matrix:
         requirements: [latest]
         python-version:
-        - '3.7'
         - '3.8'
         - '3.9'
         - '3.10'
         - '3.11'
 
     steps:
     - uses: actions/checkout@v3
```

### Comparing `translate-toolkit-3.9.0/.gitignore` & `translate-toolkit-3.9.1/.gitignore`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/.pre-commit-config.yaml` & `translate-toolkit-3.9.1/.pre-commit-config.yaml`

 * *Files 22% similar despite different names*

```diff
@@ -7,32 +7,27 @@
   - id: check-yaml
   - id: check-merge-conflict
   - id: check-json
   - id: check-toml
   - id: requirements-txt-fixer
   - id: fix-encoding-pragma
     args: [--remove]
-- repo: https://github.com/macisamuele/language-formatters-pre-commit-hooks
-  rev: v2.8.0
-  hooks:
-  - id: pretty-format-toml
-    args: [--autofix]
 - repo: meta
   hooks:
   - id: check-hooks-apply
   - id: check-useless-excludes
 - repo: https://github.com/pycqa/isort
   rev: 5.12.0
   hooks:
   - id: isort
 - repo: https://github.com/asottile/pyupgrade
-  rev: v3.4.0
+  rev: v3.6.0
   hooks:
   - id: pyupgrade
-    args: [--py36-plus]
+    args: [--py38-plus]
 - repo: https://github.com/psf/black
   rev: 23.3.0
   hooks:
   - id: black
 - repo: https://github.com/PyCQA/flake8
   rev: 6.0.0
   hooks:
@@ -42,11 +37,13 @@
     - flake8-mutable
     - flake8-polyfill
 - repo: https://github.com/PyCQA/pydocstyle
   rev: 6.3.0
   hooks:
   - id: pydocstyle
 - repo: https://github.com/macisamuele/language-formatters-pre-commit-hooks
-  rev: v2.8.0
+  rev: v2.9.0
   hooks:
   - id: pretty-format-yaml
     args: [--autofix, --indent, '2']
+  - id: pretty-format-toml
+    args: [--autofix]
```

### Comparing `translate-toolkit-3.9.0/.readthedocs.yml` & `translate-toolkit-3.9.1/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/COPYING` & `translate-toolkit-3.9.1/COPYING`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/CREDITS` & `translate-toolkit-3.9.1/CREDITS`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/Makefile` & `translate-toolkit-3.9.1/Makefile`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/PKG-INFO` & `translate-toolkit-3.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: translate-toolkit
-Version: 3.9.0
+Version: 3.9.1
 Summary: Tools and API for translation and localization engineering.
 Home-page: https://toolkit.translatehouse.org/
 Download-URL: https://github.com/translate/translate/releases/
 Author: Translate
 Author-email: translate-devel@lists.sourceforge.net
 License: GPL-2.0-or-later
 Project-URL: Issue Tracker, https://github.com/translate/translate/issues
@@ -19,23 +19,22 @@
 Classifier: Operating System :: OS Independent
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Internationalization
 Classifier: Topic :: Software Development :: Localization
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 Provides-Extra: all
 Provides-Extra: Subtitles
 Provides-Extra: Trados
 Provides-Extra: chardet
 Provides-Extra: tmserver
 Provides-Extra: Fluent
@@ -145,15 +144,15 @@
 .. note:: Please check ``requirements/*.txt``::
 
        pip install -r requirements/optional.txt
 
    Will install all optional dependencies convering support for many other
    formats.
 
-The Toolkit requires Python 3.7 or newer.
+The Toolkit requires Python 3.8 or newer.
 
 The package lxml is required. You should install version 4.6.3 or later.
 <http://lxml.de/> Depending on your platform, the easiest way to install might
 be through your system's package management. Alternatively you can try ::
 
     pip install lxml
```

### Comparing `translate-toolkit-3.9.0/README.rst` & `translate-toolkit-3.9.1/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -94,15 +94,15 @@
 .. note:: Please check ``requirements/*.txt``::
 
        pip install -r requirements/optional.txt
 
    Will install all optional dependencies convering support for many other
    formats.
 
-The Toolkit requires Python 3.7 or newer.
+The Toolkit requires Python 3.8 or newer.
 
 The package lxml is required. You should install version 4.6.3 or later.
 <http://lxml.de/> Depending on your platform, the easiest way to install might
 be through your system's package management. Alternatively you can try ::
 
     pip install lxml
```

### Comparing `translate-toolkit-3.9.0/docs/Makefile` & `translate-toolkit-3.9.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/docs/_ext/translate_docs.py` & `translate-toolkit-3.9.1/docs/_ext/translate_docs.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/docs/_themes/README.rst` & `translate-toolkit-3.9.1/docs/_themes/README.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/docs/_themes/sphinx-bootstrap/layout.html` & `translate-toolkit-3.9.1/docs/_themes/sphinx-bootstrap/layout.html`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/docs/_themes/sphinx-bootstrap/search.html` & `translate-toolkit-3.9.1/docs/_themes/sphinx-bootstrap/search.html`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/docs/_themes/sphinx-bootstrap/static/bootstrap-responsive.css` & `translate-toolkit-3.9.1/docs/_themes/sphinx-bootstrap/static/bootstrap-responsive.css`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/docs/_themes/sphinx-bootstrap/static/bootstrap-sphinx.js` & `translate-toolkit-3.9.1/docs/_themes/sphinx-bootstrap/static/bootstrap-sphinx.js`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/docs/_themes/sphinx-bootstrap/static/bootstrap.css` & `translate-toolkit-3.9.1/docs/_themes/sphinx-bootstrap/static/bootstrap.css`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/docs/_themes/sphinx-bootstrap/static/bootstrap.js` & `translate-toolkit-3.9.1/docs/_themes/sphinx-bootstrap/static/bootstrap.js`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/docs/_themes/sphinx-bootstrap/static/font/fontawesome-webfont.eot` & `translate-toolkit-3.9.1/docs/_themes/sphinx-bootstrap/static/font/fontawesome-webfont.eot`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/docs/_themes/sphinx-bootstrap/static/font/fontawesome-webfont.svg` & `translate-toolkit-3.9.1/docs/_themes/sphinx-bootstrap/static/font/fontawesome-webfont.svg`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/docs/_themes/sphinx-bootstrap/static/font/fontawesome-webfont.ttf` & `translate-toolkit-3.9.1/docs/_themes/sphinx-bootstrap/static/font/fontawesome-webfont.ttf`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/docs/_themes/sphinx-bootstrap/static/font/fontawesome-webfont.woff` & `translate-toolkit-3.9.1/docs/_themes/sphinx-bootstrap/static/font/fontawesome-webfont.woff`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/docs/_themes/sphinx-bootstrap/static/jquery.js` & `translate-toolkit-3.9.1/docs/_themes/sphinx-bootstrap/static/jquery.js`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/docs/_themes/sphinx-bootstrap/static/less/font-awesome.less` & `translate-toolkit-3.9.1/docs/_themes/sphinx-bootstrap/static/less/font-awesome.less`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/docs/_themes/sphinx-bootstrap/static/less/theme.less` & `translate-toolkit-3.9.1/docs/_themes/sphinx-bootstrap/static/less/theme.less`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/docs/_themes/sphinx-bootstrap/static/less/variables.less` & `translate-toolkit-3.9.1/docs/_themes/sphinx-bootstrap/static/less/variables.less`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/docs/api/convert.rst` & `translate-toolkit-3.9.1/docs/api/convert.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/docs/api/filters.rst` & `translate-toolkit-3.9.1/docs/api/filters.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/docs/api/index.rst` & `translate-toolkit-3.9.1/docs/api/index.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/docs/api/lang.rst` & `translate-toolkit-3.9.1/docs/api/lang.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/docs/api/misc.rst` & `translate-toolkit-3.9.1/docs/api/misc.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/docs/api/storage.rst` & `translate-toolkit-3.9.1/docs/api/storage.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/docs/api/tools.rst` & `translate-toolkit-3.9.1/docs/api/tools.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/docs/commands/csv2po.rst` & `translate-toolkit-3.9.1/docs/commands/csv2po.rst`

 * *Files 4% similar despite different names*

```diff
@@ -86,14 +86,16 @@
 |        |                 | into the PO file                            |
 +--------+-----------------+---------------------------------------------+
 |  B     | Source Language | The msgid or source string                  |
 +--------+-----------------+---------------------------------------------+
 |  C     | Target Language | The msgstr or target language               |
 +--------+-----------------+---------------------------------------------+
 
+The layout can be customized by ``--columnorder``, you can add, or remove columns using that as well, for example ``--columnorder=context,source,target``.
+
 .. _csv2po#examples:
 
 Examples
 ========
 
 These examples demonstrate the use of csv2po::
```

### Comparing `translate-toolkit-3.9.0/docs/commands/csv2tbx.rst` & `translate-toolkit-3.9.1/docs/commands/csv2tbx.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/docs/commands/flatxml2po.rst` & `translate-toolkit-3.9.1/docs/commands/flatxml2po.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/docs/commands/general_usage.rst` & `translate-toolkit-3.9.1/docs/commands/general_usage.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/docs/commands/html2po.rst` & `translate-toolkit-3.9.1/docs/commands/html2po.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/docs/commands/ical2po.rst` & `translate-toolkit-3.9.1/docs/commands/ical2po.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/docs/commands/index.rst` & `translate-toolkit-3.9.1/docs/commands/index.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/docs/commands/ini2po.rst` & `translate-toolkit-3.9.1/docs/commands/ini2po.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/docs/commands/json2po.rst` & `translate-toolkit-3.9.1/docs/commands/json2po.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/docs/commands/levenshtein_distance.rst` & `translate-toolkit-3.9.1/docs/commands/levenshtein_distance.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/docs/commands/moz-l10n-builder.rst` & `translate-toolkit-3.9.1/docs/commands/moz-l10n-builder.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/docs/commands/moz2po.rst` & `translate-toolkit-3.9.1/docs/commands/moz2po.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/docs/commands/mozilla_l10n_scripts.rst` & `translate-toolkit-3.9.1/docs/commands/mozilla_l10n_scripts.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/docs/commands/odf2xliff.rst` & `translate-toolkit-3.9.1/docs/commands/odf2xliff.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/docs/commands/oo2po.rst` & `translate-toolkit-3.9.1/docs/commands/oo2po.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/docs/commands/option_accelerator.rst` & `translate-toolkit-3.9.1/docs/commands/option_accelerator.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/docs/commands/option_duplicates.rst` & `translate-toolkit-3.9.1/docs/commands/option_duplicates.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/docs/commands/option_errorlevel.rst` & `translate-toolkit-3.9.1/docs/commands/option_errorlevel.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/docs/commands/option_filteraction.rst` & `translate-toolkit-3.9.1/docs/commands/option_filteraction.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/docs/commands/option_multifile.rst` & `translate-toolkit-3.9.1/docs/commands/option_multifile.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/docs/commands/option_personality.rst` & `translate-toolkit-3.9.1/docs/commands/option_personality.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/docs/commands/option_progress.rst` & `translate-toolkit-3.9.1/docs/commands/option_progress.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/docs/commands/option_rewrite.rst` & `translate-toolkit-3.9.1/docs/commands/option_rewrite.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/docs/commands/phase.rst` & `translate-toolkit-3.9.1/docs/commands/phase.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/docs/commands/php2po.rst` & `translate-toolkit-3.9.1/docs/commands/php2po.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/docs/commands/po2tmx.rst` & `translate-toolkit-3.9.1/docs/commands/po2tmx.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/docs/commands/po2wordfast.rst` & `translate-toolkit-3.9.1/docs/commands/po2wordfast.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/docs/commands/poclean.rst` & `translate-toolkit-3.9.1/docs/commands/poclean.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/docs/commands/pocommentclean.rst` & `translate-toolkit-3.9.1/docs/commands/pocommentclean.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/docs/commands/pocompendium.rst` & `translate-toolkit-3.9.1/docs/commands/pocompendium.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/docs/commands/pocompile.rst` & `translate-toolkit-3.9.1/docs/commands/pocompile.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/docs/commands/poconflicts.rst` & `translate-toolkit-3.9.1/docs/commands/poconflicts.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/docs/commands/pocount.rst` & `translate-toolkit-3.9.1/docs/commands/pocount.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/docs/commands/podebug.rst` & `translate-toolkit-3.9.1/docs/commands/podebug.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/docs/commands/pofilter.rst` & `translate-toolkit-3.9.1/docs/commands/pofilter.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/docs/commands/pofilter_tests.rst` & `translate-toolkit-3.9.1/docs/commands/pofilter_tests.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/docs/commands/pogrep.rst` & `translate-toolkit-3.9.1/docs/commands/pogrep.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/docs/commands/pomerge.rst` & `translate-toolkit-3.9.1/docs/commands/pomerge.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/docs/commands/pomigrate2.rst` & `translate-toolkit-3.9.1/docs/commands/pomigrate2.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/docs/commands/popuretext.rst` & `translate-toolkit-3.9.1/docs/commands/popuretext.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/docs/commands/poreencode.rst` & `translate-toolkit-3.9.1/docs/commands/poreencode.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/docs/commands/porestructure.rst` & `translate-toolkit-3.9.1/docs/commands/porestructure.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/docs/commands/posegment.rst` & `translate-toolkit-3.9.1/docs/commands/posegment.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/docs/commands/posplit.rst` & `translate-toolkit-3.9.1/docs/commands/posplit.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/docs/commands/poswap.rst` & `translate-toolkit-3.9.1/docs/commands/poswap.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/docs/commands/pot2po.rst` & `translate-toolkit-3.9.1/docs/commands/pot2po.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/docs/commands/poterminology.rst` & `translate-toolkit-3.9.1/docs/commands/poterminology.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/docs/commands/poterminology_stopword_file.rst` & `translate-toolkit-3.9.1/docs/commands/poterminology_stopword_file.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/docs/commands/pretranslate.rst` & `translate-toolkit-3.9.1/docs/commands/pretranslate.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/docs/commands/prop2po.rst` & `translate-toolkit-3.9.1/docs/commands/prop2po.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/docs/commands/rc2po.rst` & `translate-toolkit-3.9.1/docs/commands/rc2po.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/docs/commands/resx2po.rst` & `translate-toolkit-3.9.1/docs/commands/resx2po.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/docs/commands/sub2po.rst` & `translate-toolkit-3.9.1/docs/commands/sub2po.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/docs/commands/symb2po.rst` & `translate-toolkit-3.9.1/docs/commands/symb2po.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/docs/commands/tbx2po.rst` & `translate-toolkit-3.9.1/docs/commands/tbx2po.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/docs/commands/tiki2po.rst` & `translate-toolkit-3.9.1/docs/commands/tiki2po.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/docs/commands/tmserver.rst` & `translate-toolkit-3.9.1/docs/commands/tmserver.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/docs/commands/ts2po.rst` & `translate-toolkit-3.9.1/docs/commands/ts2po.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/docs/commands/txt2po.rst` & `translate-toolkit-3.9.1/docs/commands/txt2po.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/docs/commands/web2py2po.rst` & `translate-toolkit-3.9.1/docs/commands/web2py2po.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/docs/commands/xliff2po.rst` & `translate-toolkit-3.9.1/docs/commands/xliff2po.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/docs/commands/yaml2po.rst` & `translate-toolkit-3.9.1/docs/commands/yaml2po.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/docs/conf.py` & `translate-toolkit-3.9.1/docs/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 # -- Project information -----------------------------------------------------
 
 project = "Translate Toolkit"
 copyright = "2002-2023, Translate"
 
 # The short X.Y version.
-version = "3.9.0"
+version = "3.9.1"
 
 # The full version, including alpha/beta/rc tags
 release = version
 
 # -- General configuration ---------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
```

### Comparing `translate-toolkit-3.9.0/docs/contents.rst.inc` & `translate-toolkit-3.9.1/docs/contents.rst.inc`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/docs/developers/building.rst` & `translate-toolkit-3.9.1/docs/developers/building.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/docs/developers/contributing.rst` & `translate-toolkit-3.9.1/docs/developers/contributing.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/docs/developers/deprecation.rst` & `translate-toolkit-3.9.1/docs/developers/deprecation.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/docs/developers/developers.rst` & `translate-toolkit-3.9.1/docs/developers/developers.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/docs/developers/releasing.rst` & `translate-toolkit-3.9.1/docs/developers/releasing.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/docs/developers/reporting_bugs.rst` & `translate-toolkit-3.9.1/docs/developers/reporting_bugs.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/docs/developers/styleguide.rst` & `translate-toolkit-3.9.1/docs/developers/styleguide.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/docs/developers/testing.rst` & `translate-toolkit-3.9.1/docs/developers/testing.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/docs/features.rst` & `translate-toolkit-3.9.1/docs/features.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/docs/formats/android.rst` & `translate-toolkit-3.9.1/docs/formats/android.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/docs/formats/base_classes.rst` & `translate-toolkit-3.9.1/docs/formats/base_classes.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/docs/formats/catkeys.rst` & `translate-toolkit-3.9.1/docs/formats/catkeys.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/docs/formats/conformance.rst` & `translate-toolkit-3.9.1/docs/formats/conformance.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/docs/formats/csv.rst` & `translate-toolkit-3.9.1/docs/formats/csv.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/docs/formats/dtd.rst` & `translate-toolkit-3.9.1/docs/formats/dtd.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/docs/formats/flatxml.rst` & `translate-toolkit-3.9.1/docs/formats/flatxml.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/docs/formats/html.rst` & `translate-toolkit-3.9.1/docs/formats/html.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/docs/formats/ical.rst` & `translate-toolkit-3.9.1/docs/formats/ical.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/docs/formats/index.rst` & `translate-toolkit-3.9.1/docs/formats/index.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/docs/formats/ini.rst` & `translate-toolkit-3.9.1/docs/formats/ini.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/docs/formats/json.rst` & `translate-toolkit-3.9.1/docs/formats/json.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/docs/formats/mo.rst` & `translate-toolkit-3.9.1/docs/formats/mo.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/docs/formats/odf.rst` & `translate-toolkit-3.9.1/docs/formats/odf.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/docs/formats/omegat_glossary.rst` & `translate-toolkit-3.9.1/docs/formats/omegat_glossary.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/docs/formats/php.rst` & `translate-toolkit-3.9.1/docs/formats/php.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/docs/formats/po.rst` & `translate-toolkit-3.9.1/docs/formats/po.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/docs/formats/properties.rst` & `translate-toolkit-3.9.1/docs/formats/properties.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/docs/formats/qm.rst` & `translate-toolkit-3.9.1/docs/formats/qm.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/docs/formats/qt_phrase_book.rst` & `translate-toolkit-3.9.1/docs/formats/qt_phrase_book.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/docs/formats/quoting_and_escaping.rst` & `translate-toolkit-3.9.1/docs/formats/quoting_and_escaping.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/docs/formats/rc.rst` & `translate-toolkit-3.9.1/docs/formats/rc.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/docs/formats/resx.rst` & `translate-toolkit-3.9.1/docs/formats/resx.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/docs/formats/strings.rst` & `translate-toolkit-3.9.1/docs/formats/strings.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/docs/formats/subtitles.rst` & `translate-toolkit-3.9.1/docs/formats/subtitles.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/docs/formats/tbx.rst` & `translate-toolkit-3.9.1/docs/formats/tbx.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/docs/formats/text.rst` & `translate-toolkit-3.9.1/docs/formats/text.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/docs/formats/tmx.rst` & `translate-toolkit-3.9.1/docs/formats/tmx.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/docs/formats/ts.rst` & `translate-toolkit-3.9.1/docs/formats/ts.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/docs/formats/utx.rst` & `translate-toolkit-3.9.1/docs/formats/utx.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/docs/formats/wiki.rst` & `translate-toolkit-3.9.1/docs/formats/wiki.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/docs/formats/wordfast.rst` & `translate-toolkit-3.9.1/docs/formats/wordfast.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/docs/formats/xliff.rst` & `translate-toolkit-3.9.1/docs/formats/xliff.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/docs/guides/checking_for_inconsistencies.rst` & `translate-toolkit-3.9.1/docs/guides/checking_for_inconsistencies.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/docs/guides/cleanup_translator_comments.rst` & `translate-toolkit-3.9.1/docs/guides/cleanup_translator_comments.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/docs/guides/creating_a_terminology_list_from_your_existing_translations.rst` & `translate-toolkit-3.9.1/docs/guides/creating_a_terminology_list_from_your_existing_translations.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/docs/guides/creating_mozilla_pot_files.rst` & `translate-toolkit-3.9.1/docs/guides/creating_mozilla_pot_files.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/docs/guides/document_translation.rst` & `translate-toolkit-3.9.1/docs/guides/document_translation.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/docs/guides/index.rst` & `translate-toolkit-3.9.1/docs/guides/index.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/docs/guides/migrating_translations.rst` & `translate-toolkit-3.9.1/docs/guides/migrating_translations.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/docs/guides/running_the_tools_on_microsoft_windows.rst` & `translate-toolkit-3.9.1/docs/guides/running_the_tools_on_microsoft_windows.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/docs/guides/using_csv2po.rst` & `translate-toolkit-3.9.1/docs/guides/using_csv2po.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/docs/guides/using_oo2po.rst` & `translate-toolkit-3.9.1/docs/guides/using_oo2po.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/docs/guides/using_pofilter.rst` & `translate-toolkit-3.9.1/docs/guides/using_pofilter.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/docs/history.rst` & `translate-toolkit-3.9.1/docs/history.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/docs/installation.rst` & `translate-toolkit-3.9.1/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/docs/make.bat` & `translate-toolkit-3.9.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/docs/releases/0.10.rst` & `translate-toolkit-3.9.1/docs/releases/0.10.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/docs/releases/0.11.rst` & `translate-toolkit-3.9.1/docs/releases/0.11.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/docs/releases/0.9.rst` & `translate-toolkit-3.9.1/docs/releases/0.9.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/docs/releases/1.0.1.rst` & `translate-toolkit-3.9.1/docs/releases/1.0.1.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/docs/releases/1.0.rst` & `translate-toolkit-3.9.1/docs/releases/1.0.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/docs/releases/1.1.0.rst` & `translate-toolkit-3.9.1/docs/releases/1.1.0.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/docs/releases/1.1.1.rst` & `translate-toolkit-3.9.1/docs/releases/1.1.1.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/docs/releases/1.10.0.rst` & `translate-toolkit-3.9.1/docs/releases/1.10.0.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/docs/releases/1.11.0.rst` & `translate-toolkit-3.9.1/docs/releases/1.11.0.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/docs/releases/1.12.0.rst` & `translate-toolkit-3.9.1/docs/releases/1.12.0.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/docs/releases/1.13.0.rst` & `translate-toolkit-3.9.1/docs/releases/1.13.0.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/docs/releases/1.2.0.rst` & `translate-toolkit-3.9.1/docs/releases/1.2.0.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/docs/releases/1.4.0.rst` & `translate-toolkit-3.9.1/docs/releases/1.4.0.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/docs/releases/1.4.1.rst` & `translate-toolkit-3.9.1/docs/releases/1.4.1.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/docs/releases/1.6.0.rst` & `translate-toolkit-3.9.1/docs/releases/1.6.0.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/docs/releases/1.8.1.rst` & `translate-toolkit-3.9.1/docs/releases/1.8.1.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/docs/releases/1.9.0.rst` & `translate-toolkit-3.9.1/docs/releases/1.9.0.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/docs/releases/2.0.0.rst` & `translate-toolkit-3.9.1/docs/releases/2.0.0.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/docs/releases/2.1.0.rst` & `translate-toolkit-3.9.1/docs/releases/2.1.0.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/docs/releases/2.2.0.rst` & `translate-toolkit-3.9.1/docs/releases/2.2.0.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/docs/releases/2.2.1.rst` & `translate-toolkit-3.9.1/docs/releases/2.2.1.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/docs/releases/2.2.4.rst` & `translate-toolkit-3.9.1/docs/releases/2.2.4.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/docs/releases/2.2.5.rst` & `translate-toolkit-3.9.1/docs/releases/2.2.5.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/docs/releases/2.3.0.rst` & `translate-toolkit-3.9.1/docs/releases/2.3.0.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/docs/releases/2.3.1.rst` & `translate-toolkit-3.9.1/docs/releases/2.3.1.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/docs/releases/2.4.0.rst` & `translate-toolkit-3.9.1/docs/releases/2.4.0.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/docs/releases/2.5.0.rst` & `translate-toolkit-3.9.1/docs/releases/2.5.0.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/docs/releases/2.5.1.rst` & `translate-toolkit-3.9.1/docs/releases/2.5.1.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/docs/releases/3.0.0.rst` & `translate-toolkit-3.9.1/docs/releases/3.0.0.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/docs/releases/3.1.0.rst` & `translate-toolkit-3.9.1/docs/releases/3.1.0.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/docs/releases/3.2.0.rst` & `translate-toolkit-3.9.1/docs/releases/3.2.0.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/docs/releases/3.3.0.rst` & `translate-toolkit-3.9.1/docs/releases/3.3.0.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/docs/releases/3.3.2.rst` & `translate-toolkit-3.9.1/docs/releases/3.3.2.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/docs/releases/3.3.3.rst` & `translate-toolkit-3.9.1/docs/releases/3.3.3.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/docs/releases/3.4.0.rst` & `translate-toolkit-3.9.1/docs/releases/3.4.0.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/docs/releases/3.4.1.rst` & `translate-toolkit-3.9.1/docs/releases/3.4.1.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/docs/releases/3.6.0.rst` & `translate-toolkit-3.9.1/docs/releases/3.6.0.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/docs/releases/3.6.1.rst` & `translate-toolkit-3.9.1/docs/releases/3.6.1.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/docs/releases/3.7.0.rst` & `translate-toolkit-3.9.1/docs/releases/3.7.0.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/docs/releases/3.7.3.rst` & `translate-toolkit-3.9.1/docs/releases/3.7.3.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/docs/releases/3.7.4.rst` & `translate-toolkit-3.9.1/docs/releases/3.7.4.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/docs/releases/3.8.0.rst` & `translate-toolkit-3.9.1/docs/releases/3.8.0.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/docs/releases/3.8.1.rst` & `translate-toolkit-3.9.1/docs/releases/3.8.1.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/docs/releases/3.9.0.rst` & `translate-toolkit-3.9.1/docs/releases/3.9.0.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/docs/releases/README.rst` & `translate-toolkit-3.9.1/docs/releases/README.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/docs/releases/index.rst` & `translate-toolkit-3.9.1/docs/releases/index.rst`

 * *Files 4% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 
 Final releases
 ==============
 
 .. toctree::
    :maxdepth: 1
 
+   3.9.1 <3.9.1>
    3.9.0 <3.9.0>
    3.8.6 <3.8.6>
    3.8.5 <3.8.5>
    3.8.4 <3.8.4>
    3.8.3 <3.8.3>
    3.8.2 <3.8.2>
    3.8.1 <3.8.1>
```

### Comparing `translate-toolkit-3.9.0/requirements/optional.txt` & `translate-toolkit-3.9.1/requirements/optional.txt`

 * *Files 2% similar despite different names*

```diff
@@ -3,25 +3,25 @@
 # Format support
 aeidon==1.12        # Subtitles
 # Format support
 BeautifulSoup4>=4.3  # Trados
 # Encoding detection
 charset-normalizer==3.1.0   # chardet
 # Tmserver backend
-cheroot==9.0.0       # tmserver
+cheroot==10.0.0       # tmserver
 # Format support
 fluent.syntax==0.19.0 # Fluent
 # Format support
 iniparse==0.5        # INI
 # Format support
 phply==1.2.6         # PHP
 # To provide translations for language names without need for OS package.
 pycountry==22.3.5          # Languages
 pyenchant==3.2.2     # spellcheck
 # Windows Resources (rc2po and po2rc)
 pyparsing==3.0.9     # RC
 # Faster matching in e.g. pot2po
 python-Levenshtein>=0.12    # Levenshtein
 # Format support
-ruamel.yaml==0.17.26 # YAML
+ruamel.yaml==0.17.31 # YAML
 # Format support
 vobject==0.9.6.1     # iCal
```

### Comparing `translate-toolkit-3.9.0/setup.cfg` & `translate-toolkit-3.9.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,14 @@
 	Operating System :: OS Independent
 	Operating System :: Microsoft :: Windows
 	Operating System :: MacOS :: MacOS X
 	Operating System :: Unix
 	Programming Language :: Python
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3 :: Only
-	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
 	Topic :: Software Development :: Internationalization
 	Topic :: Software Development :: Localization
 	Topic :: Software Development :: Libraries :: Python Modules
@@ -35,15 +34,15 @@
 project_urls = 
 	Issue Tracker=https://github.com/translate/translate/issues
 	Documentation=https://docs.translatehouse.org/projects/translate-toolkit/
 	Source Code=https://github.com/translate/translate
 
 [options]
 packages = find_namespace:
-python_requires = >=3.7
+python_requires = >=3.8
 include_package_data = 1
 zip_safe = 0
 scripts = 
 	tools/mozilla/build_firefox.sh
 	tools/mozilla/buildxpi.py
 	tools/mozilla/get_moz_enUS.py
 	tools/pocommentclean
```

### Comparing `translate-toolkit-3.9.0/setup.py` & `translate-toolkit-3.9.1/setup.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/tests/cli/data/test_flatxml2po/out.po` & `translate-toolkit-3.9.1/tests/cli/data/test_flatxml2po/out.po`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/tests/cli/data/test_junitmsgfmt_failure/stdout.txt` & `translate-toolkit-3.9.1/tests/cli/data/test_junitmsgfmt_failure/stdout.txt`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/tests/cli/data/test_junitmsgfmt_untranslated/stdout.txt` & `translate-toolkit-3.9.1/tests/cli/data/test_junitmsgfmt_untranslated/stdout.txt`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/tests/cli/data/test_pocount_xliff_states_no/states.xlf` & `translate-toolkit-3.9.1/tests/cli/data/test_pocount_xliff_states_no/states.xlf`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/tests/cli/data/test_pocount_xliff_states_yes/states.xlf` & `translate-toolkit-3.9.1/tests/cli/data/test_pocount_xliff_states_yes/states.xlf`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/tests/cli/data/test_pofilter_listfilters/stdout.txt` & `translate-toolkit-3.9.1/tests/cli/data/test_pofilter_listfilters/stdout.txt`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/tests/cli/data/test_pofilter_manpage/stdout.txt` & `translate-toolkit-3.9.1/tests/cli/data/test_pofilter_manpage/stdout.txt`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/tests/cli/data/test_prop2po_files_templates/out.po` & `translate-toolkit-3.9.1/tests/cli/data/test_prop2po_files_templates/out.po`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/tests/cli/data/test_rc2po/one.rc` & `translate-toolkit-3.9.1/tests/cli/data/test_rc2po/one.rc`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/tests/cli/data/test_rc2po/out.po` & `translate-toolkit-3.9.1/tests/cli/data/test_rc2po/out.po`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/tests/cli/example_test.sh` & `translate-toolkit-3.9.1/tests/cli/example_test.sh`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/tests/cli/test.inc.sh` & `translate-toolkit-3.9.1/tests/cli/test.inc.sh`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/tests/odf_xliff/test_2-test_odf2xliff-reference.xlf` & `translate-toolkit-3.9.1/tests/odf_xliff/test_2-test_odf2xliff-reference.xlf`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/tests/odf_xliff/test_2.odt` & `translate-toolkit-3.9.1/tests/odf_xliff/test_2.odt`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/tests/odf_xliff/test_inline-test_odf2xliff_inline-reference.xlf` & `translate-toolkit-3.9.1/tests/odf_xliff/test_inline-test_odf2xliff_inline-reference.xlf`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/tests/odf_xliff/test_inline.odt` & `translate-toolkit-3.9.1/tests/odf_xliff/test_inline.odt`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/tests/odf_xliff/test_odf_xliff.py` & `translate-toolkit-3.9.1/tests/odf_xliff/test_odf_xliff.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/tests/xliff_conformance/af-pootle.po` & `translate-toolkit-3.9.1/tests/xliff_conformance/af-pootle.po`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/tests/xliff_conformance/en-US.sdf` & `translate-toolkit-3.9.1/tests/xliff_conformance/en-US.sdf`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/tests/xliff_conformance/test_xliff_conformance.py` & `translate-toolkit-3.9.1/tests/xliff_conformance/test_xliff_conformance.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/tests/xliff_conformance/xliff-core-1.1.xsd` & `translate-toolkit-3.9.1/tests/xliff_conformance/xliff-core-1.1.xsd`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/tools/mozilla/README.firefox_build_instructions.rst` & `translate-toolkit-3.9.1/tools/mozilla/README.firefox_build_instructions.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/tools/mozilla/Vagrantfile` & `translate-toolkit-3.9.1/tools/mozilla/Vagrantfile`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/tools/mozilla/accesskey_checker` & `translate-toolkit-3.9.1/tools/mozilla/accesskey_checker`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/tools/mozilla/accesskey_checker_PO` & `translate-toolkit-3.9.1/tools/mozilla/accesskey_checker_PO`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/tools/mozilla/build_firefox.sh` & `translate-toolkit-3.9.1/tools/mozilla/build_firefox.sh`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/tools/mozilla/build_tb3_langs.sh` & `translate-toolkit-3.9.1/tools/mozilla/build_tb3_langs.sh`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/tools/mozilla/buildxpi.py` & `translate-toolkit-3.9.1/tools/mozilla/buildxpi.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/tools/mozilla/get_moz_enUS.py` & `translate-toolkit-3.9.1/tools/mozilla/get_moz_enUS.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/tools/mozilla/moz-l10n-builder` & `translate-toolkit-3.9.1/tools/mozilla/moz-l10n-builder`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/tools/mozilla/moz_l10n_builder.py` & `translate-toolkit-3.9.1/tools/mozilla/moz_l10n_builder.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/tools/mozilla/mozcronbuild.py` & `translate-toolkit-3.9.1/tools/mozilla/mozcronbuild.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/tools/mozilla/mozilla-l10n.patch` & `translate-toolkit-3.9.1/tools/mozilla/mozilla-l10n.patch`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/tools/mozilla/mozzy.sh` & `translate-toolkit-3.9.1/tools/mozilla/mozzy.sh`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/tools/mozilla/postinstall.sh` & `translate-toolkit-3.9.1/tools/mozilla/postinstall.sh`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/tools/phase` & `translate-toolkit-3.9.1/tools/phase`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/tools/phaselist2goals` & `translate-toolkit-3.9.1/tools/phaselist2goals`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/tools/pocommentclean` & `translate-toolkit-3.9.1/tools/pocommentclean`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/tools/pocompendium` & `translate-toolkit-3.9.1/tools/pocompendium`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/tools/pomigrate2` & `translate-toolkit-3.9.1/tools/pomigrate2`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/tools/popuretext` & `translate-toolkit-3.9.1/tools/popuretext`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/tools/poreencode` & `translate-toolkit-3.9.1/tools/poreencode`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/tools/posplit` & `translate-toolkit-3.9.1/tools/posplit`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/__init__.py` & `translate-toolkit-3.9.1/translate/__init__.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/__version__.py` & `translate-toolkit-3.9.1/translate/__version__.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program; if not, see <http://www.gnu.org/licenses/>.
 
 """This file contains the version of the Translate Toolkit."""
 
-ver = (3, 9, 0)
+ver = (3, 9, 1)
 """Machine readable version number. Used by tools that need to adjust code
 paths based on a Translate Toolkit release number."""
 
 build = ver[0] * 10000 + ver[1] * 100 + ver[2]
 """The build number is used by external users of the Translate Toolkit to
 trigger refreshes.  Thus increase the build number whenever changes are made to
 code touching stats or quality checks.  An increased build number will force a
```

### Comparing `translate-toolkit-3.9.0/translate/convert/__init__.py` & `translate-toolkit-3.9.1/translate/convert/__init__.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/convert/accesskey.py` & `translate-toolkit-3.9.1/translate/convert/accesskey.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/convert/convert.py` & `translate-toolkit-3.9.1/translate/convert/convert.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/convert/csv2po.py` & `translate-toolkit-3.9.1/translate/convert/csv2po.py`

 * *Files 1% similar despite different names*

```diff
@@ -106,14 +106,15 @@
     def convertunit(csvunit):
         """converts csv unit to po unit"""
         pounit = po.pounit(encoding="UTF-8")
         if csvunit.location:
             pounit.addlocation(csvunit.location)
         pounit.source = csvunit.source
         pounit.target = csvunit.target
+        pounit.setcontext(csvunit.getcontext())
         return pounit
 
     def handlecsvunit(self, csvunit):
         """handles reintegrating a csv unit into the .po file"""
         if len(csvunit.location.strip()) > 0 and csvunit.location in self.commentindex:
             pounit = self.commentindex[csvunit.location]
         elif csvunit.source in self.sourceindex:
```

### Comparing `translate-toolkit-3.9.0/translate/convert/csv2tbx.py` & `translate-toolkit-3.9.1/translate/convert/csv2tbx.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/convert/dtd2po.py` & `translate-toolkit-3.9.1/translate/convert/dtd2po.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/convert/factory.py` & `translate-toolkit-3.9.1/translate/convert/factory.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/convert/flatxml2po.py` & `translate-toolkit-3.9.1/translate/convert/flatxml2po.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/convert/html2po.py` & `translate-toolkit-3.9.1/translate/convert/html2po.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/convert/ical2po.py` & `translate-toolkit-3.9.1/translate/convert/ical2po.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/convert/idml2po.py` & `translate-toolkit-3.9.1/translate/convert/idml2po.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/convert/ini2po.py` & `translate-toolkit-3.9.1/translate/convert/ini2po.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/convert/json2po.py` & `translate-toolkit-3.9.1/translate/convert/json2po.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/convert/moz2po.py` & `translate-toolkit-3.9.1/translate/convert/moz2po.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/convert/mozfunny2prop.py` & `translate-toolkit-3.9.1/translate/convert/mozfunny2prop.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/convert/mozlang2po.py` & `translate-toolkit-3.9.1/translate/convert/mozlang2po.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/convert/odf2xliff.py` & `translate-toolkit-3.9.1/translate/convert/odf2xliff.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/convert/oo2po.py` & `translate-toolkit-3.9.1/translate/convert/oo2po.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/convert/oo2xliff.py` & `translate-toolkit-3.9.1/translate/convert/oo2xliff.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/convert/php2po.py` & `translate-toolkit-3.9.1/translate/convert/php2po.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/convert/po2csv.py` & `translate-toolkit-3.9.1/translate/convert/po2csv.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,14 +39,15 @@
             # csvunit.target = "target"
         elif inputunit.isblank():
             return None
         else:
             csvunit.location = self.convertcomments(inputunit)
             csvunit.source = inputunit.source
             csvunit.target = inputunit.target
+            csvunit.setcontext(inputunit.getcontext())
         return csvunit
 
     def convertplurals(self, inputunit):
         """Convert PO plural units
 
         We only convert the first plural form.  So languages with multiple
         plurals are not handled.  For single plural languages we simply
```

### Comparing `translate-toolkit-3.9.0/translate/convert/po2dtd.py` & `translate-toolkit-3.9.1/translate/convert/po2dtd.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/convert/po2flatxml.py` & `translate-toolkit-3.9.1/translate/convert/po2flatxml.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/convert/po2html.py` & `translate-toolkit-3.9.1/translate/convert/po2html.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/convert/po2ical.py` & `translate-toolkit-3.9.1/translate/convert/po2ical.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/convert/po2idml.py` & `translate-toolkit-3.9.1/translate/convert/po2idml.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/convert/po2ini.py` & `translate-toolkit-3.9.1/translate/convert/po2ini.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/convert/po2json.py` & `translate-toolkit-3.9.1/translate/convert/po2json.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/convert/po2moz.py` & `translate-toolkit-3.9.1/translate/convert/po2moz.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/convert/po2mozlang.py` & `translate-toolkit-3.9.1/translate/convert/po2mozlang.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/convert/po2oo.py` & `translate-toolkit-3.9.1/translate/convert/po2oo.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/convert/po2php.py` & `translate-toolkit-3.9.1/translate/convert/po2php.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/convert/po2prop.py` & `translate-toolkit-3.9.1/translate/convert/po2prop.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/convert/po2rc.py` & `translate-toolkit-3.9.1/translate/convert/po2rc.py`

 * *Files 14% similar despite different names*

```diff
@@ -26,31 +26,34 @@
 
 from translate.convert import convert
 from translate.storage import po, rc
 from translate.storage.rc import (
     generate_menu_pre_name,
     generate_popup_caption_name,
     generate_popup_pre_name,
+    rcfile,
 )
 
-NL = "\r\n"
 BLOCK_START = "BEGIN"
 BLOCK_END = "END"
 
 EMPTY_LOCATION = ""
 
 
 def is_iterable_but_not_string(o):
     """Check if object is iterable but not a string."""
     return isinstance(o, Iterable) and not isinstance(o, str)
 
 
 class rerc:
     def __init__(self, templatefile, charset="utf-8", lang=None, sublang=None):
-        self.templatefile = templatefile
+        self.templatecontent = templatefile.read()
+        self.templatestore = rcfile()
+        self.templatestore.charset = charset
+        self.templatestore.parse(self.templatecontent)
         self.inputdict = {}
         self.charset = charset
         self.lang = lang
         self.sublang = sublang
 
     @staticmethod
     def convert_comment(addnl, comment):
@@ -77,38 +80,38 @@
                     yield '"' + self.inputdict[msgid][name] + '"'
                 elif EMPTY_LOCATION in self.inputdict[msgid]:
                     yield '"' + self.inputdict[msgid][EMPTY_LOCATION] + '"'
             else:
                 yield toks.caption
 
             yield from toks.post_caption  # The rest of the options
-            yield NL
+            yield self.templatestore.newline
         else:
             yield " "
             yield from toks.post_caption  # The rest of the options
-            yield NL
+            yield self.templatestore.newline
 
         yield BLOCK_START
-        yield NL
+        yield self.templatestore.newline
         addnl = False
 
         for c in toks.controls:
             if isinstance(c, str):
                 yield from self.convert_comment(addnl, c)
                 addnl = True
                 continue
             if addnl:
-                yield NL
+                yield self.templatestore.newline
                 addnl = False
             yield "    "
             c0 = c[0]
             if len(c0[0]) >= 16:
                 yield c0[0]
                 # If more than 16 char, put it on a new line to align it.
-                yield NL + " " * (16 + 4)
+                yield self.templatestore.newline + " " * (16 + 4)
             else:
                 yield c0[0].ljust(16)
 
             tmp = []
 
             # collect initial quoted items to form msgid
             i = 1
@@ -134,40 +137,43 @@
             for a in c[i:]:
                 if is_iterable_but_not_string(a):
                     tmp.append(" | ".join(a))
                 else:
                     tmp.append(a)
 
             yield ",".join(tmp)
-            yield NL
+            yield self.templatestore.newline
 
+        if addnl:
+            yield self.templatestore.newline
+            addnl = False
         yield BLOCK_END
 
     def convert_string_table(self, s, loc, toks):
         yield toks[0]
         if toks[1]:
             yield f" {toks[1]}"
-        yield NL
+        yield self.templatestore.newline
         yield BLOCK_START
-        yield NL
+        yield self.templatestore.newline
 
         addnl = False
         for c in toks.controls:
             if isinstance(c, str):
                 yield from self.convert_comment(addnl, c)
                 addnl = True
                 continue
             if addnl:
-                yield NL
+                yield self.templatestore.newline
                 addnl = False
             yield "    "
             c0 = c[0]
             if len(c0[0]) >= 24:
                 yield c0[0]
-                yield NL + " " * (24 + 4)
+                yield self.templatestore.newline + " " * (24 + 4)
             else:
                 yield c0[0].ljust(24)
 
             name = rc.generate_stringtable_name(c0[0])
             msgid = "".join(cn[1:-1] for cn in c[1:])
 
             tmp = c[1:]
@@ -175,19 +181,22 @@
                 if name in self.inputdict[msgid]:
                     tmp = ['"' + self.inputdict[msgid][name] + '"']
                 elif EMPTY_LOCATION in self.inputdict[msgid]:
                     tmp = ['"' + self.inputdict[msgid][EMPTY_LOCATION] + '"']
 
             for part in tmp[:-1]:
                 yield part
-                yield NL + " " * (24 + 4)
+                yield self.templatestore.newline + " " * (24 + 4)
             yield tmp[-1]
 
-            yield NL
+            yield self.templatestore.newline
 
+        if addnl:
+            yield self.templatestore.newline
+            addnl = False
         yield BLOCK_END
 
     def convert_language(self, s, loc, toks):
         yield "LANGUAGE "
         yield self.lang
         if self.sublang:
             yield ", "
@@ -212,19 +221,19 @@
         else:
             yield " "
 
         for value in popup.values_:
             yield ", "
             yield value
         yield from popup.post_caption  # The rest of the options
-        yield NL
+        yield self.templatestore.newline
 
         yield identation
         yield BLOCK_START
-        yield NL
+        yield self.templatestore.newline
 
         for element in popup.elements:
             if isinstance(element, str):
                 yield from self.convert_comment(True, element)
                 continue
 
             if element.block_type and element.block_type == "MENUITEM":
@@ -247,39 +256,39 @@
 
                     yield ", ".join(element.values_)
                 elif element.values_[0] == "SEPARATOR":
                     yield "SEPARATOR"
                 else:
                     raise NotImplementedError()
 
-                yield NL
+                yield self.templatestore.newline
 
             elif element.popups:
                 for sub_popup in element.popups:
                     yield from self.convert_popup(
                         sub_popup,
                         generate_popup_pre_name(pre_name, popup.caption[1:-1]),
                         ident + 1,
                     )
         yield identation
         yield BLOCK_END
-        yield NL
+        yield self.templatestore.newline
 
     def convert_menu(self, s, loc, toks):
         yield toks.block_id[0]
         yield " "
         yield toks.block_type
 
         # A menu can't have CAPTION, so don't try to translate it.
         yield " "
         yield from toks.post_caption  # The rest of the options
-        yield NL
+        yield self.templatestore.newline
 
         yield BLOCK_START
-        yield NL
+        yield self.templatestore.newline
 
         pre_name = generate_menu_pre_name(toks.block_type, toks.block_id[0])
 
         for p in toks.popups:
             yield from self.convert_popup(p, pre_name)
 
         yield BLOCK_END
@@ -303,15 +312,15 @@
 
         return toks
 
     def convertstore(self, inputstore, includefuzzy=False):
         self.makestoredict(inputstore, includefuzzy)
         statement = rc.rc_statement()
         statement.add_parse_action(self.translate_strings)
-        return statement.transform_string(self.templatefile.read().decode(self.charset))
+        return statement.transform_string(self.templatecontent.decode(self.charset))
 
     def makestoredict(self, store, includefuzzy=False):
         """make a dictionary of the translations"""
         for unit in store.units:
             if includefuzzy or not unit.isfuzzy():
                 rcstring = unit.target
                 if len(rcstring.strip()) == 0:
```

### Comparing `translate-toolkit-3.9.0/translate/convert/po2resx.py` & `translate-toolkit-3.9.1/translate/convert/po2resx.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/convert/po2sub.py` & `translate-toolkit-3.9.1/translate/convert/po2sub.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/convert/po2symb.py` & `translate-toolkit-3.9.1/translate/convert/po2symb.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/convert/po2tiki.py` & `translate-toolkit-3.9.1/translate/convert/po2tiki.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/convert/po2tmx.py` & `translate-toolkit-3.9.1/translate/convert/po2tmx.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/convert/po2ts.py` & `translate-toolkit-3.9.1/translate/convert/po2ts.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/convert/po2txt.py` & `translate-toolkit-3.9.1/translate/convert/po2txt.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/convert/po2web2py.py` & `translate-toolkit-3.9.1/translate/convert/po2web2py.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/convert/po2wordfast.py` & `translate-toolkit-3.9.1/translate/convert/po2wordfast.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/convert/po2xliff.py` & `translate-toolkit-3.9.1/translate/convert/po2xliff.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/convert/po2yaml.py` & `translate-toolkit-3.9.1/translate/convert/po2yaml.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/convert/pot2po.py` & `translate-toolkit-3.9.1/translate/convert/pot2po.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/convert/prop2mozfunny.py` & `translate-toolkit-3.9.1/translate/convert/prop2mozfunny.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/convert/prop2po.py` & `translate-toolkit-3.9.1/translate/convert/prop2po.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/convert/rc2po.py` & `translate-toolkit-3.9.1/translate/convert/rc2po.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/convert/resx2po.py` & `translate-toolkit-3.9.1/translate/convert/resx2po.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/convert/roundtrip-OOo` & `translate-toolkit-3.9.1/translate/convert/roundtrip-OOo`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/convert/roundtrip-gaia` & `translate-toolkit-3.9.1/translate/convert/roundtrip-gaia`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/convert/roundtrip-mozilla` & `translate-toolkit-3.9.1/translate/convert/roundtrip-mozilla`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/convert/sub2po.py` & `translate-toolkit-3.9.1/translate/convert/sub2po.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/convert/symb2po.py` & `translate-toolkit-3.9.1/translate/convert/symb2po.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/convert/tbx2po.py` & `translate-toolkit-3.9.1/translate/convert/tbx2po.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/convert/test.idml` & `translate-toolkit-3.9.1/translate/convert/test.idml`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/convert/test.odt` & `translate-toolkit-3.9.1/translate/convert/test.odt`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/convert/test_accesskey.py` & `translate-toolkit-3.9.1/translate/convert/test_accesskey.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/convert/test_convert.py` & `translate-toolkit-3.9.1/translate/convert/test_convert.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/convert/test_csv2po.py` & `translate-toolkit-3.9.1/translate/convert/test_csv2po.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/convert/test_dtd2po.py` & `translate-toolkit-3.9.1/translate/convert/test_dtd2po.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/convert/test_flatxml2po.py` & `translate-toolkit-3.9.1/translate/convert/test_flatxml2po.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/convert/test_html2po.py` & `translate-toolkit-3.9.1/translate/convert/test_html2po.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/convert/test_ical2po.py` & `translate-toolkit-3.9.1/translate/convert/test_ical2po.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/convert/test_ini2po.py` & `translate-toolkit-3.9.1/translate/convert/test_ini2po.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/convert/test_json2po.py` & `translate-toolkit-3.9.1/translate/convert/test_json2po.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/convert/test_mozfunny2prop.py` & `translate-toolkit-3.9.1/translate/convert/test_mozfunny2prop.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/convert/test_mozlang2po.py` & `translate-toolkit-3.9.1/translate/convert/test_mozlang2po.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/convert/test_oo2po.py` & `translate-toolkit-3.9.1/translate/convert/test_oo2po.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/convert/test_oo2xliff.py` & `translate-toolkit-3.9.1/translate/convert/test_oo2xliff.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/convert/test_php2po.py` & `translate-toolkit-3.9.1/translate/convert/test_php2po.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/convert/test_po2csv.py` & `translate-toolkit-3.9.1/translate/convert/test_po2csv.py`

 * *Files 4% similar despite different names*

```diff
@@ -161,7 +161,20 @@
         content = self.open_testfile("test.csv", "r").read()
         assert (
             content
             == """"target","source"
 "Target","Same"
 """
         )
+
+    def test_context(self):
+        pocontent = '#: simple.c\nmsgctxt "Context"\nmsgid "Same"\nmsgstr "Target"\n'
+        self.create_testfile("test.po", pocontent)
+
+        self.run_command("test.po", "test.csv", columnorder="context,source,target")
+        content = self.open_testfile("test.csv", "r").read()
+        assert (
+            content
+            == """"context","source","target"
+"Context","Same","Target"
+"""
+        )
```

### Comparing `translate-toolkit-3.9.0/translate/convert/test_po2dtd.py` & `translate-toolkit-3.9.1/translate/convert/test_po2dtd.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/convert/test_po2flatxml.py` & `translate-toolkit-3.9.1/translate/convert/test_po2flatxml.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/convert/test_po2html.py` & `translate-toolkit-3.9.1/translate/convert/test_po2html.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/convert/test_po2ical.py` & `translate-toolkit-3.9.1/translate/convert/test_po2ical.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/convert/test_po2idml.py` & `translate-toolkit-3.9.1/translate/convert/test_po2idml.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/convert/test_po2ini.py` & `translate-toolkit-3.9.1/translate/convert/test_po2ini.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/convert/test_po2json.py` & `translate-toolkit-3.9.1/translate/convert/test_po2json.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/convert/test_po2mozlang.py` & `translate-toolkit-3.9.1/translate/convert/test_po2mozlang.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/convert/test_po2oo.py` & `translate-toolkit-3.9.1/translate/convert/test_po2oo.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/convert/test_po2php.py` & `translate-toolkit-3.9.1/translate/convert/test_po2php.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/convert/test_po2prop.py` & `translate-toolkit-3.9.1/translate/convert/test_po2prop.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/convert/test_po2rc.py` & `translate-toolkit-3.9.1/translate/convert/test_po2rc.py`

 * *Files 11% similar despite different names*

```diff
@@ -24,14 +24,15 @@
     CTEXT           "You can use it without registering it",IDC_STATIC,35,131,128,19,SS_SUNKEN
     PUSHBUTTON      "Offline",IDC_OFFLINE,149,108,42,13
     PUSHBUTTON      "See license",IDC_LICENCIA,10,162,85,15
     RTEXT           "If you don't have internet, please use magic.",IDC_STATIC,23,105,120,18
     ICON            IDR_MAINFRAME,IDC_STATIC,44,74,20,20
     CTEXT           "Use your finger to activate the program.",IDC_ACTIVADA,17,50,175,17
     ICON            IDR_MAINFRAME1,IDC_STATIC6,18,19,20,20
+    // Comment
 END
 
 MainMenu MENU
 {
     POPUP "&Debug"
     {
         MENUITEM "&Memory usage", ID_MEMORY
@@ -54,14 +55,19 @@
 msgid "License dialog"
 msgstr "Licenční dialog"
 
 #: DIALOGEX.IDD_REGGHC_DIALOG.CTEXT.IDC_STATIC1
 msgid "My very good program"
 msgstr "Mój bardzo dobry program"
 """
+POFILE_QUOTES = r"""
+#: DIALOGEX.IDD_REGGHC_DIALOG.CTEXT.IDC_STATIC1
+msgid "My very good program"
+msgstr "My \"good\" program"
+"""
 
 
 class TestPO2RCCommand(test_convert.TestConvertCommand):
     """Tests running actual po2rc commands on files"""
 
     convertmodule = po2rc
     defaultoptions = {"progress": "none"}
@@ -84,14 +90,28 @@
         )
         with self.open_testfile("output.rc") as handle:
             rc_result = rcfile(handle)
         assert len(rc_result.units) == 14
         assert rc_result.units[0].target == "Licenční dialog"
         assert rc_result.units[4].target == "Mój bardzo dobry program"
 
+    def test_convert_quotes(self):
+        """Tests the conversion to a po file"""
+        self.create_testfile("simple.rc", RC_SOURCE)
+        self.create_testfile("simple.po", POFILE_QUOTES)
+        self.run_command(
+            template="simple.rc", i="simple.po", o="output.rc", l="LANG_CZECH"
+        )
+        with self.open_testfile("output.rc") as handle:
+            print(handle.read())
+        with self.open_testfile("output.rc") as handle:
+            rc_result = rcfile(handle)
+        assert len(rc_result.units) == 14
+        assert rc_result.units[4].target == 'My "good" program'
+
     def test_convert_comment(self):
         self.create_testfile(
             "simple.rc",
             """
 STRINGTABLE
 BEGIN
     // IDS_COMMENTED        "Comment"
@@ -306,7 +326,73 @@
                 )
                 .splitlines()
             ]
         with self.open_testfile("output.rc") as handle:
             rc_result = rcfile(handle)
         assert len(rc_result.units) == 4
         assert rc_result.units[3].target == "Vypnout..."
+
+    def test_convert_newlines(self):
+        """Tests the conversion to a po file"""
+        source = """
+STRINGTABLE
+BEGIN
+ID_T_1 "Hello"
+END
+"""
+        expected = """
+STRINGTABLE
+BEGIN
+    ID_T_1                  "Ahoj"
+END
+"""
+        pofile = """
+#: STRINGTABLE.ID_T_1
+msgid "Hello"
+msgstr "Ahoj"
+"""
+        self.create_testfile("simple.rc", "\r\n".join(source.splitlines()))
+        self.create_testfile("simple.po", pofile)
+        self.run_command(
+            template="simple.rc", i="simple.po", o="output.rc", l="LANG_CZECH"
+        )
+        with self.open_testfile("output.rc", "rb") as handle:
+            content = handle.read()
+            assert content == "\r\n".join(expected.splitlines()).encode()
+
+        self.create_testfile("simple.rc", "\n".join(source.splitlines()))
+        self.create_testfile("simple.po", pofile)
+        self.run_command(
+            template="simple.rc", i="simple.po", o="output.rc", l="LANG_CZECH"
+        )
+        with self.open_testfile("output.rc", "rb") as handle:
+            content = handle.read()
+            assert content == "\n".join(expected.splitlines()).encode()
+
+    def test_convert_comment_after(self):
+        source = """
+STRINGTABLE
+BEGIN
+    ID_T_1 "Hello"
+    //   Comment
+END
+"""
+        expected = """
+STRINGTABLE
+BEGIN
+    ID_T_1                  "Ahoj"
+    //   Comment
+END
+"""
+        pofile = """
+#: STRINGTABLE.ID_T_1
+msgid "Hello"
+msgstr "Ahoj"
+"""
+        self.create_testfile("simple.rc", source)
+        self.create_testfile("simple.po", pofile)
+        self.run_command(
+            template="simple.rc", i="simple.po", o="output.rc", l="LANG_CZECH"
+        )
+        with self.open_testfile("output.rc", "rb") as handle:
+            content = handle.read()
+            assert content.decode() == expected
```

### Comparing `translate-toolkit-3.9.0/translate/convert/test_po2resx.py` & `translate-toolkit-3.9.1/translate/convert/test_po2resx.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/convert/test_po2sub.py` & `translate-toolkit-3.9.1/translate/convert/test_po2sub.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/convert/test_po2tiki.py` & `translate-toolkit-3.9.1/translate/convert/test_po2tiki.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/convert/test_po2tmx.py` & `translate-toolkit-3.9.1/translate/convert/test_po2tmx.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/convert/test_po2ts.py` & `translate-toolkit-3.9.1/translate/convert/test_po2ts.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/convert/test_po2txt.py` & `translate-toolkit-3.9.1/translate/convert/test_po2txt.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/convert/test_po2web2py.py` & `translate-toolkit-3.9.1/translate/convert/test_po2web2py.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/convert/test_po2xliff.py` & `translate-toolkit-3.9.1/translate/convert/test_po2xliff.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/convert/test_po2yaml.py` & `translate-toolkit-3.9.1/translate/convert/test_po2yaml.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/convert/test_pot2po.py` & `translate-toolkit-3.9.1/translate/convert/test_pot2po.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/convert/test_prop2mozfunny.py` & `translate-toolkit-3.9.1/translate/convert/test_prop2mozfunny.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/convert/test_prop2po.py` & `translate-toolkit-3.9.1/translate/convert/test_prop2po.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/convert/test_rc2po.py` & `translate-toolkit-3.9.1/translate/convert/test_rc2po.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/convert/test_resx2po.py` & `translate-toolkit-3.9.1/translate/convert/test_resx2po.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/convert/test_tiki2po.py` & `translate-toolkit-3.9.1/translate/convert/test_tiki2po.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/convert/test_ts2po.py` & `translate-toolkit-3.9.1/translate/convert/test_ts2po.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/convert/test_txt2po.py` & `translate-toolkit-3.9.1/translate/convert/test_txt2po.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/convert/test_web2py2po.py` & `translate-toolkit-3.9.1/translate/convert/test_web2py2po.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/convert/test_xliff2odf.py` & `translate-toolkit-3.9.1/translate/convert/test_xliff2odf.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/convert/test_xliff2po.py` & `translate-toolkit-3.9.1/translate/convert/test_xliff2po.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/convert/test_yaml2po.py` & `translate-toolkit-3.9.1/translate/convert/test_yaml2po.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/convert/tiki2po.py` & `translate-toolkit-3.9.1/translate/convert/tiki2po.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/convert/ts2po.py` & `translate-toolkit-3.9.1/translate/convert/ts2po.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/convert/txt2po.py` & `translate-toolkit-3.9.1/translate/convert/txt2po.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/convert/web2py2po.py` & `translate-toolkit-3.9.1/translate/convert/web2py2po.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/convert/xliff2odf.py` & `translate-toolkit-3.9.1/translate/convert/xliff2odf.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/convert/xliff2oo.py` & `translate-toolkit-3.9.1/translate/convert/xliff2oo.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/convert/xliff2po.py` & `translate-toolkit-3.9.1/translate/convert/xliff2po.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/convert/yaml2po.py` & `translate-toolkit-3.9.1/translate/convert/yaml2po.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/filters/__init__.py` & `translate-toolkit-3.9.1/translate/filters/__init__.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/filters/autocorrect.py` & `translate-toolkit-3.9.1/translate/filters/autocorrect.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/filters/checks.py` & `translate-toolkit-3.9.1/translate/filters/checks.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/filters/decoration.py` & `translate-toolkit-3.9.1/translate/filters/decoration.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/filters/decorators.py` & `translate-toolkit-3.9.1/translate/filters/decorators.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/filters/helpers.py` & `translate-toolkit-3.9.1/translate/filters/helpers.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/filters/pofilter.py` & `translate-toolkit-3.9.1/translate/filters/pofilter.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/filters/prefilters.py` & `translate-toolkit-3.9.1/translate/filters/prefilters.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/filters/spelling.py` & `translate-toolkit-3.9.1/translate/filters/spelling.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/filters/test_autocorrect.py` & `translate-toolkit-3.9.1/translate/filters/test_autocorrect.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/filters/test_checks.py` & `translate-toolkit-3.9.1/translate/filters/test_checks.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/filters/test_decoration.py` & `translate-toolkit-3.9.1/translate/filters/test_decoration.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/filters/test_pofilter.py` & `translate-toolkit-3.9.1/translate/filters/test_pofilter.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/filters/test_prefilters.py` & `translate-toolkit-3.9.1/translate/filters/test_prefilters.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/lang/__init__.py` & `translate-toolkit-3.9.1/translate/lang/__init__.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/lang/af.py` & `translate-toolkit-3.9.1/translate/lang/af.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/lang/ak.py` & `translate-toolkit-3.9.1/translate/lang/ak.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/lang/am.py` & `translate-toolkit-3.9.1/translate/lang/am.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/lang/ar.py` & `translate-toolkit-3.9.1/translate/lang/ar.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/lang/az.py` & `translate-toolkit-3.9.1/translate/lang/az.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/lang/bn.py` & `translate-toolkit-3.9.1/translate/lang/bn.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/lang/bo.py` & `translate-toolkit-3.9.1/translate/lang/bo.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/lang/code_as.py` & `translate-toolkit-3.9.1/translate/lang/code_as.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/lang/code_or.py` & `translate-toolkit-3.9.1/translate/lang/code_or.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/lang/common.py` & `translate-toolkit-3.9.1/translate/lang/common.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/lang/da.py` & `translate-toolkit-3.9.1/translate/lang/da.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/lang/data.py` & `translate-toolkit-3.9.1/translate/lang/data.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/lang/de.py` & `translate-toolkit-3.9.1/translate/lang/de.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/lang/dz.py` & `translate-toolkit-3.9.1/translate/lang/dz.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/lang/el.py` & `translate-toolkit-3.9.1/translate/lang/el.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/lang/es.py` & `translate-toolkit-3.9.1/translate/lang/es.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/lang/fa.py` & `translate-toolkit-3.9.1/translate/lang/fa.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/lang/factory.py` & `translate-toolkit-3.9.1/translate/lang/factory.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/lang/fi.py` & `translate-toolkit-3.9.1/translate/lang/fi.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/lang/fr.py` & `translate-toolkit-3.9.1/translate/lang/fr.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/lang/gd.py` & `translate-toolkit-3.9.1/translate/lang/gd.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/lang/gu.py` & `translate-toolkit-3.9.1/translate/lang/gu.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/lang/he.py` & `translate-toolkit-3.9.1/translate/lang/he.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/lang/hi.py` & `translate-toolkit-3.9.1/translate/lang/hi.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/lang/hy.py` & `translate-toolkit-3.9.1/translate/lang/hy.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/lang/identify.py` & `translate-toolkit-3.9.1/translate/lang/identify.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/lang/ja.py` & `translate-toolkit-3.9.1/translate/lang/ja.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/lang/km.py` & `translate-toolkit-3.9.1/translate/lang/km.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/lang/kn.py` & `translate-toolkit-3.9.1/translate/lang/kn.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/lang/ko.py` & `translate-toolkit-3.9.1/translate/lang/ko.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/lang/kw.py` & `translate-toolkit-3.9.1/translate/lang/kw.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/lang/lo.py` & `translate-toolkit-3.9.1/translate/lang/lo.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/lang/ml.py` & `translate-toolkit-3.9.1/translate/lang/ml.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/lang/mr.py` & `translate-toolkit-3.9.1/translate/lang/mr.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/lang/ms.py` & `translate-toolkit-3.9.1/translate/lang/ms.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/lang/my.py` & `translate-toolkit-3.9.1/translate/lang/my.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/lang/ne.py` & `translate-toolkit-3.9.1/translate/lang/ne.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/lang/ngram.py` & `translate-toolkit-3.9.1/translate/lang/ngram.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/lang/nqo.py` & `translate-toolkit-3.9.1/translate/lang/nqo.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/lang/nso.py` & `translate-toolkit-3.9.1/translate/lang/nso.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/lang/pa.py` & `translate-toolkit-3.9.1/translate/lang/pa.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/lang/pl.py` & `translate-toolkit-3.9.1/translate/lang/pl.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/lang/poedit.py` & `translate-toolkit-3.9.1/translate/lang/poedit.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/lang/pt_BR.py` & `translate-toolkit-3.9.1/translate/lang/pt_BR.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/lang/ro.py` & `translate-toolkit-3.9.1/translate/lang/ro.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/lang/scn.py` & `translate-toolkit-3.9.1/translate/lang/scn.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/lang/si.py` & `translate-toolkit-3.9.1/translate/lang/si.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/lang/son.py` & `translate-toolkit-3.9.1/translate/lang/son.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/lang/st.py` & `translate-toolkit-3.9.1/translate/lang/st.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/lang/su.py` & `translate-toolkit-3.9.1/translate/lang/su.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/lang/sv.py` & `translate-toolkit-3.9.1/translate/lang/sv.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/lang/ta.py` & `translate-toolkit-3.9.1/translate/lang/ta.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/lang/te.py` & `translate-toolkit-3.9.1/translate/lang/te.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/lang/team.py` & `translate-toolkit-3.9.1/translate/lang/team.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/lang/test-language-teams.sh` & `translate-toolkit-3.9.1/translate/lang/test-language-teams.sh`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/lang/test_af.py` & `translate-toolkit-3.9.1/translate/lang/test_af.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/lang/test_am.py` & `translate-toolkit-3.9.1/translate/lang/test_am.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/lang/test_ar.py` & `translate-toolkit-3.9.1/translate/lang/test_ar.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/lang/test_common.py` & `translate-toolkit-3.9.1/translate/lang/test_common.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/lang/test_data.py` & `translate-toolkit-3.9.1/translate/lang/test_data.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/lang/test_el.py` & `translate-toolkit-3.9.1/translate/lang/test_el.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/lang/test_es.py` & `translate-toolkit-3.9.1/translate/lang/test_es.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/lang/test_fa.py` & `translate-toolkit-3.9.1/translate/lang/test_fa.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/lang/test_factory.py` & `translate-toolkit-3.9.1/translate/lang/test_factory.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/lang/test_fr.py` & `translate-toolkit-3.9.1/translate/lang/test_fr.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/lang/test_hy.py` & `translate-toolkit-3.9.1/translate/lang/test_hy.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/lang/test_identify.py` & `translate-toolkit-3.9.1/translate/lang/test_identify.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/lang/test_ja.py` & `translate-toolkit-3.9.1/translate/lang/test_ja.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/lang/test_km.py` & `translate-toolkit-3.9.1/translate/lang/test_km.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/lang/test_ko.py` & `translate-toolkit-3.9.1/translate/lang/test_ko.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/lang/test_ne.py` & `translate-toolkit-3.9.1/translate/lang/test_ne.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/lang/test_nqo.py` & `translate-toolkit-3.9.1/translate/lang/test_nqo.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/lang/test_or.py` & `translate-toolkit-3.9.1/translate/lang/test_or.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/lang/test_poedit.py` & `translate-toolkit-3.9.1/translate/lang/test_poedit.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/lang/test_ro.py` & `translate-toolkit-3.9.1/translate/lang/test_ro.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/lang/test_scn.py` & `translate-toolkit-3.9.1/translate/lang/test_scn.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/lang/test_team.py` & `translate-toolkit-3.9.1/translate/lang/test_team.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/lang/test_th.py` & `translate-toolkit-3.9.1/translate/lang/test_th.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/lang/test_vi.py` & `translate-toolkit-3.9.1/translate/lang/test_vi.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/lang/test_zh.py` & `translate-toolkit-3.9.1/translate/lang/test_zh.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/lang/th.py` & `translate-toolkit-3.9.1/translate/lang/th.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/lang/tr.py` & `translate-toolkit-3.9.1/translate/lang/tr.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/lang/ug.py` & `translate-toolkit-3.9.1/translate/lang/ug.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/lang/ur.py` & `translate-toolkit-3.9.1/translate/lang/ur.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/lang/ve.py` & `translate-toolkit-3.9.1/translate/lang/ve.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/lang/vi.py` & `translate-toolkit-3.9.1/translate/lang/vi.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/lang/wo.py` & `translate-toolkit-3.9.1/translate/lang/wo.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/lang/zh.py` & `translate-toolkit-3.9.1/translate/lang/zh.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/lang/zh_cn.py` & `translate-toolkit-3.9.1/translate/lang/zh_cn.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/lang/zh_hk.py` & `translate-toolkit-3.9.1/translate/lang/zh_hk.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/lang/zh_tw.py` & `translate-toolkit-3.9.1/translate/lang/zh_tw.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/misc/__init__.py` & `translate-toolkit-3.9.1/translate/misc/__init__.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/misc/deprecation.py` & `translate-toolkit-3.9.1/translate/misc/deprecation.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/misc/dictutils.py` & `translate-toolkit-3.9.1/translate/misc/dictutils.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/misc/file_discovery.py` & `translate-toolkit-3.9.1/translate/misc/file_discovery.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/misc/multistring.py` & `translate-toolkit-3.9.1/translate/misc/multistring.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/misc/optrecurse.py` & `translate-toolkit-3.9.1/translate/misc/optrecurse.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/misc/ourdom.py` & `translate-toolkit-3.9.1/translate/misc/ourdom.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/misc/progressbar.py` & `translate-toolkit-3.9.1/translate/misc/progressbar.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/misc/quote.py` & `translate-toolkit-3.9.1/translate/misc/quote.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/misc/selector.py` & `translate-toolkit-3.9.1/translate/misc/selector.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/misc/test_multistring.py` & `translate-toolkit-3.9.1/translate/misc/test_multistring.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/misc/test_optrecurse.py` & `translate-toolkit-3.9.1/translate/misc/test_optrecurse.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/misc/test_quote.py` & `translate-toolkit-3.9.1/translate/misc/test_quote.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/misc/test_xml_helpers.py` & `translate-toolkit-3.9.1/translate/misc/test_xml_helpers.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/misc/wStringIO.py` & `translate-toolkit-3.9.1/translate/misc/wStringIO.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/misc/wsgi.py` & `translate-toolkit-3.9.1/translate/misc/wsgi.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/misc/xml_helpers.py` & `translate-toolkit-3.9.1/translate/misc/xml_helpers.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/search/__init__.py` & `translate-toolkit-3.9.1/translate/search/__init__.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/search/lshtein.py` & `translate-toolkit-3.9.1/translate/search/lshtein.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/search/match.py` & `translate-toolkit-3.9.1/translate/search/match.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/search/terminology.py` & `translate-toolkit-3.9.1/translate/search/terminology.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/search/test_lshtein.py` & `translate-toolkit-3.9.1/translate/search/test_lshtein.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/search/test_match.py` & `translate-toolkit-3.9.1/translate/search/test_match.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/services/__init__.py` & `translate-toolkit-3.9.1/translate/services/__init__.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/services/test_tmserver.py` & `translate-toolkit-3.9.1/translate/services/test_tmserver.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/services/tmserver.py` & `translate-toolkit-3.9.1/translate/services/tmserver.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/share/langmodels/Ndebele.lm` & `translate-toolkit-3.9.1/translate/share/langmodels/Ndebele.lm`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/share/langmodels/NorthernSotho.lm` & `translate-toolkit-3.9.1/translate/share/langmodels/NorthernSotho.lm`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/share/langmodels/README` & `translate-toolkit-3.9.1/translate/share/langmodels/README`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/share/langmodels/Sotho.lm` & `translate-toolkit-3.9.1/translate/share/langmodels/Sotho.lm`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/share/langmodels/Swati.lm` & `translate-toolkit-3.9.1/translate/share/langmodels/Swati.lm`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/share/langmodels/Tsonga.lm` & `translate-toolkit-3.9.1/translate/share/langmodels/Tsonga.lm`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/share/langmodels/Tswana.lm` & `translate-toolkit-3.9.1/translate/share/langmodels/Tswana.lm`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/share/langmodels/Venda.lm` & `translate-toolkit-3.9.1/translate/share/langmodels/Venda.lm`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/share/langmodels/Xhosa.lm` & `translate-toolkit-3.9.1/translate/share/langmodels/Xhosa.lm`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/share/langmodels/Zulu.lm` & `translate-toolkit-3.9.1/translate/share/langmodels/Zulu.lm`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/share/langmodels/afrikaans.lm` & `translate-toolkit-3.9.1/translate/share/langmodels/afrikaans.lm`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/share/langmodels/albanian.lm` & `translate-toolkit-3.9.1/translate/share/langmodels/albanian.lm`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/share/langmodels/arabic.lm` & `translate-toolkit-3.9.1/translate/share/langmodels/arabic.lm`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/share/langmodels/basque.lm` & `translate-toolkit-3.9.1/translate/share/langmodels/basque.lm`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/share/langmodels/belarus.lm` & `translate-toolkit-3.9.1/translate/share/langmodels/belarus.lm`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/share/langmodels/bosnian.lm` & `translate-toolkit-3.9.1/translate/share/langmodels/bosnian.lm`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/share/langmodels/breton.lm` & `translate-toolkit-3.9.1/translate/share/langmodels/breton.lm`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/share/langmodels/catalan.lm` & `translate-toolkit-3.9.1/translate/share/langmodels/catalan.lm`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/share/langmodels/chinese_simplified.lm` & `translate-toolkit-3.9.1/translate/share/langmodels/chinese_simplified.lm`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/share/langmodels/chinese_traditional.lm` & `translate-toolkit-3.9.1/translate/share/langmodels/chinese_traditional.lm`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/share/langmodels/croatian.lm` & `translate-toolkit-3.9.1/translate/share/langmodels/croatian.lm`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/share/langmodels/czech.lm` & `translate-toolkit-3.9.1/translate/share/langmodels/czech.lm`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/share/langmodels/danish.lm` & `translate-toolkit-3.9.1/translate/share/langmodels/danish.lm`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/share/langmodels/dutch.lm` & `translate-toolkit-3.9.1/translate/share/langmodels/dutch.lm`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/share/langmodels/english.lm` & `translate-toolkit-3.9.1/translate/share/langmodels/english.lm`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/share/langmodels/esperanto.lm` & `translate-toolkit-3.9.1/translate/share/langmodels/esperanto.lm`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/share/langmodels/estonian.lm` & `translate-toolkit-3.9.1/translate/share/langmodels/estonian.lm`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/share/langmodels/finnish.lm` & `translate-toolkit-3.9.1/translate/share/langmodels/finnish.lm`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/share/langmodels/fpdb.conf` & `translate-toolkit-3.9.1/translate/share/langmodels/fpdb.conf`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/share/langmodels/french.lm` & `translate-toolkit-3.9.1/translate/share/langmodels/french.lm`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/share/langmodels/frisian.lm` & `translate-toolkit-3.9.1/translate/share/langmodels/frisian.lm`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/share/langmodels/german.lm` & `translate-toolkit-3.9.1/translate/share/langmodels/german.lm`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/share/langmodels/greek.lm` & `translate-toolkit-3.9.1/translate/share/langmodels/greek.lm`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/share/langmodels/hebrew.lm` & `translate-toolkit-3.9.1/translate/share/langmodels/hebrew.lm`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/share/langmodels/hungarian.lm` & `translate-toolkit-3.9.1/translate/share/langmodels/hungarian.lm`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/share/langmodels/icelandic.lm` & `translate-toolkit-3.9.1/translate/share/langmodels/icelandic.lm`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/share/langmodels/indonesian.lm` & `translate-toolkit-3.9.1/translate/share/langmodels/indonesian.lm`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/share/langmodels/irish_gaelic.lm` & `translate-toolkit-3.9.1/translate/share/langmodels/irish_gaelic.lm`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/share/langmodels/italian.lm` & `translate-toolkit-3.9.1/translate/share/langmodels/italian.lm`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/share/langmodels/japanese.lm` & `translate-toolkit-3.9.1/translate/share/langmodels/japanese.lm`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/share/langmodels/latin.lm` & `translate-toolkit-3.9.1/translate/share/langmodels/latin.lm`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/share/langmodels/latvian.lm` & `translate-toolkit-3.9.1/translate/share/langmodels/latvian.lm`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/share/langmodels/lithuanian.lm` & `translate-toolkit-3.9.1/translate/share/langmodels/lithuanian.lm`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/share/langmodels/malay.lm` & `translate-toolkit-3.9.1/translate/share/langmodels/malay.lm`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/share/langmodels/manx_gaelic.lm` & `translate-toolkit-3.9.1/translate/share/langmodels/manx_gaelic.lm`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/share/langmodels/norwegian.lm` & `translate-toolkit-3.9.1/translate/share/langmodels/norwegian.lm`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/share/langmodels/polish.lm` & `translate-toolkit-3.9.1/translate/share/langmodels/polish.lm`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/share/langmodels/portuguese.lm` & `translate-toolkit-3.9.1/translate/share/langmodels/portuguese.lm`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/share/langmodels/quechua.lm` & `translate-toolkit-3.9.1/translate/share/langmodels/quechua.lm`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/share/langmodels/romanian.lm` & `translate-toolkit-3.9.1/translate/share/langmodels/romanian.lm`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/share/langmodels/romansh.lm` & `translate-toolkit-3.9.1/translate/share/langmodels/romansh.lm`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/share/langmodels/russian.lm` & `translate-toolkit-3.9.1/translate/share/langmodels/russian.lm`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/share/langmodels/scots.lm` & `translate-toolkit-3.9.1/translate/share/langmodels/scots.lm`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/share/langmodels/scots_gaelic.lm` & `translate-toolkit-3.9.1/translate/share/langmodels/scots_gaelic.lm`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/share/langmodels/serbian_ascii.lm` & `translate-toolkit-3.9.1/translate/share/langmodels/serbian_ascii.lm`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/share/langmodels/slovak_ascii.lm` & `translate-toolkit-3.9.1/translate/share/langmodels/slovak_ascii.lm`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/share/langmodels/slovenian.lm` & `translate-toolkit-3.9.1/translate/share/langmodels/slovenian.lm`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/share/langmodels/spanish.lm` & `translate-toolkit-3.9.1/translate/share/langmodels/spanish.lm`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/share/langmodels/swahili.lm` & `translate-toolkit-3.9.1/translate/share/langmodels/swahili.lm`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/share/langmodels/swedish.lm` & `translate-toolkit-3.9.1/translate/share/langmodels/swedish.lm`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/share/langmodels/tagalog.lm` & `translate-toolkit-3.9.1/translate/share/langmodels/tagalog.lm`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/share/langmodels/turkish.lm` & `translate-toolkit-3.9.1/translate/share/langmodels/turkish.lm`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/share/langmodels/ukrainian.lm` & `translate-toolkit-3.9.1/translate/share/langmodels/ukrainian.lm`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/share/langmodels/vietnamese.lm` & `translate-toolkit-3.9.1/translate/share/langmodels/vietnamese.lm`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/share/langmodels/welsh.lm` & `translate-toolkit-3.9.1/translate/share/langmodels/welsh.lm`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/share/stoplist-en` & `translate-toolkit-3.9.1/translate/share/stoplist-en`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/storage/__init__.py` & `translate-toolkit-3.9.1/translate/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/storage/_factory_classes.py` & `translate-toolkit-3.9.1/translate/storage/_factory_classes.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/storage/aresource.py` & `translate-toolkit-3.9.1/translate/storage/aresource.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/storage/base.py` & `translate-toolkit-3.9.1/translate/storage/base.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/storage/benchmark.py` & `translate-toolkit-3.9.1/translate/storage/benchmark.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/storage/bundleprojstore.py` & `translate-toolkit-3.9.1/translate/storage/bundleprojstore.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/storage/catkeys.py` & `translate-toolkit-3.9.1/translate/storage/catkeys.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/storage/cpo.py` & `translate-toolkit-3.9.1/translate/storage/cpo.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/storage/csvl10n.py` & `translate-toolkit-3.9.1/translate/storage/csvl10n.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/storage/directory.py` & `translate-toolkit-3.9.1/translate/storage/directory.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/storage/dtd.py` & `translate-toolkit-3.9.1/translate/storage/dtd.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/storage/factory.py` & `translate-toolkit-3.9.1/translate/storage/factory.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/storage/flatxml.py` & `translate-toolkit-3.9.1/translate/storage/flatxml.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/storage/fluent.py` & `translate-toolkit-3.9.1/translate/storage/fluent.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/storage/fpo.py` & `translate-toolkit-3.9.1/translate/storage/fpo.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/storage/html.py` & `translate-toolkit-3.9.1/translate/storage/html.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/storage/ical.py` & `translate-toolkit-3.9.1/translate/storage/ical.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/storage/idml.py` & `translate-toolkit-3.9.1/translate/storage/idml.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/storage/ini.py` & `translate-toolkit-3.9.1/translate/storage/ini.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/storage/jsonl10n.py` & `translate-toolkit-3.9.1/translate/storage/jsonl10n.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/storage/lisa.py` & `translate-toolkit-3.9.1/translate/storage/lisa.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/storage/mo.py` & `translate-toolkit-3.9.1/translate/storage/mo.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/storage/mozilla_lang.py` & `translate-toolkit-3.9.1/translate/storage/mozilla_lang.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/storage/odf_io.py` & `translate-toolkit-3.9.1/translate/storage/odf_io.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/storage/odf_shared.py` & `translate-toolkit-3.9.1/translate/storage/odf_shared.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/storage/omegat.py` & `translate-toolkit-3.9.1/translate/storage/omegat.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/storage/oo.py` & `translate-toolkit-3.9.1/translate/storage/oo.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/storage/php.py` & `translate-toolkit-3.9.1/translate/storage/php.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/storage/placeables/__init__.py` & `translate-toolkit-3.9.1/translate/storage/placeables/__init__.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/storage/placeables/base.py` & `translate-toolkit-3.9.1/translate/storage/placeables/base.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/storage/placeables/general.py` & `translate-toolkit-3.9.1/translate/storage/placeables/general.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/storage/placeables/interfaces.py` & `translate-toolkit-3.9.1/translate/storage/placeables/interfaces.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/storage/placeables/lisa.py` & `translate-toolkit-3.9.1/translate/storage/placeables/lisa.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/storage/placeables/parse.py` & `translate-toolkit-3.9.1/translate/storage/placeables/parse.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/storage/placeables/strelem.py` & `translate-toolkit-3.9.1/translate/storage/placeables/strelem.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/storage/placeables/terminology.py` & `translate-toolkit-3.9.1/translate/storage/placeables/terminology.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/storage/placeables/test_base.py` & `translate-toolkit-3.9.1/translate/storage/placeables/test_base.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/storage/placeables/test_general.py` & `translate-toolkit-3.9.1/translate/storage/placeables/test_general.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/storage/placeables/test_lisa.py` & `translate-toolkit-3.9.1/translate/storage/placeables/test_lisa.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/storage/placeables/test_terminology.py` & `translate-toolkit-3.9.1/translate/storage/placeables/test_terminology.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/storage/placeables/xliff.py` & `translate-toolkit-3.9.1/translate/storage/placeables/xliff.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/storage/po.py` & `translate-toolkit-3.9.1/translate/storage/po.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/storage/pocommon.py` & `translate-toolkit-3.9.1/translate/storage/pocommon.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/storage/poheader.py` & `translate-toolkit-3.9.1/translate/storage/poheader.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/storage/poparser.py` & `translate-toolkit-3.9.1/translate/storage/poparser.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/storage/poxliff.py` & `translate-toolkit-3.9.1/translate/storage/poxliff.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/storage/project.py` & `translate-toolkit-3.9.1/translate/storage/project.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/storage/projstore.py` & `translate-toolkit-3.9.1/translate/storage/projstore.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/storage/properties.java` & `translate-toolkit-3.9.1/translate/storage/properties.java`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/storage/properties.py` & `translate-toolkit-3.9.1/translate/storage/properties.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/storage/pypo.py` & `translate-toolkit-3.9.1/translate/storage/pypo.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/storage/qm.py` & `translate-toolkit-3.9.1/translate/storage/qm.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/storage/qph.py` & `translate-toolkit-3.9.1/translate/storage/qph.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/storage/rc.py` & `translate-toolkit-3.9.1/translate/storage/rc.py`

 * *Files 8% similar despite different names*

```diff
@@ -48,28 +48,24 @@
 )
 from pyparsing.common import pyparsing_common
 
 from translate.storage import base
 
 
 def escape_to_python(string):
-    """Escape a given .rc string into a valid Python string."""
-    pystring = re.sub('"\\s*\\\\\n\\s*"', "", string)  # xxx"\n"xxx line continuation
-    pystring = re.sub("\\\\\\\n", "", pystring)  # backslash newline line continuation
-    pystring = re.sub(
-        "\\\\n", "\n", pystring
-    )  # Convert escaped newline to a real newline
-    pystring = re.sub(
-        "\\\\r", "\r", pystring
-    )  # Convert escaped carriage-return to a real carriage-return
-    pystring = re.sub("\\\\t", "\t", pystring)  # Convert escape tab to a real tab
-    pystring = re.sub(
-        "\\\\\\\\", "\\\\", pystring
-    )  # Convert escape backslash to a real escaped backslash
-    return pystring
+    """Unescape a given .rc string into a valid Python string."""
+    return (
+        re.sub('"\\s*\\\\\n\\s*"', "", string)  # xxx"\n"xxx line continuation
+        .replace("\\\n", "")  # backslash newline line continuation
+        .replace(r"\r", "\r")
+        .replace(r"\n", "\n")
+        .replace(r"\t", "\t")
+        .replace(r"\\", "\\")
+        .replace('""', '"')
+    )
 
 
 def extract_text(values):
     result = []
     for value in values:
         if isinstance(value, str) and value.startswith('"'):
             result.append(escape_to_python(value[1:-1]))
@@ -88,19 +84,21 @@
             break
 
     return "UNKNOWN_ID"
 
 
 def escape_to_rc(string):
     """Escape a given Python string into a valid .rc string."""
-    rcstring = re.sub("\\\\", "\\\\\\\\", string)
-    rcstring = re.sub("\t", "\\\\t", rcstring)
-    rcstring = re.sub("\n", "\\\\n", rcstring)
-    rcstring = re.sub("\r", "\\\\r", rcstring)
-    return rcstring
+    return (
+        string.replace("\\", r"\\")
+        .replace("\t", r"\t")
+        .replace("\n", r"\n")
+        .replace("\r", r"\r")
+        .replace('"', '""')
+    )
 
 
 class rcunit(base.TranslationUnit):
     """A unit of an rc file"""
 
     def __init__(self, source="", **kwargs):
         """Construct a blank rcunit."""
@@ -162,15 +160,15 @@
 def rc_statement():
     """
     Generate a RC statement parser that can be used to parse a RC file
 
     :rtype: pyparsing.ParserElement
     """
 
-    one_line_comment = "//" + rest_of_line
+    one_line_comment = Combine("//" + rest_of_line)
 
     comments = c_style_comment ^ one_line_comment
 
     precompiler = AtLineStart(Word("#", alphanums) + rest_of_line)
 
     language_definition = (
         "LANGUAGE"
@@ -325,14 +323,15 @@
         self, inputfile=None, lang=None, sublang=None, encoding=None, **kwargs
     ):
         """Construct an rcfile, optionally reading in from inputfile."""
         super().__init__(encoding=encoding, **kwargs)
         self.filename = getattr(inputfile, "name", "")
         self.lang = lang
         self.sublang = sublang
+        self.newline = "\r\n"
         if inputfile is not None:
             rcsrc = inputfile.read()
             inputfile.close()
             self.parse(
                 rcsrc,
                 encoding=encoding or "auto",
             )
@@ -374,14 +373,22 @@
             self.encoding = "utf-16-le"
             decoded = rcsrc.decode(self.encoding)
         else:
             decoded, self.encoding = self.detect_encoding(
                 rcsrc, default_encodings=[self.default_encoding]
             )
 
+        # Extract first newline
+        for line in decoded.splitlines(True):
+            if len(line) >= 2 and line[-2] in ("\r", "\n"):
+                self.newline = line[-2:]
+            else:
+                self.newline = line[-1]
+            break
+
         decoded = decoded.replace("\r", "")
 
         # Parse the strings into a structure.
         results = rc_statement().search_string(decoded)
 
         processblocks = True
```

### Comparing `translate-toolkit-3.9.0/translate/storage/resourcedictionary.py` & `translate-toolkit-3.9.1/translate/storage/resourcedictionary.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/storage/resx.py` & `translate-toolkit-3.9.1/translate/storage/resx.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/storage/statistics.py` & `translate-toolkit-3.9.1/translate/storage/statistics.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/storage/stringsdict.py` & `translate-toolkit-3.9.1/translate/storage/stringsdict.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/storage/subtitles.py` & `translate-toolkit-3.9.1/translate/storage/subtitles.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/storage/symbian.py` & `translate-toolkit-3.9.1/translate/storage/symbian.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/storage/tbx.py` & `translate-toolkit-3.9.1/translate/storage/tbx.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/storage/test_aresource.py` & `translate-toolkit-3.9.1/translate/storage/test_aresource.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/storage/test_base.py` & `translate-toolkit-3.9.1/translate/storage/test_base.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/storage/test_catkeys.py` & `translate-toolkit-3.9.1/translate/storage/test_catkeys.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/storage/test_cpo.py` & `translate-toolkit-3.9.1/translate/storage/test_cpo.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/storage/test_csvl10n.py` & `translate-toolkit-3.9.1/translate/storage/test_csvl10n.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/storage/test_directory.py` & `translate-toolkit-3.9.1/translate/storage/test_directory.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/storage/test_dtd.py` & `translate-toolkit-3.9.1/translate/storage/test_dtd.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/storage/test_factory.py` & `translate-toolkit-3.9.1/translate/storage/test_factory.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/storage/test_flatxml.py` & `translate-toolkit-3.9.1/translate/storage/test_flatxml.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/storage/test_fluent.py` & `translate-toolkit-3.9.1/translate/storage/test_fluent.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/storage/test_html.py` & `translate-toolkit-3.9.1/translate/storage/test_html.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/storage/test_jsonl10n.py` & `translate-toolkit-3.9.1/translate/storage/test_jsonl10n.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/storage/test_mo.py` & `translate-toolkit-3.9.1/translate/storage/test_mo.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/storage/test_monolingual.py` & `translate-toolkit-3.9.1/translate/storage/test_monolingual.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/storage/test_mozilla_lang.py` & `translate-toolkit-3.9.1/translate/storage/test_mozilla_lang.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/storage/test_oo.py` & `translate-toolkit-3.9.1/translate/storage/test_oo.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/storage/test_php.py` & `translate-toolkit-3.9.1/translate/storage/test_php.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/storage/test_po.py` & `translate-toolkit-3.9.1/translate/storage/test_po.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/storage/test_pocommon.py` & `translate-toolkit-3.9.1/translate/storage/test_pocommon.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/storage/test_poheader.py` & `translate-toolkit-3.9.1/translate/storage/test_poheader.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/storage/test_poxliff.py` & `translate-toolkit-3.9.1/translate/storage/test_poxliff.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/storage/test_properties.py` & `translate-toolkit-3.9.1/translate/storage/test_properties.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/storage/test_pypo.py` & `translate-toolkit-3.9.1/translate/storage/test_pypo.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/storage/test_qm.py` & `translate-toolkit-3.9.1/translate/storage/test_qm.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/storage/test_qph.py` & `translate-toolkit-3.9.1/translate/storage/test_qph.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/storage/test_rc.py` & `translate-toolkit-3.9.1/translate/storage/test_rc.py`

 * *Files 3% similar despite different names*

```diff
@@ -597,7 +597,21 @@
         assert rc_file.units[1].name == "MENU.1.MENUITEM.2"
         assert rc_file.units[2].source == "This is a dialog."
         assert rc_file.units[2].name == "DIALOGEX.3.CAPTION"
         assert rc_file.units[3].source == "This is a button."
         assert rc_file.units[3].name == "DIALOGEX.3.CONTROL.4"
         assert rc_file.units[4].source == "This is a string."
         assert rc_file.units[4].name == "STRINGTABLE.5"
+
+    def test_quotes(self):
+        rc_source = """
+STRINGTABLE
+BEGIN
+IDS_TEST_123     "The timestamp for ""ABCDEF"" could not be read."
+END
+"""
+        rc_file = self.source_parse(rc_source)
+        assert len(rc_file.units) == 1
+        assert rc_file.units[0].name == "STRINGTABLE.IDS_TEST_123"
+        assert (
+            rc_file.units[0].source == 'The timestamp for "ABCDEF" could not be read.'
+        )
```

### Comparing `translate-toolkit-3.9.0/translate/storage/test_resourcedictionary.py` & `translate-toolkit-3.9.1/translate/storage/test_resourcedictionary.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/storage/test_resx.py` & `translate-toolkit-3.9.1/translate/storage/test_resx.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/storage/test_stringsdict.py` & `translate-toolkit-3.9.1/translate/storage/test_stringsdict.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/storage/test_subtitles.py` & `translate-toolkit-3.9.1/translate/storage/test_subtitles.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/storage/test_tbx.py` & `translate-toolkit-3.9.1/translate/storage/test_tbx.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/storage/test_tiki.py` & `translate-toolkit-3.9.1/translate/storage/test_tiki.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/storage/test_tmx.py` & `translate-toolkit-3.9.1/translate/storage/test_tmx.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/storage/test_trados.py` & `translate-toolkit-3.9.1/translate/storage/test_trados.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/storage/test_ts2.py` & `translate-toolkit-3.9.1/translate/storage/test_ts2.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/storage/test_txt.py` & `translate-toolkit-3.9.1/translate/storage/test_txt.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/storage/test_wordfast.py` & `translate-toolkit-3.9.1/translate/storage/test_wordfast.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/storage/test_xliff.py` & `translate-toolkit-3.9.1/translate/storage/test_xliff.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/storage/test_yaml.py` & `translate-toolkit-3.9.1/translate/storage/test_yaml.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/storage/test_zip.py` & `translate-toolkit-3.9.1/translate/storage/test_zip.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/storage/tiki.py` & `translate-toolkit-3.9.1/translate/storage/tiki.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/storage/tmdb.py` & `translate-toolkit-3.9.1/translate/storage/tmdb.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/storage/tmx.py` & `translate-toolkit-3.9.1/translate/storage/tmx.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/storage/trados.py` & `translate-toolkit-3.9.1/translate/storage/trados.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/storage/ts.py` & `translate-toolkit-3.9.1/translate/storage/ts.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/storage/ts2.py` & `translate-toolkit-3.9.1/translate/storage/ts2.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/storage/txt.py` & `translate-toolkit-3.9.1/translate/storage/txt.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/storage/utx.py` & `translate-toolkit-3.9.1/translate/storage/utx.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/storage/wordfast.py` & `translate-toolkit-3.9.1/translate/storage/wordfast.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/storage/workflow.py` & `translate-toolkit-3.9.1/translate/storage/workflow.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/storage/xliff.py` & `translate-toolkit-3.9.1/translate/storage/xliff.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/storage/xml_extract/__init__.py` & `translate-toolkit-3.9.1/translate/storage/xml_extract/__init__.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/storage/xml_extract/extract.py` & `translate-toolkit-3.9.1/translate/storage/xml_extract/extract.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/storage/xml_extract/generate.py` & `translate-toolkit-3.9.1/translate/storage/xml_extract/generate.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/storage/xml_extract/misc.py` & `translate-toolkit-3.9.1/translate/storage/xml_extract/misc.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/storage/xml_extract/test_misc.py` & `translate-toolkit-3.9.1/translate/storage/xml_extract/test_misc.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/storage/xml_extract/test_unit_tree.py` & `translate-toolkit-3.9.1/translate/storage/xml_extract/test_unit_tree.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/storage/xml_extract/test_xpath_breadcrumb.py` & `translate-toolkit-3.9.1/translate/storage/xml_extract/test_xpath_breadcrumb.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/storage/xml_extract/unit_tree.py` & `translate-toolkit-3.9.1/translate/storage/xml_extract/unit_tree.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/storage/xml_extract/xpath_breadcrumb.py` & `translate-toolkit-3.9.1/translate/storage/xml_extract/xpath_breadcrumb.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/storage/xml_name.py` & `translate-toolkit-3.9.1/translate/storage/xml_name.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/storage/yaml.py` & `translate-toolkit-3.9.1/translate/storage/yaml.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/storage/zip.py` & `translate-toolkit-3.9.1/translate/storage/zip.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/tools/__init__.py` & `translate-toolkit-3.9.1/translate/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/tools/__snapshots__/test_junitmsgfmt.ambr` & `translate-toolkit-3.9.1/translate/tools/__snapshots__/test_junitmsgfmt.ambr`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/tools/__snapshots__/test_pocount.ambr` & `translate-toolkit-3.9.1/translate/tools/__snapshots__/test_pocount.ambr`

 * *Files 25% similar despite different names*

```diff
@@ -1,8 +1,89 @@
 # serializer version: 1
+# name: test_cases[po-file-csv]
+  CaptureResult(
+    err='',
+    out='''
+      Filename,Translated Messages,Translated Source Words,Translated Target Words,Fuzzy Messages,Fuzzy Source Words,Untranslated Messages,Untranslated Source Words,Total Message,Total Source Words,Review Messages,Review Source Words
+      tests/cli/data/test_pocount_po_csv/one.po,1,3,3,0,0,0,0,1,3,0,0
+  
+    ''',
+  )
+# ---
+# name: test_cases[po-file-fuzzy]
+  CaptureResult(
+    err='',
+    out='''
+      Processing file : tests/cli/data/test_pocount_po_fuzzy/one.po
+      Type               Strings      Words (source)    Words (translation)
+      Translated:       1 ( 50%)          2 ( 50%)               3
+      Fuzzy:            1 ( 50%)          2 ( 50%)             n/a
+      Untranslated:     0 (  0%)          0 (  0%)             n/a
+      Total:            2                 4                      3
+      
+      Unreviewed:       1 ( 50%)          2 ( 50%)               3
+      Needs-Work:       1 ( 50%)          2 ( 50%)               0
+      
+  
+    ''',
+  )
+# ---
+# name: test_cases[po-file]
+  CaptureResult(
+    err='',
+    out='''
+      Processing file : tests/cli/data/test_pocount_po_file/one.po
+      Type               Strings      Words (source)    Words (translation)
+      Translated:       1 (100%)          3 (100%)               3
+      Fuzzy:            0 (  0%)          0 (  0%)             n/a
+      Untranslated:     0 (  0%)          0 (  0%)             n/a
+      Total:            1                 3                      3
+      
+      Unreviewed:       1 (100%)          3 (100%)               3
+      
+  
+    ''',
+  )
+# ---
+# name: test_cases[xliff-states-no]
+  CaptureResult(
+    err='',
+    out='''
+      Processing file : tests/cli/data/test_pocount_xliff_states_no/states.xlf
+      Type               Strings      Words (source)    Words (translation)
+      Translated:       0 (  0%)          0 (  0%)               0
+      Fuzzy:            8 (100%)          8 (100%)             n/a
+      Untranslated:     0 (  0%)          0 (  0%)             n/a
+      Total:            8                 8                      0
+      
+      Needs-Work:       6 ( 75%)          6 ( 75%)               0
+      Unreviewed:       2 ( 25%)          2 ( 25%)               0
+      
+  
+    ''',
+  )
+# ---
+# name: test_cases[xliff-states-yes]
+  CaptureResult(
+    err='',
+    out='''
+      Processing file : tests/cli/data/test_pocount_xliff_states_yes/states.xlf
+      Type               Strings      Words (source)    Words (translation)
+      Translated:       8 (100%)          8 (100%)               8
+      Fuzzy:            0 (  0%)          0 (  0%)             n/a
+      Untranslated:     0 (  0%)          0 (  0%)             n/a
+      Total:            8                 8                      8
+      
+      Unreviewed:       7 ( 87%)          7 ( 87%)               7
+      Final:            1 ( 12%)          1 ( 12%)               1
+      
+  
+    ''',
+  )
+# ---
 # name: test_output[no-color=False-incomplete=False-csv]
   '''
   Filename,Translated Messages,Translated Source Words,Translated Target Words,Fuzzy Messages,Fuzzy Source Words,Untranslated Messages,Untranslated Source Words,Total Message,Total Source Words,Review Messages,Review Source Words
   tests/cli/data/test_pocount_po_csv/one.po,1,3,3,0,0,0,0,1,3,0,0
   tests/cli/data/test_pocount_po_file/one.po,1,3,3,0,0,0,0,1,3,0,0
   tests/cli/data/test_pocount_po_fuzzy/one.po,1,2,3,1,2,0,0,2,4,0,0
```

### Comparing `translate-toolkit-3.9.0/translate/tools/build_tmdb.py` & `translate-toolkit-3.9.1/translate/tools/build_tmdb.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/tools/junitmsgfmt.py` & `translate-toolkit-3.9.1/translate/tools/junitmsgfmt.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/tools/phppo2pypo.py` & `translate-toolkit-3.9.1/translate/tools/phppo2pypo.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/tools/poclean.py` & `translate-toolkit-3.9.1/translate/tools/poclean.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/tools/pocompile.py` & `translate-toolkit-3.9.1/translate/tools/pocompile.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/tools/poconflicts.py` & `translate-toolkit-3.9.1/translate/tools/poconflicts.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/tools/pocount.py` & `translate-toolkit-3.9.1/translate/tools/pocount.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,27 +30,22 @@
 import logging
 import os
 import re
 import sys
 from argparse import ArgumentParser
 from collections import defaultdict
 from dataclasses import dataclass
+from functools import cached_property
 from operator import itemgetter
 
 from translate.lang.common import Common
 from translate.misc.multistring import multistring
 from translate.storage import factory
 from translate.storage.workflow import StateEnum
 
-try:
-    from functools import cached_property
-except ImportError:
-    # Fix for python 3.7
-    cached_property = property
-
 extended_state_strings = {
     StateEnum.EMPTY: "empty",
     StateEnum.NEEDS_WORK: "needs-work",
     StateEnum.REJECTED: "rejected",
     StateEnum.NEEDS_REVIEW: "needs-review",
     StateEnum.UNREVIEWED: "unreviewed",
     StateEnum.FINAL: "final",
```

### Comparing `translate-toolkit-3.9.0/translate/tools/podebug.py` & `translate-toolkit-3.9.1/translate/tools/podebug.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/tools/pogrep.py` & `translate-toolkit-3.9.1/translate/tools/pogrep.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/tools/pomerge.py` & `translate-toolkit-3.9.1/translate/tools/pomerge.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/tools/porestructure.py` & `translate-toolkit-3.9.1/translate/tools/porestructure.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/tools/posegment.py` & `translate-toolkit-3.9.1/translate/tools/posegment.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/tools/poswap.py` & `translate-toolkit-3.9.1/translate/tools/poswap.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/tools/poterminology.py` & `translate-toolkit-3.9.1/translate/tools/poterminology.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/tools/pretranslate.py` & `translate-toolkit-3.9.1/translate/tools/pretranslate.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/tools/pydiff.py` & `translate-toolkit-3.9.1/translate/tools/pydiff.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/tools/pypo2phppo.py` & `translate-toolkit-3.9.1/translate/tools/pypo2phppo.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/tools/test_help.py` & `translate-toolkit-3.9.1/translate/tools/test_help.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/tools/test_phppo2pypo.py` & `translate-toolkit-3.9.1/translate/tools/test_phppo2pypo.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/tools/test_pocount.py` & `translate-toolkit-3.9.1/translate/tools/test_pocount.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,25 @@
+import subprocess
+import sys
 from io import BytesIO
 
-from pytest import mark
+from pytest import CaptureFixture, mark, param
 
 from translate.storage import po
 from translate.tools import pocount
 
-from ._test_utils import requires_py38_mark, test_po_files
+# For now test files left in the old places, but it's better to move
+# them somwhere like tests/data.
+_po_csv, _po_file, _po_fuzzy = test_files = [
+    "tests/cli/data/test_pocount_po_csv/one.po",
+    "tests/cli/data/test_pocount_po_file/one.po",
+    "tests/cli/data/test_pocount_po_fuzzy/one.po",
+]
+_xliff_states_yes = "tests/cli/data/test_pocount_xliff_states_yes/states.xlf"
+_xliff_states_no = "tests/cli/data/test_pocount_xliff_states_no/states.xlf"
 
 
 class TestCount:
     @staticmethod
     def count(source, expectedsource, target=None, expectedtarget=None):
         """simple helper to check the respective word counts"""
         poelement = po.pounit(source)
@@ -162,22 +172,68 @@
 
     def test_totalsourcewords(self):
         pofile = BytesIO(self.inputdata)
         stats = pocount.calcstats(pofile)
         assert stats["totalsourcewords"] == 6
 
 
-@requires_py38_mark
 @mark.parametrize("style", ["csv", "full", "short-strings", "short-words"])
 @mark.parametrize("incomplete", [True, False], ids=lambda v: f"incomplete={v}")
 @mark.parametrize("no_color", [True, False], ids=lambda v: f"no-color={v}")
-def test_output(style, incomplete, no_color, capsys, snapshot):
+def test_output(style, incomplete, no_color, capsys: CaptureFixture[str], snapshot):
     opts = [f"--{style}"]
     if incomplete:
         opts.append("--incomplete")
     if no_color:
         opts.append("--no-color")
 
-    pocount.main([*opts, *test_po_files])
+    pocount.main([*opts, *test_files])
     stdout = capsys.readouterr()[0]
 
     assert stdout == snapshot
+
+
+@mark.parametrize(
+    "opts",
+    [
+        param([_po_file, "--no-color"], id="po-file"),
+        param([_po_fuzzy, "--no-color"], id="po-file-fuzzy"),
+        param([_po_csv, "--no-color", "--csv"], id="po-file-csv"),
+        param([_xliff_states_yes, "--no-color"], id="xliff-states-yes"),
+        param([_xliff_states_no, "--no-color"], id="xliff-states-no"),
+    ],
+)
+def test_cases(opts, capsys: CaptureFixture[str], snapshot):
+    pocount.main(opts)
+
+    result = capsys.readouterr()
+
+    assert result == snapshot
+
+
+@mark.parametrize(
+    "opts,expected",
+    [
+        param(
+            ["--csv", "--short"],
+            "argument --short: not allowed with argument --csv",
+            id="mutually-exclusive",
+        ),
+        param(
+            ["missing.po"],
+            "cannot process missing.po: does not exist",
+            id="missing-file",
+        ),
+        param([], "the following arguments are required: files", id="no-args"),
+    ],
+)
+def test_error_cases(opts, expected):
+    # We're using special case for this, to produce correct output.
+    # Also, using partial matching instead of snapshots, becouse mac-os argparse
+    # output is slightly different.
+    result = subprocess.run(
+        [sys.executable, pocount.__file__, *opts],
+        capture_output=True,
+        text=True,
+    )
+
+    assert expected in result.stderr
```

### Comparing `translate-toolkit-3.9.0/translate/tools/test_podebug.py` & `translate-toolkit-3.9.1/translate/tools/test_podebug.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/tools/test_pogrep.py` & `translate-toolkit-3.9.1/translate/tools/test_pogrep.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/tools/test_pomerge.py` & `translate-toolkit-3.9.1/translate/tools/test_pomerge.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/tools/test_posegment.py` & `translate-toolkit-3.9.1/translate/tools/test_posegment.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/tools/test_poterminology.py` & `translate-toolkit-3.9.1/translate/tools/test_poterminology.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/tools/test_pretranslate.py` & `translate-toolkit-3.9.1/translate/tools/test_pretranslate.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate/tools/test_pypo2phppo.py` & `translate-toolkit-3.9.1/translate/tools/test_pypo2phppo.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate_toolkit.egg-info/PKG-INFO` & `translate-toolkit-3.9.1/translate_toolkit.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: translate-toolkit
-Version: 3.9.0
+Version: 3.9.1
 Summary: Tools and API for translation and localization engineering.
 Home-page: https://toolkit.translatehouse.org/
 Download-URL: https://github.com/translate/translate/releases/
 Author: Translate
 Author-email: translate-devel@lists.sourceforge.net
 License: GPL-2.0-or-later
 Project-URL: Issue Tracker, https://github.com/translate/translate/issues
@@ -19,23 +19,22 @@
 Classifier: Operating System :: OS Independent
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Internationalization
 Classifier: Topic :: Software Development :: Localization
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 Provides-Extra: all
 Provides-Extra: Subtitles
 Provides-Extra: Trados
 Provides-Extra: chardet
 Provides-Extra: tmserver
 Provides-Extra: Fluent
@@ -145,15 +144,15 @@
 .. note:: Please check ``requirements/*.txt``::
 
        pip install -r requirements/optional.txt
 
    Will install all optional dependencies convering support for many other
    formats.
 
-The Toolkit requires Python 3.7 or newer.
+The Toolkit requires Python 3.8 or newer.
 
 The package lxml is required. You should install version 4.6.3 or later.
 <http://lxml.de/> Depending on your platform, the easiest way to install might
 be through your system's package management. Alternatively you can try ::
 
     pip install lxml
```

### Comparing `translate-toolkit-3.9.0/translate_toolkit.egg-info/SOURCES.txt` & `translate-toolkit-3.9.1/translate_toolkit.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -256,14 +256,15 @@
 docs/releases/3.8.1.rst
 docs/releases/3.8.2.rst
 docs/releases/3.8.3.rst
 docs/releases/3.8.4.rst
 docs/releases/3.8.5.rst
 docs/releases/3.8.6.rst
 docs/releases/3.9.0.rst
+docs/releases/3.9.1.rst
 docs/releases/README.rst
 docs/releases/index.rst
 requirements/dev.txt
 requirements/dist.txt
 requirements/lint.txt
 requirements/optional.txt
 requirements/required.txt
@@ -285,21 +286,14 @@
 tests/cli/test_po2flatxml_template.sh
 tests/cli/test_po2html.sh
 tests/cli/test_po2json_files_removeuntranslated.sh
 tests/cli/test_po2prop_mozilla_files.sh
 tests/cli/test_po2ts.sh
 tests/cli/test_po2txt.sh
 tests/cli/test_po2txt_threshold.sh
-tests/cli/test_pocount.sh
-tests/cli/test_pocount_mutually_exclusive.sh
-tests/cli/test_pocount_nonexistant.sh
-tests/cli/test_pocount_po_file.sh
-tests/cli/test_pocount_po_fuzzy.sh
-tests/cli/test_pocount_xliff_states_no.sh
-tests/cli/test_pocount_xliff_states_yes.sh
 tests/cli/test_pofilter_listfilters.sh
 tests/cli/test_pofilter_manpage.sh
 tests/cli/test_posegment.sh
 tests/cli/test_poswap_comments.sh
 tests/cli/test_poswap_fr_af.sh
 tests/cli/test_poswap_fr_af_reverse.sh
 tests/cli/test_poswap_missing_units.sh
@@ -345,28 +339,20 @@
 tests/cli/data/test_po2prop_mozilla_files/translations.po
 tests/cli/data/test_po2ts/one.po
 tests/cli/data/test_po2ts/out.txt
 tests/cli/data/test_po2txt/one.po
 tests/cli/data/test_po2txt/out.txt
 tests/cli/data/test_po2txt_threshold/one.po
 tests/cli/data/test_po2txt_threshold/out.txt
-tests/cli/data/test_pocount/stderr.txt
-tests/cli/data/test_pocount_mutually_exclusive/stderr.txt
-tests/cli/data/test_pocount_nonexistant/stderr.txt
 tests/cli/data/test_pocount_po_csv/one.po
 tests/cli/data/test_pocount_po_file/one.po
-tests/cli/data/test_pocount_po_file/stdout.txt
 tests/cli/data/test_pocount_po_fuzzy/one.po
-tests/cli/data/test_pocount_po_fuzzy/stdout.txt
 tests/cli/data/test_pocount_po_plurals/plural.po
-tests/cli/data/test_pocount_po_plurals/stdout.txt
 tests/cli/data/test_pocount_xliff_states_no/states.xlf
-tests/cli/data/test_pocount_xliff_states_no/stdout.txt
 tests/cli/data/test_pocount_xliff_states_yes/states.xlf
-tests/cli/data/test_pocount_xliff_states_yes/stdout.txt
 tests/cli/data/test_pofilter_listfilters/stdout.txt
 tests/cli/data/test_pofilter_manpage/stdout.txt
 tests/cli/data/test_posegment/one.po
 tests/cli/data/test_posegment/out.po
 tests/cli/data/test_poswap_comments/af.po
 tests/cli/data/test_poswap_comments/fr.po
 tests/cli/data/test_poswap_comments/out.po
@@ -874,15 +860,14 @@
 translate/storage/xml_extract/misc.py
 translate/storage/xml_extract/test_misc.py
 translate/storage/xml_extract/test_unit_tree.py
 translate/storage/xml_extract/test_xpath_breadcrumb.py
 translate/storage/xml_extract/unit_tree.py
 translate/storage/xml_extract/xpath_breadcrumb.py
 translate/tools/__init__.py
-translate/tools/_test_utils.py
 translate/tools/build_tmdb.py
 translate/tools/junitmsgfmt.py
 translate/tools/phppo2pypo.py
 translate/tools/poclean.py
 translate/tools/pocompile.py
 translate/tools/poconflicts.py
 translate/tools/pocount.py
```

### Comparing `translate-toolkit-3.9.0/translate_toolkit.egg-info/entry_points.txt` & `translate-toolkit-3.9.1/translate_toolkit.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.9.0/translate_toolkit.egg-info/requires.txt` & `translate-toolkit-3.9.1/translate_toolkit.egg-info/requires.txt`

 * *Files 21% similar despite different names*

```diff
@@ -21,35 +21,35 @@
 [Subtitles]
 aeidon==1.12
 
 [Trados]
 BeautifulSoup4>=4.3
 
 [YAML]
-ruamel.yaml==0.17.26
+ruamel.yaml==0.17.31
 
 [all]
 aeidon==1.12
 BeautifulSoup4>=4.3
 charset-normalizer==3.1.0
-cheroot==9.0.0
+cheroot==10.0.0
 fluent.syntax==0.19.0
 iniparse==0.5
 phply==1.2.6
 pycountry==22.3.5
 pyenchant==3.2.2
 pyparsing==3.0.9
 python-Levenshtein>=0.12
-ruamel.yaml==0.17.26
+ruamel.yaml==0.17.31
 vobject==0.9.6.1
 
 [chardet]
 charset-normalizer==3.1.0
 
 [iCal]
 vobject==0.9.6.1
 
 [spellcheck]
 pyenchant==3.2.2
 
 [tmserver]
-cheroot==9.0.0
+cheroot==10.0.0
```

