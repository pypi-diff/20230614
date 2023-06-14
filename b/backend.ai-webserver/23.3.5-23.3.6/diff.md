# Comparing `tmp/backend.ai-webserver-23.3.5.tar.gz` & `tmp/backend.ai-webserver-23.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "backend.ai-webserver-23.3.5.tar", last modified: Tue Jun 13 03:42:14 2023, max compression
+gzip compressed data, was "backend.ai-webserver-23.3.6.tar", last modified: Wed Jun 14 11:13:24 2023, max compression
```

## Comparing `backend.ai-webserver-23.3.5.tar` & `backend.ai-webserver-23.3.6.tar`

### file list

```diff
@@ -1,343 +1,343 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:42:14.904270 backend.ai-webserver-23.3.5/
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3014 2023-06-13 03:42:14.904270 backend.ai-webserver-23.3.5/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:42:14.828270 backend.ai-webserver-23.3.5/ai/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:42:14.828270 backend.ai-webserver-23.3.5/ai/backend/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:42:14.832270 backend.ai-webserver-23.3.5/ai/backend/web/
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     6194 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)    17637 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/proxy.py
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    30139 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:42:14.832270 backend.ai-webserver-23.3.5/ai/backend/web/static/
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/asset-manifest.json
--rw-r--r--   0 runner    (1001) docker     (123)     4459 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/config.toml
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/default.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:42:14.828270 backend.ai-webserver-23.3.5/ai/backend/web/static/dist/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:42:14.848270 backend.ai-webserver-23.3.5/ai/backend/web/static/dist/components/
--rw-r--r--   0 runner    (1001) docker     (123)    19470 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/dist/components/backend-ai-agent-summary-view-2ee21519.js
--rw-r--r--   0 runner    (1001) docker     (123)    82052 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/dist/components/backend-ai-agent-view-4f1cf328.js
--rw-r--r--   0 runner    (1001) docker     (123)     5578 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/dist/components/backend-ai-change-forgot-password-view-c3c64c37.js
--rw-r--r--   0 runner    (1001) docker     (123)   125014 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/dist/components/backend-ai-credential-view-f1a0fa17.js
--rw-r--r--   0 runner    (1001) docker     (123)   207666 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/dist/components/backend-ai-data-view-48c7459c.js
--rw-r--r--   0 runner    (1001) docker     (123)     6357 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/dist/components/backend-ai-edu-applauncher-b2bc846d.js
--rw-r--r--   0 runner    (1001) docker     (123)     4405 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/dist/components/backend-ai-email-verification-view-233abe92.js
--rw-r--r--   0 runner    (1001) docker     (123)    87367 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/dist/components/backend-ai-environment-view-50d103c9.js
--rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/dist/components/backend-ai-error-view-dc4bd660.js
--rw-r--r--   0 runner    (1001) docker     (123)    22282 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/dist/components/backend-ai-import-view-8d0888d2.js
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/dist/components/backend-ai-information-view-03c2890e.js
--rw-r--r--   0 runner    (1001) docker     (123)     3611 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/dist/components/backend-ai-list-status-5163ce5c.js
--rw-r--r--   0 runner    (1001) docker     (123)     7192 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/dist/components/backend-ai-maintenance-view-85a49dd0.js
--rw-r--r--   0 runner    (1001) docker     (123)     7919 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/dist/components/backend-ai-multi-select-ddd96cfb.js
--rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/dist/components/backend-ai-permission-denied-view-98eecd20.js
--rw-r--r--   0 runner    (1001) docker     (123)    39157 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/dist/components/backend-ai-resource-monitor-3d648354.js
--rw-r--r--   0 runner    (1001) docker     (123)   239617 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/dist/components/backend-ai-session-launcher-88b8173e.js
--rw-r--r--   0 runner    (1001) docker     (123)   136463 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/dist/components/backend-ai-session-view-4aabdfe3.js
--rw-r--r--   0 runner    (1001) docker     (123)    30793 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/dist/components/backend-ai-settings-view-5b62a307.js
--rw-r--r--   0 runner    (1001) docker     (123)    59311 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/dist/components/backend-ai-statistics-view-557cd6bb.js
--rw-r--r--   0 runner    (1001) docker     (123)    90679 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/dist/components/backend-ai-summary-view-59cccc2b.js
--rw-r--r--   0 runner    (1001) docker     (123)    54694 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/dist/components/backend-ai-usersettings-view-625e99ca.js
--rw-r--r--   0 runner    (1001) docker     (123)  1197377 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/dist/components/backend-ai-webui-661d9e43.js
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/dist/components/backend-ai-webui.js
--rw-r--r--   0 runner    (1001) docker     (123)   202894 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/dist/components/chart-js-49cb22bc.js
--rw-r--r--   0 runner    (1001) docker     (123)     8543 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/dist/components/dir-utils-38e4cf3d.js
--rw-r--r--   0 runner    (1001) docker     (123)     5166 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/dist/components/expansion-9d1f3a9b.js
--rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/dist/components/json_to_csv-35c9e191.js
--rw-r--r--   0 runner    (1001) docker     (123)    10112 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/dist/components/label-1ef3652f.js
--rw-r--r--   0 runner    (1001) docker     (123)     4870 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/dist/components/lablup-activity-panel-0289184a.js
--rw-r--r--   0 runner    (1001) docker     (123)   204073 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/dist/components/lablup-codemirror-04889726.js
--rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/dist/components/lablup-grid-sort-filter-column-9ffbb621.js
--rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/dist/components/lablup-loading-spinner-4649a250.js
--rw-r--r--   0 runner    (1001) docker     (123)    17307 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/dist/components/lablup-progress-bar-095aec81.js
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/dist/components/media-query-controller-e400dd2c.js
--rw-r--r--   0 runner    (1001) docker     (123)     1682 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/dist/components/mwc-check-list-item-c64cf1a4.js
--rw-r--r--   0 runner    (1001) docker     (123)    25704 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/dist/components/mwc-switch-e9473fc7.js
--rw-r--r--   0 runner    (1001) docker     (123)    46306 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/dist/components/mwc-tab-bar-064ccbb5.js
--rw-r--r--   0 runner    (1001) docker     (123)     3152 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/dist/components/progress-spinner-153eedb3.js
--rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/dist/components/radio-behavior-b66ed7c9.js
--rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/dist/components/select-73255102.js
--rw-r--r--   0 runner    (1001) docker     (123)    47299 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/dist/components/slider-cae179ae.js
--rw-r--r--   0 runner    (1001) docker     (123)     3028 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/dist/components/switch-1f68b491.js
--rw-r--r--   0 runner    (1001) docker     (123)     9151 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/dist/components/tab-group-6baff1e0.js
--rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/dist/components/textfield-6b6134ab.js
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/dist/components/translate-unsafe-html-861558b4.js
--rw-r--r--   0 runner    (1001) docker     (123)    99653 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/dist/components/vaadin-grid-c3d5c3c2.js
--rw-r--r--   0 runner    (1001) docker     (123)     6300 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/dist/components/vaadin-grid-filter-column-4c9cb29f.js
--rw-r--r--   0 runner    (1001) docker     (123)     4108 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/dist/components/vaadin-grid-selection-column-f0bd0bf3.js
--rw-r--r--   0 runner    (1001) docker     (123)     6676 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/dist/components/vaadin-grid-sort-column-7bed08ef.js
--rw-r--r--   0 runner    (1001) docker     (123)   246765 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/dist/components/vaadin-iconset-07d3debe.js
--rw-r--r--   0 runner    (1001) docker     (123)      792 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/dist/components/vaadin-item-0d805f04.js
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/dist/components/vaadin-item-mixin-88cba3b7.js
--rw-r--r--   0 runner    (1001) docker     (123)     3211 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:42:14.852270 backend.ai-webserver-23.3.5/ai/backend/web/static/manifest/
--rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/manifest/app.js
--rw-r--r--   0 runner    (1001) docker     (123)   134560 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/manifest/backend-ai.icns
--rw-r--r--   0 runner    (1001) docker     (123)   370070 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/manifest/backend-ai.ico
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:42:14.852270 backend.ai-webserver-23.3.5/ai/backend/web/static/manifest/backend-ai.iconset/
--rw-r--r--   0 runner    (1001) docker     (123)    10757 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/manifest/backend-ai.iconset/icon_128x128@1x.png
--rw-r--r--   0 runner    (1001) docker     (123)    18546 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/manifest/backend-ai.iconset/icon_128x128@2x.png
--rw-r--r--   0 runner    (1001) docker     (123)     3489 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/manifest/backend-ai.iconset/icon_16x16@1x.png
--rw-r--r--   0 runner    (1001) docker     (123)     4568 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/manifest/backend-ai.iconset/icon_16x16@2x.png
--rw-r--r--   0 runner    (1001) docker     (123)    18546 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/manifest/backend-ai.iconset/icon_256x256@1x.png
--rw-r--r--   0 runner    (1001) docker     (123)    36092 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/manifest/backend-ai.iconset/icon_256x256@2x.png
--rw-r--r--   0 runner    (1001) docker     (123)     4568 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/manifest/backend-ai.iconset/icon_32x32@1x.png
--rw-r--r--   0 runner    (1001) docker     (123)     6561 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/manifest/backend-ai.iconset/icon_32x32@2x.png
--rw-r--r--   0 runner    (1001) docker     (123)    36092 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/manifest/backend-ai.iconset/icon_512x512@1x.png
--rw-r--r--   0 runner    (1001) docker     (123)   230498 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/manifest/backend-ai.iconset/icon_512x512@2x.png
--rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/manifest/backend.ai-brand-simple.svg
--rw-r--r--   0 runner    (1001) docker     (123)     6253 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/manifest/backend.ai-brand-white.svg
--rw-r--r--   0 runner    (1001) docker     (123)     6316 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/manifest/backend.ai-brand.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2952 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/manifest/backend.ai-text.svg
--rw-r--r--   0 runner    (1001) docker     (123)    15086 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/manifest/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      876 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/manifest.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:42:14.856270 backend.ai-webserver-23.3.5/ai/backend/web/static/resources/
--rw-r--r--   0 runner    (1001) docker     (123)     6620 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/resources/app_template.json
--rw-r--r--   0 runner    (1001) docker     (123)     3465 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/resources/badge-dark.svg
--rw-r--r--   0 runner    (1001) docker     (123)     3809 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/resources/badge.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/resources/custom-kt.css
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/resources/custom-original.css
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/resources/custom.css
--rw-r--r--   0 runner    (1001) docker     (123)     2216 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/resources/device_metadata.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:42:14.856270 backend.ai-webserver-23.3.5/ai/backend/web/static/resources/documents/
--rw-r--r--   0 runner    (1001) docker     (123)    16782 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/resources/documents/privacy-policy.en.html
--rw-r--r--   0 runner    (1001) docker     (123)    17867 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/resources/documents/privacy-policy.ko.html
--rw-r--r--   0 runner    (1001) docker     (123)    45111 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/resources/documents/terms-of-service.en.html
--rw-r--r--   0 runner    (1001) docker     (123)    48789 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/resources/documents/terms-of-service.ko.html
--rw-r--r--   0 runner    (1001) docker     (123)   100353 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/resources/fashion-how-white.svg
--rw-r--r--   0 runner    (1001) docker     (123)   100242 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/resources/fashion-how.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:42:14.868270 backend.ai-webserver-23.3.5/ai/backend/web/static/resources/fonts/
--rw-r--r--   0 runner    (1001) docker     (123)   141484 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/resources/fonts/MaterialIcons-Regular.woff
--rw-r--r--   0 runner    (1001) docker     (123)    99932 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/resources/fonts/MaterialIcons-Regular.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    60840 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/resources/fonts/MaterialIcons-Regular.woff2_
--rw-r--r--   0 runner    (1001) docker     (123)    57620 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/resources/fonts/MaterialIcons-Regular.woff_
--rw-r--r--   0 runner    (1001) docker     (123)    92136 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/resources/fonts/fa-brands-400.woff
--rw-r--r--   0 runner    (1001) docker     (123)    78460 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/resources/fonts/fa-brands-400.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    16772 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/resources/fonts/fa-regular-400.woff
--rw-r--r--   0 runner    (1001) docker     (123)    13548 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/resources/fonts/fa-regular-400.woff2
--rw-r--r--   0 runner    (1001) docker     (123)   104280 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/resources/fonts/fa-solid-900.woff
--rw-r--r--   0 runner    (1001) docker     (123)    80300 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/resources/fonts/fa-solid-900.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    58053 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/resources/fonts/font-awesome-all.min.css
--rw-r--r--   0 runner    (1001) docker     (123)    37094 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/resources/fonts/font-awesome.css
--rw-r--r--   0 runner    (1001) docker     (123)     7575 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/resources/fonts/fonts.css
--rw-r--r--   0 runner    (1001) docker     (123)    22500 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/resources/fonts/montserrat-v13-latin-100.woff
--rw-r--r--   0 runner    (1001) docker     (123)    18376 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/resources/fonts/montserrat-v13-latin-100.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    22888 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/resources/fonts/montserrat-v13-latin-100italic.woff
--rw-r--r--   0 runner    (1001) docker     (123)    18644 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/resources/fonts/montserrat-v13-latin-100italic.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    24012 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/resources/fonts/montserrat-v13-latin-italic.woff
--rw-r--r--   0 runner    (1001) docker     (123)    19660 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/resources/fonts/montserrat-v13-latin-italic.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    23480 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/resources/fonts/montserrat-v13-latin-regular.woff
--rw-r--r--   0 runner    (1001) docker     (123)    19172 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/resources/fonts/montserrat-v13-latin-regular.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    16252 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/resources/fonts/quicksand-v13-latin-300.woff
--rw-r--r--   0 runner    (1001) docker     (123)    12780 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/resources/fonts/quicksand-v13-latin-300.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    17072 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/resources/fonts/quicksand-v13-latin-500.woff
--rw-r--r--   0 runner    (1001) docker     (123)    13616 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/resources/fonts/quicksand-v13-latin-500.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    16152 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/resources/fonts/quicksand-v13-latin-700.woff
--rw-r--r--   0 runner    (1001) docker     (123)    13108 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/resources/fonts/quicksand-v13-latin-700.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    17032 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/resources/fonts/quicksand-v13-latin-regular.woff
--rw-r--r--   0 runner    (1001) docker     (123)    13760 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/resources/fonts/quicksand-v13-latin-regular.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    20368 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/resources/fonts/roboto-v19-latin-100.woff
--rw-r--r--   0 runner    (1001) docker     (123)    15808 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/resources/fonts/roboto-v19-latin-100.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    21704 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/resources/fonts/roboto-v19-latin-100italic.woff
--rw-r--r--   0 runner    (1001) docker     (123)    17008 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/resources/fonts/roboto-v19-latin-100italic.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    20348 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/resources/fonts/roboto-v19-latin-300.woff
--rw-r--r--   0 runner    (1001) docker     (123)    15784 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/resources/fonts/roboto-v19-latin-300.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    22204 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/resources/fonts/roboto-v19-latin-300italic.woff
--rw-r--r--   0 runner    (1001) docker     (123)    17448 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/resources/fonts/roboto-v19-latin-300italic.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    20392 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/resources/fonts/roboto-v19-latin-900.woff
--rw-r--r--   0 runner    (1001) docker     (123)    15712 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/resources/fonts/roboto-v19-latin-900.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    22304 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/resources/fonts/roboto-v19-latin-900italic.woff
--rw-r--r--   0 runner    (1001) docker     (123)    17520 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/resources/fonts/roboto-v19-latin-900italic.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    21952 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/resources/fonts/roboto-v19-latin-italic.woff
--rw-r--r--   0 runner    (1001) docker     (123)    17324 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/resources/fonts/roboto-v19-latin-italic.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    20268 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/resources/fonts/roboto-v19-latin-regular.woff
--rw-r--r--   0 runner    (1001) docker     (123)    15736 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/resources/fonts/roboto-v19-latin-regular.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    43900 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/resources/fonts/ubuntu-v14-latin-300.woff
--rw-r--r--   0 runner    (1001) docker     (123)    38108 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/resources/fonts/ubuntu-v14-latin-300.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    43092 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/resources/fonts/ubuntu-v14-latin-300italic.woff
--rw-r--r--   0 runner    (1001) docker     (123)    37548 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/resources/fonts/ubuntu-v14-latin-300italic.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    34688 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/resources/fonts/ubuntu-v14-latin-500.woff
--rw-r--r--   0 runner    (1001) docker     (123)    29864 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/resources/fonts/ubuntu-v14-latin-500.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    36836 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/resources/fonts/ubuntu-v14-latin-500italic.woff
--rw-r--r--   0 runner    (1001) docker     (123)    31748 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/resources/fonts/ubuntu-v14-latin-500italic.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    33424 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/resources/fonts/ubuntu-v14-latin-700.woff
--rw-r--r--   0 runner    (1001) docker     (123)    28968 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/resources/fonts/ubuntu-v14-latin-700.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    34668 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/resources/fonts/ubuntu-v14-latin-700italic.woff
--rw-r--r--   0 runner    (1001) docker     (123)    30092 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/resources/fonts/ubuntu-v14-latin-700italic.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    41016 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/resources/fonts/ubuntu-v14-latin-italic.woff
--rw-r--r--   0 runner    (1001) docker     (123)    35832 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/resources/fonts/ubuntu-v14-latin-italic.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    39164 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/resources/fonts/ubuntu-v14-latin-regular.woff
--rw-r--r--   0 runner    (1001) docker     (123)    34260 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/resources/fonts/ubuntu-v14-latin-regular.woff2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:42:14.872270 backend.ai-webserver-23.3.5/ai/backend/web/static/resources/i18n/
--rw-r--r--   0 runner    (1001) docker     (123)    63323 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/resources/i18n/de.json
--rw-r--r--   0 runner    (1001) docker     (123)    91324 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/resources/i18n/el.json
--rw-r--r--   0 runner    (1001) docker     (123)    72187 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/resources/i18n/en.json
--rw-r--r--   0 runner    (1001) docker     (123)    63733 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/resources/i18n/es.json
--rw-r--r--   0 runner    (1001) docker     (123)    59666 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/resources/i18n/fi.json
--rw-r--r--   0 runner    (1001) docker     (123)    75880 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/resources/i18n/fr.json
--rw-r--r--   0 runner    (1001) docker     (123)    68882 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/resources/i18n/id.json
--rw-r--r--   0 runner    (1001) docker     (123)    62630 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/resources/i18n/it.json
--rw-r--r--   0 runner    (1001) docker     (123)    71153 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/resources/i18n/ja.json
--rw-r--r--   0 runner    (1001) docker     (123)    84462 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/resources/i18n/ko.json
--rw-r--r--   0 runner    (1001) docker     (123)    95092 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/resources/i18n/mn.json
--rw-r--r--   0 runner    (1001) docker     (123)    58578 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/resources/i18n/ms.json
--rw-r--r--   0 runner    (1001) docker     (123)    61937 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/resources/i18n/pl.json
--rw-r--r--   0 runner    (1001) docker     (123)    61465 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/resources/i18n/pt.json
--rw-r--r--   0 runner    (1001) docker     (123)    61520 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/resources/i18n/pt_BR.json
--rw-r--r--   0 runner    (1001) docker     (123)    98637 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/resources/i18n/ru.json
--rw-r--r--   0 runner    (1001) docker     (123)    60890 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/resources/i18n/tr.json
--rw-r--r--   0 runner    (1001) docker     (123)    68337 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/resources/i18n/vi.json
--rw-r--r--   0 runner    (1001) docker     (123)    53748 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/resources/i18n/zh_CN.json
--rw-r--r--   0 runner    (1001) docker     (123)    53750 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/resources/i18n/zh_TW.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:42:14.884270 backend.ai-webserver-23.3.5/ai/backend/web/static/resources/icons/
--rw-r--r--   0 runner    (1001) docker     (123)     1566 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/resources/icons/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)    21411 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/resources/icons/ROCm.png
--rw-r--r--   0 runner    (1001) docker     (123)    20312 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/resources/icons/ROCm_black.png
--rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/resources/icons/apache-spark.svg
--rw-r--r--   0 runner    (1001) docker     (123)     5050 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/resources/icons/aws.png
--rw-r--r--   0 runner    (1001) docker     (123)    12687 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/resources/icons/azure.png
--rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/resources/icons/c.svg
--rw-r--r--   0 runner    (1001) docker     (123)     5741 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/resources/icons/caffe.png
--rw-r--r--   0 runner    (1001) docker     (123)      982 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/resources/icons/caffe2.svg
--rw-r--r--   0 runner    (1001) docker     (123)    28363 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/resources/icons/ceph.png
--rw-r--r--   0 runner    (1001) docker     (123)     5370 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/resources/icons/check-list.svg
--rw-r--r--   0 runner    (1001) docker     (123)     3562 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/resources/icons/classification.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/resources/icons/cpp.svg
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/resources/icons/default.png
--rw-r--r--   0 runner    (1001) docker     (123)     3113 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/resources/icons/default_app.svg
--rw-r--r--   0 runner    (1001) docker     (123)      945 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/resources/icons/file_type_cuda.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/resources/icons/file_type_python.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2925 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/resources/icons/filebrowser.svg
--rw-r--r--   0 runner    (1001) docker     (123)    15775 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/resources/icons/flux.png
--rw-r--r--   0 runner    (1001) docker     (123)    10953 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/resources/icons/gcc.png
--rw-r--r--   0 runner    (1001) docker     (123)    22672 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/resources/icons/gcp.png
--rw-r--r--   0 runner    (1001) docker     (123)    11250 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/resources/icons/gdrive.png
--rw-r--r--   0 runner    (1001) docker     (123)     5602 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/resources/icons/h2o.png
--rw-r--r--   0 runner    (1001) docker     (123)     6649 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/resources/icons/haskell.png
--rw-r--r--   0 runner    (1001) docker     (123)    31187 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/resources/icons/javascript.png
--rw-r--r--   0 runner    (1001) docker     (123)     3404 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/resources/icons/julia.png
--rw-r--r--   0 runner    (1001) docker     (123)    16618 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/resources/icons/jupyter.png
--rw-r--r--   0 runner    (1001) docker     (123)    46557 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/resources/icons/jupyterlab.png
--rw-r--r--   0 runner    (1001) docker     (123)  1150358 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/resources/icons/kitty.png
--rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/resources/icons/lablup.png
--rw-r--r--   0 runner    (1001) docker     (123)    18225 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/resources/icons/local.png
--rw-r--r--   0 runner    (1001) docker     (123)    14460 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/resources/icons/lua.png
--rw-r--r--   0 runner    (1001) docker     (123)    56266 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/resources/icons/matlab.png
--rw-r--r--   0 runner    (1001) docker     (123)    25435 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/resources/icons/mlflow.png
--rw-r--r--   0 runner    (1001) docker     (123)     4404 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/resources/icons/mxnet.svg
--rw-r--r--   0 runner    (1001) docker     (123)     7280 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/resources/icons/nbp.png
--rw-r--r--   0 runner    (1001) docker     (123)    13523 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/resources/icons/nni.png
--rw-r--r--   0 runner    (1001) docker     (123)    15790 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/resources/icons/nni.svg
--rw-r--r--   0 runner    (1001) docker     (123)   144381 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/resources/icons/nodejs.png
--rw-r--r--   0 runner    (1001) docker     (123)    11549 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/resources/icons/novnc.svg
--rw-r--r--   0 runner    (1001) docker     (123)     5557 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/resources/icons/nvidia.png
--rw-r--r--   0 runner    (1001) docker     (123)    14684 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/resources/icons/octave.png
--rw-r--r--   0 runner    (1001) docker     (123)     8349 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/resources/icons/openstack.png
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/resources/icons/orbit.svg
--rw-r--r--   0 runner    (1001) docker     (123)   150992 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/resources/icons/php.png
--rw-r--r--   0 runner    (1001) docker     (123)    27901 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/resources/icons/purestorage.png
--rw-r--r--   0 runner    (1001) docker     (123)   177194 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/resources/icons/python.png
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/resources/icons/pytorch.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/resources/icons/r-lang.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/resources/icons/rebel.svg
--rw-r--r--   0 runner    (1001) docker     (123)     5521 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/resources/icons/rust.svg
--rw-r--r--   0 runner    (1001) docker     (123)     5041 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/resources/icons/sftp.png
--rw-r--r--   0 runner    (1001) docker     (123)     3627 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/resources/icons/sftp2.png
--rw-r--r--   0 runner    (1001) docker     (123)    51521 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/resources/icons/swift-tensorflow.png
--rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/resources/icons/swift.svg
--rw-r--r--   0 runner    (1001) docker     (123)     6965 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/resources/icons/tensorflow.png
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/resources/icons/terminal.svg
--rw-r--r--   0 runner    (1001) docker     (123)    15484 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/resources/icons/texlive.png
--rw-r--r--   0 runner    (1001) docker     (123)     2844 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/resources/icons/tpu.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/resources/icons/ubuntu.svg
--rw-r--r--   0 runner    (1001) docker     (123)     4446 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/resources/icons/vscode.svg
--rw-r--r--   0 runner    (1001) docker     (123)    67813 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/resources/icons/xfce.png
--rw-r--r--   0 runner    (1001) docker     (123)     2253 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/resources/icons/xrdp.svg
--rw-r--r--   0 runner    (1001) docker     (123)    26430 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/resources/image_metadata.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:42:14.888270 backend.ai-webserver-23.3.5/ai/backend/web/static/resources/images/
--rw-r--r--   0 runner    (1001) docker     (123)  1352095 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/resources/images/401_unauthorized_access.svg
--rw-r--r--   0 runner    (1001) docker     (123)    62250 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/resources/images/404_not_found.svg
--rw-r--r--   0 runner    (1001) docker     (123)   103075 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/resources/images/launcher-background.png
--rw-r--r--   0 runner    (1001) docker     (123)    84446 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/resources/images/loading-background-large.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    20788 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/resources/images/loading-background.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    19682 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/resources/images/web-terminal-guide-1.png
--rw-r--r--   0 runner    (1001) docker     (123)    18386 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/resources/images/web-terminal-guide-2.png
--rw-r--r--   0 runner    (1001) docker     (123)    69357 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/resources/images/web-terminal-guide-3.png
--rw-r--r--   0 runner    (1001) docker     (123)    18296 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/resources/images/web-terminal-guide-4.png
--rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/resources/logo.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:42:14.888270 backend.ai-webserver-23.3.5/ai/backend/web/static/resources/menu_icons/
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/resources/menu_icons/icon_create_a_key_pair.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/resources/menu_icons/icon_keypair_management.svg
--rw-r--r--   0 runner    (1001) docker     (123)      685 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/resources/menu_icons/icon_upload_files.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2993 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/resources/storage_metadata.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:42:14.888270 backend.ai-webserver-23.3.5/ai/backend/web/static/resources/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     6717 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/resources/templates/under_construction.html
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/resources/theme.json
--rw-r--r--   0 runner    (1001) docker     (123)     4176 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/resources/webui.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:42:14.828270 backend.ai-webserver-23.3.5/ai/backend/web/static/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:42:14.888270 backend.ai-webserver-23.3.5/ai/backend/web/static/src/lib/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:42:14.896270 backend.ai-webserver-23.3.5/ai/backend/web/static/src/lib/bundles/
--rw-r--r--   0 runner    (1001) docker     (123)    19998 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/src/lib/bundles/webcomponents-ce.js
--rw-r--r--   0 runner    (1001) docker     (123)   129129 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/src/lib/bundles/webcomponents-ce.js.map
--rw-r--r--   0 runner    (1001) docker     (123)    10669 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/src/lib/bundles/webcomponents-pf_dom.js
--rw-r--r--   0 runner    (1001) docker     (123)    45370 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/src/lib/bundles/webcomponents-pf_dom.js.map
--rw-r--r--   0 runner    (1001) docker     (123)    14541 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/src/lib/bundles/webcomponents-pf_js.js
--rw-r--r--   0 runner    (1001) docker     (123)    53114 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/src/lib/bundles/webcomponents-pf_js.js.map
--rw-r--r--   0 runner    (1001) docker     (123)   133025 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/src/lib/bundles/webcomponents-sd-ce-pf.js
--rw-r--r--   0 runner    (1001) docker     (123)   806549 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/src/lib/bundles/webcomponents-sd-ce-pf.js.map
--rw-r--r--   0 runner    (1001) docker     (123)    95511 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/src/lib/bundles/webcomponents-sd-ce.js
--rw-r--r--   0 runner    (1001) docker     (123)   630748 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/src/lib/bundles/webcomponents-sd-ce.js.map
--rw-r--r--   0 runner    (1001) docker     (123)    76437 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/src/lib/bundles/webcomponents-sd.js
--rw-r--r--   0 runner    (1001) docker     (123)   501551 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/src/lib/bundles/webcomponents-sd.js.map
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:42:14.896270 backend.ai-webserver-23.3.5/ai/backend/web/static/src/lib/web-animations-js/
--rw-r--r--   0 runner    (1001) docker     (123)    50580 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/src/lib/web-animations-js/web-animations-next-lite.min.js
--rw-r--r--   0 runner    (1001) docker     (123)     7773 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/src/lib/webcomponents-loader.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:42:14.832270 backend.ai-webserver-23.3.5/ai/backend/web/static/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:42:14.904270 backend.ai-webserver-23.3.5/ai/backend/web/static/static/js/
--rw-r--r--   0 runner    (1001) docker     (123)   154086 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/static/js/149.924fa2a6.chunk.js
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/static/js/149.924fa2a6.chunk.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)   623058 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/static/js/149.924fa2a6.chunk.js.map
--rw-r--r--   0 runner    (1001) docker     (123)     6739 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/static/js/478.8c8fd27b.chunk.js
--rw-r--r--   0 runner    (1001) docker     (123)    22813 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/static/js/478.8c8fd27b.chunk.js.map
--rw-r--r--   0 runner    (1001) docker     (123)   164411 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/static/js/488.70f8dcf6.chunk.js
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/static/js/488.70f8dcf6.chunk.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)   666043 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/static/js/488.70f8dcf6.chunk.js.map
--rw-r--r--   0 runner    (1001) docker     (123)     7801 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/static/js/540.c51503fa.chunk.js
--rw-r--r--   0 runner    (1001) docker     (123)    23524 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/static/js/540.c51503fa.chunk.js.map
--rw-r--r--   0 runner    (1001) docker     (123)    82120 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/static/js/558.9310b842.chunk.js
--rw-r--r--   0 runner    (1001) docker     (123)   261609 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/static/js/558.9310b842.chunk.js.map
--rw-r--r--   0 runner    (1001) docker     (123)    84119 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/static/js/618.fdb02897.chunk.js
--rw-r--r--   0 runner    (1001) docker     (123)   318442 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/static/js/618.fdb02897.chunk.js.map
--rw-r--r--   0 runner    (1001) docker     (123)   149146 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/static/js/627.a131ed07.chunk.js
--rw-r--r--   0 runner    (1001) docker     (123)   615392 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/static/js/627.a131ed07.chunk.js.map
--rw-r--r--   0 runner    (1001) docker     (123)     3020 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/static/js/818.9b28dc99.chunk.js
--rw-r--r--   0 runner    (1001) docker     (123)     7181 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/static/js/818.9b28dc99.chunk.js.map
--rw-r--r--   0 runner    (1001) docker     (123)   152760 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/static/js/main.8f973991.js
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/static/js/main.8f973991.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)   395128 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/static/js/main.8f973991.js.map
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:42:14.904270 backend.ai-webserver-23.3.5/ai/backend/web/static/static/media/
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/static/media/getFetch.40f37ddea2378391108f.cjs
--rw-r--r--   0 runner    (1001) docker     (123)     6772 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/sw.js
--rw-r--r--   0 runner    (1001) docker     (123)    11027 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/sw.js.map
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/version.json
--rw-r--r--   0 runner    (1001) docker     (123)    14328 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/workbox-d249b2c8.js
--rw-r--r--   0 runner    (1001) docker     (123)   137419 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/static/workbox-d249b2c8.js.map
--rw-r--r--   0 runner    (1001) docker     (123)     4333 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     2981 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/template.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:42:14.904270 backend.ai-webserver-23.3.5/ai/backend/web/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     3035 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/templates/config.toml.j2
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/ai/backend/web/templates/config_ini.toml.j2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:42:14.904270 backend.ai-webserver-23.3.5/backend.ai_webserver.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3014 2023-06-13 03:42:14.000000 backend.ai-webserver-23.3.5/backend.ai_webserver.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17896 2023-06-13 03:42:14.000000 backend.ai-webserver-23.3.5/backend.ai_webserver.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 03:42:14.000000 backend.ai-webserver-23.3.5/backend.ai_webserver.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 03:42:14.000000 backend.ai-webserver-23.3.5/backend.ai_webserver.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/backend.ai_webserver.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-06-13 03:42:14.000000 backend.ai-webserver-23.3.5/backend.ai_webserver.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-06-13 03:42:14.000000 backend.ai-webserver-23.3.5/backend.ai_webserver.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/backend_shim.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 03:42:14.904270 backend.ai-webserver-23.3.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)    21479 2023-06-13 03:42:13.000000 backend.ai-webserver-23.3.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:13:24.237651 backend.ai-webserver-23.3.6/
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3014 2023-06-14 11:13:24.237651 backend.ai-webserver-23.3.6/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:13:24.189652 backend.ai-webserver-23.3.6/ai/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:13:24.189652 backend.ai-webserver-23.3.6/ai/backend/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:13:24.189652 backend.ai-webserver-23.3.6/ai/backend/web/
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6194 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17637 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/proxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    30139 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:13:24.189652 backend.ai-webserver-23.3.6/ai/backend/web/static/
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/asset-manifest.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4459 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/config.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/default.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:13:24.189652 backend.ai-webserver-23.3.6/ai/backend/web/static/dist/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:13:24.201652 backend.ai-webserver-23.3.6/ai/backend/web/static/dist/components/
+-rw-r--r--   0 runner    (1001) docker     (123)    19470 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/dist/components/backend-ai-agent-summary-view-2ee21519.js
+-rw-r--r--   0 runner    (1001) docker     (123)    82052 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/dist/components/backend-ai-agent-view-4f1cf328.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5578 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/dist/components/backend-ai-change-forgot-password-view-c3c64c37.js
+-rw-r--r--   0 runner    (1001) docker     (123)   125014 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/dist/components/backend-ai-credential-view-f1a0fa17.js
+-rw-r--r--   0 runner    (1001) docker     (123)   207666 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/dist/components/backend-ai-data-view-48c7459c.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6357 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/dist/components/backend-ai-edu-applauncher-b2bc846d.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4405 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/dist/components/backend-ai-email-verification-view-233abe92.js
+-rw-r--r--   0 runner    (1001) docker     (123)    87367 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/dist/components/backend-ai-environment-view-50d103c9.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/dist/components/backend-ai-error-view-dc4bd660.js
+-rw-r--r--   0 runner    (1001) docker     (123)    22282 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/dist/components/backend-ai-import-view-8d0888d2.js
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/dist/components/backend-ai-information-view-03c2890e.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3611 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/dist/components/backend-ai-list-status-5163ce5c.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7192 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/dist/components/backend-ai-maintenance-view-85a49dd0.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7919 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/dist/components/backend-ai-multi-select-ddd96cfb.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/dist/components/backend-ai-permission-denied-view-98eecd20.js
+-rw-r--r--   0 runner    (1001) docker     (123)    39157 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/dist/components/backend-ai-resource-monitor-3d648354.js
+-rw-r--r--   0 runner    (1001) docker     (123)   239617 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/dist/components/backend-ai-session-launcher-88b8173e.js
+-rw-r--r--   0 runner    (1001) docker     (123)   136463 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/dist/components/backend-ai-session-view-4aabdfe3.js
+-rw-r--r--   0 runner    (1001) docker     (123)    30793 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/dist/components/backend-ai-settings-view-5b62a307.js
+-rw-r--r--   0 runner    (1001) docker     (123)    59311 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/dist/components/backend-ai-statistics-view-557cd6bb.js
+-rw-r--r--   0 runner    (1001) docker     (123)    90679 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/dist/components/backend-ai-summary-view-59cccc2b.js
+-rw-r--r--   0 runner    (1001) docker     (123)    54694 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/dist/components/backend-ai-usersettings-view-625e99ca.js
+-rw-r--r--   0 runner    (1001) docker     (123)  1197377 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/dist/components/backend-ai-webui-661d9e43.js
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/dist/components/backend-ai-webui.js
+-rw-r--r--   0 runner    (1001) docker     (123)   202894 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/dist/components/chart-js-49cb22bc.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8543 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/dist/components/dir-utils-38e4cf3d.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5166 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/dist/components/expansion-9d1f3a9b.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/dist/components/json_to_csv-35c9e191.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10112 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/dist/components/label-1ef3652f.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4870 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/dist/components/lablup-activity-panel-0289184a.js
+-rw-r--r--   0 runner    (1001) docker     (123)   204073 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/dist/components/lablup-codemirror-04889726.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/dist/components/lablup-grid-sort-filter-column-9ffbb621.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/dist/components/lablup-loading-spinner-4649a250.js
+-rw-r--r--   0 runner    (1001) docker     (123)    17307 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/dist/components/lablup-progress-bar-095aec81.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/dist/components/media-query-controller-e400dd2c.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1682 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/dist/components/mwc-check-list-item-c64cf1a4.js
+-rw-r--r--   0 runner    (1001) docker     (123)    25704 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/dist/components/mwc-switch-e9473fc7.js
+-rw-r--r--   0 runner    (1001) docker     (123)    46306 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/dist/components/mwc-tab-bar-064ccbb5.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3152 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/dist/components/progress-spinner-153eedb3.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/dist/components/radio-behavior-b66ed7c9.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/dist/components/select-73255102.js
+-rw-r--r--   0 runner    (1001) docker     (123)    47299 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/dist/components/slider-cae179ae.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3028 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/dist/components/switch-1f68b491.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9151 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/dist/components/tab-group-6baff1e0.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/dist/components/textfield-6b6134ab.js
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/dist/components/translate-unsafe-html-861558b4.js
+-rw-r--r--   0 runner    (1001) docker     (123)    99653 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/dist/components/vaadin-grid-c3d5c3c2.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6300 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/dist/components/vaadin-grid-filter-column-4c9cb29f.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4108 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/dist/components/vaadin-grid-selection-column-f0bd0bf3.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6676 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/dist/components/vaadin-grid-sort-column-7bed08ef.js
+-rw-r--r--   0 runner    (1001) docker     (123)   246765 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/dist/components/vaadin-iconset-07d3debe.js
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/dist/components/vaadin-item-0d805f04.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/dist/components/vaadin-item-mixin-88cba3b7.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3211 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:13:24.201652 backend.ai-webserver-23.3.6/ai/backend/web/static/manifest/
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/manifest/app.js
+-rw-r--r--   0 runner    (1001) docker     (123)   134560 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/manifest/backend-ai.icns
+-rw-r--r--   0 runner    (1001) docker     (123)   370070 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/manifest/backend-ai.ico
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:13:24.201652 backend.ai-webserver-23.3.6/ai/backend/web/static/manifest/backend-ai.iconset/
+-rw-r--r--   0 runner    (1001) docker     (123)    10757 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/manifest/backend-ai.iconset/icon_128x128@1x.png
+-rw-r--r--   0 runner    (1001) docker     (123)    18546 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/manifest/backend-ai.iconset/icon_128x128@2x.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3489 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/manifest/backend-ai.iconset/icon_16x16@1x.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4568 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/manifest/backend-ai.iconset/icon_16x16@2x.png
+-rw-r--r--   0 runner    (1001) docker     (123)    18546 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/manifest/backend-ai.iconset/icon_256x256@1x.png
+-rw-r--r--   0 runner    (1001) docker     (123)    36092 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/manifest/backend-ai.iconset/icon_256x256@2x.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4568 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/manifest/backend-ai.iconset/icon_32x32@1x.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6561 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/manifest/backend-ai.iconset/icon_32x32@2x.png
+-rw-r--r--   0 runner    (1001) docker     (123)    36092 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/manifest/backend-ai.iconset/icon_512x512@1x.png
+-rw-r--r--   0 runner    (1001) docker     (123)   230498 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/manifest/backend-ai.iconset/icon_512x512@2x.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/manifest/backend.ai-brand-simple.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     6253 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/manifest/backend.ai-brand-white.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     6316 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/manifest/backend.ai-brand.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2952 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/manifest/backend.ai-text.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    15086 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/manifest/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/manifest.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:13:24.205652 backend.ai-webserver-23.3.6/ai/backend/web/static/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)     6620 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/resources/app_template.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3465 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/resources/badge-dark.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3809 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/resources/badge.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/resources/custom-kt.css
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/resources/custom-original.css
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/resources/custom.css
+-rw-r--r--   0 runner    (1001) docker     (123)     2216 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/resources/device_metadata.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:13:24.205652 backend.ai-webserver-23.3.6/ai/backend/web/static/resources/documents/
+-rw-r--r--   0 runner    (1001) docker     (123)    16782 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/resources/documents/privacy-policy.en.html
+-rw-r--r--   0 runner    (1001) docker     (123)    17867 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/resources/documents/privacy-policy.ko.html
+-rw-r--r--   0 runner    (1001) docker     (123)    45111 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/resources/documents/terms-of-service.en.html
+-rw-r--r--   0 runner    (1001) docker     (123)    48789 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/resources/documents/terms-of-service.ko.html
+-rw-r--r--   0 runner    (1001) docker     (123)   100353 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/resources/fashion-how-white.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   100242 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/resources/fashion-how.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:13:24.213652 backend.ai-webserver-23.3.6/ai/backend/web/static/resources/fonts/
+-rw-r--r--   0 runner    (1001) docker     (123)   141484 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/resources/fonts/MaterialIcons-Regular.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    99932 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/resources/fonts/MaterialIcons-Regular.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    60840 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/resources/fonts/MaterialIcons-Regular.woff2_
+-rw-r--r--   0 runner    (1001) docker     (123)    57620 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/resources/fonts/MaterialIcons-Regular.woff_
+-rw-r--r--   0 runner    (1001) docker     (123)    92136 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/resources/fonts/fa-brands-400.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    78460 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/resources/fonts/fa-brands-400.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    16772 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/resources/fonts/fa-regular-400.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    13548 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/resources/fonts/fa-regular-400.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)   104280 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/resources/fonts/fa-solid-900.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    80300 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/resources/fonts/fa-solid-900.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    58053 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/resources/fonts/font-awesome-all.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)    37094 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/resources/fonts/font-awesome.css
+-rw-r--r--   0 runner    (1001) docker     (123)     7575 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/resources/fonts/fonts.css
+-rw-r--r--   0 runner    (1001) docker     (123)    22500 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/resources/fonts/montserrat-v13-latin-100.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    18376 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/resources/fonts/montserrat-v13-latin-100.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    22888 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/resources/fonts/montserrat-v13-latin-100italic.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    18644 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/resources/fonts/montserrat-v13-latin-100italic.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    24012 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/resources/fonts/montserrat-v13-latin-italic.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    19660 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/resources/fonts/montserrat-v13-latin-italic.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    23480 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/resources/fonts/montserrat-v13-latin-regular.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    19172 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/resources/fonts/montserrat-v13-latin-regular.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    16252 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/resources/fonts/quicksand-v13-latin-300.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    12780 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/resources/fonts/quicksand-v13-latin-300.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    17072 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/resources/fonts/quicksand-v13-latin-500.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    13616 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/resources/fonts/quicksand-v13-latin-500.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    16152 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/resources/fonts/quicksand-v13-latin-700.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    13108 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/resources/fonts/quicksand-v13-latin-700.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    17032 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/resources/fonts/quicksand-v13-latin-regular.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    13760 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/resources/fonts/quicksand-v13-latin-regular.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    20368 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/resources/fonts/roboto-v19-latin-100.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    15808 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/resources/fonts/roboto-v19-latin-100.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    21704 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/resources/fonts/roboto-v19-latin-100italic.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    17008 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/resources/fonts/roboto-v19-latin-100italic.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    20348 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/resources/fonts/roboto-v19-latin-300.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    15784 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/resources/fonts/roboto-v19-latin-300.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    22204 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/resources/fonts/roboto-v19-latin-300italic.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    17448 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/resources/fonts/roboto-v19-latin-300italic.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    20392 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/resources/fonts/roboto-v19-latin-900.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    15712 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/resources/fonts/roboto-v19-latin-900.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    22304 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/resources/fonts/roboto-v19-latin-900italic.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    17520 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/resources/fonts/roboto-v19-latin-900italic.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    21952 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/resources/fonts/roboto-v19-latin-italic.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    17324 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/resources/fonts/roboto-v19-latin-italic.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    20268 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/resources/fonts/roboto-v19-latin-regular.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    15736 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/resources/fonts/roboto-v19-latin-regular.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    43900 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/resources/fonts/ubuntu-v14-latin-300.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    38108 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/resources/fonts/ubuntu-v14-latin-300.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    43092 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/resources/fonts/ubuntu-v14-latin-300italic.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    37548 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/resources/fonts/ubuntu-v14-latin-300italic.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    34688 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/resources/fonts/ubuntu-v14-latin-500.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    29864 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/resources/fonts/ubuntu-v14-latin-500.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    36836 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/resources/fonts/ubuntu-v14-latin-500italic.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    31748 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/resources/fonts/ubuntu-v14-latin-500italic.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    33424 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/resources/fonts/ubuntu-v14-latin-700.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    28968 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/resources/fonts/ubuntu-v14-latin-700.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    34668 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/resources/fonts/ubuntu-v14-latin-700italic.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    30092 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/resources/fonts/ubuntu-v14-latin-700italic.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    41016 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/resources/fonts/ubuntu-v14-latin-italic.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    35832 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/resources/fonts/ubuntu-v14-latin-italic.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    39164 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/resources/fonts/ubuntu-v14-latin-regular.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    34260 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/resources/fonts/ubuntu-v14-latin-regular.woff2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:13:24.217651 backend.ai-webserver-23.3.6/ai/backend/web/static/resources/i18n/
+-rw-r--r--   0 runner    (1001) docker     (123)    63323 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/resources/i18n/de.json
+-rw-r--r--   0 runner    (1001) docker     (123)    91324 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/resources/i18n/el.json
+-rw-r--r--   0 runner    (1001) docker     (123)    72187 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/resources/i18n/en.json
+-rw-r--r--   0 runner    (1001) docker     (123)    63733 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/resources/i18n/es.json
+-rw-r--r--   0 runner    (1001) docker     (123)    59666 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/resources/i18n/fi.json
+-rw-r--r--   0 runner    (1001) docker     (123)    75880 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/resources/i18n/fr.json
+-rw-r--r--   0 runner    (1001) docker     (123)    68882 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/resources/i18n/id.json
+-rw-r--r--   0 runner    (1001) docker     (123)    62630 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/resources/i18n/it.json
+-rw-r--r--   0 runner    (1001) docker     (123)    71153 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/resources/i18n/ja.json
+-rw-r--r--   0 runner    (1001) docker     (123)    84462 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/resources/i18n/ko.json
+-rw-r--r--   0 runner    (1001) docker     (123)    95092 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/resources/i18n/mn.json
+-rw-r--r--   0 runner    (1001) docker     (123)    58578 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/resources/i18n/ms.json
+-rw-r--r--   0 runner    (1001) docker     (123)    61937 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/resources/i18n/pl.json
+-rw-r--r--   0 runner    (1001) docker     (123)    61465 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/resources/i18n/pt.json
+-rw-r--r--   0 runner    (1001) docker     (123)    61520 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/resources/i18n/pt_BR.json
+-rw-r--r--   0 runner    (1001) docker     (123)    98637 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/resources/i18n/ru.json
+-rw-r--r--   0 runner    (1001) docker     (123)    60890 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/resources/i18n/tr.json
+-rw-r--r--   0 runner    (1001) docker     (123)    68337 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/resources/i18n/vi.json
+-rw-r--r--   0 runner    (1001) docker     (123)    53748 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/resources/i18n/zh_CN.json
+-rw-r--r--   0 runner    (1001) docker     (123)    53750 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/resources/i18n/zh_TW.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:13:24.225651 backend.ai-webserver-23.3.6/ai/backend/web/static/resources/icons/
+-rw-r--r--   0 runner    (1001) docker     (123)     1566 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/resources/icons/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)    21411 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/resources/icons/ROCm.png
+-rw-r--r--   0 runner    (1001) docker     (123)    20312 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/resources/icons/ROCm_black.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/resources/icons/apache-spark.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     5050 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/resources/icons/aws.png
+-rw-r--r--   0 runner    (1001) docker     (123)    12687 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/resources/icons/azure.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/resources/icons/c.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     5741 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/resources/icons/caffe.png
+-rw-r--r--   0 runner    (1001) docker     (123)      982 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/resources/icons/caffe2.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    28363 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/resources/icons/ceph.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5370 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/resources/icons/check-list.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3562 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/resources/icons/classification.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/resources/icons/cpp.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/resources/icons/default.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3113 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/resources/icons/default_app.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/resources/icons/file_type_cuda.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/resources/icons/file_type_python.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2925 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/resources/icons/filebrowser.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    15775 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/resources/icons/flux.png
+-rw-r--r--   0 runner    (1001) docker     (123)    10953 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/resources/icons/gcc.png
+-rw-r--r--   0 runner    (1001) docker     (123)    22672 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/resources/icons/gcp.png
+-rw-r--r--   0 runner    (1001) docker     (123)    11250 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/resources/icons/gdrive.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5602 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/resources/icons/h2o.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6649 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/resources/icons/haskell.png
+-rw-r--r--   0 runner    (1001) docker     (123)    31187 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/resources/icons/javascript.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3404 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/resources/icons/julia.png
+-rw-r--r--   0 runner    (1001) docker     (123)    16618 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/resources/icons/jupyter.png
+-rw-r--r--   0 runner    (1001) docker     (123)    46557 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/resources/icons/jupyterlab.png
+-rw-r--r--   0 runner    (1001) docker     (123)  1150358 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/resources/icons/kitty.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/resources/icons/lablup.png
+-rw-r--r--   0 runner    (1001) docker     (123)    18225 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/resources/icons/local.png
+-rw-r--r--   0 runner    (1001) docker     (123)    14460 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/resources/icons/lua.png
+-rw-r--r--   0 runner    (1001) docker     (123)    56266 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/resources/icons/matlab.png
+-rw-r--r--   0 runner    (1001) docker     (123)    25435 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/resources/icons/mlflow.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4404 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/resources/icons/mxnet.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     7280 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/resources/icons/nbp.png
+-rw-r--r--   0 runner    (1001) docker     (123)    13523 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/resources/icons/nni.png
+-rw-r--r--   0 runner    (1001) docker     (123)    15790 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/resources/icons/nni.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   144381 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/resources/icons/nodejs.png
+-rw-r--r--   0 runner    (1001) docker     (123)    11549 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/resources/icons/novnc.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     5557 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/resources/icons/nvidia.png
+-rw-r--r--   0 runner    (1001) docker     (123)    14684 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/resources/icons/octave.png
+-rw-r--r--   0 runner    (1001) docker     (123)     8349 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/resources/icons/openstack.png
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/resources/icons/orbit.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   150992 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/resources/icons/php.png
+-rw-r--r--   0 runner    (1001) docker     (123)    27901 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/resources/icons/purestorage.png
+-rw-r--r--   0 runner    (1001) docker     (123)   177194 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/resources/icons/python.png
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/resources/icons/pytorch.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/resources/icons/r-lang.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/resources/icons/rebel.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     5521 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/resources/icons/rust.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     5041 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/resources/icons/sftp.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3627 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/resources/icons/sftp2.png
+-rw-r--r--   0 runner    (1001) docker     (123)    51521 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/resources/icons/swift-tensorflow.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/resources/icons/swift.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     6965 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/resources/icons/tensorflow.png
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/resources/icons/terminal.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    15484 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/resources/icons/texlive.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2844 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/resources/icons/tpu.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/resources/icons/ubuntu.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     4446 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/resources/icons/vscode.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    67813 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/resources/icons/xfce.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2253 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/resources/icons/xrdp.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    26430 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/resources/image_metadata.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:13:24.225651 backend.ai-webserver-23.3.6/ai/backend/web/static/resources/images/
+-rw-r--r--   0 runner    (1001) docker     (123)  1352095 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/resources/images/401_unauthorized_access.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    62250 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/resources/images/404_not_found.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   103075 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/resources/images/launcher-background.png
+-rw-r--r--   0 runner    (1001) docker     (123)    84446 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/resources/images/loading-background-large.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    20788 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/resources/images/loading-background.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    19682 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/resources/images/web-terminal-guide-1.png
+-rw-r--r--   0 runner    (1001) docker     (123)    18386 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/resources/images/web-terminal-guide-2.png
+-rw-r--r--   0 runner    (1001) docker     (123)    69357 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/resources/images/web-terminal-guide-3.png
+-rw-r--r--   0 runner    (1001) docker     (123)    18296 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/resources/images/web-terminal-guide-4.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/resources/logo.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:13:24.225651 backend.ai-webserver-23.3.6/ai/backend/web/static/resources/menu_icons/
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/resources/menu_icons/icon_create_a_key_pair.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/resources/menu_icons/icon_keypair_management.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/resources/menu_icons/icon_upload_files.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2993 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/resources/storage_metadata.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:13:24.225651 backend.ai-webserver-23.3.6/ai/backend/web/static/resources/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     6717 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/resources/templates/under_construction.html
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/resources/theme.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4176 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/resources/webui.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:13:24.189652 backend.ai-webserver-23.3.6/ai/backend/web/static/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:13:24.225651 backend.ai-webserver-23.3.6/ai/backend/web/static/src/lib/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:13:24.229651 backend.ai-webserver-23.3.6/ai/backend/web/static/src/lib/bundles/
+-rw-r--r--   0 runner    (1001) docker     (123)    19998 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/src/lib/bundles/webcomponents-ce.js
+-rw-r--r--   0 runner    (1001) docker     (123)   129129 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/src/lib/bundles/webcomponents-ce.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)    10669 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/src/lib/bundles/webcomponents-pf_dom.js
+-rw-r--r--   0 runner    (1001) docker     (123)    45370 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/src/lib/bundles/webcomponents-pf_dom.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)    14541 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/src/lib/bundles/webcomponents-pf_js.js
+-rw-r--r--   0 runner    (1001) docker     (123)    53114 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/src/lib/bundles/webcomponents-pf_js.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)   133025 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/src/lib/bundles/webcomponents-sd-ce-pf.js
+-rw-r--r--   0 runner    (1001) docker     (123)   806549 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/src/lib/bundles/webcomponents-sd-ce-pf.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)    95511 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/src/lib/bundles/webcomponents-sd-ce.js
+-rw-r--r--   0 runner    (1001) docker     (123)   630748 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/src/lib/bundles/webcomponents-sd-ce.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)    76437 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/src/lib/bundles/webcomponents-sd.js
+-rw-r--r--   0 runner    (1001) docker     (123)   501551 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/src/lib/bundles/webcomponents-sd.js.map
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:13:24.229651 backend.ai-webserver-23.3.6/ai/backend/web/static/src/lib/web-animations-js/
+-rw-r--r--   0 runner    (1001) docker     (123)    50580 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/src/lib/web-animations-js/web-animations-next-lite.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7773 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/src/lib/webcomponents-loader.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:13:24.189652 backend.ai-webserver-23.3.6/ai/backend/web/static/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:13:24.237651 backend.ai-webserver-23.3.6/ai/backend/web/static/static/js/
+-rw-r--r--   0 runner    (1001) docker     (123)   154086 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/static/js/149.924fa2a6.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/static/js/149.924fa2a6.chunk.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   623058 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/static/js/149.924fa2a6.chunk.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)     6739 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/static/js/478.8c8fd27b.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (123)    22813 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/static/js/478.8c8fd27b.chunk.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)   164411 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/static/js/488.70f8dcf6.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/static/js/488.70f8dcf6.chunk.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   666043 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/static/js/488.70f8dcf6.chunk.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)     7801 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/static/js/540.c51503fa.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (123)    23524 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/static/js/540.c51503fa.chunk.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)    82120 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/static/js/558.9310b842.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (123)   261609 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/static/js/558.9310b842.chunk.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)    84119 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/static/js/618.fdb02897.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (123)   318442 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/static/js/618.fdb02897.chunk.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)   149146 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/static/js/627.a131ed07.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (123)   615392 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/static/js/627.a131ed07.chunk.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)     3020 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/static/js/818.9b28dc99.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7181 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/static/js/818.9b28dc99.chunk.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)   152760 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/static/js/main.8f973991.js
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/static/js/main.8f973991.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   395128 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/static/js/main.8f973991.js.map
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:13:24.237651 backend.ai-webserver-23.3.6/ai/backend/web/static/static/media/
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/static/media/getFetch.40f37ddea2378391108f.cjs
+-rw-r--r--   0 runner    (1001) docker     (123)     6772 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/sw.js
+-rw-r--r--   0 runner    (1001) docker     (123)    11027 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/sw.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/version.json
+-rw-r--r--   0 runner    (1001) docker     (123)    14328 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/workbox-d249b2c8.js
+-rw-r--r--   0 runner    (1001) docker     (123)   137419 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/static/workbox-d249b2c8.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)     4333 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2981 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/template.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:13:24.237651 backend.ai-webserver-23.3.6/ai/backend/web/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     3035 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/templates/config.toml.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/ai/backend/web/templates/config_ini.toml.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:13:24.237651 backend.ai-webserver-23.3.6/backend.ai_webserver.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3014 2023-06-14 11:13:24.000000 backend.ai-webserver-23.3.6/backend.ai_webserver.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17896 2023-06-14 11:13:24.000000 backend.ai-webserver-23.3.6/backend.ai_webserver.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 11:13:24.000000 backend.ai-webserver-23.3.6/backend.ai_webserver.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 11:13:24.000000 backend.ai-webserver-23.3.6/backend.ai_webserver.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 11:13:23.000000 backend.ai-webserver-23.3.6/backend.ai_webserver.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-06-14 11:13:24.000000 backend.ai-webserver-23.3.6/backend.ai_webserver.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-06-14 11:13:24.000000 backend.ai-webserver-23.3.6/backend.ai_webserver.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/backend_shim.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 11:13:24.237651 backend.ai-webserver-23.3.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)    21479 2023-06-14 11:13:22.000000 backend.ai-webserver-23.3.6/setup.py
```

### Comparing `backend.ai-webserver-23.3.5/PKG-INFO` & `backend.ai-webserver-23.3.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: backend.ai-webserver
-Version: 23.3.5
+Version: 23.3.6
 Summary: Backend.AI WebUI Host
 Home-page: https://github.com/lablup/backend.ai
 Author: Lablup Inc. and contributors
 License: LGPLv3
 Project-URL: Documentation, https://docs.backend.ai/
 Project-URL: Source, https://github.com/lablup/backend.ai
 Classifier: Intended Audience :: Developers
```

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/auth.py` & `backend.ai-webserver-23.3.6/ai/backend/web/auth.py`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/config.py` & `backend.ai-webserver-23.3.6/ai/backend/web/config.py`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/logging.py` & `backend.ai-webserver-23.3.6/ai/backend/web/logging.py`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/proxy.py` & `backend.ai-webserver-23.3.6/ai/backend/web/proxy.py`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/server.py` & `backend.ai-webserver-23.3.6/ai/backend/web/server.py`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/asset-manifest.json` & `backend.ai-webserver-23.3.6/ai/backend/web/static/asset-manifest.json`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/config.toml` & `backend.ai-webserver-23.3.6/ai/backend/web/static/config.toml`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/dist/components/backend-ai-agent-summary-view-2ee21519.js` & `backend.ai-webserver-23.3.6/ai/backend/web/static/dist/components/backend-ai-agent-summary-view-2ee21519.js`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/dist/components/backend-ai-agent-view-4f1cf328.js` & `backend.ai-webserver-23.3.6/ai/backend/web/static/dist/components/backend-ai-agent-view-4f1cf328.js`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/dist/components/backend-ai-change-forgot-password-view-c3c64c37.js` & `backend.ai-webserver-23.3.6/ai/backend/web/static/dist/components/backend-ai-change-forgot-password-view-c3c64c37.js`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/dist/components/backend-ai-credential-view-f1a0fa17.js` & `backend.ai-webserver-23.3.6/ai/backend/web/static/dist/components/backend-ai-credential-view-f1a0fa17.js`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/dist/components/backend-ai-data-view-48c7459c.js` & `backend.ai-webserver-23.3.6/ai/backend/web/static/dist/components/backend-ai-data-view-48c7459c.js`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/dist/components/backend-ai-edu-applauncher-b2bc846d.js` & `backend.ai-webserver-23.3.6/ai/backend/web/static/dist/components/backend-ai-edu-applauncher-b2bc846d.js`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/dist/components/backend-ai-email-verification-view-233abe92.js` & `backend.ai-webserver-23.3.6/ai/backend/web/static/dist/components/backend-ai-email-verification-view-233abe92.js`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/dist/components/backend-ai-environment-view-50d103c9.js` & `backend.ai-webserver-23.3.6/ai/backend/web/static/dist/components/backend-ai-environment-view-50d103c9.js`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/dist/components/backend-ai-error-view-dc4bd660.js` & `backend.ai-webserver-23.3.6/ai/backend/web/static/dist/components/backend-ai-error-view-dc4bd660.js`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/dist/components/backend-ai-import-view-8d0888d2.js` & `backend.ai-webserver-23.3.6/ai/backend/web/static/dist/components/backend-ai-import-view-8d0888d2.js`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/dist/components/backend-ai-list-status-5163ce5c.js` & `backend.ai-webserver-23.3.6/ai/backend/web/static/dist/components/backend-ai-list-status-5163ce5c.js`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/dist/components/backend-ai-maintenance-view-85a49dd0.js` & `backend.ai-webserver-23.3.6/ai/backend/web/static/dist/components/backend-ai-maintenance-view-85a49dd0.js`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/dist/components/backend-ai-multi-select-ddd96cfb.js` & `backend.ai-webserver-23.3.6/ai/backend/web/static/dist/components/backend-ai-multi-select-ddd96cfb.js`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/dist/components/backend-ai-permission-denied-view-98eecd20.js` & `backend.ai-webserver-23.3.6/ai/backend/web/static/dist/components/backend-ai-permission-denied-view-98eecd20.js`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/dist/components/backend-ai-resource-monitor-3d648354.js` & `backend.ai-webserver-23.3.6/ai/backend/web/static/dist/components/backend-ai-resource-monitor-3d648354.js`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/dist/components/backend-ai-session-launcher-88b8173e.js` & `backend.ai-webserver-23.3.6/ai/backend/web/static/dist/components/backend-ai-session-launcher-88b8173e.js`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/dist/components/backend-ai-session-view-4aabdfe3.js` & `backend.ai-webserver-23.3.6/ai/backend/web/static/dist/components/backend-ai-session-view-4aabdfe3.js`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/dist/components/backend-ai-settings-view-5b62a307.js` & `backend.ai-webserver-23.3.6/ai/backend/web/static/dist/components/backend-ai-settings-view-5b62a307.js`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/dist/components/backend-ai-statistics-view-557cd6bb.js` & `backend.ai-webserver-23.3.6/ai/backend/web/static/dist/components/backend-ai-statistics-view-557cd6bb.js`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/dist/components/backend-ai-summary-view-59cccc2b.js` & `backend.ai-webserver-23.3.6/ai/backend/web/static/dist/components/backend-ai-summary-view-59cccc2b.js`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/dist/components/backend-ai-usersettings-view-625e99ca.js` & `backend.ai-webserver-23.3.6/ai/backend/web/static/dist/components/backend-ai-usersettings-view-625e99ca.js`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/dist/components/backend-ai-webui-661d9e43.js` & `backend.ai-webserver-23.3.6/ai/backend/web/static/dist/components/backend-ai-webui-661d9e43.js`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/dist/components/chart-js-49cb22bc.js` & `backend.ai-webserver-23.3.6/ai/backend/web/static/dist/components/chart-js-49cb22bc.js`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/dist/components/dir-utils-38e4cf3d.js` & `backend.ai-webserver-23.3.6/ai/backend/web/static/dist/components/dir-utils-38e4cf3d.js`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/dist/components/expansion-9d1f3a9b.js` & `backend.ai-webserver-23.3.6/ai/backend/web/static/dist/components/expansion-9d1f3a9b.js`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/dist/components/json_to_csv-35c9e191.js` & `backend.ai-webserver-23.3.6/ai/backend/web/static/dist/components/json_to_csv-35c9e191.js`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/dist/components/label-1ef3652f.js` & `backend.ai-webserver-23.3.6/ai/backend/web/static/dist/components/label-1ef3652f.js`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/dist/components/lablup-activity-panel-0289184a.js` & `backend.ai-webserver-23.3.6/ai/backend/web/static/dist/components/lablup-activity-panel-0289184a.js`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/dist/components/lablup-codemirror-04889726.js` & `backend.ai-webserver-23.3.6/ai/backend/web/static/dist/components/lablup-codemirror-04889726.js`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/dist/components/lablup-grid-sort-filter-column-9ffbb621.js` & `backend.ai-webserver-23.3.6/ai/backend/web/static/dist/components/lablup-grid-sort-filter-column-9ffbb621.js`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/dist/components/lablup-loading-spinner-4649a250.js` & `backend.ai-webserver-23.3.6/ai/backend/web/static/dist/components/lablup-loading-spinner-4649a250.js`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/dist/components/lablup-progress-bar-095aec81.js` & `backend.ai-webserver-23.3.6/ai/backend/web/static/dist/components/lablup-progress-bar-095aec81.js`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/dist/components/media-query-controller-e400dd2c.js` & `backend.ai-webserver-23.3.6/ai/backend/web/static/dist/components/media-query-controller-e400dd2c.js`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/dist/components/mwc-check-list-item-c64cf1a4.js` & `backend.ai-webserver-23.3.6/ai/backend/web/static/dist/components/mwc-check-list-item-c64cf1a4.js`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/dist/components/mwc-switch-e9473fc7.js` & `backend.ai-webserver-23.3.6/ai/backend/web/static/dist/components/mwc-switch-e9473fc7.js`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/dist/components/mwc-tab-bar-064ccbb5.js` & `backend.ai-webserver-23.3.6/ai/backend/web/static/dist/components/mwc-tab-bar-064ccbb5.js`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/dist/components/progress-spinner-153eedb3.js` & `backend.ai-webserver-23.3.6/ai/backend/web/static/dist/components/progress-spinner-153eedb3.js`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/dist/components/radio-behavior-b66ed7c9.js` & `backend.ai-webserver-23.3.6/ai/backend/web/static/dist/components/radio-behavior-b66ed7c9.js`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/dist/components/select-73255102.js` & `backend.ai-webserver-23.3.6/ai/backend/web/static/dist/components/select-73255102.js`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/dist/components/slider-cae179ae.js` & `backend.ai-webserver-23.3.6/ai/backend/web/static/dist/components/slider-cae179ae.js`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/dist/components/switch-1f68b491.js` & `backend.ai-webserver-23.3.6/ai/backend/web/static/dist/components/switch-1f68b491.js`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/dist/components/tab-group-6baff1e0.js` & `backend.ai-webserver-23.3.6/ai/backend/web/static/dist/components/tab-group-6baff1e0.js`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/dist/components/textfield-6b6134ab.js` & `backend.ai-webserver-23.3.6/ai/backend/web/static/dist/components/textfield-6b6134ab.js`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/dist/components/vaadin-grid-c3d5c3c2.js` & `backend.ai-webserver-23.3.6/ai/backend/web/static/dist/components/vaadin-grid-c3d5c3c2.js`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/dist/components/vaadin-grid-filter-column-4c9cb29f.js` & `backend.ai-webserver-23.3.6/ai/backend/web/static/dist/components/vaadin-grid-filter-column-4c9cb29f.js`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/dist/components/vaadin-grid-selection-column-f0bd0bf3.js` & `backend.ai-webserver-23.3.6/ai/backend/web/static/dist/components/vaadin-grid-selection-column-f0bd0bf3.js`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/dist/components/vaadin-grid-sort-column-7bed08ef.js` & `backend.ai-webserver-23.3.6/ai/backend/web/static/dist/components/vaadin-grid-sort-column-7bed08ef.js`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/dist/components/vaadin-iconset-07d3debe.js` & `backend.ai-webserver-23.3.6/ai/backend/web/static/dist/components/vaadin-iconset-07d3debe.js`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/dist/components/vaadin-item-0d805f04.js` & `backend.ai-webserver-23.3.6/ai/backend/web/static/dist/components/vaadin-item-0d805f04.js`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/dist/components/vaadin-item-mixin-88cba3b7.js` & `backend.ai-webserver-23.3.6/ai/backend/web/static/dist/components/vaadin-item-mixin-88cba3b7.js`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/index.html` & `backend.ai-webserver-23.3.6/ai/backend/web/static/index.html`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/manifest/app.js` & `backend.ai-webserver-23.3.6/ai/backend/web/static/manifest/app.js`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/manifest/backend-ai.icns` & `backend.ai-webserver-23.3.6/ai/backend/web/static/manifest/backend-ai.icns`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/manifest/backend-ai.ico` & `backend.ai-webserver-23.3.6/ai/backend/web/static/manifest/backend-ai.ico`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/manifest/backend-ai.iconset/icon_128x128@1x.png` & `backend.ai-webserver-23.3.6/ai/backend/web/static/manifest/backend-ai.iconset/icon_128x128@1x.png`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/manifest/backend-ai.iconset/icon_128x128@2x.png` & `backend.ai-webserver-23.3.6/ai/backend/web/static/manifest/backend-ai.iconset/icon_128x128@2x.png`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/manifest/backend-ai.iconset/icon_16x16@1x.png` & `backend.ai-webserver-23.3.6/ai/backend/web/static/manifest/backend-ai.iconset/icon_16x16@1x.png`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/manifest/backend-ai.iconset/icon_16x16@2x.png` & `backend.ai-webserver-23.3.6/ai/backend/web/static/manifest/backend-ai.iconset/icon_16x16@2x.png`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/manifest/backend-ai.iconset/icon_256x256@1x.png` & `backend.ai-webserver-23.3.6/ai/backend/web/static/manifest/backend-ai.iconset/icon_256x256@1x.png`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/manifest/backend-ai.iconset/icon_256x256@2x.png` & `backend.ai-webserver-23.3.6/ai/backend/web/static/manifest/backend-ai.iconset/icon_256x256@2x.png`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/manifest/backend-ai.iconset/icon_32x32@1x.png` & `backend.ai-webserver-23.3.6/ai/backend/web/static/manifest/backend-ai.iconset/icon_32x32@1x.png`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/manifest/backend-ai.iconset/icon_32x32@2x.png` & `backend.ai-webserver-23.3.6/ai/backend/web/static/manifest/backend-ai.iconset/icon_32x32@2x.png`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/manifest/backend-ai.iconset/icon_512x512@1x.png` & `backend.ai-webserver-23.3.6/ai/backend/web/static/manifest/backend-ai.iconset/icon_512x512@1x.png`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/manifest/backend-ai.iconset/icon_512x512@2x.png` & `backend.ai-webserver-23.3.6/ai/backend/web/static/manifest/backend-ai.iconset/icon_512x512@2x.png`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/manifest/backend.ai-brand-simple.svg` & `backend.ai-webserver-23.3.6/ai/backend/web/static/manifest/backend.ai-brand-simple.svg`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/manifest/backend.ai-brand-white.svg` & `backend.ai-webserver-23.3.6/ai/backend/web/static/manifest/backend.ai-brand-white.svg`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/manifest/backend.ai-brand.svg` & `backend.ai-webserver-23.3.6/ai/backend/web/static/manifest/backend.ai-brand.svg`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/manifest/backend.ai-text.svg` & `backend.ai-webserver-23.3.6/ai/backend/web/static/manifest/backend.ai-text.svg`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/manifest/favicon.ico` & `backend.ai-webserver-23.3.6/ai/backend/web/static/manifest/favicon.ico`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/manifest.json` & `backend.ai-webserver-23.3.6/ai/backend/web/static/manifest.json`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/resources/app_template.json` & `backend.ai-webserver-23.3.6/ai/backend/web/static/resources/app_template.json`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/resources/badge-dark.svg` & `backend.ai-webserver-23.3.6/ai/backend/web/static/resources/badge-dark.svg`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/resources/badge.svg` & `backend.ai-webserver-23.3.6/ai/backend/web/static/resources/badge.svg`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/resources/custom-kt.css` & `backend.ai-webserver-23.3.6/ai/backend/web/static/resources/custom-kt.css`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/resources/device_metadata.json` & `backend.ai-webserver-23.3.6/ai/backend/web/static/resources/device_metadata.json`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/resources/documents/privacy-policy.en.html` & `backend.ai-webserver-23.3.6/ai/backend/web/static/resources/documents/privacy-policy.en.html`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/resources/documents/privacy-policy.ko.html` & `backend.ai-webserver-23.3.6/ai/backend/web/static/resources/documents/privacy-policy.ko.html`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/resources/documents/terms-of-service.en.html` & `backend.ai-webserver-23.3.6/ai/backend/web/static/resources/documents/terms-of-service.en.html`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/resources/documents/terms-of-service.ko.html` & `backend.ai-webserver-23.3.6/ai/backend/web/static/resources/documents/terms-of-service.ko.html`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/resources/fashion-how-white.svg` & `backend.ai-webserver-23.3.6/ai/backend/web/static/resources/fashion-how-white.svg`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/resources/fashion-how.svg` & `backend.ai-webserver-23.3.6/ai/backend/web/static/resources/fashion-how.svg`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/resources/fonts/MaterialIcons-Regular.woff` & `backend.ai-webserver-23.3.6/ai/backend/web/static/resources/fonts/MaterialIcons-Regular.woff`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/resources/fonts/MaterialIcons-Regular.woff2` & `backend.ai-webserver-23.3.6/ai/backend/web/static/resources/fonts/MaterialIcons-Regular.woff2`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/resources/fonts/MaterialIcons-Regular.woff2_` & `backend.ai-webserver-23.3.6/ai/backend/web/static/resources/fonts/MaterialIcons-Regular.woff2_`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/resources/fonts/MaterialIcons-Regular.woff_` & `backend.ai-webserver-23.3.6/ai/backend/web/static/resources/fonts/MaterialIcons-Regular.woff_`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/resources/fonts/fa-brands-400.woff` & `backend.ai-webserver-23.3.6/ai/backend/web/static/resources/fonts/fa-brands-400.woff`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/resources/fonts/fa-brands-400.woff2` & `backend.ai-webserver-23.3.6/ai/backend/web/static/resources/fonts/fa-brands-400.woff2`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/resources/fonts/fa-regular-400.woff` & `backend.ai-webserver-23.3.6/ai/backend/web/static/resources/fonts/fa-regular-400.woff`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/resources/fonts/fa-regular-400.woff2` & `backend.ai-webserver-23.3.6/ai/backend/web/static/resources/fonts/fa-regular-400.woff2`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/resources/fonts/fa-solid-900.woff` & `backend.ai-webserver-23.3.6/ai/backend/web/static/resources/fonts/fa-solid-900.woff`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/resources/fonts/fa-solid-900.woff2` & `backend.ai-webserver-23.3.6/ai/backend/web/static/resources/fonts/fa-solid-900.woff2`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/resources/fonts/font-awesome-all.min.css` & `backend.ai-webserver-23.3.6/ai/backend/web/static/resources/fonts/font-awesome-all.min.css`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/resources/fonts/font-awesome.css` & `backend.ai-webserver-23.3.6/ai/backend/web/static/resources/fonts/font-awesome.css`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/resources/fonts/fonts.css` & `backend.ai-webserver-23.3.6/ai/backend/web/static/resources/fonts/fonts.css`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/resources/fonts/montserrat-v13-latin-100.woff` & `backend.ai-webserver-23.3.6/ai/backend/web/static/resources/fonts/montserrat-v13-latin-100.woff`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/resources/fonts/montserrat-v13-latin-100.woff2` & `backend.ai-webserver-23.3.6/ai/backend/web/static/resources/fonts/montserrat-v13-latin-100.woff2`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/resources/fonts/montserrat-v13-latin-100italic.woff` & `backend.ai-webserver-23.3.6/ai/backend/web/static/resources/fonts/montserrat-v13-latin-100italic.woff`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/resources/fonts/montserrat-v13-latin-100italic.woff2` & `backend.ai-webserver-23.3.6/ai/backend/web/static/resources/fonts/montserrat-v13-latin-100italic.woff2`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/resources/fonts/montserrat-v13-latin-italic.woff` & `backend.ai-webserver-23.3.6/ai/backend/web/static/resources/fonts/montserrat-v13-latin-italic.woff`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/resources/fonts/montserrat-v13-latin-italic.woff2` & `backend.ai-webserver-23.3.6/ai/backend/web/static/resources/fonts/montserrat-v13-latin-italic.woff2`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/resources/fonts/montserrat-v13-latin-regular.woff` & `backend.ai-webserver-23.3.6/ai/backend/web/static/resources/fonts/montserrat-v13-latin-regular.woff`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/resources/fonts/montserrat-v13-latin-regular.woff2` & `backend.ai-webserver-23.3.6/ai/backend/web/static/resources/fonts/montserrat-v13-latin-regular.woff2`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/resources/fonts/quicksand-v13-latin-300.woff` & `backend.ai-webserver-23.3.6/ai/backend/web/static/resources/fonts/quicksand-v13-latin-300.woff`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/resources/fonts/quicksand-v13-latin-300.woff2` & `backend.ai-webserver-23.3.6/ai/backend/web/static/resources/fonts/quicksand-v13-latin-300.woff2`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/resources/fonts/quicksand-v13-latin-500.woff` & `backend.ai-webserver-23.3.6/ai/backend/web/static/resources/fonts/quicksand-v13-latin-500.woff`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/resources/fonts/quicksand-v13-latin-500.woff2` & `backend.ai-webserver-23.3.6/ai/backend/web/static/resources/fonts/quicksand-v13-latin-500.woff2`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/resources/fonts/quicksand-v13-latin-700.woff` & `backend.ai-webserver-23.3.6/ai/backend/web/static/resources/fonts/quicksand-v13-latin-700.woff`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/resources/fonts/quicksand-v13-latin-700.woff2` & `backend.ai-webserver-23.3.6/ai/backend/web/static/resources/fonts/quicksand-v13-latin-700.woff2`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/resources/fonts/quicksand-v13-latin-regular.woff` & `backend.ai-webserver-23.3.6/ai/backend/web/static/resources/fonts/quicksand-v13-latin-regular.woff`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/resources/fonts/quicksand-v13-latin-regular.woff2` & `backend.ai-webserver-23.3.6/ai/backend/web/static/resources/fonts/quicksand-v13-latin-regular.woff2`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/resources/fonts/roboto-v19-latin-100.woff` & `backend.ai-webserver-23.3.6/ai/backend/web/static/resources/fonts/roboto-v19-latin-100.woff`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/resources/fonts/roboto-v19-latin-100.woff2` & `backend.ai-webserver-23.3.6/ai/backend/web/static/resources/fonts/roboto-v19-latin-100.woff2`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/resources/fonts/roboto-v19-latin-100italic.woff` & `backend.ai-webserver-23.3.6/ai/backend/web/static/resources/fonts/roboto-v19-latin-100italic.woff`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/resources/fonts/roboto-v19-latin-100italic.woff2` & `backend.ai-webserver-23.3.6/ai/backend/web/static/resources/fonts/roboto-v19-latin-100italic.woff2`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/resources/fonts/roboto-v19-latin-300.woff` & `backend.ai-webserver-23.3.6/ai/backend/web/static/resources/fonts/roboto-v19-latin-300.woff`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/resources/fonts/roboto-v19-latin-300.woff2` & `backend.ai-webserver-23.3.6/ai/backend/web/static/resources/fonts/roboto-v19-latin-300.woff2`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/resources/fonts/roboto-v19-latin-300italic.woff` & `backend.ai-webserver-23.3.6/ai/backend/web/static/resources/fonts/roboto-v19-latin-300italic.woff`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/resources/fonts/roboto-v19-latin-300italic.woff2` & `backend.ai-webserver-23.3.6/ai/backend/web/static/resources/fonts/roboto-v19-latin-300italic.woff2`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/resources/fonts/roboto-v19-latin-900.woff` & `backend.ai-webserver-23.3.6/ai/backend/web/static/resources/fonts/roboto-v19-latin-900.woff`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/resources/fonts/roboto-v19-latin-900.woff2` & `backend.ai-webserver-23.3.6/ai/backend/web/static/resources/fonts/roboto-v19-latin-900.woff2`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/resources/fonts/roboto-v19-latin-900italic.woff` & `backend.ai-webserver-23.3.6/ai/backend/web/static/resources/fonts/roboto-v19-latin-900italic.woff`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/resources/fonts/roboto-v19-latin-900italic.woff2` & `backend.ai-webserver-23.3.6/ai/backend/web/static/resources/fonts/roboto-v19-latin-900italic.woff2`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/resources/fonts/roboto-v19-latin-italic.woff` & `backend.ai-webserver-23.3.6/ai/backend/web/static/resources/fonts/roboto-v19-latin-italic.woff`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/resources/fonts/roboto-v19-latin-italic.woff2` & `backend.ai-webserver-23.3.6/ai/backend/web/static/resources/fonts/roboto-v19-latin-italic.woff2`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/resources/fonts/roboto-v19-latin-regular.woff` & `backend.ai-webserver-23.3.6/ai/backend/web/static/resources/fonts/roboto-v19-latin-regular.woff`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/resources/fonts/roboto-v19-latin-regular.woff2` & `backend.ai-webserver-23.3.6/ai/backend/web/static/resources/fonts/roboto-v19-latin-regular.woff2`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/resources/fonts/ubuntu-v14-latin-300.woff` & `backend.ai-webserver-23.3.6/ai/backend/web/static/resources/fonts/ubuntu-v14-latin-300.woff`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/resources/fonts/ubuntu-v14-latin-300.woff2` & `backend.ai-webserver-23.3.6/ai/backend/web/static/resources/fonts/ubuntu-v14-latin-300.woff2`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/resources/fonts/ubuntu-v14-latin-300italic.woff` & `backend.ai-webserver-23.3.6/ai/backend/web/static/resources/fonts/ubuntu-v14-latin-300italic.woff`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/resources/fonts/ubuntu-v14-latin-300italic.woff2` & `backend.ai-webserver-23.3.6/ai/backend/web/static/resources/fonts/ubuntu-v14-latin-300italic.woff2`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/resources/fonts/ubuntu-v14-latin-500.woff` & `backend.ai-webserver-23.3.6/ai/backend/web/static/resources/fonts/ubuntu-v14-latin-500.woff`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/resources/fonts/ubuntu-v14-latin-500.woff2` & `backend.ai-webserver-23.3.6/ai/backend/web/static/resources/fonts/ubuntu-v14-latin-500.woff2`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/resources/fonts/ubuntu-v14-latin-500italic.woff` & `backend.ai-webserver-23.3.6/ai/backend/web/static/resources/fonts/ubuntu-v14-latin-500italic.woff`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/resources/fonts/ubuntu-v14-latin-500italic.woff2` & `backend.ai-webserver-23.3.6/ai/backend/web/static/resources/fonts/ubuntu-v14-latin-500italic.woff2`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/resources/fonts/ubuntu-v14-latin-700.woff` & `backend.ai-webserver-23.3.6/ai/backend/web/static/resources/fonts/ubuntu-v14-latin-700.woff`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/resources/fonts/ubuntu-v14-latin-700.woff2` & `backend.ai-webserver-23.3.6/ai/backend/web/static/resources/fonts/ubuntu-v14-latin-700.woff2`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/resources/fonts/ubuntu-v14-latin-700italic.woff` & `backend.ai-webserver-23.3.6/ai/backend/web/static/resources/fonts/ubuntu-v14-latin-700italic.woff`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/resources/fonts/ubuntu-v14-latin-700italic.woff2` & `backend.ai-webserver-23.3.6/ai/backend/web/static/resources/fonts/ubuntu-v14-latin-700italic.woff2`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/resources/fonts/ubuntu-v14-latin-italic.woff` & `backend.ai-webserver-23.3.6/ai/backend/web/static/resources/fonts/ubuntu-v14-latin-italic.woff`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/resources/fonts/ubuntu-v14-latin-italic.woff2` & `backend.ai-webserver-23.3.6/ai/backend/web/static/resources/fonts/ubuntu-v14-latin-italic.woff2`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/resources/fonts/ubuntu-v14-latin-regular.woff` & `backend.ai-webserver-23.3.6/ai/backend/web/static/resources/fonts/ubuntu-v14-latin-regular.woff`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/resources/fonts/ubuntu-v14-latin-regular.woff2` & `backend.ai-webserver-23.3.6/ai/backend/web/static/resources/fonts/ubuntu-v14-latin-regular.woff2`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/resources/i18n/de.json` & `backend.ai-webserver-23.3.6/ai/backend/web/static/resources/i18n/de.json`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/resources/i18n/el.json` & `backend.ai-webserver-23.3.6/ai/backend/web/static/resources/i18n/el.json`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/resources/i18n/en.json` & `backend.ai-webserver-23.3.6/ai/backend/web/static/resources/i18n/en.json`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/resources/i18n/es.json` & `backend.ai-webserver-23.3.6/ai/backend/web/static/resources/i18n/es.json`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/resources/i18n/fi.json` & `backend.ai-webserver-23.3.6/ai/backend/web/static/resources/i18n/fi.json`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/resources/i18n/fr.json` & `backend.ai-webserver-23.3.6/ai/backend/web/static/resources/i18n/fr.json`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/resources/i18n/id.json` & `backend.ai-webserver-23.3.6/ai/backend/web/static/resources/i18n/id.json`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/resources/i18n/it.json` & `backend.ai-webserver-23.3.6/ai/backend/web/static/resources/i18n/it.json`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/resources/i18n/ja.json` & `backend.ai-webserver-23.3.6/ai/backend/web/static/resources/i18n/ja.json`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/resources/i18n/ko.json` & `backend.ai-webserver-23.3.6/ai/backend/web/static/resources/i18n/ko.json`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/resources/i18n/mn.json` & `backend.ai-webserver-23.3.6/ai/backend/web/static/resources/i18n/mn.json`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/resources/i18n/ms.json` & `backend.ai-webserver-23.3.6/ai/backend/web/static/resources/i18n/ms.json`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/resources/i18n/pl.json` & `backend.ai-webserver-23.3.6/ai/backend/web/static/resources/i18n/pl.json`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/resources/i18n/pt.json` & `backend.ai-webserver-23.3.6/ai/backend/web/static/resources/i18n/pt.json`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/resources/i18n/pt_BR.json` & `backend.ai-webserver-23.3.6/ai/backend/web/static/resources/i18n/pt_BR.json`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/resources/i18n/ru.json` & `backend.ai-webserver-23.3.6/ai/backend/web/static/resources/i18n/ru.json`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/resources/i18n/tr.json` & `backend.ai-webserver-23.3.6/ai/backend/web/static/resources/i18n/tr.json`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/resources/i18n/vi.json` & `backend.ai-webserver-23.3.6/ai/backend/web/static/resources/i18n/vi.json`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/resources/i18n/zh_CN.json` & `backend.ai-webserver-23.3.6/ai/backend/web/static/resources/i18n/zh_CN.json`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/resources/i18n/zh_TW.json` & `backend.ai-webserver-23.3.6/ai/backend/web/static/resources/i18n/zh_TW.json`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/resources/icons/LICENSE.md` & `backend.ai-webserver-23.3.6/ai/backend/web/static/resources/icons/LICENSE.md`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/resources/icons/ROCm.png` & `backend.ai-webserver-23.3.6/ai/backend/web/static/resources/icons/ROCm.png`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/resources/icons/ROCm_black.png` & `backend.ai-webserver-23.3.6/ai/backend/web/static/resources/icons/ROCm_black.png`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/resources/icons/apache-spark.svg` & `backend.ai-webserver-23.3.6/ai/backend/web/static/resources/icons/apache-spark.svg`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/resources/icons/aws.png` & `backend.ai-webserver-23.3.6/ai/backend/web/static/resources/icons/aws.png`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/resources/icons/azure.png` & `backend.ai-webserver-23.3.6/ai/backend/web/static/resources/icons/azure.png`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/resources/icons/c.svg` & `backend.ai-webserver-23.3.6/ai/backend/web/static/resources/icons/c.svg`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/resources/icons/caffe.png` & `backend.ai-webserver-23.3.6/ai/backend/web/static/resources/icons/caffe.png`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/resources/icons/caffe2.svg` & `backend.ai-webserver-23.3.6/ai/backend/web/static/resources/icons/caffe2.svg`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/resources/icons/ceph.png` & `backend.ai-webserver-23.3.6/ai/backend/web/static/resources/icons/ceph.png`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/resources/icons/check-list.svg` & `backend.ai-webserver-23.3.6/ai/backend/web/static/resources/icons/check-list.svg`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/resources/icons/classification.svg` & `backend.ai-webserver-23.3.6/ai/backend/web/static/resources/icons/classification.svg`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/resources/icons/cpp.svg` & `backend.ai-webserver-23.3.6/ai/backend/web/static/resources/icons/cpp.svg`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/resources/icons/default.png` & `backend.ai-webserver-23.3.6/ai/backend/web/static/resources/icons/default.png`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/resources/icons/default_app.svg` & `backend.ai-webserver-23.3.6/ai/backend/web/static/resources/icons/default_app.svg`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/resources/icons/file_type_cuda.svg` & `backend.ai-webserver-23.3.6/ai/backend/web/static/resources/icons/file_type_cuda.svg`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/resources/icons/file_type_python.svg` & `backend.ai-webserver-23.3.6/ai/backend/web/static/resources/icons/file_type_python.svg`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/resources/icons/filebrowser.svg` & `backend.ai-webserver-23.3.6/ai/backend/web/static/resources/icons/filebrowser.svg`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/resources/icons/flux.png` & `backend.ai-webserver-23.3.6/ai/backend/web/static/resources/icons/flux.png`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/resources/icons/gcc.png` & `backend.ai-webserver-23.3.6/ai/backend/web/static/resources/icons/gcc.png`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/resources/icons/gcp.png` & `backend.ai-webserver-23.3.6/ai/backend/web/static/resources/icons/gcp.png`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/resources/icons/gdrive.png` & `backend.ai-webserver-23.3.6/ai/backend/web/static/resources/icons/gdrive.png`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/resources/icons/h2o.png` & `backend.ai-webserver-23.3.6/ai/backend/web/static/resources/icons/h2o.png`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/resources/icons/haskell.png` & `backend.ai-webserver-23.3.6/ai/backend/web/static/resources/icons/haskell.png`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/resources/icons/javascript.png` & `backend.ai-webserver-23.3.6/ai/backend/web/static/resources/icons/javascript.png`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/resources/icons/julia.png` & `backend.ai-webserver-23.3.6/ai/backend/web/static/resources/icons/julia.png`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/resources/icons/jupyter.png` & `backend.ai-webserver-23.3.6/ai/backend/web/static/resources/icons/jupyter.png`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/resources/icons/jupyterlab.png` & `backend.ai-webserver-23.3.6/ai/backend/web/static/resources/icons/jupyterlab.png`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/resources/icons/kitty.png` & `backend.ai-webserver-23.3.6/ai/backend/web/static/resources/icons/kitty.png`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/resources/icons/lablup.png` & `backend.ai-webserver-23.3.6/ai/backend/web/static/resources/icons/lablup.png`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/resources/icons/local.png` & `backend.ai-webserver-23.3.6/ai/backend/web/static/resources/icons/local.png`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/resources/icons/lua.png` & `backend.ai-webserver-23.3.6/ai/backend/web/static/resources/icons/lua.png`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/resources/icons/matlab.png` & `backend.ai-webserver-23.3.6/ai/backend/web/static/resources/icons/matlab.png`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/resources/icons/mlflow.png` & `backend.ai-webserver-23.3.6/ai/backend/web/static/resources/icons/mlflow.png`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/resources/icons/mxnet.svg` & `backend.ai-webserver-23.3.6/ai/backend/web/static/resources/icons/mxnet.svg`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/resources/icons/nbp.png` & `backend.ai-webserver-23.3.6/ai/backend/web/static/resources/icons/nbp.png`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/resources/icons/nni.png` & `backend.ai-webserver-23.3.6/ai/backend/web/static/resources/icons/nni.png`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/resources/icons/nni.svg` & `backend.ai-webserver-23.3.6/ai/backend/web/static/resources/icons/nni.svg`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/resources/icons/nodejs.png` & `backend.ai-webserver-23.3.6/ai/backend/web/static/resources/icons/nodejs.png`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/resources/icons/novnc.svg` & `backend.ai-webserver-23.3.6/ai/backend/web/static/resources/icons/novnc.svg`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/resources/icons/nvidia.png` & `backend.ai-webserver-23.3.6/ai/backend/web/static/resources/icons/nvidia.png`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/resources/icons/octave.png` & `backend.ai-webserver-23.3.6/ai/backend/web/static/resources/icons/octave.png`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/resources/icons/openstack.png` & `backend.ai-webserver-23.3.6/ai/backend/web/static/resources/icons/openstack.png`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/resources/icons/orbit.svg` & `backend.ai-webserver-23.3.6/ai/backend/web/static/resources/icons/orbit.svg`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/resources/icons/php.png` & `backend.ai-webserver-23.3.6/ai/backend/web/static/resources/icons/php.png`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/resources/icons/purestorage.png` & `backend.ai-webserver-23.3.6/ai/backend/web/static/resources/icons/purestorage.png`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/resources/icons/python.png` & `backend.ai-webserver-23.3.6/ai/backend/web/static/resources/icons/python.png`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/resources/icons/pytorch.svg` & `backend.ai-webserver-23.3.6/ai/backend/web/static/resources/icons/pytorch.svg`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/resources/icons/r-lang.svg` & `backend.ai-webserver-23.3.6/ai/backend/web/static/resources/icons/r-lang.svg`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/resources/icons/rebel.svg` & `backend.ai-webserver-23.3.6/ai/backend/web/static/resources/icons/rebel.svg`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/resources/icons/rust.svg` & `backend.ai-webserver-23.3.6/ai/backend/web/static/resources/icons/rust.svg`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/resources/icons/sftp.png` & `backend.ai-webserver-23.3.6/ai/backend/web/static/resources/icons/sftp.png`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/resources/icons/sftp2.png` & `backend.ai-webserver-23.3.6/ai/backend/web/static/resources/icons/sftp2.png`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/resources/icons/swift-tensorflow.png` & `backend.ai-webserver-23.3.6/ai/backend/web/static/resources/icons/swift-tensorflow.png`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/resources/icons/swift.svg` & `backend.ai-webserver-23.3.6/ai/backend/web/static/resources/icons/swift.svg`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/resources/icons/tensorflow.png` & `backend.ai-webserver-23.3.6/ai/backend/web/static/resources/icons/tensorflow.png`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/resources/icons/terminal.svg` & `backend.ai-webserver-23.3.6/ai/backend/web/static/resources/icons/terminal.svg`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/resources/icons/texlive.png` & `backend.ai-webserver-23.3.6/ai/backend/web/static/resources/icons/texlive.png`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/resources/icons/tpu.svg` & `backend.ai-webserver-23.3.6/ai/backend/web/static/resources/icons/tpu.svg`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/resources/icons/ubuntu.svg` & `backend.ai-webserver-23.3.6/ai/backend/web/static/resources/icons/ubuntu.svg`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/resources/icons/vscode.svg` & `backend.ai-webserver-23.3.6/ai/backend/web/static/resources/icons/vscode.svg`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/resources/icons/xfce.png` & `backend.ai-webserver-23.3.6/ai/backend/web/static/resources/icons/xfce.png`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/resources/icons/xrdp.svg` & `backend.ai-webserver-23.3.6/ai/backend/web/static/resources/icons/xrdp.svg`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/resources/image_metadata.json` & `backend.ai-webserver-23.3.6/ai/backend/web/static/resources/image_metadata.json`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/resources/images/401_unauthorized_access.svg` & `backend.ai-webserver-23.3.6/ai/backend/web/static/resources/images/401_unauthorized_access.svg`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/resources/images/404_not_found.svg` & `backend.ai-webserver-23.3.6/ai/backend/web/static/resources/images/404_not_found.svg`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/resources/images/launcher-background.png` & `backend.ai-webserver-23.3.6/ai/backend/web/static/resources/images/launcher-background.png`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/resources/images/loading-background-large.jpg` & `backend.ai-webserver-23.3.6/ai/backend/web/static/resources/images/loading-background-large.jpg`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/resources/images/loading-background.jpg` & `backend.ai-webserver-23.3.6/ai/backend/web/static/resources/images/loading-background.jpg`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/resources/images/web-terminal-guide-1.png` & `backend.ai-webserver-23.3.6/ai/backend/web/static/resources/images/web-terminal-guide-1.png`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/resources/images/web-terminal-guide-2.png` & `backend.ai-webserver-23.3.6/ai/backend/web/static/resources/images/web-terminal-guide-2.png`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/resources/images/web-terminal-guide-3.png` & `backend.ai-webserver-23.3.6/ai/backend/web/static/resources/images/web-terminal-guide-3.png`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/resources/images/web-terminal-guide-4.png` & `backend.ai-webserver-23.3.6/ai/backend/web/static/resources/images/web-terminal-guide-4.png`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/resources/logo.png` & `backend.ai-webserver-23.3.6/ai/backend/web/static/resources/logo.png`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/resources/menu_icons/icon_create_a_key_pair.svg` & `backend.ai-webserver-23.3.6/ai/backend/web/static/resources/menu_icons/icon_create_a_key_pair.svg`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/resources/menu_icons/icon_keypair_management.svg` & `backend.ai-webserver-23.3.6/ai/backend/web/static/resources/menu_icons/icon_keypair_management.svg`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/resources/menu_icons/icon_upload_files.svg` & `backend.ai-webserver-23.3.6/ai/backend/web/static/resources/menu_icons/icon_upload_files.svg`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/resources/storage_metadata.json` & `backend.ai-webserver-23.3.6/ai/backend/web/static/resources/storage_metadata.json`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/resources/templates/under_construction.html` & `backend.ai-webserver-23.3.6/ai/backend/web/static/resources/templates/under_construction.html`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/resources/webui.css` & `backend.ai-webserver-23.3.6/ai/backend/web/static/resources/webui.css`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/src/lib/bundles/webcomponents-ce.js` & `backend.ai-webserver-23.3.6/ai/backend/web/static/src/lib/bundles/webcomponents-ce.js`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/src/lib/bundles/webcomponents-ce.js.map` & `backend.ai-webserver-23.3.6/ai/backend/web/static/src/lib/bundles/webcomponents-ce.js.map`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/src/lib/bundles/webcomponents-pf_dom.js` & `backend.ai-webserver-23.3.6/ai/backend/web/static/src/lib/bundles/webcomponents-pf_dom.js`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/src/lib/bundles/webcomponents-pf_dom.js.map` & `backend.ai-webserver-23.3.6/ai/backend/web/static/src/lib/bundles/webcomponents-pf_dom.js.map`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/src/lib/bundles/webcomponents-pf_js.js` & `backend.ai-webserver-23.3.6/ai/backend/web/static/src/lib/bundles/webcomponents-pf_js.js`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/src/lib/bundles/webcomponents-pf_js.js.map` & `backend.ai-webserver-23.3.6/ai/backend/web/static/src/lib/bundles/webcomponents-pf_js.js.map`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/src/lib/bundles/webcomponents-sd-ce-pf.js` & `backend.ai-webserver-23.3.6/ai/backend/web/static/src/lib/bundles/webcomponents-sd-ce-pf.js`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/src/lib/bundles/webcomponents-sd-ce-pf.js.map` & `backend.ai-webserver-23.3.6/ai/backend/web/static/src/lib/bundles/webcomponents-sd-ce-pf.js.map`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/src/lib/bundles/webcomponents-sd-ce.js` & `backend.ai-webserver-23.3.6/ai/backend/web/static/src/lib/bundles/webcomponents-sd-ce.js`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/src/lib/bundles/webcomponents-sd-ce.js.map` & `backend.ai-webserver-23.3.6/ai/backend/web/static/src/lib/bundles/webcomponents-sd-ce.js.map`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/src/lib/bundles/webcomponents-sd.js` & `backend.ai-webserver-23.3.6/ai/backend/web/static/src/lib/bundles/webcomponents-sd.js`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/src/lib/bundles/webcomponents-sd.js.map` & `backend.ai-webserver-23.3.6/ai/backend/web/static/src/lib/bundles/webcomponents-sd.js.map`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/src/lib/web-animations-js/web-animations-next-lite.min.js` & `backend.ai-webserver-23.3.6/ai/backend/web/static/src/lib/web-animations-js/web-animations-next-lite.min.js`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/src/lib/webcomponents-loader.js` & `backend.ai-webserver-23.3.6/ai/backend/web/static/src/lib/webcomponents-loader.js`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/static/js/149.924fa2a6.chunk.js` & `backend.ai-webserver-23.3.6/ai/backend/web/static/static/js/149.924fa2a6.chunk.js`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/static/js/149.924fa2a6.chunk.js.map` & `backend.ai-webserver-23.3.6/ai/backend/web/static/static/js/149.924fa2a6.chunk.js.map`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/static/js/478.8c8fd27b.chunk.js` & `backend.ai-webserver-23.3.6/ai/backend/web/static/static/js/478.8c8fd27b.chunk.js`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/static/js/478.8c8fd27b.chunk.js.map` & `backend.ai-webserver-23.3.6/ai/backend/web/static/static/js/478.8c8fd27b.chunk.js.map`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/static/js/488.70f8dcf6.chunk.js` & `backend.ai-webserver-23.3.6/ai/backend/web/static/static/js/488.70f8dcf6.chunk.js`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/static/js/488.70f8dcf6.chunk.js.map` & `backend.ai-webserver-23.3.6/ai/backend/web/static/static/js/488.70f8dcf6.chunk.js.map`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/static/js/540.c51503fa.chunk.js` & `backend.ai-webserver-23.3.6/ai/backend/web/static/static/js/540.c51503fa.chunk.js`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/static/js/540.c51503fa.chunk.js.map` & `backend.ai-webserver-23.3.6/ai/backend/web/static/static/js/540.c51503fa.chunk.js.map`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/static/js/558.9310b842.chunk.js` & `backend.ai-webserver-23.3.6/ai/backend/web/static/static/js/558.9310b842.chunk.js`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/static/js/558.9310b842.chunk.js.map` & `backend.ai-webserver-23.3.6/ai/backend/web/static/static/js/558.9310b842.chunk.js.map`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/static/js/618.fdb02897.chunk.js` & `backend.ai-webserver-23.3.6/ai/backend/web/static/static/js/618.fdb02897.chunk.js`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/static/js/618.fdb02897.chunk.js.map` & `backend.ai-webserver-23.3.6/ai/backend/web/static/static/js/618.fdb02897.chunk.js.map`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/static/js/627.a131ed07.chunk.js` & `backend.ai-webserver-23.3.6/ai/backend/web/static/static/js/627.a131ed07.chunk.js`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/static/js/627.a131ed07.chunk.js.map` & `backend.ai-webserver-23.3.6/ai/backend/web/static/static/js/627.a131ed07.chunk.js.map`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/static/js/818.9b28dc99.chunk.js` & `backend.ai-webserver-23.3.6/ai/backend/web/static/static/js/818.9b28dc99.chunk.js`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/static/js/818.9b28dc99.chunk.js.map` & `backend.ai-webserver-23.3.6/ai/backend/web/static/static/js/818.9b28dc99.chunk.js.map`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/static/js/main.8f973991.js` & `backend.ai-webserver-23.3.6/ai/backend/web/static/static/js/main.8f973991.js`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/static/js/main.8f973991.js.LICENSE.txt` & `backend.ai-webserver-23.3.6/ai/backend/web/static/static/js/main.8f973991.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/static/js/main.8f973991.js.map` & `backend.ai-webserver-23.3.6/ai/backend/web/static/static/js/main.8f973991.js.map`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/sw.js` & `backend.ai-webserver-23.3.6/ai/backend/web/static/sw.js`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/sw.js.map` & `backend.ai-webserver-23.3.6/ai/backend/web/static/sw.js.map`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/workbox-d249b2c8.js` & `backend.ai-webserver-23.3.6/ai/backend/web/static/workbox-d249b2c8.js`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/static/workbox-d249b2c8.js.map` & `backend.ai-webserver-23.3.6/ai/backend/web/static/workbox-d249b2c8.js.map`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/stats.py` & `backend.ai-webserver-23.3.6/ai/backend/web/stats.py`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/template.py` & `backend.ai-webserver-23.3.6/ai/backend/web/template.py`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/ai/backend/web/templates/config.toml.j2` & `backend.ai-webserver-23.3.6/ai/backend/web/templates/config.toml.j2`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/backend.ai_webserver.egg-info/PKG-INFO` & `backend.ai-webserver-23.3.6/backend.ai_webserver.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: backend.ai-webserver
-Version: 23.3.5
+Version: 23.3.6
 Summary: Backend.AI WebUI Host
 Home-page: https://github.com/lablup/backend.ai
 Author: Lablup Inc. and contributors
 License: LGPLv3
 Project-URL: Documentation, https://docs.backend.ai/
 Project-URL: Source, https://github.com/lablup/backend.ai
 Classifier: Intended Audience :: Developers
```

### Comparing `backend.ai-webserver-23.3.5/backend.ai_webserver.egg-info/SOURCES.txt` & `backend.ai-webserver-23.3.6/backend.ai_webserver.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/backend_shim.py` & `backend.ai-webserver-23.3.6/backend_shim.py`

 * *Files identical despite different names*

### Comparing `backend.ai-webserver-23.3.5/setup.py` & `backend.ai-webserver-23.3.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,21 +21,21 @@
     ],
     'description': 'Backend.AI WebUI Host',
     'install_requires': (
         'Jinja2~=3.1.2',
         'aiohttp_cors~=0.7',
         'aiohttp~=3.8.1',
         'aiotools~=1.6.1',
-        """backend.ai-cli==23.03.5
+        """backend.ai-cli==23.03.6
 """,
-        """backend.ai-client==23.03.5
+        """backend.ai-client==23.03.6
 """,
-        """backend.ai-common==23.03.5
+        """backend.ai-common==23.03.6
 """,
-        """backend.ai-plugin==23.03.5
+        """backend.ai-plugin==23.03.6
 """,
         'click>=7.1.2',
         'coloredlogs~=15.0',
         'pycryptodome>=3.14.1',
         'redis[hiredis]~=4.5.5',
         'setproctitle~=1.3.2',
         'tomli~=2.0.1',
@@ -423,11 +423,11 @@
     ),
     'project_urls': {
         'Documentation': 'https://docs.backend.ai/',
         'Source': 'https://github.com/lablup/backend.ai',
     },
     'python_requires': '>=3.11,<3.12',
     'url': 'https://github.com/lablup/backend.ai',
-    'version': """23.03.5
+    'version': """23.03.6
 """,
     'zip_safe': False,
 })
```

