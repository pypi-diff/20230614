# Comparing `tmp/soil-sdk-0.6.8.dev2.tar.gz` & `tmp/soil-sdk-0.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "soil-sdk-0.6.8.dev2.tar", last modified: Fri Mar 10 09:30:31 2023, max compression
+gzip compressed data, was "soil-sdk-0.6.9.tar", last modified: Wed Mar 22 10:23:33 2023, max compression
```

## Comparing `soil-sdk-0.6.8.dev2.tar` & `soil-sdk-0.6.9.tar`

### file list

```diff
@@ -1,465 +1,465 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-10 09:30:31.671071 soil-sdk-0.6.8.dev2/
--rw-rw-rw-   0 root         (0) root         (0)    53248 2023-03-10 09:30:26.000000 soil-sdk-0.6.8.dev2/.coverage
--rw-rw-rw-   0 root         (0) root         (0)      877 2023-03-10 09:30:26.000000 soil-sdk-0.6.8.dev2/.gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)     1580 2023-03-09 09:42:09.000000 soil-sdk-0.6.8.dev2/.pre-commit-config.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-10 09:30:31.631070 soil-sdk-0.6.8.dev2/.vscode/
--rw-rw-rw-   0 root         (0) root         (0)      370 2022-09-02 11:29:48.000000 soil-sdk-0.6.8.dev2/.vscode/launch.json
--rw-rw-rw-   0 root         (0) root         (0)      611 2022-09-02 11:29:48.000000 soil-sdk-0.6.8.dev2/.vscode/settings.json
--rw-rw-rw-   0 root         (0) root         (0)      202 2023-03-10 09:30:31.000000 soil-sdk-0.6.8.dev2/AUTHORS
--rw-rw-rw-   0 root         (0) root         (0)     2981 2023-03-10 09:30:31.000000 soil-sdk-0.6.8.dev2/ChangeLog
--rw-r--r--   0 root         (0) root         (0)     1663 2023-03-10 09:30:31.671071 soil-sdk-0.6.8.dev2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1330 2023-03-10 09:30:26.000000 soil-sdk-0.6.8.dev2/README.md
--rw-rw-rw-   0 root         (0) root         (0)       16 2022-09-06 12:27:32.000000 soil-sdk-0.6.8.dev2/bandit.yml
--rw-rw-rw-   0 root         (0) root         (0)      221 2022-09-02 11:29:48.000000 soil-sdk-0.6.8.dev2/dependabot.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-10 09:30:31.631070 soil-sdk-0.6.8.dev2/docker/
--rw-rw-rw-   0 root         (0) root         (0)      395 2023-03-10 09:05:11.000000 soil-sdk-0.6.8.dev2/docker/Dockerfile-test
--rw-rw-rw-   0 root         (0) root         (0)      140 2023-03-09 10:25:17.000000 soil-sdk-0.6.8.dev2/docker/docker-compose-test.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-10 09:30:31.631070 soil-sdk-0.6.8.dev2/docs/
--rw-rw-rw-   0 root         (0) root         (0)       21 2022-09-02 11:29:48.000000 soil-sdk-0.6.8.dev2/docs/.dockerignore
--rw-rw-rw-   0 root         (0) root         (0)      165 2022-09-02 11:29:48.000000 soil-sdk-0.6.8.dev2/docs/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)      145 2022-09-02 11:29:48.000000 soil-sdk-0.6.8.dev2/docs/Dockerfile
--rw-rw-rw-   0 root         (0) root         (0)      497 2022-09-02 11:29:48.000000 soil-sdk-0.6.8.dev2/docs/docker-compose.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-10 09:30:31.631070 soil-sdk-0.6.8.dev2/docs/docs/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-10 09:30:31.631070 soil-sdk-0.6.8.dev2/docs/docs/assets/
--rw-rw-rw-   0 root         (0) root         (0)    19945 2022-09-02 11:29:48.000000 soil-sdk-0.6.8.dev2/docs/docs/assets/example-app-dir.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-10 09:30:31.631070 soil-sdk-0.6.8.dev2/docs/docs/sdk-reference/
--rw-rw-rw-   0 root         (0) root         (0)      980 2022-09-02 11:29:48.000000 soil-sdk-0.6.8.dev2/docs/docs/sdk-reference/sidebar.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-10 09:30:31.635071 soil-sdk-0.6.8.dev2/docs/docs/sdk-reference/soil/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-10 09:30:31.635071 soil-sdk-0.6.8.dev2/docs/docs/sdk-reference/soil/alerts/
--rw-rw-rw-   0 root         (0) root         (0)      277 2022-09-02 11:29:48.000000 soil-sdk-0.6.8.dev2/docs/docs/sdk-reference/soil/alerts/alerts.md
--rw-rw-rw-   0 root         (0) root         (0)      278 2022-09-02 11:29:48.000000 soil-sdk-0.6.8.dev2/docs/docs/sdk-reference/soil/alias.md
--rw-rw-rw-   0 root         (0) root         (0)     2135 2022-09-02 11:29:48.000000 soil-sdk-0.6.8.dev2/docs/docs/sdk-reference/soil/api.md
--rw-rw-rw-   0 root         (0) root         (0)      528 2022-09-02 11:29:48.000000 soil-sdk-0.6.8.dev2/docs/docs/sdk-reference/soil/configuration.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-10 09:30:31.635071 soil-sdk-0.6.8.dev2/docs/docs/sdk-reference/soil/connectors/
--rw-rw-rw-   0 root         (0) root         (0)      917 2022-09-02 11:29:48.000000 soil-sdk-0.6.8.dev2/docs/docs/sdk-reference/soil/connectors/elastic_search.md
--rw-rw-rw-   0 root         (0) root         (0)      240 2022-09-02 11:29:48.000000 soil-sdk-0.6.8.dev2/docs/docs/sdk-reference/soil/data.md
--rw-rw-rw-   0 root         (0) root         (0)      838 2022-09-02 11:29:48.000000 soil-sdk-0.6.8.dev2/docs/docs/sdk-reference/soil/data_structure.md
--rw-rw-rw-   0 root         (0) root         (0)      542 2022-09-02 11:29:48.000000 soil-sdk-0.6.8.dev2/docs/docs/sdk-reference/soil/decorator.md
--rw-rw-rw-   0 root         (0) root         (0)      302 2022-09-02 11:29:48.000000 soil-sdk-0.6.8.dev2/docs/docs/sdk-reference/soil/dictionary.md
--rw-rw-rw-   0 root         (0) root         (0)     2520 2022-09-02 11:29:48.000000 soil-sdk-0.6.8.dev2/docs/docs/sdk-reference/soil/errors.md
--rw-rw-rw-   0 root         (0) root         (0)     1077 2022-09-02 11:29:48.000000 soil-sdk-0.6.8.dev2/docs/docs/sdk-reference/soil/finder.md
--rw-rw-rw-   0 root         (0) root         (0)      545 2022-09-02 11:29:48.000000 soil-sdk-0.6.8.dev2/docs/docs/sdk-reference/soil/modulify.md
--rw-rw-rw-   0 root         (0) root         (0)      756 2022-09-02 11:29:48.000000 soil-sdk-0.6.8.dev2/docs/docs/sdk-reference/soil/pipeline.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-10 09:30:31.635071 soil-sdk-0.6.8.dev2/docs/docs/sdk-reference/soil/storage/
--rw-rw-rw-   0 root         (0) root         (0)      622 2022-09-02 11:29:48.000000 soil-sdk-0.6.8.dev2/docs/docs/sdk-reference/soil/storage/base_storage.md
--rw-rw-rw-   0 root         (0) root         (0)     1017 2022-09-02 11:29:48.000000 soil-sdk-0.6.8.dev2/docs/docs/sdk-reference/soil/storage/compound_storage.md
--rw-rw-rw-   0 root         (0) root         (0)     1245 2022-09-02 11:29:48.000000 soil-sdk-0.6.8.dev2/docs/docs/sdk-reference/soil/storage/elasticsearch.md
--rw-rw-rw-   0 root         (0) root         (0)     1415 2022-09-02 11:29:48.000000 soil-sdk-0.6.8.dev2/docs/docs/sdk-reference/soil/storage/object_storage.md
--rw-rw-rw-   0 root         (0) root         (0)      599 2022-09-02 11:29:48.000000 soil-sdk-0.6.8.dev2/docs/docs/sdk-reference/soil/task.md
--rw-rw-rw-   0 root         (0) root         (0)      466 2022-09-02 11:29:48.000000 soil-sdk-0.6.8.dev2/docs/docs/sdk-reference/soil/types.md
--rw-rw-rw-   0 root         (0) root         (0)     1585 2022-09-02 11:29:48.000000 soil-sdk-0.6.8.dev2/docs/docs/sdk-reference/soil/utils.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-10 09:30:31.635071 soil-sdk-0.6.8.dev2/docs/docs/soil-library/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-10 09:30:31.635071 soil-sdk-0.6.8.dev2/docs/docs/soil-library/data_structures/
--rw-rw-rw-   0 root         (0) root         (0)      166 2022-09-02 11:29:48.000000 soil-sdk-0.6.8.dev2/docs/docs/soil-library/data_structures/NBClusters.md
--rw-rw-rw-   0 root         (0) root         (0)     1702 2022-09-02 11:29:48.000000 soil-sdk-0.6.8.dev2/docs/docs/soil-library/data_structures/data_structure.md
--rw-rw-rw-   0 root         (0) root         (0)      209 2022-09-02 11:29:48.000000 soil-sdk-0.6.8.dev2/docs/docs/soil-library/data_structures/frequent_itemsets.md
--rw-rw-rw-   0 root         (0) root         (0)      809 2022-09-02 11:29:48.000000 soil-sdk-0.6.8.dev2/docs/docs/soil-library/data_structures/hypergraph.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-10 09:30:31.635071 soil-sdk-0.6.8.dev2/docs/docs/soil-library/data_structures/predefined/
--rw-rw-rw-   0 root         (0) root         (0)      351 2022-09-02 11:29:48.000000 soil-sdk-0.6.8.dev2/docs/docs/soil-library/data_structures/predefined/dict.md
--rw-rw-rw-   0 root         (0) root         (0)      351 2022-09-02 11:29:48.000000 soil-sdk-0.6.8.dev2/docs/docs/soil-library/data_structures/predefined/list.md
--rw-rw-rw-   0 root         (0) root         (0)      378 2022-09-02 11:29:48.000000 soil-sdk-0.6.8.dev2/docs/docs/soil-library/data_structures/predefined/ndarray.md
--rw-rw-rw-   0 root         (0) root         (0)      505 2022-09-02 11:29:48.000000 soil-sdk-0.6.8.dev2/docs/docs/soil-library/data_structures/predefined/object_ds.md
--rw-rw-rw-   0 root         (0) root         (0)      401 2022-09-02 11:29:48.000000 soil-sdk-0.6.8.dev2/docs/docs/soil-library/data_structures/predefined/pd_data_frame.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-10 09:30:31.635071 soil-sdk-0.6.8.dev2/docs/docs/soil-library/data_structures/streams/
--rw-rw-rw-   0 root         (0) root         (0)      512 2022-09-02 11:29:48.000000 soil-sdk-0.6.8.dev2/docs/docs/soil-library/data_structures/streams/patients.md
--rw-rw-rw-   0 root         (0) root         (0)      348 2022-09-02 11:29:48.000000 soil-sdk-0.6.8.dev2/docs/docs/soil-library/data_structures/streams/stream.md
--rw-rw-rw-   0 root         (0) root         (0)      474 2022-09-02 11:29:48.000000 soil-sdk-0.6.8.dev2/docs/docs/soil-library/data_structures/streams/trajectory_clusters.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-10 09:30:31.635071 soil-sdk-0.6.8.dev2/docs/docs/soil-library/modules/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-10 09:30:31.635071 soil-sdk-0.6.8.dev2/docs/docs/soil-library/modules/clustering/
--rw-rw-rw-   0 root         (0) root         (0)     1263 2022-09-02 11:29:48.000000 soil-sdk-0.6.8.dev2/docs/docs/soil-library/modules/clustering/NBClustering.md
--rw-rw-rw-   0 root         (0) root         (0)      892 2022-09-02 11:29:48.000000 soil-sdk-0.6.8.dev2/docs/docs/soil-library/modules/clustering/NBClustering_categorical.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-10 09:30:31.635071 soil-sdk-0.6.8.dev2/docs/docs/soil-library/modules/clustering/SIDIWO/
--rw-rw-rw-   0 root         (0) root         (0)     1815 2022-09-02 11:29:48.000000 soil-sdk-0.6.8.dev2/docs/docs/soil-library/modules/clustering/SIDIWO/sidiwo.md
--rw-rw-rw-   0 root         (0) root         (0)      412 2022-09-02 11:29:48.000000 soil-sdk-0.6.8.dev2/docs/docs/soil-library/modules/experiment.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-10 09:30:31.635071 soil-sdk-0.6.8.dev2/docs/docs/soil-library/modules/higher_order/
--rw-rw-rw-   0 root         (0) root         (0)     1673 2022-09-02 11:29:48.000000 soil-sdk-0.6.8.dev2/docs/docs/soil-library/modules/higher_order/Predictor.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-10 09:30:31.635071 soil-sdk-0.6.8.dev2/docs/docs/soil-library/modules/itemsets/
--rw-rw-rw-   0 root         (0) root         (0)      353 2022-09-02 11:29:48.000000 soil-sdk-0.6.8.dev2/docs/docs/soil-library/modules/itemsets/frequent_itemsets_compare.md
--rw-rw-rw-   0 root         (0) root         (0)      297 2022-09-02 11:29:48.000000 soil-sdk-0.6.8.dev2/docs/docs/soil-library/modules/itemsets/frequent_itemsets_hypergraph.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-10 09:30:31.631070 soil-sdk-0.6.8.dev2/docs/docs/soil-library/modules/preprocessing/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-10 09:30:31.635071 soil-sdk-0.6.8.dev2/docs/docs/soil-library/modules/preprocessing/filters/
--rw-rw-rw-   0 root         (0) root         (0)      222 2022-09-02 11:29:48.000000 soil-sdk-0.6.8.dev2/docs/docs/soil-library/modules/preprocessing/filters/events_filter.md
--rw-rw-rw-   0 root         (0) root         (0)      884 2022-09-02 11:29:48.000000 soil-sdk-0.6.8.dev2/docs/docs/soil-library/modules/preprocessing/filters/row_filter.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-10 09:30:31.635071 soil-sdk-0.6.8.dev2/docs/docs/soil-library/modules/statistics/
--rw-rw-rw-   0 root         (0) root         (0)      276 2022-09-02 11:29:48.000000 soil-sdk-0.6.8.dev2/docs/docs/soil-library/modules/statistics/customstatistics.md
--rw-rw-rw-   0 root         (0) root         (0)      273 2022-09-02 11:29:48.000000 soil-sdk-0.6.8.dev2/docs/docs/soil-library/modules/statistics/time_statistics.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-10 09:30:31.635071 soil-sdk-0.6.8.dev2/docs/docs/soil-library/modules/temporal/
--rw-rw-rw-   0 root         (0) root         (0)      959 2022-09-02 11:29:48.000000 soil-sdk-0.6.8.dev2/docs/docs/soil-library/modules/temporal/trajectories.md
--rw-rw-rw-   0 root         (0) root         (0)     2821 2022-09-02 11:29:48.000000 soil-sdk-0.6.8.dev2/docs/docs/soil-library/sidebar.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-10 09:30:31.639071 soil-sdk-0.6.8.dev2/docs/docs/tutorial/
--rw-rw-rw-   0 root         (0) root         (0)     2719 2022-09-02 11:29:48.000000 soil-sdk-0.6.8.dev2/docs/docs/tutorial/alerts.md
--rw-rw-rw-   0 root         (0) root         (0)     3905 2022-09-02 11:29:48.000000 soil-sdk-0.6.8.dev2/docs/docs/tutorial/data-structures.md
--rw-rw-rw-   0 root         (0) root         (0)     2540 2022-09-02 11:29:48.000000 soil-sdk-0.6.8.dev2/docs/docs/tutorial/data.md
--rw-rw-rw-   0 root         (0) root         (0)     1486 2022-09-02 11:29:48.000000 soil-sdk-0.6.8.dev2/docs/docs/tutorial/deployments.md
--rw-rw-rw-   0 root         (0) root         (0)     2917 2023-03-07 10:10:25.000000 soil-sdk-0.6.8.dev2/docs/docs/tutorial/get-started.mdx
--rw-rw-rw-   0 root         (0) root         (0)     2681 2022-09-02 11:29:48.000000 soil-sdk-0.6.8.dev2/docs/docs/tutorial/logging.md
--rw-rw-rw-   0 root         (0) root         (0)     2847 2022-09-02 11:29:48.000000 soil-sdk-0.6.8.dev2/docs/docs/tutorial/modules.md
--rw-rw-rw-   0 root         (0) root         (0)      672 2022-09-02 11:29:48.000000 soil-sdk-0.6.8.dev2/docs/docs/tutorial/notebooks.md
--rw-rw-rw-   0 root         (0) root         (0)     1942 2022-09-02 11:29:48.000000 soil-sdk-0.6.8.dev2/docs/docs/tutorial/scripts.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-10 09:30:31.639071 soil-sdk-0.6.8.dev2/docs/website/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-10 09:30:31.639071 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/
--rw-rw-rw-   0 root         (0) root         (0)      260 2023-02-17 10:34:02.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/DONT-EDIT-THIS-FOLDER
--rw-rw-rw-   0 root         (0) root         (0)    20016 2023-02-17 10:34:02.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/client-manifest.json
--rw-rw-rw-   0 root         (0) root         (0)      697 2023-02-17 10:34:02.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/client-modules.js
--rw-rw-rw-   0 root         (0) root         (0)        2 2023-02-17 10:34:02.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/codeTranslations.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-10 09:30:31.631070 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-blog/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-10 09:30:31.639071 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-blog/default/
--rw-rw-rw-   0 root         (0) root         (0)    13142 2023-02-17 10:34:02.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-blog/default/blog-archive-80c.json
--rw-rw-rw-   0 root         (0) root         (0)      151 2023-02-17 10:34:02.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-blog/default/blog-c06.json
--rw-rw-rw-   0 root         (0) root         (0)      559 2023-02-17 10:34:02.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-blog/default/blog-post-list-prop-default.json
--rw-rw-rw-   0 root         (0) root         (0)       65 2023-02-17 10:34:02.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-blog/default/plugin-route-context-module-100.json
--rw-rw-rw-   0 root         (0) root         (0)     1073 2023-02-17 10:34:02.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-blog/default/site-blog-2016-03-11-blog-post-md-bf9.json
--rw-rw-rw-   0 root         (0) root         (0)     1206 2023-02-17 10:34:02.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-blog/default/site-blog-2017-04-10-blog-post-two-md-dfa.json
--rw-rw-rw-   0 root         (0) root         (0)     1071 2023-02-17 10:34:02.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-blog/default/site-blog-2017-09-25-testing-rss-md-4d8.json
--rw-rw-rw-   0 root         (0) root         (0)      827 2023-02-17 10:34:02.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-blog/default/site-blog-2017-09-26-adding-rss-md-ad7.json
--rw-rw-rw-   0 root         (0) root         (0)      760 2023-02-17 10:34:02.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-blog/default/site-blog-2017-10-24-new-version-1-0-0-md-bbb.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-10 09:30:31.631070 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-10 09:30:31.663071 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/
--rw-rw-rw-   0 root         (0) root         (0)       65 2023-02-17 10:34:02.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/plugin-route-context-module-100.json
--rw-rw-rw-   0 root         (0) root         (0)      633 2022-09-02 11:29:48.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-docs-sdk-reference-soil-alias-md-698.json
--rw-rw-rw-   0 root         (0) root         (0)      614 2022-09-02 11:29:48.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-docs-sdk-reference-soil-api-md-fbe.json
--rw-rw-rw-   0 root         (0) root         (0)      684 2022-09-02 11:29:48.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-docs-sdk-reference-soil-cli-soil-cli-md-727.json
--rw-rw-rw-   0 root         (0) root         (0)      673 2022-09-02 11:29:48.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-docs-sdk-reference-soil-configuration-md-707.json
--rw-rw-rw-   0 root         (0) root         (0)      760 2022-09-02 11:29:48.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-docs-sdk-reference-soil-connectors-elastic-search-md-eca.json
--rw-rw-rw-   0 root         (0) root         (0)      586 2022-09-02 11:29:48.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-docs-sdk-reference-soil-data-md-d6b.json
--rw-rw-rw-   0 root         (0) root         (0)      686 2022-09-02 11:29:48.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-docs-sdk-reference-soil-data-structure-md-e8d.json
--rw-rw-rw-   0 root         (0) root         (0)      632 2022-09-02 11:29:48.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-docs-sdk-reference-soil-finder-md-60a.json
--rw-rw-rw-   0 root         (0) root         (0)      643 2022-09-02 11:29:48.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-docs-sdk-reference-soil-modulify-md-0c9.json
--rw-rw-rw-   0 root         (0) root         (0)      630 2022-09-02 11:29:48.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-docs-sdk-reference-soil-pipeline-md-312.json
--rw-rw-rw-   0 root         (0) root         (0)      601 2022-09-02 11:29:48.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-docs-sdk-reference-soil-types-md-24f.json
--rw-rw-rw-   0 root         (0) root         (0)      578 2022-09-02 11:29:48.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-sdk-reference-sdk-reference-md-a6b.json
--rw-rw-rw-   0 root         (0) root         (0)     1035 2023-02-17 10:34:02.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-sdk-reference-soil-alerts-alerts-md-231.json
--rw-rw-rw-   0 root         (0) root         (0)      963 2023-02-17 10:34:02.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-sdk-reference-soil-alias-md-2bb.json
--rw-rw-rw-   0 root         (0) root         (0)      936 2023-02-17 10:34:02.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-sdk-reference-soil-api-md-cf6.json
--rw-rw-rw-   0 root         (0) root         (0)      654 2022-09-02 11:29:48.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-sdk-reference-soil-cli-soil-cli-md-c6c.json
--rw-rw-rw-   0 root         (0) root         (0)      983 2023-02-17 10:34:02.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-sdk-reference-soil-configuration-md-b6d.json
--rw-rw-rw-   0 root         (0) root         (0)      896 2023-02-17 10:34:02.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-sdk-reference-soil-connectors-elastic-search-md-8f4.json
--rw-rw-rw-   0 root         (0) root         (0)      927 2023-02-17 10:34:02.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-sdk-reference-soil-data-md-d6c.json
--rw-rw-rw-   0 root         (0) root         (0)     1009 2023-02-17 10:34:02.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-sdk-reference-soil-data-structure-md-3d5.json
--rw-rw-rw-   0 root         (0) root         (0)      970 2023-02-17 10:34:02.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-sdk-reference-soil-decorator-md-6e4.json
--rw-rw-rw-   0 root         (0) root         (0)      989 2023-02-17 10:34:02.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-sdk-reference-soil-dictionary-md-7b7.json
--rw-rw-rw-   0 root         (0) root         (0)      927 2023-02-17 10:34:02.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-sdk-reference-soil-errors-md-4c9.json
--rw-rw-rw-   0 root         (0) root         (0)      949 2023-02-17 10:34:02.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-sdk-reference-soil-finder-md-839.json
--rw-rw-rw-   0 root         (0) root         (0)      962 2023-02-17 10:34:02.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-sdk-reference-soil-modulify-md-37b.json
--rw-rw-rw-   0 root         (0) root         (0)      945 2023-02-17 10:34:02.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-sdk-reference-soil-pipeline-md-5a1.json
--rw-rw-rw-   0 root         (0) root         (0)     1073 2023-02-17 10:34:02.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-sdk-reference-soil-storage-base-storage-md-4fa.json
--rw-rw-rw-   0 root         (0) root         (0)     1131 2023-02-17 10:34:02.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-sdk-reference-soil-storage-compound-storage-md-96f.json
--rw-rw-rw-   0 root         (0) root         (0)     1115 2023-02-17 10:34:02.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-sdk-reference-soil-storage-elasticsearch-md-f3d.json
--rw-rw-rw-   0 root         (0) root         (0)     1085 2023-02-17 10:34:02.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-sdk-reference-soil-storage-object-storage-md-ce3.json
--rw-rw-rw-   0 root         (0) root         (0)      901 2023-02-17 10:34:02.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-sdk-reference-soil-task-md-a67.json
--rw-rw-rw-   0 root         (0) root         (0)      907 2023-02-17 10:34:02.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-sdk-reference-soil-types-md-3ef.json
--rw-rw-rw-   0 root         (0) root         (0)      835 2023-02-17 10:34:02.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-sdk-reference-soil-utils-md-092.json
--rw-rw-rw-   0 root         (0) root         (0)     1140 2023-02-17 10:34:02.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-data-structures-data-structure-md-1fb.json
--rw-rw-rw-   0 root         (0) root         (0)     1155 2023-02-17 10:34:02.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-data-structures-frequent-itemsets-md-3bb.json
--rw-rw-rw-   0 root         (0) root         (0)     1092 2023-02-17 10:34:02.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-data-structures-hypergraph-md-c0e.json
--rw-rw-rw-   0 root         (0) root         (0)      903 2022-09-02 11:29:48.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-data-structures-init-md-de6.json
--rw-rw-rw-   0 root         (0) root         (0)      903 2022-09-02 11:29:48.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-data-structures-model-md-0ad.json
--rw-rw-rw-   0 root         (0) root         (0)     1076 2022-09-02 11:29:48.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-data-structures-nb-clusters-categorical-md-046.json
--rw-rw-rw-   0 root         (0) root         (0)     1091 2023-02-17 10:34:02.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-data-structures-nb-clusters-md-7ed.json
--rw-rw-rw-   0 root         (0) root         (0)      977 2022-09-02 11:29:48.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-data-structures-paginated-list-md-973.json
--rw-rw-rw-   0 root         (0) root         (0)     1139 2023-02-17 10:34:02.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-data-structures-predefined-dict-md-379.json
--rw-rw-rw-   0 root         (0) root         (0)      995 2022-09-02 11:29:48.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-data-structures-predefined-init-md-575.json
--rw-rw-rw-   0 root         (0) root         (0)     1126 2023-02-17 10:34:02.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-data-structures-predefined-list-md-5ee.json
--rw-rw-rw-   0 root         (0) root         (0)     1145 2023-02-17 10:34:02.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-data-structures-predefined-ndarray-md-7db.json
--rw-rw-rw-   0 root         (0) root         (0)     1191 2023-02-17 10:34:02.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-data-structures-predefined-object-ds-md-f15.json
--rw-rw-rw-   0 root         (0) root         (0)     1213 2023-02-17 10:34:02.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-data-structures-predefined-pd-data-frame-md-a71.json
--rw-rw-rw-   0 root         (0) root         (0)      935 2022-09-02 11:29:48.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-data-structures-statistics-md-07b.json
--rw-rw-rw-   0 root         (0) root         (0)     1082 2022-09-02 11:29:48.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-data-structures-streams-association-rules-md-820.json
--rw-rw-rw-   0 root         (0) root         (0)      957 2022-09-02 11:29:48.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-data-structures-streams-init-md-d9b.json
--rw-rw-rw-   0 root         (0) root         (0)     1129 2023-02-17 10:34:02.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-data-structures-streams-patients-md-60e.json
--rw-rw-rw-   0 root         (0) root         (0)     1097 2023-02-17 10:34:02.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-data-structures-streams-stream-md-317.json
--rw-rw-rw-   0 root         (0) root         (0)      996 2023-02-17 10:34:02.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-data-structures-streams-trajectory-clusters-md-1d9.json
--rw-rw-rw-   0 root         (0) root         (0)     1005 2022-09-02 11:29:48.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-data-structures-time-statistics-md-fcd.json
--rw-rw-rw-   0 root         (0) root         (0)      957 2022-09-02 11:29:48.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-data-structures-trajectories-md-899.json
--rw-rw-rw-   0 root         (0) root         (0)     1027 2022-09-02 11:29:48.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-ehra-data-structures-hypergraph-md-084.json
--rw-rw-rw-   0 root         (0) root         (0)     1071 2022-09-02 11:29:48.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-ehra-data-structures-streams-patients-md-ced.json
--rw-rw-rw-   0 root         (0) root         (0)     1102 2022-09-02 11:29:48.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-ehra-data-structures-streams-trajectory-clusters-md-7cf.json
--rw-rw-rw-   0 root         (0) root         (0)     1170 2022-09-02 11:29:48.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-ehra-modules-clustering-nb-clustering-categorical-md-300.json
--rw-rw-rw-   0 root         (0) root         (0)     1056 2022-09-02 11:29:48.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-ehra-modules-clustering-nb-clustering-md-11b.json
--rw-rw-rw-   0 root         (0) root         (0)     1108 2022-09-02 11:29:48.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-ehra-modules-clustering-sidiwo-sidiwo-md-266.json
--rw-rw-rw-   0 root         (0) root         (0)      901 2022-09-02 11:29:48.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-ehra-modules-experiment-md-047.json
--rw-rw-rw-   0 root         (0) root         (0)     1081 2022-09-02 11:29:48.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-ehra-modules-higher-order-predictor-md-414.json
--rw-rw-rw-   0 root         (0) root         (0)     1183 2022-09-02 11:29:48.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-ehra-modules-itemsets-frequent-itemsets-compare-md-6e5.json
--rw-rw-rw-   0 root         (0) root         (0)     1206 2022-09-02 11:29:48.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-ehra-modules-itemsets-frequent-itemsets-hypergraph-md-d85.json
--rw-rw-rw-   0 root         (0) root         (0)     1157 2022-09-02 11:29:48.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-ehra-modules-preprocessing-filters-events-filter-md-2cf.json
--rw-rw-rw-   0 root         (0) root         (0)     1142 2022-09-02 11:29:48.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-ehra-modules-preprocessing-filters-row-filter-md-b96.json
--rw-rw-rw-   0 root         (0) root         (0)     1096 2022-09-02 11:29:48.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-ehra-modules-statistics-customstatistics-md-353.json
--rw-rw-rw-   0 root         (0) root         (0)     1082 2022-09-02 11:29:48.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-ehra-modules-statistics-time-statistics-md-7fa.json
--rw-rw-rw-   0 root         (0) root         (0)     1090 2022-09-02 11:29:48.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-ehra-modules-temporal-trajectories-md-419.json
--rw-rw-rw-   0 root         (0) root         (0)      897 2022-09-02 11:29:48.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-modules-clustering-init-md-349.json
--rw-rw-rw-   0 root         (0) root         (0)     1250 2023-02-17 10:34:02.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-modules-clustering-nb-clustering-categorical-md-0c4.json
--rw-rw-rw-   0 root         (0) root         (0)     1148 2023-02-17 10:34:02.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-modules-clustering-nb-clustering-md-19d.json
--rw-rw-rw-   0 root         (0) root         (0)      994 2022-09-02 11:29:48.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-modules-clustering-sidiwo-init-md-729.json
--rw-rw-rw-   0 root         (0) root         (0)     1174 2023-02-17 10:34:02.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-modules-clustering-sidiwo-sidiwo-md-478.json
--rw-rw-rw-   0 root         (0) root         (0)      995 2023-02-17 10:34:02.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-modules-experiment-md-a5e.json
--rw-rw-rw-   0 root         (0) root         (0)      943 2022-09-02 11:29:48.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-modules-higher-order-init-md-c2b.json
--rw-rw-rw-   0 root         (0) root         (0)     1165 2023-02-17 10:34:02.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-modules-higher-order-predictor-md-b65.json
--rw-rw-rw-   0 root         (0) root         (0)      765 2022-09-02 11:29:48.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-modules-init-md-f13.json
--rw-rw-rw-   0 root         (0) root         (0)     1083 2022-09-02 11:29:48.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-modules-itemsets-association-rules-md-8b6.json
--rw-rw-rw-   0 root         (0) root         (0)     1292 2023-02-17 10:34:02.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-modules-itemsets-frequent-itemsets-compare-md-49b.json
--rw-rw-rw-   0 root         (0) root         (0)     1299 2023-02-17 10:34:02.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-modules-itemsets-frequent-itemsets-hypergraph-md-0d1.json
--rw-rw-rw-   0 root         (0) root         (0)     1048 2022-09-02 11:29:48.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-modules-itemsets-frequent-itemsets-md-ca7.json
--rw-rw-rw-   0 root         (0) root         (0)      925 2022-09-02 11:29:48.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-modules-itemsets-init-md-a1a.json
--rw-rw-rw-   0 root         (0) root         (0)     1131 2022-09-02 11:29:48.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-modules-preprocessing-filters-column-filter-md-04c.json
--rw-rw-rw-   0 root         (0) root         (0)     1278 2023-02-17 10:34:02.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-modules-preprocessing-filters-events-filter-md-59c.json
--rw-rw-rw-   0 root         (0) root         (0)     1101 2022-09-02 11:29:48.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-modules-preprocessing-filters-flattener-md-1a6.json
--rw-rw-rw-   0 root         (0) root         (0)     1005 2022-09-02 11:29:48.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-modules-preprocessing-filters-init-md-728.json
--rw-rw-rw-   0 root         (0) root         (0)     1219 2023-02-17 10:34:02.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-modules-preprocessing-filters-row-filter-md-77e.json
--rw-rw-rw-   0 root         (0) root         (0)      939 2022-09-02 11:29:48.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-modules-preprocessing-init-md-8d4.json
--rw-rw-rw-   0 root         (0) root         (0)      946 2022-09-02 11:29:48.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-modules-preprocessing-pipe-md-fd6.json
--rw-rw-rw-   0 root         (0) root         (0)     1065 2022-09-02 11:29:48.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-modules-preprocessing-sampling-init-md-dba.json
--rw-rw-rw-   0 root         (0) root         (0)     1126 2022-09-02 11:29:48.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-modules-preprocessing-sampling-reservoir-sampling-md-cfe.json
--rw-rw-rw-   0 root         (0) root         (0)     1179 2023-02-17 10:34:02.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-modules-statistics-customstatistics-md-3e3.json
--rw-rw-rw-   0 root         (0) root         (0)      917 2022-09-02 11:29:48.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-modules-statistics-init-md-135.json
--rw-rw-rw-   0 root         (0) root         (0)      970 2022-09-02 11:29:48.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-modules-statistics-statistics-md-0db.json
--rw-rw-rw-   0 root         (0) root         (0)     1169 2023-02-17 10:34:02.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-modules-statistics-time-statistics-md-92c.json
--rw-rw-rw-   0 root         (0) root         (0)      939 2022-09-02 11:29:48.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-modules-temporal-init-md-37a.json
--rw-rw-rw-   0 root         (0) root         (0)      864 2023-02-17 10:34:02.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-modules-temporal-trajectories-md-285.json
--rw-rw-rw-   0 root         (0) root         (0)      559 2022-09-02 11:29:48.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-soil-library-md-65d.json
--rw-rw-rw-   0 root         (0) root         (0)     1135 2023-02-17 10:34:02.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-tutorial-alerts-md-43b.json
--rw-rw-rw-   0 root         (0) root         (0)      832 2023-02-17 10:34:02.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-tutorial-data-md-0d2.json
--rw-rw-rw-   0 root         (0) root         (0)     1202 2023-02-17 10:34:02.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-tutorial-data-structures-md-14d.json
--rw-rw-rw-   0 root         (0) root         (0)     1160 2023-02-17 10:34:02.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-tutorial-deployments-md-62e.json
--rw-rw-rw-   0 root         (0) root         (0)      609 2022-09-02 11:29:48.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-tutorial-get-started-md-d5b.json
--rw-rw-rw-   0 root         (0) root         (0)      798 2023-02-17 10:34:02.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-tutorial-get-started-mdx-36a.json
--rw-rw-rw-   0 root         (0) root         (0)      844 2023-02-17 10:34:02.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-tutorial-logging-md-507.json
--rw-rw-rw-   0 root         (0) root         (0)      942 2023-02-17 10:34:02.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-tutorial-modules-md-cd8.json
--rw-rw-rw-   0 root         (0) root         (0)      944 2023-02-17 10:34:02.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-tutorial-notebooks-md-58b.json
--rw-rw-rw-   0 root         (0) root         (0)     1027 2023-02-17 10:34:02.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-tutorial-scripts-md-0f5.json
--rw-rw-rw-   0 root         (0) root         (0)      478 2022-09-02 11:29:48.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-tutorial-subtasks-md-e0d.json
--rw-rw-rw-   0 root         (0) root         (0)      775 2022-09-02 11:29:48.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-1-sdk-reference-sdk-reference-md-59f.json
--rw-rw-rw-   0 root         (0) root         (0)      853 2022-09-02 11:29:48.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-1-soil-library-soil-library-md-ce1.json
--rw-rw-rw-   0 root         (0) root         (0)      776 2022-09-02 11:29:48.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-1-tutorial-data-md-e4a.json
--rw-rw-rw-   0 root         (0) root         (0)      830 2022-09-02 11:29:48.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-1-tutorial-data-structures-md-53e.json
--rw-rw-rw-   0 root         (0) root         (0)      679 2022-09-02 11:29:48.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-1-tutorial-get-started-md-cbe.json
--rw-rw-rw-   0 root         (0) root         (0)      567 2022-09-02 11:29:48.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-1-tutorial-logging-md-4a1.json
--rw-rw-rw-   0 root         (0) root         (0)      894 2022-09-02 11:29:48.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-1-tutorial-modules-md-547.json
--rw-rw-rw-   0 root         (0) root         (0)      945 2022-09-02 11:29:48.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-1-tutorial-scripts-md-a17.json
--rw-rw-rw-   0 root         (0) root         (0)      775 2022-09-02 11:29:48.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-2-sdk-reference-sdk-reference-md-62b.json
--rw-rw-rw-   0 root         (0) root         (0)      853 2022-09-02 11:29:48.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-2-soil-library-soil-library-md-1c7.json
--rw-rw-rw-   0 root         (0) root         (0)      776 2022-09-02 11:29:48.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-2-tutorial-data-md-278.json
--rw-rw-rw-   0 root         (0) root         (0)     1124 2022-09-02 11:29:48.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-2-tutorial-data-structures-md-89f.json
--rw-rw-rw-   0 root         (0) root         (0)      679 2022-09-02 11:29:48.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-2-tutorial-get-started-md-022.json
--rw-rw-rw-   0 root         (0) root         (0)      567 2022-09-02 11:29:48.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-2-tutorial-logging-md-4c2.json
--rw-rw-rw-   0 root         (0) root         (0)      894 2022-09-02 11:29:48.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-2-tutorial-modules-md-cdc.json
--rw-rw-rw-   0 root         (0) root         (0)      945 2022-09-02 11:29:48.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-2-tutorial-scripts-md-d50.json
--rw-rw-rw-   0 root         (0) root         (0)      775 2022-09-02 11:29:48.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-3-sdk-reference-sdk-reference-md-75e.json
--rw-rw-rw-   0 root         (0) root         (0)      853 2022-09-02 11:29:48.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-3-soil-library-soil-library-md-aaf.json
--rw-rw-rw-   0 root         (0) root         (0)      776 2022-09-02 11:29:48.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-3-tutorial-data-md-bc1.json
--rw-rw-rw-   0 root         (0) root         (0)     1124 2022-09-02 11:29:48.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-3-tutorial-data-structures-md-805.json
--rw-rw-rw-   0 root         (0) root         (0)      679 2022-09-02 11:29:48.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-3-tutorial-get-started-md-9c5.json
--rw-rw-rw-   0 root         (0) root         (0)      798 2022-09-02 11:29:48.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-3-tutorial-logging-md-0a4.json
--rw-rw-rw-   0 root         (0) root         (0)      880 2022-09-02 11:29:48.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-3-tutorial-modules-md-c8e.json
--rw-rw-rw-   0 root         (0) root         (0)      945 2022-09-02 11:29:48.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-3-tutorial-scripts-md-dbf.json
--rw-rw-rw-   0 root         (0) root         (0)      775 2022-09-02 11:29:48.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-4-sdk-reference-sdk-reference-md-343.json
--rw-rw-rw-   0 root         (0) root         (0)      853 2022-09-02 11:29:48.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-4-soil-library-soil-library-md-b38.json
--rw-rw-rw-   0 root         (0) root         (0)      776 2022-09-02 11:29:48.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-4-tutorial-data-md-8d7.json
--rw-rw-rw-   0 root         (0) root         (0)     1124 2022-09-02 11:29:48.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-4-tutorial-data-structures-md-b95.json
--rw-rw-rw-   0 root         (0) root         (0)      679 2022-09-02 11:29:48.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-4-tutorial-get-started-md-c2c.json
--rw-rw-rw-   0 root         (0) root         (0)      798 2022-09-02 11:29:48.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-4-tutorial-logging-md-750.json
--rw-rw-rw-   0 root         (0) root         (0)      880 2022-09-02 11:29:48.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-4-tutorial-modules-md-447.json
--rw-rw-rw-   0 root         (0) root         (0)      945 2022-09-02 11:29:48.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-4-tutorial-scripts-md-904.json
--rw-rw-rw-   0 root         (0) root         (0)      775 2022-09-02 11:29:48.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-5-sdk-reference-sdk-reference-md-c6e.json
--rw-rw-rw-   0 root         (0) root         (0)      853 2022-09-02 11:29:48.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-5-soil-library-soil-library-md-f09.json
--rw-rw-rw-   0 root         (0) root         (0)      776 2022-09-02 11:29:48.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-5-tutorial-data-md-ae6.json
--rw-rw-rw-   0 root         (0) root         (0)     1124 2022-09-02 11:29:48.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-5-tutorial-data-structures-md-d2f.json
--rw-rw-rw-   0 root         (0) root         (0)      679 2022-09-02 11:29:48.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-5-tutorial-get-started-md-392.json
--rw-rw-rw-   0 root         (0) root         (0)      798 2022-09-02 11:29:48.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-5-tutorial-logging-md-645.json
--rw-rw-rw-   0 root         (0) root         (0)      880 2022-09-02 11:29:48.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-5-tutorial-modules-md-3bc.json
--rw-rw-rw-   0 root         (0) root         (0)      945 2022-09-02 11:29:48.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-5-tutorial-scripts-md-bd1.json
--rw-rw-rw-   0 root         (0) root         (0)      775 2022-09-02 11:29:48.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-6-sdk-reference-sdk-reference-md-073.json
--rw-rw-rw-   0 root         (0) root         (0)      853 2022-09-02 11:29:48.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-6-soil-library-soil-library-md-53e.json
--rw-rw-rw-   0 root         (0) root         (0)      776 2022-09-02 11:29:48.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-6-tutorial-data-md-cba.json
--rw-rw-rw-   0 root         (0) root         (0)     1124 2022-09-02 11:29:48.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-6-tutorial-data-structures-md-c96.json
--rw-rw-rw-   0 root         (0) root         (0)      679 2022-09-02 11:29:48.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-6-tutorial-get-started-md-6a0.json
--rw-rw-rw-   0 root         (0) root         (0)      798 2022-09-02 11:29:48.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-6-tutorial-logging-md-7c2.json
--rw-rw-rw-   0 root         (0) root         (0)      880 2022-09-02 11:29:48.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-6-tutorial-modules-md-dd3.json
--rw-rw-rw-   0 root         (0) root         (0)      945 2022-09-02 11:29:48.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-6-tutorial-scripts-md-e55.json
--rw-rw-rw-   0 root         (0) root         (0)      775 2022-09-02 11:29:48.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-7-sdk-reference-sdk-reference-md-5bd.json
--rw-rw-rw-   0 root         (0) root         (0)      853 2022-09-02 11:29:48.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-7-soil-library-soil-library-md-b02.json
--rw-rw-rw-   0 root         (0) root         (0)      776 2022-09-02 11:29:48.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-7-tutorial-data-md-345.json
--rw-rw-rw-   0 root         (0) root         (0)     1124 2022-09-02 11:29:48.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-7-tutorial-data-structures-md-b1a.json
--rw-rw-rw-   0 root         (0) root         (0)      679 2022-09-02 11:29:48.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-7-tutorial-get-started-md-661.json
--rw-rw-rw-   0 root         (0) root         (0)      798 2022-09-02 11:29:48.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-7-tutorial-logging-md-aae.json
--rw-rw-rw-   0 root         (0) root         (0)      880 2022-09-02 11:29:48.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-7-tutorial-modules-md-9f2.json
--rw-rw-rw-   0 root         (0) root         (0)      945 2022-09-02 11:29:48.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-7-tutorial-scripts-md-21c.json
--rw-rw-rw-   0 root         (0) root         (0)      775 2022-09-02 11:29:48.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-8-sdk-reference-sdk-reference-md-670.json
--rw-rw-rw-   0 root         (0) root         (0)      853 2022-09-02 11:29:48.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-8-soil-library-soil-library-md-3b4.json
--rw-rw-rw-   0 root         (0) root         (0)      776 2022-09-02 11:29:48.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-8-tutorial-data-md-e4f.json
--rw-rw-rw-   0 root         (0) root         (0)     1124 2022-09-02 11:29:48.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-8-tutorial-data-structures-md-04f.json
--rw-rw-rw-   0 root         (0) root         (0)      679 2022-09-02 11:29:48.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-8-tutorial-get-started-md-610.json
--rw-rw-rw-   0 root         (0) root         (0)      798 2022-09-02 11:29:48.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-8-tutorial-logging-md-0d8.json
--rw-rw-rw-   0 root         (0) root         (0)      880 2022-09-02 11:29:48.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-8-tutorial-modules-md-a2c.json
--rw-rw-rw-   0 root         (0) root         (0)      945 2022-09-02 11:29:48.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-8-tutorial-scripts-md-700.json
--rw-rw-rw-   0 root         (0) root         (0)      633 2022-09-02 11:29:48.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-1-0-sdk-reference-sdk-reference-md-172.json
--rw-rw-rw-   0 root         (0) root         (0)      619 2022-09-02 11:29:48.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-1-0-soil-library-soil-library-md-963.json
--rw-rw-rw-   0 root         (0) root         (0)      543 2022-09-02 11:29:48.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-1-0-tutorial-data-md-eac.json
--rw-rw-rw-   0 root         (0) root         (0)      913 2022-09-02 11:29:48.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-1-0-tutorial-data-structures-md-f2b.json
--rw-rw-rw-   0 root         (0) root         (0)      667 2022-09-02 11:29:48.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-1-0-tutorial-get-started-md-526.json
--rw-rw-rw-   0 root         (0) root         (0)      598 2022-09-02 11:29:48.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-1-0-tutorial-get-started-mdx-539.json
--rw-rw-rw-   0 root         (0) root         (0)      567 2022-09-02 11:29:48.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-1-0-tutorial-logging-md-3a5.json
--rw-rw-rw-   0 root         (0) root         (0)      647 2022-09-02 11:29:48.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-1-0-tutorial-modules-md-1ad.json
--rw-rw-rw-   0 root         (0) root         (0)      746 2022-09-02 11:29:48.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-1-0-tutorial-scripts-md-caa.json
--rw-rw-rw-   0 root         (0) root         (0)      652 2022-09-02 11:29:48.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-1-1-sdk-reference-soil-alias-md-6d0.json
--rw-rw-rw-   0 root         (0) root         (0)      633 2022-09-02 11:29:48.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-1-1-sdk-reference-soil-api-md-056.json
--rw-rw-rw-   0 root         (0) root         (0)      692 2022-09-02 11:29:48.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-1-1-sdk-reference-soil-configuration-md-7c5.json
--rw-rw-rw-   0 root         (0) root         (0)      779 2022-09-02 11:29:48.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-1-1-sdk-reference-soil-connectors-elastic-search-md-b85.json
--rw-rw-rw-   0 root         (0) root         (0)      605 2022-09-02 11:29:48.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-1-1-sdk-reference-soil-data-md-797.json
--rw-rw-rw-   0 root         (0) root         (0)      705 2022-09-02 11:29:48.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-1-1-sdk-reference-soil-data-structure-md-916.json
--rw-rw-rw-   0 root         (0) root         (0)      651 2022-09-02 11:29:48.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-1-1-sdk-reference-soil-finder-md-c72.json
--rw-rw-rw-   0 root         (0) root         (0)      662 2022-09-02 11:29:48.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-1-1-sdk-reference-soil-modulify-md-b9a.json
--rw-rw-rw-   0 root         (0) root         (0)      649 2022-09-02 11:29:48.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-1-1-sdk-reference-soil-pipeline-md-6eb.json
--rw-rw-rw-   0 root         (0) root         (0)      620 2022-09-02 11:29:48.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-1-1-sdk-reference-soil-types-md-00c.json
--rw-rw-rw-   0 root         (0) root         (0)      613 2022-09-02 11:29:48.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-1-1-soil-library-soil-library-md-2b7.json
--rw-rw-rw-   0 root         (0) root         (0)      537 2022-09-02 11:29:48.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-1-1-tutorial-data-md-b95.json
--rw-rw-rw-   0 root         (0) root         (0)      907 2022-09-02 11:29:48.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-1-1-tutorial-data-structures-md-03c.json
--rw-rw-rw-   0 root         (0) root         (0)      592 2022-09-02 11:29:48.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-1-1-tutorial-get-started-mdx-cf0.json
--rw-rw-rw-   0 root         (0) root         (0)      561 2022-09-02 11:29:48.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-1-1-tutorial-logging-md-bb1.json
--rw-rw-rw-   0 root         (0) root         (0)      641 2022-09-02 11:29:48.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-1-1-tutorial-modules-md-4b3.json
--rw-rw-rw-   0 root         (0) root         (0)      740 2022-09-02 11:29:48.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-1-1-tutorial-scripts-md-7f6.json
--rw-rw-rw-   0 root         (0) root         (0)      652 2022-09-02 11:29:48.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-1-2-sdk-reference-soil-alias-md-165.json
--rw-rw-rw-   0 root         (0) root         (0)      633 2022-09-02 11:29:48.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-1-2-sdk-reference-soil-api-md-f09.json
--rw-rw-rw-   0 root         (0) root         (0)      692 2022-09-02 11:29:48.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-1-2-sdk-reference-soil-configuration-md-4f6.json
--rw-rw-rw-   0 root         (0) root         (0)      779 2022-09-02 11:29:48.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-1-2-sdk-reference-soil-connectors-elastic-search-md-224.json
--rw-rw-rw-   0 root         (0) root         (0)      605 2022-09-02 11:29:48.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-1-2-sdk-reference-soil-data-md-cd7.json
--rw-rw-rw-   0 root         (0) root         (0)      705 2022-09-02 11:29:48.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-1-2-sdk-reference-soil-data-structure-md-849.json
--rw-rw-rw-   0 root         (0) root         (0)      651 2022-09-02 11:29:48.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-1-2-sdk-reference-soil-finder-md-da9.json
--rw-rw-rw-   0 root         (0) root         (0)      662 2022-09-02 11:29:48.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-1-2-sdk-reference-soil-modulify-md-47e.json
--rw-rw-rw-   0 root         (0) root         (0)      649 2022-09-02 11:29:48.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-1-2-sdk-reference-soil-pipeline-md-945.json
--rw-rw-rw-   0 root         (0) root         (0)      620 2022-09-02 11:29:48.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-1-2-sdk-reference-soil-types-md-b0e.json
--rw-rw-rw-   0 root         (0) root         (0)      613 2022-09-02 11:29:48.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-1-2-soil-library-soil-library-md-04e.json
--rw-rw-rw-   0 root         (0) root         (0)      537 2022-09-02 11:29:48.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-1-2-tutorial-data-md-0e1.json
--rw-rw-rw-   0 root         (0) root         (0)      907 2022-09-02 11:29:49.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-1-2-tutorial-data-structures-md-ad9.json
--rw-rw-rw-   0 root         (0) root         (0)      592 2022-09-02 11:29:49.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-1-2-tutorial-get-started-mdx-7f5.json
--rw-rw-rw-   0 root         (0) root         (0)      561 2022-09-02 11:29:49.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-1-2-tutorial-logging-md-cb9.json
--rw-rw-rw-   0 root         (0) root         (0)      641 2022-09-02 11:29:49.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-1-2-tutorial-modules-md-ad2.json
--rw-rw-rw-   0 root         (0) root         (0)      740 2022-09-02 11:29:49.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-1-2-tutorial-scripts-md-aef.json
--rw-rw-rw-   0 root         (0) root         (0)     1968 2022-09-02 11:29:49.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/version-0-0-1-metadata-prop-e31.json
--rw-rw-rw-   0 root         (0) root         (0)     1968 2022-09-02 11:29:49.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/version-0-0-2-metadata-prop-b4f.json
--rw-rw-rw-   0 root         (0) root         (0)     2162 2022-09-02 11:29:49.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/version-0-0-3-metadata-prop-272.json
--rw-rw-rw-   0 root         (0) root         (0)     2162 2022-09-02 11:29:49.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/version-0-0-4-metadata-prop-937.json
--rw-rw-rw-   0 root         (0) root         (0)     2162 2022-09-02 11:29:49.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/version-0-0-5-metadata-prop-e97.json
--rw-rw-rw-   0 root         (0) root         (0)     2162 2022-09-02 11:29:49.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/version-0-0-6-metadata-prop-46a.json
--rw-rw-rw-   0 root         (0) root         (0)     2162 2022-09-02 11:29:49.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/version-0-0-7-metadata-prop-558.json
--rw-rw-rw-   0 root         (0) root         (0)     2162 2022-09-02 11:29:49.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/version-0-0-8-metadata-prop-5dc.json
--rw-rw-rw-   0 root         (0) root         (0)      138 2022-09-02 11:29:49.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/version-0-1-0-metadata-prop-69a.json
--rw-rw-rw-   0 root         (0) root         (0)      137 2022-09-02 11:29:49.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/version-0-1-1-metadata-prop-aee.json
--rw-rw-rw-   0 root         (0) root         (0)      137 2022-09-02 11:29:49.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/version-0-1-2-metadata-prop-be9.json
--rw-rw-rw-   0 root         (0) root         (0)    29936 2023-02-17 10:34:02.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/version-current-metadata-prop-751.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-10 09:30:31.631070 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-pages/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-10 09:30:31.663071 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-pages/default/
--rw-rw-rw-   0 root         (0) root         (0)       66 2023-02-17 10:34:02.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-pages/default/plugin-route-context-module-100.json
--rw-rw-rw-   0 root         (0) root         (0)       80 2022-09-02 11:29:49.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-pages/default/site-src-pages-index-mdx-e7c.json
--rw-rw-rw-   0 root         (0) root         (0)       83 2022-09-02 11:29:49.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-pages/default/site-src-pages-test-mdx-362.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-10 09:30:31.631070 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-debug/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-10 09:30:31.663071 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-debug/default/
--rw-rw-rw-   0 root         (0) root         (0)   104640 2022-09-02 11:29:49.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-debug/default/docusaurus-debug-all-content-673.json
--rw-rw-rw-   0 root         (0) root         (0)       58 2022-09-02 11:29:49.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-debug/default/plugin-route-context-module-100.json
--rw-rw-rw-   0 root         (0) root         (0)     2663 2022-09-02 11:29:49.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus.config.js
--rw-rw-rw-   0 root         (0) root         (0)     5946 2023-02-17 10:34:02.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus.config.mjs
--rw-rw-rw-   0 root         (0) root         (0)    10462 2023-02-17 10:34:02.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/globalData.json
--rw-rw-rw-   0 root         (0) root         (0)      229 2023-02-17 10:34:02.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/i18n.json
--rw-rw-rw-   0 root         (0) root         (0)    28392 2023-02-17 10:34:02.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/registry.js
--rw-rw-rw-   0 root         (0) root         (0)    13307 2023-02-17 10:34:02.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/routes.js
--rw-rw-rw-   0 root         (0) root         (0)    13579 2023-02-17 10:34:02.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/routesChunkNames.json
--rw-rw-rw-   0 root         (0) root         (0)      840 2023-02-17 10:34:02.000000 soil-sdk-0.6.8.dev2/docs/website/.docusaurus/site-metadata.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-10 09:30:31.663071 soil-sdk-0.6.8.dev2/docs/website/blog/
--rw-rw-rw-   0 root         (0) root         (0)     3295 2022-09-02 11:29:49.000000 soil-sdk-0.6.8.dev2/docs/website/blog/2016-03-11-blog-post.md
--rw-rw-rw-   0 root         (0) root         (0)     3298 2022-09-02 11:29:49.000000 soil-sdk-0.6.8.dev2/docs/website/blog/2017-04-10-blog-post-two.md
--rw-rw-rw-   0 root         (0) root         (0)      480 2022-09-02 11:29:49.000000 soil-sdk-0.6.8.dev2/docs/website/blog/2017-09-25-testing-rss.md
--rw-rw-rw-   0 root         (0) root         (0)      182 2022-09-02 11:29:49.000000 soil-sdk-0.6.8.dev2/docs/website/blog/2017-09-26-adding-rss.md
--rw-rw-rw-   0 root         (0) root         (0)      199 2022-09-02 11:29:49.000000 soil-sdk-0.6.8.dev2/docs/website/blog/2017-10-24-new-version-1.0.0.md
--rw-rw-rw-   0 root         (0) root         (0)     1949 2022-09-02 11:29:49.000000 soil-sdk-0.6.8.dev2/docs/website/docusaurus.config.js
--rw-rw-rw-   0 root         (0) root         (0)      531 2023-02-06 08:17:43.000000 soil-sdk-0.6.8.dev2/docs/website/package.json
--rw-rw-rw-   0 root         (0) root         (0)      447 2022-09-02 11:29:49.000000 soil-sdk-0.6.8.dev2/docs/website/sidebars.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-10 09:30:31.631070 soil-sdk-0.6.8.dev2/docs/website/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-10 09:30:31.663071 soil-sdk-0.6.8.dev2/docs/website/src/css/
--rw-rw-rw-   0 root         (0) root         (0)      276 2022-09-02 11:29:49.000000 soil-sdk-0.6.8.dev2/docs/website/src/css/customTheme.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-10 09:30:31.663071 soil-sdk-0.6.8.dev2/docs/website/src/pages/
--rw-rw-rw-   0 root         (0) root         (0)     4747 2022-09-02 11:29:49.000000 soil-sdk-0.6.8.dev2/docs/website/src/pages/index.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-10 09:30:31.631070 soil-sdk-0.6.8.dev2/docs/website/static/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-10 09:30:31.663071 soil-sdk-0.6.8.dev2/docs/website/static/css/
--rw-rw-rw-   0 root         (0) root         (0)      482 2022-09-02 11:29:49.000000 soil-sdk-0.6.8.dev2/docs/website/static/css/custom.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-10 09:30:31.667071 soil-sdk-0.6.8.dev2/docs/website/static/img/
--rw-rw-rw-   0 root         (0) root         (0)      766 2022-09-02 11:29:49.000000 soil-sdk-0.6.8.dev2/docs/website/static/img/favicon.ico
--rw-rw-rw-   0 root         (0) root         (0)    15538 2022-09-02 11:29:49.000000 soil-sdk-0.6.8.dev2/docs/website/static/img/favicon_amalfi.png
--rw-rw-rw-   0 root         (0) root         (0)     4370 2022-09-02 11:29:49.000000 soil-sdk-0.6.8.dev2/docs/website/static/img/oss_logo.png
--rw-rw-rw-   0 root         (0) root         (0)     4388 2022-09-02 11:29:49.000000 soil-sdk-0.6.8.dev2/docs/website/static/img/undraw_abstract_x68e.svg
--rw-rw-rw-   0 root         (0) root         (0)    17343 2022-09-02 11:29:49.000000 soil-sdk-0.6.8.dev2/docs/website/static/img/undraw_code_review.svg
--rw-rw-rw-   0 root         (0) root         (0)    22330 2022-09-02 11:29:49.000000 soil-sdk-0.6.8.dev2/docs/website/static/img/undraw_mind_map_cwng.svg
--rw-rw-rw-   0 root         (0) root         (0)    32999 2022-09-02 11:29:49.000000 soil-sdk-0.6.8.dev2/docs/website/static/img/undraw_monitor.svg
--rw-rw-rw-   0 root         (0) root         (0)    15536 2022-09-02 11:29:49.000000 soil-sdk-0.6.8.dev2/docs/website/static/img/undraw_note_list.svg
--rw-rw-rw-   0 root         (0) root         (0)    26627 2022-09-02 11:29:49.000000 soil-sdk-0.6.8.dev2/docs/website/static/img/undraw_online.svg
--rw-rw-rw-   0 root         (0) root         (0)    16533 2022-09-02 11:29:49.000000 soil-sdk-0.6.8.dev2/docs/website/static/img/undraw_open_source.svg
--rw-rw-rw-   0 root         (0) root         (0)    36675 2022-09-02 11:29:49.000000 soil-sdk-0.6.8.dev2/docs/website/static/img/undraw_operating_system.svg
--rw-rw-rw-   0 root         (0) root         (0)    24273 2022-09-02 11:29:49.000000 soil-sdk-0.6.8.dev2/docs/website/static/img/undraw_react.svg
--rw-rw-rw-   0 root         (0) root         (0)     9259 2022-09-02 11:29:49.000000 soil-sdk-0.6.8.dev2/docs/website/static/img/undraw_server_push_vtms.svg
--rw-rw-rw-   0 root         (0) root         (0)     9421 2022-09-02 11:29:49.000000 soil-sdk-0.6.8.dev2/docs/website/static/img/undraw_tweetstorm.svg
--rw-rw-rw-   0 root         (0) root         (0)    19900 2022-09-02 11:29:49.000000 soil-sdk-0.6.8.dev2/docs/website/static/img/undraw_version_control_9bpv.svg
--rw-rw-rw-   0 root         (0) root         (0)    29040 2022-09-02 11:29:49.000000 soil-sdk-0.6.8.dev2/docs/website/static/img/undraw_youtube_tutorial.svg
--rw-rw-rw-   0 root         (0) root         (0)      305 2022-09-02 11:29:49.000000 soil-sdk-0.6.8.dev2/pydoc-markdown-library.yml
--rw-rw-rw-   0 root         (0) root         (0)      305 2022-09-02 11:29:49.000000 soil-sdk-0.6.8.dev2/pydoc-markdown.yml
--rw-rw-rw-   0 root         (0) root         (0)      178 2023-03-09 10:25:17.000000 soil-sdk-0.6.8.dev2/pyrightconfig.json
--rw-rw-rw-   0 root         (0) root         (0)     1308 2023-03-10 09:30:31.671071 soil-sdk-0.6.8.dev2/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      109 2023-03-10 09:05:11.000000 soil-sdk-0.6.8.dev2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-10 09:30:31.667071 soil-sdk-0.6.8.dev2/soil/
--rw-rw-rw-   0 root         (0) root         (0)      703 2023-03-10 09:05:11.000000 soil-sdk-0.6.8.dev2/soil/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-10 09:30:31.667071 soil-sdk-0.6.8.dev2/soil/alerts/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-09-02 11:29:49.000000 soil-sdk-0.6.8.dev2/soil/alerts/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      349 2022-09-06 12:27:32.000000 soil-sdk-0.6.8.dev2/soil/alerts/alerts.py
--rw-rw-rw-   0 root         (0) root         (0)      618 2023-03-09 10:25:17.000000 soil-sdk-0.6.8.dev2/soil/alias.py
--rw-rw-rw-   0 root         (0) root         (0)    10030 2023-01-23 11:00:18.000000 soil-sdk-0.6.8.dev2/soil/api.py
--rw-rw-rw-   0 root         (0) root         (0)     5103 2022-09-06 12:27:32.000000 soil-sdk-0.6.8.dev2/soil/configuration.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-10 09:30:31.667071 soil-sdk-0.6.8.dev2/soil/connectors/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-09-02 11:29:49.000000 soil-sdk-0.6.8.dev2/soil/connectors/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1046 2022-09-02 11:29:49.000000 soil-sdk-0.6.8.dev2/soil/connectors/elastic_search.py
--rw-rw-rw-   0 root         (0) root         (0)     2696 2023-03-10 09:05:11.000000 soil-sdk-0.6.8.dev2/soil/data.py
--rw-rw-rw-   0 root         (0) root         (0)     4706 2022-09-02 11:29:49.000000 soil-sdk-0.6.8.dev2/soil/data_structure.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-10 09:30:31.667071 soil-sdk-0.6.8.dev2/soil/data_structures/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-09-02 11:29:49.000000 soil-sdk-0.6.8.dev2/soil/data_structures/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1794 2022-09-02 11:29:49.000000 soil-sdk-0.6.8.dev2/soil/decorator.py
--rw-rw-rw-   0 root         (0) root         (0)      503 2022-09-02 11:29:49.000000 soil-sdk-0.6.8.dev2/soil/dictionary.py
--rw-rw-rw-   0 root         (0) root         (0)     1922 2022-09-02 11:29:49.000000 soil-sdk-0.6.8.dev2/soil/errors.py
--rw-rw-rw-   0 root         (0) root         (0)     2128 2023-01-24 10:13:27.000000 soil-sdk-0.6.8.dev2/soil/finder.py
--rw-rw-rw-   0 root         (0) root         (0)      146 2022-09-06 12:27:32.000000 soil-sdk-0.6.8.dev2/soil/logger.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-10 09:30:31.667071 soil-sdk-0.6.8.dev2/soil/modules/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-09-02 11:29:49.000000 soil-sdk-0.6.8.dev2/soil/modules/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3918 2023-03-07 09:55:51.000000 soil-sdk-0.6.8.dev2/soil/modulify.py
--rw-rw-rw-   0 root         (0) root         (0)     3237 2022-09-06 12:27:32.000000 soil-sdk-0.6.8.dev2/soil/pipeline.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-09-13 13:06:18.000000 soil-sdk-0.6.8.dev2/soil/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-10 09:30:31.667071 soil-sdk-0.6.8.dev2/soil/storage/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-09-02 11:29:49.000000 soil-sdk-0.6.8.dev2/soil/storage/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      663 2023-03-09 08:50:35.000000 soil-sdk-0.6.8.dev2/soil/storage/base_storage.py
--rw-rw-rw-   0 root         (0) root         (0)     1095 2022-09-06 12:27:32.000000 soil-sdk-0.6.8.dev2/soil/storage/compound_storage.py
--rw-rw-rw-   0 root         (0) root         (0)     1507 2022-09-02 11:29:49.000000 soil-sdk-0.6.8.dev2/soil/storage/elasticsearch.py
--rw-rw-rw-   0 root         (0) root         (0)     1665 2022-09-02 11:29:49.000000 soil-sdk-0.6.8.dev2/soil/storage/object_storage.py
--rw-rw-rw-   0 root         (0) root         (0)      813 2022-09-02 11:29:49.000000 soil-sdk-0.6.8.dev2/soil/task.py
--rw-rw-rw-   0 root         (0) root         (0)     1357 2023-03-09 09:42:09.000000 soil-sdk-0.6.8.dev2/soil/types.py
--rw-rw-rw-   0 root         (0) root         (0)     2976 2022-09-02 11:29:49.000000 soil-sdk-0.6.8.dev2/soil/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-10 09:30:31.667071 soil-sdk-0.6.8.dev2/soil_cli/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-09-02 11:29:49.000000 soil-sdk-0.6.8.dev2/soil_cli/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7893 2022-09-06 12:27:32.000000 soil-sdk-0.6.8.dev2/soil_cli/soil_cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-10 09:30:31.671071 soil-sdk-0.6.8.dev2/soil_sdk.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1663 2023-03-10 09:30:31.000000 soil-sdk-0.6.8.dev2/soil_sdk.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    36817 2023-03-10 09:30:31.000000 soil-sdk-0.6.8.dev2/soil_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-10 09:30:31.000000 soil-sdk-0.6.8.dev2/soil_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       48 2023-03-10 09:30:31.000000 soil-sdk-0.6.8.dev2/soil_sdk.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-10 09:30:31.000000 soil-sdk-0.6.8.dev2/soil_sdk.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       47 2023-03-10 09:30:31.000000 soil-sdk-0.6.8.dev2/soil_sdk.egg-info/pbr.json
--rw-r--r--   0 root         (0) root         (0)      216 2023-03-10 09:30:31.000000 soil-sdk-0.6.8.dev2/soil_sdk.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2023-03-10 09:30:31.000000 soil-sdk-0.6.8.dev2/soil_sdk.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-10 09:30:31.671071 soil-sdk-0.6.8.dev2/test/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-09-02 11:29:49.000000 soil-sdk-0.6.8.dev2/test/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-10 09:30:31.671071 soil-sdk-0.6.8.dev2/test/unit/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-09-02 11:29:49.000000 soil-sdk-0.6.8.dev2/test/unit/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-10 09:30:31.671071 soil-sdk-0.6.8.dev2/test/unit/soil/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-09-02 11:29:49.000000 soil-sdk-0.6.8.dev2/test/unit/soil/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1514 2022-09-06 12:27:32.000000 soil-sdk-0.6.8.dev2/test/unit/soil/test_alerts.py
--rw-rw-rw-   0 root         (0) root         (0)    12383 2023-03-09 10:25:17.000000 soil-sdk-0.6.8.dev2/test/unit/soil/test_alias.py
--rw-rw-rw-   0 root         (0) root         (0)    10457 2023-03-09 09:42:09.000000 soil-sdk-0.6.8.dev2/test/unit/soil/test_data.py
--rw-rw-rw-   0 root         (0) root         (0)     2629 2022-09-02 11:29:49.000000 soil-sdk-0.6.8.dev2/test/unit/soil/test_decorator.py
--rw-rw-rw-   0 root         (0) root         (0)     3606 2022-09-06 12:27:32.000000 soil-sdk-0.6.8.dev2/test/unit/soil/test_dictionary.py
--rw-rw-rw-   0 root         (0) root         (0)     2587 2023-01-24 10:13:27.000000 soil-sdk-0.6.8.dev2/test/unit/soil/test_finder.py
--rw-rw-rw-   0 root         (0) root         (0)    11400 2023-02-16 12:38:32.000000 soil-sdk-0.6.8.dev2/test/unit/soil/test_pipelines.py
--rw-rw-rw-   0 root         (0) root         (0)      510 2022-09-06 12:27:32.000000 soil-sdk-0.6.8.dev2/test/unit/soil/test_task.py
--rw-rw-rw-   0 root         (0) root         (0)    34958 2022-09-06 12:27:32.000000 soil-sdk-0.6.8.dev2/test/unit/soil/test_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 10:23:33.011042 soil-sdk-0.6.9/
+-rw-rw-rw-   0 root         (0) root         (0)    53248 2023-03-22 10:19:17.000000 soil-sdk-0.6.9/.coverage
+-rw-rw-rw-   0 root         (0) root         (0)      877 2023-03-10 09:30:26.000000 soil-sdk-0.6.9/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1580 2023-03-09 09:42:09.000000 soil-sdk-0.6.9/.pre-commit-config.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 10:23:32.931040 soil-sdk-0.6.9/.vscode/
+-rw-rw-rw-   0 root         (0) root         (0)      370 2022-09-02 11:29:48.000000 soil-sdk-0.6.9/.vscode/launch.json
+-rw-rw-rw-   0 root         (0) root         (0)      611 2022-09-02 11:29:48.000000 soil-sdk-0.6.9/.vscode/settings.json
+-rw-rw-rw-   0 root         (0) root         (0)      202 2023-03-22 10:23:32.000000 soil-sdk-0.6.9/AUTHORS
+-rw-rw-rw-   0 root         (0) root         (0)     3040 2023-03-22 10:23:32.000000 soil-sdk-0.6.9/ChangeLog
+-rw-r--r--   0 root         (0) root         (0)     1658 2023-03-22 10:23:33.011042 soil-sdk-0.6.9/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1330 2023-03-10 09:30:26.000000 soil-sdk-0.6.9/README.md
+-rw-rw-rw-   0 root         (0) root         (0)       16 2022-09-06 12:27:32.000000 soil-sdk-0.6.9/bandit.yml
+-rw-rw-rw-   0 root         (0) root         (0)      221 2022-09-02 11:29:48.000000 soil-sdk-0.6.9/dependabot.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 10:23:32.931040 soil-sdk-0.6.9/docker/
+-rw-rw-rw-   0 root         (0) root         (0)      395 2023-03-10 09:05:11.000000 soil-sdk-0.6.9/docker/Dockerfile-test
+-rw-rw-rw-   0 root         (0) root         (0)      140 2023-03-09 10:25:17.000000 soil-sdk-0.6.9/docker/docker-compose-test.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 10:23:32.931040 soil-sdk-0.6.9/docs/
+-rw-rw-rw-   0 root         (0) root         (0)       21 2022-09-02 11:29:48.000000 soil-sdk-0.6.9/docs/.dockerignore
+-rw-rw-rw-   0 root         (0) root         (0)      165 2022-09-02 11:29:48.000000 soil-sdk-0.6.9/docs/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)      145 2022-09-02 11:29:48.000000 soil-sdk-0.6.9/docs/Dockerfile
+-rw-rw-rw-   0 root         (0) root         (0)      497 2022-09-02 11:29:48.000000 soil-sdk-0.6.9/docs/docker-compose.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 10:23:32.927040 soil-sdk-0.6.9/docs/docs/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 10:23:32.931040 soil-sdk-0.6.9/docs/docs/assets/
+-rw-rw-rw-   0 root         (0) root         (0)    19945 2022-09-02 11:29:48.000000 soil-sdk-0.6.9/docs/docs/assets/example-app-dir.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 10:23:32.931040 soil-sdk-0.6.9/docs/docs/sdk-reference/
+-rw-rw-rw-   0 root         (0) root         (0)      980 2022-09-02 11:29:48.000000 soil-sdk-0.6.9/docs/docs/sdk-reference/sidebar.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 10:23:32.935041 soil-sdk-0.6.9/docs/docs/sdk-reference/soil/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 10:23:32.935041 soil-sdk-0.6.9/docs/docs/sdk-reference/soil/alerts/
+-rw-rw-rw-   0 root         (0) root         (0)      277 2022-09-02 11:29:48.000000 soil-sdk-0.6.9/docs/docs/sdk-reference/soil/alerts/alerts.md
+-rw-rw-rw-   0 root         (0) root         (0)      278 2022-09-02 11:29:48.000000 soil-sdk-0.6.9/docs/docs/sdk-reference/soil/alias.md
+-rw-rw-rw-   0 root         (0) root         (0)     2135 2022-09-02 11:29:48.000000 soil-sdk-0.6.9/docs/docs/sdk-reference/soil/api.md
+-rw-rw-rw-   0 root         (0) root         (0)      528 2022-09-02 11:29:48.000000 soil-sdk-0.6.9/docs/docs/sdk-reference/soil/configuration.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 10:23:32.935041 soil-sdk-0.6.9/docs/docs/sdk-reference/soil/connectors/
+-rw-rw-rw-   0 root         (0) root         (0)      917 2022-09-02 11:29:48.000000 soil-sdk-0.6.9/docs/docs/sdk-reference/soil/connectors/elastic_search.md
+-rw-rw-rw-   0 root         (0) root         (0)      240 2022-09-02 11:29:48.000000 soil-sdk-0.6.9/docs/docs/sdk-reference/soil/data.md
+-rw-rw-rw-   0 root         (0) root         (0)      838 2022-09-02 11:29:48.000000 soil-sdk-0.6.9/docs/docs/sdk-reference/soil/data_structure.md
+-rw-rw-rw-   0 root         (0) root         (0)      542 2022-09-02 11:29:48.000000 soil-sdk-0.6.9/docs/docs/sdk-reference/soil/decorator.md
+-rw-rw-rw-   0 root         (0) root         (0)      302 2022-09-02 11:29:48.000000 soil-sdk-0.6.9/docs/docs/sdk-reference/soil/dictionary.md
+-rw-rw-rw-   0 root         (0) root         (0)     2520 2022-09-02 11:29:48.000000 soil-sdk-0.6.9/docs/docs/sdk-reference/soil/errors.md
+-rw-rw-rw-   0 root         (0) root         (0)     1077 2022-09-02 11:29:48.000000 soil-sdk-0.6.9/docs/docs/sdk-reference/soil/finder.md
+-rw-rw-rw-   0 root         (0) root         (0)      545 2022-09-02 11:29:48.000000 soil-sdk-0.6.9/docs/docs/sdk-reference/soil/modulify.md
+-rw-rw-rw-   0 root         (0) root         (0)      756 2022-09-02 11:29:48.000000 soil-sdk-0.6.9/docs/docs/sdk-reference/soil/pipeline.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 10:23:32.935041 soil-sdk-0.6.9/docs/docs/sdk-reference/soil/storage/
+-rw-rw-rw-   0 root         (0) root         (0)      622 2022-09-02 11:29:48.000000 soil-sdk-0.6.9/docs/docs/sdk-reference/soil/storage/base_storage.md
+-rw-rw-rw-   0 root         (0) root         (0)     1017 2022-09-02 11:29:48.000000 soil-sdk-0.6.9/docs/docs/sdk-reference/soil/storage/compound_storage.md
+-rw-rw-rw-   0 root         (0) root         (0)     1245 2022-09-02 11:29:48.000000 soil-sdk-0.6.9/docs/docs/sdk-reference/soil/storage/elasticsearch.md
+-rw-rw-rw-   0 root         (0) root         (0)     1415 2022-09-02 11:29:48.000000 soil-sdk-0.6.9/docs/docs/sdk-reference/soil/storage/object_storage.md
+-rw-rw-rw-   0 root         (0) root         (0)      599 2022-09-02 11:29:48.000000 soil-sdk-0.6.9/docs/docs/sdk-reference/soil/task.md
+-rw-rw-rw-   0 root         (0) root         (0)      466 2022-09-02 11:29:48.000000 soil-sdk-0.6.9/docs/docs/sdk-reference/soil/types.md
+-rw-rw-rw-   0 root         (0) root         (0)     1585 2022-09-02 11:29:48.000000 soil-sdk-0.6.9/docs/docs/sdk-reference/soil/utils.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 10:23:32.939041 soil-sdk-0.6.9/docs/docs/soil-library/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 10:23:32.939041 soil-sdk-0.6.9/docs/docs/soil-library/data_structures/
+-rw-rw-rw-   0 root         (0) root         (0)      166 2022-09-02 11:29:48.000000 soil-sdk-0.6.9/docs/docs/soil-library/data_structures/NBClusters.md
+-rw-rw-rw-   0 root         (0) root         (0)     1702 2022-09-02 11:29:48.000000 soil-sdk-0.6.9/docs/docs/soil-library/data_structures/data_structure.md
+-rw-rw-rw-   0 root         (0) root         (0)      209 2022-09-02 11:29:48.000000 soil-sdk-0.6.9/docs/docs/soil-library/data_structures/frequent_itemsets.md
+-rw-rw-rw-   0 root         (0) root         (0)      809 2022-09-02 11:29:48.000000 soil-sdk-0.6.9/docs/docs/soil-library/data_structures/hypergraph.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 10:23:32.939041 soil-sdk-0.6.9/docs/docs/soil-library/data_structures/predefined/
+-rw-rw-rw-   0 root         (0) root         (0)      351 2022-09-02 11:29:48.000000 soil-sdk-0.6.9/docs/docs/soil-library/data_structures/predefined/dict.md
+-rw-rw-rw-   0 root         (0) root         (0)      351 2022-09-02 11:29:48.000000 soil-sdk-0.6.9/docs/docs/soil-library/data_structures/predefined/list.md
+-rw-rw-rw-   0 root         (0) root         (0)      378 2022-09-02 11:29:48.000000 soil-sdk-0.6.9/docs/docs/soil-library/data_structures/predefined/ndarray.md
+-rw-rw-rw-   0 root         (0) root         (0)      505 2022-09-02 11:29:48.000000 soil-sdk-0.6.9/docs/docs/soil-library/data_structures/predefined/object_ds.md
+-rw-rw-rw-   0 root         (0) root         (0)      401 2022-09-02 11:29:48.000000 soil-sdk-0.6.9/docs/docs/soil-library/data_structures/predefined/pd_data_frame.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 10:23:32.939041 soil-sdk-0.6.9/docs/docs/soil-library/data_structures/streams/
+-rw-rw-rw-   0 root         (0) root         (0)      512 2022-09-02 11:29:48.000000 soil-sdk-0.6.9/docs/docs/soil-library/data_structures/streams/patients.md
+-rw-rw-rw-   0 root         (0) root         (0)      348 2022-09-02 11:29:48.000000 soil-sdk-0.6.9/docs/docs/soil-library/data_structures/streams/stream.md
+-rw-rw-rw-   0 root         (0) root         (0)      474 2022-09-02 11:29:48.000000 soil-sdk-0.6.9/docs/docs/soil-library/data_structures/streams/trajectory_clusters.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 10:23:32.939041 soil-sdk-0.6.9/docs/docs/soil-library/modules/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 10:23:32.939041 soil-sdk-0.6.9/docs/docs/soil-library/modules/clustering/
+-rw-rw-rw-   0 root         (0) root         (0)     1263 2022-09-02 11:29:48.000000 soil-sdk-0.6.9/docs/docs/soil-library/modules/clustering/NBClustering.md
+-rw-rw-rw-   0 root         (0) root         (0)      892 2022-09-02 11:29:48.000000 soil-sdk-0.6.9/docs/docs/soil-library/modules/clustering/NBClustering_categorical.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 10:23:32.939041 soil-sdk-0.6.9/docs/docs/soil-library/modules/clustering/SIDIWO/
+-rw-rw-rw-   0 root         (0) root         (0)     1815 2022-09-02 11:29:48.000000 soil-sdk-0.6.9/docs/docs/soil-library/modules/clustering/SIDIWO/sidiwo.md
+-rw-rw-rw-   0 root         (0) root         (0)      412 2022-09-02 11:29:48.000000 soil-sdk-0.6.9/docs/docs/soil-library/modules/experiment.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 10:23:32.939041 soil-sdk-0.6.9/docs/docs/soil-library/modules/higher_order/
+-rw-rw-rw-   0 root         (0) root         (0)     1673 2022-09-02 11:29:48.000000 soil-sdk-0.6.9/docs/docs/soil-library/modules/higher_order/Predictor.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 10:23:32.939041 soil-sdk-0.6.9/docs/docs/soil-library/modules/itemsets/
+-rw-rw-rw-   0 root         (0) root         (0)      353 2022-09-02 11:29:48.000000 soil-sdk-0.6.9/docs/docs/soil-library/modules/itemsets/frequent_itemsets_compare.md
+-rw-rw-rw-   0 root         (0) root         (0)      297 2022-09-02 11:29:48.000000 soil-sdk-0.6.9/docs/docs/soil-library/modules/itemsets/frequent_itemsets_hypergraph.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 10:23:32.923040 soil-sdk-0.6.9/docs/docs/soil-library/modules/preprocessing/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 10:23:32.943041 soil-sdk-0.6.9/docs/docs/soil-library/modules/preprocessing/filters/
+-rw-rw-rw-   0 root         (0) root         (0)      222 2022-09-02 11:29:48.000000 soil-sdk-0.6.9/docs/docs/soil-library/modules/preprocessing/filters/events_filter.md
+-rw-rw-rw-   0 root         (0) root         (0)      884 2022-09-02 11:29:48.000000 soil-sdk-0.6.9/docs/docs/soil-library/modules/preprocessing/filters/row_filter.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 10:23:32.943041 soil-sdk-0.6.9/docs/docs/soil-library/modules/statistics/
+-rw-rw-rw-   0 root         (0) root         (0)      276 2022-09-02 11:29:48.000000 soil-sdk-0.6.9/docs/docs/soil-library/modules/statistics/customstatistics.md
+-rw-rw-rw-   0 root         (0) root         (0)      273 2022-09-02 11:29:48.000000 soil-sdk-0.6.9/docs/docs/soil-library/modules/statistics/time_statistics.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 10:23:32.943041 soil-sdk-0.6.9/docs/docs/soil-library/modules/temporal/
+-rw-rw-rw-   0 root         (0) root         (0)      959 2022-09-02 11:29:48.000000 soil-sdk-0.6.9/docs/docs/soil-library/modules/temporal/trajectories.md
+-rw-rw-rw-   0 root         (0) root         (0)     2821 2022-09-02 11:29:48.000000 soil-sdk-0.6.9/docs/docs/soil-library/sidebar.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 10:23:32.943041 soil-sdk-0.6.9/docs/docs/tutorial/
+-rw-rw-rw-   0 root         (0) root         (0)     2719 2022-09-02 11:29:48.000000 soil-sdk-0.6.9/docs/docs/tutorial/alerts.md
+-rw-rw-rw-   0 root         (0) root         (0)     3905 2022-09-02 11:29:48.000000 soil-sdk-0.6.9/docs/docs/tutorial/data-structures.md
+-rw-rw-rw-   0 root         (0) root         (0)     2540 2022-09-02 11:29:48.000000 soil-sdk-0.6.9/docs/docs/tutorial/data.md
+-rw-rw-rw-   0 root         (0) root         (0)     1486 2022-09-02 11:29:48.000000 soil-sdk-0.6.9/docs/docs/tutorial/deployments.md
+-rw-rw-rw-   0 root         (0) root         (0)     2917 2023-03-07 10:10:25.000000 soil-sdk-0.6.9/docs/docs/tutorial/get-started.mdx
+-rw-rw-rw-   0 root         (0) root         (0)     2681 2022-09-02 11:29:48.000000 soil-sdk-0.6.9/docs/docs/tutorial/logging.md
+-rw-rw-rw-   0 root         (0) root         (0)     2847 2022-09-02 11:29:48.000000 soil-sdk-0.6.9/docs/docs/tutorial/modules.md
+-rw-rw-rw-   0 root         (0) root         (0)      672 2022-09-02 11:29:48.000000 soil-sdk-0.6.9/docs/docs/tutorial/notebooks.md
+-rw-rw-rw-   0 root         (0) root         (0)     1942 2022-09-02 11:29:48.000000 soil-sdk-0.6.9/docs/docs/tutorial/scripts.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 10:23:32.943041 soil-sdk-0.6.9/docs/website/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 10:23:32.947041 soil-sdk-0.6.9/docs/website/.docusaurus/
+-rw-rw-rw-   0 root         (0) root         (0)      260 2023-02-17 10:34:02.000000 soil-sdk-0.6.9/docs/website/.docusaurus/DONT-EDIT-THIS-FOLDER
+-rw-rw-rw-   0 root         (0) root         (0)    20016 2023-02-17 10:34:02.000000 soil-sdk-0.6.9/docs/website/.docusaurus/client-manifest.json
+-rw-rw-rw-   0 root         (0) root         (0)      697 2023-02-17 10:34:02.000000 soil-sdk-0.6.9/docs/website/.docusaurus/client-modules.js
+-rw-rw-rw-   0 root         (0) root         (0)        2 2023-02-17 10:34:02.000000 soil-sdk-0.6.9/docs/website/.docusaurus/codeTranslations.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 10:23:32.927040 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-blog/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 10:23:32.947041 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-blog/default/
+-rw-rw-rw-   0 root         (0) root         (0)    13142 2023-02-17 10:34:02.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-blog/default/blog-archive-80c.json
+-rw-rw-rw-   0 root         (0) root         (0)      151 2023-02-17 10:34:02.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-blog/default/blog-c06.json
+-rw-rw-rw-   0 root         (0) root         (0)      559 2023-02-17 10:34:02.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-blog/default/blog-post-list-prop-default.json
+-rw-rw-rw-   0 root         (0) root         (0)       65 2023-02-17 10:34:02.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-blog/default/plugin-route-context-module-100.json
+-rw-rw-rw-   0 root         (0) root         (0)     1073 2023-02-17 10:34:02.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-blog/default/site-blog-2016-03-11-blog-post-md-bf9.json
+-rw-rw-rw-   0 root         (0) root         (0)     1206 2023-02-17 10:34:02.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-blog/default/site-blog-2017-04-10-blog-post-two-md-dfa.json
+-rw-rw-rw-   0 root         (0) root         (0)     1071 2023-02-17 10:34:02.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-blog/default/site-blog-2017-09-25-testing-rss-md-4d8.json
+-rw-rw-rw-   0 root         (0) root         (0)      827 2023-02-17 10:34:02.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-blog/default/site-blog-2017-09-26-adding-rss-md-ad7.json
+-rw-rw-rw-   0 root         (0) root         (0)      760 2023-02-17 10:34:02.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-blog/default/site-blog-2017-10-24-new-version-1-0-0-md-bbb.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 10:23:32.927040 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 10:23:32.995041 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/
+-rw-rw-rw-   0 root         (0) root         (0)       65 2023-02-17 10:34:02.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/plugin-route-context-module-100.json
+-rw-rw-rw-   0 root         (0) root         (0)      633 2022-09-02 11:29:48.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-docs-sdk-reference-soil-alias-md-698.json
+-rw-rw-rw-   0 root         (0) root         (0)      614 2022-09-02 11:29:48.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-docs-sdk-reference-soil-api-md-fbe.json
+-rw-rw-rw-   0 root         (0) root         (0)      684 2022-09-02 11:29:48.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-docs-sdk-reference-soil-cli-soil-cli-md-727.json
+-rw-rw-rw-   0 root         (0) root         (0)      673 2022-09-02 11:29:48.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-docs-sdk-reference-soil-configuration-md-707.json
+-rw-rw-rw-   0 root         (0) root         (0)      760 2022-09-02 11:29:48.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-docs-sdk-reference-soil-connectors-elastic-search-md-eca.json
+-rw-rw-rw-   0 root         (0) root         (0)      586 2022-09-02 11:29:48.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-docs-sdk-reference-soil-data-md-d6b.json
+-rw-rw-rw-   0 root         (0) root         (0)      686 2022-09-02 11:29:48.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-docs-sdk-reference-soil-data-structure-md-e8d.json
+-rw-rw-rw-   0 root         (0) root         (0)      632 2022-09-02 11:29:48.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-docs-sdk-reference-soil-finder-md-60a.json
+-rw-rw-rw-   0 root         (0) root         (0)      643 2022-09-02 11:29:48.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-docs-sdk-reference-soil-modulify-md-0c9.json
+-rw-rw-rw-   0 root         (0) root         (0)      630 2022-09-02 11:29:48.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-docs-sdk-reference-soil-pipeline-md-312.json
+-rw-rw-rw-   0 root         (0) root         (0)      601 2022-09-02 11:29:48.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-docs-sdk-reference-soil-types-md-24f.json
+-rw-rw-rw-   0 root         (0) root         (0)      578 2022-09-02 11:29:48.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-sdk-reference-sdk-reference-md-a6b.json
+-rw-rw-rw-   0 root         (0) root         (0)     1035 2023-02-17 10:34:02.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-sdk-reference-soil-alerts-alerts-md-231.json
+-rw-rw-rw-   0 root         (0) root         (0)      963 2023-02-17 10:34:02.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-sdk-reference-soil-alias-md-2bb.json
+-rw-rw-rw-   0 root         (0) root         (0)      936 2023-02-17 10:34:02.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-sdk-reference-soil-api-md-cf6.json
+-rw-rw-rw-   0 root         (0) root         (0)      654 2022-09-02 11:29:48.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-sdk-reference-soil-cli-soil-cli-md-c6c.json
+-rw-rw-rw-   0 root         (0) root         (0)      983 2023-02-17 10:34:02.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-sdk-reference-soil-configuration-md-b6d.json
+-rw-rw-rw-   0 root         (0) root         (0)      896 2023-02-17 10:34:02.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-sdk-reference-soil-connectors-elastic-search-md-8f4.json
+-rw-rw-rw-   0 root         (0) root         (0)      927 2023-02-17 10:34:02.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-sdk-reference-soil-data-md-d6c.json
+-rw-rw-rw-   0 root         (0) root         (0)     1009 2023-02-17 10:34:02.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-sdk-reference-soil-data-structure-md-3d5.json
+-rw-rw-rw-   0 root         (0) root         (0)      970 2023-02-17 10:34:02.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-sdk-reference-soil-decorator-md-6e4.json
+-rw-rw-rw-   0 root         (0) root         (0)      989 2023-02-17 10:34:02.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-sdk-reference-soil-dictionary-md-7b7.json
+-rw-rw-rw-   0 root         (0) root         (0)      927 2023-02-17 10:34:02.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-sdk-reference-soil-errors-md-4c9.json
+-rw-rw-rw-   0 root         (0) root         (0)      949 2023-02-17 10:34:02.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-sdk-reference-soil-finder-md-839.json
+-rw-rw-rw-   0 root         (0) root         (0)      962 2023-02-17 10:34:02.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-sdk-reference-soil-modulify-md-37b.json
+-rw-rw-rw-   0 root         (0) root         (0)      945 2023-02-17 10:34:02.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-sdk-reference-soil-pipeline-md-5a1.json
+-rw-rw-rw-   0 root         (0) root         (0)     1073 2023-02-17 10:34:02.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-sdk-reference-soil-storage-base-storage-md-4fa.json
+-rw-rw-rw-   0 root         (0) root         (0)     1131 2023-02-17 10:34:02.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-sdk-reference-soil-storage-compound-storage-md-96f.json
+-rw-rw-rw-   0 root         (0) root         (0)     1115 2023-02-17 10:34:02.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-sdk-reference-soil-storage-elasticsearch-md-f3d.json
+-rw-rw-rw-   0 root         (0) root         (0)     1085 2023-02-17 10:34:02.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-sdk-reference-soil-storage-object-storage-md-ce3.json
+-rw-rw-rw-   0 root         (0) root         (0)      901 2023-02-17 10:34:02.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-sdk-reference-soil-task-md-a67.json
+-rw-rw-rw-   0 root         (0) root         (0)      907 2023-02-17 10:34:02.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-sdk-reference-soil-types-md-3ef.json
+-rw-rw-rw-   0 root         (0) root         (0)      835 2023-02-17 10:34:02.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-sdk-reference-soil-utils-md-092.json
+-rw-rw-rw-   0 root         (0) root         (0)     1140 2023-02-17 10:34:02.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-data-structures-data-structure-md-1fb.json
+-rw-rw-rw-   0 root         (0) root         (0)     1155 2023-02-17 10:34:02.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-data-structures-frequent-itemsets-md-3bb.json
+-rw-rw-rw-   0 root         (0) root         (0)     1092 2023-02-17 10:34:02.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-data-structures-hypergraph-md-c0e.json
+-rw-rw-rw-   0 root         (0) root         (0)      903 2022-09-02 11:29:48.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-data-structures-init-md-de6.json
+-rw-rw-rw-   0 root         (0) root         (0)      903 2022-09-02 11:29:48.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-data-structures-model-md-0ad.json
+-rw-rw-rw-   0 root         (0) root         (0)     1076 2022-09-02 11:29:48.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-data-structures-nb-clusters-categorical-md-046.json
+-rw-rw-rw-   0 root         (0) root         (0)     1091 2023-02-17 10:34:02.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-data-structures-nb-clusters-md-7ed.json
+-rw-rw-rw-   0 root         (0) root         (0)      977 2022-09-02 11:29:48.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-data-structures-paginated-list-md-973.json
+-rw-rw-rw-   0 root         (0) root         (0)     1139 2023-02-17 10:34:02.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-data-structures-predefined-dict-md-379.json
+-rw-rw-rw-   0 root         (0) root         (0)      995 2022-09-02 11:29:48.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-data-structures-predefined-init-md-575.json
+-rw-rw-rw-   0 root         (0) root         (0)     1126 2023-02-17 10:34:02.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-data-structures-predefined-list-md-5ee.json
+-rw-rw-rw-   0 root         (0) root         (0)     1145 2023-02-17 10:34:02.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-data-structures-predefined-ndarray-md-7db.json
+-rw-rw-rw-   0 root         (0) root         (0)     1191 2023-02-17 10:34:02.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-data-structures-predefined-object-ds-md-f15.json
+-rw-rw-rw-   0 root         (0) root         (0)     1213 2023-02-17 10:34:02.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-data-structures-predefined-pd-data-frame-md-a71.json
+-rw-rw-rw-   0 root         (0) root         (0)      935 2022-09-02 11:29:48.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-data-structures-statistics-md-07b.json
+-rw-rw-rw-   0 root         (0) root         (0)     1082 2022-09-02 11:29:48.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-data-structures-streams-association-rules-md-820.json
+-rw-rw-rw-   0 root         (0) root         (0)      957 2022-09-02 11:29:48.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-data-structures-streams-init-md-d9b.json
+-rw-rw-rw-   0 root         (0) root         (0)     1129 2023-02-17 10:34:02.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-data-structures-streams-patients-md-60e.json
+-rw-rw-rw-   0 root         (0) root         (0)     1097 2023-02-17 10:34:02.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-data-structures-streams-stream-md-317.json
+-rw-rw-rw-   0 root         (0) root         (0)      996 2023-02-17 10:34:02.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-data-structures-streams-trajectory-clusters-md-1d9.json
+-rw-rw-rw-   0 root         (0) root         (0)     1005 2022-09-02 11:29:48.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-data-structures-time-statistics-md-fcd.json
+-rw-rw-rw-   0 root         (0) root         (0)      957 2022-09-02 11:29:48.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-data-structures-trajectories-md-899.json
+-rw-rw-rw-   0 root         (0) root         (0)     1027 2022-09-02 11:29:48.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-ehra-data-structures-hypergraph-md-084.json
+-rw-rw-rw-   0 root         (0) root         (0)     1071 2022-09-02 11:29:48.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-ehra-data-structures-streams-patients-md-ced.json
+-rw-rw-rw-   0 root         (0) root         (0)     1102 2022-09-02 11:29:48.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-ehra-data-structures-streams-trajectory-clusters-md-7cf.json
+-rw-rw-rw-   0 root         (0) root         (0)     1170 2022-09-02 11:29:48.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-ehra-modules-clustering-nb-clustering-categorical-md-300.json
+-rw-rw-rw-   0 root         (0) root         (0)     1056 2022-09-02 11:29:48.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-ehra-modules-clustering-nb-clustering-md-11b.json
+-rw-rw-rw-   0 root         (0) root         (0)     1108 2022-09-02 11:29:48.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-ehra-modules-clustering-sidiwo-sidiwo-md-266.json
+-rw-rw-rw-   0 root         (0) root         (0)      901 2022-09-02 11:29:48.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-ehra-modules-experiment-md-047.json
+-rw-rw-rw-   0 root         (0) root         (0)     1081 2022-09-02 11:29:48.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-ehra-modules-higher-order-predictor-md-414.json
+-rw-rw-rw-   0 root         (0) root         (0)     1183 2022-09-02 11:29:48.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-ehra-modules-itemsets-frequent-itemsets-compare-md-6e5.json
+-rw-rw-rw-   0 root         (0) root         (0)     1206 2022-09-02 11:29:48.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-ehra-modules-itemsets-frequent-itemsets-hypergraph-md-d85.json
+-rw-rw-rw-   0 root         (0) root         (0)     1157 2022-09-02 11:29:48.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-ehra-modules-preprocessing-filters-events-filter-md-2cf.json
+-rw-rw-rw-   0 root         (0) root         (0)     1142 2022-09-02 11:29:48.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-ehra-modules-preprocessing-filters-row-filter-md-b96.json
+-rw-rw-rw-   0 root         (0) root         (0)     1096 2022-09-02 11:29:48.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-ehra-modules-statistics-customstatistics-md-353.json
+-rw-rw-rw-   0 root         (0) root         (0)     1082 2022-09-02 11:29:48.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-ehra-modules-statistics-time-statistics-md-7fa.json
+-rw-rw-rw-   0 root         (0) root         (0)     1090 2022-09-02 11:29:48.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-ehra-modules-temporal-trajectories-md-419.json
+-rw-rw-rw-   0 root         (0) root         (0)      897 2022-09-02 11:29:48.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-modules-clustering-init-md-349.json
+-rw-rw-rw-   0 root         (0) root         (0)     1250 2023-02-17 10:34:02.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-modules-clustering-nb-clustering-categorical-md-0c4.json
+-rw-rw-rw-   0 root         (0) root         (0)     1148 2023-02-17 10:34:02.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-modules-clustering-nb-clustering-md-19d.json
+-rw-rw-rw-   0 root         (0) root         (0)      994 2022-09-02 11:29:48.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-modules-clustering-sidiwo-init-md-729.json
+-rw-rw-rw-   0 root         (0) root         (0)     1174 2023-02-17 10:34:02.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-modules-clustering-sidiwo-sidiwo-md-478.json
+-rw-rw-rw-   0 root         (0) root         (0)      995 2023-02-17 10:34:02.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-modules-experiment-md-a5e.json
+-rw-rw-rw-   0 root         (0) root         (0)      943 2022-09-02 11:29:48.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-modules-higher-order-init-md-c2b.json
+-rw-rw-rw-   0 root         (0) root         (0)     1165 2023-02-17 10:34:02.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-modules-higher-order-predictor-md-b65.json
+-rw-rw-rw-   0 root         (0) root         (0)      765 2022-09-02 11:29:48.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-modules-init-md-f13.json
+-rw-rw-rw-   0 root         (0) root         (0)     1083 2022-09-02 11:29:48.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-modules-itemsets-association-rules-md-8b6.json
+-rw-rw-rw-   0 root         (0) root         (0)     1292 2023-02-17 10:34:02.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-modules-itemsets-frequent-itemsets-compare-md-49b.json
+-rw-rw-rw-   0 root         (0) root         (0)     1299 2023-02-17 10:34:02.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-modules-itemsets-frequent-itemsets-hypergraph-md-0d1.json
+-rw-rw-rw-   0 root         (0) root         (0)     1048 2022-09-02 11:29:48.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-modules-itemsets-frequent-itemsets-md-ca7.json
+-rw-rw-rw-   0 root         (0) root         (0)      925 2022-09-02 11:29:48.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-modules-itemsets-init-md-a1a.json
+-rw-rw-rw-   0 root         (0) root         (0)     1131 2022-09-02 11:29:48.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-modules-preprocessing-filters-column-filter-md-04c.json
+-rw-rw-rw-   0 root         (0) root         (0)     1278 2023-02-17 10:34:02.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-modules-preprocessing-filters-events-filter-md-59c.json
+-rw-rw-rw-   0 root         (0) root         (0)     1101 2022-09-02 11:29:48.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-modules-preprocessing-filters-flattener-md-1a6.json
+-rw-rw-rw-   0 root         (0) root         (0)     1005 2022-09-02 11:29:48.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-modules-preprocessing-filters-init-md-728.json
+-rw-rw-rw-   0 root         (0) root         (0)     1219 2023-02-17 10:34:02.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-modules-preprocessing-filters-row-filter-md-77e.json
+-rw-rw-rw-   0 root         (0) root         (0)      939 2022-09-02 11:29:48.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-modules-preprocessing-init-md-8d4.json
+-rw-rw-rw-   0 root         (0) root         (0)      946 2022-09-02 11:29:48.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-modules-preprocessing-pipe-md-fd6.json
+-rw-rw-rw-   0 root         (0) root         (0)     1065 2022-09-02 11:29:48.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-modules-preprocessing-sampling-init-md-dba.json
+-rw-rw-rw-   0 root         (0) root         (0)     1126 2022-09-02 11:29:48.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-modules-preprocessing-sampling-reservoir-sampling-md-cfe.json
+-rw-rw-rw-   0 root         (0) root         (0)     1179 2023-02-17 10:34:02.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-modules-statistics-customstatistics-md-3e3.json
+-rw-rw-rw-   0 root         (0) root         (0)      917 2022-09-02 11:29:48.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-modules-statistics-init-md-135.json
+-rw-rw-rw-   0 root         (0) root         (0)      970 2022-09-02 11:29:48.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-modules-statistics-statistics-md-0db.json
+-rw-rw-rw-   0 root         (0) root         (0)     1169 2023-02-17 10:34:02.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-modules-statistics-time-statistics-md-92c.json
+-rw-rw-rw-   0 root         (0) root         (0)      939 2022-09-02 11:29:48.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-modules-temporal-init-md-37a.json
+-rw-rw-rw-   0 root         (0) root         (0)      864 2023-02-17 10:34:02.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-modules-temporal-trajectories-md-285.json
+-rw-rw-rw-   0 root         (0) root         (0)      559 2022-09-02 11:29:48.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-soil-library-md-65d.json
+-rw-rw-rw-   0 root         (0) root         (0)     1135 2023-02-17 10:34:02.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-tutorial-alerts-md-43b.json
+-rw-rw-rw-   0 root         (0) root         (0)      832 2023-02-17 10:34:02.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-tutorial-data-md-0d2.json
+-rw-rw-rw-   0 root         (0) root         (0)     1202 2023-02-17 10:34:02.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-tutorial-data-structures-md-14d.json
+-rw-rw-rw-   0 root         (0) root         (0)     1160 2023-02-17 10:34:02.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-tutorial-deployments-md-62e.json
+-rw-rw-rw-   0 root         (0) root         (0)      609 2022-09-02 11:29:48.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-tutorial-get-started-md-d5b.json
+-rw-rw-rw-   0 root         (0) root         (0)      798 2023-02-17 10:34:02.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-tutorial-get-started-mdx-36a.json
+-rw-rw-rw-   0 root         (0) root         (0)      844 2023-02-17 10:34:02.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-tutorial-logging-md-507.json
+-rw-rw-rw-   0 root         (0) root         (0)      942 2023-02-17 10:34:02.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-tutorial-modules-md-cd8.json
+-rw-rw-rw-   0 root         (0) root         (0)      944 2023-02-17 10:34:02.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-tutorial-notebooks-md-58b.json
+-rw-rw-rw-   0 root         (0) root         (0)     1027 2023-02-17 10:34:02.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-tutorial-scripts-md-0f5.json
+-rw-rw-rw-   0 root         (0) root         (0)      478 2022-09-02 11:29:48.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-tutorial-subtasks-md-e0d.json
+-rw-rw-rw-   0 root         (0) root         (0)      775 2022-09-02 11:29:48.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-1-sdk-reference-sdk-reference-md-59f.json
+-rw-rw-rw-   0 root         (0) root         (0)      853 2022-09-02 11:29:48.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-1-soil-library-soil-library-md-ce1.json
+-rw-rw-rw-   0 root         (0) root         (0)      776 2022-09-02 11:29:48.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-1-tutorial-data-md-e4a.json
+-rw-rw-rw-   0 root         (0) root         (0)      830 2022-09-02 11:29:48.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-1-tutorial-data-structures-md-53e.json
+-rw-rw-rw-   0 root         (0) root         (0)      679 2022-09-02 11:29:48.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-1-tutorial-get-started-md-cbe.json
+-rw-rw-rw-   0 root         (0) root         (0)      567 2022-09-02 11:29:48.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-1-tutorial-logging-md-4a1.json
+-rw-rw-rw-   0 root         (0) root         (0)      894 2022-09-02 11:29:48.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-1-tutorial-modules-md-547.json
+-rw-rw-rw-   0 root         (0) root         (0)      945 2022-09-02 11:29:48.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-1-tutorial-scripts-md-a17.json
+-rw-rw-rw-   0 root         (0) root         (0)      775 2022-09-02 11:29:48.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-2-sdk-reference-sdk-reference-md-62b.json
+-rw-rw-rw-   0 root         (0) root         (0)      853 2022-09-02 11:29:48.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-2-soil-library-soil-library-md-1c7.json
+-rw-rw-rw-   0 root         (0) root         (0)      776 2022-09-02 11:29:48.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-2-tutorial-data-md-278.json
+-rw-rw-rw-   0 root         (0) root         (0)     1124 2022-09-02 11:29:48.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-2-tutorial-data-structures-md-89f.json
+-rw-rw-rw-   0 root         (0) root         (0)      679 2022-09-02 11:29:48.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-2-tutorial-get-started-md-022.json
+-rw-rw-rw-   0 root         (0) root         (0)      567 2022-09-02 11:29:48.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-2-tutorial-logging-md-4c2.json
+-rw-rw-rw-   0 root         (0) root         (0)      894 2022-09-02 11:29:48.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-2-tutorial-modules-md-cdc.json
+-rw-rw-rw-   0 root         (0) root         (0)      945 2022-09-02 11:29:48.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-2-tutorial-scripts-md-d50.json
+-rw-rw-rw-   0 root         (0) root         (0)      775 2022-09-02 11:29:48.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-3-sdk-reference-sdk-reference-md-75e.json
+-rw-rw-rw-   0 root         (0) root         (0)      853 2022-09-02 11:29:48.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-3-soil-library-soil-library-md-aaf.json
+-rw-rw-rw-   0 root         (0) root         (0)      776 2022-09-02 11:29:48.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-3-tutorial-data-md-bc1.json
+-rw-rw-rw-   0 root         (0) root         (0)     1124 2022-09-02 11:29:48.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-3-tutorial-data-structures-md-805.json
+-rw-rw-rw-   0 root         (0) root         (0)      679 2022-09-02 11:29:48.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-3-tutorial-get-started-md-9c5.json
+-rw-rw-rw-   0 root         (0) root         (0)      798 2022-09-02 11:29:48.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-3-tutorial-logging-md-0a4.json
+-rw-rw-rw-   0 root         (0) root         (0)      880 2022-09-02 11:29:48.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-3-tutorial-modules-md-c8e.json
+-rw-rw-rw-   0 root         (0) root         (0)      945 2022-09-02 11:29:48.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-3-tutorial-scripts-md-dbf.json
+-rw-rw-rw-   0 root         (0) root         (0)      775 2022-09-02 11:29:48.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-4-sdk-reference-sdk-reference-md-343.json
+-rw-rw-rw-   0 root         (0) root         (0)      853 2022-09-02 11:29:48.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-4-soil-library-soil-library-md-b38.json
+-rw-rw-rw-   0 root         (0) root         (0)      776 2022-09-02 11:29:48.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-4-tutorial-data-md-8d7.json
+-rw-rw-rw-   0 root         (0) root         (0)     1124 2022-09-02 11:29:48.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-4-tutorial-data-structures-md-b95.json
+-rw-rw-rw-   0 root         (0) root         (0)      679 2022-09-02 11:29:48.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-4-tutorial-get-started-md-c2c.json
+-rw-rw-rw-   0 root         (0) root         (0)      798 2022-09-02 11:29:48.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-4-tutorial-logging-md-750.json
+-rw-rw-rw-   0 root         (0) root         (0)      880 2022-09-02 11:29:48.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-4-tutorial-modules-md-447.json
+-rw-rw-rw-   0 root         (0) root         (0)      945 2022-09-02 11:29:48.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-4-tutorial-scripts-md-904.json
+-rw-rw-rw-   0 root         (0) root         (0)      775 2022-09-02 11:29:48.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-5-sdk-reference-sdk-reference-md-c6e.json
+-rw-rw-rw-   0 root         (0) root         (0)      853 2022-09-02 11:29:48.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-5-soil-library-soil-library-md-f09.json
+-rw-rw-rw-   0 root         (0) root         (0)      776 2022-09-02 11:29:48.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-5-tutorial-data-md-ae6.json
+-rw-rw-rw-   0 root         (0) root         (0)     1124 2022-09-02 11:29:48.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-5-tutorial-data-structures-md-d2f.json
+-rw-rw-rw-   0 root         (0) root         (0)      679 2022-09-02 11:29:48.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-5-tutorial-get-started-md-392.json
+-rw-rw-rw-   0 root         (0) root         (0)      798 2022-09-02 11:29:48.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-5-tutorial-logging-md-645.json
+-rw-rw-rw-   0 root         (0) root         (0)      880 2022-09-02 11:29:48.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-5-tutorial-modules-md-3bc.json
+-rw-rw-rw-   0 root         (0) root         (0)      945 2022-09-02 11:29:48.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-5-tutorial-scripts-md-bd1.json
+-rw-rw-rw-   0 root         (0) root         (0)      775 2022-09-02 11:29:48.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-6-sdk-reference-sdk-reference-md-073.json
+-rw-rw-rw-   0 root         (0) root         (0)      853 2022-09-02 11:29:48.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-6-soil-library-soil-library-md-53e.json
+-rw-rw-rw-   0 root         (0) root         (0)      776 2022-09-02 11:29:48.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-6-tutorial-data-md-cba.json
+-rw-rw-rw-   0 root         (0) root         (0)     1124 2022-09-02 11:29:48.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-6-tutorial-data-structures-md-c96.json
+-rw-rw-rw-   0 root         (0) root         (0)      679 2022-09-02 11:29:48.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-6-tutorial-get-started-md-6a0.json
+-rw-rw-rw-   0 root         (0) root         (0)      798 2022-09-02 11:29:48.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-6-tutorial-logging-md-7c2.json
+-rw-rw-rw-   0 root         (0) root         (0)      880 2022-09-02 11:29:48.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-6-tutorial-modules-md-dd3.json
+-rw-rw-rw-   0 root         (0) root         (0)      945 2022-09-02 11:29:48.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-6-tutorial-scripts-md-e55.json
+-rw-rw-rw-   0 root         (0) root         (0)      775 2022-09-02 11:29:48.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-7-sdk-reference-sdk-reference-md-5bd.json
+-rw-rw-rw-   0 root         (0) root         (0)      853 2022-09-02 11:29:48.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-7-soil-library-soil-library-md-b02.json
+-rw-rw-rw-   0 root         (0) root         (0)      776 2022-09-02 11:29:48.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-7-tutorial-data-md-345.json
+-rw-rw-rw-   0 root         (0) root         (0)     1124 2022-09-02 11:29:48.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-7-tutorial-data-structures-md-b1a.json
+-rw-rw-rw-   0 root         (0) root         (0)      679 2022-09-02 11:29:48.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-7-tutorial-get-started-md-661.json
+-rw-rw-rw-   0 root         (0) root         (0)      798 2022-09-02 11:29:48.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-7-tutorial-logging-md-aae.json
+-rw-rw-rw-   0 root         (0) root         (0)      880 2022-09-02 11:29:48.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-7-tutorial-modules-md-9f2.json
+-rw-rw-rw-   0 root         (0) root         (0)      945 2022-09-02 11:29:48.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-7-tutorial-scripts-md-21c.json
+-rw-rw-rw-   0 root         (0) root         (0)      775 2022-09-02 11:29:48.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-8-sdk-reference-sdk-reference-md-670.json
+-rw-rw-rw-   0 root         (0) root         (0)      853 2022-09-02 11:29:48.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-8-soil-library-soil-library-md-3b4.json
+-rw-rw-rw-   0 root         (0) root         (0)      776 2022-09-02 11:29:48.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-8-tutorial-data-md-e4f.json
+-rw-rw-rw-   0 root         (0) root         (0)     1124 2022-09-02 11:29:48.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-8-tutorial-data-structures-md-04f.json
+-rw-rw-rw-   0 root         (0) root         (0)      679 2022-09-02 11:29:48.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-8-tutorial-get-started-md-610.json
+-rw-rw-rw-   0 root         (0) root         (0)      798 2022-09-02 11:29:48.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-8-tutorial-logging-md-0d8.json
+-rw-rw-rw-   0 root         (0) root         (0)      880 2022-09-02 11:29:48.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-8-tutorial-modules-md-a2c.json
+-rw-rw-rw-   0 root         (0) root         (0)      945 2022-09-02 11:29:48.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-8-tutorial-scripts-md-700.json
+-rw-rw-rw-   0 root         (0) root         (0)      633 2022-09-02 11:29:48.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-1-0-sdk-reference-sdk-reference-md-172.json
+-rw-rw-rw-   0 root         (0) root         (0)      619 2022-09-02 11:29:48.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-1-0-soil-library-soil-library-md-963.json
+-rw-rw-rw-   0 root         (0) root         (0)      543 2022-09-02 11:29:48.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-1-0-tutorial-data-md-eac.json
+-rw-rw-rw-   0 root         (0) root         (0)      913 2022-09-02 11:29:48.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-1-0-tutorial-data-structures-md-f2b.json
+-rw-rw-rw-   0 root         (0) root         (0)      667 2022-09-02 11:29:48.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-1-0-tutorial-get-started-md-526.json
+-rw-rw-rw-   0 root         (0) root         (0)      598 2022-09-02 11:29:48.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-1-0-tutorial-get-started-mdx-539.json
+-rw-rw-rw-   0 root         (0) root         (0)      567 2022-09-02 11:29:48.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-1-0-tutorial-logging-md-3a5.json
+-rw-rw-rw-   0 root         (0) root         (0)      647 2022-09-02 11:29:48.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-1-0-tutorial-modules-md-1ad.json
+-rw-rw-rw-   0 root         (0) root         (0)      746 2022-09-02 11:29:48.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-1-0-tutorial-scripts-md-caa.json
+-rw-rw-rw-   0 root         (0) root         (0)      652 2022-09-02 11:29:48.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-1-1-sdk-reference-soil-alias-md-6d0.json
+-rw-rw-rw-   0 root         (0) root         (0)      633 2022-09-02 11:29:48.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-1-1-sdk-reference-soil-api-md-056.json
+-rw-rw-rw-   0 root         (0) root         (0)      692 2022-09-02 11:29:48.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-1-1-sdk-reference-soil-configuration-md-7c5.json
+-rw-rw-rw-   0 root         (0) root         (0)      779 2022-09-02 11:29:48.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-1-1-sdk-reference-soil-connectors-elastic-search-md-b85.json
+-rw-rw-rw-   0 root         (0) root         (0)      605 2022-09-02 11:29:48.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-1-1-sdk-reference-soil-data-md-797.json
+-rw-rw-rw-   0 root         (0) root         (0)      705 2022-09-02 11:29:48.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-1-1-sdk-reference-soil-data-structure-md-916.json
+-rw-rw-rw-   0 root         (0) root         (0)      651 2022-09-02 11:29:48.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-1-1-sdk-reference-soil-finder-md-c72.json
+-rw-rw-rw-   0 root         (0) root         (0)      662 2022-09-02 11:29:48.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-1-1-sdk-reference-soil-modulify-md-b9a.json
+-rw-rw-rw-   0 root         (0) root         (0)      649 2022-09-02 11:29:48.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-1-1-sdk-reference-soil-pipeline-md-6eb.json
+-rw-rw-rw-   0 root         (0) root         (0)      620 2022-09-02 11:29:48.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-1-1-sdk-reference-soil-types-md-00c.json
+-rw-rw-rw-   0 root         (0) root         (0)      613 2022-09-02 11:29:48.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-1-1-soil-library-soil-library-md-2b7.json
+-rw-rw-rw-   0 root         (0) root         (0)      537 2022-09-02 11:29:48.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-1-1-tutorial-data-md-b95.json
+-rw-rw-rw-   0 root         (0) root         (0)      907 2022-09-02 11:29:48.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-1-1-tutorial-data-structures-md-03c.json
+-rw-rw-rw-   0 root         (0) root         (0)      592 2022-09-02 11:29:48.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-1-1-tutorial-get-started-mdx-cf0.json
+-rw-rw-rw-   0 root         (0) root         (0)      561 2022-09-02 11:29:48.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-1-1-tutorial-logging-md-bb1.json
+-rw-rw-rw-   0 root         (0) root         (0)      641 2022-09-02 11:29:48.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-1-1-tutorial-modules-md-4b3.json
+-rw-rw-rw-   0 root         (0) root         (0)      740 2022-09-02 11:29:48.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-1-1-tutorial-scripts-md-7f6.json
+-rw-rw-rw-   0 root         (0) root         (0)      652 2022-09-02 11:29:48.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-1-2-sdk-reference-soil-alias-md-165.json
+-rw-rw-rw-   0 root         (0) root         (0)      633 2022-09-02 11:29:48.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-1-2-sdk-reference-soil-api-md-f09.json
+-rw-rw-rw-   0 root         (0) root         (0)      692 2022-09-02 11:29:48.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-1-2-sdk-reference-soil-configuration-md-4f6.json
+-rw-rw-rw-   0 root         (0) root         (0)      779 2022-09-02 11:29:48.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-1-2-sdk-reference-soil-connectors-elastic-search-md-224.json
+-rw-rw-rw-   0 root         (0) root         (0)      605 2022-09-02 11:29:48.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-1-2-sdk-reference-soil-data-md-cd7.json
+-rw-rw-rw-   0 root         (0) root         (0)      705 2022-09-02 11:29:48.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-1-2-sdk-reference-soil-data-structure-md-849.json
+-rw-rw-rw-   0 root         (0) root         (0)      651 2022-09-02 11:29:48.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-1-2-sdk-reference-soil-finder-md-da9.json
+-rw-rw-rw-   0 root         (0) root         (0)      662 2022-09-02 11:29:48.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-1-2-sdk-reference-soil-modulify-md-47e.json
+-rw-rw-rw-   0 root         (0) root         (0)      649 2022-09-02 11:29:48.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-1-2-sdk-reference-soil-pipeline-md-945.json
+-rw-rw-rw-   0 root         (0) root         (0)      620 2022-09-02 11:29:48.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-1-2-sdk-reference-soil-types-md-b0e.json
+-rw-rw-rw-   0 root         (0) root         (0)      613 2022-09-02 11:29:48.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-1-2-soil-library-soil-library-md-04e.json
+-rw-rw-rw-   0 root         (0) root         (0)      537 2022-09-02 11:29:48.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-1-2-tutorial-data-md-0e1.json
+-rw-rw-rw-   0 root         (0) root         (0)      907 2022-09-02 11:29:49.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-1-2-tutorial-data-structures-md-ad9.json
+-rw-rw-rw-   0 root         (0) root         (0)      592 2022-09-02 11:29:49.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-1-2-tutorial-get-started-mdx-7f5.json
+-rw-rw-rw-   0 root         (0) root         (0)      561 2022-09-02 11:29:49.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-1-2-tutorial-logging-md-cb9.json
+-rw-rw-rw-   0 root         (0) root         (0)      641 2022-09-02 11:29:49.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-1-2-tutorial-modules-md-ad2.json
+-rw-rw-rw-   0 root         (0) root         (0)      740 2022-09-02 11:29:49.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-1-2-tutorial-scripts-md-aef.json
+-rw-rw-rw-   0 root         (0) root         (0)     1968 2022-09-02 11:29:49.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/version-0-0-1-metadata-prop-e31.json
+-rw-rw-rw-   0 root         (0) root         (0)     1968 2022-09-02 11:29:49.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/version-0-0-2-metadata-prop-b4f.json
+-rw-rw-rw-   0 root         (0) root         (0)     2162 2022-09-02 11:29:49.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/version-0-0-3-metadata-prop-272.json
+-rw-rw-rw-   0 root         (0) root         (0)     2162 2022-09-02 11:29:49.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/version-0-0-4-metadata-prop-937.json
+-rw-rw-rw-   0 root         (0) root         (0)     2162 2022-09-02 11:29:49.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/version-0-0-5-metadata-prop-e97.json
+-rw-rw-rw-   0 root         (0) root         (0)     2162 2022-09-02 11:29:49.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/version-0-0-6-metadata-prop-46a.json
+-rw-rw-rw-   0 root         (0) root         (0)     2162 2022-09-02 11:29:49.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/version-0-0-7-metadata-prop-558.json
+-rw-rw-rw-   0 root         (0) root         (0)     2162 2022-09-02 11:29:49.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/version-0-0-8-metadata-prop-5dc.json
+-rw-rw-rw-   0 root         (0) root         (0)      138 2022-09-02 11:29:49.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/version-0-1-0-metadata-prop-69a.json
+-rw-rw-rw-   0 root         (0) root         (0)      137 2022-09-02 11:29:49.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/version-0-1-1-metadata-prop-aee.json
+-rw-rw-rw-   0 root         (0) root         (0)      137 2022-09-02 11:29:49.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/version-0-1-2-metadata-prop-be9.json
+-rw-rw-rw-   0 root         (0) root         (0)    29936 2023-02-17 10:34:02.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/version-current-metadata-prop-751.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 10:23:32.927040 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-pages/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 10:23:32.995041 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-pages/default/
+-rw-rw-rw-   0 root         (0) root         (0)       66 2023-02-17 10:34:02.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-pages/default/plugin-route-context-module-100.json
+-rw-rw-rw-   0 root         (0) root         (0)       80 2022-09-02 11:29:49.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-pages/default/site-src-pages-index-mdx-e7c.json
+-rw-rw-rw-   0 root         (0) root         (0)       83 2022-09-02 11:29:49.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-pages/default/site-src-pages-test-mdx-362.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 10:23:32.927040 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-debug/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 10:23:32.999042 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-debug/default/
+-rw-rw-rw-   0 root         (0) root         (0)   104640 2022-09-02 11:29:49.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-debug/default/docusaurus-debug-all-content-673.json
+-rw-rw-rw-   0 root         (0) root         (0)       58 2022-09-02 11:29:49.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-debug/default/plugin-route-context-module-100.json
+-rw-rw-rw-   0 root         (0) root         (0)     2663 2022-09-02 11:29:49.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus.config.js
+-rw-rw-rw-   0 root         (0) root         (0)     5946 2023-02-17 10:34:02.000000 soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus.config.mjs
+-rw-rw-rw-   0 root         (0) root         (0)    10462 2023-02-17 10:34:02.000000 soil-sdk-0.6.9/docs/website/.docusaurus/globalData.json
+-rw-rw-rw-   0 root         (0) root         (0)      229 2023-02-17 10:34:02.000000 soil-sdk-0.6.9/docs/website/.docusaurus/i18n.json
+-rw-rw-rw-   0 root         (0) root         (0)    28392 2023-02-17 10:34:02.000000 soil-sdk-0.6.9/docs/website/.docusaurus/registry.js
+-rw-rw-rw-   0 root         (0) root         (0)    13307 2023-02-17 10:34:02.000000 soil-sdk-0.6.9/docs/website/.docusaurus/routes.js
+-rw-rw-rw-   0 root         (0) root         (0)    13579 2023-02-17 10:34:02.000000 soil-sdk-0.6.9/docs/website/.docusaurus/routesChunkNames.json
+-rw-rw-rw-   0 root         (0) root         (0)      840 2023-02-17 10:34:02.000000 soil-sdk-0.6.9/docs/website/.docusaurus/site-metadata.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 10:23:32.999042 soil-sdk-0.6.9/docs/website/blog/
+-rw-rw-rw-   0 root         (0) root         (0)     3295 2022-09-02 11:29:49.000000 soil-sdk-0.6.9/docs/website/blog/2016-03-11-blog-post.md
+-rw-rw-rw-   0 root         (0) root         (0)     3298 2022-09-02 11:29:49.000000 soil-sdk-0.6.9/docs/website/blog/2017-04-10-blog-post-two.md
+-rw-rw-rw-   0 root         (0) root         (0)      480 2022-09-02 11:29:49.000000 soil-sdk-0.6.9/docs/website/blog/2017-09-25-testing-rss.md
+-rw-rw-rw-   0 root         (0) root         (0)      182 2022-09-02 11:29:49.000000 soil-sdk-0.6.9/docs/website/blog/2017-09-26-adding-rss.md
+-rw-rw-rw-   0 root         (0) root         (0)      199 2022-09-02 11:29:49.000000 soil-sdk-0.6.9/docs/website/blog/2017-10-24-new-version-1.0.0.md
+-rw-rw-rw-   0 root         (0) root         (0)     1949 2022-09-02 11:29:49.000000 soil-sdk-0.6.9/docs/website/docusaurus.config.js
+-rw-rw-rw-   0 root         (0) root         (0)      531 2023-02-06 08:17:43.000000 soil-sdk-0.6.9/docs/website/package.json
+-rw-rw-rw-   0 root         (0) root         (0)      447 2022-09-02 11:29:49.000000 soil-sdk-0.6.9/docs/website/sidebars.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 10:23:32.927040 soil-sdk-0.6.9/docs/website/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 10:23:32.999042 soil-sdk-0.6.9/docs/website/src/css/
+-rw-rw-rw-   0 root         (0) root         (0)      276 2022-09-02 11:29:49.000000 soil-sdk-0.6.9/docs/website/src/css/customTheme.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 10:23:32.999042 soil-sdk-0.6.9/docs/website/src/pages/
+-rw-rw-rw-   0 root         (0) root         (0)     4747 2022-09-02 11:29:49.000000 soil-sdk-0.6.9/docs/website/src/pages/index.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 10:23:32.927040 soil-sdk-0.6.9/docs/website/static/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 10:23:32.999042 soil-sdk-0.6.9/docs/website/static/css/
+-rw-rw-rw-   0 root         (0) root         (0)      482 2022-09-02 11:29:49.000000 soil-sdk-0.6.9/docs/website/static/css/custom.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 10:23:33.003042 soil-sdk-0.6.9/docs/website/static/img/
+-rw-rw-rw-   0 root         (0) root         (0)      766 2022-09-02 11:29:49.000000 soil-sdk-0.6.9/docs/website/static/img/favicon.ico
+-rw-rw-rw-   0 root         (0) root         (0)    15538 2022-09-02 11:29:49.000000 soil-sdk-0.6.9/docs/website/static/img/favicon_amalfi.png
+-rw-rw-rw-   0 root         (0) root         (0)     4370 2022-09-02 11:29:49.000000 soil-sdk-0.6.9/docs/website/static/img/oss_logo.png
+-rw-rw-rw-   0 root         (0) root         (0)     4388 2022-09-02 11:29:49.000000 soil-sdk-0.6.9/docs/website/static/img/undraw_abstract_x68e.svg
+-rw-rw-rw-   0 root         (0) root         (0)    17343 2022-09-02 11:29:49.000000 soil-sdk-0.6.9/docs/website/static/img/undraw_code_review.svg
+-rw-rw-rw-   0 root         (0) root         (0)    22330 2022-09-02 11:29:49.000000 soil-sdk-0.6.9/docs/website/static/img/undraw_mind_map_cwng.svg
+-rw-rw-rw-   0 root         (0) root         (0)    32999 2022-09-02 11:29:49.000000 soil-sdk-0.6.9/docs/website/static/img/undraw_monitor.svg
+-rw-rw-rw-   0 root         (0) root         (0)    15536 2022-09-02 11:29:49.000000 soil-sdk-0.6.9/docs/website/static/img/undraw_note_list.svg
+-rw-rw-rw-   0 root         (0) root         (0)    26627 2022-09-02 11:29:49.000000 soil-sdk-0.6.9/docs/website/static/img/undraw_online.svg
+-rw-rw-rw-   0 root         (0) root         (0)    16533 2022-09-02 11:29:49.000000 soil-sdk-0.6.9/docs/website/static/img/undraw_open_source.svg
+-rw-rw-rw-   0 root         (0) root         (0)    36675 2022-09-02 11:29:49.000000 soil-sdk-0.6.9/docs/website/static/img/undraw_operating_system.svg
+-rw-rw-rw-   0 root         (0) root         (0)    24273 2022-09-02 11:29:49.000000 soil-sdk-0.6.9/docs/website/static/img/undraw_react.svg
+-rw-rw-rw-   0 root         (0) root         (0)     9259 2022-09-02 11:29:49.000000 soil-sdk-0.6.9/docs/website/static/img/undraw_server_push_vtms.svg
+-rw-rw-rw-   0 root         (0) root         (0)     9421 2022-09-02 11:29:49.000000 soil-sdk-0.6.9/docs/website/static/img/undraw_tweetstorm.svg
+-rw-rw-rw-   0 root         (0) root         (0)    19900 2022-09-02 11:29:49.000000 soil-sdk-0.6.9/docs/website/static/img/undraw_version_control_9bpv.svg
+-rw-rw-rw-   0 root         (0) root         (0)    29040 2022-09-02 11:29:49.000000 soil-sdk-0.6.9/docs/website/static/img/undraw_youtube_tutorial.svg
+-rw-rw-rw-   0 root         (0) root         (0)      305 2022-09-02 11:29:49.000000 soil-sdk-0.6.9/pydoc-markdown-library.yml
+-rw-rw-rw-   0 root         (0) root         (0)      305 2022-09-02 11:29:49.000000 soil-sdk-0.6.9/pydoc-markdown.yml
+-rw-rw-rw-   0 root         (0) root         (0)      178 2023-03-09 10:25:17.000000 soil-sdk-0.6.9/pyrightconfig.json
+-rw-rw-rw-   0 root         (0) root         (0)     1308 2023-03-22 10:23:33.011042 soil-sdk-0.6.9/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      109 2023-03-10 09:05:11.000000 soil-sdk-0.6.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 10:23:33.003042 soil-sdk-0.6.9/soil/
+-rw-rw-rw-   0 root         (0) root         (0)      657 2023-03-22 10:19:17.000000 soil-sdk-0.6.9/soil/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 10:23:33.003042 soil-sdk-0.6.9/soil/alerts/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-09-02 11:29:49.000000 soil-sdk-0.6.9/soil/alerts/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      349 2022-09-06 12:27:32.000000 soil-sdk-0.6.9/soil/alerts/alerts.py
+-rw-rw-rw-   0 root         (0) root         (0)      618 2023-03-09 10:25:17.000000 soil-sdk-0.6.9/soil/alias.py
+-rw-rw-rw-   0 root         (0) root         (0)    10030 2023-01-23 11:00:18.000000 soil-sdk-0.6.9/soil/api.py
+-rw-rw-rw-   0 root         (0) root         (0)     5103 2022-09-06 12:27:32.000000 soil-sdk-0.6.9/soil/configuration.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 10:23:33.003042 soil-sdk-0.6.9/soil/connectors/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-09-02 11:29:49.000000 soil-sdk-0.6.9/soil/connectors/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1046 2022-09-02 11:29:49.000000 soil-sdk-0.6.9/soil/connectors/elastic_search.py
+-rw-rw-rw-   0 root         (0) root         (0)     2682 2023-03-22 10:19:17.000000 soil-sdk-0.6.9/soil/data.py
+-rw-rw-rw-   0 root         (0) root         (0)     4706 2022-09-02 11:29:49.000000 soil-sdk-0.6.9/soil/data_structure.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 10:23:33.003042 soil-sdk-0.6.9/soil/data_structures/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-09-02 11:29:49.000000 soil-sdk-0.6.9/soil/data_structures/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1794 2022-09-02 11:29:49.000000 soil-sdk-0.6.9/soil/decorator.py
+-rw-rw-rw-   0 root         (0) root         (0)      503 2022-09-02 11:29:49.000000 soil-sdk-0.6.9/soil/dictionary.py
+-rw-rw-rw-   0 root         (0) root         (0)     1922 2022-09-02 11:29:49.000000 soil-sdk-0.6.9/soil/errors.py
+-rw-rw-rw-   0 root         (0) root         (0)     2128 2023-01-24 10:13:27.000000 soil-sdk-0.6.9/soil/finder.py
+-rw-rw-rw-   0 root         (0) root         (0)      146 2022-09-06 12:27:32.000000 soil-sdk-0.6.9/soil/logger.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 10:23:33.003042 soil-sdk-0.6.9/soil/modules/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-09-02 11:29:49.000000 soil-sdk-0.6.9/soil/modules/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3918 2023-03-07 09:55:51.000000 soil-sdk-0.6.9/soil/modulify.py
+-rw-rw-rw-   0 root         (0) root         (0)     3237 2022-09-06 12:27:32.000000 soil-sdk-0.6.9/soil/pipeline.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-09-13 13:06:18.000000 soil-sdk-0.6.9/soil/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 10:23:33.007042 soil-sdk-0.6.9/soil/storage/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-09-02 11:29:49.000000 soil-sdk-0.6.9/soil/storage/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      663 2023-03-09 08:50:35.000000 soil-sdk-0.6.9/soil/storage/base_storage.py
+-rw-rw-rw-   0 root         (0) root         (0)     1095 2022-09-06 12:27:32.000000 soil-sdk-0.6.9/soil/storage/compound_storage.py
+-rw-rw-rw-   0 root         (0) root         (0)     1507 2022-09-02 11:29:49.000000 soil-sdk-0.6.9/soil/storage/elasticsearch.py
+-rw-rw-rw-   0 root         (0) root         (0)     1665 2022-09-02 11:29:49.000000 soil-sdk-0.6.9/soil/storage/object_storage.py
+-rw-rw-rw-   0 root         (0) root         (0)      813 2022-09-02 11:29:49.000000 soil-sdk-0.6.9/soil/task.py
+-rw-rw-rw-   0 root         (0) root         (0)     1540 2023-03-22 10:19:17.000000 soil-sdk-0.6.9/soil/types.py
+-rw-rw-rw-   0 root         (0) root         (0)     2976 2022-09-02 11:29:49.000000 soil-sdk-0.6.9/soil/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 10:23:33.007042 soil-sdk-0.6.9/soil_cli/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-09-02 11:29:49.000000 soil-sdk-0.6.9/soil_cli/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7893 2022-09-06 12:27:32.000000 soil-sdk-0.6.9/soil_cli/soil_cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 10:23:33.007042 soil-sdk-0.6.9/soil_sdk.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1658 2023-03-22 10:23:32.000000 soil-sdk-0.6.9/soil_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    36817 2023-03-22 10:23:32.000000 soil-sdk-0.6.9/soil_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-03-22 10:23:32.000000 soil-sdk-0.6.9/soil_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       48 2023-03-22 10:23:32.000000 soil-sdk-0.6.9/soil_sdk.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-03-22 10:23:32.000000 soil-sdk-0.6.9/soil_sdk.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       46 2023-03-22 10:23:32.000000 soil-sdk-0.6.9/soil_sdk.egg-info/pbr.json
+-rw-r--r--   0 root         (0) root         (0)      216 2023-03-22 10:23:32.000000 soil-sdk-0.6.9/soil_sdk.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2023-03-22 10:23:32.000000 soil-sdk-0.6.9/soil_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 10:23:33.007042 soil-sdk-0.6.9/test/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-09-02 11:29:49.000000 soil-sdk-0.6.9/test/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 10:23:33.007042 soil-sdk-0.6.9/test/unit/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-09-02 11:29:49.000000 soil-sdk-0.6.9/test/unit/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 10:23:33.007042 soil-sdk-0.6.9/test/unit/soil/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-09-02 11:29:49.000000 soil-sdk-0.6.9/test/unit/soil/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1514 2022-09-06 12:27:32.000000 soil-sdk-0.6.9/test/unit/soil/test_alerts.py
+-rw-rw-rw-   0 root         (0) root         (0)    12383 2023-03-09 10:25:17.000000 soil-sdk-0.6.9/test/unit/soil/test_alias.py
+-rw-rw-rw-   0 root         (0) root         (0)    10457 2023-03-09 09:42:09.000000 soil-sdk-0.6.9/test/unit/soil/test_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     2629 2022-09-02 11:29:49.000000 soil-sdk-0.6.9/test/unit/soil/test_decorator.py
+-rw-rw-rw-   0 root         (0) root         (0)     3606 2022-09-06 12:27:32.000000 soil-sdk-0.6.9/test/unit/soil/test_dictionary.py
+-rw-rw-rw-   0 root         (0) root         (0)     2587 2023-01-24 10:13:27.000000 soil-sdk-0.6.9/test/unit/soil/test_finder.py
+-rw-rw-rw-   0 root         (0) root         (0)    11400 2023-02-16 12:38:32.000000 soil-sdk-0.6.9/test/unit/soil/test_pipelines.py
+-rw-rw-rw-   0 root         (0) root         (0)      510 2022-09-06 12:27:32.000000 soil-sdk-0.6.9/test/unit/soil/test_task.py
+-rw-rw-rw-   0 root         (0) root         (0)    34958 2022-09-06 12:27:32.000000 soil-sdk-0.6.9/test/unit/soil/test_utils.py
```

### Comparing `soil-sdk-0.6.8.dev2/.gitlab-ci.yml` & `soil-sdk-0.6.9/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/.pre-commit-config.yaml` & `soil-sdk-0.6.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/.vscode/settings.json` & `soil-sdk-0.6.9/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/ChangeLog` & `soil-sdk-0.6.9/ChangeLog`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,18 @@
 CHANGES
 =======
 
+0.6.9
+-----
+
+* exported soil types and serializableDS protocol solved
+
+0.6.8
+-----
+
 * Added artifact to CI
 * updated readme
 
 0.6.7
 -----
 
 * typeddict as generic
@@ -150,8 +158,7 @@
 
 * Do not upload modules in test environment
 
 0.3.7
 -----
 
 * Updated documentation
-* Added compound storage
```

### Comparing `soil-sdk-0.6.8.dev2/PKG-INFO` & `soil-sdk-0.6.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: soil-sdk
-Version: 0.6.8.dev2
+Version: 0.6.9
 Summary: SOIL Software Development Kit
 Home-page: https://developer.amalfianalytics.com/
 Author: Amalfi Analytics
 Author-email: info@amalfianalytics.com
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown; charset=UTF-8
 Provides-Extra: dev
```

### Comparing `soil-sdk-0.6.8.dev2/README.md` & `soil-sdk-0.6.9/README.md`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/docs/assets/example-app-dir.png` & `soil-sdk-0.6.9/docs/docs/assets/example-app-dir.png`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/docs/sdk-reference/sidebar.json` & `soil-sdk-0.6.9/docs/docs/sdk-reference/sidebar.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/docs/sdk-reference/soil/api.md` & `soil-sdk-0.6.9/docs/docs/sdk-reference/soil/api.md`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/docs/sdk-reference/soil/configuration.md` & `soil-sdk-0.6.9/docs/docs/sdk-reference/soil/configuration.md`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/docs/sdk-reference/soil/connectors/elastic_search.md` & `soil-sdk-0.6.9/docs/docs/sdk-reference/soil/connectors/elastic_search.md`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/docs/sdk-reference/soil/data_structure.md` & `soil-sdk-0.6.9/docs/docs/sdk-reference/soil/data_structure.md`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/docs/sdk-reference/soil/decorator.md` & `soil-sdk-0.6.9/docs/docs/sdk-reference/soil/decorator.md`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/docs/sdk-reference/soil/errors.md` & `soil-sdk-0.6.9/docs/docs/sdk-reference/soil/errors.md`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/docs/sdk-reference/soil/finder.md` & `soil-sdk-0.6.9/docs/docs/sdk-reference/soil/finder.md`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/docs/sdk-reference/soil/modulify.md` & `soil-sdk-0.6.9/docs/docs/sdk-reference/soil/modulify.md`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/docs/sdk-reference/soil/pipeline.md` & `soil-sdk-0.6.9/docs/docs/sdk-reference/soil/pipeline.md`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/docs/sdk-reference/soil/storage/base_storage.md` & `soil-sdk-0.6.9/docs/docs/sdk-reference/soil/storage/base_storage.md`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/docs/sdk-reference/soil/storage/compound_storage.md` & `soil-sdk-0.6.9/docs/docs/sdk-reference/soil/storage/compound_storage.md`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/docs/sdk-reference/soil/storage/elasticsearch.md` & `soil-sdk-0.6.9/docs/docs/sdk-reference/soil/storage/elasticsearch.md`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/docs/sdk-reference/soil/storage/object_storage.md` & `soil-sdk-0.6.9/docs/docs/sdk-reference/soil/storage/object_storage.md`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/docs/sdk-reference/soil/task.md` & `soil-sdk-0.6.9/docs/docs/sdk-reference/soil/task.md`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/docs/sdk-reference/soil/utils.md` & `soil-sdk-0.6.9/docs/docs/sdk-reference/soil/utils.md`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/docs/soil-library/data_structures/data_structure.md` & `soil-sdk-0.6.9/docs/docs/soil-library/data_structures/data_structure.md`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/docs/soil-library/data_structures/hypergraph.md` & `soil-sdk-0.6.9/docs/docs/soil-library/data_structures/hypergraph.md`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/docs/soil-library/data_structures/streams/patients.md` & `soil-sdk-0.6.9/docs/docs/soil-library/data_structures/streams/patients.md`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/docs/soil-library/modules/clustering/NBClustering.md` & `soil-sdk-0.6.9/docs/docs/soil-library/modules/clustering/NBClustering.md`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/docs/soil-library/modules/clustering/NBClustering_categorical.md` & `soil-sdk-0.6.9/docs/docs/soil-library/modules/clustering/NBClustering_categorical.md`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/docs/soil-library/modules/clustering/SIDIWO/sidiwo.md` & `soil-sdk-0.6.9/docs/docs/soil-library/modules/clustering/SIDIWO/sidiwo.md`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/docs/soil-library/modules/higher_order/Predictor.md` & `soil-sdk-0.6.9/docs/docs/soil-library/modules/higher_order/Predictor.md`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/docs/soil-library/modules/preprocessing/filters/row_filter.md` & `soil-sdk-0.6.9/docs/docs/soil-library/modules/preprocessing/filters/row_filter.md`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/docs/soil-library/modules/temporal/trajectories.md` & `soil-sdk-0.6.9/docs/docs/soil-library/modules/temporal/trajectories.md`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/docs/soil-library/sidebar.json` & `soil-sdk-0.6.9/docs/docs/soil-library/sidebar.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/docs/tutorial/alerts.md` & `soil-sdk-0.6.9/docs/docs/tutorial/alerts.md`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/docs/tutorial/data-structures.md` & `soil-sdk-0.6.9/docs/docs/tutorial/data-structures.md`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/docs/tutorial/data.md` & `soil-sdk-0.6.9/docs/docs/tutorial/data.md`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/docs/tutorial/deployments.md` & `soil-sdk-0.6.9/docs/docs/tutorial/deployments.md`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/docs/tutorial/get-started.mdx` & `soil-sdk-0.6.9/docs/docs/tutorial/get-started.mdx`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/docs/tutorial/logging.md` & `soil-sdk-0.6.9/docs/docs/tutorial/logging.md`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/docs/tutorial/modules.md` & `soil-sdk-0.6.9/docs/docs/tutorial/modules.md`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/docs/tutorial/notebooks.md` & `soil-sdk-0.6.9/docs/docs/tutorial/notebooks.md`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/docs/tutorial/scripts.md` & `soil-sdk-0.6.9/docs/docs/tutorial/scripts.md`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/client-manifest.json` & `soil-sdk-0.6.9/docs/website/.docusaurus/client-manifest.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/client-modules.js` & `soil-sdk-0.6.9/docs/website/.docusaurus/client-modules.js`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-blog/default/blog-archive-80c.json` & `soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-blog/default/blog-archive-80c.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-blog/default/blog-post-list-prop-default.json` & `soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-blog/default/blog-post-list-prop-default.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-blog/default/site-blog-2016-03-11-blog-post-md-bf9.json` & `soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-blog/default/site-blog-2016-03-11-blog-post-md-bf9.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-blog/default/site-blog-2017-04-10-blog-post-two-md-dfa.json` & `soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-blog/default/site-blog-2017-04-10-blog-post-two-md-dfa.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-blog/default/site-blog-2017-09-25-testing-rss-md-4d8.json` & `soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-blog/default/site-blog-2017-09-25-testing-rss-md-4d8.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-blog/default/site-blog-2017-09-26-adding-rss-md-ad7.json` & `soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-blog/default/site-blog-2017-09-26-adding-rss-md-ad7.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-blog/default/site-blog-2017-10-24-new-version-1-0-0-md-bbb.json` & `soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-blog/default/site-blog-2017-10-24-new-version-1-0-0-md-bbb.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-docs-sdk-reference-soil-alias-md-698.json` & `soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-docs-sdk-reference-soil-alias-md-698.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-docs-sdk-reference-soil-api-md-fbe.json` & `soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-docs-sdk-reference-soil-api-md-fbe.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-docs-sdk-reference-soil-cli-soil-cli-md-727.json` & `soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-docs-sdk-reference-soil-cli-soil-cli-md-727.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-docs-sdk-reference-soil-configuration-md-707.json` & `soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-docs-sdk-reference-soil-configuration-md-707.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-docs-sdk-reference-soil-connectors-elastic-search-md-eca.json` & `soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-docs-sdk-reference-soil-connectors-elastic-search-md-eca.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-docs-sdk-reference-soil-data-md-d6b.json` & `soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-docs-sdk-reference-soil-data-md-d6b.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-docs-sdk-reference-soil-data-structure-md-e8d.json` & `soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-docs-sdk-reference-soil-data-structure-md-e8d.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-docs-sdk-reference-soil-finder-md-60a.json` & `soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-docs-sdk-reference-soil-finder-md-60a.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-docs-sdk-reference-soil-modulify-md-0c9.json` & `soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-docs-sdk-reference-soil-modulify-md-0c9.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-docs-sdk-reference-soil-pipeline-md-312.json` & `soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-docs-sdk-reference-soil-pipeline-md-312.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-docs-sdk-reference-soil-types-md-24f.json` & `soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-docs-sdk-reference-soil-types-md-24f.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-sdk-reference-sdk-reference-md-a6b.json` & `soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-sdk-reference-sdk-reference-md-a6b.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-sdk-reference-soil-alerts-alerts-md-231.json` & `soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-sdk-reference-soil-alerts-alerts-md-231.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-sdk-reference-soil-alias-md-2bb.json` & `soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-sdk-reference-soil-alias-md-2bb.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-sdk-reference-soil-api-md-cf6.json` & `soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-sdk-reference-soil-api-md-cf6.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-sdk-reference-soil-cli-soil-cli-md-c6c.json` & `soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-sdk-reference-soil-cli-soil-cli-md-c6c.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-sdk-reference-soil-configuration-md-b6d.json` & `soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-sdk-reference-soil-configuration-md-b6d.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-sdk-reference-soil-connectors-elastic-search-md-8f4.json` & `soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-sdk-reference-soil-connectors-elastic-search-md-8f4.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-sdk-reference-soil-data-md-d6c.json` & `soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-sdk-reference-soil-data-md-d6c.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-sdk-reference-soil-data-structure-md-3d5.json` & `soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-sdk-reference-soil-data-structure-md-3d5.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-sdk-reference-soil-decorator-md-6e4.json` & `soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-sdk-reference-soil-decorator-md-6e4.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-sdk-reference-soil-dictionary-md-7b7.json` & `soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-sdk-reference-soil-dictionary-md-7b7.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-sdk-reference-soil-errors-md-4c9.json` & `soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-sdk-reference-soil-errors-md-4c9.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-sdk-reference-soil-finder-md-839.json` & `soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-sdk-reference-soil-finder-md-839.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-sdk-reference-soil-modulify-md-37b.json` & `soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-sdk-reference-soil-modulify-md-37b.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-sdk-reference-soil-pipeline-md-5a1.json` & `soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-sdk-reference-soil-pipeline-md-5a1.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-sdk-reference-soil-storage-base-storage-md-4fa.json` & `soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-sdk-reference-soil-storage-base-storage-md-4fa.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-sdk-reference-soil-storage-compound-storage-md-96f.json` & `soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-sdk-reference-soil-storage-compound-storage-md-96f.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-sdk-reference-soil-storage-elasticsearch-md-f3d.json` & `soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-sdk-reference-soil-storage-elasticsearch-md-f3d.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-sdk-reference-soil-storage-object-storage-md-ce3.json` & `soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-sdk-reference-soil-storage-object-storage-md-ce3.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-sdk-reference-soil-task-md-a67.json` & `soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-sdk-reference-soil-task-md-a67.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-sdk-reference-soil-types-md-3ef.json` & `soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-sdk-reference-soil-types-md-3ef.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-sdk-reference-soil-utils-md-092.json` & `soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-sdk-reference-soil-utils-md-092.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-data-structures-data-structure-md-1fb.json` & `soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-data-structures-data-structure-md-1fb.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-data-structures-frequent-itemsets-md-3bb.json` & `soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-data-structures-frequent-itemsets-md-3bb.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-data-structures-hypergraph-md-c0e.json` & `soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-data-structures-hypergraph-md-c0e.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-data-structures-init-md-de6.json` & `soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-data-structures-init-md-de6.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-data-structures-model-md-0ad.json` & `soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-data-structures-model-md-0ad.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-data-structures-nb-clusters-categorical-md-046.json` & `soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-data-structures-nb-clusters-categorical-md-046.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-data-structures-nb-clusters-md-7ed.json` & `soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-data-structures-nb-clusters-md-7ed.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-data-structures-paginated-list-md-973.json` & `soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-data-structures-paginated-list-md-973.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-data-structures-predefined-dict-md-379.json` & `soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-data-structures-predefined-dict-md-379.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-data-structures-predefined-init-md-575.json` & `soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-data-structures-predefined-init-md-575.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-data-structures-predefined-list-md-5ee.json` & `soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-data-structures-predefined-list-md-5ee.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-data-structures-predefined-ndarray-md-7db.json` & `soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-data-structures-predefined-ndarray-md-7db.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-data-structures-predefined-object-ds-md-f15.json` & `soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-data-structures-predefined-object-ds-md-f15.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-data-structures-predefined-pd-data-frame-md-a71.json` & `soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-data-structures-predefined-pd-data-frame-md-a71.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-data-structures-statistics-md-07b.json` & `soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-data-structures-statistics-md-07b.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-data-structures-streams-association-rules-md-820.json` & `soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-data-structures-streams-association-rules-md-820.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-data-structures-streams-init-md-d9b.json` & `soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-data-structures-streams-init-md-d9b.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-data-structures-streams-patients-md-60e.json` & `soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-data-structures-streams-patients-md-60e.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-data-structures-streams-stream-md-317.json` & `soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-data-structures-streams-stream-md-317.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-data-structures-streams-trajectory-clusters-md-1d9.json` & `soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-data-structures-streams-trajectory-clusters-md-1d9.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-data-structures-time-statistics-md-fcd.json` & `soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-data-structures-time-statistics-md-fcd.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-data-structures-trajectories-md-899.json` & `soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-data-structures-trajectories-md-899.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-ehra-data-structures-hypergraph-md-084.json` & `soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-ehra-data-structures-hypergraph-md-084.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-ehra-data-structures-streams-patients-md-ced.json` & `soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-ehra-data-structures-streams-patients-md-ced.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-ehra-data-structures-streams-trajectory-clusters-md-7cf.json` & `soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-ehra-data-structures-streams-trajectory-clusters-md-7cf.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-ehra-modules-clustering-nb-clustering-categorical-md-300.json` & `soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-ehra-modules-clustering-nb-clustering-categorical-md-300.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-ehra-modules-clustering-nb-clustering-md-11b.json` & `soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-ehra-modules-clustering-nb-clustering-md-11b.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-ehra-modules-clustering-sidiwo-sidiwo-md-266.json` & `soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-ehra-modules-clustering-sidiwo-sidiwo-md-266.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-ehra-modules-experiment-md-047.json` & `soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-ehra-modules-experiment-md-047.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-ehra-modules-higher-order-predictor-md-414.json` & `soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-ehra-modules-higher-order-predictor-md-414.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-ehra-modules-itemsets-frequent-itemsets-compare-md-6e5.json` & `soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-ehra-modules-itemsets-frequent-itemsets-compare-md-6e5.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-ehra-modules-itemsets-frequent-itemsets-hypergraph-md-d85.json` & `soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-ehra-modules-itemsets-frequent-itemsets-hypergraph-md-d85.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-ehra-modules-preprocessing-filters-events-filter-md-2cf.json` & `soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-ehra-modules-preprocessing-filters-events-filter-md-2cf.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-ehra-modules-preprocessing-filters-row-filter-md-b96.json` & `soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-ehra-modules-preprocessing-filters-row-filter-md-b96.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-ehra-modules-statistics-customstatistics-md-353.json` & `soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-ehra-modules-statistics-customstatistics-md-353.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-ehra-modules-statistics-time-statistics-md-7fa.json` & `soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-ehra-modules-statistics-time-statistics-md-7fa.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-ehra-modules-temporal-trajectories-md-419.json` & `soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-ehra-modules-temporal-trajectories-md-419.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-modules-clustering-init-md-349.json` & `soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-modules-clustering-init-md-349.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-modules-clustering-nb-clustering-categorical-md-0c4.json` & `soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-modules-clustering-nb-clustering-categorical-md-0c4.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-modules-clustering-nb-clustering-md-19d.json` & `soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-modules-clustering-nb-clustering-md-19d.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-modules-clustering-sidiwo-init-md-729.json` & `soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-modules-clustering-sidiwo-init-md-729.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-modules-clustering-sidiwo-sidiwo-md-478.json` & `soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-modules-clustering-sidiwo-sidiwo-md-478.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-modules-experiment-md-a5e.json` & `soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-modules-experiment-md-a5e.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-modules-higher-order-init-md-c2b.json` & `soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-modules-higher-order-init-md-c2b.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-modules-higher-order-predictor-md-b65.json` & `soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-modules-higher-order-predictor-md-b65.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-modules-init-md-f13.json` & `soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-modules-init-md-f13.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-modules-itemsets-association-rules-md-8b6.json` & `soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-modules-itemsets-association-rules-md-8b6.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-modules-itemsets-frequent-itemsets-compare-md-49b.json` & `soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-modules-itemsets-frequent-itemsets-compare-md-49b.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-modules-itemsets-frequent-itemsets-hypergraph-md-0d1.json` & `soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-modules-itemsets-frequent-itemsets-hypergraph-md-0d1.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-modules-itemsets-frequent-itemsets-md-ca7.json` & `soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-modules-itemsets-frequent-itemsets-md-ca7.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-modules-itemsets-init-md-a1a.json` & `soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-modules-itemsets-init-md-a1a.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-modules-preprocessing-filters-column-filter-md-04c.json` & `soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-modules-preprocessing-filters-column-filter-md-04c.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-modules-preprocessing-filters-events-filter-md-59c.json` & `soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-modules-preprocessing-filters-events-filter-md-59c.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-modules-preprocessing-filters-flattener-md-1a6.json` & `soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-modules-preprocessing-filters-flattener-md-1a6.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-modules-preprocessing-filters-init-md-728.json` & `soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-modules-preprocessing-filters-init-md-728.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-modules-preprocessing-filters-row-filter-md-77e.json` & `soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-modules-preprocessing-filters-row-filter-md-77e.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-modules-preprocessing-init-md-8d4.json` & `soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-modules-preprocessing-init-md-8d4.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-modules-preprocessing-pipe-md-fd6.json` & `soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-modules-preprocessing-pipe-md-fd6.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-modules-preprocessing-sampling-init-md-dba.json` & `soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-modules-preprocessing-sampling-init-md-dba.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-modules-preprocessing-sampling-reservoir-sampling-md-cfe.json` & `soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-modules-preprocessing-sampling-reservoir-sampling-md-cfe.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-modules-statistics-customstatistics-md-3e3.json` & `soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-modules-statistics-customstatistics-md-3e3.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-modules-statistics-init-md-135.json` & `soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-modules-statistics-init-md-135.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-modules-statistics-statistics-md-0db.json` & `soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-modules-statistics-statistics-md-0db.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-modules-statistics-time-statistics-md-92c.json` & `soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-modules-statistics-time-statistics-md-92c.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-modules-temporal-init-md-37a.json` & `soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-modules-temporal-init-md-37a.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-modules-temporal-trajectories-md-285.json` & `soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-modules-temporal-trajectories-md-285.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-soil-library-md-65d.json` & `soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-soil-library-soil-library-md-65d.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-tutorial-alerts-md-43b.json` & `soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-tutorial-alerts-md-43b.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-tutorial-data-md-0d2.json` & `soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-tutorial-data-md-0d2.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-tutorial-data-structures-md-14d.json` & `soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-tutorial-data-structures-md-14d.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-tutorial-deployments-md-62e.json` & `soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-tutorial-deployments-md-62e.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-tutorial-get-started-md-d5b.json` & `soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-tutorial-get-started-md-d5b.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-tutorial-get-started-mdx-36a.json` & `soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-tutorial-get-started-mdx-36a.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-tutorial-logging-md-507.json` & `soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-tutorial-logging-md-507.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-tutorial-modules-md-cd8.json` & `soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-tutorial-modules-md-cd8.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-tutorial-notebooks-md-58b.json` & `soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-tutorial-notebooks-md-58b.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-tutorial-scripts-md-0f5.json` & `soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-docs-tutorial-scripts-md-0f5.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-1-sdk-reference-sdk-reference-md-59f.json` & `soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-1-sdk-reference-sdk-reference-md-59f.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-1-soil-library-soil-library-md-ce1.json` & `soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-1-soil-library-soil-library-md-ce1.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-1-tutorial-data-md-e4a.json` & `soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-1-tutorial-data-md-e4a.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-1-tutorial-data-structures-md-53e.json` & `soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-1-tutorial-data-structures-md-53e.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-1-tutorial-get-started-md-cbe.json` & `soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-1-tutorial-get-started-md-cbe.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-1-tutorial-logging-md-4a1.json` & `soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-1-tutorial-logging-md-4a1.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-1-tutorial-modules-md-547.json` & `soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-1-tutorial-modules-md-547.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-1-tutorial-scripts-md-a17.json` & `soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-1-tutorial-scripts-md-a17.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-2-sdk-reference-sdk-reference-md-62b.json` & `soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-2-sdk-reference-sdk-reference-md-62b.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-2-soil-library-soil-library-md-1c7.json` & `soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-2-soil-library-soil-library-md-1c7.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-2-tutorial-data-md-278.json` & `soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-2-tutorial-data-md-278.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-2-tutorial-data-structures-md-89f.json` & `soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-2-tutorial-data-structures-md-89f.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-2-tutorial-get-started-md-022.json` & `soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-2-tutorial-get-started-md-022.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-2-tutorial-logging-md-4c2.json` & `soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-2-tutorial-logging-md-4c2.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-2-tutorial-modules-md-cdc.json` & `soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-2-tutorial-modules-md-cdc.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-2-tutorial-scripts-md-d50.json` & `soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-2-tutorial-scripts-md-d50.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-3-sdk-reference-sdk-reference-md-75e.json` & `soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-3-sdk-reference-sdk-reference-md-75e.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-3-soil-library-soil-library-md-aaf.json` & `soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-3-soil-library-soil-library-md-aaf.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-3-tutorial-data-md-bc1.json` & `soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-3-tutorial-data-md-bc1.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-3-tutorial-data-structures-md-805.json` & `soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-3-tutorial-data-structures-md-805.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-3-tutorial-get-started-md-9c5.json` & `soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-3-tutorial-get-started-md-9c5.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-3-tutorial-logging-md-0a4.json` & `soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-3-tutorial-logging-md-0a4.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-3-tutorial-modules-md-c8e.json` & `soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-3-tutorial-modules-md-c8e.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-3-tutorial-scripts-md-dbf.json` & `soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-3-tutorial-scripts-md-dbf.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-4-sdk-reference-sdk-reference-md-343.json` & `soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-4-sdk-reference-sdk-reference-md-343.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-4-soil-library-soil-library-md-b38.json` & `soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-4-soil-library-soil-library-md-b38.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-4-tutorial-data-md-8d7.json` & `soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-4-tutorial-data-md-8d7.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-4-tutorial-data-structures-md-b95.json` & `soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-4-tutorial-data-structures-md-b95.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-4-tutorial-get-started-md-c2c.json` & `soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-4-tutorial-get-started-md-c2c.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-4-tutorial-logging-md-750.json` & `soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-4-tutorial-logging-md-750.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-4-tutorial-modules-md-447.json` & `soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-4-tutorial-modules-md-447.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-4-tutorial-scripts-md-904.json` & `soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-4-tutorial-scripts-md-904.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-5-sdk-reference-sdk-reference-md-c6e.json` & `soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-5-sdk-reference-sdk-reference-md-c6e.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-5-soil-library-soil-library-md-f09.json` & `soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-5-soil-library-soil-library-md-f09.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-5-tutorial-data-md-ae6.json` & `soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-5-tutorial-data-md-ae6.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-5-tutorial-data-structures-md-d2f.json` & `soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-5-tutorial-data-structures-md-d2f.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-5-tutorial-get-started-md-392.json` & `soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-5-tutorial-get-started-md-392.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-5-tutorial-logging-md-645.json` & `soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-5-tutorial-logging-md-645.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-5-tutorial-modules-md-3bc.json` & `soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-5-tutorial-modules-md-3bc.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-5-tutorial-scripts-md-bd1.json` & `soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-5-tutorial-scripts-md-bd1.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-6-sdk-reference-sdk-reference-md-073.json` & `soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-6-sdk-reference-sdk-reference-md-073.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-6-soil-library-soil-library-md-53e.json` & `soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-6-soil-library-soil-library-md-53e.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-6-tutorial-data-md-cba.json` & `soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-6-tutorial-data-md-cba.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-6-tutorial-data-structures-md-c96.json` & `soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-6-tutorial-data-structures-md-c96.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-6-tutorial-get-started-md-6a0.json` & `soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-6-tutorial-get-started-md-6a0.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-6-tutorial-logging-md-7c2.json` & `soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-6-tutorial-logging-md-7c2.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-6-tutorial-modules-md-dd3.json` & `soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-6-tutorial-modules-md-dd3.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-6-tutorial-scripts-md-e55.json` & `soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-6-tutorial-scripts-md-e55.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-7-sdk-reference-sdk-reference-md-5bd.json` & `soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-7-sdk-reference-sdk-reference-md-5bd.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-7-soil-library-soil-library-md-b02.json` & `soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-7-soil-library-soil-library-md-b02.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-7-tutorial-data-md-345.json` & `soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-7-tutorial-data-md-345.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-7-tutorial-data-structures-md-b1a.json` & `soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-7-tutorial-data-structures-md-b1a.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-7-tutorial-get-started-md-661.json` & `soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-7-tutorial-get-started-md-661.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-7-tutorial-logging-md-aae.json` & `soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-7-tutorial-logging-md-aae.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-7-tutorial-modules-md-9f2.json` & `soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-7-tutorial-modules-md-9f2.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-7-tutorial-scripts-md-21c.json` & `soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-7-tutorial-scripts-md-21c.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-8-sdk-reference-sdk-reference-md-670.json` & `soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-8-sdk-reference-sdk-reference-md-670.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-8-soil-library-soil-library-md-3b4.json` & `soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-8-soil-library-soil-library-md-3b4.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-8-tutorial-data-md-e4f.json` & `soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-8-tutorial-data-md-e4f.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-8-tutorial-data-structures-md-04f.json` & `soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-8-tutorial-data-structures-md-04f.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-8-tutorial-get-started-md-610.json` & `soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-8-tutorial-get-started-md-610.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-8-tutorial-logging-md-0d8.json` & `soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-8-tutorial-logging-md-0d8.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-8-tutorial-modules-md-a2c.json` & `soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-8-tutorial-modules-md-a2c.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-8-tutorial-scripts-md-700.json` & `soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-0-8-tutorial-scripts-md-700.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-1-0-sdk-reference-sdk-reference-md-172.json` & `soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-1-0-sdk-reference-sdk-reference-md-172.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-1-0-soil-library-soil-library-md-963.json` & `soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-1-0-soil-library-soil-library-md-963.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-1-0-tutorial-data-md-eac.json` & `soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-1-0-tutorial-data-md-eac.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-1-0-tutorial-data-structures-md-f2b.json` & `soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-1-0-tutorial-data-structures-md-f2b.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-1-0-tutorial-get-started-md-526.json` & `soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-1-0-tutorial-get-started-md-526.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-1-0-tutorial-get-started-mdx-539.json` & `soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-1-0-tutorial-get-started-mdx-539.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-1-0-tutorial-logging-md-3a5.json` & `soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-1-0-tutorial-logging-md-3a5.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-1-0-tutorial-modules-md-1ad.json` & `soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-1-0-tutorial-modules-md-1ad.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-1-0-tutorial-scripts-md-caa.json` & `soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-1-0-tutorial-scripts-md-caa.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-1-1-sdk-reference-soil-alias-md-6d0.json` & `soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-1-1-sdk-reference-soil-alias-md-6d0.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-1-1-sdk-reference-soil-api-md-056.json` & `soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-1-1-sdk-reference-soil-api-md-056.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-1-1-sdk-reference-soil-configuration-md-7c5.json` & `soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-1-1-sdk-reference-soil-configuration-md-7c5.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-1-1-sdk-reference-soil-connectors-elastic-search-md-b85.json` & `soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-1-1-sdk-reference-soil-connectors-elastic-search-md-b85.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-1-1-sdk-reference-soil-data-md-797.json` & `soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-1-1-sdk-reference-soil-data-md-797.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-1-1-sdk-reference-soil-data-structure-md-916.json` & `soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-1-1-sdk-reference-soil-data-structure-md-916.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-1-1-sdk-reference-soil-finder-md-c72.json` & `soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-1-1-sdk-reference-soil-finder-md-c72.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-1-1-sdk-reference-soil-modulify-md-b9a.json` & `soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-1-1-sdk-reference-soil-modulify-md-b9a.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-1-1-sdk-reference-soil-pipeline-md-6eb.json` & `soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-1-1-sdk-reference-soil-pipeline-md-6eb.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-1-1-sdk-reference-soil-types-md-00c.json` & `soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-1-1-sdk-reference-soil-types-md-00c.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-1-1-soil-library-soil-library-md-2b7.json` & `soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-1-1-soil-library-soil-library-md-2b7.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-1-1-tutorial-data-md-b95.json` & `soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-1-1-tutorial-data-md-b95.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-1-1-tutorial-data-structures-md-03c.json` & `soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-1-1-tutorial-data-structures-md-03c.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-1-1-tutorial-get-started-mdx-cf0.json` & `soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-1-1-tutorial-get-started-mdx-cf0.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-1-1-tutorial-logging-md-bb1.json` & `soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-1-1-tutorial-logging-md-bb1.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-1-1-tutorial-modules-md-4b3.json` & `soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-1-1-tutorial-modules-md-4b3.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-1-1-tutorial-scripts-md-7f6.json` & `soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-1-1-tutorial-scripts-md-7f6.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-1-2-sdk-reference-soil-alias-md-165.json` & `soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-1-2-sdk-reference-soil-alias-md-165.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-1-2-sdk-reference-soil-api-md-f09.json` & `soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-1-2-sdk-reference-soil-api-md-f09.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-1-2-sdk-reference-soil-configuration-md-4f6.json` & `soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-1-2-sdk-reference-soil-configuration-md-4f6.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-1-2-sdk-reference-soil-connectors-elastic-search-md-224.json` & `soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-1-2-sdk-reference-soil-connectors-elastic-search-md-224.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-1-2-sdk-reference-soil-data-md-cd7.json` & `soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-1-2-sdk-reference-soil-data-md-cd7.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-1-2-sdk-reference-soil-data-structure-md-849.json` & `soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-1-2-sdk-reference-soil-data-structure-md-849.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-1-2-sdk-reference-soil-finder-md-da9.json` & `soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-1-2-sdk-reference-soil-finder-md-da9.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-1-2-sdk-reference-soil-modulify-md-47e.json` & `soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-1-2-sdk-reference-soil-modulify-md-47e.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-1-2-sdk-reference-soil-pipeline-md-945.json` & `soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-1-2-sdk-reference-soil-pipeline-md-945.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-1-2-sdk-reference-soil-types-md-b0e.json` & `soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-1-2-sdk-reference-soil-types-md-b0e.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-1-2-soil-library-soil-library-md-04e.json` & `soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-1-2-soil-library-soil-library-md-04e.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-1-2-tutorial-data-md-0e1.json` & `soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-1-2-tutorial-data-md-0e1.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-1-2-tutorial-data-structures-md-ad9.json` & `soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-1-2-tutorial-data-structures-md-ad9.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-1-2-tutorial-get-started-mdx-7f5.json` & `soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-1-2-tutorial-get-started-mdx-7f5.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-1-2-tutorial-logging-md-cb9.json` & `soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-1-2-tutorial-logging-md-cb9.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-1-2-tutorial-modules-md-ad2.json` & `soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-1-2-tutorial-modules-md-ad2.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-1-2-tutorial-scripts-md-aef.json` & `soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/site-versioned-docs-version-0-1-2-tutorial-scripts-md-aef.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/version-0-0-1-metadata-prop-e31.json` & `soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/version-0-0-1-metadata-prop-e31.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/version-0-0-2-metadata-prop-b4f.json` & `soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/version-0-0-2-metadata-prop-b4f.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/version-0-0-3-metadata-prop-272.json` & `soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/version-0-0-3-metadata-prop-272.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/version-0-0-4-metadata-prop-937.json` & `soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/version-0-0-4-metadata-prop-937.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/version-0-0-5-metadata-prop-e97.json` & `soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/version-0-0-5-metadata-prop-e97.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/version-0-0-6-metadata-prop-46a.json` & `soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/version-0-0-6-metadata-prop-46a.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/version-0-0-7-metadata-prop-558.json` & `soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/version-0-0-7-metadata-prop-558.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/version-0-0-8-metadata-prop-5dc.json` & `soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/version-0-0-8-metadata-prop-5dc.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/version-current-metadata-prop-751.json` & `soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-content-docs/default/version-current-metadata-prop-751.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus-plugin-debug/default/docusaurus-debug-all-content-673.json` & `soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus-plugin-debug/default/docusaurus-debug-all-content-673.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus.config.js` & `soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus.config.js`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/docusaurus.config.mjs` & `soil-sdk-0.6.9/docs/website/.docusaurus/docusaurus.config.mjs`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/globalData.json` & `soil-sdk-0.6.9/docs/website/.docusaurus/globalData.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/registry.js` & `soil-sdk-0.6.9/docs/website/.docusaurus/registry.js`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/routes.js` & `soil-sdk-0.6.9/docs/website/.docusaurus/routes.js`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/routesChunkNames.json` & `soil-sdk-0.6.9/docs/website/.docusaurus/routesChunkNames.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/.docusaurus/site-metadata.json` & `soil-sdk-0.6.9/docs/website/.docusaurus/site-metadata.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/blog/2016-03-11-blog-post.md` & `soil-sdk-0.6.9/docs/website/blog/2016-03-11-blog-post.md`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/blog/2017-04-10-blog-post-two.md` & `soil-sdk-0.6.9/docs/website/blog/2017-04-10-blog-post-two.md`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/docusaurus.config.js` & `soil-sdk-0.6.9/docs/website/docusaurus.config.js`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/package.json` & `soil-sdk-0.6.9/docs/website/package.json`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/src/pages/index.js` & `soil-sdk-0.6.9/docs/website/src/pages/index.js`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/static/img/favicon.ico` & `soil-sdk-0.6.9/docs/website/static/img/favicon.ico`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/static/img/favicon_amalfi.png` & `soil-sdk-0.6.9/docs/website/static/img/favicon_amalfi.png`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/static/img/oss_logo.png` & `soil-sdk-0.6.9/docs/website/static/img/oss_logo.png`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/static/img/undraw_abstract_x68e.svg` & `soil-sdk-0.6.9/docs/website/static/img/undraw_abstract_x68e.svg`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/static/img/undraw_code_review.svg` & `soil-sdk-0.6.9/docs/website/static/img/undraw_code_review.svg`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/static/img/undraw_mind_map_cwng.svg` & `soil-sdk-0.6.9/docs/website/static/img/undraw_mind_map_cwng.svg`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/static/img/undraw_monitor.svg` & `soil-sdk-0.6.9/docs/website/static/img/undraw_monitor.svg`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/static/img/undraw_note_list.svg` & `soil-sdk-0.6.9/docs/website/static/img/undraw_note_list.svg`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/static/img/undraw_online.svg` & `soil-sdk-0.6.9/docs/website/static/img/undraw_online.svg`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/static/img/undraw_open_source.svg` & `soil-sdk-0.6.9/docs/website/static/img/undraw_open_source.svg`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/static/img/undraw_operating_system.svg` & `soil-sdk-0.6.9/docs/website/static/img/undraw_operating_system.svg`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/static/img/undraw_react.svg` & `soil-sdk-0.6.9/docs/website/static/img/undraw_react.svg`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/static/img/undraw_server_push_vtms.svg` & `soil-sdk-0.6.9/docs/website/static/img/undraw_server_push_vtms.svg`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/static/img/undraw_tweetstorm.svg` & `soil-sdk-0.6.9/docs/website/static/img/undraw_tweetstorm.svg`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/static/img/undraw_version_control_9bpv.svg` & `soil-sdk-0.6.9/docs/website/static/img/undraw_version_control_9bpv.svg`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/docs/website/static/img/undraw_youtube_tutorial.svg` & `soil-sdk-0.6.9/docs/website/static/img/undraw_youtube_tutorial.svg`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/setup.cfg` & `soil-sdk-0.6.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/soil/__init__.py` & `soil-sdk-0.6.9/soil/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from soil.decorator import decorator
 from soil.dictionary import dictionary
 from soil.logger import logger
 
 # pylint:disable=consider-using-from-import
 from soil.modulify import modulify
 from soil.task import task, task_wait
-from soil.types import SerializableDataStructure
+from soil import types
 
 finder.upload_modules()
 
 __all__ = [
     "modulify",
     "data_structures",
     "modules",
@@ -26,9 +26,9 @@
     "connectors",
     "decorator",
     "task",
     "task_wait",
     "alerts",
     "dictionary",
     "errors",
-    "SerializableDataStructure",
+    "types",
 ]
```

### Comparing `soil-sdk-0.6.8.dev2/soil/alias.py` & `soil-sdk-0.6.9/soil/alias.py`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/soil/api.py` & `soil-sdk-0.6.9/soil/api.py`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/soil/configuration.py` & `soil-sdk-0.6.9/soil/configuration.py`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/soil/connectors/elastic_search.py` & `soil-sdk-0.6.9/soil/connectors/elastic_search.py`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/soil/data.py` & `soil-sdk-0.6.9/soil/data.py`

 * *Files 8% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 
 
 @overload
 def data(
     data_object: str,
     metadata: None = None,
     *,
-    return_type: Type[_GenericDataStructure] = None,
+    return_type: Type[_GenericDataStructure],
 ) -> _GenericDataStructure:
     ...
 
 
 @overload
 def data(
     data_object: _DataObject,
@@ -58,15 +58,15 @@
 
 
 @overload
 def data(
     data_object: _DataObject,
     metadata: dict[str, Any] | None = None,
     *,
-    return_type: Type[_GenericDataStructure] = None,
+    return_type: Type[_GenericDataStructure],
 ) -> _GenericDataStructure:
     ...
 
 
 def data(
     data_object: str | _DataObject,
     metadata: dict[str, Any] | None = None,
```

### Comparing `soil-sdk-0.6.8.dev2/soil/data_structure.py` & `soil-sdk-0.6.9/soil/data_structure.py`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/soil/decorator.py` & `soil-sdk-0.6.9/soil/decorator.py`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/soil/errors.py` & `soil-sdk-0.6.9/soil/errors.py`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/soil/finder.py` & `soil-sdk-0.6.9/soil/finder.py`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/soil/modulify.py` & `soil-sdk-0.6.9/soil/modulify.py`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/soil/pipeline.py` & `soil-sdk-0.6.9/soil/pipeline.py`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/soil/storage/base_storage.py` & `soil-sdk-0.6.9/soil/storage/base_storage.py`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/soil/storage/compound_storage.py` & `soil-sdk-0.6.9/soil/storage/compound_storage.py`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/soil/storage/elasticsearch.py` & `soil-sdk-0.6.9/soil/storage/elasticsearch.py`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/soil/storage/object_storage.py` & `soil-sdk-0.6.9/soil/storage/object_storage.py`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/soil/task.py` & `soil-sdk-0.6.9/soil/task.py`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/soil/types.py` & `soil-sdk-0.6.9/soil/types.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """ Types used by soil library"""
 # pylint:disable=unnecessary-ellipsis
 from enum import Enum
-from typing import Any, Dict, List, Protocol, Self, Type, TypedDict
+from typing import Dict, List, Protocol, Self, Type, TypedDict, TypeVar
 
 from soil.storage.base_storage import BaseStorage
 
 Plan = List[Dict[str, str]]
 
 
 class GetModule(TypedDict):
@@ -44,27 +44,31 @@
 class Result(TypedDict):
     """Type for GET results/:resultId"""
 
     _id: str
     type: str
 
 
-class SerializableDataStructure(Protocol):
+Storage = TypeVar("Storage", bound=BaseStorage)
+MetadataDict = TypeVar("MetadataDict", bound=TypedDict)
+
+
+class SerializableDataStructure(Protocol[Storage, MetadataDict]):
     """Data Strucutre base protocol"""
 
     @property
-    def metadata(self: Self) -> TypedDict:
+    def metadata(self: Self) -> MetadataDict:
         """Metadata of the DS protocol"""
         ...
 
-    def serialize(self) -> BaseStorage:
+    def serialize(self) -> Storage:
         """Serializes the DS."""
         ...
 
     @classmethod
     def deserialize(
         cls: Type[Self],
-        storage: BaseStorage,
-        metadata: Any,
-    ) -> Self:
+        storage: Storage,
+        metadata: MetadataDict,
+    ) -> "SerializableDataStructure[Storage, MetadataDict]":
         """Deserialize DS method."""
         ...
```

### Comparing `soil-sdk-0.6.8.dev2/soil/utils.py` & `soil-sdk-0.6.9/soil/utils.py`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/soil_cli/soil_cli.py` & `soil-sdk-0.6.9/soil_cli/soil_cli.py`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/soil_sdk.egg-info/PKG-INFO` & `soil-sdk-0.6.9/soil_sdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: soil-sdk
-Version: 0.6.8.dev2
+Version: 0.6.9
 Summary: SOIL Software Development Kit
 Home-page: https://developer.amalfianalytics.com/
 Author: Amalfi Analytics
 Author-email: info@amalfianalytics.com
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown; charset=UTF-8
 Provides-Extra: dev
```

### Comparing `soil-sdk-0.6.8.dev2/soil_sdk.egg-info/SOURCES.txt` & `soil-sdk-0.6.9/soil_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/test/unit/soil/test_alerts.py` & `soil-sdk-0.6.9/test/unit/soil/test_alerts.py`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/test/unit/soil/test_alias.py` & `soil-sdk-0.6.9/test/unit/soil/test_alias.py`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/test/unit/soil/test_data.py` & `soil-sdk-0.6.9/test/unit/soil/test_data.py`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/test/unit/soil/test_decorator.py` & `soil-sdk-0.6.9/test/unit/soil/test_decorator.py`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/test/unit/soil/test_dictionary.py` & `soil-sdk-0.6.9/test/unit/soil/test_dictionary.py`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/test/unit/soil/test_finder.py` & `soil-sdk-0.6.9/test/unit/soil/test_finder.py`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/test/unit/soil/test_pipelines.py` & `soil-sdk-0.6.9/test/unit/soil/test_pipelines.py`

 * *Files identical despite different names*

### Comparing `soil-sdk-0.6.8.dev2/test/unit/soil/test_utils.py` & `soil-sdk-0.6.9/test/unit/soil/test_utils.py`

 * *Files identical despite different names*

