# Comparing `tmp/PRauto-0.213.tar.gz` & `tmp/PRauto-0.214.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PRauto-0.213.tar", last modified: Mon Jun 12 05:13:51 2023, max compression
+gzip compressed data, was "PRauto-0.214.tar", last modified: Wed Jun 14 05:58:51 2023, max compression
```

## Comparing `PRauto-0.213.tar` & `PRauto-0.214.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-06-12 05:13:51.029045 PRauto-0.213/
--rw-rw-rw-   0        0        0     1098 2023-04-18 06:21:00.000000 PRauto-0.213/LICENSE
--rw-rw-rw-   0        0        0      349 2023-06-12 05:13:51.029045 PRauto-0.213/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-12 05:13:51.003719 PRauto-0.213/PRauto.egg-info/
--rw-rw-rw-   0        0        0      349 2023-06-12 05:13:50.000000 PRauto-0.213/PRauto.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      416 2023-06-12 05:13:50.000000 PRauto-0.213/PRauto.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-12 05:13:50.000000 PRauto-0.213/PRauto.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      125 2023-06-12 05:13:50.000000 PRauto-0.213/PRauto.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-06-12 05:13:50.000000 PRauto-0.213/PRauto.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2604 2023-06-05 02:04:20.000000 PRauto-0.213/README.md
-drwxrwxrwx   0        0        0        0 2023-06-12 05:13:51.005718 PRauto-0.213/prauto/
--rw-rw-rw-   0        0        0        0 2023-04-17 00:34:40.000000 PRauto-0.213/prauto/__init__.py
--rw-rw-rw-   0        0        0     3501 2023-06-12 05:08:39.000000 PRauto-0.213/prauto/__main__.py
-drwxrwxrwx   0        0        0        0 2023-06-12 05:13:51.013718 PRauto-0.213/prauto/prepauto/
--rw-rw-rw-   0        0        0        0 2023-04-19 01:47:21.000000 PRauto-0.213/prauto/prepauto/__init__.py
--rw-rw-rw-   0        0        0    14202 2023-05-10 05:53:19.000000 PRauto-0.213/prauto/prepauto/__main__.py
-drwxrwxrwx   0        0        0        0 2023-06-12 05:13:51.027047 PRauto-0.213/prauto/retriever/
--rw-rw-rw-   0        0        0        0 2023-04-17 00:31:39.000000 PRauto-0.213/prauto/retriever/__init__.py
--rw-rw-rw-   0        0        0     3064 2023-06-05 02:01:33.000000 PRauto-0.213/prauto/retriever/__main__.py
--rw-rw-rw-   0        0        0     4848 2023-04-18 07:55:44.000000 PRauto-0.213/prauto/retriever/get_fasta.py
--rw-rw-rw-   0        0        0     7842 2023-06-07 08:27:19.000000 PRauto-0.213/prauto/retriever/get_ligand.py
--rw-rw-rw-   0        0        0     4276 2023-04-26 06:35:58.000000 PRauto-0.213/prauto/retriever/get_pdb.py
--rw-rw-rw-   0        0        0       42 2023-06-12 05:13:51.029045 PRauto-0.213/setup.cfg
--rw-rw-rw-   0        0        0     1250 2023-06-12 05:10:11.000000 PRauto-0.213/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-14 05:58:51.837493 PRauto-0.214/
+-rw-rw-rw-   0        0        0     1098 2023-04-18 06:21:00.000000 PRauto-0.214/LICENSE
+-rw-rw-rw-   0        0        0      349 2023-06-14 05:58:51.836496 PRauto-0.214/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-14 05:58:51.803492 PRauto-0.214/PRauto.egg-info/
+-rw-rw-rw-   0        0        0      349 2023-06-14 05:58:51.000000 PRauto-0.214/PRauto.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      416 2023-06-14 05:58:51.000000 PRauto-0.214/PRauto.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-14 05:58:51.000000 PRauto-0.214/PRauto.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      125 2023-06-14 05:58:51.000000 PRauto-0.214/PRauto.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-14 05:58:51.000000 PRauto-0.214/PRauto.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2604 2023-06-05 02:04:20.000000 PRauto-0.214/README.md
+drwxrwxrwx   0        0        0        0 2023-06-14 05:58:51.807521 PRauto-0.214/prauto/
+-rw-rw-rw-   0        0        0        0 2023-04-17 00:34:40.000000 PRauto-0.214/prauto/__init__.py
+-rw-rw-rw-   0        0        0     3501 2023-06-12 05:08:39.000000 PRauto-0.214/prauto/__main__.py
+drwxrwxrwx   0        0        0        0 2023-06-14 05:58:51.810494 PRauto-0.214/prauto/prepauto/
+-rw-rw-rw-   0        0        0        0 2023-04-19 01:47:21.000000 PRauto-0.214/prauto/prepauto/__init__.py
+-rw-rw-rw-   0        0        0    14483 2023-06-13 02:25:28.000000 PRauto-0.214/prauto/prepauto/__main__.py
+drwxrwxrwx   0        0        0        0 2023-06-14 05:58:51.834492 PRauto-0.214/prauto/retriever/
+-rw-rw-rw-   0        0        0        0 2023-04-17 00:31:39.000000 PRauto-0.214/prauto/retriever/__init__.py
+-rw-rw-rw-   0        0        0     3064 2023-06-05 02:01:33.000000 PRauto-0.214/prauto/retriever/__main__.py
+-rw-rw-rw-   0        0        0     4848 2023-04-18 07:55:44.000000 PRauto-0.214/prauto/retriever/get_fasta.py
+-rw-rw-rw-   0        0        0     7842 2023-06-07 08:27:19.000000 PRauto-0.214/prauto/retriever/get_ligand.py
+-rw-rw-rw-   0        0        0     4276 2023-04-26 06:35:58.000000 PRauto-0.214/prauto/retriever/get_pdb.py
+-rw-rw-rw-   0        0        0       42 2023-06-14 05:58:51.838490 PRauto-0.214/setup.cfg
+-rw-rw-rw-   0        0        0     1250 2023-06-14 05:55:54.000000 PRauto-0.214/setup.py
```

### Comparing `PRauto-0.213/LICENSE` & `PRauto-0.214/LICENSE`

 * *Files identical despite different names*

### Comparing `PRauto-0.213/README.md` & `PRauto-0.214/README.md`

 * *Files identical despite different names*

### Comparing `PRauto-0.213/prauto/__main__.py` & `PRauto-0.214/prauto/__main__.py`

 * *Files identical despite different names*

### Comparing `PRauto-0.213/prauto/prepauto/__main__.py` & `PRauto-0.214/prauto/prepauto/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,26 +58,27 @@
             target_chain = []
             for keys in current_data.keys():
                 if current_data[keys]['db_id'].split('_')[0] == target_id:
                     target_chain.append(current_data[keys]['chain'])
             target_chain_ids = list(set(target_chain))
             print(f"{os.path.basename(pdb_file).replace('.pdb', '')}'s target chains : ", target_chain_ids)
             if len(target_chain_ids) == 0 :
-                for chain in structure.get_chains():
-                    # Get the ID of the chain and check if it should be saved
-                    chain_id = chain.get_id()
-                    output_file = os.path.join(output_dir,
-                                               f"{os.path.basename(pdb_file).replace('.pdb', '')}_{chain_id}_not_matched.pdb")
-                    print(f"{os.path.basename(output_file)} extraction completed")
-                    # Save the separated chain to a PDB file
-                    io = PDBIO()
-                    io.set_structure(chain)
-                    if not os.path.exists(os.path.dirname(output_file)):
-                        os.makedirs(os.path.dirname(output_file))
-                    io.save(output_file)
+                pass
+            #     for chain in structure.get_chains():
+            #         # Get the ID of the chain and check if it should be saved
+            #         chain_id = chain.get_id()
+            #         output_file = os.path.join(output_dir,
+            #                                    f"{os.path.basename(pdb_file).replace('.pdb', '')}_{chain_id}_not_matched.pdb")
+            #         print(f"{os.path.basename(output_file)} extraction completed")
+            #         # Save the separated chain to a PDB file
+            #         io = PDBIO()
+            #         io.set_structure(chain)
+            #         if not os.path.exists(os.path.dirname(output_file)):
+            #             os.makedirs(os.path.dirname(output_file))
+            #         io.save(output_file)
 
             else:
                 for chain in structure.get_chains():
                     # Get the ID of the chain and check if it should be saved
                     chain_id = chain.get_id()
                     if chain_id in target_chain_ids:
                         output_file = os.path.join(output_dir,
@@ -201,16 +202,21 @@
                     rm_start = data['pdb_start']
                     rm_end = data['pdb_end']
                     if (rm_start - rm_end) > 0:
                         print(f'Wrong DBREF data: {pdb_file} , Check resi {rm_start}-{rm_end}')
                         save = 0
                     pymol.cmd.remove(f"(chain {rm_chain} and resi {rm_start}-{rm_end})")
                     print(f"{pdb_file}, resi{rm_start}-{rm_end} has been removed")
+            except:
+                pass
 
-            except: pass
+            # try:
+            #     pymol.cmd.remove("(resi 1000-* and not hetatm)")
+            # except:
+            #     pass
 
             try:
                 for data in renumber_dict[name_for_dict]:
                     rn_chain = data['chain']
                     rn_start = data['pdb_start']
                     rn_end = data['pdb_end']
                     un_start = data['uniprot_start']
@@ -227,14 +233,15 @@
 
                         print(f"{pdb_file}, resi{rn_start}-{rn_end} has been renumbered")
 
             except:
                 print(pdb_file, 'renumber error')
                 pass
 
+
             # Align the pdb file to the reference pdb file
             pymol.cmd.align(pdb_file[:-4], 'ref')
 
             pymol.cmd.origin('ref')
             pymol.cmd.zoom("all", 0.8)
             #
             # Remove the organic and solvent
@@ -298,21 +305,24 @@
 
     # Extract the chains from the input PDB files that match the molecules in the reference PDB file
     remove_dict, renumber_dict = extract_target_chains(pdb_files, target_id, output_dir)
     print('remove_dict: ',remove_dict)
     print('\n' * 7)
     print('###########  Target chains extraction Complete  ###########'+'\n' * 2)
     print('Step 2: Start preprocessing with pymol'+'\n' * 8)
-    align_ref = filedialog.askopenfilename(title='Select the file you want to use as the align criteria',initialdir=output_dir)
+    align_ref = filedialog.askopenfilename(title='Select the file you want to use as the align criteria', initialdir=output_dir)
 
-    with open(os.path.join(align_ref), 'r') as f:
-        ligand_menu = []
+    with open(os.path.join(ref_pdb_file), 'r') as f:
         for line in f:
             if line.startswith('HETNAM'):
                 print(line)
+
+    with open(os.path.join(align_ref), 'r') as f:
+        ligand_menu = []
+        for line in f:
             if line.startswith('HETATM'):
                 ligand_menu.append(line[17:20].replace(' ', ''))
         print(list(set(ligand_menu)))
 
     ligand_name = input("Enter ligand name: ")
     print('\n' * 1)
     ligand_range = input("Range around the ligand you do not want to delete(Å): ")
```

### Comparing `PRauto-0.213/prauto/retriever/__main__.py` & `PRauto-0.214/prauto/retriever/__main__.py`

 * *Files identical despite different names*

### Comparing `PRauto-0.213/prauto/retriever/get_fasta.py` & `PRauto-0.214/prauto/retriever/get_fasta.py`

 * *Files identical despite different names*

### Comparing `PRauto-0.213/prauto/retriever/get_ligand.py` & `PRauto-0.214/prauto/retriever/get_ligand.py`

 * *Files identical despite different names*

### Comparing `PRauto-0.213/prauto/retriever/get_pdb.py` & `PRauto-0.214/prauto/retriever/get_pdb.py`

 * *Files identical despite different names*

### Comparing `PRauto-0.213/setup.py` & `PRauto-0.214/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 from setuptools import setup, find_packages, Extension
 import setuptools
 with open('requirements.txt') as f:
     required = f.read().splitlines()
 
 setuptools.setup(name='PRauto',
-        version = '0.213',
+        version = '0.214',
         packages = find_packages(include=['prauto','prauto.*']),
         url = 'https://github.com/KimJisanER/PRauto',
         license = 'MIT license',
         author = 'Ji San Kim',
         author_email = 'jisan1233@gmail.com',
         keywords = 'PDB, FASTA, sdf, Automation',
         description = """
```

