# Comparing `tmp/buckaroo-0.3.2.tar.gz` & `tmp/buckaroo-0.3.3.tar.gz`

## Comparing `buckaroo-0.3.2.tar` & `buckaroo-0.3.3.tar`

### file list

```diff
@@ -1,108 +1,105 @@
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 buckaroo-0.3.2/.coveragerc
--rw-r--r--   0        0        0     7520 2020-02-02 00:00:00.000000 buckaroo-0.3.2/RELEASE.md
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 buckaroo-0.3.2/Untitled.ipynb
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 buckaroo-0.3.2/babel.config.js
--rw-r--r--   0        0        0    24393 2020-02-02 00:00:00.000000 buckaroo-0.3.2/bike-share-data-explore.ipynb
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 buckaroo-0.3.2/buckaroo.json
--rw-r--r--   0        0        0    24936 2020-02-02 00:00:00.000000 buckaroo-0.3.2/col-ordering.ipynb
--rwxr-xr-x   0        0        0      237 2020-02-02 00:00:00.000000 buckaroo-0.3.2/full_build.sh
--rw-r--r--   0        0        0   129498 2020-02-02 00:00:00.000000 buckaroo-0.3.2/gbfs-play.ipynb
--rw-r--r--   0        0        0    97653 2020-02-02 00:00:00.000000 buckaroo-0.3.2/gbfs-play2.ipynb
--rw-r--r--   0        0        0     7542 2020-02-02 00:00:00.000000 buckaroo-0.3.2/introduction.ipynb
--rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 buckaroo-0.3.2/notes.txt
--rw-r--r--   0        0        0   693792 2020-02-02 00:00:00.000000 buckaroo-0.3.2/package-lock.json
--rw-r--r--   0        0        0     6096 2020-02-02 00:00:00.000000 buckaroo-0.3.2/package.json
--rw-r--r--   0        0        0     6380 2020-02-02 00:00:00.000000 buckaroo-0.3.2/package.json.old
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 buckaroo-0.3.2/setup.py
--rw-r--r--   0        0        0     4479 2020-02-02 00:00:00.000000 buckaroo-0.3.2/tryit.ipynb
--rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 buckaroo-0.3.2/tsconfig.json
--rw-r--r--   0        0        0     5105 2020-02-02 00:00:00.000000 buckaroo-0.3.2/webpack.config.js
--rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 buckaroo-0.3.2/webpack.lab.config.js
--rw-r--r--   0        0        0   365701 2020-02-02 00:00:00.000000 buckaroo-0.3.2/yarn.lock
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 buckaroo-0.3.2/.yarn/cache/.gitignore
--rw-r--r--   0        0        0     1707 2020-02-02 00:00:00.000000 buckaroo-0.3.2/buckaroo/__init__.py
--rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 buckaroo-0.3.2/buckaroo/_frontend.py
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 buckaroo-0.3.2/buckaroo/_version.py
--rw-r--r--   0        0        0     5065 2020-02-02 00:00:00.000000 buckaroo-0.3.2/buckaroo/all_transforms.py
--rw-r--r--   0        0        0     7038 2020-02-02 00:00:00.000000 buckaroo-0.3.2/buckaroo/buckaroo_widget.py
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 buckaroo-0.3.2/buckaroo/channeldata.json
--rw-r--r--   0        0        0     1652 2020-02-02 00:00:00.000000 buckaroo-0.3.2/buckaroo/configure_utils.py
--rw-r--r--   0        0        0     5608 2020-02-02 00:00:00.000000 buckaroo-0.3.2/buckaroo/dcf_transform.py
--rw-r--r--   0        0        0     6535 2020-02-02 00:00:00.000000 buckaroo-0.3.2/buckaroo/df_methods.py
--rw-r--r--   0        0        0     1786 2020-02-02 00:00:00.000000 buckaroo-0.3.2/buckaroo/index.html
--rw-r--r--   0        0        0    17284 2020-02-02 00:00:00.000000 buckaroo-0.3.2/buckaroo/lispy.py
--rw-r--r--   0        0        0     7578 2020-02-02 00:00:00.000000 buckaroo-0.3.2/buckaroo/summary_stats.py
--rw-r--r--   0        0        0     2707 2020-02-02 00:00:00.000000 buckaroo-0.3.2/buckaroo/views.py
--rw-r--r--   0        0        0     5513 2020-02-02 00:00:00.000000 buckaroo-0.3.2/buckaroo/labextension/package.json
--rw-r--r--   0        0        0   145367 2020-02-02 00:00:00.000000 buckaroo-0.3.2/buckaroo/labextension/static/0.c008020c7e2133e6c7db.js
--rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 buckaroo-0.3.2/buckaroo/labextension/static/0.c008020c7e2133e6c7db.js.LICENSE.txt
--rw-r--r--   0        0        0    35455 2020-02-02 00:00:00.000000 buckaroo-0.3.2/buckaroo/labextension/static/399.252405500e4886745cf0.js
--rw-r--r--   0        0        0   231664 2020-02-02 00:00:00.000000 buckaroo-0.3.2/buckaroo/labextension/static/41.dea207301743f71053c5.js
--rw-r--r--   0        0        0     1153 2020-02-02 00:00:00.000000 buckaroo-0.3.2/buckaroo/labextension/static/480.c541de2b54a15c8f7330.js
--rw-r--r--   0        0        0    70484 2020-02-02 00:00:00.000000 buckaroo-0.3.2/buckaroo/labextension/static/486.f08778dfb765d893ceaf.js
--rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 buckaroo-0.3.2/buckaroo/labextension/static/486.f08778dfb765d893ceaf.js.LICENSE.txt
--rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 buckaroo-0.3.2/buckaroo/labextension/static/568.50d29d049ddb62602cc0.js
--rw-r--r--   0        0        0  1067038 2020-02-02 00:00:00.000000 buckaroo-0.3.2/buckaroo/labextension/static/731.d4bf968c7a94633ef5a3.js
--rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 buckaroo-0.3.2/buckaroo/labextension/static/731.d4bf968c7a94633ef5a3.js.LICENSE.txt
--rw-r--r--   0        0        0   139612 2020-02-02 00:00:00.000000 buckaroo-0.3.2/buckaroo/labextension/static/935.2832d17fef97c1ec6694.js
--rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 buckaroo-0.3.2/buckaroo/labextension/static/935.2832d17fef97c1ec6694.js.LICENSE.txt
--rw-r--r--   0        0        0     7838 2020-02-02 00:00:00.000000 buckaroo-0.3.2/buckaroo/labextension/static/remoteEntry.25db2035d9cfb129895d.js
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 buckaroo-0.3.2/buckaroo/labextension/static/style.js
--rw-r--r--   0        0        0    11965 2020-02-02 00:00:00.000000 buckaroo-0.3.2/buckaroo/labextension/static/third-party-licenses.json
--rw-r--r--   0        0        0  1691110 2020-02-02 00:00:00.000000 buckaroo-0.3.2/buckaroo/nbextension/index.js
--rw-r--r--   0        0        0     2019 2020-02-02 00:00:00.000000 buckaroo-0.3.2/buckaroo/nbextension/index.js.LICENSE.txt
--rw-r--r--   0        0        0  5896429 2020-02-02 00:00:00.000000 buckaroo-0.3.2/buckaroo/nbextension/index.js.map
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 buckaroo-0.3.2/buckaroo/noarch/current_repodata.json
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 buckaroo-0.3.2/buckaroo/noarch/current_repodata.json.bz2
--rw-r--r--   0        0        0     2400 2020-02-02 00:00:00.000000 buckaroo-0.3.2/buckaroo/noarch/index.html
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 buckaroo-0.3.2/buckaroo/noarch/repodata.json
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 buckaroo-0.3.2/buckaroo/noarch/repodata.json.bz2
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 buckaroo-0.3.2/buckaroo/noarch/repodata_from_packages.json
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 buckaroo-0.3.2/buckaroo/noarch/repodata_from_packages.json.bz2
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 buckaroo-0.3.2/docs/Makefile
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 buckaroo-0.3.2/docs/make.bat
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 buckaroo-0.3.2/docs/source/.#index.rst -> paddy@Paddys-MacBook-Air.local.405
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 buckaroo-0.3.2/docs/source/.#nodejs-download.html -> paddy@Paddys-MacBook-Air.local.405
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 buckaroo-0.3.2/docs/source/.#vs-code-download.html -> paddy@Paddys-MacBook-Air.local.405
--rw-r--r--   0        0        0     5575 2020-02-02 00:00:00.000000 buckaroo-0.3.2/docs/source/FAQ.rst
--rw-r--r--   0        0        0      928 2020-02-02 00:00:00.000000 buckaroo-0.3.2/docs/source/conf.py
--rw-r--r--   0        0        0     4104 2020-02-02 00:00:00.000000 buckaroo-0.3.2/docs/source/contributing.rst
--rw-r--r--   0        0        0     1422 2020-02-02 00:00:00.000000 buckaroo-0.3.2/docs/source/index.rst
--rwxr-xr-x   0        0        0      295 2020-02-02 00:00:00.000000 buckaroo-0.3.2/docs/source/install.rst
--rw-r--r--   0        0        0     3404 2020-02-02 00:00:00.000000 buckaroo-0.3.2/docs/source/using.rst
--rw-r--r--   0        0        0     2019 2020-02-02 00:00:00.000000 buckaroo-0.3.2/docs/source/_static/embed-bundle.js.LICENSE.txt
--rw-r--r--   0        0        0     7144 2020-02-02 00:00:00.000000 buckaroo-0.3.2/example-notebooks/testcases-fast.ipynb
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 buckaroo-0.3.2/js/comp1.tsx
--rw-r--r--   0        0        0     3330 2020-02-02 00:00:00.000000 buckaroo-0.3.2/js/dcefwidget.ts
--rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 buckaroo-0.3.2/js/extension.ts
--rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 buckaroo-0.3.2/js/index.ts
--rw-r--r--   0        0        0     1268 2020-02-02 00:00:00.000000 buckaroo-0.3.2/js/plugin.ts
--rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 buckaroo-0.3.2/js/version.ts
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 buckaroo-0.3.2/js/components/.#DFViewer.tsx -> paddy@Paddys-MacBook-Air.local.405
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 buckaroo-0.3.2/js/components/.#staticData.ts -> paddy@Paddys-MacBook-Air.local.405
--rw-r--r--   0        0        0     2179 2020-02-02 00:00:00.000000 buckaroo-0.3.2/js/components/ColumnsEditor.tsx
--rw-r--r--   0        0        0     1033 2020-02-02 00:00:00.000000 buckaroo-0.3.2/js/components/CommandUtils.ts
--rw-r--r--   0        0        0     2849 2020-02-02 00:00:00.000000 buckaroo-0.3.2/js/components/DCFCell.tsx
--rw-r--r--   0        0        0     4520 2020-02-02 00:00:00.000000 buckaroo-0.3.2/js/components/DFViewer.tsx
--rw-r--r--   0        0        0     3617 2020-02-02 00:00:00.000000 buckaroo-0.3.2/js/components/DependentTabs.tsx
--rw-r--r--   0        0        0     4875 2020-02-02 00:00:00.000000 buckaroo-0.3.2/js/components/OperationDetail.tsx
--rw-r--r--   0        0        0     1178 2020-02-02 00:00:00.000000 buckaroo-0.3.2/js/components/OperationUtils.ts
--rw-r--r--   0        0        0     6989 2020-02-02 00:00:00.000000 buckaroo-0.3.2/js/components/Operations.tsx
--rw-r--r--   0        0        0     3422 2020-02-02 00:00:00.000000 buckaroo-0.3.2/js/components/StatusBar.tsx
--rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 buckaroo-0.3.2/js/components/bakedOperationDefaults.ts
--rw-r--r--   0        0        0     3002 2020-02-02 00:00:00.000000 buckaroo-0.3.2/js/components/gridUtils.ts
--rw-r--r--   0        0        0     6305 2020-02-02 00:00:00.000000 buckaroo-0.3.2/js/components/staticData.ts
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 buckaroo-0.3.2/js/components/utils.ts
--rw-r--r--   0        0        0     3026 2020-02-02 00:00:00.000000 buckaroo-0.3.2/js/style/dcf-npm.css
--rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 buckaroo-0.3.2/js/style/icons/arrow-down-short-dark.svg
--rwxr-xr-x   0        0        0      416 2020-02-02 00:00:00.000000 buckaroo-0.3.2/js/style/icons/arrow-down-short.svg
--rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 buckaroo-0.3.2/js/style/icons/arrow-up-short-dark.svg
--rwxr-xr-x   0        0        0      400 2020-02-02 00:00:00.000000 buckaroo-0.3.2/js/style/icons/arrow-up-short.svg
--rwxr-xr-x   0        0        0      349 2020-02-02 00:00:00.000000 buckaroo-0.3.2/js/style/icons/filter-dark.svg
--rwxr-xr-x   0        0        0      349 2020-02-02 00:00:00.000000 buckaroo-0.3.2/js/style/icons/filter.svg
--rw-r--r--   0        0        0  1420117 2020-02-02 00:00:00.000000 buckaroo-0.3.2/static/images/Buckaroo-screenshot.png
--rw-r--r--   0        0        0     2093 2020-02-02 00:00:00.000000 buckaroo-0.3.2/.gitignore
--rw-r--r--   0        0        0     1494 2020-02-02 00:00:00.000000 buckaroo-0.3.2/LICENSE.txt
--rw-r--r--   0        0        0    10241 2020-02-02 00:00:00.000000 buckaroo-0.3.2/README.md
--rw-r--r--   0        0        0     3221 2020-02-02 00:00:00.000000 buckaroo-0.3.2/pyproject.toml
--rw-r--r--   0        0        0    13091 2020-02-02 00:00:00.000000 buckaroo-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 buckaroo-0.3.3/.coveragerc
+-rw-r--r--   0        0        0     7520 2020-02-02 00:00:00.000000 buckaroo-0.3.3/RELEASE.md
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 buckaroo-0.3.3/Untitled.ipynb
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 buckaroo-0.3.3/babel.config.js
+-rw-r--r--   0        0        0    24393 2020-02-02 00:00:00.000000 buckaroo-0.3.3/bike-share-data-explore.ipynb
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 buckaroo-0.3.3/buckaroo.json
+-rw-r--r--   0        0        0    24936 2020-02-02 00:00:00.000000 buckaroo-0.3.3/col-ordering.ipynb
+-rwxr-xr-x   0        0        0      237 2020-02-02 00:00:00.000000 buckaroo-0.3.3/full_build.sh
+-rw-r--r--   0        0        0   129498 2020-02-02 00:00:00.000000 buckaroo-0.3.3/gbfs-play.ipynb
+-rw-r--r--   0        0        0    97653 2020-02-02 00:00:00.000000 buckaroo-0.3.3/gbfs-play2.ipynb
+-rw-r--r--   0        0        0     7542 2020-02-02 00:00:00.000000 buckaroo-0.3.3/introduction.ipynb
+-rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 buckaroo-0.3.3/notes.txt
+-rw-r--r--   0        0        0   693792 2020-02-02 00:00:00.000000 buckaroo-0.3.3/package-lock.json
+-rw-r--r--   0        0        0     6096 2020-02-02 00:00:00.000000 buckaroo-0.3.3/package.json
+-rw-r--r--   0        0        0     6380 2020-02-02 00:00:00.000000 buckaroo-0.3.3/package.json.old
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 buckaroo-0.3.3/setup.py
+-rw-r--r--   0        0        0     4479 2020-02-02 00:00:00.000000 buckaroo-0.3.3/tryit.ipynb
+-rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 buckaroo-0.3.3/tsconfig.json
+-rw-r--r--   0        0        0     5105 2020-02-02 00:00:00.000000 buckaroo-0.3.3/webpack.config.js
+-rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 buckaroo-0.3.3/webpack.lab.config.js
+-rw-r--r--   0        0        0   365701 2020-02-02 00:00:00.000000 buckaroo-0.3.3/yarn.lock
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 buckaroo-0.3.3/.yarn/cache/.gitignore
+-rw-r--r--   0        0        0     1716 2020-02-02 00:00:00.000000 buckaroo-0.3.3/buckaroo/__init__.py
+-rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 buckaroo-0.3.3/buckaroo/_frontend.py
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 buckaroo-0.3.3/buckaroo/_version.py
+-rw-r--r--   0        0        0     5065 2020-02-02 00:00:00.000000 buckaroo-0.3.3/buckaroo/all_transforms.py
+-rw-r--r--   0        0        0     7007 2020-02-02 00:00:00.000000 buckaroo-0.3.3/buckaroo/buckaroo_widget.py
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 buckaroo-0.3.3/buckaroo/channeldata.json
+-rw-r--r--   0        0        0     1652 2020-02-02 00:00:00.000000 buckaroo-0.3.3/buckaroo/configure_utils.py
+-rw-r--r--   0        0        0     5608 2020-02-02 00:00:00.000000 buckaroo-0.3.3/buckaroo/dcf_transform.py
+-rw-r--r--   0        0        0     6535 2020-02-02 00:00:00.000000 buckaroo-0.3.3/buckaroo/df_methods.py
+-rw-r--r--   0        0        0     1786 2020-02-02 00:00:00.000000 buckaroo-0.3.3/buckaroo/index.html
+-rw-r--r--   0        0        0    17284 2020-02-02 00:00:00.000000 buckaroo-0.3.3/buckaroo/lispy.py
+-rw-r--r--   0        0        0     7577 2020-02-02 00:00:00.000000 buckaroo-0.3.3/buckaroo/summary_stats.py
+-rw-r--r--   0        0        0     2707 2020-02-02 00:00:00.000000 buckaroo-0.3.3/buckaroo/views.py
+-rw-r--r--   0        0        0     5513 2020-02-02 00:00:00.000000 buckaroo-0.3.3/buckaroo/labextension/package.json
+-rw-r--r--   0        0        0   145367 2020-02-02 00:00:00.000000 buckaroo-0.3.3/buckaroo/labextension/static/0.c008020c7e2133e6c7db.js
+-rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 buckaroo-0.3.3/buckaroo/labextension/static/0.c008020c7e2133e6c7db.js.LICENSE.txt
+-rw-r--r--   0        0        0    35455 2020-02-02 00:00:00.000000 buckaroo-0.3.3/buckaroo/labextension/static/399.252405500e4886745cf0.js
+-rw-r--r--   0        0        0   231664 2020-02-02 00:00:00.000000 buckaroo-0.3.3/buckaroo/labextension/static/41.dea207301743f71053c5.js
+-rw-r--r--   0        0        0     1153 2020-02-02 00:00:00.000000 buckaroo-0.3.3/buckaroo/labextension/static/480.c541de2b54a15c8f7330.js
+-rw-r--r--   0        0        0    70484 2020-02-02 00:00:00.000000 buckaroo-0.3.3/buckaroo/labextension/static/486.f08778dfb765d893ceaf.js
+-rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 buckaroo-0.3.3/buckaroo/labextension/static/486.f08778dfb765d893ceaf.js.LICENSE.txt
+-rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 buckaroo-0.3.3/buckaroo/labextension/static/568.50d29d049ddb62602cc0.js
+-rw-r--r--   0        0        0  1067038 2020-02-02 00:00:00.000000 buckaroo-0.3.3/buckaroo/labextension/static/731.d4bf968c7a94633ef5a3.js
+-rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 buckaroo-0.3.3/buckaroo/labextension/static/731.d4bf968c7a94633ef5a3.js.LICENSE.txt
+-rw-r--r--   0        0        0   139612 2020-02-02 00:00:00.000000 buckaroo-0.3.3/buckaroo/labextension/static/935.2832d17fef97c1ec6694.js
+-rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 buckaroo-0.3.3/buckaroo/labextension/static/935.2832d17fef97c1ec6694.js.LICENSE.txt
+-rw-r--r--   0        0        0     7838 2020-02-02 00:00:00.000000 buckaroo-0.3.3/buckaroo/labextension/static/remoteEntry.25db2035d9cfb129895d.js
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 buckaroo-0.3.3/buckaroo/labextension/static/style.js
+-rw-r--r--   0        0        0    11965 2020-02-02 00:00:00.000000 buckaroo-0.3.3/buckaroo/labextension/static/third-party-licenses.json
+-rw-r--r--   0        0        0  1691110 2020-02-02 00:00:00.000000 buckaroo-0.3.3/buckaroo/nbextension/index.js
+-rw-r--r--   0        0        0     2019 2020-02-02 00:00:00.000000 buckaroo-0.3.3/buckaroo/nbextension/index.js.LICENSE.txt
+-rw-r--r--   0        0        0  5896429 2020-02-02 00:00:00.000000 buckaroo-0.3.3/buckaroo/nbextension/index.js.map
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 buckaroo-0.3.3/buckaroo/noarch/current_repodata.json
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 buckaroo-0.3.3/buckaroo/noarch/current_repodata.json.bz2
+-rw-r--r--   0        0        0     2400 2020-02-02 00:00:00.000000 buckaroo-0.3.3/buckaroo/noarch/index.html
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 buckaroo-0.3.3/buckaroo/noarch/repodata.json
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 buckaroo-0.3.3/buckaroo/noarch/repodata.json.bz2
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 buckaroo-0.3.3/buckaroo/noarch/repodata_from_packages.json
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 buckaroo-0.3.3/buckaroo/noarch/repodata_from_packages.json.bz2
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 buckaroo-0.3.3/docs/Makefile
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 buckaroo-0.3.3/docs/make.bat
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 buckaroo-0.3.3/docs/source/.#nodejs-download.html -> paddy@Paddys-MacBook-Air.local.405
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 buckaroo-0.3.3/docs/source/.#vs-code-download.html -> paddy@Paddys-MacBook-Air.local.405
+-rw-r--r--   0        0        0     5575 2020-02-02 00:00:00.000000 buckaroo-0.3.3/docs/source/FAQ.rst
+-rw-r--r--   0        0        0      928 2020-02-02 00:00:00.000000 buckaroo-0.3.3/docs/source/conf.py
+-rw-r--r--   0        0        0     4104 2020-02-02 00:00:00.000000 buckaroo-0.3.3/docs/source/contributing.rst
+-rw-r--r--   0        0        0     1422 2020-02-02 00:00:00.000000 buckaroo-0.3.3/docs/source/index.rst
+-rwxr-xr-x   0        0        0      295 2020-02-02 00:00:00.000000 buckaroo-0.3.3/docs/source/install.rst
+-rw-r--r--   0        0        0     3404 2020-02-02 00:00:00.000000 buckaroo-0.3.3/docs/source/using.rst
+-rw-r--r--   0        0        0     2019 2020-02-02 00:00:00.000000 buckaroo-0.3.3/docs/source/_static/embed-bundle.js.LICENSE.txt
+-rw-r--r--   0        0        0     7144 2020-02-02 00:00:00.000000 buckaroo-0.3.3/example-notebooks/testcases-fast.ipynb
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 buckaroo-0.3.3/js/comp1.tsx
+-rw-r--r--   0        0        0     3330 2020-02-02 00:00:00.000000 buckaroo-0.3.3/js/dcefwidget.ts
+-rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 buckaroo-0.3.3/js/extension.ts
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 buckaroo-0.3.3/js/index.ts
+-rw-r--r--   0        0        0     1268 2020-02-02 00:00:00.000000 buckaroo-0.3.3/js/plugin.ts
+-rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 buckaroo-0.3.3/js/version.ts
+-rw-r--r--   0        0        0     2179 2020-02-02 00:00:00.000000 buckaroo-0.3.3/js/components/ColumnsEditor.tsx
+-rw-r--r--   0        0        0     1033 2020-02-02 00:00:00.000000 buckaroo-0.3.3/js/components/CommandUtils.ts
+-rw-r--r--   0        0        0     2849 2020-02-02 00:00:00.000000 buckaroo-0.3.3/js/components/DCFCell.tsx
+-rw-r--r--   0        0        0     4520 2020-02-02 00:00:00.000000 buckaroo-0.3.3/js/components/DFViewer.tsx
+-rw-r--r--   0        0        0     3617 2020-02-02 00:00:00.000000 buckaroo-0.3.3/js/components/DependentTabs.tsx
+-rw-r--r--   0        0        0     4875 2020-02-02 00:00:00.000000 buckaroo-0.3.3/js/components/OperationDetail.tsx
+-rw-r--r--   0        0        0     1178 2020-02-02 00:00:00.000000 buckaroo-0.3.3/js/components/OperationUtils.ts
+-rw-r--r--   0        0        0     6989 2020-02-02 00:00:00.000000 buckaroo-0.3.3/js/components/Operations.tsx
+-rw-r--r--   0        0        0     3422 2020-02-02 00:00:00.000000 buckaroo-0.3.3/js/components/StatusBar.tsx
+-rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 buckaroo-0.3.3/js/components/bakedOperationDefaults.ts
+-rw-r--r--   0        0        0     3002 2020-02-02 00:00:00.000000 buckaroo-0.3.3/js/components/gridUtils.ts
+-rw-r--r--   0        0        0     6305 2020-02-02 00:00:00.000000 buckaroo-0.3.3/js/components/staticData.ts
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 buckaroo-0.3.3/js/components/utils.ts
+-rw-r--r--   0        0        0     3026 2020-02-02 00:00:00.000000 buckaroo-0.3.3/js/style/dcf-npm.css
+-rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 buckaroo-0.3.3/js/style/icons/arrow-down-short-dark.svg
+-rwxr-xr-x   0        0        0      416 2020-02-02 00:00:00.000000 buckaroo-0.3.3/js/style/icons/arrow-down-short.svg
+-rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 buckaroo-0.3.3/js/style/icons/arrow-up-short-dark.svg
+-rwxr-xr-x   0        0        0      400 2020-02-02 00:00:00.000000 buckaroo-0.3.3/js/style/icons/arrow-up-short.svg
+-rwxr-xr-x   0        0        0      349 2020-02-02 00:00:00.000000 buckaroo-0.3.3/js/style/icons/filter-dark.svg
+-rwxr-xr-x   0        0        0      349 2020-02-02 00:00:00.000000 buckaroo-0.3.3/js/style/icons/filter.svg
+-rw-r--r--   0        0        0  1420117 2020-02-02 00:00:00.000000 buckaroo-0.3.3/static/images/Buckaroo-screenshot.png
+-rw-r--r--   0        0        0     2093 2020-02-02 00:00:00.000000 buckaroo-0.3.3/.gitignore
+-rw-r--r--   0        0        0     1494 2020-02-02 00:00:00.000000 buckaroo-0.3.3/LICENSE.txt
+-rw-r--r--   0        0        0    10241 2020-02-02 00:00:00.000000 buckaroo-0.3.3/README.md
+-rw-r--r--   0        0        0     3221 2020-02-02 00:00:00.000000 buckaroo-0.3.3/pyproject.toml
+-rw-r--r--   0        0        0    13091 2020-02-02 00:00:00.000000 buckaroo-0.3.3/PKG-INFO
```

### Comparing `buckaroo-0.3.2/RELEASE.md` & `buckaroo-0.3.3/RELEASE.md`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.2/bike-share-data-explore.ipynb` & `buckaroo-0.3.3/bike-share-data-explore.ipynb`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.2/col-ordering.ipynb` & `buckaroo-0.3.3/col-ordering.ipynb`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.2/gbfs-play.ipynb` & `buckaroo-0.3.3/gbfs-play.ipynb`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.2/gbfs-play2.ipynb` & `buckaroo-0.3.3/gbfs-play2.ipynb`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.2/introduction.ipynb` & `buckaroo-0.3.3/introduction.ipynb`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.2/package-lock.json` & `buckaroo-0.3.3/package-lock.json`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.2/package.json` & `buckaroo-0.3.3/package.json`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.2/package.json.old` & `buckaroo-0.3.3/package.json.old`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.2/tryit.ipynb` & `buckaroo-0.3.3/tryit.ipynb`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.2/tsconfig.json` & `buckaroo-0.3.3/tsconfig.json`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.2/webpack.config.js` & `buckaroo-0.3.3/webpack.config.js`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.2/yarn.lock` & `buckaroo-0.3.3/yarn.lock`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.2/buckaroo/__init__.py` & `buckaroo-0.3.3/buckaroo/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-
+from .buckaroo_widget import BuckarooWidget, enable, disable
 
 dest = 'buckaroo-labextension'
 def _jupyter_labextension_paths():
     """Called by Jupyter Lab Server to detect if it is a valid labextension and
     to install the widget
     Returns
     =======
@@ -39,8 +39,9 @@
     return [{
         'section': 'notebook',
         'src': 'nbextension',
         'dest': dest,
         'require': '%s/extension' % dest
     }]
 
-from .buckaroo_widget import BuckarooWidget, enable, disable
+
+enable()
```

### Comparing `buckaroo-0.3.2/buckaroo/all_transforms.py` & `buckaroo-0.3.3/buckaroo/all_transforms.py`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.2/buckaroo/buckaroo_widget.py` & `buckaroo-0.3.3/buckaroo/buckaroo_widget.py`

 * *Files 3% similar despite different names*

```diff
@@ -55,34 +55,34 @@
     operation_results = Dict({}).tag(sync=True)
 
 
     dfConfig = Dict(
         {
         'totalRows': 1234569,
         'columns': 30,
-        'rowsShown': 500,
+        'rowsShown': 0,
         'sampleSize': 10_000,
         'sampled':False,
         'summaryStats': False,
-        'reorderdColumns': True,
+        'reorderdColumns': False,
         'showTransformed': True,
         'showCommands': True,
     }).tag(sync=True)
         
 
     summary_df_cols = [
         'dtype', 'length', 'nan_count', 'distinct_count', 'empty_count',
         'empty_per', 'unique_per', 'nan_per', 'is_numeric', 'is_integer',
         'is_datetime', 'mode', 'min', 'max','mean',
         ]
     
     def __init__(self, df,
                  sampled=True,
                  summaryStats=False,
-                 reorderdColumns=True,
+                 reorderdColumns=False,
                  showTransformed=True,
                  showCommands=True,
                  really_reorder_columns=False):
         super().__init__()
 
         rows = len(df)
         cols = len(df.columns)
@@ -185,20 +185,18 @@
         raise ImportError('This feature requires IPython 1.0+')
 
     ip = get_ipython()
     ip_formatter = ip.display_formatter.ipython_display_formatter
 
     ip_formatter.for_type(pd.DataFrame, _display_as_buckaroo)
     
-enable()
 
 def disable():
     """
-    Automatically use buckaroo to display all DataFrames
-    instances in the notebook.
+    disable bucakroo as the default display method for DataFrames
 
     """
     try:
         from IPython.core.getipython import get_ipython
     except ImportError:
         raise ImportError('This feature requires IPython 1.0+')
```

### Comparing `buckaroo-0.3.2/buckaroo/configure_utils.py` & `buckaroo-0.3.3/buckaroo/configure_utils.py`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.2/buckaroo/dcf_transform.py` & `buckaroo-0.3.3/buckaroo/dcf_transform.py`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.2/buckaroo/df_methods.py` & `buckaroo-0.3.3/buckaroo/df_methods.py`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.2/buckaroo/index.html` & `buckaroo-0.3.3/buckaroo/index.html`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.2/buckaroo/lispy.py` & `buckaroo-0.3.3/buckaroo/lispy.py`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.2/buckaroo/summary_stats.py` & `buckaroo-0.3.3/buckaroo/summary_stats.py`

 * *Files 0% similar despite different names*

```diff
@@ -201,15 +201,15 @@
     sdf = df.sample(np.min([sample_size, len(df)]))
     if include_outliers:
         outlier_idxs = []
         for col in df.columns:
             outlier_idxs.extend(get_outlier_idxs(df[col]) )
         outlier_idxs.extend(sdf.index)
         uniq_idx = np.unique(outlier_idxs)
-        return df.iloc[uniq_idx]
+        return df.loc[uniq_idx]
     return sdf
 
 def add_col_rankings(df, sdf):
     sdf.loc['one_distinct'] = 0
 
     only_ones = (sdf.loc['distinct_count'] <= 1)
     sdf.loc['one_distinct', only_ones[only_ones==True].index.values] = -20
```

### Comparing `buckaroo-0.3.2/buckaroo/views.py` & `buckaroo-0.3.3/buckaroo/views.py`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.2/buckaroo/labextension/package.json` & `buckaroo-0.3.3/buckaroo/labextension/package.json`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.2/buckaroo/labextension/static/0.c008020c7e2133e6c7db.js` & `buckaroo-0.3.3/buckaroo/labextension/static/0.c008020c7e2133e6c7db.js`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.2/buckaroo/labextension/static/0.c008020c7e2133e6c7db.js.LICENSE.txt` & `buckaroo-0.3.3/buckaroo/labextension/static/0.c008020c7e2133e6c7db.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.2/buckaroo/labextension/static/399.252405500e4886745cf0.js` & `buckaroo-0.3.3/buckaroo/labextension/static/399.252405500e4886745cf0.js`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.2/buckaroo/labextension/static/41.dea207301743f71053c5.js` & `buckaroo-0.3.3/buckaroo/labextension/static/41.dea207301743f71053c5.js`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.2/buckaroo/labextension/static/480.c541de2b54a15c8f7330.js` & `buckaroo-0.3.3/buckaroo/labextension/static/480.c541de2b54a15c8f7330.js`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.2/buckaroo/labextension/static/486.f08778dfb765d893ceaf.js` & `buckaroo-0.3.3/buckaroo/labextension/static/486.f08778dfb765d893ceaf.js`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.2/buckaroo/labextension/static/568.50d29d049ddb62602cc0.js` & `buckaroo-0.3.3/buckaroo/labextension/static/568.50d29d049ddb62602cc0.js`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.2/buckaroo/labextension/static/731.d4bf968c7a94633ef5a3.js` & `buckaroo-0.3.3/buckaroo/labextension/static/731.d4bf968c7a94633ef5a3.js`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.2/buckaroo/labextension/static/935.2832d17fef97c1ec6694.js` & `buckaroo-0.3.3/buckaroo/labextension/static/935.2832d17fef97c1ec6694.js`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.2/buckaroo/labextension/static/935.2832d17fef97c1ec6694.js.LICENSE.txt` & `buckaroo-0.3.3/buckaroo/labextension/static/935.2832d17fef97c1ec6694.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.2/buckaroo/labextension/static/remoteEntry.25db2035d9cfb129895d.js` & `buckaroo-0.3.3/buckaroo/labextension/static/remoteEntry.25db2035d9cfb129895d.js`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.2/buckaroo/labextension/static/third-party-licenses.json` & `buckaroo-0.3.3/buckaroo/labextension/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.2/buckaroo/nbextension/index.js` & `buckaroo-0.3.3/buckaroo/nbextension/index.js`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.2/buckaroo/nbextension/index.js.LICENSE.txt` & `buckaroo-0.3.3/buckaroo/nbextension/index.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.2/buckaroo/nbextension/index.js.map` & `buckaroo-0.3.3/buckaroo/nbextension/index.js.map`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.2/buckaroo/noarch/index.html` & `buckaroo-0.3.3/buckaroo/noarch/index.html`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.2/docs/Makefile` & `buckaroo-0.3.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.2/docs/make.bat` & `buckaroo-0.3.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.2/docs/source/FAQ.rst` & `buckaroo-0.3.3/docs/source/FAQ.rst`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.2/docs/source/conf.py` & `buckaroo-0.3.3/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.2/docs/source/contributing.rst` & `buckaroo-0.3.3/docs/source/contributing.rst`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.2/docs/source/index.rst` & `buckaroo-0.3.3/docs/source/index.rst`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 Buckaroo is a tool to quickly clean and explore DataFrames with a visual UI for common cleaning operations AND emitting python code that performs the transformation. 
 
 
 We all know how awkward it is to clean data in jupyter notebooks.  Multiple cells of exploratory work, trying different transforms, looking up different transforms, adhoc functions that work in one notebook and have to be either copied/pasta-ed to the next notebook, or rewritten from scratch.  Buckaroo aims to massively speed up that process.
 
 .. raw:: html
 
-	 <iframe width="560" height="315" src="https://www.youtube.com/embed/4Wbm2OcrD7U" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>
+	 <iframe width="560" height="315" src="https://www.youtube.com/embed/3XdU5hpOUYY" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>
 
 
 
 .. note::
 
    This project is under active development.
```

### Comparing `buckaroo-0.3.2/docs/source/using.rst` & `buckaroo-0.3.3/docs/source/using.rst`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.2/docs/source/_static/embed-bundle.js.LICENSE.txt` & `buckaroo-0.3.3/docs/source/_static/embed-bundle.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.2/example-notebooks/testcases-fast.ipynb` & `buckaroo-0.3.3/example-notebooks/testcases-fast.ipynb`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.2/js/dcefwidget.ts` & `buckaroo-0.3.3/js/dcefwidget.ts`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.2/js/extension.ts` & `buckaroo-0.3.3/js/extension.ts`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.2/js/plugin.ts` & `buckaroo-0.3.3/js/plugin.ts`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.2/js/components/ColumnsEditor.tsx` & `buckaroo-0.3.3/js/components/ColumnsEditor.tsx`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.2/js/components/CommandUtils.ts` & `buckaroo-0.3.3/js/components/CommandUtils.ts`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.2/js/components/DCFCell.tsx` & `buckaroo-0.3.3/js/components/DCFCell.tsx`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.2/js/components/DFViewer.tsx` & `buckaroo-0.3.3/js/components/DFViewer.tsx`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.2/js/components/DependentTabs.tsx` & `buckaroo-0.3.3/js/components/DependentTabs.tsx`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.2/js/components/OperationDetail.tsx` & `buckaroo-0.3.3/js/components/OperationDetail.tsx`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.2/js/components/OperationUtils.ts` & `buckaroo-0.3.3/js/components/OperationUtils.ts`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.2/js/components/Operations.tsx` & `buckaroo-0.3.3/js/components/Operations.tsx`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.2/js/components/StatusBar.tsx` & `buckaroo-0.3.3/js/components/StatusBar.tsx`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.2/js/components/gridUtils.ts` & `buckaroo-0.3.3/js/components/gridUtils.ts`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.2/js/components/staticData.ts` & `buckaroo-0.3.3/js/components/staticData.ts`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.2/js/components/utils.ts` & `buckaroo-0.3.3/js/components/utils.ts`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.2/js/style/dcf-npm.css` & `buckaroo-0.3.3/js/style/dcf-npm.css`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.2/static/images/Buckaroo-screenshot.png` & `buckaroo-0.3.3/static/images/Buckaroo-screenshot.png`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.2/.gitignore` & `buckaroo-0.3.3/.gitignore`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.2/LICENSE.txt` & `buckaroo-0.3.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.2/README.md` & `buckaroo-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `buckaroo-0.3.2/pyproject.toml` & `buckaroo-0.3.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
 ]
 dependencies = [
     "ipywidgets>=7.6.0,<9"
 ]
-version = "0.3.2"
+version = "0.3.3"
 
 [project.license]
 file = "LICENSE.txt"
 
 [project.optional-dependencies]
 test = [
     "nbval>=0.9",
```

### Comparing `buckaroo-0.3.2/PKG-INFO` & `buckaroo-0.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: buckaroo
-Version: 0.3.2
+Version: 0.3.3
 Summary: Buckaroo - GUI Data wrangling for pandas
 Project-URL: Homepage, https://github.com/paddymul/buckaroo
 Author: Paddy Mullen
 License: Copyright (c) 2019 Bloomberg
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without
```

