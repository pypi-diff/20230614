# Comparing `tmp/ai_services-0.5.0rc8.tar.gz` & `tmp/ai_services-0.5.0rc9.tar.gz`

## Comparing `ai_services-0.5.0rc8.tar` & `ai_services-0.5.0rc9.tar`

### file list

```diff
@@ -1,254 +1,247 @@
--rw-r--r--   0        0        0     5930 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/.dockerignore
--rw-r--r--   0        0        0    20893 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/.pylintrc
--rw-r--r--   0        0        0     1473 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/Makefile
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/mypy.ini
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/py.typed
--rw-r--r--   0        0        0     1881 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/.venv/ai-services/lib/python3.8/site-packages/alabaster/about.html
--rw-r--r--   0        0        0      866 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/.venv/ai-services/lib/python3.8/site-packages/alabaster/donate.html
--rw-r--r--   0        0        0     4285 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/.venv/ai-services/lib/python3.8/site-packages/alabaster/layout.html
--rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/.venv/ai-services/lib/python3.8/site-packages/alabaster/navigation.html
--rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/.venv/ai-services/lib/python3.8/site-packages/alabaster/relations.html
--rw-r--r--   0        0        0     3137 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/.venv/ai-services/lib/python3.8/site-packages/alembic/templates/async/alembic.ini.mako
--rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/.venv/ai-services/lib/python3.8/site-packages/alembic/templates/async/script.py.mako
--rw-r--r--   0        0        0     3246 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/.venv/ai-services/lib/python3.8/site-packages/alembic/templates/generic/alembic.ini.mako
--rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/.venv/ai-services/lib/python3.8/site-packages/alembic/templates/generic/script.py.mako
--rw-r--r--   0        0        0     3340 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/.venv/ai-services/lib/python3.8/site-packages/alembic/templates/multidb/alembic.ini.mako
--rw-r--r--   0        0        0      965 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/.venv/ai-services/lib/python3.8/site-packages/alembic/templates/multidb/script.py.mako
--rw-r--r--   0        0        0     5400 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/.venv/ai-services/lib/python3.8/site-packages/coverage/htmlfiles/index.html
--rw-r--r--   0        0        0     6437 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/.venv/ai-services/lib/python3.8/site-packages/coverage/htmlfiles/pyfile.html
--rw-r--r--   0        0        0    26094 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/.venv/ai-services/lib/python3.8/site-packages/docutils-0.18.1.dist-info/SOURCES.html
--rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/.venv/ai-services/lib/python3.8/site-packages/docutils-0.18.1.dist-info/dependency_links.html
--rw-r--r--   0        0        0      969 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/.venv/ai-services/lib/python3.8/site-packages/docutils-0.18.1.dist-info/top_level.html
--rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/.venv/ai-services/lib/python3.8/site-packages/sanic_ext/extensions/openapi/ui/redoc.html
--rw-r--r--   0        0        0     1477 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/.venv/ai-services/lib/python3.8/site-packages/sanic_ext/extensions/openapi/ui/swagger.html
--rw-r--r--   0        0        0     3321 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/.venv/ai-services/lib/python3.8/site-packages/sphinx/themes/agogo/layout.html
--rw-r--r--   0        0        0     1636 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/.venv/ai-services/lib/python3.8/site-packages/sphinx/themes/basic/defindex.html
--rw-r--r--   0        0        0     1892 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/.venv/ai-services/lib/python3.8/site-packages/sphinx/themes/basic/domainindex.html
--rw-r--r--   0        0        0     1804 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/.venv/ai-services/lib/python3.8/site-packages/sphinx/themes/basic/genindex-single.html
--rw-r--r--   0        0        0     1210 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/.venv/ai-services/lib/python3.8/site-packages/sphinx/themes/basic/genindex-split.html
--rw-r--r--   0        0        0     2069 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/.venv/ai-services/lib/python3.8/site-packages/sphinx/themes/basic/genindex.html
--rw-r--r--   0        0        0      432 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/.venv/ai-services/lib/python3.8/site-packages/sphinx/themes/basic/globaltoc.html
--rw-r--r--   0        0        0     7682 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/.venv/ai-services/lib/python3.8/site-packages/sphinx/themes/basic/layout.html
--rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/.venv/ai-services/lib/python3.8/site-packages/sphinx/themes/basic/localtoc.html
--rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/.venv/ai-services/lib/python3.8/site-packages/sphinx/themes/basic/page.html
--rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/.venv/ai-services/lib/python3.8/site-packages/sphinx/themes/basic/relations.html
--rw-r--r--   0        0        0     2039 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/.venv/ai-services/lib/python3.8/site-packages/sphinx/themes/basic/search.html
--rw-r--r--   0        0        0      809 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/.venv/ai-services/lib/python3.8/site-packages/sphinx/themes/basic/searchbox.html
--rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/.venv/ai-services/lib/python3.8/site-packages/sphinx/themes/basic/sourcelink.html
--rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/.venv/ai-services/lib/python3.8/site-packages/sphinx/themes/basic/changes/frameset.html
--rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/.venv/ai-services/lib/python3.8/site-packages/sphinx/themes/basic/changes/rstsource.html
--rw-r--r--   0        0        0     1306 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/.venv/ai-services/lib/python3.8/site-packages/sphinx/themes/basic/changes/versionchanges.html
--rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/.venv/ai-services/lib/python3.8/site-packages/sphinx/themes/bizstyle/layout.html
--rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/.venv/ai-services/lib/python3.8/site-packages/sphinx/themes/classic/layout.html
--rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/.venv/ai-services/lib/python3.8/site-packages/sphinx/themes/epub/epub-cover.html
--rw-r--r--   0        0        0      543 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/.venv/ai-services/lib/python3.8/site-packages/sphinx/themes/epub/layout.html
--rw-r--r--   0        0        0     2012 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/.venv/ai-services/lib/python3.8/site-packages/sphinx/themes/haiku/layout.html
--rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/.venv/ai-services/lib/python3.8/site-packages/sphinx/themes/nonav/layout.html
--rw-r--r--   0        0        0      875 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/.venv/ai-services/lib/python3.8/site-packages/sphinx/themes/pyramid/layout.html
--rw-r--r--   0        0        0     1661 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/.venv/ai-services/lib/python3.8/site-packages/sphinx/themes/scrolls/layout.html
--rw-r--r--   0        0        0     4277 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/.venv/ai-services/lib/python3.8/site-packages/sphinx_rtd_theme/breadcrumbs.html
--rw-r--r--   0        0        0     2915 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/.venv/ai-services/lib/python3.8/site-packages/sphinx_rtd_theme/footer.html
--rw-r--r--   0        0        0     9716 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/.venv/ai-services/lib/python3.8/site-packages/sphinx_rtd_theme/layout.html
--rw-r--r--   0        0        0     1759 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/.venv/ai-services/lib/python3.8/site-packages/sphinx_rtd_theme/search.html
--rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/.venv/ai-services/lib/python3.8/site-packages/sphinx_rtd_theme/searchbox.html
--rw-r--r--   0        0        0     1247 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/.venv/ai-services/lib/python3.8/site-packages/sphinx_rtd_theme/versions.html
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/.venv/ai-services/lib/python3.8/site-packages/tornado/test/static/dir/index.html
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/.venv/ai-services/lib/python3.8/site-packages/tornado/test/templates/utf8.html
--rw-r--r--   0        0        0     1881 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/dist/ai_services-0.4.1/.venv/lib/python3.8/site-packages/alabaster/about.html
--rw-r--r--   0        0        0      866 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/dist/ai_services-0.4.1/.venv/lib/python3.8/site-packages/alabaster/donate.html
--rw-r--r--   0        0        0     4285 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/dist/ai_services-0.4.1/.venv/lib/python3.8/site-packages/alabaster/layout.html
--rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/dist/ai_services-0.4.1/.venv/lib/python3.8/site-packages/alabaster/navigation.html
--rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/dist/ai_services-0.4.1/.venv/lib/python3.8/site-packages/alabaster/relations.html
--rw-r--r--   0        0        0     5400 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/dist/ai_services-0.4.1/.venv/lib/python3.8/site-packages/coverage/htmlfiles/index.html
--rw-r--r--   0        0        0     6437 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/dist/ai_services-0.4.1/.venv/lib/python3.8/site-packages/coverage/htmlfiles/pyfile.html
--rw-r--r--   0        0        0    26094 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/dist/ai_services-0.4.1/.venv/lib/python3.8/site-packages/docutils-0.17.1.dist-info/SOURCES.html
--rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/dist/ai_services-0.4.1/.venv/lib/python3.8/site-packages/docutils-0.17.1.dist-info/dependency_links.html
--rw-r--r--   0        0        0      969 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/dist/ai_services-0.4.1/.venv/lib/python3.8/site-packages/docutils-0.17.1.dist-info/top_level.html
--rw-r--r--   0        0        0     1620 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/dist/ai_services-0.4.1/.venv/lib/python3.8/site-packages/matplotlib/backends/web_backend/all_figures.html
--rw-r--r--   0        0        0     1311 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/dist/ai_services-0.4.1/.venv/lib/python3.8/site-packages/matplotlib/backends/web_backend/ipython_inline_figure.html
--rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/dist/ai_services-0.4.1/.venv/lib/python3.8/site-packages/matplotlib/backends/web_backend/single_figure.html
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/dist/ai_services-0.4.1/.venv/lib/python3.8/site-packages/numpy/core/lib/npy-pkg-config/mlib.ini
--rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/dist/ai_services-0.4.1/.venv/lib/python3.8/site-packages/numpy/core/lib/npy-pkg-config/npymath.ini
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/dist/ai_services-0.4.1/.venv/lib/python3.8/site-packages/numpy/typing/tests/data/mypy.ini
--rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/dist/ai_services-0.4.1/.venv/lib/python3.8/site-packages/sanic_ext/extensions/openapi/ui/redoc.html
--rw-r--r--   0        0        0     1530 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/dist/ai_services-0.4.1/.venv/lib/python3.8/site-packages/sanic_ext/extensions/openapi/ui/swagger.html
--rw-r--r--   0        0        0     3303 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/dist/ai_services-0.4.1/.venv/lib/python3.8/site-packages/sphinx/themes/agogo/layout.html
--rw-r--r--   0        0        0     1636 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/dist/ai_services-0.4.1/.venv/lib/python3.8/site-packages/sphinx/themes/basic/defindex.html
--rw-r--r--   0        0        0     1892 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/dist/ai_services-0.4.1/.venv/lib/python3.8/site-packages/sphinx/themes/basic/domainindex.html
--rw-r--r--   0        0        0     1804 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/dist/ai_services-0.4.1/.venv/lib/python3.8/site-packages/sphinx/themes/basic/genindex-single.html
--rw-r--r--   0        0        0     1210 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/dist/ai_services-0.4.1/.venv/lib/python3.8/site-packages/sphinx/themes/basic/genindex-split.html
--rw-r--r--   0        0        0     2069 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/dist/ai_services-0.4.1/.venv/lib/python3.8/site-packages/sphinx/themes/basic/genindex.html
--rw-r--r--   0        0        0      432 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/dist/ai_services-0.4.1/.venv/lib/python3.8/site-packages/sphinx/themes/basic/globaltoc.html
--rw-r--r--   0        0        0     7633 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/dist/ai_services-0.4.1/.venv/lib/python3.8/site-packages/sphinx/themes/basic/layout.html
--rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/dist/ai_services-0.4.1/.venv/lib/python3.8/site-packages/sphinx/themes/basic/localtoc.html
--rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/dist/ai_services-0.4.1/.venv/lib/python3.8/site-packages/sphinx/themes/basic/page.html
--rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/dist/ai_services-0.4.1/.venv/lib/python3.8/site-packages/sphinx/themes/basic/relations.html
--rw-r--r--   0        0        0     2039 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/dist/ai_services-0.4.1/.venv/lib/python3.8/site-packages/sphinx/themes/basic/search.html
--rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/dist/ai_services-0.4.1/.venv/lib/python3.8/site-packages/sphinx/themes/basic/searchbox.html
--rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/dist/ai_services-0.4.1/.venv/lib/python3.8/site-packages/sphinx/themes/basic/sourcelink.html
--rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/dist/ai_services-0.4.1/.venv/lib/python3.8/site-packages/sphinx/themes/basic/changes/frameset.html
--rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/dist/ai_services-0.4.1/.venv/lib/python3.8/site-packages/sphinx/themes/basic/changes/rstsource.html
--rw-r--r--   0        0        0     1306 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/dist/ai_services-0.4.1/.venv/lib/python3.8/site-packages/sphinx/themes/basic/changes/versionchanges.html
--rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/dist/ai_services-0.4.1/.venv/lib/python3.8/site-packages/sphinx/themes/bizstyle/layout.html
--rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/dist/ai_services-0.4.1/.venv/lib/python3.8/site-packages/sphinx/themes/classic/layout.html
--rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/dist/ai_services-0.4.1/.venv/lib/python3.8/site-packages/sphinx/themes/epub/epub-cover.html
--rw-r--r--   0        0        0      543 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/dist/ai_services-0.4.1/.venv/lib/python3.8/site-packages/sphinx/themes/epub/layout.html
--rw-r--r--   0        0        0     2012 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/dist/ai_services-0.4.1/.venv/lib/python3.8/site-packages/sphinx/themes/haiku/layout.html
--rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/dist/ai_services-0.4.1/.venv/lib/python3.8/site-packages/sphinx/themes/nonav/layout.html
--rw-r--r--   0        0        0      875 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/dist/ai_services-0.4.1/.venv/lib/python3.8/site-packages/sphinx/themes/pyramid/layout.html
--rw-r--r--   0        0        0     1661 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/dist/ai_services-0.4.1/.venv/lib/python3.8/site-packages/sphinx/themes/scrolls/layout.html
--rw-r--r--   0        0        0     4220 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/dist/ai_services-0.4.1/.venv/lib/python3.8/site-packages/sphinx_rtd_theme/breadcrumbs.html
--rw-r--r--   0        0        0     2914 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/dist/ai_services-0.4.1/.venv/lib/python3.8/site-packages/sphinx_rtd_theme/footer.html
--rw-r--r--   0        0        0     9660 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/dist/ai_services-0.4.1/.venv/lib/python3.8/site-packages/sphinx_rtd_theme/layout.html
--rw-r--r--   0        0        0     1759 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/dist/ai_services-0.4.1/.venv/lib/python3.8/site-packages/sphinx_rtd_theme/search.html
--rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/dist/ai_services-0.4.1/.venv/lib/python3.8/site-packages/sphinx_rtd_theme/searchbox.html
--rw-r--r--   0        0        0     1247 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/dist/ai_services-0.4.1/.venv/lib/python3.8/site-packages/sphinx_rtd_theme/versions.html
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/dist/ai_services-0.4.1/.venv/lib/python3.8/site-packages/tornado/test/static/dir/index.html
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/dist/ai_services-0.4.1/.venv/lib/python3.8/site-packages/tornado/test/templates/utf8.html
--rw-r--r--   0        0        0     1581 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/dist/ai_services-0.4.1/dist/ai_services-0.4.0/example/alembic.ini
--rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/dist/ai_services-0.4.1/dist/ai_services-0.4.0/example/example/templates/_layout.html
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/dist/ai_services-0.4.1/dist/ai_services-0.4.0/example/example/templates/index.html
--rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/dist/ai_services-0.4.1/dist/ai_services-0.4.0/example/front/index.html
--rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/dist/ai_services-0.4.1/dist/ai_services-0.4.0/services/files/_layout.default.html
--rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/dist/ai_services-0.4.1/dist/ai_services-0.4.0/services/files/_layout.vite.html
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/dist/ai_services-0.4.1/dist/ai_services-0.4.0/services/files/index.html
--rw-r--r--   0        0        0     1424 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/dist/ai_services-0.4.1/dist/ai_services-0.4.0/services/files/app/alembic.ini
--rw-r--r--   0        0        0     1581 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/dist/ai_services-0.4.1/example/alembic.ini
--rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/dist/ai_services-0.4.1/example/example/migrations/script.py.mako
--rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/dist/ai_services-0.4.1/example/example/templates/_layout.html
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/dist/ai_services-0.4.1/example/example/templates/index.html
--rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/dist/ai_services-0.4.1/example/front/index.html
--rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/dist/ai_services-0.4.1/services/files/_layout.default.html
--rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/dist/ai_services-0.4.1/services/files/_layout.vite.html
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/dist/ai_services-0.4.1/services/files/index.html
--rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/dist/ai_services-0.4.1/services/files/alembic/script.py.mako
--rw-r--r--   0        0        0     1424 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/dist/ai_services-0.4.1/services/files/app/alembic.ini
--rw-r--r--   0        0        0     1585 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/dist/ai_services-0.4.1/test_app/alembic.ini
--rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/dist/ai_services-0.4.1/test_app/front/index.html
--rw-r--r--   0        0        0    14075 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/dist/ai_services-0.4.1/test_app/front/node_modules/@tailwindcss/forms/index.html
--rw-r--r--   0        0        0     8148 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/dist/ai_services-0.4.1/test_app/front/node_modules/@tailwindcss/forms/kitchen-sink.html
--rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/dist/ai_services-0.4.1/test_app/test_app/templates/_layout.html
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/dist/ai_services-0.4.1/test_app/test_app/templates/index.html
--rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/docs/databases.md
--rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/docs/references.md
--rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/docs/release.md
--rw-r--r--   0        0        0     1581 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/example/alembic.ini
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/example/example/__init__.py
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/example/example/db.py
--rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/example/example/models.py
--rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/example/example/views.py
--rw-r--r--   0        0        0     1055 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/example/example/web.py
--rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/example/example/api/example.py
--rw-r--r--   0        0        0     1820 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/example/example/api/users.py
--rw-r--r--   0        0        0     2735 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/example/example/migrations/env.py
--rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/example/example/migrations/script.py.mako
--rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/example/example/templates/_layout.html
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/example/example/templates/index.html
--rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/example/front/.gitignore
--rw-r--r--   0        0        0     2903 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/example/front/README.md
--rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/example/front/index.html
--rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/example/front/jsconfig.json
--rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/example/front/package.json
--rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/example/front/svelte.config.js
--rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/example/front/vite.config.js
--rw-r--r--   0        0        0     1497 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/example/front/public/vite.svg
--rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/example/front/src/App.svelte
--rw-r--r--   0        0        0     1310 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/example/front/src/app.css
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/example/front/src/main.js
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/example/front/src/vite-env.d.ts
--rw-r--r--   0        0        0     1950 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/example/front/src/assets/svelte.svg
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/example/server_conf/__init__.py
--rw-r--r--   0        0        0     1522 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/example/server_conf/settings.py
--rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/scripts/get_version.py
--rwxr-xr-x   0        0        0      181 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/scripts/update_versions.sh
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/services/__about__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/services/__init__.py
--rw-r--r--   0        0        0     2914 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/services/base.py
--rw-r--r--   0        0        0     1777 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/services/cli.py
--rw-r--r--   0        0        0     1251 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/services/cli_project.py
--rw-r--r--   0        0        0     2352 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/services/conf.py
--rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/services/defaults.py
--rw-r--r--   0        0        0     1466 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/services/errors.py
--rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/services/global_settings.py
--rw-r--r--   0        0        0     6619 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/services/init_script.py
--rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/services/jt.py
--rw-r--r--   0        0        0     3013 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/services/redis_conn.py
--rw-r--r--   0        0        0     2693 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/services/server.py
--rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/services/shortcuts.py
--rw-r--r--   0        0        0    11682 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/services/storage.py
--rw-r--r--   0        0        0     9147 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/services/types.py
--rw-r--r--   0        0        0     1672 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/services/users.py
--rw-r--r--   0        0        0     7470 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/services/utils.py
--rw-r--r--   0        0        0    15010 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/services/workers.py
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/services/commands/__init__.py
--rw-r--r--   0        0        0     1190 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/services/commands/common.py
--rw-r--r--   0        0        0     4142 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/services/commands/db.py
--rw-r--r--   0        0        0     5298 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/services/commands/tasks.py
--rw-r--r--   0        0        0     2555 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/services/commands/web.py
--rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/services/db/__init__.py
--rw-r--r--   0        0        0     2175 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/services/db/common.py
--rw-r--r--   0        0        0     3885 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/services/db/managers.py
--rw-r--r--   0        0        0     3106 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/services/db/migration.py
--rw-r--r--   0        0        0     1832 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/services/db/pages.py
--rw-r--r--   0        0        0     2270 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/services/db/plugin.py
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/services/db/pragmas.py
--rw-r--r--   0        0        0    10305 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/services/db/sqlhelper.py
--rw-r--r--   0        0        0     1267 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/services/db/utils.py
--rw-r--r--   0        0        0     1305 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/services/db/web.py
--rw-r--r--   0        0        0     8164 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/services/ext/google.py
--rw-r--r--   0        0        0     8530 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/services/ext/sql/workers.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/services/files/__init__.py
--rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/services/files/_layout.default.html
--rw-r--r--   0        0        0     1157 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/services/files/_layout.vite.html
--rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/services/files/index.html
--rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/services/files/login.html
--rw-r--r--   0        0        0     1839 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/services/files/settings.py
--rw-r--r--   0        0        0     2746 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/services/files/alembic/env.py
--rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/services/files/alembic/script.py.mako
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/services/files/app/__init__.py
--rw-r--r--   0        0        0     1424 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/services/files/app/alembic.ini
--rw-r--r--   0        0        0     1151 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/services/files/app/api_bp.py
--rw-r--r--   0        0        0      745 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/services/files/app/db.py
--rw-r--r--   0        0        0     3132 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/services/files/app/managers.py
--rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/services/files/app/models.py
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/services/files/app/tasks.py
--rw-r--r--   0        0        0     2186 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/services/files/app/users_bp.py
--rw-r--r--   0        0        0     2181 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/services/files/app/users_models.py
--rw-r--r--   0        0        0     3048 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/services/files/app/views.py
--rw-r--r--   0        0        0     2934 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/services/files/app/web.py
--rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/services/files/app/commands/shell.py
--rw-r--r--   0        0        0     5048 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/services/files/app/commands/users.py
--rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/services/security/__init__.py
--rw-r--r--   0        0        0     1363 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/services/security/base.py
--rw-r--r--   0        0        0     6531 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/services/security/jwtauth.py
--rw-r--r--   0        0        0      964 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/services/security/memory_store.py
--rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/services/security/password.py
--rw-r--r--   0        0        0      969 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/services/security/redis_store.py
--rw-r--r--   0        0        0     1482 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/services/security/scopes.py
--rw-r--r--   0        0        0     2350 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/services/security/sessionauth.py
--rw-r--r--   0        0        0     2767 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/services/security/sql_store.py
--rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/services/security/utils.py
--rw-r--r--   0        0        0     3686 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/services/security/web.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/services/templates/__init__.py
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/services/templates/html.py
--rw-r--r--   0        0        0     4795 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/services/templates/render.py
--rw-r--r--   0        0        0     3839 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/services/templates/simple_tags.py
--rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/services/templates/static.py
--rw-r--r--   0        0        0     3222 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/services/templates/vite.py
--rw-r--r--   0        0        0     1735 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/test_app/alembic.ini
--rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/test_app/test2/migrations/script.py.mako
--rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/test_app/test2/templates/_layout.html
--rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/test_app/test2/templates/index.html
--rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/test_app/test3/templates/_layout.html
--rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/test_app/test3/templates/index.html
--rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/test_app/test4/templates/_layout.html
--rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/test_app/test4/templates/index.html
--rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/test_app/test_app/migrations/script.py.mako
--rw-r--r--   0        0        0     1157 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/test_app/test_app/templates/_layout.html
--rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/test_app/test_app/templates/index.html
--rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/test_app/test_app/templates/login.html
--rw-r--r--   0        0        0     8021 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/.gitignore
--rw-r--r--   0        0        0    15977 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/LICENSE
--rw-r--r--   0        0        0     5242 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/README.md
--rw-r--r--   0        0        0     2496 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/pyproject.toml
--rw-r--r--   0        0        0     6759 2020-02-02 00:00:00.000000 ai_services-0.5.0rc8/PKG-INFO
+-rw-r--r--   0        0        0     5930 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/.dockerignore
+-rw-r--r--   0        0        0    20893 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/.pylintrc
+-rw-r--r--   0        0        0     1473 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/Makefile
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/mypy.ini
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/py.typed
+-rw-r--r--   0        0        0     1881 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/.venv/ai-services/lib/python3.8/site-packages/alabaster/about.html
+-rw-r--r--   0        0        0      866 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/.venv/ai-services/lib/python3.8/site-packages/alabaster/donate.html
+-rw-r--r--   0        0        0     4285 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/.venv/ai-services/lib/python3.8/site-packages/alabaster/layout.html
+-rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/.venv/ai-services/lib/python3.8/site-packages/alabaster/navigation.html
+-rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/.venv/ai-services/lib/python3.8/site-packages/alabaster/relations.html
+-rw-r--r--   0        0        0     3137 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/.venv/ai-services/lib/python3.8/site-packages/alembic/templates/async/alembic.ini.mako
+-rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/.venv/ai-services/lib/python3.8/site-packages/alembic/templates/async/script.py.mako
+-rw-r--r--   0        0        0     3246 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/.venv/ai-services/lib/python3.8/site-packages/alembic/templates/generic/alembic.ini.mako
+-rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/.venv/ai-services/lib/python3.8/site-packages/alembic/templates/generic/script.py.mako
+-rw-r--r--   0        0        0     3340 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/.venv/ai-services/lib/python3.8/site-packages/alembic/templates/multidb/alembic.ini.mako
+-rw-r--r--   0        0        0      965 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/.venv/ai-services/lib/python3.8/site-packages/alembic/templates/multidb/script.py.mako
+-rw-r--r--   0        0        0     5400 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/.venv/ai-services/lib/python3.8/site-packages/coverage/htmlfiles/index.html
+-rw-r--r--   0        0        0     6437 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/.venv/ai-services/lib/python3.8/site-packages/coverage/htmlfiles/pyfile.html
+-rw-r--r--   0        0        0    26094 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/.venv/ai-services/lib/python3.8/site-packages/docutils-0.18.1.dist-info/SOURCES.html
+-rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/.venv/ai-services/lib/python3.8/site-packages/docutils-0.18.1.dist-info/dependency_links.html
+-rw-r--r--   0        0        0      969 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/.venv/ai-services/lib/python3.8/site-packages/docutils-0.18.1.dist-info/top_level.html
+-rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/.venv/ai-services/lib/python3.8/site-packages/sanic_ext/extensions/openapi/ui/redoc.html
+-rw-r--r--   0        0        0     1477 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/.venv/ai-services/lib/python3.8/site-packages/sanic_ext/extensions/openapi/ui/swagger.html
+-rw-r--r--   0        0        0     3321 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/.venv/ai-services/lib/python3.8/site-packages/sphinx/themes/agogo/layout.html
+-rw-r--r--   0        0        0     1636 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/.venv/ai-services/lib/python3.8/site-packages/sphinx/themes/basic/defindex.html
+-rw-r--r--   0        0        0     1892 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/.venv/ai-services/lib/python3.8/site-packages/sphinx/themes/basic/domainindex.html
+-rw-r--r--   0        0        0     1804 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/.venv/ai-services/lib/python3.8/site-packages/sphinx/themes/basic/genindex-single.html
+-rw-r--r--   0        0        0     1210 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/.venv/ai-services/lib/python3.8/site-packages/sphinx/themes/basic/genindex-split.html
+-rw-r--r--   0        0        0     2069 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/.venv/ai-services/lib/python3.8/site-packages/sphinx/themes/basic/genindex.html
+-rw-r--r--   0        0        0      432 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/.venv/ai-services/lib/python3.8/site-packages/sphinx/themes/basic/globaltoc.html
+-rw-r--r--   0        0        0     7682 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/.venv/ai-services/lib/python3.8/site-packages/sphinx/themes/basic/layout.html
+-rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/.venv/ai-services/lib/python3.8/site-packages/sphinx/themes/basic/localtoc.html
+-rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/.venv/ai-services/lib/python3.8/site-packages/sphinx/themes/basic/page.html
+-rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/.venv/ai-services/lib/python3.8/site-packages/sphinx/themes/basic/relations.html
+-rw-r--r--   0        0        0     2039 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/.venv/ai-services/lib/python3.8/site-packages/sphinx/themes/basic/search.html
+-rw-r--r--   0        0        0      809 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/.venv/ai-services/lib/python3.8/site-packages/sphinx/themes/basic/searchbox.html
+-rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/.venv/ai-services/lib/python3.8/site-packages/sphinx/themes/basic/sourcelink.html
+-rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/.venv/ai-services/lib/python3.8/site-packages/sphinx/themes/basic/changes/frameset.html
+-rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/.venv/ai-services/lib/python3.8/site-packages/sphinx/themes/basic/changes/rstsource.html
+-rw-r--r--   0        0        0     1306 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/.venv/ai-services/lib/python3.8/site-packages/sphinx/themes/basic/changes/versionchanges.html
+-rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/.venv/ai-services/lib/python3.8/site-packages/sphinx/themes/bizstyle/layout.html
+-rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/.venv/ai-services/lib/python3.8/site-packages/sphinx/themes/classic/layout.html
+-rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/.venv/ai-services/lib/python3.8/site-packages/sphinx/themes/epub/epub-cover.html
+-rw-r--r--   0        0        0      543 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/.venv/ai-services/lib/python3.8/site-packages/sphinx/themes/epub/layout.html
+-rw-r--r--   0        0        0     2012 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/.venv/ai-services/lib/python3.8/site-packages/sphinx/themes/haiku/layout.html
+-rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/.venv/ai-services/lib/python3.8/site-packages/sphinx/themes/nonav/layout.html
+-rw-r--r--   0        0        0      875 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/.venv/ai-services/lib/python3.8/site-packages/sphinx/themes/pyramid/layout.html
+-rw-r--r--   0        0        0     1661 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/.venv/ai-services/lib/python3.8/site-packages/sphinx/themes/scrolls/layout.html
+-rw-r--r--   0        0        0     4277 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/.venv/ai-services/lib/python3.8/site-packages/sphinx_rtd_theme/breadcrumbs.html
+-rw-r--r--   0        0        0     2915 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/.venv/ai-services/lib/python3.8/site-packages/sphinx_rtd_theme/footer.html
+-rw-r--r--   0        0        0     9716 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/.venv/ai-services/lib/python3.8/site-packages/sphinx_rtd_theme/layout.html
+-rw-r--r--   0        0        0     1759 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/.venv/ai-services/lib/python3.8/site-packages/sphinx_rtd_theme/search.html
+-rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/.venv/ai-services/lib/python3.8/site-packages/sphinx_rtd_theme/searchbox.html
+-rw-r--r--   0        0        0     1247 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/.venv/ai-services/lib/python3.8/site-packages/sphinx_rtd_theme/versions.html
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/.venv/ai-services/lib/python3.8/site-packages/tornado/test/static/dir/index.html
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/.venv/ai-services/lib/python3.8/site-packages/tornado/test/templates/utf8.html
+-rw-r--r--   0        0        0     1881 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/dist/ai_services-0.4.1/.venv/lib/python3.8/site-packages/alabaster/about.html
+-rw-r--r--   0        0        0      866 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/dist/ai_services-0.4.1/.venv/lib/python3.8/site-packages/alabaster/donate.html
+-rw-r--r--   0        0        0     4285 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/dist/ai_services-0.4.1/.venv/lib/python3.8/site-packages/alabaster/layout.html
+-rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/dist/ai_services-0.4.1/.venv/lib/python3.8/site-packages/alabaster/navigation.html
+-rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/dist/ai_services-0.4.1/.venv/lib/python3.8/site-packages/alabaster/relations.html
+-rw-r--r--   0        0        0     5400 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/dist/ai_services-0.4.1/.venv/lib/python3.8/site-packages/coverage/htmlfiles/index.html
+-rw-r--r--   0        0        0     6437 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/dist/ai_services-0.4.1/.venv/lib/python3.8/site-packages/coverage/htmlfiles/pyfile.html
+-rw-r--r--   0        0        0    26094 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/dist/ai_services-0.4.1/.venv/lib/python3.8/site-packages/docutils-0.17.1.dist-info/SOURCES.html
+-rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/dist/ai_services-0.4.1/.venv/lib/python3.8/site-packages/docutils-0.17.1.dist-info/dependency_links.html
+-rw-r--r--   0        0        0      969 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/dist/ai_services-0.4.1/.venv/lib/python3.8/site-packages/docutils-0.17.1.dist-info/top_level.html
+-rw-r--r--   0        0        0     1620 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/dist/ai_services-0.4.1/.venv/lib/python3.8/site-packages/matplotlib/backends/web_backend/all_figures.html
+-rw-r--r--   0        0        0     1311 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/dist/ai_services-0.4.1/.venv/lib/python3.8/site-packages/matplotlib/backends/web_backend/ipython_inline_figure.html
+-rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/dist/ai_services-0.4.1/.venv/lib/python3.8/site-packages/matplotlib/backends/web_backend/single_figure.html
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/dist/ai_services-0.4.1/.venv/lib/python3.8/site-packages/numpy/core/lib/npy-pkg-config/mlib.ini
+-rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/dist/ai_services-0.4.1/.venv/lib/python3.8/site-packages/numpy/core/lib/npy-pkg-config/npymath.ini
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/dist/ai_services-0.4.1/.venv/lib/python3.8/site-packages/numpy/typing/tests/data/mypy.ini
+-rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/dist/ai_services-0.4.1/.venv/lib/python3.8/site-packages/sanic_ext/extensions/openapi/ui/redoc.html
+-rw-r--r--   0        0        0     1530 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/dist/ai_services-0.4.1/.venv/lib/python3.8/site-packages/sanic_ext/extensions/openapi/ui/swagger.html
+-rw-r--r--   0        0        0     3303 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/dist/ai_services-0.4.1/.venv/lib/python3.8/site-packages/sphinx/themes/agogo/layout.html
+-rw-r--r--   0        0        0     1636 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/dist/ai_services-0.4.1/.venv/lib/python3.8/site-packages/sphinx/themes/basic/defindex.html
+-rw-r--r--   0        0        0     1892 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/dist/ai_services-0.4.1/.venv/lib/python3.8/site-packages/sphinx/themes/basic/domainindex.html
+-rw-r--r--   0        0        0     1804 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/dist/ai_services-0.4.1/.venv/lib/python3.8/site-packages/sphinx/themes/basic/genindex-single.html
+-rw-r--r--   0        0        0     1210 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/dist/ai_services-0.4.1/.venv/lib/python3.8/site-packages/sphinx/themes/basic/genindex-split.html
+-rw-r--r--   0        0        0     2069 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/dist/ai_services-0.4.1/.venv/lib/python3.8/site-packages/sphinx/themes/basic/genindex.html
+-rw-r--r--   0        0        0      432 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/dist/ai_services-0.4.1/.venv/lib/python3.8/site-packages/sphinx/themes/basic/globaltoc.html
+-rw-r--r--   0        0        0     7633 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/dist/ai_services-0.4.1/.venv/lib/python3.8/site-packages/sphinx/themes/basic/layout.html
+-rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/dist/ai_services-0.4.1/.venv/lib/python3.8/site-packages/sphinx/themes/basic/localtoc.html
+-rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/dist/ai_services-0.4.1/.venv/lib/python3.8/site-packages/sphinx/themes/basic/page.html
+-rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/dist/ai_services-0.4.1/.venv/lib/python3.8/site-packages/sphinx/themes/basic/relations.html
+-rw-r--r--   0        0        0     2039 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/dist/ai_services-0.4.1/.venv/lib/python3.8/site-packages/sphinx/themes/basic/search.html
+-rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/dist/ai_services-0.4.1/.venv/lib/python3.8/site-packages/sphinx/themes/basic/searchbox.html
+-rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/dist/ai_services-0.4.1/.venv/lib/python3.8/site-packages/sphinx/themes/basic/sourcelink.html
+-rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/dist/ai_services-0.4.1/.venv/lib/python3.8/site-packages/sphinx/themes/basic/changes/frameset.html
+-rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/dist/ai_services-0.4.1/.venv/lib/python3.8/site-packages/sphinx/themes/basic/changes/rstsource.html
+-rw-r--r--   0        0        0     1306 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/dist/ai_services-0.4.1/.venv/lib/python3.8/site-packages/sphinx/themes/basic/changes/versionchanges.html
+-rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/dist/ai_services-0.4.1/.venv/lib/python3.8/site-packages/sphinx/themes/bizstyle/layout.html
+-rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/dist/ai_services-0.4.1/.venv/lib/python3.8/site-packages/sphinx/themes/classic/layout.html
+-rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/dist/ai_services-0.4.1/.venv/lib/python3.8/site-packages/sphinx/themes/epub/epub-cover.html
+-rw-r--r--   0        0        0      543 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/dist/ai_services-0.4.1/.venv/lib/python3.8/site-packages/sphinx/themes/epub/layout.html
+-rw-r--r--   0        0        0     2012 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/dist/ai_services-0.4.1/.venv/lib/python3.8/site-packages/sphinx/themes/haiku/layout.html
+-rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/dist/ai_services-0.4.1/.venv/lib/python3.8/site-packages/sphinx/themes/nonav/layout.html
+-rw-r--r--   0        0        0      875 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/dist/ai_services-0.4.1/.venv/lib/python3.8/site-packages/sphinx/themes/pyramid/layout.html
+-rw-r--r--   0        0        0     1661 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/dist/ai_services-0.4.1/.venv/lib/python3.8/site-packages/sphinx/themes/scrolls/layout.html
+-rw-r--r--   0        0        0     4220 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/dist/ai_services-0.4.1/.venv/lib/python3.8/site-packages/sphinx_rtd_theme/breadcrumbs.html
+-rw-r--r--   0        0        0     2914 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/dist/ai_services-0.4.1/.venv/lib/python3.8/site-packages/sphinx_rtd_theme/footer.html
+-rw-r--r--   0        0        0     9660 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/dist/ai_services-0.4.1/.venv/lib/python3.8/site-packages/sphinx_rtd_theme/layout.html
+-rw-r--r--   0        0        0     1759 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/dist/ai_services-0.4.1/.venv/lib/python3.8/site-packages/sphinx_rtd_theme/search.html
+-rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/dist/ai_services-0.4.1/.venv/lib/python3.8/site-packages/sphinx_rtd_theme/searchbox.html
+-rw-r--r--   0        0        0     1247 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/dist/ai_services-0.4.1/.venv/lib/python3.8/site-packages/sphinx_rtd_theme/versions.html
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/dist/ai_services-0.4.1/.venv/lib/python3.8/site-packages/tornado/test/static/dir/index.html
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/dist/ai_services-0.4.1/.venv/lib/python3.8/site-packages/tornado/test/templates/utf8.html
+-rw-r--r--   0        0        0     1581 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/dist/ai_services-0.4.1/dist/ai_services-0.4.0/example/alembic.ini
+-rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/dist/ai_services-0.4.1/dist/ai_services-0.4.0/example/example/templates/_layout.html
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/dist/ai_services-0.4.1/dist/ai_services-0.4.0/example/example/templates/index.html
+-rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/dist/ai_services-0.4.1/dist/ai_services-0.4.0/example/front/index.html
+-rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/dist/ai_services-0.4.1/dist/ai_services-0.4.0/services/files/_layout.default.html
+-rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/dist/ai_services-0.4.1/dist/ai_services-0.4.0/services/files/_layout.vite.html
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/dist/ai_services-0.4.1/dist/ai_services-0.4.0/services/files/index.html
+-rw-r--r--   0        0        0     1424 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/dist/ai_services-0.4.1/dist/ai_services-0.4.0/services/files/app/alembic.ini
+-rw-r--r--   0        0        0     1581 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/dist/ai_services-0.4.1/example/alembic.ini
+-rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/dist/ai_services-0.4.1/example/example/migrations/script.py.mako
+-rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/dist/ai_services-0.4.1/example/example/templates/_layout.html
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/dist/ai_services-0.4.1/example/example/templates/index.html
+-rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/dist/ai_services-0.4.1/example/front/index.html
+-rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/dist/ai_services-0.4.1/services/files/_layout.default.html
+-rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/dist/ai_services-0.4.1/services/files/_layout.vite.html
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/dist/ai_services-0.4.1/services/files/index.html
+-rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/dist/ai_services-0.4.1/services/files/alembic/script.py.mako
+-rw-r--r--   0        0        0     1424 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/dist/ai_services-0.4.1/services/files/app/alembic.ini
+-rw-r--r--   0        0        0     1585 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/dist/ai_services-0.4.1/test_app/alembic.ini
+-rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/dist/ai_services-0.4.1/test_app/front/index.html
+-rw-r--r--   0        0        0    14075 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/dist/ai_services-0.4.1/test_app/front/node_modules/@tailwindcss/forms/index.html
+-rw-r--r--   0        0        0     8148 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/dist/ai_services-0.4.1/test_app/front/node_modules/@tailwindcss/forms/kitchen-sink.html
+-rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/dist/ai_services-0.4.1/test_app/test_app/templates/_layout.html
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/dist/ai_services-0.4.1/test_app/test_app/templates/index.html
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/docs/databases.md
+-rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/docs/references.md
+-rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/docs/release.md
+-rw-r--r--   0        0        0     1581 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/example/alembic.ini
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/example/example/__init__.py
+-rw-r--r--   0        0        0      744 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/example/example/db.py
+-rw-r--r--   0        0        0     3107 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/example/example/managers.py
+-rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/example/example/models.py
+-rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/example/example/tasks.py
+-rw-r--r--   0        0        0     2108 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/example/example/users_models.py
+-rw-r--r--   0        0        0     2832 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/example/example/views.py
+-rw-r--r--   0        0        0     1941 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/example/example/web.py
+-rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/example/example/api/example.py
+-rw-r--r--   0        0        0     2185 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/example/example/api/users.py
+-rw-r--r--   0        0        0      792 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/example/example/commands/shell.py
+-rw-r--r--   0        0        0     5047 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/example/example/commands/users.py
+-rw-r--r--   0        0        0     2735 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/example/example/migrations/env.py
+-rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/example/example/migrations/script.py.mako
+-rw-r--r--   0        0        0     1157 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/example/example/templates/_layout.html
+-rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/example/example/templates/index.html
+-rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/example/example/templates/login.html
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/example/server_conf/__init__.py
+-rw-r--r--   0        0        0     1748 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/example/server_conf/settings.py
+-rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/scripts/get_version.py
+-rwxr-xr-x   0        0        0      181 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/scripts/update_versions.sh
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/services/__about__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/services/__init__.py
+-rw-r--r--   0        0        0     2914 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/services/base.py
+-rw-r--r--   0        0        0     1777 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/services/cli.py
+-rw-r--r--   0        0        0     1411 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/services/cli_project.py
+-rw-r--r--   0        0        0     2352 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/services/conf.py
+-rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/services/defaults.py
+-rw-r--r--   0        0        0     1466 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/services/errors.py
+-rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/services/global_settings.py
+-rw-r--r--   0        0        0     6645 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/services/init_script.py
+-rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/services/jt.py
+-rw-r--r--   0        0        0     3013 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/services/redis_conn.py
+-rw-r--r--   0        0        0     2693 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/services/server.py
+-rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/services/shortcuts.py
+-rw-r--r--   0        0        0    11682 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/services/storage.py
+-rw-r--r--   0        0        0     9147 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/services/types.py
+-rw-r--r--   0        0        0     1672 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/services/users.py
+-rw-r--r--   0        0        0     7470 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/services/utils.py
+-rw-r--r--   0        0        0    15010 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/services/workers.py
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/services/commands/__init__.py
+-rw-r--r--   0        0        0     1190 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/services/commands/common.py
+-rw-r--r--   0        0        0     4142 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/services/commands/db.py
+-rw-r--r--   0        0        0     5298 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/services/commands/tasks.py
+-rw-r--r--   0        0        0     2533 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/services/commands/web.py
+-rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/services/db/__init__.py
+-rw-r--r--   0        0        0     2175 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/services/db/common.py
+-rw-r--r--   0        0        0     3885 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/services/db/managers.py
+-rw-r--r--   0        0        0     3106 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/services/db/migration.py
+-rw-r--r--   0        0        0     1832 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/services/db/pages.py
+-rw-r--r--   0        0        0     2270 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/services/db/plugin.py
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/services/db/pragmas.py
+-rw-r--r--   0        0        0    10305 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/services/db/sqlhelper.py
+-rw-r--r--   0        0        0     1267 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/services/db/utils.py
+-rw-r--r--   0        0        0     1305 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/services/db/web.py
+-rw-r--r--   0        0        0     8164 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/services/ext/google.py
+-rw-r--r--   0        0        0     8530 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/services/ext/sql/workers.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/services/files/__init__.py
+-rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/services/files/_layout.default.html
+-rw-r--r--   0        0        0     1157 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/services/files/_layout.vite.html
+-rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/services/files/index.html
+-rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/services/files/login.html
+-rw-r--r--   0        0        0     1974 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/services/files/settings.py
+-rw-r--r--   0        0        0     2746 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/services/files/alembic/env.py
+-rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/services/files/alembic/script.py.mako
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/services/files/app/__init__.py
+-rw-r--r--   0        0        0     1424 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/services/files/app/alembic.ini
+-rw-r--r--   0        0        0     1210 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/services/files/app/api_bp.py
+-rw-r--r--   0        0        0      745 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/services/files/app/db.py
+-rw-r--r--   0        0        0     3132 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/services/files/app/managers.py
+-rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/services/files/app/models.py
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/services/files/app/tasks.py
+-rw-r--r--   0        0        0     2186 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/services/files/app/users_bp.py
+-rw-r--r--   0        0        0     2181 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/services/files/app/users_models.py
+-rw-r--r--   0        0        0     3048 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/services/files/app/views.py
+-rw-r--r--   0        0        0     2934 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/services/files/app/web.py
+-rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/services/files/app/commands/shell.py
+-rw-r--r--   0        0        0     5048 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/services/files/app/commands/users.py
+-rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/services/security/__init__.py
+-rw-r--r--   0        0        0     1363 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/services/security/base.py
+-rw-r--r--   0        0        0     6531 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/services/security/jwtauth.py
+-rw-r--r--   0        0        0      964 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/services/security/memory_store.py
+-rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/services/security/password.py
+-rw-r--r--   0        0        0      969 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/services/security/redis_store.py
+-rw-r--r--   0        0        0     1482 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/services/security/scopes.py
+-rw-r--r--   0        0        0     2350 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/services/security/sessionauth.py
+-rw-r--r--   0        0        0     2767 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/services/security/sql_store.py
+-rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/services/security/utils.py
+-rw-r--r--   0        0        0     3686 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/services/security/web.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/services/templates/__init__.py
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/services/templates/html.py
+-rw-r--r--   0        0        0     4795 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/services/templates/render.py
+-rw-r--r--   0        0        0     3839 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/services/templates/simple_tags.py
+-rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/services/templates/static.py
+-rw-r--r--   0        0        0     3222 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/services/templates/vite.py
+-rw-r--r--   0        0        0     1585 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/test_app/alembic.ini
+-rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/test_app/test2/migrations/script.py.mako
+-rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/test_app/test2/templates/_layout.html
+-rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/test_app/test2/templates/index.html
+-rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/test_app/test3/templates/_layout.html
+-rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/test_app/test3/templates/index.html
+-rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/test_app/test4/templates/_layout.html
+-rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/test_app/test4/templates/index.html
+-rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/test_app/test_app/migrations/script.py.mako
+-rw-r--r--   0        0        0     1157 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/test_app/test_app/templates/_layout.html
+-rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/test_app/test_app/templates/index.html
+-rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/test_app/test_app/templates/login.html
+-rw-r--r--   0        0        0     8021 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/.gitignore
+-rw-r--r--   0        0        0    15977 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/LICENSE
+-rw-r--r--   0        0        0     5534 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/README.md
+-rw-r--r--   0        0        0     2496 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/pyproject.toml
+-rw-r--r--   0        0        0     7051 2020-02-02 00:00:00.000000 ai_services-0.5.0rc9/PKG-INFO
```

### Comparing `ai_services-0.5.0rc8/.dockerignore` & `ai_services-0.5.0rc9/.dockerignore`

 * *Files identical despite different names*

### Comparing `ai_services-0.5.0rc8/.pylintrc` & `ai_services-0.5.0rc9/.pylintrc`

 * *Files identical despite different names*

### Comparing `ai_services-0.5.0rc8/Makefile` & `ai_services-0.5.0rc9/Makefile`

 * *Files identical despite different names*

### Comparing `ai_services-0.5.0rc8/.venv/ai-services/lib/python3.8/site-packages/alabaster/about.html` & `ai_services-0.5.0rc9/.venv/ai-services/lib/python3.8/site-packages/alabaster/about.html`

 * *Files identical despite different names*

### Comparing `ai_services-0.5.0rc8/.venv/ai-services/lib/python3.8/site-packages/alabaster/donate.html` & `ai_services-0.5.0rc9/.venv/ai-services/lib/python3.8/site-packages/alabaster/donate.html`

 * *Files identical despite different names*

### Comparing `ai_services-0.5.0rc8/.venv/ai-services/lib/python3.8/site-packages/alabaster/layout.html` & `ai_services-0.5.0rc9/.venv/ai-services/lib/python3.8/site-packages/alabaster/layout.html`

 * *Files identical despite different names*

### Comparing `ai_services-0.5.0rc8/.venv/ai-services/lib/python3.8/site-packages/alabaster/relations.html` & `ai_services-0.5.0rc9/.venv/ai-services/lib/python3.8/site-packages/alabaster/relations.html`

 * *Files identical despite different names*

### Comparing `ai_services-0.5.0rc8/.venv/ai-services/lib/python3.8/site-packages/alembic/templates/async/alembic.ini.mako` & `ai_services-0.5.0rc9/.venv/ai-services/lib/python3.8/site-packages/alembic/templates/async/alembic.ini.mako`

 * *Files identical despite different names*

### Comparing `ai_services-0.5.0rc8/.venv/ai-services/lib/python3.8/site-packages/alembic/templates/generic/alembic.ini.mako` & `ai_services-0.5.0rc9/.venv/ai-services/lib/python3.8/site-packages/alembic/templates/generic/alembic.ini.mako`

 * *Files identical despite different names*

### Comparing `ai_services-0.5.0rc8/.venv/ai-services/lib/python3.8/site-packages/alembic/templates/multidb/alembic.ini.mako` & `ai_services-0.5.0rc9/.venv/ai-services/lib/python3.8/site-packages/alembic/templates/multidb/alembic.ini.mako`

 * *Files identical despite different names*

### Comparing `ai_services-0.5.0rc8/.venv/ai-services/lib/python3.8/site-packages/alembic/templates/multidb/script.py.mako` & `ai_services-0.5.0rc9/.venv/ai-services/lib/python3.8/site-packages/alembic/templates/multidb/script.py.mako`

 * *Files identical despite different names*

### Comparing `ai_services-0.5.0rc8/.venv/ai-services/lib/python3.8/site-packages/coverage/htmlfiles/index.html` & `ai_services-0.5.0rc9/.venv/ai-services/lib/python3.8/site-packages/coverage/htmlfiles/index.html`

 * *Files identical despite different names*

### Comparing `ai_services-0.5.0rc8/.venv/ai-services/lib/python3.8/site-packages/coverage/htmlfiles/pyfile.html` & `ai_services-0.5.0rc9/.venv/ai-services/lib/python3.8/site-packages/coverage/htmlfiles/pyfile.html`

 * *Files identical despite different names*

### Comparing `ai_services-0.5.0rc8/.venv/ai-services/lib/python3.8/site-packages/docutils-0.18.1.dist-info/SOURCES.html` & `ai_services-0.5.0rc9/.venv/ai-services/lib/python3.8/site-packages/docutils-0.18.1.dist-info/SOURCES.html`

 * *Files identical despite different names*

### Comparing `ai_services-0.5.0rc8/.venv/ai-services/lib/python3.8/site-packages/docutils-0.18.1.dist-info/dependency_links.html` & `ai_services-0.5.0rc9/.venv/ai-services/lib/python3.8/site-packages/docutils-0.18.1.dist-info/dependency_links.html`

 * *Files identical despite different names*

### Comparing `ai_services-0.5.0rc8/.venv/ai-services/lib/python3.8/site-packages/docutils-0.18.1.dist-info/top_level.html` & `ai_services-0.5.0rc9/.venv/ai-services/lib/python3.8/site-packages/docutils-0.18.1.dist-info/top_level.html`

 * *Files identical despite different names*

### Comparing `ai_services-0.5.0rc8/.venv/ai-services/lib/python3.8/site-packages/sanic_ext/extensions/openapi/ui/redoc.html` & `ai_services-0.5.0rc9/.venv/ai-services/lib/python3.8/site-packages/sanic_ext/extensions/openapi/ui/redoc.html`

 * *Files identical despite different names*

### Comparing `ai_services-0.5.0rc8/.venv/ai-services/lib/python3.8/site-packages/sanic_ext/extensions/openapi/ui/swagger.html` & `ai_services-0.5.0rc9/.venv/ai-services/lib/python3.8/site-packages/sanic_ext/extensions/openapi/ui/swagger.html`

 * *Files identical despite different names*

### Comparing `ai_services-0.5.0rc8/.venv/ai-services/lib/python3.8/site-packages/sphinx/themes/agogo/layout.html` & `ai_services-0.5.0rc9/.venv/ai-services/lib/python3.8/site-packages/sphinx/themes/agogo/layout.html`

 * *Files identical despite different names*

### Comparing `ai_services-0.5.0rc8/.venv/ai-services/lib/python3.8/site-packages/sphinx/themes/basic/defindex.html` & `ai_services-0.5.0rc9/.venv/ai-services/lib/python3.8/site-packages/sphinx/themes/basic/defindex.html`

 * *Files identical despite different names*

### Comparing `ai_services-0.5.0rc8/.venv/ai-services/lib/python3.8/site-packages/sphinx/themes/basic/domainindex.html` & `ai_services-0.5.0rc9/.venv/ai-services/lib/python3.8/site-packages/sphinx/themes/basic/domainindex.html`

 * *Files identical despite different names*

### Comparing `ai_services-0.5.0rc8/.venv/ai-services/lib/python3.8/site-packages/sphinx/themes/basic/genindex-single.html` & `ai_services-0.5.0rc9/.venv/ai-services/lib/python3.8/site-packages/sphinx/themes/basic/genindex-single.html`

 * *Files identical despite different names*

### Comparing `ai_services-0.5.0rc8/.venv/ai-services/lib/python3.8/site-packages/sphinx/themes/basic/genindex-split.html` & `ai_services-0.5.0rc9/.venv/ai-services/lib/python3.8/site-packages/sphinx/themes/basic/genindex-split.html`

 * *Files identical despite different names*

### Comparing `ai_services-0.5.0rc8/.venv/ai-services/lib/python3.8/site-packages/sphinx/themes/basic/genindex.html` & `ai_services-0.5.0rc9/.venv/ai-services/lib/python3.8/site-packages/sphinx/themes/basic/genindex.html`

 * *Files identical despite different names*

### Comparing `ai_services-0.5.0rc8/.venv/ai-services/lib/python3.8/site-packages/sphinx/themes/basic/layout.html` & `ai_services-0.5.0rc9/.venv/ai-services/lib/python3.8/site-packages/sphinx/themes/basic/layout.html`

 * *Files identical despite different names*

### Comparing `ai_services-0.5.0rc8/.venv/ai-services/lib/python3.8/site-packages/sphinx/themes/basic/relations.html` & `ai_services-0.5.0rc9/.venv/ai-services/lib/python3.8/site-packages/sphinx/themes/basic/relations.html`

 * *Files identical despite different names*

### Comparing `ai_services-0.5.0rc8/.venv/ai-services/lib/python3.8/site-packages/sphinx/themes/basic/search.html` & `ai_services-0.5.0rc9/.venv/ai-services/lib/python3.8/site-packages/sphinx/themes/basic/search.html`

 * *Files identical despite different names*

### Comparing `ai_services-0.5.0rc8/.venv/ai-services/lib/python3.8/site-packages/sphinx/themes/basic/searchbox.html` & `ai_services-0.5.0rc9/.venv/ai-services/lib/python3.8/site-packages/sphinx/themes/basic/searchbox.html`

 * *Files identical despite different names*

### Comparing `ai_services-0.5.0rc8/.venv/ai-services/lib/python3.8/site-packages/sphinx/themes/basic/sourcelink.html` & `ai_services-0.5.0rc9/.venv/ai-services/lib/python3.8/site-packages/sphinx/themes/basic/sourcelink.html`

 * *Files identical despite different names*

### Comparing `ai_services-0.5.0rc8/.venv/ai-services/lib/python3.8/site-packages/sphinx/themes/basic/changes/versionchanges.html` & `ai_services-0.5.0rc9/.venv/ai-services/lib/python3.8/site-packages/sphinx/themes/basic/changes/versionchanges.html`

 * *Files identical despite different names*

### Comparing `ai_services-0.5.0rc8/.venv/ai-services/lib/python3.8/site-packages/sphinx/themes/bizstyle/layout.html` & `ai_services-0.5.0rc9/.venv/ai-services/lib/python3.8/site-packages/sphinx/themes/bizstyle/layout.html`

 * *Files identical despite different names*

### Comparing `ai_services-0.5.0rc8/.venv/ai-services/lib/python3.8/site-packages/sphinx/themes/classic/layout.html` & `ai_services-0.5.0rc9/.venv/ai-services/lib/python3.8/site-packages/sphinx/themes/classic/layout.html`

 * *Files identical despite different names*

### Comparing `ai_services-0.5.0rc8/.venv/ai-services/lib/python3.8/site-packages/sphinx/themes/epub/epub-cover.html` & `ai_services-0.5.0rc9/.venv/ai-services/lib/python3.8/site-packages/sphinx/themes/epub/epub-cover.html`

 * *Files identical despite different names*

### Comparing `ai_services-0.5.0rc8/.venv/ai-services/lib/python3.8/site-packages/sphinx/themes/epub/layout.html` & `ai_services-0.5.0rc9/.venv/ai-services/lib/python3.8/site-packages/sphinx/themes/epub/layout.html`

 * *Files identical despite different names*

### Comparing `ai_services-0.5.0rc8/.venv/ai-services/lib/python3.8/site-packages/sphinx/themes/haiku/layout.html` & `ai_services-0.5.0rc9/.venv/ai-services/lib/python3.8/site-packages/sphinx/themes/haiku/layout.html`

 * *Files identical despite different names*

### Comparing `ai_services-0.5.0rc8/.venv/ai-services/lib/python3.8/site-packages/sphinx/themes/nonav/layout.html` & `ai_services-0.5.0rc9/.venv/ai-services/lib/python3.8/site-packages/sphinx/themes/nonav/layout.html`

 * *Files identical despite different names*

### Comparing `ai_services-0.5.0rc8/.venv/ai-services/lib/python3.8/site-packages/sphinx/themes/pyramid/layout.html` & `ai_services-0.5.0rc9/.venv/ai-services/lib/python3.8/site-packages/sphinx/themes/pyramid/layout.html`

 * *Files identical despite different names*

### Comparing `ai_services-0.5.0rc8/.venv/ai-services/lib/python3.8/site-packages/sphinx/themes/scrolls/layout.html` & `ai_services-0.5.0rc9/.venv/ai-services/lib/python3.8/site-packages/sphinx/themes/scrolls/layout.html`

 * *Files identical despite different names*

### Comparing `ai_services-0.5.0rc8/.venv/ai-services/lib/python3.8/site-packages/sphinx_rtd_theme/breadcrumbs.html` & `ai_services-0.5.0rc9/.venv/ai-services/lib/python3.8/site-packages/sphinx_rtd_theme/breadcrumbs.html`

 * *Files identical despite different names*

### Comparing `ai_services-0.5.0rc8/.venv/ai-services/lib/python3.8/site-packages/sphinx_rtd_theme/footer.html` & `ai_services-0.5.0rc9/.venv/ai-services/lib/python3.8/site-packages/sphinx_rtd_theme/footer.html`

 * *Files identical despite different names*

### Comparing `ai_services-0.5.0rc8/.venv/ai-services/lib/python3.8/site-packages/sphinx_rtd_theme/layout.html` & `ai_services-0.5.0rc9/.venv/ai-services/lib/python3.8/site-packages/sphinx_rtd_theme/layout.html`

 * *Files identical despite different names*

### Comparing `ai_services-0.5.0rc8/.venv/ai-services/lib/python3.8/site-packages/sphinx_rtd_theme/search.html` & `ai_services-0.5.0rc9/.venv/ai-services/lib/python3.8/site-packages/sphinx_rtd_theme/search.html`

 * *Files identical despite different names*

### Comparing `ai_services-0.5.0rc8/.venv/ai-services/lib/python3.8/site-packages/sphinx_rtd_theme/versions.html` & `ai_services-0.5.0rc9/.venv/ai-services/lib/python3.8/site-packages/sphinx_rtd_theme/versions.html`

 * *Files identical despite different names*

### Comparing `ai_services-0.5.0rc8/dist/ai_services-0.4.1/.venv/lib/python3.8/site-packages/alabaster/about.html` & `ai_services-0.5.0rc9/dist/ai_services-0.4.1/.venv/lib/python3.8/site-packages/alabaster/about.html`

 * *Files identical despite different names*

### Comparing `ai_services-0.5.0rc8/dist/ai_services-0.4.1/.venv/lib/python3.8/site-packages/alabaster/donate.html` & `ai_services-0.5.0rc9/dist/ai_services-0.4.1/.venv/lib/python3.8/site-packages/alabaster/donate.html`

 * *Files identical despite different names*

### Comparing `ai_services-0.5.0rc8/dist/ai_services-0.4.1/.venv/lib/python3.8/site-packages/alabaster/layout.html` & `ai_services-0.5.0rc9/dist/ai_services-0.4.1/.venv/lib/python3.8/site-packages/alabaster/layout.html`

 * *Files identical despite different names*

### Comparing `ai_services-0.5.0rc8/dist/ai_services-0.4.1/.venv/lib/python3.8/site-packages/alabaster/relations.html` & `ai_services-0.5.0rc9/dist/ai_services-0.4.1/.venv/lib/python3.8/site-packages/alabaster/relations.html`

 * *Files identical despite different names*

### Comparing `ai_services-0.5.0rc8/dist/ai_services-0.4.1/.venv/lib/python3.8/site-packages/coverage/htmlfiles/index.html` & `ai_services-0.5.0rc9/dist/ai_services-0.4.1/.venv/lib/python3.8/site-packages/coverage/htmlfiles/index.html`

 * *Files identical despite different names*

### Comparing `ai_services-0.5.0rc8/dist/ai_services-0.4.1/.venv/lib/python3.8/site-packages/coverage/htmlfiles/pyfile.html` & `ai_services-0.5.0rc9/dist/ai_services-0.4.1/.venv/lib/python3.8/site-packages/coverage/htmlfiles/pyfile.html`

 * *Files identical despite different names*

### Comparing `ai_services-0.5.0rc8/dist/ai_services-0.4.1/.venv/lib/python3.8/site-packages/docutils-0.17.1.dist-info/SOURCES.html` & `ai_services-0.5.0rc9/dist/ai_services-0.4.1/.venv/lib/python3.8/site-packages/docutils-0.17.1.dist-info/SOURCES.html`

 * *Files identical despite different names*

### Comparing `ai_services-0.5.0rc8/dist/ai_services-0.4.1/.venv/lib/python3.8/site-packages/docutils-0.17.1.dist-info/dependency_links.html` & `ai_services-0.5.0rc9/dist/ai_services-0.4.1/.venv/lib/python3.8/site-packages/docutils-0.17.1.dist-info/dependency_links.html`

 * *Files identical despite different names*

### Comparing `ai_services-0.5.0rc8/dist/ai_services-0.4.1/.venv/lib/python3.8/site-packages/docutils-0.17.1.dist-info/top_level.html` & `ai_services-0.5.0rc9/dist/ai_services-0.4.1/.venv/lib/python3.8/site-packages/docutils-0.17.1.dist-info/top_level.html`

 * *Files identical despite different names*

### Comparing `ai_services-0.5.0rc8/dist/ai_services-0.4.1/.venv/lib/python3.8/site-packages/matplotlib/backends/web_backend/all_figures.html` & `ai_services-0.5.0rc9/dist/ai_services-0.4.1/.venv/lib/python3.8/site-packages/matplotlib/backends/web_backend/all_figures.html`

 * *Files identical despite different names*

### Comparing `ai_services-0.5.0rc8/dist/ai_services-0.4.1/.venv/lib/python3.8/site-packages/matplotlib/backends/web_backend/ipython_inline_figure.html` & `ai_services-0.5.0rc9/dist/ai_services-0.4.1/.venv/lib/python3.8/site-packages/matplotlib/backends/web_backend/ipython_inline_figure.html`

 * *Files identical despite different names*

### Comparing `ai_services-0.5.0rc8/dist/ai_services-0.4.1/.venv/lib/python3.8/site-packages/matplotlib/backends/web_backend/single_figure.html` & `ai_services-0.5.0rc9/dist/ai_services-0.4.1/.venv/lib/python3.8/site-packages/matplotlib/backends/web_backend/single_figure.html`

 * *Files identical despite different names*

### Comparing `ai_services-0.5.0rc8/dist/ai_services-0.4.1/.venv/lib/python3.8/site-packages/sanic_ext/extensions/openapi/ui/redoc.html` & `ai_services-0.5.0rc9/dist/ai_services-0.4.1/.venv/lib/python3.8/site-packages/sanic_ext/extensions/openapi/ui/redoc.html`

 * *Files identical despite different names*

### Comparing `ai_services-0.5.0rc8/dist/ai_services-0.4.1/.venv/lib/python3.8/site-packages/sanic_ext/extensions/openapi/ui/swagger.html` & `ai_services-0.5.0rc9/dist/ai_services-0.4.1/.venv/lib/python3.8/site-packages/sanic_ext/extensions/openapi/ui/swagger.html`

 * *Files identical despite different names*

### Comparing `ai_services-0.5.0rc8/dist/ai_services-0.4.1/.venv/lib/python3.8/site-packages/sphinx/themes/agogo/layout.html` & `ai_services-0.5.0rc9/dist/ai_services-0.4.1/.venv/lib/python3.8/site-packages/sphinx/themes/agogo/layout.html`

 * *Files identical despite different names*

### Comparing `ai_services-0.5.0rc8/dist/ai_services-0.4.1/.venv/lib/python3.8/site-packages/sphinx/themes/basic/defindex.html` & `ai_services-0.5.0rc9/dist/ai_services-0.4.1/.venv/lib/python3.8/site-packages/sphinx/themes/basic/defindex.html`

 * *Files identical despite different names*

### Comparing `ai_services-0.5.0rc8/dist/ai_services-0.4.1/.venv/lib/python3.8/site-packages/sphinx/themes/basic/domainindex.html` & `ai_services-0.5.0rc9/dist/ai_services-0.4.1/.venv/lib/python3.8/site-packages/sphinx/themes/basic/domainindex.html`

 * *Files identical despite different names*

### Comparing `ai_services-0.5.0rc8/dist/ai_services-0.4.1/.venv/lib/python3.8/site-packages/sphinx/themes/basic/genindex-single.html` & `ai_services-0.5.0rc9/dist/ai_services-0.4.1/.venv/lib/python3.8/site-packages/sphinx/themes/basic/genindex-single.html`

 * *Files identical despite different names*

### Comparing `ai_services-0.5.0rc8/dist/ai_services-0.4.1/.venv/lib/python3.8/site-packages/sphinx/themes/basic/genindex-split.html` & `ai_services-0.5.0rc9/dist/ai_services-0.4.1/.venv/lib/python3.8/site-packages/sphinx/themes/basic/genindex-split.html`

 * *Files identical despite different names*

### Comparing `ai_services-0.5.0rc8/dist/ai_services-0.4.1/.venv/lib/python3.8/site-packages/sphinx/themes/basic/genindex.html` & `ai_services-0.5.0rc9/dist/ai_services-0.4.1/.venv/lib/python3.8/site-packages/sphinx/themes/basic/genindex.html`

 * *Files identical despite different names*

### Comparing `ai_services-0.5.0rc8/dist/ai_services-0.4.1/.venv/lib/python3.8/site-packages/sphinx/themes/basic/layout.html` & `ai_services-0.5.0rc9/dist/ai_services-0.4.1/.venv/lib/python3.8/site-packages/sphinx/themes/basic/layout.html`

 * *Files identical despite different names*

### Comparing `ai_services-0.5.0rc8/dist/ai_services-0.4.1/.venv/lib/python3.8/site-packages/sphinx/themes/basic/relations.html` & `ai_services-0.5.0rc9/dist/ai_services-0.4.1/.venv/lib/python3.8/site-packages/sphinx/themes/basic/relations.html`

 * *Files identical despite different names*

### Comparing `ai_services-0.5.0rc8/dist/ai_services-0.4.1/.venv/lib/python3.8/site-packages/sphinx/themes/basic/search.html` & `ai_services-0.5.0rc9/dist/ai_services-0.4.1/.venv/lib/python3.8/site-packages/sphinx/themes/basic/search.html`

 * *Files identical despite different names*

### Comparing `ai_services-0.5.0rc8/dist/ai_services-0.4.1/.venv/lib/python3.8/site-packages/sphinx/themes/basic/searchbox.html` & `ai_services-0.5.0rc9/dist/ai_services-0.4.1/.venv/lib/python3.8/site-packages/sphinx/themes/basic/searchbox.html`

 * *Files identical despite different names*

### Comparing `ai_services-0.5.0rc8/dist/ai_services-0.4.1/.venv/lib/python3.8/site-packages/sphinx/themes/basic/sourcelink.html` & `ai_services-0.5.0rc9/dist/ai_services-0.4.1/.venv/lib/python3.8/site-packages/sphinx/themes/basic/sourcelink.html`

 * *Files identical despite different names*

### Comparing `ai_services-0.5.0rc8/dist/ai_services-0.4.1/.venv/lib/python3.8/site-packages/sphinx/themes/basic/changes/versionchanges.html` & `ai_services-0.5.0rc9/dist/ai_services-0.4.1/.venv/lib/python3.8/site-packages/sphinx/themes/basic/changes/versionchanges.html`

 * *Files identical despite different names*

### Comparing `ai_services-0.5.0rc8/dist/ai_services-0.4.1/.venv/lib/python3.8/site-packages/sphinx/themes/bizstyle/layout.html` & `ai_services-0.5.0rc9/dist/ai_services-0.4.1/.venv/lib/python3.8/site-packages/sphinx/themes/bizstyle/layout.html`

 * *Files identical despite different names*

### Comparing `ai_services-0.5.0rc8/dist/ai_services-0.4.1/.venv/lib/python3.8/site-packages/sphinx/themes/epub/epub-cover.html` & `ai_services-0.5.0rc9/dist/ai_services-0.4.1/.venv/lib/python3.8/site-packages/sphinx/themes/epub/epub-cover.html`

 * *Files identical despite different names*

### Comparing `ai_services-0.5.0rc8/dist/ai_services-0.4.1/.venv/lib/python3.8/site-packages/sphinx/themes/epub/layout.html` & `ai_services-0.5.0rc9/dist/ai_services-0.4.1/.venv/lib/python3.8/site-packages/sphinx/themes/epub/layout.html`

 * *Files identical despite different names*

### Comparing `ai_services-0.5.0rc8/dist/ai_services-0.4.1/.venv/lib/python3.8/site-packages/sphinx/themes/haiku/layout.html` & `ai_services-0.5.0rc9/dist/ai_services-0.4.1/.venv/lib/python3.8/site-packages/sphinx/themes/haiku/layout.html`

 * *Files identical despite different names*

### Comparing `ai_services-0.5.0rc8/dist/ai_services-0.4.1/.venv/lib/python3.8/site-packages/sphinx/themes/nonav/layout.html` & `ai_services-0.5.0rc9/dist/ai_services-0.4.1/.venv/lib/python3.8/site-packages/sphinx/themes/nonav/layout.html`

 * *Files identical despite different names*

### Comparing `ai_services-0.5.0rc8/dist/ai_services-0.4.1/.venv/lib/python3.8/site-packages/sphinx/themes/pyramid/layout.html` & `ai_services-0.5.0rc9/dist/ai_services-0.4.1/.venv/lib/python3.8/site-packages/sphinx/themes/pyramid/layout.html`

 * *Files identical despite different names*

### Comparing `ai_services-0.5.0rc8/dist/ai_services-0.4.1/.venv/lib/python3.8/site-packages/sphinx/themes/scrolls/layout.html` & `ai_services-0.5.0rc9/dist/ai_services-0.4.1/.venv/lib/python3.8/site-packages/sphinx/themes/scrolls/layout.html`

 * *Files identical despite different names*

### Comparing `ai_services-0.5.0rc8/dist/ai_services-0.4.1/.venv/lib/python3.8/site-packages/sphinx_rtd_theme/breadcrumbs.html` & `ai_services-0.5.0rc9/dist/ai_services-0.4.1/.venv/lib/python3.8/site-packages/sphinx_rtd_theme/breadcrumbs.html`

 * *Files identical despite different names*

### Comparing `ai_services-0.5.0rc8/dist/ai_services-0.4.1/.venv/lib/python3.8/site-packages/sphinx_rtd_theme/footer.html` & `ai_services-0.5.0rc9/dist/ai_services-0.4.1/.venv/lib/python3.8/site-packages/sphinx_rtd_theme/footer.html`

 * *Files identical despite different names*

### Comparing `ai_services-0.5.0rc8/dist/ai_services-0.4.1/.venv/lib/python3.8/site-packages/sphinx_rtd_theme/layout.html` & `ai_services-0.5.0rc9/dist/ai_services-0.4.1/.venv/lib/python3.8/site-packages/sphinx_rtd_theme/layout.html`

 * *Files identical despite different names*

### Comparing `ai_services-0.5.0rc8/dist/ai_services-0.4.1/.venv/lib/python3.8/site-packages/sphinx_rtd_theme/search.html` & `ai_services-0.5.0rc9/dist/ai_services-0.4.1/.venv/lib/python3.8/site-packages/sphinx_rtd_theme/search.html`

 * *Files identical despite different names*

### Comparing `ai_services-0.5.0rc8/dist/ai_services-0.4.1/.venv/lib/python3.8/site-packages/sphinx_rtd_theme/versions.html` & `ai_services-0.5.0rc9/dist/ai_services-0.4.1/.venv/lib/python3.8/site-packages/sphinx_rtd_theme/versions.html`

 * *Files identical despite different names*

### Comparing `ai_services-0.5.0rc8/dist/ai_services-0.4.1/dist/ai_services-0.4.0/example/alembic.ini` & `ai_services-0.5.0rc9/dist/ai_services-0.4.1/dist/ai_services-0.4.0/example/alembic.ini`

 * *Files identical despite different names*

### Comparing `ai_services-0.5.0rc8/dist/ai_services-0.4.1/dist/ai_services-0.4.0/example/example/templates/_layout.html` & `ai_services-0.5.0rc9/dist/ai_services-0.4.1/dist/ai_services-0.4.0/example/example/templates/_layout.html`

 * *Files identical despite different names*

### Comparing `ai_services-0.5.0rc8/dist/ai_services-0.4.1/dist/ai_services-0.4.0/services/files/_layout.default.html` & `ai_services-0.5.0rc9/dist/ai_services-0.4.1/dist/ai_services-0.4.0/services/files/_layout.default.html`

 * *Files identical despite different names*

### Comparing `ai_services-0.5.0rc8/dist/ai_services-0.4.1/dist/ai_services-0.4.0/services/files/_layout.vite.html` & `ai_services-0.5.0rc9/dist/ai_services-0.4.1/dist/ai_services-0.4.0/services/files/_layout.vite.html`

 * *Files identical despite different names*

### Comparing `ai_services-0.5.0rc8/dist/ai_services-0.4.1/dist/ai_services-0.4.0/services/files/app/alembic.ini` & `ai_services-0.5.0rc9/dist/ai_services-0.4.1/dist/ai_services-0.4.0/services/files/app/alembic.ini`

 * *Files identical despite different names*

### Comparing `ai_services-0.5.0rc8/dist/ai_services-0.4.1/example/alembic.ini` & `ai_services-0.5.0rc9/dist/ai_services-0.4.1/example/alembic.ini`

 * *Files identical despite different names*

### Comparing `ai_services-0.5.0rc8/dist/ai_services-0.4.1/example/example/templates/_layout.html` & `ai_services-0.5.0rc9/dist/ai_services-0.4.1/example/example/templates/_layout.html`

 * *Files identical despite different names*

### Comparing `ai_services-0.5.0rc8/dist/ai_services-0.4.1/services/files/_layout.default.html` & `ai_services-0.5.0rc9/dist/ai_services-0.4.1/services/files/_layout.default.html`

 * *Files identical despite different names*

### Comparing `ai_services-0.5.0rc8/dist/ai_services-0.4.1/services/files/_layout.vite.html` & `ai_services-0.5.0rc9/dist/ai_services-0.4.1/services/files/_layout.vite.html`

 * *Files identical despite different names*

### Comparing `ai_services-0.5.0rc8/dist/ai_services-0.4.1/services/files/app/alembic.ini` & `ai_services-0.5.0rc9/dist/ai_services-0.4.1/services/files/app/alembic.ini`

 * *Files identical despite different names*

### Comparing `ai_services-0.5.0rc8/dist/ai_services-0.4.1/test_app/alembic.ini` & `ai_services-0.5.0rc9/dist/ai_services-0.4.1/test_app/alembic.ini`

 * *Files identical despite different names*

### Comparing `ai_services-0.5.0rc8/dist/ai_services-0.4.1/test_app/front/node_modules/@tailwindcss/forms/index.html` & `ai_services-0.5.0rc9/dist/ai_services-0.4.1/test_app/front/node_modules/@tailwindcss/forms/index.html`

 * *Files identical despite different names*

### Comparing `ai_services-0.5.0rc8/dist/ai_services-0.4.1/test_app/front/node_modules/@tailwindcss/forms/kitchen-sink.html` & `ai_services-0.5.0rc9/dist/ai_services-0.4.1/test_app/front/node_modules/@tailwindcss/forms/kitchen-sink.html`

 * *Files identical despite different names*

### Comparing `ai_services-0.5.0rc8/dist/ai_services-0.4.1/test_app/test_app/templates/_layout.html` & `ai_services-0.5.0rc9/dist/ai_services-0.4.1/test_app/test_app/templates/_layout.html`

 * *Files identical despite different names*

### Comparing `ai_services-0.5.0rc8/docs/release.md` & `ai_services-0.5.0rc9/docs/release.md`

 * *Files identical despite different names*

### Comparing `ai_services-0.5.0rc8/example/alembic.ini` & `ai_services-0.5.0rc9/example/alembic.ini`

 * *Files identical despite different names*

### Comparing `ai_services-0.5.0rc8/example/example/api/users.py` & `ai_services-0.5.0rc9/example/example/api/users.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,55 +1,64 @@
 from sanic import Blueprint, Request
 from sanic.response import json
 from sanic_ext import openapi
+
+from services.db.plugin import DBHelper
 from services.errors import AuthValidationFailed, WebAuthFailed
 from services.security import protected
-from services.types import JWTResponse, UserLogin
-from services.users import get_users_mg
+from services.security.jwtauth import JWTAuth
+from services.types import JWTPayload, JWTResponse, UserLogin
+
+from ..managers import UserManager
 
 users_bp = Blueprint("users", url_prefix="users", version="v1")
 
 
 @users_bp.post("/login")
 @openapi.response(200, {"application/json": JWTResponse})
 @openapi.response(403, dict(msg=str), "Not Found")
 @openapi.body(UserLogin)
-async def login_handler(request: Request):
-    manager = get_users_mg(request)
+async def login_handler(request: Request, um: UserManager, auth: JWTAuth, db: DBHelper):
+    # session = db.get_session(request)
     try:
         creds = UserLogin(**request.json)
-        user = await manager.authenticate(username=creds.username,
-                                          password=creds.password)
+        async with db.session() as session:
+            user = await um.authenticate(
+                session, username=creds.username, to_verify=creds.password
+            )
     except AuthValidationFailed as exc:
         raise WebAuthFailed() from exc
 
-    jwt = await manager.generate_token(user)
-    return json(jwt.dict(), 200)
+    # jwt = await manager.generate_token(user)
+    payload = JWTPayload(custom={"usr": user.username, "scopes": user.scopes})
+    tkn = await auth.generate_token(payload)
+    return json(tkn.dict(), 200)
 
 
 @users_bp.get("/verify")
 @openapi.response(200, {"application/json": JWTResponse})
-@protected()
+@protected(validators=["jwt"])
 async def verify_handler(request: Request):
     return json(request.ctx.token_data, 200)
 
 
 @users_bp.post("/refresh_token")
 @openapi.response(200, {"application/json": JWTResponse})
 @openapi.body(JWTResponse)
-async def refresh_handler(request):
-    if not request.app.config.AUTH_ALLOW_REFRESH:
+async def refresh_handler(request, auth: JWTAuth):
+    if not request.app.config.JWT_ALLOW_REFRESH:
         return json(dict(msg="Not found"), 404)
 
     at = request.token
     rftkn = request.json.get("refresh_token")
     if not rftkn:
         raise WebAuthFailed()
 
     old_token = JWTResponse(access_token=at, refresh_token=rftkn)
-    manager = get_users_mg(request)
     # redis = request.ctx.web_redis
     try:
-        jwt_res = await manager.refresh_token(old_token)
+        jwt_res = await auth.refresh_token(
+            old_token.access_token, old_token.refresh_token
+        )
         return json(jwt_res.dict(), 200)
     except AuthValidationFailed as e:
         raise WebAuthFailed() from e
```

### Comparing `ai_services-0.5.0rc8/example/example/migrations/env.py` & `ai_services-0.5.0rc9/example/example/migrations/env.py`

 * *Files identical despite different names*

### Comparing `ai_services-0.5.0rc8/example/example/templates/_layout.html` & `ai_services-0.5.0rc9/services/files/_layout.default.html`

 * *Files 26% similar despite different names*

```diff
@@ -1,24 +1,37 @@
 <!DOCTYPE html>
-<html lang="en">
+<html lang="{{ data.lang }}">
   <head>
+    <title>{% block title %}{{ data.title }}{% endblock title %}</title>
     <meta http-equiv="X-UA-Compatible" content="IE=edge">
     <meta http-equiv="content-type" content="text/html; charset=utf-8">
     <meta charset="utf-8">
-    <!-- Enable responsiveness on mobile devices-->
-    <meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1">
-    <title>Testing</title>
     {% block meta %}
+    {% for key, value in data.meta.dict().items() -%}
+    {% if value -%}
+    <meta name="{{ key }}" content="{{ value }}">
+    {% endif -%}
+    {% endfor -%}
     {% endblock meta %}
-
-    {% vite_asset "main.js" %}
   </head>
   <body class="antialiased bg-white dark:bg-gray-900 h-full">
-    
-    {% block content %}
-    {% endblock content %}
-
+    {% block menu -%}
+    <nav class="menu">
+      <ul>
+        <li><a href="/">Home</a></li>
+        {% if data.content.username -%}
+        <li><a href="{{ url_for ('web.logout_handler') }}">Logout</a></li>
+        {% else -%}
+        <li><a href="{{ url_for ('web.LoginView') }}">Login</a></li>
+        {% endif -%}
+      </ul>
+    </nav>
+    {% endblock menu %}
+    {% block content -%}
+    {% endblock content -%}
     {% block scripts %}
-    {% vite_dev %}
     {% endblock scripts %}
+    {% if conf.DEBUG -%}
+    {{ conf }}
+    {% endif -%}
   </body>
 </html>
```

#### html2text {}

```diff
@@ -1,6 +1,14 @@
 
 
-
-{% block meta %} {% endblock meta %} {% vite_asset "main.js" %}
-{% block content %} {% endblock content %} {% block scripts %} {% vite_dev %}
-{% endblock scripts %}
+ {% block meta %} {% for key, value in data.meta.dict().items() -%} {% if value
+-%}
+ {% endif -%} {% endfor -%} {% endblock meta %}
+{% block menu -%}
+    * Home
+    * {% if data.content.username -%}
+    * Logout
+    * {% else -%}
+    * Login
+    * {% endif -%}
+ {% endblock menu %} {% block content -%} {% endblock content -%} {% block
+scripts %} {% endblock scripts %} {% if conf.DEBUG -%} {{ conf }} {% endif -%}
```

### Comparing `ai_services-0.5.0rc8/example/server_conf/settings.py` & `ai_services-0.5.0rc9/example/server_conf/settings.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,42 +1,37 @@
 import sys
-
 from services import defaults, types
 
 # WARNING:
 # We do our best effort to keep sensible information private
 # but in the scenario of an intrusion into the network or machines
 # where servers are hosted, then it represents a risk for the information
 # stored in those machines.
 
 # General Folders for the server
-SECURITY = types.SecuritySettings(
-    JWT_SECRET="Changeme",
-    JWT_ALG="HS256",
-    AUTH_SALT="Changeme",
-)
-
-USER_MODEL = "example.models.UserModel"
-
 DATABASES = {
     "default": types.Database(
         name="default",
         async_url="sqlite+aiosqlite:///db.sqlite",
         sync_url="sqlite:///db.sqlite",
         description="Default database",
     )
 }
 
 APPS = [
-    # "services.users.web.WebApp",
-    "services.security.web.WebApp",
     "example.web.WebApp",
 ]
 
-
+SECURITY2 = types.SecurityConfig(
+    secret_key="qzaWO-gCnGp5LPKNdSpz0iVTmyoopxxNNmnjtgB61qk",
+    jwt=types.JWTConfig(
+        alg="HS256",
+        secret="qzaWO-gCnGp5LPKNdSpz0iVTmyoopxxNNmnjtgB61qk"
+    )
+)
 
 VITE_ENABLED = True
 VITE_CONFIG = types.ViteConfig(
     # Where dynamic assets in vite are configurated
     VITE_STATIC_URL_PATH="assets",
     # Local path from the python app where the vite dynamic assets are
     VITE_STATIC_DIR="front/src/assets",
@@ -49,12 +44,22 @@
     # special case for react
     VITE_REACT_MODE=False,
     # base url in the vite server the same as
     #    https://vitejs.dev/config/server-options.html#server-base
     VITE_BASE="/"
 )
 
+STATICFILES_DIRS = [
+        types.StaticDir(
+            name="public",
+            uripath="",
+            localdir="front/public/"
+        )
+]
+STORAGE = types.Storage(
+    bucket=".storage"
+    store_class="services.storage.AsyncLocal"
 
-
+)
 TEMPLATES_DIR = [
     "example/templates"
-]
+]
```

### Comparing `ai_services-0.5.0rc8/services/base.py` & `ai_services-0.5.0rc9/services/base.py`

 * *Files identical despite different names*

### Comparing `ai_services-0.5.0rc8/services/cli.py` & `ai_services-0.5.0rc9/services/cli.py`

 * *Files identical despite different names*

### Comparing `ai_services-0.5.0rc8/services/cli_project.py` & `ai_services-0.5.0rc9/services/cli_project.py`

 * *Files 10% similar despite different names*

```diff
@@ -35,27 +35,35 @@
     "--sql",
     default=True,
     is_flag=True,
     show_default=True,
     help="Add DB related files",
 )
 @click.option(
+    "--storage",
+    default=False,
+    is_flag=True,
+    show_default=True,
+    help="Add default storage",
+)
+@click.option(
     "--name",
     default=None,
     help="Name of the project, if empty it will ask you for a name",
 )
 @click.argument("base_path")
-def create_service_project(base_path, name, vite, users, tasks, sql):
+def create_service_project(base_path, name, vite, users, tasks, sql, storage):
     """Start a new project"""
     root = Path(base_path).resolve()
     opts = init_script.ScriptOpts(
         base_path=root,
         secret_key=token_urlsafe(32),
         app_name=name,
         users=users,
         vite_enabled=vite,
         tasks=tasks,
         sql=sql,
+        storage=storage,
     )
     print(opts)
 
     init_script.create_project(opts)
```

### Comparing `ai_services-0.5.0rc8/services/conf.py` & `ai_services-0.5.0rc9/services/conf.py`

 * *Files identical despite different names*

### Comparing `ai_services-0.5.0rc8/services/errors.py` & `ai_services-0.5.0rc9/services/errors.py`

 * *Files identical despite different names*

### Comparing `ai_services-0.5.0rc8/services/init_script.py` & `ai_services-0.5.0rc9/services/init_script.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 class ScriptOpts(BaseModel):
     base_path: Path
     secret_key: str
     app_name: Optional[str] = None
     vite_enabled: bool = False
     users: bool = True
     tasks: bool = False
+    storage: bool = False
     sql: bool = True
 
 
 console = Console()
 
 
 def _welcome_message():
```

### Comparing `ai_services-0.5.0rc8/services/jt.py` & `ai_services-0.5.0rc9/services/jt.py`

 * *Files identical despite different names*

### Comparing `ai_services-0.5.0rc8/services/redis_conn.py` & `ai_services-0.5.0rc9/services/redis_conn.py`

 * *Files identical despite different names*

### Comparing `ai_services-0.5.0rc8/services/server.py` & `ai_services-0.5.0rc9/services/server.py`

 * *Files identical despite different names*

### Comparing `ai_services-0.5.0rc8/services/storage.py` & `ai_services-0.5.0rc9/services/storage.py`

 * *Files identical despite different names*

### Comparing `ai_services-0.5.0rc8/services/types.py` & `ai_services-0.5.0rc9/services/types.py`

 * *Files identical despite different names*

### Comparing `ai_services-0.5.0rc8/services/users.py` & `ai_services-0.5.0rc9/services/users.py`

 * *Files identical despite different names*

### Comparing `ai_services-0.5.0rc8/services/utils.py` & `ai_services-0.5.0rc9/services/utils.py`

 * *Files identical despite different names*

### Comparing `ai_services-0.5.0rc8/services/workers.py` & `ai_services-0.5.0rc9/services/workers.py`

 * *Files identical despite different names*

### Comparing `ai_services-0.5.0rc8/services/commands/common.py` & `ai_services-0.5.0rc9/services/commands/common.py`

 * *Files identical despite different names*

### Comparing `ai_services-0.5.0rc8/services/commands/db.py` & `ai_services-0.5.0rc9/services/commands/db.py`

 * *Files identical despite different names*

### Comparing `ai_services-0.5.0rc8/services/commands/tasks.py` & `ai_services-0.5.0rc9/services/commands/tasks.py`

 * *Files identical despite different names*

### Comparing `ai_services-0.5.0rc8/services/commands/web.py` & `ai_services-0.5.0rc9/services/commands/web.py`

 * *Files 3% similar despite different names*

```diff
@@ -56,15 +56,15 @@
     print(f"Autoreload: {auto_reload}")
     print(f"Workers: {w}")
     print(f"Listening: {host}:{port}")
     print(f"OS PID: {os.getpid()}")
     print(f"With storage: {storage}")
 
     loader = AppLoader(
-        factory=partial(create_srv, settings=settings, with_storage=storage)
+        factory=partial(create_srv, settings=settings)
     )
     srv = loader.load()
     srv.prepare(
         host=host,
         port=int(port),
         dev=dev,
         auto_reload=auto_reload if not debug else False,
```

### Comparing `ai_services-0.5.0rc8/services/db/common.py` & `ai_services-0.5.0rc9/services/db/common.py`

 * *Files identical despite different names*

### Comparing `ai_services-0.5.0rc8/services/db/managers.py` & `ai_services-0.5.0rc9/services/db/managers.py`

 * *Files identical despite different names*

### Comparing `ai_services-0.5.0rc8/services/db/migration.py` & `ai_services-0.5.0rc9/services/db/migration.py`

 * *Files identical despite different names*

### Comparing `ai_services-0.5.0rc8/services/db/pages.py` & `ai_services-0.5.0rc9/services/db/pages.py`

 * *Files identical despite different names*

### Comparing `ai_services-0.5.0rc8/services/db/plugin.py` & `ai_services-0.5.0rc9/services/db/plugin.py`

 * *Files identical despite different names*

### Comparing `ai_services-0.5.0rc8/services/db/sqlhelper.py` & `ai_services-0.5.0rc9/services/db/sqlhelper.py`

 * *Files identical despite different names*

### Comparing `ai_services-0.5.0rc8/services/db/utils.py` & `ai_services-0.5.0rc9/services/db/utils.py`

 * *Files identical despite different names*

### Comparing `ai_services-0.5.0rc8/services/db/web.py` & `ai_services-0.5.0rc9/services/db/web.py`

 * *Files identical despite different names*

### Comparing `ai_services-0.5.0rc8/services/ext/google.py` & `ai_services-0.5.0rc9/services/ext/google.py`

 * *Files identical despite different names*

### Comparing `ai_services-0.5.0rc8/services/ext/sql/workers.py` & `ai_services-0.5.0rc9/services/ext/sql/workers.py`

 * *Files identical despite different names*

### Comparing `ai_services-0.5.0rc8/services/files/_layout.default.html` & `ai_services-0.5.0rc9/test_app/test2/templates/_layout.html`

 * *Files identical despite different names*

### Comparing `ai_services-0.5.0rc8/services/files/_layout.vite.html` & `ai_services-0.5.0rc9/example/example/templates/_layout.html`

 * *Files identical despite different names*

### Comparing `ai_services-0.5.0rc8/services/files/login.html` & `ai_services-0.5.0rc9/example/example/templates/login.html`

 * *Files identical despite different names*

### Comparing `ai_services-0.5.0rc8/services/files/settings.py` & `ai_services-0.5.0rc9/services/files/settings.py`

 * *Files 13% similar despite different names*

```diff
@@ -62,10 +62,20 @@
 TASKS = types.TasksBackend(
     uri="sqlite+aiosqlite:///tasks.sqlite"
     backend_class="services.ext.sql.workers.SQLBackend"
 
 )
 {% endif -%}
 
+{% if data.storage -%}
+STORAGE = types.Storage(
+    bucket=".storage"
+    store_class="services.storage.AsyncLocal"
+
+)
+{% endif -%}
+
+
 TEMPLATES_DIR = [
     "{{ data.app_name }}/templates"
 ]
+
```

### Comparing `ai_services-0.5.0rc8/services/files/alembic/env.py` & `ai_services-0.5.0rc9/services/files/alembic/env.py`

 * *Files identical despite different names*

### Comparing `ai_services-0.5.0rc8/services/files/app/alembic.ini` & `ai_services-0.5.0rc9/services/files/app/alembic.ini`

 * *Files identical despite different names*

### Comparing `ai_services-0.5.0rc8/services/files/app/db.py` & `ai_services-0.5.0rc9/services/files/app/db.py`

 * *Files identical despite different names*

### Comparing `ai_services-0.5.0rc8/services/files/app/managers.py` & `ai_services-0.5.0rc9/services/files/app/managers.py`

 * *Files identical despite different names*

### Comparing `ai_services-0.5.0rc8/services/files/app/models.py` & `ai_services-0.5.0rc9/services/files/app/models.py`

 * *Files identical despite different names*

### Comparing `ai_services-0.5.0rc8/services/files/app/users_bp.py` & `ai_services-0.5.0rc9/services/files/app/users_bp.py`

 * *Files identical despite different names*

### Comparing `ai_services-0.5.0rc8/services/files/app/users_models.py` & `ai_services-0.5.0rc9/services/files/app/users_models.py`

 * *Files identical despite different names*

### Comparing `ai_services-0.5.0rc8/services/files/app/views.py` & `ai_services-0.5.0rc9/services/files/app/views.py`

 * *Files identical despite different names*

### Comparing `ai_services-0.5.0rc8/services/files/app/web.py` & `ai_services-0.5.0rc9/services/files/app/web.py`

 * *Files identical despite different names*

### Comparing `ai_services-0.5.0rc8/services/files/app/commands/shell.py` & `ai_services-0.5.0rc9/services/files/app/commands/shell.py`

 * *Files identical despite different names*

### Comparing `ai_services-0.5.0rc8/services/files/app/commands/users.py` & `ai_services-0.5.0rc9/services/files/app/commands/users.py`

 * *Files identical despite different names*

### Comparing `ai_services-0.5.0rc8/services/security/base.py` & `ai_services-0.5.0rc9/services/security/base.py`

 * *Files identical despite different names*

### Comparing `ai_services-0.5.0rc8/services/security/jwtauth.py` & `ai_services-0.5.0rc9/services/security/jwtauth.py`

 * *Files identical despite different names*

### Comparing `ai_services-0.5.0rc8/services/security/memory_store.py` & `ai_services-0.5.0rc9/services/security/memory_store.py`

 * *Files identical despite different names*

### Comparing `ai_services-0.5.0rc8/services/security/password.py` & `ai_services-0.5.0rc9/services/security/password.py`

 * *Files identical despite different names*

### Comparing `ai_services-0.5.0rc8/services/security/redis_store.py` & `ai_services-0.5.0rc9/services/security/redis_store.py`

 * *Files identical despite different names*

### Comparing `ai_services-0.5.0rc8/services/security/scopes.py` & `ai_services-0.5.0rc9/services/security/scopes.py`

 * *Files identical despite different names*

### Comparing `ai_services-0.5.0rc8/services/security/sessionauth.py` & `ai_services-0.5.0rc9/services/security/sessionauth.py`

 * *Files identical despite different names*

### Comparing `ai_services-0.5.0rc8/services/security/sql_store.py` & `ai_services-0.5.0rc9/services/security/sql_store.py`

 * *Files identical despite different names*

### Comparing `ai_services-0.5.0rc8/services/security/utils.py` & `ai_services-0.5.0rc9/services/security/utils.py`

 * *Files identical despite different names*

### Comparing `ai_services-0.5.0rc8/services/security/web.py` & `ai_services-0.5.0rc9/services/security/web.py`

 * *Files identical despite different names*

### Comparing `ai_services-0.5.0rc8/services/templates/render.py` & `ai_services-0.5.0rc9/services/templates/render.py`

 * *Files identical despite different names*

### Comparing `ai_services-0.5.0rc8/services/templates/simple_tags.py` & `ai_services-0.5.0rc9/services/templates/simple_tags.py`

 * *Files identical despite different names*

### Comparing `ai_services-0.5.0rc8/services/templates/static.py` & `ai_services-0.5.0rc9/services/templates/static.py`

 * *Files identical despite different names*

### Comparing `ai_services-0.5.0rc8/services/templates/vite.py` & `ai_services-0.5.0rc9/services/templates/vite.py`

 * *Files identical despite different names*

### Comparing `ai_services-0.5.0rc8/test_app/alembic.ini` & `ai_services-0.5.0rc9/test_app/alembic.ini`

 * *Files 7% similar despite different names*

```diff
@@ -59,15 +59,7 @@
 
 [test_app]
 sqlalchemy.url = 
 script_location = %(here)s/test_app/migrations/
 models_module = test_app.models
 version_table = test_app_version
 db_name = default
-
-
-[test2]
-sqlalchemy.url = 
-script_location = %(here)s/test2/migrations/
-models_module = test2.models
-version_table = test2_version
-db_name = default
```

### Comparing `ai_services-0.5.0rc8/test_app/test2/templates/_layout.html` & `ai_services-0.5.0rc9/test_app/test3/templates/_layout.html`

 * *Files identical despite different names*

### Comparing `ai_services-0.5.0rc8/test_app/test3/templates/_layout.html` & `ai_services-0.5.0rc9/test_app/test4/templates/_layout.html`

 * *Files identical despite different names*

### Comparing `ai_services-0.5.0rc8/test_app/test4/templates/_layout.html` & `ai_services-0.5.0rc9/services/files/_layout.vite.html`

 * *Files 19% similar despite different names*

```diff
@@ -1,37 +1,41 @@
 <!DOCTYPE html>
 <html lang="{{ data.lang }}">
   <head>
     <title>{% block title %}{{ data.title }}{% endblock title %}</title>
     <meta http-equiv="X-UA-Compatible" content="IE=edge">
     <meta http-equiv="content-type" content="text/html; charset=utf-8">
     <meta charset="utf-8">
-    {% block meta %}
+    {% block meta -%}
     {% for key, value in data.meta.dict().items() -%}
     {% if value -%}
     <meta name="{{ key }}" content="{{ value }}">
     {% endif -%}
     {% endfor -%}
-    {% endblock meta %}
+    {% endblock meta -%}
+    {% vite_asset "main.js" %}
   </head>
   <body class="antialiased bg-white dark:bg-gray-900 h-full">
     {% block menu -%}
     <nav class="menu">
       <ul>
         <li><a href="/">Home</a></li>
-        {% if data.content.username -%}
+        {% if data.content.username %}
         <li><a href="{{ url_for ('web.logout_handler') }}">Logout</a></li>
-        {% else -%}
+        {% else %}
         <li><a href="{{ url_for ('web.LoginView') }}">Login</a></li>
-        {% endif -%}
+        {% endif %}
       </ul>
     </nav>
-    {% endblock menu %}
+    {% endblock menu -%}
     {% block content -%}
     {% endblock content -%}
-    {% block scripts %}
+
+    {% block scripts -%}
+    {% vite_dev %}
     {% endblock scripts %}
-    {% if conf.DEBUG -%}
+
+    {% if conf.DEBUG %}
     {{ conf }}
-    {% endif -%}
+    {% endif %}
   </body>
 </html>
```

#### html2text {}

```diff
@@ -1,14 +1,15 @@
 
 
- {% block meta %} {% for key, value in data.meta.dict().items() -%} {% if value
--%}
- {% endif -%} {% endfor -%} {% endblock meta %}
+ {% block meta -%} {% for key, value in data.meta.dict().items() -%} {% if
+value -%}
+ {% endif -%} {% endfor -%} {% endblock meta -%} {% vite_asset "main.js" %}
 {% block menu -%}
     * Home
-    * {% if data.content.username -%}
+    * {% if data.content.username %}
     * Logout
-    * {% else -%}
+    * {% else %}
     * Login
-    * {% endif -%}
- {% endblock menu %} {% block content -%} {% endblock content -%} {% block
-scripts %} {% endblock scripts %} {% if conf.DEBUG -%} {{ conf }} {% endif -%}
+    * {% endif %}
+ {% endblock menu -%} {% block content -%} {% endblock content -%} {% block
+scripts -%} {% vite_dev %} {% endblock scripts %} {% if conf.DEBUG %} {{ conf
+}} {% endif %}
```

### Comparing `ai_services-0.5.0rc8/test_app/test_app/templates/_layout.html` & `ai_services-0.5.0rc9/test_app/test_app/templates/_layout.html`

 * *Files identical despite different names*

### Comparing `ai_services-0.5.0rc8/test_app/test_app/templates/login.html` & `ai_services-0.5.0rc9/services/files/login.html`

 * *Files identical despite different names*

### Comparing `ai_services-0.5.0rc8/.gitignore` & `ai_services-0.5.0rc9/.gitignore`

 * *Files identical despite different names*

### Comparing `ai_services-0.5.0rc8/LICENSE` & `ai_services-0.5.0rc9/LICENSE`

 * *Files identical despite different names*

### Comparing `ai_services-0.5.0rc8/README.md` & `ai_services-0.5.0rc9/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -12,20 +12,22 @@
 The library tries to be the less intrusive possible, it is not intended to be a new framework but more to provided abstractions and code generation tools over 
 good established libraries and technologies. 
 
 ## Features
 
 - Async Web sever (Sanic)
 - Generation code for apps (like Django)
-- Multiple databases support (sync and async using SQLAlchemy 1.4/2.0)
+- Multiple databases support (sync and async using SQLAlchemy 2.0)
 - Schema migration tools pre-configurated to work in the first run (Alembic)
 - OpenApi/Swagger docs generation (Sanic)
 - Simple user system and authentication endpoints
 - JWT support
 - Vite support
+- Simple tasks implementations
+- Storage implementation for uploading files (local and google storage)
 
 
 ## Quickstart
 
 *Note: please use your favorite tool for python environments and dependencies*
 
 ```
@@ -52,31 +54,35 @@
          srv web -L -D
 ```
 
 It will ask you for a name for the firts app. 
 
 Then your folder will be:
 
-```
+```console
  » tree -a -L 2
 .
 ├── alembic.ini
-├── server_conf
+├── example
 │   ├── __init__.py
 │   ├── __pycache__
-│   └── settings.py
-└── test_app
+│   ├── api
+│   ├── commands
+│   ├── db.py
+│   ├── managers.py
+│   ├── migrations
+│   ├── models.py
+│   ├── tasks.py
+│   ├── templates
+│   ├── users_models.py
+│   ├── views.py
+│   └── web.py
+└── server_conf
     ├── __init__.py
-    ├── __pycache__
-    ├── db.py
-    ├── migrations
-    ├── models.py
-    ├── users_bp.py
-    ├── views_bp.py
-    └── web.py
+    └── settings.py
 ```
 
 Finally, the last step if you want to use the User system provided in the code, you will need to run a revision and upgrade action:
 
 ```
 srv db revision test_app -m first -R 0001 -m first
 srv db upgrade test_app
@@ -84,27 +90,28 @@
 
 With the default configuration, it will creates a `db.sqlite` file in the root of your project.
 
 Note: srv db uses alembic under the hood and Alembic is configurated in a way that is possible keep using it outside of `srv db`, it is more like a wrapper. 
 
 ## Status
 
-:warning: The library is being in use in one project, but it is still under active development and therefore full backward compatibility is not guaranteed before reaching v1.0.0.
+:warning: The library is being in use in some production projects, but it is still under active development and therefore full backward compatibility is not guaranteed before reaching v1.0.0.
 
 
 ## Roadmap:
 
 - [x] UserManager abstraction
 - [x] Add groups 
 - [ ] User Registration
 - [x] Expand command for users administration
 - [x] Custom commands hooks in `srv` 
 - [ ] Dev env files {Makefile, Dockerfile, docker-compose, etc}
 - [ ] Task Queue abstraction {Redis, Google Cloud Pub/Sub, etc}
-- [ ] File upload abstraction? (TBD)
+- [x] Simple task system implemented
+- [x] File upload (local and google storage)
 - [ ] OAuth 2.0 integration
 - [ ] documentation (guides and reference api)
 - [ ] Tools and abstraction for logging (stdout, google cloud log, etc)
 - [ ] Metrics (prometheus)
 - [x] Update to Sanic 22.9
 - [x] Update to SQLAlchemy 2.0
 - [ ] Websockets examples
```

### Comparing `ai_services-0.5.0rc8/pyproject.toml` & `ai_services-0.5.0rc9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ai_services-0.5.0rc8/PKG-INFO` & `ai_services-0.5.0rc9/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ai-services
-Version: 0.5.0rc8
+Version: 0.5.0rc9
 Summary: "A simple web framework based on Sanic"
 Project-URL: Documentation, https://github.com/nuxion/services#readme
 Project-URL: Issues, https://github.com/nuxion/services/issues
 Project-URL: Source, https://github.com/nuxion/services
 Author-email: nuxion <nuxion@gmail.com>
 License-Expression: MIT
 License-File: LICENSE
@@ -51,20 +51,22 @@
 The library tries to be the less intrusive possible, it is not intended to be a new framework but more to provided abstractions and code generation tools over 
 good established libraries and technologies. 
 
 ## Features
 
 - Async Web sever (Sanic)
 - Generation code for apps (like Django)
-- Multiple databases support (sync and async using SQLAlchemy 1.4/2.0)
+- Multiple databases support (sync and async using SQLAlchemy 2.0)
 - Schema migration tools pre-configurated to work in the first run (Alembic)
 - OpenApi/Swagger docs generation (Sanic)
 - Simple user system and authentication endpoints
 - JWT support
 - Vite support
+- Simple tasks implementations
+- Storage implementation for uploading files (local and google storage)
 
 
 ## Quickstart
 
 *Note: please use your favorite tool for python environments and dependencies*
 
 ```
@@ -91,31 +93,35 @@
          srv web -L -D
 ```
 
 It will ask you for a name for the firts app. 
 
 Then your folder will be:
 
-```
+```console
  » tree -a -L 2
 .
 ├── alembic.ini
-├── server_conf
+├── example
 │   ├── __init__.py
 │   ├── __pycache__
-│   └── settings.py
-└── test_app
+│   ├── api
+│   ├── commands
+│   ├── db.py
+│   ├── managers.py
+│   ├── migrations
+│   ├── models.py
+│   ├── tasks.py
+│   ├── templates
+│   ├── users_models.py
+│   ├── views.py
+│   └── web.py
+└── server_conf
     ├── __init__.py
-    ├── __pycache__
-    ├── db.py
-    ├── migrations
-    ├── models.py
-    ├── users_bp.py
-    ├── views_bp.py
-    └── web.py
+    └── settings.py
 ```
 
 Finally, the last step if you want to use the User system provided in the code, you will need to run a revision and upgrade action:
 
 ```
 srv db revision test_app -m first -R 0001 -m first
 srv db upgrade test_app
@@ -123,27 +129,28 @@
 
 With the default configuration, it will creates a `db.sqlite` file in the root of your project.
 
 Note: srv db uses alembic under the hood and Alembic is configurated in a way that is possible keep using it outside of `srv db`, it is more like a wrapper. 
 
 ## Status
 
-:warning: The library is being in use in one project, but it is still under active development and therefore full backward compatibility is not guaranteed before reaching v1.0.0.
+:warning: The library is being in use in some production projects, but it is still under active development and therefore full backward compatibility is not guaranteed before reaching v1.0.0.
 
 
 ## Roadmap:
 
 - [x] UserManager abstraction
 - [x] Add groups 
 - [ ] User Registration
 - [x] Expand command for users administration
 - [x] Custom commands hooks in `srv` 
 - [ ] Dev env files {Makefile, Dockerfile, docker-compose, etc}
 - [ ] Task Queue abstraction {Redis, Google Cloud Pub/Sub, etc}
-- [ ] File upload abstraction? (TBD)
+- [x] Simple task system implemented
+- [x] File upload (local and google storage)
 - [ ] OAuth 2.0 integration
 - [ ] documentation (guides and reference api)
 - [ ] Tools and abstraction for logging (stdout, google cloud log, etc)
 - [ ] Metrics (prometheus)
 - [x] Update to Sanic 22.9
 - [x] Update to SQLAlchemy 2.0
 - [ ] Websockets examples
```

