# Comparing `tmp/glue-genes-1.0.1.tar.gz` & `tmp/glue-genes-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "glue-genes-1.0.1.tar", last modified: Tue Mar 21 15:38:56 2023, max compression
+gzip compressed data, was "glue-genes-1.1.0.tar", last modified: Wed Jun 14 20:21:23 2023, max compression
```

## Comparing `glue-genes-1.0.1.tar` & `glue-genes-1.1.0.tar`

### file list

```diff
@@ -1,153 +1,166 @@
-drwxr-xr-x   0 jfoster    (501) staff       (20)        0 2023-03-21 15:38:56.895455 glue-genes-1.0.1/
-drwxr-xr-x   0 jfoster    (501) staff       (20)        0 2023-03-21 15:38:56.842433 glue-genes-1.0.1/.github/
-drwxr-xr-x   0 jfoster    (501) staff       (20)        0 2023-03-21 15:38:56.846009 glue-genes-1.0.1/.github/workflows/
--rw-r--r--   0 jfoster    (501) staff       (20)     1198 2023-03-21 15:20:59.000000 glue-genes-1.0.1/.github/workflows/ci_workflows.yml
--rw-r--r--   0 jfoster    (501) staff       (20)      513 2023-03-21 15:20:59.000000 glue-genes-1.0.1/.github/workflows/python-package-conda.yml
--rw-r--r--   0 jfoster    (501) staff       (20)     1071 2023-03-21 15:20:59.000000 glue-genes-1.0.1/.github/workflows/static.yml
--rw-r--r--   0 jfoster    (501) staff       (20)     3148 2023-02-01 16:07:58.000000 glue-genes-1.0.1/.gitignore
--rw-r--r--   0 jfoster    (501) staff       (20)      221 2023-03-21 15:20:59.000000 glue-genes-1.0.1/.readthedocs.yml
--rw-r--r--   0 jfoster    (501) staff       (20)       90 2023-02-01 16:08:32.000000 glue-genes-1.0.1/CHANGES.md
--rw-r--r--   0 jfoster    (501) staff       (20)     1571 2023-02-01 16:07:58.000000 glue-genes-1.0.1/LICENSE
--rw-r--r--   0 jfoster    (501) staff       (20)     2425 2023-03-21 15:38:56.895567 glue-genes-1.0.1/PKG-INFO
--rw-r--r--   0 jfoster    (501) staff       (20)     1572 2023-03-21 15:20:59.000000 glue-genes-1.0.1/README.md
-drwxr-xr-x   0 jfoster    (501) staff       (20)        0 2023-03-21 15:38:56.846476 glue-genes-1.0.1/docs/
--rw-r--r--   0 jfoster    (501) staff       (20)      638 2023-02-01 16:07:58.000000 glue-genes-1.0.1/docs/Makefile
--rw-r--r--   0 jfoster    (501) staff       (20)      804 2023-02-01 16:07:58.000000 glue-genes-1.0.1/docs/make.bat
--rw-r--r--   0 jfoster    (501) staff       (20)       65 2023-02-01 16:07:58.000000 glue-genes-1.0.1/docs/requirements.txt
-drwxr-xr-x   0 jfoster    (501) staff       (20)        0 2023-03-21 15:38:56.846882 glue-genes-1.0.1/docs/source/
-drwxr-xr-x   0 jfoster    (501) staff       (20)        0 2023-03-21 15:38:56.847004 glue-genes-1.0.1/docs/source/_static/
--rw-r--r--   0 jfoster    (501) staff       (20)      128 2023-02-01 16:07:58.000000 glue-genes-1.0.1/docs/source/_static/style.css
-drwxr-xr-x   0 jfoster    (501) staff       (20)        0 2023-03-21 15:38:56.847135 glue-genes-1.0.1/docs/source/api/
--rw-r--r--   0 jfoster    (501) staff       (20)      286 2023-02-01 16:07:58.000000 glue-genes-1.0.1/docs/source/api/index.rst
-drwxr-xr-x   0 jfoster    (501) staff       (20)        0 2023-03-21 15:38:56.848018 glue-genes-1.0.1/docs/source/api/reference/
--rw-r--r--   0 jfoster    (501) staff       (20)      728 2023-02-01 16:08:32.000000 glue-genes-1.0.1/docs/source/api/reference/analysis.rst
-drwxr-xr-x   0 jfoster    (501) staff       (20)        0 2023-03-21 15:38:56.849800 glue-genes-1.0.1/docs/source/api/reference/api/
--rw-r--r--   0 jfoster    (501) staff       (20)      204 2023-02-01 16:08:32.000000 glue-genes-1.0.1/docs/source/api/reference/api/glue_genes.glue_genomics_data.bed_factory.read_bed.rst
--rw-r--r--   0 jfoster    (501) staff       (20)      222 2023-02-01 16:08:32.000000 glue-genes-1.0.1/docs/source/api/reference/api/glue_genes.glue_genomics_data.bigwig_factory.read_bigwig.rst
--rw-r--r--   0 jfoster    (501) staff       (20)      222 2023-02-01 16:08:32.000000 glue-genes-1.0.1/docs/source/api/reference/api/glue_genes.glue_single_cell.anndata_factory.read_anndata.rst
--rw-r--r--   0 jfoster    (501) staff       (20)     1939 2023-02-01 16:08:32.000000 glue-genes-1.0.1/docs/source/api/reference/api/glue_genes.glue_single_cell.data.DataAnnData.rst
--rw-r--r--   0 jfoster    (501) staff       (20)      477 2023-02-01 16:08:32.000000 glue-genes-1.0.1/docs/source/api/reference/api/glue_genes.glue_single_cell.data.DataAnnDataTranslator.rst
--rw-r--r--   0 jfoster    (501) staff       (20)      263 2023-02-01 16:08:32.000000 glue-genes-1.0.1/docs/source/api/reference/api/glue_genes.glue_single_cell.qt.diff_gene_exp.get_gene_list_diff_exp.rst
--rw-r--r--   0 jfoster    (501) staff       (20)      660 2023-02-01 16:08:32.000000 glue-genes-1.0.1/docs/source/api/reference/api/glue_genes.glue_single_cell.qt.pca_subset.GeneSummaryListener.rst
--rw-r--r--   0 jfoster    (501) staff       (20)      279 2023-02-01 16:08:32.000000 glue-genes-1.0.1/docs/source/api/reference/api/glue_genes.glue_single_cell.qt.pca_subset.do_calculation_over_gene_subset.rst
--rw-r--r--   0 jfoster    (501) staff       (20)     1196 2023-02-01 16:08:32.000000 glue-genes-1.0.1/docs/source/api/reference/api/glue_genes.glue_single_cell.qtl_viewer.layer_artist.QTLLayerArtist.rst
--rw-r--r--   0 jfoster    (501) staff       (20)     2279 2023-02-01 16:08:32.000000 glue-genes-1.0.1/docs/source/api/reference/api/glue_genes.glue_single_cell.qtl_viewer.state.QTLViewerState.rst
--rw-r--r--   0 jfoster    (501) staff       (20)    13919 2023-02-01 16:08:32.000000 glue-genes-1.0.1/docs/source/api/reference/api/glue_genes.glue_single_cell.qtl_viewer.viewer.QTLViewer.rst
--rw-r--r--   0 jfoster    (501) staff       (20)      474 2023-02-01 16:08:32.000000 glue-genes-1.0.1/docs/source/api/reference/io.rst
--rw-r--r--   0 jfoster    (501) staff       (20)      362 2023-02-01 16:08:32.000000 glue-genes-1.0.1/docs/source/api/reference/singlecelldata.rst
--rw-r--r--   0 jfoster    (501) staff       (20)      465 2023-03-21 15:20:59.000000 glue-genes-1.0.1/docs/source/api/reference/viewers.rst
--rw-r--r--   0 jfoster    (501) staff       (20)     2692 2023-02-01 16:07:58.000000 glue-genes-1.0.1/docs/source/conf.py
-drwxr-xr-x   0 jfoster    (501) staff       (20)        0 2023-03-21 15:38:56.849954 glue-genes-1.0.1/docs/source/getting-started/
--rw-r--r--   0 jfoster    (501) staff       (20)     1940 2023-03-21 15:20:59.000000 glue-genes-1.0.1/docs/source/getting-started/index.rst
-drwxr-xr-x   0 jfoster    (501) staff       (20)        0 2023-03-21 15:38:56.851097 glue-genes-1.0.1/docs/source/how-to/
--rw-r--r--   0 jfoster    (501) staff       (20)     4324 2023-02-01 16:07:58.000000 glue-genes-1.0.1/docs/source/how-to/cells-to-genes.rst
--rw-r--r--   0 jfoster    (501) staff       (20)     1970 2023-02-01 16:07:58.000000 glue-genes-1.0.1/docs/source/how-to/data-in.rst
-drwxr-xr-x   0 jfoster    (501) staff       (20)        0 2023-03-21 15:38:56.857123 glue-genes-1.0.1/docs/source/how-to/images/
--rw-r--r--   0 jfoster    (501) staff       (20)   112508 2023-02-01 16:07:58.000000 glue-genes-1.0.1/docs/source/how-to/images/connect_choose_plugin.png
--rw-r--r--   0 jfoster    (501) staff       (20)   135183 2023-02-01 16:07:58.000000 glue-genes-1.0.1/docs/source/how-to/images/connect_create_gene_subset.png
--rw-r--r--   0 jfoster    (501) staff       (20)   119197 2023-02-01 16:07:58.000000 glue-genes-1.0.1/docs/source/how-to/images/connect_dge_dialog.png
--rw-r--r--   0 jfoster    (501) staff       (20)    37239 2023-02-01 16:07:58.000000 glue-genes-1.0.1/docs/source/how-to/images/connect_dge_menubar.png
--rw-r--r--   0 jfoster    (501) staff       (20)    74465 2023-02-01 16:07:58.000000 glue-genes-1.0.1/docs/source/how-to/images/connect_summary_dialog.png
--rw-r--r--   0 jfoster    (501) staff       (20)    83263 2023-02-01 16:07:58.000000 glue-genes-1.0.1/docs/source/how-to/images/create_from_data_manager.png
--rw-r--r--   0 jfoster    (501) staff       (20)    53447 2023-02-01 16:07:58.000000 glue-genes-1.0.1/docs/source/how-to/images/create_new_viewer.png
--rw-r--r--   0 jfoster    (501) staff       (20)   125108 2023-02-01 16:07:58.000000 glue-genes-1.0.1/docs/source/how-to/images/drag_to_create.gif
--rw-r--r--   0 jfoster    (501) staff       (20)    97386 2023-02-01 16:07:58.000000 glue-genes-1.0.1/docs/source/how-to/images/link_data_join_on_key.png
--rw-r--r--   0 jfoster    (501) staff       (20)   189126 2023-02-01 16:07:58.000000 glue-genes-1.0.1/docs/source/how-to/images/link_data_join_on_key_done.png
--rw-r--r--   0 jfoster    (501) staff       (20)    41081 2023-02-01 16:07:58.000000 glue-genes-1.0.1/docs/source/how-to/images/link_data_menu.png
--rw-r--r--   0 jfoster    (501) staff       (20)    20219 2023-02-01 16:07:58.000000 glue-genes-1.0.1/docs/source/how-to/images/link_data_toolbar.png
--rw-r--r--   0 jfoster    (501) staff       (20)   163667 2023-02-01 16:07:58.000000 glue-genes-1.0.1/docs/source/how-to/images/linking_attributes_step1.png
--rw-r--r--   0 jfoster    (501) staff       (20)   177252 2023-02-01 16:07:58.000000 glue-genes-1.0.1/docs/source/how-to/images/linking_attributes_step2.png
--rw-r--r--   0 jfoster    (501) staff       (20)   109823 2023-02-01 16:07:58.000000 glue-genes-1.0.1/docs/source/how-to/images/loading_options.png
--rw-r--r--   0 jfoster    (501) staff       (20)    21634 2023-02-01 16:07:58.000000 glue-genes-1.0.1/docs/source/how-to/images/open_data_set_icon.png
--rw-r--r--   0 jfoster    (501) staff       (20)    50506 2023-02-01 16:07:58.000000 glue-genes-1.0.1/docs/source/how-to/images/open_data_set_menu.png
--rw-r--r--   0 jfoster    (501) staff       (20)   183650 2023-02-01 16:07:58.000000 glue-genes-1.0.1/docs/source/how-to/images/single_cell_loading_options.png
--rw-r--r--   0 jfoster    (501) staff       (20)     1018 2023-02-01 16:07:58.000000 glue-genes-1.0.1/docs/source/how-to/index.rst
--rw-r--r--   0 jfoster    (501) staff       (20)      444 2023-03-21 15:20:59.000000 glue-genes-1.0.1/docs/source/how-to/installation.rst
--rw-r--r--   0 jfoster    (501) staff       (20)     5436 2023-03-21 15:20:59.000000 glue-genes-1.0.1/docs/source/how-to/linking-data.rst
--rw-r--r--   0 jfoster    (501) staff       (20)      962 2023-02-01 16:07:58.000000 glue-genes-1.0.1/docs/source/how-to/starting.rst
--rw-r--r--   0 jfoster    (501) staff       (20)     2172 2023-02-01 16:07:58.000000 glue-genes-1.0.1/docs/source/how-to/visualize-data.rst
-drwxr-xr-x   0 jfoster    (501) staff       (20)        0 2023-03-21 15:38:56.858557 glue-genes-1.0.1/docs/source/images/
--rw-r--r--   0 jfoster    (501) staff       (20)      399 2023-02-01 16:07:58.000000 glue-genes-1.0.1/docs/source/images/api_reference.svg
--rw-r--r--   0 jfoster    (501) staff       (20)     1476 2023-02-01 16:07:58.000000 glue-genes-1.0.1/docs/source/images/favicon.png
--rw-r--r--   0 jfoster    (501) staff       (20)      307 2023-02-01 16:07:58.000000 glue-genes-1.0.1/docs/source/images/getting_started.svg
--rw-r--r--   0 jfoster    (501) staff       (20)    17810 2023-02-01 16:07:58.000000 glue-genes-1.0.1/docs/source/images/glue_genes_icon.png
--rw-r--r--   0 jfoster    (501) staff       (20)    25278 2023-02-01 16:07:58.000000 glue-genes-1.0.1/docs/source/images/glue_genes_logo_stacked.png
--rw-r--r--   0 jfoster    (501) staff       (20)      334 2023-02-01 16:07:58.000000 glue-genes-1.0.1/docs/source/images/how_to.svg
--rw-r--r--   0 jfoster    (501) staff       (20)      209 2023-02-01 16:07:58.000000 glue-genes-1.0.1/docs/source/images/user_guide.svg
--rw-r--r--   0 jfoster    (501) staff       (20)     2986 2023-03-21 15:20:59.000000 glue-genes-1.0.1/docs/source/index.rst
-drwxr-xr-x   0 jfoster    (501) staff       (20)        0 2023-03-21 15:38:56.858717 glue-genes-1.0.1/docs/source/user-guide/
-drwxr-xr-x   0 jfoster    (501) staff       (20)        0 2023-03-21 15:38:56.859889 glue-genes-1.0.1/docs/source/user-guide/images/
--rw-r--r--   0 jfoster    (501) staff       (20)    90590 2023-02-01 16:07:58.000000 glue-genes-1.0.1/docs/source/user-guide/images/enrichr.png
--rw-r--r--   0 jfoster    (501) staff       (20)   113749 2023-02-01 16:07:58.000000 glue-genes-1.0.1/docs/source/user-guide/images/qtl_viewer.png
--rw-r--r--   0 jfoster    (501) staff       (20)   123788 2023-02-01 16:07:58.000000 glue-genes-1.0.1/docs/source/user-guide/images/single_cell_schematic.png
--rw-r--r--   0 jfoster    (501) staff       (20)    93300 2023-02-01 16:07:58.000000 glue-genes-1.0.1/docs/source/user-guide/images/small_multiples_viewer.png
--rw-r--r--   0 jfoster    (501) staff       (20)     5764 2023-02-01 16:07:58.000000 glue-genes-1.0.1/docs/source/user-guide/index.rst
--rw-r--r--   0 jfoster    (501) staff       (20)      178 2023-03-21 15:20:59.000000 glue-genes-1.0.1/environment.yml
-drwxr-xr-x   0 jfoster    (501) staff       (20)        0 2023-03-21 15:38:56.860742 glue-genes-1.0.1/glue_genes/
--rw-r--r--   0 jfoster    (501) staff       (20)        0 2023-02-01 16:08:32.000000 glue-genes-1.0.1/glue_genes/__init__.py
-drwxr-xr-x   0 jfoster    (501) staff       (20)        0 2023-03-21 15:38:56.863065 glue-genes-1.0.1/glue_genes/glue_genomics_data/
--rw-r--r--   0 jfoster    (501) staff       (20)      111 2023-02-01 16:08:32.000000 glue-genes-1.0.1/glue_genes/glue_genomics_data/__init__.py
--rw-r--r--   0 jfoster    (501) staff       (20)     1325 2023-02-01 16:08:32.000000 glue-genes-1.0.1/glue_genes/glue_genomics_data/bed_factory.py
--rw-r--r--   0 jfoster    (501) staff       (20)     1347 2023-02-01 16:08:32.000000 glue-genes-1.0.1/glue_genes/glue_genomics_data/bigwig_factory.py
-drwxr-xr-x   0 jfoster    (501) staff       (20)        0 2023-03-21 15:38:56.863910 glue-genes-1.0.1/glue_genes/glue_single_cell/
--rw-r--r--   0 jfoster    (501) staff       (20)     1995 2023-02-01 16:08:32.000000 glue-genes-1.0.1/glue_genes/glue_single_cell/__init__.py
--rw-r--r--   0 jfoster    (501) staff       (20)     9970 2023-03-21 15:20:59.000000 glue-genes-1.0.1/glue_genes/glue_single_cell/anndata_factory.py
--rw-r--r--   0 jfoster    (501) staff       (20)    20427 2023-03-21 15:20:59.000000 glue-genes-1.0.1/glue_genes/glue_single_cell/data.py
--rw-r--r--   0 jfoster    (501) staff       (20)      742 2023-02-01 16:08:32.000000 glue-genes-1.0.1/glue_genes/glue_single_cell/menubar_plugin.py
-drwxr-xr-x   0 jfoster    (501) staff       (20)        0 2023-03-21 15:38:56.865072 glue-genes-1.0.1/glue_genes/glue_single_cell/qt/
--rw-r--r--   0 jfoster    (501) staff       (20)        0 2023-02-01 16:08:32.000000 glue-genes-1.0.1/glue_genes/glue_single_cell/qt/__init__.py
--rw-r--r--   0 jfoster    (501) staff       (20)     5880 2023-02-01 16:08:32.000000 glue-genes-1.0.1/glue_genes/glue_single_cell/qt/diff_gene_exp.py
--rw-r--r--   0 jfoster    (501) staff       (20)     4978 2023-02-01 16:08:32.000000 glue-genes-1.0.1/glue_genes/glue_single_cell/qt/diff_gene_exp.ui
--rw-r--r--   0 jfoster    (501) staff       (20)     3351 2023-02-01 16:08:32.000000 glue-genes-1.0.1/glue_genes/glue_single_cell/qt/enrichr.py
--rw-r--r--   0 jfoster    (501) staff       (20)     3756 2023-02-01 16:08:32.000000 glue-genes-1.0.1/glue_genes/glue_single_cell/qt/enrichr.ui
--rw-r--r--   0 jfoster    (501) staff       (20)     8402 2023-02-01 16:08:32.000000 glue-genes-1.0.1/glue_genes/glue_single_cell/qt/load_data.py
--rw-r--r--   0 jfoster    (501) staff       (20)     8637 2023-02-01 16:08:32.000000 glue-genes-1.0.1/glue_genes/glue_single_cell/qt/load_data.ui
--rw-r--r--   0 jfoster    (501) staff       (20)    11045 2023-02-01 16:08:32.000000 glue-genes-1.0.1/glue_genes/glue_single_cell/qt/pca_subset.py
--rw-r--r--   0 jfoster    (501) staff       (20)     3779 2023-02-01 16:08:32.000000 glue-genes-1.0.1/glue_genes/glue_single_cell/qt/pca_subset.ui
-drwxr-xr-x   0 jfoster    (501) staff       (20)        0 2023-03-21 15:38:56.865881 glue-genes-1.0.1/glue_genes/glue_single_cell/qt/tests/
--rw-r--r--   0 jfoster    (501) staff       (20)        0 2023-02-01 16:08:32.000000 glue-genes-1.0.1/glue_genes/glue_single_cell/qt/tests/__init__.py
-drwxr-xr-x   0 jfoster    (501) staff       (20)        0 2023-03-21 15:38:56.873359 glue-genes-1.0.1/glue_genes/glue_single_cell/qt/tests/data/
--rw-r--r--   0 jfoster    (501) staff       (20)  1222520 2023-02-01 16:08:32.000000 glue-genes-1.0.1/glue_genes/glue_single_cell/qt/tests/data/test_data.h5ad
--rw-r--r--   0 jfoster    (501) staff       (20)   430945 2023-02-01 16:08:32.000000 glue-genes-1.0.1/glue_genes/glue_single_cell/qt/tests/data/test_data_compressed.h5ad
--rw-r--r--   0 jfoster    (501) staff       (20)  1001104 2023-02-01 16:08:32.000000 glue-genes-1.0.1/glue_genes/glue_single_cell/qt/tests/data/test_data_dense.h5ad
--rw-r--r--   0 jfoster    (501) staff       (20)   298998 2023-02-01 16:08:32.000000 glue-genes-1.0.1/glue_genes/glue_single_cell/qt/tests/data/test_data_dense_compressed.h5ad
--rw-r--r--   0 jfoster    (501) staff       (20)  5312200 2023-02-01 16:08:32.000000 glue-genes-1.0.1/glue_genes/glue_single_cell/qt/tests/data/test_other_data.h5ad
--rw-r--r--   0 jfoster    (501) staff       (20)     5850 2023-02-01 16:08:32.000000 glue-genes-1.0.1/glue_genes/glue_single_cell/qt/tests/test_data_load.py
--rw-r--r--   0 jfoster    (501) staff       (20)     1675 2023-02-01 16:08:32.000000 glue-genes-1.0.1/glue_genes/glue_single_cell/qt/tests/test_diff_gene_exp.py
--rw-r--r--   0 jfoster    (501) staff       (20)     1827 2023-02-01 16:08:32.000000 glue-genes-1.0.1/glue_genes/glue_single_cell/qt/tests/test_enrichr.py
--rw-r--r--   0 jfoster    (501) staff       (20)    10628 2023-02-01 16:08:32.000000 glue-genes-1.0.1/glue_genes/glue_single_cell/qt/tests/test_pca_subset.py
-drwxr-xr-x   0 jfoster    (501) staff       (20)        0 2023-03-21 15:38:56.887036 glue-genes-1.0.1/glue_genes/glue_single_cell/qtl_viewer/
--rw-r--r--   0 jfoster    (501) staff       (20)        0 2023-02-01 16:08:32.000000 glue-genes-1.0.1/glue_genes/glue_single_cell/qtl_viewer/__init__.py
--rw-r--r--   0 jfoster    (501) staff       (20)    12306 2023-03-21 15:20:59.000000 glue-genes-1.0.1/glue_genes/glue_single_cell/qtl_viewer/layer_artist.py
-drwxr-xr-x   0 jfoster    (501) staff       (20)        0 2023-03-21 15:38:56.888980 glue-genes-1.0.1/glue_genes/glue_single_cell/qtl_viewer/qt/
--rw-r--r--   0 jfoster    (501) staff       (20)        0 2023-02-01 16:08:32.000000 glue-genes-1.0.1/glue_genes/glue_single_cell/qtl_viewer/qt/__init__.py
--rw-r--r--   0 jfoster    (501) staff       (20)     6437 2023-02-01 16:08:32.000000 glue-genes-1.0.1/glue_genes/glue_single_cell/qtl_viewer/qt/layer_style_editor.py
--rw-r--r--   0 jfoster    (501) staff       (20)    17774 2023-02-01 16:08:32.000000 glue-genes-1.0.1/glue_genes/glue_single_cell/qtl_viewer/qt/layer_style_editor.ui
--rw-r--r--   0 jfoster    (501) staff       (20)     4308 2023-02-01 16:08:32.000000 glue-genes-1.0.1/glue_genes/glue_single_cell/qtl_viewer/qt/options_widget.py
--rw-r--r--   0 jfoster    (501) staff       (20)    10208 2023-02-01 16:08:32.000000 glue-genes-1.0.1/glue_genes/glue_single_cell/qtl_viewer/qt/options_widget.ui
--rw-r--r--   0 jfoster    (501) staff       (20)     2023 2023-02-01 16:08:32.000000 glue-genes-1.0.1/glue_genes/glue_single_cell/qtl_viewer/qt/slider_with_label_widget.ui
--rw-r--r--   0 jfoster    (501) staff       (20)     5385 2023-02-01 16:08:32.000000 glue-genes-1.0.1/glue_genes/glue_single_cell/qtl_viewer/state.py
-drwxr-xr-x   0 jfoster    (501) staff       (20)        0 2023-03-21 15:38:56.889217 glue-genes-1.0.1/glue_genes/glue_single_cell/qtl_viewer/tests/
--rw-r--r--   0 jfoster    (501) staff       (20)        0 2023-02-01 16:08:32.000000 glue-genes-1.0.1/glue_genes/glue_single_cell/qtl_viewer/tests/__init__.py
--rw-r--r--   0 jfoster    (501) staff       (20)     5423 2023-02-01 16:08:32.000000 glue-genes-1.0.1/glue_genes/glue_single_cell/qtl_viewer/tests/test_qtl_data_viewer.py
--rw-r--r--   0 jfoster    (501) staff       (20)     5056 2023-03-21 15:20:59.000000 glue-genes-1.0.1/glue_genes/glue_single_cell/qtl_viewer/viewer.py
--rw-r--r--   0 jfoster    (501) staff       (20)     5438 2023-03-21 15:20:59.000000 glue-genes-1.0.1/glue_genes/glue_single_cell/state.py
-drwxr-xr-x   0 jfoster    (501) staff       (20)        0 2023-03-21 15:38:56.889728 glue-genes-1.0.1/glue_genes/glue_single_cell/tests/
--rw-r--r--   0 jfoster    (501) staff       (20)      105 2023-02-01 16:08:32.000000 glue-genes-1.0.1/glue_genes/glue_single_cell/tests/context.py
-drwxr-xr-x   0 jfoster    (501) staff       (20)        0 2023-03-21 15:38:56.894547 glue-genes-1.0.1/glue_genes/glue_single_cell/tests/test_data/
--rw-r--r--   0 jfoster    (501) staff       (20)  1222520 2023-02-01 16:08:32.000000 glue-genes-1.0.1/glue_genes/glue_single_cell/tests/test_data/test_data.h5ad
--rw-r--r--   0 jfoster    (501) staff       (20)   360068 2023-02-01 16:08:32.000000 glue-genes-1.0.1/glue_genes/glue_single_cell/tests/test_data/test_dataset.h5ad
--rw-r--r--   0 jfoster    (501) staff       (20)   364036 2023-02-01 16:08:32.000000 glue-genes-1.0.1/glue_genes/glue_single_cell/tests/test_data/test_dataset_float32.h5ad
--rw-r--r--   0 jfoster    (501) staff       (20)     4960 2023-02-01 16:08:32.000000 glue-genes-1.0.1/glue_genes/glue_single_cell/tests/test_data_math.py
-drwxr-xr-x   0 jfoster    (501) staff       (20)        0 2023-03-21 15:38:56.862315 glue-genes-1.0.1/glue_genes.egg-info/
--rw-r--r--   0 jfoster    (501) staff       (20)     2425 2023-03-21 15:38:56.000000 glue-genes-1.0.1/glue_genes.egg-info/PKG-INFO
--rw-r--r--   0 jfoster    (501) staff       (20)     5831 2023-03-21 15:38:56.000000 glue-genes-1.0.1/glue_genes.egg-info/SOURCES.txt
--rw-r--r--   0 jfoster    (501) staff       (20)        1 2023-03-21 15:38:56.000000 glue-genes-1.0.1/glue_genes.egg-info/dependency_links.txt
--rw-r--r--   0 jfoster    (501) staff       (20)      125 2023-03-21 15:38:56.000000 glue-genes-1.0.1/glue_genes.egg-info/entry_points.txt
--rw-r--r--   0 jfoster    (501) staff       (20)        1 2023-02-01 16:09:28.000000 glue-genes-1.0.1/glue_genes.egg-info/not-zip-safe
--rw-r--r--   0 jfoster    (501) staff       (20)      309 2023-03-21 15:38:56.000000 glue-genes-1.0.1/glue_genes.egg-info/requires.txt
--rw-r--r--   0 jfoster    (501) staff       (20)       11 2023-03-21 15:38:56.000000 glue-genes-1.0.1/glue_genes.egg-info/top_level.txt
--rw-r--r--   0 jfoster    (501) staff       (20)      190 2023-03-21 15:33:48.000000 glue-genes-1.0.1/pyproject.toml
--rw-r--r--   0 jfoster    (501) staff       (20)     2081 2023-03-21 15:38:56.896034 glue-genes-1.0.1/setup.cfg
--rwxr-xr-x   0 jfoster    (501) staff       (20)      398 2023-02-01 16:07:58.000000 glue-genes-1.0.1/setup.py
--rw-r--r--   0 jfoster    (501) staff       (20)      825 2023-02-01 16:08:32.000000 glue-genes-1.0.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 20:21:23.473149 glue-genes-1.1.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 20:21:23.401149 glue-genes-1.1.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-06-14 20:20:33.000000 glue-genes-1.1.0/.github/release.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 20:21:23.405149 glue-genes-1.1.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-06-14 20:20:33.000000 glue-genes-1.1.0/.github/workflows/ci_workflows.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-06-14 20:20:33.000000 glue-genes-1.1.0/.github/workflows/python-package-conda.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-14 20:20:33.000000 glue-genes-1.1.0/.github/workflows/static.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-06-14 20:20:33.000000 glue-genes-1.1.0/.github/workflows/update-changelog.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3148 2023-06-14 20:20:33.000000 glue-genes-1.1.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-06-14 20:20:33.000000 glue-genes-1.1.0/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-14 20:20:33.000000 glue-genes-1.1.0/CHANGES.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-06-14 20:20:33.000000 glue-genes-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2291 2023-06-14 20:21:23.473149 glue-genes-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-06-14 20:20:33.000000 glue-genes-1.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-06-14 20:20:33.000000 glue-genes-1.1.0/codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 20:21:23.405149 glue-genes-1.1.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-06-14 20:20:33.000000 glue-genes-1.1.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-06-14 20:20:33.000000 glue-genes-1.1.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-14 20:20:33.000000 glue-genes-1.1.0/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 20:21:23.405149 glue-genes-1.1.0/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 20:21:23.405149 glue-genes-1.1.0/docs/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-14 20:20:33.000000 glue-genes-1.1.0/docs/source/_static/style.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 20:21:23.405149 glue-genes-1.1.0/docs/source/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-06-14 20:20:33.000000 glue-genes-1.1.0/docs/source/api/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 20:21:23.409149 glue-genes-1.1.0/docs/source/api/reference/
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-06-14 20:20:33.000000 glue-genes-1.1.0/docs/source/api/reference/analysis.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 20:21:23.413149 glue-genes-1.1.0/docs/source/api/reference/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-06-14 20:20:33.000000 glue-genes-1.1.0/docs/source/api/reference/api/glue_genes.glue_genomics_data.bed_factory.read_bed.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-06-14 20:20:33.000000 glue-genes-1.1.0/docs/source/api/reference/api/glue_genes.glue_genomics_data.bigwig_factory.read_bigwig.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-06-14 20:20:33.000000 glue-genes-1.1.0/docs/source/api/reference/api/glue_genes.glue_single_cell.anndata_factory.read_anndata.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-06-14 20:20:33.000000 glue-genes-1.1.0/docs/source/api/reference/api/glue_genes.glue_single_cell.data.DataAnnData.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-06-14 20:20:33.000000 glue-genes-1.1.0/docs/source/api/reference/api/glue_genes.glue_single_cell.data.DataAnnDataTranslator.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-06-14 20:20:33.000000 glue-genes-1.1.0/docs/source/api/reference/api/glue_genes.glue_single_cell.qt.diff_gene_exp.get_gene_list_diff_exp.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-06-14 20:20:33.000000 glue-genes-1.1.0/docs/source/api/reference/api/glue_genes.glue_single_cell.qt.pca_subset.GeneSummaryListener.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-06-14 20:20:33.000000 glue-genes-1.1.0/docs/source/api/reference/api/glue_genes.glue_single_cell.qt.pca_subset.do_calculation_over_gene_subset.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-06-14 20:20:33.000000 glue-genes-1.1.0/docs/source/api/reference/api/glue_genes.glue_single_cell.qtl_viewer.layer_artist.QTLLayerArtist.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-06-14 20:20:33.000000 glue-genes-1.1.0/docs/source/api/reference/api/glue_genes.glue_single_cell.qtl_viewer.state.QTLViewerState.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    13919 2023-06-14 20:20:33.000000 glue-genes-1.1.0/docs/source/api/reference/api/glue_genes.glue_single_cell.qtl_viewer.viewer.QTLViewer.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-06-14 20:20:33.000000 glue-genes-1.1.0/docs/source/api/reference/io.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-06-14 20:20:33.000000 glue-genes-1.1.0/docs/source/api/reference/singlecelldata.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-06-14 20:20:33.000000 glue-genes-1.1.0/docs/source/api/reference/viewers.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2692 2023-06-14 20:20:33.000000 glue-genes-1.1.0/docs/source/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 20:21:23.413149 glue-genes-1.1.0/docs/source/getting-started/
+-rw-r--r--   0 runner    (1001) docker     (123)     1927 2023-06-14 20:20:33.000000 glue-genes-1.1.0/docs/source/getting-started/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 20:21:23.417149 glue-genes-1.1.0/docs/source/how-to/
+-rw-r--r--   0 runner    (1001) docker     (123)     4324 2023-06-14 20:20:33.000000 glue-genes-1.1.0/docs/source/how-to/cells-to-genes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-06-14 20:20:33.000000 glue-genes-1.1.0/docs/source/how-to/data-in.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 20:21:23.425149 glue-genes-1.1.0/docs/source/how-to/images/
+-rw-r--r--   0 runner    (1001) docker     (123)   112508 2023-06-14 20:20:33.000000 glue-genes-1.1.0/docs/source/how-to/images/connect_choose_plugin.png
+-rw-r--r--   0 runner    (1001) docker     (123)   135183 2023-06-14 20:20:33.000000 glue-genes-1.1.0/docs/source/how-to/images/connect_create_gene_subset.png
+-rw-r--r--   0 runner    (1001) docker     (123)   119197 2023-06-14 20:20:33.000000 glue-genes-1.1.0/docs/source/how-to/images/connect_dge_dialog.png
+-rw-r--r--   0 runner    (1001) docker     (123)    37239 2023-06-14 20:20:33.000000 glue-genes-1.1.0/docs/source/how-to/images/connect_dge_menubar.png
+-rw-r--r--   0 runner    (1001) docker     (123)    74465 2023-06-14 20:20:33.000000 glue-genes-1.1.0/docs/source/how-to/images/connect_summary_dialog.png
+-rw-r--r--   0 runner    (1001) docker     (123)    83263 2023-06-14 20:20:33.000000 glue-genes-1.1.0/docs/source/how-to/images/create_from_data_manager.png
+-rw-r--r--   0 runner    (1001) docker     (123)    53447 2023-06-14 20:20:33.000000 glue-genes-1.1.0/docs/source/how-to/images/create_new_viewer.png
+-rw-r--r--   0 runner    (1001) docker     (123)   125108 2023-06-14 20:20:33.000000 glue-genes-1.1.0/docs/source/how-to/images/drag_to_create.gif
+-rw-r--r--   0 runner    (1001) docker     (123)    97386 2023-06-14 20:20:33.000000 glue-genes-1.1.0/docs/source/how-to/images/link_data_join_on_key.png
+-rw-r--r--   0 runner    (1001) docker     (123)   189126 2023-06-14 20:20:33.000000 glue-genes-1.1.0/docs/source/how-to/images/link_data_join_on_key_done.png
+-rw-r--r--   0 runner    (1001) docker     (123)    41081 2023-06-14 20:20:33.000000 glue-genes-1.1.0/docs/source/how-to/images/link_data_menu.png
+-rw-r--r--   0 runner    (1001) docker     (123)    20219 2023-06-14 20:20:33.000000 glue-genes-1.1.0/docs/source/how-to/images/link_data_toolbar.png
+-rw-r--r--   0 runner    (1001) docker     (123)   163667 2023-06-14 20:20:33.000000 glue-genes-1.1.0/docs/source/how-to/images/linking_attributes_step1.png
+-rw-r--r--   0 runner    (1001) docker     (123)   177252 2023-06-14 20:20:33.000000 glue-genes-1.1.0/docs/source/how-to/images/linking_attributes_step2.png
+-rw-r--r--   0 runner    (1001) docker     (123)   109823 2023-06-14 20:20:33.000000 glue-genes-1.1.0/docs/source/how-to/images/loading_options.png
+-rw-r--r--   0 runner    (1001) docker     (123)    21634 2023-06-14 20:20:33.000000 glue-genes-1.1.0/docs/source/how-to/images/open_data_set_icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)    50506 2023-06-14 20:20:33.000000 glue-genes-1.1.0/docs/source/how-to/images/open_data_set_menu.png
+-rw-r--r--   0 runner    (1001) docker     (123)   183650 2023-06-14 20:20:33.000000 glue-genes-1.1.0/docs/source/how-to/images/single_cell_loading_options.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-06-14 20:20:33.000000 glue-genes-1.1.0/docs/source/how-to/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3135 2023-06-14 20:20:33.000000 glue-genes-1.1.0/docs/source/how-to/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5436 2023-06-14 20:20:33.000000 glue-genes-1.1.0/docs/source/how-to/linking-data.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-06-14 20:20:33.000000 glue-genes-1.1.0/docs/source/how-to/starting.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-06-14 20:20:33.000000 glue-genes-1.1.0/docs/source/how-to/visualize-data.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 20:21:23.429149 glue-genes-1.1.0/docs/source/images/
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-06-14 20:20:33.000000 glue-genes-1.1.0/docs/source/images/api_reference.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-06-14 20:20:33.000000 glue-genes-1.1.0/docs/source/images/favicon.png
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-06-14 20:20:33.000000 glue-genes-1.1.0/docs/source/images/getting_started.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    17810 2023-06-14 20:20:33.000000 glue-genes-1.1.0/docs/source/images/glue_genes_icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)    25278 2023-06-14 20:20:33.000000 glue-genes-1.1.0/docs/source/images/glue_genes_logo_stacked.png
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-06-14 20:20:33.000000 glue-genes-1.1.0/docs/source/images/how_to.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-06-14 20:20:33.000000 glue-genes-1.1.0/docs/source/images/user_guide.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2986 2023-06-14 20:20:33.000000 glue-genes-1.1.0/docs/source/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 20:21:23.429149 glue-genes-1.1.0/docs/source/user-guide/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 20:21:23.433149 glue-genes-1.1.0/docs/source/user-guide/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    90590 2023-06-14 20:20:33.000000 glue-genes-1.1.0/docs/source/user-guide/images/enrichr.png
+-rw-r--r--   0 runner    (1001) docker     (123)   113749 2023-06-14 20:20:33.000000 glue-genes-1.1.0/docs/source/user-guide/images/qtl_viewer.png
+-rw-r--r--   0 runner    (1001) docker     (123)   123788 2023-06-14 20:20:33.000000 glue-genes-1.1.0/docs/source/user-guide/images/single_cell_schematic.png
+-rw-r--r--   0 runner    (1001) docker     (123)    93300 2023-06-14 20:20:33.000000 glue-genes-1.1.0/docs/source/user-guide/images/small_multiples_viewer.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5764 2023-06-14 20:20:33.000000 glue-genes-1.1.0/docs/source/user-guide/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-06-14 20:20:33.000000 glue-genes-1.1.0/environment.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 20:21:23.433149 glue-genes-1.1.0/glue_genes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 20:20:33.000000 glue-genes-1.1.0/glue_genes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 20:21:23.441149 glue-genes-1.1.0/glue_genes/glue_genomics_data/
+-rw-r--r--   0 runner    (1001) docker     (123)      421 2023-06-14 20:20:33.000000 glue-genes-1.1.0/glue_genes/glue_genomics_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-06-14 20:20:33.000000 glue-genes-1.1.0/glue_genes/glue_genomics_data/bed_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-06-14 20:20:33.000000 glue-genes-1.1.0/glue_genes/glue_genomics_data/bigwig_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15412 2023-06-14 20:20:33.000000 glue-genes-1.1.0/glue_genes/glue_genomics_data/multires_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3481 2023-06-14 20:20:33.000000 glue-genes-1.1.0/glue_genes/glue_genomics_data/ome_zarr_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2215 2023-06-14 20:20:33.000000 glue-genes-1.1.0/glue_genes/glue_genomics_data/openslide_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5115 2023-06-14 20:20:33.000000 glue-genes-1.1.0/glue_genes/glue_genomics_data/spaceranger_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 20:21:23.441149 glue-genes-1.1.0/glue_genes/glue_genomics_data/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     8382 2023-06-14 20:20:33.000000 glue-genes-1.1.0/glue_genes/glue_genomics_data/tests/test_multi_resolution_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-06-14 20:20:33.000000 glue-genes-1.1.0/glue_genes/glue_genomics_data/zarr_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 20:21:23.445149 glue-genes-1.1.0/glue_genes/glue_single_cell/
+-rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-06-14 20:20:33.000000 glue-genes-1.1.0/glue_genes/glue_single_cell/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12571 2023-06-14 20:20:33.000000 glue-genes-1.1.0/glue_genes/glue_single_cell/anndata_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-06-14 20:20:33.000000 glue-genes-1.1.0/glue_genes/glue_single_cell/component.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20076 2023-06-14 20:20:33.000000 glue-genes-1.1.0/glue_genes/glue_single_cell/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-06-14 20:20:33.000000 glue-genes-1.1.0/glue_genes/glue_single_cell/menubar_plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 20:21:23.449149 glue-genes-1.1.0/glue_genes/glue_single_cell/qt/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 20:20:33.000000 glue-genes-1.1.0/glue_genes/glue_single_cell/qt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5890 2023-06-14 20:20:33.000000 glue-genes-1.1.0/glue_genes/glue_single_cell/qt/diff_gene_exp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5010 2023-06-14 20:20:33.000000 glue-genes-1.1.0/glue_genes/glue_single_cell/qt/diff_gene_exp.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     3361 2023-06-14 20:20:33.000000 glue-genes-1.1.0/glue_genes/glue_single_cell/qt/enrichr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3788 2023-06-14 20:20:33.000000 glue-genes-1.1.0/glue_genes/glue_single_cell/qt/enrichr.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     8402 2023-06-14 20:20:33.000000 glue-genes-1.1.0/glue_genes/glue_single_cell/qt/load_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8637 2023-06-14 20:20:33.000000 glue-genes-1.1.0/glue_genes/glue_single_cell/qt/load_data.ui
+-rw-r--r--   0 runner    (1001) docker     (123)    11251 2023-06-14 20:20:33.000000 glue-genes-1.1.0/glue_genes/glue_single_cell/qt/summarize_gene_subset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3816 2023-06-14 20:20:33.000000 glue-genes-1.1.0/glue_genes/glue_single_cell/qt/summarize_gene_subset.ui
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 20:21:23.449149 glue-genes-1.1.0/glue_genes/glue_single_cell/qt/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 20:20:33.000000 glue-genes-1.1.0/glue_genes/glue_single_cell/qt/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 20:21:23.457149 glue-genes-1.1.0/glue_genes/glue_single_cell/qt/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 20:20:33.000000 glue-genes-1.1.0/glue_genes/glue_single_cell/qt/tests/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1222520 2023-06-14 20:20:33.000000 glue-genes-1.1.0/glue_genes/glue_single_cell/qt/tests/data/test_data.h5ad
+-rw-r--r--   0 runner    (1001) docker     (123)   430945 2023-06-14 20:20:33.000000 glue-genes-1.1.0/glue_genes/glue_single_cell/qt/tests/data/test_data_compressed.h5ad
+-rw-r--r--   0 runner    (1001) docker     (123)  1001104 2023-06-14 20:20:33.000000 glue-genes-1.1.0/glue_genes/glue_single_cell/qt/tests/data/test_data_dense.h5ad
+-rw-r--r--   0 runner    (1001) docker     (123)   298998 2023-06-14 20:20:33.000000 glue-genes-1.1.0/glue_genes/glue_single_cell/qt/tests/data/test_data_dense_compressed.h5ad
+-rw-r--r--   0 runner    (1001) docker     (123)  5312200 2023-06-14 20:20:33.000000 glue-genes-1.1.0/glue_genes/glue_single_cell/qt/tests/data/test_other_data.h5ad
+-rw-r--r--   0 runner    (1001) docker     (123)     5850 2023-06-14 20:20:33.000000 glue-genes-1.1.0/glue_genes/glue_single_cell/qt/tests/test_data_load.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-06-14 20:20:33.000000 glue-genes-1.1.0/glue_genes/glue_single_cell/qt/tests/test_diff_gene_exp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-06-14 20:20:33.000000 glue-genes-1.1.0/glue_genes/glue_single_cell/qt/tests/test_enrichr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10712 2023-06-14 20:20:33.000000 glue-genes-1.1.0/glue_genes/glue_single_cell/qt/tests/test_summarize_gene_subset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 20:21:23.465149 glue-genes-1.1.0/glue_genes/glue_single_cell/qtl_viewer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 20:20:33.000000 glue-genes-1.1.0/glue_genes/glue_single_cell/qtl_viewer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12306 2023-06-14 20:20:33.000000 glue-genes-1.1.0/glue_genes/glue_single_cell/qtl_viewer/layer_artist.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 20:21:23.465149 glue-genes-1.1.0/glue_genes/glue_single_cell/qtl_viewer/qt/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 20:20:33.000000 glue-genes-1.1.0/glue_genes/glue_single_cell/qtl_viewer/qt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6437 2023-06-14 20:20:33.000000 glue-genes-1.1.0/glue_genes/glue_single_cell/qtl_viewer/qt/layer_style_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17814 2023-06-14 20:20:33.000000 glue-genes-1.1.0/glue_genes/glue_single_cell/qtl_viewer/qt/layer_style_editor.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     4308 2023-06-14 20:20:33.000000 glue-genes-1.1.0/glue_genes/glue_single_cell/qtl_viewer/qt/options_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10224 2023-06-14 20:20:33.000000 glue-genes-1.1.0/glue_genes/glue_single_cell/qtl_viewer/qt/options_widget.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-06-14 20:20:33.000000 glue-genes-1.1.0/glue_genes/glue_single_cell/qtl_viewer/qt/slider_with_label_widget.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     5385 2023-06-14 20:20:33.000000 glue-genes-1.1.0/glue_genes/glue_single_cell/qtl_viewer/state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 20:21:23.469149 glue-genes-1.1.0/glue_genes/glue_single_cell/qtl_viewer/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 20:20:33.000000 glue-genes-1.1.0/glue_genes/glue_single_cell/qtl_viewer/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5423 2023-06-14 20:20:33.000000 glue-genes-1.1.0/glue_genes/glue_single_cell/qtl_viewer/tests/test_qtl_data_viewer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5056 2023-06-14 20:20:33.000000 glue-genes-1.1.0/glue_genes/glue_single_cell/qtl_viewer/viewer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5434 2023-06-14 20:20:33.000000 glue-genes-1.1.0/glue_genes/glue_single_cell/state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 20:21:23.469149 glue-genes-1.1.0/glue_genes/glue_single_cell/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-14 20:20:33.000000 glue-genes-1.1.0/glue_genes/glue_single_cell/tests/context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 20:21:23.473149 glue-genes-1.1.0/glue_genes/glue_single_cell/tests/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 20:20:33.000000 glue-genes-1.1.0/glue_genes/glue_single_cell/tests/test_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1222520 2023-06-14 20:20:33.000000 glue-genes-1.1.0/glue_genes/glue_single_cell/tests/test_data/test_data.h5ad
+-rw-r--r--   0 runner    (1001) docker     (123)   360068 2023-06-14 20:20:33.000000 glue-genes-1.1.0/glue_genes/glue_single_cell/tests/test_data/test_dataset.h5ad
+-rw-r--r--   0 runner    (1001) docker     (123)   364036 2023-06-14 20:20:33.000000 glue-genes-1.1.0/glue_genes/glue_single_cell/tests/test_data/test_dataset_float32.h5ad
+-rw-r--r--   0 runner    (1001) docker     (123)     4960 2023-06-14 20:20:33.000000 glue-genes-1.1.0/glue_genes/glue_single_cell/tests/test_data_math.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2519 2023-06-14 20:20:33.000000 glue-genes-1.1.0/glue_genes/glue_single_cell/tests/test_synccomponent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 20:21:23.437149 glue-genes-1.1.0/glue_genes.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2291 2023-06-14 20:21:23.000000 glue-genes-1.1.0/glue_genes.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6441 2023-06-14 20:21:23.000000 glue-genes-1.1.0/glue_genes.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 20:21:23.000000 glue-genes-1.1.0/glue_genes.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-06-14 20:21:23.000000 glue-genes-1.1.0/glue_genes.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 20:21:23.000000 glue-genes-1.1.0/glue_genes.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-06-14 20:21:23.000000 glue-genes-1.1.0/glue_genes.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-14 20:21:23.000000 glue-genes-1.1.0/glue_genes.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2220 2023-06-14 20:21:23.473149 glue-genes-1.1.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)      398 2023-06-14 20:20:33.000000 glue-genes-1.1.0/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-06-14 20:20:33.000000 glue-genes-1.1.0/tox.ini
```

### Comparing `glue-genes-1.0.1/.github/workflows/python-package-conda.yml` & `glue-genes-1.1.0/.github/workflows/python-package-conda.yml`

 * *Files identical despite different names*

### Comparing `glue-genes-1.0.1/.github/workflows/static.yml` & `glue-genes-1.1.0/.github/workflows/static.yml`

 * *Files identical despite different names*

### Comparing `glue-genes-1.0.1/.gitignore` & `glue-genes-1.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `glue-genes-1.0.1/LICENSE` & `glue-genes-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `glue-genes-1.0.1/PKG-INFO` & `glue-genes-1.1.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: glue-genes
-Version: 1.0.1
+Version: 1.1.0
 Summary: Multidimensional data visualization for genomics
 Home-page: https://gluesolutions.github.io/glue-genes/
 Author: glue solutions inc.
 Author-email: jfoster@gluesolutions.io
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
@@ -15,15 +15,17 @@
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: License :: OSI Approved :: BSD License
 Provides: glue_genes
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: docs
 Provides-Extra: test
-Provides-Extra: qt
+Provides-Extra: qt5
+Provides-Extra: qt6
+Provides-Extra: openslide
 License-File: LICENSE
 
 ![glue_genes_logo_stacked](https://user-images.githubusercontent.com/3639698/137145077-2c2c9011-68bd-4770-9d58-494bf7632a33.png)
 
 
 The glue-genes meta-package
 ===========================
@@ -43,29 +45,22 @@
 
 * Data loaders for genomics data file formats such as .bed, .bigwig, .h5ad, and .loom
 * Viewers including: 2D Heatmap, Small Multiples, QTL Viewer
 * Menubar plug-ins to facilitate analysis of single-cell transcriptomics data
 
 ### Install
 
-Due to some complicated binary dependencies, the recommended procedure for 
-installing this package is to use [conda](https://www.anaconda.com) and install into a new environment as follows:
+See [the glue genes documentation](https://glue-genes.readthedocs.io/en/latest/how-to/installation.html) for installation help.
 
-```
-conda create -n glue-genes python==3.9
-conda activate glue-genes
-
-conda install glue-core
-pip install glue-genes
-```
+We recommend installing into a new virtual environment. 
 
-### Usage
-
-The Scanpy differential gene expression plugin requires some custom actions to run at startup, which can be achieved by starting glue using this command:
+`pip install glue-genes[qt6]`
 
-`glue --startup=setup_anndata`
+### Usage
 
+After installation, glue (with the glue genes plug-ins loaded) can be invoked at the terminal:
+`glue`
 
 
 ### Development
 
 glue genes is under active development. Please file all bug reports as github issues.
```

### Comparing `glue-genes-1.0.1/docs/Makefile` & `glue-genes-1.1.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `glue-genes-1.0.1/docs/make.bat` & `glue-genes-1.1.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `glue-genes-1.0.1/docs/source/api/reference/analysis.rst` & `glue-genes-1.1.0/docs/source/api/reference/analysis.rst`

 * *Files identical despite different names*

### Comparing `glue-genes-1.0.1/docs/source/api/reference/api/glue_genes.glue_single_cell.data.DataAnnData.rst` & `glue-genes-1.1.0/docs/source/api/reference/api/glue_genes.glue_single_cell.data.DataAnnData.rst`

 * *Files identical despite different names*

### Comparing `glue-genes-1.0.1/docs/source/api/reference/api/glue_genes.glue_single_cell.qt.pca_subset.GeneSummaryListener.rst` & `glue-genes-1.1.0/docs/source/api/reference/api/glue_genes.glue_single_cell.qt.pca_subset.GeneSummaryListener.rst`

 * *Files identical despite different names*

### Comparing `glue-genes-1.0.1/docs/source/api/reference/api/glue_genes.glue_single_cell.qtl_viewer.layer_artist.QTLLayerArtist.rst` & `glue-genes-1.1.0/docs/source/api/reference/api/glue_genes.glue_single_cell.qtl_viewer.layer_artist.QTLLayerArtist.rst`

 * *Files identical despite different names*

### Comparing `glue-genes-1.0.1/docs/source/api/reference/api/glue_genes.glue_single_cell.qtl_viewer.state.QTLViewerState.rst` & `glue-genes-1.1.0/docs/source/api/reference/api/glue_genes.glue_single_cell.qtl_viewer.state.QTLViewerState.rst`

 * *Files identical despite different names*

### Comparing `glue-genes-1.0.1/docs/source/api/reference/api/glue_genes.glue_single_cell.qtl_viewer.viewer.QTLViewer.rst` & `glue-genes-1.1.0/docs/source/api/reference/api/glue_genes.glue_single_cell.qtl_viewer.viewer.QTLViewer.rst`

 * *Files identical despite different names*

### Comparing `glue-genes-1.0.1/docs/source/conf.py` & `glue-genes-1.1.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `glue-genes-1.0.1/docs/source/getting-started/index.rst` & `glue-genes-1.1.0/docs/source/getting-started/index.rst`

 * *Files 14% similar despite different names*

```diff
@@ -2,26 +2,19 @@
 
 Getting Started with glue genes
 ################################
 
 Installation
 ================
 
-You can install glue genes as a Python package.
-
-We recommend installing into a dedicated virtual environment using conda::
-
-    conda create -n glue-genes-env
-    conda activate glue-genes-env
-
-    conda install -c conda-forge glue-core
-    pip install glue-genes
-
-This process uses conda to get some of the difficult-to-install dependencies
-for glue set up first.
+If you already have an existing Python setup on your machine and are comfortable with
+installing Python packages, we recommend that you install glue genes as a Python
+package following the instructions for :ref:`python-installation`. If you are not
+experienced with Python, you can follow the instructions to install the
+:ref:`standalone-applications`.
 
 Brief Introduction to glue
 ============================
 
 glue genes is a custom version of the glue Python library to explore relationships within and among related datasets.
 The main features of glue include:
```

### Comparing `glue-genes-1.0.1/docs/source/how-to/cells-to-genes.rst` & `glue-genes-1.1.0/docs/source/how-to/cells-to-genes.rst`

 * *Files identical despite different names*

### Comparing `glue-genes-1.0.1/docs/source/how-to/data-in.rst` & `glue-genes-1.1.0/docs/source/how-to/data-in.rst`

 * *Files identical despite different names*

### Comparing `glue-genes-1.0.1/docs/source/how-to/images/connect_choose_plugin.png` & `glue-genes-1.1.0/docs/source/how-to/images/connect_choose_plugin.png`

 * *Files identical despite different names*

### Comparing `glue-genes-1.0.1/docs/source/how-to/images/connect_create_gene_subset.png` & `glue-genes-1.1.0/docs/source/how-to/images/connect_create_gene_subset.png`

 * *Files identical despite different names*

### Comparing `glue-genes-1.0.1/docs/source/how-to/images/connect_dge_dialog.png` & `glue-genes-1.1.0/docs/source/how-to/images/connect_dge_dialog.png`

 * *Files identical despite different names*

### Comparing `glue-genes-1.0.1/docs/source/how-to/images/connect_dge_menubar.png` & `glue-genes-1.1.0/docs/source/how-to/images/connect_dge_menubar.png`

 * *Files identical despite different names*

### Comparing `glue-genes-1.0.1/docs/source/how-to/images/connect_summary_dialog.png` & `glue-genes-1.1.0/docs/source/how-to/images/connect_summary_dialog.png`

 * *Files identical despite different names*

### Comparing `glue-genes-1.0.1/docs/source/how-to/images/create_from_data_manager.png` & `glue-genes-1.1.0/docs/source/how-to/images/create_from_data_manager.png`

 * *Files identical despite different names*

### Comparing `glue-genes-1.0.1/docs/source/how-to/images/create_new_viewer.png` & `glue-genes-1.1.0/docs/source/how-to/images/create_new_viewer.png`

 * *Files identical despite different names*

### Comparing `glue-genes-1.0.1/docs/source/how-to/images/drag_to_create.gif` & `glue-genes-1.1.0/docs/source/how-to/images/drag_to_create.gif`

 * *Files identical despite different names*

### Comparing `glue-genes-1.0.1/docs/source/how-to/images/link_data_join_on_key.png` & `glue-genes-1.1.0/docs/source/how-to/images/link_data_join_on_key.png`

 * *Files identical despite different names*

### Comparing `glue-genes-1.0.1/docs/source/how-to/images/link_data_join_on_key_done.png` & `glue-genes-1.1.0/docs/source/how-to/images/link_data_join_on_key_done.png`

 * *Files identical despite different names*

### Comparing `glue-genes-1.0.1/docs/source/how-to/images/link_data_menu.png` & `glue-genes-1.1.0/docs/source/how-to/images/link_data_menu.png`

 * *Files identical despite different names*

### Comparing `glue-genes-1.0.1/docs/source/how-to/images/link_data_toolbar.png` & `glue-genes-1.1.0/docs/source/how-to/images/link_data_toolbar.png`

 * *Files identical despite different names*

### Comparing `glue-genes-1.0.1/docs/source/how-to/images/linking_attributes_step1.png` & `glue-genes-1.1.0/docs/source/how-to/images/linking_attributes_step1.png`

 * *Files identical despite different names*

### Comparing `glue-genes-1.0.1/docs/source/how-to/images/linking_attributes_step2.png` & `glue-genes-1.1.0/docs/source/how-to/images/linking_attributes_step2.png`

 * *Files identical despite different names*

### Comparing `glue-genes-1.0.1/docs/source/how-to/images/loading_options.png` & `glue-genes-1.1.0/docs/source/how-to/images/loading_options.png`

 * *Files identical despite different names*

### Comparing `glue-genes-1.0.1/docs/source/how-to/images/open_data_set_icon.png` & `glue-genes-1.1.0/docs/source/how-to/images/open_data_set_icon.png`

 * *Files identical despite different names*

### Comparing `glue-genes-1.0.1/docs/source/how-to/images/open_data_set_menu.png` & `glue-genes-1.1.0/docs/source/how-to/images/open_data_set_menu.png`

 * *Files identical despite different names*

### Comparing `glue-genes-1.0.1/docs/source/how-to/images/single_cell_loading_options.png` & `glue-genes-1.1.0/docs/source/how-to/images/single_cell_loading_options.png`

 * *Files identical despite different names*

### Comparing `glue-genes-1.0.1/docs/source/how-to/index.rst` & `glue-genes-1.1.0/docs/source/how-to/index.rst`

 * *Files identical despite different names*

### Comparing `glue-genes-1.0.1/docs/source/how-to/linking-data.rst` & `glue-genes-1.1.0/docs/source/how-to/linking-data.rst`

 * *Files identical despite different names*

### Comparing `glue-genes-1.0.1/docs/source/how-to/starting.rst` & `glue-genes-1.1.0/docs/source/how-to/starting.rst`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 .. _Starting:
 
 How do I start glue genes?
 ####################################
 
-Once you have :ref:`installed<Installation>` glue genes, you need to start it from a terminal by typing::
+If you have install glue as a Python package you need to start it from a terminal by typing::
 
     glue --startup=setup_anndata
 
 .. note::
 
    The very first time glue genes launches after installation (or an update) it can take quite a long time (a minute or more). Subsequent launches are fast.
 
@@ -15,11 +15,15 @@
 
 If something does not seem to be working correctly with glue genes (typically some of data loaders or viewers you expect are not present) try launching glue genes with the ``-v`` flag::
 
     glue -v --startup=setup_anndata
 
 and checking the terminal output for error messages. 
 
+If, instead, you have installed the :ref:`standalone-applications` then you can simply double-click
+the application icon to launch glue. Note that you may have to deal with the security prompts if you
+did not deal with them during installation. See `Mac security instructions <http://docs.glueviz.org/en/stable/installation/standalone.html#macos-x>`_ and `Windows security instructions <http://docs.glueviz.org/en/stable/installation/standalone.html#windows>`_.
+
 
 What Next?
 **********
 After launching glue genes you probably want to :ref:`load some data for analysis<Get Data In>`.
```

### Comparing `glue-genes-1.0.1/docs/source/how-to/visualize-data.rst` & `glue-genes-1.1.0/docs/source/how-to/visualize-data.rst`

 * *Files identical despite different names*

### Comparing `glue-genes-1.0.1/docs/source/images/favicon.png` & `glue-genes-1.1.0/docs/source/images/favicon.png`

 * *Files identical despite different names*

### Comparing `glue-genes-1.0.1/docs/source/images/glue_genes_icon.png` & `glue-genes-1.1.0/docs/source/images/glue_genes_icon.png`

 * *Files identical despite different names*

### Comparing `glue-genes-1.0.1/docs/source/images/glue_genes_logo_stacked.png` & `glue-genes-1.1.0/docs/source/images/glue_genes_logo_stacked.png`

 * *Files identical despite different names*

### Comparing `glue-genes-1.0.1/docs/source/index.rst` & `glue-genes-1.1.0/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `glue-genes-1.0.1/docs/source/user-guide/images/enrichr.png` & `glue-genes-1.1.0/docs/source/user-guide/images/enrichr.png`

 * *Files identical despite different names*

### Comparing `glue-genes-1.0.1/docs/source/user-guide/images/qtl_viewer.png` & `glue-genes-1.1.0/docs/source/user-guide/images/qtl_viewer.png`

 * *Files identical despite different names*

### Comparing `glue-genes-1.0.1/docs/source/user-guide/images/single_cell_schematic.png` & `glue-genes-1.1.0/docs/source/user-guide/images/single_cell_schematic.png`

 * *Files identical despite different names*

### Comparing `glue-genes-1.0.1/docs/source/user-guide/images/small_multiples_viewer.png` & `glue-genes-1.1.0/docs/source/user-guide/images/small_multiples_viewer.png`

 * *Files identical despite different names*

### Comparing `glue-genes-1.0.1/docs/source/user-guide/index.rst` & `glue-genes-1.1.0/docs/source/user-guide/index.rst`

 * *Files identical despite different names*

### Comparing `glue-genes-1.0.1/glue_genes/glue_genomics_data/bed_factory.py` & `glue-genes-1.1.0/glue_genes/glue_genomics_data/bed_factory.py`

 * *Files identical despite different names*

### Comparing `glue-genes-1.0.1/glue_genes/glue_genomics_data/bigwig_factory.py` & `glue-genes-1.1.0/glue_genes/glue_genomics_data/bigwig_factory.py`

 * *Files identical despite different names*

### Comparing `glue-genes-1.0.1/glue_genes/glue_single_cell/__init__.py` & `glue-genes-1.1.0/glue_genes/glue_single_cell/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,24 +1,18 @@
 def setup():
     from glue.config import qt_client
 
     from .anndata_factory import read_anndata  # noqa
-    from .anndata_factory import setup_anndata  # noqa
     from .menubar_plugin import diff_gene_exp_plugin  # noqa
     from .menubar_plugin import enrichrpy_plugin  # noqa
-    from .menubar_plugin import pca_subset_exp_plugin  # noqa
+    from .menubar_plugin import summarize_gene_subset_exp_plugin  # noqa
     from .qtl_viewer.viewer import QTLViewer  # noqa
 
     qt_client.add(QTLViewer)
 
-    # Add colormaps we can use when we use the pca_subset_exp_plugin
-    # to maps gene expression to a summary over cells. A summary generated
-    # from a red subset can then be displayed using the 'Reds' colormap
-    # This does not happen automatically... at least not yet
-
     d3_dozen = [
         "#1E77B3",
         "#FF7E0F",
         "#2BA02A",
         "#D62628",
         "#9367BC",
         "#8C564B",
@@ -53,19 +47,14 @@
         "#6027FE",
     ]
 
     import matplotlib.cm as cm
     from glue.config import colormaps
     from matplotlib.colors import ListedColormap
 
-    colormaps.add("Reds", cm.Reds)
-    colormaps.add("Greens", cm.Greens)
-    colormaps.add("Blues", cm.Blues)
-    colormaps.add("Purples", cm.Purples)
-    colormaps.add("Oranges", cm.Oranges)
     # Add some categorical colormaps
 
     colormaps.add("d3_dozen", ListedColormap(d3_dozen, name="d3_dozen"))
     colormaps.add("d3_twenty", ListedColormap(d3_twenty, name="d3_twenty"))
 
     colormaps.add("Pastel1", cm.Pastel1)
     colormaps.add("Paired", cm.Paired)
```

### Comparing `glue-genes-1.0.1/glue_genes/glue_single_cell/anndata_factory.py` & `glue-genes-1.1.0/glue_genes/glue_single_cell/anndata_factory.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,109 +1,43 @@
 from pathlib import Path
 
+import numpy as np
+import pandas as pd
 import scanpy as sc
-from glue.config import data_factory, startup_action
-from glue.core import Data, HubListener
-from glue.core.message import DataCollectionAddMessage
+from glue.config import data_factory, autolinker
+from glue.core import Data
+from glue.core.link_helpers import JoinLink
+from glue.core.component import ExtendedComponent
+from glue.core.component_id import PixelComponentID
+from glue.core.data import RegionData
 from glue.utils.qt import set_cursor_cm
 from qtpy.QtCore import Qt
+from shapely.geometry import Point
 
 from .data import DataAnnData
 from .qt.load_data import LoadDataDialog
 
 __all__ = [
     "read_anndata",
-    "setup_gui_joins",
     "join_anndata_on_keys",
-    "AnnDataListener",
-    "setup_anndata",
 ]
 
 
-class AnnDataListener(HubListener):
-    """
-    Set up :class:`~glue.core.link_helpers.JoinLink` for :class:`~.DataAnnData` objects.
-
-    Listen for :class:`~.DataAnnData` objects to be added to the
-    data collection object, and, if one is, setup the
-    correct join_on_key joins in a way that they will
-    show up in the GUI.
-
-    """
-
-    def __init__(self, hub):
-        hub.subscribe(self, DataCollectionAddMessage, handler=self.setup_anndata)
-
-    def setup_anndata(self, message):
-        data = message.data
-        dc = message.sender
-        if isinstance(data, DataAnnData):
-            setup_gui_joins(dc, data)
-
-
-@startup_action("setup_anndata")
-def setup_anndata(session, data_collection):
-    """
-    A startup action to set up the :class:`~.AnnDataListener`
-    """
-
-    data_collection.anndatalistener = AnnDataListener(data_collection.hub)
-    return
-
-
 def df_to_data(obj, label=None, skip_components=[]):
     result = Data(label=label)
     for c in obj.columns:
         if c not in skip_components:
             result.add_component(obj[c], str(c))
     return result
 
 
 def is_anndata(filename, **kwargs):
     return filename.endswith(".h5ad") or filename.endswith(".loom")
 
 
-def setup_gui_joins(dc, data):
-    """
-    Set up :class:`~glue.core.link_helpers.JoinLink` that mirror the existing join_on_key links,
-    so these links show in the Link Editor.
-
-    Parameters
-    ----------
-    dc : :class:`~glue.core.data_collection.DataCollection`
-        The DataCollection object associated with this glue session
-    data : :class:`~glue_genes.glue_single_cell.data.DataAnnData`
-        The DataAnnData object that defines join_on_key links
-        to the associated obs and var Data objects
-
-    Notes
-    -----
-    We cannot do this at data load because these links are defined
-    at the level of a data_collection, which may not exist at
-    data load time. Instead we call this through a listener
-    when a :class:`~glue_genes.glue_single_cell.data.DataAnnData` object is added to a data collection.
-
-    """
-    try:  # If we are using a version of glue that supports links in the GUI
-        from glue.core.link_helpers import JoinLink
-
-        do_gui_link = True
-    except ImportError:
-        print("Cannot set up GUI join_on_key links")
-        do_gui_link = False
-    if do_gui_link:
-        for other, joins in data._key_joins.items():
-            cid, cid_other = joins
-            gui_link = JoinLink(
-                cids1=[cid[0]], cids2=[cid_other[0]], data1=data, data2=other
-            )
-            if gui_link not in dc._link_manager._external_links:
-                dc.add_link(gui_link)
-
-
 def join_anndata_on_keys(datasets):
     """
     Use join_on_key to stitch the various components on an anndata
     dataset back together. We join on the pixel ids and indices
     because it is far faster to do this than to join on the string
     names for genes and cells.
 
@@ -171,15 +105,14 @@
     subsample_factor: int, optional
         If specified, and `subsample`, reduce the size of obs by this factor
     try_backed: bool, optional
         Attempt to use disk-based access to the data. If AnnData fails to load the file this
         way it will be loaded into memory.
 
     """
-    list_of_data_objs = []
     basename = Path(file_name).stem
 
     if not skip_dialog:
         with set_cursor_cm(Qt.ArrowCursor):
             load_dialog = LoadDataDialog(filename=file_name)
             if load_dialog.exec_():
                 skip_components = load_dialog.skip_components
@@ -196,40 +129,93 @@
         except OSError:
             adata = sc.read(file_name, sparse=True, backed=False)
             backed = False
     else:
         adata = sc.read(file_name, sparse=True, backed=False)
         backed = False
 
+    if "spatial" in adata.uns_keys():
+        make_spatial_components = True
+    else:
+        make_spatial_components = False
+
+    return translate_adata_to_DataAnnData(
+        adata,
+        subsample=subsample,
+        backed=backed,
+        basename=basename,
+        file_name=file_name,
+        skip_components=skip_components,
+        subsample_factor=subsample_factor,
+        try_backed=try_backed,
+        make_spatial_components=make_spatial_components,
+    )
+
+
+def translate_adata_to_DataAnnData(
+    adata,
+    subsample=False,
+    backed=False,
+    basename="",
+    file_name="",
+    skip_components=[],
+    subsample_factor=1,
+    try_backed=False,
+    skip_joins=False,
+    make_spatial_components=False,
+):
+    list_of_data_objs = []
+
+    adata.var_names_make_unique()
+
     if subsample:
         adata = sc.pp.subsample(
             adata, fraction=subsample_factor, copy=True, random_state=0
         )
 
     if backed:
         XData = DataAnnData(
             Xarray=adata.X, full_anndata_obj=adata, backed=backed, label=f"{basename}_X"
         )
     else:
         XData = DataAnnData(Xarray=adata.X, backed=backed, label=f"{basename}_X")
 
     XData.meta["orig_filename"] = basename
+
+    if make_spatial_components:
+        library_id = list(adata.uns["spatial"].keys())[0]
+        basename = (
+            library_id  # This is often a nicer name, but maybe this should be optional?
+        )
+        # Want radius
+        # We should not assume this much about the structure of spatial
+        # but this is okay for now...
+        scale_fac = adata.uns["spatial"][library_id]["scalefactors"]
+        # hi_res_scale_fac = scale_fac["tissue_hires_scalef"]
+        # Want radius
+        spot_size = scale_fac["spot_diameter_fullres"] / 2.0  # * hi_res_scale_fac / 2.0
+
     XData.meta["full_filename"] = file_name
     XData.meta["Xdata"] = XData.uuid
     XData.meta["anndatatype"] = "X Array"
     XData.meta["join_on_obs"] = True
     XData.meta["join_on_var"] = True
 
     # This meta-data is attached to the DataAnnData object so that
     # We can pass it to LoadLog on save/restore
     XData.meta["loadlog_skip_components"] = skip_components
     XData.meta["loadlog_subsample"] = subsample
     XData.meta["loadlog_subsample_factor"] = subsample_factor
     XData.meta["loadlog_try_backed"] = try_backed
 
+    # uns is unstructured data on the AnnData object
+    # We just store it in metadata so we can recreate
+    # the AnnData object
+    XData.meta["uns"] = adata.uns
+
     list_of_data_objs.append(XData)
 
     # The var array is all components of the same length
     # and is stored by AnnData as a Pandas DataFrame
     try:
         var = adata.var
         var_data = df_to_data(
@@ -244,15 +230,21 @@
         list_of_data_objs.append(var_data)
     except:  # noqa E722
         pass
 
     for key in adata.varm_keys():
         if key not in skip_components:
             data_arr = adata.varm[key]
-            data_to_add = {f"{key}_{i}": k for i, k in enumerate(data_arr.T)}
+            # Sometimes this is a dataframe with names, and sometimes a simple np.array
+            if isinstance(data_arr, pd.DataFrame):
+                data_to_add = {
+                    f"{key}_{col}": data_arr[col].values for col in data_arr.columns
+                }
+            else:
+                data_to_add = {f"{key}_{i}": k for i, k in enumerate(data_arr.T)}
             for comp_name, comp in data_to_add.items():
                 var_data.add_component(comp, comp_name)
 
     # The obs array is all components of the same length
     # and is stored by AnnData as a Pandas DataFrame
     try:
         obs = adata.obs
@@ -268,15 +260,90 @@
         list_of_data_objs.append(obs_data)
     except:  # noqa E722
         pass
 
     for key in adata.obsm_keys():
         if key not in skip_components:
             data_arr = adata.obsm[key]
-            data_to_add = {f"{key}_{i}": k for i, k in enumerate(data_arr.T)}
+            # Sometimes this is a dataframe with names, and sometimes a simple np.array
+            if isinstance(data_arr, pd.DataFrame):
+                data_to_add = {
+                    f"{key}_{col}": data_arr[col].values for col in data_arr.columns
+                }
+            else:
+                data_to_add = {f"{key}_{i}": k for i, k in enumerate(data_arr.T)}
             for comp_name, comp in data_to_add.items():
                 obs_data.add_component(comp, comp_name)
 
+    if make_spatial_components:
+        obs_data = list_of_data_objs.pop()
+
+        library_id = list(adata.uns["spatial"].keys())[0]
+        image_data = adata.uns["spatial"][library_id]["images"]["hires"]
+        scale_fac = adata.uns["spatial"][library_id]["scalefactors"]
+        hi_res_scale_fac = scale_fac["tissue_hires_scalef"]
+
+        new_spatial_0 = obs_data["spatial_0"]
+        new_spatial_1 = (
+            int(image_data.shape[0] / hi_res_scale_fac) - obs_data["spatial_1"]
+        )  # flip coordinates
+        spatial_0_id = obs_data.id["spatial_0"]
+        spatial_1_id = obs_data.id["spatial_1"]
+        obs_data.update_components({spatial_1_id: new_spatial_1})
+        obs_data.update_components({spatial_0_id: new_spatial_0})
+
+        # We need to cast the obs Data object into a RegionData object
+        spots = []
+        for x, y in zip(obs_data["spatial_0"], obs_data["spatial_1"]):
+            spots.append(Point(x, y).buffer(spot_size))
+        spot_arr = np.array(spots)
+
+        obs_data_new = RegionData(label=obs_data.label)
+        for compid in obs_data.components:
+            if not isinstance(compid, PixelComponentID):
+                # Use same names (with .label) but NOT same ComponentIDs!
+                obs_data_new.add_component(obs_data.get_component(compid), compid.label)
+
+        spot_comp = ExtendedComponent(
+            spot_arr,
+            parent_component_ids=[
+                obs_data_new.id["spatial_0"],
+                obs_data_new.id["spatial_1"],
+            ],
+        )
+
+        obs_data_new.add_component(spot_comp, label="spots")
+        obs_data_new.meta = obs_data.meta
+        XData.meta["obs_data"] = obs_data_new
+        list_of_data_objs.append(obs_data_new)
+
     # obs_data.meta['xarray_data'] = Xdata
     # var_data.meta['xarray_data'] = Xdata
 
     return join_anndata_on_keys(list_of_data_objs)
+
+
+@autolinker("AnnData")
+def anndata_autolink(data_collection):
+    """
+    This sets up automatic links between the components of an Anndata
+    dataset, specifically join_on_key links between the X and obs/var
+    datasets. This is pretty straightforward because our data loader
+    already sets up the _key_joins in the dataset and this is "just"
+    adding them as full GUI links.
+    """
+    anndata_datasets = [
+        data for data in data_collection if isinstance(data, DataAnnData)
+    ]
+    if len(anndata_datasets) < 1:
+        return []
+
+    gui_links = []
+    for data in anndata_datasets:
+        for other, joins in data._key_joins.items():
+            cid, cid_other = joins
+            gui_link = JoinLink(
+                cids1=[cid[0]], cids2=[cid_other[0]], data1=data, data2=other
+            )
+            if gui_link not in data_collection._link_manager._external_links:
+                gui_links.append(gui_link)
+    return gui_links
```

### Comparing `glue-genes-1.0.1/glue_genes/glue_single_cell/data.py` & `glue-genes-1.1.0/glue_genes/glue_single_cell/data.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,35 +43,30 @@
 from glue.config import data_translator, session_patch
 from glue.core import DataCollection
 from glue.core.component import Component, CoordinateComponent
 from glue.core.component_id import ComponentID, PixelComponentID
 from glue.core.component_link import ComponentLink
 from glue.core.data import Data, Subset
 from glue.core.exceptions import IncompatibleAttribute
-from glue.core.state import (
-    GlueSerializeError,
-    _load_data_collection_4,
-    _save_data_collection_4,
-    loader,
-    saver,
-)
+from glue.core.state import (GlueSerializeError, _load_data_collection_4,
+                             _save_data_collection_4, loader, saver)
 from scipy.sparse import isspmatrix
 
 __all__ = ["DataAnnData", "DataAnnDataTranslator"]
 
 
 class DataAnnData(Data):
     """
     A :class:`~glue.core.data.Data` class to handle on-disk and sparse access to a large AnnData X matrix.
 
     Attributes
     ----------
     Xdata
     listeners : list
-                Any :class:`~glue_genes.glue_single_cell.anndata_factory.AnnDataListener` associated with this object.
+                Any :class:`GeneSummaryListener` associated with this object.
     backed : bool
              True if the matrix is not loaded into memory but is accessed from the disk.
     sparse : bool
              True if the underlying matrix is sparse
     """
 
     def __init__(
@@ -92,20 +87,14 @@
             comp_to_add = Component(Xdata)
             self.add_component(comp_to_add, label=component_id)
             if isspmatrix(Xdata):
                 self.sparse = True
             elif type(Xdata) == anndata._core.sparse_dataset.SparseDataset:
                 self.sparse = True
 
-        # When we create this data object, we don't have a hub set up yet,
-        # so we can't init the SubsetListener at Data creation time. Instead,
-        # we add a Listener to the DataCollection object in a custom
-        # startup_action, and this adds a subset_listener to DataAnnData
-        # objects that are added to the data collection.
-
     @property
     def Xdata(self):
         """
         The full AnnData object, accessible for analysis functions that need one.
         """
         if self._Xdata:
             return self._Xdata
@@ -590,12 +579,12 @@
             var_data = self.unwrap_components(var_glue_data)
             if data_or_subset.backed:
                 adata = scanpy.read(
                     data_or_subset.meta["full_filename"], sparse=True, backed="r"
                 )
             else:
                 adata = anndata.AnnData(
-                    data_or_subset["Xarray"], obs=obs_data, var=var_data
+                    data_or_subset["Xarray"], obs=obs_data, var=var_data, uns=data_or_subset.meta.get('uns'),
                 )
             return adata
         else:
             pass
```

### Comparing `glue-genes-1.0.1/glue_genes/glue_single_cell/menubar_plugin.py` & `glue-genes-1.1.0/glue_genes/glue_single_cell/menubar_plugin.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from glue.config import menubar_plugin
 
 from .qt.diff_gene_exp import DiffGeneExpDialog
 from .qt.enrichr import EnrichpyDialog
-from .qt.pca_subset import PCASubsetDialog
+from .qt.summarize_gene_subset import SummarizeGeneSubsetDialog
 
 
-@menubar_plugin("Scanpy Differential Gene Expression")
+@menubar_plugin("Calculate Differential Gene Expression")
 def diff_gene_exp_plugin(session, data_collection):
     DiffGeneExpDialog.create_subset(data_collection, default=None, parent=None)
     return
 
 
 @menubar_plugin("Calculate Summary Over Gene Subset")
-def pca_subset_exp_plugin(session, data_collection):
-    PCASubsetDialog.summarize(data_collection, default=None, parent=None)
+def summarize_gene_subset_exp_plugin(session, data_collection):
+    SummarizeGeneSubsetDialog.summarize(data_collection, default=None, parent=None)
     return
 
 
 @menubar_plugin("Enrich Gene Set via Enrichr")
 def enrichrpy_plugin(session, data_collection):
     EnrichpyDialog.enrich(data_collection, default=None, parent=None)
     return
```

### Comparing `glue-genes-1.0.1/glue_genes/glue_single_cell/qt/diff_gene_exp.py` & `glue-genes-1.1.0/glue_genes/glue_single_cell/qt/diff_gene_exp.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from glue.core.data import Data
 from glue.core.link_helpers import JoinLink
 from glue.core.subset import CategorySubsetState
 from glue.utils.qt import load_ui
 from qtpy import QtWidgets
 
 from ..state import DiffGeneExpState
-from .pca_subset import dialog
+from .summarize_gene_subset import dialog
 
 __all__ = ["get_gene_list_diff_exp", "DiffGeneExpDialog"]
 
 
 def get_gene_list_diff_exp(subset1, subset2, data, n_genes=50):
     """
     Get differential gene expression for two subsets over a dataset
@@ -85,15 +85,14 @@
     gene_list = gene_list[0:n_genes]
 
     return gene_list, dge_data
 
 
 class DiffGeneExpDialog(QtWidgets.QDialog):
     def __init__(self, collect, default=None, parent=None):
-
         super(DiffGeneExpDialog, self).__init__(parent=parent)
 
         self.state = DiffGeneExpState(collect)
 
         self.ui = load_ui("diff_gene_exp.ui", self, directory=os.path.dirname(__file__))
         self._connections = autoconnect_callbacks_to_qt(self.state, self.ui)
```

### Comparing `glue-genes-1.0.1/glue_genes/glue_single_cell/qt/diff_gene_exp.ui` & `glue-genes-1.1.0/glue_genes/glue_single_cell/qt/diff_gene_exp.ui`

 * *Files 2% similar despite different names*

#### Comparing `glue-genes-1.0.1/glue_genes/glue_single_cell/qt/diff_gene_exp.ui` & `glue-genes-1.1.0/glue_genes/glue_single_cell/qt/diff_gene_exp.ui`

```diff
@@ -32,24 +32,24 @@
             <set>Qt::TextBrowserInteraction</set>
           </property>
         </widget>
       </item>
       <item row="2" column="0">
         <widget class="QComboBox" name="combosel_data">
           <property name="sizeAdjustPolicy">
-            <enum>QComboBox::AdjustToMinimumContentsLength</enum>
+            <enum>QComboBox::AdjustToMinimumContentsLengthWithIcon</enum>
           </property>
         </widget>
       </item>
       <item row="3" column="0">
         <layout class="QHBoxLayout" name="horizontalLayout_11">
           <item>
             <widget class="QComboBox" name="combosel_gene_att">
               <property name="sizeAdjustPolicy">
-                <enum>QComboBox::AdjustToMinimumContentsLength</enum>
+                <enum>QComboBox::AdjustToMinimumContentsLengthWithIcon</enum>
               </property>
             </widget>
           </item>
           <item>
             <widget class="QLabel" name="label_11">
               <property name="text">
                 <string>Gene Name/ID Attribute</string>
@@ -66,15 +66,15 @@
                 <string>Subset 1</string>
               </property>
             </widget>
           </item>
           <item>
             <widget class="QComboBox" name="combosel_subset1">
               <property name="sizeAdjustPolicy">
-                <enum>QComboBox::AdjustToMinimumContentsLength</enum>
+                <enum>QComboBox::AdjustToMinimumContentsLengthWithIcon</enum>
               </property>
             </widget>
           </item>
         </layout>
       </item>
       <item row="5" column="0">
         <layout class="QHBoxLayout" name="horizontalLayout_9">
@@ -84,15 +84,15 @@
                 <string>Subset 2</string>
               </property>
             </widget>
           </item>
           <item>
             <widget class="QComboBox" name="combosel_subset2">
               <property name="sizeAdjustPolicy">
-                <enum>QComboBox::AdjustToMinimumContentsLength</enum>
+                <enum>QComboBox::AdjustToMinimumContentsLengthWithIcon</enum>
               </property>
             </widget>
           </item>
         </layout>
       </item>
       <item row="6" column="0">
         <layout class="QHBoxLayout" name="horizontalLayout">
```

### Comparing `glue-genes-1.0.1/glue_genes/glue_single_cell/qt/enrichr.py` & `glue-genes-1.1.0/glue_genes/glue_single_cell/qt/enrichr.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import enrichrpy.enrichr
 from echo.qt import autoconnect_callbacks_to_qt
 from glue.utils.qt import load_ui
 from qtpy import QtWidgets
 
 from ..anndata_factory import df_to_data
 from ..state import EnrichpyState
-from .pca_subset import dialog
+from .summarize_gene_subset import dialog
 
 __all__ = ["EnrichpyDialog"]
 
 
 def convert_genes_to_list(row):
     arr = row.split(";")
     lg = [x for x in arr]
@@ -32,15 +32,14 @@
     gene list and only restore if we need to.
     """
     return [x.capitalize() for x in row]
 
 
 class EnrichpyDialog(QtWidgets.QDialog):
     def __init__(self, collect, default=None, parent=None):
-
         super(EnrichpyDialog, self).__init__(parent=parent)
 
         self.state = EnrichpyState(collect)
 
         self.ui = load_ui("enrichr.ui", self, directory=os.path.dirname(__file__))
         self._connections = autoconnect_callbacks_to_qt(self.state, self.ui)
```

### Comparing `glue-genes-1.0.1/glue_genes/glue_single_cell/qt/enrichr.ui` & `glue-genes-1.1.0/glue_genes/glue_single_cell/qt/enrichr.ui`

 * *Files 2% similar despite different names*

#### Comparing `glue-genes-1.0.1/glue_genes/glue_single_cell/qt/enrichr.ui` & `glue-genes-1.1.0/glue_genes/glue_single_cell/qt/enrichr.ui`

```diff
@@ -22,15 +22,15 @@
                 <string>Enrichr library</string>
               </property>
             </widget>
           </item>
           <item>
             <widget class="QComboBox" name="combosel_gene_set">
               <property name="sizeAdjustPolicy">
-                <enum>QComboBox::AdjustToMinimumContentsLength</enum>
+                <enum>QComboBox::AdjustToMinimumContentsLengthWithIcon</enum>
               </property>
             </widget>
           </item>
         </layout>
       </item>
       <item row="6" column="0">
         <layout class="QHBoxLayout" name="horizontalLayout_6">
@@ -75,15 +75,15 @@
             <set>Qt::AlignCenter</set>
           </property>
         </widget>
       </item>
       <item row="2" column="0">
         <widget class="QComboBox" name="combosel_data">
           <property name="sizeAdjustPolicy">
-            <enum>QComboBox::AdjustToMinimumContentsLength</enum>
+            <enum>QComboBox::AdjustToMinimumContentsLengthWithIcon</enum>
           </property>
         </widget>
       </item>
       <item row="4" column="0">
         <layout class="QHBoxLayout" name="horizontalLayout_7">
           <item>
             <widget class="QLabel" name="label_8">
@@ -91,26 +91,26 @@
                 <string>Subset of Genes</string>
               </property>
             </widget>
           </item>
           <item>
             <widget class="QComboBox" name="combosel_subset">
               <property name="sizeAdjustPolicy">
-                <enum>QComboBox::AdjustToMinimumContentsLength</enum>
+                <enum>QComboBox::AdjustToMinimumContentsLengthWithIcon</enum>
               </property>
             </widget>
           </item>
         </layout>
       </item>
       <item row="3" column="0">
         <layout class="QHBoxLayout" name="horizontalLayout_11">
           <item>
             <widget class="QComboBox" name="combosel_gene_att">
               <property name="sizeAdjustPolicy">
-                <enum>QComboBox::AdjustToMinimumContentsLength</enum>
+                <enum>QComboBox::AdjustToMinimumContentsLengthWithIcon</enum>
               </property>
             </widget>
           </item>
           <item>
             <widget class="QLabel" name="label_11">
               <property name="text">
                 <string>Gene Name/ID Attribute</string>
```

### Comparing `glue-genes-1.0.1/glue_genes/glue_single_cell/qt/load_data.py` & `glue-genes-1.1.0/glue_genes/glue_single_cell/qt/load_data.py`

 * *Files identical despite different names*

### Comparing `glue-genes-1.0.1/glue_genes/glue_single_cell/qt/load_data.ui` & `glue-genes-1.1.0/glue_genes/glue_single_cell/qt/load_data.ui`

 * *Files identical despite different names*

### Comparing `glue-genes-1.0.1/glue_genes/glue_single_cell/qt/pca_subset.py` & `glue-genes-1.1.0/glue_genes/glue_single_cell/qt/summarize_gene_subset.py`

 * *Files 15% similar despite different names*

```diff
@@ -9,24 +9,26 @@
 """
 
 import os
 
 import numpy as np
 import scanpy as sc
 from echo.qt import autoconnect_callbacks_to_qt
-from glue.core import Data, HubListener
+from glue.core import HubListener
 from glue.core.exceptions import IncompatibleAttribute
 from glue.core.message import SubsetDeleteMessage, SubsetUpdateMessage
 from glue.utils.qt import load_ui
 from qtpy import QtWidgets
 from qtpy.QtWidgets import QMessageBox
+from glue_genes.glue_single_cell.component import SyncComponent
+from glue.core.component_id import ComponentID
 
-from ..state import PCASubsetState
+from ..state import SummarizeGeneSubsetState
 
-__all__ = ["PCASubsetDialog", "GeneSummaryListener"]
+__all__ = ["SummarizeGeneSubsetDialog", "GeneSummaryListener"]
 
 
 def dialog(title, text, icon):
     if icon == "warn":
         icon = QMessageBox.Warning
     elif icon == "info":
         icon = QMessageBox.Information
@@ -95,51 +97,53 @@
 
     elif calculation == "Means":
         if raw:
             adata_sel = adata.raw.X[
                 :, mask
             ]  # This will fail if genesubset is not actually over genes
             if data_with_Xarray.sparse is True:
-                data_arr = np.expand_dims(
-                    adata_sel.mean(axis=1).A1, axis=1
-                )  # Expand to make same dimensionality as PCA
+                data_arr = (adata_sel.mean(axis=1).A1,)
             else:
-                data_arr = np.expand_dims(adata_sel.mean(axis=1), axis=1)
+                data_arr = adata_sel.mean(axis=1)
 
         else:
             adata_sel = adata.X[:, mask]
             if data_with_Xarray.sparse is True:
-                data_arr = np.expand_dims(
-                    adata_sel.mean(axis=1).A1, axis=1
-                )  # Expand to make same dimensionality as PCA
+                data_arr = adata_sel.mean(axis=1).A1
             else:
-                data_arr = np.expand_dims(adata_sel.mean(axis=1), axis=1)
+                data_arr = adata_sel.mean(axis=1)
 
     return data_arr
 
 
-def apply_data_arr(target_dataset, data_arr, basename, key="PCA"):
+def apply_data_arr(target_dataset, data_arr, basename, subset, key="Means"):
     """
+    Add appropriately named SyncComponents from data_arr to target_dataset
+
     This is a sort of clunky approach to doing this.
 
     We generate a Data object from the data_arr that was returned,
     and then add the non-coordinate components of this Data object
     to the target dataset.
     """
-
-    data = Data(
-        **{f"{key}_{i}": k for i, k in enumerate(data_arr.T)}, label=f"{basename}_{key}"
-    )
-    for x in data.components:
-        if x not in data.coordinate_components:
-            new_comp_name = f"{basename}_{x}"
-            target_dataset.add_component(data.get_component(f"{x}"), new_comp_name)
-    return (
-        new_comp_name  # This just gets the last one, which is not quite correct for PCA
-    )
+    cids = []
+    if data_arr.ndim == 2:
+        for i, k in enumerate(data_arr.T):
+            component_name = f"{basename}_{key}_{i} (sync)"
+            cid = ComponentID(component_name)
+            comp = SyncComponent(k, subsets=[subset])
+            _ = target_dataset.add_component(comp, cid)
+            cids.append(cid)
+    else:
+        component_name = f"{basename}_{key} (sync)"
+        cid = ComponentID(component_name)
+        comp = SyncComponent(data_arr, subsets=[subset])
+        _ = target_dataset.add_component(comp, cid)
+        cids.append(cid)
+    return cids
 
 
 class GeneSummaryListener(HubListener):
     """
     A Listener to keep the new components in target_dataset
     up-to-date with any changes in the genesubset.
 
@@ -149,21 +153,23 @@
         The subset over genes to watch
     basename : str
         The subset label
     key : str
         The kind of summary performed: [Means, PCA, Module]
     data_with_Xarray : :class:`~.DataAnnData`
         The expression matrix (X) used to reference the target_dataset
-
+    comps : list
+        A list of the components to keep in sync
     """
 
-    def __init__(self, genesubset, basename, key, data_with_Xarray=None):
+    def __init__(self, genesubset, basename, key, data_with_Xarray=None, comps=[]):
         self.genesubset = genesubset
         self.basename = basename
         self.key = key
+        self.comps = comps
         if data_with_Xarray is not None:
             self.set_circular_refs(data_with_Xarray)
 
     def set_circular_refs(self, data_with_Xarray):
         self.data_with_Xarray = data_with_Xarray
         self.hub = data_with_Xarray.hub
         self.target_dataset = self.data_with_Xarray.meta["obs_data"]
@@ -175,83 +181,80 @@
             self.hub = self.data_with_Xarray.hub
         # hub.subscribe(self, SubsetCreateMessage,
         #              handler=self.update_subset)
         self.hub.subscribe(self, SubsetUpdateMessage, handler=self.update_subset)
         self.hub.subscribe(self, SubsetDeleteMessage, handler=self.delete_subset)
 
     def __gluestate__(self, context):
-
         return dict(
             genesubset=context.id(self.genesubset),
             basename=context.do(self.basename),
             key=context.do(self.key),
             data_with_Xarray=context.id(self.data_with_Xarray),
+            comps=context.id(self.comps),
         )
 
     @classmethod
     def __setgluestate__(cls, rec, context):
         # target_dataset = context.object(rec['data_with_Xarray'])
         result = cls(
             genesubset=context.object(rec["genesubset"]),
             basename=context.object(rec["basename"]),
             key=context.object(rec["key"]),
+            comps=context.object(rec["comps"]),
         )
         yield result
         data_with_Xarray = context.object(rec["data_with_Xarray"])
         result.set_circular_refs(data_with_Xarray)
         # result.register_to_hub()
 
     def update_subset(self, message):
         """
         if the subset is the one we care about
         then we rerun the calculation.
 
         TODO: If the subset is the same subset and has just been
         renamed then we need to update the component name
+
+        TODO: If the subset is no longer over a valid set of attributes
+              we should... what?
         """
         subset = message.subset
         if subset == self.genesubset:
             # if subset.attributes == self.genesubset_attributes:
             new_data = do_calculation_over_gene_subset(
                 self.data_with_Xarray, self.genesubset, calculation=self.key
             )
-
-            if new_data is not None:
-                mapping = {
-                    f"{self.basename}_{self.key}_{i}": k
-                    for i, k in enumerate(new_data.T)
-                }
-                for (
-                    x
-                ) in (
-                    self.target_dataset.components
-                ):  # This is to get the right component ids
-                    xstr = f"{x.label}"
-                    if xstr in mapping.keys():
-                        mapping[x] = mapping.pop(xstr)
-                self.target_dataset.update_components(mapping)
+            mapping = {}
+            if new_data.ndim == 2:
+                for c, k in zip(self.comps, new_data.T):
+                    mapping[c] = k
+            else:
+                mapping[self.comps[0]] = new_data
+            self.target_dataset.update_components(mapping)
 
     def delete_subset(self, message):
         """
-        Remove the attributes from target_dataset
+        TODO: Remove the attributes from target_dataset
         """
         pass
 
     def receive_message(self, message):
         pass
 
 
-class PCASubsetDialog(QtWidgets.QDialog):
+class SummarizeGeneSubsetDialog(QtWidgets.QDialog):
     def __init__(self, collect, default=None, parent=None):
+        super().__init__(parent=parent)
 
-        super(PCASubsetDialog, self).__init__(parent=parent)
-
-        self.state = PCASubsetState(collect)
+        self.state = SummarizeGeneSubsetState(collect)
 
-        self.ui = load_ui("pca_subset.ui", self, directory=os.path.dirname(__file__))
+        self.ui = load_ui(
+            "summarize_gene_subset.ui", self, directory=os.path.dirname(__file__)
+        )
         self._connections = autoconnect_callbacks_to_qt(self.state, self.ui)
 
         self._collect = collect
 
         if default is not None:
             self.state.data = default
 
@@ -288,28 +291,29 @@
         elif self.state.do_pca:
             key = "PCA"
         elif self.state.do_module:
             key = "Module"
         data_arr = do_calculation_over_gene_subset(
             data_with_Xarray, genesubset, calculation=key
         )
-
+        new_comps = []
         if data_arr is not None:
-
-            new_comp_name = apply_data_arr(target_dataset, data_arr, basename, key=key)
+            new_comps = apply_data_arr(
+                target_dataset, data_arr, basename, genesubset, key=key
+            )
             gene_summary_listener = GeneSummaryListener(
-                genesubset, basename, key, data_with_Xarray
+                genesubset, basename, key, data_with_Xarray, new_comps
             )
             gene_summary_listener.register_to_hub()
             data_with_Xarray.listeners.append(gene_summary_listener)
 
         confirm = dialog(  # noqa: F841
             "Adding a new component",
             f"The component:\n"
-            f"{new_comp_name}\n"
+            f"{new_comps}\n"
             f"has been added to:\n"
             f"{target_dataset.label}\n"
             f"and will be automatically updated when {genesubset.label} is changed.",
             "info",
         )
 
     @classmethod
```

### Comparing `glue-genes-1.0.1/glue_genes/glue_single_cell/qt/pca_subset.ui` & `glue-genes-1.1.0/glue_genes/glue_single_cell/qt/summarize_gene_subset.ui`

 * *Files 6% similar despite different names*

#### Comparing `glue-genes-1.0.1/glue_genes/glue_single_cell/qt/pca_subset.ui` & `glue-genes-1.1.0/glue_genes/glue_single_cell/qt/summarize_gene_subset.ui`

```diff
@@ -1,21 +1,21 @@
 <?xml version="1.0" encoding="utf-8"?>
 <ui version="4.0">
   <class>PCASubset</class>
-  <widget class="QDialog" name="PCASubset">
+  <widget class="QDialog" name="SummarizeGeneSubset">
     <property name="geometry">
       <rect>
         <x>0</x>
         <y>0</y>
         <width>462</width>
         <height>356</height>
       </rect>
     </property>
     <property name="windowTitle">
-      <string>Summarize Gene Subset</string>
+      <string>Compute Summary over Gene Subset</string>
     </property>
     <layout class="QGridLayout" name="gridLayout">
       <item row="0" column="0">
         <widget class="QLabel" name="label_5">
           <property name="text">
             <string>This plug-in computes a summary statistic over cells based on a subset of genes and keeps that statistic up-to-date as you change the gene subset. You need to have a subset of genes defined before you run this.</string>
           </property>
@@ -26,15 +26,15 @@
             <bool>true</bool>
           </property>
         </widget>
       </item>
       <item row="2" column="0">
         <widget class="QComboBox" name="combosel_data">
           <property name="sizeAdjustPolicy">
-            <enum>QComboBox::AdjustToMinimumContentsLength</enum>
+            <enum>QComboBox::AdjustToMinimumContentsLengthWithIcon</enum>
           </property>
         </widget>
       </item>
       <item row="3" column="0">
         <layout class="QHBoxLayout" name="horizontalLayout_7">
           <item>
             <widget class="QLabel" name="label_8">
@@ -42,15 +42,15 @@
                 <string>Subset of Genes to summarize</string>
               </property>
             </widget>
           </item>
           <item>
             <widget class="QComboBox" name="combosel_genesubset">
               <property name="sizeAdjustPolicy">
-                <enum>QComboBox::AdjustToMinimumContentsLength</enum>
+                <enum>QComboBox::AdjustToMinimumContentsLengthWithIcon</enum>
               </property>
             </widget>
           </item>
         </layout>
       </item>
       <item row="4" column="0">
         <layout class="QHBoxLayout" name="horizontalLayout_3">
```

### Comparing `glue-genes-1.0.1/glue_genes/glue_single_cell/qt/tests/data/test_data.h5ad` & `glue-genes-1.1.0/glue_genes/glue_single_cell/qt/tests/data/test_data.h5ad`

 * *Files identical despite different names*

### Comparing `glue-genes-1.0.1/glue_genes/glue_single_cell/qt/tests/data/test_data_compressed.h5ad` & `glue-genes-1.1.0/glue_genes/glue_single_cell/qt/tests/data/test_data_compressed.h5ad`

 * *Files identical despite different names*

### Comparing `glue-genes-1.0.1/glue_genes/glue_single_cell/qt/tests/data/test_data_dense.h5ad` & `glue-genes-1.1.0/glue_genes/glue_single_cell/qt/tests/data/test_data_dense.h5ad`

 * *Files identical despite different names*

### Comparing `glue-genes-1.0.1/glue_genes/glue_single_cell/qt/tests/data/test_data_dense_compressed.h5ad` & `glue-genes-1.1.0/glue_genes/glue_single_cell/qt/tests/data/test_data_dense_compressed.h5ad`

 * *Files identical despite different names*

### Comparing `glue-genes-1.0.1/glue_genes/glue_single_cell/qt/tests/data/test_other_data.h5ad` & `glue-genes-1.1.0/glue_genes/glue_single_cell/qt/tests/data/test_other_data.h5ad`

 * *Files identical despite different names*

### Comparing `glue-genes-1.0.1/glue_genes/glue_single_cell/qt/tests/test_data_load.py` & `glue-genes-1.1.0/glue_genes/glue_single_cell/qt/tests/test_data_load.py`

 * *Files identical despite different names*

### Comparing `glue-genes-1.0.1/glue_genes/glue_single_cell/qt/tests/test_diff_gene_exp.py` & `glue-genes-1.1.0/glue_genes/glue_single_cell/qt/tests/test_diff_gene_exp.py`

 * *Files identical despite different names*

### Comparing `glue-genes-1.0.1/glue_genes/glue_single_cell/qt/tests/test_enrichr.py` & `glue-genes-1.1.0/glue_genes/glue_single_cell/qt/tests/test_enrichr.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 from glue.app.qt import GlueApplication
 from glue.core import Data
 from glue.core.state import GlueUnSerializer
-
+import pytest
 from ..enrichr import EnrichpyDialog
 
 
 class TestEnrichr(object):
     def get_data(self):
-
         fake_data = Data(
             gene_id=["Sox17", "Adhfe1", "Prex2", "Msc", "Rdh10", "Gsta3"],
             qtl=[1, 2, 3, 4, 5, 5],
             label="qtl",
         )
         return fake_data
 
@@ -25,29 +24,32 @@
 
         self.gene_data = self.dc[0]
 
         self.subset1 = self.dc.new_subset_group(
             label="Interesting Genes", subset_state=self.gene_data.id["qtl"] < 5
         )
 
+    @pytest.mark.skip(reason="Need to mock the response to limit API calls")
     def do_enrichr(self):
         enrichrdiag = EnrichpyDialog(self.dc)
         enrichrdiag.state.data = self.dc[0]
         enrichrdiag.state.subset = self.subset1
         enrichrdiag.state.gene_att = self.dc[0].id["gene_id"]
         enrichrdiag.state.gene_set = "KEGG_2019_Mouse"
 
         enrichrdiag._apply(do_dialog=False)
 
+    @pytest.mark.skip(reason="Need to mock the response to limit API calls")
     def test_get_enrich(self):
         assert len(self.dc) == 1  # We add a new dataset
         self.do_enrichr()
         assert len(self.dc) == 2  # We add a new dataset
-        assert len(self.dc[1].components) == 10
+        assert len(self.dc[1].components) == 1
 
+    @pytest.mark.skip(reason="Need to mock the response to limit API calls")
     def test_save_and_restore(self, tmpdir):
         self.do_enrichr()
         filename = tmpdir.join("test_anndata_load_session.glu").strpath
         self.session.application.save_session(filename)
         with open(filename, "r") as f:
             session = f.read()
```

### Comparing `glue-genes-1.0.1/glue_genes/glue_single_cell/qt/tests/test_pca_subset.py` & `glue-genes-1.1.0/glue_genes/glue_single_cell/qt/tests/test_summarize_gene_subset.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,16 +23,16 @@
 from glue.core import data_factories as df
 from glue.core.data_collection import DataCollection
 from glue.core.link_helpers import JoinLink
 from glue.core.state import GlueUnSerializer
 
 from glue_genes.glue_single_cell.anndata_factory import read_anndata
 
-from ..pca_subset import (
-    PCASubsetDialog,
+from ..summarize_gene_subset import (
+    SummarizeGeneSubsetDialog,
     apply_data_arr,
     do_calculation_over_gene_subset,
 )
 
 DATA = os.path.join(os.path.dirname(__file__), "data")
 
 
@@ -66,36 +66,36 @@
         d1_var = self.dc[1]
 
         s = self.dc.new_subset_group()
 
         # s = d1_var.new_subset()
         s.subset_state = d1_var.id["gene_stuff_0"] > 0
 
-        sumdiag = PCASubsetDialog(self.dc)
+        sumdiag = SummarizeGeneSubsetDialog(self.dc)
         sumdiag.state.data = self.dc[2]
         sumdiag.state.genesubset = s
         sumdiag.state.do_means = True
         sumdiag.state.do_pca = False
         sumdiag.state.do_module = False
 
         with patch(
-            "glue_genes.glue_single_cell.qt.pca_subset.dialog"
+            "glue_genes.glue_single_cell.qt.summarize_gene_subset.dialog"
         ) as fakedialog:  # noqa: F841
             sumdiag._apply()
 
         assert len(self.dc[0].listeners) == 1
         assert len(self.dc[2].components) == 6
-        assert np.sum(self.dc[2]["Subset 1_Means_0"]) > 99
-        assert np.sum(self.dc[2]["Subset 1_Means_0"]) < 100
+        assert np.sum(self.dc[2]["Subset 1_Means (sync)"]) > 99
+        assert np.sum(self.dc[2]["Subset 1_Means (sync)"]) < 100
 
         sumdiag.state.genesubset.subset_state = d1_var.id["gene_stuff_0"] > 0.6
 
-        assert np.sum(self.dc[2]["Subset 1_Means_0"]) > 99
+        assert np.sum(self.dc[2]["Subset 1_Means (sync)"]) > 99
         assert (
-            not np.sum(self.dc[2]["Subset 1_Means_0"]) < 100
+            not np.sum(self.dc[2]["Subset 1_Means (sync)"]) < 100
         )  # Check that updating subset changes the result
 
         filename = tmpdir.join("test_anndata_load_session.glu").strpath
         self.session.application.save_session(filename)
 
         with open(filename, "r") as f:
             session = f.read()
@@ -109,22 +109,21 @@
         assert len(dc) == 7
 
         assert len(dc[0].listeners) == 1
         assert len(dc[2].components) == 6
 
         dc.subset_groups[0].subset_state = dc[1].id["gene_stuff_0"] > 0
 
-        assert np.sum(dc[2]["Subset 1_Means_0"]) > 99
-        assert np.sum(dc[2]["Subset 1_Means_0"]) < 100
+        assert np.sum(dc[2]["Subset 1_Means (sync)"]) > 99
+        assert np.sum(dc[2]["Subset 1_Means (sync)"]) < 100
         ga.close()
 
 
 class TestCellSummary(object):
     def setup_method(self, method):
-
         d1 = df.load_data(
             os.path.join(DATA, "test_data.h5ad"), factory=read_anndata, skip_dialog=True
         )
         d2 = df.load_data(
             os.path.join(DATA, "test_other_data.h5ad"),
             factory=read_anndata,
             skip_dialog=True,
@@ -272,15 +271,15 @@
         subset_group = self.dc.new_subset_group("T cells", state)
 
         # This is what we do in the dialog
         for subset in subset_group.subsets:
             if subset.data == self.dc[0].meta["var_data"]:
                 genesubset = subset
         with patch(
-            "glue_genes.glue_single_cell.qt.pca_subset.dialog"
+            "glue_genes.glue_single_cell.qt.summarize_gene_subset.dialog"
         ) as fakedialog:  # noqa: F841
             data_arr = do_calculation_over_gene_subset(
                 d1_adata, genesubset, calculation="Means"
             )
         assert data_arr is None
 
     def test_adding_to_dataset(self):
@@ -290,21 +289,20 @@
 
         assert len(d1_obs.components) == 5
 
         s = d1_var.new_subset()
         s.subset_state = d1_var.id["gene_stuff_0"] > 0
 
         data_arr = do_calculation_over_gene_subset(d1_adata, s, calculation="Means")
-        apply_data_arr(d1_obs, data_arr, "d1", key="Means")
+        apply_data_arr(d1_obs, data_arr, "d1", s, key="Means")
         assert len(d1_obs.components) == 6
 
 
 class TestCellSummaryBacked(TestCellSummary):
     def setup_method(self, method):
-
         d1 = df.load_data(
             os.path.join(DATA, "test_data.h5ad"),
             factory=read_anndata,
             skip_dialog=True,
             try_backed=True,
         )
         d2 = df.load_data(
```

### Comparing `glue-genes-1.0.1/glue_genes/glue_single_cell/qtl_viewer/layer_artist.py` & `glue-genes-1.1.0/glue_genes/glue_single_cell/qtl_viewer/layer_artist.py`

 * *Files identical despite different names*

### Comparing `glue-genes-1.0.1/glue_genes/glue_single_cell/qtl_viewer/qt/layer_style_editor.py` & `glue-genes-1.1.0/glue_genes/glue_single_cell/qtl_viewer/qt/layer_style_editor.py`

 * *Files identical despite different names*

### Comparing `glue-genes-1.0.1/glue_genes/glue_single_cell/qtl_viewer/qt/layer_style_editor.ui` & `glue-genes-1.1.0/glue_genes/glue_single_cell/qtl_viewer/qt/layer_style_editor.ui`

 * *Files 0% similar despite different names*

#### Comparing `glue-genes-1.0.1/glue_genes/glue_single_cell/qtl_viewer/qt/layer_style_editor.ui` & `glue-genes-1.1.0/glue_genes/glue_single_cell/qtl_viewer/qt/layer_style_editor.ui`

```diff
@@ -127,15 +127,15 @@
                     </size>
                   </property>
                 </spacer>
               </item>
               <item row="2" column="1" colspan="3">
                 <widget class="QComboBox" name="combosel_cmap_att">
                   <property name="sizeAdjustPolicy">
-                    <enum>QComboBox::AdjustToMinimumContentsLength</enum>
+                    <enum>QComboBox::AdjustToMinimumContentsLengthWithIcon</enum>
                   </property>
                 </widget>
               </item>
               <item row="0" column="1">
                 <widget class="QComboBox" name="combosel_cmap_mode">
                   <property name="maximumSize">
                     <size>
@@ -224,15 +224,15 @@
                   <property name="sizePolicy">
                     <sizepolicy hsizetype="Expanding" vsizetype="Fixed">
                       <horstretch>0</horstretch>
                       <verstretch>0</verstretch>
                     </sizepolicy>
                   </property>
                   <property name="sizeAdjustPolicy">
-                    <enum>QComboBox::AdjustToMinimumContentsLength</enum>
+                    <enum>QComboBox::AdjustToMinimumContentsLengthWithIcon</enum>
                   </property>
                 </widget>
               </item>
             </layout>
           </widget>
           <widget class="QWidget" name="tab_2">
             <attribute name="title">
@@ -262,15 +262,15 @@
                   <property name="maximumSize">
                     <size>
                       <width>120</width>
                       <height>16777215</height>
                     </size>
                   </property>
                   <property name="sizeAdjustPolicy">
-                    <enum>QComboBox::AdjustToMinimumContentsLength</enum>
+                    <enum>QComboBox::AdjustToMinimumContentsLengthWithIcon</enum>
                   </property>
                 </widget>
               </item>
               <item row="0" column="0">
                 <widget class="QLabel" name="label">
                   <property name="font">
                     <font>
@@ -467,15 +467,15 @@
               </item>
               <item row="2" column="3">
                 <widget class="QSpinBox" name="value_size"/>
               </item>
               <item row="4" column="1" colspan="3">
                 <widget class="QComboBox" name="combosel_size_att">
                   <property name="sizeAdjustPolicy">
-                    <enum>QComboBox::AdjustToMinimumContentsLength</enum>
+                    <enum>QComboBox::AdjustToMinimumContentsLengthWithIcon</enum>
                   </property>
                 </widget>
               </item>
               <item row="0" column="1" colspan="3">
                 <widget class="QCheckBox" name="bool_markers_visible">
                   <property name="text">
                     <string/>
@@ -510,15 +510,15 @@
                   <property name="maximumSize">
                     <size>
                       <width>16777215</width>
                       <height>16777215</height>
                     </size>
                   </property>
                   <property name="sizeAdjustPolicy">
-                    <enum>QComboBox::AdjustToMinimumContentsLength</enum>
+                    <enum>QComboBox::AdjustToMinimumContentsLengthWithIcon</enum>
                   </property>
                 </widget>
               </item>
               <item row="9" column="0">
                 <widget class="QLabel" name="label_contrast">
                   <property name="font">
                     <font>
```

### Comparing `glue-genes-1.0.1/glue_genes/glue_single_cell/qtl_viewer/qt/options_widget.py` & `glue-genes-1.1.0/glue_genes/glue_single_cell/qtl_viewer/qt/options_widget.py`

 * *Files identical despite different names*

### Comparing `glue-genes-1.0.1/glue_genes/glue_single_cell/qtl_viewer/qt/options_widget.ui` & `glue-genes-1.1.0/glue_genes/glue_single_cell/qtl_viewer/qt/options_widget.ui`

 * *Files 1% similar despite different names*

#### Comparing `glue-genes-1.0.1/glue_genes/glue_single_cell/qtl_viewer/qt/options_widget.ui` & `glue-genes-1.1.0/glue_genes/glue_single_cell/qtl_viewer/qt/options_widget.ui`

```diff
@@ -66,15 +66,15 @@
                     <string>x axis</string>
                   </property>
                 </widget>
               </item>
               <item row="0" column="1">
                 <widget class="QComboBox" name="combosel_x_att">
                   <property name="sizeAdjustPolicy">
-                    <enum>QComboBox::AdjustToMinimumContentsLength</enum>
+                    <enum>QComboBox::AdjustToMinimumContentsLengthWithIcon</enum>
                   </property>
                 </widget>
               </item>
               <item row="4" column="0">
                 <widget class="QLabel" name="LOD_lab">
                   <property name="font">
                     <font>
@@ -115,15 +115,15 @@
                     <string>Units</string>
                   </property>
                 </widget>
               </item>
               <item row="1" column="1">
                 <widget class="QComboBox" name="combosel_y_att">
                   <property name="sizeAdjustPolicy">
-                    <enum>QComboBox::AdjustToMinimumContentsLength</enum>
+                    <enum>QComboBox::AdjustToMinimumContentsLengthWithIcon</enum>
                   </property>
                 </widget>
               </item>
               <item row="2" column="1">
                 <widget class="QComboBox" name="combosel_species"/>
               </item>
               <item row="2" column="0">
```

### Comparing `glue-genes-1.0.1/glue_genes/glue_single_cell/qtl_viewer/qt/slider_with_label_widget.ui` & `glue-genes-1.1.0/glue_genes/glue_single_cell/qtl_viewer/qt/slider_with_label_widget.ui`

 * *Files identical despite different names*

### Comparing `glue-genes-1.0.1/glue_genes/glue_single_cell/qtl_viewer/state.py` & `glue-genes-1.1.0/glue_genes/glue_single_cell/qtl_viewer/state.py`

 * *Files identical despite different names*

### Comparing `glue-genes-1.0.1/glue_genes/glue_single_cell/qtl_viewer/tests/test_qtl_data_viewer.py` & `glue-genes-1.1.0/glue_genes/glue_single_cell/qtl_viewer/tests/test_qtl_data_viewer.py`

 * *Files identical despite different names*

### Comparing `glue-genes-1.0.1/glue_genes/glue_single_cell/qtl_viewer/viewer.py` & `glue-genes-1.1.0/glue_genes/glue_single_cell/qtl_viewer/viewer.py`

 * *Files identical despite different names*

### Comparing `glue-genes-1.0.1/glue_genes/glue_single_cell/state.py` & `glue-genes-1.1.0/glue_genes/glue_single_cell/state.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     DataCollectionComboHelper,
     ManualDataComboHelper,
 )
 from glue.core.state_objects import State
 
 from .data import DataAnnData
 
-__all__ = ["DiffGeneExpState", "PCASubsetState", "EnrichpyState"]
+__all__ = ["DiffGeneExpState", "SummarizeGeneSubsetState", "EnrichpyState"]
 
 
 class EnrichpyState(State):
     data = SelectionCallbackProperty()  # The data object to enrich
     subset = (
         SelectionCallbackProperty()
     )  # Required: a subset that can be applied to data
@@ -22,15 +22,14 @@
         SelectionCallbackProperty()
     )  # The Enrichr library to use. Could be linked to organism to get a filtered list.
     # This is a terrible name, because it is confusing with gene subsets
     # but this is the Enrichpy parameter name
     gene_att = SelectionCallbackProperty()  # The attribute with gene labels in it
 
     def __init__(self, data_collection):
-
         super(EnrichpyState, self).__init__()
 
         self.data_collection = data_collection
         self.data_helper = DataCollectionComboHelper(self, "data", data_collection)
         self.subset_helper = ComboHelper(self, "subset")
         self.gene_set_helper = ComboHelper(self, "gene_set")
 
@@ -66,23 +65,21 @@
         self.gene_set_helper.display = display_kegg_name
 
     def _on_data_change(self, *args, **kwargs):
         self.gene_att_helper.set_multiple_data([] if self.data is None else [self.data])
 
 
 class DiffGeneExpState(State):
-
     data = SelectionCallbackProperty()
     subset1 = SelectionCallbackProperty()
     subset2 = SelectionCallbackProperty()
     gene_att = SelectionCallbackProperty()
     num_genes = CallbackProperty(50)
 
     def __init__(self, data_collection):
-
         super(DiffGeneExpState, self).__init__()
 
         self.data_collection = data_collection
         self.data_helper = ManualDataComboHelper(self, "data", data_collection)
         self.gene_att_helper = ComponentIDComboHelper(
             self, "gene_att", categorical=True, numeric=True
         )
@@ -117,24 +114,23 @@
             self.gene_att_helper.set_multiple_data(
                 [] if self.data is None else [self.data.meta["var_data"]]
             )
         except:  # noqa E722
             pass
 
 
-class PCASubsetState(State):
-
+class SummarizeGeneSubsetState(State):
     data = SelectionCallbackProperty()
     genesubset = SelectionCallbackProperty()
     do_means = CallbackProperty(True)
     do_pca = CallbackProperty(False)
     do_module = CallbackProperty(False)
 
     def __init__(self, data_collection):
-        super(PCASubsetState, self).__init__()
+        super().__init__()
         self.data_collection = data_collection
         self.data_helper = ManualDataComboHelper(
             self, "data", data_collection
         )  # This should only allow cell-like datasets
         self.genesubset_helper = ComboHelper(
             self, "genesubset"
         )  # This should only allow subsets that are defined over genes...
```

### Comparing `glue-genes-1.0.1/glue_genes/glue_single_cell/tests/test_data/test_data.h5ad` & `glue-genes-1.1.0/glue_genes/glue_single_cell/tests/test_data/test_data.h5ad`

 * *Files identical despite different names*

### Comparing `glue-genes-1.0.1/glue_genes/glue_single_cell/tests/test_data/test_dataset.h5ad` & `glue-genes-1.1.0/glue_genes/glue_single_cell/tests/test_data/test_dataset.h5ad`

 * *Files identical despite different names*

### Comparing `glue-genes-1.0.1/glue_genes/glue_single_cell/tests/test_data/test_dataset_float32.h5ad` & `glue-genes-1.1.0/glue_genes/glue_single_cell/tests/test_data/test_dataset_float32.h5ad`

 * *Files identical despite different names*

### Comparing `glue-genes-1.0.1/glue_genes/glue_single_cell/tests/test_data_math.py` & `glue-genes-1.1.0/glue_genes/glue_single_cell/tests/test_data_math.py`

 * *Files identical despite different names*

### Comparing `glue-genes-1.0.1/glue_genes.egg-info/PKG-INFO` & `glue-genes-1.1.0/glue_genes.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: glue-genes
-Version: 1.0.1
+Version: 1.1.0
 Summary: Multidimensional data visualization for genomics
 Home-page: https://gluesolutions.github.io/glue-genes/
 Author: glue solutions inc.
 Author-email: jfoster@gluesolutions.io
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
@@ -15,15 +15,17 @@
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: License :: OSI Approved :: BSD License
 Provides: glue_genes
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: docs
 Provides-Extra: test
-Provides-Extra: qt
+Provides-Extra: qt5
+Provides-Extra: qt6
+Provides-Extra: openslide
 License-File: LICENSE
 
 ![glue_genes_logo_stacked](https://user-images.githubusercontent.com/3639698/137145077-2c2c9011-68bd-4770-9d58-494bf7632a33.png)
 
 
 The glue-genes meta-package
 ===========================
@@ -43,29 +45,22 @@
 
 * Data loaders for genomics data file formats such as .bed, .bigwig, .h5ad, and .loom
 * Viewers including: 2D Heatmap, Small Multiples, QTL Viewer
 * Menubar plug-ins to facilitate analysis of single-cell transcriptomics data
 
 ### Install
 
-Due to some complicated binary dependencies, the recommended procedure for 
-installing this package is to use [conda](https://www.anaconda.com) and install into a new environment as follows:
+See [the glue genes documentation](https://glue-genes.readthedocs.io/en/latest/how-to/installation.html) for installation help.
 
-```
-conda create -n glue-genes python==3.9
-conda activate glue-genes
-
-conda install glue-core
-pip install glue-genes
-```
+We recommend installing into a new virtual environment. 
 
-### Usage
-
-The Scanpy differential gene expression plugin requires some custom actions to run at startup, which can be achieved by starting glue using this command:
+`pip install glue-genes[qt6]`
 
-`glue --startup=setup_anndata`
+### Usage
 
+After installation, glue (with the glue genes plug-ins loaded) can be invoked at the terminal:
+`glue`
 
 
 ### Development
 
 glue genes is under active development. Please file all bug reports as github issues.
```

### Comparing `glue-genes-1.0.1/glue_genes.egg-info/SOURCES.txt` & `glue-genes-1.1.0/glue_genes.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 .gitignore
 .readthedocs.yml
 CHANGES.md
 LICENSE
 README.md
+codecov.yml
 environment.yml
-pyproject.toml
 setup.cfg
 setup.py
 tox.ini
+.github/release.yml
 .github/workflows/ci_workflows.yml
 .github/workflows/python-package-conda.yml
 .github/workflows/static.yml
+.github/workflows/update-changelog.yaml
 docs/Makefile
 docs/make.bat
 docs/requirements.txt
 docs/source/conf.py
 docs/source/index.rst
 docs/source/_static/style.css
 docs/source/api/index.rst
@@ -78,33 +80,41 @@
 glue_genes.egg-info/entry_points.txt
 glue_genes.egg-info/not-zip-safe
 glue_genes.egg-info/requires.txt
 glue_genes.egg-info/top_level.txt
 glue_genes/glue_genomics_data/__init__.py
 glue_genes/glue_genomics_data/bed_factory.py
 glue_genes/glue_genomics_data/bigwig_factory.py
+glue_genes/glue_genomics_data/multires_data.py
+glue_genes/glue_genomics_data/ome_zarr_factory.py
+glue_genes/glue_genomics_data/openslide_factory.py
+glue_genes/glue_genomics_data/spaceranger_factory.py
+glue_genes/glue_genomics_data/zarr_factory.py
+glue_genes/glue_genomics_data/tests/test_multi_resolution_data.py
 glue_genes/glue_single_cell/__init__.py
 glue_genes/glue_single_cell/anndata_factory.py
+glue_genes/glue_single_cell/component.py
 glue_genes/glue_single_cell/data.py
 glue_genes/glue_single_cell/menubar_plugin.py
 glue_genes/glue_single_cell/state.py
 glue_genes/glue_single_cell/qt/__init__.py
 glue_genes/glue_single_cell/qt/diff_gene_exp.py
 glue_genes/glue_single_cell/qt/diff_gene_exp.ui
 glue_genes/glue_single_cell/qt/enrichr.py
 glue_genes/glue_single_cell/qt/enrichr.ui
 glue_genes/glue_single_cell/qt/load_data.py
 glue_genes/glue_single_cell/qt/load_data.ui
-glue_genes/glue_single_cell/qt/pca_subset.py
-glue_genes/glue_single_cell/qt/pca_subset.ui
+glue_genes/glue_single_cell/qt/summarize_gene_subset.py
+glue_genes/glue_single_cell/qt/summarize_gene_subset.ui
 glue_genes/glue_single_cell/qt/tests/__init__.py
 glue_genes/glue_single_cell/qt/tests/test_data_load.py
 glue_genes/glue_single_cell/qt/tests/test_diff_gene_exp.py
 glue_genes/glue_single_cell/qt/tests/test_enrichr.py
-glue_genes/glue_single_cell/qt/tests/test_pca_subset.py
+glue_genes/glue_single_cell/qt/tests/test_summarize_gene_subset.py
+glue_genes/glue_single_cell/qt/tests/data/__init__.py
 glue_genes/glue_single_cell/qt/tests/data/test_data.h5ad
 glue_genes/glue_single_cell/qt/tests/data/test_data_compressed.h5ad
 glue_genes/glue_single_cell/qt/tests/data/test_data_dense.h5ad
 glue_genes/glue_single_cell/qt/tests/data/test_data_dense_compressed.h5ad
 glue_genes/glue_single_cell/qt/tests/data/test_other_data.h5ad
 glue_genes/glue_single_cell/qtl_viewer/__init__.py
 glue_genes/glue_single_cell/qtl_viewer/layer_artist.py
@@ -116,10 +126,12 @@
 glue_genes/glue_single_cell/qtl_viewer/qt/options_widget.py
 glue_genes/glue_single_cell/qtl_viewer/qt/options_widget.ui
 glue_genes/glue_single_cell/qtl_viewer/qt/slider_with_label_widget.ui
 glue_genes/glue_single_cell/qtl_viewer/tests/__init__.py
 glue_genes/glue_single_cell/qtl_viewer/tests/test_qtl_data_viewer.py
 glue_genes/glue_single_cell/tests/context.py
 glue_genes/glue_single_cell/tests/test_data_math.py
+glue_genes/glue_single_cell/tests/test_synccomponent.py
+glue_genes/glue_single_cell/tests/test_data/__init__.py
 glue_genes/glue_single_cell/tests/test_data/test_data.h5ad
 glue_genes/glue_single_cell/tests/test_data/test_dataset.h5ad
 glue_genes/glue_single_cell/tests/test_data/test_dataset_float32.h5ad
```

### Comparing `glue-genes-1.0.1/setup.cfg` & `glue-genes-1.1.0/setup.cfg`

 * *Files 22% similar despite different names*

```diff
@@ -20,23 +20,23 @@
 
 [options]
 zip_safe = False
 packages = find:
 python_requires = >=3.8
 setup_requires = setuptools_scm
 install_requires = 
-	glue-core>=1.8.0
+	glue-core-for-glue-genes
 	qtpy>=1.9
-	glue-small-multiples>=1.0
-	glue-heatmap>=1.0
-	glue-vispy-viewers>=1.0.6
 	anndata>=0.8
 	scanpy>=1.9
 	enrichrpy>=0.1
 	pyranges>=0.0.120
+	squidpy
+	zarr>=2
+	ome-zarr
 
 [options.entry_points]
 glue.plugins = 
 	glue_single_cell = glue_genes.glue_single_cell:setup
 	glue_genomics_data = glue_genes.glue_genomics_data:setup
 
 [options.extras_require]
@@ -44,28 +44,34 @@
 	sphinx
 	sphinxcontrib-spelling
 	numpydoc
 	pytest-doctestplus
 	sphinx_design
 	furo
 test = 
-	PyQt5>=5.14
 	pytest
+	pytest-cov
+	pytest-faulthandler
+	pytest-flake8
 	pytest-doctestplus
 	mock
-qt = 
-	PyQt5>=5.14
+qt5 = 
+	PyQt5>=5.15
+qt6 = 
+	PyQt6==6.4.*
+	pyqt6-qt6==6.4.* # PyQt6.5 does not work yet
+openslide = 
+	openslide-python # Only(?) available through Conda unless OpenSlide already installed
+	napari-lazy-openslide
 
 [options.package_data]
-* = *.png, *.ui, *.glu, *.hdf5, *.xlsx, *.txt, *.csv, *.svg, *.bgz, *.tbi *.h5ad
+* = *.png, *.ui, *.glu, *.hdf5, *.xlsx, *.txt, *.csv, *.svg, *.bgz, *.tbi, *.h5ad
 
 [tool:pytest]
 minversion = 6
-testpaths = docs glue_genes
-doctest_plus = enabled
 xfail_strict = true
 filterwarnings = 
 	error
 	ignore:numpy\.ndarray size changed:RuntimeWarning
 	ignore::PendingDeprecationWarning:xlrd
 	ignore:Session._key_changed is deprecated
 	ignore:zmq.* is deprecated
```

### Comparing `glue-genes-1.0.1/tox.ini` & `glue-genes-1.1.0/tox.ini`

 * *Files 15% similar despite different names*

```diff
@@ -1,37 +1,33 @@
 [tox]
-envlist = py{38,39,310}-{test,docs}-{pyqt514,pyqt515,pyqt63,pyqt64,pyside514,pyside515,pyside63,pyside64}-{stable,dev}
+envlist = py{38,39,310,311}-{test,docs}-{pyqt514,pyqt515,pyqt63,pyqt64,pyside514,pyside515,pyside63}
 requires = pip >= 18.0
            setuptools >= 30.3.0
 
 [testenv]
 passenv =
     DISPLAY
     HOME
 changedir =
+    test: .tmp/{envname}
     docs: docs
 deps =
     pyqt514: PyQt5==5.14.*
     pyqt515: PyQt5==5.15.*
     pyqt63: PyQt6==6.3.*
     pyqt64: PyQt6==6.4.*
-    pyside514: PySide2==5.14.*
     pyside515: PySide2==5.15.*
     pyside63: PySide6==6.3.*
-    pyside64: PySide6==6.4.*
-    dev: git+https://github.com/glue-viz/glue
-    stable: glue-core==1.6.*
     all: pytest-qt
-
 extras =
     test: test
     docs: docs
 commands =
-    pip freeze
-    test: pytest glue_genes
+    test: pip freeze
+    test: pytest --pyargs glue_genes --cov glue_genes {posargs}
     docs: sphinx-build -W -b html -d _build/doctrees   . _build/html
 
 [testenv:codestyle]
 deps = flake8
 skip_install = true
 commands =
     flake8 glue_genes
```

