# Comparing `tmp/xsdata-24.4.tar.gz` & `tmp/xsdata-24.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xsdata-24.4.tar", last modified: Mon Apr  1 05:14:15 2024, max compression
+gzip compressed data, was "xsdata-24.5.tar", last modified: Tue May  7 16:28:25 2024, max compression
```

## Comparing `xsdata-24.4.tar` & `xsdata-24.5.tar`

### file list

```diff
@@ -1,517 +1,515 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 05:14:15.484624 xsdata-24.4/
--rw-r--r--   0 runner    (1001) docker     (127)    37903 2024-04-01 05:14:11.000000 xsdata-24.4/CHANGES.md
--rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-04-01 05:14:11.000000 xsdata-24.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-01 05:14:11.000000 xsdata-24.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6963 2024-04-01 05:14:15.484624 xsdata-24.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4474 2024-04-01 05:14:11.000000 xsdata-24.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 05:14:15.412624 xsdata-24.4/docs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 05:14:11.000000 xsdata-24.4/docs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 05:14:15.412624 xsdata-24.4/docs/api/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 05:14:11.000000 xsdata-24.4/docs/api/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-01 05:14:11.000000 xsdata-24.4/docs/changelog.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 05:14:15.412624 xsdata-24.4/docs/codegen/
--rw-r--r--   0 runner    (1001) docker     (127)     5122 2024-04-01 05:14:11.000000 xsdata-24.4/docs/codegen/architecture.md
--rw-r--r--   0 runner    (1001) docker     (127)    11393 2024-04-01 05:14:11.000000 xsdata-24.4/docs/codegen/config.md
--rw-r--r--   0 runner    (1001) docker     (127)      838 2024-04-01 05:14:11.000000 xsdata-24.4/docs/codegen/docstrings.md
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-04-01 05:14:11.000000 xsdata-24.4/docs/codegen/download_schemas.md
--rw-r--r--   0 runner    (1001) docker     (127)      608 2024-04-01 05:14:11.000000 xsdata-24.4/docs/codegen/dtd_modeling.md
--rw-r--r--   0 runner    (1001) docker     (127)      912 2024-04-01 05:14:11.000000 xsdata-24.4/docs/codegen/intro.md
--rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-04-01 05:14:11.000000 xsdata-24.4/docs/codegen/samples_modeling.md
--rw-r--r--   0 runner    (1001) docker     (127)     4090 2024-04-01 05:14:11.000000 xsdata-24.4/docs/codegen/wsdl_modeling.md
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-01 05:14:11.000000 xsdata-24.4/docs/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 05:14:15.412624 xsdata-24.4/docs/data_binding/
--rw-r--r--   0 runner    (1001) docker     (127)     7201 2024-04-01 05:14:11.000000 xsdata-24.4/docs/data_binding/basics.md
--rw-r--r--   0 runner    (1001) docker     (127)     1763 2024-04-01 05:14:11.000000 xsdata-24.4/docs/data_binding/dict_decoding.md
--rw-r--r--   0 runner    (1001) docker     (127)     1798 2024-04-01 05:14:11.000000 xsdata-24.4/docs/data_binding/dict_encoding.md
--rw-r--r--   0 runner    (1001) docker     (127)     4320 2024-04-01 05:14:11.000000 xsdata-24.4/docs/data_binding/json_parsing.md
--rw-r--r--   0 runner    (1001) docker     (127)     3459 2024-04-01 05:14:11.000000 xsdata-24.4/docs/data_binding/json_serializing.md
--rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-04-01 05:14:11.000000 xsdata-24.4/docs/data_binding/pycode_serializing.md
--rw-r--r--   0 runner    (1001) docker     (127)     1612 2024-04-01 05:14:11.000000 xsdata-24.4/docs/data_binding/tree_serializing.md
--rw-r--r--   0 runner    (1001) docker     (127)     5384 2024-04-01 05:14:11.000000 xsdata-24.4/docs/data_binding/xml_parsing.md
--rw-r--r--   0 runner    (1001) docker     (127)     8281 2024-04-01 05:14:11.000000 xsdata-24.4/docs/data_binding/xml_serializing.md
--rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-04-01 05:14:11.000000 xsdata-24.4/docs/faq.md
--rw-r--r--   0 runner    (1001) docker     (127)      342 2024-04-01 05:14:11.000000 xsdata-24.4/docs/favicon.png
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-04-01 05:14:11.000000 xsdata-24.4/docs/hooks.py
--rw-r--r--   0 runner    (1001) docker     (127)      470 2024-04-01 05:14:11.000000 xsdata-24.4/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-04-01 05:14:11.000000 xsdata-24.4/docs/installation.md
--rw-r--r--   0 runner    (1001) docker     (127)      792 2024-04-01 05:14:11.000000 xsdata-24.4/docs/logo-small.svg
--rw-r--r--   0 runner    (1001) docker     (127)     3535 2024-04-01 05:14:11.000000 xsdata-24.4/docs/logo.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 05:14:15.416624 xsdata-24.4/docs/models/
--rw-r--r--   0 runner    (1001) docker     (127)     3286 2024-04-01 05:14:11.000000 xsdata-24.4/docs/models/classes.md
--rw-r--r--   0 runner    (1001) docker     (127)    10287 2024-04-01 05:14:11.000000 xsdata-24.4/docs/models/fields.md
--rw-r--r--   0 runner    (1001) docker     (127)    11189 2024-04-01 05:14:11.000000 xsdata-24.4/docs/models/types.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 05:14:15.416624 xsdata-24.4/docs/overrides/
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-04-01 05:14:11.000000 xsdata-24.4/docs/overrides/main.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 05:14:15.416624 xsdata-24.4/docs/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-04-01 05:14:11.000000 xsdata-24.4/docs/plugins/how_to.md
--rw-r--r--   0 runner    (1001) docker     (127)      774 2024-04-01 05:14:11.000000 xsdata-24.4/docs/plugins/list.md
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-01 05:14:11.000000 xsdata-24.4/docs/robots.txt
--rw-r--r--   0 runner    (1001) docker     (127)      771 2024-04-01 05:14:11.000000 xsdata-24.4/docs/samples.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 05:14:15.416624 xsdata-24.4/docs/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 05:14:11.000000 xsdata-24.4/docs/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      788 2024-04-01 05:14:11.000000 xsdata-24.4/docs/scripts/generate_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     3369 2024-04-01 05:14:11.000000 xsdata-24.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 05:14:15.484624 xsdata-24.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 05:14:15.416624 xsdata-24.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-01 05:14:11.000000 xsdata-24.4/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 05:14:15.416624 xsdata-24.4/tests/codegen/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 05:14:11.000000 xsdata-24.4/tests/codegen/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 05:14:15.424624 xsdata-24.4/tests/codegen/handlers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 05:14:11.000000 xsdata-24.4/tests/codegen/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5685 2024-04-01 05:14:11.000000 xsdata-24.4/tests/codegen/handlers/test_add_attribute_substitutions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3768 2024-04-01 05:14:11.000000 xsdata-24.4/tests/codegen/handlers/test_calculate_attribute_paths.py
--rw-r--r--   0 runner    (1001) docker     (127)    11132 2024-04-01 05:14:11.000000 xsdata-24.4/tests/codegen/handlers/test_create_compound_fields.py
--rw-r--r--   0 runner    (1001) docker     (127)     4403 2024-04-01 05:14:11.000000 xsdata-24.4/tests/codegen/handlers/test_create_wrapper_fields.py
--rw-r--r--   0 runner    (1001) docker     (127)     8158 2024-04-01 05:14:11.000000 xsdata-24.4/tests/codegen/handlers/test_designate_class_packages.py
--rw-r--r--   0 runner    (1001) docker     (127)     2590 2024-04-01 05:14:11.000000 xsdata-24.4/tests/codegen/handlers/test_detect_circular_references.py
--rw-r--r--   0 runner    (1001) docker     (127)     9496 2024-04-01 05:14:11.000000 xsdata-24.4/tests/codegen/handlers/test_disambiguate_choices.py
--rw-r--r--   0 runner    (1001) docker     (127)     1600 2024-04-01 05:14:11.000000 xsdata-24.4/tests/codegen/handlers/test_filter_classes.py
--rw-r--r--   0 runner    (1001) docker     (127)     3684 2024-04-01 05:14:11.000000 xsdata-24.4/tests/codegen/handlers/test_flatten_attribute_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)    20025 2024-04-01 05:14:11.000000 xsdata-24.4/tests/codegen/handlers/test_flatten_class_extensions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3013 2024-04-01 05:14:11.000000 xsdata-24.4/tests/codegen/handlers/test_merge_attributes.py
--rw-r--r--   0 runner    (1001) docker     (127)    16126 2024-04-01 05:14:11.000000 xsdata-24.4/tests/codegen/handlers/test_process_attributes_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-04-01 05:14:11.000000 xsdata-24.4/tests/codegen/handlers/test_process_mixed_content_class.py
--rw-r--r--   0 runner    (1001) docker     (127)      633 2024-04-01 05:14:11.000000 xsdata-24.4/tests/codegen/handlers/test_rename_duplicate_attributes.py
--rw-r--r--   0 runner    (1001) docker     (127)     6663 2024-04-01 05:14:11.000000 xsdata-24.4/tests/codegen/handlers/test_rename_duplicate_classes.py
--rw-r--r--   0 runner    (1001) docker     (127)     2975 2024-04-01 05:14:11.000000 xsdata-24.4/tests/codegen/handlers/test_reset_attribute_sequence_numbers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2449 2024-04-01 05:14:11.000000 xsdata-24.4/tests/codegen/handlers/test_reset_attribute_sequences.py
--rw-r--r--   0 runner    (1001) docker     (127)    12009 2024-04-01 05:14:11.000000 xsdata-24.4/tests/codegen/handlers/test_sanitize_attributes_default_value.py
--rw-r--r--   0 runner    (1001) docker     (127)     2699 2024-04-01 05:14:11.000000 xsdata-24.4/tests/codegen/handlers/test_sanitize_enumeration_class.py
--rw-r--r--   0 runner    (1001) docker     (127)     4785 2024-04-01 05:14:11.000000 xsdata-24.4/tests/codegen/handlers/test_unnest_inner_classes.py
--rw-r--r--   0 runner    (1001) docker     (127)     4441 2024-04-01 05:14:11.000000 xsdata-24.4/tests/codegen/handlers/test_update_attributes_effective_choice.py
--rw-r--r--   0 runner    (1001) docker     (127)     4678 2024-04-01 05:14:11.000000 xsdata-24.4/tests/codegen/handlers/test_vacuum_inner_classes.py
--rw-r--r--   0 runner    (1001) docker     (127)     7657 2024-04-01 05:14:11.000000 xsdata-24.4/tests/codegen/handlers/test_validate_attributes_overrides.py
--rw-r--r--   0 runner    (1001) docker     (127)     1966 2024-04-01 05:14:11.000000 xsdata-24.4/tests/codegen/handlers/test_validate_references.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 05:14:15.424624 xsdata-24.4/tests/codegen/mappers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 05:14:11.000000 xsdata-24.4/tests/codegen/mappers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    29219 2024-04-01 05:14:11.000000 xsdata-24.4/tests/codegen/mappers/test_definitions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3987 2024-04-01 05:14:11.000000 xsdata-24.4/tests/codegen/mappers/test_dict.py
--rw-r--r--   0 runner    (1001) docker     (127)    15038 2024-04-01 05:14:11.000000 xsdata-24.4/tests/codegen/mappers/test_dtd.py
--rw-r--r--   0 runner    (1001) docker     (127)    11922 2024-04-01 05:14:11.000000 xsdata-24.4/tests/codegen/mappers/test_element.py
--rw-r--r--   0 runner    (1001) docker     (127)    16997 2024-04-01 05:14:11.000000 xsdata-24.4/tests/codegen/mappers/test_schema.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 05:14:15.424624 xsdata-24.4/tests/codegen/models/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 05:14:11.000000 xsdata-24.4/tests/codegen/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6918 2024-04-01 05:14:11.000000 xsdata-24.4/tests/codegen/models/test_attr.py
--rw-r--r--   0 runner    (1001) docker     (127)      647 2024-04-01 05:14:11.000000 xsdata-24.4/tests/codegen/models/test_attr_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     7059 2024-04-01 05:14:11.000000 xsdata-24.4/tests/codegen/models/test_class.py
--rw-r--r--   0 runner    (1001) docker     (127)      854 2024-04-01 05:14:11.000000 xsdata-24.4/tests/codegen/models/test_codegen.py
--rw-r--r--   0 runner    (1001) docker     (127)     4340 2024-04-01 05:14:11.000000 xsdata-24.4/tests/codegen/models/test_restrictions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 05:14:15.424624 xsdata-24.4/tests/codegen/parsers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 05:14:11.000000 xsdata-24.4/tests/codegen/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-01 05:14:11.000000 xsdata-24.4/tests/codegen/parsers/test_definitions.py
--rw-r--r--   0 runner    (1001) docker     (127)     6478 2024-04-01 05:14:11.000000 xsdata-24.4/tests/codegen/parsers/test_dtd.py
--rw-r--r--   0 runner    (1001) docker     (127)    15693 2024-04-01 05:14:11.000000 xsdata-24.4/tests/codegen/parsers/test_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     6088 2024-04-01 05:14:11.000000 xsdata-24.4/tests/codegen/test_container.py
--rw-r--r--   0 runner    (1001) docker     (127)     8862 2024-04-01 05:14:11.000000 xsdata-24.4/tests/codegen/test_resolver.py
--rw-r--r--   0 runner    (1001) docker     (127)    19437 2024-04-01 05:14:11.000000 xsdata-24.4/tests/codegen/test_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)    15138 2024-04-01 05:14:11.000000 xsdata-24.4/tests/codegen/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6657 2024-04-01 05:14:11.000000 xsdata-24.4/tests/codegen/test_validator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3112 2024-04-01 05:14:11.000000 xsdata-24.4/tests/codegen/test_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1500 2024-04-01 05:14:11.000000 xsdata-24.4/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 05:14:15.428624 xsdata-24.4/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 05:14:11.000000 xsdata-24.4/tests/fixtures/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 05:14:15.428624 xsdata-24.4/tests/fixtures/annotations/
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-01 05:14:11.000000 xsdata-24.4/tests/fixtures/annotations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      596 2024-04-01 05:14:11.000000 xsdata-24.4/tests/fixtures/annotations/model.py
--rw-r--r--   0 runner    (1001) docker     (127)      580 2024-04-01 05:14:11.000000 xsdata-24.4/tests/fixtures/annotations/model.xsd
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-01 05:14:11.000000 xsdata-24.4/tests/fixtures/annotations/sample.xml
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-01 05:14:11.000000 xsdata-24.4/tests/fixtures/annotations/units.py
--rw-r--r--   0 runner    (1001) docker     (127)      660 2024-04-01 05:14:11.000000 xsdata-24.4/tests/fixtures/annotations/units.xsd
--rw-r--r--   0 runner    (1001) docker     (127)      950 2024-04-01 05:14:11.000000 xsdata-24.4/tests/fixtures/annotations/xsdata.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 05:14:15.428624 xsdata-24.4/tests/fixtures/artists/
--rw-r--r--   0 runner    (1001) docker     (127)      463 2024-04-01 05:14:11.000000 xsdata-24.4/tests/fixtures/artists/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4517 2024-04-01 05:14:11.000000 xsdata-24.4/tests/fixtures/artists/art001.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-04-01 05:14:11.000000 xsdata-24.4/tests/fixtures/artists/art002.xml
--rw-r--r--   0 runner    (1001) docker     (127)     2629 2024-04-01 05:14:11.000000 xsdata-24.4/tests/fixtures/artists/art003.xml
--rw-r--r--   0 runner    (1001) docker     (127)     9232 2024-04-01 05:14:11.000000 xsdata-24.4/tests/fixtures/artists/metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 05:14:15.432624 xsdata-24.4/tests/fixtures/books/
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-01 05:14:11.000000 xsdata-24.4/tests/fixtures/books/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-01 05:14:11.000000 xsdata-24.4/tests/fixtures/books/bk001.xml
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-04-01 05:14:11.000000 xsdata-24.4/tests/fixtures/books/bk002.xml
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-01 05:14:11.000000 xsdata-24.4/tests/fixtures/books/books-xinclude.xml
--rw-r--r--   0 runner    (1001) docker     (127)      485 2024-04-01 05:14:11.000000 xsdata-24.4/tests/fixtures/books/books.json
--rw-r--r--   0 runner    (1001) docker     (127)     2184 2024-04-01 05:14:11.000000 xsdata-24.4/tests/fixtures/books/books.py
--rw-r--r--   0 runner    (1001) docker     (127)      602 2024-04-01 05:14:11.000000 xsdata-24.4/tests/fixtures/books/books.xml
--rw-r--r--   0 runner    (1001) docker     (127)      602 2024-04-01 05:14:11.000000 xsdata-24.4/tests/fixtures/books/books_auto_ns.xml
--rw-r--r--   0 runner    (1001) docker     (127)      608 2024-04-01 05:14:11.000000 xsdata-24.4/tests/fixtures/books/books_default_ns.xml
--rw-r--r--   0 runner    (1001) docker     (127)     3842 2024-04-01 05:14:11.000000 xsdata-24.4/tests/fixtures/books/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (127)     2405 2024-04-01 05:14:11.000000 xsdata-24.4/tests/fixtures/books/schema.xsd
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 05:14:15.432624 xsdata-24.4/tests/fixtures/calculator/
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-04-01 05:14:11.000000 xsdata-24.4/tests/fixtures/calculator/AddRQ.xml
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-01 05:14:11.000000 xsdata-24.4/tests/fixtures/calculator/AddRS.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-01 05:14:11.000000 xsdata-24.4/tests/fixtures/calculator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13579 2024-04-01 05:14:11.000000 xsdata-24.4/tests/fixtures/calculator/services.py
--rw-r--r--   0 runner    (1001) docker     (127)     7880 2024-04-01 05:14:11.000000 xsdata-24.4/tests/fixtures/calculator/services.wsdl
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 05:14:15.432624 xsdata-24.4/tests/fixtures/compound/
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-01 05:14:11.000000 xsdata-24.4/tests/fixtures/compound/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1198 2024-04-01 05:14:11.000000 xsdata-24.4/tests/fixtures/compound/models.py
--rw-r--r--   0 runner    (1001) docker     (127)      361 2024-04-01 05:14:11.000000 xsdata-24.4/tests/fixtures/compound/sample.json
--rw-r--r--   0 runner    (1001) docker     (127)      560 2024-04-01 05:14:11.000000 xsdata-24.4/tests/fixtures/compound/sample.py
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-01 05:14:11.000000 xsdata-24.4/tests/fixtures/compound/sample.xml
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-04-01 05:14:11.000000 xsdata-24.4/tests/fixtures/compound/sample.xsdata.xml
--rw-r--r--   0 runner    (1001) docker     (127)      844 2024-04-01 05:14:11.000000 xsdata-24.4/tests/fixtures/compound/schema.xsd
--rw-r--r--   0 runner    (1001) docker     (127)      680 2024-04-01 05:14:11.000000 xsdata-24.4/tests/fixtures/datatypes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 05:14:15.432624 xsdata-24.4/tests/fixtures/docstrings/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 05:14:11.000000 xsdata-24.4/tests/fixtures/docstrings/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 05:14:15.432624 xsdata-24.4/tests/fixtures/docstrings/accessible/
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-01 05:14:11.000000 xsdata-24.4/tests/fixtures/docstrings/accessible/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2931 2024-04-01 05:14:11.000000 xsdata-24.4/tests/fixtures/docstrings/accessible/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 05:14:15.432624 xsdata-24.4/tests/fixtures/docstrings/blank/
--rw-r--r--   0 runner    (1001) docker     (127)      282 2024-04-01 05:14:11.000000 xsdata-24.4/tests/fixtures/docstrings/blank/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-04-01 05:14:11.000000 xsdata-24.4/tests/fixtures/docstrings/blank/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 05:14:15.436624 xsdata-24.4/tests/fixtures/docstrings/google/
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-04-01 05:14:11.000000 xsdata-24.4/tests/fixtures/docstrings/google/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2871 2024-04-01 05:14:11.000000 xsdata-24.4/tests/fixtures/docstrings/google/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 05:14:15.436624 xsdata-24.4/tests/fixtures/docstrings/numpy/
--rw-r--r--   0 runner    (1001) docker     (127)      282 2024-04-01 05:14:11.000000 xsdata-24.4/tests/fixtures/docstrings/numpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2914 2024-04-01 05:14:11.000000 xsdata-24.4/tests/fixtures/docstrings/numpy/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 05:14:15.436624 xsdata-24.4/tests/fixtures/docstrings/rst/
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-01 05:14:11.000000 xsdata-24.4/tests/fixtures/docstrings/rst/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2797 2024-04-01 05:14:11.000000 xsdata-24.4/tests/fixtures/docstrings/rst/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     4081 2024-04-01 05:14:11.000000 xsdata-24.4/tests/fixtures/docstrings/schema.xsd
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 05:14:15.436624 xsdata-24.4/tests/fixtures/dtd/
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-01 05:14:11.000000 xsdata-24.4/tests/fixtures/dtd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      400 2024-04-01 05:14:11.000000 xsdata-24.4/tests/fixtures/dtd/complete_example.dtd
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-01 05:14:11.000000 xsdata-24.4/tests/fixtures/dtd/default_namespace.dtd
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 05:14:15.436624 xsdata-24.4/tests/fixtures/dtd/models/
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-04-01 05:14:11.000000 xsdata-24.4/tests/fixtures/dtd/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2819 2024-04-01 05:14:11.000000 xsdata-24.4/tests/fixtures/dtd/models/complete_example.py
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-01 05:14:11.000000 xsdata-24.4/tests/fixtures/dtd/prefix_namespace.dtd
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 05:14:15.436624 xsdata-24.4/tests/fixtures/hello/
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-01 05:14:11.000000 xsdata-24.4/tests/fixtures/hello/HelloRQ.xml
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-01 05:14:11.000000 xsdata-24.4/tests/fixtures/hello/HelloRS.xml
--rw-r--r--   0 runner    (1001) docker     (127)      489 2024-04-01 05:14:11.000000 xsdata-24.4/tests/fixtures/hello/HelloRS_SoapFault.xml
--rw-r--r--   0 runner    (1001) docker     (127)      430 2024-04-01 05:14:11.000000 xsdata-24.4/tests/fixtures/hello/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4612 2024-04-01 05:14:11.000000 xsdata-24.4/tests/fixtures/hello/hello.py
--rw-r--r--   0 runner    (1001) docker     (127)     3084 2024-04-01 05:14:11.000000 xsdata-24.4/tests/fixtures/hello/hello.wsdl
--rw-r--r--   0 runner    (1001) docker     (127)      781 2024-04-01 05:14:11.000000 xsdata-24.4/tests/fixtures/hello/hello.xsd
--rw-r--r--   0 runner    (1001) docker     (127)     4760 2024-04-01 05:14:11.000000 xsdata-24.4/tests/fixtures/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 05:14:15.436624 xsdata-24.4/tests/fixtures/primer/
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-04-01 05:14:11.000000 xsdata-24.4/tests/fixtures/primer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4624 2024-04-01 05:14:11.000000 xsdata-24.4/tests/fixtures/primer/order.py
--rw-r--r--   0 runner    (1001) docker     (127)     3032 2024-04-01 05:14:11.000000 xsdata-24.4/tests/fixtures/primer/order.xsd
--rw-r--r--   0 runner    (1001) docker     (127)      890 2024-04-01 05:14:11.000000 xsdata-24.4/tests/fixtures/primer/sample.json
--rw-r--r--   0 runner    (1001) docker     (127)     1315 2024-04-01 05:14:11.000000 xsdata-24.4/tests/fixtures/primer/sample.py
--rw-r--r--   0 runner    (1001) docker     (127)      881 2024-04-01 05:14:11.000000 xsdata-24.4/tests/fixtures/primer/sample.xml
--rw-r--r--   0 runner    (1001) docker     (127)      889 2024-04-01 05:14:11.000000 xsdata-24.4/tests/fixtures/primer/sample.xsdata.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 05:14:15.440624 xsdata-24.4/tests/fixtures/series/
--rw-r--r--   0 runner    (1001) docker     (127)      344 2024-04-01 05:14:11.000000 xsdata-24.4/tests/fixtures/series/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 05:14:15.440624 xsdata-24.4/tests/fixtures/series/samples/
--rw-r--r--   0 runner    (1001) docker     (127)     1263 2024-04-01 05:14:11.000000 xsdata-24.4/tests/fixtures/series/samples/show1.json
--rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-04-01 05:14:11.000000 xsdata-24.4/tests/fixtures/series/samples/show2.json
--rw-r--r--   0 runner    (1001) docker     (127)     6665 2024-04-01 05:14:11.000000 xsdata-24.4/tests/fixtures/series/series.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 05:14:15.440624 xsdata-24.4/tests/fixtures/stripe/
--rw-r--r--   0 runner    (1001) docker     (127)      931 2024-04-01 05:14:11.000000 xsdata-24.4/tests/fixtures/stripe/.xsdata.xml
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 05:14:11.000000 xsdata-24.4/tests/fixtures/stripe/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 05:14:15.440624 xsdata-24.4/tests/fixtures/stripe/models/
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-04-01 05:14:11.000000 xsdata-24.4/tests/fixtures/stripe/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3034 2024-04-01 05:14:11.000000 xsdata-24.4/tests/fixtures/stripe/models/balance.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 05:14:15.440624 xsdata-24.4/tests/fixtures/stripe/samples/
--rw-r--r--   0 runner    (1001) docker     (127)     2628 2024-04-01 05:14:11.000000 xsdata-24.4/tests/fixtures/stripe/samples/balance.json
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-01 05:14:11.000000 xsdata-24.4/tests/fixtures/submodels.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 05:14:15.440624 xsdata-24.4/tests/fixtures/typemapping/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 05:14:11.000000 xsdata-24.4/tests/fixtures/typemapping/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-04-01 05:14:11.000000 xsdata-24.4/tests/fixtures/typemapping/city.py
--rw-r--r--   0 runner    (1001) docker     (127)      278 2024-04-01 05:14:11.000000 xsdata-24.4/tests/fixtures/typemapping/house.py
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-04-01 05:14:11.000000 xsdata-24.4/tests/fixtures/typemapping/street.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 05:14:15.440624 xsdata-24.4/tests/fixtures/wrapper/
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-01 05:14:11.000000 xsdata-24.4/tests/fixtures/wrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1874 2024-04-01 05:14:11.000000 xsdata-24.4/tests/fixtures/wrapper/models.py
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-01 05:14:11.000000 xsdata-24.4/tests/fixtures/wrapper/sample.json
--rw-r--r--   0 runner    (1001) docker     (127)      353 2024-04-01 05:14:11.000000 xsdata-24.4/tests/fixtures/wrapper/sample.py
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-04-01 05:14:11.000000 xsdata-24.4/tests/fixtures/wrapper/sample.xml
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-04-01 05:14:11.000000 xsdata-24.4/tests/fixtures/wrapper/sample.xsdata.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1482 2024-04-01 05:14:11.000000 xsdata-24.4/tests/fixtures/wrapper/schema.xsd
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 05:14:15.440624 xsdata-24.4/tests/formats/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 05:14:11.000000 xsdata-24.4/tests/formats/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 05:14:15.444624 xsdata-24.4/tests/formats/dataclass/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 05:14:11.000000 xsdata-24.4/tests/formats/dataclass/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 05:14:15.444624 xsdata-24.4/tests/formats/dataclass/models/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 05:14:11.000000 xsdata-24.4/tests/formats/dataclass/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17171 2024-04-01 05:14:11.000000 xsdata-24.4/tests/formats/dataclass/models/test_builders.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 05:14:15.444624 xsdata-24.4/tests/formats/dataclass/parsers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 05:14:11.000000 xsdata-24.4/tests/formats/dataclass/parsers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 05:14:15.444624 xsdata-24.4/tests/formats/dataclass/parsers/handlers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 05:14:11.000000 xsdata-24.4/tests/formats/dataclass/parsers/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2755 2024-04-01 05:14:11.000000 xsdata-24.4/tests/formats/dataclass/parsers/handlers/test_lxml.py
--rw-r--r--   0 runner    (1001) docker     (127)     3179 2024-04-01 05:14:11.000000 xsdata-24.4/tests/formats/dataclass/parsers/handlers/test_native.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 05:14:15.448624 xsdata-24.4/tests/formats/dataclass/parsers/nodes/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 05:14:11.000000 xsdata-24.4/tests/formats/dataclass/parsers/nodes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19744 2024-04-01 05:14:11.000000 xsdata-24.4/tests/formats/dataclass/parsers/nodes/test_element.py
--rw-r--r--   0 runner    (1001) docker     (127)     3064 2024-04-01 05:14:11.000000 xsdata-24.4/tests/formats/dataclass/parsers/nodes/test_primitive.py
--rw-r--r--   0 runner    (1001) docker     (127)      377 2024-04-01 05:14:11.000000 xsdata-24.4/tests/formats/dataclass/parsers/nodes/test_skip.py
--rw-r--r--   0 runner    (1001) docker     (127)     1676 2024-04-01 05:14:11.000000 xsdata-24.4/tests/formats/dataclass/parsers/nodes/test_standard.py
--rw-r--r--   0 runner    (1001) docker     (127)     3960 2024-04-01 05:14:11.000000 xsdata-24.4/tests/formats/dataclass/parsers/nodes/test_union.py
--rw-r--r--   0 runner    (1001) docker     (127)     2221 2024-04-01 05:14:11.000000 xsdata-24.4/tests/formats/dataclass/parsers/nodes/test_wildcard.py
--rw-r--r--   0 runner    (1001) docker     (127)     2757 2024-04-01 05:14:11.000000 xsdata-24.4/tests/formats/dataclass/parsers/nodes/test_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)    14258 2024-04-01 05:14:11.000000 xsdata-24.4/tests/formats/dataclass/parsers/test_dict.py
--rw-r--r--   0 runner    (1001) docker     (127)      815 2024-04-01 05:14:11.000000 xsdata-24.4/tests/formats/dataclass/parsers/test_json.py
--rw-r--r--   0 runner    (1001) docker     (127)     1172 2024-04-01 05:14:11.000000 xsdata-24.4/tests/formats/dataclass/parsers/test_mixins.py
--rw-r--r--   0 runner    (1001) docker     (127)     7729 2024-04-01 05:14:11.000000 xsdata-24.4/tests/formats/dataclass/parsers/test_node.py
--rw-r--r--   0 runner    (1001) docker     (127)      981 2024-04-01 05:14:11.000000 xsdata-24.4/tests/formats/dataclass/parsers/test_tree.py
--rw-r--r--   0 runner    (1001) docker     (127)     3845 2024-04-01 05:14:11.000000 xsdata-24.4/tests/formats/dataclass/parsers/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2210 2024-04-01 05:14:11.000000 xsdata-24.4/tests/formats/dataclass/parsers/test_xml.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 05:14:15.448624 xsdata-24.4/tests/formats/dataclass/serializers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 05:14:11.000000 xsdata-24.4/tests/formats/dataclass/serializers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4106 2024-04-01 05:14:11.000000 xsdata-24.4/tests/formats/dataclass/serializers/test_code.py
--rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-04-01 05:14:11.000000 xsdata-24.4/tests/formats/dataclass/serializers/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3584 2024-04-01 05:14:11.000000 xsdata-24.4/tests/formats/dataclass/serializers/test_dict.py
--rw-r--r--   0 runner    (1001) docker     (127)     3274 2024-04-01 05:14:11.000000 xsdata-24.4/tests/formats/dataclass/serializers/test_json.py
--rw-r--r--   0 runner    (1001) docker     (127)    30343 2024-04-01 05:14:11.000000 xsdata-24.4/tests/formats/dataclass/serializers/test_mixins.py
--rw-r--r--   0 runner    (1001) docker     (127)     1490 2024-04-01 05:14:11.000000 xsdata-24.4/tests/formats/dataclass/serializers/test_xml.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 05:14:15.448624 xsdata-24.4/tests/formats/dataclass/serializers/tree/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 05:14:11.000000 xsdata-24.4/tests/formats/dataclass/serializers/tree/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-04-01 05:14:11.000000 xsdata-24.4/tests/formats/dataclass/serializers/tree/test_lxml.py
--rw-r--r--   0 runner    (1001) docker     (127)      728 2024-04-01 05:14:11.000000 xsdata-24.4/tests/formats/dataclass/serializers/tree/test_mixins.py
--rw-r--r--   0 runner    (1001) docker     (127)     1410 2024-04-01 05:14:11.000000 xsdata-24.4/tests/formats/dataclass/serializers/tree/test_native.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 05:14:15.448624 xsdata-24.4/tests/formats/dataclass/serializers/writers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 05:14:11.000000 xsdata-24.4/tests/formats/dataclass/serializers/writers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2408 2024-04-01 05:14:11.000000 xsdata-24.4/tests/formats/dataclass/serializers/writers/test_lxml.py
--rw-r--r--   0 runner    (1001) docker     (127)     2299 2024-04-01 05:14:11.000000 xsdata-24.4/tests/formats/dataclass/serializers/writers/test_native.py
--rw-r--r--   0 runner    (1001) docker     (127)     5542 2024-04-01 05:14:11.000000 xsdata-24.4/tests/formats/dataclass/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-04-01 05:14:11.000000 xsdata-24.4/tests/formats/dataclass/test_compat.py
--rw-r--r--   0 runner    (1001) docker     (127)     5501 2024-04-01 05:14:11.000000 xsdata-24.4/tests/formats/dataclass/test_context.py
--rw-r--r--   0 runner    (1001) docker     (127)     9303 2024-04-01 05:14:11.000000 xsdata-24.4/tests/formats/dataclass/test_elements.py
--rw-r--r--   0 runner    (1001) docker     (127)    42646 2024-04-01 05:14:11.000000 xsdata-24.4/tests/formats/dataclass/test_filters.py
--rw-r--r--   0 runner    (1001) docker     (127)     9091 2024-04-01 05:14:11.000000 xsdata-24.4/tests/formats/dataclass/test_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2639 2024-04-01 05:14:11.000000 xsdata-24.4/tests/formats/dataclass/test_transport.py
--rw-r--r--   0 runner    (1001) docker     (127)     6438 2024-04-01 05:14:11.000000 xsdata-24.4/tests/formats/dataclass/test_typing.py
--rw-r--r--   0 runner    (1001) docker     (127)    15785 2024-04-01 05:14:11.000000 xsdata-24.4/tests/formats/test_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2605 2024-04-01 05:14:11.000000 xsdata-24.4/tests/formats/test_mixins.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 05:14:15.452624 xsdata-24.4/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 05:14:11.000000 xsdata-24.4/tests/integration/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 05:14:15.452624 xsdata-24.4/tests/integration/benchmarks/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 05:14:11.000000 xsdata-24.4/tests/integration/benchmarks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      301 2024-04-01 05:14:11.000000 xsdata-24.4/tests/integration/benchmarks/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      774 2024-04-01 05:14:11.000000 xsdata-24.4/tests/integration/benchmarks/test_converters.py
--rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-04-01 05:14:11.000000 xsdata-24.4/tests/integration/benchmarks/test_handlers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1852 2024-04-01 05:14:11.000000 xsdata-24.4/tests/integration/benchmarks/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-01 05:14:11.000000 xsdata-24.4/tests/integration/test_annotations.py
--rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-04-01 05:14:11.000000 xsdata-24.4/tests/integration/test_artists.py
--rw-r--r--   0 runner    (1001) docker     (127)      761 2024-04-01 05:14:11.000000 xsdata-24.4/tests/integration/test_books.py
--rw-r--r--   0 runner    (1001) docker     (127)     1868 2024-04-01 05:14:11.000000 xsdata-24.4/tests/integration/test_calculator.py
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-01 05:14:11.000000 xsdata-24.4/tests/integration/test_compound.py
--rw-r--r--   0 runner    (1001) docker     (127)     1863 2024-04-01 05:14:11.000000 xsdata-24.4/tests/integration/test_docstrings.py
--rw-r--r--   0 runner    (1001) docker     (127)      561 2024-04-01 05:14:11.000000 xsdata-24.4/tests/integration/test_dtd.py
--rw-r--r--   0 runner    (1001) docker     (127)     3608 2024-04-01 05:14:11.000000 xsdata-24.4/tests/integration/test_hello_rpc.py
--rw-r--r--   0 runner    (1001) docker     (127)      673 2024-04-01 05:14:11.000000 xsdata-24.4/tests/integration/test_primer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-04-01 05:14:11.000000 xsdata-24.4/tests/integration/test_series.py
--rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-04-01 05:14:11.000000 xsdata-24.4/tests/integration/test_stripe.py
--rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-04-01 05:14:11.000000 xsdata-24.4/tests/integration/test_type_mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)      763 2024-04-01 05:14:11.000000 xsdata-24.4/tests/integration/test_wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 05:14:15.452624 xsdata-24.4/tests/models/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 05:14:11.000000 xsdata-24.4/tests/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 05:14:15.452624 xsdata-24.4/tests/models/enums/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 05:14:11.000000 xsdata-24.4/tests/models/enums/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2854 2024-04-01 05:14:11.000000 xsdata-24.4/tests/models/enums/test_datatype.py
--rw-r--r--   0 runner    (1001) docker     (127)     9622 2024-04-01 05:14:11.000000 xsdata-24.4/tests/models/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    21721 2024-04-01 05:14:11.000000 xsdata-24.4/tests/models/test_datatype.py
--rw-r--r--   0 runner    (1001) docker     (127)     5877 2024-04-01 05:14:11.000000 xsdata-24.4/tests/models/test_mixins.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 05:14:15.452624 xsdata-24.4/tests/models/wsdl/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 05:14:11.000000 xsdata-24.4/tests/models/wsdl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      670 2024-04-01 05:14:11.000000 xsdata-24.4/tests/models/wsdl/test_binding.py
--rw-r--r--   0 runner    (1001) docker     (127)     2682 2024-04-01 05:14:11.000000 xsdata-24.4/tests/models/wsdl/test_definitions.py
--rw-r--r--   0 runner    (1001) docker     (127)      438 2024-04-01 05:14:11.000000 xsdata-24.4/tests/models/wsdl/test_port_type.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 05:14:15.456624 xsdata-24.4/tests/models/xsd/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 05:14:11.000000 xsdata-24.4/tests/models/xsd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      601 2024-04-01 05:14:11.000000 xsdata-24.4/tests/models/xsd/test_all.py
--rw-r--r--   0 runner    (1001) docker     (127)      722 2024-04-01 05:14:11.000000 xsdata-24.4/tests/models/xsd/test_alternative.py
--rw-r--r--   0 runner    (1001) docker     (127)     1353 2024-04-01 05:14:11.000000 xsdata-24.4/tests/models/xsd/test_annotation_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-04-01 05:14:11.000000 xsdata-24.4/tests/models/xsd/test_any.py
--rw-r--r--   0 runner    (1001) docker     (127)     1380 2024-04-01 05:14:11.000000 xsdata-24.4/tests/models/xsd/test_any_attribute.py
--rw-r--r--   0 runner    (1001) docker     (127)     2467 2024-04-01 05:14:11.000000 xsdata-24.4/tests/models/xsd/test_attribute.py
--rw-r--r--   0 runner    (1001) docker     (127)      432 2024-04-01 05:14:11.000000 xsdata-24.4/tests/models/xsd/test_attribute_group.py
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-01 05:14:11.000000 xsdata-24.4/tests/models/xsd/test_choice.py
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-01 05:14:11.000000 xsdata-24.4/tests/models/xsd/test_complex_content.py
--rw-r--r--   0 runner    (1001) docker     (127)      504 2024-04-01 05:14:11.000000 xsdata-24.4/tests/models/xsd/test_complex_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     3654 2024-04-01 05:14:11.000000 xsdata-24.4/tests/models/xsd/test_element.py
--rw-r--r--   0 runner    (1001) docker     (127)      691 2024-04-01 05:14:11.000000 xsdata-24.4/tests/models/xsd/test_enumeration.py
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-04-01 05:14:11.000000 xsdata-24.4/tests/models/xsd/test_extension.py
--rw-r--r--   0 runner    (1001) docker     (127)      911 2024-04-01 05:14:11.000000 xsdata-24.4/tests/models/xsd/test_group.py
--rw-r--r--   0 runner    (1001) docker     (127)      607 2024-04-01 05:14:11.000000 xsdata-24.4/tests/models/xsd/test_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     2803 2024-04-01 05:14:11.000000 xsdata-24.4/tests/models/xsd/test_restriction.py
--rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-04-01 05:14:11.000000 xsdata-24.4/tests/models/xsd/test_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)      626 2024-04-01 05:14:11.000000 xsdata-24.4/tests/models/xsd/test_sequence.py
--rw-r--r--   0 runner    (1001) docker     (127)     1718 2024-04-01 05:14:11.000000 xsdata-24.4/tests/models/xsd/test_simple_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     1819 2024-04-01 05:14:11.000000 xsdata-24.4/tests/models/xsd/test_union.py
--rw-r--r--   0 runner    (1001) docker     (127)     7902 2024-04-01 05:14:11.000000 xsdata-24.4/tests/test_cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 05:14:15.456624 xsdata-24.4/tests/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 05:14:11.000000 xsdata-24.4/tests/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1894 2024-04-01 05:14:11.000000 xsdata-24.4/tests/utils/test_collections.py
--rw-r--r--   0 runner    (1001) docker     (127)     4551 2024-04-01 05:14:11.000000 xsdata-24.4/tests/utils/test_dates.py
--rw-r--r--   0 runner    (1001) docker     (127)     5446 2024-04-01 05:14:11.000000 xsdata-24.4/tests/utils/test_downloader.py
--rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-04-01 05:14:11.000000 xsdata-24.4/tests/utils/test_hooks.py
--rw-r--r--   0 runner    (1001) docker     (127)     5202 2024-04-01 05:14:11.000000 xsdata-24.4/tests/utils/test_namespaces.py
--rw-r--r--   0 runner    (1001) docker     (127)      428 2024-04-01 05:14:11.000000 xsdata-24.4/tests/utils/test_objects.py
--rw-r--r--   0 runner    (1001) docker     (127)      508 2024-04-01 05:14:11.000000 xsdata-24.4/tests/utils/test_testing.py
--rw-r--r--   0 runner    (1001) docker     (127)     7816 2024-04-01 05:14:11.000000 xsdata-24.4/tests/utils/test_text.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 05:14:15.460624 xsdata-24.4/xsdata/
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-01 05:14:11.000000 xsdata-24.4/xsdata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-01 05:14:11.000000 xsdata-24.4/xsdata/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5044 2024-04-01 05:14:11.000000 xsdata-24.4/xsdata/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 05:14:15.460624 xsdata-24.4/xsdata/codegen/
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-01 05:14:11.000000 xsdata-24.4/xsdata/codegen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8927 2024-04-01 05:14:11.000000 xsdata-24.4/xsdata/codegen/container.py
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-01 05:14:11.000000 xsdata-24.4/xsdata/codegen/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 05:14:15.464624 xsdata-24.4/xsdata/codegen/handlers/
--rw-r--r--   0 runner    (1001) docker     (127)     2218 2024-04-01 05:14:11.000000 xsdata-24.4/xsdata/codegen/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4190 2024-04-01 05:14:11.000000 xsdata-24.4/xsdata/codegen/handlers/add_attribute_substitutions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2435 2024-04-01 05:14:11.000000 xsdata-24.4/xsdata/codegen/handlers/calculate_attribute_paths.py
--rw-r--r--   0 runner    (1001) docker     (127)     8570 2024-04-01 05:14:11.000000 xsdata-24.4/xsdata/codegen/handlers/create_compound_fields.py
--rw-r--r--   0 runner    (1001) docker     (127)     4322 2024-04-01 05:14:11.000000 xsdata-24.4/xsdata/codegen/handlers/create_wrapper_fields.py
--rw-r--r--   0 runner    (1001) docker     (127)     8124 2024-04-01 05:14:11.000000 xsdata-24.4/xsdata/codegen/handlers/designate_class_packages.py
--rw-r--r--   0 runner    (1001) docker     (127)     2767 2024-04-01 05:14:11.000000 xsdata-24.4/xsdata/codegen/handlers/detect_circular_references.py
--rw-r--r--   0 runner    (1001) docker     (127)     9488 2024-04-01 05:14:11.000000 xsdata-24.4/xsdata/codegen/handlers/disambiguate_choices.py
--rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-04-01 05:14:11.000000 xsdata-24.4/xsdata/codegen/handlers/filter_classes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1867 2024-04-01 05:14:11.000000 xsdata-24.4/xsdata/codegen/handlers/flatten_attribute_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)    13595 2024-04-01 05:14:11.000000 xsdata-24.4/xsdata/codegen/handlers/flatten_class_extensions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2394 2024-04-01 05:14:11.000000 xsdata-24.4/xsdata/codegen/handlers/merge_attributes.py
--rw-r--r--   0 runner    (1001) docker     (127)    10816 2024-04-01 05:14:11.000000 xsdata-24.4/xsdata/codegen/handlers/process_attributes_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     1425 2024-04-01 05:14:11.000000 xsdata-24.4/xsdata/codegen/handlers/process_mixed_content_class.py
--rw-r--r--   0 runner    (1001) docker     (127)      483 2024-04-01 05:14:11.000000 xsdata-24.4/xsdata/codegen/handlers/rename_duplicate_attributes.py
--rw-r--r--   0 runner    (1001) docker     (127)     6346 2024-04-01 05:14:11.000000 xsdata-24.4/xsdata/codegen/handlers/rename_duplicate_classes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1631 2024-04-01 05:14:11.000000 xsdata-24.4/xsdata/codegen/handlers/reset_attribute_sequence_numbers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1623 2024-04-01 05:14:11.000000 xsdata-24.4/xsdata/codegen/handlers/reset_attribute_sequences.py
--rw-r--r--   0 runner    (1001) docker     (127)     8394 2024-04-01 05:14:11.000000 xsdata-24.4/xsdata/codegen/handlers/sanitize_attributes_default_value.py
--rw-r--r--   0 runner    (1001) docker     (127)     1903 2024-04-01 05:14:11.000000 xsdata-24.4/xsdata/codegen/handlers/sanitize_enumeration_class.py
--rw-r--r--   0 runner    (1001) docker     (127)     3515 2024-04-01 05:14:11.000000 xsdata-24.4/xsdata/codegen/handlers/unnest_inner_classes.py
--rw-r--r--   0 runner    (1001) docker     (127)     4647 2024-04-01 05:14:11.000000 xsdata-24.4/xsdata/codegen/handlers/update_attributes_effective_choice.py
--rw-r--r--   0 runner    (1001) docker     (127)     3459 2024-04-01 05:14:11.000000 xsdata-24.4/xsdata/codegen/handlers/vacuum_inner_classes.py
--rw-r--r--   0 runner    (1001) docker     (127)     7071 2024-04-01 05:14:11.000000 xsdata-24.4/xsdata/codegen/handlers/validate_attributes_overrides.py
--rw-r--r--   0 runner    (1001) docker     (127)     2610 2024-04-01 05:14:11.000000 xsdata-24.4/xsdata/codegen/handlers/validate_references.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 05:14:15.468624 xsdata-24.4/xsdata/codegen/mappers/
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-04-01 05:14:11.000000 xsdata-24.4/xsdata/codegen/mappers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18286 2024-04-01 05:14:11.000000 xsdata-24.4/xsdata/codegen/mappers/definitions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2343 2024-04-01 05:14:11.000000 xsdata-24.4/xsdata/codegen/mappers/dict.py
--rw-r--r--   0 runner    (1001) docker     (127)    10812 2024-04-01 05:14:11.000000 xsdata-24.4/xsdata/codegen/mappers/dtd.py
--rw-r--r--   0 runner    (1001) docker     (127)     5748 2024-04-01 05:14:11.000000 xsdata-24.4/xsdata/codegen/mappers/element.py
--rw-r--r--   0 runner    (1001) docker     (127)     3625 2024-04-01 05:14:11.000000 xsdata-24.4/xsdata/codegen/mappers/mixins.py
--rw-r--r--   0 runner    (1001) docker     (127)    12416 2024-04-01 05:14:11.000000 xsdata-24.4/xsdata/codegen/mappers/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     4872 2024-04-01 05:14:11.000000 xsdata-24.4/xsdata/codegen/mixins.py
--rw-r--r--   0 runner    (1001) docker     (127)    25480 2024-04-01 05:14:11.000000 xsdata-24.4/xsdata/codegen/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 05:14:15.468624 xsdata-24.4/xsdata/codegen/parsers/
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-04-01 05:14:11.000000 xsdata-24.4/xsdata/codegen/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1579 2024-04-01 05:14:11.000000 xsdata-24.4/xsdata/codegen/parsers/definitions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4034 2024-04-01 05:14:11.000000 xsdata-24.4/xsdata/codegen/parsers/dtd.py
--rw-r--r--   0 runner    (1001) docker     (127)    13281 2024-04-01 05:14:11.000000 xsdata-24.4/xsdata/codegen/parsers/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     5905 2024-04-01 05:14:11.000000 xsdata-24.4/xsdata/codegen/resolver.py
--rw-r--r--   0 runner    (1001) docker     (127)      427 2024-04-01 05:14:11.000000 xsdata-24.4/xsdata/codegen/stopwatch.py
--rw-r--r--   0 runner    (1001) docker     (127)    14691 2024-04-01 05:14:11.000000 xsdata-24.4/xsdata/codegen/transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)    16189 2024-04-01 05:14:11.000000 xsdata-24.4/xsdata/codegen/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6532 2024-04-01 05:14:11.000000 xsdata-24.4/xsdata/codegen/validator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3160 2024-04-01 05:14:11.000000 xsdata-24.4/xsdata/codegen/writer.py
--rw-r--r--   0 runner    (1001) docker     (127)      668 2024-04-01 05:14:11.000000 xsdata-24.4/xsdata/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 05:14:15.468624 xsdata-24.4/xsdata/formats/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 05:14:11.000000 xsdata-24.4/xsdata/formats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24837 2024-04-01 05:14:11.000000 xsdata-24.4/xsdata/formats/converter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 05:14:15.468624 xsdata-24.4/xsdata/formats/dataclass/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 05:14:11.000000 xsdata-24.4/xsdata/formats/dataclass/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6107 2024-04-01 05:14:11.000000 xsdata-24.4/xsdata/formats/dataclass/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     5534 2024-04-01 05:14:11.000000 xsdata-24.4/xsdata/formats/dataclass/compat.py
--rw-r--r--   0 runner    (1001) docker     (127)    10591 2024-04-01 05:14:11.000000 xsdata-24.4/xsdata/formats/dataclass/context.py
--rw-r--r--   0 runner    (1001) docker     (127)    32550 2024-04-01 05:14:11.000000 xsdata-24.4/xsdata/formats/dataclass/filters.py
--rw-r--r--   0 runner    (1001) docker     (127)    10032 2024-04-01 05:14:11.000000 xsdata-24.4/xsdata/formats/dataclass/generator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 05:14:15.468624 xsdata-24.4/xsdata/formats/dataclass/models/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 05:14:11.000000 xsdata-24.4/xsdata/formats/dataclass/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21090 2024-04-01 05:14:11.000000 xsdata-24.4/xsdata/formats/dataclass/models/builders.py
--rw-r--r--   0 runner    (1001) docker     (127)    18544 2024-04-01 05:14:11.000000 xsdata-24.4/xsdata/formats/dataclass/models/elements.py
--rw-r--r--   0 runner    (1001) docker     (127)     1255 2024-04-01 05:14:11.000000 xsdata-24.4/xsdata/formats/dataclass/models/generics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 05:14:15.472624 xsdata-24.4/xsdata/formats/dataclass/parsers/
--rw-r--r--   0 runner    (1001) docker     (127)      366 2024-04-01 05:14:11.000000 xsdata-24.4/xsdata/formats/dataclass/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7457 2024-04-01 05:14:11.000000 xsdata-24.4/xsdata/formats/dataclass/parsers/bases.py
--rw-r--r--   0 runner    (1001) docker     (127)     1555 2024-04-01 05:14:11.000000 xsdata-24.4/xsdata/formats/dataclass/parsers/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    15149 2024-04-01 05:14:11.000000 xsdata-24.4/xsdata/formats/dataclass/parsers/dict.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 05:14:15.472624 xsdata-24.4/xsdata/formats/dataclass/parsers/handlers/
--rw-r--r--   0 runner    (1001) docker     (127)      629 2024-04-01 05:14:11.000000 xsdata-24.4/xsdata/formats/dataclass/parsers/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2749 2024-04-01 05:14:11.000000 xsdata-24.4/xsdata/formats/dataclass/parsers/handlers/lxml.py
--rw-r--r--   0 runner    (1001) docker     (127)     5300 2024-04-01 05:14:11.000000 xsdata-24.4/xsdata/formats/dataclass/parsers/handlers/native.py
--rw-r--r--   0 runner    (1001) docker     (127)     3207 2024-04-01 05:14:11.000000 xsdata-24.4/xsdata/formats/dataclass/parsers/json.py
--rw-r--r--   0 runner    (1001) docker     (127)     9214 2024-04-01 05:14:11.000000 xsdata-24.4/xsdata/formats/dataclass/parsers/mixins.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 05:14:15.472624 xsdata-24.4/xsdata/formats/dataclass/parsers/nodes/
--rw-r--r--   0 runner    (1001) docker     (127)      642 2024-04-01 05:14:11.000000 xsdata-24.4/xsdata/formats/dataclass/parsers/nodes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19989 2024-04-01 05:14:11.000000 xsdata-24.4/xsdata/formats/dataclass/parsers/nodes/element.py
--rw-r--r--   0 runner    (1001) docker     (127)     2195 2024-04-01 05:14:11.000000 xsdata-24.4/xsdata/formats/dataclass/parsers/nodes/primitive.py
--rw-r--r--   0 runner    (1001) docker     (127)      613 2024-04-01 05:14:11.000000 xsdata-24.4/xsdata/formats/dataclass/parsers/nodes/skip.py
--rw-r--r--   0 runner    (1001) docker     (127)     2357 2024-04-01 05:14:11.000000 xsdata-24.4/xsdata/formats/dataclass/parsers/nodes/standard.py
--rw-r--r--   0 runner    (1001) docker     (127)     5715 2024-04-01 05:14:11.000000 xsdata-24.4/xsdata/formats/dataclass/parsers/nodes/union.py
--rw-r--r--   0 runner    (1001) docker     (127)     4003 2024-04-01 05:14:11.000000 xsdata-24.4/xsdata/formats/dataclass/parsers/nodes/wildcard.py
--rw-r--r--   0 runner    (1001) docker     (127)     1711 2024-04-01 05:14:11.000000 xsdata-24.4/xsdata/formats/dataclass/parsers/nodes/wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     2435 2024-04-01 05:14:11.000000 xsdata-24.4/xsdata/formats/dataclass/parsers/tree.py
--rw-r--r--   0 runner    (1001) docker     (127)     5079 2024-04-01 05:14:11.000000 xsdata-24.4/xsdata/formats/dataclass/parsers/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3927 2024-04-01 05:14:11.000000 xsdata-24.4/xsdata/formats/dataclass/parsers/xml.py
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-01 05:14:11.000000 xsdata-24.4/xsdata/formats/dataclass/ruff.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 05:14:15.476624 xsdata-24.4/xsdata/formats/dataclass/serializers/
--rw-r--r--   0 runner    (1001) docker     (127)      684 2024-04-01 05:14:11.000000 xsdata-24.4/xsdata/formats/dataclass/serializers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5781 2024-04-01 05:14:11.000000 xsdata-24.4/xsdata/formats/dataclass/serializers/code.py
--rw-r--r--   0 runner    (1001) docker     (127)     2180 2024-04-01 05:14:11.000000 xsdata-24.4/xsdata/formats/dataclass/serializers/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3160 2024-04-01 05:14:11.000000 xsdata-24.4/xsdata/formats/dataclass/serializers/dict.py
--rw-r--r--   0 runner    (1001) docker     (127)     1168 2024-04-01 05:14:11.000000 xsdata-24.4/xsdata/formats/dataclass/serializers/json.py
--rw-r--r--   0 runner    (1001) docker     (127)    29455 2024-04-01 05:14:11.000000 xsdata-24.4/xsdata/formats/dataclass/serializers/mixins.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 05:14:15.476624 xsdata-24.4/xsdata/formats/dataclass/serializers/tree/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 05:14:11.000000 xsdata-24.4/xsdata/formats/dataclass/serializers/tree/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-04-01 05:14:11.000000 xsdata-24.4/xsdata/formats/dataclass/serializers/tree/lxml.py
--rw-r--r--   0 runner    (1001) docker     (127)     1879 2024-04-01 05:14:11.000000 xsdata-24.4/xsdata/formats/dataclass/serializers/tree/mixins.py
--rw-r--r--   0 runner    (1001) docker     (127)      604 2024-04-01 05:14:11.000000 xsdata-24.4/xsdata/formats/dataclass/serializers/tree/native.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 05:14:15.476624 xsdata-24.4/xsdata/formats/dataclass/serializers/writers/
--rw-r--r--   0 runner    (1001) docker     (127)      625 2024-04-01 05:14:11.000000 xsdata-24.4/xsdata/formats/dataclass/serializers/writers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2068 2024-04-01 05:14:11.000000 xsdata-24.4/xsdata/formats/dataclass/serializers/writers/lxml.py
--rw-r--r--   0 runner    (1001) docker     (127)     3264 2024-04-01 05:14:11.000000 xsdata-24.4/xsdata/formats/dataclass/serializers/writers/native.py
--rw-r--r--   0 runner    (1001) docker     (127)     1645 2024-04-01 05:14:11.000000 xsdata-24.4/xsdata/formats/dataclass/serializers/xml.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 05:14:15.476624 xsdata-24.4/xsdata/formats/dataclass/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     2497 2024-04-01 05:14:11.000000 xsdata-24.4/xsdata/formats/dataclass/templates/class.jinja2
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-01 05:14:11.000000 xsdata-24.4/xsdata/formats/dataclass/templates/docstrings.accessible.jinja2
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 05:14:11.000000 xsdata-24.4/xsdata/formats/dataclass/templates/docstrings.blank.jinja2
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-04-01 05:14:11.000000 xsdata-24.4/xsdata/formats/dataclass/templates/docstrings.google.jinja2
--rw-r--r--   0 runner    (1001) docker     (127)      402 2024-04-01 05:14:11.000000 xsdata-24.4/xsdata/formats/dataclass/templates/docstrings.numpy.jinja2
--rw-r--r--   0 runner    (1001) docker     (127)      360 2024-04-01 05:14:11.000000 xsdata-24.4/xsdata/formats/dataclass/templates/docstrings.rst.jinja2
--rw-r--r--   0 runner    (1001) docker     (127)      781 2024-04-01 05:14:11.000000 xsdata-24.4/xsdata/formats/dataclass/templates/enum.jinja2
--rw-r--r--   0 runner    (1001) docker     (127)      376 2024-04-01 05:14:11.000000 xsdata-24.4/xsdata/formats/dataclass/templates/imports.jinja2
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-01 05:14:11.000000 xsdata-24.4/xsdata/formats/dataclass/templates/module.jinja2
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-04-01 05:14:11.000000 xsdata-24.4/xsdata/formats/dataclass/templates/package.jinja2
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-01 05:14:11.000000 xsdata-24.4/xsdata/formats/dataclass/templates/service.jinja2
--rw-r--r--   0 runner    (1001) docker     (127)     2461 2024-04-01 05:14:11.000000 xsdata-24.4/xsdata/formats/dataclass/transports.py
--rw-r--r--   0 runner    (1001) docker     (127)     4308 2024-04-01 05:14:11.000000 xsdata-24.4/xsdata/formats/dataclass/typing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3280 2024-04-01 05:14:11.000000 xsdata-24.4/xsdata/formats/mixins.py
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-01 05:14:11.000000 xsdata-24.4/xsdata/formats/types.py
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-01 05:14:11.000000 xsdata-24.4/xsdata/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 05:14:15.480624 xsdata-24.4/xsdata/models/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 05:14:11.000000 xsdata-24.4/xsdata/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17827 2024-04-01 05:14:11.000000 xsdata-24.4/xsdata/models/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    21018 2024-04-01 05:14:11.000000 xsdata-24.4/xsdata/models/datatype.py
--rw-r--r--   0 runner    (1001) docker     (127)     3121 2024-04-01 05:14:11.000000 xsdata-24.4/xsdata/models/dtd.py
--rw-r--r--   0 runner    (1001) docker     (127)     9943 2024-04-01 05:14:11.000000 xsdata-24.4/xsdata/models/enums.py
--rw-r--r--   0 runner    (1001) docker     (127)     7288 2024-04-01 05:14:11.000000 xsdata-24.4/xsdata/models/mixins.py
--rw-r--r--   0 runner    (1001) docker     (127)     9908 2024-04-01 05:14:11.000000 xsdata-24.4/xsdata/models/wsdl.py
--rw-r--r--   0 runner    (1001) docker     (127)    33275 2024-04-01 05:14:11.000000 xsdata-24.4/xsdata/models/xsd.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 05:14:11.000000 xsdata-24.4/xsdata/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 05:14:15.480624 xsdata-24.4/xsdata/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)     4067 2024-04-01 05:14:11.000000 xsdata-24.4/xsdata/schemas/mathml3-common.xsd
--rw-r--r--   0 runner    (1001) docker     (127)    28457 2024-04-01 05:14:11.000000 xsdata-24.4/xsdata/schemas/mathml3-content.xsd
--rw-r--r--   0 runner    (1001) docker     (127)    84129 2024-04-01 05:14:11.000000 xsdata-24.4/xsdata/schemas/mathml3-presentation.xsd
--rw-r--r--   0 runner    (1001) docker     (127)     6846 2024-04-01 05:14:11.000000 xsdata-24.4/xsdata/schemas/mathml3-strict-content.xsd
--rw-r--r--   0 runner    (1001) docker     (127)      436 2024-04-01 05:14:11.000000 xsdata-24.4/xsdata/schemas/mathml3.xsd
--rw-r--r--   0 runner    (1001) docker     (127)     8051 2024-04-01 05:14:11.000000 xsdata-24.4/xsdata/schemas/xlink.xsd
--rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-04-01 05:14:11.000000 xsdata-24.4/xsdata/schemas/xml.xsd
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-04-01 05:14:11.000000 xsdata-24.4/xsdata/schemas/xsi.xsd
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 05:14:15.480624 xsdata-24.4/xsdata/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 05:14:11.000000 xsdata-24.4/xsdata/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5005 2024-04-01 05:14:11.000000 xsdata-24.4/xsdata/utils/click.py
--rw-r--r--   0 runner    (1001) docker     (127)     3093 2024-04-01 05:14:11.000000 xsdata-24.4/xsdata/utils/collections.py
--rw-r--r--   0 runner    (1001) docker     (127)      435 2024-04-01 05:14:11.000000 xsdata-24.4/xsdata/utils/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     8011 2024-04-01 05:14:11.000000 xsdata-24.4/xsdata/utils/dates.py
--rw-r--r--   0 runner    (1001) docker     (127)      736 2024-04-01 05:14:11.000000 xsdata-24.4/xsdata/utils/debug.py
--rw-r--r--   0 runner    (1001) docker     (127)     4999 2024-04-01 05:14:11.000000 xsdata-24.4/xsdata/utils/downloader.py
--rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-04-01 05:14:11.000000 xsdata-24.4/xsdata/utils/graphs.py
--rw-r--r--   0 runner    (1001) docker     (127)      390 2024-04-01 05:14:11.000000 xsdata-24.4/xsdata/utils/hooks.py
--rw-r--r--   0 runner    (1001) docker     (127)     4779 2024-04-01 05:14:11.000000 xsdata-24.4/xsdata/utils/namespaces.py
--rw-r--r--   0 runner    (1001) docker     (127)      763 2024-04-01 05:14:11.000000 xsdata-24.4/xsdata/utils/objects.py
--rw-r--r--   0 runner    (1001) docker     (127)      868 2024-04-01 05:14:11.000000 xsdata-24.4/xsdata/utils/package.py
--rw-r--r--   0 runner    (1001) docker     (127)    17119 2024-04-01 05:14:11.000000 xsdata-24.4/xsdata/utils/testing.py
--rw-r--r--   0 runner    (1001) docker     (127)     4902 2024-04-01 05:14:11.000000 xsdata-24.4/xsdata/utils/text.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 05:14:15.484624 xsdata-24.4/xsdata.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6963 2024-04-01 05:14:15.000000 xsdata-24.4/xsdata.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    16607 2024-04-01 05:14:15.000000 xsdata-24.4/xsdata.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 05:14:15.000000 xsdata-24.4/xsdata.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-01 05:14:15.000000 xsdata-24.4/xsdata.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      374 2024-04-01 05:14:15.000000 xsdata-24.4/xsdata.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-01 05:14:15.000000 xsdata-24.4/xsdata.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 16:28:25.907989 xsdata-24.5/
+-rw-r--r--   0 runner    (1001) docker     (127)    38585 2024-05-07 16:28:15.000000 xsdata-24.5/CHANGES.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-05-07 16:28:15.000000 xsdata-24.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-07 16:28:15.000000 xsdata-24.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6011 2024-05-07 16:28:25.907989 xsdata-24.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3522 2024-05-07 16:28:15.000000 xsdata-24.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 16:28:25.831989 xsdata-24.5/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 16:28:15.000000 xsdata-24.5/docs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 16:28:25.831989 xsdata-24.5/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 16:28:15.000000 xsdata-24.5/docs/api/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-07 16:28:15.000000 xsdata-24.5/docs/changelog.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 16:28:25.831989 xsdata-24.5/docs/codegen/
+-rw-r--r--   0 runner    (1001) docker     (127)     5122 2024-05-07 16:28:15.000000 xsdata-24.5/docs/codegen/architecture.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11393 2024-05-07 16:28:15.000000 xsdata-24.5/docs/codegen/config.md
+-rw-r--r--   0 runner    (1001) docker     (127)      838 2024-05-07 16:28:15.000000 xsdata-24.5/docs/codegen/docstrings.md
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-07 16:28:15.000000 xsdata-24.5/docs/codegen/download_schemas.md
+-rw-r--r--   0 runner    (1001) docker     (127)      608 2024-05-07 16:28:15.000000 xsdata-24.5/docs/codegen/dtd_modeling.md
+-rw-r--r--   0 runner    (1001) docker     (127)      912 2024-05-07 16:28:15.000000 xsdata-24.5/docs/codegen/intro.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-05-07 16:28:15.000000 xsdata-24.5/docs/codegen/samples_modeling.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4090 2024-05-07 16:28:15.000000 xsdata-24.5/docs/codegen/wsdl_modeling.md
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-07 16:28:15.000000 xsdata-24.5/docs/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 16:28:25.835989 xsdata-24.5/docs/data_binding/
+-rw-r--r--   0 runner    (1001) docker     (127)     7201 2024-05-07 16:28:15.000000 xsdata-24.5/docs/data_binding/basics.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1763 2024-05-07 16:28:15.000000 xsdata-24.5/docs/data_binding/dict_decoding.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1798 2024-05-07 16:28:15.000000 xsdata-24.5/docs/data_binding/dict_encoding.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4320 2024-05-07 16:28:15.000000 xsdata-24.5/docs/data_binding/json_parsing.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3459 2024-05-07 16:28:15.000000 xsdata-24.5/docs/data_binding/json_serializing.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-05-07 16:28:15.000000 xsdata-24.5/docs/data_binding/pycode_serializing.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-05-07 16:28:15.000000 xsdata-24.5/docs/data_binding/tree_serializing.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5384 2024-05-07 16:28:15.000000 xsdata-24.5/docs/data_binding/xml_parsing.md
+-rw-r--r--   0 runner    (1001) docker     (127)     8281 2024-05-07 16:28:15.000000 xsdata-24.5/docs/data_binding/xml_serializing.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-05-07 16:28:15.000000 xsdata-24.5/docs/faq.md
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-05-07 16:28:15.000000 xsdata-24.5/docs/favicon.png
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-05-07 16:28:15.000000 xsdata-24.5/docs/hooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)      470 2024-05-07 16:28:15.000000 xsdata-24.5/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-05-07 16:28:15.000000 xsdata-24.5/docs/installation.md
+-rw-r--r--   0 runner    (1001) docker     (127)      792 2024-05-07 16:28:15.000000 xsdata-24.5/docs/logo-small.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     3535 2024-05-07 16:28:15.000000 xsdata-24.5/docs/logo.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 16:28:25.835989 xsdata-24.5/docs/models/
+-rw-r--r--   0 runner    (1001) docker     (127)     3286 2024-05-07 16:28:15.000000 xsdata-24.5/docs/models/classes.md
+-rw-r--r--   0 runner    (1001) docker     (127)    10287 2024-05-07 16:28:15.000000 xsdata-24.5/docs/models/fields.md
+-rw-r--r--   0 runner    (1001) docker     (127)    10969 2024-05-07 16:28:15.000000 xsdata-24.5/docs/models/types.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 16:28:25.835989 xsdata-24.5/docs/overrides/
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-05-07 16:28:15.000000 xsdata-24.5/docs/overrides/main.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 16:28:25.835989 xsdata-24.5/docs/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-05-07 16:28:15.000000 xsdata-24.5/docs/plugins/how_to.md
+-rw-r--r--   0 runner    (1001) docker     (127)      774 2024-05-07 16:28:15.000000 xsdata-24.5/docs/plugins/list.md
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-07 16:28:15.000000 xsdata-24.5/docs/robots.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      771 2024-05-07 16:28:15.000000 xsdata-24.5/docs/samples.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 16:28:25.835989 xsdata-24.5/docs/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 16:28:15.000000 xsdata-24.5/docs/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      788 2024-05-07 16:28:15.000000 xsdata-24.5/docs/scripts/generate_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3369 2024-05-07 16:28:15.000000 xsdata-24.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 16:28:25.907989 xsdata-24.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 16:28:25.835989 xsdata-24.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-07 16:28:15.000000 xsdata-24.5/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 16:28:25.835989 xsdata-24.5/tests/codegen/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 16:28:15.000000 xsdata-24.5/tests/codegen/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 16:28:25.843989 xsdata-24.5/tests/codegen/handlers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 16:28:15.000000 xsdata-24.5/tests/codegen/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5685 2024-05-07 16:28:15.000000 xsdata-24.5/tests/codegen/handlers/test_add_attribute_substitutions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3768 2024-05-07 16:28:15.000000 xsdata-24.5/tests/codegen/handlers/test_calculate_attribute_paths.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11132 2024-05-07 16:28:15.000000 xsdata-24.5/tests/codegen/handlers/test_create_compound_fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4403 2024-05-07 16:28:15.000000 xsdata-24.5/tests/codegen/handlers/test_create_wrapper_fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8329 2024-05-07 16:28:15.000000 xsdata-24.5/tests/codegen/handlers/test_designate_class_packages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2590 2024-05-07 16:28:15.000000 xsdata-24.5/tests/codegen/handlers/test_detect_circular_references.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9496 2024-05-07 16:28:15.000000 xsdata-24.5/tests/codegen/handlers/test_disambiguate_choices.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1600 2024-05-07 16:28:15.000000 xsdata-24.5/tests/codegen/handlers/test_filter_classes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2562 2024-05-07 16:28:15.000000 xsdata-24.5/tests/codegen/handlers/test_flatten_attribute_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20025 2024-05-07 16:28:15.000000 xsdata-24.5/tests/codegen/handlers/test_flatten_class_extensions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3013 2024-05-07 16:28:15.000000 xsdata-24.5/tests/codegen/handlers/test_merge_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16126 2024-05-07 16:28:15.000000 xsdata-24.5/tests/codegen/handlers/test_process_attributes_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-05-07 16:28:15.000000 xsdata-24.5/tests/codegen/handlers/test_process_mixed_content_class.py
+-rw-r--r--   0 runner    (1001) docker     (127)      633 2024-05-07 16:28:15.000000 xsdata-24.5/tests/codegen/handlers/test_rename_duplicate_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6663 2024-05-07 16:28:15.000000 xsdata-24.5/tests/codegen/handlers/test_rename_duplicate_classes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2975 2024-05-07 16:28:15.000000 xsdata-24.5/tests/codegen/handlers/test_reset_attribute_sequence_numbers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2449 2024-05-07 16:28:15.000000 xsdata-24.5/tests/codegen/handlers/test_reset_attribute_sequences.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12009 2024-05-07 16:28:15.000000 xsdata-24.5/tests/codegen/handlers/test_sanitize_attributes_default_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2699 2024-05-07 16:28:15.000000 xsdata-24.5/tests/codegen/handlers/test_sanitize_enumeration_class.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4785 2024-05-07 16:28:15.000000 xsdata-24.5/tests/codegen/handlers/test_unnest_inner_classes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4441 2024-05-07 16:28:15.000000 xsdata-24.5/tests/codegen/handlers/test_update_attributes_effective_choice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4678 2024-05-07 16:28:15.000000 xsdata-24.5/tests/codegen/handlers/test_vacuum_inner_classes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7657 2024-05-07 16:28:15.000000 xsdata-24.5/tests/codegen/handlers/test_validate_attributes_overrides.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2974 2024-05-07 16:28:15.000000 xsdata-24.5/tests/codegen/handlers/test_validate_references.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 16:28:25.843989 xsdata-24.5/tests/codegen/mappers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 16:28:15.000000 xsdata-24.5/tests/codegen/mappers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29219 2024-05-07 16:28:15.000000 xsdata-24.5/tests/codegen/mappers/test_definitions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4295 2024-05-07 16:28:15.000000 xsdata-24.5/tests/codegen/mappers/test_dict.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15038 2024-05-07 16:28:15.000000 xsdata-24.5/tests/codegen/mappers/test_dtd.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11922 2024-05-07 16:28:15.000000 xsdata-24.5/tests/codegen/mappers/test_element.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16997 2024-05-07 16:28:15.000000 xsdata-24.5/tests/codegen/mappers/test_schema.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 16:28:25.843989 xsdata-24.5/tests/codegen/models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 16:28:15.000000 xsdata-24.5/tests/codegen/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6918 2024-05-07 16:28:15.000000 xsdata-24.5/tests/codegen/models/test_attr.py
+-rw-r--r--   0 runner    (1001) docker     (127)      647 2024-05-07 16:28:15.000000 xsdata-24.5/tests/codegen/models/test_attr_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7059 2024-05-07 16:28:15.000000 xsdata-24.5/tests/codegen/models/test_class.py
+-rw-r--r--   0 runner    (1001) docker     (127)      854 2024-05-07 16:28:15.000000 xsdata-24.5/tests/codegen/models/test_codegen.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4340 2024-05-07 16:28:15.000000 xsdata-24.5/tests/codegen/models/test_restrictions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 16:28:25.843989 xsdata-24.5/tests/codegen/parsers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 16:28:15.000000 xsdata-24.5/tests/codegen/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-07 16:28:15.000000 xsdata-24.5/tests/codegen/parsers/test_definitions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6478 2024-05-07 16:28:15.000000 xsdata-24.5/tests/codegen/parsers/test_dtd.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15693 2024-05-07 16:28:15.000000 xsdata-24.5/tests/codegen/parsers/test_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6158 2024-05-07 16:28:15.000000 xsdata-24.5/tests/codegen/test_container.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8862 2024-05-07 16:28:15.000000 xsdata-24.5/tests/codegen/test_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19437 2024-05-07 16:28:15.000000 xsdata-24.5/tests/codegen/test_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15304 2024-05-07 16:28:15.000000 xsdata-24.5/tests/codegen/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6657 2024-05-07 16:28:15.000000 xsdata-24.5/tests/codegen/test_validator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3112 2024-05-07 16:28:15.000000 xsdata-24.5/tests/codegen/test_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1500 2024-05-07 16:28:15.000000 xsdata-24.5/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 16:28:25.843989 xsdata-24.5/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 16:28:15.000000 xsdata-24.5/tests/fixtures/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 16:28:25.847989 xsdata-24.5/tests/fixtures/annotations/
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-05-07 16:28:15.000000 xsdata-24.5/tests/fixtures/annotations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-05-07 16:28:15.000000 xsdata-24.5/tests/fixtures/annotations/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-05-07 16:28:15.000000 xsdata-24.5/tests/fixtures/annotations/model.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-07 16:28:15.000000 xsdata-24.5/tests/fixtures/annotations/sample.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-05-07 16:28:15.000000 xsdata-24.5/tests/fixtures/annotations/units.py
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2024-05-07 16:28:15.000000 xsdata-24.5/tests/fixtures/annotations/units.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)      950 2024-05-07 16:28:15.000000 xsdata-24.5/tests/fixtures/annotations/xsdata.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 16:28:25.847989 xsdata-24.5/tests/fixtures/artists/
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-05-07 16:28:15.000000 xsdata-24.5/tests/fixtures/artists/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4517 2024-05-07 16:28:15.000000 xsdata-24.5/tests/fixtures/artists/art001.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-05-07 16:28:15.000000 xsdata-24.5/tests/fixtures/artists/art002.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     2629 2024-05-07 16:28:15.000000 xsdata-24.5/tests/fixtures/artists/art003.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     9232 2024-05-07 16:28:15.000000 xsdata-24.5/tests/fixtures/artists/metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 16:28:25.847989 xsdata-24.5/tests/fixtures/books/
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-07 16:28:15.000000 xsdata-24.5/tests/fixtures/books/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-05-07 16:28:15.000000 xsdata-24.5/tests/fixtures/books/bk001.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-05-07 16:28:15.000000 xsdata-24.5/tests/fixtures/books/bk002.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-07 16:28:15.000000 xsdata-24.5/tests/fixtures/books/books-xinclude.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      485 2024-05-07 16:28:15.000000 xsdata-24.5/tests/fixtures/books/books.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2184 2024-05-07 16:28:15.000000 xsdata-24.5/tests/fixtures/books/books.py
+-rw-r--r--   0 runner    (1001) docker     (127)      602 2024-05-07 16:28:15.000000 xsdata-24.5/tests/fixtures/books/books.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      602 2024-05-07 16:28:15.000000 xsdata-24.5/tests/fixtures/books/books_auto_ns.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      608 2024-05-07 16:28:15.000000 xsdata-24.5/tests/fixtures/books/books_default_ns.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     3842 2024-05-07 16:28:15.000000 xsdata-24.5/tests/fixtures/books/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2405 2024-05-07 16:28:15.000000 xsdata-24.5/tests/fixtures/books/schema.xsd
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 16:28:25.851989 xsdata-24.5/tests/fixtures/calculator/
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-05-07 16:28:15.000000 xsdata-24.5/tests/fixtures/calculator/AddRQ.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-07 16:28:15.000000 xsdata-24.5/tests/fixtures/calculator/AddRS.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-05-07 16:28:15.000000 xsdata-24.5/tests/fixtures/calculator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13579 2024-05-07 16:28:15.000000 xsdata-24.5/tests/fixtures/calculator/services.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7880 2024-05-07 16:28:15.000000 xsdata-24.5/tests/fixtures/calculator/services.wsdl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 16:28:25.851989 xsdata-24.5/tests/fixtures/compound/
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-07 16:28:15.000000 xsdata-24.5/tests/fixtures/compound/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1198 2024-05-07 16:28:15.000000 xsdata-24.5/tests/fixtures/compound/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-05-07 16:28:15.000000 xsdata-24.5/tests/fixtures/compound/sample.json
+-rw-r--r--   0 runner    (1001) docker     (127)      560 2024-05-07 16:28:15.000000 xsdata-24.5/tests/fixtures/compound/sample.py
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-07 16:28:15.000000 xsdata-24.5/tests/fixtures/compound/sample.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-05-07 16:28:15.000000 xsdata-24.5/tests/fixtures/compound/sample.xsdata.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      844 2024-05-07 16:28:15.000000 xsdata-24.5/tests/fixtures/compound/schema.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)      680 2024-05-07 16:28:15.000000 xsdata-24.5/tests/fixtures/datatypes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 16:28:25.851989 xsdata-24.5/tests/fixtures/docstrings/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 16:28:15.000000 xsdata-24.5/tests/fixtures/docstrings/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 16:28:25.851989 xsdata-24.5/tests/fixtures/docstrings/accessible/
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-07 16:28:15.000000 xsdata-24.5/tests/fixtures/docstrings/accessible/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2931 2024-05-07 16:28:15.000000 xsdata-24.5/tests/fixtures/docstrings/accessible/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 16:28:25.851989 xsdata-24.5/tests/fixtures/docstrings/blank/
+-rw-r--r--   0 runner    (1001) docker     (127)      282 2024-05-07 16:28:15.000000 xsdata-24.5/tests/fixtures/docstrings/blank/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-05-07 16:28:15.000000 xsdata-24.5/tests/fixtures/docstrings/blank/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 16:28:25.851989 xsdata-24.5/tests/fixtures/docstrings/google/
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-05-07 16:28:15.000000 xsdata-24.5/tests/fixtures/docstrings/google/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2871 2024-05-07 16:28:15.000000 xsdata-24.5/tests/fixtures/docstrings/google/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 16:28:25.851989 xsdata-24.5/tests/fixtures/docstrings/numpy/
+-rw-r--r--   0 runner    (1001) docker     (127)      282 2024-05-07 16:28:15.000000 xsdata-24.5/tests/fixtures/docstrings/numpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2914 2024-05-07 16:28:15.000000 xsdata-24.5/tests/fixtures/docstrings/numpy/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 16:28:25.851989 xsdata-24.5/tests/fixtures/docstrings/rst/
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-05-07 16:28:15.000000 xsdata-24.5/tests/fixtures/docstrings/rst/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2797 2024-05-07 16:28:15.000000 xsdata-24.5/tests/fixtures/docstrings/rst/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4081 2024-05-07 16:28:15.000000 xsdata-24.5/tests/fixtures/docstrings/schema.xsd
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 16:28:25.855989 xsdata-24.5/tests/fixtures/dtd/
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-07 16:28:15.000000 xsdata-24.5/tests/fixtures/dtd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-05-07 16:28:15.000000 xsdata-24.5/tests/fixtures/dtd/complete_example.dtd
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-07 16:28:15.000000 xsdata-24.5/tests/fixtures/dtd/default_namespace.dtd
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 16:28:25.855989 xsdata-24.5/tests/fixtures/dtd/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-05-07 16:28:15.000000 xsdata-24.5/tests/fixtures/dtd/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2819 2024-05-07 16:28:15.000000 xsdata-24.5/tests/fixtures/dtd/models/complete_example.py
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-07 16:28:15.000000 xsdata-24.5/tests/fixtures/dtd/prefix_namespace.dtd
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 16:28:25.855989 xsdata-24.5/tests/fixtures/hello/
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-05-07 16:28:15.000000 xsdata-24.5/tests/fixtures/hello/HelloRQ.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-07 16:28:15.000000 xsdata-24.5/tests/fixtures/hello/HelloRS.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      489 2024-05-07 16:28:15.000000 xsdata-24.5/tests/fixtures/hello/HelloRS_SoapFault.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      430 2024-05-07 16:28:15.000000 xsdata-24.5/tests/fixtures/hello/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4612 2024-05-07 16:28:15.000000 xsdata-24.5/tests/fixtures/hello/hello.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3084 2024-05-07 16:28:15.000000 xsdata-24.5/tests/fixtures/hello/hello.wsdl
+-rw-r--r--   0 runner    (1001) docker     (127)      781 2024-05-07 16:28:15.000000 xsdata-24.5/tests/fixtures/hello/hello.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)     4760 2024-05-07 16:28:15.000000 xsdata-24.5/tests/fixtures/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 16:28:25.855989 xsdata-24.5/tests/fixtures/primer/
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-05-07 16:28:15.000000 xsdata-24.5/tests/fixtures/primer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4624 2024-05-07 16:28:15.000000 xsdata-24.5/tests/fixtures/primer/order.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3032 2024-05-07 16:28:15.000000 xsdata-24.5/tests/fixtures/primer/order.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)      890 2024-05-07 16:28:15.000000 xsdata-24.5/tests/fixtures/primer/sample.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1315 2024-05-07 16:28:15.000000 xsdata-24.5/tests/fixtures/primer/sample.py
+-rw-r--r--   0 runner    (1001) docker     (127)      881 2024-05-07 16:28:15.000000 xsdata-24.5/tests/fixtures/primer/sample.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      889 2024-05-07 16:28:15.000000 xsdata-24.5/tests/fixtures/primer/sample.xsdata.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 16:28:25.855989 xsdata-24.5/tests/fixtures/series/
+-rw-r--r--   0 runner    (1001) docker     (127)      344 2024-05-07 16:28:15.000000 xsdata-24.5/tests/fixtures/series/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 16:28:25.855989 xsdata-24.5/tests/fixtures/series/samples/
+-rw-r--r--   0 runner    (1001) docker     (127)     1263 2024-05-07 16:28:15.000000 xsdata-24.5/tests/fixtures/series/samples/show1.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-05-07 16:28:15.000000 xsdata-24.5/tests/fixtures/series/samples/show2.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6665 2024-05-07 16:28:15.000000 xsdata-24.5/tests/fixtures/series/series.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 16:28:25.859989 xsdata-24.5/tests/fixtures/stripe/
+-rw-r--r--   0 runner    (1001) docker     (127)      931 2024-05-07 16:28:15.000000 xsdata-24.5/tests/fixtures/stripe/.xsdata.xml
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 16:28:15.000000 xsdata-24.5/tests/fixtures/stripe/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 16:28:25.859989 xsdata-24.5/tests/fixtures/stripe/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-07 16:28:15.000000 xsdata-24.5/tests/fixtures/stripe/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3034 2024-05-07 16:28:15.000000 xsdata-24.5/tests/fixtures/stripe/models/balance.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 16:28:25.859989 xsdata-24.5/tests/fixtures/stripe/samples/
+-rw-r--r--   0 runner    (1001) docker     (127)     2628 2024-05-07 16:28:15.000000 xsdata-24.5/tests/fixtures/stripe/samples/balance.json
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-07 16:28:15.000000 xsdata-24.5/tests/fixtures/submodels.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 16:28:25.859989 xsdata-24.5/tests/fixtures/typemapping/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 16:28:15.000000 xsdata-24.5/tests/fixtures/typemapping/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-05-07 16:28:15.000000 xsdata-24.5/tests/fixtures/typemapping/city.py
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-05-07 16:28:15.000000 xsdata-24.5/tests/fixtures/typemapping/house.py
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-07 16:28:15.000000 xsdata-24.5/tests/fixtures/typemapping/street.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 16:28:25.859989 xsdata-24.5/tests/fixtures/wrapper/
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-07 16:28:15.000000 xsdata-24.5/tests/fixtures/wrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1874 2024-05-07 16:28:15.000000 xsdata-24.5/tests/fixtures/wrapper/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-05-07 16:28:15.000000 xsdata-24.5/tests/fixtures/wrapper/sample.json
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-05-07 16:28:15.000000 xsdata-24.5/tests/fixtures/wrapper/sample.py
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-07 16:28:15.000000 xsdata-24.5/tests/fixtures/wrapper/sample.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-07 16:28:15.000000 xsdata-24.5/tests/fixtures/wrapper/sample.xsdata.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1482 2024-05-07 16:28:15.000000 xsdata-24.5/tests/fixtures/wrapper/schema.xsd
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 16:28:25.859989 xsdata-24.5/tests/formats/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 16:28:15.000000 xsdata-24.5/tests/formats/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 16:28:25.863989 xsdata-24.5/tests/formats/dataclass/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 16:28:15.000000 xsdata-24.5/tests/formats/dataclass/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 16:28:25.863989 xsdata-24.5/tests/formats/dataclass/cases/
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-07 16:28:15.000000 xsdata-24.5/tests/formats/dataclass/cases/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-05-07 16:28:15.000000 xsdata-24.5/tests/formats/dataclass/cases/attribute.py
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-07 16:28:15.000000 xsdata-24.5/tests/formats/dataclass/cases/attributes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-05-07 16:28:15.000000 xsdata-24.5/tests/formats/dataclass/cases/element.py
+-rw-r--r--   0 runner    (1001) docker     (127)      881 2024-05-07 16:28:15.000000 xsdata-24.5/tests/formats/dataclass/cases/elements.py
+-rw-r--r--   0 runner    (1001) docker     (127)      643 2024-05-07 16:28:15.000000 xsdata-24.5/tests/formats/dataclass/cases/wildcard.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 16:28:25.863989 xsdata-24.5/tests/formats/dataclass/models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 16:28:15.000000 xsdata-24.5/tests/formats/dataclass/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14827 2024-05-07 16:28:15.000000 xsdata-24.5/tests/formats/dataclass/models/test_builders.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 16:28:25.863989 xsdata-24.5/tests/formats/dataclass/parsers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 16:28:15.000000 xsdata-24.5/tests/formats/dataclass/parsers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 16:28:25.867989 xsdata-24.5/tests/formats/dataclass/parsers/handlers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 16:28:15.000000 xsdata-24.5/tests/formats/dataclass/parsers/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2755 2024-05-07 16:28:15.000000 xsdata-24.5/tests/formats/dataclass/parsers/handlers/test_lxml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3179 2024-05-07 16:28:15.000000 xsdata-24.5/tests/formats/dataclass/parsers/handlers/test_native.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 16:28:25.867989 xsdata-24.5/tests/formats/dataclass/parsers/nodes/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 16:28:15.000000 xsdata-24.5/tests/formats/dataclass/parsers/nodes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19712 2024-05-07 16:28:15.000000 xsdata-24.5/tests/formats/dataclass/parsers/nodes/test_element.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3064 2024-05-07 16:28:15.000000 xsdata-24.5/tests/formats/dataclass/parsers/nodes/test_primitive.py
+-rw-r--r--   0 runner    (1001) docker     (127)      377 2024-05-07 16:28:15.000000 xsdata-24.5/tests/formats/dataclass/parsers/nodes/test_skip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1676 2024-05-07 16:28:15.000000 xsdata-24.5/tests/formats/dataclass/parsers/nodes/test_standard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3960 2024-05-07 16:28:15.000000 xsdata-24.5/tests/formats/dataclass/parsers/nodes/test_union.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2221 2024-05-07 16:28:15.000000 xsdata-24.5/tests/formats/dataclass/parsers/nodes/test_wildcard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2757 2024-05-07 16:28:15.000000 xsdata-24.5/tests/formats/dataclass/parsers/nodes/test_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14597 2024-05-07 16:28:15.000000 xsdata-24.5/tests/formats/dataclass/parsers/test_dict.py
+-rw-r--r--   0 runner    (1001) docker     (127)      815 2024-05-07 16:28:15.000000 xsdata-24.5/tests/formats/dataclass/parsers/test_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1172 2024-05-07 16:28:15.000000 xsdata-24.5/tests/formats/dataclass/parsers/test_mixins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7729 2024-05-07 16:28:15.000000 xsdata-24.5/tests/formats/dataclass/parsers/test_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)      981 2024-05-07 16:28:15.000000 xsdata-24.5/tests/formats/dataclass/parsers/test_tree.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4763 2024-05-07 16:28:15.000000 xsdata-24.5/tests/formats/dataclass/parsers/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2210 2024-05-07 16:28:15.000000 xsdata-24.5/tests/formats/dataclass/parsers/test_xml.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 16:28:25.867989 xsdata-24.5/tests/formats/dataclass/serializers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 16:28:15.000000 xsdata-24.5/tests/formats/dataclass/serializers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4106 2024-05-07 16:28:15.000000 xsdata-24.5/tests/formats/dataclass/serializers/test_code.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-05-07 16:28:15.000000 xsdata-24.5/tests/formats/dataclass/serializers/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3584 2024-05-07 16:28:15.000000 xsdata-24.5/tests/formats/dataclass/serializers/test_dict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3274 2024-05-07 16:28:15.000000 xsdata-24.5/tests/formats/dataclass/serializers/test_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30343 2024-05-07 16:28:15.000000 xsdata-24.5/tests/formats/dataclass/serializers/test_mixins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1490 2024-05-07 16:28:15.000000 xsdata-24.5/tests/formats/dataclass/serializers/test_xml.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 16:28:25.867989 xsdata-24.5/tests/formats/dataclass/serializers/writers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 16:28:15.000000 xsdata-24.5/tests/formats/dataclass/serializers/writers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3327 2024-05-07 16:28:15.000000 xsdata-24.5/tests/formats/dataclass/serializers/writers/test_lxml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2299 2024-05-07 16:28:15.000000 xsdata-24.5/tests/formats/dataclass/serializers/writers/test_native.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5580 2024-05-07 16:28:15.000000 xsdata-24.5/tests/formats/dataclass/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-05-07 16:28:15.000000 xsdata-24.5/tests/formats/dataclass/test_compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5501 2024-05-07 16:28:15.000000 xsdata-24.5/tests/formats/dataclass/test_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9303 2024-05-07 16:28:15.000000 xsdata-24.5/tests/formats/dataclass/test_elements.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42650 2024-05-07 16:28:15.000000 xsdata-24.5/tests/formats/dataclass/test_filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9091 2024-05-07 16:28:15.000000 xsdata-24.5/tests/formats/dataclass/test_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2639 2024-05-07 16:28:15.000000 xsdata-24.5/tests/formats/dataclass/test_transport.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2485 2024-05-07 16:28:15.000000 xsdata-24.5/tests/formats/dataclass/test_typing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16482 2024-05-07 16:28:15.000000 xsdata-24.5/tests/formats/test_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2605 2024-05-07 16:28:15.000000 xsdata-24.5/tests/formats/test_mixins.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 16:28:25.871989 xsdata-24.5/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 16:28:15.000000 xsdata-24.5/tests/integration/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 16:28:25.871989 xsdata-24.5/tests/integration/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 16:28:15.000000 xsdata-24.5/tests/integration/benchmarks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2024-05-07 16:28:15.000000 xsdata-24.5/tests/integration/benchmarks/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      774 2024-05-07 16:28:15.000000 xsdata-24.5/tests/integration/benchmarks/test_converters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-05-07 16:28:15.000000 xsdata-24.5/tests/integration/benchmarks/test_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1852 2024-05-07 16:28:15.000000 xsdata-24.5/tests/integration/benchmarks/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-07 16:28:15.000000 xsdata-24.5/tests/integration/test_annotations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-05-07 16:28:15.000000 xsdata-24.5/tests/integration/test_artists.py
+-rw-r--r--   0 runner    (1001) docker     (127)      761 2024-05-07 16:28:15.000000 xsdata-24.5/tests/integration/test_books.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1868 2024-05-07 16:28:15.000000 xsdata-24.5/tests/integration/test_calculator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-07 16:28:15.000000 xsdata-24.5/tests/integration/test_compound.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1863 2024-05-07 16:28:15.000000 xsdata-24.5/tests/integration/test_docstrings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      561 2024-05-07 16:28:15.000000 xsdata-24.5/tests/integration/test_dtd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3608 2024-05-07 16:28:15.000000 xsdata-24.5/tests/integration/test_hello_rpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      673 2024-05-07 16:28:15.000000 xsdata-24.5/tests/integration/test_primer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-05-07 16:28:15.000000 xsdata-24.5/tests/integration/test_series.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-05-07 16:28:15.000000 xsdata-24.5/tests/integration/test_stripe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-05-07 16:28:15.000000 xsdata-24.5/tests/integration/test_type_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)      763 2024-05-07 16:28:15.000000 xsdata-24.5/tests/integration/test_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 16:28:25.871989 xsdata-24.5/tests/models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 16:28:15.000000 xsdata-24.5/tests/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 16:28:25.871989 xsdata-24.5/tests/models/enums/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 16:28:15.000000 xsdata-24.5/tests/models/enums/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2854 2024-05-07 16:28:15.000000 xsdata-24.5/tests/models/enums/test_datatype.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9622 2024-05-07 16:28:15.000000 xsdata-24.5/tests/models/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21721 2024-05-07 16:28:15.000000 xsdata-24.5/tests/models/test_datatype.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5877 2024-05-07 16:28:15.000000 xsdata-24.5/tests/models/test_mixins.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 16:28:25.875989 xsdata-24.5/tests/models/wsdl/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 16:28:15.000000 xsdata-24.5/tests/models/wsdl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      670 2024-05-07 16:28:15.000000 xsdata-24.5/tests/models/wsdl/test_binding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2682 2024-05-07 16:28:15.000000 xsdata-24.5/tests/models/wsdl/test_definitions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      438 2024-05-07 16:28:15.000000 xsdata-24.5/tests/models/wsdl/test_port_type.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 16:28:25.875989 xsdata-24.5/tests/models/xsd/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 16:28:15.000000 xsdata-24.5/tests/models/xsd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      601 2024-05-07 16:28:15.000000 xsdata-24.5/tests/models/xsd/test_all.py
+-rw-r--r--   0 runner    (1001) docker     (127)      722 2024-05-07 16:28:15.000000 xsdata-24.5/tests/models/xsd/test_alternative.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1353 2024-05-07 16:28:15.000000 xsdata-24.5/tests/models/xsd/test_annotation_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-05-07 16:28:15.000000 xsdata-24.5/tests/models/xsd/test_any.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1380 2024-05-07 16:28:15.000000 xsdata-24.5/tests/models/xsd/test_any_attribute.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2467 2024-05-07 16:28:15.000000 xsdata-24.5/tests/models/xsd/test_attribute.py
+-rw-r--r--   0 runner    (1001) docker     (127)      432 2024-05-07 16:28:15.000000 xsdata-24.5/tests/models/xsd/test_attribute_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-07 16:28:15.000000 xsdata-24.5/tests/models/xsd/test_choice.py
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-07 16:28:15.000000 xsdata-24.5/tests/models/xsd/test_complex_content.py
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-05-07 16:28:15.000000 xsdata-24.5/tests/models/xsd/test_complex_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3654 2024-05-07 16:28:15.000000 xsdata-24.5/tests/models/xsd/test_element.py
+-rw-r--r--   0 runner    (1001) docker     (127)      691 2024-05-07 16:28:15.000000 xsdata-24.5/tests/models/xsd/test_enumeration.py
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-05-07 16:28:15.000000 xsdata-24.5/tests/models/xsd/test_extension.py
+-rw-r--r--   0 runner    (1001) docker     (127)      911 2024-05-07 16:28:15.000000 xsdata-24.5/tests/models/xsd/test_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)      607 2024-05-07 16:28:15.000000 xsdata-24.5/tests/models/xsd/test_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2803 2024-05-07 16:28:15.000000 xsdata-24.5/tests/models/xsd/test_restriction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-05-07 16:28:15.000000 xsdata-24.5/tests/models/xsd/test_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)      626 2024-05-07 16:28:15.000000 xsdata-24.5/tests/models/xsd/test_sequence.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1718 2024-05-07 16:28:15.000000 xsdata-24.5/tests/models/xsd/test_simple_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1819 2024-05-07 16:28:15.000000 xsdata-24.5/tests/models/xsd/test_union.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7902 2024-05-07 16:28:15.000000 xsdata-24.5/tests/test_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 16:28:25.879989 xsdata-24.5/tests/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 16:28:15.000000 xsdata-24.5/tests/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1894 2024-05-07 16:28:15.000000 xsdata-24.5/tests/utils/test_collections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4551 2024-05-07 16:28:15.000000 xsdata-24.5/tests/utils/test_dates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5446 2024-05-07 16:28:15.000000 xsdata-24.5/tests/utils/test_downloader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-05-07 16:28:15.000000 xsdata-24.5/tests/utils/test_hooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5202 2024-05-07 16:28:15.000000 xsdata-24.5/tests/utils/test_namespaces.py
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-05-07 16:28:15.000000 xsdata-24.5/tests/utils/test_objects.py
+-rw-r--r--   0 runner    (1001) docker     (127)      508 2024-05-07 16:28:15.000000 xsdata-24.5/tests/utils/test_testing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7816 2024-05-07 16:28:15.000000 xsdata-24.5/tests/utils/test_text.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 16:28:25.879989 xsdata-24.5/xsdata/
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-07 16:28:15.000000 xsdata-24.5/xsdata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-05-07 16:28:15.000000 xsdata-24.5/xsdata/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5044 2024-05-07 16:28:15.000000 xsdata-24.5/xsdata/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 16:28:25.883989 xsdata-24.5/xsdata/codegen/
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-07 16:28:15.000000 xsdata-24.5/xsdata/codegen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8928 2024-05-07 16:28:15.000000 xsdata-24.5/xsdata/codegen/container.py
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-07 16:28:15.000000 xsdata-24.5/xsdata/codegen/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 16:28:25.887989 xsdata-24.5/xsdata/codegen/handlers/
+-rw-r--r--   0 runner    (1001) docker     (127)     2218 2024-05-07 16:28:15.000000 xsdata-24.5/xsdata/codegen/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4190 2024-05-07 16:28:15.000000 xsdata-24.5/xsdata/codegen/handlers/add_attribute_substitutions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2435 2024-05-07 16:28:15.000000 xsdata-24.5/xsdata/codegen/handlers/calculate_attribute_paths.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8570 2024-05-07 16:28:15.000000 xsdata-24.5/xsdata/codegen/handlers/create_compound_fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4322 2024-05-07 16:28:15.000000 xsdata-24.5/xsdata/codegen/handlers/create_wrapper_fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8679 2024-05-07 16:28:15.000000 xsdata-24.5/xsdata/codegen/handlers/designate_class_packages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2767 2024-05-07 16:28:15.000000 xsdata-24.5/xsdata/codegen/handlers/detect_circular_references.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9526 2024-05-07 16:28:15.000000 xsdata-24.5/xsdata/codegen/handlers/disambiguate_choices.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-05-07 16:28:15.000000 xsdata-24.5/xsdata/codegen/handlers/filter_classes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1957 2024-05-07 16:28:15.000000 xsdata-24.5/xsdata/codegen/handlers/flatten_attribute_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13595 2024-05-07 16:28:15.000000 xsdata-24.5/xsdata/codegen/handlers/flatten_class_extensions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2394 2024-05-07 16:28:15.000000 xsdata-24.5/xsdata/codegen/handlers/merge_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10816 2024-05-07 16:28:15.000000 xsdata-24.5/xsdata/codegen/handlers/process_attributes_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1425 2024-05-07 16:28:15.000000 xsdata-24.5/xsdata/codegen/handlers/process_mixed_content_class.py
+-rw-r--r--   0 runner    (1001) docker     (127)      483 2024-05-07 16:28:15.000000 xsdata-24.5/xsdata/codegen/handlers/rename_duplicate_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6346 2024-05-07 16:28:15.000000 xsdata-24.5/xsdata/codegen/handlers/rename_duplicate_classes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1631 2024-05-07 16:28:15.000000 xsdata-24.5/xsdata/codegen/handlers/reset_attribute_sequence_numbers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1623 2024-05-07 16:28:15.000000 xsdata-24.5/xsdata/codegen/handlers/reset_attribute_sequences.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8394 2024-05-07 16:28:15.000000 xsdata-24.5/xsdata/codegen/handlers/sanitize_attributes_default_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1903 2024-05-07 16:28:15.000000 xsdata-24.5/xsdata/codegen/handlers/sanitize_enumeration_class.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3543 2024-05-07 16:28:15.000000 xsdata-24.5/xsdata/codegen/handlers/unnest_inner_classes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4647 2024-05-07 16:28:15.000000 xsdata-24.5/xsdata/codegen/handlers/update_attributes_effective_choice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3459 2024-05-07 16:28:15.000000 xsdata-24.5/xsdata/codegen/handlers/vacuum_inner_classes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7071 2024-05-07 16:28:15.000000 xsdata-24.5/xsdata/codegen/handlers/validate_attributes_overrides.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3806 2024-05-07 16:28:15.000000 xsdata-24.5/xsdata/codegen/handlers/validate_references.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 16:28:25.887989 xsdata-24.5/xsdata/codegen/mappers/
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-07 16:28:15.000000 xsdata-24.5/xsdata/codegen/mappers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18320 2024-05-07 16:28:15.000000 xsdata-24.5/xsdata/codegen/mappers/definitions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2394 2024-05-07 16:28:15.000000 xsdata-24.5/xsdata/codegen/mappers/dict.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10841 2024-05-07 16:28:15.000000 xsdata-24.5/xsdata/codegen/mappers/dtd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5790 2024-05-07 16:28:15.000000 xsdata-24.5/xsdata/codegen/mappers/element.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3787 2024-05-07 16:28:15.000000 xsdata-24.5/xsdata/codegen/mappers/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12450 2024-05-07 16:28:15.000000 xsdata-24.5/xsdata/codegen/mappers/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4970 2024-05-07 16:28:15.000000 xsdata-24.5/xsdata/codegen/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25868 2024-05-07 16:28:15.000000 xsdata-24.5/xsdata/codegen/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 16:28:25.891989 xsdata-24.5/xsdata/codegen/parsers/
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-05-07 16:28:15.000000 xsdata-24.5/xsdata/codegen/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1579 2024-05-07 16:28:15.000000 xsdata-24.5/xsdata/codegen/parsers/definitions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4034 2024-05-07 16:28:15.000000 xsdata-24.5/xsdata/codegen/parsers/dtd.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13281 2024-05-07 16:28:15.000000 xsdata-24.5/xsdata/codegen/parsers/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5905 2024-05-07 16:28:15.000000 xsdata-24.5/xsdata/codegen/resolver.py
+-rw-r--r--   0 runner    (1001) docker     (127)      427 2024-05-07 16:28:15.000000 xsdata-24.5/xsdata/codegen/stopwatch.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14691 2024-05-07 16:28:15.000000 xsdata-24.5/xsdata/codegen/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17146 2024-05-07 16:28:15.000000 xsdata-24.5/xsdata/codegen/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6532 2024-05-07 16:28:15.000000 xsdata-24.5/xsdata/codegen/validator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3160 2024-05-07 16:28:15.000000 xsdata-24.5/xsdata/codegen/writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-05-07 16:28:15.000000 xsdata-24.5/xsdata/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 16:28:25.891989 xsdata-24.5/xsdata/formats/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 16:28:15.000000 xsdata-24.5/xsdata/formats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24988 2024-05-07 16:28:15.000000 xsdata-24.5/xsdata/formats/converter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 16:28:25.891989 xsdata-24.5/xsdata/formats/dataclass/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 16:28:15.000000 xsdata-24.5/xsdata/formats/dataclass/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6159 2024-05-07 16:28:15.000000 xsdata-24.5/xsdata/formats/dataclass/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5534 2024-05-07 16:28:15.000000 xsdata-24.5/xsdata/formats/dataclass/compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10591 2024-05-07 16:28:15.000000 xsdata-24.5/xsdata/formats/dataclass/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32362 2024-05-07 16:28:15.000000 xsdata-24.5/xsdata/formats/dataclass/filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10032 2024-05-07 16:28:15.000000 xsdata-24.5/xsdata/formats/dataclass/generator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 16:28:25.891989 xsdata-24.5/xsdata/formats/dataclass/models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 16:28:15.000000 xsdata-24.5/xsdata/formats/dataclass/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19251 2024-05-07 16:28:15.000000 xsdata-24.5/xsdata/formats/dataclass/models/builders.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18544 2024-05-07 16:28:15.000000 xsdata-24.5/xsdata/formats/dataclass/models/elements.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1255 2024-05-07 16:28:15.000000 xsdata-24.5/xsdata/formats/dataclass/models/generics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 16:28:25.895989 xsdata-24.5/xsdata/formats/dataclass/parsers/
+-rw-r--r--   0 runner    (1001) docker     (127)      366 2024-05-07 16:28:15.000000 xsdata-24.5/xsdata/formats/dataclass/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7457 2024-05-07 16:28:15.000000 xsdata-24.5/xsdata/formats/dataclass/parsers/bases.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1555 2024-05-07 16:28:15.000000 xsdata-24.5/xsdata/formats/dataclass/parsers/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15298 2024-05-07 16:28:15.000000 xsdata-24.5/xsdata/formats/dataclass/parsers/dict.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 16:28:25.895989 xsdata-24.5/xsdata/formats/dataclass/parsers/handlers/
+-rw-r--r--   0 runner    (1001) docker     (127)      629 2024-05-07 16:28:15.000000 xsdata-24.5/xsdata/formats/dataclass/parsers/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2749 2024-05-07 16:28:15.000000 xsdata-24.5/xsdata/formats/dataclass/parsers/handlers/lxml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5300 2024-05-07 16:28:15.000000 xsdata-24.5/xsdata/formats/dataclass/parsers/handlers/native.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3207 2024-05-07 16:28:15.000000 xsdata-24.5/xsdata/formats/dataclass/parsers/json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9214 2024-05-07 16:28:15.000000 xsdata-24.5/xsdata/formats/dataclass/parsers/mixins.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 16:28:25.895989 xsdata-24.5/xsdata/formats/dataclass/parsers/nodes/
+-rw-r--r--   0 runner    (1001) docker     (127)      642 2024-05-07 16:28:15.000000 xsdata-24.5/xsdata/formats/dataclass/parsers/nodes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20133 2024-05-07 16:28:15.000000 xsdata-24.5/xsdata/formats/dataclass/parsers/nodes/element.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2195 2024-05-07 16:28:15.000000 xsdata-24.5/xsdata/formats/dataclass/parsers/nodes/primitive.py
+-rw-r--r--   0 runner    (1001) docker     (127)      613 2024-05-07 16:28:15.000000 xsdata-24.5/xsdata/formats/dataclass/parsers/nodes/skip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2357 2024-05-07 16:28:15.000000 xsdata-24.5/xsdata/formats/dataclass/parsers/nodes/standard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5715 2024-05-07 16:28:15.000000 xsdata-24.5/xsdata/formats/dataclass/parsers/nodes/union.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4003 2024-05-07 16:28:15.000000 xsdata-24.5/xsdata/formats/dataclass/parsers/nodes/wildcard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1711 2024-05-07 16:28:15.000000 xsdata-24.5/xsdata/formats/dataclass/parsers/nodes/wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2435 2024-05-07 16:28:15.000000 xsdata-24.5/xsdata/formats/dataclass/parsers/tree.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6115 2024-05-07 16:28:15.000000 xsdata-24.5/xsdata/formats/dataclass/parsers/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3927 2024-05-07 16:28:15.000000 xsdata-24.5/xsdata/formats/dataclass/parsers/xml.py
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-07 16:28:15.000000 xsdata-24.5/xsdata/formats/dataclass/ruff.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 16:28:25.899989 xsdata-24.5/xsdata/formats/dataclass/serializers/
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-05-07 16:28:15.000000 xsdata-24.5/xsdata/formats/dataclass/serializers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5781 2024-05-07 16:28:15.000000 xsdata-24.5/xsdata/formats/dataclass/serializers/code.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2180 2024-05-07 16:28:15.000000 xsdata-24.5/xsdata/formats/dataclass/serializers/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3160 2024-05-07 16:28:15.000000 xsdata-24.5/xsdata/formats/dataclass/serializers/dict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1168 2024-05-07 16:28:15.000000 xsdata-24.5/xsdata/formats/dataclass/serializers/json.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33720 2024-05-07 16:28:15.000000 xsdata-24.5/xsdata/formats/dataclass/serializers/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-05-07 16:28:15.000000 xsdata-24.5/xsdata/formats/dataclass/serializers/tree.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 16:28:25.899989 xsdata-24.5/xsdata/formats/dataclass/serializers/writers/
+-rw-r--r--   0 runner    (1001) docker     (127)      493 2024-05-07 16:28:15.000000 xsdata-24.5/xsdata/formats/dataclass/serializers/writers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2901 2024-05-07 16:28:15.000000 xsdata-24.5/xsdata/formats/dataclass/serializers/writers/lxml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3264 2024-05-07 16:28:15.000000 xsdata-24.5/xsdata/formats/dataclass/serializers/writers/native.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-05-07 16:28:15.000000 xsdata-24.5/xsdata/formats/dataclass/serializers/xml.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 16:28:25.899989 xsdata-24.5/xsdata/formats/dataclass/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     2350 2024-05-07 16:28:15.000000 xsdata-24.5/xsdata/formats/dataclass/templates/class.jinja2
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-07 16:28:15.000000 xsdata-24.5/xsdata/formats/dataclass/templates/docstrings.accessible.jinja2
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 16:28:15.000000 xsdata-24.5/xsdata/formats/dataclass/templates/docstrings.blank.jinja2
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-05-07 16:28:15.000000 xsdata-24.5/xsdata/formats/dataclass/templates/docstrings.google.jinja2
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-05-07 16:28:15.000000 xsdata-24.5/xsdata/formats/dataclass/templates/docstrings.numpy.jinja2
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-05-07 16:28:15.000000 xsdata-24.5/xsdata/formats/dataclass/templates/docstrings.rst.jinja2
+-rw-r--r--   0 runner    (1001) docker     (127)      781 2024-05-07 16:28:15.000000 xsdata-24.5/xsdata/formats/dataclass/templates/enum.jinja2
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2024-05-07 16:28:15.000000 xsdata-24.5/xsdata/formats/dataclass/templates/imports.jinja2
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-07 16:28:15.000000 xsdata-24.5/xsdata/formats/dataclass/templates/module.jinja2
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-05-07 16:28:15.000000 xsdata-24.5/xsdata/formats/dataclass/templates/package.jinja2
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-07 16:28:15.000000 xsdata-24.5/xsdata/formats/dataclass/templates/service.jinja2
+-rw-r--r--   0 runner    (1001) docker     (127)     2461 2024-05-07 16:28:15.000000 xsdata-24.5/xsdata/formats/dataclass/transports.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5823 2024-05-07 16:28:15.000000 xsdata-24.5/xsdata/formats/dataclass/typing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3280 2024-05-07 16:28:15.000000 xsdata-24.5/xsdata/formats/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-07 16:28:15.000000 xsdata-24.5/xsdata/formats/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-07 16:28:15.000000 xsdata-24.5/xsdata/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 16:28:25.899989 xsdata-24.5/xsdata/models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 16:28:15.000000 xsdata-24.5/xsdata/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17867 2024-05-07 16:28:15.000000 xsdata-24.5/xsdata/models/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21018 2024-05-07 16:28:15.000000 xsdata-24.5/xsdata/models/datatype.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3121 2024-05-07 16:28:15.000000 xsdata-24.5/xsdata/models/dtd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9943 2024-05-07 16:28:15.000000 xsdata-24.5/xsdata/models/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7288 2024-05-07 16:28:15.000000 xsdata-24.5/xsdata/models/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9908 2024-05-07 16:28:15.000000 xsdata-24.5/xsdata/models/wsdl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33275 2024-05-07 16:28:15.000000 xsdata-24.5/xsdata/models/xsd.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 16:28:15.000000 xsdata-24.5/xsdata/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 16:28:25.903989 xsdata-24.5/xsdata/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)     4067 2024-05-07 16:28:15.000000 xsdata-24.5/xsdata/schemas/mathml3-common.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)    28457 2024-05-07 16:28:15.000000 xsdata-24.5/xsdata/schemas/mathml3-content.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)    84129 2024-05-07 16:28:15.000000 xsdata-24.5/xsdata/schemas/mathml3-presentation.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)     6846 2024-05-07 16:28:15.000000 xsdata-24.5/xsdata/schemas/mathml3-strict-content.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)      436 2024-05-07 16:28:15.000000 xsdata-24.5/xsdata/schemas/mathml3.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)     8051 2024-05-07 16:28:15.000000 xsdata-24.5/xsdata/schemas/xlink.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-05-07 16:28:15.000000 xsdata-24.5/xsdata/schemas/xml.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-05-07 16:28:15.000000 xsdata-24.5/xsdata/schemas/xsi.xsd
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 16:28:25.903989 xsdata-24.5/xsdata/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 16:28:15.000000 xsdata-24.5/xsdata/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5005 2024-05-07 16:28:15.000000 xsdata-24.5/xsdata/utils/click.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3093 2024-05-07 16:28:15.000000 xsdata-24.5/xsdata/utils/collections.py
+-rw-r--r--   0 runner    (1001) docker     (127)      435 2024-05-07 16:28:15.000000 xsdata-24.5/xsdata/utils/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8011 2024-05-07 16:28:15.000000 xsdata-24.5/xsdata/utils/dates.py
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-05-07 16:28:15.000000 xsdata-24.5/xsdata/utils/debug.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4999 2024-05-07 16:28:15.000000 xsdata-24.5/xsdata/utils/downloader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-05-07 16:28:15.000000 xsdata-24.5/xsdata/utils/graphs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2024-05-07 16:28:15.000000 xsdata-24.5/xsdata/utils/hooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4779 2024-05-07 16:28:15.000000 xsdata-24.5/xsdata/utils/namespaces.py
+-rw-r--r--   0 runner    (1001) docker     (127)      763 2024-05-07 16:28:15.000000 xsdata-24.5/xsdata/utils/objects.py
+-rw-r--r--   0 runner    (1001) docker     (127)      868 2024-05-07 16:28:15.000000 xsdata-24.5/xsdata/utils/package.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17119 2024-05-07 16:28:15.000000 xsdata-24.5/xsdata/utils/testing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4918 2024-05-07 16:28:15.000000 xsdata-24.5/xsdata/utils/text.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 16:28:25.907989 xsdata-24.5/xsdata.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6011 2024-05-07 16:28:25.000000 xsdata-24.5/xsdata.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    16479 2024-05-07 16:28:25.000000 xsdata-24.5/xsdata.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 16:28:25.000000 xsdata-24.5/xsdata.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-07 16:28:25.000000 xsdata-24.5/xsdata.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-05-07 16:28:25.000000 xsdata-24.5/xsdata.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-07 16:28:25.000000 xsdata-24.5/xsdata.egg-info/top_level.txt
```

### Comparing `xsdata-24.4/CHANGES.md` & `xsdata-24.5/CHANGES.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,27 @@
+## 24.5 (2024-05-07)
+
+**Features**
+
+- Rewrite TreeSerializer, drop support for native python ElementTree
+  ([#1032](https://github.com/tefra/xsdata/pull/1032))
+- Validate fields fixed values ([#1013](https://github.com/tefra/xsdata/pull/1013))
+- Detect optional fields in dict mapper
+- Refactor typing annotations analyze process
+- Generate ForwardRef() instead of Type[]
+
+**Fixes**
+
+- Allow soap client config subclassing
+  ([#1010](https://github.com/tefra/xsdata/pull/1010))
+- Avoid recursive error on nested group references
+  ([#1016](https://github.com/tefra/xsdata/pull/1016))
+- Add warning for same module designation
+  ([#1018](https://github.com/tefra/xsdata/pull/1018))
+
 ## 24.4 (2024-04-01)
 
 **Features**
 
 - Add xml and lxml tree serializers ([#975](https://github.com/tefra/xsdata/pull/975))
 - Capture namespace prefixes in user dicts
   ([#978](https://github.com/tefra/xsdata/pull/978))
```

### Comparing `xsdata-24.4/LICENSE` & `xsdata-24.5/LICENSE`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/PKG-INFO` & `xsdata-24.5/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xsdata
-Version: 24.4
+Version: 24.5
 Summary: Python XML Binding
 Author-email: Christodoulos Tsoulloftas <chris@komposta.net>
 License: MIT
 Project-URL: Homepage, https://github.com/tefra/xsdata
 Project-URL: Source, https://github.com/tefra/xsdata
 Project-URL: Documentation, https://xsdata.readthedocs.io/
 Project-URL: Changelog, https://xsdata.readthedocs.io/en/latest/changelog/
@@ -128,48 +128,26 @@
 - XML and JSON parser, serializer
 - PyCode serializer
 - Handlers and Writers based on lxml and native xml python
 - Support wildcard elements and attributes
 - Support xinclude statements and unknown properties
 - Customize behaviour through config
 
-## Changelog: 24.3.1 (2024-03-10)
-
-**Fixes**
-
-- Unnest class with circular reference
-  ([#974](https://github.com/tefra/xsdata/pull/974))
-
-## Changelog: 24.4 (2024-04-01)
+## Changelog: 24.5 (2024-05-07)
 
 **Features**
 
-- Add xml and lxml tree serializers ([#975](https://github.com/tefra/xsdata/pull/975))
-- Capture namespace prefixes in user dicts
-  ([#978](https://github.com/tefra/xsdata/pull/978))
-- Add cli option to generate wrapper fields
-  ([#982](https://github.com/tefra/xsdata/pull/982))
-- Support wrapper fields in JSON data bindings
-  ([#982](https://github.com/tefra/xsdata/pull/982))
-- Use abstract suffixes to resolve class name conflicts
-  ([#985](https://github.com/tefra/xsdata/pull/985))
-- Add the version number in the cli cache key
-  ([#990](https://github.com/tefra/xsdata/pull/990))
-- Use unicodedata.name for attrs with only special characters
-  ([#993](https://github.com/tefra/xsdata/pull/993))
-- Add src code excerpts on ruff errors
-  ([#996](https://github.com/tefra/xsdata/pull/996))
-- Detect circular imports and raise appropriate error
-  ([#999](https://github.com/tefra/xsdata/pull/999))
-- Add support for Python 3.13 ([#1001](https://github.com/tefra/xsdata/pull/1001))
-- Add cli debug messages with performance stats
+- Rewrite TreeSerializer, drop support for native python ElementTree
+  ([#1032](https://github.com/tefra/xsdata/pull/1032))
+- Validate fields fixed values ([#1013](https://github.com/tefra/xsdata/pull/1013))
+- Detect optional fields in dict mapper
+- Refactor typing annotations analyze process
+- Generate ForwardRef() instead of Type[]
 
 **Fixes**
 
-- Use deepcopy to clone codegen models
-  ([#980](https://github.com/tefra/xsdata/pull/980))
-- Generate type hints for compound fields with token elements
-  ([#997](https://github.com/tefra/xsdata/pull/997))
-- Protect prohibited attrs from turning into lists
-  ([#998](https://github.com/tefra/xsdata/pull/998))
-- Convert child attr to list when parent is list
-  ([#998](https://github.com/tefra/xsdata/pull/998))
+- Allow soap client config subclassing
+  ([#1010](https://github.com/tefra/xsdata/pull/1010))
+- Avoid recursive error on nested group references
+  ([#1016](https://github.com/tefra/xsdata/pull/1016))
+- Add warning for same module designation
+  ([#1018](https://github.com/tefra/xsdata/pull/1018))
```

### Comparing `xsdata-24.4/docs/codegen/architecture.md` & `xsdata-24.5/docs/codegen/architecture.md`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/docs/codegen/config.md` & `xsdata-24.5/docs/codegen/config.md`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/docs/codegen/docstrings.md` & `xsdata-24.5/docs/codegen/docstrings.md`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/docs/codegen/dtd_modeling.md` & `xsdata-24.5/docs/codegen/dtd_modeling.md`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/docs/codegen/intro.md` & `xsdata-24.5/docs/codegen/intro.md`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/docs/codegen/samples_modeling.md` & `xsdata-24.5/docs/codegen/samples_modeling.md`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/docs/codegen/wsdl_modeling.md` & `xsdata-24.5/docs/codegen/wsdl_modeling.md`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/docs/data_binding/basics.md` & `xsdata-24.5/docs/data_binding/basics.md`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/docs/data_binding/dict_decoding.md` & `xsdata-24.5/docs/data_binding/dict_decoding.md`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/docs/data_binding/dict_encoding.md` & `xsdata-24.5/docs/data_binding/dict_encoding.md`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/docs/data_binding/json_parsing.md` & `xsdata-24.5/docs/data_binding/json_parsing.md`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/docs/data_binding/json_serializing.md` & `xsdata-24.5/docs/data_binding/json_serializing.md`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/docs/data_binding/pycode_serializing.md` & `xsdata-24.5/docs/data_binding/pycode_serializing.md`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/docs/data_binding/xml_parsing.md` & `xsdata-24.5/docs/data_binding/xml_parsing.md`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/docs/data_binding/xml_serializing.md` & `xsdata-24.5/docs/data_binding/xml_serializing.md`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/docs/faq.md` & `xsdata-24.5/docs/faq.md`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/docs/installation.md` & `xsdata-24.5/docs/installation.md`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/docs/logo-small.svg` & `xsdata-24.5/docs/logo-small.svg`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/docs/logo.svg` & `xsdata-24.5/docs/logo.svg`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/docs/models/classes.md` & `xsdata-24.5/docs/models/classes.md`

 * *Files 3% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 ...         name = "xsdata"
 ...
 >>> print(serializer.render(Root()))
 <xsdata/>
 
 ```
 
-**Type:** `srt`
+**Type:** `str`
 
 **Default:** `The class name`
 
 ### `namespace`
 
 The namespace name of the XML element
 
@@ -62,15 +62,15 @@
 ...         namespace = "xsdata"
 ...
 >>> print(serializer.render(Root()))
 <ns0:Root xmlns:ns0="xsdata"/>
 
 ```
 
-**Type:** `srt | None`
+**Type:** `str | None`
 
 **Default:** `None`
 
 ### `nillable`
 
 Specify if the attribute `xsi:nil="true"` is needed when the class is serialized and it
 doesn't have any meaningful content.
@@ -98,15 +98,15 @@
 **Default:** `False`
 
 ### `target_namespace`
 
 The namespace name, the XML element was defined under. Used during auto-type discovery
 when the element form is `unqualified`.
 
-**Type:** `srt | None`
+**Type:** `str | None`
 
 **Default:** `None`
 
 ### `global_type`
 
 Specify if the class represents an element that can appear in the document root. When
 false the class can be used only another class dependency, and it's excluded from
```

### Comparing `xsdata-24.4/docs/models/fields.md` & `xsdata-24.5/docs/models/fields.md`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 <Root>
   <one>xml</one>
   <two>json</two>
 </Root>
 
 ```
 
-**Type:** `srt`
+**Type:** `str`
 
 **Default:** `The field name`
 
 ### `namespace`
 
 The namespace name of the XML element or attribute.
```

### Comparing `xsdata-24.4/docs/models/types.md` & `xsdata-24.5/docs/models/types.md`

 * *Files 2% similar despite different names*

```diff
@@ -21,27 +21,25 @@
 ### List
 
 `typing.List`
 
 | Case           | Example                                                                           |
 | -------------- | --------------------------------------------------------------------------------- |
 | List           | `value: List[str] = field(default_factory=list)`                                  |
-| Optional List  | `value: Optional[List[str]] = field(default=None)`                                |
 | List Union     | `value: List[Union[str, int]] = field(default_factory=list)`                      |
 | Tokens List    | `value: List[str] = field(default_factory=list, metadata={"tokens": True})`       |
 | List of Tokens | `value: List[List[str]] = field(default_factory=list, metadata={"tokens": True})` |
 
 ### Tuple
 
 `typing.Tuple` can be use in `frozen` dataclasses, for immutable instances.
 
 | Case            | Example                                                                                        |
 | --------------- | ---------------------------------------------------------------------------------------------- |
 | Tuple           | `value: Tuple[str, ...] = field(default_factory=tuple)`                                        |
-| Optional Tuple  | `value: Optional[Tuple[str, ...]] = field(default=None)`                                       |
 | Tuple Union     | `value: Tuple[Union[str, int], ...] = field(default_factory=tuple)`                            |
 | Tokens Tuple    | `value: Tuple[str, ...] = field(default_factory=tuple, metadata={"tokens": True})`             |
 | Tuple of Tokens | `value: Tuple[Tuple[str, ...], ...] = field(default_factory=tuple, metadata={"tokens": True})` |
 
 ### Dict
 
 `typing.Dict` is reserved for `Attributes` type fields to capture any undefined
```

### Comparing `xsdata-24.4/docs/plugins/how_to.md` & `xsdata-24.5/docs/plugins/how_to.md`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/docs/plugins/list.md` & `xsdata-24.5/docs/plugins/list.md`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/docs/samples.md` & `xsdata-24.5/docs/samples.md`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/docs/scripts/generate_api.py` & `xsdata-24.5/docs/scripts/generate_api.py`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/pyproject.toml` & `xsdata-24.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/tests/codegen/handlers/test_add_attribute_substitutions.py` & `xsdata-24.5/tests/codegen/handlers/test_add_attribute_substitutions.py`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/tests/codegen/handlers/test_calculate_attribute_paths.py` & `xsdata-24.5/tests/codegen/handlers/test_calculate_attribute_paths.py`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/tests/codegen/handlers/test_create_compound_fields.py` & `xsdata-24.5/tests/codegen/handlers/test_create_compound_fields.py`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/tests/codegen/handlers/test_create_wrapper_fields.py` & `xsdata-24.5/tests/codegen/handlers/test_create_wrapper_fields.py`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/tests/codegen/handlers/test_designate_class_packages.py` & `xsdata-24.5/tests/codegen/handlers/test_designate_class_packages.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,47 +19,51 @@
         self.handler = DesignateClassPackages(container=self.container)
 
     def test_group_by_filenames(self):
         voc = "file://HL7V3/NE2008/coreschemas/voc.xsd"
         prpa = "file://HL7V3/NE2008/multicacheschemas/PRPA_MT201307UV02.xsd"
         coct = "file://HL7V3/NE2008/multicacheschemas/COCT_MT080000UV.xsd"
         foo_bar = "http://xsdata/foo/bar/schema.xsd"
+        foo_wsdl = "http://xsdata/foo/bar/schema.wsdl"
         foo_common = "http://xsdata/foo/common.xsd"
         xsi = Namespace.XSI.location
         xlink = Namespace.XLINK.location
 
         core = ClassFactory.list(1, inner=[ClassFactory.create()], location=voc)
         multi_one = ClassFactory.list(2, location=prpa)
         multi_two = ClassFactory.list(1, location=coct)
         http_one = ClassFactory.list(1, location=foo_bar)
+        wsdl_one = ClassFactory.list(1, location=foo_wsdl)
         http_two = ClassFactory.list(1, location=foo_common)
         local_one = ClassFactory.list(1, location=xsi)
         local_two = ClassFactory.list(1, location=xlink)
 
         self.container.extend(core)
         self.container.extend(multi_one)
         self.container.extend(multi_two)
         self.container.extend(http_one)
+        self.container.extend(wsdl_one)
         self.container.extend(http_two)
         self.container.extend(local_one)
         self.container.extend(local_two)
 
-        self.config.output.package = "foo.bar"
+        self.config.output.package = "foo"
 
         self.handler.run()
 
-        self.assertEqual("foo.bar.coreschemas", core[0].package)
-        self.assertEqual("foo.bar.coreschemas", core[0].inner[0].package)
-        self.assertEqual("foo.bar.multicacheschemas", multi_one[0].package)
-        self.assertEqual("foo.bar.multicacheschemas", multi_one[1].package)
-        self.assertEqual("foo.bar.multicacheschemas", multi_two[0].package)
-        self.assertEqual("foo.bar.bar", http_one[0].package)
-        self.assertEqual("foo.bar", http_two[0].package)
-        self.assertEqual("foo.bar", local_one[0].package)
-        self.assertEqual("foo.bar", local_two[0].package)
+        self.assertEqual("foo.coreschemas", core[0].package)
+        self.assertEqual("foo.coreschemas", core[0].inner[0].package)
+        self.assertEqual("foo.multicacheschemas", multi_one[0].package)
+        self.assertEqual("foo.multicacheschemas", multi_one[1].package)
+        self.assertEqual("foo.multicacheschemas", multi_two[0].package)
+        self.assertEqual("foo.bar", http_one[0].package)
+        self.assertEqual("foo", http_two[0].package)
+        self.assertEqual("foo.bar", wsdl_one[0].package)
+        self.assertEqual("foo", local_one[0].package)
+        self.assertEqual("foo", local_two[0].package)
 
     def test_group_by_namespace(self):
         classes = [
             ClassFactory.create(qname="{myNS.tempuri.org}a", location="foo"),
             ClassFactory.create(qname="{myNS.tempuri.org}b", location="foo"),
             ClassFactory.create(qname="b", location="bar"),
         ]
```

### Comparing `xsdata-24.4/tests/codegen/handlers/test_detect_circular_references.py` & `xsdata-24.5/tests/codegen/handlers/test_detect_circular_references.py`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/tests/codegen/handlers/test_disambiguate_choices.py` & `xsdata-24.5/tests/codegen/handlers/test_disambiguate_choices.py`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/tests/codegen/handlers/test_filter_classes.py` & `xsdata-24.5/tests/codegen/handlers/test_filter_classes.py`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/tests/codegen/handlers/test_flatten_class_extensions.py` & `xsdata-24.5/tests/codegen/handlers/test_flatten_class_extensions.py`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/tests/codegen/handlers/test_merge_attributes.py` & `xsdata-24.5/tests/codegen/handlers/test_merge_attributes.py`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/tests/codegen/handlers/test_process_attributes_types.py` & `xsdata-24.5/tests/codegen/handlers/test_process_attributes_types.py`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/tests/codegen/handlers/test_process_mixed_content_class.py` & `xsdata-24.5/tests/codegen/handlers/test_process_mixed_content_class.py`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/tests/codegen/handlers/test_rename_duplicate_attributes.py` & `xsdata-24.5/tests/codegen/handlers/test_rename_duplicate_attributes.py`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/tests/codegen/handlers/test_rename_duplicate_classes.py` & `xsdata-24.5/tests/codegen/handlers/test_rename_duplicate_classes.py`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/tests/codegen/handlers/test_reset_attribute_sequence_numbers.py` & `xsdata-24.5/tests/codegen/handlers/test_reset_attribute_sequence_numbers.py`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/tests/codegen/handlers/test_reset_attribute_sequences.py` & `xsdata-24.5/tests/codegen/handlers/test_reset_attribute_sequences.py`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/tests/codegen/handlers/test_sanitize_attributes_default_value.py` & `xsdata-24.5/tests/codegen/handlers/test_sanitize_attributes_default_value.py`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/tests/codegen/handlers/test_sanitize_enumeration_class.py` & `xsdata-24.5/tests/codegen/handlers/test_sanitize_enumeration_class.py`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/tests/codegen/handlers/test_unnest_inner_classes.py` & `xsdata-24.5/tests/codegen/handlers/test_unnest_inner_classes.py`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/tests/codegen/handlers/test_update_attributes_effective_choice.py` & `xsdata-24.5/tests/codegen/handlers/test_update_attributes_effective_choice.py`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/tests/codegen/handlers/test_vacuum_inner_classes.py` & `xsdata-24.5/tests/codegen/handlers/test_vacuum_inner_classes.py`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/tests/codegen/handlers/test_validate_attributes_overrides.py` & `xsdata-24.5/tests/codegen/handlers/test_validate_attributes_overrides.py`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/tests/codegen/handlers/test_validate_references.py` & `xsdata-24.5/tests/codegen/handlers/test_validate_references.py`

 * *Files 16% similar despite different names*

```diff
@@ -56,7 +56,41 @@
                 types=[AttrTypeFactory.create(qname="foo", reference=inner.ref)]
             )
         )
         self.container.add(first)
 
         with self.assertRaises(CodegenError):
             self.handler.run()
+
+    def test_validate_parent_references_with_root_class_with_parent(self):
+        target = ClassFactory.create()
+        target.parent = ClassFactory.create()
+        self.container.add(target)
+
+        with self.assertRaises(CodegenError):
+            self.handler.run()
+
+    def test_validate_parent_references_with_wrong_parent(self):
+        parent = ClassFactory.create()
+        child = ClassFactory.create()
+        wrong = ClassFactory.create()
+
+        parent.inner.append(child)
+        child.parent = wrong
+
+        self.container.extend([parent, wrong])
+
+        with self.assertRaises(CodegenError):
+            self.handler.run()
+
+    def test_validate_parent_references_with_wrong_parent_ref(self):
+        parent = ClassFactory.create()
+        child = ClassFactory.create()
+        wrong = parent.clone()
+
+        parent.inner.append(child)
+        child.parent = wrong
+
+        self.container.extend([parent])
+
+        with self.assertRaises(CodegenError):
+            self.handler.run()
```

### Comparing `xsdata-24.4/tests/codegen/mappers/test_definitions.py` & `xsdata-24.5/tests/codegen/mappers/test_definitions.py`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/tests/codegen/mappers/test_dict.py` & `xsdata-24.5/tests/codegen/mappers/test_dict.py`

 * *Files 10% similar despite different names*

```diff
@@ -85,21 +85,21 @@
         expected = AttrFactory.create(
             name="a",
             tag=Tag.ELEMENT,
             types=[
                 AttrTypeFactory.native(DataType.ANY_SIMPLE_TYPE, tag=Tag.ELEMENT),
             ],
         )
-        restrictions = Restrictions(min_occurs=1, max_occurs=sys.maxsize)
+        restrictions = Restrictions(min_occurs=0, max_occurs=sys.maxsize)
         self.assertEqual(expected, target.attrs[0])
         self.assertEqual(restrictions, target.attrs[0].restrictions)
 
     def test_build_class_attribute_from_dict(self):
         target = ClassFactory.create()
-        data = {"sub1": 1, "sub2": "value"}
+        data = {"sub1": 1, "sub2": "value", "sub3": None}
         DictMapper.build_class_attribute(target, "a", data)
 
         expected = AttrFactory.create(
             name="a",
             tag=Tag.ELEMENT,
             types=[AttrTypeFactory.create(qname="a", forward=True)],
         )
@@ -109,13 +109,18 @@
             tag=Tag.ELEMENT,
             location="",
             module=None,
             ns_map={},
             attrs=[
                 AttrFactory.native(DataType.SHORT, name="sub1"),
                 AttrFactory.native(DataType.STRING, name="sub2"),
+                AttrFactory.native(DataType.STRING, name="sub3"),
             ],
         )
 
         self.assertEqual(expected, target.attrs[0])
         self.assertEqual(expected_inner, target.inner[0])
         self.assertEqual(1, len(target.inner))
+
+        self.assertFalse(target.inner[0].attrs[0].restrictions.is_optional)
+        self.assertFalse(target.inner[0].attrs[1].restrictions.is_optional)
+        self.assertTrue(target.inner[0].attrs[2].restrictions.is_optional)
```

### Comparing `xsdata-24.4/tests/codegen/mappers/test_dtd.py` & `xsdata-24.5/tests/codegen/mappers/test_dtd.py`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/tests/codegen/mappers/test_element.py` & `xsdata-24.5/tests/codegen/mappers/test_element.py`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/tests/codegen/mappers/test_schema.py` & `xsdata-24.5/tests/codegen/mappers/test_schema.py`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/tests/codegen/models/test_attr.py` & `xsdata-24.5/tests/codegen/models/test_attr.py`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/tests/codegen/models/test_attr_type.py` & `xsdata-24.5/tests/codegen/models/test_attr_type.py`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/tests/codegen/models/test_class.py` & `xsdata-24.5/tests/codegen/models/test_class.py`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/tests/codegen/models/test_codegen.py` & `xsdata-24.5/tests/codegen/models/test_codegen.py`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/tests/codegen/models/test_restrictions.py` & `xsdata-24.5/tests/codegen/models/test_restrictions.py`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/tests/codegen/parsers/test_definitions.py` & `xsdata-24.5/tests/codegen/parsers/test_definitions.py`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/tests/codegen/parsers/test_dtd.py` & `xsdata-24.5/tests/codegen/parsers/test_dtd.py`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/tests/codegen/parsers/test_schema.py` & `xsdata-24.5/tests/codegen/parsers/test_schema.py`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/tests/codegen/test_container.py` & `xsdata-24.5/tests/codegen/test_container.py`

 * *Files 2% similar despite different names*

```diff
@@ -110,14 +110,17 @@
         with self.assertRaises(KeyError):
             self.container.first("aa")
 
     def test_process_class(self):
         target = ClassFactory.create(
             inner=[ClassFactory.elements(2), ClassFactory.elements(1)]
         )
+        for inner in target.inner:
+            inner.parent = target
+
         self.container.add(target)
 
         self.container.process()
         self.assertEqual(Status.FINALIZED, target.status)
         self.assertEqual(Status.FINALIZED, target.inner[0].status)
         self.assertEqual(Status.FINALIZED, target.inner[1].status)
```

### Comparing `xsdata-24.4/tests/codegen/test_resolver.py` & `xsdata-24.5/tests/codegen/test_resolver.py`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/tests/codegen/test_transformer.py` & `xsdata-24.5/tests/codegen/test_transformer.py`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/tests/codegen/test_utils.py` & `xsdata-24.5/tests/codegen/test_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -210,28 +210,14 @@
         source = ClassFactory.create()
         target = ClassFactory.create()
         attr_type = AttrTypeFactory.create(forward=True, qname=target.qname)
 
         with self.assertRaises(CodegenError):
             ClassUtils.copy_inner_class(source, target, attr_type)
 
-    def test_find_inner(self):
-        obj = ClassFactory.create(qname="{a}parent")
-        first = ClassFactory.create(qname="{a}a")
-        second = ClassFactory.create(qname="{c}c")
-        third = ClassFactory.enumeration(2, qname="{d}d")
-        obj.inner.extend((first, second, third))
-
-        with self.assertRaises(CodegenError):
-            self.assertIsNone(ClassUtils.find_inner(obj, "nope"))
-
-        self.assertEqual(first, ClassUtils.find_inner(obj, "{a}a"))
-        self.assertEqual(second, ClassUtils.find_inner(obj, "{c}c"))
-        self.assertEqual(third, ClassUtils.find_inner(obj, "{d}d"))
-
     def test_flatten(self):
         target = ClassFactory.create(
             qname="{xsdata}root", attrs=AttrFactory.list(3), inner=ClassFactory.list(2)
         )
 
         for attr in target.attrs:
             attr.types.extend([x.clone() for x in attr.types])
@@ -396,7 +382,32 @@
 
         actual = ClassUtils.filter_types([])
         self.assertEqual(xs_string, actual[0])
 
         types = [xs_any]
         actual = ClassUtils.filter_types(types)
         self.assertEqual(1, len(actual))
+
+    def test_find_nested(self):
+        a = ClassFactory.create(qname="a")
+        b = ClassFactory.create(qname="b")
+        c = ClassFactory.create(qname="c")
+
+        a.inner.append(b)
+        b.inner.append(c)
+        c.parent = b
+        b.parent = a
+
+        self.assertEqual(a, ClassUtils.find_nested(a, "a"))
+        self.assertEqual(b, ClassUtils.find_nested(a, "b"))
+        self.assertEqual(b, ClassUtils.find_nested(c, "b"))
+        self.assertEqual(a, ClassUtils.find_nested(c, "a"))
+
+        a2 = ClassFactory.create(qname="a")
+        c.inner.append(a2)
+        a2.parent = c
+
+        # Breadth-first search
+        self.assertEqual(a2, ClassUtils.find_nested(c, "a"))
+
+        with self.assertRaises(CodegenError):
+            ClassUtils.find_nested(a, "nope")
```

### Comparing `xsdata-24.4/tests/codegen/test_validator.py` & `xsdata-24.5/tests/codegen/test_validator.py`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/tests/codegen/test_writer.py` & `xsdata-24.5/tests/codegen/test_writer.py`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/tests/conftest.py` & `xsdata-24.5/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/tests/fixtures/annotations/model.py` & `xsdata-24.5/tests/fixtures/annotations/model.py`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/tests/fixtures/annotations/model.xsd` & `xsdata-24.5/tests/fixtures/annotations/model.xsd`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/tests/fixtures/annotations/units.xsd` & `xsdata-24.5/tests/fixtures/annotations/units.xsd`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/tests/fixtures/annotations/xsdata.xml` & `xsdata-24.5/tests/fixtures/annotations/xsdata.xml`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/tests/fixtures/artists/art001.xml` & `xsdata-24.5/tests/fixtures/artists/art001.xml`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/tests/fixtures/artists/art002.xml` & `xsdata-24.5/tests/fixtures/artists/art002.xml`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/tests/fixtures/artists/art003.xml` & `xsdata-24.5/tests/fixtures/artists/art003.xml`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/tests/fixtures/artists/metadata.py` & `xsdata-24.5/tests/fixtures/artists/metadata.py`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/tests/fixtures/books/books.py` & `xsdata-24.5/tests/fixtures/books/books.py`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/tests/fixtures/books/books.xml` & `xsdata-24.5/tests/fixtures/books/books.xml`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/tests/fixtures/books/books_auto_ns.xml` & `xsdata-24.5/tests/fixtures/books/books_auto_ns.xml`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/tests/fixtures/books/books_default_ns.xml` & `xsdata-24.5/tests/fixtures/books/books_default_ns.xml`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/tests/fixtures/books/fixtures.py` & `xsdata-24.5/tests/fixtures/books/fixtures.py`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/tests/fixtures/books/schema.xsd` & `xsdata-24.5/tests/fixtures/books/schema.xsd`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/tests/fixtures/calculator/__init__.py` & `xsdata-24.5/tests/fixtures/calculator/__init__.py`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/tests/fixtures/calculator/services.py` & `xsdata-24.5/tests/fixtures/calculator/services.py`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/tests/fixtures/calculator/services.wsdl` & `xsdata-24.5/tests/fixtures/calculator/services.wsdl`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/tests/fixtures/compound/models.py` & `xsdata-24.5/tests/fixtures/compound/models.py`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/tests/fixtures/compound/sample.py` & `xsdata-24.5/tests/fixtures/compound/sample.py`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/tests/fixtures/compound/schema.xsd` & `xsdata-24.5/tests/fixtures/compound/schema.xsd`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/tests/fixtures/datatypes.py` & `xsdata-24.5/tests/fixtures/datatypes.py`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/tests/fixtures/docstrings/accessible/schema.py` & `xsdata-24.5/tests/fixtures/docstrings/accessible/schema.py`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/tests/fixtures/docstrings/blank/schema.py` & `xsdata-24.5/tests/fixtures/docstrings/blank/schema.py`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/tests/fixtures/docstrings/google/schema.py` & `xsdata-24.5/tests/fixtures/docstrings/google/schema.py`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/tests/fixtures/docstrings/numpy/schema.py` & `xsdata-24.5/tests/fixtures/docstrings/numpy/schema.py`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/tests/fixtures/docstrings/rst/schema.py` & `xsdata-24.5/tests/fixtures/docstrings/rst/schema.py`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/tests/fixtures/docstrings/schema.xsd` & `xsdata-24.5/tests/fixtures/docstrings/schema.xsd`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/tests/fixtures/dtd/models/complete_example.py` & `xsdata-24.5/tests/fixtures/dtd/models/complete_example.py`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/tests/fixtures/hello/hello.py` & `xsdata-24.5/tests/fixtures/hello/hello.py`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/tests/fixtures/hello/hello.wsdl` & `xsdata-24.5/tests/fixtures/hello/hello.wsdl`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/tests/fixtures/hello/hello.xsd` & `xsdata-24.5/tests/fixtures/hello/hello.xsd`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/tests/fixtures/models.py` & `xsdata-24.5/tests/fixtures/models.py`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/tests/fixtures/primer/order.py` & `xsdata-24.5/tests/fixtures/primer/order.py`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/tests/fixtures/primer/order.xsd` & `xsdata-24.5/tests/fixtures/primer/order.xsd`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/tests/fixtures/primer/sample.json` & `xsdata-24.5/tests/fixtures/primer/sample.json`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/tests/fixtures/primer/sample.py` & `xsdata-24.5/tests/fixtures/primer/sample.py`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/tests/fixtures/primer/sample.xml` & `xsdata-24.5/tests/fixtures/primer/sample.xml`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/tests/fixtures/primer/sample.xsdata.xml` & `xsdata-24.5/tests/fixtures/primer/sample.xsdata.xml`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/tests/fixtures/series/samples/show1.json` & `xsdata-24.5/tests/fixtures/series/samples/show1.json`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/tests/fixtures/series/samples/show2.json` & `xsdata-24.5/tests/fixtures/series/samples/show2.json`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/tests/fixtures/series/series.py` & `xsdata-24.5/tests/fixtures/series/series.py`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/tests/fixtures/stripe/.xsdata.xml` & `xsdata-24.5/tests/fixtures/stripe/.xsdata.xml`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/tests/fixtures/stripe/models/balance.py` & `xsdata-24.5/tests/fixtures/stripe/models/balance.py`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/tests/fixtures/stripe/samples/balance.json` & `xsdata-24.5/tests/fixtures/stripe/samples/balance.json`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/tests/fixtures/wrapper/models.py` & `xsdata-24.5/tests/fixtures/wrapper/models.py`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/tests/fixtures/wrapper/schema.xsd` & `xsdata-24.5/tests/fixtures/wrapper/schema.xsd`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/tests/formats/dataclass/models/test_builders.py` & `xsdata-24.5/tests/formats/dataclass/models/test_builders.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,11 @@
-import functools
 import sys
-import uuid
 from dataclasses import dataclass, field, fields, make_dataclass
 from decimal import Decimal
-from typing import Dict, Iterator, List, Union, get_type_hints
+from typing import Iterator, List, get_type_hints
 from unittest import TestCase, mock
 from xml.etree.ElementTree import QName
 
 from tests.fixtures.artists import Artist
 from tests.fixtures.books import BookForm
 from tests.fixtures.models import (
     AmbiguousChoiceType,
@@ -444,78 +442,7 @@
         self.assertEqual(("!p",), actual)
 
         actual = func(XmlType.WILDCARD, "##other   ##local", "p")
         self.assertEqual(("", "!p"), tuple(sorted(actual)))
 
         actual = func(XmlType.WILDCARD, "##targetNamespace   foo", "p")
         self.assertEqual(("foo", "p"), tuple(sorted(actual)))
-
-    def test_analyze_types(self):
-        func = functools.partial(self.builder.analyze_types, BookForm, "foo")
-
-        actual = func(List[List[Union[str, int]]], None)
-        self.assertEqual((list, list, (int, str)), actual)
-
-        actual = func(Union[str, int], None)
-        self.assertEqual((None, None, (int, str)), actual)
-
-        actual = func(Dict[str, int], None)
-        self.assertEqual((dict, None, (int, str)), actual)
-
-        with self.assertRaises(XmlContextError) as cm:
-            func(List[List[List[int]]], None)
-
-        self.assertEqual(
-            "Error on BookForm::foo: Unsupported field typing `typing.List[typing.List[typing.List[int]]]`",
-            str(cm.exception),
-        )
-
-    def test_is_valid(self):
-        # Attributes need origin dict
-        self.assertFalse(
-            self.builder.is_valid(XmlType.ATTRIBUTES, None, None, (), False, True)
-        )
-
-        # Attributes don't support any origin
-        self.assertFalse(
-            self.builder.is_valid(XmlType.ATTRIBUTES, dict, list, (), False, True)
-        )
-
-        # Attributes don't support xs:NMTOKENS
-        self.assertFalse(
-            self.builder.is_valid(XmlType.ATTRIBUTES, dict, None, (), True, True)
-        )
-
-        self.assertTrue(
-            self.builder.is_valid(
-                XmlType.ATTRIBUTES, dict, None, (str, str), False, True
-            )
-        )
-
-        # xs:NMTOKENS need origin list
-        self.assertFalse(
-            self.builder.is_valid(XmlType.TEXT, dict, None, (), True, True)
-        )
-
-        # xs:NMTOKENS need origin list
-        self.assertFalse(self.builder.is_valid(XmlType.TEXT, set, None, (), True, True))
-
-        # Any type object is a superset, it's only supported alone
-        self.assertFalse(
-            self.builder.is_valid(
-                XmlType.ELEMENT, None, None, (object, int), False, True
-            )
-        )
-
-        # Type is not registered in converter.
-        self.assertFalse(
-            self.builder.is_valid(
-                XmlType.TEXT, None, None, (int, uuid.UUID), False, True
-            )
-        )
-
-        # init false vars are ignored!
-        self.assertTrue(
-            self.builder.is_valid(
-                XmlType.TEXT, None, None, (int, uuid.UUID), False, False
-            )
-        )
```

### Comparing `xsdata-24.4/tests/formats/dataclass/parsers/handlers/test_lxml.py` & `xsdata-24.5/tests/formats/dataclass/parsers/handlers/test_lxml.py`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/tests/formats/dataclass/parsers/handlers/test_native.py` & `xsdata-24.5/tests/formats/dataclass/parsers/handlers/test_native.py`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/tests/formats/dataclass/parsers/nodes/test_element.py` & `xsdata-24.5/tests/formats/dataclass/parsers/nodes/test_element.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,15 +79,15 @@
         self.assertTrue(self.node.bind("foo", None, None, objects))
         self.assertEqual(("foo", NillableType(None)), objects[-1])
 
     def test_bind_fixed_value(self):
         self.node.meta = self.context.build(FixedType)
 
         objects = []
-        self.assertTrue(self.node.bind("foo", "not the fixed value", None, objects))
+        self.assertTrue(self.node.bind("foo", "abc", None, objects))
         self.assertEqual(("foo", FixedType()), objects[-1])
 
     def test_bind_with_derived_element(self):
         self.node.meta = self.context.build(TypeA)
         self.node.derived_factory = DerivedElement
 
         objects = []
@@ -178,15 +178,15 @@
         self.node.bind_wild_text(params, var, "first", None)
         self.assertEqual({"wildcard": ["first", None, "txt", "tail", "tail"]}, params)
 
     def test_bind_attrs(self):
         self.node.meta = self.context.build(AttrsType)
         self.node.attrs = {
             "index": "0",
-            "fixed": "will be ignored",
+            "fixed": "ignored",
             "{what}ever": "qname",
             "extended": "attr",
         }
 
         params = {}
         self.node.bind_attrs(params)
 
@@ -194,15 +194,15 @@
         self.assertEqual(expected, params)
 
     def test_bind_attrs_with_fail_on_unknown_attributes(self):
         self.node.meta = self.context.build(AttrsType)
         self.node.config.fail_on_unknown_attributes = True
         self.node.attrs = {
             "index": "0",
-            "fixed": "will be ignored",
+            "fixed": "ignored",
             "{what}ever": "qname",
             "extended": "attr",
         }
 
         params = {}
         self.node.bind_attrs(params)
```

### Comparing `xsdata-24.4/tests/formats/dataclass/parsers/nodes/test_primitive.py` & `xsdata-24.5/tests/formats/dataclass/parsers/nodes/test_primitive.py`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/tests/formats/dataclass/parsers/nodes/test_standard.py` & `xsdata-24.5/tests/formats/dataclass/parsers/nodes/test_standard.py`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/tests/formats/dataclass/parsers/nodes/test_union.py` & `xsdata-24.5/tests/formats/dataclass/parsers/nodes/test_union.py`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/tests/formats/dataclass/parsers/nodes/test_wildcard.py` & `xsdata-24.5/tests/formats/dataclass/parsers/nodes/test_wildcard.py`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/tests/formats/dataclass/parsers/nodes/test_wrapper.py` & `xsdata-24.5/tests/formats/dataclass/parsers/nodes/test_wrapper.py`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/tests/formats/dataclass/parsers/test_dict.py` & `xsdata-24.5/tests/formats/dataclass/parsers/test_dict.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 import json
-from dataclasses import asdict, make_dataclass
+from dataclasses import asdict, dataclass, field
 from decimal import Decimal
 from typing import List, Optional, Union
 from xml.etree.ElementTree import QName
 
 from tests import fixtures_dir
 from tests.fixtures.books import BookForm, Books
 from tests.fixtures.models import (
     AttrsType,
     BaseC,
     BaseType,
     ChoiceType,
     ExtendedType,
+    FixedType,
     OptionalChoiceType,
     TypeA,
     TypeB,
     TypeC,
     TypeD,
     UnionType,
 )
@@ -169,14 +170,21 @@
         self.assertEqual(1, obj.x)
         self.assertEqual("a", obj.y)
         self.assertIsNone(obj.z)
 
         with self.assertRaises(ParserError):
             self.decoder.bind_dataclass({"x": 1, "y": "a"}, TypeD)
 
+    def test_bind_dataclass_with_fixed_field(self):
+        obj = self.decoder.bind_dataclass({"value": "abc"}, FixedType)
+        self.assertEqual("abc", obj.value)
+
+        with self.assertRaises(ParserError):
+            self.decoder.bind_dataclass({"value": "abcd"}, FixedType)
+
     def test_bind_derived_dataclass(self):
         data = {
             "qname": "{urn:books}BookForm",
             "type": None,
             "value": {
                 "author": "Nagata, Suanne",
                 "title": "Becoming Somebody",
@@ -377,15 +385,18 @@
         with self.assertRaises(ParserError) as cm:
             data["any"]["type"] = "notexists"
             self.decoder.bind_dataclass(data, ExtendedType)
 
         self.assertEqual("Unable to locate xsi:type `notexists`", str(cm.exception))
 
     def test_bind_text_with_unions(self):
-        Fixture = make_dataclass("Fixture", [("x", List[Union[int, float, str, bool]])])
+        @dataclass
+        class Fixture:
+            x: List[Union[int, float, str, bool]] = field(metadata={"tokens": True})
+
         values = ["foo", 12.2, "12.2", 12, "12", True, "false"]
 
         result = self.decoder.decode({"x": values}, Fixture)
         expected = ["foo", 12.2, 12.2, 12, 12, True, False]
         self.assertEqual({"x": expected}, asdict(result))
 
     def test_find_var(self):
```

### Comparing `xsdata-24.4/tests/formats/dataclass/parsers/test_json.py` & `xsdata-24.5/tests/formats/dataclass/parsers/test_json.py`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/tests/formats/dataclass/parsers/test_mixins.py` & `xsdata-24.5/tests/formats/dataclass/parsers/test_mixins.py`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/tests/formats/dataclass/parsers/test_node.py` & `xsdata-24.5/tests/formats/dataclass/parsers/test_node.py`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/tests/formats/dataclass/parsers/test_tree.py` & `xsdata-24.5/tests/formats/dataclass/parsers/test_tree.py`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/tests/formats/dataclass/parsers/test_utils.py` & `xsdata-24.5/tests/formats/dataclass/parsers/test_utils.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 from unittest import mock
 
+from tests.fixtures.models import TypeA
+from xsdata.exceptions import ParserError
 from xsdata.formats.converter import ConverterFactory
 from xsdata.formats.dataclass.context import XmlContext
 from xsdata.formats.dataclass.parsers.utils import ParserUtils
 from xsdata.models.enums import Namespace, QNames
-from xsdata.utils.testing import FactoryTestCase
+from xsdata.utils.testing import FactoryTestCase, XmlMetaFactory, XmlVarFactory
 
 
 class ParserUtilsTests(FactoryTestCase):
     def setUp(self) -> None:
         super().setUp()
         self.ctx = XmlContext()
 
@@ -90,7 +92,25 @@
         ns_map = {"xsi": Namespace.XSI.uri, "xsd": Namespace.XS.uri}
         value = ParserUtils.parse_any_attribute("xsd:string", ns_map)
         self.assertEqual("{http://www.w3.org/2001/XMLSchema}string", value)
 
         ns_map["http"] = "happens"
         value = ParserUtils.parse_any_attribute("http://www.com", ns_map)
         self.assertEqual("http://www.com", value)
+
+    def test_validate_fixed_value(self):
+        meta = XmlMetaFactory.create(clazz=TypeA, qname="foo")
+        var = XmlVarFactory.create("fixed", default="a")
+        with self.assertRaises(ParserError) as cm:
+            ParserUtils.validate_fixed_value(meta, var, "b")
+
+        self.assertEqual("Fixed value mismatch foo:fixed, `a != b`", str(cm.exception))
+
+        var = XmlVarFactory.create("fixed", default=lambda: "a")
+        with self.assertRaises(ParserError):
+            ParserUtils.validate_fixed_value(meta, var, "b")
+
+        var = XmlVarFactory.create("fixed", default=lambda: " a ")
+        ParserUtils.validate_fixed_value(meta, var, "  a  ")
+
+        var = XmlVarFactory.create("fixed", default=lambda: float("nan"))
+        ParserUtils.validate_fixed_value(meta, var, float("nan"))
```

### Comparing `xsdata-24.4/tests/formats/dataclass/parsers/test_xml.py` & `xsdata-24.5/tests/formats/dataclass/parsers/test_xml.py`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/tests/formats/dataclass/serializers/test_code.py` & `xsdata-24.5/tests/formats/dataclass/serializers/test_code.py`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/tests/formats/dataclass/serializers/test_config.py` & `xsdata-24.5/tests/formats/dataclass/serializers/test_config.py`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/tests/formats/dataclass/serializers/test_dict.py` & `xsdata-24.5/tests/formats/dataclass/serializers/test_dict.py`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/tests/formats/dataclass/serializers/test_json.py` & `xsdata-24.5/tests/formats/dataclass/serializers/test_json.py`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/tests/formats/dataclass/serializers/test_mixins.py` & `xsdata-24.5/tests/formats/dataclass/serializers/test_mixins.py`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/tests/formats/dataclass/serializers/test_xml.py` & `xsdata-24.5/tests/formats/dataclass/serializers/test_xml.py`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/tests/formats/dataclass/serializers/writers/test_lxml.py` & `xsdata-24.5/tests/formats/dataclass/serializers/writers/test_native.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,41 +1,35 @@
 from dataclasses import make_dataclass
 from unittest import TestCase
 
 from tests import fixtures_dir
 from tests.fixtures.books.fixtures import books
 from xsdata.formats.dataclass.serializers import XmlSerializer
 from xsdata.formats.dataclass.serializers.config import SerializerConfig
-from xsdata.formats.dataclass.serializers.writers import LxmlEventWriter
+from xsdata.formats.dataclass.serializers.writers import XmlEventWriter
 
 
-class LxmlEventWriterTests(TestCase):
+class XmlEventWriterTests(TestCase):
     def setUp(self):
         config = SerializerConfig(indent="  ")
-        self.serializer = XmlSerializer(config=config, writer=LxmlEventWriter)
+        self.serializer = XmlSerializer(config=config, writer=XmlEventWriter)
 
     def test_render(self):
         actual = self.serializer.render(books)
         expected = fixtures_dir.joinpath("books/books_auto_ns.xml").read_text()
-
         self.assertEqual(expected, actual)
 
     def test_render_with_provided_namespaces(self):
         actual = self.serializer.render(books, {"brk": "urn:books"})
         expected = fixtures_dir.joinpath("books/books.xml").read_text()
-
         self.assertEqual(expected, actual)
 
     def test_render_with_default_namespace_prefix(self):
         actual = self.serializer.render(books, {None: "urn:books"})
         expected = fixtures_dir.joinpath("books/books_default_ns.xml").read_text()
-
-        xml_declaration, actual = actual.split("\n", 1)
-        _, expected = expected.split("\n", 1)
-
         self.assertEqual(expected, actual)
 
     def test_encoding(self):
         self.serializer.config.encoding = "ISO-8859-1"
         x = make_dataclass("x", [("value", str)])
         obj = x("á, é, í, ó")
         actual = self.serializer.render(obj)
```

### Comparing `xsdata-24.4/tests/formats/dataclass/serializers/writers/test_native.py` & `xsdata-24.5/tests/formats/dataclass/serializers/writers/test_lxml.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,35 +1,45 @@
 from dataclasses import make_dataclass
 from unittest import TestCase
 
+import lxml
+
 from tests import fixtures_dir
 from tests.fixtures.books.fixtures import books
-from xsdata.formats.dataclass.serializers import XmlSerializer
+from xsdata.formats.dataclass.serializers import TreeSerializer, XmlSerializer
 from xsdata.formats.dataclass.serializers.config import SerializerConfig
-from xsdata.formats.dataclass.serializers.writers import XmlEventWriter
+from xsdata.formats.dataclass.serializers.writers import (
+    LxmlEventWriter,
+)
 
 
-class XmlEventWriterTests(TestCase):
+class LxmlEventWriterTests(TestCase):
     def setUp(self):
         config = SerializerConfig(indent="  ")
-        self.serializer = XmlSerializer(config=config, writer=XmlEventWriter)
+        self.serializer = XmlSerializer(config=config, writer=LxmlEventWriter)
 
     def test_render(self):
         actual = self.serializer.render(books)
         expected = fixtures_dir.joinpath("books/books_auto_ns.xml").read_text()
+
         self.assertEqual(expected, actual)
 
     def test_render_with_provided_namespaces(self):
         actual = self.serializer.render(books, {"brk": "urn:books"})
         expected = fixtures_dir.joinpath("books/books.xml").read_text()
+
         self.assertEqual(expected, actual)
 
     def test_render_with_default_namespace_prefix(self):
         actual = self.serializer.render(books, {None: "urn:books"})
         expected = fixtures_dir.joinpath("books/books_default_ns.xml").read_text()
+
+        xml_declaration, actual = actual.split("\n", 1)
+        _, expected = expected.split("\n", 1)
+
         self.assertEqual(expected, actual)
 
     def test_encoding(self):
         self.serializer.config.encoding = "ISO-8859-1"
         x = make_dataclass("x", [("value", str)])
         obj = x("á, é, í, ó")
         actual = self.serializer.render(obj)
@@ -48,7 +58,34 @@
         self.serializer.config.indent = None
         actual = self.serializer.render(books)
         expected = fixtures_dir.joinpath("books/books_auto_ns.xml").read_text()
 
         _, actual = actual.split("\n", 1)
         _, expected = expected.split("\n", 1)
         self.assertEqual(expected.replace("  ", "").replace("\n", ""), actual)
+
+
+class LxmlTreeBuilderTests(TestCase):
+    def setUp(self):
+        super().setUp()
+        self.serializer = TreeSerializer()
+        self.serializer.config.indent = "  "
+
+    def test_render(self):
+        tree = self.serializer.render(books)
+
+        actual = lxml.etree.tostring(tree).decode()
+
+        expected = fixtures_dir.joinpath("books/books_auto_ns.xml").read_text()
+        expected = "\n".join(expected.splitlines()[1:])
+        self.assertEqual(expected, actual)
+
+    def test_render_with_no_indent(self):
+        self.serializer.config.indent = ""
+        tree = self.serializer.render(books)
+
+        lxml.etree.indent(tree, "  ")
+        actual = lxml.etree.tostring(tree).decode()
+
+        expected = fixtures_dir.joinpath("books/books_auto_ns.xml").read_text()
+        expected = "\n".join(expected.splitlines()[1:])
+        self.assertEqual(expected, actual)
```

### Comparing `xsdata-24.4/tests/formats/dataclass/test_client.py` & `xsdata-24.5/tests/formats/dataclass/test_client.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from dataclasses import asdict, replace
 from unittest import TestCase, mock
 
 from tests.fixtures.calculator import (
     Add,
     CalculatorSoapAdd,
     CalculatorSoapAddInput,
     CalculatorSoapAddOutput,
@@ -39,15 +40,15 @@
 
         client = Client(config, serializer=XmlSerializer())
         self.assertIs(client.parser.context, client.serializer.context)
 
     def test_from_service(self):
         client = Client.from_service(CalculatorSoapAdd, location="http://testurl.com")
 
-        actual = client.config._asdict()
+        actual = asdict(client.config)
         expected = {
             "style": "document",
             "input": CalculatorSoapAddInput,
             "location": "http://testurl.com",
             "soap_action": "http://tempuri.org/Add",
             "output": CalculatorSoapAddOutput,
             "transport": "http://schemas.xmlsoap.org/soap/http",
@@ -134,15 +135,15 @@
         client = Client(config=config)
 
         headers = {"foo": "bar"}
         result = client.prepare_headers(headers)
         self.assertEqual({"content-type": "text/xml", "foo": "bar"}, result)
         self.assertEqual(1, len(headers))
 
-        config = config._replace(soap_action="add")
+        config = replace(config, soap_action="add")
         client = Client(config=config)
         result = client.prepare_headers({})
         self.assertEqual({"SOAPAction": "add", "content-type": "text/xml"}, result)
 
     def test_prepare_headers_raises_error_with_unsupported_binding_transport(self):
         config = Config.from_service(CalculatorSoapAdd, transport="foobar")
         client = Client(config=config)
```

### Comparing `xsdata-24.4/tests/formats/dataclass/test_compat.py` & `xsdata-24.5/tests/formats/dataclass/test_compat.py`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/tests/formats/dataclass/test_context.py` & `xsdata-24.5/tests/formats/dataclass/test_context.py`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/tests/formats/dataclass/test_elements.py` & `xsdata-24.5/tests/formats/dataclass/test_elements.py`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/tests/formats/dataclass/test_filters.py` & `xsdata-24.5/tests/formats/dataclass/test_filters.py`

 * *Files 5% similar despite different names*

```diff
@@ -35,14 +35,32 @@
 
 class FiltersTests(FactoryTestCase):
     def setUp(self) -> None:
         super().setUp()
         config = GeneratorConfig()
         self.filters = Filters(config)
 
+        obj = ClassFactory.create(qname="a")
+        obj_nested = ClassFactory.create(qname="b")
+        obj_nested_nested = ClassFactory.create(qname="c")
+        obj_nested_nested_nested = ClassFactory.create(qname="d")
+
+        obj_nested_nested_nested.parent = obj_nested_nested
+        obj_nested_nested.parent = obj_nested
+        obj_nested.parent = obj
+
+        obj.inner.append(obj_nested)
+        obj_nested.inner.append(obj_nested_nested)
+        obj_nested_nested.inner.append(obj_nested_nested_nested)
+
+        self.obj = obj
+        self.obj_nested = obj_nested
+        self.obj_nested_nested = obj_nested_nested
+        self.obj_nested_nested_nested = obj_nested_nested_nested
+
     def test_class_name(self):
         self.filters.substitutions[ObjectType.CLASS]["Abc"] = "Cba"
 
         self.assertEqual("XsString", self.filters.class_name("xs:string"))
         self.assertEqual("FooBarBam", self.filters.class_name("foo:bar_bam"))
         self.assertEqual("ListType", self.filters.class_name("List"))
         self.assertEqual("TypeType", self.filters.class_name(".*"))
@@ -227,27 +245,27 @@
         self.assertEqual("FooType", actual)
 
     @mock.patch.object(Filters, "field_default_value")
     def test_field_definition(self, mock_field_default_value):
         mock_field_default_value.side_effect = [1, False]
         attr = AttrFactory.native(DataType.INT)
 
-        result = self.filters.field_definition(attr, {}, None, ["Root"])
+        result = self.filters.field_definition(self.obj, attr, None)
         expected = (
             "field(\n"
             "        default=1,\n"
             "        metadata={\n"
             '            "name": "attr_B",\n'
             '            "type": "Element",\n'
             "        }\n"
             "    )"
         )
         self.assertEqual(expected, result)
 
-        result = self.filters.field_definition(attr, {}, None, ["Root"])
+        result = self.filters.field_definition(self.obj, attr, None)
         expected = (
             "field(\n"
             "        metadata={\n"
             '            "name": "attr_B",\n'
             '            "type": "Element",\n'
             "        }\n"
             "    )"
@@ -255,15 +273,15 @@
         self.assertEqual(expected, result)
 
     def test_field_definition_with_prohibited_attr(self):
         attr = AttrFactory.native(DataType.INT)
         attr.restrictions.max_occurs = 0
         attr.default = "1"
 
-        result = self.filters.field_definition(attr, {}, None, ["Root"])
+        result = self.filters.field_definition(self.obj, attr, None)
         expected = (
             "field(\n"
             "        init=False,\n"
             "        metadata={\n"
             '            "type": "Ignore",\n'
             "        }\n"
             "    )"
@@ -275,30 +293,30 @@
         mock_field_default_value.return_value = None
         str_attr = AttrFactory.create(types=[type_str], tag=Tag.RESTRICTION)
         # intentionally using a double-quote in the pattern to test for a regression in
         # https://github.com/tefra/xsdata/issues/592
         pattern = '([^\\ \\? > < \\* / " ": |]{1,256})'
         str_attr.restrictions.pattern = pattern
 
-        result = self.filters.field_definition(str_attr, {}, None, ["Root"])
+        result = self.filters.field_definition(self.obj, str_attr, None)
         expected = (
             "field(\n"
             "        default=None,\n"
             "        metadata={\n"
             '            "pattern": r"([^\\ \\? > < \\* / \\" \\": |]{1,256})",\n'
             "        }\n"
             "    )"
         )
         self.assertEqual(expected, result)
 
     @mock.patch.object(Filters, "field_metadata")
     def test_field_definition_without_metadata(self, mock_field_metadata):
         mock_field_metadata.return_value = {}
         str_attr = AttrFactory.create(types=[type_str], tag=Tag.RESTRICTION)
-        result = self.filters.field_definition(str_attr, {}, None, ["Root"])
+        result = self.filters.field_definition(self.obj, str_attr, None)
         expected = "field(\n" "        default=None\n" "    )"
         self.assertEqual(expected, result)
 
     def test_field_default_value_with_value_none(self):
         attr = AttrFactory.create(types=[type_str])
         self.assertEqual(None, self.filters.field_default_value(attr))
 
@@ -425,91 +443,90 @@
 
         attr.default = "true"
         self.assertEqual("True", self.filters.field_default_value(attr))
 
     def test_field_metadata(self):
         attr = AttrFactory.element()
         expected = {"name": "attr_B", "type": "Element"}
-        self.assertEqual(expected, self.filters.field_metadata(attr, None, ["cls"]))
-        self.assertEqual(expected, self.filters.field_metadata(attr, "foo", ["cls"]))
+        self.assertEqual(expected, self.filters.field_metadata(self.obj, attr, None))
 
     def test_field_metadata_namespace(self):
         attr = AttrFactory.element(namespace="foo")
         expected = {"name": "attr_B", "namespace": "foo", "type": "Element"}
 
-        actual = self.filters.field_metadata(attr, None, ["cls"])
+        actual = self.filters.field_metadata(self.obj, attr, None)
         self.assertEqual(expected, actual)
 
-        actual = self.filters.field_metadata(attr, "foo", ["cls"])
+        actual = self.filters.field_metadata(self.obj, attr, "foo")
         self.assertNotIn("namespace", actual)
 
         attr = AttrFactory.attribute(namespace="foo")
         expected = {"name": "attr_C", "namespace": "foo", "type": "Attribute"}
-        actual = self.filters.field_metadata(attr, None, ["cls"])
+        actual = self.filters.field_metadata(self.obj, attr, None)
         self.assertEqual(expected, actual)
 
-        actual = self.filters.field_metadata(attr, "foo", ["cls"])
+        actual = self.filters.field_metadata(self.obj, attr, "foo")
         self.assertIn("namespace", actual)
 
     def test_field_metadata_name(self):
         attr = AttrFactory.element(name="bar")
         attr.local_name = "foo"
 
-        actual = self.filters.field_metadata(attr, None, ["cls"])
+        actual = self.filters.field_metadata(self.obj, attr, None)
         self.assertEqual("foo", actual["name"])
 
         attr = AttrFactory.element(name="Foo")
         attr.local_name = "foo"
-        actual = self.filters.field_metadata(attr, None, ["cls"])
+        actual = self.filters.field_metadata(self.obj, attr, None)
         self.assertNotIn("name", actual)
 
         attr = AttrFactory.create(tag=Tag.ANY, name="bar")
         attr.local_name = "foo"
-        actual = self.filters.field_metadata(attr, None, ["cls"])
+        actual = self.filters.field_metadata(self.obj, attr, None)
         self.assertNotIn("name", actual)
 
     def test_field_metadata_wrapper(self):
         attr = AttrFactory.element(wrapper="foo")
         expected = {"name": "attr_B", "wrapper": "foo", "type": "Element"}
 
-        actual = self.filters.field_metadata(attr, None, ["cls"])
+        actual = self.filters.field_metadata(self.obj, attr, None)
         self.assertEqual(expected, actual)
 
     def test_field_metadata_restrictions(self):
         attr = AttrFactory.create(tag=Tag.RESTRICTION)
         attr.types.append(AttrTypeFactory.native(DataType.INT))
         attr.restrictions.min_occurs = 1
         attr.restrictions.max_occurs = 2
         attr.restrictions.max_inclusive = "2"
 
         expected = {"min_occurs": 1, "max_occurs": 2, "max_inclusive": 2}
-        self.assertEqual(expected, self.filters.field_metadata(attr, None, []))
+        self.assertEqual(expected, self.filters.field_metadata(self.obj, attr, None))
 
         attr.restrictions.min_occurs = 1
         attr.restrictions.max_occurs = 1
         expected = {"required": True, "max_inclusive": 2}
-        self.assertEqual(expected, self.filters.field_metadata(attr, None, []))
+        self.assertEqual(expected, self.filters.field_metadata(self.obj, attr, None))
 
         attr.restrictions.nillable = True
         expected = {"nillable": True, "max_inclusive": 2}
-        self.assertEqual(expected, self.filters.field_metadata(attr, None, []))
+        self.assertEqual(expected, self.filters.field_metadata(self.obj, attr, None))
 
         attr.default = None
         attr.restrictions.tokens = True
         expected = {"max_inclusive": 2, "nillable": True, "tokens": True}
-        self.assertEqual(expected, self.filters.field_metadata(attr, None, []))
+        self.assertEqual(expected, self.filters.field_metadata(self.obj, attr, None))
 
     def test_field_metadata_mixed(self):
         attr = AttrFactory.element(mixed=True)
         expected = {"mixed": True, "name": "attr_B", "type": "Element"}
-        self.assertEqual(expected, self.filters.field_metadata(attr, "foo", ["cls"]))
+        self.assertEqual(expected, self.filters.field_metadata(self.obj, attr, "foo"))
 
     def test_field_metadata_choices(self):
         attr = AttrFactory.create(choices=AttrFactory.list(2, tag=Tag.ELEMENT))
-        actual = self.filters.field_metadata(attr, "foo", ["cls"])
+        actual = self.filters.field_metadata(self.obj, attr, "foo")
         expected = (
             {"name": "attr_B", "type": "Type[str]"},
             {"name": "attr_C", "type": "Type[str]"},
         )
 
         self.assertEqual(expected, actual["choices"])
 
@@ -525,15 +542,15 @@
                 AttrFactory.element(namespace="bar"),
                 AttrFactory.any(namespace="##other"),
                 AttrFactory.element(name="bar", default="aa"),
                 AttrFactory.element(name="tok", restrictions=Restrictions(tokens=True)),
             ]
         )
 
-        actual = self.filters.field_choices(attr, "foo", ["a", "b"])
+        actual = self.filters.field_choices(self.obj, attr, "foo")
         expected = (
             {"name": "$", "type": "Type[float]", "max_exclusive": 10.0},
             {"name": "attr_B", "namespace": "bar", "type": "Type[str]"},
             {
                 "namespace": "##other",
                 "wildcard": True,
                 "type": "Type[object]",
@@ -547,196 +564,175 @@
             },
         )
 
         self.assertEqual(expected, actual)
 
         self.filters.docstring_style = DocstringStyle.ACCESSIBLE
         attr.choices[0].help = "help"
-        actual = self.filters.field_choices(attr, None, [])
+        actual = self.filters.field_choices(self.obj, attr, None)
         self.assertEqual(attr.choices[0].help, actual[0]["doc"])
         self.assertNotIn("doc", actual[1])
 
     def test_field_type_with_default_value(self):
         attr = AttrFactory.create(
             default="1", types=AttrTypeFactory.list(1, qname="foo_bar")
         )
 
-        self.assertEqual("FooBar", self.filters.field_type(attr, []))
+        self.assertEqual("FooBar", self.filters.field_type(self.obj, attr))
 
         attr.restrictions.nillable = True
-        self.assertEqual("Optional[FooBar]", self.filters.field_type(attr, []))
+        self.assertEqual("Optional[FooBar]", self.filters.field_type(self.obj, attr))
 
         self.filters.union_type = True
-        self.assertEqual("None | FooBar", self.filters.field_type(attr, []))
+        self.assertEqual("None | FooBar", self.filters.field_type(self.obj, attr))
 
     def test_field_type_with_optional_value(self):
         attr = AttrFactory.create(types=AttrTypeFactory.list(1, qname="foo_bar"))
 
-        self.assertEqual("Optional[FooBar]", self.filters.field_type(attr, []))
+        self.assertEqual("Optional[FooBar]", self.filters.field_type(self.obj, attr))
 
         self.filters.format.kw_only = True
-        self.assertEqual("FooBar", self.filters.field_type(attr, []))
+        self.assertEqual("FooBar", self.filters.field_type(self.obj, attr))
 
         attr.restrictions.min_occurs = 0
-        self.assertEqual("Optional[FooBar]", self.filters.field_type(attr, []))
+        self.assertEqual("Optional[FooBar]", self.filters.field_type(self.obj, attr))
 
         self.filters.union_type = True
-        self.assertEqual("None | FooBar", self.filters.field_type(attr, []))
+        self.assertEqual("None | FooBar", self.filters.field_type(self.obj, attr))
 
     def test_field_type_with_circular_reference(self):
         attr = AttrFactory.create(
-            types=AttrTypeFactory.list(1, qname="foo_bar", circular=True)
+            types=AttrTypeFactory.list(1, qname="c", circular=True)
         )
 
         self.assertEqual(
-            'Optional["FooBar"]', self.filters.field_type(attr, ["Parent"])
+            'Optional["C"]',
+            self.filters.field_type(self.obj_nested_nested_nested, attr),
         )
 
     def test_field_type_with_forward_reference(self):
         attr = AttrFactory.create(
-            types=AttrTypeFactory.list(1, qname="foo_bar", forward=True)
+            types=AttrTypeFactory.list(1, qname="b", forward=True)
         )
         self.assertEqual(
-            'Optional["Parent.Inner.FooBar"]',
-            self.filters.field_type(attr, ["Parent", "Inner"]),
+            'Optional["A.B"]',
+            self.filters.field_type(self.obj_nested_nested, attr),
         )
 
         self.filters.postponed_annotations = True
         self.filters.union_type = True
         self.assertEqual(
-            "None | Parent.Inner.FooBar",
-            self.filters.field_type(attr, ["Parent", "Inner"]),
-        )
-
-    def test_field_type_with_forward_and_circular_reference(self):
-        attr = AttrFactory.create(
-            types=AttrTypeFactory.list(1, qname="foo_bar", forward=True, circular=True)
-        )
-
-        self.assertEqual(
-            'Optional["Parent.Inner"]',
-            self.filters.field_type(attr, ["Parent", "Inner"]),
+            "None | A.B", self.filters.field_type(self.obj_nested_nested, attr)
         )
 
     def test_field_type_with_array_type(self):
         attr = AttrFactory.create(
-            types=AttrTypeFactory.list(1, qname="foo_bar", forward=True)
+            types=AttrTypeFactory.list(1, qname="c", forward=True)
         )
         attr.restrictions.max_occurs = 2
         self.assertEqual(
-            'List["A.Parent.FooBar"]',
-            self.filters.field_type(attr, ["A", "Parent"]),
+            'List["A.B.C"]',
+            self.filters.field_type(self.obj, attr),
         )
 
         self.filters.format.frozen = True
-        self.assertEqual(
-            'Tuple["A.Parent.FooBar", ...]',
-            self.filters.field_type(attr, ["A", "Parent"]),
-        )
+        self.assertEqual('Tuple["A.B.C", ...]', self.filters.field_type(self.obj, attr))
 
         self.filters.subscriptable_types = True
-        self.assertEqual(
-            'tuple["A.Parent.FooBar", ...]',
-            self.filters.field_type(attr, ["A", "Parent"]),
-        )
+        self.assertEqual('tuple["A.B.C", ...]', self.filters.field_type(self.obj, attr))
 
         self.filters.format.frozen = False
-        self.assertEqual(
-            'list["A.Parent.FooBar"]',
-            self.filters.field_type(attr, ["A", "Parent"]),
-        )
+        self.assertEqual('list["A.B.C"]', self.filters.field_type(self.obj, attr))
 
     def test_field_type_with_token_attr(self):
         attr = AttrFactory.create(
             types=AttrTypeFactory.list(1, qname="foo_bar"),
             restrictions=Restrictions(tokens=True),
         )
-        self.assertEqual("List[FooBar]", self.filters.field_type(attr, []))
+        self.assertEqual("List[FooBar]", self.filters.field_type(self.obj, attr))
 
         attr.restrictions.max_occurs = 2
-        self.assertEqual("List[List[FooBar]]", self.filters.field_type(attr, []))
+        self.assertEqual("List[List[FooBar]]", self.filters.field_type(self.obj, attr))
 
         attr.restrictions.max_occurs = 1
         self.filters.format.frozen = True
-        self.assertEqual("Tuple[FooBar, ...]", self.filters.field_type(attr, []))
+        self.assertEqual("Tuple[FooBar, ...]", self.filters.field_type(self.obj, attr))
 
         attr.restrictions.max_occurs = 2
         self.assertEqual(
-            "Tuple[Tuple[FooBar, ...], ...]", self.filters.field_type(attr, [])
+            "Tuple[Tuple[FooBar, ...], ...]", self.filters.field_type(self.obj, attr)
         )
 
         self.filters.subscriptable_types = True
         self.assertEqual(
-            "tuple[tuple[FooBar, ...], ...]", self.filters.field_type(attr, [])
+            "tuple[tuple[FooBar, ...], ...]", self.filters.field_type(self.obj, attr)
         )
 
     def test_field_type_with_alias(self):
         attr = AttrFactory.create(
-            types=AttrTypeFactory.list(
-                1, qname="foo_bar", forward=True, alias="Boss:Life"
-            )
+            types=AttrTypeFactory.list(1, qname="b", forward=True, alias="Boss:Life")
         )
         attr.restrictions.max_occurs = 2
         self.assertEqual(
-            'List["A.Parent.BossLife"]',
-            self.filters.field_type(attr, ["A", "Parent"]),
+            'List["A.BossLife"]',
+            self.filters.field_type(self.obj_nested_nested_nested, attr),
         )
 
     def test_field_type_with_multiple_types(self):
         attr = AttrFactory.create(
             types=[
-                AttrTypeFactory.create(qname="life", alias="Boss:Life", forward=True),
+                AttrTypeFactory.create(qname="c", alias="Boss:Life", forward=True),
                 AttrTypeFactory.native(DataType.INT),
             ]
         )
         attr.restrictions.max_occurs = 2
 
         self.assertEqual(
-            'List[Union["A.Parent.BossLife", int]]',
-            self.filters.field_type(attr, ["A", "Parent"]),
+            'List[Union["A.B.BossLife", int]]',
+            self.filters.field_type(self.obj_nested_nested_nested, attr),
         )
 
         self.filters.union_type = True
         self.assertEqual(
-            'List["A.Parent.BossLife" | int]',
-            self.filters.field_type(attr, ["A", "Parent"]),
+            'List["A.B.BossLife" | int]',
+            self.filters.field_type(self.obj_nested_nested_nested, attr),
         )
         self.filters.subscriptable_types = True
         self.assertEqual(
-            'list["A.Parent.BossLife" | int]',
-            self.filters.field_type(attr, ["A", "Parent"]),
+            'list["A.B.BossLife" | int]',
+            self.filters.field_type(self.obj_nested_nested_nested, attr),
         )
 
     def test_field_type_with_any_attribute(self):
         attr = AttrFactory.any_attribute()
 
-        self.assertEqual("Dict[str, str]", self.filters.field_type(attr, ["a", "b"]))
+        self.assertEqual("Dict[str, str]", self.filters.field_type(self.obj, attr))
 
         self.filters.subscriptable_types = True
-        self.assertEqual("dict[str, str]", self.filters.field_type(attr, ["a", "b"]))
+        self.assertEqual("dict[str, str]", self.filters.field_type(self.obj, attr))
 
     def test_field_type_with_native_type(self):
         attr = AttrFactory.create(
             types=[
                 AttrTypeFactory.native(DataType.INT),
                 AttrTypeFactory.native(DataType.POSITIVE_INTEGER),
                 AttrTypeFactory.native(DataType.STRING),
             ]
         )
         self.assertEqual(
-            "Optional[Union[int, str]]", self.filters.field_type(attr, ["a", "b"])
+            "Optional[Union[int, str]]", self.filters.field_type(self.obj, attr)
         )
 
         self.filters.union_type = True
-        self.assertEqual("None | int | str", self.filters.field_type(attr, ["a", "b"]))
+        self.assertEqual("None | int | str", self.filters.field_type(self.obj, attr))
 
     def test_field_type_with_prohibited_attr(self):
         attr = AttrFactory.create(restrictions=Restrictions(max_occurs=0))
 
-        self.assertEqual("Any", self.filters.field_type(attr, ["a", "b"]))
+        self.assertEqual("Any", self.filters.field_type(self.obj, attr))
 
     def test_field_type_with_compound_attr(self):
         attr = AttrFactory.create(
             tag=Tag.CHOICE,
             choices=[
                 AttrFactory.create(
                     name="a", types=[AttrTypeFactory.native(DataType.STRING)]
@@ -750,85 +746,84 @@
                     restrictions=Restrictions(tokens=True),
                 ),
             ],
             restrictions=Restrictions(min_occurs=0, max_occurs=1),
         )
 
         expected = "Optional[Union[str, int, List[Decimal]]]"
-        self.assertEqual(expected, self.filters.field_type(attr, []))
+        self.assertEqual(expected, self.filters.field_type(self.obj, attr))
 
         attr.restrictions.max_occurs = 2
         expected = "List[Union[str, int, List[Decimal]]]"
-        self.assertEqual(expected, self.filters.field_type(attr, []))
+        self.assertEqual(expected, self.filters.field_type(self.obj, attr))
 
         attr.restrictions.min_occurs = attr.restrictions.max_occurs = 1
         self.filters.format.kw_only = True
         expected = "Union[str, int, List[Decimal]]"
-        self.assertEqual(expected, self.filters.field_type(attr, []))
+        self.assertEqual(expected, self.filters.field_type(self.obj, attr))
 
     def test_choice_type(self):
         choice = AttrFactory.create(types=[AttrTypeFactory.create("foobar")])
-        actual = self.filters.choice_type(choice, ["a", "b"])
+        target = ClassFactory.create()
+        actual = self.filters.choice_type(target, choice)
         self.assertEqual("Type[Foobar]", actual)
 
-        self.filters.subscriptable_types = True
-        actual = self.filters.choice_type(choice, ["a", "b"])
-        self.assertEqual("type[Foobar]", actual)
-
     def test_choice_type_with_forward_reference(self):
         choice = AttrFactory.create(
             types=[AttrTypeFactory.create("foobar", forward=True)]
         )
-        actual = self.filters.choice_type(choice, ["a", "b"])
-        self.assertEqual('Type["A.B.Foobar"]', actual)
+        target = ClassFactory.create(qname="foobar")
+        parent = ClassFactory.create(qname="a")
+        parent.inner.append(target)
+        target.parent = parent
+
+        actual = self.filters.choice_type(parent, choice)
+        self.assertEqual('ForwardRef("A.Foobar")', actual)
 
     def test_choice_type_with_circular_reference(self):
-        choice = AttrFactory.create(
-            types=[AttrTypeFactory.create("foobar", circular=True)]
-        )
-        actual = self.filters.choice_type(choice, ["a", "b"])
-        self.assertEqual('Type["Foobar"]', actual)
+        choice = AttrFactory.create(types=[AttrTypeFactory.create("c", circular=True)])
+        actual = self.filters.choice_type(self.obj_nested_nested_nested, choice)
+        self.assertEqual('ForwardRef("C")', actual)
 
         self.filters.postponed_annotations = True
-        actual = self.filters.choice_type(choice, ["a", "b"])
-        self.assertEqual('Type["Foobar"]', actual)
+        actual = self.filters.choice_type(self.obj_nested_nested_nested, choice)
+        self.assertEqual('ForwardRef("C")', actual)
 
     def test_choice_type_with_multiple_types(self):
         choice = AttrFactory.create(types=[type_str, type_bool])
-        actual = self.filters.choice_type(choice, ["a", "b"])
+        target = ClassFactory.create()
+        actual = self.filters.choice_type(target, choice)
         self.assertEqual("Type[Union[str, bool]]", actual)
 
-        self.filters.subscriptable_types = True
-        actual = self.filters.choice_type(choice, ["a", "b"])
-        self.assertEqual("type[Union[str, bool]]", actual)
-
         self.filters.union_type = True
-        actual = self.filters.choice_type(choice, ["a", "b"])
-        self.assertEqual("type[str | bool]", actual)
+        actual = self.filters.choice_type(target, choice)
+        self.assertEqual("Type[str | bool]", actual)
 
     def test_choice_type_with_list_types_are_ignored(self):
         choice = AttrFactory.create(types=[type_str, type_bool])
         choice.restrictions.max_occurs = 200
-        actual = self.filters.choice_type(choice, ["a", "b"])
+        target = ClassFactory.create()
+        actual = self.filters.choice_type(target, choice)
         self.assertEqual("Type[Union[str, bool]]", actual)
 
     def test_choice_type_with_restrictions_tokens_true(self):
         choice = AttrFactory.create(types=[type_str, type_bool])
         choice.restrictions.tokens = True
-        actual = self.filters.choice_type(choice, ["a", "b"])
+        target = ClassFactory.create()
+        actual = self.filters.choice_type(target, choice)
         self.assertEqual("Type[List[Union[str, bool]]]", actual)
 
         self.filters.format.frozen = True
-        actual = self.filters.choice_type(choice, ["a", "b"])
+        actual = self.filters.choice_type(target, choice)
         self.assertEqual("Type[Tuple[Union[str, bool], ...]]", actual)
 
         self.filters.union_type = True
         self.filters.subscriptable_types = True
-        actual = self.filters.choice_type(choice, ["a", "b"])
-        self.assertEqual("type[tuple[str | bool, ...]]", actual)
+        actual = self.filters.choice_type(target, choice)
+        self.assertEqual("Type[tuple[str | bool, ...]]", actual)
 
     def test_default_imports_with_decimal(self):
         expected = "from decimal import Decimal"
 
         self.assertIn(expected, self.filters.default_imports("Optional[Decimal]"))
         self.assertIn(expected, self.filters.default_imports("Union[str, Decimal]"))
         self.assertIn(expected, self.filters.default_imports("Union[Decimal, "))
@@ -896,16 +891,16 @@
         expected = "from typing import Optional"
         self.assertIn(expected, self.filters.default_imports(output))
 
         output = " Union[ "
         expected = "from typing import Union"
         self.assertIn(expected, self.filters.default_imports(output))
 
-        output = " Type["
-        expected = "from typing import Type"
+        output = ": ForwardRef("
+        expected = "from typing import ForwardRef"
         self.assertIn(expected, self.filters.default_imports(output))
 
         output = ": Any = "
         expected = "from typing import Any"
         self.assertIn(expected, self.filters.default_imports(output))
 
     def test_default_imports_combo(self):
@@ -942,16 +937,15 @@
             "text_two": "fo'o",
             "text_three": 'fo"o',
             "pattern": "foo",
             "custom": Telephone(30, 123, 4567),
             "level_two": {"a": 1},
             "list": [
                 {"type": "Type[object]"},
-                {"type": 'type["something"]'},
-                {"type": "Type[object] mpla"},
+                {"type": 'ForwardRef("something")'},
             ],
             "default": "1",
             "default_factory": "list",
         }
 
         expected = (
             "{\n"
@@ -965,18 +959,15 @@
             '        "a": 1,\n'
             "    },\n"
             '    "list": [\n'
             "        {\n"
             '            "type": object,\n'
             "        },\n"
             "        {\n"
-            '            "type": type["something"],\n'
-            "        },\n"
-            "        {\n"
-            '            "type": "Type[object] mpla",\n'
+            '            "type": ForwardRef("something"),\n'
             "        },\n"
             "    ],\n"
             '    "default": 1,\n'
             '    "default_factory": list,\n'
             "}"
         )
         self.assertEqual(expected, self.filters.format_metadata(data))
```

### Comparing `xsdata-24.4/tests/formats/dataclass/test_generator.py` & `xsdata-24.5/tests/formats/dataclass/test_generator.py`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/tests/formats/dataclass/test_transport.py` & `xsdata-24.5/tests/formats/dataclass/test_transport.py`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/tests/formats/test_converter.py` & `xsdata-24.5/tests/formats/test_converter.py`

 * *Files 6% similar despite different names*

```diff
@@ -49,14 +49,26 @@
         self.assertFalse(converter.test("a", [int]))
         self.assertTrue(converter.test("01", [int]))
         self.assertFalse(converter.test("01", [int], strict=True))
         self.assertTrue(converter.test("1", [int]))
 
         self.assertTrue(converter.test("0", [float]))
         self.assertFalse(converter.test("0", [float], strict=True))
+
+        self.assertTrue(converter.test("INF", [float], strict=True))
+        self.assertTrue(converter.test("inf", [float], strict=True))
+        self.assertTrue(converter.test("+INF", [float], strict=True))
+        self.assertTrue(converter.test("+inf", [float], strict=True))
+        self.assertTrue(converter.test("-INF", [float], strict=True))
+        self.assertTrue(converter.test("-inf", [float], strict=True))
+        self.assertTrue(converter.test("NAN", [float], strict=True))
+        self.assertTrue(converter.test("NaN", [float], strict=True))
+        self.assertTrue(converter.test("nan", [float], strict=True))
+        self.assertTrue(converter.test("-NAN", [float], strict=True))
+
         self.assertTrue(converter.test(".0", [float]))
         self.assertFalse(converter.test(".0", [float], strict=True))
         self.assertTrue(converter.test("1.0", [float]))
 
     def test_unknown_converter(self):
         class A:
             pass
```

### Comparing `xsdata-24.4/tests/formats/test_mixins.py` & `xsdata-24.5/tests/formats/test_mixins.py`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/tests/integration/benchmarks/test_converters.py` & `xsdata-24.5/tests/integration/benchmarks/test_converters.py`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/tests/integration/benchmarks/test_handlers.py` & `xsdata-24.5/tests/integration/benchmarks/test_handlers.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,38 +1,41 @@
 import random
 
 import pytest
 
 from tests import xsdata_temp_dir
 from tests.integration.benchmarks.utils import make_books, parse, write
 from xsdata.formats.dataclass.context import XmlContext
-from xsdata.formats.dataclass.parsers import handlers as readers
-from xsdata.formats.dataclass.serializers import writers
+from xsdata.formats.dataclass.parsers.handlers import LxmlEventHandler, XmlEventHandler
+from xsdata.formats.dataclass.serializers.writers import LxmlEventWriter, XmlEventWriter
 
 context = XmlContext()
-readers_list = list(readers.__all__)
-writers_list = list(writers.__all__)
-
-readers_list.remove("default_handler")
-writers_list.remove("default_writer")
+readers_list = [
+    LxmlEventHandler,
+    XmlEventHandler,
+]
+writers_list = [
+    XmlEventWriter,
+    LxmlEventWriter,
+]
 
 random.shuffle(readers_list)
 random.shuffle(writers_list)
 
 numbers = [100, 1000, 10000]
 
 fixtures = {number: make_books(number) for number in numbers}
 
 
 @pytest.mark.benchmark(disable_gc=True, group="Serialize")
 @pytest.mark.parametrize("number", numbers)
 @pytest.mark.parametrize("writer", writers_list)
 def test_serialize(benchmark, writer, number):
-    benchmark(write, number, fixtures[number], getattr(writers, writer))
+    benchmark(write, number, fixtures[number], writer)
 
 
 @pytest.mark.benchmark(disable_gc=True, group="Parse")
 @pytest.mark.parametrize("number", numbers)
 @pytest.mark.parametrize("handler", readers_list)
 def test_parse(benchmark, handler, number):
     src = xsdata_temp_dir.joinpath(f"benchmark_{number}.xml").read_bytes()
-    benchmark(parse, src, getattr(readers, handler))
+    benchmark(parse, src, handler)
```

### Comparing `xsdata-24.4/tests/integration/benchmarks/utils.py` & `xsdata-24.5/tests/integration/benchmarks/utils.py`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/tests/integration/test_annotations.py` & `xsdata-24.5/tests/integration/test_annotations.py`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/tests/integration/test_artists.py` & `xsdata-24.5/tests/integration/test_artists.py`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/tests/integration/test_books.py` & `xsdata-24.5/tests/integration/test_books.py`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/tests/integration/test_calculator.py` & `xsdata-24.5/tests/integration/test_calculator.py`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/tests/integration/test_compound.py` & `xsdata-24.5/tests/integration/test_compound.py`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/tests/integration/test_docstrings.py` & `xsdata-24.5/tests/integration/test_docstrings.py`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/tests/integration/test_dtd.py` & `xsdata-24.5/tests/integration/test_dtd.py`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/tests/integration/test_hello_rpc.py` & `xsdata-24.5/tests/integration/test_hello_rpc.py`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/tests/integration/test_primer.py` & `xsdata-24.5/tests/integration/test_primer.py`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/tests/integration/test_series.py` & `xsdata-24.5/tests/integration/test_series.py`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/tests/integration/test_stripe.py` & `xsdata-24.5/tests/integration/test_stripe.py`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/tests/integration/test_type_mapping.py` & `xsdata-24.5/tests/integration/test_type_mapping.py`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/tests/integration/test_wrapper.py` & `xsdata-24.5/tests/integration/test_wrapper.py`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/tests/models/enums/test_datatype.py` & `xsdata-24.5/tests/models/enums/test_datatype.py`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/tests/models/test_config.py` & `xsdata-24.5/tests/models/test_config.py`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/tests/models/test_datatype.py` & `xsdata-24.5/tests/models/test_datatype.py`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/tests/models/test_mixins.py` & `xsdata-24.5/tests/models/test_mixins.py`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/tests/models/wsdl/test_binding.py` & `xsdata-24.5/tests/models/wsdl/test_binding.py`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/tests/models/wsdl/test_definitions.py` & `xsdata-24.5/tests/models/wsdl/test_definitions.py`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/tests/models/xsd/test_all.py` & `xsdata-24.5/tests/models/xsd/test_all.py`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/tests/models/xsd/test_alternative.py` & `xsdata-24.5/tests/models/xsd/test_alternative.py`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/tests/models/xsd/test_annotation_base.py` & `xsdata-24.5/tests/models/xsd/test_annotation_base.py`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/tests/models/xsd/test_any.py` & `xsdata-24.5/tests/models/xsd/test_any.py`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/tests/models/xsd/test_any_attribute.py` & `xsdata-24.5/tests/models/xsd/test_any_attribute.py`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/tests/models/xsd/test_attribute.py` & `xsdata-24.5/tests/models/xsd/test_attribute.py`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/tests/models/xsd/test_choice.py` & `xsdata-24.5/tests/models/xsd/test_choice.py`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/tests/models/xsd/test_element.py` & `xsdata-24.5/tests/models/xsd/test_element.py`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/tests/models/xsd/test_enumeration.py` & `xsdata-24.5/tests/models/xsd/test_enumeration.py`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/tests/models/xsd/test_group.py` & `xsdata-24.5/tests/models/xsd/test_group.py`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/tests/models/xsd/test_list.py` & `xsdata-24.5/tests/models/xsd/test_list.py`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/tests/models/xsd/test_restriction.py` & `xsdata-24.5/tests/models/xsd/test_restriction.py`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/tests/models/xsd/test_schema.py` & `xsdata-24.5/tests/models/xsd/test_schema.py`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/tests/models/xsd/test_sequence.py` & `xsdata-24.5/tests/models/xsd/test_sequence.py`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/tests/models/xsd/test_simple_type.py` & `xsdata-24.5/tests/models/xsd/test_simple_type.py`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/tests/models/xsd/test_union.py` & `xsdata-24.5/tests/models/xsd/test_union.py`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/tests/test_cli.py` & `xsdata-24.5/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/tests/utils/test_collections.py` & `xsdata-24.5/tests/utils/test_collections.py`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/tests/utils/test_dates.py` & `xsdata-24.5/tests/utils/test_dates.py`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/tests/utils/test_downloader.py` & `xsdata-24.5/tests/utils/test_downloader.py`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/tests/utils/test_hooks.py` & `xsdata-24.5/tests/utils/test_hooks.py`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/tests/utils/test_namespaces.py` & `xsdata-24.5/tests/utils/test_namespaces.py`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/tests/utils/test_text.py` & `xsdata-24.5/tests/utils/test_text.py`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/xsdata/cli.py` & `xsdata-24.5/xsdata/cli.py`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/xsdata/codegen/container.py` & `xsdata-24.5/xsdata/codegen/container.py`

 * *Files 1% similar despite different names*

```diff
@@ -144,15 +144,15 @@
 
         Returns:
             The inner class instance
 
         Raises:
             CodeGenerationError: If the inner class is not found.
         """
-        inner = ClassUtils.find_inner(source, qname)
+        inner = ClassUtils.find_nested(source, qname)
         if inner.status < self.step:
             self.process_class(inner, self.step)
 
         return inner
 
     def first(self, qname: str) -> Class:
         """Return the first class that matches the qualified name.
```

### Comparing `xsdata-24.4/xsdata/codegen/exceptions.py` & `xsdata-24.5/xsdata/codegen/exceptions.py`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/xsdata/codegen/handlers/__init__.py` & `xsdata-24.5/xsdata/codegen/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/xsdata/codegen/handlers/add_attribute_substitutions.py` & `xsdata-24.5/xsdata/codegen/handlers/add_attribute_substitutions.py`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/xsdata/codegen/handlers/calculate_attribute_paths.py` & `xsdata-24.5/xsdata/codegen/handlers/calculate_attribute_paths.py`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/xsdata/codegen/handlers/create_compound_fields.py` & `xsdata-24.5/xsdata/codegen/handlers/create_compound_fields.py`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/xsdata/codegen/handlers/create_wrapper_fields.py` & `xsdata-24.5/xsdata/codegen/handlers/create_wrapper_fields.py`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/xsdata/codegen/handlers/designate_class_packages.py` & `xsdata-24.5/xsdata/codegen/handlers/designate_class_packages.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from urllib.parse import urlparse
 
 from toposort import toposort_flatten
 
 from xsdata.codegen.exceptions import CodegenError
 from xsdata.codegen.mixins import ContainerHandlerInterface
 from xsdata.codegen.models import Class, get_location, get_target_namespace
+from xsdata.logger import logger
 from xsdata.models.config import ObjectType, StructureStyle
 from xsdata.models.enums import COMMON_SCHEMA_DIR
 from xsdata.utils import collections
 from xsdata.utils.graphs import strongly_connected_components
 from xsdata.utils.namespaces import to_package_name
 from xsdata.utils.package import module_name
 
@@ -53,27 +54,39 @@
 
         Example:
             http://xsdata/foo/bar/schema.xsd -> foo.bar.schema.py
         """
         package = self.container.config.output.package
         class_map = collections.group_by(self.container, key=get_location)
         groups = self.group_common_paths(class_map.keys())
+        modules_map = defaultdict(list)
 
         for keys in groups:
             if len(keys) == 1:
                 common_path = os.path.dirname(keys[0])
             else:
                 common_path = os.path.commonpath(keys)
 
             for key in keys:
                 items = class_map[key]
                 suffix = ".".join(Path(key).parent.relative_to(common_path).parts)
-
                 package_name = f"{package}.{suffix}" if suffix else package
-                self.assign(items, package_name, module_name(key))
+                mod_name = module_name(key)
+                modules_map[(package_name, mod_name)].append(key)
+
+                self.assign(items, package_name, mod_name)
+
+        for locations in modules_map.values():
+            if len(locations) > 1:
+                logger.warning(
+                    "Classes from different locations are designated to same module.\n"
+                    "You can resolve this if you switch to another `--structure-style`."
+                    "\n%s",
+                    "\n".join(locations),
+                )
 
     def group_by_namespace(self):
         """Group classes by their target namespace.
 
         Example:
             {myNS.tempuri.org}Root -> org.tempuri.myNS.py
         """
```

### Comparing `xsdata-24.4/xsdata/codegen/handlers/detect_circular_references.py` & `xsdata-24.5/xsdata/codegen/handlers/detect_circular_references.py`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/xsdata/codegen/handlers/disambiguate_choices.py` & `xsdata-24.5/xsdata/codegen/handlers/disambiguate_choices.py`

 * *Files 0% similar despite different names*

```diff
@@ -167,14 +167,15 @@
             forward=inner,
             circular=is_circular,
         )
         choice.types = [ref_type]
         if not inner:
             self.container.add(ref_class)
         else:
+            ref_class.parent = target
             target.inner.append(ref_class)
 
     def is_simple_type(self, choice: Attr) -> bool:
         """Return whether the choice attr is a simple type reference."""
         if any(tp.native for tp in choice.types):
             return True
```

### Comparing `xsdata-24.4/xsdata/codegen/handlers/filter_classes.py` & `xsdata-24.5/xsdata/codegen/handlers/filter_classes.py`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/xsdata/codegen/handlers/flatten_attribute_groups.py` & `xsdata-24.5/xsdata/codegen/handlers/flatten_attribute_groups.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from xsdata.codegen.exceptions import CodegenError
 from xsdata.codegen.mixins import RelativeHandlerInterface
-from xsdata.codegen.models import Attr, Class
+from xsdata.codegen.models import Attr, Class, Status
 from xsdata.codegen.utils import ClassUtils
 
 
 class FlattenAttributeGroups(RelativeHandlerInterface):
     """Replace groups and attGroups with the source class attributes."""
 
     __slots__ = ()
@@ -47,8 +47,9 @@
 
         if not source:
             raise CodegenError("Unknown group reference", tag=attr.tag, qname=qname)
 
         if source is target:
             ClassUtils.remove_attribute(target, attr)
         else:
-            ClassUtils.copy_group_attributes(source, target, attr)
+            is_circular_ref = source.status == Status.UNGROUPING
+            ClassUtils.copy_group_attributes(source, target, attr, is_circular_ref)
```

### Comparing `xsdata-24.4/xsdata/codegen/handlers/flatten_class_extensions.py` & `xsdata-24.5/xsdata/codegen/handlers/flatten_class_extensions.py`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/xsdata/codegen/handlers/merge_attributes.py` & `xsdata-24.5/xsdata/codegen/handlers/merge_attributes.py`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/xsdata/codegen/handlers/process_attributes_types.py` & `xsdata-24.5/xsdata/codegen/handlers/process_attributes_types.py`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/xsdata/codegen/handlers/process_mixed_content_class.py` & `xsdata-24.5/xsdata/codegen/handlers/process_mixed_content_class.py`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/xsdata/codegen/handlers/rename_duplicate_classes.py` & `xsdata-24.5/xsdata/codegen/handlers/rename_duplicate_classes.py`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/xsdata/codegen/handlers/reset_attribute_sequence_numbers.py` & `xsdata-24.5/xsdata/codegen/handlers/reset_attribute_sequence_numbers.py`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/xsdata/codegen/handlers/reset_attribute_sequences.py` & `xsdata-24.5/xsdata/codegen/handlers/reset_attribute_sequences.py`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/xsdata/codegen/handlers/sanitize_attributes_default_value.py` & `xsdata-24.5/xsdata/codegen/handlers/sanitize_attributes_default_value.py`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/xsdata/codegen/handlers/sanitize_enumeration_class.py` & `xsdata-24.5/xsdata/codegen/handlers/sanitize_enumeration_class.py`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/xsdata/codegen/handlers/unnest_inner_classes.py` & `xsdata-24.5/xsdata/codegen/handlers/unnest_inner_classes.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,14 +56,15 @@
             inner: The inner class to clone and prepare
             name: The parent class name to use a prefix
 
         Returns:
             The new class instance
         """
         clone = inner.clone()
+        clone.parent = None
         clone.local_type = True
         clone.qname = build_qname(inner.target_namespace, f"{name}_{inner.name}")
 
         for attr in clone.attrs:
             for tp in attr.types:
                 if tp.circular and tp.qname == inner.qname:
                     tp.qname = clone.qname
```

### Comparing `xsdata-24.4/xsdata/codegen/handlers/update_attributes_effective_choice.py` & `xsdata-24.5/xsdata/codegen/handlers/update_attributes_effective_choice.py`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/xsdata/codegen/handlers/vacuum_inner_classes.py` & `xsdata-24.5/xsdata/codegen/handlers/vacuum_inner_classes.py`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/xsdata/codegen/handlers/validate_attributes_overrides.py` & `xsdata-24.5/xsdata/codegen/handlers/validate_attributes_overrides.py`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/xsdata/codegen/mappers/definitions.py` & `xsdata-24.5/xsdata/codegen/mappers/definitions.py`

 * *Files 1% similar despite different names*

```diff
@@ -372,14 +372,15 @@
                 qname=namespaces.build_qname(target.target_namespace, name),
                 tag=Tag.BINDING_MESSAGE,
                 location=target.location,
                 ns_map=target.ns_map.copy(),
             )
             attr = cls.build_attr(name, inner.qname, forward=True, namespace=namespace)
 
+            inner.parent = target
             target.inner.append(inner)
             target.attrs.append(attr)
 
         return inner
 
     @classmethod
     def map_port_type_message(
```

### Comparing `xsdata-24.4/xsdata/codegen/mappers/dict.py` & `xsdata-24.5/xsdata/codegen/mappers/dict.py`

 * *Files 4% similar despite different names*

```diff
@@ -62,13 +62,14 @@
             else:
                 for val in value:
                     cls.build_class_attribute(target, name, val)
                     target.attrs[-1].restrictions.max_occurs = sys.maxsize
         else:
             if isinstance(value, dict):
                 inner = cls.build_class(value, name)
+                inner.parent = target
                 attr_type = AttrType(qname=inner.qname, forward=True)
                 target.inner.append(inner)
             else:
                 attr_type = cls.build_attr_type(name, value)
 
-            cls.build_attr(target, name, attr_type)
+            cls.build_attr(target, name, attr_type, value=value)
```

### Comparing `xsdata-24.4/xsdata/codegen/mappers/dtd.py` & `xsdata-24.5/xsdata/codegen/mappers/dtd.py`

 * *Files 0% similar despite different names*

```diff
@@ -323,9 +323,9 @@
                     fixed=True,
                     default=value,
                     name=value,
                     tag=Tag.ENUMERATION,
                     types=[attr_type.clone()],
                 )
             )
-
+        inner.parent = target
         target.inner.append(inner)
```

### Comparing `xsdata-24.4/xsdata/codegen/mappers/element.py` & `xsdata-24.5/xsdata/codegen/mappers/element.py`

 * *Files 1% similar despite different names*

```diff
@@ -102,14 +102,15 @@
         for index, child in enumerate(element.children):
             if isinstance(child, AnyElement) and child.qname:
                 if child.tail:
                     target.mixed = True
 
                 if child.attributes or child.children:
                     inner = cls.build_class(child, namespace)
+                    inner.parent = target
                     attr_type = AttrType(qname=inner.qname, forward=True)
                     target.inner.append(inner)
                 else:
                     attr_type = cls.build_attr_type(child.qname, child.text)
 
                 sequence = collections.find_connected_component(sequences, index)
                 cls.build_attr(
```

### Comparing `xsdata-24.4/xsdata/codegen/mappers/mixins.py` & `xsdata-24.5/xsdata/codegen/mappers/mixins.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,50 +3,58 @@
 
 from xsdata.codegen.models import Attr, AttrType, Class
 from xsdata.formats.converter import converter
 from xsdata.models.enums import DataType, QNames, Tag
 from xsdata.utils import collections
 from xsdata.utils.namespaces import split_qname
 
+_UNSET = object()
+
 
 class RawDocumentMapper:
     """Mixin class for raw json/xml documents."""
 
     @classmethod
     def build_attr(
         cls,
         target: Class,
         qname: str,
         attr_type: AttrType,
         parent_namespace: Optional[str] = None,
         tag: str = Tag.ELEMENT,
         sequence: int = 0,
+        value: Any = _UNSET,
     ):
         """Build an attr for the given class instance.
 
         Args:
             target: The target class instance
             qname: The attr qualified name
             attr_type: The attr type instance
             parent_namespace: The parent namespace
             tag: The attr tag
             sequence: The attr sequence number
+            value: The attr sample value
         """
         namespace, name = split_qname(qname)
         namespace = cls.select_namespace(namespace, parent_namespace, tag)
         index = len(target.attrs)
 
         attr = Attr(index=index, name=name, tag=tag, namespace=namespace)
         attr.types.append(attr_type)
 
         if sequence:
             attr.restrictions.path.append(("s", sequence, 1, sys.maxsize))
 
         attr.restrictions.min_occurs = 1
         attr.restrictions.max_occurs = 1
+
+        if value is None:
+            attr.restrictions.min_occurs = 0
+
         cls.add_attribute(target, attr)
 
     @classmethod
     def build_attr_type(cls, qname: str, value: Any) -> AttrType:
         """Build an attribute type for the given attribute name and value.
 
         Args:
```

### Comparing `xsdata-24.4/xsdata/codegen/mappers/schema.py` & `xsdata-24.5/xsdata/codegen/mappers/schema.py`

 * *Files 0% similar despite different names*

```diff
@@ -356,14 +356,15 @@
             A list of attr type instances.
         """
         types = [cls.build_attr_type(target, tp) for tp in obj.attr_types]
 
         location = target.location
         namespace = target.target_namespace
         for inner in cls.build_inner_classes(obj, location, namespace):
+            inner.parent = target
             target.inner.append(inner)
             types.append(AttrType(qname=inner.qname, forward=True))
 
         if len(types) == 0:
             types.append(cls.build_attr_type(target, name=obj.default_type))
 
         return collections.unique_sequence(types)
```

### Comparing `xsdata-24.4/xsdata/codegen/mixins.py` & `xsdata-24.5/xsdata/codegen/mixins.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,18 @@
         self.data: Dict[str, List[Class]] = {}
 
     @abc.abstractmethod
     def __iter__(self) -> Iterator[Class]:
         """Yield an iterator for the class map values."""
 
     @abc.abstractmethod
+    def process(self):
+        """Run the processor and filter steps."""
+
+    @abc.abstractmethod
     def find(self, qname: str, condition: Callable = return_true) -> Optional[Class]:
         """Find class that matches the given qualified name and condition callable.
 
         Classes are allowed to have the same qualified name, e.g. xsd:Element
         extending xsd:ComplexType with the same name, you can provide and additional
         callback to filter the classes like the tag.
```

### Comparing `xsdata-24.4/xsdata/codegen/models.py` & `xsdata-24.5/xsdata/codegen/models.py`

 * *Files 3% similar despite different names*

```diff
@@ -508,14 +508,15 @@
         default: The default value
         fixed: Specifies whether the default value is fixed
         substitutions: The list of all the substitution groups this class belongs to
         extensions: The list of all the extension instances
         attrs: The list of all the attr instances
         inner: The list of all the inner class instances
         ns_map: The namespace prefix-URI map
+        parent: The parent outer class
     """
 
     qname: str
     tag: str
     location: str = field(compare=False)
     mixed: bool = field(default=False)
     abstract: bool = field(default=False)
@@ -531,14 +532,15 @@
     default: Any = field(default=None, compare=False)
     fixed: bool = field(default=False, compare=False)
     substitutions: List[str] = field(default_factory=list)
     extensions: List[Extension] = field(default_factory=list)
     attrs: List[Attr] = field(default_factory=list)
     inner: List["Class"] = field(default_factory=list)
     ns_map: Dict = field(default_factory=dict)
+    parent: Optional["Class"] = field(default=None, compare=False)
 
     @property
     def name(self) -> str:
         """Shortcut for the class local name."""
         return namespaces.local_name(self.qname)
 
     @property
@@ -708,14 +710,24 @@
                 return True
 
             if any(choice for choice in attr.choices if choice.is_forward_ref):
                 return True
 
         return any(inner.has_forward_ref() for inner in self.inner)
 
+    def parent_names(self) -> List[str]:
+        """Return the outer class names."""
+        result = []
+        target = self.parent
+        while target is not None:
+            result.append(target.name)
+            target = target.parent
+
+        return list(reversed(result))
+
 
 @dataclass
 class Import:
     """Python import statement model representation.
 
     Args:
         qname: The qualified name of the imported class
```

### Comparing `xsdata-24.4/xsdata/codegen/parsers/definitions.py` & `xsdata-24.5/xsdata/codegen/parsers/definitions.py`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/xsdata/codegen/parsers/dtd.py` & `xsdata-24.5/xsdata/codegen/parsers/dtd.py`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/xsdata/codegen/parsers/schema.py` & `xsdata-24.5/xsdata/codegen/parsers/schema.py`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/xsdata/codegen/resolver.py` & `xsdata-24.5/xsdata/codegen/resolver.py`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/xsdata/codegen/transformer.py` & `xsdata-24.5/xsdata/codegen/transformer.py`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/xsdata/codegen/utils.py` & `xsdata-24.5/xsdata/codegen/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import sys
-from typing import Iterator, List, Optional, Set
+from collections import deque
+from typing import Deque, Iterator, List, Optional, Set
 
 from xsdata.codegen.exceptions import CodegenError
 from xsdata.codegen.models import (
     Attr,
     AttrType,
     Class,
     Extension,
@@ -110,34 +111,39 @@
                     continue
 
                 target.attrs.insert(index, clone)
 
             index += 1
 
     @classmethod
-    def copy_group_attributes(cls, source: Class, target: Class, attr: Attr):
+    def copy_group_attributes(
+        cls, source: Class, target: Class, attr: Attr, skip_inner_classes: bool = False
+    ):
         """Copy the attrs of the source class to the target class.
 
         The attr represents a reference to the source class which is
         derived from xs:group or xs:attributeGroup and will be removed.
 
         Args:
             source: The source class instance
             target: The target class instance
             attr: The group attr instance
+            skip_inner_classes: Whether the attr is circular reference, which
+                means we can skip copying the inner classes.
         """
         index = target.attrs.index(attr)
         target.attrs.pop(index)
 
         for source_attr in source.attrs:
             clone = cls.clone_attribute(source_attr, attr.restrictions)
             target.attrs.insert(index, clone)
             index += 1
 
-            cls.copy_inner_classes(source, target, clone)
+            if not skip_inner_classes:
+                cls.copy_inner_classes(source, target, clone)
 
     @classmethod
     def copy_extensions(cls, source: Class, target: Class, extension: Extension):
         """Copy the source class extensions to the target class instance.
 
         Merge the extension restrictions with the source class extensions
         restrictions.
@@ -191,48 +197,29 @@
             source: The source class instance
             target: The target class instance
             attr_type: The attr type with the possible forward reference
         """
         if not attr_type.forward:
             return
 
-        inner = ClassUtils.find_inner(source, attr_type.qname)
+        inner = ClassUtils.find_nested(source, attr_type.qname)
         if inner is target:
             attr_type.circular = True
             attr_type.reference = target.ref
         else:
             # In extreme cases this adds duplicate inner classes
             clone = inner.clone()
             clone.package = target.package
             clone.module = target.module
             clone.status = Status.RAW
             attr_type.reference = clone.ref
+            clone.parent = target
             target.inner.append(clone)
 
     @classmethod
-    def find_inner(cls, source: Class, qname: str) -> Class:
-        """Find an inner class in the source class by its qualified name.
-
-        Args:
-            source: The parent class instance
-            qname: The inner class qualified name
-
-        Returns:
-            The inner class instance
-
-        Raises:
-            CodeGenerationError: If no inner class matched.
-        """
-        for inner in source.inner:
-            if inner.qname == qname:
-                return inner
-
-        raise CodegenError("Missing inner class", parent=source, qname=qname)
-
-    @classmethod
     def find_attr(cls, source: Class, name: str) -> Optional[Attr]:
         """Find an attr in the source class by its name.
 
         Args:
             source: The source class instance
             name: The attr name to lookup
 
@@ -255,14 +242,15 @@
             target: The target class instance
             location: The source location of the target class
 
         Yields:
             An iterator over all the found classes.
         """
         target.location = location
+        target.parent = None
 
         while target.inner:
             yield from cls.flatten(target.inner.pop(), location)
 
         for attr in target.attrs:
             attr.types = collections.unique_sequence(attr.types, key="qname")
             for tp in attr.types:
@@ -489,7 +477,48 @@
                 lambda x: x.datatype in (DataType.ANY_TYPE, DataType.ANY_SIMPLE_TYPE),
             )
 
         if not types:
             types.append(AttrType(qname=str(DataType.STRING), native=True))
 
         return types
+
+    @classmethod
+    def find_nested(cls, target: Class, qname: str) -> Class:
+        """Find a nested class by qname.
+
+        Breath-first search implementation, that goes
+        from the current level to bottom before looking
+        for outer classes.
+
+        Args:
+            target: The class instance to begin the search
+            qname: The qualified name of the nested class to find
+
+        Raises:
+            CodegenException: If the nested class cannot be found.
+
+        Returns:
+            The nested class instance.
+        """
+        queue: Deque[Class] = deque()
+        visited: Set[int] = set()
+
+        if target.inner:
+            queue.extend(target.inner)
+        elif target.parent:
+            queue.append(target.parent)
+
+        while len(queue) > 0:
+            item = queue.popleft()
+            visited.add(item.ref)
+            if item.qname == qname:
+                return item
+
+            for inner in item.inner:
+                if inner.ref not in visited:
+                    queue.append(inner)
+
+            if len(queue) == 0 and item.parent:
+                queue.append(item.parent)
+
+        raise CodegenError("Missing inner class", parent=target, qname=qname)
```

### Comparing `xsdata-24.4/xsdata/codegen/validator.py` & `xsdata-24.5/xsdata/codegen/validator.py`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/xsdata/codegen/writer.py` & `xsdata-24.5/xsdata/codegen/writer.py`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/xsdata/exceptions.py` & `xsdata-24.5/xsdata/exceptions.py`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/xsdata/formats/converter.py` & `xsdata-24.5/xsdata/formats/converter.py`

 * *Files 1% similar despite different names*

```diff
@@ -156,14 +156,19 @@
         with warnings.catch_warnings(record=True) as w:
             decoded = self.deserialize(value, types, **kwargs)
 
         if w and w[-1].category is ConverterWarning:
             return False
 
         if strict and isinstance(decoded, (float, int, Decimal, XmlPeriod)):
+            if isinstance(decoded, float) and (
+                math.isinf(decoded) or math.isnan(decoded)
+            ):
+                return True
+
             encoded = self.serialize(decoded, **kwargs)
             return value.strip() == encoded
 
         return True
 
     def register_converter(self, data_type: Type, func: Union[Callable, Converter]):
         """Register a callable or converter for the given data type.
```

### Comparing `xsdata-24.4/xsdata/formats/dataclass/client.py` & `xsdata-24.5/xsdata/formats/dataclass/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,19 @@
-from typing import Any, Dict, NamedTuple, Optional, Type, Union
+from dataclasses import dataclass, fields
+from typing import Any, Dict, Optional, Type, Union
 
 from xsdata.exceptions import ClientValueError
 from xsdata.formats.dataclass.context import XmlContext
 from xsdata.formats.dataclass.parsers import DictDecoder, XmlParser
 from xsdata.formats.dataclass.serializers import XmlSerializer
 from xsdata.formats.dataclass.transports import DefaultTransport, Transport
 
 
-class Config(NamedTuple):
+@dataclass(frozen=True)
+class Config:
     """Service configuration class.
 
     Attributes:
         style: The binding style
         location: The service endpoint url
         transport: The transport namespace
         soap_action: The soap action
@@ -41,16 +43,16 @@
                 input: The input class
                 output: The output class
 
         Returns:
             A new config instance.
         """
         params = {
-            key: kwargs[key] if key in kwargs else getattr(obj, key, None)
-            for key in cls._fields
+            f.name: kwargs[f.name] if f.name in kwargs else getattr(obj, f.name, None)
+            for f in fields(cls)
         }
 
         return cls(**params)
 
 
 class TransportTypes:
     """Transport types."""
```

### Comparing `xsdata-24.4/xsdata/formats/dataclass/compat.py` & `xsdata-24.5/xsdata/formats/dataclass/compat.py`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/xsdata/formats/dataclass/context.py` & `xsdata-24.5/xsdata/formats/dataclass/context.py`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/xsdata/formats/dataclass/filters.py` & `xsdata-24.5/xsdata/formats/dataclass/filters.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,14 +15,15 @@
     Type,
 )
 
 from docformatter import configuration, format
 from jinja2 import Environment
 
 from xsdata.codegen.models import Attr, AttrType, Class
+from xsdata.codegen.utils import ClassUtils
 from xsdata.formats.converter import converter
 from xsdata.formats.dataclass.models.elements import XmlType
 from xsdata.models.config import (
     DocstringStyle,
     ExtensionType,
     GeneratorConfig,
     GeneratorExtension,
@@ -239,22 +240,22 @@
         for search, replace in self.substitutions[obj_type].items():
             name = re.sub(rf"{search}", rf"{replace}", name)
 
         return name
 
     def field_definition(
         self,
+        obj: Class,
         attr: Attr,
-        ns_map: Dict,
         parent_namespace: Optional[str],
-        parents: List[str],
     ) -> str:
         """Return the field definition with any extra metadata."""
+        ns_map = obj.ns_map
         default_value = self.field_default_value(attr, ns_map)
-        metadata = self.field_metadata(attr, parent_namespace, parents)
+        metadata = self.field_metadata(obj, attr, parent_namespace)
 
         kwargs: Dict[str, Any] = {}
         if attr.fixed or attr.is_prohibited:
             kwargs["init"] = False
 
         if default_value is not False and not attr.is_prohibited:
             key = self.FACTORY_KEY if attr.is_factory else self.DEFAULT_KEY
@@ -417,54 +418,54 @@
 
     def post_meta_hook(self, obj: Class) -> Optional[str]:
         """Plugin hook to render additional information after the xsdata meta class."""
         return None
 
     def field_metadata(
         self,
+        obj: Class,
         attr: Attr,
         parent_namespace: Optional[str],
-        parents: List[str],
     ) -> Dict:
         """Return a metadata dictionary for the given attribute."""
         if attr.is_prohibited:
             return {"type": XmlType.IGNORE}
 
         name = namespace = None
 
         if not attr.is_nameless and attr.local_name != self.field_name(
-            attr.name, parents[-1]
+            attr.name, obj.name
         ):
             name = attr.local_name
 
         if parent_namespace != attr.namespace or attr.is_attribute:
             namespace = attr.namespace
 
         restrictions = attr.restrictions.asdict(attr.native_types)
 
         metadata = {
             "wrapper": attr.wrapper,
             "name": name,
             "type": attr.xml_type,
             "namespace": namespace,
             "mixed": attr.mixed,
-            "choices": self.field_choices(attr, parent_namespace, parents),
+            "choices": self.field_choices(obj, attr, parent_namespace),
             **restrictions,
         }
 
         if self.docstring_style == DocstringStyle.ACCESSIBLE and attr.help:
             metadata["doc"] = self.clean_docstring(attr.help, False)
 
         return self.filter_metadata(metadata)
 
     def field_choices(
         self,
+        obj: Class,
         attr: Attr,
         parent_namespace: Optional[str],
-        parents: List[str],
     ) -> Optional[Tuple]:
         """Return a tuple of field metadata if the attr has choices."""
         if not attr.choices:
             return None
 
         result = []
         for choice in attr.choices:
@@ -473,15 +474,15 @@
             namespace = (
                 choice.namespace if parent_namespace != choice.namespace else None
             )
 
             metadata = {
                 "name": choice.local_name,
                 "wildcard": choice.is_wildcard,
-                "type": self.choice_type(choice, parents),
+                "type": self.choice_type(obj, choice),
                 "namespace": namespace,
             }
 
             if choice.is_nameless:
                 del metadata["name"]
 
             if choice.is_tokens:
@@ -553,18 +554,19 @@
     def format_string(self, data: str, indent: int, key: str = "", pad: int = 0) -> str:
         """Return a pretty string representation of a string.
 
         If the total length of the input string plus indent plus the key
         length and the additional pad is more than the max line length,
         wrap the text into multiple lines, avoiding breaking long words
         """
-        if (data.startswith("Type[") or data.startswith("type[")) and data.endswith(
-            "]"
-        ):
-            return data if data[5] == '"' else data[5:-1]
+        if data.startswith("ForwardRef("):
+            return data
+
+        if data.startswith("Type["):
+            return data[5:-1]
 
         if data.startswith("Literal[") and data.endswith("]"):
             return data[8:-1]
 
         if key in (self.FACTORY_KEY, self.DEFAULT_KEY):
             return data
 
@@ -737,23 +739,23 @@
         )
 
         if attr.is_enumeration:
             return self.format_metadata(tuple(tokens), indent=8)
 
         return f"lambda: {self.format_metadata(tokens, indent=8)}"
 
-    def field_type(self, attr: Attr, parents: List[str]) -> str:
+    def field_type(self, obj: Class, attr: Attr) -> str:
         """Generate type hints for the given attr."""
         if attr.is_prohibited:
             return "Any"
 
         if attr.tag == Tag.CHOICE:
-            return self.compound_field_types(attr, parents)
+            return self.compound_field_types(obj, attr)
 
-        result = self._field_type_names(attr, parents, choice=False)
+        result = self._field_type_names(obj, attr, choice=False)
 
         iterable_fmt = self._get_iterable_format()
         if attr.is_tokens:
             result = iterable_fmt.format(result)
 
         if attr.is_list:
             return iterable_fmt.format(result)
@@ -767,101 +769,96 @@
         if attr.is_nillable or (
             attr.default is None and (attr.is_optional or not self.format.kw_only)
         ):
             return f"None | {result}" if self.union_type else f"Optional[{result}]"
 
         return result
 
-    def compound_field_types(self, attr: Attr, parents: List[str]) -> str:
+    def compound_field_types(self, obj: Class, attr: Attr) -> str:
         """Generate type hint for a compound field.
 
         Args:
+            obj: The parent class instance
             attr: The compound attr instance
-            parents: A list of the parent class names
 
         Returns:
             The string representation of the type hint.
         """
         results = []
         iterable_fmt = self._get_iterable_format()
         for choice in attr.choices:
-            names = self._field_type_names(choice, parents, choice=False)
+            names = self._field_type_names(obj, choice, choice=False)
             if choice.is_tokens:
                 names = iterable_fmt.format(names)
             results.append(names)
 
         result = self._join_type_names(results)
 
         if attr.is_list:
             return iterable_fmt.format(result)
 
         if attr.is_optional or not self.format.kw_only:
             return f"None | {result}" if self.union_type else f"Optional[{result}]"
 
         return result
 
-    def choice_type(self, choice: Attr, parents: List[str]) -> str:
+    def choice_type(self, obj: Class, choice: Attr) -> str:
         """Generate type hints for the given choice.
 
         Choices support a subset of features from normal attributes.
         First of all we don't have a proper type hint but a type
         metadata key. That's why we always need to wrap as Type[xxx].
         The second big difference is that our choice belongs to a
         compound field that might be a list, that's why list restriction
         is also ignored.
 
         Args:
+            obj: The parent class instance
             choice: The choice instance
-            parents: A list of the parent class names
 
         Returns:
             The string representation of the type hint.
         """
-        result = self._field_type_names(choice, parents, choice=True)
+        result = self._field_type_names(obj, choice, choice=True)
 
         if choice.is_tokens:
             iterable_fmt = self._get_iterable_format()
             result = iterable_fmt.format(result)
 
-        if self.subscriptable_types:
-            return f"type[{result}]"
+        if result.startswith('"'):
+            return f"ForwardRef({result})"
 
         return f"Type[{result}]"
 
     def _field_type_names(
         self,
+        obj: Class,
         attr: Attr,
-        parents: List[str],
         choice: bool = False,
     ) -> str:
-        type_names = [
-            self._field_type_name(x, parents, choice=choice) for x in attr.types
-        ]
+        type_names = [self._field_type_name(obj, x, choice=choice) for x in attr.types]
         return self._join_type_names(type_names)
 
     def _join_type_names(self, type_names: List[str]) -> str:
         type_names = collections.unique_sequence(type_names)
         if len(type_names) == 1:
             return type_names[0]
 
         if self.union_type:
             return " | ".join(type_names)
 
         return f'Union[{", ".join(type_names)}]'
 
     def _field_type_name(
-        self, attr_type: AttrType, parents: List[str], choice: bool = False
+        self, obj: Class, attr_type: AttrType, choice: bool = False
     ) -> str:
         name = self.type_name(attr_type)
-
-        if attr_type.forward and attr_type.circular:
-            outer_str = ".".join(map(self.class_name, parents))
-            name = f'"{outer_str}"'
-        elif attr_type.forward:
-            outer_str = ".".join(map(self.class_name, parents))
+        if attr_type.forward:
+            inner = ClassUtils.find_nested(obj, attr_type.qname)
+            outer_str = ".".join(map(self.class_name, inner.parent_names()))
             name = f'"{outer_str}.{name}"'
         elif attr_type.circular:
             name = f'"{name}"'
 
         if self.postponed_annotations and not choice:
             name = name.strip('"')
 
@@ -911,16 +908,16 @@
             "decimal": {"Decimal": type_patterns("Decimal")},
             "enum": {"Enum": ["(Enum)"]},
             "typing": {
                 "Dict": [": Dict"],
                 "List": [": List["],
                 "Optional": ["Optional["],
                 "Tuple": ["Tuple["],
-                "Type": ["Type["],
                 "Union": ["Union["],
+                "ForwardRef": [": ForwardRef("],
                 "Any": type_patterns("Any"),
             },
             "xml.etree.ElementTree": {"QName": type_patterns("QName")},
             "xsdata.models.datatype": {
                 "XmlDate": type_patterns("XmlDate"),
                 "XmlDateTime": type_patterns("XmlDateTime"),
                 "XmlDuration": type_patterns("XmlDuration"),
```

### Comparing `xsdata-24.4/xsdata/formats/dataclass/generator.py` & `xsdata-24.5/xsdata/formats/dataclass/generator.py`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/xsdata/formats/dataclass/models/builders.py` & `xsdata-24.5/xsdata/formats/dataclass/models/builders.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,20 +16,37 @@
     get_type_hints,
 )
 
 from xsdata.exceptions import XmlContextError
 from xsdata.formats.converter import converter
 from xsdata.formats.dataclass.compat import ClassType
 from xsdata.formats.dataclass.models.elements import XmlMeta, XmlType, XmlVar
-from xsdata.formats.dataclass.typing import evaluate
+from xsdata.formats.dataclass.typing import (
+    evaluate,
+    evaluate_attribute,
+    evaluate_attributes,
+    evaluate_element,
+    evaluate_elements,
+    evaluate_text,
+    evaluate_wildcard,
+)
 from xsdata.models.enums import NamespaceType
 from xsdata.utils.collections import first
 from xsdata.utils.constants import EMPTY_SEQUENCE, return_input
 from xsdata.utils.namespaces import build_qname
 
+evaluations: Dict[str, Callable] = {
+    XmlType.TEXT: evaluate_text,
+    XmlType.ELEMENT: evaluate_element,
+    XmlType.ELEMENTS: evaluate_elements,
+    XmlType.WILDCARD: evaluate_wildcard,
+    XmlType.ATTRIBUTE: evaluate_attribute,
+    XmlType.ATTRIBUTES: evaluate_attributes,
+}
+
 
 class ClassMeta:
     """The binding model combined metadata.
 
     Args:
         element_name_generator: The element name generator
         attribute_name_generator: The attribute name generator
@@ -345,28 +362,28 @@
         name: str,
         type_hint: Any,
         metadata: Mapping[str, Any],
         init: bool,
         parent_namespace: Optional[str],
         default_value: Any,
         globalns: Any,
-        factory: Optional[Callable] = None,
+        parent_factory: Optional[Callable] = None,
     ) -> Optional[XmlVar]:
         """Build the binding metadata for a class field.
 
         Args:
             model: The model class
             name: The model field name
             type_hint: The typing annotations of the field
             metadata: The field metadata mapping
             init: Specify whether this field can be initialized
             parent_namespace: The class namespace
             default_value: The field default value or factory
             globalns: Python's global namespace
-            factory: The value factory
+            parent_factory: The value factory
 
         Returns:
             The field binding metadata instance.
         """
         xml_type = metadata.get("type", self.default_xml_type)
         if xml_type == XmlType.IGNORE:
             return None
@@ -379,45 +396,41 @@
         process_contents = metadata.get("process_contents", "strict")
         required = metadata.get("required", False)
         nillable = metadata.get("nillable", False)
         format_str = metadata.get("format", None)
         sequence = metadata.get("sequence", None)
         wrapper = metadata.get("wrapper", None)
 
-        origin, sub_origin, types = self.analyze_types(model, name, type_hint, globalns)
+        annotation = evaluate(type_hint, globalns)
+
+        try:
+            analyze = evaluations[xml_type]
+            types, factory, tokens_factory = analyze(annotation, tokens=tokens)
+            types = tuple(converter.sort_types(types))
+            if not self.is_typing_supported(types):
+                raise TypeError
 
-        if not self.is_valid(xml_type, origin, sub_origin, types, tokens, init):
+        except TypeError:
             raise XmlContextError(
                 f"Error on {model.__qualname__}::{name}: "
                 f"Xml {xml_type} does not support typing `{type_hint}`"
             )
 
-        if xml_type == XmlType.ELEMENTS:
-            sub_origin = None
-            types = (object,)
-
+        factory = factory or parent_factory
         local_name = local_name or self.build_local_name(xml_type, name)
-
-        if tokens and sub_origin is None:
-            sub_origin = origin
-            origin = None
-
-        if origin is None:
-            origin = factory
-
         any_type = self.is_any_type(types, xml_type)
         clazz = first(tp for tp in types if self.class_type.is_model(tp))
         namespaces = self.resolve_namespaces(xml_type, namespace, parent_namespace)
 
         elements = {}
         wildcards = []
         self.index += 1
         cur_index = self.index
         for choice in self.build_choices(
-            model, name, choices, origin, globalns, parent_namespace
+            model, name, choices, factory, globalns, parent_namespace
         ):
             if choice.is_element:
                 elements[choice.qname] = choice
             else:  # choice.is_wildcard:
                 wildcards.append(choice)
 
         return XmlVar(
@@ -430,30 +443,30 @@
             format=format_str,
             clazz=clazz,
             any_type=any_type,
             process_contents=process_contents,
             required=required,
             nillable=nillable,
             sequence=sequence,
-            factory=origin,
-            tokens_factory=sub_origin,
+            factory=factory,
+            tokens_factory=tokens_factory,
             default=default_value,
             types=types,
             elements=elements,
             wildcards=wildcards,
             namespaces=namespaces,
             xml_type=xml_type,
         )
 
     def build_choices(
         self,
         model: Type,
         name: str,
         choices: List[Dict],
-        factory: Callable,
+        factory: Optional[Callable],
         globalns: Any,
         parent_namespace: Optional[str],
     ) -> Iterator[XmlVar]:
         """Build the binding metadata for a compound dataclass field.
 
         Args:
             model: The model class
@@ -566,86 +579,14 @@
     def is_any_type(cls, types: Sequence[Type], xml_type: str) -> bool:
         """Return whether the given xml type supports generic values."""
         if xml_type in (XmlType.ELEMENT, XmlType.ELEMENTS):
             return object in types
 
         return False
 
-    @classmethod
-    def analyze_types(
-        cls,
-        model: Type,
-        name: str,
-        type_hint: Any,
-        globalns: Any,
-    ) -> Tuple[Any, Any, Tuple[Type, ...]]:
-        """Analyze a type hint and return the origin, sub origin and the type args.
-
-        The only case we support a sub origin is for fields derived from
-        xs:NMTOKENS!
-
-        # Todo please rewrite this in a way that makes sense :(
-
-        Raises:
-            XmlContextError: if the typing is not supported for binding
-        """
-        try:
-            types = evaluate(type_hint, globalns)
-            origin = None
-            sub_origin = None
-
-            while types[0] in (tuple, list, dict):
-                if origin is None:
-                    origin = types[0]
-                elif sub_origin is None:
-                    sub_origin = types[0]
-                else:
-                    raise TypeError()
-
-                types = types[1:]
-
-            return origin, sub_origin, tuple(converter.sort_types(types))
-        except Exception:
-            raise XmlContextError(
-                f"Error on {model.__qualname__}::{name}: "
-                f"Unsupported field typing `{type_hint}`"
-            )
-
-    def is_valid(
-        self,
-        xml_type: str,
-        origin: Any,
-        sub_origin: Any,
-        types: Sequence[Type],
-        tokens: bool,
-        init: bool,
-    ) -> bool:
-        """Validate the given xml type against common unsupported cases."""
-        if not init:
-            # Ignore init==false vars
-            return True
-
-        if xml_type == XmlType.ATTRIBUTES:
-            # Attributes need origin dict, no sub origin and tokens
-            if origin is not dict or sub_origin or tokens:
-                return False
-        elif origin is dict or tokens and origin not in (list, tuple):
-            # Origin dict is only supported by Attributes
-            # xs:NMTOKENS need origin list
-            return False
-
-        if object in types and xml_type != XmlType.ELEMENTS:
-            # Any type, secondary types are not allowed except for 'Elements' XML type
-            return len(types) == 1
-
-        if xml_type == XmlType.ELEMENTS:
-            return True
-
-        return self.is_typing_supported(types)
-
     def is_typing_supported(self, types: Sequence[Type]) -> bool:
         """Validate all types are registered in the converter."""
         for tp in types:
             if (
                 not self.class_type.is_model(tp)
                 and tp not in converter.registry
                 and not issubclass(tp, Enum)
```

### Comparing `xsdata-24.4/xsdata/formats/dataclass/models/elements.py` & `xsdata-24.5/xsdata/formats/dataclass/models/elements.py`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/xsdata/formats/dataclass/models/generics.py` & `xsdata-24.5/xsdata/formats/dataclass/models/generics.py`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/xsdata/formats/dataclass/parsers/bases.py` & `xsdata-24.5/xsdata/formats/dataclass/parsers/bases.py`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/xsdata/formats/dataclass/parsers/config.py` & `xsdata-24.5/xsdata/formats/dataclass/parsers/config.py`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/xsdata/formats/dataclass/parsers/dict.py` & `xsdata-24.5/xsdata/formats/dataclass/parsers/dict.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 import warnings
 from dataclasses import dataclass, field
 from typing import Any, Dict, Iterable, List, Optional, Type, Union
 
+from typing_extensions import get_args, get_origin
+
 from xsdata.exceptions import ConverterWarning, ParserError
 from xsdata.formats.converter import converter
 from xsdata.formats.dataclass.context import XmlContext
 from xsdata.formats.dataclass.models.elements import XmlMeta, XmlVar
 from xsdata.formats.dataclass.parsers.config import ParserConfig
 from xsdata.formats.dataclass.parsers.utils import ParserUtils
-from xsdata.formats.dataclass.typing import get_args, get_origin
 from xsdata.formats.types import T
 from xsdata.utils import collections
 from xsdata.utils.constants import EMPTY_MAP
 
 
 @dataclass
 class DictDecoder:
@@ -128,33 +129,39 @@
         meta = self.context.build(clazz)
         xml_vars = meta.get_all_vars()
 
         params = {}
         for key, value in data.items():
             var = self.find_var(xml_vars, key, value)
 
-            if var is None and self.config.fail_on_unknown_properties:
-                raise ParserError(f"Unknown property {clazz.__qualname__}.{key}")
-
-            if var and var.init:
-                if var.wrapper:
-                    value = value[var.local_name]
-
-                params[var.name] = self.bind_value(meta, var, value)
+            if var is None:
+                if self.config.fail_on_unknown_properties:
+                    raise ParserError(f"Unknown property {clazz.__qualname__}.{key}")
+                else:
+                    continue
+
+            if var.wrapper:
+                value = value[var.local_name]
+
+            value = self.bind_value(meta, var, value)
+            if var.init:
+                params[var.name] = value
+            else:
+                ParserUtils.validate_fixed_value(meta, var, value)
 
         try:
             return self.config.class_factory(clazz, params)
         except TypeError as e:
             raise ParserError(e)
 
     def bind_derived_dataclass(self, data: Dict, clazz: Type[T]) -> Any:
         """Bind the input data to the given class type.
 
         Examples:
-            >>> {
+            {
                 "qname": "foo",
                 "type": "my:type",
                 "value": {"prop": "value"}
             }
 
         Args:
             data: The derived element dictionary
```

### Comparing `xsdata-24.4/xsdata/formats/dataclass/parsers/handlers/__init__.py` & `xsdata-24.5/xsdata/formats/dataclass/parsers/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/xsdata/formats/dataclass/parsers/handlers/lxml.py` & `xsdata-24.5/xsdata/formats/dataclass/parsers/handlers/lxml.py`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/xsdata/formats/dataclass/parsers/handlers/native.py` & `xsdata-24.5/xsdata/formats/dataclass/parsers/handlers/native.py`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/xsdata/formats/dataclass/parsers/json.py` & `xsdata-24.5/xsdata/formats/dataclass/parsers/json.py`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/xsdata/formats/dataclass/parsers/mixins.py` & `xsdata-24.5/xsdata/formats/dataclass/parsers/mixins.py`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/xsdata/formats/dataclass/parsers/nodes/__init__.py` & `xsdata-24.5/xsdata/formats/dataclass/parsers/nodes/__init__.py`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/xsdata/formats/dataclass/parsers/nodes/element.py` & `xsdata-24.5/xsdata/formats/dataclass/parsers/nodes/element.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import math
 from typing import Any, Dict, List, Optional, Set, Type
 
 from xsdata.exceptions import ParserError
 from xsdata.formats.converter import converter
 from xsdata.formats.dataclass.context import XmlContext
 from xsdata.formats.dataclass.models.elements import XmlMeta, XmlVar
 from xsdata.formats.dataclass.parsers import nodes
@@ -187,23 +188,27 @@
         Ignores fields with init==false!
 
         Args:
             params: The class parameters
             var: The xml var instance
             value: The attribute value
         """
+        value = ParserUtils.parse_value(
+            value=value,
+            types=var.types,
+            default=var.default,
+            ns_map=self.ns_map,
+            tokens_factory=var.tokens_factory,
+            format=var.format,
+        )
+
         if var.init:
-            params[var.name] = ParserUtils.parse_value(
-                value=value,
-                types=var.types,
-                default=var.default,
-                ns_map=self.ns_map,
-                tokens_factory=var.tokens_factory,
-                format=var.format,
-            )
+            params[var.name] = value
+        else:
+            ParserUtils.validate_fixed_value(self.meta, var, value)
 
     def bind_any_attr(self, params: Dict, var: XmlVar, qname: str, value: Any):
         """Parse an element attribute to a wildcard field.
 
         Args:
             params: The class parameters
             var: The xml var instance
@@ -360,26 +365,31 @@
             parameters or not.
         """
         var = self.meta.text
 
         if not var or (text is None and not self.xsi_nil):
             return False
 
+        if self.xsi_nil and not text:
+            value = None
+        else:
+            value = ParserUtils.parse_value(
+                value=text,
+                types=var.types,
+                default=var.default,
+                ns_map=self.ns_map,
+                tokens_factory=var.tokens_factory,
+                format=var.format,
+            )
+
         if var.init:
-            if self.xsi_nil and not text:
-                params[var.name] = None
-            else:
-                params[var.name] = ParserUtils.parse_value(
-                    value=text,
-                    types=var.types,
-                    default=var.default,
-                    ns_map=self.ns_map,
-                    tokens_factory=var.tokens_factory,
-                    format=var.format,
-                )
+            params[var.name] = value
+        else:
+            ParserUtils.validate_fixed_value(self.meta, var, value)
+
         return True
 
     def bind_wild_text(
         self,
         params: Dict,
         var: XmlVar,
         text: Optional[str],
```

### Comparing `xsdata-24.4/xsdata/formats/dataclass/parsers/nodes/primitive.py` & `xsdata-24.5/xsdata/formats/dataclass/parsers/nodes/primitive.py`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/xsdata/formats/dataclass/parsers/nodes/skip.py` & `xsdata-24.5/xsdata/formats/dataclass/parsers/nodes/skip.py`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/xsdata/formats/dataclass/parsers/nodes/standard.py` & `xsdata-24.5/xsdata/formats/dataclass/parsers/nodes/standard.py`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/xsdata/formats/dataclass/parsers/nodes/union.py` & `xsdata-24.5/xsdata/formats/dataclass/parsers/nodes/union.py`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/xsdata/formats/dataclass/parsers/nodes/wildcard.py` & `xsdata-24.5/xsdata/formats/dataclass/parsers/nodes/wildcard.py`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/xsdata/formats/dataclass/parsers/nodes/wrapper.py` & `xsdata-24.5/xsdata/formats/dataclass/parsers/nodes/wrapper.py`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/xsdata/formats/dataclass/parsers/tree.py` & `xsdata-24.5/xsdata/formats/dataclass/parsers/tree.py`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/xsdata/formats/dataclass/parsers/utils.py` & `xsdata-24.5/xsdata/formats/dataclass/parsers/utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,14 @@
+import math
 from collections import UserList
 from typing import Any, Callable, Dict, Iterable, Optional, Sequence, Type
 
+from xsdata.exceptions import ParserError
 from xsdata.formats.converter import QNameConverter, converter
+from xsdata.formats.dataclass.models.elements import XmlMeta, XmlVar
 from xsdata.models.enums import QNames
 from xsdata.utils import collections, constants, text
 from xsdata.utils.namespaces import build_qname
 
 
 class PendingCollection(UserList):
     """An iterable implementation of parsed values.
@@ -158,7 +161,35 @@
             The expanded value.
         """
         prefix, suffix = text.split(value)
         if prefix and prefix in ns_map and not suffix.startswith("//"):
             value = build_qname(ns_map[prefix], suffix)
 
         return value
+
+    @classmethod
+    def validate_fixed_value(cls, meta: XmlMeta, var: XmlVar, value: Any):
+        """Validate if the parsed value matches the fixed value.
+
+        Special cases
+            - float nans are never equal in python
+            - strings with whitespaces, need trimming
+
+        """
+
+        default_value = var.default() if callable(var.default) else var.default
+        if (
+            isinstance(default_value, float)
+            and isinstance(value, float)
+            and math.isnan(default_value)
+            and math.isnan(value)
+        ) or (
+            isinstance(default_value, str)
+            and isinstance(value, str)
+            and default_value.strip() == value.strip()
+        ):
+            return
+
+        if default_value != value:
+            raise ParserError(
+                f"Fixed value mismatch {meta.qname}:{var.qname}, `{default_value} != {value}`"
+            )
```

### Comparing `xsdata-24.4/xsdata/formats/dataclass/parsers/xml.py` & `xsdata-24.5/xsdata/formats/dataclass/parsers/xml.py`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/xsdata/formats/dataclass/serializers/__init__.py` & `xsdata-24.5/xsdata/formats/dataclass/serializers/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 from xsdata.formats.dataclass.serializers.code import PycodeSerializer
 from xsdata.formats.dataclass.serializers.dict import DictEncoder, DictFactory
 from xsdata.formats.dataclass.serializers.json import JsonSerializer
-from xsdata.formats.dataclass.serializers.tree.native import XmlTreeSerializer
 from xsdata.formats.dataclass.serializers.xml import XmlSerializer
 
 __all__ = [
     "DictEncoder",
     "DictFactory",
     "JsonSerializer",
     "XmlSerializer",
     "PycodeSerializer",
 ]
 
 try:
-    from xsdata.formats.dataclass.serializers.tree.lxml import LxmlTreeSerializer
+    from xsdata.formats.dataclass.serializers.tree import TreeSerializer
 
-    __all__.append("LxmlTreeSerializer")
+    __all__.append("TreeSerializer")
 except ImportError:  # pragma: no cover
-    pass  # pragma: no cover
+    pass
```

### Comparing `xsdata-24.4/xsdata/formats/dataclass/serializers/code.py` & `xsdata-24.5/xsdata/formats/dataclass/serializers/code.py`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/xsdata/formats/dataclass/serializers/config.py` & `xsdata-24.5/xsdata/formats/dataclass/serializers/config.py`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/xsdata/formats/dataclass/serializers/dict.py` & `xsdata-24.5/xsdata/formats/dataclass/serializers/dict.py`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/xsdata/formats/dataclass/serializers/json.py` & `xsdata-24.5/xsdata/formats/dataclass/serializers/json.py`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/xsdata/formats/dataclass/serializers/mixins.py` & `xsdata-24.5/xsdata/formats/dataclass/serializers/mixins.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import abc
+from abc import ABC
 from dataclasses import dataclass, field
 from enum import Enum
 from typing import (
     Any,
     Dict,
     Final,
     Iterable,
@@ -45,71 +46,52 @@
 AttrEvent: TypeAlias = Tuple[Literal["attr"], str, Any]
 DataEvent: TypeAlias = Tuple[Literal["data"], str]
 EndEvent: TypeAlias = Tuple[Literal["end"], str]
 
 EventIterator = Iterator[Union[StartEvent, AttrEvent, DataEvent, EndEvent]]
 
 
-class XmlWriter(abc.ABC):
-    """A consistency wrapper for sax content handlers.
+class EventHandler(abc.ABC):
+    """A consistency wrapper for sax events.
 
     Args:
         config: The serializer config instance
-        output: The output stream to write the result
         ns_map: A user defined namespace prefix-URI map
 
     Attributes:
-        handler: The content handler instance
         in_tail: Specifies whether the text content has been written
         tail: The current element tail content
         attrs: The current element attributes
         ns_context: The namespace context queue
         pending_tag: The pending element namespace, name tuple
         pending_prefixes: The pending element namespace prefixes
     """
 
     __slots__ = (
         "config",
-        "output",
         "ns_map",
         # Instance attributes
-        "handler",
         "in_tail",
         "tail",
         "attrs",
         "ns_context",
         "pending_tag",
         "pending_prefixes",
     )
 
-    def __init__(
-        self,
-        config: SerializerConfig,
-        output: TextIO,
-        ns_map: Dict,
-    ):
+    def __init__(self, config: SerializerConfig, ns_map: Dict):
         self.config = config
-        self.output = output
         self.ns_map = ns_map
 
         self.in_tail = False
         self.tail: Optional[str] = None
         self.attrs: Dict = {}
         self.ns_context: List[Dict] = []
         self.pending_tag: Optional[Tuple] = None
         self.pending_prefixes: List[List] = []
-        self.handler = self.build_handler()
-
-    @abc.abstractmethod
-    def build_handler(self) -> ContentHandler:
-        """Build the content handler instance.
-
-        Returns:
-            A content handler instance.
-        """
 
     def write(self, events: EventIterator):
         """Feed the sax content handler with events.
 
         The receiver will also add additional root attributes
         like xsi or no namespace location.
 
@@ -143,25 +125,15 @@
             elif name == XmlWriterEvent.ATTR:
                 self.add_attribute(*args)
             elif name == XmlWriterEvent.DATA:
                 self.set_data(*args)
             else:
                 raise XmlWriterError(f"Unhandled event: `{name}`")
 
-        self.handler.endDocument()
-
-    def start_document(self):
-        """Start document notification receiver.
-
-        Write the xml version and encoding, if the
-        configuration is enabled.
-        """
-        if self.config.xml_declaration:
-            self.output.write(f'<?xml version="{self.config.xml_version}"')
-            self.output.write(f' encoding="{self.config.encoding}"?>\n')
+        self.end_document()
 
     def start_tag(self, qname: str):
         """Start tag notification receiver.
 
         The receiver will flush the start of any pending element, create
         new namespaces context and queue the current tag for generation.
 
@@ -226,15 +198,15 @@
             data: The element text or tail content
         """
         value = self.encode_data(data)
         self.flush_start(is_nil=value is None)
 
         if value:
             if not self.in_tail:
-                self.handler.characters(value)
+                self.set_characters(value)
             else:
                 self.tail = value
 
         self.in_tail = True
 
     def end_tag(self, qname: str):
         """End tag notification receiver.
@@ -243,27 +215,27 @@
         the element, its tail content and its namespaces prefix mapping
         and current context.
 
         Args:
             qname: The qualified name of the element
         """
         self.flush_start(True)
-        self.handler.endElementNS(split_qname(qname), "")
+        self.end_element(split_qname(qname), qname)
 
         if self.tail:
-            self.handler.characters(self.tail)
+            self.set_characters(self.tail)
 
         self.tail = None
         self.in_tail = False
         self.ns_context.pop()
         if self.ns_context:
             self.ns_map = self.ns_context[-1]
 
         for prefix in self.pending_prefixes.pop():
-            self.handler.endPrefixMapping(prefix)
+            self.end_prefix_mapping(prefix)
 
     def flush_start(self, is_nil: bool = True):
         """Flush start notification receiver.
 
         The receiver will pop the xsi:nil attribute if the element is
         not empty, prepare and send the namespace prefix-URI map and
         the element with its attributes to the content handler for
@@ -281,15 +253,15 @@
 
         for name in self.attrs:
             self.add_namespace(name[0])
 
         self.reset_default_namespace()
         self.start_namespaces()
 
-        self.handler.startElementNS(self.pending_tag, "", self.attrs)  # type: ignore
+        self.start_element(self.pending_tag, "", self.attrs)
         self.attrs = {}
         self.in_tail = False
         self.pending_tag = None
 
     def start_namespaces(self):
         """Send the current namespace prefix-URI map to the content handler.
 
@@ -303,15 +275,15 @@
             parent_ns_map = self.ns_context[-2]
         except IndexError:
             parent_ns_map = EMPTY_MAP
 
         for prefix, uri in self.ns_map.items():
             if parent_ns_map.get(prefix) != uri:
                 prefixes.append(prefix)
-                self.handler.startPrefixMapping(prefix, uri)
+                self.start_prefix_mapping(prefix, uri)
 
     def reset_default_namespace(self):
         """Reset the default namespace if the pending element is not qualified."""
         if self.pending_tag and not self.pending_tag[0] and None in self.ns_map:
             self.ns_map[None] = ""
 
     @classmethod
@@ -343,14 +315,185 @@
             return data
 
         if isinstance(data, list) and not data:
             return None
 
         return converter.serialize(data, ns_map=self.ns_map)
 
+    @abc.abstractmethod
+    def start_document(self):
+        """Start document notification receiver."""
+
+    @abc.abstractmethod
+    def end_document(self):
+        """End document notification receiver."""
+
+    @abc.abstractmethod
+    def start_element(self, name: Tuple[str, str], qname: str, attrs: Dict):
+        """Start element notification receiver.
+
+        Args:
+            name: The qname as tuple
+            qname: The qualified name
+            attrs: The attributes mapping
+        """
+
+    @abc.abstractmethod
+    def end_element(self, name: Tuple[str, str], qname: str):
+        """End element notification receiver.
+
+        Args:
+            name: The qname as tuple
+            qname: The qualified name
+        """
+
+    @abc.abstractmethod
+    def set_characters(self, data: str):
+        """Characters notification receiver.
+
+        Args:
+            data: The characters data to write
+        """
+
+    @abc.abstractmethod
+    def start_prefix_mapping(self, prefix: Optional[str], uri: str):
+        """Start namespace prefix notification receiver.
+
+        Args:
+            prefix: The namespace prefix
+            uri: The namespace URI
+        """
+
+    @abc.abstractmethod
+    def end_prefix_mapping(self, prefix: str):
+        """End namespace prefix notification receiver.
+
+        Args:
+            prefix: The namespace prefix
+        """
+
+
+class EventContentHandler(EventHandler):
+    """A consistency wrapper for sax content handlers.
+
+    Args:
+        config: The serializer config instance
+        ns_map: A user defined namespace prefix-URI map
+
+    Attributes:
+        handler: The content handler instance
+        in_tail: Specifies whether the text content has been written
+        tail: The current element tail content
+        attrs: The current element attributes
+        ns_context: The namespace context queue
+        pending_tag: The pending element namespace, name tuple
+        pending_prefixes: The pending element namespace prefixes
+    """
+
+    def __init__(self, config: SerializerConfig, ns_map: Dict):
+        super().__init__(config, ns_map)
+        self.handler = self.build_handler()
+
+    @abc.abstractmethod
+    def build_handler(self) -> ContentHandler:
+        """Build the content handler instance.
+
+        Returns:
+            A content handler instance.
+        """
+
+    def start_document(self):
+        """Start document notification receiver.
+
+        Write the xml version and encoding, if the
+        configuration is enabled.
+        """
+        self.handler.startDocument()
+
+    def end_document(self):
+        """End document entrypoint."""
+        self.handler.endDocument()
+
+    def end_element(self, name: Tuple[str, str], qname: str):
+        """End element notification receiver.
+
+        Args:
+            name: The qname as tuple
+            qname: The qualified name
+        """
+        self.handler.endElementNS(name, qname)
+
+    def set_characters(self, data: str):
+        """Characters notification receiver.
+
+        Args:
+            data: The characters data to write
+        """
+        self.handler.characters(data)
+
+    def end_prefix_mapping(self, prefix: str):
+        """End namespace prefix notification receiver.
+
+        Args:
+            prefix: The namespace prefix
+        """
+        self.handler.endPrefixMapping(prefix)
+
+    def start_element(self, name: Tuple[str, str], qname: str, attrs: Dict):
+        """Start element notification receiver.
+
+        Args:
+            name: The qname as tuple
+            qname: The qualified name
+            attrs: The attributes mapping
+        """
+        self.handler.startElementNS(name, qname, attrs)  # type: ignore
+
+    def start_prefix_mapping(self, prefix: Optional[str], uri: str):
+        """Start namespace prefix notification receiver.
+
+        Args:
+            prefix: The namespace prefix
+            uri: The namespace URI
+        """
+        self.handler.startPrefixMapping(prefix, uri)
+
+
+class XmlWriter(EventContentHandler, ABC):
+    """A consistency wrapper for sax content writers.
+
+    Args:
+        config: The serializer config instance
+        output: The writer output stream
+        ns_map: A user defined namespace prefix-URI map
+
+    Attributes:
+        handler: The content handler instance
+        in_tail: Specifies whether the text content has been written
+        tail: The current element tail content
+        attrs: The current element attributes
+        ns_context: The namespace context queue
+        pending_tag: The pending element namespace, name tuple
+        pending_prefixes: The pending element namespace prefixes
+    """
+
+    def __init__(self, config: SerializerConfig, output: TextIO, ns_map: Dict):
+        self.output = output
+        super().__init__(config, ns_map)
+
+    def start_document(self):
+        """Start document notification receiver.
+
+        Write the xml version and encoding, if the
+        configuration is enabled.
+        """
+        if self.config.xml_declaration:
+            self.output.write(f'<?xml version="{self.config.xml_version}"')
+            self.output.write(f' encoding="{self.config.encoding}"?>\n')
+
 
 @dataclass
 class EventGenerator:
     context: XmlContext = field(default_factory=XmlContext)
     config: SerializerConfig = field(default_factory=SerializerConfig)
 
     def generate(self, obj: Any) -> EventIterator:
```

### Comparing `xsdata-24.4/xsdata/formats/dataclass/serializers/writers/lxml.py` & `xsdata-24.5/xsdata/formats/dataclass/serializers/writers/lxml.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from typing import Iterator
 
 from lxml import etree
 from lxml.sax import ElementTreeContentHandler
 
-from xsdata.formats.dataclass.serializers.mixins import XmlWriter
+from xsdata.formats.dataclass.serializers.mixins import EventContentHandler, XmlWriter
 
 
 class LxmlEventWriter(XmlWriter):
     """Xml event writer based on `lxml.sax.ElementTreeContentHandler`.
 
-    The writer converts the events to an lxml tree which is
+    The writer converts the events to a lxml tree which is
     then converted to string.
 
     Args:
         config: The serializer config instance
         output: The output stream to write the result
         ns_map: A user defined namespace prefix-URI map
 
@@ -61,7 +61,38 @@
             xml_declaration=False,
         ).decode(self.config.encoding)
 
         self.output.write(xml)
 
         if self.config.indent:
             self.output.write("\n")
+
+
+class LxmlTreeBuilder(EventContentHandler):
+    def build_handler(self) -> ElementTreeContentHandler:
+        """Build the content handler instance.
+
+        Returns:
+            An element tree content handler instance.
+        """
+        return ElementTreeContentHandler()
+
+    def build(self, events: Iterator) -> etree.ElementTree:
+        """Feed the sax content handler with events.
+
+        Args:
+            events: An iterator of sax events
+
+        Raises:
+            XmlWriterError: On unknown events.
+
+        Returns:
+            The element tree instance.
+        """
+        self.write(events)
+
+        assert isinstance(self.handler, ElementTreeContentHandler)
+
+        if self.config.indent:
+            etree.indent(self.handler.etree, self.config.indent)
+
+        return self.handler.etree
```

### Comparing `xsdata-24.4/xsdata/formats/dataclass/serializers/writers/native.py` & `xsdata-24.5/xsdata/formats/dataclass/serializers/writers/native.py`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/xsdata/formats/dataclass/serializers/xml.py` & `xsdata-24.5/xsdata/formats/dataclass/serializers/xml.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,29 +8,29 @@
     Type,
 )
 
 from xsdata.formats.dataclass.serializers.mixins import (
     EventGenerator,
     XmlWriter,
 )
-from xsdata.formats.dataclass.serializers.writers import default_writer
+from xsdata.formats.dataclass.serializers.writers import DEFAULT_XML_WRITER
 from xsdata.utils import namespaces
 
 
 @dataclass
 class XmlSerializer(EventGenerator):
     """Xml serializer for data classes.
 
     Args:
         config: The serializer config instance
         context: The models context instance
         writer: The xml writer class
     """
 
-    writer: Type[XmlWriter] = field(default=default_writer())
+    writer: Type[XmlWriter] = field(default=DEFAULT_XML_WRITER)
 
     def render(self, obj: Any, ns_map: Optional[Dict] = None) -> str:
         """Serialize the input model instance to xml string.
 
         Args:
             obj: The input model instance to serialize
             ns_map: A user defined namespace prefix-URI map
```

### Comparing `xsdata-24.4/xsdata/formats/dataclass/templates/class.jinja2` & `xsdata-24.5/xsdata/formats/dataclass/templates/class.jinja2`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 {% set level = level|default(0) -%}
 {% set help | format_docstring(level + 1) %}
     {%- include "docstrings." + docstring_name + ".jinja2" -%}
 {% endset -%}
 {% set parent_namespace = obj.namespace if obj.namespace is not none else parent_namespace|default(None) -%}
-{% set parents = parents|default([obj.name]) -%}
 {% set class_name =  obj.name|class_name -%}
 {% set class_annotations =  obj | class_annotations(class_name) -%}
 {% set global_type = level == 0 and not obj.local_type -%}
 {% set local_name =  obj.meta_name or obj.name -%}
 {% set local_name = None if class_name == local_name or not global_type else local_name -%}
 {% set base_classes = obj | class_bases(class_name) | join(', ')-%}
 {% set post_meta_output = obj | post_meta_hook -%}
@@ -38,20 +37,19 @@
 {% elif obj.attrs|length == 0 and not help and not extra_output %}
     pass
 {%- endif -%}
 {%- if post_meta_output %}
 {{ post_meta_output|indent(4, first=True) }}
 {%- endif -%}
 {%- for attr in obj.attrs %}
-    {%- set field_typing = attr|field_type(parents) %}
-    {%- set field_definition = attr|field_definition(obj.ns_map, parent_namespace, parents) %}
+    {%- set field_typing = obj|field_type(attr) %}
+    {%- set field_definition = obj|field_definition(attr, parent_namespace) %}
     {{ attr.name|field_name(obj.name) }}: {{ field_typing }} = {{ field_definition }}
 {%- endfor -%}
 {%- for inner in obj.inner %}
     {%- set tpl = "enum.jinja2" if inner.is_enumeration else "class.jinja2" -%}
-    {%- set inner_parents = parents + [inner.name] -%}
     {%- filter indent(4) -%}
-        {%- with obj=inner, parents=inner_parents, level=(level + 1) -%}
+        {%- with obj=inner, level=(level + 1) -%}
             {% include tpl %}
         {%- endwith -%}
     {%- endfilter -%}
 {%- endfor -%}
```

### Comparing `xsdata-24.4/xsdata/formats/dataclass/templates/enum.jinja2` & `xsdata-24.5/xsdata/formats/dataclass/templates/enum.jinja2`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/xsdata/formats/dataclass/transports.py` & `xsdata-24.5/xsdata/formats/dataclass/transports.py`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/xsdata/formats/mixins.py` & `xsdata-24.5/xsdata/formats/mixins.py`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/xsdata/models/config.py` & `xsdata-24.5/xsdata/models/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -493,15 +493,15 @@
 
     class Meta:
         """Metadata options."""
 
         name = "Config"
         namespace = "http://pypi.org/project/xsdata"
 
-    version: str = attribute(init=False, default=__version__)
+    version: str = attribute(default=__version__)
     output: GeneratorOutput = element(default_factory=GeneratorOutput)
     conventions: GeneratorConventions = element(default_factory=GeneratorConventions)
     substitutions: GeneratorSubstitutions = element(
         default_factory=GeneratorSubstitutions
     )
     extensions: GeneratorExtensions = element(default_factory=GeneratorExtensions)
 
@@ -538,15 +538,17 @@
         parser = XmlParser(
             context=ctx,
             config=ParserConfig(
                 fail_on_unknown_properties=False,
                 fail_on_converter_warnings=True,
             ),
         )
-        return parser.from_path(path, cls)
+        cfg = parser.from_path(path, cls)
+        cfg.version = __version__
+        return cfg
 
     @classmethod
     def write(cls, output: TextIO, obj: "GeneratorConfig"):
         """Write the configuration to the output stream as xml."""
         ctx = XmlContext(
             element_name_generator=text.pascal_case,
             attribute_name_generator=text.camel_case,
```

### Comparing `xsdata-24.4/xsdata/models/datatype.py` & `xsdata-24.5/xsdata/models/datatype.py`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/xsdata/models/dtd.py` & `xsdata-24.5/xsdata/models/dtd.py`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/xsdata/models/enums.py` & `xsdata-24.5/xsdata/models/enums.py`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/xsdata/models/mixins.py` & `xsdata-24.5/xsdata/models/mixins.py`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/xsdata/models/wsdl.py` & `xsdata-24.5/xsdata/models/wsdl.py`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/xsdata/models/xsd.py` & `xsdata-24.5/xsdata/models/xsd.py`

 * *Files 0% similar despite different names*

```diff
@@ -958,50 +958,50 @@
 
 @dataclass
 class Import(AnnotationBase):
     """XSD Import model representation."""
 
     namespace: Optional[str] = attribute()
     schema_location: Optional[str] = attribute(name="schemaLocation")
-    location: Optional[str] = field(default=None, metadata={"type": "ignore"})
+    location: Optional[str] = field(default=None, metadata={"type": "Ignore"})
 
 
 @dataclass
 class Include(AnnotationBase):
     """XSD Include model representation."""
 
     schema_location: Optional[str] = attribute(name="schemaLocation")
-    location: Optional[str] = field(default=None, metadata={"type": "ignore"})
+    location: Optional[str] = field(default=None, metadata={"type": "Ignore"})
 
 
 @dataclass
 class Redefine(AnnotationBase):
     """XSD Redefine model representation."""
 
     schema_location: Optional[str] = attribute(name="schemaLocation")
     simple_types: Array[SimpleType] = array_element(name="simpleType")
     complex_types: Array[ComplexType] = array_element(name="complexType")
     groups: Array[Group] = array_element(name="group")
     attribute_groups: Array[AttributeGroup] = array_element(name="attributeGroup")
-    location: Optional[str] = field(default=None, metadata={"type": "ignore"})
+    location: Optional[str] = field(default=None, metadata={"type": "Ignore"})
 
 
 @dataclass
 class Override(AnnotationBase):
     """XSD Override model representation."""
 
     schema_location: Optional[str] = attribute(name="schemaLocation")
     simple_types: Array[SimpleType] = array_element(name="simpleType")
     complex_types: Array[ComplexType] = array_element(name="complexType")
     groups: Array[Group] = array_element(name="group")
     attribute_groups: Array[AttributeGroup] = array_element(name="attributeGroup")
     elements: Array[Element] = array_element(name="element")
     attributes: Array[Attribute] = array_element(name="attribute")
     notations: Array[Notation] = array_element(name="notation")
-    location: Optional[str] = field(default=None, metadata={"type": "ignore"})
+    location: Optional[str] = field(default=None, metadata={"type": "Ignore"})
 
 
 @dataclass
 class Schema(AnnotationBase):
     """XSD Schema model representation."""
 
     class Meta:
@@ -1036,15 +1036,15 @@
     simple_types: Array[SimpleType] = array_element(name="simpleType")
     complex_types: Array[ComplexType] = array_element(name="complexType")
     groups: Array[Group] = array_element(name="group")
     attribute_groups: Array[AttributeGroup] = array_element(name="attributeGroup")
     elements: Array[Element] = array_element(name="element")
     attributes: Array[Attribute] = array_element(name="attribute")
     notations: Array[Notation] = array_element(name="notation")
-    location: Optional[str] = field(default=None, metadata={"type": "ignore"})
+    location: Optional[str] = field(default=None, metadata={"type": "Ignore"})
 
     def included(self) -> Iterator[UnionType[Import, Include, Redefine, Override]]:
         """Yields an iterator of included resources."""
         yield from self.imports
 
         yield from self.includes
```

### Comparing `xsdata-24.4/xsdata/schemas/mathml3-common.xsd` & `xsdata-24.5/xsdata/schemas/mathml3-common.xsd`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/xsdata/schemas/mathml3-content.xsd` & `xsdata-24.5/xsdata/schemas/mathml3-content.xsd`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/xsdata/schemas/mathml3-presentation.xsd` & `xsdata-24.5/xsdata/schemas/mathml3-presentation.xsd`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/xsdata/schemas/mathml3-strict-content.xsd` & `xsdata-24.5/xsdata/schemas/mathml3-strict-content.xsd`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/xsdata/schemas/xlink.xsd` & `xsdata-24.5/xsdata/schemas/xlink.xsd`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/xsdata/schemas/xml.xsd` & `xsdata-24.5/xsdata/schemas/xml.xsd`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/xsdata/utils/click.py` & `xsdata-24.5/xsdata/utils/click.py`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/xsdata/utils/collections.py` & `xsdata-24.5/xsdata/utils/collections.py`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/xsdata/utils/dates.py` & `xsdata-24.5/xsdata/utils/dates.py`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/xsdata/utils/debug.py` & `xsdata-24.5/xsdata/utils/debug.py`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/xsdata/utils/downloader.py` & `xsdata-24.5/xsdata/utils/downloader.py`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/xsdata/utils/graphs.py` & `xsdata-24.5/xsdata/utils/graphs.py`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/xsdata/utils/namespaces.py` & `xsdata-24.5/xsdata/utils/namespaces.py`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/xsdata/utils/objects.py` & `xsdata-24.5/xsdata/utils/objects.py`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/xsdata/utils/package.py` & `xsdata-24.5/xsdata/utils/package.py`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/xsdata/utils/testing.py` & `xsdata-24.5/xsdata/utils/testing.py`

 * *Files identical despite different names*

### Comparing `xsdata-24.4/xsdata/utils/text.py` & `xsdata-24.5/xsdata/utils/text.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,14 +53,15 @@
     "pass",
     "raise",
     "return",
     "self",
     "str",
     "try",
     "type",
+    "validate",
     "while",
     "with",
     "yield",
 }
 
 is_reserved = stop_words.__contains__
```

### Comparing `xsdata-24.4/xsdata.egg-info/PKG-INFO` & `xsdata-24.5/xsdata.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xsdata
-Version: 24.4
+Version: 24.5
 Summary: Python XML Binding
 Author-email: Christodoulos Tsoulloftas <chris@komposta.net>
 License: MIT
 Project-URL: Homepage, https://github.com/tefra/xsdata
 Project-URL: Source, https://github.com/tefra/xsdata
 Project-URL: Documentation, https://xsdata.readthedocs.io/
 Project-URL: Changelog, https://xsdata.readthedocs.io/en/latest/changelog/
@@ -128,48 +128,26 @@
 - XML and JSON parser, serializer
 - PyCode serializer
 - Handlers and Writers based on lxml and native xml python
 - Support wildcard elements and attributes
 - Support xinclude statements and unknown properties
 - Customize behaviour through config
 
-## Changelog: 24.3.1 (2024-03-10)
-
-**Fixes**
-
-- Unnest class with circular reference
-  ([#974](https://github.com/tefra/xsdata/pull/974))
-
-## Changelog: 24.4 (2024-04-01)
+## Changelog: 24.5 (2024-05-07)
 
 **Features**
 
-- Add xml and lxml tree serializers ([#975](https://github.com/tefra/xsdata/pull/975))
-- Capture namespace prefixes in user dicts
-  ([#978](https://github.com/tefra/xsdata/pull/978))
-- Add cli option to generate wrapper fields
-  ([#982](https://github.com/tefra/xsdata/pull/982))
-- Support wrapper fields in JSON data bindings
-  ([#982](https://github.com/tefra/xsdata/pull/982))
-- Use abstract suffixes to resolve class name conflicts
-  ([#985](https://github.com/tefra/xsdata/pull/985))
-- Add the version number in the cli cache key
-  ([#990](https://github.com/tefra/xsdata/pull/990))
-- Use unicodedata.name for attrs with only special characters
-  ([#993](https://github.com/tefra/xsdata/pull/993))
-- Add src code excerpts on ruff errors
-  ([#996](https://github.com/tefra/xsdata/pull/996))
-- Detect circular imports and raise appropriate error
-  ([#999](https://github.com/tefra/xsdata/pull/999))
-- Add support for Python 3.13 ([#1001](https://github.com/tefra/xsdata/pull/1001))
-- Add cli debug messages with performance stats
+- Rewrite TreeSerializer, drop support for native python ElementTree
+  ([#1032](https://github.com/tefra/xsdata/pull/1032))
+- Validate fields fixed values ([#1013](https://github.com/tefra/xsdata/pull/1013))
+- Detect optional fields in dict mapper
+- Refactor typing annotations analyze process
+- Generate ForwardRef() instead of Type[]
 
 **Fixes**
 
-- Use deepcopy to clone codegen models
-  ([#980](https://github.com/tefra/xsdata/pull/980))
-- Generate type hints for compound fields with token elements
-  ([#997](https://github.com/tefra/xsdata/pull/997))
-- Protect prohibited attrs from turning into lists
-  ([#998](https://github.com/tefra/xsdata/pull/998))
-- Convert child attr to list when parent is list
-  ([#998](https://github.com/tefra/xsdata/pull/998))
+- Allow soap client config subclassing
+  ([#1010](https://github.com/tefra/xsdata/pull/1010))
+- Avoid recursive error on nested group references
+  ([#1016](https://github.com/tefra/xsdata/pull/1016))
+- Add warning for same module designation
+  ([#1018](https://github.com/tefra/xsdata/pull/1018))
```

### Comparing `xsdata-24.4/xsdata.egg-info/SOURCES.txt` & `xsdata-24.5/xsdata.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -191,14 +191,20 @@
 tests/formats/dataclass/test_compat.py
 tests/formats/dataclass/test_context.py
 tests/formats/dataclass/test_elements.py
 tests/formats/dataclass/test_filters.py
 tests/formats/dataclass/test_generator.py
 tests/formats/dataclass/test_transport.py
 tests/formats/dataclass/test_typing.py
+tests/formats/dataclass/cases/__init__.py
+tests/formats/dataclass/cases/attribute.py
+tests/formats/dataclass/cases/attributes.py
+tests/formats/dataclass/cases/element.py
+tests/formats/dataclass/cases/elements.py
+tests/formats/dataclass/cases/wildcard.py
 tests/formats/dataclass/models/__init__.py
 tests/formats/dataclass/models/test_builders.py
 tests/formats/dataclass/parsers/__init__.py
 tests/formats/dataclass/parsers/test_dict.py
 tests/formats/dataclass/parsers/test_json.py
 tests/formats/dataclass/parsers/test_mixins.py
 tests/formats/dataclass/parsers/test_node.py
@@ -219,18 +225,14 @@
 tests/formats/dataclass/serializers/__init__.py
 tests/formats/dataclass/serializers/test_code.py
 tests/formats/dataclass/serializers/test_config.py
 tests/formats/dataclass/serializers/test_dict.py
 tests/formats/dataclass/serializers/test_json.py
 tests/formats/dataclass/serializers/test_mixins.py
 tests/formats/dataclass/serializers/test_xml.py
-tests/formats/dataclass/serializers/tree/__init__.py
-tests/formats/dataclass/serializers/tree/test_lxml.py
-tests/formats/dataclass/serializers/tree/test_mixins.py
-tests/formats/dataclass/serializers/tree/test_native.py
 tests/formats/dataclass/serializers/writers/__init__.py
 tests/formats/dataclass/serializers/writers/test_lxml.py
 tests/formats/dataclass/serializers/writers/test_native.py
 tests/integration/__init__.py
 tests/integration/test_annotations.py
 tests/integration/test_artists.py
 tests/integration/test_books.py
@@ -387,19 +389,16 @@
 xsdata/formats/dataclass/parsers/nodes/wrapper.py
 xsdata/formats/dataclass/serializers/__init__.py
 xsdata/formats/dataclass/serializers/code.py
 xsdata/formats/dataclass/serializers/config.py
 xsdata/formats/dataclass/serializers/dict.py
 xsdata/formats/dataclass/serializers/json.py
 xsdata/formats/dataclass/serializers/mixins.py
+xsdata/formats/dataclass/serializers/tree.py
 xsdata/formats/dataclass/serializers/xml.py
-xsdata/formats/dataclass/serializers/tree/__init__.py
-xsdata/formats/dataclass/serializers/tree/lxml.py
-xsdata/formats/dataclass/serializers/tree/mixins.py
-xsdata/formats/dataclass/serializers/tree/native.py
 xsdata/formats/dataclass/serializers/writers/__init__.py
 xsdata/formats/dataclass/serializers/writers/lxml.py
 xsdata/formats/dataclass/serializers/writers/native.py
 xsdata/formats/dataclass/templates/class.jinja2
 xsdata/formats/dataclass/templates/docstrings.accessible.jinja2
 xsdata/formats/dataclass/templates/docstrings.blank.jinja2
 xsdata/formats/dataclass/templates/docstrings.google.jinja2
```

