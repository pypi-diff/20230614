# Comparing `tmp/pymetasnap-0.1.0.tar.gz` & `tmp/pymetasnap-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymetasnap-0.1.0.tar", max compression
+gzip compressed data, was "pymetasnap-0.1.1.tar", max compression
```

## Comparing `pymetasnap-0.1.0.tar` & `pymetasnap-0.1.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1073 2023-06-13 21:50:58.885304 pymetasnap-0.1.0/LICENSE
--rw-r--r--   0        0        0     2858 2023-06-13 21:50:58.885304 pymetasnap-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-06-13 21:50:58.885304 pymetasnap-0.1.0/extractor/__init__.py
--rw-r--r--   0        0        0     2403 2023-06-13 21:50:58.885304 pymetasnap-0.1.0/extractor/core.py
--rw-r--r--   0        0        0     1272 2023-06-13 21:50:58.885304 pymetasnap-0.1.0/extractor/main.py
--rw-r--r--   0        0        0     2465 2023-06-13 21:50:58.885304 pymetasnap-0.1.0/extractor/render.py
--rw-r--r--   0        0        0     1818 2023-06-13 21:50:58.885304 pymetasnap-0.1.0/extractor/utils.py
--rw-r--r--   0        0        0      763 2023-06-13 21:50:58.885304 pymetasnap-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     3779 1970-01-01 00:00:00.000000 pymetasnap-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-06-14 14:10:43.716731 pymetasnap-0.1.1/LICENSE
+-rw-r--r--   0        0        0     3003 2023-06-14 14:10:43.716731 pymetasnap-0.1.1/README.md
+-rw-r--r--   0        0        0        0 2023-06-14 14:10:43.716731 pymetasnap-0.1.1/extractor/__init__.py
+-rw-r--r--   0        0        0     2403 2023-06-14 14:10:43.716731 pymetasnap-0.1.1/extractor/core.py
+-rw-r--r--   0        0        0     1286 2023-06-14 14:10:43.716731 pymetasnap-0.1.1/extractor/main.py
+-rw-r--r--   0        0        0     2550 2023-06-14 14:10:43.716731 pymetasnap-0.1.1/extractor/render.py
+-rw-r--r--   0        0        0     1916 2023-06-14 14:10:43.716731 pymetasnap-0.1.1/extractor/utils.py
+-rw-r--r--   0        0        0      823 2023-06-14 14:10:43.716731 pymetasnap-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     3964 1970-01-01 00:00:00.000000 pymetasnap-0.1.1/PKG-INFO
```

### Comparing `pymetasnap-0.1.0/LICENSE` & `pymetasnap-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pymetasnap-0.1.0/README.md` & `pymetasnap-0.1.1/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,60 +1,69 @@
-# cli-pymetasnap
+# pymetasnap
 
-cli-pypi-metadata-extractor is a command-line tool that enables you to extract metadata from the Python Package Index (PyPI). It allows you to retrieve essential information about Python packages hosted on PyPI, including package names, versions, licenses, project URLs, and more.
+pymetasnap is a command-line tool that enables you to extract metadata from the Python Package Index (PyPI). It allows you to retrieve essential information about Python packages hosted on PyPI, including package names, versions, licenses, project URLs, and more.
 
-By leveraging the PyPI API, cli-pypi-metadata-extractor automates the process of gathering package metadata, making it convenient for developers, researchers, and anyone interested in exploring package information in a structured manner.
+By leveraging the PyPI API, pymetasnap automates the process of gathering package metadata, making it convenient for developers, researchers, and anyone interested in exploring package information in a structured manner.
 
 ## Features
 
 Retrieve metadata for Python packages from PyPI.
 Extract package names, versions, licenses, and other relevant information.
 Fetch project URLs and version-specific URLs for detailed package exploration.
 Store the extracted metadata in CSV or Excel format for further analysis.
 
 ## Installation
 
-You can install cli-pypi-metadata-extractor using pip:
+You can install pymetasnap using pip:
 
 ```bash
-pip install cli-pypi-metadata-extractor
+pip install pymetasnap
 ```
 
-Usage
+### Usage
+
+#### Detached mode
+
 To extract metadata for Python packages from PyPI, use the following command:
 
 ```bash
-cli-pypi-metadata-extractor --source-path <path_of_the_txt_file> --output <output_path> --format <output_format>
+pymetasnap --source-path <path_of_the_txt_file> --output <output_path> --format <output_format>
 ```
 
 Replace the following placeholders in the command:
 
-`<path_of_the_txt_file>`: Names of the packages to retrieve metadata for (separated by spaces).
-`<output_path>`: Path to store the extracted metadata file.
-`<input_format>`: Format of the input file (csv or xlsx).
+- `<path_of_the_txt_file>`: Names of the packages to retrieve metadata for (separated by spaces).
+- `<output_path>`: Path to store the extracted metadata file.
+- `<input_format>`: Format of the input file (csv or xlsx).
 Example usage:
 
 ```bash
-cli-pypi-metadata-extractor --source-path ./requirements.txt --output metadata.csv --format csv
+pymetasnap --source-path ./requirements.txt --output metadata.csv --format csv
 ```
 
+#### Interactive mode
+
+Additionally, an interactive mode is available, allowing you to provide the required values through user prompts as follows:
+
+[![asciicast](https://asciinema.org/a/4xs1k6elJ40kJ4YhKxuS93Rfh.svg)](https://asciinema.org/a/4xs1k6elJ40kJ4YhKxuS93Rfh)
+
 ## Output
 
 The tool generates a file containing the extracted metadata for the specified packages in the provided output format (CSV or Excel). The output file includes columns for package name, version, license, repository URL, project URL, and version-specific URL. This information can be used for various purposes, such as dependency analysis, license compliance, or package research.
 
 ## Contributing
 
-Contributions to cli-pypi-metadata-extractor are welcome! If you encounter any issues or have suggestions for improvements, please open an issue on the project's GitHub repository.
+Contributions to pymetasnap are welcome! If you encounter any issues or have suggestions for improvements, please open an issue on the project's GitHub repository.
 
 When contributing, please ensure that you follow the existing coding style, write tests for new features, and make sure the tests pass before submitting a pull request.
 
 ## License
 
-cli-pypi-metadata-extractor is licensed under the MIT License. See the LICENSE file for more details.
+pymetasnap is licensed under the MIT License. See the LICENSE file for more details.
 
 ## Acknowledgments
 
-The cli-pypi-metadata-extractor tool builds upon the PyPI API to provide a convenient way to access package metadata. We would like to express our gratitude to the PyPI maintainers and the Python community for their continuous efforts in maintaining and improving the Python Package Index.
+The pymetasnap tool builds upon the PyPI API to provide a convenient way to access package metadata. We would like to express our gratitude to the PyPI maintainers and the Python community for their continuous efforts in maintaining and improving the Python Package Index.
 
 ## Contact
 
 For any inquiries or feedback, please contact the project maintainer at cristian.o.rincon.b@gmail.com.
```

### Comparing `pymetasnap-0.1.0/extractor/core.py` & `pymetasnap-0.1.1/extractor/core.py`

 * *Files identical despite different names*

### Comparing `pymetasnap-0.1.0/extractor/main.py` & `pymetasnap-0.1.1/extractor/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 
 @app.command(name="version")
 def version():
     return print(get_version_from_pyproject())
 
 
-@app.command()
+@app.command(name="extract")
 def main(
     source_path: Annotated[
         Path,
         typer.Option(
             exists=True,
             file_okay=True,
             dir_okay=False,
```

### Comparing `pymetasnap-0.1.0/extractor/render.py` & `pymetasnap-0.1.1/extractor/render.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
+"""This module contains Requirements class, which is the core of the current process."""
+
 import re
 from typing import List, Tuple
 
-from loguru import logger
-
 
 class Requirements:
     """
     A class that handles parsing and rendering requirements data.
 
     Attributes:
         None
@@ -24,15 +24,15 @@
 
         Args:
             source_path: The path to the file to be read.
 
         Returns:
             The contents of the file as a string.
         """
-        return open(source_path).read()
+        return open(source_path, "r").read()
 
     def _from_pip_freeze(self, data: str) -> List[Tuple[str, str]]:
         """
         Parse data in the pip freeze format.
 
         Args:
             data: The pip freeze formatted data to be parsed.
@@ -56,23 +56,23 @@
             data: The pip list formatted data to be parsed.
 
         Returns:
             A list of tuples containing package names and versions.
         """
         lines = data.strip().split("\n")
         package_data = [tuple(line.split()) for line in lines[2:]]
-        return [(package[0], package[1]) for package in package_data]
+        return [(package[0], package[1]) for package in package_data]  # pylint
 
     def render(self, source_path: str, format: str) -> List[Tuple[str, str]]:
         """
         Render the requirements data based on the specified format.
 
         Args:
             source_path: The path to the requirements file.
-            format: The format of the requirements file (e.g., "pip_freeze", "pip_list").
+            format: The format of the requirements file (e.g., "pip_freeze", "pip_list"). # noqa
 
         Returns:
             A list of tuples containing package names and versions.
         """
         data = self._read_file_contents(source_path)
         if format == "pip_freeze":
             return self._from_pip_freeze(data)
```

### Comparing `pymetasnap-0.1.0/extractor/utils.py` & `pymetasnap-0.1.1/extractor/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,31 +7,39 @@
 from extractor.core import filter_data, get_raw_data
 from extractor.render import Requirements
 
 
 def get_version_from_pyproject():
     with open("pyproject.toml") as f:
         pyproject_data = toml.load(f)
-        version = pyproject_data.get("tool", {}).get("poetry", {}).get("version")
+        version = (
+            pyproject_data.get("tool", {}).get("poetry", {}).get("version")
+        )  # noqa
     return version
 
 
 def filter_requirements(requirements_file_data, installed_requirements_data):
     base_reqs = [req[0] for req in requirements_file_data]
-    return [ireq for ireq in installed_requirements_data if ireq[0] in base_reqs]
+    return [
+        ireq for ireq in installed_requirements_data if ireq[0] in base_reqs
+    ]  # noqa
 
 
 def get_filtered_metadata(requirements_file, installed_requirements, output):
     handler = Requirements()
     print("Getting requirements list...")
     requirements_file_data = handler.render(requirements_file, "pip_freeze")
     print("Getting installed libraries list...")
-    installed_requirements_data = handler.render(installed_requirements, "pip_freeze")
-
-    result = filter_requirements(requirements_file_data, installed_requirements_data)
+    installed_requirements_data = handler.render(
+        installed_requirements, "pip_freeze"
+    )  # noqa
+
+    result = filter_requirements(
+        requirements_file_data, installed_requirements_data
+    )  # noqa
 
     pkgs_raw_metadata = []
     for pkg in track(result, description="Processing..."):
         filtered_data = filter_data(get_raw_data(pkg[0]), pkg[1])
         pkgs_raw_metadata.append(filtered_data)
     df = pd.DataFrame(pkgs_raw_metadata)
     print(f"Storing into: {output}")
```

### Comparing `pymetasnap-0.1.0/pyproject.toml` & `pymetasnap-0.1.1/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pymetasnap"
-version = "0.1.0"
+version = "0.1.1"
 description = "This package allows you to scrape metadata from the Python Package Index"
 authors = ["cristian-rincon <cristian.o.rincon.b@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "extractor"}]
 
 [tool.poetry.scripts]
@@ -16,16 +16,19 @@
 rich = "^13.4.1"
 shellingham = "^1.5.0.post1"
 openpyxl = "^3.1.2"
 pandas = "^2.0.2"
 loguru = "^0.7.0"
 requests = "^2.31.0"
 toml = "^0.10.2"
+pylint = "^2.17.4"
 
 
 [tool.poetry.group.dev.dependencies]
 black = {version = "^23.3.0", allow-prereleases = true}
 pytest = "^7.3.1"
+pylint = "^2.17.4"
+pre-commit = "^3.3.2"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `pymetasnap-0.1.0/PKG-INFO` & `pymetasnap-0.1.1/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,85 +1,95 @@
 Metadata-Version: 2.1
 Name: pymetasnap
-Version: 0.1.0
+Version: 0.1.1
 Summary: This package allows you to scrape metadata from the Python Package Index
 License: MIT
 Author: cristian-rincon
 Author-email: cristian.o.rincon.b@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: loguru (>=0.7.0,<0.8.0)
 Requires-Dist: openpyxl (>=3.1.2,<4.0.0)
 Requires-Dist: pandas (>=2.0.2,<3.0.0)
+Requires-Dist: pylint (>=2.17.4,<3.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: rich (>=13.4.1,<14.0.0)
 Requires-Dist: shellingham (>=1.5.0.post1,<2.0.0)
 Requires-Dist: toml (>=0.10.2,<0.11.0)
 Requires-Dist: typer[all] (>=0.9.0,<0.10.0)
 Description-Content-Type: text/markdown
 
-# cli-pymetasnap
+# pymetasnap
 
-cli-pypi-metadata-extractor is a command-line tool that enables you to extract metadata from the Python Package Index (PyPI). It allows you to retrieve essential information about Python packages hosted on PyPI, including package names, versions, licenses, project URLs, and more.
+pymetasnap is a command-line tool that enables you to extract metadata from the Python Package Index (PyPI). It allows you to retrieve essential information about Python packages hosted on PyPI, including package names, versions, licenses, project URLs, and more.
 
-By leveraging the PyPI API, cli-pypi-metadata-extractor automates the process of gathering package metadata, making it convenient for developers, researchers, and anyone interested in exploring package information in a structured manner.
+By leveraging the PyPI API, pymetasnap automates the process of gathering package metadata, making it convenient for developers, researchers, and anyone interested in exploring package information in a structured manner.
 
 ## Features
 
 Retrieve metadata for Python packages from PyPI.
 Extract package names, versions, licenses, and other relevant information.
 Fetch project URLs and version-specific URLs for detailed package exploration.
 Store the extracted metadata in CSV or Excel format for further analysis.
 
 ## Installation
 
-You can install cli-pypi-metadata-extractor using pip:
+You can install pymetasnap using pip:
 
 ```bash
-pip install cli-pypi-metadata-extractor
+pip install pymetasnap
 ```
 
-Usage
+### Usage
+
+#### Detached mode
+
 To extract metadata for Python packages from PyPI, use the following command:
 
 ```bash
-cli-pypi-metadata-extractor --source-path <path_of_the_txt_file> --output <output_path> --format <output_format>
+pymetasnap --source-path <path_of_the_txt_file> --output <output_path> --format <output_format>
 ```
 
 Replace the following placeholders in the command:
 
-`<path_of_the_txt_file>`: Names of the packages to retrieve metadata for (separated by spaces).
-`<output_path>`: Path to store the extracted metadata file.
-`<input_format>`: Format of the input file (csv or xlsx).
+- `<path_of_the_txt_file>`: Names of the packages to retrieve metadata for (separated by spaces).
+- `<output_path>`: Path to store the extracted metadata file.
+- `<input_format>`: Format of the input file (csv or xlsx).
 Example usage:
 
 ```bash
-cli-pypi-metadata-extractor --source-path ./requirements.txt --output metadata.csv --format csv
+pymetasnap --source-path ./requirements.txt --output metadata.csv --format csv
 ```
 
+#### Interactive mode
+
+Additionally, an interactive mode is available, allowing you to provide the required values through user prompts as follows:
+
+[![asciicast](https://asciinema.org/a/4xs1k6elJ40kJ4YhKxuS93Rfh.svg)](https://asciinema.org/a/4xs1k6elJ40kJ4YhKxuS93Rfh)
+
 ## Output
 
 The tool generates a file containing the extracted metadata for the specified packages in the provided output format (CSV or Excel). The output file includes columns for package name, version, license, repository URL, project URL, and version-specific URL. This information can be used for various purposes, such as dependency analysis, license compliance, or package research.
 
 ## Contributing
 
-Contributions to cli-pypi-metadata-extractor are welcome! If you encounter any issues or have suggestions for improvements, please open an issue on the project's GitHub repository.
+Contributions to pymetasnap are welcome! If you encounter any issues or have suggestions for improvements, please open an issue on the project's GitHub repository.
 
 When contributing, please ensure that you follow the existing coding style, write tests for new features, and make sure the tests pass before submitting a pull request.
 
 ## License
 
-cli-pypi-metadata-extractor is licensed under the MIT License. See the LICENSE file for more details.
+pymetasnap is licensed under the MIT License. See the LICENSE file for more details.
 
 ## Acknowledgments
 
-The cli-pypi-metadata-extractor tool builds upon the PyPI API to provide a convenient way to access package metadata. We would like to express our gratitude to the PyPI maintainers and the Python community for their continuous efforts in maintaining and improving the Python Package Index.
+The pymetasnap tool builds upon the PyPI API to provide a convenient way to access package metadata. We would like to express our gratitude to the PyPI maintainers and the Python community for their continuous efforts in maintaining and improving the Python Package Index.
 
 ## Contact
 
 For any inquiries or feedback, please contact the project maintainer at cristian.o.rincon.b@gmail.com.
```

