# Comparing `tmp/fileformats-0.6.2.tar.gz` & `tmp/fileformats-0.6.3.tar.gz`

## Comparing `fileformats-0.6.2.tar` & `fileformats-0.6.3.tar`

### file list

```diff
@@ -1,45 +1,47 @@
--rw-r--r--   0        0        0     1342 2020-02-02 00:00:00.000000 fileformats-0.6.2/fileformats/archive/__init__.py
--rw-r--r--   0        0        0     8869 2020-02-02 00:00:00.000000 fileformats-0.6.2/fileformats/archive/converters.py
--rw-r--r--   0        0        0     2515 2020-02-02 00:00:00.000000 fileformats-0.6.2/fileformats/archive/tests/test_archive_converters.py
--rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 fileformats-0.6.2/fileformats/audio/__init__.py
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 fileformats-0.6.2/fileformats/core/__init__.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 fileformats-0.6.2/fileformats/core/_version.py
--rw-r--r--   0        0        0    41153 2020-02-02 00:00:00.000000 fileformats-0.6.2/fileformats/core/base.py
--rw-r--r--   0        0        0     5584 2020-02-02 00:00:00.000000 fileformats-0.6.2/fileformats/core/converter.py
--rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 fileformats-0.6.2/fileformats/core/exceptions.py
--rw-r--r--   0        0        0     4609 2020-02-02 00:00:00.000000 fileformats-0.6.2/fileformats/core/mark.py
--rw-r--r--   0        0        0    24541 2020-02-02 00:00:00.000000 fileformats-0.6.2/fileformats/core/mixin.py
--rw-r--r--   0        0        0    10881 2020-02-02 00:00:00.000000 fileformats-0.6.2/fileformats/core/utils.py
--rw-r--r--   0        0        0     8171 2020-02-02 00:00:00.000000 fileformats-0.6.2/fileformats/core/tests/test_classifiers.py
--rw-r--r--   0        0        0     3990 2020-02-02 00:00:00.000000 fileformats-0.6.2/fileformats/core/tests/test_converter.py
--rw-r--r--   0        0        0     5998 2020-02-02 00:00:00.000000 fileformats-0.6.2/fileformats/core/tests/test_detection.py
--rw-r--r--   0        0        0     3336 2020-02-02 00:00:00.000000 fileformats-0.6.2/fileformats/core/tests/test_general.py
--rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 fileformats-0.6.2/fileformats/core/tests/test_mime.py
--rw-r--r--   0        0        0     7043 2020-02-02 00:00:00.000000 fileformats-0.6.2/fileformats/core/tests/test_mixin.py
--rw-r--r--   0        0        0     5884 2020-02-02 00:00:00.000000 fileformats-0.6.2/fileformats/core/tests/test_utils.py
--rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 fileformats-0.6.2/fileformats/document/__init__.py
--rw-r--r--   0        0        0     4843 2020-02-02 00:00:00.000000 fileformats-0.6.2/fileformats/field/__init__.py
--rw-r--r--   0        0        0     2205 2020-02-02 00:00:00.000000 fileformats-0.6.2/fileformats/field/tests/test_fields.py
--rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 fileformats-0.6.2/fileformats/field/tests/test_fields_mime.py
--rw-r--r--   0        0        0     7937 2020-02-02 00:00:00.000000 fileformats-0.6.2/fileformats/generic/__init__.py
--rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 fileformats-0.6.2/fileformats/image/__init__.py
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 fileformats-0.6.2/fileformats/image/base.py
--rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 fileformats-0.6.2/fileformats/image/converters.py
--rw-r--r--   0        0        0     1893 2020-02-02 00:00:00.000000 fileformats-0.6.2/fileformats/image/raster.py
--rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 fileformats-0.6.2/fileformats/image/vector.py
--rw-r--r--   0        0        0      536 2020-02-02 00:00:00.000000 fileformats-0.6.2/fileformats/image/tests/test_image_converters.py
--rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 fileformats-0.6.2/fileformats/image/tests/test_image_raster.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 fileformats-0.6.2/fileformats/misc/__init__.py
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 fileformats-0.6.2/fileformats/misc/medical.py
--rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 fileformats-0.6.2/fileformats/numeric/__init__.py
--rw-r--r--   0        0        0     2159 2020-02-02 00:00:00.000000 fileformats-0.6.2/fileformats/serialization/__init__.py
--rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 fileformats-0.6.2/fileformats/serialization/converters.py
--rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 fileformats-0.6.2/fileformats/serialization/tests/test_serialization_converters.py
--rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 fileformats-0.6.2/fileformats/text/__init__.py
--rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 fileformats-0.6.2/fileformats/video/__init__.py
--rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 fileformats-0.6.2/.gitignore
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 fileformats-0.6.2/AUTHORS
--rw-r--r--   0        0        0    14222 2020-02-02 00:00:00.000000 fileformats-0.6.2/LICENSE
--rw-r--r--   0        0        0     5235 2020-02-02 00:00:00.000000 fileformats-0.6.2/README.rst
--rw-r--r--   0        0        0     2458 2020-02-02 00:00:00.000000 fileformats-0.6.2/pyproject.toml
--rw-r--r--   0        0        0    22512 2020-02-02 00:00:00.000000 fileformats-0.6.2/PKG-INFO
+-rw-r--r--   0        0        0     1342 2020-02-02 00:00:00.000000 fileformats-0.6.3/fileformats/archive/__init__.py
+-rw-r--r--   0        0        0     8869 2020-02-02 00:00:00.000000 fileformats-0.6.3/fileformats/archive/converters.py
+-rw-r--r--   0        0        0     2515 2020-02-02 00:00:00.000000 fileformats-0.6.3/fileformats/archive/tests/test_archive_converters.py
+-rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 fileformats-0.6.3/fileformats/audio/__init__.py
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 fileformats-0.6.3/fileformats/core/__init__.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 fileformats-0.6.3/fileformats/core/_version.py
+-rw-r--r--   0        0        0     5584 2020-02-02 00:00:00.000000 fileformats-0.6.3/fileformats/core/converter.py
+-rw-r--r--   0        0        0    10508 2020-02-02 00:00:00.000000 fileformats-0.6.3/fileformats/core/datatype.py
+-rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 fileformats-0.6.3/fileformats/core/exceptions.py
+-rw-r--r--   0        0        0     1218 2020-02-02 00:00:00.000000 fileformats-0.6.3/fileformats/core/field.py
+-rw-r--r--   0        0        0    32098 2020-02-02 00:00:00.000000 fileformats-0.6.3/fileformats/core/fileset.py
+-rw-r--r--   0        0        0     4612 2020-02-02 00:00:00.000000 fileformats-0.6.3/fileformats/core/mark.py
+-rw-r--r--   0        0        0    24544 2020-02-02 00:00:00.000000 fileformats-0.6.3/fileformats/core/mixin.py
+-rw-r--r--   0        0        0     8213 2020-02-02 00:00:00.000000 fileformats-0.6.3/fileformats/core/utils.py
+-rw-r--r--   0        0        0     8171 2020-02-02 00:00:00.000000 fileformats-0.6.3/fileformats/core/tests/test_classifiers.py
+-rw-r--r--   0        0        0     3990 2020-02-02 00:00:00.000000 fileformats-0.6.3/fileformats/core/tests/test_converter.py
+-rw-r--r--   0        0        0     5998 2020-02-02 00:00:00.000000 fileformats-0.6.3/fileformats/core/tests/test_detection.py
+-rw-r--r--   0        0        0     3336 2020-02-02 00:00:00.000000 fileformats-0.6.3/fileformats/core/tests/test_general.py
+-rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 fileformats-0.6.3/fileformats/core/tests/test_mime.py
+-rw-r--r--   0        0        0     7043 2020-02-02 00:00:00.000000 fileformats-0.6.3/fileformats/core/tests/test_mixin.py
+-rw-r--r--   0        0        0     6954 2020-02-02 00:00:00.000000 fileformats-0.6.3/fileformats/core/tests/test_utils.py
+-rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 fileformats-0.6.3/fileformats/document/__init__.py
+-rw-r--r--   0        0        0     4843 2020-02-02 00:00:00.000000 fileformats-0.6.3/fileformats/field/__init__.py
+-rw-r--r--   0        0        0     2205 2020-02-02 00:00:00.000000 fileformats-0.6.3/fileformats/field/tests/test_fields.py
+-rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 fileformats-0.6.3/fileformats/field/tests/test_fields_mime.py
+-rw-r--r--   0        0        0     7940 2020-02-02 00:00:00.000000 fileformats-0.6.3/fileformats/generic/__init__.py
+-rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 fileformats-0.6.3/fileformats/image/__init__.py
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 fileformats-0.6.3/fileformats/image/base.py
+-rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 fileformats-0.6.3/fileformats/image/converters.py
+-rw-r--r--   0        0        0     1893 2020-02-02 00:00:00.000000 fileformats-0.6.3/fileformats/image/raster.py
+-rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 fileformats-0.6.3/fileformats/image/vector.py
+-rw-r--r--   0        0        0      536 2020-02-02 00:00:00.000000 fileformats-0.6.3/fileformats/image/tests/test_image_converters.py
+-rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 fileformats-0.6.3/fileformats/image/tests/test_image_raster.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 fileformats-0.6.3/fileformats/misc/__init__.py
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 fileformats-0.6.3/fileformats/misc/medical.py
+-rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 fileformats-0.6.3/fileformats/numeric/__init__.py
+-rw-r--r--   0        0        0     2159 2020-02-02 00:00:00.000000 fileformats-0.6.3/fileformats/serialization/__init__.py
+-rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 fileformats-0.6.3/fileformats/serialization/converters.py
+-rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 fileformats-0.6.3/fileformats/serialization/tests/test_serialization_converters.py
+-rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 fileformats-0.6.3/fileformats/text/__init__.py
+-rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 fileformats-0.6.3/fileformats/video/__init__.py
+-rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 fileformats-0.6.3/.gitignore
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 fileformats-0.6.3/AUTHORS
+-rw-r--r--   0        0        0    14222 2020-02-02 00:00:00.000000 fileformats-0.6.3/LICENSE
+-rw-r--r--   0        0        0     5235 2020-02-02 00:00:00.000000 fileformats-0.6.3/README.rst
+-rw-r--r--   0        0        0     2458 2020-02-02 00:00:00.000000 fileformats-0.6.3/pyproject.toml
+-rw-r--r--   0        0        0    22512 2020-02-02 00:00:00.000000 fileformats-0.6.3/PKG-INFO
```

### Comparing `fileformats-0.6.2/fileformats/archive/__init__.py` & `fileformats-0.6.3/fileformats/archive/__init__.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.6.2/fileformats/archive/converters.py` & `fileformats-0.6.3/fileformats/archive/converters.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.6.2/fileformats/archive/tests/test_archive_converters.py` & `fileformats-0.6.3/fileformats/archive/tests/test_archive_converters.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.6.2/fileformats/audio/__init__.py` & `fileformats-0.6.3/fileformats/audio/__init__.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.6.2/fileformats/core/base.py` & `fileformats-0.6.3/fileformats/core/fileset.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,309 +1,50 @@
 from __future__ import annotations
 import os
 from copy import copy
 import struct
-from inspect import isclass
+from enum import Enum
 from warnings import warn
 import traceback
 import typing as ty
 import importlib
 import shutil
 from operator import itemgetter
 import itertools
 import functools
 from pathlib import Path
 import hashlib
 import logging
 import attrs
 from .utils import (
-    subpackages,
     classproperty,
     fspaths_converter,
     to_mime_format_name,
-    from_mime_format_name,
     STANDARD_NAMESPACES,
-    add_exc_note,
     describe_task,
 )
 from .converter import SubtypeVar
 from .exceptions import (
     FileFormatsError,
     FormatMismatchError,
     FormatConversionError,
-    FormatRecognitionError,
 )
+from .datatype import DataType
 
 # Tools imported from Arcana, will remove again once file-formats and "cells"
 # have been split
 REQUIRED_ANNOTATION = "__fileformats_required__"
 CHECK_ANNOTATION = "__fileformats_check__"
 
 FILE_CHUNK_LEN_DEFAULT = 8192
 
 
 logger = logging.getLogger("fileformats")
 
 
-class DataType:
-    is_fileset = False
-    is_field = False
-
-    @classmethod
-    def type_var(cls, name):
-        return SubtypeVar(name, cls)
-
-    @classmethod
-    def matches(cls, values) -> bool:
-        """Checks whether the given value (fspaths for file-sets) match the datatype
-        specified by the class
-
-        Parameters
-        ----------
-        values : ty.Any
-            values to check whether they match the given datatype
-
-        Returns
-        -------
-        matches : bool
-            whether the datatype matches the provided values
-        """
-        try:
-            cls(values)
-        except FormatMismatchError:
-            return False
-        else:
-            return True
-
-    @classmethod
-    def issubtype(cls, super_type: type, allow_same: bool = True):
-        """Check to see whether datatype class is a subtype of a given super class.
-        In this case the subtype is expected to be able to be treated as if it was
-        the super class.
-
-        Overridden in the ``WithClassifiers`` mixin to add support for
-        classified subtypes
-
-        Parameters
-        ----------
-        super_type : type
-            the class to check whether the given class is a subtype of
-        allow_same : bool, optional
-            whether there is a match if the classes are the same, by default True
-
-        Returns
-        -------
-        is_subtype : bool
-            whether or not the current class can be considered a subtype of the super (or
-            is the super itself)
-        """
-        if allow_same and cls is super_type:
-            return True
-        if isinstance(super_type, SubtypeVar):
-            super_type = super_type.base
-        return issubclass(cls, super_type)
-
-    @classproperty
-    def namespace(cls):
-        """The "namespace" the format belongs to under the "fileformats" umbrella
-        namespace"""
-        module_parts = cls.__module__.split(".")
-        if module_parts[0] != "fileformats":
-            raise FileFormatsError(
-                f"Cannot create reversible MIME type for {cls} as it is not in the "
-                "fileformats namespace"
-            )
-        return module_parts[1]
-
-    @classproperty
-    def all_types(self):
-        return itertools.chain(FileSet.all_formats, Field.all_fields)
-
-    @classmethod
-    def subclasses(cls):
-        """Iterate over all installed subclasses"""
-        for subpkg in subpackages():
-            for attr_name in dir(subpkg):
-                attr = getattr(subpkg, attr_name)
-                if isclass(attr) and issubclass(attr, cls):
-                    yield attr
-
-    @classmethod
-    def get_converter(cls, source_format: type, name: str = "converter", **kwargs):
-        if source_format.issubtype(cls):
-            return None
-        else:
-            raise FormatConversionError(
-                f"Cannot converter between '{cls.mime_like}' and '{source_format.mime_like}'"
-            )
-
-    @classproperty
-    def mime_like(cls):
-        """Generates a "MIME-like" identifier from a format class (i.e.
-        an identifier for a non-MIME class in the MIME style), e.g.
-
-            fileformats.text.Plain to "text/plain"
-
-        and
-
-            fileformats.image.TiffFx to "image/tiff-fx"
-
-        Parameters
-        ----------
-        klass : type(FileSet)
-            FileSet subclass
-        iana_mime : bool
-            whether to use standardised IANA format or a more relaxed type format corresponding
-            to the fileformats extension the type belongs to
-
-        Returns
-        -------
-        type
-            the corresponding file format class
-        """
-        mime = f"{cls.namespace}/{to_mime_format_name(cls.__name__)}"
-        try:
-            cls.from_mime(mime)
-        except FormatRecognitionError as e:
-            add_exc_note(
-                e,
-                (
-                    f"Cannot create reversible MIME type for {cls} as it is not present "
-                    f"in a top-level fileformats namespace package '{cls.namespace}'"
-                ),
-            )
-            raise e
-        return mime
-
-    @classmethod
-    def from_mime(cls, mime_string):
-        """Resolves a FileFormat class from a MIME (IANA) or "MIME-like" identifier (i.e.
-        an identifier for a non-MIME class in the MIME style), e.g.
-
-            "text/plain" resolves to fileformats.text.Plain
-
-        and
-
-            "image/tiff-fx" resolves to fileformats.image.TiffFx
-
-        Parameters
-        ----------
-        mime_string : str
-            MIME identifier
-
-        Returns
-        -------
-        type
-            the corresponding file format class
-        """
-        try:
-            namespace, format_name = mime_string.split("/")
-        except ValueError:
-            raise FormatRecognitionError(
-                f"Format '{mime_string}' is not a valid MIME-like format of <namespace>/<format>"
-            )
-        try:
-            return FileSet.formats_by_iana_mime[mime_string]
-        except KeyError:
-            pass
-        if namespace == "application":
-            # We treat the "application" namespace as a catch-all for any formats that are
-            # not explicitly covered by the IANA standard (which is kind of how the IANA
-            # treats it). Therefore, we loop through all subclasses across the different
-            # namespaces to find one that matches the name.
-            if not format_name.startswith("x-"):
-                raise FormatRecognitionError(
-                    "Did not find class matching official (i.e. non-extension) MIME type "
-                    f"{mime_string} (i.e. one not starting with 'application/x-'"
-                ) from None
-            format_name = format_name[2:]  # remove "x-" prefix
-            matching_name = FileSet.formats_by_name[format_name]
-            if not matching_name:
-                namespace_names = [n.__name__ for n in subpackages()]
-                class_name = from_mime_format_name(format_name)
-                raise FormatRecognitionError(
-                    f"Did not find class matching extension the class name '{class_name}' "
-                    f"corresponding to MIME type '{mime_string}' "
-                    f"in any of the installed namespaces: {namespace_names}"
-                )
-            elif len(matching_name) > 1:
-                namespace_names = [f.__module__.__name__ for f in matching_name]
-                raise FormatRecognitionError(
-                    f"Ambiguous extended MIME type '{mime_string}', could refer to "
-                    f"{', '.join(repr(f) for f in matching_name)} installed types. "
-                    f"Explicitly set the 'iana_mime' attribute on one or all of these types "
-                    f"to disambiguate, or uninstall all but one of the following "
-                    "namespaces: "
-                )
-            else:
-                klass = next(iter(matching_name))
-        else:
-            class_name = from_mime_format_name(format_name)
-            try:
-                module = importlib.import_module("fileformats." + namespace)
-            except ImportError:
-                raise FormatRecognitionError(
-                    f"Did not find fileformats namespace package corresponding to {namespace} "
-                    f"required to interpret '{mime_string}' MIME, or MIME-like, type. "
-                    f"try installing the namespace package with "
-                    f"'python3 -m pip install fileformats-{namespace}'."
-                ) from None
-            try:
-                klass = getattr(module, class_name)
-            except AttributeError:
-                if "+" in format_name:
-                    qualifier_names, classified_name = format_name.split("+")
-                    try:
-                        classifiers = [
-                            getattr(module, from_mime_format_name(q))
-                            for q in qualifier_names.split(".")
-                        ]
-                    except AttributeError:
-                        raise FormatRecognitionError(
-                            f"Could not load classifiers [{qualifier_names}] from "
-                            f"fileformats.{namespace}, corresponding to MIME, "
-                            f"or MIME-like, type {mime_string}"
-                        ) from None
-                    try:
-                        classified = getattr(
-                            module, from_mime_format_name(classified_name)
-                        )
-                    except AttributeError:
-                        try:
-                            classified = cls.generically_qualifies_by_name[
-                                classified_name
-                            ]
-                        except KeyError:
-                            raise FormatRecognitionError(
-                                f"Could not load classified class '{classified_name}' from "
-                                f"fileformats.{namespace} or list of generic types "
-                                f"({list(cls.generically_qualifies_by_name)}), "
-                                f"corresponding to MIME, or MIME-like, type {mime_string}"
-                            ) from None
-                    klass = classified[classifiers]
-                else:
-                    raise FormatRecognitionError(
-                        f"Did not find '{class_name}' class in fileformats.{namespace} "
-                        f"corresponding to MIME, or MIME-like, type {mime_string}"
-                    ) from None
-        return klass
-
-    @classproperty
-    def generically_qualifies_by_name(cls):
-        if cls._generically_qualifies_by_name is None:
-            cls._generically_qualifies_by_name = {
-                to_mime_format_name(f.__name__): f
-                for f in FileSet.all_formats
-                if getattr(f, "generically_qualifies", False)
-            }
-        return cls._generically_qualifies_by_name
-
-    _generically_qualifies_by_name = None  # Register all generically classified types
-
-
 @attrs.define
 class FileSet(DataType):
     """
     The base class for all format types within the fileformats package. A generic
     representation of a collection of files related to a single data resource. A
     file-set can be a single file or directory or a collection thereof, such as a
     primary file with a "side-car" header.
@@ -333,14 +74,55 @@
 
     # Store converters registered by @converter decorator that convert to FileSet
     # NB: each class will have its own version of this dictionary
     converters = {}
 
     is_fileset = True
 
+    class CopyMode(Enum):
+        """Designates the desired behaviour of the FileSet.copy() method"""
+
+        dont_copy = 0b0001  # simply leave the files where they are (i.e. don't copy)
+        symlink = 0b0010  # symlink the file into the destination directory
+        hardlink = 0b0100  # hardlink the file into the destination directory
+        copy = (
+            0b1000  # duplicate (actually copy) the file into the destination directory
+        )
+
+        link = 0b0110  # use either linking method (preferring symbolic)
+        link_or_copy = 0b1110  # use either linking method or copy (preferring symbolic, hardlink and then copy)
+        symlink_or_copy = 0b1010
+        hardlink_or_copy = 0b1100
+
+        # Masks
+        all = 0b1111  # use any method (preferring dont_copy)
+        no_supported = 0b0000  # none of the requested methods are supported
+
+        # rarely used combinations
+        dont_copy_or_symlink = 0b0011
+        dont_copy_or_hardlink = 0b0101
+        dont_copy_or_link = 0b0111
+        dont_copy_or_symlink_or_copy = 0b1011
+        dont_copy_or_hardlink_or_copy = 0b1101
+
+        def __xor__(self, other):
+            return type(self)(self.value ^ other.value)
+
+        def __and__(self, other):
+            return type(self)(self.value & other.value)
+
+        def __or__(self, other):
+            return type(self)(self.value | other.value)
+
+        def __sub__(self, other):
+            return type(self)((self.value & (self.value ^ other.value)))
+
+        def __bool__(self):
+            return bool(self.value)
+
     def __hash__(self):
         return hash(sorted(self.fspaths))
 
     def __repr__(self):
         return f"{type(self).__name__}('" + "', '".join(self.fspaths) + "')"
 
     def __attrs_post_init__(self):
@@ -473,67 +255,75 @@
             else:
                 yield attr_name
 
     def copy(
         self,
         dest_dir: Path,
         stem: ty.Optional[str] = None,
-        link_type: ty.Optional[str] = None,
+        mode: ty.Union[CopyMode, str] = CopyMode.copy,
         trim: bool = True,
         make_dirs: bool = False,
         overwrite: bool = False,
+        supported_modes: CopyMode = CopyMode.all,
     ):
         """Copies the file-set to a new directory, optionally renaming the files
         to have consistent name-stems.
 
         Parameters
         ----------
         dest_dir : str
             Path to the parent directory to save the file-set
         stem: str, optional
             the file name excluding file extensions, to give the files/dirs in the parent
             directory, by default the original file name is used
-        link_type : str, optional
-            Whether to use hard ('hard') or symbolic ('symbolic') links instead of
-            copying files to the new location. If None then the files are copied,
-            None by default.
+        mode : CopyMode or str, optional
+            designates whether to perform an actual copy or whether a link (symbolic or
+            hard) is okay, 'duplicate' by default.
         trim : bool, optional
             Only copy the paths in the file-set that are "required" by the format,
             true by default
         make_dirs : bool, optional
             Make the parent destination and all missing ancestors if they are missing,
             false by default
         overwrite : bool, optional
             whether to overwrite existing files/directories if present
-        """
+        supported_modes : CopyMode, optional
+            supported modes for the copy operation. Used to mask out the requested
+            copy mode
+        """
+        mode = self.CopyMode[mode] if isinstance(mode, str) else mode
+        selected_mode = mode & supported_modes
+        if not selected_mode:
+            raise FileFormatsError(
+                f"Cannot copy {self} using {mode} mode as it is not supported "
+                f"({supported_modes})"
+            )
+        if selected_mode & self.CopyMode.dont_copy:
+            return self
         dest_dir = Path(dest_dir)  # ensure a Path not a string
         if make_dirs:
             dest_dir.mkdir(parents=True, exist_ok=True)
-        if link_type is None:
-            copy_dir = shutil.copytree
-            copy_file = shutil.copyfile
-        elif link_type == "hard":
+        if selected_mode & self.CopyMode.symlink:
+            copy_dir = copy_file = os.symlink
+        elif selected_mode & self.CopyMode.hardlink:
             copy_file = os.link
 
             def hardlink_dir(src: Path, dest: Path):
                 for dpath, _, fpaths in os.walk(src):
                     dpath = Path(dpath)
                     relpath = dpath.relative_to(src)
                     (dest / relpath).mkdir()
                     for fpath in fpaths:
                         os.link(dpath / fpath, dest / relpath / fpath)
 
             copy_dir = hardlink_dir
-        elif link_type == "symbolic":
-            copy_dir = copy_file = os.symlink
         else:
-            raise FileFormatsError(
-                f"Unrecognised link_type option {link_type}, can be 'hard', 'symbolic' "
-                "or None"
-            )
+            assert selected_mode & self.CopyMode.copy
+            copy_dir = shutil.copytree
+            copy_file = shutil.copyfile
         new_paths = []
         if trim and self.required_paths():
             fspaths_to_copy = self.required_paths()
         else:
             fspaths_to_copy = self.fspaths
         if not fspaths_to_copy:
             raise FileFormatsError(
@@ -562,14 +352,15 @@
             else:
                 copy_file(fspath, new_path)
             new_paths.append(new_path)
         return type(self)(new_paths)
 
     def copy_to(self, *args, **kwargs):
         """For b/w compatibility (temporary message)"""
+        warn("'FileSet.copy_to()' has been deprecated, please use copy() instead")
         return self.copy(*args, **kwargs)
 
     def select_by_ext(
         self, fileformat: ty.Optional[type] = None, allow_none: bool = False
     ) -> Path:
         """Selects a single path from a set of file-system paths based on the file
         extension
@@ -1067,44 +858,7 @@
         for key, chunk_iter in self.byte_chunks():
             yield (",'" + key + "'=").encode()
             yield from chunk_iter
 
     _all_formats = None
     _formats_by_iana_mime = None
     _formats_by_name = None
-
-
-@attrs.define
-class Field(DataType):
-    value = attrs.field()
-
-    type = None
-    is_field = True
-    primitive = None
-
-    def __str__(self):
-        return str(self.value)
-
-    @property
-    def metadata(self):
-        return {}
-
-    @classproperty
-    def all_fields(cls) -> list[ty.Type[Field]]:  # pylint: disable=no-self-argument
-        """Iterate over all field formats in fileformats.* namespaces"""
-        import fileformats.field  # noqa
-
-        return [f for f in Field.subclasses() if f.primitive is not None]
-
-    @classmethod
-    def from_primitive(cls, dtype: type):
-        try:
-            datatype = next(iter(f for f in cls.all_fields if f.primitive is dtype))
-        except StopIteration as e:
-            field_types_str = ", ".join(t.__name__ for t in cls.all_fields)
-            raise FileFormatsError(
-                f"{dtype} doesn't not correspond to a valid fileformats field type "
-                f"({field_types_str})"
-            ) from e
-        return datatype
-
-    _all_fields = None
```

### Comparing `fileformats-0.6.2/fileformats/core/converter.py` & `fileformats-0.6.3/fileformats/core/converter.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.6.2/fileformats/core/mark.py` & `fileformats-0.6.3/fileformats/core/mark.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import importlib
 import attrs
-from .base import DataType, REQUIRED_ANNOTATION, CHECK_ANNOTATION
+from .fileset import DataType, REQUIRED_ANNOTATION, CHECK_ANNOTATION
 from .converter import ConverterWrapper
 from .exceptions import FormatConversionError
 
 
 __all__ = ["required", "check", "converter"]
```

### Comparing `fileformats-0.6.2/fileformats/core/mixin.py` & `fileformats-0.6.3/fileformats/core/mixin.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from pathlib import Path
 import typing as ty
 from collections import Counter
 from . import mark
-from .base import FileSet
+from .fileset import FileSet
 from .utils import classproperty, describe_task, to_mime_format_name
 from .converter import SubtypeVar
 from .exceptions import FileFormatsError, FormatMismatchError, FormatRecognitionError
 
 
 class WithMagicNumber:
     """Mixin class for Files with magic numbers at the start of their
```

### Comparing `fileformats-0.6.2/fileformats/core/utils.py` & `fileformats-0.6.3/fileformats/core/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -275,81 +275,7 @@
     if inspect.isfunction(task):
         import cloudpickle
 
         task = cloudpickle.loads(task().inputs._func)
     src_file = inspect.getsourcefile(task)
     src_line = inspect.getsourcelines(task)[-1]
     return f"{task} (defined at line {src_line} of {src_file})"
-
-
-# def on_cifs(fname):
-#     """
-#     Check whether a file path is on a CIFS filesystem mounted in a POSIX host.
-
-#     POSIX hosts are assumed to have the ``mount`` command.
-
-#     On Windows, Docker mounts host directories into containers through CIFS
-#     shares, which has support for Minshall+French symlinks, or text files that
-#     the CIFS driver exposes to the OS as symlinks.
-#     We have found that under concurrent access to the filesystem, this feature
-#     can result in failures to create or read recently-created symlinks,
-#     leading to inconsistent behavior and ``FileNotFoundError`` errors.
-
-#     This check is written to support disabling symlinks on CIFS shares.
-
-#     NB: This function and sub-functions are copied from the nipype.utils.filemanip module
-
-#     """
-#     # Only the first match (most recent parent) counts
-#     for fspath, fstype in _cifs_table:
-#         if fname.startswith(fspath):
-#             return fstype == "cifs"
-#     return False
-
-
-# def _generate_cifs_table():
-#     """
-#     Construct a reverse-length-ordered list of mount points that fall under a CIFS mount.
-
-#     This precomputation allows efficient checking for whether a given path
-#     would be on a CIFS filesystem.
-#     On systems without a ``mount`` command, or with no CIFS mounts, returns an
-#     empty list.
-
-#     """
-#     exit_code, output = sp.getstatusoutput("mount")
-
-#     # Not POSIX
-#     if exit_code != 0:
-#         return []
-
-#     # Linux mount example:  sysfs on /sys type sysfs (rw,nosuid,nodev,noexec)
-#     #                          <PATH>^^^^      ^^^^^<FSTYPE>
-#     # OSX mount example:    /dev/disk2 on / (hfs, local, journaled)
-#     #                               <PATH>^  ^^^<FSTYPE>
-#     pattern = re.compile(r".*? on (/.*?) (?:type |\()([^\s,\)]+)")
-
-#     # Keep line and match for error reporting (match == None on failure)
-#     # Ignore empty lines
-#     matches = [(ll, pattern.match(ll)) for ll in output.strip().splitlines() if ll]
-
-#     # (path, fstype) tuples, sorted by path length (longest first)
-#     mount_info = sorted(
-#         (match.groups() for _, match in matches if match is not None),
-#         key=lambda x: len(x[0]),
-#         reverse=True,
-#     )
-#     cifs_paths = [path for path, fstype in mount_info if fstype.lower() == "cifs"]
-
-#     # Report failures as warnings
-#     for line, match in matches:
-#         if match is None:
-#             logger.debug("Cannot parse mount line: '%s'", line)
-
-#     return [
-#         mount
-#         for mount in mount_info
-#         if any(mount[0].startswith(path) for path in cifs_paths)
-#     ]
-
-
-# _cifs_table = _generate_cifs_table()
```

### Comparing `fileformats-0.6.2/fileformats/core/tests/test_classifiers.py` & `fileformats-0.6.3/fileformats/core/tests/test_classifiers.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.6.2/fileformats/core/tests/test_converter.py` & `fileformats-0.6.3/fileformats/core/tests/test_converter.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.6.2/fileformats/core/tests/test_detection.py` & `fileformats-0.6.3/fileformats/core/tests/test_detection.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.6.2/fileformats/core/tests/test_general.py` & `fileformats-0.6.3/fileformats/core/tests/test_general.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.6.2/fileformats/core/tests/test_mime.py` & `fileformats-0.6.3/fileformats/core/tests/test_mime.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.6.2/fileformats/core/tests/test_mixin.py` & `fileformats-0.6.3/fileformats/core/tests/test_mixin.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.6.2/fileformats/core/tests/test_utils.py` & `fileformats-0.6.3/fileformats/core/tests/test_utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -69,23 +69,47 @@
     cpy = fsobject.copy(dest_dir)
     assert all(p.parent == dest_dir for p in cpy.fspaths)
     assert set(p.name for p in cpy.fspaths) == set(p.name for p in fsobject.fspaths)
     assert cpy.hash() == fsobject.hash()
 
 
 def test_copy_symlink(fsobject: FsObject, dest_dir: Path):
-    cpy = fsobject.copy(dest_dir, link_type="symbolic")
+    cpy = fsobject.copy(dest_dir, mode=File.CopyMode.symlink)
     assert all(p.parent == dest_dir for p in cpy.fspaths)
     assert set(p.name for p in cpy.fspaths) == set(p.name for p in fsobject.fspaths)
-    assert set(p.is_symlink() for p in cpy.fspaths)
+    assert all(p.is_symlink() for p in cpy.fspaths)
+    assert cpy.hash() == fsobject.hash()
+
+
+def test_copy_symlink_with_fallback(fsobject: FsObject, dest_dir: Path):
+    "Simulate source object on CIFS share, should be copied not symlinked"
+    cpy = fsobject.copy(
+        dest_dir,
+        mode=File.CopyMode.link_or_copy,
+        supported_modes=File.CopyMode.hardlink_or_copy,
+    )
+    assert all(p.parent == dest_dir for p in cpy.fspaths)
+    assert set(p.name for p in cpy.fspaths) == set(p.name for p in fsobject.fspaths)
+    assert not any(p.is_symlink() for p in cpy.fspaths)
+    assert cpy.hash() == fsobject.hash()
+
+
+def test_copy_symlink_with_unrequired_fallback(fsobject: FsObject, dest_dir: Path):
+    "Simulate source object not on CIFS share, should be symlinked not copied"
+    cpy = fsobject.copy(
+        dest_dir, mode=File.CopyMode.link_or_copy, supported_modes=File.CopyMode.link
+    )
+    assert all(p.parent == dest_dir for p in cpy.fspaths)
+    assert set(p.name for p in cpy.fspaths) == set(p.name for p in fsobject.fspaths)
+    assert all(p.is_symlink() for p in cpy.fspaths)
     assert cpy.hash() == fsobject.hash()
 
 
 def test_copy_hardlink(fsobject: FsObject, dest_dir: Path):
-    cpy = fsobject.copy(dest_dir, link_type="hard")
+    cpy = fsobject.copy(dest_dir, mode=File.CopyMode.symlink)
     assert all(p.parent == dest_dir for p in cpy.fspaths)
     assert set(p.name for p in cpy.fspaths) == set(p.name for p in fsobject.fspaths)
     assert all(
         os.path.samefile(c, o)
         for c, o in zip(sorted(cpy.fspaths), sorted(fsobject.fspaths))
         if o.is_file()
     )
```

### Comparing `fileformats-0.6.2/fileformats/document/__init__.py` & `fileformats-0.6.3/fileformats/document/__init__.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.6.2/fileformats/field/__init__.py` & `fileformats-0.6.3/fileformats/field/__init__.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.6.2/fileformats/field/tests/test_fields.py` & `fileformats-0.6.3/fileformats/field/tests/test_fields.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.6.2/fileformats/field/tests/test_fields_mime.py` & `fileformats-0.6.3/fileformats/field/tests/test_fields_mime.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.6.2/fileformats/generic/__init__.py` & `fileformats-0.6.3/fileformats/generic/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
 from pathlib import Path
 import attrs
-from fileformats.core.base import FileSet
+from fileformats.core.fileset import FileSet
 from fileformats.core.exceptions import FormatMismatchError, FileFormatsError
 from fileformats.core import mark
 from fileformats.core.utils import splitext, classproperty
 from fileformats.core.mixin import WithClassifiers
 
 
 @attrs.define
```

### Comparing `fileformats-0.6.2/fileformats/image/converters.py` & `fileformats-0.6.3/fileformats/image/converters.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.6.2/fileformats/image/raster.py` & `fileformats-0.6.3/fileformats/image/raster.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.6.2/fileformats/image/tests/test_image_converters.py` & `fileformats-0.6.3/fileformats/image/tests/test_image_converters.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.6.2/fileformats/image/tests/test_image_raster.py` & `fileformats-0.6.3/fileformats/image/tests/test_image_raster.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.6.2/fileformats/serialization/__init__.py` & `fileformats-0.6.3/fileformats/serialization/__init__.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.6.2/fileformats/serialization/converters.py` & `fileformats-0.6.3/fileformats/serialization/converters.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.6.2/fileformats/serialization/tests/test_serialization_converters.py` & `fileformats-0.6.3/fileformats/serialization/tests/test_serialization_converters.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.6.2/fileformats/text/__init__.py` & `fileformats-0.6.3/fileformats/text/__init__.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.6.2/LICENSE` & `fileformats-0.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `fileformats-0.6.2/README.rst` & `fileformats-0.6.3/README.rst`

 * *Files identical despite different names*

### Comparing `fileformats-0.6.2/pyproject.toml` & `fileformats-0.6.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fileformats-0.6.2/PKG-INFO` & `fileformats-0.6.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fileformats
-Version: 0.6.2
+Version: 0.6.3
 Summary: Classes for representing different file formats in Python classes for use in type hinting in data workflows
 Project-URL: repository, https://github.com/ArcanaFramework/fileformats
 Author-email: "Thomas G. Close" <tom.g.close@gmail.com>
 Maintainer-email: "Thomas G. Close" <tom.g.close@gmail.com>
 License: Creative Commons Attribution 4.0 International Public License
         By exercising the Licensed Rights (defined below), You accept and agree to be bound by the terms and conditions of this Creative Commons Attribution 4.0 International Public License ("Public License"). To the extent this Public License may be interpreted as a contract, You are granted the Licensed Rights in consideration of Your acceptance of these terms and conditions, and the Licensor grants You such rights in consideration of benefits the Licensor receives from making the Licensed Material available under these terms and conditions.
```

