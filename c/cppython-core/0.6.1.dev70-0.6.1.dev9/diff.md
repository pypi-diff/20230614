# Comparing `tmp/cppython-core-0.6.1.dev70.tar.gz` & `tmp/cppython-core-0.6.1.dev9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cppython-core-0.6.1.dev70.tar", last modified: Wed Jun 14 21:15:45 2023, max compression
+gzip compressed data, was "cppython-core-0.6.1.dev9.tar", last modified: Sun Oct  9 15:14:07 2022, max compression
```

## Comparing `cppython-core-0.6.1.dev70.tar` & `cppython-core-0.6.1.dev9.tar`

### file list

```diff
@@ -1,20 +1,21 @@
--rw-r--r--   0        0        0     1070 2023-06-14 21:15:18.812352 cppython-core-0.6.1.dev70/LICENSE.md
--rw-r--r--   0        0        0       46 2023-06-14 21:15:18.812352 cppython-core-0.6.1.dev70/README.md
--rw-r--r--   0        0        0        3 2023-06-14 21:15:18.812352 cppython-core-0.6.1.dev70/cppython_core/__init__.py
--rw-r--r--   0        0        0     1522 2023-06-14 21:15:18.812352 cppython-core-0.6.1.dev70/cppython_core/exceptions.py
--rw-r--r--   0        0        0        3 2023-06-14 21:15:18.812352 cppython-core-0.6.1.dev70/cppython_core/plugin_schema/__init__.py
--rw-r--r--   0        0        0     2079 2023-06-14 21:15:18.812352 cppython-core-0.6.1.dev70/cppython_core/plugin_schema/generator.py
--rw-r--r--   0        0        0     2592 2023-06-14 21:15:18.812352 cppython-core-0.6.1.dev70/cppython_core/plugin_schema/provider.py
--rw-r--r--   0        0        0     1623 2023-06-14 21:15:18.812352 cppython-core-0.6.1.dev70/cppython_core/plugin_schema/scm.py
--rw-r--r--   0        0        0        0 2023-06-14 21:15:18.812352 cppython-core-0.6.1.dev70/cppython_core/py.typed
--rw-r--r--   0        0        0     7658 2023-06-14 21:15:18.812352 cppython-core-0.6.1.dev70/cppython_core/resolution.py
--rw-r--r--   0        0        0    10478 2023-06-14 21:15:18.812352 cppython-core-0.6.1.dev70/cppython_core/schema.py
--rw-r--r--   0        0        0     2762 2023-06-14 21:15:18.812352 cppython-core-0.6.1.dev70/cppython_core/utility.py
--rw-r--r--   0        0        0     2095 2023-06-14 21:15:18.812352 cppython-core-0.6.1.dev70/pyproject.toml
--rw-r--r--   0        0        0        3 2023-06-14 21:15:18.812352 cppython-core-0.6.1.dev70/tests/__init__.py
--rw-r--r--   0        0        0        3 2023-06-14 21:15:18.812352 cppython-core-0.6.1.dev70/tests/unit/__init__.py
--rw-r--r--   0        0        0     3171 2023-06-14 21:15:18.812352 cppython-core-0.6.1.dev70/tests/unit/test_plugin_schema.py
--rw-r--r--   0        0        0     1678 2023-06-14 21:15:18.812352 cppython-core-0.6.1.dev70/tests/unit/test_resolution.py
--rw-r--r--   0        0        0     1847 2023-06-14 21:15:18.812352 cppython-core-0.6.1.dev70/tests/unit/test_schema.py
--rw-r--r--   0        0        0     6128 2023-06-14 21:15:18.812352 cppython-core-0.6.1.dev70/tests/unit/test_utility.py
--rw-r--r--   0        0        0      433 1970-01-01 00:00:00.000000 cppython-core-0.6.1.dev70/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-10-09 15:13:58.861916 cppython-core-0.6.1.dev9/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (121)       46 2022-10-09 15:13:58.861916 cppython-core-0.6.1.dev9/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)        3 2022-10-09 15:13:58.861916 cppython-core-0.6.1.dev9/cppython_core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      785 2022-10-09 15:13:58.861916 cppython-core-0.6.1.dev9/cppython_core/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (121)        3 2022-10-09 15:13:58.861916 cppython-core-0.6.1.dev9/cppython_core/plugin_schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      831 2022-10-09 15:13:58.861916 cppython-core-0.6.1.dev9/cppython_core/plugin_schema/generator.py
+-rw-r--r--   0 runner    (1001) docker     (121)      650 2022-10-09 15:13:58.861916 cppython-core-0.6.1.dev9/cppython_core/plugin_schema/interface.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2009 2022-10-09 15:13:58.861916 cppython-core-0.6.1.dev9/cppython_core/plugin_schema/provider.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1099 2022-10-09 15:13:58.861916 cppython-core-0.6.1.dev9/cppython_core/plugin_schema/vcs.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-09 15:13:58.861916 cppython-core-0.6.1.dev9/cppython_core/py.typed
+-rw-r--r--   0 runner    (1001) docker     (121)     5301 2022-10-09 15:13:58.861916 cppython-core-0.6.1.dev9/cppython_core/resolution.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10761 2022-10-09 15:13:58.861916 cppython-core-0.6.1.dev9/cppython_core/schema.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2506 2022-10-09 15:13:58.861916 cppython-core-0.6.1.dev9/cppython_core/utility.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2254 2022-10-09 15:13:58.861916 cppython-core-0.6.1.dev9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)        3 2022-10-09 15:13:58.861916 cppython-core-0.6.1.dev9/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)        3 2022-10-09 15:13:58.861916 cppython-core-0.6.1.dev9/tests/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1750 2022-10-09 15:13:58.861916 cppython-core-0.6.1.dev9/tests/unit/test_plugin_schema.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3543 2022-10-09 15:13:58.861916 cppython-core-0.6.1.dev9/tests/unit/test_resolution.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3152 2022-10-09 15:13:58.861916 cppython-core-0.6.1.dev9/tests/unit/test_schema.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6346 2022-10-09 15:13:58.861916 cppython-core-0.6.1.dev9/tests/unit/test_utility.py
+-rw-------   0 runner    (1001) docker     (121)      432 2022-10-09 15:14:07.457900 cppython-core-0.6.1.dev9/PKG-INFO
```

### Comparing `cppython-core-0.6.1.dev70/LICENSE.md` & `cppython-core-0.6.1.dev9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `cppython-core-0.6.1.dev70/cppython_core/exceptions.py` & `cppython-core-0.6.1.dev9/cppython_core/exceptions.py`

 * *Files 20% similar despite different names*

```diff
@@ -16,50 +16,14 @@
 
         Returns:
             str -- The underlying error
         """
         return self._error
 
 
-class PluginError(Exception):
-    """Raised when there is a plugin error"""
-
-    def __init__(self, error: str) -> None:
-        self._error = error
-
-        super().__init__(error)
-
-    @property
-    def error(self) -> str:
-        """Returns the underlying error
-
-        Returns:
-            str -- The underlying error
-        """
-        return self._error
-
-
-class NotSupportedError(Exception):
-    """Raised when something is not supported"""
-
-    def __init__(self, error: str) -> None:
-        self._error = error
-
-        super().__init__(error)
-
-    @property
-    def error(self) -> str:
-        """Returns the underlying error
-
-        Returns:
-            str -- The underlying error
-        """
-        return self._error
-
-
 class ProcessError(Exception):
     """Raised when there is a configuration error"""
 
     def __init__(self, error: str) -> None:
         self._error = error
 
         super().__init__(error)
```

### Comparing `cppython-core-0.6.1.dev70/cppython_core/plugin_schema/provider.py` & `cppython-core-0.6.1.dev9/cppython_core/plugin_schema/provider.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,89 +1,75 @@
 """Provider data plugin definitions"""
+from __future__ import annotations
+
 from abc import abstractmethod
-from typing import Any, Protocol, TypeVar, runtime_checkable
+from pathlib import Path
+from typing import TypeVar
 
+from pydantic import Field
 from pydantic.types import DirectoryPath
 
-from cppython_core.plugin_schema.generator import SyncConsumer
-from cppython_core.schema import (
-    CorePluginData,
-    DataPlugin,
-    DataPluginGroupData,
-    SupportedDataFeatures,
-    SyncData,
-)
+from cppython_core.schema import DataPlugin, PluginGroupData
 
 
-class ProviderPluginGroupData(DataPluginGroupData):
+class ProviderData(PluginGroupData):
     """Base class for the configuration data that is set by the project for the provider"""
 
-
-class SupportedProviderFeatures(SupportedDataFeatures):
-    """Provider plugin feature support"""
+    root_directory: DirectoryPath = Field(description="The directory where the pyproject.toml lives")
 
 
-class SyncProducer(Protocol):
-    """Interface for producing synchronization data with generators"""
+class Provider(DataPlugin[ProviderData]):
+    """Abstract type to be inherited by CPPython Provider plugins"""
 
     @staticmethod
-    @abstractmethod
-    def supported_sync_type(sync_type: type[SyncData]) -> bool:
-        """Queries for support for a given synchronization type
-
-        Args:
-            sync_type: The type to query support for
+    def group() -> str:
+        """The plugin group name as used by 'setuptools'
 
         Returns:
-            Support
+            The group name
         """
-        raise NotImplementedError
 
+        return "provider"
+
+    @classmethod
     @abstractmethod
-    def sync_data(self, consumer: SyncConsumer) -> SyncData | None:
-        """Requests generator information from the provider. The generator is either defined by a provider specific file
-        or the CPPython configuration table
+    def tooling_downloaded(cls, path: Path) -> bool:
+        """Returns whether the provider tooling needs to be downloaded
 
         Args:
-            consumer: The consumer
+            path: The directory to check for downloaded tooling
+
+        Raises:
+            NotImplementedError: Must be sub-classed
 
         Returns:
-            An instantiated data type, or None if no instantiation is made
+            Whether the tooling has been downloaded or not
         """
-        raise NotImplementedError
 
+        raise NotImplementedError()
 
-@runtime_checkable
-class Provider(DataPlugin, SyncProducer, Protocol):
-    """Abstract type to be inherited by CPPython Provider plugins"""
-
+    @classmethod
     @abstractmethod
-    def __init__(
-        self, group_data: ProviderPluginGroupData, core_data: CorePluginData, configuration_data: dict[str, Any]
-    ) -> None:
-        raise NotImplementedError
-
-    @staticmethod
-    @abstractmethod
-    def features(directory: DirectoryPath) -> SupportedProviderFeatures:
-        """Broadcasts the shared features of the Provider plugin to CPPython
+    async def download_tooling(cls, path: Path) -> None:
+        """Installs the external tooling required by the provider
 
         Args:
-            directory: The root directory where features are evaluated
+            path: The directory to download any extra tooling to
 
-        Returns:
-            The supported features
+        Raises:
+            NotImplementedError: Must be sub-classed
         """
-        raise NotImplementedError
+
+        raise NotImplementedError()
 
     @abstractmethod
     def install(self) -> None:
         """Called when dependencies need to be installed from a lock file."""
-        raise NotImplementedError
+        raise NotImplementedError()
 
     @abstractmethod
     def update(self) -> None:
         """Called when dependencies need to be updated and written to the lock file."""
-        raise NotImplementedError
+        raise NotImplementedError()
 
 
 ProviderT = TypeVar("ProviderT", bound=Provider)
```

### Comparing `cppython-core-0.6.1.dev70/cppython_core/plugin_schema/scm.py` & `cppython-core-0.6.1.dev9/cppython_core/plugin_schema/vcs.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,61 +1,48 @@
 """Version control data plugin definitions"""
-from abc import abstractmethod
-from typing import Protocol, TypeVar, runtime_checkable
-
-from pydantic import DirectoryPath, Field
-
-from cppython_core.schema import Plugin, PluginGroupData, SupportedFeatures
-
-
-class SCMPluginGroupData(PluginGroupData):
-    """SCM plugin input data"""
-
+from __future__ import annotations
 
-class SupportedSCMFeatures(SupportedFeatures):
-    """SCM plugin feature support"""
+from abc import abstractmethod
+from pathlib import Path
+from typing import TypeVar
 
-    repository: bool = Field(description="True if the directory is a repository for the SCM. False, otherwise")
+from cppython_core.schema import Plugin
 
 
-@runtime_checkable
-class SCM(Plugin, Protocol):
+class VersionControl(Plugin):
     """Base class for version control systems"""
 
     @abstractmethod
-    def __init__(self, group_data: SCMPluginGroupData) -> None:
-        raise NotImplementedError
-
-    @staticmethod
-    @abstractmethod
-    def features(directory: DirectoryPath) -> SupportedSCMFeatures:
-        """Broadcasts the shared features of the SCM plugin to CPPython
+    def is_repository(self, path: Path) -> bool:
+        """Queries repository status of a path
 
         Args:
-            directory: The root directory where features are evaluated
+            path: The input path to query
 
         Returns:
-            The supported features
+            Whether the given path is a repository root
         """
-        raise NotImplementedError
+        raise NotImplementedError()
 
     @abstractmethod
-    def version(self, directory: DirectoryPath) -> str:
+    def extract_version(self, path: Path) -> str:
         """Extracts the system's version metadata
 
         Args:
-            directory: The input directory
+            path: The repository path
 
         Returns:
-            A version string
+            A version
         """
-        raise NotImplementedError
+        raise NotImplementedError()
 
-    def description(self) -> str | None:
-        """Requests extraction of the project description
+    @staticmethod
+    def group() -> str:
+        """The plugin group name as used by 'setuptools'summary
 
         Returns:
-            Returns the project description, or none if unavailable
+            The group name
         """
+        return "vcs"
 
 
-SCMT = TypeVar("SCMT", bound=SCM)
+VersionControlT = TypeVar("VersionControlT", bound=VersionControl)
```

### Comparing `cppython-core-0.6.1.dev70/cppython_core/schema.py` & `cppython-core-0.6.1.dev9/cppython_core/schema.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,63 +1,76 @@
 """Data types for CPPython that encapsulate the requirements between the plugins and the core library
 """
 
-from abc import abstractmethod
+from __future__ import annotations
+
+from abc import ABC, abstractmethod
+from collections.abc import Callable
+from dataclasses import dataclass
+from logging import Logger, getLogger
 from pathlib import Path
-from typing import Any, NewType, Protocol, TypeVar
+from typing import Any
+from typing import Generator as TypingGenerator
+from typing import Generic, NewType, TypeVar
 
-from pydantic import BaseModel, Field, field_validator, model_validator
+from packaging.requirements import InvalidRequirement, Requirement
+from pydantic import BaseModel, Extra, Field, validator
 from pydantic.types import DirectoryPath, FilePath
 
 
 class CPPythonModel(BaseModel):
     """The base model to use for all CPPython models"""
 
-    model_config = {"populate_by_name": False}
+    @dataclass
+    class Config:
+        """Pydantic built-in configuration"""
+
+        # Data aliases should only exist for Configuration types. Constructors will never take aliases by field name
+        allow_population_by_field_name = False
+
+        # Mutation will happen via data resolution
+        allow_mutation = False
 
 
 ModelT = TypeVar("ModelT", bound=CPPythonModel)
 
 
-class ProjectData(CPPythonModel, extra="forbid"):
+class ProjectData(CPPythonModel, extra=Extra.forbid):
     """Resolved data of 'ProjectConfiguration'"""
 
     pyproject_file: FilePath = Field(description="The path where the pyproject.toml exists")
     verbosity: int = Field(default=0, description="The verbosity level as an integer [0,2]")
 
 
-class ProjectConfiguration(CPPythonModel, extra="forbid"):
+class ProjectConfiguration(CPPythonModel, extra=Extra.forbid):
     """Project-wide configuration"""
 
     pyproject_file: FilePath = Field(description="The path where the pyproject.toml exists")
     version: str | None = Field(
         description=(
             "The version number a 'dynamic' project version will resolve to. If not provided a CPPython project will"
-            " initialize its SCM plugins to discover any available version"
+            " initialize its VCS plugins to discover any available version"
         )
     )
     verbosity: int = Field(default=0, description="The verbosity level as an integer [0,2]")
-    debug: bool = Field(
-        default=False, description="Debug mode. Additional processing will happen to expose more debug information"
-    )
 
-    @field_validator("verbosity")
+    @validator("verbosity")
     @classmethod
     def min_max(cls, value: int) -> int:
         """Validator that clamps the input value
 
         Args:
             value: Input to validate
 
         Returns:
             The clamped input value
         """
         return min(max(value, 0), 2)
 
-    @field_validator("pyproject_file")
+    @validator("pyproject_file")
     @classmethod
     def pyproject_name(cls, value: FilePath) -> FilePath:
         """Validator that verifies the name of the file
 
         Args:
             value: Input to validate
 
@@ -89,58 +102,107 @@
     """
 
     dynamic: list[str] = Field(default=[], description="https://peps.python.org/pep-0621/#dynamic")
     name: str = Field(description="https://peps.python.org/pep-0621/#name")
     version: str | None = Field(default=None, description="https://peps.python.org/pep-0621/#version")
     description: str = Field(default="", description="https://peps.python.org/pep-0621/#description")
 
-    @model_validator(mode="after")  # type: ignore
+    @validator("version", always=True)
     @classmethod
-    def dynamic_data(cls, model: "PEP621Configuration") -> "PEP621Configuration":
-        """Validates that dynamic data is represented correctly
+    def dynamic_version(cls, value: str | None, values: dict[str, Any]) -> str | None:
+        """Validates that version is present or that the name is present in the dynamic field
 
         Args:
-            model: The input model data
+            value: The input version
+            values: All values of the Model prior to running this validation
 
         Raises:
             ValueError: If dynamic versioning is incorrect
 
         Returns:
-            The data
+            The validated input version
         """
 
-        for field in model.model_fields.keys():
-            if field == "dynamic":
-                continue
-            value = getattr(model, field)
-            if field not in model.dynamic:
-                if value is None:
-                    raise ValueError(f"'{field}' is not a dynamic field. It must be defined")
-            else:
-                if value is not None:
-                    raise ValueError(f"'{field}' is a dynamic field. It must not be defined")
+        if "version" not in values["dynamic"]:
+            if value is None:
+                raise ValueError("'version' is not a dynamic field. It must be defined")
+        else:
+            if value is not None:
+                raise ValueError("'version' is a dynamic field. It must not be defined")
 
-        return model
+        return value
 
 
 def _default_install_location() -> Path:
     return Path.home() / ".cppython"
 
 
-class CPPythonData(CPPythonModel, extra="forbid"):
+class PEP508(Requirement):
+    """PEP 508 conforming string"""
+
+    @classmethod
+    def __get_validators__(cls) -> TypingGenerator[Callable[..., Any], None, None]:
+        """Yields the set of validators defined for this type so pydantic can use them internally
+
+        Yields:
+            A new validator Callable
+        """
+        yield cls.validate_requirement
+        yield cls.validate_cppython
+
+    @classmethod
+    def validate_requirement(cls, value: "PEP508") -> PEP508:
+        """Enforce type that this class can be cast to a Requirement
+        TODO - Use the Self type python 3.11
+
+        Args:
+            value: The input value to validate
+
+        Raises:
+            TypeError: Raised if the input value is not the right type
+            ValueError: Raised if a PEP508 requirement can't be parsed
+
+        Returns:
+            The validated input value
+        """
+        if not isinstance(value, str):
+            raise TypeError("string required")
+
+        try:
+            Requirement(value)
+        except InvalidRequirement as invalid:
+            raise ValueError from invalid
+
+        return value
+
+    @classmethod
+    def validate_cppython(cls, value: "PEP508") -> PEP508:
+        """TODO: Use for something
+        TODO - Use the Self type python 3.11
+
+        Args:
+            value: The input value to validate
+
+        Returns:
+            The validated input value
+        """
+
+        return value
+
+
+class CPPythonData(CPPythonModel, extra=Extra.forbid):
     """Resolved CPPython data with local and global configuration"""
 
+    dependencies: list[PEP508]
     install_path: DirectoryPath
     tool_path: DirectoryPath
     build_path: DirectoryPath
     current_check: bool
-    provider_name: str
-    generator_name: str
 
-    @field_validator("install_path", "tool_path", "build_path")
+    @validator("install_path", "tool_path", "build_path")
     @classmethod
     def validate_absolute_path(cls, value: DirectoryPath) -> DirectoryPath:
         """Enforce the input is an absolute path
 
         Args:
             value: The input value
 
@@ -154,195 +216,147 @@
             raise ValueError("Absolute path required")
 
         return value
 
 
 CPPythonPluginData = NewType("CPPythonPluginData", CPPythonData)
 
-PluginName = NewType("PluginName", str)
-PluginGroup = NewType("PluginGroup", str)
-PluginFullName = NewType("PluginFullName", str)
-
-
-class SyncData(CPPythonModel):
-    """Data that passes in a plugin sync"""
-
-    provider_name: PluginName
 
+class CPPythonGlobalConfiguration(CPPythonModel, extra=Extra.forbid):
+    """Global data extracted by the tool"""
 
-SyncDataT = TypeVar("SyncDataT", bound=SyncData)
+    current_check: bool = Field(default=True, alias="current-check", description="Checks for a new CPPython version")
 
 
-class SupportedFeatures(CPPythonModel):
-    """Plugin feature support"""
+class CPPythonLocalConfiguration(CPPythonModel, extra=Extra.forbid):
+    """Data required by the tool"""
 
-    initialization: bool = Field(
-        default=False, description="Whether the plugin supports initialization from an empty state"
+    dependencies: list[PEP508] = Field(default=[], description="List of PEP508 dependencies")
+    install_path: Path = Field(
+        default=_default_install_location(), alias="install-path", description="The global install path for the project"
+    )
+    tool_path: Path = Field(
+        default=Path("tool"), alias="tool-path", description="The local tooling path for the project"
+    )
+    build_path: Path = Field(
+        default=Path("build"), alias="build-path", description="The local build path for the project"
+    )
+    provider: dict[str, dict[str, Any]] = Field(
+        default={}, description="Optional list of dynamically generated 'provider' plugin data"
+    )
+    generator: dict[str, dict[str, Any]] = Field(
+        default={}, description="Optional list of dynamically generated 'generator' plugin data"
+    )
+    vcs: dict[str, dict[str, Any]] = Field(
+        default={}, description="Optional list of dynamically generated 'vcs' plugin data"
     )
 
-
-class Information(CPPythonModel):
-    """Plugin information that complements the packaged project metadata"""
-
-
-class PluginGroupData(CPPythonModel, extra="forbid"):
-    """Plugin group data"""
-
-    root_directory: DirectoryPath = Field(description="The directory of the project")
-
-
-class Plugin(Protocol):
-    """CPPython plugin"""
-
-    @abstractmethod
-    def __init__(self, group_data: PluginGroupData) -> None:
-        raise NotImplementedError
-
-    @staticmethod
-    @abstractmethod
-    def features(directory: DirectoryPath) -> SupportedFeatures:
-        """Broadcasts the shared features of the plugin to CPPython
+    def extract_plugin_data(self, plugin_type: type[DataPluginT]) -> dict[str, Any]:
+        """Extracts a plugin data type from the CPPython table
 
         Args:
-            directory: The root directory where features are evaluated
-
-        Returns:
-            The supported features
-        """
-        raise NotImplementedError
+            plugin_type: The plugin type
 
-    @staticmethod
-    @abstractmethod
-    def information() -> Information:
-        """Retrieves plugin information that complements the packaged project metadata
+        Raises:
+            KeyError: If there is no plugin data with the given name
 
         Returns:
-            The plugin's information
+            The plugin data
         """
-        raise NotImplementedError
 
+        attribute = getattr(self, plugin_type.group())
+        data: dict[str, Any] = attribute[plugin_type.name()]
 
-PluginT = TypeVar("PluginT", bound=Plugin)
+        return data
 
 
-class DataPluginGroupData(PluginGroupData):
-    """Data plugin group data"""
+class ToolData(CPPythonModel):
+    """Tool entry of pyproject.toml"""
 
+    cppython: CPPythonLocalConfiguration | None = Field(default=None)
 
-class CorePluginData(CPPythonModel):
-    """Core resolved data that will be passed to data plugins"""
 
-    project_data: ProjectData
-    pep621_data: PEP621Data
-    cppython_data: CPPythonPluginData
+class PyProject(CPPythonModel):
+    """pyproject.toml schema"""
 
+    project: PEP621Configuration
+    tool: ToolData | None = Field(default=None)
 
-class SupportedDataFeatures(SupportedFeatures):
-    """Data plugin feature support"""
 
+class Plugin(ABC):
+    """Abstract plugin type"""
 
-class DataPlugin(Plugin, Protocol):
-    """Abstract plugin type for internal CPPython data"""
+    _logger: Logger
 
+    @staticmethod
     @abstractmethod
-    def __init__(
-        self, group_data: DataPluginGroupData, core_data: CorePluginData, configuration_data: dict[str, Any]
-    ) -> None:
-        raise NotImplementedError
+    def name() -> str:
+        """The name of the plugin"""
+        raise NotImplementedError()
 
     @staticmethod
     @abstractmethod
-    def features(directory: DirectoryPath) -> SupportedDataFeatures:
-        """Broadcasts the shared features of the data plugin to CPPython
-
-        Args:
-            directory: The root directory where features are evaluated
-
-        Returns:
-            The supported features
-        """
-        raise NotImplementedError
+    def group() -> str:
+        """The plugin group name"""
+        raise NotImplementedError()
 
     @classmethod
-    async def download_tooling(cls, directory: DirectoryPath) -> None:
-        """Installs the external tooling required by the plugin. Should be overridden if required
+    def logger(cls) -> Logger:
+        """Returns the plugin specific sub-logger
 
-        Args:
-            directory: The directory to download any extra tooling to
+        Returns:
+            The plugin's named logger
         """
 
+        if not hasattr(cls, "_logger"):
+            cls._logger = getLogger(f"cppython.{cls.group()}.{cls.name()}")
 
-DataPluginT = TypeVar("DataPluginT", bound=DataPlugin)
+        return cls._logger
 
 
-class CPPythonGlobalConfiguration(CPPythonModel, extra="forbid"):
-    """Global data extracted by the tool"""
-
-    current_check: bool = Field(default=True, alias="current-check", description="Checks for a new CPPython version")
-
-
-ProviderData = NewType("ProviderData", dict[str, Any])
-GeneratorData = NewType("GeneratorData", dict[str, Any])
-
-
-class CPPythonLocalConfiguration(CPPythonModel, extra="forbid"):
-    """Data required by the tool"""
-
-    install_path: Path = Field(
-        default=_default_install_location(), alias="install-path", description="The global install path for the project"
-    )
-    tool_path: Path = Field(
-        default=Path("tool"), alias="tool-path", description="The local tooling path for the project"
-    )
-    build_path: Path = Field(
-        default=Path("build"), alias="build-path", description="The local build path for the project"
-    )
-    provider: ProviderData = Field(
-        default=ProviderData({}), description="Provider plugin data associated with 'provider_name"
-    )
-    provider_name: str | None = Field(
-        default=None, alias="provider-name", description="If empty, the provider will be automatically deduced."
-    )
-    generator: GeneratorData = Field(
-        default=GeneratorData({}), description="Generator plugin data associated with 'generator_name'"
-    )
-    generator_name: str | None = Field(
-        default=None, alias="generator-name", description="If empty, the generator will be automatically deduced."
-    )
-
-
-class ToolData(CPPythonModel):
-    """Tool entry of pyproject.toml"""
-
-    cppython: CPPythonLocalConfiguration = Field(description="CPPython tool data")
-
-
-class PyProject(CPPythonModel):
-    """pyproject.toml schema"""
-
-    project: PEP621Configuration = Field(description="PEP621: https://www.python.org/dev/peps/pep-0621/")
-    tool: ToolData = Field(description="Tool data")
+PluginT = TypeVar("PluginT", bound=Plugin)
 
 
-class CoreData(CPPythonModel):
-    """Core resolved data that will be resolved"""
+class PluginGroupData(CPPythonModel, ABC, extra=Extra.forbid):
+    """_summary_"""
 
-    project_data: ProjectData
-    pep621_data: PEP621Data
-    cppython_data: CPPythonData
 
+PluginGroupDataT = TypeVar("PluginGroupDataT", bound=PluginGroupData)
 
-class Interface(Protocol):
-    """Type for interfaces to allow feedback from CPPython"""
 
-    @abstractmethod
-    def write_pyproject(self) -> None:
-        """Called when CPPython requires the interface to write out pyproject.toml changes"""
-        raise NotImplementedError
+class DataPlugin(Plugin, Generic[PluginGroupDataT]):
+    """Abstract plugin type for internal CPPython data"""
 
-    @abstractmethod
-    def write_configuration(self) -> None:
-        """Called when CPPython requires the interface to write out configuration changes"""
-        raise NotImplementedError
+    def __init__(
+        self,
+        group_data: PluginGroupDataT,
+        project: PEP621Data,
+        cppython: CPPythonData,
+        generator_data: dict[str, Any],
+    ) -> None:
+        self._group_data = group_data
+        self._project = project
+        self._cppython = cppython
+        self._generator_data = generator_data
+
+    @property
+    def group_data(self) -> PluginGroupDataT:
+        """Returns the PluginGroupData object set at initialization"""
+        return self._group_data
+
+    @property
+    def project(self) -> PEP621Data:
+        """Returns the PEP621Data object set at initialization"""
+        return self._project
+
+    @property
+    def cppython(self) -> CPPythonData:
+        """Returns the CPPythonDataData object set at initialization"""
+        return self._cppython
+
+    @property
+    def generator_data(self) -> dict[str, Any]:
+        """Returns the data set at initialization"""
+        return self._generator_data
 
 
-InterfaceT = TypeVar("InterfaceT", bound=Interface)
+DataPluginT = TypeVar("DataPluginT", bound=DataPlugin[Any])
```

### Comparing `cppython-core-0.6.1.dev70/cppython_core/utility.py` & `cppython-core-0.6.1.dev9/cppython_core/utility.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 """Core Utilities
 """
 
 import json
 import logging
-import re
 import subprocess
 from logging import Logger
 from pathlib import Path
-from typing import Any, NamedTuple
+from typing import Any
 
 from pydantic import BaseModel
 
 from cppython_core.exceptions import ProcessError
+from cppython_core.schema import ModelT
 
 
 def subprocess_call(
     arguments: list[str | Path], logger: Logger, log_level: int = logging.WARNING, suppress: bool = False, **kwargs: Any
 ) -> None:
     """Executes a subprocess call with logger and utility attachments. Captures STDOUT and STDERR
 
@@ -39,14 +39,28 @@
                 if not suppress:
                     logger.log(log_level, line.rstrip())
 
     if process.returncode != 0:
         raise ProcessError("Subprocess task failed")
 
 
+def read_model_json(path: Path, model: type[ModelT]) -> ModelT:
+    """Reading routine. Only keeps Model data
+
+    Args:
+        path: The file to read
+        model: The model to read
+
+    Returns:
+        The read model
+    """
+
+    return model.parse_file(path=path)
+
+
 def read_json(path: Path) -> Any:
     """Reading routine
 
     Args:
         path: The json file to read
 
     Returns:
@@ -76,33 +90,7 @@
     Args:
         path: The json to write
         data: The data to write into json
     """
 
     with open(path, "w", encoding="utf-8") as file:
         json.dump(data, file, ensure_ascii=False, indent=4)
-
-
-_canonicalize_regex = re.compile(r"((?<=[a-z])[A-Z]|(?<!\A)[A-Z](?=[a-z]))")
-
-
-class NormalizedName(NamedTuple):
-    """Normalized name"""
-
-    name: str
-    group: str
-
-
-def canonicalize_name(name: str) -> NormalizedName:
-    """Performs normalization on an input string
-
-    Args:
-        name: The string to parse
-
-    Returns:
-        The normalized name
-    """
-
-    sub = re.sub(_canonicalize_regex, r" \1", name)
-    values = sub.split(" ")
-    result = "".join(values[:-1])
-    return NormalizedName(result.lower(), values[-1].lower())
```

### Comparing `cppython-core-0.6.1.dev70/pyproject.toml` & `cppython-core-0.6.1.dev9/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,46 +1,49 @@
 [project]
 description = "Data definitions for CPPython"
 name = "cppython-core"
-license = "MIT"
+license-expression = "MIT"
 authors = [
     { name = "Synodic Software", email = "contact@synodic.software" },
 ]
 readme = "README.md"
 dynamic = []
-requires-python = ">=3.11"
+requires-python = ">=3.10"
 dependencies = [
-    "pydantic>=2.0b1",
+    "pydantic>=1.10.1",
+    "packaging>=21.3",
 ]
-version = "0.6.1.dev70"
+version = "0.6.1.dev9"
 
 [project.license-files]
 paths = [
     "LICENSE.md",
 ]
 
 [project.urls]
 homepage = "https://github.com/Synodic-Software/CPPython-Core"
 repository = "https://github.com/Synodic-Software/CPPython-Core"
 
+[project.optional-dependencies]
+
 [tool.pdm.version]
 use_scm = true
 
 [tool.pdm.dev-dependencies]
 lint = [
-    "black>=23.1.0",
+    "black>=22.6.0",
     "isort>=5.10.1",
-    "mypy>=1.0.0",
-    "pylint>=2.16.1",
+    "mypy>=0.971",
+    "pylint>=2.15.2",
 ]
 test = [
     "pytest>=7.1.2",
-    "pytest-cov>=4.0.0",
+    "pytest-cov>=3.0.0",
+    "pytest-mock>=3.8.2",
     "tomlkit>=0.11.4",
-    "pytest-mock>=3.10.0",
 ]
 
 [tool.pdm.scripts.analyze]
 shell = "pylint --verbose cppython_core tests"
 
 [tool.pdm.scripts.format]
 shell = "black --check --verbose ."
@@ -77,26 +80,30 @@
 skip_gitignore = true
 
 [tool.mypy]
 exclude = "__pypackages__"
 plugins = [
     "pydantic.mypy",
 ]
+show_error_codes = true
 strict = true
 
 [tool.pylint.MAIN]
 load-plugins = [
     "pylint.extensions.code_style",
     "pylint.extensions.typing",
     "pylint.extensions.docstyle",
     "pylint.extensions.docparams",
     "pylint.extensions.private_import",
     "pylint.extensions.bad_builtin",
 ]
 
+[tool.pylint.messages_control]
+extension-pkg-whitelist = "pydantic"
+
 [tool.pylint.format]
 max-line-length = "120"
 
 [tool.pylint.parameter_documentation]
 accept-no-param-doc = false
 accept-no-raise-doc = false
 accept-no-return-doc = false
```

### Comparing `cppython-core-0.6.1.dev70/tests/unit/test_schema.py` & `cppython-core-0.6.1.dev9/tests/unit/test_schema.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,57 +1,104 @@
-"""Test custom schema validation that cannot be verified by the Pydantic validation"""
+"""Test custom schema validation that cannot be verified by the Pydantic validation
+"""
 
 import pytest
 from pydantic import Field
 from tomlkit import parse
 
 from cppython_core.schema import (
+    PEP508,
     CPPythonGlobalConfiguration,
     CPPythonLocalConfiguration,
     CPPythonModel,
     PEP621Configuration,
+    PyProject,
 )
 
 
 class TestSchema:
     """Test validation"""
 
-    class Model(CPPythonModel):
+    class TestModel(CPPythonModel):
         """Testing Model"""
 
         aliased_variable: bool = Field(default=False, alias="aliased-variable", description="Alias test")
 
     def test_model_construction(self) -> None:
         """Verifies that the base model type has the expected construction behaviors"""
 
-        model = self.Model(**{"aliased_variable": True})
+        model = self.TestModel(aliased_variable=True)
         assert model.aliased_variable is False
 
-        model = self.Model(**{"aliased-variable": True})
+        model = self.TestModel(**{"aliased-variable": True})
         assert model.aliased_variable is True
 
     def test_model_construction_from_data(self) -> None:
         """Verifies that the base model type has the expected construction behaviors"""
 
         data = """
         aliased_variable = false\n
         aliased-variable = true
         """
 
-        result = self.Model.model_validate(parse(data).value)
+        result = self.TestModel.parse_obj(parse(data).value)
         assert result.aliased_variable is True
 
     def test_cppython_local(self) -> None:
         """Ensures that the CPPython local config data can be defaulted"""
         CPPythonLocalConfiguration()
 
     def test_cppython_global(self) -> None:
         """Ensures that the CPPython global config data can be defaulted"""
         CPPythonGlobalConfiguration()
 
+    def test_cppython_table(self) -> None:
+        """Ensures that the nesting yaml table behavior can be read properly"""
+
+        data = """
+        [project]\n
+        name = "test"\n
+        version = "1.0.0"\n
+        description = "A test document"\n
+
+        [tool.cppython]\n
+        """
+
+        document = parse(data).value
+        pyproject = PyProject(**document)
+        assert pyproject.tool is not None
+        assert pyproject.tool.cppython is not None
+
+    def test_empty_cppython(self) -> None:
+        """Ensure that the common none condition works"""
+
+        data = """
+        [project]\n
+        name = "test"\n
+        version = "1.0.0"\n
+        description = "A test document"\n
+
+        [tool.test]\n
+        """
+
+        document = parse(data).value
+        pyproject = PyProject(**document)
+        assert pyproject.tool is not None
+        assert pyproject.tool.cppython is None
+
+    def test_508(self) -> None:
+        """Ensure correct parsing of the 'packaging' type via the PEP508 intermediate type"""
+
+        requirement = PEP508('requests [security,tests] >= 2.8.1, == 2.8.* ; python_version < "2.7"')
+
+        assert requirement.name == "requests"
+
+        with pytest.raises(ValueError):
+            PEP508("this is not conforming")
+
     def test_pep621_version(self) -> None:
         """Tests the dynamic version validation"""
 
         with pytest.raises(ValueError):
             PEP621Configuration(name="empty-test")
 
         with pytest.raises(ValueError):
```

### Comparing `cppython-core-0.6.1.dev70/tests/unit/test_utility.py` & `cppython-core-0.6.1.dev9/tests/unit/test_utility.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,72 +6,79 @@
 from pathlib import Path
 from sys import executable
 
 import pytest
 from pytest import LogCaptureFixture
 
 from cppython_core.exceptions import ProcessError
-from cppython_core.schema import CPPythonModel
-from cppython_core.utility import canonicalize_name, subprocess_call
+from cppython_core.schema import CPPythonModel, Plugin
+from cppython_core.utility import read_model_json, subprocess_call, write_model_json
 
 cppython_logger = logging.getLogger("cppython")
 cppython_logger.addHandler(StreamHandler())
 
 
 class TestUtility:
     """Tests the utility functionality"""
 
     class ModelTest(CPPythonModel):
         """Model definition to help test IO utilities"""
 
         test_path: Path
         test_int: int
 
-    def test_none(self) -> None:
-        """Verifies that no exception is thrown with an empty string"""
+    def test_plugin_log(self, caplog: LogCaptureFixture) -> None:
+        """Ensures that the root logger receives the auto-gathered plugin logger
 
-        test = canonicalize_name("")
+        Args:
+            caplog: Fixture for capturing logging input
+        """
 
-        assert test.group == ""
-        assert test.name == ""
+        class MockPlugin(Plugin):
+            """A dummy plugin to verify logging metadata"""
 
-    def test_only_group(self) -> None:
-        """Verifies that no exception is thrown when only a group is specified"""
+            @staticmethod
+            def name() -> str:
+                """Static name to compare in this test
 
-        test = canonicalize_name("Group")
+                Returns:
+                    Name of the plugin
+                """
+                return "mock"
 
-        assert test.group == "group"
-        assert test.name == ""
+            @staticmethod
+            def group() -> str:
+                """Static group to compare in this test
 
-    def test_name_group(self) -> None:
-        """Test that canonicalization works"""
+                Returns:
+                    Name of the group
+                """
+                return "group"
 
-        test = canonicalize_name("NameGroup")
+        logger = MockPlugin.logger()
 
-        assert test.group == "group"
-        assert test.name == "name"
+        with caplog.at_level(logging.INFO):
+            logger.info("test")
+            assert caplog.record_tuples == [("cppython.group.mock", logging.INFO, "test")]
 
-    def test_group_only_caps(self) -> None:
-        """Test that canonicalization works"""
-        test = canonicalize_name("NameGROUP")
+    def test_model_read_write(self, tmp_path: Path) -> None:
+        """Tests a full IO write -> read for data maintenance
 
-        assert test.group == "group"
-        assert test.name == "name"
+        Args:
+            tmp_path: Temporary path for writing
+        """
 
-    def test_name_only_caps(self) -> None:
-        """Test that canonicalization works"""
-        test = canonicalize_name("NAMEGroup")
-        assert test.group == "group"
-        assert test.name == "name"
+        test_model = TestUtility.ModelTest(test_path=Path(), test_int=3)
 
-    def test_name_multi_caps(self) -> None:
-        """Test that caps works"""
-        test = canonicalize_name("NAmeGroup")
-        assert test.group == "group"
-        assert test.name == "name"
+        json_path = tmp_path / "test.json"
+
+        write_model_json(json_path, test_model)
+        output = read_model_json(json_path, TestUtility.ModelTest)
+
+        assert test_model == output
 
 
 class TestSubprocess:
     """Subprocess testing"""
 
     def test_subprocess_stdout(self, caplog: LogCaptureFixture) -> None:
         """Test subprocess_call
```

