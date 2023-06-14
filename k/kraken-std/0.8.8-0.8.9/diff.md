# Comparing `tmp/kraken_std-0.8.8.tar.gz` & `tmp/kraken_std-0.8.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kraken_std-0.8.8.tar", max compression
+gzip compressed data, was "kraken_std-0.8.9.tar", max compression
```

## Comparing `kraken_std-0.8.8.tar` & `kraken_std-0.8.9.tar`

### file list

```diff
@@ -1,84 +1,84 @@
--rw-r--r--   0        0        0      988 2023-04-28 15:40:23.308715 kraken_std-0.8.8/LICENSE
--rw-r--r--   0        0        0     1745 2023-04-28 15:41:06.165351 kraken_std-0.8.8/pyproject.toml
--rw-r--r--   0        0        0     1498 2023-04-28 15:40:23.308715 kraken_std-0.8.8/readme.md
--rw-r--r--   0        0        0       22 2023-04-28 15:41:06.165351 kraken_std-0.8.8/src/kraken/std/__init__.py
--rw-r--r--   0        0        0    14470 2023-04-28 15:40:23.308715 kraken_std-0.8.8/src/kraken/std/cargo/__init__.py
--rw-r--r--   0        0        0     2403 2023-04-28 15:40:23.308715 kraken_std-0.8.8/src/kraken/std/cargo/config.py
--rw-r--r--   0        0        0     1753 2023-04-28 15:40:23.308715 kraken_std-0.8.8/src/kraken/std/cargo/data/certs/cert.pem
--rw-r--r--   0        0        0     3243 2023-04-28 15:40:23.308715 kraken_std-0.8.8/src/kraken/std/cargo/data/certs/key.pem
--rw-r--r--   0        0        0     7912 2023-04-28 15:40:23.308715 kraken_std-0.8.8/src/kraken/std/cargo/manifest.py
--rw-r--r--   0        0        0     2294 2023-04-28 15:40:23.308715 kraken_std-0.8.8/src/kraken/std/cargo/mitm.py
--rw-r--r--   0        0        0     1737 2023-04-28 15:40:23.308715 kraken_std-0.8.8/src/kraken/std/cargo/mitm_impl.py
--rw-r--r--   0        0        0        0 2023-04-28 15:40:23.308715 kraken_std-0.8.8/src/kraken/std/cargo/tasks/__init__.py
--rw-r--r--   0        0        0      778 2023-04-28 15:40:23.308715 kraken_std-0.8.8/src/kraken/std/cargo/tasks/_cargo_sqlx.py
--rw-r--r--   0        0        0     5640 2023-04-28 15:40:23.308715 kraken_std-0.8.8/src/kraken/std/cargo/tasks/cargo_auth_proxy_task.py
--rw-r--r--   0        0        0     5959 2023-04-28 15:40:23.308715 kraken_std-0.8.8/src/kraken/std/cargo/tasks/cargo_build_task.py
--rw-r--r--   0        0        0     3163 2023-04-28 15:40:23.308715 kraken_std-0.8.8/src/kraken/std/cargo/tasks/cargo_bump_version_task.py
--rw-r--r--   0        0        0     2177 2023-04-28 15:40:23.308715 kraken_std-0.8.8/src/kraken/std/cargo/tasks/cargo_check_toolchain_version.py
--rw-r--r--   0        0        0      907 2023-04-28 15:40:23.308715 kraken_std-0.8.8/src/kraken/std/cargo/tasks/cargo_clippy_task.py
--rw-r--r--   0        0        0      732 2023-04-28 15:40:23.308715 kraken_std-0.8.8/src/kraken/std/cargo/tasks/cargo_deny_task.py
--rw-r--r--   0        0        0      730 2023-04-28 15:40:23.308715 kraken_std-0.8.8/src/kraken/std/cargo/tasks/cargo_fmt_task.py
--rw-r--r--   0        0        0     2074 2023-04-28 15:40:23.308715 kraken_std-0.8.8/src/kraken/std/cargo/tasks/cargo_publish_task.py
--rw-r--r--   0        0        0     1137 2023-04-28 15:40:23.308715 kraken_std-0.8.8/src/kraken/std/cargo/tasks/cargo_sqlx_migrate.py
--rw-r--r--   0        0        0      772 2023-04-28 15:40:23.308715 kraken_std-0.8.8/src/kraken/std/cargo/tasks/cargo_sqlx_prepare.py
--rw-r--r--   0        0        0     2088 2023-04-28 15:40:23.308715 kraken_std-0.8.8/src/kraken/std/cargo/tasks/cargo_sync_config_task.py
--rw-r--r--   0        0        0      493 2023-04-28 15:40:23.308715 kraken_std-0.8.8/src/kraken/std/cargo/tasks/cargo_test_task.py
--rw-r--r--   0        0        0      391 2023-04-28 15:40:23.308715 kraken_std-0.8.8/src/kraken/std/cargo/tasks/cargo_update_task.py
--rw-r--r--   0        0        0      720 2023-04-28 15:40:23.308715 kraken_std-0.8.8/src/kraken/std/cargo/version.py
--rw-r--r--   0        0        0        0 2023-04-28 15:40:23.308715 kraken_std-0.8.8/src/kraken/std/descriptors/__init__.py
--rw-r--r--   0        0        0      874 2023-04-28 15:40:23.308715 kraken_std-0.8.8/src/kraken/std/descriptors/resource.py
--rw-r--r--   0        0        0    10002 2023-04-28 15:40:23.308715 kraken_std-0.8.8/src/kraken/std/dist.py
--rw-r--r--   0        0        0     3911 2023-04-28 15:40:23.308715 kraken_std-0.8.8/src/kraken/std/docker/__init__.py
--rw-r--r--   0        0        0     3254 2023-04-28 15:40:23.308715 kraken_std-0.8.8/src/kraken/std/docker/buildx.py
--rw-r--r--   0        0        0     1426 2023-04-28 15:40:23.308715 kraken_std-0.8.8/src/kraken/std/docker/dockerapi.py
--rw-r--r--   0        0        0     8949 2023-04-28 15:40:23.308715 kraken_std-0.8.8/src/kraken/std/docker/kaniko.py
--rw-r--r--   0        0        0     1938 2023-04-28 15:40:23.308715 kraken_std-0.8.8/src/kraken/std/docker/manifest_tool.py
--rw-r--r--   0        0        0     3650 2023-04-28 15:40:23.308715 kraken_std-0.8.8/src/kraken/std/docker/native.py
--rw-r--r--   0        0        0        0 2023-04-28 15:40:23.308715 kraken_std-0.8.8/src/kraken/std/docker/py.typed
--rw-r--r--   0        0        0     2264 2023-04-28 15:40:23.308715 kraken_std-0.8.8/src/kraken/std/docker/util.py
--rw-r--r--   0        0        0     1761 2023-04-28 15:40:23.312715 kraken_std-0.8.8/src/kraken/std/git/__init__.py
--rw-r--r--   0        0        0     1107 2023-04-28 15:40:23.312715 kraken_std-0.8.8/src/kraken/std/git/config.py
--rw-r--r--   0        0        0     9451 2023-04-28 15:40:23.312715 kraken_std-0.8.8/src/kraken/std/git/gitignore.py
--rw-r--r--   0        0        0        0 2023-04-28 15:40:23.312715 kraken_std-0.8.8/src/kraken/std/git/tasks/__init__.py
--rw-r--r--   0        0        0      448 2023-04-28 15:40:23.312715 kraken_std-0.8.8/src/kraken/std/git/tasks/const.py
--rw-r--r--   0        0        0     2919 2023-04-28 15:40:23.312715 kraken_std-0.8.8/src/kraken/std/git/tasks/gitignore_check_task.py
--rw-r--r--   0        0        0     2754 2023-04-28 15:40:23.312715 kraken_std-0.8.8/src/kraken/std/git/tasks/gitignore_sync_task.py
--rw-r--r--   0        0        0     2973 2023-04-28 15:40:23.312715 kraken_std-0.8.8/src/kraken/std/git/version.py
--rw-r--r--   0        0        0     6368 2023-04-28 15:40:23.312715 kraken_std-0.8.8/src/kraken/std/helm/__init__.py
--rw-r--r--   0        0        0     2132 2023-04-28 15:40:23.312715 kraken_std-0.8.8/src/kraken/std/helm/helmapi.py
--rw-r--r--   0        0        0     2310 2023-04-28 15:40:23.312715 kraken_std-0.8.8/src/kraken/std/http/__init__.py
--rw-r--r--   0        0        0     3431 2023-04-28 15:40:23.312715 kraken_std-0.8.8/src/kraken/std/http/lint_ban_bare_requests.py
--rw-r--r--   0        0        0        0 2023-04-28 15:40:23.312715 kraken_std-0.8.8/src/kraken/std/py.typed
--rw-r--r--   0        0        0     1670 2023-04-28 15:40:23.312715 kraken_std-0.8.8/src/kraken/std/python/__init__.py
--rw-r--r--   0        0        0     3586 2023-04-28 15:40:23.312715 kraken_std-0.8.8/src/kraken/std/python/buildsystem/__init__.py
--rw-r--r--   0        0        0     1332 2023-04-28 15:40:23.312715 kraken_std-0.8.8/src/kraken/std/python/buildsystem/helpers.py
--rw-r--r--   0        0        0     3120 2023-04-28 15:40:23.312715 kraken_std-0.8.8/src/kraken/std/python/buildsystem/maturin.py
--rw-r--r--   0        0        0     7985 2023-04-28 15:40:23.312715 kraken_std-0.8.8/src/kraken/std/python/buildsystem/poetry.py
--rw-r--r--   0        0        0     4415 2023-04-28 15:40:23.312715 kraken_std-0.8.8/src/kraken/std/python/buildsystem/slap.py
--rw-r--r--   0        0        0     6406 2023-04-28 15:40:23.312715 kraken_std-0.8.8/src/kraken/std/python/pyproject.py
--rw-r--r--   0        0        0     6401 2023-04-28 15:40:23.312715 kraken_std-0.8.8/src/kraken/std/python/settings.py
--rw-r--r--   0        0        0        0 2023-04-28 15:40:23.312715 kraken_std-0.8.8/src/kraken/std/python/tasks/__init__.py
--rw-r--r--   0        0        0     3249 2023-04-28 15:40:23.312715 kraken_std-0.8.8/src/kraken/std/python/tasks/base_task.py
--rw-r--r--   0        0        0     2076 2023-04-28 15:40:23.312715 kraken_std-0.8.8/src/kraken/std/python/tasks/black_task.py
--rw-r--r--   0        0        0     1922 2023-04-28 15:40:23.312715 kraken_std-0.8.8/src/kraken/std/python/tasks/build_task.py
--rw-r--r--   0        0        0     1046 2023-04-28 15:40:23.312715 kraken_std-0.8.8/src/kraken/std/python/tasks/flake8_task.py
--rw-r--r--   0        0        0     2377 2023-04-28 15:40:23.312715 kraken_std-0.8.8/src/kraken/std/python/tasks/info_task.py
--rw-r--r--   0        0        0     2834 2023-04-28 15:40:23.312715 kraken_std-0.8.8/src/kraken/std/python/tasks/install_task.py
--rw-r--r--   0        0        0     1844 2023-04-28 15:40:23.312715 kraken_std-0.8.8/src/kraken/std/python/tasks/isort_task.py
--rw-r--r--   0        0        0      946 2023-04-28 15:40:23.312715 kraken_std-0.8.8/src/kraken/std/python/tasks/login_task.py
--rw-r--r--   0        0        0     1463 2023-04-28 15:40:23.312715 kraken_std-0.8.8/src/kraken/std/python/tasks/mypy_subtest_task.py
--rw-r--r--   0        0        0     2352 2023-04-28 15:40:23.312715 kraken_std-0.8.8/src/kraken/std/python/tasks/mypy_task.py
--rw-r--r--   0        0        0     2598 2023-04-28 15:40:23.312715 kraken_std-0.8.8/src/kraken/std/python/tasks/publish_task.py
--rw-r--r--   0        0        0     2043 2023-04-28 15:40:23.312715 kraken_std-0.8.8/src/kraken/std/python/tasks/pycln_task.py
--rw-r--r--   0        0        0     1034 2023-04-28 15:40:23.312715 kraken_std-0.8.8/src/kraken/std/python/tasks/pylint_task.py
--rw-r--r--   0        0        0     2398 2023-04-28 15:40:23.312715 kraken_std-0.8.8/src/kraken/std/python/tasks/pytest_task.py
--rw-r--r--   0        0        0     4531 2023-04-28 15:40:23.312715 kraken_std-0.8.8/src/kraken/std/python/tasks/pyupgrade_task.py
--rw-r--r--   0        0        0     1778 2023-04-28 15:40:23.312715 kraken_std-0.8.8/src/kraken/std/python/tasks/update_lockfile_task.py
--rw-r--r--   0        0        0     1656 2023-04-28 15:40:23.312715 kraken_std-0.8.8/src/kraken/std/python/tasks/update_pyproject_task.py
--rw-r--r--   0        0        0     1127 2023-04-28 15:40:23.312715 kraken_std-0.8.8/src/kraken/std/python/version.py
--rw-r--r--   0        0        0     4042 2023-04-28 15:40:23.312715 kraken_std-0.8.8/src/kraken/std/sccache.py
--rw-r--r--   0        0        0      390 2023-04-28 15:40:23.312715 kraken_std-0.8.8/src/kraken/std/util/__init__.py
--rw-r--r--   0        0        0     1906 2023-04-28 15:40:23.312715 kraken_std-0.8.8/src/kraken/std/util/check_file_exists_and_is_committed_task.py
--rw-r--r--   0        0        0     6010 2023-04-28 15:40:23.312715 kraken_std-0.8.8/src/kraken/std/util/check_valid_readme_exists_task.py
--rw-r--r--   0        0        0     2645 2023-04-28 15:40:23.312715 kraken_std-0.8.8/src/kraken/std/util/copyright_task.py
--rw-r--r--   0        0        0     2516 1970-01-01 00:00:00.000000 kraken_std-0.8.8/PKG-INFO
+-rw-r--r--   0        0        0      988 2023-04-28 16:47:27.024684 kraken_std-0.8.9/LICENSE
+-rw-r--r--   0        0        0     1745 2023-04-28 16:48:24.819025 kraken_std-0.8.9/pyproject.toml
+-rw-r--r--   0        0        0     1498 2023-04-28 16:47:27.024684 kraken_std-0.8.9/readme.md
+-rw-r--r--   0        0        0       22 2023-04-28 16:48:24.819025 kraken_std-0.8.9/src/kraken/std/__init__.py
+-rw-r--r--   0        0        0    14524 2023-04-28 16:47:27.024684 kraken_std-0.8.9/src/kraken/std/cargo/__init__.py
+-rw-r--r--   0        0        0     2403 2023-04-28 16:47:27.024684 kraken_std-0.8.9/src/kraken/std/cargo/config.py
+-rw-r--r--   0        0        0     1753 2023-04-28 16:47:27.024684 kraken_std-0.8.9/src/kraken/std/cargo/data/certs/cert.pem
+-rw-r--r--   0        0        0     3243 2023-04-28 16:47:27.024684 kraken_std-0.8.9/src/kraken/std/cargo/data/certs/key.pem
+-rw-r--r--   0        0        0     7912 2023-04-28 16:47:27.024684 kraken_std-0.8.9/src/kraken/std/cargo/manifest.py
+-rw-r--r--   0        0        0     2294 2023-04-28 16:47:27.024684 kraken_std-0.8.9/src/kraken/std/cargo/mitm.py
+-rw-r--r--   0        0        0     1737 2023-04-28 16:47:27.024684 kraken_std-0.8.9/src/kraken/std/cargo/mitm_impl.py
+-rw-r--r--   0        0        0        0 2023-04-28 16:47:27.024684 kraken_std-0.8.9/src/kraken/std/cargo/tasks/__init__.py
+-rw-r--r--   0        0        0      778 2023-04-28 16:47:27.024684 kraken_std-0.8.9/src/kraken/std/cargo/tasks/_cargo_sqlx.py
+-rw-r--r--   0        0        0     5640 2023-04-28 16:47:27.024684 kraken_std-0.8.9/src/kraken/std/cargo/tasks/cargo_auth_proxy_task.py
+-rw-r--r--   0        0        0     5959 2023-04-28 16:47:27.028684 kraken_std-0.8.9/src/kraken/std/cargo/tasks/cargo_build_task.py
+-rw-r--r--   0        0        0     3163 2023-04-28 16:47:27.028684 kraken_std-0.8.9/src/kraken/std/cargo/tasks/cargo_bump_version_task.py
+-rw-r--r--   0        0        0     2177 2023-04-28 16:47:27.028684 kraken_std-0.8.9/src/kraken/std/cargo/tasks/cargo_check_toolchain_version.py
+-rw-r--r--   0        0        0      907 2023-04-28 16:47:27.028684 kraken_std-0.8.9/src/kraken/std/cargo/tasks/cargo_clippy_task.py
+-rw-r--r--   0        0        0      732 2023-04-28 16:47:27.028684 kraken_std-0.8.9/src/kraken/std/cargo/tasks/cargo_deny_task.py
+-rw-r--r--   0        0        0      730 2023-04-28 16:47:27.028684 kraken_std-0.8.9/src/kraken/std/cargo/tasks/cargo_fmt_task.py
+-rw-r--r--   0        0        0     2074 2023-04-28 16:47:27.028684 kraken_std-0.8.9/src/kraken/std/cargo/tasks/cargo_publish_task.py
+-rw-r--r--   0        0        0     1137 2023-04-28 16:47:27.028684 kraken_std-0.8.9/src/kraken/std/cargo/tasks/cargo_sqlx_migrate.py
+-rw-r--r--   0        0        0      772 2023-04-28 16:47:27.028684 kraken_std-0.8.9/src/kraken/std/cargo/tasks/cargo_sqlx_prepare.py
+-rw-r--r--   0        0        0     2088 2023-04-28 16:47:27.028684 kraken_std-0.8.9/src/kraken/std/cargo/tasks/cargo_sync_config_task.py
+-rw-r--r--   0        0        0      493 2023-04-28 16:47:27.028684 kraken_std-0.8.9/src/kraken/std/cargo/tasks/cargo_test_task.py
+-rw-r--r--   0        0        0      391 2023-04-28 16:47:27.028684 kraken_std-0.8.9/src/kraken/std/cargo/tasks/cargo_update_task.py
+-rw-r--r--   0        0        0      720 2023-04-28 16:47:27.028684 kraken_std-0.8.9/src/kraken/std/cargo/version.py
+-rw-r--r--   0        0        0        0 2023-04-28 16:47:27.028684 kraken_std-0.8.9/src/kraken/std/descriptors/__init__.py
+-rw-r--r--   0        0        0      874 2023-04-28 16:47:27.028684 kraken_std-0.8.9/src/kraken/std/descriptors/resource.py
+-rw-r--r--   0        0        0    10002 2023-04-28 16:47:27.028684 kraken_std-0.8.9/src/kraken/std/dist.py
+-rw-r--r--   0        0        0     3911 2023-04-28 16:47:27.028684 kraken_std-0.8.9/src/kraken/std/docker/__init__.py
+-rw-r--r--   0        0        0     3254 2023-04-28 16:47:27.028684 kraken_std-0.8.9/src/kraken/std/docker/buildx.py
+-rw-r--r--   0        0        0     1426 2023-04-28 16:47:27.028684 kraken_std-0.8.9/src/kraken/std/docker/dockerapi.py
+-rw-r--r--   0        0        0     8949 2023-04-28 16:47:27.028684 kraken_std-0.8.9/src/kraken/std/docker/kaniko.py
+-rw-r--r--   0        0        0     1938 2023-04-28 16:47:27.028684 kraken_std-0.8.9/src/kraken/std/docker/manifest_tool.py
+-rw-r--r--   0        0        0     3650 2023-04-28 16:47:27.028684 kraken_std-0.8.9/src/kraken/std/docker/native.py
+-rw-r--r--   0        0        0        0 2023-04-28 16:47:27.028684 kraken_std-0.8.9/src/kraken/std/docker/py.typed
+-rw-r--r--   0        0        0     2264 2023-04-28 16:47:27.028684 kraken_std-0.8.9/src/kraken/std/docker/util.py
+-rw-r--r--   0        0        0     1761 2023-04-28 16:47:27.028684 kraken_std-0.8.9/src/kraken/std/git/__init__.py
+-rw-r--r--   0        0        0     1107 2023-04-28 16:47:27.028684 kraken_std-0.8.9/src/kraken/std/git/config.py
+-rw-r--r--   0        0        0     9451 2023-04-28 16:47:27.028684 kraken_std-0.8.9/src/kraken/std/git/gitignore.py
+-rw-r--r--   0        0        0        0 2023-04-28 16:47:27.028684 kraken_std-0.8.9/src/kraken/std/git/tasks/__init__.py
+-rw-r--r--   0        0        0      448 2023-04-28 16:47:27.028684 kraken_std-0.8.9/src/kraken/std/git/tasks/const.py
+-rw-r--r--   0        0        0     2919 2023-04-28 16:47:27.028684 kraken_std-0.8.9/src/kraken/std/git/tasks/gitignore_check_task.py
+-rw-r--r--   0        0        0     2754 2023-04-28 16:47:27.028684 kraken_std-0.8.9/src/kraken/std/git/tasks/gitignore_sync_task.py
+-rw-r--r--   0        0        0     2973 2023-04-28 16:47:27.028684 kraken_std-0.8.9/src/kraken/std/git/version.py
+-rw-r--r--   0        0        0     6368 2023-04-28 16:47:27.028684 kraken_std-0.8.9/src/kraken/std/helm/__init__.py
+-rw-r--r--   0        0        0     2132 2023-04-28 16:47:27.028684 kraken_std-0.8.9/src/kraken/std/helm/helmapi.py
+-rw-r--r--   0        0        0     2310 2023-04-28 16:47:27.028684 kraken_std-0.8.9/src/kraken/std/http/__init__.py
+-rw-r--r--   0        0        0     3431 2023-04-28 16:47:27.028684 kraken_std-0.8.9/src/kraken/std/http/lint_ban_bare_requests.py
+-rw-r--r--   0        0        0        0 2023-04-28 16:47:27.028684 kraken_std-0.8.9/src/kraken/std/py.typed
+-rw-r--r--   0        0        0     1670 2023-04-28 16:47:27.028684 kraken_std-0.8.9/src/kraken/std/python/__init__.py
+-rw-r--r--   0        0        0     3586 2023-04-28 16:47:27.032684 kraken_std-0.8.9/src/kraken/std/python/buildsystem/__init__.py
+-rw-r--r--   0        0        0     1332 2023-04-28 16:47:27.032684 kraken_std-0.8.9/src/kraken/std/python/buildsystem/helpers.py
+-rw-r--r--   0        0        0     3120 2023-04-28 16:47:27.032684 kraken_std-0.8.9/src/kraken/std/python/buildsystem/maturin.py
+-rw-r--r--   0        0        0     7985 2023-04-28 16:47:27.032684 kraken_std-0.8.9/src/kraken/std/python/buildsystem/poetry.py
+-rw-r--r--   0        0        0     4415 2023-04-28 16:47:27.032684 kraken_std-0.8.9/src/kraken/std/python/buildsystem/slap.py
+-rw-r--r--   0        0        0     6406 2023-04-28 16:47:27.032684 kraken_std-0.8.9/src/kraken/std/python/pyproject.py
+-rw-r--r--   0        0        0     6401 2023-04-28 16:47:27.032684 kraken_std-0.8.9/src/kraken/std/python/settings.py
+-rw-r--r--   0        0        0        0 2023-04-28 16:47:27.032684 kraken_std-0.8.9/src/kraken/std/python/tasks/__init__.py
+-rw-r--r--   0        0        0     3249 2023-04-28 16:47:27.032684 kraken_std-0.8.9/src/kraken/std/python/tasks/base_task.py
+-rw-r--r--   0        0        0     2076 2023-04-28 16:47:27.032684 kraken_std-0.8.9/src/kraken/std/python/tasks/black_task.py
+-rw-r--r--   0        0        0     1922 2023-04-28 16:47:27.032684 kraken_std-0.8.9/src/kraken/std/python/tasks/build_task.py
+-rw-r--r--   0        0        0     1046 2023-04-28 16:47:27.032684 kraken_std-0.8.9/src/kraken/std/python/tasks/flake8_task.py
+-rw-r--r--   0        0        0     2377 2023-04-28 16:47:27.032684 kraken_std-0.8.9/src/kraken/std/python/tasks/info_task.py
+-rw-r--r--   0        0        0     2834 2023-04-28 16:47:27.032684 kraken_std-0.8.9/src/kraken/std/python/tasks/install_task.py
+-rw-r--r--   0        0        0     1844 2023-04-28 16:47:27.032684 kraken_std-0.8.9/src/kraken/std/python/tasks/isort_task.py
+-rw-r--r--   0        0        0      946 2023-04-28 16:47:27.032684 kraken_std-0.8.9/src/kraken/std/python/tasks/login_task.py
+-rw-r--r--   0        0        0     1463 2023-04-28 16:47:27.032684 kraken_std-0.8.9/src/kraken/std/python/tasks/mypy_subtest_task.py
+-rw-r--r--   0        0        0     2352 2023-04-28 16:47:27.032684 kraken_std-0.8.9/src/kraken/std/python/tasks/mypy_task.py
+-rw-r--r--   0        0        0     2598 2023-04-28 16:47:27.032684 kraken_std-0.8.9/src/kraken/std/python/tasks/publish_task.py
+-rw-r--r--   0        0        0     2043 2023-04-28 16:47:27.032684 kraken_std-0.8.9/src/kraken/std/python/tasks/pycln_task.py
+-rw-r--r--   0        0        0     1034 2023-04-28 16:47:27.032684 kraken_std-0.8.9/src/kraken/std/python/tasks/pylint_task.py
+-rw-r--r--   0        0        0     2398 2023-04-28 16:47:27.032684 kraken_std-0.8.9/src/kraken/std/python/tasks/pytest_task.py
+-rw-r--r--   0        0        0     4531 2023-04-28 16:47:27.032684 kraken_std-0.8.9/src/kraken/std/python/tasks/pyupgrade_task.py
+-rw-r--r--   0        0        0     1778 2023-04-28 16:47:27.032684 kraken_std-0.8.9/src/kraken/std/python/tasks/update_lockfile_task.py
+-rw-r--r--   0        0        0     1656 2023-04-28 16:47:27.032684 kraken_std-0.8.9/src/kraken/std/python/tasks/update_pyproject_task.py
+-rw-r--r--   0        0        0     1127 2023-04-28 16:47:27.032684 kraken_std-0.8.9/src/kraken/std/python/version.py
+-rw-r--r--   0        0        0     4042 2023-04-28 16:47:27.032684 kraken_std-0.8.9/src/kraken/std/sccache.py
+-rw-r--r--   0        0        0      390 2023-04-28 16:47:27.032684 kraken_std-0.8.9/src/kraken/std/util/__init__.py
+-rw-r--r--   0        0        0     1906 2023-04-28 16:47:27.032684 kraken_std-0.8.9/src/kraken/std/util/check_file_exists_and_is_committed_task.py
+-rw-r--r--   0        0        0     6010 2023-04-28 16:47:27.032684 kraken_std-0.8.9/src/kraken/std/util/check_valid_readme_exists_task.py
+-rw-r--r--   0        0        0     2645 2023-04-28 16:47:27.032684 kraken_std-0.8.9/src/kraken/std/util/copyright_task.py
+-rw-r--r--   0        0        0     2516 1970-01-01 00:00:00.000000 kraken_std-0.8.9/PKG-INFO
```

### Comparing `kraken_std-0.8.8/LICENSE` & `kraken_std-0.8.9/LICENSE`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.8/pyproject.toml` & `kraken_std-0.8.9/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "kraken-std"
-version = "0.8.8"
+version = "0.8.9"
 description = "The Kraken standard library."
 authors = ["Niklas Rosenstein <rosensteinniklas@gmail.com>"]
 license = "MIT"
 readme = "readme.md"
 packages = [{ include = "kraken/std", from = "src" }]
 classifiers = []
 keywords = []
```

### Comparing `kraken_std-0.8.8/readme.md` & `kraken_std-0.8.9/readme.md`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.8/src/kraken/std/cargo/__init__.py` & `kraken_std-0.8.9/src/kraken/std/cargo/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,25 +30,27 @@
     "cargo_bump_version",
     "cargo_clippy",
     "cargo_deny",
     "cargo_fmt",
     "cargo_publish",
     "cargo_registry",
     "cargo_sqlx_migrate",
+    "cargo_sqlx_prepare",
     "cargo_sync_config",
     "cargo_update",
     "CargoAuthProxyTask",
     "CargoBuildTask",
     "CargoBumpVersionTask",
     "CargoClippyTask",
     "CargoDenyTask",
     "CargoProject",
     "CargoPublishTask",
     "CargoRegistry",
     "CargoSqlxMigrateTask",
+    "CargoSqlxPrepareTask",
     "CargoSyncConfigTask",
     "CargoTestTask",
     "cargo_check_toolchain_version",
     "CargoCheckToolchainVersionTask",
 ]
 
 #: This is the name of a group in every project that contains Cargo tasks to contain the tasks that either support
```

### Comparing `kraken_std-0.8.8/src/kraken/std/cargo/config.py` & `kraken_std-0.8.9/src/kraken/std/cargo/config.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.8/src/kraken/std/cargo/data/certs/cert.pem` & `kraken_std-0.8.9/src/kraken/std/cargo/data/certs/cert.pem`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.8/src/kraken/std/cargo/data/certs/key.pem` & `kraken_std-0.8.9/src/kraken/std/cargo/data/certs/key.pem`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.8/src/kraken/std/cargo/manifest.py` & `kraken_std-0.8.9/src/kraken/std/cargo/manifest.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.8/src/kraken/std/cargo/mitm.py` & `kraken_std-0.8.9/src/kraken/std/cargo/mitm.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.8/src/kraken/std/cargo/mitm_impl.py` & `kraken_std-0.8.9/src/kraken/std/cargo/mitm_impl.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.8/src/kraken/std/cargo/tasks/_cargo_sqlx.py` & `kraken_std-0.8.9/src/kraken/std/cargo/tasks/_cargo_sqlx.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.8/src/kraken/std/cargo/tasks/cargo_auth_proxy_task.py` & `kraken_std-0.8.9/src/kraken/std/cargo/tasks/cargo_auth_proxy_task.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.8/src/kraken/std/cargo/tasks/cargo_build_task.py` & `kraken_std-0.8.9/src/kraken/std/cargo/tasks/cargo_build_task.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.8/src/kraken/std/cargo/tasks/cargo_bump_version_task.py` & `kraken_std-0.8.9/src/kraken/std/cargo/tasks/cargo_bump_version_task.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.8/src/kraken/std/cargo/tasks/cargo_check_toolchain_version.py` & `kraken_std-0.8.9/src/kraken/std/cargo/tasks/cargo_check_toolchain_version.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.8/src/kraken/std/cargo/tasks/cargo_clippy_task.py` & `kraken_std-0.8.9/src/kraken/std/cargo/tasks/cargo_clippy_task.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.8/src/kraken/std/cargo/tasks/cargo_deny_task.py` & `kraken_std-0.8.9/src/kraken/std/cargo/tasks/cargo_deny_task.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.8/src/kraken/std/cargo/tasks/cargo_fmt_task.py` & `kraken_std-0.8.9/src/kraken/std/cargo/tasks/cargo_fmt_task.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.8/src/kraken/std/cargo/tasks/cargo_publish_task.py` & `kraken_std-0.8.9/src/kraken/std/cargo/tasks/cargo_publish_task.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.8/src/kraken/std/cargo/tasks/cargo_sqlx_migrate.py` & `kraken_std-0.8.9/src/kraken/std/cargo/tasks/cargo_sqlx_migrate.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.8/src/kraken/std/cargo/tasks/cargo_sqlx_prepare.py` & `kraken_std-0.8.9/src/kraken/std/cargo/tasks/cargo_sqlx_prepare.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.8/src/kraken/std/cargo/tasks/cargo_sync_config_task.py` & `kraken_std-0.8.9/src/kraken/std/cargo/tasks/cargo_sync_config_task.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.8/src/kraken/std/cargo/version.py` & `kraken_std-0.8.9/src/kraken/std/cargo/version.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.8/src/kraken/std/descriptors/resource.py` & `kraken_std-0.8.9/src/kraken/std/descriptors/resource.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.8/src/kraken/std/dist.py` & `kraken_std-0.8.9/src/kraken/std/dist.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.8/src/kraken/std/docker/__init__.py` & `kraken_std-0.8.9/src/kraken/std/docker/__init__.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.8/src/kraken/std/docker/buildx.py` & `kraken_std-0.8.9/src/kraken/std/docker/buildx.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.8/src/kraken/std/docker/dockerapi.py` & `kraken_std-0.8.9/src/kraken/std/docker/dockerapi.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.8/src/kraken/std/docker/kaniko.py` & `kraken_std-0.8.9/src/kraken/std/docker/kaniko.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.8/src/kraken/std/docker/manifest_tool.py` & `kraken_std-0.8.9/src/kraken/std/docker/manifest_tool.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.8/src/kraken/std/docker/native.py` & `kraken_std-0.8.9/src/kraken/std/docker/native.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.8/src/kraken/std/docker/util.py` & `kraken_std-0.8.9/src/kraken/std/docker/util.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.8/src/kraken/std/git/__init__.py` & `kraken_std-0.8.9/src/kraken/std/git/__init__.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.8/src/kraken/std/git/config.py` & `kraken_std-0.8.9/src/kraken/std/git/config.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.8/src/kraken/std/git/gitignore.py` & `kraken_std-0.8.9/src/kraken/std/git/gitignore.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.8/src/kraken/std/git/tasks/gitignore_check_task.py` & `kraken_std-0.8.9/src/kraken/std/git/tasks/gitignore_check_task.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.8/src/kraken/std/git/tasks/gitignore_sync_task.py` & `kraken_std-0.8.9/src/kraken/std/git/tasks/gitignore_sync_task.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.8/src/kraken/std/git/version.py` & `kraken_std-0.8.9/src/kraken/std/git/version.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.8/src/kraken/std/helm/__init__.py` & `kraken_std-0.8.9/src/kraken/std/helm/__init__.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.8/src/kraken/std/helm/helmapi.py` & `kraken_std-0.8.9/src/kraken/std/helm/helmapi.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.8/src/kraken/std/http/__init__.py` & `kraken_std-0.8.9/src/kraken/std/http/__init__.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.8/src/kraken/std/http/lint_ban_bare_requests.py` & `kraken_std-0.8.9/src/kraken/std/http/lint_ban_bare_requests.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.8/src/kraken/std/python/__init__.py` & `kraken_std-0.8.9/src/kraken/std/python/__init__.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.8/src/kraken/std/python/buildsystem/__init__.py` & `kraken_std-0.8.9/src/kraken/std/python/buildsystem/__init__.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.8/src/kraken/std/python/buildsystem/helpers.py` & `kraken_std-0.8.9/src/kraken/std/python/buildsystem/helpers.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.8/src/kraken/std/python/buildsystem/maturin.py` & `kraken_std-0.8.9/src/kraken/std/python/buildsystem/maturin.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.8/src/kraken/std/python/buildsystem/poetry.py` & `kraken_std-0.8.9/src/kraken/std/python/buildsystem/poetry.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.8/src/kraken/std/python/buildsystem/slap.py` & `kraken_std-0.8.9/src/kraken/std/python/buildsystem/slap.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.8/src/kraken/std/python/pyproject.py` & `kraken_std-0.8.9/src/kraken/std/python/pyproject.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.8/src/kraken/std/python/settings.py` & `kraken_std-0.8.9/src/kraken/std/python/settings.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.8/src/kraken/std/python/tasks/base_task.py` & `kraken_std-0.8.9/src/kraken/std/python/tasks/base_task.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.8/src/kraken/std/python/tasks/black_task.py` & `kraken_std-0.8.9/src/kraken/std/python/tasks/black_task.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.8/src/kraken/std/python/tasks/build_task.py` & `kraken_std-0.8.9/src/kraken/std/python/tasks/build_task.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.8/src/kraken/std/python/tasks/flake8_task.py` & `kraken_std-0.8.9/src/kraken/std/python/tasks/flake8_task.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.8/src/kraken/std/python/tasks/info_task.py` & `kraken_std-0.8.9/src/kraken/std/python/tasks/info_task.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.8/src/kraken/std/python/tasks/install_task.py` & `kraken_std-0.8.9/src/kraken/std/python/tasks/install_task.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.8/src/kraken/std/python/tasks/isort_task.py` & `kraken_std-0.8.9/src/kraken/std/python/tasks/isort_task.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.8/src/kraken/std/python/tasks/login_task.py` & `kraken_std-0.8.9/src/kraken/std/python/tasks/login_task.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.8/src/kraken/std/python/tasks/mypy_subtest_task.py` & `kraken_std-0.8.9/src/kraken/std/python/tasks/mypy_subtest_task.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.8/src/kraken/std/python/tasks/mypy_task.py` & `kraken_std-0.8.9/src/kraken/std/python/tasks/mypy_task.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.8/src/kraken/std/python/tasks/publish_task.py` & `kraken_std-0.8.9/src/kraken/std/python/tasks/publish_task.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.8/src/kraken/std/python/tasks/pycln_task.py` & `kraken_std-0.8.9/src/kraken/std/python/tasks/pycln_task.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.8/src/kraken/std/python/tasks/pylint_task.py` & `kraken_std-0.8.9/src/kraken/std/python/tasks/pylint_task.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.8/src/kraken/std/python/tasks/pytest_task.py` & `kraken_std-0.8.9/src/kraken/std/python/tasks/pytest_task.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.8/src/kraken/std/python/tasks/pyupgrade_task.py` & `kraken_std-0.8.9/src/kraken/std/python/tasks/pyupgrade_task.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.8/src/kraken/std/python/tasks/update_lockfile_task.py` & `kraken_std-0.8.9/src/kraken/std/python/tasks/update_lockfile_task.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.8/src/kraken/std/python/tasks/update_pyproject_task.py` & `kraken_std-0.8.9/src/kraken/std/python/tasks/update_pyproject_task.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.8/src/kraken/std/python/version.py` & `kraken_std-0.8.9/src/kraken/std/python/version.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.8/src/kraken/std/sccache.py` & `kraken_std-0.8.9/src/kraken/std/sccache.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.8/src/kraken/std/util/check_file_exists_and_is_committed_task.py` & `kraken_std-0.8.9/src/kraken/std/util/check_file_exists_and_is_committed_task.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.8/src/kraken/std/util/check_valid_readme_exists_task.py` & `kraken_std-0.8.9/src/kraken/std/util/check_valid_readme_exists_task.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.8/src/kraken/std/util/copyright_task.py` & `kraken_std-0.8.9/src/kraken/std/util/copyright_task.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.8/PKG-INFO` & `kraken_std-0.8.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kraken-std
-Version: 0.8.8
+Version: 0.8.9
 Summary: The Kraken standard library.
 License: MIT
 Author: Niklas Rosenstein
 Author-email: rosensteinniklas@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

