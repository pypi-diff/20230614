# Comparing `tmp/genomepy-0.9.2.tar.gz` & `tmp/genomepy-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/genomepy-0.9.2.tar", last modified: Fri Jan 29 10:38:21 2021, max compression
+gzip compressed data, was "dist/genomepy-0.9.3.tar", last modified: Wed Feb  3 14:44:05 2021, max compression
```

## Comparing `genomepy-0.9.2.tar` & `genomepy-0.9.3.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 siebrenf  (1000) siebrenf  (1000)        0 2021-01-29 10:38:21.672340 genomepy-0.9.2/
--rw-r--r--   0 siebrenf  (1000) siebrenf  (1000)    10266 2021-01-28 21:40:52.000000 genomepy-0.9.2/CHANGELOG.md
--rw-r--r--   0 siebrenf  (1000) siebrenf  (1000)     1094 2021-01-28 18:42:02.000000 genomepy-0.9.2/LICENSE
--rw-r--r--   0 siebrenf  (1000) siebrenf  (1000)    25472 2021-01-29 10:38:21.656690 genomepy-0.9.2/PKG-INFO
--rw-r--r--   0 siebrenf  (1000) siebrenf  (1000)    20305 2021-01-28 21:25:40.000000 genomepy-0.9.2/README.md
-drwxr-xr-x   0 siebrenf  (1000) siebrenf  (1000)        0 2021-01-29 10:38:21.542273 genomepy-0.9.2/genomepy/
--rw-r--r--   0 siebrenf  (1000) siebrenf  (1000)       72 2021-01-28 21:40:52.000000 genomepy-0.9.2/genomepy/__about__.py
--rw-r--r--   0 siebrenf  (1000) siebrenf  (1000)      509 2021-01-28 18:42:02.000000 genomepy-0.9.2/genomepy/__init__.py
--rw-r--r--   0 siebrenf  (1000) siebrenf  (1000)     1163 2021-01-28 18:42:02.000000 genomepy-0.9.2/genomepy/argparse_support.py
-drwxr-xr-x   0 siebrenf  (1000) siebrenf  (1000)        0 2021-01-29 10:38:21.587129 genomepy-0.9.2/genomepy/cfg/
--rw-r--r--   0 siebrenf  (1000) siebrenf  (1000)       61 2021-01-28 18:42:02.000000 genomepy-0.9.2/genomepy/cfg/default.yaml
--rwxr-xr-x   0 siebrenf  (1000) siebrenf  (1000)     8362 2021-01-28 18:42:02.000000 genomepy-0.9.2/genomepy/cli.py
--rw-r--r--   0 siebrenf  (1000) siebrenf  (1000)      135 2021-01-28 18:42:02.000000 genomepy-0.9.2/genomepy/exceptions.py
--rw-r--r--   0 siebrenf  (1000) siebrenf  (1000)    12751 2021-01-28 18:42:02.000000 genomepy-0.9.2/genomepy/functions.py
--rw-r--r--   0 siebrenf  (1000) siebrenf  (1000)    15688 2021-01-28 18:42:02.000000 genomepy-0.9.2/genomepy/genome.py
--rw-r--r--   0 siebrenf  (1000) siebrenf  (1000)     2331 2021-01-28 18:42:02.000000 genomepy-0.9.2/genomepy/plugin.py
-drwxr-xr-x   0 siebrenf  (1000) siebrenf  (1000)        0 2021-01-29 10:38:21.656690 genomepy-0.9.2/genomepy/plugins/
--rw-r--r--   0 siebrenf  (1000) siebrenf  (1000)      258 2021-01-28 18:42:02.000000 genomepy-0.9.2/genomepy/plugins/__init__.py
--rw-r--r--   0 siebrenf  (1000) siebrenf  (1000)     2366 2021-01-28 18:42:02.000000 genomepy-0.9.2/genomepy/plugins/blacklist.py
--rw-r--r--   0 siebrenf  (1000) siebrenf  (1000)     1105 2021-01-28 18:42:02.000000 genomepy-0.9.2/genomepy/plugins/bowtie2.py
--rw-r--r--   0 siebrenf  (1000) siebrenf  (1000)     1159 2021-01-28 18:42:02.000000 genomepy-0.9.2/genomepy/plugins/bwa.py
--rw-r--r--   0 siebrenf  (1000) siebrenf  (1000)     1567 2021-01-28 21:35:18.000000 genomepy-0.9.2/genomepy/plugins/gmap.py
--rw-r--r--   0 siebrenf  (1000) siebrenf  (1000)     2601 2021-01-28 18:42:02.000000 genomepy-0.9.2/genomepy/plugins/hisat2.py
--rw-r--r--   0 siebrenf  (1000) siebrenf  (1000)     1155 2021-01-28 18:42:02.000000 genomepy-0.9.2/genomepy/plugins/minimap2.py
--rw-r--r--   0 siebrenf  (1000) siebrenf  (1000)     1933 2021-01-28 18:42:02.000000 genomepy-0.9.2/genomepy/plugins/star.py
--rw-r--r--   0 siebrenf  (1000) siebrenf  (1000)    41842 2021-01-29 10:38:07.000000 genomepy-0.9.2/genomepy/provider.py
--rw-r--r--   0 siebrenf  (1000) siebrenf  (1000)    18959 2021-01-28 21:33:11.000000 genomepy-0.9.2/genomepy/utils.py
-drwxr-xr-x   0 siebrenf  (1000) siebrenf  (1000)        0 2021-01-29 10:38:21.571492 genomepy-0.9.2/genomepy.egg-info/
--rw-r--r--   0 siebrenf  (1000) siebrenf  (1000)    25472 2021-01-29 10:38:20.000000 genomepy-0.9.2/genomepy.egg-info/PKG-INFO
--rw-r--r--   0 siebrenf  (1000) siebrenf  (1000)      686 2021-01-29 10:38:20.000000 genomepy-0.9.2/genomepy.egg-info/SOURCES.txt
--rw-r--r--   0 siebrenf  (1000) siebrenf  (1000)        1 2021-01-29 10:38:20.000000 genomepy-0.9.2/genomepy.egg-info/dependency_links.txt
--rw-r--r--   0 siebrenf  (1000) siebrenf  (1000)       47 2021-01-29 10:38:20.000000 genomepy-0.9.2/genomepy.egg-info/entry_points.txt
--rw-r--r--   0 siebrenf  (1000) siebrenf  (1000)       99 2021-01-29 10:38:20.000000 genomepy-0.9.2/genomepy.egg-info/requires.txt
--rw-r--r--   0 siebrenf  (1000) siebrenf  (1000)       26 2021-01-29 10:38:20.000000 genomepy-0.9.2/genomepy.egg-info/top_level.txt
--rw-r--r--   0 siebrenf  (1000) siebrenf  (1000)       38 2021-01-29 10:38:21.672340 genomepy-0.9.2/setup.cfg
--rw-r--r--   0 siebrenf  (1000) siebrenf  (1000)     1798 2021-01-28 21:25:40.000000 genomepy-0.9.2/setup.py
+drwxr-xr-x   0 siebrenf  (1000) siebrenf  (1000)        0 2021-02-03 14:44:05.736700 genomepy-0.9.3/
+-rw-r--r--   0 siebrenf  (1000) siebrenf  (1000)    10550 2021-02-03 13:06:39.000000 genomepy-0.9.3/CHANGELOG.md
+-rw-r--r--   0 siebrenf  (1000) siebrenf  (1000)     1094 2021-01-28 18:42:02.000000 genomepy-0.9.3/LICENSE
+-rw-r--r--   0 siebrenf  (1000) siebrenf  (1000)    25472 2021-02-03 14:44:05.735699 genomepy-0.9.3/PKG-INFO
+-rw-r--r--   0 siebrenf  (1000) siebrenf  (1000)    20305 2021-01-28 21:25:40.000000 genomepy-0.9.3/README.md
+drwxr-xr-x   0 siebrenf  (1000) siebrenf  (1000)        0 2021-02-03 14:44:05.650703 genomepy-0.9.3/genomepy/
+-rw-r--r--   0 siebrenf  (1000) siebrenf  (1000)       72 2021-02-03 13:06:39.000000 genomepy-0.9.3/genomepy/__about__.py
+-rw-r--r--   0 siebrenf  (1000) siebrenf  (1000)      509 2021-01-28 18:42:02.000000 genomepy-0.9.3/genomepy/__init__.py
+-rw-r--r--   0 siebrenf  (1000) siebrenf  (1000)     1163 2021-01-28 18:42:02.000000 genomepy-0.9.3/genomepy/argparse_support.py
+drwxr-xr-x   0 siebrenf  (1000) siebrenf  (1000)        0 2021-02-03 14:44:05.717787 genomepy-0.9.3/genomepy/cfg/
+-rw-r--r--   0 siebrenf  (1000) siebrenf  (1000)       61 2021-01-28 18:42:02.000000 genomepy-0.9.3/genomepy/cfg/default.yaml
+-rwxr-xr-x   0 siebrenf  (1000) siebrenf  (1000)     8362 2021-01-28 18:42:02.000000 genomepy-0.9.3/genomepy/cli.py
+-rw-r--r--   0 siebrenf  (1000) siebrenf  (1000)      135 2021-01-28 18:42:02.000000 genomepy-0.9.3/genomepy/exceptions.py
+-rw-r--r--   0 siebrenf  (1000) siebrenf  (1000)    12751 2021-01-28 18:42:02.000000 genomepy-0.9.3/genomepy/functions.py
+-rw-r--r--   0 siebrenf  (1000) siebrenf  (1000)    15691 2021-02-03 13:05:58.000000 genomepy-0.9.3/genomepy/genome.py
+-rw-r--r--   0 siebrenf  (1000) siebrenf  (1000)     2331 2021-01-28 18:42:02.000000 genomepy-0.9.3/genomepy/plugin.py
+drwxr-xr-x   0 siebrenf  (1000) siebrenf  (1000)        0 2021-02-03 14:44:05.732703 genomepy-0.9.3/genomepy/plugins/
+-rw-r--r--   0 siebrenf  (1000) siebrenf  (1000)        0 2021-02-03 13:05:58.000000 genomepy-0.9.3/genomepy/plugins/__init__.py
+-rw-r--r--   0 siebrenf  (1000) siebrenf  (1000)     2366 2021-01-28 18:42:02.000000 genomepy-0.9.3/genomepy/plugins/blacklist.py
+-rw-r--r--   0 siebrenf  (1000) siebrenf  (1000)     1105 2021-01-28 18:42:02.000000 genomepy-0.9.3/genomepy/plugins/bowtie2.py
+-rw-r--r--   0 siebrenf  (1000) siebrenf  (1000)     1159 2021-01-28 18:42:02.000000 genomepy-0.9.3/genomepy/plugins/bwa.py
+-rw-r--r--   0 siebrenf  (1000) siebrenf  (1000)     1567 2021-01-28 21:35:18.000000 genomepy-0.9.3/genomepy/plugins/gmap.py
+-rw-r--r--   0 siebrenf  (1000) siebrenf  (1000)     2601 2021-01-28 18:42:02.000000 genomepy-0.9.3/genomepy/plugins/hisat2.py
+-rw-r--r--   0 siebrenf  (1000) siebrenf  (1000)     1155 2021-01-28 18:42:02.000000 genomepy-0.9.3/genomepy/plugins/minimap2.py
+-rw-r--r--   0 siebrenf  (1000) siebrenf  (1000)     1933 2021-01-28 18:42:02.000000 genomepy-0.9.3/genomepy/plugins/star.py
+-rw-r--r--   0 siebrenf  (1000) siebrenf  (1000)    42473 2021-02-03 13:05:58.000000 genomepy-0.9.3/genomepy/provider.py
+-rw-r--r--   0 siebrenf  (1000) siebrenf  (1000)    20582 2021-02-03 13:06:39.000000 genomepy-0.9.3/genomepy/utils.py
+drwxr-xr-x   0 siebrenf  (1000) siebrenf  (1000)        0 2021-02-03 14:44:05.714700 genomepy-0.9.3/genomepy.egg-info/
+-rw-r--r--   0 siebrenf  (1000) siebrenf  (1000)    25472 2021-02-03 14:44:05.000000 genomepy-0.9.3/genomepy.egg-info/PKG-INFO
+-rw-r--r--   0 siebrenf  (1000) siebrenf  (1000)      686 2021-02-03 14:44:05.000000 genomepy-0.9.3/genomepy.egg-info/SOURCES.txt
+-rw-r--r--   0 siebrenf  (1000) siebrenf  (1000)        1 2021-02-03 14:44:05.000000 genomepy-0.9.3/genomepy.egg-info/dependency_links.txt
+-rw-r--r--   0 siebrenf  (1000) siebrenf  (1000)       47 2021-02-03 14:44:05.000000 genomepy-0.9.3/genomepy.egg-info/entry_points.txt
+-rw-r--r--   0 siebrenf  (1000) siebrenf  (1000)       99 2021-02-03 14:44:05.000000 genomepy-0.9.3/genomepy.egg-info/requires.txt
+-rw-r--r--   0 siebrenf  (1000) siebrenf  (1000)       26 2021-02-03 14:44:05.000000 genomepy-0.9.3/genomepy.egg-info/top_level.txt
+-rw-r--r--   0 siebrenf  (1000) siebrenf  (1000)       38 2021-02-03 14:44:05.736700 genomepy-0.9.3/setup.cfg
+-rw-r--r--   0 siebrenf  (1000) siebrenf  (1000)     1798 2021-01-28 21:25:40.000000 genomepy-0.9.3/setup.py
```

### Comparing `genomepy-0.9.2/CHANGELOG.md` & `genomepy-0.9.3/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,23 @@
 
 Here, the changes to `genomepy` will be summarized.
 
 The format is based on [Keep a Changelog](http://keepachangelog.com/en/1.0.0/).
 
 ## [Unreleased]
 
+## [0.9.3] - 2021-02-03
+
+### Changed
+- URL provider got better at searching for annotation files
+- NCBI provider will fall back on FTP if HTTPS is offline
+
+### Fixed
+- genomes from ftp locations not working
+
 ## [0.9.2] - 2021-01-28
 
 ### Added
 - progress bars for downloading and bgzipping (the slow stuff)
 - spinner to indexing plugins (the slowest stuff)
 
 ### Changed
@@ -273,14 +282,15 @@
 - Started CHANGELOG.
 - Genome listings are cached locally.
 - Added `-m hard` option to `install` to hard-mask sequences.
 - Added `-l` option to `install` for a custom name.
 - Added `-r` and `--match/--no-match` option to select sequences by regex.
 
 [Unreleased]: https://github.com/vanheeringen-lab/genomepy/compare/master...develop
+[0.9.3]: https://github.com/vanheeringen-lab/genomepy/compare/0.9.2...0.9.3
 [0.9.2]: https://github.com/vanheeringen-lab/genomepy/compare/0.9.1...0.9.2
 [0.9.1]: https://github.com/vanheeringen-lab/genomepy/compare/0.9.0...0.9.1
 [0.9.0]: https://github.com/vanheeringen-lab/genomepy/compare/0.8.4...0.9.0
 [0.8.4]: https://github.com/vanheeringen-lab/genomepy/compare/0.8.3...0.8.4
 [0.8.3]: https://github.com/vanheeringen-lab/genomepy/compare/0.8.2...0.8.3
 [0.8.2]: https://github.com/vanheeringen-lab/genomepy/compare/0.8.1...0.8.2
 [0.8.1]: https://github.com/vanheeringen-lab/genomepy/compare/0.7.2...0.8.1
```

### Comparing `genomepy-0.9.2/LICENSE` & `genomepy-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `genomepy-0.9.2/PKG-INFO` & `genomepy-0.9.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: genomepy
-Version: 0.9.2
+Version: 0.9.3
 Summary: Automatic downloading and processing of genomes and metadata in command line and Python
 Home-page: https://github.com/vanheeringen-lab/genomepy
 Author: Simon van Heeringen
 Author-email: simon.vanheeringen@gmail.com
 License: MIT
 Description: # genomepy
```

### Comparing `genomepy-0.9.2/README.md` & `genomepy-0.9.3/README.md`

 * *Files identical despite different names*

### Comparing `genomepy-0.9.2/genomepy/argparse_support.py` & `genomepy-0.9.3/genomepy/argparse_support.py`

 * *Files identical despite different names*

### Comparing `genomepy-0.9.2/genomepy/cli.py` & `genomepy-0.9.3/genomepy/cli.py`

 * *Files identical despite different names*

### Comparing `genomepy-0.9.2/genomepy/functions.py` & `genomepy-0.9.3/genomepy/functions.py`

 * *Files identical despite different names*

### Comparing `genomepy-0.9.2/genomepy/genome.py` & `genomepy-0.9.3/genomepy/genome.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,15 +45,15 @@
         self.name = self._parse_name(name)
         self.filename = self._parse_filename(name)
         super(Genome, self).__init__(self.filename)
 
         # file paths
         self.genome_file = self.filename
         self.genome_dir = os.path.dirname(self.filename)
-        self.index_file = self.filename + ".fai"
+        self.index_file = self.genome_file + ".fai"
         self.sizes_file = self.genome_file + ".sizes"
         self.gaps_file = os.path.join(self.genome_dir, self.name + ".gaps.bed")
         self.readme_file = os.path.join(self.genome_dir, "README.txt")
 
         # genome attributes
         self.sizes = {}
         self.gaps = {}
```

### Comparing `genomepy-0.9.2/genomepy/plugin.py` & `genomepy-0.9.3/genomepy/plugin.py`

 * *Files identical despite different names*

### Comparing `genomepy-0.9.2/genomepy/plugins/blacklist.py` & `genomepy-0.9.3/genomepy/plugins/blacklist.py`

 * *Files identical despite different names*

### Comparing `genomepy-0.9.2/genomepy/plugins/bowtie2.py` & `genomepy-0.9.3/genomepy/plugins/bowtie2.py`

 * *Files identical despite different names*

### Comparing `genomepy-0.9.2/genomepy/plugins/bwa.py` & `genomepy-0.9.3/genomepy/plugins/bwa.py`

 * *Files identical despite different names*

### Comparing `genomepy-0.9.2/genomepy/plugins/gmap.py` & `genomepy-0.9.3/genomepy/plugins/gmap.py`

 * *Files identical despite different names*

### Comparing `genomepy-0.9.2/genomepy/plugins/hisat2.py` & `genomepy-0.9.3/genomepy/plugins/hisat2.py`

 * *Files identical despite different names*

### Comparing `genomepy-0.9.2/genomepy/plugins/minimap2.py` & `genomepy-0.9.3/genomepy/plugins/minimap2.py`

 * *Files identical despite different names*

### Comparing `genomepy-0.9.2/genomepy/plugins/star.py` & `genomepy-0.9.3/genomepy/plugins/star.py`

 * *Files identical despite different names*

### Comparing `genomepy-0.9.2/genomepy/provider.py` & `genomepy-0.9.3/genomepy/provider.py`

 * *Files 5% similar despite different names*

```diff
@@ -367,15 +367,15 @@
         # generate intermediate file (GenePred)
         pred_file = annot_file.replace(ext, ".gp")
         if "bed" in ext:
             cmd = "bedToGenePred {0} {1}"
         elif "gff" in ext:
             cmd = "gff3ToGenePred -geneNameAttr=gene {0} {1}"
         elif "gtf" in ext:
-            cmd = "gtfToGenePred {0} {1}"
+            cmd = "gtfToGenePred -ignoreGroupsWithoutExons {0} {1}"
         elif "txt" in ext:
             # UCSC annotations only
             with open(annot_file) as f:
                 cols = f.readline().split("\t")
 
             # extract the genePred format columns
             start_col = 1
@@ -520,15 +520,15 @@
         ------
         tuples with name and metadata
         """
         genomes = self.genomes
         term = safe(str(term))
         if term.startswith("GCA_") and self.name != "NCBI":
             for row in self._search_accessions(term):
-                yield (row)
+                yield row
 
         elif is_number(term):
             for name in genomes:
                 if self._search_taxids(genomes[name], term):
                     yield self._genome_info_tuple(name)
 
         else:
@@ -1051,22 +1051,18 @@
         mask : str , optional
             Masking level. Options: soft, hard or none. Default is soft.
 
         Returns
         ------
         str with the http/ftp download link.
         """
-        genome = self.genomes[safe(name)]
+        # only soft masked genomes available. can be (un)masked in _post_process_download
+        link = self._ftp_or_html_link(name, file_suffix="_genomic.fna.gz")
 
-        # only soft masked genomes available. can be (un)masked in _post _process_download
-        link = genome["ftp_path"]
-        link = link.replace("ftp://", "https://")
-        link += "/" + link.split("/")[-1] + "_genomic.fna.gz"
-
-        if check_url(link, 2):
+        if link:
             return link
 
         raise GenomeDownloadError(
             f"Could not download genome {name} from {self.name}.\n"
             "URL is broken. Select another genome or provider.\n"
             f"Broken URL: {link}"
         )
@@ -1088,18 +1084,17 @@
         out_dir : str
             Output directory
 
         mask : str , optional
             masking level: soft/hard/none, default=soft
         """
         # Create mapping of accessions to names
-        genome = self.genomes[safe(name)]
-        url = genome["ftp_path"]
-        url += f"/{url.split('/')[-1]}_assembly_report.txt"
-        url = url.replace("ftp://", "https://")
+        url = self._ftp_or_html_link(
+            name, file_suffix="_assembly_report.txt", skip_check=True
+        )
 
         tr = {}
         urlcleanup()
         with urlopen(url) as response:
             for line in response.read().decode("utf-8").splitlines():
                 if line.startswith("#"):
                     continue
@@ -1144,21 +1139,29 @@
         Parse and test the link to the NCBI annotation file.
 
         Parameters
         ----------
         name : str
             Genome name
         """
+        return self._ftp_or_html_link(name, file_suffix="_genomic.gff.gz")
+
+    def _ftp_or_html_link(self, name, file_suffix, skip_check=False):
+        """
+        NCBI's files are accessible over FTP and HTTPS
+        Try HTTPS first and return the first functioning link
+        """
         genome = self.genomes[safe(name)]
-        link = genome["ftp_path"]
-        link = link.replace("ftp://", "https://")
-        link += "/" + link.split("/")[-1] + "_genomic.gff.gz"
+        ftp_link = genome["ftp_path"]
+        html_link = ftp_link.replace("ftp://", "https://")
+        for link in [html_link, ftp_link]:
+            link += "/" + link.split("/")[-1] + file_suffix
 
-        if check_url(link, 2):
-            return link
+            if skip_check or check_url(link, max_tries=2, timeout=10):
+                return link
 
 
 @register_provider("URL")
 class UrlProvider(ProviderBase):
     """
     URL genome provider.
 
@@ -1184,14 +1187,17 @@
         return "na"
 
     def search(self, term):
         """return an empty generator,
         same as if no genomes were found at the other providers"""
         yield from ()
 
+    def _genome_info_tuple(self, name):
+        return tuple()
+
     def get_genome_download_link(self, url, mask=None, **kwargs):
         return url
 
     def get_annotation_download_link(self, name, **kwargs):
         """
         check if the linked annotation file is of a supported file type (gtf/gff3/bed)
         """
@@ -1199,63 +1205,49 @@
         if link:
             ext = get_file_info(link)[0]
             if ext not in [".gtf", ".gff", ".gff3", ".bed"]:
                 raise TypeError(
                     "Only (gzipped) gtf, gff and bed files are supported.\n"
                 )
 
-            if check_url(link):
-                return link
+            return link
 
     @staticmethod
-    def search_url_for_annotation(url):
-        """Attempts to find a gtf or gff3 file in the same location as the genome url"""
+    def search_url_for_annotations(url, name):
+        """Attempts to find gtf or gff3 files in the same location as the genome url"""
         urldir = os.path.dirname(url)
         sys.stderr.write(
-            "You have requested gene annotation to be downloaded.\n"
+            "You have requested the gene annotation to be downloaded.\n"
             "Genomepy will check the remote directory:\n"
             f"{urldir} for annotation files...\n"
         )
 
-        # try to find a GTF or GFF3 file
-        name = get_localname(url)
-        with urlopen(urldir) as f:
-            for urlline in f.readlines():
-                urlstr = str(urlline)
-                if any(
-                    substring in urlstr.lower() for substring in [".gtf", name + ".gff"]
-                ):
-                    break
+        def fuzzy_annotation_search(search_name, search_list):
+            """Returns all files containing both name and an annotation extension"""
+            hits = []
+            for ext in ["gtf", "gff"]:
+                # .*? = non greedy filler. 3? = optional 3 (for gff3). (\.gz)? = optional .gz
+                expr = f"{search_name}.*?\.{ext}3?(\.gz)?"  # noqa: W605
+                for line in search_list:
+                    hit = re.search(expr, line, flags=re.IGNORECASE)
+                    if hit:
+                        hits.append(hit[0])
+            return hits
 
-        # retrieve the filename from the HTML line
-        fname = ""
-        for split in re.split('>|<|><|/|"', urlstr):
-            if split.lower().endswith(
-                (
-                    ".gtf",
-                    ".gtf.gz",
-                    name + ".gff",
-                    name + ".gff.gz",
-                    name + ".gff3",
-                    name + ".gff3.gz",
-                )
-            ):
-                fname = split
-                break
-        else:
+        # try to find a GTF or GFF3 file
+        dirty_list = [str(line) for line in urlopen(urldir).readlines()]
+        fnames = fuzzy_annotation_search(name, dirty_list)
+        if not fnames:
             raise FileNotFoundError(
                 "Could not parse the remote directory. "
                 "Please supply a URL using --url-to-annotation.\n"
             )
 
-        # set variables for downloading
-        link = urldir + "/" + fname
-
-        if check_url(link):
-            return link
+        links = [urldir + "/" + fname for fname in fnames]
+        return links
 
     def download_annotation(self, url, genomes_dir=None, localname=None, **kwargs):
         """
         Attempts to download a gtf or gff3 file from the same location as the genome url
 
         Parameters
         ----------
@@ -1275,12 +1267,24 @@
                 url to annotation file (only required if this not located in the same directory as the fasta)
         """
         name = get_localname(url)
         localname = get_localname(name, localname)
         genomes_dir = get_genomes_dir(genomes_dir, check_exist=False)
 
         if kwargs.get("to_annotation"):
-            link = self.get_annotation_download_link(None, **kwargs)
+            links = [self.get_annotation_download_link(None, **kwargs)]
         else:
-            link = self.search_url_for_annotation(url)
+            # can return multiple possible hits
+            links = self.search_url_for_annotations(url, name)
 
-        self.attempt_and_report(name, localname, link, genomes_dir)
+        for link in links:
+            try:
+                self.attempt_and_report(name, localname, link, genomes_dir)
+                break
+            except GenomeDownloadError as e:
+                if not link == links[-1]:
+                    sys.stdout.write(
+                        "\nOne of the potential annotations was incompatible with genomepy."
+                        + "\nAttempting another...\n\n"
+                    )
+                    continue
+                return e
```

### Comparing `genomepy-0.9.2/genomepy/utils.py` & `genomepy-0.9.3/genomepy/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,56 +1,96 @@
 """Utility functions."""
 import os
 import itertools
 import norns
 import re
 import sys
+import urllib.error
 import urllib.request
 import requests
 import subprocess as sp
 import tarfile
 import gzip
 import shutil
+import socket
 import time
 
+from ftplib import FTP, all_errors
 from glob import glob
 from norns import exceptions
 from pyfaidx import Fasta
-from socket import timeout
 from tqdm.auto import tqdm
 from tempfile import mkdtemp
 
+from genomepy.exceptions import GenomeDownloadError
+
 config = norns.config("genomepy", default="cfg/default.yaml")
 
 
 def download_file(url, filename):
     """
     Helper method handling downloading large files from `url` to `filename`.
-    Displays a progress bar with download speeds in MB/s.
     Returns a pointer to `filename`.
     """
-    chunk_size = 1024
-    r = requests.get(url, stream=True)
-    file_size = int(r.headers.get("Content-Length", 0))
-    with open(filename, "wb") as f:
-        pbar = tqdm(
+
+    def decorated_pbar(total):
+        """Displays a progress bar with download speeds in MB/s."""
+        return tqdm(
             desc="Download",
             unit_scale=True,
             unit_divisor=1024,
-            total=file_size,
+            total=total,
             unit="B",
-            leave=False,
         )
-        for chunk in r.iter_content(chunk_size=chunk_size):
-            if chunk:  # filter out keep-alive new chunks
-                pbar.update(len(chunk))
-                f.write(chunk)
+
+    def write_n_update_pbar(data):
+        pbar.update(len(data))
+        f.write(data)
+
+    if url.startswith("ftp"):
+        ftp, target = connect_ftp_link(url)
+        file_size = ftp.size(target)
+        with open(filename, "wb") as f:
+            pbar = decorated_pbar(file_size)
+
+            ftp.retrbinary(f"RETR {target}", write_n_update_pbar)
+            ftp.quit()  # logout
+
+    else:
+        r = requests.get(url, stream=True)
+        file_size = int(r.headers.get("Content-Length", 0))
+        with open(filename, "wb") as f:
+            pbar = decorated_pbar(file_size)
+
+            for chunk in r.iter_content(chunk_size=1024):
+                if chunk:  # filter out keep-alive new chunks
+                    write_n_update_pbar(chunk)
+
+    pbar.close()  # stop updating pbar
     return filename
 
 
+def connect_ftp_link(link, timeout=None):
+    """
+    anonymous login to ftp
+    accepts link in the form of ftp://ftp.name.domain/... and ftp.name.domain/...
+    """
+    link = link.replace("ftp://", "")
+    host = link.split("/")[0]
+    target = link.split(host)[1]
+
+    try:
+        ftp = FTP(host, timeout=timeout)
+    except socket.gaierror:
+        raise GenomeDownloadError(f"FTP host not found: {host}")
+
+    ftp.login()
+    return ftp, target
+
+
 def read_readme(readme):
     """
     parse readme file
 
     Parameters
     ----------
     readme: str
@@ -298,24 +338,37 @@
         return safe(localname)
     try:
         urllib.request.urlopen(name)
     except (IOError, ValueError):
         return safe(name)
     else:
         # try to get the name from the url
-        name = name[name.rfind("/") + 1 :]
-        name = safe(name[: name.find(".fa")])
-        # remove potential unwanted text from the name (ex: _genomes or .est_)
-        unwanted = ["genome", "sequence", "cds", "pep", "transcript", "EST"]
-        name = re.sub(
-            r"(\.?_?){}(s?\.?_?)".format("(s?\.?_?)|".join(unwanted)),  # noqa: W605
-            "",
-            name,
-            flags=re.IGNORECASE,
-        )
+        name = name.split("/")[-1]  # remove path
+        name = name.replace(".gz", "")  # remove .gz
+        name = os.path.splitext(name)[0]  # remove .fa/.fna/.fasta etc
+        name = safe(name)  # remove spaces
+        # remove unwanted substrings from the name (ex: _genomes or .est_)
+        unwanted = [
+            "genome",
+            "genomic",
+            "sequence",
+            "dna",
+            "cds",
+            "pep",
+            "transcript",
+            "EST",
+            "toplevel",
+            "primary",
+            "assembly",
+        ]
+        spacers = "(-?_?\.?)"  # noqa: W605
+        for substring in unwanted:
+            name = re.sub(
+                f"{spacers}{substring}(s?){spacers}", "", name, flags=re.IGNORECASE
+            )
         return name
 
 
 def tar_to_bigfile(fname, outfile):
     """Convert tar of multiple FASTAs to one file."""
     fnames = []
     # Extract files to temporary directory
@@ -396,29 +449,39 @@
     *args are passed as variables to func.
     """
     _try = 1
     while _try <= tries:
         try:
             answer = func(*args)
             return answer
-        except (urllib.request.URLError, timeout):
+        except (urllib.error.URLError, socket.timeout):
             time.sleep(1)
             _try += 1
 
 
-def check_url(url, max_tries=1, time_out=15):
+def check_url(url, max_tries=1, timeout=15):
     """Check if URL works. Returns bool"""
 
-    def _check_url(_url=url, _time_out=time_out):
-        ret = urllib.request.urlopen(_url, timeout=_time_out)
-        # check return code for http(s) urls
-        if _url.startswith("ftp") or ret.getcode() == 200:
-            return True
+    def _check_url(_url, _timeout):
+        if _url.startswith("ftp"):
+            ftp, target = connect_ftp_link(_url, timeout=_timeout)
+            try:
+                listing = ftp.nlst(target)
+            except all_errors:
+                listing = []
+            ftp.quit()  # logout
+            if listing:
+                return True
+        else:
+            ret = urllib.request.urlopen(_url, timeout=_timeout)
+            if ret.getcode() == 200:
+                return True
+        return False
 
-    return retry(_check_url, max_tries, url, time_out)
+    return retry(_check_url, max_tries, url, timeout)
 
 
 def read_url(url):
     """Read a text-based URL."""
     response = urllib.request.urlopen(url)
     data = response.read()
     text = data.decode("utf-8")
```

### Comparing `genomepy-0.9.2/genomepy.egg-info/PKG-INFO` & `genomepy-0.9.3/genomepy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: genomepy
-Version: 0.9.2
+Version: 0.9.3
 Summary: Automatic downloading and processing of genomes and metadata in command line and Python
 Home-page: https://github.com/vanheeringen-lab/genomepy
 Author: Simon van Heeringen
 Author-email: simon.vanheeringen@gmail.com
 License: MIT
 Description: # genomepy
```

### Comparing `genomepy-0.9.2/genomepy.egg-info/SOURCES.txt` & `genomepy-0.9.3/genomepy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `genomepy-0.9.2/setup.py` & `genomepy-0.9.3/setup.py`

 * *Files identical despite different names*

