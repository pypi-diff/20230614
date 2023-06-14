# Comparing `tmp/non_admin_draftail-0.4.1.tar.gz` & `tmp/non_admin_draftail-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "non_admin_draftail-0.4.1.tar", last modified: Mon Aug 17 13:07:56 2020, max compression
+gzip compressed data, was "non_admin_draftail-0.9.0.tar", last modified: Mon Sep 14 12:58:27 2020, max compression
```

## Comparing `non_admin_draftail-0.4.1.tar` & `non_admin_draftail-0.9.0.tar`

### file list

```diff
@@ -1,79 +1,43 @@
--rw-r--r--   0        0        0     1548 2020-08-17 12:35:59.679891 non_admin_draftail-0.4.1/LICENSE
--rwxr-xr-x   0        0        0       69 2020-08-17 12:39:50.033939 non_admin_draftail-0.4.1/non_admin_draftail/__init__.py
--rwxr-xr-x   0        0        0      109 2020-08-17 12:39:54.367978 non_admin_draftail-0.4.1/non_admin_draftail/apps.py
--rwxr-xr-x   0        0        0    15323 2020-08-17 12:39:54.370329 non_admin_draftail-0.4.1/non_admin_draftail/static/non_admin_draftail/draftail/draftail.css
--rw-r--r--   0        0        0    27945 2020-08-17 12:39:54.370501 non_admin_draftail-0.4.1/non_admin_draftail/static/non_admin_draftail/draftail/draftail.css.map
--rwxr-xr-x   0        0        0   490207 2020-08-17 12:39:54.370135 non_admin_draftail-0.4.1/non_admin_draftail/static/non_admin_draftail/draftail/draftail.js
--rw-r--r--   0        0        0  3295187 2020-08-17 12:39:54.369734 non_admin_draftail-0.4.1/non_admin_draftail/static/non_admin_draftail/draftail/draftail.js.map
--rwxr-xr-x   0        0        0      124 2020-08-17 12:39:54.371040 non_admin_draftail-0.4.1/non_admin_draftail/static/non_admin_draftail/fonts/wagtail-font.css
--rwxr-xr-x   0        0        0    24140 2020-08-17 12:39:54.370870 non_admin_draftail-0.4.1/non_admin_draftail/static/non_admin_draftail/fonts/wagtail.woff
--rwxr-xr-x   0        0        0       41 2020-08-17 12:39:50.034367 non_admin_draftail-0.4.1/non_admin_draftail/static_src/.babelrc
--rwxr-xr-x   0        0        0       24 2020-08-17 12:39:54.194085 non_admin_draftail-0.4.1/non_admin_draftail/static_src/.gitignore
--rwxr-xr-x   0        0        0      808 2020-08-17 12:39:54.193931 non_admin_draftail-0.4.1/non_admin_draftail/static_src/README.md
--rwxr-xr-x   0        0        0   345224 2020-08-17 12:39:54.194339 non_admin_draftail-0.4.1/non_admin_draftail/static_src/package-lock.json
--rwxr-xr-x   0        0        0      771 2020-08-17 12:39:54.194520 non_admin_draftail-0.4.1/non_admin_draftail/static_src/package.json
--rwxr-xr-x   0        0        0     1498 2020-08-17 12:39:54.356552 non_admin_draftail-0.4.1/non_admin_draftail/static_src/src/components/Draftail/DraftUtils.js
--rwxr-xr-x   0        0        0     2872 2020-08-17 12:39:54.359744 non_admin_draftail-0.4.1/non_admin_draftail/static_src/src/components/Draftail/DraftUtils.test.js
--rwxr-xr-x   0        0        0     2418 2020-08-17 12:39:54.359936 non_admin_draftail-0.4.1/non_admin_draftail/static_src/src/components/Draftail/Draftail.scss
--rwxr-xr-x   0        0        0     3847 2020-08-17 12:39:54.361364 non_admin_draftail-0.4.1/non_admin_draftail/static_src/src/components/Draftail/EditorFallback/EditorFallback.js
--rwxr-xr-x   0        0        0      464 2020-08-17 12:39:54.361559 non_admin_draftail-0.4.1/non_admin_draftail/static_src/src/components/Draftail/EditorFallback/EditorFallback.scss
--rwxr-xr-x   0        0        0     3177 2020-08-17 12:39:54.361768 non_admin_draftail-0.4.1/non_admin_draftail/static_src/src/components/Draftail/EditorFallback/EditorFallback.test.js
--rwxr-xr-x   0        0        0     2821 2020-08-17 12:39:54.362146 non_admin_draftail-0.4.1/non_admin_draftail/static_src/src/components/Draftail/EditorFallback/__snapshots__/EditorFallback.test.js.snap
--rwxr-xr-x   0        0        0     1223 2020-08-17 12:39:54.355746 non_admin_draftail-0.4.1/non_admin_draftail/static_src/src/components/Draftail/Tooltip/Tooltip.js
--rwxr-xr-x   0        0        0     1977 2020-08-17 12:39:54.355930 non_admin_draftail-0.4.1/non_admin_draftail/static_src/src/components/Draftail/Tooltip/Tooltip.scss
--rwxr-xr-x   0        0        0      756 2020-08-17 12:39:54.355557 non_admin_draftail-0.4.1/non_admin_draftail/static_src/src/components/Draftail/Tooltip/Tooltip.test.js
--rwxr-xr-x   0        0        0      613 2020-08-17 12:39:54.356345 non_admin_draftail-0.4.1/non_admin_draftail/static_src/src/components/Draftail/Tooltip/__snapshots__/Tooltip.test.js.snap
--rwxr-xr-x   0        0        0     1274 2020-08-17 12:39:54.362524 non_admin_draftail-0.4.1/non_admin_draftail/static_src/src/components/Draftail/__snapshots__/index.test.js.snap
--rwxr-xr-x   0        0        0      971 2020-08-17 12:39:54.354315 non_admin_draftail-0.4.1/non_admin_draftail/static_src/src/components/Draftail/blocks/EmbedBlock.js
--rwxr-xr-x   0        0        0       78 2020-08-17 12:39:54.353057 non_admin_draftail-0.4.1/non_admin_draftail/static_src/src/components/Draftail/blocks/EmbedBlock.scss
--rwxr-xr-x   0        0        0      827 2020-08-17 12:39:54.352600 non_admin_draftail-0.4.1/non_admin_draftail/static_src/src/components/Draftail/blocks/EmbedBlock.test.js
--rwxr-xr-x   0        0        0     1418 2020-08-17 12:39:54.352800 non_admin_draftail-0.4.1/non_admin_draftail/static_src/src/components/Draftail/blocks/ImageBlock.js
--rwxr-xr-x   0        0        0      641 2020-08-17 12:39:54.352390 non_admin_draftail-0.4.1/non_admin_draftail/static_src/src/components/Draftail/blocks/ImageBlock.scss
--rwxr-xr-x   0        0        0     2349 2020-08-17 12:39:54.353509 non_admin_draftail-0.4.1/non_admin_draftail/static_src/src/components/Draftail/blocks/ImageBlock.test.js
--rwxr-xr-x   0        0        0     3037 2020-08-17 12:39:54.353784 non_admin_draftail-0.4.1/non_admin_draftail/static_src/src/components/Draftail/blocks/MediaBlock.js
--rwxr-xr-x   0        0        0      875 2020-08-17 12:39:54.354032 non_admin_draftail-0.4.1/non_admin_draftail/static_src/src/components/Draftail/blocks/MediaBlock.scss
--rwxr-xr-x   0        0        0     2967 2020-08-17 12:39:54.352111 non_admin_draftail-0.4.1/non_admin_draftail/static_src/src/components/Draftail/blocks/MediaBlock.test.js
--rwxr-xr-x   0        0        0      912 2020-08-17 12:39:54.354746 non_admin_draftail-0.4.1/non_admin_draftail/static_src/src/components/Draftail/blocks/__snapshots__/EmbedBlock.test.js.snap
--rwxr-xr-x   0        0        0     1470 2020-08-17 12:39:54.355168 non_admin_draftail-0.4.1/non_admin_draftail/static_src/src/components/Draftail/blocks/__snapshots__/ImageBlock.test.js.snap
--rwxr-xr-x   0        0        0     1212 2020-08-17 12:39:54.354954 non_admin_draftail-0.4.1/non_admin_draftail/static_src/src/components/Draftail/blocks/__snapshots__/MediaBlock.test.js.snap
--rwxr-xr-x   0        0        0      923 2020-08-17 12:39:54.358206 non_admin_draftail-0.4.1/non_admin_draftail/static_src/src/components/Draftail/decorators/Document.js
--rwxr-xr-x   0        0        0     1454 2020-08-17 12:39:54.357797 non_admin_draftail-0.4.1/non_admin_draftail/static_src/src/components/Draftail/decorators/Document.test.js
--rwxr-xr-x   0        0        0     1709 2020-08-17 12:39:54.357365 non_admin_draftail-0.4.1/non_admin_draftail/static_src/src/components/Draftail/decorators/Link.js
--rwxr-xr-x   0        0        0     1889 2020-08-17 12:39:54.357612 non_admin_draftail-0.4.1/non_admin_draftail/static_src/src/components/Draftail/decorators/Link.test.js
--rwxr-xr-x   0        0        0     3901 2020-08-17 12:39:54.356947 non_admin_draftail-0.4.1/non_admin_draftail/static_src/src/components/Draftail/decorators/TooltipEntity.js
--rwxr-xr-x   0        0        0      294 2020-08-17 12:39:54.357144 non_admin_draftail-0.4.1/non_admin_draftail/static_src/src/components/Draftail/decorators/TooltipEntity.scss
--rwxr-xr-x   0        0        0     3416 2020-08-17 12:39:54.358028 non_admin_draftail-0.4.1/non_admin_draftail/static_src/src/components/Draftail/decorators/TooltipEntity.test.js
--rwxr-xr-x   0        0        0     3217 2020-08-17 12:39:54.358654 non_admin_draftail-0.4.1/non_admin_draftail/static_src/src/components/Draftail/decorators/__snapshots__/Document.test.js.snap
--rwxr-xr-x   0        0        0     1638 2020-08-17 12:39:54.358940 non_admin_draftail-0.4.1/non_admin_draftail/static_src/src/components/Draftail/decorators/__snapshots__/Link.test.js.snap
--rwxr-xr-x   0        0        0     1759 2020-08-17 12:39:54.359143 non_admin_draftail-0.4.1/non_admin_draftail/static_src/src/components/Draftail/decorators/__snapshots__/TooltipEntity.test.js.snap
--rwxr-xr-x   0        0        0     4250 2020-08-17 12:39:54.359346 non_admin_draftail-0.4.1/non_admin_draftail/static_src/src/components/Draftail/index.js
--rwxr-xr-x   0        0        0     4266 2020-08-17 12:39:54.359543 non_admin_draftail-0.4.1/non_admin_draftail/static_src/src/components/Draftail/index.test.js
--rwxr-xr-x   0        0        0     6993 2020-08-17 12:39:54.360378 non_admin_draftail-0.4.1/non_admin_draftail/static_src/src/components/Draftail/sources/ModalWorkflowSource.js
--rwxr-xr-x   0        0        0     9973 2020-08-17 12:39:54.360572 non_admin_draftail-0.4.1/non_admin_draftail/static_src/src/components/Draftail/sources/ModalWorkflowSource.test.js
--rwxr-xr-x   0        0        0     3129 2020-08-17 12:39:54.360959 non_admin_draftail-0.4.1/non_admin_draftail/static_src/src/components/Draftail/sources/__snapshots__/ModalWorkflowSource.test.js.snap
--rwxr-xr-x   0        0        0      713 2020-08-17 12:39:54.363159 non_admin_draftail-0.4.1/non_admin_draftail/static_src/src/components/Icon/Icon.js
--rwxr-xr-x   0        0        0      493 2020-08-17 12:39:54.362942 non_admin_draftail-0.4.1/non_admin_draftail/static_src/src/components/Icon/Icon.test.js
--rwxr-xr-x   0        0        0      468 2020-08-17 12:39:54.363659 non_admin_draftail-0.4.1/non_admin_draftail/static_src/src/components/Icon/__snapshots__/Icon.test.js.snap
--rwxr-xr-x   0        0        0      725 2020-08-17 12:39:54.364179 non_admin_draftail-0.4.1/non_admin_draftail/static_src/src/components/Modal/Modal.js
--rwxr-xr-x   0        0        0     1498 2020-08-17 12:39:54.364416 non_admin_draftail-0.4.1/non_admin_draftail/static_src/src/components/Modal/Modal.scss
--rwxr-xr-x   0        0        0     1772 2020-08-17 12:39:54.350548 non_admin_draftail-0.4.1/non_admin_draftail/static_src/src/components/Portal/Portal.js
--rwxr-xr-x   0        0        0     2877 2020-08-17 12:39:54.350844 non_admin_draftail-0.4.1/non_admin_draftail/static_src/src/components/Portal/Portal.test.js
--rwxr-xr-x   0        0        0      673 2020-08-17 12:39:54.351358 non_admin_draftail-0.4.1/non_admin_draftail/static_src/src/components/Portal/__snapshots__/Portal.test.js.snap
--rwxr-xr-x   0        0        0      346 2020-08-17 12:39:54.348324 non_admin_draftail-0.4.1/non_admin_draftail/static_src/src/config/wagtailConfig.js
--rwxr-xr-x   0        0        0      593 2020-08-17 12:39:54.348553 non_admin_draftail-0.4.1/non_admin_draftail/static_src/src/config/wagtailConfig.test.js
--rwxr-xr-x   0        0        0      802 2020-08-17 12:39:54.348702 non_admin_draftail-0.4.1/non_admin_draftail/static_src/src/index.js
--rwxr-xr-x   0        0        0     4296 2020-08-17 12:39:54.365145 non_admin_draftail-0.4.1/non_admin_draftail/static_src/src/sources/EmbedSource/index.js
--rwxr-xr-x   0        0        0      605 2020-08-17 12:39:54.365327 non_admin_draftail-0.4.1/non_admin_draftail/static_src/src/sources/EmbedSource/style.scss
--rwxr-xr-x   0        0        0     3683 2020-08-17 12:39:54.365681 non_admin_draftail-0.4.1/non_admin_draftail/static_src/src/sources/LinkSource/index.js
--rwxr-xr-x   0        0        0      602 2020-08-17 12:39:54.365856 non_admin_draftail-0.4.1/non_admin_draftail/static_src/src/sources/LinkSource/style.scss
--rwxr-xr-x   0        0        0     6772 2020-08-17 12:39:54.349519 non_admin_draftail-0.4.1/non_admin_draftail/static_src/src/styles/icons.scss
--rwxr-xr-x   0        0        0       55 2020-08-17 12:39:54.349199 non_admin_draftail-0.4.1/non_admin_draftail/static_src/src/styles/styles.scss
--rwxr-xr-x   0        0        0      413 2020-08-17 12:46:30.692362 non_admin_draftail-0.4.1/non_admin_draftail/templates/non_admin_draftail/tags/non_admin_draftail_strings.html
--rwxr-xr-x   0        0        0      245 2020-08-17 12:39:54.372102 non_admin_draftail-0.4.1/non_admin_draftail/templates/non_admin_draftail/widgets/non_admin_draftail_rich_text_area.html
--rwxr-xr-x   0        0        0      419 2020-08-17 12:39:50.032969 non_admin_draftail-0.4.1/non_admin_draftail/templatetags/non_admin_draftail_tags.py
--rw-r--r--   0        0        0      204 2020-08-17 12:39:54.372287 non_admin_draftail-0.4.1/non_admin_draftail/urls.py
--rw-r--r--   0        0        0     1804 2020-08-17 12:39:54.372687 non_admin_draftail-0.4.1/non_admin_draftail/views.py
--rwxr-xr-x   0        0        0     1154 2020-08-17 12:39:54.368171 non_admin_draftail-0.4.1/non_admin_draftail/widgets.py
--rw-r--r--   0        0        0      449 2020-08-17 13:07:47.056520 non_admin_draftail-0.4.1/pyproject.toml
--rw-r--r--   0        0        0     2474 2020-08-17 13:07:56.849005 non_admin_draftail-0.4.1/setup.py
--rw-r--r--   0        0        0      525 2020-08-17 13:07:56.849519 non_admin_draftail-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1548 2020-08-17 12:35:59.679891 non_admin_draftail-0.9.0/LICENSE
+-rwxr-xr-x   0        0        0       70 2020-09-14 12:56:44.069656 non_admin_draftail-0.9.0/non_admin_draftail/__init__.py
+-rwxr-xr-x   0        0        0      109 2020-09-14 12:56:44.070006 non_admin_draftail-0.9.0/non_admin_draftail/apps.py
+-rw-r--r--   0        0        0      165 2020-09-14 12:56:44.070204 non_admin_draftail-0.9.0/non_admin_draftail/conf.py
+-rw-r--r--   0        0        0     2416 2020-09-14 12:56:44.070650 non_admin_draftail-0.9.0/non_admin_draftail/forms.py
+-rw-r--r--   0        0        0     2109 2020-09-14 12:56:44.071043 non_admin_draftail-0.9.0/non_admin_draftail/static/non_admin_draftail/draftail.css
+-rw-r--r--   0        0        0     3418 2020-09-14 12:56:44.071300 non_admin_draftail-0.9.0/non_admin_draftail/static/non_admin_draftail/draftail.css.map
+-rw-r--r--   0        0        0    16759 2020-09-14 12:56:44.071718 non_admin_draftail-0.9.0/non_admin_draftail/static/non_admin_draftail/draftail.js.map
+-rw-r--r--   0        0        0     4364 2020-09-14 12:56:44.072021 non_admin_draftail-0.9.0/non_admin_draftail/static/non_admin_draftail/modal-workflow.js
+-rwxr-xr-x   0        0        0       25 2020-09-14 12:56:44.072338 non_admin_draftail-0.9.0/non_admin_draftail/static_src/.gitignore
+-rwxr-xr-x   0        0        0      808 2020-08-17 13:23:05.730972 non_admin_draftail-0.9.0/non_admin_draftail/static_src/README.md
+-rw-r--r--   0        0        0   319346 2020-09-14 12:56:44.073975 non_admin_draftail-0.9.0/non_admin_draftail/static_src/package-lock.json
+-rwxr-xr-x   0        0        0      507 2020-09-14 12:56:44.074643 non_admin_draftail-0.9.0/non_admin_draftail/static_src/package.json
+-rw-r--r--   0        0        0       62 2020-09-14 12:56:44.075124 non_admin_draftail-0.9.0/non_admin_draftail/static_src/src/index.js
+-rw-r--r--   0        0        0     1326 2020-09-14 12:56:44.076027 non_admin_draftail-0.9.0/non_admin_draftail/static_src/src/styles/chooser.scss
+-rw-r--r--   0        0        0     1242 2020-09-14 12:56:44.076270 non_admin_draftail-0.9.0/non_admin_draftail/static_src/src/styles/modal.scss
+-rw-r--r--   0        0        0      181 2020-09-14 12:56:44.076530 non_admin_draftail-0.9.0/non_admin_draftail/templates/non_admin_draftail/_draftail_css.html
+-rw-r--r--   0        0        0     2251 2020-09-14 12:56:44.076808 non_admin_draftail-0.9.0/non_admin_draftail/templates/non_admin_draftail/_draftail_js.html
+-rw-r--r--   0        0        0      632 2020-09-14 12:56:44.077663 non_admin_draftail-0.9.0/non_admin_draftail/templates/non_admin_draftail/document/chooser.html
+-rw-r--r--   0        0        0     1273 2020-09-14 12:56:44.078295 non_admin_draftail-0.9.0/non_admin_draftail/templates/non_admin_draftail/document/results.html
+-rw-r--r--   0        0        0      107 2020-09-14 12:56:44.078724 non_admin_draftail-0.9.0/non_admin_draftail/templates/non_admin_draftail/draftail_media.html
+-rw-r--r--   0        0        0      442 2020-09-14 12:56:44.079490 non_admin_draftail-0.9.0/non_admin_draftail/templates/non_admin_draftail/embed/chooser.html
+-rw-r--r--   0        0        0      535 2020-09-14 12:56:44.080235 non_admin_draftail-0.9.0/non_admin_draftail/templates/non_admin_draftail/image/select_format.html
+-rw-r--r--   0        0        0      636 2020-09-14 12:56:44.080532 non_admin_draftail-0.9.0/non_admin_draftail/templates/non_admin_draftail/image/upload.html
+-rw-r--r--   0        0        0     1431 2020-09-14 12:56:44.081376 non_admin_draftail-0.9.0/non_admin_draftail/templates/non_admin_draftail/link/_link_types.html
+-rw-r--r--   0        0        0      502 2020-09-14 12:56:44.081804 non_admin_draftail-0.9.0/non_admin_draftail/templates/non_admin_draftail/link/anchor_link.html
+-rw-r--r--   0        0        0      499 2020-09-14 12:56:44.082248 non_admin_draftail-0.9.0/non_admin_draftail/templates/non_admin_draftail/link/email_link.html
+-rw-r--r--   0        0        0      498 2020-09-14 12:56:44.082793 non_admin_draftail-0.9.0/non_admin_draftail/templates/non_admin_draftail/link/external_link.html
+-rw-r--r--   0        0        0      498 2020-09-14 12:56:44.083154 non_admin_draftail-0.9.0/non_admin_draftail/templates/non_admin_draftail/link/phone_link.html
+-rw-r--r--   0        0        0      269 2020-09-14 12:56:44.083644 non_admin_draftail-0.9.0/non_admin_draftail/templates/non_admin_draftail/modal_base.html
+-rwxr-xr-x   0        0        0      202 2020-09-14 12:56:44.084013 non_admin_draftail-0.9.0/non_admin_draftail/templates/non_admin_draftail/widgets/non_admin_draftail_rich_text_area.html
+-rw-r--r--   0        0        0        0 2020-09-14 12:56:44.084098 non_admin_draftail-0.9.0/non_admin_draftail/templatetags/__init__.py
+-rw-r--r--   0        0        0      182 2020-09-14 12:56:44.084831 non_admin_draftail-0.9.0/non_admin_draftail/templatetags/non_admin_draftail_tags.py
+-rw-r--r--   0        0        0     1609 2020-09-14 12:56:44.085310 non_admin_draftail-0.9.0/non_admin_draftail/urls.py
+-rw-r--r--   0        0        0        0 2020-09-14 12:56:44.085440 non_admin_draftail-0.9.0/non_admin_draftail/views/__init__.py
+-rw-r--r--   0        0        0     3403 2020-09-14 12:56:44.086001 non_admin_draftail-0.9.0/non_admin_draftail/views/document.py
+-rw-r--r--   0        0        0     3182 2020-09-14 12:56:44.086395 non_admin_draftail-0.9.0/non_admin_draftail/views/embed.py
+-rw-r--r--   0        0        0     4456 2020-09-14 12:56:44.086673 non_admin_draftail-0.9.0/non_admin_draftail/views/image.py
+-rw-r--r--   0        0        0     6317 2020-09-14 12:56:44.087081 non_admin_draftail-0.9.0/non_admin_draftail/views/link.py
+-rwxr-xr-x   0        0        0      832 2020-09-14 12:56:44.087410 non_admin_draftail-0.9.0/non_admin_draftail/widgets.py
+-rw-r--r--   0        0        0     1115 2020-09-14 12:58:05.520234 non_admin_draftail-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     2463 2020-09-14 12:58:29.068306 non_admin_draftail-0.9.0/setup.py
+-rw-r--r--   0        0        0      597 2020-09-14 12:58:29.068547 non_admin_draftail-0.9.0/PKG-INFO
```

### Comparing `non_admin_draftail-0.4.1/LICENSE` & `non_admin_draftail-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `non_admin_draftail-0.4.1/non_admin_draftail/static_src/README.md` & `non_admin_draftail-0.9.0/non_admin_draftail/static_src/README.md`

 * *Files identical despite different names*

### Comparing `non_admin_draftail-0.4.1/non_admin_draftail/static_src/package-lock.json` & `non_admin_draftail-0.9.0/non_admin_draftail/static_src/package-lock.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9849403471286658%*

 * *Differences: {"'dependencies'": "{'@babel/core': {'version': '7.11.4', 'resolved': "*

 * *                   "'https://registry.npmjs.org/@babel/core/-/core-7.11.4.tgz', 'integrity': "*

 * *                   "'sha512-5deljj5HlqRXN+5oJTY7Zs37iH3z3b++KjiKtIsJy1NrjOOVSEaJHEetLBhyu0aQOSNNZ/0IuEAan9GzRuDXHg==', "*

 * *                   "'requires': {'@babel/code-frame': '^7.10.4', '@babel/generator': '^7.11.4', "*

 * *                   "'@babel/helpers': '^7.10.4', '@babel/parser': '^7.11.4', '@babel/template': "*

 * *                   "'^7.10.4 […]*

```diff
@@ -7,44 +7,212 @@
                 "@babel/highlight": "^7.0.0"
             },
             "resolved": "https://registry.npmjs.org/@babel/code-frame/-/code-frame-7.5.5.tgz",
             "version": "7.5.5"
         },
         "@babel/core": {
             "dependencies": {
-                "debug": {
+                "@babel/code-frame": {
                     "dev": true,
-                    "integrity": "sha512-pYAIzeRo8J6KPEaJ0VWOh5Pzkbw/RetuzehGM7QRRX5he4fPHx2rdKMB256ehJCkX+XRQm16eZLqLNS8RSZXZw==",
+                    "integrity": "sha512-vG6SvB6oYEhvgisZNFRmRCUkLz11c7rp+tbNTynGqc6mS1d5ATd/sGyV6W0KZZnXRKMTzZDRgQT3Ou9jhpAfUg==",
                     "requires": {
-                        "ms": "^2.1.1"
+                        "@babel/highlight": "^7.10.4"
                     },
-                    "resolved": "https://registry.npmjs.org/debug/-/debug-4.1.1.tgz",
-                    "version": "4.1.1"
+                    "resolved": "https://registry.npmjs.org/@babel/code-frame/-/code-frame-7.10.4.tgz",
+                    "version": "7.10.4"
+                },
+                "@babel/generator": {
+                    "dev": true,
+                    "integrity": "sha512-Rn26vueFx0eOoz7iifCN2UHT6rGtnkSGWSoDRIy8jZN3B91PzeSULbswfLoOWuTuAcNwpG/mxy+uCTDnZ9Mp1g==",
+                    "requires": {
+                        "@babel/types": "^7.11.0",
+                        "jsesc": "^2.5.1",
+                        "source-map": "^0.5.0"
+                    },
+                    "resolved": "https://registry.npmjs.org/@babel/generator/-/generator-7.11.4.tgz",
+                    "version": "7.11.4"
+                },
+                "@babel/helper-function-name": {
+                    "dev": true,
+                    "integrity": "sha512-YdaSyz1n8gY44EmN7x44zBn9zQ1Ry2Y+3GTA+3vH6Mizke1Vw0aWDM66FOYEPw8//qKkmqOckrGgTYa+6sceqQ==",
+                    "requires": {
+                        "@babel/helper-get-function-arity": "^7.10.4",
+                        "@babel/template": "^7.10.4",
+                        "@babel/types": "^7.10.4"
+                    },
+                    "resolved": "https://registry.npmjs.org/@babel/helper-function-name/-/helper-function-name-7.10.4.tgz",
+                    "version": "7.10.4"
+                },
+                "@babel/helper-get-function-arity": {
+                    "dev": true,
+                    "integrity": "sha512-EkN3YDB+SRDgiIUnNgcmiD361ti+AVbL3f3Henf6dqqUyr5dMsorno0lJWJuLhDhkI5sYEpgj6y9kB8AOU1I2A==",
+                    "requires": {
+                        "@babel/types": "^7.10.4"
+                    },
+                    "resolved": "https://registry.npmjs.org/@babel/helper-get-function-arity/-/helper-get-function-arity-7.10.4.tgz",
+                    "version": "7.10.4"
+                },
+                "@babel/helper-member-expression-to-functions": {
+                    "dev": true,
+                    "integrity": "sha512-JbFlKHFntRV5qKw3YC0CvQnDZ4XMwgzzBbld7Ly4Mj4cbFy3KywcR8NtNctRToMWJOVvLINJv525Gd6wwVEx/Q==",
+                    "requires": {
+                        "@babel/types": "^7.11.0"
+                    },
+                    "resolved": "https://registry.npmjs.org/@babel/helper-member-expression-to-functions/-/helper-member-expression-to-functions-7.11.0.tgz",
+                    "version": "7.11.0"
+                },
+                "@babel/helper-module-imports": {
+                    "dev": true,
+                    "integrity": "sha512-nEQJHqYavI217oD9+s5MUBzk6x1IlvoS9WTPfgG43CbMEeStE0v+r+TucWdx8KFGowPGvyOkDT9+7DHedIDnVw==",
+                    "requires": {
+                        "@babel/types": "^7.10.4"
+                    },
+                    "resolved": "https://registry.npmjs.org/@babel/helper-module-imports/-/helper-module-imports-7.10.4.tgz",
+                    "version": "7.10.4"
+                },
+                "@babel/helper-module-transforms": {
+                    "dev": true,
+                    "integrity": "sha512-02EVu8COMuTRO1TAzdMtpBPbe6aQ1w/8fePD2YgQmxZU4gpNWaL9gK3Jp7dxlkUlUCJOTaSeA+Hrm1BRQwqIhg==",
+                    "requires": {
+                        "@babel/helper-module-imports": "^7.10.4",
+                        "@babel/helper-replace-supers": "^7.10.4",
+                        "@babel/helper-simple-access": "^7.10.4",
+                        "@babel/helper-split-export-declaration": "^7.11.0",
+                        "@babel/template": "^7.10.4",
+                        "@babel/types": "^7.11.0",
+                        "lodash": "^4.17.19"
+                    },
+                    "resolved": "https://registry.npmjs.org/@babel/helper-module-transforms/-/helper-module-transforms-7.11.0.tgz",
+                    "version": "7.11.0"
+                },
+                "@babel/helper-optimise-call-expression": {
+                    "dev": true,
+                    "integrity": "sha512-n3UGKY4VXwXThEiKrgRAoVPBMqeoPgHVqiHZOanAJCG9nQUL2pLRQirUzl0ioKclHGpGqRgIOkgcIJaIWLpygg==",
+                    "requires": {
+                        "@babel/types": "^7.10.4"
+                    },
+                    "resolved": "https://registry.npmjs.org/@babel/helper-optimise-call-expression/-/helper-optimise-call-expression-7.10.4.tgz",
+                    "version": "7.10.4"
+                },
+                "@babel/helper-replace-supers": {
+                    "dev": true,
+                    "integrity": "sha512-sPxZfFXocEymYTdVK1UNmFPBN+Hv5mJkLPsYWwGBxZAxaWfFu+xqp7b6qWD0yjNuNL2VKc6L5M18tOXUP7NU0A==",
+                    "requires": {
+                        "@babel/helper-member-expression-to-functions": "^7.10.4",
+                        "@babel/helper-optimise-call-expression": "^7.10.4",
+                        "@babel/traverse": "^7.10.4",
+                        "@babel/types": "^7.10.4"
+                    },
+                    "resolved": "https://registry.npmjs.org/@babel/helper-replace-supers/-/helper-replace-supers-7.10.4.tgz",
+                    "version": "7.10.4"
+                },
+                "@babel/helper-simple-access": {
+                    "dev": true,
+                    "integrity": "sha512-0fMy72ej/VEvF8ULmX6yb5MtHG4uH4Dbd6I/aHDb/JVg0bbivwt9Wg+h3uMvX+QSFtwr5MeItvazbrc4jtRAXw==",
+                    "requires": {
+                        "@babel/template": "^7.10.4",
+                        "@babel/types": "^7.10.4"
+                    },
+                    "resolved": "https://registry.npmjs.org/@babel/helper-simple-access/-/helper-simple-access-7.10.4.tgz",
+                    "version": "7.10.4"
+                },
+                "@babel/helper-split-export-declaration": {
+                    "dev": true,
+                    "integrity": "sha512-74Vejvp6mHkGE+m+k5vHY93FX2cAtrw1zXrZXRlG4l410Nm9PxfEiVTn1PjDPV5SnmieiueY4AFg2xqhNFuuZg==",
+                    "requires": {
+                        "@babel/types": "^7.11.0"
+                    },
+                    "resolved": "https://registry.npmjs.org/@babel/helper-split-export-declaration/-/helper-split-export-declaration-7.11.0.tgz",
+                    "version": "7.11.0"
+                },
+                "@babel/highlight": {
+                    "dev": true,
+                    "integrity": "sha512-i6rgnR/YgPEQzZZnbTHHuZdlE8qyoBNalD6F+q4vAFlcMEcqmkoG+mPqJYJCo63qPf74+Y1UZsl3l6f7/RIkmA==",
+                    "requires": {
+                        "@babel/helper-validator-identifier": "^7.10.4",
+                        "chalk": "^2.0.0",
+                        "js-tokens": "^4.0.0"
+                    },
+                    "resolved": "https://registry.npmjs.org/@babel/highlight/-/highlight-7.10.4.tgz",
+                    "version": "7.10.4"
+                },
+                "@babel/parser": {
+                    "dev": true,
+                    "integrity": "sha512-MggwidiH+E9j5Sh8pbrX5sJvMcsqS5o+7iB42M9/k0CD63MjYbdP4nhSh7uB5wnv2/RVzTZFTxzF/kIa5mrCqA==",
+                    "resolved": "https://registry.npmjs.org/@babel/parser/-/parser-7.11.4.tgz",
+                    "version": "7.11.4"
+                },
+                "@babel/template": {
+                    "dev": true,
+                    "integrity": "sha512-ZCjD27cGJFUB6nmCB1Enki3r+L5kJveX9pq1SvAUKoICy6CZ9yD8xO086YXdYhvNjBdnekm4ZnaP5yC8Cs/1tA==",
+                    "requires": {
+                        "@babel/code-frame": "^7.10.4",
+                        "@babel/parser": "^7.10.4",
+                        "@babel/types": "^7.10.4"
+                    },
+                    "resolved": "https://registry.npmjs.org/@babel/template/-/template-7.10.4.tgz",
+                    "version": "7.10.4"
+                },
+                "@babel/traverse": {
+                    "dev": true,
+                    "integrity": "sha512-ZB2V+LskoWKNpMq6E5UUCrjtDUh5IOTAyIl0dTjIEoXum/iKWkoIEKIRDnUucO6f+2FzNkE0oD4RLKoPIufDtg==",
+                    "requires": {
+                        "@babel/code-frame": "^7.10.4",
+                        "@babel/generator": "^7.11.0",
+                        "@babel/helper-function-name": "^7.10.4",
+                        "@babel/helper-split-export-declaration": "^7.11.0",
+                        "@babel/parser": "^7.11.0",
+                        "@babel/types": "^7.11.0",
+                        "debug": "^4.1.0",
+                        "globals": "^11.1.0",
+                        "lodash": "^4.17.19"
+                    },
+                    "resolved": "https://registry.npmjs.org/@babel/traverse/-/traverse-7.11.0.tgz",
+                    "version": "7.11.0"
+                },
+                "@babel/types": {
+                    "dev": true,
+                    "integrity": "sha512-O53yME4ZZI0jO1EVGtF1ePGl0LHirG4P1ibcD80XyzZcKhcMFeCXmh4Xb1ifGBIV233Qg12x4rBfQgA+tmOukA==",
+                    "requires": {
+                        "@babel/helper-validator-identifier": "^7.10.4",
+                        "lodash": "^4.17.19",
+                        "to-fast-properties": "^2.0.0"
+                    },
+                    "resolved": "https://registry.npmjs.org/@babel/types/-/types-7.11.0.tgz",
+                    "version": "7.11.0"
+                },
+                "lodash": {
+                    "dev": true,
+                    "integrity": "sha512-PlhdFcillOINfeV7Ni6oF1TAEayyZBoZ8bcshTHqOYJYlrqzRK5hagpagky5o4HfCzzd1TRkXPMFq6cKk9rGmA==",
+                    "resolved": "https://registry.npmjs.org/lodash/-/lodash-4.17.20.tgz",
+                    "version": "4.17.20"
                 }
             },
             "dev": true,
-            "integrity": "sha512-M42+ScN4+1S9iB6f+TL7QBpoQETxbclx+KNoKJABghnKYE+fMzSGqst0BZJc8CpI625bwPwYgUyRvxZ+0mZzpw==",
+            "integrity": "sha512-5deljj5HlqRXN+5oJTY7Zs37iH3z3b++KjiKtIsJy1NrjOOVSEaJHEetLBhyu0aQOSNNZ/0IuEAan9GzRuDXHg==",
             "requires": {
-                "@babel/code-frame": "^7.5.5",
-                "@babel/generator": "^7.7.4",
-                "@babel/helpers": "^7.7.4",
-                "@babel/parser": "^7.7.5",
-                "@babel/template": "^7.7.4",
-                "@babel/traverse": "^7.7.4",
-                "@babel/types": "^7.7.4",
+                "@babel/code-frame": "^7.10.4",
+                "@babel/generator": "^7.11.4",
+                "@babel/helper-module-transforms": "^7.11.0",
+                "@babel/helpers": "^7.10.4",
+                "@babel/parser": "^7.11.4",
+                "@babel/template": "^7.10.4",
+                "@babel/traverse": "^7.11.0",
+                "@babel/types": "^7.11.0",
                 "convert-source-map": "^1.7.0",
                 "debug": "^4.1.0",
-                "json5": "^2.1.0",
-                "lodash": "^4.17.13",
+                "gensync": "^1.0.0-beta.1",
+                "json5": "^2.1.2",
+                "lodash": "^4.17.19",
                 "resolve": "^1.3.2",
                 "semver": "^5.4.1",
                 "source-map": "^0.5.0"
             },
-            "resolved": "https://registry.npmjs.org/@babel/core/-/core-7.7.5.tgz",
-            "version": "7.7.5"
+            "resolved": "https://registry.npmjs.org/@babel/core/-/core-7.11.4.tgz",
+            "version": "7.11.4"
         },
         "@babel/generator": {
             "dev": true,
             "integrity": "sha512-m5qo2WgdOJeyYngKImbkyQrnUN1mPceaG5BV+G0E3gWsa4l/jCSryWJdM2x8OuGAOyh+3d5pVYfZWCiNFtynxg==",
             "requires": {
                 "@babel/types": "^7.7.4",
                 "jsesc": "^2.5.1",
@@ -250,36 +418,155 @@
             "integrity": "sha512-guAg1SXFcVr04Guk9eq0S4/rWS++sbmyqosJzVs8+1fH5NI+ZcmkaSkc7dmtAFbHFva6yRJnjW3yAcGxjueDug==",
             "requires": {
                 "@babel/types": "^7.7.4"
             },
             "resolved": "https://registry.npmjs.org/@babel/helper-split-export-declaration/-/helper-split-export-declaration-7.7.4.tgz",
             "version": "7.7.4"
         },
+        "@babel/helper-validator-identifier": {
+            "dev": true,
+            "integrity": "sha512-3U9y+43hz7ZM+rzG24Qe2mufW5KhvFg/NhnNph+i9mgCtdTCtMJuI1TMkrIUiK7Ix4PYlRF9I5dhqaLYA/ADXw==",
+            "resolved": "https://registry.npmjs.org/@babel/helper-validator-identifier/-/helper-validator-identifier-7.10.4.tgz",
+            "version": "7.10.4"
+        },
         "@babel/helper-wrap-function": {
             "dev": true,
             "integrity": "sha512-VsfzZt6wmsocOaVU0OokwrIytHND55yvyT4BPB9AIIgwr8+x7617hetdJTsuGwygN5RC6mxA9EJztTjuwm2ofg==",
             "requires": {
                 "@babel/helper-function-name": "^7.7.4",
                 "@babel/template": "^7.7.4",
                 "@babel/traverse": "^7.7.4",
                 "@babel/types": "^7.7.4"
             },
             "resolved": "https://registry.npmjs.org/@babel/helper-wrap-function/-/helper-wrap-function-7.7.4.tgz",
             "version": "7.7.4"
         },
         "@babel/helpers": {
+            "dependencies": {
+                "@babel/code-frame": {
+                    "dev": true,
+                    "integrity": "sha512-vG6SvB6oYEhvgisZNFRmRCUkLz11c7rp+tbNTynGqc6mS1d5ATd/sGyV6W0KZZnXRKMTzZDRgQT3Ou9jhpAfUg==",
+                    "requires": {
+                        "@babel/highlight": "^7.10.4"
+                    },
+                    "resolved": "https://registry.npmjs.org/@babel/code-frame/-/code-frame-7.10.4.tgz",
+                    "version": "7.10.4"
+                },
+                "@babel/generator": {
+                    "dev": true,
+                    "integrity": "sha512-Rn26vueFx0eOoz7iifCN2UHT6rGtnkSGWSoDRIy8jZN3B91PzeSULbswfLoOWuTuAcNwpG/mxy+uCTDnZ9Mp1g==",
+                    "requires": {
+                        "@babel/types": "^7.11.0",
+                        "jsesc": "^2.5.1",
+                        "source-map": "^0.5.0"
+                    },
+                    "resolved": "https://registry.npmjs.org/@babel/generator/-/generator-7.11.4.tgz",
+                    "version": "7.11.4"
+                },
+                "@babel/helper-function-name": {
+                    "dev": true,
+                    "integrity": "sha512-YdaSyz1n8gY44EmN7x44zBn9zQ1Ry2Y+3GTA+3vH6Mizke1Vw0aWDM66FOYEPw8//qKkmqOckrGgTYa+6sceqQ==",
+                    "requires": {
+                        "@babel/helper-get-function-arity": "^7.10.4",
+                        "@babel/template": "^7.10.4",
+                        "@babel/types": "^7.10.4"
+                    },
+                    "resolved": "https://registry.npmjs.org/@babel/helper-function-name/-/helper-function-name-7.10.4.tgz",
+                    "version": "7.10.4"
+                },
+                "@babel/helper-get-function-arity": {
+                    "dev": true,
+                    "integrity": "sha512-EkN3YDB+SRDgiIUnNgcmiD361ti+AVbL3f3Henf6dqqUyr5dMsorno0lJWJuLhDhkI5sYEpgj6y9kB8AOU1I2A==",
+                    "requires": {
+                        "@babel/types": "^7.10.4"
+                    },
+                    "resolved": "https://registry.npmjs.org/@babel/helper-get-function-arity/-/helper-get-function-arity-7.10.4.tgz",
+                    "version": "7.10.4"
+                },
+                "@babel/helper-split-export-declaration": {
+                    "dev": true,
+                    "integrity": "sha512-74Vejvp6mHkGE+m+k5vHY93FX2cAtrw1zXrZXRlG4l410Nm9PxfEiVTn1PjDPV5SnmieiueY4AFg2xqhNFuuZg==",
+                    "requires": {
+                        "@babel/types": "^7.11.0"
+                    },
+                    "resolved": "https://registry.npmjs.org/@babel/helper-split-export-declaration/-/helper-split-export-declaration-7.11.0.tgz",
+                    "version": "7.11.0"
+                },
+                "@babel/highlight": {
+                    "dev": true,
+                    "integrity": "sha512-i6rgnR/YgPEQzZZnbTHHuZdlE8qyoBNalD6F+q4vAFlcMEcqmkoG+mPqJYJCo63qPf74+Y1UZsl3l6f7/RIkmA==",
+                    "requires": {
+                        "@babel/helper-validator-identifier": "^7.10.4",
+                        "chalk": "^2.0.0",
+                        "js-tokens": "^4.0.0"
+                    },
+                    "resolved": "https://registry.npmjs.org/@babel/highlight/-/highlight-7.10.4.tgz",
+                    "version": "7.10.4"
+                },
+                "@babel/parser": {
+                    "dev": true,
+                    "integrity": "sha512-MggwidiH+E9j5Sh8pbrX5sJvMcsqS5o+7iB42M9/k0CD63MjYbdP4nhSh7uB5wnv2/RVzTZFTxzF/kIa5mrCqA==",
+                    "resolved": "https://registry.npmjs.org/@babel/parser/-/parser-7.11.4.tgz",
+                    "version": "7.11.4"
+                },
+                "@babel/template": {
+                    "dev": true,
+                    "integrity": "sha512-ZCjD27cGJFUB6nmCB1Enki3r+L5kJveX9pq1SvAUKoICy6CZ9yD8xO086YXdYhvNjBdnekm4ZnaP5yC8Cs/1tA==",
+                    "requires": {
+                        "@babel/code-frame": "^7.10.4",
+                        "@babel/parser": "^7.10.4",
+                        "@babel/types": "^7.10.4"
+                    },
+                    "resolved": "https://registry.npmjs.org/@babel/template/-/template-7.10.4.tgz",
+                    "version": "7.10.4"
+                },
+                "@babel/traverse": {
+                    "dev": true,
+                    "integrity": "sha512-ZB2V+LskoWKNpMq6E5UUCrjtDUh5IOTAyIl0dTjIEoXum/iKWkoIEKIRDnUucO6f+2FzNkE0oD4RLKoPIufDtg==",
+                    "requires": {
+                        "@babel/code-frame": "^7.10.4",
+                        "@babel/generator": "^7.11.0",
+                        "@babel/helper-function-name": "^7.10.4",
+                        "@babel/helper-split-export-declaration": "^7.11.0",
+                        "@babel/parser": "^7.11.0",
+                        "@babel/types": "^7.11.0",
+                        "debug": "^4.1.0",
+                        "globals": "^11.1.0",
+                        "lodash": "^4.17.19"
+                    },
+                    "resolved": "https://registry.npmjs.org/@babel/traverse/-/traverse-7.11.0.tgz",
+                    "version": "7.11.0"
+                },
+                "@babel/types": {
+                    "dev": true,
+                    "integrity": "sha512-O53yME4ZZI0jO1EVGtF1ePGl0LHirG4P1ibcD80XyzZcKhcMFeCXmh4Xb1ifGBIV233Qg12x4rBfQgA+tmOukA==",
+                    "requires": {
+                        "@babel/helper-validator-identifier": "^7.10.4",
+                        "lodash": "^4.17.19",
+                        "to-fast-properties": "^2.0.0"
+                    },
+                    "resolved": "https://registry.npmjs.org/@babel/types/-/types-7.11.0.tgz",
+                    "version": "7.11.0"
+                },
+                "lodash": {
+                    "dev": true,
+                    "integrity": "sha512-PlhdFcillOINfeV7Ni6oF1TAEayyZBoZ8bcshTHqOYJYlrqzRK5hagpagky5o4HfCzzd1TRkXPMFq6cKk9rGmA==",
+                    "resolved": "https://registry.npmjs.org/lodash/-/lodash-4.17.20.tgz",
+                    "version": "4.17.20"
+                }
+            },
             "dev": true,
-            "integrity": "sha512-ak5NGZGJ6LV85Q1Zc9gn2n+ayXOizryhjSUBTdu5ih1tlVCJeuQENzc4ItyCVhINVXvIT/ZQ4mheGIsfBkpskg==",
+            "integrity": "sha512-L2gX/XeUONeEbI78dXSrJzGdz4GQ+ZTA/aazfUsFaWjSe95kiCuOZ5HsXvkiw3iwF+mFHSRUfJU8t6YavocdXA==",
             "requires": {
-                "@babel/template": "^7.7.4",
-                "@babel/traverse": "^7.7.4",
-                "@babel/types": "^7.7.4"
+                "@babel/template": "^7.10.4",
+                "@babel/traverse": "^7.10.4",
+                "@babel/types": "^7.10.4"
             },
-            "resolved": "https://registry.npmjs.org/@babel/helpers/-/helpers-7.7.4.tgz",
-            "version": "7.7.4"
+            "resolved": "https://registry.npmjs.org/@babel/helpers/-/helpers-7.10.4.tgz",
+            "version": "7.10.4"
         },
         "@babel/highlight": {
             "dev": true,
             "integrity": "sha512-7dV4eu9gBxoM0dAnj/BCFDW9LFU0zvTrkq0ugM7pnHEgguOEeOz1so2ZghEdzviYzQEED0r4EAgpsBChKy1TRQ==",
             "requires": {
                 "chalk": "^2.0.0",
                 "esutils": "^2.0.2",
@@ -664,54 +951,25 @@
             "integrity": "sha512-MatJhlC4iHsIskWYyawl53KuHrt+kALSADLQQ/HkhTjX954fkxIEh4q5slL4oRAnsm/eDoZ4q0CIZpcqBuxhJQ==",
             "requires": {
                 "@babel/helper-plugin-utils": "^7.0.0"
             },
             "resolved": "https://registry.npmjs.org/@babel/plugin-transform-property-literals/-/plugin-transform-property-literals-7.7.4.tgz",
             "version": "7.7.4"
         },
-        "@babel/plugin-transform-react-display-name": {
-            "dev": true,
-            "integrity": "sha512-sBbIvqYkthai0X0vkD2xsAwluBp+LtNHH+/V4a5ydifmTtb8KOVOlrMIk/MYmIc4uTYDnjZUHQildYNo36SRJw==",
-            "requires": {
-                "@babel/helper-plugin-utils": "^7.0.0"
-            },
-            "resolved": "https://registry.npmjs.org/@babel/plugin-transform-react-display-name/-/plugin-transform-react-display-name-7.7.4.tgz",
-            "version": "7.7.4"
-        },
         "@babel/plugin-transform-react-jsx": {
             "dev": true,
             "integrity": "sha512-LixU4BS95ZTEAZdPaIuyg/k8FiiqN9laQ0dMHB4MlpydHY53uQdWCUrwjLr5o6ilS6fAgZey4Q14XBjl5tL6xw==",
             "requires": {
                 "@babel/helper-builder-react-jsx": "^7.7.4",
                 "@babel/helper-plugin-utils": "^7.0.0",
                 "@babel/plugin-syntax-jsx": "^7.7.4"
             },
             "resolved": "https://registry.npmjs.org/@babel/plugin-transform-react-jsx/-/plugin-transform-react-jsx-7.7.4.tgz",
             "version": "7.7.4"
         },
-        "@babel/plugin-transform-react-jsx-self": {
-            "dev": true,
-            "integrity": "sha512-PWYjSfqrO273mc1pKCRTIJXyqfc9vWYBax88yIhQb+bpw3XChVC7VWS4VwRVs63wFHKxizvGSd00XEr+YB9Q2A==",
-            "requires": {
-                "@babel/helper-plugin-utils": "^7.0.0",
-                "@babel/plugin-syntax-jsx": "^7.7.4"
-            },
-            "resolved": "https://registry.npmjs.org/@babel/plugin-transform-react-jsx-self/-/plugin-transform-react-jsx-self-7.7.4.tgz",
-            "version": "7.7.4"
-        },
-        "@babel/plugin-transform-react-jsx-source": {
-            "dev": true,
-            "integrity": "sha512-5ZU9FnPhqtHsOXxutRtXZAzoEJwDaP32QcobbMP1/qt7NYcsCNK8XgzJcJfoEr/ZnzVvUNInNjIW22Z6I8p9mg==",
-            "requires": {
-                "@babel/helper-plugin-utils": "^7.0.0",
-                "@babel/plugin-syntax-jsx": "^7.7.4"
-            },
-            "resolved": "https://registry.npmjs.org/@babel/plugin-transform-react-jsx-source/-/plugin-transform-react-jsx-source-7.7.4.tgz",
-            "version": "7.7.4"
-        },
         "@babel/plugin-transform-regenerator": {
             "dev": true,
             "integrity": "sha512-/8I8tPvX2FkuEyWbjRCt4qTAgZK0DVy8QRguhA524UH48RfGJy94On2ri+dCuwOpcerPRl9O4ebQkRcVzIaGBw==",
             "requires": {
                 "regenerator-transform": "^0.14.0"
             },
             "resolved": "https://registry.npmjs.org/@babel/plugin-transform-regenerator/-/plugin-transform-regenerator-7.7.5.tgz",
@@ -838,27 +1096,14 @@
                 "invariant": "^2.2.2",
                 "js-levenshtein": "^1.1.3",
                 "semver": "^5.5.0"
             },
             "resolved": "https://registry.npmjs.org/@babel/preset-env/-/preset-env-7.7.6.tgz",
             "version": "7.7.6"
         },
-        "@babel/preset-react": {
-            "dev": true,
-            "integrity": "sha512-j+vZtg0/8pQr1H8wKoaJyGL2IEk3rG/GIvua7Sec7meXVIvGycihlGMx5xcU00kqCJbwzHs18xTu3YfREOqQ+g==",
-            "requires": {
-                "@babel/helper-plugin-utils": "^7.0.0",
-                "@babel/plugin-transform-react-display-name": "^7.7.4",
-                "@babel/plugin-transform-react-jsx": "^7.7.4",
-                "@babel/plugin-transform-react-jsx-self": "^7.7.4",
-                "@babel/plugin-transform-react-jsx-source": "^7.7.4"
-            },
-            "resolved": "https://registry.npmjs.org/@babel/preset-react/-/preset-react-7.7.4.tgz",
-            "version": "7.7.4"
-        },
         "@babel/runtime": {
             "dev": true,
             "integrity": "sha512-BWAJxpNVa0QlE5gZdWjSxXtemZyZ9RmrmVozxt3NUXeZhVIJ5ANyqmMc0JDrivBZyxUuQvFxlvH4OWWOogGfUw==",
             "requires": {
                 "regenerator-runtime": "^0.13.2"
             },
             "resolved": "https://registry.npmjs.org/@babel/runtime/-/runtime-7.7.6.tgz",
@@ -980,14 +1225,36 @@
         "@parcel/utils": {
             "dev": true,
             "integrity": "sha512-cA3p4jTlaMeOtAKR/6AadanOPvKeg8VwgnHhOyfi0yClD0TZS/hi9xu12w4EzA/8NtHu0g6o4RDfcNjqN8l1AQ==",
             "resolved": "https://registry.npmjs.org/@parcel/utils/-/utils-1.11.0.tgz",
             "version": "1.11.0"
         },
         "@parcel/watcher": {
+            "dependencies": {
+                "chokidar": {
+                    "dev": true,
+                    "integrity": "sha512-ZmZUazfOzf0Nve7duiCKD23PFSCs4JPoYyccjUFF3aQkQadqBhfzhjkwBH2mNOG9cTBwhamM37EIsIkZw3nRgg==",
+                    "requires": {
+                        "anymatch": "^2.0.0",
+                        "async-each": "^1.0.1",
+                        "braces": "^2.3.2",
+                        "fsevents": "^1.2.7",
+                        "glob-parent": "^3.1.0",
+                        "inherits": "^2.0.3",
+                        "is-binary-path": "^1.0.0",
+                        "is-glob": "^4.0.0",
+                        "normalize-path": "^3.0.0",
+                        "path-is-absolute": "^1.0.0",
+                        "readdirp": "^2.2.1",
+                        "upath": "^1.1.1"
+                    },
+                    "resolved": "https://registry.npmjs.org/chokidar/-/chokidar-2.1.8.tgz",
+                    "version": "2.1.8"
+                }
+            },
             "dev": true,
             "integrity": "sha512-od+uCtCxC/KoNQAIE1vWx1YTyKYY+7CTrxBJPRh3cDWw/C0tCtlBMVlrbplscGoEpt6B27KhJDCv82PBxOERNA==",
             "requires": {
                 "@parcel/utils": "^1.11.0",
                 "chokidar": "^2.1.5"
             },
             "resolved": "https://registry.npmjs.org/@parcel/watcher/-/watcher-1.12.1.tgz",
@@ -1011,20 +1278,14 @@
         },
         "abab": {
             "dev": true,
             "integrity": "sha512-tsFzPpcttalNjFBCFMqsKYQcWxxen1pgJR56by//QwvJc4/OUS3kPOOttx2tSIfjsylB0pYu7f5D3K1RCxUnUg==",
             "resolved": "https://registry.npmjs.org/abab/-/abab-2.0.3.tgz",
             "version": "2.0.3"
         },
-        "abbrev": {
-            "dev": true,
-            "integrity": "sha512-nne9/IiQ/hzIhY6pdDnbBtz7DjPTKrY00P/zvPSm5pOFkl6xuGrGnXn/VtTNNfNtAfZ9/1RtehkszU9qcTii0Q==",
-            "resolved": "https://registry.npmjs.org/abbrev/-/abbrev-1.1.1.tgz",
-            "version": "1.1.1"
-        },
         "acorn": {
             "dev": true,
             "integrity": "sha512-1D++VG7BhrtvQpNbBzovKNc1FLGGEE/oGe7b9xJm/RFHMBeUaUGpluV9RLjZa47YFdPcDAenEYuq9pQPcMdLJg==",
             "resolved": "https://registry.npmjs.org/acorn/-/acorn-5.7.4.tgz",
             "version": "5.7.4"
         },
         "acorn-globals": {
@@ -1065,20 +1326,14 @@
         },
         "alphanum-sort": {
             "dev": true,
             "integrity": "sha1-l6ERlkmyEa0zaR2fn0hqjsn74KM=",
             "resolved": "https://registry.npmjs.org/alphanum-sort/-/alphanum-sort-1.0.2.tgz",
             "version": "1.0.2"
         },
-        "amdefine": {
-            "dev": true,
-            "integrity": "sha1-SlKCrBZHKek2Gbz9OtFR+BfOkfU=",
-            "resolved": "https://registry.npmjs.org/amdefine/-/amdefine-1.0.1.tgz",
-            "version": "1.0.1"
-        },
         "ansi-styles": {
             "dev": true,
             "integrity": "sha512-VT0ZI6kZRdTh8YyJw3SMbYm/u+NqfsAxEpWO0Pf9sq8/e94WxxOpPKx9FR1FlyCtOVDNOQ+8ntlqFxiRc+r5qA==",
             "requires": {
                 "color-convert": "^1.9.0"
             },
             "resolved": "https://registry.npmjs.org/ansi-styles/-/ansi-styles-3.2.1.tgz",
@@ -1110,62 +1365,14 @@
             "requires": {
                 "micromatch": "^3.1.4",
                 "normalize-path": "^2.1.1"
             },
             "resolved": "https://registry.npmjs.org/anymatch/-/anymatch-2.0.0.tgz",
             "version": "2.0.0"
         },
-        "aproba": {
-            "dev": true,
-            "integrity": "sha512-Y9J6ZjXtoYh8RnXVCMOU/ttDmk1aBjunq9vO0ta5x85WDQiQfUF9sIPBITdbiiIVcBo03Hi3jMxigBtsddlXRw==",
-            "resolved": "https://registry.npmjs.org/aproba/-/aproba-1.2.0.tgz",
-            "version": "1.2.0"
-        },
-        "are-we-there-yet": {
-            "dependencies": {
-                "isarray": {
-                    "dev": true,
-                    "integrity": "sha1-u5NdSFgsuhaMBoNJV6VKPgcSTxE=",
-                    "resolved": "https://registry.npmjs.org/isarray/-/isarray-1.0.0.tgz",
-                    "version": "1.0.0"
-                },
-                "readable-stream": {
-                    "dev": true,
-                    "integrity": "sha512-tQtKA9WIAhBF3+VLAseyMqZeBjW0AHJoxOtYqSUZNJxauErmLbVm2FW1y+J/YA9dUrAC39ITejlZWhVIwawkKw==",
-                    "requires": {
-                        "core-util-is": "~1.0.0",
-                        "inherits": "~2.0.3",
-                        "isarray": "~1.0.0",
-                        "process-nextick-args": "~2.0.0",
-                        "safe-buffer": "~5.1.1",
-                        "string_decoder": "~1.1.1",
-                        "util-deprecate": "~1.0.1"
-                    },
-                    "resolved": "https://registry.npmjs.org/readable-stream/-/readable-stream-2.3.6.tgz",
-                    "version": "2.3.6"
-                },
-                "string_decoder": {
-                    "dev": true,
-                    "integrity": "sha512-n/ShnvDi6FHbbVfviro+WojiFzv+s8MPMHBczVePfUpDJLwoLT0ht1l4YwBCbi8pJAveEEdnkHyPyTP/mzRfwg==",
-                    "requires": {
-                        "safe-buffer": "~5.1.0"
-                    },
-                    "resolved": "https://registry.npmjs.org/string_decoder/-/string_decoder-1.1.1.tgz",
-                    "version": "1.1.1"
-                }
-            },
-            "dev": true,
-            "integrity": "sha512-5hYdAkZlcG8tOLujVDTgCT+uPX0VnpAH28gWsLfzpXYm7wP6mp5Q/gYyR7YQ0cKVJcXJnl3j2kpBan13PtQf6w==",
-            "requires": {
-                "delegates": "^1.0.0",
-                "readable-stream": "^2.0.6"
-            },
-            "resolved": "https://registry.npmjs.org/are-we-there-yet/-/are-we-there-yet-1.1.5.tgz",
-            "version": "1.1.5"
-        },
         "argparse": {
             "dev": true,
             "integrity": "sha512-o5Roy6tNG4SL/FOkCAN6RzjiakZS25RLYFrcMttJqbdd8BWrnA+fGz57iN5Pb06pvBGvl5gQ0B48dJlslXvoTg==",
             "requires": {
                 "sprintf-js": "~1.0.2"
             },
             "resolved": "https://registry.npmjs.org/argparse/-/argparse-1.0.10.tgz",
@@ -1191,31 +1398,20 @@
         },
         "array-equal": {
             "dev": true,
             "integrity": "sha1-jCpe8kcv2ep0KwTHenUJO6J1fJM=",
             "resolved": "https://registry.npmjs.org/array-equal/-/array-equal-1.0.0.tgz",
             "version": "1.0.0"
         },
-        "array-find-index": {
-            "dev": true,
-            "integrity": "sha1-3wEKoSh+Fku9pvlyOwqWoexBh6E=",
-            "resolved": "https://registry.npmjs.org/array-find-index/-/array-find-index-1.0.2.tgz",
-            "version": "1.0.2"
-        },
         "array-unique": {
             "dev": true,
             "integrity": "sha1-qJS3XUvE9s1nnvMkSp/Y9Gri1Cg=",
             "resolved": "https://registry.npmjs.org/array-unique/-/array-unique-0.3.2.tgz",
             "version": "0.3.2"
         },
-        "asap": {
-            "integrity": "sha1-5QNHYR1+aQlDIIu9r+vLwvuGbUY=",
-            "resolved": "https://registry.npmjs.org/asap/-/asap-2.0.6.tgz",
-            "version": "2.0.6"
-        },
         "asn1": {
             "dev": true,
             "integrity": "sha512-jxwzQpLQjSmWXgwaCZE9Nz+glAG01yF1QnWgbhGwHI5A6FRIEY6IVqtHhIepHqI7/kyEyQEagBC5mBEFlIYvdg==",
             "requires": {
                 "safer-buffer": "~2.1.0"
             },
             "resolved": "https://registry.npmjs.org/asn1/-/asn1-0.2.4.tgz",
@@ -1273,20 +1469,14 @@
         },
         "async-each": {
             "dev": true,
             "integrity": "sha512-z/WhQ5FPySLdvREByI2vZiTWwCnF0moMJ1hK9YQwDTHKh6I7/uSckMetoRGb5UBZPC1z0jlw+n/XCgjeH7y1AQ==",
             "resolved": "https://registry.npmjs.org/async-each/-/async-each-1.0.3.tgz",
             "version": "1.0.3"
         },
-        "async-foreach": {
-            "dev": true,
-            "integrity": "sha1-NhIfhFwFeBct5Bmpfb6x0W7DRUI=",
-            "resolved": "https://registry.npmjs.org/async-foreach/-/async-foreach-0.1.3.tgz",
-            "version": "0.1.3"
-        },
         "async-limiter": {
             "dev": true,
             "integrity": "sha512-csOlWGAcRFJaI6m+F2WKdnMKr4HhdhFVBk0H/QbJFMCr+uO2kwohwXQPxw/9OCxp05r5ghVBFSyioixx3gfkNQ==",
             "resolved": "https://registry.npmjs.org/async-limiter/-/async-limiter-1.0.1.tgz",
             "version": "1.0.1"
         },
         "asynckit": {
@@ -1297,29 +1487,14 @@
         },
         "atob": {
             "dev": true,
             "integrity": "sha512-Wm6ukoaOGJi/73p/cl2GvLjTI5JM1k/O14isD73YML8StrH/7/lRFgmg8nICZgD3bZZvjwCGxtMOD3wWNAu8cg==",
             "resolved": "https://registry.npmjs.org/atob/-/atob-2.1.2.tgz",
             "version": "2.1.2"
         },
-        "autoprefixer": {
-            "dev": true,
-            "integrity": "sha512-8T5Y1C5Iyj6PgkPSFd0ODvK9DIleuPKUPYniNxybS47g2k2wFgLZ46lGQHlBuGKIAEV8fbCDfKCCRS1tvOgc3Q==",
-            "requires": {
-                "browserslist": "^4.8.0",
-                "caniuse-lite": "^1.0.30001012",
-                "chalk": "^2.4.2",
-                "normalize-range": "^0.1.2",
-                "num2fraction": "^1.2.2",
-                "postcss": "^7.0.23",
-                "postcss-value-parser": "^4.0.2"
-            },
-            "resolved": "https://registry.npmjs.org/autoprefixer/-/autoprefixer-9.7.3.tgz",
-            "version": "9.7.3"
-        },
         "aws-sign2": {
             "dev": true,
             "integrity": "sha1-tG6JCTSpWR8tL2+G1+ap8bP+dqg=",
             "resolved": "https://registry.npmjs.org/aws-sign2/-/aws-sign2-0.7.0.tgz",
             "version": "0.7.0"
         },
         "aws4": {
@@ -1473,23 +1648,14 @@
             "integrity": "sha512-p2q/t/mhvuOj/UeLlV6566GD/guowlr0hHxClI0W9m7MWYkL1F0hLo+0Aexs9HSPCtR1SXQ0TD3MMKrXZajbiQ==",
             "requires": {
                 "file-uri-to-path": "1.0.0"
             },
             "resolved": "https://registry.npmjs.org/bindings/-/bindings-1.5.0.tgz",
             "version": "1.5.0"
         },
-        "block-stream": {
-            "dev": true,
-            "integrity": "sha1-E+v+d4oDIFz+A3UUgeu0szAMEmo=",
-            "requires": {
-                "inherits": "~2.0.0"
-            },
-            "resolved": "https://registry.npmjs.org/block-stream/-/block-stream-0.0.9.tgz",
-            "version": "0.0.9"
-        },
         "bn.js": {
             "dev": true,
             "integrity": "sha512-ItfYfPLkWHUjckQCk8xC+LwxgK8NYcXywGigJgSwOP8Y2iyWT4f2vsZnoOXTTbo+o5yXmIUJ4gn5538SO5S3gA==",
             "resolved": "https://registry.npmjs.org/bn.js/-/bn.js-4.11.8.tgz",
             "version": "4.11.8"
         },
         "boolbase": {
@@ -1737,14 +1903,20 @@
         },
         "callsites": {
             "dev": true,
             "integrity": "sha1-BuuE8A7qQT2oav/vrL/7Ngk7PFA=",
             "resolved": "https://registry.npmjs.org/callsites/-/callsites-2.0.0.tgz",
             "version": "2.0.0"
         },
+        "camelcase": {
+            "dev": true,
+            "integrity": "sha512-L28STB170nwWS63UjtlEOE3dldQApaJXZkOI1uMFfzf3rRuPegHaHesyee+YxQ+W6SvRDQV6UrdOdRiR153wJg==",
+            "resolved": "https://registry.npmjs.org/camelcase/-/camelcase-5.3.1.tgz",
+            "version": "5.3.1"
+        },
         "caniuse-api": {
             "dev": true,
             "integrity": "sha512-bsTwuIg/BZZK/vreVTYYbSWoe2F+71P7K5QGEX+pT250DZbfU1MQ5prOKpPR+LL6uWKK3KMwMCAS74QB3Um1uw==",
             "requires": {
                 "browserslist": "^4.0.0",
                 "caniuse-lite": "^1.0.0",
                 "lodash.memoize": "^4.1.2",
@@ -1784,32 +1956,113 @@
                 "escape-string-regexp": "^1.0.5",
                 "supports-color": "^5.3.0"
             },
             "resolved": "https://registry.npmjs.org/chalk/-/chalk-2.4.2.tgz",
             "version": "2.4.2"
         },
         "chokidar": {
+            "dependencies": {
+                "anymatch": {
+                    "dev": true,
+                    "integrity": "sha512-mM8522psRCqzV+6LhomX5wgp25YVibjh8Wj23I5RPkPppSVSjyKD2A2mBJmWGa+KN7f2D6LNh9jkBCeyLktzjg==",
+                    "requires": {
+                        "normalize-path": "^3.0.0",
+                        "picomatch": "^2.0.4"
+                    },
+                    "resolved": "https://registry.npmjs.org/anymatch/-/anymatch-3.1.1.tgz",
+                    "version": "3.1.1"
+                },
+                "binary-extensions": {
+                    "dev": true,
+                    "integrity": "sha512-1Yj8h9Q+QDF5FzhMs/c9+6UntbD5MkRfRwac8DoEm9ZfUBZ7tZ55YcGVAzEe4bXsdQHEk+s9S5wsOKVdZrw0tQ==",
+                    "resolved": "https://registry.npmjs.org/binary-extensions/-/binary-extensions-2.1.0.tgz",
+                    "version": "2.1.0"
+                },
+                "braces": {
+                    "dev": true,
+                    "integrity": "sha512-b8um+L1RzM3WDSzvhm6gIz1yfTbBt6YTlcEKAvsmqCZZFw46z626lVj9j1yEPW33H5H+lBQpZMP1k8l+78Ha0A==",
+                    "requires": {
+                        "fill-range": "^7.0.1"
+                    },
+                    "resolved": "https://registry.npmjs.org/braces/-/braces-3.0.2.tgz",
+                    "version": "3.0.2"
+                },
+                "fill-range": {
+                    "dev": true,
+                    "integrity": "sha512-qOo9F+dMUmC2Lcb4BbVvnKJxTPjCm+RRpe4gDuGrzkL7mEVl/djYSu2OdQ2Pa302N4oqkSg9ir6jaLWJ2USVpQ==",
+                    "requires": {
+                        "to-regex-range": "^5.0.1"
+                    },
+                    "resolved": "https://registry.npmjs.org/fill-range/-/fill-range-7.0.1.tgz",
+                    "version": "7.0.1"
+                },
+                "fsevents": {
+                    "dev": true,
+                    "integrity": "sha512-Auw9a4AxqWpa9GUfj370BMPzzyncfBABW8Mab7BGWBYDj4Isgq+cDKtx0i6u9jcX9pQDnswsaaOTgTmA5pEjuQ==",
+                    "optional": true,
+                    "resolved": "https://registry.npmjs.org/fsevents/-/fsevents-2.1.3.tgz",
+                    "version": "2.1.3"
+                },
+                "glob-parent": {
+                    "dev": true,
+                    "integrity": "sha512-FnI+VGOpnlGHWZxthPGR+QhR78fuiK0sNLkHQv+bL9fQi57lNNdquIbna/WrfROrolq8GK5Ek6BiMwqL/voRYQ==",
+                    "requires": {
+                        "is-glob": "^4.0.1"
+                    },
+                    "resolved": "https://registry.npmjs.org/glob-parent/-/glob-parent-5.1.1.tgz",
+                    "version": "5.1.1"
+                },
+                "is-binary-path": {
+                    "dev": true,
+                    "integrity": "sha512-ZMERYes6pDydyuGidse7OsHxtbI7WVeUEozgR/g7rd0xUimYNlvZRE/K2MgZTjWy725IfelLeVcEM97mmtRGXw==",
+                    "requires": {
+                        "binary-extensions": "^2.0.0"
+                    },
+                    "resolved": "https://registry.npmjs.org/is-binary-path/-/is-binary-path-2.1.0.tgz",
+                    "version": "2.1.0"
+                },
+                "is-number": {
+                    "dev": true,
+                    "integrity": "sha512-41Cifkg6e8TylSpdtTpeLVMqvSBEVzTttHvERD741+pnZ8ANv0004MRL43QKPDlK9cGvNp6NZWZUBlbGXYxxng==",
+                    "resolved": "https://registry.npmjs.org/is-number/-/is-number-7.0.0.tgz",
+                    "version": "7.0.0"
+                },
+                "readdirp": {
+                    "dev": true,
+                    "integrity": "sha512-0xe001vZBnJEK+uKcj8qOhyAKPzIT+gStxWr3LCB0DwcXR5NZJ3IaC+yGnHCYzB/S7ov3m3EEbZI2zeNvX+hGQ==",
+                    "requires": {
+                        "picomatch": "^2.2.1"
+                    },
+                    "resolved": "https://registry.npmjs.org/readdirp/-/readdirp-3.4.0.tgz",
+                    "version": "3.4.0"
+                },
+                "to-regex-range": {
+                    "dev": true,
+                    "integrity": "sha512-65P7iz6X5yEr1cwcgvQxbbIw7Uk3gOy5dIdtZ4rDveLqhrdJP+Li/Hx6tyK0NEb+2GCyneCMJiGqrADCSNk8sQ==",
+                    "requires": {
+                        "is-number": "^7.0.0"
+                    },
+                    "resolved": "https://registry.npmjs.org/to-regex-range/-/to-regex-range-5.0.1.tgz",
+                    "version": "5.0.1"
+                }
+            },
             "dev": true,
-            "integrity": "sha512-ZmZUazfOzf0Nve7duiCKD23PFSCs4JPoYyccjUFF3aQkQadqBhfzhjkwBH2mNOG9cTBwhamM37EIsIkZw3nRgg==",
+            "integrity": "sha512-IZHaDeBeI+sZJRX7lGcXsdzgvZqKv6sECqsbErJA4mHWfpRrD8B97kSFN4cQz6nGBGiuFia1MKR4d6c1o8Cv7A==",
             "requires": {
-                "anymatch": "^2.0.0",
-                "async-each": "^1.0.1",
-                "braces": "^2.3.2",
-                "fsevents": "^1.2.7",
-                "glob-parent": "^3.1.0",
-                "inherits": "^2.0.3",
-                "is-binary-path": "^1.0.0",
-                "is-glob": "^4.0.0",
-                "normalize-path": "^3.0.0",
-                "path-is-absolute": "^1.0.0",
-                "readdirp": "^2.2.1",
-                "upath": "^1.1.1"
+                "anymatch": "~3.1.1",
+                "braces": "~3.0.2",
+                "fsevents": "~2.1.2",
+                "glob-parent": "~5.1.0",
+                "is-binary-path": "~2.1.0",
+                "is-glob": "~4.0.1",
+                "normalize-path": "~3.0.0",
+                "readdirp": "~3.4.0"
             },
-            "resolved": "https://registry.npmjs.org/chokidar/-/chokidar-2.1.8.tgz",
-            "version": "2.1.8"
+            "resolved": "https://registry.npmjs.org/chokidar/-/chokidar-3.4.2.tgz",
+            "version": "3.4.2"
         },
         "cipher-base": {
             "dev": true,
             "integrity": "sha512-Kkht5ye6ZGmwv40uUDZztayT2ThLQGfnj/T71N/XzeZeo3nf8foyW7zGTsPYkEya3m5f3cAypH+qe7YOrM1U2Q==",
             "requires": {
                 "inherits": "^2.0.1",
                 "safe-buffer": "^5.0.1"
@@ -1851,62 +2104,14 @@
         },
         "cli-spinners": {
             "dev": true,
             "integrity": "sha512-1QL4544moEsDVH9T/l6Cemov/37iv1RtoKf7NJ04A60+4MREXNfx/QvavbH6QoGdsD4N4Mwy49cmaINR/o2mdg==",
             "resolved": "https://registry.npmjs.org/cli-spinners/-/cli-spinners-1.3.1.tgz",
             "version": "1.3.1"
         },
-        "cliui": {
-            "dependencies": {
-                "ansi-regex": {
-                    "dev": true,
-                    "integrity": "sha1-w7M6te42DYbg5ijwRorn7yfWVN8=",
-                    "resolved": "https://registry.npmjs.org/ansi-regex/-/ansi-regex-2.1.1.tgz",
-                    "version": "2.1.1"
-                },
-                "is-fullwidth-code-point": {
-                    "dev": true,
-                    "integrity": "sha1-754xOG8DGn8NZDr4L95QxFfvAMs=",
-                    "requires": {
-                        "number-is-nan": "^1.0.0"
-                    },
-                    "resolved": "https://registry.npmjs.org/is-fullwidth-code-point/-/is-fullwidth-code-point-1.0.0.tgz",
-                    "version": "1.0.0"
-                },
-                "string-width": {
-                    "dev": true,
-                    "integrity": "sha1-EYvfW4zcUaKn5w0hHgfisLmxB9M=",
-                    "requires": {
-                        "code-point-at": "^1.0.0",
-                        "is-fullwidth-code-point": "^1.0.0",
-                        "strip-ansi": "^3.0.0"
-                    },
-                    "resolved": "https://registry.npmjs.org/string-width/-/string-width-1.0.2.tgz",
-                    "version": "1.0.2"
-                },
-                "strip-ansi": {
-                    "dev": true,
-                    "integrity": "sha1-ajhfuIU9lS1f8F0Oiq+UJ43GPc8=",
-                    "requires": {
-                        "ansi-regex": "^2.0.0"
-                    },
-                    "resolved": "https://registry.npmjs.org/strip-ansi/-/strip-ansi-3.0.1.tgz",
-                    "version": "3.0.1"
-                }
-            },
-            "dev": true,
-            "integrity": "sha1-EgYBU3qRbSmUD5NNo7SNWFo5IT0=",
-            "requires": {
-                "string-width": "^1.0.1",
-                "strip-ansi": "^3.0.1",
-                "wrap-ansi": "^2.0.0"
-            },
-            "resolved": "https://registry.npmjs.org/cliui/-/cliui-3.2.0.tgz",
-            "version": "3.2.0"
-        },
         "clone": {
             "dev": true,
             "integrity": "sha1-G39Ln1kfHo+DZwQBYANFoCiHQ18=",
             "resolved": "https://registry.npmjs.org/clone/-/clone-2.1.2.tgz",
             "version": "2.1.2"
         },
         "coa": {
@@ -1916,20 +2121,14 @@
                 "@types/q": "^1.5.1",
                 "chalk": "^2.4.1",
                 "q": "^1.1.2"
             },
             "resolved": "https://registry.npmjs.org/coa/-/coa-2.0.2.tgz",
             "version": "2.0.2"
         },
-        "code-point-at": {
-            "dev": true,
-            "integrity": "sha1-DQcLTQQ6W+ozovGkDi7bPZpMz3c=",
-            "resolved": "https://registry.npmjs.org/code-point-at/-/code-point-at-1.1.0.tgz",
-            "version": "1.1.0"
-        },
         "collection-visit": {
             "dev": true,
             "integrity": "sha1-S8A3PBZLwykbTTaMgpzxqApZ3KA=",
             "requires": {
                 "map-visit": "^1.0.0",
                 "object-visit": "^1.0.0"
             },
@@ -2006,20 +2205,14 @@
         },
         "console-browserify": {
             "dev": true,
             "integrity": "sha512-ZMkYO/LkF17QvCPqM0gxw8yUzigAOZOSWSHg91FH6orS7vcEj5dVZTidN2fQ14yBSdg97RqhSNwLUXInd52OTA==",
             "resolved": "https://registry.npmjs.org/console-browserify/-/console-browserify-1.2.0.tgz",
             "version": "1.2.0"
         },
-        "console-control-strings": {
-            "dev": true,
-            "integrity": "sha1-PXz0Rk22RG6mRL9LOVB/mFEAjo4=",
-            "resolved": "https://registry.npmjs.org/console-control-strings/-/console-control-strings-1.1.0.tgz",
-            "version": "1.1.0"
-        },
         "constants-browserify": {
             "dev": true,
             "integrity": "sha1-wguW2MYXdIqvHBYCF2DNJ/y4y3U=",
             "resolved": "https://registry.npmjs.org/constants-browserify/-/constants-browserify-1.0.0.tgz",
             "version": "1.0.0"
         },
         "convert-source-map": {
@@ -2431,23 +2624,14 @@
             "integrity": "sha512-GBrLZYZ4X4x6/QEoBnIrqb8B/f5l4+8me2dkom/j1Gtbxy0kBv6OGzKuAsGM75bkGwGAFkt56Iwg28S3XTZgSA==",
             "requires": {
                 "cssom": "0.3.x"
             },
             "resolved": "https://registry.npmjs.org/cssstyle/-/cssstyle-1.4.0.tgz",
             "version": "1.4.0"
         },
-        "currently-unhandled": {
-            "dev": true,
-            "integrity": "sha1-mI3zP+qxke95mmE2nddsF635V+o=",
-            "requires": {
-                "array-find-index": "^1.0.1"
-            },
-            "resolved": "https://registry.npmjs.org/currently-unhandled/-/currently-unhandled-0.4.1.tgz",
-            "version": "0.4.1"
-        },
         "dashdash": {
             "dev": true,
             "integrity": "sha1-hTz6D3y+L+1d4gMmuN1YEDX24vA=",
             "requires": {
                 "assert-plus": "^1.0.0"
             },
             "resolved": "https://registry.npmjs.org/dashdash/-/dashdash-1.14.1.tgz",
@@ -2470,31 +2654,35 @@
             "requires": {
                 "bindings": "^1.5.0",
                 "node-addon-api": "^1.7.1"
             },
             "resolved": "https://registry.npmjs.org/deasync/-/deasync-0.1.16.tgz",
             "version": "0.1.16"
         },
+        "debug": {
+            "dev": true,
+            "integrity": "sha512-pYAIzeRo8J6KPEaJ0VWOh5Pzkbw/RetuzehGM7QRRX5he4fPHx2rdKMB256ehJCkX+XRQm16eZLqLNS8RSZXZw==",
+            "requires": {
+                "ms": "^2.1.1"
+            },
+            "resolved": "https://registry.npmjs.org/debug/-/debug-4.1.1.tgz",
+            "version": "4.1.1"
+        },
         "decamelize": {
             "dev": true,
             "integrity": "sha1-9lNNFRSCabIDUue+4m9QH5oZEpA=",
             "resolved": "https://registry.npmjs.org/decamelize/-/decamelize-1.2.0.tgz",
             "version": "1.2.0"
         },
         "decode-uri-component": {
             "dev": true,
             "integrity": "sha1-6zkTMzRYd1y4TNGh+uBiEGu4dUU=",
             "resolved": "https://registry.npmjs.org/decode-uri-component/-/decode-uri-component-0.2.0.tgz",
             "version": "0.2.0"
         },
-        "decorate-component-with-props": {
-            "integrity": "sha512-tTYQojixN64yK3/WBODMfvss/zbmyUx9HQXhzSxZiSiofeekVeRyyuToy9BCiTMrVEIKWxTcla2t3y5qdaUF7Q==",
-            "resolved": "https://registry.npmjs.org/decorate-component-with-props/-/decorate-component-with-props-1.1.0.tgz",
-            "version": "1.1.0"
-        },
         "deep-is": {
             "dev": true,
             "integrity": "sha1-s2nW+128E+7PUk+RsHD+7cNXzzQ=",
             "resolved": "https://registry.npmjs.org/deep-is/-/deep-is-0.1.3.tgz",
             "version": "0.1.3"
         },
         "defaults": {
@@ -2566,20 +2754,14 @@
         },
         "delayed-stream": {
             "dev": true,
             "integrity": "sha1-3zrhmayt+31ECqrgsp4icrJOxhk=",
             "resolved": "https://registry.npmjs.org/delayed-stream/-/delayed-stream-1.0.0.tgz",
             "version": "1.0.0"
         },
-        "delegates": {
-            "dev": true,
-            "integrity": "sha1-hMbhWbgZBP3KWaDvRM2HDTElD5o=",
-            "resolved": "https://registry.npmjs.org/delegates/-/delegates-1.0.0.tgz",
-            "version": "1.0.0"
-        },
         "depd": {
             "dev": true,
             "integrity": "sha1-m81S4UwJd2PnSbJ0xDRu0uVgtak=",
             "resolved": "https://registry.npmjs.org/depd/-/depd-1.1.2.tgz",
             "version": "1.1.2"
         },
         "des.js": {
@@ -2671,76 +2853,29 @@
                 "domelementtype": "1"
             },
             "resolved": "https://registry.npmjs.org/domutils/-/domutils-1.7.0.tgz",
             "version": "1.7.0"
         },
         "dot-prop": {
             "dev": true,
-            "integrity": "sha512-tUMXrxlExSW6U2EXiiKGSBVdYgtV8qlHL+C10TsW4PURY/ic+eaysnSkwB4kA/mBlCyy/IKDJ+Lc3wbWeaXtuQ==",
-            "requires": {
-                "is-obj": "^1.0.0"
-            },
-            "resolved": "https://registry.npmjs.org/dot-prop/-/dot-prop-4.2.0.tgz",
+            "resolved": "",
             "version": "4.2.0"
         },
         "dotenv": {
             "dev": true,
             "integrity": "sha512-4As8uPrjfwb7VXC+WnLCbXK7y+Ueb2B3zgNCePYfhxS1PYeaO1YTeplffTEcbfLhvFNGLAz90VvJs9yomG7bow==",
             "resolved": "https://registry.npmjs.org/dotenv/-/dotenv-5.0.1.tgz",
             "version": "5.0.1"
         },
         "dotenv-expand": {
             "dev": true,
             "integrity": "sha512-YXQl1DSa4/PQyRfgrv6aoNjhasp/p4qs9FjJ4q4cQk+8m4r6k4ZSiEyytKG8f8W9gi8WsQtIObNmKd+tMzNTmA==",
             "resolved": "https://registry.npmjs.org/dotenv-expand/-/dotenv-expand-5.1.0.tgz",
             "version": "5.1.0"
         },
-        "draft-js": {
-            "integrity": "sha512-LE6jSCV9nkPhfVX2ggcRLA4FKs6zWq9ceuO/88BpXdNCS7mjRTgs0NsV6piUCJX9YxMsB9An33wnkMmU2sD2Zg==",
-            "requires": {
-                "fbjs": "^0.8.15",
-                "immutable": "~3.7.4",
-                "object-assign": "^4.1.0"
-            },
-            "resolved": "https://registry.npmjs.org/draft-js/-/draft-js-0.10.5.tgz",
-            "version": "0.10.5"
-        },
-        "draft-js-plugins-editor": {
-            "integrity": "sha512-fKGe71irNvFHJ5L/lUrh+3vPkBNq0de6x+cgiZUJ9zQERc5KPBtGXIFiarLFVHyrRTCPq+K6xmgfFSAERaFHPw==",
-            "requires": {
-                "decorate-component-with-props": "^1.0.2",
-                "find-with-regex": "^1.1.3",
-                "immutable": "~3.7.4",
-                "prop-types": "^15.5.8",
-                "union-class-names": "^1.0.0"
-            },
-            "resolved": "https://registry.npmjs.org/draft-js-plugins-editor/-/draft-js-plugins-editor-2.1.1.tgz",
-            "version": "2.1.1"
-        },
-        "draftail": {
-            "integrity": "sha512-LOG4YgrJX4BMYJX5XrKGBegH9f/M21I8nFt+7MrPAB0ABXpURZhUVzVfWVa6hEdw6yOl2Z1T4H2G4OFTouK6Bg==",
-            "requires": {
-                "decorate-component-with-props": "^1.0.2",
-                "draft-js-plugins-editor": "^2.1.1",
-                "draftjs-conductor": "^1.0.0",
-                "draftjs-filters": "^2.2.3"
-            },
-            "resolved": "https://registry.npmjs.org/draftail/-/draftail-1.3.0.tgz",
-            "version": "1.3.0"
-        },
-        "draftjs-conductor": {
-            "integrity": "sha512-pz5MIpS2aH6fgo2jrHo0Rt+rxqRgqnbrxEaaTiFLW4Dg/0U0eZhyxZPt6pByoS20Q7jCYOpolGpszKodNVi+TQ==",
-            "resolved": "https://registry.npmjs.org/draftjs-conductor/-/draftjs-conductor-1.0.0.tgz",
-            "version": "1.0.0"
-        },
-        "draftjs-filters": {
-            "integrity": "sha512-DWjIxCFnoysGcl9//aATv4C+zT9BL830+3TWIXQqsthVA52ETiHxMJ0S+R5nUAROVg6tjq7OsgNl19F8U+qxgw==",
-            "resolved": "https://registry.npmjs.org/draftjs-filters/-/draftjs-filters-2.2.4.tgz",
-            "version": "2.2.4"
-        },
         "duplexer2": {
             "dependencies": {
                 "isarray": {
                     "dev": true,
                     "integrity": "sha1-u5NdSFgsuhaMBoNJV6VKPgcSTxE=",
                     "resolved": "https://registry.npmjs.org/isarray/-/isarray-1.0.0.tgz",
                     "version": "1.0.0"
@@ -2798,41 +2933,33 @@
             "dev": true,
             "integrity": "sha512-Tc8JQEfGQ1MzfSzI/bTlSr7btJv/FFO7Yh6tanqVmIWOuNCu6/D1MilIEgLtmWqIrsv+o4IjpLAhgMBr/ncNAA==",
             "resolved": "https://registry.npmjs.org/electron-to-chromium/-/electron-to-chromium-1.3.322.tgz",
             "version": "1.3.322"
         },
         "elliptic": {
             "dev": true,
-            "integrity": "sha512-f4x70okzZbIQl/NSRLkI/+tteV/9WqL98zx+SQ69KbXxmVrmjwsNUPn/gYJJ0sHvEak24cZgHIPegRePAtA/xw==",
+            "integrity": "sha512-IMqzv5wNQf+E6aHeIqATs0tOLeOTwj1QKbRcS3jBbYkl5oLAserA8yJTT7/VyHUYG91PRmPyeQDObKLPpeS4dw==",
             "requires": {
                 "bn.js": "^4.4.0",
                 "brorand": "^1.0.1",
                 "hash.js": "^1.0.0",
                 "hmac-drbg": "^1.0.0",
                 "inherits": "^2.0.1",
                 "minimalistic-assert": "^1.0.0",
                 "minimalistic-crypto-utils": "^1.0.0"
             },
-            "resolved": "https://registry.npmjs.org/elliptic/-/elliptic-6.5.2.tgz",
-            "version": "6.5.2"
+            "resolved": "https://registry.npmjs.org/elliptic/-/elliptic-6.5.3.tgz",
+            "version": "6.5.3"
         },
         "encodeurl": {
             "dev": true,
             "integrity": "sha1-rT/0yG7C0CkyL1oCw6mmBslbP1k=",
             "resolved": "https://registry.npmjs.org/encodeurl/-/encodeurl-1.0.2.tgz",
             "version": "1.0.2"
         },
-        "encoding": {
-            "integrity": "sha1-U4tm8+5izRq1HsMjgp0flIDHS+s=",
-            "requires": {
-                "iconv-lite": "~0.4.13"
-            },
-            "resolved": "https://registry.npmjs.org/encoding/-/encoding-0.1.12.tgz",
-            "version": "0.1.12"
-        },
         "entities": {
             "dev": true,
             "integrity": "sha512-f2LZMYl1Fzu7YSBKg+RoROelpOaNrcGmE9AZubeDfrCEia483oW4MI4VyFd5VNHIgQ/7qm1I0wUHK1eJnn2y2w==",
             "resolved": "https://registry.npmjs.org/entities/-/entities-1.1.2.tgz",
             "version": "1.1.2"
         },
         "envinfo": {
@@ -2964,19 +3091,14 @@
             "requires": {
                 "md5.js": "^1.3.4",
                 "safe-buffer": "^5.1.1"
             },
             "resolved": "https://registry.npmjs.org/evp_bytestokey/-/evp_bytestokey-1.0.3.tgz",
             "version": "1.0.3"
         },
-        "exenv": {
-            "integrity": "sha1-KueOhdmJQVhnCwPUe+wfA72Ru50=",
-            "resolved": "https://registry.npmjs.org/exenv/-/exenv-1.2.2.tgz",
-            "version": "1.2.2"
-        },
         "expand-brackets": {
             "dependencies": {
                 "debug": {
                     "dev": true,
                     "integrity": "sha512-bC7ElrdJaJnPbAP+1EotYvqZsb3ecl5wi6Bfi6BJTUcNowp6cvspg0jXznRTKDjm/E7AdgFBVeAPVMNcKGsHMA==",
                     "requires": {
                         "ms": "2.0.0"
@@ -3167,35 +3289,14 @@
         },
         "fastparse": {
             "dev": true,
             "integrity": "sha512-483XLLxTVIwWK3QTrMGRqUfUpoOs/0hbQrl2oz4J0pAcm3A3bu84wxTFqGqkJzewCLdME38xJLJAxBABfQT8sQ==",
             "resolved": "https://registry.npmjs.org/fastparse/-/fastparse-1.1.2.tgz",
             "version": "1.1.2"
         },
-        "fbjs": {
-            "dependencies": {
-                "core-js": {
-                    "integrity": "sha1-ZSKUwUZR2yj6k70tX/KYOk8IxjY=",
-                    "resolved": "https://registry.npmjs.org/core-js/-/core-js-1.2.7.tgz",
-                    "version": "1.2.7"
-                }
-            },
-            "integrity": "sha1-xNWY6taUkRJlPWWIsBpc3Nn5D90=",
-            "requires": {
-                "core-js": "^1.0.0",
-                "isomorphic-fetch": "^2.1.1",
-                "loose-envify": "^1.0.0",
-                "object-assign": "^4.1.0",
-                "promise": "^7.1.1",
-                "setimmediate": "^1.0.5",
-                "ua-parser-js": "^0.7.18"
-            },
-            "resolved": "https://registry.npmjs.org/fbjs/-/fbjs-0.8.17.tgz",
-            "version": "0.8.17"
-        },
         "file-uri-to-path": {
             "dev": true,
             "integrity": "sha512-0Zt+s3L7Vf1biwWZ29aARiVYLx7iMGnEUl9x33fbB/j3jR81u/O2LbqK+Bm1CDSNDKVtJ/YjwY7TUd5SkeLQLw==",
             "resolved": "https://registry.npmjs.org/file-uri-to-path/-/file-uri-to-path-1.0.0.tgz",
             "version": "1.0.0"
         },
         "filesize": {
@@ -3223,19 +3324,14 @@
                 "is-number": "^3.0.0",
                 "repeat-string": "^1.6.1",
                 "to-regex-range": "^2.1.0"
             },
             "resolved": "https://registry.npmjs.org/fill-range/-/fill-range-4.0.0.tgz",
             "version": "4.0.0"
         },
-        "find-with-regex": {
-            "integrity": "sha512-zkEVQ1H3PIQL/19ADKt1lCQU4QGM3OneiderUcFgn5EgTm/TnoUh7HxPAwP8w/vXxWSLC6KtpbDQpypJ5+majw==",
-            "resolved": "https://registry.npmjs.org/find-with-regex/-/find-with-regex-1.1.3.tgz",
-            "version": "1.1.3"
-        },
         "for-in": {
             "dev": true,
             "integrity": "sha1-gQaNKVqBQuwKxybG4iAMMPttXoA=",
             "resolved": "https://registry.npmjs.org/for-in/-/for-in-1.0.2.tgz",
             "version": "1.0.2"
         },
         "foreach": {
@@ -3281,667 +3377,647 @@
             "integrity": "sha1-FQStJSMVjKpA20onh8sBQRmU6k8=",
             "resolved": "https://registry.npmjs.org/fs.realpath/-/fs.realpath-1.0.0.tgz",
             "version": "1.0.0"
         },
         "fsevents": {
             "dependencies": {
                 "abbrev": {
-                    "bundled": true,
                     "dev": true,
+                    "integrity": "sha512-nne9/IiQ/hzIhY6pdDnbBtz7DjPTKrY00P/zvPSm5pOFkl6xuGrGnXn/VtTNNfNtAfZ9/1RtehkszU9qcTii0Q==",
                     "optional": true,
+                    "resolved": false,
                     "version": "1.1.1"
                 },
                 "ansi-regex": {
-                    "bundled": true,
                     "dev": true,
+                    "integrity": "sha1-w7M6te42DYbg5ijwRorn7yfWVN8=",
                     "optional": true,
+                    "resolved": false,
                     "version": "2.1.1"
                 },
                 "aproba": {
-                    "bundled": true,
                     "dev": true,
+                    "integrity": "sha512-Y9J6ZjXtoYh8RnXVCMOU/ttDmk1aBjunq9vO0ta5x85WDQiQfUF9sIPBITdbiiIVcBo03Hi3jMxigBtsddlXRw==",
                     "optional": true,
+                    "resolved": false,
                     "version": "1.2.0"
                 },
                 "are-we-there-yet": {
-                    "bundled": true,
                     "dev": true,
+                    "integrity": "sha512-5hYdAkZlcG8tOLujVDTgCT+uPX0VnpAH28gWsLfzpXYm7wP6mp5Q/gYyR7YQ0cKVJcXJnl3j2kpBan13PtQf6w==",
                     "optional": true,
                     "requires": {
                         "delegates": "^1.0.0",
                         "readable-stream": "^2.0.6"
                     },
+                    "resolved": false,
                     "version": "1.1.5"
                 },
                 "balanced-match": {
-                    "bundled": true,
                     "dev": true,
+                    "integrity": "sha1-ibTRmasr7kneFk6gK4nORi1xt2c=",
                     "optional": true,
+                    "resolved": false,
                     "version": "1.0.0"
                 },
                 "brace-expansion": {
-                    "bundled": true,
                     "dev": true,
+                    "integrity": "sha512-iCuPHDFgrHX7H2vEI/5xpz07zSHB00TpugqhmYtVmMO6518mCuRMoOYFldEBl0g187ufozdaHgWKcYFb61qGiA==",
                     "optional": true,
                     "requires": {
                         "balanced-match": "^1.0.0",
                         "concat-map": "0.0.1"
                     },
+                    "resolved": false,
                     "version": "1.1.11"
                 },
                 "chownr": {
-                    "bundled": true,
                     "dev": true,
+                    "integrity": "sha512-i70fVHhmV3DtTl6nqvZOnIjbY0Pe4kAUjwHj8z0zAdgBtYrJyYwLKCCuRBQ5ppkyL0AkN7HKRnETdmdp1zqNXw==",
                     "optional": true,
+                    "resolved": false,
                     "version": "1.1.3"
                 },
                 "code-point-at": {
-                    "bundled": true,
                     "dev": true,
+                    "integrity": "sha1-DQcLTQQ6W+ozovGkDi7bPZpMz3c=",
                     "optional": true,
+                    "resolved": false,
                     "version": "1.1.0"
                 },
                 "concat-map": {
-                    "bundled": true,
                     "dev": true,
+                    "integrity": "sha1-2Klr13/Wjfd5OnMDajug1UBdR3s=",
                     "optional": true,
+                    "resolved": false,
                     "version": "0.0.1"
                 },
                 "console-control-strings": {
-                    "bundled": true,
                     "dev": true,
+                    "integrity": "sha1-PXz0Rk22RG6mRL9LOVB/mFEAjo4=",
                     "optional": true,
+                    "resolved": false,
                     "version": "1.1.0"
                 },
                 "core-util-is": {
-                    "bundled": true,
                     "dev": true,
+                    "integrity": "sha1-tf1UIgqivFq1eqtxQMlAdUUDwac=",
                     "optional": true,
+                    "resolved": false,
                     "version": "1.0.2"
                 },
                 "debug": {
-                    "bundled": true,
                     "dev": true,
+                    "integrity": "sha512-mel+jf7nrtEl5Pn1Qx46zARXKDpBbvzezse7p7LqINmdoIk8PYP5SySaxEmYv6TZ0JyEKA1hsCId6DIhgITtWQ==",
                     "optional": true,
                     "requires": {
                         "ms": "^2.1.1"
                     },
+                    "resolved": false,
                     "version": "3.2.6"
                 },
                 "deep-extend": {
-                    "bundled": true,
                     "dev": true,
+                    "integrity": "sha512-LOHxIOaPYdHlJRtCQfDIVZtfw/ufM8+rVj649RIHzcm/vGwQRXFt6OPqIFWsm2XEMrNIEtWR64sY1LEKD2vAOA==",
                     "optional": true,
+                    "resolved": false,
                     "version": "0.6.0"
                 },
                 "delegates": {
-                    "bundled": true,
                     "dev": true,
+                    "integrity": "sha1-hMbhWbgZBP3KWaDvRM2HDTElD5o=",
                     "optional": true,
+                    "resolved": false,
                     "version": "1.0.0"
                 },
                 "detect-libc": {
-                    "bundled": true,
                     "dev": true,
+                    "integrity": "sha1-+hN8S9aY7fVc1c0CrFWfkaTEups=",
                     "optional": true,
+                    "resolved": false,
                     "version": "1.0.3"
                 },
                 "fs-minipass": {
-                    "bundled": true,
                     "dev": true,
+                    "integrity": "sha512-GWSSJGFy4e9GUeCcbIkED+bgAoFyj7XF1mV8rma3QW4NIqX9Kyx79N/PF61H5udOV3aY1IaMLs6pGbH71nlCTA==",
                     "optional": true,
                     "requires": {
                         "minipass": "^2.6.0"
                     },
+                    "resolved": false,
                     "version": "1.2.7"
                 },
                 "fs.realpath": {
-                    "bundled": true,
                     "dev": true,
+                    "integrity": "sha1-FQStJSMVjKpA20onh8sBQRmU6k8=",
                     "optional": true,
+                    "resolved": false,
                     "version": "1.0.0"
                 },
                 "gauge": {
-                    "bundled": true,
                     "dev": true,
+                    "integrity": "sha1-LANAXHU4w51+s3sxcCLjJfsBi/c=",
                     "optional": true,
                     "requires": {
                         "aproba": "^1.0.3",
                         "console-control-strings": "^1.0.0",
                         "has-unicode": "^2.0.0",
                         "object-assign": "^4.1.0",
                         "signal-exit": "^3.0.0",
                         "string-width": "^1.0.1",
                         "strip-ansi": "^3.0.1",
                         "wide-align": "^1.1.0"
                     },
+                    "resolved": false,
                     "version": "2.7.4"
                 },
                 "glob": {
-                    "bundled": true,
                     "dev": true,
+                    "integrity": "sha512-LwaxwyZ72Lk7vZINtNNrywX0ZuLyStrdDtabefZKAY5ZGJhVtgdznluResxNmPitE0SAO+O26sWTHeKSI2wMBA==",
                     "optional": true,
                     "requires": {
                         "fs.realpath": "^1.0.0",
                         "inflight": "^1.0.4",
                         "inherits": "2",
                         "minimatch": "^3.0.4",
                         "once": "^1.3.0",
                         "path-is-absolute": "^1.0.0"
                     },
+                    "resolved": false,
                     "version": "7.1.6"
                 },
                 "has-unicode": {
-                    "bundled": true,
                     "dev": true,
+                    "integrity": "sha1-4Ob+aijPUROIVeCG0Wkedx3iqLk=",
                     "optional": true,
+                    "resolved": false,
                     "version": "2.0.1"
                 },
                 "iconv-lite": {
-                    "bundled": true,
                     "dev": true,
+                    "integrity": "sha512-v3MXnZAcvnywkTUEZomIActle7RXXeedOR31wwl7VlyoXO4Qi9arvSenNQWne1TcRwhCL1HwLI21bEqdpj8/rA==",
                     "optional": true,
                     "requires": {
                         "safer-buffer": ">= 2.1.2 < 3"
                     },
+                    "resolved": false,
                     "version": "0.4.24"
                 },
                 "ignore-walk": {
-                    "bundled": true,
                     "dev": true,
+                    "integrity": "sha512-m7o6xuOaT1aqheYHKf8W6J5pYH85ZI9w077erOzLje3JsB1gkafkAhHHY19dqjulgIZHFm32Cp5uNZgcQqdJKw==",
                     "optional": true,
                     "requires": {
                         "minimatch": "^3.0.4"
                     },
+                    "resolved": false,
                     "version": "3.0.3"
                 },
                 "inflight": {
-                    "bundled": true,
                     "dev": true,
+                    "integrity": "sha1-Sb1jMdfQLQwJvJEKEHW6gWW1bfk=",
                     "optional": true,
                     "requires": {
                         "once": "^1.3.0",
                         "wrappy": "1"
                     },
+                    "resolved": false,
                     "version": "1.0.6"
                 },
                 "inherits": {
-                    "bundled": true,
                     "dev": true,
+                    "integrity": "sha512-k/vGaX4/Yla3WzyMCvTQOXYeIHvqOKtnqBduzTHpzpQZzAskKMhZ2K+EnBiSM9zGSoIFeMpXKxa4dYeZIQqewQ==",
                     "optional": true,
+                    "resolved": false,
                     "version": "2.0.4"
                 },
                 "ini": {
-                    "bundled": true,
                     "dev": true,
+                    "integrity": "sha512-RZY5huIKCMRWDUqZlEi72f/lmXKMvuszcMBduliQ3nnWbx9X/ZBQO7DijMEYS9EhHBb2qacRUMtC7svLwe0lcw==",
                     "optional": true,
+                    "resolved": false,
                     "version": "1.3.5"
                 },
                 "is-fullwidth-code-point": {
-                    "bundled": true,
                     "dev": true,
+                    "integrity": "sha1-754xOG8DGn8NZDr4L95QxFfvAMs=",
                     "optional": true,
                     "requires": {
                         "number-is-nan": "^1.0.0"
                     },
+                    "resolved": false,
                     "version": "1.0.0"
                 },
                 "isarray": {
-                    "bundled": true,
                     "dev": true,
+                    "integrity": "sha1-u5NdSFgsuhaMBoNJV6VKPgcSTxE=",
                     "optional": true,
+                    "resolved": false,
                     "version": "1.0.0"
                 },
                 "minimatch": {
-                    "bundled": true,
                     "dev": true,
+                    "integrity": "sha512-yJHVQEhyqPLUTgt9B83PXu6W3rx4MvvHvSUvToogpwoGDOUQ+yDrR0HRot+yOCdCO7u4hX3pWft6kWBBcqh0UA==",
                     "optional": true,
                     "requires": {
                         "brace-expansion": "^1.1.7"
                     },
+                    "resolved": false,
                     "version": "3.0.4"
                 },
-                "minimist": {
-                    "bundled": true,
-                    "dev": true,
-                    "optional": true,
-                    "version": "0.0.8"
-                },
                 "minipass": {
-                    "bundled": true,
                     "dev": true,
+                    "integrity": "sha512-wxfUjg9WebH+CUDX/CdbRlh5SmfZiy/hpkxaRI16Y9W56Pa75sWgd/rvFilSgrauD9NyFymP/+JFV3KwzIsJeg==",
                     "optional": true,
                     "requires": {
                         "safe-buffer": "^5.1.2",
                         "yallist": "^3.0.0"
                     },
+                    "resolved": false,
                     "version": "2.9.0"
                 },
                 "minizlib": {
-                    "bundled": true,
                     "dev": true,
+                    "integrity": "sha512-6ZYMOEnmVsdCeTJVE0W9ZD+pVnE8h9Hma/iOwwRDsdQoePpoX56/8B6z3P9VNwppJuBKNRuFDRNRqRWexT9G9Q==",
                     "optional": true,
                     "requires": {
                         "minipass": "^2.9.0"
                     },
+                    "resolved": false,
                     "version": "1.3.3"
                 },
                 "mkdirp": {
-                    "bundled": true,
                     "dev": true,
+                    "integrity": "sha512-NKmAlESf6jMGym1++R0Ra7wvhV+wFW63FaSOFPwRahvea0gMUcGUhVeAg/0BC0wiv9ih5NYPB1Wn1UEI1/L+xQ==",
                     "optional": true,
                     "requires": {
-                        "minimist": "0.0.8"
+                        "minimist": "^1.2.5"
                     },
-                    "version": "0.5.1"
+                    "resolved": "https://registry.npmjs.org/mkdirp/-/mkdirp-0.5.5.tgz",
+                    "version": "0.5.5"
                 },
                 "ms": {
-                    "bundled": true,
                     "dev": true,
+                    "integrity": "sha512-sGkPx+VjMtmA6MX27oA4FBFELFCZZ4S4XqeGOXCv68tT+jb3vk/RyaKWP0PTKyWtmLSM0b+adUTEvbs1PEaH2w==",
                     "optional": true,
+                    "resolved": false,
                     "version": "2.1.2"
                 },
                 "needle": {
-                    "bundled": true,
                     "dev": true,
+                    "integrity": "sha512-4Hnwzr3mi5L97hMYeNl8wRW/Onhy4nUKR/lVemJ8gJedxxUyBLm9kkrDColJvoSfwi0jCNhD+xCdOtiGDQiRZg==",
                     "optional": true,
                     "requires": {
                         "debug": "^3.2.6",
                         "iconv-lite": "^0.4.4",
                         "sax": "^1.2.4"
                     },
+                    "resolved": false,
                     "version": "2.4.0"
                 },
                 "node-pre-gyp": {
-                    "bundled": true,
                     "dev": true,
+                    "integrity": "sha512-+CvDC7ZttU/sSt9rFjix/P05iS43qHCOOGzcr3Ry99bXG7VX953+vFyEuph/tfqoYu8dttBkE86JSKBO2OzcxA==",
                     "optional": true,
                     "requires": {
                         "detect-libc": "^1.0.2",
                         "mkdirp": "^0.5.1",
                         "needle": "^2.2.1",
                         "nopt": "^4.0.1",
                         "npm-packlist": "^1.1.6",
                         "npmlog": "^4.0.2",
                         "rc": "^1.2.7",
                         "rimraf": "^2.6.1",
                         "semver": "^5.3.0",
                         "tar": "^4.4.2"
                     },
+                    "resolved": false,
                     "version": "0.14.0"
                 },
                 "nopt": {
-                    "bundled": true,
                     "dev": true,
+                    "integrity": "sha1-0NRoWv1UFRk8jHUFYC0NF81kR00=",
                     "optional": true,
                     "requires": {
                         "abbrev": "1",
                         "osenv": "^0.1.4"
                     },
+                    "resolved": false,
                     "version": "4.0.1"
                 },
                 "npm-bundled": {
-                    "bundled": true,
                     "dev": true,
+                    "integrity": "sha512-gqkfgGePhTpAEgUsGEgcq1rqPXA+tv/aVBlgEzfXwA1yiUJF7xtEt3CtVwOjNYQOVknDk0F20w58Fnm3EtG0fA==",
                     "optional": true,
                     "requires": {
                         "npm-normalize-package-bin": "^1.0.1"
                     },
+                    "resolved": false,
                     "version": "1.1.1"
                 },
                 "npm-normalize-package-bin": {
-                    "bundled": true,
                     "dev": true,
+                    "integrity": "sha512-EPfafl6JL5/rU+ot6P3gRSCpPDW5VmIzX959Ob1+ySFUuuYHWHekXpwdUZcKP5C+DS4GEtdJluwBjnsNDl+fSA==",
                     "optional": true,
+                    "resolved": false,
                     "version": "1.0.1"
                 },
                 "npm-packlist": {
-                    "bundled": true,
                     "dev": true,
+                    "integrity": "sha512-vAj7dIkp5NhieaGZxBJB8fF4R0078rqsmhJcAfXZ6O7JJhjhPK96n5Ry1oZcfLXgfun0GWTZPOxaEyqv8GBykQ==",
                     "optional": true,
                     "requires": {
                         "ignore-walk": "^3.0.1",
                         "npm-bundled": "^1.0.1"
                     },
+                    "resolved": false,
                     "version": "1.4.7"
                 },
                 "npmlog": {
-                    "bundled": true,
                     "dev": true,
+                    "integrity": "sha512-2uUqazuKlTaSI/dC8AzicUck7+IrEaOnN/e0jd3Xtt1KcGpwx30v50mL7oPyr/h9bL3E4aZccVwpwP+5W9Vjkg==",
                     "optional": true,
                     "requires": {
                         "are-we-there-yet": "~1.1.2",
                         "console-control-strings": "~1.1.0",
                         "gauge": "~2.7.3",
                         "set-blocking": "~2.0.0"
                     },
+                    "resolved": false,
                     "version": "4.1.2"
                 },
                 "number-is-nan": {
-                    "bundled": true,
                     "dev": true,
+                    "integrity": "sha1-CXtgK1NCKlIsGvuHkDGDNpQaAR0=",
                     "optional": true,
+                    "resolved": false,
                     "version": "1.0.1"
                 },
                 "object-assign": {
-                    "bundled": true,
                     "dev": true,
+                    "integrity": "sha1-IQmtx5ZYh8/AXLvUQsrIv7s2CGM=",
                     "optional": true,
+                    "resolved": false,
                     "version": "4.1.1"
                 },
                 "once": {
-                    "bundled": true,
                     "dev": true,
+                    "integrity": "sha1-WDsap3WWHUsROsF9nFC6753Xa9E=",
                     "optional": true,
                     "requires": {
                         "wrappy": "1"
                     },
+                    "resolved": false,
                     "version": "1.4.0"
                 },
                 "os-homedir": {
-                    "bundled": true,
                     "dev": true,
+                    "integrity": "sha1-/7xJiDNuDoM94MFox+8VISGqf7M=",
                     "optional": true,
+                    "resolved": false,
                     "version": "1.0.2"
                 },
                 "os-tmpdir": {
-                    "bundled": true,
                     "dev": true,
+                    "integrity": "sha1-u+Z0BseaqFxc/sdm/lc0VV36EnQ=",
                     "optional": true,
+                    "resolved": false,
                     "version": "1.0.2"
                 },
                 "osenv": {
-                    "bundled": true,
                     "dev": true,
+                    "integrity": "sha512-0CWcCECdMVc2Rw3U5w9ZjqX6ga6ubk1xDVKxtBQPK7wis/0F2r9T6k4ydGYhecl7YUBxBVxhL5oisPsNxAPe2g==",
                     "optional": true,
                     "requires": {
                         "os-homedir": "^1.0.0",
                         "os-tmpdir": "^1.0.0"
                     },
+                    "resolved": false,
                     "version": "0.1.5"
                 },
                 "path-is-absolute": {
-                    "bundled": true,
                     "dev": true,
+                    "integrity": "sha1-F0uSaHNVNP+8es5r9TpanhtcX18=",
                     "optional": true,
+                    "resolved": false,
                     "version": "1.0.1"
                 },
                 "process-nextick-args": {
-                    "bundled": true,
                     "dev": true,
+                    "integrity": "sha512-3ouUOpQhtgrbOa17J7+uxOTpITYWaGP7/AhoR3+A+/1e9skrzelGi/dXzEYyvbxubEF6Wn2ypscTKiKJFFn1ag==",
                     "optional": true,
+                    "resolved": false,
                     "version": "2.0.1"
                 },
                 "rc": {
-                    "bundled": true,
                     "dependencies": {
                         "minimist": {
-                            "bundled": true,
                             "dev": true,
+                            "integrity": "sha512-FM9nNUYrRBAELZQT3xeZQ7fmMOBg6nWNmJKTcgsJeaLstP/UODVpGsr5OhXhhXg6f+qtJ8uiZ+PUxkDWcgIXLw==",
                             "optional": true,
-                            "version": "1.2.0"
+                            "resolved": "https://registry.npmjs.org/minimist/-/minimist-1.2.5.tgz",
+                            "version": "1.2.5"
                         }
                     },
                     "dev": true,
+                    "integrity": "sha512-y3bGgqKj3QBdxLbLkomlohkvsA8gdAiUQlSBJnBhfn+BPxg4bc62d8TcBW15wavDfgexCgccckhcZvywyQYPOw==",
                     "optional": true,
                     "requires": {
                         "deep-extend": "^0.6.0",
                         "ini": "~1.3.0",
                         "minimist": "^1.2.0",
                         "strip-json-comments": "~2.0.1"
                     },
+                    "resolved": false,
                     "version": "1.2.8"
                 },
                 "readable-stream": {
-                    "bundled": true,
                     "dev": true,
+                    "integrity": "sha512-tQtKA9WIAhBF3+VLAseyMqZeBjW0AHJoxOtYqSUZNJxauErmLbVm2FW1y+J/YA9dUrAC39ITejlZWhVIwawkKw==",
                     "optional": true,
                     "requires": {
                         "core-util-is": "~1.0.0",
                         "inherits": "~2.0.3",
                         "isarray": "~1.0.0",
                         "process-nextick-args": "~2.0.0",
                         "safe-buffer": "~5.1.1",
                         "string_decoder": "~1.1.1",
                         "util-deprecate": "~1.0.1"
                     },
+                    "resolved": false,
                     "version": "2.3.6"
                 },
                 "rimraf": {
-                    "bundled": true,
                     "dev": true,
+                    "integrity": "sha512-uWjbaKIK3T1OSVptzX7Nl6PvQ3qAGtKEtVRjRuazjfL3Bx5eI409VZSqgND+4UNnmzLVdPj9FqFJNPqBZFve4w==",
                     "optional": true,
                     "requires": {
                         "glob": "^7.1.3"
                     },
+                    "resolved": false,
                     "version": "2.7.1"
                 },
                 "safe-buffer": {
-                    "bundled": true,
                     "dev": true,
+                    "integrity": "sha512-Gd2UZBJDkXlY7GbJxfsE8/nvKkUEU1G38c1siN6QP6a9PT9MmHB8GnpscSmMJSoF8LOIrt8ud/wPtojys4G6+g==",
                     "optional": true,
+                    "resolved": false,
                     "version": "5.1.2"
                 },
                 "safer-buffer": {
-                    "bundled": true,
                     "dev": true,
+                    "integrity": "sha512-YZo3K82SD7Riyi0E1EQPojLz7kpepnSQI9IyPbHHg1XXXevb5dJI7tpyN2ADxGcQbHG7vcyRHk0cbwqcQriUtg==",
                     "optional": true,
+                    "resolved": false,
                     "version": "2.1.2"
                 },
                 "sax": {
-                    "bundled": true,
                     "dev": true,
+                    "integrity": "sha512-NqVDv9TpANUjFm0N8uM5GxL36UgKi9/atZw+x7YFnQ8ckwFGKrl4xX4yWtrey3UJm5nP1kUbnYgLopqWNSRhWw==",
                     "optional": true,
+                    "resolved": false,
                     "version": "1.2.4"
                 },
                 "semver": {
-                    "bundled": true,
                     "dev": true,
+                    "integrity": "sha512-sauaDf/PZdVgrLTNYHRtpXa1iRiKcaebiKQ1BJdpQlWH2lCvexQdX55snPFyK7QzpudqbCI0qXFfOasHdyNDGQ==",
                     "optional": true,
+                    "resolved": false,
                     "version": "5.7.1"
                 },
                 "set-blocking": {
-                    "bundled": true,
                     "dev": true,
+                    "integrity": "sha1-BF+XgtARrppoA93TgrJDkrPYkPc=",
                     "optional": true,
+                    "resolved": false,
                     "version": "2.0.0"
                 },
                 "signal-exit": {
-                    "bundled": true,
                     "dev": true,
+                    "integrity": "sha1-tf3AjxKH6hF4Yo5BXiUTK3NkbG0=",
                     "optional": true,
+                    "resolved": false,
                     "version": "3.0.2"
                 },
                 "string-width": {
-                    "bundled": true,
                     "dev": true,
+                    "integrity": "sha1-EYvfW4zcUaKn5w0hHgfisLmxB9M=",
                     "optional": true,
                     "requires": {
                         "code-point-at": "^1.0.0",
                         "is-fullwidth-code-point": "^1.0.0",
                         "strip-ansi": "^3.0.0"
                     },
+                    "resolved": false,
                     "version": "1.0.2"
                 },
                 "string_decoder": {
-                    "bundled": true,
                     "dev": true,
+                    "integrity": "sha512-n/ShnvDi6FHbbVfviro+WojiFzv+s8MPMHBczVePfUpDJLwoLT0ht1l4YwBCbi8pJAveEEdnkHyPyTP/mzRfwg==",
                     "optional": true,
                     "requires": {
                         "safe-buffer": "~5.1.0"
                     },
+                    "resolved": false,
                     "version": "1.1.1"
                 },
                 "strip-ansi": {
-                    "bundled": true,
                     "dev": true,
+                    "integrity": "sha1-ajhfuIU9lS1f8F0Oiq+UJ43GPc8=",
                     "optional": true,
                     "requires": {
                         "ansi-regex": "^2.0.0"
                     },
+                    "resolved": false,
                     "version": "3.0.1"
                 },
                 "strip-json-comments": {
-                    "bundled": true,
                     "dev": true,
+                    "integrity": "sha1-PFMZQukIwml8DsNEhYwobHygpgo=",
                     "optional": true,
+                    "resolved": false,
                     "version": "2.0.1"
                 },
                 "tar": {
-                    "bundled": true,
                     "dev": true,
+                    "integrity": "sha512-w2VwSrBoHa5BsSyH+KxEqeQBAllHhccyMFVHtGtdMpF4W7IRWfZjFiQceJPChOeTsSDVUpER2T8FA93pr0L+QA==",
                     "optional": true,
                     "requires": {
                         "chownr": "^1.1.1",
                         "fs-minipass": "^1.2.5",
                         "minipass": "^2.8.6",
                         "minizlib": "^1.2.1",
                         "mkdirp": "^0.5.0",
                         "safe-buffer": "^5.1.2",
                         "yallist": "^3.0.3"
                     },
+                    "resolved": false,
                     "version": "4.4.13"
                 },
                 "util-deprecate": {
-                    "bundled": true,
                     "dev": true,
+                    "integrity": "sha1-RQ1Nyfpw3nMnYvvS1KKJgUGaDM8=",
                     "optional": true,
+                    "resolved": false,
                     "version": "1.0.2"
                 },
                 "wide-align": {
-                    "bundled": true,
                     "dev": true,
+                    "integrity": "sha512-QGkOQc8XL6Bt5PwnsExKBPuMKBxnGxWWW3fU55Xt4feHozMUhdUMaBCk290qpm/wG5u/RSKzwdAC4i51YigihA==",
                     "optional": true,
                     "requires": {
                         "string-width": "^1.0.2 || 2"
                     },
+                    "resolved": false,
                     "version": "1.1.3"
                 },
                 "wrappy": {
-                    "bundled": true,
                     "dev": true,
+                    "integrity": "sha1-tSQ9jz7BqjXxNkYFvA0QNuMKtp8=",
                     "optional": true,
+                    "resolved": false,
                     "version": "1.0.2"
                 },
                 "yallist": {
-                    "bundled": true,
                     "dev": true,
+                    "integrity": "sha512-a4UGQaWPH59mOXUYnAG2ewncQS4i4F43Tv3JoAM+s2VDAmS9NsK8GpDMLrCHPksFT7h3K6TOoUNn2pb7RoXx4g==",
                     "optional": true,
+                    "resolved": false,
                     "version": "3.1.1"
                 }
             },
             "dev": true,
             "integrity": "sha512-+ux3lx6peh0BpvY0JebGyZoiR4D+oYzdPZMKJwkZ+sFkNJzpL7tXc/wehS49gUAxg3tmMHPHZkA8JU2rhhgDHw==",
             "optional": true,
             "requires": {
                 "bindings": "^1.5.0",
                 "nan": "^2.12.1",
                 "node-pre-gyp": "*"
             },
             "resolved": "https://registry.npmjs.org/fsevents/-/fsevents-1.2.11.tgz",
             "version": "1.2.11"
         },
-        "fstream": {
-            "dev": true,
-            "integrity": "sha512-WvJ193OHa0GHPEL+AycEJgxvBEwyfRkN1vhjca23OaPVMCaLCXTd5qAu82AjTcgP1UJmytkOKb63Ypde7raDIg==",
-            "requires": {
-                "graceful-fs": "^4.1.2",
-                "inherits": "~2.0.0",
-                "mkdirp": ">=0.5 0",
-                "rimraf": "2"
-            },
-            "resolved": "https://registry.npmjs.org/fstream/-/fstream-1.0.12.tgz",
-            "version": "1.0.12"
-        },
         "function-bind": {
             "dev": true,
             "integrity": "sha512-yIovAzMX49sF8Yl58fSCWJ5svSLuaibPxXQJFLmBObTuCr0Mf1KiPopGM9NiFjiYBCbfaa2Fh6breQ6ANVTI0A==",
             "resolved": "https://registry.npmjs.org/function-bind/-/function-bind-1.1.1.tgz",
             "version": "1.1.1"
         },
-        "gauge": {
-            "dependencies": {
-                "ansi-regex": {
-                    "dev": true,
-                    "integrity": "sha1-w7M6te42DYbg5ijwRorn7yfWVN8=",
-                    "resolved": "https://registry.npmjs.org/ansi-regex/-/ansi-regex-2.1.1.tgz",
-                    "version": "2.1.1"
-                },
-                "is-fullwidth-code-point": {
-                    "dev": true,
-                    "integrity": "sha1-754xOG8DGn8NZDr4L95QxFfvAMs=",
-                    "requires": {
-                        "number-is-nan": "^1.0.0"
-                    },
-                    "resolved": "https://registry.npmjs.org/is-fullwidth-code-point/-/is-fullwidth-code-point-1.0.0.tgz",
-                    "version": "1.0.0"
-                },
-                "string-width": {
-                    "dev": true,
-                    "integrity": "sha1-EYvfW4zcUaKn5w0hHgfisLmxB9M=",
-                    "requires": {
-                        "code-point-at": "^1.0.0",
-                        "is-fullwidth-code-point": "^1.0.0",
-                        "strip-ansi": "^3.0.0"
-                    },
-                    "resolved": "https://registry.npmjs.org/string-width/-/string-width-1.0.2.tgz",
-                    "version": "1.0.2"
-                },
-                "strip-ansi": {
-                    "dev": true,
-                    "integrity": "sha1-ajhfuIU9lS1f8F0Oiq+UJ43GPc8=",
-                    "requires": {
-                        "ansi-regex": "^2.0.0"
-                    },
-                    "resolved": "https://registry.npmjs.org/strip-ansi/-/strip-ansi-3.0.1.tgz",
-                    "version": "3.0.1"
-                }
-            },
-            "dev": true,
-            "integrity": "sha1-LANAXHU4w51+s3sxcCLjJfsBi/c=",
-            "requires": {
-                "aproba": "^1.0.3",
-                "console-control-strings": "^1.0.0",
-                "has-unicode": "^2.0.0",
-                "object-assign": "^4.1.0",
-                "signal-exit": "^3.0.0",
-                "string-width": "^1.0.1",
-                "strip-ansi": "^3.0.1",
-                "wide-align": "^1.1.0"
-            },
-            "resolved": "https://registry.npmjs.org/gauge/-/gauge-2.7.4.tgz",
-            "version": "2.7.4"
-        },
-        "gaze": {
-            "dev": true,
-            "integrity": "sha512-BRdNm8hbWzFzWHERTrejLqwHDfS4GibPoq5wjTPIoJHoBtKGPg3xAFfxmM+9ztbXelxcf2hwQcaz1PtmFeue8g==",
-            "requires": {
-                "globule": "^1.0.0"
-            },
-            "resolved": "https://registry.npmjs.org/gaze/-/gaze-1.1.3.tgz",
-            "version": "1.1.3"
-        },
-        "get-caller-file": {
+        "gensync": {
             "dev": true,
-            "integrity": "sha512-3t6rVToeoZfYSGd8YoLFR2DJkiQrIiUrGcjvFX2mDw3bn6k2OtwHN0TNCLbBO+w8qTvimhDkv+LSscbJY1vE6w==",
-            "resolved": "https://registry.npmjs.org/get-caller-file/-/get-caller-file-1.0.3.tgz",
-            "version": "1.0.3"
+            "integrity": "sha512-r8EC6NO1sngH/zdD9fiRDLdcgnbayXah+mLgManTaIZJqEC1MZstmnox8KpnI2/fxQwrp5OpCOYWLp4rBl4Jcg==",
+            "resolved": "https://registry.npmjs.org/gensync/-/gensync-1.0.0-beta.1.tgz",
+            "version": "1.0.0-beta.1"
         },
         "get-port": {
             "dev": true,
             "integrity": "sha1-3Xzn3hh8Bsi/NTeWrHHgmfCYDrw=",
             "resolved": "https://registry.npmjs.org/get-port/-/get-port-3.2.0.tgz",
             "version": "3.2.0"
         },
-        "get-stdin": {
-            "dev": true,
-            "integrity": "sha1-uWjGsKBDhDJJAui/Gl3zJXmkUP4=",
-            "resolved": "https://registry.npmjs.org/get-stdin/-/get-stdin-4.0.1.tgz",
-            "version": "4.0.1"
-        },
         "get-value": {
             "dev": true,
             "integrity": "sha1-3BXKHGcjh8p2vTesCjlbogQqLCg=",
             "resolved": "https://registry.npmjs.org/get-value/-/get-value-2.0.6.tgz",
             "version": "2.0.6"
         },
         "getpass": {
@@ -3996,25 +4072,14 @@
         },
         "globals": {
             "dev": true,
             "integrity": "sha512-WOBp/EEGUiIsJSp7wcv/y6MO+lV9UoncWqxuFfm8eBwzWNgyfBd6Gz+IeKQ9jCmyhoH99g15M3T+QaVHFjizVA==",
             "resolved": "https://registry.npmjs.org/globals/-/globals-11.12.0.tgz",
             "version": "11.12.0"
         },
-        "globule": {
-            "dev": true,
-            "integrity": "sha512-g7QtgWF4uYSL5/dn71WxubOrS7JVGCnFPEnoeChJmBnyR9Mw8nGoEwOgJL/RC2Te0WhbsEUCejfH8SZNJ+adYQ==",
-            "requires": {
-                "glob": "~7.1.1",
-                "lodash": "~4.17.10",
-                "minimatch": "~3.0.2"
-            },
-            "resolved": "https://registry.npmjs.org/globule/-/globule-1.2.1.tgz",
-            "version": "1.2.1"
-        },
         "graceful-fs": {
             "dev": true,
             "integrity": "sha512-a30VEBm4PEdx1dRB7MFK7BejejvCvBronbLjht+sHuGYj8PHs7M/5Z+rt5lw551vZ7yfTCj4Vuyy3mSJytDWRQ==",
             "resolved": "https://registry.npmjs.org/graceful-fs/-/graceful-fs-4.2.3.tgz",
             "version": "4.2.3"
         },
         "grapheme-breaker": {
@@ -4077,20 +4142,14 @@
         },
         "has-symbols": {
             "dev": true,
             "integrity": "sha512-PLcsoqu++dmEIZB+6totNFKq/7Do+Z0u4oT0zKOJNl3lYK6vGwwu2hjHs+68OEZbTjiUE9bgOABXbP/GvrS0Kg==",
             "resolved": "https://registry.npmjs.org/has-symbols/-/has-symbols-1.0.1.tgz",
             "version": "1.0.1"
         },
-        "has-unicode": {
-            "dev": true,
-            "integrity": "sha1-4Ob+aijPUROIVeCG0Wkedx3iqLk=",
-            "resolved": "https://registry.npmjs.org/has-unicode/-/has-unicode-2.0.1.tgz",
-            "version": "2.0.1"
-        },
         "has-value": {
             "dev": true,
             "integrity": "sha1-GLKB2lhbHFxR3vJMkw7SmgvmsXc=",
             "requires": {
                 "get-value": "^2.0.6",
                 "has-values": "^1.0.0",
                 "isobject": "^3.0.0"
@@ -4158,20 +4217,14 @@
                 "hash.js": "^1.0.3",
                 "minimalistic-assert": "^1.0.0",
                 "minimalistic-crypto-utils": "^1.0.1"
             },
             "resolved": "https://registry.npmjs.org/hmac-drbg/-/hmac-drbg-1.0.1.tgz",
             "version": "1.0.1"
         },
-        "hosted-git-info": {
-            "dev": true,
-            "integrity": "sha512-kssjab8CvdXfcXMXVcvsXum4Hwdq9XGtRD3TteMEvEbq0LXyiNQr6AprqKqfeaDXze7SxWvRxdpwE6ku7ikLkg==",
-            "resolved": "https://registry.npmjs.org/hosted-git-info/-/hosted-git-info-2.8.5.tgz",
-            "version": "2.8.5"
-        },
         "hsl-regex": {
             "dev": true,
             "integrity": "sha1-1JMwx4ntgZ4nakwNJy3/owsY/m4=",
             "resolved": "https://registry.npmjs.org/hsl-regex/-/hsl-regex-1.0.0.tgz",
             "version": "1.0.0"
         },
         "hsla-regex": {
@@ -4315,14 +4368,15 @@
         "https-browserify": {
             "dev": true,
             "integrity": "sha1-7AbBDgo0wPL68Zn3/X/Hj//QPHM=",
             "resolved": "https://registry.npmjs.org/https-browserify/-/https-browserify-1.0.0.tgz",
             "version": "1.0.0"
         },
         "iconv-lite": {
+            "dev": true,
             "integrity": "sha512-v3MXnZAcvnywkTUEZomIActle7RXXeedOR31wwl7VlyoXO4Qi9arvSenNQWne1TcRwhCL1HwLI21bEqdpj8/rA==",
             "requires": {
                 "safer-buffer": ">= 2.1.2 < 3"
             },
             "resolved": "https://registry.npmjs.org/iconv-lite/-/iconv-lite-0.4.24.tgz",
             "version": "0.4.24"
         },
@@ -4334,19 +4388,14 @@
         },
         "ieee754": {
             "dev": true,
             "integrity": "sha512-4vf7I2LYV/HaWerSo3XmlMkp5eZ83i+/CDluXi/IGTs/O1sejBNhTtnxzmRZfvOUqj7lZjqHkeTvpgSFDlWZTg==",
             "resolved": "https://registry.npmjs.org/ieee754/-/ieee754-1.1.13.tgz",
             "version": "1.1.13"
         },
-        "immutable": {
-            "integrity": "sha1-E7TTyxK++hVIKib+Gy665kAHHks=",
-            "resolved": "https://registry.npmjs.org/immutable/-/immutable-3.7.6.tgz",
-            "version": "3.7.6"
-        },
         "import-fresh": {
             "dependencies": {
                 "resolve-from": {
                     "dev": true,
                     "integrity": "sha1-six699nWiBvItuZTM17rywoYh0g=",
                     "resolved": "https://registry.npmjs.org/resolve-from/-/resolve-from-3.0.0.tgz",
                     "version": "3.0.0"
@@ -4357,20 +4406,14 @@
             "requires": {
                 "caller-path": "^2.0.0",
                 "resolve-from": "^3.0.0"
             },
             "resolved": "https://registry.npmjs.org/import-fresh/-/import-fresh-2.0.0.tgz",
             "version": "2.0.0"
         },
-        "in-publish": {
-            "dev": true,
-            "integrity": "sha1-4g/146KvwmkDILbcVSaCqcf631E=",
-            "resolved": "https://registry.npmjs.org/in-publish/-/in-publish-2.0.0.tgz",
-            "version": "2.0.0"
-        },
         "indexes-of": {
             "dev": true,
             "integrity": "sha1-8w9xbI4r00bHtn0985FVZqfAVgc=",
             "resolved": "https://registry.npmjs.org/indexes-of/-/indexes-of-1.0.1.tgz",
             "version": "1.0.1"
         },
         "inflight": {
@@ -4394,20 +4437,14 @@
             "integrity": "sha512-phJfQVBuaJM5raOpJjSfkiD6BpbCE4Ns//LaXl6wGYtUBY83nWS6Rf9tXm2e8VaK60JEjYldbPif/A2B1C2gNA==",
             "requires": {
                 "loose-envify": "^1.0.0"
             },
             "resolved": "https://registry.npmjs.org/invariant/-/invariant-2.2.4.tgz",
             "version": "2.2.4"
         },
-        "invert-kv": {
-            "dev": true,
-            "integrity": "sha1-EEqOSqym09jNFXqO+L+rLXo//bY=",
-            "resolved": "https://registry.npmjs.org/invert-kv/-/invert-kv-1.0.0.tgz",
-            "version": "1.0.0"
-        },
         "is-absolute-url": {
             "dev": true,
             "integrity": "sha1-UFMN+4T8yap9vnhS6Do3uTufKqY=",
             "resolved": "https://registry.npmjs.org/is-absolute-url/-/is-absolute-url-2.1.0.tgz",
             "version": "2.1.0"
         },
         "is-accessor-descriptor": {
@@ -4536,23 +4573,14 @@
         },
         "is-extglob": {
             "dev": true,
             "integrity": "sha1-qIwCU1eR8C7TfHahueqXc8gz+MI=",
             "resolved": "https://registry.npmjs.org/is-extglob/-/is-extglob-2.1.1.tgz",
             "version": "2.1.1"
         },
-        "is-finite": {
-            "dev": true,
-            "integrity": "sha1-zGZ3aVYCvlUO8R6LSqYwU0K20Ko=",
-            "requires": {
-                "number-is-nan": "^1.0.0"
-            },
-            "resolved": "https://registry.npmjs.org/is-finite/-/is-finite-1.0.2.tgz",
-            "version": "1.0.2"
-        },
         "is-glob": {
             "dev": true,
             "integrity": "sha512-5G0tKtBTFImOqDnLB2hG6Bp2qcKEFduo4tZu9MT/H6NQv/ghhy30o55ufafxJ/LdH79LLs2Kfrn85TLKyA7BUg==",
             "requires": {
                 "is-extglob": "^2.1.1"
             },
             "resolved": "https://registry.npmjs.org/is-glob/-/is-glob-4.0.1.tgz",
@@ -4589,20 +4617,14 @@
             "integrity": "sha1-JP1iAaR4LPUFYcgQJ2r8fRLXEZU=",
             "requires": {
                 "kind-of": "^3.0.2"
             },
             "resolved": "https://registry.npmjs.org/is-number/-/is-number-3.0.0.tgz",
             "version": "3.0.0"
         },
-        "is-obj": {
-            "dev": true,
-            "integrity": "sha1-PkcprB9f3gJc19g6iW2rn09n2w8=",
-            "resolved": "https://registry.npmjs.org/is-obj/-/is-obj-1.0.1.tgz",
-            "version": "1.0.1"
-        },
         "is-plain-object": {
             "dev": true,
             "integrity": "sha512-h5PpgXkWitc38BBMYawTYMWJHFZJVnBquFE57xFpjB8pJFiF6gZ+bU+WyI/yqXiFR5mdLsgYNaPe8uao6Uv9Og==",
             "requires": {
                 "isobject": "^3.0.1"
             },
             "resolved": "https://registry.npmjs.org/is-plain-object/-/is-plain-object-2.0.4.tgz",
@@ -4619,19 +4641,14 @@
         },
         "is-resolvable": {
             "dev": true,
             "integrity": "sha512-qgDYXFSR5WvEfuS5dMj6oTMEbrrSaM0CrFk2Yiq/gXnBvD9pMa2jGXxyhGLfvhZpuMZe18CJpFxAt3CRs42NMg==",
             "resolved": "https://registry.npmjs.org/is-resolvable/-/is-resolvable-1.1.0.tgz",
             "version": "1.1.0"
         },
-        "is-stream": {
-            "integrity": "sha1-EtSj3U5o4Lec6428hBc66A2RykQ=",
-            "resolved": "https://registry.npmjs.org/is-stream/-/is-stream-1.1.0.tgz",
-            "version": "1.1.0"
-        },
         "is-svg": {
             "dev": true,
             "integrity": "sha512-gi4iHK53LR2ujhLVVj+37Ykh9GLqYHX6JOVXbLAucaG/Cqw9xwdFOjDM2qeifLs1sF1npXXFvDu0r5HNgCMrzQ==",
             "requires": {
                 "html-comment-regex": "^1.1.0"
             },
             "resolved": "https://registry.npmjs.org/is-svg/-/is-svg-3.0.0.tgz",
@@ -4654,20 +4671,14 @@
         },
         "is-url": {
             "dev": true,
             "integrity": "sha512-ITvGim8FhRiYe4IQ5uHSkj7pVaPDrCTkNd3yq3cV7iZAcJdHTUMPMEHcqSOy9xZ9qFenQCvi+2wjH9a1nXqHww==",
             "resolved": "https://registry.npmjs.org/is-url/-/is-url-1.2.4.tgz",
             "version": "1.2.4"
         },
-        "is-utf8": {
-            "dev": true,
-            "integrity": "sha1-Sw2hRCEE0bM2NA6AeX6GXPOffXI=",
-            "resolved": "https://registry.npmjs.org/is-utf8/-/is-utf8-0.2.1.tgz",
-            "version": "0.2.1"
-        },
         "is-windows": {
             "dev": true,
             "integrity": "sha512-eXK1UInq2bPmjyX6e3VHIzMLobc4J94i4AWn+Hpq3OU5KkrRC96OAcR3PRJ/pGu6m8TRnBHP9dkXQVsT/COVIA==",
             "resolved": "https://registry.npmjs.org/is-windows/-/is-windows-1.0.2.tgz",
             "version": "1.0.2"
         },
         "is-wsl": {
@@ -4690,42 +4701,28 @@
         },
         "isobject": {
             "dev": true,
             "integrity": "sha1-TkMekrEalzFjaqH5yNHMvP2reN8=",
             "resolved": "https://registry.npmjs.org/isobject/-/isobject-3.0.1.tgz",
             "version": "3.0.1"
         },
-        "isomorphic-fetch": {
-            "integrity": "sha1-YRrhrPFPXoH3KVB0coGf6XM1WKk=",
-            "requires": {
-                "node-fetch": "^1.0.1",
-                "whatwg-fetch": ">=0.10.0"
-            },
-            "resolved": "https://registry.npmjs.org/isomorphic-fetch/-/isomorphic-fetch-2.2.1.tgz",
-            "version": "2.2.1"
-        },
         "isstream": {
             "dev": true,
             "integrity": "sha1-R+Y/evVa+m+S4VAOaQ64uFKcCZo=",
             "resolved": "https://registry.npmjs.org/isstream/-/isstream-0.1.2.tgz",
             "version": "0.1.2"
         },
-        "js-base64": {
-            "dev": true,
-            "integrity": "sha512-M7kLczedRMYX4L8Mdh4MzyAMM9O5osx+4FcOQuTvr3A9F2D9S5JXheN0ewNbrvK2UatkTRhL5ejGmGSjNMiZuw==",
-            "resolved": "https://registry.npmjs.org/js-base64/-/js-base64-2.5.1.tgz",
-            "version": "2.5.1"
-        },
         "js-levenshtein": {
             "dev": true,
             "integrity": "sha512-X2BB11YZtrRqY4EnQcLX5Rh373zbK4alC1FW7D7MBhL2gtcC17cTnr6DmfHZeS0s2rTHjUTMMHfG7gO8SSdw+g==",
             "resolved": "https://registry.npmjs.org/js-levenshtein/-/js-levenshtein-1.1.6.tgz",
             "version": "1.1.6"
         },
         "js-tokens": {
+            "dev": true,
             "integrity": "sha512-RdJUflcE3cUzKiMqQgsCu06FPu9UdIJO0beYbPhHN4k6apgJtifcoCtT9bcxOpYBtpD2kCM6Sbzg4CausW/PKQ==",
             "resolved": "https://registry.npmjs.org/js-tokens/-/js-tokens-4.0.0.tgz",
             "version": "4.0.0"
         },
         "js-yaml": {
             "dev": true,
             "integrity": "sha512-YfbcO7jXDdyj0DGxYVSlSeQNHbD7XPWvrVWeVUujrQEoZzWJIRrCPoyk6kL6IAjAG2IolMK4T0hNUe0HOUs5Jw==",
@@ -4862,21 +4859,29 @@
         "json-stringify-safe": {
             "dev": true,
             "integrity": "sha1-Epai1Y/UXxmg9s4B1lcB4sc1tus=",
             "resolved": "https://registry.npmjs.org/json-stringify-safe/-/json-stringify-safe-5.0.1.tgz",
             "version": "5.0.1"
         },
         "json5": {
+            "dependencies": {
+                "minimist": {
+                    "dev": true,
+                    "integrity": "sha512-FM9nNUYrRBAELZQT3xeZQ7fmMOBg6nWNmJKTcgsJeaLstP/UODVpGsr5OhXhhXg6f+qtJ8uiZ+PUxkDWcgIXLw==",
+                    "resolved": "https://registry.npmjs.org/minimist/-/minimist-1.2.5.tgz",
+                    "version": "1.2.5"
+                }
+            },
             "dev": true,
-            "integrity": "sha512-l+3HXD0GEI3huGq1njuqtzYK8OYJyXMkOLtQ53pjWh89tvWS2h6l+1zMkYWqlb57+SiQodKZyvMEFb2X+KrFhQ==",
+            "integrity": "sha512-KXPvOm8K9IJKFM0bmdn8QXh7udDh1g/giieX0NLCaMnb4hEiVFqnop2ImTXCc5e0/oHz3LTqmHGtExn5hfMkOA==",
             "requires": {
-                "minimist": "^1.2.0"
+                "minimist": "^1.2.5"
             },
-            "resolved": "https://registry.npmjs.org/json5/-/json5-2.1.1.tgz",
-            "version": "2.1.1"
+            "resolved": "https://registry.npmjs.org/json5/-/json5-2.1.3.tgz",
+            "version": "2.1.3"
         },
         "jsprim": {
             "dev": true,
             "integrity": "sha1-MT5mvB5cwG5Di8G3SZwuXFastqI=",
             "requires": {
                 "assert-plus": "1.0.0",
                 "extsprintf": "1.3.0",
@@ -4884,42 +4889,33 @@
                 "verror": "1.10.0"
             },
             "resolved": "https://registry.npmjs.org/jsprim/-/jsprim-1.4.1.tgz",
             "version": "1.4.1"
         },
         "kind-of": {
             "dev": true,
-            "integrity": "sha512-s5kLOcnH0XqDO+FvuaLX8DDjZ18CGFk7VygH40QoKPUQhW4e2rvM0rwUq0t8IQDOwYSeLK01U90OjzBTme2QqA==",
-            "resolved": "https://registry.npmjs.org/kind-of/-/kind-of-6.0.2.tgz",
-            "version": "6.0.2"
-        },
-        "lcid": {
-            "dev": true,
-            "integrity": "sha1-MIrMr6C8SDo4Z7S28rlQYlHRuDU=",
-            "requires": {
-                "invert-kv": "^1.0.0"
-            },
-            "resolved": "https://registry.npmjs.org/lcid/-/lcid-1.0.0.tgz",
-            "version": "1.0.0"
+            "integrity": "sha512-dcS1ul+9tmeD95T+x28/ehLgd9mENa3LsvDTtzm3vyBEO7RPptvAD+t44WVXaUjTBRcrpFeFlC8WCruUR456hw==",
+            "resolved": "https://registry.npmjs.org/kind-of/-/kind-of-6.0.3.tgz",
+            "version": "6.0.3"
         },
         "levn": {
             "dev": true,
             "integrity": "sha1-OwmSTt+fCDwEkP3UwLxEIeBHZO4=",
             "requires": {
                 "prelude-ls": "~1.1.2",
                 "type-check": "~0.3.2"
             },
             "resolved": "https://registry.npmjs.org/levn/-/levn-0.3.0.tgz",
             "version": "0.3.0"
         },
         "lodash": {
             "dev": true,
-            "integrity": "sha512-8xOcRHvCjnocdS5cpwXQXVzmmh5e5+saE2QGoeQmbKmRS6J3VQppPOIt0MnmE+4xlZoumy0GPG0D0MVIQbNA1A==",
-            "resolved": "https://registry.npmjs.org/lodash/-/lodash-4.17.15.tgz",
-            "version": "4.17.15"
+            "integrity": "sha512-PlhdFcillOINfeV7Ni6oF1TAEayyZBoZ8bcshTHqOYJYlrqzRK5hagpagky5o4HfCzzd1TRkXPMFq6cKk9rGmA==",
+            "resolved": "https://registry.npmjs.org/lodash/-/lodash-4.17.20.tgz",
+            "version": "4.17.20"
         },
         "lodash.clone": {
             "dev": true,
             "integrity": "sha1-GVhwRQ9aExkkeN9Lw9I9LeoZB7Y=",
             "resolved": "https://registry.npmjs.org/lodash.clone/-/lodash.clone-4.5.0.tgz",
             "version": "4.5.0"
         },
@@ -4947,41 +4943,22 @@
             "requires": {
                 "chalk": "^2.0.1"
             },
             "resolved": "https://registry.npmjs.org/log-symbols/-/log-symbols-2.2.0.tgz",
             "version": "2.2.0"
         },
         "loose-envify": {
+            "dev": true,
             "integrity": "sha512-lyuxPGr/Wfhrlem2CL/UcnUc1zcqKAImBDzukY7Y5F/yQiNdko6+fRLevlw1HgMySw7f611UIY408EtxRSoK3Q==",
             "requires": {
                 "js-tokens": "^3.0.0 || ^4.0.0"
             },
             "resolved": "https://registry.npmjs.org/loose-envify/-/loose-envify-1.4.0.tgz",
             "version": "1.4.0"
         },
-        "loud-rejection": {
-            "dev": true,
-            "integrity": "sha1-W0b4AUft7leIcPCG0Eghz5mOVR8=",
-            "requires": {
-                "currently-unhandled": "^0.4.1",
-                "signal-exit": "^3.0.0"
-            },
-            "resolved": "https://registry.npmjs.org/loud-rejection/-/loud-rejection-1.6.0.tgz",
-            "version": "1.6.0"
-        },
-        "lru-cache": {
-            "dev": true,
-            "integrity": "sha512-sWZlbEP2OsHNkXrMl5GYk/jKk70MBng6UU4YI/qGDYbgf6YbP4EvmqISbXCoJiRKs+1bSpFHVgQxvJ17F2li5g==",
-            "requires": {
-                "pseudomap": "^1.0.2",
-                "yallist": "^2.1.2"
-            },
-            "resolved": "https://registry.npmjs.org/lru-cache/-/lru-cache-4.1.5.tgz",
-            "version": "4.1.5"
-        },
         "magic-string": {
             "dev": true,
             "integrity": "sha512-oreip9rJZkzvA8Qzk9HFs8fZGF/u7H/gtrE8EN6RjKJ9kh2HlC+yQ2QezifqTZfGyiuAV0dRv5a+y/8gBb1m9w==",
             "requires": {
                 "vlq": "^0.2.2"
             },
             "resolved": "https://registry.npmjs.org/magic-string/-/magic-string-0.22.5.tgz",
@@ -5111,17 +5088,17 @@
                 "brace-expansion": "^1.1.7"
             },
             "resolved": "https://registry.npmjs.org/minimatch/-/minimatch-3.0.4.tgz",
             "version": "3.0.4"
         },
         "minimist": {
             "dev": true,
-            "integrity": "sha1-o1AIsg9BOD7sH7kU9M1d95omQoQ=",
-            "resolved": "https://registry.npmjs.org/minimist/-/minimist-1.2.0.tgz",
-            "version": "1.2.0"
+            "integrity": "sha512-FM9nNUYrRBAELZQT3xeZQ7fmMOBg6nWNmJKTcgsJeaLstP/UODVpGsr5OhXhhXg6f+qtJ8uiZ+PUxkDWcgIXLw==",
+            "resolved": "https://registry.npmjs.org/minimist/-/minimist-1.2.5.tgz",
+            "version": "1.2.5"
         },
         "mixin-deep": {
             "dependencies": {
                 "is-extendable": {
                     "dev": true,
                     "integrity": "sha512-arnXMxT1hhoKo9k1LZdmlNyJdDDfy2v0fXjFlmok4+i8ul/6WlbVge9bhM74OpNPQPMGUToDtz+KXa1PneJxOA==",
                     "requires": {
@@ -5137,39 +5114,32 @@
                 "for-in": "^1.0.2",
                 "is-extendable": "^1.0.1"
             },
             "resolved": "https://registry.npmjs.org/mixin-deep/-/mixin-deep-1.3.2.tgz",
             "version": "1.3.2"
         },
         "mkdirp": {
-            "dependencies": {
-                "minimist": {
-                    "dev": true,
-                    "integrity": "sha1-hX/Kv8M5fSYluCKCYuhqp6ARsF0=",
-                    "resolved": "https://registry.npmjs.org/minimist/-/minimist-0.0.8.tgz",
-                    "version": "0.0.8"
-                }
-            },
             "dev": true,
-            "integrity": "sha1-MAV0OOrGz3+MR2fzhkjWaX11yQM=",
+            "integrity": "sha512-NKmAlESf6jMGym1++R0Ra7wvhV+wFW63FaSOFPwRahvea0gMUcGUhVeAg/0BC0wiv9ih5NYPB1Wn1UEI1/L+xQ==",
             "requires": {
-                "minimist": "0.0.8"
+                "minimist": "^1.2.5"
             },
-            "resolved": "https://registry.npmjs.org/mkdirp/-/mkdirp-0.5.1.tgz",
-            "version": "0.5.1"
+            "resolved": "https://registry.npmjs.org/mkdirp/-/mkdirp-0.5.5.tgz",
+            "version": "0.5.5"
         },
         "ms": {
             "dev": true,
             "integrity": "sha512-sGkPx+VjMtmA6MX27oA4FBFELFCZZ4S4XqeGOXCv68tT+jb3vk/RyaKWP0PTKyWtmLSM0b+adUTEvbs1PEaH2w==",
             "resolved": "https://registry.npmjs.org/ms/-/ms-2.1.2.tgz",
             "version": "2.1.2"
         },
         "nan": {
             "dev": true,
             "integrity": "sha512-INOFj37C7k3AfaNTtX8RhsTw7qRy7eLET14cROi9+5HAVbbHuIWUHEauBv5qT4Av2tWasiTY1Jw6puUNqRJXQg==",
+            "optional": true,
             "resolved": "https://registry.npmjs.org/nan/-/nan-2.14.0.tgz",
             "version": "2.14.0"
         },
         "nanomatch": {
             "dev": true,
             "integrity": "sha512-fpoe2T0RbHwBTBUOftAfBPaDEi06ufaUai0mE6Yn1kacc3SnTErfb/h+X94VXzI64rKFHYImXSvdwGGCmwOqCA==",
             "requires": {
@@ -5196,57 +5166,20 @@
         },
         "node-addon-api": {
             "dev": true,
             "integrity": "sha512-2+DuKodWvwRTrCfKOeR24KIc5unKjOh8mz17NCzVnHWfjAdDqbfbjqh7gUT+BkXBRQM52+xCHciKWonJ3CbJMQ==",
             "resolved": "https://registry.npmjs.org/node-addon-api/-/node-addon-api-1.7.1.tgz",
             "version": "1.7.1"
         },
-        "node-fetch": {
-            "integrity": "sha512-NhZ4CsKx7cYm2vSrBAr2PvFOe6sWDf0UYLRqA6svUYg7+/TSfVAu49jYC4BvQ4Sms9SZgdqGBgroqfDhJdTyKQ==",
-            "requires": {
-                "encoding": "^0.1.11",
-                "is-stream": "^1.0.1"
-            },
-            "resolved": "https://registry.npmjs.org/node-fetch/-/node-fetch-1.7.3.tgz",
-            "version": "1.7.3"
-        },
         "node-forge": {
             "dev": true,
             "integrity": "sha512-sol30LUpz1jQFBjOKwbjxijiE3b6pjd74YwfD0fJOKPjF+fONKb2Yg8rYgS6+bK6VDl+/wfr4IYpC7jDzLUIfw==",
             "resolved": "https://registry.npmjs.org/node-forge/-/node-forge-0.7.6.tgz",
             "version": "0.7.6"
         },
-        "node-gyp": {
-            "dependencies": {
-                "semver": {
-                    "dev": true,
-                    "integrity": "sha1-myzl094C0XxgEq0yaqa00M9U+U8=",
-                    "resolved": "https://registry.npmjs.org/semver/-/semver-5.3.0.tgz",
-                    "version": "5.3.0"
-                }
-            },
-            "dev": true,
-            "integrity": "sha512-3g8lYefrRRzvGeSowdJKAKyks8oUpLEd/DyPV4eMhVlhJ0aNaZqIrNUIPuEWWTAoPqyFkfGrM67MC69baqn6vA==",
-            "requires": {
-                "fstream": "^1.0.0",
-                "glob": "^7.0.3",
-                "graceful-fs": "^4.1.2",
-                "mkdirp": "^0.5.0",
-                "nopt": "2 || 3",
-                "npmlog": "0 || 1 || 2 || 3 || 4",
-                "osenv": "0",
-                "request": "^2.87.0",
-                "rimraf": "2",
-                "semver": "~5.3.0",
-                "tar": "^2.0.0",
-                "which": "1"
-            },
-            "resolved": "https://registry.npmjs.org/node-gyp/-/node-gyp-3.8.0.tgz",
-            "version": "3.8.0"
-        },
         "node-libs-browser": {
             "dependencies": {
                 "isarray": {
                     "dev": true,
                     "integrity": "sha1-u5NdSFgsuhaMBoNJV6VKPgcSTxE=",
                     "resolved": "https://registry.npmjs.org/isarray/-/isarray-1.0.0.tgz",
                     "version": "1.0.0"
@@ -5344,338 +5277,49 @@
             "integrity": "sha512-OQ/ESmUqGawI2PRX+XIRao44qWYBBfN54ImQYdWVTQqUckuejOg76ysSqDBK8NG3zwySRVnX36JwDQ6x+9GxzA==",
             "requires": {
                 "semver": "^6.3.0"
             },
             "resolved": "https://registry.npmjs.org/node-releases/-/node-releases-1.1.42.tgz",
             "version": "1.1.42"
         },
-        "node-sass": {
-            "dependencies": {
-                "ansi-regex": {
-                    "dev": true,
-                    "integrity": "sha1-w7M6te42DYbg5ijwRorn7yfWVN8=",
-                    "resolved": "https://registry.npmjs.org/ansi-regex/-/ansi-regex-2.1.1.tgz",
-                    "version": "2.1.1"
-                },
-                "ansi-styles": {
-                    "dev": true,
-                    "integrity": "sha1-tDLdM1i2NM914eRmQ2gkBTPB3b4=",
-                    "resolved": "https://registry.npmjs.org/ansi-styles/-/ansi-styles-2.2.1.tgz",
-                    "version": "2.2.1"
-                },
-                "camelcase": {
-                    "dev": true,
-                    "integrity": "sha1-fB0W1nmhu+WcoCys7PsBHiAfWh8=",
-                    "resolved": "https://registry.npmjs.org/camelcase/-/camelcase-2.1.1.tgz",
-                    "version": "2.1.1"
-                },
-                "camelcase-keys": {
-                    "dev": true,
-                    "integrity": "sha1-MIvur/3ygRkFHvodkyITyRuPkuc=",
-                    "requires": {
-                        "camelcase": "^2.0.0",
-                        "map-obj": "^1.0.0"
-                    },
-                    "resolved": "https://registry.npmjs.org/camelcase-keys/-/camelcase-keys-2.1.0.tgz",
-                    "version": "2.1.0"
-                },
-                "chalk": {
-                    "dev": true,
-                    "integrity": "sha1-qBFcVeSnAv5NFQq9OHKCKn4J/Jg=",
-                    "requires": {
-                        "ansi-styles": "^2.2.1",
-                        "escape-string-regexp": "^1.0.2",
-                        "has-ansi": "^2.0.0",
-                        "strip-ansi": "^3.0.0",
-                        "supports-color": "^2.0.0"
-                    },
-                    "resolved": "https://registry.npmjs.org/chalk/-/chalk-1.1.3.tgz",
-                    "version": "1.1.3"
-                },
-                "cross-spawn": {
-                    "dev": true,
-                    "integrity": "sha1-ElYDfsufDF9549bvE14wdwGEuYI=",
-                    "requires": {
-                        "lru-cache": "^4.0.1",
-                        "which": "^1.2.9"
-                    },
-                    "resolved": "https://registry.npmjs.org/cross-spawn/-/cross-spawn-3.0.1.tgz",
-                    "version": "3.0.1"
-                },
-                "find-up": {
-                    "dev": true,
-                    "integrity": "sha1-ay6YIrGizgpgq2TWEOzK1TyyTQ8=",
-                    "requires": {
-                        "path-exists": "^2.0.0",
-                        "pinkie-promise": "^2.0.0"
-                    },
-                    "resolved": "https://registry.npmjs.org/find-up/-/find-up-1.1.2.tgz",
-                    "version": "1.1.2"
-                },
-                "indent-string": {
-                    "dev": true,
-                    "integrity": "sha1-ji1INIdCEhtKghi3oTfppSBJ3IA=",
-                    "requires": {
-                        "repeating": "^2.0.0"
-                    },
-                    "resolved": "https://registry.npmjs.org/indent-string/-/indent-string-2.1.0.tgz",
-                    "version": "2.1.0"
-                },
-                "load-json-file": {
-                    "dev": true,
-                    "integrity": "sha1-lWkFcI1YtLq0wiYbBPWfMcmTdMA=",
-                    "requires": {
-                        "graceful-fs": "^4.1.2",
-                        "parse-json": "^2.2.0",
-                        "pify": "^2.0.0",
-                        "pinkie-promise": "^2.0.0",
-                        "strip-bom": "^2.0.0"
-                    },
-                    "resolved": "https://registry.npmjs.org/load-json-file/-/load-json-file-1.1.0.tgz",
-                    "version": "1.1.0"
-                },
-                "map-obj": {
-                    "dev": true,
-                    "integrity": "sha1-2TPOuSBdgr3PSIb2dCvcK03qFG0=",
-                    "resolved": "https://registry.npmjs.org/map-obj/-/map-obj-1.0.1.tgz",
-                    "version": "1.0.1"
-                },
-                "meow": {
-                    "dev": true,
-                    "integrity": "sha1-cstmi0JSKCkKu/qFaJJYcwioAfs=",
-                    "requires": {
-                        "camelcase-keys": "^2.0.0",
-                        "decamelize": "^1.1.2",
-                        "loud-rejection": "^1.0.0",
-                        "map-obj": "^1.0.1",
-                        "minimist": "^1.1.3",
-                        "normalize-package-data": "^2.3.4",
-                        "object-assign": "^4.0.1",
-                        "read-pkg-up": "^1.0.1",
-                        "redent": "^1.0.0",
-                        "trim-newlines": "^1.0.0"
-                    },
-                    "resolved": "https://registry.npmjs.org/meow/-/meow-3.7.0.tgz",
-                    "version": "3.7.0"
-                },
-                "parse-json": {
-                    "dev": true,
-                    "integrity": "sha1-9ID0BDTvgHQfhGkJn43qGPVaTck=",
-                    "requires": {
-                        "error-ex": "^1.2.0"
-                    },
-                    "resolved": "https://registry.npmjs.org/parse-json/-/parse-json-2.2.0.tgz",
-                    "version": "2.2.0"
-                },
-                "path-exists": {
-                    "dev": true,
-                    "integrity": "sha1-D+tsZPD8UY2adU3V77YscCJ2H0s=",
-                    "requires": {
-                        "pinkie-promise": "^2.0.0"
-                    },
-                    "resolved": "https://registry.npmjs.org/path-exists/-/path-exists-2.1.0.tgz",
-                    "version": "2.1.0"
-                },
-                "path-type": {
-                    "dev": true,
-                    "integrity": "sha1-WcRPfuSR2nBNpBXaWkBwuk+P5EE=",
-                    "requires": {
-                        "graceful-fs": "^4.1.2",
-                        "pify": "^2.0.0",
-                        "pinkie-promise": "^2.0.0"
-                    },
-                    "resolved": "https://registry.npmjs.org/path-type/-/path-type-1.1.0.tgz",
-                    "version": "1.1.0"
-                },
-                "pify": {
-                    "dev": true,
-                    "integrity": "sha1-7RQaasBDqEnqWISY59yosVMw6Qw=",
-                    "resolved": "https://registry.npmjs.org/pify/-/pify-2.3.0.tgz",
-                    "version": "2.3.0"
-                },
-                "read-pkg": {
-                    "dev": true,
-                    "integrity": "sha1-9f+qXs0pyzHAR0vKfXVra7KePyg=",
-                    "requires": {
-                        "load-json-file": "^1.0.0",
-                        "normalize-package-data": "^2.3.2",
-                        "path-type": "^1.0.0"
-                    },
-                    "resolved": "https://registry.npmjs.org/read-pkg/-/read-pkg-1.1.0.tgz",
-                    "version": "1.1.0"
-                },
-                "read-pkg-up": {
-                    "dev": true,
-                    "integrity": "sha1-nWPBMnbAZZGNV/ACpX9AobZD+wI=",
-                    "requires": {
-                        "find-up": "^1.0.0",
-                        "read-pkg": "^1.0.0"
-                    },
-                    "resolved": "https://registry.npmjs.org/read-pkg-up/-/read-pkg-up-1.0.1.tgz",
-                    "version": "1.0.1"
-                },
-                "redent": {
-                    "dev": true,
-                    "integrity": "sha1-z5Fqsf1fHxbfsggi3W7H9zDCr94=",
-                    "requires": {
-                        "indent-string": "^2.1.0",
-                        "strip-indent": "^1.0.1"
-                    },
-                    "resolved": "https://registry.npmjs.org/redent/-/redent-1.0.0.tgz",
-                    "version": "1.0.0"
-                },
-                "strip-ansi": {
-                    "dev": true,
-                    "integrity": "sha1-ajhfuIU9lS1f8F0Oiq+UJ43GPc8=",
-                    "requires": {
-                        "ansi-regex": "^2.0.0"
-                    },
-                    "resolved": "https://registry.npmjs.org/strip-ansi/-/strip-ansi-3.0.1.tgz",
-                    "version": "3.0.1"
-                },
-                "strip-bom": {
-                    "dev": true,
-                    "integrity": "sha1-YhmoVhZSBJHzV4i9vxRHqZx+aw4=",
-                    "requires": {
-                        "is-utf8": "^0.2.0"
-                    },
-                    "resolved": "https://registry.npmjs.org/strip-bom/-/strip-bom-2.0.0.tgz",
-                    "version": "2.0.0"
-                },
-                "strip-indent": {
-                    "dev": true,
-                    "integrity": "sha1-DHlipq3vp7vUrDZkYKY4VSrhoKI=",
-                    "requires": {
-                        "get-stdin": "^4.0.1"
-                    },
-                    "resolved": "https://registry.npmjs.org/strip-indent/-/strip-indent-1.0.1.tgz",
-                    "version": "1.0.1"
-                },
-                "supports-color": {
-                    "dev": true,
-                    "integrity": "sha1-U10EXOa2Nj+kARcIRimZXp3zJMc=",
-                    "resolved": "https://registry.npmjs.org/supports-color/-/supports-color-2.0.0.tgz",
-                    "version": "2.0.0"
-                },
-                "trim-newlines": {
-                    "dev": true,
-                    "integrity": "sha1-WIeWa7WCpFA6QetST301ARgVphM=",
-                    "resolved": "https://registry.npmjs.org/trim-newlines/-/trim-newlines-1.0.0.tgz",
-                    "version": "1.0.0"
-                }
-            },
-            "dev": true,
-            "integrity": "sha512-W1XBrvoJ1dy7VsvTAS5q1V45lREbTlZQqFbiHb3R3OTTCma0XBtuG6xZ6Z4506nR4lmHPTqVRwxT6KgtWC97CA==",
-            "requires": {
-                "async-foreach": "^0.1.3",
-                "chalk": "^1.1.1",
-                "cross-spawn": "^3.0.0",
-                "gaze": "^1.0.0",
-                "get-stdin": "^4.0.1",
-                "glob": "^7.0.3",
-                "in-publish": "^2.0.0",
-                "lodash": "^4.17.15",
-                "meow": "^3.7.0",
-                "mkdirp": "^0.5.1",
-                "nan": "^2.13.2",
-                "node-gyp": "^3.8.0",
-                "npmlog": "^4.0.0",
-                "request": "^2.88.0",
-                "sass-graph": "^2.2.4",
-                "stdout-stream": "^1.4.0",
-                "true-case-path": "^1.0.2"
-            },
-            "resolved": "https://registry.npmjs.org/node-sass/-/node-sass-4.13.0.tgz",
-            "version": "4.13.0"
-        },
-        "nopt": {
-            "dev": true,
-            "integrity": "sha1-xkZdvwirzU2zWTF/eaxopkayj/k=",
-            "requires": {
-                "abbrev": "1"
-            },
-            "resolved": "https://registry.npmjs.org/nopt/-/nopt-3.0.6.tgz",
-            "version": "3.0.6"
-        },
         "normalize-html-whitespace": {
             "dev": true,
             "integrity": "sha512-9ui7CGtOOlehQu0t/OhhlmDyc71mKVlv+4vF+me4iZLPrNtRL2xoquEdfZxasC/bdQi/Hr3iTrpyRKIG+ocabA==",
             "resolved": "https://registry.npmjs.org/normalize-html-whitespace/-/normalize-html-whitespace-1.0.0.tgz",
             "version": "1.0.0"
         },
-        "normalize-package-data": {
-            "dev": true,
-            "integrity": "sha512-/5CMN3T0R4XTj4DcGaexo+roZSdSFW/0AOOTROrjxzCG1wrWXEsGbRKevjlIL+ZDE4sZlJr5ED4YW0yqmkK+eA==",
-            "requires": {
-                "hosted-git-info": "^2.1.4",
-                "resolve": "^1.10.0",
-                "semver": "2 || 3 || 4 || 5",
-                "validate-npm-package-license": "^3.0.1"
-            },
-            "resolved": "https://registry.npmjs.org/normalize-package-data/-/normalize-package-data-2.5.0.tgz",
-            "version": "2.5.0"
-        },
         "normalize-path": {
             "dev": true,
             "integrity": "sha512-6eZs5Ls3WtCisHWp9S2GUy8dqkpGi4BVSz3GaqiE6ezub0512ESztXUwUB6C6IKbQkY2Pnb/mD4WYojCRwcwLA==",
             "resolved": "https://registry.npmjs.org/normalize-path/-/normalize-path-3.0.0.tgz",
             "version": "3.0.0"
         },
-        "normalize-range": {
-            "dev": true,
-            "integrity": "sha1-LRDAa9/TEuqXd2laTShDlFa3WUI=",
-            "resolved": "https://registry.npmjs.org/normalize-range/-/normalize-range-0.1.2.tgz",
-            "version": "0.1.2"
-        },
-        "npmlog": {
-            "dev": true,
-            "integrity": "sha512-2uUqazuKlTaSI/dC8AzicUck7+IrEaOnN/e0jd3Xtt1KcGpwx30v50mL7oPyr/h9bL3E4aZccVwpwP+5W9Vjkg==",
-            "requires": {
-                "are-we-there-yet": "~1.1.2",
-                "console-control-strings": "~1.1.0",
-                "gauge": "~2.7.3",
-                "set-blocking": "~2.0.0"
-            },
-            "resolved": "https://registry.npmjs.org/npmlog/-/npmlog-4.1.2.tgz",
-            "version": "4.1.2"
-        },
         "nth-check": {
             "dev": true,
             "integrity": "sha512-WeBOdju8SnzPN5vTUJYxYUxLeXpCaVP5i5e0LF8fg7WORF2Wd7wFX/pk0tYZk7s8T+J7VLy0Da6J1+wCT0AtHg==",
             "requires": {
                 "boolbase": "~1.0.0"
             },
             "resolved": "https://registry.npmjs.org/nth-check/-/nth-check-1.0.2.tgz",
             "version": "1.0.2"
         },
-        "num2fraction": {
-            "dev": true,
-            "integrity": "sha1-b2gragJ6Tp3fpFZM0lidHU5mnt4=",
-            "resolved": "https://registry.npmjs.org/num2fraction/-/num2fraction-1.2.2.tgz",
-            "version": "1.2.2"
-        },
-        "number-is-nan": {
-            "dev": true,
-            "integrity": "sha1-CXtgK1NCKlIsGvuHkDGDNpQaAR0=",
-            "resolved": "https://registry.npmjs.org/number-is-nan/-/number-is-nan-1.0.1.tgz",
-            "version": "1.0.1"
-        },
         "nwsapi": {
             "dev": true,
             "integrity": "sha512-h2AatdwYH+JHiZpv7pt/gSX1XoRGb7L/qSIeuqA6GwYoF9w1vP1cw42TO0aI2pNyshRK5893hNSl+1//vHK7hQ==",
             "resolved": "https://registry.npmjs.org/nwsapi/-/nwsapi-2.2.0.tgz",
             "version": "2.2.0"
         },
         "oauth-sign": {
             "dev": true,
             "integrity": "sha512-fexhUFFPTGV8ybAtSIGbV6gOkSv8UtRbDBnAyLQw4QPKkgNlsH2ByPGtMUqdWkos6YCRmAqViwgZrJc/mRDzZQ==",
             "resolved": "https://registry.npmjs.org/oauth-sign/-/oauth-sign-0.9.0.tgz",
             "version": "0.9.0"
         },
         "object-assign": {
+            "dev": true,
             "integrity": "sha1-IQmtx5ZYh8/AXLvUQsrIv7s2CGM=",
             "resolved": "https://registry.npmjs.org/object-assign/-/object-assign-4.1.1.tgz",
             "version": "4.1.1"
         },
         "object-copy": {
             "dependencies": {
                 "define-property": {
@@ -5860,45 +5504,14 @@
         },
         "os-browserify": {
             "dev": true,
             "integrity": "sha1-hUNzx/XCMVkU/Jv8a9gjj92h7Cc=",
             "resolved": "https://registry.npmjs.org/os-browserify/-/os-browserify-0.3.0.tgz",
             "version": "0.3.0"
         },
-        "os-homedir": {
-            "dev": true,
-            "integrity": "sha1-/7xJiDNuDoM94MFox+8VISGqf7M=",
-            "resolved": "https://registry.npmjs.org/os-homedir/-/os-homedir-1.0.2.tgz",
-            "version": "1.0.2"
-        },
-        "os-locale": {
-            "dev": true,
-            "integrity": "sha1-IPnxeuKe00XoveWDsT0gCYA8FNk=",
-            "requires": {
-                "lcid": "^1.0.0"
-            },
-            "resolved": "https://registry.npmjs.org/os-locale/-/os-locale-1.4.0.tgz",
-            "version": "1.4.0"
-        },
-        "os-tmpdir": {
-            "dev": true,
-            "integrity": "sha1-u+Z0BseaqFxc/sdm/lc0VV36EnQ=",
-            "resolved": "https://registry.npmjs.org/os-tmpdir/-/os-tmpdir-1.0.2.tgz",
-            "version": "1.0.2"
-        },
-        "osenv": {
-            "dev": true,
-            "integrity": "sha512-0CWcCECdMVc2Rw3U5w9ZjqX6ga6ubk1xDVKxtBQPK7wis/0F2r9T6k4ydGYhecl7YUBxBVxhL5oisPsNxAPe2g==",
-            "requires": {
-                "os-homedir": "^1.0.0",
-                "os-tmpdir": "^1.0.0"
-            },
-            "resolved": "https://registry.npmjs.org/osenv/-/osenv-0.1.5.tgz",
-            "version": "0.1.5"
-        },
         "pako": {
             "dev": true,
             "integrity": "sha1-8/dSL073gjSNqBYbrZ7P1Rv4OnU=",
             "resolved": "https://registry.npmjs.org/pako/-/pako-0.2.9.tgz",
             "version": "0.2.9"
         },
         "parcel-bundler": {
@@ -6097,28 +5710,19 @@
         },
         "physical-cpu-count": {
             "dev": true,
             "integrity": "sha1-GN4vl+S/epVRrXURlCtUlverpmA=",
             "resolved": "https://registry.npmjs.org/physical-cpu-count/-/physical-cpu-count-2.0.0.tgz",
             "version": "2.0.0"
         },
-        "pinkie": {
+        "picomatch": {
             "dev": true,
-            "integrity": "sha1-clVrgM+g1IqXToDnckjoDtT3+HA=",
-            "resolved": "https://registry.npmjs.org/pinkie/-/pinkie-2.0.4.tgz",
-            "version": "2.0.4"
-        },
-        "pinkie-promise": {
-            "dev": true,
-            "integrity": "sha1-ITXW36ejWMBprJsXh3YogihFD/o=",
-            "requires": {
-                "pinkie": "^2.0.0"
-            },
-            "resolved": "https://registry.npmjs.org/pinkie-promise/-/pinkie-promise-2.0.1.tgz",
-            "version": "2.0.1"
+            "integrity": "sha512-q0M/9eZHzmr0AulXyPwNfZjtwZ/RBZlbN3K3CErVrk50T2ASYI7Bye0EvekFY3IP1Nt2DHu0re+V2ZHIpMkuWg==",
+            "resolved": "https://registry.npmjs.org/picomatch/-/picomatch-2.2.2.tgz",
+            "version": "2.2.2"
         },
         "pn": {
             "dev": true,
             "integrity": "sha512-2qHaIQr2VLRFoxe2nASzsV6ef4yOOH+Fi9FBOVH6cqeSgUnoyySPZkxzLuzd+RYOQTRpROA0ztTMqxROKSb/nA==",
             "resolved": "https://registry.npmjs.org/pn/-/pn-1.1.0.tgz",
             "version": "1.1.0"
         },
@@ -6791,20 +6395,14 @@
                 "alphanum-sort": "^1.0.0",
                 "postcss": "^7.0.0",
                 "uniqs": "^2.0.0"
             },
             "resolved": "https://registry.npmjs.org/postcss-unique-selectors/-/postcss-unique-selectors-4.0.1.tgz",
             "version": "4.0.1"
         },
-        "postcss-value-parser": {
-            "dev": true,
-            "integrity": "sha512-LmeoohTpp/K4UiyQCwuGWlONxXamGzCMtFxLq4W1nZVGIQLYvMCJx3yAF9qyyuFpflABI9yVdtJAqbihOsCsJQ==",
-            "resolved": "https://registry.npmjs.org/postcss-value-parser/-/postcss-value-parser-4.0.2.tgz",
-            "version": "4.0.2"
-        },
         "posthtml": {
             "dev": true,
             "integrity": "sha512-C2hrAPzmRdpuL3iH0TDdQ6XCc9M7Dcc3zEW5BLerY65G4tWWszwv6nG/ksi6ul5i2mx22ubdljgktXCtNkydkw==",
             "requires": {
                 "posthtml-parser": "^0.4.1",
                 "posthtml-render": "^1.1.5"
             },
@@ -6846,38 +6444,14 @@
         },
         "process-nextick-args": {
             "dev": true,
             "integrity": "sha512-3ouUOpQhtgrbOa17J7+uxOTpITYWaGP7/AhoR3+A+/1e9skrzelGi/dXzEYyvbxubEF6Wn2ypscTKiKJFFn1ag==",
             "resolved": "https://registry.npmjs.org/process-nextick-args/-/process-nextick-args-2.0.1.tgz",
             "version": "2.0.1"
         },
-        "promise": {
-            "integrity": "sha512-nolQXZ/4L+bP/UGlkfaIujX9BKxGwmQ9OT4mOt5yvy8iK1h3wqTEJCijzGANTCCl9nWjY41juyAn2K3Q1hLLTg==",
-            "requires": {
-                "asap": "~2.0.3"
-            },
-            "resolved": "https://registry.npmjs.org/promise/-/promise-7.3.1.tgz",
-            "version": "7.3.1"
-        },
-        "prop-types": {
-            "integrity": "sha512-8QQikdH7//R2vurIJSutZ1smHYTcLpRWEOlHnzcWHmBYrOGUysKwSsrC89BCiFj3CbrfJ/nXFdJepOVrY1GCHQ==",
-            "requires": {
-                "loose-envify": "^1.4.0",
-                "object-assign": "^4.1.1",
-                "react-is": "^16.8.1"
-            },
-            "resolved": "https://registry.npmjs.org/prop-types/-/prop-types-15.7.2.tgz",
-            "version": "15.7.2"
-        },
-        "pseudomap": {
-            "dev": true,
-            "integrity": "sha1-8FKijacOYYkX7wqKw0wa5aaChrM=",
-            "resolved": "https://registry.npmjs.org/pseudomap/-/pseudomap-1.0.2.tgz",
-            "version": "1.0.2"
-        },
         "psl": {
             "dev": true,
             "integrity": "sha512-SYKKmVel98NCOYXpkwUqZqh0ahZeeKfmisiLIcEZdsb+WbLv02g/dI5BUmZnIyOe7RzZtLax81nnb2HbvC2tzA==",
             "resolved": "https://registry.npmjs.org/psl/-/psl-1.6.0.tgz",
             "version": "1.6.0"
         },
         "public-encrypt": {
@@ -6904,20 +6478,14 @@
             "dependencies": {
                 "ansi-regex": {
                     "dev": true,
                     "integrity": "sha512-1apePfXM1UOSqw0o9IiFAovVz9M5S1Dg+4TrDwfMewQ6p/rmMueb7tWZjQ1rx4Loy1ArBggoqGpfqqdI4rondg==",
                     "resolved": "https://registry.npmjs.org/ansi-regex/-/ansi-regex-4.1.0.tgz",
                     "version": "4.1.0"
                 },
-                "camelcase": {
-                    "dev": true,
-                    "integrity": "sha512-L28STB170nwWS63UjtlEOE3dldQApaJXZkOI1uMFfzf3rRuPegHaHesyee+YxQ+W6SvRDQV6UrdOdRiR153wJg==",
-                    "resolved": "https://registry.npmjs.org/camelcase/-/camelcase-5.3.1.tgz",
-                    "version": "5.3.1"
-                },
                 "cliui": {
                     "dev": true,
                     "integrity": "sha512-PYeGSEmmHM6zvoef2w8TPzlrnNpXIjTipYK780YswmIP9vjxmd6Y2a3CB2Ks6/AU8NHjZugXvo8w3oWM2qnwXA==",
                     "requires": {
                         "string-width": "^3.1.0",
                         "strip-ansi": "^5.2.0",
                         "wrap-ansi": "^5.1.0"
@@ -7066,24 +6634,14 @@
                         "string-width": "^3.0.0",
                         "which-module": "^2.0.0",
                         "y18n": "^4.0.0",
                         "yargs-parser": "^15.0.0"
                     },
                     "resolved": "https://registry.npmjs.org/yargs/-/yargs-14.2.2.tgz",
                     "version": "14.2.2"
-                },
-                "yargs-parser": {
-                    "dev": true,
-                    "integrity": "sha512-xLTUnCMc4JhxrPEPUYD5IBR1mWCK/aT6+RJ/K29JY2y1vD+FhtgKK0AXRWvI262q3QSffAQuTouFIKUuHX89wQ==",
-                    "requires": {
-                        "camelcase": "^5.0.0",
-                        "decamelize": "^1.2.0"
-                    },
-                    "resolved": "https://registry.npmjs.org/yargs-parser/-/yargs-parser-15.0.0.tgz",
-                    "version": "15.0.0"
                 }
             },
             "dev": true,
             "integrity": "sha512-hkOreFTgiyMHMmC2BxzdIw5DuC6kxAbP/gGOGd3MEsF3+5m69rIvUEPaxrnoUtfODTFKe9hcXjGwC6jcjoyhOw==",
             "requires": {
                 "glob": "^7.1.3",
                 "postcss": "^7.0.14",
@@ -7149,56 +6707,14 @@
         },
         "range-parser": {
             "dev": true,
             "integrity": "sha512-Hrgsx+orqoygnmhFbKaHE6c296J+HTAQXoxEF6gNupROmmGJRoyzfG3ccAveqCBrwr/2yxQ5BVd/GTl5agOwSg==",
             "resolved": "https://registry.npmjs.org/range-parser/-/range-parser-1.2.1.tgz",
             "version": "1.2.1"
         },
-        "react": {
-            "integrity": "sha512-YMZQQq32xHLX0bz5Mnibv1/LHb3Sqzngu7xstSM+vrkE5Kzr9xE0yMByK5kMoTK30YVJE61WfbxIFFvfeDKT1w==",
-            "requires": {
-                "loose-envify": "^1.1.0",
-                "object-assign": "^4.1.1",
-                "prop-types": "^15.6.2"
-            },
-            "resolved": "https://registry.npmjs.org/react/-/react-16.13.1.tgz",
-            "version": "16.13.1"
-        },
-        "react-dom": {
-            "integrity": "sha512-81PIMmVLnCNLO/fFOQxdQkvEq/+Hfpv24XNJfpyZhTRfO0QcmQIF/PgCa1zCOj2w1hrn12MFLyaJ/G0+Mxtfag==",
-            "requires": {
-                "loose-envify": "^1.1.0",
-                "object-assign": "^4.1.1",
-                "prop-types": "^15.6.2",
-                "scheduler": "^0.19.1"
-            },
-            "resolved": "https://registry.npmjs.org/react-dom/-/react-dom-16.13.1.tgz",
-            "version": "16.13.1"
-        },
-        "react-is": {
-            "integrity": "sha512-rPCkf/mWBtKc97aLL9/txD8DZdemK0vkA3JMLShjlJB3Pj3s+lpf1KaBzMfQrAmhMQB0n1cU/SUGgKKBCe837Q==",
-            "resolved": "https://registry.npmjs.org/react-is/-/react-is-16.12.0.tgz",
-            "version": "16.12.0"
-        },
-        "react-lifecycles-compat": {
-            "integrity": "sha512-fBASbA6LnOU9dOU2eW7aQ8xmYBSXUIWr+UmF9b1efZBazGNO+rcXT/icdKnYm2pTwcRylVUYwW7H1PHfLekVzA==",
-            "resolved": "https://registry.npmjs.org/react-lifecycles-compat/-/react-lifecycles-compat-3.0.4.tgz",
-            "version": "3.0.4"
-        },
-        "react-modal": {
-            "integrity": "sha512-o8gvvCOFaG1T7W6JUvsYjRjMVToLZgLIsi5kdhFIQCtHxDkA47LznX62j+l6YQkpXDbvQegsDyxe/+JJsFQN7w==",
-            "requires": {
-                "exenv": "^1.2.0",
-                "prop-types": "^15.5.10",
-                "react-lifecycles-compat": "^3.0.0",
-                "warning": "^4.0.3"
-            },
-            "resolved": "https://registry.npmjs.org/react-modal/-/react-modal-3.11.2.tgz",
-            "version": "3.11.2"
-        },
         "readdirp": {
             "dependencies": {
                 "isarray": {
                     "dev": true,
                     "integrity": "sha1-u5NdSFgsuhaMBoNJV6VKPgcSTxE=",
                     "resolved": "https://registry.npmjs.org/isarray/-/isarray-1.0.0.tgz",
                     "version": "1.0.0"
@@ -7329,23 +6845,14 @@
         },
         "repeat-string": {
             "dev": true,
             "integrity": "sha1-jcrkcOHIirwtYA//Sndihtp15jc=",
             "resolved": "https://registry.npmjs.org/repeat-string/-/repeat-string-1.6.1.tgz",
             "version": "1.6.1"
         },
-        "repeating": {
-            "dev": true,
-            "integrity": "sha1-UhTFOpJtNVJwdSf7q0FdvAjQbdo=",
-            "requires": {
-                "is-finite": "^1.0.0"
-            },
-            "resolved": "https://registry.npmjs.org/repeating/-/repeating-2.0.1.tgz",
-            "version": "2.0.1"
-        },
         "request": {
             "dev": true,
             "integrity": "sha512-NAqBSrijGLZdM0WZNsInLJpkJokL72XYjUpnB0iwsRgxh7dB6COrHnTBNwN0E+lHDAJzu7kLAkDeY08z2/A0hg==",
             "requires": {
                 "aws-sign2": "~0.7.0",
                 "aws4": "^1.8.0",
                 "caseless": "~0.12.0",
@@ -7392,20 +6899,14 @@
         },
         "require-directory": {
             "dev": true,
             "integrity": "sha1-jGStX9MNqxyXbiNE/+f3kqam30I=",
             "resolved": "https://registry.npmjs.org/require-directory/-/require-directory-2.1.1.tgz",
             "version": "2.1.1"
         },
-        "require-main-filename": {
-            "dev": true,
-            "integrity": "sha1-l/cXtp1IeE9fUmpsWqj/3aBVpNE=",
-            "resolved": "https://registry.npmjs.org/require-main-filename/-/require-main-filename-1.0.1.tgz",
-            "version": "1.0.1"
-        },
         "resolve": {
             "dev": true,
             "integrity": "sha512-CxqObCX8K8YtAhOBRg+lrcdn+LK+WYOS8tSjqSFbjtrI5PnS63QPhZl4+yKfrU9tdsbMu9Anr/amegT87M9Z6w==",
             "requires": {
                 "path-parse": "^1.0.6"
             },
             "resolved": "https://registry.npmjs.org/resolve/-/resolve-1.13.1.tgz",
@@ -7476,29 +6977,27 @@
             "requires": {
                 "ret": "~0.1.10"
             },
             "resolved": "https://registry.npmjs.org/safe-regex/-/safe-regex-1.1.0.tgz",
             "version": "1.1.0"
         },
         "safer-buffer": {
+            "dev": true,
             "integrity": "sha512-YZo3K82SD7Riyi0E1EQPojLz7kpepnSQI9IyPbHHg1XXXevb5dJI7tpyN2ADxGcQbHG7vcyRHk0cbwqcQriUtg==",
             "resolved": "https://registry.npmjs.org/safer-buffer/-/safer-buffer-2.1.2.tgz",
             "version": "2.1.2"
         },
-        "sass-graph": {
+        "sass": {
             "dev": true,
-            "integrity": "sha1-E/vWPNHK8JCLn9k0dq1DpR0eC0k=",
+            "integrity": "sha512-bzN0uvmzfsTvjz0qwccN1sPm2HxxpNI/Xa+7PlUEMS+nQvbyuEK7Y0qFqxlPHhiNHb1Ze8WQJtU31olMObkAMw==",
             "requires": {
-                "glob": "^7.0.0",
-                "lodash": "^4.0.0",
-                "scss-tokenizer": "^0.2.3",
-                "yargs": "^7.0.0"
+                "chokidar": ">=2.0.0 <4.0.0"
             },
-            "resolved": "https://registry.npmjs.org/sass-graph/-/sass-graph-2.2.4.tgz",
-            "version": "2.2.4"
+            "resolved": "https://registry.npmjs.org/sass/-/sass-1.26.10.tgz",
+            "version": "1.26.10"
         },
         "sax": {
             "dev": true,
             "integrity": "sha512-NqVDv9TpANUjFm0N8uM5GxL36UgKi9/atZw+x7YFnQ8ckwFGKrl4xX4yWtrey3UJm5nP1kUbnYgLopqWNSRhWw==",
             "resolved": "https://registry.npmjs.org/sax/-/sax-1.2.4.tgz",
             "version": "1.2.4"
         },
@@ -7507,44 +7006,14 @@
             "integrity": "sha512-Ydydq3zC+WYDJK1+gRxRapLIED9PWeSuuS41wqyoRmzvhhh9nc+QQrVMKJYzJFULazeGhzSV0QleN2wD3boh2g==",
             "requires": {
                 "xmlchars": "^2.1.1"
             },
             "resolved": "https://registry.npmjs.org/saxes/-/saxes-3.1.11.tgz",
             "version": "3.1.11"
         },
-        "scheduler": {
-            "integrity": "sha512-n/zwRWRYSUj0/3g/otKDRPMh6qv2SYMWNq85IEa8iZyAv8od9zDYpGSnpBEjNgcMNq6Scbu5KfIPxNF72R/2EA==",
-            "requires": {
-                "loose-envify": "^1.1.0",
-                "object-assign": "^4.1.1"
-            },
-            "resolved": "https://registry.npmjs.org/scheduler/-/scheduler-0.19.1.tgz",
-            "version": "0.19.1"
-        },
-        "scss-tokenizer": {
-            "dependencies": {
-                "source-map": {
-                    "dev": true,
-                    "integrity": "sha1-66T12pwNyZneaAMti092FzZSA2s=",
-                    "requires": {
-                        "amdefine": ">=0.0.4"
-                    },
-                    "resolved": "https://registry.npmjs.org/source-map/-/source-map-0.4.4.tgz",
-                    "version": "0.4.4"
-                }
-            },
-            "dev": true,
-            "integrity": "sha1-jrBtualyMzOCTT9VMGQRSYR85dE=",
-            "requires": {
-                "js-base64": "^2.1.8",
-                "source-map": "^0.4.2"
-            },
-            "resolved": "https://registry.npmjs.org/scss-tokenizer/-/scss-tokenizer-0.2.3.tgz",
-            "version": "0.2.3"
-        },
         "semver": {
             "dev": true,
             "integrity": "sha512-sauaDf/PZdVgrLTNYHRtpXa1iRiKcaebiKQ1BJdpQlWH2lCvexQdX55snPFyK7QzpudqbCI0qXFfOasHdyNDGQ==",
             "resolved": "https://registry.npmjs.org/semver/-/semver-5.7.1.tgz",
             "version": "5.7.1"
         },
         "send": {
@@ -7637,14 +7106,15 @@
                 "is-plain-object": "^2.0.3",
                 "split-string": "^3.0.1"
             },
             "resolved": "https://registry.npmjs.org/set-value/-/set-value-2.0.1.tgz",
             "version": "2.0.1"
         },
         "setimmediate": {
+            "dev": true,
             "integrity": "sha1-KQy7Iy4waULX1+qbg3Mqt4VvgoU=",
             "resolved": "https://registry.npmjs.org/setimmediate/-/setimmediate-1.0.5.tgz",
             "version": "1.0.5"
         },
         "setprototypeof": {
             "dev": true,
             "integrity": "sha512-JvdAWfbXeIGaZ9cILp38HntZSFSo3mWg6xGcJJsd+d4aRMOqauag1C63dJfDw7OaMYwEbHMOxEZ1lqVRYP2OAw==",
@@ -7872,46 +7342,14 @@
         },
         "source-map-url": {
             "dev": true,
             "integrity": "sha1-PpNdfd1zYxuXZZlW1VEo6HtQhKM=",
             "resolved": "https://registry.npmjs.org/source-map-url/-/source-map-url-0.4.0.tgz",
             "version": "0.4.0"
         },
-        "spdx-correct": {
-            "dev": true,
-            "integrity": "sha512-lr2EZCctC2BNR7j7WzJ2FpDznxky1sjfxvvYEyzxNyb6lZXHODmEoJeFu4JupYlkfha1KZpJyoqiJ7pgA1qq8Q==",
-            "requires": {
-                "spdx-expression-parse": "^3.0.0",
-                "spdx-license-ids": "^3.0.0"
-            },
-            "resolved": "https://registry.npmjs.org/spdx-correct/-/spdx-correct-3.1.0.tgz",
-            "version": "3.1.0"
-        },
-        "spdx-exceptions": {
-            "dev": true,
-            "integrity": "sha512-2XQACfElKi9SlVb1CYadKDXvoajPgBVPn/gOQLrTvHdElaVhr7ZEbqJaRnJLVNeaI4cMEAgVCeBMKF6MWRDCRA==",
-            "resolved": "https://registry.npmjs.org/spdx-exceptions/-/spdx-exceptions-2.2.0.tgz",
-            "version": "2.2.0"
-        },
-        "spdx-expression-parse": {
-            "dev": true,
-            "integrity": "sha512-Yg6D3XpRD4kkOmTpdgbUiEJFKghJH03fiC1OPll5h/0sO6neh2jqRDVHOQ4o/LMea0tgCkbMgea5ip/e+MkWyg==",
-            "requires": {
-                "spdx-exceptions": "^2.1.0",
-                "spdx-license-ids": "^3.0.0"
-            },
-            "resolved": "https://registry.npmjs.org/spdx-expression-parse/-/spdx-expression-parse-3.0.0.tgz",
-            "version": "3.0.0"
-        },
-        "spdx-license-ids": {
-            "dev": true,
-            "integrity": "sha512-J+FWzZoynJEXGphVIS+XEh3kFSjZX/1i9gFBaWQcB+/tmpe2qUsSBABpcxqxnAxFdiUFEgAX1bjYGQvIZmoz9Q==",
-            "resolved": "https://registry.npmjs.org/spdx-license-ids/-/spdx-license-ids-3.0.5.tgz",
-            "version": "3.0.5"
-        },
         "split-string": {
             "dev": true,
             "integrity": "sha512-NzNVhJDYpwceVVii8/Hu6DKfD2G+NrQHlS/V/qgv763EYudVwEcMQNxd2lh+0VrUByXN/oJkl5grOhYWvQUYiw==",
             "requires": {
                 "extend-shallow": "^3.0.0"
             },
             "resolved": "https://registry.npmjs.org/split-string/-/split-string-3.1.0.tgz",
@@ -8072,55 +7510,14 @@
         },
         "statuses": {
             "dev": true,
             "integrity": "sha1-Fhx9rBd2Wf2YEfQ3cfqZOBR4Yow=",
             "resolved": "https://registry.npmjs.org/statuses/-/statuses-1.5.0.tgz",
             "version": "1.5.0"
         },
-        "stdout-stream": {
-            "dependencies": {
-                "isarray": {
-                    "dev": true,
-                    "integrity": "sha1-u5NdSFgsuhaMBoNJV6VKPgcSTxE=",
-                    "resolved": "https://registry.npmjs.org/isarray/-/isarray-1.0.0.tgz",
-                    "version": "1.0.0"
-                },
-                "readable-stream": {
-                    "dev": true,
-                    "integrity": "sha512-tQtKA9WIAhBF3+VLAseyMqZeBjW0AHJoxOtYqSUZNJxauErmLbVm2FW1y+J/YA9dUrAC39ITejlZWhVIwawkKw==",
-                    "requires": {
-                        "core-util-is": "~1.0.0",
-                        "inherits": "~2.0.3",
-                        "isarray": "~1.0.0",
-                        "process-nextick-args": "~2.0.0",
-                        "safe-buffer": "~5.1.1",
-                        "string_decoder": "~1.1.1",
-                        "util-deprecate": "~1.0.1"
-                    },
-                    "resolved": "https://registry.npmjs.org/readable-stream/-/readable-stream-2.3.6.tgz",
-                    "version": "2.3.6"
-                },
-                "string_decoder": {
-                    "dev": true,
-                    "integrity": "sha512-n/ShnvDi6FHbbVfviro+WojiFzv+s8MPMHBczVePfUpDJLwoLT0ht1l4YwBCbi8pJAveEEdnkHyPyTP/mzRfwg==",
-                    "requires": {
-                        "safe-buffer": "~5.1.0"
-                    },
-                    "resolved": "https://registry.npmjs.org/string_decoder/-/string_decoder-1.1.1.tgz",
-                    "version": "1.1.1"
-                }
-            },
-            "dev": true,
-            "integrity": "sha512-j4emi03KXqJWcIeF8eIXkjMFN1Cmb8gUlDYGeBALLPo5qdyTfA9bOtl8m33lRoC+vFMkP3gl0WsDr6+gzxbbTA==",
-            "requires": {
-                "readable-stream": "^2.0.1"
-            },
-            "resolved": "https://registry.npmjs.org/stdout-stream/-/stdout-stream-1.4.1.tgz",
-            "version": "1.4.1"
-        },
         "stealthy-require": {
             "dev": true,
             "integrity": "sha1-NbCYdbT/SfJqd35QmzCQoyJr8ks=",
             "resolved": "https://registry.npmjs.org/stealthy-require/-/stealthy-require-1.1.1.tgz",
             "version": "1.1.1"
         },
         "stream-browserify": {
@@ -8286,25 +7683,14 @@
         },
         "symbol-tree": {
             "dev": true,
             "integrity": "sha512-9QNk5KwDF+Bvz+PyObkmSYjI5ksVUYtjW7AU22r2NKcfLJcXp96hkDWU3+XndOsUb+AQ9QhfzfCT2O+CNWT5Tw==",
             "resolved": "https://registry.npmjs.org/symbol-tree/-/symbol-tree-3.2.4.tgz",
             "version": "3.2.4"
         },
-        "tar": {
-            "dev": true,
-            "integrity": "sha512-FCEhQ/4rE1zYv9rYXJw/msRqsnmlje5jHP6huWeBZ704jUTy02c5AZyWujpMR1ax6mVw9NyJMfuK2CMDWVIfgA==",
-            "requires": {
-                "block-stream": "*",
-                "fstream": "^1.0.12",
-                "inherits": "2"
-            },
-            "resolved": "https://registry.npmjs.org/tar/-/tar-2.2.2.tgz",
-            "version": "2.2.2"
-        },
         "terser": {
             "dependencies": {
                 "source-map": {
                     "dev": true,
                     "integrity": "sha512-UjgapumWlbMhkBgzT7Ykc5YXUT46F0iKu8SGXq0bcwP5dz/h0Plj6enJqjz1Zbq2l5WaqYnrVbwWOWMyF3F47g==",
                     "resolved": "https://registry.npmjs.org/source-map/-/source-map-0.6.1.tgz",
                     "version": "0.6.1"
@@ -8472,23 +7858,14 @@
             "integrity": "sha1-qLE/1r/SSJUZZ0zN5VujaTtwbQk=",
             "requires": {
                 "punycode": "^2.1.0"
             },
             "resolved": "https://registry.npmjs.org/tr46/-/tr46-1.0.1.tgz",
             "version": "1.0.1"
         },
-        "true-case-path": {
-            "dev": true,
-            "integrity": "sha512-m6s2OdQe5wgpFMC+pAJ+q9djG82O2jcHPOI6RNg1yy9rCYR+WD6Nbpl32fDpfC56nirdRy+opFa/Vk7HYhqaew==",
-            "requires": {
-                "glob": "^7.1.2"
-            },
-            "resolved": "https://registry.npmjs.org/true-case-path/-/true-case-path-1.0.3.tgz",
-            "version": "1.0.3"
-        },
         "tty-browserify": {
             "dev": true,
             "integrity": "sha1-oVe6QC2iTpv5V/mqadUk7tQpAaY=",
             "resolved": "https://registry.npmjs.org/tty-browserify/-/tty-browserify-0.0.0.tgz",
             "version": "0.0.0"
         },
         "tunnel-agent": {
@@ -8517,19 +7894,14 @@
         },
         "typedarray": {
             "dev": true,
             "integrity": "sha1-hnrHTjhkGHsdPUfZlqeOxciDB3c=",
             "resolved": "https://registry.npmjs.org/typedarray/-/typedarray-0.0.6.tgz",
             "version": "0.0.6"
         },
-        "ua-parser-js": {
-            "integrity": "sha512-+O8/qh/Qj8CgC6eYBVBykMrNtp5Gebn4dlGD/kKXVkJNDwyrAwSIqwz8CDf+tsAIWVycKcku6gIXJ0qwx/ZXaQ==",
-            "resolved": "https://registry.npmjs.org/ua-parser-js/-/ua-parser-js-0.7.21.tgz",
-            "version": "0.7.21"
-        },
         "uncss": {
             "dependencies": {
                 "cssesc": {
                     "dev": true,
                     "integrity": "sha512-/Tb/JcjK111nNScGob5MNtsntNM1aCNUDipB/TkwZFhyDrrE47SOx/18wF2bbjgc3ZzCSKW1T5nt5EbFoAz/Vg==",
                     "resolved": "https://registry.npmjs.org/cssesc/-/cssesc-3.0.0.tgz",
                     "version": "3.0.0"
@@ -8602,19 +7974,14 @@
             "requires": {
                 "pako": "^0.2.5",
                 "tiny-inflate": "^1.0.0"
             },
             "resolved": "https://registry.npmjs.org/unicode-trie/-/unicode-trie-0.3.1.tgz",
             "version": "0.3.1"
         },
-        "union-class-names": {
-            "integrity": "sha1-kllgitrMOQlKKwz+FseOYgBheEc=",
-            "resolved": "https://registry.npmjs.org/union-class-names/-/union-class-names-1.0.0.tgz",
-            "version": "1.0.0"
-        },
         "union-value": {
             "dev": true,
             "integrity": "sha512-tJfXmxMeWYnczCVs7XAEvIV7ieppALdyepWMkHkwciRpZraG/xwT+s2JN8+pr1+8jCRf80FFzvr+MpQeeoF4Xg==",
             "requires": {
                 "arr-union": "^3.1.0",
                 "get-value": "^2.0.6",
                 "is-extendable": "^0.1.1",
@@ -8773,24 +8140,14 @@
         },
         "v8-compile-cache": {
             "dev": true,
             "integrity": "sha512-usZBT3PW+LOjM25wbqIlZwPeJV+3OSz3M1k1Ws8snlW39dZyYL9lOGC5FgPVHfk0jKmjiDV8Z0mIbVQPiwFs7g==",
             "resolved": "https://registry.npmjs.org/v8-compile-cache/-/v8-compile-cache-2.1.0.tgz",
             "version": "2.1.0"
         },
-        "validate-npm-package-license": {
-            "dev": true,
-            "integrity": "sha512-DpKm2Ui/xN7/HQKCtpZxoRWBhZ9Z0kqtygG8XCgNQ8ZlDnxuQmWhj566j8fN4Cu3/JmbhsDo7fcAJq4s9h27Ew==",
-            "requires": {
-                "spdx-correct": "^3.0.0",
-                "spdx-expression-parse": "^3.0.0"
-            },
-            "resolved": "https://registry.npmjs.org/validate-npm-package-license/-/validate-npm-package-license-3.0.4.tgz",
-            "version": "3.0.4"
-        },
         "vendors": {
             "dev": true,
             "integrity": "sha512-fOi47nsJP5Wqefa43kyWSg80qF+Q3XA6MUkgi7Hp1HQaKDQW4cQrK2D0P7mmbFtsV1N89am55Yru/nyEwRubcw==",
             "resolved": "https://registry.npmjs.org/vendors/-/vendors-1.0.3.tgz",
             "version": "1.0.3"
         },
         "verror": {
@@ -8832,22 +8189,14 @@
                 "domexception": "^1.0.1",
                 "webidl-conversions": "^4.0.2",
                 "xml-name-validator": "^3.0.0"
             },
             "resolved": "https://registry.npmjs.org/w3c-xmlserializer/-/w3c-xmlserializer-1.1.2.tgz",
             "version": "1.1.2"
         },
-        "warning": {
-            "integrity": "sha512-rpJyN222KWIvHJ/F53XSZv0Zl/accqHR8et1kpaMTD/fLCRxtV8iX8czMzY7sVZupTI3zcUTg8eycS2kNF9l6w==",
-            "requires": {
-                "loose-envify": "^1.0.0"
-            },
-            "resolved": "https://registry.npmjs.org/warning/-/warning-4.0.3.tgz",
-            "version": "4.0.3"
-        },
         "wcwidth": {
             "dev": true,
             "integrity": "sha1-8LDc+RW8X/FSivrbLA4XtTLaL+g=",
             "requires": {
                 "defaults": "^1.0.3"
             },
             "resolved": "https://registry.npmjs.org/wcwidth/-/wcwidth-1.0.1.tgz",
@@ -8864,19 +8213,14 @@
             "integrity": "sha512-b5lim54JOPN9HtzvK9HFXvBma/rnfFeqsic0hSpjtDbVxR3dJKLc+KB4V6GgiGOvl7CY/KNh8rxSo9DKQrnUEw==",
             "requires": {
                 "iconv-lite": "0.4.24"
             },
             "resolved": "https://registry.npmjs.org/whatwg-encoding/-/whatwg-encoding-1.0.5.tgz",
             "version": "1.0.5"
         },
-        "whatwg-fetch": {
-            "integrity": "sha512-9GSJUgz1D4MfyKU7KRqwOjXCXTqWdFNvEr7eUBYchQiVc744mqK/MzXPNR2WsPkmkOa4ywfg8C2n8h+13Bey1Q==",
-            "resolved": "https://registry.npmjs.org/whatwg-fetch/-/whatwg-fetch-3.0.0.tgz",
-            "version": "3.0.0"
-        },
         "whatwg-mimetype": {
             "dev": true,
             "integrity": "sha512-M4yMwr6mAnQz76TbJm914+gPpB/nCwvZbJU28cUD6dR004SAxDLOOSUaB1JDRqLtaOV/vi0IC5lEAGFgrjGv/g==",
             "resolved": "https://registry.npmjs.org/whatwg-mimetype/-/whatwg-mimetype-2.3.0.tgz",
             "version": "2.3.0"
         },
         "whatwg-url": {
@@ -8895,115 +8239,20 @@
             "integrity": "sha512-HxJdYWq1MTIQbJ3nw0cqssHoTNU267KlrDuGZ1WYlxDStUtKUhOaJmh112/TZmHxxUfuJqPXSOm7tDyas0OSIQ==",
             "requires": {
                 "isexe": "^2.0.0"
             },
             "resolved": "https://registry.npmjs.org/which/-/which-1.3.1.tgz",
             "version": "1.3.1"
         },
-        "which-module": {
-            "dev": true,
-            "integrity": "sha1-u6Y8qGGUiZT/MHc2CJ47lgJsKk8=",
-            "resolved": "https://registry.npmjs.org/which-module/-/which-module-1.0.0.tgz",
-            "version": "1.0.0"
-        },
-        "wide-align": {
-            "dependencies": {
-                "ansi-regex": {
-                    "dev": true,
-                    "integrity": "sha1-7QMXwyIGT3lGbAKWa922Bas32Zg=",
-                    "resolved": "https://registry.npmjs.org/ansi-regex/-/ansi-regex-3.0.0.tgz",
-                    "version": "3.0.0"
-                },
-                "is-fullwidth-code-point": {
-                    "dev": true,
-                    "integrity": "sha1-o7MKXE8ZkYMWeqq5O+764937ZU8=",
-                    "resolved": "https://registry.npmjs.org/is-fullwidth-code-point/-/is-fullwidth-code-point-2.0.0.tgz",
-                    "version": "2.0.0"
-                },
-                "string-width": {
-                    "dev": true,
-                    "integrity": "sha512-nOqH59deCq9SRHlxq1Aw85Jnt4w6KvLKqWVik6oA9ZklXLNIOlqg4F2yrT1MVaTjAqvVwdfeZ7w7aCvJD7ugkw==",
-                    "requires": {
-                        "is-fullwidth-code-point": "^2.0.0",
-                        "strip-ansi": "^4.0.0"
-                    },
-                    "resolved": "https://registry.npmjs.org/string-width/-/string-width-2.1.1.tgz",
-                    "version": "2.1.1"
-                },
-                "strip-ansi": {
-                    "dev": true,
-                    "integrity": "sha1-qEeQIusaw2iocTibY1JixQXuNo8=",
-                    "requires": {
-                        "ansi-regex": "^3.0.0"
-                    },
-                    "resolved": "https://registry.npmjs.org/strip-ansi/-/strip-ansi-4.0.0.tgz",
-                    "version": "4.0.0"
-                }
-            },
-            "dev": true,
-            "integrity": "sha512-QGkOQc8XL6Bt5PwnsExKBPuMKBxnGxWWW3fU55Xt4feHozMUhdUMaBCk290qpm/wG5u/RSKzwdAC4i51YigihA==",
-            "requires": {
-                "string-width": "^1.0.2 || 2"
-            },
-            "resolved": "https://registry.npmjs.org/wide-align/-/wide-align-1.1.3.tgz",
-            "version": "1.1.3"
-        },
         "word-wrap": {
             "dev": true,
             "integrity": "sha512-Hz/mrNwitNRh/HUAtM/VT/5VH+ygD6DV7mYKZAtHOrbs8U7lvPS6xf7EJKMF0uW1KJCl0H701g3ZGus+muE5vQ==",
             "resolved": "https://registry.npmjs.org/word-wrap/-/word-wrap-1.2.3.tgz",
             "version": "1.2.3"
         },
-        "wrap-ansi": {
-            "dependencies": {
-                "ansi-regex": {
-                    "dev": true,
-                    "integrity": "sha1-w7M6te42DYbg5ijwRorn7yfWVN8=",
-                    "resolved": "https://registry.npmjs.org/ansi-regex/-/ansi-regex-2.1.1.tgz",
-                    "version": "2.1.1"
-                },
-                "is-fullwidth-code-point": {
-                    "dev": true,
-                    "integrity": "sha1-754xOG8DGn8NZDr4L95QxFfvAMs=",
-                    "requires": {
-                        "number-is-nan": "^1.0.0"
-                    },
-                    "resolved": "https://registry.npmjs.org/is-fullwidth-code-point/-/is-fullwidth-code-point-1.0.0.tgz",
-                    "version": "1.0.0"
-                },
-                "string-width": {
-                    "dev": true,
-                    "integrity": "sha1-EYvfW4zcUaKn5w0hHgfisLmxB9M=",
-                    "requires": {
-                        "code-point-at": "^1.0.0",
-                        "is-fullwidth-code-point": "^1.0.0",
-                        "strip-ansi": "^3.0.0"
-                    },
-                    "resolved": "https://registry.npmjs.org/string-width/-/string-width-1.0.2.tgz",
-                    "version": "1.0.2"
-                },
-                "strip-ansi": {
-                    "dev": true,
-                    "integrity": "sha1-ajhfuIU9lS1f8F0Oiq+UJ43GPc8=",
-                    "requires": {
-                        "ansi-regex": "^2.0.0"
-                    },
-                    "resolved": "https://registry.npmjs.org/strip-ansi/-/strip-ansi-3.0.1.tgz",
-                    "version": "3.0.1"
-                }
-            },
-            "dev": true,
-            "integrity": "sha1-2Pw9KE3QV5T+hJc8rs3Rz4JP3YU=",
-            "requires": {
-                "string-width": "^1.0.1",
-                "strip-ansi": "^3.0.1"
-            },
-            "resolved": "https://registry.npmjs.org/wrap-ansi/-/wrap-ansi-2.1.0.tgz",
-            "version": "2.1.0"
-        },
         "wrappy": {
             "dev": true,
             "integrity": "sha1-tSQ9jz7BqjXxNkYFvA0QNuMKtp8=",
             "resolved": "https://registry.npmjs.org/wrappy/-/wrappy-1.0.2.tgz",
             "version": "1.0.2"
         },
         "ws": {
@@ -9029,186 +8278,23 @@
         },
         "xtend": {
             "dev": true,
             "integrity": "sha512-LKYU1iAXJXUgAXn9URjiu+MWhyUXHsvfp7mcuYm9dSUKK0/CjtrUwFAxD82/mCWbtLsGjFIad0wIsod4zrTAEQ==",
             "resolved": "https://registry.npmjs.org/xtend/-/xtend-4.0.2.tgz",
             "version": "4.0.2"
         },
-        "y18n": {
+        "yargs-parser": {
             "dev": true,
-            "integrity": "sha1-bRX7qITAhnnA136I53WegR4H+kE=",
-            "resolved": "https://registry.npmjs.org/y18n/-/y18n-3.2.1.tgz",
-            "version": "3.2.1"
-        },
-        "yallist": {
-            "dev": true,
-            "integrity": "sha1-HBH5IY8HYImkfdUS+TxmmaaoHVI=",
-            "resolved": "https://registry.npmjs.org/yallist/-/yallist-2.1.2.tgz",
-            "version": "2.1.2"
-        },
-        "yargs": {
-            "dependencies": {
-                "ansi-regex": {
-                    "dev": true,
-                    "integrity": "sha1-w7M6te42DYbg5ijwRorn7yfWVN8=",
-                    "resolved": "https://registry.npmjs.org/ansi-regex/-/ansi-regex-2.1.1.tgz",
-                    "version": "2.1.1"
-                },
-                "camelcase": {
-                    "dev": true,
-                    "integrity": "sha1-MvxLn82vhF/N9+c7uXysImHwqwo=",
-                    "resolved": "https://registry.npmjs.org/camelcase/-/camelcase-3.0.0.tgz",
-                    "version": "3.0.0"
-                },
-                "find-up": {
-                    "dev": true,
-                    "integrity": "sha1-ay6YIrGizgpgq2TWEOzK1TyyTQ8=",
-                    "requires": {
-                        "path-exists": "^2.0.0",
-                        "pinkie-promise": "^2.0.0"
-                    },
-                    "resolved": "https://registry.npmjs.org/find-up/-/find-up-1.1.2.tgz",
-                    "version": "1.1.2"
-                },
-                "is-fullwidth-code-point": {
-                    "dev": true,
-                    "integrity": "sha1-754xOG8DGn8NZDr4L95QxFfvAMs=",
-                    "requires": {
-                        "number-is-nan": "^1.0.0"
-                    },
-                    "resolved": "https://registry.npmjs.org/is-fullwidth-code-point/-/is-fullwidth-code-point-1.0.0.tgz",
-                    "version": "1.0.0"
-                },
-                "load-json-file": {
-                    "dev": true,
-                    "integrity": "sha1-lWkFcI1YtLq0wiYbBPWfMcmTdMA=",
-                    "requires": {
-                        "graceful-fs": "^4.1.2",
-                        "parse-json": "^2.2.0",
-                        "pify": "^2.0.0",
-                        "pinkie-promise": "^2.0.0",
-                        "strip-bom": "^2.0.0"
-                    },
-                    "resolved": "https://registry.npmjs.org/load-json-file/-/load-json-file-1.1.0.tgz",
-                    "version": "1.1.0"
-                },
-                "parse-json": {
-                    "dev": true,
-                    "integrity": "sha1-9ID0BDTvgHQfhGkJn43qGPVaTck=",
-                    "requires": {
-                        "error-ex": "^1.2.0"
-                    },
-                    "resolved": "https://registry.npmjs.org/parse-json/-/parse-json-2.2.0.tgz",
-                    "version": "2.2.0"
-                },
-                "path-exists": {
-                    "dev": true,
-                    "integrity": "sha1-D+tsZPD8UY2adU3V77YscCJ2H0s=",
-                    "requires": {
-                        "pinkie-promise": "^2.0.0"
-                    },
-                    "resolved": "https://registry.npmjs.org/path-exists/-/path-exists-2.1.0.tgz",
-                    "version": "2.1.0"
-                },
-                "path-type": {
-                    "dev": true,
-                    "integrity": "sha1-WcRPfuSR2nBNpBXaWkBwuk+P5EE=",
-                    "requires": {
-                        "graceful-fs": "^4.1.2",
-                        "pify": "^2.0.0",
-                        "pinkie-promise": "^2.0.0"
-                    },
-                    "resolved": "https://registry.npmjs.org/path-type/-/path-type-1.1.0.tgz",
-                    "version": "1.1.0"
-                },
-                "pify": {
-                    "dev": true,
-                    "integrity": "sha1-7RQaasBDqEnqWISY59yosVMw6Qw=",
-                    "resolved": "https://registry.npmjs.org/pify/-/pify-2.3.0.tgz",
-                    "version": "2.3.0"
-                },
-                "read-pkg": {
-                    "dev": true,
-                    "integrity": "sha1-9f+qXs0pyzHAR0vKfXVra7KePyg=",
-                    "requires": {
-                        "load-json-file": "^1.0.0",
-                        "normalize-package-data": "^2.3.2",
-                        "path-type": "^1.0.0"
-                    },
-                    "resolved": "https://registry.npmjs.org/read-pkg/-/read-pkg-1.1.0.tgz",
-                    "version": "1.1.0"
-                },
-                "read-pkg-up": {
-                    "dev": true,
-                    "integrity": "sha1-nWPBMnbAZZGNV/ACpX9AobZD+wI=",
-                    "requires": {
-                        "find-up": "^1.0.0",
-                        "read-pkg": "^1.0.0"
-                    },
-                    "resolved": "https://registry.npmjs.org/read-pkg-up/-/read-pkg-up-1.0.1.tgz",
-                    "version": "1.0.1"
-                },
-                "string-width": {
-                    "dev": true,
-                    "integrity": "sha1-EYvfW4zcUaKn5w0hHgfisLmxB9M=",
-                    "requires": {
-                        "code-point-at": "^1.0.0",
-                        "is-fullwidth-code-point": "^1.0.0",
-                        "strip-ansi": "^3.0.0"
-                    },
-                    "resolved": "https://registry.npmjs.org/string-width/-/string-width-1.0.2.tgz",
-                    "version": "1.0.2"
-                },
-                "strip-ansi": {
-                    "dev": true,
-                    "integrity": "sha1-ajhfuIU9lS1f8F0Oiq+UJ43GPc8=",
-                    "requires": {
-                        "ansi-regex": "^2.0.0"
-                    },
-                    "resolved": "https://registry.npmjs.org/strip-ansi/-/strip-ansi-3.0.1.tgz",
-                    "version": "3.0.1"
-                },
-                "strip-bom": {
-                    "dev": true,
-                    "integrity": "sha1-YhmoVhZSBJHzV4i9vxRHqZx+aw4=",
-                    "requires": {
-                        "is-utf8": "^0.2.0"
-                    },
-                    "resolved": "https://registry.npmjs.org/strip-bom/-/strip-bom-2.0.0.tgz",
-                    "version": "2.0.0"
-                },
-                "yargs-parser": {
-                    "dev": true,
-                    "integrity": "sha1-J17PDX/+Bcd+ZOfIbkzZS/DhIoo=",
-                    "requires": {
-                        "camelcase": "^3.0.0"
-                    },
-                    "resolved": "https://registry.npmjs.org/yargs-parser/-/yargs-parser-5.0.0.tgz",
-                    "version": "5.0.0"
-                }
-            },
-            "dev": true,
-            "integrity": "sha1-a6MY6xaWFyf10oT46gA+jWFU0Mg=",
+            "integrity": "sha512-0OAMV2mAZQrs3FkNpDQcBk1x5HXb8X4twADss4S0Iuk+2dGnLOE/fRHrsYm542GduMveyA77OF4wrNJuanRCWw==",
             "requires": {
-                "camelcase": "^3.0.0",
-                "cliui": "^3.2.0",
-                "decamelize": "^1.1.1",
-                "get-caller-file": "^1.0.1",
-                "os-locale": "^1.4.0",
-                "read-pkg-up": "^1.0.1",
-                "require-directory": "^2.1.1",
-                "require-main-filename": "^1.0.1",
-                "set-blocking": "^2.0.0",
-                "string-width": "^1.0.2",
-                "which-module": "^1.0.0",
-                "y18n": "^3.2.1",
-                "yargs-parser": "^5.0.0"
+                "camelcase": "^5.0.0",
+                "decamelize": "^1.2.0"
             },
-            "resolved": "https://registry.npmjs.org/yargs/-/yargs-7.1.0.tgz",
-            "version": "7.1.0"
+            "resolved": "https://registry.npmjs.org/yargs-parser/-/yargs-parser-15.0.1.tgz",
+            "version": "15.0.1"
         }
     },
     "lockfileVersion": 1,
     "name": "static_src",
     "requires": true,
     "version": "1.0.0"
 }
```

### Comparing `non_admin_draftail-0.4.1/PKG-INFO` & `non_admin_draftail-0.9.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 Metadata-Version: 2.1
 Name: non-admin-draftail
-Version: 0.4.1
+Version: 0.9.0
 Summary: You can now use Wagtail Draftail editor on non-admin pages
 Home-page: https://timonweb.com
 License: MIT
 Author: Tim Kamanin
 Author-email: tim@timonweb.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Requires-Dist: django (>=2.2,<3.2)
+Requires-Dist: wagtail (>=2.8,<2.11)
 Project-URL: Repository, https://github.com/timonweb/non-admin-draftail
```

