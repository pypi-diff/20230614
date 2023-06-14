# Comparing `tmp/pdm-mina-0.2.1.tar.gz` & `tmp/pdm_mina-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdm-mina-0.2.1.tar", last modified: Sun Dec 25 09:41:31 2022, max compression
+gzip compressed data, was "pdm_mina-0.2.2.tar", last modified: Wed Jun 14 12:12:15 2023, max compression
```

## Comparing `pdm-mina-0.2.1.tar` & `pdm_mina-0.2.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-rw-rw-   0        0        0        0 2022-12-25 09:34:05.034518 pdm-mina-0.2.1/mina/__init__.py
--rw-rw-rw-   0        0        0        0 2022-12-25 09:34:05.036472 pdm-mina-0.2.1/mina/commands/__init__.py
--rw-rw-rw-   0        0        0     5787 2022-12-25 09:39:56.579189 pdm-mina-0.2.1/mina/commands/build.py
--rw-rw-rw-   0        0        0     1195 2022-12-25 09:39:56.283766 pdm-mina-0.2.1/mina/commands/list.py
--rw-rw-rw-   0        0        0      832 2022-12-25 09:34:05.037449 pdm-mina-0.2.1/mina/plugin.py
--rw-rw-rw-   0        0        0     1435 2022-12-25 09:41:13.215550 pdm-mina-0.2.1/pyproject.toml
--rw-rw-rw-   0        0        0     4279 2022-12-25 09:34:05.033543 pdm-mina-0.2.1/README.md
--rw-rw-rw-   0        0        0     4280 2022-12-25 09:41:31.232497 pdm-mina-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     4153 2023-06-14 12:12:03.795548 pdm_mina-0.2.2/README.md
+-rw-r--r--   0        0        0        0 2023-06-14 12:12:03.795548 pdm_mina-0.2.2/mina/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-14 12:12:03.795548 pdm_mina-0.2.2/mina/commands/__init__.py
+-rw-r--r--   0        0        0     5621 2023-06-14 12:12:03.795548 pdm_mina-0.2.2/mina/commands/build.py
+-rw-r--r--   0        0        0     1160 2023-06-14 12:12:03.795548 pdm_mina-0.2.2/mina/commands/list.py
+-rw-r--r--   0        0        0      804 2023-06-14 12:12:03.795548 pdm_mina-0.2.2/mina/plugin.py
+-rw-r--r--   0        0        0     1562 2023-06-14 12:12:15.960226 pdm_mina-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     4394 1970-01-01 00:00:00.000000 pdm_mina-0.2.2/PKG-INFO
```

### Comparing `pdm-mina-0.2.1/mina/commands/build.py` & `pdm_mina-0.2.2/mina/commands/build.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,167 +1,167 @@
-from __future__ import annotations
-
-import argparse
-import shutil
-import sys
-from pathlib import Path
-
-try:
-    import tomllib as tomli  # type: ignore
-except ImportError:
-    try:
-        from pdm.pep517._vendor import tomli
-    except ImportError:
-        import tomli
-from pdm.builders.sdist import SdistBuilder
-from pdm.builders.wheel import WheelBuilder
-from pdm.cli.commands.base import BaseCommand
-from pdm.exceptions import ProjectError
-from pdm.project.core import Project
-
-
-def do_build_mina(
-    project: Project,
-    packages: list[str],
-    option_sdist: bool = True,
-    option_wheel: bool = True,
-    option_dest: str = "dist",
-    option_clean: bool = True,
-    config_settings: dict[str, str] | None = None,
-):
-    if project.is_global:
-        project.core.ui.echo("You can't build packages in global project.", err=True)
-        raise ProjectError("Global project not supported")
-    if not option_wheel and not option_sdist:
-        project.core.ui.echo("You must build at least one of sdist or wheel.", err=True)
-        raise ProjectError("No build type specified")
-    dest = Path(option_dest).absolute()
-    if option_clean:
-        shutil.rmtree(dest, ignore_errors=True)
-    artifacts: list[str] = []
-    for package in packages:
-        settings = (config_settings or {}).copy()
-        settings.setdefault("--mina-target", package)
-        project.core.ui.echo(f"Building package {package}...")
-        with project.core.ui.logging("Building packages"):
-            if option_sdist:
-                project.core.ui.echo("  - Building sdist")
-                loc = SdistBuilder(project.root, project.environment).build(
-                    option_dest, settings
-                )
-                project.core.ui.echo(f"    - completed: {loc}")
-                artifacts.append(loc)
-            if option_wheel:
-                project.core.ui.echo("  - Building wheel")
-                loc = WheelBuilder(project.root, project.environment).build(
-                    option_dest, settings
-                )
-                project.core.ui.echo(f"    - completed: {loc}")
-                artifacts.append(loc)
-            project.core.ui.echo(f"{package} build completed.")
-    project.core.ui.echo(
-        f"Successfully built {len(packages)} packages: {len(artifacts)} artifacts"
-    )
-    return artifacts
-
-
-class MinaCommandNamespace:
-    packages: list[str]
-    all: bool
-    sdist: bool
-    wheel: bool
-    dest: str
-    clean: bool
-    config_setting: list[str]
-
-
-class MinaBuildCommand(BaseCommand):
-    def add_arguments(self, parser: argparse.ArgumentParser) -> None:
-        parser.add_argument(
-            "packages",
-            nargs="*",
-            help="Packages to build, which must be defined in pyproject.toml.",
-        )
-        parser.add_argument(
-            "-a",
-            "--all",
-            default=False,
-            action="store_true",
-            help="Build all packages.",
-        )
-        parser.add_argument(
-            "--no-sdist",
-            dest="sdist",
-            default=True,
-            action="store_false",
-            help="Don't build source tarballs",
-        )
-        parser.add_argument(
-            "--no-wheel",
-            dest="wheel",
-            default=True,
-            action="store_false",
-            help="Don't build wheels",
-        )
-        parser.add_argument(
-            "-d", "--dest", default="dist", help="Target directory to put artifacts"
-        )
-        parser.add_argument(
-            "--no-clean",
-            dest="clean",
-            default=True,
-            action="store_false",
-            help="Do not clean the target directory",
-        )
-        parser.add_argument(
-            "--config-setting",
-            "-C",
-            action="append",
-            default=[],
-            help="Pass options to the backend. options with a value must be "
-            'specified after "=": "--config-setting=--opt(=value)" '
-            'or "-C--opt(=value)"',
-        )
-
-    def handle(self, project: Project, options: MinaCommandNamespace):
-        if not (project.root / "pyproject.toml").exists():
-            project.core.ui.echo("No pyproject.toml found.", err=True)
-            sys.exit(1)
-        pyproj = tomli.loads(
-            (project.root / "pyproject.toml").read_text(encoding="utf-8")
-        )
-        mina_packages = pyproj.get("tool", {}).get("mina", {}).get("packages", [])
-        packages = options.packages
-
-        if options.all:
-            if packages:
-                raise ProjectError("Cannot specify packages and --all")
-            packages = mina_packages
-
-        if not packages:
-            raise ProjectError("No package specified")
-
-        errors: list[str] = [
-            package for package in packages if package not in mina_packages
-        ]
-        if errors:
-            raise ProjectError(f"Package(s) not found: {', '.join(errors)}")
-
-        config_settings = {}
-        for item in options.config_setting:
-            name, _, value = item.partition("=")
-            if name not in config_settings:
-                config_settings[name] = value
-            else:
-                if not isinstance(config_settings[name], list):
-                    config_settings[name] = [config_settings[name]]
-                config_settings[name].append(value)
-        artifacts = do_build_mina(
-            project,
-            packages,
-            options.sdist,
-            options.wheel,
-            options.dest,
-            options.clean,
-            config_settings,
-        )
-        # artifacts 后面还可以拿来做其他的事情, 比如 publish.
+from __future__ import annotations
+
+import argparse
+import shutil
+import sys
+from pathlib import Path
+
+try:
+    import tomllib as tomli  # type: ignore
+except ImportError:
+    try:
+        from pdm.backend._vendor import tomli
+    except ImportError:
+        import tomli
+from pdm.builders.sdist import SdistBuilder
+from pdm.builders.wheel import WheelBuilder
+from pdm.cli.commands.base import BaseCommand
+from pdm.exceptions import ProjectError
+from pdm.project.core import Project
+
+
+def do_build_mina(
+    project: Project,
+    packages: list[str],
+    option_sdist: bool = True,
+    option_wheel: bool = True,
+    option_dest: str = "dist",
+    option_clean: bool = True,
+    config_settings: dict[str, str] | None = None,
+):
+    if project.is_global:
+        project.core.ui.echo("You can't build packages in global project.", err=True)
+        raise ProjectError("Global project not supported")
+    if not option_wheel and not option_sdist:
+        project.core.ui.echo("You must build at least one of sdist or wheel.", err=True)
+        raise ProjectError("No build type specified")
+    dest = Path(option_dest).absolute()
+    if option_clean:
+        shutil.rmtree(dest, ignore_errors=True)
+    artifacts: list[str] = []
+    for package in packages:
+        settings = (config_settings or {}).copy()
+        settings.setdefault("--mina-target", package)
+        project.core.ui.echo(f"Building package {package}...")
+        with project.core.ui.logging("Building packages"):
+            if option_sdist:
+                project.core.ui.echo("  - Building sdist")
+                loc = SdistBuilder(project.root, project.environment).build(
+                    option_dest, settings
+                )
+                project.core.ui.echo(f"    - completed: {loc}")
+                artifacts.append(loc)
+            if option_wheel:
+                project.core.ui.echo("  - Building wheel")
+                loc = WheelBuilder(project.root, project.environment).build(
+                    option_dest, settings
+                )
+                project.core.ui.echo(f"    - completed: {loc}")
+                artifacts.append(loc)
+            project.core.ui.echo(f"{package} build completed.")
+    project.core.ui.echo(
+        f"Successfully built {len(packages)} packages: {len(artifacts)} artifacts"
+    )
+    return artifacts
+
+
+class MinaCommandNamespace:
+    packages: list[str]
+    all: bool
+    sdist: bool
+    wheel: bool
+    dest: str
+    clean: bool
+    config_setting: list[str]
+
+
+class MinaBuildCommand(BaseCommand):
+    def add_arguments(self, parser: argparse.ArgumentParser) -> None:
+        parser.add_argument(
+            "packages",
+            nargs="*",
+            help="Packages to build, which must be defined in pyproject.toml.",
+        )
+        parser.add_argument(
+            "-a",
+            "--all",
+            default=False,
+            action="store_true",
+            help="Build all packages.",
+        )
+        parser.add_argument(
+            "--no-sdist",
+            dest="sdist",
+            default=True,
+            action="store_false",
+            help="Don't build source tarballs",
+        )
+        parser.add_argument(
+            "--no-wheel",
+            dest="wheel",
+            default=True,
+            action="store_false",
+            help="Don't build wheels",
+        )
+        parser.add_argument(
+            "-d", "--dest", default="dist", help="Target directory to put artifacts"
+        )
+        parser.add_argument(
+            "--no-clean",
+            dest="clean",
+            default=True,
+            action="store_false",
+            help="Do not clean the target directory",
+        )
+        parser.add_argument(
+            "--config-setting",
+            "-C",
+            action="append",
+            default=[],
+            help="Pass options to the backend. options with a value must be "
+            'specified after "=": "--config-setting=--opt(=value)" '
+            'or "-C--opt(=value)"',
+        )
+
+    def handle(self, project: Project, options: MinaCommandNamespace):
+        if not (project.root / "pyproject.toml").exists():
+            project.core.ui.echo("No pyproject.toml found.", err=True)
+            sys.exit(1)
+        pyproj = tomli.loads(
+            (project.root / "pyproject.toml").read_text(encoding="utf-8")
+        )
+        mina_packages = pyproj.get("tool", {}).get("mina", {}).get("packages", [])
+        packages = options.packages
+
+        if options.all:
+            if packages:
+                raise ProjectError("Cannot specify packages and --all")
+            packages = mina_packages
+
+        if not packages:
+            raise ProjectError("No package specified")
+
+        errors: list[str] = [
+            package for package in packages if package not in mina_packages
+        ]
+        if errors:
+            raise ProjectError(f"Package(s) not found: {', '.join(errors)}")
+
+        config_settings = {}
+        for item in options.config_setting:
+            name, _, value = item.partition("=")
+            if name not in config_settings:
+                config_settings[name] = value
+            else:
+                if not isinstance(config_settings[name], list):
+                    config_settings[name] = [config_settings[name]]
+                config_settings[name].append(value)
+        artifacts = do_build_mina(
+            project,
+            packages,
+            options.sdist,
+            options.wheel,
+            options.dest,
+            options.clean,
+            config_settings,
+        )
+        # artifacts 后面还可以拿来做其他的事情, 比如 publish.
```

### Comparing `pdm-mina-0.2.1/mina/plugin.py` & `pdm_mina-0.2.2/mina/plugin.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,28 +1,28 @@
-from argparse import ArgumentParser, Namespace
-from typing import TYPE_CHECKING
-
-from pdm.cli.commands.base import BaseCommand
-from pdm.project.core import Project
-
-from mina.commands.build import MinaBuildCommand
-from mina.commands.list import MinaPackagesListCommand
-
-if TYPE_CHECKING:
-    from pdm.core import Core
-
-
-class MinaCommand(BaseCommand):
-    """Mina command."""
-
-    def add_arguments(self, parser: ArgumentParser):
-        self.parser = parser
-        subparser = parser.add_subparsers()
-        MinaPackagesListCommand.register_to(subparser, "list")
-        MinaBuildCommand.register_to(subparser, "build")
-
-    def handle(self, project: Project, options: Namespace) -> None:
-        self.parser.print_help()
-
-
-def ensure_pdm(core: "Core"):
-    core.register_command(MinaCommand, "mina")
+from argparse import ArgumentParser, Namespace
+from typing import TYPE_CHECKING
+
+from pdm.cli.commands.base import BaseCommand
+from pdm.project.core import Project
+
+from mina.commands.build import MinaBuildCommand
+from mina.commands.list import MinaPackagesListCommand
+
+if TYPE_CHECKING:
+    from pdm.core import Core
+
+
+class MinaCommand(BaseCommand):
+    """Mina command."""
+
+    def add_arguments(self, parser: ArgumentParser):
+        self.parser = parser
+        subparser = parser.add_subparsers()
+        MinaPackagesListCommand.register_to(subparser, "list")
+        MinaBuildCommand.register_to(subparser, "build")
+
+    def handle(self, project: Project, options: Namespace) -> None:
+        self.parser.print_help()
+
+
+def ensure_pdm(core: "Core"):
+    core.register_command(MinaCommand, "mina")
```

### Comparing `pdm-mina-0.2.1/pyproject.toml` & `pdm_mina-0.2.2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [project]
 name = "pdm-mina"
-version = "0.2.1"
+version = "0.2.2"
 dependencies = [
-    "pdm>=2.0.0b1",
+    "pdm>=2.5.0",
     "mina-build>=0.2.1",
     "tomli>=1.1.0; python_version < \"3.11\"",
 ]
 requires-python = ">=3.9"
 readme = "README.md"
 
 [project.license]
@@ -18,34 +18,42 @@
 [tool.pdm.dev-dependencies]
 dev = [
     "black>=22.3.0",
     "isort>=5.10.1",
     "devtools>=0.8.0",
 ]
 
+[tool.pdm.build]
+includes = [
+    "mina",
+]
+excludes = [
+    "mina/backend",
+]
+
 [tool.mina]
 enabled = true
 override-global = false
 
 [tool.mina.packages.backend]
 override = false
 includes = [
     "mina/backend",
 ]
 raw-dependencies = []
 
 [tool.mina.packages.backend.project]
 name = "mina-build"
-version = "0.2.9"
+version = "0.4.0"
 description = "build backend for Mina Package Structure"
 authors = [
     { name = "GreyElaina", email = "GreyElaina@outlook.com" },
 ]
 dependencies = [
-    "pdm-pep517",
+    "pdm-backend",
     "tomli",
 ]
 requires-python = ">=3.9"
 readme = "README.build.md"
 
 [tool.mina.packages.backend.project.license]
 text = "MIT"
@@ -56,19 +64,19 @@
 ]
 excludes = [
     "mina/backend",
 ]
 
 [tool.mina.packages.cli-pdm.project]
 name = "pdm-mina"
-version = "0.2.1"
+version = "0.2.2"
 dependencies = [
-    "pdm",
-    "mina-build",
-    "tomli",
+    "pdm>=2.5.0",
+    "mina-build>=0.2.1",
+    "tomli>=1.1.0; python_version < \"3.11\"",
 ]
 requires-python = ">=3.9"
 readme = "README.md"
 
 [tool.mina.packages.cli-pdm.project.license]
 text = "MIT"
```

### Comparing `pdm-mina-0.2.1/README.md` & `pdm_mina-0.2.2/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,130 +1,140 @@
-# Mina Package Structure
-
-[简体中文](README.md) | [English](README.en.md)
-
-`Mina` 是基于 `pdm-pep517` 的 "模块分包" 实现.
-
-`Mina` 同样也是 `Mina Package Structure` 的实现, 作为一门独特的规范, 其具有以下特性:
-
- - 将整个项目作为工作区环境, 通过现有的设施统一管理所有分包使用的依赖树;
- - 分包各自声明自己的信息和工作区中引用的依赖;
- - 对 `pdm-pep517` 构建发布时所读取的 `Metadata` 进行修补以复用其构建流程;
- - 通过提供完整的 `PEP-517` 构建后端 (`build backend`), 避免了一些潜在的问题.
-
-`Mina` 提供了名为 [`mina-build`](https://pypi.org/project/mina-build/) 的 `PEP-517` 实现,
-同时还提供作为 `PDM Plugin` 的简易 CLI 实现;
-
-`mina-build` 仅在配置了需要构建的分包名称时才会注入 `pdm-pep517` 的构建流程,
-其他情况下的行为与 `pdm-pep517` 无异.
-
-CLI 中虽提供了一个 `pdm mina build <package>` 指令,
-但你也可以通过环境变量 `MINA_BUILD_TARGET` 或是 `config-setting` 中设置 `--mina-target` 指定需要打包的分包.
-
-## Quick Start
-
-### 安装 CLI
-
-目前, Mina 仅支持将 `pdm` 作为主要的用户功能入口, 但或许 `poetry` 会在之后得到支持?
-
-```bash
-elaina@localhost $ pip install pdm-mina
-# or pdm
-elaina@localhost $ pdm add pdm-mina -d
-```
-
-### 引入 mina-build
-
-在项目的 `pyproject.toml` 中配置以下项:
-
-```toml
-[build-system]
-requires = ["mina-build>=0.2.5"]
-build-backend = "mina.backend"
-```
-
-### 编辑 pyproject.toml
-
-假设你有如下的目录结构:
-
-```
-mina-example/
-├── avilla/
-│   ├── core/
-│   │   └── __init__.py
-│   ├── io/
-│   │   └── __init__.py
-│   ├── onebot/
-│   │   └── __init__.py
-│   └── elizabeth/
-│       └── __init__.py
-└── pyproject.toml
-```
-
-如果需要将 `avilla` 下的模块发为多个包, 用 `Mina` 可以简单的做到,
-比如上面这种我们就可以在 `pyproject.toml` 内填入以下几个表来声明分包:
-
-```toml
-[tool.mina.packages."core"]
-[tool.mina.packages."io"]
-[tool.mina.packages."onebot"]
-[tool.mina.packages."elizabeth"]
-```
-
-`Mina` 的分包声明沿用了 `PEP-621` 中的声明方式.
-我们这里以配置分包 `core` 举例.
-
-```toml
-[tool.mina.packages."core"]
-includes = [
-    "avilla/core"
-]
-# 相当于 tool.pdm.includes, 如果不填我不知道会发生什么, 可能就是普通的情况 -- 打包 name 所指向的模块.
-
-# raw-dependencies = [...]
-#    这一配置项会在处理完 project.dependencies 后直接排入依赖声明.
-#    你可以用这个特性来声明分包之间的依赖.
-
-# override = false
-
-[tool.mina.packages."core".project]
-name = "avilla-core"  # 分包在 `pypi` 上的名称, 必填
-description = "..."
-authors = ["..."]
-version = "0.1.0"  # 版本, 不保证支持动态获取(因为我没用过也没试过)
-requires-python = ">=3.9"
-dependencies = [  # 建议填入
-    "aiohttp",  # 这里虽然使用 `PEP-508` 规范, 但所有包都会被重定向至 project.dependencies 上的同名项.
-    "starlette",
-    "pydantic"
-]
-optional-dependencies = {
-    "amnesia": ["graia-amnesia"]  # optional dependencies 示例
-}
-entry-points = {pdm = {mina = "mina.plugin:ensure_pdm"}}  # entry-points 的声明方式
-```
-
-填入后, 你可以通过 CLI 的 `pdm mina list` 简单的检查, 或是直接 `pdm mina build <pkg>` 测试;
-
-### 构建发布包
-
-使用 `pdm mina build <pkg>` 可以构建对应的分包.
-
-如果你希望, 你可以使用 `pdm mina build -a/--all` 一次性构建所有的分包.
-
-这里推荐使用 `twine` + `keyring` 发布到 PyPI 上, 当然 `pdm-publish`, 或是用 Github Actions 也是可以的.
-
-## 覆盖工作区配置
-
-如果你希望, 你可以让 Mina 在处理和注入分包的 `project` 定义时, 使用覆盖工作区配置的形式来获得 Project Spec; 本特性默认不启用:
-
-```toml
-[tool.mina]
-override-global = true  # 全局启用该特性
-
-[tool.mina.packages."core"]
-override = true  # 仅在 core 分包启用该特性
-```
-
-# 开源协议
-
+Metadata-Version: 2.1
+Name: pdm-mina
+Version: 0.2.2
+License: MIT
+Requires-Python: >=3.9
+Requires-Dist: pdm>=2.5.0
+Requires-Dist: mina-build>=0.2.1
+Requires-Dist: tomli>=1.1.0; python_version < "3.11"
+Description-Content-Type: text/markdown
+
+# Mina Package Structure
+
+[简体中文](README.md) | [English](README.en.md)
+
+`Mina` 是基于 `pdm-backend` 的 "模块分包" 实现.
+
+`Mina` 同样也是 `Mina Package Structure` 的实现, 作为一门独特的规范, 其具有以下特性:
+
+ - 将整个项目作为工作区环境, 通过现有的设施统一管理所有分包使用的依赖树;
+ - 分包各自声明自己的信息和工作区中引用的依赖;
+ - 对 `pdm-backend` 构建发布时所读取的 `Metadata` 进行修补以复用其构建流程;
+ - 通过提供完整的 `PEP-517` 构建后端 (`build backend`), 避免了一些潜在的问题.
+
+`Mina` 提供了名为 [`mina-build`](https://pypi.org/project/mina-build/) 的 `PEP-517` 实现,
+同时还提供作为 `PDM Plugin` 的简易 CLI 实现;
+
+`mina-build` 仅在配置了需要构建的分包名称时才会注入 `pdm-pep517` 的构建流程,
+其他情况下的行为与 `pdm-backend` 无异.
+
+CLI 中虽提供了一个 `pdm mina build <package>` 指令,
+但你也可以通过环境变量 `MINA_BUILD_TARGET` 或是 `config-setting` 中设置 `--mina-target` 指定需要打包的分包.
+
+## Quick Start
+
+### 安装 CLI
+
+目前, Mina 仅支持将 `pdm` 作为主要的用户功能入口, 但或许 `poetry` 会在之后得到支持?
+
+```bash
+elaina@localhost $ pip install pdm-mina
+# or pdm
+elaina@localhost $ pdm add pdm-mina -d
+```
+
+### 引入 mina-build
+
+在项目的 `pyproject.toml` 中配置以下项:
+
+```toml
+[build-system]
+requires = ["mina-build>=0.2.5"]
+build-backend = "mina.backend"
+```
+
+### 编辑 pyproject.toml
+
+假设你有如下的目录结构:
+
+```
+mina-example/
+├── avilla/
+│   ├── core/
+│   │   └── __init__.py
+│   ├── io/
+│   │   └── __init__.py
+│   ├── onebot/
+│   │   └── __init__.py
+│   └── elizabeth/
+│       └── __init__.py
+└── pyproject.toml
+```
+
+如果需要将 `avilla` 下的模块发为多个包, 用 `Mina` 可以简单的做到,
+比如上面这种我们就可以在 `pyproject.toml` 内填入以下几个表来声明分包:
+
+```toml
+[tool.mina.packages."core"]
+[tool.mina.packages."io"]
+[tool.mina.packages."onebot"]
+[tool.mina.packages."elizabeth"]
+```
+
+`Mina` 的分包声明沿用了 `PEP-621` 中的声明方式.
+我们这里以配置分包 `core` 举例.
+
+```toml
+[tool.mina.packages."core"]
+includes = [
+    "avilla/core"
+]
+# 相当于 tool.pdm.includes, 如果不填我不知道会发生什么, 可能就是普通的情况 -- 打包 name 所指向的模块.
+
+# raw-dependencies = [...]
+#    这一配置项会在处理完 project.dependencies 后直接排入依赖声明.
+#    你可以用这个特性来声明分包之间的依赖.
+
+# override = false
+
+[tool.mina.packages."core".project]
+name = "avilla-core"  # 分包在 `pypi` 上的名称, 必填
+description = "..."
+authors = ["..."]
+version = "0.1.0"  # 版本, 不保证支持动态获取(因为我没用过也没试过)
+requires-python = ">=3.9"
+dependencies = [  # 建议填入
+    "aiohttp",  # 这里虽然使用 `PEP-508` 规范, 但所有包都会被重定向至 project.dependencies 上的同名项.
+    "starlette",
+    "pydantic"
+]
+optional-dependencies = {
+    "amnesia": ["graia-amnesia"]  # optional dependencies 示例
+}
+entry-points = {pdm = {mina = "mina.plugin:ensure_pdm"}}  # entry-points 的声明方式
+```
+
+填入后, 你可以通过 CLI 的 `pdm mina list` 简单的检查, 或是直接 `pdm mina build <pkg>` 测试;
+
+### 构建发布包
+
+使用 `pdm mina build <pkg>` 可以构建对应的分包.
+
+如果你希望, 你可以使用 `pdm mina build -a/--all` 一次性构建所有的分包.
+
+这里推荐使用 `twine` + `keyring` 发布到 PyPI 上, 当然 `pdm-publish`, 或是用 Github Actions 也是可以的.
+
+## 覆盖工作区配置
+
+如果你希望, 你可以让 Mina 在处理和注入分包的 `project` 定义时, 使用覆盖工作区配置的形式来获得 Project Spec; 本特性默认不启用:
+
+```toml
+[tool.mina]
+override-global = true  # 全局启用该特性
+
+[tool.mina.packages."core"]
+override = true  # 仅在 core 分包启用该特性
+```
+
+# 开源协议
+
 本项目使用 MIT 协议开源.
```

### Comparing `pdm-mina-0.2.1/PKG-INFO` & `pdm_mina-0.2.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,32 +1,25 @@
-Metadata-Version: 2.1
-Name: pdm-mina
-Version: 0.2.1
-License: MIT
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-
 # Mina Package Structure
 
 [简体中文](README.md) | [English](README.en.md)
 
-`Mina` 是基于 `pdm-pep517` 的 "模块分包" 实现.
+`Mina` 是基于 `pdm-backend` 的 "模块分包" 实现.
 
 `Mina` 同样也是 `Mina Package Structure` 的实现, 作为一门独特的规范, 其具有以下特性:
 
  - 将整个项目作为工作区环境, 通过现有的设施统一管理所有分包使用的依赖树;
  - 分包各自声明自己的信息和工作区中引用的依赖;
- - 对 `pdm-pep517` 构建发布时所读取的 `Metadata` 进行修补以复用其构建流程;
+ - 对 `pdm-backend` 构建发布时所读取的 `Metadata` 进行修补以复用其构建流程;
  - 通过提供完整的 `PEP-517` 构建后端 (`build backend`), 避免了一些潜在的问题.
 
 `Mina` 提供了名为 [`mina-build`](https://pypi.org/project/mina-build/) 的 `PEP-517` 实现,
 同时还提供作为 `PDM Plugin` 的简易 CLI 实现;
 
 `mina-build` 仅在配置了需要构建的分包名称时才会注入 `pdm-pep517` 的构建流程,
-其他情况下的行为与 `pdm-pep517` 无异.
+其他情况下的行为与 `pdm-backend` 无异.
 
 CLI 中虽提供了一个 `pdm mina build <package>` 指令,
 但你也可以通过环境变量 `MINA_BUILD_TARGET` 或是 `config-setting` 中设置 `--mina-target` 指定需要打包的分包.
 
 ## Quick Start
 
 ### 安装 CLI
@@ -130,8 +123,8 @@
 
 [tool.mina.packages."core"]
 override = true  # 仅在 core 分包启用该特性
 ```
 
 # 开源协议
 
-本项目使用 MIT 协议开源.
+本项目使用 MIT 协议开源.
```

