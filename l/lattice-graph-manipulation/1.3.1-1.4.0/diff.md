# Comparing `tmp/Lattice-Graph-Manipulation-1.3.1.tar.gz` & `tmp/Lattice-Graph-Manipulation-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Lattice-Graph-Manipulation-1.3.1.tar", last modified: Mon Jun 12 16:17:45 2023, max compression
+gzip compressed data, was "Lattice-Graph-Manipulation-1.4.0.tar", last modified: Wed Jun 14 01:08:42 2023, max compression
```

## Comparing `Lattice-Graph-Manipulation-1.3.1.tar` & `Lattice-Graph-Manipulation-1.4.0.tar`

### file list

```diff
@@ -1,91 +1,91 @@
--rw-r--r--   0        0        0     1070 2023-04-30 13:12:10.136468 Lattice-Graph-Manipulation-1.3.1/LICENSE
--rw-r--r--   0        0        0      400 2023-05-13 14:20:26.202077 Lattice-Graph-Manipulation-1.3.1/Lattice_Scripts/0c61af02-51eb-402b-afe9-2a1c0cafb88b.gv
--rw-r--r--   0        0        0     6332 2023-05-13 14:20:26.225410 Lattice-Graph-Manipulation-1.3.1/Lattice_Scripts/0c61af02-51eb-402b-afe9-2a1c0cafb88b.gv.pdf
--rw-r--r--   0        0        0      624 2023-05-13 14:31:43.449798 Lattice-Graph-Manipulation-1.3.1/Lattice_Scripts/22aba17d-0803-40d1-a6d7-f5526b847a82.gv
--rw-r--r--   0        0        0     7344 2023-05-13 14:31:43.479797 Lattice-Graph-Manipulation-1.3.1/Lattice_Scripts/22aba17d-0803-40d1-a6d7-f5526b847a82.gv.pdf
--rw-r--r--   0        0        0      541 2023-05-09 00:00:20.318358 Lattice-Graph-Manipulation-1.3.1/Lattice_Scripts/3202f283-fd53-489f-a524-6c2fd4eb742a.gv
--rw-r--r--   0        0        0     6152 2023-05-09 00:00:20.345023 Lattice-Graph-Manipulation-1.3.1/Lattice_Scripts/3202f283-fd53-489f-a524-6c2fd4eb742a.gv.pdf
--rw-r--r--   0        0        0        0 2023-05-09 00:13:53.962236 Lattice-Graph-Manipulation-1.3.1/Lattice_Scripts/40861fca-41e9-4582-8ebf-fb5f53177aa2
--rw-r--r--   0        0        0        0 2023-05-09 00:13:53.958902 Lattice-Graph-Manipulation-1.3.1/Lattice_Scripts/420099d8-e96d-4900-9fe7-b952495b28c0
--rw-r--r--   0        0        0      541 2023-05-09 15:26:45.205033 Lattice-Graph-Manipulation-1.3.1/Lattice_Scripts/5ee8c02a-4299-4464-9406-c91d7596a3df.gv
--rw-r--r--   0        0        0     6152 2023-05-09 15:26:45.228366 Lattice-Graph-Manipulation-1.3.1/Lattice_Scripts/5ee8c02a-4299-4464-9406-c91d7596a3df.gv.pdf
--rw-r--r--   0        0        0      541 2023-05-09 00:00:25.531313 Lattice-Graph-Manipulation-1.3.1/Lattice_Scripts/6243ae9e-b9ca-4301-bc1b-23820b5b5c67.gv
--rw-r--r--   0        0        0     6118 2023-05-09 00:00:25.551312 Lattice-Graph-Manipulation-1.3.1/Lattice_Scripts/6243ae9e-b9ca-4301-bc1b-23820b5b5c67.gv.pdf
--rw-r--r--   0        0        0      541 2023-05-09 00:00:07.779270 Lattice-Graph-Manipulation-1.3.1/Lattice_Scripts/7101765c-cde4-4086-a6cf-85ca9f573d33.gv
--rw-r--r--   0        0        0     6118 2023-05-09 00:00:07.805935 Lattice-Graph-Manipulation-1.3.1/Lattice_Scripts/7101765c-cde4-4086-a6cf-85ca9f573d33.gv.pdf
--rw-r--r--   0        0        0      541 2023-05-09 00:00:23.294809 Lattice-Graph-Manipulation-1.3.1/Lattice_Scripts/80d5097d-a203-4423-9177-8db54d9ff8cc.gv
--rw-r--r--   0        0        0     6152 2023-05-09 00:00:23.314807 Lattice-Graph-Manipulation-1.3.1/Lattice_Scripts/80d5097d-a203-4423-9177-8db54d9ff8cc.gv.pdf
--rw-r--r--   0        0        0      657 2023-05-15 17:36:35.263258 Lattice-Graph-Manipulation-1.3.1/Lattice_Scripts/8558953d-ec61-4d46-ab51-cad78015e389.gv
--rw-r--r--   0        0        0     5072 2023-05-15 17:36:35.316592 Lattice-Graph-Manipulation-1.3.1/Lattice_Scripts/8558953d-ec61-4d46-ab51-cad78015e389.gv.pdf
--rw-r--r--   0        0        0      588 2023-05-15 13:32:19.489910 Lattice-Graph-Manipulation-1.3.1/Lattice_Scripts/9167244b-dc36-488e-9a24-8c0f207c3aaa.gv
--rw-r--r--   0        0        0     4963 2023-05-15 13:32:19.523243 Lattice-Graph-Manipulation-1.3.1/Lattice_Scripts/9167244b-dc36-488e-9a24-8c0f207c3aaa.gv.pdf
--rw-r--r--   0        0        0      657 2023-05-15 17:35:59.843239 Lattice-Graph-Manipulation-1.3.1/Lattice_Scripts/91f695f0-ac92-403e-81d8-f7d76a5a6eba.gv
--rw-r--r--   0        0        0     5072 2023-05-15 17:35:59.913240 Lattice-Graph-Manipulation-1.3.1/Lattice_Scripts/91f695f0-ac92-403e-81d8-f7d76a5a6eba.gv.pdf
--rw-r--r--   0        0        0      541 2023-05-09 15:26:37.261708 Lattice-Graph-Manipulation-1.3.1/Lattice_Scripts/9d8f8c6d-22ed-4a7e-af45-8ac72691f52c.gv
--rw-r--r--   0        0        0     6142 2023-05-09 15:26:37.285041 Lattice-Graph-Manipulation-1.3.1/Lattice_Scripts/9d8f8c6d-22ed-4a7e-af45-8ac72691f52c.gv.pdf
--rw-r--r--   0        0        0        0 2023-04-30 13:12:22.483002 Lattice-Graph-Manipulation-1.3.1/Lattice_Scripts/__init__.py
--rw-r--r--   0        0        0      384 2023-05-13 14:21:44.373379 Lattice-Graph-Manipulation-1.3.1/Lattice_Scripts/a972d228-3f01-42fc-89e8-b0431bcd87b6.gv
--rw-r--r--   0        0        0     6561 2023-05-13 14:21:44.393379 Lattice-Graph-Manipulation-1.3.1/Lattice_Scripts/a972d228-3f01-42fc-89e8-b0431bcd87b6.gv.pdf
--rw-r--r--   0        0        0      639 2023-05-07 00:22:21.936580 Lattice-Graph-Manipulation-1.3.1/Lattice_Scripts/bb_tree.py
--rw-r--r--   0        0        0      624 2023-06-12 16:14:40.207937 Lattice-Graph-Manipulation-1.3.1/Lattice_Scripts/ce8e0387-b735-400d-a303-cc56e4769a9b.gv
--rw-r--r--   0        0        0     7350 2023-06-12 16:14:40.231270 Lattice-Graph-Manipulation-1.3.1/Lattice_Scripts/ce8e0387-b735-400d-a303-cc56e4769a9b.gv.pdf
--rw-r--r--   0        0        0      541 2023-05-13 11:26:54.780832 Lattice-Graph-Manipulation-1.3.1/Lattice_Scripts/d962d2ca-0365-46f3-9b0e-3c07645b036d.gv
--rw-r--r--   0        0        0     6151 2023-05-13 11:26:54.804166 Lattice-Graph-Manipulation-1.3.1/Lattice_Scripts/d962d2ca-0365-46f3-9b0e-3c07645b036d.gv.pdf
--rw-r--r--   0        0        0     1368 2023-05-05 22:09:45.090958 Lattice-Graph-Manipulation-1.3.1/Lattice_Scripts/dot_output/124ce352-4606-4b8e-83cf-894a431e02f5.gv
--rw-r--r--   0        0        0     5573 2023-05-05 22:09:45.107624 Lattice-Graph-Manipulation-1.3.1/Lattice_Scripts/dot_output/124ce352-4606-4b8e-83cf-894a431e02f5.gv.pdf
--rw-r--r--   0        0        0     4236 2023-05-05 22:01:27.915042 Lattice-Graph-Manipulation-1.3.1/Lattice_Scripts/dot_output/18839347-7fff-4bf6-b283-22b194da1d73.gv
--rw-r--r--   0        0        0     7654 2023-05-05 22:01:27.935042 Lattice-Graph-Manipulation-1.3.1/Lattice_Scripts/dot_output/18839347-7fff-4bf6-b283-22b194da1d73.gv.pdf
--rw-r--r--   0        0        0     1368 2023-05-05 21:59:43.450219 Lattice-Graph-Manipulation-1.3.1/Lattice_Scripts/dot_output/2b89469f-7c20-4e83-987a-243eed3f15b0.gv
--rw-r--r--   0        0        0     5567 2023-05-05 21:59:43.470219 Lattice-Graph-Manipulation-1.3.1/Lattice_Scripts/dot_output/2b89469f-7c20-4e83-987a-243eed3f15b0.gv.pdf
--rw-r--r--   0        0        0     4236 2023-05-05 22:02:54.341480 Lattice-Graph-Manipulation-1.3.1/Lattice_Scripts/dot_output/4d9238b6-e314-4c1d-8fe0-851f2237e653.gv
--rw-r--r--   0        0        0     7750 2023-05-05 22:02:54.361480 Lattice-Graph-Manipulation-1.3.1/Lattice_Scripts/dot_output/4d9238b6-e314-4c1d-8fe0-851f2237e653.gv.pdf
--rw-r--r--   0        0        0     4236 2023-05-05 22:04:13.795053 Lattice-Graph-Manipulation-1.3.1/Lattice_Scripts/dot_output/6dd10e1b-c98d-4a1f-8297-302f270b51da.gv
--rw-r--r--   0        0        0     7593 2023-05-05 22:04:13.815054 Lattice-Graph-Manipulation-1.3.1/Lattice_Scripts/dot_output/6dd10e1b-c98d-4a1f-8297-302f270b51da.gv.pdf
--rw-r--r--   0        0        0     7905 2023-05-07 00:23:54.513172 Lattice-Graph-Manipulation-1.3.1/Lattice_Scripts/dot_output/721f21a0-d8ee-4cfd-acfb-67b3b4021d94.gv
--rw-r--r--   0        0        0     9268 2023-05-07 00:23:54.536505 Lattice-Graph-Manipulation-1.3.1/Lattice_Scripts/dot_output/721f21a0-d8ee-4cfd-acfb-67b3b4021d94.gv.pdf
--rw-r--r--   0        0        0     7905 2023-05-07 00:19:22.396730 Lattice-Graph-Manipulation-1.3.1/Lattice_Scripts/dot_output/782355df-1bc9-4714-85ed-65e312e0396b.gv
--rw-r--r--   0        0        0     9201 2023-05-07 00:19:22.426730 Lattice-Graph-Manipulation-1.3.1/Lattice_Scripts/dot_output/782355df-1bc9-4714-85ed-65e312e0396b.gv.pdf
--rw-r--r--   0        0        0     4236 2023-05-05 22:02:27.888198 Lattice-Graph-Manipulation-1.3.1/Lattice_Scripts/dot_output/7b10a609-60ba-416a-8572-7e3ebf8c1bc5.gv
--rw-r--r--   0        0        0     7617 2023-05-05 22:02:27.911531 Lattice-Graph-Manipulation-1.3.1/Lattice_Scripts/dot_output/7b10a609-60ba-416a-8572-7e3ebf8c1bc5.gv.pdf
--rw-r--r--   0        0        0     7905 2023-05-07 00:36:00.902560 Lattice-Graph-Manipulation-1.3.1/Lattice_Scripts/dot_output/85690484-fe37-4e5f-9c48-d61eb19c0e86.gv
--rw-r--r--   0        0        0     9214 2023-05-07 00:36:00.925894 Lattice-Graph-Manipulation-1.3.1/Lattice_Scripts/dot_output/85690484-fe37-4e5f-9c48-d61eb19c0e86.gv.pdf
--rw-r--r--   0        0        0     5352 2023-05-05 22:10:28.170815 Lattice-Graph-Manipulation-1.3.1/Lattice_Scripts/dot_output/89621631-a0d6-4cf1-b1d6-98bee69eafd6.gv
--rw-r--r--   0        0        0     7753 2023-05-05 22:10:28.194148 Lattice-Graph-Manipulation-1.3.1/Lattice_Scripts/dot_output/89621631-a0d6-4cf1-b1d6-98bee69eafd6.gv.pdf
--rw-r--r--   0        0        0     7905 2023-05-05 22:10:58.647394 Lattice-Graph-Manipulation-1.3.1/Lattice_Scripts/dot_output/8a952fcc-a0a5-4902-9942-cb18880ee393.gv
--rw-r--r--   0        0        0     9267 2023-05-05 22:10:58.670728 Lattice-Graph-Manipulation-1.3.1/Lattice_Scripts/dot_output/8a952fcc-a0a5-4902-9942-cb18880ee393.gv.pdf
--rw-r--r--   0        0        0     2304 2023-05-07 00:23:41.253183 Lattice-Graph-Manipulation-1.3.1/Lattice_Scripts/dot_output/98af54bc-3975-4394-804d-66789065d1c9.gv
--rw-r--r--   0        0        0     6086 2023-05-07 00:23:41.273183 Lattice-Graph-Manipulation-1.3.1/Lattice_Scripts/dot_output/98af54bc-3975-4394-804d-66789065d1c9.gv.pdf
--rw-r--r--   0        0        0      451 2023-05-05 16:12:08.031549 Lattice-Graph-Manipulation-1.3.1/Lattice_Scripts/dot_output/b68224e8-ee0f-43bd-ad54-cbb0bc805f8e.gv
--rw-r--r--   0        0        0     6700 2023-05-05 16:12:08.054882 Lattice-Graph-Manipulation-1.3.1/Lattice_Scripts/dot_output/b68224e8-ee0f-43bd-ad54-cbb0bc805f8e.gv.pdf
--rw-r--r--   0        0        0     7905 2023-05-07 00:34:13.555984 Lattice-Graph-Manipulation-1.3.1/Lattice_Scripts/dot_output/bdea7672-3cf4-48bc-861a-86787c8e9122.gv
--rw-r--r--   0        0        0     9276 2023-05-07 00:34:13.579317 Lattice-Graph-Manipulation-1.3.1/Lattice_Scripts/dot_output/bdea7672-3cf4-48bc-861a-86787c8e9122.gv.pdf
--rw-r--r--   0        0        0      451 2023-05-07 00:20:50.539988 Lattice-Graph-Manipulation-1.3.1/Lattice_Scripts/dot_output/c04b2718-239f-4811-8f73-d78111718784.gv
--rw-r--r--   0        0        0     6728 2023-05-07 00:20:50.559988 Lattice-Graph-Manipulation-1.3.1/Lattice_Scripts/dot_output/c04b2718-239f-4811-8f73-d78111718784.gv.pdf
--rw-r--r--   0        0        0     2364 2023-05-05 22:01:03.491857 Lattice-Graph-Manipulation-1.3.1/Lattice_Scripts/dot_output/d1456d21-9a4f-4356-8f63-dd10573cf1b9.gv
--rw-r--r--   0        0        0     6142 2023-05-05 22:01:03.511857 Lattice-Graph-Manipulation-1.3.1/Lattice_Scripts/dot_output/d1456d21-9a4f-4356-8f63-dd10573cf1b9.gv.pdf
--rw-r--r--   0        0        0     1368 2023-05-05 21:58:56.455608 Lattice-Graph-Manipulation-1.3.1/Lattice_Scripts/dot_output/f814a715-e5ec-4cab-85bd-746f5d0dcb84.gv
--rw-r--r--   0        0        0     5809 2023-05-05 21:58:56.478942 Lattice-Graph-Manipulation-1.3.1/Lattice_Scripts/dot_output/f814a715-e5ec-4cab-85bd-746f5d0dcb84.gv.pdf
--rw-r--r--   0        0        0      541 2023-05-07 00:36:08.819221 Lattice-Graph-Manipulation-1.3.1/Lattice_Scripts/dot_output/fb51fde2-173b-4824-91c0-0b1036767689.gv
--rw-r--r--   0        0        0     6146 2023-05-07 00:36:08.852554 Lattice-Graph-Manipulation-1.3.1/Lattice_Scripts/dot_output/fb51fde2-173b-4824-91c0-0b1036767689.gv.pdf
--rw-r--r--   0        0        0      541 2023-05-09 00:00:23.338139 Lattice-Graph-Manipulation-1.3.1/Lattice_Scripts/e9422bf1-3455-4d4a-afc9-de9fca5ae2f7.gv
--rw-r--r--   0        0        0     6152 2023-05-09 00:00:23.368137 Lattice-Graph-Manipulation-1.3.1/Lattice_Scripts/e9422bf1-3455-4d4a-afc9-de9fca5ae2f7.gv.pdf
--rw-r--r--   0        0        0      470 2023-05-09 15:29:25.438125 Lattice-Graph-Manipulation-1.3.1/Lattice_Scripts/f99dc209-e23f-406f-8d61-5e0943af8836.gv
--rw-r--r--   0        0        0     7583 2023-05-09 15:29:25.458125 Lattice-Graph-Manipulation-1.3.1/Lattice_Scripts/f99dc209-e23f-406f-8d61-5e0943af8836.gv.pdf
--rw-r--r--   0        0        0        0 2023-05-09 00:13:53.962236 Lattice-Graph-Manipulation-1.3.1/Lattice_Scripts/ff81f168-34cc-4770-8535-2befc371ab12
--rw-r--r--   0        0        0     1095 2023-05-20 20:33:45.716098 Lattice-Graph-Manipulation-1.3.1/Lattice_Scripts/grid_example.py
--rw-r--r--   0        0        0      648 2023-05-01 21:34:44.057078 Lattice-Graph-Manipulation-1.3.1/Lattice_Scripts/simple_examples.py
--rw-r--r--   0        0        0     1258 2023-05-15 23:23:21.738387 Lattice-Graph-Manipulation-1.3.1/Lattice_Scripts/simple_graph.py
--rw-r--r--   0        0        0        9 2023-04-30 13:12:10.136468 Lattice-Graph-Manipulation-1.3.1/README.md
--rw-r--r--   0        0        0       61 2023-04-30 13:12:22.483002 Lattice-Graph-Manipulation-1.3.1/lattice/__init__.py
--rw-r--r--   0        0        0      148 2023-05-04 09:15:27.080595 Lattice-Graph-Manipulation-1.3.1/lattice/edge/__init__.py
--rw-r--r--   0        0        0      584 2023-05-01 21:31:00.683002 Lattice-Graph-Manipulation-1.3.1/lattice/edge/edge.py
--rw-r--r--   0        0        0      440 2023-04-30 13:12:22.483002 Lattice-Graph-Manipulation-1.3.1/lattice/edge/traversaledge.py
--rw-r--r--   0        0        0      358 2023-05-04 09:11:10.130523 Lattice-Graph-Manipulation-1.3.1/lattice/edge/visualedge.py
--rw-r--r--   0        0        0      114 2023-04-30 13:12:22.483002 Lattice-Graph-Manipulation-1.3.1/lattice/graph/__init__.py
--rw-r--r--   0        0        0     1558 2023-05-01 21:00:58.830421 Lattice-Graph-Manipulation-1.3.1/lattice/graph/bbtree.py
--rw-r--r--   0        0        0     4879 2023-06-12 16:14:40.144603 Lattice-Graph-Manipulation-1.3.1/lattice/graph/graph.py
--rw-r--r--   0        0        0      829 2023-05-05 12:55:46.790589 Lattice-Graph-Manipulation-1.3.1/lattice/graph/tree.py
--rw-r--r--   0        0        0       43 2023-04-30 13:12:22.483002 Lattice-Graph-Manipulation-1.3.1/lattice/node/__init__.py
--rw-r--r--   0        0        0     1399 2023-05-15 13:04:33.398011 Lattice-Graph-Manipulation-1.3.1/lattice/node/node.py
--rw-r--r--   0        0        0      439 2023-06-12 16:17:41.741128 Lattice-Graph-Manipulation-1.3.1/pyproject.toml
--rw-r--r--   0        0        0      196 1970-01-01 00:00:00.000000 Lattice-Graph-Manipulation-1.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-04-30 13:12:10.136468 Lattice-Graph-Manipulation-1.4.0/LICENSE
+-rw-r--r--   0        0        0      400 2023-05-13 14:20:26.202077 Lattice-Graph-Manipulation-1.4.0/Lattice_Scripts/0c61af02-51eb-402b-afe9-2a1c0cafb88b.gv
+-rw-r--r--   0        0        0     6332 2023-05-13 14:20:26.225410 Lattice-Graph-Manipulation-1.4.0/Lattice_Scripts/0c61af02-51eb-402b-afe9-2a1c0cafb88b.gv.pdf
+-rw-r--r--   0        0        0      624 2023-05-13 14:31:43.449798 Lattice-Graph-Manipulation-1.4.0/Lattice_Scripts/22aba17d-0803-40d1-a6d7-f5526b847a82.gv
+-rw-r--r--   0        0        0     7344 2023-05-13 14:31:43.479797 Lattice-Graph-Manipulation-1.4.0/Lattice_Scripts/22aba17d-0803-40d1-a6d7-f5526b847a82.gv.pdf
+-rw-r--r--   0        0        0      541 2023-05-09 00:00:20.318358 Lattice-Graph-Manipulation-1.4.0/Lattice_Scripts/3202f283-fd53-489f-a524-6c2fd4eb742a.gv
+-rw-r--r--   0        0        0     6152 2023-05-09 00:00:20.345023 Lattice-Graph-Manipulation-1.4.0/Lattice_Scripts/3202f283-fd53-489f-a524-6c2fd4eb742a.gv.pdf
+-rw-r--r--   0        0        0        0 2023-05-09 00:13:53.962236 Lattice-Graph-Manipulation-1.4.0/Lattice_Scripts/40861fca-41e9-4582-8ebf-fb5f53177aa2
+-rw-r--r--   0        0        0        0 2023-05-09 00:13:53.958902 Lattice-Graph-Manipulation-1.4.0/Lattice_Scripts/420099d8-e96d-4900-9fe7-b952495b28c0
+-rw-r--r--   0        0        0      541 2023-05-09 15:26:45.205033 Lattice-Graph-Manipulation-1.4.0/Lattice_Scripts/5ee8c02a-4299-4464-9406-c91d7596a3df.gv
+-rw-r--r--   0        0        0     6152 2023-05-09 15:26:45.228366 Lattice-Graph-Manipulation-1.4.0/Lattice_Scripts/5ee8c02a-4299-4464-9406-c91d7596a3df.gv.pdf
+-rw-r--r--   0        0        0      541 2023-05-09 00:00:25.531313 Lattice-Graph-Manipulation-1.4.0/Lattice_Scripts/6243ae9e-b9ca-4301-bc1b-23820b5b5c67.gv
+-rw-r--r--   0        0        0     6118 2023-05-09 00:00:25.551312 Lattice-Graph-Manipulation-1.4.0/Lattice_Scripts/6243ae9e-b9ca-4301-bc1b-23820b5b5c67.gv.pdf
+-rw-r--r--   0        0        0      541 2023-05-09 00:00:07.779270 Lattice-Graph-Manipulation-1.4.0/Lattice_Scripts/7101765c-cde4-4086-a6cf-85ca9f573d33.gv
+-rw-r--r--   0        0        0     6118 2023-05-09 00:00:07.805935 Lattice-Graph-Manipulation-1.4.0/Lattice_Scripts/7101765c-cde4-4086-a6cf-85ca9f573d33.gv.pdf
+-rw-r--r--   0        0        0      541 2023-05-09 00:00:23.294809 Lattice-Graph-Manipulation-1.4.0/Lattice_Scripts/80d5097d-a203-4423-9177-8db54d9ff8cc.gv
+-rw-r--r--   0        0        0     6152 2023-05-09 00:00:23.314807 Lattice-Graph-Manipulation-1.4.0/Lattice_Scripts/80d5097d-a203-4423-9177-8db54d9ff8cc.gv.pdf
+-rw-r--r--   0        0        0      657 2023-05-15 17:36:35.263258 Lattice-Graph-Manipulation-1.4.0/Lattice_Scripts/8558953d-ec61-4d46-ab51-cad78015e389.gv
+-rw-r--r--   0        0        0     5072 2023-05-15 17:36:35.316592 Lattice-Graph-Manipulation-1.4.0/Lattice_Scripts/8558953d-ec61-4d46-ab51-cad78015e389.gv.pdf
+-rw-r--r--   0        0        0      588 2023-05-15 13:32:19.489910 Lattice-Graph-Manipulation-1.4.0/Lattice_Scripts/9167244b-dc36-488e-9a24-8c0f207c3aaa.gv
+-rw-r--r--   0        0        0     4963 2023-05-15 13:32:19.523243 Lattice-Graph-Manipulation-1.4.0/Lattice_Scripts/9167244b-dc36-488e-9a24-8c0f207c3aaa.gv.pdf
+-rw-r--r--   0        0        0      657 2023-05-15 17:35:59.843239 Lattice-Graph-Manipulation-1.4.0/Lattice_Scripts/91f695f0-ac92-403e-81d8-f7d76a5a6eba.gv
+-rw-r--r--   0        0        0     5072 2023-05-15 17:35:59.913240 Lattice-Graph-Manipulation-1.4.0/Lattice_Scripts/91f695f0-ac92-403e-81d8-f7d76a5a6eba.gv.pdf
+-rw-r--r--   0        0        0      541 2023-05-09 15:26:37.261708 Lattice-Graph-Manipulation-1.4.0/Lattice_Scripts/9d8f8c6d-22ed-4a7e-af45-8ac72691f52c.gv
+-rw-r--r--   0        0        0     6142 2023-05-09 15:26:37.285041 Lattice-Graph-Manipulation-1.4.0/Lattice_Scripts/9d8f8c6d-22ed-4a7e-af45-8ac72691f52c.gv.pdf
+-rw-r--r--   0        0        0        0 2023-04-30 13:12:22.483002 Lattice-Graph-Manipulation-1.4.0/Lattice_Scripts/__init__.py
+-rw-r--r--   0        0        0      384 2023-05-13 14:21:44.373379 Lattice-Graph-Manipulation-1.4.0/Lattice_Scripts/a972d228-3f01-42fc-89e8-b0431bcd87b6.gv
+-rw-r--r--   0        0        0     6561 2023-05-13 14:21:44.393379 Lattice-Graph-Manipulation-1.4.0/Lattice_Scripts/a972d228-3f01-42fc-89e8-b0431bcd87b6.gv.pdf
+-rw-r--r--   0        0        0      639 2023-05-07 00:22:21.936580 Lattice-Graph-Manipulation-1.4.0/Lattice_Scripts/bb_tree.py
+-rw-r--r--   0        0        0      624 2023-06-12 16:14:40.207937 Lattice-Graph-Manipulation-1.4.0/Lattice_Scripts/ce8e0387-b735-400d-a303-cc56e4769a9b.gv
+-rw-r--r--   0        0        0     7350 2023-06-12 16:14:40.231270 Lattice-Graph-Manipulation-1.4.0/Lattice_Scripts/ce8e0387-b735-400d-a303-cc56e4769a9b.gv.pdf
+-rw-r--r--   0        0        0      541 2023-05-13 11:26:54.780832 Lattice-Graph-Manipulation-1.4.0/Lattice_Scripts/d962d2ca-0365-46f3-9b0e-3c07645b036d.gv
+-rw-r--r--   0        0        0     6151 2023-05-13 11:26:54.804166 Lattice-Graph-Manipulation-1.4.0/Lattice_Scripts/d962d2ca-0365-46f3-9b0e-3c07645b036d.gv.pdf
+-rw-r--r--   0        0        0     1368 2023-05-05 22:09:45.090958 Lattice-Graph-Manipulation-1.4.0/Lattice_Scripts/dot_output/124ce352-4606-4b8e-83cf-894a431e02f5.gv
+-rw-r--r--   0        0        0     5573 2023-05-05 22:09:45.107624 Lattice-Graph-Manipulation-1.4.0/Lattice_Scripts/dot_output/124ce352-4606-4b8e-83cf-894a431e02f5.gv.pdf
+-rw-r--r--   0        0        0     4236 2023-05-05 22:01:27.915042 Lattice-Graph-Manipulation-1.4.0/Lattice_Scripts/dot_output/18839347-7fff-4bf6-b283-22b194da1d73.gv
+-rw-r--r--   0        0        0     7654 2023-05-05 22:01:27.935042 Lattice-Graph-Manipulation-1.4.0/Lattice_Scripts/dot_output/18839347-7fff-4bf6-b283-22b194da1d73.gv.pdf
+-rw-r--r--   0        0        0     1368 2023-05-05 21:59:43.450219 Lattice-Graph-Manipulation-1.4.0/Lattice_Scripts/dot_output/2b89469f-7c20-4e83-987a-243eed3f15b0.gv
+-rw-r--r--   0        0        0     5567 2023-05-05 21:59:43.470219 Lattice-Graph-Manipulation-1.4.0/Lattice_Scripts/dot_output/2b89469f-7c20-4e83-987a-243eed3f15b0.gv.pdf
+-rw-r--r--   0        0        0     4236 2023-05-05 22:02:54.341480 Lattice-Graph-Manipulation-1.4.0/Lattice_Scripts/dot_output/4d9238b6-e314-4c1d-8fe0-851f2237e653.gv
+-rw-r--r--   0        0        0     7750 2023-05-05 22:02:54.361480 Lattice-Graph-Manipulation-1.4.0/Lattice_Scripts/dot_output/4d9238b6-e314-4c1d-8fe0-851f2237e653.gv.pdf
+-rw-r--r--   0        0        0     4236 2023-05-05 22:04:13.795053 Lattice-Graph-Manipulation-1.4.0/Lattice_Scripts/dot_output/6dd10e1b-c98d-4a1f-8297-302f270b51da.gv
+-rw-r--r--   0        0        0     7593 2023-05-05 22:04:13.815054 Lattice-Graph-Manipulation-1.4.0/Lattice_Scripts/dot_output/6dd10e1b-c98d-4a1f-8297-302f270b51da.gv.pdf
+-rw-r--r--   0        0        0     7905 2023-05-07 00:23:54.513172 Lattice-Graph-Manipulation-1.4.0/Lattice_Scripts/dot_output/721f21a0-d8ee-4cfd-acfb-67b3b4021d94.gv
+-rw-r--r--   0        0        0     9268 2023-05-07 00:23:54.536505 Lattice-Graph-Manipulation-1.4.0/Lattice_Scripts/dot_output/721f21a0-d8ee-4cfd-acfb-67b3b4021d94.gv.pdf
+-rw-r--r--   0        0        0     7905 2023-05-07 00:19:22.396730 Lattice-Graph-Manipulation-1.4.0/Lattice_Scripts/dot_output/782355df-1bc9-4714-85ed-65e312e0396b.gv
+-rw-r--r--   0        0        0     9201 2023-05-07 00:19:22.426730 Lattice-Graph-Manipulation-1.4.0/Lattice_Scripts/dot_output/782355df-1bc9-4714-85ed-65e312e0396b.gv.pdf
+-rw-r--r--   0        0        0     4236 2023-05-05 22:02:27.888198 Lattice-Graph-Manipulation-1.4.0/Lattice_Scripts/dot_output/7b10a609-60ba-416a-8572-7e3ebf8c1bc5.gv
+-rw-r--r--   0        0        0     7617 2023-05-05 22:02:27.911531 Lattice-Graph-Manipulation-1.4.0/Lattice_Scripts/dot_output/7b10a609-60ba-416a-8572-7e3ebf8c1bc5.gv.pdf
+-rw-r--r--   0        0        0     7905 2023-05-07 00:36:00.902560 Lattice-Graph-Manipulation-1.4.0/Lattice_Scripts/dot_output/85690484-fe37-4e5f-9c48-d61eb19c0e86.gv
+-rw-r--r--   0        0        0     9214 2023-05-07 00:36:00.925894 Lattice-Graph-Manipulation-1.4.0/Lattice_Scripts/dot_output/85690484-fe37-4e5f-9c48-d61eb19c0e86.gv.pdf
+-rw-r--r--   0        0        0     5352 2023-05-05 22:10:28.170815 Lattice-Graph-Manipulation-1.4.0/Lattice_Scripts/dot_output/89621631-a0d6-4cf1-b1d6-98bee69eafd6.gv
+-rw-r--r--   0        0        0     7753 2023-05-05 22:10:28.194148 Lattice-Graph-Manipulation-1.4.0/Lattice_Scripts/dot_output/89621631-a0d6-4cf1-b1d6-98bee69eafd6.gv.pdf
+-rw-r--r--   0        0        0     7905 2023-05-05 22:10:58.647394 Lattice-Graph-Manipulation-1.4.0/Lattice_Scripts/dot_output/8a952fcc-a0a5-4902-9942-cb18880ee393.gv
+-rw-r--r--   0        0        0     9267 2023-05-05 22:10:58.670728 Lattice-Graph-Manipulation-1.4.0/Lattice_Scripts/dot_output/8a952fcc-a0a5-4902-9942-cb18880ee393.gv.pdf
+-rw-r--r--   0        0        0     2304 2023-05-07 00:23:41.253183 Lattice-Graph-Manipulation-1.4.0/Lattice_Scripts/dot_output/98af54bc-3975-4394-804d-66789065d1c9.gv
+-rw-r--r--   0        0        0     6086 2023-05-07 00:23:41.273183 Lattice-Graph-Manipulation-1.4.0/Lattice_Scripts/dot_output/98af54bc-3975-4394-804d-66789065d1c9.gv.pdf
+-rw-r--r--   0        0        0      451 2023-05-05 16:12:08.031549 Lattice-Graph-Manipulation-1.4.0/Lattice_Scripts/dot_output/b68224e8-ee0f-43bd-ad54-cbb0bc805f8e.gv
+-rw-r--r--   0        0        0     6700 2023-05-05 16:12:08.054882 Lattice-Graph-Manipulation-1.4.0/Lattice_Scripts/dot_output/b68224e8-ee0f-43bd-ad54-cbb0bc805f8e.gv.pdf
+-rw-r--r--   0        0        0     7905 2023-05-07 00:34:13.555984 Lattice-Graph-Manipulation-1.4.0/Lattice_Scripts/dot_output/bdea7672-3cf4-48bc-861a-86787c8e9122.gv
+-rw-r--r--   0        0        0     9276 2023-05-07 00:34:13.579317 Lattice-Graph-Manipulation-1.4.0/Lattice_Scripts/dot_output/bdea7672-3cf4-48bc-861a-86787c8e9122.gv.pdf
+-rw-r--r--   0        0        0      451 2023-05-07 00:20:50.539988 Lattice-Graph-Manipulation-1.4.0/Lattice_Scripts/dot_output/c04b2718-239f-4811-8f73-d78111718784.gv
+-rw-r--r--   0        0        0     6728 2023-05-07 00:20:50.559988 Lattice-Graph-Manipulation-1.4.0/Lattice_Scripts/dot_output/c04b2718-239f-4811-8f73-d78111718784.gv.pdf
+-rw-r--r--   0        0        0     2364 2023-05-05 22:01:03.491857 Lattice-Graph-Manipulation-1.4.0/Lattice_Scripts/dot_output/d1456d21-9a4f-4356-8f63-dd10573cf1b9.gv
+-rw-r--r--   0        0        0     6142 2023-05-05 22:01:03.511857 Lattice-Graph-Manipulation-1.4.0/Lattice_Scripts/dot_output/d1456d21-9a4f-4356-8f63-dd10573cf1b9.gv.pdf
+-rw-r--r--   0        0        0     1368 2023-05-05 21:58:56.455608 Lattice-Graph-Manipulation-1.4.0/Lattice_Scripts/dot_output/f814a715-e5ec-4cab-85bd-746f5d0dcb84.gv
+-rw-r--r--   0        0        0     5809 2023-05-05 21:58:56.478942 Lattice-Graph-Manipulation-1.4.0/Lattice_Scripts/dot_output/f814a715-e5ec-4cab-85bd-746f5d0dcb84.gv.pdf
+-rw-r--r--   0        0        0      541 2023-05-07 00:36:08.819221 Lattice-Graph-Manipulation-1.4.0/Lattice_Scripts/dot_output/fb51fde2-173b-4824-91c0-0b1036767689.gv
+-rw-r--r--   0        0        0     6146 2023-05-07 00:36:08.852554 Lattice-Graph-Manipulation-1.4.0/Lattice_Scripts/dot_output/fb51fde2-173b-4824-91c0-0b1036767689.gv.pdf
+-rw-r--r--   0        0        0      541 2023-05-09 00:00:23.338139 Lattice-Graph-Manipulation-1.4.0/Lattice_Scripts/e9422bf1-3455-4d4a-afc9-de9fca5ae2f7.gv
+-rw-r--r--   0        0        0     6152 2023-05-09 00:00:23.368137 Lattice-Graph-Manipulation-1.4.0/Lattice_Scripts/e9422bf1-3455-4d4a-afc9-de9fca5ae2f7.gv.pdf
+-rw-r--r--   0        0        0      470 2023-05-09 15:29:25.438125 Lattice-Graph-Manipulation-1.4.0/Lattice_Scripts/f99dc209-e23f-406f-8d61-5e0943af8836.gv
+-rw-r--r--   0        0        0     7583 2023-05-09 15:29:25.458125 Lattice-Graph-Manipulation-1.4.0/Lattice_Scripts/f99dc209-e23f-406f-8d61-5e0943af8836.gv.pdf
+-rw-r--r--   0        0        0        0 2023-05-09 00:13:53.962236 Lattice-Graph-Manipulation-1.4.0/Lattice_Scripts/ff81f168-34cc-4770-8535-2befc371ab12
+-rw-r--r--   0        0        0     1095 2023-05-20 20:33:45.716098 Lattice-Graph-Manipulation-1.4.0/Lattice_Scripts/grid_example.py
+-rw-r--r--   0        0        0      648 2023-05-01 21:34:44.057078 Lattice-Graph-Manipulation-1.4.0/Lattice_Scripts/simple_examples.py
+-rw-r--r--   0        0        0     1258 2023-05-15 23:23:21.738387 Lattice-Graph-Manipulation-1.4.0/Lattice_Scripts/simple_graph.py
+-rw-r--r--   0        0        0        9 2023-04-30 13:12:10.136468 Lattice-Graph-Manipulation-1.4.0/README.md
+-rw-r--r--   0        0        0       61 2023-04-30 13:12:22.483002 Lattice-Graph-Manipulation-1.4.0/lattice/__init__.py
+-rw-r--r--   0        0        0      148 2023-05-04 09:15:27.080595 Lattice-Graph-Manipulation-1.4.0/lattice/edge/__init__.py
+-rw-r--r--   0        0        0      584 2023-05-01 21:31:00.683002 Lattice-Graph-Manipulation-1.4.0/lattice/edge/edge.py
+-rw-r--r--   0        0        0      440 2023-04-30 13:12:22.483002 Lattice-Graph-Manipulation-1.4.0/lattice/edge/traversaledge.py
+-rw-r--r--   0        0        0      358 2023-05-04 09:11:10.130523 Lattice-Graph-Manipulation-1.4.0/lattice/edge/visualedge.py
+-rw-r--r--   0        0        0      114 2023-04-30 13:12:22.483002 Lattice-Graph-Manipulation-1.4.0/lattice/graph/__init__.py
+-rw-r--r--   0        0        0     1558 2023-05-01 21:00:58.830421 Lattice-Graph-Manipulation-1.4.0/lattice/graph/bbtree.py
+-rw-r--r--   0        0        0     5046 2023-06-14 01:08:31.151594 Lattice-Graph-Manipulation-1.4.0/lattice/graph/graph.py
+-rw-r--r--   0        0        0      829 2023-05-05 12:55:46.790589 Lattice-Graph-Manipulation-1.4.0/lattice/graph/tree.py
+-rw-r--r--   0        0        0       43 2023-04-30 13:12:22.483002 Lattice-Graph-Manipulation-1.4.0/lattice/node/__init__.py
+-rw-r--r--   0        0        0     1399 2023-05-15 13:04:33.398011 Lattice-Graph-Manipulation-1.4.0/lattice/node/node.py
+-rw-r--r--   0        0        0      438 2023-06-14 01:08:38.491601 Lattice-Graph-Manipulation-1.4.0/pyproject.toml
+-rw-r--r--   0        0        0      196 1970-01-01 00:00:00.000000 Lattice-Graph-Manipulation-1.4.0/PKG-INFO
```

### Comparing `Lattice-Graph-Manipulation-1.3.1/LICENSE` & `Lattice-Graph-Manipulation-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `Lattice-Graph-Manipulation-1.3.1/Lattice_Scripts/0c61af02-51eb-402b-afe9-2a1c0cafb88b.gv.pdf` & `Lattice-Graph-Manipulation-1.4.0/Lattice_Scripts/0c61af02-51eb-402b-afe9-2a1c0cafb88b.gv.pdf`

 * *Files identical despite different names*

### Comparing `Lattice-Graph-Manipulation-1.3.1/Lattice_Scripts/22aba17d-0803-40d1-a6d7-f5526b847a82.gv` & `Lattice-Graph-Manipulation-1.4.0/Lattice_Scripts/22aba17d-0803-40d1-a6d7-f5526b847a82.gv`

 * *Files identical despite different names*

### Comparing `Lattice-Graph-Manipulation-1.3.1/Lattice_Scripts/22aba17d-0803-40d1-a6d7-f5526b847a82.gv.pdf` & `Lattice-Graph-Manipulation-1.4.0/Lattice_Scripts/22aba17d-0803-40d1-a6d7-f5526b847a82.gv.pdf`

 * *Files identical despite different names*

### Comparing `Lattice-Graph-Manipulation-1.3.1/Lattice_Scripts/3202f283-fd53-489f-a524-6c2fd4eb742a.gv` & `Lattice-Graph-Manipulation-1.4.0/Lattice_Scripts/3202f283-fd53-489f-a524-6c2fd4eb742a.gv`

 * *Files identical despite different names*

### Comparing `Lattice-Graph-Manipulation-1.3.1/Lattice_Scripts/3202f283-fd53-489f-a524-6c2fd4eb742a.gv.pdf` & `Lattice-Graph-Manipulation-1.4.0/Lattice_Scripts/3202f283-fd53-489f-a524-6c2fd4eb742a.gv.pdf`

 * *Files identical despite different names*

### Comparing `Lattice-Graph-Manipulation-1.3.1/Lattice_Scripts/5ee8c02a-4299-4464-9406-c91d7596a3df.gv` & `Lattice-Graph-Manipulation-1.4.0/Lattice_Scripts/5ee8c02a-4299-4464-9406-c91d7596a3df.gv`

 * *Files identical despite different names*

### Comparing `Lattice-Graph-Manipulation-1.3.1/Lattice_Scripts/5ee8c02a-4299-4464-9406-c91d7596a3df.gv.pdf` & `Lattice-Graph-Manipulation-1.4.0/Lattice_Scripts/5ee8c02a-4299-4464-9406-c91d7596a3df.gv.pdf`

 * *Files identical despite different names*

### Comparing `Lattice-Graph-Manipulation-1.3.1/Lattice_Scripts/6243ae9e-b9ca-4301-bc1b-23820b5b5c67.gv` & `Lattice-Graph-Manipulation-1.4.0/Lattice_Scripts/6243ae9e-b9ca-4301-bc1b-23820b5b5c67.gv`

 * *Files identical despite different names*

### Comparing `Lattice-Graph-Manipulation-1.3.1/Lattice_Scripts/6243ae9e-b9ca-4301-bc1b-23820b5b5c67.gv.pdf` & `Lattice-Graph-Manipulation-1.4.0/Lattice_Scripts/6243ae9e-b9ca-4301-bc1b-23820b5b5c67.gv.pdf`

 * *Files identical despite different names*

### Comparing `Lattice-Graph-Manipulation-1.3.1/Lattice_Scripts/7101765c-cde4-4086-a6cf-85ca9f573d33.gv` & `Lattice-Graph-Manipulation-1.4.0/Lattice_Scripts/7101765c-cde4-4086-a6cf-85ca9f573d33.gv`

 * *Files identical despite different names*

### Comparing `Lattice-Graph-Manipulation-1.3.1/Lattice_Scripts/7101765c-cde4-4086-a6cf-85ca9f573d33.gv.pdf` & `Lattice-Graph-Manipulation-1.4.0/Lattice_Scripts/7101765c-cde4-4086-a6cf-85ca9f573d33.gv.pdf`

 * *Files identical despite different names*

### Comparing `Lattice-Graph-Manipulation-1.3.1/Lattice_Scripts/80d5097d-a203-4423-9177-8db54d9ff8cc.gv` & `Lattice-Graph-Manipulation-1.4.0/Lattice_Scripts/80d5097d-a203-4423-9177-8db54d9ff8cc.gv`

 * *Files identical despite different names*

### Comparing `Lattice-Graph-Manipulation-1.3.1/Lattice_Scripts/80d5097d-a203-4423-9177-8db54d9ff8cc.gv.pdf` & `Lattice-Graph-Manipulation-1.4.0/Lattice_Scripts/80d5097d-a203-4423-9177-8db54d9ff8cc.gv.pdf`

 * *Files identical despite different names*

### Comparing `Lattice-Graph-Manipulation-1.3.1/Lattice_Scripts/8558953d-ec61-4d46-ab51-cad78015e389.gv` & `Lattice-Graph-Manipulation-1.4.0/Lattice_Scripts/8558953d-ec61-4d46-ab51-cad78015e389.gv`

 * *Files identical despite different names*

### Comparing `Lattice-Graph-Manipulation-1.3.1/Lattice_Scripts/8558953d-ec61-4d46-ab51-cad78015e389.gv.pdf` & `Lattice-Graph-Manipulation-1.4.0/Lattice_Scripts/8558953d-ec61-4d46-ab51-cad78015e389.gv.pdf`

 * *Files identical despite different names*

### Comparing `Lattice-Graph-Manipulation-1.3.1/Lattice_Scripts/9167244b-dc36-488e-9a24-8c0f207c3aaa.gv` & `Lattice-Graph-Manipulation-1.4.0/Lattice_Scripts/9167244b-dc36-488e-9a24-8c0f207c3aaa.gv`

 * *Files identical despite different names*

### Comparing `Lattice-Graph-Manipulation-1.3.1/Lattice_Scripts/9167244b-dc36-488e-9a24-8c0f207c3aaa.gv.pdf` & `Lattice-Graph-Manipulation-1.4.0/Lattice_Scripts/9167244b-dc36-488e-9a24-8c0f207c3aaa.gv.pdf`

 * *Files identical despite different names*

### Comparing `Lattice-Graph-Manipulation-1.3.1/Lattice_Scripts/91f695f0-ac92-403e-81d8-f7d76a5a6eba.gv` & `Lattice-Graph-Manipulation-1.4.0/Lattice_Scripts/91f695f0-ac92-403e-81d8-f7d76a5a6eba.gv`

 * *Files identical despite different names*

### Comparing `Lattice-Graph-Manipulation-1.3.1/Lattice_Scripts/91f695f0-ac92-403e-81d8-f7d76a5a6eba.gv.pdf` & `Lattice-Graph-Manipulation-1.4.0/Lattice_Scripts/91f695f0-ac92-403e-81d8-f7d76a5a6eba.gv.pdf`

 * *Files identical despite different names*

### Comparing `Lattice-Graph-Manipulation-1.3.1/Lattice_Scripts/9d8f8c6d-22ed-4a7e-af45-8ac72691f52c.gv` & `Lattice-Graph-Manipulation-1.4.0/Lattice_Scripts/9d8f8c6d-22ed-4a7e-af45-8ac72691f52c.gv`

 * *Files identical despite different names*

### Comparing `Lattice-Graph-Manipulation-1.3.1/Lattice_Scripts/9d8f8c6d-22ed-4a7e-af45-8ac72691f52c.gv.pdf` & `Lattice-Graph-Manipulation-1.4.0/Lattice_Scripts/9d8f8c6d-22ed-4a7e-af45-8ac72691f52c.gv.pdf`

 * *Files identical despite different names*

### Comparing `Lattice-Graph-Manipulation-1.3.1/Lattice_Scripts/a972d228-3f01-42fc-89e8-b0431bcd87b6.gv.pdf` & `Lattice-Graph-Manipulation-1.4.0/Lattice_Scripts/a972d228-3f01-42fc-89e8-b0431bcd87b6.gv.pdf`

 * *Files identical despite different names*

### Comparing `Lattice-Graph-Manipulation-1.3.1/Lattice_Scripts/bb_tree.py` & `Lattice-Graph-Manipulation-1.4.0/Lattice_Scripts/bb_tree.py`

 * *Files identical despite different names*

### Comparing `Lattice-Graph-Manipulation-1.3.1/Lattice_Scripts/ce8e0387-b735-400d-a303-cc56e4769a9b.gv` & `Lattice-Graph-Manipulation-1.4.0/Lattice_Scripts/ce8e0387-b735-400d-a303-cc56e4769a9b.gv`

 * *Files identical despite different names*

### Comparing `Lattice-Graph-Manipulation-1.3.1/Lattice_Scripts/ce8e0387-b735-400d-a303-cc56e4769a9b.gv.pdf` & `Lattice-Graph-Manipulation-1.4.0/Lattice_Scripts/ce8e0387-b735-400d-a303-cc56e4769a9b.gv.pdf`

 * *Files identical despite different names*

### Comparing `Lattice-Graph-Manipulation-1.3.1/Lattice_Scripts/d962d2ca-0365-46f3-9b0e-3c07645b036d.gv` & `Lattice-Graph-Manipulation-1.4.0/Lattice_Scripts/d962d2ca-0365-46f3-9b0e-3c07645b036d.gv`

 * *Files identical despite different names*

### Comparing `Lattice-Graph-Manipulation-1.3.1/Lattice_Scripts/d962d2ca-0365-46f3-9b0e-3c07645b036d.gv.pdf` & `Lattice-Graph-Manipulation-1.4.0/Lattice_Scripts/d962d2ca-0365-46f3-9b0e-3c07645b036d.gv.pdf`

 * *Files identical despite different names*

### Comparing `Lattice-Graph-Manipulation-1.3.1/Lattice_Scripts/dot_output/124ce352-4606-4b8e-83cf-894a431e02f5.gv` & `Lattice-Graph-Manipulation-1.4.0/Lattice_Scripts/dot_output/124ce352-4606-4b8e-83cf-894a431e02f5.gv`

 * *Files identical despite different names*

### Comparing `Lattice-Graph-Manipulation-1.3.1/Lattice_Scripts/dot_output/124ce352-4606-4b8e-83cf-894a431e02f5.gv.pdf` & `Lattice-Graph-Manipulation-1.4.0/Lattice_Scripts/dot_output/124ce352-4606-4b8e-83cf-894a431e02f5.gv.pdf`

 * *Files identical despite different names*

### Comparing `Lattice-Graph-Manipulation-1.3.1/Lattice_Scripts/dot_output/18839347-7fff-4bf6-b283-22b194da1d73.gv` & `Lattice-Graph-Manipulation-1.4.0/Lattice_Scripts/dot_output/18839347-7fff-4bf6-b283-22b194da1d73.gv`

 * *Files identical despite different names*

### Comparing `Lattice-Graph-Manipulation-1.3.1/Lattice_Scripts/dot_output/18839347-7fff-4bf6-b283-22b194da1d73.gv.pdf` & `Lattice-Graph-Manipulation-1.4.0/Lattice_Scripts/dot_output/18839347-7fff-4bf6-b283-22b194da1d73.gv.pdf`

 * *Files identical despite different names*

### Comparing `Lattice-Graph-Manipulation-1.3.1/Lattice_Scripts/dot_output/2b89469f-7c20-4e83-987a-243eed3f15b0.gv` & `Lattice-Graph-Manipulation-1.4.0/Lattice_Scripts/dot_output/2b89469f-7c20-4e83-987a-243eed3f15b0.gv`

 * *Files identical despite different names*

### Comparing `Lattice-Graph-Manipulation-1.3.1/Lattice_Scripts/dot_output/2b89469f-7c20-4e83-987a-243eed3f15b0.gv.pdf` & `Lattice-Graph-Manipulation-1.4.0/Lattice_Scripts/dot_output/2b89469f-7c20-4e83-987a-243eed3f15b0.gv.pdf`

 * *Files identical despite different names*

### Comparing `Lattice-Graph-Manipulation-1.3.1/Lattice_Scripts/dot_output/4d9238b6-e314-4c1d-8fe0-851f2237e653.gv` & `Lattice-Graph-Manipulation-1.4.0/Lattice_Scripts/dot_output/4d9238b6-e314-4c1d-8fe0-851f2237e653.gv`

 * *Files identical despite different names*

### Comparing `Lattice-Graph-Manipulation-1.3.1/Lattice_Scripts/dot_output/4d9238b6-e314-4c1d-8fe0-851f2237e653.gv.pdf` & `Lattice-Graph-Manipulation-1.4.0/Lattice_Scripts/dot_output/4d9238b6-e314-4c1d-8fe0-851f2237e653.gv.pdf`

 * *Files identical despite different names*

### Comparing `Lattice-Graph-Manipulation-1.3.1/Lattice_Scripts/dot_output/6dd10e1b-c98d-4a1f-8297-302f270b51da.gv` & `Lattice-Graph-Manipulation-1.4.0/Lattice_Scripts/dot_output/6dd10e1b-c98d-4a1f-8297-302f270b51da.gv`

 * *Files identical despite different names*

### Comparing `Lattice-Graph-Manipulation-1.3.1/Lattice_Scripts/dot_output/6dd10e1b-c98d-4a1f-8297-302f270b51da.gv.pdf` & `Lattice-Graph-Manipulation-1.4.0/Lattice_Scripts/dot_output/6dd10e1b-c98d-4a1f-8297-302f270b51da.gv.pdf`

 * *Files identical despite different names*

### Comparing `Lattice-Graph-Manipulation-1.3.1/Lattice_Scripts/dot_output/721f21a0-d8ee-4cfd-acfb-67b3b4021d94.gv` & `Lattice-Graph-Manipulation-1.4.0/Lattice_Scripts/dot_output/721f21a0-d8ee-4cfd-acfb-67b3b4021d94.gv`

 * *Files identical despite different names*

### Comparing `Lattice-Graph-Manipulation-1.3.1/Lattice_Scripts/dot_output/721f21a0-d8ee-4cfd-acfb-67b3b4021d94.gv.pdf` & `Lattice-Graph-Manipulation-1.4.0/Lattice_Scripts/dot_output/721f21a0-d8ee-4cfd-acfb-67b3b4021d94.gv.pdf`

 * *Files identical despite different names*

### Comparing `Lattice-Graph-Manipulation-1.3.1/Lattice_Scripts/dot_output/782355df-1bc9-4714-85ed-65e312e0396b.gv` & `Lattice-Graph-Manipulation-1.4.0/Lattice_Scripts/dot_output/782355df-1bc9-4714-85ed-65e312e0396b.gv`

 * *Files identical despite different names*

### Comparing `Lattice-Graph-Manipulation-1.3.1/Lattice_Scripts/dot_output/782355df-1bc9-4714-85ed-65e312e0396b.gv.pdf` & `Lattice-Graph-Manipulation-1.4.0/Lattice_Scripts/dot_output/782355df-1bc9-4714-85ed-65e312e0396b.gv.pdf`

 * *Files identical despite different names*

### Comparing `Lattice-Graph-Manipulation-1.3.1/Lattice_Scripts/dot_output/7b10a609-60ba-416a-8572-7e3ebf8c1bc5.gv` & `Lattice-Graph-Manipulation-1.4.0/Lattice_Scripts/dot_output/7b10a609-60ba-416a-8572-7e3ebf8c1bc5.gv`

 * *Files identical despite different names*

### Comparing `Lattice-Graph-Manipulation-1.3.1/Lattice_Scripts/dot_output/7b10a609-60ba-416a-8572-7e3ebf8c1bc5.gv.pdf` & `Lattice-Graph-Manipulation-1.4.0/Lattice_Scripts/dot_output/7b10a609-60ba-416a-8572-7e3ebf8c1bc5.gv.pdf`

 * *Files identical despite different names*

### Comparing `Lattice-Graph-Manipulation-1.3.1/Lattice_Scripts/dot_output/85690484-fe37-4e5f-9c48-d61eb19c0e86.gv` & `Lattice-Graph-Manipulation-1.4.0/Lattice_Scripts/dot_output/85690484-fe37-4e5f-9c48-d61eb19c0e86.gv`

 * *Files identical despite different names*

### Comparing `Lattice-Graph-Manipulation-1.3.1/Lattice_Scripts/dot_output/85690484-fe37-4e5f-9c48-d61eb19c0e86.gv.pdf` & `Lattice-Graph-Manipulation-1.4.0/Lattice_Scripts/dot_output/85690484-fe37-4e5f-9c48-d61eb19c0e86.gv.pdf`

 * *Files identical despite different names*

### Comparing `Lattice-Graph-Manipulation-1.3.1/Lattice_Scripts/dot_output/89621631-a0d6-4cf1-b1d6-98bee69eafd6.gv` & `Lattice-Graph-Manipulation-1.4.0/Lattice_Scripts/dot_output/89621631-a0d6-4cf1-b1d6-98bee69eafd6.gv`

 * *Files identical despite different names*

### Comparing `Lattice-Graph-Manipulation-1.3.1/Lattice_Scripts/dot_output/89621631-a0d6-4cf1-b1d6-98bee69eafd6.gv.pdf` & `Lattice-Graph-Manipulation-1.4.0/Lattice_Scripts/dot_output/89621631-a0d6-4cf1-b1d6-98bee69eafd6.gv.pdf`

 * *Files identical despite different names*

### Comparing `Lattice-Graph-Manipulation-1.3.1/Lattice_Scripts/dot_output/8a952fcc-a0a5-4902-9942-cb18880ee393.gv` & `Lattice-Graph-Manipulation-1.4.0/Lattice_Scripts/dot_output/8a952fcc-a0a5-4902-9942-cb18880ee393.gv`

 * *Files identical despite different names*

### Comparing `Lattice-Graph-Manipulation-1.3.1/Lattice_Scripts/dot_output/8a952fcc-a0a5-4902-9942-cb18880ee393.gv.pdf` & `Lattice-Graph-Manipulation-1.4.0/Lattice_Scripts/dot_output/8a952fcc-a0a5-4902-9942-cb18880ee393.gv.pdf`

 * *Files identical despite different names*

### Comparing `Lattice-Graph-Manipulation-1.3.1/Lattice_Scripts/dot_output/98af54bc-3975-4394-804d-66789065d1c9.gv` & `Lattice-Graph-Manipulation-1.4.0/Lattice_Scripts/dot_output/98af54bc-3975-4394-804d-66789065d1c9.gv`

 * *Files identical despite different names*

### Comparing `Lattice-Graph-Manipulation-1.3.1/Lattice_Scripts/dot_output/98af54bc-3975-4394-804d-66789065d1c9.gv.pdf` & `Lattice-Graph-Manipulation-1.4.0/Lattice_Scripts/dot_output/98af54bc-3975-4394-804d-66789065d1c9.gv.pdf`

 * *Files identical despite different names*

### Comparing `Lattice-Graph-Manipulation-1.3.1/Lattice_Scripts/dot_output/b68224e8-ee0f-43bd-ad54-cbb0bc805f8e.gv.pdf` & `Lattice-Graph-Manipulation-1.4.0/Lattice_Scripts/dot_output/b68224e8-ee0f-43bd-ad54-cbb0bc805f8e.gv.pdf`

 * *Files identical despite different names*

### Comparing `Lattice-Graph-Manipulation-1.3.1/Lattice_Scripts/dot_output/bdea7672-3cf4-48bc-861a-86787c8e9122.gv` & `Lattice-Graph-Manipulation-1.4.0/Lattice_Scripts/dot_output/bdea7672-3cf4-48bc-861a-86787c8e9122.gv`

 * *Files identical despite different names*

### Comparing `Lattice-Graph-Manipulation-1.3.1/Lattice_Scripts/dot_output/bdea7672-3cf4-48bc-861a-86787c8e9122.gv.pdf` & `Lattice-Graph-Manipulation-1.4.0/Lattice_Scripts/dot_output/bdea7672-3cf4-48bc-861a-86787c8e9122.gv.pdf`

 * *Files identical despite different names*

### Comparing `Lattice-Graph-Manipulation-1.3.1/Lattice_Scripts/dot_output/c04b2718-239f-4811-8f73-d78111718784.gv.pdf` & `Lattice-Graph-Manipulation-1.4.0/Lattice_Scripts/dot_output/c04b2718-239f-4811-8f73-d78111718784.gv.pdf`

 * *Files identical despite different names*

### Comparing `Lattice-Graph-Manipulation-1.3.1/Lattice_Scripts/dot_output/d1456d21-9a4f-4356-8f63-dd10573cf1b9.gv` & `Lattice-Graph-Manipulation-1.4.0/Lattice_Scripts/dot_output/d1456d21-9a4f-4356-8f63-dd10573cf1b9.gv`

 * *Files identical despite different names*

### Comparing `Lattice-Graph-Manipulation-1.3.1/Lattice_Scripts/dot_output/d1456d21-9a4f-4356-8f63-dd10573cf1b9.gv.pdf` & `Lattice-Graph-Manipulation-1.4.0/Lattice_Scripts/dot_output/d1456d21-9a4f-4356-8f63-dd10573cf1b9.gv.pdf`

 * *Files identical despite different names*

### Comparing `Lattice-Graph-Manipulation-1.3.1/Lattice_Scripts/dot_output/f814a715-e5ec-4cab-85bd-746f5d0dcb84.gv` & `Lattice-Graph-Manipulation-1.4.0/Lattice_Scripts/dot_output/f814a715-e5ec-4cab-85bd-746f5d0dcb84.gv`

 * *Files identical despite different names*

### Comparing `Lattice-Graph-Manipulation-1.3.1/Lattice_Scripts/dot_output/f814a715-e5ec-4cab-85bd-746f5d0dcb84.gv.pdf` & `Lattice-Graph-Manipulation-1.4.0/Lattice_Scripts/dot_output/f814a715-e5ec-4cab-85bd-746f5d0dcb84.gv.pdf`

 * *Files identical despite different names*

### Comparing `Lattice-Graph-Manipulation-1.3.1/Lattice_Scripts/dot_output/fb51fde2-173b-4824-91c0-0b1036767689.gv` & `Lattice-Graph-Manipulation-1.4.0/Lattice_Scripts/dot_output/fb51fde2-173b-4824-91c0-0b1036767689.gv`

 * *Files identical despite different names*

### Comparing `Lattice-Graph-Manipulation-1.3.1/Lattice_Scripts/dot_output/fb51fde2-173b-4824-91c0-0b1036767689.gv.pdf` & `Lattice-Graph-Manipulation-1.4.0/Lattice_Scripts/dot_output/fb51fde2-173b-4824-91c0-0b1036767689.gv.pdf`

 * *Files identical despite different names*

### Comparing `Lattice-Graph-Manipulation-1.3.1/Lattice_Scripts/e9422bf1-3455-4d4a-afc9-de9fca5ae2f7.gv` & `Lattice-Graph-Manipulation-1.4.0/Lattice_Scripts/e9422bf1-3455-4d4a-afc9-de9fca5ae2f7.gv`

 * *Files identical despite different names*

### Comparing `Lattice-Graph-Manipulation-1.3.1/Lattice_Scripts/e9422bf1-3455-4d4a-afc9-de9fca5ae2f7.gv.pdf` & `Lattice-Graph-Manipulation-1.4.0/Lattice_Scripts/e9422bf1-3455-4d4a-afc9-de9fca5ae2f7.gv.pdf`

 * *Files identical despite different names*

### Comparing `Lattice-Graph-Manipulation-1.3.1/Lattice_Scripts/f99dc209-e23f-406f-8d61-5e0943af8836.gv.pdf` & `Lattice-Graph-Manipulation-1.4.0/Lattice_Scripts/f99dc209-e23f-406f-8d61-5e0943af8836.gv.pdf`

 * *Files identical despite different names*

### Comparing `Lattice-Graph-Manipulation-1.3.1/Lattice_Scripts/grid_example.py` & `Lattice-Graph-Manipulation-1.4.0/Lattice_Scripts/grid_example.py`

 * *Files identical despite different names*

### Comparing `Lattice-Graph-Manipulation-1.3.1/Lattice_Scripts/simple_examples.py` & `Lattice-Graph-Manipulation-1.4.0/Lattice_Scripts/simple_examples.py`

 * *Files identical despite different names*

### Comparing `Lattice-Graph-Manipulation-1.3.1/Lattice_Scripts/simple_graph.py` & `Lattice-Graph-Manipulation-1.4.0/Lattice_Scripts/simple_graph.py`

 * *Files identical despite different names*

### Comparing `Lattice-Graph-Manipulation-1.3.1/lattice/edge/edge.py` & `Lattice-Graph-Manipulation-1.4.0/lattice/edge/edge.py`

 * *Files identical despite different names*

### Comparing `Lattice-Graph-Manipulation-1.3.1/lattice/graph/bbtree.py` & `Lattice-Graph-Manipulation-1.4.0/lattice/graph/bbtree.py`

 * *Files identical despite different names*

### Comparing `Lattice-Graph-Manipulation-1.3.1/lattice/graph/graph.py` & `Lattice-Graph-Manipulation-1.4.0/lattice/graph/graph.py`

 * *Files 3% similar despite different names*

```diff
@@ -41,17 +41,22 @@
     def add_node(self, node: Node, label):
         """Create a node within the graph"""
         self._nodes[label] = node
 
     def get_node(self, name: str):
         return self._nodes.get(name)
 
-    def deepcopy(self):
-        """Return a network of nodes encased by this graph, but copied"""
-        new_graph = Graph()
+    def deepcopy(self, input_graph):
+        """Return a network of nodes encased by this graph, but copied
+        if an input graph is given add the new nodes there instead
+        """
+        if input_graph:
+            new_graph = input_graph
+        else:
+            new_graph = Graph()
         explored = {}
         for name, node in self.nodes.items():
             if node not in explored:
                 new_node = node.copy(label=node.get_label())
                 explored[node] = new_node
                 new_graph.add_nodes(**{name: new_node})
                 explored = self._recursive_copier(new_node, node, explored, new_graph)
```

### Comparing `Lattice-Graph-Manipulation-1.3.1/lattice/graph/tree.py` & `Lattice-Graph-Manipulation-1.4.0/lattice/graph/tree.py`

 * *Files identical despite different names*

### Comparing `Lattice-Graph-Manipulation-1.3.1/lattice/node/node.py` & `Lattice-Graph-Manipulation-1.4.0/lattice/node/node.py`

 * *Files identical despite different names*

