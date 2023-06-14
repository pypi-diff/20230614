# Comparing `tmp/pankmer-0.12.8.tar.gz` & `tmp/pankmer-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data
+gzip compressed data, was "pankmer-0.9.0.tar", last modified: Sat Feb  4 08:39:36 2023, max compression
```

## Comparing `pankmer-0.12.8.tar` & `pankmer-0.9.0.tar`

### file list

```diff
@@ -1,33 +1,34 @@
--rw-r--r--   0        0        0      654 1970-01-01 00:00:00.000000 pankmer-0.12.8/rust/Cargo.toml
--rw-r--r--   0      501       20      453 2023-05-02 11:05:38.000000 pankmer-0.12.8/rust/Cargo_backup.toml
--rw-r--r--   0      501       20     2446 2023-05-28 17:15:47.000000 pankmer-0.12.8/rust/src/adj_matrix.rs
--rw-r--r--   0      501       20     2172 2023-06-14 06:39:56.000000 pankmer-0.12.8/rust/src/decompose_kmers.rs
--rw-r--r--   0      501       20     5819 2023-06-14 06:39:56.000000 pankmer-0.12.8/rust/src/get_kmers.rs
--rw-r--r--   0      501       20     1079 2023-05-28 17:15:47.000000 pankmer-0.12.8/rust/src/helpers.rs
--rw-r--r--   0      501       20     8545 2023-06-14 06:39:56.000000 pankmer-0.12.8/rust/src/lib.rs
--rw-r--r--   0      501       20     2765 2023-06-14 06:39:56.000000 pankmer-0.12.8/rust/src/measure.rs
--rw-r--r--   0      501       20     1535 2023-06-14 06:39:56.000000 pankmer-0.12.8/rust/src/mem_blocks.rs
--rw-r--r--   0      501       20     3480 2023-06-14 06:39:56.000000 pankmer-0.12.8/rust/src/metadata.rs
--rw-r--r--   0      501       20    11404 2023-06-14 06:39:56.000000 pankmer-0.12.8/rust/src/pkidx.rs
--rw-r--r--   0      501       20     5052 2023-06-14 06:39:56.000000 pankmer-0.12.8/rust/src/score_list_io.rs
--rw-r--r--   0      501       20     1151 2023-06-14 07:54:27.000000 pankmer-0.12.8/pyproject.toml
--rw-r--r--   0      501       20    32404 2023-06-14 07:10:33.000000 pankmer-0.12.8/rust/Cargo.lock
--rw-r--r--   0      501       20     6062 2023-02-04 07:49:15.000000 pankmer-0.12.8/src/pankmer/tree.py
--rw-r--r--   0      501       20     4443 2023-05-28 17:15:47.000000 pankmer-0.12.8/src/pankmer/collect.py
--rw-r--r--   0      501       20       58 2023-05-28 17:15:47.000000 pankmer-0.12.8/src/pankmer/version.py
--rw-r--r--   0      501       20    17939 2023-02-04 07:49:15.000000 pankmer-0.12.8/src/pankmer/env.py
--rw-r--r--   0      501       20     3314 2023-05-02 11:05:38.000000 pankmer-0.12.8/src/pankmer/clustermap.py
--rw-r--r--   0      501       20      214 2023-05-19 03:56:34.000000 pankmer-0.12.8/src/pankmer/get_lower_bound.py
--rw-r--r--   0      501       20     1493 2023-02-04 07:49:15.000000 pankmer-0.12.8/src/pankmer/download.py
--rw-r--r--   0      501       20      313 2023-06-14 06:39:56.000000 pankmer-0.12.8/src/pankmer/__init__.py
--rw-r--r--   0      501       20     1815 2023-05-28 17:15:47.000000 pankmer-0.12.8/src/pankmer/adjacency_matrix.py
--rw-r--r--   0      501       20     1824 2023-06-14 07:54:27.000000 pankmer-0.12.8/src/pankmer/upset.py
--rw-r--r--   0      501       20     3320 2023-06-14 06:39:56.000000 pankmer-0.12.8/src/pankmer/subset.py
--rw-r--r--   0      501       20      534 2023-05-02 11:05:38.000000 pankmer-0.12.8/src/pankmer/gzip_agnostic_open.py
--rw-r--r--   0      501       20    18604 2023-06-14 07:54:27.000000 pankmer-0.12.8/src/pankmer/reg_coverage.py
--rw-r--r--   0      501       20     2923 2023-06-14 07:54:27.000000 pankmer-0.12.8/src/pankmer/anchormap.py
--rw-r--r--   0      501       20      757 2023-05-28 17:15:47.000000 pankmer-0.12.8/src/pankmer/count.py
--rw-r--r--   0      501       20     2320 2023-05-22 10:16:39.000000 pankmer-0.12.8/src/pankmer/dryrun.py
--rw-r--r--   0      501       20    61707 2023-06-14 06:39:56.000000 pankmer-0.12.8/src/pankmer/pankmer.py
--rw-r--r--   0      501       20     4299 2023-06-14 06:39:56.000000 pankmer-0.12.8/README.md
--rw-r--r--   0        0        0     5280 1970-01-01 00:00:00.000000 pankmer-0.12.8/PKG-INFO
+drwxr-xr-x   0 anthonyaylward   (501) staff       (20)        0 2023-02-04 08:39:36.228165 pankmer-0.9.0/
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     1582 2023-02-04 07:58:07.000000 pankmer-0.9.0/LICENSE
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     5077 2023-02-04 08:39:36.227417 pankmer-0.9.0/PKG-INFO
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     4331 2023-02-04 07:49:14.000000 pankmer-0.9.0/README.md
+drwxr-xr-x   0 anthonyaylward   (501) staff       (20)        0 2023-02-04 08:39:36.187702 pankmer-0.9.0/pankmer.egg-info/
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     5077 2023-02-04 08:39:36.000000 pankmer-0.9.0/pankmer.egg-info/PKG-INFO
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)      638 2023-02-04 08:39:36.000000 pankmer-0.9.0/pankmer.egg-info/SOURCES.txt
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)        1 2023-02-04 08:39:36.000000 pankmer-0.9.0/pankmer.egg-info/dependency_links.txt
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)       49 2023-02-04 08:39:36.000000 pankmer-0.9.0/pankmer.egg-info/entry_points.txt
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)       68 2023-02-04 08:39:36.000000 pankmer-0.9.0/pankmer.egg-info/requires.txt
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)        8 2023-02-04 08:39:36.000000 pankmer-0.9.0/pankmer.egg-info/top_level.txt
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     1174 2023-02-04 08:27:05.000000 pankmer-0.9.0/pyproject.toml
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)       38 2023-02-04 08:39:36.228268 pankmer-0.9.0/setup.cfg
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)      450 2023-01-16 17:12:04.000000 pankmer-0.9.0/setup.py
+drwxr-xr-x   0 anthonyaylward   (501) staff       (20)        0 2023-02-04 08:39:36.180795 pankmer-0.9.0/src/
+drwxr-xr-x   0 anthonyaylward   (501) staff       (20)        0 2023-02-04 08:39:36.218482 pankmer-0.9.0/src/pankmer/
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)      257 2023-02-04 07:49:15.000000 pankmer-0.9.0/src/pankmer/__init__.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     1832 2023-02-04 07:49:15.000000 pankmer-0.9.0/src/pankmer/adjacency_matrix.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     3009 2023-02-04 07:49:15.000000 pankmer-0.9.0/src/pankmer/clustermap.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)      907 2023-02-04 07:49:15.000000 pankmer-0.9.0/src/pankmer/count.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     1493 2023-02-04 07:49:15.000000 pankmer-0.9.0/src/pankmer/download.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)    17939 2023-02-04 07:49:15.000000 pankmer-0.9.0/src/pankmer/env.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)      213 2023-02-04 07:49:15.000000 pankmer-0.9.0/src/pankmer/get_lower_bound.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)      364 2023-02-04 07:49:15.000000 pankmer-0.9.0/src/pankmer/gzip_agnostic_open.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)    13154 2023-02-04 07:49:15.000000 pankmer-0.9.0/src/pankmer/index.pyx
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)    46421 2023-02-04 07:49:15.000000 pankmer-0.9.0/src/pankmer/pankmer.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)      355 2023-02-04 07:49:15.000000 pankmer-0.9.0/src/pankmer/populate.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)    17507 2023-02-04 07:49:15.000000 pankmer-0.9.0/src/pankmer/reg_coverage.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     6062 2023-02-04 07:49:15.000000 pankmer-0.9.0/src/pankmer/tree.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)       81 2023-02-04 08:26:57.000000 pankmer-0.9.0/src/pankmer/version.py
+drwxr-xr-x   0 anthonyaylward   (501) staff       (20)        0 2023-02-04 08:39:36.224115 pankmer-0.9.0/test/
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     4278 2023-01-16 17:12:04.000000 pankmer-0.9.0/test/test_compiled.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     6969 2023-02-04 07:49:15.000000 pankmer-0.9.0/test/test_slow.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     2255 2023-01-16 17:12:04.000000 pankmer-0.9.0/test/test_tree.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `pankmer-0.12.8/pyproject.toml` & `pankmer-0.9.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,41 +1,40 @@
 [build-system]
-requires = ["maturin>=0.14,<0.15"]
-build-backend = "maturin"
+requires = ["setuptools", "wheel", "Cython", "numpy"]
+build-backend = "setuptools.build_meta"
 
 [project]
 name = "pankmer"
-version = "0.12.8" # Don't forget to match with Cargo.toml and docs/source/conf.py
+version = "0.9.0" # Don't forget to match with version.py and docs/source/conf.py
 authors = [
   { name="Anthony Aylward", email="aaylward@salk.edu" },
   { name="Semar Petrus" },
   { name="Allen Mamerto" },
   { name="Nolan Hartwick" },
 ]
 description = "Generate a PanGenome given a set of genomes"
 readme = "README.md"
-requires-python = ">=3.8"
+requires-python = ">=3.8,<3.11"
 classifiers = [
     "Programming Language :: Rust",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: PyPy",
     "Operating System :: OS Independent",
     "License :: OSI Approved :: BSD License",
 ]
 dependencies = [
-    "biopython",
+    "biopython<=1.79",
     "gff2bed",
     "newick",
+    "pandas",
     "pyfaidx",
     "scipy",
     "seaborn",
-    "urllib3",
-    "upsetplot",
-    "pybedtools"
+    "urllib3"
 ]
 
 [project.urls]
 "Homepage" = "https://gitlab.com/salk-tm/pankmer"
 "Documentation" = "https://salk-tm.gitlab.io/pankmer"
 
 [project.scripts]
```

### Comparing `pankmer-0.12.8/src/pankmer/tree.py` & `pankmer-0.9.0/src/pankmer/tree.py`

 * *Files identical despite different names*

### Comparing `pankmer-0.12.8/src/pankmer/env.py` & `pankmer-0.9.0/src/pankmer/env.py`

 * *Files identical despite different names*

### Comparing `pankmer-0.12.8/src/pankmer/clustermap.py` & `pankmer-0.9.0/src/pankmer/clustermap.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,16 +2,15 @@
 import seaborn as sns
 from pankmer.tree import adj_to_jaccard, adj_to_overlap, compute_linkage_matrix
 
 def clustermap(adj_matrix, output: str, cmap: str = 'mako_r',
                width: float = 7.0, height: float = 7.0,
                metric='intersection', method='complete',
                optimal_ordering: bool = True, square: bool = True,
-               heatmap_tick_pos='right', cbar_tick_pos='left',
-               dendrogram_ratio: float = 0.2, dendrogram_spacer:float = 0.1):
+               heatmap_tick_pos='right', cbar_tick_pos='left'):
     """Plot a clustered heatmap of genome similarity values
 
     Parameters
     ----------
     adj_matrix : DataFrame
         a Pandas data frame representing the adjacency matrix
     output : str
@@ -33,29 +32,25 @@
         between successive leaves is minimal. See
         `scipy.cluster.hierarchy.linkage`
     square : bool
         If True, the heatmap will be drawn square. This may force the figure
         dimensions to be altered slightly
     cbar_tick_pos : str
         Position of color bar ticks. Must be "left" or "right" [left]
-    dendrogram_ratio : float
-        Fraction of plot width used for dendrogram [0.2]
-    dendrogram_spacer : float
-        Fraction of plot width used as spacer between dendrogram and heatmap [0.1]
     """
     
     if metric == 'jaccard':
         adj_matrix = adj_to_jaccard(adj_matrix)
     elif metric == 'overlap':
         adj_matrix = adj_to_overlap(adj_matrix)
     linkage = compute_linkage_matrix(adj_matrix, method=method,
                                      optimal_ordering=optimal_ordering)
     ax = sns.clustermap(adj_matrix, cmap=cmap, figsize=(width, height),
                         row_linkage=linkage, col_linkage=linkage,
-                        xticklabels=False, dendrogram_ratio=(dendrogram_ratio,0))
+                        xticklabels=False, dendrogram_ratio=(.2,0))
     if square:
         ax.ax_heatmap.set_aspect("equal")
     ax.ax_col_dendrogram.set_visible(False)
     ax_hm_pos = ax.ax_heatmap.get_position()
     ax_row_pos = ax.ax_row_dendrogram.get_position()
     match heatmap_tick_pos:
         case 'left':
@@ -63,11 +58,11 @@
                                         ax_hm_pos.width, ax_hm_pos.height])
         case 'right':
             ax.ax_heatmap.set_position([ax_hm_pos.x0-.1, ax_hm_pos.y0,
                                         ax_hm_pos.width, ax_hm_pos.height])
     ax.ax_heatmap.yaxis.set_ticks_position(heatmap_tick_pos)
     ax.ax_heatmap.set_yticklabels(ax.ax_heatmap.get_yticklabels(), rotation=0)
     ax.ax_row_dendrogram.set_position([ax_row_pos.x0, ax_hm_pos.y0, 
-                                       ax_row_pos.width-dendrogram_spacer, ax_hm_pos.height])
+                                       ax_row_pos.width-.1, ax_hm_pos.height])
     ax.ax_cbar.set_position([.97, ax_hm_pos.y0, .03, ax_hm_pos.height])
     ax.ax_cbar.yaxis.set_ticks_position(cbar_tick_pos)
     ax.savefig(output)
```

### Comparing `pankmer-0.12.8/src/pankmer/download.py` & `pankmer-0.9.0/src/pankmer/download.py`

 * *Files identical despite different names*

### Comparing `pankmer-0.12.8/src/pankmer/adjacency_matrix.py` & `pankmer-0.9.0/src/pankmer/adjacency_matrix.py`

 * *Files 3% similar despite different names*

```diff
@@ -30,20 +30,20 @@
         a PKResults object
     
     Returns
     -------
     DataFrame
         an adjacency matrix    
     """
-    pass
+
     score_counts = {}
-    for _, _, score in results:
+    for _, score in results:
         score_counts[score] = score_counts.get(score, 0) + 1
-    print(score_counts)
     mat = np.zeros((results.number_of_genomes,
                     results.number_of_genomes), dtype=int)
     for score, count in score_counts.items():
-        score_multi = np.array(score) * count
+        score_arr = results.decode_score(score)
+        score_multi = np.array(score_arr) * count
         mat = add_score_mat_np(score_multi, mat)
     genome_names = tuple(str(os.path.basename(g)).replace('.fasta.gz', '').replace('.fa.gz', '')
                          for g in results.genomes)
     return pd.DataFrame(mat, index=genome_names, columns=genome_names)
```

### Comparing `pankmer-0.12.8/src/pankmer/reg_coverage.py` & `pankmer-0.9.0/src/pankmer/reg_coverage.py`

 * *Files 4% similar despite different names*

```diff
@@ -176,15 +176,15 @@
                                         summary_func=summary_func)
 
 
 def check_for_bgzip(reference: str):
     try:
         BgzfReader(reference)
     except ValueError:
-        raise RuntimeError('Input FASTA must be BGZIP compressed')
+        raise RuntimeError('Input FASTA must be BGZIP compressed')        
 
 
 def get_chromosome_sizes_from_ref(reference: str):
     """Extract chromosome sizes from reference FASTA
 
     Parameters
     ----------
@@ -271,16 +271,15 @@
 def genome_coverage_plot(plotting_data, output: str,
                          groups=None, loci=None, sizes=None,
                          title: str = 'Coverage', x_label: str = 'Chromosome',
                          legend: bool = False,
                          legend_title: str = 'Group', legend_loc: str = 'best',
                          width: float = 7.0, height: float = 3.0,
                          color_palette=COLOR_PALETTE, alpha: float = 0.5,
-                         linewidth: int = 3, xtlabel_rotation: int = 0,
-                         xtlabel_ha: str = 'center'):
+                         linewidth: int = 3):
     """Generate a plot of average k-mer coverage values in bins, from a DF
     generated by genome_coverage_df
 
     Parameters
     ----------
     plotting_data
         pandas DataFrame as generated by genome_coverage_df
@@ -309,92 +308,76 @@
         height of the plot in inches
     color_palette
         color palette for plot lines
     alpha : float
         alpha value for plot lines
     linewidth : float
         width value for plot lines
-    xtlabel_rotation : int
-        rotation for x-axis tick labels
-    xtlabel_ha : str
-        horizontal alignment for x-axis tick labels (left, center, right)
     """
 
     chromosomes = plotting_data.loc[:,'SeqID'].unique()
-    if legend:
-        data_groups = plotting_data.loc[:,legend_title].unique()
-        if groups is None:
-            groups = data_groups
-        else:
-            groups_dict = dict(zip(data_groups, groups))
-            plotting_data[legend_title] = tuple(groups_dict[x] for x in plotting_data[legend_title])
-            plotting_data[f'{legend_title}_chrom'] = tuple(groups_dict[x] for x in plotting_data[f'{legend_title}_chrom'])
     palette = tuple(islice(cycle(color_palette[:len(groups)]),
                                  len(chromosomes) * len(groups)))
     shifts = plotting_data.loc[:,['SeqID', x_label]].groupby('SeqID').min()
-    if sizes is not None:
-        sizes.index = sizes.name
-        sizes = sizes.loc[chromosomes, 'size']
     if loci is not None:
         if sizes is None:
             raise RuntimeError('loci argument requires sizes argument')
+        sizes.index = sizes.name
+        sizes = sizes.loc[chromosomes, 'size']
         scales = sizes / sizes.mean()
         loci_parsed = tuple(
             (int(p)/sizes[c] * scales[c] + shifts.loc[c, x_label], n)
             for c, p, n in (l.split(':') for l in loci))
         loci_x = tuple(l[0] for l in loci_parsed)
         ticks_labels = sorted(loci_parsed + tuple(zip(shifts[x_label],
                                                       chromosomes)))
         xticks = tuple(tl[0] for tl in ticks_labels)
         xlabels = tuple(tl[1] for tl in ticks_labels)
     else:
         xticks = shifts[x_label]
         xlabels = chromosomes
     ax = sns.lineplot(x=x_label, y='K-mer coverage (%)',
-                      hue=f'{legend_title}_chrom', data=plotting_data, errorbar=None,
-                      linewidth=linewidth,
-                      palette=palette,
-                      alpha=alpha,
+                      hue=f'{legend_title}_chrom', data=plotting_data, ci=None,
+                      linewidth=linewidth, palette=palette, alpha=alpha,
                       legend='auto' if legend else False)
     ax.set_title(title)
     if (loci is not None) and (sizes is not None):
         ax.vlines(x=loci_x, ymin=min(plotting_data['K-mer coverage (%)']),
                   ymax=max(plotting_data['K-mer coverage (%)']),
                   colors='gray',
                   linestyles='dashed')
-    if (len(chromosomes) == 1) and (sizes is not None):
+    if len(chromosomes) == 1:
         xticks = ax.get_xticks()[1:-1]
-        xlabels=tuple(f"{x*sizes.loc[chromosomes[0]]/1e6:.1f}" for x in xticks)
+        xlabels=tuple(f"{x*sizes.loc[chromosomes[0], 'size']/1e6:.1f}" for x in xticks)
     ax.set_xticks(xticks)
-    ax.set_xticklabels(xlabels, rotation=xtlabel_rotation, ha=xtlabel_ha)
+    ax.set_xticklabels(xlabels, ha='left')
     if legend:
         if legend_loc == 'outside':
             leg = ax.legend(bbox_to_anchor=(1.02, 1), loc='upper left',
                             borderaxespad=0, title=legend_title)
         else:
             leg = ax.legend(loc=legend_loc, title=legend_title)
         for line in leg.get_lines():
             line.set_linewidth(linewidth)
             line.set_alpha(alpha)
     fig = ax.get_figure()
-    fig.set_figwidth(width)
     fig.set_figheight(height)
+    fig.set_figwidth(width)
     fig.tight_layout()
     fig.savefig(output)
     fig.clf()
 
 
 def genome_coverage(*pk_results, output: str, ref: str, chromosomes: list,
                     output_table=None, summary_func=mean, groups=None, loci=None,
                     title: str = 'Coverage', x_label: str = 'Chromosome',
                     legend: bool = False, legend_title='Group', legend_loc='best',
                     bin_size: int = 0, width: float = 7.0, height: float = 3.0,
                     color_palette=COLOR_PALETTE, alpha: float = 0.5,
-                    linewidth: int = 3, processes: int = 1,
-                    xtlabel_rotation: int = 0, xtlabel_ha: str = 'center'):
+                    linewidth: int = 3, processes: int = 1):
 
     """Generate a plot of average k-mer coverage values in bins across the
     input genome
 
     Parameters
     ----------
     pk_results
@@ -434,18 +417,14 @@
         color palette for plot lines
     alpha : float
         alpha value for plot lines
     linewidth : float
         width value for plot lines
     processes: int
         number of processes to use
-    xtlabel_rotation : int
-        rotation for x-axis tick labels
-    xtlabel_ha : str
-        horizontal alignment for x-axis tick labels (left, center, right)
     """
 
     check_for_bgzip(ref)
     if not groups:
         groups = list(range(len(pk_results)))
     for result in pk_results:
         result.threads = processes
@@ -457,16 +436,15 @@
         legend_title=legend_title, bin_size=bin_size, x_label=x_label)
     if output_table:
         plotting_data.to_csv(output_table, sep='\t', index=False)
     genome_coverage_plot(plotting_data, output=output,
         groups=groups, loci=loci, sizes=sizes, title=title, x_label=x_label,
         legend=legend, legend_title=legend_title, legend_loc=legend_loc,
         width=width, height=height, color_palette=color_palette, alpha=alpha,
-        linewidth=linewidth, xtlabel_rotation=xtlabel_rotation,
-        xtlabel_ha=xtlabel_ha)
+        linewidth=linewidth)
 
 
 def coverage_heatmap(pk_results, refs, features, output, n_features=None, width=7, height=7):
     if not output.endswith('.png'):
         raise RuntimeError('output file path must end with .png')
     results = tuple(pk_results.get_collapsed_regional_scores(ref, gff_to_dict(gff, n_features=n_features))
         for ref, gff in zip(refs, features))
```

### Comparing `pankmer-0.12.8/src/pankmer/count.py` & `pankmer-0.9.0/src/pankmer/count.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,25 +1,29 @@
 import pandas as pd
-from collections import Counter
 
 def count_kmers(*pk_results, names=None):
     """Count total and diagnostic K-mers in one or more indexes
 
     Parameters
     ----------
     pk_results
         a PKResults object
     names
         an iterable of the names for each input index
 
     Returns
     -------
     DataFrame
-        table of K-mer counts for each index
+        table of total and diagnostic K-mer counts for each index
     """
-    names = names or range(len(pk_results))
-    max_score = max(pkr.number_of_genomes for pkr in pk_results)
-    kmer_counts = pd.DataFrame(0, columns=names, index=range(1, max_score+1))
-    for pkr, name in zip(pk_results, names):
-        for s, c in  Counter(sum(score) for _, _, score in pkr).items():
-            kmer_counts.loc[s, name] = c
+
+    kmer_counts = pd.DataFrame(columns=('index', 'total', 'diagnostic'))
+    for pkr, name in zip(pk_results, names or range(len(pk_results))):
+        total_count, diagnostic_count = 0, 0
+        for _, score in pkr:
+            total_count += 1
+            if sum(score) < pkr.number_of_genomes:
+                diagnostic_count += 1
+        kmer_counts = pd.concat((kmer_counts, pd.DataFrame(
+            ((name, total_count, diagnostic_count),),
+            columns=('index', 'total', 'diagnostic'))))
     return kmer_counts
```

### Comparing `pankmer-0.12.8/src/pankmer/pankmer.py` & `pankmer-0.9.0/src/pankmer/pankmer.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,74 +1,62 @@
 #!/usr/bin/env python
 import argparse
-import gzip
-import io
-from os.path import join, isfile, isdir, basename, dirname, exists
-import seaborn as sns
-from os import mkdir, listdir
+from os.path import join, isfile, isdir, basename
+import os
 import sys
 import time
+import gzip
 from multiprocessing import Pool
 import pandas as pd
+import io
 import math
 import json
 from Bio import SeqIO
 import numpy as np
 import shutil
 import tarfile
-import itertools
-from operator import itemgetter
 
 # from pankmer.index import (print_err, genome_name, break_seq, get_kmers,
 #                    score_byte_to_blist, kmer_byte_to_blist, kmer_byte_to_long)
-from pankmer.index import (kmer_size, break_seq, print_err, score_byte_to_blist,
-                           run_index, load_scores, measure_genomes)
+from pankmer.index import (print_err, break_seq, get_kmers, score_byte_to_blist,
+                           run_index)
 from pankmer.env import EXAMPLE_DATA_DIR
 from pankmer.download import download_example
 from pankmer.count import count_kmers
-from pankmer.collect import COL_COLOR_PALETTE, collect
-from pankmer.upset import upset
-from pankmer.subset import subset
 from pankmer.adjacency_matrix import get_adjacency_matrix
-from pankmer.tree import tree, adj_to_jaccard, adj_to_overlap
+from pankmer.tree import tree
 from pankmer.clustermap import clustermap
 from pankmer.reg_coverage import (COLOR_PALETTE, reg_coverage, genome_coverage,
                                   genome_coverage_plot, coverage_heatmap)
-from pankmer.anchormap import anchormap
-from pankmer.dryrun import dryrun
 from pankmer.version import __version__
 from pankmer.gzip_agnostic_open import gzip_agnostic_open
 from pankmer.get_lower_bound import get_lower_bound
 
-#===============================================================================
-KMER_MAX = 2**64-1
-
-#===============================================================================
 
-def retrieve_metadata(metadata_path):
+def retreive_metadata(metadata_path):
     if isinstance(metadata_path, tarfile.ExFileObject):
         metadata = json.load(metadata_path)
     else:
         with open(metadata_path, 'rt') as infile:
             metadata = json.load(infile)
     genomes = {}
     for pos in range(len(metadata['genomes'])):
         genome = metadata['genomes'][str(pos)]
         size = metadata['genome_sizes'][genome]
         genomes[genome] = size
-    return metadata['kmer_size'], genomes, metadata['positions'], metadata['mem_blocks']
+    return metadata['kmer_size'], genomes, metadata['positions']
 
 
 def get_positional_kmers(fasta_path, upper, lower, contig_header='id'):
     kmers_dict = {}
     with gzip_agnostic_open(fasta_path, 'rt') as infile:
         for record in SeqIO.parse(infile, 'fasta'):
             names = {'id': record.id, 'description': record.description}
             seq_byte = bytes(str(record.seq).upper(), 'ascii')
-            kmers_dict[names[contig_header]] = break_seq(seq_byte, upper, lower, KMER_MAX)
+            kmers_dict[names[contig_header]] = break_seq(seq_byte, upper, lower)
     return kmers_dict
 
 
 def get_sorted_kmer_scores(args: list) -> dict:
     index_path, kmers = args
     results = PKResults(index_path)
     lower = min(list(kmers.keys()))
@@ -76,90 +64,85 @@
     lb_bit = int(lower).to_bytes(results.kmer_bitsize, byteorder="big", signed=False) # lower bound bit
     ub_bit = int(upper).to_bytes(results.kmer_bitsize, byteorder="big", signed=False)
     # Find lower bound position from index
     initial_lower_bound = get_lower_bound(results.positions, lower)
     # Move iterator from initial lower bound to actual lower bound
     if initial_lower_bound != None:
         results.seek_kmer(initial_lower_bound)
-        results.seek_i(initial_lower_bound)
-    for kmer_bit, _, score in results:
+        results.seek_score(initial_lower_bound)
+    for kmer_bit, score_bit in results:
         if kmer_bit > ub_bit:
             break
         kmer  = results.decode_kmer(kmer_bit)
         if kmer in kmers:
+            score = results.decode_score(score_bit)
             kmers[kmer] = score
     return kmers
 
 
 class PKIterator:
     def __init__(self, results):
         self._results = results
     
     def __next__(self):
         kmer = self._results.get_kmer_byte()
-        i_score = self._results.get_score_byte()
-        if kmer == None or i_score == None:
+        score = self._results.get_score_byte()
+        if kmer == None or score == None:
             self._results.reset_iter()
             raise StopIteration
-        return (kmer, *i_score)
+        return kmer, score
 
 
 class PKResults:
     def __init__(self, results_dir: str, threads: int = 1):
-        index_files = ['metadata.json', 'kmers.bgz', 'indices.bgz', 'scores.pks']
-        self.input_is_tar = False
+        index_files = ['metadata.json', 'kmers.b.gz', 'scores.b.gz']
         if isfile(results_dir) and tarfile.is_tarfile(results_dir):
             self.input_is_tar = True
             self.tar = tarfile.open(results_dir)
             found_files = {basename(tarinfo.name) for tarinfo in self.tar
                             if tarinfo.isreg()}
             for file in index_files:
                 if file not in found_files:
                     raise ValueError(f"{file} is not found in index!")
-            indices_filename, kmers_filename, metadata_filename, scores_filename = sorted(
+            kmers_filename, metadata_filename, scores_filename = sorted(
                 tarinfo.name for tarinfo in self.tar if tarinfo.isreg())
-            kmer_size, genomes, positions, mem_blocks = retrieve_metadata(
+            kmer_size, genomes, positions = retreive_metadata(
                 self.tar.extractfile(metadata_filename))
-            self.number_of_genomes = len(genomes)
-            self.scores = {i: tuple(self.decode_score(bytes(s))) for i, s in enumerate(load_scores(str(results_dir), str(results_dir)))}
             self.kmers_stream = gzip.open(self.tar.extractfile(kmers_filename), 'rb')
-            self.indices_stream = gzip.open(self.tar.extractfile(indices_filename), 'rb')
+            self.scores_stream = gzip.open(self.tar.extractfile(scores_filename), 'rb')
         elif isdir(results_dir):
             for file in index_files:
                 file_path = join(results_dir, file)
                 if not isfile(file_path):
                     raise ValueError(f"{file} is not found in results directory!")
-            kmer_size, genomes, positions, mem_blocks = retrieve_metadata(join(results_dir, 'metadata.json'))
-            self.number_of_genomes = len(genomes)
-            self.scores = {i: tuple(self.decode_score(bytes(s))) for i, s in enumerate(load_scores(str(results_dir), ''))}
-            self.kmers_stream = gzip.open(join(results_dir, 'kmers.bgz'), 'rb')
-            self.indices_stream = gzip.open(join(results_dir, 'indices.bgz'), 'rb')
+            kmer_size, genomes, positions = retreive_metadata(join(results_dir, 'metadata.json'))
+            self.kmers_stream = gzip.open(join(results_dir, 'kmers.b.gz'), 'rb')
+            self.scores_stream = gzip.open(join(results_dir, 'scores.b.gz'), 'rb')
         else:
             raise ValueError(f"{results_dir} is not a valid directory!")
         self.results_dir = results_dir
         self.kmer_size = kmer_size
         self.genomes = genomes
+        self.number_of_genomes = len(genomes)
         self.positions = positions
         self.kmer_bitsize = math.ceil(((kmer_size*2))/8)
-        self.i_bitsize = 8
+        self.score_bitsize = math.ceil(len(genomes)/8)
         self.threads = threads
-        self.mem_blocks = mem_blocks
         self.kmer_buffer = io.BufferedReader(self.kmers_stream)
-        self.i_buffer = io.BufferedReader(self.indices_stream)
+        self.score_buffer = io.BufferedReader(self.scores_stream)
         
     def __iter__(self) -> PKIterator:
         """ Object iterator
 
         Returns
         -------
         PKIterator
             returns a kmer and a score in bytes
         """        
         return PKIterator(self)
-
         
     def get_kmer_byte(self) -> bytes:
         """read bytes in size of one kmer from kmers file
 
         Returns
         -------
         bytes
@@ -174,45 +157,44 @@
         """read bytes in size of one score from scores file
 
         Returns
         -------
         bytes
             bytes represting what samples have a Kmer
         """        
-        i_byte = self.i_buffer.read(self.i_bitsize)
-        if not i_byte:
+        score_byte = self.score_buffer.read(self.score_bitsize)
+        if not score_byte:
             return None
-        i = int.from_bytes(i_byte, byteorder='big', signed=False)
-        return i_byte, self.scores[i]
+        return score_byte
     
     def seek_kmer(self, kmer_num : int):
         """Move Kmer file pointer past a number of Kmers
 
         Parameters
         ----------
         kmer_num : int
             Number of Kmers to skip
         """        
         self.kmer_buffer.seek(kmer_num*self.kmer_bitsize)
     
-    def seek_i(self, i_num: int):
+    def seek_score(self, score_num: int):
         """Move Score file pointer past a number of scores
 
         Parameters
         ----------
         score_num : int
             Number of scores to skip
         """        
-        self.i_buffer.seek(i_num*self.i_bitsize)
+        self.score_buffer.seek(score_num*self.score_bitsize)
 
     def reset_iter(self):
         """Move Kmer and Score files' pointers to 0 position
         """        
         self.seek_kmer(0)
-        self.seek_i(0)
+        self.seek_score(0)
         
     def set_threads(self, threads : int):
         """Set number of threads to run multithreaded processes
 
         Parameters
         ----------
         threads : int
@@ -268,15 +250,15 @@
         -------
         int
             Python integer representing canonical Kmer
         """        
         upper = (1<<(self.kmer_size*2))-1
         lower = 0
         kmer_byte = bytes(kmer.upper(), 'ascii')
-        kmer_list = break_seq(kmer_byte, upper, lower, KMER_MAX)
+        kmer_list = break_seq(kmer_byte, upper, lower)
         if len(kmer_list) > 1:
             raise ValueError(f"encode_kmer should be used for one Kmer of size {self.kmer_size} only! "
                              f"Please use get_sequence_kmerbits for a sequence larger than that.")
         return kmer_list[0]
     
     def get_sequence_kmerbits(self, seq : str, upper : int = None, lower : int = None) -> list:
         """Get canonical Kmers making up the sequence
@@ -292,15 +274,15 @@
             list of Python integers representing the canonical Kmers
         """        
         if upper == None:
             upper = (1<<(self.kmer_size*2))-1
         if lower == None:
             lower = 0
         seq_byte = bytes(str(seq).upper(), 'ascii')
-        kmer_bits = break_seq(seq_byte, upper, lower, KMER_MAX)
+        kmer_bits = break_seq(seq_byte, upper, lower)
         
         return kmer_bits
     
     def get_kmer_scores(self, kmers : dict = None) -> dict:
         """Retrieve scores of Kmer in the Kmers dictionary.
         if no dictionary is supplied then retrieve all scores.
 
@@ -321,15 +303,15 @@
             for kmer, score in self:
                 kmers[kmer] = score
         else:
             # get only scores in kmers
             for kmer, score in self:
                 kmer_int = self.decode_kmer(kmer)
                 if kmer_int in kmers:
-                    kmers[kmer_int] = score
+                    kmers[kmer_int] = self.decode_score(score)
         return kmers
     
     def get_sequence_score(self, seq : str, kmers : dict = None) -> list:
         """Retrieve scores of canonical Kmers in the sequence
 
         Parameters
         ----------
@@ -714,211 +696,62 @@
 #             score = score_buffer.read(score_bitsize)
 
 #     return scores_counts
 
 
 def get_kmers_wrapper(seq, upper, lower):
     seq_byte = bytes(str(seq).upper(), 'ascii')
-    kmers = break_seq(seq_byte, upper, lower, KMER_MAX)
+    kmers = break_seq(seq_byte, upper, lower)
     return kmers
 
 
-def index_wrapper(genomes_input, outdir: str, split_memory: int = 1,
-                  split_disk: int = 1, threads: int = 1, index: str = '',
-                  fraction: float = 1.0, gzip_level: int = 6, k=kmer_size()):
-    if split_disk > split_memory:
-        raise RuntimeError('split_disk must be less than or equal split_memory')
-    if basename(outdir).endswith('.tar'):
-        output_is_tar = True
-        outdir = join(dirname(outdir), basename(outdir)[:-4])
-    else:
-        output_is_tar = False
-
-    if not isinstance(genomes_input, (tuple, list)):
-        genomes_input = list(genomes_input) if isinstance(genomes_input, set) else [genomes_input]
-    if len(genomes_input) == 1 and isfile(genomes_input[0]) and tarfile.is_tarfile(genomes_input[0]):
-        input_is_tar = True
-        with tarfile.open(genomes_input[0]) as tar:
-            genomes = [tarinfo.name for tarinfo in tar if tarinfo.isreg()]
-    else:
-        input_is_tar = False
-        genomes = list(itertools.chain.from_iterable(
-            ([join(g, f) for f in sorted(listdir(g))] if isdir(g) else [g])
-            for g in genomes_input))
-        # Check if input files exist and are files
-        for genome in genomes:
-            if not exists(genome) or not isfile(genome):
-                raise RuntimeError(f"{genome} does not exist or is not a file!")
-                return 1
-
-    # Make the output directory if it doesn't exist
-    if not exists(outdir):
-        mkdir(outdir)
-
-    print_err('Recording genome sizes')
-    genomes_dict = measure_genomes(genomes, str(genomes_input[0]) if input_is_tar else '')
-    positions_dictionary, mem_blocks = run_index((str(genomes_input[0]) if input_is_tar else ''),
-            genomes, str(outdir),
-            split_memory=split_memory, split_disk=split_disk, threads=threads,
-            index=index, input_is_tar=input_is_tar, fraction=fraction,
-            gzip_level=gzip_level, kmersize=k)
-    
-    # if index:
-    #     genomes, genomes_dict = update_genomes(index, genomes, genomes_dict)
-
-    print_err("Saving metadata.")
-    metadata_dict = {'kmer_size': kmer_size(),
-        'version': __version__,
-        'genomes': {c:g for c, g in enumerate(genomes)},
-        'genome_sizes': genomes_dict,
-        'positions': dict(sorted(positions_dictionary.items(), key=itemgetter(1))),
-        'mem_blocks': mem_blocks,
-        'fraction_cutoff': [fraction, int(fraction*KMER_MAX)]
-    }
-    with open(f'{outdir}/metadata.json', 'w') as outfile:
-        json.dump(metadata_dict, outfile)
-    if output_is_tar:
-        with tarfile.open(f'{outdir}.tar', 'w') as tar:
-            tar.add(outdir)
-        shutil.rmtree(outdir)
-
-def run_index_wrapper(args):
+def index_wrapper(args):
     if args.time:
         start = time.time()
-    # index = args.index
-    # index_wrapper(genomes_input, fraction, 31, output)
-    index_wrapper(args.genomes, args.output, split_memory=args.split_memory,
-                  split_disk=args.split_disk, threads=args.threads, index='',
-                  k=31, fraction=args.fraction, gzip_level=args.gzip_level)
+    genomes_input = args.genomes
+    output = args.output
+    split_memory = args.split_memory
+    threads = args.threads
+    index = args.index
+    run_index(genomes_input, output,
+        split_memory=split_memory, threads=threads, index=index)
     if args.time:
         stop = time.time()
         print(f'Indexed in {(stop - start) / 60:.2f} minutes')
 
 
 def run_count(args):
     kmer_counts = count_kmers(*(PKResults(i) for i in args.index), names=args.index)
-    kmer_counts.to_csv(sys.stdout, sep='\t')
-
-
-def run_collect(args):
-    sat_df = collect(PKResults(args.index), args.output, title=args.title,
-                        width=args.width, height=args.height,
-                        palette=args.color_palette, alpha=args.alpha,
-                        linewidth=args.linewidth, conf=args.conf,
-                        contours=args.contours, legend_loc=args.legend_loc)
-    if args.table:
-        sat_df.to_csv(args.table, sep='\t', index=False)
-
-
-def run_upset(args):
-    if args.time:
-        start = time.time()
-    upset(PKResults(args.input), args.output, args.genomes,
-          vertical=args.vertical,
-          show_counts=args.show_counts,
-          min_subset_size=args.min_subset_size,
-          max_subset_size=args.max_subset_size,
-          exclusive=args.exclusive,
-          table=args.table)
-    if args.time:
-        stop = time.time()
-        print(f'UpSet plot generated in {(stop - start) / 60:.2f} minutes')
-
-
-def run_subset(args):
-    if args.time:
-        start = time.time()
-    subset(PKResults(args.input), args.output, args.genomes,
-          exclusive=args.exclusive, gzip_level=args.gzip_level)
-    if args.time:
-        stop = time.time()
-        print(f'subset index generated in {(stop - start) / 60:.2f} minutes')
+    kmer_counts.to_csv(sys.stdout, sep='\t', index=False)
 
 
 def run_adjacency_matrix(args):
     if args.time:
         start = time.time()
-    if args.output.endswith('.csv'):
-        separator = ','
-    elif args.output.endswith('.tsv'):
-        separator = '\t'
-    else:
-        raise RuntimeError('output must end with .csv or .tsv')
     results = PKResults(args.input_dir)
+    output = args.output
     df = get_adjacency_matrix(results)
-    df.to_csv(args.output, sep=separator)
+    df.to_csv(output)
     if args.time:
         stop = time.time()
         print(f'Matrix generated in {(stop - start) / 60:.2f} minutes')
 
 
 def run_tree(args):
-    if str(args.input).endswith('.csv'):
-        adj_matrix = pd.read_csv(args.input, index_col=0)
-    elif str(args.input).endswith('.tsv'):
-        adj_matrix = pd.read_table(args.input, index_col=0)
-    else:
-        raise RuntimeError('input must end with .csv or .tsv')
+    adj_matrix = pd.read_csv(args.input, index_col=0)
     tree(adj_matrix, newick=args.newick, metric=args.metric, method=args.method,
          transformed_matrix=args.transformed_matrix)
 
 
 def run_clustermap(args):
-    if str(args.input).endswith('.csv'):
-        adj_matrix = pd.read_csv(args.input, index_col=0)
-    elif str(args.input).endswith('.tsv'):
-        adj_matrix = pd.read_table(args.input, index_col=0)
-    else:
-        raise RuntimeError('input must end with .csv or .tsv')
+    adj_matrix = pd.read_csv(args.input, index_col=0)
     clustermap(adj_matrix, args.output, cmap=args.colormap, width=args.width,
-        height=args.height, metric=args.metric, method=args.method,
-        heatmap_tick_pos=args.heatmap_ticks,
-        cbar_tick_pos=args.cbar_ticks, dendrogram_ratio=args.dend_ratio,
-        dendrogram_spacer=args.dend_spacer)
-
-
-def run_similarity(args):
-    if str(args.input).endswith('.csv'):
-        adj_matrix = pd.read_csv(args.input, index_col=0)
-    elif str(args.input).endswith('.tsv'):
-        adj_matrix = pd.read_table(args.input, index_col=0)
-    else:
-        raise RuntimeError('input must end with .csv or .tsv')
-    if args.output.endswith('.csv'):
-        separator = ','
-    elif args.output.endswith('.tsv'):
-        separator = '\t'
-    else:
-        raise RuntimeError('output must end with .csv or .tsv')
-    if args.metric == 'jaccard':
-        df = adj_to_jaccard(adj_matrix)
-    elif args.metric == 'overlap':
-        df = adj_to_overlap(adj_matrix)
-    df.to_csv(args.output, sep=separator)
-
-
-def run_distance(args):
-    if str(args.input).endswith('.csv'):
-        adj_matrix = pd.read_csv(args.input, index_col=0)
-    elif str(args.input).endswith('.tsv'):
-        adj_matrix = pd.read_table(args.input, index_col=0)
-    else:
-        raise RuntimeError('input must end with .csv or .tsv')
-    if args.output.endswith('.csv'):
-        separator = ','
-    elif args.output.endswith('.tsv'):
-        separator = '\t'
-    else:
-        raise RuntimeError('output must end with .csv or .tsv')
-    if args.metric == 'jaccard':
-        df = 1 - adj_to_jaccard(adj_matrix)
-    elif args.metric == 'overlap':
-        df = 1 - adj_to_overlap(adj_matrix)
-    df.to_csv(args.output, sep=separator)
-
+               height=args.height, metric=args.metric, method=args.method,
+               heatmap_tick_pos=args.heatmap_ticks,
+               cbar_tick_pos=args.cbar_ticks)
 
 
 def run_regcoverage(args):
     if args.output:
         reg_coverage(*(PKResults(i) for i in args.index), ref=args.ref,
             coords=args.coords, output_file=args.output, bgzip=args.bgzip,
             genes=args.genes, flank=args.flank, processes=args.processes)
@@ -963,191 +796,86 @@
         title=args.title, x_label=x_label, legend=args.legend,
         legend_title=legend_title,
         legend_loc=args.legend_loc, width=args.width, height=args.height,
         color_palette=args.color_palette, alpha=args.alpha,
         linewidth=args.linewidth)
 
 
-def run_anchormap(args):
-    anchormap(PKResults(args.index), args.output, args.anchors, args.anno,
-              threads=args.threads)
-
-
 def run_coverage_heatmap(args):
     coverage_heatmap(PKResults(args.index), args.refs, args.features,
         args.output, n_features=args.n_features, width=args.width,
         height=args.height)
 
 
-def run_dryrun(args):
-    metadata_dict = dryrun(args.genomes, split_memory=args.split_memory, threads=args.threads)
-    json.dump(metadata_dict, sys.stdout)
-
-
 def run_download_example(args):
     download_example(args.dir, args.bacterial, args.n_samples)
 
 
 def main():
     parser = argparse.ArgumentParser(
         add_help=True)
-    parser.add_argument('--version', action='version',
-                    version='%(prog)s {version}'.format(version=__version__))
+    parser.add_argument('--version', action='store_true',
+        help='print version number')
     subparsers = parser.add_subparsers(dest='func')
     index_parser = subparsers.add_parser('index',
         help='generate k-mer index')
     index_parser.add_argument(
-        '-g', '--genomes', metavar='<genomes[.tar]>',
-        required=True,
-        nargs='+',
+        '-g', '--genomes', metavar='<genomes[.tar]>', type=str, action='store',
+        dest='genomes', required=True,
         help='directory containig input genomes')
     index_parser.add_argument(
-        '-o', '--output', metavar='<output[.tar]>',
-        required=True,
+        '-o', '--output', metavar='<output[.tar]>', type=str, action='store',
+        dest='output', required=True,
         help='output directory or tarfile that will contain the k-mer index')
     index_parser.add_argument(
-        '--split-memory', metavar='<int>', type=int, default=1,
-        help='split indexing into multiple rounds to reduce memory usage')
-    index_parser.add_argument(
-        '--split-disk', metavar='<int>', type=int, default=1,
-        help='split indexing into multiple rounds to reduce temp disk usage')
-    index_parser.add_argument(
-        '-t', '--threads', metavar='<int>',
-        type=int, help=('Number of threads to use'), default=1)
+        '--split-memory', metavar='<int>', action='store',
+        dest='split_memory', type=int, help=(
+        'Parallel.'
+        'This splits the indexing into multiple rounds; reducing memory.'
+        ), default=1)
     index_parser.add_argument(
-        '--fraction', metavar='<float>', type=float, default=1.0, help=(
-        'Fraction of k-mer minimizers to use'))
+        '-t', '--threads', metavar='<int>', action='store',
+        dest='threads', type=int, help=('Number of threads to use'), default=1)
     index_parser.add_argument(
-        '--gzip-level', choices=range(1,10), type=int, default=6,
-        help='gzip compression level [6]')
-    # index_parser.add_argument(
-    #     '-i', '--index', metavar='<index[.tar]>',
-    #     dest='index', required=False, default='',
-    #     help=('Path to existing index to update.')
-    # )
+        '-i', '--index', metavar='<index[.tar]>', type=str, action='store',
+        dest='index', required=False, default=None,
+        help=('Path to existing index to update.')
+    )
     index_parser.add_argument(
         '--time', action='store_true',
         help='Report the time required to execute'
     )
-    index_parser.set_defaults(func=run_index_wrapper)
+    index_parser.set_defaults(func=index_wrapper)
 
     count_parser = subparsers.add_parser('count',
         help='count k-mers in one or more indexes')
     count_parser.add_argument(
         '-i', '--index', metavar='<index[.tar]>', type=str, action='store',
         dest='index', required=True, nargs='+', help='a k-mer index')
     count_parser.set_defaults(func=run_count)
 
-    collect_parser = subparsers.add_parser('collect',
-        help='calculate k-mer collection curve')
-    collect_parser.add_argument(
-        '-i', '--index', metavar='<index[.tar]>', type=str, action='store',
-        required=True, help='a k-mer index')
-    collect_parser.add_argument(
-        '-o', '--output', metavar='<output.{pdf,png,svg}>', type=str,
-        action='store', dest='output',
-        help='destination file for plot')
-    collect_parser.add_argument(
-        '-t', '--table', metavar='<output-table.tsv>',
-        help='output TSV file containing plotted data')
-    collect_parser.add_argument('--title', metavar='<"Plot title">',
-        help='set the title for the plot')
-    collect_parser.add_argument('--width', metavar='<float>', type=float,
-        default=4.0, help='set width of figure in inches [4]')
-    collect_parser.add_argument('--height', metavar='<float>', type=float,
-        default=3.0, help='set height of figure in inches [3]')
-    collect_parser.add_argument('--color-palette', metavar='<#color>', nargs='+',
-        default=COL_COLOR_PALETTE, help='color palette to use')
-    collect_parser.add_argument('--alpha', metavar='<float>', type=float,
-        default=1.0, help='transparency value for lines [1.0]')
-    collect_parser.add_argument('--linewidth', metavar='<int>', type=int,
-        default=3, help='line width for plot [3]')
-    conf_or_cont = collect_parser.add_mutually_exclusive_group()
-    conf_or_cont.add_argument('--conf', action='store_true',
-        help='calculate confidence intervals for collection curves')
-    conf_or_cont.add_argument('--contours', metavar='<int>', type=int,
-        nargs='+', help='set contours for collection curves (in percent)')
-    collect_parser.add_argument('--legend-loc',
-        choices=('best', 'upper left', 'upper right', 'lower left',
-                 'lower right', 'outside'),
-        default='best', help='location of legend [best]')
-    collect_parser.set_defaults(func=run_collect)
-
-    upset_parser = subparsers.add_parser('upset', help='generate upset plot')
-    upset_parser.add_argument(
-        '-i', '--input', metavar='<index[.tar]>',
-        required=True, help='a k-mer index')
-    upset_parser.add_argument(
-        '-o', '--output', metavar='<output.{pdf,png,svg}>', required=True,
-        help='destination file for upset plot')
-    upset_parser.add_argument(
-        '-g', '--genomes', metavar='<genome>', required=True, nargs='+',
-        help='list of genomes to include')
-    upset_parser.add_argument(
-        '-v', '--vertical', action='store_true',
-        help='draw the plot vertically')
-    upset_parser.add_argument(
-        '-x', '--exclusive', action='store_true',
-        help='exclude k-mers that occur in genomes other than the input set')
-    upset_parser.add_argument(
-        '-t', '--table', metavar='<table.tsv[.gz]>',
-        help='write (optionally compressed) table of values in tsv format')
-    upset_parser.add_argument(
-        '--show-counts', action='store_true',
-        help='show counts for each subset')
-    upset_parser.add_argument(
-        '--min-subset-size', metavar='<int>', type=int,
-        help='show only subsets larger than a minimum size')
-    upset_parser.add_argument(
-        '--max-subset-size', metavar='<int>', type=int,
-        help='show only subsets smaller than a maximum size')
-    upset_parser.add_argument(
-        '--time', action='store_true',
-        help='report the time required to execute')
-    upset_parser.set_defaults(func=run_upset)
-
-    subset_parser = subparsers.add_parser('subset', help='subset an index')
-    subset_parser.add_argument(
-        '-i', '--input', metavar='<input-index[.tar]>',
-        required=True, help='a k-mer index')
-    subset_parser.add_argument(
-        '-o', '--output', metavar='<output-index[.tar]>', required=True,
-        help='destination file for subset index')
-    subset_parser.add_argument(
-        '-g', '--genomes', metavar='<genome>', required=True, nargs='+',
-        help='list of genomes to include ')
-    subset_parser.add_argument(
-        '-x', '--exclusive', action='store_true',
-        help='exclude k-mers that occur in genomes other than the input set')
-    subset_parser.add_argument(
-        '--gzip-level',  choices=range(1,10), type=int, default=6,
-        help='gzip compression level [6]')
-    subset_parser.add_argument(
-        '--time', action='store_true',
-        help='report the time required to execute')
-    subset_parser.set_defaults(func=run_subset)
-
     adjmat_parser = subparsers.add_parser('adj-matrix',
         help='generate adjacency matrix')
     adjmat_parser.add_argument(
-        '-i', '--input', metavar='<index[.tar]>',
+        '-i', '--input', metavar='<index[.tar]>', type=str, action='store',
         dest='input_dir', required=True, help='a k-mer index')
     adjmat_parser.add_argument(
-        '-o', '--output', metavar='<adjmatrix.{csv,tsv}>',
+        '-o', '--output', metavar='<adjmatrix.csv>', type=str, action='store',
         dest='output', required=True,
         help='destination file for adjacency matrix')
     adjmat_parser.add_argument(
         '--time', action='store_true',
-        help='Report the time required to execute')
+        help='Report the time required to execute'
+    )
     adjmat_parser.set_defaults(func=run_adjacency_matrix)
 
     tree_parser = subparsers.add_parser('tree',
         help='generate a heirarchical clustering tree from an adjacency matrix')
     tree_parser.add_argument(
-        '-i', '--input', metavar='<adjmatrix.{csv,tsv}>',
+        '-i', '--input', metavar='<adjmatrix.csv>', type=str, action='store',
         dest='input', required=True, help='adjacency matrix file')
     tree_parser.add_argument(
         '-n', '--newick', action='store_true', dest='newick',
         help='output tree in NEWICK format'
     )
     tree_parser.add_argument(
         '--metric', choices=('intersection', 'jaccard', 'overlap'),
@@ -1161,15 +889,15 @@
         '--transformed-matrix', metavar='<matrix.csv>',
         help='Write similarity transformed matrix to file')
     tree_parser.set_defaults(func=run_tree)
 
     clustermap_parser = subparsers.add_parser('clustermap',
         help='plot a clustered heatmap from the adjacency matrix')
     clustermap_parser.add_argument(
-        '-i', '--input', metavar='<adjmatrix.{csv,tsv}>', type=str, action='store',
+        '-i', '--input', metavar='<adjmatrix.csv>', type=str, action='store',
         dest='input', required=True,
         help='adjacency matrix file')
     clustermap_parser.add_argument(
         '-o', '--output', metavar='<adjmatrix.{pdf,png,svg}>', type=str, action='store',
         dest='output', required=True,
         help='destination file for plot')
     clustermap_parser.add_argument(
@@ -1194,48 +922,16 @@
         '--heatmap-ticks', choices=('left', 'right'),
         default='left',
         help='Position of heatmap ticks. Must be "left" or "right" [left]')
     clustermap_parser.add_argument(
         '--cbar-ticks', choices=('left', 'right'),
         default='left',
         help='Position of color bar ticks. Must be "left" or "right" [left]')
-    clustermap_parser.add_argument(
-        '--dend-ratio', metavar='<float>', type=float, default=0.2,
-        help='Fraction of plot width used for dendrogram [0.2]')
-    clustermap_parser.add_argument(
-        '--dend-spacer', metavar='<float>', type=float, default=0.1,
-        help='Fraction of plot width used as spacer between dendrogram and heatmap [0.1]')
     clustermap_parser.set_defaults(func=run_clustermap)
 
-    similarity_parser = subparsers.add_parser('similarity',
-        help='generate a similarity matrix from an adjacency matrix')
-    similarity_parser.add_argument(
-        '-i', '--input', metavar='<adjmatrix.{csv,tsv}>',
-        required=True, help='adjacency matrix file')
-    similarity_parser.add_argument(
-        '-o', '--output', metavar='<simmatrix.{csv,tsv}>',
-        required=True, help='similarity matrix file')
-    similarity_parser.add_argument(
-        '--metric', choices=('jaccard', 'overlap'),
-        dest='metric', default='jaccard', help='similarity metric [jaccard]')
-    similarity_parser.set_defaults(func=run_similarity)
-
-    distance_parser = subparsers.add_parser('distance',
-        help='generate a distance matrix from an adjacency matrix')
-    distance_parser.add_argument(
-        '-i', '--input', metavar='<adjmatrix.{csv,tsv}>',
-        required=True, help='adjacency matrix file')
-    distance_parser.add_argument(
-        '-o', '--output', metavar='<distmatrix.{csv,tsv}>',
-        required=True, help='distance matrix file')
-    distance_parser.add_argument(
-        '--metric', choices=('jaccard', 'overlap'),
-        dest='metric', default='jaccard', help='distance metric [jaccard]')
-    distance_parser.set_defaults(func=run_distance)
-
     regcov_parser = subparsers.add_parser('reg-coverage',
         help='generate regional coverage')
     regcov_parser.add_argument(
         '-i', '--index', metavar='<index[.tar]>', type=str, action='store',
         dest='index', required=True, nargs='+', help='index')
     regcov_parser.add_argument(
         '-r', '--reference', metavar='<reference.fa.gz>', type=str, action='store',
@@ -1299,15 +995,15 @@
         choices=(-2,-1,0,1,2),
         help=('Set bin size. The input <int> is converted to the bin size by '
               'the formula: 10^(<int>+6) bp. The default value is 0, i.e. '
               '1-megabase bins. [0]'))
     genomecov_parser.add_argument('--width', metavar='<float>', type=float,
         default=7.0, help='set width of figure in inches [7]')
     genomecov_parser.add_argument('--height', metavar='<float>', type=float,
-        default=3.0, help='set height of figure in inches [3]')
+        default=3.0, help='set width of figure in inches [3]')
     genomecov_parser.add_argument('--color-palette', metavar='<#color>', nargs='+',
         default=COLOR_PALETTE, help='color palette to use')
     genomecov_parser.add_argument('--alpha', metavar='<float>', type=float,
         default=0.5, help='transparency value for lines [0.5]')
     genomecov_parser.add_argument('--linewidth', metavar='<int>', type=int,
         default=3, help='line width for plot [3]')
     genomecov_parser.add_argument('--processes', metavar='<int>', type=int,
@@ -1320,17 +1016,17 @@
         '-t', '--table', metavar='<genomecov.tsv>', type=str, action='store',
         dest='table', required=True, help='genomic coverage results')
     gcplot_parser.add_argument(
         '-o', '--output', metavar='<output.{pdf,png,svg}>', type=str,
         action='store', dest='output', required=True,
         help='destination file for plot')
     gcplot_parser.add_argument('--groups', metavar='<"Group">', nargs='+',
-        help='list of groups for provided indexes')
+        help='list of groups for provided indexes [0]')
     gcplot_parser.add_argument('--loci', metavar='<"chr:pos:name">', nargs='+',
-        help='list of loci to mark on plot')
+        help='list of loci to mark on plot [0]')
     gcplot_parser.add_argument('--chromsizes', metavar='<file.chrom.sizes>',
         help='chromsizes file of the reference used to generate the table')
     gcplot_parser.add_argument('--title', metavar='<"Plot title">',
         help='set the title for the plot')
     gcplot_parser.add_argument('--x-label', metavar='<"Label">',
         help='set x-axis label for the plot')
     gcplot_parser.add_argument('--legend', action='store_true',
@@ -1340,15 +1036,15 @@
     gcplot_parser.add_argument('--legend-loc',
         choices=('best', 'upper left', 'upper right', 'lower left',
                  'lower right', 'outside'),
         default='best', help='location of legend [best]')
     gcplot_parser.add_argument('--width', metavar='<float>', type=float,
         default=7.0, help='set width of figure in inches [7]')
     gcplot_parser.add_argument('--height', metavar='<float>', type=float,
-        default=3.0, help='set height of figure in inches [3]')
+        default=3.0, help='set width of figure in inches [3]')
     gcplot_parser.add_argument('--color-palette', metavar='<#color>', nargs='+',
         default=COLOR_PALETTE, help='color palette to use')
     gcplot_parser.add_argument('--alpha', metavar='<float>', type=float,
         default=0.5, help='transparency value for lines [0.5]')
     gcplot_parser.add_argument('--linewidth', metavar='<int>', type=int,
         default=3, help='line width for plot [3]')
     gcplot_parser.set_defaults(func=run_genome_coverage_plot)
@@ -1376,58 +1072,29 @@
         '--width', metavar='<float>', type=float, action='store',
         dest='width', default=7, help='width of plot in inches', )
     covhm_parser.add_argument(
         '--height', metavar='<float>', type=float, action='store',
         dest='height', default=7, help='height of plot in inches', )
     covhm_parser.set_defaults(func=run_coverage_heatmap)
 
-    anchormap_parser = subparsers.add_parser('anchormap',
-        help='export an anchormap for downstream visualization')
-    anchormap_parser.add_argument(
-        '-i', '--index', metavar='<index[.tar]>', required=True, help='index')
-    anchormap_parser.add_argument(
-        '-o', '--output', metavar='<anchormap_dir/>', required=True,
-        help='output directory for the anchormap')
-    anchormap_parser.add_argument('--anchors', metavar='<anchor.fasta[.gz]>',
-                                  required=True, nargs='+',
-                                  help='the anchor genomes')
-    anchormap_parser.add_argument('--anno', metavar='<anno.gff[.gz]>',
-                                  required=True, nargs='+', help='annotations')
-    anchormap_parser.add_argument(
-        '-t', '--threads', metavar='<int>',
-        type=int, help='Number of threads to use', default=1)
-    anchormap_parser.set_defaults(func=run_anchormap)
-
-    dryrun_parser = subparsers.add_parser('dryrun',
-        help='perform a dry run of indexing and print metadata')
-    dryrun_parser.add_argument(
-        '-g', '--genomes', metavar='<genomes[.tar]>',
-        required=True,
-        nargs='+',
-        help='directory containig input genomes')
-    dryrun_parser.add_argument(
-        '--split-memory', metavar='<int>',
-        type=int, help=(
-        'Parallel.'
-        'This splits the indexing into multiple rounds; reducing memory.'
-        ), default=1)
-    dryrun_parser.add_argument(
-        '-t', '--threads', metavar='<int>',
-        type=int, help=('Number of threads to use'), default=1)
-    dryrun_parser.set_defaults(func=run_dryrun)
-
     download_parser = subparsers.add_parser('download-example',
         help='download an example dataset')
     download_parser.add_argument(
         '-d', '--dir', metavar='<dir/>', type=str, action='store',
         dest='dir', default=EXAMPLE_DATA_DIR,
         help='destination directory for example data')
     download_parser.add_argument(
         '-b', '--bacterial', action='store_true', dest='bacterial',
         help='if True, download bacterial genomes')
     download_parser.add_argument(
-        '-n', '--n-samples', metavar='<int>', type=int, default=1, action='store', dest='n_samples',
+        '-n', '--n-samples', metavar='<int>', type=int, action='store', dest='n_samples',
         help='number of bacterial samples to download, max 164 [1]')
     download_parser.set_defaults(func=run_download_example)
 
     args = parser.parse_args()
+    if args.version:
+        print(__version__)
+        sys.exit()
     args.func(args)
+
+if __name__ == "__main__":
+    main()
```

### Comparing `pankmer-0.12.8/README.md` & `pankmer-0.9.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,58 +1,58 @@
 Primary contact: Anthony Aylward, aaylward@salk.edu
 
 # PanKmer
 
 _k_-mer based and reference-free pangenome analysis. See the quickstart below, or read the [documentation](https://salk-tm.gitlab.io/pankmer/index.html).
 
 ## Installation
+### With pip
+```
+pip install git+https://gitlab.com/salk-tm/pankmer.git
+```
+
 ### In a conda environment
 First create an environment that includes all dependencies:
 ```
-conda create -c conda-forge -c bioconda -n pankmer rust python \
-  biopython seaborn urllib3 python-newick pyfaidx gff2bed upsetplot \
-  pybedtools
+conda create -c conda-forge -c bioconda -n pankmer python==3.10 biopython==1.79 cython pandas setuptools seaborn urllib3 wheel python-newick pyfaidx gff2bed
 ```
-Then install PanKmer with `pip`:
+If running on OSX, a few additional packages will be required:
 ```
 conda activate pankmer
-pip install pankmer
+conda install -c conda-forge clang_osx-64 clangxx_osx-64 gfortran_osx-64
 ```
-
-### With pip
-PanKmer is built with [Rust](https://doc.rust-lang.org/stable/book/title-page.html),
-so you will need to [install](https://doc.rust-lang.org/stable/book/ch01-01-installation.html)
-it if you have not already done so. Then you can install PanKmer with `pip`:
+Then install PanKmer with pip:
 ```
-pip install pankmer
+conda activate pankmer
+pip install pip install git+https://gitlab.com/salk-tm/pankmer.git
 ```
 
 ### Check installation
 Check that the installation was successful by running:
 ```
 pankmer --version
 ```
 
 ## Tutorial
 ### Download example dataset
 
-The `download-example` subcommand will download a small example dataset of
+The `download_example` subcommand will download a small example dataset of
 Chr19 sequences from _S. polyrhiza._
 ```
-pankmer download-example -d .
+pankmer download_example -d .
 ```
 After running this command the directory `PanKmer_example_Sp_Chr19/` will be present in the working directory. It contains FASTA files representing Chr19 from three genomes, and GFF files giving their gene annotations.
 ```
 ls PanKmer_example_Sp_Chr19/*
 ```
 ```
 PanKmer_example_Sp_Chr19/README.md
 
 PanKmer_example_Sp_Chr19/Sp_Chr19_features:
-Sp9509_oxford_v3_Chr19.gff3.gz Sp9512_a02_genes_Chr19.gff3.gz
+Sp7498_HiC_Chr19.gff.gz Sp9509_oxford_v3_Chr19.gff3.gz Sp9512_a02_genes_Chr19.gff3.gz
 
 PanKmer_example_Sp_Chr19/Sp_Chr19_genomes:
 Sp7498_HiC_Chr19.fasta.gz Sp9509_oxford_v3_Chr19.fasta.gz Sp9512_a02_genome_Chr19.fasta.gz
 ```
 
 To get started, navigate to the downloaded directory.
 ```
@@ -75,26 +75,25 @@
 Sp_Chr19_index/
 Sp_Chr19_index/kmers.b.gz
 Sp_Chr19_index/metadata.json
 Sp_Chr19_index/scores.b.gz
 ```
 
 > #### Note
-> The input genomes argument proided with the `-g` flag can be a directory, a tar archive, or a space-separated list of FASTA files.
+> The input genomes argument proided with the `-g` flag can be a directory, a tar archive, or a comma-separated list of FASTA files.
 >
 > If the output argument provided with the `-o` flag ends with `.tar`, then the index will be written as a tar archive. Otherwise it will be written as a directory.
 
 
 ### Create an adjacency matrix
 
-A useful application of the _k_-mer index is to generate an adjacency matrix. This is a table of _k_-mer similarity values for each pair of genomes in the index. We can generate one using the `adj-matrix` subcommand, which will produce a CSV or TSV file containing the matrix.
+A useful application of the _k_-mer index is to generate an adjacency matrix. This is a table of _k_-mer similarity values for each pair of genomes in the index. We can generate one using the `adj-matrix` subcommand, which will produce a CSV file containing the matrix.
 
 ```
 pankmer adj-matrix -i Sp_Chr19_index.tar -o Sp_Chr19_adj_matrix.csv
-pankmer adj-matrix -i Sp_Chr19_index.tar -o Sp_Chr19_adj_matrix.tsv
 ```
 
 > #### Note
 > The input index argument proided with the `-i` flag can be tar archive or a directory.
 
 ### Plot a clustered heatmap
 
@@ -108,19 +107,19 @@
   --height 6.5
 ```
 
 ![example heatmap](docs/source/_static/Sp_Chr19_adj_matrix.svg)
 
 ### Generate a gene variability heatmap
 
-Generate a heatmap showing variability of genes across genomes. The following command uses the `--n-features` option to limit analysis to the first two genes from each input GFF3 file. The resulting image shows the level of variability observed across genes from each genome.
+Generate a heatmap showing variability of genes across genomes. The following command uses the `--n-features` option to limit analysis to the first two genes from each input GFF file. The resulting image shows the level of variability observed across genes from each genome.
 
 ```
 pankmer reg_heatmap -i Sp_Chr19_index/ \
-  -r Sp_Chr19_genomes/Sp9509_oxford_v3_Chr19.fasta.gz Sp_Chr19_genomes/Sp9512_a02_genome_Chr19.fasta.gz \
-  -f Sp_Chr19_features/Sp9509_oxford_v3_Chr19.gff3.gz Sp_Chr19_features/Sp9512_a02_genes_Chr19.gff3.gz \
+  -r Sp_Chr19_genomes/Sp7498_HiC_Chr19.fasta.gz Sp_Chr19_genomes/Sp9509_oxford_v3_Chr19.fasta.gz Sp_Chr19_genomes/Sp9512_a02_genome_Chr19.fasta.gz \
+  -f Sp_Chr19_features/Sp7498_HiC_Chr19.gff.gz Sp_Chr19_features/Sp9509_oxford_v3_Chr19.gff3.gz Sp_Chr19_features/Sp9512_a02_genes_Chr19.gff3.gz \
   -o Sp_Chr19_gene_var.png \
   --n-features 2 \
   --height 3
 ```
 
 ![example heatmap](example/Sp_Chr19_gene_variability.png)
```

### Comparing `pankmer-0.12.8/PKG-INFO` & `pankmer-0.9.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,85 +1,76 @@
 Metadata-Version: 2.1
 Name: pankmer
-Version: 0.12.8
+Version: 0.9.0
+Summary: Generate a PanGenome given a set of genomes
+Author: Semar Petrus, Allen Mamerto, Nolan Hartwick
+Author-email: Anthony Aylward <aaylward@salk.edu>
+Project-URL: Homepage, https://gitlab.com/salk-tm/pankmer
+Project-URL: Documentation, https://salk-tm.gitlab.io/pankmer
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: BSD License
-Requires-Dist: biopython
-Requires-Dist: gff2bed
-Requires-Dist: newick
-Requires-Dist: pyfaidx
-Requires-Dist: scipy
-Requires-Dist: seaborn
-Requires-Dist: urllib3
-Requires-Dist: upsetplot
-Requires-Dist: pybedtools
+Requires-Python: <3.11,>=3.8
+Description-Content-Type: text/markdown
 License-File: LICENSE
-Summary: Generate a PanGenome given a set of genomes
-Author: Semar Petrus, Allen Mamerto, Nolan Hartwick
-Author-email: Anthony Aylward <aaylward@salk.edu>
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
-Project-URL: Homepage, https://gitlab.com/salk-tm/pankmer
-Project-URL: Documentation, https://salk-tm.gitlab.io/pankmer
 
 Primary contact: Anthony Aylward, aaylward@salk.edu
 
 # PanKmer
 
 _k_-mer based and reference-free pangenome analysis. See the quickstart below, or read the [documentation](https://salk-tm.gitlab.io/pankmer/index.html).
 
 ## Installation
+### With pip
+```
+pip install git+https://gitlab.com/salk-tm/pankmer.git
+```
+
 ### In a conda environment
 First create an environment that includes all dependencies:
 ```
-conda create -c conda-forge -c bioconda -n pankmer rust python \
-  biopython seaborn urllib3 python-newick pyfaidx gff2bed upsetplot \
-  pybedtools
+conda create -c conda-forge -c bioconda -n pankmer python==3.10 biopython==1.79 cython pandas setuptools seaborn urllib3 wheel python-newick pyfaidx gff2bed
 ```
-Then install PanKmer with `pip`:
+If running on OSX, a few additional packages will be required:
 ```
 conda activate pankmer
-pip install pankmer
+conda install -c conda-forge clang_osx-64 clangxx_osx-64 gfortran_osx-64
 ```
-
-### With pip
-PanKmer is built with [Rust](https://doc.rust-lang.org/stable/book/title-page.html),
-so you will need to [install](https://doc.rust-lang.org/stable/book/ch01-01-installation.html)
-it if you have not already done so. Then you can install PanKmer with `pip`:
+Then install PanKmer with pip:
 ```
-pip install pankmer
+conda activate pankmer
+pip install pip install git+https://gitlab.com/salk-tm/pankmer.git
 ```
 
 ### Check installation
 Check that the installation was successful by running:
 ```
 pankmer --version
 ```
 
 ## Tutorial
 ### Download example dataset
 
-The `download-example` subcommand will download a small example dataset of
+The `download_example` subcommand will download a small example dataset of
 Chr19 sequences from _S. polyrhiza._
 ```
-pankmer download-example -d .
+pankmer download_example -d .
 ```
 After running this command the directory `PanKmer_example_Sp_Chr19/` will be present in the working directory. It contains FASTA files representing Chr19 from three genomes, and GFF files giving their gene annotations.
 ```
 ls PanKmer_example_Sp_Chr19/*
 ```
 ```
 PanKmer_example_Sp_Chr19/README.md
 
 PanKmer_example_Sp_Chr19/Sp_Chr19_features:
-Sp9509_oxford_v3_Chr19.gff3.gz Sp9512_a02_genes_Chr19.gff3.gz
+Sp7498_HiC_Chr19.gff.gz Sp9509_oxford_v3_Chr19.gff3.gz Sp9512_a02_genes_Chr19.gff3.gz
 
 PanKmer_example_Sp_Chr19/Sp_Chr19_genomes:
 Sp7498_HiC_Chr19.fasta.gz Sp9509_oxford_v3_Chr19.fasta.gz Sp9512_a02_genome_Chr19.fasta.gz
 ```
 
 To get started, navigate to the downloaded directory.
 ```
@@ -102,26 +93,25 @@
 Sp_Chr19_index/
 Sp_Chr19_index/kmers.b.gz
 Sp_Chr19_index/metadata.json
 Sp_Chr19_index/scores.b.gz
 ```
 
 > #### Note
-> The input genomes argument proided with the `-g` flag can be a directory, a tar archive, or a space-separated list of FASTA files.
+> The input genomes argument proided with the `-g` flag can be a directory, a tar archive, or a comma-separated list of FASTA files.
 >
 > If the output argument provided with the `-o` flag ends with `.tar`, then the index will be written as a tar archive. Otherwise it will be written as a directory.
 
 
 ### Create an adjacency matrix
 
-A useful application of the _k_-mer index is to generate an adjacency matrix. This is a table of _k_-mer similarity values for each pair of genomes in the index. We can generate one using the `adj-matrix` subcommand, which will produce a CSV or TSV file containing the matrix.
+A useful application of the _k_-mer index is to generate an adjacency matrix. This is a table of _k_-mer similarity values for each pair of genomes in the index. We can generate one using the `adj-matrix` subcommand, which will produce a CSV file containing the matrix.
 
 ```
 pankmer adj-matrix -i Sp_Chr19_index.tar -o Sp_Chr19_adj_matrix.csv
-pankmer adj-matrix -i Sp_Chr19_index.tar -o Sp_Chr19_adj_matrix.tsv
 ```
 
 > #### Note
 > The input index argument proided with the `-i` flag can be tar archive or a directory.
 
 ### Plot a clustered heatmap
 
@@ -135,20 +125,19 @@
   --height 6.5
 ```
 
 ![example heatmap](docs/source/_static/Sp_Chr19_adj_matrix.svg)
 
 ### Generate a gene variability heatmap
 
-Generate a heatmap showing variability of genes across genomes. The following command uses the `--n-features` option to limit analysis to the first two genes from each input GFF3 file. The resulting image shows the level of variability observed across genes from each genome.
+Generate a heatmap showing variability of genes across genomes. The following command uses the `--n-features` option to limit analysis to the first two genes from each input GFF file. The resulting image shows the level of variability observed across genes from each genome.
 
 ```
 pankmer reg_heatmap -i Sp_Chr19_index/ \
-  -r Sp_Chr19_genomes/Sp9509_oxford_v3_Chr19.fasta.gz Sp_Chr19_genomes/Sp9512_a02_genome_Chr19.fasta.gz \
-  -f Sp_Chr19_features/Sp9509_oxford_v3_Chr19.gff3.gz Sp_Chr19_features/Sp9512_a02_genes_Chr19.gff3.gz \
+  -r Sp_Chr19_genomes/Sp7498_HiC_Chr19.fasta.gz Sp_Chr19_genomes/Sp9509_oxford_v3_Chr19.fasta.gz Sp_Chr19_genomes/Sp9512_a02_genome_Chr19.fasta.gz \
+  -f Sp_Chr19_features/Sp7498_HiC_Chr19.gff.gz Sp_Chr19_features/Sp9509_oxford_v3_Chr19.gff3.gz Sp_Chr19_features/Sp9512_a02_genes_Chr19.gff3.gz \
   -o Sp_Chr19_gene_var.png \
   --n-features 2 \
   --height 3
 ```
 
 ![example heatmap](example/Sp_Chr19_gene_variability.png)
-
```

