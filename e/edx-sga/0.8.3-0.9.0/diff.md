# Comparing `tmp/edx-sga-0.8.3.tar.gz` & `tmp/edx-sga-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/edx-sga-0.8.3.tar", last modified: Wed Aug 22 19:07:34 2018, max compression
+gzip compressed data, was "dist/edx-sga-0.9.0.tar", last modified: Tue Oct  1 15:39:33 2019, max compression
```

## Comparing `edx-sga-0.8.3.tar` & `edx-sga-0.9.0.tar`

### file list

```diff
@@ -1,287 +1,287 @@
-drwx------   0 u45925   (45925) dyno     (45925)        0 2018-08-22 19:07:34.000000 edx-sga-0.8.3/
-drwx------   0 u45925   (45925) dyno     (45925)        0 2018-08-22 19:07:34.000000 edx-sga-0.8.3/edx_sga/
--rw-------   0 u45925   (45925) dyno     (45925)      365 2018-08-22 19:07:10.000000 edx-sga-0.8.3/edx_sga/constants.py
--rw-------   0 u45925   (45925) dyno     (45925)     2203 2018-08-22 19:07:10.000000 edx-sga-0.8.3/edx_sga/utils.py
-drwx------   0 u45925   (45925) dyno     (45925)        0 2018-08-22 19:07:34.000000 edx-sga-0.8.3/edx_sga/locale/
-drwx------   0 u45925   (45925) dyno     (45925)        0 2018-08-22 19:07:34.000000 edx-sga-0.8.3/edx_sga/locale/fake2/
-drwx------   0 u45925   (45925) dyno     (45925)        0 2018-08-22 19:07:34.000000 edx-sga-0.8.3/edx_sga/locale/fake2/LC_MESSAGES/
--rw-------   0 u45925   (45925) dyno     (45925)     7578 2018-08-22 19:07:10.000000 edx-sga-0.8.3/edx_sga/locale/fake2/LC_MESSAGES/django.po
--rw-------   0 u45925   (45925) dyno     (45925)     1842 2018-08-22 19:07:10.000000 edx-sga-0.8.3/edx_sga/locale/fake2/LC_MESSAGES/djangojs.po
--rw-------   0 u45925   (45925) dyno     (45925)     5090 2018-08-22 19:07:10.000000 edx-sga-0.8.3/edx_sga/locale/fake2/LC_MESSAGES/django.mo
--rw-------   0 u45925   (45925) dyno     (45925)     1321 2018-08-22 19:07:10.000000 edx-sga-0.8.3/edx_sga/locale/fake2/LC_MESSAGES/djangojs.mo
--rw-------   0 u45925   (45925) dyno     (45925)      588 2018-08-22 19:07:10.000000 edx-sga-0.8.3/edx_sga/locale/config.yaml
-drwx------   0 u45925   (45925) dyno     (45925)        0 2018-08-22 19:07:34.000000 edx-sga-0.8.3/edx_sga/locale/rtl/
-drwx------   0 u45925   (45925) dyno     (45925)        0 2018-08-22 19:07:34.000000 edx-sga-0.8.3/edx_sga/locale/rtl/LC_MESSAGES/
--rw-------   0 u45925   (45925) dyno     (45925)     7848 2018-08-22 19:07:10.000000 edx-sga-0.8.3/edx_sga/locale/rtl/LC_MESSAGES/django.po
--rw-------   0 u45925   (45925) dyno     (45925)     1885 2018-08-22 19:07:10.000000 edx-sga-0.8.3/edx_sga/locale/rtl/LC_MESSAGES/djangojs.po
--rw-------   0 u45925   (45925) dyno     (45925)     5360 2018-08-22 19:07:10.000000 edx-sga-0.8.3/edx_sga/locale/rtl/LC_MESSAGES/django.mo
--rw-------   0 u45925   (45925) dyno     (45925)     1364 2018-08-22 19:07:10.000000 edx-sga-0.8.3/edx_sga/locale/rtl/LC_MESSAGES/djangojs.mo
-drwx------   0 u45925   (45925) dyno     (45925)        0 2018-08-22 19:07:34.000000 edx-sga-0.8.3/edx_sga/locale/eo/
-drwx------   0 u45925   (45925) dyno     (45925)        0 2018-08-22 19:07:34.000000 edx-sga-0.8.3/edx_sga/locale/eo/LC_MESSAGES/
--rw-------   0 u45925   (45925) dyno     (45925)     9860 2018-08-22 19:07:10.000000 edx-sga-0.8.3/edx_sga/locale/eo/LC_MESSAGES/django.po
--rw-------   0 u45925   (45925) dyno     (45925)     2379 2018-08-22 19:07:10.000000 edx-sga-0.8.3/edx_sga/locale/eo/LC_MESSAGES/djangojs.po
--rw-------   0 u45925   (45925) dyno     (45925)     7312 2018-08-22 19:07:10.000000 edx-sga-0.8.3/edx_sga/locale/eo/LC_MESSAGES/django.mo
--rw-------   0 u45925   (45925) dyno     (45925)     1846 2018-08-22 19:07:10.000000 edx-sga-0.8.3/edx_sga/locale/eo/LC_MESSAGES/djangojs.mo
-drwx------   0 u45925   (45925) dyno     (45925)        0 2018-08-22 19:07:34.000000 edx-sga-0.8.3/edx_sga/locale/en/
-drwx------   0 u45925   (45925) dyno     (45925)        0 2018-08-22 19:07:34.000000 edx-sga-0.8.3/edx_sga/locale/en/LC_MESSAGES/
--rw-------   0 u45925   (45925) dyno     (45925)     5404 2018-08-22 19:07:10.000000 edx-sga-0.8.3/edx_sga/locale/en/LC_MESSAGES/django.po
--rw-------   0 u45925   (45925) dyno     (45925)     1395 2018-08-22 19:07:10.000000 edx-sga-0.8.3/edx_sga/locale/en/LC_MESSAGES/djangojs.po
--rw-------   0 u45925   (45925) dyno     (45925)      378 2018-08-22 19:07:10.000000 edx-sga-0.8.3/edx_sga/locale/en/LC_MESSAGES/django.mo
--rw-------   0 u45925   (45925) dyno     (45925)      378 2018-08-22 19:07:10.000000 edx-sga-0.8.3/edx_sga/locale/en/LC_MESSAGES/djangojs.mo
--rw-------   0 u45925   (45925) dyno     (45925)    37342 2018-08-22 19:07:10.000000 edx-sga-0.8.3/edx_sga/sga.py
-drwx------   0 u45925   (45925) dyno     (45925)        0 2018-08-22 19:07:34.000000 edx-sga-0.8.3/edx_sga/management/
-drwx------   0 u45925   (45925) dyno     (45925)        0 2018-08-22 19:07:34.000000 edx-sga-0.8.3/edx_sga/management/commands/
--rw-------   0 u45925   (45925) dyno     (45925)     2783 2018-08-22 19:07:10.000000 edx-sga-0.8.3/edx_sga/management/commands/sga_migrate_submissions.py
--rw-------   0 u45925   (45925) dyno     (45925)       36 2018-08-22 19:07:10.000000 edx-sga-0.8.3/edx_sga/management/commands/__init__.py
--rw-------   0 u45925   (45925) dyno     (45925)       36 2018-08-22 19:07:10.000000 edx-sga-0.8.3/edx_sga/management/__init__.py
-drwx------   0 u45925   (45925) dyno     (45925)        0 2018-08-22 19:07:34.000000 edx-sga-0.8.3/edx_sga/static/
-drwx------   0 u45925   (45925) dyno     (45925)        0 2018-08-22 19:07:34.000000 edx-sga-0.8.3/edx_sga/static/css/
--rw-------   0 u45925   (45925) dyno     (45925)     2696 2018-08-22 19:07:10.000000 edx-sga-0.8.3/edx_sga/static/css/edx_sga.css
-drwx------   0 u45925   (45925) dyno     (45925)        0 2018-08-22 19:07:34.000000 edx-sga-0.8.3/edx_sga/static/js/
-drwx------   0 u45925   (45925) dyno     (45925)        0 2018-08-22 19:07:34.000000 edx-sga-0.8.3/edx_sga/static/js/src/
--rw-------   0 u45925   (45925) dyno     (45925)      829 2018-08-22 19:07:10.000000 edx-sga-0.8.3/edx_sga/static/js/src/studio.js
--rw-------   0 u45925   (45925) dyno     (45925)    18702 2018-08-22 19:07:10.000000 edx-sga-0.8.3/edx_sga/static/js/src/edx_sga.js
--rw-------   0 u45925   (45925) dyno     (45925)    16520 2018-08-22 19:07:10.000000 edx-sga-0.8.3/edx_sga/static/js/src/jquery.tablesorter.min.js
-drwx------   0 u45925   (45925) dyno     (45925)        0 2018-08-22 19:07:34.000000 edx-sga-0.8.3/edx_sga/static/js/bower/
-drwx------   0 u45925   (45925) dyno     (45925)        0 2018-08-22 19:07:34.000000 edx-sga-0.8.3/edx_sga/static/js/bower/underscore/
--rw-------   0 u45925   (45925) dyno     (45925)     1225 2018-08-22 19:07:10.000000 edx-sga-0.8.3/edx_sga/static/js/bower/underscore/README.md
--rw-------   0 u45925   (45925) dyno     (45925)    52919 2018-08-22 19:07:10.000000 edx-sga-0.8.3/edx_sga/static/js/bower/underscore/underscore.js
--rw-------   0 u45925   (45925) dyno     (45925)      702 2018-08-22 19:07:10.000000 edx-sga-0.8.3/edx_sga/static/js/bower/underscore/.bower.json
--rw-------   0 u45925   (45925) dyno     (45925)    27589 2018-08-22 19:07:10.000000 edx-sga-0.8.3/edx_sga/static/js/bower/underscore/underscore-min.map
--rw-------   0 u45925   (45925) dyno     (45925)    16449 2018-08-22 19:07:10.000000 edx-sga-0.8.3/edx_sga/static/js/bower/underscore/underscore-min.js
--rw-------   0 u45925   (45925) dyno     (45925)     1117 2018-08-22 19:07:10.000000 edx-sga-0.8.3/edx_sga/static/js/bower/underscore/LICENSE
--rw-------   0 u45925   (45925) dyno     (45925)      293 2018-08-22 19:07:10.000000 edx-sga-0.8.3/edx_sga/static/js/bower/underscore/bower.json
-drwx------   0 u45925   (45925) dyno     (45925)        0 2018-08-22 19:07:34.000000 edx-sga-0.8.3/edx_sga/static/js/bower/sinon/
--rw-------   0 u45925   (45925) dyno     (45925)       15 2018-08-22 19:07:10.000000 edx-sga-0.8.3/edx_sga/static/js/bower/sinon/.eslintignore
-drwx------   0 u45925   (45925) dyno     (45925)        0 2018-08-22 19:07:34.000000 edx-sga-0.8.3/edx_sga/static/js/bower/sinon/lib/
-drwx------   0 u45925   (45925) dyno     (45925)        0 2018-08-22 19:07:34.000000 edx-sga-0.8.3/edx_sga/static/js/bower/sinon/lib/sinon/
--rw-------   0 u45925   (45925) dyno     (45925)     6121 2018-08-22 19:07:10.000000 edx-sga-0.8.3/edx_sga/static/js/bower/sinon/lib/sinon/stub.js
--rw-------   0 u45925   (45925) dyno     (45925)     3209 2018-08-22 19:07:10.000000 edx-sga-0.8.3/edx_sga/static/js/bower/sinon/lib/sinon/test.js
--rw-------   0 u45925   (45925) dyno     (45925)     2804 2018-08-22 19:07:10.000000 edx-sga-0.8.3/edx_sga/static/js/bower/sinon/lib/sinon/test_case.js
--rw-------   0 u45925   (45925) dyno     (45925)     1900 2018-08-22 19:07:10.000000 edx-sga-0.8.3/edx_sga/static/js/bower/sinon/lib/sinon/log_error.js
--rw-------   0 u45925   (45925) dyno     (45925)     8682 2018-08-22 19:07:10.000000 edx-sga-0.8.3/edx_sga/static/js/bower/sinon/lib/sinon/match.js
--rw-------   0 u45925   (45925) dyno     (45925)     2549 2018-08-22 19:07:10.000000 edx-sga-0.8.3/edx_sga/static/js/bower/sinon/lib/sinon/format.js
--rw-------   0 u45925   (45925) dyno     (45925)     5078 2018-08-22 19:07:10.000000 edx-sga-0.8.3/edx_sga/static/js/bower/sinon/lib/sinon/sandbox.js
--rw-------   0 u45925   (45925) dyno     (45925)     1196 2018-08-22 19:07:10.000000 edx-sga-0.8.3/edx_sga/static/js/bower/sinon/lib/sinon/times_in_words.js
--rw-------   0 u45925   (45925) dyno     (45925)     8430 2018-08-22 19:07:10.000000 edx-sga-0.8.3/edx_sga/static/js/bower/sinon/lib/sinon/assert.js
--rw-------   0 u45925   (45925) dyno     (45925)    15868 2018-08-22 19:07:10.000000 edx-sga-0.8.3/edx_sga/static/js/bower/sinon/lib/sinon/spy.js
--rw-------   0 u45925   (45925) dyno     (45925)     4656 2018-08-22 19:07:10.000000 edx-sga-0.8.3/edx_sga/static/js/bower/sinon/lib/sinon/collection.js
-drwx------   0 u45925   (45925) dyno     (45925)        0 2018-08-22 19:07:34.000000 edx-sga-0.8.3/edx_sga/static/js/bower/sinon/lib/sinon/util/
--rw-------   0 u45925   (45925) dyno     (45925)    22473 2018-08-22 19:07:10.000000 edx-sga-0.8.3/edx_sga/static/js/bower/sinon/lib/sinon/util/fake_xml_http_request.js
--rw-------   0 u45925   (45925) dyno     (45925)    13439 2018-08-22 19:07:10.000000 edx-sga-0.8.3/edx_sga/static/js/bower/sinon/lib/sinon/util/core.js
--rw-------   0 u45925   (45925) dyno     (45925)     3345 2018-08-22 19:07:10.000000 edx-sga-0.8.3/edx_sga/static/js/bower/sinon/lib/sinon/util/fake_server_with_clock.js
--rw-------   0 u45925   (45925) dyno     (45925)     1989 2018-08-22 19:07:10.000000 edx-sga-0.8.3/edx_sga/static/js/bower/sinon/lib/sinon/util/fake_timers.js
--rw-------   0 u45925   (45925) dyno     (45925)     7569 2018-08-22 19:07:10.000000 edx-sga-0.8.3/edx_sga/static/js/bower/sinon/lib/sinon/util/fake_xdomain_request.js
--rw-------   0 u45925   (45925) dyno     (45925)     8238 2018-08-22 19:07:10.000000 edx-sga-0.8.3/edx_sga/static/js/bower/sinon/lib/sinon/util/fake_server.js
--rw-------   0 u45925   (45925) dyno     (45925)      714 2018-08-22 19:07:10.000000 edx-sga-0.8.3/edx_sga/static/js/bower/sinon/lib/sinon/util/xdr_ie.js
--rw-------   0 u45925   (45925) dyno     (45925)     3690 2018-08-22 19:07:10.000000 edx-sga-0.8.3/edx_sga/static/js/bower/sinon/lib/sinon/util/event.js
--rw-------   0 u45925   (45925) dyno     (45925)      837 2018-08-22 19:07:10.000000 edx-sga-0.8.3/edx_sga/static/js/bower/sinon/lib/sinon/util/xhr_ie.js
--rw-------   0 u45925   (45925) dyno     (45925)     1292 2018-08-22 19:07:10.000000 edx-sga-0.8.3/edx_sga/static/js/bower/sinon/lib/sinon/util/timers_ie.js
--rw-------   0 u45925   (45925) dyno     (45925)     7729 2018-08-22 19:07:10.000000 edx-sga-0.8.3/edx_sga/static/js/bower/sinon/lib/sinon/call.js
--rw-------   0 u45925   (45925) dyno     (45925)     1320 2018-08-22 19:07:10.000000 edx-sga-0.8.3/edx_sga/static/js/bower/sinon/lib/sinon/typeOf.js
--rw-------   0 u45925   (45925) dyno     (45925)    11791 2018-08-22 19:07:10.000000 edx-sga-0.8.3/edx_sga/static/js/bower/sinon/lib/sinon/behavior.js
--rw-------   0 u45925   (45925) dyno     (45925)     3443 2018-08-22 19:07:10.000000 edx-sga-0.8.3/edx_sga/static/js/bower/sinon/lib/sinon/extend.js
--rw-------   0 u45925   (45925) dyno     (45925)    15777 2018-08-22 19:07:10.000000 edx-sga-0.8.3/edx_sga/static/js/bower/sinon/lib/sinon/mock.js
--rw-------   0 u45925   (45925) dyno     (45925)     1430 2018-08-22 19:07:10.000000 edx-sga-0.8.3/edx_sga/static/js/bower/sinon/lib/sinon.js
--rw-------   0 u45925   (45925) dyno     (45925)     1869 2018-08-22 19:07:10.000000 edx-sga-0.8.3/edx_sga/static/js/bower/sinon/README.md
--rw-------   0 u45925   (45925) dyno     (45925)      314 2018-08-22 19:07:10.000000 edx-sga-0.8.3/edx_sga/static/js/bower/sinon/.jscsrc
--rw-------   0 u45925   (45925) dyno     (45925)    23129 2018-08-22 19:07:10.000000 edx-sga-0.8.3/edx_sga/static/js/bower/sinon/Changelog.txt
--rw-------   0 u45925   (45925) dyno     (45925)      876 2018-08-22 19:07:10.000000 edx-sga-0.8.3/edx_sga/static/js/bower/sinon/.travis.yml
--rw-------   0 u45925   (45925) dyno     (45925)      378 2018-08-22 19:07:10.000000 edx-sga-0.8.3/edx_sga/static/js/bower/sinon/.bower.json
--rwx------   0 u45925   (45925) dyno     (45925)      438 2018-08-22 19:07:10.000000 edx-sga-0.8.3/edx_sga/static/js/bower/sinon/release.sh
-drwx------   0 u45925   (45925) dyno     (45925)        0 2018-08-22 19:07:34.000000 edx-sga-0.8.3/edx_sga/static/js/bower/sinon/scripts/
--rwx------   0 u45925   (45925) dyno     (45925)      231 2018-08-22 19:07:10.000000 edx-sga-0.8.3/edx_sga/static/js/bower/sinon/scripts/eslint-pre-commit
--rwx------   0 u45925   (45925) dyno     (45925)      768 2018-08-22 19:07:10.000000 edx-sga-0.8.3/edx_sga/static/js/bower/sinon/scripts/ci-test.sh
--rw-------   0 u45925   (45925) dyno     (45925)      744 2018-08-22 19:07:10.000000 edx-sga-0.8.3/edx_sga/static/js/bower/sinon/RELEASE.md
--rw-------   0 u45925   (45925) dyno     (45925)     4033 2018-08-22 19:07:10.000000 edx-sga-0.8.3/edx_sga/static/js/bower/sinon/AUTHORS
-drwx------   0 u45925   (45925) dyno     (45925)        0 2018-08-22 19:07:34.000000 edx-sga-0.8.3/edx_sga/static/js/bower/sinon/test/
--rw-------   0 u45925   (45925) dyno     (45925)     2247 2018-08-22 19:07:10.000000 edx-sga-0.8.3/edx_sga/static/js/bower/sinon/test/log-error-test.js
--rw-------   0 u45925   (45925) dyno     (45925)    34009 2018-08-22 19:07:10.000000 edx-sga-0.8.3/edx_sga/static/js/bower/sinon/test/mock-test.js
--rw-------   0 u45925   (45925) dyno     (45925)      841 2018-08-22 19:07:10.000000 edx-sga-0.8.3/edx_sga/static/js/bower/sinon/test/format-test.js
--rw-------   0 u45925   (45925) dyno     (45925)     1346 2018-08-22 19:07:10.000000 edx-sga-0.8.3/edx_sga/static/js/bower/sinon/test/typeOf-test.js
--rw-------   0 u45925   (45925) dyno     (45925)    58120 2018-08-22 19:07:10.000000 edx-sga-0.8.3/edx_sga/static/js/bower/sinon/test/stub-test.js
--rw-------   0 u45925   (45925) dyno     (45925)      347 2018-08-22 19:07:10.000000 edx-sga-0.8.3/edx_sga/static/js/bower/sinon/test/hello-world-test.js
--rw-------   0 u45925   (45925) dyno     (45925)    53776 2018-08-22 19:07:10.000000 edx-sga-0.8.3/edx_sga/static/js/bower/sinon/test/assert-test.js
--rw-------   0 u45925   (45925) dyno     (45925)     1537 2018-08-22 19:07:10.000000 edx-sga-0.8.3/edx_sga/static/js/bower/sinon/test/test-helper.js
--rw-------   0 u45925   (45925) dyno     (45925)    16139 2018-08-22 19:07:10.000000 edx-sga-0.8.3/edx_sga/static/js/bower/sinon/test/sandbox-test.js
--rw-------   0 u45925   (45925) dyno     (45925)      313 2018-08-22 19:07:10.000000 edx-sga-0.8.3/edx_sga/static/js/bower/sinon/test/buster-packaged.js
-drwx------   0 u45925   (45925) dyno     (45925)        0 2018-08-22 19:07:34.000000 edx-sga-0.8.3/edx_sga/static/js/bower/sinon/test/util/
--rw-------   0 u45925   (45925) dyno     (45925)    31795 2018-08-22 19:07:10.000000 edx-sga-0.8.3/edx_sga/static/js/bower/sinon/test/util/fake-server-test.js
--rw-------   0 u45925   (45925) dyno     (45925)     7532 2018-08-22 19:07:10.000000 edx-sga-0.8.3/edx_sga/static/js/bower/sinon/test/util/fake-server-with-clock-test.js
--rw-------   0 u45925   (45925) dyno     (45925)    14734 2018-08-22 19:07:10.000000 edx-sga-0.8.3/edx_sga/static/js/bower/sinon/test/util/fake-xdomain-request-test.js
--rw-------   0 u45925   (45925) dyno     (45925)     4643 2018-08-22 19:07:10.000000 edx-sga-0.8.3/edx_sga/static/js/bower/sinon/test/util/event-test.js
--rw-------   0 u45925   (45925) dyno     (45925)    36722 2018-08-22 19:07:10.000000 edx-sga-0.8.3/edx_sga/static/js/bower/sinon/test/util/fake-timers-test.js
--rw-------   0 u45925   (45925) dyno     (45925)    58912 2018-08-22 19:07:10.000000 edx-sga-0.8.3/edx_sga/static/js/bower/sinon/test/util/fake-xml-http-request-test.js
--rw-------   0 u45925   (45925) dyno     (45925)    22374 2018-08-22 19:07:10.000000 edx-sga-0.8.3/edx_sga/static/js/bower/sinon/test/match-test.js
--rw-------   0 u45925   (45925) dyno     (45925)    42564 2018-08-22 19:07:10.000000 edx-sga-0.8.3/edx_sga/static/js/bower/sinon/test/call-test.js
--rw-------   0 u45925   (45925) dyno     (45925)      896 2018-08-22 19:07:10.000000 edx-sga-0.8.3/edx_sga/static/js/bower/sinon/test/buster.js
-drwx------   0 u45925   (45925) dyno     (45925)        0 2018-08-22 19:07:34.000000 edx-sga-0.8.3/edx_sga/static/js/bower/sinon/test/issues/
--rw-------   0 u45925   (45925) dyno     (45925)     2971 2018-08-22 19:07:10.000000 edx-sga-0.8.3/edx_sga/static/js/bower/sinon/test/issues/issues-test.js
--rw-------   0 u45925   (45925) dyno     (45925)     1350 2018-08-22 19:07:10.000000 edx-sga-0.8.3/edx_sga/static/js/bower/sinon/test/times-in-words-test.js
--rw-------   0 u45925   (45925) dyno     (45925)    11924 2018-08-22 19:07:10.000000 edx-sga-0.8.3/edx_sga/static/js/bower/sinon/test/collection-test.js
--rw-------   0 u45925   (45925) dyno     (45925)     1807 2018-08-22 19:07:10.000000 edx-sga-0.8.3/edx_sga/static/js/bower/sinon/test/extend-test.js
--rw-------   0 u45925   (45925) dyno     (45925)    18694 2018-08-22 19:07:10.000000 edx-sga-0.8.3/edx_sga/static/js/bower/sinon/test/test-test.js
--rw-------   0 u45925   (45925) dyno     (45925)    69039 2018-08-22 19:07:10.000000 edx-sga-0.8.3/edx_sga/static/js/bower/sinon/test/spy-test.js
--rw-------   0 u45925   (45925) dyno     (45925)    24007 2018-08-22 19:07:10.000000 edx-sga-0.8.3/edx_sga/static/js/bower/sinon/test/sinon-test.js
--rw-------   0 u45925   (45925) dyno     (45925)     7641 2018-08-22 19:07:10.000000 edx-sga-0.8.3/edx_sga/static/js/bower/sinon/test/test-case-test.js
--rw-------   0 u45925   (45925) dyno     (45925)     6124 2018-08-22 19:07:10.000000 edx-sga-0.8.3/edx_sga/static/js/bower/sinon/.eslintrc
--rw-------   0 u45925   (45925) dyno     (45925)     1211 2018-08-22 19:07:10.000000 edx-sga-0.8.3/edx_sga/static/js/bower/sinon/package.json
--rw-------   0 u45925   (45925) dyno     (45925)      382 2018-08-22 19:07:10.000000 edx-sga-0.8.3/edx_sga/static/js/bower/sinon/.editorconfig
--rwx------   0 u45925   (45925) dyno     (45925)     4310 2018-08-22 19:07:10.000000 edx-sga-0.8.3/edx_sga/static/js/bower/sinon/build
--rw-------   0 u45925   (45925) dyno     (45925)     1572 2018-08-22 19:07:10.000000 edx-sga-0.8.3/edx_sga/static/js/bower/sinon/LICENSE
--rw-------   0 u45925   (45925) dyno     (45925)       27 2018-08-22 19:07:10.000000 edx-sga-0.8.3/edx_sga/static/js/bower/sinon/.gitignore
--rw-------   0 u45925   (45925) dyno     (45925)     5364 2018-08-22 19:07:10.000000 edx-sga-0.8.3/edx_sga/static/js/bower/sinon/CONTRIBUTING.md
-drwx------   0 u45925   (45925) dyno     (45925)        0 2018-08-22 19:07:34.000000 edx-sga-0.8.3/edx_sga/static/js/bower/requirejs/
--rw-------   0 u45925   (45925) dyno     (45925)    84263 2018-08-22 19:07:10.000000 edx-sga-0.8.3/edx_sga/static/js/bower/requirejs/require.js
--rw-------   0 u45925   (45925) dyno     (45925)       75 2018-08-22 19:07:10.000000 edx-sga-0.8.3/edx_sga/static/js/bower/requirejs/README.md
--rw-------   0 u45925   (45925) dyno     (45925)      592 2018-08-22 19:07:10.000000 edx-sga-0.8.3/edx_sga/static/js/bower/requirejs/.bower.json
--rw-------   0 u45925   (45925) dyno     (45925)      306 2018-08-22 19:07:10.000000 edx-sga-0.8.3/edx_sga/static/js/bower/requirejs/bower.json
-drwx------   0 u45925   (45925) dyno     (45925)        0 2018-08-22 19:07:34.000000 edx-sga-0.8.3/edx_sga/static/js/bower/jquery/
-drwx------   0 u45925   (45925) dyno     (45925)        0 2018-08-22 19:07:34.000000 edx-sga-0.8.3/edx_sga/static/js/bower/jquery/src/
-drwx------   0 u45925   (45925) dyno     (45925)        0 2018-08-22 19:07:34.000000 edx-sga-0.8.3/edx_sga/static/js/bower/jquery/src/attributes/
--rw-------   0 u45925   (45925) dyno     (45925)     3839 2018-08-22 19:07:10.000000 edx-sga-0.8.3/edx_sga/static/js/bower/jquery/src/attributes/val.js
--rw-------   0 u45925   (45925) dyno     (45925)      893 2018-08-22 19:07:10.000000 edx-sga-0.8.3/edx_sga/static/js/bower/jquery/src/attributes/support.js
--rw-------   0 u45925   (45925) dyno     (45925)     3320 2018-08-22 19:07:10.000000 edx-sga-0.8.3/edx_sga/static/js/bower/jquery/src/attributes/attr.js
--rw-------   0 u45925   (45925) dyno     (45925)     4155 2018-08-22 19:07:10.000000 edx-sga-0.8.3/edx_sga/static/js/bower/jquery/src/attributes/classes.js
--rw-------   0 u45925   (45925) dyno     (45925)     1854 2018-08-22 19:07:10.000000 edx-sga-0.8.3/edx_sga/static/js/bower/jquery/src/attributes/prop.js
--rw-------   0 u45925   (45925) dyno     (45925)       33 2018-08-22 19:07:10.000000 edx-sga-0.8.3/edx_sga/static/js/bower/jquery/src/selector.js
--rw-------   0 u45925   (45925) dyno     (45925)      294 2018-08-22 19:07:10.000000 edx-sga-0.8.3/edx_sga/static/js/bower/jquery/src/selector-sizzle.js
-drwx------   0 u45925   (45925) dyno     (45925)        0 2018-08-22 19:07:34.000000 edx-sga-0.8.3/edx_sga/static/js/bower/jquery/src/traversing/
--rw-------   0 u45925   (45925) dyno     (45925)     2464 2018-08-22 19:07:10.000000 edx-sga-0.8.3/edx_sga/static/js/bower/jquery/src/traversing/findFilter.js
-drwx------   0 u45925   (45925) dyno     (45925)        0 2018-08-22 19:07:34.000000 edx-sga-0.8.3/edx_sga/static/js/bower/jquery/src/traversing/var/
--rw-------   0 u45925   (45925) dyno     (45925)      110 2018-08-22 19:07:10.000000 edx-sga-0.8.3/edx_sga/static/js/bower/jquery/src/traversing/var/rneedsContext.js
-drwx------   0 u45925   (45925) dyno     (45925)        0 2018-08-22 19:07:34.000000 edx-sga-0.8.3/edx_sga/static/js/bower/jquery/src/exports/
--rw-------   0 u45925   (45925) dyno     (45925)      641 2018-08-22 19:07:10.000000 edx-sga-0.8.3/edx_sga/static/js/bower/jquery/src/exports/global.js
--rw-------   0 u45925   (45925) dyno     (45925)     1006 2018-08-22 19:07:10.000000 edx-sga-0.8.3/edx_sga/static/js/bower/jquery/src/exports/amd.js
--rw-------   0 u45925   (45925) dyno     (45925)     1393 2018-08-22 19:07:10.000000 edx-sga-0.8.3/edx_sga/static/js/bower/jquery/src/intro.js
--rw-------   0 u45925   (45925) dyno     (45925)     1776 2018-08-22 19:07:10.000000 edx-sga-0.8.3/edx_sga/static/js/bower/jquery/src/dimensions.js
-drwx------   0 u45925   (45925) dyno     (45925)        0 2018-08-22 19:07:34.000000 edx-sga-0.8.3/edx_sga/static/js/bower/jquery/src/queue/
--rw-------   0 u45925   (45925) dyno     (45925)      561 2018-08-22 19:07:10.000000 edx-sga-0.8.3/edx_sga/static/js/bower/jquery/src/queue/delay.js
--rw-------   0 u45925   (45925) dyno     (45925)    11790 2018-08-22 19:07:10.000000 edx-sga-0.8.3/edx_sga/static/js/bower/jquery/src/core.js
--rw-------   0 u45925   (45925) dyno     (45925)        5 2018-08-22 19:07:10.000000 edx-sga-0.8.3/edx_sga/static/js/bower/jquery/src/outro.js
--rw-------   0 u45925   (45925) dyno     (45925)    21168 2018-08-22 19:07:10.000000 edx-sga-0.8.3/edx_sga/static/js/bower/jquery/src/ajax.js
-drwx------   0 u45925   (45925) dyno     (45925)        0 2018-08-22 19:07:34.000000 edx-sga-0.8.3/edx_sga/static/js/bower/jquery/src/css/
--rw-------   0 u45925   (45925) dyno     (45925)     1867 2018-08-22 19:07:10.000000 edx-sga-0.8.3/edx_sga/static/js/bower/jquery/src/css/defaultDisplay.js
--rw-------   0 u45925   (45925) dyno     (45925)     3198 2018-08-22 19:07:10.000000 edx-sga-0.8.3/edx_sga/static/js/bower/jquery/src/css/support.js
--rw-------   0 u45925   (45925) dyno     (45925)      509 2018-08-22 19:07:10.000000 edx-sga-0.8.3/edx_sga/static/js/bower/jquery/src/css/addGetHookIf.js
--rw-------   0 u45925   (45925) dyno     (45925)     1452 2018-08-22 19:07:10.000000 edx-sga-0.8.3/edx_sga/static/js/bower/jquery/src/css/curCSS.js
-drwx------   0 u45925   (45925) dyno     (45925)        0 2018-08-22 19:07:34.000000 edx-sga-0.8.3/edx_sga/static/js/bower/jquery/src/css/var/
--rw-------   0 u45925   (45925) dyno     (45925)      410 2018-08-22 19:07:10.000000 edx-sga-0.8.3/edx_sga/static/js/bower/jquery/src/css/var/getStyles.js
--rw-------   0 u45925   (45925) dyno     (45925)       45 2018-08-22 19:07:10.000000 edx-sga-0.8.3/edx_sga/static/js/bower/jquery/src/css/var/rmargin.js
--rw-------   0 u45925   (45925) dyno     (45925)       70 2018-08-22 19:07:10.000000 edx-sga-0.8.3/edx_sga/static/js/bower/jquery/src/css/var/cssExpand.js
--rw-------   0 u45925   (45925) dyno     (45925)      113 2018-08-22 19:07:10.000000 edx-sga-0.8.3/edx_sga/static/js/bower/jquery/src/css/var/rnumnonpx.js
--rw-------   0 u45925   (45925) dyno     (45925)      355 2018-08-22 19:07:10.000000 edx-sga-0.8.3/edx_sga/static/js/bower/jquery/src/css/var/isHidden.js
--rw-------   0 u45925   (45925) dyno     (45925)      555 2018-08-22 19:07:10.000000 edx-sga-0.8.3/edx_sga/static/js/bower/jquery/src/css/swap.js
--rw-------   0 u45925   (45925) dyno     (45925)      380 2018-08-22 19:07:10.000000 edx-sga-0.8.3/edx_sga/static/js/bower/jquery/src/css/hiddenVisibleSelectors.js
--rw-------   0 u45925   (45925) dyno     (45925)    16914 2018-08-22 19:07:10.000000 edx-sga-0.8.3/edx_sga/static/js/bower/jquery/src/effects.js
--rw-------   0 u45925   (45925) dyno     (45925)     3214 2018-08-22 19:07:10.000000 edx-sga-0.8.3/edx_sga/static/js/bower/jquery/src/serialize.js
--rw-------   0 u45925   (45925) dyno     (45925)     5506 2018-08-22 19:07:10.000000 edx-sga-0.8.3/edx_sga/static/js/bower/jquery/src/callbacks.js
-drwx------   0 u45925   (45925) dyno     (45925)        0 2018-08-22 19:07:34.000000 edx-sga-0.8.3/edx_sga/static/js/bower/jquery/src/core/
--rw-------   0 u45925   (45925) dyno     (45925)     1210 2018-08-22 19:07:10.000000 edx-sga-0.8.3/edx_sga/static/js/bower/jquery/src/core/access.js
--rw-------   0 u45925   (45925) dyno     (45925)      938 2018-08-22 19:07:10.000000 edx-sga-0.8.3/edx_sga/static/js/bower/jquery/src/core/parseHTML.js
--rw-------   0 u45925   (45925) dyno     (45925)     3401 2018-08-22 19:07:10.000000 edx-sga-0.8.3/edx_sga/static/js/bower/jquery/src/core/init.js
--rw-------   0 u45925   (45925) dyno     (45925)     2381 2018-08-22 19:07:10.000000 edx-sga-0.8.3/edx_sga/static/js/bower/jquery/src/core/ready.js
-drwx------   0 u45925   (45925) dyno     (45925)        0 2018-08-22 19:07:34.000000 edx-sga-0.8.3/edx_sga/static/js/bower/jquery/src/core/var/
--rw-------   0 u45925   (45925) dyno     (45925)       91 2018-08-22 19:07:10.000000 edx-sga-0.8.3/edx_sga/static/js/bower/jquery/src/core/var/rsingleTag.js
--rw-------   0 u45925   (45925) dyno     (45925)     3063 2018-08-22 19:07:10.000000 edx-sga-0.8.3/edx_sga/static/js/bower/jquery/src/queue.js
--rw-------   0 u45925   (45925) dyno     (45925)    15039 2018-08-22 19:07:10.000000 edx-sga-0.8.3/edx_sga/static/js/bower/jquery/src/manipulation.js
--rw-------   0 u45925   (45925) dyno     (45925)      223 2018-08-22 19:07:10.000000 edx-sga-0.8.3/edx_sga/static/js/bower/jquery/src/deprecated.js
-drwx------   0 u45925   (45925) dyno     (45925)        0 2018-08-22 19:07:34.000000 edx-sga-0.8.3/edx_sga/static/js/bower/jquery/src/effects/
--rw-------   0 u45925   (45925) dyno     (45925)      225 2018-08-22 19:07:10.000000 edx-sga-0.8.3/edx_sga/static/js/bower/jquery/src/effects/animatedSelector.js
--rw-------   0 u45925   (45925) dyno     (45925)     3028 2018-08-22 19:07:10.000000 edx-sga-0.8.3/edx_sga/static/js/bower/jquery/src/effects/Tween.js
--rw-------   0 u45925   (45925) dyno     (45925)    12346 2018-08-22 19:07:10.000000 edx-sga-0.8.3/edx_sga/static/js/bower/jquery/src/css.js
-drwx------   0 u45925   (45925) dyno     (45925)        0 2018-08-22 19:07:34.000000 edx-sga-0.8.3/edx_sga/static/js/bower/jquery/src/var/
--rw-------   0 u45925   (45925) dyno     (45925)       64 2018-08-22 19:07:10.000000 edx-sga-0.8.3/edx_sga/static/js/bower/jquery/src/var/indexOf.js
--rw-------   0 u45925   (45925) dyno     (45925)       63 2018-08-22 19:07:10.000000 edx-sga-0.8.3/edx_sga/static/js/bower/jquery/src/var/concat.js
--rw-------   0 u45925   (45925) dyno     (45925)       36 2018-08-22 19:07:10.000000 edx-sga-0.8.3/edx_sga/static/js/bower/jquery/src/var/arr.js
--rw-------   0 u45925   (45925) dyno     (45925)       99 2018-08-22 19:07:10.000000 edx-sga-0.8.3/edx_sga/static/js/bower/jquery/src/var/support.js
--rw-------   0 u45925   (45925) dyno     (45925)       42 2018-08-22 19:07:10.000000 edx-sga-0.8.3/edx_sga/static/js/bower/jquery/src/var/rnotwhite.js
--rw-------   0 u45925   (45925) dyno     (45925)       86 2018-08-22 19:07:10.000000 edx-sga-0.8.3/edx_sga/static/js/bower/jquery/src/var/toString.js
--rw-------   0 u45925   (45925) dyno     (45925)       61 2018-08-22 19:07:10.000000 edx-sga-0.8.3/edx_sga/static/js/bower/jquery/src/var/push.js
--rw-------   0 u45925   (45925) dyno     (45925)       62 2018-08-22 19:07:10.000000 edx-sga-0.8.3/edx_sga/static/js/bower/jquery/src/var/slice.js
--rw-------   0 u45925   (45925) dyno     (45925)       92 2018-08-22 19:07:10.000000 edx-sga-0.8.3/edx_sga/static/js/bower/jquery/src/var/hasOwn.js
--rw-------   0 u45925   (45925) dyno     (45925)       64 2018-08-22 19:07:10.000000 edx-sga-0.8.3/edx_sga/static/js/bower/jquery/src/var/class2type.js
--rw-------   0 u45925   (45925) dyno     (45925)       80 2018-08-22 19:07:10.000000 edx-sga-0.8.3/edx_sga/static/js/bower/jquery/src/var/pnum.js
--rw-------   0 u45925   (45925) dyno     (45925)       50 2018-08-22 19:07:10.000000 edx-sga-0.8.3/edx_sga/static/js/bower/jquery/src/var/strundefined.js
-drwx------   0 u45925   (45925) dyno     (45925)        0 2018-08-22 19:07:34.000000 edx-sga-0.8.3/edx_sga/static/js/bower/jquery/src/ajax/
--rw-------   0 u45925   (45925) dyno     (45925)     2516 2018-08-22 19:07:10.000000 edx-sga-0.8.3/edx_sga/static/js/bower/jquery/src/ajax/jsonp.js
--rw-------   0 u45925   (45925) dyno     (45925)     1669 2018-08-22 19:07:10.000000 edx-sga-0.8.3/edx_sga/static/js/bower/jquery/src/ajax/load.js
-drwx------   0 u45925   (45925) dyno     (45925)        0 2018-08-22 19:07:34.000000 edx-sga-0.8.3/edx_sga/static/js/bower/jquery/src/ajax/var/
--rw-------   0 u45925   (45925) dyno     (45925)       40 2018-08-22 19:07:10.000000 edx-sga-0.8.3/edx_sga/static/js/bower/jquery/src/ajax/var/rquery.js
--rw-------   0 u45925   (45925) dyno     (45925)       73 2018-08-22 19:07:10.000000 edx-sga-0.8.3/edx_sga/static/js/bower/jquery/src/ajax/var/nonce.js
--rw-------   0 u45925   (45925) dyno     (45925)      222 2018-08-22 19:07:10.000000 edx-sga-0.8.3/edx_sga/static/js/bower/jquery/src/ajax/parseJSON.js
--rw-------   0 u45925   (45925) dyno     (45925)      485 2018-08-22 19:07:10.000000 edx-sga-0.8.3/edx_sga/static/js/bower/jquery/src/ajax/parseXML.js
--rw-------   0 u45925   (45925) dyno     (45925)     3488 2018-08-22 19:07:10.000000 edx-sga-0.8.3/edx_sga/static/js/bower/jquery/src/ajax/xhr.js
--rw-------   0 u45925   (45925) dyno     (45925)     1271 2018-08-22 19:07:10.000000 edx-sga-0.8.3/edx_sga/static/js/bower/jquery/src/ajax/script.js
-drwx------   0 u45925   (45925) dyno     (45925)        0 2018-08-22 19:07:34.000000 edx-sga-0.8.3/edx_sga/static/js/bower/jquery/src/manipulation/
--rw-------   0 u45925   (45925) dyno     (45925)      975 2018-08-22 19:07:10.000000 edx-sga-0.8.3/edx_sga/static/js/bower/jquery/src/manipulation/support.js
--rw-------   0 u45925   (45925) dyno     (45925)      240 2018-08-22 19:07:10.000000 edx-sga-0.8.3/edx_sga/static/js/bower/jquery/src/manipulation/_evalUrl.js
-drwx------   0 u45925   (45925) dyno     (45925)        0 2018-08-22 19:07:34.000000 edx-sga-0.8.3/edx_sga/static/js/bower/jquery/src/manipulation/var/
--rw-------   0 u45925   (45925) dyno     (45925)       59 2018-08-22 19:07:10.000000 edx-sga-0.8.3/edx_sga/static/js/bower/jquery/src/manipulation/var/rcheckableType.js
--rw-------   0 u45925   (45925) dyno     (45925)     1496 2018-08-22 19:07:10.000000 edx-sga-0.8.3/edx_sga/static/js/bower/jquery/src/wrap.js
--rw-------   0 u45925   (45925) dyno     (45925)      200 2018-08-22 19:07:10.000000 edx-sga-0.8.3/edx_sga/static/js/bower/jquery/src/attributes.js
--rw-------   0 u45925   (45925) dyno     (45925)     4434 2018-08-22 19:07:10.000000 edx-sga-0.8.3/edx_sga/static/js/bower/jquery/src/selector-native.js
-drwx------   0 u45925   (45925) dyno     (45925)        0 2018-08-22 19:07:34.000000 edx-sga-0.8.3/edx_sga/static/js/bower/jquery/src/data/
--rw-------   0 u45925   (45925) dyno     (45925)      383 2018-08-22 19:07:10.000000 edx-sga-0.8.3/edx_sga/static/js/bower/jquery/src/data/accepts.js
--rw-------   0 u45925   (45925) dyno     (45925)     4882 2018-08-22 19:07:10.000000 edx-sga-0.8.3/edx_sga/static/js/bower/jquery/src/data/Data.js
-drwx------   0 u45925   (45925) dyno     (45925)        0 2018-08-22 19:07:34.000000 edx-sga-0.8.3/edx_sga/static/js/bower/jquery/src/data/var/
--rw-------   0 u45925   (45925) dyno     (45925)       66 2018-08-22 19:07:10.000000 edx-sga-0.8.3/edx_sga/static/js/bower/jquery/src/data/var/data_priv.js
--rw-------   0 u45925   (45925) dyno     (45925)       66 2018-08-22 19:07:10.000000 edx-sga-0.8.3/edx_sga/static/js/bower/jquery/src/data/var/data_user.js
--rw-------   0 u45925   (45925) dyno     (45925)     4535 2018-08-22 19:07:10.000000 edx-sga-0.8.3/edx_sga/static/js/bower/jquery/src/traversing.js
-drwx------   0 u45925   (45925) dyno     (45925)        0 2018-08-22 19:07:34.000000 edx-sga-0.8.3/edx_sga/static/js/bower/jquery/src/event/
--rw-------   0 u45925   (45925) dyno     (45925)      123 2018-08-22 19:07:10.000000 edx-sga-0.8.3/edx_sga/static/js/bower/jquery/src/event/support.js
--rw-------   0 u45925   (45925) dyno     (45925)      322 2018-08-22 19:07:10.000000 edx-sga-0.8.3/edx_sga/static/js/bower/jquery/src/event/ajax.js
--rw-------   0 u45925   (45925) dyno     (45925)     1094 2018-08-22 19:07:10.000000 edx-sga-0.8.3/edx_sga/static/js/bower/jquery/src/event/alias.js
--rw-------   0 u45925   (45925) dyno     (45925)    24475 2018-08-22 19:07:10.000000 edx-sga-0.8.3/edx_sga/static/js/bower/jquery/src/event.js
--rw-------   0 u45925   (45925) dyno     (45925)     5588 2018-08-22 19:07:10.000000 edx-sga-0.8.3/edx_sga/static/js/bower/jquery/src/offset.js
--rw-------   0 u45925   (45925) dyno     (45925)     4414 2018-08-22 19:07:10.000000 edx-sga-0.8.3/edx_sga/static/js/bower/jquery/src/deferred.js
--rw-------   0 u45925   (45925) dyno     (45925)      574 2018-08-22 19:07:10.000000 edx-sga-0.8.3/edx_sga/static/js/bower/jquery/src/jquery.js
--rw-------   0 u45925   (45925) dyno     (45925)     4942 2018-08-22 19:07:10.000000 edx-sga-0.8.3/edx_sga/static/js/bower/jquery/src/data.js
--rw-------   0 u45925   (45925) dyno     (45925)     1099 2018-08-22 19:07:10.000000 edx-sga-0.8.3/edx_sga/static/js/bower/jquery/MIT-LICENSE.txt
--rw-------   0 u45925   (45925) dyno     (45925)      752 2018-08-22 19:07:10.000000 edx-sga-0.8.3/edx_sga/static/js/bower/jquery/.bower.json
--rw-------   0 u45925   (45925) dyno     (45925)      451 2018-08-22 19:07:10.000000 edx-sga-0.8.3/edx_sga/static/js/bower/jquery/bower.json
-drwx------   0 u45925   (45925) dyno     (45925)        0 2018-08-22 19:07:34.000000 edx-sga-0.8.3/edx_sga/static/js/bower/URIjs/
--rw-------   0 u45925   (45925) dyno     (45925)    35696 2018-08-22 19:07:10.000000 edx-sga-0.8.3/edx_sga/static/js/bower/URIjs/README.md
-drwx------   0 u45925   (45925) dyno     (45925)        0 2018-08-22 19:07:34.000000 edx-sga-0.8.3/edx_sga/static/js/bower/URIjs/src/
--rw-------   0 u45925   (45925) dyno     (45925)     2600 2018-08-22 19:07:10.000000 edx-sga-0.8.3/edx_sga/static/js/bower/URIjs/src/jquery.URI.min.js
--rw-------   0 u45925   (45925) dyno     (45925)    44088 2018-08-22 19:07:10.000000 edx-sga-0.8.3/edx_sga/static/js/bower/URIjs/src/URI.min.js
--rw-------   0 u45925   (45925) dyno     (45925)    14811 2018-08-22 19:07:10.000000 edx-sga-0.8.3/edx_sga/static/js/bower/URIjs/src/URITemplate.js
--rw-------   0 u45925   (45925) dyno     (45925)     3185 2018-08-22 19:07:10.000000 edx-sga-0.8.3/edx_sga/static/js/bower/URIjs/src/URI.fragmentQuery.js
--rw-------   0 u45925   (45925) dyno     (45925)    11908 2018-08-22 19:07:10.000000 edx-sga-0.8.3/edx_sga/static/js/bower/URIjs/src/SecondLevelDomains.js
--rw-------   0 u45925   (45925) dyno     (45925)     6740 2018-08-22 19:07:10.000000 edx-sga-0.8.3/edx_sga/static/js/bower/URIjs/src/jquery.URI.js
--rw-------   0 u45925   (45925) dyno     (45925)     4491 2018-08-22 19:07:10.000000 edx-sga-0.8.3/edx_sga/static/js/bower/URIjs/src/IPv6.js
--rw-------   0 u45925   (45925) dyno     (45925)    13969 2018-08-22 19:07:10.000000 edx-sga-0.8.3/edx_sga/static/js/bower/URIjs/src/punycode.js
--rw-------   0 u45925   (45925) dyno     (45925)     2736 2018-08-22 19:07:10.000000 edx-sga-0.8.3/edx_sga/static/js/bower/URIjs/src/URI.fragmentURI.js
--rw-------   0 u45925   (45925) dyno     (45925)    60844 2018-08-22 19:07:10.000000 edx-sga-0.8.3/edx_sga/static/js/bower/URIjs/src/URI.js
--rw-------   0 u45925   (45925) dyno     (45925)      524 2018-08-22 19:07:10.000000 edx-sga-0.8.3/edx_sga/static/js/bower/URIjs/.bower.json
--rw-------   0 u45925   (45925) dyno     (45925)     1077 2018-08-22 19:07:10.000000 edx-sga-0.8.3/edx_sga/static/js/bower/URIjs/LICENSE.txt
--rw-------   0 u45925   (45925) dyno     (45925)     1154 2018-08-22 19:07:10.000000 edx-sga-0.8.3/edx_sga/static/js/bower/URIjs/contributing.md
--rw-------   0 u45925   (45925) dyno     (45925)      214 2018-08-22 19:07:10.000000 edx-sga-0.8.3/edx_sga/static/js/bower/URIjs/bower.json
-drwx------   0 u45925   (45925) dyno     (45925)        0 2018-08-22 19:07:34.000000 edx-sga-0.8.3/edx_sga/tests/
--rw-------   0 u45925   (45925) dyno     (45925)    40407 2018-08-22 19:07:10.000000 edx-sga-0.8.3/edx_sga/tests/integration_tests.py
--rw-------   0 u45925   (45925) dyno     (45925)     3917 2018-08-22 19:07:10.000000 edx-sga-0.8.3/edx_sga/tests/common.py
--rw-------   0 u45925   (45925) dyno     (45925)    29655 2018-08-22 19:07:10.000000 edx-sga-0.8.3/edx_sga/tests/test_sga.py
--rw-------   0 u45925   (45925) dyno     (45925)        0 2018-08-22 19:07:10.000000 edx-sga-0.8.3/edx_sga/tests/__init__.py
--rw-------   0 u45925   (45925) dyno     (45925)      914 2018-08-22 19:07:10.000000 edx-sga-0.8.3/edx_sga/tests/test_utils.py
--rw-------   0 u45925   (45925) dyno     (45925)     5326 2018-08-22 19:07:10.000000 edx-sga-0.8.3/edx_sga/tests/test_showanswer.py
--rw-------   0 u45925   (45925) dyno     (45925)       71 2018-08-22 19:07:10.000000 edx-sga-0.8.3/edx_sga/__init__.py
-drwx------   0 u45925   (45925) dyno     (45925)        0 2018-08-22 19:07:34.000000 edx-sga-0.8.3/edx_sga/templates/
-drwx------   0 u45925   (45925) dyno     (45925)        0 2018-08-22 19:07:34.000000 edx-sga-0.8.3/edx_sga/templates/staff_graded_assignment/
--rw-------   0 u45925   (45925) dyno     (45925)     7948 2018-08-22 19:07:10.000000 edx-sga-0.8.3/edx_sga/templates/staff_graded_assignment/show.html
--rw-------   0 u45925   (45925) dyno     (45925)     5438 2018-08-22 19:07:10.000000 edx-sga-0.8.3/edx_sga/tasks.py
--rw-------   0 u45925   (45925) dyno     (45925)     3998 2018-08-22 19:07:10.000000 edx-sga-0.8.3/edx_sga/showanswer.py
--rw-------   0 u45925   (45925) dyno     (45925)      462 2018-08-22 19:07:10.000000 edx-sga-0.8.3/edx_sga/wsgi.py
--rw-------   0 u45925   (45925) dyno     (45925)     1988 2018-08-22 19:07:10.000000 edx-sga-0.8.3/edx_sga/test_settings.py
--rw-------   0 u45925   (45925) dyno     (45925)    12950 2018-08-22 19:07:10.000000 edx-sga-0.8.3/README.md
--rw-------   0 u45925   (45925) dyno     (45925)       38 2018-08-22 19:07:34.000000 edx-sga-0.8.3/setup.cfg
--rw-------   0 u45925   (45925) dyno     (45925)      272 2018-08-22 19:07:34.000000 edx-sga-0.8.3/PKG-INFO
-drwx------   0 u45925   (45925) dyno     (45925)        0 2018-08-22 19:07:34.000000 edx-sga-0.8.3/edx_sga.egg-info/
--rw-------   0 u45925   (45925) dyno     (45925)        1 2018-08-22 19:07:34.000000 edx-sga-0.8.3/edx_sga.egg-info/dependency_links.txt
--rw-------   0 u45925   (45925) dyno     (45925)      272 2018-08-22 19:07:34.000000 edx-sga-0.8.3/edx_sga.egg-info/PKG-INFO
--rw-------   0 u45925   (45925) dyno     (45925)    10767 2018-08-22 19:07:34.000000 edx-sga-0.8.3/edx_sga.egg-info/SOURCES.txt
--rw-------   0 u45925   (45925) dyno     (45925)        1 2018-08-22 19:07:34.000000 edx-sga-0.8.3/edx_sga.egg-info/not-zip-safe
--rw-------   0 u45925   (45925) dyno     (45925)       20 2018-08-22 19:07:34.000000 edx-sga-0.8.3/edx_sga.egg-info/requires.txt
--rw-------   0 u45925   (45925) dyno     (45925)        8 2018-08-22 19:07:34.000000 edx-sga-0.8.3/edx_sga.egg-info/top_level.txt
--rw-------   0 u45925   (45925) dyno     (45925)       63 2018-08-22 19:07:34.000000 edx-sga-0.8.3/edx_sga.egg-info/entry_points.txt
--rw-------   0 u45925   (45925) dyno     (45925)     1044 2018-08-22 19:07:10.000000 edx-sga-0.8.3/setup.py
--rw-------   0 u45925   (45925) dyno     (45925)      108 2018-08-22 19:07:10.000000 edx-sga-0.8.3/MANIFEST.in
+drwx------   0 u56791   (56791) dyno     (56791)        0 2019-10-01 15:39:33.000000 edx-sga-0.9.0/
+-rw-------   0 u56791   (56791) dyno     (56791)      108 2019-10-01 15:39:23.000000 edx-sga-0.9.0/MANIFEST.in
+-rw-------   0 u56791   (56791) dyno     (56791)       38 2019-10-01 15:39:33.000000 edx-sga-0.9.0/setup.cfg
+drwx------   0 u56791   (56791) dyno     (56791)        0 2019-10-01 15:39:33.000000 edx-sga-0.9.0/edx_sga/
+drwx------   0 u56791   (56791) dyno     (56791)        0 2019-10-01 15:39:33.000000 edx-sga-0.9.0/edx_sga/tests/
+-rw-------   0 u56791   (56791) dyno     (56791)     5326 2019-10-01 15:39:23.000000 edx-sga-0.9.0/edx_sga/tests/test_showanswer.py
+-rw-------   0 u56791   (56791) dyno     (56791)     3917 2019-10-01 15:39:23.000000 edx-sga-0.9.0/edx_sga/tests/common.py
+-rw-------   0 u56791   (56791) dyno     (56791)      914 2019-10-01 15:39:23.000000 edx-sga-0.9.0/edx_sga/tests/test_utils.py
+-rw-------   0 u56791   (56791) dyno     (56791)    31677 2019-10-01 15:39:23.000000 edx-sga-0.9.0/edx_sga/tests/test_sga.py
+-rw-------   0 u56791   (56791) dyno     (56791)    40452 2019-10-01 15:39:23.000000 edx-sga-0.9.0/edx_sga/tests/integration_tests.py
+-rw-------   0 u56791   (56791) dyno     (56791)        0 2019-10-01 15:39:23.000000 edx-sga-0.9.0/edx_sga/tests/__init__.py
+drwx------   0 u56791   (56791) dyno     (56791)        0 2019-10-01 15:39:33.000000 edx-sga-0.9.0/edx_sga/templates/
+drwx------   0 u56791   (56791) dyno     (56791)        0 2019-10-01 15:39:33.000000 edx-sga-0.9.0/edx_sga/templates/staff_graded_assignment/
+-rw-------   0 u56791   (56791) dyno     (56791)     8056 2019-10-01 15:39:23.000000 edx-sga-0.9.0/edx_sga/templates/staff_graded_assignment/show.html
+-rw-------   0 u56791   (56791) dyno     (56791)     5438 2019-10-01 15:39:23.000000 edx-sga-0.9.0/edx_sga/tasks.py
+-rw-------   0 u56791   (56791) dyno     (56791)     1988 2019-10-01 15:39:23.000000 edx-sga-0.9.0/edx_sga/test_settings.py
+-rw-------   0 u56791   (56791) dyno     (56791)     2203 2019-10-01 15:39:23.000000 edx-sga-0.9.0/edx_sga/utils.py
+drwx------   0 u56791   (56791) dyno     (56791)        0 2019-10-01 15:39:33.000000 edx-sga-0.9.0/edx_sga/management/
+drwx------   0 u56791   (56791) dyno     (56791)        0 2019-10-01 15:39:33.000000 edx-sga-0.9.0/edx_sga/management/commands/
+-rw-------   0 u56791   (56791) dyno     (56791)       36 2019-10-01 15:39:23.000000 edx-sga-0.9.0/edx_sga/management/commands/__init__.py
+-rw-------   0 u56791   (56791) dyno     (56791)     2813 2019-10-01 15:39:23.000000 edx-sga-0.9.0/edx_sga/management/commands/sga_migrate_submissions.py
+-rw-------   0 u56791   (56791) dyno     (56791)       36 2019-10-01 15:39:23.000000 edx-sga-0.9.0/edx_sga/management/__init__.py
+-rw-------   0 u56791   (56791) dyno     (56791)      365 2019-10-01 15:39:23.000000 edx-sga-0.9.0/edx_sga/constants.py
+drwx------   0 u56791   (56791) dyno     (56791)        0 2019-10-01 15:39:33.000000 edx-sga-0.9.0/edx_sga/locale/
+-rw-------   0 u56791   (56791) dyno     (56791)      588 2019-10-01 15:39:23.000000 edx-sga-0.9.0/edx_sga/locale/config.yaml
+drwx------   0 u56791   (56791) dyno     (56791)        0 2019-10-01 15:39:33.000000 edx-sga-0.9.0/edx_sga/locale/fake2/
+drwx------   0 u56791   (56791) dyno     (56791)        0 2019-10-01 15:39:33.000000 edx-sga-0.9.0/edx_sga/locale/fake2/LC_MESSAGES/
+-rw-------   0 u56791   (56791) dyno     (56791)     7578 2019-10-01 15:39:23.000000 edx-sga-0.9.0/edx_sga/locale/fake2/LC_MESSAGES/django.po
+-rw-------   0 u56791   (56791) dyno     (56791)     1842 2019-10-01 15:39:23.000000 edx-sga-0.9.0/edx_sga/locale/fake2/LC_MESSAGES/djangojs.po
+-rw-------   0 u56791   (56791) dyno     (56791)     5090 2019-10-01 15:39:23.000000 edx-sga-0.9.0/edx_sga/locale/fake2/LC_MESSAGES/django.mo
+-rw-------   0 u56791   (56791) dyno     (56791)     1321 2019-10-01 15:39:23.000000 edx-sga-0.9.0/edx_sga/locale/fake2/LC_MESSAGES/djangojs.mo
+drwx------   0 u56791   (56791) dyno     (56791)        0 2019-10-01 15:39:33.000000 edx-sga-0.9.0/edx_sga/locale/rtl/
+drwx------   0 u56791   (56791) dyno     (56791)        0 2019-10-01 15:39:33.000000 edx-sga-0.9.0/edx_sga/locale/rtl/LC_MESSAGES/
+-rw-------   0 u56791   (56791) dyno     (56791)     7848 2019-10-01 15:39:23.000000 edx-sga-0.9.0/edx_sga/locale/rtl/LC_MESSAGES/django.po
+-rw-------   0 u56791   (56791) dyno     (56791)     1885 2019-10-01 15:39:23.000000 edx-sga-0.9.0/edx_sga/locale/rtl/LC_MESSAGES/djangojs.po
+-rw-------   0 u56791   (56791) dyno     (56791)     5360 2019-10-01 15:39:23.000000 edx-sga-0.9.0/edx_sga/locale/rtl/LC_MESSAGES/django.mo
+-rw-------   0 u56791   (56791) dyno     (56791)     1364 2019-10-01 15:39:23.000000 edx-sga-0.9.0/edx_sga/locale/rtl/LC_MESSAGES/djangojs.mo
+drwx------   0 u56791   (56791) dyno     (56791)        0 2019-10-01 15:39:33.000000 edx-sga-0.9.0/edx_sga/locale/en/
+drwx------   0 u56791   (56791) dyno     (56791)        0 2019-10-01 15:39:33.000000 edx-sga-0.9.0/edx_sga/locale/en/LC_MESSAGES/
+-rw-------   0 u56791   (56791) dyno     (56791)     5404 2019-10-01 15:39:23.000000 edx-sga-0.9.0/edx_sga/locale/en/LC_MESSAGES/django.po
+-rw-------   0 u56791   (56791) dyno     (56791)     1395 2019-10-01 15:39:23.000000 edx-sga-0.9.0/edx_sga/locale/en/LC_MESSAGES/djangojs.po
+-rw-------   0 u56791   (56791) dyno     (56791)      378 2019-10-01 15:39:23.000000 edx-sga-0.9.0/edx_sga/locale/en/LC_MESSAGES/django.mo
+-rw-------   0 u56791   (56791) dyno     (56791)      378 2019-10-01 15:39:23.000000 edx-sga-0.9.0/edx_sga/locale/en/LC_MESSAGES/djangojs.mo
+drwx------   0 u56791   (56791) dyno     (56791)        0 2019-10-01 15:39:33.000000 edx-sga-0.9.0/edx_sga/locale/eo/
+drwx------   0 u56791   (56791) dyno     (56791)        0 2019-10-01 15:39:33.000000 edx-sga-0.9.0/edx_sga/locale/eo/LC_MESSAGES/
+-rw-------   0 u56791   (56791) dyno     (56791)     9860 2019-10-01 15:39:23.000000 edx-sga-0.9.0/edx_sga/locale/eo/LC_MESSAGES/django.po
+-rw-------   0 u56791   (56791) dyno     (56791)     2379 2019-10-01 15:39:23.000000 edx-sga-0.9.0/edx_sga/locale/eo/LC_MESSAGES/djangojs.po
+-rw-------   0 u56791   (56791) dyno     (56791)     7312 2019-10-01 15:39:23.000000 edx-sga-0.9.0/edx_sga/locale/eo/LC_MESSAGES/django.mo
+-rw-------   0 u56791   (56791) dyno     (56791)     1846 2019-10-01 15:39:23.000000 edx-sga-0.9.0/edx_sga/locale/eo/LC_MESSAGES/djangojs.mo
+drwx------   0 u56791   (56791) dyno     (56791)        0 2019-10-01 15:39:33.000000 edx-sga-0.9.0/edx_sga/static/
+drwx------   0 u56791   (56791) dyno     (56791)        0 2019-10-01 15:39:33.000000 edx-sga-0.9.0/edx_sga/static/js/
+drwx------   0 u56791   (56791) dyno     (56791)        0 2019-10-01 15:39:33.000000 edx-sga-0.9.0/edx_sga/static/js/src/
+-rw-------   0 u56791   (56791) dyno     (56791)      829 2019-10-01 15:39:23.000000 edx-sga-0.9.0/edx_sga/static/js/src/studio.js
+-rw-------   0 u56791   (56791) dyno     (56791)    16520 2019-10-01 15:39:23.000000 edx-sga-0.9.0/edx_sga/static/js/src/jquery.tablesorter.min.js
+-rw-------   0 u56791   (56791) dyno     (56791)    19408 2019-10-01 15:39:23.000000 edx-sga-0.9.0/edx_sga/static/js/src/edx_sga.js
+drwx------   0 u56791   (56791) dyno     (56791)        0 2019-10-01 15:39:33.000000 edx-sga-0.9.0/edx_sga/static/js/bower/
+drwx------   0 u56791   (56791) dyno     (56791)        0 2019-10-01 15:39:33.000000 edx-sga-0.9.0/edx_sga/static/js/bower/underscore/
+-rw-------   0 u56791   (56791) dyno     (56791)     1117 2019-10-01 15:39:23.000000 edx-sga-0.9.0/edx_sga/static/js/bower/underscore/LICENSE
+-rw-------   0 u56791   (56791) dyno     (56791)    27589 2019-10-01 15:39:23.000000 edx-sga-0.9.0/edx_sga/static/js/bower/underscore/underscore-min.map
+-rw-------   0 u56791   (56791) dyno     (56791)      293 2019-10-01 15:39:23.000000 edx-sga-0.9.0/edx_sga/static/js/bower/underscore/bower.json
+-rw-------   0 u56791   (56791) dyno     (56791)    16449 2019-10-01 15:39:23.000000 edx-sga-0.9.0/edx_sga/static/js/bower/underscore/underscore-min.js
+-rw-------   0 u56791   (56791) dyno     (56791)     1225 2019-10-01 15:39:23.000000 edx-sga-0.9.0/edx_sga/static/js/bower/underscore/README.md
+-rw-------   0 u56791   (56791) dyno     (56791)    52919 2019-10-01 15:39:23.000000 edx-sga-0.9.0/edx_sga/static/js/bower/underscore/underscore.js
+-rw-------   0 u56791   (56791) dyno     (56791)      702 2019-10-01 15:39:23.000000 edx-sga-0.9.0/edx_sga/static/js/bower/underscore/.bower.json
+drwx------   0 u56791   (56791) dyno     (56791)        0 2019-10-01 15:39:33.000000 edx-sga-0.9.0/edx_sga/static/js/bower/URIjs/
+drwx------   0 u56791   (56791) dyno     (56791)        0 2019-10-01 15:39:33.000000 edx-sga-0.9.0/edx_sga/static/js/bower/URIjs/src/
+-rw-------   0 u56791   (56791) dyno     (56791)     2600 2019-10-01 15:39:23.000000 edx-sga-0.9.0/edx_sga/static/js/bower/URIjs/src/jquery.URI.min.js
+-rw-------   0 u56791   (56791) dyno     (56791)     2736 2019-10-01 15:39:23.000000 edx-sga-0.9.0/edx_sga/static/js/bower/URIjs/src/URI.fragmentURI.js
+-rw-------   0 u56791   (56791) dyno     (56791)    13969 2019-10-01 15:39:23.000000 edx-sga-0.9.0/edx_sga/static/js/bower/URIjs/src/punycode.js
+-rw-------   0 u56791   (56791) dyno     (56791)     4491 2019-10-01 15:39:23.000000 edx-sga-0.9.0/edx_sga/static/js/bower/URIjs/src/IPv6.js
+-rw-------   0 u56791   (56791) dyno     (56791)    11908 2019-10-01 15:39:23.000000 edx-sga-0.9.0/edx_sga/static/js/bower/URIjs/src/SecondLevelDomains.js
+-rw-------   0 u56791   (56791) dyno     (56791)    44088 2019-10-01 15:39:23.000000 edx-sga-0.9.0/edx_sga/static/js/bower/URIjs/src/URI.min.js
+-rw-------   0 u56791   (56791) dyno     (56791)     3185 2019-10-01 15:39:23.000000 edx-sga-0.9.0/edx_sga/static/js/bower/URIjs/src/URI.fragmentQuery.js
+-rw-------   0 u56791   (56791) dyno     (56791)    14811 2019-10-01 15:39:23.000000 edx-sga-0.9.0/edx_sga/static/js/bower/URIjs/src/URITemplate.js
+-rw-------   0 u56791   (56791) dyno     (56791)    60844 2019-10-01 15:39:23.000000 edx-sga-0.9.0/edx_sga/static/js/bower/URIjs/src/URI.js
+-rw-------   0 u56791   (56791) dyno     (56791)     6740 2019-10-01 15:39:23.000000 edx-sga-0.9.0/edx_sga/static/js/bower/URIjs/src/jquery.URI.js
+-rw-------   0 u56791   (56791) dyno     (56791)     1154 2019-10-01 15:39:23.000000 edx-sga-0.9.0/edx_sga/static/js/bower/URIjs/contributing.md
+-rw-------   0 u56791   (56791) dyno     (56791)      214 2019-10-01 15:39:23.000000 edx-sga-0.9.0/edx_sga/static/js/bower/URIjs/bower.json
+-rw-------   0 u56791   (56791) dyno     (56791)     1077 2019-10-01 15:39:23.000000 edx-sga-0.9.0/edx_sga/static/js/bower/URIjs/LICENSE.txt
+-rw-------   0 u56791   (56791) dyno     (56791)    35696 2019-10-01 15:39:23.000000 edx-sga-0.9.0/edx_sga/static/js/bower/URIjs/README.md
+-rw-------   0 u56791   (56791) dyno     (56791)      524 2019-10-01 15:39:23.000000 edx-sga-0.9.0/edx_sga/static/js/bower/URIjs/.bower.json
+drwx------   0 u56791   (56791) dyno     (56791)        0 2019-10-01 15:39:33.000000 edx-sga-0.9.0/edx_sga/static/js/bower/jquery/
+drwx------   0 u56791   (56791) dyno     (56791)        0 2019-10-01 15:39:33.000000 edx-sga-0.9.0/edx_sga/static/js/bower/jquery/src/
+drwx------   0 u56791   (56791) dyno     (56791)        0 2019-10-01 15:39:33.000000 edx-sga-0.9.0/edx_sga/static/js/bower/jquery/src/manipulation/
+-rw-------   0 u56791   (56791) dyno     (56791)      240 2019-10-01 15:39:23.000000 edx-sga-0.9.0/edx_sga/static/js/bower/jquery/src/manipulation/_evalUrl.js
+-rw-------   0 u56791   (56791) dyno     (56791)      975 2019-10-01 15:39:23.000000 edx-sga-0.9.0/edx_sga/static/js/bower/jquery/src/manipulation/support.js
+drwx------   0 u56791   (56791) dyno     (56791)        0 2019-10-01 15:39:33.000000 edx-sga-0.9.0/edx_sga/static/js/bower/jquery/src/manipulation/var/
+-rw-------   0 u56791   (56791) dyno     (56791)       59 2019-10-01 15:39:23.000000 edx-sga-0.9.0/edx_sga/static/js/bower/jquery/src/manipulation/var/rcheckableType.js
+-rw-------   0 u56791   (56791) dyno     (56791)    24475 2019-10-01 15:39:23.000000 edx-sga-0.9.0/edx_sga/static/js/bower/jquery/src/event.js
+-rw-------   0 u56791   (56791) dyno     (56791)      223 2019-10-01 15:39:23.000000 edx-sga-0.9.0/edx_sga/static/js/bower/jquery/src/deprecated.js
+-rw-------   0 u56791   (56791) dyno     (56791)       33 2019-10-01 15:39:23.000000 edx-sga-0.9.0/edx_sga/static/js/bower/jquery/src/selector.js
+-rw-------   0 u56791   (56791) dyno     (56791)     5588 2019-10-01 15:39:23.000000 edx-sga-0.9.0/edx_sga/static/js/bower/jquery/src/offset.js
+-rw-------   0 u56791   (56791) dyno     (56791)    15039 2019-10-01 15:39:23.000000 edx-sga-0.9.0/edx_sga/static/js/bower/jquery/src/manipulation.js
+-rw-------   0 u56791   (56791) dyno     (56791)     1496 2019-10-01 15:39:23.000000 edx-sga-0.9.0/edx_sga/static/js/bower/jquery/src/wrap.js
+-rw-------   0 u56791   (56791) dyno     (56791)    12346 2019-10-01 15:39:23.000000 edx-sga-0.9.0/edx_sga/static/js/bower/jquery/src/css.js
+-rw-------   0 u56791   (56791) dyno     (56791)     1393 2019-10-01 15:39:23.000000 edx-sga-0.9.0/edx_sga/static/js/bower/jquery/src/intro.js
+drwx------   0 u56791   (56791) dyno     (56791)        0 2019-10-01 15:39:33.000000 edx-sga-0.9.0/edx_sga/static/js/bower/jquery/src/exports/
+-rw-------   0 u56791   (56791) dyno     (56791)      641 2019-10-01 15:39:23.000000 edx-sga-0.9.0/edx_sga/static/js/bower/jquery/src/exports/global.js
+-rw-------   0 u56791   (56791) dyno     (56791)     1006 2019-10-01 15:39:23.000000 edx-sga-0.9.0/edx_sga/static/js/bower/jquery/src/exports/amd.js
+drwx------   0 u56791   (56791) dyno     (56791)        0 2019-10-01 15:39:33.000000 edx-sga-0.9.0/edx_sga/static/js/bower/jquery/src/queue/
+-rw-------   0 u56791   (56791) dyno     (56791)      561 2019-10-01 15:39:23.000000 edx-sga-0.9.0/edx_sga/static/js/bower/jquery/src/queue/delay.js
+-rw-------   0 u56791   (56791) dyno     (56791)    16914 2019-10-01 15:39:23.000000 edx-sga-0.9.0/edx_sga/static/js/bower/jquery/src/effects.js
+-rw-------   0 u56791   (56791) dyno     (56791)      574 2019-10-01 15:39:23.000000 edx-sga-0.9.0/edx_sga/static/js/bower/jquery/src/jquery.js
+drwx------   0 u56791   (56791) dyno     (56791)        0 2019-10-01 15:39:33.000000 edx-sga-0.9.0/edx_sga/static/js/bower/jquery/src/var/
+-rw-------   0 u56791   (56791) dyno     (56791)       64 2019-10-01 15:39:23.000000 edx-sga-0.9.0/edx_sga/static/js/bower/jquery/src/var/class2type.js
+-rw-------   0 u56791   (56791) dyno     (56791)       63 2019-10-01 15:39:23.000000 edx-sga-0.9.0/edx_sga/static/js/bower/jquery/src/var/concat.js
+-rw-------   0 u56791   (56791) dyno     (56791)       36 2019-10-01 15:39:23.000000 edx-sga-0.9.0/edx_sga/static/js/bower/jquery/src/var/arr.js
+-rw-------   0 u56791   (56791) dyno     (56791)       42 2019-10-01 15:39:23.000000 edx-sga-0.9.0/edx_sga/static/js/bower/jquery/src/var/rnotwhite.js
+-rw-------   0 u56791   (56791) dyno     (56791)       64 2019-10-01 15:39:23.000000 edx-sga-0.9.0/edx_sga/static/js/bower/jquery/src/var/indexOf.js
+-rw-------   0 u56791   (56791) dyno     (56791)       99 2019-10-01 15:39:23.000000 edx-sga-0.9.0/edx_sga/static/js/bower/jquery/src/var/support.js
+-rw-------   0 u56791   (56791) dyno     (56791)       80 2019-10-01 15:39:23.000000 edx-sga-0.9.0/edx_sga/static/js/bower/jquery/src/var/pnum.js
+-rw-------   0 u56791   (56791) dyno     (56791)       61 2019-10-01 15:39:23.000000 edx-sga-0.9.0/edx_sga/static/js/bower/jquery/src/var/push.js
+-rw-------   0 u56791   (56791) dyno     (56791)       62 2019-10-01 15:39:23.000000 edx-sga-0.9.0/edx_sga/static/js/bower/jquery/src/var/slice.js
+-rw-------   0 u56791   (56791) dyno     (56791)       92 2019-10-01 15:39:23.000000 edx-sga-0.9.0/edx_sga/static/js/bower/jquery/src/var/hasOwn.js
+-rw-------   0 u56791   (56791) dyno     (56791)       86 2019-10-01 15:39:23.000000 edx-sga-0.9.0/edx_sga/static/js/bower/jquery/src/var/toString.js
+-rw-------   0 u56791   (56791) dyno     (56791)       50 2019-10-01 15:39:23.000000 edx-sga-0.9.0/edx_sga/static/js/bower/jquery/src/var/strundefined.js
+-rw-------   0 u56791   (56791) dyno     (56791)     3063 2019-10-01 15:39:23.000000 edx-sga-0.9.0/edx_sga/static/js/bower/jquery/src/queue.js
+drwx------   0 u56791   (56791) dyno     (56791)        0 2019-10-01 15:39:33.000000 edx-sga-0.9.0/edx_sga/static/js/bower/jquery/src/effects/
+-rw-------   0 u56791   (56791) dyno     (56791)      225 2019-10-01 15:39:23.000000 edx-sga-0.9.0/edx_sga/static/js/bower/jquery/src/effects/animatedSelector.js
+-rw-------   0 u56791   (56791) dyno     (56791)     3028 2019-10-01 15:39:23.000000 edx-sga-0.9.0/edx_sga/static/js/bower/jquery/src/effects/Tween.js
+-rw-------   0 u56791   (56791) dyno     (56791)     4414 2019-10-01 15:39:23.000000 edx-sga-0.9.0/edx_sga/static/js/bower/jquery/src/deferred.js
+-rw-------   0 u56791   (56791) dyno     (56791)     4535 2019-10-01 15:39:23.000000 edx-sga-0.9.0/edx_sga/static/js/bower/jquery/src/traversing.js
+-rw-------   0 u56791   (56791) dyno     (56791)     3214 2019-10-01 15:39:23.000000 edx-sga-0.9.0/edx_sga/static/js/bower/jquery/src/serialize.js
+-rw-------   0 u56791   (56791) dyno     (56791)     1776 2019-10-01 15:39:23.000000 edx-sga-0.9.0/edx_sga/static/js/bower/jquery/src/dimensions.js
+drwx------   0 u56791   (56791) dyno     (56791)        0 2019-10-01 15:39:33.000000 edx-sga-0.9.0/edx_sga/static/js/bower/jquery/src/attributes/
+-rw-------   0 u56791   (56791) dyno     (56791)     4155 2019-10-01 15:39:23.000000 edx-sga-0.9.0/edx_sga/static/js/bower/jquery/src/attributes/classes.js
+-rw-------   0 u56791   (56791) dyno     (56791)      893 2019-10-01 15:39:23.000000 edx-sga-0.9.0/edx_sga/static/js/bower/jquery/src/attributes/support.js
+-rw-------   0 u56791   (56791) dyno     (56791)     1854 2019-10-01 15:39:23.000000 edx-sga-0.9.0/edx_sga/static/js/bower/jquery/src/attributes/prop.js
+-rw-------   0 u56791   (56791) dyno     (56791)     3320 2019-10-01 15:39:23.000000 edx-sga-0.9.0/edx_sga/static/js/bower/jquery/src/attributes/attr.js
+-rw-------   0 u56791   (56791) dyno     (56791)     3839 2019-10-01 15:39:23.000000 edx-sga-0.9.0/edx_sga/static/js/bower/jquery/src/attributes/val.js
+-rw-------   0 u56791   (56791) dyno     (56791)     4434 2019-10-01 15:39:23.000000 edx-sga-0.9.0/edx_sga/static/js/bower/jquery/src/selector-native.js
+drwx------   0 u56791   (56791) dyno     (56791)        0 2019-10-01 15:39:33.000000 edx-sga-0.9.0/edx_sga/static/js/bower/jquery/src/event/
+-rw-------   0 u56791   (56791) dyno     (56791)      123 2019-10-01 15:39:23.000000 edx-sga-0.9.0/edx_sga/static/js/bower/jquery/src/event/support.js
+-rw-------   0 u56791   (56791) dyno     (56791)     1094 2019-10-01 15:39:23.000000 edx-sga-0.9.0/edx_sga/static/js/bower/jquery/src/event/alias.js
+-rw-------   0 u56791   (56791) dyno     (56791)      322 2019-10-01 15:39:23.000000 edx-sga-0.9.0/edx_sga/static/js/bower/jquery/src/event/ajax.js
+drwx------   0 u56791   (56791) dyno     (56791)        0 2019-10-01 15:39:33.000000 edx-sga-0.9.0/edx_sga/static/js/bower/jquery/src/data/
+-rw-------   0 u56791   (56791) dyno     (56791)      383 2019-10-01 15:39:23.000000 edx-sga-0.9.0/edx_sga/static/js/bower/jquery/src/data/accepts.js
+drwx------   0 u56791   (56791) dyno     (56791)        0 2019-10-01 15:39:33.000000 edx-sga-0.9.0/edx_sga/static/js/bower/jquery/src/data/var/
+-rw-------   0 u56791   (56791) dyno     (56791)       66 2019-10-01 15:39:23.000000 edx-sga-0.9.0/edx_sga/static/js/bower/jquery/src/data/var/data_user.js
+-rw-------   0 u56791   (56791) dyno     (56791)       66 2019-10-01 15:39:23.000000 edx-sga-0.9.0/edx_sga/static/js/bower/jquery/src/data/var/data_priv.js
+-rw-------   0 u56791   (56791) dyno     (56791)     4882 2019-10-01 15:39:23.000000 edx-sga-0.9.0/edx_sga/static/js/bower/jquery/src/data/Data.js
+-rw-------   0 u56791   (56791) dyno     (56791)      200 2019-10-01 15:39:23.000000 edx-sga-0.9.0/edx_sga/static/js/bower/jquery/src/attributes.js
+drwx------   0 u56791   (56791) dyno     (56791)        0 2019-10-01 15:39:33.000000 edx-sga-0.9.0/edx_sga/static/js/bower/jquery/src/traversing/
+-rw-------   0 u56791   (56791) dyno     (56791)     2464 2019-10-01 15:39:23.000000 edx-sga-0.9.0/edx_sga/static/js/bower/jquery/src/traversing/findFilter.js
+drwx------   0 u56791   (56791) dyno     (56791)        0 2019-10-01 15:39:33.000000 edx-sga-0.9.0/edx_sga/static/js/bower/jquery/src/traversing/var/
+-rw-------   0 u56791   (56791) dyno     (56791)      110 2019-10-01 15:39:23.000000 edx-sga-0.9.0/edx_sga/static/js/bower/jquery/src/traversing/var/rneedsContext.js
+drwx------   0 u56791   (56791) dyno     (56791)        0 2019-10-01 15:39:33.000000 edx-sga-0.9.0/edx_sga/static/js/bower/jquery/src/ajax/
+-rw-------   0 u56791   (56791) dyno     (56791)     1271 2019-10-01 15:39:23.000000 edx-sga-0.9.0/edx_sga/static/js/bower/jquery/src/ajax/script.js
+-rw-------   0 u56791   (56791) dyno     (56791)     3488 2019-10-01 15:39:23.000000 edx-sga-0.9.0/edx_sga/static/js/bower/jquery/src/ajax/xhr.js
+-rw-------   0 u56791   (56791) dyno     (56791)      485 2019-10-01 15:39:23.000000 edx-sga-0.9.0/edx_sga/static/js/bower/jquery/src/ajax/parseXML.js
+drwx------   0 u56791   (56791) dyno     (56791)        0 2019-10-01 15:39:33.000000 edx-sga-0.9.0/edx_sga/static/js/bower/jquery/src/ajax/var/
+-rw-------   0 u56791   (56791) dyno     (56791)       40 2019-10-01 15:39:23.000000 edx-sga-0.9.0/edx_sga/static/js/bower/jquery/src/ajax/var/rquery.js
+-rw-------   0 u56791   (56791) dyno     (56791)       73 2019-10-01 15:39:23.000000 edx-sga-0.9.0/edx_sga/static/js/bower/jquery/src/ajax/var/nonce.js
+-rw-------   0 u56791   (56791) dyno     (56791)     2516 2019-10-01 15:39:23.000000 edx-sga-0.9.0/edx_sga/static/js/bower/jquery/src/ajax/jsonp.js
+-rw-------   0 u56791   (56791) dyno     (56791)     1669 2019-10-01 15:39:23.000000 edx-sga-0.9.0/edx_sga/static/js/bower/jquery/src/ajax/load.js
+-rw-------   0 u56791   (56791) dyno     (56791)      222 2019-10-01 15:39:23.000000 edx-sga-0.9.0/edx_sga/static/js/bower/jquery/src/ajax/parseJSON.js
+-rw-------   0 u56791   (56791) dyno     (56791)      294 2019-10-01 15:39:23.000000 edx-sga-0.9.0/edx_sga/static/js/bower/jquery/src/selector-sizzle.js
+drwx------   0 u56791   (56791) dyno     (56791)        0 2019-10-01 15:39:33.000000 edx-sga-0.9.0/edx_sga/static/js/bower/jquery/src/core/
+drwx------   0 u56791   (56791) dyno     (56791)        0 2019-10-01 15:39:33.000000 edx-sga-0.9.0/edx_sga/static/js/bower/jquery/src/core/var/
+-rw-------   0 u56791   (56791) dyno     (56791)       91 2019-10-01 15:39:23.000000 edx-sga-0.9.0/edx_sga/static/js/bower/jquery/src/core/var/rsingleTag.js
+-rw-------   0 u56791   (56791) dyno     (56791)     2381 2019-10-01 15:39:23.000000 edx-sga-0.9.0/edx_sga/static/js/bower/jquery/src/core/ready.js
+-rw-------   0 u56791   (56791) dyno     (56791)      938 2019-10-01 15:39:23.000000 edx-sga-0.9.0/edx_sga/static/js/bower/jquery/src/core/parseHTML.js
+-rw-------   0 u56791   (56791) dyno     (56791)     3401 2019-10-01 15:39:23.000000 edx-sga-0.9.0/edx_sga/static/js/bower/jquery/src/core/init.js
+-rw-------   0 u56791   (56791) dyno     (56791)     1210 2019-10-01 15:39:23.000000 edx-sga-0.9.0/edx_sga/static/js/bower/jquery/src/core/access.js
+-rw-------   0 u56791   (56791) dyno     (56791)    11790 2019-10-01 15:39:23.000000 edx-sga-0.9.0/edx_sga/static/js/bower/jquery/src/core.js
+-rw-------   0 u56791   (56791) dyno     (56791)    21168 2019-10-01 15:39:23.000000 edx-sga-0.9.0/edx_sga/static/js/bower/jquery/src/ajax.js
+-rw-------   0 u56791   (56791) dyno     (56791)        5 2019-10-01 15:39:23.000000 edx-sga-0.9.0/edx_sga/static/js/bower/jquery/src/outro.js
+-rw-------   0 u56791   (56791) dyno     (56791)     4942 2019-10-01 15:39:23.000000 edx-sga-0.9.0/edx_sga/static/js/bower/jquery/src/data.js
+drwx------   0 u56791   (56791) dyno     (56791)        0 2019-10-01 15:39:33.000000 edx-sga-0.9.0/edx_sga/static/js/bower/jquery/src/css/
+-rw-------   0 u56791   (56791) dyno     (56791)     1452 2019-10-01 15:39:23.000000 edx-sga-0.9.0/edx_sga/static/js/bower/jquery/src/css/curCSS.js
+-rw-------   0 u56791   (56791) dyno     (56791)     1867 2019-10-01 15:39:23.000000 edx-sga-0.9.0/edx_sga/static/js/bower/jquery/src/css/defaultDisplay.js
+-rw-------   0 u56791   (56791) dyno     (56791)     3198 2019-10-01 15:39:23.000000 edx-sga-0.9.0/edx_sga/static/js/bower/jquery/src/css/support.js
+drwx------   0 u56791   (56791) dyno     (56791)        0 2019-10-01 15:39:33.000000 edx-sga-0.9.0/edx_sga/static/js/bower/jquery/src/css/var/
+-rw-------   0 u56791   (56791) dyno     (56791)      355 2019-10-01 15:39:23.000000 edx-sga-0.9.0/edx_sga/static/js/bower/jquery/src/css/var/isHidden.js
+-rw-------   0 u56791   (56791) dyno     (56791)       70 2019-10-01 15:39:23.000000 edx-sga-0.9.0/edx_sga/static/js/bower/jquery/src/css/var/cssExpand.js
+-rw-------   0 u56791   (56791) dyno     (56791)       45 2019-10-01 15:39:23.000000 edx-sga-0.9.0/edx_sga/static/js/bower/jquery/src/css/var/rmargin.js
+-rw-------   0 u56791   (56791) dyno     (56791)      113 2019-10-01 15:39:23.000000 edx-sga-0.9.0/edx_sga/static/js/bower/jquery/src/css/var/rnumnonpx.js
+-rw-------   0 u56791   (56791) dyno     (56791)      410 2019-10-01 15:39:23.000000 edx-sga-0.9.0/edx_sga/static/js/bower/jquery/src/css/var/getStyles.js
+-rw-------   0 u56791   (56791) dyno     (56791)      555 2019-10-01 15:39:23.000000 edx-sga-0.9.0/edx_sga/static/js/bower/jquery/src/css/swap.js
+-rw-------   0 u56791   (56791) dyno     (56791)      380 2019-10-01 15:39:23.000000 edx-sga-0.9.0/edx_sga/static/js/bower/jquery/src/css/hiddenVisibleSelectors.js
+-rw-------   0 u56791   (56791) dyno     (56791)      509 2019-10-01 15:39:23.000000 edx-sga-0.9.0/edx_sga/static/js/bower/jquery/src/css/addGetHookIf.js
+-rw-------   0 u56791   (56791) dyno     (56791)     5506 2019-10-01 15:39:23.000000 edx-sga-0.9.0/edx_sga/static/js/bower/jquery/src/callbacks.js
+-rw-------   0 u56791   (56791) dyno     (56791)     1099 2019-10-01 15:39:23.000000 edx-sga-0.9.0/edx_sga/static/js/bower/jquery/MIT-LICENSE.txt
+-rw-------   0 u56791   (56791) dyno     (56791)      451 2019-10-01 15:39:23.000000 edx-sga-0.9.0/edx_sga/static/js/bower/jquery/bower.json
+-rw-------   0 u56791   (56791) dyno     (56791)      752 2019-10-01 15:39:23.000000 edx-sga-0.9.0/edx_sga/static/js/bower/jquery/.bower.json
+drwx------   0 u56791   (56791) dyno     (56791)        0 2019-10-01 15:39:33.000000 edx-sga-0.9.0/edx_sga/static/js/bower/requirejs/
+-rw-------   0 u56791   (56791) dyno     (56791)    84263 2019-10-01 15:39:23.000000 edx-sga-0.9.0/edx_sga/static/js/bower/requirejs/require.js
+-rw-------   0 u56791   (56791) dyno     (56791)      306 2019-10-01 15:39:23.000000 edx-sga-0.9.0/edx_sga/static/js/bower/requirejs/bower.json
+-rw-------   0 u56791   (56791) dyno     (56791)       75 2019-10-01 15:39:23.000000 edx-sga-0.9.0/edx_sga/static/js/bower/requirejs/README.md
+-rw-------   0 u56791   (56791) dyno     (56791)      592 2019-10-01 15:39:23.000000 edx-sga-0.9.0/edx_sga/static/js/bower/requirejs/.bower.json
+drwx------   0 u56791   (56791) dyno     (56791)        0 2019-10-01 15:39:33.000000 edx-sga-0.9.0/edx_sga/static/js/bower/sinon/
+-rwx------   0 u56791   (56791) dyno     (56791)      438 2019-10-01 15:39:23.000000 edx-sga-0.9.0/edx_sga/static/js/bower/sinon/release.sh
+-rw-------   0 u56791   (56791) dyno     (56791)       27 2019-10-01 15:39:23.000000 edx-sga-0.9.0/edx_sga/static/js/bower/sinon/.gitignore
+-rw-------   0 u56791   (56791) dyno     (56791)     1572 2019-10-01 15:39:23.000000 edx-sga-0.9.0/edx_sga/static/js/bower/sinon/LICENSE
+-rw-------   0 u56791   (56791) dyno     (56791)      382 2019-10-01 15:39:23.000000 edx-sga-0.9.0/edx_sga/static/js/bower/sinon/.editorconfig
+-rw-------   0 u56791   (56791) dyno     (56791)     1211 2019-10-01 15:39:23.000000 edx-sga-0.9.0/edx_sga/static/js/bower/sinon/package.json
+drwx------   0 u56791   (56791) dyno     (56791)        0 2019-10-01 15:39:33.000000 edx-sga-0.9.0/edx_sga/static/js/bower/sinon/scripts/
+-rwx------   0 u56791   (56791) dyno     (56791)      768 2019-10-01 15:39:23.000000 edx-sga-0.9.0/edx_sga/static/js/bower/sinon/scripts/ci-test.sh
+-rwx------   0 u56791   (56791) dyno     (56791)      231 2019-10-01 15:39:23.000000 edx-sga-0.9.0/edx_sga/static/js/bower/sinon/scripts/eslint-pre-commit
+drwx------   0 u56791   (56791) dyno     (56791)        0 2019-10-01 15:39:33.000000 edx-sga-0.9.0/edx_sga/static/js/bower/sinon/test/
+-rw-------   0 u56791   (56791) dyno     (56791)      896 2019-10-01 15:39:23.000000 edx-sga-0.9.0/edx_sga/static/js/bower/sinon/test/buster.js
+-rw-------   0 u56791   (56791) dyno     (56791)    22374 2019-10-01 15:39:23.000000 edx-sga-0.9.0/edx_sga/static/js/bower/sinon/test/match-test.js
+-rw-------   0 u56791   (56791) dyno     (56791)    69039 2019-10-01 15:39:23.000000 edx-sga-0.9.0/edx_sga/static/js/bower/sinon/test/spy-test.js
+-rw-------   0 u56791   (56791) dyno     (56791)    18694 2019-10-01 15:39:23.000000 edx-sga-0.9.0/edx_sga/static/js/bower/sinon/test/test-test.js
+-rw-------   0 u56791   (56791) dyno     (56791)     1807 2019-10-01 15:39:23.000000 edx-sga-0.9.0/edx_sga/static/js/bower/sinon/test/extend-test.js
+-rw-------   0 u56791   (56791) dyno     (56791)     7641 2019-10-01 15:39:23.000000 edx-sga-0.9.0/edx_sga/static/js/bower/sinon/test/test-case-test.js
+-rw-------   0 u56791   (56791) dyno     (56791)     1346 2019-10-01 15:39:23.000000 edx-sga-0.9.0/edx_sga/static/js/bower/sinon/test/typeOf-test.js
+-rw-------   0 u56791   (56791) dyno     (56791)    24007 2019-10-01 15:39:23.000000 edx-sga-0.9.0/edx_sga/static/js/bower/sinon/test/sinon-test.js
+-rw-------   0 u56791   (56791) dyno     (56791)      313 2019-10-01 15:39:23.000000 edx-sga-0.9.0/edx_sga/static/js/bower/sinon/test/buster-packaged.js
+-rw-------   0 u56791   (56791) dyno     (56791)    58120 2019-10-01 15:39:23.000000 edx-sga-0.9.0/edx_sga/static/js/bower/sinon/test/stub-test.js
+-rw-------   0 u56791   (56791) dyno     (56791)    34009 2019-10-01 15:39:23.000000 edx-sga-0.9.0/edx_sga/static/js/bower/sinon/test/mock-test.js
+-rw-------   0 u56791   (56791) dyno     (56791)    53776 2019-10-01 15:39:23.000000 edx-sga-0.9.0/edx_sga/static/js/bower/sinon/test/assert-test.js
+drwx------   0 u56791   (56791) dyno     (56791)        0 2019-10-01 15:39:33.000000 edx-sga-0.9.0/edx_sga/static/js/bower/sinon/test/util/
+-rw-------   0 u56791   (56791) dyno     (56791)    58912 2019-10-01 15:39:23.000000 edx-sga-0.9.0/edx_sga/static/js/bower/sinon/test/util/fake-xml-http-request-test.js
+-rw-------   0 u56791   (56791) dyno     (56791)     4643 2019-10-01 15:39:23.000000 edx-sga-0.9.0/edx_sga/static/js/bower/sinon/test/util/event-test.js
+-rw-------   0 u56791   (56791) dyno     (56791)    36722 2019-10-01 15:39:23.000000 edx-sga-0.9.0/edx_sga/static/js/bower/sinon/test/util/fake-timers-test.js
+-rw-------   0 u56791   (56791) dyno     (56791)     7532 2019-10-01 15:39:23.000000 edx-sga-0.9.0/edx_sga/static/js/bower/sinon/test/util/fake-server-with-clock-test.js
+-rw-------   0 u56791   (56791) dyno     (56791)    14734 2019-10-01 15:39:23.000000 edx-sga-0.9.0/edx_sga/static/js/bower/sinon/test/util/fake-xdomain-request-test.js
+-rw-------   0 u56791   (56791) dyno     (56791)    31795 2019-10-01 15:39:23.000000 edx-sga-0.9.0/edx_sga/static/js/bower/sinon/test/util/fake-server-test.js
+-rw-------   0 u56791   (56791) dyno     (56791)     1350 2019-10-01 15:39:23.000000 edx-sga-0.9.0/edx_sga/static/js/bower/sinon/test/times-in-words-test.js
+-rw-------   0 u56791   (56791) dyno     (56791)     2247 2019-10-01 15:39:23.000000 edx-sga-0.9.0/edx_sga/static/js/bower/sinon/test/log-error-test.js
+drwx------   0 u56791   (56791) dyno     (56791)        0 2019-10-01 15:39:33.000000 edx-sga-0.9.0/edx_sga/static/js/bower/sinon/test/issues/
+-rw-------   0 u56791   (56791) dyno     (56791)     2971 2019-10-01 15:39:23.000000 edx-sga-0.9.0/edx_sga/static/js/bower/sinon/test/issues/issues-test.js
+-rw-------   0 u56791   (56791) dyno     (56791)      841 2019-10-01 15:39:23.000000 edx-sga-0.9.0/edx_sga/static/js/bower/sinon/test/format-test.js
+-rw-------   0 u56791   (56791) dyno     (56791)    16139 2019-10-01 15:39:23.000000 edx-sga-0.9.0/edx_sga/static/js/bower/sinon/test/sandbox-test.js
+-rw-------   0 u56791   (56791) dyno     (56791)     1537 2019-10-01 15:39:23.000000 edx-sga-0.9.0/edx_sga/static/js/bower/sinon/test/test-helper.js
+-rw-------   0 u56791   (56791) dyno     (56791)      347 2019-10-01 15:39:23.000000 edx-sga-0.9.0/edx_sga/static/js/bower/sinon/test/hello-world-test.js
+-rw-------   0 u56791   (56791) dyno     (56791)    11924 2019-10-01 15:39:23.000000 edx-sga-0.9.0/edx_sga/static/js/bower/sinon/test/collection-test.js
+-rw-------   0 u56791   (56791) dyno     (56791)    42564 2019-10-01 15:39:23.000000 edx-sga-0.9.0/edx_sga/static/js/bower/sinon/test/call-test.js
+-rw-------   0 u56791   (56791) dyno     (56791)     1869 2019-10-01 15:39:23.000000 edx-sga-0.9.0/edx_sga/static/js/bower/sinon/README.md
+-rw-------   0 u56791   (56791) dyno     (56791)     6124 2019-10-01 15:39:23.000000 edx-sga-0.9.0/edx_sga/static/js/bower/sinon/.eslintrc
+-rw-------   0 u56791   (56791) dyno     (56791)      314 2019-10-01 15:39:23.000000 edx-sga-0.9.0/edx_sga/static/js/bower/sinon/.jscsrc
+-rw-------   0 u56791   (56791) dyno     (56791)     4033 2019-10-01 15:39:23.000000 edx-sga-0.9.0/edx_sga/static/js/bower/sinon/AUTHORS
+-rwx------   0 u56791   (56791) dyno     (56791)     4310 2019-10-01 15:39:23.000000 edx-sga-0.9.0/edx_sga/static/js/bower/sinon/build
+-rw-------   0 u56791   (56791) dyno     (56791)      744 2019-10-01 15:39:23.000000 edx-sga-0.9.0/edx_sga/static/js/bower/sinon/RELEASE.md
+-rw-------   0 u56791   (56791) dyno     (56791)    23129 2019-10-01 15:39:23.000000 edx-sga-0.9.0/edx_sga/static/js/bower/sinon/Changelog.txt
+-rw-------   0 u56791   (56791) dyno     (56791)       15 2019-10-01 15:39:23.000000 edx-sga-0.9.0/edx_sga/static/js/bower/sinon/.eslintignore
+-rw-------   0 u56791   (56791) dyno     (56791)      876 2019-10-01 15:39:23.000000 edx-sga-0.9.0/edx_sga/static/js/bower/sinon/.travis.yml
+-rw-------   0 u56791   (56791) dyno     (56791)      378 2019-10-01 15:39:23.000000 edx-sga-0.9.0/edx_sga/static/js/bower/sinon/.bower.json
+-rw-------   0 u56791   (56791) dyno     (56791)     5364 2019-10-01 15:39:23.000000 edx-sga-0.9.0/edx_sga/static/js/bower/sinon/CONTRIBUTING.md
+drwx------   0 u56791   (56791) dyno     (56791)        0 2019-10-01 15:39:33.000000 edx-sga-0.9.0/edx_sga/static/js/bower/sinon/lib/
+-rw-------   0 u56791   (56791) dyno     (56791)     1430 2019-10-01 15:39:23.000000 edx-sga-0.9.0/edx_sga/static/js/bower/sinon/lib/sinon.js
+drwx------   0 u56791   (56791) dyno     (56791)        0 2019-10-01 15:39:33.000000 edx-sga-0.9.0/edx_sga/static/js/bower/sinon/lib/sinon/
+-rw-------   0 u56791   (56791) dyno     (56791)     6121 2019-10-01 15:39:23.000000 edx-sga-0.9.0/edx_sga/static/js/bower/sinon/lib/sinon/stub.js
+-rw-------   0 u56791   (56791) dyno     (56791)     8682 2019-10-01 15:39:23.000000 edx-sga-0.9.0/edx_sga/static/js/bower/sinon/lib/sinon/match.js
+-rw-------   0 u56791   (56791) dyno     (56791)     7729 2019-10-01 15:39:23.000000 edx-sga-0.9.0/edx_sga/static/js/bower/sinon/lib/sinon/call.js
+-rw-------   0 u56791   (56791) dyno     (56791)     2804 2019-10-01 15:39:23.000000 edx-sga-0.9.0/edx_sga/static/js/bower/sinon/lib/sinon/test_case.js
+-rw-------   0 u56791   (56791) dyno     (56791)     8430 2019-10-01 15:39:23.000000 edx-sga-0.9.0/edx_sga/static/js/bower/sinon/lib/sinon/assert.js
+-rw-------   0 u56791   (56791) dyno     (56791)     1900 2019-10-01 15:39:23.000000 edx-sga-0.9.0/edx_sga/static/js/bower/sinon/lib/sinon/log_error.js
+-rw-------   0 u56791   (56791) dyno     (56791)    15868 2019-10-01 15:39:23.000000 edx-sga-0.9.0/edx_sga/static/js/bower/sinon/lib/sinon/spy.js
+-rw-------   0 u56791   (56791) dyno     (56791)     3209 2019-10-01 15:39:23.000000 edx-sga-0.9.0/edx_sga/static/js/bower/sinon/lib/sinon/test.js
+-rw-------   0 u56791   (56791) dyno     (56791)     1196 2019-10-01 15:39:23.000000 edx-sga-0.9.0/edx_sga/static/js/bower/sinon/lib/sinon/times_in_words.js
+-rw-------   0 u56791   (56791) dyno     (56791)     3443 2019-10-01 15:39:23.000000 edx-sga-0.9.0/edx_sga/static/js/bower/sinon/lib/sinon/extend.js
+drwx------   0 u56791   (56791) dyno     (56791)        0 2019-10-01 15:39:33.000000 edx-sga-0.9.0/edx_sga/static/js/bower/sinon/lib/sinon/util/
+-rw-------   0 u56791   (56791) dyno     (56791)     1989 2019-10-01 15:39:23.000000 edx-sga-0.9.0/edx_sga/static/js/bower/sinon/lib/sinon/util/fake_timers.js
+-rw-------   0 u56791   (56791) dyno     (56791)      714 2019-10-01 15:39:23.000000 edx-sga-0.9.0/edx_sga/static/js/bower/sinon/lib/sinon/util/xdr_ie.js
+-rw-------   0 u56791   (56791) dyno     (56791)     8238 2019-10-01 15:39:23.000000 edx-sga-0.9.0/edx_sga/static/js/bower/sinon/lib/sinon/util/fake_server.js
+-rw-------   0 u56791   (56791) dyno     (56791)     3690 2019-10-01 15:39:23.000000 edx-sga-0.9.0/edx_sga/static/js/bower/sinon/lib/sinon/util/event.js
+-rw-------   0 u56791   (56791) dyno     (56791)      837 2019-10-01 15:39:23.000000 edx-sga-0.9.0/edx_sga/static/js/bower/sinon/lib/sinon/util/xhr_ie.js
+-rw-------   0 u56791   (56791) dyno     (56791)     1292 2019-10-01 15:39:23.000000 edx-sga-0.9.0/edx_sga/static/js/bower/sinon/lib/sinon/util/timers_ie.js
+-rw-------   0 u56791   (56791) dyno     (56791)     7569 2019-10-01 15:39:23.000000 edx-sga-0.9.0/edx_sga/static/js/bower/sinon/lib/sinon/util/fake_xdomain_request.js
+-rw-------   0 u56791   (56791) dyno     (56791)    22473 2019-10-01 15:39:23.000000 edx-sga-0.9.0/edx_sga/static/js/bower/sinon/lib/sinon/util/fake_xml_http_request.js
+-rw-------   0 u56791   (56791) dyno     (56791)     3345 2019-10-01 15:39:23.000000 edx-sga-0.9.0/edx_sga/static/js/bower/sinon/lib/sinon/util/fake_server_with_clock.js
+-rw-------   0 u56791   (56791) dyno     (56791)    13439 2019-10-01 15:39:23.000000 edx-sga-0.9.0/edx_sga/static/js/bower/sinon/lib/sinon/util/core.js
+-rw-------   0 u56791   (56791) dyno     (56791)     4656 2019-10-01 15:39:23.000000 edx-sga-0.9.0/edx_sga/static/js/bower/sinon/lib/sinon/collection.js
+-rw-------   0 u56791   (56791) dyno     (56791)     1320 2019-10-01 15:39:23.000000 edx-sga-0.9.0/edx_sga/static/js/bower/sinon/lib/sinon/typeOf.js
+-rw-------   0 u56791   (56791) dyno     (56791)    15777 2019-10-01 15:39:23.000000 edx-sga-0.9.0/edx_sga/static/js/bower/sinon/lib/sinon/mock.js
+-rw-------   0 u56791   (56791) dyno     (56791)    11791 2019-10-01 15:39:23.000000 edx-sga-0.9.0/edx_sga/static/js/bower/sinon/lib/sinon/behavior.js
+-rw-------   0 u56791   (56791) dyno     (56791)     2549 2019-10-01 15:39:23.000000 edx-sga-0.9.0/edx_sga/static/js/bower/sinon/lib/sinon/format.js
+-rw-------   0 u56791   (56791) dyno     (56791)     5078 2019-10-01 15:39:23.000000 edx-sga-0.9.0/edx_sga/static/js/bower/sinon/lib/sinon/sandbox.js
+drwx------   0 u56791   (56791) dyno     (56791)        0 2019-10-01 15:39:33.000000 edx-sga-0.9.0/edx_sga/static/css/
+-rw-------   0 u56791   (56791) dyno     (56791)     2696 2019-10-01 15:39:23.000000 edx-sga-0.9.0/edx_sga/static/css/edx_sga.css
+-rw-------   0 u56791   (56791) dyno     (56791)      462 2019-10-01 15:39:23.000000 edx-sga-0.9.0/edx_sga/wsgi.py
+-rw-------   0 u56791   (56791) dyno     (56791)       71 2019-10-01 15:39:23.000000 edx-sga-0.9.0/edx_sga/__init__.py
+-rw-------   0 u56791   (56791) dyno     (56791)     3998 2019-10-01 15:39:23.000000 edx-sga-0.9.0/edx_sga/showanswer.py
+-rw-------   0 u56791   (56791) dyno     (56791)    38114 2019-10-01 15:39:23.000000 edx-sga-0.9.0/edx_sga/sga.py
+-rw-------   0 u56791   (56791) dyno     (56791)     1044 2019-10-01 15:39:23.000000 edx-sga-0.9.0/setup.py
+-rw-------   0 u56791   (56791) dyno     (56791)    12950 2019-10-01 15:39:23.000000 edx-sga-0.9.0/README.md
+-rw-------   0 u56791   (56791) dyno     (56791)      272 2019-10-01 15:39:33.000000 edx-sga-0.9.0/PKG-INFO
+drwx------   0 u56791   (56791) dyno     (56791)        0 2019-10-01 15:39:33.000000 edx-sga-0.9.0/edx_sga.egg-info/
+-rw-------   0 u56791   (56791) dyno     (56791)       63 2019-10-01 15:39:33.000000 edx-sga-0.9.0/edx_sga.egg-info/entry_points.txt
+-rw-------   0 u56791   (56791) dyno     (56791)    10767 2019-10-01 15:39:33.000000 edx-sga-0.9.0/edx_sga.egg-info/SOURCES.txt
+-rw-------   0 u56791   (56791) dyno     (56791)        1 2019-10-01 15:39:33.000000 edx-sga-0.9.0/edx_sga.egg-info/not-zip-safe
+-rw-------   0 u56791   (56791) dyno     (56791)       20 2019-10-01 15:39:33.000000 edx-sga-0.9.0/edx_sga.egg-info/requires.txt
+-rw-------   0 u56791   (56791) dyno     (56791)      272 2019-10-01 15:39:33.000000 edx-sga-0.9.0/edx_sga.egg-info/PKG-INFO
+-rw-------   0 u56791   (56791) dyno     (56791)        1 2019-10-01 15:39:33.000000 edx-sga-0.9.0/edx_sga.egg-info/dependency_links.txt
+-rw-------   0 u56791   (56791) dyno     (56791)        8 2019-10-01 15:39:33.000000 edx-sga-0.9.0/edx_sga.egg-info/top_level.txt
```

### Comparing `edx-sga-0.8.3/edx_sga/utils.py` & `edx-sga-0.9.0/edx_sga/utils.py`

 * *Files identical despite different names*

### Comparing `edx-sga-0.8.3/edx_sga/locale/fake2/LC_MESSAGES/django.po` & `edx-sga-0.9.0/edx_sga/locale/fake2/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `edx-sga-0.8.3/edx_sga/locale/fake2/LC_MESSAGES/djangojs.po` & `edx-sga-0.9.0/edx_sga/locale/fake2/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `edx-sga-0.8.3/edx_sga/locale/fake2/LC_MESSAGES/django.mo` & `edx-sga-0.9.0/edx_sga/locale/fake2/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `edx-sga-0.8.3/edx_sga/locale/fake2/LC_MESSAGES/djangojs.mo` & `edx-sga-0.9.0/edx_sga/locale/fake2/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `edx-sga-0.8.3/edx_sga/locale/config.yaml` & `edx-sga-0.9.0/edx_sga/locale/config.yaml`

 * *Files identical despite different names*

### Comparing `edx-sga-0.8.3/edx_sga/locale/rtl/LC_MESSAGES/django.po` & `edx-sga-0.9.0/edx_sga/locale/rtl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `edx-sga-0.8.3/edx_sga/locale/rtl/LC_MESSAGES/djangojs.po` & `edx-sga-0.9.0/edx_sga/locale/rtl/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `edx-sga-0.8.3/edx_sga/locale/rtl/LC_MESSAGES/django.mo` & `edx-sga-0.9.0/edx_sga/locale/rtl/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `edx-sga-0.8.3/edx_sga/locale/rtl/LC_MESSAGES/djangojs.mo` & `edx-sga-0.9.0/edx_sga/locale/rtl/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `edx-sga-0.8.3/edx_sga/locale/eo/LC_MESSAGES/django.po` & `edx-sga-0.9.0/edx_sga/locale/eo/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `edx-sga-0.8.3/edx_sga/locale/eo/LC_MESSAGES/djangojs.po` & `edx-sga-0.9.0/edx_sga/locale/eo/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `edx-sga-0.8.3/edx_sga/locale/eo/LC_MESSAGES/django.mo` & `edx-sga-0.9.0/edx_sga/locale/eo/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `edx-sga-0.8.3/edx_sga/locale/eo/LC_MESSAGES/djangojs.mo` & `edx-sga-0.9.0/edx_sga/locale/eo/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `edx-sga-0.8.3/edx_sga/locale/en/LC_MESSAGES/django.po` & `edx-sga-0.9.0/edx_sga/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `edx-sga-0.8.3/edx_sga/locale/en/LC_MESSAGES/djangojs.po` & `edx-sga-0.9.0/edx_sga/locale/en/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `edx-sga-0.8.3/edx_sga/sga.py` & `edx-sga-0.9.0/edx_sga/sga.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,25 +4,28 @@
 """
 import json
 import logging
 import mimetypes
 import os
 import urllib
 
+from contextlib import closing
+from zipfile import ZipFile
 import pkg_resources
 import pytz
-from courseware.models import StudentModule  # lint-amnesty, pylint: disable=import-error
+
+from lms.djangoapps.courseware.models import StudentModule  # lint-amnesty, pylint: disable=import-error
 from django.conf import settings  # lint-amnesty, pylint: disable=import-error
 from django.core.exceptions import PermissionDenied  # lint-amnesty, pylint: disable=import-error
 from django.core.files import File  # lint-amnesty, pylint: disable=import-error
 from django.core.files.storage import default_storage  # lint-amnesty, pylint: disable=import-error
 from django.template import Context, Template  # lint-amnesty, pylint: disable=import-error
 from django.utils.encoding import force_text  # pylint: disable=import-error
 from django.utils.timezone import now as django_now  # pylint: disable=import-error
-from django.utils.translation import ugettext_lazy as _  # pylint: disable=import-error
+from django.utils.translation import ugettext as _  # pylint: disable=import-error
 from safe_lxml import etree  # pylint: disable=import-error
 from student.models import user_by_anonymous_id  # lint-amnesty, pylint: disable=import-error
 from submissions import api as submissions_api  # lint-amnesty, pylint: disable=import-error
 from submissions.models import (
     Submission,
     StudentItem as SubmissionsStudent
 )  # lint-amnesty, pylint: disable=import-error
@@ -507,14 +510,19 @@
                     location,
                     user.username
                 )
                 # if last zip file is older the last submission then recreate task
                 if zip_file_time >= last_assignment_date:
                     zip_file_ready = True
 
+                # check if some one reset submission. If yes the recreate zip file
+                assignment_count = len(assignments)
+                if self.count_archive_files(user) != assignment_count:
+                    zip_file_ready = False
+
         if not zip_file_ready:
             log.info("Creating new zip file for block: %s for instructor: %s", location, user.username)
             zip_student_submissions.delay(
                 self.block_course_id,
                 self.block_id,
                 location,
                 user.username
@@ -968,14 +976,28 @@
             user.username,
             self.block_course_id,
             self.block_id,
             self.location
         )
         return True if default_storage.exists(zip_file_path) else False
 
+    def count_archive_files(self, user):
+        """
+        returns number of files archive in zip.
+        """
+        zip_file_path = get_zip_file_path(
+            user.username,
+            self.block_course_id,
+            self.block_id,
+            self.location
+        )
+        with default_storage.open(zip_file_path, 'rb') as zip_file:
+            with closing(ZipFile(zip_file)) as archive:
+                return len(archive.infolist())
+
     def get_real_user(self):
         """returns session user"""
         return self.runtime.get_real_user(self.xmodule_runtime.anonymous_student_id)
 
     def correctness_available(self):
         """
         For SGA is_correct just means the user submitted the problem, which we always know one way or the other
```

### Comparing `edx-sga-0.8.3/edx_sga/management/commands/sga_migrate_submissions.py` & `edx-sga-0.9.0/edx_sga/management/commands/sga_migrate_submissions.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 Django command which migrates existing SGA submissions for a course from all
 old SGA implementation before v0.4.0 to newer version that uses the
 'submissions' application.
 """
 import json
 
 from django.core.management.base import BaseCommand, CommandError  # lint-amnesty, pylint: disable=import-error
-from courseware.courses import get_course_by_id  # lint-amnesty, pylint: disable=import-error
-from courseware.models import StudentModule  # lint-amnesty, pylint: disable=import-error
+from lms.djangoapps.courseware.courses import get_course_by_id  # lint-amnesty, pylint: disable=import-error
+from lms.djangoapps.courseware.models import StudentModule  # lint-amnesty, pylint: disable=import-error
 from opaque_keys.edx.keys import CourseKey  # lint-amnesty, pylint: disable=import-error
 from student.models import anonymous_id_for_user  # lint-amnesty, pylint: disable=import-error
 from submissions import api as submissions_api  # lint-amnesty, pylint: disable=import-error
 from xmodule.modulestore.django import modulestore  # lint-amnesty, pylint: disable=import-error
 
 
 class Command(BaseCommand):
```

### Comparing `edx-sga-0.8.3/edx_sga/static/css/edx_sga.css` & `edx-sga-0.9.0/edx_sga/static/css/edx_sga.css`

 * *Files identical despite different names*

### Comparing `edx-sga-0.8.3/edx_sga/static/js/src/studio.js` & `edx-sga-0.9.0/edx_sga/static/js/src/studio.js`

 * *Files identical despite different names*

### Comparing `edx-sga-0.8.3/edx_sga/static/js/src/edx_sga.js` & `edx-sga-0.9.0/edx_sga/static/js/src/edx_sga.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -113,14 +113,17 @@
                         // The happy path, no errors
                         render(data.result);
                     }
                 }
             });
 
             updateChangeEvent(fileUpload);
+            if (state.error) {
+                $(content).find('p.error').focus();
+            }
         }
 
         function renderStaffGrading(data) {
             if (data.hasOwnProperty('error')) {
                 gradeFormError(data['error']);
             } else {
                 gradeFormError('');
@@ -246,14 +249,16 @@
             var row = $(this).parents("tr");
             var form = $(element).find("#enter-grade-form");
             $(element).find('#student-name').text(row.data('fullname'));
             form.find('#module_id-input').val(row.data('module_id'));
             form.find('#submission_id-input').val(row.data('submission_id'));
             form.find('#grade-input').val(row.data('score'));
             form.find('#comment-input').text(row.data('comment'));
+            form.find('#remove-grade').prop('disabled', false);
+            form.find('.ccx-enter-grade-spinner').hide();
             form.off('submit').on('submit', function(event) {
                 var max_score = row.parents('#grade-info').data('max_score');
                 var score = Number(form.find('#grade-input').val());
                 event.preventDefault();
                 if (!score) {
                     gradeFormError('<br/>' + gettext('Grade must be a number.'));
                 } else if (score !== parseInt(score)) {
@@ -262,26 +267,35 @@
                     gradeFormError('<br/>' + gettext('Grade must be positive.'));
                 } else if (score > max_score) {
                     gradeFormError('<br/>' + interpolate(gettext('Maximum score is %(max_score)s'), {
                         max_score: max_score
                     }, true));
                 } else {
                     // No errors
+                    form.find('.ccx-enter-grade-spinner').show();
                     $.post(enterGradeUrl, form.serialize())
-                        .success(renderStaffGrading);
+                        .success(renderStaffGrading)
+                        .fail(function() {
+                            form.find('.ccx-enter-grade-spinner').hide();
+                        });
                 }
             });
-            form.find('#remove-grade').on('click', function(event) {
+            form.find('#remove-grade').off('click').on('click', function(event) {
+                $(this).prop('disabled', true);
+                form.find('.ccx-enter-grade-spinner').show();
                 var url = removeGradeUrl + '?module_id=' +
                     row.data('module_id') + '&student_id=' +
                     row.data('student_id');
                 event.preventDefault();
                 if (row.data('score')) {
                     // if there is no grade then it is pointless to call api.
-                    $.get(url).success(renderStaffGrading);
+                    $.get(url).success(renderStaffGrading).fail(function() {
+                        $(this).prop('disabled', false);
+                        form.find('.ccx-enter-grade-spinner').hide();
+                    });
                 } else {
                     gradeFormError('<br/>' + gettext('No grade to remove.'));
                 }
             });
             form.find('#enter-grade-cancel').on('click', function() {
                 /* We're kind of stretching the limits of leanModal, here,
                  * by nesting modals one on top of the other.  One side effect
```

### Comparing `edx-sga-0.8.3/edx_sga/static/js/src/jquery.tablesorter.min.js` & `edx-sga-0.9.0/edx_sga/static/js/src/jquery.tablesorter.min.js`

 * *Files identical despite different names*

### Comparing `edx-sga-0.8.3/edx_sga/static/js/bower/underscore/README.md` & `edx-sga-0.9.0/edx_sga/static/js/bower/underscore/README.md`

 * *Files identical despite different names*

### Comparing `edx-sga-0.8.3/edx_sga/static/js/bower/underscore/underscore.js` & `edx-sga-0.9.0/edx_sga/static/js/bower/underscore/underscore.js`

 * *Files identical despite different names*

### Comparing `edx-sga-0.8.3/edx_sga/static/js/bower/underscore/.bower.json` & `edx-sga-0.9.0/edx_sga/static/js/bower/underscore/.bower.json`

 * *Files identical despite different names*

### Comparing `edx-sga-0.8.3/edx_sga/static/js/bower/underscore/underscore-min.map` & `edx-sga-0.9.0/edx_sga/static/js/bower/underscore/underscore-min.map`

 * *Files identical despite different names*

### Comparing `edx-sga-0.8.3/edx_sga/static/js/bower/underscore/underscore-min.js` & `edx-sga-0.9.0/edx_sga/static/js/bower/underscore/underscore-min.js`

 * *Files identical despite different names*

### Comparing `edx-sga-0.8.3/edx_sga/static/js/bower/underscore/LICENSE` & `edx-sga-0.9.0/edx_sga/static/js/bower/underscore/LICENSE`

 * *Files identical despite different names*

### Comparing `edx-sga-0.8.3/edx_sga/static/js/bower/sinon/lib/sinon/stub.js` & `edx-sga-0.9.0/edx_sga/static/js/bower/sinon/lib/sinon/stub.js`

 * *Files identical despite different names*

### Comparing `edx-sga-0.8.3/edx_sga/static/js/bower/sinon/lib/sinon/test.js` & `edx-sga-0.9.0/edx_sga/static/js/bower/sinon/lib/sinon/test.js`

 * *Files identical despite different names*

### Comparing `edx-sga-0.8.3/edx_sga/static/js/bower/sinon/lib/sinon/test_case.js` & `edx-sga-0.9.0/edx_sga/static/js/bower/sinon/lib/sinon/test_case.js`

 * *Files identical despite different names*

### Comparing `edx-sga-0.8.3/edx_sga/static/js/bower/sinon/lib/sinon/log_error.js` & `edx-sga-0.9.0/edx_sga/static/js/bower/sinon/lib/sinon/log_error.js`

 * *Files identical despite different names*

### Comparing `edx-sga-0.8.3/edx_sga/static/js/bower/sinon/lib/sinon/match.js` & `edx-sga-0.9.0/edx_sga/static/js/bower/sinon/lib/sinon/match.js`

 * *Files identical despite different names*

### Comparing `edx-sga-0.8.3/edx_sga/static/js/bower/sinon/lib/sinon/format.js` & `edx-sga-0.9.0/edx_sga/static/js/bower/sinon/lib/sinon/format.js`

 * *Files identical despite different names*

### Comparing `edx-sga-0.8.3/edx_sga/static/js/bower/sinon/lib/sinon/sandbox.js` & `edx-sga-0.9.0/edx_sga/static/js/bower/sinon/lib/sinon/sandbox.js`

 * *Files identical despite different names*

### Comparing `edx-sga-0.8.3/edx_sga/static/js/bower/sinon/lib/sinon/times_in_words.js` & `edx-sga-0.9.0/edx_sga/static/js/bower/sinon/lib/sinon/times_in_words.js`

 * *Files identical despite different names*

### Comparing `edx-sga-0.8.3/edx_sga/static/js/bower/sinon/lib/sinon/assert.js` & `edx-sga-0.9.0/edx_sga/static/js/bower/sinon/lib/sinon/assert.js`

 * *Files identical despite different names*

### Comparing `edx-sga-0.8.3/edx_sga/static/js/bower/sinon/lib/sinon/spy.js` & `edx-sga-0.9.0/edx_sga/static/js/bower/sinon/lib/sinon/spy.js`

 * *Files identical despite different names*

### Comparing `edx-sga-0.8.3/edx_sga/static/js/bower/sinon/lib/sinon/collection.js` & `edx-sga-0.9.0/edx_sga/static/js/bower/sinon/lib/sinon/collection.js`

 * *Files identical despite different names*

### Comparing `edx-sga-0.8.3/edx_sga/static/js/bower/sinon/lib/sinon/util/fake_xml_http_request.js` & `edx-sga-0.9.0/edx_sga/static/js/bower/sinon/lib/sinon/util/fake_xml_http_request.js`

 * *Files identical despite different names*

### Comparing `edx-sga-0.8.3/edx_sga/static/js/bower/sinon/lib/sinon/util/core.js` & `edx-sga-0.9.0/edx_sga/static/js/bower/sinon/lib/sinon/util/core.js`

 * *Files identical despite different names*

### Comparing `edx-sga-0.8.3/edx_sga/static/js/bower/sinon/lib/sinon/util/fake_server_with_clock.js` & `edx-sga-0.9.0/edx_sga/static/js/bower/sinon/lib/sinon/util/fake_server_with_clock.js`

 * *Files identical despite different names*

### Comparing `edx-sga-0.8.3/edx_sga/static/js/bower/sinon/lib/sinon/util/fake_timers.js` & `edx-sga-0.9.0/edx_sga/static/js/bower/sinon/lib/sinon/util/fake_timers.js`

 * *Files identical despite different names*

### Comparing `edx-sga-0.8.3/edx_sga/static/js/bower/sinon/lib/sinon/util/fake_xdomain_request.js` & `edx-sga-0.9.0/edx_sga/static/js/bower/sinon/lib/sinon/util/fake_xdomain_request.js`

 * *Files identical despite different names*

### Comparing `edx-sga-0.8.3/edx_sga/static/js/bower/sinon/lib/sinon/util/fake_server.js` & `edx-sga-0.9.0/edx_sga/static/js/bower/sinon/lib/sinon/util/fake_server.js`

 * *Files identical despite different names*

### Comparing `edx-sga-0.8.3/edx_sga/static/js/bower/sinon/lib/sinon/util/xdr_ie.js` & `edx-sga-0.9.0/edx_sga/static/js/bower/sinon/lib/sinon/util/xdr_ie.js`

 * *Files identical despite different names*

### Comparing `edx-sga-0.8.3/edx_sga/static/js/bower/sinon/lib/sinon/util/event.js` & `edx-sga-0.9.0/edx_sga/static/js/bower/sinon/lib/sinon/util/event.js`

 * *Files identical despite different names*

### Comparing `edx-sga-0.8.3/edx_sga/static/js/bower/sinon/lib/sinon/util/xhr_ie.js` & `edx-sga-0.9.0/edx_sga/static/js/bower/sinon/lib/sinon/util/xhr_ie.js`

 * *Files identical despite different names*

### Comparing `edx-sga-0.8.3/edx_sga/static/js/bower/sinon/lib/sinon/util/timers_ie.js` & `edx-sga-0.9.0/edx_sga/static/js/bower/sinon/lib/sinon/util/timers_ie.js`

 * *Files identical despite different names*

### Comparing `edx-sga-0.8.3/edx_sga/static/js/bower/sinon/lib/sinon/call.js` & `edx-sga-0.9.0/edx_sga/static/js/bower/sinon/lib/sinon/call.js`

 * *Files identical despite different names*

### Comparing `edx-sga-0.8.3/edx_sga/static/js/bower/sinon/lib/sinon/typeOf.js` & `edx-sga-0.9.0/edx_sga/static/js/bower/sinon/lib/sinon/typeOf.js`

 * *Files identical despite different names*

### Comparing `edx-sga-0.8.3/edx_sga/static/js/bower/sinon/lib/sinon/behavior.js` & `edx-sga-0.9.0/edx_sga/static/js/bower/sinon/lib/sinon/behavior.js`

 * *Files identical despite different names*

### Comparing `edx-sga-0.8.3/edx_sga/static/js/bower/sinon/lib/sinon/extend.js` & `edx-sga-0.9.0/edx_sga/static/js/bower/sinon/lib/sinon/extend.js`

 * *Files identical despite different names*

### Comparing `edx-sga-0.8.3/edx_sga/static/js/bower/sinon/lib/sinon/mock.js` & `edx-sga-0.9.0/edx_sga/static/js/bower/sinon/lib/sinon/mock.js`

 * *Files identical despite different names*

### Comparing `edx-sga-0.8.3/edx_sga/static/js/bower/sinon/lib/sinon.js` & `edx-sga-0.9.0/edx_sga/static/js/bower/sinon/lib/sinon.js`

 * *Files identical despite different names*

### Comparing `edx-sga-0.8.3/edx_sga/static/js/bower/sinon/README.md` & `edx-sga-0.9.0/edx_sga/static/js/bower/sinon/README.md`

 * *Files identical despite different names*

### Comparing `edx-sga-0.8.3/edx_sga/static/js/bower/sinon/Changelog.txt` & `edx-sga-0.9.0/edx_sga/static/js/bower/sinon/Changelog.txt`

 * *Files identical despite different names*

### Comparing `edx-sga-0.8.3/edx_sga/static/js/bower/sinon/.travis.yml` & `edx-sga-0.9.0/edx_sga/static/js/bower/sinon/.travis.yml`

 * *Files identical despite different names*

### Comparing `edx-sga-0.8.3/edx_sga/static/js/bower/sinon/scripts/ci-test.sh` & `edx-sga-0.9.0/edx_sga/static/js/bower/sinon/scripts/ci-test.sh`

 * *Files identical despite different names*

### Comparing `edx-sga-0.8.3/edx_sga/static/js/bower/sinon/RELEASE.md` & `edx-sga-0.9.0/edx_sga/static/js/bower/sinon/RELEASE.md`

 * *Files identical despite different names*

### Comparing `edx-sga-0.8.3/edx_sga/static/js/bower/sinon/AUTHORS` & `edx-sga-0.9.0/edx_sga/static/js/bower/sinon/AUTHORS`

 * *Files identical despite different names*

### Comparing `edx-sga-0.8.3/edx_sga/static/js/bower/sinon/test/log-error-test.js` & `edx-sga-0.9.0/edx_sga/static/js/bower/sinon/test/log-error-test.js`

 * *Files identical despite different names*

### Comparing `edx-sga-0.8.3/edx_sga/static/js/bower/sinon/test/mock-test.js` & `edx-sga-0.9.0/edx_sga/static/js/bower/sinon/test/mock-test.js`

 * *Files identical despite different names*

### Comparing `edx-sga-0.8.3/edx_sga/static/js/bower/sinon/test/format-test.js` & `edx-sga-0.9.0/edx_sga/static/js/bower/sinon/test/format-test.js`

 * *Files identical despite different names*

### Comparing `edx-sga-0.8.3/edx_sga/static/js/bower/sinon/test/typeOf-test.js` & `edx-sga-0.9.0/edx_sga/static/js/bower/sinon/test/typeOf-test.js`

 * *Files identical despite different names*

### Comparing `edx-sga-0.8.3/edx_sga/static/js/bower/sinon/test/stub-test.js` & `edx-sga-0.9.0/edx_sga/static/js/bower/sinon/test/stub-test.js`

 * *Files identical despite different names*

### Comparing `edx-sga-0.8.3/edx_sga/static/js/bower/sinon/test/assert-test.js` & `edx-sga-0.9.0/edx_sga/static/js/bower/sinon/test/assert-test.js`

 * *Files identical despite different names*

### Comparing `edx-sga-0.8.3/edx_sga/static/js/bower/sinon/test/test-helper.js` & `edx-sga-0.9.0/edx_sga/static/js/bower/sinon/test/test-helper.js`

 * *Files identical despite different names*

### Comparing `edx-sga-0.8.3/edx_sga/static/js/bower/sinon/test/sandbox-test.js` & `edx-sga-0.9.0/edx_sga/static/js/bower/sinon/test/sandbox-test.js`

 * *Files identical despite different names*

### Comparing `edx-sga-0.8.3/edx_sga/static/js/bower/sinon/test/util/fake-server-test.js` & `edx-sga-0.9.0/edx_sga/static/js/bower/sinon/test/util/fake-server-test.js`

 * *Files identical despite different names*

### Comparing `edx-sga-0.8.3/edx_sga/static/js/bower/sinon/test/util/fake-server-with-clock-test.js` & `edx-sga-0.9.0/edx_sga/static/js/bower/sinon/test/util/fake-server-with-clock-test.js`

 * *Files identical despite different names*

### Comparing `edx-sga-0.8.3/edx_sga/static/js/bower/sinon/test/util/fake-xdomain-request-test.js` & `edx-sga-0.9.0/edx_sga/static/js/bower/sinon/test/util/fake-xdomain-request-test.js`

 * *Files identical despite different names*

### Comparing `edx-sga-0.8.3/edx_sga/static/js/bower/sinon/test/util/event-test.js` & `edx-sga-0.9.0/edx_sga/static/js/bower/sinon/test/util/event-test.js`

 * *Files identical despite different names*

### Comparing `edx-sga-0.8.3/edx_sga/static/js/bower/sinon/test/util/fake-timers-test.js` & `edx-sga-0.9.0/edx_sga/static/js/bower/sinon/test/util/fake-timers-test.js`

 * *Files identical despite different names*

### Comparing `edx-sga-0.8.3/edx_sga/static/js/bower/sinon/test/util/fake-xml-http-request-test.js` & `edx-sga-0.9.0/edx_sga/static/js/bower/sinon/test/util/fake-xml-http-request-test.js`

 * *Files identical despite different names*

### Comparing `edx-sga-0.8.3/edx_sga/static/js/bower/sinon/test/match-test.js` & `edx-sga-0.9.0/edx_sga/static/js/bower/sinon/test/match-test.js`

 * *Files identical despite different names*

### Comparing `edx-sga-0.8.3/edx_sga/static/js/bower/sinon/test/call-test.js` & `edx-sga-0.9.0/edx_sga/static/js/bower/sinon/test/call-test.js`

 * *Files identical despite different names*

### Comparing `edx-sga-0.8.3/edx_sga/static/js/bower/sinon/test/buster.js` & `edx-sga-0.9.0/edx_sga/static/js/bower/sinon/test/buster.js`

 * *Files identical despite different names*

### Comparing `edx-sga-0.8.3/edx_sga/static/js/bower/sinon/test/issues/issues-test.js` & `edx-sga-0.9.0/edx_sga/static/js/bower/sinon/test/issues/issues-test.js`

 * *Files identical despite different names*

### Comparing `edx-sga-0.8.3/edx_sga/static/js/bower/sinon/test/times-in-words-test.js` & `edx-sga-0.9.0/edx_sga/static/js/bower/sinon/test/times-in-words-test.js`

 * *Files identical despite different names*

### Comparing `edx-sga-0.8.3/edx_sga/static/js/bower/sinon/test/collection-test.js` & `edx-sga-0.9.0/edx_sga/static/js/bower/sinon/test/collection-test.js`

 * *Files identical despite different names*

### Comparing `edx-sga-0.8.3/edx_sga/static/js/bower/sinon/test/extend-test.js` & `edx-sga-0.9.0/edx_sga/static/js/bower/sinon/test/extend-test.js`

 * *Files identical despite different names*

### Comparing `edx-sga-0.8.3/edx_sga/static/js/bower/sinon/test/test-test.js` & `edx-sga-0.9.0/edx_sga/static/js/bower/sinon/test/test-test.js`

 * *Files identical despite different names*

### Comparing `edx-sga-0.8.3/edx_sga/static/js/bower/sinon/test/spy-test.js` & `edx-sga-0.9.0/edx_sga/static/js/bower/sinon/test/spy-test.js`

 * *Files identical despite different names*

### Comparing `edx-sga-0.8.3/edx_sga/static/js/bower/sinon/test/sinon-test.js` & `edx-sga-0.9.0/edx_sga/static/js/bower/sinon/test/sinon-test.js`

 * *Files identical despite different names*

### Comparing `edx-sga-0.8.3/edx_sga/static/js/bower/sinon/test/test-case-test.js` & `edx-sga-0.9.0/edx_sga/static/js/bower/sinon/test/test-case-test.js`

 * *Files identical despite different names*

### Comparing `edx-sga-0.8.3/edx_sga/static/js/bower/sinon/.eslintrc` & `edx-sga-0.9.0/edx_sga/static/js/bower/sinon/.eslintrc`

 * *Files identical despite different names*

### Comparing `edx-sga-0.8.3/edx_sga/static/js/bower/sinon/package.json` & `edx-sga-0.9.0/edx_sga/static/js/bower/sinon/package.json`

 * *Files identical despite different names*

### Comparing `edx-sga-0.8.3/edx_sga/static/js/bower/sinon/build` & `edx-sga-0.9.0/edx_sga/static/js/bower/sinon/build`

 * *Files identical despite different names*

### Comparing `edx-sga-0.8.3/edx_sga/static/js/bower/sinon/LICENSE` & `edx-sga-0.9.0/edx_sga/static/js/bower/sinon/LICENSE`

 * *Files identical despite different names*

### Comparing `edx-sga-0.8.3/edx_sga/static/js/bower/sinon/CONTRIBUTING.md` & `edx-sga-0.9.0/edx_sga/static/js/bower/sinon/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `edx-sga-0.8.3/edx_sga/static/js/bower/requirejs/require.js` & `edx-sga-0.9.0/edx_sga/static/js/bower/requirejs/require.js`

 * *Files identical despite different names*

### Comparing `edx-sga-0.8.3/edx_sga/static/js/bower/requirejs/.bower.json` & `edx-sga-0.9.0/edx_sga/static/js/bower/requirejs/.bower.json`

 * *Files identical despite different names*

### Comparing `edx-sga-0.8.3/edx_sga/static/js/bower/jquery/src/attributes/val.js` & `edx-sga-0.9.0/edx_sga/static/js/bower/jquery/src/attributes/val.js`

 * *Files identical despite different names*

### Comparing `edx-sga-0.8.3/edx_sga/static/js/bower/jquery/src/attributes/support.js` & `edx-sga-0.9.0/edx_sga/static/js/bower/jquery/src/attributes/support.js`

 * *Files identical despite different names*

### Comparing `edx-sga-0.8.3/edx_sga/static/js/bower/jquery/src/attributes/attr.js` & `edx-sga-0.9.0/edx_sga/static/js/bower/jquery/src/attributes/attr.js`

 * *Files identical despite different names*

### Comparing `edx-sga-0.8.3/edx_sga/static/js/bower/jquery/src/attributes/classes.js` & `edx-sga-0.9.0/edx_sga/static/js/bower/jquery/src/attributes/classes.js`

 * *Files identical despite different names*

### Comparing `edx-sga-0.8.3/edx_sga/static/js/bower/jquery/src/attributes/prop.js` & `edx-sga-0.9.0/edx_sga/static/js/bower/jquery/src/attributes/prop.js`

 * *Files identical despite different names*

### Comparing `edx-sga-0.8.3/edx_sga/static/js/bower/jquery/src/traversing/findFilter.js` & `edx-sga-0.9.0/edx_sga/static/js/bower/jquery/src/traversing/findFilter.js`

 * *Files identical despite different names*

### Comparing `edx-sga-0.8.3/edx_sga/static/js/bower/jquery/src/exports/global.js` & `edx-sga-0.9.0/edx_sga/static/js/bower/jquery/src/exports/global.js`

 * *Files identical despite different names*

### Comparing `edx-sga-0.8.3/edx_sga/static/js/bower/jquery/src/exports/amd.js` & `edx-sga-0.9.0/edx_sga/static/js/bower/jquery/src/exports/amd.js`

 * *Files identical despite different names*

### Comparing `edx-sga-0.8.3/edx_sga/static/js/bower/jquery/src/intro.js` & `edx-sga-0.9.0/edx_sga/static/js/bower/jquery/src/intro.js`

 * *Files identical despite different names*

### Comparing `edx-sga-0.8.3/edx_sga/static/js/bower/jquery/src/dimensions.js` & `edx-sga-0.9.0/edx_sga/static/js/bower/jquery/src/dimensions.js`

 * *Files identical despite different names*

### Comparing `edx-sga-0.8.3/edx_sga/static/js/bower/jquery/src/queue/delay.js` & `edx-sga-0.9.0/edx_sga/static/js/bower/jquery/src/queue/delay.js`

 * *Files identical despite different names*

### Comparing `edx-sga-0.8.3/edx_sga/static/js/bower/jquery/src/core.js` & `edx-sga-0.9.0/edx_sga/static/js/bower/jquery/src/core.js`

 * *Files identical despite different names*

### Comparing `edx-sga-0.8.3/edx_sga/static/js/bower/jquery/src/ajax.js` & `edx-sga-0.9.0/edx_sga/static/js/bower/jquery/src/ajax.js`

 * *Files identical despite different names*

### Comparing `edx-sga-0.8.3/edx_sga/static/js/bower/jquery/src/css/defaultDisplay.js` & `edx-sga-0.9.0/edx_sga/static/js/bower/jquery/src/css/defaultDisplay.js`

 * *Files identical despite different names*

### Comparing `edx-sga-0.8.3/edx_sga/static/js/bower/jquery/src/css/support.js` & `edx-sga-0.9.0/edx_sga/static/js/bower/jquery/src/css/support.js`

 * *Files identical despite different names*

### Comparing `edx-sga-0.8.3/edx_sga/static/js/bower/jquery/src/css/curCSS.js` & `edx-sga-0.9.0/edx_sga/static/js/bower/jquery/src/css/curCSS.js`

 * *Files identical despite different names*

### Comparing `edx-sga-0.8.3/edx_sga/static/js/bower/jquery/src/css/swap.js` & `edx-sga-0.9.0/edx_sga/static/js/bower/jquery/src/css/swap.js`

 * *Files identical despite different names*

### Comparing `edx-sga-0.8.3/edx_sga/static/js/bower/jquery/src/effects.js` & `edx-sga-0.9.0/edx_sga/static/js/bower/jquery/src/effects.js`

 * *Files identical despite different names*

### Comparing `edx-sga-0.8.3/edx_sga/static/js/bower/jquery/src/serialize.js` & `edx-sga-0.9.0/edx_sga/static/js/bower/jquery/src/serialize.js`

 * *Files identical despite different names*

### Comparing `edx-sga-0.8.3/edx_sga/static/js/bower/jquery/src/callbacks.js` & `edx-sga-0.9.0/edx_sga/static/js/bower/jquery/src/callbacks.js`

 * *Files identical despite different names*

### Comparing `edx-sga-0.8.3/edx_sga/static/js/bower/jquery/src/core/access.js` & `edx-sga-0.9.0/edx_sga/static/js/bower/jquery/src/core/access.js`

 * *Files identical despite different names*

### Comparing `edx-sga-0.8.3/edx_sga/static/js/bower/jquery/src/core/parseHTML.js` & `edx-sga-0.9.0/edx_sga/static/js/bower/jquery/src/core/parseHTML.js`

 * *Files identical despite different names*

### Comparing `edx-sga-0.8.3/edx_sga/static/js/bower/jquery/src/core/init.js` & `edx-sga-0.9.0/edx_sga/static/js/bower/jquery/src/core/init.js`

 * *Files identical despite different names*

### Comparing `edx-sga-0.8.3/edx_sga/static/js/bower/jquery/src/core/ready.js` & `edx-sga-0.9.0/edx_sga/static/js/bower/jquery/src/core/ready.js`

 * *Files identical despite different names*

### Comparing `edx-sga-0.8.3/edx_sga/static/js/bower/jquery/src/queue.js` & `edx-sga-0.9.0/edx_sga/static/js/bower/jquery/src/queue.js`

 * *Files identical despite different names*

### Comparing `edx-sga-0.8.3/edx_sga/static/js/bower/jquery/src/manipulation.js` & `edx-sga-0.9.0/edx_sga/static/js/bower/jquery/src/manipulation.js`

 * *Files identical despite different names*

### Comparing `edx-sga-0.8.3/edx_sga/static/js/bower/jquery/src/effects/Tween.js` & `edx-sga-0.9.0/edx_sga/static/js/bower/jquery/src/effects/Tween.js`

 * *Files identical despite different names*

### Comparing `edx-sga-0.8.3/edx_sga/static/js/bower/jquery/src/css.js` & `edx-sga-0.9.0/edx_sga/static/js/bower/jquery/src/css.js`

 * *Files identical despite different names*

### Comparing `edx-sga-0.8.3/edx_sga/static/js/bower/jquery/src/ajax/jsonp.js` & `edx-sga-0.9.0/edx_sga/static/js/bower/jquery/src/ajax/jsonp.js`

 * *Files identical despite different names*

### Comparing `edx-sga-0.8.3/edx_sga/static/js/bower/jquery/src/ajax/load.js` & `edx-sga-0.9.0/edx_sga/static/js/bower/jquery/src/ajax/load.js`

 * *Files identical despite different names*

### Comparing `edx-sga-0.8.3/edx_sga/static/js/bower/jquery/src/ajax/xhr.js` & `edx-sga-0.9.0/edx_sga/static/js/bower/jquery/src/ajax/xhr.js`

 * *Files identical despite different names*

### Comparing `edx-sga-0.8.3/edx_sga/static/js/bower/jquery/src/ajax/script.js` & `edx-sga-0.9.0/edx_sga/static/js/bower/jquery/src/ajax/script.js`

 * *Files identical despite different names*

### Comparing `edx-sga-0.8.3/edx_sga/static/js/bower/jquery/src/manipulation/support.js` & `edx-sga-0.9.0/edx_sga/static/js/bower/jquery/src/manipulation/support.js`

 * *Files identical despite different names*

### Comparing `edx-sga-0.8.3/edx_sga/static/js/bower/jquery/src/wrap.js` & `edx-sga-0.9.0/edx_sga/static/js/bower/jquery/src/wrap.js`

 * *Files identical despite different names*

### Comparing `edx-sga-0.8.3/edx_sga/static/js/bower/jquery/src/selector-native.js` & `edx-sga-0.9.0/edx_sga/static/js/bower/jquery/src/selector-native.js`

 * *Files identical despite different names*

### Comparing `edx-sga-0.8.3/edx_sga/static/js/bower/jquery/src/data/Data.js` & `edx-sga-0.9.0/edx_sga/static/js/bower/jquery/src/data/Data.js`

 * *Files identical despite different names*

### Comparing `edx-sga-0.8.3/edx_sga/static/js/bower/jquery/src/traversing.js` & `edx-sga-0.9.0/edx_sga/static/js/bower/jquery/src/traversing.js`

 * *Files identical despite different names*

### Comparing `edx-sga-0.8.3/edx_sga/static/js/bower/jquery/src/event/alias.js` & `edx-sga-0.9.0/edx_sga/static/js/bower/jquery/src/event/alias.js`

 * *Files identical despite different names*

### Comparing `edx-sga-0.8.3/edx_sga/static/js/bower/jquery/src/event.js` & `edx-sga-0.9.0/edx_sga/static/js/bower/jquery/src/event.js`

 * *Files identical despite different names*

### Comparing `edx-sga-0.8.3/edx_sga/static/js/bower/jquery/src/offset.js` & `edx-sga-0.9.0/edx_sga/static/js/bower/jquery/src/offset.js`

 * *Files identical despite different names*

### Comparing `edx-sga-0.8.3/edx_sga/static/js/bower/jquery/src/deferred.js` & `edx-sga-0.9.0/edx_sga/static/js/bower/jquery/src/deferred.js`

 * *Files identical despite different names*

### Comparing `edx-sga-0.8.3/edx_sga/static/js/bower/jquery/src/jquery.js` & `edx-sga-0.9.0/edx_sga/static/js/bower/jquery/src/jquery.js`

 * *Files identical despite different names*

### Comparing `edx-sga-0.8.3/edx_sga/static/js/bower/jquery/src/data.js` & `edx-sga-0.9.0/edx_sga/static/js/bower/jquery/src/data.js`

 * *Files identical despite different names*

### Comparing `edx-sga-0.8.3/edx_sga/static/js/bower/jquery/MIT-LICENSE.txt` & `edx-sga-0.9.0/edx_sga/static/js/bower/jquery/MIT-LICENSE.txt`

 * *Files identical despite different names*

### Comparing `edx-sga-0.8.3/edx_sga/static/js/bower/jquery/.bower.json` & `edx-sga-0.9.0/edx_sga/static/js/bower/jquery/.bower.json`

 * *Files identical despite different names*

### Comparing `edx-sga-0.8.3/edx_sga/static/js/bower/URIjs/README.md` & `edx-sga-0.9.0/edx_sga/static/js/bower/URIjs/README.md`

 * *Files identical despite different names*

### Comparing `edx-sga-0.8.3/edx_sga/static/js/bower/URIjs/src/jquery.URI.min.js` & `edx-sga-0.9.0/edx_sga/static/js/bower/URIjs/src/jquery.URI.min.js`

 * *Files identical despite different names*

### Comparing `edx-sga-0.8.3/edx_sga/static/js/bower/URIjs/src/URI.min.js` & `edx-sga-0.9.0/edx_sga/static/js/bower/URIjs/src/URI.min.js`

 * *Files identical despite different names*

### Comparing `edx-sga-0.8.3/edx_sga/static/js/bower/URIjs/src/URITemplate.js` & `edx-sga-0.9.0/edx_sga/static/js/bower/URIjs/src/URITemplate.js`

 * *Files identical despite different names*

### Comparing `edx-sga-0.8.3/edx_sga/static/js/bower/URIjs/src/URI.fragmentQuery.js` & `edx-sga-0.9.0/edx_sga/static/js/bower/URIjs/src/URI.fragmentQuery.js`

 * *Files identical despite different names*

### Comparing `edx-sga-0.8.3/edx_sga/static/js/bower/URIjs/src/SecondLevelDomains.js` & `edx-sga-0.9.0/edx_sga/static/js/bower/URIjs/src/SecondLevelDomains.js`

 * *Files identical despite different names*

### Comparing `edx-sga-0.8.3/edx_sga/static/js/bower/URIjs/src/jquery.URI.js` & `edx-sga-0.9.0/edx_sga/static/js/bower/URIjs/src/jquery.URI.js`

 * *Files identical despite different names*

### Comparing `edx-sga-0.8.3/edx_sga/static/js/bower/URIjs/src/IPv6.js` & `edx-sga-0.9.0/edx_sga/static/js/bower/URIjs/src/IPv6.js`

 * *Files identical despite different names*

### Comparing `edx-sga-0.8.3/edx_sga/static/js/bower/URIjs/src/punycode.js` & `edx-sga-0.9.0/edx_sga/static/js/bower/URIjs/src/punycode.js`

 * *Files identical despite different names*

### Comparing `edx-sga-0.8.3/edx_sga/static/js/bower/URIjs/src/URI.fragmentURI.js` & `edx-sga-0.9.0/edx_sga/static/js/bower/URIjs/src/URI.fragmentURI.js`

 * *Files identical despite different names*

### Comparing `edx-sga-0.8.3/edx_sga/static/js/bower/URIjs/src/URI.js` & `edx-sga-0.9.0/edx_sga/static/js/bower/URIjs/src/URI.js`

 * *Files identical despite different names*

### Comparing `edx-sga-0.8.3/edx_sga/static/js/bower/URIjs/.bower.json` & `edx-sga-0.9.0/edx_sga/static/js/bower/URIjs/.bower.json`

 * *Files identical despite different names*

### Comparing `edx-sga-0.8.3/edx_sga/static/js/bower/URIjs/LICENSE.txt` & `edx-sga-0.9.0/edx_sga/static/js/bower/URIjs/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `edx-sga-0.8.3/edx_sga/static/js/bower/URIjs/contributing.md` & `edx-sga-0.9.0/edx_sga/static/js/bower/URIjs/contributing.md`

 * *Files identical despite different names*

### Comparing `edx-sga-0.8.3/edx_sga/tests/integration_tests.py` & `edx-sga-0.9.0/edx_sga/tests/integration_tests.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,17 +12,17 @@
 
 from ddt import ddt, data, unpack
 import mock
 from opaque_keys.edx.locator import CourseLocator
 from opaque_keys.edx.locations import Location  # lint-amnesty, pylint: disable=import-error
 import pytz
 
-from courseware import module_render as render  # lint-amnesty, pylint: disable=import-error
-from courseware.models import StudentModule  # lint-amnesty, pylint: disable=import-error
-from courseware.tests.factories import StaffFactory  # lint-amnesty, pylint: disable=import-error
+from lms.djangoapps.courseware import module_render as render  # lint-amnesty, pylint: disable=import-error
+from lms.djangoapps.courseware.models import StudentModule  # lint-amnesty, pylint: disable=import-error
+from lms.djangoapps.courseware.tests.factories import StaffFactory  # lint-amnesty, pylint: disable=import-error
 from django.contrib.auth.models import User  # lint-amnesty, pylint: disable=import-error
 from django.core.exceptions import PermissionDenied  # lint-amnesty, pylint: disable=import-error
 from django.db import transaction  # lint-amnesty, pylint: disable=import-error
 from django.test.utils import override_settings  # lint-amnesty, pylint: disable=import-error
 from submissions import api as submissions_api  # lint-amnesty, pylint: disable=import-error
 from submissions.models import StudentItem  # lint-amnesty, pylint: disable=import-error
 from student.models import anonymous_id_for_user, UserProfile  # lint-amnesty, pylint: disable=import-error
```

### Comparing `edx-sga-0.8.3/edx_sga/tests/common.py` & `edx-sga-0.9.0/edx_sga/tests/common.py`

 * *Files identical despite different names*

### Comparing `edx-sga-0.8.3/edx_sga/tests/test_sga.py` & `edx-sga-0.9.0/edx_sga/tests/test_sga.py`

 * *Files 2% similar despite different names*

```diff
@@ -597,29 +597,32 @@
             return_value=score
         ), mock.patch(
             "edx_sga.sga.is_finalized_submission",
             return_value=is_finalized_submission
         ):
             assert block.upload_allowed(submission_data={}) is expected_value
 
+    @mock.patch('edx_sga.sga.StaffGradedAssignmentXBlock.count_archive_files')
     @mock.patch('edx_sga.sga.zip_student_submissions')
     @mock.patch('edx_sga.sga.StaffGradedAssignmentXBlock.get_sorted_submissions')
     @data((False, False), (True, True))
     @unpack
     def test_prepare_download_submissions(
             self,
             is_zip_file_available,
             downloadable,
             get_sorted_submissions,
             zip_student_submissions,
+            count_archive_files
     ):
         """
         Test prepare download api
         """
         block = self.make_xblock()
+        count_archive_files.return_value = 2
         get_sorted_submissions.return_value = [
             {
                 'submission_id': uuid.uuid4().hex,
                 'filename': "test_{}.txt".format(uuid.uuid4().hex),
                 'timestamp': datetime.datetime.now(tz=pytz.utc)
             } for __ in range(2)
         ]
@@ -634,14 +637,57 @@
             'edx_sga.utils.default_storage.modified_time',
             return_value=datetime.datetime.now()
         ):
             response = block.prepare_download_submissions(None)
             response_body = json.loads(response.body)
             assert response_body["downloadable"] is downloadable
 
+    @mock.patch('edx_sga.sga.get_file_modified_time_utc')
+    @mock.patch('edx_sga.sga.StaffGradedAssignmentXBlock.count_archive_files')
+    @mock.patch('edx_sga.sga.zip_student_submissions')
+    @mock.patch('edx_sga.sga.StaffGradedAssignmentXBlock.get_sorted_submissions')
+    @data((2, True, False), (1, False, True))
+    @unpack
+    def test_prepare_download_submissions_when_student_score_reset(
+            self,
+            count_archive_files,
+            downloadable,
+            zip_task_called,
+            get_sorted_submissions,
+            zip_student_submissions,
+            count_archive_files_mock,
+            get_file_modified_time_utc
+    ):
+        """
+        Test prepare download api
+        """
+        now = datetime.datetime.now(tz=pytz.utc)
+        block = self.make_xblock()
+        count_archive_files_mock.return_value = count_archive_files
+        get_sorted_submissions.return_value = [
+            {
+                'submission_id': uuid.uuid4().hex,
+                'filename': "test_{}.txt".format(uuid.uuid4().hex),
+                'timestamp': now
+            } for __ in range(2)
+        ]
+        get_file_modified_time_utc.return_value = now
+        zip_student_submissions.delay = mock.Mock()
+        with mock.patch(
+            "edx_sga.sga.StaffGradedAssignmentXBlock.is_zip_file_available", return_value=True
+        ), mock.patch(
+            'edx_sga.sga.StaffGradedAssignmentXBlock.get_real_user', return_value=self.staff
+        ), mock.patch(
+            'edx_sga.utils.default_storage.modified_time', return_value=datetime.datetime.now()
+        ):
+            response = block.prepare_download_submissions(None)
+            response_body = json.loads(response.body)
+            assert response_body["downloadable"] is downloadable
+            assert zip_student_submissions.delay.called is zip_task_called
+
     @mock.patch('edx_sga.sga.zip_student_submissions')
     @mock.patch('edx_sga.sga.StaffGradedAssignmentXBlock.get_sorted_submissions')
     def test_prepare_download_submissions_task_called(
             self,
             get_sorted_submissions,
             zip_student_submissions
     ):
@@ -667,15 +713,15 @@
             'edx_sga.sga.default_storage.modified_time',
             return_value=datetime.datetime.now()
         ):
             response = block.prepare_download_submissions(None)
             response_body = json.loads(response.body)
             assert response_body["downloadable"] is False
 
-        zip_student_submissions.delay.assert_called_with(
+        zip_student_submissions.delay.assert_called_once_with(
             unicode(block.block_course_id),
             unicode(block.block_id),
             unicode(block.location),
             self.staff.username
         )
 
     @data((False, False), (True, True))
```

### Comparing `edx-sga-0.8.3/edx_sga/tests/test_utils.py` & `edx-sga-0.9.0/edx_sga/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `edx-sga-0.8.3/edx_sga/tests/test_showanswer.py` & `edx-sga-0.9.0/edx_sga/tests/test_showanswer.py`

 * *Files identical despite different names*

### Comparing `edx-sga-0.8.3/edx_sga/templates/staff_graded_assignment/show.html` & `edx-sga-0.9.0/edx_sga/templates/staff_graded_assignment/show.html`

 * *Files 0% similar despite different names*

```diff
@@ -50,15 +50,15 @@
     <% } %>
     <% if (solution) { %>
       <div class="solution">
         <%= solution %>
       </div>
     <% } %>
     <% if (error) { %>
-      <p class="error"><%= error %></p>
+      <p class="error" tabindex="-1" aria-live="polite"><%= error %></p>
     <% } %>
   </script>
 
   <div id="sga-content">
   </div>
 
   {% if is_course_staff %}
@@ -201,14 +201,15 @@
             <button type="submit">{% trans "Submit" %}</button>
             <button type="button" id="enter-grade-cancel">
               {% trans "Cancel" %}
             </button>
             <button type="button" id="remove-grade">
               {% trans "Remove grade" %}
             </button>
+            <i class="fa fa-spinner fa-pulse ccx-enter-grade-spinner"></i>
           </div>
         </form>
       </div>
     </div>
   </section>
   {% endif %}
 </div>
```

### Comparing `edx-sga-0.8.3/edx_sga/tasks.py` & `edx-sga-0.9.0/edx_sga/tasks.py`

 * *Files identical despite different names*

### Comparing `edx-sga-0.8.3/edx_sga/showanswer.py` & `edx-sga-0.9.0/edx_sga/showanswer.py`

 * *Files identical despite different names*

### Comparing `edx-sga-0.8.3/edx_sga/test_settings.py` & `edx-sga-0.9.0/edx_sga/test_settings.py`

 * *Files identical despite different names*

### Comparing `edx-sga-0.8.3/README.md` & `edx-sga-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `edx-sga-0.8.3/edx_sga.egg-info/SOURCES.txt` & `edx-sga-0.9.0/edx_sga.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `edx-sga-0.8.3/setup.py` & `edx-sga-0.9.0/setup.py`

 * *Files identical despite different names*

