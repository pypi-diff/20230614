# Comparing `tmp/semantha_sdk-5.3.2.tar.gz` & `tmp/semantha_sdk-5.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "semantha_sdk-5.3.2.tar", max compression
+gzip compressed data, was "semantha_sdk-5.4.0.tar", max compression
```

## Comparing `semantha_sdk-5.3.2.tar` & `semantha_sdk-5.4.0.tar`

### file list

```diff
@@ -1,145 +1,152 @@
--rw-r--r--   0        0        0    11545 2022-12-09 10:06:55.386837 semantha_sdk-5.3.2/LICENSE
--rw-r--r--   0        0        0     1618 2023-06-01 16:10:03.325342 semantha_sdk-5.3.2/pyproject.toml
--rw-r--r--   0        0        0     7795 2023-06-01 10:21:34.644458 semantha_sdk-5.3.2/README.md
--rw-r--r--   0        0        0     1288 2023-05-11 17:26:57.327736 semantha_sdk-5.3.2/semantha_sdk/__init__.py
--rw-r--r--   0        0        0        0 2023-05-11 17:26:57.329739 semantha_sdk-5.3.2/semantha_sdk/api/__init__.py
--rw-r--r--   0        0        0     1634 2023-06-01 08:29:07.930000 semantha_sdk-5.3.2/semantha_sdk/api/answers.py
--rw-r--r--   0        0        0      930 2023-06-01 08:29:07.488000 semantha_sdk-5.3.2/semantha_sdk/api/bulk.py
--rw-r--r--   0        0        0      729 2023-06-01 08:29:07.509000 semantha_sdk-5.3.2/semantha_sdk/api/bulk_domains.py
--rw-r--r--   0        0        0      739 2023-06-01 08:29:07.718000 semantha_sdk-5.3.2/semantha_sdk/api/bulk_model.py
--rw-r--r--   0        0        0     1628 2023-06-01 08:29:07.588000 semantha_sdk-5.3.2/semantha_sdk/api/bulkdomains_documentclasses.py
--rw-r--r--   0        0        0     1493 2023-06-01 08:29:07.539000 semantha_sdk-5.3.2/semantha_sdk/api/bulkdomains_domain.py
--rw-r--r--   0        0        0     3671 2023-06-01 08:29:07.677000 semantha_sdk-5.3.2/semantha_sdk/api/bulkdomains_referencedocuments.py
--rw-r--r--   0        0        0     3423 2023-06-01 08:29:07.710000 semantha_sdk-5.3.2/semantha_sdk/api/bulkdomains_references.py
--rw-r--r--   0        0        0     1191 2023-06-01 08:29:07.755000 semantha_sdk-5.3.2/semantha_sdk/api/bulkmodel_boostwords.py
--rw-r--r--   0        0        0      832 2023-06-01 08:29:07.775000 semantha_sdk-5.3.2/semantha_sdk/api/bulkmodel_class.py
--rw-r--r--   0        0        0     1730 2023-06-01 08:29:07.765000 semantha_sdk-5.3.2/semantha_sdk/api/bulkmodel_classes.py
--rw-r--r--   0        0        0     1577 2023-06-01 08:29:07.793000 semantha_sdk-5.3.2/semantha_sdk/api/bulkmodel_dataproperties.py
--rw-r--r--   0        0        0     2722 2023-06-01 08:29:07.744000 semantha_sdk-5.3.2/semantha_sdk/api/bulkmodel_domain.py
--rw-r--r--   0        0        0      726 2023-06-01 08:29:07.726000 semantha_sdk-5.3.2/semantha_sdk/api/bulkmodel_domains.py
--rw-r--r--   0        0        0     1509 2023-06-01 08:29:07.801000 semantha_sdk-5.3.2/semantha_sdk/api/bulkmodel_instances.py
--rw-r--r--   0        0        0     1508 2023-06-01 08:29:07.820000 semantha_sdk-5.3.2/semantha_sdk/api/bulkmodel_metadata.py
--rw-r--r--   0        0        0     1216 2023-06-01 08:29:07.830000 semantha_sdk-5.3.2/semantha_sdk/api/bulkmodel_namedentities.py
--rw-r--r--   0        0        0     1111 2023-06-01 08:29:07.837000 semantha_sdk-5.3.2/semantha_sdk/api/bulkmodel_stopwords.py
--rw-r--r--   0        0        0     1170 2023-06-01 08:29:07.846000 semantha_sdk-5.3.2/semantha_sdk/api/bulkmodel_synonyms.py
--rw-r--r--   0        0        0      976 2023-06-01 08:29:07.785000 semantha_sdk-5.3.2/semantha_sdk/api/bulkmodelclass_instances.py
--rw-r--r--   0        0        0     5667 2023-06-01 08:29:08.061000 semantha_sdk-5.3.2/semantha_sdk/api/clusters.py
--rw-r--r--   0        0        0     1050 2023-06-01 08:29:07.857000 semantha_sdk-5.3.2/semantha_sdk/api/currentuser.py
--rw-r--r--   0        0        0     1369 2023-06-01 08:29:07.881000 semantha_sdk-5.3.2/semantha_sdk/api/diff.py
--rw-r--r--   0        0        0     2315 2023-06-01 08:29:07.950000 semantha_sdk-5.3.2/semantha_sdk/api/documentannotations.py
--rw-r--r--   0        0        0     1387 2023-06-01 08:29:07.972000 semantha_sdk-5.3.2/semantha_sdk/api/documentclass.py
--rw-r--r--   0        0        0     1823 2023-06-01 08:29:07.960000 semantha_sdk-5.3.2/semantha_sdk/api/documentclasses.py
--rw-r--r--   0        0        0     3566 2023-06-01 08:29:07.990000 semantha_sdk-5.3.2/semantha_sdk/api/documentcomparisons.py
--rw-r--r--   0        0        0     3497 2023-06-01 08:29:08.005000 semantha_sdk-5.3.2/semantha_sdk/api/documents.py
--rw-r--r--   0        0        0     4161 2023-06-01 08:29:07.915000 semantha_sdk-5.3.2/semantha_sdk/api/domain.py
--rw-r--r--   0        0        0     1013 2023-06-01 08:29:07.890000 semantha_sdk-5.3.2/semantha_sdk/api/domains.py
--rw-r--r--   0        0        0      791 2023-06-01 08:29:08.258000 semantha_sdk-5.3.2/semantha_sdk/api/info.py
--rw-r--r--   0        0        0     1648 2023-06-01 08:29:08.270000 semantha_sdk-5.3.2/semantha_sdk/api/languages.py
--rw-r--r--   0        0        0     1529 2023-06-01 08:29:08.280000 semantha_sdk-5.3.2/semantha_sdk/api/model.py
--rw-r--r--   0        0        0     1545 2023-06-01 08:29:08.333000 semantha_sdk-5.3.2/semantha_sdk/api/model_boostwords.py
--rw-r--r--   0        0        0      762 2023-06-01 08:29:08.287000 semantha_sdk-5.3.2/semantha_sdk/api/model_datatypes.py
--rw-r--r--   0        0        0     1524 2023-06-01 08:29:08.309000 semantha_sdk-5.3.2/semantha_sdk/api/model_domain.py
--rw-r--r--   0        0        0      706 2023-06-01 08:29:08.299000 semantha_sdk-5.3.2/semantha_sdk/api/model_domains.py
--rw-r--r--   0        0        0      777 2023-06-01 08:29:08.359000 semantha_sdk-5.3.2/semantha_sdk/api/model_extractortypes.py
--rw-r--r--   0        0        0      774 2023-06-01 08:29:08.365000 semantha_sdk-5.3.2/semantha_sdk/api/model_metadatatypes.py
--rw-r--r--   0        0        0     1514 2023-06-01 08:29:08.351000 semantha_sdk-5.3.2/semantha_sdk/api/model_synonyms.py
--rw-r--r--   0        0        0     1107 2023-06-01 08:29:08.014000 semantha_sdk-5.3.2/semantha_sdk/api/modelclasses.py
--rw-r--r--   0        0        0     2315 2023-06-01 08:29:08.024000 semantha_sdk-5.3.2/semantha_sdk/api/modelinstances.py
--rw-r--r--   0        0        0     1546 2023-06-01 08:29:08.068000 semantha_sdk-5.3.2/semantha_sdk/api/namedentities.py
--rw-r--r--   0        0        0     1494 2023-06-01 08:29:08.108000 semantha_sdk-5.3.2/semantha_sdk/api/paragraph.py
--rw-r--r--   0        0        0      682 2023-06-01 08:29:08.100000 semantha_sdk-5.3.2/semantha_sdk/api/paragraphs.py
--rw-r--r--   0        0        0     2074 2023-06-01 08:29:08.094000 semantha_sdk-5.3.2/semantha_sdk/api/referencedocument.py
--rw-r--r--   0        0        0     8930 2023-06-01 08:29:08.047000 semantha_sdk-5.3.2/semantha_sdk/api/referencedocuments.py
--rw-r--r--   0        0        0     6565 2023-06-01 08:29:08.149000 semantha_sdk-5.3.2/semantha_sdk/api/references.py
--rw-r--r--   0        0        0      789 2023-06-01 08:29:07.866000 semantha_sdk-5.3.2/semantha_sdk/api/roles.py
--rw-r--r--   0        0        0     2113 2023-05-11 17:26:57.387783 semantha_sdk-5.3.2/semantha_sdk/api/semantha_api.py
--rw-r--r--   0        0        0      413 2023-05-11 17:26:57.389783 semantha_sdk-5.3.2/semantha_sdk/api/semantha_endpoint.py
--rw-r--r--   0        0        0      836 2023-06-01 08:29:08.122000 semantha_sdk-5.3.2/semantha_sdk/api/sentence.py
--rw-r--r--   0        0        0      676 2023-06-01 08:29:08.114000 semantha_sdk-5.3.2/semantha_sdk/api/sentences.py
--rw-r--r--   0        0        0     1379 2023-06-01 08:29:08.158000 semantha_sdk-5.3.2/semantha_sdk/api/settings.py
--rw-r--r--   0        0        0     5389 2023-06-01 08:29:08.174000 semantha_sdk-5.3.2/semantha_sdk/api/similaritymatrix.py
--rw-r--r--   0        0        0     4015 2023-06-01 08:29:08.199000 semantha_sdk-5.3.2/semantha_sdk/api/similaritymatrix_cluster.py
--rw-r--r--   0        0        0      844 2023-06-01 08:29:08.077000 semantha_sdk-5.3.2/semantha_sdk/api/statistic.py
--rw-r--r--   0        0        0      840 2023-06-01 08:29:08.220000 semantha_sdk-5.3.2/semantha_sdk/api/tag.py
--rw-r--r--   0        0        0     1115 2023-06-01 08:29:08.230000 semantha_sdk-5.3.2/semantha_sdk/api/tag_referencedocuments.py
--rw-r--r--   0        0        0      912 2023-06-01 08:29:08.210000 semantha_sdk-5.3.2/semantha_sdk/api/tags.py
--rw-r--r--   0        0        0     1310 2023-06-01 08:29:08.248000 semantha_sdk-5.3.2/semantha_sdk/api/validation.py
--rw-r--r--   0        0        0     4351 2023-06-01 14:03:14.059000 semantha_sdk-5.3.2/semantha_sdk/model/__init__.py
--rw-r--r--   0        0        0      607 2023-06-01 14:03:13.965000 semantha_sdk-5.3.2/semantha_sdk/model/annotation_cell.py
--rw-r--r--   0        0        0      654 2023-06-01 14:03:13.969000 semantha_sdk-5.3.2/semantha_sdk/model/annotation_page.py
--rw-r--r--   0        0        0      556 2023-06-01 14:03:14.024000 semantha_sdk-5.3.2/semantha_sdk/model/answer.py
--rw-r--r--   0        0        0      535 2023-06-01 14:03:14.007000 semantha_sdk-5.3.2/semantha_sdk/model/answer_reference.py
--rw-r--r--   0        0        0      546 2023-06-01 14:03:13.991000 semantha_sdk-5.3.2/semantha_sdk/model/boost_word.py
--rw-r--r--   0        0        0      930 2023-06-01 14:03:13.998000 semantha_sdk-5.3.2/semantha_sdk/model/class_bulk.py
--rw-r--r--   0        0        0      508 2023-06-01 14:03:13.971000 semantha_sdk-5.3.2/semantha_sdk/model/clustered_document.py
--rw-r--r--   0        0        0      672 2023-06-01 14:03:13.979000 semantha_sdk-5.3.2/semantha_sdk/model/clustering_response.py
--rw-r--r--   0        0        0     1139 2023-06-01 14:03:13.984000 semantha_sdk-5.3.2/semantha_sdk/model/complex_property.py
--rw-r--r--   0        0        0      516 2023-06-01 14:03:14.013000 semantha_sdk-5.3.2/semantha_sdk/model/current_user.py
--rw-r--r--   0        0        0      604 2023-06-01 14:03:14.044000 semantha_sdk-5.3.2/semantha_sdk/model/data_property.py
--rw-r--r--   0        0        0      476 2023-06-01 14:03:13.962000 semantha_sdk-5.3.2/semantha_sdk/model/difference.py
--rw-r--r--   0        0        0      519 2023-06-01 14:03:14.018000 semantha_sdk-5.3.2/semantha_sdk/model/distance.py
--rw-r--r--   0        0        0     1213 2023-06-01 14:03:14.043000 semantha_sdk-5.3.2/semantha_sdk/model/document.py
--rw-r--r--   0        0        0      939 2023-06-01 14:03:13.955000 semantha_sdk-5.3.2/semantha_sdk/model/document_class.py
--rw-r--r--   0        0        0      723 2023-06-01 14:03:14.030000 semantha_sdk-5.3.2/semantha_sdk/model/document_class_bulk.py
--rw-r--r--   0        0        0      566 2023-06-01 14:03:14.037000 semantha_sdk-5.3.2/semantha_sdk/model/document_class_node.py
--rw-r--r--   0        0        0      628 2023-06-01 14:03:13.989000 semantha_sdk-5.3.2/semantha_sdk/model/document_cluster.py
--rw-r--r--   0        0        0     1004 2023-06-01 14:03:13.976000 semantha_sdk-5.3.2/semantha_sdk/model/document_information.py
--rw-r--r--   0        0        0      503 2023-06-01 14:03:13.942000 semantha_sdk-5.3.2/semantha_sdk/model/document_meta_data.py
--rw-r--r--   0        0        0      498 2023-06-01 14:03:13.963000 semantha_sdk-5.3.2/semantha_sdk/model/document_named_entity.py
--rw-r--r--   0        0        0      510 2023-06-01 14:03:13.970000 semantha_sdk-5.3.2/semantha_sdk/model/document_table.py
--rw-r--r--   0        0        0      564 2023-06-01 14:03:13.994000 semantha_sdk-5.3.2/semantha_sdk/model/domain.py
--rw-r--r--   0        0        0      447 2023-06-01 14:03:14.032000 semantha_sdk-5.3.2/semantha_sdk/model/entity.py
--rw-r--r--   0        0        0      597 2023-06-01 14:03:13.977000 semantha_sdk-5.3.2/semantha_sdk/model/extraction_area.py
--rw-r--r--   0        0        0      729 2023-06-01 14:03:14.015000 semantha_sdk-5.3.2/semantha_sdk/model/extraction_file.py
--rw-r--r--   0        0        0      536 2023-06-01 14:03:14.022000 semantha_sdk-5.3.2/semantha_sdk/model/extraction_reference.py
--rw-r--r--   0        0        0      842 2023-06-01 14:03:14.012000 semantha_sdk-5.3.2/semantha_sdk/model/features.py
--rw-r--r--   0        0        0      512 2023-06-01 14:03:14.017000 semantha_sdk-5.3.2/semantha_sdk/model/file_reference.py
--rw-r--r--   0        0        0      498 2023-06-01 14:03:14.008000 semantha_sdk-5.3.2/semantha_sdk/model/finding.py
--rw-r--r--   0        0        0      524 2023-06-01 14:03:14.019000 semantha_sdk-5.3.2/semantha_sdk/model/info.py
--rw-r--r--   0        0        0      839 2023-06-01 14:03:14.028000 semantha_sdk-5.3.2/semantha_sdk/model/instance.py
--rw-r--r--   0        0        0      531 2023-06-01 14:03:13.947000 semantha_sdk-5.3.2/semantha_sdk/model/instance_child.py
--rw-r--r--   0        0        0      408 2023-06-01 14:03:13.992000 semantha_sdk-5.3.2/semantha_sdk/model/label.py
--rw-r--r--   0        0        0      474 2023-06-01 14:03:13.961000 semantha_sdk-5.3.2/semantha_sdk/model/language_detection.py
--rw-r--r--   0        0        0      576 2023-06-01 14:03:13.982000 semantha_sdk-5.3.2/semantha_sdk/model/linked_instance.py
--rw-r--r--   0        0        0      483 2023-06-01 14:03:13.973000 semantha_sdk-5.3.2/semantha_sdk/model/linked_value.py
--rw-r--r--   0        0        0      582 2023-06-01 14:03:13.944000 semantha_sdk-5.3.2/semantha_sdk/model/matrix_row.py
--rw-r--r--   0        0        0      499 2023-06-01 14:03:14.016000 semantha_sdk-5.3.2/semantha_sdk/model/meta_info_page.py
--rw-r--r--   0        0        0      493 2023-06-01 14:03:13.959000 semantha_sdk-5.3.2/semantha_sdk/model/metadata.py
--rw-r--r--   0        0        0      430 2023-06-01 14:03:13.958000 semantha_sdk-5.3.2/semantha_sdk/model/metadata_value.py
--rw-r--r--   0        0        0      528 2023-06-01 14:03:14.021000 semantha_sdk-5.3.2/semantha_sdk/model/model_class.py
--rw-r--r--   0        0        0     1482 2023-06-01 14:03:13.968000 semantha_sdk-5.3.2/semantha_sdk/model/model_instance.py
--rw-r--r--   0        0        0      485 2023-06-01 14:03:14.006000 semantha_sdk-5.3.2/semantha_sdk/model/named_entity.py
--rw-r--r--   0        0        0      812 2023-06-01 14:03:13.952000 semantha_sdk-5.3.2/semantha_sdk/model/page.py
--rw-r--r--   0        0        0      528 2023-06-01 14:03:14.023000 semantha_sdk-5.3.2/semantha_sdk/model/page_content.py
--rw-r--r--   0        0        0      948 2023-06-01 14:03:14.034000 semantha_sdk-5.3.2/semantha_sdk/model/paragraph.py
--rw-r--r--   0        0        0      486 2023-06-01 14:03:13.992000 semantha_sdk-5.3.2/semantha_sdk/model/paragraph_update.py
--rw-r--r--   0        0        0      493 2023-06-01 14:03:14.037000 semantha_sdk-5.3.2/semantha_sdk/model/plotly_chart.py
--rw-r--r--   0        0        0      577 2023-06-01 14:03:13.980000 semantha_sdk-5.3.2/semantha_sdk/model/process_information.py
--rw-r--r--   0        0        0      445 2023-06-01 14:03:14.020000 semantha_sdk-5.3.2/semantha_sdk/model/rect.py
--rw-r--r--   0        0        0      775 2023-06-01 14:03:14.026000 semantha_sdk-5.3.2/semantha_sdk/model/reference.py
--rw-r--r--   0        0        0      728 2023-06-01 14:03:13.960000 semantha_sdk-5.3.2/semantha_sdk/model/reference_documents_response_container.py
--rw-r--r--   0        0        0      646 2023-06-01 14:03:14.000000 semantha_sdk-5.3.2/semantha_sdk/model/response_meta_info.py
--rw-r--r--   0        0        0      500 2023-06-01 14:03:14.040000 semantha_sdk-5.3.2/semantha_sdk/model/row.py
--rw-r--r--   0        0        0      650 2023-05-11 17:26:57.498002 semantha_sdk-5.3.2/semantha_sdk/model/semantha_entity.py
--rw-r--r--   0        0        0      873 2023-06-01 14:03:14.035000 semantha_sdk-5.3.2/semantha_sdk/model/semantic_model.py
--rw-r--r--   0        0        0      518 2023-06-01 14:03:13.981000 semantha_sdk-5.3.2/semantha_sdk/model/semi_super_vised_document.py
--rw-r--r--   0        0        0      792 2023-06-01 14:03:13.986000 semantha_sdk-5.3.2/semantha_sdk/model/sentence.py
--rw-r--r--   0        0        0     1669 2023-06-01 14:03:14.004000 semantha_sdk-5.3.2/semantha_sdk/model/settings.py
--rw-r--r--   0        0        0      454 2023-06-01 14:03:14.009000 semantha_sdk-5.3.2/semantha_sdk/model/simple_property.py
--rw-r--r--   0        0        0      695 2023-06-01 14:03:13.950000 semantha_sdk-5.3.2/semantha_sdk/model/smart_cluster_response_container.py
--rw-r--r--   0        0        0      851 2023-06-01 14:03:13.988000 semantha_sdk-5.3.2/semantha_sdk/model/smart_cluster_semi_supervised_request.py
--rw-r--r--   0        0        0      608 2023-06-01 14:03:14.031000 semantha_sdk-5.3.2/semantha_sdk/model/statistic.py
--rw-r--r--   0        0        0      480 2023-06-01 14:03:13.953000 semantha_sdk-5.3.2/semantha_sdk/model/stop_word.py
--rw-r--r--   0        0        0      542 2023-06-01 14:03:14.039000 semantha_sdk-5.3.2/semantha_sdk/model/synonym.py
--rw-r--r--   0        0        0      446 2023-06-01 14:03:13.957000 semantha_sdk-5.3.2/semantha_sdk/model/table_cell.py
--rw-r--r--   0        0        0      565 2023-06-01 14:03:13.999000 semantha_sdk-5.3.2/semantha_sdk/model/table_instance.py
--rw-r--r--   0        0        0      462 2023-06-01 14:03:13.956000 semantha_sdk-5.3.2/semantha_sdk/model/tag_docs.py
--rw-r--r--   0        0        0      464 2023-06-01 14:03:13.995000 semantha_sdk-5.3.2/semantha_sdk/model/version.py
--rw-r--r--   0        0        0       47 2023-05-11 17:26:57.519543 semantha_sdk-5.3.2/semantha_sdk/request/__init__.py
--rw-r--r--   0        0        0      552 2023-05-11 17:26:57.521550 semantha_sdk-5.3.2/semantha_sdk/request/semantha_request.py
--rw-r--r--   0        0        0       57 2023-05-11 17:26:57.522556 semantha_sdk-5.3.2/semantha_sdk/response/__init__.py
--rw-r--r--   0        0        0      107 2023-05-11 17:26:57.524555 semantha_sdk-5.3.2/semantha_sdk/response/semantha_error.py
--rw-r--r--   0        0        0     3472 2023-05-11 17:26:57.525555 semantha_sdk-5.3.2/semantha_sdk/response/semantha_response.py
--rw-r--r--   0        0        0       37 2023-05-11 17:26:57.527555 semantha_sdk-5.3.2/semantha_sdk/rest/__init__.py
--rw-r--r--   0        0        0     4354 2023-05-11 17:26:57.528555 semantha_sdk-5.3.2/semantha_sdk/rest/rest_client.py
--rw-r--r--   0        0        0     8464 1970-01-01 00:00:00.000000 semantha_sdk-5.3.2/PKG-INFO
+-rw-r--r--   0        0        0    11545 2022-12-09 10:06:55.386837 semantha_sdk-5.4.0/LICENSE
+-rw-r--r--   0        0        0     1618 2023-06-13 17:47:41.628078 semantha_sdk-5.4.0/pyproject.toml
+-rw-r--r--   0        0        0    14233 2023-06-13 15:55:55.289520 semantha_sdk-5.4.0/README.md
+-rw-r--r--   0        0        0     1288 2023-05-11 17:26:57.327736 semantha_sdk-5.4.0/semantha_sdk/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-11 17:26:57.329739 semantha_sdk-5.4.0/semantha_sdk/api/__init__.py
+-rw-r--r--   0        0        0     1634 2023-06-13 15:51:25.476000 semantha_sdk-5.4.0/semantha_sdk/api/answers.py
+-rw-r--r--   0        0        0      930 2023-06-13 15:51:25.348000 semantha_sdk-5.4.0/semantha_sdk/api/bulk.py
+-rw-r--r--   0        0        0      729 2023-06-13 15:51:25.352000 semantha_sdk-5.4.0/semantha_sdk/api/bulk_domains.py
+-rw-r--r--   0        0        0      739 2023-06-13 15:51:25.409000 semantha_sdk-5.4.0/semantha_sdk/api/bulk_model.py
+-rw-r--r--   0        0        0     1628 2023-06-13 15:51:25.375000 semantha_sdk-5.4.0/semantha_sdk/api/bulkdomains_documentclasses.py
+-rw-r--r--   0        0        0     1493 2023-06-13 15:51:25.361000 semantha_sdk-5.4.0/semantha_sdk/api/bulkdomains_domain.py
+-rw-r--r--   0        0        0     3671 2023-06-13 15:51:25.396000 semantha_sdk-5.4.0/semantha_sdk/api/bulkdomains_referencedocuments.py
+-rw-r--r--   0        0        0     3423 2023-06-13 15:51:25.406000 semantha_sdk-5.4.0/semantha_sdk/api/bulkdomains_references.py
+-rw-r--r--   0        0        0     1191 2023-06-13 15:51:25.422000 semantha_sdk-5.4.0/semantha_sdk/api/bulkmodel_boostwords.py
+-rw-r--r--   0        0        0      832 2023-06-13 15:51:25.430000 semantha_sdk-5.4.0/semantha_sdk/api/bulkmodel_class.py
+-rw-r--r--   0        0        0     1730 2023-06-13 15:51:25.426000 semantha_sdk-5.4.0/semantha_sdk/api/bulkmodel_classes.py
+-rw-r--r--   0        0        0     1577 2023-06-13 15:51:25.436000 semantha_sdk-5.4.0/semantha_sdk/api/bulkmodel_dataproperties.py
+-rw-r--r--   0        0        0     2722 2023-06-13 15:51:25.418000 semantha_sdk-5.4.0/semantha_sdk/api/bulkmodel_domain.py
+-rw-r--r--   0        0        0      726 2023-06-13 15:51:25.414000 semantha_sdk-5.4.0/semantha_sdk/api/bulkmodel_domains.py
+-rw-r--r--   0        0        0     1509 2023-06-13 15:51:25.439000 semantha_sdk-5.4.0/semantha_sdk/api/bulkmodel_instances.py
+-rw-r--r--   0        0        0     1508 2023-06-13 15:51:25.448000 semantha_sdk-5.4.0/semantha_sdk/api/bulkmodel_metadata.py
+-rw-r--r--   0        0        0     1216 2023-06-13 15:51:25.451000 semantha_sdk-5.4.0/semantha_sdk/api/bulkmodel_namedentities.py
+-rw-r--r--   0        0        0     1111 2023-06-13 15:51:25.453000 semantha_sdk-5.4.0/semantha_sdk/api/bulkmodel_stopwords.py
+-rw-r--r--   0        0        0     1170 2023-06-13 15:51:25.455000 semantha_sdk-5.4.0/semantha_sdk/api/bulkmodel_synonyms.py
+-rw-r--r--   0        0        0      976 2023-06-13 15:51:25.433000 semantha_sdk-5.4.0/semantha_sdk/api/bulkmodelclass_instances.py
+-rw-r--r--   0        0        0     5667 2023-06-13 15:51:25.526000 semantha_sdk-5.4.0/semantha_sdk/api/clusters.py
+-rw-r--r--   0        0        0     1050 2023-06-13 15:51:25.457000 semantha_sdk-5.4.0/semantha_sdk/api/currentuser.py
+-rw-r--r--   0        0        0     1369 2023-06-13 15:51:25.462000 semantha_sdk-5.4.0/semantha_sdk/api/diff.py
+-rw-r--r--   0        0        0     2315 2023-06-13 15:51:25.481000 semantha_sdk-5.4.0/semantha_sdk/api/documentannotations.py
+-rw-r--r--   0        0        0     1387 2023-06-13 15:51:25.492000 semantha_sdk-5.4.0/semantha_sdk/api/documentclass.py
+-rw-r--r--   0        0        0     1823 2023-06-13 15:51:25.487000 semantha_sdk-5.4.0/semantha_sdk/api/documentclasses.py
+-rw-r--r--   0        0        0     3566 2023-06-13 15:51:25.498000 semantha_sdk-5.4.0/semantha_sdk/api/documentcomparisons.py
+-rw-r--r--   0        0        0     3497 2023-06-13 15:51:25.502000 semantha_sdk-5.4.0/semantha_sdk/api/documents.py
+-rw-r--r--   0        0        0     4424 2023-06-13 15:51:25.471000 semantha_sdk-5.4.0/semantha_sdk/api/domain.py
+-rw-r--r--   0        0        0     1013 2023-06-13 15:51:25.465000 semantha_sdk-5.4.0/semantha_sdk/api/domains.py
+-rw-r--r--   0        0        0      791 2023-06-13 15:51:25.603000 semantha_sdk-5.4.0/semantha_sdk/api/info.py
+-rw-r--r--   0        0        0     1648 2023-06-13 15:51:25.606000 semantha_sdk-5.4.0/semantha_sdk/api/languages.py
+-rw-r--r--   0        0        0     1529 2023-06-13 15:51:25.609000 semantha_sdk-5.4.0/semantha_sdk/api/model.py
+-rw-r--r--   0        0        0     1278 2023-06-13 15:51:25.622000 semantha_sdk-5.4.0/semantha_sdk/api/model_boostword.py
+-rw-r--r--   0        0        0     1754 2023-06-13 15:51:25.619000 semantha_sdk-5.4.0/semantha_sdk/api/model_boostwords.py
+-rw-r--r--   0        0        0      762 2023-06-13 15:51:25.610000 semantha_sdk-5.4.0/semantha_sdk/api/model_datatypes.py
+-rw-r--r--   0        0        0     2050 2023-06-13 15:51:25.616000 semantha_sdk-5.4.0/semantha_sdk/api/model_domain.py
+-rw-r--r--   0        0        0      706 2023-06-13 15:51:25.612000 semantha_sdk-5.4.0/semantha_sdk/api/model_domains.py
+-rw-r--r--   0        0        0      777 2023-06-13 15:51:25.641000 semantha_sdk-5.4.0/semantha_sdk/api/model_extractortypes.py
+-rw-r--r--   0        0        0      774 2023-06-13 15:51:25.644000 semantha_sdk-5.4.0/semantha_sdk/api/model_metadatatypes.py
+-rw-r--r--   0        0        0     1798 2023-06-13 15:51:25.625000 semantha_sdk-5.4.0/semantha_sdk/api/model_namedentities.py
+-rw-r--r--   0        0        0     1314 2023-06-13 15:51:25.630000 semantha_sdk-5.4.0/semantha_sdk/api/model_namedentity.py
+-rw-r--r--   0        0        0     1266 2023-06-13 15:51:25.635000 semantha_sdk-5.4.0/semantha_sdk/api/model_stopword.py
+-rw-r--r--   0        0        0     1738 2023-06-13 15:51:25.633000 semantha_sdk-5.4.0/semantha_sdk/api/model_stopwords.py
+-rw-r--r--   0        0        0     1247 2023-06-13 15:51:25.639000 semantha_sdk-5.4.0/semantha_sdk/api/model_synonym.py
+-rw-r--r--   0        0        0     1715 2023-06-13 15:51:25.637000 semantha_sdk-5.4.0/semantha_sdk/api/model_synonyms.py
+-rw-r--r--   0        0        0     1107 2023-06-13 15:51:25.506000 semantha_sdk-5.4.0/semantha_sdk/api/modelclasses.py
+-rw-r--r--   0        0        0     2315 2023-06-13 15:51:25.509000 semantha_sdk-5.4.0/semantha_sdk/api/modelinstances.py
+-rw-r--r--   0        0        0     1546 2023-06-13 15:51:25.529000 semantha_sdk-5.4.0/semantha_sdk/api/namedentities.py
+-rw-r--r--   0        0        0     1494 2023-06-13 15:51:25.542000 semantha_sdk-5.4.0/semantha_sdk/api/paragraph.py
+-rw-r--r--   0        0        0      682 2023-06-13 15:51:25.539000 semantha_sdk-5.4.0/semantha_sdk/api/paragraphs.py
+-rw-r--r--   0        0        0     2074 2023-06-13 15:51:25.537000 semantha_sdk-5.4.0/semantha_sdk/api/referencedocument.py
+-rw-r--r--   0        0        0     8930 2023-06-13 15:51:25.518000 semantha_sdk-5.4.0/semantha_sdk/api/referencedocuments.py
+-rw-r--r--   0        0        0     6565 2023-06-13 15:51:25.554000 semantha_sdk-5.4.0/semantha_sdk/api/references.py
+-rw-r--r--   0        0        0      789 2023-06-13 15:51:25.459000 semantha_sdk-5.4.0/semantha_sdk/api/roles.py
+-rw-r--r--   0        0        0     2113 2023-05-11 17:26:57.387783 semantha_sdk-5.4.0/semantha_sdk/api/semantha_api.py
+-rw-r--r--   0        0        0      413 2023-05-11 17:26:57.389783 semantha_sdk-5.4.0/semantha_sdk/api/semantha_endpoint.py
+-rw-r--r--   0        0        0      836 2023-06-13 15:51:25.547000 semantha_sdk-5.4.0/semantha_sdk/api/sentence.py
+-rw-r--r--   0        0        0      676 2023-06-13 15:51:25.545000 semantha_sdk-5.4.0/semantha_sdk/api/sentences.py
+-rw-r--r--   0        0        0     1379 2023-06-13 15:51:25.558000 semantha_sdk-5.4.0/semantha_sdk/api/settings.py
+-rw-r--r--   0        0        0     5389 2023-06-13 15:51:25.563000 semantha_sdk-5.4.0/semantha_sdk/api/similaritymatrix.py
+-rw-r--r--   0        0        0     4015 2023-06-13 15:51:25.567000 semantha_sdk-5.4.0/semantha_sdk/api/similaritymatrix_cluster.py
+-rw-r--r--   0        0        0      844 2023-06-13 15:51:25.531000 semantha_sdk-5.4.0/semantha_sdk/api/statistic.py
+-rw-r--r--   0        0        0     1069 2023-06-13 15:51:25.586000 semantha_sdk-5.4.0/semantha_sdk/api/summarizations.py
+-rw-r--r--   0        0        0      840 2023-06-13 15:51:25.591000 semantha_sdk-5.4.0/semantha_sdk/api/tag.py
+-rw-r--r--   0        0        0     1115 2023-06-13 15:51:25.592000 semantha_sdk-5.4.0/semantha_sdk/api/tag_referencedocuments.py
+-rw-r--r--   0        0        0      912 2023-06-13 15:51:25.588000 semantha_sdk-5.4.0/semantha_sdk/api/tags.py
+-rw-r--r--   0        0        0     1310 2023-06-13 15:51:25.601000 semantha_sdk-5.4.0/semantha_sdk/api/validation.py
+-rw-r--r--   0        0        0     4351 2023-06-12 08:36:49.200000 semantha_sdk-5.4.0/semantha_sdk/model/__init__.py
+-rw-r--r--   0        0        0      607 2023-06-12 08:36:48.908000 semantha_sdk-5.4.0/semantha_sdk/model/annotation_cell.py
+-rw-r--r--   0        0        0      654 2023-06-12 08:36:48.924000 semantha_sdk-5.4.0/semantha_sdk/model/annotation_page.py
+-rw-r--r--   0        0        0      556 2023-06-12 08:36:49.089000 semantha_sdk-5.4.0/semantha_sdk/model/answer.py
+-rw-r--r--   0        0        0      535 2023-06-12 08:36:49.028000 semantha_sdk-5.4.0/semantha_sdk/model/answer_reference.py
+-rw-r--r--   0        0        0      546 2023-06-12 08:36:48.976000 semantha_sdk-5.4.0/semantha_sdk/model/boost_word.py
+-rw-r--r--   0        0        0      930 2023-06-12 08:36:48.998000 semantha_sdk-5.4.0/semantha_sdk/model/class_bulk.py
+-rw-r--r--   0        0        0      508 2023-06-12 08:36:48.929000 semantha_sdk-5.4.0/semantha_sdk/model/clustered_document.py
+-rw-r--r--   0        0        0      672 2023-06-12 08:36:48.945000 semantha_sdk-5.4.0/semantha_sdk/model/clustering_response.py
+-rw-r--r--   0        0        0     1139 2023-06-12 08:36:48.960000 semantha_sdk-5.4.0/semantha_sdk/model/complex_property.py
+-rw-r--r--   0        0        0      516 2023-06-12 08:36:49.045000 semantha_sdk-5.4.0/semantha_sdk/model/current_user.py
+-rw-r--r--   0        0        0      604 2023-06-12 08:36:49.155000 semantha_sdk-5.4.0/semantha_sdk/model/data_property.py
+-rw-r--r--   0        0        0      476 2023-06-12 08:36:48.898000 semantha_sdk-5.4.0/semantha_sdk/model/difference.py
+-rw-r--r--   0        0        0      519 2023-06-12 08:36:49.063000 semantha_sdk-5.4.0/semantha_sdk/model/distance.py
+-rw-r--r--   0        0        0     1213 2023-06-12 08:36:49.150000 semantha_sdk-5.4.0/semantha_sdk/model/document.py
+-rw-r--r--   0        0        0      939 2023-06-12 08:36:48.878000 semantha_sdk-5.4.0/semantha_sdk/model/document_class.py
+-rw-r--r--   0        0        0      723 2023-06-12 08:36:49.110000 semantha_sdk-5.4.0/semantha_sdk/model/document_class_bulk.py
+-rw-r--r--   0        0        0      566 2023-06-12 08:36:49.130000 semantha_sdk-5.4.0/semantha_sdk/model/document_class_node.py
+-rw-r--r--   0        0        0      628 2023-06-12 08:36:48.972000 semantha_sdk-5.4.0/semantha_sdk/model/document_cluster.py
+-rw-r--r--   0        0        0     1004 2023-06-12 08:36:48.940000 semantha_sdk-5.4.0/semantha_sdk/model/document_information.py
+-rw-r--r--   0        0        0      503 2023-06-12 08:36:48.835000 semantha_sdk-5.4.0/semantha_sdk/model/document_meta_data.py
+-rw-r--r--   0        0        0      498 2023-06-12 08:36:48.903000 semantha_sdk-5.4.0/semantha_sdk/model/document_named_entity.py
+-rw-r--r--   0        0        0      510 2023-06-12 08:36:48.926000 semantha_sdk-5.4.0/semantha_sdk/model/document_table.py
+-rw-r--r--   0        0        0      564 2023-06-12 08:36:48.989000 semantha_sdk-5.4.0/semantha_sdk/model/domain.py
+-rw-r--r--   0        0        0      447 2023-06-12 08:36:49.116000 semantha_sdk-5.4.0/semantha_sdk/model/entity.py
+-rw-r--r--   0        0        0      597 2023-06-12 08:36:48.943000 semantha_sdk-5.4.0/semantha_sdk/model/extraction_area.py
+-rw-r--r--   0        0        0      729 2023-06-12 08:36:49.053000 semantha_sdk-5.4.0/semantha_sdk/model/extraction_file.py
+-rw-r--r--   0        0        0      536 2023-06-12 08:36:49.081000 semantha_sdk-5.4.0/semantha_sdk/model/extraction_reference.py
+-rw-r--r--   0        0        0      842 2023-06-12 08:36:49.041000 semantha_sdk-5.4.0/semantha_sdk/model/features.py
+-rw-r--r--   0        0        0      512 2023-06-12 08:36:49.059000 semantha_sdk-5.4.0/semantha_sdk/model/file_reference.py
+-rw-r--r--   0        0        0      498 2023-06-12 08:36:49.031000 semantha_sdk-5.4.0/semantha_sdk/model/finding.py
+-rw-r--r--   0        0        0      524 2023-06-12 08:36:49.068000 semantha_sdk-5.4.0/semantha_sdk/model/info.py
+-rw-r--r--   0        0        0      839 2023-06-12 08:36:49.103000 semantha_sdk-5.4.0/semantha_sdk/model/instance.py
+-rw-r--r--   0        0        0      531 2023-06-12 08:36:48.852000 semantha_sdk-5.4.0/semantha_sdk/model/instance_child.py
+-rw-r--r--   0        0        0      408 2023-06-12 08:36:48.984000 semantha_sdk-5.4.0/semantha_sdk/model/label.py
+-rw-r--r--   0        0        0      474 2023-06-12 08:36:48.896000 semantha_sdk-5.4.0/semantha_sdk/model/language_detection.py
+-rw-r--r--   0        0        0      576 2023-06-12 08:36:48.953000 semantha_sdk-5.4.0/semantha_sdk/model/linked_instance.py
+-rw-r--r--   0        0        0      483 2023-06-12 08:36:48.932000 semantha_sdk-5.4.0/semantha_sdk/model/linked_value.py
+-rw-r--r--   0        0        0      582 2023-06-12 08:36:48.841000 semantha_sdk-5.4.0/semantha_sdk/model/matrix_row.py
+-rw-r--r--   0        0        0      499 2023-06-12 08:36:49.056000 semantha_sdk-5.4.0/semantha_sdk/model/meta_info_page.py
+-rw-r--r--   0        0        0      493 2023-06-12 08:36:48.892000 semantha_sdk-5.4.0/semantha_sdk/model/metadata.py
+-rw-r--r--   0        0        0      430 2023-06-12 08:36:48.888000 semantha_sdk-5.4.0/semantha_sdk/model/metadata_value.py
+-rw-r--r--   0        0        0      528 2023-06-12 08:36:49.077000 semantha_sdk-5.4.0/semantha_sdk/model/model_class.py
+-rw-r--r--   0        0        0     1482 2023-06-12 08:36:48.919000 semantha_sdk-5.4.0/semantha_sdk/model/model_instance.py
+-rw-r--r--   0        0        0      485 2023-06-12 08:36:49.025000 semantha_sdk-5.4.0/semantha_sdk/model/named_entity.py
+-rw-r--r--   0        0        0      812 2023-06-12 08:36:48.865000 semantha_sdk-5.4.0/semantha_sdk/model/page.py
+-rw-r--r--   0        0        0      528 2023-06-12 08:36:49.083000 semantha_sdk-5.4.0/semantha_sdk/model/page_content.py
+-rw-r--r--   0        0        0      948 2023-06-12 08:36:49.123000 semantha_sdk-5.4.0/semantha_sdk/model/paragraph.py
+-rw-r--r--   0        0        0      486 2023-06-12 08:36:48.981000 semantha_sdk-5.4.0/semantha_sdk/model/paragraph_update.py
+-rw-r--r--   0        0        0      493 2023-06-12 08:36:49.132000 semantha_sdk-5.4.0/semantha_sdk/model/plotly_chart.py
+-rw-r--r--   0        0        0      577 2023-06-12 08:36:48.948000 semantha_sdk-5.4.0/semantha_sdk/model/process_information.py
+-rw-r--r--   0        0        0      445 2023-06-12 08:36:49.073000 semantha_sdk-5.4.0/semantha_sdk/model/rect.py
+-rw-r--r--   0        0        0      775 2023-06-12 08:36:49.095000 semantha_sdk-5.4.0/semantha_sdk/model/reference.py
+-rw-r--r--   0        0        0      728 2023-06-12 08:36:48.894000 semantha_sdk-5.4.0/semantha_sdk/model/reference_documents_response_container.py
+-rw-r--r--   0        0        0      646 2023-06-12 08:36:49.007000 semantha_sdk-5.4.0/semantha_sdk/model/response_meta_info.py
+-rw-r--r--   0        0        0      500 2023-06-12 08:36:49.141000 semantha_sdk-5.4.0/semantha_sdk/model/row.py
+-rw-r--r--   0        0        0      650 2023-05-11 17:26:57.498002 semantha_sdk-5.4.0/semantha_sdk/model/semantha_entity.py
+-rw-r--r--   0        0        0      873 2023-06-12 08:36:49.127000 semantha_sdk-5.4.0/semantha_sdk/model/semantic_model.py
+-rw-r--r--   0        0        0      518 2023-06-12 08:36:48.950000 semantha_sdk-5.4.0/semantha_sdk/model/semi_super_vised_document.py
+-rw-r--r--   0        0        0      792 2023-06-12 08:36:48.965000 semantha_sdk-5.4.0/semantha_sdk/model/sentence.py
+-rw-r--r--   0        0        0     1669 2023-06-12 08:36:49.022000 semantha_sdk-5.4.0/semantha_sdk/model/settings.py
+-rw-r--r--   0        0        0      454 2023-06-12 08:36:49.033000 semantha_sdk-5.4.0/semantha_sdk/model/simple_property.py
+-rw-r--r--   0        0        0      695 2023-06-12 08:36:48.860000 semantha_sdk-5.4.0/semantha_sdk/model/smart_cluster_response_container.py
+-rw-r--r--   0        0        0      851 2023-06-12 08:36:48.969000 semantha_sdk-5.4.0/semantha_sdk/model/smart_cluster_semi_supervised_request.py
+-rw-r--r--   0        0        0      608 2023-06-12 08:36:49.114000 semantha_sdk-5.4.0/semantha_sdk/model/statistic.py
+-rw-r--r--   0        0        0      480 2023-06-12 08:36:48.869000 semantha_sdk-5.4.0/semantha_sdk/model/stop_word.py
+-rw-r--r--   0        0        0      542 2023-06-12 08:36:49.136000 semantha_sdk-5.4.0/semantha_sdk/model/synonym.py
+-rw-r--r--   0        0        0      446 2023-06-12 08:36:48.884000 semantha_sdk-5.4.0/semantha_sdk/model/table_cell.py
+-rw-r--r--   0        0        0      565 2023-06-12 08:36:49.004000 semantha_sdk-5.4.0/semantha_sdk/model/table_instance.py
+-rw-r--r--   0        0        0      462 2023-06-12 08:36:48.881000 semantha_sdk-5.4.0/semantha_sdk/model/tag_docs.py
+-rw-r--r--   0        0        0      464 2023-06-12 08:36:48.992000 semantha_sdk-5.4.0/semantha_sdk/model/version.py
+-rw-r--r--   0        0        0       47 2023-05-11 17:26:57.519543 semantha_sdk-5.4.0/semantha_sdk/request/__init__.py
+-rw-r--r--   0        0        0      552 2023-05-11 17:26:57.521550 semantha_sdk-5.4.0/semantha_sdk/request/semantha_request.py
+-rw-r--r--   0        0        0       57 2023-05-11 17:26:57.522556 semantha_sdk-5.4.0/semantha_sdk/response/__init__.py
+-rw-r--r--   0        0        0      107 2023-05-11 17:26:57.524555 semantha_sdk-5.4.0/semantha_sdk/response/semantha_error.py
+-rw-r--r--   0        0        0     3472 2023-05-11 17:26:57.525555 semantha_sdk-5.4.0/semantha_sdk/response/semantha_response.py
+-rw-r--r--   0        0        0       37 2023-05-11 17:26:57.527555 semantha_sdk-5.4.0/semantha_sdk/rest/__init__.py
+-rw-r--r--   0        0        0     4354 2023-05-11 17:26:57.528555 semantha_sdk-5.4.0/semantha_sdk/rest/rest_client.py
+-rw-r--r--   0        0        0    14791 1970-01-01 00:00:00.000000 semantha_sdk-5.4.0/PKG-INFO
```

### Comparing `semantha_sdk-5.3.2/LICENSE` & `semantha_sdk-5.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.3.2/pyproject.toml` & `semantha_sdk-5.4.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "semantha-sdk"
-version = "5.3.2"
+version = "5.4.0"
 description = "This is a python client sdk for accessing semantha (the semantic platform)"
 authors = [
     "Sebastian Weigelt <sebastian.weigelt@semantha.ai>",
     "Georg Müller <georg@semantha.ai>",
     "Tom Kaminski <tom.kaminski@semantha.ai>",
     "Timo Januschke <timo.januschke@semantha.ai>"
 ]
```

### Comparing `semantha_sdk-5.3.2/semantha_sdk/__init__.py` & `semantha_sdk-5.4.0/semantha_sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.3.2/semantha_sdk/api/answers.py` & `semantha_sdk-5.4.0/semantha_sdk/api/answers.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.3.2/semantha_sdk/api/bulk.py` & `semantha_sdk-5.4.0/semantha_sdk/api/bulk.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.3.2/semantha_sdk/api/bulk_domains.py` & `semantha_sdk-5.4.0/semantha_sdk/api/bulk_domains.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.3.2/semantha_sdk/api/bulk_model.py` & `semantha_sdk-5.4.0/semantha_sdk/api/bulk_model.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.3.2/semantha_sdk/api/bulkdomains_documentclasses.py` & `semantha_sdk-5.4.0/semantha_sdk/api/bulkdomains_documentclasses.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.3.2/semantha_sdk/api/bulkdomains_domain.py` & `semantha_sdk-5.4.0/semantha_sdk/api/bulkdomains_domain.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.3.2/semantha_sdk/api/bulkdomains_referencedocuments.py` & `semantha_sdk-5.4.0/semantha_sdk/api/bulkdomains_referencedocuments.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.3.2/semantha_sdk/api/bulkdomains_references.py` & `semantha_sdk-5.4.0/semantha_sdk/api/bulkdomains_references.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.3.2/semantha_sdk/api/bulkmodel_boostwords.py` & `semantha_sdk-5.4.0/semantha_sdk/api/bulkmodel_boostwords.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.3.2/semantha_sdk/api/bulkmodel_class.py` & `semantha_sdk-5.4.0/semantha_sdk/api/bulkmodel_class.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.3.2/semantha_sdk/api/bulkmodel_classes.py` & `semantha_sdk-5.4.0/semantha_sdk/api/bulkmodel_classes.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.3.2/semantha_sdk/api/bulkmodel_dataproperties.py` & `semantha_sdk-5.4.0/semantha_sdk/api/bulkmodel_dataproperties.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.3.2/semantha_sdk/api/bulkmodel_domain.py` & `semantha_sdk-5.4.0/semantha_sdk/api/bulkmodel_domain.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.3.2/semantha_sdk/api/bulkmodel_domains.py` & `semantha_sdk-5.4.0/semantha_sdk/api/bulkmodel_domains.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.3.2/semantha_sdk/api/bulkmodel_instances.py` & `semantha_sdk-5.4.0/semantha_sdk/api/bulkmodel_instances.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.3.2/semantha_sdk/api/bulkmodel_metadata.py` & `semantha_sdk-5.4.0/semantha_sdk/api/bulkmodel_metadata.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.3.2/semantha_sdk/api/bulkmodel_namedentities.py` & `semantha_sdk-5.4.0/semantha_sdk/api/bulkmodel_namedentities.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.3.2/semantha_sdk/api/bulkmodel_stopwords.py` & `semantha_sdk-5.4.0/semantha_sdk/api/bulkmodel_stopwords.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.3.2/semantha_sdk/api/bulkmodel_synonyms.py` & `semantha_sdk-5.4.0/semantha_sdk/api/bulkmodel_synonyms.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.3.2/semantha_sdk/api/bulkmodelclass_instances.py` & `semantha_sdk-5.4.0/semantha_sdk/api/bulkmodelclass_instances.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.3.2/semantha_sdk/api/clusters.py` & `semantha_sdk-5.4.0/semantha_sdk/api/clusters.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.3.2/semantha_sdk/api/currentuser.py` & `semantha_sdk-5.4.0/semantha_sdk/api/currentuser.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.3.2/semantha_sdk/api/diff.py` & `semantha_sdk-5.4.0/semantha_sdk/api/diff.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.3.2/semantha_sdk/api/documentannotations.py` & `semantha_sdk-5.4.0/semantha_sdk/api/documentannotations.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.3.2/semantha_sdk/api/documentclass.py` & `semantha_sdk-5.4.0/semantha_sdk/api/documentclass.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.3.2/semantha_sdk/api/documentclasses.py` & `semantha_sdk-5.4.0/semantha_sdk/api/documentclasses.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.3.2/semantha_sdk/api/documentcomparisons.py` & `semantha_sdk-5.4.0/semantha_sdk/api/documentcomparisons.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.3.2/semantha_sdk/api/documents.py` & `semantha_sdk-5.4.0/semantha_sdk/api/documents.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.3.2/semantha_sdk/api/domain.py` & `semantha_sdk-5.4.0/semantha_sdk/api/domain.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from semantha_sdk.api.modelclasses import ModelclassesEndpoint
 from semantha_sdk.api.modelinstances import ModelinstancesEndpoint
 from semantha_sdk.api.referencedocuments import ReferencedocumentsEndpoint
 from semantha_sdk.api.references import ReferencesEndpoint
 from semantha_sdk.api.semantha_endpoint import SemanthaAPIEndpoint
 from semantha_sdk.api.settings import SettingsEndpoint
 from semantha_sdk.api.similaritymatrix import SimilaritymatrixEndpoint
+from semantha_sdk.api.summarizations import SummarizationsEndpoint
 from semantha_sdk.api.tags import TagsEndpoint
 from semantha_sdk.api.validation import ValidationEndpoint
 from semantha_sdk.model.domain import Domain, DomainSchema
 from semantha_sdk.rest.rest_client import RestClient
 
 
 class DomainEndpoint(SemanthaAPIEndpoint):
@@ -44,14 +45,15 @@
         self.__documents = DocumentsEndpoint(session, self._endpoint)
         self.__modelclasses = ModelclassesEndpoint(session, self._endpoint)
         self.__modelinstances = ModelinstancesEndpoint(session, self._endpoint)
         self.__referencedocuments = ReferencedocumentsEndpoint(session, self._endpoint)
         self.__references = ReferencesEndpoint(session, self._endpoint)
         self.__settings = SettingsEndpoint(session, self._endpoint)
         self.__similaritymatrix = SimilaritymatrixEndpoint(session, self._endpoint)
+        self.__summarizations = SummarizationsEndpoint(session, self._endpoint)
         self.__tags = TagsEndpoint(session, self._endpoint)
         self.__validation = ValidationEndpoint(session, self._endpoint)
 
 
     @property
     def answers(self) -> AnswersEndpoint:
         return self.__answers
@@ -104,14 +106,19 @@
 
     @property
     def similaritymatrix(self) -> SimilaritymatrixEndpoint:
         return self.__similaritymatrix
 
 
     @property
+    def summarizations(self) -> SummarizationsEndpoint:
+        return self.__summarizations
+
+
+    @property
     def tags(self) -> TagsEndpoint:
         return self.__tags
 
 
     @property
     def validation(self) -> ValidationEndpoint:
         return self.__validation
```

### Comparing `semantha_sdk-5.3.2/semantha_sdk/api/domains.py` & `semantha_sdk-5.4.0/semantha_sdk/api/domains.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.3.2/semantha_sdk/api/info.py` & `semantha_sdk-5.4.0/semantha_sdk/api/info.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.3.2/semantha_sdk/api/languages.py` & `semantha_sdk-5.4.0/semantha_sdk/api/languages.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.3.2/semantha_sdk/api/model.py` & `semantha_sdk-5.4.0/semantha_sdk/api/model.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.3.2/semantha_sdk/api/model_boostwords.py` & `semantha_sdk-5.4.0/semantha_sdk/api/model_boostwords.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from semantha_sdk.api.model_boostword import ModelBoostwordEndpoint
 from semantha_sdk.api.semantha_endpoint import SemanthaAPIEndpoint
 from semantha_sdk.model.boost_word import BoostWord, BoostWordSchema
 from semantha_sdk.rest.rest_client import MediaType
 from semantha_sdk.rest.rest_client import RestClient
 from typing import List
 
 
@@ -47,7 +48,12 @@
         """
         self._session.delete(self._endpoint).execute()
 
     def __init__(self, session: RestClient, parent_endpoint: str) -> None:
         super().__init__(session, parent_endpoint)
 
 
+
+    def __call__(self, id: str) -> ModelBoostwordEndpoint:
+        return ModelBoostwordEndpoint(self._session, self._endpoint, id)
+
+
```

### Comparing `semantha_sdk-5.3.2/semantha_sdk/api/model_datatypes.py` & `semantha_sdk-5.4.0/semantha_sdk/api/model_datatypes.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.3.2/semantha_sdk/api/model_domain.py` & `semantha_sdk-5.4.0/semantha_sdk/api/model_domain.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 from io import IOBase
 from semantha_sdk.api.model_boostwords import ModelBoostwordsEndpoint
+from semantha_sdk.api.model_namedentities import ModelNamedentitiesEndpoint
+from semantha_sdk.api.model_stopwords import ModelStopwordsEndpoint
 from semantha_sdk.api.model_synonyms import ModelSynonymsEndpoint
 from semantha_sdk.api.semantha_endpoint import SemanthaAPIEndpoint
 from semantha_sdk.rest.rest_client import RestClient
 
 
 class ModelDomainEndpoint(SemanthaAPIEndpoint):
     """ author semantha, this is a generated class do not change manually! """
@@ -32,19 +34,31 @@
         )
 
 
     def __init__(self, session: RestClient, parent_endpoint: str, domainname: str) -> None:
         super().__init__(session, parent_endpoint)
         self._domainname=domainname
         self.__boostwords = ModelBoostwordsEndpoint(session, self._endpoint)
+        self.__namedentities = ModelNamedentitiesEndpoint(session, self._endpoint)
+        self.__stopwords = ModelStopwordsEndpoint(session, self._endpoint)
         self.__synonyms = ModelSynonymsEndpoint(session, self._endpoint)
 
 
     @property
     def boostwords(self) -> ModelBoostwordsEndpoint:
         return self.__boostwords
 
 
     @property
+    def namedentities(self) -> ModelNamedentitiesEndpoint:
+        return self.__namedentities
+
+
+    @property
+    def stopwords(self) -> ModelStopwordsEndpoint:
+        return self.__stopwords
+
+
+    @property
     def synonyms(self) -> ModelSynonymsEndpoint:
         return self.__synonyms
```

### Comparing `semantha_sdk-5.3.2/semantha_sdk/api/model_domains.py` & `semantha_sdk-5.4.0/semantha_sdk/api/model_domains.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.3.2/semantha_sdk/api/model_extractortypes.py` & `semantha_sdk-5.4.0/semantha_sdk/api/model_extractortypes.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.3.2/semantha_sdk/api/model_metadatatypes.py` & `semantha_sdk-5.4.0/semantha_sdk/api/model_metadatatypes.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.3.2/semantha_sdk/api/model_synonyms.py` & `semantha_sdk-5.4.0/semantha_sdk/api/model_synonyms.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from semantha_sdk.api.model_synonym import ModelSynonymEndpoint
 from semantha_sdk.api.semantha_endpoint import SemanthaAPIEndpoint
 from semantha_sdk.model.synonym import Synonym, SynonymSchema
 from semantha_sdk.rest.rest_client import MediaType
 from semantha_sdk.rest.rest_client import RestClient
 from typing import List
 
 
@@ -47,7 +48,12 @@
         """
         self._session.delete(self._endpoint).execute()
 
     def __init__(self, session: RestClient, parent_endpoint: str) -> None:
         super().__init__(session, parent_endpoint)
 
 
+
+    def __call__(self, id: str) -> ModelSynonymEndpoint:
+        return ModelSynonymEndpoint(self._session, self._endpoint, id)
+
+
```

### Comparing `semantha_sdk-5.3.2/semantha_sdk/api/modelclasses.py` & `semantha_sdk-5.4.0/semantha_sdk/api/modelclasses.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.3.2/semantha_sdk/api/modelinstances.py` & `semantha_sdk-5.4.0/semantha_sdk/api/modelinstances.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.3.2/semantha_sdk/api/namedentities.py` & `semantha_sdk-5.4.0/semantha_sdk/api/namedentities.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.3.2/semantha_sdk/api/paragraph.py` & `semantha_sdk-5.4.0/semantha_sdk/api/paragraph.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.3.2/semantha_sdk/api/paragraphs.py` & `semantha_sdk-5.4.0/semantha_sdk/api/paragraphs.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.3.2/semantha_sdk/api/referencedocument.py` & `semantha_sdk-5.4.0/semantha_sdk/api/referencedocument.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.3.2/semantha_sdk/api/referencedocuments.py` & `semantha_sdk-5.4.0/semantha_sdk/api/referencedocuments.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.3.2/semantha_sdk/api/references.py` & `semantha_sdk-5.4.0/semantha_sdk/api/references.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.3.2/semantha_sdk/api/roles.py` & `semantha_sdk-5.4.0/semantha_sdk/api/roles.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.3.2/semantha_sdk/api/semantha_api.py` & `semantha_sdk-5.4.0/semantha_sdk/api/semantha_api.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.3.2/semantha_sdk/api/sentence.py` & `semantha_sdk-5.4.0/semantha_sdk/api/sentence.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.3.2/semantha_sdk/api/sentences.py` & `semantha_sdk-5.4.0/semantha_sdk/api/sentences.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.3.2/semantha_sdk/api/settings.py` & `semantha_sdk-5.4.0/semantha_sdk/api/settings.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.3.2/semantha_sdk/api/similaritymatrix.py` & `semantha_sdk-5.4.0/semantha_sdk/api/similaritymatrix.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.3.2/semantha_sdk/api/similaritymatrix_cluster.py` & `semantha_sdk-5.4.0/semantha_sdk/api/similaritymatrix_cluster.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.3.2/semantha_sdk/api/statistic.py` & `semantha_sdk-5.4.0/semantha_sdk/api/statistic.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.3.2/semantha_sdk/api/tag.py` & `semantha_sdk-5.4.0/semantha_sdk/api/tag.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.3.2/semantha_sdk/api/tag_referencedocuments.py` & `semantha_sdk-5.4.0/semantha_sdk/api/tag_referencedocuments.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.3.2/semantha_sdk/api/tags.py` & `semantha_sdk-5.4.0/semantha_sdk/api/tags.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.3.2/semantha_sdk/api/validation.py` & `semantha_sdk-5.4.0/semantha_sdk/api/validation.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.3.2/semantha_sdk/model/__init__.py` & `semantha_sdk-5.4.0/semantha_sdk/model/__init__.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.3.2/semantha_sdk/model/annotation_cell.py` & `semantha_sdk-5.4.0/semantha_sdk/model/annotation_cell.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.3.2/semantha_sdk/model/annotation_page.py` & `semantha_sdk-5.4.0/semantha_sdk/model/annotation_page.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.3.2/semantha_sdk/model/answer.py` & `semantha_sdk-5.4.0/semantha_sdk/model/answer.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.3.2/semantha_sdk/model/answer_reference.py` & `semantha_sdk-5.4.0/semantha_sdk/model/answer_reference.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.3.2/semantha_sdk/model/boost_word.py` & `semantha_sdk-5.4.0/semantha_sdk/model/boost_word.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.3.2/semantha_sdk/model/class_bulk.py` & `semantha_sdk-5.4.0/semantha_sdk/model/class_bulk.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.3.2/semantha_sdk/model/clustering_response.py` & `semantha_sdk-5.4.0/semantha_sdk/model/clustering_response.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.3.2/semantha_sdk/model/complex_property.py` & `semantha_sdk-5.4.0/semantha_sdk/model/complex_property.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.3.2/semantha_sdk/model/current_user.py` & `semantha_sdk-5.4.0/semantha_sdk/model/current_user.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.3.2/semantha_sdk/model/data_property.py` & `semantha_sdk-5.4.0/semantha_sdk/model/data_property.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.3.2/semantha_sdk/model/distance.py` & `semantha_sdk-5.4.0/semantha_sdk/model/distance.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.3.2/semantha_sdk/model/document.py` & `semantha_sdk-5.4.0/semantha_sdk/model/document.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.3.2/semantha_sdk/model/document_class.py` & `semantha_sdk-5.4.0/semantha_sdk/model/document_class.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.3.2/semantha_sdk/model/document_class_bulk.py` & `semantha_sdk-5.4.0/semantha_sdk/model/document_class_bulk.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.3.2/semantha_sdk/model/document_class_node.py` & `semantha_sdk-5.4.0/semantha_sdk/model/document_class_node.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.3.2/semantha_sdk/model/document_cluster.py` & `semantha_sdk-5.4.0/semantha_sdk/model/document_cluster.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.3.2/semantha_sdk/model/document_information.py` & `semantha_sdk-5.4.0/semantha_sdk/model/document_information.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.3.2/semantha_sdk/model/domain.py` & `semantha_sdk-5.4.0/semantha_sdk/model/domain.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.3.2/semantha_sdk/model/extraction_area.py` & `semantha_sdk-5.4.0/semantha_sdk/model/extraction_area.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.3.2/semantha_sdk/model/extraction_file.py` & `semantha_sdk-5.4.0/semantha_sdk/model/extraction_file.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.3.2/semantha_sdk/model/extraction_reference.py` & `semantha_sdk-5.4.0/semantha_sdk/model/extraction_reference.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.3.2/semantha_sdk/model/features.py` & `semantha_sdk-5.4.0/semantha_sdk/model/features.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.3.2/semantha_sdk/model/file_reference.py` & `semantha_sdk-5.4.0/semantha_sdk/model/file_reference.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.3.2/semantha_sdk/model/info.py` & `semantha_sdk-5.4.0/semantha_sdk/model/info.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.3.2/semantha_sdk/model/instance.py` & `semantha_sdk-5.4.0/semantha_sdk/model/instance.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.3.2/semantha_sdk/model/instance_child.py` & `semantha_sdk-5.4.0/semantha_sdk/model/instance_child.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.3.2/semantha_sdk/model/linked_instance.py` & `semantha_sdk-5.4.0/semantha_sdk/model/linked_instance.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.3.2/semantha_sdk/model/matrix_row.py` & `semantha_sdk-5.4.0/semantha_sdk/model/matrix_row.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.3.2/semantha_sdk/model/model_class.py` & `semantha_sdk-5.4.0/semantha_sdk/model/model_class.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.3.2/semantha_sdk/model/model_instance.py` & `semantha_sdk-5.4.0/semantha_sdk/model/model_instance.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.3.2/semantha_sdk/model/page.py` & `semantha_sdk-5.4.0/semantha_sdk/model/page.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.3.2/semantha_sdk/model/page_content.py` & `semantha_sdk-5.4.0/semantha_sdk/model/page_content.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.3.2/semantha_sdk/model/paragraph.py` & `semantha_sdk-5.4.0/semantha_sdk/model/paragraph.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.3.2/semantha_sdk/model/process_information.py` & `semantha_sdk-5.4.0/semantha_sdk/model/process_information.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.3.2/semantha_sdk/model/reference.py` & `semantha_sdk-5.4.0/semantha_sdk/model/reference.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.3.2/semantha_sdk/model/reference_documents_response_container.py` & `semantha_sdk-5.4.0/semantha_sdk/model/reference_documents_response_container.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.3.2/semantha_sdk/model/response_meta_info.py` & `semantha_sdk-5.4.0/semantha_sdk/model/response_meta_info.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.3.2/semantha_sdk/model/semantha_entity.py` & `semantha_sdk-5.4.0/semantha_sdk/model/semantha_entity.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.3.2/semantha_sdk/model/semantic_model.py` & `semantha_sdk-5.4.0/semantha_sdk/model/semantic_model.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.3.2/semantha_sdk/model/semi_super_vised_document.py` & `semantha_sdk-5.4.0/semantha_sdk/model/semi_super_vised_document.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.3.2/semantha_sdk/model/sentence.py` & `semantha_sdk-5.4.0/semantha_sdk/model/sentence.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.3.2/semantha_sdk/model/settings.py` & `semantha_sdk-5.4.0/semantha_sdk/model/settings.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.3.2/semantha_sdk/model/smart_cluster_response_container.py` & `semantha_sdk-5.4.0/semantha_sdk/model/smart_cluster_response_container.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.3.2/semantha_sdk/model/smart_cluster_semi_supervised_request.py` & `semantha_sdk-5.4.0/semantha_sdk/model/smart_cluster_semi_supervised_request.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.3.2/semantha_sdk/model/statistic.py` & `semantha_sdk-5.4.0/semantha_sdk/model/statistic.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.3.2/semantha_sdk/model/synonym.py` & `semantha_sdk-5.4.0/semantha_sdk/model/synonym.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.3.2/semantha_sdk/model/table_instance.py` & `semantha_sdk-5.4.0/semantha_sdk/model/table_instance.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.3.2/semantha_sdk/request/semantha_request.py` & `semantha_sdk-5.4.0/semantha_sdk/request/semantha_request.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.3.2/semantha_sdk/response/semantha_response.py` & `semantha_sdk-5.4.0/semantha_sdk/response/semantha_response.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-5.3.2/semantha_sdk/rest/rest_client.py` & `semantha_sdk-5.4.0/semantha_sdk/rest/rest_client.py`

 * *Files identical despite different names*

