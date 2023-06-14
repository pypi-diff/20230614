# Comparing `tmp/onto_tool-1.7.2.tar.gz` & `tmp/onto_tool-1.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onto_tool-1.7.2.tar", last modified: Mon Apr 11 21:42:00 2022, max compression
+gzip compressed data, was "onto_tool-1.7.3.tar", last modified: Wed Jun 14 01:37:12 2023, max compression
```

## Comparing `onto_tool-1.7.2.tar` & `onto_tool-1.7.3.tar`

### file list

```diff
@@ -1,39 +1,40 @@
-drwxr-xr-x   0 grahamneiln  (1000) grahamneiln  (1000)        0 2022-04-11 21:42:00.181034 onto_tool-1.7.2/
--rw-r--r--   0 grahamneiln  (1000) grahamneiln  (1000)    32002 2022-04-11 21:42:00.181034 onto_tool-1.7.2/PKG-INFO
--rw-r--r--   0 grahamneiln  (1000) grahamneiln  (1000)    27123 2022-04-01 15:54:04.000000 onto_tool-1.7.2/README.md
-drwxr-xr-x   0 grahamneiln  (1000) grahamneiln  (1000)        0 2022-04-11 21:42:00.181034 onto_tool-1.7.2/onto_tool/
--rw-r--r--   0 grahamneiln  (1000) grahamneiln  (1000)       18 2022-04-11 21:41:23.000000 onto_tool-1.7.2/onto_tool/__init__.py
--rw-r--r--   0 grahamneiln  (1000) grahamneiln  (1000)      105 2022-04-01 15:54:04.000000 onto_tool-1.7.2/onto_tool/__main__.py
--rw-r--r--   0 grahamneiln  (1000) grahamneiln  (1000)    13423 2022-04-01 15:54:04.000000 onto_tool-1.7.2/onto_tool/bundle_schema.yaml
--rw-r--r--   0 grahamneiln  (1000) grahamneiln  (1000)    16023 2022-04-01 15:54:04.000000 onto_tool-1.7.2/onto_tool/command_line.py
--rw-r--r--   0 grahamneiln  (1000) grahamneiln  (1000)     2862 2022-04-01 15:54:04.000000 onto_tool-1.7.2/onto_tool/mdutils.py
--rw-r--r--   0 grahamneiln  (1000) grahamneiln  (1000)    53313 2022-04-01 15:54:04.000000 onto_tool-1.7.2/onto_tool/onto_tool.py
--rw-r--r--   0 grahamneiln  (1000) grahamneiln  (1000)    40027 2022-04-11 21:41:23.000000 onto_tool-1.7.2/onto_tool/ontograph.py
--rw-r--r--   0 grahamneiln  (1000) grahamneiln  (1000)     1235 2022-04-01 15:54:04.000000 onto_tool-1.7.2/onto_tool/sparql_utils.py
-drwxr-xr-x   0 grahamneiln  (1000) grahamneiln  (1000)        0 2022-04-11 21:42:00.181034 onto_tool-1.7.2/onto_tool.egg-info/
--rw-r--r--   0 grahamneiln  (1000) grahamneiln  (1000)    32002 2022-04-11 21:42:00.000000 onto_tool-1.7.2/onto_tool.egg-info/PKG-INFO
--rw-r--r--   0 grahamneiln  (1000) grahamneiln  (1000)      813 2022-04-11 21:42:00.000000 onto_tool-1.7.2/onto_tool.egg-info/SOURCES.txt
--rw-r--r--   0 grahamneiln  (1000) grahamneiln  (1000)        1 2022-04-11 21:42:00.000000 onto_tool-1.7.2/onto_tool.egg-info/dependency_links.txt
--rw-r--r--   0 grahamneiln  (1000) grahamneiln  (1000)       60 2022-04-11 21:42:00.000000 onto_tool-1.7.2/onto_tool.egg-info/entry_points.txt
--rw-r--r--   0 grahamneiln  (1000) grahamneiln  (1000)      131 2022-04-11 21:42:00.000000 onto_tool-1.7.2/onto_tool.egg-info/requires.txt
--rw-r--r--   0 grahamneiln  (1000) grahamneiln  (1000)       16 2022-04-11 21:42:00.000000 onto_tool-1.7.2/onto_tool.egg-info/top_level.txt
--rw-r--r--   0 grahamneiln  (1000) grahamneiln  (1000)       38 2022-04-11 21:42:00.181034 onto_tool-1.7.2/setup.cfg
--rw-r--r--   0 grahamneiln  (1000) grahamneiln  (1000)     1297 2022-04-11 21:38:25.000000 onto_tool-1.7.2/setup.py
-drwxr-xr-x   0 grahamneiln  (1000) grahamneiln  (1000)        0 2022-04-11 21:42:00.181034 onto_tool-1.7.2/tests/
--rw-r--r--   0 grahamneiln  (1000) grahamneiln  (1000)        0 2022-04-01 15:54:04.000000 onto_tool-1.7.2/tests/__init__.py
-drwxr-xr-x   0 grahamneiln  (1000) grahamneiln  (1000)        0 2022-04-11 21:42:00.181034 onto_tool-1.7.2/tests/bundle/
--rw-r--r--   0 grahamneiln  (1000) grahamneiln  (1000)       94 2022-04-01 15:54:04.000000 onto_tool-1.7.2/tests/bundle/__init__.py
--rw-r--r--   0 grahamneiln  (1000) grahamneiln  (1000)      376 2022-04-01 15:54:04.000000 onto_tool-1.7.2/tests/bundle/test_file_ref.py
--rw-r--r--   0 grahamneiln  (1000) grahamneiln  (1000)      563 2022-04-01 15:54:04.000000 onto_tool-1.7.2/tests/bundle/test_logging.py
--rw-r--r--   0 grahamneiln  (1000) grahamneiln  (1000)      356 2022-04-01 15:54:04.000000 onto_tool-1.7.2/tests/bundle/test_message.py
--rw-r--r--   0 grahamneiln  (1000) grahamneiln  (1000)     3676 2022-04-01 15:54:04.000000 onto_tool-1.7.2/tests/bundle/test_sparql.py
--rw-r--r--   0 grahamneiln  (1000) grahamneiln  (1000)      454 2022-04-01 15:54:04.000000 onto_tool-1.7.2/tests/bundle/test_syntax_error.py
--rw-r--r--   0 grahamneiln  (1000) grahamneiln  (1000)     1310 2022-04-01 15:54:04.000000 onto_tool-1.7.2/tests/bundle/test_transform.py
--rw-r--r--   0 grahamneiln  (1000) grahamneiln  (1000)     5148 2022-04-01 15:54:04.000000 onto_tool-1.7.2/tests/bundle/test_verify.py
-drwxr-xr-x   0 grahamneiln  (1000) grahamneiln  (1000)        0 2022-04-11 21:42:00.181034 onto_tool-1.7.2/tests/graphic/
--rw-r--r--   0 grahamneiln  (1000) grahamneiln  (1000)       96 2022-04-01 15:54:04.000000 onto_tool-1.7.2/tests/graphic/__init__.py
--rw-r--r--   0 grahamneiln  (1000) grahamneiln  (1000)     4831 2022-04-01 15:54:04.000000 onto_tool-1.7.2/tests/graphic/test_instance.py
--rw-r--r--   0 grahamneiln  (1000) grahamneiln  (1000)      635 2022-04-01 15:54:04.000000 onto_tool-1.7.2/tests/graphic/test_schema.py
--rw-r--r--   0 grahamneiln  (1000) grahamneiln  (1000)     2566 2022-04-01 15:54:04.000000 onto_tool-1.7.2/tests/test_export.py
--rw-r--r--   0 grahamneiln  (1000) grahamneiln  (1000)     1611 2022-04-01 15:54:04.000000 onto_tool-1.7.2/tests/test_issue-36.py
--rw-r--r--   0 grahamneiln  (1000) grahamneiln  (1000)     1413 2022-04-01 15:54:04.000000 onto_tool-1.7.2/tests/test_update.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 01:37:12.727115 onto_tool-1.7.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11324 2023-06-14 01:36:59.000000 onto_tool-1.7.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    27685 2023-06-14 01:37:12.727115 onto_tool-1.7.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    27123 2023-06-14 01:36:59.000000 onto_tool-1.7.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 01:37:12.723115 onto_tool-1.7.3/onto_tool/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-14 01:36:59.000000 onto_tool-1.7.3/onto_tool/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-14 01:36:59.000000 onto_tool-1.7.3/onto_tool/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13423 2023-06-14 01:36:59.000000 onto_tool-1.7.3/onto_tool/bundle_schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    16023 2023-06-14 01:36:59.000000 onto_tool-1.7.3/onto_tool/command_line.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2862 2023-06-14 01:36:59.000000 onto_tool-1.7.3/onto_tool/mdutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53313 2023-06-14 01:36:59.000000 onto_tool-1.7.3/onto_tool/onto_tool.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40027 2023-06-14 01:36:59.000000 onto_tool-1.7.3/onto_tool/ontograph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-06-14 01:36:59.000000 onto_tool-1.7.3/onto_tool/sparql_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 01:37:12.727115 onto_tool-1.7.3/onto_tool.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    27685 2023-06-14 01:37:12.000000 onto_tool-1.7.3/onto_tool.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-06-14 01:37:12.000000 onto_tool-1.7.3/onto_tool.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 01:37:12.000000 onto_tool-1.7.3/onto_tool.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-14 01:37:12.000000 onto_tool-1.7.3/onto_tool.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-14 01:37:12.000000 onto_tool-1.7.3/onto_tool.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-14 01:37:12.000000 onto_tool-1.7.3/onto_tool.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 01:37:12.727115 onto_tool-1.7.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-06-14 01:36:59.000000 onto_tool-1.7.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 01:37:12.727115 onto_tool-1.7.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 01:36:59.000000 onto_tool-1.7.3/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 01:37:12.727115 onto_tool-1.7.3/tests/bundle/
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-14 01:36:59.000000 onto_tool-1.7.3/tests/bundle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-06-14 01:36:59.000000 onto_tool-1.7.3/tests/bundle/test_file_ref.py
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-06-14 01:36:59.000000 onto_tool-1.7.3/tests/bundle/test_logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-06-14 01:36:59.000000 onto_tool-1.7.3/tests/bundle/test_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3676 2023-06-14 01:36:59.000000 onto_tool-1.7.3/tests/bundle/test_sparql.py
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-06-14 01:36:59.000000 onto_tool-1.7.3/tests/bundle/test_syntax_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-06-14 01:36:59.000000 onto_tool-1.7.3/tests/bundle/test_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5148 2023-06-14 01:36:59.000000 onto_tool-1.7.3/tests/bundle/test_verify.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 01:37:12.727115 onto_tool-1.7.3/tests/graphic/
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-14 01:36:59.000000 onto_tool-1.7.3/tests/graphic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4831 2023-06-14 01:36:59.000000 onto_tool-1.7.3/tests/graphic/test_instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-06-14 01:36:59.000000 onto_tool-1.7.3/tests/graphic/test_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-06-14 01:36:59.000000 onto_tool-1.7.3/tests/test_export.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-06-14 01:36:59.000000 onto_tool-1.7.3/tests/test_issue-36.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-06-14 01:36:59.000000 onto_tool-1.7.3/tests/test_update.py
```

### Comparing `onto_tool-1.7.2/PKG-INFO` & `onto_tool-1.7.3/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,557 +1,541 @@
-Metadata-Version: 2.1
-Name: onto_tool
-Version: 1.7.2
-Summary: Ontology Maintenance and Release Tool
-Home-page: https://github.com/semanticarts/ontology-toolkit
-Author: Boris Pelakh
-Author-email: boris.pelakh@semanticarts.com
-License: UNKNOWN
-Description: # ontology-toolkit
-        
-        Maintain version and dependency info in RDF ontologies.
-        
-        ## Installation
-        
-        ## Easy Install 
-        
-        To install the most recent released version of the toolkit use `pip install onto-tool`. 
-        
-        ## Development Install
-        
-        To experiment with unreleased features currently in development, clone this repo and navigate to the installed directory.  Run `python -m setup install`, which
-        will install the `onto_tool` command and all its dependencies into your environment.
-        
-        ```
-        $ onto_tool -h
-        usage: onto_tool [-h] [-k] [-v] {update,export,bundle,graphic} ...
-        
-        Ontology toolkit.
-        
-        positional arguments:
-          {update,export,bundle,graphic}
-                                sub-command help
-            update              Update versions and dependencies
-            export              Export ontology
-            bundle              Bundle ontology for release
-            graphic             Create PNG graphic and dot file from OWL files or SPARQL Endpoint
-        
-        optional arguments:
-          -h, --help            show this help message and exit
-          -k, --insecure        Allow insecure server connections when using SSL
-          -v, --version         Report onto-tool version and exit
-        ```
-        
-        ## Sub-Commands
-        
-        ### Update
-        
-        The `update` sub-command modifies ontology version and dependency information
-        ```
-        $ onto_tool update -h
-        usage: onto_tool update [-h] [-f {xml,turtle,nt} | -i] [--debug] [-o OUTPUT]
-                                [-b [{all,strict}]] [--retain-definedBy]
-                                [--versioned-definedBy] [-v SET_VERSION]
-                                [--version-info [VERSION_INFO]]
-                                [-d DEPENDENCY VERSION]
-                                [ontology [ontology ...]]
-        
-        positional arguments:
-          ontology              Ontology file or directory containing OWL files
-        
-        optional arguments:
-          -h, --help            show this help message and exit
-          -f {xml,turtle,nt}, --format {xml,turtle,nt}
-                                Output format
-          -i, --in-place        Overwrite each input file with update, preserving
-                                format
-          --debug               Emit verbose debug output
-          -o OUTPUT, --output OUTPUT
-                                Path to output file. Will be ignored if --in-place is
-                                specified.
-          -b [{all,strict}], --defined-by [{all,strict}]
-                                Add rdfs:isDefinedBy to every resource defined. If the
-                                (default) "strict" argument is provided, only
-                                owl:Class, owl:ObjectProperty, owl:DatatypeProperty,
-                                owl:AnnotationProperty and owl:Thing entities will be
-                                annotated. If "all" is provided, every entity that has
-                                any properties other than rdf:type will be annotated.
-                                Will override any existing rdfs:isDefinedBy
-                                annotations on the affected entities unless --retain-
-                                definedBy is specified.
-          -v SET_VERSION, --set-version SET_VERSION
-                                Set the version of the defined ontology
-          --version-info [VERSION_INFO]
-                                Adjust versionInfo, defaults to "Version X.x.x"
-          -d DEPENDENCY VERSION, --dependency-version DEPENDENCY VERSION
-                                Update the import of DEPENDENCY to VERSION
-        ```
-        
-        ### Export
-        
-        The `export` sub-command will transform the ontology into the desired format, and remove version information, as required by tools such as Top Braid Composer.
-        ```
-        usage: onto_tool export [-h] [-f {xml,turtle,nt} | -c CONTEXT] [--debug]
-                                [-o OUTPUT] [-s] [-m IRI VERSION] [-b [{all,strict}]]
-                                [--retain-definedBy] [--versioned-definedBy]
-                                [ontology [ontology ...]]
-        
-        positional arguments:
-          ontology              Ontology file or directory containing OWL files
-        
-        optional arguments:
-          -h, --help            show this help message and exit
-          -f {xml,turtle,nt}, --format {xml,turtle,nt}
-                                Output format
-          -c CONTEXT, --context CONTEXT
-                                Export as N-Quads in CONTEXT.
-          --debug               Emit verbose debug output
-          -o OUTPUT, --output OUTPUT
-                                Path to output file.
-          -s, --strip-versions  Remove versions from imports.
-          -m IRI VERSION, --merge IRI VERSION
-                                Merge all inputs into a single ontology with the given
-                                IRI and version
-          -b [{all,strict}], --defined-by [{all,strict}]
-                                Add rdfs:isDefinedBy to every resource defined. If the
-                                (default) "strict" argument is provided, only
-                                owl:Class, owl:ObjectProperty, owl:DatatypeProperty,
-                                owl:AnnotationProperty and owl:Thing entities will be
-                                annotated. If "all" is provided, every entity that has
-                                any properties other than rdf:type will be annotated.
-          --retain-definedBy    When merging ontologies, retain existing values of
-                                rdfs:isDefinedBy
-        ```
-        
-        ### Graphic
-        
-        The `graphic` sub-command will create either 
-        * a comprehensive diagram showing ontology modules together with classes, object properties and individuals
-          together with the path of imports, or (if the 'wee' option is selected) a simple diagram of the ontology
-          import hierarchy, or
-        * a diagram of the use of classes and object and data properties in a triple store or local ontology files.
-            
-        Graphics are exported both as ```png``` files and also as a ```dot``` file.  This ```dot``` file can be used with Graphviz or with web tools such as [Dot Viewer](http://www.semantechs.co.uk/turtle-editor-viewer/)
-        
-        ```
-        usage: onto_tool graphic [-h] [-e ENDPOINT] [--schema | --data]
-                                 [--single-ontology-graphs] [--debug] [-o OUTPUT]
-                                 [--show-shacl]
-                                 [--link-concentrator-threshold LINK_CONCENTRATOR_THRESHOLD]
-                                 [--instance-limit INSTANCE_LIMIT]
-                                 [--predicate-threshold PREDICATE_THRESHOLD]
-                                 [--include [INCLUDE [INCLUDE ...]] |
-                                 --include-pattern [INCLUDE_REGEX [INCLUDE_REGEX ...]]
-                                 | --exclude [EXCLUDE [EXCLUDE ...]] |
-                                 --exclude-pattern
-                                 [EXCLUDE_REGEX [EXCLUDE_REGEX ...]]] [-v VERSION]
-                                 [-w [WEE [WEE ...]]]
-                                 [--label-language LABEL_LANGUAGE]
-                                 [--hide [HIDE [HIDE ...]]] [--no-image] [-t TITLE]
-                                 [ontology [ontology ...]]
-        
-        positional arguments:
-          ontology              Ontology file, directory or name pattern
-        
-        optional arguments:
-          -h, --help            show this help message and exit
-          -e ENDPOINT, --endpoint ENDPOINT
-                                URI of SPARQL endpoint to use to gather data
-          --schema              Generate ontology import graph (default)
-          --data                Analyze instances for types and links
-          --single-ontology-graphs
-                                If specified in combination with --endpoint when
-                                generating a schema graph, assume that every ontology
-                                is in its own named graph in the triple store.
-                                Otherwise rdfs:isDefinedBy will be used to locate
-                                entities defined by each ontology.
-          --debug               Emit verbose debug output
-          -o OUTPUT, --output OUTPUT
-                                Output directory for generated graphics
-          --show-shacl          Attempts to discover which classes and properties have
-                                corresponding SHACL shapes and colors them green on
-                                the graph. This detection relies on the presence of
-                                sh:targetClass targeting, and can be confused by
-                                complex logical shapes or Advanced SHACL features such
-                                as SPARQL queries.
-          --link-concentrator-threshold LINK_CONCENTRATOR_THRESHOLD
-                                When the number links originating from the same class
-                                that share a single predicate exceed this threshold
-                                (default 10), use more compact display. Setting the
-                                value to 0 disables this behavior.
-          -v VERSION, --version VERSION
-                                Version to place in graphic
-          -w [WEE [WEE ...]], --wee [WEE [WEE ...]]
-                                For ontologies matching the patterns specified, only
-                                render the name and import information. If no patterns
-                                are specified, applies to all ontologies.
-          --label-language LABEL_LANGUAGE
-                                In case entities have labels in multiple languages,
-                                select either the specified language (default: en) or
-                                a non-lanugage label.
-          --hide [HIDE [HIDE ...]]
-                                When visualizing data, hide classes and properties
-                                matching the regexpatterns specified with this option.
-          --no-image            Do not generate PNG image, only .dot output.
-          -t TITLE, --title TITLE
-                                Title to use for graph. If not supplied, the repo URI
-                                will be used if graphing an endpoint, or 'Gist' if
-                                graphing local files.
-        
-        Sampling Limits:
-          --instance-limit INSTANCE_LIMIT
-                                Specify a limit on how many triples to consider that
-                                use any one predicate to find (default 500000). This
-                                option may result in an incomplete version of the
-                                diagram, missing certain links.
-          --predicate-threshold PREDICATE_THRESHOLD
-                                Ignore predicates which occur fewer than
-                                PREDICATE_THRESHOLD times (default 10)
-        
-        Filters (only one can be used):
-          --include [INCLUDE [INCLUDE ...]]
-                                If specified for --schema, only ontologies matching
-                                the specified URIs will be shown in full detail. If
-                                specified with --data, only triples in the named
-                                graphs mentioned will be considered (this also
-                                excludes any triples in the default graph).
-          --include-pattern [INCLUDE_REGEX [INCLUDE_REGEX ...]]
-                                If specified for --schema, only ontologies matching
-                                the specified URI pattern will be shown in full
-                                detail. If specified with --data, only triples in the
-                                named graphs matching the pattern will be considered
-                                (this also excludes any triples in the default graph).
-                                For large graphs this option is significantly slower
-                                than using --include.
-          --exclude [EXCLUDE [EXCLUDE ...]]
-                                If specified for --schema, ontologies matching the
-                                specified URIs will be omitted from the graph. If
-                                specified with --data, triples in the named graphs
-                                mentioned will be excluded (this also excludes any
-                                triples in the default graph).
-          --exclude-pattern [EXCLUDE_REGEX [EXCLUDE_REGEX ...]]
-                                If specified for --schema, ontologies matching the
-                                specified URI pattern will be omitted from the graph.
-                                If specified with --data, triples in the named graphs
-                                matching the pattern will be ignored (this also
-                                excludes any triples in the default graph). For large
-                                graphs this option is significantly slower than using
-                                --exclude.
-        ```
-        
-        ### Bundle
-        
-        The `bundle` sub-command supports creating an ontology deployment containing both RDF and non-RDF artifacts for delivery or web hosting.
-        
-        ```
-        $ onto_tool bundle -h
-        usage: onto_tool bundle [-h] [--debug] [-v VARIABLE VALUE] bundle
-        
-        positional arguments:
-          bundle                JSON or YAML bundle definition
-        
-        optional arguments:
-          -h, --help            show this help message and exit
-          --debug               Emit verbose debug output
-          -v VARIABLE VALUE, --variable VARIABLE VALUE
-                                Set value of VARIABLE to VALUE
-        ```
-        
-        The bundle definition is either YAML or JSON, and contains the following sections:
-        
-        #### Variable definition
-        
-        ```yaml
-        variables:
-          name: "gist"
-          version: "X.x.x"
-          input: "."
-          rdf-toolkit: "{input}/tools/rdf-toolkit.jar"
-          output: "{name}{version}_webDownload"
-        ```
-        Variables are initialized with the default values provided, but can be overriden via the `--variable` command line option.
-        Values can reference other values using the `{name}` template syntax.
-        
-        #### Tool definition
-        
-        All tools require a `name` by which they are referenced in `transform` actions. Three different tool types are supported:
-        * Java tools (`type: "Java"`) require a path to the executable Jar file specified via the `jar` option,
-          and a list of `arguments` that will be applied to each file processed.
-          The `inputFile` and `outputFile` variables will be bound during execution, but other variables can be
-          used to construct the arguments.
-          tools:
-          ```yaml
-          - name: "serializer"
-            type: "Java"
-            jar: "{rdf-toolkit}"
-            arguments:
-              - "-tfmt"
-              - "rdf-xml"
-              - "-sdt"
-              - "explicit"
-              - "-dtd"
-              - "-ibn"
-              - "-s"
-              - "{inputFile}"
-              - "-t"
-              - "{outputFile}"
-          ```
-        * Shell tools (`type: "shell"`) execute a command specified via
-          a list of `arguments` that will be applied to each file processed.
-          The `inputFile` and `outputFile` variables will be bound during execution, but other variables can be
-          used to construct the arguments.
-          tools:
-          ```yaml
-            tools:
-            - name: "java_version"
-              type: "shell"
-              arguments:
-                - "java"
-                - "-version"
-          ```
-        * SPARQL tools apply a SPARQL Update query to each input file and serialize the resulting graph into the 
-          output file. RDF format is preserved unless overridden with the `format` option. If the query is specified
-          inline, template substitution will be applied to it, so bundle variables can be used, but double braces
-          (`{{` instead of `{`, `}}` instead of `}`) have to be used to escape actual braces.
-          ```yaml
-            - name: "add-language-en"
-              type: "sparql"
-              query: >
-                prefix skos: <http://www.w3.org/2004/02/skos/core#>
-                DELETE {{
-                  ?subject skos:prefLabel ?nolang .
-                }}
-                INSERT {{
-                  ?subject skos:prefLabel ?withlang
-                }}
-                where {{
-                  ?subject skos:prefLabel ?nolang .
-                  FILTER(lang(?nolang) = '')
-                  BIND(STRLANG(?nolang, '{lang}') as ?withlang)
-                }}
-          ```
-        
-        #### Actions
-        
-        Actions are executed in the order they are listed. Each action must have an `action` attribute,
-        and any action can contain a `message` attribute, the contents of which will be
-        emitted as a `INFO`-level log message prior to the execution of the action.
-        
-        ##### Basic File Manipulation
-        - `mkdir`, which requires a `directory` attribute to specify the path of the directory to be created 
-          (only if it doesn't already exist)
-        - `copy`, which copies files into the bundle, and supports the following arguments:
-          - `source`, `target` and `includes` - if `includes` is not present, `source` and `target` are both
-            assumed to be file paths to a single file. If `includes` is provided, `source` and `target` are 
-            assumed to be directories, and each member of the `includes` list a glob pattern inside the
-            `source` directory.
-          - `rename` - If provided, must contain `from` and `to` attributes. When specified, each file
-            is renamed as it is copied, where `from` is treated as a Python regular expression
-            applied to the base name of the source file, and `to` is the substitution string which
-            replaces it in the name of the target file. Backreferences are available for capturing groups, e.g.
-            ```yaml
-              rename:
-                from: "(.*)\\.owl"
-                to: "\\g<1>{version}.owl"
-            ```
-            will add a version number to the base name of each `.owl` file. Further documentation on
-            Python regular expression replace functionality can be found
-            [here](https://docs.python.org/3/howto/regex.html#search-and-replace).
-          - `replace` - If provided, must contain `from` and `to` attributes. When specified, each file
-            is processed after being copied, and each instance of the `from` pattern is replaced
-            with `to` string in the file contents. Python regular expression syntax and backreferences are
-            supported as shown in the `rename` documentation.
-        - `move`, which moves files according the provided options, which are identical to the ones supported
-          by `copy`.
-          
-        ##### RDF Transformation
-        
-        - `definedBy`, which inspects each input file to identify a single defined ontology, and then
-          adds a `rdfs:isDefinedBy` property to every `owl:Class`, `owl:ObjectProperty`, `owl:DatatypeProperty`
-          and `owl:AnnotationProperty` defined in the file referencing the identified ontology. Existing
-          `rdfs:isDefinedBy` values are removed prior to the addition. Input and output file specification
-          options are identical to those used by the `copy` action.
-        - `export`, which functions similarly to the command-line export functionality, gathering one or
-          more input ontologies and exporting them as a single file, with some optional transformations,
-          depending on the following specified options:
-          - `source`, `target` and `includes` - if `includes` is not present, `source` is
-            assumed to be the path to a single file. If `includes` is provided, `source` is 
-            assumed to be a directory, and each member of the `includes` list a glob pattern inside the
-            `source` directory. `target` is always treated as a single file path.
-          - `merge` - if provided, it must have two mandatory fields, `iri` and `version`. In this case, all
-            ontologies declared in the input files are removed, and a single new ontologies, specified by the 
-            `iri` is created, using `version` to build `owl:versionInfo` and `owl:versionIRI`. Any imports on
-            the removed ontologies which are not satisfied internally are transferred to the new ontology.
-          - `definedBy` - has two possible values, `strict` and `all`. If provided, a `rdfs:isDefinedBy` is
-            added to all non-blank node subjects in the exported RDF linking them to the ontology defined in the
-            combined graph. If more that one ontology is defined, the export will fail. If `strict` is specified,
-            only classes and properties will be annotated, whereas `all` does not filter by type.
-          - `retainDefinedBy` - by default, `definedBy` will override any existing `rdfs:definedBy` annotations,
-            but if this option is provided, existing annotations will be left in place.
-          - `format` - One of `turtle`, `xml`, or `nt` (N-Triples), specifies the output format for the export.
-            The default output format is `turtle`.
-          - `context` - If provided, generates a N-Quads export with the `context` argument as the name of the
-            graph. When this option is present, the value of `format` is ignored.
-          - `compress` - when this is `true`, the output is `gzip`-ed.
-        - `transform`, which applies the specified tool to a set of input files, and supports the following
-          arguments:
-          - `tool`, which references the `name` of a tool which must be defined in the `tools` section.
-          - `source`, `target` and `includes`, which function just like they do for the `copy` and `move`
-            actions, with each input and output path bound into the `inputFile` and `outputFile` variables
-            before the tool arguments are interpreted.
-          - `replace` and `rename`, which are applied after the tool invocation, and work as described above.
-        - `sparql` reads RDF files provided via the `source` and `includes` options and executes a SPARQL
-          query on the resulting combined graph.
-            * If the `query` option is a valid file path, the query is read from that file,
-              otherwise the contents of the `query` option are interpreted as the query.
-            * `SELECT` query results are stored in the file specified via `target` as a CSV.
-            * RDF results from a `CONSTRUCT` query are
-          stored as either Turtle, RDF/XML or N-Triples, depending on the `format` option (`turtle`, `xml`, or `nt`).
-              Update queries will alter the input data in place, and the resulting
-              graph will be output in the specified format.
-            * `UPDATE` queries executed on local files will modify the in-memory graph and then serialize the
-              resulting graph to the `target`.
-            * The default functionality is to combine all RDF sources specified via `includes`
-              and execute queries on the resulting graph. However, if `eachFile: true` is added,
-              all queries will be applied to each source file separately, and will produce a 
-              separate output file. In this case, `target` will be treated as a directory, and
-              the `rename` option should be used when needed to construct the output file names. For example, the following
-              action extracts the labels out of each RDF file into a separate CSV with matching names:
-              ```yaml
-              - action: 'sparql'
-                message: "Multi-file processing with SELECT"
-                eachFile: true
-                source: '{input}'
-                includes:
-                  - '*_ontology.ttl'
-                target: "{output}/each/select"
-                rename:
-                  from: "(.*)\\.ttl"
-                  to: "\\g<1>.csv"
-                query: >
-                  prefix rdfs: <http://www.w3.org/2000/01/rdf-schema#>
-                  prefix skos: <http://www.w3.org/2004/02/skos/core#>
-                  select ?label
-                  WHERE {{
-                    ?s rdfs:label ?label .
-                  }} order by ?label
-              ```
-            * As an alternative to operating on local RDF specified via 'source', a query can
-              be executed on a triple store by specifying an `endpoint`, which must
-              contain a `query_uri`, and can optionally specify `user`/`password` which will
-              authenticate via HTTP basic authentication. Update queries will modify the
-              triple store directly, and a separate `update_uri` can be specified
-              for databases which require it.
-        
-          
-        ##### Utility Actions
-        - `markdown` transforms a `.md` file referenced in `source` into an HTML output specified in `target`.
-        - `graph` reads RDF files provided via the `source` and `includes` options and generates a graphical
-          representation of the ontology, as in the `graphic` sub-command described above. Both `.dot` and
-          `.png` outputs are written to the directory specified in the `target` option, and `title` and 
-          `version` attributes configure the title on the generated graph. If `compact` is specified as
-          `True`, a concise graph including only ontology names and imports is generated.
-        
-        ##### Validation
-        The `verify` action reads RDF files provided via the `source` and `includes` options and performs validation on the
-        resulting combined graph. If the validation fails, the bundle process exits with a non-zero status and
-        does not execute subsequent actions. The type of verification performed depends on the 
-        value of the `type` option:
-        * If `type` is `select`, one or more SPARQL `SELECT` queries are executed against the graph, and the
-          first query to return a non-empty result will terminate the bundle. The results of the query will
-          be output to the log, and also written as CSV to a file path specified by the `target` option, if
-          provided. Queries can be specified in one of two ways (only one can be present):
-          * If the `query` option is a valid file path, the query is read from that file,
-            otherwise the contents of the `query` option are interpreted as the query, e.g.
-            ```yaml
-            query: >
-              prefix skos: <http://www.w3.org/2004/02/skos/core#>
-              select ?unlabeled where {{
-                ?unlabeled a ?type .
-                filter not exists {{ ?unlabeled skos:prefLabel ?label }}
-              }}
-            ```
-          * If `queries` is provided, a list of queries will be built from the `source` and `includes`
-            sub-options. The queries will be executed in order specified. If `stopOnFail` is omitted or
-            is `true`, the first  query that produces a failing result will cause `verify` to abort. If
-            `stopOnFail` is `false`, all queries will be executed regardless of failures, and the value
-            of `target` is treated as a directory where the results of _each_ failing query will be written.
-            ```yaml
-              - action: 'verify'
-                type: 'select'
-                source: '{input}'
-                includes:
-                  - 'verify_data.ttl'
-                target: '{output}/verify_select_results'
-                stopOnFail: false
-                queries:
-                  source: '{input}'
-                  includes:
-                    - 'verify_*_select_query.rq'
-            ```
-        * If `type` is `ask`, one or more SPARQL `ASK` queries will be executed. Queries are
-          specified similarly to the `select` validation. Unless `stopOnFail` is set to `false`, the first
-          query producing a result that does not match the required `expected` option, the bundle will terminate.
-          For example:
-          ```yaml
-          actions:
-            - action: 'verify'
-              type: 'ask'
-              source: '{input}'
-              includes:
-                - 'verify_data.ttl'
-              queries:
-                source: '{input}'
-                includes:
-                  - '*_ask_query.rq'
-              expected: false
-          ```
-        * If `type` is `shacl`, a SHACL shape graph will be constructed from the file specified via the `shapes`
-          option (which must have a `source`, and optionally `includes`), with the bundle terminating only if
-          any `sh:Violation` results are present, unless the `failOn` option specifies otherwise.`
-          The report is emitted to the log, and saved as Turtle to the path specified in the `target` option if it's provided.
-          For example:
-          ```yaml
-          - action: 'verify'
-            type: 'shacl'
-            inference: 'rdfs'
-            source: '{input}'
-            includes:
-              - 'verify_data.ttl'
-            target: '{output}/verify_shacl_errors.ttl'
-            failOn: "warning"
-            shapes:
-              source: '{input}/verify_shacl_shapes.ttl'
-          ```
-          If the `inference` option is provided, the reasoner will be run on the graph prior
-          to applying the SHACL rules. The valid values are:
-            * `rdfs`,
-            * `owlrl`,
-            * `both`, or
-            * `none` (default).
-        * If `type` is `construct`, the queries are expected to `CONSTRUCT` a [SHACL ValidationReport](https://www.w3.org/TR/shacl/#validation-report).
-          The validation will be considered as a failure if the resulting graph is non-empty. `target`,
-          `stopOnFail` and `query`/`queries` are handled same as `select` validation, and `failOn` is used to determine which
-          violations will terminate execution.
-        * Validation can be performed against a SPARQL endpoint instead of local RDF
-          data by specifying `endpoint` instead of `source`/`includes`. `endpoint` must
-          contain a `query_uri`, and can optionally specify `user`/`password` which will
-          authenticate via HTTP basic authentication. For example:
-          ```
-          - action: 'verify'
-            type: 'construct'
-            endpoint:
-              query_uri: 'https://my.endpoint.com/sparql'
-              user: 'test-user'
-              password: 'test-user'
-            target: '{output}/verify_construct_results'
-            stopOnFail: false
-            query: '{input}/verify_via_construct.rq'
-          ```
-        
-Platform: UNKNOWN
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
+# ontology-toolkit
+
+Maintain version and dependency info in RDF ontologies.
+
+## Installation
+
+## Easy Install 
+
+To install the most recent released version of the toolkit use `pip install onto-tool`. 
+
+## Development Install
+
+To experiment with unreleased features currently in development, clone this repo and navigate to the installed directory.  Run `python -m setup install`, which
+will install the `onto_tool` command and all its dependencies into your environment.
+
+```
+$ onto_tool -h
+usage: onto_tool [-h] [-k] [-v] {update,export,bundle,graphic} ...
+
+Ontology toolkit.
+
+positional arguments:
+  {update,export,bundle,graphic}
+                        sub-command help
+    update              Update versions and dependencies
+    export              Export ontology
+    bundle              Bundle ontology for release
+    graphic             Create PNG graphic and dot file from OWL files or SPARQL Endpoint
+
+optional arguments:
+  -h, --help            show this help message and exit
+  -k, --insecure        Allow insecure server connections when using SSL
+  -v, --version         Report onto-tool version and exit
+```
+
+## Sub-Commands
+
+### Update
+
+The `update` sub-command modifies ontology version and dependency information
+```
+$ onto_tool update -h
+usage: onto_tool update [-h] [-f {xml,turtle,nt} | -i] [--debug] [-o OUTPUT]
+                        [-b [{all,strict}]] [--retain-definedBy]
+                        [--versioned-definedBy] [-v SET_VERSION]
+                        [--version-info [VERSION_INFO]]
+                        [-d DEPENDENCY VERSION]
+                        [ontology [ontology ...]]
+
+positional arguments:
+  ontology              Ontology file or directory containing OWL files
+
+optional arguments:
+  -h, --help            show this help message and exit
+  -f {xml,turtle,nt}, --format {xml,turtle,nt}
+                        Output format
+  -i, --in-place        Overwrite each input file with update, preserving
+                        format
+  --debug               Emit verbose debug output
+  -o OUTPUT, --output OUTPUT
+                        Path to output file. Will be ignored if --in-place is
+                        specified.
+  -b [{all,strict}], --defined-by [{all,strict}]
+                        Add rdfs:isDefinedBy to every resource defined. If the
+                        (default) "strict" argument is provided, only
+                        owl:Class, owl:ObjectProperty, owl:DatatypeProperty,
+                        owl:AnnotationProperty and owl:Thing entities will be
+                        annotated. If "all" is provided, every entity that has
+                        any properties other than rdf:type will be annotated.
+                        Will override any existing rdfs:isDefinedBy
+                        annotations on the affected entities unless --retain-
+                        definedBy is specified.
+  -v SET_VERSION, --set-version SET_VERSION
+                        Set the version of the defined ontology
+  --version-info [VERSION_INFO]
+                        Adjust versionInfo, defaults to "Version X.x.x"
+  -d DEPENDENCY VERSION, --dependency-version DEPENDENCY VERSION
+                        Update the import of DEPENDENCY to VERSION
+```
+
+### Export
+
+The `export` sub-command will transform the ontology into the desired format, and remove version information, as required by tools such as Top Braid Composer.
+```
+usage: onto_tool export [-h] [-f {xml,turtle,nt} | -c CONTEXT] [--debug]
+                        [-o OUTPUT] [-s] [-m IRI VERSION] [-b [{all,strict}]]
+                        [--retain-definedBy] [--versioned-definedBy]
+                        [ontology [ontology ...]]
+
+positional arguments:
+  ontology              Ontology file or directory containing OWL files
+
+optional arguments:
+  -h, --help            show this help message and exit
+  -f {xml,turtle,nt}, --format {xml,turtle,nt}
+                        Output format
+  -c CONTEXT, --context CONTEXT
+                        Export as N-Quads in CONTEXT.
+  --debug               Emit verbose debug output
+  -o OUTPUT, --output OUTPUT
+                        Path to output file.
+  -s, --strip-versions  Remove versions from imports.
+  -m IRI VERSION, --merge IRI VERSION
+                        Merge all inputs into a single ontology with the given
+                        IRI and version
+  -b [{all,strict}], --defined-by [{all,strict}]
+                        Add rdfs:isDefinedBy to every resource defined. If the
+                        (default) "strict" argument is provided, only
+                        owl:Class, owl:ObjectProperty, owl:DatatypeProperty,
+                        owl:AnnotationProperty and owl:Thing entities will be
+                        annotated. If "all" is provided, every entity that has
+                        any properties other than rdf:type will be annotated.
+  --retain-definedBy    When merging ontologies, retain existing values of
+                        rdfs:isDefinedBy
+```
+
+### Graphic
+
+The `graphic` sub-command will create either 
+* a comprehensive diagram showing ontology modules together with classes, object properties and individuals
+  together with the path of imports, or (if the 'wee' option is selected) a simple diagram of the ontology
+  import hierarchy, or
+* a diagram of the use of classes and object and data properties in a triple store or local ontology files.
+    
+Graphics are exported both as ```png``` files and also as a ```dot``` file.  This ```dot``` file can be used with Graphviz or with web tools such as [Dot Viewer](http://www.semantechs.co.uk/turtle-editor-viewer/)
+
+```
+usage: onto_tool graphic [-h] [-e ENDPOINT] [--schema | --data]
+                         [--single-ontology-graphs] [--debug] [-o OUTPUT]
+                         [--show-shacl]
+                         [--link-concentrator-threshold LINK_CONCENTRATOR_THRESHOLD]
+                         [--instance-limit INSTANCE_LIMIT]
+                         [--predicate-threshold PREDICATE_THRESHOLD]
+                         [--include [INCLUDE [INCLUDE ...]] |
+                         --include-pattern [INCLUDE_REGEX [INCLUDE_REGEX ...]]
+                         | --exclude [EXCLUDE [EXCLUDE ...]] |
+                         --exclude-pattern
+                         [EXCLUDE_REGEX [EXCLUDE_REGEX ...]]] [-v VERSION]
+                         [-w [WEE [WEE ...]]]
+                         [--label-language LABEL_LANGUAGE]
+                         [--hide [HIDE [HIDE ...]]] [--no-image] [-t TITLE]
+                         [ontology [ontology ...]]
+
+positional arguments:
+  ontology              Ontology file, directory or name pattern
+
+optional arguments:
+  -h, --help            show this help message and exit
+  -e ENDPOINT, --endpoint ENDPOINT
+                        URI of SPARQL endpoint to use to gather data
+  --schema              Generate ontology import graph (default)
+  --data                Analyze instances for types and links
+  --single-ontology-graphs
+                        If specified in combination with --endpoint when
+                        generating a schema graph, assume that every ontology
+                        is in its own named graph in the triple store.
+                        Otherwise rdfs:isDefinedBy will be used to locate
+                        entities defined by each ontology.
+  --debug               Emit verbose debug output
+  -o OUTPUT, --output OUTPUT
+                        Output directory for generated graphics
+  --show-shacl          Attempts to discover which classes and properties have
+                        corresponding SHACL shapes and colors them green on
+                        the graph. This detection relies on the presence of
+                        sh:targetClass targeting, and can be confused by
+                        complex logical shapes or Advanced SHACL features such
+                        as SPARQL queries.
+  --link-concentrator-threshold LINK_CONCENTRATOR_THRESHOLD
+                        When the number links originating from the same class
+                        that share a single predicate exceed this threshold
+                        (default 10), use more compact display. Setting the
+                        value to 0 disables this behavior.
+  -v VERSION, --version VERSION
+                        Version to place in graphic
+  -w [WEE [WEE ...]], --wee [WEE [WEE ...]]
+                        For ontologies matching the patterns specified, only
+                        render the name and import information. If no patterns
+                        are specified, applies to all ontologies.
+  --label-language LABEL_LANGUAGE
+                        In case entities have labels in multiple languages,
+                        select either the specified language (default: en) or
+                        a non-lanugage label.
+  --hide [HIDE [HIDE ...]]
+                        When visualizing data, hide classes and properties
+                        matching the regexpatterns specified with this option.
+  --no-image            Do not generate PNG image, only .dot output.
+  -t TITLE, --title TITLE
+                        Title to use for graph. If not supplied, the repo URI
+                        will be used if graphing an endpoint, or 'Gist' if
+                        graphing local files.
+
+Sampling Limits:
+  --instance-limit INSTANCE_LIMIT
+                        Specify a limit on how many triples to consider that
+                        use any one predicate to find (default 500000). This
+                        option may result in an incomplete version of the
+                        diagram, missing certain links.
+  --predicate-threshold PREDICATE_THRESHOLD
+                        Ignore predicates which occur fewer than
+                        PREDICATE_THRESHOLD times (default 10)
+
+Filters (only one can be used):
+  --include [INCLUDE [INCLUDE ...]]
+                        If specified for --schema, only ontologies matching
+                        the specified URIs will be shown in full detail. If
+                        specified with --data, only triples in the named
+                        graphs mentioned will be considered (this also
+                        excludes any triples in the default graph).
+  --include-pattern [INCLUDE_REGEX [INCLUDE_REGEX ...]]
+                        If specified for --schema, only ontologies matching
+                        the specified URI pattern will be shown in full
+                        detail. If specified with --data, only triples in the
+                        named graphs matching the pattern will be considered
+                        (this also excludes any triples in the default graph).
+                        For large graphs this option is significantly slower
+                        than using --include.
+  --exclude [EXCLUDE [EXCLUDE ...]]
+                        If specified for --schema, ontologies matching the
+                        specified URIs will be omitted from the graph. If
+                        specified with --data, triples in the named graphs
+                        mentioned will be excluded (this also excludes any
+                        triples in the default graph).
+  --exclude-pattern [EXCLUDE_REGEX [EXCLUDE_REGEX ...]]
+                        If specified for --schema, ontologies matching the
+                        specified URI pattern will be omitted from the graph.
+                        If specified with --data, triples in the named graphs
+                        matching the pattern will be ignored (this also
+                        excludes any triples in the default graph). For large
+                        graphs this option is significantly slower than using
+                        --exclude.
+```
+
+### Bundle
+
+The `bundle` sub-command supports creating an ontology deployment containing both RDF and non-RDF artifacts for delivery or web hosting.
+
+```
+$ onto_tool bundle -h
+usage: onto_tool bundle [-h] [--debug] [-v VARIABLE VALUE] bundle
+
+positional arguments:
+  bundle                JSON or YAML bundle definition
+
+optional arguments:
+  -h, --help            show this help message and exit
+  --debug               Emit verbose debug output
+  -v VARIABLE VALUE, --variable VARIABLE VALUE
+                        Set value of VARIABLE to VALUE
+```
+
+The bundle definition is either YAML or JSON, and contains the following sections:
+
+#### Variable definition
+
+```yaml
+variables:
+  name: "gist"
+  version: "X.x.x"
+  input: "."
+  rdf-toolkit: "{input}/tools/rdf-toolkit.jar"
+  output: "{name}{version}_webDownload"
+```
+Variables are initialized with the default values provided, but can be overriden via the `--variable` command line option.
+Values can reference other values using the `{name}` template syntax.
+
+#### Tool definition
+
+All tools require a `name` by which they are referenced in `transform` actions. Three different tool types are supported:
+* Java tools (`type: "Java"`) require a path to the executable Jar file specified via the `jar` option,
+  and a list of `arguments` that will be applied to each file processed.
+  The `inputFile` and `outputFile` variables will be bound during execution, but other variables can be
+  used to construct the arguments.
+  tools:
+  ```yaml
+  - name: "serializer"
+    type: "Java"
+    jar: "{rdf-toolkit}"
+    arguments:
+      - "-tfmt"
+      - "rdf-xml"
+      - "-sdt"
+      - "explicit"
+      - "-dtd"
+      - "-ibn"
+      - "-s"
+      - "{inputFile}"
+      - "-t"
+      - "{outputFile}"
+  ```
+* Shell tools (`type: "shell"`) execute a command specified via
+  a list of `arguments` that will be applied to each file processed.
+  The `inputFile` and `outputFile` variables will be bound during execution, but other variables can be
+  used to construct the arguments.
+  tools:
+  ```yaml
+    tools:
+    - name: "java_version"
+      type: "shell"
+      arguments:
+        - "java"
+        - "-version"
+  ```
+* SPARQL tools apply a SPARQL Update query to each input file and serialize the resulting graph into the 
+  output file. RDF format is preserved unless overridden with the `format` option. If the query is specified
+  inline, template substitution will be applied to it, so bundle variables can be used, but double braces
+  (`{{` instead of `{`, `}}` instead of `}`) have to be used to escape actual braces.
+  ```yaml
+    - name: "add-language-en"
+      type: "sparql"
+      query: >
+        prefix skos: <http://www.w3.org/2004/02/skos/core#>
+        DELETE {{
+          ?subject skos:prefLabel ?nolang .
+        }}
+        INSERT {{
+          ?subject skos:prefLabel ?withlang
+        }}
+        where {{
+          ?subject skos:prefLabel ?nolang .
+          FILTER(lang(?nolang) = '')
+          BIND(STRLANG(?nolang, '{lang}') as ?withlang)
+        }}
+  ```
+
+#### Actions
+
+Actions are executed in the order they are listed. Each action must have an `action` attribute,
+and any action can contain a `message` attribute, the contents of which will be
+emitted as a `INFO`-level log message prior to the execution of the action.
+
+##### Basic File Manipulation
+- `mkdir`, which requires a `directory` attribute to specify the path of the directory to be created 
+  (only if it doesn't already exist)
+- `copy`, which copies files into the bundle, and supports the following arguments:
+  - `source`, `target` and `includes` - if `includes` is not present, `source` and `target` are both
+    assumed to be file paths to a single file. If `includes` is provided, `source` and `target` are 
+    assumed to be directories, and each member of the `includes` list a glob pattern inside the
+    `source` directory.
+  - `rename` - If provided, must contain `from` and `to` attributes. When specified, each file
+    is renamed as it is copied, where `from` is treated as a Python regular expression
+    applied to the base name of the source file, and `to` is the substitution string which
+    replaces it in the name of the target file. Backreferences are available for capturing groups, e.g.
+    ```yaml
+      rename:
+        from: "(.*)\\.owl"
+        to: "\\g<1>{version}.owl"
+    ```
+    will add a version number to the base name of each `.owl` file. Further documentation on
+    Python regular expression replace functionality can be found
+    [here](https://docs.python.org/3/howto/regex.html#search-and-replace).
+  - `replace` - If provided, must contain `from` and `to` attributes. When specified, each file
+    is processed after being copied, and each instance of the `from` pattern is replaced
+    with `to` string in the file contents. Python regular expression syntax and backreferences are
+    supported as shown in the `rename` documentation.
+- `move`, which moves files according the provided options, which are identical to the ones supported
+  by `copy`.
+  
+##### RDF Transformation
+
+- `definedBy`, which inspects each input file to identify a single defined ontology, and then
+  adds a `rdfs:isDefinedBy` property to every `owl:Class`, `owl:ObjectProperty`, `owl:DatatypeProperty`
+  and `owl:AnnotationProperty` defined in the file referencing the identified ontology. Existing
+  `rdfs:isDefinedBy` values are removed prior to the addition. Input and output file specification
+  options are identical to those used by the `copy` action.
+- `export`, which functions similarly to the command-line export functionality, gathering one or
+  more input ontologies and exporting them as a single file, with some optional transformations,
+  depending on the following specified options:
+  - `source`, `target` and `includes` - if `includes` is not present, `source` is
+    assumed to be the path to a single file. If `includes` is provided, `source` is 
+    assumed to be a directory, and each member of the `includes` list a glob pattern inside the
+    `source` directory. `target` is always treated as a single file path.
+  - `merge` - if provided, it must have two mandatory fields, `iri` and `version`. In this case, all
+    ontologies declared in the input files are removed, and a single new ontologies, specified by the 
+    `iri` is created, using `version` to build `owl:versionInfo` and `owl:versionIRI`. Any imports on
+    the removed ontologies which are not satisfied internally are transferred to the new ontology.
+  - `definedBy` - has two possible values, `strict` and `all`. If provided, a `rdfs:isDefinedBy` is
+    added to all non-blank node subjects in the exported RDF linking them to the ontology defined in the
+    combined graph. If more that one ontology is defined, the export will fail. If `strict` is specified,
+    only classes and properties will be annotated, whereas `all` does not filter by type.
+  - `retainDefinedBy` - by default, `definedBy` will override any existing `rdfs:definedBy` annotations,
+    but if this option is provided, existing annotations will be left in place.
+  - `format` - One of `turtle`, `xml`, or `nt` (N-Triples), specifies the output format for the export.
+    The default output format is `turtle`.
+  - `context` - If provided, generates a N-Quads export with the `context` argument as the name of the
+    graph. When this option is present, the value of `format` is ignored.
+  - `compress` - when this is `true`, the output is `gzip`-ed.
+- `transform`, which applies the specified tool to a set of input files, and supports the following
+  arguments:
+  - `tool`, which references the `name` of a tool which must be defined in the `tools` section.
+  - `source`, `target` and `includes`, which function just like they do for the `copy` and `move`
+    actions, with each input and output path bound into the `inputFile` and `outputFile` variables
+    before the tool arguments are interpreted.
+  - `replace` and `rename`, which are applied after the tool invocation, and work as described above.
+- `sparql` reads RDF files provided via the `source` and `includes` options and executes a SPARQL
+  query on the resulting combined graph.
+    * If the `query` option is a valid file path, the query is read from that file,
+      otherwise the contents of the `query` option are interpreted as the query.
+    * `SELECT` query results are stored in the file specified via `target` as a CSV.
+    * RDF results from a `CONSTRUCT` query are
+  stored as either Turtle, RDF/XML or N-Triples, depending on the `format` option (`turtle`, `xml`, or `nt`).
+      Update queries will alter the input data in place, and the resulting
+      graph will be output in the specified format.
+    * `UPDATE` queries executed on local files will modify the in-memory graph and then serialize the
+      resulting graph to the `target`.
+    * The default functionality is to combine all RDF sources specified via `includes`
+      and execute queries on the resulting graph. However, if `eachFile: true` is added,
+      all queries will be applied to each source file separately, and will produce a 
+      separate output file. In this case, `target` will be treated as a directory, and
+      the `rename` option should be used when needed to construct the output file names. For example, the following
+      action extracts the labels out of each RDF file into a separate CSV with matching names:
+      ```yaml
+      - action: 'sparql'
+        message: "Multi-file processing with SELECT"
+        eachFile: true
+        source: '{input}'
+        includes:
+          - '*_ontology.ttl'
+        target: "{output}/each/select"
+        rename:
+          from: "(.*)\\.ttl"
+          to: "\\g<1>.csv"
+        query: >
+          prefix rdfs: <http://www.w3.org/2000/01/rdf-schema#>
+          prefix skos: <http://www.w3.org/2004/02/skos/core#>
+          select ?label
+          WHERE {{
+            ?s rdfs:label ?label .
+          }} order by ?label
+      ```
+    * As an alternative to operating on local RDF specified via 'source', a query can
+      be executed on a triple store by specifying an `endpoint`, which must
+      contain a `query_uri`, and can optionally specify `user`/`password` which will
+      authenticate via HTTP basic authentication. Update queries will modify the
+      triple store directly, and a separate `update_uri` can be specified
+      for databases which require it.
+
+  
+##### Utility Actions
+- `markdown` transforms a `.md` file referenced in `source` into an HTML output specified in `target`.
+- `graph` reads RDF files provided via the `source` and `includes` options and generates a graphical
+  representation of the ontology, as in the `graphic` sub-command described above. Both `.dot` and
+  `.png` outputs are written to the directory specified in the `target` option, and `title` and 
+  `version` attributes configure the title on the generated graph. If `compact` is specified as
+  `True`, a concise graph including only ontology names and imports is generated.
+
+##### Validation
+The `verify` action reads RDF files provided via the `source` and `includes` options and performs validation on the
+resulting combined graph. If the validation fails, the bundle process exits with a non-zero status and
+does not execute subsequent actions. The type of verification performed depends on the 
+value of the `type` option:
+* If `type` is `select`, one or more SPARQL `SELECT` queries are executed against the graph, and the
+  first query to return a non-empty result will terminate the bundle. The results of the query will
+  be output to the log, and also written as CSV to a file path specified by the `target` option, if
+  provided. Queries can be specified in one of two ways (only one can be present):
+  * If the `query` option is a valid file path, the query is read from that file,
+    otherwise the contents of the `query` option are interpreted as the query, e.g.
+    ```yaml
+    query: >
+      prefix skos: <http://www.w3.org/2004/02/skos/core#>
+      select ?unlabeled where {{
+        ?unlabeled a ?type .
+        filter not exists {{ ?unlabeled skos:prefLabel ?label }}
+      }}
+    ```
+  * If `queries` is provided, a list of queries will be built from the `source` and `includes`
+    sub-options. The queries will be executed in order specified. If `stopOnFail` is omitted or
+    is `true`, the first  query that produces a failing result will cause `verify` to abort. If
+    `stopOnFail` is `false`, all queries will be executed regardless of failures, and the value
+    of `target` is treated as a directory where the results of _each_ failing query will be written.
+    ```yaml
+      - action: 'verify'
+        type: 'select'
+        source: '{input}'
+        includes:
+          - 'verify_data.ttl'
+        target: '{output}/verify_select_results'
+        stopOnFail: false
+        queries:
+          source: '{input}'
+          includes:
+            - 'verify_*_select_query.rq'
+    ```
+* If `type` is `ask`, one or more SPARQL `ASK` queries will be executed. Queries are
+  specified similarly to the `select` validation. Unless `stopOnFail` is set to `false`, the first
+  query producing a result that does not match the required `expected` option, the bundle will terminate.
+  For example:
+  ```yaml
+  actions:
+    - action: 'verify'
+      type: 'ask'
+      source: '{input}'
+      includes:
+        - 'verify_data.ttl'
+      queries:
+        source: '{input}'
+        includes:
+          - '*_ask_query.rq'
+      expected: false
+  ```
+* If `type` is `shacl`, a SHACL shape graph will be constructed from the file specified via the `shapes`
+  option (which must have a `source`, and optionally `includes`), with the bundle terminating only if
+  any `sh:Violation` results are present, unless the `failOn` option specifies otherwise.`
+  The report is emitted to the log, and saved as Turtle to the path specified in the `target` option if it's provided.
+  For example:
+  ```yaml
+  - action: 'verify'
+    type: 'shacl'
+    inference: 'rdfs'
+    source: '{input}'
+    includes:
+      - 'verify_data.ttl'
+    target: '{output}/verify_shacl_errors.ttl'
+    failOn: "warning"
+    shapes:
+      source: '{input}/verify_shacl_shapes.ttl'
+  ```
+  If the `inference` option is provided, the reasoner will be run on the graph prior
+  to applying the SHACL rules. The valid values are:
+    * `rdfs`,
+    * `owlrl`,
+    * `both`, or
+    * `none` (default).
+* If `type` is `construct`, the queries are expected to `CONSTRUCT` a [SHACL ValidationReport](https://www.w3.org/TR/shacl/#validation-report).
+  The validation will be considered as a failure if the resulting graph is non-empty. `target`,
+  `stopOnFail` and `query`/`queries` are handled same as `select` validation, and `failOn` is used to determine which
+  violations will terminate execution.
+* Validation can be performed against a SPARQL endpoint instead of local RDF
+  data by specifying `endpoint` instead of `source`/`includes`. `endpoint` must
+  contain a `query_uri`, and can optionally specify `user`/`password` which will
+  authenticate via HTTP basic authentication. For example:
+  ```
+  - action: 'verify'
+    type: 'construct'
+    endpoint:
+      query_uri: 'https://my.endpoint.com/sparql'
+      user: 'test-user'
+      password: 'test-user'
+    target: '{output}/verify_construct_results'
+    stopOnFail: false
+    query: '{input}/verify_via_construct.rq'
+  ```
```

### Comparing `onto_tool-1.7.2/README.md` & `onto_tool-1.7.3/onto_tool.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,24 @@
+Metadata-Version: 2.1
+Name: onto-tool
+Version: 1.7.3
+Summary: Ontology Maintenance and Release Tool
+Home-page: https://github.com/semanticarts/ontology-toolkit
+Author: Boris Pelakh
+Author-email: boris.pelakh@semanticarts.com
+License: UNKNOWN
+Platform: UNKNOWN
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # ontology-toolkit
 
 Maintain version and dependency info in RDF ontologies.
 
 ## Installation
 
 ## Easy Install 
@@ -535,7 +552,9 @@
       query_uri: 'https://my.endpoint.com/sparql'
       user: 'test-user'
       password: 'test-user'
     target: '{output}/verify_construct_results'
     stopOnFail: false
     query: '{input}/verify_via_construct.rq'
   ```
+
+
```

### Comparing `onto_tool-1.7.2/onto_tool/bundle_schema.yaml` & `onto_tool-1.7.3/onto_tool/bundle_schema.yaml`

 * *Files identical despite different names*

### Comparing `onto_tool-1.7.2/onto_tool/command_line.py` & `onto_tool-1.7.3/onto_tool/command_line.py`

 * *Files identical despite different names*

### Comparing `onto_tool-1.7.2/onto_tool/mdutils.py` & `onto_tool-1.7.3/onto_tool/mdutils.py`

 * *Files identical despite different names*

### Comparing `onto_tool-1.7.2/onto_tool/onto_tool.py` & `onto_tool-1.7.3/onto_tool/onto_tool.py`

 * *Files identical despite different names*

### Comparing `onto_tool-1.7.2/onto_tool/ontograph.py` & `onto_tool-1.7.3/onto_tool/ontograph.py`

 * *Files identical despite different names*

### Comparing `onto_tool-1.7.2/onto_tool/sparql_utils.py` & `onto_tool-1.7.3/onto_tool/sparql_utils.py`

 * *Files identical despite different names*

### Comparing `onto_tool-1.7.2/onto_tool.egg-info/PKG-INFO` & `onto_tool-1.7.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,557 +1,560 @@
 Metadata-Version: 2.1
-Name: onto-tool
-Version: 1.7.2
+Name: onto_tool
+Version: 1.7.3
 Summary: Ontology Maintenance and Release Tool
 Home-page: https://github.com/semanticarts/ontology-toolkit
 Author: Boris Pelakh
 Author-email: boris.pelakh@semanticarts.com
 License: UNKNOWN
-Description: # ontology-toolkit
-        
-        Maintain version and dependency info in RDF ontologies.
-        
-        ## Installation
-        
-        ## Easy Install 
-        
-        To install the most recent released version of the toolkit use `pip install onto-tool`. 
-        
-        ## Development Install
-        
-        To experiment with unreleased features currently in development, clone this repo and navigate to the installed directory.  Run `python -m setup install`, which
-        will install the `onto_tool` command and all its dependencies into your environment.
-        
-        ```
-        $ onto_tool -h
-        usage: onto_tool [-h] [-k] [-v] {update,export,bundle,graphic} ...
-        
-        Ontology toolkit.
-        
-        positional arguments:
-          {update,export,bundle,graphic}
-                                sub-command help
-            update              Update versions and dependencies
-            export              Export ontology
-            bundle              Bundle ontology for release
-            graphic             Create PNG graphic and dot file from OWL files or SPARQL Endpoint
-        
-        optional arguments:
-          -h, --help            show this help message and exit
-          -k, --insecure        Allow insecure server connections when using SSL
-          -v, --version         Report onto-tool version and exit
-        ```
-        
-        ## Sub-Commands
-        
-        ### Update
-        
-        The `update` sub-command modifies ontology version and dependency information
-        ```
-        $ onto_tool update -h
-        usage: onto_tool update [-h] [-f {xml,turtle,nt} | -i] [--debug] [-o OUTPUT]
-                                [-b [{all,strict}]] [--retain-definedBy]
-                                [--versioned-definedBy] [-v SET_VERSION]
-                                [--version-info [VERSION_INFO]]
-                                [-d DEPENDENCY VERSION]
-                                [ontology [ontology ...]]
-        
-        positional arguments:
-          ontology              Ontology file or directory containing OWL files
-        
-        optional arguments:
-          -h, --help            show this help message and exit
-          -f {xml,turtle,nt}, --format {xml,turtle,nt}
-                                Output format
-          -i, --in-place        Overwrite each input file with update, preserving
-                                format
-          --debug               Emit verbose debug output
-          -o OUTPUT, --output OUTPUT
-                                Path to output file. Will be ignored if --in-place is
-                                specified.
-          -b [{all,strict}], --defined-by [{all,strict}]
-                                Add rdfs:isDefinedBy to every resource defined. If the
-                                (default) "strict" argument is provided, only
-                                owl:Class, owl:ObjectProperty, owl:DatatypeProperty,
-                                owl:AnnotationProperty and owl:Thing entities will be
-                                annotated. If "all" is provided, every entity that has
-                                any properties other than rdf:type will be annotated.
-                                Will override any existing rdfs:isDefinedBy
-                                annotations on the affected entities unless --retain-
-                                definedBy is specified.
-          -v SET_VERSION, --set-version SET_VERSION
-                                Set the version of the defined ontology
-          --version-info [VERSION_INFO]
-                                Adjust versionInfo, defaults to "Version X.x.x"
-          -d DEPENDENCY VERSION, --dependency-version DEPENDENCY VERSION
-                                Update the import of DEPENDENCY to VERSION
-        ```
-        
-        ### Export
-        
-        The `export` sub-command will transform the ontology into the desired format, and remove version information, as required by tools such as Top Braid Composer.
-        ```
-        usage: onto_tool export [-h] [-f {xml,turtle,nt} | -c CONTEXT] [--debug]
-                                [-o OUTPUT] [-s] [-m IRI VERSION] [-b [{all,strict}]]
-                                [--retain-definedBy] [--versioned-definedBy]
-                                [ontology [ontology ...]]
-        
-        positional arguments:
-          ontology              Ontology file or directory containing OWL files
-        
-        optional arguments:
-          -h, --help            show this help message and exit
-          -f {xml,turtle,nt}, --format {xml,turtle,nt}
-                                Output format
-          -c CONTEXT, --context CONTEXT
-                                Export as N-Quads in CONTEXT.
-          --debug               Emit verbose debug output
-          -o OUTPUT, --output OUTPUT
-                                Path to output file.
-          -s, --strip-versions  Remove versions from imports.
-          -m IRI VERSION, --merge IRI VERSION
-                                Merge all inputs into a single ontology with the given
-                                IRI and version
-          -b [{all,strict}], --defined-by [{all,strict}]
-                                Add rdfs:isDefinedBy to every resource defined. If the
-                                (default) "strict" argument is provided, only
-                                owl:Class, owl:ObjectProperty, owl:DatatypeProperty,
-                                owl:AnnotationProperty and owl:Thing entities will be
-                                annotated. If "all" is provided, every entity that has
-                                any properties other than rdf:type will be annotated.
-          --retain-definedBy    When merging ontologies, retain existing values of
-                                rdfs:isDefinedBy
-        ```
-        
-        ### Graphic
-        
-        The `graphic` sub-command will create either 
-        * a comprehensive diagram showing ontology modules together with classes, object properties and individuals
-          together with the path of imports, or (if the 'wee' option is selected) a simple diagram of the ontology
-          import hierarchy, or
-        * a diagram of the use of classes and object and data properties in a triple store or local ontology files.
-            
-        Graphics are exported both as ```png``` files and also as a ```dot``` file.  This ```dot``` file can be used with Graphviz or with web tools such as [Dot Viewer](http://www.semantechs.co.uk/turtle-editor-viewer/)
-        
-        ```
-        usage: onto_tool graphic [-h] [-e ENDPOINT] [--schema | --data]
-                                 [--single-ontology-graphs] [--debug] [-o OUTPUT]
-                                 [--show-shacl]
-                                 [--link-concentrator-threshold LINK_CONCENTRATOR_THRESHOLD]
-                                 [--instance-limit INSTANCE_LIMIT]
-                                 [--predicate-threshold PREDICATE_THRESHOLD]
-                                 [--include [INCLUDE [INCLUDE ...]] |
-                                 --include-pattern [INCLUDE_REGEX [INCLUDE_REGEX ...]]
-                                 | --exclude [EXCLUDE [EXCLUDE ...]] |
-                                 --exclude-pattern
-                                 [EXCLUDE_REGEX [EXCLUDE_REGEX ...]]] [-v VERSION]
-                                 [-w [WEE [WEE ...]]]
-                                 [--label-language LABEL_LANGUAGE]
-                                 [--hide [HIDE [HIDE ...]]] [--no-image] [-t TITLE]
-                                 [ontology [ontology ...]]
-        
-        positional arguments:
-          ontology              Ontology file, directory or name pattern
-        
-        optional arguments:
-          -h, --help            show this help message and exit
-          -e ENDPOINT, --endpoint ENDPOINT
-                                URI of SPARQL endpoint to use to gather data
-          --schema              Generate ontology import graph (default)
-          --data                Analyze instances for types and links
-          --single-ontology-graphs
-                                If specified in combination with --endpoint when
-                                generating a schema graph, assume that every ontology
-                                is in its own named graph in the triple store.
-                                Otherwise rdfs:isDefinedBy will be used to locate
-                                entities defined by each ontology.
-          --debug               Emit verbose debug output
-          -o OUTPUT, --output OUTPUT
-                                Output directory for generated graphics
-          --show-shacl          Attempts to discover which classes and properties have
-                                corresponding SHACL shapes and colors them green on
-                                the graph. This detection relies on the presence of
-                                sh:targetClass targeting, and can be confused by
-                                complex logical shapes or Advanced SHACL features such
-                                as SPARQL queries.
-          --link-concentrator-threshold LINK_CONCENTRATOR_THRESHOLD
-                                When the number links originating from the same class
-                                that share a single predicate exceed this threshold
-                                (default 10), use more compact display. Setting the
-                                value to 0 disables this behavior.
-          -v VERSION, --version VERSION
-                                Version to place in graphic
-          -w [WEE [WEE ...]], --wee [WEE [WEE ...]]
-                                For ontologies matching the patterns specified, only
-                                render the name and import information. If no patterns
-                                are specified, applies to all ontologies.
-          --label-language LABEL_LANGUAGE
-                                In case entities have labels in multiple languages,
-                                select either the specified language (default: en) or
-                                a non-lanugage label.
-          --hide [HIDE [HIDE ...]]
-                                When visualizing data, hide classes and properties
-                                matching the regexpatterns specified with this option.
-          --no-image            Do not generate PNG image, only .dot output.
-          -t TITLE, --title TITLE
-                                Title to use for graph. If not supplied, the repo URI
-                                will be used if graphing an endpoint, or 'Gist' if
-                                graphing local files.
-        
-        Sampling Limits:
-          --instance-limit INSTANCE_LIMIT
-                                Specify a limit on how many triples to consider that
-                                use any one predicate to find (default 500000). This
-                                option may result in an incomplete version of the
-                                diagram, missing certain links.
-          --predicate-threshold PREDICATE_THRESHOLD
-                                Ignore predicates which occur fewer than
-                                PREDICATE_THRESHOLD times (default 10)
-        
-        Filters (only one can be used):
-          --include [INCLUDE [INCLUDE ...]]
-                                If specified for --schema, only ontologies matching
-                                the specified URIs will be shown in full detail. If
-                                specified with --data, only triples in the named
-                                graphs mentioned will be considered (this also
-                                excludes any triples in the default graph).
-          --include-pattern [INCLUDE_REGEX [INCLUDE_REGEX ...]]
-                                If specified for --schema, only ontologies matching
-                                the specified URI pattern will be shown in full
-                                detail. If specified with --data, only triples in the
-                                named graphs matching the pattern will be considered
-                                (this also excludes any triples in the default graph).
-                                For large graphs this option is significantly slower
-                                than using --include.
-          --exclude [EXCLUDE [EXCLUDE ...]]
-                                If specified for --schema, ontologies matching the
-                                specified URIs will be omitted from the graph. If
-                                specified with --data, triples in the named graphs
-                                mentioned will be excluded (this also excludes any
-                                triples in the default graph).
-          --exclude-pattern [EXCLUDE_REGEX [EXCLUDE_REGEX ...]]
-                                If specified for --schema, ontologies matching the
-                                specified URI pattern will be omitted from the graph.
-                                If specified with --data, triples in the named graphs
-                                matching the pattern will be ignored (this also
-                                excludes any triples in the default graph). For large
-                                graphs this option is significantly slower than using
-                                --exclude.
-        ```
-        
-        ### Bundle
-        
-        The `bundle` sub-command supports creating an ontology deployment containing both RDF and non-RDF artifacts for delivery or web hosting.
-        
-        ```
-        $ onto_tool bundle -h
-        usage: onto_tool bundle [-h] [--debug] [-v VARIABLE VALUE] bundle
-        
-        positional arguments:
-          bundle                JSON or YAML bundle definition
-        
-        optional arguments:
-          -h, --help            show this help message and exit
-          --debug               Emit verbose debug output
-          -v VARIABLE VALUE, --variable VARIABLE VALUE
-                                Set value of VARIABLE to VALUE
-        ```
-        
-        The bundle definition is either YAML or JSON, and contains the following sections:
-        
-        #### Variable definition
-        
-        ```yaml
-        variables:
-          name: "gist"
-          version: "X.x.x"
-          input: "."
-          rdf-toolkit: "{input}/tools/rdf-toolkit.jar"
-          output: "{name}{version}_webDownload"
-        ```
-        Variables are initialized with the default values provided, but can be overriden via the `--variable` command line option.
-        Values can reference other values using the `{name}` template syntax.
-        
-        #### Tool definition
-        
-        All tools require a `name` by which they are referenced in `transform` actions. Three different tool types are supported:
-        * Java tools (`type: "Java"`) require a path to the executable Jar file specified via the `jar` option,
-          and a list of `arguments` that will be applied to each file processed.
-          The `inputFile` and `outputFile` variables will be bound during execution, but other variables can be
-          used to construct the arguments.
-          tools:
-          ```yaml
-          - name: "serializer"
-            type: "Java"
-            jar: "{rdf-toolkit}"
-            arguments:
-              - "-tfmt"
-              - "rdf-xml"
-              - "-sdt"
-              - "explicit"
-              - "-dtd"
-              - "-ibn"
-              - "-s"
-              - "{inputFile}"
-              - "-t"
-              - "{outputFile}"
-          ```
-        * Shell tools (`type: "shell"`) execute a command specified via
-          a list of `arguments` that will be applied to each file processed.
-          The `inputFile` and `outputFile` variables will be bound during execution, but other variables can be
-          used to construct the arguments.
-          tools:
-          ```yaml
-            tools:
-            - name: "java_version"
-              type: "shell"
-              arguments:
-                - "java"
-                - "-version"
-          ```
-        * SPARQL tools apply a SPARQL Update query to each input file and serialize the resulting graph into the 
-          output file. RDF format is preserved unless overridden with the `format` option. If the query is specified
-          inline, template substitution will be applied to it, so bundle variables can be used, but double braces
-          (`{{` instead of `{`, `}}` instead of `}`) have to be used to escape actual braces.
-          ```yaml
-            - name: "add-language-en"
-              type: "sparql"
-              query: >
-                prefix skos: <http://www.w3.org/2004/02/skos/core#>
-                DELETE {{
-                  ?subject skos:prefLabel ?nolang .
-                }}
-                INSERT {{
-                  ?subject skos:prefLabel ?withlang
-                }}
-                where {{
-                  ?subject skos:prefLabel ?nolang .
-                  FILTER(lang(?nolang) = '')
-                  BIND(STRLANG(?nolang, '{lang}') as ?withlang)
-                }}
-          ```
-        
-        #### Actions
-        
-        Actions are executed in the order they are listed. Each action must have an `action` attribute,
-        and any action can contain a `message` attribute, the contents of which will be
-        emitted as a `INFO`-level log message prior to the execution of the action.
-        
-        ##### Basic File Manipulation
-        - `mkdir`, which requires a `directory` attribute to specify the path of the directory to be created 
-          (only if it doesn't already exist)
-        - `copy`, which copies files into the bundle, and supports the following arguments:
-          - `source`, `target` and `includes` - if `includes` is not present, `source` and `target` are both
-            assumed to be file paths to a single file. If `includes` is provided, `source` and `target` are 
-            assumed to be directories, and each member of the `includes` list a glob pattern inside the
-            `source` directory.
-          - `rename` - If provided, must contain `from` and `to` attributes. When specified, each file
-            is renamed as it is copied, where `from` is treated as a Python regular expression
-            applied to the base name of the source file, and `to` is the substitution string which
-            replaces it in the name of the target file. Backreferences are available for capturing groups, e.g.
-            ```yaml
-              rename:
-                from: "(.*)\\.owl"
-                to: "\\g<1>{version}.owl"
-            ```
-            will add a version number to the base name of each `.owl` file. Further documentation on
-            Python regular expression replace functionality can be found
-            [here](https://docs.python.org/3/howto/regex.html#search-and-replace).
-          - `replace` - If provided, must contain `from` and `to` attributes. When specified, each file
-            is processed after being copied, and each instance of the `from` pattern is replaced
-            with `to` string in the file contents. Python regular expression syntax and backreferences are
-            supported as shown in the `rename` documentation.
-        - `move`, which moves files according the provided options, which are identical to the ones supported
-          by `copy`.
-          
-        ##### RDF Transformation
-        
-        - `definedBy`, which inspects each input file to identify a single defined ontology, and then
-          adds a `rdfs:isDefinedBy` property to every `owl:Class`, `owl:ObjectProperty`, `owl:DatatypeProperty`
-          and `owl:AnnotationProperty` defined in the file referencing the identified ontology. Existing
-          `rdfs:isDefinedBy` values are removed prior to the addition. Input and output file specification
-          options are identical to those used by the `copy` action.
-        - `export`, which functions similarly to the command-line export functionality, gathering one or
-          more input ontologies and exporting them as a single file, with some optional transformations,
-          depending on the following specified options:
-          - `source`, `target` and `includes` - if `includes` is not present, `source` is
-            assumed to be the path to a single file. If `includes` is provided, `source` is 
-            assumed to be a directory, and each member of the `includes` list a glob pattern inside the
-            `source` directory. `target` is always treated as a single file path.
-          - `merge` - if provided, it must have two mandatory fields, `iri` and `version`. In this case, all
-            ontologies declared in the input files are removed, and a single new ontologies, specified by the 
-            `iri` is created, using `version` to build `owl:versionInfo` and `owl:versionIRI`. Any imports on
-            the removed ontologies which are not satisfied internally are transferred to the new ontology.
-          - `definedBy` - has two possible values, `strict` and `all`. If provided, a `rdfs:isDefinedBy` is
-            added to all non-blank node subjects in the exported RDF linking them to the ontology defined in the
-            combined graph. If more that one ontology is defined, the export will fail. If `strict` is specified,
-            only classes and properties will be annotated, whereas `all` does not filter by type.
-          - `retainDefinedBy` - by default, `definedBy` will override any existing `rdfs:definedBy` annotations,
-            but if this option is provided, existing annotations will be left in place.
-          - `format` - One of `turtle`, `xml`, or `nt` (N-Triples), specifies the output format for the export.
-            The default output format is `turtle`.
-          - `context` - If provided, generates a N-Quads export with the `context` argument as the name of the
-            graph. When this option is present, the value of `format` is ignored.
-          - `compress` - when this is `true`, the output is `gzip`-ed.
-        - `transform`, which applies the specified tool to a set of input files, and supports the following
-          arguments:
-          - `tool`, which references the `name` of a tool which must be defined in the `tools` section.
-          - `source`, `target` and `includes`, which function just like they do for the `copy` and `move`
-            actions, with each input and output path bound into the `inputFile` and `outputFile` variables
-            before the tool arguments are interpreted.
-          - `replace` and `rename`, which are applied after the tool invocation, and work as described above.
-        - `sparql` reads RDF files provided via the `source` and `includes` options and executes a SPARQL
-          query on the resulting combined graph.
-            * If the `query` option is a valid file path, the query is read from that file,
-              otherwise the contents of the `query` option are interpreted as the query.
-            * `SELECT` query results are stored in the file specified via `target` as a CSV.
-            * RDF results from a `CONSTRUCT` query are
-          stored as either Turtle, RDF/XML or N-Triples, depending on the `format` option (`turtle`, `xml`, or `nt`).
-              Update queries will alter the input data in place, and the resulting
-              graph will be output in the specified format.
-            * `UPDATE` queries executed on local files will modify the in-memory graph and then serialize the
-              resulting graph to the `target`.
-            * The default functionality is to combine all RDF sources specified via `includes`
-              and execute queries on the resulting graph. However, if `eachFile: true` is added,
-              all queries will be applied to each source file separately, and will produce a 
-              separate output file. In this case, `target` will be treated as a directory, and
-              the `rename` option should be used when needed to construct the output file names. For example, the following
-              action extracts the labels out of each RDF file into a separate CSV with matching names:
-              ```yaml
-              - action: 'sparql'
-                message: "Multi-file processing with SELECT"
-                eachFile: true
-                source: '{input}'
-                includes:
-                  - '*_ontology.ttl'
-                target: "{output}/each/select"
-                rename:
-                  from: "(.*)\\.ttl"
-                  to: "\\g<1>.csv"
-                query: >
-                  prefix rdfs: <http://www.w3.org/2000/01/rdf-schema#>
-                  prefix skos: <http://www.w3.org/2004/02/skos/core#>
-                  select ?label
-                  WHERE {{
-                    ?s rdfs:label ?label .
-                  }} order by ?label
-              ```
-            * As an alternative to operating on local RDF specified via 'source', a query can
-              be executed on a triple store by specifying an `endpoint`, which must
-              contain a `query_uri`, and can optionally specify `user`/`password` which will
-              authenticate via HTTP basic authentication. Update queries will modify the
-              triple store directly, and a separate `update_uri` can be specified
-              for databases which require it.
-        
-          
-        ##### Utility Actions
-        - `markdown` transforms a `.md` file referenced in `source` into an HTML output specified in `target`.
-        - `graph` reads RDF files provided via the `source` and `includes` options and generates a graphical
-          representation of the ontology, as in the `graphic` sub-command described above. Both `.dot` and
-          `.png` outputs are written to the directory specified in the `target` option, and `title` and 
-          `version` attributes configure the title on the generated graph. If `compact` is specified as
-          `True`, a concise graph including only ontology names and imports is generated.
-        
-        ##### Validation
-        The `verify` action reads RDF files provided via the `source` and `includes` options and performs validation on the
-        resulting combined graph. If the validation fails, the bundle process exits with a non-zero status and
-        does not execute subsequent actions. The type of verification performed depends on the 
-        value of the `type` option:
-        * If `type` is `select`, one or more SPARQL `SELECT` queries are executed against the graph, and the
-          first query to return a non-empty result will terminate the bundle. The results of the query will
-          be output to the log, and also written as CSV to a file path specified by the `target` option, if
-          provided. Queries can be specified in one of two ways (only one can be present):
-          * If the `query` option is a valid file path, the query is read from that file,
-            otherwise the contents of the `query` option are interpreted as the query, e.g.
-            ```yaml
-            query: >
-              prefix skos: <http://www.w3.org/2004/02/skos/core#>
-              select ?unlabeled where {{
-                ?unlabeled a ?type .
-                filter not exists {{ ?unlabeled skos:prefLabel ?label }}
-              }}
-            ```
-          * If `queries` is provided, a list of queries will be built from the `source` and `includes`
-            sub-options. The queries will be executed in order specified. If `stopOnFail` is omitted or
-            is `true`, the first  query that produces a failing result will cause `verify` to abort. If
-            `stopOnFail` is `false`, all queries will be executed regardless of failures, and the value
-            of `target` is treated as a directory where the results of _each_ failing query will be written.
-            ```yaml
-              - action: 'verify'
-                type: 'select'
-                source: '{input}'
-                includes:
-                  - 'verify_data.ttl'
-                target: '{output}/verify_select_results'
-                stopOnFail: false
-                queries:
-                  source: '{input}'
-                  includes:
-                    - 'verify_*_select_query.rq'
-            ```
-        * If `type` is `ask`, one or more SPARQL `ASK` queries will be executed. Queries are
-          specified similarly to the `select` validation. Unless `stopOnFail` is set to `false`, the first
-          query producing a result that does not match the required `expected` option, the bundle will terminate.
-          For example:
-          ```yaml
-          actions:
-            - action: 'verify'
-              type: 'ask'
-              source: '{input}'
-              includes:
-                - 'verify_data.ttl'
-              queries:
-                source: '{input}'
-                includes:
-                  - '*_ask_query.rq'
-              expected: false
-          ```
-        * If `type` is `shacl`, a SHACL shape graph will be constructed from the file specified via the `shapes`
-          option (which must have a `source`, and optionally `includes`), with the bundle terminating only if
-          any `sh:Violation` results are present, unless the `failOn` option specifies otherwise.`
-          The report is emitted to the log, and saved as Turtle to the path specified in the `target` option if it's provided.
-          For example:
-          ```yaml
-          - action: 'verify'
-            type: 'shacl'
-            inference: 'rdfs'
-            source: '{input}'
-            includes:
-              - 'verify_data.ttl'
-            target: '{output}/verify_shacl_errors.ttl'
-            failOn: "warning"
-            shapes:
-              source: '{input}/verify_shacl_shapes.ttl'
-          ```
-          If the `inference` option is provided, the reasoner will be run on the graph prior
-          to applying the SHACL rules. The valid values are:
-            * `rdfs`,
-            * `owlrl`,
-            * `both`, or
-            * `none` (default).
-        * If `type` is `construct`, the queries are expected to `CONSTRUCT` a [SHACL ValidationReport](https://www.w3.org/TR/shacl/#validation-report).
-          The validation will be considered as a failure if the resulting graph is non-empty. `target`,
-          `stopOnFail` and `query`/`queries` are handled same as `select` validation, and `failOn` is used to determine which
-          violations will terminate execution.
-        * Validation can be performed against a SPARQL endpoint instead of local RDF
-          data by specifying `endpoint` instead of `source`/`includes`. `endpoint` must
-          contain a `query_uri`, and can optionally specify `user`/`password` which will
-          authenticate via HTTP basic authentication. For example:
-          ```
-          - action: 'verify'
-            type: 'construct'
-            endpoint:
-              query_uri: 'https://my.endpoint.com/sparql'
-              user: 'test-user'
-              password: 'test-user'
-            target: '{output}/verify_construct_results'
-            stopOnFail: false
-            query: '{input}/verify_via_construct.rq'
-          ```
-        
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# ontology-toolkit
+
+Maintain version and dependency info in RDF ontologies.
+
+## Installation
+
+## Easy Install 
+
+To install the most recent released version of the toolkit use `pip install onto-tool`. 
+
+## Development Install
+
+To experiment with unreleased features currently in development, clone this repo and navigate to the installed directory.  Run `python -m setup install`, which
+will install the `onto_tool` command and all its dependencies into your environment.
+
+```
+$ onto_tool -h
+usage: onto_tool [-h] [-k] [-v] {update,export,bundle,graphic} ...
+
+Ontology toolkit.
+
+positional arguments:
+  {update,export,bundle,graphic}
+                        sub-command help
+    update              Update versions and dependencies
+    export              Export ontology
+    bundle              Bundle ontology for release
+    graphic             Create PNG graphic and dot file from OWL files or SPARQL Endpoint
+
+optional arguments:
+  -h, --help            show this help message and exit
+  -k, --insecure        Allow insecure server connections when using SSL
+  -v, --version         Report onto-tool version and exit
+```
+
+## Sub-Commands
+
+### Update
+
+The `update` sub-command modifies ontology version and dependency information
+```
+$ onto_tool update -h
+usage: onto_tool update [-h] [-f {xml,turtle,nt} | -i] [--debug] [-o OUTPUT]
+                        [-b [{all,strict}]] [--retain-definedBy]
+                        [--versioned-definedBy] [-v SET_VERSION]
+                        [--version-info [VERSION_INFO]]
+                        [-d DEPENDENCY VERSION]
+                        [ontology [ontology ...]]
+
+positional arguments:
+  ontology              Ontology file or directory containing OWL files
+
+optional arguments:
+  -h, --help            show this help message and exit
+  -f {xml,turtle,nt}, --format {xml,turtle,nt}
+                        Output format
+  -i, --in-place        Overwrite each input file with update, preserving
+                        format
+  --debug               Emit verbose debug output
+  -o OUTPUT, --output OUTPUT
+                        Path to output file. Will be ignored if --in-place is
+                        specified.
+  -b [{all,strict}], --defined-by [{all,strict}]
+                        Add rdfs:isDefinedBy to every resource defined. If the
+                        (default) "strict" argument is provided, only
+                        owl:Class, owl:ObjectProperty, owl:DatatypeProperty,
+                        owl:AnnotationProperty and owl:Thing entities will be
+                        annotated. If "all" is provided, every entity that has
+                        any properties other than rdf:type will be annotated.
+                        Will override any existing rdfs:isDefinedBy
+                        annotations on the affected entities unless --retain-
+                        definedBy is specified.
+  -v SET_VERSION, --set-version SET_VERSION
+                        Set the version of the defined ontology
+  --version-info [VERSION_INFO]
+                        Adjust versionInfo, defaults to "Version X.x.x"
+  -d DEPENDENCY VERSION, --dependency-version DEPENDENCY VERSION
+                        Update the import of DEPENDENCY to VERSION
+```
+
+### Export
+
+The `export` sub-command will transform the ontology into the desired format, and remove version information, as required by tools such as Top Braid Composer.
+```
+usage: onto_tool export [-h] [-f {xml,turtle,nt} | -c CONTEXT] [--debug]
+                        [-o OUTPUT] [-s] [-m IRI VERSION] [-b [{all,strict}]]
+                        [--retain-definedBy] [--versioned-definedBy]
+                        [ontology [ontology ...]]
+
+positional arguments:
+  ontology              Ontology file or directory containing OWL files
+
+optional arguments:
+  -h, --help            show this help message and exit
+  -f {xml,turtle,nt}, --format {xml,turtle,nt}
+                        Output format
+  -c CONTEXT, --context CONTEXT
+                        Export as N-Quads in CONTEXT.
+  --debug               Emit verbose debug output
+  -o OUTPUT, --output OUTPUT
+                        Path to output file.
+  -s, --strip-versions  Remove versions from imports.
+  -m IRI VERSION, --merge IRI VERSION
+                        Merge all inputs into a single ontology with the given
+                        IRI and version
+  -b [{all,strict}], --defined-by [{all,strict}]
+                        Add rdfs:isDefinedBy to every resource defined. If the
+                        (default) "strict" argument is provided, only
+                        owl:Class, owl:ObjectProperty, owl:DatatypeProperty,
+                        owl:AnnotationProperty and owl:Thing entities will be
+                        annotated. If "all" is provided, every entity that has
+                        any properties other than rdf:type will be annotated.
+  --retain-definedBy    When merging ontologies, retain existing values of
+                        rdfs:isDefinedBy
+```
+
+### Graphic
+
+The `graphic` sub-command will create either 
+* a comprehensive diagram showing ontology modules together with classes, object properties and individuals
+  together with the path of imports, or (if the 'wee' option is selected) a simple diagram of the ontology
+  import hierarchy, or
+* a diagram of the use of classes and object and data properties in a triple store or local ontology files.
+    
+Graphics are exported both as ```png``` files and also as a ```dot``` file.  This ```dot``` file can be used with Graphviz or with web tools such as [Dot Viewer](http://www.semantechs.co.uk/turtle-editor-viewer/)
+
+```
+usage: onto_tool graphic [-h] [-e ENDPOINT] [--schema | --data]
+                         [--single-ontology-graphs] [--debug] [-o OUTPUT]
+                         [--show-shacl]
+                         [--link-concentrator-threshold LINK_CONCENTRATOR_THRESHOLD]
+                         [--instance-limit INSTANCE_LIMIT]
+                         [--predicate-threshold PREDICATE_THRESHOLD]
+                         [--include [INCLUDE [INCLUDE ...]] |
+                         --include-pattern [INCLUDE_REGEX [INCLUDE_REGEX ...]]
+                         | --exclude [EXCLUDE [EXCLUDE ...]] |
+                         --exclude-pattern
+                         [EXCLUDE_REGEX [EXCLUDE_REGEX ...]]] [-v VERSION]
+                         [-w [WEE [WEE ...]]]
+                         [--label-language LABEL_LANGUAGE]
+                         [--hide [HIDE [HIDE ...]]] [--no-image] [-t TITLE]
+                         [ontology [ontology ...]]
+
+positional arguments:
+  ontology              Ontology file, directory or name pattern
+
+optional arguments:
+  -h, --help            show this help message and exit
+  -e ENDPOINT, --endpoint ENDPOINT
+                        URI of SPARQL endpoint to use to gather data
+  --schema              Generate ontology import graph (default)
+  --data                Analyze instances for types and links
+  --single-ontology-graphs
+                        If specified in combination with --endpoint when
+                        generating a schema graph, assume that every ontology
+                        is in its own named graph in the triple store.
+                        Otherwise rdfs:isDefinedBy will be used to locate
+                        entities defined by each ontology.
+  --debug               Emit verbose debug output
+  -o OUTPUT, --output OUTPUT
+                        Output directory for generated graphics
+  --show-shacl          Attempts to discover which classes and properties have
+                        corresponding SHACL shapes and colors them green on
+                        the graph. This detection relies on the presence of
+                        sh:targetClass targeting, and can be confused by
+                        complex logical shapes or Advanced SHACL features such
+                        as SPARQL queries.
+  --link-concentrator-threshold LINK_CONCENTRATOR_THRESHOLD
+                        When the number links originating from the same class
+                        that share a single predicate exceed this threshold
+                        (default 10), use more compact display. Setting the
+                        value to 0 disables this behavior.
+  -v VERSION, --version VERSION
+                        Version to place in graphic
+  -w [WEE [WEE ...]], --wee [WEE [WEE ...]]
+                        For ontologies matching the patterns specified, only
+                        render the name and import information. If no patterns
+                        are specified, applies to all ontologies.
+  --label-language LABEL_LANGUAGE
+                        In case entities have labels in multiple languages,
+                        select either the specified language (default: en) or
+                        a non-lanugage label.
+  --hide [HIDE [HIDE ...]]
+                        When visualizing data, hide classes and properties
+                        matching the regexpatterns specified with this option.
+  --no-image            Do not generate PNG image, only .dot output.
+  -t TITLE, --title TITLE
+                        Title to use for graph. If not supplied, the repo URI
+                        will be used if graphing an endpoint, or 'Gist' if
+                        graphing local files.
+
+Sampling Limits:
+  --instance-limit INSTANCE_LIMIT
+                        Specify a limit on how many triples to consider that
+                        use any one predicate to find (default 500000). This
+                        option may result in an incomplete version of the
+                        diagram, missing certain links.
+  --predicate-threshold PREDICATE_THRESHOLD
+                        Ignore predicates which occur fewer than
+                        PREDICATE_THRESHOLD times (default 10)
+
+Filters (only one can be used):
+  --include [INCLUDE [INCLUDE ...]]
+                        If specified for --schema, only ontologies matching
+                        the specified URIs will be shown in full detail. If
+                        specified with --data, only triples in the named
+                        graphs mentioned will be considered (this also
+                        excludes any triples in the default graph).
+  --include-pattern [INCLUDE_REGEX [INCLUDE_REGEX ...]]
+                        If specified for --schema, only ontologies matching
+                        the specified URI pattern will be shown in full
+                        detail. If specified with --data, only triples in the
+                        named graphs matching the pattern will be considered
+                        (this also excludes any triples in the default graph).
+                        For large graphs this option is significantly slower
+                        than using --include.
+  --exclude [EXCLUDE [EXCLUDE ...]]
+                        If specified for --schema, ontologies matching the
+                        specified URIs will be omitted from the graph. If
+                        specified with --data, triples in the named graphs
+                        mentioned will be excluded (this also excludes any
+                        triples in the default graph).
+  --exclude-pattern [EXCLUDE_REGEX [EXCLUDE_REGEX ...]]
+                        If specified for --schema, ontologies matching the
+                        specified URI pattern will be omitted from the graph.
+                        If specified with --data, triples in the named graphs
+                        matching the pattern will be ignored (this also
+                        excludes any triples in the default graph). For large
+                        graphs this option is significantly slower than using
+                        --exclude.
+```
+
+### Bundle
+
+The `bundle` sub-command supports creating an ontology deployment containing both RDF and non-RDF artifacts for delivery or web hosting.
+
+```
+$ onto_tool bundle -h
+usage: onto_tool bundle [-h] [--debug] [-v VARIABLE VALUE] bundle
+
+positional arguments:
+  bundle                JSON or YAML bundle definition
+
+optional arguments:
+  -h, --help            show this help message and exit
+  --debug               Emit verbose debug output
+  -v VARIABLE VALUE, --variable VARIABLE VALUE
+                        Set value of VARIABLE to VALUE
+```
+
+The bundle definition is either YAML or JSON, and contains the following sections:
+
+#### Variable definition
+
+```yaml
+variables:
+  name: "gist"
+  version: "X.x.x"
+  input: "."
+  rdf-toolkit: "{input}/tools/rdf-toolkit.jar"
+  output: "{name}{version}_webDownload"
+```
+Variables are initialized with the default values provided, but can be overriden via the `--variable` command line option.
+Values can reference other values using the `{name}` template syntax.
+
+#### Tool definition
+
+All tools require a `name` by which they are referenced in `transform` actions. Three different tool types are supported:
+* Java tools (`type: "Java"`) require a path to the executable Jar file specified via the `jar` option,
+  and a list of `arguments` that will be applied to each file processed.
+  The `inputFile` and `outputFile` variables will be bound during execution, but other variables can be
+  used to construct the arguments.
+  tools:
+  ```yaml
+  - name: "serializer"
+    type: "Java"
+    jar: "{rdf-toolkit}"
+    arguments:
+      - "-tfmt"
+      - "rdf-xml"
+      - "-sdt"
+      - "explicit"
+      - "-dtd"
+      - "-ibn"
+      - "-s"
+      - "{inputFile}"
+      - "-t"
+      - "{outputFile}"
+  ```
+* Shell tools (`type: "shell"`) execute a command specified via
+  a list of `arguments` that will be applied to each file processed.
+  The `inputFile` and `outputFile` variables will be bound during execution, but other variables can be
+  used to construct the arguments.
+  tools:
+  ```yaml
+    tools:
+    - name: "java_version"
+      type: "shell"
+      arguments:
+        - "java"
+        - "-version"
+  ```
+* SPARQL tools apply a SPARQL Update query to each input file and serialize the resulting graph into the 
+  output file. RDF format is preserved unless overridden with the `format` option. If the query is specified
+  inline, template substitution will be applied to it, so bundle variables can be used, but double braces
+  (`{{` instead of `{`, `}}` instead of `}`) have to be used to escape actual braces.
+  ```yaml
+    - name: "add-language-en"
+      type: "sparql"
+      query: >
+        prefix skos: <http://www.w3.org/2004/02/skos/core#>
+        DELETE {{
+          ?subject skos:prefLabel ?nolang .
+        }}
+        INSERT {{
+          ?subject skos:prefLabel ?withlang
+        }}
+        where {{
+          ?subject skos:prefLabel ?nolang .
+          FILTER(lang(?nolang) = '')
+          BIND(STRLANG(?nolang, '{lang}') as ?withlang)
+        }}
+  ```
+
+#### Actions
+
+Actions are executed in the order they are listed. Each action must have an `action` attribute,
+and any action can contain a `message` attribute, the contents of which will be
+emitted as a `INFO`-level log message prior to the execution of the action.
+
+##### Basic File Manipulation
+- `mkdir`, which requires a `directory` attribute to specify the path of the directory to be created 
+  (only if it doesn't already exist)
+- `copy`, which copies files into the bundle, and supports the following arguments:
+  - `source`, `target` and `includes` - if `includes` is not present, `source` and `target` are both
+    assumed to be file paths to a single file. If `includes` is provided, `source` and `target` are 
+    assumed to be directories, and each member of the `includes` list a glob pattern inside the
+    `source` directory.
+  - `rename` - If provided, must contain `from` and `to` attributes. When specified, each file
+    is renamed as it is copied, where `from` is treated as a Python regular expression
+    applied to the base name of the source file, and `to` is the substitution string which
+    replaces it in the name of the target file. Backreferences are available for capturing groups, e.g.
+    ```yaml
+      rename:
+        from: "(.*)\\.owl"
+        to: "\\g<1>{version}.owl"
+    ```
+    will add a version number to the base name of each `.owl` file. Further documentation on
+    Python regular expression replace functionality can be found
+    [here](https://docs.python.org/3/howto/regex.html#search-and-replace).
+  - `replace` - If provided, must contain `from` and `to` attributes. When specified, each file
+    is processed after being copied, and each instance of the `from` pattern is replaced
+    with `to` string in the file contents. Python regular expression syntax and backreferences are
+    supported as shown in the `rename` documentation.
+- `move`, which moves files according the provided options, which are identical to the ones supported
+  by `copy`.
+  
+##### RDF Transformation
+
+- `definedBy`, which inspects each input file to identify a single defined ontology, and then
+  adds a `rdfs:isDefinedBy` property to every `owl:Class`, `owl:ObjectProperty`, `owl:DatatypeProperty`
+  and `owl:AnnotationProperty` defined in the file referencing the identified ontology. Existing
+  `rdfs:isDefinedBy` values are removed prior to the addition. Input and output file specification
+  options are identical to those used by the `copy` action.
+- `export`, which functions similarly to the command-line export functionality, gathering one or
+  more input ontologies and exporting them as a single file, with some optional transformations,
+  depending on the following specified options:
+  - `source`, `target` and `includes` - if `includes` is not present, `source` is
+    assumed to be the path to a single file. If `includes` is provided, `source` is 
+    assumed to be a directory, and each member of the `includes` list a glob pattern inside the
+    `source` directory. `target` is always treated as a single file path.
+  - `merge` - if provided, it must have two mandatory fields, `iri` and `version`. In this case, all
+    ontologies declared in the input files are removed, and a single new ontologies, specified by the 
+    `iri` is created, using `version` to build `owl:versionInfo` and `owl:versionIRI`. Any imports on
+    the removed ontologies which are not satisfied internally are transferred to the new ontology.
+  - `definedBy` - has two possible values, `strict` and `all`. If provided, a `rdfs:isDefinedBy` is
+    added to all non-blank node subjects in the exported RDF linking them to the ontology defined in the
+    combined graph. If more that one ontology is defined, the export will fail. If `strict` is specified,
+    only classes and properties will be annotated, whereas `all` does not filter by type.
+  - `retainDefinedBy` - by default, `definedBy` will override any existing `rdfs:definedBy` annotations,
+    but if this option is provided, existing annotations will be left in place.
+  - `format` - One of `turtle`, `xml`, or `nt` (N-Triples), specifies the output format for the export.
+    The default output format is `turtle`.
+  - `context` - If provided, generates a N-Quads export with the `context` argument as the name of the
+    graph. When this option is present, the value of `format` is ignored.
+  - `compress` - when this is `true`, the output is `gzip`-ed.
+- `transform`, which applies the specified tool to a set of input files, and supports the following
+  arguments:
+  - `tool`, which references the `name` of a tool which must be defined in the `tools` section.
+  - `source`, `target` and `includes`, which function just like they do for the `copy` and `move`
+    actions, with each input and output path bound into the `inputFile` and `outputFile` variables
+    before the tool arguments are interpreted.
+  - `replace` and `rename`, which are applied after the tool invocation, and work as described above.
+- `sparql` reads RDF files provided via the `source` and `includes` options and executes a SPARQL
+  query on the resulting combined graph.
+    * If the `query` option is a valid file path, the query is read from that file,
+      otherwise the contents of the `query` option are interpreted as the query.
+    * `SELECT` query results are stored in the file specified via `target` as a CSV.
+    * RDF results from a `CONSTRUCT` query are
+  stored as either Turtle, RDF/XML or N-Triples, depending on the `format` option (`turtle`, `xml`, or `nt`).
+      Update queries will alter the input data in place, and the resulting
+      graph will be output in the specified format.
+    * `UPDATE` queries executed on local files will modify the in-memory graph and then serialize the
+      resulting graph to the `target`.
+    * The default functionality is to combine all RDF sources specified via `includes`
+      and execute queries on the resulting graph. However, if `eachFile: true` is added,
+      all queries will be applied to each source file separately, and will produce a 
+      separate output file. In this case, `target` will be treated as a directory, and
+      the `rename` option should be used when needed to construct the output file names. For example, the following
+      action extracts the labels out of each RDF file into a separate CSV with matching names:
+      ```yaml
+      - action: 'sparql'
+        message: "Multi-file processing with SELECT"
+        eachFile: true
+        source: '{input}'
+        includes:
+          - '*_ontology.ttl'
+        target: "{output}/each/select"
+        rename:
+          from: "(.*)\\.ttl"
+          to: "\\g<1>.csv"
+        query: >
+          prefix rdfs: <http://www.w3.org/2000/01/rdf-schema#>
+          prefix skos: <http://www.w3.org/2004/02/skos/core#>
+          select ?label
+          WHERE {{
+            ?s rdfs:label ?label .
+          }} order by ?label
+      ```
+    * As an alternative to operating on local RDF specified via 'source', a query can
+      be executed on a triple store by specifying an `endpoint`, which must
+      contain a `query_uri`, and can optionally specify `user`/`password` which will
+      authenticate via HTTP basic authentication. Update queries will modify the
+      triple store directly, and a separate `update_uri` can be specified
+      for databases which require it.
+
+  
+##### Utility Actions
+- `markdown` transforms a `.md` file referenced in `source` into an HTML output specified in `target`.
+- `graph` reads RDF files provided via the `source` and `includes` options and generates a graphical
+  representation of the ontology, as in the `graphic` sub-command described above. Both `.dot` and
+  `.png` outputs are written to the directory specified in the `target` option, and `title` and 
+  `version` attributes configure the title on the generated graph. If `compact` is specified as
+  `True`, a concise graph including only ontology names and imports is generated.
+
+##### Validation
+The `verify` action reads RDF files provided via the `source` and `includes` options and performs validation on the
+resulting combined graph. If the validation fails, the bundle process exits with a non-zero status and
+does not execute subsequent actions. The type of verification performed depends on the 
+value of the `type` option:
+* If `type` is `select`, one or more SPARQL `SELECT` queries are executed against the graph, and the
+  first query to return a non-empty result will terminate the bundle. The results of the query will
+  be output to the log, and also written as CSV to a file path specified by the `target` option, if
+  provided. Queries can be specified in one of two ways (only one can be present):
+  * If the `query` option is a valid file path, the query is read from that file,
+    otherwise the contents of the `query` option are interpreted as the query, e.g.
+    ```yaml
+    query: >
+      prefix skos: <http://www.w3.org/2004/02/skos/core#>
+      select ?unlabeled where {{
+        ?unlabeled a ?type .
+        filter not exists {{ ?unlabeled skos:prefLabel ?label }}
+      }}
+    ```
+  * If `queries` is provided, a list of queries will be built from the `source` and `includes`
+    sub-options. The queries will be executed in order specified. If `stopOnFail` is omitted or
+    is `true`, the first  query that produces a failing result will cause `verify` to abort. If
+    `stopOnFail` is `false`, all queries will be executed regardless of failures, and the value
+    of `target` is treated as a directory where the results of _each_ failing query will be written.
+    ```yaml
+      - action: 'verify'
+        type: 'select'
+        source: '{input}'
+        includes:
+          - 'verify_data.ttl'
+        target: '{output}/verify_select_results'
+        stopOnFail: false
+        queries:
+          source: '{input}'
+          includes:
+            - 'verify_*_select_query.rq'
+    ```
+* If `type` is `ask`, one or more SPARQL `ASK` queries will be executed. Queries are
+  specified similarly to the `select` validation. Unless `stopOnFail` is set to `false`, the first
+  query producing a result that does not match the required `expected` option, the bundle will terminate.
+  For example:
+  ```yaml
+  actions:
+    - action: 'verify'
+      type: 'ask'
+      source: '{input}'
+      includes:
+        - 'verify_data.ttl'
+      queries:
+        source: '{input}'
+        includes:
+          - '*_ask_query.rq'
+      expected: false
+  ```
+* If `type` is `shacl`, a SHACL shape graph will be constructed from the file specified via the `shapes`
+  option (which must have a `source`, and optionally `includes`), with the bundle terminating only if
+  any `sh:Violation` results are present, unless the `failOn` option specifies otherwise.`
+  The report is emitted to the log, and saved as Turtle to the path specified in the `target` option if it's provided.
+  For example:
+  ```yaml
+  - action: 'verify'
+    type: 'shacl'
+    inference: 'rdfs'
+    source: '{input}'
+    includes:
+      - 'verify_data.ttl'
+    target: '{output}/verify_shacl_errors.ttl'
+    failOn: "warning"
+    shapes:
+      source: '{input}/verify_shacl_shapes.ttl'
+  ```
+  If the `inference` option is provided, the reasoner will be run on the graph prior
+  to applying the SHACL rules. The valid values are:
+    * `rdfs`,
+    * `owlrl`,
+    * `both`, or
+    * `none` (default).
+* If `type` is `construct`, the queries are expected to `CONSTRUCT` a [SHACL ValidationReport](https://www.w3.org/TR/shacl/#validation-report).
+  The validation will be considered as a failure if the resulting graph is non-empty. `target`,
+  `stopOnFail` and `query`/`queries` are handled same as `select` validation, and `failOn` is used to determine which
+  violations will terminate execution.
+* Validation can be performed against a SPARQL endpoint instead of local RDF
+  data by specifying `endpoint` instead of `source`/`includes`. `endpoint` must
+  contain a `query_uri`, and can optionally specify `user`/`password` which will
+  authenticate via HTTP basic authentication. For example:
+  ```
+  - action: 'verify'
+    type: 'construct'
+    endpoint:
+      query_uri: 'https://my.endpoint.com/sparql'
+      user: 'test-user'
+      password: 'test-user'
+    target: '{output}/verify_construct_results'
+    stopOnFail: false
+    query: '{input}/verify_via_construct.rq'
+  ```
+
+
```

### Comparing `onto_tool-1.7.2/onto_tool.egg-info/SOURCES.txt` & `onto_tool-1.7.3/onto_tool.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE
 README.md
 setup.py
 onto_tool/__init__.py
 onto_tool/__main__.py
 onto_tool/bundle_schema.yaml
 onto_tool/command_line.py
 onto_tool/mdutils.py
```

### Comparing `onto_tool-1.7.2/setup.py` & `onto_tool-1.7.3/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -13,19 +13,18 @@
     description="Ontology Maintenance and Release Tool",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/semanticarts/ontology-toolkit",
     packages=setuptools.find_packages(),
     install_requires=[
         'pyparsing==2.4.7',
-        'rdflib~=6.0.0',
+        'rdflib~=6.1.1',
         'pydot',
         'jinja2',
         'markdown',
-        'mdx_smartypants',
         'pyyaml',
         'jsonschema>=3.2.0',
         'SPARQLWrapper>=1.8.5',
         'pyshacl~=0.17.0'
     ],
     tests_require=[
         'pytest'
```

### Comparing `onto_tool-1.7.2/tests/bundle/test_logging.py` & `onto_tool-1.7.3/tests/bundle/test_logging.py`

 * *Files identical despite different names*

### Comparing `onto_tool-1.7.2/tests/bundle/test_sparql.py` & `onto_tool-1.7.3/tests/bundle/test_sparql.py`

 * *Files identical despite different names*

### Comparing `onto_tool-1.7.2/tests/bundle/test_transform.py` & `onto_tool-1.7.3/tests/bundle/test_transform.py`

 * *Files identical despite different names*

### Comparing `onto_tool-1.7.2/tests/bundle/test_verify.py` & `onto_tool-1.7.3/tests/bundle/test_verify.py`

 * *Files identical despite different names*

### Comparing `onto_tool-1.7.2/tests/graphic/test_instance.py` & `onto_tool-1.7.3/tests/graphic/test_instance.py`

 * *Files identical despite different names*

### Comparing `onto_tool-1.7.2/tests/graphic/test_schema.py` & `onto_tool-1.7.3/tests/graphic/test_schema.py`

 * *Files identical despite different names*

### Comparing `onto_tool-1.7.2/tests/test_export.py` & `onto_tool-1.7.3/tests/test_export.py`

 * *Files identical despite different names*

### Comparing `onto_tool-1.7.2/tests/test_issue-36.py` & `onto_tool-1.7.3/tests/test_issue-36.py`

 * *Files identical despite different names*

### Comparing `onto_tool-1.7.2/tests/test_update.py` & `onto_tool-1.7.3/tests/test_update.py`

 * *Files identical despite different names*

