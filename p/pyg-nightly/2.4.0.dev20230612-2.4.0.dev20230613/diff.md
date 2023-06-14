# Comparing `tmp/pyg_nightly-2.4.0.dev20230612.tar.gz` & `tmp/pyg_nightly-2.4.0.dev20230613.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyg_nightly-2.4.0.dev20230612.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "pyg_nightly-2.4.0.dev20230613.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `pyg_nightly-2.4.0.dev20230612.tar` & `pyg_nightly-2.4.0.dev20230613.tar`

### file list

```diff
@@ -1,564 +1,564 @@
--rw-r--r--   0        0        0    60889 2023-06-12 06:06:11.551693 pyg_nightly-2.4.0.dev20230612/README.md
--rw-r--r--   0        0        0     4092 2023-06-12 06:06:12.079696 pyg_nightly-2.4.0.dev20230612/pyproject.toml
--rw-r--r--   0        0        0     1055 2023-06-12 06:06:12.075696 pyg_nightly-2.4.0.dev20230612/torch_geometric/__init__.py
--rw-r--r--   0        0        0     3392 2023-06-12 06:06:11.599693 pyg_nightly-2.4.0.dev20230612/torch_geometric/compile.py
--rw-r--r--   0        0        0      352 2023-06-12 06:06:11.599693 pyg_nightly-2.4.0.dev20230612/torch_geometric/contrib/__init__.py
--rw-r--r--   0        0        0       23 2023-06-12 06:06:11.599693 pyg_nightly-2.4.0.dev20230612/torch_geometric/contrib/datasets/__init__.py
--rw-r--r--   0        0        0      163 2023-06-12 06:06:11.599693 pyg_nightly-2.4.0.dev20230612/torch_geometric/contrib/explain/__init__.py
--rw-r--r--   0        0        0    22723 2023-06-12 06:06:11.599693 pyg_nightly-2.4.0.dev20230612/torch_geometric/contrib/explain/graphmask_explainer.py
--rw-r--r--   0        0        0    16627 2023-06-12 06:06:11.599693 pyg_nightly-2.4.0.dev20230612/torch_geometric/contrib/explain/pgm_explainer.py
--rw-r--r--   0        0        0       72 2023-06-12 06:06:11.599693 pyg_nightly-2.4.0.dev20230612/torch_geometric/contrib/nn/__init__.py
--rw-r--r--   0        0        0       23 2023-06-12 06:06:11.599693 pyg_nightly-2.4.0.dev20230612/torch_geometric/contrib/nn/conv/__init__.py
--rw-r--r--   0        0        0      113 2023-06-12 06:06:11.599693 pyg_nightly-2.4.0.dev20230612/torch_geometric/contrib/nn/models/__init__.py
--rw-r--r--   0        0        0    33261 2023-06-12 06:06:11.599693 pyg_nightly-2.4.0.dev20230612/torch_geometric/contrib/nn/models/rbcd_attack.py
--rw-r--r--   0        0        0       23 2023-06-12 06:06:11.599693 pyg_nightly-2.4.0.dev20230612/torch_geometric/contrib/transforms/__init__.py
--rw-r--r--   0        0        0     3383 2023-06-12 06:06:11.599693 pyg_nightly-2.4.0.dev20230612/torch_geometric/data/__init__.py
--rw-r--r--   0        0        0     7428 2023-06-12 06:06:11.599693 pyg_nightly-2.4.0.dev20230612/torch_geometric/data/batch.py
--rw-r--r--   0        0        0    10658 2023-06-12 06:06:11.599693 pyg_nightly-2.4.0.dev20230612/torch_geometric/data/collate.py
--rw-r--r--   0        0        0    37497 2023-06-12 06:06:11.599693 pyg_nightly-2.4.0.dev20230612/torch_geometric/data/data.py
--rw-r--r--   0        0        0     2922 2023-06-12 06:06:11.599693 pyg_nightly-2.4.0.dev20230612/torch_geometric/data/datapipes.py
--rw-r--r--   0        0        0    15051 2023-06-12 06:06:11.599693 pyg_nightly-2.4.0.dev20230612/torch_geometric/data/dataset.py
--rw-r--r--   0        0        0     1359 2023-06-12 06:06:11.599693 pyg_nightly-2.4.0.dev20230612/torch_geometric/data/download.py
--rw-r--r--   0        0        0     2252 2023-06-12 06:06:11.603693 pyg_nightly-2.4.0.dev20230612/torch_geometric/data/extract.py
--rw-r--r--   0        0        0    21075 2023-06-12 06:06:11.603693 pyg_nightly-2.4.0.dev20230612/torch_geometric/data/feature_store.py
--rw-r--r--   0        0        0    13495 2023-06-12 06:06:11.603693 pyg_nightly-2.4.0.dev20230612/torch_geometric/data/graph_store.py
--rw-r--r--   0        0        0    44329 2023-06-12 06:06:11.603693 pyg_nightly-2.4.0.dev20230612/torch_geometric/data/hetero_data.py
--rw-r--r--   0        0        0     8072 2023-06-12 06:06:11.603693 pyg_nightly-2.4.0.dev20230612/torch_geometric/data/in_memory_dataset.py
--rw-r--r--   0        0        0      178 2023-06-12 06:06:11.603693 pyg_nightly-2.4.0.dev20230612/torch_geometric/data/lightning/__init__.py
--rw-r--r--   0        0        0    28490 2023-06-12 06:06:11.603693 pyg_nightly-2.4.0.dev20230612/torch_geometric/data/lightning/datamodule.py
--rw-r--r--   0        0        0      338 2023-06-12 06:06:11.603693 pyg_nightly-2.4.0.dev20230612/torch_geometric/data/makedirs.py
--rw-r--r--   0        0        0     3962 2023-06-12 06:06:11.603693 pyg_nightly-2.4.0.dev20230612/torch_geometric/data/remote_backend_utils.py
--rw-r--r--   0        0        0     4360 2023-06-12 06:06:11.603693 pyg_nightly-2.4.0.dev20230612/torch_geometric/data/separate.py
--rw-r--r--   0        0        0    25245 2023-06-12 06:06:11.603693 pyg_nightly-2.4.0.dev20230612/torch_geometric/data/storage.py
--rw-r--r--   0        0        0     5219 2023-06-12 06:06:11.603693 pyg_nightly-2.4.0.dev20230612/torch_geometric/data/summary.py
--rw-r--r--   0        0        0     9354 2023-06-12 06:06:11.603693 pyg_nightly-2.4.0.dev20230612/torch_geometric/data/temporal.py
--rw-r--r--   0        0        0     1038 2023-06-12 06:06:11.603693 pyg_nightly-2.4.0.dev20230612/torch_geometric/data/view.py
--rw-r--r--   0        0        0     5300 2023-06-12 06:06:11.603693 pyg_nightly-2.4.0.dev20230612/torch_geometric/datasets/__init__.py
--rw-r--r--   0        0        0     4220 2023-06-12 06:06:11.603693 pyg_nightly-2.4.0.dev20230612/torch_geometric/datasets/actor.py
--rw-r--r--   0        0        0     5584 2023-06-12 06:06:11.603693 pyg_nightly-2.4.0.dev20230612/torch_geometric/datasets/airfrans.py
--rw-r--r--   0        0        0     3711 2023-06-12 06:06:11.603693 pyg_nightly-2.4.0.dev20230612/torch_geometric/datasets/airports.py
--rw-r--r--   0        0        0     3050 2023-06-12 06:06:11.603693 pyg_nightly-2.4.0.dev20230612/torch_geometric/datasets/amazon.py
--rw-r--r--   0        0        0     3109 2023-06-12 06:06:11.603693 pyg_nightly-2.4.0.dev20230612/torch_geometric/datasets/amazon_book.py
--rw-r--r--   0        0        0     4099 2023-06-12 06:06:11.603693 pyg_nightly-2.4.0.dev20230612/torch_geometric/datasets/amazon_products.py
--rw-r--r--   0        0        0     4942 2023-06-12 06:06:11.603693 pyg_nightly-2.4.0.dev20230612/torch_geometric/datasets/aminer.py
--rw-r--r--   0        0        0     5266 2023-06-12 06:06:11.603693 pyg_nightly-2.4.0.dev20230612/torch_geometric/datasets/aqsol.py
--rw-r--r--   0        0        0     5735 2023-06-12 06:06:11.603693 pyg_nightly-2.4.0.dev20230612/torch_geometric/datasets/attributed_graph_dataset.py
--rw-r--r--   0        0        0     4063 2023-06-12 06:06:11.603693 pyg_nightly-2.4.0.dev20230612/torch_geometric/datasets/ba2motif_dataset.py
--rw-r--r--   0        0        0     3518 2023-06-12 06:06:11.603693 pyg_nightly-2.4.0.dev20230612/torch_geometric/datasets/ba_multi_shapes.py
--rw-r--r--   0        0        0     3824 2023-06-12 06:06:11.603693 pyg_nightly-2.4.0.dev20230612/torch_geometric/datasets/ba_shapes.py
--rw-r--r--   0        0        0     4137 2023-06-12 06:06:11.603693 pyg_nightly-2.4.0.dev20230612/torch_geometric/datasets/bitcoin_otc.py
--rw-r--r--   0        0        0     4205 2023-06-12 06:06:11.603693 pyg_nightly-2.4.0.dev20230612/torch_geometric/datasets/citation_full.py
--rw-r--r--   0        0        0     3009 2023-06-12 06:06:11.603693 pyg_nightly-2.4.0.dev20230612/torch_geometric/datasets/coauthor.py
--rw-r--r--   0        0        0     4564 2023-06-12 06:06:11.603693 pyg_nightly-2.4.0.dev20230612/torch_geometric/datasets/coma.py
--rw-r--r--   0        0        0     5192 2023-06-12 06:06:11.603693 pyg_nightly-2.4.0.dev20230612/torch_geometric/datasets/dblp.py
--rw-r--r--   0        0        0     5608 2023-06-12 06:06:11.603693 pyg_nightly-2.4.0.dev20230612/torch_geometric/datasets/dbp15k.py
--rw-r--r--   0        0        0     2308 2023-06-12 06:06:11.603693 pyg_nightly-2.4.0.dev20230612/torch_geometric/datasets/deezer_europe.py
--rw-r--r--   0        0        0     3862 2023-06-12 06:06:11.603693 pyg_nightly-2.4.0.dev20230612/torch_geometric/datasets/dgraph.py
--rw-r--r--   0        0        0     5865 2023-06-12 06:06:11.603693 pyg_nightly-2.4.0.dev20230612/torch_geometric/datasets/dynamic_faust.py
--rw-r--r--   0        0        0     4498 2023-06-12 06:06:11.603693 pyg_nightly-2.4.0.dev20230612/torch_geometric/datasets/elliptic.py
--rw-r--r--   0        0        0     2990 2023-06-12 06:06:11.603693 pyg_nightly-2.4.0.dev20230612/torch_geometric/datasets/elliptic_temporal.py
--rw-r--r--   0        0        0     2631 2023-06-12 06:06:11.603693 pyg_nightly-2.4.0.dev20230612/torch_geometric/datasets/email_eu_core.py
--rw-r--r--   0        0        0     7001 2023-06-12 06:06:11.603693 pyg_nightly-2.4.0.dev20230612/torch_geometric/datasets/entities.py
--rw-r--r--   0        0        0     5817 2023-06-12 06:06:11.603693 pyg_nightly-2.4.0.dev20230612/torch_geometric/datasets/explainer_dataset.py
--rw-r--r--   0        0        0     2228 2023-06-12 06:06:11.603693 pyg_nightly-2.4.0.dev20230612/torch_geometric/datasets/facebook.py
--rw-r--r--   0        0        0    10215 2023-06-12 06:06:11.603693 pyg_nightly-2.4.0.dev20230612/torch_geometric/datasets/fake.py
--rw-r--r--   0        0        0     3924 2023-06-12 06:06:11.603693 pyg_nightly-2.4.0.dev20230612/torch_geometric/datasets/faust.py
--rw-r--r--   0        0        0     4099 2023-06-12 06:06:11.603693 pyg_nightly-2.4.0.dev20230612/torch_geometric/datasets/flickr.py
--rw-r--r--   0        0        0     3815 2023-06-12 06:06:11.603693 pyg_nightly-2.4.0.dev20230612/torch_geometric/datasets/freebase.py
--rw-r--r--   0        0        0     3416 2023-06-12 06:06:11.603693 pyg_nightly-2.4.0.dev20230612/torch_geometric/datasets/gdelt.py
--rw-r--r--   0        0        0     2967 2023-06-12 06:06:11.603693 pyg_nightly-2.4.0.dev20230612/torch_geometric/datasets/gdelt_lite.py
--rw-r--r--   0        0        0     9261 2023-06-12 06:06:11.603693 pyg_nightly-2.4.0.dev20230612/torch_geometric/datasets/ged_dataset.py
--rw-r--r--   0        0        0     2626 2023-06-12 06:06:11.603693 pyg_nightly-2.4.0.dev20230612/torch_geometric/datasets/gemsec.py
--rw-r--r--   0        0        0     3954 2023-06-12 06:06:11.603693 pyg_nightly-2.4.0.dev20230612/torch_geometric/datasets/geometry.py
--rw-r--r--   0        0        0     2484 2023-06-12 06:06:11.603693 pyg_nightly-2.4.0.dev20230612/torch_geometric/datasets/github.py
--rw-r--r--   0        0        0     6762 2023-06-12 06:06:11.603693 pyg_nightly-2.4.0.dev20230612/torch_geometric/datasets/gnn_benchmark_dataset.py
--rw-r--r--   0        0        0      221 2023-06-12 06:06:11.607693 pyg_nightly-2.4.0.dev20230612/torch_geometric/datasets/graph_generator/__init__.py
--rw-r--r--   0        0        0      965 2023-06-12 06:06:11.607693 pyg_nightly-2.4.0.dev20230612/torch_geometric/datasets/graph_generator/ba_graph.py
--rw-r--r--   0        0        0      949 2023-06-12 06:06:11.607693 pyg_nightly-2.4.0.dev20230612/torch_geometric/datasets/graph_generator/base.py
--rw-r--r--   0        0        0      918 2023-06-12 06:06:11.607693 pyg_nightly-2.4.0.dev20230612/torch_geometric/datasets/graph_generator/er_graph.py
--rw-r--r--   0        0        0     1159 2023-06-12 06:06:11.607693 pyg_nightly-2.4.0.dev20230612/torch_geometric/datasets/graph_generator/grid_graph.py
--rw-r--r--   0        0        0     4043 2023-06-12 06:06:11.607693 pyg_nightly-2.4.0.dev20230612/torch_geometric/datasets/heterophilous_graph_dataset.py
--rw-r--r--   0        0        0     8467 2023-06-12 06:06:11.607693 pyg_nightly-2.4.0.dev20230612/torch_geometric/datasets/hgb_dataset.py
--rw-r--r--   0        0        0     6541 2023-06-12 06:06:11.607693 pyg_nightly-2.4.0.dev20230612/torch_geometric/datasets/hm.py
--rw-r--r--   0        0        0    11053 2023-06-12 06:06:11.607693 pyg_nightly-2.4.0.dev20230612/torch_geometric/datasets/hydro_net.py
--rw-r--r--   0        0        0     4447 2023-06-12 06:06:11.607693 pyg_nightly-2.4.0.dev20230612/torch_geometric/datasets/icews.py
--rw-r--r--   0        0        0     4389 2023-06-12 06:06:11.607693 pyg_nightly-2.4.0.dev20230612/torch_geometric/datasets/igmc_dataset.py
--rw-r--r--   0        0        0     4000 2023-06-12 06:06:11.607693 pyg_nightly-2.4.0.dev20230612/torch_geometric/datasets/imdb.py
--rw-r--r--   0        0        0     7169 2023-06-12 06:06:11.607693 pyg_nightly-2.4.0.dev20230612/torch_geometric/datasets/infection_dataset.py
--rw-r--r--   0        0        0     3439 2023-06-12 06:06:11.607693 pyg_nightly-2.4.0.dev20230612/torch_geometric/datasets/jodie.py
--rw-r--r--   0        0        0     3444 2023-06-12 06:06:11.607693 pyg_nightly-2.4.0.dev20230612/torch_geometric/datasets/karate.py
--rw-r--r--   0        0        0     4349 2023-06-12 06:06:11.607693 pyg_nightly-2.4.0.dev20230612/torch_geometric/datasets/last_fm.py
--rw-r--r--   0        0        0     2283 2023-06-12 06:06:11.607693 pyg_nightly-2.4.0.dev20230612/torch_geometric/datasets/lastfm_asia.py
--rw-r--r--   0        0        0     6582 2023-06-12 06:06:11.607693 pyg_nightly-2.4.0.dev20230612/torch_geometric/datasets/linkx_dataset.py
--rw-r--r--   0        0        0    11559 2023-06-12 06:06:11.607693 pyg_nightly-2.4.0.dev20230612/torch_geometric/datasets/lrgb.py
--rw-r--r--   0        0        0     5044 2023-06-12 06:06:11.607693 pyg_nightly-2.4.0.dev20230612/torch_geometric/datasets/malnet_tiny.py
--rw-r--r--   0        0        0    16482 2023-06-12 06:06:11.607693 pyg_nightly-2.4.0.dev20230612/torch_geometric/datasets/md17.py
--rw-r--r--   0        0        0     3770 2023-06-12 06:06:11.607693 pyg_nightly-2.4.0.dev20230612/torch_geometric/datasets/mixhop_synthetic_dataset.py
--rw-r--r--   0        0        0     3136 2023-06-12 06:06:11.607693 pyg_nightly-2.4.0.dev20230612/torch_geometric/datasets/mnist_superpixels.py
--rw-r--r--   0        0        0     5251 2023-06-12 06:06:11.607693 pyg_nightly-2.4.0.dev20230612/torch_geometric/datasets/modelnet.py
--rw-r--r--   0        0        0     6593 2023-06-12 06:06:11.607693 pyg_nightly-2.4.0.dev20230612/torch_geometric/datasets/molecule_net.py
--rw-r--r--   0        0        0      227 2023-06-12 06:06:11.607693 pyg_nightly-2.4.0.dev20230612/torch_geometric/datasets/motif_generator/__init__.py
--rw-r--r--   0        0        0      910 2023-06-12 06:06:11.607693 pyg_nightly-2.4.0.dev20230612/torch_geometric/datasets/motif_generator/base.py
--rw-r--r--   0        0        0     1203 2023-06-12 06:06:11.607693 pyg_nightly-2.4.0.dev20230612/torch_geometric/datasets/motif_generator/custom.py
--rw-r--r--   0        0        0      984 2023-06-12 06:06:11.607693 pyg_nightly-2.4.0.dev20230612/torch_geometric/datasets/motif_generator/cycle.py
--rw-r--r--   0        0        0      801 2023-06-12 06:06:11.607693 pyg_nightly-2.4.0.dev20230612/torch_geometric/datasets/motif_generator/house.py
--rw-r--r--   0        0        0     3807 2023-06-12 06:06:11.607693 pyg_nightly-2.4.0.dev20230612/torch_geometric/datasets/movie_lens.py
--rw-r--r--   0        0        0     6002 2023-06-12 06:06:11.607693 pyg_nightly-2.4.0.dev20230612/torch_geometric/datasets/movie_lens_100k.py
--rw-r--r--   0        0        0     5162 2023-06-12 06:06:11.607693 pyg_nightly-2.4.0.dev20230612/torch_geometric/datasets/movie_lens_1m.py
--rw-r--r--   0        0        0     2889 2023-06-12 06:06:11.607693 pyg_nightly-2.4.0.dev20230612/torch_geometric/datasets/nell.py
--rw-r--r--   0        0        0     7190 2023-06-12 06:06:11.607693 pyg_nightly-2.4.0.dev20230612/torch_geometric/datasets/ogb_mag.py
--rw-r--r--   0        0        0     3415 2023-06-12 06:06:11.607693 pyg_nightly-2.4.0.dev20230612/torch_geometric/datasets/omdb.py
--rw-r--r--   0        0        0     3964 2023-06-12 06:06:11.607693 pyg_nightly-2.4.0.dev20230612/torch_geometric/datasets/particle.py
--rw-r--r--   0        0        0    11009 2023-06-12 06:06:11.607693 pyg_nightly-2.4.0.dev20230612/torch_geometric/datasets/pascal.py
--rw-r--r--   0        0        0     4602 2023-06-12 06:06:11.607693 pyg_nightly-2.4.0.dev20230612/torch_geometric/datasets/pascal_pf.py
--rw-r--r--   0        0        0     5716 2023-06-12 06:06:11.607693 pyg_nightly-2.4.0.dev20230612/torch_geometric/datasets/pcpnet_dataset.py
--rw-r--r--   0        0        0     6975 2023-06-12 06:06:11.607693 pyg_nightly-2.4.0.dev20230612/torch_geometric/datasets/planetoid.py
--rw-r--r--   0        0        0     2842 2023-06-12 06:06:11.607693 pyg_nightly-2.4.0.dev20230612/torch_geometric/datasets/polblogs.py
--rw-r--r--   0        0        0     4866 2023-06-12 06:06:11.607693 pyg_nightly-2.4.0.dev20230612/torch_geometric/datasets/ppi.py
--rw-r--r--   0        0        0     3182 2023-06-12 06:06:11.607693 pyg_nightly-2.4.0.dev20230612/torch_geometric/datasets/qm7.py
--rw-r--r--   0        0        0    16813 2023-06-12 06:06:11.607693 pyg_nightly-2.4.0.dev20230612/torch_geometric/datasets/qm9.py
--rw-r--r--   0        0        0     2941 2023-06-12 06:06:11.607693 pyg_nightly-2.4.0.dev20230612/torch_geometric/datasets/reddit.py
--rw-r--r--   0        0        0     4439 2023-06-12 06:06:11.607693 pyg_nightly-2.4.0.dev20230612/torch_geometric/datasets/reddit2.py
--rw-r--r--   0        0        0     4345 2023-06-12 06:06:11.607693 pyg_nightly-2.4.0.dev20230612/torch_geometric/datasets/rel_link_pred_dataset.py
--rw-r--r--   0        0        0     4173 2023-06-12 06:06:11.607693 pyg_nightly-2.4.0.dev20230612/torch_geometric/datasets/s3dis.py
--rw-r--r--   0        0        0     8140 2023-06-12 06:06:11.607693 pyg_nightly-2.4.0.dev20230612/torch_geometric/datasets/sbm_dataset.py
--rw-r--r--   0        0        0     8088 2023-06-12 06:06:11.607693 pyg_nightly-2.4.0.dev20230612/torch_geometric/datasets/shapenet.py
--rw-r--r--   0        0        0     6150 2023-06-12 06:06:11.607693 pyg_nightly-2.4.0.dev20230612/torch_geometric/datasets/shrec2016.py
--rw-r--r--   0        0        0     9283 2023-06-12 06:06:11.607693 pyg_nightly-2.4.0.dev20230612/torch_geometric/datasets/snap_dataset.py
--rw-r--r--   0        0        0     3031 2023-06-12 06:06:11.607693 pyg_nightly-2.4.0.dev20230612/torch_geometric/datasets/suite_sparse.py
--rw-r--r--   0        0        0     3959 2023-06-12 06:06:11.607693 pyg_nightly-2.4.0.dev20230612/torch_geometric/datasets/taobao.py
--rw-r--r--   0        0        0     4451 2023-06-12 06:06:11.607693 pyg_nightly-2.4.0.dev20230612/torch_geometric/datasets/tosca.py
--rw-r--r--   0        0        0     7302 2023-06-12 06:06:11.607693 pyg_nightly-2.4.0.dev20230612/torch_geometric/datasets/tu_dataset.py
--rw-r--r--   0        0        0     3464 2023-06-12 06:06:11.607693 pyg_nightly-2.4.0.dev20230612/torch_geometric/datasets/twitch.py
--rw-r--r--   0        0        0     6929 2023-06-12 06:06:11.607693 pyg_nightly-2.4.0.dev20230612/torch_geometric/datasets/upfd.py
--rw-r--r--   0        0        0      182 2023-06-12 06:06:11.611693 pyg_nightly-2.4.0.dev20230612/torch_geometric/datasets/utils/__init__.py
--rw-r--r--   0        0        0     1732 2023-06-12 06:06:11.611693 pyg_nightly-2.4.0.dev20230612/torch_geometric/datasets/utils/cheatsheet.py
--rw-r--r--   0        0        0     4615 2023-06-12 06:06:11.611693 pyg_nightly-2.4.0.dev20230612/torch_geometric/datasets/webkb.py
--rw-r--r--   0        0        0     3674 2023-06-12 06:06:11.611693 pyg_nightly-2.4.0.dev20230612/torch_geometric/datasets/wikics.py
--rw-r--r--   0        0        0     6083 2023-06-12 06:06:11.611693 pyg_nightly-2.4.0.dev20230612/torch_geometric/datasets/wikipedia_network.py
--rw-r--r--   0        0        0     6632 2023-06-12 06:06:11.611693 pyg_nightly-2.4.0.dev20230612/torch_geometric/datasets/willow_object_class.py
--rw-r--r--   0        0        0     7857 2023-06-12 06:06:11.611693 pyg_nightly-2.4.0.dev20230612/torch_geometric/datasets/word_net.py
--rw-r--r--   0        0        0     4116 2023-06-12 06:06:11.611693 pyg_nightly-2.4.0.dev20230612/torch_geometric/datasets/yelp.py
--rw-r--r--   0        0        0     6171 2023-06-12 06:06:11.611693 pyg_nightly-2.4.0.dev20230612/torch_geometric/datasets/zinc.py
--rw-r--r--   0        0        0     1197 2023-06-12 06:06:11.611693 pyg_nightly-2.4.0.dev20230612/torch_geometric/debug.py
--rw-r--r--   0        0        0      748 2023-06-12 06:06:11.611693 pyg_nightly-2.4.0.dev20230612/torch_geometric/deprecation.py
--rw-r--r--   0        0        0      171 2023-06-12 06:06:11.611693 pyg_nightly-2.4.0.dev20230612/torch_geometric/distributed/__init__.py
--rw-r--r--   0        0        0     3679 2023-06-12 06:06:11.611693 pyg_nightly-2.4.0.dev20230612/torch_geometric/distributed/local_feature_store.py
--rw-r--r--   0        0        0     1835 2023-06-12 06:06:11.611693 pyg_nightly-2.4.0.dev20230612/torch_geometric/distributed/local_graph_store.py
--rw-r--r--   0        0        0     4618 2023-06-12 06:06:11.611693 pyg_nightly-2.4.0.dev20230612/torch_geometric/experimental.py
--rw-r--r--   0        0        0      359 2023-06-12 06:06:11.611693 pyg_nightly-2.4.0.dev20230612/torch_geometric/explain/__init__.py
--rw-r--r--   0        0        0      418 2023-06-12 06:06:11.611693 pyg_nightly-2.4.0.dev20230612/torch_geometric/explain/algorithm/__init__.py
--rw-r--r--   0        0        0     4491 2023-06-12 06:06:11.611693 pyg_nightly-2.4.0.dev20230612/torch_geometric/explain/algorithm/attention_explainer.py
--rw-r--r--   0        0        0     6899 2023-06-12 06:06:11.611693 pyg_nightly-2.4.0.dev20230612/torch_geometric/explain/algorithm/base.py
--rw-r--r--   0        0        0    12489 2023-06-12 06:06:11.611693 pyg_nightly-2.4.0.dev20230612/torch_geometric/explain/algorithm/captum.py
--rw-r--r--   0        0        0     6530 2023-06-12 06:06:11.611693 pyg_nightly-2.4.0.dev20230612/torch_geometric/explain/algorithm/captum_explainer.py
--rw-r--r--   0        0        0     2867 2023-06-12 06:06:11.611693 pyg_nightly-2.4.0.dev20230612/torch_geometric/explain/algorithm/dummy_explainer.py
--rw-r--r--   0        0        0    11868 2023-06-12 06:06:11.611693 pyg_nightly-2.4.0.dev20230612/torch_geometric/explain/algorithm/gnn_explainer.py
--rw-r--r--   0        0        0    10370 2023-06-12 06:06:11.611693 pyg_nightly-2.4.0.dev20230612/torch_geometric/explain/algorithm/pg_explainer.py
--rw-r--r--   0        0        0     2308 2023-06-12 06:06:11.611693 pyg_nightly-2.4.0.dev20230612/torch_geometric/explain/algorithm/utils.py
--rw-r--r--   0        0        0     7834 2023-06-12 06:06:11.611693 pyg_nightly-2.4.0.dev20230612/torch_geometric/explain/config.py
--rw-r--r--   0        0        0    10375 2023-06-12 06:06:11.611693 pyg_nightly-2.4.0.dev20230612/torch_geometric/explain/explainer.py
--rw-r--r--   0        0        0    14842 2023-06-12 06:06:11.611693 pyg_nightly-2.4.0.dev20230612/torch_geometric/explain/explanation.py
--rw-r--r--   0        0        0      301 2023-06-12 06:06:11.611693 pyg_nightly-2.4.0.dev20230612/torch_geometric/explain/metric/__init__.py
--rw-r--r--   0        0        0     1888 2023-06-12 06:06:11.611693 pyg_nightly-2.4.0.dev20230612/torch_geometric/explain/metric/basic.py
--rw-r--r--   0        0        0     3063 2023-06-12 06:06:11.611693 pyg_nightly-2.4.0.dev20230612/torch_geometric/explain/metric/faithfulness.py
--rw-r--r--   0        0        0     6157 2023-06-12 06:06:11.611693 pyg_nightly-2.4.0.dev20230612/torch_geometric/explain/metric/fidelity.py
--rw-r--r--   0        0        0     2045 2023-06-12 06:06:11.611693 pyg_nightly-2.4.0.dev20230612/torch_geometric/graphgym/__init__.py
--rw-r--r--   0        0        0      510 2023-06-12 06:06:11.611693 pyg_nightly-2.4.0.dev20230612/torch_geometric/graphgym/benchmark.py
--rw-r--r--   0        0        0     2371 2023-06-12 06:06:11.611693 pyg_nightly-2.4.0.dev20230612/torch_geometric/graphgym/checkpoint.py
--rw-r--r--   0        0        0      738 2023-06-12 06:06:11.611693 pyg_nightly-2.4.0.dev20230612/torch_geometric/graphgym/cmd_args.py
--rw-r--r--   0        0        0    17221 2023-06-12 06:06:11.611693 pyg_nightly-2.4.0.dev20230612/torch_geometric/graphgym/config.py
--rw-r--r--   0        0        0    14575 2023-06-12 06:06:11.611693 pyg_nightly-2.4.0.dev20230612/torch_geometric/graphgym/config_store.py
--rw-r--r--   0        0        0      389 2023-06-12 06:06:11.611693 pyg_nightly-2.4.0.dev20230612/torch_geometric/graphgym/contrib/__init__.py
--rw-r--r--   0        0        0      221 2023-06-12 06:06:11.611693 pyg_nightly-2.4.0.dev20230612/torch_geometric/graphgym/contrib/act/__init__.py
--rw-r--r--   0        0        0      221 2023-06-12 06:06:11.611693 pyg_nightly-2.4.0.dev20230612/torch_geometric/graphgym/contrib/config/__init__.py
--rw-r--r--   0        0        0      221 2023-06-12 06:06:11.611693 pyg_nightly-2.4.0.dev20230612/torch_geometric/graphgym/contrib/encoder/__init__.py
--rw-r--r--   0        0        0      221 2023-06-12 06:06:11.611693 pyg_nightly-2.4.0.dev20230612/torch_geometric/graphgym/contrib/head/__init__.py
--rw-r--r--   0        0        0      221 2023-06-12 06:06:11.611693 pyg_nightly-2.4.0.dev20230612/torch_geometric/graphgym/contrib/layer/__init__.py
--rw-r--r--   0        0        0     8304 2023-06-12 06:06:11.611693 pyg_nightly-2.4.0.dev20230612/torch_geometric/graphgym/contrib/layer/generalconv.py
--rw-r--r--   0        0        0      221 2023-06-12 06:06:11.611693 pyg_nightly-2.4.0.dev20230612/torch_geometric/graphgym/contrib/loader/__init__.py
--rw-r--r--   0        0        0      221 2023-06-12 06:06:11.611693 pyg_nightly-2.4.0.dev20230612/torch_geometric/graphgym/contrib/loss/__init__.py
--rw-r--r--   0        0        0      221 2023-06-12 06:06:11.611693 pyg_nightly-2.4.0.dev20230612/torch_geometric/graphgym/contrib/network/__init__.py
--rw-r--r--   0        0        0      221 2023-06-12 06:06:11.611693 pyg_nightly-2.4.0.dev20230612/torch_geometric/graphgym/contrib/optimizer/__init__.py
--rw-r--r--   0        0        0      221 2023-06-12 06:06:11.611693 pyg_nightly-2.4.0.dev20230612/torch_geometric/graphgym/contrib/pooling/__init__.py
--rw-r--r--   0        0        0      221 2023-06-12 06:06:11.611693 pyg_nightly-2.4.0.dev20230612/torch_geometric/graphgym/contrib/stage/__init__.py
--rw-r--r--   0        0        0      221 2023-06-12 06:06:11.611693 pyg_nightly-2.4.0.dev20230612/torch_geometric/graphgym/contrib/train/__init__.py
--rw-r--r--   0        0        0      221 2023-06-12 06:06:11.611693 pyg_nightly-2.4.0.dev20230612/torch_geometric/graphgym/contrib/transform/__init__.py
--rw-r--r--   0        0        0      375 2023-06-12 06:06:11.611693 pyg_nightly-2.4.0.dev20230612/torch_geometric/graphgym/imports.py
--rw-r--r--   0        0        0      490 2023-06-12 06:06:11.611693 pyg_nightly-2.4.0.dev20230612/torch_geometric/graphgym/init.py
--rw-r--r--   0        0        0    11763 2023-06-12 06:06:11.611693 pyg_nightly-2.4.0.dev20230612/torch_geometric/graphgym/loader.py
--rw-r--r--   0        0        0    11329 2023-06-12 06:06:11.611693 pyg_nightly-2.4.0.dev20230612/torch_geometric/graphgym/logger.py
--rw-r--r--   0        0        0     1474 2023-06-12 06:06:11.611693 pyg_nightly-2.4.0.dev20230612/torch_geometric/graphgym/loss.py
--rw-r--r--   0        0        0     3110 2023-06-12 06:06:11.611693 pyg_nightly-2.4.0.dev20230612/torch_geometric/graphgym/model_builder.py
--rw-r--r--   0        0        0     1121 2023-06-12 06:06:11.615693 pyg_nightly-2.4.0.dev20230612/torch_geometric/graphgym/models/__init__.py
--rw-r--r--   0        0        0      822 2023-06-12 06:06:11.615693 pyg_nightly-2.4.0.dev20230612/torch_geometric/graphgym/models/act.py
--rw-r--r--   0        0        0     2546 2023-06-12 06:06:11.615693 pyg_nightly-2.4.0.dev20230612/torch_geometric/graphgym/models/encoder.py
--rw-r--r--   0        0        0     5133 2023-06-12 06:06:11.615693 pyg_nightly-2.4.0.dev20230612/torch_geometric/graphgym/models/gnn.py
--rw-r--r--   0        0        0     4434 2023-06-12 06:06:11.615693 pyg_nightly-2.4.0.dev20230612/torch_geometric/graphgym/models/head.py
--rw-r--r--   0        0        0    12486 2023-06-12 06:06:11.615693 pyg_nightly-2.4.0.dev20230612/torch_geometric/graphgym/models/layer.py
--rw-r--r--   0        0        0      288 2023-06-12 06:06:11.615693 pyg_nightly-2.4.0.dev20230612/torch_geometric/graphgym/models/pooling.py
--rw-r--r--   0        0        0     1391 2023-06-12 06:06:11.615693 pyg_nightly-2.4.0.dev20230612/torch_geometric/graphgym/models/transform.py
--rw-r--r--   0        0        0     2544 2023-06-12 06:06:11.615693 pyg_nightly-2.4.0.dev20230612/torch_geometric/graphgym/optim.py
--rw-r--r--   0        0        0     3944 2023-06-12 06:06:11.615693 pyg_nightly-2.4.0.dev20230612/torch_geometric/graphgym/register.py
--rw-r--r--   0        0        0     1887 2023-06-12 06:06:11.615693 pyg_nightly-2.4.0.dev20230612/torch_geometric/graphgym/train.py
--rw-r--r--   0        0        0        0 2023-06-12 06:06:11.615693 pyg_nightly-2.4.0.dev20230612/torch_geometric/graphgym/utils/LICENSE
--rw-r--r--   0        0        0      641 2023-06-12 06:06:11.615693 pyg_nightly-2.4.0.dev20230612/torch_geometric/graphgym/utils/__init__.py
--rw-r--r--   0        0        0     9513 2023-06-12 06:06:11.615693 pyg_nightly-2.4.0.dev20230612/torch_geometric/graphgym/utils/agg_runs.py
--rw-r--r--   0        0        0     3056 2023-06-12 06:06:11.615693 pyg_nightly-2.4.0.dev20230612/torch_geometric/graphgym/utils/comp_budget.py
--rw-r--r--   0        0        0     1352 2023-06-12 06:06:11.615693 pyg_nightly-2.4.0.dev20230612/torch_geometric/graphgym/utils/device.py
--rw-r--r--   0        0        0      690 2023-06-12 06:06:11.615693 pyg_nightly-2.4.0.dev20230612/torch_geometric/graphgym/utils/epoch.py
--rw-r--r--   0        0        0     2050 2023-06-12 06:06:11.615693 pyg_nightly-2.4.0.dev20230612/torch_geometric/graphgym/utils/io.py
--rw-r--r--   0        0        0      606 2023-06-12 06:06:11.615693 pyg_nightly-2.4.0.dev20230612/torch_geometric/graphgym/utils/plot.py
--rw-r--r--   0        0        0      198 2023-06-12 06:06:11.615693 pyg_nightly-2.4.0.dev20230612/torch_geometric/graphgym/utils/tools.py
--rw-r--r--   0        0        0      830 2023-06-12 06:06:11.615693 pyg_nightly-2.4.0.dev20230612/torch_geometric/home.py
--rw-r--r--   0        0        0      528 2023-06-12 06:06:11.615693 pyg_nightly-2.4.0.dev20230612/torch_geometric/io/__init__.py
--rw-r--r--   0        0        0     1148 2023-06-12 06:06:11.615693 pyg_nightly-2.4.0.dev20230612/torch_geometric/io/npz.py
--rw-r--r--   0        0        0      957 2023-06-12 06:06:11.615693 pyg_nightly-2.4.0.dev20230612/torch_geometric/io/obj.py
--rw-r--r--   0        0        0     2586 2023-06-12 06:06:11.615693 pyg_nightly-2.4.0.dev20230612/torch_geometric/io/off.py
--rw-r--r--   0        0        0     4243 2023-06-12 06:06:11.615693 pyg_nightly-2.4.0.dev20230612/torch_geometric/io/planetoid.py
--rw-r--r--   0        0        0      476 2023-06-12 06:06:11.615693 pyg_nightly-2.4.0.dev20230612/torch_geometric/io/ply.py
--rw-r--r--   0        0        0     1136 2023-06-12 06:06:11.615693 pyg_nightly-2.4.0.dev20230612/torch_geometric/io/sdf.py
--rw-r--r--   0        0        0     4733 2023-06-12 06:06:11.615693 pyg_nightly-2.4.0.dev20230612/torch_geometric/io/tu.py
--rw-r--r--   0        0        0      562 2023-06-12 06:06:11.615693 pyg_nightly-2.4.0.dev20230612/torch_geometric/io/txt_array.py
--rw-r--r--   0        0        0      768 2023-06-12 06:06:11.615693 pyg_nightly-2.4.0.dev20230612/torch_geometric/lazy_loader.py
--rw-r--r--   0        0        0     1675 2023-06-12 06:06:11.615693 pyg_nightly-2.4.0.dev20230612/torch_geometric/loader/__init__.py
--rw-r--r--   0        0        0     1433 2023-06-12 06:06:11.615693 pyg_nightly-2.4.0.dev20230612/torch_geometric/loader/base.py
--rw-r--r--   0        0        0    11594 2023-06-12 06:06:11.615693 pyg_nightly-2.4.0.dev20230612/torch_geometric/loader/cluster.py
--rw-r--r--   0        0        0     1449 2023-06-12 06:06:11.615693 pyg_nightly-2.4.0.dev20230612/torch_geometric/loader/data_list_loader.py
--rw-r--r--   0        0        0     3222 2023-06-12 06:06:11.615693 pyg_nightly-2.4.0.dev20230612/torch_geometric/loader/dataloader.py
--rw-r--r--   0        0        0     1683 2023-06-12 06:06:11.615693 pyg_nightly-2.4.0.dev20230612/torch_geometric/loader/dense_data_loader.py
--rw-r--r--   0        0        0     4285 2023-06-12 06:06:11.615693 pyg_nightly-2.4.0.dev20230612/torch_geometric/loader/dynamic_batch_sampler.py
--rw-r--r--   0        0        0     8448 2023-06-12 06:06:11.615693 pyg_nightly-2.4.0.dev20230612/torch_geometric/loader/graph_saint.py
--rw-r--r--   0        0        0     6012 2023-06-12 06:06:11.615693 pyg_nightly-2.4.0.dev20230612/torch_geometric/loader/hgt_loader.py
--rw-r--r--   0        0        0     3754 2023-06-12 06:06:11.615693 pyg_nightly-2.4.0.dev20230612/torch_geometric/loader/imbalanced_sampler.py
--rw-r--r--   0        0        0    14219 2023-06-12 06:06:11.615693 pyg_nightly-2.4.0.dev20230612/torch_geometric/loader/link_loader.py
--rw-r--r--   0        0        0    12587 2023-06-12 06:06:11.615693 pyg_nightly-2.4.0.dev20230612/torch_geometric/loader/link_neighbor_loader.py
--rw-r--r--   0        0        0     6317 2023-06-12 06:06:11.615693 pyg_nightly-2.4.0.dev20230612/torch_geometric/loader/mixin.py
--rw-r--r--   0        0        0    11382 2023-06-12 06:06:11.615693 pyg_nightly-2.4.0.dev20230612/torch_geometric/loader/neighbor_loader.py
--rw-r--r--   0        0        0     8513 2023-06-12 06:06:11.615693 pyg_nightly-2.4.0.dev20230612/torch_geometric/loader/neighbor_sampler.py
--rw-r--r--   0        0        0     9365 2023-06-12 06:06:11.615693 pyg_nightly-2.4.0.dev20230612/torch_geometric/loader/node_loader.py
--rw-r--r--   0        0        0     2141 2023-06-12 06:06:11.615693 pyg_nightly-2.4.0.dev20230612/torch_geometric/loader/prefetch.py
--rw-r--r--   0        0        0     2196 2023-06-12 06:06:11.615693 pyg_nightly-2.4.0.dev20230612/torch_geometric/loader/random_node_loader.py
--rw-r--r--   0        0        0     4173 2023-06-12 06:06:11.615693 pyg_nightly-2.4.0.dev20230612/torch_geometric/loader/shadow.py
--rw-r--r--   0        0        0     1319 2023-06-12 06:06:11.615693 pyg_nightly-2.4.0.dev20230612/torch_geometric/loader/temporal_dataloader.py
--rw-r--r--   0        0        0    12273 2023-06-12 06:06:11.615693 pyg_nightly-2.4.0.dev20230612/torch_geometric/loader/utils.py
--rw-r--r--   0        0        0     3518 2023-06-12 06:06:11.615693 pyg_nightly-2.4.0.dev20230612/torch_geometric/loader/zip_loader.py
--rw-r--r--   0        0        0      832 2023-06-12 06:06:11.615693 pyg_nightly-2.4.0.dev20230612/torch_geometric/logging.py
--rw-r--r--   0        0        0      847 2023-06-12 06:06:11.615693 pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/__init__.py
--rw-r--r--   0        0        0     1397 2023-06-12 06:06:11.615693 pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/aggr/__init__.py
--rw-r--r--   0        0        0     2395 2023-06-12 06:06:11.615693 pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/aggr/attention.py
--rw-r--r--   0        0        0     7449 2023-06-12 06:06:11.615693 pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/aggr/base.py
--rw-r--r--   0        0        0    11000 2023-06-12 06:06:11.615693 pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/aggr/basic.py
--rw-r--r--   0        0        0     2064 2023-06-12 06:06:11.615693 pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/aggr/deep_sets.py
--rw-r--r--   0        0        0     6456 2023-06-12 06:06:11.615693 pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/aggr/equilibrium.py
--rw-r--r--   0        0        0    12229 2023-06-12 06:06:11.615693 pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/aggr/fused.py
--rw-r--r--   0        0        0     3346 2023-06-12 06:06:11.615693 pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/aggr/gmt.py
--rw-r--r--   0        0        0     1747 2023-06-12 06:06:11.615693 pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/aggr/gru.py
--rw-r--r--   0        0        0     1767 2023-06-12 06:06:11.619693 pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/aggr/lstm.py
--rw-r--r--   0        0        0     1995 2023-06-12 06:06:11.619693 pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/aggr/mlp.py
--rw-r--r--   0        0        0     8170 2023-06-12 06:06:11.619693 pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/aggr/multi.py
--rw-r--r--   0        0        0     6174 2023-06-12 06:06:11.619693 pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/aggr/quantile.py
--rw-r--r--   0        0        0     4642 2023-06-12 06:06:11.619693 pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/aggr/scaler.py
--rw-r--r--   0        0        0     2517 2023-06-12 06:06:11.619693 pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/aggr/set2set.py
--rw-r--r--   0        0        0     3723 2023-06-12 06:06:11.619693 pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/aggr/set_transformer.py
--rw-r--r--   0        0        0     2061 2023-06-12 06:06:11.619693 pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/aggr/sort.py
--rw-r--r--   0        0        0     8322 2023-06-12 06:06:11.619693 pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/aggr/utils.py
--rw-r--r--   0        0        0       76 2023-06-12 06:06:11.619693 pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/attention/__init__.py
--rw-r--r--   0        0        0     7687 2023-06-12 06:06:11.619693 pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/attention/performer.py
--rw-r--r--   0        0        0     3360 2023-06-12 06:06:11.619693 pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/conv/__init__.py
--rw-r--r--   0        0        0     3088 2023-06-12 06:06:11.619693 pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/conv/agnn_conv.py
--rw-r--r--   0        0        0     4388 2023-06-12 06:06:11.619693 pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/conv/antisymmetric_conv.py
--rw-r--r--   0        0        0     6010 2023-06-12 06:06:11.619693 pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/conv/appnp.py
--rw-r--r--   0        0        0     6637 2023-06-12 06:06:11.619693 pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/conv/arma_conv.py
--rw-r--r--   0        0        0     4036 2023-06-12 06:06:11.619693 pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/conv/cg_conv.py
--rw-r--r--   0        0        0     6444 2023-06-12 06:06:11.619693 pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/conv/cheb_conv.py
--rw-r--r--   0        0        0     5303 2023-06-12 06:06:11.619693 pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/conv/cluster_gcn_conv.py
--rw-r--r--   0        0        0      251 2023-06-12 06:06:11.619693 pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/conv/cugraph/__init__.py
--rw-r--r--   0        0        0     8195 2023-06-12 06:06:11.619693 pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/conv/cugraph/base.py
--rw-r--r--   0        0        0     2849 2023-06-12 06:06:11.619693 pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/conv/cugraph/gat_conv.py
--rw-r--r--   0        0        0     4218 2023-06-12 06:06:11.619693 pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/conv/cugraph/rgcn_conv.py
--rw-r--r--   0        0        0     2802 2023-06-12 06:06:11.619693 pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/conv/cugraph/sage_conv.py
--rw-r--r--   0        0        0    12105 2023-06-12 06:06:11.619693 pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/conv/dna_conv.py
--rw-r--r--   0        0        0     5550 2023-06-12 06:06:11.619693 pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/conv/edge_conv.py
--rw-r--r--   0        0        0    10482 2023-06-12 06:06:11.619693 pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/conv/eg_conv.py
--rw-r--r--   0        0        0     7927 2023-06-12 06:06:11.619693 pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/conv/fa_conv.py
--rw-r--r--   0        0        0     4453 2023-06-12 06:06:11.619693 pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/conv/feast_conv.py
--rw-r--r--   0        0        0     6332 2023-06-12 06:06:11.619693 pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/conv/film_conv.py
--rw-r--r--   0        0        0     4242 2023-06-12 06:06:11.619693 pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/conv/fused_gat_conv.py
--rw-r--r--   0        0        0    13610 2023-06-12 06:06:11.619693 pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/conv/gat_conv.py
--rw-r--r--   0        0        0     3582 2023-06-12 06:06:11.619693 pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/conv/gated_graph_conv.py
--rw-r--r--   0        0        0    12423 2023-06-12 06:06:11.619693 pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/conv/gatv2_conv.py
--rw-r--r--   0        0        0     7022 2023-06-12 06:06:11.619693 pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/conv/gcn2_conv.py
--rw-r--r--   0        0        0     9333 2023-06-12 06:06:11.619693 pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/conv/gcn_conv.py
--rw-r--r--   0        0        0     9992 2023-06-12 06:06:11.619693 pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/conv/gen_conv.py
--rw-r--r--   0        0        0     7536 2023-06-12 06:06:11.619693 pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/conv/general_conv.py
--rw-r--r--   0        0        0     7444 2023-06-12 06:06:11.619693 pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/conv/gin_conv.py
--rw-r--r--   0        0        0     8320 2023-06-12 06:06:11.619693 pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/conv/gmm_conv.py
--rw-r--r--   0        0        0     6672 2023-06-12 06:06:11.619693 pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/conv/gps_conv.py
--rw-r--r--   0        0        0     3547 2023-06-12 06:06:11.623694 pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/conv/graph_conv.py
--rw-r--r--   0        0        0     5023 2023-06-12 06:06:11.623694 pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/conv/gravnet_conv.py
--rw-r--r--   0        0        0     7354 2023-06-12 06:06:11.623694 pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/conv/han_conv.py
--rw-r--r--   0        0        0     6063 2023-06-12 06:06:11.623694 pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/conv/heat_conv.py
--rw-r--r--   0        0        0     6470 2023-06-12 06:06:11.623694 pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/conv/hetero_conv.py
--rw-r--r--   0        0        0     9282 2023-06-12 06:06:11.623694 pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/conv/hgt_conv.py
--rw-r--r--   0        0        0     7580 2023-06-12 06:06:11.623694 pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/conv/hypergraph_conv.py
--rw-r--r--   0        0        0     3523 2023-06-12 06:06:11.623694 pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/conv/le_conv.py
--rw-r--r--   0        0        0     2418 2023-06-12 06:06:11.623694 pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/conv/lg_conv.py
--rw-r--r--   0        0        0    11524 2023-06-12 06:06:11.623694 pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/conv/message_passing.jinja
--rw-r--r--   0        0        0    39859 2023-06-12 06:06:11.623694 pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/conv/message_passing.py
--rw-r--r--   0        0        0     4321 2023-06-12 06:06:11.623694 pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/conv/mf_conv.py
--rw-r--r--   0        0        0     4743 2023-06-12 06:06:11.623694 pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/conv/nn_conv.py
--rw-r--r--   0        0        0     4928 2023-06-12 06:06:11.623694 pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/conv/pan_conv.py
--rw-r--r--   0        0        0     4916 2023-06-12 06:06:11.623694 pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/conv/pdn_conv.py
--rw-r--r--   0        0        0     8242 2023-06-12 06:06:11.623694 pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/conv/pna_conv.py
--rw-r--r--   0        0        0     4522 2023-06-12 06:06:11.623694 pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/conv/point_conv.py
--rw-r--r--   0        0        0     3288 2023-06-12 06:06:11.623694 pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/conv/point_gnn_conv.py
--rw-r--r--   0        0        0     5889 2023-06-12 06:06:11.623694 pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/conv/point_transformer_conv.py
--rw-r--r--   0        0        0     5422 2023-06-12 06:06:11.623694 pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/conv/ppf_conv.py
--rw-r--r--   0        0        0     4180 2023-06-12 06:06:11.623694 pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/conv/res_gated_graph_conv.py
--rw-r--r--   0        0        0    22785 2023-06-12 06:06:11.623694 pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/conv/rgat_conv.py
--rw-r--r--   0        0        0    14977 2023-06-12 06:06:11.623694 pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/conv/rgcn_conv.py
--rw-r--r--   0        0        0     5813 2023-06-12 06:06:11.623694 pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/conv/sage_conv.py
--rw-r--r--   0        0        0     4597 2023-06-12 06:06:11.623694 pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/conv/sg_conv.py
--rw-r--r--   0        0        0     6283 2023-06-12 06:06:11.623694 pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/conv/signed_conv.py
--rw-r--r--   0        0        0     3899 2023-06-12 06:06:11.623694 pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/conv/simple_conv.py
--rw-r--r--   0        0        0     6330 2023-06-12 06:06:11.623694 pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/conv/spline_conv.py
--rw-r--r--   0        0        0     5185 2023-06-12 06:06:11.623694 pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/conv/ssg_conv.py
--rw-r--r--   0        0        0    11980 2023-06-12 06:06:11.623694 pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/conv/supergat_conv.py
--rw-r--r--   0        0        0     4215 2023-06-12 06:06:11.623694 pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/conv/tag_conv.py
--rw-r--r--   0        0        0     9425 2023-06-12 06:06:11.623694 pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/conv/transformer_conv.py
--rw-r--r--   0        0        0      823 2023-06-12 06:06:11.623694 pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/conv/utils/__init__.py
--rw-r--r--   0        0        0     2692 2023-06-12 06:06:11.623694 pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/conv/utils/cheatsheet.py
--rw-r--r--   0        0        0      186 2023-06-12 06:06:11.623694 pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/conv/utils/helpers.py
--rw-r--r--   0        0        0     3259 2023-06-12 06:06:11.623694 pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/conv/utils/inspector.py
--rw-r--r--   0        0        0      679 2023-06-12 06:06:11.623694 pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/conv/utils/jit.py
--rw-r--r--   0        0        0     3859 2023-06-12 06:06:11.623694 pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/conv/utils/typing.py
--rw-r--r--   0        0        0     3103 2023-06-12 06:06:11.623694 pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/conv/wl_conv.py
--rw-r--r--   0        0        0     2349 2023-06-12 06:06:11.623694 pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/conv/wl_conv_continuous.py
--rw-r--r--   0        0        0     5955 2023-06-12 06:06:11.623694 pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/conv/x_conv.py
--rw-r--r--   0        0        0     3960 2023-06-12 06:06:11.623694 pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/data_parallel.py
--rw-r--r--   0        0        0      712 2023-06-12 06:06:11.623694 pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/dense/__init__.py
--rw-r--r--   0        0        0     4228 2023-06-12 06:06:11.623694 pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/dense/dense_gat_conv.py
--rw-r--r--   0        0        0     2989 2023-06-12 06:06:11.623694 pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/dense/dense_gcn_conv.py
--rw-r--r--   0        0        0     2357 2023-06-12 06:06:11.623694 pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/dense/dense_gin_conv.py
--rw-r--r--   0        0        0     2737 2023-06-12 06:06:11.623694 pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/dense/dense_graph_conv.py
--rw-r--r--   0        0        0     2658 2023-06-12 06:06:11.623694 pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/dense/dense_sage_conv.py
--rw-r--r--   0        0        0     3050 2023-06-12 06:06:11.623694 pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/dense/diff_pool.py
--rw-r--r--   0        0        0     5671 2023-06-12 06:06:11.623694 pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/dense/dmon_pool.py
--rw-r--r--   0        0        0    17141 2023-06-12 06:06:11.627694 pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/dense/linear.py
--rw-r--r--   0        0        0     4111 2023-06-12 06:06:11.627694 pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/dense/mincut_pool.py
--rw-r--r--   0        0        0     3125 2023-06-12 06:06:11.627694 pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/encoding.py
--rw-r--r--   0        0        0       92 2023-06-12 06:06:11.627694 pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/functional/__init__.py
--rw-r--r--   0        0        0     1549 2023-06-12 06:06:11.627694 pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/functional/bro.py
--rw-r--r--   0        0        0      863 2023-06-12 06:06:11.627694 pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/functional/gini.py
--rw-r--r--   0        0        0    15551 2023-06-12 06:06:11.627694 pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/fx.py
--rw-r--r--   0        0        0     1088 2023-06-12 06:06:11.627694 pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/glob.py
--rw-r--r--   0        0        0     2457 2023-06-12 06:06:11.627694 pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/inits.py
--rw-r--r--   0        0        0      241 2023-06-12 06:06:11.627694 pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/kge/__init__.py
--rw-r--r--   0        0        0     5739 2023-06-12 06:06:11.627694 pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/kge/base.py
--rw-r--r--   0        0        0     3234 2023-06-12 06:06:11.627694 pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/kge/complex.py
--rw-r--r--   0        0        0     2462 2023-06-12 06:06:11.627694 pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/kge/distmult.py
--rw-r--r--   0        0        0      771 2023-06-12 06:06:11.627694 pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/kge/loader.py
--rw-r--r--   0        0        0     3208 2023-06-12 06:06:11.627694 pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/kge/rotate.py
--rw-r--r--   0        0        0     3088 2023-06-12 06:06:11.627694 pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/kge/transe.py
--rw-r--r--   0        0        0     8937 2023-06-12 06:06:11.627694 pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/lr_scheduler.py
--rw-r--r--   0        0        0     9512 2023-06-12 06:06:11.627694 pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/model_hub.py
--rw-r--r--   0        0        0     1647 2023-06-12 06:06:11.627694 pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/models/__init__.py
--rw-r--r--   0        0        0     6591 2023-06-12 06:06:11.627694 pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/models/attentive_fp.py
--rw-r--r--   0        0        0    10656 2023-06-12 06:06:11.627694 pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/models/autoencoder.py
--rw-r--r--   0        0        0    27754 2023-06-12 06:06:11.627694 pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/models/basic_gnn.py
--rw-r--r--   0        0        0     4138 2023-06-12 06:06:11.627694 pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/models/captum.py
--rw-r--r--   0        0        0     6799 2023-06-12 06:06:11.627694 pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/models/correct_and_smooth.py
--rw-r--r--   0        0        0     3972 2023-06-12 06:06:11.627694 pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/models/deep_graph_infomax.py
--rw-r--r--   0        0        0     4223 2023-06-12 06:06:11.627694 pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/models/deepgcn.py
--rw-r--r--   0        0        0    34432 2023-06-12 06:06:11.627694 pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/models/dimenet.py
--rw-r--r--   0        0        0     4611 2023-06-12 06:06:11.627694 pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/models/dimenet_utils.py
--rw-r--r--   0        0        0     7859 2023-06-12 06:06:11.627694 pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/models/gnnff.py
--rw-r--r--   0        0        0     1667 2023-06-12 06:06:11.627694 pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/models/graph_mixer.py
--rw-r--r--   0        0        0     5381 2023-06-12 06:06:11.627694 pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/models/graph_unet.py
--rw-r--r--   0        0        0     3397 2023-06-12 06:06:11.627694 pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/models/jumping_knowledge.py
--rw-r--r--   0        0        0     3937 2023-06-12 06:06:11.627694 pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/models/label_prop.py
--rw-r--r--   0        0        0    11282 2023-06-12 06:06:11.627694 pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/models/lightgcn.py
--rw-r--r--   0        0        0     7901 2023-06-12 06:06:11.627694 pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/models/linkx.py
--rw-r--r--   0        0        0     2566 2023-06-12 06:06:11.627694 pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/models/mask_label.py
--rw-r--r--   0        0        0     6529 2023-06-12 06:06:11.627694 pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/models/meta.py
--rw-r--r--   0        0        0    10318 2023-06-12 06:06:11.627694 pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/models/metapath2vec.py
--rw-r--r--   0        0        0     8980 2023-06-12 06:06:11.627694 pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/models/mlp.py
--rw-r--r--   0        0        0     7641 2023-06-12 06:06:11.627694 pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/models/node2vec.py
--rw-r--r--   0        0        0     3257 2023-06-12 06:06:11.627694 pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/models/pmlp.py
--rw-r--r--   0        0        0     8979 2023-06-12 06:06:11.627694 pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/models/re_net.py
--rw-r--r--   0        0        0     5789 2023-06-12 06:06:11.627694 pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/models/rect.py
--rw-r--r--   0        0        0    11818 2023-06-12 06:06:11.627694 pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/models/rev_gnn.py
--rw-r--r--   0        0        0    16599 2023-06-12 06:06:11.627694 pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/models/schnet.py
--rw-r--r--   0        0        0     9840 2023-06-12 06:06:11.627694 pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/models/signed_gcn.py
--rw-r--r--   0        0        0    11590 2023-06-12 06:06:11.627694 pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/models/tgn.py
--rw-r--r--   0        0        0     1957 2023-06-12 06:06:11.627694 pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/module_dict.py
--rw-r--r--   0        0        0      638 2023-06-12 06:06:11.627694 pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/norm/__init__.py
--rw-r--r--   0        0        0     8258 2023-06-12 06:06:11.627694 pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/norm/batch_norm.py
--rw-r--r--   0        0        0     4706 2023-06-12 06:06:11.627694 pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/norm/diff_group_norm.py
--rw-r--r--   0        0        0     2715 2023-06-12 06:06:11.627694 pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/norm/graph_norm.py
--rw-r--r--   0        0        0     1492 2023-06-12 06:06:11.627694 pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/norm/graph_size_norm.py
--rw-r--r--   0        0        0     4670 2023-06-12 06:06:11.627694 pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/norm/instance_norm.py
--rw-r--r--   0        0        0     7806 2023-06-12 06:06:11.627694 pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/norm/layer_norm.py
--rw-r--r--   0        0        0     1311 2023-06-12 06:06:11.627694 pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/norm/mean_subtraction_norm.py
--rw-r--r--   0        0        0     1654 2023-06-12 06:06:11.631693 pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/norm/msg_norm.py
--rw-r--r--   0        0        0     2809 2023-06-12 06:06:11.631693 pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/norm/pair_norm.py
--rw-r--r--   0        0        0     1982 2023-06-12 06:06:11.631693 pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/parameter_dict.py
--rw-r--r--   0        0        0    13307 2023-06-12 06:06:11.631693 pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/pool/__init__.py
--rw-r--r--   0        0        0     3967 2023-06-12 06:06:11.631693 pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/pool/approx_knn.py
--rw-r--r--   0        0        0     6870 2023-06-12 06:06:11.631693 pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/pool/asap.py
--rw-r--r--   0        0        0     3966 2023-06-12 06:06:11.631693 pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/pool/avg_pool.py
--rw-r--r--   0        0        0       92 2023-06-12 06:06:11.631693 pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/pool/connect/__init__.py
--rw-r--r--   0        0        0     4001 2023-06-12 06:06:11.631693 pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/pool/connect/base.py
--rw-r--r--   0        0        0      273 2023-06-12 06:06:11.631693 pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/pool/consecutive.py
--rw-r--r--   0        0        0     1600 2023-06-12 06:06:11.631693 pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/pool/decimation.py
--rw-r--r--   0        0        0     8567 2023-06-12 06:06:11.631693 pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/pool/edge_pool.py
--rw-r--r--   0        0        0     3510 2023-06-12 06:06:11.631693 pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/pool/glob.py
--rw-r--r--   0        0        0     1292 2023-06-12 06:06:11.631693 pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/pool/graclus.py
--rw-r--r--   0        0        0     4262 2023-06-12 06:06:11.631693 pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/pool/max_pool.py
--rw-r--r--   0        0        0     5362 2023-06-12 06:06:11.631693 pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/pool/mem_pool.py
--rw-r--r--   0        0        0     4400 2023-06-12 06:06:11.631693 pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/pool/pan_pool.py
--rw-r--r--   0        0        0      631 2023-06-12 06:06:11.631693 pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/pool/pool.py
--rw-r--r--   0        0        0     5966 2023-06-12 06:06:11.631693 pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/pool/sag_pool.py
--rw-r--r--   0        0        0      135 2023-06-12 06:06:11.631693 pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/pool/select/__init__.py
--rw-r--r--   0        0        0     3208 2023-06-12 06:06:11.631693 pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/pool/select/base.py
--rw-r--r--   0        0        0     6262 2023-06-12 06:06:11.631693 pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/pool/select/topk.py
--rw-r--r--   0        0        0     5760 2023-06-12 06:06:11.631693 pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/pool/topk_pool.py
--rw-r--r--   0        0        0     2737 2023-06-12 06:06:11.631693 pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/pool/voxel_grid.py
--rw-r--r--   0        0        0      412 2023-06-12 06:06:11.631693 pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/reshape.py
--rw-r--r--   0        0        0     6155 2023-06-12 06:06:11.631693 pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/resolver.py
--rw-r--r--   0        0        0     1071 2023-06-12 06:06:11.631693 pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/sequential.jinja
--rw-r--r--   0        0        0     4577 2023-06-12 06:06:11.631693 pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/sequential.py
--rw-r--r--   0        0        0     5616 2023-06-12 06:06:11.631693 pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/summary.py
--rw-r--r--   0        0        0     1282 2023-06-12 06:06:11.631693 pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/to_fixed_size_transformer.py
--rw-r--r--   0        0        0     6486 2023-06-12 06:06:11.631693 pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/to_hetero_module.py
--rw-r--r--   0        0        0    18407 2023-06-12 06:06:11.631693 pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/to_hetero_transformer.py
--rw-r--r--   0        0        0    23103 2023-06-12 06:06:11.631693 pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/to_hetero_with_bases_transformer.py
--rw-r--r--   0        0        0      102 2023-06-12 06:06:11.631693 pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/unpool/__init__.py
--rw-r--r--   0        0        0     2586 2023-06-12 06:06:11.631693 pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/unpool/knn_interpolate.py
--rw-r--r--   0        0        0      803 2023-06-12 06:06:11.631693 pyg_nightly-2.4.0.dev20230612/torch_geometric/profile/__init__.py
--rw-r--r--   0        0        0     4363 2023-06-12 06:06:11.631693 pyg_nightly-2.4.0.dev20230612/torch_geometric/profile/benchmark.py
--rw-r--r--   0        0        0    10364 2023-06-12 06:06:11.631693 pyg_nightly-2.4.0.dev20230612/torch_geometric/profile/profile.py
--rw-r--r--   0        0        0    16665 2023-06-12 06:06:11.631693 pyg_nightly-2.4.0.dev20230612/torch_geometric/profile/profiler.py
--rw-r--r--   0        0        0     4563 2023-06-12 06:06:11.631693 pyg_nightly-2.4.0.dev20230612/torch_geometric/profile/utils.py
--rw-r--r--   0        0        0     1251 2023-06-12 06:06:11.631693 pyg_nightly-2.4.0.dev20230612/torch_geometric/resolver.py
--rw-r--r--   0        0        0      481 2023-06-12 06:06:11.631693 pyg_nightly-2.4.0.dev20230612/torch_geometric/sampler/__init__.py
--rw-r--r--   0        0        0    22762 2023-06-12 06:06:11.631693 pyg_nightly-2.4.0.dev20230612/torch_geometric/sampler/base.py
--rw-r--r--   0        0        0     2734 2023-06-12 06:06:11.631693 pyg_nightly-2.4.0.dev20230612/torch_geometric/sampler/hgt_sampler.py
--rw-r--r--   0        0        0    26480 2023-06-12 06:06:11.631693 pyg_nightly-2.4.0.dev20230612/torch_geometric/sampler/neighbor_sampler.py
--rw-r--r--   0        0        0     5252 2023-06-12 06:06:11.631693 pyg_nightly-2.4.0.dev20230612/torch_geometric/sampler/utils.py
--rw-r--r--   0        0        0      354 2023-06-12 06:06:11.631693 pyg_nightly-2.4.0.dev20230612/torch_geometric/seed.py
--rw-r--r--   0        0        0      710 2023-06-12 06:06:11.631693 pyg_nightly-2.4.0.dev20230612/torch_geometric/testing/__init__.py
--rw-r--r--   0        0        0     4368 2023-06-12 06:06:11.631693 pyg_nightly-2.4.0.dev20230612/torch_geometric/testing/asserts.py
--rw-r--r--   0        0        0     1933 2023-06-12 06:06:11.631693 pyg_nightly-2.4.0.dev20230612/torch_geometric/testing/data.py
--rw-r--r--   0        0        0     3842 2023-06-12 06:06:11.631693 pyg_nightly-2.4.0.dev20230612/torch_geometric/testing/decorators.py
--rw-r--r--   0        0        0     1855 2023-06-12 06:06:11.631693 pyg_nightly-2.4.0.dev20230612/torch_geometric/testing/feature_store.py
--rw-r--r--   0        0        0     1009 2023-06-12 06:06:11.631693 pyg_nightly-2.4.0.dev20230612/torch_geometric/testing/graph_store.py
--rw-r--r--   0        0        0     4136 2023-06-12 06:06:11.631693 pyg_nightly-2.4.0.dev20230612/torch_geometric/transforms/__init__.py
--rw-r--r--   0        0        0    13964 2023-06-12 06:06:11.631693 pyg_nightly-2.4.0.dev20230612/torch_geometric/transforms/add_metapaths.py
--rw-r--r--   0        0        0     4836 2023-06-12 06:06:11.631693 pyg_nightly-2.4.0.dev20230612/torch_geometric/transforms/add_positional_encoding.py
--rw-r--r--   0        0        0     2087 2023-06-12 06:06:11.631693 pyg_nightly-2.4.0.dev20230612/torch_geometric/transforms/add_remaining_self_loops.py
--rw-r--r--   0        0        0     2018 2023-06-12 06:06:11.631693 pyg_nightly-2.4.0.dev20230612/torch_geometric/transforms/add_self_loops.py
--rw-r--r--   0        0        0     1298 2023-06-12 06:06:11.631693 pyg_nightly-2.4.0.dev20230612/torch_geometric/transforms/base_transform.py
--rw-r--r--   0        0        0     1936 2023-06-12 06:06:11.635694 pyg_nightly-2.4.0.dev20230612/torch_geometric/transforms/cartesian.py
--rw-r--r--   0        0        0      640 2023-06-12 06:06:11.635694 pyg_nightly-2.4.0.dev20230612/torch_geometric/transforms/center.py
--rw-r--r--   0        0        0     1658 2023-06-12 06:06:11.635694 pyg_nightly-2.4.0.dev20230612/torch_geometric/transforms/compose.py
--rw-r--r--   0        0        0     1960 2023-06-12 06:06:11.635694 pyg_nightly-2.4.0.dev20230612/torch_geometric/transforms/constant.py
--rw-r--r--   0        0        0     1222 2023-06-12 06:06:11.635694 pyg_nightly-2.4.0.dev20230612/torch_geometric/transforms/delaunay.py
--rw-r--r--   0        0        0     1809 2023-06-12 06:06:11.635694 pyg_nightly-2.4.0.dev20230612/torch_geometric/transforms/distance.py
--rw-r--r--   0        0        0     1034 2023-06-12 06:06:11.635694 pyg_nightly-2.4.0.dev20230612/torch_geometric/transforms/face_to_edge.py
--rw-r--r--   0        0        0     2982 2023-06-12 06:06:11.635694 pyg_nightly-2.4.0.dev20230612/torch_geometric/transforms/feature_propagation.py
--rw-r--r--   0        0        0     2367 2023-06-12 06:06:11.635694 pyg_nightly-2.4.0.dev20230612/torch_geometric/transforms/fixed_points.py
--rw-r--r--   0        0        0     1397 2023-06-12 06:06:11.635694 pyg_nightly-2.4.0.dev20230612/torch_geometric/transforms/gcn_norm.py
--rw-r--r--   0        0        0    24215 2023-06-12 06:06:11.635694 pyg_nightly-2.4.0.dev20230612/torch_geometric/transforms/gdc.py
--rw-r--r--   0        0        0     1018 2023-06-12 06:06:11.635694 pyg_nightly-2.4.0.dev20230612/torch_geometric/transforms/generate_mesh_normals.py
--rw-r--r--   0        0        0     2511 2023-06-12 06:06:11.635694 pyg_nightly-2.4.0.dev20230612/torch_geometric/transforms/grid_sampling.py
--rw-r--r--   0        0        0     2543 2023-06-12 06:06:11.635694 pyg_nightly-2.4.0.dev20230612/torch_geometric/transforms/knn_graph.py
--rw-r--r--   0        0        0     2465 2023-06-12 06:06:11.635694 pyg_nightly-2.4.0.dev20230612/torch_geometric/transforms/laplacian_lambda_max.py
--rw-r--r--   0        0        0     2000 2023-06-12 06:06:11.635694 pyg_nightly-2.4.0.dev20230612/torch_geometric/transforms/largest_connected_components.py
--rw-r--r--   0        0        0     3723 2023-06-12 06:06:11.635694 pyg_nightly-2.4.0.dev20230612/torch_geometric/transforms/line_graph.py
--rw-r--r--   0        0        0     1996 2023-06-12 06:06:11.635694 pyg_nightly-2.4.0.dev20230612/torch_geometric/transforms/linear_transformation.py
--rw-r--r--   0        0        0     1698 2023-06-12 06:06:11.635694 pyg_nightly-2.4.0.dev20230612/torch_geometric/transforms/local_cartesian.py
--rw-r--r--   0        0        0     1404 2023-06-12 06:06:11.635694 pyg_nightly-2.4.0.dev20230612/torch_geometric/transforms/local_degree_profile.py
--rw-r--r--   0        0        0     4598 2023-06-12 06:06:11.635694 pyg_nightly-2.4.0.dev20230612/torch_geometric/transforms/mask.py
--rw-r--r--   0        0        0     6091 2023-06-12 06:06:11.635694 pyg_nightly-2.4.0.dev20230612/torch_geometric/transforms/node_property_split.py
--rw-r--r--   0        0        0     1028 2023-06-12 06:06:11.635694 pyg_nightly-2.4.0.dev20230612/torch_geometric/transforms/normalize_features.py
--rw-r--r--   0        0        0     1738 2023-06-12 06:06:11.635694 pyg_nightly-2.4.0.dev20230612/torch_geometric/transforms/normalize_rotation.py
--rw-r--r--   0        0        0      620 2023-06-12 06:06:11.635694 pyg_nightly-2.4.0.dev20230612/torch_geometric/transforms/normalize_scale.py
--rw-r--r--   0        0        0     1533 2023-06-12 06:06:11.635694 pyg_nightly-2.4.0.dev20230612/torch_geometric/transforms/one_hot_degree.py
--rw-r--r--   0        0        0    21975 2023-06-12 06:06:11.635694 pyg_nightly-2.4.0.dev20230612/torch_geometric/transforms/pad.py
--rw-r--r--   0        0        0     1793 2023-06-12 06:06:11.635694 pyg_nightly-2.4.0.dev20230612/torch_geometric/transforms/point_pair_features.py
--rw-r--r--   0        0        0     2126 2023-06-12 06:06:11.635694 pyg_nightly-2.4.0.dev20230612/torch_geometric/transforms/polar.py
--rw-r--r--   0        0        0     2050 2023-06-12 06:06:11.635694 pyg_nightly-2.4.0.dev20230612/torch_geometric/transforms/radius_graph.py
--rw-r--r--   0        0        0      988 2023-06-12 06:06:11.635694 pyg_nightly-2.4.0.dev20230612/torch_geometric/transforms/random_flip.py
--rw-r--r--   0        0        0     1510 2023-06-12 06:06:11.635694 pyg_nightly-2.4.0.dev20230612/torch_geometric/transforms/random_jitter.py
--rw-r--r--   0        0        0    14297 2023-06-12 06:06:11.635694 pyg_nightly-2.4.0.dev20230612/torch_geometric/transforms/random_link_split.py
--rw-r--r--   0        0        0     5768 2023-06-12 06:06:11.635694 pyg_nightly-2.4.0.dev20230612/torch_geometric/transforms/random_node_split.py
--rw-r--r--   0        0        0     1903 2023-06-12 06:06:11.635694 pyg_nightly-2.4.0.dev20230612/torch_geometric/transforms/random_rotate.py
--rw-r--r--   0        0        0     1215 2023-06-12 06:06:11.635694 pyg_nightly-2.4.0.dev20230612/torch_geometric/transforms/random_scale.py
--rw-r--r--   0        0        0     1319 2023-06-12 06:06:11.635694 pyg_nightly-2.4.0.dev20230612/torch_geometric/transforms/random_shear.py
--rw-r--r--   0        0        0     1805 2023-06-12 06:06:11.635694 pyg_nightly-2.4.0.dev20230612/torch_geometric/transforms/remove_duplicated_edges.py
--rw-r--r--   0        0        0     2283 2023-06-12 06:06:11.635694 pyg_nightly-2.4.0.dev20230612/torch_geometric/transforms/remove_isolated_nodes.py
--rw-r--r--   0        0        0      959 2023-06-12 06:06:11.635694 pyg_nightly-2.4.0.dev20230612/torch_geometric/transforms/remove_training_classes.py
--rw-r--r--   0        0        0     6111 2023-06-12 06:06:11.635694 pyg_nightly-2.4.0.dev20230612/torch_geometric/transforms/rooted_subgraph.py
--rw-r--r--   0        0        0     2140 2023-06-12 06:06:11.635694 pyg_nightly-2.4.0.dev20230612/torch_geometric/transforms/sample_points.py
--rw-r--r--   0        0        0     2128 2023-06-12 06:06:11.635694 pyg_nightly-2.4.0.dev20230612/torch_geometric/transforms/sign.py
--rw-r--r--   0        0        0     2241 2023-06-12 06:06:11.635694 pyg_nightly-2.4.0.dev20230612/torch_geometric/transforms/spherical.py
--rw-r--r--   0        0        0     1002 2023-06-12 06:06:11.635694 pyg_nightly-2.4.0.dev20230612/torch_geometric/transforms/svd_feature_reduction.py
--rw-r--r--   0        0        0     1607 2023-06-12 06:06:11.635694 pyg_nightly-2.4.0.dev20230612/torch_geometric/transforms/target_indegree.py
--rw-r--r--   0        0        0     2327 2023-06-12 06:06:11.635694 pyg_nightly-2.4.0.dev20230612/torch_geometric/transforms/to_dense.py
--rw-r--r--   0        0        0     1455 2023-06-12 06:06:11.635694 pyg_nightly-2.4.0.dev20230612/torch_geometric/transforms/to_device.py
--rw-r--r--   0        0        0     5353 2023-06-12 06:06:11.635694 pyg_nightly-2.4.0.dev20230612/torch_geometric/transforms/to_sparse_tensor.py
--rw-r--r--   0        0        0     2621 2023-06-12 06:06:11.635694 pyg_nightly-2.4.0.dev20230612/torch_geometric/transforms/to_superpixels.py
--rw-r--r--   0        0        0     2972 2023-06-12 06:06:11.635694 pyg_nightly-2.4.0.dev20230612/torch_geometric/transforms/to_undirected.py
--rw-r--r--   0        0        0     1214 2023-06-12 06:06:11.635694 pyg_nightly-2.4.0.dev20230612/torch_geometric/transforms/two_hop.py
--rw-r--r--   0        0        0     2783 2023-06-12 06:06:11.635694 pyg_nightly-2.4.0.dev20230612/torch_geometric/transforms/virtual_node.py
--rw-r--r--   0        0        0     9575 2023-06-12 06:06:11.635694 pyg_nightly-2.4.0.dev20230612/torch_geometric/typing.py
--rw-r--r--   0        0        0     4549 2023-06-12 06:06:11.635694 pyg_nightly-2.4.0.dev20230612/torch_geometric/utils/__init__.py
--rw-r--r--   0        0        0     2347 2023-06-12 06:06:11.635694 pyg_nightly-2.4.0.dev20230612/torch_geometric/utils/assortativity.py
--rw-r--r--   0        0        0     9080 2023-06-12 06:06:11.635694 pyg_nightly-2.4.0.dev20230612/torch_geometric/utils/augmentation.py
--rw-r--r--   0        0        0     5037 2023-06-12 06:06:11.635694 pyg_nightly-2.4.0.dev20230612/torch_geometric/utils/coalesce.py
--rw-r--r--   0        0        0    19630 2023-06-12 06:06:11.635694 pyg_nightly-2.4.0.dev20230612/torch_geometric/utils/convert.py
--rw-r--r--   0        0        0     2313 2023-06-12 06:06:11.635694 pyg_nightly-2.4.0.dev20230612/torch_geometric/utils/cross_entropy.py
--rw-r--r--   0        0        0     1018 2023-06-12 06:06:11.635694 pyg_nightly-2.4.0.dev20230612/torch_geometric/utils/degree.py
--rw-r--r--   0        0        0    11323 2023-06-12 06:06:11.635694 pyg_nightly-2.4.0.dev20230612/torch_geometric/utils/dropout.py
--rw-r--r--   0        0        0     1657 2023-06-12 06:06:11.635694 pyg_nightly-2.4.0.dev20230612/torch_geometric/utils/embedding.py
--rw-r--r--   0        0        0     4042 2023-06-12 06:06:11.635694 pyg_nightly-2.4.0.dev20230612/torch_geometric/utils/geodesic.py
--rw-r--r--   0        0        0     3755 2023-06-12 06:06:11.635694 pyg_nightly-2.4.0.dev20230612/torch_geometric/utils/get_laplacian.py
--rw-r--r--   0        0        0     4423 2023-06-12 06:06:11.635694 pyg_nightly-2.4.0.dev20230612/torch_geometric/utils/get_mesh_laplacian.py
--rw-r--r--   0        0        0     2536 2023-06-12 06:06:11.635694 pyg_nightly-2.4.0.dev20230612/torch_geometric/utils/grid.py
--rw-r--r--   0        0        0     9798 2023-06-12 06:06:11.635694 pyg_nightly-2.4.0.dev20230612/torch_geometric/utils/hetero.py
--rw-r--r--   0        0        0     4818 2023-06-12 06:06:11.635694 pyg_nightly-2.4.0.dev20230612/torch_geometric/utils/homophily.py
--rw-r--r--   0        0        0     3574 2023-06-12 06:06:11.635694 pyg_nightly-2.4.0.dev20230612/torch_geometric/utils/isolated.py
--rw-r--r--   0        0        0    15855 2023-06-12 06:06:11.635694 pyg_nightly-2.4.0.dev20230612/torch_geometric/utils/loop.py
--rw-r--r--   0        0        0     5200 2023-06-12 06:06:11.639694 pyg_nightly-2.4.0.dev20230612/torch_geometric/utils/map.py
--rw-r--r--   0        0        0     1884 2023-06-12 06:06:11.639694 pyg_nightly-2.4.0.dev20230612/torch_geometric/utils/mask.py
--rw-r--r--   0        0        0      608 2023-06-12 06:06:11.639694 pyg_nightly-2.4.0.dev20230612/torch_geometric/utils/mixin.py
--rw-r--r--   0        0        0    14643 2023-06-12 06:06:11.639694 pyg_nightly-2.4.0.dev20230612/torch_geometric/utils/negative_sampling.py
--rw-r--r--   0        0        0     3344 2023-06-12 06:06:11.639694 pyg_nightly-2.4.0.dev20230612/torch_geometric/utils/nested.py
--rw-r--r--   0        0        0     1169 2023-06-12 06:06:11.639694 pyg_nightly-2.4.0.dev20230612/torch_geometric/utils/normalized_cut.py
--rw-r--r--   0        0        0     1917 2023-06-12 06:06:11.639694 pyg_nightly-2.4.0.dev20230612/torch_geometric/utils/num_nodes.py
--rw-r--r--   0        0        0     1404 2023-06-12 06:06:11.639694 pyg_nightly-2.4.0.dev20230612/torch_geometric/utils/one_hot.py
--rw-r--r--   0        0        0     5154 2023-06-12 06:06:11.639694 pyg_nightly-2.4.0.dev20230612/torch_geometric/utils/random.py
--rw-r--r--   0        0        0      815 2023-06-12 06:06:11.639694 pyg_nightly-2.4.0.dev20230612/torch_geometric/utils/repeat.py
--rw-r--r--   0        0        0     8329 2023-06-12 06:06:11.639694 pyg_nightly-2.4.0.dev20230612/torch_geometric/utils/scatter.py
--rw-r--r--   0        0        0     1110 2023-06-12 06:06:11.639694 pyg_nightly-2.4.0.dev20230612/torch_geometric/utils/segment.py
--rw-r--r--   0        0        0     2149 2023-06-12 06:06:11.639694 pyg_nightly-2.4.0.dev20230612/torch_geometric/utils/select.py
--rw-r--r--   0        0        0     6016 2023-06-12 06:06:11.639694 pyg_nightly-2.4.0.dev20230612/torch_geometric/utils/smiles.py
--rw-r--r--   0        0        0     2718 2023-06-12 06:06:11.639694 pyg_nightly-2.4.0.dev20230612/torch_geometric/utils/softmax.py
--rw-r--r--   0        0        0     1017 2023-06-12 06:06:11.639694 pyg_nightly-2.4.0.dev20230612/torch_geometric/utils/sort.py
--rw-r--r--   0        0        0     3066 2023-06-12 06:06:11.639694 pyg_nightly-2.4.0.dev20230612/torch_geometric/utils/sort_edge_index.py
--rw-r--r--   0        0        0    14860 2023-06-12 06:06:11.639694 pyg_nightly-2.4.0.dev20230612/torch_geometric/utils/sparse.py
--rw-r--r--   0        0        0     5678 2023-06-12 06:06:11.639694 pyg_nightly-2.4.0.dev20230612/torch_geometric/utils/spmm.py
--rw-r--r--   0        0        0    12370 2023-06-12 06:06:11.639694 pyg_nightly-2.4.0.dev20230612/torch_geometric/utils/subgraph.py
--rw-r--r--   0        0        0     3439 2023-06-12 06:06:11.639694 pyg_nightly-2.4.0.dev20230612/torch_geometric/utils/to_dense_adj.py
--rw-r--r--   0        0        0     4628 2023-06-12 06:06:11.639694 pyg_nightly-2.4.0.dev20230612/torch_geometric/utils/to_dense_batch.py
--rw-r--r--   0        0        0     3489 2023-06-12 06:06:11.639694 pyg_nightly-2.4.0.dev20230612/torch_geometric/utils/train_test_split_edges.py
--rw-r--r--   0        0        0     4867 2023-06-12 06:06:11.639694 pyg_nightly-2.4.0.dev20230612/torch_geometric/utils/tree_decomposition.py
--rw-r--r--   0        0        0     6730 2023-06-12 06:06:11.639694 pyg_nightly-2.4.0.dev20230612/torch_geometric/utils/trim_to_layer.py
--rw-r--r--   0        0        0     2125 2023-06-12 06:06:11.639694 pyg_nightly-2.4.0.dev20230612/torch_geometric/utils/unbatch.py
--rw-r--r--   0        0        0     5770 2023-06-12 06:06:11.639694 pyg_nightly-2.4.0.dev20230612/torch_geometric/utils/undirected.py
--rw-r--r--   0        0        0      123 2023-06-12 06:06:11.639694 pyg_nightly-2.4.0.dev20230612/torch_geometric/visualization/__init__.py
--rw-r--r--   0        0        0     4149 2023-06-12 06:06:11.643694 pyg_nightly-2.4.0.dev20230612/torch_geometric/visualization/graph.py
--rw-r--r--   0        0        0      388 2023-06-12 06:06:11.643694 pyg_nightly-2.4.0.dev20230612/torch_geometric/visualization/influence.py
--rw-r--r--   0        0        0    63943 1970-01-01 00:00:00.000000 pyg_nightly-2.4.0.dev20230612/PKG-INFO
+-rw-r--r--   0        0        0    60889 2023-06-13 06:05:51.762066 pyg_nightly-2.4.0.dev20230613/README.md
+-rw-r--r--   0        0        0     4092 2023-06-13 06:05:52.326109 pyg_nightly-2.4.0.dev20230613/pyproject.toml
+-rw-r--r--   0        0        0     1055 2023-06-13 06:05:52.322108 pyg_nightly-2.4.0.dev20230613/torch_geometric/__init__.py
+-rw-r--r--   0        0        0     3392 2023-06-13 06:05:51.806069 pyg_nightly-2.4.0.dev20230613/torch_geometric/compile.py
+-rw-r--r--   0        0        0      352 2023-06-13 06:05:51.806069 pyg_nightly-2.4.0.dev20230613/torch_geometric/contrib/__init__.py
+-rw-r--r--   0        0        0       23 2023-06-13 06:05:51.806069 pyg_nightly-2.4.0.dev20230613/torch_geometric/contrib/datasets/__init__.py
+-rw-r--r--   0        0        0      163 2023-06-13 06:05:51.806069 pyg_nightly-2.4.0.dev20230613/torch_geometric/contrib/explain/__init__.py
+-rw-r--r--   0        0        0    22723 2023-06-13 06:05:51.806069 pyg_nightly-2.4.0.dev20230613/torch_geometric/contrib/explain/graphmask_explainer.py
+-rw-r--r--   0        0        0    16627 2023-06-13 06:05:51.806069 pyg_nightly-2.4.0.dev20230613/torch_geometric/contrib/explain/pgm_explainer.py
+-rw-r--r--   0        0        0       72 2023-06-13 06:05:51.806069 pyg_nightly-2.4.0.dev20230613/torch_geometric/contrib/nn/__init__.py
+-rw-r--r--   0        0        0       23 2023-06-13 06:05:51.806069 pyg_nightly-2.4.0.dev20230613/torch_geometric/contrib/nn/conv/__init__.py
+-rw-r--r--   0        0        0      113 2023-06-13 06:05:51.806069 pyg_nightly-2.4.0.dev20230613/torch_geometric/contrib/nn/models/__init__.py
+-rw-r--r--   0        0        0    33261 2023-06-13 06:05:51.806069 pyg_nightly-2.4.0.dev20230613/torch_geometric/contrib/nn/models/rbcd_attack.py
+-rw-r--r--   0        0        0       23 2023-06-13 06:05:51.806069 pyg_nightly-2.4.0.dev20230613/torch_geometric/contrib/transforms/__init__.py
+-rw-r--r--   0        0        0     3383 2023-06-13 06:05:51.806069 pyg_nightly-2.4.0.dev20230613/torch_geometric/data/__init__.py
+-rw-r--r--   0        0        0     7428 2023-06-13 06:05:51.806069 pyg_nightly-2.4.0.dev20230613/torch_geometric/data/batch.py
+-rw-r--r--   0        0        0    10658 2023-06-13 06:05:51.806069 pyg_nightly-2.4.0.dev20230613/torch_geometric/data/collate.py
+-rw-r--r--   0        0        0    37497 2023-06-13 06:05:51.806069 pyg_nightly-2.4.0.dev20230613/torch_geometric/data/data.py
+-rw-r--r--   0        0        0     2922 2023-06-13 06:05:51.806069 pyg_nightly-2.4.0.dev20230613/torch_geometric/data/datapipes.py
+-rw-r--r--   0        0        0    15051 2023-06-13 06:05:51.806069 pyg_nightly-2.4.0.dev20230613/torch_geometric/data/dataset.py
+-rw-r--r--   0        0        0     1359 2023-06-13 06:05:51.806069 pyg_nightly-2.4.0.dev20230613/torch_geometric/data/download.py
+-rw-r--r--   0        0        0     2252 2023-06-13 06:05:51.806069 pyg_nightly-2.4.0.dev20230613/torch_geometric/data/extract.py
+-rw-r--r--   0        0        0    21075 2023-06-13 06:05:51.806069 pyg_nightly-2.4.0.dev20230613/torch_geometric/data/feature_store.py
+-rw-r--r--   0        0        0    13495 2023-06-13 06:05:51.806069 pyg_nightly-2.4.0.dev20230613/torch_geometric/data/graph_store.py
+-rw-r--r--   0        0        0    44329 2023-06-13 06:05:51.806069 pyg_nightly-2.4.0.dev20230613/torch_geometric/data/hetero_data.py
+-rw-r--r--   0        0        0     8072 2023-06-13 06:05:51.806069 pyg_nightly-2.4.0.dev20230613/torch_geometric/data/in_memory_dataset.py
+-rw-r--r--   0        0        0      178 2023-06-13 06:05:51.806069 pyg_nightly-2.4.0.dev20230613/torch_geometric/data/lightning/__init__.py
+-rw-r--r--   0        0        0    28490 2023-06-13 06:05:51.806069 pyg_nightly-2.4.0.dev20230613/torch_geometric/data/lightning/datamodule.py
+-rw-r--r--   0        0        0      338 2023-06-13 06:05:51.806069 pyg_nightly-2.4.0.dev20230613/torch_geometric/data/makedirs.py
+-rw-r--r--   0        0        0     3962 2023-06-13 06:05:51.806069 pyg_nightly-2.4.0.dev20230613/torch_geometric/data/remote_backend_utils.py
+-rw-r--r--   0        0        0     4360 2023-06-13 06:05:51.806069 pyg_nightly-2.4.0.dev20230613/torch_geometric/data/separate.py
+-rw-r--r--   0        0        0    25245 2023-06-13 06:05:51.806069 pyg_nightly-2.4.0.dev20230613/torch_geometric/data/storage.py
+-rw-r--r--   0        0        0     5219 2023-06-13 06:05:51.806069 pyg_nightly-2.4.0.dev20230613/torch_geometric/data/summary.py
+-rw-r--r--   0        0        0     9354 2023-06-13 06:05:51.806069 pyg_nightly-2.4.0.dev20230613/torch_geometric/data/temporal.py
+-rw-r--r--   0        0        0     1038 2023-06-13 06:05:51.806069 pyg_nightly-2.4.0.dev20230613/torch_geometric/data/view.py
+-rw-r--r--   0        0        0     5300 2023-06-13 06:05:51.806069 pyg_nightly-2.4.0.dev20230613/torch_geometric/datasets/__init__.py
+-rw-r--r--   0        0        0     4220 2023-06-13 06:05:51.806069 pyg_nightly-2.4.0.dev20230613/torch_geometric/datasets/actor.py
+-rw-r--r--   0        0        0     5584 2023-06-13 06:05:51.806069 pyg_nightly-2.4.0.dev20230613/torch_geometric/datasets/airfrans.py
+-rw-r--r--   0        0        0     3711 2023-06-13 06:05:51.806069 pyg_nightly-2.4.0.dev20230613/torch_geometric/datasets/airports.py
+-rw-r--r--   0        0        0     3050 2023-06-13 06:05:51.806069 pyg_nightly-2.4.0.dev20230613/torch_geometric/datasets/amazon.py
+-rw-r--r--   0        0        0     3109 2023-06-13 06:05:51.806069 pyg_nightly-2.4.0.dev20230613/torch_geometric/datasets/amazon_book.py
+-rw-r--r--   0        0        0     4099 2023-06-13 06:05:51.806069 pyg_nightly-2.4.0.dev20230613/torch_geometric/datasets/amazon_products.py
+-rw-r--r--   0        0        0     4942 2023-06-13 06:05:51.806069 pyg_nightly-2.4.0.dev20230613/torch_geometric/datasets/aminer.py
+-rw-r--r--   0        0        0     5266 2023-06-13 06:05:51.806069 pyg_nightly-2.4.0.dev20230613/torch_geometric/datasets/aqsol.py
+-rw-r--r--   0        0        0     5735 2023-06-13 06:05:51.806069 pyg_nightly-2.4.0.dev20230613/torch_geometric/datasets/attributed_graph_dataset.py
+-rw-r--r--   0        0        0     4063 2023-06-13 06:05:51.806069 pyg_nightly-2.4.0.dev20230613/torch_geometric/datasets/ba2motif_dataset.py
+-rw-r--r--   0        0        0     3518 2023-06-13 06:05:51.810070 pyg_nightly-2.4.0.dev20230613/torch_geometric/datasets/ba_multi_shapes.py
+-rw-r--r--   0        0        0     3824 2023-06-13 06:05:51.810070 pyg_nightly-2.4.0.dev20230613/torch_geometric/datasets/ba_shapes.py
+-rw-r--r--   0        0        0     4137 2023-06-13 06:05:51.810070 pyg_nightly-2.4.0.dev20230613/torch_geometric/datasets/bitcoin_otc.py
+-rw-r--r--   0        0        0     4205 2023-06-13 06:05:51.810070 pyg_nightly-2.4.0.dev20230613/torch_geometric/datasets/citation_full.py
+-rw-r--r--   0        0        0     3009 2023-06-13 06:05:51.810070 pyg_nightly-2.4.0.dev20230613/torch_geometric/datasets/coauthor.py
+-rw-r--r--   0        0        0     4564 2023-06-13 06:05:51.810070 pyg_nightly-2.4.0.dev20230613/torch_geometric/datasets/coma.py
+-rw-r--r--   0        0        0     5192 2023-06-13 06:05:51.810070 pyg_nightly-2.4.0.dev20230613/torch_geometric/datasets/dblp.py
+-rw-r--r--   0        0        0     5608 2023-06-13 06:05:51.810070 pyg_nightly-2.4.0.dev20230613/torch_geometric/datasets/dbp15k.py
+-rw-r--r--   0        0        0     2308 2023-06-13 06:05:51.810070 pyg_nightly-2.4.0.dev20230613/torch_geometric/datasets/deezer_europe.py
+-rw-r--r--   0        0        0     3862 2023-06-13 06:05:51.810070 pyg_nightly-2.4.0.dev20230613/torch_geometric/datasets/dgraph.py
+-rw-r--r--   0        0        0     5865 2023-06-13 06:05:51.810070 pyg_nightly-2.4.0.dev20230613/torch_geometric/datasets/dynamic_faust.py
+-rw-r--r--   0        0        0     4498 2023-06-13 06:05:51.810070 pyg_nightly-2.4.0.dev20230613/torch_geometric/datasets/elliptic.py
+-rw-r--r--   0        0        0     2990 2023-06-13 06:05:51.810070 pyg_nightly-2.4.0.dev20230613/torch_geometric/datasets/elliptic_temporal.py
+-rw-r--r--   0        0        0     2631 2023-06-13 06:05:51.810070 pyg_nightly-2.4.0.dev20230613/torch_geometric/datasets/email_eu_core.py
+-rw-r--r--   0        0        0     7001 2023-06-13 06:05:51.810070 pyg_nightly-2.4.0.dev20230613/torch_geometric/datasets/entities.py
+-rw-r--r--   0        0        0     5817 2023-06-13 06:05:51.810070 pyg_nightly-2.4.0.dev20230613/torch_geometric/datasets/explainer_dataset.py
+-rw-r--r--   0        0        0     2228 2023-06-13 06:05:51.810070 pyg_nightly-2.4.0.dev20230613/torch_geometric/datasets/facebook.py
+-rw-r--r--   0        0        0    10215 2023-06-13 06:05:51.810070 pyg_nightly-2.4.0.dev20230613/torch_geometric/datasets/fake.py
+-rw-r--r--   0        0        0     3924 2023-06-13 06:05:51.810070 pyg_nightly-2.4.0.dev20230613/torch_geometric/datasets/faust.py
+-rw-r--r--   0        0        0     4099 2023-06-13 06:05:51.810070 pyg_nightly-2.4.0.dev20230613/torch_geometric/datasets/flickr.py
+-rw-r--r--   0        0        0     3815 2023-06-13 06:05:51.810070 pyg_nightly-2.4.0.dev20230613/torch_geometric/datasets/freebase.py
+-rw-r--r--   0        0        0     3416 2023-06-13 06:05:51.810070 pyg_nightly-2.4.0.dev20230613/torch_geometric/datasets/gdelt.py
+-rw-r--r--   0        0        0     2967 2023-06-13 06:05:51.810070 pyg_nightly-2.4.0.dev20230613/torch_geometric/datasets/gdelt_lite.py
+-rw-r--r--   0        0        0     9261 2023-06-13 06:05:51.810070 pyg_nightly-2.4.0.dev20230613/torch_geometric/datasets/ged_dataset.py
+-rw-r--r--   0        0        0     2626 2023-06-13 06:05:51.810070 pyg_nightly-2.4.0.dev20230613/torch_geometric/datasets/gemsec.py
+-rw-r--r--   0        0        0     3954 2023-06-13 06:05:51.810070 pyg_nightly-2.4.0.dev20230613/torch_geometric/datasets/geometry.py
+-rw-r--r--   0        0        0     2484 2023-06-13 06:05:51.810070 pyg_nightly-2.4.0.dev20230613/torch_geometric/datasets/github.py
+-rw-r--r--   0        0        0     6762 2023-06-13 06:05:51.810070 pyg_nightly-2.4.0.dev20230613/torch_geometric/datasets/gnn_benchmark_dataset.py
+-rw-r--r--   0        0        0      221 2023-06-13 06:05:51.810070 pyg_nightly-2.4.0.dev20230613/torch_geometric/datasets/graph_generator/__init__.py
+-rw-r--r--   0        0        0      965 2023-06-13 06:05:51.810070 pyg_nightly-2.4.0.dev20230613/torch_geometric/datasets/graph_generator/ba_graph.py
+-rw-r--r--   0        0        0      949 2023-06-13 06:05:51.810070 pyg_nightly-2.4.0.dev20230613/torch_geometric/datasets/graph_generator/base.py
+-rw-r--r--   0        0        0      918 2023-06-13 06:05:51.810070 pyg_nightly-2.4.0.dev20230613/torch_geometric/datasets/graph_generator/er_graph.py
+-rw-r--r--   0        0        0     1159 2023-06-13 06:05:51.810070 pyg_nightly-2.4.0.dev20230613/torch_geometric/datasets/graph_generator/grid_graph.py
+-rw-r--r--   0        0        0     4043 2023-06-13 06:05:51.810070 pyg_nightly-2.4.0.dev20230613/torch_geometric/datasets/heterophilous_graph_dataset.py
+-rw-r--r--   0        0        0     8467 2023-06-13 06:05:51.810070 pyg_nightly-2.4.0.dev20230613/torch_geometric/datasets/hgb_dataset.py
+-rw-r--r--   0        0        0     6541 2023-06-13 06:05:51.810070 pyg_nightly-2.4.0.dev20230613/torch_geometric/datasets/hm.py
+-rw-r--r--   0        0        0    11053 2023-06-13 06:05:51.810070 pyg_nightly-2.4.0.dev20230613/torch_geometric/datasets/hydro_net.py
+-rw-r--r--   0        0        0     4447 2023-06-13 06:05:51.810070 pyg_nightly-2.4.0.dev20230613/torch_geometric/datasets/icews.py
+-rw-r--r--   0        0        0     4389 2023-06-13 06:05:51.810070 pyg_nightly-2.4.0.dev20230613/torch_geometric/datasets/igmc_dataset.py
+-rw-r--r--   0        0        0     4000 2023-06-13 06:05:51.810070 pyg_nightly-2.4.0.dev20230613/torch_geometric/datasets/imdb.py
+-rw-r--r--   0        0        0     7169 2023-06-13 06:05:51.810070 pyg_nightly-2.4.0.dev20230613/torch_geometric/datasets/infection_dataset.py
+-rw-r--r--   0        0        0     3439 2023-06-13 06:05:51.810070 pyg_nightly-2.4.0.dev20230613/torch_geometric/datasets/jodie.py
+-rw-r--r--   0        0        0     3444 2023-06-13 06:05:51.810070 pyg_nightly-2.4.0.dev20230613/torch_geometric/datasets/karate.py
+-rw-r--r--   0        0        0     4349 2023-06-13 06:05:51.810070 pyg_nightly-2.4.0.dev20230613/torch_geometric/datasets/last_fm.py
+-rw-r--r--   0        0        0     2283 2023-06-13 06:05:51.810070 pyg_nightly-2.4.0.dev20230613/torch_geometric/datasets/lastfm_asia.py
+-rw-r--r--   0        0        0     6582 2023-06-13 06:05:51.810070 pyg_nightly-2.4.0.dev20230613/torch_geometric/datasets/linkx_dataset.py
+-rw-r--r--   0        0        0    11559 2023-06-13 06:05:51.810070 pyg_nightly-2.4.0.dev20230613/torch_geometric/datasets/lrgb.py
+-rw-r--r--   0        0        0     5044 2023-06-13 06:05:51.810070 pyg_nightly-2.4.0.dev20230613/torch_geometric/datasets/malnet_tiny.py
+-rw-r--r--   0        0        0    16482 2023-06-13 06:05:51.810070 pyg_nightly-2.4.0.dev20230613/torch_geometric/datasets/md17.py
+-rw-r--r--   0        0        0     3770 2023-06-13 06:05:51.810070 pyg_nightly-2.4.0.dev20230613/torch_geometric/datasets/mixhop_synthetic_dataset.py
+-rw-r--r--   0        0        0     3136 2023-06-13 06:05:51.810070 pyg_nightly-2.4.0.dev20230613/torch_geometric/datasets/mnist_superpixels.py
+-rw-r--r--   0        0        0     5251 2023-06-13 06:05:51.810070 pyg_nightly-2.4.0.dev20230613/torch_geometric/datasets/modelnet.py
+-rw-r--r--   0        0        0     6593 2023-06-13 06:05:51.810070 pyg_nightly-2.4.0.dev20230613/torch_geometric/datasets/molecule_net.py
+-rw-r--r--   0        0        0      227 2023-06-13 06:05:51.810070 pyg_nightly-2.4.0.dev20230613/torch_geometric/datasets/motif_generator/__init__.py
+-rw-r--r--   0        0        0      910 2023-06-13 06:05:51.810070 pyg_nightly-2.4.0.dev20230613/torch_geometric/datasets/motif_generator/base.py
+-rw-r--r--   0        0        0     1203 2023-06-13 06:05:51.810070 pyg_nightly-2.4.0.dev20230613/torch_geometric/datasets/motif_generator/custom.py
+-rw-r--r--   0        0        0      984 2023-06-13 06:05:51.810070 pyg_nightly-2.4.0.dev20230613/torch_geometric/datasets/motif_generator/cycle.py
+-rw-r--r--   0        0        0      801 2023-06-13 06:05:51.810070 pyg_nightly-2.4.0.dev20230613/torch_geometric/datasets/motif_generator/house.py
+-rw-r--r--   0        0        0     3807 2023-06-13 06:05:51.810070 pyg_nightly-2.4.0.dev20230613/torch_geometric/datasets/movie_lens.py
+-rw-r--r--   0        0        0     6002 2023-06-13 06:05:51.810070 pyg_nightly-2.4.0.dev20230613/torch_geometric/datasets/movie_lens_100k.py
+-rw-r--r--   0        0        0     5162 2023-06-13 06:05:51.810070 pyg_nightly-2.4.0.dev20230613/torch_geometric/datasets/movie_lens_1m.py
+-rw-r--r--   0        0        0     2889 2023-06-13 06:05:51.810070 pyg_nightly-2.4.0.dev20230613/torch_geometric/datasets/nell.py
+-rw-r--r--   0        0        0     7190 2023-06-13 06:05:51.810070 pyg_nightly-2.4.0.dev20230613/torch_geometric/datasets/ogb_mag.py
+-rw-r--r--   0        0        0     3415 2023-06-13 06:05:51.810070 pyg_nightly-2.4.0.dev20230613/torch_geometric/datasets/omdb.py
+-rw-r--r--   0        0        0     3964 2023-06-13 06:05:51.810070 pyg_nightly-2.4.0.dev20230613/torch_geometric/datasets/particle.py
+-rw-r--r--   0        0        0    11009 2023-06-13 06:05:51.810070 pyg_nightly-2.4.0.dev20230613/torch_geometric/datasets/pascal.py
+-rw-r--r--   0        0        0     4602 2023-06-13 06:05:51.810070 pyg_nightly-2.4.0.dev20230613/torch_geometric/datasets/pascal_pf.py
+-rw-r--r--   0        0        0     5716 2023-06-13 06:05:51.810070 pyg_nightly-2.4.0.dev20230613/torch_geometric/datasets/pcpnet_dataset.py
+-rw-r--r--   0        0        0     6975 2023-06-13 06:05:51.810070 pyg_nightly-2.4.0.dev20230613/torch_geometric/datasets/planetoid.py
+-rw-r--r--   0        0        0     2842 2023-06-13 06:05:51.814070 pyg_nightly-2.4.0.dev20230613/torch_geometric/datasets/polblogs.py
+-rw-r--r--   0        0        0     4866 2023-06-13 06:05:51.814070 pyg_nightly-2.4.0.dev20230613/torch_geometric/datasets/ppi.py
+-rw-r--r--   0        0        0     3182 2023-06-13 06:05:51.814070 pyg_nightly-2.4.0.dev20230613/torch_geometric/datasets/qm7.py
+-rw-r--r--   0        0        0    16813 2023-06-13 06:05:51.814070 pyg_nightly-2.4.0.dev20230613/torch_geometric/datasets/qm9.py
+-rw-r--r--   0        0        0     2941 2023-06-13 06:05:51.814070 pyg_nightly-2.4.0.dev20230613/torch_geometric/datasets/reddit.py
+-rw-r--r--   0        0        0     4439 2023-06-13 06:05:51.814070 pyg_nightly-2.4.0.dev20230613/torch_geometric/datasets/reddit2.py
+-rw-r--r--   0        0        0     4345 2023-06-13 06:05:51.814070 pyg_nightly-2.4.0.dev20230613/torch_geometric/datasets/rel_link_pred_dataset.py
+-rw-r--r--   0        0        0     4173 2023-06-13 06:05:51.814070 pyg_nightly-2.4.0.dev20230613/torch_geometric/datasets/s3dis.py
+-rw-r--r--   0        0        0     8140 2023-06-13 06:05:51.814070 pyg_nightly-2.4.0.dev20230613/torch_geometric/datasets/sbm_dataset.py
+-rw-r--r--   0        0        0     8088 2023-06-13 06:05:51.814070 pyg_nightly-2.4.0.dev20230613/torch_geometric/datasets/shapenet.py
+-rw-r--r--   0        0        0     6150 2023-06-13 06:05:51.814070 pyg_nightly-2.4.0.dev20230613/torch_geometric/datasets/shrec2016.py
+-rw-r--r--   0        0        0     9283 2023-06-13 06:05:51.814070 pyg_nightly-2.4.0.dev20230613/torch_geometric/datasets/snap_dataset.py
+-rw-r--r--   0        0        0     3031 2023-06-13 06:05:51.814070 pyg_nightly-2.4.0.dev20230613/torch_geometric/datasets/suite_sparse.py
+-rw-r--r--   0        0        0     3959 2023-06-13 06:05:51.814070 pyg_nightly-2.4.0.dev20230613/torch_geometric/datasets/taobao.py
+-rw-r--r--   0        0        0     4451 2023-06-13 06:05:51.814070 pyg_nightly-2.4.0.dev20230613/torch_geometric/datasets/tosca.py
+-rw-r--r--   0        0        0     7302 2023-06-13 06:05:51.814070 pyg_nightly-2.4.0.dev20230613/torch_geometric/datasets/tu_dataset.py
+-rw-r--r--   0        0        0     3464 2023-06-13 06:05:51.814070 pyg_nightly-2.4.0.dev20230613/torch_geometric/datasets/twitch.py
+-rw-r--r--   0        0        0     6929 2023-06-13 06:05:51.814070 pyg_nightly-2.4.0.dev20230613/torch_geometric/datasets/upfd.py
+-rw-r--r--   0        0        0      182 2023-06-13 06:05:51.814070 pyg_nightly-2.4.0.dev20230613/torch_geometric/datasets/utils/__init__.py
+-rw-r--r--   0        0        0     1732 2023-06-13 06:05:51.814070 pyg_nightly-2.4.0.dev20230613/torch_geometric/datasets/utils/cheatsheet.py
+-rw-r--r--   0        0        0     4615 2023-06-13 06:05:51.814070 pyg_nightly-2.4.0.dev20230613/torch_geometric/datasets/webkb.py
+-rw-r--r--   0        0        0     3674 2023-06-13 06:05:51.814070 pyg_nightly-2.4.0.dev20230613/torch_geometric/datasets/wikics.py
+-rw-r--r--   0        0        0     6083 2023-06-13 06:05:51.814070 pyg_nightly-2.4.0.dev20230613/torch_geometric/datasets/wikipedia_network.py
+-rw-r--r--   0        0        0     6632 2023-06-13 06:05:51.814070 pyg_nightly-2.4.0.dev20230613/torch_geometric/datasets/willow_object_class.py
+-rw-r--r--   0        0        0     7857 2023-06-13 06:05:51.814070 pyg_nightly-2.4.0.dev20230613/torch_geometric/datasets/word_net.py
+-rw-r--r--   0        0        0     4116 2023-06-13 06:05:51.814070 pyg_nightly-2.4.0.dev20230613/torch_geometric/datasets/yelp.py
+-rw-r--r--   0        0        0     6171 2023-06-13 06:05:51.814070 pyg_nightly-2.4.0.dev20230613/torch_geometric/datasets/zinc.py
+-rw-r--r--   0        0        0     1197 2023-06-13 06:05:51.814070 pyg_nightly-2.4.0.dev20230613/torch_geometric/debug.py
+-rw-r--r--   0        0        0      748 2023-06-13 06:05:51.814070 pyg_nightly-2.4.0.dev20230613/torch_geometric/deprecation.py
+-rw-r--r--   0        0        0      171 2023-06-13 06:05:51.814070 pyg_nightly-2.4.0.dev20230613/torch_geometric/distributed/__init__.py
+-rw-r--r--   0        0        0     7687 2023-06-13 06:05:51.814070 pyg_nightly-2.4.0.dev20230613/torch_geometric/distributed/local_feature_store.py
+-rw-r--r--   0        0        0     4158 2023-06-13 06:05:51.814070 pyg_nightly-2.4.0.dev20230613/torch_geometric/distributed/local_graph_store.py
+-rw-r--r--   0        0        0     4618 2023-06-13 06:05:51.814070 pyg_nightly-2.4.0.dev20230613/torch_geometric/experimental.py
+-rw-r--r--   0        0        0      359 2023-06-13 06:05:51.814070 pyg_nightly-2.4.0.dev20230613/torch_geometric/explain/__init__.py
+-rw-r--r--   0        0        0      418 2023-06-13 06:05:51.814070 pyg_nightly-2.4.0.dev20230613/torch_geometric/explain/algorithm/__init__.py
+-rw-r--r--   0        0        0     4491 2023-06-13 06:05:51.814070 pyg_nightly-2.4.0.dev20230613/torch_geometric/explain/algorithm/attention_explainer.py
+-rw-r--r--   0        0        0     6899 2023-06-13 06:05:51.814070 pyg_nightly-2.4.0.dev20230613/torch_geometric/explain/algorithm/base.py
+-rw-r--r--   0        0        0    12489 2023-06-13 06:05:51.814070 pyg_nightly-2.4.0.dev20230613/torch_geometric/explain/algorithm/captum.py
+-rw-r--r--   0        0        0     6530 2023-06-13 06:05:51.814070 pyg_nightly-2.4.0.dev20230613/torch_geometric/explain/algorithm/captum_explainer.py
+-rw-r--r--   0        0        0     2867 2023-06-13 06:05:51.814070 pyg_nightly-2.4.0.dev20230613/torch_geometric/explain/algorithm/dummy_explainer.py
+-rw-r--r--   0        0        0    11868 2023-06-13 06:05:51.814070 pyg_nightly-2.4.0.dev20230613/torch_geometric/explain/algorithm/gnn_explainer.py
+-rw-r--r--   0        0        0    10370 2023-06-13 06:05:51.814070 pyg_nightly-2.4.0.dev20230613/torch_geometric/explain/algorithm/pg_explainer.py
+-rw-r--r--   0        0        0     2308 2023-06-13 06:05:51.814070 pyg_nightly-2.4.0.dev20230613/torch_geometric/explain/algorithm/utils.py
+-rw-r--r--   0        0        0     7834 2023-06-13 06:05:51.814070 pyg_nightly-2.4.0.dev20230613/torch_geometric/explain/config.py
+-rw-r--r--   0        0        0    10375 2023-06-13 06:05:51.814070 pyg_nightly-2.4.0.dev20230613/torch_geometric/explain/explainer.py
+-rw-r--r--   0        0        0    14842 2023-06-13 06:05:51.814070 pyg_nightly-2.4.0.dev20230613/torch_geometric/explain/explanation.py
+-rw-r--r--   0        0        0      301 2023-06-13 06:05:51.814070 pyg_nightly-2.4.0.dev20230613/torch_geometric/explain/metric/__init__.py
+-rw-r--r--   0        0        0     1888 2023-06-13 06:05:51.814070 pyg_nightly-2.4.0.dev20230613/torch_geometric/explain/metric/basic.py
+-rw-r--r--   0        0        0     3063 2023-06-13 06:05:51.814070 pyg_nightly-2.4.0.dev20230613/torch_geometric/explain/metric/faithfulness.py
+-rw-r--r--   0        0        0     6157 2023-06-13 06:05:51.814070 pyg_nightly-2.4.0.dev20230613/torch_geometric/explain/metric/fidelity.py
+-rw-r--r--   0        0        0     2045 2023-06-13 06:05:51.814070 pyg_nightly-2.4.0.dev20230613/torch_geometric/graphgym/__init__.py
+-rw-r--r--   0        0        0      510 2023-06-13 06:05:51.814070 pyg_nightly-2.4.0.dev20230613/torch_geometric/graphgym/benchmark.py
+-rw-r--r--   0        0        0     2371 2023-06-13 06:05:51.814070 pyg_nightly-2.4.0.dev20230613/torch_geometric/graphgym/checkpoint.py
+-rw-r--r--   0        0        0      738 2023-06-13 06:05:51.814070 pyg_nightly-2.4.0.dev20230613/torch_geometric/graphgym/cmd_args.py
+-rw-r--r--   0        0        0    17221 2023-06-13 06:05:51.814070 pyg_nightly-2.4.0.dev20230613/torch_geometric/graphgym/config.py
+-rw-r--r--   0        0        0    14575 2023-06-13 06:05:51.814070 pyg_nightly-2.4.0.dev20230613/torch_geometric/graphgym/config_store.py
+-rw-r--r--   0        0        0      389 2023-06-13 06:05:51.814070 pyg_nightly-2.4.0.dev20230613/torch_geometric/graphgym/contrib/__init__.py
+-rw-r--r--   0        0        0      221 2023-06-13 06:05:51.814070 pyg_nightly-2.4.0.dev20230613/torch_geometric/graphgym/contrib/act/__init__.py
+-rw-r--r--   0        0        0      221 2023-06-13 06:05:51.814070 pyg_nightly-2.4.0.dev20230613/torch_geometric/graphgym/contrib/config/__init__.py
+-rw-r--r--   0        0        0      221 2023-06-13 06:05:51.814070 pyg_nightly-2.4.0.dev20230613/torch_geometric/graphgym/contrib/encoder/__init__.py
+-rw-r--r--   0        0        0      221 2023-06-13 06:05:51.814070 pyg_nightly-2.4.0.dev20230613/torch_geometric/graphgym/contrib/head/__init__.py
+-rw-r--r--   0        0        0      221 2023-06-13 06:05:51.814070 pyg_nightly-2.4.0.dev20230613/torch_geometric/graphgym/contrib/layer/__init__.py
+-rw-r--r--   0        0        0     8304 2023-06-13 06:05:51.814070 pyg_nightly-2.4.0.dev20230613/torch_geometric/graphgym/contrib/layer/generalconv.py
+-rw-r--r--   0        0        0      221 2023-06-13 06:05:51.814070 pyg_nightly-2.4.0.dev20230613/torch_geometric/graphgym/contrib/loader/__init__.py
+-rw-r--r--   0        0        0      221 2023-06-13 06:05:51.814070 pyg_nightly-2.4.0.dev20230613/torch_geometric/graphgym/contrib/loss/__init__.py
+-rw-r--r--   0        0        0      221 2023-06-13 06:05:51.818070 pyg_nightly-2.4.0.dev20230613/torch_geometric/graphgym/contrib/network/__init__.py
+-rw-r--r--   0        0        0      221 2023-06-13 06:05:51.818070 pyg_nightly-2.4.0.dev20230613/torch_geometric/graphgym/contrib/optimizer/__init__.py
+-rw-r--r--   0        0        0      221 2023-06-13 06:05:51.818070 pyg_nightly-2.4.0.dev20230613/torch_geometric/graphgym/contrib/pooling/__init__.py
+-rw-r--r--   0        0        0      221 2023-06-13 06:05:51.818070 pyg_nightly-2.4.0.dev20230613/torch_geometric/graphgym/contrib/stage/__init__.py
+-rw-r--r--   0        0        0      221 2023-06-13 06:05:51.818070 pyg_nightly-2.4.0.dev20230613/torch_geometric/graphgym/contrib/train/__init__.py
+-rw-r--r--   0        0        0      221 2023-06-13 06:05:51.818070 pyg_nightly-2.4.0.dev20230613/torch_geometric/graphgym/contrib/transform/__init__.py
+-rw-r--r--   0        0        0      375 2023-06-13 06:05:51.818070 pyg_nightly-2.4.0.dev20230613/torch_geometric/graphgym/imports.py
+-rw-r--r--   0        0        0      490 2023-06-13 06:05:51.818070 pyg_nightly-2.4.0.dev20230613/torch_geometric/graphgym/init.py
+-rw-r--r--   0        0        0    11763 2023-06-13 06:05:51.818070 pyg_nightly-2.4.0.dev20230613/torch_geometric/graphgym/loader.py
+-rw-r--r--   0        0        0    11329 2023-06-13 06:05:51.818070 pyg_nightly-2.4.0.dev20230613/torch_geometric/graphgym/logger.py
+-rw-r--r--   0        0        0     1474 2023-06-13 06:05:51.818070 pyg_nightly-2.4.0.dev20230613/torch_geometric/graphgym/loss.py
+-rw-r--r--   0        0        0     3110 2023-06-13 06:05:51.818070 pyg_nightly-2.4.0.dev20230613/torch_geometric/graphgym/model_builder.py
+-rw-r--r--   0        0        0     1121 2023-06-13 06:05:51.818070 pyg_nightly-2.4.0.dev20230613/torch_geometric/graphgym/models/__init__.py
+-rw-r--r--   0        0        0      822 2023-06-13 06:05:51.818070 pyg_nightly-2.4.0.dev20230613/torch_geometric/graphgym/models/act.py
+-rw-r--r--   0        0        0     2546 2023-06-13 06:05:51.818070 pyg_nightly-2.4.0.dev20230613/torch_geometric/graphgym/models/encoder.py
+-rw-r--r--   0        0        0     5133 2023-06-13 06:05:51.818070 pyg_nightly-2.4.0.dev20230613/torch_geometric/graphgym/models/gnn.py
+-rw-r--r--   0        0        0     4434 2023-06-13 06:05:51.818070 pyg_nightly-2.4.0.dev20230613/torch_geometric/graphgym/models/head.py
+-rw-r--r--   0        0        0    12486 2023-06-13 06:05:51.818070 pyg_nightly-2.4.0.dev20230613/torch_geometric/graphgym/models/layer.py
+-rw-r--r--   0        0        0      288 2023-06-13 06:05:51.818070 pyg_nightly-2.4.0.dev20230613/torch_geometric/graphgym/models/pooling.py
+-rw-r--r--   0        0        0     1391 2023-06-13 06:05:51.818070 pyg_nightly-2.4.0.dev20230613/torch_geometric/graphgym/models/transform.py
+-rw-r--r--   0        0        0     2544 2023-06-13 06:05:51.818070 pyg_nightly-2.4.0.dev20230613/torch_geometric/graphgym/optim.py
+-rw-r--r--   0        0        0     3944 2023-06-13 06:05:51.818070 pyg_nightly-2.4.0.dev20230613/torch_geometric/graphgym/register.py
+-rw-r--r--   0        0        0     1887 2023-06-13 06:05:51.818070 pyg_nightly-2.4.0.dev20230613/torch_geometric/graphgym/train.py
+-rw-r--r--   0        0        0        0 2023-06-13 06:05:51.818070 pyg_nightly-2.4.0.dev20230613/torch_geometric/graphgym/utils/LICENSE
+-rw-r--r--   0        0        0      641 2023-06-13 06:05:51.818070 pyg_nightly-2.4.0.dev20230613/torch_geometric/graphgym/utils/__init__.py
+-rw-r--r--   0        0        0     9513 2023-06-13 06:05:51.818070 pyg_nightly-2.4.0.dev20230613/torch_geometric/graphgym/utils/agg_runs.py
+-rw-r--r--   0        0        0     3056 2023-06-13 06:05:51.818070 pyg_nightly-2.4.0.dev20230613/torch_geometric/graphgym/utils/comp_budget.py
+-rw-r--r--   0        0        0     1352 2023-06-13 06:05:51.818070 pyg_nightly-2.4.0.dev20230613/torch_geometric/graphgym/utils/device.py
+-rw-r--r--   0        0        0      690 2023-06-13 06:05:51.818070 pyg_nightly-2.4.0.dev20230613/torch_geometric/graphgym/utils/epoch.py
+-rw-r--r--   0        0        0     2050 2023-06-13 06:05:51.818070 pyg_nightly-2.4.0.dev20230613/torch_geometric/graphgym/utils/io.py
+-rw-r--r--   0        0        0      606 2023-06-13 06:05:51.818070 pyg_nightly-2.4.0.dev20230613/torch_geometric/graphgym/utils/plot.py
+-rw-r--r--   0        0        0      198 2023-06-13 06:05:51.818070 pyg_nightly-2.4.0.dev20230613/torch_geometric/graphgym/utils/tools.py
+-rw-r--r--   0        0        0      830 2023-06-13 06:05:51.818070 pyg_nightly-2.4.0.dev20230613/torch_geometric/home.py
+-rw-r--r--   0        0        0      528 2023-06-13 06:05:51.818070 pyg_nightly-2.4.0.dev20230613/torch_geometric/io/__init__.py
+-rw-r--r--   0        0        0     1148 2023-06-13 06:05:51.818070 pyg_nightly-2.4.0.dev20230613/torch_geometric/io/npz.py
+-rw-r--r--   0        0        0      957 2023-06-13 06:05:51.818070 pyg_nightly-2.4.0.dev20230613/torch_geometric/io/obj.py
+-rw-r--r--   0        0        0     2586 2023-06-13 06:05:51.818070 pyg_nightly-2.4.0.dev20230613/torch_geometric/io/off.py
+-rw-r--r--   0        0        0     4243 2023-06-13 06:05:51.818070 pyg_nightly-2.4.0.dev20230613/torch_geometric/io/planetoid.py
+-rw-r--r--   0        0        0      476 2023-06-13 06:05:51.818070 pyg_nightly-2.4.0.dev20230613/torch_geometric/io/ply.py
+-rw-r--r--   0        0        0     1136 2023-06-13 06:05:51.818070 pyg_nightly-2.4.0.dev20230613/torch_geometric/io/sdf.py
+-rw-r--r--   0        0        0     4733 2023-06-13 06:05:51.818070 pyg_nightly-2.4.0.dev20230613/torch_geometric/io/tu.py
+-rw-r--r--   0        0        0      562 2023-06-13 06:05:51.818070 pyg_nightly-2.4.0.dev20230613/torch_geometric/io/txt_array.py
+-rw-r--r--   0        0        0      768 2023-06-13 06:05:51.818070 pyg_nightly-2.4.0.dev20230613/torch_geometric/lazy_loader.py
+-rw-r--r--   0        0        0     1675 2023-06-13 06:05:51.818070 pyg_nightly-2.4.0.dev20230613/torch_geometric/loader/__init__.py
+-rw-r--r--   0        0        0     1433 2023-06-13 06:05:51.818070 pyg_nightly-2.4.0.dev20230613/torch_geometric/loader/base.py
+-rw-r--r--   0        0        0    11594 2023-06-13 06:05:51.818070 pyg_nightly-2.4.0.dev20230613/torch_geometric/loader/cluster.py
+-rw-r--r--   0        0        0     1449 2023-06-13 06:05:51.818070 pyg_nightly-2.4.0.dev20230613/torch_geometric/loader/data_list_loader.py
+-rw-r--r--   0        0        0     3222 2023-06-13 06:05:51.818070 pyg_nightly-2.4.0.dev20230613/torch_geometric/loader/dataloader.py
+-rw-r--r--   0        0        0     1683 2023-06-13 06:05:51.818070 pyg_nightly-2.4.0.dev20230613/torch_geometric/loader/dense_data_loader.py
+-rw-r--r--   0        0        0     4285 2023-06-13 06:05:51.818070 pyg_nightly-2.4.0.dev20230613/torch_geometric/loader/dynamic_batch_sampler.py
+-rw-r--r--   0        0        0     8448 2023-06-13 06:05:51.818070 pyg_nightly-2.4.0.dev20230613/torch_geometric/loader/graph_saint.py
+-rw-r--r--   0        0        0     6012 2023-06-13 06:05:51.818070 pyg_nightly-2.4.0.dev20230613/torch_geometric/loader/hgt_loader.py
+-rw-r--r--   0        0        0     3754 2023-06-13 06:05:51.818070 pyg_nightly-2.4.0.dev20230613/torch_geometric/loader/imbalanced_sampler.py
+-rw-r--r--   0        0        0    14219 2023-06-13 06:05:51.818070 pyg_nightly-2.4.0.dev20230613/torch_geometric/loader/link_loader.py
+-rw-r--r--   0        0        0    12587 2023-06-13 06:05:51.818070 pyg_nightly-2.4.0.dev20230613/torch_geometric/loader/link_neighbor_loader.py
+-rw-r--r--   0        0        0     6317 2023-06-13 06:05:51.818070 pyg_nightly-2.4.0.dev20230613/torch_geometric/loader/mixin.py
+-rw-r--r--   0        0        0    11382 2023-06-13 06:05:51.818070 pyg_nightly-2.4.0.dev20230613/torch_geometric/loader/neighbor_loader.py
+-rw-r--r--   0        0        0     8513 2023-06-13 06:05:51.818070 pyg_nightly-2.4.0.dev20230613/torch_geometric/loader/neighbor_sampler.py
+-rw-r--r--   0        0        0     9365 2023-06-13 06:05:51.818070 pyg_nightly-2.4.0.dev20230613/torch_geometric/loader/node_loader.py
+-rw-r--r--   0        0        0     2141 2023-06-13 06:05:51.818070 pyg_nightly-2.4.0.dev20230613/torch_geometric/loader/prefetch.py
+-rw-r--r--   0        0        0     2196 2023-06-13 06:05:51.818070 pyg_nightly-2.4.0.dev20230613/torch_geometric/loader/random_node_loader.py
+-rw-r--r--   0        0        0     4173 2023-06-13 06:05:51.818070 pyg_nightly-2.4.0.dev20230613/torch_geometric/loader/shadow.py
+-rw-r--r--   0        0        0     1319 2023-06-13 06:05:51.818070 pyg_nightly-2.4.0.dev20230613/torch_geometric/loader/temporal_dataloader.py
+-rw-r--r--   0        0        0    12273 2023-06-13 06:05:51.818070 pyg_nightly-2.4.0.dev20230613/torch_geometric/loader/utils.py
+-rw-r--r--   0        0        0     3518 2023-06-13 06:05:51.818070 pyg_nightly-2.4.0.dev20230613/torch_geometric/loader/zip_loader.py
+-rw-r--r--   0        0        0      832 2023-06-13 06:05:51.818070 pyg_nightly-2.4.0.dev20230613/torch_geometric/logging.py
+-rw-r--r--   0        0        0      847 2023-06-13 06:05:51.818070 pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/__init__.py
+-rw-r--r--   0        0        0     1397 2023-06-13 06:05:51.818070 pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/aggr/__init__.py
+-rw-r--r--   0        0        0     2395 2023-06-13 06:05:51.818070 pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/aggr/attention.py
+-rw-r--r--   0        0        0     7449 2023-06-13 06:05:51.818070 pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/aggr/base.py
+-rw-r--r--   0        0        0    11000 2023-06-13 06:05:51.818070 pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/aggr/basic.py
+-rw-r--r--   0        0        0     2064 2023-06-13 06:05:51.818070 pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/aggr/deep_sets.py
+-rw-r--r--   0        0        0     6643 2023-06-13 06:05:51.818070 pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/aggr/equilibrium.py
+-rw-r--r--   0        0        0    12229 2023-06-13 06:05:51.818070 pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/aggr/fused.py
+-rw-r--r--   0        0        0     3346 2023-06-13 06:05:51.818070 pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/aggr/gmt.py
+-rw-r--r--   0        0        0     1747 2023-06-13 06:05:51.822070 pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/aggr/gru.py
+-rw-r--r--   0        0        0     1767 2023-06-13 06:05:51.822070 pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/aggr/lstm.py
+-rw-r--r--   0        0        0     1995 2023-06-13 06:05:51.822070 pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/aggr/mlp.py
+-rw-r--r--   0        0        0     8170 2023-06-13 06:05:51.822070 pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/aggr/multi.py
+-rw-r--r--   0        0        0     6174 2023-06-13 06:05:51.822070 pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/aggr/quantile.py
+-rw-r--r--   0        0        0     4642 2023-06-13 06:05:51.822070 pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/aggr/scaler.py
+-rw-r--r--   0        0        0     2517 2023-06-13 06:05:51.822070 pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/aggr/set2set.py
+-rw-r--r--   0        0        0     3723 2023-06-13 06:05:51.822070 pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/aggr/set_transformer.py
+-rw-r--r--   0        0        0     2061 2023-06-13 06:05:51.822070 pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/aggr/sort.py
+-rw-r--r--   0        0        0     8322 2023-06-13 06:05:51.822070 pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/aggr/utils.py
+-rw-r--r--   0        0        0       76 2023-06-13 06:05:51.822070 pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/attention/__init__.py
+-rw-r--r--   0        0        0     7687 2023-06-13 06:05:51.822070 pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/attention/performer.py
+-rw-r--r--   0        0        0     3360 2023-06-13 06:05:51.822070 pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/conv/__init__.py
+-rw-r--r--   0        0        0     3088 2023-06-13 06:05:51.822070 pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/conv/agnn_conv.py
+-rw-r--r--   0        0        0     4388 2023-06-13 06:05:51.822070 pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/conv/antisymmetric_conv.py
+-rw-r--r--   0        0        0     6010 2023-06-13 06:05:51.822070 pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/conv/appnp.py
+-rw-r--r--   0        0        0     6637 2023-06-13 06:05:51.822070 pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/conv/arma_conv.py
+-rw-r--r--   0        0        0     4036 2023-06-13 06:05:51.822070 pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/conv/cg_conv.py
+-rw-r--r--   0        0        0     6444 2023-06-13 06:05:51.822070 pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/conv/cheb_conv.py
+-rw-r--r--   0        0        0     5303 2023-06-13 06:05:51.822070 pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/conv/cluster_gcn_conv.py
+-rw-r--r--   0        0        0      251 2023-06-13 06:05:51.822070 pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/conv/cugraph/__init__.py
+-rw-r--r--   0        0        0     8195 2023-06-13 06:05:51.822070 pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/conv/cugraph/base.py
+-rw-r--r--   0        0        0     2849 2023-06-13 06:05:51.822070 pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/conv/cugraph/gat_conv.py
+-rw-r--r--   0        0        0     4218 2023-06-13 06:05:51.822070 pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/conv/cugraph/rgcn_conv.py
+-rw-r--r--   0        0        0     2802 2023-06-13 06:05:51.822070 pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/conv/cugraph/sage_conv.py
+-rw-r--r--   0        0        0    12105 2023-06-13 06:05:51.822070 pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/conv/dna_conv.py
+-rw-r--r--   0        0        0     5550 2023-06-13 06:05:51.822070 pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/conv/edge_conv.py
+-rw-r--r--   0        0        0    10482 2023-06-13 06:05:51.822070 pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/conv/eg_conv.py
+-rw-r--r--   0        0        0     7927 2023-06-13 06:05:51.822070 pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/conv/fa_conv.py
+-rw-r--r--   0        0        0     4453 2023-06-13 06:05:51.822070 pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/conv/feast_conv.py
+-rw-r--r--   0        0        0     6332 2023-06-13 06:05:51.822070 pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/conv/film_conv.py
+-rw-r--r--   0        0        0     4242 2023-06-13 06:05:51.822070 pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/conv/fused_gat_conv.py
+-rw-r--r--   0        0        0    13610 2023-06-13 06:05:51.822070 pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/conv/gat_conv.py
+-rw-r--r--   0        0        0     3582 2023-06-13 06:05:51.822070 pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/conv/gated_graph_conv.py
+-rw-r--r--   0        0        0    12423 2023-06-13 06:05:51.822070 pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/conv/gatv2_conv.py
+-rw-r--r--   0        0        0     7022 2023-06-13 06:05:51.822070 pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/conv/gcn2_conv.py
+-rw-r--r--   0        0        0     9333 2023-06-13 06:05:51.822070 pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/conv/gcn_conv.py
+-rw-r--r--   0        0        0     9992 2023-06-13 06:05:51.822070 pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/conv/gen_conv.py
+-rw-r--r--   0        0        0     7536 2023-06-13 06:05:51.822070 pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/conv/general_conv.py
+-rw-r--r--   0        0        0     7444 2023-06-13 06:05:51.822070 pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/conv/gin_conv.py
+-rw-r--r--   0        0        0     8320 2023-06-13 06:05:51.822070 pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/conv/gmm_conv.py
+-rw-r--r--   0        0        0     6672 2023-06-13 06:05:51.822070 pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/conv/gps_conv.py
+-rw-r--r--   0        0        0     3547 2023-06-13 06:05:51.822070 pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/conv/graph_conv.py
+-rw-r--r--   0        0        0     5023 2023-06-13 06:05:51.822070 pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/conv/gravnet_conv.py
+-rw-r--r--   0        0        0     7354 2023-06-13 06:05:51.822070 pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/conv/han_conv.py
+-rw-r--r--   0        0        0     6063 2023-06-13 06:05:51.822070 pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/conv/heat_conv.py
+-rw-r--r--   0        0        0     6470 2023-06-13 06:05:51.822070 pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/conv/hetero_conv.py
+-rw-r--r--   0        0        0     9282 2023-06-13 06:05:51.822070 pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/conv/hgt_conv.py
+-rw-r--r--   0        0        0     7911 2023-06-13 06:05:51.822070 pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/conv/hypergraph_conv.py
+-rw-r--r--   0        0        0     3523 2023-06-13 06:05:51.822070 pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/conv/le_conv.py
+-rw-r--r--   0        0        0     2418 2023-06-13 06:05:51.822070 pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/conv/lg_conv.py
+-rw-r--r--   0        0        0    11524 2023-06-13 06:05:51.822070 pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/conv/message_passing.jinja
+-rw-r--r--   0        0        0    39859 2023-06-13 06:05:51.822070 pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/conv/message_passing.py
+-rw-r--r--   0        0        0     4321 2023-06-13 06:05:51.822070 pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/conv/mf_conv.py
+-rw-r--r--   0        0        0     4743 2023-06-13 06:05:51.826071 pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/conv/nn_conv.py
+-rw-r--r--   0        0        0     4928 2023-06-13 06:05:51.826071 pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/conv/pan_conv.py
+-rw-r--r--   0        0        0     4916 2023-06-13 06:05:51.826071 pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/conv/pdn_conv.py
+-rw-r--r--   0        0        0     8242 2023-06-13 06:05:51.826071 pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/conv/pna_conv.py
+-rw-r--r--   0        0        0     4522 2023-06-13 06:05:51.826071 pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/conv/point_conv.py
+-rw-r--r--   0        0        0     3288 2023-06-13 06:05:51.826071 pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/conv/point_gnn_conv.py
+-rw-r--r--   0        0        0     5889 2023-06-13 06:05:51.826071 pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/conv/point_transformer_conv.py
+-rw-r--r--   0        0        0     5422 2023-06-13 06:05:51.826071 pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/conv/ppf_conv.py
+-rw-r--r--   0        0        0     4180 2023-06-13 06:05:51.826071 pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/conv/res_gated_graph_conv.py
+-rw-r--r--   0        0        0    22785 2023-06-13 06:05:51.826071 pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/conv/rgat_conv.py
+-rw-r--r--   0        0        0    14977 2023-06-13 06:05:51.826071 pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/conv/rgcn_conv.py
+-rw-r--r--   0        0        0     5813 2023-06-13 06:05:51.826071 pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/conv/sage_conv.py
+-rw-r--r--   0        0        0     4597 2023-06-13 06:05:51.826071 pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/conv/sg_conv.py
+-rw-r--r--   0        0        0     6283 2023-06-13 06:05:51.826071 pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/conv/signed_conv.py
+-rw-r--r--   0        0        0     3899 2023-06-13 06:05:51.826071 pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/conv/simple_conv.py
+-rw-r--r--   0        0        0     6330 2023-06-13 06:05:51.826071 pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/conv/spline_conv.py
+-rw-r--r--   0        0        0     5185 2023-06-13 06:05:51.826071 pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/conv/ssg_conv.py
+-rw-r--r--   0        0        0    11980 2023-06-13 06:05:51.826071 pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/conv/supergat_conv.py
+-rw-r--r--   0        0        0     4215 2023-06-13 06:05:51.826071 pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/conv/tag_conv.py
+-rw-r--r--   0        0        0     9425 2023-06-13 06:05:51.826071 pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/conv/transformer_conv.py
+-rw-r--r--   0        0        0      823 2023-06-13 06:05:51.826071 pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/conv/utils/__init__.py
+-rw-r--r--   0        0        0     2692 2023-06-13 06:05:51.826071 pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/conv/utils/cheatsheet.py
+-rw-r--r--   0        0        0      186 2023-06-13 06:05:51.826071 pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/conv/utils/helpers.py
+-rw-r--r--   0        0        0     3259 2023-06-13 06:05:51.826071 pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/conv/utils/inspector.py
+-rw-r--r--   0        0        0      679 2023-06-13 06:05:51.826071 pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/conv/utils/jit.py
+-rw-r--r--   0        0        0     3859 2023-06-13 06:05:51.826071 pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/conv/utils/typing.py
+-rw-r--r--   0        0        0     3103 2023-06-13 06:05:51.826071 pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/conv/wl_conv.py
+-rw-r--r--   0        0        0     2349 2023-06-13 06:05:51.826071 pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/conv/wl_conv_continuous.py
+-rw-r--r--   0        0        0     5955 2023-06-13 06:05:51.826071 pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/conv/x_conv.py
+-rw-r--r--   0        0        0     3960 2023-06-13 06:05:51.826071 pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/data_parallel.py
+-rw-r--r--   0        0        0      712 2023-06-13 06:05:51.826071 pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/dense/__init__.py
+-rw-r--r--   0        0        0     4228 2023-06-13 06:05:51.826071 pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/dense/dense_gat_conv.py
+-rw-r--r--   0        0        0     2989 2023-06-13 06:05:51.826071 pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/dense/dense_gcn_conv.py
+-rw-r--r--   0        0        0     2357 2023-06-13 06:05:51.826071 pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/dense/dense_gin_conv.py
+-rw-r--r--   0        0        0     2737 2023-06-13 06:05:51.826071 pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/dense/dense_graph_conv.py
+-rw-r--r--   0        0        0     2658 2023-06-13 06:05:51.826071 pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/dense/dense_sage_conv.py
+-rw-r--r--   0        0        0     3050 2023-06-13 06:05:51.826071 pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/dense/diff_pool.py
+-rw-r--r--   0        0        0     5671 2023-06-13 06:05:51.826071 pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/dense/dmon_pool.py
+-rw-r--r--   0        0        0    17141 2023-06-13 06:05:51.826071 pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/dense/linear.py
+-rw-r--r--   0        0        0     4111 2023-06-13 06:05:51.826071 pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/dense/mincut_pool.py
+-rw-r--r--   0        0        0     3125 2023-06-13 06:05:51.826071 pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/encoding.py
+-rw-r--r--   0        0        0       92 2023-06-13 06:05:51.826071 pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/functional/__init__.py
+-rw-r--r--   0        0        0     1549 2023-06-13 06:05:51.826071 pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/functional/bro.py
+-rw-r--r--   0        0        0      863 2023-06-13 06:05:51.826071 pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/functional/gini.py
+-rw-r--r--   0        0        0    15551 2023-06-13 06:05:51.826071 pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/fx.py
+-rw-r--r--   0        0        0     1088 2023-06-13 06:05:51.826071 pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/glob.py
+-rw-r--r--   0        0        0     2457 2023-06-13 06:05:51.826071 pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/inits.py
+-rw-r--r--   0        0        0      241 2023-06-13 06:05:51.826071 pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/kge/__init__.py
+-rw-r--r--   0        0        0     5739 2023-06-13 06:05:51.826071 pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/kge/base.py
+-rw-r--r--   0        0        0     3234 2023-06-13 06:05:51.826071 pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/kge/complex.py
+-rw-r--r--   0        0        0     2462 2023-06-13 06:05:51.826071 pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/kge/distmult.py
+-rw-r--r--   0        0        0      771 2023-06-13 06:05:51.826071 pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/kge/loader.py
+-rw-r--r--   0        0        0     3208 2023-06-13 06:05:51.826071 pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/kge/rotate.py
+-rw-r--r--   0        0        0     3088 2023-06-13 06:05:51.826071 pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/kge/transe.py
+-rw-r--r--   0        0        0     8937 2023-06-13 06:05:51.826071 pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/lr_scheduler.py
+-rw-r--r--   0        0        0     9512 2023-06-13 06:05:51.826071 pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/model_hub.py
+-rw-r--r--   0        0        0     1647 2023-06-13 06:05:51.826071 pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/models/__init__.py
+-rw-r--r--   0        0        0     6591 2023-06-13 06:05:51.826071 pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/models/attentive_fp.py
+-rw-r--r--   0        0        0    10656 2023-06-13 06:05:51.826071 pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/models/autoencoder.py
+-rw-r--r--   0        0        0    28624 2023-06-13 06:05:51.826071 pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/models/basic_gnn.py
+-rw-r--r--   0        0        0     4138 2023-06-13 06:05:51.826071 pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/models/captum.py
+-rw-r--r--   0        0        0     6799 2023-06-13 06:05:51.826071 pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/models/correct_and_smooth.py
+-rw-r--r--   0        0        0     3972 2023-06-13 06:05:51.826071 pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/models/deep_graph_infomax.py
+-rw-r--r--   0        0        0     4223 2023-06-13 06:05:51.826071 pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/models/deepgcn.py
+-rw-r--r--   0        0        0    34432 2023-06-13 06:05:51.826071 pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/models/dimenet.py
+-rw-r--r--   0        0        0     4611 2023-06-13 06:05:51.826071 pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/models/dimenet_utils.py
+-rw-r--r--   0        0        0     7859 2023-06-13 06:05:51.826071 pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/models/gnnff.py
+-rw-r--r--   0        0        0     1667 2023-06-13 06:05:51.826071 pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/models/graph_mixer.py
+-rw-r--r--   0        0        0     5381 2023-06-13 06:05:51.826071 pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/models/graph_unet.py
+-rw-r--r--   0        0        0     3397 2023-06-13 06:05:51.826071 pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/models/jumping_knowledge.py
+-rw-r--r--   0        0        0     3937 2023-06-13 06:05:51.826071 pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/models/label_prop.py
+-rw-r--r--   0        0        0    11282 2023-06-13 06:05:51.830071 pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/models/lightgcn.py
+-rw-r--r--   0        0        0     7901 2023-06-13 06:05:51.830071 pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/models/linkx.py
+-rw-r--r--   0        0        0     2566 2023-06-13 06:05:51.830071 pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/models/mask_label.py
+-rw-r--r--   0        0        0     6529 2023-06-13 06:05:51.830071 pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/models/meta.py
+-rw-r--r--   0        0        0    10318 2023-06-13 06:05:51.830071 pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/models/metapath2vec.py
+-rw-r--r--   0        0        0     8980 2023-06-13 06:05:51.830071 pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/models/mlp.py
+-rw-r--r--   0        0        0     7641 2023-06-13 06:05:51.830071 pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/models/node2vec.py
+-rw-r--r--   0        0        0     3524 2023-06-13 06:05:51.830071 pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/models/pmlp.py
+-rw-r--r--   0        0        0     8979 2023-06-13 06:05:51.830071 pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/models/re_net.py
+-rw-r--r--   0        0        0     5789 2023-06-13 06:05:51.830071 pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/models/rect.py
+-rw-r--r--   0        0        0    11818 2023-06-13 06:05:51.830071 pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/models/rev_gnn.py
+-rw-r--r--   0        0        0    16599 2023-06-13 06:05:51.830071 pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/models/schnet.py
+-rw-r--r--   0        0        0     9840 2023-06-13 06:05:51.830071 pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/models/signed_gcn.py
+-rw-r--r--   0        0        0    11590 2023-06-13 06:05:51.830071 pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/models/tgn.py
+-rw-r--r--   0        0        0     1957 2023-06-13 06:05:51.830071 pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/module_dict.py
+-rw-r--r--   0        0        0      638 2023-06-13 06:05:51.830071 pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/norm/__init__.py
+-rw-r--r--   0        0        0     8258 2023-06-13 06:05:51.830071 pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/norm/batch_norm.py
+-rw-r--r--   0        0        0     4706 2023-06-13 06:05:51.830071 pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/norm/diff_group_norm.py
+-rw-r--r--   0        0        0     2715 2023-06-13 06:05:51.830071 pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/norm/graph_norm.py
+-rw-r--r--   0        0        0     1492 2023-06-13 06:05:51.830071 pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/norm/graph_size_norm.py
+-rw-r--r--   0        0        0     4670 2023-06-13 06:05:51.830071 pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/norm/instance_norm.py
+-rw-r--r--   0        0        0     7806 2023-06-13 06:05:51.830071 pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/norm/layer_norm.py
+-rw-r--r--   0        0        0     1311 2023-06-13 06:05:51.830071 pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/norm/mean_subtraction_norm.py
+-rw-r--r--   0        0        0     1654 2023-06-13 06:05:51.830071 pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/norm/msg_norm.py
+-rw-r--r--   0        0        0     2809 2023-06-13 06:05:51.830071 pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/norm/pair_norm.py
+-rw-r--r--   0        0        0     1982 2023-06-13 06:05:51.830071 pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/parameter_dict.py
+-rw-r--r--   0        0        0    13307 2023-06-13 06:05:51.830071 pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/pool/__init__.py
+-rw-r--r--   0        0        0     3967 2023-06-13 06:05:51.830071 pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/pool/approx_knn.py
+-rw-r--r--   0        0        0     6870 2023-06-13 06:05:51.830071 pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/pool/asap.py
+-rw-r--r--   0        0        0     3966 2023-06-13 06:05:51.830071 pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/pool/avg_pool.py
+-rw-r--r--   0        0        0       92 2023-06-13 06:05:51.830071 pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/pool/connect/__init__.py
+-rw-r--r--   0        0        0     4001 2023-06-13 06:05:51.830071 pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/pool/connect/base.py
+-rw-r--r--   0        0        0      273 2023-06-13 06:05:51.830071 pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/pool/consecutive.py
+-rw-r--r--   0        0        0     1600 2023-06-13 06:05:51.830071 pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/pool/decimation.py
+-rw-r--r--   0        0        0     8567 2023-06-13 06:05:51.830071 pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/pool/edge_pool.py
+-rw-r--r--   0        0        0     3510 2023-06-13 06:05:51.830071 pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/pool/glob.py
+-rw-r--r--   0        0        0     1292 2023-06-13 06:05:51.830071 pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/pool/graclus.py
+-rw-r--r--   0        0        0     4262 2023-06-13 06:05:51.830071 pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/pool/max_pool.py
+-rw-r--r--   0        0        0     5362 2023-06-13 06:05:51.830071 pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/pool/mem_pool.py
+-rw-r--r--   0        0        0     4400 2023-06-13 06:05:51.830071 pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/pool/pan_pool.py
+-rw-r--r--   0        0        0      631 2023-06-13 06:05:51.830071 pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/pool/pool.py
+-rw-r--r--   0        0        0     5966 2023-06-13 06:05:51.830071 pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/pool/sag_pool.py
+-rw-r--r--   0        0        0      135 2023-06-13 06:05:51.830071 pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/pool/select/__init__.py
+-rw-r--r--   0        0        0     3208 2023-06-13 06:05:51.830071 pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/pool/select/base.py
+-rw-r--r--   0        0        0     6262 2023-06-13 06:05:51.830071 pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/pool/select/topk.py
+-rw-r--r--   0        0        0     5760 2023-06-13 06:05:51.830071 pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/pool/topk_pool.py
+-rw-r--r--   0        0        0     2737 2023-06-13 06:05:51.830071 pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/pool/voxel_grid.py
+-rw-r--r--   0        0        0      412 2023-06-13 06:05:51.830071 pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/reshape.py
+-rw-r--r--   0        0        0     6155 2023-06-13 06:05:51.830071 pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/resolver.py
+-rw-r--r--   0        0        0     1071 2023-06-13 06:05:51.830071 pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/sequential.jinja
+-rw-r--r--   0        0        0     4577 2023-06-13 06:05:51.830071 pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/sequential.py
+-rw-r--r--   0        0        0     5616 2023-06-13 06:05:51.830071 pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/summary.py
+-rw-r--r--   0        0        0     1282 2023-06-13 06:05:51.830071 pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/to_fixed_size_transformer.py
+-rw-r--r--   0        0        0     6486 2023-06-13 06:05:51.830071 pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/to_hetero_module.py
+-rw-r--r--   0        0        0    18407 2023-06-13 06:05:51.830071 pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/to_hetero_transformer.py
+-rw-r--r--   0        0        0    23103 2023-06-13 06:05:51.830071 pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/to_hetero_with_bases_transformer.py
+-rw-r--r--   0        0        0      102 2023-06-13 06:05:51.830071 pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/unpool/__init__.py
+-rw-r--r--   0        0        0     2586 2023-06-13 06:05:51.830071 pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/unpool/knn_interpolate.py
+-rw-r--r--   0        0        0      803 2023-06-13 06:05:51.830071 pyg_nightly-2.4.0.dev20230613/torch_geometric/profile/__init__.py
+-rw-r--r--   0        0        0     5110 2023-06-13 06:05:51.830071 pyg_nightly-2.4.0.dev20230613/torch_geometric/profile/benchmark.py
+-rw-r--r--   0        0        0    10364 2023-06-13 06:05:51.830071 pyg_nightly-2.4.0.dev20230613/torch_geometric/profile/profile.py
+-rw-r--r--   0        0        0    16665 2023-06-13 06:05:51.834071 pyg_nightly-2.4.0.dev20230613/torch_geometric/profile/profiler.py
+-rw-r--r--   0        0        0     4563 2023-06-13 06:05:51.834071 pyg_nightly-2.4.0.dev20230613/torch_geometric/profile/utils.py
+-rw-r--r--   0        0        0     1251 2023-06-13 06:05:51.834071 pyg_nightly-2.4.0.dev20230613/torch_geometric/resolver.py
+-rw-r--r--   0        0        0      481 2023-06-13 06:05:51.834071 pyg_nightly-2.4.0.dev20230613/torch_geometric/sampler/__init__.py
+-rw-r--r--   0        0        0    22762 2023-06-13 06:05:51.834071 pyg_nightly-2.4.0.dev20230613/torch_geometric/sampler/base.py
+-rw-r--r--   0        0        0     2734 2023-06-13 06:05:51.834071 pyg_nightly-2.4.0.dev20230613/torch_geometric/sampler/hgt_sampler.py
+-rw-r--r--   0        0        0    26480 2023-06-13 06:05:51.834071 pyg_nightly-2.4.0.dev20230613/torch_geometric/sampler/neighbor_sampler.py
+-rw-r--r--   0        0        0     5252 2023-06-13 06:05:51.834071 pyg_nightly-2.4.0.dev20230613/torch_geometric/sampler/utils.py
+-rw-r--r--   0        0        0      354 2023-06-13 06:05:51.834071 pyg_nightly-2.4.0.dev20230613/torch_geometric/seed.py
+-rw-r--r--   0        0        0      710 2023-06-13 06:05:51.834071 pyg_nightly-2.4.0.dev20230613/torch_geometric/testing/__init__.py
+-rw-r--r--   0        0        0     4368 2023-06-13 06:05:51.834071 pyg_nightly-2.4.0.dev20230613/torch_geometric/testing/asserts.py
+-rw-r--r--   0        0        0     1933 2023-06-13 06:05:51.834071 pyg_nightly-2.4.0.dev20230613/torch_geometric/testing/data.py
+-rw-r--r--   0        0        0     3842 2023-06-13 06:05:51.834071 pyg_nightly-2.4.0.dev20230613/torch_geometric/testing/decorators.py
+-rw-r--r--   0        0        0     1855 2023-06-13 06:05:51.834071 pyg_nightly-2.4.0.dev20230613/torch_geometric/testing/feature_store.py
+-rw-r--r--   0        0        0     1009 2023-06-13 06:05:51.834071 pyg_nightly-2.4.0.dev20230613/torch_geometric/testing/graph_store.py
+-rw-r--r--   0        0        0     4136 2023-06-13 06:05:51.834071 pyg_nightly-2.4.0.dev20230613/torch_geometric/transforms/__init__.py
+-rw-r--r--   0        0        0    13964 2023-06-13 06:05:51.834071 pyg_nightly-2.4.0.dev20230613/torch_geometric/transforms/add_metapaths.py
+-rw-r--r--   0        0        0     4836 2023-06-13 06:05:51.834071 pyg_nightly-2.4.0.dev20230613/torch_geometric/transforms/add_positional_encoding.py
+-rw-r--r--   0        0        0     2087 2023-06-13 06:05:51.834071 pyg_nightly-2.4.0.dev20230613/torch_geometric/transforms/add_remaining_self_loops.py
+-rw-r--r--   0        0        0     2018 2023-06-13 06:05:51.834071 pyg_nightly-2.4.0.dev20230613/torch_geometric/transforms/add_self_loops.py
+-rw-r--r--   0        0        0     1298 2023-06-13 06:05:51.834071 pyg_nightly-2.4.0.dev20230613/torch_geometric/transforms/base_transform.py
+-rw-r--r--   0        0        0     1936 2023-06-13 06:05:51.834071 pyg_nightly-2.4.0.dev20230613/torch_geometric/transforms/cartesian.py
+-rw-r--r--   0        0        0      640 2023-06-13 06:05:51.834071 pyg_nightly-2.4.0.dev20230613/torch_geometric/transforms/center.py
+-rw-r--r--   0        0        0     1658 2023-06-13 06:05:51.834071 pyg_nightly-2.4.0.dev20230613/torch_geometric/transforms/compose.py
+-rw-r--r--   0        0        0     1960 2023-06-13 06:05:51.834071 pyg_nightly-2.4.0.dev20230613/torch_geometric/transforms/constant.py
+-rw-r--r--   0        0        0     1222 2023-06-13 06:05:51.834071 pyg_nightly-2.4.0.dev20230613/torch_geometric/transforms/delaunay.py
+-rw-r--r--   0        0        0     1809 2023-06-13 06:05:51.834071 pyg_nightly-2.4.0.dev20230613/torch_geometric/transforms/distance.py
+-rw-r--r--   0        0        0     1034 2023-06-13 06:05:51.834071 pyg_nightly-2.4.0.dev20230613/torch_geometric/transforms/face_to_edge.py
+-rw-r--r--   0        0        0     2982 2023-06-13 06:05:51.834071 pyg_nightly-2.4.0.dev20230613/torch_geometric/transforms/feature_propagation.py
+-rw-r--r--   0        0        0     2367 2023-06-13 06:05:51.834071 pyg_nightly-2.4.0.dev20230613/torch_geometric/transforms/fixed_points.py
+-rw-r--r--   0        0        0     1397 2023-06-13 06:05:51.834071 pyg_nightly-2.4.0.dev20230613/torch_geometric/transforms/gcn_norm.py
+-rw-r--r--   0        0        0    24215 2023-06-13 06:05:51.834071 pyg_nightly-2.4.0.dev20230613/torch_geometric/transforms/gdc.py
+-rw-r--r--   0        0        0     1018 2023-06-13 06:05:51.834071 pyg_nightly-2.4.0.dev20230613/torch_geometric/transforms/generate_mesh_normals.py
+-rw-r--r--   0        0        0     2511 2023-06-13 06:05:51.834071 pyg_nightly-2.4.0.dev20230613/torch_geometric/transforms/grid_sampling.py
+-rw-r--r--   0        0        0     2543 2023-06-13 06:05:51.834071 pyg_nightly-2.4.0.dev20230613/torch_geometric/transforms/knn_graph.py
+-rw-r--r--   0        0        0     2465 2023-06-13 06:05:51.834071 pyg_nightly-2.4.0.dev20230613/torch_geometric/transforms/laplacian_lambda_max.py
+-rw-r--r--   0        0        0     2000 2023-06-13 06:05:51.834071 pyg_nightly-2.4.0.dev20230613/torch_geometric/transforms/largest_connected_components.py
+-rw-r--r--   0        0        0     3723 2023-06-13 06:05:51.834071 pyg_nightly-2.4.0.dev20230613/torch_geometric/transforms/line_graph.py
+-rw-r--r--   0        0        0     1996 2023-06-13 06:05:51.834071 pyg_nightly-2.4.0.dev20230613/torch_geometric/transforms/linear_transformation.py
+-rw-r--r--   0        0        0     1698 2023-06-13 06:05:51.834071 pyg_nightly-2.4.0.dev20230613/torch_geometric/transforms/local_cartesian.py
+-rw-r--r--   0        0        0     1404 2023-06-13 06:05:51.834071 pyg_nightly-2.4.0.dev20230613/torch_geometric/transforms/local_degree_profile.py
+-rw-r--r--   0        0        0     4598 2023-06-13 06:05:51.834071 pyg_nightly-2.4.0.dev20230613/torch_geometric/transforms/mask.py
+-rw-r--r--   0        0        0     6091 2023-06-13 06:05:51.834071 pyg_nightly-2.4.0.dev20230613/torch_geometric/transforms/node_property_split.py
+-rw-r--r--   0        0        0     1028 2023-06-13 06:05:51.834071 pyg_nightly-2.4.0.dev20230613/torch_geometric/transforms/normalize_features.py
+-rw-r--r--   0        0        0     1738 2023-06-13 06:05:51.834071 pyg_nightly-2.4.0.dev20230613/torch_geometric/transforms/normalize_rotation.py
+-rw-r--r--   0        0        0      620 2023-06-13 06:05:51.834071 pyg_nightly-2.4.0.dev20230613/torch_geometric/transforms/normalize_scale.py
+-rw-r--r--   0        0        0     1533 2023-06-13 06:05:51.834071 pyg_nightly-2.4.0.dev20230613/torch_geometric/transforms/one_hot_degree.py
+-rw-r--r--   0        0        0    21975 2023-06-13 06:05:51.834071 pyg_nightly-2.4.0.dev20230613/torch_geometric/transforms/pad.py
+-rw-r--r--   0        0        0     1793 2023-06-13 06:05:51.834071 pyg_nightly-2.4.0.dev20230613/torch_geometric/transforms/point_pair_features.py
+-rw-r--r--   0        0        0     2126 2023-06-13 06:05:51.834071 pyg_nightly-2.4.0.dev20230613/torch_geometric/transforms/polar.py
+-rw-r--r--   0        0        0     2050 2023-06-13 06:05:51.834071 pyg_nightly-2.4.0.dev20230613/torch_geometric/transforms/radius_graph.py
+-rw-r--r--   0        0        0      988 2023-06-13 06:05:51.834071 pyg_nightly-2.4.0.dev20230613/torch_geometric/transforms/random_flip.py
+-rw-r--r--   0        0        0     1510 2023-06-13 06:05:51.834071 pyg_nightly-2.4.0.dev20230613/torch_geometric/transforms/random_jitter.py
+-rw-r--r--   0        0        0    14297 2023-06-13 06:05:51.834071 pyg_nightly-2.4.0.dev20230613/torch_geometric/transforms/random_link_split.py
+-rw-r--r--   0        0        0     5768 2023-06-13 06:05:51.834071 pyg_nightly-2.4.0.dev20230613/torch_geometric/transforms/random_node_split.py
+-rw-r--r--   0        0        0     1903 2023-06-13 06:05:51.834071 pyg_nightly-2.4.0.dev20230613/torch_geometric/transforms/random_rotate.py
+-rw-r--r--   0        0        0     1215 2023-06-13 06:05:51.834071 pyg_nightly-2.4.0.dev20230613/torch_geometric/transforms/random_scale.py
+-rw-r--r--   0        0        0     1319 2023-06-13 06:05:51.834071 pyg_nightly-2.4.0.dev20230613/torch_geometric/transforms/random_shear.py
+-rw-r--r--   0        0        0     1805 2023-06-13 06:05:51.834071 pyg_nightly-2.4.0.dev20230613/torch_geometric/transforms/remove_duplicated_edges.py
+-rw-r--r--   0        0        0     2283 2023-06-13 06:05:51.834071 pyg_nightly-2.4.0.dev20230613/torch_geometric/transforms/remove_isolated_nodes.py
+-rw-r--r--   0        0        0      959 2023-06-13 06:05:51.834071 pyg_nightly-2.4.0.dev20230613/torch_geometric/transforms/remove_training_classes.py
+-rw-r--r--   0        0        0     6111 2023-06-13 06:05:51.834071 pyg_nightly-2.4.0.dev20230613/torch_geometric/transforms/rooted_subgraph.py
+-rw-r--r--   0        0        0     2140 2023-06-13 06:05:51.834071 pyg_nightly-2.4.0.dev20230613/torch_geometric/transforms/sample_points.py
+-rw-r--r--   0        0        0     2128 2023-06-13 06:05:51.834071 pyg_nightly-2.4.0.dev20230613/torch_geometric/transforms/sign.py
+-rw-r--r--   0        0        0     2241 2023-06-13 06:05:51.834071 pyg_nightly-2.4.0.dev20230613/torch_geometric/transforms/spherical.py
+-rw-r--r--   0        0        0     1002 2023-06-13 06:05:51.834071 pyg_nightly-2.4.0.dev20230613/torch_geometric/transforms/svd_feature_reduction.py
+-rw-r--r--   0        0        0     1607 2023-06-13 06:05:51.834071 pyg_nightly-2.4.0.dev20230613/torch_geometric/transforms/target_indegree.py
+-rw-r--r--   0        0        0     2327 2023-06-13 06:05:51.834071 pyg_nightly-2.4.0.dev20230613/torch_geometric/transforms/to_dense.py
+-rw-r--r--   0        0        0     1455 2023-06-13 06:05:51.834071 pyg_nightly-2.4.0.dev20230613/torch_geometric/transforms/to_device.py
+-rw-r--r--   0        0        0     5353 2023-06-13 06:05:51.834071 pyg_nightly-2.4.0.dev20230613/torch_geometric/transforms/to_sparse_tensor.py
+-rw-r--r--   0        0        0     2621 2023-06-13 06:05:51.834071 pyg_nightly-2.4.0.dev20230613/torch_geometric/transforms/to_superpixels.py
+-rw-r--r--   0        0        0     2972 2023-06-13 06:05:51.834071 pyg_nightly-2.4.0.dev20230613/torch_geometric/transforms/to_undirected.py
+-rw-r--r--   0        0        0     1214 2023-06-13 06:05:51.834071 pyg_nightly-2.4.0.dev20230613/torch_geometric/transforms/two_hop.py
+-rw-r--r--   0        0        0     2783 2023-06-13 06:05:51.834071 pyg_nightly-2.4.0.dev20230613/torch_geometric/transforms/virtual_node.py
+-rw-r--r--   0        0        0     9575 2023-06-13 06:05:51.834071 pyg_nightly-2.4.0.dev20230613/torch_geometric/typing.py
+-rw-r--r--   0        0        0     4549 2023-06-13 06:05:51.834071 pyg_nightly-2.4.0.dev20230613/torch_geometric/utils/__init__.py
+-rw-r--r--   0        0        0     2347 2023-06-13 06:05:51.834071 pyg_nightly-2.4.0.dev20230613/torch_geometric/utils/assortativity.py
+-rw-r--r--   0        0        0     9080 2023-06-13 06:05:51.838072 pyg_nightly-2.4.0.dev20230613/torch_geometric/utils/augmentation.py
+-rw-r--r--   0        0        0     5037 2023-06-13 06:05:51.838072 pyg_nightly-2.4.0.dev20230613/torch_geometric/utils/coalesce.py
+-rw-r--r--   0        0        0    19630 2023-06-13 06:05:51.838072 pyg_nightly-2.4.0.dev20230613/torch_geometric/utils/convert.py
+-rw-r--r--   0        0        0     2313 2023-06-13 06:05:51.838072 pyg_nightly-2.4.0.dev20230613/torch_geometric/utils/cross_entropy.py
+-rw-r--r--   0        0        0     1018 2023-06-13 06:05:51.838072 pyg_nightly-2.4.0.dev20230613/torch_geometric/utils/degree.py
+-rw-r--r--   0        0        0    11323 2023-06-13 06:05:51.838072 pyg_nightly-2.4.0.dev20230613/torch_geometric/utils/dropout.py
+-rw-r--r--   0        0        0     1657 2023-06-13 06:05:51.838072 pyg_nightly-2.4.0.dev20230613/torch_geometric/utils/embedding.py
+-rw-r--r--   0        0        0     4042 2023-06-13 06:05:51.838072 pyg_nightly-2.4.0.dev20230613/torch_geometric/utils/geodesic.py
+-rw-r--r--   0        0        0     3755 2023-06-13 06:05:51.838072 pyg_nightly-2.4.0.dev20230613/torch_geometric/utils/get_laplacian.py
+-rw-r--r--   0        0        0     4423 2023-06-13 06:05:51.838072 pyg_nightly-2.4.0.dev20230613/torch_geometric/utils/get_mesh_laplacian.py
+-rw-r--r--   0        0        0     2536 2023-06-13 06:05:51.838072 pyg_nightly-2.4.0.dev20230613/torch_geometric/utils/grid.py
+-rw-r--r--   0        0        0     9798 2023-06-13 06:05:51.838072 pyg_nightly-2.4.0.dev20230613/torch_geometric/utils/hetero.py
+-rw-r--r--   0        0        0     4818 2023-06-13 06:05:51.838072 pyg_nightly-2.4.0.dev20230613/torch_geometric/utils/homophily.py
+-rw-r--r--   0        0        0     3574 2023-06-13 06:05:51.838072 pyg_nightly-2.4.0.dev20230613/torch_geometric/utils/isolated.py
+-rw-r--r--   0        0        0    15855 2023-06-13 06:05:51.838072 pyg_nightly-2.4.0.dev20230613/torch_geometric/utils/loop.py
+-rw-r--r--   0        0        0     5200 2023-06-13 06:05:51.838072 pyg_nightly-2.4.0.dev20230613/torch_geometric/utils/map.py
+-rw-r--r--   0        0        0     1884 2023-06-13 06:05:51.838072 pyg_nightly-2.4.0.dev20230613/torch_geometric/utils/mask.py
+-rw-r--r--   0        0        0      608 2023-06-13 06:05:51.838072 pyg_nightly-2.4.0.dev20230613/torch_geometric/utils/mixin.py
+-rw-r--r--   0        0        0    14643 2023-06-13 06:05:51.838072 pyg_nightly-2.4.0.dev20230613/torch_geometric/utils/negative_sampling.py
+-rw-r--r--   0        0        0     3344 2023-06-13 06:05:51.838072 pyg_nightly-2.4.0.dev20230613/torch_geometric/utils/nested.py
+-rw-r--r--   0        0        0     1169 2023-06-13 06:05:51.838072 pyg_nightly-2.4.0.dev20230613/torch_geometric/utils/normalized_cut.py
+-rw-r--r--   0        0        0     1917 2023-06-13 06:05:51.838072 pyg_nightly-2.4.0.dev20230613/torch_geometric/utils/num_nodes.py
+-rw-r--r--   0        0        0     1404 2023-06-13 06:05:51.838072 pyg_nightly-2.4.0.dev20230613/torch_geometric/utils/one_hot.py
+-rw-r--r--   0        0        0     5154 2023-06-13 06:05:51.838072 pyg_nightly-2.4.0.dev20230613/torch_geometric/utils/random.py
+-rw-r--r--   0        0        0      815 2023-06-13 06:05:51.838072 pyg_nightly-2.4.0.dev20230613/torch_geometric/utils/repeat.py
+-rw-r--r--   0        0        0     8329 2023-06-13 06:05:51.838072 pyg_nightly-2.4.0.dev20230613/torch_geometric/utils/scatter.py
+-rw-r--r--   0        0        0     1110 2023-06-13 06:05:51.838072 pyg_nightly-2.4.0.dev20230613/torch_geometric/utils/segment.py
+-rw-r--r--   0        0        0     2149 2023-06-13 06:05:51.838072 pyg_nightly-2.4.0.dev20230613/torch_geometric/utils/select.py
+-rw-r--r--   0        0        0     6016 2023-06-13 06:05:51.838072 pyg_nightly-2.4.0.dev20230613/torch_geometric/utils/smiles.py
+-rw-r--r--   0        0        0     2718 2023-06-13 06:05:51.838072 pyg_nightly-2.4.0.dev20230613/torch_geometric/utils/softmax.py
+-rw-r--r--   0        0        0     1017 2023-06-13 06:05:51.838072 pyg_nightly-2.4.0.dev20230613/torch_geometric/utils/sort.py
+-rw-r--r--   0        0        0     3066 2023-06-13 06:05:51.838072 pyg_nightly-2.4.0.dev20230613/torch_geometric/utils/sort_edge_index.py
+-rw-r--r--   0        0        0    14860 2023-06-13 06:05:51.838072 pyg_nightly-2.4.0.dev20230613/torch_geometric/utils/sparse.py
+-rw-r--r--   0        0        0     5678 2023-06-13 06:05:51.838072 pyg_nightly-2.4.0.dev20230613/torch_geometric/utils/spmm.py
+-rw-r--r--   0        0        0    12370 2023-06-13 06:05:51.838072 pyg_nightly-2.4.0.dev20230613/torch_geometric/utils/subgraph.py
+-rw-r--r--   0        0        0     3439 2023-06-13 06:05:51.838072 pyg_nightly-2.4.0.dev20230613/torch_geometric/utils/to_dense_adj.py
+-rw-r--r--   0        0        0     4628 2023-06-13 06:05:51.838072 pyg_nightly-2.4.0.dev20230613/torch_geometric/utils/to_dense_batch.py
+-rw-r--r--   0        0        0     3489 2023-06-13 06:05:51.838072 pyg_nightly-2.4.0.dev20230613/torch_geometric/utils/train_test_split_edges.py
+-rw-r--r--   0        0        0     4867 2023-06-13 06:05:51.838072 pyg_nightly-2.4.0.dev20230613/torch_geometric/utils/tree_decomposition.py
+-rw-r--r--   0        0        0     6730 2023-06-13 06:05:51.838072 pyg_nightly-2.4.0.dev20230613/torch_geometric/utils/trim_to_layer.py
+-rw-r--r--   0        0        0     2125 2023-06-13 06:05:51.838072 pyg_nightly-2.4.0.dev20230613/torch_geometric/utils/unbatch.py
+-rw-r--r--   0        0        0     5770 2023-06-13 06:05:51.838072 pyg_nightly-2.4.0.dev20230613/torch_geometric/utils/undirected.py
+-rw-r--r--   0        0        0      123 2023-06-13 06:05:51.838072 pyg_nightly-2.4.0.dev20230613/torch_geometric/visualization/__init__.py
+-rw-r--r--   0        0        0     4149 2023-06-13 06:05:51.838072 pyg_nightly-2.4.0.dev20230613/torch_geometric/visualization/graph.py
+-rw-r--r--   0        0        0      388 2023-06-13 06:05:51.838072 pyg_nightly-2.4.0.dev20230613/torch_geometric/visualization/influence.py
+-rw-r--r--   0        0        0    63943 1970-01-01 00:00:00.000000 pyg_nightly-2.4.0.dev20230613/PKG-INFO
```

### Comparing `pyg_nightly-2.4.0.dev20230612/README.md` & `pyg_nightly-2.4.0.dev20230613/README.md`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/pyproject.toml` & `pyg_nightly-2.4.0.dev20230613/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires=["flit_core >=3.2,<4"]
 build-backend="flit_core.buildapi"
 
 [project]
 name="pyg-nightly"
-version="2.4.0.dev20230612"
+version="2.4.0.dev20230613"
 authors=[
     {name="Matthias Fey", email="matthias@pyg.org"},
 ]
 description="Graph Neural Network Library for PyTorch"
 readme="README.md"
 requires-python=">=3.7"
 keywords=[
```

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/__init__.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from .experimental import (is_experimental_mode_enabled, experimental_mode,
                            set_experimental_mode)
 from .lazy_loader import LazyLoader
 
 contrib = LazyLoader('contrib', globals(), 'torch_geometric.contrib')
 graphgym = LazyLoader('graphgym', globals(), 'torch_geometric.graphgym')
 
-__version__ = '2.4.0.dev20230612'
+__version__ = '2.4.0.dev20230613'
 
 __all__ = [
     'seed_everything',
     'get_home_dir',
     'set_home_dir',
     'compile',
     'is_debug_enabled',
```

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/compile.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/compile.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/contrib/explain/graphmask_explainer.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/contrib/explain/graphmask_explainer.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/contrib/explain/pgm_explainer.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/contrib/explain/pgm_explainer.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/contrib/nn/models/rbcd_attack.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/contrib/nn/models/rbcd_attack.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/data/__init__.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/data/__init__.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/data/batch.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/data/batch.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/data/collate.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/data/collate.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/data/data.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/data/data.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/data/datapipes.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/data/datapipes.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/data/dataset.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/data/dataset.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/data/download.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/data/download.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/data/extract.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/data/extract.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/data/feature_store.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/data/feature_store.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/data/graph_store.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/data/graph_store.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/data/hetero_data.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/data/hetero_data.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/data/in_memory_dataset.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/data/in_memory_dataset.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/data/lightning/datamodule.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/data/lightning/datamodule.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/data/remote_backend_utils.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/data/remote_backend_utils.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/data/separate.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/data/separate.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/data/storage.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/data/storage.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/data/summary.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/data/summary.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/data/temporal.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/data/temporal.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/data/view.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/data/view.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/datasets/__init__.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/datasets/actor.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/datasets/actor.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/datasets/airfrans.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/datasets/airfrans.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/datasets/airports.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/datasets/airports.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/datasets/amazon.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/datasets/amazon.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/datasets/amazon_book.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/datasets/amazon_book.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/datasets/amazon_products.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/datasets/amazon_products.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/datasets/aminer.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/datasets/aminer.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/datasets/aqsol.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/datasets/aqsol.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/datasets/attributed_graph_dataset.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/datasets/attributed_graph_dataset.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/datasets/ba2motif_dataset.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/datasets/ba2motif_dataset.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/datasets/ba_multi_shapes.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/datasets/ba_multi_shapes.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/datasets/ba_shapes.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/datasets/ba_shapes.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/datasets/bitcoin_otc.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/datasets/bitcoin_otc.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/datasets/citation_full.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/datasets/citation_full.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/datasets/coauthor.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/datasets/coauthor.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/datasets/coma.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/datasets/coma.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/datasets/dblp.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/datasets/dblp.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/datasets/dbp15k.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/datasets/dbp15k.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/datasets/deezer_europe.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/datasets/deezer_europe.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/datasets/dgraph.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/datasets/dgraph.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/datasets/dynamic_faust.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/datasets/dynamic_faust.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/datasets/elliptic.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/datasets/elliptic.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/datasets/elliptic_temporal.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/datasets/elliptic_temporal.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/datasets/email_eu_core.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/datasets/email_eu_core.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/datasets/entities.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/datasets/entities.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/datasets/explainer_dataset.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/datasets/explainer_dataset.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/datasets/facebook.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/datasets/facebook.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/datasets/fake.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/datasets/fake.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/datasets/faust.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/datasets/faust.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/datasets/flickr.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/datasets/flickr.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/datasets/freebase.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/datasets/freebase.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/datasets/gdelt.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/datasets/gdelt.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/datasets/gdelt_lite.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/datasets/gdelt_lite.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/datasets/ged_dataset.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/datasets/ged_dataset.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/datasets/gemsec.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/datasets/gemsec.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/datasets/geometry.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/datasets/geometry.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/datasets/github.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/datasets/github.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/datasets/gnn_benchmark_dataset.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/datasets/gnn_benchmark_dataset.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/datasets/graph_generator/ba_graph.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/datasets/graph_generator/ba_graph.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/datasets/graph_generator/base.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/datasets/graph_generator/base.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/datasets/graph_generator/er_graph.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/datasets/graph_generator/er_graph.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/datasets/graph_generator/grid_graph.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/datasets/graph_generator/grid_graph.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/datasets/heterophilous_graph_dataset.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/datasets/heterophilous_graph_dataset.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/datasets/hgb_dataset.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/datasets/hgb_dataset.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/datasets/hm.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/datasets/hm.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/datasets/hydro_net.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/datasets/hydro_net.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/datasets/icews.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/datasets/icews.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/datasets/igmc_dataset.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/datasets/igmc_dataset.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/datasets/imdb.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/datasets/imdb.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/datasets/infection_dataset.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/datasets/infection_dataset.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/datasets/jodie.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/datasets/jodie.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/datasets/karate.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/datasets/karate.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/datasets/last_fm.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/datasets/last_fm.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/datasets/lastfm_asia.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/datasets/lastfm_asia.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/datasets/linkx_dataset.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/datasets/linkx_dataset.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/datasets/lrgb.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/datasets/lrgb.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/datasets/malnet_tiny.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/datasets/malnet_tiny.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/datasets/md17.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/datasets/md17.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/datasets/mixhop_synthetic_dataset.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/datasets/mixhop_synthetic_dataset.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/datasets/mnist_superpixels.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/datasets/mnist_superpixels.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/datasets/modelnet.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/datasets/modelnet.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/datasets/molecule_net.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/datasets/molecule_net.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/datasets/motif_generator/base.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/datasets/motif_generator/base.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/datasets/motif_generator/custom.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/datasets/motif_generator/custom.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/datasets/motif_generator/cycle.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/datasets/motif_generator/cycle.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/datasets/motif_generator/house.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/datasets/motif_generator/house.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/datasets/movie_lens.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/datasets/movie_lens.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/datasets/movie_lens_100k.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/datasets/movie_lens_100k.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/datasets/movie_lens_1m.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/datasets/movie_lens_1m.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/datasets/nell.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/datasets/nell.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/datasets/ogb_mag.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/datasets/ogb_mag.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/datasets/omdb.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/datasets/omdb.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/datasets/particle.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/datasets/particle.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/datasets/pascal.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/datasets/pascal.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/datasets/pascal_pf.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/datasets/pascal_pf.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/datasets/pcpnet_dataset.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/datasets/pcpnet_dataset.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/datasets/planetoid.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/datasets/planetoid.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/datasets/polblogs.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/datasets/polblogs.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/datasets/ppi.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/datasets/ppi.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/datasets/qm7.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/datasets/qm7.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/datasets/qm9.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/datasets/qm9.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/datasets/reddit.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/datasets/reddit.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/datasets/reddit2.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/datasets/reddit2.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/datasets/rel_link_pred_dataset.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/datasets/rel_link_pred_dataset.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/datasets/s3dis.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/datasets/s3dis.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/datasets/sbm_dataset.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/datasets/sbm_dataset.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/datasets/shapenet.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/datasets/shapenet.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/datasets/shrec2016.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/datasets/shrec2016.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/datasets/snap_dataset.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/datasets/snap_dataset.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/datasets/suite_sparse.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/datasets/suite_sparse.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/datasets/taobao.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/datasets/taobao.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/datasets/tosca.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/datasets/tosca.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/datasets/tu_dataset.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/datasets/tu_dataset.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/datasets/twitch.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/datasets/twitch.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/datasets/upfd.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/datasets/upfd.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/datasets/utils/cheatsheet.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/datasets/utils/cheatsheet.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/datasets/webkb.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/datasets/webkb.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/datasets/wikics.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/datasets/wikics.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/datasets/wikipedia_network.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/datasets/wikipedia_network.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/datasets/willow_object_class.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/datasets/willow_object_class.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/datasets/word_net.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/datasets/word_net.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/datasets/yelp.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/datasets/yelp.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/datasets/zinc.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/datasets/zinc.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/debug.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/debug.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/deprecation.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/deprecation.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/experimental.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/experimental.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/explain/algorithm/attention_explainer.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/explain/algorithm/attention_explainer.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/explain/algorithm/base.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/explain/algorithm/base.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/explain/algorithm/captum.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/explain/algorithm/captum.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/explain/algorithm/captum_explainer.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/explain/algorithm/captum_explainer.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/explain/algorithm/dummy_explainer.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/explain/algorithm/dummy_explainer.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/explain/algorithm/gnn_explainer.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/explain/algorithm/gnn_explainer.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/explain/algorithm/pg_explainer.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/explain/algorithm/pg_explainer.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/explain/algorithm/utils.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/explain/algorithm/utils.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/explain/config.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/explain/config.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/explain/explainer.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/explain/explainer.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/explain/explanation.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/explain/explanation.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/explain/metric/basic.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/explain/metric/basic.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/explain/metric/faithfulness.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/explain/metric/faithfulness.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/explain/metric/fidelity.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/explain/metric/fidelity.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/graphgym/__init__.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/graphgym/__init__.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/graphgym/checkpoint.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/graphgym/checkpoint.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/graphgym/cmd_args.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/graphgym/cmd_args.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/graphgym/config.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/graphgym/config.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/graphgym/config_store.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/graphgym/config_store.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/graphgym/contrib/layer/generalconv.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/graphgym/contrib/layer/generalconv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/graphgym/loader.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/graphgym/loader.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/graphgym/logger.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/graphgym/logger.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/graphgym/loss.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/graphgym/loss.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/graphgym/model_builder.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/graphgym/model_builder.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/graphgym/models/__init__.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/graphgym/models/__init__.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/graphgym/models/act.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/graphgym/models/act.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/graphgym/models/encoder.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/graphgym/models/encoder.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/graphgym/models/gnn.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/graphgym/models/gnn.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/graphgym/models/head.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/graphgym/models/head.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/graphgym/models/layer.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/graphgym/models/layer.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/graphgym/models/transform.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/graphgym/models/transform.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/graphgym/optim.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/graphgym/optim.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/graphgym/register.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/graphgym/register.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/graphgym/train.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/graphgym/train.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/graphgym/utils/__init__.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/graphgym/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/graphgym/utils/agg_runs.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/graphgym/utils/agg_runs.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/graphgym/utils/comp_budget.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/graphgym/utils/comp_budget.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/graphgym/utils/device.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/graphgym/utils/device.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/graphgym/utils/epoch.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/graphgym/utils/epoch.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/graphgym/utils/io.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/graphgym/utils/io.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/graphgym/utils/plot.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/graphgym/utils/plot.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/home.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/home.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/io/__init__.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/io/__init__.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/io/npz.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/io/npz.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/io/obj.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/io/obj.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/io/off.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/io/off.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/io/planetoid.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/io/planetoid.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/io/sdf.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/io/sdf.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/io/tu.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/io/tu.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/io/txt_array.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/io/txt_array.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/lazy_loader.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/lazy_loader.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/loader/__init__.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/loader/__init__.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/loader/base.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/loader/base.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/loader/cluster.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/loader/cluster.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/loader/data_list_loader.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/loader/data_list_loader.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/loader/dataloader.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/loader/dataloader.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/loader/dense_data_loader.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/loader/dense_data_loader.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/loader/dynamic_batch_sampler.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/loader/dynamic_batch_sampler.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/loader/graph_saint.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/loader/graph_saint.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/loader/hgt_loader.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/loader/hgt_loader.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/loader/imbalanced_sampler.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/loader/imbalanced_sampler.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/loader/link_loader.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/loader/link_loader.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/loader/link_neighbor_loader.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/loader/link_neighbor_loader.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/loader/mixin.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/loader/mixin.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/loader/neighbor_loader.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/loader/neighbor_loader.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/loader/neighbor_sampler.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/loader/neighbor_sampler.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/loader/node_loader.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/loader/node_loader.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/loader/prefetch.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/loader/prefetch.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/loader/random_node_loader.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/loader/random_node_loader.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/loader/shadow.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/loader/shadow.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/loader/temporal_dataloader.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/loader/temporal_dataloader.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/loader/utils.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/loader/utils.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/loader/zip_loader.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/loader/zip_loader.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/logging.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/logging.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/__init__.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/__init__.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/aggr/__init__.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/aggr/__init__.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/aggr/attention.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/aggr/attention.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/aggr/base.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/aggr/base.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/aggr/basic.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/aggr/basic.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/aggr/deep_sets.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/aggr/deep_sets.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/aggr/equilibrium.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/aggr/equilibrium.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,30 +22,33 @@
         self.layers.append(torch.nn.Linear(sizes[-2], sizes[-1]))
 
         self.res_trans = torch.nn.ModuleList([
             torch.nn.Linear(in_channels, layer_size)
             for layer_size in num_layers + [out_channels]
         ])
 
-    def forward(self, x: Tensor, y: Tensor, index: Optional[Tensor]) -> Tensor:
+    def forward(self, x: Tensor, y: Tensor, index: Optional[Tensor],
+                dim_size: Optional[int] = None) -> Tensor:
         if index is None:
             inp = torch.cat([x, y.expand(x.size(0), -1)], dim=1)
         else:
             inp = torch.cat([x, y[index]], dim=1)
 
         h = inp
         for layer, res in zip(self.layers, self.res_trans):
             h = layer(h)
             h = res(inp) + h
 
         if index is None:
             return h.mean()
 
-        size = int(index.max().item() + 1)
-        return scatter(h, index, dim=0, dim_size=size, reduce='mean').sum()
+        if dim_size is None:
+            dim_size = int(index.max().item() + 1)
+
+        return scatter(h, index, 0, dim_size, reduce='mean').sum()
 
 
 class MomentumOptimizer(torch.nn.Module):
     r"""
     Provides an inner loop optimizer for the implicitly defined output
     layer. It is based on an unrolled Nesterov momentum algorithm.
 
@@ -82,21 +85,22 @@
         return self.sigmoid(self._mom)
 
     def forward(
         self,
         x: Tensor,
         y: Tensor,
         index: Optional[Tensor],
+        dim_size: Optional[int],
         func: Callable[[Tensor, Tensor, Optional[Tensor]], Tensor],
         iterations: int = 5,
     ) -> Tuple[Tensor, float]:
 
         momentum_buffer = torch.zeros_like(y)
         for _ in range(iterations):
-            val = func(x, y, index)
+            val = func(x, y, index, dim_size)
             grad = torch.autograd.grad(val, y, create_graph=True,
                                        retain_graph=True)[0]
             delta = self.learning_rate * grad
             momentum_buffer = self.momentum * momentum_buffer - delta
             y = y + momentum_buffer
         return y
 
@@ -149,26 +153,27 @@
     def init_output(self, dim_size: int) -> Tensor:
         return torch.zeros(dim_size, self.output_dim, requires_grad=True,
                            device=self.lamb.device).float()
 
     def reg(self, y: Tensor) -> Tensor:
         return self.softplus(self.lamb) * y.square().sum(dim=-1).mean()
 
-    def energy(self, x: Tensor, y: Tensor, index: Optional[Tensor]):
-        return self.potential(x, y, index) + self.reg(y)
+    def energy(self, x: Tensor, y: Tensor, index: Optional[Tensor],
+               dim_size: Optional[int] = None):
+        return self.potential(x, y, index, dim_size) + self.reg(y)
 
     def forward(self, x: Tensor, index: Optional[Tensor] = None,
                 ptr: Optional[Tensor] = None, dim_size: Optional[int] = None,
                 dim: int = -2) -> Tensor:
 
         self.assert_index_present(index)
 
         dim_size = int(index.max()) + 1 if dim_size is None else dim_size
 
         with torch.enable_grad():
-            y = self.optimizer(x, self.init_output(dim_size), index,
+            y = self.optimizer(x, self.init_output(dim_size), index, dim_size,
                                self.energy, iterations=self.grad_iter)
 
         return y
 
     def __repr__(self) -> str:
         return (f'{self.__class__.__name__}()')
```

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/aggr/fused.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/aggr/fused.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/aggr/gmt.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/aggr/gmt.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/aggr/gru.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/aggr/gru.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/aggr/lstm.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/aggr/lstm.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/aggr/mlp.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/aggr/mlp.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/aggr/multi.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/aggr/multi.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/aggr/quantile.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/aggr/quantile.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/aggr/scaler.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/aggr/scaler.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/aggr/set2set.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/aggr/set2set.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/aggr/set_transformer.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/aggr/set_transformer.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/aggr/sort.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/aggr/sort.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/aggr/utils.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/aggr/utils.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/attention/performer.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/attention/performer.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/conv/__init__.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/conv/__init__.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/conv/agnn_conv.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/conv/agnn_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/conv/antisymmetric_conv.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/conv/antisymmetric_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/conv/appnp.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/conv/appnp.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/conv/arma_conv.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/conv/arma_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/conv/cg_conv.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/conv/cg_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/conv/cheb_conv.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/conv/cheb_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/conv/cluster_gcn_conv.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/conv/cluster_gcn_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/conv/cugraph/base.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/conv/cugraph/base.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/conv/cugraph/gat_conv.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/conv/cugraph/gat_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/conv/cugraph/rgcn_conv.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/conv/cugraph/rgcn_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/conv/cugraph/sage_conv.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/conv/cugraph/sage_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/conv/dna_conv.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/conv/dna_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/conv/edge_conv.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/conv/edge_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/conv/eg_conv.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/conv/eg_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/conv/fa_conv.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/conv/fa_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/conv/feast_conv.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/conv/feast_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/conv/film_conv.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/conv/film_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/conv/fused_gat_conv.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/conv/fused_gat_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/conv/gat_conv.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/conv/gat_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/conv/gated_graph_conv.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/conv/gated_graph_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/conv/gatv2_conv.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/conv/gatv2_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/conv/gcn2_conv.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/conv/gcn2_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/conv/gcn_conv.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/conv/gcn_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/conv/gen_conv.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/conv/gen_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/conv/general_conv.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/conv/general_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/conv/gin_conv.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/conv/gin_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/conv/gmm_conv.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/conv/gmm_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/conv/gps_conv.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/conv/gps_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/conv/graph_conv.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/conv/graph_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/conv/gravnet_conv.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/conv/gravnet_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/conv/han_conv.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/conv/han_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/conv/heat_conv.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/conv/heat_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/conv/hetero_conv.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/conv/hetero_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/conv/hgt_conv.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/conv/hgt_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/conv/hypergraph_conv.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/conv/hypergraph_conv.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from typing import Optional
 
 import torch
 import torch.nn.functional as F
 from torch import Tensor
 from torch.nn import Parameter
 
+from torch_geometric.experimental import disable_dynamic_shapes
 from torch_geometric.nn.conv import MessagePassing
 from torch_geometric.nn.dense.linear import Linear
 from torch_geometric.nn.inits import glorot, zeros
 from torch_geometric.utils import scatter, softmax
 
 
 class HypergraphConv(MessagePassing):
@@ -103,17 +104,19 @@
     def reset_parameters(self):
         super().reset_parameters()
         self.lin.reset_parameters()
         if self.use_attention:
             glorot(self.att)
         zeros(self.bias)
 
+    @disable_dynamic_shapes(required_args=['num_edges'])
     def forward(self, x: Tensor, hyperedge_index: Tensor,
                 hyperedge_weight: Optional[Tensor] = None,
-                hyperedge_attr: Optional[Tensor] = None) -> Tensor:
+                hyperedge_attr: Optional[Tensor] = None,
+                num_edges: Optional[int] = None) -> Tensor:
         r"""Runs the forward pass of the module.
 
         Args:
             x (torch.Tensor): Node feature matrix
                 :math:`\mathbf{X} \in \mathbb{R}^{N \times F}`.
             hyperedge_index (torch.Tensor): The hyperedge indices, *i.e.*
                 the sparse incidence matrix
@@ -121,18 +124,23 @@
                 nodes to edges.
             hyperedge_weight (torch.Tensor, optional): Hyperedge weights
                 :math:`\mathbf{W} \in \mathbb{R}^M`. (default: :obj:`None`)
             hyperedge_attr (torch.Tensor, optional): Hyperedge feature matrix
                 in :math:`\mathbb{R}^{M \times F}`.
                 These features only need to get passed in case
                 :obj:`use_attention=True`. (default: :obj:`None`)
+            num_edges (int, optional) : The number of edges :math:`M`.
+                (default: :obj:`None`)
         """
-        num_nodes, num_edges = x.size(0), 0
-        if hyperedge_index.numel() > 0:
-            num_edges = int(hyperedge_index[1].max()) + 1
+        num_nodes = x.size(0)
+
+        if num_edges is None:
+            num_edges = 0
+            if hyperedge_index.numel() > 0:
+                num_edges = int(hyperedge_index[1].max()) + 1
 
         if hyperedge_weight is None:
             hyperedge_weight = x.new_ones(num_edges)
 
         x = self.lin(x)
 
         alpha = None
```

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/conv/le_conv.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/conv/le_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/conv/lg_conv.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/conv/lg_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/conv/message_passing.jinja` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/conv/message_passing.jinja`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/conv/message_passing.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/conv/message_passing.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/conv/mf_conv.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/conv/mf_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/conv/nn_conv.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/conv/nn_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/conv/pan_conv.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/conv/pan_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/conv/pdn_conv.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/conv/pdn_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/conv/pna_conv.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/conv/pna_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/conv/point_conv.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/conv/point_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/conv/point_gnn_conv.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/conv/point_gnn_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/conv/point_transformer_conv.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/conv/point_transformer_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/conv/ppf_conv.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/conv/ppf_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/conv/res_gated_graph_conv.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/conv/res_gated_graph_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/conv/rgat_conv.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/conv/rgat_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/conv/rgcn_conv.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/conv/rgcn_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/conv/sage_conv.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/conv/sage_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/conv/sg_conv.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/conv/sg_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/conv/signed_conv.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/conv/signed_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/conv/simple_conv.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/conv/simple_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/conv/spline_conv.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/conv/spline_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/conv/ssg_conv.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/conv/ssg_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/conv/supergat_conv.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/conv/supergat_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/conv/tag_conv.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/conv/tag_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/conv/transformer_conv.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/conv/transformer_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/conv/utils/__init__.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/conv/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/conv/utils/cheatsheet.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/conv/utils/cheatsheet.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/conv/utils/inspector.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/conv/utils/inspector.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/conv/utils/jit.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/conv/utils/jit.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/conv/utils/typing.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/conv/utils/typing.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/conv/wl_conv.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/conv/wl_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/conv/wl_conv_continuous.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/conv/wl_conv_continuous.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/conv/x_conv.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/conv/x_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/data_parallel.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/data_parallel.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/dense/__init__.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/dense/__init__.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/dense/dense_gat_conv.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/dense/dense_gat_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/dense/dense_gcn_conv.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/dense/dense_gcn_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/dense/dense_gin_conv.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/dense/dense_gin_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/dense/dense_graph_conv.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/dense/dense_graph_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/dense/dense_sage_conv.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/dense/dense_sage_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/dense/diff_pool.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/dense/diff_pool.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/dense/dmon_pool.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/dense/dmon_pool.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/dense/linear.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/dense/linear.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/dense/mincut_pool.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/dense/mincut_pool.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/encoding.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/encoding.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/functional/bro.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/functional/bro.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/functional/gini.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/functional/gini.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/fx.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/fx.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/glob.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/glob.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/inits.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/inits.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/kge/base.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/kge/base.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/kge/complex.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/kge/complex.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/kge/distmult.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/kge/distmult.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/kge/loader.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/kge/loader.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/kge/rotate.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/kge/rotate.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/kge/transe.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/kge/transe.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/lr_scheduler.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/lr_scheduler.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/model_hub.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/model_hub.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/models/__init__.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/models/__init__.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/models/attentive_fp.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/models/attentive_fp.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/models/autoencoder.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/models/autoencoder.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/models/basic_gnn.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/models/basic_gnn.py`

 * *Files 3% similar despite different names*

```diff
@@ -237,61 +237,78 @@
                 xs.append(x)
 
         x = self.jk(xs) if hasattr(self, 'jk') else x
         x = self.lin(x) if hasattr(self, 'lin') else x
         return x
 
     @torch.no_grad()
-    def inference(self, loader: NeighborLoader,
-                  device: Optional[torch.device] = None,
-                  progress_bar: bool = False) -> Tensor:
+    def inference(
+        self,
+        loader: NeighborLoader,
+        device: Optional[Union[str, torch.device]] = None,
+        embedding_device: Union[str, torch.device] = 'cpu',
+        progress_bar: bool = False,
+    ) -> Tensor:
         r"""Performs layer-wise inference on large-graphs using a
         :class:`~torch_geometric.loader.NeighborLoader`, where
         :class:`~torch_geometric.loader.NeighborLoader` should sample the
         full neighborhood for only one layer.
         This is an efficient way to compute the output embeddings for all
         nodes in the graph.
         Only applicable in case :obj:`jk=None` or `jk='last'`.
+
+        Args:
+            loader (torch_geometric.loader.NeighborLoader): A neighbor loader
+                object that generates full 1-hop subgraphs, *i.e.*,
+                :obj:`loader.num_neighbors = [-1]`.
+            device (torch.device, optional): The device to run the GNN on.
+                (default: :obj:`None`)
+            embedding_device (torch.device, optional): The device to store
+                intermediate embeddings on. If intermediate embeddings fit on
+                GPU, this option helps to avoid unnecessary device transfers.
+                (default: :obj:`"cpu"`)
+            progress_bar (bool, optional): If set to :obj:`True`, will print a
+                progress bar during computation. (default: :obj:`False`)
         """
         assert self.jk_mode is None or self.jk_mode == 'last'
         assert isinstance(loader, NeighborLoader)
         assert len(loader.dataset) == loader.data.num_nodes
         assert len(loader.node_sampler.num_neighbors) == 1
         assert not self.training
         # assert not loader.shuffle  # TODO (matthias) does not work :(
         if progress_bar:
             pbar = tqdm(total=len(self.convs) * len(loader))
             pbar.set_description('Inference')
 
-        x_all = loader.data.x.cpu()
+        x_all = loader.data.x.to(embedding_device)
         loader.data.n_id = torch.arange(x_all.size(0))
 
         for i in range(self.num_layers):
             xs: List[Tensor] = []
             for batch in loader:
                 x = x_all[batch.n_id].to(device)
                 if hasattr(batch, 'adj_t'):
                     edge_index = batch.adj_t.to(device)
                 else:
                     edge_index = batch.edge_index.to(device)
                 x = self.convs[i](x, edge_index)[:batch.batch_size]
                 if i == self.num_layers - 1 and self.jk_mode is None:
-                    xs.append(x.cpu())
+                    xs.append(x.to(embedding_device))
                     if progress_bar:
                         pbar.update(1)
                     continue
                 if self.act is not None and self.act_first:
                     x = self.act(x)
                 if self.norms is not None:
                     x = self.norms[i](x)
                 if self.act is not None and not self.act_first:
                     x = self.act(x)
                 if i == self.num_layers - 1 and hasattr(self, 'lin'):
                     x = self.lin(x)
-                xs.append(x.cpu())
+                xs.append(x.to(embedding_device))
                 if progress_bar:
                     pbar.update(1)
             x_all = torch.cat(xs, dim=0)
         if progress_bar:
             pbar.close()
         del loader.data.n_id
```

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/models/captum.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/models/captum.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/models/correct_and_smooth.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/models/correct_and_smooth.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/models/deep_graph_infomax.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/models/deep_graph_infomax.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/models/deepgcn.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/models/deepgcn.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/models/dimenet.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/models/dimenet.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/models/dimenet_utils.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/models/dimenet_utils.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/models/gnnff.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/models/gnnff.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/models/graph_mixer.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/models/graph_mixer.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/models/graph_unet.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/models/graph_unet.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/models/jumping_knowledge.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/models/jumping_knowledge.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/models/label_prop.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/models/label_prop.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/models/lightgcn.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/models/lightgcn.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/models/linkx.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/models/linkx.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/models/mask_label.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/models/mask_label.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/models/meta.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/models/meta.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/models/metapath2vec.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/models/metapath2vec.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/models/mlp.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/models/mlp.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/models/node2vec.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/models/node2vec.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/models/pmlp.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/models/pmlp.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,24 +18,27 @@
     Args:
         in_channels (int): Size of each input sample.
         hidden_channels (int): Size of each hidden sample.
         out_channels (int): Size of each output sample.
         num_layers (int): The number of layers.
         dropout (float, optional): Dropout probability of each hidden
             embedding. (default: :obj:`0.`)
+        norm (bool, optional): If set to :obj:`False`, will not apply batch
+            normalization. (default: :obj:`True`)
         bias (bool, optional): If set to :obj:`False`, the module
             will not learn additive biases. (default: :obj:`True`)
     """
     def __init__(
         self,
         in_channels: int,
         hidden_channels: int,
         out_channels: int,
         num_layers: int,
         dropout: float = 0.,
+        norm: bool = True,
         bias: bool = True,
     ):
         super().__init__()
 
         self.in_channels = in_channels
         self.hidden_channels = hidden_channels
         self.out_channels = out_channels
@@ -46,16 +49,21 @@
         self.lins = torch.nn.ModuleList()
         self.lins.append(Linear(in_channels, hidden_channels, self.bias))
         for _ in range(self.num_layers - 2):
             lin = Linear(hidden_channels, hidden_channels, self.bias)
             self.lins.append(lin)
         self.lins.append(Linear(hidden_channels, out_channels, self.bias))
 
-        self.norm = torch.nn.BatchNorm1d(hidden_channels, affine=False,
-                                         track_running_stats=False)
+        self.norm = None
+        if norm:
+            self.norm = torch.nn.BatchNorm1d(
+                hidden_channels,
+                affine=False,
+                track_running_stats=False,
+            )
 
         self.conv = SimpleConv(aggr='mean', combine_root='self_loop')
 
         self.reset_parameters()
 
     def reset_parameters(self):
         r"""Resets all learnable parameters of the module."""
@@ -77,15 +85,16 @@
         for i in range(self.num_layers):
             x = x @ self.lins[i].weight.t()
             if not self.training:
                 x = self.conv(x, edge_index)
             if self.bias:
                 x = x + self.lins[i].bias
             if i != self.num_layers - 1:
-                x = self.norm(x)
+                if self.norm is not None:
+                    x = self.norm(x)
                 x = x.relu()
                 x = F.dropout(x, p=self.dropout, training=self.training)
 
         return x
 
     def __repr__(self) -> str:
         return (f'{self.__class__.__name__}({self.in_channels}, '
```

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/models/re_net.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/models/re_net.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/models/rect.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/models/rect.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/models/rev_gnn.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/models/rev_gnn.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/models/schnet.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/models/schnet.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/models/signed_gcn.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/models/signed_gcn.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/models/tgn.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/models/tgn.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/module_dict.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/module_dict.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/norm/__init__.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/norm/__init__.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/norm/batch_norm.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/norm/batch_norm.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/norm/diff_group_norm.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/norm/diff_group_norm.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/norm/graph_norm.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/norm/graph_norm.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/norm/graph_size_norm.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/norm/graph_size_norm.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/norm/instance_norm.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/norm/instance_norm.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/norm/layer_norm.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/norm/layer_norm.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/norm/mean_subtraction_norm.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/norm/mean_subtraction_norm.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/norm/msg_norm.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/norm/msg_norm.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/norm/pair_norm.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/norm/pair_norm.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/parameter_dict.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/parameter_dict.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/pool/__init__.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/pool/__init__.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/pool/approx_knn.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/pool/approx_knn.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/pool/asap.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/pool/asap.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/pool/avg_pool.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/pool/avg_pool.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/pool/connect/base.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/pool/connect/base.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/pool/decimation.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/pool/decimation.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/pool/edge_pool.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/pool/edge_pool.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/pool/glob.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/pool/glob.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/pool/graclus.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/pool/graclus.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/pool/max_pool.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/pool/max_pool.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/pool/mem_pool.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/pool/mem_pool.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/pool/pan_pool.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/pool/pan_pool.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/pool/pool.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/pool/pool.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/pool/sag_pool.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/pool/sag_pool.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/pool/select/base.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/pool/select/base.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/pool/select/topk.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/pool/select/topk.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/pool/topk_pool.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/pool/topk_pool.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/pool/voxel_grid.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/pool/voxel_grid.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/resolver.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/resolver.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/sequential.jinja` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/sequential.jinja`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/sequential.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/sequential.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/summary.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/summary.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/to_fixed_size_transformer.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/to_fixed_size_transformer.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/to_hetero_module.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/to_hetero_module.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/to_hetero_transformer.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/to_hetero_transformer.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/to_hetero_with_bases_transformer.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/to_hetero_with_bases_transformer.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/nn/unpool/knn_interpolate.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/nn/unpool/knn_interpolate.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/profile/__init__.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/profile/__init__.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/profile/benchmark.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/profile/benchmark.py`

 * *Files 12% similar despite different names*

```diff
@@ -23,14 +23,16 @@
 def benchmark(
     funcs: List[Callable],
     args: Union[Tuple[Any], List[Tuple[Any]]],
     num_steps: int,
     func_names: Optional[List[str]] = None,
     num_warmups: int = 10,
     backward: bool = False,
+    per_step: bool = False,
+    progress_bar: bool = False,
 ):
     r"""Benchmark a list of functions :obj:`funcs` that receive the same set
     of arguments :obj:`args`.
 
     Args:
         funcs ([Callable]): The list of functions to benchmark.
         args ((Any, ) or [(Any, )]): The arguments to pass to the functions.
@@ -40,14 +42,18 @@
         func_names ([str], optional): The names of the functions. If not given,
             will try to infer the name from the function itself.
             (default: :obj:`None`)
         num_warmups (int, optional): The number of warmup steps.
             (default: :obj:`10`)
         backward (bool, optional): If set to :obj:`True`, will benchmark both
             forward and backward passes. (default: :obj:`False`)
+        per_step (bool, optional): If set to :obj:`True`, will report runtimes
+            per step. (default: :obj:`False`)
+        progress_bar (bool, optional): If set to :obj:`True`, will print a
+            progress bar during benchmarking. (default: :obj:`False`)
     """
     from tabulate import tabulate
 
     if num_steps <= 0:
         raise ValueError(f"'num_steps' must be a positive integer "
                          f"(got {num_steps})")
 
@@ -61,16 +67,21 @@
     if len(funcs) != len(func_names):
         raise ValueError(f"Length of 'funcs' (got {len(funcs)}) and "
                          f"'func_names' (got {len(func_names)}) must be equal")
 
     # Zero-copy `args` for each function (if necessary):
     args_list = [args] * len(funcs) if isinstance(args, tuple) else args
 
+    iterator = zip(funcs, args_list, func_names)
+    if progress_bar:
+        from tqdm import tqdm
+        iterator = tqdm(iterator, total=len(funcs))
+
     ts: List[List[str]] = []
-    for func, args, name in zip(funcs, args_list, func_names):
+    for func, args, name in iterator:
         t_forward = t_backward = 0
         for i in range(num_warmups + num_steps):
             args = require_grad(args, backward)
 
             if torch.cuda.is_available():
                 torch.cuda.synchronize()
             t_start = time.perf_counter()
@@ -96,18 +107,25 @@
                 out.backward(out_grad)
 
                 if torch.cuda.is_available():
                     torch.cuda.synchronize()
                 if i >= num_warmups:
                     t_backward += time.perf_counter() - t_start
 
-        ts.append([name, f'{t_forward:.4f}s'])
+        if per_step:
+            ts.append([name, f'{t_forward/num_steps:.6f}s'])
+        else:
+            ts.append([name, f'{t_forward:.4f}s'])
         if backward:
-            ts[-1].append(f'{t_backward:.4f}s')
-            ts[-1].append(f'{t_forward + t_backward:.4f}s')
+            if per_step:
+                ts[-1].append(f'{t_backward/num_steps:.6f}s')
+                ts[-1].append(f'{(t_forward + t_backward)/num_steps:.6f}s')
+            else:
+                ts[-1].append(f'{t_backward:.4f}s')
+                ts[-1].append(f'{t_forward + t_backward:.4f}s')
 
     header = ['Name', 'Forward']
     if backward:
         header.extend(['Backward', 'Total'])
 
     print(tabulate(ts, headers=header, tablefmt='psql'))
```

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/profile/profile.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/profile/profile.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/profile/profiler.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/profile/profiler.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/profile/utils.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/profile/utils.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/resolver.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/resolver.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/sampler/base.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/sampler/base.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/sampler/hgt_sampler.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/sampler/hgt_sampler.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/sampler/neighbor_sampler.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/sampler/neighbor_sampler.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/sampler/utils.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/sampler/utils.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/testing/__init__.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/testing/asserts.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/testing/asserts.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/testing/data.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/testing/data.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/testing/decorators.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/testing/decorators.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/testing/feature_store.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/testing/feature_store.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/testing/graph_store.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/testing/graph_store.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/transforms/__init__.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/transforms/__init__.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/transforms/add_metapaths.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/transforms/add_metapaths.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/transforms/add_positional_encoding.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/transforms/add_positional_encoding.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/transforms/add_remaining_self_loops.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/transforms/add_remaining_self_loops.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/transforms/add_self_loops.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/transforms/add_self_loops.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/transforms/base_transform.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/transforms/base_transform.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/transforms/cartesian.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/transforms/cartesian.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/transforms/center.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/transforms/center.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/transforms/compose.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/transforms/compose.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/transforms/constant.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/transforms/constant.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/transforms/delaunay.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/transforms/delaunay.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/transforms/distance.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/transforms/distance.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/transforms/face_to_edge.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/transforms/face_to_edge.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/transforms/feature_propagation.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/transforms/feature_propagation.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/transforms/fixed_points.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/transforms/fixed_points.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/transforms/gcn_norm.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/transforms/gcn_norm.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/transforms/gdc.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/transforms/gdc.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/transforms/generate_mesh_normals.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/transforms/generate_mesh_normals.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/transforms/grid_sampling.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/transforms/grid_sampling.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/transforms/knn_graph.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/transforms/knn_graph.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/transforms/laplacian_lambda_max.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/transforms/laplacian_lambda_max.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/transforms/largest_connected_components.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/transforms/largest_connected_components.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/transforms/line_graph.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/transforms/line_graph.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/transforms/linear_transformation.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/transforms/linear_transformation.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/transforms/local_cartesian.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/transforms/local_cartesian.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/transforms/local_degree_profile.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/transforms/local_degree_profile.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/transforms/mask.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/transforms/mask.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/transforms/node_property_split.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/transforms/node_property_split.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/transforms/normalize_features.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/transforms/normalize_features.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/transforms/normalize_rotation.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/transforms/normalize_rotation.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/transforms/normalize_scale.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/transforms/normalize_scale.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/transforms/one_hot_degree.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/transforms/one_hot_degree.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/transforms/pad.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/transforms/pad.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/transforms/point_pair_features.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/transforms/point_pair_features.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/transforms/polar.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/transforms/polar.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/transforms/radius_graph.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/transforms/radius_graph.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/transforms/random_flip.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/transforms/random_flip.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/transforms/random_jitter.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/transforms/random_jitter.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/transforms/random_link_split.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/transforms/random_link_split.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/transforms/random_node_split.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/transforms/random_node_split.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/transforms/random_rotate.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/transforms/random_rotate.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/transforms/random_scale.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/transforms/random_scale.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/transforms/random_shear.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/transforms/random_shear.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/transforms/remove_duplicated_edges.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/transforms/remove_duplicated_edges.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/transforms/remove_isolated_nodes.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/transforms/remove_isolated_nodes.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/transforms/remove_training_classes.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/transforms/remove_training_classes.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/transforms/rooted_subgraph.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/transforms/rooted_subgraph.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/transforms/sample_points.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/transforms/sample_points.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/transforms/sign.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/transforms/sign.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/transforms/spherical.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/transforms/spherical.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/transforms/svd_feature_reduction.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/transforms/svd_feature_reduction.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/transforms/target_indegree.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/transforms/target_indegree.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/transforms/to_dense.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/transforms/to_dense.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/transforms/to_device.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/transforms/to_device.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/transforms/to_sparse_tensor.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/transforms/to_sparse_tensor.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/transforms/to_superpixels.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/transforms/to_superpixels.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/transforms/to_undirected.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/transforms/to_undirected.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/transforms/two_hop.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/transforms/two_hop.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/transforms/virtual_node.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/transforms/virtual_node.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/typing.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/typing.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/utils/__init__.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/utils/assortativity.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/utils/assortativity.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/utils/augmentation.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/utils/augmentation.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/utils/coalesce.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/utils/coalesce.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/utils/convert.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/utils/convert.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/utils/cross_entropy.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/utils/cross_entropy.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/utils/degree.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/utils/degree.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/utils/dropout.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/utils/dropout.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/utils/embedding.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/utils/embedding.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/utils/geodesic.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/utils/geodesic.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/utils/get_laplacian.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/utils/get_laplacian.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/utils/get_mesh_laplacian.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/utils/get_mesh_laplacian.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/utils/grid.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/utils/grid.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/utils/hetero.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/utils/hetero.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/utils/homophily.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/utils/homophily.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/utils/isolated.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/utils/isolated.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/utils/loop.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/utils/loop.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/utils/map.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/utils/map.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/utils/mask.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/utils/mask.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/utils/mixin.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/utils/mixin.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/utils/negative_sampling.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/utils/negative_sampling.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/utils/nested.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/utils/nested.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/utils/normalized_cut.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/utils/normalized_cut.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/utils/num_nodes.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/utils/num_nodes.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/utils/one_hot.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/utils/one_hot.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/utils/random.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/utils/random.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/utils/repeat.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/utils/repeat.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/utils/scatter.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/utils/scatter.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/utils/segment.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/utils/segment.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/utils/select.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/utils/select.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/utils/smiles.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/utils/smiles.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/utils/softmax.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/utils/softmax.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/utils/sort.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/utils/sort.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/utils/sort_edge_index.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/utils/sort_edge_index.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/utils/sparse.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/utils/sparse.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/utils/spmm.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/utils/spmm.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/utils/subgraph.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/utils/subgraph.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/utils/to_dense_adj.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/utils/to_dense_adj.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/utils/to_dense_batch.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/utils/to_dense_batch.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/utils/train_test_split_edges.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/utils/train_test_split_edges.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/utils/tree_decomposition.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/utils/tree_decomposition.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/utils/trim_to_layer.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/utils/trim_to_layer.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/utils/unbatch.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/utils/unbatch.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/utils/undirected.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/utils/undirected.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/torch_geometric/visualization/graph.py` & `pyg_nightly-2.4.0.dev20230613/torch_geometric/visualization/graph.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230612/PKG-INFO` & `pyg_nightly-2.4.0.dev20230613/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyg-nightly
-Version: 2.4.0.dev20230612
+Version: 2.4.0.dev20230613
 Summary: Graph Neural Network Library for PyTorch
 Keywords: deep-learning,pytorch,geometric-deep-learning,graph-neural-networks,graph-convolutional-networks
 Author-email: Matthias Fey <matthias@pyg.org>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
```

