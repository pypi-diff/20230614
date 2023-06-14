# Comparing `tmp/ptal_api-0.11.6.1.tar.gz` & `tmp/ptal_api-0.12.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ptal_api-0.11.6.1.tar", max compression
+gzip compressed data, was "ptal_api-0.12.0.tar", max compression
```

## Comparing `ptal_api-0.11.6.1.tar` & `ptal_api-0.12.0.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0      627 2023-04-24 11:23:04.939750 ptal_api-0.11.6.1/README.md
--rw-r--r--   0        0        0        0 2023-05-25 16:49:19.030532 ptal_api-0.11.6.1/ptal_api/__init__.py
--rw-r--r--   0        0        0   100253 2023-05-25 16:45:27.776257 ptal_api-0.11.6.1/ptal_api/adapter.py
--rw-r--r--   0        0        0      184 2023-05-16 13:32:51.877997 ptal_api-0.11.6.1/ptal_api/core/kb_sync/kb_iterator_config.py
--rw-r--r--   0        0        0      160 2023-04-24 11:23:04.943750 ptal_api-0.11.6.1/ptal_api/core/kb_sync/object_time_interval.py
--rw-r--r--   0        0        0      435 2023-04-24 11:23:04.943750 ptal_api-0.11.6.1/ptal_api/core/type_mapper/app_settings/logging.conf
--rw-r--r--   0        0        0      737 2023-05-02 10:24:35.487480 ptal_api-0.11.6.1/ptal_api/core/type_mapper/common/common.py
--rw-r--r--   0        0        0    14955 2023-05-25 14:41:26.834648 ptal_api-0.11.6.1/ptal_api/core/type_mapper/data_model/base_data_model.py
--rw-r--r--   0        0        0      904 2023-05-02 10:24:35.491480 ptal_api-0.11.6.1/ptal_api/core/type_mapper/data_model/config_data_model.py
--rw-r--r--   0        0        0     3255 2023-05-02 10:24:35.491480 ptal_api-0.11.6.1/ptal_api/core/type_mapper/data_model/custom_data_model.py
--rw-r--r--   0        0        0     3501 2023-04-24 11:23:04.943750 ptal_api-0.11.6.1/ptal_api/core/type_mapper/model_parameters/name_code_mapping.yml
--rw-r--r--   0        0        0     2194 2023-05-02 10:24:35.491480 ptal_api-0.11.6.1/ptal_api/core/type_mapper/modules/custom_data_handler.py
--rw-r--r--   0        0        0     1464 2023-05-02 10:24:35.491480 ptal_api-0.11.6.1/ptal_api/core/type_mapper/modules/file_generator.py
--rw-r--r--   0        0        0     4556 2023-05-02 10:24:35.491480 ptal_api-0.11.6.1/ptal_api/core/type_mapper/modules/object_name_transformer.py
--rw-r--r--   0        0        0    23314 2023-05-02 10:24:35.491480 ptal_api-0.11.6.1/ptal_api/core/type_mapper/modules/type_mapping_generator.py
--rw-r--r--   0        0        0     1800 2023-05-02 10:24:35.491480 ptal_api-0.11.6.1/ptal_api/core/type_mapper/modules/type_mapping_loader/type_mapping_loader.py
--rw-r--r--   0        0        0      418 2023-04-24 11:23:04.943750 ptal_api-0.11.6.1/ptal_api/core/type_mapper/modules/type_mapping_loader/type_mapping_loader_interface.py
--rw-r--r--   0        0        0      192 2023-04-24 11:23:04.943750 ptal_api-0.11.6.1/ptal_api/core/values/date_dataclass.py
--rw-r--r--   0        0        0     3279 2023-05-25 16:31:12.226717 ptal_api-0.11.6.1/ptal_api/core/values/value_mapping.py
--rw-r--r--   0        0        0        0 2023-05-25 16:49:19.030532 ptal_api-0.11.6.1/ptal_api/providers/__init__.py
--rw-r--r--   0        0        0     4668 2023-05-02 10:24:35.491480 ptal_api-0.11.6.1/ptal_api/providers/gql_providers.py
--rw-r--r--   0        0        0     1186 2023-05-02 11:37:55.718860 ptal_api-0.11.6.1/ptal_api/schema/README.md
--rw-r--r--   0        0        0        0 2023-05-25 16:49:19.030532 ptal_api-0.11.6.1/ptal_api/schema/__init__.py
--rw-r--r--   0        0        0   289804 2023-05-25 16:31:12.230717 ptal_api-0.11.6.1/ptal_api/schema/api_schema.py
--rw-r--r--   0        0        0    93413 2023-05-25 16:31:12.230717 ptal_api-0.11.6.1/ptal_api/schema/crawlers_api_schema.py
--rw-r--r--   0        0        0    74033 2023-05-02 11:37:55.722860 ptal_api-0.11.6.1/ptal_api/schema/tcontroller_api_schema.py
--rw-r--r--   0        0        0   136845 2023-05-25 16:31:12.234717 ptal_api-0.11.6.1/ptal_api/schema/utils_api_schema.py
--rw-r--r--   0        0        0     3662 2023-05-02 10:24:35.491480 ptal_api-0.11.6.1/ptal_api/scripts/type_mapper.py
--rw-r--r--   0        0        0        0 2023-05-25 16:49:19.030532 ptal_api-0.11.6.1/ptal_api/tdm_builder/__init__.py
--rw-r--r--   0        0        0     1211 2023-05-02 10:24:35.491480 ptal_api-0.11.6.1/ptal_api/tdm_builder/tdm_builder.py
--rw-r--r--   0        0        0     1873 2023-05-25 16:45:27.776257 ptal_api-0.11.6.1/pyproject.toml
--rw-r--r--   0        0        0     1491 1970-01-01 00:00:00.000000 ptal_api-0.11.6.1/PKG-INFO
+-rw-r--r--   0        0        0      627 2023-05-29 10:30:59.749331 ptal_api-0.12.0/README.md
+-rw-r--r--   0        0        0        0 2023-05-29 10:38:17.402116 ptal_api-0.12.0/ptal_api/__init__.py
+-rw-r--r--   0        0        0   100253 2023-05-29 10:30:59.749331 ptal_api-0.12.0/ptal_api/adapter.py
+-rw-r--r--   0        0        0      184 2023-05-29 10:30:59.749331 ptal_api-0.12.0/ptal_api/core/kb_sync/kb_iterator_config.py
+-rw-r--r--   0        0        0      160 2023-05-29 10:30:59.749331 ptal_api-0.12.0/ptal_api/core/kb_sync/object_time_interval.py
+-rw-r--r--   0        0        0      435 2023-05-29 10:30:59.749331 ptal_api-0.12.0/ptal_api/core/type_mapper/app_settings/logging.conf
+-rw-r--r--   0        0        0      737 2023-05-29 10:30:59.749331 ptal_api-0.12.0/ptal_api/core/type_mapper/common/common.py
+-rw-r--r--   0        0        0    14955 2023-05-29 10:30:59.749331 ptal_api-0.12.0/ptal_api/core/type_mapper/data_model/base_data_model.py
+-rw-r--r--   0        0        0      904 2023-05-29 10:30:59.749331 ptal_api-0.12.0/ptal_api/core/type_mapper/data_model/config_data_model.py
+-rw-r--r--   0        0        0     3255 2023-05-29 10:30:59.749331 ptal_api-0.12.0/ptal_api/core/type_mapper/data_model/custom_data_model.py
+-rw-r--r--   0        0        0     3501 2023-05-29 10:30:59.749331 ptal_api-0.12.0/ptal_api/core/type_mapper/model_parameters/name_code_mapping.yml
+-rw-r--r--   0        0        0     2194 2023-05-29 10:30:59.749331 ptal_api-0.12.0/ptal_api/core/type_mapper/modules/custom_data_handler.py
+-rw-r--r--   0        0        0     1464 2023-05-29 10:30:59.749331 ptal_api-0.12.0/ptal_api/core/type_mapper/modules/file_generator.py
+-rw-r--r--   0        0        0     4556 2023-05-29 10:30:59.753331 ptal_api-0.12.0/ptal_api/core/type_mapper/modules/object_name_transformer.py
+-rw-r--r--   0        0        0    23314 2023-05-29 10:30:59.753331 ptal_api-0.12.0/ptal_api/core/type_mapper/modules/type_mapping_generator.py
+-rw-r--r--   0        0        0     1800 2023-05-29 10:30:59.753331 ptal_api-0.12.0/ptal_api/core/type_mapper/modules/type_mapping_loader/type_mapping_loader.py
+-rw-r--r--   0        0        0      418 2023-05-29 10:30:59.753331 ptal_api-0.12.0/ptal_api/core/type_mapper/modules/type_mapping_loader/type_mapping_loader_interface.py
+-rw-r--r--   0        0        0      192 2023-05-29 10:30:59.753331 ptal_api-0.12.0/ptal_api/core/values/date_dataclass.py
+-rw-r--r--   0        0        0     3279 2023-05-29 10:30:59.753331 ptal_api-0.12.0/ptal_api/core/values/value_mapping.py
+-rw-r--r--   0        0        0        0 2023-05-29 10:38:17.402116 ptal_api-0.12.0/ptal_api/providers/__init__.py
+-rw-r--r--   0        0        0     4668 2023-05-29 10:30:59.753331 ptal_api-0.12.0/ptal_api/providers/gql_providers.py
+-rw-r--r--   0        0        0     1186 2023-05-29 10:30:59.753331 ptal_api-0.12.0/ptal_api/schema/README.md
+-rw-r--r--   0        0        0        0 2023-05-29 10:38:17.402116 ptal_api-0.12.0/ptal_api/schema/__init__.py
+-rw-r--r--   0        0        0   290619 2023-05-29 10:30:59.753331 ptal_api-0.12.0/ptal_api/schema/api_schema.py
+-rw-r--r--   0        0        0    95040 2023-05-29 10:30:59.753331 ptal_api-0.12.0/ptal_api/schema/crawlers_api_schema.py
+-rw-r--r--   0        0        0    74033 2023-05-29 10:30:59.753331 ptal_api-0.12.0/ptal_api/schema/tcontroller_api_schema.py
+-rw-r--r--   0        0        0   137251 2023-05-29 10:30:59.753331 ptal_api-0.12.0/ptal_api/schema/utils_api_schema.py
+-rw-r--r--   0        0        0     3662 2023-05-29 10:30:59.753331 ptal_api-0.12.0/ptal_api/scripts/type_mapper.py
+-rw-r--r--   0        0        0        0 2023-05-29 10:38:17.402116 ptal_api-0.12.0/ptal_api/tdm_builder/__init__.py
+-rw-r--r--   0        0        0     1211 2023-05-29 10:30:59.753331 ptal_api-0.12.0/ptal_api/tdm_builder/tdm_builder.py
+-rw-r--r--   0        0        0     1871 2023-05-29 10:30:59.753331 ptal_api-0.12.0/pyproject.toml
+-rw-r--r--   0        0        0     1489 1970-01-01 00:00:00.000000 ptal_api-0.12.0/PKG-INFO
```

### Comparing `ptal_api-0.11.6.1/README.md` & `ptal_api-0.12.0/README.md`

 * *Files identical despite different names*

### Comparing `ptal_api-0.11.6.1/ptal_api/adapter.py` & `ptal_api-0.12.0/ptal_api/adapter.py`

 * *Files identical despite different names*

### Comparing `ptal_api-0.11.6.1/ptal_api/core/type_mapper/common/common.py` & `ptal_api-0.12.0/ptal_api/core/type_mapper/common/common.py`

 * *Files identical despite different names*

### Comparing `ptal_api-0.11.6.1/ptal_api/core/type_mapper/data_model/base_data_model.py` & `ptal_api-0.12.0/ptal_api/core/type_mapper/data_model/base_data_model.py`

 * *Files identical despite different names*

### Comparing `ptal_api-0.11.6.1/ptal_api/core/type_mapper/data_model/config_data_model.py` & `ptal_api-0.12.0/ptal_api/core/type_mapper/data_model/config_data_model.py`

 * *Files identical despite different names*

### Comparing `ptal_api-0.11.6.1/ptal_api/core/type_mapper/data_model/custom_data_model.py` & `ptal_api-0.12.0/ptal_api/core/type_mapper/data_model/custom_data_model.py`

 * *Files identical despite different names*

### Comparing `ptal_api-0.11.6.1/ptal_api/core/type_mapper/model_parameters/name_code_mapping.yml` & `ptal_api-0.12.0/ptal_api/core/type_mapper/model_parameters/name_code_mapping.yml`

 * *Files identical despite different names*

### Comparing `ptal_api-0.11.6.1/ptal_api/core/type_mapper/modules/custom_data_handler.py` & `ptal_api-0.12.0/ptal_api/core/type_mapper/modules/custom_data_handler.py`

 * *Files identical despite different names*

### Comparing `ptal_api-0.11.6.1/ptal_api/core/type_mapper/modules/file_generator.py` & `ptal_api-0.12.0/ptal_api/core/type_mapper/modules/file_generator.py`

 * *Files identical despite different names*

### Comparing `ptal_api-0.11.6.1/ptal_api/core/type_mapper/modules/object_name_transformer.py` & `ptal_api-0.12.0/ptal_api/core/type_mapper/modules/object_name_transformer.py`

 * *Files identical despite different names*

### Comparing `ptal_api-0.11.6.1/ptal_api/core/type_mapper/modules/type_mapping_generator.py` & `ptal_api-0.12.0/ptal_api/core/type_mapper/modules/type_mapping_generator.py`

 * *Files identical despite different names*

### Comparing `ptal_api-0.11.6.1/ptal_api/core/type_mapper/modules/type_mapping_loader/type_mapping_loader.py` & `ptal_api-0.12.0/ptal_api/core/type_mapper/modules/type_mapping_loader/type_mapping_loader.py`

 * *Files identical despite different names*

### Comparing `ptal_api-0.11.6.1/ptal_api/core/values/value_mapping.py` & `ptal_api-0.12.0/ptal_api/core/values/value_mapping.py`

 * *Files identical despite different names*

### Comparing `ptal_api-0.11.6.1/ptal_api/providers/gql_providers.py` & `ptal_api-0.12.0/ptal_api/providers/gql_providers.py`

 * *Files identical despite different names*

### Comparing `ptal_api-0.11.6.1/ptal_api/schema/README.md` & `ptal_api-0.12.0/ptal_api/schema/README.md`

 * *Files identical despite different names*

### Comparing `ptal_api-0.11.6.1/ptal_api/schema/api_schema.py` & `ptal_api-0.12.0/ptal_api/schema/api_schema.py`

 * *Files 0% similar despite different names*

```diff
@@ -189,15 +189,15 @@
 class DocumentViewColumnType(sgqlc.types.Enum):
     __schema__ = api_schema
     __choices__ = ('accessLevel', 'account', 'creator', 'externalUrl', 'lastUpdater', 'platform', 'publicationAuthor', 'publicationDate', 'systemRegistrationDate', 'systemUpdateDate', 'trustLevel')
 
 
 class DocumentViewMetricType(sgqlc.types.Enum):
     __schema__ = api_schema
-    __choices__ = ('countChildDocs', 'countConcepts', 'countDisambiguatedEntities', 'countEntities', 'countEvents', 'countLinks', 'countNamedEntities', 'countObjects', 'countPropertyCandidates', 'countResearchMaps', 'countTasks')
+    __choices__ = ('countChildDocs', 'countConcepts', 'countDisambiguatedEntities', 'countEntities', 'countEvents', 'countLinks', 'countNamedEntities', 'countObjects', 'countPropertyCandidates', 'countResearchMaps', 'countStoryDocs', 'countTasks')
 
 
 class ElementType(sgqlc.types.Enum):
     __schema__ = api_schema
     __choices__ = ('blackList', 'whiteList')
 
 
@@ -1986,14 +1986,21 @@
 class ConceptCandidateFactMention(sgqlc.types.Type):
     __schema__ = api_schema
     __field_names__ = ('concept', 'mention')
     concept = sgqlc.types.Field(sgqlc.types.non_null('ConceptCandidateFact'), graphql_name='concept')
     mention = sgqlc.types.Field(sgqlc.types.non_null('Mention'), graphql_name='mention')
 
 
+class ConceptFacet(sgqlc.types.Type):
+    __schema__ = api_schema
+    __field_names__ = ('count', 'value')
+    count = sgqlc.types.Field(sgqlc.types.non_null(Long), graphql_name='count')
+    value = sgqlc.types.Field(sgqlc.types.non_null('Concept'), graphql_name='value')
+
+
 class ConceptFactLink(sgqlc.types.Type):
     __schema__ = api_schema
     __field_names__ = ('concept_id', 'concept_fact_id', 'status', 'is_implicit', 'concept', 'concept_fact')
     concept_id = sgqlc.types.Field(sgqlc.types.non_null(ID), graphql_name='conceptId')
     concept_fact_id = sgqlc.types.Field(sgqlc.types.non_null(ID), graphql_name='conceptFactId')
     status = sgqlc.types.Field(FactStatus, graphql_name='status')
     is_implicit = sgqlc.types.Field(sgqlc.types.non_null(Boolean), graphql_name='isImplicit')
@@ -2292,16 +2299,18 @@
     document = sgqlc.types.Field(sgqlc.types.non_null('Document'), graphql_name='document')
     is_from_favorites = sgqlc.types.Field(sgqlc.types.non_null(Boolean), graphql_name='isFromFavorites')
     is_from_deleted = sgqlc.types.Field(sgqlc.types.non_null(Boolean), graphql_name='isFromDeleted')
 
 
 class DocumentFromDocumentFeedPagination(sgqlc.types.Type):
     __schema__ = api_schema
-    __field_names__ = ('list_document', 'total', 'show_total')
+    __field_names__ = ('list_document', 'list_named_entity_count_facet', 'list_concept_count_facet', 'total', 'show_total')
     list_document = sgqlc.types.Field(sgqlc.types.non_null(sgqlc.types.list_of(sgqlc.types.non_null(DocumentFromDocumentFeed))), graphql_name='listDocument')
+    list_named_entity_count_facet = sgqlc.types.Field(sgqlc.types.non_null(sgqlc.types.list_of(sgqlc.types.non_null('Facet'))), graphql_name='listNamedEntityCountFacet')
+    list_concept_count_facet = sgqlc.types.Field(sgqlc.types.non_null(sgqlc.types.list_of(sgqlc.types.non_null(ConceptFacet))), graphql_name='listConceptCountFacet')
     total = sgqlc.types.Field(sgqlc.types.non_null(Int), graphql_name='total')
     show_total = sgqlc.types.Field(sgqlc.types.non_null(Int), graphql_name='showTotal')
 
 
 class DocumentLink(sgqlc.types.Type):
     __schema__ = api_schema
     __field_names__ = ('parent_id', 'child_id')
@@ -2599,24 +2608,25 @@
     __field_names__ = ('total', 'list_merged_concept')
     total = sgqlc.types.Field(sgqlc.types.non_null(Long), graphql_name='total')
     list_merged_concept = sgqlc.types.Field(sgqlc.types.non_null(sgqlc.types.list_of(sgqlc.types.non_null(MergedConcept))), graphql_name='listMergedConcept')
 
 
 class Metrics(sgqlc.types.Type):
     __schema__ = api_schema
-    __field_names__ = ('count_objects', 'count_events', 'count_named_entities', 'count_disambiguated_entities', 'count_property_candidates', 'count_links', 'count_research_maps', 'count_child_docs', 'count_tasks', 'count_concepts', 'count_entities')
+    __field_names__ = ('count_objects', 'count_events', 'count_named_entities', 'count_disambiguated_entities', 'count_property_candidates', 'count_links', 'count_research_maps', 'count_child_docs', 'count_tasks', 'count_story_docs', 'count_concepts', 'count_entities')
     count_objects = sgqlc.types.Field(sgqlc.types.non_null(Int), graphql_name='countObjects')
     count_events = sgqlc.types.Field(sgqlc.types.non_null(Int), graphql_name='countEvents')
     count_named_entities = sgqlc.types.Field(sgqlc.types.non_null(Int), graphql_name='countNamedEntities')
     count_disambiguated_entities = sgqlc.types.Field(sgqlc.types.non_null(Int), graphql_name='countDisambiguatedEntities')
     count_property_candidates = sgqlc.types.Field(sgqlc.types.non_null(Int), graphql_name='countPropertyCandidates')
     count_links = sgqlc.types.Field(sgqlc.types.non_null(Int), graphql_name='countLinks')
     count_research_maps = sgqlc.types.Field(sgqlc.types.non_null(Int), graphql_name='countResearchMaps')
     count_child_docs = sgqlc.types.Field(sgqlc.types.non_null(Int), graphql_name='countChildDocs')
     count_tasks = sgqlc.types.Field(sgqlc.types.non_null(Int), graphql_name='countTasks')
+    count_story_docs = sgqlc.types.Field(sgqlc.types.non_null(Int), graphql_name='countStoryDocs')
     count_concepts = sgqlc.types.Field(sgqlc.types.non_null(Int), graphql_name='countConcepts')
     count_entities = sgqlc.types.Field(sgqlc.types.non_null(Int), graphql_name='countEntities')
 
 
 class Mutation(sgqlc.types.Type):
     __schema__ = api_schema
     __field_names__ = ('add_concept', 'add_concept_link', 'reverse_concept_link', 'update_concept_link', 'add_concept_property', 'add_concept_link_property', 'add_concept_fact', 'delete_concept_fact', 'add_concept_link_property_fact', 'delete_concept_link_property_fact', 'add_concept_property_fact', 'delete_concept_property_fact', 'add_concept_link_fact', 'delete_concept_link_fact', 'update_concept', 'update_concept_avatar', 'update_concept_property', 'delete_concept_property', 'delete_concept_link', 'delete_concept', 'delete_concept_link_property', 'merge_concepts', 'unmerge_concepts', 'delete_fact', 'normalize_value', 'update_concept_subscriptions', 'add_concept_type', 'add_composite_concept_type', 'add_composite_concept_type_template', 'add_composite_concept_type_widget_type', 'set_concept_type_default_view', 'add_concept_property_type', 'add_concept_link_property_type', 'add_concept_link_type', 'add_concept_property_value_type', 'add_concept_type_view', 'update_concept_type', 'update_composite_concept_type', 'update_composite_concept_type_template_filename', 'update_composite_concept_type_widget_type', 'update_composite_concept_type_widget_types_order', 'update_concept_property_type', 'update_concept_main_property_type_order', 'update_concept_link_property_type', 'update_concept_link_type', 'update_concept_property_value_type', 'update_concept_type_view', 'delete_concept_type_avatar', 'delete_concept_type', 'delete_composite_concept_type', 'delete_composite_concept_type_widget_type', 'delete_concept_property_type', 'delete_concept_link_property_type', 'delete_concept_link_type', 'delete_concept_property_value_type', 'delete_concept_type_view', 'delete_bulk', 'move_bulk', 'update_type_search_element', 'add_composite_property_value_template', 'update_composite_property_value_template', 'delete_composite_property_value_template', 'add_issue', 'delete_issue', 'add_concept_to_issue', 'add_document_to_issue', 'add_issue_to_issue', 'delete_document_from_issue', 'delete_concept_from_issue', 'delete_issue_from_issue', 'update_issue', 'update_issue_massive', 'add_comment_to_issue', 'update_issue_comment', 'delete_issue_comment', 'update_document', 'update_document_avatar', 'remove_candidate_fact_from_document', 'remove_all_kbfacts_from_document', 'delete_documents', 'add_document_double', 'update_document_node', 'update_document_subscriptions', 'mark_document_as_read', 'mark_document_as_unread', 'delete_research_map', 'bulk_delete_research_map', 'add_research_map', 'add_research_map_from_files', 'update_research_map', 'add_content_on_research_map', 'delete_content_from_research_map', 'batch_move_nodes_on_map', 'batch_update_group_on_map', 'add_top_neighbors_on_map', 'add_concept_fact_neighbors_on_map', 'set_research_map_active', 'find_shortest_path_on_map', 'find_shortest_implicit_path_on_map', 'add_group', 'update_group', 'delete_group', 'create_redmine_issue', 'update_redmine_issue', 'unlink_issues', 'add_access_level', 'update_access_level', 'delete_access_level', 'add_template_docx', 'update_markers_bulk', 'update_document_bulk', 'add_platform', 'update_platform', 'delete_platform', 'add_account', 'update_account', 'delete_account', 'add_document_feed', 'update_document_feed', 'add_document_to_document_feed_favorites', 'delete_document_from_document_feed_favorites', 'delete_document_from_document_feed', 'restore_document_to_document_feed', 'delete_document_feed', 'update_concept_registry_view', 'update_document_registry_view', 'update_document_card_view', 'add_chart', 'update_chart', 'delete_chart')
@@ -3753,15 +3763,15 @@
 class StoryPagination(sgqlc.types.Type):
     __schema__ = api_schema
     __field_names__ = ('list_story', 'total', 'show_total', 'list_named_entity_count_facet', 'list_concept_count_facet', 'list_account_count_facet', 'list_platform_count_facet', 'list_markers', 'sources', 'new_documents_today')
     list_story = sgqlc.types.Field(sgqlc.types.non_null(sgqlc.types.list_of(sgqlc.types.non_null(Story))), graphql_name='listStory')
     total = sgqlc.types.Field(sgqlc.types.non_null(Int), graphql_name='total')
     show_total = sgqlc.types.Field(sgqlc.types.non_null(Int), graphql_name='showTotal')
     list_named_entity_count_facet = sgqlc.types.Field(sgqlc.types.non_null(sgqlc.types.list_of(sgqlc.types.non_null(Facet))), graphql_name='listNamedEntityCountFacet')
-    list_concept_count_facet = sgqlc.types.Field(sgqlc.types.non_null(sgqlc.types.list_of(sgqlc.types.non_null(Facet))), graphql_name='listConceptCountFacet')
+    list_concept_count_facet = sgqlc.types.Field(sgqlc.types.non_null(sgqlc.types.list_of(sgqlc.types.non_null(ConceptFacet))), graphql_name='listConceptCountFacet')
     list_account_count_facet = sgqlc.types.Field(sgqlc.types.non_null(sgqlc.types.list_of(sgqlc.types.non_null(AccountFacet))), graphql_name='listAccountCountFacet')
     list_platform_count_facet = sgqlc.types.Field(sgqlc.types.non_null(sgqlc.types.list_of(sgqlc.types.non_null(PlatformFacet))), graphql_name='listPlatformCountFacet')
     list_markers = sgqlc.types.Field(sgqlc.types.non_null(sgqlc.types.list_of(sgqlc.types.non_null(Facet))), graphql_name='listMarkers')
     sources = sgqlc.types.Field(sgqlc.types.non_null(Int), graphql_name='sources')
     new_documents_today = sgqlc.types.Field(sgqlc.types.non_null(Int), graphql_name='newDocumentsToday')
```

### Comparing `ptal_api-0.11.6.1/ptal_api/schema/crawlers_api_schema.py` & `ptal_api-0.12.0/ptal_api/schema/crawlers_api_schema.py`

 * *Files 0% similar despite different names*

```diff
@@ -115,14 +115,19 @@
 
 
 class MetricSorting(sgqlc.types.Enum):
     __schema__ = crawlers_api_schema
     __choices__ = ('timestamp',)
 
 
+class MonitoringStatus(sgqlc.types.Enum):
+    __schema__ = crawlers_api_schema
+    __choices__ = ('Critical', 'Ok', 'Pending', 'SameItemsJob', 'SameItemsPeriodic', 'ZeroItemsZeroDuplicates')
+
+
 class PeriodicJobSorting(sgqlc.types.Enum):
     __schema__ = crawlers_api_schema
     __choices__ = ('crawlerId', 'crawlerName', 'creator', 'id', 'lastUpdater', 'name', 'nextScheduleTime', 'priority', 'projectId', 'projectName', 'status', 'systemRegistrationDate', 'systemUpdateDate')
 
 
 class PeriodicJobStatus(sgqlc.types.Enum):
     __schema__ = crawlers_api_schema
@@ -675,23 +680,24 @@
     __field_names__ = ('total', 'list_job')
     total = sgqlc.types.Field(sgqlc.types.non_null(Int), graphql_name='total')
     list_job = sgqlc.types.Field(sgqlc.types.non_null('Jobs'), graphql_name='listJob')
 
 
 class JobStats(sgqlc.types.Type):
     __schema__ = crawlers_api_schema
-    __field_names__ = ('jobs_count', 'total_time', 'items_scraped_count', 'requests_count', 'errors_count', 'duplicated_request_count', 'jobs_with_errors_logs_count', 'jobs_with_critical_logs_count')
+    __field_names__ = ('jobs_count', 'total_time', 'items_scraped_count', 'requests_count', 'errors_count', 'duplicated_request_count', 'jobs_with_errors_logs_count', 'jobs_with_critical_logs_count', 'item_domains')
     jobs_count = sgqlc.types.Field(Int, graphql_name='jobsCount')
     total_time = sgqlc.types.Field(Long, graphql_name='totalTime')
     items_scraped_count = sgqlc.types.Field(Long, graphql_name='itemsScrapedCount')
     requests_count = sgqlc.types.Field(Long, graphql_name='requestsCount')
     errors_count = sgqlc.types.Field(Int, graphql_name='errorsCount')
     duplicated_request_count = sgqlc.types.Field(Int, graphql_name='duplicatedRequestCount')
     jobs_with_errors_logs_count = sgqlc.types.Field(Int, graphql_name='jobsWithErrorsLogsCount')
     jobs_with_critical_logs_count = sgqlc.types.Field(Int, graphql_name='jobsWithCriticalLogsCount')
+    item_domains = sgqlc.types.Field(sgqlc.types.non_null(sgqlc.types.list_of(sgqlc.types.non_null('Platform'))), graphql_name='itemDomains')
 
 
 class Jobs(sgqlc.types.Type):
     __schema__ = crawlers_api_schema
     __field_names__ = ('pending', 'running', 'finished')
     pending = sgqlc.types.Field(sgqlc.types.non_null(JobList), graphql_name='pending')
     running = sgqlc.types.Field(sgqlc.types.non_null(JobList), graphql_name='running')
@@ -736,15 +742,15 @@
     __field_names__ = ('total', 'list_metric')
     total = sgqlc.types.Field(sgqlc.types.non_null(Long), graphql_name='total')
     list_metric = sgqlc.types.Field(sgqlc.types.non_null(sgqlc.types.list_of(sgqlc.types.non_null(Metric))), graphql_name='listMetric')
 
 
 class Mutation(sgqlc.types.Type):
     __schema__ = crawlers_api_schema
-    __field_names__ = ('update_crawler', 'update_crawler_settings_arguments', 'delete_crawler_versions', 'delete_crawlers', 'update_site_map_crawler_body', 'add_crawl_state', 'update_crawl_state', 'delete_crawl_state', 'add_credential', 'update_credential', 'delete_credential', 'single_upload', 'add_job', 'delete_job', 'cancel_job', 'suspend_job', 'resume_job', 'download_pending_jobs', 'schedule_uploaded_jobs', 'add_periodic_job', 'run_periodic_jobs', 'update_enable_jobs_scheduling', 'update_disable_jobs_scheduling', 'delete_periodic_job', 'update_periodic_job', 'update_periodic_job_settings_and_arguments', 'delete_project', 'delete_project_versions', 'add_project', 'update_project', 'update_project_settings_and_arguments', 'add_information_source_loader', 'delete_information_source_loader', 'add_recovery_job', 'cancel_recovery_job')
+    __field_names__ = ('update_crawler', 'update_crawler_settings_arguments', 'delete_crawler_versions', 'delete_crawlers', 'update_site_map_crawler_body', 'add_crawl_state', 'update_crawl_state', 'delete_crawl_state', 'add_credential', 'update_credential', 'delete_credential', 'single_upload', 'add_job', 'delete_job', 'cancel_job', 'suspend_job', 'resume_job', 'download_pending_jobs', 'schedule_uploaded_jobs', 'add_periodic_job', 'run_periodic_jobs', 'update_enable_jobs_scheduling', 'update_disable_jobs_scheduling', 'delete_periodic_job', 'update_periodic_job', 'update_periodic_job_settings_and_arguments', 'import_periodic_jobs', 'delete_project', 'delete_project_versions', 'add_project', 'update_project', 'update_project_settings_and_arguments', 'add_information_source_loader', 'delete_information_source_loader', 'add_recovery_job', 'cancel_recovery_job')
     update_crawler = sgqlc.types.Field(sgqlc.types.non_null('Crawler'), graphql_name='updateCrawler', args=sgqlc.types.ArgDict((
         ('crawler_update_input', sgqlc.types.Arg(sgqlc.types.non_null(CrawlerUpdateInput), graphql_name='crawlerUpdateInput', default=None)),
         ('crawler_id', sgqlc.types.Arg(sgqlc.types.non_null(ID), graphql_name='crawlerId', default=None)),
         ('project_id', sgqlc.types.Arg(sgqlc.types.non_null(ID), graphql_name='projectId', default=None)),
 ))
     )
     update_crawler_settings_arguments = sgqlc.types.Field(sgqlc.types.non_null('Crawler'), graphql_name='updateCrawlerSettingsArguments', args=sgqlc.types.ArgDict((
@@ -851,14 +857,18 @@
     )
     update_periodic_job_settings_and_arguments = sgqlc.types.Field(sgqlc.types.non_null(ID), graphql_name='updatePeriodicJobSettingsAndArguments', args=sgqlc.types.ArgDict((
         ('id', sgqlc.types.Arg(sgqlc.types.non_null(ID), graphql_name='id', default=None)),
         ('settings', sgqlc.types.Arg(sgqlc.types.non_null(sgqlc.types.list_of(sgqlc.types.non_null(KeyValueInputType))), graphql_name='settings', default=None)),
         ('args', sgqlc.types.Arg(sgqlc.types.non_null(sgqlc.types.list_of(sgqlc.types.non_null(KeyValueInputType))), graphql_name='args', default=None)),
 ))
     )
+    import_periodic_jobs = sgqlc.types.Field(sgqlc.types.non_null(sgqlc.types.list_of(sgqlc.types.non_null('PeriodicJob'))), graphql_name='importPeriodicJobs', args=sgqlc.types.ArgDict((
+        ('file_uuid', sgqlc.types.Arg(sgqlc.types.non_null(String), graphql_name='fileUUID', default=None)),
+))
+    )
     delete_project = sgqlc.types.Field(sgqlc.types.non_null('State'), graphql_name='deleteProject', args=sgqlc.types.ArgDict((
         ('ids', sgqlc.types.Arg(sgqlc.types.non_null(sgqlc.types.list_of(sgqlc.types.non_null(ID))), graphql_name='ids', default=None)),
 ))
     )
     delete_project_versions = sgqlc.types.Field(sgqlc.types.non_null('State'), graphql_name='deleteProjectVersions', args=sgqlc.types.ArgDict((
         ('project_id', sgqlc.types.Arg(sgqlc.types.non_null(ID), graphql_name='projectId', default=None)),
         ('ids', sgqlc.types.Arg(sgqlc.types.non_null(sgqlc.types.list_of(sgqlc.types.non_null(ID))), graphql_name='ids', default=None)),
@@ -913,14 +923,20 @@
 class PeriodicJobPagination(sgqlc.types.Type):
     __schema__ = crawlers_api_schema
     __field_names__ = ('total', 'list_periodic_job')
     total = sgqlc.types.Field(sgqlc.types.non_null(Long), graphql_name='total')
     list_periodic_job = sgqlc.types.Field(sgqlc.types.non_null(sgqlc.types.list_of(sgqlc.types.non_null('PeriodicJob'))), graphql_name='listPeriodicJob')
 
 
+class Platform(sgqlc.types.Type):
+    __schema__ = crawlers_api_schema
+    __field_names__ = ('id',)
+    id = sgqlc.types.Field(sgqlc.types.non_null(ID), graphql_name='id')
+
+
 class ProjectData(sgqlc.types.Type):
     __schema__ = crawlers_api_schema
     __field_names__ = ('id', 'title')
     id = sgqlc.types.Field(sgqlc.types.non_null(ID), graphql_name='id')
     title = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='title')
 
 
@@ -949,15 +965,15 @@
     jobs_with_errors_logs_count = sgqlc.types.Field(Int, graphql_name='jobsWithErrorsLogsCount')
     job_ids_with_error_logs = sgqlc.types.Field(sgqlc.types.non_null(sgqlc.types.list_of(sgqlc.types.non_null(Long))), graphql_name='jobIdsWithErrorLogs')
     jobs_with_critical_logs_count = sgqlc.types.Field(Int, graphql_name='jobsWithCriticalLogsCount')
 
 
 class Query(sgqlc.types.Type):
     __schema__ = crawlers_api_schema
-    __field_names__ = ('analytics', 'crawler', 'list_crawler', 'pagination_crawler', 'crawler_args_and_settings_description', 'crawler_site_map', 'crawl_state', 'crawl_state_by_parameters', 'pagination_crawl_state', 'credential', 'pagination_credential', 'job', 'list_job', 'pagination_job_logs', 'pagination_job_requests', 'pagination_job_metrics', 'pagination_job', 'periodic_job', 'pagination_periodic_job', 'pagination_periodic_job_logs', 'pagination_periodic_job_requests', 'pagination_periodic_job_metrics', 'check_periodic_job_by_input', 'project', 'pagination_project', 'project_args_and_settings_description', 'project_default_args_and_settings_description', 'information_source_loader', 'pagination_information_source_loader', 'information_source', 'pagination_information_source', 'recovery_job', 'pagination_recovery_job', 'version', 'list_version', 'pagination_versions_crawler', 'pagination_egg_file_versions_project', 'web_scraper_version_is_compatible')
+    __field_names__ = ('analytics', 'crawler', 'list_crawler', 'pagination_crawler', 'crawler_args_and_settings_description', 'crawler_site_map', 'crawl_state', 'crawl_state_by_parameters', 'pagination_crawl_state', 'credential', 'pagination_credential', 'job', 'list_job', 'pagination_job_logs', 'pagination_job_requests', 'pagination_job_metrics', 'pagination_job', 'periodic_job', 'pagination_periodic_job', 'pagination_periodic_job_logs', 'pagination_periodic_job_requests', 'pagination_periodic_job_metrics', 'check_periodic_job_by_input', 'export_periodic_jobs', 'project', 'pagination_project', 'project_args_and_settings_description', 'project_default_args_and_settings_description', 'information_source_loader', 'pagination_information_source_loader', 'information_source', 'pagination_information_source', 'recovery_job', 'pagination_recovery_job', 'version', 'list_version', 'pagination_versions_crawler', 'pagination_egg_file_versions_project', 'web_scraper_version_is_compatible')
     analytics = sgqlc.types.Field(sgqlc.types.non_null('Stats'), graphql_name='analytics')
     crawler = sgqlc.types.Field(sgqlc.types.non_null('Crawler'), graphql_name='crawler', args=sgqlc.types.ArgDict((
         ('id', sgqlc.types.Arg(sgqlc.types.non_null(ID), graphql_name='id', default=None)),
 ))
     )
     list_crawler = sgqlc.types.Field(sgqlc.types.non_null(sgqlc.types.list_of('Crawler')), graphql_name='listCrawler', args=sgqlc.types.ArgDict((
         ('ids', sgqlc.types.Arg(sgqlc.types.non_null(sgqlc.types.list_of(sgqlc.types.non_null(ID))), graphql_name='ids', default=None)),
@@ -1090,14 +1106,18 @@
         ('sort_field', sgqlc.types.Arg(MetricSorting, graphql_name='sortField', default='timestamp')),
 ))
     )
     check_periodic_job_by_input = sgqlc.types.Field('PeriodicJob', graphql_name='checkPeriodicJobByInput', args=sgqlc.types.ArgDict((
         ('periodic_job_input', sgqlc.types.Arg(sgqlc.types.non_null(PeriodicJobInput), graphql_name='periodicJobInput', default=None)),
 ))
     )
+    export_periodic_jobs = sgqlc.types.Field(sgqlc.types.non_null(JSON), graphql_name='exportPeriodicJobs', args=sgqlc.types.ArgDict((
+        ('filter_settings', sgqlc.types.Arg(PeriodicJobFilterSettings, graphql_name='filterSettings', default={})),
+))
+    )
     project = sgqlc.types.Field(sgqlc.types.non_null('Project'), graphql_name='project', args=sgqlc.types.ArgDict((
         ('id', sgqlc.types.Arg(sgqlc.types.non_null(ID), graphql_name='id', default=None)),
 ))
     )
     pagination_project = sgqlc.types.Field(sgqlc.types.non_null(ProjectPagination), graphql_name='paginationProject', args=sgqlc.types.ArgDict((
         ('limit', sgqlc.types.Arg(Int, graphql_name='limit', default=20)),
         ('offset', sgqlc.types.Arg(Int, graphql_name='offset', default=0)),
@@ -1362,22 +1382,23 @@
     actual_status = sgqlc.types.Field(sgqlc.types.non_null(InformationSourceLoaderActualStatus), graphql_name='actualStatus')
     status = sgqlc.types.Field(sgqlc.types.non_null(CollectionStatus), graphql_name='status')
     metrics = sgqlc.types.Field(sgqlc.types.non_null(InformationSourceLoaderStats), graphql_name='metrics')
 
 
 class Job(sgqlc.types.Type, RecordInterface):
     __schema__ = crawlers_api_schema
-    __field_names__ = ('id', 'status', 'priority', 'message_priority', 'start_time', 'end_time', 'collection_status', 'is_noise', 'crawler', 'project', 'version', 'periodic', 'settings', 'args', 'metrics', 'job_stats', 'histogram_requests', 'histogram_items', 'schema')
+    __field_names__ = ('id', 'status', 'priority', 'message_priority', 'start_time', 'end_time', 'collection_status', 'monitoring_status', 'is_noise', 'crawler', 'project', 'version', 'periodic', 'settings', 'args', 'metrics', 'job_stats', 'histogram_requests', 'histogram_items', 'schema')
     id = sgqlc.types.Field(sgqlc.types.non_null(ID), graphql_name='id')
     status = sgqlc.types.Field(sgqlc.types.non_null(JobStatus), graphql_name='status')
     priority = sgqlc.types.Field(sgqlc.types.non_null(JobPriorityType), graphql_name='priority')
     message_priority = sgqlc.types.Field(sgqlc.types.non_null(MessagePriority), graphql_name='messagePriority')
     start_time = sgqlc.types.Field(UnixTime, graphql_name='startTime')
     end_time = sgqlc.types.Field(UnixTime, graphql_name='endTime')
     collection_status = sgqlc.types.Field(sgqlc.types.non_null(CollectionStatus), graphql_name='collectionStatus')
+    monitoring_status = sgqlc.types.Field(sgqlc.types.non_null(MonitoringStatus), graphql_name='monitoringStatus')
     is_noise = sgqlc.types.Field(sgqlc.types.non_null(Boolean), graphql_name='isNoise')
     crawler = sgqlc.types.Field(sgqlc.types.non_null(CrawlerData), graphql_name='crawler')
     project = sgqlc.types.Field(sgqlc.types.non_null(ProjectData), graphql_name='project')
     version = sgqlc.types.Field(sgqlc.types.non_null(VersionData), graphql_name='version')
     periodic = sgqlc.types.Field(PeriodicJobData, graphql_name='periodic')
     settings = sgqlc.types.Field(sgqlc.types.non_null(sgqlc.types.list_of(sgqlc.types.non_null(KeyValue))), graphql_name='settings')
     args = sgqlc.types.Field(sgqlc.types.non_null(sgqlc.types.list_of(sgqlc.types.non_null(KeyValue))), graphql_name='args')
@@ -1386,24 +1407,25 @@
     histogram_requests = sgqlc.types.Field(sgqlc.types.non_null(sgqlc.types.list_of(sgqlc.types.non_null(DateHistogramBucket))), graphql_name='histogramRequests')
     histogram_items = sgqlc.types.Field(sgqlc.types.non_null(sgqlc.types.list_of(sgqlc.types.non_null(DateHistogramBucket))), graphql_name='histogramItems')
     schema = sgqlc.types.Field(sgqlc.types.non_null(sgqlc.types.list_of(sgqlc.types.non_null(KeyValue))), graphql_name='schema')
 
 
 class PeriodicJob(sgqlc.types.Type, RecordInterface):
     __schema__ = crawlers_api_schema
-    __field_names__ = ('id', 'name', 'description', 'project', 'crawler', 'version', 'priority', 'message_priority', 'status', 'cron', 'cron_utcoffset_minutes', 'next_schedule_time', 'update_on_reload', 'settings', 'args', 'metrics', 'histogram_requests', 'histogram_items', 'job_stats')
+    __field_names__ = ('id', 'name', 'description', 'project', 'crawler', 'version', 'priority', 'message_priority', 'status', 'monitoring_status', 'cron', 'cron_utcoffset_minutes', 'next_schedule_time', 'update_on_reload', 'settings', 'args', 'metrics', 'histogram_requests', 'histogram_items', 'job_stats', 'job_failed_monitoring_statuses')
     id = sgqlc.types.Field(sgqlc.types.non_null(ID), graphql_name='id')
     name = sgqlc.types.Field(String, graphql_name='name')
     description = sgqlc.types.Field(String, graphql_name='description')
     project = sgqlc.types.Field(sgqlc.types.non_null(ProjectData), graphql_name='project')
     crawler = sgqlc.types.Field(sgqlc.types.non_null(CrawlerData), graphql_name='crawler')
     version = sgqlc.types.Field(sgqlc.types.non_null(VersionData), graphql_name='version')
     priority = sgqlc.types.Field(sgqlc.types.non_null(JobPriorityType), graphql_name='priority')
     message_priority = sgqlc.types.Field(sgqlc.types.non_null(MessagePriority), graphql_name='messagePriority')
     status = sgqlc.types.Field(sgqlc.types.non_null(PeriodicJobStatus), graphql_name='status')
+    monitoring_status = sgqlc.types.Field(sgqlc.types.non_null(MonitoringStatus), graphql_name='monitoringStatus')
     cron = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='cron')
     cron_utcoffset_minutes = sgqlc.types.Field(sgqlc.types.non_null(Int), graphql_name='cronUTCOffsetMinutes')
     next_schedule_time = sgqlc.types.Field(UnixTime, graphql_name='nextScheduleTime')
     update_on_reload = sgqlc.types.Field(sgqlc.types.non_null(Boolean), graphql_name='updateOnReload')
     settings = sgqlc.types.Field(sgqlc.types.non_null(sgqlc.types.list_of(sgqlc.types.non_null(KeyValue))), graphql_name='settings')
     args = sgqlc.types.Field(sgqlc.types.non_null(sgqlc.types.list_of(sgqlc.types.non_null(KeyValue))), graphql_name='args')
     metrics = sgqlc.types.Field(sgqlc.types.non_null(PeriodicJobMetrics), graphql_name='metrics')
@@ -1415,14 +1437,15 @@
         ('interval', sgqlc.types.Arg(TimestampInterval, graphql_name='interval', default=None)),
 ))
     )
     job_stats = sgqlc.types.Field(sgqlc.types.non_null(JobStats), graphql_name='jobStats', args=sgqlc.types.ArgDict((
         ('interval', sgqlc.types.Arg(TimestampInterval, graphql_name='interval', default=None)),
 ))
     )
+    job_failed_monitoring_statuses = sgqlc.types.Field(sgqlc.types.non_null(sgqlc.types.list_of(sgqlc.types.non_null(MonitoringStatus))), graphql_name='jobFailedMonitoringStatuses')
 
 
 class Project(sgqlc.types.Type, RecordInterface):
     __schema__ = crawlers_api_schema
     __field_names__ = ('id', 'name', 'title', 'description', 'crawlers_num', 'periodic_jobs_num', 'jobs_num', 'settings', 'args', 'project_stats', 'histogram_items', 'histogram_crawlers', 'current_version', 'egg_file')
     id = sgqlc.types.Field(sgqlc.types.non_null(ID), graphql_name='id')
     name = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='name')
```

### Comparing `ptal_api-0.11.6.1/ptal_api/schema/tcontroller_api_schema.py` & `ptal_api-0.12.0/ptal_api/schema/tcontroller_api_schema.py`

 * *Files identical despite different names*

### Comparing `ptal_api-0.11.6.1/ptal_api/schema/utils_api_schema.py` & `ptal_api-0.12.0/ptal_api/schema/utils_api_schema.py`

 * *Files 1% similar despite different names*

```diff
@@ -758,14 +758,21 @@
 class ConceptCandidateFactMention(sgqlc.types.Type):
     __schema__ = utils_api_schema
     __field_names__ = ('concept', 'mention')
     concept = sgqlc.types.Field(sgqlc.types.non_null('ConceptCandidateFact'), graphql_name='concept')
     mention = sgqlc.types.Field(sgqlc.types.non_null('Mention'), graphql_name='mention')
 
 
+class ConceptFacet(sgqlc.types.Type):
+    __schema__ = utils_api_schema
+    __field_names__ = ('count', 'value')
+    count = sgqlc.types.Field(sgqlc.types.non_null(Long), graphql_name='count')
+    value = sgqlc.types.Field(sgqlc.types.non_null('Concept'), graphql_name='value')
+
+
 class ConceptFactLink(sgqlc.types.Type):
     __schema__ = utils_api_schema
     __field_names__ = ('concept_id', 'concept_fact_id', 'status', 'is_implicit', 'concept', 'concept_fact')
     concept_id = sgqlc.types.Field(sgqlc.types.non_null(ID), graphql_name='conceptId')
     concept_fact_id = sgqlc.types.Field(sgqlc.types.non_null(ID), graphql_name='conceptFactId')
     status = sgqlc.types.Field(FactStatus, graphql_name='status')
     is_implicit = sgqlc.types.Field(sgqlc.types.non_null(Boolean), graphql_name='isImplicit')
@@ -1204,24 +1211,25 @@
     __field_names__ = ('total', 'list_merged_concept')
     total = sgqlc.types.Field(sgqlc.types.non_null(Long), graphql_name='total')
     list_merged_concept = sgqlc.types.Field(sgqlc.types.non_null(sgqlc.types.list_of(sgqlc.types.non_null(MergedConcept))), graphql_name='listMergedConcept')
 
 
 class Metrics(sgqlc.types.Type):
     __schema__ = utils_api_schema
-    __field_names__ = ('count_objects', 'count_events', 'count_named_entities', 'count_disambiguated_entities', 'count_property_candidates', 'count_links', 'count_research_maps', 'count_child_docs', 'count_tasks', 'count_concepts', 'count_entities')
+    __field_names__ = ('count_objects', 'count_events', 'count_named_entities', 'count_disambiguated_entities', 'count_property_candidates', 'count_links', 'count_research_maps', 'count_child_docs', 'count_tasks', 'count_story_docs', 'count_concepts', 'count_entities')
     count_objects = sgqlc.types.Field(sgqlc.types.non_null(Int), graphql_name='countObjects')
     count_events = sgqlc.types.Field(sgqlc.types.non_null(Int), graphql_name='countEvents')
     count_named_entities = sgqlc.types.Field(sgqlc.types.non_null(Int), graphql_name='countNamedEntities')
     count_disambiguated_entities = sgqlc.types.Field(sgqlc.types.non_null(Int), graphql_name='countDisambiguatedEntities')
     count_property_candidates = sgqlc.types.Field(sgqlc.types.non_null(Int), graphql_name='countPropertyCandidates')
     count_links = sgqlc.types.Field(sgqlc.types.non_null(Int), graphql_name='countLinks')
     count_research_maps = sgqlc.types.Field(sgqlc.types.non_null(Int), graphql_name='countResearchMaps')
     count_child_docs = sgqlc.types.Field(sgqlc.types.non_null(Int), graphql_name='countChildDocs')
     count_tasks = sgqlc.types.Field(sgqlc.types.non_null(Int), graphql_name='countTasks')
+    count_story_docs = sgqlc.types.Field(sgqlc.types.non_null(Int), graphql_name='countStoryDocs')
     count_concepts = sgqlc.types.Field(sgqlc.types.non_null(Int), graphql_name='countConcepts')
     count_entities = sgqlc.types.Field(sgqlc.types.non_null(Int), graphql_name='countEntities')
 
 
 class Mutation(sgqlc.types.Type):
     __schema__ = utils_api_schema
     __field_names__ = ('add_alias_to_concept', 'get_or_add_account', 'get_or_add_platform', 'get_or_add_concept')
@@ -1456,15 +1464,15 @@
 class StoryPagination(sgqlc.types.Type):
     __schema__ = utils_api_schema
     __field_names__ = ('list_story', 'total', 'show_total', 'list_named_entity_count_facet', 'list_concept_count_facet', 'list_account_count_facet', 'list_platform_count_facet', 'list_markers', 'sources', 'new_documents_today')
     list_story = sgqlc.types.Field(sgqlc.types.non_null(sgqlc.types.list_of(sgqlc.types.non_null(Story))), graphql_name='listStory')
     total = sgqlc.types.Field(sgqlc.types.non_null(Int), graphql_name='total')
     show_total = sgqlc.types.Field(sgqlc.types.non_null(Int), graphql_name='showTotal')
     list_named_entity_count_facet = sgqlc.types.Field(sgqlc.types.non_null(sgqlc.types.list_of(sgqlc.types.non_null(Facet))), graphql_name='listNamedEntityCountFacet')
-    list_concept_count_facet = sgqlc.types.Field(sgqlc.types.non_null(sgqlc.types.list_of(sgqlc.types.non_null(Facet))), graphql_name='listConceptCountFacet')
+    list_concept_count_facet = sgqlc.types.Field(sgqlc.types.non_null(sgqlc.types.list_of(sgqlc.types.non_null(ConceptFacet))), graphql_name='listConceptCountFacet')
     list_account_count_facet = sgqlc.types.Field(sgqlc.types.non_null(sgqlc.types.list_of(sgqlc.types.non_null(AccountFacet))), graphql_name='listAccountCountFacet')
     list_platform_count_facet = sgqlc.types.Field(sgqlc.types.non_null(sgqlc.types.list_of(sgqlc.types.non_null(PlatformFacet))), graphql_name='listPlatformCountFacet')
     list_markers = sgqlc.types.Field(sgqlc.types.non_null(sgqlc.types.list_of(sgqlc.types.non_null(Facet))), graphql_name='listMarkers')
     sources = sgqlc.types.Field(sgqlc.types.non_null(Int), graphql_name='sources')
     new_documents_today = sgqlc.types.Field(sgqlc.types.non_null(Int), graphql_name='newDocumentsToday')
```

### Comparing `ptal_api-0.11.6.1/ptal_api/scripts/type_mapper.py` & `ptal_api-0.12.0/ptal_api/scripts/type_mapper.py`

 * *Files identical despite different names*

### Comparing `ptal_api-0.11.6.1/ptal_api/tdm_builder/tdm_builder.py` & `ptal_api-0.12.0/ptal_api/tdm_builder/tdm_builder.py`

 * *Files identical despite different names*

### Comparing `ptal_api-0.11.6.1/pyproject.toml` & `ptal_api-0.12.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ptal-api"
-version = "0.11.6.1"
+version = "0.12.0"
 description = "TALISMAN API adapter"
 authors = ["Evgeny Bechkalo <bechkalo@ispras.ru>", "Ivan Medvedev <medvedev.iv@ispras.ru>", "Alexey Isakov <isakov@ispras.ru>"]
 readme = "README.md"
 packages = [{include = "ptal_api"}]
 classifiers = [
     'Development Status :: 3 - Alpha',
     'Programming Language :: Python :: 3',
```

### Comparing `ptal_api-0.11.6.1/PKG-INFO` & `ptal_api-0.12.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ptal-api
-Version: 0.11.6.1
+Version: 0.12.0
 Summary: TALISMAN API adapter
 Author: Evgeny Bechkalo
 Author-email: bechkalo@ispras.ru
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

