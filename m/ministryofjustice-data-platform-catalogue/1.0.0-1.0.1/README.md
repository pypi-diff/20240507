# Comparing `tmp/ministryofjustice_data_platform_catalogue-1.0.0.tar.gz` & `tmp/ministryofjustice_data_platform_catalogue-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ministryofjustice_data_platform_catalogue-1.0.0.tar", max compression
+gzip compressed data, was "ministryofjustice_data_platform_catalogue-1.0.1.tar", max compression
```

## Comparing `ministryofjustice_data_platform_catalogue-1.0.0.tar` & `ministryofjustice_data_platform_catalogue-1.0.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     3041 2024-04-30 09:05:10.108268 ministryofjustice_data_platform_catalogue-1.0.0/README.md
--rw-r--r--   0        0        0     3038 2024-04-30 09:05:10.108268 ministryofjustice_data_platform_catalogue-1.0.0/data_platform_catalogue/client/README.md
--rw-r--r--   0        0        0        0 2024-04-30 09:05:10.108268 ministryofjustice_data_platform_catalogue-1.0.0/data_platform_catalogue/client/__init__.py
--rw-r--r--   0        0        0    19189 2024-04-30 09:05:10.108268 ministryofjustice_data_platform_catalogue-1.0.0/data_platform_catalogue/client/datahub_client.py
--rw-r--r--   0        0        0      544 2024-04-30 09:05:10.108268 ministryofjustice_data_platform_catalogue-1.0.0/data_platform_catalogue/client/exceptions.py
--rw-r--r--   0        0        0        0 2024-04-30 09:05:10.108268 ministryofjustice_data_platform_catalogue-1.0.0/data_platform_catalogue/client/graphql/__init__.py
--rw-r--r--   0        0        0      694 2024-04-30 09:05:10.108268 ministryofjustice_data_platform_catalogue-1.0.0/data_platform_catalogue/client/graphql/facets.graphql
--rw-r--r--   0        0        0      651 2024-04-30 09:05:10.108268 ministryofjustice_data_platform_catalogue-1.0.0/data_platform_catalogue/client/graphql/getChartDetails.graphql
--rw-r--r--   0        0        0     2305 2024-04-30 09:05:10.108268 ministryofjustice_data_platform_catalogue-1.0.0/data_platform_catalogue/client/graphql/getDatasetDetails.graphql
--rw-r--r--   0        0        0      519 2024-04-30 09:05:10.108268 ministryofjustice_data_platform_catalogue-1.0.0/data_platform_catalogue/client/graphql/getGlossaryTerms.graphql
--rw-r--r--   0        0        0      656 2024-04-30 09:05:10.108268 ministryofjustice_data_platform_catalogue-1.0.0/data_platform_catalogue/client/graphql/listContainerEntities.graphql
--rw-r--r--   0        0        0     5891 2024-04-30 09:05:10.108268 ministryofjustice_data_platform_catalogue-1.0.0/data_platform_catalogue/client/graphql/search.graphql
--rw-r--r--   0        0        0     7194 2024-04-30 09:05:10.108268 ministryofjustice_data_platform_catalogue-1.0.0/data_platform_catalogue/client/graphql_helpers.py
--rw-r--r--   0        0        0    13517 2024-04-30 09:05:10.108268 ministryofjustice_data_platform_catalogue-1.0.0/data_platform_catalogue/client/search.py
--rw-r--r--   0        0        0     7325 2024-04-30 09:05:10.108268 ministryofjustice_data_platform_catalogue-1.0.0/data_platform_catalogue/entities.py
--rw-r--r--   0        0        0     2391 2024-04-30 09:05:10.108268 ministryofjustice_data_platform_catalogue-1.0.0/data_platform_catalogue/search_types.py
--rw-r--r--   0        0        0      750 2024-04-30 09:05:10.108268 ministryofjustice_data_platform_catalogue-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     3810 1970-01-01 00:00:00.000000 ministryofjustice_data_platform_catalogue-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0      667 2024-05-07 09:09:20.865223 ministryofjustice_data_platform_catalogue-1.0.1/README.md
+-rw-r--r--   0        0        0        0 2024-05-07 09:09:20.865223 ministryofjustice_data_platform_catalogue-1.0.1/data_platform_catalogue/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-07 09:09:20.865223 ministryofjustice_data_platform_catalogue-1.0.1/data_platform_catalogue/client/__init__.py
+-rw-r--r--   0        0        0    19105 2024-05-07 09:09:20.865223 ministryofjustice_data_platform_catalogue-1.0.1/data_platform_catalogue/client/datahub_client.py
+-rw-r--r--   0        0        0      544 2024-05-07 09:09:20.865223 ministryofjustice_data_platform_catalogue-1.0.1/data_platform_catalogue/client/exceptions.py
+-rw-r--r--   0        0        0        0 2024-05-07 09:09:20.865223 ministryofjustice_data_platform_catalogue-1.0.1/data_platform_catalogue/client/graphql/__init__.py
+-rw-r--r--   0        0        0      694 2024-05-07 09:09:20.865223 ministryofjustice_data_platform_catalogue-1.0.1/data_platform_catalogue/client/graphql/facets.graphql
+-rw-r--r--   0        0        0      651 2024-05-07 09:09:20.865223 ministryofjustice_data_platform_catalogue-1.0.1/data_platform_catalogue/client/graphql/getChartDetails.graphql
+-rw-r--r--   0        0        0     2305 2024-05-07 09:09:20.865223 ministryofjustice_data_platform_catalogue-1.0.1/data_platform_catalogue/client/graphql/getDatasetDetails.graphql
+-rw-r--r--   0        0        0      519 2024-05-07 09:09:20.865223 ministryofjustice_data_platform_catalogue-1.0.1/data_platform_catalogue/client/graphql/getGlossaryTerms.graphql
+-rw-r--r--   0        0        0      656 2024-05-07 09:09:20.865223 ministryofjustice_data_platform_catalogue-1.0.1/data_platform_catalogue/client/graphql/listContainerEntities.graphql
+-rw-r--r--   0        0        0     5891 2024-05-07 09:09:20.865223 ministryofjustice_data_platform_catalogue-1.0.1/data_platform_catalogue/client/graphql/search.graphql
+-rw-r--r--   0        0        0     8194 2024-05-07 09:09:20.865223 ministryofjustice_data_platform_catalogue-1.0.1/data_platform_catalogue/client/graphql_helpers.py
+-rw-r--r--   0        0        0    13436 2024-05-07 09:09:20.865223 ministryofjustice_data_platform_catalogue-1.0.1/data_platform_catalogue/client/search.py
+-rw-r--r--   0        0        0     7302 2024-05-07 09:09:20.865223 ministryofjustice_data_platform_catalogue-1.0.1/data_platform_catalogue/entities.py
+-rw-r--r--   0        0        0     2418 2024-05-07 09:09:20.865223 ministryofjustice_data_platform_catalogue-1.0.1/data_platform_catalogue/search_types.py
+-rw-r--r--   0        0        0      764 2024-05-07 09:09:20.865223 ministryofjustice_data_platform_catalogue-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     1457 1970-01-01 00:00:00.000000 ministryofjustice_data_platform_catalogue-1.0.1/PKG-INFO
```

### Comparing `ministryofjustice_data_platform_catalogue-1.0.0/data_platform_catalogue/client/datahub_client.py` & `ministryofjustice_data_platform_catalogue-1.0.1/data_platform_catalogue/client/datahub_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,15 @@
     InvalidDomain,
     ReferencedEntityMissing,
 )
 from data_platform_catalogue.client.graphql_helpers import (
     parse_columns,
     parse_created_and_modified,
     parse_domain,
+    parse_names,
     parse_owner,
     parse_properties,
     parse_relations,
     parse_tags,
 )
 from data_platform_catalogue.client.search import SearchClient
 from data_platform_catalogue.entities import (
@@ -218,30 +219,30 @@
             ]
             platform_name = response["platform"]["name"]
             properties, custom_properties = parse_properties(response)
             columns = parse_columns(response)
             domain = parse_domain(response)
             owner = parse_owner(response)
             tags = parse_tags(response)
-            name = properties.get("name", response.get("name"))
             created, modified = parse_created_and_modified(properties)
+            name, display_name, qualified_name = parse_names(response, properties)
 
             # A dataset can't have multiple parents, but if we did
             # start to use in that we'd need to change this
             if response["container_relations"]["total"] > 0:
                 relations = parse_relations(
                     RelationshipType.PARENT, response["container_relations"]
                 )
             else:
                 relations = {}
             return Table(
                 urn=None,
-                display_name=properties.get("qualifiedName") or name,
+                display_name=display_name,
                 name=name,
-                fully_qualified_name=properties.get("qualifiedName") or name,
+                fully_qualified_name=qualified_name,
                 description=properties.get("description", ""),
                 relationships=relations,
                 domain=domain,
                 governance=Governance(
                     data_owner=owner,
                     data_stewards=[owner],
                 ),
@@ -260,24 +261,23 @@
                 "chart"
             ]
             platform_name = response["platform"]["name"]
             properties, custom_properties = parse_properties(response)
             domain = parse_domain(response)
             owner = parse_owner(response)
             tags = parse_tags(response)
+            name, display_name, qualified_name = parse_names(response, properties)
 
             return Chart(
                 urn=urn,
                 external_url=properties.get("externalUrl", ""),
                 description=properties.get("description", ""),
-                display_name=properties.get("displayName", properties.get("name")),
-                name=properties["name"],
-                fully_qualified_name=properties.get(
-                    "qualifiedName", properties.get("name")
-                ),
+                name=name,
+                display_name=display_name,
+                fully_qualified_name=qualified_name,
                 domain=domain,
                 governance=Governance(
                     data_owner=owner,
                     data_stewards=[
                         OwnerRef(
                             display_name="", email="Contact email for the user", urn=""
                         )
@@ -508,16 +508,15 @@
         we cannot push nested structures to datahub custom properties
         """
         custom_properties_dict = json.loads(
             custom_properties.model_dump_json(), parse_int=str
         )
         custom_properties_unnested = self._flatten_dict(custom_properties_dict)
         custom_properties_unnested_all_string_values = {
-            key: str(value)
-            # if value is not None else value
+            key: str(value) if value is not None else ""
             for key, value in custom_properties_unnested.items()
         }
 
         return custom_properties_unnested_all_string_values
 
     def _flatten_dict(self, d, custom_properties=None):
         if custom_properties is None:
```

### Comparing `ministryofjustice_data_platform_catalogue-1.0.0/data_platform_catalogue/client/exceptions.py` & `ministryofjustice_data_platform_catalogue-1.0.1/data_platform_catalogue/client/exceptions.py`

 * *Files identical despite different names*

### Comparing `ministryofjustice_data_platform_catalogue-1.0.0/data_platform_catalogue/client/graphql/facets.graphql` & `ministryofjustice_data_platform_catalogue-1.0.1/data_platform_catalogue/client/graphql/facets.graphql`

 * *Files identical despite different names*

### Comparing `ministryofjustice_data_platform_catalogue-1.0.0/data_platform_catalogue/client/graphql/getChartDetails.graphql` & `ministryofjustice_data_platform_catalogue-1.0.1/data_platform_catalogue/client/graphql/getChartDetails.graphql`

 * *Files identical despite different names*

### Comparing `ministryofjustice_data_platform_catalogue-1.0.0/data_platform_catalogue/client/graphql/getDatasetDetails.graphql` & `ministryofjustice_data_platform_catalogue-1.0.1/data_platform_catalogue/client/graphql/getDatasetDetails.graphql`

 * *Files identical despite different names*

### Comparing `ministryofjustice_data_platform_catalogue-1.0.0/data_platform_catalogue/client/graphql/getGlossaryTerms.graphql` & `ministryofjustice_data_platform_catalogue-1.0.1/data_platform_catalogue/client/graphql/getGlossaryTerms.graphql`

 * *Files identical despite different names*

### Comparing `ministryofjustice_data_platform_catalogue-1.0.0/data_platform_catalogue/client/graphql/listContainerEntities.graphql` & `ministryofjustice_data_platform_catalogue-1.0.1/data_platform_catalogue/client/graphql/listContainerEntities.graphql`

 * *Files identical despite different names*

### Comparing `ministryofjustice_data_platform_catalogue-1.0.0/data_platform_catalogue/client/graphql/search.graphql` & `ministryofjustice_data_platform_catalogue-1.0.1/data_platform_catalogue/client/graphql/search.graphql`

 * *Files identical despite different names*

### Comparing `ministryofjustice_data_platform_catalogue-1.0.0/data_platform_catalogue/client/graphql_helpers.py` & `ministryofjustice_data_platform_catalogue-1.0.1/data_platform_catalogue/client/graphql_helpers.py`

 * *Files 6% similar despite different names*

```diff
@@ -86,30 +86,59 @@
     """
     Parse properties and editableProperties into a single dictionary.
     """
     properties = entity["properties"] or {}
     editable_properties = entity.get("editableProperties") or {}
     properties.update(editable_properties)
     custom_properties_dict = {
-        i["key"]: i["value"] for i in properties.get("customProperties", [])
+        i["key"]: i["value"] or "" for i in properties.get("customProperties", [])
     }
+
+    if "dpia_required" in custom_properties_dict:
+        custom_properties_dict["dpia_required"] = (
+            custom_properties_dict["dpia_required"] == "True"
+        )
+
     properties.pop("customProperties", None)
     access_information = AccessInformation.model_validate(custom_properties_dict)
     usage_restrictions = UsageRestrictions.model_validate(custom_properties_dict)
     data_summary = DataSummary.model_validate(custom_properties_dict)
 
     custom_properties = CustomEntityProperties(
         access_information=access_information,
         usage_restrictions=usage_restrictions,
         data_summary=data_summary,
     )
 
     return properties, custom_properties
 
 
+def parse_names(
+    entity: dict[str, Any], properties: dict[str, Any]
+) -> Tuple[str, str, str]:
+    """
+    Returns a tuple of 3 name values.
+
+    The first value is the non-qualified version of the entity name,
+    and the second value is the human-friendly display name.
+
+    Either of these can be used when showing the entity providing it is within
+    the context of its container.
+
+    The third value is the fully qualified name (e.g. my_database.my_table), which
+    can be used to show the entity out of context.
+    """
+    top_level_name = entity.get("name")
+    name = properties.get("name", top_level_name)
+    display_name = properties.get("displayName") or name
+    qualified_name = properties.get("qualifiedName") or top_level_name or name
+
+    return name, display_name, qualified_name
+
+
 def parse_domain(entity: dict[str, Any]) -> DomainRef:
     domain = entity.get("domain") or {}
     inner_domain = domain.get("domain") or {}
     domain_id = inner_domain.get("urn", "")
     if inner_domain:
         domain_properties, _ = parse_properties(inner_domain)
         display_name = domain_properties.get("name", "")
@@ -173,15 +202,15 @@
         field_path = field["fieldPath"]
         display_name = field_path.split(".")[-1]
 
         result.append(
             Column(
                 name=field_path,
                 display_name=display_name,
-                description=field["description"],
+                description=field.get("description") or "",
                 type=field.get("nativeDataType", field["type"]),
                 nullable=field["nullable"],
                 is_primary_key=is_primary_key,
                 foreign_keys=foreign_keys_for_field,
             )
         )
```

### Comparing `ministryofjustice_data_platform_catalogue-1.0.0/data_platform_catalogue/client/search.py` & `ministryofjustice_data_platform_catalogue-1.0.1/data_platform_catalogue/client/search.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 import json
 import logging
 from importlib.resources import files
 from typing import Any, Sequence
 
-from data_platform_catalogue.client.exceptions import (  # pylint: disable=E0611
-    CatalogueError,
-)
+from data_platform_catalogue.client.exceptions import CatalogueError
 from data_platform_catalogue.client.graphql_helpers import (
     parse_created_and_modified,
     parse_domain,
     parse_last_modified,
+    parse_names,
     parse_owner,
     parse_properties,
     parse_relations,
     parse_tags,
 )
-from data_platform_catalogue.entities import RelationshipType  # pylint: disable=E0611
+from data_platform_catalogue.entities import RelationshipType
 from data_platform_catalogue.search_types import (
     FacetOption,
     MultiSelectFilter,
     ResultType,
     SearchFacets,
     SearchResponse,
     SearchResult,
@@ -240,15 +239,15 @@
         """
         Map a dataset entity to a SearchResult
         """
         owner = parse_owner(entity)
         properties, custom_properties = parse_properties(entity)
         tags = parse_tags(entity)
         last_modified = parse_last_modified(entity)
-        name = entity.get("name")
+        name, display_name, qualified_name = parse_names(entity, properties)
 
         relations = parse_relations(
             RelationshipType.PARENT, entity.get("relationships", {})
         )
         domain = parse_domain(entity)
 
         metadata = {
@@ -261,26 +260,23 @@
             "entity_types": self._parse_types_and_sub_types(entity, "Dataset"),
         }
 
         metadata.update(custom_properties.usage_restrictions.model_dump())
         metadata.update(custom_properties.access_information.model_dump())
         metadata.update(custom_properties.data_summary.model_dump())
 
-        # TODO: the way we return name/display name/qualified name should be
-        # consistent with the upsert/get methods
-        fqn = properties.get("qualifiedName", name)
-
         _, modified = parse_created_and_modified(properties)
 
         return SearchResult(
             urn=entity["urn"],
             result_type=result_type,
             matches=matches,
-            name=properties.get("name", name),
-            fully_qualified_name=fqn,
+            name=name,
+            display_name=display_name,
+            fully_qualified_name=qualified_name,
             description=properties.get("description", ""),
             metadata=metadata,
             tags=[tag_str.display_name for tag_str in tags],
             last_modified=modified or last_modified,
         )
 
     def _parse_facets(self, facets: list[dict[str, Any]]) -> SearchFacets:
@@ -305,20 +301,23 @@
             results[field] = options
 
         return SearchFacets(results)
 
     def _parse_glossary_term(self, entity) -> SearchResult:
         properties, _ = parse_properties(entity)
         metadata = {"parentNodes": entity["parentNodes"]["nodes"]}
+        name, display_name, qualified_name = parse_names(entity, properties)
 
         return SearchResult(
             urn=entity["urn"],
             result_type=ResultType.GLOSSARY_TERM,
             matches={},
-            name=properties["name"],
+            name=name,
+            display_name=display_name,
+            fully_qualified_name=qualified_name,
             description=properties.get("description", ""),
             metadata=metadata,
             tags=[],
             last_modified=None,
         )
 
     def get_glossary_terms(self, count: int = 1000) -> SearchResponse:
@@ -347,18 +346,15 @@
         Map a Container entity to a SearchResult
         """
         tags = parse_tags(entity)
         last_modified = parse_last_modified(entity)
         properties, custom_properties = parse_properties(entity)
         domain = parse_domain(entity)
         owner = parse_owner(entity)
-
-        # TODO: the way we return name/display name/qualified name should be
-        # consistent with the upsert/get methods
-        fqn = properties.get("qualifiedName", properties["name"])
+        name, display_name, qualified_name = parse_names(entity, properties)
 
         metadata = {
             "owner": owner.display_name,
             "owner_email": owner.email,
             "domain_name": domain.display_name,
             "domain_id": domain.urn,
             "entity_types": self._parse_types_and_sub_types(entity, "Container"),
@@ -369,16 +365,17 @@
         metadata.update(custom_properties.data_summary.model_dump())
         metadata.update(custom_properties)
 
         return SearchResult(
             urn=entity["urn"],
             result_type=ResultType.DATABASE,
             matches=matches,
-            name=properties["name"],
-            fully_qualified_name=fqn,
+            name=name,
+            fully_qualified_name=qualified_name,
+            display_name=display_name,
             description=properties.get("description", ""),
             metadata=metadata,
             tags=[tag.display_name for tag in tags],
             last_modified=last_modified,
         )
 
     def _parse_types_and_sub_types(self, entity: dict, entity_type: str) -> dict:
```

### Comparing `ministryofjustice_data_platform_catalogue-1.0.0/data_platform_catalogue/entities.py` & `ministryofjustice_data_platform_catalogue-1.0.1/data_platform_catalogue/entities.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,16 +47,16 @@
         description="The data type of the column as it appears in the table",
     )
     description: str = Field(description="A description of the column")
     nullable: bool = Field(description="Whether the field is nullable or not")
     is_primary_key: bool = Field(
         description="Whether the field is part of the primary key"
     )
-    foreign_keys: list[ColumnRef] | None = Field(
-        description="References to columns in other tables"
+    foreign_keys: list[ColumnRef] = Field(
+        description="References to columns in other tables", default_factory=list
     )
 
 
 class OwnerRef(BaseModel):
     """
     A reference to a named individual that performs some kind of governance
     """
@@ -110,20 +110,20 @@
 
 
 class UsageRestrictions(BaseModel):
     """
     Metadata about how entities may be used.
     """
 
-    dpia_required: bool | str | None = Field(
+    dpia_required: bool | None = Field(
         description="Bool for if a data privacy impact assessment (DPIA) is required to access this database",
         default=None,
     )
-    dpia_location: str | None = Field(
-        description="Where to find the DPIA document", default=None
+    dpia_location: str = Field(
+        description="Where to find the DPIA document", default=""
     )
 
 
 class AccessInformation(BaseModel):
     """
     Any metadata about how to access a data entity.
     The same data entity may be accessable via multiple means.
@@ -132,17 +132,15 @@
     where_to_access_dataset: str = Field(
         description="User-friendly description of where the data can be accessed",
         default="",
     )
     source_dataset_name: str = Field(
         description="The name of a dataset this data was derived from", default=""
     )
-    s3_location: str | None = Field(
-        description="Location of the data in s3", default=None
-    )
+    s3_location: str = Field(description="Location of the data in s3", default="")
 
 
 class DataSummary(BaseModel):
     """
     Summarised information derived from the actual data.
     """
```

### Comparing `ministryofjustice_data_platform_catalogue-1.0.0/data_platform_catalogue/search_types.py` & `ministryofjustice_data_platform_catalogue-1.0.1/data_platform_catalogue/search_types.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,14 +53,15 @@
 
 
 @dataclass
 class SearchResult:
     urn: str
     result_type: ResultType
     name: str
+    display_name: str = ""
     fully_qualified_name: str = ""
     description: str = ""
     matches: dict[str, str] = field(default_factory=dict)
     metadata: dict[str, Any] = field(default_factory=dict)
     tags: list[str] = field(default_factory=list)
     last_modified: datetime | None = None
     created: datetime | None = None
```

### Comparing `ministryofjustice_data_platform_catalogue-1.0.0/pyproject.toml` & `ministryofjustice_data_platform_catalogue-1.0.1/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -6,25 +6,24 @@
 profile = "black"
 
 [tool.pylint]
 max-line-length = 120
 
 [tool.poetry]
 name = "ministryofjustice-data-platform-catalogue"
-version = "1.0.0"
-description = "Library to integrate the MoJ data platform with the catalogue component."
+version = "1.0.1"
+description = "Wrapper around Datahub supporting custom properties for the Find MOJ Data service."
 authors = ["MoJ Data Platform Team <data-platform-tech@digital.justice.gov.uk>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "data_platform_catalogue" }]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 acryl-datahub = { extras = ["datahub-rest"], version = "^0.12.1.3" }
 freezegun = "^1.4.0"
 deepdiff = "^6.7.1"
-pydantic = "2"
+pydantic = "^2.7.1"
 
 [tool.poetry.group.dev.dependencies]
 requests-mock = "^1.11.0"
 pytest = "^7.4.2"
-
```

