# Comparing `tmp/omamer-0.2.5.tar.gz` & `tmp/omamer-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "omamer-0.2.5.tar", last modified: Tue Mar 21 15:30:51 2023, max compression
+gzip compressed data, was "omamer-0.2.6.tar", last modified: Wed Jun 14 07:44:43 2023, max compression
```

## Comparing `omamer-0.2.5.tar` & `omamer-0.2.6.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 15:30:51.628071 omamer-0.2.5/
--rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-03-21 15:30:39.000000 omamer-0.2.5/COPYING
--rw-r--r--   0 runner    (1001) docker     (123)     7651 2023-03-21 15:30:39.000000 omamer-0.2.5/COPYING.LESSER
--rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-03-21 15:30:39.000000 omamer-0.2.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-03-21 15:30:51.628071 omamer-0.2.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8916 2023-03-21 15:30:39.000000 omamer-0.2.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 15:30:51.628071 omamer-0.2.5/bin/
--rwxr-xr-x   0 runner    (1001) docker     (123)     7412 2023-03-21 15:30:39.000000 omamer-0.2.5/bin/omamer
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 15:30:51.628071 omamer-0.2.5/omamer/
--rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-03-21 15:30:39.000000 omamer-0.2.5/omamer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5294 2023-03-21 15:30:39.000000 omamer-0.2.5/omamer/_runners.py
--rw-r--r--   0 runner    (1001) docker     (123)    23808 2023-03-21 15:30:39.000000 omamer-0.2.5/omamer/_runners_axiom.py
--rw-r--r--   0 runner    (1001) docker     (123)    23379 2023-03-21 15:30:39.000000 omamer-0.2.5/omamer/_runners_curnagl.py
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-03-21 15:30:39.000000 omamer-0.2.5/omamer/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3520 2023-03-21 15:30:39.000000 omamer-0.2.5/omamer/alphabets.py
--rw-r--r--   0 runner    (1001) docker     (123)    25228 2023-03-21 15:30:39.000000 omamer-0.2.5/omamer/benchmark.py
--rw-r--r--   0 runner    (1001) docker     (123)    70677 2023-03-21 15:30:39.000000 omamer-0.2.5/omamer/database.py
--rw-r--r--   0 runner    (1001) docker     (123)    11809 2023-03-21 15:30:39.000000 omamer-0.2.5/omamer/hierarchy.py
--rw-r--r--   0 runner    (1001) docker     (123)    16613 2023-03-21 15:30:39.000000 omamer-0.2.5/omamer/index.py
--rw-r--r--   0 runner    (1001) docker     (123)    83399 2023-03-21 15:30:39.000000 omamer-0.2.5/omamer/merge_search.py
--rw-r--r--   0 runner    (1001) docker     (123)    12158 2023-03-21 15:30:39.000000 omamer-0.2.5/omamer/omamer2matreex.py
--rw-r--r--   0 runner    (1001) docker     (123)    37405 2023-03-21 15:30:39.000000 omamer-0.2.5/omamer/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 15:30:51.628071 omamer-0.2.5/omamer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-03-21 15:30:51.000000 omamer-0.2.5/omamer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-03-21 15:30:51.000000 omamer-0.2.5/omamer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-21 15:30:51.000000 omamer-0.2.5/omamer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-03-21 15:30:51.000000 omamer-0.2.5/omamer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-03-21 15:30:51.000000 omamer-0.2.5/omamer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-03-21 15:30:51.632071 omamer-0.2.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-03-21 15:30:39.000000 omamer-0.2.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 07:44:43.501456 omamer-0.2.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-06-14 07:44:33.000000 omamer-0.2.6/COPYING
+-rw-r--r--   0 runner    (1001) docker     (123)     7651 2023-06-14 07:44:33.000000 omamer-0.2.6/COPYING.LESSER
+-rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-06-14 07:44:33.000000 omamer-0.2.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-06-14 07:44:43.501456 omamer-0.2.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8961 2023-06-14 07:44:33.000000 omamer-0.2.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 07:44:43.501456 omamer-0.2.6/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7412 2023-06-14 07:44:33.000000 omamer-0.2.6/bin/omamer
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 07:44:43.501456 omamer-0.2.6/omamer/
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-06-14 07:44:33.000000 omamer-0.2.6/omamer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5294 2023-06-14 07:44:33.000000 omamer-0.2.6/omamer/_runners.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23808 2023-06-14 07:44:33.000000 omamer-0.2.6/omamer/_runners_axiom.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23379 2023-06-14 07:44:33.000000 omamer-0.2.6/omamer/_runners_curnagl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-06-14 07:44:33.000000 omamer-0.2.6/omamer/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3520 2023-06-14 07:44:33.000000 omamer-0.2.6/omamer/alphabets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25228 2023-06-14 07:44:33.000000 omamer-0.2.6/omamer/benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (123)    70677 2023-06-14 07:44:33.000000 omamer-0.2.6/omamer/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11809 2023-06-14 07:44:33.000000 omamer-0.2.6/omamer/hierarchy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16614 2023-06-14 07:44:33.000000 omamer-0.2.6/omamer/index.py
+-rw-r--r--   0 runner    (1001) docker     (123)    83411 2023-06-14 07:44:33.000000 omamer-0.2.6/omamer/merge_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12158 2023-06-14 07:44:33.000000 omamer-0.2.6/omamer/omamer2matreex.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37413 2023-06-14 07:44:33.000000 omamer-0.2.6/omamer/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 07:44:43.501456 omamer-0.2.6/omamer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-06-14 07:44:43.000000 omamer-0.2.6/omamer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-06-14 07:44:43.000000 omamer-0.2.6/omamer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 07:44:43.000000 omamer-0.2.6/omamer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-14 07:44:43.000000 omamer-0.2.6/omamer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-14 07:44:43.000000 omamer-0.2.6/omamer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-06-14 07:44:43.505456 omamer-0.2.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-06-14 07:44:33.000000 omamer-0.2.6/setup.py
```

### Comparing `omamer-0.2.5/COPYING` & `omamer-0.2.6/COPYING`

 * *Files identical despite different names*

### Comparing `omamer-0.2.5/COPYING.LESSER` & `omamer-0.2.6/COPYING.LESSER`

 * *Files identical despite different names*

### Comparing `omamer-0.2.5/LICENSE` & `omamer-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `omamer-0.2.5/README.md` & `omamer-0.2.6/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -92,14 +92,17 @@
 The OMAmer-score of the predicted HOG. At the subfamily level, this score captures the excess of similarity that is shared between the query and a given HOG, thus excluding the similarity with regions conserved in more ancestral HOGs.
 
 #### Subfamily gene set
 Extant gene IDs of predicted HOG, which you can look for in the OMA browser search bar or its REST API (https://omabrowser.org/api/docs). 
 
 # Change log
 
+#### Version 0.2.6
+- support for numpy>1.23
+
 #### Version 0.2.5
  - Fixes an issue when storing the pre-conputed statistics
 
 #### Version 0.2.4
  - Improved loading time for standard search by pre-computing statistics
  - Adding new command line option "info" to show the metadata of the 
    dataset used to build the omamer database.
```

### Comparing `omamer-0.2.5/bin/omamer` & `omamer-0.2.6/bin/omamer`

 * *Files identical despite different names*

### Comparing `omamer-0.2.5/omamer/__init__.py` & `omamer-0.2.6/omamer/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,11 +18,11 @@
 
     You should have received a copy of the GNU Lesser General Public License
     along with OMAmer. If not, see <http://www.gnu.org/licenses/>.
 '''
 from datetime import date
 
 __packagename__ = "omamer"
-__version__ = "0.2.5"
+__version__ = "0.2.6"
 __copyright__ = "(C) 2019-{:d} Victor Rossier <victor.rossier@unil.ch> and Alex Warwick Vesztrocy <alex@warwickvesztrocy.co.uk>".format(
     date.today().year
 )
```

### Comparing `omamer-0.2.5/omamer/_runners.py` & `omamer-0.2.6/omamer/_runners.py`

 * *Files identical despite different names*

### Comparing `omamer-0.2.5/omamer/_runners_axiom.py` & `omamer-0.2.6/omamer/_runners_axiom.py`

 * *Files identical despite different names*

### Comparing `omamer-0.2.5/omamer/_runners_curnagl.py` & `omamer-0.2.6/omamer/_runners_curnagl.py`

 * *Files identical despite different names*

### Comparing `omamer-0.2.5/omamer/_utils.py` & `omamer-0.2.6/omamer/_utils.py`

 * *Files identical despite different names*

### Comparing `omamer-0.2.5/omamer/alphabets.py` & `omamer-0.2.6/omamer/alphabets.py`

 * *Files identical despite different names*

### Comparing `omamer-0.2.5/omamer/benchmark.py` & `omamer-0.2.6/omamer/benchmark.py`

 * *Files identical despite different names*

### Comparing `omamer-0.2.5/omamer/database.py` & `omamer-0.2.6/omamer/database.py`

 * *Files identical despite different names*

### Comparing `omamer-0.2.5/omamer/hierarchy.py` & `omamer-0.2.6/omamer/hierarchy.py`

 * *Files identical despite different names*

### Comparing `omamer-0.2.5/omamer/index.py` & `omamer-0.2.6/omamer/index.py`

 * *Files 0% similar despite different names*

```diff
@@ -283,15 +283,15 @@
             # fill until the end
             table_idx[kk:] = ii_table_buff
             return ii_table_buff
 
         LOG.debug(" - filter suffix array and compute its HOG mask")
         n = len(self.db._prot_tab)
         sa_mask = np.zeros(sa.shape, dtype=np.uint64)
-        sa_filter = np.zeros(sa.shape, dtype=np.bool)
+        sa_filter = np.zeros(sa.shape, dtype=np.bool8)
 
         _compute_mask_and_filter(
             sa,
             sa_mask,
             sa_filter,
             self.k,
             n,
```

### Comparing `omamer-0.2.5/omamer/merge_search.py` & `omamer-0.2.6/omamer/merge_search.py`

 * *Files 0% similar despite different names*

```diff
@@ -1022,26 +1022,26 @@
 
             # update best score
             if ss > best_s:
                 best_s = ss
 
             # stop if subfamily implies the true taxon
             if true_tax_off is not None:
-                hog_off = np.int(root_hog_off + j)
+                hog_off = np.int64(root_hog_off + j)
                 if is_taxon_implied(true_tax_lineage, hog_off, hog_tab, chog_buff):
                     break
                 #hog_taxa = get_hog_taxon_levels(hog_off, hog_tab, hog_taxa_buff)
                 #if np.argwhere(hog_taxa == true_tax_off).size == 1:
                 #    break
 
         # skip if no subfamily-score > subfamily-score threshold or if best subfamily-score < family-score threshold
         if (best_j is None) or (best_s < fst):
             continue
 
-        q2hog_off[i] = np.int(best_j + root_hog_off)
+        q2hog_off[i] = np.int64(best_j + root_hog_off)
         q2hog_score[i] = ss
         q2max_hog_score[i] = best_s
 
     return q2hog_off, q2hog_score, q2max_hog_score
 
 #@numba.njit
 #def get_closest_taxa_from_ref(q2hog_off, ref_taxoff, tax_tab, hog_tab, hog_taxa_buff):
@@ -1424,15 +1424,15 @@
             # get a flag for k-mer with any X (= last k-mer + 1)
             x_flag = table_idx.size - 1
 
             # iterate of sequences
             for zz in numba.prange(len(seqs_idx) - 1):
 
                 ## get the query sequence
-                s = seqs[seqs_idx[zz] : np.int(seqs_idx[zz + 1] - 1)]
+                s = seqs[seqs_idx[zz] : np.int64(seqs_idx[zz + 1] - 1)]
                 query_len = s.shape[0]
                 n_kmers = query_len - (k - 1)
 
                 # double check we don't have short peptides (of len < k)
                 # note: written in this order to provide loop-optimisation hint (?)
                 if n_kmers > 0:
                     pass
@@ -1553,15 +1553,15 @@
             # get a flag for k-mer with any X (= last k-mer + 1)
             x_flag = table_idx.size - 1
 
             # iterate of sequences
             for zz in numba.prange(len(seqs_idx) - 1):
 
                 ## get the query sequence
-                s = seqs[seqs_idx[zz] : np.int(seqs_idx[zz + 1] - 1)]
+                s = seqs[seqs_idx[zz] : np.int64(seqs_idx[zz + 1] - 1)]
                 query_len = s.shape[0]
                 n_kmers = query_len - (k - 1)
 
                 # double check we don't have short peptides (of len < k)
                 # note: written in this order to provide loop-optimisation hint (?)
                 if n_kmers > 0:
                     pass
@@ -1687,15 +1687,15 @@
             # get a flag for k-mer with any X (= last k-mer + 1)
             x_flag = table_idx.size - 1
 
             # iterate of sequences
             for zz in numba.prange(len(seqs_idx) - 1):
 
                 ## get the query sequence
-                s = seqs[seqs_idx[zz] : np.int(seqs_idx[zz + 1] - 1)]
+                s = seqs[seqs_idx[zz] : np.int64(seqs_idx[zz + 1] - 1)]
                 query_len = s.shape[0]
                 n_kmers = query_len - (k - 1)
 
                 # double check we don't have short peptides (of len < k)
                 # note: written in this order to provide loop-optimisation hint (?)
                 if n_kmers > 0:
                     pass
@@ -1868,15 +1868,15 @@
             # get a flag for k-mer with any X (= last k-mer + 1)
             x_flag = table_idx.size - 1
 
             # iterate of sequences
             for zz in numba.prange(len(seqs_idx) - 1):
 
                 ## get the query sequence
-                s = seqs[seqs_idx[zz] : np.int(seqs_idx[zz + 1] - 1)]
+                s = seqs[seqs_idx[zz] : np.int64(seqs_idx[zz + 1] - 1)]
                 query_len = s.shape[0]
                 n_kmers = query_len - (k - 1)
 
                 # double check we don't have short peptides (of len < k)
                 # note: written in this order to provide loop-optimisation hint (?)
                 if n_kmers > 0:
                     pass
```

### Comparing `omamer-0.2.5/omamer/omamer2matreex.py` & `omamer-0.2.6/omamer/omamer2matreex.py`

 * *Files identical despite different names*

### Comparing `omamer-0.2.5/omamer/validation.py` & `omamer-0.2.6/omamer/validation.py`

 * *Files 1% similar despite different names*

```diff
@@ -635,17 +635,17 @@
 		self._fam_fp_pos.flush()
 
 	@staticmethod
 	def _validate_positive(query_prot_offsets, thresholds, queryFam_ranked, queryFam_scores, prot_tab, pvalue_score, fam_filter_lca):
 	    '''
 	    results from the positive query set
 	    '''
-	    tp_query2tresh = np.zeros((query_prot_offsets.size, thresholds.size), dtype=np.bool)
-	    fn_query2tresh = np.zeros((query_prot_offsets.size, thresholds.size), dtype=np.bool)
-	    fp_query2tresh = np.zeros((query_prot_offsets.size, thresholds.size), dtype=np.bool)
+	    tp_query2tresh = np.zeros((query_prot_offsets.size, thresholds.size), dtype=np.bool8)
+	    fn_query2tresh = np.zeros((query_prot_offsets.size, thresholds.size), dtype=np.bool8)
+	    fp_query2tresh = np.zeros((query_prot_offsets.size, thresholds.size), dtype=np.bool8)
 	    
 	    # insure these are a flat arrays
 	    queryFam_ranked = queryFam_ranked.flatten()
 	    queryFam_scores = queryFam_scores.flatten()
 
 	    for q in range(query_prot_offsets.size):
 
@@ -685,16 +685,16 @@
 	    return tp_query2tresh, fn_query2tresh, fp_query2tresh
 
 	@staticmethod
 	def _validate_negative(thresholds, queryFam_ranked, queryFam_scores, pvalue_score):
 	    '''
 	    results from the negative query set
 	    '''
-	    tn_query2tresh = np.zeros((queryFam_ranked.size, thresholds.size), dtype=np.bool)
-	    fp_query2tresh = np.zeros((queryFam_ranked.size, thresholds.size), dtype=np.bool)
+	    tn_query2tresh = np.zeros((queryFam_ranked.size, thresholds.size), dtype=np.bool8)
+	    fp_query2tresh = np.zeros((queryFam_ranked.size, thresholds.size), dtype=np.bool8)
 
 	    # insure these are a flat arrays
 	    queryFam_ranked = queryFam_ranked.flatten()
 	    queryFam_scores = queryFam_scores.flatten()
 	    
 	    for q in range(queryFam_ranked.size):
 
@@ -895,15 +895,15 @@
 		        neg_part2fp_nr[p, t] = neg_fp_nr
 		        part2fp_nr[p, t] = fp_nr
 
 		# query number (union of positive fp, fn and tp)
 		part2query_nr = np.zeros((part_num), dtype=np.uint64)
 		for p in range(part_num):
 		    part = partitions[p]
-		    part2query_nr[p] = np.sum(np.array(fp_pos_query2tresh[:, 0][part], dtype=np.bool) + np.array(fn_query2tresh[:, 0][part], dtype=np.bool) + np.array(tp_query2tresh[:, 0][part], dtype=np.bool))
+		    part2query_nr[p] = np.sum(np.array(fp_pos_query2tresh[:, 0][part], dtype=np.bool8) + np.array(fn_query2tresh[:, 0][part], dtype=np.bool8) + np.array(tp_query2tresh[:, 0][part], dtype=np.bool8))
 
 		return part2pre, part2rec, part2spe, part2query_nr
 
 	def compute_precision_recall_specificity_family(self, partitions=np.array([])):
 		return self._compute_precision_recall_specificity_family(
 			self._fam_tp[:], self._fam_fn[:], self._fam_tn[:], self._fam_fp_pos[:], self._fam_fp_neg[:], partitions)
```

### Comparing `omamer-0.2.5/setup.py` & `omamer-0.2.6/setup.py`

 * *Files identical despite different names*

