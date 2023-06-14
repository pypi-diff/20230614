# Comparing `tmp/mina-build-0.2.9.tar.gz` & `tmp/mina-build-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mina-build-0.2.9.tar", last modified: Sun Dec 25 09:41:26 2022, max compression
+gzip compressed data, was "mina-build-0.4.0.tar", last modified: Wed Jun 14 12:10:04 2023, max compression
```

## Comparing `mina-build-0.2.9.tar` & `mina-build-0.4.0.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-rw-rw-   0        0        0     9731 2022-12-25 09:40:06.944904 mina-build-0.2.9/mina/backend/__init__.py
--rw-rw-rw-   0        0        0     1497 2022-12-25 09:41:13.215550 mina-build-0.2.9/pyproject.toml
--rw-rw-rw-   0        0        0      386 2022-12-25 09:34:05.031591 mina-build-0.2.9/README.build.md
--rw-rw-rw-   0        0        0      611 2022-12-25 09:41:26.412939 mina-build-0.2.9/PKG-INFO
+-rw-r--r--   0        0        0      381 2023-06-14 12:09:44.821847 mina-build-0.4.0/README.build.md
+-rw-r--r--   0        0        0    11045 2023-06-14 12:09:44.821847 mina-build-0.4.0/mina/backend/__init__.py
+-rw-r--r--   0        0        0     1499 2023-06-14 12:09:44.821847 mina-build-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0      613 1970-01-01 00:00:00.000000 mina-build-0.4.0/PKG-INFO
```

### Comparing `mina-build-0.2.9/mina/backend/__init__.py` & `mina-build-0.4.0/mina/backend/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,261 +1,304 @@
-from __future__ import annotations
-
-import functools
-import os
-from pathlib import Path
-from typing import Any, Dict, Mapping, Optional
-
-try:
-    import tomllib as tomli  # type: ignore
-except ImportError:
-    try:
-        from pdm.pep517._vendor import tomli
-    except ImportError:
-        import tomli
-
-from pdm.pep517._vendor.packaging.requirements import Requirement
-from pdm.pep517.api import _prepare_metadata
-from pdm.pep517.api import \
-    get_requires_for_build_sdist as get_requires_for_build_sdist
-from pdm.pep517.api import \
-    get_requires_for_build_wheel as get_requires_for_build_wheel
-from pdm.pep517.api import \
-    prepare_metadata_for_build_wheel as prepare_metadata_for_build_wheel
-from pdm.pep517.base import Builder
-from pdm.pep517.editable import EditableBuilder
-from pdm.pep517.metadata import Config, Metadata
-from pdm.pep517.sdist import SdistBuilder
-from pdm.pep517.wheel import WheelBuilder
-
-
-@functools.lru_cache(None)
-def _get_config_root():
-    cwd = Path.cwd()
-    return tomli.loads((cwd / "pyproject.toml").read_text(encoding="utf-8"))
-
-
-@functools.lru_cache(None)
-def _get_root_project():
-    return _get_config_root().get("project", {})
-
-
-@functools.lru_cache(None)
-def _get_tool_mina() -> dict[str, Any]:
-    return _get_config_root().get("tool", {}).get("mina", {})
-
-
-@functools.lru_cache(None)
-def _get_package(package: str) -> Dict[str, Any]:
-    return _get_tool_mina().get("packages", {}).get(package, {})
-
-
-def _has_package(package: str) -> bool:
-    return _get_package(package) is not None
-
-
-def _get_build_target(
-    config_settings: Optional[Mapping[str, Any]] = None
-) -> str | None:
-    return (
-        (config_settings or {}).get("--mina-target")
-        or os.environ.get("MINA_BUILD_TARGET")
-        or _get_tool_mina().get("mina-build-target")
-    )
-
-
-def _using_override_global() -> bool:
-    return _get_tool_mina().get("override-global", False)
-
-
-def _using_override(package: str | None) -> bool:
-    if package and _has_package(package):
-        pkg = _get_package(package)
-        if "override" in pkg:
-            return pkg["override"]
-    return _using_override_global()
-
-
-def _patch_dep(_meta: Metadata, pkg_project: dict[str, Any]):
-    if "dependencies" in pkg_project:
-        optional_dependencies = []
-
-        optional_deps = pkg_project["dependencies"]
-        workspace_deps = _get_root_project().get("dependencies", [])
-        workspace_deps = [Requirement(i) for i in workspace_deps]
-        workspace_deps = {i.name: i for i in workspace_deps if i.name is not None}
-
-        for dep in optional_deps:
-            req = Requirement(dep)
-            if req.name is None:
-                raise ValueError(f"'{dep}' is not a valid requirement")
-            if req.name not in workspace_deps:
-                raise ValueError(f"{req.name} is not defined in project requirements")
-            optional_dependencies.append(str(workspace_deps[req.name]))
-
-        pkg_project["dependencies"] = _meta._convert_dependencies(optional_dependencies)
-
-    if "optional-dependencies" in pkg_project:
-        optional_dependencies = {}
-
-        deps = pkg_project["optional-dependencies"]
-
-        # workspace don't use optional dep: it must contains ALL deps mina required.
-        workspace_deps = _get_root_project().get("dependencies", [])
-        workspace_deps = [Requirement(i) for i in workspace_deps]
-        workspace_deps = {i.name: i for i in workspace_deps if i.name is not None}
-
-        for group, optional_deps in deps.items():
-            group_deps = []
-            for dep in optional_deps:
-                req = Requirement(dep)
-                if req.name is None:
-                    raise ValueError(f"'{dep}' is not a valid requirement")
-                if req.name not in workspace_deps:
-                    raise ValueError(
-                        f"{req.name} is not defined in project requirements"
-                    )
-                group_deps.append(str(workspace_deps[req.name]))
-            optional_dependencies[group] = group_deps
-
-        pkg_project["optional-dependencies"] = _meta._convert_optional_dependencies(
-            optional_dependencies
-        )
-
-
-def _patch_pdm_metadata(package: str):
-    cwd = Path.cwd()
-    _meta = Builder(cwd).meta
-
-    config = tomli.loads((cwd / "pyproject.toml").read_text(encoding="utf-8"))
-
-    package_conf = (
-        config.get("tool", {}).get("mina", {}).get("packages", {}).get(package, None)
-    )
-    if package_conf is None:
-        raise ValueError(f"No package named '{package}'")
-    package_project = package_conf.get("project", {})
-
-    _patch_dep(_meta, package_project)
-
-    pdm_settings = config.get("tool", {}).get("pdm", {})
-
-    # dev-dependencies is unnecessary for a pkg(for workspace), so it will be ignored by mina.
-
-    if "includes" in package_conf:
-        pdm_settings["includes"] = package_conf["includes"]
-
-    if "excludes" in package_conf:
-        pdm_settings["excludes"] = package_conf["excludes"]
-
-    if "source-includes" in package_conf:
-        pdm_settings["source-includes"] = package_conf["source-includes"]
-
-    if "is-purelib" in package_conf:
-        pdm_settings["is-purelib"] = package_conf["is-purelib"]
-
-    if "entry-points" in package_conf:
-        pdm_settings["entry-points"] = package_conf["entry-points"]
-
-    if "build" in package_conf:
-        pdm_settings["build"] = package_conf["build"]
-
-    if "raw-dependencies" in package_conf and _meta.dependencies is not None:
-        _meta.dependencies.extend(package_conf["raw-dependencies"])
-
-    if _using_override(package):
-        project_conf = config.get("project", {})
-        _meta.data = dict(project_conf, **package_project)
-    else:
-        _meta.data = package_project
-
-    _meta.config = Config(_meta.root, pdm_settings)
-    _meta.validate(True)
-
-    return _meta
-
-
-def prepare_metadata_for_build_wheel(
-    metadata_directory: str, config_settings: Optional[Mapping[str, Any]] = None
-) -> str:
-    """Prepare the metadata, places it in metadata_directory"""
-    _patched_meta = None
-    mina_target = _get_build_target(config_settings)
-    if mina_target is not None:
-        if not _has_package(mina_target):
-            raise ValueError(f"{mina_target} is not defined as a mina package")
-        _patched_meta = _patch_pdm_metadata(mina_target)  # os.chdir may break behavior
-    with WheelBuilder(Path.cwd(), config_settings) as builder:
-        if _patched_meta is not None:
-            builder._meta = _patched_meta
-        return _prepare_metadata(builder, metadata_directory)
-
-
-def build_wheel(
-    wheel_directory: str,
-    config_settings: Optional[Mapping[str, Any]] = None,
-    metadata_directory: Optional[str] = None,
-) -> str:
-    """Builds a wheel, places it in wheel_directory"""
-    _patched_meta = None
-    mina_target = _get_build_target(config_settings)
-    if mina_target is not None:
-        if not _has_package(mina_target):
-            raise ValueError(f"{mina_target} is not defined as a mina package")
-        _patched_meta = _patch_pdm_metadata(mina_target)  # os.chdir may break behavior
-    with WheelBuilder(Path.cwd(), config_settings) as builder:
-        if _patched_meta is not None:
-            builder._meta = _patched_meta
-        return Path(builder.build(wheel_directory)).name
-
-
-def build_sdist(
-    sdist_directory: str, config_settings: Optional[Mapping[str, Any]] = None
-) -> str:
-    """Builds an sdist, places it in sdist_directory"""
-    _patched_meta = None
-    mina_target = _get_build_target(config_settings)
-    if mina_target is not None:
-        if not _has_package(mina_target):
-            raise ValueError(f"{mina_target} is not defined as a mina package")
-        _patched_meta = _patch_pdm_metadata(mina_target)  # os.chdir may break behavior
-    with SdistBuilder(Path.cwd(), config_settings) as builder:
-        if _patched_meta is not None:
-            builder._meta = _patched_meta
-        return Path(builder.build(sdist_directory)).name
-
-
-get_requires_for_build_editable = get_requires_for_build_wheel
-
-
-def prepare_metadata_for_build_editable(
-    metadata_directory: str, config_settings: Optional[Mapping[str, Any]] = None
-) -> str:
-    """Prepare the metadata, places it in metadata_directory"""
-    _patched_meta = None
-    mina_target = _get_build_target(config_settings)
-    if mina_target is not None:
-        if not _has_package(mina_target):
-            raise ValueError(f"{mina_target} is not defined as a mina package")
-        _patched_meta = _patch_pdm_metadata(mina_target)  # os.chdir may break behavior
-    with EditableBuilder(Path.cwd(), config_settings) as builder:
-        if _patched_meta is not None:
-            builder._meta = _patched_meta
-        builder._prepare_editable()
-        return _prepare_metadata(builder, metadata_directory)
-
-
-def build_editable(
-    wheel_directory: str,
-    config_settings: Optional[Mapping[str, Any]] = None,
-    metadata_directory: Optional[str] = None,
-) -> str:
-    _patched_meta = None
-    mina_target = _get_build_target(config_settings)
-    if mina_target is not None:
-        if not _has_package(mina_target):
-            raise ValueError(f"{mina_target} is not defined as a mina package")
-        _patched_meta = _patch_pdm_metadata(mina_target)  # os.chdir may break behavior
-    with EditableBuilder(Path.cwd(), config_settings) as builder:
-        if _patched_meta is not None:
-            builder._meta = _patched_meta
-        return Path(builder.build(wheel_directory)).name
+from __future__ import annotations
+
+import functools
+import os
+from pathlib import Path
+from typing import Any, Dict, Mapping, Optional
+
+try:
+    import tomllib as tomli  # type: ignore
+except ImportError:
+    try:
+        from pdm.backend._vendor import tomli
+    except ImportError:
+        import tomli
+
+from pdm.backend._vendor.packaging.requirements import Requirement
+from pdm.backend import \
+    get_requires_for_build_sdist as get_requires_for_build_sdist
+from pdm.backend import \
+    get_requires_for_build_wheel as get_requires_for_build_wheel
+from pdm.backend import \
+    prepare_metadata_for_build_wheel as prepare_metadata_for_build_wheel
+from pdm.backend.base import Builder
+from pdm.backend.config import Metadata, BuildConfig
+
+
+@functools.lru_cache(None)
+def _get_config_root():
+    cwd = Path.cwd()
+    return tomli.loads((cwd / "pyproject.toml").read_text(encoding="utf-8"))
+
+
+@functools.lru_cache(None)
+def _get_root_project():
+    return _get_config_root().get("project", {})
+
+
+@functools.lru_cache(None)
+def _get_tool_mina() -> dict[str, Any]:
+    return _get_config_root().get("tool", {}).get("mina", {})
+
+
+@functools.lru_cache(None)
+def _get_package(package: str) -> Dict[str, Any]:
+    return _get_tool_mina().get("packages", {}).get(package, {})
+
+
+def _has_package(package: str) -> bool:
+    return _get_package(package) is not None
+
+
+def _get_build_target(
+    config_settings: Optional[Mapping[str, Any]] = None
+) -> str | None:
+    return (
+        (config_settings or {}).get("--mina-target")
+        or os.environ.get("MINA_BUILD_TARGET")
+        or _get_tool_mina().get("mina-build-target")
+    )
+
+
+def _using_override_global() -> bool:
+    return _get_tool_mina().get("override-global", False)
+
+
+def _using_override(package: str | None) -> bool:
+    if package and _has_package(package):
+        pkg = _get_package(package)
+        if "override" in pkg:
+            return pkg["override"]
+    return _using_override_global()
+
+
+def _patch_dep(pkg_project: dict[str, Any]):
+    if "dependencies" in pkg_project:
+        optional_dependencies: list[str] = []
+
+        optional_deps: list[str] = pkg_project["dependencies"]
+        workspace_deps_origin: list[str] = _get_root_project().get("dependencies", [])
+        workspace_deps_convert = [Requirement(i) for i in workspace_deps_origin]
+        workspace_deps_map = {
+            i.name: i for i in workspace_deps_convert if i.name is not None
+        }
+
+        for dep in optional_deps:
+            req = Requirement(dep)
+            if req.name is None:
+                raise ValueError(f"'{dep}' is not a valid requirement")
+            if req.name not in workspace_deps_map:
+                raise ValueError(f"{req.name} is not defined in project requirements")
+            optional_dependencies.append(str(workspace_deps_map[req.name]))
+
+        pkg_project["dependencies"] = optional_dependencies
+
+    if "optional-dependencies" in pkg_project:
+        optional_dependencies: dict[str, list[str]] = {}
+
+        deps: dict[str, list[str]] = pkg_project["optional-dependencies"]
+
+        # workspace don't use optional dep: it must contains ALL deps mina required.
+        workspace_deps_origin: list[str] = _get_root_project().get("dependencies", [])
+        workspace_deps_convert = [Requirement(i) for i in workspace_deps_origin]
+        workspace_deps_map = {
+            i.name: i for i in workspace_deps_convert if i.name is not None
+        }
+
+        for group, optional_deps in deps.items():
+            group_deps = []
+            for dep in optional_deps:
+                req = Requirement(dep)
+                if req.name is None:
+                    raise ValueError(f"'{dep}' is not a valid requirement")
+                if req.name not in workspace_deps_map:
+                    raise ValueError(
+                        f"{req.name} is not defined in project requirements"
+                    )
+                group_deps.append(str(workspace_deps_map[req.name]))
+            optional_dependencies[group] = group_deps
+
+        pkg_project["optional-dependencies"] = optional_dependencies
+
+
+def _patch_pdm_config(package: str):
+    cwd = Path.cwd()
+    config = Builder(cwd).config
+
+    package_conf = (
+        config.data.get("tool", {})
+        .get("mina", {})
+        .get("packages", {})
+        .get(package, None)
+    )
+    if package_conf is None:
+        raise ValueError(f"No package named '{package}'")
+    package_project = package_conf.get("project", {})
+
+    _patch_dep(package_project)
+
+    pdm_settings = config.data.get("tool", {}).get("pdm", {}).get("build", {})
+
+    # dev-dependencies is unnecessary for a pkg(for workspace), so it will be ignored by mina.
+
+    if "custom-hook" in package_conf:
+        pdm_settings["custom-hook"] = package_conf["custom-hook"]
+
+    if "includes" in package_conf:
+        pdm_settings["includes"] = package_conf["includes"]
+
+    if "excludes" in package_conf:
+        pdm_settings["excludes"] = package_conf["excludes"]
+
+    if "source-includes" in package_conf:
+        pdm_settings["source-includes"] = package_conf["source-includes"]
+
+    if "is-purelib" in package_conf:
+        pdm_settings["is-purelib"] = package_conf["is-purelib"]
+
+    if "run-setuptools" in package_conf:
+        pdm_settings["run-setuptools"] = package_conf["run-setuptools"]
+
+    if "package-dir" in package_conf:
+        pdm_settings["package-dir"] = package_conf["package-dir"]
+
+    if "editable-backend" in package_conf:
+        pdm_settings["editable-backend"] = package_conf["editable-backend"]
+
+    if "wheel-data" in package_conf:
+        pdm_settings["wheel-data"] = package_conf["wheel-data"]
+
+    if "entry-points" in package_conf:
+        if "entry-points" not in package_project:
+            package_project["entry-points"] = {}
+        for group, entry_points in package_conf["entry-points"].items():
+            if group not in package_project["entry-points"]:
+                package_project["entry-points"][group] = {}
+            package_project["entry-points"][group].update(entry_points)
+
+    if "scripts" in package_conf:
+        package_project.setdefault("entry-points", {})[
+            "console_scripts"
+        ] = package_conf["scripts"]
+    if "gui-scripts" in package_conf:
+        package_project.setdefault("entry-points", {})["gui_scripts"] = package_conf[
+            "gui-scripts"
+        ]
+
+    if (
+        "raw-dependencies" in package_conf
+        and config.metadata.get("dependencies") is not None
+    ):
+        config.data["project"]["dependencies"].extend(package_conf["raw-dependencies"])
+
+    if _using_override(package):
+        project_conf = config.data["project"]
+        config.data["project"] = dict(project_conf, **package_project)
+    else:
+        config.data["project"] = package_project
+
+    config.data["tool"].setdefault("pdm", {})["build"] = pdm_settings
+    config.validate(config.data, config.root)
+    config.metadata = Metadata(config.data["project"])
+    config.build_config = BuildConfig(config.root, pdm_settings)
+    return config
+
+
+def prepare_metadata_for_build_wheel(
+    metadata_directory: str, config_settings: Optional[Mapping[str, Any]] = None
+) -> str:
+    """Prepare the metadata, places it in metadata_directory"""
+    from pdm.backend.wheel import WheelBuilder
+
+    _patched_config = None
+    mina_target = _get_build_target(config_settings)
+    if mina_target is not None:
+        if not _has_package(mina_target):
+            raise ValueError(f"{mina_target} is not defined as a mina package")
+        _patched_config = _patch_pdm_config(mina_target)  # os.chdir may break behavior
+    with WheelBuilder(Path.cwd(), config_settings) as builder:
+        if _patched_config is not None:
+            builder.config = _patched_config
+        return builder.prepare_metadata(metadata_directory).name
+
+
+def build_wheel(
+    wheel_directory: str,
+    config_settings: Optional[Mapping[str, Any]] = None,
+    metadata_directory: Optional[str] = None,
+) -> str:
+    """Builds a wheel, places it in wheel_directory"""
+    from pdm.backend.wheel import WheelBuilder
+
+    _patched_config = None
+    mina_target = _get_build_target(config_settings)
+    if mina_target is not None:
+        if not _has_package(mina_target):
+            raise ValueError(f"{mina_target} is not defined as a mina package")
+        _patched_config = _patch_pdm_config(mina_target)  # os.chdir may break behavior
+
+    with WheelBuilder(Path.cwd(), config_settings) as builder:
+        if _patched_config is not None:
+            builder.config = _patched_config
+        return builder.build(
+            wheel_directory, metadata_directory=metadata_directory
+        ).name
+
+
+def build_sdist(
+    sdist_directory: str, config_settings: Optional[Mapping[str, Any]] = None
+) -> str:
+    """Builds an sdist, places it in sdist_directory"""
+    from pdm.backend.sdist import SdistBuilder
+
+    _patched_config = None
+    mina_target = _get_build_target(config_settings)
+    if mina_target is not None:
+        if not _has_package(mina_target):
+            raise ValueError(f"{mina_target} is not defined as a mina package")
+        _patched_config = _patch_pdm_config(mina_target)  # os.chdir may break behavior
+    with SdistBuilder(Path.cwd(), config_settings) as builder:
+        if _patched_config is not None:
+            builder.config = _patched_config
+        return builder.build(sdist_directory).name
+
+
+get_requires_for_build_editable = get_requires_for_build_wheel
+
+
+def prepare_metadata_for_build_editable(
+    metadata_directory: str, config_settings: Optional[Mapping[str, Any]] = None
+) -> str:
+    """Prepare the metadata, places it in metadata_directory"""
+    from pdm.backend.editable import EditableBuilder
+
+    _patched_config = None
+    mina_target = _get_build_target(config_settings)
+    if mina_target is not None:
+        if not _has_package(mina_target):
+            raise ValueError(f"{mina_target} is not defined as a mina package")
+        _patched_config = _patch_pdm_config(mina_target)  # os.chdir may break behavior
+    with EditableBuilder(Path.cwd(), config_settings) as builder:
+        if _patched_config is not None:
+            builder.config = _patched_config
+        return builder.prepare_metadata(metadata_directory).name
+
+
+def build_editable(
+    wheel_directory: str,
+    config_settings: Optional[Mapping[str, Any]] = None,
+    metadata_directory: Optional[str] = None,
+) -> str:
+    from pdm.backend.editable import EditableBuilder
+
+    _patched_config = None
+    mina_target = _get_build_target(config_settings)
+    if mina_target is not None:
+        if not _has_package(mina_target):
+            raise ValueError(f"{mina_target} is not defined as a mina package")
+        _patched_config = _patch_pdm_config(mina_target)  # os.chdir may break behavior
+    with EditableBuilder(Path.cwd(), config_settings) as builder:
+        if _patched_config is not None:
+            builder.config = _patched_config
+        return builder.build(
+            wheel_directory, metadata_directory=metadata_directory
+        ).name
```

### Comparing `mina-build-0.2.9/pyproject.toml` & `mina-build-0.4.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [project]
 name = "mina-build"
-version = "0.2.9"
+version = "0.4.0"
 description = "build backend for Mina Package Structure"
 authors = [
     { name = "GreyElaina", email = "GreyElaina@outlook.com" },
 ]
 dependencies = [
-    "pdm-pep517>=1.0.1",
+    "pdm-backend>=2.1.0",
     "tomli>=1.1.0; python_version < \"3.11\"",
 ]
 requires-python = ">=3.9"
 readme = "README.build.md"
 
 [project.license]
 text = "MIT"
@@ -31,21 +31,21 @@
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
@@ -56,15 +56,15 @@
 ]
 excludes = [
     "mina/backend",
 ]
 
 [tool.mina.packages.cli-pdm.project]
 name = "pdm-mina"
-version = "0.2.1"
+version = "0.2.2"
 dependencies = [
     "pdm",
     "mina-build",
     "tomli",
 ]
 requires-python = ">=3.9"
 readme = "README.md"
```

### Comparing `mina-build-0.2.9/PKG-INFO` & `mina-build-0.4.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: mina-build
-Version: 0.2.9
+Version: 0.4.0
 Summary: build backend for Mina Package Structure
 License: MIT
 Author-email: GreyElaina <GreyElaina@outlook.com>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 
 # PEP-517 implementation for Mina Package Structure
 
-`mina-build` 是 `Mina Package Structure` 的具体实现, 基于 `pdm-pep517` 的现有建构.
+`mina-build` 是 `Mina Package Structure` 的具体实现, 基于 `pdm-backend` 的现有建构.
 
 你需要在 `pyproject.toml` 内将 `tool.mina.enabled` 设为 `true` 才能使用 Mina 的相关功能,
-否则 `mina-build` 的行为与 `pdm-pep517` 一致.
+否则 `mina-build` 的行为与 `pdm-backend` 一致.
 
 若是需要关于 `Mina` 的更多信息, 请参阅其他的文稿.
```

