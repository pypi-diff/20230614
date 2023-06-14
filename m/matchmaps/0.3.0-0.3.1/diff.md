# Comparing `tmp/matchmaps-0.3.0.tar.gz` & `tmp/matchmaps-0.3.1.tar.gz`

## Comparing `matchmaps-0.3.0.tar` & `matchmaps-0.3.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 matchmaps-0.3.0/.github_changelog_generator
--rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 matchmaps-0.3.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 matchmaps-0.3.0/setup.py
--rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 matchmaps-0.3.0/tox.ini
--rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 matchmaps-0.3.0/.github/ISSUE_TEMPLATE.md
--rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 matchmaps-0.3.0/.github/TEST_FAIL_TEMPLATE.md
--rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 matchmaps-0.3.0/.github/dependabot.yml
--rw-r--r--   0        0        0     1394 2020-02-02 00:00:00.000000 matchmaps-0.3.0/.github/workflows/build_docs.yml
--rw-r--r--   0        0        0     1771 2020-02-02 00:00:00.000000 matchmaps-0.3.0/.github/workflows/ci.yml
--rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 matchmaps-0.3.0/.github/workflows/cron.yml
--rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 matchmaps-0.3.0/docs/Makefile
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 matchmaps-0.3.0/docs/about.md
--rw-r--r--   0        0        0      489 2020-02-02 00:00:00.000000 matchmaps-0.3.0/docs/cli.md
--rw-r--r--   0        0        0     6252 2020-02-02 00:00:00.000000 matchmaps-0.3.0/docs/conf.py
--rw-r--r--   0        0        0     2434 2020-02-02 00:00:00.000000 matchmaps-0.3.0/docs/index.md
--rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 matchmaps-0.3.0/docs/make.bat
--rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 matchmaps-0.3.0/docs/_static/custom.css
--rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 matchmaps-0.3.0/src/matchmaps/__init__.py
--rw-r--r--   0        0        0    13894 2020-02-02 00:00:00.000000 matchmaps-0.3.0/src/matchmaps/_compute_mr_diff.py
--rw-r--r--   0        0        0     7530 2020-02-02 00:00:00.000000 matchmaps-0.3.0/src/matchmaps/_compute_ncs_diff.py
--rwxr-xr-x   0        0        0    12085 2020-02-02 00:00:00.000000 matchmaps-0.3.0/src/matchmaps/_compute_realspace_diff.py
--rw-r--r--   0        0        0    26050 2020-02-02 00:00:00.000000 matchmaps-0.3.0/src/matchmaps/_utils.py
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 matchmaps-0.3.0/tests/test_matchmaps.py
--rw-r--r--   0        0        0     1269 2020-02-02 00:00:00.000000 matchmaps-0.3.0/.gitignore
--rw-r--r--   0        0        0     1514 2020-02-02 00:00:00.000000 matchmaps-0.3.0/LICENSE
--rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 matchmaps-0.3.0/README.md
--rw-r--r--   0        0        0     5565 2020-02-02 00:00:00.000000 matchmaps-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     2366 2020-02-02 00:00:00.000000 matchmaps-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 matchmaps-0.3.1/.github_changelog_generator
+-rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 matchmaps-0.3.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 matchmaps-0.3.1/setup.py
+-rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 matchmaps-0.3.1/tox.ini
+-rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 matchmaps-0.3.1/.github/ISSUE_TEMPLATE.md
+-rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 matchmaps-0.3.1/.github/TEST_FAIL_TEMPLATE.md
+-rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 matchmaps-0.3.1/.github/dependabot.yml
+-rw-r--r--   0        0        0     1394 2020-02-02 00:00:00.000000 matchmaps-0.3.1/.github/workflows/build_docs.yml
+-rw-r--r--   0        0        0     1771 2020-02-02 00:00:00.000000 matchmaps-0.3.1/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 matchmaps-0.3.1/.github/workflows/cron.yml
+-rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 matchmaps-0.3.1/docs/Makefile
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 matchmaps-0.3.1/docs/about.md
+-rw-r--r--   0        0        0      489 2020-02-02 00:00:00.000000 matchmaps-0.3.1/docs/cli.md
+-rw-r--r--   0        0        0     6252 2020-02-02 00:00:00.000000 matchmaps-0.3.1/docs/conf.py
+-rw-r--r--   0        0        0     2434 2020-02-02 00:00:00.000000 matchmaps-0.3.1/docs/index.md
+-rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 matchmaps-0.3.1/docs/make.bat
+-rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 matchmaps-0.3.1/docs/_static/custom.css
+-rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 matchmaps-0.3.1/src/matchmaps/__init__.py
+-rw-r--r--   0        0        0    13918 2020-02-02 00:00:00.000000 matchmaps-0.3.1/src/matchmaps/_compute_mr_diff.py
+-rw-r--r--   0        0        0     7530 2020-02-02 00:00:00.000000 matchmaps-0.3.1/src/matchmaps/_compute_ncs_diff.py
+-rwxr-xr-x   0        0        0    12085 2020-02-02 00:00:00.000000 matchmaps-0.3.1/src/matchmaps/_compute_realspace_diff.py
+-rw-r--r--   0        0        0    26064 2020-02-02 00:00:00.000000 matchmaps-0.3.1/src/matchmaps/_utils.py
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 matchmaps-0.3.1/tests/test_matchmaps.py
+-rw-r--r--   0        0        0     1269 2020-02-02 00:00:00.000000 matchmaps-0.3.1/.gitignore
+-rw-r--r--   0        0        0     1514 2020-02-02 00:00:00.000000 matchmaps-0.3.1/LICENSE
+-rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 matchmaps-0.3.1/README.md
+-rw-r--r--   0        0        0     5565 2020-02-02 00:00:00.000000 matchmaps-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     2366 2020-02-02 00:00:00.000000 matchmaps-0.3.1/PKG-INFO
```

### Comparing `matchmaps-0.3.0/.pre-commit-config.yaml` & `matchmaps-0.3.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `matchmaps-0.3.0/setup.py` & `matchmaps-0.3.1/setup.py`

 * *Files identical despite different names*

### Comparing `matchmaps-0.3.0/tox.ini` & `matchmaps-0.3.1/tox.ini`

 * *Files identical despite different names*

### Comparing `matchmaps-0.3.0/.github/workflows/build_docs.yml` & `matchmaps-0.3.1/.github/workflows/build_docs.yml`

 * *Files identical despite different names*

### Comparing `matchmaps-0.3.0/.github/workflows/ci.yml` & `matchmaps-0.3.1/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `matchmaps-0.3.0/.github/workflows/cron.yml` & `matchmaps-0.3.1/.github/workflows/cron.yml`

 * *Files identical despite different names*

### Comparing `matchmaps-0.3.0/docs/Makefile` & `matchmaps-0.3.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `matchmaps-0.3.0/docs/conf.py` & `matchmaps-0.3.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `matchmaps-0.3.0/docs/index.md` & `matchmaps-0.3.1/docs/index.md`

 * *Files identical despite different names*

### Comparing `matchmaps-0.3.0/docs/make.bat` & `matchmaps-0.3.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `matchmaps-0.3.0/src/matchmaps/_compute_mr_diff.py` & `matchmaps-0.3.1/src/matchmaps/_compute_mr_diff.py`

 * *Files 1% similar despite different names*

```diff
@@ -122,16 +122,16 @@
         eff=None,
         verbose=verbose,
     )
 
     # TO-DO: fix ligand occupancies in pdb_mr_to_on
     edited_mr_pdb = _restore_ligand_occupancy(
         pdb_to_be_restored=phaser_nickname + ".1.pdb",
-        # original_pdb=pdboff,
-        ligands=ligands,
+        original_pdb=pdboff,
+        # ligands=ligands,
         output_dir=output_dir,
     )
 
     # the refinement process *should* be identical. Waters are gone already
     # I just need to make sure that the phaser outputs go together
     print(f"{time.strftime('%H:%M:%S')}: Running phenix.refine for the 'on' data...")
 
@@ -141,14 +141,15 @@
         input_dir=input_dir,
         output_dir=output_dir,
         ligands=ligands,
         eff=eff,
         verbose=verbose,
         rbr_selections=rbr_phenix,
         off_labels=f"{Fon},{SigFon}",  # workaround for compatibility
+        mr_naming=True,
     )
 
     print(f"{time.strftime('%H:%M:%S')}: Running phenix.refine for the 'off' data...")
 
     nickname_off = rigid_body_refinement_wrapper(
         mtzon=mtzoff,
         pdboff=pdboff,
```

### Comparing `matchmaps-0.3.0/src/matchmaps/_compute_ncs_diff.py` & `matchmaps-0.3.1/src/matchmaps/_compute_ncs_diff.py`

 * *Files identical despite different names*

### Comparing `matchmaps-0.3.0/src/matchmaps/_compute_realspace_diff.py` & `matchmaps-0.3.1/src/matchmaps/_compute_realspace_diff.py`

 * *Files identical despite different names*

### Comparing `matchmaps-0.3.0/src/matchmaps/_utils.py` & `matchmaps-0.3.1/src/matchmaps/_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -157,14 +157,15 @@
     input_dir,
     output_dir,
     off_labels=None,
     ligands=None,
     eff=None,
     verbose=False,
     rbr_selections=None,
+    mr_naming=False,
 ):
     # confirm that phenix is active in the command-line environment
     if shutil.which("phenix.refine") is None:
         raise OSError(
             "Cannot find executable, phenix.refine. Please set up your phenix environment."
         )
 
@@ -219,15 +220,15 @@
   }
 }
     """
     else:
         with open(input_dir + eff) as file:
             eff_contents = file.read()
 
-    if off_labels is None:
+    if (off_labels is None) or (mr_naming):
         nickname = f"{mtzon.removesuffix('.mtz')}_rbr_to_{pdboff.removesuffix('.pdb')}"
     else:
         nickname = f"{mtzon.removesuffix('.mtz')}_rbr_to_self"
 
     # check existing files because phenix doesn't like to overwrite things
 
     # number = _find_available_suffix(prefix=f"{output_dir}/{nickname}_", suffix='_1.*')
@@ -531,15 +532,14 @@
 
     with open(output_dir + pdb_to_be_restored, "r") as p:
         pdb = p.readlines()
     pdb_hetatm = []
     n = 0
     for i in range(len(pdb)):
         if ("HETATM" in pdb[i]) and (not "REMARK" in pdb[i]):
-            print(i, n)
             pdb[i] = pdb[i][:56] + original_occs[n] + pdb[i][60:]
             n += 1
 
     edited_pdb = original_pdb.removesuffix(".pdb") + "_restorehetatms.pdb"
 
     with open(output_dir + edited_pdb, "w") as output:
         output.write("".join(pdb))
```

### Comparing `matchmaps-0.3.0/.gitignore` & `matchmaps-0.3.1/.gitignore`

 * *Files identical despite different names*

### Comparing `matchmaps-0.3.0/LICENSE` & `matchmaps-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `matchmaps-0.3.0/README.md` & `matchmaps-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `matchmaps-0.3.0/pyproject.toml` & `matchmaps-0.3.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `matchmaps-0.3.0/PKG-INFO` & `matchmaps-0.3.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: matchmaps
-Version: 0.3.0
+Version: 0.3.1
 Summary: Make unbiased difference maps even for non-isomorphous inputs
 Project-URL: homepage, https://dennisbrookner.github.io/matchmaps/
 Project-URL: repository, https://github.com/dennisbrookner/matchmaps
 Author-email: Dennis Brookner <debrookner@gmail.com>
 License: BSD 3-Clause License
 License-File: LICENSE
 Classifier: Development Status :: 3 - Alpha
```

