# Comparing `tmp/ptal_api-0.12.0.1.tar.gz` & `tmp/ptal_api-0.12.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ptal_api-0.12.0.1.tar", max compression
+gzip compressed data, was "ptal_api-0.12.2.tar", max compression
```

## Comparing `ptal_api-0.12.0.1.tar` & `ptal_api-0.12.2.tar`

### file list

```diff
@@ -1,33 +1,39 @@
--rw-r--r--   0        0        0      627 2023-06-14 09:48:33.647136 ptal_api-0.12.0.1/README.md
--rw-r--r--   0        0        0        0 2023-06-14 09:48:33.703136 ptal_api-0.12.0.1/ptal_api/__init__.py
--rw-r--r--   0        0        0   108219 2023-06-14 09:48:33.647136 ptal_api-0.12.0.1/ptal_api/adapter.py
--rw-r--r--   0        0        0      184 2023-06-14 09:48:33.647136 ptal_api-0.12.0.1/ptal_api/core/kb_sync/kb_iterator_config.py
--rw-r--r--   0        0        0      160 2023-06-14 09:48:33.647136 ptal_api-0.12.0.1/ptal_api/core/kb_sync/object_time_interval.py
--rw-r--r--   0        0        0      484 2023-06-14 09:48:33.651136 ptal_api-0.12.0.1/ptal_api/core/query_factory.py
--rw-r--r--   0        0        0      435 2023-06-14 09:48:33.651136 ptal_api-0.12.0.1/ptal_api/core/type_mapper/app_settings/logging.conf
--rw-r--r--   0        0        0      737 2023-06-14 09:48:33.651136 ptal_api-0.12.0.1/ptal_api/core/type_mapper/common/common.py
--rw-r--r--   0        0        0    14955 2023-06-14 09:48:33.651136 ptal_api-0.12.0.1/ptal_api/core/type_mapper/data_model/base_data_model.py
--rw-r--r--   0        0        0      904 2023-06-14 09:48:33.651136 ptal_api-0.12.0.1/ptal_api/core/type_mapper/data_model/config_data_model.py
--rw-r--r--   0        0        0     3255 2023-06-14 09:48:33.651136 ptal_api-0.12.0.1/ptal_api/core/type_mapper/data_model/custom_data_model.py
--rw-r--r--   0        0        0     3501 2023-06-14 09:48:33.651136 ptal_api-0.12.0.1/ptal_api/core/type_mapper/model_parameters/name_code_mapping.yml
--rw-r--r--   0        0        0     2194 2023-06-14 09:48:33.651136 ptal_api-0.12.0.1/ptal_api/core/type_mapper/modules/custom_data_handler.py
--rw-r--r--   0        0        0     1464 2023-06-14 09:48:33.651136 ptal_api-0.12.0.1/ptal_api/core/type_mapper/modules/file_generator.py
--rw-r--r--   0        0        0     4556 2023-06-14 09:48:33.651136 ptal_api-0.12.0.1/ptal_api/core/type_mapper/modules/object_name_transformer.py
--rw-r--r--   0        0        0    23314 2023-06-14 09:48:33.651136 ptal_api-0.12.0.1/ptal_api/core/type_mapper/modules/type_mapping_generator.py
--rw-r--r--   0        0        0     1800 2023-06-14 09:48:33.651136 ptal_api-0.12.0.1/ptal_api/core/type_mapper/modules/type_mapping_loader/type_mapping_loader.py
--rw-r--r--   0        0        0      418 2023-06-14 09:48:33.651136 ptal_api-0.12.0.1/ptal_api/core/type_mapper/modules/type_mapping_loader/type_mapping_loader_interface.py
--rw-r--r--   0        0        0      192 2023-06-14 09:48:33.651136 ptal_api-0.12.0.1/ptal_api/core/values/date_dataclass.py
--rw-r--r--   0        0        0     3279 2023-06-14 09:48:33.651136 ptal_api-0.12.0.1/ptal_api/core/values/value_mapping.py
--rw-r--r--   0        0        0        0 2023-06-14 09:48:33.703136 ptal_api-0.12.0.1/ptal_api/providers/__init__.py
--rw-r--r--   0        0        0     4668 2023-06-14 09:48:33.651136 ptal_api-0.12.0.1/ptal_api/providers/gql_providers.py
--rw-r--r--   0        0        0     1186 2023-06-14 09:48:33.651136 ptal_api-0.12.0.1/ptal_api/schema/README.md
--rw-r--r--   0        0        0        0 2023-06-14 09:48:33.703136 ptal_api-0.12.0.1/ptal_api/schema/__init__.py
--rw-r--r--   0        0        0   290619 2023-06-14 09:48:33.655136 ptal_api-0.12.0.1/ptal_api/schema/api_schema.py
--rw-r--r--   0        0        0    95040 2023-06-14 09:48:33.655136 ptal_api-0.12.0.1/ptal_api/schema/crawlers_api_schema.py
--rw-r--r--   0        0        0    74033 2023-06-14 09:48:33.655136 ptal_api-0.12.0.1/ptal_api/schema/tcontroller_api_schema.py
--rw-r--r--   0        0        0   137251 2023-06-14 09:48:33.655136 ptal_api-0.12.0.1/ptal_api/schema/utils_api_schema.py
--rw-r--r--   0        0        0     3662 2023-06-14 09:48:33.655136 ptal_api-0.12.0.1/ptal_api/scripts/type_mapper.py
--rw-r--r--   0        0        0        0 2023-06-14 09:48:33.707136 ptal_api-0.12.0.1/ptal_api/tdm_builder/__init__.py
--rw-r--r--   0        0        0     1211 2023-06-14 09:48:33.655136 ptal_api-0.12.0.1/ptal_api/tdm_builder/tdm_builder.py
--rw-r--r--   0        0        0     1873 2023-06-14 09:48:33.655136 ptal_api-0.12.0.1/pyproject.toml
--rw-r--r--   0        0        0     1491 1970-01-01 00:00:00.000000 ptal_api-0.12.0.1/PKG-INFO
+-rw-r--r--   0        0        0      627 2023-06-27 08:38:38.936916 ptal_api-0.12.2/README.md
+-rw-r--r--   0        0        0        0 2023-06-27 08:38:38.992917 ptal_api-0.12.2/ptal_api/__init__.py
+-rw-r--r--   0        0        0   120656 2023-06-27 08:38:38.936916 ptal_api-0.12.2/ptal_api/adapter.py
+-rw-r--r--   0        0        0      184 2023-06-27 08:38:38.936916 ptal_api-0.12.2/ptal_api/core/kb_sync/kb_iterator_config.py
+-rw-r--r--   0        0        0      160 2023-06-27 08:38:38.936916 ptal_api-0.12.2/ptal_api/core/kb_sync/object_time_interval.py
+-rw-r--r--   0        0        0      484 2023-06-27 08:38:38.936916 ptal_api-0.12.2/ptal_api/core/query_factory.py
+-rw-r--r--   0        0        0      435 2023-06-27 08:38:38.936916 ptal_api-0.12.2/ptal_api/core/type_mapper/app_settings/logging.conf
+-rw-r--r--   0        0        0      737 2023-06-27 08:38:38.940916 ptal_api-0.12.2/ptal_api/core/type_mapper/common/common.py
+-rw-r--r--   0        0        0    14955 2023-06-27 08:38:38.940916 ptal_api-0.12.2/ptal_api/core/type_mapper/data_model/base_data_model.py
+-rw-r--r--   0        0        0      904 2023-06-27 08:38:38.940916 ptal_api-0.12.2/ptal_api/core/type_mapper/data_model/config_data_model.py
+-rw-r--r--   0        0        0     3255 2023-06-27 08:38:38.940916 ptal_api-0.12.2/ptal_api/core/type_mapper/data_model/custom_data_model.py
+-rw-r--r--   0        0        0     3501 2023-06-27 08:38:38.940916 ptal_api-0.12.2/ptal_api/core/type_mapper/model_parameters/name_code_mapping.yml
+-rw-r--r--   0        0        0     2194 2023-06-27 08:38:38.940916 ptal_api-0.12.2/ptal_api/core/type_mapper/modules/custom_data_handler.py
+-rw-r--r--   0        0        0     1464 2023-06-27 08:38:38.940916 ptal_api-0.12.2/ptal_api/core/type_mapper/modules/file_generator.py
+-rw-r--r--   0        0        0     4556 2023-06-27 08:38:38.940916 ptal_api-0.12.2/ptal_api/core/type_mapper/modules/object_name_transformer.py
+-rw-r--r--   0        0        0    23314 2023-06-27 08:38:38.940916 ptal_api-0.12.2/ptal_api/core/type_mapper/modules/type_mapping_generator.py
+-rw-r--r--   0        0        0     1800 2023-06-27 08:38:38.940916 ptal_api-0.12.2/ptal_api/core/type_mapper/modules/type_mapping_loader/type_mapping_loader.py
+-rw-r--r--   0        0        0      418 2023-06-27 08:38:38.940916 ptal_api-0.12.2/ptal_api/core/type_mapper/modules/type_mapping_loader/type_mapping_loader_interface.py
+-rw-r--r--   0        0        0      192 2023-06-27 08:38:38.940916 ptal_api-0.12.2/ptal_api/core/values/date_dataclass.py
+-rw-r--r--   0        0        0     3571 2023-06-27 08:38:38.940916 ptal_api-0.12.2/ptal_api/core/values/value_mapping.py
+-rw-r--r--   0        0        0      295 2023-06-27 08:38:38.940916 ptal_api-0.12.2/ptal_api/pretty_adapter/common.py
+-rw-r--r--   0        0        0     1880 2023-06-27 08:38:38.940916 ptal_api-0.12.2/ptal_api/pretty_adapter/object_types.py
+-rw-r--r--   0        0        0     2884 2023-06-27 08:38:38.940916 ptal_api-0.12.2/ptal_api/pretty_adapter/objects.py
+-rw-r--r--   0        0        0     3716 2023-06-27 08:38:38.940916 ptal_api-0.12.2/ptal_api/pretty_adapter/pretty_adapter.py
+-rw-r--r--   0        0        0      595 2023-06-27 08:38:38.940916 ptal_api-0.12.2/ptal_api/pretty_adapter/property_values.py
+-rw-r--r--   0        0        0    16486 2023-06-27 08:38:38.940916 ptal_api-0.12.2/ptal_api/pretty_adapter/transformer.py
+-rw-r--r--   0        0        0        0 2023-06-27 08:38:38.996917 ptal_api-0.12.2/ptal_api/providers/__init__.py
+-rw-r--r--   0        0        0     4668 2023-06-27 08:38:38.940916 ptal_api-0.12.2/ptal_api/providers/gql_providers.py
+-rw-r--r--   0        0        0     1282 2023-06-27 08:38:38.940916 ptal_api-0.12.2/ptal_api/schema/README.md
+-rw-r--r--   0        0        0        0 2023-06-27 08:38:38.996917 ptal_api-0.12.2/ptal_api/schema/__init__.py
+-rw-r--r--   0        0        0   290589 2023-06-27 08:38:38.944916 ptal_api-0.12.2/ptal_api/schema/api_schema.py
+-rw-r--r--   0        0        0    96961 2023-06-27 08:38:38.944916 ptal_api-0.12.2/ptal_api/schema/crawlers_api_schema.py
+-rw-r--r--   0        0        0    74033 2023-06-27 08:38:38.944916 ptal_api-0.12.2/ptal_api/schema/tcontroller_api_schema.py
+-rw-r--r--   0        0        0   137221 2023-06-27 08:38:38.948916 ptal_api-0.12.2/ptal_api/schema/utils_api_schema.py
+-rw-r--r--   0        0        0     3662 2023-06-27 08:38:38.948916 ptal_api-0.12.2/ptal_api/scripts/type_mapper.py
+-rw-r--r--   0        0        0        0 2023-06-27 08:38:38.996917 ptal_api-0.12.2/ptal_api/tdm_builder/__init__.py
+-rw-r--r--   0        0        0     1211 2023-06-27 08:38:38.948916 ptal_api-0.12.2/ptal_api/tdm_builder/tdm_builder.py
+-rw-r--r--   0        0        0     1871 2023-06-27 08:38:38.948916 ptal_api-0.12.2/pyproject.toml
+-rw-r--r--   0        0        0     1489 1970-01-01 00:00:00.000000 ptal_api-0.12.2/PKG-INFO
```

### Comparing `ptal_api-0.12.0.1/README.md` & `ptal_api-0.12.2/README.md`

 * *Files identical despite different names*

### Comparing `ptal_api-0.12.0.1/ptal_api/adapter.py` & `ptal_api-0.12.2/ptal_api/adapter.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,37 +1,39 @@
 import json
 import logging
 from copy import copy
 from functools import wraps
 from time import time
 from typing import Any, Dict, Iterable, List, Optional, Sequence, Union
 
+from deprecation import deprecated
 from sgqlc.operation import Fragment
 
 from .core.kb_sync.kb_iterator_config import KBIteratorConfig
 from .core.kb_sync.object_time_interval import ObjectTimeInterval
 from .core.query_factory import make_operation
 from .core.type_mapper.data_model.base_data_model import TypeMapping
 from .core.type_mapper.modules.type_mapping_loader.type_mapping_loader import TypeMappingLoader
 from .core.type_mapper.modules.type_mapping_loader.type_mapping_loader_interface import TypeMappingLoaderInterface
 from .core.values.value_mapping import get_map_helper
+from .pretty_adapter import object_types, objects
+from .pretty_adapter.transformer import prettify
 from .providers.gql_providers import AbstractGQLClient
 from .schema import tcontroller_api_schema as tc
 from .schema import utils_api_schema as uas
 from .schema.api_schema import (
     ComponentValueInput,
     CompositeConcept,
     CompositeConceptWidgetRowPagination,
     CompositePropertyTypeFilterSettings,
     CompositePropertyTypeSorting,
     CompositePropertyValueTemplate,
     CompositePropertyValueType,
     CompositeValue,
     Concept,
-    ConceptCandidateFact,
     ConceptFact,
     ConceptFactPagination,
     ConceptFilterSettings,
     ConceptLink,
     ConceptLinkCreationMutationInput,
     ConceptLinkFilterSettings,
     ConceptLinkPagination,
@@ -123,21 +125,23 @@
         type_mapping: Optional[Union[str, dict, TypeMapping]] = None,
         type_mapping_loader: Optional[TypeMappingLoaderInterface] = None,
         tdm_builder: Optional[AbstractTdmBuilder] = None,
         utils_gql_client: Optional[AbstractGQLClient] = None,
         kb_iterator_config: Optional[KBIteratorConfig] = None,
         limit: int = 100,
         perform_synchronously: bool = True,
+        prettify_output: bool = False,
     ) -> None:
         self._gql_client = gql_client
         self._utils_gql_client = utils_gql_client
         self._type_mapping_loader = type_mapping_loader if type_mapping_loader else TypeMappingLoader(logger)
         self._type_mapping = self._type_mapping_loader.load_type_mapping(type_mapping)
         self._limit = limit
         self._perform_synchronously = perform_synchronously
+        self.prettify_output = prettify_output
 
         self.document_fields_truncated = (
             "id",
             "external_url",
             "uuid",
         )
         self.document_fields = (
@@ -151,22 +155,19 @@
             "system_registration_date",
             "system_update_date",
             "notes",
             "access_level",
             "trust_level",
             "uuid",
         )
-
-        self.document_text_fields_truncated = ("text",)
         self.document_text_fields = (
             "node_id",
             "text",
         )
         self.document_text_metadata_fields = ("paragraph_type",)
-
         self.document_platform_fields = (
             "id",
             "name",
         )
         self.document_account_fields = (
             "id",
             "name",
@@ -180,23 +181,20 @@
             "notes",
             "markers",
             "system_registration_date",
             "system_update_date",
         )
         self.concept_type_fields = ("id", "name")
 
-        self.concept_property_fields = ("is_main", "id", "system_registration_date")
-        self.concept_property_type_fields_truncated = ("id",)
+        self.concept_property_fields = ("id", "is_main", "system_registration_date")
         self.concept_property_type_fields = ("id", "name")
         self.cpvt_fields_truncated = ("id", "name", "value_type")
         self.cpvt_fields = ("id", "name", "value_type", "value_restriction", "pretrained_nercmodels")
 
         self.concept_link_fields = ("id", "notes")
-        self.concept_link_concept_from_fields = ("id",)
-        self.concept_link_concept_to_fields = ("id",)
         self.concept_link_type_fields = ("id", "name", "is_directed", "is_hierarchical")
         self.concept_link_type_fields_truncated = ("id", "name", "is_directed")
 
         self.concept_fact_fields = ("id",)
 
         self.composite_concept_widget_type = ("id", "name")
         self.composite_concept_widget_type_columns_info = ("name",)
@@ -212,14 +210,22 @@
         self.tdm_builder = tdm_builder
 
         if kb_iterator_config:
             self.kb_iterator_config = kb_iterator_config
         else:
             self.kb_iterator_config = KBIteratorConfig(1000, 1609448400)  # Fri Jan 01 2021 00:00:00 GMT+0300
 
+    @property
+    def prettify_output(self) -> bool:
+        return self._prettify_output
+
+    @prettify_output.setter
+    def prettify_output(self, value: bool) -> None:
+        self._prettify_output = value
+
     def get_tdm_builder(self) -> Optional[AbstractTdmBuilder]:
         return self.tdm_builder
 
     @property
     def type_mapping(self):
         return self._type_mapping
 
@@ -342,41 +348,35 @@
             self._configure_output_link_fields(pcl.list_concept_link(), with_link_properties=with_link_properties)
         if with_facts:
             pcf: ConceptFactPagination = concept_object.pagination_concept_fact(
                 offset=0, limit=10000, filter_settings={}
             )
             lcf = pcf.list_concept_fact()
             lcf.__fields__(*self.concept_fact_fields)
-            d = lcf.document()
-            d.__fields__(*self.document_fields)
-            dm = d.metadata()
-            dm.platform().__fields__(*self.document_platform_fields)
-            dm.account().__fields__(*self.document_account_fields)
+            self._configure_output_document_fields(lcf.document(), with_extended_information=True)
         if with_potential_facts:
-            lccf: List[ConceptCandidateFact] = concept_object.list_concept_candidate_fact()
+            lccf = concept_object.list_concept_candidate_fact()
             lccf.__fields__(*self.concept_fact_fields)
-            d = lccf.document()
-            d.__fields__(*self.document_fields)
-            dm = d.metadata()
-            dm.platform().__fields__(*self.document_platform_fields)
-            dm.account().__fields__(*self.document_account_fields)
+            self._configure_output_document_fields(lccf.document(), with_extended_information=True)
         if with_metrics:
             concept_object.metric()
 
-    def _configure_output_link_fields(self, link_object, with_link_properties=False):
+    def _configure_output_link_fields(self, link_object, with_link_properties=False, with_facts=False):
         link_object.__fields__(*self.concept_link_fields)
-        link_object.access_level()
-        link_object.concept_from().__fields__(*self.concept_link_concept_from_fields)
-        link_object.concept_to().__fields__(*self.concept_link_concept_to_fields)
         link_object.concept_link_type().__fields__(*self.concept_link_type_fields_truncated)
+        link_object.access_level()
+        self._configure_output_concept_fields(link_object.concept_from())
+        self._configure_output_concept_fields(link_object.concept_to())
         if with_link_properties:
             pcp: ConceptPropertyPagination = link_object.pagination_concept_link_property(
                 offset=0, limit=10000, filter_settings={}
             )
             self._configure_output_properties_fields(pcp.list_concept_property())
+        if with_facts:
+            link_object.__fields__("list_concept_link_fact")
 
     def _configure_output_document_fields(
         self,
         doc_object,
         *,
         with_extended_information=False,
         with_text=False,
@@ -415,23 +415,24 @@
                 with_extended_information=with_extended_information,
                 with_text=with_text,
                 with_text_metadata=with_text_metadata,
                 with_updater=with_updater,
                 with_creator=with_creator,
             )
 
+    @prettify
     def _create_concept_with_input(
         self,
         form: ConceptMutationInput,
         with_properties=False,
         with_links=False,
         with_link_properties=False,
         with_metrics=False,
         perform_synchronously: Optional[bool] = None,
-    ) -> Concept:
+    ) -> Union[Concept, objects.Concept]:
         op = make_operation(Mutation, "create_concept_with_input")
         ac = op.add_concept(
             performance_control=PerformSynchronously(
                 perform_synchronously=self.get_perform_synchronously_value(perform_synchronously)
             ),
             form=form,
         )
@@ -480,14 +481,15 @@
         return value_input
 
     def _configure_pipeline_topic_fields(self, kafka_topic: tc.KafkaTopic):
         kafka_topic.__fields__(*self.pipeline_topic_fields)
         kafka_topic.metrics().__fields__(*self.pipeline_metrics_fields)
         kafka_topic.pipeline().pipeline_config().__fields__(*self.pipeline_config_fields)
 
+    # @prettify
     def get_all_documents(
         self,
         grouping: DocumentGrouping = "none",
         filter_settings: Optional[DocumentFilterSettings] = None,
         direction: SortDirection = "descending",
         sort_field: DocumentSorting = "score",
         extra_settings: Optional[ExtraSettings] = None,
@@ -567,14 +569,15 @@
                 with_creator=with_creator,
                 with_facts=with_facts,
                 with_children=with_children,
             )
             yield from documents
             i += 1
 
+    # @prettify
     def get_documents(
         self,
         skip: int = 0,
         take: Optional[int] = None,
         grouping: DocumentGrouping = "none",
         filter_settings: Optional[DocumentFilterSettings] = None,
         direction: SortDirection = "descending",
@@ -602,15 +605,15 @@
             grouping=grouping,
             filter_settings=filter_settings,
             direction=direction,
             sort_field=sort_field,
             extra_settings=extra_settings,
             **pagination_story_kwargs,
         )
-        ps.list_story().list_document().__fields__(*self.document_fields_truncated)
+        self._configure_output_document_fields(ps.list_story().list_document())
         self._configure_output_document_fields(
             ps.list_story().main(),
             with_extended_information=with_extended_information,
             with_text=with_text,
             with_text_metadata=with_text_metadata,
             with_text_translation=with_text_translation,
             with_updater=with_updater,
@@ -631,14 +634,15 @@
             limit=1, filter_settings=filter_settings, extra_settings=ExtraSettings()
         )
         ps.show_total()
         res = self._gql_client.execute(op)
         res = op + res
         return res.pagination_story.show_total
 
+    # @prettify
     def get_documents_by_limit_offset_filter_extra_settings(
         self,
         skip: int = 0,
         take: Optional[int] = None,
         filter_settings: Optional[DocumentFilterSettings] = None,
         extra_settings: Optional[ExtraSettings] = None,
     ) -> Sequence[Story]:
@@ -646,21 +650,22 @@
         take = self.get_take_value(take)
         ps: StoryPagination = op.pagination_story(
             offset=skip,
             limit=take,
             extra_settings=extra_settings if extra_settings else ExtraSettings(),
             filter_settings=filter_settings if filter_settings else DocumentFilterSettings(),
         )
-        ps.list_story().list_document().__fields__(*self.document_fields_truncated)
+        self._configure_output_document_fields(ps.list_story().list_document())
         self._configure_output_document_fields(ps.list_story().main())
 
         res = self._gql_client.execute(op)
         res = op + res
         return res.pagination_story.list_story
 
+    # @prettify
     def get_document(self, document_id: str) -> Document:
         op = make_operation(Query, "get_document")
         d: Document = op.document(id=document_id)
         self._configure_output_document_fields(
             d,
             with_extended_information=True,
             with_text=True,
@@ -692,24 +697,47 @@
             filter_settings=filter_settings if filter_settings else ConceptLinkFilterSettings()
         )
         pcl.total()
         res = self._gql_client.execute(op)
         res = op + res
         return res.pagination_concept_link.total
 
+    @prettify
     def get_concept(
         self,
         concept_id: str,
         with_aliases: bool = False,
         with_properties: bool = True,
         with_links: bool = True,
         with_link_properties: bool = True,
         with_facts: bool = False,
         with_potential_facts: bool = False,
         with_metrics: bool = True,
+    ) -> Union[Concept, objects.Concept]:
+        return self._get_concept(
+            concept_id,
+            with_aliases,
+            with_properties,
+            with_links,
+            with_link_properties,
+            with_facts,
+            with_potential_facts,
+            with_metrics,
+        )
+
+    def _get_concept(
+        self,
+        concept_id: str,
+        with_aliases: bool = False,
+        with_properties: bool = True,
+        with_links: bool = True,
+        with_link_properties: bool = True,
+        with_facts: bool = False,
+        with_potential_facts: bool = False,
+        with_metrics: bool = True,
     ) -> Concept:
         op = make_operation(Query, "get_concept")
         c: Concept = op.concept(id=concept_id)
         self._configure_output_concept_fields(
             c,
             with_aliases=with_aliases,
             with_properties=with_properties,
@@ -723,77 +751,73 @@
         res = op + res
 
         if self.tdm_builder is not None:
             self.tdm_builder.add_concept_fact(res.concept)
 
         return res.concept
 
-    def get_concept_property(self, concept_property_id: str) -> Concept:
+    @prettify
+    def get_concept_property(self, concept_property_id: str) -> Union[ConceptProperty, objects.Property]:
         op = make_operation(Query, "get_concept_property")
         cp: ConceptProperty = op.concept_property(id=concept_property_id)
 
-        cp.__fields__(*self.concept_property_fields)
-        cp.property_type().__fields__(*self.concept_property_type_fields)
-        self._configure_output_value_fields(cp.value)
+        self._configure_output_properties_fields(cp)
         res = self._gql_client.execute(op)
         res = op + res
 
         return res.concept_property
 
+    # @prettify
     def get_concept_facts(
         self, concept_id: str, filter_settings: Optional[DocumentLinkFilterSetting] = None
     ) -> Sequence[ConceptFact]:
         op = make_operation(Query, "get_concept_facts")
         c: Concept = op.concept(id=concept_id)
         pcf: ConceptFactPagination = c.pagination_concept_fact(
             filter_settings=filter_settings if filter_settings else DocumentLinkFilterSetting()
         )
         lcf = pcf.list_concept_fact()
         lcf.__fields__(*self.concept_fact_fields)
-        d = lcf.document()
-        d.__fields__(*self.document_fields)
-        dm = d.metadata()
-        dm.platform().__fields__(*self.document_platform_fields)
-        dm.account().__fields__(*self.document_account_fields)
+        self._configure_output_document_fields(lcf.document(), with_extended_information=True)
 
         res = self._gql_client.execute(op)
         res = op + res
 
         return res.concept.pagination_concept_fact.list_concept_fact
 
-    def get_concept_link(self, link_id: str, with_facts: bool = False) -> ConceptLink:
+    def _get_concept_link(self, link_id: str, with_facts: bool = False) -> ConceptLink:
         op = make_operation(Query, "get_concept_link")
         cl: ConceptLink = op.concept_link(id=link_id)
-        cl.__fields__(*self.concept_link_fields)
-        self._configure_output_concept_fields(cl.concept_from)
-        self._configure_output_concept_fields(cl.concept_to)
-        cl.concept_link_type.__fields__(*self.concept_link_type_fields_truncated)
-        if with_facts:
-            cl.__fields__("list_concept_link_fact")
+        self._configure_output_link_fields(cl, with_facts=with_facts)
         res = self._gql_client.execute(op)
         res = op + res
 
         if self.tdm_builder is not None:
             self.tdm_builder.add_link_fact(res.concept_link)
 
         return res.concept_link
 
+    @prettify
+    def get_concept_link(self, link_id: str, with_facts: bool = False) -> Union[ConceptLink, objects.Link]:
+        return self._get_concept_link(link_id, with_facts)
+
+    @prettify
     def get_all_concepts(
         self,
         filter_settings: Optional[ConceptFilterSettings] = None,
         direction: SortDirection = "descending",
         sort_field: ConceptSorting = "score",
         with_aliases: bool = False,
         with_properties: bool = False,
         with_links: bool = False,
         with_link_properties: bool = False,
         with_facts: bool = False,
         with_potential_facts: bool = False,
         with_metrics: bool = False,
-    ) -> Iterable[Concept]:
+    ) -> Union[Iterable[Concept], Iterable[objects.Concept]]:
         if not filter_settings:
             filter_settings = ConceptFilterSettings()
         total = self.get_concept_count(filter_settings=filter_settings)
 
         if total > self.kb_iterator_config.max_total_count:
             had_creation_date = hasattr(filter_settings, "creation_date")
             old_timestamp_interval = None
@@ -848,29 +872,30 @@
                 with_facts=with_facts,
                 with_potential_facts=with_potential_facts,
                 with_metrics=with_metrics,
             )
             yield from concepts
             i += 1
 
+    @prettify
     def get_concepts(
         self,
         skip: int = 0,
         take: Optional[int] = None,
         filter_settings: Optional[ConceptFilterSettings] = None,
         direction: SortDirection = "descending",
         sort_field: ConceptSorting = "score",
         with_aliases: bool = False,
         with_properties: bool = False,
         with_links: bool = False,
         with_link_properties: bool = False,
         with_facts: bool = False,
         with_potential_facts: bool = False,
         with_metrics: bool = False,
-    ) -> Sequence[Concept]:
+    ) -> Union[Sequence[Concept], Sequence[objects.Concept]]:
         op = make_operation(Query, "get_concepts")
         take = self.get_take_value(take)
         pagination_concept_kwargs = {}
         if not filter_settings:
             filter_settings = ConceptFilterSettings()
         cp: ConceptPagination = op.pagination_concept(
             limit=take,
@@ -890,23 +915,24 @@
             with_potential_facts=with_potential_facts,
             with_metrics=with_metrics,
         )
         res = self._gql_client.execute(op)
         res = op + res
         return res.pagination_concept.list_concept
 
+    @deprecated(details="Use get_concepts method instead")
     def get_concepts_by_limit_offset_filter_settings(
         self,
         skip: int = 0,
         take: Optional[int] = None,
         filter_settings: Optional[ConceptFilterSettings] = None,
         with_aliases: bool = False,
         with_facts: bool = False,
         with_potential_facts=False,
-    ) -> Sequence[Concept]:
+    ) -> Union[Sequence[Concept], Sequence[objects.Concept]]:
         op = make_operation(Query, "get_concepts_by_limit_offset_filter_settings")
         take = self.get_take_value(take)
         cp: ConceptPagination = op.pagination_concept(
             filter_settings=filter_settings if filter_settings else ConceptFilterSettings(), offset=skip, limit=take
         )
         self._configure_output_concept_fields(
             cp.list_concept(),
@@ -914,17 +940,18 @@
             with_facts=with_facts,
             with_potential_facts=with_potential_facts,
         )
         res = self._gql_client.execute(op)
         res = op + res
         return res.pagination_concept.list_concept
 
+    @prettify
     def get_all_concept_links(
         self, filter_settings: Optional[ConceptLinkFilterSettings] = None, with_link_properties: bool = False
-    ) -> Iterable[ConceptLink]:
+    ) -> Union[Iterable[ConceptLink], Iterable[objects.Link]]:
         if not filter_settings:
             filter_settings = ConceptLinkFilterSettings()
 
         total = self.get_concept_link_count(filter_settings=filter_settings)
 
         if total > self.kb_iterator_config.max_total_count:
             had_creation_date = hasattr(filter_settings, "creation_date")
@@ -964,31 +991,33 @@
                 take=self._limit,
                 filter_settings=filter_settings,
                 with_link_properties=with_link_properties,
             )
             yield from links
             i += 1
 
+    @prettify
     def get_concept_links_by_limit_offset_filter_settings(
         self,
         skip: int = 0,
         take: Optional[int] = None,
         filter_settings: Optional[ConceptLinkFilterSettings] = None,
         with_link_properties: bool = False,
-    ) -> Sequence[ConceptLink]:
+    ) -> Union[Sequence[ConceptLink], Sequence[objects.Link]]:
         op = make_operation(Query, "get_concept_links_by_limit_offset_filter_settings")
         take = self.get_take_value(take)
         pcl: ConceptLinkPagination = op.pagination_concept_link(
             filter_settings=filter_settings if filter_settings else ConceptLinkFilterSettings(), offset=skip, limit=take
         )
         self._configure_output_link_fields(pcl.list_concept_link(), with_link_properties=with_link_properties)
         res = self._gql_client.execute(op)
         res = op + res
         return res.pagination_concept_link.list_concept_link
 
+    @deprecated(details="Use get_concepts method instead")
     def get_concepts_by_type_id_with_offset(
         self,
         type_id: str,
         skip: int,
         take: Optional[int] = None,
         direction="descending",
         sort_field="systemRegistrationDate",
@@ -1018,14 +1047,15 @@
             with_facts=with_facts,
             with_potential_facts=with_potential_facts,
         )
         res = self._gql_client.execute(op)
         res = op + res
         return res.pagination_concept
 
+    @deprecated(details="Use get_concepts method instead")
     def get_concepts_by_type_id_with_offset_with_markers(
         self,
         type_id: str,
         skip: int = 0,
         take: Optional[int] = None,
         markers: Optional[List[str]] = None,
         direction="descending",
@@ -1053,22 +1083,23 @@
             with_facts=with_facts,
             with_potential_facts=with_potential_facts,
         )
         res = self._gql_client.execute(op)
         res = op + res
         return res.pagination_concept
 
+    @prettify
     def get_concepts_by_name(
         self,
         name: str,
         type_id: Optional[str] = None,
         with_aliases: bool = False,
         with_facts: bool = False,
         with_potential_facts=False,
-    ) -> Sequence[Concept]:
+    ) -> Union[Sequence[Concept], Sequence[objects.Concept]]:
         op = make_operation(Query, "get_concepts_by_name")
         if type_id:
             concept_filter_settings: ConceptFilterSettings = ConceptFilterSettings(
                 exact_name=name, concept_type_ids=[type_id]
             )
         else:
             concept_filter_settings: ConceptFilterSettings = ConceptFilterSettings(exact_name=name)
@@ -1079,22 +1110,23 @@
             with_facts=with_facts,
             with_potential_facts=with_potential_facts,
         )
         res = self._gql_client.execute(op)
         res = op + res
         return res.pagination_concept.list_concept
 
+    @prettify
     def get_concepts_by_near_name(
         self,
         name: str,
         type_id: Optional[str] = None,
         with_aliases: bool = False,
         with_facts: bool = False,
         with_potential_facts=False,
-    ) -> Sequence[Concept]:
+    ) -> Union[Sequence[Concept], Sequence[objects.Concept]]:
         op = make_operation(Query, "get_concepts_by_near_name")
         if type_id:
             concept_filter_settings: ConceptFilterSettings = ConceptFilterSettings(
                 name=name, concept_type_ids=[type_id]
             )
         else:
             concept_filter_settings: ConceptFilterSettings = ConceptFilterSettings(name=name)
@@ -1105,23 +1137,24 @@
             with_facts=with_facts,
             with_potential_facts=with_potential_facts,
         )
         res = self._gql_client.execute(op)
         res = op + res
         return res.pagination_concept.list_concept
 
+    @prettify
     def get_concepts_by_property_name(
         self,
         property_type_id: str,
         string_filter: str,
         property_type: str = "concept",
         with_aliases: bool = False,
         with_facts: bool = False,
         with_potential_facts=False,
-    ) -> Sequence[Concept]:
+    ) -> Union[Sequence[Concept], Sequence[objects.Concept]]:
         op = make_operation(Query, "get_concepts_by_property_name")
         cp: ConceptPagination = op.pagination_concept(
             filter_settings=ConceptFilterSettings(
                 property_filter_settings=[
                     PropertyFilterSettings(
                         property_type=property_type,
                         property_type_id=property_type_id,
@@ -1136,53 +1169,63 @@
             with_facts=with_facts,
             with_potential_facts=with_potential_facts,
         )
         res = self._gql_client.execute(op)
         res = op + res
         return res.pagination_concept.list_concept
 
-    def get_concept_properties(self, concept_id: str, with_facts: bool = False) -> Sequence[ConceptProperty]:
+    @prettify
+    def get_concept_properties(
+        self, concept_id: str, with_facts: bool = False
+    ) -> Union[Sequence[ConceptProperty], Sequence[objects.Property]]:
         op = make_operation(Query, "get_concept_properties")
         concept: Concept = op.concept(id=concept_id)
         pcp: ConceptPropertyPagination = concept.pagination_concept_property(
             offset=0, limit=10000, filter_settings=ConceptPropertyFilterSettings()
         )
         self._configure_output_properties_fields(pcp.list_concept_property(), with_facts)
 
         res = self._gql_client.execute(op)
         res = op + res  # type: Query
         return res.concept.pagination_concept_property.list_concept_property
 
-    def get_concept_links(self, concept_id: str, with_link_properties: bool = False) -> Sequence[ConceptLink]:
+    @prettify
+    def get_concept_links(
+        self, concept_id: str, with_link_properties: bool = False
+    ) -> Union[Sequence[ConceptLink], Sequence[objects.Link]]:
         op = make_operation(Query, "get_concept_links")
 
         concept: Concept = op.concept(id=concept_id)
         pcl: ConceptLinkPagination = concept.pagination_concept_link(
             offset=0, limit=10000, filter_settings=ConceptLinkFilterSettings()
         )
         self._configure_output_link_fields(pcl.list_concept_link(), with_link_properties=with_link_properties)
         res = self._gql_client.execute(op)
         res = op + res  # type: Query
         return res.concept.pagination_concept_link.list_concept_link
 
+    @prettify
     def get_concept_links_concept(
         self, concept_id: str, link_type_id: str, with_link_properties: bool = False
-    ) -> Sequence[ConceptLink]:
+    ) -> Union[Sequence[ConceptLink], Sequence[objects.Link]]:
         op = make_operation(Query, "get_concept_links_concept")
 
         concept = op.concept(id=concept_id)
         pcl = concept.pagination_concept_link(
             offset=0, limit=10000, filter_settings=ConceptLinkFilterSettings(concept_link_type=[link_type_id])
         )
         self._configure_output_link_fields(pcl.list_concept_link(), with_link_properties=with_link_properties)
         res = self._gql_client.execute(op)
         res = op + res  # type: Query
         return res.concept.pagination_concept_link.list_concept_link
 
-    def get_link_properties(self, link_id: str, with_facts: bool = False) -> Sequence[ConceptProperty]:
+    @prettify
+    def get_link_properties(
+        self, link_id: str, with_facts: bool = False
+    ) -> Union[Sequence[ConceptProperty], Sequence[objects.Property]]:
         op = make_operation(Query, "get_link_properties")
         concept_link: ConceptLink = op.concept_link(id=link_id)
         pcp: ConceptPropertyPagination = concept_link.pagination_concept_link_property(
             offset=0, limit=10000, filter_settings=ConceptPropertyFilterSettings()
         )
         self._configure_output_properties_fields(pcp.list_concept_property(), with_facts)
 
@@ -1240,605 +1283,743 @@
                 for time_interval in self._get_object_time_intervals(filter_settings, max_interval_size):
                     yield time_interval
         elif object_count > 0:
             yield ObjectTimeInterval(
                 start_time=start, end_time=end, object_count=object_count, max_interval_size=max_interval_size
             )
 
+    @prettify
     def create_concept(
         self,
         name: str,
         type_id: str,
         notes: Optional[str] = None,
         with_properties: bool = False,
         with_links: bool = False,
         with_link_properties: bool = False,
         perform_synchronously: Optional[bool] = None,
-    ) -> Concept:
+    ) -> Union[Concept, objects.Concept]:
         cmi: ConceptMutationInput = ConceptMutationInput(name=name, concept_type_id=type_id, notes=notes)
         return self._create_concept_with_input(
             cmi,
             with_properties=with_properties,
             with_links=with_links,
             with_link_properties=with_link_properties,
             perform_synchronously=perform_synchronously,
         )
 
-    def update_concept(
+    def _update_concept(
         self,
-        c: Concept,
-        markers: Optional[List[str]] = None,
-        notes: Optional[str] = None,
+        concept_id: str,
+        name: str,
+        concept_type_id: str,
+        markers: List[str],
+        notes: str,
+        access_level_id: str,
         perform_synchronously: Optional[bool] = None,
     ) -> Concept:
         perform_synchronously = self.get_perform_synchronously_value(perform_synchronously)
         op = make_operation(Mutation, "update_concept")
         uc: Concept = op.update_concept(
             performance_control=PerformSynchronously(perform_synchronously=perform_synchronously),
             form=ConceptUpdateInput(
-                concept_id=c.id,
-                name=c.name,
-                concept_type_id=c.concept_type.id,
-                markers=markers if markers is not None else c.markers,
-                notes=notes if notes is not None else c.notes,
-                access_level_id=c.access_level.id,
+                concept_id=concept_id,
+                name=name,
+                concept_type_id=concept_type_id,
+                markers=markers,
+                notes=notes,
+                access_level_id=access_level_id,
             ),
         )
         self._configure_output_concept_fields(uc)
         res = self._gql_client.execute(op)
         res = op + res
 
         return res.update_concept
 
-    def update_link(
+    @prettify
+    def update_concept(
         self,
-        link: ConceptLink,
+        c: Concept,
+        markers: Optional[List[str]] = None,
         notes: Optional[str] = None,
+        perform_synchronously: Optional[bool] = None,
+    ) -> Union[Concept, objects.Concept]:
+        return self._update_concept(
+            concept_id=c.id,
+            name=c.name,
+            concept_type_id=c.concept_type.id,
+            markers=markers if markers is not None else c.markers,
+            notes=notes if notes is not None else c.notes,
+            access_level_id=c.access_level.id,
+            perform_synchronously=perform_synchronously,
+        )
+
+    def _update_link(
+        self,
+        link_id: str,
+        access_level_id: str,
+        notes: str,
     ) -> ConceptLink:
         op = make_operation(Mutation, "update_link")
         ucl: Concept = op.update_concept_link(
             form=ConceptLinkUpdateMutationInput(
-                id=link.id,
-                notes=notes if notes is not None else link.notes,
-                access_level_id=link.access_level.id,
+                id=link_id,
+                notes=notes,
+                access_level_id=access_level_id,
             ),
         )
         self._configure_output_link_fields(ucl)
         res = self._gql_client.execute(op)
         res = op + res
 
         return res.update_concept_link
 
-    def update_concept_property_value_types(self, cpvt: ConceptPropertyValueType) -> ConceptPropertyValueType:
+    @prettify
+    def update_link(
+        self,
+        link: ConceptLink,
+        notes: Optional[str] = None,
+    ) -> ConceptLink:
+        return self._update_link(
+            link_id=link.id, notes=notes if notes is not None else link.notes, access_level_id=link.access_level.id
+        )
+
+    @prettify
+    def update_concept_property_value_types(
+        self, cpvt: ConceptPropertyValueType
+    ) -> Union[ConceptPropertyValueType, object_types.BaseValueType]:
         op = make_operation(Mutation, "update_concept_property_value_types")
         ucpvt = op.update_concept_property_value_type(
             form=ConceptPropertyValueTypeUpdateInput(
                 id=cpvt.id,
                 name=cpvt.name,
                 value_type=cpvt.value_type,
                 pretrained_nercmodels=cpvt.pretrained_nercmodels,
                 value_restriction=cpvt.value_restriction,
             )
         )
-        ucpvt.__fields__("id")
+        ucpvt.__fields__(*self.cpvt_fields_truncated)
         res = self._gql_client.execute(op)
         res = op + res
 
         return res.update_concept_property_value_type
 
-    def update_concept_string_property(self, cp: ConceptProperty) -> ConceptProperty:
+    @prettify
+    def update_concept_string_property(self, cp: ConceptProperty) -> Union[ConceptProperty, objects.Property]:
         op = make_operation(Mutation, "update_concept_string_property")
         ucp: ConceptProperty = op.update_concept_property(
             form=ConceptPropertyUpdateInput(
                 property_id=cp.id,
                 is_main=cp.is_main,
                 access_level_id=cp.access_level.id,
                 value_input=[
                     ComponentValueInput(value=ValueInput(string_value_input=StringValueInput(value=cp.value.value)))
                 ],
             )
         )
-        ucp.__fields__("id")
+        self._configure_output_properties_fields(ucp)
         res = self._gql_client.execute(op)
         res = op + res
 
         return res.update_concept_property
 
-    def update_concept_int_property(self, cp: ConceptProperty) -> ConceptProperty:
+    @prettify
+    def update_concept_int_property(self, cp: ConceptProperty) -> Union[ConceptProperty, objects.Property]:
         op = make_operation(Mutation, "update_concept_int_property")
         ucp: ConceptProperty = op.update_concept_property(
             form=ConceptPropertyUpdateInput(
                 property_id=cp.id,
                 is_main=cp.is_main,
                 access_level_id=cp.access_level.id,
                 value_input=[
                     ComponentValueInput(value=ValueInput(int_value_input=IntValueInput(value=cp.value.number)))
                 ],
             )
         )
-        ucp.__fields__("id")
+        self._configure_output_properties_fields(ucp)
         res = self._gql_client.execute(op)
         res = op + res
 
         return res.update_concept_property
 
-    def update_concept_composite_property(self, cp: ConceptProperty) -> ConceptProperty:
+    @prettify
+    def update_concept_composite_property(self, cp: ConceptProperty) -> Union[ConceptProperty, objects.Property]:
         op = make_operation(Mutation, "update_concept_composite_property")
         value_input = []
         for value in cp.value.list_value:
-            if type(value.value) is StringValue or type(value.value) is uas.StringValue:
+            if isinstance(value.value, (StringValue, uas.StringValue)):
                 value_input.append(
                     ComponentValueInput(
                         id=value.id, value=ValueInput(string_value_input=StringValueInput(value=value.value.value))
                     )
                 )
-            elif type(value.value) is IntValue or type(value.value) is uas.IntValue:
+            elif isinstance(value.value, (IntValue, uas.IntValue)):
                 value_input.append(
                     ComponentValueInput(
                         id=value.id, value=ValueInput(int_value_input=IntValueInput(value=value.value.number))
                     )
                 )
-            elif type(value.value) is DateTimeValue or type(value.value) is uas.DateTimeValue:
+            elif isinstance(value.value, (DateTimeValue, uas.DateTimeValue)):
                 value_input.append(
                     ComponentValueInput(
                         id=value.id,
                         value=ValueInput(
                             date_time_value_input=DateTimeValueInput(date=value.value.date, time=value.value.time)
                         ),
                     )
                 )
-            elif type(value.value) is StringLocaleValue or type(value.value) is uas.StringLocaleValue:
+            elif isinstance(value.value, (StringLocaleValue, uas.StringLocaleValue)):
                 value_input.append(
                     ComponentValueInput(
                         id=value.id,
                         value=ValueInput(
                             string_locale_value_input=StringLocaleValueInput(
                                 value=value.value.value, locale=value.value.locale
                             )
                         ),
                     )
                 )
-            elif type(value.value) is LinkValue or type(value.value) is uas.LinkValue:
+            elif isinstance(value.value, (LinkValue, uas.LinkValue)):
                 value_input.append(
                     ComponentValueInput(
                         id=value.id, value=ValueInput(link_value_input=LinkValueInput(link=value.value.link))
                     )
                 )
-            elif type(value.value) is DoubleValue or type(value.value) is uas.DoubleValue:
+            elif isinstance(value.value, (DoubleValue, uas.DoubleValue)):
                 value_input.append(
                     ComponentValueInput(
                         id=value.id, value=ValueInput(double_value_input=DoubleValueInput(double=value.value.double))
                     )
                 )
         ucp: ConceptProperty = op.update_concept_property(
             form=ConceptPropertyUpdateInput(
                 property_id=cp.id, is_main=cp.is_main, access_level_id=cp.access_level.id, value_input=value_input
             )
         )
-        ucp.__fields__("id")
+        self._configure_output_properties_fields(ucp)
+        res = self._gql_client.execute(op)
+        res = op + res
+
+        return res.update_concept_property
+
+    def _update_concept_property_with_input(
+        self,
+        property_id: str,
+        is_main: bool,
+        value_input: List[ComponentValueInput],
+        access_level_id: str,
+    ) -> ConceptProperty:
+        op = make_operation(Mutation, "update_concept_property_with_input")
+        ucp: ConceptProperty = op.update_concept_property(
+            form=ConceptPropertyUpdateInput(
+                property_id=property_id,
+                is_main=is_main,
+                value_input=value_input,
+                access_level_id=access_level_id,
+            )
+        )
+        self._configure_output_properties_fields(ucp)
         res = self._gql_client.execute(op)
         res = op + res
 
         return res.update_concept_property
 
+    @prettify
+    def update_concept_property_with_input(
+        self,
+        concept_property: ConceptProperty,
+        value_input: List[ComponentValueInput],
+    ) -> Union[ConceptProperty, objects.Property]:
+        return self._update_concept_property_with_input(
+            property_id=concept_property.id,
+            is_main=concept_property.is_main,
+            value_input=value_input,
+            access_level_id=concept_property.access_level.id,
+        )
+
     def delete_concept_property(self, cp_id: str) -> bool:
         op = make_operation(Mutation, "delete_concept_property")
         dcp = op.delete_concept_property(id=cp_id)
         dcp.__fields__("is_success")
         res = self._gql_client.execute(op)
         res = op + res
 
         return res.delete_concept_property.is_success
 
+    @prettify
     def get_all_concept_types(
         self,
         filter_settings: Optional[ConceptTypeFilterSettings] = None,
         direction: SortDirection = "ascending",
         sort_field: ConceptTypeSorting = "id",
-    ) -> Iterable[ConceptType]:
+    ) -> Union[Iterable[ConceptType], Iterable[object_types.ConceptType]]:
         current_step = 0
         while True:
             concept_types = self.get_concept_types(
                 skip=current_step,
                 take=self.limit,
                 filter_settings=filter_settings,
                 direction=direction,
                 sort_field=sort_field,
             )
             if len(concept_types) < 1:
                 break
             current_step += self.limit
             yield from concept_types
 
+    @prettify
     def get_concept_types(
         self,
         skip: int = 0,
         take: Optional[int] = None,
         filter_settings: Optional[ConceptTypeFilterSettings] = None,
         direction: SortDirection = "ascending",
         sort_field: ConceptTypeSorting = "id",
-    ) -> Sequence[ConceptType]:
+    ) -> Union[Sequence[ConceptType], Sequence[object_types.ConceptType]]:
         op = make_operation(Query, "get_concept_types")
         take = self.get_take_value(take)
         if not filter_settings:
             filter_settings = ConceptTypeFilterSettings()
         pct: ConceptTypePagination = op.pagination_concept_type(
             direction=direction, filter_settings=filter_settings, limit=take, offset=skip, sort_field=sort_field
         )
         pct.list_concept_type().__fields__(*self.concept_type_fields)
         res = self._gql_client.execute(op)
         res = op + res
         return res.pagination_concept_type.list_concept_type
 
-    def get_concept_types_by_name(self, name: str) -> Sequence[ConceptType]:
+    def _get_concept_types_by_name(self, name: str) -> Sequence[ConceptType]:
         op = make_operation(Query, "get_concept_types_by_name")
         ctp: ConceptTypePagination = op.pagination_concept_type(filter_settings=ConceptTypeFilterSettings(name=name))
         ctp.list_concept_type().__fields__(*self.concept_type_fields)
         res = self._gql_client.execute(op)
         res = op + res
         return res.pagination_concept_type.list_concept_type
 
-    def get_concept_type_info(self, concept_type_id: str) -> ConceptType:
+    @prettify
+    def get_concept_types_by_name(self, name: str) -> Union[Sequence[ConceptType], Sequence[object_types.ConceptType]]:
+        return self._get_concept_types_by_name(name)
+
+    @prettify
+    def get_concept_type_info(self, concept_type_id: str) -> Union[ConceptType, object_types.ConceptType]:
         op = make_operation(Query, "get_concept_type_info")
         ct = op.concept_type(id=concept_type_id)
         ct.__fields__(*self.concept_type_fields)
         lcpt = ct.list_concept_property_type()
         lcpt.__fields__(*self.concept_property_type_fields)
         lclt = ct.list_concept_link_type()
         lclt.__fields__(*self.concept_link_type_fields)
         lclt.list_concept_link_property_type().__fields__(*self.concept_property_type_fields)
 
         res = self._gql_client.execute(op)
         res = op + res
         return res.concept_type
 
-    def get_concept_type(self, concept_type_code: str) -> Optional[ConceptType]:
+    def _get_concept_type(self, concept_type_code: str) -> Optional[ConceptType]:
         concept_type = self._type_mapping.get_concept_type(concept_type_code)
         if concept_type:
             return concept_type
 
         concept_type_name = self._type_mapping.get_concept_type_name(concept_type_code)
-        concept_types = self.get_concept_types_by_name(concept_type_name)
+        concept_types = self._get_concept_types_by_name(concept_type_name)
         for concept_type in concept_types:
             if concept_type.name == concept_type_name:
                 self._type_mapping.add_concept_type(concept_type_code, concept_type)
                 return concept_type
         return None
 
+    @prettify
+    def get_concept_type(self, concept_type_code: str) -> Union[ConceptType, object_types.ConceptType, None]:
+        return self._get_concept_type(concept_type_code)
+
+    @prettify
     def get_all_concept_property_types(
         self,
         filter_settings: Optional[ConceptPropertyTypeFilterSettings] = None,
         direction: SortDirection = "ascending",
         sort_field: ConceptPropertyTypeSorting = "name",
-    ) -> Iterable[ConceptPropertyType]:
+    ) -> Union[Iterable[ConceptPropertyType], Iterable[object_types.PropertyType]]:
         current_step = 0
         while True:
             concept_property_types = self.get_concept_property_types(
                 skip=current_step,
                 take=self.limit,
                 filter_settings=filter_settings,
                 direction=direction,
                 sort_field=sort_field,
             )
             if len(concept_property_types) < 1:
                 break
             current_step += self.limit
             yield from concept_property_types
 
+    @prettify
     def get_concept_property_types(
         self,
         skip: int = 0,
         take: Optional[int] = None,
         filter_settings: Optional[ConceptPropertyTypeFilterSettings] = None,
         direction: SortDirection = "ascending",
         sort_field: ConceptPropertyTypeSorting = "name",
-    ) -> Sequence[ConceptPropertyType]:
+    ) -> Union[Sequence[ConceptPropertyType], Sequence[object_types.PropertyType]]:
         op = make_operation(Query, "get_concept_property_types")
         take = self.get_take_value(take)
         if not filter_settings:
             filter_settings = ConceptPropertyTypeFilterSettings()
         pcpt: ConceptPropertyTypePagination = op.pagination_concept_property_type(
             direction=direction, filter_settings=filter_settings, limit=take, offset=skip, sort_field=sort_field
         )
         lcpt = pcpt.list_concept_property_type()
         lcpt.__fields__(*self.concept_property_type_fields)
         self._configure_property_value_type_fields(lcpt.value_type, True)
         res = self._gql_client.execute(op)
         res = op + res
         return res.pagination_concept_property_type.list_concept_property_type
 
-    def get_concept_properties_types_by_name(
+    def _get_concept_properties_types_by_name(
         self, concept_type_id: str, prop_name: str
     ) -> Sequence[ConceptPropertyType]:
         op = make_operation(Query, "get_concept_properties_types_by_name")
         cptp: ConceptPropertyTypePagination = op.pagination_concept_property_type(
             filter_settings=ConceptPropertyTypeFilterSettings(name=prop_name, concept_type_id=concept_type_id)
         )
         lcpt = cptp.list_concept_property_type()
         lcpt.__fields__(*self.concept_property_type_fields)
         self._configure_property_value_type_fields(lcpt.value_type, True)
         res = self._gql_client.execute(op)
         res = op + res
         return res.pagination_concept_property_type.list_concept_property_type
 
+    @prettify
+    def get_concept_properties_types_by_name(
+        self, concept_type_id: str, prop_name: str
+    ) -> Union[Sequence[ConceptPropertyType], Sequence[object_types.PropertyType]]:
+        return self._get_concept_properties_types_by_name(concept_type_id, prop_name)
+
+    @prettify
     def get_all_concept_composite_property_types(
         self,
         filter_settings: Optional[CompositePropertyTypeFilterSettings] = None,
         direction: SortDirection = "ascending",
         sort_field: CompositePropertyTypeSorting = "name",
-    ) -> Iterable[ConceptPropertyType]:
+    ) -> Union[Iterable[ConceptPropertyType], Iterable[object_types.PropertyType]]:
         current_step = 0
         while True:
             concept_composite_property_types = self.get_concept_composite_property_types(
                 skip=current_step,
                 take=self.limit,
                 filter_settings=filter_settings,
                 direction=direction,
                 sort_field=sort_field,
             )
             if len(concept_composite_property_types) < 1:
                 break
             current_step += self.limit
             yield from concept_composite_property_types
 
+    @prettify
     def get_concept_composite_property_types(
         self,
         skip: int = 0,
         take: Optional[int] = None,
         filter_settings: Optional[CompositePropertyTypeFilterSettings] = None,
         direction: SortDirection = "ascending",
         sort_field: CompositePropertyTypeSorting = "name",
-    ) -> Sequence[ConceptPropertyType]:
+    ) -> Union[Sequence[ConceptPropertyType], Sequence[object_types.PropertyType]]:
         op = make_operation(Query, "get_concept_composite_property_types")
         take = self.get_take_value(take)
         if not filter_settings:
             filter_settings = CompositePropertyTypeFilterSettings()
         pccpt: ConceptPropertyTypePagination = op.pagination_composite_concept_property_type(
             direction=direction, filter_settings=filter_settings, limit=take, offset=skip, sort_field=sort_field
         )
         lcpt = pccpt.list_concept_property_type()
         lcpt.__fields__(*self.concept_property_type_fields)
         self._configure_property_value_type_fields(lcpt.value_type, True)
         res = self._gql_client.execute(op)
         res = op + res
         return res.pagination_composite_concept_property_type.list_concept_property_type
 
-    def get_concept_property_type(
+    def _get_concept_property_type(
         self, concept_type_code: str, property_type_code: str
     ) -> Optional[ConceptPropertyType]:
         property_type = self._type_mapping.get_concept_property_type(concept_type_code, property_type_code)
         if property_type:
             return property_type
 
-        concept_type = self.get_concept_type(concept_type_code)
+        concept_type = self._get_concept_type(concept_type_code)
         if not concept_type:
             raise Exception("Cannot get concept property type: no concept type id")
 
         property_type_name = self._type_mapping.get_concept_property_type_name(concept_type_code, property_type_code)
-        property_types = self.get_concept_properties_types_by_name(concept_type.id, property_type_name)
+        property_types = self._get_concept_properties_types_by_name(concept_type.id, property_type_name)
         for property_type in property_types:
             if property_type.name == property_type_name:
                 self._type_mapping.add_concept_property_type(concept_type_code, property_type_code, property_type)
                 return property_type
         return None
 
+    @prettify
+    def get_concept_property_type(
+        self, concept_type_code: str, property_type_code: str
+    ) -> Union[ConceptPropertyType, object_types.PropertyType, None]:
+        return self._get_concept_property_type(concept_type_code, property_type_code)
+
+    @prettify
     def get_all_concept_property_value_types(
         self,
         filter_settings: Optional[ConceptPropertyValueTypeFilterSettings] = None,
         direction: SortDirection = "ascending",
         sort_field: ConceptPropertyValueTypeSorting = "id",
-    ) -> Iterable[ConceptPropertyValueType]:
+    ) -> Union[Iterable[ConceptPropertyValueType], Iterable[object_types.BaseValueType]]:
         current_step = 0
         while True:
             concept_property_value_types = self.get_concept_property_value_types(
                 skip=current_step,
                 take=self.limit,
                 filter_settings=filter_settings,
                 direction=direction,
                 sort_field=sort_field,
             )
             if len(concept_property_value_types) < 1:
                 break
             current_step += self.limit
             yield from concept_property_value_types
 
+    @prettify
     def get_concept_property_value_types(
         self,
         skip: int = 0,
         take: Optional[int] = None,
         filter_settings: Optional[ConceptPropertyValueTypeFilterSettings] = None,
         direction: SortDirection = "ascending",
         sort_field: ConceptPropertyValueTypeSorting = "id",
-    ) -> Sequence[ConceptPropertyValueType]:
+    ) -> Union[Sequence[ConceptPropertyValueType], Sequence[object_types.BaseValueType]]:
         op = make_operation(Query, "get_concept_property_value_types")
         take = self.get_take_value(take)
         if not filter_settings:
             filter_settings = ConceptPropertyValueTypeFilterSettings()
         pcpvt: ConceptPropertyValueTypePagination = op.pagination_concept_property_value_type(
             direction=direction, filter_settings=filter_settings, limit=take, offset=skip, sort_field=sort_field
         )
         pcpvt.list_concept_property_value_type().__fields__(*self.cpvt_fields)
         res = self._gql_client.execute(op)
         res = op + res
         return res.pagination_concept_property_value_type.list_concept_property_value_type
 
-    def get_concept_property_value_types_by_name(
+    def _get_concept_property_value_types_by_name(
         self, prop_value_type_name: str, limit: int = 20, offset: int = 0
     ) -> Sequence[ConceptPropertyValueType]:
         op = make_operation(Query, "get_concept_property_value_types_by_name")
         cpvtp: ConceptPropertyValueTypePagination = op.pagination_concept_property_value_type(
             filter_settings=ConceptPropertyValueTypeFilterSettings(name=prop_value_type_name),
             limit=limit,
             offset=offset,
         )
         cpvtp.list_concept_property_value_type().__fields__(*self.cpvt_fields)
         res = self._gql_client.execute(op)
         res = op + res
         return res.pagination_concept_property_value_type.list_concept_property_value_type
 
+    @prettify
+    def get_concept_property_value_types_by_name(
+        self, prop_value_type_name: str, limit: int = 20, offset: int = 0
+    ) -> Union[Sequence[ConceptPropertyValueType], Sequence[object_types.BaseValueType]]:
+        return self._get_concept_property_value_types_by_name(prop_value_type_name, limit, offset)
+
+    @prettify
     def get_concept_property_value_type(
         self, concept_property_value_type_code: str
-    ) -> Optional[ConceptPropertyValueType]:
+    ) -> Union[ConceptPropertyValueType, object_types.BaseValueType, None]:
         property_value_type = self._type_mapping.get_concept_property_value_type(concept_property_value_type_code)
         if property_value_type:
             return property_value_type
 
         value_type_name = self._type_mapping.get_concept_property_value_type_name(concept_property_value_type_code)
-        value_types = self.get_concept_property_value_types_by_name(value_type_name)
+        value_types = self._get_concept_property_value_types_by_name(value_type_name)
         for value_type in value_types:
             if value_type.name == value_type_name:
                 self._type_mapping.add_concept_property_value_type(concept_property_value_type_code, value_type)
                 return value_type
         return None
 
+    @prettify
     def get_all_concept_link_property_types(
         self,
         filter_settings: Optional[ConceptPropertyTypeFilterSettings] = None,
         direction: SortDirection = "ascending",
         sort_field: ConceptPropertyTypeSorting = "name",
-    ) -> Iterable[ConceptPropertyType]:
+    ) -> Union[Iterable[ConceptPropertyType], Iterable[object_types.PropertyType]]:
         current_step = 0
         while True:
             concept_link_property_types = self.get_link_property_types(
                 skip=current_step,
                 take=self.limit,
                 filter_settings=filter_settings,
                 direction=direction,
                 sort_field=sort_field,
             )
             if len(concept_link_property_types) < 1:
                 break
             current_step += self.limit
             yield from concept_link_property_types
 
+    @prettify
     def get_link_property_types(
         self,
         skip: int = 0,
         take: Optional[int] = None,
         filter_settings: Optional[ConceptPropertyTypeFilterSettings] = None,
         direction: SortDirection = "ascending",
         sort_field: ConceptPropertyTypeSorting = "name",
-    ) -> Sequence[ConceptPropertyType]:
+    ) -> Union[Sequence[ConceptPropertyType], Sequence[object_types.PropertyType]]:
         op = make_operation(Query, "get_link_property_types")
         take = self.get_take_value(take)
         if not filter_settings:
             filter_settings = ConceptPropertyTypeFilterSettings()
         pclpt: ConceptPropertyTypePagination = op.pagination_concept_link_property_type(
             direction=direction, filter_settings=filter_settings, limit=take, offset=skip, sort_field=sort_field
         )
         lcpt = pclpt.list_concept_property_type()
         lcpt.__fields__(*self.concept_property_type_fields)
         self._configure_property_value_type_fields(lcpt.value_type, True)
         res = self._gql_client.execute(op)
         res = op + res
         return res.pagination_concept_link_property_type.list_concept_property_type
 
-    def get_link_properties_types_by_name(self, link_type_id: str, prop_name: str) -> Sequence[ConceptPropertyType]:
-        op = make_operation(Query, "get_link_properties_types_by_name")
+    def _get_link_properties_types_by_name(self, link_type_id: str, prop_name: str) -> Sequence[ConceptPropertyType]:
+        op = make_operation(Query, "_get_link_properties_types_by_name")
         cptp: ConceptPropertyTypePagination = op.pagination_concept_link_property_type(
             filter_settings=ConceptPropertyTypeFilterSettings(name=prop_name, concept_link_type_id=link_type_id)
         )
         lcpt = cptp.list_concept_property_type()
         lcpt.__fields__(*self.concept_property_type_fields)
         self._configure_property_value_type_fields(lcpt.value_type, True)
         res = self._gql_client.execute(op)
         res = op + res
         return res.pagination_concept_link_property_type.list_concept_property_type
 
+    @prettify
+    def get_link_properties_types_by_name(
+        self, link_type_id: str, prop_name: str
+    ) -> Union[Sequence[ConceptPropertyType], Sequence[object_types.PropertyType]]:
+        return self._get_link_properties_types_by_name(link_type_id, prop_name)
+
+    @prettify
     def get_all_concept_link_composite_property_types(
         self,
         filter_settings: Optional[CompositePropertyTypeFilterSettings] = None,
         direction: SortDirection = "ascending",
         sort_field: CompositePropertyTypeSorting = "name",
-    ) -> Iterable[ConceptPropertyType]:
+    ) -> Union[Iterable[ConceptPropertyType], Iterable[object_types.PropertyType]]:
         current_step = 0
         while True:
             concept_link_composite_property_types = self.get_link_composite_property_types(
                 skip=current_step,
                 take=self.limit,
                 filter_settings=filter_settings,
                 direction=direction,
                 sort_field=sort_field,
             )
             if len(concept_link_composite_property_types) < 1:
                 break
             current_step += self.limit
             yield from concept_link_composite_property_types
 
+    @prettify
     def get_link_composite_property_types(
         self,
         skip: int = 0,
         take: Optional[int] = None,
         filter_settings: Optional[CompositePropertyTypeFilterSettings] = None,
         direction: SortDirection = "ascending",
         sort_field: CompositePropertyTypeSorting = "name",
-    ) -> Sequence[ConceptPropertyType]:
+    ) -> Union[Sequence[ConceptPropertyType], Sequence[object_types.PropertyType]]:
         op = make_operation(Query, "get_link_composite_property_types")
         take = self.get_take_value(take)
         if not filter_settings:
             filter_settings = CompositePropertyTypeFilterSettings()
         pclpt: ConceptPropertyTypePagination = op.pagination_composite_link_property_type(
             direction=direction, filter_settings=filter_settings, limit=take, offset=skip, sort_field=sort_field
         )
         lcpt = pclpt.list_concept_property_type()
         lcpt.__fields__(*self.concept_property_type_fields)
         self._configure_property_value_type_fields(lcpt.value_type, True)
         res = self._gql_client.execute(op)
         res = op + res
         return res.pagination_composite_link_property_type.list_concept_property_type
 
-    def get_composite_link_properties_types_by_name(
+    def _get_composite_link_properties_types_by_name(
         self, link_type_id: str, prop_name: str
     ) -> Sequence[ConceptPropertyType]:
         op = make_operation(Query, "get_composite_link_properties_types_by_name")
         cptp: ConceptPropertyTypePagination = op.pagination_composite_link_property_type(
             filter_settings=CompositePropertyTypeFilterSettings(name=prop_name, link_type_id=link_type_id)
         )
         lcpt = cptp.list_concept_property_type()
         lcpt.__fields__(*self.concept_property_type_fields)
         self._configure_property_value_type_fields(lcpt.value_type, True)
         res = self._gql_client.execute(op)
         res = op + res
         return res.pagination_composite_link_property_type.list_concept_property_type
 
-    def get_link_property_type(self, link_type_code: str, property_type_code: str) -> Optional[ConceptPropertyType]:
+    @prettify
+    def get_composite_link_properties_types_by_name(
+        self, link_type_id: str, prop_name: str
+    ) -> Union[Sequence[ConceptPropertyType], Sequence[object_types.PropertyType]]:
+        return self._get_composite_link_properties_types_by_name(link_type_id, prop_name)
+
+    def _get_link_property_type(self, link_type_code: str, property_type_code: str) -> Optional[ConceptPropertyType]:
         property_type = self._type_mapping.get_concept_link_property_type(link_type_code, property_type_code)
         if property_type:
             return property_type
-        link_type = self.get_link_type(link_type_code)
+        link_type = self._get_link_type(link_type_code)
 
         property_type_name = self._type_mapping.get_concept_link_property_type_name(link_type_code, property_type_code)
-        property_types = self.get_link_properties_types_by_name(link_type.id, property_type_name)
+        property_types = self._get_link_properties_types_by_name(link_type.id, property_type_name)
         for property_type in property_types:
             if property_type.name == property_type_name:
                 self._type_mapping.add_concept_link_property_type(link_type_code, property_type_code, property_type)
                 return property_type
         return None
 
-    def get_link_composite_property_type(
+    @prettify
+    def get_link_property_type(
+        self, link_type_code: str, property_type_code: str
+    ) -> Union[ConceptPropertyType, object_types.PropertyType, None]:
+        return self._get_link_property_type(link_type_code, property_type_code)
+
+    def _get_link_composite_property_type(
         self, link_type_code: str, property_type_code: str
     ) -> Optional[ConceptPropertyType]:
         property_type = self._type_mapping.get_concept_link_composite_property_type(link_type_code, property_type_code)
         if property_type:
             return property_type
-        link_type = self.get_link_type(link_type_code)
+        link_type = self._get_link_type(link_type_code)
 
         property_type_name = self._type_mapping.get_concept_link_composite_property_type_name(
             link_type_code, property_type_code
         )
-        property_types = self.get_composite_link_properties_types_by_name(link_type.id, property_type_name)
+        property_types = self._get_composite_link_properties_types_by_name(link_type.id, property_type_name)
         for property_type in property_types:
             if property_type.name == property_type_name:
                 self._type_mapping.add_concept_link_composite_property_type(
                     link_type_code, property_type_code, property_type
                 )
                 return property_type
         return None
 
-    def add_property_by_id(
+    @prettify
+    def get_link_composite_property_type(
+        self, link_type_code: str, property_type_code: str
+    ) -> Union[ConceptPropertyType, object_types.PropertyType, None]:
+        return self._get_link_composite_property_type(link_type_code, property_type_code)
+
+    def _add_property_by_id(
         self,
         id: str,
         type_id: str,
         value: Any,
         is_main: bool,
         value_type: str,
         perform_synchronously: Optional[bool] = None,
@@ -1851,53 +2032,109 @@
             form=ConceptPropertyCreateInput(
                 concept_id=id,
                 property_type_id=type_id,
                 is_main=is_main,
                 value_input=[ComponentValueInput(value=get_map_helper(value_type).get_value_input(value))],
             ),
         )
-        acp.__fields__("id")
-        acp.property_type().__fields__(*self.concept_property_type_fields)
+        self._configure_output_properties_fields(acp)
         res = self._gql_client.execute(op)
         res = op + res
 
         return res.add_concept_property
 
-    def add_property(
+    @prettify
+    def add_property_by_id(
+        self,
+        id: str,
+        type_id: str,
+        value: Any,
+        is_main: bool,
+        value_type: str,
+        perform_synchronously: Optional[bool] = None,
+    ) -> Union[ConceptProperty, objects.Property]:
+        return self._add_property_by_id(id, type_id, value, is_main, value_type, perform_synchronously)
+
+    def _add_concept_property_with_input_by_id(
+        self,
+        concept_id: str,
+        property_type_id: str,
+        value_input: List[ComponentValueInput],
+        is_main: bool,
+        perform_synchronously: Optional[bool] = None,
+    ) -> ConceptProperty:
+        op = make_operation(Mutation, "_add_property_with_input_by_id")
+        acp = op.add_concept_property(
+            performance_control=PerformSynchronously(
+                perform_synchronously=self.get_perform_synchronously_value(perform_synchronously)
+            ),
+            form=ConceptPropertyCreateInput(
+                concept_id=concept_id,
+                property_type_id=property_type_id,
+                is_main=is_main,
+                value_input=value_input,
+            ),
+        )
+        self._configure_output_properties_fields(acp)
+        res = self._gql_client.execute(op)
+        res = op + res
+
+        return res.add_concept_property
+
+    def _add_property(
         self,
         concept_id: str,
         concept_type_code: str,
         property_type_code: str,
         value: Any,
         is_main: bool = False,
         perform_synchronously: Optional[bool] = None,
     ) -> ConceptProperty:
-        property_type: ConceptPropertyType = self.get_concept_property_type(concept_type_code, property_type_code)
+        property_type: ConceptPropertyType = self._get_concept_property_type(concept_type_code, property_type_code)
         if not property_type:
             raise Exception("Cannot add property: no property type id")
-        if type(property_type.value_type) is CompositePropertyValueTemplate:
+        if isinstance(property_type.value_type, (CompositePropertyValueTemplate, uas.CompositePropertyValueTemplate)):
             component_values = self._type_mapping.get_concept_composite_property_component_values(
                 concept_type_code, property_type_code
             )
             components_type_mapping: Dict[str, CompositePropertyValueType] = self._get_components_mapping(
                 component_values, property_type.value_type.component_value_types
             )
-            prop = self.add_composite_property_by_id(
+            prop = self._add_composite_property_by_id(
                 concept_id, property_type.id, value, is_main, components_type_mapping, perform_synchronously
             )
         else:
-            prop = self.add_property_by_id(
+            prop = self._add_property_by_id(
                 concept_id, property_type.id, value, is_main, property_type.value_type.value_type, perform_synchronously
             )
         if self.tdm_builder is not None:
-            self.tdm_builder.add_concept_property_fact(prop, self.get_concept(concept_id), value, property_type)
+            self.tdm_builder.add_concept_property_fact(prop, self._get_concept(concept_id), value, property_type)
 
         return prop
 
-    def add_link_property_by_id(
+    @prettify
+    def add_property(
+        self,
+        concept_id: str,
+        concept_type_code: str,
+        property_type_code: str,
+        value: Any,
+        is_main: bool = False,
+        perform_synchronously: Optional[bool] = None,
+    ) -> Union[ConceptProperty, objects.Property]:
+        return self._add_property(
+            concept_id=concept_id,
+            concept_type_code=concept_type_code,
+            property_type_code=property_type_code,
+            value=value,
+            is_main=is_main,
+            perform_synchronously=perform_synchronously,
+        )
+
+    def _add_link_property_by_id(
         self,
         link_id: str,
         type_id: str,
         value: str,
         is_main: bool,
         value_type: str,
         perform_synchronously: Optional[bool] = None,
@@ -1910,39 +2147,54 @@
             form=ConceptLinkPropertyInput(
                 property_type_id=type_id,
                 link_id=link_id,
                 is_main=is_main,
                 value_input=[ComponentValueInput(value=get_map_helper(value_type).get_value_input(value))],
             ),
         )
-        aclp.__fields__("id")
-        aclp.property_type().__fields__(*self.concept_property_type_fields)
+        self._configure_output_properties_fields(aclp)
         res = self._gql_client.execute(op)
         res = op + res
 
         return res.add_concept_link_property
 
-    def add_concept_link_property_type(self, link_type_id: str, name: str, value_type_id: str) -> ConceptPropertyType:
+    @prettify
+    def add_link_property_by_id(
+        self,
+        link_id: str,
+        type_id: str,
+        value: str,
+        is_main: bool,
+        value_type: str,
+        perform_synchronously: Optional[bool] = None,
+    ) -> Union[ConceptProperty, objects.Property]:
+        return self._add_link_property_by_id(link_id, type_id, value, is_main, value_type, perform_synchronously)
+
+    @prettify
+    def add_concept_link_property_type(
+        self, link_type_id: str, name: str, value_type_id: str
+    ) -> Union[ConceptPropertyType, object_types.PropertyType]:
         op = make_operation(Mutation, "add_concept_link_property_type")
         aclpt = op.add_concept_link_property_type(
             form=ConceptLinkPropertyTypeCreationInput(
                 link_type_id=link_type_id,
                 name=name,
                 value_type_id=value_type_id,
             )
         )
         aclpt.__fields__(*self.concept_property_type_fields)
         res = self._gql_client.execute(op)
         res = op + res
 
         return res.add_concept_link_property_type
 
+    @prettify
     def update_concept_link_property_type(
         self, link_property_type_id: str, name: str, value_type_id: str
-    ) -> ConceptPropertyType:
+    ) -> Union[ConceptPropertyType, object_types.PropertyType]:
         op = make_operation(Mutation, "update_concept_link_property_type")
         acpt = op.update_concept_link_property_type(
             form=ConceptLinkPropertyTypeUpdateInput(
                 id=link_property_type_id,
                 name=name,
                 value_type_id=value_type_id,
             )
@@ -1957,15 +2209,18 @@
         op = make_operation(Mutation, "delete_concept_link_property_type")
         op.delete_concept_link_property_type(id=property_type_id)
         res = self._gql_client.execute(op)
         res = op + res
 
         return res.delete_concept_link_property_type
 
-    def add_concept_property_type(self, concept_type_id: str, name: str, value_type_id: str) -> ConceptPropertyType:
+    @prettify
+    def add_concept_property_type(
+        self, concept_type_id: str, name: str, value_type_id: str
+    ) -> Union[ConceptPropertyType, object_types.PropertyType]:
         op = make_operation(Mutation, "add_concept_property_type")
         acpt = op.add_concept_property_type(
             form=ConceptPropertyTypeCreationInput(
                 concept_type_id=concept_type_id,
                 name=name,
                 value_type_id=value_type_id,
             )
@@ -1980,15 +2235,15 @@
         op = make_operation(Mutation, "delete_concept_property_type")
         op.delete_concept_property_type(id=property_type_id)
         res = self._gql_client.execute(op)
         res = op + res
 
         return res.delete_concept_property_type
 
-    def add_link_composite_property_by_id(
+    def _add_link_composite_property_by_id(
         self,
         link_id: str,
         property_type_id: str,
         values: dict,
         components_type_mapping: Dict[str, CompositePropertyValueType],
         is_main: bool,
         perform_synchronously: Optional[bool] = None,
@@ -2001,22 +2256,35 @@
             form=ConceptLinkPropertyInput(
                 property_type_id=property_type_id,
                 link_id=link_id,
                 is_main=is_main,
                 value_input=self._get_value_input(values, components_type_mapping),
             ),
         )
-        aclp.__fields__("id")
-        aclp.property_type().__fields__(*self.concept_property_type_fields)
+        self._configure_output_properties_fields(aclp)
         res = self._gql_client.execute(op)
         res = op + res
 
         return res.add_concept_link_property
 
-    def add_composite_property_by_id(
+    @prettify
+    def add_link_composite_property_by_id(
+        self,
+        link_id: str,
+        property_type_id: str,
+        values: dict,
+        components_type_mapping: Dict[str, CompositePropertyValueType],
+        is_main: bool,
+        perform_synchronously: Optional[bool] = None,
+    ) -> Union[ConceptProperty, objects.Property]:
+        return self._add_link_composite_property_by_id(
+            link_id, property_type_id, values, components_type_mapping, is_main, perform_synchronously
+        )
+
+    def _add_composite_property_by_id(
         self,
         id: str,
         type_id: str,
         values: dict,
         is_main: bool,
         components_type_mapping: Dict[str, CompositePropertyValueType],
         perform_synchronously: Optional[bool] = None,
@@ -2029,98 +2297,162 @@
             form=ConceptPropertyCreateInput(
                 concept_id=id,
                 property_type_id=type_id,
                 is_main=is_main,
                 value_input=self._get_value_input(values, components_type_mapping),
             ),
         )
-        acp.__fields__("id")
-        acp.property_type().__fields__(*self.concept_property_type_fields)
+        self._configure_output_properties_fields(acp)
         res = self._gql_client.execute(op)
         res = op + res
 
         return res.add_concept_property
 
-    def add_link_property(
+    @prettify
+    def add_composite_property_by_id(
+        self,
+        id: str,
+        type_id: str,
+        values: dict,
+        is_main: bool,
+        components_type_mapping: Dict[str, CompositePropertyValueType],
+        perform_synchronously: Optional[bool] = None,
+    ) -> Union[ConceptProperty, objects.Property]:
+        return self._add_composite_property_by_id(
+            id, type_id, values, is_main, components_type_mapping, perform_synchronously
+        )
+
+    def _add_link_property_with_input_by_id(
+        self,
+        link_id: str,
+        property_type_id: str,
+        value_input: List[ComponentValueInput],
+        is_main: bool,
+        perform_synchronously: Optional[bool] = None,
+    ) -> ConceptProperty:
+        op = make_operation(Mutation, "_add_link_property_with_input_by_id")
+        aclp = op.add_concept_link_property(
+            performance_control=PerformSynchronously(
+                perform_synchronously=self.get_perform_synchronously_value(perform_synchronously)
+            ),
+            form=ConceptLinkPropertyInput(
+                property_type_id=property_type_id,
+                link_id=link_id,
+                is_main=is_main,
+                value_input=value_input,
+            ),
+        )
+        self._configure_output_properties_fields(aclp)
+        res = self._gql_client.execute(op)
+        res = op + res
+
+        return res.add_concept_link_property
+
+    def _add_link_property(
         self,
         link_id: str,
         link_type_code: str,
         property_type_code: str,
         value: Any,
         is_composite: Optional[bool] = False,
         is_main: bool = False,
         perform_synchronously: Optional[bool] = None,
     ) -> ConceptProperty:
         property_type = (
-            self.get_link_composite_property_type(link_type_code, property_type_code)
+            self._get_link_composite_property_type(link_type_code, property_type_code)
             if is_composite
-            else self.get_link_property_type(link_type_code, property_type_code)
+            else self._get_link_property_type(link_type_code, property_type_code)
         )
         if not property_type:
             raise Exception("Cannot add property: no property type id")
 
         if is_composite:
             component_values = self._type_mapping.get_concept_link_composite_property_component_values(
                 link_type_code, property_type_code
             )
             components_type_mapping: Dict[str, CompositePropertyValueType] = self._get_components_mapping(
                 component_values, property_type.value_type.component_value_types
             )
 
-            link_property = self.add_link_composite_property_by_id(
+            link_property = self._add_link_composite_property_by_id(
                 link_id,
                 property_type.id,
                 value,
                 components_type_mapping,
                 is_main,
                 perform_synchronously,
             )
         else:
-            link_property = self.add_link_property_by_id(
+            link_property = self._add_link_property_by_id(
                 link_id,
                 property_type.id,
                 value,
                 is_main,
                 property_type.value_type.value_type,
                 perform_synchronously,
             )
 
         if self.tdm_builder is not None:
-            self.tdm_builder.add_link_property_fact(link_property, self.get_concept_link(link_id), value, property_type)
+            self.tdm_builder.add_link_property_fact(
+                link_property, self._get_concept_link(link_id), value, property_type
+            )
 
         return link_property
 
+    @prettify
+    def add_link_property(
+        self,
+        link_id: str,
+        link_type_code: str,
+        property_type_code: str,
+        value: Any,
+        is_composite: Optional[bool] = False,
+        is_main: bool = False,
+        perform_synchronously: Optional[bool] = None,
+    ) -> Union[ConceptProperty, objects.Property]:
+        return self._add_link_property(
+            link_id=link_id,
+            link_type_code=link_type_code,
+            property_type_code=property_type_code,
+            value=value,
+            is_composite=is_composite,
+            is_main=is_main,
+            perform_synchronously=perform_synchronously,
+        )
+
+    @prettify
     def get_all_concept_link_types(
         self,
         filter_settings: Optional[ConceptLinkTypeFilterSettings] = None,
         direction: SortDirection = "ascending",
         sort_field: ConceptLinkTypeSorting = "id",
-    ) -> Iterable[ConceptLinkType]:
+    ) -> Union[Iterable[ConceptLinkType], Iterable[object_types.LinkType]]:
         current_step = 0
         while True:
             concept_link_types = self.get_concept_link_types(
                 skip=current_step,
                 take=self.limit,
                 filter_settings=filter_settings,
                 direction=direction,
                 sort_field=sort_field,
             )
             if len(concept_link_types) < 1:
                 break
             current_step += self.limit
             yield from concept_link_types
 
+    @prettify
     def get_concept_link_types(
         self,
         skip: int = 0,
         take: Optional[int] = None,
         filter_settings: Optional[ConceptLinkTypeFilterSettings] = None,
         direction: SortDirection = "ascending",
         sort_field: ConceptLinkTypeSorting = "id",
-    ) -> Sequence[ConceptLinkType]:
+    ) -> Union[Sequence[ConceptLinkType], Sequence[object_types.LinkType]]:
         op = make_operation(Query, "get_concept_link_types")
         take = self.get_take_value(take)
         if not filter_settings:
             filter_settings = ConceptLinkTypeFilterSettings()
         pclt: ConceptLinkTypePagination = op.pagination_concept_link_type(
             direction=direction, filter_settings=filter_settings, limit=take, offset=skip, sort_field=sort_field
         )
@@ -2128,15 +2460,15 @@
         lclt.__fields__(*self.concept_link_type_fields)
         lclt.concept_from_type().__fields__(*self.concept_type_fields)
         lclt.concept_to_type().__fields__(*self.concept_type_fields)
         res = self._gql_client.execute(op)
         res = op + res
         return res.pagination_concept_link_type.list_concept_link_type
 
-    def get_concept_link_type_by_name(
+    def _get_concept_link_type_by_name(
         self, link_name: str, from_type_id: str, to_type_id: str, limit: int = 20
     ) -> Sequence[ConceptLinkType]:
         op = make_operation(Query, "get_concept_link_type_by_name")
         pclt: ConceptLinkTypePagination = op.pagination_concept_link_type(
             filter_settings=ConceptLinkTypeFilterSettings(
                 name=link_name, concept_from_type_id=from_type_id, concept_to_type_id=to_type_id
             ),
@@ -2146,65 +2478,78 @@
         lclt.__fields__(*self.concept_link_type_fields)
         lclt.concept_from_type().__fields__(*self.concept_type_fields)
         lclt.concept_to_type().__fields__(*self.concept_type_fields)
         res = self._gql_client.execute(op)
         res = op + res
         return res.pagination_concept_link_type.list_concept_link_type
 
-    def get_link_type(self, link_type_code: str) -> Optional[ConceptLinkType]:
+    @prettify
+    def get_concept_link_type_by_name(
+        self, link_name: str, from_type_id: str, to_type_id: str, limit: int = 20
+    ) -> Union[Sequence[ConceptLinkType], Sequence[object_types.LinkType]]:
+        return self._get_concept_link_type_by_name(link_name, from_type_id, to_type_id, limit)
+
+    def _get_link_type(self, link_type_code: str) -> Optional[ConceptLinkType]:
         link_type = self._type_mapping.get_concept_link_type(link_type_code)
         if link_type:
             return link_type
 
         concept_from_type_code = self._type_mapping.get_source_concept_type_code(link_type_code)
         concept_to_type_code = self._type_mapping.get_target_concept_type_code(link_type_code)
-        concept_from_type = self.get_concept_type(concept_from_type_code)
-        concept_to_type = self.get_concept_type(concept_to_type_code)
+        concept_from_type = self._get_concept_type(concept_from_type_code)
+        concept_to_type = self._get_concept_type(concept_to_type_code)
         link_type_name = self._type_mapping.get_concept_link_type_name(link_type_code)
-        link_types = self.get_concept_link_type_by_name(link_type_name, concept_from_type.id, concept_to_type.id)
+        link_types = self._get_concept_link_type_by_name(link_type_name, concept_from_type.id, concept_to_type.id)
         for link_type in link_types:
             if link_type.name == link_type_name:
                 self._type_mapping.add_concept_link_type(link_type_code, link_type)
                 return link_type
         return None
 
-    def add_relation_by_id(
+    @prettify
+    def get_link_type(self, link_type_code: str) -> Union[ConceptLinkType, object_types.LinkType, None]:
+        return self._get_link_type(link_type_code)
+
+    def _add_relation_by_id(
         self, from_id: str, to_id: str, link_type_id: str, perform_synchronously: Optional[bool] = None
     ) -> ConceptLink:
         op = make_operation(Mutation, "add_relation_by_id")
         acl = op.add_concept_link(
             performance_control=PerformSynchronously(
                 perform_synchronously=self.get_perform_synchronously_value(perform_synchronously)
             ),
             form=ConceptLinkCreationMutationInput(
                 concept_from_id=from_id, concept_to_id=to_id, link_type_id=link_type_id
             ),
         )
-        acl.__fields__(*self.concept_link_fields)
-        acl.concept_link_type.__fields__(*self.concept_property_type_fields)
-        acl.concept_link_type.__fields__(*self.concept_link_type_fields_truncated)
-        self._configure_output_concept_fields(acl.concept_from)
-        self._configure_output_concept_fields(acl.concept_to)
+        self._configure_output_link_fields(acl)
 
         res = self._gql_client.execute(op)
         res = op + res
 
         return res.add_concept_link
 
+    @prettify
+    def add_relation_by_id(
+        self, from_id: str, to_id: str, link_type_id: str, perform_synchronously: Optional[bool] = None
+    ) -> Union[ConceptLink, objects.Link]:
+        return self._add_relation_by_id(from_id, to_id, link_type_id, perform_synchronously)
+
+    @prettify
     def add_relation(
         self,
         concept_from_id: str,
         concept_to_id: str,
         type_code: str,
         perform_synchronously: Optional[bool] = None,
-    ) -> ConceptLink:
-        link_type = self.get_link_type(type_code)
+    ) -> Union[ConceptLink, objects.Link]:
+        link_type = self._get_link_type(type_code)
         if not link_type:
             raise Exception("Cannot add relation: no link type")
-        relation = self.add_relation_by_id(
+        relation = self._add_relation_by_id(
             concept_from_id, concept_to_id, link_type.id, perform_synchronously=perform_synchronously
         )
 
         if self.tdm_builder is not None:
             self.tdm_builder.add_link_fact(relation)
 
         return relation
@@ -2232,26 +2577,28 @@
         clp: ConceptProperty = op.delete_concept_link_property(id=link_property_id)
         clp.__fields__("is_success")
         res = self._gql_client.execute(op)
         res = op + res
 
         return res.delete_concept_link_property.is_success
 
+    @prettify
     def add_concept_markers(
         self, concept_id: str, markers: List[str], perform_synchronously: Optional[bool] = None
-    ) -> Concept:
-        c = self.get_concept(concept_id)
+    ) -> Union[Concept, objects.Concept]:
+        c = self._get_concept(concept_id)
         c.markers.extend(markers)
         new_markers = list(set(c.markers))
         return self.update_concept(c, markers=new_markers, perform_synchronously=perform_synchronously)
 
+    @prettify
     def set_concept_markers(
         self, concept_id: str, markers: List[str], perform_synchronously: Optional[bool] = None
-    ) -> Concept:
-        c = self.get_concept(concept_id)
+    ) -> Union[Concept, objects.Concept]:
+        c = self._get_concept(concept_id)
         return self.update_concept(c, markers=markers, perform_synchronously=perform_synchronously)
 
     def get_composite_concept(self, root_concept_id: str, composite_concept_type_id: str) -> CompositeConcept:
         op = make_operation(Query, "get_composite_concept")
         cc: CompositeConcept = op.composite_concept(
             root_concept_id=root_concept_id, composite_concept_type_id=composite_concept_type_id
         )
@@ -2348,26 +2695,28 @@
         op.delete_concept_link_property_fact(
             id=fact_id,
         )
         res = self._gql_client.execute(op)
         res = op + res
         return res.delete_concept_link_property_fact
 
-    def merge_concepts(self, c_main_id: str, c_merged_id: str) -> Concept:
+    @prettify
+    def merge_concepts(self, c_main_id: str, c_merged_id: str) -> Union[Concept, objects.Concept]:
         op = make_operation(Mutation, "merge_concepts")
         mc: Concept = op.merge_concepts(
             form=ConceptMergeInput(main_concept_id=c_main_id, merged_concept_id=c_merged_id)
         )
         self._configure_output_concept_fields(mc)
         res = self._gql_client.execute(op)
         res = op + res
 
         return res.merge_concepts
 
-    def unmerge_concepts(self, c_main_id: str, c_merged_id: List[str]) -> Concept:
+    @prettify
+    def unmerge_concepts(self, c_main_id: str, c_merged_id: List[str]) -> Union[Concept, objects.Concept]:
         op = make_operation(Mutation, "unmerge_concepts")
         umc: Concept = op.unmerge_concepts(
             form=ConceptUnmergeInput(main_concept_id=c_main_id, merged_concept_id=c_merged_id)
         )
         self._configure_output_concept_fields(umc)
         res = self._gql_client.execute(op)
         res = op + res
@@ -2387,28 +2736,30 @@
         res = op + res
         return res.pagination_crawler.list_crawler
 
     # endregion
 
     # region Utils methods
 
+    @prettify
     @check_utils_gql_client
     def create_or_get_concept_by_name(
         self,
         name: str,
         type_id: str,
         notes: Optional[str] = None,
         take_first_result: bool = False,
         with_properties: bool = False,
         with_links: bool = False,
         with_link_properties: bool = False,
         with_facts: bool = False,
         with_potential_facts: bool = False,
         with_metrics: bool = False,
-    ) -> Concept:
+    ) -> Union[Concept, objects.Concept]:
+        """Finds concept by near name"""
         op = make_operation(uas.Mutation, "create_or_get_concept_by_name")
         if type_id:
             concept_filter_settings = uas.ConceptFilterSettings(exact_name=name, concept_type_ids=[type_id])
         else:
             concept_filter_settings = uas.ConceptFilterSettings(exact_name=name)
         goac = op.get_or_add_concept(
             filter_settings=concept_filter_settings,
@@ -2594,15 +2945,15 @@
             uuids = (doc.main.uuid for doc in documents)
 
         yield from self.reprocess_messages(topic_id=topic_id, message_ids=uuids, priority=priority, use_kb=use_kb)
 
     def reprocess_messages(
         self,
         topic_id: str,
-        message_ids: Sequence[str],
+        message_ids: Iterable[str],
         priority: tc.MessagePriority = "Normal",
         use_kb: bool = False,
     ) -> Iterable[Union[str, Exception]]:
         import sgqlc.types
 
         mut = make_operation(
             tc.Mutation,
```

### Comparing `ptal_api-0.12.0.1/ptal_api/core/type_mapper/common/common.py` & `ptal_api-0.12.2/ptal_api/core/type_mapper/common/common.py`

 * *Files identical despite different names*

### Comparing `ptal_api-0.12.0.1/ptal_api/core/type_mapper/data_model/base_data_model.py` & `ptal_api-0.12.2/ptal_api/core/type_mapper/data_model/base_data_model.py`

 * *Files identical despite different names*

### Comparing `ptal_api-0.12.0.1/ptal_api/core/type_mapper/data_model/config_data_model.py` & `ptal_api-0.12.2/ptal_api/core/type_mapper/data_model/config_data_model.py`

 * *Files identical despite different names*

### Comparing `ptal_api-0.12.0.1/ptal_api/core/type_mapper/data_model/custom_data_model.py` & `ptal_api-0.12.2/ptal_api/core/type_mapper/data_model/custom_data_model.py`

 * *Files identical despite different names*

### Comparing `ptal_api-0.12.0.1/ptal_api/core/type_mapper/model_parameters/name_code_mapping.yml` & `ptal_api-0.12.2/ptal_api/core/type_mapper/model_parameters/name_code_mapping.yml`

 * *Files identical despite different names*

### Comparing `ptal_api-0.12.0.1/ptal_api/core/type_mapper/modules/custom_data_handler.py` & `ptal_api-0.12.2/ptal_api/core/type_mapper/modules/custom_data_handler.py`

 * *Files identical despite different names*

### Comparing `ptal_api-0.12.0.1/ptal_api/core/type_mapper/modules/file_generator.py` & `ptal_api-0.12.2/ptal_api/core/type_mapper/modules/file_generator.py`

 * *Files identical despite different names*

### Comparing `ptal_api-0.12.0.1/ptal_api/core/type_mapper/modules/object_name_transformer.py` & `ptal_api-0.12.2/ptal_api/core/type_mapper/modules/object_name_transformer.py`

 * *Files identical despite different names*

### Comparing `ptal_api-0.12.0.1/ptal_api/core/type_mapper/modules/type_mapping_generator.py` & `ptal_api-0.12.2/ptal_api/core/type_mapper/modules/type_mapping_generator.py`

 * *Files identical despite different names*

### Comparing `ptal_api-0.12.0.1/ptal_api/core/type_mapper/modules/type_mapping_loader/type_mapping_loader.py` & `ptal_api-0.12.2/ptal_api/core/type_mapper/modules/type_mapping_loader/type_mapping_loader.py`

 * *Files identical despite different names*

### Comparing `ptal_api-0.12.0.1/ptal_api/core/values/value_mapping.py` & `ptal_api-0.12.2/ptal_api/core/values/value_mapping.py`

 * *Files 16% similar despite different names*

```diff
@@ -104,19 +104,28 @@
         return value_input
 
     @staticmethod
     def get_tdm_value_format(value: str) -> Dict:
         return {"link": value}
 
 
+STRING_VALUE = "StringValue"
+INT_VALUE = "IntValue"
+DOUBLE_VALUE = "DoubleValue"
+DATE_VALUE = "DateValue"
+DATE_TIME_VALUE = "DateTimeValue"
+LINK_VALUE = "LinkValue"
+COMPOSITE_VALUE = "CompositeValue"
+
+
 def get_map_helper(value_type: str) -> Type[AbstractValueMapper]:
-    if value_type == "String":
+    if value_type in ("String", STRING_VALUE):
         return StringValueMapper
-    if value_type == "Int":
+    if value_type in ("Int", INT_VALUE):
         return IntValueMapper
-    if value_type == "Double":
+    if value_type in ("Double", DOUBLE_VALUE):
         return DoubleValueMapper
-    if value_type == "Date":
+    if value_type in ("Date", DATE_VALUE, DATE_TIME_VALUE):
         return DateValueMapper
-    if value_type == "Link":
+    if value_type in ("Link", LINK_VALUE):
         return LinkValueMapper
     raise NotImplementedError(f"{value_type} type not implemented")
```

### Comparing `ptal_api-0.12.0.1/ptal_api/providers/gql_providers.py` & `ptal_api-0.12.2/ptal_api/providers/gql_providers.py`

 * *Files identical despite different names*

### Comparing `ptal_api-0.12.0.1/ptal_api/schema/api_schema.py` & `ptal_api-0.12.2/ptal_api/schema/api_schema.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import sgqlc.types
-# import sgqlc.types.datetime
 
 
 api_schema = sgqlc.types.Schema()
 
 
 
 ########################################################################
@@ -4243,28 +4242,29 @@
         ('filter_settings', sgqlc.types.Arg(ConceptFilterSettings, graphql_name='filterSettings', default=None)),
 ))
     )
 
 
 class Document(sgqlc.types.Type, RecordInterface):
     __schema__ = api_schema
-    __field_names__ = ('id', 'title', 'external_url', 'publication_date', 'publication_author', 'notes', 'document_type', 'highlightings', 'markers', 'tables', 'metadata', 'uuid', 'trust_level', 'score', 'has_text', 'parent', 'list_child', 'pagination_child', 'internal_url', 'avatar', 'metric', 'pagination_concept_fact', 'list_concept_fact', 'pagination_concept_link_fact', 'list_concept_link_document_fact', 'preview', 'pagination_redmine_issues', 'pagination_issue', 'access_level', 'text', 'story', 'list_subscription', 'pagination_similar_documents', 'is_read', 'list_fact')
+    __field_names__ = ('id', 'title', 'external_url', 'publication_date', 'publication_author', 'notes', 'document_type', 'highlightings', 'markers', 'tables', 'metadata', 'uuid', 'trust_level', 'story', 'score', 'has_text', 'parent', 'list_child', 'pagination_child', 'internal_url', 'avatar', 'metric', 'pagination_concept_fact', 'list_concept_fact', 'pagination_concept_link_fact', 'list_concept_link_document_fact', 'preview', 'pagination_redmine_issues', 'pagination_issue', 'access_level', 'text', 'list_subscription', 'pagination_similar_documents', 'is_read', 'list_fact')
     id = sgqlc.types.Field(sgqlc.types.non_null(ID), graphql_name='id')
     title = sgqlc.types.Field(String, graphql_name='title')
     external_url = sgqlc.types.Field(String, graphql_name='externalUrl')
     publication_date = sgqlc.types.Field(UnixTime, graphql_name='publicationDate')
     publication_author = sgqlc.types.Field(String, graphql_name='publicationAuthor')
     notes = sgqlc.types.Field(String, graphql_name='notes')
     document_type = sgqlc.types.Field(sgqlc.types.non_null(DocumentType), graphql_name='documentType')
     highlightings = sgqlc.types.Field(sgqlc.types.non_null(sgqlc.types.list_of(sgqlc.types.non_null(Highlighting))), graphql_name='highlightings')
     markers = sgqlc.types.Field(sgqlc.types.non_null(sgqlc.types.list_of(sgqlc.types.non_null(String))), graphql_name='markers')
     tables = sgqlc.types.Field(sgqlc.types.non_null(sgqlc.types.list_of(sgqlc.types.non_null(Table))), graphql_name='tables')
     metadata = sgqlc.types.Field(DocumentMetadata, graphql_name='metadata')
     uuid = sgqlc.types.Field(sgqlc.types.non_null(ID), graphql_name='uuid')
     trust_level = sgqlc.types.Field(TrustLevel, graphql_name='trustLevel')
+    story = sgqlc.types.Field(sgqlc.types.non_null(ID), graphql_name='story')
     score = sgqlc.types.Field(sgqlc.types.non_null(sgqlc.types.list_of(sgqlc.types.non_null(Score))), graphql_name='score')
     has_text = sgqlc.types.Field(sgqlc.types.non_null(Boolean), graphql_name='hasText')
     parent = sgqlc.types.Field('Document', graphql_name='parent')
     list_child = sgqlc.types.Field(sgqlc.types.non_null(sgqlc.types.list_of(sgqlc.types.non_null('Document'))), graphql_name='listChild')
     pagination_child = sgqlc.types.Field(sgqlc.types.non_null(DocumentPagination), graphql_name='paginationChild', args=sgqlc.types.ArgDict((
         ('offset', sgqlc.types.Arg(Int, graphql_name='offset', default=0)),
         ('limit', sgqlc.types.Arg(Int, graphql_name='limit', default=20)),
@@ -4302,15 +4302,14 @@
 ))
     )
     access_level = sgqlc.types.Field(sgqlc.types.non_null(AccessLevel), graphql_name='accessLevel')
     text = sgqlc.types.Field(sgqlc.types.non_null(sgqlc.types.list_of(sgqlc.types.non_null(FlatDocumentStructure))), graphql_name='text', args=sgqlc.types.ArgDict((
         ('show_hidden', sgqlc.types.Arg(Boolean, graphql_name='showHidden', default=False)),
 ))
     )
-    story = sgqlc.types.Field(sgqlc.types.non_null(ID), graphql_name='story')
     list_subscription = sgqlc.types.Field(sgqlc.types.non_null(DocumentSubscriptions), graphql_name='listSubscription')
     pagination_similar_documents = sgqlc.types.Field(sgqlc.types.non_null(DocumentPagination), graphql_name='paginationSimilarDocuments', args=sgqlc.types.ArgDict((
         ('offset', sgqlc.types.Arg(Int, graphql_name='offset', default=0)),
         ('limit', sgqlc.types.Arg(Int, graphql_name='limit', default=20)),
 ))
     )
     is_read = sgqlc.types.Field(sgqlc.types.non_null(Boolean), graphql_name='isRead')
```

### Comparing `ptal_api-0.12.0.1/ptal_api/schema/crawlers_api_schema.py` & `ptal_api-0.12.2/ptal_api/schema/crawlers_api_schema.py`

 * *Files 1% similar despite different names*

```diff
@@ -339,25 +339,26 @@
     job_pending_sorting = sgqlc.types.Field('JobsPendingSort', graphql_name='jobPendingSorting')
     job_running_sorting = sgqlc.types.Field('JobsRunningSort', graphql_name='jobRunningSorting')
     job_finished_sorting = sgqlc.types.Field('JobsFinishedSort', graphql_name='jobFinishedSorting')
 
 
 class JobsFilterSettings(sgqlc.types.Input):
     __schema__ = crawlers_api_schema
-    __field_names__ = ('input_value', 'projects', 'crawlers', 'creators', 'updaters', 'system_registration_date', 'system_update_date', 'periodic_jobs', 'collection_statuses', 'job_ids', 'start_time', 'end_time')
+    __field_names__ = ('input_value', 'projects', 'crawlers', 'creators', 'updaters', 'system_registration_date', 'system_update_date', 'periodic_jobs', 'collection_statuses', 'job_status', 'job_ids', 'start_time', 'end_time')
     input_value = sgqlc.types.Field(String, graphql_name='inputValue')
     projects = sgqlc.types.Field(sgqlc.types.list_of(sgqlc.types.non_null(ID)), graphql_name='projects')
     crawlers = sgqlc.types.Field(sgqlc.types.list_of(sgqlc.types.non_null(ID)), graphql_name='crawlers')
     creators = sgqlc.types.Field(sgqlc.types.list_of(sgqlc.types.non_null(String)), graphql_name='creators')
     updaters = sgqlc.types.Field(sgqlc.types.list_of(sgqlc.types.non_null(String)), graphql_name='updaters')
     system_registration_date = sgqlc.types.Field('TimestampInterval', graphql_name='systemRegistrationDate')
     system_update_date = sgqlc.types.Field('TimestampInterval', graphql_name='systemUpdateDate')
     periodic_jobs = sgqlc.types.Field(sgqlc.types.list_of(sgqlc.types.non_null(ID)), graphql_name='periodicJobs')
     collection_statuses = sgqlc.types.Field(sgqlc.types.list_of(sgqlc.types.non_null(CollectionStatus)), graphql_name='collectionStatuses')
-    job_ids = sgqlc.types.Field(sgqlc.types.list_of(sgqlc.types.non_null(Long)), graphql_name='jobIds')
+    job_status = sgqlc.types.Field(JobStatus, graphql_name='jobStatus')
+    job_ids = sgqlc.types.Field(sgqlc.types.list_of(sgqlc.types.non_null(ID)), graphql_name='jobIds')
     start_time = sgqlc.types.Field('TimestampInterval', graphql_name='startTime')
     end_time = sgqlc.types.Field('TimestampInterval', graphql_name='endTime')
 
 
 class JobsFinishedSort(sgqlc.types.Input):
     __schema__ = crawlers_api_schema
     __field_names__ = ('sort', 'direction')
@@ -692,14 +693,21 @@
     errors_count = sgqlc.types.Field(Int, graphql_name='errorsCount')
     duplicated_request_count = sgqlc.types.Field(Int, graphql_name='duplicatedRequestCount')
     jobs_with_errors_logs_count = sgqlc.types.Field(Int, graphql_name='jobsWithErrorsLogsCount')
     jobs_with_critical_logs_count = sgqlc.types.Field(Int, graphql_name='jobsWithCriticalLogsCount')
     item_domains = sgqlc.types.Field(sgqlc.types.non_null(sgqlc.types.list_of(sgqlc.types.non_null('Platform'))), graphql_name='itemDomains')
 
 
+class JobSubscription(sgqlc.types.Type):
+    __schema__ = crawlers_api_schema
+    __field_names__ = ('job', 'position')
+    job = sgqlc.types.Field(sgqlc.types.non_null('Job'), graphql_name='job')
+    position = sgqlc.types.Field(sgqlc.types.non_null(Int), graphql_name='position')
+
+
 class Jobs(sgqlc.types.Type):
     __schema__ = crawlers_api_schema
     __field_names__ = ('pending', 'running', 'finished')
     pending = sgqlc.types.Field(sgqlc.types.non_null(JobList), graphql_name='pending')
     running = sgqlc.types.Field(sgqlc.types.non_null(JobList), graphql_name='running')
     finished = sgqlc.types.Field(sgqlc.types.non_null(JobList), graphql_name='finished')
 
@@ -965,15 +973,15 @@
     jobs_with_errors_logs_count = sgqlc.types.Field(Int, graphql_name='jobsWithErrorsLogsCount')
     job_ids_with_error_logs = sgqlc.types.Field(sgqlc.types.non_null(sgqlc.types.list_of(sgqlc.types.non_null(Long))), graphql_name='jobIdsWithErrorLogs')
     jobs_with_critical_logs_count = sgqlc.types.Field(Int, graphql_name='jobsWithCriticalLogsCount')
 
 
 class Query(sgqlc.types.Type):
     __schema__ = crawlers_api_schema
-    __field_names__ = ('analytics', 'crawler', 'list_crawler', 'pagination_crawler', 'crawler_args_and_settings_description', 'crawler_site_map', 'crawl_state', 'crawl_state_by_parameters', 'pagination_crawl_state', 'credential', 'pagination_credential', 'job', 'list_job', 'pagination_job_logs', 'pagination_job_requests', 'pagination_job_metrics', 'pagination_job', 'periodic_job', 'pagination_periodic_job', 'pagination_periodic_job_logs', 'pagination_periodic_job_requests', 'pagination_periodic_job_metrics', 'check_periodic_job_by_input', 'export_periodic_jobs', 'project', 'pagination_project', 'project_args_and_settings_description', 'project_default_args_and_settings_description', 'information_source_loader', 'pagination_information_source_loader', 'information_source', 'pagination_information_source', 'recovery_job', 'pagination_recovery_job', 'version', 'list_version', 'pagination_versions_crawler', 'pagination_egg_file_versions_project', 'web_scraper_version_is_compatible')
+    __field_names__ = ('analytics', 'crawler', 'list_crawler', 'pagination_crawler', 'crawler_args_and_settings_description', 'crawler_site_map', 'crawl_state', 'crawl_state_by_parameters', 'pagination_crawl_state', 'credential', 'pagination_credential', 'job', 'list_job', 'pagination_job_logs', 'pagination_job_requests', 'pagination_job_metrics', 'pagination_job', 'pagination_job_new', 'periodic_job', 'pagination_periodic_job', 'pagination_periodic_job_logs', 'pagination_periodic_job_requests', 'pagination_periodic_job_metrics', 'check_periodic_job_by_input', 'export_periodic_jobs', 'project', 'pagination_project', 'project_args_and_settings_description', 'project_default_args_and_settings_description', 'information_source_loader', 'pagination_information_source_loader', 'information_source', 'pagination_information_source', 'recovery_job', 'pagination_recovery_job', 'version', 'list_version', 'pagination_versions_crawler', 'pagination_egg_file_versions_project', 'web_scraper_version_is_compatible')
     analytics = sgqlc.types.Field(sgqlc.types.non_null('Stats'), graphql_name='analytics')
     crawler = sgqlc.types.Field(sgqlc.types.non_null('Crawler'), graphql_name='crawler', args=sgqlc.types.ArgDict((
         ('id', sgqlc.types.Arg(sgqlc.types.non_null(ID), graphql_name='id', default=None)),
 ))
     )
     list_crawler = sgqlc.types.Field(sgqlc.types.non_null(sgqlc.types.list_of('Crawler')), graphql_name='listCrawler', args=sgqlc.types.ArgDict((
         ('ids', sgqlc.types.Arg(sgqlc.types.non_null(sgqlc.types.list_of(sgqlc.types.non_null(ID))), graphql_name='ids', default=None)),
@@ -1060,15 +1068,22 @@
         ('sort_field', sgqlc.types.Arg(MetricSorting, graphql_name='sortField', default='timestamp')),
 ))
     )
     pagination_job = sgqlc.types.Field(sgqlc.types.non_null(JobPagination), graphql_name='paginationJob', args=sgqlc.types.ArgDict((
         ('limit', sgqlc.types.Arg(Int, graphql_name='limit', default=20)),
         ('offset', sgqlc.types.Arg(Int, graphql_name='offset', default=0)),
         ('sort', sgqlc.types.Arg(JobSorting, graphql_name='sort', default={'jobPendingSorting': {'sort': 'id', 'direction': 'descending'}, 'jobRunningSorting': {'sort': 'id', 'direction': 'descending'}, 'jobFinishedSorting': {'sort': 'id', 'direction': 'descending'}})),
-        ('jobs_filter_settings', sgqlc.types.Arg(JobsFilterSettings, graphql_name='jobsFilterSettings', default={})),
+        ('jobs_filter_settings', sgqlc.types.Arg(JobsFilterSettings, graphql_name='jobsFilterSettings', default={'jobStatus': 'Finished'})),
+))
+    )
+    pagination_job_new = sgqlc.types.Field(sgqlc.types.non_null(JobList), graphql_name='paginationJobNew', args=sgqlc.types.ArgDict((
+        ('limit', sgqlc.types.Arg(Int, graphql_name='limit', default=20)),
+        ('offset', sgqlc.types.Arg(Int, graphql_name='offset', default=0)),
+        ('sort', sgqlc.types.Arg(JobSorting, graphql_name='sort', default={'jobPendingSorting': {'sort': 'id', 'direction': 'descending'}, 'jobRunningSorting': {'sort': 'id', 'direction': 'descending'}, 'jobFinishedSorting': {'sort': 'id', 'direction': 'descending'}})),
+        ('jobs_filter_settings', sgqlc.types.Arg(JobsFilterSettings, graphql_name='jobsFilterSettings', default={'jobStatus': 'Finished'})),
 ))
     )
     periodic_job = sgqlc.types.Field(sgqlc.types.non_null('PeriodicJob'), graphql_name='periodicJob', args=sgqlc.types.ArgDict((
         ('id', sgqlc.types.Arg(sgqlc.types.non_null(ID), graphql_name='id', default=None)),
 ))
     )
     pagination_periodic_job = sgqlc.types.Field(sgqlc.types.non_null(PeriodicJobPagination), graphql_name='paginationPeriodicJob', args=sgqlc.types.ArgDict((
@@ -1284,14 +1299,26 @@
     )
     previous_items_histogram = sgqlc.types.Field(sgqlc.types.non_null(sgqlc.types.list_of(sgqlc.types.non_null(DateHistogramBucket))), graphql_name='previousItemsHistogram', args=sgqlc.types.ArgDict((
         ('interval', sgqlc.types.Arg(TimestampInterval, graphql_name='interval', default=None)),
 ))
     )
 
 
+class Subscription(sgqlc.types.Type):
+    __schema__ = crawlers_api_schema
+    __field_names__ = ('job',)
+    job = sgqlc.types.Field(sgqlc.types.non_null(JobSubscription), graphql_name='job', args=sgqlc.types.ArgDict((
+        ('limit', sgqlc.types.Arg(Int, graphql_name='limit', default=20)),
+        ('offset', sgqlc.types.Arg(Int, graphql_name='offset', default=0)),
+        ('sort', sgqlc.types.Arg(JobSorting, graphql_name='sort', default={'jobPendingSorting': {'sort': 'id', 'direction': 'descending'}, 'jobRunningSorting': {'sort': 'id', 'direction': 'descending'}, 'jobFinishedSorting': {'sort': 'id', 'direction': 'descending'}})),
+        ('jobs_filter_settings', sgqlc.types.Arg(JobsFilterSettings, graphql_name='jobsFilterSettings', default={'jobStatus': 'Finished'})),
+))
+    )
+
+
 class UpdateProjectStats(sgqlc.types.Type):
     __schema__ = crawlers_api_schema
     __field_names__ = ('added_crawlers_count', 'deleted_crawlers_count', 'updated_crawlers_count', 'is_metadata_updated', 'updated_periodic_ids', 'stopped_periodic_ids')
     added_crawlers_count = sgqlc.types.Field(sgqlc.types.non_null(Long), graphql_name='addedCrawlersCount')
     deleted_crawlers_count = sgqlc.types.Field(sgqlc.types.non_null(Long), graphql_name='deletedCrawlersCount')
     updated_crawlers_count = sgqlc.types.Field(sgqlc.types.non_null(Long), graphql_name='updatedCrawlersCount')
     is_metadata_updated = sgqlc.types.Field(sgqlc.types.non_null(Boolean), graphql_name='isMetadataUpdated')
@@ -1487,9 +1514,9 @@
 ########################################################################
 
 ########################################################################
 # Schema Entry Points
 ########################################################################
 crawlers_api_schema.query_type = Query
 crawlers_api_schema.mutation_type = Mutation
-crawlers_api_schema.subscription_type = None
+crawlers_api_schema.subscription_type = Subscription
```

### Comparing `ptal_api-0.12.0.1/ptal_api/schema/tcontroller_api_schema.py` & `ptal_api-0.12.2/ptal_api/schema/tcontroller_api_schema.py`

 * *Files identical despite different names*

### Comparing `ptal_api-0.12.0.1/ptal_api/schema/utils_api_schema.py` & `ptal_api-0.12.2/ptal_api/schema/utils_api_schema.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import sgqlc.types
-# import sgqlc.types.datetime
 
 
 utils_api_schema = sgqlc.types.Schema()
 
 
 
 ########################################################################
@@ -1916,28 +1915,29 @@
         ('filter_settings', sgqlc.types.Arg(ConceptFilterSettings, graphql_name='filterSettings', default=None)),
 ))
     )
 
 
 class Document(sgqlc.types.Type, RecordInterface):
     __schema__ = utils_api_schema
-    __field_names__ = ('id', 'title', 'external_url', 'publication_date', 'publication_author', 'notes', 'document_type', 'highlightings', 'markers', 'tables', 'metadata', 'uuid', 'trust_level', 'score', 'has_text', 'parent', 'list_child', 'pagination_child', 'internal_url', 'avatar', 'metric', 'pagination_concept_fact', 'list_concept_fact', 'pagination_concept_link_fact', 'list_concept_link_document_fact', 'preview', 'pagination_redmine_issues', 'pagination_issue', 'access_level', 'text', 'story', 'list_subscription', 'pagination_similar_documents', 'is_read', 'list_fact')
+    __field_names__ = ('id', 'title', 'external_url', 'publication_date', 'publication_author', 'notes', 'document_type', 'highlightings', 'markers', 'tables', 'metadata', 'uuid', 'trust_level', 'story', 'score', 'has_text', 'parent', 'list_child', 'pagination_child', 'internal_url', 'avatar', 'metric', 'pagination_concept_fact', 'list_concept_fact', 'pagination_concept_link_fact', 'list_concept_link_document_fact', 'preview', 'pagination_redmine_issues', 'pagination_issue', 'access_level', 'text', 'list_subscription', 'pagination_similar_documents', 'is_read', 'list_fact')
     id = sgqlc.types.Field(sgqlc.types.non_null(ID), graphql_name='id')
     title = sgqlc.types.Field(String, graphql_name='title')
     external_url = sgqlc.types.Field(String, graphql_name='externalUrl')
     publication_date = sgqlc.types.Field(UnixTime, graphql_name='publicationDate')
     publication_author = sgqlc.types.Field(String, graphql_name='publicationAuthor')
     notes = sgqlc.types.Field(String, graphql_name='notes')
     document_type = sgqlc.types.Field(sgqlc.types.non_null(DocumentType), graphql_name='documentType')
     highlightings = sgqlc.types.Field(sgqlc.types.non_null(sgqlc.types.list_of(sgqlc.types.non_null(Highlighting))), graphql_name='highlightings')
     markers = sgqlc.types.Field(sgqlc.types.non_null(sgqlc.types.list_of(sgqlc.types.non_null(String))), graphql_name='markers')
     tables = sgqlc.types.Field(sgqlc.types.non_null(sgqlc.types.list_of(sgqlc.types.non_null(Table))), graphql_name='tables')
     metadata = sgqlc.types.Field(DocumentMetadata, graphql_name='metadata')
     uuid = sgqlc.types.Field(sgqlc.types.non_null(ID), graphql_name='uuid')
     trust_level = sgqlc.types.Field(TrustLevel, graphql_name='trustLevel')
+    story = sgqlc.types.Field(sgqlc.types.non_null(ID), graphql_name='story')
     score = sgqlc.types.Field(sgqlc.types.non_null(sgqlc.types.list_of(sgqlc.types.non_null(Score))), graphql_name='score')
     has_text = sgqlc.types.Field(sgqlc.types.non_null(Boolean), graphql_name='hasText')
     parent = sgqlc.types.Field('Document', graphql_name='parent')
     list_child = sgqlc.types.Field(sgqlc.types.non_null(sgqlc.types.list_of(sgqlc.types.non_null('Document'))), graphql_name='listChild')
     pagination_child = sgqlc.types.Field(sgqlc.types.non_null(DocumentPagination), graphql_name='paginationChild', args=sgqlc.types.ArgDict((
         ('offset', sgqlc.types.Arg(Int, graphql_name='offset', default=0)),
         ('limit', sgqlc.types.Arg(Int, graphql_name='limit', default=20)),
@@ -1975,15 +1975,14 @@
 ))
     )
     access_level = sgqlc.types.Field(sgqlc.types.non_null(AccessLevel), graphql_name='accessLevel')
     text = sgqlc.types.Field(sgqlc.types.non_null(sgqlc.types.list_of(sgqlc.types.non_null(FlatDocumentStructure))), graphql_name='text', args=sgqlc.types.ArgDict((
         ('show_hidden', sgqlc.types.Arg(Boolean, graphql_name='showHidden', default=False)),
 ))
     )
-    story = sgqlc.types.Field(sgqlc.types.non_null(ID), graphql_name='story')
     list_subscription = sgqlc.types.Field(sgqlc.types.non_null(DocumentSubscriptions), graphql_name='listSubscription')
     pagination_similar_documents = sgqlc.types.Field(sgqlc.types.non_null(DocumentPagination), graphql_name='paginationSimilarDocuments', args=sgqlc.types.ArgDict((
         ('offset', sgqlc.types.Arg(Int, graphql_name='offset', default=0)),
         ('limit', sgqlc.types.Arg(Int, graphql_name='limit', default=20)),
 ))
     )
     is_read = sgqlc.types.Field(sgqlc.types.non_null(Boolean), graphql_name='isRead')
```

### Comparing `ptal_api-0.12.0.1/ptal_api/scripts/type_mapper.py` & `ptal_api-0.12.2/ptal_api/scripts/type_mapper.py`

 * *Files identical despite different names*

### Comparing `ptal_api-0.12.0.1/ptal_api/tdm_builder/tdm_builder.py` & `ptal_api-0.12.2/ptal_api/tdm_builder/tdm_builder.py`

 * *Files identical despite different names*

### Comparing `ptal_api-0.12.0.1/pyproject.toml` & `ptal_api-0.12.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ptal-api"
-version = "0.12.0.1"
+version = "0.12.2"
 description = "TALISMAN API adapter"
 authors = ["Evgeny Bechkalo <bechkalo@ispras.ru>", "Ivan Medvedev <medvedev.iv@ispras.ru>", "Alexey Isakov <isakov@ispras.ru>"]
 readme = "README.md"
 packages = [{include = "ptal_api"}]
 classifiers = [
     'Development Status :: 3 - Alpha',
     'Programming Language :: Python :: 3',
```

### Comparing `ptal_api-0.12.0.1/PKG-INFO` & `ptal_api-0.12.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ptal-api
-Version: 0.12.0.1
+Version: 0.12.2
 Summary: TALISMAN API adapter
 Author: Evgeny Bechkalo
 Author-email: bechkalo@ispras.ru
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

