# Comparing `tmp/deepsearch_toolkit-0.8.0.tar.gz` & `tmp/deepsearch_toolkit-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deepsearch_toolkit-0.8.0.tar", max compression
+gzip compressed data, was "deepsearch_toolkit-0.9.0.tar", max compression
```

## Comparing `deepsearch_toolkit-0.8.0.tar` & `deepsearch_toolkit-0.9.0.tar`

### file list

```diff
@@ -1,435 +1,435 @@
--rw-r--r--   0        0        0     1088 2023-01-06 13:47:35.271094 deepsearch_toolkit-0.8.0/LICENSE
--rw-r--r--   0        0        0     3100 2023-01-06 13:47:35.271094 deepsearch_toolkit-0.8.0/README.md
--rw-r--r--   0        0        0      263 2023-01-06 13:47:35.271094 deepsearch_toolkit-0.8.0/deepsearch/__init__.py
--rw-r--r--   0        0        0      671 2023-01-06 13:47:35.271094 deepsearch_toolkit-0.8.0/deepsearch/cli.py
--rw-r--r--   0        0        0       22 2023-01-06 13:47:35.271094 deepsearch_toolkit-0.8.0/deepsearch/core/__init__.py
--rw-r--r--   0        0        0        0 2023-01-06 13:47:35.271094 deepsearch_toolkit-0.8.0/deepsearch/core/cli/__init__.py
--rw-r--r--   0        0        0      745 2023-01-06 13:47:35.271094 deepsearch_toolkit-0.8.0/deepsearch/core/cli/config.py
--rw-r--r--   0        0        0     1267 2023-01-06 13:47:35.271094 deepsearch_toolkit-0.8.0/deepsearch/core/cli/login.py
--rw-r--r--   0        0        0      577 2023-01-06 13:47:35.271094 deepsearch_toolkit-0.8.0/deepsearch/core/cli/main.py
--rw-r--r--   0        0        0     1000 2023-01-06 13:47:35.271094 deepsearch_toolkit-0.8.0/deepsearch/core/cli/plugins.py
--rw-r--r--   0        0        0       83 2023-01-06 13:47:35.271094 deepsearch_toolkit-0.8.0/deepsearch/core/client/__init__.py
--rw-r--r--   0        0        0      373 2023-01-06 13:47:35.271094 deepsearch_toolkit-0.8.0/deepsearch/core/client/config.py
--rw-r--r--   0        0        0        0 2023-01-06 13:47:35.271094 deepsearch_toolkit-0.8.0/deepsearch/core/util/__init__.py
--rw-r--r--   0        0        0      457 2023-01-06 13:47:35.271094 deepsearch_toolkit-0.8.0/deepsearch/core/util/_version.py
--rw-r--r--   0        0        0      560 2023-01-06 13:47:35.271094 deepsearch_toolkit-0.8.0/deepsearch/core/util/ccs_utils.py
--rw-r--r--   0        0        0      487 2023-01-06 13:47:35.271094 deepsearch_toolkit-0.8.0/deepsearch/core/util/cli_output.py
--rw-r--r--   0        0        0     1391 2023-01-06 13:47:35.271094 deepsearch_toolkit-0.8.0/deepsearch/core/util/config_paths.py
--rw-r--r--   0        0        0       79 2023-01-06 13:47:35.271094 deepsearch_toolkit-0.8.0/deepsearch/cps/__init__.py
--rw-r--r--   0        0        0       26 2023-01-06 13:47:35.271094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/.gitattributes
--rw-r--r--   0        0        0       89 2023-01-06 13:47:35.271094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/README.md
--rw-r--r--   0        0        0        0 2023-01-06 13:47:35.271094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/__init__.py
--rw-r--r--   0        0        0        0 2023-01-06 13:47:35.271094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/kg/__init__.py
--rw-r--r--   0        0        0     2347 2023-01-06 13:47:35.271094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/kg/create/__init__.py
--rw-r--r--   0        0        0      437 2023-01-06 13:47:35.271094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/kg/create/api/__init__.py
--rw-r--r--   0        0        0    42138 2023-01-06 13:47:35.271094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/kg/create/api/edges_api.py
--rw-r--r--   0        0        0     6763 2023-01-06 13:47:35.271094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/kg/create/api/indices_api.py
--rw-r--r--   0        0        0    35757 2023-01-06 13:47:35.271094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/kg/create/api/knowledge_graphs_api.py
--rw-r--r--   0        0        0    18521 2023-01-06 13:47:35.271094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/kg/create/api/nodes_api.py
--rw-r--r--   0        0        0    10807 2023-01-06 13:47:35.271094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/kg/create/api/tasks_api.py
--rw-r--r--   0        0        0    26333 2023-01-06 13:47:35.271094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/kg/create/api_client.py
--rw-r--r--   0        0        0    13351 2023-01-06 13:47:35.271094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/kg/create/configuration.py
--rw-r--r--   0        0        0     3803 2023-01-06 13:47:35.271094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/kg/create/exceptions.py
--rw-r--r--   0        0        0     1456 2023-01-06 13:47:35.271094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/kg/create/models/__init__.py
--rw-r--r--   0        0        0     6487 2023-01-06 13:47:35.271094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/kg/create/models/database_source.py
--rw-r--r--   0        0        0     4321 2023-01-06 13:47:35.271094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/kg/create/models/database_source_mongo.py
--rw-r--r--   0        0        0     7453 2023-01-06 13:47:35.271094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/kg/create/models/database_source_s3.py
--rw-r--r--   0        0        0     4243 2023-01-06 13:47:35.271094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/kg/create/models/edge_matrix.py
--rw-r--r--   0        0        0     5932 2023-01-06 13:47:35.271094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/kg/create/models/edge_model.py
--rw-r--r--   0        0        0     5011 2023-01-06 13:47:35.271094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/kg/create/models/inline_object.py
--rw-r--r--   0        0        0     5027 2023-01-06 13:47:35.271094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/kg/create/models/inline_object1.py
--rw-r--r--   0        0        0     5027 2023-01-06 13:47:35.271094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/kg/create/models/inline_object2.py
--rw-r--r--   0        0        0     5705 2023-01-06 13:47:35.271094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/kg/create/models/mongo_edge.py
--rw-r--r--   0        0        0     4330 2023-01-06 13:47:35.271094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/kg/create/models/mongo_edge_item.py
--rw-r--r--   0        0        0     5884 2023-01-06 13:47:35.271094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/kg/create/models/node.py
--rw-r--r--   0        0        0     7719 2023-01-06 13:47:35.271094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/kg/create/models/s3_source.py
--rw-r--r--   0        0        0     4897 2023-01-06 13:47:35.271094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/kg/create/models/sparse_matrix_with_names_or_hashes.py
--rw-r--r--   0        0        0     4491 2023-01-06 13:47:35.275094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/kg/create/models/triplet.py
--rw-r--r--   0        0        0    12350 2023-01-06 13:47:35.275094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/kg/create/rest.py
--rw-r--r--   0        0        0     2820 2023-01-06 13:47:35.275094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/kg/query/__init__.py
--rw-r--r--   0        0        0      541 2023-01-06 13:47:35.275094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/kg/query/api/__init__.py
--rw-r--r--   0        0        0    18088 2023-01-06 13:47:35.275094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/kg/query/api/description_api.py
--rw-r--r--   0        0        0    13270 2023-01-06 13:47:35.275094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/kg/query/api/inspect_api.py
--rw-r--r--   0        0        0    44595 2023-01-06 13:47:35.275094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/kg/query/api/node_data_retrieval_api.py
--rw-r--r--   0        0        0    23175 2023-01-06 13:47:35.275094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/kg/query/api/node_retrieval_api.py
--rw-r--r--   0        0        0    14635 2023-01-06 13:47:35.275094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/kg/query/api/node_search_api.py
--rw-r--r--   0        0        0    53227 2023-01-06 13:47:35.275094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/kg/query/api/query_api.py
--rw-r--r--   0        0        0    26327 2023-01-06 13:47:35.275094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/kg/query/api_client.py
--rw-r--r--   0        0        0    13332 2023-01-06 13:47:35.275094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/kg/query/configuration.py
--rw-r--r--   0        0        0     3802 2023-01-06 13:47:35.275094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/kg/query/exceptions.py
--rw-r--r--   0        0        0     1832 2023-01-06 13:47:35.275094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/kg/query/models/__init__.py
--rw-r--r--   0        0        0     4060 2023-01-06 13:47:35.275094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/kg/query/models/auth_config.py
--rw-r--r--   0        0        0     5234 2023-01-06 13:47:35.275094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/kg/query/models/error_model.py
--rw-r--r--   0        0        0     4692 2023-01-06 13:47:35.275094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/kg/query/models/graph_description.py
--rw-r--r--   0        0        0     5806 2023-01-06 13:47:35.275094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/kg/query/models/graph_edge.py
--rw-r--r--   0        0        0     6110 2023-01-06 13:47:35.275094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/kg/query/models/graph_matrix.py
--rw-r--r--   0        0        0     4948 2023-01-06 13:47:35.275094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/kg/query/models/graph_node_description.py
--rw-r--r--   0        0        0     4847 2023-01-06 13:47:35.275094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/kg/query/models/graph_node_description_categories.py
--rw-r--r--   0        0        0     5151 2023-01-06 13:47:35.275094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/kg/query/models/inline_object.py
--rw-r--r--   0        0        0     5882 2023-01-06 13:47:35.275094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/kg/query/models/node.py
--rw-r--r--   0        0        0     2734 2023-01-06 13:47:35.275094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/kg/query/models/nodes_response_model.py
--rw-r--r--   0        0        0     4607 2023-01-06 13:47:35.275094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/kg/query/models/nodes_response_model_all_of.py
--rw-r--r--   0        0        0     3635 2023-01-06 13:47:35.275094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/kg/query/models/nodes_response_model_all_of_response.py
--rw-r--r--   0        0        0     5045 2023-01-06 13:47:35.275094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/kg/query/models/response_model.py
--rw-r--r--   0        0        0     4922 2023-01-06 13:47:35.275094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/kg/query/models/workflow_response.py
--rw-r--r--   0        0        0     2746 2023-01-06 13:47:35.275094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/kg/query/models/workflow_response_model.py
--rw-r--r--   0        0        0     4604 2023-01-06 13:47:35.275094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/kg/query/models/workflow_response_model_all_of.py
--rw-r--r--   0        0        0     6662 2023-01-06 13:47:35.275094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/kg/query/models/workflow_response_node.py
--rw-r--r--   0        0        0    12348 2023-01-06 13:47:35.275094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/kg/query/rest.py
--rw-r--r--   0        0        0    28378 2023-01-06 13:47:35.275094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/__init__.py
--rw-r--r--   0        0        0     1124 2023-01-06 13:47:35.275094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/api/__init__.py
--rw-r--r--   0        0        0    32396 2023-01-06 13:47:35.275094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/api/annotate_api.py
--rw-r--r--   0        0        0   170020 2023-01-06 13:47:35.275094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/api/data_catalogs_api.py
--rw-r--r--   0        0        0   131553 2023-01-06 13:47:35.275094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/api/data_flows_api.py
--rw-r--r--   0        0        0    57195 2023-01-06 13:47:35.275094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/api/data_indices_api.py
--rw-r--r--   0        0        0   133861 2023-01-06 13:47:35.275094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/api/dictionaries_api.py
--rw-r--r--   0        0        0    25396 2023-01-06 13:47:35.275094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/api/document_annotation_api.py
--rw-r--r--   0        0        0    34436 2023-01-06 13:47:35.275094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/api/elastic_api.py
--rw-r--r--   0        0        0   200606 2023-01-06 13:47:35.279094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/api/knowledge_graphs_api.py
--rw-r--r--   0        0        0    46122 2023-01-06 13:47:35.279094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/api/model_configurations_api.py
--rw-r--r--   0        0        0    10605 2023-01-06 13:47:35.279094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/api/processing_model_api.py
--rw-r--r--   0        0        0    17431 2023-01-06 13:47:35.279094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/api/project_api.py
--rw-r--r--   0        0        0   116434 2023-01-06 13:47:35.279094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/api/system_api.py
--rw-r--r--   0        0        0    36829 2023-01-06 13:47:35.279094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/api/tasks_api.py
--rw-r--r--   0        0        0    25072 2023-01-06 13:47:35.279094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/api/uploads_api.py
--rw-r--r--   0        0        0    26327 2023-01-06 13:47:35.279094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/api_client.py
--rw-r--r--   0        0        0    13946 2023-01-06 13:47:35.279094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/configuration.py
--rw-r--r--   0        0        0     3812 2023-01-06 13:47:35.279094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/exceptions.py
--rw-r--r--   0        0        0    26821 2023-01-06 13:47:35.279094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/__init__.py
--rw-r--r--   0        0        0     7657 2023-01-06 13:47:35.279094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/annotate_document_request.py
--rw-r--r--   0        0        0     4510 2023-01-06 13:47:35.279094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/annotate_object_options.py
--rw-r--r--   0        0        0     6736 2023-01-06 13:47:35.279094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/annotate_object_options1.py
--rw-r--r--   0        0        0     6978 2023-01-06 13:47:35.279094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/annotated_document_report.py
--rw-r--r--   0        0        0     6086 2023-01-06 13:47:35.279094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/annotated_image.py
--rw-r--r--   0        0        0     4648 2023-01-06 13:47:35.279094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/annotated_object.py
--rw-r--r--   0        0        0     4664 2023-01-06 13:47:35.279094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/annotated_object1.py
--rw-r--r--   0        0        0     6086 2023-01-06 13:47:35.279094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/annotated_table.py
--rw-r--r--   0        0        0     6220 2023-01-06 13:47:35.279094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/annotated_text.py
--rw-r--r--   0        0        0     6992 2023-01-06 13:47:35.279094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/annotated_text_lines.py
--rw-r--r--   0        0        0     4286 2023-01-06 13:47:35.279094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/annotator_image_input.py
--rw-r--r--   0        0        0     5165 2023-01-06 13:47:35.279094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/annotator_input.py
--rw-r--r--   0        0        0     6724 2023-01-06 13:47:35.279094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/annotator_metadata.py
--rw-r--r--   0        0        0     5629 2023-01-06 13:47:35.279094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/annotator_parameters_or_ref.py
--rw-r--r--   0        0        0     4744 2023-01-06 13:47:35.279094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/annotator_supported_annotations_parameters.py
--rw-r--r--   0        0        0     5871 2023-01-06 13:47:35.279094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/assemble_data_flow_into_knowledge_graph_options.py
--rw-r--r--   0        0        0     5851 2023-01-06 13:47:35.279094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/assemble_data_flow_into_knowledge_graph_options1.py
--rw-r--r--   0        0        0     4136 2023-01-06 13:47:35.279094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/backend_flavour.py
--rw-r--r--   0        0        0     7053 2023-01-06 13:47:35.279094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/backend_project_proj_key_bags_bag_key_tasks_assemble_dataflow_data_flow.py
--rw-r--r--   0        0        0     5168 2023-01-06 13:47:35.279094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/backend_project_proj_key_bags_bag_key_tasks_assemble_dataflow_data_flow_raw_data_flow.py
--rw-r--r--   0        0        0     3964 2023-01-06 13:47:35.279094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/backend_project_proj_key_bags_bag_key_tasks_assemble_dataflow_render.py
--rw-r--r--   0        0        0     4364 2023-01-06 13:47:35.279094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/backup_knowledge_graph_options.py
--rw-r--r--   0        0        0    11072 2023-01-06 13:47:35.279094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/bag.py
--rw-r--r--   0        0        0     3371 2023-01-06 13:47:35.279094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/bag_amqp_backend.py
--rw-r--r--   0        0        0    10166 2023-01-06 13:47:35.279094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/bag_backend_aware.py
--rw-r--r--   0        0        0     4187 2023-01-06 13:47:35.279094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/bag_backends.py
--rw-r--r--   0        0        0     3447 2023-01-06 13:47:35.279094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/bag_callback.py
--rw-r--r--   0        0        0     4284 2023-01-06 13:47:35.279094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/bag_component_status.py
--rw-r--r--   0        0        0     3309 2023-01-06 13:47:35.279094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/bag_component_status_enum.py
--rw-r--r--   0        0        0     4717 2023-01-06 13:47:35.279094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/bag_flavour.py
--rw-r--r--   0        0        0     5271 2023-01-06 13:47:35.279094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/bag_flavour_default_quota.py
--rw-r--r--   0        0        0    10094 2023-01-06 13:47:35.279094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/bag_flavour_full_data.py
--rw-r--r--   0        0        0     6240 2023-01-06 13:47:35.279094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/bag_kg_legacy_api_backend.py
--rw-r--r--   0        0        0     4417 2023-01-06 13:47:35.279094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/bag_status.py
--rw-r--r--   0        0        0     5344 2023-01-06 13:47:35.279094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/bag_status_backend_aware.py
--rw-r--r--   0        0        0     3668 2023-01-06 13:47:35.279094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/bag_status_backend_aware_kg_amqp.py
--rw-r--r--   0        0        0     5905 2023-01-06 13:47:35.279094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/bag_status_components.py
--rw-r--r--   0        0        0     5174 2023-01-06 13:47:35.279094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/catalog_reference.py
--rw-r--r--   0        0        0     5312 2023-01-06 13:47:35.279094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/ccs_collection_reference.py
--rw-r--r--   0        0        0     5440 2023-01-06 13:47:35.279094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/ccs_task.py
--rw-r--r--   0        0        0     5215 2023-01-06 13:47:35.279094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/celery_task.py
--rw-r--r--   0        0        0    12670 2023-01-06 13:47:35.279094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/celery_task1.py
--rw-r--r--   0        0        0     5061 2023-01-06 13:47:35.279094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/celery_task_promise.py
--rw-r--r--   0        0        0     6776 2023-01-06 13:47:35.279094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/clone_data_catalog_options.py
--rw-r--r--   0        0        0     4669 2023-01-06 13:47:35.279094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/clone_data_catalog_result.py
--rw-r--r--   0        0        0     6758 2023-01-06 13:47:35.279094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/clone_dictionary_options.py
--rw-r--r--   0        0        0     7985 2023-01-06 13:47:35.279094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/clone_public_data_catalog_options.py
--rw-r--r--   0        0        0     7667 2023-01-06 13:47:35.279094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/clone_public_dictionary_options.py
--rw-r--r--   0        0        0     3557 2023-01-06 13:47:35.279094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/collection_list_coordinates.py
--rw-r--r--   0        0        0     4576 2023-01-06 13:47:35.279094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/cps_model_reference.py
--rw-r--r--   0        0        0     7188 2023-01-06 13:47:35.279094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/cps_package.py
--rw-r--r--   0        0        0     4760 2023-01-06 13:47:35.279094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/create_collection_in_dictionary_options.py
--rw-r--r--   0        0        0     4714 2023-01-06 13:47:35.279094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/create_data_catalog_collection_options.py
--rw-r--r--   0        0        0     8354 2023-01-06 13:47:35.279094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/create_data_catalog_options.py
--rw-r--r--   0        0        0     7916 2023-01-06 13:47:35.279094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/create_data_flow_template_options.py
--rw-r--r--   0        0        0     5366 2023-01-06 13:47:35.279094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/create_dictionary_options.py
--rw-r--r--   0        0        0     7026 2023-01-06 13:47:35.283094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/create_knowledge_graph_options.py
--rw-r--r--   0        0        0     7003 2023-01-06 13:47:35.283094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/create_knowledge_graph_options1.py
--rw-r--r--   0        0        0     7515 2023-01-06 13:47:35.283094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/create_project_model_config_options.py
--rw-r--r--   0        0        0     4399 2023-01-06 13:47:35.283094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/data_catalog_category_schema.py
--rw-r--r--   0        0        0     4414 2023-01-06 13:47:35.283094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/data_catalog_collection.py
--rw-r--r--   0        0        0     4396 2023-01-06 13:47:35.283094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/data_catalog_data_flow.py
--rw-r--r--   0        0        0     4672 2023-01-06 13:47:35.283094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/data_catalog_import_options.py
--rw-r--r--   0        0        0     4702 2023-01-06 13:47:35.283094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/data_catalog_import_result.py
--rw-r--r--   0        0        0     6022 2023-01-06 13:47:35.283094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/data_catalog_provenance_log.py
--rw-r--r--   0        0        0     6858 2023-01-06 13:47:35.283094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/data_catalog_provenance_log_source.py
--rw-r--r--   0        0        0     5272 2023-01-06 13:47:35.283094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/data_catalog_provenance_log_user.py
--rw-r--r--   0        0        0     3972 2023-01-06 13:47:35.283094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/data_catalog_schema.py
--rw-r--r--   0        0        0     4567 2023-01-06 13:47:35.283094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/data_catalog_topology.py
--rw-r--r--   0        0        0     7093 2023-01-06 13:47:35.283094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/data_catalog_topology_edge.py
--rw-r--r--   0        0        0     4477 2023-01-06 13:47:35.283094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/data_catalog_topology_node.py
--rw-r--r--   0        0        0     4702 2023-01-06 13:47:35.283094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/data_catalog_url_import_options.py
--rw-r--r--   0        0        0    13804 2023-01-06 13:47:35.283094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/data_catalogue.py
--rw-r--r--   0        0        0     7433 2023-01-06 13:47:35.283094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/data_collection.py
--rw-r--r--   0        0        0     9288 2023-01-06 13:47:35.283094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/data_collection_metadata.py
--rw-r--r--   0        0        0     5036 2023-01-06 13:47:35.283094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/data_collection_source.py
--rw-r--r--   0        0        0     8617 2023-01-06 13:47:35.283094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/data_flow.py
--rw-r--r--   0        0        0     4540 2023-01-06 13:47:35.283094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/data_flow_assemble_into_knowledge_graph_task.py
--rw-r--r--   0        0        0     4372 2023-01-06 13:47:35.283094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/data_flow_assemble_report.py
--rw-r--r--   0        0        0     4081 2023-01-06 13:47:35.283094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/data_flow_assemble_report_cause.py
--rw-r--r--   0        0        0     6287 2023-01-06 13:47:35.283094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/data_flow_assemble_report_chunks.py
--rw-r--r--   0        0        0     4262 2023-01-06 13:47:35.283094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/data_flow_assemble_report_errors.py
--rw-r--r--   0        0        0     5357 2023-01-06 13:47:35.283094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/data_flow_assemble_report_options.py
--rw-r--r--   0        0        0     6557 2023-01-06 13:47:35.283094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/data_flow_assemble_report_single_task.py
--rw-r--r--   0        0        0     5166 2023-01-06 13:47:35.283094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/data_flow_load_into_knowledge_graph_task.py
--rw-r--r--   0        0        0     4411 2023-01-06 13:47:35.283094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/data_flow_template.py
--rw-r--r--   0        0        0     7776 2023-01-06 13:47:35.283094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/data_flow_template_list_item.py
--rw-r--r--   0        0        0     3653 2023-01-06 13:47:35.283094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/data_flow_template_variable.py
--rw-r--r--   0        0        0     3525 2023-01-06 13:47:35.283094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/data_flow_topology_options.py
--rw-r--r--   0        0        0     4760 2023-01-06 13:47:35.283094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/data_index_upload_file_source.py
--rw-r--r--   0        0        0     9559 2023-01-06 13:47:35.283094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/dictionary.py
--rw-r--r--   0        0        0     4244 2023-01-06 13:47:35.283094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/dictionary_clone_result.py
--rw-r--r--   0        0        0     4402 2023-01-06 13:47:35.283094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/dictionary_collection.py
--rw-r--r--   0        0        0     4402 2023-01-06 13:47:35.283094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/dictionary_collection_csv_data.py
--rw-r--r--   0        0        0     5944 2023-01-06 13:47:35.283094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/dictionary_collection_patch.py
--rw-r--r--   0        0        0     4320 2023-01-06 13:47:35.283094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/dictionary_entry.py
--rw-r--r--   0        0        0     4654 2023-01-06 13:47:35.283094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/dictionary_import_options.py
--rw-r--r--   0        0        0     4276 2023-01-06 13:47:35.283094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/dictionary_import_result.py
--rw-r--r--   0        0        0     5681 2023-01-06 13:47:35.283094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/elastic_coordinates.py
--rw-r--r--   0        0        0     7622 2023-01-06 13:47:35.283094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/elastic_index_search_query_options.py
--rw-r--r--   0        0        0     4899 2023-01-06 13:47:35.283094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/elastic_index_search_results.py
--rw-r--r--   0        0        0     5876 2023-01-06 13:47:35.283094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/entity_annotation.py
--rw-r--r--   0        0        0     5265 2023-01-06 13:47:35.283094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/entity_annotation_descriptor.py
--rw-r--r--   0        0        0     4308 2023-01-06 13:47:35.283094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/error_response.py
--rw-r--r--   0        0        0     4961 2023-01-06 13:47:35.283094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/flavours_quota.py
--rw-r--r--   0        0        0     4401 2023-01-06 13:47:35.283094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/fully_rendered_data_flow.py
--rw-r--r--   0        0        0     3620 2023-01-06 13:47:35.283094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/image_cells.py
--rw-r--r--   0        0        0     4219 2023-01-06 13:47:35.283094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/image_info.py
--rw-r--r--   0        0        0     4098 2023-01-06 13:47:35.283094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/image_metadata.py
--rw-r--r--   0        0        0     4613 2023-01-06 13:47:35.283094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/image_source.py
--rw-r--r--   0        0        0     5566 2023-01-06 13:47:35.283094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/import_from_elastic_to_data_catalog_options.py
--rw-r--r--   0        0        0     7503 2023-01-06 13:47:35.283094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/import_from_elastic_to_data_catalog_options_parameters.py
--rw-r--r--   0        0        0     5576 2023-01-06 13:47:35.283094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/import_from_elastic_to_data_catalog_options_parameters_query_options.py
--rw-r--r--   0        0        0    10951 2023-01-06 13:47:35.283094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/import_from_elastic_to_data_catalog_s3_coords.py
--rw-r--r--   0        0        0     5168 2023-01-06 13:47:35.283094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/import_to_data_catalog_collection_options.py
--rw-r--r--   0        0        0     4259 2023-01-06 13:47:35.283094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/import_to_data_catalog_options.py
--rw-r--r--   0        0        0     4176 2023-01-06 13:47:35.283094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/infer_project_data_catalog_category_schema.py
--rw-r--r--   0        0        0     3620 2023-01-06 13:47:35.283094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/inline_object.py
--rw-r--r--   0        0        0     8640 2023-01-06 13:47:35.283094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/inline_object1.py
--rw-r--r--   0        0        0     3592 2023-01-06 13:47:35.283094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/inline_object2.py
--rw-r--r--   0        0        0     3586 2023-01-06 13:47:35.283094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/inline_object3.py
--rw-r--r--   0        0        0     3701 2023-01-06 13:47:35.283094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/inline_response200.py
--rw-r--r--   0        0        0     3857 2023-01-06 13:47:35.283094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/inline_response2001.py
--rw-r--r--   0        0        0     5835 2023-01-06 13:47:35.283094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/inline_response2002.py
--rw-r--r--   0        0        0     8641 2023-01-06 13:47:35.283094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/inline_response2003.py
--rw-r--r--   0        0        0     6890 2023-01-06 13:47:35.283094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/inspection_report.py
--rw-r--r--   0        0        0     6744 2023-01-06 13:47:35.283094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/kg_snapshot.py
--rw-r--r--   0        0        0     4396 2023-01-06 13:47:35.283094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/kgc_data_input.py
--rw-r--r--   0        0        0     5504 2023-01-06 13:47:35.283094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/kibana_saved_queries_result.py
--rw-r--r--   0        0        0     3647 2023-01-06 13:47:35.283094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/knowledge_graph_authentication_callback.py
--rw-r--r--   0        0        0     3483 2023-01-06 13:47:35.283094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/knowledge_graph_chart_upgrade_options.py
--rw-r--r--   0        0        0     3705 2023-01-06 13:47:35.283094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/knowledge_graph_deployment_recreation_options.py
--rw-r--r--   0        0        0     3873 2023-01-06 13:47:35.283094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/knowledge_graph_snapshot_options.py
--rw-r--r--   0        0        0    10085 2023-01-06 13:47:35.283094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/knowledge_graph_system_information.py
--rw-r--r--   0        0        0     4357 2023-01-06 13:47:35.283094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/linked_ccs_instances.py
--rw-r--r--   0        0        0     5803 2023-01-06 13:47:35.283094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/load_data_flow_into_knowledge_graph_options.py
--rw-r--r--   0        0        0     4600 2023-01-06 13:47:35.283094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/load_data_flow_into_knowledge_graph_options1.py
--rw-r--r--   0        0        0     4474 2023-01-06 13:47:35.283094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/load_kgc_data_input.py
--rw-r--r--   0        0        0     4192 2023-01-06 13:47:35.283094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/load_kgc_data_input_dataflow.py
--rw-r--r--   0        0        0     4372 2023-01-06 13:47:35.283094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/load_kgc_data_input_target.py
--rw-r--r--   0        0        0    10405 2023-01-06 13:47:35.283094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/model_configuration.py
--rw-r--r--   0        0        0     5660 2023-01-06 13:47:35.283094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/model_supported_annotations_parameters.py
--rw-r--r--   0        0        0     4291 2023-01-06 13:47:35.283094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/mongo_coordinates.py
--rw-r--r--   0        0        0     3993 2023-01-06 13:47:35.283094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/mongo_s3_coordinates.py
--rw-r--r--   0        0        0     5040 2023-01-06 13:47:35.283094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/mongo_s3_coordinates_with_collection_list.py
--rw-r--r--   0        0        0     7509 2023-01-06 13:47:35.283094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/patch_data_catalog_options.py
--rw-r--r--   0        0        0     4752 2023-01-06 13:47:35.287094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/patch_dictionary_options.py
--rw-r--r--   0        0        0     5126 2023-01-06 13:47:35.287094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/patch_knowledge_graph_options.py
--rw-r--r--   0        0        0     5142 2023-01-06 13:47:35.287094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/patch_knowledge_graph_options1.py
--rw-r--r--   0        0        0     5026 2023-01-06 13:47:35.287094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/problem.py
--rw-r--r--   0        0        0     4450 2023-01-06 13:47:35.287094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/processing_model.py
--rw-r--r--   0        0        0     4495 2023-01-06 13:47:35.287094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/processing_model_data_flow.py
--rw-r--r--   0        0        0     5450 2023-01-06 13:47:35.287094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/processing_model_description.py
--rw-r--r--   0        0        0     6675 2023-01-06 13:47:35.287094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/project_data_index_non_view.py
--rw-r--r--   0        0        0     4489 2023-01-06 13:47:35.287094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/project_data_index_source.py
--rw-r--r--   0        0        0     6343 2023-01-06 13:47:35.287094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/project_data_index_view.py
--rw-r--r--   0        0        0     8014 2023-01-06 13:47:35.287094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/project_data_index_view_of.py
--rw-r--r--   0        0        0    13095 2023-01-06 13:47:35.287094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/project_data_index_with_status.py
--rw-r--r--   0        0        0     6309 2023-01-06 13:47:35.287094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/project_data_index_with_status_view_of.py
--rw-r--r--   0        0        0     4344 2023-01-06 13:47:35.287094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/project_default_values.py
--rw-r--r--   0        0        0     5349 2023-01-06 13:47:35.287094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/project_default_values_ccs_project.py
--rw-r--r--   0        0        0     4498 2023-01-06 13:47:35.287094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/project_default_values_dataflow.py
--rw-r--r--   0        0        0     5428 2023-01-06 13:47:35.287094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/project_flavour_total_kgs.py
--rw-r--r--   0        0        0     4447 2023-01-06 13:47:35.287094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/project_flavours.py
--rw-r--r--   0        0        0     3800 2023-01-06 13:47:35.287094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/project_package_instalation_manifest.py
--rw-r--r--   0        0        0     5089 2023-01-06 13:47:35.287094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/project_proj_key_annotate_document_report_document.py
--rw-r--r--   0        0        0     4739 2023-01-06 13:47:35.287094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/project_proj_key_annotate_document_report_report.py
--rw-r--r--   0        0        0     5683 2023-01-06 13:47:35.287094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/project_proj_key_bags_bag_key_tasks_assemble_dataflow_data_flow.py
--rw-r--r--   0        0        0     4758 2023-01-06 13:47:35.287094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/project_proj_key_bags_bag_key_tasks_assemble_dataflow_data_flow_render_options.py
--rw-r--r--   0        0        0     7904 2023-01-06 13:47:35.287094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/project_proj_key_bags_bag_key_tasks_export_dataset_info.py
--rw-r--r--   0        0        0     5194 2023-01-06 13:47:35.287094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/project_proj_key_bags_bag_key_tasks_export_dataset_info_coords.py
--rw-r--r--   0        0        0     7289 2023-01-06 13:47:35.287094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/project_proj_key_bags_bag_key_tasks_export_dataset_info_coords_node_collection.py
--rw-r--r--   0        0        0     4602 2023-01-06 13:47:35.287094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/project_proj_key_bags_bag_key_tasks_export_dataset_info_node_list.py
--rw-r--r--   0        0        0     3551 2023-01-06 13:47:35.287094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/project_proj_key_bags_bag_key_tasks_suspend_snapshot.py
--rw-r--r--   0        0        0     8557 2023-01-06 13:47:35.287094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/project_proj_key_data_catalogues_dc_key_collections_collection_name_actions_import_ccs.py
--rw-r--r--   0        0        0     8870 2023-01-06 13:47:35.287094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/project_proj_key_data_catalogues_dc_key_collections_collection_name_actions_import_ccs_export_package_mongo_options.py
--rw-r--r--   0        0        0     6166 2023-01-06 13:47:35.287094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/project_proj_key_data_catalogues_dc_key_collections_collection_name_actions_import_ccs_export_package_mongo_options_assemble_options.py
--rw-r--r--   0        0        0     7200 2023-01-06 13:47:35.287094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/project_proj_key_data_catalogues_dc_key_collections_collection_name_actions_import_ccs_export_package_mongo_options_assemble_options_mode.py
--rw-r--r--   0        0        0     5022 2023-01-06 13:47:35.287094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/project_proj_key_data_catalogues_dc_key_collections_collection_name_actions_import_ccs_export_package_mongo_options_assemble_options_options.py
--rw-r--r--   0        0        0     4442 2023-01-06 13:47:35.287094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/project_proj_key_data_catalogues_dc_key_collections_collection_name_actions_import_ccs_export_package_mongo_options_inputs.py
--rw-r--r--   0        0        0     5911 2023-01-06 13:47:35.287094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/project_proj_key_data_catalogues_dc_key_collections_collection_name_actions_import_ccs_export_package_mongo_options_package_options.py
--rw-r--r--   0        0        0     3951 2023-01-06 13:47:35.287094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/project_proj_key_data_catalogues_from_mongo_options.py
--rw-r--r--   0        0        0     5398 2023-01-06 13:47:35.287094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/project_proj_key_data_catalogues_from_mongo_target.py
--rw-r--r--   0        0        0     3668 2023-01-06 13:47:35.287094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/project_proj_key_data_catalogues_from_url_options.py
--rw-r--r--   0        0        0     5654 2023-01-06 13:47:35.287094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/project_proj_key_dictionaries_from_mongo_target.py
--rw-r--r--   0        0        0     4697 2023-01-06 13:47:35.287094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/project_proj_key_kgc_dataflow_templates_debug_df_tpl_key_target_bag.py
--rw-r--r--   0        0        0     5212 2023-01-06 13:47:35.287094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/project_proj_key_kgc_dataflow_templates_df_tpl_key_actions_load_render.py
--rw-r--r--   0        0        0     5093 2023-01-06 13:47:35.287094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/project_proj_key_kgc_dataflow_templates_df_tpl_key_actions_load_render_target_bag.py
--rw-r--r--   0        0        0     3834 2023-01-06 13:47:35.287094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/project_proj_key_kgc_dataflow_templates_df_tpl_key_actions_load_target.py
--rw-r--r--   0        0        0     4650 2023-01-06 13:47:35.287094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/project_proj_key_kgc_dataflow_templates_variables.py
--rw-r--r--   0        0        0     5107 2023-01-06 13:47:35.287094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/project_proj_key_kgc_raw_dataflow_templates_actions_run_data_flow.py
--rw-r--r--   0        0        0     4975 2023-01-06 13:47:35.287094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/project_proj_key_kgc_raw_dataflow_templates_actions_run_data_flow_template.py
--rw-r--r--   0        0        0     3673 2023-01-06 13:47:35.287094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/project_proj_key_model_configs_configurations.py
--rw-r--r--   0        0        0     4477 2023-01-06 13:47:35.287094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/project_proj_key_packages_packages.py
--rw-r--r--   0        0        0     9337 2023-01-06 13:47:35.287094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/project_task.py
--rw-r--r--   0        0        0     5224 2023-01-06 13:47:35.287094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/projects_flavours.py
--rw-r--r--   0        0        0     4330 2023-01-06 13:47:35.287094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/projects_flavours_flavours.py
--rw-r--r--   0        0        0     5229 2023-01-06 13:47:35.287094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/projects_flavours_quota.py
--rw-r--r--   0        0        0     4336 2023-01-06 13:47:35.287094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/related_task.py
--rw-r--r--   0        0        0     4453 2023-01-06 13:47:35.287094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/relationship_annotation_column.py
--rw-r--r--   0        0        0     5513 2023-01-06 13:47:35.287094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/relationship_annotation_descriptor.py
--rw-r--r--   0        0        0     4852 2023-01-06 13:47:35.287094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/render_data_flow_template_options.py
--rw-r--r--   0        0        0     3680 2023-01-06 13:47:35.287094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/restore_knowledge_graph_backup_options.py
--rw-r--r--   0        0        0     4435 2023-01-06 13:47:35.287094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/resume_knowledge_graph_options.py
--rw-r--r--   0        0        0     4382 2023-01-06 13:47:35.287094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/run_data_flow_template_options.py
--rw-r--r--   0        0        0     5772 2023-01-06 13:47:35.287094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/run_data_flow_template_options1.py
--rw-r--r--   0        0        0     9951 2023-01-06 13:47:35.287094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/s3_coordinates.py
--rw-r--r--   0        0        0    10201 2023-01-06 13:47:35.287094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/s3_coordinates_with_backup_key.py
--rw-r--r--   0        0        0     4519 2023-01-06 13:47:35.287094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/s3_coordinates_with_backup_key_presigned.py
--rw-r--r--   0        0        0     8194 2023-01-06 13:47:35.287094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/storage_summary_dc.py
--rw-r--r--   0        0        0     9388 2023-01-06 13:47:35.287094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/storage_summary_kg.py
--rw-r--r--   0        0        0     7367 2023-01-06 13:47:35.287094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/storage_summary_kg_categories_fraction.py
--rw-r--r--   0        0        0     6790 2023-01-06 13:47:35.287094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/storage_summary_task.py
--rw-r--r--   0        0        0     5872 2023-01-06 13:47:35.287094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/supported_annotator_annotations.py
--rw-r--r--   0        0        0     4593 2023-01-06 13:47:35.287094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/suspend_knowledge_graph_options.py
--rw-r--r--   0        0        0     5710 2023-01-06 13:47:35.287094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/system_celery_tasks_failure_failures.py
--rw-r--r--   0        0        0     5341 2023-01-06 13:47:35.287094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/system_info.py
--rw-r--r--   0        0        0     4785 2023-01-06 13:47:35.287094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/system_info_api.py
--rw-r--r--   0        0        0     6788 2023-01-06 13:47:35.287094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/system_info_deployment.py
--rw-r--r--   0        0        0     4255 2023-01-06 13:47:35.287094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/system_info_deployment_linked_ccs_api.py
--rw-r--r--   0        0        0     4148 2023-01-06 13:47:35.287094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/system_kgs_backend.py
--rw-r--r--   0        0        0     5454 2023-01-06 13:47:35.287094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/system_kgs_deployment.py
--rw-r--r--   0        0        0     4202 2023-01-06 13:47:35.287094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/system_kgs_deployment_resources.py
--rw-r--r--   0        0        0     6464 2023-01-06 13:47:35.287094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/system_modules_configuration.py
--rw-r--r--   0        0        0     3456 2023-01-06 13:47:35.287094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/system_modules_tasks.py
--rw-r--r--   0        0        0     3432 2023-01-06 13:47:35.287094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/system_modules_tasks_tasks.py
--rw-r--r--   0        0        0     5238 2023-01-06 13:47:35.287094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/take_snapshot_settings.py
--rw-r--r--   0        0        0     5652 2023-01-06 13:47:35.287094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/take_snapshot_settings_backend_aware.py
--rw-r--r--   0        0        0     8365 2023-01-06 13:47:35.287094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/task.py
--rw-r--r--   0        0        0     9820 2023-01-06 13:47:35.287094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/temporary_upload_file_result.py
--rw-r--r--   0        0        0     3443 2023-01-06 13:47:35.287094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/temporary_upload_file_result_download.py
--rw-r--r--   0        0        0     3499 2023-01-06 13:47:35.287094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/temporary_upload_file_result_download_private.py
--rw-r--r--   0        0        0     3443 2023-01-06 13:47:35.287094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/temporary_upload_file_result_metadata.py
--rw-r--r--   0        0        0     3499 2023-01-06 13:47:35.287094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/temporary_upload_file_result_metadata_private.py
--rw-r--r--   0        0        0     4129 2023-01-06 13:47:35.287094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/temporary_upload_file_result_upload.py
--rw-r--r--   0        0        0     4213 2023-01-06 13:47:35.287094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/temporary_upload_file_result_upload_private.py
--rw-r--r--   0        0        0     3478 2023-01-06 13:47:35.287094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/token_response.py
--rw-r--r--   0        0        0     4369 2023-01-06 13:47:35.287094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/topology.py
--rw-r--r--   0        0        0     5031 2023-01-06 13:47:35.291094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/topology_edge.py
--rw-r--r--   0        0        0     3449 2023-01-06 13:47:35.291094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/topology_node.py
--rw-r--r--   0        0        0     7001 2023-01-06 13:47:35.291094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/update_data_flow_options.py
--rw-r--r--   0        0        0     6334 2023-01-06 13:47:35.291094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/update_project_model_config_options.py
--rw-r--r--   0        0        0     6790 2023-01-06 13:47:35.291094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/uploaded_file.py
--rw-r--r--   0        0        0     4401 2023-01-06 13:47:35.291094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/uploaded_file_result.py
--rw-r--r--   0        0        0     4717 2023-01-06 13:47:35.291094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/usage_stats.py
--rw-r--r--   0        0        0     5319 2023-01-06 13:47:35.291094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/well_known_df_template_variable.py
--rw-r--r--   0        0        0    12356 2023-01-06 13:47:35.291094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/rest.py
--rw-r--r--   0        0        0     2773 2023-01-06 13:47:35.291094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/user/__init__.py
--rw-r--r--   0        0        0      455 2023-01-06 13:47:35.291094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/user/api/__init__.py
--rw-r--r--   0        0        0    20416 2023-01-06 13:47:35.291094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/user/api/admin_api.py
--rw-r--r--   0        0        0    19855 2023-01-06 13:47:35.291094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/user/api/oidc_api.py
--rw-r--r--   0        0        0    71698 2023-01-06 13:47:35.291094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/user/api/projects_api.py
--rw-r--r--   0        0        0     5208 2023-01-06 13:47:35.291094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/user/api/settings_api.py
--rw-r--r--   0        0        0     5135 2023-01-06 13:47:35.291094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/user/api/user_api.py
--rw-r--r--   0        0        0    33259 2023-01-06 13:47:35.291094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/user/api/users_api.py
--rw-r--r--   0        0        0    26301 2023-01-06 13:47:35.291094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/user/api_client.py
--rw-r--r--   0        0        0    14021 2023-01-06 13:47:35.291094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/user/configuration.py
--rw-r--r--   0        0        0     3796 2023-01-06 13:47:35.291094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/user/exceptions.py
--rw-r--r--   0        0        0     1899 2023-01-06 13:47:35.291094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/user/models/__init__.py
--rw-r--r--   0        0        0     3429 2023-01-06 13:47:35.291094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/user/models/access_token.py
--rw-r--r--   0        0        0     4019 2023-01-06 13:47:35.291094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/user/models/api_key.py
--rw-r--r--   0        0        0     7956 2023-01-06 13:47:35.291094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/user/models/audit_record.py
--rw-r--r--   0        0        0     4516 2023-01-06 13:47:35.291094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/user/models/create_project_request_body.py
--rw-r--r--   0        0        0     4336 2023-01-06 13:47:35.291094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/user/models/create_tokens_request_body.py
--rw-r--r--   0        0        0     3556 2023-01-06 13:47:35.291094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/user/models/error_response.py
--rw-r--r--   0        0        0     3405 2023-01-06 13:47:35.291094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/user/models/get_access_token_request_body.py
--rw-r--r--   0        0        0     4915 2023-01-06 13:47:35.291094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/user/models/impersonate_user_token_request_body.py
--rw-r--r--   0        0        0     3555 2023-01-06 13:47:35.291094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/user/models/inline_response200.py
--rw-r--r--   0        0        0     5252 2023-01-06 13:47:35.291094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/user/models/oidc_token_response.py
--rw-r--r--   0        0        0     5003 2023-01-06 13:47:35.291094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/user/models/project.py
--rw-r--r--   0        0        0     4530 2023-01-06 13:47:35.291094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/user/models/project_user_assignment.py
--rw-r--r--   0        0        0     4790 2023-01-06 13:47:35.291094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/user/models/register_user_request_body.py
--rw-r--r--   0        0        0     4907 2023-01-06 13:47:35.291094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/user/models/service_account.py
--rw-r--r--   0        0        0     4486 2023-01-06 13:47:35.291094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/user/models/service_account_credentials.py
--rw-r--r--   0        0        0     3602 2023-01-06 13:47:35.291094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/user/models/success_message.py
--rw-r--r--   0        0        0     3566 2023-01-06 13:47:35.291094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/user/models/token_response.py
--rw-r--r--   0        0        0     4515 2023-01-06 13:47:35.291094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/user/models/user_details.py
--rw-r--r--   0        0        0     2827 2023-01-06 13:47:35.291094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/user/models/user_type.py
--rw-r--r--   0        0        0    12338 2023-01-06 13:47:35.291094 deepsearch_toolkit-0.8.0/deepsearch/cps/apis/user/rest.py
--rw-r--r--   0        0        0      110 2023-01-06 13:47:35.291094 deepsearch_toolkit-0.8.0/deepsearch/cps/cli/__init__.py
--rw-r--r--   0        0        0     1119 2023-01-06 13:47:35.291094 deepsearch_toolkit-0.8.0/deepsearch/cps/cli/cli_options.py
--rw-r--r--   0        0        0     3937 2023-01-06 13:47:35.291094 deepsearch_toolkit-0.8.0/deepsearch/cps/cli/data_indices_typer.py
--rw-r--r--   0        0        0      983 2023-01-06 13:47:35.291094 deepsearch_toolkit-0.8.0/deepsearch/cps/cli/elastic_data.py
--rw-r--r--   0        0        0     3310 2023-01-06 13:47:35.291094 deepsearch_toolkit-0.8.0/deepsearch/cps/cli/kgs.py
--rw-r--r--   0        0        0      595 2023-01-06 13:47:35.291094 deepsearch_toolkit-0.8.0/deepsearch/cps/cli/main.py
--rw-r--r--   0        0        0     1705 2023-01-06 13:47:35.291094 deepsearch_toolkit-0.8.0/deepsearch/cps/cli/projects.py
--rw-r--r--   0        0        0       76 2023-01-06 13:47:35.291094 deepsearch_toolkit-0.8.0/deepsearch/cps/client/__init__.py
--rw-r--r--   0        0        0     5758 2023-01-06 13:47:35.291094 deepsearch_toolkit-0.8.0/deepsearch/cps/client/api.py
--rw-r--r--   0        0        0        0 2023-01-06 13:47:35.291094 deepsearch_toolkit-0.8.0/deepsearch/cps/client/builders/__init__.py
--rw-r--r--   0        0        0     2207 2023-01-06 13:47:35.291094 deepsearch_toolkit-0.8.0/deepsearch/cps/client/builders/wf_builder.py
--rw-r--r--   0        0        0      458 2023-01-06 13:47:35.291094 deepsearch_toolkit-0.8.0/deepsearch/cps/client/components/__init__.py
--rw-r--r--   0        0        0      222 2023-01-06 13:47:35.291094 deepsearch_toolkit-0.8.0/deepsearch/cps/client/components/api_object.py
--rw-r--r--   0        0        0     5223 2023-01-06 13:47:35.291094 deepsearch_toolkit-0.8.0/deepsearch/cps/client/components/data_catalogs.py
--rw-r--r--   0        0        0     3528 2023-01-06 13:47:35.291094 deepsearch_toolkit-0.8.0/deepsearch/cps/client/components/data_indices.py
--rw-r--r--   0        0        0     4486 2023-01-06 13:47:35.291094 deepsearch_toolkit-0.8.0/deepsearch/cps/client/components/documents.py
--rw-r--r--   0        0        0     5087 2023-01-06 13:47:35.291094 deepsearch_toolkit-0.8.0/deepsearch/cps/client/components/elastic.py
--rw-r--r--   0        0        0     4354 2023-01-06 13:47:35.291094 deepsearch_toolkit-0.8.0/deepsearch/cps/client/components/knowledge_graphs.py
--rw-r--r--   0        0        0     2632 2023-01-06 13:47:35.291094 deepsearch_toolkit-0.8.0/deepsearch/cps/client/components/projects.py
--rw-r--r--   0        0        0     3866 2023-01-06 13:47:35.291094 deepsearch_toolkit-0.8.0/deepsearch/cps/client/components/queries.py
--rw-r--r--   0        0        0     1002 2023-01-06 13:47:35.291094 deepsearch_toolkit-0.8.0/deepsearch/cps/client/components/tasks.py
--rw-r--r--   0        0        0      135 2023-01-06 13:47:35.291094 deepsearch_toolkit-0.8.0/deepsearch/cps/client/queries/__init__.py
--rw-r--r--   0        0        0     3171 2023-01-06 13:47:35.291094 deepsearch_toolkit-0.8.0/deepsearch/cps/client/queries/query.py
--rw-r--r--   0        0        0       96 2023-01-06 13:47:35.291094 deepsearch_toolkit-0.8.0/deepsearch/cps/client/queries/query_tasks/__init__.py
--rw-r--r--   0        0        0     1646 2023-01-06 13:47:35.291094 deepsearch_toolkit-0.8.0/deepsearch/cps/client/queries/query_tasks/for_each.py
--rw-r--r--   0        0        0     1245 2023-01-06 13:47:35.291094 deepsearch_toolkit-0.8.0/deepsearch/cps/client/queries/query_tasks/workflow.py
--rw-r--r--   0        0        0     3790 2023-01-06 13:47:35.291094 deepsearch_toolkit-0.8.0/deepsearch/cps/client/queries/task.py
--rw-r--r--   0        0        0       32 2023-01-06 13:47:35.291094 deepsearch_toolkit-0.8.0/deepsearch/cps/data_indices/__init__.py
--rw-r--r--   0        0        0     4854 2023-01-06 13:47:35.291094 deepsearch_toolkit-0.8.0/deepsearch/cps/data_indices/utils.py
--rw-r--r--   0        0        0      687 2023-01-06 13:47:35.291094 deepsearch_toolkit-0.8.0/deepsearch/cps/ipython/__init__.py
--rw-r--r--   0        0        0     1961 2023-01-06 13:47:35.291094 deepsearch_toolkit-0.8.0/deepsearch/cps/ipython/kg_helpers.py
--rw-r--r--   0        0        0     4159 2023-01-06 13:47:35.291094 deepsearch_toolkit-0.8.0/deepsearch/cps/ipython/kg_widgets.py
--rw-r--r--   0        0        0        0 2023-01-06 13:47:35.291094 deepsearch_toolkit-0.8.0/deepsearch/cps/kg/__init__.py
--rw-r--r--   0        0        0     2708 2023-01-06 13:47:35.291094 deepsearch_toolkit-0.8.0/deepsearch/cps/kg/workflow/MultiLinkedList.py
--rw-r--r--   0        0        0       88 2023-01-06 13:47:35.291094 deepsearch_toolkit-0.8.0/deepsearch/cps/kg/workflow/__init__.py
--rw-r--r--   0        0        0     1594 2023-01-06 13:47:35.291094 deepsearch_toolkit-0.8.0/deepsearch/cps/kg/workflow/wf_functions.py
--rw-r--r--   0        0        0    17480 2023-01-06 13:47:35.295094 deepsearch_toolkit-0.8.0/deepsearch/cps/kg/workflow/workflow.py
--rw-r--r--   0        0        0     1941 2023-01-06 13:47:35.295094 deepsearch_toolkit-0.8.0/deepsearch/cps/queries/__init__.py
--rw-r--r--   0        0        0       36 2023-01-06 13:47:35.295094 deepsearch_toolkit-0.8.0/deepsearch/documents/__init__.py
--rw-r--r--   0        0        0        1 2023-01-06 13:47:35.295094 deepsearch_toolkit-0.8.0/deepsearch/documents/cli/__init__.py
--rw-r--r--   0        0        0     3728 2023-01-06 13:47:35.295094 deepsearch_toolkit-0.8.0/deepsearch/documents/cli/main.py
--rw-r--r--   0        0        0       36 2023-01-06 13:47:35.295094 deepsearch_toolkit-0.8.0/deepsearch/documents/core/__init__.py
--rw-r--r--   0        0        0      549 2023-01-06 13:47:35.295094 deepsearch_toolkit-0.8.0/deepsearch/documents/core/common_routines.py
--rw-r--r--   0        0        0     8751 2023-01-06 13:47:35.295094 deepsearch_toolkit-0.8.0/deepsearch/documents/core/convert.py
--rw-r--r--   0        0        0     4012 2023-01-06 13:47:35.295094 deepsearch_toolkit-0.8.0/deepsearch/documents/core/create_report.py
--rw-r--r--   0        0        0     2796 2023-01-06 13:47:35.295094 deepsearch_toolkit-0.8.0/deepsearch/documents/core/input_process.py
--rw-r--r--   0        0        0     2598 2023-01-06 13:47:35.295094 deepsearch_toolkit-0.8.0/deepsearch/documents/core/main.py
--rw-r--r--   0        0        0     9809 2023-01-06 13:47:35.295094 deepsearch_toolkit-0.8.0/deepsearch/documents/core/models.py
--rw-r--r--   0        0        0     8384 2023-01-06 13:47:35.295094 deepsearch_toolkit-0.8.0/deepsearch/documents/core/utils.py
--rw-r--r--   0        0        0        0 2023-01-06 13:47:35.295094 deepsearch_toolkit-0.8.0/deepsearch/plugins/__init__.py
--rw-r--r--   0        0        0      656 2023-01-06 13:47:35.295094 deepsearch_toolkit-0.8.0/deepsearch/plugins/example_toy_cli_plugin.py
--rw-r--r--   0        0        0        0 2023-01-06 13:47:35.295094 deepsearch_toolkit-0.8.0/deepsearch/py.typed
--rw-r--r--   0        0        0        0 2023-01-06 13:47:35.295094 deepsearch_toolkit-0.8.0/deepsearch/query/__init__.py
--rw-r--r--   0        0        0        0 2023-01-06 13:47:35.295094 deepsearch_toolkit-0.8.0/deepsearch/query/cli/__init__.py
--rw-r--r--   0        0        0     4210 2023-01-06 13:47:35.295094 deepsearch_toolkit-0.8.0/deepsearch/query/cli/main.py
--rw-r--r--   0        0        0     4367 2023-01-06 13:47:35.319094 deepsearch_toolkit-0.8.0/pyproject.toml
--rw-r--r--   0        0        0     5414 1970-01-01 00:00:00.000000 deepsearch_toolkit-0.8.0/setup.py
--rw-r--r--   0        0        0     4928 1970-01-01 00:00:00.000000 deepsearch_toolkit-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1088 2023-01-23 12:25:16.896891 deepsearch_toolkit-0.9.0/LICENSE
+-rw-r--r--   0        0        0     3100 2023-01-23 12:25:16.896891 deepsearch_toolkit-0.9.0/README.md
+-rw-r--r--   0        0        0      263 2023-01-23 12:25:16.896891 deepsearch_toolkit-0.9.0/deepsearch/__init__.py
+-rw-r--r--   0        0        0      671 2023-01-23 12:25:16.896891 deepsearch_toolkit-0.9.0/deepsearch/cli.py
+-rw-r--r--   0        0        0       22 2023-01-23 12:25:16.896891 deepsearch_toolkit-0.9.0/deepsearch/core/__init__.py
+-rw-r--r--   0        0        0        0 2023-01-23 12:25:16.896891 deepsearch_toolkit-0.9.0/deepsearch/core/cli/__init__.py
+-rw-r--r--   0        0        0      745 2023-01-23 12:25:16.896891 deepsearch_toolkit-0.9.0/deepsearch/core/cli/config.py
+-rw-r--r--   0        0        0     1267 2023-01-23 12:25:16.896891 deepsearch_toolkit-0.9.0/deepsearch/core/cli/login.py
+-rw-r--r--   0        0        0      577 2023-01-23 12:25:16.896891 deepsearch_toolkit-0.9.0/deepsearch/core/cli/main.py
+-rw-r--r--   0        0        0     1000 2023-01-23 12:25:16.896891 deepsearch_toolkit-0.9.0/deepsearch/core/cli/plugins.py
+-rw-r--r--   0        0        0       83 2023-01-23 12:25:16.896891 deepsearch_toolkit-0.9.0/deepsearch/core/client/__init__.py
+-rw-r--r--   0        0        0      373 2023-01-23 12:25:16.896891 deepsearch_toolkit-0.9.0/deepsearch/core/client/config.py
+-rw-r--r--   0        0        0        0 2023-01-23 12:25:16.896891 deepsearch_toolkit-0.9.0/deepsearch/core/util/__init__.py
+-rw-r--r--   0        0        0      457 2023-01-23 12:25:16.896891 deepsearch_toolkit-0.9.0/deepsearch/core/util/_version.py
+-rw-r--r--   0        0        0      560 2023-01-23 12:25:16.896891 deepsearch_toolkit-0.9.0/deepsearch/core/util/ccs_utils.py
+-rw-r--r--   0        0        0      487 2023-01-23 12:25:16.896891 deepsearch_toolkit-0.9.0/deepsearch/core/util/cli_output.py
+-rw-r--r--   0        0        0     1391 2023-01-23 12:25:16.896891 deepsearch_toolkit-0.9.0/deepsearch/core/util/config_paths.py
+-rw-r--r--   0        0        0       79 2023-01-23 12:25:16.896891 deepsearch_toolkit-0.9.0/deepsearch/cps/__init__.py
+-rw-r--r--   0        0        0       26 2023-01-23 12:25:16.896891 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/.gitattributes
+-rw-r--r--   0        0        0       89 2023-01-23 12:25:16.896891 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/README.md
+-rw-r--r--   0        0        0        0 2023-01-23 12:25:16.896891 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/__init__.py
+-rw-r--r--   0        0        0        0 2023-01-23 12:25:16.896891 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/kg/__init__.py
+-rw-r--r--   0        0        0     2347 2023-01-23 12:25:16.896891 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/kg/create/__init__.py
+-rw-r--r--   0        0        0      437 2023-01-23 12:25:16.896891 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/kg/create/api/__init__.py
+-rw-r--r--   0        0        0    42138 2023-01-23 12:25:16.896891 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/kg/create/api/edges_api.py
+-rw-r--r--   0        0        0     6763 2023-01-23 12:25:16.896891 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/kg/create/api/indices_api.py
+-rw-r--r--   0        0        0    35757 2023-01-23 12:25:16.896891 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/kg/create/api/knowledge_graphs_api.py
+-rw-r--r--   0        0        0    18521 2023-01-23 12:25:16.896891 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/kg/create/api/nodes_api.py
+-rw-r--r--   0        0        0    10807 2023-01-23 12:25:16.896891 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/kg/create/api/tasks_api.py
+-rw-r--r--   0        0        0    26333 2023-01-23 12:25:16.896891 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/kg/create/api_client.py
+-rw-r--r--   0        0        0    13351 2023-01-23 12:25:16.896891 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/kg/create/configuration.py
+-rw-r--r--   0        0        0     3803 2023-01-23 12:25:16.896891 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/kg/create/exceptions.py
+-rw-r--r--   0        0        0     1456 2023-01-23 12:25:16.896891 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/kg/create/models/__init__.py
+-rw-r--r--   0        0        0     6487 2023-01-23 12:25:16.896891 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/kg/create/models/database_source.py
+-rw-r--r--   0        0        0     4321 2023-01-23 12:25:16.896891 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/kg/create/models/database_source_mongo.py
+-rw-r--r--   0        0        0     7453 2023-01-23 12:25:16.896891 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/kg/create/models/database_source_s3.py
+-rw-r--r--   0        0        0     4243 2023-01-23 12:25:16.896891 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/kg/create/models/edge_matrix.py
+-rw-r--r--   0        0        0     5932 2023-01-23 12:25:16.896891 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/kg/create/models/edge_model.py
+-rw-r--r--   0        0        0     5011 2023-01-23 12:25:16.896891 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/kg/create/models/inline_object.py
+-rw-r--r--   0        0        0     5027 2023-01-23 12:25:16.896891 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/kg/create/models/inline_object1.py
+-rw-r--r--   0        0        0     5027 2023-01-23 12:25:16.896891 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/kg/create/models/inline_object2.py
+-rw-r--r--   0        0        0     5705 2023-01-23 12:25:16.896891 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/kg/create/models/mongo_edge.py
+-rw-r--r--   0        0        0     4330 2023-01-23 12:25:16.896891 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/kg/create/models/mongo_edge_item.py
+-rw-r--r--   0        0        0     5884 2023-01-23 12:25:16.896891 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/kg/create/models/node.py
+-rw-r--r--   0        0        0     7719 2023-01-23 12:25:16.896891 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/kg/create/models/s3_source.py
+-rw-r--r--   0        0        0     4897 2023-01-23 12:25:16.896891 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/kg/create/models/sparse_matrix_with_names_or_hashes.py
+-rw-r--r--   0        0        0     4491 2023-01-23 12:25:16.896891 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/kg/create/models/triplet.py
+-rw-r--r--   0        0        0    12350 2023-01-23 12:25:16.896891 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/kg/create/rest.py
+-rw-r--r--   0        0        0     2820 2023-01-23 12:25:16.900891 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/kg/query/__init__.py
+-rw-r--r--   0        0        0      541 2023-01-23 12:25:16.900891 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/kg/query/api/__init__.py
+-rw-r--r--   0        0        0    18088 2023-01-23 12:25:16.900891 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/kg/query/api/description_api.py
+-rw-r--r--   0        0        0    13270 2023-01-23 12:25:16.900891 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/kg/query/api/inspect_api.py
+-rw-r--r--   0        0        0    44595 2023-01-23 12:25:16.900891 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/kg/query/api/node_data_retrieval_api.py
+-rw-r--r--   0        0        0    23175 2023-01-23 12:25:16.900891 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/kg/query/api/node_retrieval_api.py
+-rw-r--r--   0        0        0    14635 2023-01-23 12:25:16.900891 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/kg/query/api/node_search_api.py
+-rw-r--r--   0        0        0    53227 2023-01-23 12:25:16.900891 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/kg/query/api/query_api.py
+-rw-r--r--   0        0        0    26327 2023-01-23 12:25:16.900891 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/kg/query/api_client.py
+-rw-r--r--   0        0        0    13332 2023-01-23 12:25:16.900891 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/kg/query/configuration.py
+-rw-r--r--   0        0        0     3802 2023-01-23 12:25:16.900891 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/kg/query/exceptions.py
+-rw-r--r--   0        0        0     1832 2023-01-23 12:25:16.900891 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/kg/query/models/__init__.py
+-rw-r--r--   0        0        0     4060 2023-01-23 12:25:16.900891 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/kg/query/models/auth_config.py
+-rw-r--r--   0        0        0     5234 2023-01-23 12:25:16.900891 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/kg/query/models/error_model.py
+-rw-r--r--   0        0        0     4692 2023-01-23 12:25:16.900891 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/kg/query/models/graph_description.py
+-rw-r--r--   0        0        0     5806 2023-01-23 12:25:16.900891 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/kg/query/models/graph_edge.py
+-rw-r--r--   0        0        0     6110 2023-01-23 12:25:16.900891 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/kg/query/models/graph_matrix.py
+-rw-r--r--   0        0        0     4948 2023-01-23 12:25:16.900891 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/kg/query/models/graph_node_description.py
+-rw-r--r--   0        0        0     4847 2023-01-23 12:25:16.900891 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/kg/query/models/graph_node_description_categories.py
+-rw-r--r--   0        0        0     5151 2023-01-23 12:25:16.900891 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/kg/query/models/inline_object.py
+-rw-r--r--   0        0        0     5882 2023-01-23 12:25:16.900891 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/kg/query/models/node.py
+-rw-r--r--   0        0        0     2734 2023-01-23 12:25:16.900891 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/kg/query/models/nodes_response_model.py
+-rw-r--r--   0        0        0     4607 2023-01-23 12:25:16.900891 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/kg/query/models/nodes_response_model_all_of.py
+-rw-r--r--   0        0        0     3635 2023-01-23 12:25:16.900891 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/kg/query/models/nodes_response_model_all_of_response.py
+-rw-r--r--   0        0        0     5045 2023-01-23 12:25:16.900891 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/kg/query/models/response_model.py
+-rw-r--r--   0        0        0     4922 2023-01-23 12:25:16.900891 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/kg/query/models/workflow_response.py
+-rw-r--r--   0        0        0     2746 2023-01-23 12:25:16.900891 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/kg/query/models/workflow_response_model.py
+-rw-r--r--   0        0        0     4604 2023-01-23 12:25:16.900891 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/kg/query/models/workflow_response_model_all_of.py
+-rw-r--r--   0        0        0     6662 2023-01-23 12:25:16.900891 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/kg/query/models/workflow_response_node.py
+-rw-r--r--   0        0        0    12348 2023-01-23 12:25:16.900891 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/kg/query/rest.py
+-rw-r--r--   0        0        0    28378 2023-01-23 12:25:16.900891 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/__init__.py
+-rw-r--r--   0        0        0     1124 2023-01-23 12:25:16.900891 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/api/__init__.py
+-rw-r--r--   0        0        0    32396 2023-01-23 12:25:16.900891 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/api/annotate_api.py
+-rw-r--r--   0        0        0   170020 2023-01-23 12:25:16.900891 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/api/data_catalogs_api.py
+-rw-r--r--   0        0        0   131553 2023-01-23 12:25:16.900891 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/api/data_flows_api.py
+-rw-r--r--   0        0        0    57195 2023-01-23 12:25:16.900891 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/api/data_indices_api.py
+-rw-r--r--   0        0        0   133861 2023-01-23 12:25:16.900891 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/api/dictionaries_api.py
+-rw-r--r--   0        0        0    25396 2023-01-23 12:25:16.900891 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/api/document_annotation_api.py
+-rw-r--r--   0        0        0    34436 2023-01-23 12:25:16.900891 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/api/elastic_api.py
+-rw-r--r--   0        0        0   200606 2023-01-23 12:25:16.904890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/api/knowledge_graphs_api.py
+-rw-r--r--   0        0        0    46122 2023-01-23 12:25:16.904890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/api/model_configurations_api.py
+-rw-r--r--   0        0        0    10605 2023-01-23 12:25:16.904890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/api/processing_model_api.py
+-rw-r--r--   0        0        0    17431 2023-01-23 12:25:16.904890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/api/project_api.py
+-rw-r--r--   0        0        0   116434 2023-01-23 12:25:16.904890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/api/system_api.py
+-rw-r--r--   0        0        0    36829 2023-01-23 12:25:16.904890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/api/tasks_api.py
+-rw-r--r--   0        0        0    25072 2023-01-23 12:25:16.904890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/api/uploads_api.py
+-rw-r--r--   0        0        0    26327 2023-01-23 12:25:16.904890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/api_client.py
+-rw-r--r--   0        0        0    13946 2023-01-23 12:25:16.904890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/configuration.py
+-rw-r--r--   0        0        0     3812 2023-01-23 12:25:16.904890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/exceptions.py
+-rw-r--r--   0        0        0    26821 2023-01-23 12:25:16.904890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/__init__.py
+-rw-r--r--   0        0        0     7657 2023-01-23 12:25:16.904890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/annotate_document_request.py
+-rw-r--r--   0        0        0     4510 2023-01-23 12:25:16.904890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/annotate_object_options.py
+-rw-r--r--   0        0        0     6736 2023-01-23 12:25:16.904890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/annotate_object_options1.py
+-rw-r--r--   0        0        0     6978 2023-01-23 12:25:16.904890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/annotated_document_report.py
+-rw-r--r--   0        0        0     6086 2023-01-23 12:25:16.904890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/annotated_image.py
+-rw-r--r--   0        0        0     4648 2023-01-23 12:25:16.904890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/annotated_object.py
+-rw-r--r--   0        0        0     4664 2023-01-23 12:25:16.904890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/annotated_object1.py
+-rw-r--r--   0        0        0     6086 2023-01-23 12:25:16.904890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/annotated_table.py
+-rw-r--r--   0        0        0     6220 2023-01-23 12:25:16.904890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/annotated_text.py
+-rw-r--r--   0        0        0     6992 2023-01-23 12:25:16.904890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/annotated_text_lines.py
+-rw-r--r--   0        0        0     4286 2023-01-23 12:25:16.904890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/annotator_image_input.py
+-rw-r--r--   0        0        0     5165 2023-01-23 12:25:16.904890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/annotator_input.py
+-rw-r--r--   0        0        0     6724 2023-01-23 12:25:16.904890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/annotator_metadata.py
+-rw-r--r--   0        0        0     5629 2023-01-23 12:25:16.904890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/annotator_parameters_or_ref.py
+-rw-r--r--   0        0        0     4744 2023-01-23 12:25:16.904890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/annotator_supported_annotations_parameters.py
+-rw-r--r--   0        0        0     5871 2023-01-23 12:25:16.904890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/assemble_data_flow_into_knowledge_graph_options.py
+-rw-r--r--   0        0        0     5851 2023-01-23 12:25:16.904890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/assemble_data_flow_into_knowledge_graph_options1.py
+-rw-r--r--   0        0        0     4136 2023-01-23 12:25:16.904890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/backend_flavour.py
+-rw-r--r--   0        0        0     7053 2023-01-23 12:25:16.904890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/backend_project_proj_key_bags_bag_key_tasks_assemble_dataflow_data_flow.py
+-rw-r--r--   0        0        0     5168 2023-01-23 12:25:16.904890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/backend_project_proj_key_bags_bag_key_tasks_assemble_dataflow_data_flow_raw_data_flow.py
+-rw-r--r--   0        0        0     3964 2023-01-23 12:25:16.904890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/backend_project_proj_key_bags_bag_key_tasks_assemble_dataflow_render.py
+-rw-r--r--   0        0        0     4364 2023-01-23 12:25:16.904890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/backup_knowledge_graph_options.py
+-rw-r--r--   0        0        0    11072 2023-01-23 12:25:16.904890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/bag.py
+-rw-r--r--   0        0        0     3371 2023-01-23 12:25:16.904890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/bag_amqp_backend.py
+-rw-r--r--   0        0        0    10166 2023-01-23 12:25:16.904890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/bag_backend_aware.py
+-rw-r--r--   0        0        0     4187 2023-01-23 12:25:16.904890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/bag_backends.py
+-rw-r--r--   0        0        0     3447 2023-01-23 12:25:16.904890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/bag_callback.py
+-rw-r--r--   0        0        0     4284 2023-01-23 12:25:16.904890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/bag_component_status.py
+-rw-r--r--   0        0        0     3309 2023-01-23 12:25:16.904890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/bag_component_status_enum.py
+-rw-r--r--   0        0        0     4717 2023-01-23 12:25:16.904890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/bag_flavour.py
+-rw-r--r--   0        0        0     5271 2023-01-23 12:25:16.904890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/bag_flavour_default_quota.py
+-rw-r--r--   0        0        0    10094 2023-01-23 12:25:16.904890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/bag_flavour_full_data.py
+-rw-r--r--   0        0        0     6240 2023-01-23 12:25:16.904890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/bag_kg_legacy_api_backend.py
+-rw-r--r--   0        0        0     4417 2023-01-23 12:25:16.904890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/bag_status.py
+-rw-r--r--   0        0        0     5344 2023-01-23 12:25:16.904890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/bag_status_backend_aware.py
+-rw-r--r--   0        0        0     3668 2023-01-23 12:25:16.904890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/bag_status_backend_aware_kg_amqp.py
+-rw-r--r--   0        0        0     5905 2023-01-23 12:25:16.904890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/bag_status_components.py
+-rw-r--r--   0        0        0     5174 2023-01-23 12:25:16.904890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/catalog_reference.py
+-rw-r--r--   0        0        0     5312 2023-01-23 12:25:16.904890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/ccs_collection_reference.py
+-rw-r--r--   0        0        0     5440 2023-01-23 12:25:16.904890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/ccs_task.py
+-rw-r--r--   0        0        0     5215 2023-01-23 12:25:16.904890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/celery_task.py
+-rw-r--r--   0        0        0    12670 2023-01-23 12:25:16.904890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/celery_task1.py
+-rw-r--r--   0        0        0     5061 2023-01-23 12:25:16.904890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/celery_task_promise.py
+-rw-r--r--   0        0        0     6776 2023-01-23 12:25:16.904890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/clone_data_catalog_options.py
+-rw-r--r--   0        0        0     4669 2023-01-23 12:25:16.904890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/clone_data_catalog_result.py
+-rw-r--r--   0        0        0     6758 2023-01-23 12:25:16.904890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/clone_dictionary_options.py
+-rw-r--r--   0        0        0     7985 2023-01-23 12:25:16.904890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/clone_public_data_catalog_options.py
+-rw-r--r--   0        0        0     7667 2023-01-23 12:25:16.904890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/clone_public_dictionary_options.py
+-rw-r--r--   0        0        0     3557 2023-01-23 12:25:16.904890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/collection_list_coordinates.py
+-rw-r--r--   0        0        0     4576 2023-01-23 12:25:16.904890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/cps_model_reference.py
+-rw-r--r--   0        0        0     7188 2023-01-23 12:25:16.904890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/cps_package.py
+-rw-r--r--   0        0        0     4760 2023-01-23 12:25:16.904890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/create_collection_in_dictionary_options.py
+-rw-r--r--   0        0        0     4714 2023-01-23 12:25:16.904890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/create_data_catalog_collection_options.py
+-rw-r--r--   0        0        0     8354 2023-01-23 12:25:16.904890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/create_data_catalog_options.py
+-rw-r--r--   0        0        0     7916 2023-01-23 12:25:16.908890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/create_data_flow_template_options.py
+-rw-r--r--   0        0        0     5366 2023-01-23 12:25:16.908890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/create_dictionary_options.py
+-rw-r--r--   0        0        0     7026 2023-01-23 12:25:16.908890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/create_knowledge_graph_options.py
+-rw-r--r--   0        0        0     7003 2023-01-23 12:25:16.908890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/create_knowledge_graph_options1.py
+-rw-r--r--   0        0        0     7515 2023-01-23 12:25:16.908890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/create_project_model_config_options.py
+-rw-r--r--   0        0        0     4399 2023-01-23 12:25:16.908890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/data_catalog_category_schema.py
+-rw-r--r--   0        0        0     4414 2023-01-23 12:25:16.908890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/data_catalog_collection.py
+-rw-r--r--   0        0        0     4396 2023-01-23 12:25:16.908890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/data_catalog_data_flow.py
+-rw-r--r--   0        0        0     4672 2023-01-23 12:25:16.908890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/data_catalog_import_options.py
+-rw-r--r--   0        0        0     4702 2023-01-23 12:25:16.908890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/data_catalog_import_result.py
+-rw-r--r--   0        0        0     6022 2023-01-23 12:25:16.908890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/data_catalog_provenance_log.py
+-rw-r--r--   0        0        0     6858 2023-01-23 12:25:16.908890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/data_catalog_provenance_log_source.py
+-rw-r--r--   0        0        0     5272 2023-01-23 12:25:16.908890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/data_catalog_provenance_log_user.py
+-rw-r--r--   0        0        0     3972 2023-01-23 12:25:16.908890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/data_catalog_schema.py
+-rw-r--r--   0        0        0     4567 2023-01-23 12:25:16.908890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/data_catalog_topology.py
+-rw-r--r--   0        0        0     7093 2023-01-23 12:25:16.908890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/data_catalog_topology_edge.py
+-rw-r--r--   0        0        0     4477 2023-01-23 12:25:16.908890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/data_catalog_topology_node.py
+-rw-r--r--   0        0        0     4702 2023-01-23 12:25:16.908890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/data_catalog_url_import_options.py
+-rw-r--r--   0        0        0    13804 2023-01-23 12:25:16.908890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/data_catalogue.py
+-rw-r--r--   0        0        0     7433 2023-01-23 12:25:16.908890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/data_collection.py
+-rw-r--r--   0        0        0     9288 2023-01-23 12:25:16.908890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/data_collection_metadata.py
+-rw-r--r--   0        0        0     5036 2023-01-23 12:25:16.908890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/data_collection_source.py
+-rw-r--r--   0        0        0     8617 2023-01-23 12:25:16.908890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/data_flow.py
+-rw-r--r--   0        0        0     4540 2023-01-23 12:25:16.908890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/data_flow_assemble_into_knowledge_graph_task.py
+-rw-r--r--   0        0        0     4372 2023-01-23 12:25:16.908890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/data_flow_assemble_report.py
+-rw-r--r--   0        0        0     4081 2023-01-23 12:25:16.908890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/data_flow_assemble_report_cause.py
+-rw-r--r--   0        0        0     6287 2023-01-23 12:25:16.908890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/data_flow_assemble_report_chunks.py
+-rw-r--r--   0        0        0     4262 2023-01-23 12:25:16.908890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/data_flow_assemble_report_errors.py
+-rw-r--r--   0        0        0     5357 2023-01-23 12:25:16.908890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/data_flow_assemble_report_options.py
+-rw-r--r--   0        0        0     6557 2023-01-23 12:25:16.908890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/data_flow_assemble_report_single_task.py
+-rw-r--r--   0        0        0     5166 2023-01-23 12:25:16.908890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/data_flow_load_into_knowledge_graph_task.py
+-rw-r--r--   0        0        0     4411 2023-01-23 12:25:16.908890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/data_flow_template.py
+-rw-r--r--   0        0        0     7776 2023-01-23 12:25:16.908890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/data_flow_template_list_item.py
+-rw-r--r--   0        0        0     3653 2023-01-23 12:25:16.908890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/data_flow_template_variable.py
+-rw-r--r--   0        0        0     3525 2023-01-23 12:25:16.908890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/data_flow_topology_options.py
+-rw-r--r--   0        0        0     4760 2023-01-23 12:25:16.908890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/data_index_upload_file_source.py
+-rw-r--r--   0        0        0     9559 2023-01-23 12:25:16.908890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/dictionary.py
+-rw-r--r--   0        0        0     4244 2023-01-23 12:25:16.908890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/dictionary_clone_result.py
+-rw-r--r--   0        0        0     4402 2023-01-23 12:25:16.908890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/dictionary_collection.py
+-rw-r--r--   0        0        0     4402 2023-01-23 12:25:16.908890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/dictionary_collection_csv_data.py
+-rw-r--r--   0        0        0     5944 2023-01-23 12:25:16.908890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/dictionary_collection_patch.py
+-rw-r--r--   0        0        0     4320 2023-01-23 12:25:16.908890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/dictionary_entry.py
+-rw-r--r--   0        0        0     4654 2023-01-23 12:25:16.908890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/dictionary_import_options.py
+-rw-r--r--   0        0        0     4276 2023-01-23 12:25:16.908890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/dictionary_import_result.py
+-rw-r--r--   0        0        0     5681 2023-01-23 12:25:16.908890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/elastic_coordinates.py
+-rw-r--r--   0        0        0     7622 2023-01-23 12:25:16.908890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/elastic_index_search_query_options.py
+-rw-r--r--   0        0        0     4899 2023-01-23 12:25:16.908890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/elastic_index_search_results.py
+-rw-r--r--   0        0        0     5876 2023-01-23 12:25:16.908890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/entity_annotation.py
+-rw-r--r--   0        0        0     5265 2023-01-23 12:25:16.908890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/entity_annotation_descriptor.py
+-rw-r--r--   0        0        0     4308 2023-01-23 12:25:16.908890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/error_response.py
+-rw-r--r--   0        0        0     4961 2023-01-23 12:25:16.908890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/flavours_quota.py
+-rw-r--r--   0        0        0     4401 2023-01-23 12:25:16.908890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/fully_rendered_data_flow.py
+-rw-r--r--   0        0        0     3620 2023-01-23 12:25:16.908890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/image_cells.py
+-rw-r--r--   0        0        0     4219 2023-01-23 12:25:16.908890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/image_info.py
+-rw-r--r--   0        0        0     4098 2023-01-23 12:25:16.908890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/image_metadata.py
+-rw-r--r--   0        0        0     4613 2023-01-23 12:25:16.908890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/image_source.py
+-rw-r--r--   0        0        0     5566 2023-01-23 12:25:16.908890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/import_from_elastic_to_data_catalog_options.py
+-rw-r--r--   0        0        0     7503 2023-01-23 12:25:16.908890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/import_from_elastic_to_data_catalog_options_parameters.py
+-rw-r--r--   0        0        0     5576 2023-01-23 12:25:16.908890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/import_from_elastic_to_data_catalog_options_parameters_query_options.py
+-rw-r--r--   0        0        0    10951 2023-01-23 12:25:16.908890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/import_from_elastic_to_data_catalog_s3_coords.py
+-rw-r--r--   0        0        0     5168 2023-01-23 12:25:16.908890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/import_to_data_catalog_collection_options.py
+-rw-r--r--   0        0        0     4259 2023-01-23 12:25:16.908890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/import_to_data_catalog_options.py
+-rw-r--r--   0        0        0     4176 2023-01-23 12:25:16.908890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/infer_project_data_catalog_category_schema.py
+-rw-r--r--   0        0        0     3620 2023-01-23 12:25:16.908890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/inline_object.py
+-rw-r--r--   0        0        0     8640 2023-01-23 12:25:16.908890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/inline_object1.py
+-rw-r--r--   0        0        0     3592 2023-01-23 12:25:16.908890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/inline_object2.py
+-rw-r--r--   0        0        0     3586 2023-01-23 12:25:16.908890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/inline_object3.py
+-rw-r--r--   0        0        0     3701 2023-01-23 12:25:16.908890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/inline_response200.py
+-rw-r--r--   0        0        0     3857 2023-01-23 12:25:16.908890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/inline_response2001.py
+-rw-r--r--   0        0        0     5835 2023-01-23 12:25:16.908890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/inline_response2002.py
+-rw-r--r--   0        0        0     8641 2023-01-23 12:25:16.908890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/inline_response2003.py
+-rw-r--r--   0        0        0     6890 2023-01-23 12:25:16.908890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/inspection_report.py
+-rw-r--r--   0        0        0     6744 2023-01-23 12:25:16.908890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/kg_snapshot.py
+-rw-r--r--   0        0        0     4396 2023-01-23 12:25:16.908890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/kgc_data_input.py
+-rw-r--r--   0        0        0     5504 2023-01-23 12:25:16.908890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/kibana_saved_queries_result.py
+-rw-r--r--   0        0        0     3647 2023-01-23 12:25:16.908890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/knowledge_graph_authentication_callback.py
+-rw-r--r--   0        0        0     3483 2023-01-23 12:25:16.908890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/knowledge_graph_chart_upgrade_options.py
+-rw-r--r--   0        0        0     3705 2023-01-23 12:25:16.908890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/knowledge_graph_deployment_recreation_options.py
+-rw-r--r--   0        0        0     3873 2023-01-23 12:25:16.908890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/knowledge_graph_snapshot_options.py
+-rw-r--r--   0        0        0    10085 2023-01-23 12:25:16.912890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/knowledge_graph_system_information.py
+-rw-r--r--   0        0        0     4357 2023-01-23 12:25:16.912890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/linked_ccs_instances.py
+-rw-r--r--   0        0        0     5803 2023-01-23 12:25:16.912890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/load_data_flow_into_knowledge_graph_options.py
+-rw-r--r--   0        0        0     4600 2023-01-23 12:25:16.912890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/load_data_flow_into_knowledge_graph_options1.py
+-rw-r--r--   0        0        0     4474 2023-01-23 12:25:16.912890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/load_kgc_data_input.py
+-rw-r--r--   0        0        0     4192 2023-01-23 12:25:16.912890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/load_kgc_data_input_dataflow.py
+-rw-r--r--   0        0        0     4372 2023-01-23 12:25:16.912890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/load_kgc_data_input_target.py
+-rw-r--r--   0        0        0    10405 2023-01-23 12:25:16.912890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/model_configuration.py
+-rw-r--r--   0        0        0     5660 2023-01-23 12:25:16.912890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/model_supported_annotations_parameters.py
+-rw-r--r--   0        0        0     4291 2023-01-23 12:25:16.912890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/mongo_coordinates.py
+-rw-r--r--   0        0        0     3993 2023-01-23 12:25:16.912890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/mongo_s3_coordinates.py
+-rw-r--r--   0        0        0     5040 2023-01-23 12:25:16.912890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/mongo_s3_coordinates_with_collection_list.py
+-rw-r--r--   0        0        0     7509 2023-01-23 12:25:16.912890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/patch_data_catalog_options.py
+-rw-r--r--   0        0        0     4752 2023-01-23 12:25:16.912890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/patch_dictionary_options.py
+-rw-r--r--   0        0        0     5126 2023-01-23 12:25:16.912890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/patch_knowledge_graph_options.py
+-rw-r--r--   0        0        0     5142 2023-01-23 12:25:16.912890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/patch_knowledge_graph_options1.py
+-rw-r--r--   0        0        0     5026 2023-01-23 12:25:16.912890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/problem.py
+-rw-r--r--   0        0        0     4450 2023-01-23 12:25:16.912890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/processing_model.py
+-rw-r--r--   0        0        0     4495 2023-01-23 12:25:16.912890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/processing_model_data_flow.py
+-rw-r--r--   0        0        0     5450 2023-01-23 12:25:16.912890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/processing_model_description.py
+-rw-r--r--   0        0        0     6675 2023-01-23 12:25:16.912890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/project_data_index_non_view.py
+-rw-r--r--   0        0        0     4489 2023-01-23 12:25:16.912890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/project_data_index_source.py
+-rw-r--r--   0        0        0     6343 2023-01-23 12:25:16.912890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/project_data_index_view.py
+-rw-r--r--   0        0        0     8014 2023-01-23 12:25:16.912890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/project_data_index_view_of.py
+-rw-r--r--   0        0        0    13095 2023-01-23 12:25:16.912890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/project_data_index_with_status.py
+-rw-r--r--   0        0        0     6309 2023-01-23 12:25:16.912890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/project_data_index_with_status_view_of.py
+-rw-r--r--   0        0        0     4344 2023-01-23 12:25:16.912890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/project_default_values.py
+-rw-r--r--   0        0        0     5349 2023-01-23 12:25:16.912890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/project_default_values_ccs_project.py
+-rw-r--r--   0        0        0     4498 2023-01-23 12:25:16.912890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/project_default_values_dataflow.py
+-rw-r--r--   0        0        0     5428 2023-01-23 12:25:16.912890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/project_flavour_total_kgs.py
+-rw-r--r--   0        0        0     4447 2023-01-23 12:25:16.912890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/project_flavours.py
+-rw-r--r--   0        0        0     3800 2023-01-23 12:25:16.912890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/project_package_instalation_manifest.py
+-rw-r--r--   0        0        0     5089 2023-01-23 12:25:16.912890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/project_proj_key_annotate_document_report_document.py
+-rw-r--r--   0        0        0     4739 2023-01-23 12:25:16.912890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/project_proj_key_annotate_document_report_report.py
+-rw-r--r--   0        0        0     5683 2023-01-23 12:25:16.912890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/project_proj_key_bags_bag_key_tasks_assemble_dataflow_data_flow.py
+-rw-r--r--   0        0        0     4758 2023-01-23 12:25:16.912890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/project_proj_key_bags_bag_key_tasks_assemble_dataflow_data_flow_render_options.py
+-rw-r--r--   0        0        0     7904 2023-01-23 12:25:16.912890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/project_proj_key_bags_bag_key_tasks_export_dataset_info.py
+-rw-r--r--   0        0        0     5194 2023-01-23 12:25:16.912890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/project_proj_key_bags_bag_key_tasks_export_dataset_info_coords.py
+-rw-r--r--   0        0        0     7289 2023-01-23 12:25:16.912890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/project_proj_key_bags_bag_key_tasks_export_dataset_info_coords_node_collection.py
+-rw-r--r--   0        0        0     4602 2023-01-23 12:25:16.912890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/project_proj_key_bags_bag_key_tasks_export_dataset_info_node_list.py
+-rw-r--r--   0        0        0     3551 2023-01-23 12:25:16.912890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/project_proj_key_bags_bag_key_tasks_suspend_snapshot.py
+-rw-r--r--   0        0        0     8557 2023-01-23 12:25:16.912890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/project_proj_key_data_catalogues_dc_key_collections_collection_name_actions_import_ccs.py
+-rw-r--r--   0        0        0     8870 2023-01-23 12:25:16.912890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/project_proj_key_data_catalogues_dc_key_collections_collection_name_actions_import_ccs_export_package_mongo_options.py
+-rw-r--r--   0        0        0     6166 2023-01-23 12:25:16.912890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/project_proj_key_data_catalogues_dc_key_collections_collection_name_actions_import_ccs_export_package_mongo_options_assemble_options.py
+-rw-r--r--   0        0        0     7200 2023-01-23 12:25:16.912890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/project_proj_key_data_catalogues_dc_key_collections_collection_name_actions_import_ccs_export_package_mongo_options_assemble_options_mode.py
+-rw-r--r--   0        0        0     5022 2023-01-23 12:25:16.912890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/project_proj_key_data_catalogues_dc_key_collections_collection_name_actions_import_ccs_export_package_mongo_options_assemble_options_options.py
+-rw-r--r--   0        0        0     4442 2023-01-23 12:25:16.912890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/project_proj_key_data_catalogues_dc_key_collections_collection_name_actions_import_ccs_export_package_mongo_options_inputs.py
+-rw-r--r--   0        0        0     5911 2023-01-23 12:25:16.912890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/project_proj_key_data_catalogues_dc_key_collections_collection_name_actions_import_ccs_export_package_mongo_options_package_options.py
+-rw-r--r--   0        0        0     3951 2023-01-23 12:25:16.912890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/project_proj_key_data_catalogues_from_mongo_options.py
+-rw-r--r--   0        0        0     5398 2023-01-23 12:25:16.912890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/project_proj_key_data_catalogues_from_mongo_target.py
+-rw-r--r--   0        0        0     3668 2023-01-23 12:25:16.912890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/project_proj_key_data_catalogues_from_url_options.py
+-rw-r--r--   0        0        0     5654 2023-01-23 12:25:16.912890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/project_proj_key_dictionaries_from_mongo_target.py
+-rw-r--r--   0        0        0     4697 2023-01-23 12:25:16.912890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/project_proj_key_kgc_dataflow_templates_debug_df_tpl_key_target_bag.py
+-rw-r--r--   0        0        0     5212 2023-01-23 12:25:16.912890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/project_proj_key_kgc_dataflow_templates_df_tpl_key_actions_load_render.py
+-rw-r--r--   0        0        0     5093 2023-01-23 12:25:16.912890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/project_proj_key_kgc_dataflow_templates_df_tpl_key_actions_load_render_target_bag.py
+-rw-r--r--   0        0        0     3834 2023-01-23 12:25:16.912890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/project_proj_key_kgc_dataflow_templates_df_tpl_key_actions_load_target.py
+-rw-r--r--   0        0        0     4650 2023-01-23 12:25:16.912890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/project_proj_key_kgc_dataflow_templates_variables.py
+-rw-r--r--   0        0        0     5107 2023-01-23 12:25:16.912890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/project_proj_key_kgc_raw_dataflow_templates_actions_run_data_flow.py
+-rw-r--r--   0        0        0     4975 2023-01-23 12:25:16.912890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/project_proj_key_kgc_raw_dataflow_templates_actions_run_data_flow_template.py
+-rw-r--r--   0        0        0     3673 2023-01-23 12:25:16.912890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/project_proj_key_model_configs_configurations.py
+-rw-r--r--   0        0        0     4477 2023-01-23 12:25:16.912890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/project_proj_key_packages_packages.py
+-rw-r--r--   0        0        0     9337 2023-01-23 12:25:16.912890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/project_task.py
+-rw-r--r--   0        0        0     5224 2023-01-23 12:25:16.912890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/projects_flavours.py
+-rw-r--r--   0        0        0     4330 2023-01-23 12:25:16.912890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/projects_flavours_flavours.py
+-rw-r--r--   0        0        0     5229 2023-01-23 12:25:16.912890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/projects_flavours_quota.py
+-rw-r--r--   0        0        0     4336 2023-01-23 12:25:16.912890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/related_task.py
+-rw-r--r--   0        0        0     4453 2023-01-23 12:25:16.912890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/relationship_annotation_column.py
+-rw-r--r--   0        0        0     5513 2023-01-23 12:25:16.912890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/relationship_annotation_descriptor.py
+-rw-r--r--   0        0        0     4852 2023-01-23 12:25:16.912890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/render_data_flow_template_options.py
+-rw-r--r--   0        0        0     3680 2023-01-23 12:25:16.912890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/restore_knowledge_graph_backup_options.py
+-rw-r--r--   0        0        0     4435 2023-01-23 12:25:16.912890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/resume_knowledge_graph_options.py
+-rw-r--r--   0        0        0     4382 2023-01-23 12:25:16.912890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/run_data_flow_template_options.py
+-rw-r--r--   0        0        0     5772 2023-01-23 12:25:16.912890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/run_data_flow_template_options1.py
+-rw-r--r--   0        0        0     9951 2023-01-23 12:25:16.912890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/s3_coordinates.py
+-rw-r--r--   0        0        0    10201 2023-01-23 12:25:16.912890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/s3_coordinates_with_backup_key.py
+-rw-r--r--   0        0        0     4519 2023-01-23 12:25:16.912890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/s3_coordinates_with_backup_key_presigned.py
+-rw-r--r--   0        0        0     8194 2023-01-23 12:25:16.912890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/storage_summary_dc.py
+-rw-r--r--   0        0        0     9388 2023-01-23 12:25:16.912890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/storage_summary_kg.py
+-rw-r--r--   0        0        0     7367 2023-01-23 12:25:16.912890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/storage_summary_kg_categories_fraction.py
+-rw-r--r--   0        0        0     6790 2023-01-23 12:25:16.912890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/storage_summary_task.py
+-rw-r--r--   0        0        0     5872 2023-01-23 12:25:16.912890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/supported_annotator_annotations.py
+-rw-r--r--   0        0        0     4593 2023-01-23 12:25:16.916890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/suspend_knowledge_graph_options.py
+-rw-r--r--   0        0        0     5710 2023-01-23 12:25:16.916890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/system_celery_tasks_failure_failures.py
+-rw-r--r--   0        0        0     5341 2023-01-23 12:25:16.916890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/system_info.py
+-rw-r--r--   0        0        0     4785 2023-01-23 12:25:16.916890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/system_info_api.py
+-rw-r--r--   0        0        0     6788 2023-01-23 12:25:16.916890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/system_info_deployment.py
+-rw-r--r--   0        0        0     4255 2023-01-23 12:25:16.916890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/system_info_deployment_linked_ccs_api.py
+-rw-r--r--   0        0        0     4148 2023-01-23 12:25:16.916890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/system_kgs_backend.py
+-rw-r--r--   0        0        0     5454 2023-01-23 12:25:16.916890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/system_kgs_deployment.py
+-rw-r--r--   0        0        0     4202 2023-01-23 12:25:16.916890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/system_kgs_deployment_resources.py
+-rw-r--r--   0        0        0     6464 2023-01-23 12:25:16.916890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/system_modules_configuration.py
+-rw-r--r--   0        0        0     3456 2023-01-23 12:25:16.916890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/system_modules_tasks.py
+-rw-r--r--   0        0        0     3432 2023-01-23 12:25:16.916890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/system_modules_tasks_tasks.py
+-rw-r--r--   0        0        0     5238 2023-01-23 12:25:16.916890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/take_snapshot_settings.py
+-rw-r--r--   0        0        0     5652 2023-01-23 12:25:16.916890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/take_snapshot_settings_backend_aware.py
+-rw-r--r--   0        0        0     8365 2023-01-23 12:25:16.916890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/task.py
+-rw-r--r--   0        0        0     9820 2023-01-23 12:25:16.916890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/temporary_upload_file_result.py
+-rw-r--r--   0        0        0     3443 2023-01-23 12:25:16.916890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/temporary_upload_file_result_download.py
+-rw-r--r--   0        0        0     3499 2023-01-23 12:25:16.916890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/temporary_upload_file_result_download_private.py
+-rw-r--r--   0        0        0     3443 2023-01-23 12:25:16.916890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/temporary_upload_file_result_metadata.py
+-rw-r--r--   0        0        0     3499 2023-01-23 12:25:16.916890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/temporary_upload_file_result_metadata_private.py
+-rw-r--r--   0        0        0     4129 2023-01-23 12:25:16.916890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/temporary_upload_file_result_upload.py
+-rw-r--r--   0        0        0     4213 2023-01-23 12:25:16.916890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/temporary_upload_file_result_upload_private.py
+-rw-r--r--   0        0        0     3478 2023-01-23 12:25:16.916890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/token_response.py
+-rw-r--r--   0        0        0     4369 2023-01-23 12:25:16.916890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/topology.py
+-rw-r--r--   0        0        0     5031 2023-01-23 12:25:16.916890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/topology_edge.py
+-rw-r--r--   0        0        0     3449 2023-01-23 12:25:16.916890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/topology_node.py
+-rw-r--r--   0        0        0     7001 2023-01-23 12:25:16.916890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/update_data_flow_options.py
+-rw-r--r--   0        0        0     6334 2023-01-23 12:25:16.916890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/update_project_model_config_options.py
+-rw-r--r--   0        0        0     6790 2023-01-23 12:25:16.916890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/uploaded_file.py
+-rw-r--r--   0        0        0     4401 2023-01-23 12:25:16.916890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/uploaded_file_result.py
+-rw-r--r--   0        0        0     4717 2023-01-23 12:25:16.916890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/usage_stats.py
+-rw-r--r--   0        0        0     5319 2023-01-23 12:25:16.916890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/well_known_df_template_variable.py
+-rw-r--r--   0        0        0    12356 2023-01-23 12:25:16.916890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/rest.py
+-rw-r--r--   0        0        0     2773 2023-01-23 12:25:16.916890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/user/__init__.py
+-rw-r--r--   0        0        0      455 2023-01-23 12:25:16.916890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/user/api/__init__.py
+-rw-r--r--   0        0        0    20416 2023-01-23 12:25:16.916890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/user/api/admin_api.py
+-rw-r--r--   0        0        0    19855 2023-01-23 12:25:16.916890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/user/api/oidc_api.py
+-rw-r--r--   0        0        0    71698 2023-01-23 12:25:16.916890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/user/api/projects_api.py
+-rw-r--r--   0        0        0     5208 2023-01-23 12:25:16.916890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/user/api/settings_api.py
+-rw-r--r--   0        0        0     5135 2023-01-23 12:25:16.916890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/user/api/user_api.py
+-rw-r--r--   0        0        0    33259 2023-01-23 12:25:16.916890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/user/api/users_api.py
+-rw-r--r--   0        0        0    26301 2023-01-23 12:25:16.916890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/user/api_client.py
+-rw-r--r--   0        0        0    14021 2023-01-23 12:25:16.916890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/user/configuration.py
+-rw-r--r--   0        0        0     3796 2023-01-23 12:25:16.916890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/user/exceptions.py
+-rw-r--r--   0        0        0     1899 2023-01-23 12:25:16.916890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/user/models/__init__.py
+-rw-r--r--   0        0        0     3429 2023-01-23 12:25:16.916890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/user/models/access_token.py
+-rw-r--r--   0        0        0     4019 2023-01-23 12:25:16.916890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/user/models/api_key.py
+-rw-r--r--   0        0        0     7956 2023-01-23 12:25:16.916890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/user/models/audit_record.py
+-rw-r--r--   0        0        0     4516 2023-01-23 12:25:16.916890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/user/models/create_project_request_body.py
+-rw-r--r--   0        0        0     4336 2023-01-23 12:25:16.916890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/user/models/create_tokens_request_body.py
+-rw-r--r--   0        0        0     3556 2023-01-23 12:25:16.916890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/user/models/error_response.py
+-rw-r--r--   0        0        0     3405 2023-01-23 12:25:16.916890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/user/models/get_access_token_request_body.py
+-rw-r--r--   0        0        0     4915 2023-01-23 12:25:16.916890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/user/models/impersonate_user_token_request_body.py
+-rw-r--r--   0        0        0     3555 2023-01-23 12:25:16.916890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/user/models/inline_response200.py
+-rw-r--r--   0        0        0     5252 2023-01-23 12:25:16.916890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/user/models/oidc_token_response.py
+-rw-r--r--   0        0        0     5003 2023-01-23 12:25:16.916890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/user/models/project.py
+-rw-r--r--   0        0        0     4530 2023-01-23 12:25:16.916890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/user/models/project_user_assignment.py
+-rw-r--r--   0        0        0     4790 2023-01-23 12:25:16.916890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/user/models/register_user_request_body.py
+-rw-r--r--   0        0        0     4907 2023-01-23 12:25:16.916890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/user/models/service_account.py
+-rw-r--r--   0        0        0     4486 2023-01-23 12:25:16.916890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/user/models/service_account_credentials.py
+-rw-r--r--   0        0        0     3602 2023-01-23 12:25:16.916890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/user/models/success_message.py
+-rw-r--r--   0        0        0     3566 2023-01-23 12:25:16.916890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/user/models/token_response.py
+-rw-r--r--   0        0        0     4515 2023-01-23 12:25:16.916890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/user/models/user_details.py
+-rw-r--r--   0        0        0     2827 2023-01-23 12:25:16.916890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/user/models/user_type.py
+-rw-r--r--   0        0        0    12338 2023-01-23 12:25:16.916890 deepsearch_toolkit-0.9.0/deepsearch/cps/apis/user/rest.py
+-rw-r--r--   0        0        0      110 2023-01-23 12:25:16.916890 deepsearch_toolkit-0.9.0/deepsearch/cps/cli/__init__.py
+-rw-r--r--   0        0        0     1119 2023-01-23 12:25:16.916890 deepsearch_toolkit-0.9.0/deepsearch/cps/cli/cli_options.py
+-rw-r--r--   0        0        0     3937 2023-01-23 12:25:16.916890 deepsearch_toolkit-0.9.0/deepsearch/cps/cli/data_indices_typer.py
+-rw-r--r--   0        0        0      983 2023-01-23 12:25:16.916890 deepsearch_toolkit-0.9.0/deepsearch/cps/cli/elastic_data.py
+-rw-r--r--   0        0        0     3310 2023-01-23 12:25:16.916890 deepsearch_toolkit-0.9.0/deepsearch/cps/cli/kgs.py
+-rw-r--r--   0        0        0      595 2023-01-23 12:25:16.916890 deepsearch_toolkit-0.9.0/deepsearch/cps/cli/main.py
+-rw-r--r--   0        0        0     1705 2023-01-23 12:25:16.916890 deepsearch_toolkit-0.9.0/deepsearch/cps/cli/projects.py
+-rw-r--r--   0        0        0       76 2023-01-23 12:25:16.916890 deepsearch_toolkit-0.9.0/deepsearch/cps/client/__init__.py
+-rw-r--r--   0        0        0     5758 2023-01-23 12:25:16.916890 deepsearch_toolkit-0.9.0/deepsearch/cps/client/api.py
+-rw-r--r--   0        0        0        0 2023-01-23 12:25:16.916890 deepsearch_toolkit-0.9.0/deepsearch/cps/client/builders/__init__.py
+-rw-r--r--   0        0        0     2207 2023-01-23 12:25:16.916890 deepsearch_toolkit-0.9.0/deepsearch/cps/client/builders/wf_builder.py
+-rw-r--r--   0        0        0      458 2023-01-23 12:25:16.916890 deepsearch_toolkit-0.9.0/deepsearch/cps/client/components/__init__.py
+-rw-r--r--   0        0        0      222 2023-01-23 12:25:16.916890 deepsearch_toolkit-0.9.0/deepsearch/cps/client/components/api_object.py
+-rw-r--r--   0        0        0     5223 2023-01-23 12:25:16.920890 deepsearch_toolkit-0.9.0/deepsearch/cps/client/components/data_catalogs.py
+-rw-r--r--   0        0        0     3891 2023-01-23 12:25:16.920890 deepsearch_toolkit-0.9.0/deepsearch/cps/client/components/data_indices.py
+-rw-r--r--   0        0        0     4486 2023-01-23 12:25:16.920890 deepsearch_toolkit-0.9.0/deepsearch/cps/client/components/documents.py
+-rw-r--r--   0        0        0     4964 2023-01-23 12:25:16.920890 deepsearch_toolkit-0.9.0/deepsearch/cps/client/components/elastic.py
+-rw-r--r--   0        0        0     4354 2023-01-23 12:25:16.920890 deepsearch_toolkit-0.9.0/deepsearch/cps/client/components/knowledge_graphs.py
+-rw-r--r--   0        0        0     2632 2023-01-23 12:25:16.920890 deepsearch_toolkit-0.9.0/deepsearch/cps/client/components/projects.py
+-rw-r--r--   0        0        0     3866 2023-01-23 12:25:16.920890 deepsearch_toolkit-0.9.0/deepsearch/cps/client/components/queries.py
+-rw-r--r--   0        0        0     1002 2023-01-23 12:25:16.920890 deepsearch_toolkit-0.9.0/deepsearch/cps/client/components/tasks.py
+-rw-r--r--   0        0        0      135 2023-01-23 12:25:16.920890 deepsearch_toolkit-0.9.0/deepsearch/cps/client/queries/__init__.py
+-rw-r--r--   0        0        0     3171 2023-01-23 12:25:16.920890 deepsearch_toolkit-0.9.0/deepsearch/cps/client/queries/query.py
+-rw-r--r--   0        0        0       96 2023-01-23 12:25:16.920890 deepsearch_toolkit-0.9.0/deepsearch/cps/client/queries/query_tasks/__init__.py
+-rw-r--r--   0        0        0     1646 2023-01-23 12:25:16.920890 deepsearch_toolkit-0.9.0/deepsearch/cps/client/queries/query_tasks/for_each.py
+-rw-r--r--   0        0        0     1245 2023-01-23 12:25:16.920890 deepsearch_toolkit-0.9.0/deepsearch/cps/client/queries/query_tasks/workflow.py
+-rw-r--r--   0        0        0     3790 2023-01-23 12:25:16.920890 deepsearch_toolkit-0.9.0/deepsearch/cps/client/queries/task.py
+-rw-r--r--   0        0        0       32 2023-01-23 12:25:16.920890 deepsearch_toolkit-0.9.0/deepsearch/cps/data_indices/__init__.py
+-rw-r--r--   0        0        0     4854 2023-01-23 12:25:16.920890 deepsearch_toolkit-0.9.0/deepsearch/cps/data_indices/utils.py
+-rw-r--r--   0        0        0      687 2023-01-23 12:25:16.920890 deepsearch_toolkit-0.9.0/deepsearch/cps/ipython/__init__.py
+-rw-r--r--   0        0        0     1961 2023-01-23 12:25:16.920890 deepsearch_toolkit-0.9.0/deepsearch/cps/ipython/kg_helpers.py
+-rw-r--r--   0        0        0     4159 2023-01-23 12:25:16.920890 deepsearch_toolkit-0.9.0/deepsearch/cps/ipython/kg_widgets.py
+-rw-r--r--   0        0        0        0 2023-01-23 12:25:16.920890 deepsearch_toolkit-0.9.0/deepsearch/cps/kg/__init__.py
+-rw-r--r--   0        0        0     2708 2023-01-23 12:25:16.920890 deepsearch_toolkit-0.9.0/deepsearch/cps/kg/workflow/MultiLinkedList.py
+-rw-r--r--   0        0        0       88 2023-01-23 12:25:16.920890 deepsearch_toolkit-0.9.0/deepsearch/cps/kg/workflow/__init__.py
+-rw-r--r--   0        0        0     1594 2023-01-23 12:25:16.920890 deepsearch_toolkit-0.9.0/deepsearch/cps/kg/workflow/wf_functions.py
+-rw-r--r--   0        0        0    17480 2023-01-23 12:25:16.920890 deepsearch_toolkit-0.9.0/deepsearch/cps/kg/workflow/workflow.py
+-rw-r--r--   0        0        0     1941 2023-01-23 12:25:16.920890 deepsearch_toolkit-0.9.0/deepsearch/cps/queries/__init__.py
+-rw-r--r--   0        0        0       36 2023-01-23 12:25:16.920890 deepsearch_toolkit-0.9.0/deepsearch/documents/__init__.py
+-rw-r--r--   0        0        0        1 2023-01-23 12:25:16.920890 deepsearch_toolkit-0.9.0/deepsearch/documents/cli/__init__.py
+-rw-r--r--   0        0        0     3728 2023-01-23 12:25:16.920890 deepsearch_toolkit-0.9.0/deepsearch/documents/cli/main.py
+-rw-r--r--   0        0        0       36 2023-01-23 12:25:16.920890 deepsearch_toolkit-0.9.0/deepsearch/documents/core/__init__.py
+-rw-r--r--   0        0        0      549 2023-01-23 12:25:16.920890 deepsearch_toolkit-0.9.0/deepsearch/documents/core/common_routines.py
+-rw-r--r--   0        0        0     8751 2023-01-23 12:25:16.920890 deepsearch_toolkit-0.9.0/deepsearch/documents/core/convert.py
+-rw-r--r--   0        0        0     4012 2023-01-23 12:25:16.920890 deepsearch_toolkit-0.9.0/deepsearch/documents/core/create_report.py
+-rw-r--r--   0        0        0     2796 2023-01-23 12:25:16.920890 deepsearch_toolkit-0.9.0/deepsearch/documents/core/input_process.py
+-rw-r--r--   0        0        0     2598 2023-01-23 12:25:16.920890 deepsearch_toolkit-0.9.0/deepsearch/documents/core/main.py
+-rw-r--r--   0        0        0     9809 2023-01-23 12:25:16.920890 deepsearch_toolkit-0.9.0/deepsearch/documents/core/models.py
+-rw-r--r--   0        0        0     8384 2023-01-23 12:25:16.920890 deepsearch_toolkit-0.9.0/deepsearch/documents/core/utils.py
+-rw-r--r--   0        0        0        0 2023-01-23 12:25:16.920890 deepsearch_toolkit-0.9.0/deepsearch/plugins/__init__.py
+-rw-r--r--   0        0        0      656 2023-01-23 12:25:16.920890 deepsearch_toolkit-0.9.0/deepsearch/plugins/example_toy_cli_plugin.py
+-rw-r--r--   0        0        0        0 2023-01-23 12:25:16.920890 deepsearch_toolkit-0.9.0/deepsearch/py.typed
+-rw-r--r--   0        0        0        0 2023-01-23 12:25:16.920890 deepsearch_toolkit-0.9.0/deepsearch/query/__init__.py
+-rw-r--r--   0        0        0        0 2023-01-23 12:25:16.920890 deepsearch_toolkit-0.9.0/deepsearch/query/cli/__init__.py
+-rw-r--r--   0        0        0     4210 2023-01-23 12:25:16.920890 deepsearch_toolkit-0.9.0/deepsearch/query/cli/main.py
+-rw-r--r--   0        0        0     4367 2023-01-23 12:25:16.940889 deepsearch_toolkit-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     5414 1970-01-01 00:00:00.000000 deepsearch_toolkit-0.9.0/setup.py
+-rw-r--r--   0        0        0     4928 1970-01-01 00:00:00.000000 deepsearch_toolkit-0.9.0/PKG-INFO
```

### Comparing `deepsearch_toolkit-0.8.0/LICENSE` & `deepsearch_toolkit-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/README.md` & `deepsearch_toolkit-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cli.py` & `deepsearch_toolkit-0.9.0/deepsearch/cli.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/core/cli/config.py` & `deepsearch_toolkit-0.9.0/deepsearch/core/cli/config.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/core/cli/login.py` & `deepsearch_toolkit-0.9.0/deepsearch/core/cli/login.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/core/cli/main.py` & `deepsearch_toolkit-0.9.0/deepsearch/core/cli/main.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/core/cli/plugins.py` & `deepsearch_toolkit-0.9.0/deepsearch/core/cli/plugins.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/core/util/ccs_utils.py` & `deepsearch_toolkit-0.9.0/deepsearch/core/util/ccs_utils.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/core/util/config_paths.py` & `deepsearch_toolkit-0.9.0/deepsearch/core/util/config_paths.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/kg/create/__init__.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/kg/create/__init__.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/kg/create/api/edges_api.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/kg/create/api/edges_api.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/kg/create/api/indices_api.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/kg/create/api/indices_api.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/kg/create/api/knowledge_graphs_api.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/kg/create/api/knowledge_graphs_api.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/kg/create/api/nodes_api.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/kg/create/api/nodes_api.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/kg/create/api/tasks_api.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/kg/create/api/tasks_api.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/kg/create/api_client.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/kg/create/api_client.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/kg/create/configuration.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/kg/create/configuration.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/kg/create/exceptions.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/kg/create/exceptions.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/kg/create/models/__init__.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/kg/create/models/__init__.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/kg/create/models/database_source.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/kg/create/models/database_source.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/kg/create/models/database_source_mongo.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/kg/create/models/database_source_mongo.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/kg/create/models/database_source_s3.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/kg/create/models/database_source_s3.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/kg/create/models/edge_matrix.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/kg/create/models/edge_matrix.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/kg/create/models/edge_model.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/kg/create/models/edge_model.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/kg/create/models/inline_object.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/kg/create/models/inline_object.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/kg/create/models/inline_object1.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/kg/create/models/inline_object1.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/kg/create/models/inline_object2.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/kg/create/models/inline_object2.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/kg/create/models/mongo_edge.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/kg/create/models/mongo_edge.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/kg/create/models/mongo_edge_item.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/kg/create/models/mongo_edge_item.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/kg/create/models/node.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/kg/create/models/node.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/kg/create/models/s3_source.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/kg/create/models/s3_source.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/kg/create/models/sparse_matrix_with_names_or_hashes.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/kg/create/models/sparse_matrix_with_names_or_hashes.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/kg/create/models/triplet.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/kg/create/models/triplet.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/kg/create/rest.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/kg/create/rest.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/kg/query/__init__.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/kg/query/__init__.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/kg/query/api/__init__.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/kg/query/api/__init__.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/kg/query/api/description_api.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/kg/query/api/description_api.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/kg/query/api/inspect_api.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/kg/query/api/inspect_api.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/kg/query/api/node_data_retrieval_api.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/kg/query/api/node_data_retrieval_api.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/kg/query/api/node_retrieval_api.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/kg/query/api/node_retrieval_api.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/kg/query/api/node_search_api.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/kg/query/api/node_search_api.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/kg/query/api/query_api.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/kg/query/api/query_api.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/kg/query/api_client.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/kg/query/api_client.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/kg/query/configuration.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/kg/query/configuration.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/kg/query/exceptions.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/kg/query/exceptions.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/kg/query/models/__init__.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/kg/query/models/__init__.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/kg/query/models/auth_config.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/kg/query/models/auth_config.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/kg/query/models/error_model.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/kg/query/models/error_model.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/kg/query/models/graph_description.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/kg/query/models/graph_description.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/kg/query/models/graph_edge.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/kg/query/models/graph_edge.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/kg/query/models/graph_matrix.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/kg/query/models/graph_matrix.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/kg/query/models/graph_node_description.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/kg/query/models/graph_node_description.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/kg/query/models/graph_node_description_categories.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/kg/query/models/graph_node_description_categories.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/kg/query/models/inline_object.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/kg/query/models/inline_object.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/kg/query/models/node.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/kg/query/models/node.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/kg/query/models/nodes_response_model.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/kg/query/models/nodes_response_model.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/kg/query/models/nodes_response_model_all_of.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/kg/query/models/nodes_response_model_all_of.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/kg/query/models/nodes_response_model_all_of_response.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/kg/query/models/nodes_response_model_all_of_response.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/kg/query/models/response_model.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/kg/query/models/response_model.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/kg/query/models/workflow_response.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/kg/query/models/workflow_response.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/kg/query/models/workflow_response_model.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/kg/query/models/workflow_response_model.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/kg/query/models/workflow_response_model_all_of.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/kg/query/models/workflow_response_model_all_of.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/kg/query/models/workflow_response_node.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/kg/query/models/workflow_response_node.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/kg/query/rest.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/kg/query/rest.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/__init__.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/__init__.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/api/__init__.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/api/__init__.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/api/annotate_api.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/api/annotate_api.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/api/data_catalogs_api.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/api/data_catalogs_api.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/api/data_flows_api.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/api/data_flows_api.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/api/data_indices_api.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/api/data_indices_api.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/api/dictionaries_api.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/api/dictionaries_api.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/api/document_annotation_api.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/api/document_annotation_api.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/api/elastic_api.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/api/elastic_api.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/api/knowledge_graphs_api.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/api/knowledge_graphs_api.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/api/model_configurations_api.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/api/model_configurations_api.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/api/processing_model_api.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/api/processing_model_api.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/api/project_api.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/api/project_api.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/api/system_api.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/api/system_api.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/api/tasks_api.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/api/tasks_api.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/api/uploads_api.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/api/uploads_api.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/api_client.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/api_client.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/configuration.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/configuration.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/exceptions.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/exceptions.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/__init__.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/__init__.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/annotate_document_request.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/annotate_document_request.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/annotate_object_options.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/annotate_object_options.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/annotate_object_options1.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/annotate_object_options1.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/annotated_document_report.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/annotated_document_report.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/annotated_image.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/annotated_image.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/annotated_object.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/annotated_object.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/annotated_object1.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/annotated_object1.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/annotated_table.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/annotated_table.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/annotated_text.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/annotated_text.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/annotated_text_lines.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/annotated_text_lines.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/annotator_image_input.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/annotator_image_input.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/annotator_input.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/annotator_input.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/annotator_metadata.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/annotator_metadata.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/annotator_parameters_or_ref.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/annotator_parameters_or_ref.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/annotator_supported_annotations_parameters.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/annotator_supported_annotations_parameters.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/assemble_data_flow_into_knowledge_graph_options.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/assemble_data_flow_into_knowledge_graph_options.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/assemble_data_flow_into_knowledge_graph_options1.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/assemble_data_flow_into_knowledge_graph_options1.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/backend_flavour.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/backend_flavour.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/backend_project_proj_key_bags_bag_key_tasks_assemble_dataflow_data_flow.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/backend_project_proj_key_bags_bag_key_tasks_assemble_dataflow_data_flow.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/backend_project_proj_key_bags_bag_key_tasks_assemble_dataflow_data_flow_raw_data_flow.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/backend_project_proj_key_bags_bag_key_tasks_assemble_dataflow_data_flow_raw_data_flow.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/backend_project_proj_key_bags_bag_key_tasks_assemble_dataflow_render.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/backend_project_proj_key_bags_bag_key_tasks_assemble_dataflow_render.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/backup_knowledge_graph_options.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/backup_knowledge_graph_options.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/bag.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/bag.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/bag_amqp_backend.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/bag_amqp_backend.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/bag_backend_aware.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/bag_backend_aware.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/bag_backends.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/bag_backends.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/bag_callback.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/bag_callback.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/bag_component_status.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/bag_component_status.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/bag_component_status_enum.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/bag_component_status_enum.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/bag_flavour.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/bag_flavour.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/bag_flavour_default_quota.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/bag_flavour_default_quota.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/bag_flavour_full_data.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/bag_flavour_full_data.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/bag_kg_legacy_api_backend.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/bag_kg_legacy_api_backend.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/bag_status.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/bag_status.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/bag_status_backend_aware.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/bag_status_backend_aware.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/bag_status_backend_aware_kg_amqp.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/bag_status_backend_aware_kg_amqp.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/bag_status_components.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/bag_status_components.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/catalog_reference.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/catalog_reference.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/ccs_collection_reference.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/ccs_collection_reference.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/ccs_task.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/ccs_task.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/celery_task.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/celery_task.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/celery_task1.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/celery_task1.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/celery_task_promise.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/celery_task_promise.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/clone_data_catalog_options.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/clone_data_catalog_options.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/clone_data_catalog_result.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/clone_data_catalog_result.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/clone_dictionary_options.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/clone_dictionary_options.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/clone_public_data_catalog_options.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/clone_public_data_catalog_options.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/clone_public_dictionary_options.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/clone_public_dictionary_options.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/collection_list_coordinates.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/collection_list_coordinates.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/cps_model_reference.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/cps_model_reference.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/cps_package.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/cps_package.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/create_collection_in_dictionary_options.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/create_collection_in_dictionary_options.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/create_data_catalog_collection_options.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/create_data_catalog_collection_options.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/create_data_catalog_options.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/create_data_catalog_options.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/create_data_flow_template_options.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/create_data_flow_template_options.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/create_dictionary_options.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/create_dictionary_options.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/create_knowledge_graph_options.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/create_knowledge_graph_options.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/create_knowledge_graph_options1.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/create_knowledge_graph_options1.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/create_project_model_config_options.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/create_project_model_config_options.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/data_catalog_category_schema.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/data_catalog_category_schema.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/data_catalog_collection.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/data_catalog_collection.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/data_catalog_data_flow.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/data_catalog_data_flow.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/data_catalog_import_options.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/data_catalog_import_options.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/data_catalog_import_result.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/data_catalog_import_result.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/data_catalog_provenance_log.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/data_catalog_provenance_log.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/data_catalog_provenance_log_source.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/data_catalog_provenance_log_source.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/data_catalog_provenance_log_user.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/data_catalog_provenance_log_user.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/data_catalog_schema.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/data_catalog_schema.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/data_catalog_topology.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/data_catalog_topology.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/data_catalog_topology_edge.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/data_catalog_topology_edge.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/data_catalog_topology_node.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/data_catalog_topology_node.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/data_catalog_url_import_options.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/data_catalog_url_import_options.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/data_catalogue.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/data_catalogue.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/data_collection.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/data_collection.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/data_collection_metadata.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/data_collection_metadata.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/data_collection_source.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/data_collection_source.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/data_flow.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/data_flow.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/data_flow_assemble_into_knowledge_graph_task.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/data_flow_assemble_into_knowledge_graph_task.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/data_flow_assemble_report.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/data_flow_assemble_report.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/data_flow_assemble_report_cause.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/data_flow_assemble_report_cause.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/data_flow_assemble_report_chunks.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/data_flow_assemble_report_chunks.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/data_flow_assemble_report_errors.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/data_flow_assemble_report_errors.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/data_flow_assemble_report_options.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/data_flow_assemble_report_options.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/data_flow_assemble_report_single_task.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/data_flow_assemble_report_single_task.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/data_flow_load_into_knowledge_graph_task.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/data_flow_load_into_knowledge_graph_task.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/data_flow_template.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/data_flow_template.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/data_flow_template_list_item.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/data_flow_template_list_item.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/data_flow_template_variable.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/data_flow_template_variable.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/data_flow_topology_options.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/data_flow_topology_options.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/data_index_upload_file_source.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/data_index_upload_file_source.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/dictionary.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/dictionary.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/dictionary_clone_result.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/dictionary_clone_result.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/dictionary_collection.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/dictionary_collection.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/dictionary_collection_csv_data.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/dictionary_collection_csv_data.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/dictionary_collection_patch.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/dictionary_collection_patch.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/dictionary_entry.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/dictionary_entry.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/dictionary_import_options.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/dictionary_import_options.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/dictionary_import_result.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/dictionary_import_result.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/elastic_coordinates.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/elastic_coordinates.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/elastic_index_search_query_options.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/elastic_index_search_query_options.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/elastic_index_search_results.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/elastic_index_search_results.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/entity_annotation.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/entity_annotation.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/entity_annotation_descriptor.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/entity_annotation_descriptor.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/error_response.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/error_response.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/flavours_quota.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/flavours_quota.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/fully_rendered_data_flow.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/fully_rendered_data_flow.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/image_cells.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/image_cells.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/image_info.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/image_info.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/image_metadata.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/image_metadata.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/image_source.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/image_source.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/import_from_elastic_to_data_catalog_options.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/import_from_elastic_to_data_catalog_options.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/import_from_elastic_to_data_catalog_options_parameters.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/import_from_elastic_to_data_catalog_options_parameters.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/import_from_elastic_to_data_catalog_options_parameters_query_options.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/import_from_elastic_to_data_catalog_options_parameters_query_options.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/import_from_elastic_to_data_catalog_s3_coords.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/import_from_elastic_to_data_catalog_s3_coords.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/import_to_data_catalog_collection_options.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/import_to_data_catalog_collection_options.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/import_to_data_catalog_options.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/import_to_data_catalog_options.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/infer_project_data_catalog_category_schema.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/infer_project_data_catalog_category_schema.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/inline_object.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/inline_object.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/inline_object1.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/inline_object1.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/inline_object2.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/inline_object2.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/inline_object3.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/inline_object3.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/inline_response200.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/inline_response200.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/inline_response2001.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/inline_response2001.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/inline_response2002.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/inline_response2002.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/inline_response2003.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/inline_response2003.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/inspection_report.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/inspection_report.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/kg_snapshot.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/kg_snapshot.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/kgc_data_input.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/kgc_data_input.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/kibana_saved_queries_result.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/kibana_saved_queries_result.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/knowledge_graph_authentication_callback.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/knowledge_graph_authentication_callback.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/knowledge_graph_chart_upgrade_options.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/knowledge_graph_chart_upgrade_options.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/knowledge_graph_deployment_recreation_options.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/knowledge_graph_deployment_recreation_options.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/knowledge_graph_snapshot_options.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/knowledge_graph_snapshot_options.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/knowledge_graph_system_information.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/knowledge_graph_system_information.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/linked_ccs_instances.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/linked_ccs_instances.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/load_data_flow_into_knowledge_graph_options.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/load_data_flow_into_knowledge_graph_options.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/load_data_flow_into_knowledge_graph_options1.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/load_data_flow_into_knowledge_graph_options1.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/load_kgc_data_input.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/load_kgc_data_input.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/load_kgc_data_input_dataflow.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/load_kgc_data_input_dataflow.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/load_kgc_data_input_target.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/load_kgc_data_input_target.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/model_configuration.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/model_configuration.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/model_supported_annotations_parameters.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/model_supported_annotations_parameters.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/mongo_coordinates.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/mongo_coordinates.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/mongo_s3_coordinates.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/mongo_s3_coordinates.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/mongo_s3_coordinates_with_collection_list.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/mongo_s3_coordinates_with_collection_list.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/patch_data_catalog_options.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/patch_data_catalog_options.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/patch_dictionary_options.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/patch_dictionary_options.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/patch_knowledge_graph_options.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/patch_knowledge_graph_options.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/patch_knowledge_graph_options1.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/patch_knowledge_graph_options1.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/problem.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/problem.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/processing_model.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/processing_model.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/processing_model_data_flow.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/processing_model_data_flow.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/processing_model_description.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/processing_model_description.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/project_data_index_non_view.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/project_data_index_non_view.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/project_data_index_source.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/project_data_index_source.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/project_data_index_view.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/project_data_index_view.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/project_data_index_view_of.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/project_data_index_view_of.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/project_data_index_with_status.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/project_data_index_with_status.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/project_data_index_with_status_view_of.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/project_data_index_with_status_view_of.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/project_default_values.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/project_default_values.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/project_default_values_ccs_project.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/project_default_values_ccs_project.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/project_default_values_dataflow.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/project_default_values_dataflow.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/project_flavour_total_kgs.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/project_flavour_total_kgs.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/project_flavours.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/project_flavours.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/project_package_instalation_manifest.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/project_package_instalation_manifest.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/project_proj_key_annotate_document_report_document.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/project_proj_key_annotate_document_report_document.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/project_proj_key_annotate_document_report_report.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/project_proj_key_annotate_document_report_report.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/project_proj_key_bags_bag_key_tasks_assemble_dataflow_data_flow.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/project_proj_key_bags_bag_key_tasks_assemble_dataflow_data_flow.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/project_proj_key_bags_bag_key_tasks_assemble_dataflow_data_flow_render_options.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/project_proj_key_bags_bag_key_tasks_assemble_dataflow_data_flow_render_options.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/project_proj_key_bags_bag_key_tasks_export_dataset_info.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/project_proj_key_bags_bag_key_tasks_export_dataset_info.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/project_proj_key_bags_bag_key_tasks_export_dataset_info_coords.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/project_proj_key_bags_bag_key_tasks_export_dataset_info_coords.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/project_proj_key_bags_bag_key_tasks_export_dataset_info_coords_node_collection.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/project_proj_key_bags_bag_key_tasks_export_dataset_info_coords_node_collection.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/project_proj_key_bags_bag_key_tasks_export_dataset_info_node_list.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/project_proj_key_bags_bag_key_tasks_export_dataset_info_node_list.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/project_proj_key_bags_bag_key_tasks_suspend_snapshot.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/project_proj_key_bags_bag_key_tasks_suspend_snapshot.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/project_proj_key_data_catalogues_dc_key_collections_collection_name_actions_import_ccs.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/project_proj_key_data_catalogues_dc_key_collections_collection_name_actions_import_ccs.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/project_proj_key_data_catalogues_dc_key_collections_collection_name_actions_import_ccs_export_package_mongo_options.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/project_proj_key_data_catalogues_dc_key_collections_collection_name_actions_import_ccs_export_package_mongo_options.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/project_proj_key_data_catalogues_dc_key_collections_collection_name_actions_import_ccs_export_package_mongo_options_assemble_options.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/project_proj_key_data_catalogues_dc_key_collections_collection_name_actions_import_ccs_export_package_mongo_options_assemble_options.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/project_proj_key_data_catalogues_dc_key_collections_collection_name_actions_import_ccs_export_package_mongo_options_assemble_options_mode.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/project_proj_key_data_catalogues_dc_key_collections_collection_name_actions_import_ccs_export_package_mongo_options_assemble_options_mode.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/project_proj_key_data_catalogues_dc_key_collections_collection_name_actions_import_ccs_export_package_mongo_options_assemble_options_options.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/project_proj_key_data_catalogues_dc_key_collections_collection_name_actions_import_ccs_export_package_mongo_options_assemble_options_options.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/project_proj_key_data_catalogues_dc_key_collections_collection_name_actions_import_ccs_export_package_mongo_options_inputs.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/project_proj_key_data_catalogues_dc_key_collections_collection_name_actions_import_ccs_export_package_mongo_options_inputs.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/project_proj_key_data_catalogues_dc_key_collections_collection_name_actions_import_ccs_export_package_mongo_options_package_options.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/project_proj_key_data_catalogues_dc_key_collections_collection_name_actions_import_ccs_export_package_mongo_options_package_options.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/project_proj_key_data_catalogues_from_mongo_options.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/project_proj_key_data_catalogues_from_mongo_options.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/project_proj_key_data_catalogues_from_mongo_target.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/project_proj_key_data_catalogues_from_mongo_target.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/project_proj_key_data_catalogues_from_url_options.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/project_proj_key_data_catalogues_from_url_options.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/project_proj_key_dictionaries_from_mongo_target.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/project_proj_key_dictionaries_from_mongo_target.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/project_proj_key_kgc_dataflow_templates_debug_df_tpl_key_target_bag.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/project_proj_key_kgc_dataflow_templates_debug_df_tpl_key_target_bag.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/project_proj_key_kgc_dataflow_templates_df_tpl_key_actions_load_render.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/project_proj_key_kgc_dataflow_templates_df_tpl_key_actions_load_render.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/project_proj_key_kgc_dataflow_templates_df_tpl_key_actions_load_render_target_bag.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/project_proj_key_kgc_dataflow_templates_df_tpl_key_actions_load_render_target_bag.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/project_proj_key_kgc_dataflow_templates_df_tpl_key_actions_load_target.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/project_proj_key_kgc_dataflow_templates_df_tpl_key_actions_load_target.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/project_proj_key_kgc_dataflow_templates_variables.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/project_proj_key_kgc_dataflow_templates_variables.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/project_proj_key_kgc_raw_dataflow_templates_actions_run_data_flow.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/project_proj_key_kgc_raw_dataflow_templates_actions_run_data_flow.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/project_proj_key_kgc_raw_dataflow_templates_actions_run_data_flow_template.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/project_proj_key_kgc_raw_dataflow_templates_actions_run_data_flow_template.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/project_proj_key_model_configs_configurations.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/project_proj_key_model_configs_configurations.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/project_proj_key_packages_packages.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/project_proj_key_packages_packages.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/project_task.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/project_task.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/projects_flavours.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/projects_flavours.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/projects_flavours_flavours.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/projects_flavours_flavours.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/projects_flavours_quota.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/projects_flavours_quota.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/related_task.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/related_task.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/relationship_annotation_column.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/relationship_annotation_column.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/relationship_annotation_descriptor.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/relationship_annotation_descriptor.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/render_data_flow_template_options.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/render_data_flow_template_options.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/restore_knowledge_graph_backup_options.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/restore_knowledge_graph_backup_options.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/resume_knowledge_graph_options.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/resume_knowledge_graph_options.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/run_data_flow_template_options.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/run_data_flow_template_options.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/run_data_flow_template_options1.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/run_data_flow_template_options1.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/s3_coordinates.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/s3_coordinates.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/s3_coordinates_with_backup_key.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/s3_coordinates_with_backup_key.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/s3_coordinates_with_backup_key_presigned.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/s3_coordinates_with_backup_key_presigned.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/storage_summary_dc.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/storage_summary_dc.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/storage_summary_kg.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/storage_summary_kg.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/storage_summary_kg_categories_fraction.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/storage_summary_kg_categories_fraction.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/storage_summary_task.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/storage_summary_task.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/supported_annotator_annotations.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/supported_annotator_annotations.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/suspend_knowledge_graph_options.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/suspend_knowledge_graph_options.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/system_celery_tasks_failure_failures.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/system_celery_tasks_failure_failures.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/system_info.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/system_info.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/system_info_api.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/system_info_api.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/system_info_deployment.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/system_info_deployment.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/system_info_deployment_linked_ccs_api.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/system_info_deployment_linked_ccs_api.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/system_kgs_backend.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/system_kgs_backend.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/system_kgs_deployment.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/system_kgs_deployment.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/system_kgs_deployment_resources.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/system_kgs_deployment_resources.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/system_modules_configuration.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/system_modules_configuration.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/system_modules_tasks.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/system_modules_tasks.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/system_modules_tasks_tasks.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/system_modules_tasks_tasks.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/take_snapshot_settings.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/take_snapshot_settings.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/take_snapshot_settings_backend_aware.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/take_snapshot_settings_backend_aware.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/task.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/task.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/temporary_upload_file_result.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/temporary_upload_file_result.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/temporary_upload_file_result_download.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/temporary_upload_file_result_download.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/temporary_upload_file_result_download_private.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/temporary_upload_file_result_download_private.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/temporary_upload_file_result_metadata.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/temporary_upload_file_result_metadata.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/temporary_upload_file_result_metadata_private.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/temporary_upload_file_result_metadata_private.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/temporary_upload_file_result_upload.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/temporary_upload_file_result_upload.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/temporary_upload_file_result_upload_private.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/temporary_upload_file_result_upload_private.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/token_response.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/token_response.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/topology.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/topology.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/topology_edge.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/topology_edge.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/topology_node.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/topology_node.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/update_data_flow_options.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/update_data_flow_options.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/update_project_model_config_options.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/update_project_model_config_options.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/uploaded_file.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/uploaded_file.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/uploaded_file_result.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/uploaded_file_result.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/usage_stats.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/usage_stats.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/models/well_known_df_template_variable.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/models/well_known_df_template_variable.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/public/rest.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/public/rest.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/user/__init__.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/user/__init__.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/user/api/admin_api.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/user/api/admin_api.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/user/api/oidc_api.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/user/api/oidc_api.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/user/api/projects_api.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/user/api/projects_api.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/user/api/settings_api.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/user/api/settings_api.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/user/api/user_api.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/user/api/user_api.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/user/api/users_api.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/user/api/users_api.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/user/api_client.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/user/api_client.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/user/configuration.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/user/configuration.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/user/exceptions.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/user/exceptions.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/user/models/__init__.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/user/models/__init__.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/user/models/access_token.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/user/models/access_token.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/user/models/api_key.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/user/models/api_key.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/user/models/audit_record.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/user/models/audit_record.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/user/models/create_project_request_body.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/user/models/create_project_request_body.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/user/models/create_tokens_request_body.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/user/models/create_tokens_request_body.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/user/models/error_response.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/user/models/error_response.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/user/models/get_access_token_request_body.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/user/models/get_access_token_request_body.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/user/models/impersonate_user_token_request_body.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/user/models/impersonate_user_token_request_body.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/user/models/inline_response200.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/user/models/inline_response200.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/user/models/oidc_token_response.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/user/models/oidc_token_response.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/user/models/project.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/user/models/project.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/user/models/project_user_assignment.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/user/models/project_user_assignment.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/user/models/register_user_request_body.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/user/models/register_user_request_body.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/user/models/service_account.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/user/models/service_account.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/user/models/service_account_credentials.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/user/models/service_account_credentials.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/user/models/success_message.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/user/models/success_message.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/user/models/token_response.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/user/models/token_response.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/user/models/user_details.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/user/models/user_details.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/user/models/user_type.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/user/models/user_type.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/apis/user/rest.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/apis/user/rest.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/cli/cli_options.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/cli/cli_options.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/cli/data_indices_typer.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/cli/data_indices_typer.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/cli/elastic_data.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/cli/elastic_data.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/cli/kgs.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/cli/kgs.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/cli/main.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/cli/main.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/cli/projects.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/cli/projects.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/client/api.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/client/api.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/client/builders/wf_builder.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/client/builders/wf_builder.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/client/components/data_catalogs.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/client/components/data_catalogs.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/client/components/data_indices.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/client/components/data_indices.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,45 +1,42 @@
 from __future__ import annotations
 
 from dataclasses import dataclass
 from typing import TYPE_CHECKING, Any, Dict, List, Optional
 
+from pydantic import BaseModel
+
 from deepsearch.cps.apis import public as sw_client
 from deepsearch.cps.apis.public.models.token_response import TokenResponse
 from deepsearch.cps.client.components.api_object import ApiConnectedObject
-from deepsearch.cps.client.components.elastic import ElasticProjectDataCollectionSource
 
 if TYPE_CHECKING:
     from deepsearch.cps.client import CpsApi
 
 
 class CpsApiDataIndices:
     def __init__(self, api: CpsApi) -> None:
         self.api = api
         self.sw_api = sw_client.DataIndicesApi(self.api.client.swagger_client)
 
-    # define methods:
-    def list(self, proj_key: str):
-        try:
-            projects = self.sw_api.get_project_data_indices(proj_key=proj_key)
-            return projects
-        except ValueError as e:
-            print(f"Uh oh! {e}\nAborting!")
-            raise
+    def list(self, proj_key: str) -> List[DataIndex]:
+        response: list[
+            sw_client.ProjectDataIndexWithStatus
+        ] = self.sw_api.get_project_data_indices(proj_key=proj_key)
+
+        return [DataIndex.parse_obj(item.to_dict()) for item in response]
 
-    # def create(self, proj_key: str, data: Dict[str, str]):
-    #     return self.sw_api.create_project_data_index(proj_key=proj_key, data=data)
     def create(
         self,
         proj_key: str,
         name: str,
         desc: str = "",
         type: Optional[str] = None,
         schema_key: Optional[str] = None,
-    ):
+    ) -> DataIndex:
         """
         Method to create a new index.
 
         Input
         -----
         proj_key : string
             key of project in which index is created
@@ -69,20 +66,24 @@
 
         data = {
             "name": name,
             "description": desc,
             "schema_key": schema_key,
             "type": type,
         }
-        return self.sw_api.create_project_data_index(proj_key=proj_key, data=data)
+        response: sw_client.ProjectDataIndexWithStatus = (
+            self.sw_api.create_project_data_index(proj_key=proj_key, data=data)
+        )
+
+        return DataIndex.parse_obj(response.to_dict())
 
     def delete(
         self,
         coords: ElasticProjectDataCollectionSource,
-    ):
+    ) -> None:
         request_confirmation_token: TokenResponse = (
             self.sw_api.create_project_data_index_delete_token(
                 proj_key=coords.proj_key, index_key=coords.index_key
             )
         )
         confirmation_token = request_confirmation_token.token
         return self.sw_api.delete_project_data_index(
@@ -101,10 +102,30 @@
         """
         task_id = self.sw_api.ccs_convert_upload_file_project_data_index(
             proj_key=coords.proj_key, index_key=coords.index_key, body=body
         ).task_id
         return task_id
 
 
+class ElasticProjectDataCollectionSource(BaseModel):
+    proj_key: str
+    index_key: str
+
+    def to_resource(self) -> Dict[str, Any]:
+        return {"type": "elastic", "proj_key": self.proj_key, "index": self.index_key}
+
+
+class DataIndex(BaseModel):
+
+    source: ElasticProjectDataCollectionSource
+    name: str
+    description: str
+    documents: int
+    health: str
+    status: str
+    schema_key: str
+    type: str
+
+
 @dataclass
 class CpsApiDataIndex(ApiConnectedObject):
     project: str
```

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/client/components/documents.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/client/components/documents.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/client/components/elastic.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/client/components/elastic.py`

 * *Files 12% similar despite different names*

```diff
@@ -17,14 +17,17 @@
 
 from pydantic import BaseModel
 
 from deepsearch.cps.apis import public as sw_client
 from deepsearch.cps.apis.public.models.elastic_index_search_results import (
     ElasticIndexSearchResults,
 )
+from deepsearch.cps.client.components.data_indices import (
+    ElasticProjectDataCollectionSource,
+)
 
 if TYPE_CHECKING:
     from deepsearch.cps.client import CpsApi
 
 # Either a raw string, or the entire Elastic query DSL
 ElasticSearchQuery = Union[str, Dict[str, Any]]
 
@@ -161,22 +164,14 @@
         return {
             "type": "elastic",
             "elastic_id": self.elastic_id,
             "index": self.index_key,
         }
 
 
-class ElasticProjectDataCollectionSource(BaseModel):
-    proj_key: str
-    index_key: str
-
-    def to_resource(self) -> Dict[str, Any]:
-        return {"type": "elastic", "proj_key": self.proj_key, "index": self.index_key}
-
-
 class ElasticDataCollectionMetadata(BaseModel):
     description: str
     created: Union[datetime.datetime, str]
     domain: List[str]
     aliases: List[str]
     source: str
     type: str
```

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/client/components/knowledge_graphs.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/client/components/knowledge_graphs.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/client/components/projects.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/client/components/projects.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/client/components/queries.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/client/components/queries.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/client/components/tasks.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/client/components/tasks.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/client/queries/query.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/client/queries/query.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/client/queries/query_tasks/for_each.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/client/queries/query_tasks/for_each.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/client/queries/query_tasks/workflow.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/client/queries/query_tasks/workflow.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/client/queries/task.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/client/queries/task.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/data_indices/utils.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/data_indices/utils.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/ipython/__init__.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/ipython/__init__.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/ipython/kg_helpers.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/ipython/kg_helpers.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/ipython/kg_widgets.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/ipython/kg_widgets.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/kg/workflow/MultiLinkedList.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/kg/workflow/MultiLinkedList.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/kg/workflow/wf_functions.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/kg/workflow/wf_functions.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/kg/workflow/workflow.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/kg/workflow/workflow.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/cps/queries/__init__.py` & `deepsearch_toolkit-0.9.0/deepsearch/cps/queries/__init__.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/documents/cli/main.py` & `deepsearch_toolkit-0.9.0/deepsearch/documents/cli/main.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/documents/core/common_routines.py` & `deepsearch_toolkit-0.9.0/deepsearch/documents/core/common_routines.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/documents/core/convert.py` & `deepsearch_toolkit-0.9.0/deepsearch/documents/core/convert.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/documents/core/create_report.py` & `deepsearch_toolkit-0.9.0/deepsearch/documents/core/create_report.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/documents/core/input_process.py` & `deepsearch_toolkit-0.9.0/deepsearch/documents/core/input_process.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/documents/core/main.py` & `deepsearch_toolkit-0.9.0/deepsearch/documents/core/main.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/documents/core/models.py` & `deepsearch_toolkit-0.9.0/deepsearch/documents/core/models.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/documents/core/utils.py` & `deepsearch_toolkit-0.9.0/deepsearch/documents/core/utils.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/plugins/example_toy_cli_plugin.py` & `deepsearch_toolkit-0.9.0/deepsearch/plugins/example_toy_cli_plugin.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/deepsearch/query/cli/main.py` & `deepsearch_toolkit-0.9.0/deepsearch/query/cli/main.py`

 * *Files identical despite different names*

### Comparing `deepsearch_toolkit-0.8.0/pyproject.toml` & `deepsearch_toolkit-0.9.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "deepsearch-toolkit"
-version = "0.8.0"  # DO NOT EDIT, updated automatically
+version = "0.9.0"  # DO NOT EDIT, updated automatically
 description = "Interact with the Deep Search platform for new knowledge explorations and discoveries"
 authors = ["Michele Dolfi <dol@zurich.ibm.com>", "André Carvalho <andre.carvalho2@ibm.com>", "Lokesh Mishra <mis@zurich.ibm.com>", "Christoph Auer <cau@zurich.ibm.com>", "Kasper Dinkla <dkl@zurich.ibm.com>", "Cesar Berrospi Ramis <ceb@zurich.ibm.com>", "Panos Vagenas <pva@zurich.ibm.com>", "Peter Staar <taa@zurich.ibm.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://ds4sd.github.io/deepsearch-toolkit/"
 repository = "https://github.com/DS4SD/deepsearch-toolkit"
 documentation = "https://ds4sd.github.io/deepsearch-toolkit/"
```

### Comparing `deepsearch_toolkit-0.8.0/setup.py` & `deepsearch_toolkit-0.9.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -58,15 +58,15 @@
  'urllib3>=1.26.8,<2.0.0']
 
 entry_points = \
 {'console_scripts': ['deepsearch = deepsearch.cli:app']}
 
 setup_kwargs = {
     'name': 'deepsearch-toolkit',
-    'version': '0.8.0',
+    'version': '0.9.0',
     'description': 'Interact with the Deep Search platform for new knowledge explorations and discoveries',
     'long_description': '# DeepSearch Toolkit\n\n[![PyPI version](https://img.shields.io/pypi/v/deepsearch-toolkit)](https://pypi.org/project/deepsearch-toolkit/)\n[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/deepsearch-toolkit)](https://pypi.org/project/deepsearch-toolkit/)\n[![License MIT](https://img.shields.io/github/license/ds4sd/deepsearch-toolkit)](https://opensource.org/licenses/MIT)\n[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)\n[![Docs](https://img.shields.io/badge/website-live-brightgreen)](https://ds4sd.github.io/deepsearch-toolkit/)\n\n\n*Interact with the Deep Search platform for new knowledge explorations and discoveries*\n\n\nThe Deep Search Toolkit is a Python SDK allowing a user to interact with the Deep Search platform. The Toolkit provides easy-to-use functionalities for several common processes such as document conversion, graph creation and querying.\n\n\n[Learn about IBM Deep Search](https://ds4sd.github.io/)\n\n\n## Quick links\n\n- [Github repository](https://github.com/ds4sd/deepsearch-toolkit)\n- [Documentation](https://ds4sd.github.io/deepsearch-toolkit/)\n\n\n## Install\n\nUsing `poetry` in your project? Add the toolkit with:\n```console\n$ poetry add deepsearch-toolkit\n```\n\nNew to `poetry`? Visit https://python-poetry.org/ or our [CONTRIBUTING.md](CONTRIBUTING.md) section.\n\n\nUsing `pip`:\n```console\n$ pip install deepsearch-toolkit\n```\n\n### Requirements\n\nPython 3.8+\n\n\n## Start using the toolkit\n\n ```console\n// Login to Deep Search,\n// see https://ds4sd.github.io/deepsearch-toolkit/getting_started/#authentication\n$ deepsearch login\n...\n\n\n// Convert a document\n// for more details, see https://ds4sd.github.io/deepsearch-toolkit/guide/convert_doc/\n$ deepsearch documents convert -p 1234567890abcdefghijklmnopqrstvwyz123456 -u https://arxiv.org/pdf/2206.00785.pdf\nSubmitting input:     : 100%|██████████████████████████████| 1/1 [00:01<00:00,  1.52s/it]\nConverting input:     : 100%|██████████████████████████████| 1/1 [00:33<00:00, 33.80s/it]\nDownloading result:   : 100%|██████████████████████████████| 1/1 [00:01<00:00,  1.11s/it]\nTotal online documents             1\nSuccessfully converted documents   1\n```\n\n\n## Get help and support\n\nPlease feel free to connect with us using the [discussion section](https://github.com/DS4SD/deepsearch-toolkit/discussions).\n\n\n## Contributing\n\nPlease read [Contributing to Deep Search Toolkit](./CONTRIBUTING.md) for details.\n\n\n## References\n\nIf you use `Deep Search` in your projects, please consider citing the following:\n\n```bib\n@software{Deep Search Toolkit,\nauthor = {Deep Search Team},\nmonth = {6},\ntitle = {{Deep Search Toolkit}},\nurl = {https://github.com/DS4SD/deepsearch-toolkit},\nversion = {main},\nyear = {2022}\n}\n```\n\n## License\n\nThe `Deep Search Toolkit` codebase is under MIT license.\nFor individual model usage, please refer to the model licenses found in the original packages.\n',
     'author': 'Michele Dolfi',
     'author_email': 'dol@zurich.ibm.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://ds4sd.github.io/deepsearch-toolkit/',
```

### Comparing `deepsearch_toolkit-0.8.0/PKG-INFO` & `deepsearch_toolkit-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deepsearch-toolkit
-Version: 0.8.0
+Version: 0.9.0
 Summary: Interact with the Deep Search platform for new knowledge explorations and discoveries
 Home-page: https://ds4sd.github.io/deepsearch-toolkit/
 License: MIT
 Keywords: deepsearch,convert,knowledge graph,discovery,nlp
 Author: Michele Dolfi
 Author-email: dol@zurich.ibm.com
 Requires-Python: >=3.8,<4.0
```

