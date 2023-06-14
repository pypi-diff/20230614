# Comparing `tmp/sentry_cli-2.18.1.tar.gz` & `tmp/sentry_cli-2.19.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sentry_cli-2.18.1.tar", last modified: Mon May 22 14:51:37 2023, max compression
+gzip compressed data, was "sentry_cli-2.19.0.tar", last modified: Wed Jun 14 08:24:55 2023, max compression
```

## Comparing `sentry_cli-2.18.1.tar` & `sentry_cli-2.19.0.tar`

### file list

```diff
@@ -1,129 +1,129 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 14:51:37.271726 sentry_cli-2.18.1/
--rw-r--r--   0 runner    (1001) docker     (123)    80821 2023-05-22 14:51:19.000000 sentry_cli-2.18.1/Cargo.lock
--rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-05-22 14:51:19.000000 sentry_cli-2.18.1/Cargo.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-05-22 14:51:19.000000 sentry_cli-2.18.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-22 14:51:19.000000 sentry_cli-2.18.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5915 2023-05-22 14:51:37.271726 sentry_cli-2.18.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5309 2023-05-22 14:51:19.000000 sentry_cli-2.18.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-05-22 14:51:19.000000 sentry_cli-2.18.1/build.rs
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-22 14:51:19.000000 sentry_cli-2.18.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 14:51:37.259726 sentry_cli-2.18.1/sentry_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5915 2023-05-22 14:51:37.000000 sentry_cli-2.18.1/sentry_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3065 2023-05-22 14:51:37.000000 sentry_cli-2.18.1/sentry_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 14:51:37.000000 sentry_cli-2.18.1/sentry_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 14:51:37.000000 sentry_cli-2.18.1/sentry_cli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-05-22 14:51:37.275726 sentry_cli-2.18.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-05-22 14:51:19.000000 sentry_cli-2.18.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 14:51:37.259726 sentry_cli-2.18.1/src/
--rw-r--r--   0 runner    (1001) docker     (123)    87498 2023-05-22 14:51:19.000000 sentry_cli-2.18.1/src/api.rs
--rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-05-22 14:51:19.000000 sentry_cli-2.18.1/src/bashsupport.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 14:51:37.259726 sentry_cli-2.18.1/src/commands/
--rw-r--r--   0 runner    (1001) docker     (123)     8173 2023-05-22 14:51:19.000000 sentry_cli-2.18.1/src/commands/bash_hook.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 14:51:37.263726 sentry_cli-2.18.1/src/commands/debug_files/
--rw-r--r--   0 runner    (1001) docker     (123)     3813 2023-05-22 14:51:19.000000 sentry_cli-2.18.1/src/commands/debug_files/bundle_jvm.rs
--rw-r--r--   0 runner    (1001) docker     (123)     3879 2023-05-22 14:51:19.000000 sentry_cli-2.18.1/src/commands/debug_files/bundle_sources.rs
--rw-r--r--   0 runner    (1001) docker     (123)     3032 2023-05-22 14:51:19.000000 sentry_cli-2.18.1/src/commands/debug_files/check.rs
--rw-r--r--   0 runner    (1001) docker     (123)    11579 2023-05-22 14:51:19.000000 sentry_cli-2.18.1/src/commands/debug_files/find.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-05-22 14:51:19.000000 sentry_cli-2.18.1/src/commands/debug_files/mod.rs
--rw-r--r--   0 runner    (1001) docker     (123)     3202 2023-05-22 14:51:19.000000 sentry_cli-2.18.1/src/commands/debug_files/print_sources.rs
--rw-r--r--   0 runner    (1001) docker     (123)    14830 2023-05-22 14:51:19.000000 sentry_cli-2.18.1/src/commands/debug_files/upload.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 14:51:37.263726 sentry_cli-2.18.1/src/commands/deploys/
--rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-05-22 14:51:19.000000 sentry_cli-2.18.1/src/commands/deploys/list.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-05-22 14:51:19.000000 sentry_cli-2.18.1/src/commands/deploys/mod.rs
--rw-r--r--   0 runner    (1001) docker     (123)     3457 2023-05-22 14:51:19.000000 sentry_cli-2.18.1/src/commands/deploys/new.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 14:51:37.263726 sentry_cli-2.18.1/src/commands/events/
--rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-05-22 14:51:19.000000 sentry_cli-2.18.1/src/commands/events/list.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-05-22 14:51:19.000000 sentry_cli-2.18.1/src/commands/events/mod.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 14:51:37.263726 sentry_cli-2.18.1/src/commands/files/
--rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-05-22 14:51:19.000000 sentry_cli-2.18.1/src/commands/files/delete.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-05-22 14:51:19.000000 sentry_cli-2.18.1/src/commands/files/list.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-05-22 14:51:19.000000 sentry_cli-2.18.1/src/commands/files/mod.rs
--rw-r--r--   0 runner    (1001) docker     (123)     8183 2023-05-22 14:51:19.000000 sentry_cli-2.18.1/src/commands/files/upload.rs
--rw-r--r--   0 runner    (1001) docker     (123)     4277 2023-05-22 14:51:19.000000 sentry_cli-2.18.1/src/commands/info.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 14:51:37.263726 sentry_cli-2.18.1/src/commands/issues/
--rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-05-22 14:51:19.000000 sentry_cli-2.18.1/src/commands/issues/mod.rs
--rw-r--r--   0 runner    (1001) docker     (123)      994 2023-05-22 14:51:19.000000 sentry_cli-2.18.1/src/commands/issues/mute.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-05-22 14:51:19.000000 sentry_cli-2.18.1/src/commands/issues/resolve.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-05-22 14:51:19.000000 sentry_cli-2.18.1/src/commands/issues/unresolve.rs
--rw-r--r--   0 runner    (1001) docker     (123)     3184 2023-05-22 14:51:19.000000 sentry_cli-2.18.1/src/commands/login.rs
--rw-r--r--   0 runner    (1001) docker     (123)     9055 2023-05-22 14:51:19.000000 sentry_cli-2.18.1/src/commands/mod.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 14:51:37.263726 sentry_cli-2.18.1/src/commands/monitors/
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-05-22 14:51:19.000000 sentry_cli-2.18.1/src/commands/monitors/list.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-05-22 14:51:19.000000 sentry_cli-2.18.1/src/commands/monitors/mod.rs
--rw-r--r--   0 runner    (1001) docker     (123)     3828 2023-05-22 14:51:19.000000 sentry_cli-2.18.1/src/commands/monitors/run.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 14:51:37.263726 sentry_cli-2.18.1/src/commands/organizations/
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-05-22 14:51:19.000000 sentry_cli-2.18.1/src/commands/organizations/list.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-05-22 14:51:19.000000 sentry_cli-2.18.1/src/commands/organizations/mod.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 14:51:37.263726 sentry_cli-2.18.1/src/commands/projects/
--rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-05-22 14:51:19.000000 sentry_cli-2.18.1/src/commands/projects/list.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-05-22 14:51:19.000000 sentry_cli-2.18.1/src/commands/projects/mod.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 14:51:37.263726 sentry_cli-2.18.1/src/commands/react_native/
--rw-r--r--   0 runner    (1001) docker     (123)     7090 2023-05-22 14:51:19.000000 sentry_cli-2.18.1/src/commands/react_native/appcenter.rs
--rw-r--r--   0 runner    (1001) docker     (123)     4111 2023-05-22 14:51:19.000000 sentry_cli-2.18.1/src/commands/react_native/gradle.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-05-22 14:51:19.000000 sentry_cli-2.18.1/src/commands/react_native/mod.rs
--rw-r--r--   0 runner    (1001) docker     (123)    14288 2023-05-22 14:51:19.000000 sentry_cli-2.18.1/src/commands/react_native/xcode.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 14:51:37.267726 sentry_cli-2.18.1/src/commands/releases/
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-05-22 14:51:19.000000 sentry_cli-2.18.1/src/commands/releases/archive.rs
--rw-r--r--   0 runner    (1001) docker     (123)      791 2023-05-22 14:51:19.000000 sentry_cli-2.18.1/src/commands/releases/delete.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-05-22 14:51:19.000000 sentry_cli-2.18.1/src/commands/releases/finalize.rs
--rw-r--r--   0 runner    (1001) docker     (123)     3160 2023-05-22 14:51:19.000000 sentry_cli-2.18.1/src/commands/releases/info.rs
--rw-r--r--   0 runner    (1001) docker     (123)     3300 2023-05-22 14:51:19.000000 sentry_cli-2.18.1/src/commands/releases/list.rs
--rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-05-22 14:51:19.000000 sentry_cli-2.18.1/src/commands/releases/mod.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-05-22 14:51:19.000000 sentry_cli-2.18.1/src/commands/releases/new.rs
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-05-22 14:51:19.000000 sentry_cli-2.18.1/src/commands/releases/propose_version.rs
--rw-r--r--   0 runner    (1001) docker     (123)      881 2023-05-22 14:51:19.000000 sentry_cli-2.18.1/src/commands/releases/restore.rs
--rw-r--r--   0 runner    (1001) docker     (123)     8411 2023-05-22 14:51:19.000000 sentry_cli-2.18.1/src/commands/releases/set_commits.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 14:51:37.267726 sentry_cli-2.18.1/src/commands/repos/
--rw-r--r--   0 runner    (1001) docker     (123)      877 2023-05-22 14:51:19.000000 sentry_cli-2.18.1/src/commands/repos/list.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-05-22 14:51:19.000000 sentry_cli-2.18.1/src/commands/repos/mod.rs
--rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-05-22 14:51:19.000000 sentry_cli-2.18.1/src/commands/send_envelope.rs
--rw-r--r--   0 runner    (1001) docker     (123)    11841 2023-05-22 14:51:19.000000 sentry_cli-2.18.1/src/commands/send_event.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 14:51:37.267726 sentry_cli-2.18.1/src/commands/sourcemaps/
--rw-r--r--   0 runner    (1001) docker     (123)    16362 2023-05-22 14:51:19.000000 sentry_cli-2.18.1/src/commands/sourcemaps/explain.rs
--rw-r--r--   0 runner    (1001) docker     (123)     3984 2023-05-22 14:51:19.000000 sentry_cli-2.18.1/src/commands/sourcemaps/inject.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-05-22 14:51:19.000000 sentry_cli-2.18.1/src/commands/sourcemaps/mod.rs
--rw-r--r--   0 runner    (1001) docker     (123)     3737 2023-05-22 14:51:19.000000 sentry_cli-2.18.1/src/commands/sourcemaps/resolve.rs
--rw-r--r--   0 runner    (1001) docker     (123)    14882 2023-05-22 14:51:19.000000 sentry_cli-2.18.1/src/commands/sourcemaps/upload.rs
--rw-r--r--   0 runner    (1001) docker     (123)     2532 2023-05-22 14:51:19.000000 sentry_cli-2.18.1/src/commands/uninstall.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-05-22 14:51:19.000000 sentry_cli-2.18.1/src/commands/update.rs
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-05-22 14:51:19.000000 sentry_cli-2.18.1/src/commands/upload_dif.rs
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-05-22 14:51:19.000000 sentry_cli-2.18.1/src/commands/upload_dsym.rs
--rw-r--r--   0 runner    (1001) docker     (123)    10733 2023-05-22 14:51:19.000000 sentry_cli-2.18.1/src/commands/upload_proguard.rs
--rw-r--r--   0 runner    (1001) docker     (123)    20882 2023-05-22 14:51:19.000000 sentry_cli-2.18.1/src/config.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-05-22 14:51:19.000000 sentry_cli-2.18.1/src/constants.rs
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-05-22 14:51:19.000000 sentry_cli-2.18.1/src/main.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 14:51:37.271726 sentry_cli-2.18.1/src/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-05-22 14:51:19.000000 sentry_cli-2.18.1/src/utils/android.rs
--rw-r--r--   0 runner    (1001) docker     (123)     8095 2023-05-22 14:51:19.000000 sentry_cli-2.18.1/src/utils/appcenter.rs
--rw-r--r--   0 runner    (1001) docker     (123)     4129 2023-05-22 14:51:19.000000 sentry_cli-2.18.1/src/utils/args.rs
--rw-r--r--   0 runner    (1001) docker     (123)     7299 2023-05-22 14:51:19.000000 sentry_cli-2.18.1/src/utils/chunks.rs
--rw-r--r--   0 runner    (1001) docker     (123)     4543 2023-05-22 14:51:19.000000 sentry_cli-2.18.1/src/utils/codepush.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-05-22 14:51:19.000000 sentry_cli-2.18.1/src/utils/cordova.rs
--rw-r--r--   0 runner    (1001) docker     (123)    14695 2023-05-22 14:51:19.000000 sentry_cli-2.18.1/src/utils/dif.rs
--rw-r--r--   0 runner    (1001) docker     (123)    72730 2023-05-22 14:51:19.000000 sentry_cli-2.18.1/src/utils/dif_upload.rs
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-22 14:51:19.000000 sentry_cli-2.18.1/src/utils/enc.rs
--rw-r--r--   0 runner    (1001) docker     (123)     3132 2023-05-22 14:51:19.000000 sentry_cli-2.18.1/src/utils/event.rs
--rw-r--r--   0 runner    (1001) docker     (123)     5531 2023-05-22 14:51:19.000000 sentry_cli-2.18.1/src/utils/file_search.rs
--rw-r--r--   0 runner    (1001) docker     (123)    17036 2023-05-22 14:51:19.000000 sentry_cli-2.18.1/src/utils/file_upload.rs
--rw-r--r--   0 runner    (1001) docker     (123)     2486 2023-05-22 14:51:19.000000 sentry_cli-2.18.1/src/utils/formatting.rs
--rw-r--r--   0 runner    (1001) docker     (123)     6695 2023-05-22 14:51:19.000000 sentry_cli-2.18.1/src/utils/fs.rs
--rw-r--r--   0 runner    (1001) docker     (123)     3222 2023-05-22 14:51:19.000000 sentry_cli-2.18.1/src/utils/http.rs
--rw-r--r--   0 runner    (1001) docker     (123)     3655 2023-05-22 14:51:19.000000 sentry_cli-2.18.1/src/utils/logging.rs
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-05-22 14:51:19.000000 sentry_cli-2.18.1/src/utils/mod.rs
--rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-05-22 14:51:19.000000 sentry_cli-2.18.1/src/utils/progress.rs
--rw-r--r--   0 runner    (1001) docker     (123)     4884 2023-05-22 14:51:19.000000 sentry_cli-2.18.1/src/utils/releases.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-05-22 14:51:19.000000 sentry_cli-2.18.1/src/utils/retry.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 14:51:37.271726 sentry_cli-2.18.1/src/utils/snapshots/
--rw-r--r--   0 runner    (1001) docker     (123)     4343 2023-05-22 14:51:19.000000 sentry_cli-2.18.1/src/utils/snapshots/sentry_cli__utils__vcs__generate_patch_default_twenty.snap
--rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-05-22 14:51:19.000000 sentry_cli-2.18.1/src/utils/snapshots/sentry_cli__utils__vcs__generate_patch_ignore_missing.snap
--rw-r--r--   0 runner    (1001) docker     (123)      693 2023-05-22 14:51:19.000000 sentry_cli-2.18.1/src/utils/snapshots/sentry_cli__utils__vcs__generate_patch_set_base.snap
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-05-22 14:51:19.000000 sentry_cli-2.18.1/src/utils/snapshots/sentry_cli__utils__vcs__generate_patch_set_previous_commit.snap
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-05-22 14:51:19.000000 sentry_cli-2.18.1/src/utils/snapshots/sentry_cli__utils__vcs__get_commits_from_git.snap
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 14:51:37.271726 sentry_cli-2.18.1/src/utils/sourcemaps/
--rw-r--r--   0 runner    (1001) docker     (123)    11403 2023-05-22 14:51:19.000000 sentry_cli-2.18.1/src/utils/sourcemaps/inject.rs
--rw-r--r--   0 runner    (1001) docker     (123)    36411 2023-05-22 14:51:19.000000 sentry_cli-2.18.1/src/utils/sourcemaps.rs
--rw-r--r--   0 runner    (1001) docker     (123)     4888 2023-05-22 14:51:19.000000 sentry_cli-2.18.1/src/utils/system.rs
--rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-05-22 14:51:19.000000 sentry_cli-2.18.1/src/utils/ui.rs
--rw-r--r--   0 runner    (1001) docker     (123)     8628 2023-05-22 14:51:19.000000 sentry_cli-2.18.1/src/utils/update.rs
--rw-r--r--   0 runner    (1001) docker     (123)    36048 2023-05-22 14:51:19.000000 sentry_cli-2.18.1/src/utils/vcs.rs
--rw-r--r--   0 runner    (1001) docker     (123)    19150 2023-05-22 14:51:19.000000 sentry_cli-2.18.1/src/utils/xcode.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 08:24:55.784309 sentry_cli-2.19.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    80839 2023-06-14 08:24:12.000000 sentry_cli-2.19.0/Cargo.lock
+-rw-r--r--   0 runner    (1001) docker     (123)     2736 2023-06-14 08:24:12.000000 sentry_cli-2.19.0/Cargo.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-06-14 08:24:12.000000 sentry_cli-2.19.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-14 08:24:12.000000 sentry_cli-2.19.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5915 2023-06-14 08:24:55.784309 sentry_cli-2.19.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5309 2023-06-14 08:24:12.000000 sentry_cli-2.19.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-06-14 08:24:12.000000 sentry_cli-2.19.0/build.rs
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-14 08:24:12.000000 sentry_cli-2.19.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 08:24:55.768309 sentry_cli-2.19.0/sentry_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5915 2023-06-14 08:24:55.000000 sentry_cli-2.19.0/sentry_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3065 2023-06-14 08:24:55.000000 sentry_cli-2.19.0/sentry_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 08:24:55.000000 sentry_cli-2.19.0/sentry_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 08:24:55.000000 sentry_cli-2.19.0/sentry_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-06-14 08:24:55.788309 sentry_cli-2.19.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-06-14 08:24:12.000000 sentry_cli-2.19.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 08:24:55.768309 sentry_cli-2.19.0/src/
+-rw-r--r--   0 runner    (1001) docker     (123)    87192 2023-06-14 08:24:12.000000 sentry_cli-2.19.0/src/api.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-06-14 08:24:12.000000 sentry_cli-2.19.0/src/bashsupport.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 08:24:55.768309 sentry_cli-2.19.0/src/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)     8173 2023-06-14 08:24:12.000000 sentry_cli-2.19.0/src/commands/bash_hook.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 08:24:55.772309 sentry_cli-2.19.0/src/commands/debug_files/
+-rw-r--r--   0 runner    (1001) docker     (123)     3813 2023-06-14 08:24:12.000000 sentry_cli-2.19.0/src/commands/debug_files/bundle_jvm.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     3879 2023-06-14 08:24:12.000000 sentry_cli-2.19.0/src/commands/debug_files/bundle_sources.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     3032 2023-06-14 08:24:12.000000 sentry_cli-2.19.0/src/commands/debug_files/check.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    11579 2023-06-14 08:24:12.000000 sentry_cli-2.19.0/src/commands/debug_files/find.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-06-14 08:24:12.000000 sentry_cli-2.19.0/src/commands/debug_files/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     3202 2023-06-14 08:24:12.000000 sentry_cli-2.19.0/src/commands/debug_files/print_sources.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    14830 2023-06-14 08:24:12.000000 sentry_cli-2.19.0/src/commands/debug_files/upload.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 08:24:55.772309 sentry_cli-2.19.0/src/commands/deploys/
+-rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-06-14 08:24:12.000000 sentry_cli-2.19.0/src/commands/deploys/list.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-06-14 08:24:12.000000 sentry_cli-2.19.0/src/commands/deploys/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     3457 2023-06-14 08:24:12.000000 sentry_cli-2.19.0/src/commands/deploys/new.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 08:24:55.772309 sentry_cli-2.19.0/src/commands/events/
+-rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-06-14 08:24:12.000000 sentry_cli-2.19.0/src/commands/events/list.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-06-14 08:24:12.000000 sentry_cli-2.19.0/src/commands/events/mod.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 08:24:55.772309 sentry_cli-2.19.0/src/commands/files/
+-rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-06-14 08:24:12.000000 sentry_cli-2.19.0/src/commands/files/delete.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-06-14 08:24:12.000000 sentry_cli-2.19.0/src/commands/files/list.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-06-14 08:24:12.000000 sentry_cli-2.19.0/src/commands/files/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     8183 2023-06-14 08:24:12.000000 sentry_cli-2.19.0/src/commands/files/upload.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     4277 2023-06-14 08:24:12.000000 sentry_cli-2.19.0/src/commands/info.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 08:24:55.772309 sentry_cli-2.19.0/src/commands/issues/
+-rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-06-14 08:24:12.000000 sentry_cli-2.19.0/src/commands/issues/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-06-14 08:24:12.000000 sentry_cli-2.19.0/src/commands/issues/mute.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-06-14 08:24:12.000000 sentry_cli-2.19.0/src/commands/issues/resolve.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-06-14 08:24:12.000000 sentry_cli-2.19.0/src/commands/issues/unresolve.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     3184 2023-06-14 08:24:12.000000 sentry_cli-2.19.0/src/commands/login.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     9055 2023-06-14 08:24:12.000000 sentry_cli-2.19.0/src/commands/mod.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 08:24:55.776309 sentry_cli-2.19.0/src/commands/monitors/
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-06-14 08:24:12.000000 sentry_cli-2.19.0/src/commands/monitors/list.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-06-14 08:24:12.000000 sentry_cli-2.19.0/src/commands/monitors/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     5935 2023-06-14 08:24:12.000000 sentry_cli-2.19.0/src/commands/monitors/run.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 08:24:55.776309 sentry_cli-2.19.0/src/commands/organizations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-06-14 08:24:12.000000 sentry_cli-2.19.0/src/commands/organizations/list.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-06-14 08:24:12.000000 sentry_cli-2.19.0/src/commands/organizations/mod.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 08:24:55.776309 sentry_cli-2.19.0/src/commands/projects/
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-06-14 08:24:12.000000 sentry_cli-2.19.0/src/commands/projects/list.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-06-14 08:24:12.000000 sentry_cli-2.19.0/src/commands/projects/mod.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 08:24:55.776309 sentry_cli-2.19.0/src/commands/react_native/
+-rw-r--r--   0 runner    (1001) docker     (123)     7090 2023-06-14 08:24:12.000000 sentry_cli-2.19.0/src/commands/react_native/appcenter.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     4111 2023-06-14 08:24:12.000000 sentry_cli-2.19.0/src/commands/react_native/gradle.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-06-14 08:24:12.000000 sentry_cli-2.19.0/src/commands/react_native/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    14288 2023-06-14 08:24:12.000000 sentry_cli-2.19.0/src/commands/react_native/xcode.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 08:24:55.776309 sentry_cli-2.19.0/src/commands/releases/
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-06-14 08:24:12.000000 sentry_cli-2.19.0/src/commands/releases/archive.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-06-14 08:24:12.000000 sentry_cli-2.19.0/src/commands/releases/delete.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-06-14 08:24:12.000000 sentry_cli-2.19.0/src/commands/releases/finalize.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     3160 2023-06-14 08:24:12.000000 sentry_cli-2.19.0/src/commands/releases/info.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     3300 2023-06-14 08:24:12.000000 sentry_cli-2.19.0/src/commands/releases/list.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-06-14 08:24:12.000000 sentry_cli-2.19.0/src/commands/releases/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-06-14 08:24:12.000000 sentry_cli-2.19.0/src/commands/releases/new.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-06-14 08:24:12.000000 sentry_cli-2.19.0/src/commands/releases/propose_version.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      881 2023-06-14 08:24:12.000000 sentry_cli-2.19.0/src/commands/releases/restore.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     8441 2023-06-14 08:24:12.000000 sentry_cli-2.19.0/src/commands/releases/set_commits.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 08:24:55.780309 sentry_cli-2.19.0/src/commands/repos/
+-rw-r--r--   0 runner    (1001) docker     (123)      877 2023-06-14 08:24:12.000000 sentry_cli-2.19.0/src/commands/repos/list.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-06-14 08:24:12.000000 sentry_cli-2.19.0/src/commands/repos/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-06-14 08:24:12.000000 sentry_cli-2.19.0/src/commands/send_envelope.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    11841 2023-06-14 08:24:12.000000 sentry_cli-2.19.0/src/commands/send_event.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 08:24:55.780309 sentry_cli-2.19.0/src/commands/sourcemaps/
+-rw-r--r--   0 runner    (1001) docker     (123)    16362 2023-06-14 08:24:12.000000 sentry_cli-2.19.0/src/commands/sourcemaps/explain.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     3964 2023-06-14 08:24:12.000000 sentry_cli-2.19.0/src/commands/sourcemaps/inject.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-06-14 08:24:12.000000 sentry_cli-2.19.0/src/commands/sourcemaps/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     3737 2023-06-14 08:24:12.000000 sentry_cli-2.19.0/src/commands/sourcemaps/resolve.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    14882 2023-06-14 08:24:12.000000 sentry_cli-2.19.0/src/commands/sourcemaps/upload.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     2532 2023-06-14 08:24:12.000000 sentry_cli-2.19.0/src/commands/uninstall.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-06-14 08:24:12.000000 sentry_cli-2.19.0/src/commands/update.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-06-14 08:24:12.000000 sentry_cli-2.19.0/src/commands/upload_dif.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-06-14 08:24:12.000000 sentry_cli-2.19.0/src/commands/upload_dsym.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    10733 2023-06-14 08:24:12.000000 sentry_cli-2.19.0/src/commands/upload_proguard.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    20882 2023-06-14 08:24:12.000000 sentry_cli-2.19.0/src/config.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-06-14 08:24:12.000000 sentry_cli-2.19.0/src/constants.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-06-14 08:24:12.000000 sentry_cli-2.19.0/src/main.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 08:24:55.784309 sentry_cli-2.19.0/src/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-06-14 08:24:12.000000 sentry_cli-2.19.0/src/utils/android.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     8095 2023-06-14 08:24:12.000000 sentry_cli-2.19.0/src/utils/appcenter.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     4129 2023-06-14 08:24:12.000000 sentry_cli-2.19.0/src/utils/args.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     7299 2023-06-14 08:24:12.000000 sentry_cli-2.19.0/src/utils/chunks.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     4543 2023-06-14 08:24:12.000000 sentry_cli-2.19.0/src/utils/codepush.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-06-14 08:24:12.000000 sentry_cli-2.19.0/src/utils/cordova.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    14695 2023-06-14 08:24:12.000000 sentry_cli-2.19.0/src/utils/dif.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    72888 2023-06-14 08:24:12.000000 sentry_cli-2.19.0/src/utils/dif_upload.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-06-14 08:24:12.000000 sentry_cli-2.19.0/src/utils/enc.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     3132 2023-06-14 08:24:12.000000 sentry_cli-2.19.0/src/utils/event.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     5531 2023-06-14 08:24:12.000000 sentry_cli-2.19.0/src/utils/file_search.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    17036 2023-06-14 08:24:12.000000 sentry_cli-2.19.0/src/utils/file_upload.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     2486 2023-06-14 08:24:12.000000 sentry_cli-2.19.0/src/utils/formatting.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     6695 2023-06-14 08:24:12.000000 sentry_cli-2.19.0/src/utils/fs.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     3222 2023-06-14 08:24:12.000000 sentry_cli-2.19.0/src/utils/http.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     3655 2023-06-14 08:24:12.000000 sentry_cli-2.19.0/src/utils/logging.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-06-14 08:24:12.000000 sentry_cli-2.19.0/src/utils/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-06-14 08:24:12.000000 sentry_cli-2.19.0/src/utils/progress.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     4884 2023-06-14 08:24:12.000000 sentry_cli-2.19.0/src/utils/releases.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-06-14 08:24:12.000000 sentry_cli-2.19.0/src/utils/retry.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 08:24:55.784309 sentry_cli-2.19.0/src/utils/snapshots/
+-rw-r--r--   0 runner    (1001) docker     (123)     4343 2023-06-14 08:24:12.000000 sentry_cli-2.19.0/src/utils/snapshots/sentry_cli__utils__vcs__generate_patch_default_twenty.snap
+-rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-06-14 08:24:12.000000 sentry_cli-2.19.0/src/utils/snapshots/sentry_cli__utils__vcs__generate_patch_ignore_missing.snap
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-06-14 08:24:12.000000 sentry_cli-2.19.0/src/utils/snapshots/sentry_cli__utils__vcs__generate_patch_set_base.snap
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-06-14 08:24:12.000000 sentry_cli-2.19.0/src/utils/snapshots/sentry_cli__utils__vcs__generate_patch_set_previous_commit.snap
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-06-14 08:24:12.000000 sentry_cli-2.19.0/src/utils/snapshots/sentry_cli__utils__vcs__get_commits_from_git.snap
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 08:24:55.784309 sentry_cli-2.19.0/src/utils/sourcemaps/
+-rw-r--r--   0 runner    (1001) docker     (123)    19215 2023-06-14 08:24:12.000000 sentry_cli-2.19.0/src/utils/sourcemaps/inject.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    38886 2023-06-14 08:24:12.000000 sentry_cli-2.19.0/src/utils/sourcemaps.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     4888 2023-06-14 08:24:12.000000 sentry_cli-2.19.0/src/utils/system.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-06-14 08:24:12.000000 sentry_cli-2.19.0/src/utils/ui.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     8628 2023-06-14 08:24:12.000000 sentry_cli-2.19.0/src/utils/update.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    36048 2023-06-14 08:24:12.000000 sentry_cli-2.19.0/src/utils/vcs.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    19150 2023-06-14 08:24:12.000000 sentry_cli-2.19.0/src/utils/xcode.rs
```

### Comparing `sentry_cli-2.18.1/Cargo.lock` & `sentry_cli-2.19.0/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -2155,64 +2155,65 @@
 name = "semver-parser"
 version = "0.7.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "388a1df253eca08550bef6c72392cfe7c30914bf41df5269b68cbd6ff8f570a3"
 
 [[package]]
 name = "sentry"
-version = "0.31.1"
+version = "0.31.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "37dd6c0cdca6b1d1ca44cde7fff289f2592a97965afec870faa7b81b9fc87745"
+checksum = "234f6e133d27140ad5ea3b369a7665f7fbc060fe246f81d8168665b38c08b600"
 dependencies = [
  "curl",
  "httpdate",
  "sentry-anyhow",
  "sentry-contexts",
  "sentry-core",
 ]
 
 [[package]]
 name = "sentry-anyhow"
-version = "0.31.1"
+version = "0.31.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d9c3d7032fff178c77c107c32c6d3337b12847adf67165ccc876c898e7154b00"
+checksum = "47e940be4c63b29006b4ac422cacea932c2cb5f8c209647ee86446ed27595a42"
 dependencies = [
  "anyhow",
  "sentry-backtrace",
  "sentry-core",
 ]
 
 [[package]]
 name = "sentry-backtrace"
-version = "0.31.1"
+version = "0.31.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c029fe8317cdd75cb2b52c600bab4e2ef64c552198e669ba874340447f330962"
+checksum = "d89b6b53de06308dd5ac08934b597bcd72a9aae0c20bc3ab06da69cb34d468e3"
 dependencies = [
  "backtrace",
  "once_cell",
  "regex",
  "sentry-core",
 ]
 
 [[package]]
 name = "sentry-cli"
-version = "2.18.1"
+version = "2.19.0"
 dependencies = [
  "anyhow",
  "anylog",
  "backoff",
  "backtrace",
  "brotli2",
  "bytecount",
  "chardet",
  "chrono",
  "clap",
  "console",
  "crossbeam-channel",
  "curl",
+ "data-encoding",
  "dirs",
  "dotenv",
  "elementtree",
  "encoding",
  "flate2",
  "git2",
  "glob",
@@ -2261,44 +2262,44 @@
  "which",
  "winapi 0.3.9",
  "zip",
 ]
 
 [[package]]
 name = "sentry-contexts"
-version = "0.31.1"
+version = "0.31.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bc575098d73c8b942b589ab453b06e4c43527556dd8f95532220d1b54d7c6b4b"
+checksum = "0769b66763e59976cd5c0fd817dcd51ccce404de8bebac0cd0e886c55b0fffa8"
 dependencies = [
  "hostname",
  "libc",
  "os_info",
  "rustc_version 0.4.0",
  "sentry-core",
  "uname",
 ]
 
 [[package]]
 name = "sentry-core"
-version = "0.31.1"
+version = "0.31.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "20216140001bbf05895f013abd0dae4df58faee24e016d54cbf107f070bac56b"
+checksum = "a1f954f1b89e8cd82576dc49bfab80304c9a6201343b4fe5c68c819f7a9bbed2"
 dependencies = [
  "once_cell",
  "rand",
  "sentry-types",
  "serde",
  "serde_json",
 ]
 
 [[package]]
 name = "sentry-types"
-version = "0.31.1"
+version = "0.31.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d7f6959d8cb3a77be27e588eef6ce9a2a469651a556d9de662e4d07e5ace4232"
+checksum = "85c53caf80cb1c6fcdf4d82b7bfff8477f50841e4caad7bf8e5e57a152b564cb"
 dependencies = [
  "debugid",
  "getrandom",
  "hex",
  "serde",
  "serde_json",
  "thiserror",
```

### Comparing `sentry_cli-2.18.1/Cargo.toml` & `sentry_cli-2.19.0/Cargo.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [package]
 authors = ["Armin Ronacher <armin.ronacher@active-4.com>"]
 build = "build.rs"
 name = "sentry-cli"
-version = "2.18.1"
+version = "2.19.0"
 edition = "2021"
 rust-version = "1.65"
 
 [dependencies]
 anylog = "0.6.3"
 anyhow = { version = "1.0.69", features = ["backtrace"] }
 backoff = "0.4.0"
@@ -18,15 +18,15 @@
 clap = { version = "4.1.6", default-features = false, features = [
   "std",
   "suggestions",
   "wrap_help",
   "string",
   "help",
   "usage",
-  "error-context"
+  "error-context",
 ] }
 console = "0.15.5"
 curl = { version = "0.4.44", features = ["static-curl", "static-ssl"] }
 dirs = "4.0.0"
 dotenv = "0.15.0"
 elementtree = "1.2.3"
 encoding = "0.2.33"
@@ -53,15 +53,15 @@
 proguard = { version = "5.0.0", features = ["uuid"] }
 r2d2 = "0.8.10"
 rayon = "1.6.1"
 regex = "1.7.1"
 runas = "1.0.0"
 rust-ini = "0.18.0"
 semver = "1.0.16"
-sentry = { version = "0.31.1", default-features = false, features = [
+sentry = { version = "0.31.2", default-features = false, features = [
   "anyhow",
   "curl",
   "contexts",
 ] }
 serde = { version = "1.0.152", features = ["derive"] }
 serde_json = "1.0.93"
 sha1_smol = { version = "1.0.0", features = ["serde"] }
@@ -70,14 +70,15 @@
 thiserror = "1.0.38"
 url = "2.3.1"
 username = "0.2.0"
 uuid = { version = "1.3.0", features = ["v4", "serde"] }
 walkdir = "2.3.2"
 which = "4.4.0"
 zip = "0.6.4"
+data-encoding = "2.3.3"
 
 [dev-dependencies]
 insta = { version = "1.26.0", features = ["redactions", "yaml"] }
 mockito = "0.31.1"
 predicates = "2.1.5"
 tempfile = "3.3.0"
 trycmd = "0.14.11"
```

### Comparing `sentry_cli-2.18.1/LICENSE` & `sentry_cli-2.19.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.18.1/PKG-INFO` & `sentry_cli-2.19.0/sentry_cli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: sentry_cli
-Version: 2.18.1
+Name: sentry-cli
+Version: 2.19.0
 Summary: A command line utility to work with Sentry.
 Home-page: https://github.com/getsentry/sentry-cli
 Author: Sentry
 Author-email: oss@sentry.io
 License: BSD-3-Clause
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: sentry_cli Version: 2.18.1 Summary: A command line
+Metadata-Version: 2.1 Name: sentry-cli Version: 2.19.0 Summary: A command line
 utility to work with Sentry. Home-page: https://github.com/getsentry/sentry-cli
 Author: Sentry Author-email: oss@sentry.io License: BSD-3-Clause Classifier:
 License :: OSI Approved :: BSD License Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3 :: Only Classifier:
 Programming Language :: Python :: Implementation :: CPython Classifier:
 Programming Language :: Python :: Implementation :: PyPy Requires-Python: >=3.7
 Description-Content-Type: text/markdown License-File: LICENSE
```

### Comparing `sentry_cli-2.18.1/README.md` & `sentry_cli-2.19.0/README.md`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.18.1/build.rs` & `sentry_cli-2.19.0/build.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.18.1/sentry_cli.egg-info/PKG-INFO` & `sentry_cli-2.19.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: sentry-cli
-Version: 2.18.1
+Name: sentry_cli
+Version: 2.19.0
 Summary: A command line utility to work with Sentry.
 Home-page: https://github.com/getsentry/sentry-cli
 Author: Sentry
 Author-email: oss@sentry.io
 License: BSD-3-Clause
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: sentry-cli Version: 2.18.1 Summary: A command line
+Metadata-Version: 2.1 Name: sentry_cli Version: 2.19.0 Summary: A command line
 utility to work with Sentry. Home-page: https://github.com/getsentry/sentry-cli
 Author: Sentry Author-email: oss@sentry.io License: BSD-3-Clause Classifier:
 License :: OSI Approved :: BSD License Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3 :: Only Classifier:
 Programming Language :: Python :: Implementation :: CPython Classifier:
 Programming Language :: Python :: Implementation :: PyPy Requires-Python: >=3.7
 Description-Content-Type: text/markdown License-File: LICENSE
```

### Comparing `sentry_cli-2.18.1/sentry_cli.egg-info/SOURCES.txt` & `sentry_cli-2.19.0/sentry_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.18.1/setup.cfg` & `sentry_cli-2.19.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.18.1/setup.py` & `sentry_cli-2.19.0/setup.py`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.18.1/src/api.rs` & `sentry_cli-2.19.0/src/api.rs`

 * *Files 0% similar despite different names*

```diff
@@ -1456,48 +1456,38 @@
         }
         Ok(rv)
     }
 
     /// Create a new checkin for a monitor
     pub fn create_monitor_checkin(
         &self,
-        dsn: Option<Dsn>,
         monitor_slug: &String,
-        checkin: &CreateMonitorCheckIn,
-    ) -> ApiResult<MonitorCheckIn> {
+        checkin: &ApiCreateMonitorCheckIn,
+    ) -> ApiResult<ApiMonitorCheckIn> {
         let path = &format!("/monitors/{}/checkins/", PathArg(monitor_slug),);
-        let resp = if let Some(dsn) = dsn {
-            self.request_with_dsn_auth(Method::Post, path, dsn, Some(checkin))?
-        } else {
-            self.post(path, checkin)?
-        };
+        let resp = self.post(path, checkin)?;
         if resp.status() == 404 {
             return Err(ApiErrorKind::ResourceNotFound.into());
         }
         resp.convert()
     }
 
     /// Update a checkin for a monitor
     pub fn update_monitor_checkin(
         &self,
-        dsn: Option<Dsn>,
         monitor_slug: &String,
         checkin_id: &Uuid,
-        checkin: &UpdateMonitorCheckIn,
-    ) -> ApiResult<MonitorCheckIn> {
+        checkin: &ApiUpdateMonitorCheckIn,
+    ) -> ApiResult<ApiMonitorCheckIn> {
         let path = &format!(
             "/monitors/{}/checkins/{}/",
             PathArg(monitor_slug),
             PathArg(checkin_id),
         );
-        let resp = if let Some(dsn) = dsn {
-            self.request_with_dsn_auth(Method::Put, path, dsn, Some(checkin))?
-        } else {
-            self.put(path, checkin)?
-        };
+        let resp = self.put(path, checkin)?;
 
         if resp.status() == 404 {
             return Err(ApiErrorKind::ResourceNotFound.into());
         }
         resp.convert()
     }
 
@@ -2474,39 +2464,39 @@
     pub slug: String,
     pub name: String,
     pub status: String,
 }
 
 #[derive(Debug, Serialize, Deserialize)]
 #[serde(rename_all = "snake_case")]
-pub enum MonitorCheckinStatus {
+pub enum ApiMonitorCheckInStatus {
     Unknown,
     Ok,
     InProgress,
     Error,
 }
 
 #[derive(Debug, Deserialize)]
-pub struct MonitorCheckIn {
+pub struct ApiMonitorCheckIn {
     pub id: Uuid,
-    pub status: Option<MonitorCheckinStatus>,
+    pub status: Option<ApiMonitorCheckInStatus>,
     pub duration: Option<u64>,
     pub environment: Option<String>,
 }
 
 #[derive(Debug, Serialize)]
-pub struct CreateMonitorCheckIn {
-    pub status: MonitorCheckinStatus,
+pub struct ApiCreateMonitorCheckIn {
+    pub status: ApiMonitorCheckInStatus,
     pub environment: String,
 }
 
 #[derive(Debug, Serialize, Default)]
-pub struct UpdateMonitorCheckIn {
+pub struct ApiUpdateMonitorCheckIn {
     #[serde(skip_serializing_if = "Option::is_none")]
-    pub status: Option<MonitorCheckinStatus>,
+    pub status: Option<ApiMonitorCheckInStatus>,
     #[serde(skip_serializing_if = "Option::is_none")]
     pub duration: Option<u64>,
     #[serde(skip_serializing_if = "Option::is_none")]
     pub environment: Option<String>,
 }
 
 #[derive(Deserialize, Debug)]
```

### Comparing `sentry_cli-2.18.1/src/bashsupport.sh` & `sentry_cli-2.19.0/src/bashsupport.sh`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.18.1/src/commands/bash_hook.rs` & `sentry_cli-2.19.0/src/commands/bash_hook.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.18.1/src/commands/debug_files/bundle_jvm.rs` & `sentry_cli-2.19.0/src/commands/debug_files/bundle_jvm.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.18.1/src/commands/debug_files/bundle_sources.rs` & `sentry_cli-2.19.0/src/commands/debug_files/bundle_sources.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.18.1/src/commands/debug_files/check.rs` & `sentry_cli-2.19.0/src/commands/debug_files/check.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.18.1/src/commands/debug_files/find.rs` & `sentry_cli-2.19.0/src/commands/debug_files/find.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.18.1/src/commands/debug_files/mod.rs` & `sentry_cli-2.19.0/src/commands/debug_files/mod.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.18.1/src/commands/debug_files/print_sources.rs` & `sentry_cli-2.19.0/src/commands/debug_files/print_sources.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.18.1/src/commands/debug_files/upload.rs` & `sentry_cli-2.19.0/src/commands/debug_files/upload.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.18.1/src/commands/deploys/list.rs` & `sentry_cli-2.19.0/src/commands/deploys/list.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.18.1/src/commands/deploys/mod.rs` & `sentry_cli-2.19.0/src/commands/deploys/mod.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.18.1/src/commands/deploys/new.rs` & `sentry_cli-2.19.0/src/commands/deploys/new.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.18.1/src/commands/events/list.rs` & `sentry_cli-2.19.0/src/commands/events/list.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.18.1/src/commands/events/mod.rs` & `sentry_cli-2.19.0/src/commands/events/mod.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.18.1/src/commands/files/delete.rs` & `sentry_cli-2.19.0/src/commands/files/delete.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.18.1/src/commands/files/list.rs` & `sentry_cli-2.19.0/src/commands/files/list.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.18.1/src/commands/files/mod.rs` & `sentry_cli-2.19.0/src/commands/files/mod.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.18.1/src/commands/files/upload.rs` & `sentry_cli-2.19.0/src/commands/files/upload.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.18.1/src/commands/info.rs` & `sentry_cli-2.19.0/src/commands/info.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.18.1/src/commands/issues/mod.rs` & `sentry_cli-2.19.0/src/commands/issues/mod.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.18.1/src/commands/issues/mute.rs` & `sentry_cli-2.19.0/src/commands/issues/mute.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.18.1/src/commands/issues/resolve.rs` & `sentry_cli-2.19.0/src/commands/issues/resolve.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.18.1/src/commands/issues/unresolve.rs` & `sentry_cli-2.19.0/src/commands/issues/unresolve.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.18.1/src/commands/login.rs` & `sentry_cli-2.19.0/src/commands/login.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.18.1/src/commands/mod.rs` & `sentry_cli-2.19.0/src/commands/mod.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.18.1/src/commands/monitors/list.rs` & `sentry_cli-2.19.0/src/commands/monitors/list.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.18.1/src/commands/monitors/mod.rs` & `sentry_cli-2.19.0/src/commands/monitors/mod.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.18.1/src/commands/organizations/list.rs` & `sentry_cli-2.19.0/src/commands/organizations/list.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.18.1/src/commands/organizations/mod.rs` & `sentry_cli-2.19.0/src/commands/organizations/mod.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.18.1/src/commands/projects/list.rs` & `sentry_cli-2.19.0/src/commands/projects/list.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.18.1/src/commands/projects/mod.rs` & `sentry_cli-2.19.0/src/commands/projects/mod.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.18.1/src/commands/react_native/appcenter.rs` & `sentry_cli-2.19.0/src/commands/react_native/appcenter.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.18.1/src/commands/react_native/gradle.rs` & `sentry_cli-2.19.0/src/commands/react_native/gradle.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.18.1/src/commands/react_native/mod.rs` & `sentry_cli-2.19.0/src/commands/react_native/mod.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.18.1/src/commands/react_native/xcode.rs` & `sentry_cli-2.19.0/src/commands/react_native/xcode.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.18.1/src/commands/releases/archive.rs` & `sentry_cli-2.19.0/src/commands/releases/archive.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.18.1/src/commands/releases/delete.rs` & `sentry_cli-2.19.0/src/commands/releases/delete.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.18.1/src/commands/releases/finalize.rs` & `sentry_cli-2.19.0/src/commands/releases/finalize.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.18.1/src/commands/releases/info.rs` & `sentry_cli-2.19.0/src/commands/releases/info.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.18.1/src/commands/releases/list.rs` & `sentry_cli-2.19.0/src/commands/releases/list.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.18.1/src/commands/releases/mod.rs` & `sentry_cli-2.19.0/src/commands/releases/mod.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.18.1/src/commands/releases/new.rs` & `sentry_cli-2.19.0/src/commands/releases/new.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.18.1/src/commands/releases/restore.rs` & `sentry_cli-2.19.0/src/commands/releases/restore.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.18.1/src/commands/releases/set_commits.rs` & `sentry_cli-2.19.0/src/commands/releases/set_commits.rs`

 * *Files 2% similar despite different names*

```diff
@@ -103,15 +103,15 @@
         Some(vec![])
     } else if matches.get_flag("local") {
         None
     } else {
         if let Some(commits) = matches.get_many::<String>("commits") {
             for spec in commits {
                 let commit_spec = CommitSpec::parse(spec)?;
-                if repos.iter().any(|r| r.name == commit_spec.repo) {
+                if repos.iter().any(|r| r.name.to_lowercase() == commit_spec.repo.to_lowercase()) {
                     commit_specs.push(commit_spec);
                 } else {
                     bail!("Unknown repo '{}'", commit_spec.repo);
                 }
             }
         }
         let commits = find_heads(
```

### Comparing `sentry_cli-2.18.1/src/commands/repos/list.rs` & `sentry_cli-2.19.0/src/commands/repos/list.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.18.1/src/commands/repos/mod.rs` & `sentry_cli-2.19.0/src/commands/repos/mod.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.18.1/src/commands/send_envelope.rs` & `sentry_cli-2.19.0/src/commands/send_envelope.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.18.1/src/commands/send_event.rs` & `sentry_cli-2.19.0/src/commands/send_event.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.18.1/src/commands/sourcemaps/explain.rs` & `sentry_cli-2.19.0/src/commands/sourcemaps/explain.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.18.1/src/commands/sourcemaps/inject.rs` & `sentry_cli-2.19.0/src/commands/sourcemaps/inject.rs`

 * *Files 0% similar despite different names*

```diff
@@ -61,15 +61,14 @@
         )
         .arg(
             Arg::new("dry_run")
                 .long("dry-run")
                 .action(ArgAction::SetTrue)
                 .help("Don't modify files on disk."),
         )
-        .hide(true)
 }
 
 pub fn execute(matches: &ArgMatches) -> Result<()> {
     let mut processor = SourceMapProcessor::new();
 
     let paths = matches
         .get_many::<String>("paths")
```

### Comparing `sentry_cli-2.18.1/src/commands/sourcemaps/mod.rs` & `sentry_cli-2.19.0/src/commands/sourcemaps/mod.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.18.1/src/commands/sourcemaps/resolve.rs` & `sentry_cli-2.19.0/src/commands/sourcemaps/resolve.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.18.1/src/commands/sourcemaps/upload.rs` & `sentry_cli-2.19.0/src/commands/sourcemaps/upload.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.18.1/src/commands/uninstall.rs` & `sentry_cli-2.19.0/src/commands/uninstall.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.18.1/src/commands/update.rs` & `sentry_cli-2.19.0/src/commands/update.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.18.1/src/commands/upload_proguard.rs` & `sentry_cli-2.19.0/src/commands/upload_proguard.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.18.1/src/config.rs` & `sentry_cli-2.19.0/src/config.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.18.1/src/constants.rs` & `sentry_cli-2.19.0/src/constants.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.18.1/src/utils/android.rs` & `sentry_cli-2.19.0/src/utils/android.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.18.1/src/utils/appcenter.rs` & `sentry_cli-2.19.0/src/utils/appcenter.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.18.1/src/utils/args.rs` & `sentry_cli-2.19.0/src/utils/args.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.18.1/src/utils/chunks.rs` & `sentry_cli-2.19.0/src/utils/chunks.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.18.1/src/utils/codepush.rs` & `sentry_cli-2.19.0/src/utils/codepush.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.18.1/src/utils/cordova.rs` & `sentry_cli-2.19.0/src/utils/cordova.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.18.1/src/utils/dif.rs` & `sentry_cli-2.19.0/src/utils/dif.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.18.1/src/utils/dif_upload.rs` & `sentry_cli-2.19.0/src/utils/dif_upload.rs`

 * *Files 0% similar despite different names*

```diff
@@ -504,22 +504,26 @@
 /// This function will not recurse into ZIPs contained in this ZIP.
 fn walk_difs_zip<F>(mut zip: ZipFileArchive, options: &DifUpload, mut func: F) -> Result<()>
 where
     F: FnMut(DifSource<'_>, String, ByteView<'static>) -> Result<()>,
 {
     for index in 0..zip.len() {
         let (name, buffer) = {
-            let zip_file = zip.by_index(index)?;
+            let mut zip_file = zip.by_index(index)?;
             let name = zip_file.name().to_string();
 
             if !options.valid_extension(Path::new(&name).extension()) {
                 continue;
             }
 
-            (name, ByteView::read(zip_file).map_err(Error::new)?)
+            let tmp_file = TempFile::create()?;
+            let mut tmp_fh = tmp_file.open()?;
+            std::io::copy(&mut zip_file, &mut tmp_fh)?;
+
+            (name, ByteView::map_file(tmp_fh).map_err(Error::new)?)
         };
 
         func(DifSource::Zip(&mut zip, &name), name.clone(), buffer)?;
     }
 
     Ok(())
 }
```

### Comparing `sentry_cli-2.18.1/src/utils/enc.rs` & `sentry_cli-2.19.0/src/utils/enc.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.18.1/src/utils/event.rs` & `sentry_cli-2.19.0/src/utils/event.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.18.1/src/utils/file_search.rs` & `sentry_cli-2.19.0/src/utils/file_search.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.18.1/src/utils/file_upload.rs` & `sentry_cli-2.19.0/src/utils/file_upload.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.18.1/src/utils/formatting.rs` & `sentry_cli-2.19.0/src/utils/formatting.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.18.1/src/utils/fs.rs` & `sentry_cli-2.19.0/src/utils/fs.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.18.1/src/utils/http.rs` & `sentry_cli-2.19.0/src/utils/http.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.18.1/src/utils/logging.rs` & `sentry_cli-2.19.0/src/utils/logging.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.18.1/src/utils/progress.rs` & `sentry_cli-2.19.0/src/utils/progress.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.18.1/src/utils/releases.rs` & `sentry_cli-2.19.0/src/utils/releases.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.18.1/src/utils/retry.rs` & `sentry_cli-2.19.0/src/utils/retry.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.18.1/src/utils/snapshots/sentry_cli__utils__vcs__generate_patch_default_twenty.snap` & `sentry_cli-2.19.0/src/utils/snapshots/sentry_cli__utils__vcs__generate_patch_default_twenty.snap`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.18.1/src/utils/snapshots/sentry_cli__utils__vcs__generate_patch_ignore_missing.snap` & `sentry_cli-2.19.0/src/utils/snapshots/sentry_cli__utils__vcs__generate_patch_ignore_missing.snap`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.18.1/src/utils/snapshots/sentry_cli__utils__vcs__generate_patch_set_base.snap` & `sentry_cli-2.19.0/src/utils/snapshots/sentry_cli__utils__vcs__generate_patch_set_base.snap`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.18.1/src/utils/snapshots/sentry_cli__utils__vcs__get_commits_from_git.snap` & `sentry_cli-2.19.0/src/utils/snapshots/sentry_cli__utils__vcs__get_commits_from_git.snap`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.18.1/src/utils/sourcemaps/inject.rs` & `sentry_cli-2.19.0/src/utils/sourcemaps/inject.rs`

 * *Files 26% similar despite different names*

```diff
@@ -1,25 +1,31 @@
 use console::style;
 use itertools::Itertools;
+use regex::Regex;
 use symbolic::common::{clean_path, join_path};
 
 use std::fmt;
 use std::io::{BufRead, Write};
 use std::path::PathBuf;
 
 use anyhow::{bail, Result};
+use lazy_static::lazy_static;
 use log::debug;
 use sentry::types::DebugId;
 use serde_json::Value;
 
 const CODE_SNIPPET_TEMPLATE: &str = r#"!function(){try{var e="undefined"!=typeof window?window:"undefined"!=typeof global?global:"undefined"!=typeof self?self:{},n=(new Error).stack;n&&(e._sentryDebugIds=e._sentryDebugIds||{},e._sentryDebugIds[n]="__SENTRY_DEBUG_ID__")}catch(e){}}()"#;
 const DEBUGID_PLACEHOLDER: &str = "__SENTRY_DEBUG_ID__";
 const SOURCEMAP_DEBUGID_KEY: &str = "debug_id";
 const DEBUGID_COMMENT_PREFIX: &str = "//# debugId";
 
+lazy_static! {
+    static ref USE_PRAGMA_RE: Regex = Regex::new(r#""use \w+";|'use \w+';"#).unwrap();
+}
+
 fn print_section_with_debugid(
     f: &mut fmt::Formatter<'_>,
     title: &str,
     data: &[(PathBuf, DebugId)],
 ) -> fmt::Result {
     print_section_title(f, title)?;
     for (path, debug_id) in data.iter().sorted_by_key(|x| &x.0) {
@@ -89,28 +95,144 @@
             )?;
         }
 
         Ok(())
     }
 }
 
-/// Appends the following text to a file:
+/// Fixes up a minified JS source file with a debug id.
+///
+/// This changes the source file in several ways:
+/// 1. The source code snippet
+/// `<CODE_SNIPPET>[<debug_id>]`
+/// is inserted at the earliest possible position, which is after an
+/// optional hashbang, followed by a
+/// block of comments, empty lines, and `"use […]";` or `'use […]';` pragmas.
+/// 2. A comment of the form `//# debugId=<debug_id>` is appended to the file.
+/// 3. The last source mapping comment (a comment starting with
+/// `//# sourceMappingURL=` or `//@ sourceMappingURL=`) is moved to
+/// the very end of the file, after the debug id comment from 2.
+///
+/// This function will naturally mess with the correspondence between a source file
+/// and its sourcemap. Use [`insert_empty_mapping`] on the sourcemap to fix this.
+/// # Example
 /// ```
+/// let file = "
+/// // a
+/// // comment
+/// // block
+///
+/// // another
+/// // comment
+/// // block
+///
+/// 'use strict';
+/// function t(t) {
+///   return '[object Object]' === Object.prototype.toString.call(t);
+/// }
+/// //# sourceMappingURL=/path/to/sourcemap
+/// ";
+///
+/// let mut file = file.as_bytes().to_vec();
+/// fixup_js_file(&mut file, DebugId::default()).unwrap();
+///
+/// assert_eq!(
+///     std::str::from_utf8(&file).unwrap(),
+///     r#"
+/// // a
+/// // comment
+/// // block
 ///
-/// <CODE_SNIPPET>[<debug_id>]
-/// //# sentryDebugId=<debug_id>
-///```
-/// where `<CODE_SNIPPET>[<debug_id>]`
-/// is `CODE_SNIPPET_TEMPLATE` with `debug_id` substituted for the `__SENTRY_DEBUG_ID__`
-/// placeholder.
+/// // another
+/// // comment
+/// // block
 ///
-/// Moreover, if a `sourceMappingURL` comment exists in the file, it is moved to the very end.
+/// 'use strict';
+/// !function(){try{var e="undefined"!=typeof window?window:"undefined"!=typeof global?global:"undefined"!=typeof self?self:{},n=(new Error).stack;n&&(e._sentryDebugIds=e._sentryDebugIds||{},e._sentryDebugIds[n]="00000000-0000-0000-0000-000000000000")}catch(e){}}()
+/// function t(t) {
+///   return '[object Object]' === Object.prototype.toString.call(t);
+/// }
+/// //# debugId=00000000-0000-0000-0000-000000000000
+/// //# sourceMappingURL=/path/to/sourcemap
+/// "#
+/// );
+/// ```
 pub fn fixup_js_file(js_contents: &mut Vec<u8>, debug_id: DebugId) -> Result<()> {
-    let js_lines: Result<Vec<String>, _> = js_contents.lines().collect();
-    let mut js_lines = js_lines?;
+    let mut js_lines = js_contents.lines().collect::<Result<Vec<_>, _>>()?;
+
+    js_contents.clear();
+
+    // Find the last source mapping URL comment, it's the only one that matters
+    let sourcemap_comment_idx = js_lines
+        .iter()
+        .enumerate()
+        .rev()
+        .find(|(_idx, line)| {
+            line.starts_with("//# sourceMappingURL=") || line.starts_with("//@ sourceMappingURL=")
+        })
+        .map(|(idx, _)| idx);
+
+    let sourcemap_comment = sourcemap_comment_idx.map(|idx| js_lines.remove(idx));
+
+    let mut js_lines = js_lines.into_iter().peekable();
+
+    // Handle initial hashbang
+    if let Some(hashbang) = js_lines.next_if(|line| line.trim().starts_with("#!")) {
+        writeln!(js_contents, "{hashbang}")?;
+    }
+
+    // Write comments and empty lines at the start back to the file
+    while let Some(comment_or_empty) =
+        js_lines.next_if(|line| line.trim().is_empty() || line.trim().starts_with("//"))
+    {
+        writeln!(js_contents, "{comment_or_empty}")?;
+    }
+
+    // Write use statements back to the file
+    while let Some(use_pragma) = js_lines.next_if(|line| USE_PRAGMA_RE.is_match(line)) {
+        writeln!(js_contents, "{use_pragma}")?;
+    }
+
+    // Inject the code snippet
+    let to_inject = CODE_SNIPPET_TEMPLATE.replace(DEBUGID_PLACEHOLDER, &debug_id.to_string());
+    writeln!(js_contents, "{to_inject}")?;
+
+    // Write other lines
+    for line in js_lines {
+        writeln!(js_contents, "{line}")?;
+    }
+
+    // Write the debug id comment
+    writeln!(js_contents, "{DEBUGID_COMMENT_PREFIX}={debug_id}")?;
+
+    // Lastly, write the source mapping URL comment, if there was one
+    if let Some(sourcemap_comment) = sourcemap_comment {
+        writeln!(js_contents, "{sourcemap_comment}")?;
+    }
+
+    Ok(())
+}
+
+/// Fixes up a minified JS source file with a debug id without messing with mappings.
+///
+/// This changes the source file in several ways:
+/// 1. The source code snippet
+/// `<CODE_SNIPPET>[<debug_id>]` is appended to the file.
+/// 2. A comment of the form `//# debugId=<debug_id>` is appended to the file.
+/// 3. The last source mapping comment (a comment starting with
+/// `//# sourceMappingURL=` or `//@ sourceMappingURL=`) is moved to
+/// the very end of the file, after the debug id comment from 2.
+///
+/// This function is useful in cases where a source file's corresponding sourcemap is
+/// not available. In such a case, [`fixup_js_file`] might mess up the mappings by inserting
+/// a line, with no opportunity to adjust the sourcemap accordingly. However, in general
+/// it is desirable to insert the code snippet as early as possible to make sure it runs
+/// even when an error is raised in the file.
+pub fn fixup_js_file_end(js_contents: &mut Vec<u8>, debug_id: DebugId) -> Result<()> {
+    let mut js_lines = js_contents.lines().collect::<Result<Vec<_>, _>>()?;
 
     js_contents.clear();
 
     let sourcemap_comment_idx = js_lines
         .iter()
         .enumerate()
         .rev()
@@ -132,14 +254,43 @@
     if let Some(sourcemap_comment) = sourcemap_comment {
         writeln!(js_contents, "{sourcemap_comment}")?;
     }
 
     Ok(())
 }
 
+/// Replaces a JS file's source mapping url with a new one.
+///
+/// Only the bottommost source mapping url comment will be updated. If there
+/// are no source mapping url comments in the file, this is a no-op.
+pub fn replace_sourcemap_url(js_contents: &mut Vec<u8>, new_url: &str) -> Result<()> {
+    let js_lines = js_contents.lines().collect::<Result<Vec<_>, _>>()?;
+
+    let sourcemap_comment_idx = match js_lines.iter().enumerate().rev().find(|(_idx, line)| {
+        line.starts_with("//# sourceMappingURL=") || line.starts_with("//@ sourceMappingURL=")
+    }) {
+        Some((idx, _)) => idx,
+        None => return Ok(()),
+    };
+
+    js_contents.clear();
+
+    for line in &js_lines[0..sourcemap_comment_idx] {
+        writeln!(js_contents, "{line}")?;
+    }
+
+    writeln!(js_contents, "//# sourceMappingURL={new_url}")?;
+
+    for line in &js_lines[sourcemap_comment_idx + 1..] {
+        writeln!(js_contents, "{line}")?;
+    }
+
+    Ok(())
+}
+
 /// Generates a debug ID from bytes.
 pub fn debug_id_from_bytes_hashed(bytes: &[u8]) -> DebugId {
     let mut hash = sha1_smol::Sha1::new();
     hash.update(bytes);
     let mut sha1_bytes = [0u8; 16];
     sha1_bytes.copy_from_slice(&hash.digest().bytes()[..16]);
     DebugId::from_uuid(uuid::Builder::from_sha1_bytes(sha1_bytes).into_uuid())
@@ -165,21 +316,50 @@
             Ok((debug_id, false))
         }
 
         None => {
             let debug_id = debug_id_from_bytes_hashed(sourcemap_contents);
             let id = serde_json::to_value(debug_id)?;
             map.insert(SOURCEMAP_DEBUGID_KEY.to_string(), id);
+
             sourcemap_contents.clear();
             serde_json::to_writer(sourcemap_contents, &sourcemap)?;
             Ok((debug_id, true))
         }
     }
 }
 
+/// This adds an empty mapping at the start of a sourcemap.
+///
+/// This is used to adjust a sourcemap when the corresponding source file has a
+/// new line injected near the top (see [`fixup_js_file`]).
+pub fn insert_empty_mapping(sourcemap_contents: &mut Vec<u8>) -> Result<()> {
+    let mut sourcemap: Value = serde_json::from_slice(sourcemap_contents)?;
+
+    let Some(map) = sourcemap.as_object_mut() else {
+        bail!("Invalid sourcemap");
+    };
+
+    let Some(mappings) = map.get_mut("mappings") else {
+        bail!("Invalid sourcemap");
+    };
+
+    let Value::String(mappings) = mappings else {
+        bail!("Invalid sourcemap");
+    };
+
+    // Insert empty mapping at the start
+    *mappings = format!(";{mappings}");
+
+    sourcemap_contents.clear();
+    serde_json::to_writer(sourcemap_contents, &sourcemap)?;
+
+    Ok(())
+}
+
 /// Computes a normalized sourcemap URL from a source file's own URL und the relative URL of its sourcemap.
 ///
 /// Roughly, this will combine a source URL of `some/dir/source.js` and a sourcemap URL of `path/to/source.min.js`
 /// to `some/dir/path/to/source.min.js`, taking `..` and `.` path segments as well as absolute sourcemap URLs
 /// into account.
 ///
 /// Leading `./` segments will be preserved.
@@ -202,15 +382,15 @@
 mod tests {
     use std::io::Write;
 
     use sentry::types::DebugId;
 
     use crate::utils::fs::TempFile;
 
-    use super::{fixup_js_file, fixup_sourcemap, normalize_sourcemap_url};
+    use super::{fixup_js_file, fixup_sourcemap, normalize_sourcemap_url, replace_sourcemap_url};
 
     #[test]
     fn test_fixup_sourcemap() {
         for sourcemap_path in &[
             "server/chunks/1.js.map",
             "server/edge-runtime-webpack.js.map",
             "server/pages/_document.js.map",
@@ -249,18 +429,18 @@
         let debug_id = DebugId::default();
 
         let mut source = Vec::from(source);
 
         fixup_js_file(&mut source, debug_id).unwrap();
 
         let expected = r#"//# sourceMappingURL=fake1
+!function(){try{var e="undefined"!=typeof window?window:"undefined"!=typeof global?global:"undefined"!=typeof self?self:{},n=(new Error).stack;n&&(e._sentryDebugIds=e._sentryDebugIds||{},e._sentryDebugIds[n]="00000000-0000-0000-0000-000000000000")}catch(e){}}()
 some line
 //# sourceMappingURL=fake2
 something else
-!function(){try{var e="undefined"!=typeof window?window:"undefined"!=typeof global?global:"undefined"!=typeof self?self:{},n=(new Error).stack;n&&(e._sentryDebugIds=e._sentryDebugIds||{},e._sentryDebugIds[n]="00000000-0000-0000-0000-000000000000")}catch(e){}}()
 //# debugId=00000000-0000-0000-0000-000000000000
 //# sourceMappingURL=real
 "#;
 
         assert_eq!(std::str::from_utf8(&source).unwrap(), expected);
     }
 
@@ -302,14 +482,15 @@
             file.write_all(&source).unwrap();
         }
 
         let result = std::fs::read_to_string(temp_file.path()).unwrap();
         let expected = r#"//# sourceMappingURL=fake
 
 
+!function(){try{var e="undefined"!=typeof window?window:"undefined"!=typeof global?global:"undefined"!=typeof self?self:{},n=(new Error).stack;n&&(e._sentryDebugIds=e._sentryDebugIds||{},e._sentryDebugIds[n]="00000000-0000-0000-0000-000000000000")}catch(e){}}()
 some line
 //# sourceMappingURL=fake
 //# sourceMappingURL=fake
 //# sourceMappingURL=fake
 //# sourceMappingURL=fake
 //# sourceMappingURL=fake
 //# sourceMappingURL=fake
@@ -317,24 +498,59 @@
 //# sourceMappingURL=fake
 //# sourceMappingURL=fake
 //# sourceMappingURL=fake
 //# sourceMappingURL=fake
 //# sourceMappingURL=fake
 //# sourceMappingURL=fake
 something else
-!function(){try{var e="undefined"!=typeof window?window:"undefined"!=typeof global?global:"undefined"!=typeof self?self:{},n=(new Error).stack;n&&(e._sentryDebugIds=e._sentryDebugIds||{},e._sentryDebugIds[n]="00000000-0000-0000-0000-000000000000")}catch(e){}}()
 //# debugId=00000000-0000-0000-0000-000000000000
 //# sourceMappingURL=real
 "#;
 
         println!("{}", result);
         assert_eq!(result, expected);
     }
 
     #[test]
+    fn test_fixup_js_file_use_strict() {
+        let source = r#"#!/bin/node
+//# sourceMappingURL=fake1
+
+  // some other comment
+ "use strict"; rest of the line
+'use strict';
+some line
+//# sourceMappingURL=fake2
+//# sourceMappingURL=real
+something else"#;
+
+        let debug_id = DebugId::default();
+
+        let mut source = Vec::from(source);
+
+        fixup_js_file(&mut source, debug_id).unwrap();
+
+        let expected = r#"#!/bin/node
+//# sourceMappingURL=fake1
+
+  // some other comment
+ "use strict"; rest of the line
+'use strict';
+!function(){try{var e="undefined"!=typeof window?window:"undefined"!=typeof global?global:"undefined"!=typeof self?self:{},n=(new Error).stack;n&&(e._sentryDebugIds=e._sentryDebugIds||{},e._sentryDebugIds[n]="00000000-0000-0000-0000-000000000000")}catch(e){}}()
+some line
+//# sourceMappingURL=fake2
+something else
+//# debugId=00000000-0000-0000-0000-000000000000
+//# sourceMappingURL=real
+"#;
+
+        assert_eq!(std::str::from_utf8(&source).unwrap(), expected);
+    }
+
+    #[test]
     fn test_normalize_sourcemap_url() {
         assert_eq!(
             normalize_sourcemap_url("foo/bar/baz.js", "baz.js.map"),
             "foo/bar/baz.js.map"
         );
 
         assert_eq!(
@@ -358,8 +574,31 @@
         );
 
         assert_eq!(
             normalize_sourcemap_url("././.foo/bar/baz.js", "../quux/baz.js.map"),
             "././.foo/quux/baz.js.map"
         );
     }
+
+    #[test]
+    fn test_replace_sourcemap_url() {
+        let js_contents = r#"
+//# sourceMappingURL=not this one
+some text
+//@ sourceMappingURL=not this one either
+//# sourceMappingURL=this one
+more text
+"#;
+        let mut js_contents = Vec::from(js_contents);
+
+        replace_sourcemap_url(&mut js_contents, "new url").unwrap();
+
+        let expected = r#"
+//# sourceMappingURL=not this one
+some text
+//@ sourceMappingURL=not this one either
+//# sourceMappingURL=new url
+more text
+"#;
+        assert_eq!(std::str::from_utf8(&js_contents).unwrap(), expected);
+    }
 }
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `sentry_cli-2.18.1/src/utils/sourcemaps.rs` & `sentry_cli-2.19.0/src/utils/sourcemaps.rs`

 * *Files 3% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 use crate::utils::enc::decode_unknown_string;
 use crate::utils::file_search::ReleaseFileMatch;
 use crate::utils::file_upload::{
     initialize_legacy_release_upload, FileUpload, SourceFile, SourceFiles, UploadContext,
 };
 use crate::utils::logging::is_quiet_mode;
 use crate::utils::progress::ProgressBar;
-use crate::utils::sourcemaps::inject::{fixup_js_file, normalize_sourcemap_url, InjectReport};
+use crate::utils::sourcemaps::inject::InjectReport;
 
 pub mod inject;
 
 /// The string prefix denoting a data URL.
 ///
 /// Data URLs are used to embed sourcemaps directly in javascript source files.
 const DATA_PREAMBLE: &str = "data:application/json;base64,";
@@ -762,110 +762,145 @@
     /// for JavaScript files.
     pub fn inject_debug_ids(&mut self, dry_run: bool, js_extensions: &[&str]) -> Result<()> {
         self.flush_pending_sources();
         println!("{} Injecting debug ids", style(">").dim());
 
         let mut report = InjectReport::default();
 
-        // Step 1: Produce a debug id for each source file by either reading it from the
-        // sourcemap if available or else generating a fresh one.
-        let mut debug_ids = Vec::new();
+        for (source_url, sourcemap_url) in self.sourcemap_references.iter_mut() {
+            // We only allow injection into files that match the extension
+            if !url_matches_extension(source_url, js_extensions) {
+                debug!(
+                    "skipping potential js file {} because it does not match extension",
+                    source_url
+                );
+                continue;
+            }
 
-        for (source_url, sourcemap_url) in &self.sourcemap_references {
             if let Some(debug_id) = self.debug_ids.get(source_url) {
                 report
                     .previously_injected
                     .push((source_url.into(), *debug_id));
                 continue;
             }
 
-            let sourcemap_url = match sourcemap_url {
-                Some(sourcemap_url) => sourcemap_url,
-                None => {
-                    // no source map at all, try a deterministic debug id from the contents
-                    let debug_id = self
-                        .sources
-                        .get(source_url)
-                        .map(|s| inject::debug_id_from_bytes_hashed(&s.contents))
-                        .unwrap_or_else(|| DebugId::from_uuid(Uuid::new_v4()));
-                    debug_ids.push((source_url.clone(), debug_id));
-                    continue;
-                }
-            };
-
-            if sourcemap_url.starts_with(DATA_PREAMBLE) {
-                // source map is a url, hash the source map url for the debug id
-                let debug_id = inject::debug_id_from_bytes_hashed(sourcemap_url.as_bytes());
-                debug_ids.push((source_url.clone(), debug_id));
-            } else {
-                let sourcemap_url = normalize_sourcemap_url(source_url, sourcemap_url);
-                let sourcemap_file = match self.sources.get_mut(&sourcemap_url) {
-                    Some(sourcemap_file) => sourcemap_file,
+            // Find or generate a debug id and determine whether we can inject the
+            // code snippet at the start of the source file. This is determined by whether
+            // we are able to adjust the sourcemap accordingly.
+            let (debug_id, inject_at_start) = {
+                match sourcemap_url {
                     None => {
-                        debug!("Sourcemap file {} not found", sourcemap_url);
-                        // source map cannot be found, fall back to hashing the contents if
-                        // available.  The v4 fallback should not happen.
+                        // no source map at all, try a deterministic debug id from the contents
                         let debug_id = self
                             .sources
                             .get(source_url)
                             .map(|s| inject::debug_id_from_bytes_hashed(&s.contents))
                             .unwrap_or_else(|| DebugId::from_uuid(Uuid::new_v4()));
-                        debug_ids.push((source_url.clone(), debug_id));
-                        continue;
+                        (debug_id, false)
+                    }
+                    Some(sourcemap_url) => {
+                        if let Some(encoded) = sourcemap_url.strip_prefix(DATA_PREAMBLE) {
+                            // Handle embedded sourcemaps
+
+                            // Update the embedded sourcemap and write it back to the source file
+                            let Ok(mut decoded) = data_encoding::BASE64.decode(encoded.as_bytes()) else {
+                                bail!("Invalid embedded sourcemap in source file {source_url}");
+                            };
+
+                            inject::insert_empty_mapping(&mut decoded)?;
+                            let encoded = data_encoding::BASE64.encode(&decoded);
+                            let new_sourcemap_url = format!("{DATA_PREAMBLE}{encoded}");
+
+                            let source_file = self.sources.get_mut(source_url).unwrap();
+
+                            // hash the new source map url for the debug id
+                            let debug_id =
+                                inject::debug_id_from_bytes_hashed(new_sourcemap_url.as_bytes());
+
+                            inject::replace_sourcemap_url(
+                                &mut source_file.contents,
+                                &new_sourcemap_url,
+                            )?;
+                            *sourcemap_url = new_sourcemap_url;
+
+                            (debug_id, true)
+                        } else {
+                            // Handle external sourcemaps
+
+                            let sourcemap_url =
+                                inject::normalize_sourcemap_url(source_url, sourcemap_url);
+                            match self.sources.get_mut(&sourcemap_url) {
+                                None => {
+                                    debug!("Sourcemap file {} not found", sourcemap_url);
+                                    // source map cannot be found, fall back to hashing the contents if
+                                    // available.  The v4 fallback should not happen.
+                                    let debug_id = self
+                                        .sources
+                                        .get(source_url)
+                                        .map(|s| inject::debug_id_from_bytes_hashed(&s.contents))
+                                        .unwrap_or_else(|| DebugId::from_uuid(Uuid::new_v4()));
+                                    (debug_id, false)
+                                }
+                                Some(sourcemap_file) => {
+                                    inject::insert_empty_mapping(&mut sourcemap_file.contents)
+                                        .context(format!(
+                                            "Failed to process {}",
+                                            sourcemap_file.path.display()
+                                        ))?;
+
+                                    let (debug_id, sourcemap_modified) =
+                                        inject::fixup_sourcemap(&mut sourcemap_file.contents)
+                                            .context(format!(
+                                                "Failed to process {}",
+                                                sourcemap_file.path.display()
+                                            ))?;
+
+                                    sourcemap_file
+                                        .headers
+                                        .push(("debug-id".to_string(), debug_id.to_string()));
+
+                                    if !dry_run {
+                                        let mut file = std::fs::File::create(&sourcemap_file.path)?;
+                                        file.write_all(&sourcemap_file.contents).context(
+                                            format!(
+                                                "Failed to write sourcemap file {}",
+                                                sourcemap_file.path.display()
+                                            ),
+                                        )?;
+                                    }
+
+                                    if sourcemap_modified {
+                                        report
+                                            .sourcemaps
+                                            .push((sourcemap_file.path.clone(), debug_id));
+                                    } else {
+                                        report
+                                            .skipped_sourcemaps
+                                            .push((sourcemap_file.path.clone(), debug_id));
+                                    }
+
+                                    (debug_id, true)
+                                }
+                            }
+                        }
                     }
-                };
-
-                let (debug_id, sourcemap_modified) =
-                    inject::fixup_sourcemap(&mut sourcemap_file.contents).context(format!(
-                        "Failed to process {}",
-                        sourcemap_file.path.display()
-                    ))?;
-
-                sourcemap_file
-                    .headers
-                    .push(("debug-id".to_string(), debug_id.to_string()));
-
-                if !dry_run && sourcemap_modified {
-                    let mut file = std::fs::File::create(&sourcemap_file.path)?;
-                    file.write_all(&sourcemap_file.contents).context(format!(
-                        "Failed to write sourcemap file {}",
-                        sourcemap_file.path.display()
-                    ))?;
-                }
-
-                if sourcemap_modified {
-                    report
-                        .sourcemaps
-                        .push((sourcemap_file.path.clone(), debug_id));
-                } else {
-                    report
-                        .skipped_sourcemaps
-                        .push((sourcemap_file.path.clone(), debug_id));
                 }
+            };
 
-                debug_ids.push((source_url.clone(), debug_id));
-            }
-        }
+            // Finally, inject the debug id and the code snippet into the source file
+            let source_file = self.sources.get_mut(source_url).unwrap();
 
-        // Step 2: Iterate over the minified source files and inject the debug ids.
-        for (source_url, debug_id) in debug_ids {
-            // We only allow injection into files that match the extension
-            if !url_matches_extension(&source_url, js_extensions) {
-                debug!(
-                    "skipping potential js file {} because it does not match extension",
-                    source_url
-                );
-                continue;
+            if inject_at_start {
+                inject::fixup_js_file(&mut source_file.contents, debug_id)
+                    .context(format!("Failed to process {}", source_file.path.display()))?;
+            } else {
+                inject::fixup_js_file_end(&mut source_file.contents, debug_id)
+                    .context(format!("Failed to process {}", source_file.path.display()))?;
             }
 
-            let source_file = self.sources.get_mut(&source_url).unwrap();
-
-            fixup_js_file(&mut source_file.contents, debug_id)
-                .context(format!("Failed to process {}", source_file.path.display()))?;
-
             source_file
                 .headers
                 .push(("debug-id".to_string(), debug_id.to_string()));
             self.debug_ids.insert(source_url.clone(), debug_id);
 
             if !dry_run {
                 let mut file = std::fs::File::create(&source_file.path)?;
```

### Comparing `sentry_cli-2.18.1/src/utils/system.rs` & `sentry_cli-2.19.0/src/utils/system.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.18.1/src/utils/ui.rs` & `sentry_cli-2.19.0/src/utils/ui.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.18.1/src/utils/update.rs` & `sentry_cli-2.19.0/src/utils/update.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.18.1/src/utils/vcs.rs` & `sentry_cli-2.19.0/src/utils/vcs.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.18.1/src/utils/xcode.rs` & `sentry_cli-2.19.0/src/utils/xcode.rs`

 * *Files identical despite different names*

