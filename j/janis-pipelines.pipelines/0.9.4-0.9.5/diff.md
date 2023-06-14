# Comparing `tmp/janis-pipelines.pipelines-0.9.4.tar.gz` & `tmp/janis-pipelines.pipelines-0.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/janis-pipelines.pipelines-0.9.4.tar", last modified: Mon Mar 30 01:04:54 2020, max compression
+gzip compressed data, was "dist/janis-pipelines.pipelines-0.9.5.tar", last modified: Tue Mar 31 01:54:12 2020, max compression
```

## Comparing `janis-pipelines.pipelines-0.9.4.tar` & `janis-pipelines.pipelines-0.9.5.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-03-30 01:04:54.000000 janis-pipelines.pipelines-0.9.4/
--rw-rw-r--   0 travis    (2000) travis    (2000)     4243 2020-03-30 01:04:54.000000 janis-pipelines.pipelines-0.9.4/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     3083 2020-03-30 01:04:31.000000 janis-pipelines.pipelines-0.9.4/README.md
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-03-30 01:04:54.000000 janis-pipelines.pipelines-0.9.4/janis_pipelines/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-03-30 01:04:54.000000 janis-pipelines.pipelines-0.9.4/janis_pipelines/wgs_germline/
--rw-rw-r--   0 travis    (2000) travis    (2000)    15050 2020-03-30 01:04:31.000000 janis-pipelines.pipelines-0.9.4/janis_pipelines/wgs_germline/wgsgermline.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9651 2020-03-30 01:04:31.000000 janis-pipelines.pipelines-0.9.4/janis_pipelines/wgs_germline/wgsgermline-vcallers.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-03-30 01:04:31.000000 janis-pipelines.pipelines-0.9.4/janis_pipelines/wgs_germline/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      895 2020-03-30 01:04:31.000000 janis-pipelines.pipelines-0.9.4/janis_pipelines/exportall.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-03-30 01:04:54.000000 janis-pipelines.pipelines-0.9.4/janis_pipelines/alignment/
--rw-rw-r--   0 travis    (2000) travis    (2000)     2769 2020-03-30 01:04:31.000000 janis-pipelines.pipelines-0.9.4/janis_pipelines/alignment/alignment.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-03-30 01:04:31.000000 janis-pipelines.pipelines-0.9.4/janis_pipelines/alignment/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      100 2020-03-30 01:04:31.000000 janis-pipelines.pipelines-0.9.4/janis_pipelines/__meta__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      404 2020-03-30 01:04:31.000000 janis-pipelines.pipelines-0.9.4/janis_pipelines/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-03-30 01:04:54.000000 janis-pipelines.pipelines-0.9.4/janis_pipelines/wgs_somatic/
--rw-rw-r--   0 travis    (2000) travis    (2000)    17995 2020-03-30 01:04:31.000000 janis-pipelines.pipelines-0.9.4/janis_pipelines/wgs_somatic/wgssomatic.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5241 2020-03-30 01:04:31.000000 janis-pipelines.pipelines-0.9.4/janis_pipelines/wgs_somatic/wgsomatic-vcallers.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-03-30 01:04:31.000000 janis-pipelines.pipelines-0.9.4/janis_pipelines/wgs_somatic/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-03-30 01:04:54.000000 janis-pipelines.pipelines-0.9.4/janis_pipelines/wgs_germline_gatk/
--rw-rw-r--   0 travis    (2000) travis    (2000)    10399 2020-03-30 01:04:31.000000 janis-pipelines.pipelines-0.9.4/janis_pipelines/wgs_germline_gatk/wgsgermlinegatk.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-03-30 01:04:31.000000 janis-pipelines.pipelines-0.9.4/janis_pipelines/wgs_germline_gatk/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-03-30 01:04:54.000000 janis-pipelines.pipelines-0.9.4/janis_pipelines/wgs_somatic_gatk/
--rw-rw-r--   0 travis    (2000) travis    (2000)    12275 2020-03-30 01:04:31.000000 janis-pipelines.pipelines-0.9.4/janis_pipelines/wgs_somatic_gatk/wgssomaticgatk.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-03-30 01:04:31.000000 janis-pipelines.pipelines-0.9.4/janis_pipelines/wgs_somatic_gatk/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       38 2020-03-30 01:04:54.000000 janis-pipelines.pipelines-0.9.4/setup.cfg
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-03-30 01:04:54.000000 janis-pipelines.pipelines-0.9.4/janis_pipelines.pipelines.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)     4243 2020-03-30 01:04:54.000000 janis-pipelines.pipelines-0.9.4/janis_pipelines.pipelines.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2020-03-30 01:04:54.000000 janis-pipelines.pipelines-0.9.4/janis_pipelines.pipelines.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       16 2020-03-30 01:04:54.000000 janis-pipelines.pipelines-0.9.4/janis_pipelines.pipelines.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2020-03-30 01:04:54.000000 janis-pipelines.pipelines-0.9.4/janis_pipelines.pipelines.egg-info/not-zip-safe
--rw-rw-r--   0 travis    (2000) travis    (2000)      989 2020-03-30 01:04:54.000000 janis-pipelines.pipelines-0.9.4/janis_pipelines.pipelines.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       66 2020-03-30 01:04:54.000000 janis-pipelines.pipelines-0.9.4/janis_pipelines.pipelines.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      142 2020-03-30 01:04:54.000000 janis-pipelines.pipelines-0.9.4/janis_pipelines.pipelines.egg-info/entry_points.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)     1361 2020-03-30 01:04:31.000000 janis-pipelines.pipelines-0.9.4/setup.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-03-31 01:54:12.000000 janis-pipelines.pipelines-0.9.5/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4243 2020-03-31 01:54:12.000000 janis-pipelines.pipelines-0.9.5/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3083 2020-03-31 01:53:54.000000 janis-pipelines.pipelines-0.9.5/README.md
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-03-31 01:54:12.000000 janis-pipelines.pipelines-0.9.5/janis_pipelines/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-03-31 01:54:12.000000 janis-pipelines.pipelines-0.9.5/janis_pipelines/wgs_germline/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    15083 2020-03-31 01:53:54.000000 janis-pipelines.pipelines-0.9.5/janis_pipelines/wgs_germline/wgsgermline.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9651 2020-03-31 01:53:54.000000 janis-pipelines.pipelines-0.9.5/janis_pipelines/wgs_germline/wgsgermline-vcallers.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-03-31 01:53:54.000000 janis-pipelines.pipelines-0.9.5/janis_pipelines/wgs_germline/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      895 2020-03-31 01:53:54.000000 janis-pipelines.pipelines-0.9.5/janis_pipelines/exportall.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-03-31 01:54:12.000000 janis-pipelines.pipelines-0.9.5/janis_pipelines/alignment/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2769 2020-03-31 01:53:54.000000 janis-pipelines.pipelines-0.9.5/janis_pipelines/alignment/alignment.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-03-31 01:53:54.000000 janis-pipelines.pipelines-0.9.5/janis_pipelines/alignment/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      100 2020-03-31 01:53:54.000000 janis-pipelines.pipelines-0.9.5/janis_pipelines/__meta__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      404 2020-03-31 01:53:54.000000 janis-pipelines.pipelines-0.9.5/janis_pipelines/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-03-31 01:54:12.000000 janis-pipelines.pipelines-0.9.5/janis_pipelines/wgs_somatic/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    18069 2020-03-31 01:53:54.000000 janis-pipelines.pipelines-0.9.5/janis_pipelines/wgs_somatic/wgssomatic.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5241 2020-03-31 01:53:54.000000 janis-pipelines.pipelines-0.9.5/janis_pipelines/wgs_somatic/wgsomatic-vcallers.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-03-31 01:53:54.000000 janis-pipelines.pipelines-0.9.5/janis_pipelines/wgs_somatic/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-03-31 01:54:12.000000 janis-pipelines.pipelines-0.9.5/janis_pipelines/wgs_germline_gatk/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10483 2020-03-31 01:53:54.000000 janis-pipelines.pipelines-0.9.5/janis_pipelines/wgs_germline_gatk/wgsgermlinegatk.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-03-31 01:53:54.000000 janis-pipelines.pipelines-0.9.5/janis_pipelines/wgs_germline_gatk/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-03-31 01:54:12.000000 janis-pipelines.pipelines-0.9.5/janis_pipelines/wgs_somatic_gatk/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    12775 2020-03-31 01:53:54.000000 janis-pipelines.pipelines-0.9.5/janis_pipelines/wgs_somatic_gatk/wgssomaticgatk.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-03-31 01:53:54.000000 janis-pipelines.pipelines-0.9.5/janis_pipelines/wgs_somatic_gatk/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)       38 2020-03-31 01:54:12.000000 janis-pipelines.pipelines-0.9.5/setup.cfg
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-03-31 01:54:12.000000 janis-pipelines.pipelines-0.9.5/janis_pipelines.pipelines.egg-info/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4243 2020-03-31 01:54:12.000000 janis-pipelines.pipelines-0.9.5/janis_pipelines.pipelines.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2020-03-31 01:54:12.000000 janis-pipelines.pipelines-0.9.5/janis_pipelines.pipelines.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       16 2020-03-31 01:54:12.000000 janis-pipelines.pipelines-0.9.5/janis_pipelines.pipelines.egg-info/top_level.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2020-03-31 01:54:12.000000 janis-pipelines.pipelines-0.9.5/janis_pipelines.pipelines.egg-info/not-zip-safe
+-rw-rw-r--   0 travis    (2000) travis    (2000)      989 2020-03-31 01:54:12.000000 janis-pipelines.pipelines-0.9.5/janis_pipelines.pipelines.egg-info/SOURCES.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       66 2020-03-31 01:54:12.000000 janis-pipelines.pipelines-0.9.5/janis_pipelines.pipelines.egg-info/requires.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      142 2020-03-31 01:54:12.000000 janis-pipelines.pipelines-0.9.5/janis_pipelines.pipelines.egg-info/entry_points.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1361 2020-03-31 01:53:54.000000 janis-pipelines.pipelines-0.9.5/setup.py
```

### Comparing `janis-pipelines.pipelines-0.9.4/PKG-INFO` & `janis-pipelines.pipelines-0.9.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: janis-pipelines.pipelines
-Version: 0.9.4
+Version: 0.9.5
 Summary: Bioinformatics tools for Janis; the Pipeline creation helper
 Home-page: https://github.com/PMCC-BioinformaticsCore/janis-pipelines
 Author: Michael Franklin
 Author-email: michael.franklin@petermac.org
 License: GNU
 Description: # Janis - Example Pipelines
```

### Comparing `janis-pipelines.pipelines-0.9.4/README.md` & `janis-pipelines.pipelines-0.9.5/README.md`

 * *Files identical despite different names*

### Comparing `janis-pipelines.pipelines-0.9.4/janis_pipelines/wgs_germline/wgsgermline.py` & `janis-pipelines.pipelines-0.9.5/janis_pipelines/wgs_germline/wgsgermline.py`

 * *Files 1% similar despite different names*

```diff
@@ -310,17 +310,18 @@
             source=self.merge_and_mark.out,
             output_folder="bams",
             doc="Aligned and indexed bam.",
             output_name=self.sample_name,
         )
 
         self.output(
-            "variants_combined",
+            "variants",
             source=self.sort_combined.out,
             output_folder="variants",
+            output_name=self.sample_name,
             doc="Combined variants from all 3 callers",
         )
 
         self.output(
             "variants_gatk",
             source=self.vc_gatk_merge.out,
             output_folder="variants",
```

### Comparing `janis-pipelines.pipelines-0.9.4/janis_pipelines/wgs_germline/wgsgermline-vcallers.py` & `janis-pipelines.pipelines-0.9.5/janis_pipelines/wgs_germline/wgsgermline-vcallers.py`

 * *Files identical despite different names*

### Comparing `janis-pipelines.pipelines-0.9.4/janis_pipelines/exportall.py` & `janis-pipelines.pipelines-0.9.5/janis_pipelines/exportall.py`

 * *Files identical despite different names*

### Comparing `janis-pipelines.pipelines-0.9.4/janis_pipelines/alignment/alignment.py` & `janis-pipelines.pipelines-0.9.5/janis_pipelines/alignment/alignment.py`

 * *Files identical despite different names*

### Comparing `janis-pipelines.pipelines-0.9.4/janis_pipelines/wgs_somatic/wgssomatic.py` & `janis-pipelines.pipelines-0.9.5/janis_pipelines/wgs_somatic/wgssomatic.py`

 * *Files 1% similar despite different names*

```diff
@@ -330,20 +330,22 @@
             doc="A zip file of the TUMOR FastQC quality reports.",
         )
 
         self.output(
             "normal_bam",
             source=self.normal.out,
             output_folder="bams",
+            output_name=self.normal_name,
             doc="Aligned and indexed NORMAL bam",
         )
         self.output(
             "tumor_bam",
             source=self.tumor.out,
             output_folder="bams",
+            output_name=self.tumor_name,
             doc="Aligned and indexed TUMOR bam",
         )
         self.output(
             "gridss_assembly",
             source=self.vc_gridss.out,
             output_folder="bams",
             doc="Assembly returned by GRIDSS",
@@ -370,15 +372,15 @@
         self.output(
             "variants_gridss",
             source=self.vc_gridss.out,
             output_folder="variants",
             doc="Variants from the GRIDSS variant caller",
         )
         self.output(
-            "variants_combined",
+            "variants",
             source=self.combine_variants.vcf,
             output_folder="variants",
             doc="Combined variants from all 3 callers",
         )
 
     @staticmethod
     def process_subpipeline(**connections):
```

### Comparing `janis-pipelines.pipelines-0.9.4/janis_pipelines/wgs_somatic/wgsomatic-vcallers.py` & `janis-pipelines.pipelines-0.9.5/janis_pipelines/wgs_somatic/wgsomatic-vcallers.py`

 * *Files identical despite different names*

### Comparing `janis-pipelines.pipelines-0.9.4/janis_pipelines/wgs_germline_gatk/wgsgermlinegatk.py` & `janis-pipelines.pipelines-0.9.5/janis_pipelines/wgs_germline_gatk/wgsgermlinegatk.py`

 * *Files 0% similar despite different names*

```diff
@@ -192,26 +192,28 @@
 
         self.step("sort_combined", BcfToolsSort_1_9(vcf=self.vc_gatk_merge.out))
 
         self.output(
             "bam",
             source=self.merge_and_mark.out,
             output_folder=["bams", self.sample_name],
+            output_name=self.sample_name,
             doc="Aligned and indexed bam.",
         )
         self.output(
             "reports",
             source=self.fastqc.out,
             output_folder=["reports", self.sample_name],
             doc="A zip file of the FastQC quality report.",
         )
         self.output(
             "variants",
             source=self.sort_combined.out,
             output_folder="variants",
+            output_name=self.sample_name,
             doc="Merged variants from the GATK caller",
         )
         self.output(
             "variants_split",
             source=self.vc_gatk.out,
             output_folder=["variants", "byInterval"],
             doc="Unmerged variants from the GATK caller (by interval)",
```

### Comparing `janis-pipelines.pipelines-0.9.4/janis_pipelines/wgs_somatic_gatk/wgssomaticgatk.py` & `janis-pipelines.pipelines-0.9.5/janis_pipelines/wgs_somatic_gatk/wgssomaticgatk.py`

 * *Files 6% similar despite different names*

```diff
@@ -193,22 +193,44 @@
         )
 
         self.step("vc_gatk_merge", Gatk4GatherVcfs_4_1_3(vcfs=self.vc_gatk))
         self.step("sorted", BcfToolsSort_1_9(vcf=self.vc_gatk_merge.out))
 
         # Outputs
 
-        self.output("normal_bam", source=self.normal.out, output_folder="bams")
-        self.output("tumor_bam", source=self.tumor.out, output_folder="bams")
+        self.output(
+            "normal_bam",
+            source=self.normal.out,
+            output_folder="bams",
+            output_name=self.normal_name,
+        )
+
+        self.output(
+            "tumor_bam",
+            source=self.tumor.out,
+            output_folder="bams",
+            output_name=self.tumor_name,
+        )
         self.output(
             "normal_report", source=self.normal.reports, output_folder="reports"
         )
         self.output("tumor_report", source=self.tumor.reports, output_folder="reports")
 
-        self.output("variants_gatk", source=self.sorted.out, output_folder="variants")
+        self.output(
+            "variants",
+            source=self.sorted.out,
+            output_folder="variants",
+            doc="Merged variants from the GATK caller",
+        )
+        self.output(
+            "variants_split",
+            source=self.vc_gatk.out,
+            output_folder=["variants", "byInterval"],
+            doc="Unmerged variants from the GATK caller (by interval)",
+        )
 
     @staticmethod
     def process_subpipeline(**connections):
         w = WorkflowBuilder("somatic_subpipeline")
 
         w.input("reference", FastaWithDict)
         w.input("reads", Array(FastqGzPair))
```

### Comparing `janis-pipelines.pipelines-0.9.4/janis_pipelines.pipelines.egg-info/PKG-INFO` & `janis-pipelines.pipelines-0.9.5/janis_pipelines.pipelines.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: janis-pipelines.pipelines
-Version: 0.9.4
+Version: 0.9.5
 Summary: Bioinformatics tools for Janis; the Pipeline creation helper
 Home-page: https://github.com/PMCC-BioinformaticsCore/janis-pipelines
 Author: Michael Franklin
 Author-email: michael.franklin@petermac.org
 License: GNU
 Description: # Janis - Example Pipelines
```

### Comparing `janis-pipelines.pipelines-0.9.4/janis_pipelines.pipelines.egg-info/SOURCES.txt` & `janis-pipelines.pipelines-0.9.5/janis_pipelines.pipelines.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `janis-pipelines.pipelines-0.9.4/setup.py` & `janis-pipelines.pipelines-0.9.5/setup.py`

 * *Files identical despite different names*

