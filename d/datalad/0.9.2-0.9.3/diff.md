# Comparing `tmp/datalad-0.9.2.tar.gz` & `tmp/datalad-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/datalad-0.9.2.tar", last modified: Sun Mar  4 16:37:52 2018, max compression
+gzip compressed data, was "dist/datalad-0.9.3.tar", last modified: Fri Mar 16 22:27:17 2018, max compression
```

## Comparing `datalad-0.9.2.tar` & `datalad-0.9.3.tar`

### file list

```diff
@@ -1,481 +1,484 @@
-drwx------   0 yoh      (47521) yoh      (47522)        0 2018-03-04 16:37:52.000000 datalad-0.9.2/
--rw-------   0 yoh      (47521) yoh      (47522)    10556 2018-03-04 16:37:40.000000 datalad-0.9.2/setup_support.py
--rw-------   0 yoh      (47521) yoh      (47522)      234 2018-03-04 16:37:39.000000 datalad-0.9.2/CONTRIBUTORS
--rw-------   0 yoh      (47521) yoh      (47522)    10252 2018-03-04 16:37:39.000000 datalad-0.9.2/.travis.yml
--rw-------   0 yoh      (47521) yoh      (47522)     1008 2018-03-04 16:37:39.000000 datalad-0.9.2/Makefile
-drwx------   0 yoh      (47521) yoh      (47522)        0 2018-03-04 16:37:52.000000 datalad-0.9.2/docs/
--rw-------   0 yoh      (47521) yoh      (47522)     7442 2018-03-04 16:37:40.000000 datalad-0.9.2/docs/Makefile
--rw-------   0 yoh      (47521) yoh      (47522)     2183 2018-03-04 16:37:40.000000 datalad-0.9.2/docs/config-format.rst
--rw-------   0 yoh      (47521) yoh      (47522)    21350 2018-03-04 16:37:40.000000 datalad-0.9.2/docs/design.rst
--rw-------   0 yoh      (47521) yoh      (47522)     5594 2018-03-04 16:37:40.000000 datalad-0.9.2/docs/datalad-metadata.rst
-drwx------   0 yoh      (47521) yoh      (47522)        0 2018-03-04 16:37:52.000000 datalad-0.9.2/docs/examples/
--rwx------   0 yoh      (47521) yoh      (47522)    12911 2018-03-04 16:37:40.000000 datalad-0.9.2/docs/examples/nipype_workshop_dataset.sh
--rwx------   0 yoh      (47521) yoh      (47522)     2222 2018-03-04 16:37:40.000000 datalad-0.9.2/docs/examples/make_pymvpa_collection.sh_broken
--rwx------   0 yoh      (47521) yoh      (47522)     1106 2018-03-04 16:37:40.000000 datalad-0.9.2/docs/examples/make_large_bogus_collection.sh_broken
--rw-------   0 yoh      (47521) yoh      (47522)    10504 2018-03-04 16:37:40.000000 datalad-0.9.2/docs/examples/3rdparty_analysis_workflow.sh
-drwx------   0 yoh      (47521) yoh      (47522)        0 2018-03-04 16:37:52.000000 datalad-0.9.2/docs/casts/
--rw-------   0 yoh      (47521) yoh      (47522)     3262 2018-03-04 16:37:40.000000 datalad-0.9.2/docs/casts/boxcom.sh
--rw-------   0 yoh      (47521) yoh      (47522)     1738 2018-03-04 16:37:40.000000 datalad-0.9.2/docs/casts/seamless_nested_repos.sh
--rw-------   0 yoh      (47521) yoh      (47522)     1990 2018-03-04 16:37:40.000000 datalad-0.9.2/docs/casts/simple_provenance_tracking.sh
--rw-------   0 yoh      (47521) yoh      (47522)     3120 2018-03-04 16:37:40.000000 datalad-0.9.2/docs/casts/publish_on_github.sh
--rw-------   0 yoh      (47521) yoh      (47522)     2621 2018-03-04 16:37:40.000000 datalad-0.9.2/docs/casts/basic_search.sh
--rw-------   0 yoh      (47521) yoh      (47522)     1743 2018-03-04 16:37:40.000000 datalad-0.9.2/docs/casts/track_data_from_webpage.sh
--rwx------   0 yoh      (47521) yoh      (47522)     1128 2018-03-04 16:37:40.000000 datalad-0.9.2/docs/casts/cmdline_basic_usage.sh
--rw-------   0 yoh      (47521) yoh      (47522)     4925 2018-03-04 16:37:40.000000 datalad-0.9.2/docs/casts/reproducible_analysis.sh
--rw-------   0 yoh      (47521) yoh      (47522)     5459 2018-03-04 16:37:40.000000 datalad-0.9.2/docs/casts/heudiconv_dicom_to_bids.sh
-drwx------   0 yoh      (47521) yoh      (47522)        0 2018-03-04 16:37:52.000000 datalad-0.9.2/docs/source/
--rw-------   0 yoh      (47521) yoh      (47522)     4781 2018-03-04 16:37:40.000000 datalad-0.9.2/docs/source/customization.rst
--rw-------   0 yoh      (47521) yoh      (47522)      738 2018-03-04 16:37:40.000000 datalad-0.9.2/docs/source/index.rst
--rw-------   0 yoh      (47521) yoh      (47522)    22788 2018-03-04 16:37:40.000000 datalad-0.9.2/docs/source/changelog.rst
-drwx------   0 yoh      (47521) yoh      (47522)        0 2018-03-04 16:37:52.000000 datalad-0.9.2/docs/source/_extras/
--rw-------   0 yoh      (47521) yoh      (47522)     1105 2018-03-04 16:37:40.000000 datalad-0.9.2/docs/source/_extras/schema.json
--rw-------   0 yoh      (47521) yoh      (47522)     1717 2018-03-04 16:37:40.000000 datalad-0.9.2/docs/source/glossary.rst
--rw-------   0 yoh      (47521) yoh      (47522)     3060 2018-03-04 16:37:40.000000 datalad-0.9.2/docs/source/gettingstarted.rst
-drwx------   0 yoh      (47521) yoh      (47522)        0 2018-03-04 16:37:52.000000 datalad-0.9.2/docs/source/usecases/
--rw-------   0 yoh      (47521) yoh      (47522)      185 2018-03-04 16:37:40.000000 datalad-0.9.2/docs/source/usecases/index.rst
--rw-------   0 yoh      (47521) yoh      (47522)     6446 2018-03-04 16:37:40.000000 datalad-0.9.2/docs/source/metadata.rst
--rw-------   0 yoh      (47521) yoh      (47522)     1744 2018-03-04 16:37:40.000000 datalad-0.9.2/docs/source/config.rst
--rw-------   0 yoh      (47521) yoh      (47522)     2568 2018-03-04 16:37:40.000000 datalad-0.9.2/docs/source/modref.rst
-drwx------   0 yoh      (47521) yoh      (47522)        0 2018-03-04 16:37:52.000000 datalad-0.9.2/docs/source/crawler/
--rw-------   0 yoh      (47521) yoh      (47522)      361 2018-03-04 16:37:40.000000 datalad-0.9.2/docs/source/crawler/index.rst
--rw-------   0 yoh      (47521) yoh      (47522)     2806 2018-03-04 16:37:40.000000 datalad-0.9.2/docs/source/crawler/basics.rst
-drwx------   0 yoh      (47521) yoh      (47522)        0 2018-03-04 16:37:52.000000 datalad-0.9.2/docs/source/_templates/
-drwx------   0 yoh      (47521) yoh      (47522)        0 2018-03-04 16:37:52.000000 datalad-0.9.2/docs/source/_templates/autosummary/
--rw-------   0 yoh      (47521) yoh      (47522)      436 2018-03-04 16:37:40.000000 datalad-0.9.2/docs/source/_templates/autosummary/module.rst
--rw-------   0 yoh      (47521) yoh      (47522)      859 2018-03-04 16:37:40.000000 datalad-0.9.2/docs/source/acknowledgements.rst
--rw-------   0 yoh      (47521) yoh      (47522)    10163 2018-03-04 16:37:40.000000 datalad-0.9.2/docs/source/conf.py
--rw-------   0 yoh      (47521) yoh      (47522)     8801 2018-03-04 16:37:40.000000 datalad-0.9.2/docs/source/basics.rst
-drwx------   0 yoh      (47521) yoh      (47522)        0 2018-03-04 16:37:52.000000 datalad-0.9.2/docs/source/_static/
--rw-------   0 yoh      (47521) yoh      (47522)      958 2018-03-04 16:37:40.000000 datalad-0.9.2/docs/source/_static/datalad_logo.png
--rw-------   0 yoh      (47521) yoh      (47522)     1040 2018-03-04 16:37:40.000000 datalad-0.9.2/docs/source/faq.rst
--rw-------   0 yoh      (47521) yoh      (47522)     6547 2018-03-04 16:37:40.000000 datalad-0.9.2/docs/source/related.rst
--rw-------   0 yoh      (47521) yoh      (47522)     1725 2018-03-04 16:37:40.000000 datalad-0.9.2/docs/source/cmdline.rst
--rw-------   0 yoh      (47521) yoh      (47522)     5942 2018-03-04 16:37:40.000000 datalad-0.9.2/docs/source/background.rst
--rw-------   0 yoh      (47521) yoh      (47522)     9167 2018-03-04 16:37:52.000000 datalad-0.9.2/PKG-INFO
-drwx------   0 yoh      (47521) yoh      (47522)        0 2018-03-04 16:37:52.000000 datalad-0.9.2/.github/
--rw-------   0 yoh      (47521) yoh      (47522)      163 2018-03-04 16:37:39.000000 datalad-0.9.2/.github/PULL_REQUEST_TEMPLATE.md
--rw-------   0 yoh      (47521) yoh      (47522)      430 2018-03-04 16:37:39.000000 datalad-0.9.2/.github/issue_template.md
--rw-------   0 yoh      (47521) yoh      (47522)      295 2018-03-04 16:37:39.000000 datalad-0.9.2/Gruntfile.js
--rw-------   0 yoh      (47521) yoh      (47522)     1404 2018-03-04 16:37:40.000000 datalad-0.9.2/tox.ini
--rw-------   0 yoh      (47521) yoh      (47522)      367 2018-03-04 16:37:40.000000 datalad-0.9.2/requirements.txt
-drwx------   0 yoh      (47521) yoh      (47522)        0 2018-03-04 16:37:52.000000 datalad-0.9.2/tools/
--rwx------   0 yoh      (47521) yoh      (47522)     4562 2018-03-04 16:37:40.000000 datalad-0.9.2/tools/mimic_repo
--rw-------   0 yoh      (47521) yoh      (47522)      776 2018-03-04 16:37:40.000000 datalad-0.9.2/tools/cmdline-completion
--rwx------   0 yoh      (47521) yoh      (47522)      751 2018-03-04 16:37:40.000000 datalad-0.9.2/tools/eval_under_testloopfs
--rwx------   0 yoh      (47521) yoh      (47522)     2127 2018-03-04 16:37:40.000000 datalad-0.9.2/tools/git-web-submodules.sh
-drwx------   0 yoh      (47521) yoh      (47522)        0 2018-03-04 16:37:52.000000 datalad-0.9.2/tools/testing/
--rwx------   0 yoh      (47521) yoh      (47522)     1931 2018-03-04 16:37:40.000000 datalad-0.9.2/tools/testing/test_README_in_docker
--rwx------   0 yoh      (47521) yoh      (47522)     4134 2018-03-04 16:37:40.000000 datalad-0.9.2/tools/testing/start_website_in_docker
--rwx------   0 yoh      (47521) yoh      (47522)      481 2018-03-04 16:37:40.000000 datalad-0.9.2/tools/testing/travis_ifdown_nonlo.sh
--rw-------   0 yoh      (47521) yoh      (47522)     1285 2018-03-04 16:37:40.000000 datalad-0.9.2/tools/testing/test_README_in_docker-Dockerfile.in
--rwx------   0 yoh      (47521) yoh      (47522)     1041 2018-03-04 16:37:40.000000 datalad-0.9.2/tools/testing/run_doc_examples
--rw-------   0 yoh      (47521) yoh      (47522)       33 2018-03-04 16:37:40.000000 datalad-0.9.2/tools/testing/.gitignore
--rwx------   0 yoh      (47521) yoh      (47522)     3457 2018-03-04 16:37:40.000000 datalad-0.9.2/tools/testing/make_test_repo
--rw-------   0 yoh      (47521) yoh      (47522)     2633 2018-03-04 16:37:40.000000 datalad-0.9.2/tools/testing/start_website_in_docker-Dockerfile.in
-drwx------   0 yoh      (47521) yoh      (47522)        0 2018-03-04 16:37:52.000000 datalad-0.9.2/tools/testing/bad_internals/
-drwx------   0 yoh      (47521) yoh      (47522)        0 2018-03-04 16:37:52.000000 datalad-0.9.2/tools/testing/bad_internals/_scrapy/
--rw-------   0 yoh      (47521) yoh      (47522)       57 2018-03-04 16:37:40.000000 datalad-0.9.2/tools/testing/bad_internals/_scrapy/scrapy.py
-drwx------   0 yoh      (47521) yoh      (47522)        0 2018-03-04 16:37:52.000000 datalad-0.9.2/tools/testing/conf/
-drwx------   0 yoh      (47521) yoh      (47522)        0 2018-03-04 16:37:52.000000 datalad-0.9.2/tools/testing/conf/etc/
-drwx------   0 yoh      (47521) yoh      (47522)        0 2018-03-04 16:37:52.000000 datalad-0.9.2/tools/testing/conf/etc/apt/
-drwx------   0 yoh      (47521) yoh      (47522)        0 2018-03-04 16:37:52.000000 datalad-0.9.2/tools/testing/conf/etc/apt/apt.conf.d/
--rw-------   0 yoh      (47521) yoh      (47522)      112 2018-03-04 16:37:40.000000 datalad-0.9.2/tools/testing/conf/etc/apt/apt.conf.d/99apt-cacher
--rw-------   0 yoh      (47521) yoh      (47522)      179 2018-03-04 16:37:40.000000 datalad-0.9.2/tools/testing/conf/apache-ssh-supervisor.conf
--rwx------   0 yoh      (47521) yoh      (47522)      938 2018-03-04 16:37:40.000000 datalad-0.9.2/tools/testing/make_test_repos
--rwx------   0 yoh      (47521) yoh      (47522)      593 2018-03-04 16:37:40.000000 datalad-0.9.2/tools/upgrade-annex-osx.sh
--rwx------   0 yoh      (47521) yoh      (47522)     1531 2018-03-04 16:37:40.000000 datalad-0.9.2/tools/dtime
--rwx------   0 yoh      (47521) yoh      (47522)     2117 2018-03-04 16:37:40.000000 datalad-0.9.2/tools/cast2narration
--rwx------   0 yoh      (47521) yoh      (47522)      359 2018-03-04 16:37:40.000000 datalad-0.9.2/tools/mkcontrib
--rwx------   0 yoh      (47521) yoh      (47522)      656 2018-03-04 16:37:40.000000 datalad-0.9.2/tools/cast2script
--rwx------   0 yoh      (47521) yoh      (47522)     3064 2018-03-04 16:37:40.000000 datalad-0.9.2/tools/cast_live
--rwx------   0 yoh      (47521) yoh      (47522)     2472 2018-03-04 16:37:40.000000 datalad-0.9.2/tools/copy_urls_from_datalad.py
--rw-------   0 yoh      (47521) yoh      (47522)     1715 2018-03-04 16:37:40.000000 datalad-0.9.2/tools/cast_bash.rc
-drwx------   0 yoh      (47521) yoh      (47522)        0 2018-03-04 16:37:52.000000 datalad-0.9.2/tools/ci/
--rw-------   0 yoh      (47521) yoh      (47522)      589 2018-03-04 16:37:40.000000 datalad-0.9.2/tools/ci/gpg-90F7E9EB.pub
--rwx------   0 yoh      (47521) yoh      (47522)      513 2018-03-04 16:37:40.000000 datalad-0.9.2/tools/ci/install-annex-snapshot.sh
--rwx------   0 yoh      (47521) yoh      (47522)      714 2018-03-04 16:37:40.000000 datalad-0.9.2/tools/ci/prep-travis-devel-annex.sh
--rwx------   0 yoh      (47521) yoh      (47522)      581 2018-03-04 16:37:40.000000 datalad-0.9.2/tools/ci/prep-travis-forssh.sh
--rwx------   0 yoh      (47521) yoh      (47522)       97 2018-03-04 16:37:40.000000 datalad-0.9.2/tools/ci/prep-travis-forssh-sudo.sh
--rwx------   0 yoh      (47521) yoh      (47522)     4000 2018-03-04 16:37:40.000000 datalad-0.9.2/tools/cast2asciinema
--rwx------   0 yoh      (47521) yoh      (47522)     2797 2018-03-04 16:37:40.000000 datalad-0.9.2/tools/monitor-interrupts.py
-drwx------   0 yoh      (47521) yoh      (47522)        0 2018-03-04 16:37:52.000000 datalad-0.9.2/tools/coverage-bin/
--rwx------   0 yoh      (47521) yoh      (47522)      806 2018-03-04 16:37:40.000000 datalad-0.9.2/tools/coverage-bin/git-annex-remote-datalad
--rwx------   0 yoh      (47521) yoh      (47522)      806 2018-03-04 16:37:40.000000 datalad-0.9.2/tools/coverage-bin/git-annex-remote-datalad-archives
--rwx------   0 yoh      (47521) yoh      (47522)      806 2018-03-04 16:37:40.000000 datalad-0.9.2/tools/coverage-bin/datalad
--rwx------   0 yoh      (47521) yoh      (47522)     3010 2018-03-04 16:37:40.000000 datalad-0.9.2/tools/mimic_merges
--rwx------   0 yoh      (47521) yoh      (47522)     3565 2018-03-04 16:37:40.000000 datalad-0.9.2/tools/urlinfo
--rw-------   0 yoh      (47521) yoh      (47522)    24017 2018-03-04 16:37:39.000000 datalad-0.9.2/CHANGELOG.md
--rw-------   0 yoh      (47521) yoh      (47522)     2114 2018-03-04 16:37:39.000000 datalad-0.9.2/COPYING
--rw-------   0 yoh      (47521) yoh      (47522)      377 2018-03-04 16:37:40.000000 datalad-0.9.2/requirements-devel.txt
--rw-------   0 yoh      (47521) yoh      (47522)       38 2018-03-04 16:37:52.000000 datalad-0.9.2/setup.cfg
--rw-------   0 yoh      (47521) yoh      (47522)      223 2018-03-04 16:37:39.000000 datalad-0.9.2/.gitignore
--rw-------   0 yoh      (47521) yoh      (47522)     7150 2018-03-04 16:37:39.000000 datalad-0.9.2/README.md
--rw-------   0 yoh      (47521) yoh      (47522)    18631 2018-03-04 16:37:39.000000 datalad-0.9.2/CONTRIBUTING.md
--rw-------   0 yoh      (47521) yoh      (47522)     6066 2018-03-04 16:37:39.000000 datalad-0.9.2/asv.conf.json
-drwx------   0 yoh      (47521) yoh      (47522)        0 2018-03-04 16:37:52.000000 datalad-0.9.2/cfgs/
--rw-------   0 yoh      (47521) yoh      (47522)      441 2018-03-04 16:37:39.000000 datalad-0.9.2/cfgs/openfmri.cfg
--rw-------   0 yoh      (47521) yoh      (47522)     1179 2018-03-04 16:37:39.000000 datalad-0.9.2/cfgs/openfmri-ds000001.cfg
--rw-------   0 yoh      (47521) yoh      (47522)       90 2018-03-04 16:37:39.000000 datalad-0.9.2/cfgs/arjlover.cfg
--rw-------   0 yoh      (47521) yoh      (47522)     2409 2018-03-04 16:37:39.000000 datalad-0.9.2/cfgs/nihhelpers.py
--rw-------   0 yoh      (47521) yoh      (47522)     1150 2018-03-04 16:37:39.000000 datalad-0.9.2/cfgs/nih-videos.cfg
--rw-------   0 yoh      (47521) yoh      (47522)      979 2018-03-04 16:37:39.000000 datalad-0.9.2/cfgs/arjlover-fast.cfg
--rw-------   0 yoh      (47521) yoh      (47522)      451 2018-03-04 16:37:39.000000 datalad-0.9.2/cfgs/example-feat.cfg
--rw-------   0 yoh      (47521) yoh      (47522)     2015 2018-03-04 16:37:39.000000 datalad-0.9.2/cfgs/common.cfg
--rw-------   0 yoh      (47521) yoh      (47522)      810 2018-03-04 16:37:39.000000 datalad-0.9.2/cfgs/allen-human.cfg
--rw-------   0 yoh      (47521) yoh      (47522)      305 2018-03-04 16:37:39.000000 datalad-0.9.2/CODE_OF_CONDUCT.md
-drwx------   0 yoh      (47521) yoh      (47522)        0 2018-03-04 16:37:52.000000 datalad-0.9.2/benchmarks/
--rw-------   0 yoh      (47521) yoh      (47522)     2216 2018-03-04 16:37:39.000000 datalad-0.9.2/benchmarks/core.py
--rw-------   0 yoh      (47521) yoh      (47522)        1 2018-03-04 16:37:39.000000 datalad-0.9.2/benchmarks/__init__.py
--rw-------   0 yoh      (47521) yoh      (47522)     4012 2018-03-04 16:37:39.000000 datalad-0.9.2/benchmarks/api.py
--rw-------   0 yoh      (47521) yoh      (47522)      696 2018-03-04 16:37:39.000000 datalad-0.9.2/benchmarks/common.py
--rw-------   0 yoh      (47521) yoh      (47522)      517 2018-03-04 16:37:39.000000 datalad-0.9.2/.mailmap
--rw-------   0 yoh      (47521) yoh      (47522)    10446 2018-03-04 16:37:40.000000 datalad-0.9.2/formatters.py
--rw-------   0 yoh      (47521) yoh      (47522)      125 2018-03-04 16:37:40.000000 datalad-0.9.2/readthedocs.yml
--rw-------   0 yoh      (47521) yoh      (47522)       75 2018-03-04 16:37:39.000000 datalad-0.9.2/.gitmodules
--rw-------   0 yoh      (47521) yoh      (47522)       45 2018-03-04 16:37:39.000000 datalad-0.9.2/.coveragerc
-drwx------   0 yoh      (47521) yoh      (47522)        0 2018-03-04 16:37:52.000000 datalad-0.9.2/datalad.egg-info/
--rw-------   0 yoh      (47521) yoh      (47522)        8 2018-03-04 16:37:52.000000 datalad-0.9.2/datalad.egg-info/top_level.txt
--rw-------   0 yoh      (47521) yoh      (47522)     9167 2018-03-04 16:37:52.000000 datalad-0.9.2/datalad.egg-info/PKG-INFO
--rw-------   0 yoh      (47521) yoh      (47522)     1557 2018-03-04 16:37:52.000000 datalad-0.9.2/datalad.egg-info/requires.txt
--rw-------   0 yoh      (47521) yoh      (47522)    13588 2018-03-04 16:37:52.000000 datalad-0.9.2/datalad.egg-info/SOURCES.txt
--rw-------   0 yoh      (47521) yoh      (47522)        1 2018-03-04 16:37:52.000000 datalad-0.9.2/datalad.egg-info/dependency_links.txt
-drwx------   0 yoh      (47521) yoh      (47522)        0 2018-03-04 16:37:52.000000 datalad-0.9.2/datalad/
-drwx------   0 yoh      (47521) yoh      (47522)        0 2018-03-04 16:37:52.000000 datalad-0.9.2/datalad/tests/
--rw-------   0 yoh      (47521) yoh      (47522)     1721 2018-03-04 16:37:40.000000 datalad-0.9.2/datalad/tests/test_base.py
--rw-------   0 yoh      (47521) yoh      (47522)     7686 2018-03-04 16:37:40.000000 datalad-0.9.2/datalad/tests/test_constraints.py
--rw-------   0 yoh      (47521) yoh      (47522)     2421 2018-03-04 16:37:40.000000 datalad-0.9.2/datalad/tests/test_testrepos.py
--rw-------   0 yoh      (47521) yoh      (47522)     4561 2018-03-04 16:37:40.000000 datalad-0.9.2/datalad/tests/test_interface.py
--rw-------   0 yoh      (47521) yoh      (47522)     1530 2018-03-04 16:37:40.000000 datalad-0.9.2/datalad/tests/test__main__.py
--rw-------   0 yoh      (47521) yoh      (47522)    27257 2018-03-04 16:37:40.000000 datalad-0.9.2/datalad/tests/test_utils.py
--rw-------   0 yoh      (47521) yoh      (47522)      252 2018-03-04 16:37:40.000000 datalad-0.9.2/datalad/tests/heavyoutput.py
--rw-------   0 yoh      (47521) yoh      (47522)     2961 2018-03-04 16:37:40.000000 datalad-0.9.2/datalad/tests/test_s3.py
--rw-------   0 yoh      (47521) yoh      (47522)     4013 2018-03-04 16:37:40.000000 datalad-0.9.2/datalad/tests/utils_testdatasets.py
--rw-------   0 yoh      (47521) yoh      (47522)     1442 2018-03-04 16:37:40.000000 datalad-0.9.2/datalad/tests/test_misc.py
--rw-------   0 yoh      (47521) yoh      (47522)     5302 2018-03-04 16:37:40.000000 datalad-0.9.2/datalad/tests/test_log.py
--rw-------   0 yoh      (47521) yoh      (47522)     7396 2018-03-04 16:37:40.000000 datalad-0.9.2/datalad/tests/test_auto.py
--rw-------   0 yoh      (47521) yoh      (47522)      811 2018-03-04 16:37:40.000000 datalad-0.9.2/datalad/tests/__init__.py
--rw-------   0 yoh      (47521) yoh      (47522)    19205 2018-03-04 16:37:40.000000 datalad-0.9.2/datalad/tests/test_tests_utils.py
--rw-------   0 yoh      (47521) yoh      (47522)     6891 2018-03-04 16:37:40.000000 datalad-0.9.2/datalad/tests/test_archives.py
--rw-------   0 yoh      (47521) yoh      (47522)    12049 2018-03-04 16:37:40.000000 datalad-0.9.2/datalad/tests/test_config.py
--rw-------   0 yoh      (47521) yoh      (47522)    11446 2018-03-04 16:37:40.000000 datalad-0.9.2/datalad/tests/test_cmd.py
--rw-------   0 yoh      (47521) yoh      (47522)    46247 2018-03-04 16:37:40.000000 datalad-0.9.2/datalad/tests/utils.py
--rw-------   0 yoh      (47521) yoh      (47522)     7897 2018-03-04 16:37:40.000000 datalad-0.9.2/datalad/tests/utils_testrepos.py
--rw-------   0 yoh      (47521) yoh      (47522)     1924 2018-03-04 16:37:40.000000 datalad-0.9.2/datalad/tests/test_utils_testrepos.py
--rw-------   0 yoh      (47521) yoh      (47522)     2714 2018-03-04 16:37:40.000000 datalad-0.9.2/datalad/tests/test_api.py
--rw-------   0 yoh      (47521) yoh      (47522)     6919 2018-03-04 16:37:40.000000 datalad-0.9.2/datalad/tests/test_protocols.py
--rw-------   0 yoh      (47521) yoh      (47522)     1323 2018-03-04 16:37:40.000000 datalad-0.9.2/datalad/tests/test_installed.py
--rw-------   0 yoh      (47521) yoh      (47522)     5168 2018-03-04 16:37:40.000000 datalad-0.9.2/datalad/tests/test_dochelpers.py
--rw-------   0 yoh      (47521) yoh      (47522)     1256 2018-03-04 16:37:40.000000 datalad-0.9.2/datalad/tests/test_strings.py
--rw-------   0 yoh      (47521) yoh      (47522)     3700 2018-03-04 16:37:40.000000 datalad-0.9.2/datalad/tests/test_direct_mode.py
-drwx------   0 yoh      (47521) yoh      (47522)        0 2018-03-04 16:37:52.000000 datalad-0.9.2/datalad/interface/
--rw-------   0 yoh      (47521) yoh      (47522)    17663 2018-03-04 16:37:40.000000 datalad-0.9.2/datalad/interface/base.py
-drwx------   0 yoh      (47521) yoh      (47522)        0 2018-03-04 16:37:52.000000 datalad-0.9.2/datalad/interface/tests/
--rw-------   0 yoh      (47521) yoh      (47522)    11892 2018-03-04 16:37:40.000000 datalad-0.9.2/datalad/interface/tests/test_save.py
--rw-------   0 yoh      (47521) yoh      (47522)    20545 2018-03-04 16:37:40.000000 datalad-0.9.2/datalad/interface/tests/test_add_archive_content.py
--rw-------   0 yoh      (47521) yoh      (47522)     4053 2018-03-04 16:37:40.000000 datalad-0.9.2/datalad/interface/tests/test_ls.py
--rw-------   0 yoh      (47521) yoh      (47522)    10639 2018-03-04 16:37:40.000000 datalad-0.9.2/datalad/interface/tests/test_utils.py
--rw-------   0 yoh      (47521) yoh      (47522)     3626 2018-03-04 16:37:40.000000 datalad-0.9.2/datalad/interface/tests/test_crawl_init.py
--rw-------   0 yoh      (47521) yoh      (47522)     6223 2018-03-04 16:37:40.000000 datalad-0.9.2/datalad/interface/tests/test_unlock.py
--rw-------   0 yoh      (47521) yoh      (47522)      450 2018-03-04 16:37:40.000000 datalad-0.9.2/datalad/interface/tests/__init__.py
--rw-------   0 yoh      (47521) yoh      (47522)     8010 2018-03-04 16:37:40.000000 datalad-0.9.2/datalad/interface/tests/test_diff.py
--rw-------   0 yoh      (47521) yoh      (47522)    13953 2018-03-04 16:37:40.000000 datalad-0.9.2/datalad/interface/tests/test_annotate_paths.py
--rw-------   0 yoh      (47521) yoh      (47522)     4040 2018-03-04 16:37:40.000000 datalad-0.9.2/datalad/interface/tests/test_docs.py
--rw-------   0 yoh      (47521) yoh      (47522)    11328 2018-03-04 16:37:40.000000 datalad-0.9.2/datalad/interface/tests/test_ls_webui.py
--rw-------   0 yoh      (47521) yoh      (47522)     1921 2018-03-04 16:37:40.000000 datalad-0.9.2/datalad/interface/tests/test_download_url.py
--rw-------   0 yoh      (47521) yoh      (47522)     3876 2018-03-04 16:37:40.000000 datalad-0.9.2/datalad/interface/tests/test_crawl.py
--rw-------   0 yoh      (47521) yoh      (47522)    17415 2018-03-04 16:37:40.000000 datalad-0.9.2/datalad/interface/tests/test_run.py
--rw-------   0 yoh      (47521) yoh      (47522)     2385 2018-03-04 16:37:40.000000 datalad-0.9.2/datalad/interface/tests/test_clean.py
--rw-------   0 yoh      (47521) yoh      (47522)     8670 2018-03-04 16:37:40.000000 datalad-0.9.2/datalad/interface/run.py
--rw-------   0 yoh      (47521) yoh      (47522)    24739 2018-03-04 16:37:40.000000 datalad-0.9.2/datalad/interface/add_archive_content.py
--rw-------   0 yoh      (47521) yoh      (47522)     4510 2018-03-04 16:37:40.000000 datalad-0.9.2/datalad/interface/clean.py
--rw-------   0 yoh      (47521) yoh      (47522)    13120 2018-03-04 16:37:40.000000 datalad-0.9.2/datalad/interface/results.py
--rw-------   0 yoh      (47521) yoh      (47522)     8048 2018-03-04 16:37:40.000000 datalad-0.9.2/datalad/interface/crawl.py
--rw-------   0 yoh      (47521) yoh      (47522)     3999 2018-03-04 16:37:40.000000 datalad-0.9.2/datalad/interface/download_url.py
--rw-------   0 yoh      (47521) yoh      (47522)    23859 2018-03-04 16:37:40.000000 datalad-0.9.2/datalad/interface/ls.py
--rw-------   0 yoh      (47521) yoh      (47522)     3398 2018-03-04 16:37:40.000000 datalad-0.9.2/datalad/interface/__init__.py
--rw-------   0 yoh      (47521) yoh      (47522)     6525 2018-03-04 16:37:40.000000 datalad-0.9.2/datalad/interface/unlock.py
--rw-------   0 yoh      (47521) yoh      (47522)    16884 2018-03-04 16:37:40.000000 datalad-0.9.2/datalad/interface/save.py
--rw-------   0 yoh      (47521) yoh      (47522)     1936 2018-03-04 16:37:40.000000 datalad-0.9.2/datalad/interface/test.py
--rw-------   0 yoh      (47521) yoh      (47522)    21736 2018-03-04 16:37:40.000000 datalad-0.9.2/datalad/interface/utils.py
--rw-------   0 yoh      (47521) yoh      (47522)    12505 2018-03-04 16:37:40.000000 datalad-0.9.2/datalad/interface/common_opts.py
--rw-------   0 yoh      (47521) yoh      (47522)    34837 2018-03-04 16:37:40.000000 datalad-0.9.2/datalad/interface/annotate_paths.py
--rw-------   0 yoh      (47521) yoh      (47522)    15913 2018-03-04 16:37:40.000000 datalad-0.9.2/datalad/interface/diff.py
--rw-------   0 yoh      (47521) yoh      (47522)     9291 2018-03-04 16:37:40.000000 datalad-0.9.2/datalad/interface/common_cfg.py
--rw-------   0 yoh      (47521) yoh      (47522)     3957 2018-03-04 16:37:40.000000 datalad-0.9.2/datalad/interface/crawl_init.py
--rw-------   0 yoh      (47521) yoh      (47522)    16245 2018-03-04 16:37:40.000000 datalad-0.9.2/datalad/interface/ls_webui.py
--rw-------   0 yoh      (47521) yoh      (47522)    12661 2018-03-04 16:37:40.000000 datalad-0.9.2/datalad/interface/rerun.py
--rw-------   0 yoh      (47521) yoh      (47522)     3132 2018-03-04 16:37:39.000000 datalad-0.9.2/datalad/__main__.py
-drwx------   0 yoh      (47521) yoh      (47522)        0 2018-03-04 16:37:52.000000 datalad-0.9.2/datalad/resources/
-drwx------   0 yoh      (47521) yoh      (47522)        0 2018-03-04 16:37:52.000000 datalad-0.9.2/datalad/resources/website/
-drwx------   0 yoh      (47521) yoh      (47522)        0 2018-03-04 16:37:52.000000 datalad-0.9.2/datalad/resources/website/tests/
--rw-------   0 yoh      (47521) yoh      (47522)    13759 2018-03-04 16:37:40.000000 datalad-0.9.2/datalad/resources/website/tests/test.html
-drwx------   0 yoh      (47521) yoh      (47522)        0 2018-03-04 16:37:52.000000 datalad-0.9.2/datalad/resources/website/tests/qunit/
--rw-------   0 yoh      (47521) yoh      (47522)   208178 2018-03-04 16:37:40.000000 datalad-0.9.2/datalad/resources/website/tests/qunit/sinon-1.17.5.js
--rw-------   0 yoh      (47521) yoh      (47522)   117821 2018-03-04 16:37:40.000000 datalad-0.9.2/datalad/resources/website/tests/qunit/qunit-2.0.1.js
--rw-------   0 yoh      (47521) yoh      (47522)     7456 2018-03-04 16:37:40.000000 datalad-0.9.2/datalad/resources/website/tests/qunit/qunit-2.0.1.css
--rw-------   0 yoh      (47521) yoh      (47522)     2443 2018-03-04 16:37:40.000000 datalad-0.9.2/datalad/resources/website/tests/qunit/sinon-qunit-1.0.0.js
-drwx------   0 yoh      (47521) yoh      (47522)        0 2018-03-04 16:37:52.000000 datalad-0.9.2/datalad/resources/website/assets/
-drwx------   0 yoh      (47521) yoh      (47522)        0 2018-03-04 16:37:52.000000 datalad-0.9.2/datalad/resources/website/assets/images/
--rw-------   0 yoh      (47521) yoh      (47522)    12537 2018-03-04 16:37:40.000000 datalad-0.9.2/datalad/resources/website/assets/images/logo_wide.svg
--rw-------   0 yoh      (47521) yoh      (47522)      158 2018-03-04 16:37:40.000000 datalad-0.9.2/datalad/resources/website/assets/images/sort_desc.png
--rw-------   0 yoh      (47521) yoh      (47522)      272 2018-03-04 16:37:40.000000 datalad-0.9.2/datalad/resources/website/assets/images/favicon-16x16.png
--rw-------   0 yoh      (47521) yoh      (47522)      199 2018-03-04 16:37:40.000000 datalad-0.9.2/datalad/resources/website/assets/images/sort_both.png
--rw-------   0 yoh      (47521) yoh      (47522)    15086 2018-03-04 16:37:40.000000 datalad-0.9.2/datalad/resources/website/assets/images/favicon.ico
--rw-------   0 yoh      (47521) yoh      (47522)    16891 2018-03-04 16:37:40.000000 datalad-0.9.2/datalad/resources/website/assets/images/favicon.svg
--rw-------   0 yoh      (47521) yoh      (47522)      158 2018-03-04 16:37:40.000000 datalad-0.9.2/datalad/resources/website/assets/images/sort_asc.png
-drwx------   0 yoh      (47521) yoh      (47522)        0 2018-03-04 16:37:52.000000 datalad-0.9.2/datalad/resources/website/assets/js/
--rw-------   0 yoh      (47521) yoh      (47522)     8572 2018-03-04 16:37:40.000000 datalad-0.9.2/datalad/resources/website/assets/js/md5-2.3.0.js
--rw-------   0 yoh      (47521) yoh      (47522)    21039 2018-03-04 16:37:40.000000 datalad-0.9.2/datalad/resources/website/assets/js/main.js
--rw-------   0 yoh      (47521) yoh      (47522)   447304 2018-03-04 16:37:40.000000 datalad-0.9.2/datalad/resources/website/assets/js/jquery.dataTables-1.10.12.js
--rw-------   0 yoh      (47521) yoh      (47522)   257551 2018-03-04 16:37:40.000000 datalad-0.9.2/datalad/resources/website/assets/js/jquery-2.2.4.js
-drwx------   0 yoh      (47521) yoh      (47522)        0 2018-03-04 16:37:52.000000 datalad-0.9.2/datalad/resources/website/assets/css/
--rw-------   0 yoh      (47521) yoh      (47522)    15423 2018-03-04 16:37:40.000000 datalad-0.9.2/datalad/resources/website/assets/css/jquery.dataTables-1.10.12.css
--rw-------   0 yoh      (47521) yoh      (47522)     3121 2018-03-04 16:37:40.000000 datalad-0.9.2/datalad/resources/website/index.html
-drwx------   0 yoh      (47521) yoh      (47522)        0 2018-03-04 16:37:52.000000 datalad-0.9.2/datalad/customremotes/
--rw-------   0 yoh      (47521) yoh      (47522)    23561 2018-03-04 16:37:39.000000 datalad-0.9.2/datalad/customremotes/base.py
-drwx------   0 yoh      (47521) yoh      (47522)        0 2018-03-04 16:37:52.000000 datalad-0.9.2/datalad/customremotes/tests/
--rw-------   0 yoh      (47521) yoh      (47522)     5199 2018-03-04 16:37:39.000000 datalad-0.9.2/datalad/customremotes/tests/test_base.py
--rw-------   0 yoh      (47521) yoh      (47522)     1112 2018-03-04 16:37:39.000000 datalad-0.9.2/datalad/customremotes/tests/__init__.py
--rw-------   0 yoh      (47521) yoh      (47522)    11004 2018-03-04 16:37:39.000000 datalad-0.9.2/datalad/customremotes/tests/test_archives.py
--rw-------   0 yoh      (47521) yoh      (47522)     4182 2018-03-04 16:37:39.000000 datalad-0.9.2/datalad/customremotes/tests/test_datalad.py
--rw-------   0 yoh      (47521) yoh      (47522)     4740 2018-03-04 16:37:39.000000 datalad-0.9.2/datalad/customremotes/main.py
--rw-------   0 yoh      (47521) yoh      (47522)      483 2018-03-04 16:37:39.000000 datalad-0.9.2/datalad/customremotes/__init__.py
--rw-------   0 yoh      (47521) yoh      (47522)     6906 2018-03-04 16:37:39.000000 datalad-0.9.2/datalad/customremotes/datalad.py
--rw-------   0 yoh      (47521) yoh      (47522)    16744 2018-03-04 16:37:39.000000 datalad-0.9.2/datalad/customremotes/archives.py
-drwx------   0 yoh      (47521) yoh      (47522)        0 2018-03-04 16:37:52.000000 datalad-0.9.2/datalad/plugin/
-drwx------   0 yoh      (47521) yoh      (47522)        0 2018-03-04 16:37:52.000000 datalad-0.9.2/datalad/plugin/tests/
--rw-------   0 yoh      (47521) yoh      (47522)      446 2018-03-04 16:37:40.000000 datalad-0.9.2/datalad/plugin/tests/__init__.py
--rw-------   0 yoh      (47521) yoh      (47522)     8700 2018-03-04 16:37:40.000000 datalad-0.9.2/datalad/plugin/tests/test_plugins.py
--rw-------   0 yoh      (47521) yoh      (47522)     3357 2018-03-04 16:37:40.000000 datalad-0.9.2/datalad/plugin/tests/test_tarball.py
--rw-------   0 yoh      (47521) yoh      (47522)     4256 2018-03-04 16:37:40.000000 datalad-0.9.2/datalad/plugin/no_annex.py
--rw-------   0 yoh      (47521) yoh      (47522)     2937 2018-03-04 16:37:40.000000 datalad-0.9.2/datalad/plugin/export_tarball.py
--rw-------   0 yoh      (47521) yoh      (47522)     3645 2018-03-04 16:37:40.000000 datalad-0.9.2/datalad/plugin/wtf.py
--rw-------   0 yoh      (47521) yoh      (47522)     9976 2018-03-04 16:37:40.000000 datalad-0.9.2/datalad/plugin/__init__.py
--rw-------   0 yoh      (47521) yoh      (47522)     2373 2018-03-04 16:37:40.000000 datalad-0.9.2/datalad/plugin/add_readme.py
--rw-------   0 yoh      (47521) yoh      (47522)    24506 2018-03-04 16:37:39.000000 datalad-0.9.2/datalad/config.py
--rw-------   0 yoh      (47521) yoh      (47522)    10578 2018-03-04 16:37:39.000000 datalad-0.9.2/datalad/auto.py
--rw-------   0 yoh      (47521) yoh      (47522)    10190 2018-03-04 16:37:40.000000 datalad-0.9.2/datalad/log.py
-drwx------   0 yoh      (47521) yoh      (47522)        0 2018-03-04 16:37:52.000000 datalad-0.9.2/datalad/support/
-drwx------   0 yoh      (47521) yoh      (47522)        0 2018-03-04 16:37:52.000000 datalad-0.9.2/datalad/support/tests/
--rw-------   0 yoh      (47521) yoh      (47522)      663 2018-03-04 16:37:40.000000 datalad-0.9.2/datalad/support/tests/test_cache.py
--rw-------   0 yoh      (47521) yoh      (47522)    18314 2018-03-04 16:37:40.000000 datalad-0.9.2/datalad/support/tests/test_network.py
--rw-------   0 yoh      (47521) yoh      (47522)    79763 2018-03-04 16:37:40.000000 datalad-0.9.2/datalad/support/tests/test_annexrepo.py
--rw-------   0 yoh      (47521) yoh      (47522)     1076 2018-03-04 16:37:40.000000 datalad-0.9.2/datalad/support/tests/test_vcr_.py
--rw-------   0 yoh      (47521) yoh      (47522)    42250 2018-03-04 16:37:40.000000 datalad-0.9.2/datalad/support/tests/test_gitrepo.py
--rw-------   0 yoh      (47521) yoh      (47522)     2025 2018-03-04 16:37:40.000000 datalad-0.9.2/datalad/support/tests/test_digests.py
--rw-------   0 yoh      (47521) yoh      (47522)     3184 2018-03-04 16:37:40.000000 datalad-0.9.2/datalad/support/tests/test_stats.py
--rw-------   0 yoh      (47521) yoh      (47522)      469 2018-03-04 16:37:40.000000 datalad-0.9.2/datalad/support/tests/__init__.py
--rw-------   0 yoh      (47521) yoh      (47522)     1508 2018-03-04 16:37:40.000000 datalad-0.9.2/datalad/support/tests/test_status.py
--rw-------   0 yoh      (47521) yoh      (47522)     6055 2018-03-04 16:37:40.000000 datalad-0.9.2/datalad/support/tests/test_versions.py
--rw-------   0 yoh      (47521) yoh      (47522)     1628 2018-03-04 16:37:40.000000 datalad-0.9.2/datalad/support/tests/utils.py
--rw-------   0 yoh      (47521) yoh      (47522)     1812 2018-03-04 16:37:40.000000 datalad-0.9.2/datalad/support/tests/test_sshrun.py
--rw-------   0 yoh      (47521) yoh      (47522)     1117 2018-03-04 16:37:40.000000 datalad-0.9.2/datalad/support/tests/test_json_py.py
--rw-------   0 yoh      (47521) yoh      (47522)     7912 2018-03-04 16:37:40.000000 datalad-0.9.2/datalad/support/tests/test_external_versions.py
--rw-------   0 yoh      (47521) yoh      (47522)     7611 2018-03-04 16:37:40.000000 datalad-0.9.2/datalad/support/tests/test_sshconnector.py
--rw-------   0 yoh      (47521) yoh      (47522)     6913 2018-03-04 16:37:40.000000 datalad-0.9.2/datalad/support/versions.py
--rw-------   0 yoh      (47521) yoh      (47522)     3247 2018-03-04 16:37:40.000000 datalad-0.9.2/datalad/support/keyring_.py
--rw-------   0 yoh      (47521) yoh      (47522)     5045 2018-03-04 16:37:40.000000 datalad-0.9.2/datalad/support/param.py
--rw-------   0 yoh      (47521) yoh      (47522)     3178 2018-03-04 16:37:40.000000 datalad-0.9.2/datalad/support/sshrun.py
--rw-------   0 yoh      (47521) yoh      (47522)     8584 2018-03-04 16:37:40.000000 datalad-0.9.2/datalad/support/external_versions.py
--rw-------   0 yoh      (47521) yoh      (47522)   142813 2018-03-04 16:37:40.000000 datalad-0.9.2/datalad/support/annexrepo.py
--rw-------   0 yoh      (47521) yoh      (47522)    14013 2018-03-04 16:37:40.000000 datalad-0.9.2/datalad/support/constraints.py
--rw-------   0 yoh      (47521) yoh      (47522)    81597 2018-03-04 16:37:40.000000 datalad-0.9.2/datalad/support/gitrepo.py
--rw-------   0 yoh      (47521) yoh      (47522)     2381 2018-03-04 16:37:40.000000 datalad-0.9.2/datalad/support/status.py
-drwx------   0 yoh      (47521) yoh      (47522)        0 2018-03-04 16:37:52.000000 datalad-0.9.2/datalad/support/third/
--rw-------   0 yoh      (47521) yoh      (47522)    13859 2018-03-04 16:37:40.000000 datalad-0.9.2/datalad/support/third/noseclasses.py
--rw-------   0 yoh      (47521) yoh      (47522)        0 2018-03-04 16:37:40.000000 datalad-0.9.2/datalad/support/third/__init__.py
--rw-------   0 yoh      (47521) yoh      (47522)    15888 2018-03-04 16:37:40.000000 datalad-0.9.2/datalad/support/third/nosetester.py
--rw-------   0 yoh      (47521) yoh      (47522)     3872 2018-03-04 16:37:40.000000 datalad-0.9.2/datalad/support/third/nda_aws_token_generator.py
--rw-------   0 yoh      (47521) yoh      (47522)     9015 2018-03-04 16:37:40.000000 datalad-0.9.2/datalad/support/protocol.py
--rw-------   0 yoh      (47521) yoh      (47522)     2313 2018-03-04 16:37:40.000000 datalad-0.9.2/datalad/support/nda_.py
--rw-------   0 yoh      (47521) yoh      (47522)     3055 2018-03-04 16:37:40.000000 datalad-0.9.2/datalad/support/cookies.py
--rw-------   0 yoh      (47521) yoh      (47522)      502 2018-03-04 16:37:40.000000 datalad-0.9.2/datalad/support/__init__.py
--rw-------   0 yoh      (47521) yoh      (47522)    17412 2018-03-04 16:37:40.000000 datalad-0.9.2/datalad/support/sshconnector.py
--rw-------   0 yoh      (47521) yoh      (47522)     2105 2018-03-04 16:37:40.000000 datalad-0.9.2/datalad/support/strings.py
--rw-------   0 yoh      (47521) yoh      (47522)     9770 2018-03-04 16:37:40.000000 datalad-0.9.2/datalad/support/exceptions.py
--rw-------   0 yoh      (47521) yoh      (47522)    30772 2018-03-04 16:37:40.000000 datalad-0.9.2/datalad/support/network.py
--rw-------   0 yoh      (47521) yoh      (47522)     6905 2018-03-04 16:37:40.000000 datalad-0.9.2/datalad/support/repo.py
--rw-------   0 yoh      (47521) yoh      (47522)     3413 2018-03-04 16:37:40.000000 datalad-0.9.2/datalad/support/vcr_.py
--rw-------   0 yoh      (47521) yoh      (47522)     2150 2018-03-04 16:37:40.000000 datalad-0.9.2/datalad/support/json_py.py
--rw-------   0 yoh      (47521) yoh      (47522)    14697 2018-03-04 16:37:40.000000 datalad-0.9.2/datalad/support/s3.py
--rw-------   0 yoh      (47521) yoh      (47522)     6114 2018-03-04 16:37:40.000000 datalad-0.9.2/datalad/support/configparserinc.py
--rw-------   0 yoh      (47521) yoh      (47522)     1454 2018-03-04 16:37:40.000000 datalad-0.9.2/datalad/support/ansi_colors.py
--rw-------   0 yoh      (47521) yoh      (47522)     1672 2018-03-04 16:37:40.000000 datalad-0.9.2/datalad/support/digests.py
--rw-------   0 yoh      (47521) yoh      (47522)    19407 2018-03-04 16:37:40.000000 datalad-0.9.2/datalad/support/archives.py
--rw-------   0 yoh      (47521) yoh      (47522)     6187 2018-03-04 16:37:40.000000 datalad-0.9.2/datalad/support/stats.py
--rw-------   0 yoh      (47521) yoh      (47522)     1111 2018-03-04 16:37:40.000000 datalad-0.9.2/datalad/support/cache.py
-drwx------   0 yoh      (47521) yoh      (47522)        0 2018-03-04 16:37:52.000000 datalad-0.9.2/datalad/crawler/
--rw-------   0 yoh      (47521) yoh      (47522)      504 2018-03-04 16:37:39.000000 datalad-0.9.2/datalad/crawler/base.py
-drwx------   0 yoh      (47521) yoh      (47522)        0 2018-03-04 16:37:52.000000 datalad-0.9.2/datalad/crawler/tests/
--rw-------   0 yoh      (47521) yoh      (47522)     9825 2018-03-04 16:37:39.000000 datalad-0.9.2/datalad/crawler/tests/test_pipeline.py
--rw-------   0 yoh      (47521) yoh      (47522)      566 2018-03-04 16:37:39.000000 datalad-0.9.2/datalad/crawler/tests/__init__.py
--rw-------   0 yoh      (47521) yoh      (47522)    21798 2018-03-04 16:37:39.000000 datalad-0.9.2/datalad/crawler/pipeline.py
-drwx------   0 yoh      (47521) yoh      (47522)        0 2018-03-04 16:37:52.000000 datalad-0.9.2/datalad/crawler/dbs/
--rw-------   0 yoh      (47521) yoh      (47522)     7153 2018-03-04 16:37:39.000000 datalad-0.9.2/datalad/crawler/dbs/base.py
-drwx------   0 yoh      (47521) yoh      (47522)        0 2018-03-04 16:37:52.000000 datalad-0.9.2/datalad/crawler/dbs/tests/
--rw-------   0 yoh      (47521) yoh      (47522)     5198 2018-03-04 16:37:39.000000 datalad-0.9.2/datalad/crawler/dbs/tests/test_files.py
--rw-------   0 yoh      (47521) yoh      (47522)      389 2018-03-04 16:37:39.000000 datalad-0.9.2/datalad/crawler/dbs/tests/__init__.py
--rw-------   0 yoh      (47521) yoh      (47522)     3141 2018-03-04 16:37:39.000000 datalad-0.9.2/datalad/crawler/dbs/versions.py
--rw-------   0 yoh      (47521) yoh      (47522)      461 2018-03-04 16:37:39.000000 datalad-0.9.2/datalad/crawler/dbs/__init__.py
--rw-------   0 yoh      (47521) yoh      (47522)     5217 2018-03-04 16:37:39.000000 datalad-0.9.2/datalad/crawler/dbs/files.py
-drwx------   0 yoh      (47521) yoh      (47522)        0 2018-03-04 16:37:52.000000 datalad-0.9.2/datalad/crawler/oldconfig/
--rw-------   0 yoh      (47521) yoh      (47522)     6357 2018-03-04 16:37:39.000000 datalad-0.9.2/datalad/crawler/oldconfig/base.py
-drwx------   0 yoh      (47521) yoh      (47522)        0 2018-03-04 16:37:52.000000 datalad-0.9.2/datalad/crawler/oldconfig/tests/
--rw-------   0 yoh      (47521) yoh      (47522)        0 2018-03-04 16:37:39.000000 datalad-0.9.2/datalad/crawler/oldconfig/tests/__init__.py
--rw-------   0 yoh      (47521) yoh      (47522)     2082 2018-03-04 16:37:39.000000 datalad-0.9.2/datalad/crawler/oldconfig/tests/test_config.py
--rw-------   0 yoh      (47521) yoh      (47522)      516 2018-03-04 16:37:39.000000 datalad-0.9.2/datalad/crawler/oldconfig/__init__.py
-drwx------   0 yoh      (47521) yoh      (47522)        0 2018-03-04 16:37:52.000000 datalad-0.9.2/datalad/crawler/nodes/
-drwx------   0 yoh      (47521) yoh      (47522)        0 2018-03-04 16:37:52.000000 datalad-0.9.2/datalad/crawler/nodes/tests/
--rw-------   0 yoh      (47521) yoh      (47522)    16493 2018-03-04 16:37:39.000000 datalad-0.9.2/datalad/crawler/nodes/tests/test_annex.py
--rw-------   0 yoh      (47521) yoh      (47522)     4261 2018-03-04 16:37:39.000000 datalad-0.9.2/datalad/crawler/nodes/tests/test_matches.py
--rw-------   0 yoh      (47521) yoh      (47522)     9340 2018-03-04 16:37:39.000000 datalad-0.9.2/datalad/crawler/nodes/tests/test_s3.py
--rw-------   0 yoh      (47521) yoh      (47522)    17177 2018-03-04 16:37:39.000000 datalad-0.9.2/datalad/crawler/nodes/tests/test_misc.py
--rw-------   0 yoh      (47521) yoh      (47522)      501 2018-03-04 16:37:39.000000 datalad-0.9.2/datalad/crawler/nodes/tests/__init__.py
--rw-------   0 yoh      (47521) yoh      (47522)     2973 2018-03-04 16:37:39.000000 datalad-0.9.2/datalad/crawler/nodes/tests/test_crawl_url.py
--rw-------   0 yoh      (47521) yoh      (47522)     6822 2018-03-04 16:37:39.000000 datalad-0.9.2/datalad/crawler/nodes/crawl_url.py
--rw-------   0 yoh      (47521) yoh      (47522)    67617 2018-03-04 16:37:39.000000 datalad-0.9.2/datalad/crawler/nodes/annex.py
--rw-------   0 yoh      (47521) yoh      (47522)      894 2018-03-04 16:37:39.000000 datalad-0.9.2/datalad/crawler/nodes/__init__.py
--rw-------   0 yoh      (47521) yoh      (47522)    18482 2018-03-04 16:37:39.000000 datalad-0.9.2/datalad/crawler/nodes/misc.py
--rw-------   0 yoh      (47521) yoh      (47522)    12951 2018-03-04 16:37:39.000000 datalad-0.9.2/datalad/crawler/nodes/s3.py
--rw-------   0 yoh      (47521) yoh      (47522)     7386 2018-03-04 16:37:39.000000 datalad-0.9.2/datalad/crawler/nodes/matches.py
--rw-------   0 yoh      (47521) yoh      (47522)      504 2018-03-04 16:37:39.000000 datalad-0.9.2/datalad/crawler/__init__.py
-drwx------   0 yoh      (47521) yoh      (47522)        0 2018-03-04 16:37:52.000000 datalad-0.9.2/datalad/crawler/pipelines/
-drwx------   0 yoh      (47521) yoh      (47522)        0 2018-03-04 16:37:52.000000 datalad-0.9.2/datalad/crawler/pipelines/tests/
--rw-------   0 yoh      (47521) yoh      (47522)     1065 2018-03-04 16:37:39.000000 datalad-0.9.2/datalad/crawler/pipelines/tests/test_nda.py
--rw-------   0 yoh      (47521) yoh      (47522)     2948 2018-03-04 16:37:39.000000 datalad-0.9.2/datalad/crawler/pipelines/tests/test_openfmri_collection.py
--rw-------   0 yoh      (47521) yoh      (47522)     3398 2018-03-04 16:37:39.000000 datalad-0.9.2/datalad/crawler/pipelines/tests/test_simple_s3.py
--rw-------   0 yoh      (47521) yoh      (47522)     3153 2018-03-04 16:37:39.000000 datalad-0.9.2/datalad/crawler/pipelines/tests/test_fcptable.py
--rw-------   0 yoh      (47521) yoh      (47522)      177 2018-03-04 16:37:39.000000 datalad-0.9.2/datalad/crawler/pipelines/tests/__init__.py
--rw-------   0 yoh      (47521) yoh      (47522)    24487 2018-03-04 16:37:39.000000 datalad-0.9.2/datalad/crawler/pipelines/tests/test_openfmri.py
--rw-------   0 yoh      (47521) yoh      (47522)     2889 2018-03-04 16:37:39.000000 datalad-0.9.2/datalad/crawler/pipelines/tests/test_simple_with_archives.py
--rw-------   0 yoh      (47521) yoh      (47522)      920 2018-03-04 16:37:39.000000 datalad-0.9.2/datalad/crawler/pipelines/tests/utils.py
--rw-------   0 yoh      (47521) yoh      (47522)     1847 2018-03-04 16:37:39.000000 datalad-0.9.2/datalad/crawler/pipelines/tests/test_crcns.py
--rw-------   0 yoh      (47521) yoh      (47522)    12480 2018-03-04 16:37:39.000000 datalad-0.9.2/datalad/crawler/pipelines/tests/test_balsa.py
--rw-------   0 yoh      (47521) yoh      (47522)    11087 2018-03-04 16:37:39.000000 datalad-0.9.2/datalad/crawler/pipelines/crcns.py
--rw-------   0 yoh      (47521) yoh      (47522)    14323 2018-03-04 16:37:39.000000 datalad-0.9.2/datalad/crawler/pipelines/openfmri.py
--rw-------   0 yoh      (47521) yoh      (47522)     1086 2018-03-04 16:37:39.000000 datalad-0.9.2/datalad/crawler/pipelines/template.py
--rw-------   0 yoh      (47521) yoh      (47522)     9920 2018-03-04 16:37:39.000000 datalad-0.9.2/datalad/crawler/pipelines/balsa.py
--rw-------   0 yoh      (47521) yoh      (47522)     4569 2018-03-04 16:37:39.000000 datalad-0.9.2/datalad/crawler/pipelines/simple_with_archives.py
--rw-------   0 yoh      (47521) yoh      (47522)      458 2018-03-04 16:37:39.000000 datalad-0.9.2/datalad/crawler/pipelines/__init__.py
--rw-------   0 yoh      (47521) yoh      (47522)     4163 2018-03-04 16:37:39.000000 datalad-0.9.2/datalad/crawler/pipelines/openfmri_s3.py
--rw-------   0 yoh      (47521) yoh      (47522)     3173 2018-03-04 16:37:39.000000 datalad-0.9.2/datalad/crawler/pipelines/abstractsonline.py
--rw-------   0 yoh      (47521) yoh      (47522)     6061 2018-03-04 16:37:39.000000 datalad-0.9.2/datalad/crawler/pipelines/simple_s3.py
--rw-------   0 yoh      (47521) yoh      (47522)     6072 2018-03-04 16:37:39.000000 datalad-0.9.2/datalad/crawler/pipelines/nda.py
--rw-------   0 yoh      (47521) yoh      (47522)     7165 2018-03-04 16:37:39.000000 datalad-0.9.2/datalad/crawler/pipelines/fcptable.py
--rw-------   0 yoh      (47521) yoh      (47522)     2393 2018-03-04 16:37:39.000000 datalad-0.9.2/datalad/consts.py
--rw-------   0 yoh      (47521) yoh      (47522)     6941 2018-03-04 16:37:39.000000 datalad-0.9.2/datalad/__init__.py
-drwx------   0 yoh      (47521) yoh      (47522)        0 2018-03-04 16:37:52.000000 datalad-0.9.2/datalad/ui/
--rw-------   0 yoh      (47521) yoh      (47522)     1170 2018-03-04 16:37:40.000000 datalad-0.9.2/datalad/ui/base.py
-drwx------   0 yoh      (47521) yoh      (47522)        0 2018-03-04 16:37:52.000000 datalad-0.9.2/datalad/ui/tests/
--rw-------   0 yoh      (47521) yoh      (47522)     2512 2018-03-04 16:37:40.000000 datalad-0.9.2/datalad/ui/tests/test_base.py
--rw-------   0 yoh      (47521) yoh      (47522)     3824 2018-03-04 16:37:40.000000 datalad-0.9.2/datalad/ui/tests/test_dialog.py
--rw-------   0 yoh      (47521) yoh      (47522)      442 2018-03-04 16:37:40.000000 datalad-0.9.2/datalad/ui/tests/__init__.py
--rw-------   0 yoh      (47521) yoh      (47522)    10191 2018-03-04 16:37:40.000000 datalad-0.9.2/datalad/ui/dialog.py
--rw-------   0 yoh      (47521) yoh      (47522)     2673 2018-03-04 16:37:40.000000 datalad-0.9.2/datalad/ui/__init__.py
--rw-------   0 yoh      (47521) yoh      (47522)     1633 2018-03-04 16:37:40.000000 datalad-0.9.2/datalad/ui/utils.py
--rw-------   0 yoh      (47521) yoh      (47522)     6123 2018-03-04 16:37:40.000000 datalad-0.9.2/datalad/ui/progressbars.py
-drwx------   0 yoh      (47521) yoh      (47522)        0 2018-03-04 16:37:52.000000 datalad-0.9.2/datalad/downloaders/
--rw-------   0 yoh      (47521) yoh      (47522)    22303 2018-03-04 16:37:40.000000 datalad-0.9.2/datalad/downloaders/base.py
-drwx------   0 yoh      (47521) yoh      (47522)        0 2018-03-04 16:37:52.000000 datalad-0.9.2/datalad/downloaders/tests/
--rw-------   0 yoh      (47521) yoh      (47522)      454 2018-03-04 16:37:40.000000 datalad-0.9.2/datalad/downloaders/tests/test_base.py
--rw-------   0 yoh      (47521) yoh      (47522)     4629 2018-03-04 16:37:40.000000 datalad-0.9.2/datalad/downloaders/tests/test_credentials.py
--rw-------   0 yoh      (47521) yoh      (47522)     4533 2018-03-04 16:37:40.000000 datalad-0.9.2/datalad/downloaders/tests/test_s3.py
--rw-------   0 yoh      (47521) yoh      (47522)        0 2018-03-04 16:37:40.000000 datalad-0.9.2/datalad/downloaders/tests/__init__.py
--rw-------   0 yoh      (47521) yoh      (47522)     1241 2018-03-04 16:37:40.000000 datalad-0.9.2/datalad/downloaders/tests/utils.py
--rw-------   0 yoh      (47521) yoh      (47522)     3508 2018-03-04 16:37:40.000000 datalad-0.9.2/datalad/downloaders/tests/test_providers.py
--rw-------   0 yoh      (47521) yoh      (47522)    18778 2018-03-04 16:37:40.000000 datalad-0.9.2/datalad/downloaders/tests/test_http.py
--rw-------   0 yoh      (47521) yoh      (47522)    20844 2018-03-04 16:37:40.000000 datalad-0.9.2/datalad/downloaders/http.py
-drwx------   0 yoh      (47521) yoh      (47522)        0 2018-03-04 16:37:52.000000 datalad-0.9.2/datalad/downloaders/configs/
--rw-------   0 yoh      (47521) yoh      (47522)      350 2018-03-04 16:37:40.000000 datalad-0.9.2/datalad/downloaders/configs/openfmri.cfg
--rw-------   0 yoh      (47521) yoh      (47522)      883 2018-03-04 16:37:40.000000 datalad-0.9.2/datalad/downloaders/configs/nda.cfg
--rw-------   0 yoh      (47521) yoh      (47522)     1633 2018-03-04 16:37:40.000000 datalad-0.9.2/datalad/downloaders/configs/nitrc.cfg
--rw-------   0 yoh      (47521) yoh      (47522)      203 2018-03-04 16:37:40.000000 datalad-0.9.2/datalad/downloaders/configs/indi.cfg
--rw-------   0 yoh      (47521) yoh      (47522)     1801 2018-03-04 16:37:40.000000 datalad-0.9.2/datalad/downloaders/configs/crcns.cfg
--rw-------   0 yoh      (47521) yoh      (47522)      594 2018-03-04 16:37:40.000000 datalad-0.9.2/datalad/downloaders/configs/kaggle.cfg
--rw-------   0 yoh      (47521) yoh      (47522)      289 2018-03-04 16:37:40.000000 datalad-0.9.2/datalad/downloaders/configs/providers.cfg
--rw-------   0 yoh      (47521) yoh      (47522)     1874 2018-03-04 16:37:40.000000 datalad-0.9.2/datalad/downloaders/configs/hcp.cfg
--rw-------   0 yoh      (47521) yoh      (47522)      200 2018-03-04 16:37:40.000000 datalad-0.9.2/datalad/downloaders/configs/crawdad.cfg
--rw-------   0 yoh      (47521) yoh      (47522)    14362 2018-03-04 16:37:40.000000 datalad-0.9.2/datalad/downloaders/providers.py
--rw-------   0 yoh      (47521) yoh      (47522)      744 2018-03-04 16:37:40.000000 datalad-0.9.2/datalad/downloaders/__init__.py
--rw-------   0 yoh      (47521) yoh      (47522)     9280 2018-03-04 16:37:40.000000 datalad-0.9.2/datalad/downloaders/s3.py
--rw-------   0 yoh      (47521) yoh      (47522)    10938 2018-03-04 16:37:40.000000 datalad-0.9.2/datalad/downloaders/credentials.py
--rw-------   0 yoh      (47521) yoh      (47522)     3069 2018-03-04 16:37:39.000000 datalad-0.9.2/datalad/api.py
-drwx------   0 yoh      (47521) yoh      (47522)        0 2018-03-04 16:37:52.000000 datalad-0.9.2/datalad/metadata/
-drwx------   0 yoh      (47521) yoh      (47522)        0 2018-03-04 16:37:52.000000 datalad-0.9.2/datalad/metadata/tests/
--rw-------   0 yoh      (47521) yoh      (47522)    15618 2018-03-04 16:37:40.000000 datalad-0.9.2/datalad/metadata/tests/test_base.py
--rw-------   0 yoh      (47521) yoh      (47522)    10395 2018-03-04 16:37:40.000000 datalad-0.9.2/datalad/metadata/tests/test_manipulation.py
--rw-------   0 yoh      (47521) yoh      (47522)     6231 2018-03-04 16:37:40.000000 datalad-0.9.2/datalad/metadata/tests/test_search.py
--rw-------   0 yoh      (47521) yoh      (47522)        0 2018-03-04 16:37:40.000000 datalad-0.9.2/datalad/metadata/tests/__init__.py
--rw-------   0 yoh      (47521) yoh      (47522)     9176 2018-03-04 16:37:40.000000 datalad-0.9.2/datalad/metadata/aggregate.py
-drwx------   0 yoh      (47521) yoh      (47522)        0 2018-03-04 16:37:52.000000 datalad-0.9.2/datalad/metadata/parsers/
--rw-------   0 yoh      (47521) yoh      (47522)     2359 2018-03-04 16:37:40.000000 datalad-0.9.2/datalad/metadata/parsers/base.py
-drwx------   0 yoh      (47521) yoh      (47522)        0 2018-03-04 16:37:52.000000 datalad-0.9.2/datalad/metadata/parsers/tests/
--rw-------   0 yoh      (47521) yoh      (47522)     2935 2018-03-04 16:37:40.000000 datalad-0.9.2/datalad/metadata/parsers/tests/test_datacite_xml.py
--rw-------   0 yoh      (47521) yoh      (47522)     2866 2018-03-04 16:37:40.000000 datalad-0.9.2/datalad/metadata/parsers/tests/test_frictionless_datapackage.py
--rw-------   0 yoh      (47521) yoh      (47522)      412 2018-03-04 16:37:40.000000 datalad-0.9.2/datalad/metadata/parsers/tests/__init__.py
--rw-------   0 yoh      (47521) yoh      (47522)     3457 2018-03-04 16:37:40.000000 datalad-0.9.2/datalad/metadata/parsers/tests/test_rfc822.py
--rw-------   0 yoh      (47521) yoh      (47522)     1406 2018-03-04 16:37:40.000000 datalad-0.9.2/datalad/metadata/parsers/tests/test_aggregate.py
--rw-------   0 yoh      (47521) yoh      (47522)     3810 2018-03-04 16:37:40.000000 datalad-0.9.2/datalad/metadata/parsers/tests/test_bids.py
--rw-------   0 yoh      (47521) yoh      (47522)     3628 2018-03-04 16:37:40.000000 datalad-0.9.2/datalad/metadata/parsers/datalad_rfc822.py
--rw-------   0 yoh      (47521) yoh      (47522)     3755 2018-03-04 16:37:40.000000 datalad-0.9.2/datalad/metadata/parsers/aggregate.py
--rw-------   0 yoh      (47521) yoh      (47522)     2279 2018-03-04 16:37:40.000000 datalad-0.9.2/datalad/metadata/parsers/frictionless_datapackage.py
--rw-------   0 yoh      (47521) yoh      (47522)      619 2018-03-04 16:37:40.000000 datalad-0.9.2/datalad/metadata/parsers/__init__.py
--rw-------   0 yoh      (47521) yoh      (47522)     4027 2018-03-04 16:37:40.000000 datalad-0.9.2/datalad/metadata/parsers/datacite.py
--rw-------   0 yoh      (47521) yoh      (47522)     2750 2018-03-04 16:37:40.000000 datalad-0.9.2/datalad/metadata/parsers/bids.py
--rw-------   0 yoh      (47521) yoh      (47522)    11907 2018-03-04 16:37:40.000000 datalad-0.9.2/datalad/metadata/__init__.py
--rw-------   0 yoh      (47521) yoh      (47522)    20478 2018-03-04 16:37:40.000000 datalad-0.9.2/datalad/metadata/metadata.py
--rw-------   0 yoh      (47521) yoh      (47522)    17723 2018-03-04 16:37:40.000000 datalad-0.9.2/datalad/metadata/search.py
--rw-------   0 yoh      (47521) yoh      (47522)    42364 2018-03-04 16:37:40.000000 datalad-0.9.2/datalad/utils.py
-drwx------   0 yoh      (47521) yoh      (47522)        0 2018-03-04 16:37:52.000000 datalad-0.9.2/datalad/distribution/
-drwx------   0 yoh      (47521) yoh      (47522)        0 2018-03-04 16:37:52.000000 datalad-0.9.2/datalad/distribution/tests/
--rw-------   0 yoh      (47521) yoh      (47522)    22962 2018-03-04 16:37:40.000000 datalad-0.9.2/datalad/distribution/tests/test_create_sibling.py
--rw-------   0 yoh      (47521) yoh      (47522)    13503 2018-03-04 16:37:40.000000 datalad-0.9.2/datalad/distribution/tests/test_update.py
--rw-------   0 yoh      (47521) yoh      (47522)     3276 2018-03-04 16:37:40.000000 datalad-0.9.2/datalad/distribution/tests/test_create_github.py
--rw-------   0 yoh      (47521) yoh      (47522)     3143 2018-03-04 16:37:40.000000 datalad-0.9.2/datalad/distribution/tests/test_create_test_dataset.py
--rw-------   0 yoh      (47521) yoh      (47522)     2908 2018-03-04 16:37:40.000000 datalad-0.9.2/datalad/distribution/tests/test_utils.py
--rw-------   0 yoh      (47521) yoh      (47522)     1569 2018-03-04 16:37:40.000000 datalad-0.9.2/datalad/distribution/tests/test_dataset_binding.py
--rw-------   0 yoh      (47521) yoh      (47522)     6735 2018-03-04 16:37:40.000000 datalad-0.9.2/datalad/distribution/tests/test_subdataset.py
--rw-------   0 yoh      (47521) yoh      (47522)    27076 2018-03-04 16:37:40.000000 datalad-0.9.2/datalad/distribution/tests/test_publish.py
--rw-------   0 yoh      (47521) yoh      (47522)    10489 2018-03-04 16:37:40.000000 datalad-0.9.2/datalad/distribution/tests/test_dataset.py
--rw-------   0 yoh      (47521) yoh      (47522)    33997 2018-03-04 16:37:40.000000 datalad-0.9.2/datalad/distribution/tests/test_install.py
--rw-------   0 yoh      (47521) yoh      (47522)      452 2018-03-04 16:37:40.000000 datalad-0.9.2/datalad/distribution/tests/__init__.py
--rw-------   0 yoh      (47521) yoh      (47522)    19339 2018-03-04 16:37:40.000000 datalad-0.9.2/datalad/distribution/tests/test_get.py
--rw-------   0 yoh      (47521) yoh      (47522)     9059 2018-03-04 16:37:40.000000 datalad-0.9.2/datalad/distribution/tests/test_siblings.py
--rw-------   0 yoh      (47521) yoh      (47522)    19550 2018-03-04 16:37:40.000000 datalad-0.9.2/datalad/distribution/tests/test_uninstall.py
--rw-------   0 yoh      (47521) yoh      (47522)    11123 2018-03-04 16:37:40.000000 datalad-0.9.2/datalad/distribution/tests/test_create.py
--rw-------   0 yoh      (47521) yoh      (47522)     1277 2018-03-04 16:37:40.000000 datalad-0.9.2/datalad/distribution/tests/test_dataset_config.py
--rw-------   0 yoh      (47521) yoh      (47522)    12543 2018-03-04 16:37:40.000000 datalad-0.9.2/datalad/distribution/tests/test_clone.py
--rw-------   0 yoh      (47521) yoh      (47522)    13433 2018-03-04 16:37:40.000000 datalad-0.9.2/datalad/distribution/tests/test_add.py
--rw-------   0 yoh      (47521) yoh      (47522)    36899 2018-03-04 16:37:40.000000 datalad-0.9.2/datalad/distribution/publish.py
--rw-------   0 yoh      (47521) yoh      (47522)    34419 2018-03-04 16:37:40.000000 datalad-0.9.2/datalad/distribution/create_sibling.py
--rw-------   0 yoh      (47521) yoh      (47522)    17452 2018-03-04 16:37:40.000000 datalad-0.9.2/datalad/distribution/subdatasets.py
--rw-------   0 yoh      (47521) yoh      (47522)    33694 2018-03-04 16:37:40.000000 datalad-0.9.2/datalad/distribution/siblings.py
--rw-------   0 yoh      (47521) yoh      (47522)    14812 2018-03-04 16:37:40.000000 datalad-0.9.2/datalad/distribution/remove.py
--rw-------   0 yoh      (47521) yoh      (47522)     1032 2018-03-04 16:37:40.000000 datalad-0.9.2/datalad/distribution/add_sibling.py
--rw-------   0 yoh      (47521) yoh      (47522)     6562 2018-03-04 16:37:40.000000 datalad-0.9.2/datalad/distribution/create_test_dataset.py
--rw-------   0 yoh      (47521) yoh      (47522)    15482 2018-03-04 16:37:40.000000 datalad-0.9.2/datalad/distribution/create_sibling_github.py
--rw-------   0 yoh      (47521) yoh      (47522)    19940 2018-03-04 16:37:40.000000 datalad-0.9.2/datalad/distribution/install.py
--rw-------   0 yoh      (47521) yoh      (47522)     8221 2018-03-04 16:37:40.000000 datalad-0.9.2/datalad/distribution/drop.py
--rw-------   0 yoh      (47521) yoh      (47522)     8996 2018-03-04 16:37:40.000000 datalad-0.9.2/datalad/distribution/uninstall.py
--rw-------   0 yoh      (47521) yoh      (47522)    18620 2018-03-04 16:37:40.000000 datalad-0.9.2/datalad/distribution/dataset.py
--rw-------   0 yoh      (47521) yoh      (47522)    29405 2018-03-04 16:37:40.000000 datalad-0.9.2/datalad/distribution/get.py
--rw-------   0 yoh      (47521) yoh      (47522)      498 2018-03-04 16:37:39.000000 datalad-0.9.2/datalad/distribution/__init__.py
--rw-------   0 yoh      (47521) yoh      (47522)    11979 2018-03-04 16:37:40.000000 datalad-0.9.2/datalad/distribution/clone.py
--rw-------   0 yoh      (47521) yoh      (47522)     8479 2018-03-04 16:37:40.000000 datalad-0.9.2/datalad/distribution/update.py
--rw-------   0 yoh      (47521) yoh      (47522)    24603 2018-03-04 16:37:40.000000 datalad-0.9.2/datalad/distribution/add.py
--rw-------   0 yoh      (47521) yoh      (47522)     8057 2018-03-04 16:37:40.000000 datalad-0.9.2/datalad/distribution/utils.py
--rw-------   0 yoh      (47521) yoh      (47522)    16929 2018-03-04 16:37:40.000000 datalad-0.9.2/datalad/distribution/create.py
-drwx------   0 yoh      (47521) yoh      (47522)        0 2018-03-04 16:37:52.000000 datalad-0.9.2/datalad/cmdline/
-drwx------   0 yoh      (47521) yoh      (47522)        0 2018-03-04 16:37:52.000000 datalad-0.9.2/datalad/cmdline/tests/
--rw-------   0 yoh      (47521) yoh      (47522)      448 2018-03-04 16:37:39.000000 datalad-0.9.2/datalad/cmdline/tests/__init__.py
--rw-------   0 yoh      (47521) yoh      (47522)     2744 2018-03-04 16:37:39.000000 datalad-0.9.2/datalad/cmdline/tests/test_helpers.py
--rw-------   0 yoh      (47521) yoh      (47522)     3101 2018-03-04 16:37:39.000000 datalad-0.9.2/datalad/cmdline/tests/test_formatters.py
--rw-------   0 yoh      (47521) yoh      (47522)     8463 2018-03-04 16:37:39.000000 datalad-0.9.2/datalad/cmdline/tests/test_main.py
--rw-------   0 yoh      (47521) yoh      (47522)     9146 2018-03-04 16:37:39.000000 datalad-0.9.2/datalad/cmdline/helpers.py
--rw-------   0 yoh      (47521) yoh      (47522)     2242 2018-03-04 16:37:39.000000 datalad-0.9.2/datalad/cmdline/common_args.py
--rw-------   0 yoh      (47521) yoh      (47522)    17916 2018-03-04 16:37:39.000000 datalad-0.9.2/datalad/cmdline/main.py
--rw-------   0 yoh      (47521) yoh      (47522)      433 2018-03-04 16:37:39.000000 datalad-0.9.2/datalad/cmdline/__init__.py
--rw-------   0 yoh      (47521) yoh      (47522)     2090 2018-03-04 16:37:40.000000 datalad-0.9.2/datalad/version.py
--rw-------   0 yoh      (47521) yoh      (47522)    10543 2018-03-04 16:37:40.000000 datalad-0.9.2/datalad/dochelpers.py
--rw-------   0 yoh      (47521) yoh      (47522)    26600 2018-03-04 16:37:39.000000 datalad-0.9.2/datalad/cmd.py
--rwx------   0 yoh      (47521) yoh      (47522)     5843 2018-03-04 16:37:40.000000 datalad-0.9.2/setup.py
+drwx------   0 yoh      (47521) yoh      (47522)        0 2018-03-16 22:27:17.000000 datalad-0.9.3/
+-rw-------   0 yoh      (47521) yoh      (47522)    10556 2018-03-04 16:37:40.000000 datalad-0.9.3/setup_support.py
+-rw-------   0 yoh      (47521) yoh      (47522)      234 2018-03-04 16:37:39.000000 datalad-0.9.3/CONTRIBUTORS
+-rw-------   0 yoh      (47521) yoh      (47522)    10538 2018-03-16 22:26:59.000000 datalad-0.9.3/.travis.yml
+-rw-------   0 yoh      (47521) yoh      (47522)     1008 2018-03-04 16:37:39.000000 datalad-0.9.3/Makefile
+drwx------   0 yoh      (47521) yoh      (47522)        0 2018-03-16 22:27:17.000000 datalad-0.9.3/docs/
+-rw-------   0 yoh      (47521) yoh      (47522)     7442 2018-03-04 16:37:40.000000 datalad-0.9.3/docs/Makefile
+-rw-------   0 yoh      (47521) yoh      (47522)     2183 2018-03-04 16:37:40.000000 datalad-0.9.3/docs/config-format.rst
+-rw-------   0 yoh      (47521) yoh      (47522)    21350 2018-03-04 16:37:40.000000 datalad-0.9.3/docs/design.rst
+-rw-------   0 yoh      (47521) yoh      (47522)     5594 2018-03-04 16:37:40.000000 datalad-0.9.3/docs/datalad-metadata.rst
+drwx------   0 yoh      (47521) yoh      (47522)        0 2018-03-16 22:27:17.000000 datalad-0.9.3/docs/examples/
+-rwx------   0 yoh      (47521) yoh      (47522)    12911 2018-03-04 16:37:40.000000 datalad-0.9.3/docs/examples/nipype_workshop_dataset.sh
+-rwx------   0 yoh      (47521) yoh      (47522)     2222 2018-03-04 16:37:40.000000 datalad-0.9.3/docs/examples/make_pymvpa_collection.sh_broken
+-rwx------   0 yoh      (47521) yoh      (47522)     1106 2018-03-04 16:37:40.000000 datalad-0.9.3/docs/examples/make_large_bogus_collection.sh_broken
+-rw-------   0 yoh      (47521) yoh      (47522)    10504 2018-03-04 16:37:40.000000 datalad-0.9.3/docs/examples/3rdparty_analysis_workflow.sh
+drwx------   0 yoh      (47521) yoh      (47522)        0 2018-03-16 22:27:17.000000 datalad-0.9.3/docs/casts/
+-rw-------   0 yoh      (47521) yoh      (47522)     3262 2018-03-04 16:37:40.000000 datalad-0.9.3/docs/casts/boxcom.sh
+-rw-------   0 yoh      (47521) yoh      (47522)     1738 2018-03-04 16:37:40.000000 datalad-0.9.3/docs/casts/seamless_nested_repos.sh
+-rw-------   0 yoh      (47521) yoh      (47522)     1990 2018-03-04 16:37:40.000000 datalad-0.9.3/docs/casts/simple_provenance_tracking.sh
+-rw-------   0 yoh      (47521) yoh      (47522)     3120 2018-03-04 16:37:40.000000 datalad-0.9.3/docs/casts/publish_on_github.sh
+-rw-------   0 yoh      (47521) yoh      (47522)     2621 2018-03-04 16:37:40.000000 datalad-0.9.3/docs/casts/basic_search.sh
+-rw-------   0 yoh      (47521) yoh      (47522)     1743 2018-03-04 16:37:40.000000 datalad-0.9.3/docs/casts/track_data_from_webpage.sh
+-rwx------   0 yoh      (47521) yoh      (47522)     1128 2018-03-04 16:37:40.000000 datalad-0.9.3/docs/casts/cmdline_basic_usage.sh
+-rw-------   0 yoh      (47521) yoh      (47522)     4925 2018-03-04 16:37:40.000000 datalad-0.9.3/docs/casts/reproducible_analysis.sh
+-rw-------   0 yoh      (47521) yoh      (47522)     5459 2018-03-04 16:37:40.000000 datalad-0.9.3/docs/casts/heudiconv_dicom_to_bids.sh
+drwx------   0 yoh      (47521) yoh      (47522)        0 2018-03-16 22:27:17.000000 datalad-0.9.3/docs/source/
+-rw-------   0 yoh      (47521) yoh      (47522)     4781 2018-03-04 16:37:40.000000 datalad-0.9.3/docs/source/customization.rst
+-rw-------   0 yoh      (47521) yoh      (47522)      738 2018-03-04 16:37:40.000000 datalad-0.9.3/docs/source/index.rst
+-rw-------   0 yoh      (47521) yoh      (47522)    22788 2018-03-04 16:37:40.000000 datalad-0.9.3/docs/source/changelog.rst
+drwx------   0 yoh      (47521) yoh      (47522)        0 2018-03-16 22:27:17.000000 datalad-0.9.3/docs/source/_extras/
+-rw-------   0 yoh      (47521) yoh      (47522)     1105 2018-03-04 16:37:40.000000 datalad-0.9.3/docs/source/_extras/schema.json
+-rw-------   0 yoh      (47521) yoh      (47522)     1717 2018-03-04 16:37:40.000000 datalad-0.9.3/docs/source/glossary.rst
+-rw-------   0 yoh      (47521) yoh      (47522)     3060 2018-03-04 16:37:40.000000 datalad-0.9.3/docs/source/gettingstarted.rst
+drwx------   0 yoh      (47521) yoh      (47522)        0 2018-03-16 22:27:17.000000 datalad-0.9.3/docs/source/usecases/
+-rw-------   0 yoh      (47521) yoh      (47522)      185 2018-03-04 16:37:40.000000 datalad-0.9.3/docs/source/usecases/index.rst
+-rw-------   0 yoh      (47521) yoh      (47522)     6446 2018-03-04 16:37:40.000000 datalad-0.9.3/docs/source/metadata.rst
+-rw-------   0 yoh      (47521) yoh      (47522)     1744 2018-03-04 16:37:40.000000 datalad-0.9.3/docs/source/config.rst
+-rw-------   0 yoh      (47521) yoh      (47522)     2568 2018-03-04 16:37:40.000000 datalad-0.9.3/docs/source/modref.rst
+drwx------   0 yoh      (47521) yoh      (47522)        0 2018-03-16 22:27:17.000000 datalad-0.9.3/docs/source/crawler/
+-rw-------   0 yoh      (47521) yoh      (47522)      361 2018-03-04 16:37:40.000000 datalad-0.9.3/docs/source/crawler/index.rst
+-rw-------   0 yoh      (47521) yoh      (47522)     2806 2018-03-04 16:37:40.000000 datalad-0.9.3/docs/source/crawler/basics.rst
+drwx------   0 yoh      (47521) yoh      (47522)        0 2018-03-16 22:27:17.000000 datalad-0.9.3/docs/source/_templates/
+drwx------   0 yoh      (47521) yoh      (47522)        0 2018-03-16 22:27:17.000000 datalad-0.9.3/docs/source/_templates/autosummary/
+-rw-------   0 yoh      (47521) yoh      (47522)      436 2018-03-04 16:37:40.000000 datalad-0.9.3/docs/source/_templates/autosummary/module.rst
+-rw-------   0 yoh      (47521) yoh      (47522)      859 2018-03-04 16:37:40.000000 datalad-0.9.3/docs/source/acknowledgements.rst
+-rw-------   0 yoh      (47521) yoh      (47522)    10163 2018-03-04 16:37:40.000000 datalad-0.9.3/docs/source/conf.py
+-rw-------   0 yoh      (47521) yoh      (47522)     8801 2018-03-04 16:37:40.000000 datalad-0.9.3/docs/source/basics.rst
+drwx------   0 yoh      (47521) yoh      (47522)        0 2018-03-16 22:27:17.000000 datalad-0.9.3/docs/source/_static/
+-rw-------   0 yoh      (47521) yoh      (47522)      958 2018-03-04 16:37:40.000000 datalad-0.9.3/docs/source/_static/datalad_logo.png
+-rw-------   0 yoh      (47521) yoh      (47522)     1040 2018-03-04 16:37:40.000000 datalad-0.9.3/docs/source/faq.rst
+-rw-------   0 yoh      (47521) yoh      (47522)     6547 2018-03-04 16:37:40.000000 datalad-0.9.3/docs/source/related.rst
+-rw-------   0 yoh      (47521) yoh      (47522)     1725 2018-03-04 16:37:40.000000 datalad-0.9.3/docs/source/cmdline.rst
+-rw-------   0 yoh      (47521) yoh      (47522)     5942 2018-03-04 16:37:40.000000 datalad-0.9.3/docs/source/background.rst
+-rw-------   0 yoh      (47521) yoh      (47522)     9167 2018-03-16 22:27:17.000000 datalad-0.9.3/PKG-INFO
+drwx------   0 yoh      (47521) yoh      (47522)        0 2018-03-16 22:27:17.000000 datalad-0.9.3/.github/
+-rw-------   0 yoh      (47521) yoh      (47522)      163 2018-03-04 16:37:39.000000 datalad-0.9.3/.github/PULL_REQUEST_TEMPLATE.md
+-rw-------   0 yoh      (47521) yoh      (47522)      430 2018-03-04 16:37:39.000000 datalad-0.9.3/.github/issue_template.md
+-rw-------   0 yoh      (47521) yoh      (47522)      295 2018-03-04 16:37:39.000000 datalad-0.9.3/Gruntfile.js
+-rw-------   0 yoh      (47521) yoh      (47522)     1404 2018-03-04 16:37:40.000000 datalad-0.9.3/tox.ini
+-rw-------   0 yoh      (47521) yoh      (47522)      367 2018-03-04 16:37:40.000000 datalad-0.9.3/requirements.txt
+drwx------   0 yoh      (47521) yoh      (47522)        0 2018-03-16 22:27:17.000000 datalad-0.9.3/tools/
+-rwx------   0 yoh      (47521) yoh      (47522)     4562 2018-03-04 16:37:40.000000 datalad-0.9.3/tools/mimic_repo
+-rw-------   0 yoh      (47521) yoh      (47522)      776 2018-03-04 16:37:40.000000 datalad-0.9.3/tools/cmdline-completion
+-rwx------   0 yoh      (47521) yoh      (47522)      751 2018-03-04 16:37:40.000000 datalad-0.9.3/tools/eval_under_testloopfs
+-rwx------   0 yoh      (47521) yoh      (47522)     2127 2018-03-04 16:37:40.000000 datalad-0.9.3/tools/git-web-submodules.sh
+drwx------   0 yoh      (47521) yoh      (47522)        0 2018-03-16 22:27:17.000000 datalad-0.9.3/tools/testing/
+-rwx------   0 yoh      (47521) yoh      (47522)     1931 2018-03-04 16:37:40.000000 datalad-0.9.3/tools/testing/test_README_in_docker
+-rwx------   0 yoh      (47521) yoh      (47522)     4134 2018-03-04 16:37:40.000000 datalad-0.9.3/tools/testing/start_website_in_docker
+-rwx------   0 yoh      (47521) yoh      (47522)      481 2018-03-04 16:37:40.000000 datalad-0.9.3/tools/testing/travis_ifdown_nonlo.sh
+-rw-------   0 yoh      (47521) yoh      (47522)     1285 2018-03-04 16:37:40.000000 datalad-0.9.3/tools/testing/test_README_in_docker-Dockerfile.in
+-rwx------   0 yoh      (47521) yoh      (47522)     1041 2018-03-04 16:37:40.000000 datalad-0.9.3/tools/testing/run_doc_examples
+-rw-------   0 yoh      (47521) yoh      (47522)       33 2018-03-04 16:37:40.000000 datalad-0.9.3/tools/testing/.gitignore
+-rwx------   0 yoh      (47521) yoh      (47522)     3457 2018-03-04 16:37:40.000000 datalad-0.9.3/tools/testing/make_test_repo
+-rw-------   0 yoh      (47521) yoh      (47522)     2633 2018-03-04 16:37:40.000000 datalad-0.9.3/tools/testing/start_website_in_docker-Dockerfile.in
+drwx------   0 yoh      (47521) yoh      (47522)        0 2018-03-16 22:27:17.000000 datalad-0.9.3/tools/testing/bad_internals/
+drwx------   0 yoh      (47521) yoh      (47522)        0 2018-03-16 22:27:17.000000 datalad-0.9.3/tools/testing/bad_internals/_scrapy/
+-rw-------   0 yoh      (47521) yoh      (47522)       57 2018-03-04 16:37:40.000000 datalad-0.9.3/tools/testing/bad_internals/_scrapy/scrapy.py
+drwx------   0 yoh      (47521) yoh      (47522)        0 2018-03-16 22:27:17.000000 datalad-0.9.3/tools/testing/conf/
+drwx------   0 yoh      (47521) yoh      (47522)        0 2018-03-16 22:27:17.000000 datalad-0.9.3/tools/testing/conf/etc/
+drwx------   0 yoh      (47521) yoh      (47522)        0 2018-03-16 22:27:17.000000 datalad-0.9.3/tools/testing/conf/etc/apt/
+drwx------   0 yoh      (47521) yoh      (47522)        0 2018-03-16 22:27:17.000000 datalad-0.9.3/tools/testing/conf/etc/apt/apt.conf.d/
+-rw-------   0 yoh      (47521) yoh      (47522)      112 2018-03-04 16:37:40.000000 datalad-0.9.3/tools/testing/conf/etc/apt/apt.conf.d/99apt-cacher
+-rw-------   0 yoh      (47521) yoh      (47522)      179 2018-03-04 16:37:40.000000 datalad-0.9.3/tools/testing/conf/apache-ssh-supervisor.conf
+-rwx------   0 yoh      (47521) yoh      (47522)      938 2018-03-04 16:37:40.000000 datalad-0.9.3/tools/testing/make_test_repos
+-rwx------   0 yoh      (47521) yoh      (47522)      593 2018-03-04 16:37:40.000000 datalad-0.9.3/tools/upgrade-annex-osx.sh
+-rwx------   0 yoh      (47521) yoh      (47522)     1531 2018-03-04 16:37:40.000000 datalad-0.9.3/tools/dtime
+-rwx------   0 yoh      (47521) yoh      (47522)     2117 2018-03-04 16:37:40.000000 datalad-0.9.3/tools/cast2narration
+-rwx------   0 yoh      (47521) yoh      (47522)      359 2018-03-04 16:37:40.000000 datalad-0.9.3/tools/mkcontrib
+-rwx------   0 yoh      (47521) yoh      (47522)      656 2018-03-04 16:37:40.000000 datalad-0.9.3/tools/cast2script
+-rwx------   0 yoh      (47521) yoh      (47522)     3064 2018-03-04 16:37:40.000000 datalad-0.9.3/tools/cast_live
+-rwx------   0 yoh      (47521) yoh      (47522)     2472 2018-03-04 16:37:40.000000 datalad-0.9.3/tools/copy_urls_from_datalad.py
+-rw-------   0 yoh      (47521) yoh      (47522)     1715 2018-03-04 16:37:40.000000 datalad-0.9.3/tools/cast_bash.rc
+drwx------   0 yoh      (47521) yoh      (47522)        0 2018-03-16 22:27:17.000000 datalad-0.9.3/tools/ci/
+-rw-------   0 yoh      (47521) yoh      (47522)      589 2018-03-04 16:37:40.000000 datalad-0.9.3/tools/ci/gpg-90F7E9EB.pub
+-rwx------   0 yoh      (47521) yoh      (47522)      513 2018-03-04 16:37:40.000000 datalad-0.9.3/tools/ci/install-annex-snapshot.sh
+-rwx------   0 yoh      (47521) yoh      (47522)      714 2018-03-04 16:37:40.000000 datalad-0.9.3/tools/ci/prep-travis-devel-annex.sh
+-rwx------   0 yoh      (47521) yoh      (47522)      581 2018-03-04 16:37:40.000000 datalad-0.9.3/tools/ci/prep-travis-forssh.sh
+-rwx------   0 yoh      (47521) yoh      (47522)       97 2018-03-04 16:37:40.000000 datalad-0.9.3/tools/ci/prep-travis-forssh-sudo.sh
+-rwx------   0 yoh      (47521) yoh      (47522)     4000 2018-03-04 16:37:40.000000 datalad-0.9.3/tools/cast2asciinema
+-rwx------   0 yoh      (47521) yoh      (47522)     2797 2018-03-04 16:37:40.000000 datalad-0.9.3/tools/monitor-interrupts.py
+drwx------   0 yoh      (47521) yoh      (47522)        0 2018-03-16 22:27:17.000000 datalad-0.9.3/tools/coverage-bin/
+-rwx------   0 yoh      (47521) yoh      (47522)      806 2018-03-04 16:37:40.000000 datalad-0.9.3/tools/coverage-bin/git-annex-remote-datalad
+-rwx------   0 yoh      (47521) yoh      (47522)      806 2018-03-04 16:37:40.000000 datalad-0.9.3/tools/coverage-bin/git-annex-remote-datalad-archives
+-rwx------   0 yoh      (47521) yoh      (47522)      806 2018-03-04 16:37:40.000000 datalad-0.9.3/tools/coverage-bin/datalad
+-rwx------   0 yoh      (47521) yoh      (47522)     3010 2018-03-04 16:37:40.000000 datalad-0.9.3/tools/mimic_merges
+-rwx------   0 yoh      (47521) yoh      (47522)     3565 2018-03-04 16:37:40.000000 datalad-0.9.3/tools/urlinfo
+-rw-------   0 yoh      (47521) yoh      (47522)    25104 2018-03-16 22:26:59.000000 datalad-0.9.3/CHANGELOG.md
+-rw-------   0 yoh      (47521) yoh      (47522)     2114 2018-03-04 16:37:39.000000 datalad-0.9.3/COPYING
+-rw-------   0 yoh      (47521) yoh      (47522)      377 2018-03-04 16:37:40.000000 datalad-0.9.3/requirements-devel.txt
+-rw-------   0 yoh      (47521) yoh      (47522)       38 2018-03-16 22:27:17.000000 datalad-0.9.3/setup.cfg
+-rw-------   0 yoh      (47521) yoh      (47522)      223 2018-03-04 16:37:39.000000 datalad-0.9.3/.gitignore
+-rw-------   0 yoh      (47521) yoh      (47522)     7150 2018-03-04 16:37:39.000000 datalad-0.9.3/README.md
+-rw-------   0 yoh      (47521) yoh      (47522)    18887 2018-03-16 22:26:59.000000 datalad-0.9.3/CONTRIBUTING.md
+-rw-------   0 yoh      (47521) yoh      (47522)     6066 2018-03-04 16:37:39.000000 datalad-0.9.3/asv.conf.json
+drwx------   0 yoh      (47521) yoh      (47522)        0 2018-03-16 22:27:17.000000 datalad-0.9.3/cfgs/
+-rw-------   0 yoh      (47521) yoh      (47522)      441 2018-03-04 16:37:39.000000 datalad-0.9.3/cfgs/openfmri.cfg
+-rw-------   0 yoh      (47521) yoh      (47522)     1179 2018-03-04 16:37:39.000000 datalad-0.9.3/cfgs/openfmri-ds000001.cfg
+-rw-------   0 yoh      (47521) yoh      (47522)       90 2018-03-04 16:37:39.000000 datalad-0.9.3/cfgs/arjlover.cfg
+-rw-------   0 yoh      (47521) yoh      (47522)     2409 2018-03-04 16:37:39.000000 datalad-0.9.3/cfgs/nihhelpers.py
+-rw-------   0 yoh      (47521) yoh      (47522)     1150 2018-03-04 16:37:39.000000 datalad-0.9.3/cfgs/nih-videos.cfg
+-rw-------   0 yoh      (47521) yoh      (47522)      979 2018-03-04 16:37:39.000000 datalad-0.9.3/cfgs/arjlover-fast.cfg
+-rw-------   0 yoh      (47521) yoh      (47522)      451 2018-03-04 16:37:39.000000 datalad-0.9.3/cfgs/example-feat.cfg
+-rw-------   0 yoh      (47521) yoh      (47522)     2015 2018-03-04 16:37:39.000000 datalad-0.9.3/cfgs/common.cfg
+-rw-------   0 yoh      (47521) yoh      (47522)      810 2018-03-04 16:37:39.000000 datalad-0.9.3/cfgs/allen-human.cfg
+-rw-------   0 yoh      (47521) yoh      (47522)      305 2018-03-04 16:37:39.000000 datalad-0.9.3/CODE_OF_CONDUCT.md
+drwx------   0 yoh      (47521) yoh      (47522)        0 2018-03-16 22:27:17.000000 datalad-0.9.3/benchmarks/
+-rw-------   0 yoh      (47521) yoh      (47522)     2216 2018-03-04 16:37:39.000000 datalad-0.9.3/benchmarks/core.py
+-rw-------   0 yoh      (47521) yoh      (47522)        1 2018-03-04 16:37:39.000000 datalad-0.9.3/benchmarks/__init__.py
+-rw-------   0 yoh      (47521) yoh      (47522)     4012 2018-03-04 16:37:39.000000 datalad-0.9.3/benchmarks/api.py
+-rw-------   0 yoh      (47521) yoh      (47522)      696 2018-03-04 16:37:39.000000 datalad-0.9.3/benchmarks/common.py
+-rw-------   0 yoh      (47521) yoh      (47522)      517 2018-03-04 16:37:39.000000 datalad-0.9.3/.mailmap
+-rw-------   0 yoh      (47521) yoh      (47522)    10446 2018-03-04 16:37:40.000000 datalad-0.9.3/formatters.py
+-rw-------   0 yoh      (47521) yoh      (47522)      125 2018-03-04 16:37:40.000000 datalad-0.9.3/readthedocs.yml
+-rw-------   0 yoh      (47521) yoh      (47522)       75 2018-03-04 16:37:39.000000 datalad-0.9.3/.gitmodules
+-rw-------   0 yoh      (47521) yoh      (47522)       45 2018-03-04 16:37:39.000000 datalad-0.9.3/.coveragerc
+drwx------   0 yoh      (47521) yoh      (47522)        0 2018-03-16 22:27:17.000000 datalad-0.9.3/datalad.egg-info/
+-rw-------   0 yoh      (47521) yoh      (47522)        8 2018-03-16 22:27:17.000000 datalad-0.9.3/datalad.egg-info/top_level.txt
+-rw-------   0 yoh      (47521) yoh      (47522)     9167 2018-03-16 22:27:17.000000 datalad-0.9.3/datalad.egg-info/PKG-INFO
+-rw-------   0 yoh      (47521) yoh      (47522)     1607 2018-03-16 22:27:17.000000 datalad-0.9.3/datalad.egg-info/requires.txt
+-rw-------   0 yoh      (47521) yoh      (47522)    13684 2018-03-16 22:27:17.000000 datalad-0.9.3/datalad.egg-info/SOURCES.txt
+-rw-------   0 yoh      (47521) yoh      (47522)        1 2018-03-16 22:27:17.000000 datalad-0.9.3/datalad.egg-info/dependency_links.txt
+drwx------   0 yoh      (47521) yoh      (47522)        0 2018-03-16 22:27:17.000000 datalad-0.9.3/datalad/
+drwx------   0 yoh      (47521) yoh      (47522)        0 2018-03-16 22:27:17.000000 datalad-0.9.3/datalad/tests/
+-rw-------   0 yoh      (47521) yoh      (47522)     2098 2018-03-16 22:26:59.000000 datalad-0.9.3/datalad/tests/test_base.py
+-rw-------   0 yoh      (47521) yoh      (47522)     7686 2018-03-04 16:37:40.000000 datalad-0.9.3/datalad/tests/test_constraints.py
+-rw-------   0 yoh      (47521) yoh      (47522)     2421 2018-03-04 16:37:40.000000 datalad-0.9.3/datalad/tests/test_testrepos.py
+-rw-------   0 yoh      (47521) yoh      (47522)     4561 2018-03-04 16:37:40.000000 datalad-0.9.3/datalad/tests/test_interface.py
+-rw-------   0 yoh      (47521) yoh      (47522)     1530 2018-03-04 16:37:40.000000 datalad-0.9.3/datalad/tests/test__main__.py
+-rw-------   0 yoh      (47521) yoh      (47522)    27257 2018-03-04 16:37:40.000000 datalad-0.9.3/datalad/tests/test_utils.py
+-rw-------   0 yoh      (47521) yoh      (47522)      252 2018-03-04 16:37:40.000000 datalad-0.9.3/datalad/tests/heavyoutput.py
+-rw-------   0 yoh      (47521) yoh      (47522)     2961 2018-03-04 16:37:40.000000 datalad-0.9.3/datalad/tests/test_s3.py
+-rw-------   0 yoh      (47521) yoh      (47522)     4013 2018-03-04 16:37:40.000000 datalad-0.9.3/datalad/tests/utils_testdatasets.py
+-rw-------   0 yoh      (47521) yoh      (47522)     1442 2018-03-04 16:37:40.000000 datalad-0.9.3/datalad/tests/test_misc.py
+-rw-------   0 yoh      (47521) yoh      (47522)     5302 2018-03-04 16:37:40.000000 datalad-0.9.3/datalad/tests/test_log.py
+-rw-------   0 yoh      (47521) yoh      (47522)     7396 2018-03-04 16:37:40.000000 datalad-0.9.3/datalad/tests/test_auto.py
+-rw-------   0 yoh      (47521) yoh      (47522)      811 2018-03-04 16:37:40.000000 datalad-0.9.3/datalad/tests/__init__.py
+-rw-------   0 yoh      (47521) yoh      (47522)    19205 2018-03-04 16:37:40.000000 datalad-0.9.3/datalad/tests/test_tests_utils.py
+-rw-------   0 yoh      (47521) yoh      (47522)     6891 2018-03-04 16:37:40.000000 datalad-0.9.3/datalad/tests/test_archives.py
+-rw-------   0 yoh      (47521) yoh      (47522)    12049 2018-03-04 16:37:40.000000 datalad-0.9.3/datalad/tests/test_config.py
+-rw-------   0 yoh      (47521) yoh      (47522)    11446 2018-03-04 16:37:40.000000 datalad-0.9.3/datalad/tests/test_cmd.py
+-rw-------   0 yoh      (47521) yoh      (47522)    46631 2018-03-16 22:26:59.000000 datalad-0.9.3/datalad/tests/utils.py
+-rw-------   0 yoh      (47521) yoh      (47522)     7897 2018-03-04 16:37:40.000000 datalad-0.9.3/datalad/tests/utils_testrepos.py
+-rw-------   0 yoh      (47521) yoh      (47522)     1924 2018-03-04 16:37:40.000000 datalad-0.9.3/datalad/tests/test_utils_testrepos.py
+-rw-------   0 yoh      (47521) yoh      (47522)     2714 2018-03-04 16:37:40.000000 datalad-0.9.3/datalad/tests/test_api.py
+-rw-------   0 yoh      (47521) yoh      (47522)     6919 2018-03-04 16:37:40.000000 datalad-0.9.3/datalad/tests/test_protocols.py
+-rw-------   0 yoh      (47521) yoh      (47522)     1323 2018-03-04 16:37:40.000000 datalad-0.9.3/datalad/tests/test_installed.py
+-rw-------   0 yoh      (47521) yoh      (47522)     5168 2018-03-04 16:37:40.000000 datalad-0.9.3/datalad/tests/test_dochelpers.py
+-rw-------   0 yoh      (47521) yoh      (47522)     1256 2018-03-04 16:37:40.000000 datalad-0.9.3/datalad/tests/test_strings.py
+-rw-------   0 yoh      (47521) yoh      (47522)     3700 2018-03-04 16:37:40.000000 datalad-0.9.3/datalad/tests/test_direct_mode.py
+drwx------   0 yoh      (47521) yoh      (47522)        0 2018-03-16 22:27:17.000000 datalad-0.9.3/datalad/interface/
+-rw-------   0 yoh      (47521) yoh      (47522)    17663 2018-03-04 16:37:40.000000 datalad-0.9.3/datalad/interface/base.py
+drwx------   0 yoh      (47521) yoh      (47522)        0 2018-03-16 22:27:17.000000 datalad-0.9.3/datalad/interface/tests/
+-rw-------   0 yoh      (47521) yoh      (47522)    12370 2018-03-16 22:26:59.000000 datalad-0.9.3/datalad/interface/tests/test_save.py
+-rw-------   0 yoh      (47521) yoh      (47522)    20655 2018-03-16 22:26:59.000000 datalad-0.9.3/datalad/interface/tests/test_add_archive_content.py
+-rw-------   0 yoh      (47521) yoh      (47522)     4053 2018-03-04 16:37:40.000000 datalad-0.9.3/datalad/interface/tests/test_ls.py
+-rw-------   0 yoh      (47521) yoh      (47522)    10639 2018-03-04 16:37:40.000000 datalad-0.9.3/datalad/interface/tests/test_utils.py
+-rw-------   0 yoh      (47521) yoh      (47522)     3626 2018-03-04 16:37:40.000000 datalad-0.9.3/datalad/interface/tests/test_crawl_init.py
+-rw-------   0 yoh      (47521) yoh      (47522)     6223 2018-03-04 16:37:40.000000 datalad-0.9.3/datalad/interface/tests/test_unlock.py
+-rw-------   0 yoh      (47521) yoh      (47522)      450 2018-03-04 16:37:40.000000 datalad-0.9.3/datalad/interface/tests/__init__.py
+-rw-------   0 yoh      (47521) yoh      (47522)     8010 2018-03-04 16:37:40.000000 datalad-0.9.3/datalad/interface/tests/test_diff.py
+-rw-------   0 yoh      (47521) yoh      (47522)    13953 2018-03-04 16:37:40.000000 datalad-0.9.3/datalad/interface/tests/test_annotate_paths.py
+-rw-------   0 yoh      (47521) yoh      (47522)     4040 2018-03-04 16:37:40.000000 datalad-0.9.3/datalad/interface/tests/test_docs.py
+-rw-------   0 yoh      (47521) yoh      (47522)    11328 2018-03-04 16:37:40.000000 datalad-0.9.3/datalad/interface/tests/test_ls_webui.py
+-rw-------   0 yoh      (47521) yoh      (47522)     1921 2018-03-04 16:37:40.000000 datalad-0.9.3/datalad/interface/tests/test_download_url.py
+-rw-------   0 yoh      (47521) yoh      (47522)     3876 2018-03-04 16:37:40.000000 datalad-0.9.3/datalad/interface/tests/test_crawl.py
+-rw-------   0 yoh      (47521) yoh      (47522)    17720 2018-03-16 22:26:59.000000 datalad-0.9.3/datalad/interface/tests/test_run.py
+-rw-------   0 yoh      (47521) yoh      (47522)     2385 2018-03-04 16:37:40.000000 datalad-0.9.3/datalad/interface/tests/test_clean.py
+-rw-------   0 yoh      (47521) yoh      (47522)     8670 2018-03-04 16:37:40.000000 datalad-0.9.3/datalad/interface/run.py
+-rw-------   0 yoh      (47521) yoh      (47522)    24739 2018-03-04 16:37:40.000000 datalad-0.9.3/datalad/interface/add_archive_content.py
+-rw-------   0 yoh      (47521) yoh      (47522)     4510 2018-03-04 16:37:40.000000 datalad-0.9.3/datalad/interface/clean.py
+-rw-------   0 yoh      (47521) yoh      (47522)    13120 2018-03-04 16:37:40.000000 datalad-0.9.3/datalad/interface/results.py
+-rw-------   0 yoh      (47521) yoh      (47522)     8048 2018-03-04 16:37:40.000000 datalad-0.9.3/datalad/interface/crawl.py
+-rw-------   0 yoh      (47521) yoh      (47522)     3999 2018-03-04 16:37:40.000000 datalad-0.9.3/datalad/interface/download_url.py
+-rw-------   0 yoh      (47521) yoh      (47522)    23863 2018-03-16 22:26:59.000000 datalad-0.9.3/datalad/interface/ls.py
+-rw-------   0 yoh      (47521) yoh      (47522)     3398 2018-03-04 16:37:40.000000 datalad-0.9.3/datalad/interface/__init__.py
+-rw-------   0 yoh      (47521) yoh      (47522)     6492 2018-03-16 22:26:59.000000 datalad-0.9.3/datalad/interface/unlock.py
+-rw-------   0 yoh      (47521) yoh      (47522)    17190 2018-03-16 22:26:59.000000 datalad-0.9.3/datalad/interface/save.py
+-rw-------   0 yoh      (47521) yoh      (47522)     1936 2018-03-04 16:37:40.000000 datalad-0.9.3/datalad/interface/test.py
+-rw-------   0 yoh      (47521) yoh      (47522)    21736 2018-03-04 16:37:40.000000 datalad-0.9.3/datalad/interface/utils.py
+-rw-------   0 yoh      (47521) yoh      (47522)    12546 2018-03-16 22:26:59.000000 datalad-0.9.3/datalad/interface/common_opts.py
+-rw-------   0 yoh      (47521) yoh      (47522)    34420 2018-03-16 22:26:59.000000 datalad-0.9.3/datalad/interface/annotate_paths.py
+-rw-------   0 yoh      (47521) yoh      (47522)    15880 2018-03-16 22:26:59.000000 datalad-0.9.3/datalad/interface/diff.py
+-rw-------   0 yoh      (47521) yoh      (47522)     9291 2018-03-04 16:37:40.000000 datalad-0.9.3/datalad/interface/common_cfg.py
+-rw-------   0 yoh      (47521) yoh      (47522)     3957 2018-03-04 16:37:40.000000 datalad-0.9.3/datalad/interface/crawl_init.py
+-rw-------   0 yoh      (47521) yoh      (47522)    16245 2018-03-04 16:37:40.000000 datalad-0.9.3/datalad/interface/ls_webui.py
+-rw-------   0 yoh      (47521) yoh      (47522)    12661 2018-03-04 16:37:40.000000 datalad-0.9.3/datalad/interface/rerun.py
+-rw-------   0 yoh      (47521) yoh      (47522)     3132 2018-03-04 16:37:39.000000 datalad-0.9.3/datalad/__main__.py
+drwx------   0 yoh      (47521) yoh      (47522)        0 2018-03-16 22:27:17.000000 datalad-0.9.3/datalad/resources/
+drwx------   0 yoh      (47521) yoh      (47522)        0 2018-03-16 22:27:17.000000 datalad-0.9.3/datalad/resources/website/
+drwx------   0 yoh      (47521) yoh      (47522)        0 2018-03-16 22:27:17.000000 datalad-0.9.3/datalad/resources/website/tests/
+-rw-------   0 yoh      (47521) yoh      (47522)    13759 2018-03-04 16:37:40.000000 datalad-0.9.3/datalad/resources/website/tests/test.html
+drwx------   0 yoh      (47521) yoh      (47522)        0 2018-03-16 22:27:17.000000 datalad-0.9.3/datalad/resources/website/tests/qunit/
+-rw-------   0 yoh      (47521) yoh      (47522)   208178 2018-03-04 16:37:40.000000 datalad-0.9.3/datalad/resources/website/tests/qunit/sinon-1.17.5.js
+-rw-------   0 yoh      (47521) yoh      (47522)   117821 2018-03-04 16:37:40.000000 datalad-0.9.3/datalad/resources/website/tests/qunit/qunit-2.0.1.js
+-rw-------   0 yoh      (47521) yoh      (47522)     7456 2018-03-04 16:37:40.000000 datalad-0.9.3/datalad/resources/website/tests/qunit/qunit-2.0.1.css
+-rw-------   0 yoh      (47521) yoh      (47522)     2443 2018-03-04 16:37:40.000000 datalad-0.9.3/datalad/resources/website/tests/qunit/sinon-qunit-1.0.0.js
+drwx------   0 yoh      (47521) yoh      (47522)        0 2018-03-16 22:27:17.000000 datalad-0.9.3/datalad/resources/website/assets/
+drwx------   0 yoh      (47521) yoh      (47522)        0 2018-03-16 22:27:17.000000 datalad-0.9.3/datalad/resources/website/assets/images/
+-rw-------   0 yoh      (47521) yoh      (47522)    12537 2018-03-04 16:37:40.000000 datalad-0.9.3/datalad/resources/website/assets/images/logo_wide.svg
+-rw-------   0 yoh      (47521) yoh      (47522)      158 2018-03-04 16:37:40.000000 datalad-0.9.3/datalad/resources/website/assets/images/sort_desc.png
+-rw-------   0 yoh      (47521) yoh      (47522)      272 2018-03-04 16:37:40.000000 datalad-0.9.3/datalad/resources/website/assets/images/favicon-16x16.png
+-rw-------   0 yoh      (47521) yoh      (47522)      199 2018-03-04 16:37:40.000000 datalad-0.9.3/datalad/resources/website/assets/images/sort_both.png
+-rw-------   0 yoh      (47521) yoh      (47522)    15086 2018-03-04 16:37:40.000000 datalad-0.9.3/datalad/resources/website/assets/images/favicon.ico
+-rw-------   0 yoh      (47521) yoh      (47522)    16891 2018-03-04 16:37:40.000000 datalad-0.9.3/datalad/resources/website/assets/images/favicon.svg
+-rw-------   0 yoh      (47521) yoh      (47522)      158 2018-03-04 16:37:40.000000 datalad-0.9.3/datalad/resources/website/assets/images/sort_asc.png
+drwx------   0 yoh      (47521) yoh      (47522)        0 2018-03-16 22:27:17.000000 datalad-0.9.3/datalad/resources/website/assets/js/
+-rw-------   0 yoh      (47521) yoh      (47522)     8572 2018-03-04 16:37:40.000000 datalad-0.9.3/datalad/resources/website/assets/js/md5-2.3.0.js
+-rw-------   0 yoh      (47521) yoh      (47522)    21039 2018-03-04 16:37:40.000000 datalad-0.9.3/datalad/resources/website/assets/js/main.js
+-rw-------   0 yoh      (47521) yoh      (47522)   447304 2018-03-04 16:37:40.000000 datalad-0.9.3/datalad/resources/website/assets/js/jquery.dataTables-1.10.12.js
+-rw-------   0 yoh      (47521) yoh      (47522)   257551 2018-03-04 16:37:40.000000 datalad-0.9.3/datalad/resources/website/assets/js/jquery-2.2.4.js
+drwx------   0 yoh      (47521) yoh      (47522)        0 2018-03-16 22:27:17.000000 datalad-0.9.3/datalad/resources/website/assets/css/
+-rw-------   0 yoh      (47521) yoh      (47522)    15423 2018-03-04 16:37:40.000000 datalad-0.9.3/datalad/resources/website/assets/css/jquery.dataTables-1.10.12.css
+-rw-------   0 yoh      (47521) yoh      (47522)     3121 2018-03-04 16:37:40.000000 datalad-0.9.3/datalad/resources/website/index.html
+drwx------   0 yoh      (47521) yoh      (47522)        0 2018-03-16 22:27:17.000000 datalad-0.9.3/datalad/customremotes/
+-rw-------   0 yoh      (47521) yoh      (47522)    23561 2018-03-04 16:37:39.000000 datalad-0.9.3/datalad/customremotes/base.py
+drwx------   0 yoh      (47521) yoh      (47522)        0 2018-03-16 22:27:17.000000 datalad-0.9.3/datalad/customremotes/tests/
+-rw-------   0 yoh      (47521) yoh      (47522)     5199 2018-03-04 16:37:39.000000 datalad-0.9.3/datalad/customremotes/tests/test_base.py
+-rw-------   0 yoh      (47521) yoh      (47522)     1112 2018-03-04 16:37:39.000000 datalad-0.9.3/datalad/customremotes/tests/__init__.py
+-rw-------   0 yoh      (47521) yoh      (47522)    11004 2018-03-04 16:37:39.000000 datalad-0.9.3/datalad/customremotes/tests/test_archives.py
+-rw-------   0 yoh      (47521) yoh      (47522)     4182 2018-03-04 16:37:39.000000 datalad-0.9.3/datalad/customremotes/tests/test_datalad.py
+-rw-------   0 yoh      (47521) yoh      (47522)     4740 2018-03-04 16:37:39.000000 datalad-0.9.3/datalad/customremotes/main.py
+-rw-------   0 yoh      (47521) yoh      (47522)      483 2018-03-04 16:37:39.000000 datalad-0.9.3/datalad/customremotes/__init__.py
+-rw-------   0 yoh      (47521) yoh      (47522)     6906 2018-03-04 16:37:39.000000 datalad-0.9.3/datalad/customremotes/datalad.py
+-rw-------   0 yoh      (47521) yoh      (47522)    17001 2018-03-16 22:26:59.000000 datalad-0.9.3/datalad/customremotes/archives.py
+drwx------   0 yoh      (47521) yoh      (47522)        0 2018-03-16 22:27:17.000000 datalad-0.9.3/datalad/plugin/
+drwx------   0 yoh      (47521) yoh      (47522)        0 2018-03-16 22:27:17.000000 datalad-0.9.3/datalad/plugin/tests/
+-rw-------   0 yoh      (47521) yoh      (47522)      446 2018-03-04 16:37:40.000000 datalad-0.9.3/datalad/plugin/tests/__init__.py
+-rw-------   0 yoh      (47521) yoh      (47522)     8700 2018-03-04 16:37:40.000000 datalad-0.9.3/datalad/plugin/tests/test_plugins.py
+-rw-------   0 yoh      (47521) yoh      (47522)     3354 2018-03-16 22:26:59.000000 datalad-0.9.3/datalad/plugin/tests/test_tarball.py
+-rw-------   0 yoh      (47521) yoh      (47522)     4256 2018-03-04 16:37:40.000000 datalad-0.9.3/datalad/plugin/no_annex.py
+-rw-------   0 yoh      (47521) yoh      (47522)     2934 2018-03-16 22:26:59.000000 datalad-0.9.3/datalad/plugin/export_tarball.py
+-rw-------   0 yoh      (47521) yoh      (47522)     3645 2018-03-04 16:37:40.000000 datalad-0.9.3/datalad/plugin/wtf.py
+-rw-------   0 yoh      (47521) yoh      (47522)     9976 2018-03-04 16:37:40.000000 datalad-0.9.3/datalad/plugin/__init__.py
+-rw-------   0 yoh      (47521) yoh      (47522)     2373 2018-03-04 16:37:40.000000 datalad-0.9.3/datalad/plugin/add_readme.py
+-rw-------   0 yoh      (47521) yoh      (47522)    24506 2018-03-04 16:37:39.000000 datalad-0.9.3/datalad/config.py
+-rw-------   0 yoh      (47521) yoh      (47522)    10578 2018-03-04 16:37:39.000000 datalad-0.9.3/datalad/auto.py
+-rw-------   0 yoh      (47521) yoh      (47522)    10190 2018-03-04 16:37:40.000000 datalad-0.9.3/datalad/log.py
+drwx------   0 yoh      (47521) yoh      (47522)        0 2018-03-16 22:27:17.000000 datalad-0.9.3/datalad/support/
+drwx------   0 yoh      (47521) yoh      (47522)        0 2018-03-16 22:27:17.000000 datalad-0.9.3/datalad/support/tests/
+-rw-------   0 yoh      (47521) yoh      (47522)      663 2018-03-04 16:37:40.000000 datalad-0.9.3/datalad/support/tests/test_cache.py
+-rw-------   0 yoh      (47521) yoh      (47522)    18314 2018-03-04 16:37:40.000000 datalad-0.9.3/datalad/support/tests/test_network.py
+-rw-------   0 yoh      (47521) yoh      (47522)    79763 2018-03-04 16:37:40.000000 datalad-0.9.3/datalad/support/tests/test_annexrepo.py
+-rw-------   0 yoh      (47521) yoh      (47522)     1076 2018-03-04 16:37:40.000000 datalad-0.9.3/datalad/support/tests/test_vcr_.py
+-rw-------   0 yoh      (47521) yoh      (47522)    42904 2018-03-16 22:26:59.000000 datalad-0.9.3/datalad/support/tests/test_gitrepo.py
+-rw-------   0 yoh      (47521) yoh      (47522)     2025 2018-03-04 16:37:40.000000 datalad-0.9.3/datalad/support/tests/test_digests.py
+-rw-------   0 yoh      (47521) yoh      (47522)     3184 2018-03-04 16:37:40.000000 datalad-0.9.3/datalad/support/tests/test_stats.py
+-rw-------   0 yoh      (47521) yoh      (47522)      469 2018-03-04 16:37:40.000000 datalad-0.9.3/datalad/support/tests/__init__.py
+-rw-------   0 yoh      (47521) yoh      (47522)     1508 2018-03-04 16:37:40.000000 datalad-0.9.3/datalad/support/tests/test_status.py
+-rw-------   0 yoh      (47521) yoh      (47522)     3268 2018-03-16 22:26:59.000000 datalad-0.9.3/datalad/support/tests/test_locking.py
+-rw-------   0 yoh      (47521) yoh      (47522)     6055 2018-03-04 16:37:40.000000 datalad-0.9.3/datalad/support/tests/test_versions.py
+-rw-------   0 yoh      (47521) yoh      (47522)     1628 2018-03-04 16:37:40.000000 datalad-0.9.3/datalad/support/tests/utils.py
+-rw-------   0 yoh      (47521) yoh      (47522)     1812 2018-03-04 16:37:40.000000 datalad-0.9.3/datalad/support/tests/test_sshrun.py
+-rw-------   0 yoh      (47521) yoh      (47522)     1397 2018-03-16 22:26:59.000000 datalad-0.9.3/datalad/support/tests/test_json_py.py
+-rw-------   0 yoh      (47521) yoh      (47522)     7912 2018-03-04 16:37:40.000000 datalad-0.9.3/datalad/support/tests/test_external_versions.py
+-rw-------   0 yoh      (47521) yoh      (47522)     7611 2018-03-04 16:37:40.000000 datalad-0.9.3/datalad/support/tests/test_sshconnector.py
+-rw-------   0 yoh      (47521) yoh      (47522)     6913 2018-03-04 16:37:40.000000 datalad-0.9.3/datalad/support/versions.py
+-rw-------   0 yoh      (47521) yoh      (47522)     3247 2018-03-04 16:37:40.000000 datalad-0.9.3/datalad/support/keyring_.py
+-rw-------   0 yoh      (47521) yoh      (47522)     5045 2018-03-04 16:37:40.000000 datalad-0.9.3/datalad/support/param.py
+-rw-------   0 yoh      (47521) yoh      (47522)     3178 2018-03-04 16:37:40.000000 datalad-0.9.3/datalad/support/sshrun.py
+-rw-------   0 yoh      (47521) yoh      (47522)     8584 2018-03-04 16:37:40.000000 datalad-0.9.3/datalad/support/external_versions.py
+-rw-------   0 yoh      (47521) yoh      (47522)   143144 2018-03-16 22:26:59.000000 datalad-0.9.3/datalad/support/annexrepo.py
+-rw-------   0 yoh      (47521) yoh      (47522)     7368 2018-03-16 22:26:59.000000 datalad-0.9.3/datalad/support/_lru_cache2.py
+-rw-------   0 yoh      (47521) yoh      (47522)    14013 2018-03-04 16:37:40.000000 datalad-0.9.3/datalad/support/constraints.py
+-rw-------   0 yoh      (47521) yoh      (47522)    82203 2018-03-16 22:26:59.000000 datalad-0.9.3/datalad/support/gitrepo.py
+-rw-------   0 yoh      (47521) yoh      (47522)     2381 2018-03-04 16:37:40.000000 datalad-0.9.3/datalad/support/status.py
+drwx------   0 yoh      (47521) yoh      (47522)        0 2018-03-16 22:27:17.000000 datalad-0.9.3/datalad/support/third/
+-rw-------   0 yoh      (47521) yoh      (47522)    13859 2018-03-04 16:37:40.000000 datalad-0.9.3/datalad/support/third/noseclasses.py
+-rw-------   0 yoh      (47521) yoh      (47522)        0 2018-03-04 16:37:40.000000 datalad-0.9.3/datalad/support/third/__init__.py
+-rw-------   0 yoh      (47521) yoh      (47522)    15888 2018-03-04 16:37:40.000000 datalad-0.9.3/datalad/support/third/nosetester.py
+-rw-------   0 yoh      (47521) yoh      (47522)     3872 2018-03-04 16:37:40.000000 datalad-0.9.3/datalad/support/third/nda_aws_token_generator.py
+-rw-------   0 yoh      (47521) yoh      (47522)     9015 2018-03-04 16:37:40.000000 datalad-0.9.3/datalad/support/protocol.py
+-rw-------   0 yoh      (47521) yoh      (47522)     2313 2018-03-04 16:37:40.000000 datalad-0.9.3/datalad/support/nda_.py
+-rw-------   0 yoh      (47521) yoh      (47522)     3055 2018-03-04 16:37:40.000000 datalad-0.9.3/datalad/support/cookies.py
+-rw-------   0 yoh      (47521) yoh      (47522)      502 2018-03-04 16:37:40.000000 datalad-0.9.3/datalad/support/__init__.py
+-rw-------   0 yoh      (47521) yoh      (47522)    17412 2018-03-04 16:37:40.000000 datalad-0.9.3/datalad/support/sshconnector.py
+-rw-------   0 yoh      (47521) yoh      (47522)     2105 2018-03-04 16:37:40.000000 datalad-0.9.3/datalad/support/strings.py
+-rw-------   0 yoh      (47521) yoh      (47522)     9770 2018-03-04 16:37:40.000000 datalad-0.9.3/datalad/support/exceptions.py
+-rw-------   0 yoh      (47521) yoh      (47522)    30840 2018-03-16 22:26:59.000000 datalad-0.9.3/datalad/support/network.py
+-rw-------   0 yoh      (47521) yoh      (47522)     6905 2018-03-04 16:37:40.000000 datalad-0.9.3/datalad/support/repo.py
+-rw-------   0 yoh      (47521) yoh      (47522)     3413 2018-03-04 16:37:40.000000 datalad-0.9.3/datalad/support/vcr_.py
+-rw-------   0 yoh      (47521) yoh      (47522)     2470 2018-03-16 22:26:59.000000 datalad-0.9.3/datalad/support/json_py.py
+-rw-------   0 yoh      (47521) yoh      (47522)    14697 2018-03-04 16:37:40.000000 datalad-0.9.3/datalad/support/s3.py
+-rw-------   0 yoh      (47521) yoh      (47522)     6114 2018-03-04 16:37:40.000000 datalad-0.9.3/datalad/support/configparserinc.py
+-rw-------   0 yoh      (47521) yoh      (47522)     1454 2018-03-04 16:37:40.000000 datalad-0.9.3/datalad/support/ansi_colors.py
+-rw-------   0 yoh      (47521) yoh      (47522)     1672 2018-03-04 16:37:40.000000 datalad-0.9.3/datalad/support/digests.py
+-rw-------   0 yoh      (47521) yoh      (47522)    19700 2018-03-16 22:26:59.000000 datalad-0.9.3/datalad/support/archives.py
+-rw-------   0 yoh      (47521) yoh      (47522)     6187 2018-03-04 16:37:40.000000 datalad-0.9.3/datalad/support/stats.py
+-rw-------   0 yoh      (47521) yoh      (47522)     1221 2018-03-16 22:26:59.000000 datalad-0.9.3/datalad/support/cache.py
+-rw-------   0 yoh      (47521) yoh      (47522)     3204 2018-03-16 22:26:59.000000 datalad-0.9.3/datalad/support/locking.py
+drwx------   0 yoh      (47521) yoh      (47522)        0 2018-03-16 22:27:17.000000 datalad-0.9.3/datalad/crawler/
+-rw-------   0 yoh      (47521) yoh      (47522)      504 2018-03-04 16:37:39.000000 datalad-0.9.3/datalad/crawler/base.py
+drwx------   0 yoh      (47521) yoh      (47522)        0 2018-03-16 22:27:17.000000 datalad-0.9.3/datalad/crawler/tests/
+-rw-------   0 yoh      (47521) yoh      (47522)     9825 2018-03-04 16:37:39.000000 datalad-0.9.3/datalad/crawler/tests/test_pipeline.py
+-rw-------   0 yoh      (47521) yoh      (47522)      566 2018-03-04 16:37:39.000000 datalad-0.9.3/datalad/crawler/tests/__init__.py
+-rw-------   0 yoh      (47521) yoh      (47522)    21798 2018-03-04 16:37:39.000000 datalad-0.9.3/datalad/crawler/pipeline.py
+drwx------   0 yoh      (47521) yoh      (47522)        0 2018-03-16 22:27:17.000000 datalad-0.9.3/datalad/crawler/dbs/
+-rw-------   0 yoh      (47521) yoh      (47522)     7153 2018-03-04 16:37:39.000000 datalad-0.9.3/datalad/crawler/dbs/base.py
+drwx------   0 yoh      (47521) yoh      (47522)        0 2018-03-16 22:27:17.000000 datalad-0.9.3/datalad/crawler/dbs/tests/
+-rw-------   0 yoh      (47521) yoh      (47522)     5198 2018-03-04 16:37:39.000000 datalad-0.9.3/datalad/crawler/dbs/tests/test_files.py
+-rw-------   0 yoh      (47521) yoh      (47522)      389 2018-03-04 16:37:39.000000 datalad-0.9.3/datalad/crawler/dbs/tests/__init__.py
+-rw-------   0 yoh      (47521) yoh      (47522)     3141 2018-03-04 16:37:39.000000 datalad-0.9.3/datalad/crawler/dbs/versions.py
+-rw-------   0 yoh      (47521) yoh      (47522)      461 2018-03-04 16:37:39.000000 datalad-0.9.3/datalad/crawler/dbs/__init__.py
+-rw-------   0 yoh      (47521) yoh      (47522)     5217 2018-03-04 16:37:39.000000 datalad-0.9.3/datalad/crawler/dbs/files.py
+drwx------   0 yoh      (47521) yoh      (47522)        0 2018-03-16 22:27:17.000000 datalad-0.9.3/datalad/crawler/oldconfig/
+-rw-------   0 yoh      (47521) yoh      (47522)     6357 2018-03-04 16:37:39.000000 datalad-0.9.3/datalad/crawler/oldconfig/base.py
+drwx------   0 yoh      (47521) yoh      (47522)        0 2018-03-16 22:27:17.000000 datalad-0.9.3/datalad/crawler/oldconfig/tests/
+-rw-------   0 yoh      (47521) yoh      (47522)        0 2018-03-04 16:37:39.000000 datalad-0.9.3/datalad/crawler/oldconfig/tests/__init__.py
+-rw-------   0 yoh      (47521) yoh      (47522)     2082 2018-03-04 16:37:39.000000 datalad-0.9.3/datalad/crawler/oldconfig/tests/test_config.py
+-rw-------   0 yoh      (47521) yoh      (47522)      516 2018-03-04 16:37:39.000000 datalad-0.9.3/datalad/crawler/oldconfig/__init__.py
+drwx------   0 yoh      (47521) yoh      (47522)        0 2018-03-16 22:27:17.000000 datalad-0.9.3/datalad/crawler/nodes/
+drwx------   0 yoh      (47521) yoh      (47522)        0 2018-03-16 22:27:17.000000 datalad-0.9.3/datalad/crawler/nodes/tests/
+-rw-------   0 yoh      (47521) yoh      (47522)    16493 2018-03-04 16:37:39.000000 datalad-0.9.3/datalad/crawler/nodes/tests/test_annex.py
+-rw-------   0 yoh      (47521) yoh      (47522)     4261 2018-03-04 16:37:39.000000 datalad-0.9.3/datalad/crawler/nodes/tests/test_matches.py
+-rw-------   0 yoh      (47521) yoh      (47522)     9340 2018-03-04 16:37:39.000000 datalad-0.9.3/datalad/crawler/nodes/tests/test_s3.py
+-rw-------   0 yoh      (47521) yoh      (47522)    17177 2018-03-04 16:37:39.000000 datalad-0.9.3/datalad/crawler/nodes/tests/test_misc.py
+-rw-------   0 yoh      (47521) yoh      (47522)      501 2018-03-04 16:37:39.000000 datalad-0.9.3/datalad/crawler/nodes/tests/__init__.py
+-rw-------   0 yoh      (47521) yoh      (47522)     2973 2018-03-04 16:37:39.000000 datalad-0.9.3/datalad/crawler/nodes/tests/test_crawl_url.py
+-rw-------   0 yoh      (47521) yoh      (47522)     6822 2018-03-04 16:37:39.000000 datalad-0.9.3/datalad/crawler/nodes/crawl_url.py
+-rw-------   0 yoh      (47521) yoh      (47522)    67617 2018-03-04 16:37:39.000000 datalad-0.9.3/datalad/crawler/nodes/annex.py
+-rw-------   0 yoh      (47521) yoh      (47522)      894 2018-03-04 16:37:39.000000 datalad-0.9.3/datalad/crawler/nodes/__init__.py
+-rw-------   0 yoh      (47521) yoh      (47522)    18482 2018-03-04 16:37:39.000000 datalad-0.9.3/datalad/crawler/nodes/misc.py
+-rw-------   0 yoh      (47521) yoh      (47522)    12951 2018-03-04 16:37:39.000000 datalad-0.9.3/datalad/crawler/nodes/s3.py
+-rw-------   0 yoh      (47521) yoh      (47522)     7386 2018-03-04 16:37:39.000000 datalad-0.9.3/datalad/crawler/nodes/matches.py
+-rw-------   0 yoh      (47521) yoh      (47522)      504 2018-03-04 16:37:39.000000 datalad-0.9.3/datalad/crawler/__init__.py
+drwx------   0 yoh      (47521) yoh      (47522)        0 2018-03-16 22:27:17.000000 datalad-0.9.3/datalad/crawler/pipelines/
+drwx------   0 yoh      (47521) yoh      (47522)        0 2018-03-16 22:27:17.000000 datalad-0.9.3/datalad/crawler/pipelines/tests/
+-rw-------   0 yoh      (47521) yoh      (47522)     1065 2018-03-04 16:37:39.000000 datalad-0.9.3/datalad/crawler/pipelines/tests/test_nda.py
+-rw-------   0 yoh      (47521) yoh      (47522)     2948 2018-03-04 16:37:39.000000 datalad-0.9.3/datalad/crawler/pipelines/tests/test_openfmri_collection.py
+-rw-------   0 yoh      (47521) yoh      (47522)     3398 2018-03-04 16:37:39.000000 datalad-0.9.3/datalad/crawler/pipelines/tests/test_simple_s3.py
+-rw-------   0 yoh      (47521) yoh      (47522)     3153 2018-03-04 16:37:39.000000 datalad-0.9.3/datalad/crawler/pipelines/tests/test_fcptable.py
+-rw-------   0 yoh      (47521) yoh      (47522)      177 2018-03-04 16:37:39.000000 datalad-0.9.3/datalad/crawler/pipelines/tests/__init__.py
+-rw-------   0 yoh      (47521) yoh      (47522)    24487 2018-03-04 16:37:39.000000 datalad-0.9.3/datalad/crawler/pipelines/tests/test_openfmri.py
+-rw-------   0 yoh      (47521) yoh      (47522)     2889 2018-03-04 16:37:39.000000 datalad-0.9.3/datalad/crawler/pipelines/tests/test_simple_with_archives.py
+-rw-------   0 yoh      (47521) yoh      (47522)      920 2018-03-04 16:37:39.000000 datalad-0.9.3/datalad/crawler/pipelines/tests/utils.py
+-rw-------   0 yoh      (47521) yoh      (47522)     1847 2018-03-04 16:37:39.000000 datalad-0.9.3/datalad/crawler/pipelines/tests/test_crcns.py
+-rw-------   0 yoh      (47521) yoh      (47522)    12480 2018-03-04 16:37:39.000000 datalad-0.9.3/datalad/crawler/pipelines/tests/test_balsa.py
+-rw-------   0 yoh      (47521) yoh      (47522)    11087 2018-03-04 16:37:39.000000 datalad-0.9.3/datalad/crawler/pipelines/crcns.py
+-rw-------   0 yoh      (47521) yoh      (47522)    14323 2018-03-04 16:37:39.000000 datalad-0.9.3/datalad/crawler/pipelines/openfmri.py
+-rw-------   0 yoh      (47521) yoh      (47522)     1086 2018-03-04 16:37:39.000000 datalad-0.9.3/datalad/crawler/pipelines/template.py
+-rw-------   0 yoh      (47521) yoh      (47522)     9920 2018-03-04 16:37:39.000000 datalad-0.9.3/datalad/crawler/pipelines/balsa.py
+-rw-------   0 yoh      (47521) yoh      (47522)     4569 2018-03-04 16:37:39.000000 datalad-0.9.3/datalad/crawler/pipelines/simple_with_archives.py
+-rw-------   0 yoh      (47521) yoh      (47522)      458 2018-03-04 16:37:39.000000 datalad-0.9.3/datalad/crawler/pipelines/__init__.py
+-rw-------   0 yoh      (47521) yoh      (47522)     4163 2018-03-04 16:37:39.000000 datalad-0.9.3/datalad/crawler/pipelines/openfmri_s3.py
+-rw-------   0 yoh      (47521) yoh      (47522)     3173 2018-03-04 16:37:39.000000 datalad-0.9.3/datalad/crawler/pipelines/abstractsonline.py
+-rw-------   0 yoh      (47521) yoh      (47522)     6061 2018-03-04 16:37:39.000000 datalad-0.9.3/datalad/crawler/pipelines/simple_s3.py
+-rw-------   0 yoh      (47521) yoh      (47522)     6072 2018-03-04 16:37:39.000000 datalad-0.9.3/datalad/crawler/pipelines/nda.py
+-rw-------   0 yoh      (47521) yoh      (47522)     7165 2018-03-04 16:37:39.000000 datalad-0.9.3/datalad/crawler/pipelines/fcptable.py
+-rw-------   0 yoh      (47521) yoh      (47522)     2393 2018-03-04 16:37:39.000000 datalad-0.9.3/datalad/consts.py
+-rw-------   0 yoh      (47521) yoh      (47522)     7078 2018-03-16 22:26:59.000000 datalad-0.9.3/datalad/__init__.py
+drwx------   0 yoh      (47521) yoh      (47522)        0 2018-03-16 22:27:17.000000 datalad-0.9.3/datalad/ui/
+-rw-------   0 yoh      (47521) yoh      (47522)     1170 2018-03-04 16:37:40.000000 datalad-0.9.3/datalad/ui/base.py
+drwx------   0 yoh      (47521) yoh      (47522)        0 2018-03-16 22:27:17.000000 datalad-0.9.3/datalad/ui/tests/
+-rw-------   0 yoh      (47521) yoh      (47522)     2512 2018-03-04 16:37:40.000000 datalad-0.9.3/datalad/ui/tests/test_base.py
+-rw-------   0 yoh      (47521) yoh      (47522)     3824 2018-03-04 16:37:40.000000 datalad-0.9.3/datalad/ui/tests/test_dialog.py
+-rw-------   0 yoh      (47521) yoh      (47522)      442 2018-03-04 16:37:40.000000 datalad-0.9.3/datalad/ui/tests/__init__.py
+-rw-------   0 yoh      (47521) yoh      (47522)    10191 2018-03-04 16:37:40.000000 datalad-0.9.3/datalad/ui/dialog.py
+-rw-------   0 yoh      (47521) yoh      (47522)     2673 2018-03-04 16:37:40.000000 datalad-0.9.3/datalad/ui/__init__.py
+-rw-------   0 yoh      (47521) yoh      (47522)     1633 2018-03-04 16:37:40.000000 datalad-0.9.3/datalad/ui/utils.py
+-rw-------   0 yoh      (47521) yoh      (47522)     6123 2018-03-04 16:37:40.000000 datalad-0.9.3/datalad/ui/progressbars.py
+drwx------   0 yoh      (47521) yoh      (47522)        0 2018-03-16 22:27:17.000000 datalad-0.9.3/datalad/downloaders/
+-rw-------   0 yoh      (47521) yoh      (47522)    22303 2018-03-04 16:37:40.000000 datalad-0.9.3/datalad/downloaders/base.py
+drwx------   0 yoh      (47521) yoh      (47522)        0 2018-03-16 22:27:17.000000 datalad-0.9.3/datalad/downloaders/tests/
+-rw-------   0 yoh      (47521) yoh      (47522)      454 2018-03-04 16:37:40.000000 datalad-0.9.3/datalad/downloaders/tests/test_base.py
+-rw-------   0 yoh      (47521) yoh      (47522)     4629 2018-03-04 16:37:40.000000 datalad-0.9.3/datalad/downloaders/tests/test_credentials.py
+-rw-------   0 yoh      (47521) yoh      (47522)     4533 2018-03-04 16:37:40.000000 datalad-0.9.3/datalad/downloaders/tests/test_s3.py
+-rw-------   0 yoh      (47521) yoh      (47522)        0 2018-03-04 16:37:40.000000 datalad-0.9.3/datalad/downloaders/tests/__init__.py
+-rw-------   0 yoh      (47521) yoh      (47522)     1241 2018-03-04 16:37:40.000000 datalad-0.9.3/datalad/downloaders/tests/utils.py
+-rw-------   0 yoh      (47521) yoh      (47522)     3508 2018-03-04 16:37:40.000000 datalad-0.9.3/datalad/downloaders/tests/test_providers.py
+-rw-------   0 yoh      (47521) yoh      (47522)    18778 2018-03-04 16:37:40.000000 datalad-0.9.3/datalad/downloaders/tests/test_http.py
+-rw-------   0 yoh      (47521) yoh      (47522)    20844 2018-03-04 16:37:40.000000 datalad-0.9.3/datalad/downloaders/http.py
+drwx------   0 yoh      (47521) yoh      (47522)        0 2018-03-16 22:27:17.000000 datalad-0.9.3/datalad/downloaders/configs/
+-rw-------   0 yoh      (47521) yoh      (47522)      350 2018-03-04 16:37:40.000000 datalad-0.9.3/datalad/downloaders/configs/openfmri.cfg
+-rw-------   0 yoh      (47521) yoh      (47522)      883 2018-03-04 16:37:40.000000 datalad-0.9.3/datalad/downloaders/configs/nda.cfg
+-rw-------   0 yoh      (47521) yoh      (47522)     1633 2018-03-04 16:37:40.000000 datalad-0.9.3/datalad/downloaders/configs/nitrc.cfg
+-rw-------   0 yoh      (47521) yoh      (47522)      203 2018-03-04 16:37:40.000000 datalad-0.9.3/datalad/downloaders/configs/indi.cfg
+-rw-------   0 yoh      (47521) yoh      (47522)     1801 2018-03-04 16:37:40.000000 datalad-0.9.3/datalad/downloaders/configs/crcns.cfg
+-rw-------   0 yoh      (47521) yoh      (47522)      594 2018-03-04 16:37:40.000000 datalad-0.9.3/datalad/downloaders/configs/kaggle.cfg
+-rw-------   0 yoh      (47521) yoh      (47522)      289 2018-03-04 16:37:40.000000 datalad-0.9.3/datalad/downloaders/configs/providers.cfg
+-rw-------   0 yoh      (47521) yoh      (47522)     1874 2018-03-04 16:37:40.000000 datalad-0.9.3/datalad/downloaders/configs/hcp.cfg
+-rw-------   0 yoh      (47521) yoh      (47522)      200 2018-03-04 16:37:40.000000 datalad-0.9.3/datalad/downloaders/configs/crawdad.cfg
+-rw-------   0 yoh      (47521) yoh      (47522)    14362 2018-03-04 16:37:40.000000 datalad-0.9.3/datalad/downloaders/providers.py
+-rw-------   0 yoh      (47521) yoh      (47522)      744 2018-03-04 16:37:40.000000 datalad-0.9.3/datalad/downloaders/__init__.py
+-rw-------   0 yoh      (47521) yoh      (47522)     9280 2018-03-04 16:37:40.000000 datalad-0.9.3/datalad/downloaders/s3.py
+-rw-------   0 yoh      (47521) yoh      (47522)    10938 2018-03-04 16:37:40.000000 datalad-0.9.3/datalad/downloaders/credentials.py
+-rw-------   0 yoh      (47521) yoh      (47522)     3069 2018-03-04 16:37:39.000000 datalad-0.9.3/datalad/api.py
+drwx------   0 yoh      (47521) yoh      (47522)        0 2018-03-16 22:27:17.000000 datalad-0.9.3/datalad/metadata/
+drwx------   0 yoh      (47521) yoh      (47522)        0 2018-03-16 22:27:17.000000 datalad-0.9.3/datalad/metadata/tests/
+-rw-------   0 yoh      (47521) yoh      (47522)    15618 2018-03-04 16:37:40.000000 datalad-0.9.3/datalad/metadata/tests/test_base.py
+-rw-------   0 yoh      (47521) yoh      (47522)    10395 2018-03-04 16:37:40.000000 datalad-0.9.3/datalad/metadata/tests/test_manipulation.py
+-rw-------   0 yoh      (47521) yoh      (47522)     6231 2018-03-04 16:37:40.000000 datalad-0.9.3/datalad/metadata/tests/test_search.py
+-rw-------   0 yoh      (47521) yoh      (47522)        0 2018-03-04 16:37:40.000000 datalad-0.9.3/datalad/metadata/tests/__init__.py
+-rw-------   0 yoh      (47521) yoh      (47522)     9176 2018-03-04 16:37:40.000000 datalad-0.9.3/datalad/metadata/aggregate.py
+drwx------   0 yoh      (47521) yoh      (47522)        0 2018-03-16 22:27:17.000000 datalad-0.9.3/datalad/metadata/parsers/
+-rw-------   0 yoh      (47521) yoh      (47522)     2359 2018-03-04 16:37:40.000000 datalad-0.9.3/datalad/metadata/parsers/base.py
+drwx------   0 yoh      (47521) yoh      (47522)        0 2018-03-16 22:27:17.000000 datalad-0.9.3/datalad/metadata/parsers/tests/
+-rw-------   0 yoh      (47521) yoh      (47522)     2935 2018-03-04 16:37:40.000000 datalad-0.9.3/datalad/metadata/parsers/tests/test_datacite_xml.py
+-rw-------   0 yoh      (47521) yoh      (47522)     2866 2018-03-04 16:37:40.000000 datalad-0.9.3/datalad/metadata/parsers/tests/test_frictionless_datapackage.py
+-rw-------   0 yoh      (47521) yoh      (47522)      412 2018-03-04 16:37:40.000000 datalad-0.9.3/datalad/metadata/parsers/tests/__init__.py
+-rw-------   0 yoh      (47521) yoh      (47522)     3457 2018-03-04 16:37:40.000000 datalad-0.9.3/datalad/metadata/parsers/tests/test_rfc822.py
+-rw-------   0 yoh      (47521) yoh      (47522)     1406 2018-03-04 16:37:40.000000 datalad-0.9.3/datalad/metadata/parsers/tests/test_aggregate.py
+-rw-------   0 yoh      (47521) yoh      (47522)     3810 2018-03-04 16:37:40.000000 datalad-0.9.3/datalad/metadata/parsers/tests/test_bids.py
+-rw-------   0 yoh      (47521) yoh      (47522)     3628 2018-03-04 16:37:40.000000 datalad-0.9.3/datalad/metadata/parsers/datalad_rfc822.py
+-rw-------   0 yoh      (47521) yoh      (47522)     3755 2018-03-04 16:37:40.000000 datalad-0.9.3/datalad/metadata/parsers/aggregate.py
+-rw-------   0 yoh      (47521) yoh      (47522)     2279 2018-03-04 16:37:40.000000 datalad-0.9.3/datalad/metadata/parsers/frictionless_datapackage.py
+-rw-------   0 yoh      (47521) yoh      (47522)      619 2018-03-04 16:37:40.000000 datalad-0.9.3/datalad/metadata/parsers/__init__.py
+-rw-------   0 yoh      (47521) yoh      (47522)     4027 2018-03-04 16:37:40.000000 datalad-0.9.3/datalad/metadata/parsers/datacite.py
+-rw-------   0 yoh      (47521) yoh      (47522)     2750 2018-03-04 16:37:40.000000 datalad-0.9.3/datalad/metadata/parsers/bids.py
+-rw-------   0 yoh      (47521) yoh      (47522)    11907 2018-03-04 16:37:40.000000 datalad-0.9.3/datalad/metadata/__init__.py
+-rw-------   0 yoh      (47521) yoh      (47522)    20445 2018-03-16 22:26:59.000000 datalad-0.9.3/datalad/metadata/metadata.py
+-rw-------   0 yoh      (47521) yoh      (47522)    17723 2018-03-04 16:37:40.000000 datalad-0.9.3/datalad/metadata/search.py
+-rw-------   0 yoh      (47521) yoh      (47522)    42364 2018-03-04 16:37:40.000000 datalad-0.9.3/datalad/utils.py
+drwx------   0 yoh      (47521) yoh      (47522)        0 2018-03-16 22:27:17.000000 datalad-0.9.3/datalad/distribution/
+drwx------   0 yoh      (47521) yoh      (47522)        0 2018-03-16 22:27:17.000000 datalad-0.9.3/datalad/distribution/tests/
+-rw-------   0 yoh      (47521) yoh      (47522)    22962 2018-03-04 16:37:40.000000 datalad-0.9.3/datalad/distribution/tests/test_create_sibling.py
+-rw-------   0 yoh      (47521) yoh      (47522)    13503 2018-03-04 16:37:40.000000 datalad-0.9.3/datalad/distribution/tests/test_update.py
+-rw-------   0 yoh      (47521) yoh      (47522)     3276 2018-03-04 16:37:40.000000 datalad-0.9.3/datalad/distribution/tests/test_create_github.py
+-rw-------   0 yoh      (47521) yoh      (47522)     3143 2018-03-04 16:37:40.000000 datalad-0.9.3/datalad/distribution/tests/test_create_test_dataset.py
+-rw-------   0 yoh      (47521) yoh      (47522)     2908 2018-03-04 16:37:40.000000 datalad-0.9.3/datalad/distribution/tests/test_utils.py
+-rw-------   0 yoh      (47521) yoh      (47522)     1569 2018-03-04 16:37:40.000000 datalad-0.9.3/datalad/distribution/tests/test_dataset_binding.py
+-rw-------   0 yoh      (47521) yoh      (47522)     6735 2018-03-04 16:37:40.000000 datalad-0.9.3/datalad/distribution/tests/test_subdataset.py
+-rw-------   0 yoh      (47521) yoh      (47522)    27076 2018-03-04 16:37:40.000000 datalad-0.9.3/datalad/distribution/tests/test_publish.py
+-rw-------   0 yoh      (47521) yoh      (47522)    10489 2018-03-04 16:37:40.000000 datalad-0.9.3/datalad/distribution/tests/test_dataset.py
+-rw-------   0 yoh      (47521) yoh      (47522)    33997 2018-03-04 16:37:40.000000 datalad-0.9.3/datalad/distribution/tests/test_install.py
+-rw-------   0 yoh      (47521) yoh      (47522)      452 2018-03-04 16:37:40.000000 datalad-0.9.3/datalad/distribution/tests/__init__.py
+-rw-------   0 yoh      (47521) yoh      (47522)    19339 2018-03-04 16:37:40.000000 datalad-0.9.3/datalad/distribution/tests/test_get.py
+-rw-------   0 yoh      (47521) yoh      (47522)     9059 2018-03-04 16:37:40.000000 datalad-0.9.3/datalad/distribution/tests/test_siblings.py
+-rw-------   0 yoh      (47521) yoh      (47522)    20126 2018-03-16 22:26:59.000000 datalad-0.9.3/datalad/distribution/tests/test_uninstall.py
+-rw-------   0 yoh      (47521) yoh      (47522)    11123 2018-03-04 16:37:40.000000 datalad-0.9.3/datalad/distribution/tests/test_create.py
+-rw-------   0 yoh      (47521) yoh      (47522)     1277 2018-03-04 16:37:40.000000 datalad-0.9.3/datalad/distribution/tests/test_dataset_config.py
+-rw-------   0 yoh      (47521) yoh      (47522)    12543 2018-03-04 16:37:40.000000 datalad-0.9.3/datalad/distribution/tests/test_clone.py
+-rw-------   0 yoh      (47521) yoh      (47522)    13433 2018-03-04 16:37:40.000000 datalad-0.9.3/datalad/distribution/tests/test_add.py
+-rw-------   0 yoh      (47521) yoh      (47522)    36866 2018-03-16 22:26:59.000000 datalad-0.9.3/datalad/distribution/publish.py
+-rw-------   0 yoh      (47521) yoh      (47522)    34419 2018-03-04 16:37:40.000000 datalad-0.9.3/datalad/distribution/create_sibling.py
+-rw-------   0 yoh      (47521) yoh      (47522)    17452 2018-03-04 16:37:40.000000 datalad-0.9.3/datalad/distribution/subdatasets.py
+-rw-------   0 yoh      (47521) yoh      (47522)    33694 2018-03-04 16:37:40.000000 datalad-0.9.3/datalad/distribution/siblings.py
+-rw-------   0 yoh      (47521) yoh      (47522)    14779 2018-03-16 22:26:59.000000 datalad-0.9.3/datalad/distribution/remove.py
+-rw-------   0 yoh      (47521) yoh      (47522)     1032 2018-03-04 16:37:40.000000 datalad-0.9.3/datalad/distribution/add_sibling.py
+-rw-------   0 yoh      (47521) yoh      (47522)     6562 2018-03-04 16:37:40.000000 datalad-0.9.3/datalad/distribution/create_test_dataset.py
+-rw-------   0 yoh      (47521) yoh      (47522)    15482 2018-03-04 16:37:40.000000 datalad-0.9.3/datalad/distribution/create_sibling_github.py
+-rw-------   0 yoh      (47521) yoh      (47522)    19940 2018-03-04 16:37:40.000000 datalad-0.9.3/datalad/distribution/install.py
+-rw-------   0 yoh      (47521) yoh      (47522)     8188 2018-03-16 22:26:59.000000 datalad-0.9.3/datalad/distribution/drop.py
+-rw-------   0 yoh      (47521) yoh      (47522)     8996 2018-03-04 16:37:40.000000 datalad-0.9.3/datalad/distribution/uninstall.py
+-rw-------   0 yoh      (47521) yoh      (47522)    18620 2018-03-04 16:37:40.000000 datalad-0.9.3/datalad/distribution/dataset.py
+-rw-------   0 yoh      (47521) yoh      (47522)    29372 2018-03-16 22:26:59.000000 datalad-0.9.3/datalad/distribution/get.py
+-rw-------   0 yoh      (47521) yoh      (47522)      498 2018-03-04 16:37:39.000000 datalad-0.9.3/datalad/distribution/__init__.py
+-rw-------   0 yoh      (47521) yoh      (47522)    11979 2018-03-04 16:37:40.000000 datalad-0.9.3/datalad/distribution/clone.py
+-rw-------   0 yoh      (47521) yoh      (47522)     8479 2018-03-04 16:37:40.000000 datalad-0.9.3/datalad/distribution/update.py
+-rw-------   0 yoh      (47521) yoh      (47522)    24570 2018-03-16 22:26:59.000000 datalad-0.9.3/datalad/distribution/add.py
+-rw-------   0 yoh      (47521) yoh      (47522)     8057 2018-03-04 16:37:40.000000 datalad-0.9.3/datalad/distribution/utils.py
+-rw-------   0 yoh      (47521) yoh      (47522)    17186 2018-03-16 22:26:59.000000 datalad-0.9.3/datalad/distribution/create.py
+drwx------   0 yoh      (47521) yoh      (47522)        0 2018-03-16 22:27:17.000000 datalad-0.9.3/datalad/cmdline/
+drwx------   0 yoh      (47521) yoh      (47522)        0 2018-03-16 22:27:17.000000 datalad-0.9.3/datalad/cmdline/tests/
+-rw-------   0 yoh      (47521) yoh      (47522)      448 2018-03-04 16:37:39.000000 datalad-0.9.3/datalad/cmdline/tests/__init__.py
+-rw-------   0 yoh      (47521) yoh      (47522)     2744 2018-03-04 16:37:39.000000 datalad-0.9.3/datalad/cmdline/tests/test_helpers.py
+-rw-------   0 yoh      (47521) yoh      (47522)     3101 2018-03-04 16:37:39.000000 datalad-0.9.3/datalad/cmdline/tests/test_formatters.py
+-rw-------   0 yoh      (47521) yoh      (47522)     8463 2018-03-04 16:37:39.000000 datalad-0.9.3/datalad/cmdline/tests/test_main.py
+-rw-------   0 yoh      (47521) yoh      (47522)     9146 2018-03-04 16:37:39.000000 datalad-0.9.3/datalad/cmdline/helpers.py
+-rw-------   0 yoh      (47521) yoh      (47522)     2242 2018-03-04 16:37:39.000000 datalad-0.9.3/datalad/cmdline/common_args.py
+-rw-------   0 yoh      (47521) yoh      (47522)    17916 2018-03-04 16:37:39.000000 datalad-0.9.3/datalad/cmdline/main.py
+-rw-------   0 yoh      (47521) yoh      (47522)      433 2018-03-04 16:37:39.000000 datalad-0.9.3/datalad/cmdline/__init__.py
+-rw-------   0 yoh      (47521) yoh      (47522)     2090 2018-03-16 22:26:59.000000 datalad-0.9.3/datalad/version.py
+-rw-------   0 yoh      (47521) yoh      (47522)    10543 2018-03-04 16:37:40.000000 datalad-0.9.3/datalad/dochelpers.py
+-rw-------   0 yoh      (47521) yoh      (47522)    26600 2018-03-04 16:37:39.000000 datalad-0.9.3/datalad/cmd.py
+-rwx------   0 yoh      (47521) yoh      (47522)     5864 2018-03-16 22:26:59.000000 datalad-0.9.3/setup.py
```

### Comparing `datalad-0.9.2/setup_support.py` & `datalad-0.9.3/setup_support.py`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/.travis.yml` & `datalad-0.9.3/.travis.yml`

 * *Files 4% similar despite different names*

```diff
@@ -72,14 +72,21 @@
     - DATALAD_TESTS_DATALADREMOTE=1
     - DATALAD_LOG_CMD_CWD=1
     - DATALAD_LOG_CMD_OUTPUTS=1
     - DATALAD_LOG_CMD_ENV=1
     - DATALAD_LOG_CMD_STDIN=1
     - DATALAD_TESTS_UI_BACKEND=console
     - DATALAD_TESTS_OBSCURE_PREFIX=-
+    - DATALAD_SEED=1
+    - GIT_AUTHOR_DATE="Thu, 07 Apr 2005 22:13:13 +0200"
+    - GIT_AUTHOR_NAME=blah
+    - GIT_AUTHOR_EMAIL=committer@example.com
+    - GIT_COMMITTER_DATE="Thu, 07 Apr 2005 22:13:13 +0200"
+    - GIT_COMMITTER_NAME=blah
+    - GIT_COMMITTER_EMAIL=committer@example.com
   - python: 2.7
     env:
     # to test operation under root since also would consider FS "crippled" due to
     # ability to rewrite R/O files
     - NOSE_WRAPPER="sudo -E"
     # no key authentication for root:
     - DATALAD_TESTS_SSH=0
```

### Comparing `datalad-0.9.2/Makefile` & `datalad-0.9.3/Makefile`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/docs/Makefile` & `datalad-0.9.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/docs/config-format.rst` & `datalad-0.9.3/docs/config-format.rst`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/docs/design.rst` & `datalad-0.9.3/docs/design.rst`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/docs/datalad-metadata.rst` & `datalad-0.9.3/docs/datalad-metadata.rst`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/docs/examples/nipype_workshop_dataset.sh` & `datalad-0.9.3/docs/examples/nipype_workshop_dataset.sh`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/docs/examples/make_pymvpa_collection.sh_broken` & `datalad-0.9.3/docs/examples/make_pymvpa_collection.sh_broken`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/docs/examples/make_large_bogus_collection.sh_broken` & `datalad-0.9.3/docs/examples/make_large_bogus_collection.sh_broken`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/docs/examples/3rdparty_analysis_workflow.sh` & `datalad-0.9.3/docs/examples/3rdparty_analysis_workflow.sh`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/docs/casts/boxcom.sh` & `datalad-0.9.3/docs/casts/boxcom.sh`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/docs/casts/seamless_nested_repos.sh` & `datalad-0.9.3/docs/casts/seamless_nested_repos.sh`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/docs/casts/simple_provenance_tracking.sh` & `datalad-0.9.3/docs/casts/simple_provenance_tracking.sh`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/docs/casts/publish_on_github.sh` & `datalad-0.9.3/docs/casts/publish_on_github.sh`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/docs/casts/basic_search.sh` & `datalad-0.9.3/docs/casts/basic_search.sh`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/docs/casts/track_data_from_webpage.sh` & `datalad-0.9.3/docs/casts/track_data_from_webpage.sh`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/docs/casts/cmdline_basic_usage.sh` & `datalad-0.9.3/docs/casts/cmdline_basic_usage.sh`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/docs/casts/reproducible_analysis.sh` & `datalad-0.9.3/docs/casts/reproducible_analysis.sh`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/docs/casts/heudiconv_dicom_to_bids.sh` & `datalad-0.9.3/docs/casts/heudiconv_dicom_to_bids.sh`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/docs/source/customization.rst` & `datalad-0.9.3/docs/source/customization.rst`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/docs/source/index.rst` & `datalad-0.9.3/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/docs/source/changelog.rst` & `datalad-0.9.3/docs/source/changelog.rst`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/docs/source/_extras/schema.json` & `datalad-0.9.3/docs/source/_extras/schema.json`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/docs/source/glossary.rst` & `datalad-0.9.3/docs/source/glossary.rst`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/docs/source/gettingstarted.rst` & `datalad-0.9.3/docs/source/gettingstarted.rst`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/docs/source/metadata.rst` & `datalad-0.9.3/docs/source/metadata.rst`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/docs/source/config.rst` & `datalad-0.9.3/docs/source/config.rst`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/docs/source/modref.rst` & `datalad-0.9.3/docs/source/modref.rst`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/docs/source/crawler/basics.rst` & `datalad-0.9.3/docs/source/crawler/basics.rst`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/docs/source/acknowledgements.rst` & `datalad-0.9.3/docs/source/acknowledgements.rst`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/docs/source/conf.py` & `datalad-0.9.3/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/docs/source/basics.rst` & `datalad-0.9.3/docs/source/basics.rst`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/docs/source/_static/datalad_logo.png` & `datalad-0.9.3/docs/source/_static/datalad_logo.png`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/docs/source/faq.rst` & `datalad-0.9.3/docs/source/faq.rst`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/docs/source/related.rst` & `datalad-0.9.3/docs/source/related.rst`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/docs/source/cmdline.rst` & `datalad-0.9.3/docs/source/cmdline.rst`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/docs/source/background.rst` & `datalad-0.9.3/docs/source/background.rst`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/PKG-INFO` & `datalad-0.9.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: datalad
-Version: 0.9.2
+Version: 0.9.3
 Summary: data distribution geared toward scientific datasets
 Home-page: UNKNOWN
 Author: The DataLad Team and Contributors
 Author-email: team@datalad.org
 License: UNKNOWN
 Description-Content-Type: UNKNOWN
 Description: ::
```

### Comparing `datalad-0.9.2/tox.ini` & `datalad-0.9.3/tox.ini`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/tools/mimic_repo` & `datalad-0.9.3/tools/mimic_repo`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/tools/cmdline-completion` & `datalad-0.9.3/tools/cmdline-completion`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/tools/eval_under_testloopfs` & `datalad-0.9.3/tools/eval_under_testloopfs`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/tools/git-web-submodules.sh` & `datalad-0.9.3/tools/git-web-submodules.sh`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/tools/testing/test_README_in_docker` & `datalad-0.9.3/tools/testing/test_README_in_docker`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/tools/testing/start_website_in_docker` & `datalad-0.9.3/tools/testing/start_website_in_docker`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/tools/testing/test_README_in_docker-Dockerfile.in` & `datalad-0.9.3/tools/testing/test_README_in_docker-Dockerfile.in`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/tools/testing/run_doc_examples` & `datalad-0.9.3/tools/testing/run_doc_examples`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/tools/testing/make_test_repo` & `datalad-0.9.3/tools/testing/make_test_repo`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/tools/testing/start_website_in_docker-Dockerfile.in` & `datalad-0.9.3/tools/testing/start_website_in_docker-Dockerfile.in`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/tools/testing/make_test_repos` & `datalad-0.9.3/tools/testing/make_test_repos`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/tools/upgrade-annex-osx.sh` & `datalad-0.9.3/tools/upgrade-annex-osx.sh`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/tools/dtime` & `datalad-0.9.3/tools/dtime`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/tools/cast2narration` & `datalad-0.9.3/tools/cast2narration`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/tools/cast2script` & `datalad-0.9.3/tools/cast2script`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/tools/cast_live` & `datalad-0.9.3/tools/cast_live`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/tools/copy_urls_from_datalad.py` & `datalad-0.9.3/tools/copy_urls_from_datalad.py`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/tools/cast_bash.rc` & `datalad-0.9.3/tools/cast_bash.rc`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/tools/ci/gpg-90F7E9EB.pub` & `datalad-0.9.3/tools/ci/gpg-90F7E9EB.pub`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/tools/ci/install-annex-snapshot.sh` & `datalad-0.9.3/tools/ci/install-annex-snapshot.sh`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/tools/ci/prep-travis-devel-annex.sh` & `datalad-0.9.3/tools/ci/prep-travis-devel-annex.sh`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/tools/ci/prep-travis-forssh.sh` & `datalad-0.9.3/tools/ci/prep-travis-forssh.sh`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/tools/cast2asciinema` & `datalad-0.9.3/tools/cast2asciinema`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/tools/monitor-interrupts.py` & `datalad-0.9.3/tools/monitor-interrupts.py`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/tools/coverage-bin/git-annex-remote-datalad` & `datalad-0.9.3/tools/coverage-bin/git-annex-remote-datalad`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/tools/coverage-bin/git-annex-remote-datalad-archives` & `datalad-0.9.3/tools/coverage-bin/git-annex-remote-datalad-archives`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/tools/coverage-bin/datalad` & `datalad-0.9.3/tools/coverage-bin/datalad`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/tools/mimic_merges` & `datalad-0.9.3/tools/mimic_merges`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/tools/urlinfo` & `datalad-0.9.3/tools/urlinfo`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/CHANGELOG.md` & `datalad-0.9.3/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,43 @@
     |____/   \__,_|  \__|  \__,_| |_____|  \__,_|  \__,_|
                                                Change Log
 
 This is a high level and scarce summary of the changes between releases.
 We would recommend to consult log of the 
 [DataLad git repository](http://github.com/datalad/datalad) for more details.
 
+
+## 0.9.3 (Mar 16, 2018) -- pi+0.02 release
+
+Some important bug fixes which should improve usability
+
+### Fixes
+
+- `datalad-archives` special remote now will lock on acquiring or
+  extracting an archive - this allows for it to be used with -J flag
+  for parallel operation
+- relax introduced in 0.9.2 demand on git being configured for datalad
+  operation - now we will just issue a warning
+- `datalad ls` should now list "authored date" and work also for datasets
+  in detached HEAD mode
+- `datalad save` will now save original file as well, if file was
+  "git mv"ed, so you can now `datalad run git mv old new` and have
+  changes recorded
+
+### Enhancements and new features
+
+- `--jobs` argument now could take `auto` value which would decide on
+  # of jobs depending on the # of available CPUs.
+  `git-annex` > 6.20180314 is recommended to avoid regression with -J.
+- memoize calls to `RI` meta-constructor -- should speed up operation a
+  bit
+- `DATALAD_SEED` environment variable could be used to seed Python RNG
+  and provide reproducible UUIDs etc (useful for testing and demos)
+
+
 ## 0.9.2 (Mar 04, 2017) -- it is (again) better than ever
 
 Largely a bugfix release with a few enhancements.
 
 ### Fixes
 
 - Execution of external commands (git) should not get stuck when
```

### Comparing `datalad-0.9.2/COPYING` & `datalad-0.9.3/COPYING`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/README.md` & `datalad-0.9.3/README.md`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/CONTRIBUTING.md` & `datalad-0.9.3/CONTRIBUTING.md`

 * *Files 2% similar despite different names*

```diff
@@ -413,14 +413,18 @@
   Used to add timestamp to datalad logs
 - *DATALAD_LOG_TRACEBACK*:
   Runs TraceBack function with collide set to True, if this flag is set to 'collide'.
   This replaces any common prefix between current traceback log and previous invocation with "..."
 - *DATALAD_EXC_STR_TBLIMIT*: 
   This flag is used by the datalad extract_tb function which extracts and formats stack-traces.
   It caps the number of lines to DATALAD_EXC_STR_TBLIMIT of pre-processed entries from traceback.
+- *DATALAD_SEED*:
+  To seed Python's `random` RNG, which will also be used for generation of dataset UUIDs to make
+  those random values reproducible.  You might want also to set all the relevant git config variables
+  like we do in one of the travis runs
 - *DATALAD_TESTS_TEMP_KEEP*: 
   Function rmtemp will not remove temporary file/directory created for testing if this flag is set
 - *DATALAD_TESTS_TEMP_DIR*: 
   Create a temporary directory at location specified by this flag.
   It is used by tests to create a temporary git directory while testing git annex archives etc
 - *DATALAD_TESTS_NONETWORK*: 
   Skips network tests completely if this flag is set
@@ -457,15 +461,15 @@
   Instructs to use `git` as available in current environment, and not the one which possibly comes with git-annex (default behavior).
 
 
 # Changelog section
 
 For the upcoming release use this template
 
-## 0.9.3 (??? ??, 2017) -- will be better than ever
+## 0.9.4 (??? ??, 2018) -- will be better than ever
 
 bet we will fix some bugs and make a world even a better place.
 
 ### Major refactoring and deprecations
 
 - hopefully none
```

### Comparing `datalad-0.9.2/asv.conf.json` & `datalad-0.9.3/asv.conf.json`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/cfgs/openfmri-ds000001.cfg` & `datalad-0.9.3/cfgs/openfmri-ds000001.cfg`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/cfgs/nihhelpers.py` & `datalad-0.9.3/cfgs/nihhelpers.py`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/cfgs/nih-videos.cfg` & `datalad-0.9.3/cfgs/nih-videos.cfg`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/cfgs/arjlover-fast.cfg` & `datalad-0.9.3/cfgs/arjlover-fast.cfg`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/cfgs/common.cfg` & `datalad-0.9.3/cfgs/common.cfg`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/cfgs/allen-human.cfg` & `datalad-0.9.3/cfgs/allen-human.cfg`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/benchmarks/core.py` & `datalad-0.9.3/benchmarks/core.py`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/benchmarks/api.py` & `datalad-0.9.3/benchmarks/api.py`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/benchmarks/common.py` & `datalad-0.9.3/benchmarks/common.py`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/.mailmap` & `datalad-0.9.3/.mailmap`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/formatters.py` & `datalad-0.9.3/formatters.py`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/datalad.egg-info/PKG-INFO` & `datalad-0.9.3/datalad.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: datalad
-Version: 0.9.2
+Version: 0.9.3
 Summary: data distribution geared toward scientific datasets
 Home-page: UNKNOWN
 Author: The DataLad Team and Contributors
 Author-email: team@datalad.org
 License: UNKNOWN
 Description-Content-Type: UNKNOWN
 Description: ::
```

### Comparing `datalad-0.9.2/datalad.egg-info/requires.txt` & `datalad-0.9.3/datalad.egg-info/requires.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 GitPython>=2.1.8
 PyGithub
 appdirs
 boto
 duecredit
+fasteners
 humanize
 iso8601
 jsmin
 keyring>=8.0
 keyrings.alt
 mock>=1.0.1
 msgpack
@@ -17,14 +18,15 @@
 six>=1.8.0
 tqdm
 wrapt
 
 [core]
 GitPython>=2.1.8
 appdirs
+fasteners
 humanize
 iso8601
 mock>=1.0.1
 patool>=1.7
 six>=1.8.0
 tqdm
 wrapt
@@ -43,14 +45,16 @@
 PyYAML
 appdirs
 appdirs
 boto
 boto
 duecredit
 duecredit
+fasteners
+fasteners
 httpretty>=0.8.14
 httpretty>=0.8.14
 humanize
 humanize
 iso8601
 iso8601
 jsmin
@@ -118,14 +122,15 @@
 BeautifulSoup4
 GitPython>=2.1.8
 PyGithub
 PyYAML
 appdirs
 boto
 duecredit
+fasteners
 httpretty>=0.8.14
 humanize
 iso8601
 jsmin
 keyring>=8.0
 keyrings.alt
 mock
```

### Comparing `datalad-0.9.2/datalad.egg-info/SOURCES.txt` & `datalad-0.9.3/datalad.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -254,27 +254,29 @@
 datalad/resources/website/assets/js/md5-2.3.0.js
 datalad/resources/website/tests/test.html
 datalad/resources/website/tests/qunit/qunit-2.0.1.css
 datalad/resources/website/tests/qunit/qunit-2.0.1.js
 datalad/resources/website/tests/qunit/sinon-1.17.5.js
 datalad/resources/website/tests/qunit/sinon-qunit-1.0.0.js
 datalad/support/__init__.py
+datalad/support/_lru_cache2.py
 datalad/support/annexrepo.py
 datalad/support/ansi_colors.py
 datalad/support/archives.py
 datalad/support/cache.py
 datalad/support/configparserinc.py
 datalad/support/constraints.py
 datalad/support/cookies.py
 datalad/support/digests.py
 datalad/support/exceptions.py
 datalad/support/external_versions.py
 datalad/support/gitrepo.py
 datalad/support/json_py.py
 datalad/support/keyring_.py
+datalad/support/locking.py
 datalad/support/nda_.py
 datalad/support/network.py
 datalad/support/param.py
 datalad/support/protocol.py
 datalad/support/repo.py
 datalad/support/s3.py
 datalad/support/sshconnector.py
@@ -287,14 +289,15 @@
 datalad/support/tests/__init__.py
 datalad/support/tests/test_annexrepo.py
 datalad/support/tests/test_cache.py
 datalad/support/tests/test_digests.py
 datalad/support/tests/test_external_versions.py
 datalad/support/tests/test_gitrepo.py
 datalad/support/tests/test_json_py.py
+datalad/support/tests/test_locking.py
 datalad/support/tests/test_network.py
 datalad/support/tests/test_sshconnector.py
 datalad/support/tests/test_sshrun.py
 datalad/support/tests/test_stats.py
 datalad/support/tests/test_status.py
 datalad/support/tests/test_vcr_.py
 datalad/support/tests/test_versions.py
```

### Comparing `datalad-0.9.2/datalad/tests/test_base.py` & `datalad-0.9.3/datalad/tests/test_base.py`

 * *Files 22% similar despite different names*

```diff
@@ -9,18 +9,23 @@
 
 import os
 
 from .utils import (
     chpwd,
     get_dataset_root,
     with_tree,
+    swallow_logs,
 
     assert_raises,
     assert_equal,
+    assert_in,
 )
+from datalad.support.gitrepo import check_git_configured
+
+from mock import patch
 
 
 #@with_tempfile(mkdir=True)
 # with_tempfile dereferences tempdir, so does not trigger the failure
 # on Yarik's laptop where TMPDIR=~/.tmp and ~/.tmp -> /tmp.
 # with_tree in turn just passes that ~/.tmp/ directory
 @with_tree(tree={})
@@ -35,19 +40,29 @@
             require_dataset,
             None, check_installed=True, purpose='test'
         )
 
 
 def test_git_config_fixture():
     # in the setup_package we setup a new HOME with custom config
-    from datalad.support.gitrepo import check_git_configured
     if 'GIT_HOME' not in os.environ:
         assert_equal(
             check_git_configured(),
             {
                 'user.name': 'DataLad Tester',
                 'user.email': 'test@example.com'
              }
         )
     else:
         # we pick up the ones in the 'GIT_HOME' which might differ
         assert_equal(sorted(check_git_configured()), ['user.email', 'user.name'])
+
+
+@with_tree(tree={})
+def test_git_config_warning(path):
+    with chpwd(path), \
+            patch.dict('os.environ', {'HOME': path}), \
+            swallow_logs(new_level=30) as cml:
+        # no configs in that empty HOME
+        assert_equal(check_git_configured(), {})
+        assert_in("configure git first", cml.out)
+
```

### Comparing `datalad-0.9.2/datalad/tests/test_constraints.py` & `datalad-0.9.3/datalad/tests/test_constraints.py`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/datalad/tests/test_testrepos.py` & `datalad-0.9.3/datalad/tests/test_testrepos.py`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/datalad/tests/test_interface.py` & `datalad-0.9.3/datalad/tests/test_interface.py`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/datalad/tests/test__main__.py` & `datalad-0.9.3/datalad/tests/test__main__.py`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/datalad/tests/test_utils.py` & `datalad-0.9.3/datalad/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/datalad/tests/test_s3.py` & `datalad-0.9.3/datalad/tests/test_s3.py`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/datalad/tests/utils_testdatasets.py` & `datalad-0.9.3/datalad/tests/utils_testdatasets.py`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/datalad/tests/test_misc.py` & `datalad-0.9.3/datalad/tests/test_misc.py`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/datalad/tests/test_log.py` & `datalad-0.9.3/datalad/tests/test_log.py`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/datalad/tests/test_auto.py` & `datalad-0.9.3/datalad/tests/test_auto.py`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/datalad/tests/__init__.py` & `datalad-0.9.3/datalad/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/datalad/tests/test_tests_utils.py` & `datalad-0.9.3/datalad/tests/test_tests_utils.py`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/datalad/tests/test_archives.py` & `datalad-0.9.3/datalad/tests/test_archives.py`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/datalad/tests/test_config.py` & `datalad-0.9.3/datalad/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/datalad/tests/test_cmd.py` & `datalad-0.9.3/datalad/tests/test_cmd.py`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/datalad/tests/utils.py` & `datalad-0.9.3/datalad/tests/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1206,14 +1206,29 @@
     """Verify that the values of all results for a given key in the status dicts
     match the given sequence"""
     assert_equal(
         [r[prop] for r in results],
         values)
 
 
+def assert_result_values_cond(results, prop, cond):
+    """Verify that the values of all results for a given key in the status dicts
+    fullfill condition `cond`.
+
+    Parameters
+    ----------
+    results:
+    prop: str
+    cond: callable
+    """
+    for r in assure_list(results):
+        ok_(cond(r[prop]),
+            msg="r[{prop}]: {value}".format(prop=prop, value=r[prop]))
+
+
 def ignore_nose_capturing_stdout(func):
     """Decorator workaround for nose's behaviour with redirecting sys.stdout
 
     Needed for tests involving the runner and nose redirecting stdout.
     Counter-intuitively, that means it needed for nosetests without '-s'.
     See issue reported here:
     https://code.google.com/p/python-nose/issues/detail?id=243&can=1&sort=-id&colspec=ID%20Type%20Status%20Priority%20Stars%20Milestone%20Owner%20Summary
```

### Comparing `datalad-0.9.2/datalad/tests/utils_testrepos.py` & `datalad-0.9.3/datalad/tests/utils_testrepos.py`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/datalad/tests/test_utils_testrepos.py` & `datalad-0.9.3/datalad/tests/test_utils_testrepos.py`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/datalad/tests/test_api.py` & `datalad-0.9.3/datalad/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/datalad/tests/test_protocols.py` & `datalad-0.9.3/datalad/tests/test_protocols.py`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/datalad/tests/test_installed.py` & `datalad-0.9.3/datalad/tests/test_installed.py`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/datalad/tests/test_dochelpers.py` & `datalad-0.9.3/datalad/tests/test_dochelpers.py`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/datalad/tests/test_strings.py` & `datalad-0.9.3/datalad/tests/test_strings.py`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/datalad/tests/test_direct_mode.py` & `datalad-0.9.3/datalad/tests/test_direct_mode.py`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/datalad/interface/base.py` & `datalad-0.9.3/datalad/interface/base.py`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/datalad/interface/tests/test_save.py` & `datalad-0.9.3/datalad/interface/tests/test_save.py`

 * *Files 2% similar despite different names*

```diff
@@ -257,14 +257,29 @@
         # no explicit dataset is provided by path is provided
         save(path=['subsub'], message='saving sub', super_datasets=True)
     # super should get it saved too
     assert_equal(next(ds.repo.get_branch_commits('master')).message.rstrip(),
                  'saving sub')
 
 
+def test_renamed_file():
+    @with_tempfile()
+    def check_renamed_file(recursive, no_annex, path):
+        ds = Dataset(path).create(no_annex=no_annex)
+        create_tree(path, {'old': ''})
+        ds.add('old')
+        ds.repo._git_custom_command(['old', 'new'], ['git', 'mv'])
+        ds.save(recursive=recursive)
+        ok_clean_git(path)
+
+    for recursive in True, False:
+        for no_annex in True, False:
+            yield check_renamed_file, recursive, no_annex
+
+
 @with_tempfile(mkdir=True)
 @known_failure_direct_mode  #FIXME
 def test_subdataset_save(path):
     parent = Dataset(path).create()
     sub = parent.create('sub')
     ok_clean_git(parent.path)
     create_tree(parent.path, {
```

### Comparing `datalad-0.9.2/datalad/interface/tests/test_add_archive_content.py` & `datalad-0.9.3/datalad/interface/tests/test_add_archive_content.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,14 +25,15 @@
     with_tempfile, assert_in
 from ...tests.utils import assert_equal, assert_not_equal
 from ...tests.utils import assert_false
 from ...tests.utils import assert_true
 from ...tests.utils import ok_archives_caches
 from ...tests.utils import SkipTest
 from ...tests.utils import assert_re_in
+from datalad.tests.utils import assert_result_values_cond
 
 from ...support.annexrepo import AnnexRepo
 from ...support.exceptions import FileNotInRepositoryError
 from ...support.exceptions import CommandError
 from ...tests.utils import with_tree, serve_path_via_http, ok_file_under_git, swallow_outputs
 from ...tests.utils import swallow_logs
 from ...tests.utils import integration
@@ -290,15 +291,18 @@
     repo._annex_custom_command([], ["git", "annex", "drop", "--all"])
 
     # verify that we can't drop a file if archive key was dropped and online archive was removed or changed size! ;)
     repo.get(key_1tar, key=True)
     unlink(opj(path_orig, '1.tar.gz'))
     res = repo.drop(key_1tar, key=True)
     assert_equal(res['success'], False)
-    assert_equal(res['note'], '(Use --force to override this check, or adjust numcopies.)')
+    assert_result_values_cond(
+        [res], 'note',
+        lambda x: '(Use --force to override this check, or adjust numcopies.)' in x
+    )
     assert exists(opj(repo.path, repo.get_contentlocation(key_1tar)))
 
 
 @integration
 @assert_cwd_unchanged(ok_to_chdir=True)
 @with_tree(**tree1args)
 @serve_path_via_http()
```

### Comparing `datalad-0.9.2/datalad/interface/tests/test_ls.py` & `datalad-0.9.3/datalad/interface/tests/test_ls.py`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/datalad/interface/tests/test_utils.py` & `datalad-0.9.3/datalad/interface/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/datalad/interface/tests/test_crawl_init.py` & `datalad-0.9.3/datalad/interface/tests/test_crawl_init.py`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/datalad/interface/tests/test_unlock.py` & `datalad-0.9.3/datalad/interface/tests/test_unlock.py`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/datalad/interface/tests/test_diff.py` & `datalad-0.9.3/datalad/interface/tests/test_diff.py`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/datalad/interface/tests/test_annotate_paths.py` & `datalad-0.9.3/datalad/interface/tests/test_annotate_paths.py`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/datalad/interface/tests/test_docs.py` & `datalad-0.9.3/datalad/interface/tests/test_docs.py`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/datalad/interface/tests/test_ls_webui.py` & `datalad-0.9.3/datalad/interface/tests/test_ls_webui.py`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/datalad/interface/tests/test_download_url.py` & `datalad-0.9.3/datalad/interface/tests/test_download_url.py`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/datalad/interface/tests/test_crawl.py` & `datalad-0.9.3/datalad/interface/tests/test_crawl.py`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/datalad/interface/tests/test_run.py` & `datalad-0.9.3/datalad/interface/tests/test_run.py`

 * *Files 2% similar despite different names*

```diff
@@ -292,29 +292,33 @@
 def test_rerun_branch(path):
     ds = Dataset(path).create()
 
     ds.repo.repo.git.tag("prerun")
 
     outfile = opj(path, "run-file")
 
-    with open(opj(path, "nonrun-file"), "w") as f:
-        f.write("foo")
-    ds.add("nonrun-file")
-
     ds.run('echo x$(cat run-file) > run-file')
     ds.rerun()
     eq_('xx\n', open(outfile).read())
 
+    with open(opj(path, "nonrun-file"), "w") as f:
+        f.write("foo")
+    ds.add("nonrun-file")
+
     # Rerun the commands on a new branch that starts at the parent
     # commit of the first run.
     ds.rerun(since="prerun", onto="prerun", branch="rerun")
 
     eq_(ds.repo.get_active_branch(), "rerun")
     eq_('xx\n', open(outfile).read())
 
+    # NOTE: This test depends on the non-run commit above following a run
+    # commit.  Otherwise, all the metadata (e.g., author date) aside from the
+    # parent commit that is used to generate the commit ID may be set when
+    # running the tests, which would result in two commits rather than three.
     for revrange in ["rerun..master", "master..rerun"]:
         assert_result_count(
             ds.repo.repo.git.rev_list(revrange).split(), 3)
     eq_(ds.repo.get_merge_base(["master", "rerun"]),
         ds.repo.repo.git.rev_parse("prerun"))
 
     # Start rerun branch at tip of current branch.
```

### Comparing `datalad-0.9.2/datalad/interface/tests/test_clean.py` & `datalad-0.9.3/datalad/interface/tests/test_clean.py`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/datalad/interface/run.py` & `datalad-0.9.3/datalad/interface/run.py`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/datalad/interface/add_archive_content.py` & `datalad-0.9.3/datalad/interface/add_archive_content.py`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/datalad/interface/clean.py` & `datalad-0.9.3/datalad/interface/clean.py`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/datalad/interface/results.py` & `datalad-0.9.3/datalad/interface/results.py`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/datalad/interface/crawl.py` & `datalad-0.9.3/datalad/interface/crawl.py`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/datalad/interface/download_url.py` & `datalad-0.9.3/datalad/interface/download_url.py`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/datalad/interface/ls.py` & `datalad-0.9.3/datalad/interface/ls.py`

 * *Files 1% similar despite different names*

```diff
@@ -236,15 +236,15 @@
     def describe(self):
         return self.repo.describe(tags=True)
 
     @property
     def date(self):
         """Date of the last commit
         """
-        return self.repo.get_committed_date()
+        return self.repo.get_commit_date()
 
     @property
     def count_objects(self):
         return self.repo.count_objects
 
     @property
     def git_local_size(self):
@@ -306,15 +306,15 @@
 
     @property
     def date(self):
         """Date of last modification"""
         if self.type_ is not ['git', 'annex']:
             return lstat(self._path).st_mtime
         else:
-            super(self.__class__, self).date
+            return super(self.__class__, self).date
 
     @property
     def size(self):
         """Size of the node computed based on its type"""
         type_ = self.type_
         sizes = {'total': 0.0,
                  'ondisk': 0.0,
```

### Comparing `datalad-0.9.2/datalad/interface/__init__.py` & `datalad-0.9.3/datalad/interface/__init__.py`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/datalad/interface/unlock.py` & `datalad-0.9.3/datalad/interface/unlock.py`

 * *Files 1% similar despite different names*

```diff
@@ -97,16 +97,15 @@
                 # this is a dataset
                 ap['process_content'] = True
             to_process.append(ap)
 
         content_by_ds, ds_props, completed, nondataset_paths = \
             annotated2content_by_ds(
                 to_process,
-                refds_path=refds_path,
-                path_only=False)
+                refds_path=refds_path)
         assert(not completed)
 
         for ds_path in sorted(content_by_ds.keys()):
             ds = Dataset(ds_path)
             content = content_by_ds[ds_path]
 
             # no annex, no unlock:
```

### Comparing `datalad-0.9.2/datalad/interface/save.py` & `datalad-0.9.3/datalad/interface/save.py`

 * *Files 2% similar despite different names*

```diff
@@ -117,17 +117,27 @@
     if not message:
         message = 'Recorded existing changes'
         _datalad_msg = True
 
     # we will blindly call commit not knowing if there is anything to
     # commit -- this is cheaper than to anticipate all possible ways
     # a repo in whatever mode is dirty
+    paths_to_commit = None
+    if not save_entire_ds:
+        paths_to_commit = []
+        for ap in paths:
+            paths_to_commit.append(ap['path'])
+            # was file renamed?
+            path_src = ap.get('path_src')
+            if path_src and path_src != ap['path']:
+                paths_to_commit.append(path_src)
+
     ds.repo.commit(
         message,
-        files=[ap['path'] for ap in paths] if not save_entire_ds else None,
+        files=paths_to_commit,
         _datalad_msg=_datalad_msg,
         careless=True)
 
     current_hexsha = ds.repo.get_hexsha()
     _was_modified = current_hexsha != orig_hexsha
     return current_hexsha if _was_modified else None
 
@@ -244,15 +254,15 @@
             if ap['path'] == refds_path or \
                     (ap.get('type', None) == 'dataset' and
                      not ap.get('raw_input', False) and
                      not ap.get('state', None) == 'absent'):
                 ap['process_content'] = True
                 ap['process_updated_only'] = all_updated
             to_process.append(ap)
-
+        lgr.log(2, "save, to_process=%r", to_process)
         if got_nothing and recursive and refds_path:
             # path annotation yielded nothing, most likely cause is that nothing
             # was found modified, we need to say something about the reference
             # dataset
             yield get_status_dict(
                 'save',
                 status='notneeded',
@@ -343,16 +353,15 @@
             # if there is an error now, we made this mistake in here
             on_failure='stop')
 
         # now sort into datasets so we can process them one by one
         content_by_ds, ds_props, completed, nondataset_paths = \
             annotated2content_by_ds(
                 annotated_paths,
-                refds_path=refds_path,
-                path_only=False)
+                refds_path=refds_path)
         assert(not completed)
 
         # iterate over all datasets, starting at the bottom
         for dspath in sorted(content_by_ds.keys(), reverse=True):
             ds = Dataset(dspath)
             res = get_status_dict('save', ds=ds, logger=lgr)
             if not ds.is_installed():
```

### Comparing `datalad-0.9.2/datalad/interface/test.py` & `datalad-0.9.3/datalad/interface/test.py`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/datalad/interface/utils.py` & `datalad-0.9.3/datalad/interface/utils.py`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/datalad/interface/common_opts.py` & `datalad-0.9.3/datalad/interface/common_opts.py`

 * *Files 1% similar despite different names*

```diff
@@ -128,15 +128,16 @@
     of the dataset). Use with care, and limit to "read-only" use
     cases. With this flag the installed dataset will be marked as
     untrusted.""")
 
 jobs_opt = Parameter(
     args=("-J", "--jobs"),
     metavar="NJOBS",
-    constraints=EnsureInt() | EnsureNone(),
+    default=None,
+    constraints=EnsureInt() | EnsureNone() | EnsureChoice('auto'),
     doc="""how many parallel jobs (where possible) to use.""")
 
 verbose = Parameter(
     args=("-v", "--verbose",),
     action="store_true",
     doc="""print out more detailed information while executing a command""")
```

### Comparing `datalad-0.9.2/datalad/interface/annotate_paths.py` & `datalad-0.9.3/datalad/interface/annotate_paths.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 #   copyright and license terms.
 #
 # ## ### ### ### ### ### ### ### ### ### ### ### ### ### ### ### ### ### ### ##
 """Plumbing command for analyzing and acting upon input paths"""
 
 __docformat__ = 'restructuredtext'
 
+from collections import defaultdict
 
 import logging
 import textwrap
 
 from os import curdir
 from os.path import join as opj
 from os.path import lexists
@@ -64,86 +65,82 @@
         if a.get('type', None) == 'dataset':
             dp = props.get(a['path'], {})
             dp.update(a)
             props[a['path']]
     return props
 
 
-def annotated2content_by_ds(annotated, refds_path, path_only=False):
+def annotated2content_by_ds(annotated, refds_path):
     """Helper to convert annotated paths into an old-style content_by_ds dict
 
     Only items with an `status` property value not equal to 'ok', 'notneeded',
     'impossible', or 'error' are sorted. All others are considered as
     already processed and are returned in a separate list.
 
     Parameters
     ----------
     annotated : list or generator
       Dicts with annotated path information.
     refds_path : str
       Path to the reference dataset the original path annotation was based on.
-    path_only: bool
-      Whether returned dict values are sequences of just paths for each
-      dataset, or whether the full info dicts are reported as items.
 
     Returns
     -------
     dict, dict, list, list
-      Dict keys are dataset paths, values are determined by the `path_only`
-      switch. The keys in the second dict are paths to dataset, values are
+      Dict keys are dataset paths, values are full info dicts.
+      The keys in the second dict are paths to dataset, values are
       dicts with all known properties about those datasets.
       The first list contains all already "processed" results, which
       typically need to be re-yielded. The second list contains items (same
       type as dict values) for all annotated paths that have no associated
       parent dataset (i.e. nondataset paths) -- this list will be empty by
       default, unless `nondataset_path_status` was set to ''."""
-    content_by_ds = {}
+    content_by_ds = defaultdict(list)
     ds_props = {}
     nondataset_paths = []
     completed = []
     for r in annotated:
+        r_path = r['path']
         if r.get('type', None) == 'dataset':
             # collect all properties of all known datasets from the annotated
             # paths
-            dp = ds_props.get(r['path'], {})
+            dp = ds_props.get(r_path, {})
             dp.update(r)
-            ds_props[r['path']] = dp
+            ds_props[r_path] = dp
         if r.get('status', None) in ('ok', 'notneeded', 'impossible', 'error'):
             completed.append(r)
             continue
         parentds = r.get('parentds', None)
+        appendto = []  # what entries, if any, to append r to
         if r.get('type', None) == 'dataset':
             # to dataset handling first, it is the more complex beast
             orig_request = r.get('orig_request', None)
             if parentds is None or refds_path is None or \
                     r.get('process_content', False) or (orig_request and (
                     orig_request == curdir or
                     orig_request.endswith(dirsep) or
                     orig_request.endswith('{}{}'.format(dirsep, curdir)))):
                 # a dataset that floats by on its own OR
                 # behave similar to rsync, a trailing '/' indicates the
                 # content rather then the dataset itself
                 # in both cases we want to process this part as part
                 # of the same dataset, and not any potential parent
-                toappendto = content_by_ds.get(r['path'], [])
-                toappendto.append(r['path'] if path_only else r)
-                content_by_ds[r['path']] = toappendto
+                appendto += [r_path]
             if parentds and refds_path and \
                     path_startswith(parentds, refds_path):
                 # put also in parentds record if there is any, and the parent
                 # is underneath or identical to the reference dataset
-                toappendto = content_by_ds.get(parentds, [])
-                toappendto.append(r['path'] if path_only else r)
-                content_by_ds[parentds] = toappendto
+                appendto += [parentds]
         else:
             # files and dirs
             # common case, something with a parentds
-            toappendto = content_by_ds.get(parentds, [])
-            toappendto.append(r['path'] if path_only else r)
-            content_by_ds[parentds] = toappendto
+            appendto += [parentds]
+
+        for e in appendto:
+            content_by_ds[e] += [r]
 
     return content_by_ds, ds_props, completed, nondataset_paths
 
 
 def yield_recursive(ds, path, action, recursion_limit):
     # make sure we get everything relevant in all _checked out_
     # subdatasets, obtaining of previously unavailable subdataset
```

### Comparing `datalad-0.9.2/datalad/interface/diff.py` & `datalad-0.9.3/datalad/interface/diff.py`

 * *Files 0% similar despite different names*

```diff
@@ -332,16 +332,15 @@
                            else ap['parentds']] = revision
             to_process.append(ap)
 
         # sort into datasets
         content_by_ds, ds_props, completed, nondataset_paths = \
             annotated2content_by_ds(
                 to_process,
-                refds_path=refds_path,
-                path_only=False)
+                refds_path=refds_path)
         assert(not completed)
 
         for ds_path in sorted(content_by_ds.keys()):
             if ds_path not in ds_diffies:
                 # we don't know how to diff
                 # this was not neither an input path, not did we see it
                 # when diffing its parent
```

### Comparing `datalad-0.9.2/datalad/interface/common_cfg.py` & `datalad-0.9.3/datalad/interface/common_cfg.py`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/datalad/interface/crawl_init.py` & `datalad-0.9.3/datalad/interface/crawl_init.py`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/datalad/interface/ls_webui.py` & `datalad-0.9.3/datalad/interface/ls_webui.py`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/datalad/interface/rerun.py` & `datalad-0.9.3/datalad/interface/rerun.py`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/datalad/__main__.py` & `datalad-0.9.3/datalad/__main__.py`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/datalad/resources/website/tests/test.html` & `datalad-0.9.3/datalad/resources/website/tests/test.html`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/datalad/resources/website/tests/qunit/sinon-1.17.5.js` & `datalad-0.9.3/datalad/resources/website/tests/qunit/sinon-1.17.5.js`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/datalad/resources/website/tests/qunit/qunit-2.0.1.js` & `datalad-0.9.3/datalad/resources/website/tests/qunit/qunit-2.0.1.js`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/datalad/resources/website/tests/qunit/qunit-2.0.1.css` & `datalad-0.9.3/datalad/resources/website/tests/qunit/qunit-2.0.1.css`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/datalad/resources/website/tests/qunit/sinon-qunit-1.0.0.js` & `datalad-0.9.3/datalad/resources/website/tests/qunit/sinon-qunit-1.0.0.js`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/datalad/resources/website/assets/images/logo_wide.svg` & `datalad-0.9.3/datalad/resources/website/assets/images/logo_wide.svg`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/datalad/resources/website/assets/images/favicon.ico` & `datalad-0.9.3/datalad/resources/website/assets/images/favicon.ico`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/datalad/resources/website/assets/images/favicon.svg` & `datalad-0.9.3/datalad/resources/website/assets/images/favicon.svg`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/datalad/resources/website/assets/js/md5-2.3.0.js` & `datalad-0.9.3/datalad/resources/website/assets/js/md5-2.3.0.js`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/datalad/resources/website/assets/js/main.js` & `datalad-0.9.3/datalad/resources/website/assets/js/main.js`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/datalad/resources/website/assets/js/jquery.dataTables-1.10.12.js` & `datalad-0.9.3/datalad/resources/website/assets/js/jquery.dataTables-1.10.12.js`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/datalad/resources/website/assets/js/jquery-2.2.4.js` & `datalad-0.9.3/datalad/resources/website/assets/js/jquery-2.2.4.js`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/datalad/resources/website/assets/css/jquery.dataTables-1.10.12.css` & `datalad-0.9.3/datalad/resources/website/assets/css/jquery.dataTables-1.10.12.css`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/datalad/resources/website/index.html` & `datalad-0.9.3/datalad/resources/website/index.html`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/datalad/customremotes/base.py` & `datalad-0.9.3/datalad/customremotes/base.py`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/datalad/customremotes/tests/test_base.py` & `datalad-0.9.3/datalad/customremotes/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/datalad/customremotes/tests/__init__.py` & `datalad-0.9.3/datalad/customremotes/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/datalad/customremotes/tests/test_archives.py` & `datalad-0.9.3/datalad/customremotes/tests/test_archives.py`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/datalad/customremotes/tests/test_datalad.py` & `datalad-0.9.3/datalad/customremotes/tests/test_datalad.py`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/datalad/customremotes/main.py` & `datalad-0.9.3/datalad/customremotes/main.py`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/datalad/customremotes/datalad.py` & `datalad-0.9.3/datalad/customremotes/datalad.py`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/datalad/customremotes/archives.py` & `datalad-0.9.3/datalad/customremotes/archives.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 lgr = logging.getLogger('datalad.customremotes.archive')
 lgr.log(5, "Importing datalad.customremotes.archive")
 
 from ..dochelpers import exc_str
 from ..cmd import link_file_load
 from ..support.archives import ArchivesCache
 from ..support.network import URL
+from ..support.locking import lock_if_check_fails
 from ..utils import getpwd
 from ..utils import unique
 from .base import AnnexCustomRemote
 from .main import main as super_main
 
 
 # TODO: RF functionality not specific to being a custom remote (loop etc)
@@ -320,51 +321,36 @@
         akeys_tried = []
         # the same file could come from multiple files within the same archive
         # So far it doesn't make sense to "try all" of them since if one fails
         # it means the others would fail too, so it makes sense to immediately
         # prune the list so we keep only the ones from unique akeys.
         # May be whenever we support extraction directly from the tarballs
         # we should go through all and choose the one easiest to get or smth.
-        from humanize import naturalsize
         for akey, afile in self._gen_akey_afiles(key, sorted=True, unique_akeys=True):
             if not akey:
                 lgr.warning("Got an empty archive key %r for key %s. Skipping",
                             akey, key)
                 continue
             akeys_tried.append(akey)
             try:
-                akey_fpath = self.get_contentlocation(akey)
+                with lock_if_check_fails(
+                    check=(self.get_contentlocation, (akey,)),
+                    lock_path=(lambda k: opj(self.repo.path, '.git', 'datalad-archives-%s' % k), (akey,)),
+                    operation="annex-get"
+                ) as (akey_fpath, lock):
+                    if lock:
+                        assert not akey_fpath
+                        self._annex_get_archive_by_key(akey)
+                        akey_fpath = self.get_contentlocation(akey)
+
                 if not akey_fpath:
-                    # TODO: make it more stringent?
-                    # Command could have fail to run if key was not present locally yet
-                    # Thus retrieve the key using annex
-                    # TODO: we need to report user somehow about this happening and progress on the download
-                    akey_size = self.repo.get_size_from_key(akey)
-                    self.info(
-                        "To obtain some keys we need to fetch an archive "
-                        "of size %s"
-                        % (naturalsize(akey_size) if akey_size else "unknown")
-                    )
-
-                    def progress_indicators(l):
-                        self.info("PROGRESS-JSON: " + l.rstrip(os.linesep))
-
-                    self.runner(["git-annex", "get",
-                                 "--json", "--json-progress",
-                                 "--key", akey
-                                 ],
-                                log_stdout=progress_indicators,
-                                log_stderr='offline',
-                                # False, # to avoid lock down
-                                log_online=True,
-                                cwd=self.path, expect_stderr=True)
-
-                    akey_fpath = self.get_contentlocation(akey)
-                    if not akey_fpath:
-                        raise RuntimeError("We were reported to fetch it alright but now can't get its location.  Check logic")
+                    raise RuntimeError(
+                        "We were reported to fetch it alright but now can't "
+                        "get its location.  Check logic"
+                )
 
                 akey_path = opj(self.repo.path, akey_fpath)
                 assert exists(akey_path), "Key file %s is not present" % akey_path
 
                 # Extract that bloody file from the bloody archive
                 # TODO: implement/use caching, for now a simple one
                 #  actually patool doesn't support extraction of a single file
@@ -384,13 +370,40 @@
                 continue
 
         raise RuntimeError(
             "Failed to fetch any archive containing {key}. "
             "Tried: {akeys_tried}".format(**locals())
         )
 
+    def _annex_get_archive_by_key(self, akey):
+        # TODO: make it more stringent?
+        # Command could have fail to run if key was not present locally yet
+        # Thus retrieve the key using annex
+        # TODO: we need to report user somehow about this happening and
+        # progress on the download
+        from humanize import naturalsize
+        akey_size = self.repo.get_size_from_key(akey)
+        self.info(
+            "To obtain some keys we need to fetch an archive "
+            "of size %s"
+            % (naturalsize(akey_size) if akey_size else "unknown")
+        )
+
+        def progress_indicators(l):
+            self.info("PROGRESS-JSON: " + l.rstrip(os.linesep))
+
+        self.runner(["git-annex", "get",
+                     "--json", "--json-progress",
+                     "--key", akey
+                     ],
+                    log_stdout=progress_indicators,
+                    log_stderr='offline',
+                    # False, # to avoid lock down
+                    log_online=True,
+                    cwd=self.path, expect_stderr=True)
+
 
 def main():
     """cmdline entry point"""
     super_main(backend="archive")
 
 lgr.log(5, "Done importing datalad.customremotes.archive")
```

### Comparing `datalad-0.9.2/datalad/plugin/tests/test_plugins.py` & `datalad-0.9.3/datalad/plugin/tests/test_plugins.py`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/datalad/plugin/tests/test_tarball.py` & `datalad-0.9.3/datalad/plugin/tests/test_tarball.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,15 +45,15 @@
     assert_raises(ValueError, plugin, 'export_tarball', Dataset('nowhere'))
 
 
 @with_tree(_dataset_template)
 def test_tarball(path):
     ds = Dataset(opj(path, 'ds')).create(force=True)
     ds.add('.')
-    committed_date = ds.repo.get_committed_date()
+    committed_date = ds.repo.get_commit_date()
     default_outname = opj(path, 'datalad_{}.tar.gz'.format(ds.id))
     with chpwd(path):
         res = list(ds.plugin('export_tarball'))
         assert_status('ok', res)
         assert_result_count(res, 1)
         assert(isabs(res[0]['path']))
     assert_true(os.path.exists(default_outname))
```

### Comparing `datalad-0.9.2/datalad/plugin/no_annex.py` & `datalad-0.9.3/datalad/plugin/no_annex.py`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/datalad/plugin/export_tarball.py` & `datalad-0.9.3/datalad/plugin/export_tarball.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     from datalad.utils import file_basename
     from datalad.support.annexrepo import AnnexRepo
 
     import logging
     lgr = logging.getLogger('datalad.plugin.tarball')
 
     repo = dataset.repo
-    committed_date = repo.get_committed_date()
+    committed_date = repo.get_commit_date()
 
     # could be used later on to filter files by some criterion
     def _filter_tarinfo(ti):
         # Reset the date to match the one of the last commit, not from the
         # filesystem since git doesn't track those at all
         # TODO: use the date of the last commit when any particular
         # file was changed -- would be the most kosher yoh thinks to the
```

### Comparing `datalad-0.9.2/datalad/plugin/wtf.py` & `datalad-0.9.3/datalad/plugin/wtf.py`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/datalad/plugin/__init__.py` & `datalad-0.9.3/datalad/plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/datalad/plugin/add_readme.py` & `datalad-0.9.3/datalad/plugin/add_readme.py`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/datalad/config.py` & `datalad-0.9.3/datalad/config.py`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/datalad/auto.py` & `datalad-0.9.3/datalad/auto.py`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/datalad/log.py` & `datalad-0.9.3/datalad/log.py`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/datalad/support/tests/test_cache.py` & `datalad-0.9.3/datalad/support/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/datalad/support/tests/test_network.py` & `datalad-0.9.3/datalad/support/tests/test_network.py`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/datalad/support/tests/test_annexrepo.py` & `datalad-0.9.3/datalad/support/tests/test_annexrepo.py`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/datalad/support/tests/test_vcr_.py` & `datalad-0.9.3/datalad/support/tests/test_vcr_.py`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/datalad/support/tests/test_gitrepo.py` & `datalad-0.9.3/datalad/support/tests/test_gitrepo.py`

 * *Files 0% similar despite different names*

```diff
@@ -1215,41 +1215,57 @@
     create_tree(gr.path, {'.gitattributes': "* tag\n* sec.key=val"})
     # ATM we do not do any translation of values, so if it is just a tag, it
     # would be what git returns -- "set"
     eq_(gr.get_git_attributes(), {'tag': 'set', 'sec.key': 'val'})
 
 
 @with_tempfile(mkdir=True)
-def test_check_git_configured(newhome):
-    try:
-        old = GitRepo._config_checked
-        GitRepo._config_checked = False
-        with patch.dict('os.environ', {'HOME': newhome}):
-            # clear clear home
-            assert_raises(RuntimeError, GitRepo, newhome, create=True)
-        # But then if we
-    finally:
-        GitRepo._config_checked = old
-
-
-@with_tempfile(mkdir=True)
 def test_get_tags(path):
     gr = GitRepo(path, create=True)
     eq_(gr.get_tags(), [])
 
-    create_tree(gr.path, {'file': ""})
-    gr.add('file')
-    gr.commit(msg="msg")
-    eq_(gr.get_tags(), [])
-
-    gr.tag("nonannotated")
-    tags1 = [{'name': 'nonannotated', 'hexsha': gr.get_hexsha()}]
-    eq_(gr.get_tags(), tags1)
-
-    sleep(1)  # so timestamp changes -- we sort in incremental order
-    create_tree(gr.path, {'file': "123"})
-    gr.add('file')
-    gr.commit(msg="changed")
+    # Explicitly override the committer date because tests may set it to a
+    # fixed value, but we want to check that the returned tags are sorted by
+    # the committer date.
+    with patch.dict("os.environ", {"GIT_COMMITTER_DATE":
+                                   "Thu, 07 Apr 2005 22:13:13 +0200"}):
+        create_tree(gr.path, {'file': ""})
+        gr.add('file')
+        gr.commit(msg="msg")
+        eq_(gr.get_tags(), [])
+
+        gr.tag("nonannotated")
+        tags1 = [{'name': 'nonannotated', 'hexsha': gr.get_hexsha()}]
+        eq_(gr.get_tags(), tags1)
+
+    with patch.dict("os.environ", {"GIT_COMMITTER_DATE":
+                                   "Fri, 08 Apr 2005 22:13:13 +0200"}):
+
+        create_tree(gr.path, {'file': "123"})
+        gr.add('file')
+        gr.commit(msg="changed")
 
     gr.tag("annotated", message="annotation")
     tags2 = tags1 + [{'name': 'annotated', 'hexsha': gr.get_hexsha()}]
-    eq_(gr.get_tags(), tags2)
+    eq_(gr.get_tags(), tags2)
+
+
+@with_tree(tree={'1': ""})
+def test_get_committed_date(path):
+    gr = GitRepo(path, create=True)
+    assert_equal(gr.get_commit_date(), None)
+
+    # Let's make a commit with a custom date
+    DATE = "Wed Mar 14 03:47:30 2018 -0000"
+    DATE_EPOCH = 1520999250
+    gr.add('1')
+    gr.commit("committed", date=DATE)
+    gr = GitRepo(path, create=True)
+    date = gr.get_commit_date()
+    neq_(date, None)
+    eq_(date, DATE_EPOCH)
+
+    eq_(date, gr.get_commit_date('master'))
+    # and even if we get into a detached head
+    gr.checkout(gr.get_hexsha())
+    eq_(gr.get_active_branch(), None)
+    eq_(date, gr.get_commit_date('master'))
```

### Comparing `datalad-0.9.2/datalad/support/tests/test_digests.py` & `datalad-0.9.3/datalad/support/tests/test_digests.py`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/datalad/support/tests/test_stats.py` & `datalad-0.9.3/datalad/support/tests/test_stats.py`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/datalad/support/tests/test_status.py` & `datalad-0.9.3/datalad/support/tests/test_status.py`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/datalad/support/tests/test_versions.py` & `datalad-0.9.3/datalad/support/tests/test_versions.py`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/datalad/support/tests/utils.py` & `datalad-0.9.3/datalad/support/tests/utils.py`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/datalad/support/tests/test_sshrun.py` & `datalad-0.9.3/datalad/support/tests/test_sshrun.py`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/datalad/support/tests/test_json_py.py` & `datalad-0.9.3/datalad/support/tests/test_json_py.py`

 * *Files 19% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 #   copyright and license terms.
 #
 # ## ### ### ### ### ### ### ### ### ### ### ### ### ### ### ### ### ### ### ##
 
 import logging
 
 from datalad.support.json_py import load
+from datalad.support.json_py import loads
 from datalad.support.json_py import JSONDecodeError
 
 from datalad.tests.utils import with_tempfile
 from datalad.tests.utils import eq_
 from datalad.tests.utils import assert_raises
 from datalad.tests.utils import assert_in
 from datalad.tests.utils import swallow_logs
@@ -23,7 +24,14 @@
 def test_load_screwy_unicode(fname):
     # test that we can tollerate some screwy unicode embeddings within json
     assert_raises(JSONDecodeError, load, fname, fixup=False)
     with swallow_logs(new_level=logging.WARNING) as cml:
         eq_(load(fname), {'Authors': ['A1', 'A2']})
         assert_in('Failed to decode content', cml.out)
 
+
+def test_loads():
+    eq_(loads('{"a": 2}'), {'a': 2})
+    with assert_raises(JSONDecodeError),\
+            swallow_logs(new_level=logging.WARNING) as cml:
+        loads('{"a": 2}x')
+    assert_in('Failed to load content from', cml.out)
```

### Comparing `datalad-0.9.2/datalad/support/tests/test_external_versions.py` & `datalad-0.9.3/datalad/support/tests/test_external_versions.py`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/datalad/support/tests/test_sshconnector.py` & `datalad-0.9.3/datalad/support/tests/test_sshconnector.py`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/datalad/support/versions.py` & `datalad-0.9.3/datalad/support/versions.py`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/datalad/support/keyring_.py` & `datalad-0.9.3/datalad/support/keyring_.py`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/datalad/support/param.py` & `datalad-0.9.3/datalad/support/param.py`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/datalad/support/sshrun.py` & `datalad-0.9.3/datalad/support/sshrun.py`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/datalad/support/external_versions.py` & `datalad-0.9.3/datalad/support/external_versions.py`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/datalad/support/annexrepo.py` & `datalad-0.9.3/datalad/support/annexrepo.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 from os.path import realpath
 from os.path import lexists
 from os.path import isdir
 from os.path import isabs
 from os.path import relpath
 from os.path import normpath
 from subprocess import Popen, PIPE
+from multiprocessing import cpu_count
 from weakref import WeakValueDictionary
 
 from six import string_types
 from six import iteritems
 from six.moves import filter
 from git import InvalidGitRepositoryError
 
@@ -50,14 +51,15 @@
 from datalad.utils import auto_repr
 from datalad.utils import on_windows
 from datalad.utils import swallow_logs
 from datalad.utils import assure_list
 from datalad.utils import _path_
 from datalad.utils import generate_chunks
 from datalad.utils import CMD_MAX_ARG
+from datalad.support.json_py import loads as json_loads
 from datalad.cmd import GitRunner
 
 # imports from same module:
 from .repo import RepoInterface
 from .gitrepo import GitRepo
 from .gitrepo import NoSuchPathError
 from .gitrepo import normalize_path
@@ -79,14 +81,17 @@
 from .exceptions import MissingExternalDependency
 from .exceptions import IncompleteResultsError
 from .exceptions import AccessDeniedError
 from .exceptions import AccessFailedError
 
 lgr = logging.getLogger('datalad.annex')
 
+# Limit to # of CPUs and up to 8, but at least 3 to start with
+N_AUTO_JOBS = min(8, max(3, cpu_count()))
+
 
 class AnnexRepo(GitRepo, RepoInterface):
     """Representation of an git-annex repository.
 
     Paths given to any of the class methods will be interpreted as relative
     to PWD, in case this is currently beneath AnnexRepo's base dir
     (`self.path`). If PWD is outside of the repository, relative paths
@@ -1257,16 +1262,17 @@
         ----------
         files : list of str
             paths to get
         remote : str, optional
             from which remote to fetch content
         options : list of str, optional
             commandline options for the git annex get command
-        jobs : int, optional
-            how many jobs to run in parallel (passed to git-annex call)
+        jobs : int or None, optional
+            how many jobs to run in parallel (passed to git-annex call).
+            If not specified (None), then
         key : bool, optional
             If provided file value is actually a key
 
         Returns
         -------
         files : list of dict
         """
@@ -2269,15 +2275,17 @@
                 kwargs.update(dict(
                     log_stdout=progress_indicators,
                     log_stderr='offline',  # False, # to avoid lock down
                     log_online=True
                 ))
             # TODO: refactor to account for possible --batch ones
             annex_options = ['--json']
-            if jobs:
+            if jobs == 'auto':
+                jobs = N_AUTO_JOBS
+            if jobs and jobs != 1:
                 annex_options += ['-J%d' % jobs]
             if opts:
                 annex_options += opts
 
             # TODO: RF to use --batch where possible instead of splitting
             # into multiple invocations
             if not files:
@@ -2384,15 +2392,15 @@
                     "Running %s resulted in stderr output: %s",
                     command, shorten(e.stderr)
                 )
         finally:
             if progress_indicators:
                 progress_indicators.finish()
 
-        json_objects = (json.loads(line)
+        json_objects = (json_loads(line)
                         for line in out.splitlines() if line.startswith('{'))
         # protect against progress leakage
         json_objects = [j for j in json_objects if 'byte-progress' not in j]
         return json_objects
 
     # TODO: reconsider having any magic at all and maybe just return a list/dict always
     @normalize_paths
@@ -3280,15 +3288,15 @@
         out += line
         if re.match(r'^.*\b(failed|ok)$', line.rstrip()):
             break
     return out.rstrip()
 
 
 def readline_json(stdout):
-    return json.loads(stdout.readline().strip())
+    return json_loads(stdout.readline().strip())
 
 
 @auto_repr
 class BatchedAnnex(object):
     """Container for an annex process which would allow for persistent communication
     """
 
@@ -3489,15 +3497,15 @@
             return line
 
         # Process some messages which remotes etc might push to us
         if list(j) == ['info']:
             # Just INFO was received without anything else -- we log it at INFO
             info = j['info']
             if info.startswith('PROGRESS-JSON: '):
-                j_ = json.loads(info[len('PROGRESS-JSON: '):])
+                j_ = json_loads(info[len('PROGRESS-JSON: '):])
                 if ('command' in j_ and 'key' in j_) or 'byte-progress' in j_:
                     j = j_
                 else:
                     self._log_info(info)
             else:
                 self._log_info(info)
                 return
```

### Comparing `datalad-0.9.2/datalad/support/constraints.py` & `datalad-0.9.3/datalad/support/constraints.py`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/datalad/support/gitrepo.py` & `datalad-0.9.3/datalad/support/gitrepo.py`

 * *Files 1% similar despite different names*

```diff
@@ -334,25 +334,28 @@
     Returns
     -------
     dict with user.name and user.email entries
     """
 
     check_runner = GitRunner()
     vals = {}
+    exc_ = ""
     for c in 'user.name', 'user.email':
         try:
             v, err = check_runner.run(['git', 'config', c])
             vals[c] = v.rstrip('\n')
         except CommandError as exc:
-            lgr.debug("Failed to verify that git is configured: %s",
-                      exc_str(exc))
-            raise RuntimeError(
-                "You must configure git first (set both user.name and "
-                "user.email) before using DataLad."
-            )
+            exc_ += exc_str(exc)
+    if exc_:
+        lgr.warning(
+            "It is highly recommended to configure git first (set both "
+            "user.name and user.email) before using DataLad. Failed to "
+            "verify that git is configured: %s.  Some operations might fail or "
+            "not perform correctly." % exc_
+        )
     return vals
 
 
 def _remove_empty_items(list_):
     """Remove empty entries from list
 
     This is needed, since some functions of GitPython may convert
@@ -995,15 +998,15 @@
 
     @staticmethod
     def _get_prefixed_commit_msg(msg):
         DATALAD_PREFIX = "[DATALAD]"
         return DATALAD_PREFIX if not msg else "%s %s" % (DATALAD_PREFIX, msg)
 
     def commit(self, msg=None, options=None, _datalad_msg=False, careless=True,
-               files=None):
+               files=None, date=None):
         """Commit changes to git.
 
         Parameters
         ----------
         msg: str, optional
           commit-message
         options: list of str, optional
@@ -1012,28 +1015,34 @@
           To signal that commit is automated commit by datalad, so
           it would carry the [DATALAD] prefix
         careless: bool, optional
           if False, raise when there's nothing actually committed;
           if True, don't care
         files: list of str, optional
           path(s) to commit
+        date: str, optional
+          Date in one of the formats git understands
         """
 
         self.precommit()
 
         if _datalad_msg:
             msg = self._get_prefixed_commit_msg(msg)
 
+        options = options or []
+
         if not msg:
             if options:
                 if "--allow-empty-message" not in options:
                         options.append("--allow-empty-message")
             else:
                 options = ["--allow-empty-message"]
 
+        if date:
+            options += ["--date", date]
         # Note: We used to use a direct call to git only if there were options,
         # since we can't pass all possible options to gitpython's implementation
         # of commit.
         # But there's an additional issue. GitPython implements commit in a way,
         # that it might create a new commit, when a direct call wouldn't. This
         # was discovered with a modified (but unstaged) submodule, leading to a
         # commit, that apparently did nothing - git status still showed the very
@@ -1152,26 +1161,38 @@
             raise
 
         if not bases:
             return None
         assert(len(bases) == 1)  # we do not do 'all' yet
         return bases[0].hexsha
 
-    def get_committed_date(self, branch=None):
-        """Get the date stamp of the last commit (in a branch). None if no commit"""
+    def get_commit_date(self, branch=None, date='authored'):
+        """Get the date stamp of the last commit (in a branch or head otherwise)
+
+        Parameters
+        ----------
+        date: {'authored', 'committed'}
+          Which date to return.  "authored" will be the date shown by "git show"
+          and the one possibly specified via --date to `git commit`
+
+        Returns
+        -------
+        int or None
+          None if no commit
+        """
         try:
-            commit = next(
-                self.get_branch_commits(branch
-                                        or self.get_active_branch())
-            )
+            if branch:
+                commit = next(self.get_branch_commits(branch))
+            else:
+                commit = self.repo.head.commit
         except Exception as exc:
             lgr.debug("Got exception while trying to get last commit: %s",
                       exc_str(exc))
             return None
-        return commit.committed_date
+        return getattr(commit, "%s_date" % date)
 
     def get_active_branch(self):
         try:
             branch = self.repo.active_branch.name
         except TypeError as e:
             if "HEAD is a detached symbolic reference" in str(e):
                 lgr.debug("detached HEAD in {0}".format(self))
```

### Comparing `datalad-0.9.2/datalad/support/status.py` & `datalad-0.9.3/datalad/support/status.py`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/datalad/support/third/noseclasses.py` & `datalad-0.9.3/datalad/support/third/noseclasses.py`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/datalad/support/third/nosetester.py` & `datalad-0.9.3/datalad/support/third/nosetester.py`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/datalad/support/third/nda_aws_token_generator.py` & `datalad-0.9.3/datalad/support/third/nda_aws_token_generator.py`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/datalad/support/protocol.py` & `datalad-0.9.3/datalad/support/protocol.py`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/datalad/support/nda_.py` & `datalad-0.9.3/datalad/support/nda_.py`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/datalad/support/cookies.py` & `datalad-0.9.3/datalad/support/cookies.py`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/datalad/support/sshconnector.py` & `datalad-0.9.3/datalad/support/sshconnector.py`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/datalad/support/strings.py` & `datalad-0.9.3/datalad/support/strings.py`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/datalad/support/exceptions.py` & `datalad-0.9.3/datalad/support/exceptions.py`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/datalad/support/network.py` & `datalad-0.9.3/datalad/support/network.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,14 +37,15 @@
 from six.moves.urllib.error import URLError
 
 from datalad.dochelpers import exc_str
 from datalad.utils import on_windows
 from datalad.utils import assure_dir
 from datalad import consts
 from datalad import cfg
+from datalad.support.cache import lru_cache
 
 # TODO not sure what needs to use `six` here yet
 # !!! Lazily import requests where needed -- needs 30ms or so
 # import requests
 
 
 def get_response_disposition_filename(s):
@@ -277,14 +278,15 @@
 #
 # Useful functionality in requests.models
 #  utils.requote_uri -- quote/unquote cycle to guarantee consistent appearance
 #  RequestEncodingMixin._encode_params -- Will successfully encode parameters when passed as a dict or a list of ...
 #  PreparedRequest().prepare_url(url, params) -- nicely cares about url encodings etc
 #
 
+@lru_cache(maxsize=100)
 def _guess_ri_cls(ri):
     """Factory function which would determine which type of a ri a provided string is"""
     TYPES = {
         'url': URL,
         'ssh':  SSHRI,
         'file': PathRI,
         'datalad': DataLadRI
```

### Comparing `datalad-0.9.2/datalad/support/repo.py` & `datalad-0.9.3/datalad/support/repo.py`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/datalad/support/vcr_.py` & `datalad-0.9.3/datalad/support/vcr_.py`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/datalad/support/json_py.py` & `datalad-0.9.3/datalad/support/json_py.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from io import open
 import codecs
 
 # wrapped below
 from simplejson import load as jsonload
 from simplejson import dump as jsondump
 # simply mirrored for now
-from simplejson import loads
+from simplejson import loads as json_loads
 from simplejson import JSONDecodeError
 
 
 # TODO think about minimizing the JSON output by default
 json_dump_kwargs = dict(indent=2, sort_keys=True, ensure_ascii=False, encoding='utf-8')
 
 # Let's just reuse top level one for now
@@ -33,14 +33,26 @@
     with open(fname, 'wb') as f:
         return jsondump(
             obj,
             codecs.getwriter('utf-8')(f),
             **json_dump_kwargs)
 
 
+def loads(s, *args, **kwargs):
+    """Helper to log actual value which failed to be parsed"""
+    try:
+        return json_loads(s, *args, **kwargs)
+    except:
+        lgr.error(
+            "Failed to load content from %r with args=%r kwargs=%r"
+            % (s, args, kwargs)
+        )
+        raise
+
+
 def load(fname, fixup=True, **kw):
     """Load JSON from a file, possibly fixing it up if initial load attempt fails
 
     Parameters
     ----------
     fixup : bool
       In case of failed load, apply a set of fixups with hope to resolve issues
```

### Comparing `datalad-0.9.2/datalad/support/s3.py` & `datalad-0.9.3/datalad/support/s3.py`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/datalad/support/configparserinc.py` & `datalad-0.9.3/datalad/support/configparserinc.py`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/datalad/support/ansi_colors.py` & `datalad-0.9.3/datalad/support/ansi_colors.py`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/datalad/support/digests.py` & `datalad-0.9.3/datalad/support/digests.py`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/datalad/support/archives.py` & `datalad-0.9.3/datalad/support/archives.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 from os.path import realpath
 from six import next
 from six.moves.urllib.parse import unquote as urlunquote
 
 import string
 import random
 
+from .locking import lock_if_check_fails
 from ..utils import any_re_search
 
 import logging
 lgr = logging.getLogger('datalad.files')
 
 # Monkey-patch patoolib's logging, so it logs coherently with the rest of
 # datalad
@@ -404,44 +405,52 @@
             and os.stat(self.stamp_path).st_mtime >= os.stat(self.path).st_mtime
 
     def assure_extracted(self):
         """Return path to the extracted `archive`.  Extract archive if necessary
         """
         path = self.path
 
-        if not self.is_extracted:
-            # we need to extract the archive
-            # TODO: extract to _tmp and then move in a single command so we
-            # don't end up picking up broken pieces
-            lgr.debug("Extracting {self._archive} under {path}".format(**locals()))
-            if exists(path):
-                lgr.debug("Previous extracted (but probably not fully) cached archive found. Removing %s", path)
-                rmtree(path)
-
-            os.makedirs(path)
-            assert(exists(path))
-            # remove old stamp
-            if exists(self.stamp_path):
-                rmtree(self.stamp_path)
-            decompress_file(self._archive, path, leading_directories=None)
-
-            # TODO: must optional since we might to use this content, move it into the tree etc
-            # lgr.debug("Adjusting permissions to R/O for the extracted content")
-            # rotree(path)
-            assert(exists(path))
-
-            # create a stamp
-            with open(self.stamp_path, 'w') as f:
-                f.write(self._archive)
-
-            # assert that stamp mtime is not older than archive's directory
-            assert(self.is_extracted)
-
+        with lock_if_check_fails(
+            check=(lambda s: s.is_extracted, (self,)),
+            lock_path=path,
+            operation="extract"
+        ) as (check, lock):
+            if lock:
+                assert not check
+                self._extract_archive(path)
         return path
 
+    def _extract_archive(self, path):
+        # we need to extract the archive
+        # TODO: extract to _tmp and then move in a single command so we
+        # don't end up picking up broken pieces
+        lgr.debug("Extracting {self._archive} under {path}".format(**locals()))
+        if exists(path):
+            lgr.debug(
+                "Previous extracted (but probably not fully) cached archive "
+                "found. Removing %s",
+                path)
+            rmtree(path)
+        os.makedirs(path)
+        assert (exists(path))
+        # remove old stamp
+        if exists(self.stamp_path):
+            rmtree(self.stamp_path)
+        decompress_file(self._archive, path, leading_directories=None)
+        # TODO: must optional since we might to use this content, move it
+        # into the tree etc
+        # lgr.debug("Adjusting permissions to R/O for the extracted content")
+        # rotree(path)
+        assert (exists(path))
+        # create a stamp
+        with open(self.stamp_path, 'w') as f:
+            f.write(self._archive)
+        # assert that stamp mtime is not older than archive's directory
+        assert (self.is_extracted)
+
     # TODO: remove?
     #def has_file_ready(self, afile):
     #    lgr.debug("Checking file {afile} from archive {archive}".format(**locals()))
     #    return exists(self.get_extracted_filename(afile))
 
     def get_extracted_filename(self, afile):
         """Return full path to the `afile` within extracted `archive`
```

### Comparing `datalad-0.9.2/datalad/support/stats.py` & `datalad-0.9.3/datalad/support/stats.py`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/datalad/support/cache.py` & `datalad-0.9.3/datalad/support/cache.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,14 +6,20 @@
 #   copyright and license terms.
 #
 # ## ### ### ### ### ### ### ### ### ### ### ### ### ### ### ### ### ### ### ##
 """Simple constructs to be used as caches
 """
 
 from collections import OrderedDict
+from six import PY2
+
+if PY2:
+    from ._lru_cache2 import lru_cache
+else:
+    from functools import lru_cache
 
 
 # based on http://stackoverflow.com/a/2437645/1265472
 class DictCache(OrderedDict):
     """A simple cache (dictionary) with limited size which expunges oldest entries
     """
     def __init__(self, *args, **kwds):
```

### Comparing `datalad-0.9.2/datalad/crawler/tests/test_pipeline.py` & `datalad-0.9.3/datalad/crawler/tests/test_pipeline.py`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/datalad/crawler/tests/__init__.py` & `datalad-0.9.3/datalad/crawler/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/datalad/crawler/pipeline.py` & `datalad-0.9.3/datalad/crawler/pipeline.py`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/datalad/crawler/dbs/base.py` & `datalad-0.9.3/datalad/crawler/dbs/base.py`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/datalad/crawler/dbs/tests/test_files.py` & `datalad-0.9.3/datalad/crawler/dbs/tests/test_files.py`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/datalad/crawler/dbs/versions.py` & `datalad-0.9.3/datalad/crawler/dbs/versions.py`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/datalad/crawler/dbs/files.py` & `datalad-0.9.3/datalad/crawler/dbs/files.py`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/datalad/crawler/oldconfig/base.py` & `datalad-0.9.3/datalad/crawler/oldconfig/base.py`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/datalad/crawler/oldconfig/tests/test_config.py` & `datalad-0.9.3/datalad/crawler/oldconfig/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/datalad/crawler/oldconfig/__init__.py` & `datalad-0.9.3/datalad/crawler/oldconfig/__init__.py`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/datalad/crawler/nodes/tests/test_annex.py` & `datalad-0.9.3/datalad/crawler/nodes/tests/test_annex.py`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/datalad/crawler/nodes/tests/test_matches.py` & `datalad-0.9.3/datalad/crawler/nodes/tests/test_matches.py`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/datalad/crawler/nodes/tests/test_s3.py` & `datalad-0.9.3/datalad/crawler/nodes/tests/test_s3.py`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/datalad/crawler/nodes/tests/test_misc.py` & `datalad-0.9.3/datalad/crawler/nodes/tests/test_misc.py`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/datalad/crawler/nodes/tests/test_crawl_url.py` & `datalad-0.9.3/datalad/crawler/nodes/tests/test_crawl_url.py`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/datalad/crawler/nodes/crawl_url.py` & `datalad-0.9.3/datalad/crawler/nodes/crawl_url.py`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/datalad/crawler/nodes/annex.py` & `datalad-0.9.3/datalad/crawler/nodes/annex.py`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/datalad/crawler/nodes/__init__.py` & `datalad-0.9.3/datalad/crawler/nodes/__init__.py`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/datalad/crawler/nodes/misc.py` & `datalad-0.9.3/datalad/crawler/nodes/misc.py`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/datalad/crawler/nodes/s3.py` & `datalad-0.9.3/datalad/crawler/nodes/s3.py`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/datalad/crawler/nodes/matches.py` & `datalad-0.9.3/datalad/crawler/nodes/matches.py`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/datalad/crawler/pipelines/tests/test_nda.py` & `datalad-0.9.3/datalad/crawler/pipelines/tests/test_nda.py`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/datalad/crawler/pipelines/tests/test_openfmri_collection.py` & `datalad-0.9.3/datalad/crawler/pipelines/tests/test_openfmri_collection.py`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/datalad/crawler/pipelines/tests/test_simple_s3.py` & `datalad-0.9.3/datalad/crawler/pipelines/tests/test_simple_s3.py`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/datalad/crawler/pipelines/tests/test_fcptable.py` & `datalad-0.9.3/datalad/crawler/pipelines/tests/test_fcptable.py`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/datalad/crawler/pipelines/tests/test_openfmri.py` & `datalad-0.9.3/datalad/crawler/pipelines/tests/test_openfmri.py`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/datalad/crawler/pipelines/tests/test_simple_with_archives.py` & `datalad-0.9.3/datalad/crawler/pipelines/tests/test_simple_with_archives.py`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/datalad/crawler/pipelines/tests/utils.py` & `datalad-0.9.3/datalad/crawler/pipelines/tests/utils.py`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/datalad/crawler/pipelines/tests/test_crcns.py` & `datalad-0.9.3/datalad/crawler/pipelines/tests/test_crcns.py`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/datalad/crawler/pipelines/tests/test_balsa.py` & `datalad-0.9.3/datalad/crawler/pipelines/tests/test_balsa.py`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/datalad/crawler/pipelines/crcns.py` & `datalad-0.9.3/datalad/crawler/pipelines/crcns.py`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/datalad/crawler/pipelines/openfmri.py` & `datalad-0.9.3/datalad/crawler/pipelines/openfmri.py`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/datalad/crawler/pipelines/template.py` & `datalad-0.9.3/datalad/crawler/pipelines/template.py`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/datalad/crawler/pipelines/balsa.py` & `datalad-0.9.3/datalad/crawler/pipelines/balsa.py`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/datalad/crawler/pipelines/simple_with_archives.py` & `datalad-0.9.3/datalad/crawler/pipelines/simple_with_archives.py`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/datalad/crawler/pipelines/openfmri_s3.py` & `datalad-0.9.3/datalad/crawler/pipelines/openfmri_s3.py`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/datalad/crawler/pipelines/abstractsonline.py` & `datalad-0.9.3/datalad/crawler/pipelines/abstractsonline.py`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/datalad/crawler/pipelines/simple_s3.py` & `datalad-0.9.3/datalad/crawler/pipelines/simple_s3.py`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/datalad/crawler/pipelines/nda.py` & `datalad-0.9.3/datalad/crawler/pipelines/nda.py`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/datalad/crawler/pipelines/fcptable.py` & `datalad-0.9.3/datalad/crawler/pipelines/fcptable.py`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/datalad/consts.py` & `datalad-0.9.3/datalad/consts.py`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/datalad/__init__.py` & `datalad-0.9.3/datalad/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,20 @@
 #   See COPYING file distributed along with the datalad package for the
 #   copyright and license terms.
 #
 # ## ### ### ### ### ### ### ### ### ### ### ### ### ### ### ### ### ### ### ##
 """DataLad aims to expose (scientific) data available online as a unified data
 distribution with the convenience of git-annex repositories as a backend."""
 
+# For reproducible demos/tests
+import os
+_seed = os.environ.get('DATALAD_SEED', None)
+if _seed:
+    import random
+    random.seed(_seed)
 
 # Other imports are interspersed with lgr.debug to ease troubleshooting startup
 # delays etc.
 
 # If there is a bundled git, make sure GitPython uses it too:
 from datalad.cmd import GitRunner
 GitRunner._check_git_path()
```

### Comparing `datalad-0.9.2/datalad/ui/base.py` & `datalad-0.9.3/datalad/ui/base.py`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/datalad/ui/tests/test_base.py` & `datalad-0.9.3/datalad/ui/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/datalad/ui/tests/test_dialog.py` & `datalad-0.9.3/datalad/ui/tests/test_dialog.py`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/datalad/ui/dialog.py` & `datalad-0.9.3/datalad/ui/dialog.py`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/datalad/ui/__init__.py` & `datalad-0.9.3/datalad/ui/__init__.py`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/datalad/ui/utils.py` & `datalad-0.9.3/datalad/ui/utils.py`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/datalad/ui/progressbars.py` & `datalad-0.9.3/datalad/ui/progressbars.py`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/datalad/downloaders/base.py` & `datalad-0.9.3/datalad/downloaders/base.py`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/datalad/downloaders/tests/test_credentials.py` & `datalad-0.9.3/datalad/downloaders/tests/test_credentials.py`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/datalad/downloaders/tests/test_s3.py` & `datalad-0.9.3/datalad/downloaders/tests/test_s3.py`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/datalad/downloaders/tests/utils.py` & `datalad-0.9.3/datalad/downloaders/tests/utils.py`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/datalad/downloaders/tests/test_providers.py` & `datalad-0.9.3/datalad/downloaders/tests/test_providers.py`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/datalad/downloaders/tests/test_http.py` & `datalad-0.9.3/datalad/downloaders/tests/test_http.py`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/datalad/downloaders/http.py` & `datalad-0.9.3/datalad/downloaders/http.py`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/datalad/downloaders/configs/nda.cfg` & `datalad-0.9.3/datalad/downloaders/configs/nda.cfg`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/datalad/downloaders/configs/nitrc.cfg` & `datalad-0.9.3/datalad/downloaders/configs/nitrc.cfg`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/datalad/downloaders/configs/crcns.cfg` & `datalad-0.9.3/datalad/downloaders/configs/crcns.cfg`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/datalad/downloaders/configs/kaggle.cfg` & `datalad-0.9.3/datalad/downloaders/configs/kaggle.cfg`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/datalad/downloaders/configs/hcp.cfg` & `datalad-0.9.3/datalad/downloaders/configs/hcp.cfg`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/datalad/downloaders/providers.py` & `datalad-0.9.3/datalad/downloaders/providers.py`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/datalad/downloaders/__init__.py` & `datalad-0.9.3/datalad/downloaders/__init__.py`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/datalad/downloaders/s3.py` & `datalad-0.9.3/datalad/downloaders/s3.py`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/datalad/downloaders/credentials.py` & `datalad-0.9.3/datalad/downloaders/credentials.py`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/datalad/api.py` & `datalad-0.9.3/datalad/api.py`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/datalad/metadata/tests/test_base.py` & `datalad-0.9.3/datalad/metadata/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/datalad/metadata/tests/test_manipulation.py` & `datalad-0.9.3/datalad/metadata/tests/test_manipulation.py`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/datalad/metadata/tests/test_search.py` & `datalad-0.9.3/datalad/metadata/tests/test_search.py`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/datalad/metadata/aggregate.py` & `datalad-0.9.3/datalad/metadata/aggregate.py`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/datalad/metadata/parsers/base.py` & `datalad-0.9.3/datalad/metadata/parsers/base.py`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/datalad/metadata/parsers/tests/test_datacite_xml.py` & `datalad-0.9.3/datalad/metadata/parsers/tests/test_datacite_xml.py`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/datalad/metadata/parsers/tests/test_frictionless_datapackage.py` & `datalad-0.9.3/datalad/metadata/parsers/tests/test_frictionless_datapackage.py`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/datalad/metadata/parsers/tests/test_rfc822.py` & `datalad-0.9.3/datalad/metadata/parsers/tests/test_rfc822.py`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/datalad/metadata/parsers/tests/test_aggregate.py` & `datalad-0.9.3/datalad/metadata/parsers/tests/test_aggregate.py`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/datalad/metadata/parsers/tests/test_bids.py` & `datalad-0.9.3/datalad/metadata/parsers/tests/test_bids.py`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/datalad/metadata/parsers/datalad_rfc822.py` & `datalad-0.9.3/datalad/metadata/parsers/datalad_rfc822.py`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/datalad/metadata/parsers/aggregate.py` & `datalad-0.9.3/datalad/metadata/parsers/aggregate.py`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/datalad/metadata/parsers/frictionless_datapackage.py` & `datalad-0.9.3/datalad/metadata/parsers/frictionless_datapackage.py`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/datalad/metadata/parsers/__init__.py` & `datalad-0.9.3/datalad/metadata/parsers/__init__.py`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/datalad/metadata/parsers/datacite.py` & `datalad-0.9.3/datalad/metadata/parsers/datacite.py`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/datalad/metadata/parsers/bids.py` & `datalad-0.9.3/datalad/metadata/parsers/bids.py`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/datalad/metadata/__init__.py` & `datalad-0.9.3/datalad/metadata/__init__.py`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/datalad/metadata/metadata.py` & `datalad-0.9.3/datalad/metadata/metadata.py`

 * *Files 1% similar despite different names*

```diff
@@ -316,16 +316,15 @@
                 if GitRepo.is_valid_repo(ap['path']):
                     ap['process_content'] = True
             to_process.append(ap)
 
         content_by_ds, ds_props, completed, nondataset_paths = \
             annotated2content_by_ds(
                 to_process,
-                refds_path=refds_path,
-                path_only=False)
+                refds_path=refds_path)
         assert(not completed)
 
         # iterate over all datasets, order doesn't matter
         to_save = []
         for ds_path in content_by_ds:
             # ignore submodule entries
             content = [ap for ap in content_by_ds[ds_path]
```

### Comparing `datalad-0.9.2/datalad/metadata/search.py` & `datalad-0.9.3/datalad/metadata/search.py`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/datalad/utils.py` & `datalad-0.9.3/datalad/utils.py`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/datalad/distribution/tests/test_create_sibling.py` & `datalad-0.9.3/datalad/distribution/tests/test_create_sibling.py`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/datalad/distribution/tests/test_update.py` & `datalad-0.9.3/datalad/distribution/tests/test_update.py`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/datalad/distribution/tests/test_create_github.py` & `datalad-0.9.3/datalad/distribution/tests/test_create_github.py`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/datalad/distribution/tests/test_create_test_dataset.py` & `datalad-0.9.3/datalad/distribution/tests/test_create_test_dataset.py`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/datalad/distribution/tests/test_utils.py` & `datalad-0.9.3/datalad/distribution/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/datalad/distribution/tests/test_dataset_binding.py` & `datalad-0.9.3/datalad/distribution/tests/test_dataset_binding.py`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/datalad/distribution/tests/test_subdataset.py` & `datalad-0.9.3/datalad/distribution/tests/test_subdataset.py`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/datalad/distribution/tests/test_publish.py` & `datalad-0.9.3/datalad/distribution/tests/test_publish.py`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/datalad/distribution/tests/test_dataset.py` & `datalad-0.9.3/datalad/distribution/tests/test_dataset.py`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/datalad/distribution/tests/test_install.py` & `datalad-0.9.3/datalad/distribution/tests/test_install.py`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/datalad/distribution/tests/test_get.py` & `datalad-0.9.3/datalad/distribution/tests/test_get.py`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/datalad/distribution/tests/test_siblings.py` & `datalad-0.9.3/datalad/distribution/tests/test_siblings.py`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/datalad/distribution/tests/test_uninstall.py` & `datalad-0.9.3/datalad/distribution/tests/test_uninstall.py`

 * *Files 3% similar despite different names*

```diff
@@ -31,14 +31,15 @@
 from datalad.tests.utils import eq_
 from datalad.tests.utils import with_testrepos
 from datalad.tests.utils import SkipTest
 from datalad.tests.utils import assert_raises
 from datalad.tests.utils import assert_status
 from datalad.tests.utils import assert_in
 from datalad.tests.utils import assert_result_count
+from datalad.tests.utils import assert_result_values_cond
 from datalad.tests.utils import ok_file_under_git
 from datalad.tests.utils import ok_clean_git
 from datalad.tests.utils import with_tempfile
 from datalad.tests.utils import with_tree
 from datalad.tests.utils import create_tree
 from datalad.tests.utils import skip_if_no_network
 from datalad.tests.utils import use_cassette
@@ -322,16 +323,20 @@
     # now uninstall in subdataset through superdataset
     target_fname = opj('deep', 'dir', 'test')
     # sane starting point
     ok_(exists(opj(ds.path, target_fname)))
     # doesn't have the minimum number of copies for a safe drop
     res = ds.drop(target_fname, recursive=True, on_failure='ignore')
     assert_status('error', res)
-    assert_result_count(res, 1,
-                        message='configured minimum number of copies not found')
+    assert_result_values_cond(
+        res, 'message',
+        lambda x: "configured minimum number of copies not found" in x or
+        "Could only verify the existence of 0 out of 1 necessary copies" in x
+    )
+
     # this should do it
     ds.drop(target_fname, check=False, recursive=True)
     # link is dead
     lname = opj(ds.path, target_fname)
     ok_(not exists(lname))
     # entire hierarchy saved
     ok_clean_git(subds.path)
@@ -398,16 +403,24 @@
     eq_(sorted(ds.subdatasets(result_xfm='relpaths')), ['deep1'])
     ok_clean_git(ds.path)
 
     # and we fail to remove since content can't be dropped
     res = ds.remove(on_failure='ignore')
     assert_result_count(
         res, 1,
-        status='error', path=testfile,
-        message='configured minimum number of copies not found')
+        status='error', path=testfile)
+    # Following two assertions on message are relying on the actual error.
+    # We have a second result with status 'impossible' for the ds, that we need
+    # to filter out for those assertions:
+    err_result = [r for r in res if r['status'] == 'error'][0]
+    assert_result_values_cond(
+        [err_result], 'message',
+        lambda x: "configured minimum number of copies not found" in x or
+        "Could only verify the existence of 0 out of 1 necessary copies" in x
+    )
     eq_(ds.remove(recursive=True, check=False, result_xfm='datasets'),
         [subds, ds])
     ok_(not exists(path))
 
 
 @with_tempfile()
 def test_remove_recreation(path):
```

### Comparing `datalad-0.9.2/datalad/distribution/tests/test_create.py` & `datalad-0.9.3/datalad/distribution/tests/test_create.py`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/datalad/distribution/tests/test_dataset_config.py` & `datalad-0.9.3/datalad/distribution/tests/test_dataset_config.py`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/datalad/distribution/tests/test_clone.py` & `datalad-0.9.3/datalad/distribution/tests/test_clone.py`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/datalad/distribution/tests/test_add.py` & `datalad-0.9.3/datalad/distribution/tests/test_add.py`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/datalad/distribution/publish.py` & `datalad-0.9.3/datalad/distribution/publish.py`

 * *Files 1% similar despite different names*

```diff
@@ -756,16 +756,15 @@
                 yield ap
                 continue
             to_process.append(ap)
 
         content_by_ds, ds_props, completed, nondataset_paths = \
             annotated2content_by_ds(
                 to_process,
-                refds_path=refds_path,
-                path_only=False)
+                refds_path=refds_path)
         assert(not completed)
 
         lgr.debug(
             "Evaluating %i dataset publication candidate(s)",
             len(content_by_ds))
         # TODO: fancier sorting, so we still follow somewhat the hierarchy
         #       in sorted order, e.g.
```

### Comparing `datalad-0.9.2/datalad/distribution/create_sibling.py` & `datalad-0.9.3/datalad/distribution/create_sibling.py`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/datalad/distribution/subdatasets.py` & `datalad-0.9.3/datalad/distribution/subdatasets.py`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/datalad/distribution/siblings.py` & `datalad-0.9.3/datalad/distribution/siblings.py`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/datalad/distribution/remove.py` & `datalad-0.9.3/datalad/distribution/remove.py`

 * *Files 1% similar despite different names*

```diff
@@ -156,16 +156,15 @@
             raise ValueError(
                 "refusing to uninstall current or parent directory")
 
         # now sort into datasets so we can process them one by one
         content_by_ds, ds_props, completed, nondataset_paths = \
             annotated2content_by_ds(
                 to_process,
-                refds_path=refds_path,
-                path_only=False)
+                refds_path=refds_path)
         assert(not completed)
 
         # iterate over all datasets, starting at the bottom
         # to make the removal of dataset content known upstairs
         to_save = []
         # track which submodules we have removed in the process, to avoid
         # failure in case we revisit them due to a subsequent path argument
```

### Comparing `datalad-0.9.2/datalad/distribution/add_sibling.py` & `datalad-0.9.3/datalad/distribution/add_sibling.py`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/datalad/distribution/create_test_dataset.py` & `datalad-0.9.3/datalad/distribution/create_test_dataset.py`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/datalad/distribution/create_sibling_github.py` & `datalad-0.9.3/datalad/distribution/create_sibling_github.py`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/datalad/distribution/install.py` & `datalad-0.9.3/datalad/distribution/install.py`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/datalad/distribution/drop.py` & `datalad-0.9.3/datalad/distribution/drop.py`

 * *Files 2% similar despite different names*

```diff
@@ -201,16 +201,15 @@
                 # and skip silently
                 continue
             to_drop.append(ap)
 
         content_by_ds, ds_props, completed, nondataset_paths = \
             annotated2content_by_ds(
                 to_drop,
-                refds_path=refds_path,
-                path_only=False)
+                refds_path=refds_path)
         assert(not completed)
 
         # iterate over all datasets, order doesn't matter
         for ds_path in content_by_ds:
             ds = Dataset(ds_path)
             # TODO generator
             # this should yield what it did
```

### Comparing `datalad-0.9.2/datalad/distribution/uninstall.py` & `datalad-0.9.3/datalad/distribution/uninstall.py`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/datalad/distribution/dataset.py` & `datalad-0.9.3/datalad/distribution/dataset.py`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/datalad/distribution/get.py` & `datalad-0.9.3/datalad/distribution/get.py`

 * *Files 1% similar despite different names*

```diff
@@ -589,16 +589,15 @@
         # merge the two AP lists
         to_get.extend(rec_get)
 
         # sort into datasets
         content_by_ds, ds_props, completed, nondataset_paths = \
             annotated2content_by_ds(
                 to_get,
-                refds_path=refds_path,
-                path_only=False)
+                refds_path=refds_path)
         assert(not completed)
 
         # hand over to git-annex, get files content,
         # report files in git as 'notneeded' to get
         for ds_path in sorted(content_by_ds.keys()):
             ds = Dataset(ds_path)
             # grab content, ignore subdataset entries
```

### Comparing `datalad-0.9.2/datalad/distribution/clone.py` & `datalad-0.9.3/datalad/distribution/clone.py`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/datalad/distribution/update.py` & `datalad-0.9.3/datalad/distribution/update.py`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/datalad/distribution/add.py` & `datalad-0.9.3/datalad/distribution/add.py`

 * *Files 0% similar despite different names*

```diff
@@ -319,16 +319,15 @@
             return_type='generator',
             # if there is an error now, we made this mistake in here
             on_failure='stop')
 
         content_by_ds, ds_props, completed, nondataset_paths = \
             annotated2content_by_ds(
                 annotated_paths,
-                refds_path=refds_path,
-                path_only=False)
+                refds_path=refds_path)
         assert(not completed)
 
         if not content_by_ds:
             # we should have complained about any inappropriate path argument
             # above, so if nothing is left, we can simply exit
             return
```

### Comparing `datalad-0.9.2/datalad/distribution/utils.py` & `datalad-0.9.3/datalad/distribution/utils.py`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/datalad/distribution/create.py` & `datalad-0.9.3/datalad/distribution/create.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,21 +7,23 @@
 #
 # ## ### ### ### ### ### ### ### ### ### ### ### ### ### ### ### ### ### ### ##
 """High-level interface for dataset creation
 
 """
 
 import logging
+import random
 import uuid
 
 from os import listdir
 from os.path import isdir
 from os.path import relpath
 from os.path import join as opj
 
+from datalad import _seed
 from datalad.interface.base import Interface
 from datalad.interface.annotate_paths import AnnotatePaths
 from datalad.interface.utils import eval_results
 from datalad.interface.base import build_doc
 from datalad.interface.common_opts import git_opts
 from datalad.interface.common_opts import annex_opts
 from datalad.interface.common_opts import annex_init_opts
@@ -344,17 +346,24 @@
 
         # record an ID for this repo for the afterlife
         # to be able to track siblings and children
         id_var = 'datalad.dataset.id'
         if id_var in tbds.config:
             # make sure we reset this variable completely, in case of a re-create
             tbds.config.unset(id_var, where='dataset')
+
+        if _seed is None:
+            # just the standard way
+            uuid_id = uuid.uuid1().urn.split(':')[-1]
+        else:
+            # Let's generate preseeded ones
+            uuid_id = str(uuid.UUID(int=random.getrandbits(128)))
         tbds.config.add(
             id_var,
-            tbds.id if tbds.id is not None else uuid.uuid1().urn.split(':')[-1],
+            tbds.id if tbds.id is not None else uuid_id,
             where='dataset')
 
         # make sure that v6 annex repos never commit content under .datalad
         with open(opj(tbds.path, '.datalad', '.gitattributes'), 'a') as gitattr:
             # TODO this will need adjusting, when annex'ed aggregate meta data
             # comes around
             gitattr.write('# Text files (according to file --mime-type) are added directly to git.\n')
```

### Comparing `datalad-0.9.2/datalad/cmdline/tests/test_helpers.py` & `datalad-0.9.3/datalad/cmdline/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/datalad/cmdline/tests/test_formatters.py` & `datalad-0.9.3/datalad/cmdline/tests/test_formatters.py`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/datalad/cmdline/tests/test_main.py` & `datalad-0.9.3/datalad/cmdline/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/datalad/cmdline/helpers.py` & `datalad-0.9.3/datalad/cmdline/helpers.py`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/datalad/cmdline/common_args.py` & `datalad-0.9.3/datalad/cmdline/common_args.py`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/datalad/cmdline/main.py` & `datalad-0.9.3/datalad/cmdline/main.py`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/datalad/version.py` & `datalad-0.9.3/datalad/version.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 """Defines version to be imported in the module and obtained from setup.py
 """
 
 import sys
 from os.path import lexists, dirname, join as opj, curdir
 
 # Hard coded version, to be done by release process
-__version__ = '0.9.2'
+__version__ = '0.9.3'
 
 # NOTE: might cause problems with "python setup.py develop" deployments
 #  so I have even changed buildbot to use  pip install -e .
 moddir = dirname(__file__)
 projdir = curdir if moddir == 'datalad' else dirname(moddir)
 if lexists(opj(projdir, '.git')):
     # If under git -- attempt to deduce a better "dynamic" version following git
```

### Comparing `datalad-0.9.2/datalad/dochelpers.py` & `datalad-0.9.3/datalad/dochelpers.py`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/datalad/cmd.py` & `datalad-0.9.3/datalad/cmd.py`

 * *Files identical despite different names*

### Comparing `datalad-0.9.2/setup.py` & `datalad-0.9.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,14 +52,15 @@
 
 requires = {
     'core': [
         'appdirs',
         'GitPython>=2.1.8',
         'iso8601',
         'humanize',
+        'fasteners',
         'mock>=1.0.1',  # mock is also used for auto.py, not only for testing
         'patool>=1.7',
         'six>=1.8.0',
         'wrapt',
     ] + pbar_requires,
     'downloaders': [
         'boto',
```

