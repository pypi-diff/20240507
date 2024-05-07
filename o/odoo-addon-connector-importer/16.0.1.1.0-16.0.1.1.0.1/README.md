# Comparing `tmp/odoo_addon_connector_importer-16.0.1.1.0-py3-none-any.whl.zip` & `tmp/odoo_addon_connector_importer-16.0.1.1.0.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,78 +1,79 @@
-Zip file size: 104989 bytes, number of entries: 76
--rw-r--r--  2.0 unx     4426 b- defN 23-Oct-16 09:59 odoo/addons/connector_importer/README.rst
--rw-r--r--  2.0 unx       72 b- defN 23-Oct-16 09:59 odoo/addons/connector_importer/__init__.py
--rw-r--r--  2.0 unx     1033 b- defN 23-Oct-16 09:59 odoo/addons/connector_importer/__manifest__.py
--rw-r--r--  2.0 unx      985 b- defN 23-Oct-16 09:59 odoo/addons/connector_importer/events.py
--rw-r--r--  2.0 unx      757 b- defN 23-Oct-16 09:59 odoo/addons/connector_importer/log.py
--rw-r--r--  2.0 unx     1059 b- defN 23-Oct-16 09:59 odoo/addons/connector_importer/menuitems.xml
--rw-r--r--  2.0 unx      251 b- defN 23-Oct-16 09:59 odoo/addons/connector_importer/components/__init__.py
--rw-r--r--  2.0 unx      566 b- defN 23-Oct-16 09:59 odoo/addons/connector_importer/components/automapper.py
--rw-r--r--  2.0 unx      332 b- defN 23-Oct-16 09:59 odoo/addons/connector_importer/components/base.py
--rw-r--r--  2.0 unx     7078 b- defN 23-Oct-16 09:59 odoo/addons/connector_importer/components/dynamicmapper.py
--rw-r--r--  2.0 unx    15898 b- defN 23-Oct-16 09:59 odoo/addons/connector_importer/components/importer.py
--rw-r--r--  2.0 unx     6589 b- defN 23-Oct-16 09:59 odoo/addons/connector_importer/components/importer_csv_std.py
--rw-r--r--  2.0 unx     3356 b- defN 23-Oct-16 09:59 odoo/addons/connector_importer/components/listeners.py
--rw-r--r--  2.0 unx     4380 b- defN 23-Oct-16 09:59 odoo/addons/connector_importer/components/mapper.py
--rw-r--r--  2.0 unx     9335 b- defN 23-Oct-16 09:59 odoo/addons/connector_importer/components/odoorecord.py
--rw-r--r--  2.0 unx     1436 b- defN 23-Oct-16 09:59 odoo/addons/connector_importer/components/odoorecord_csv_std.py
--rw-r--r--  2.0 unx     4204 b- defN 23-Oct-16 09:59 odoo/addons/connector_importer/components/tracker.py
--rw-r--r--  2.0 unx       19 b- defN 23-Oct-16 09:59 odoo/addons/connector_importer/controllers/__init__.py
--rw-r--r--  2.0 unx      788 b- defN 23-Oct-16 09:59 odoo/addons/connector_importer/controllers/main.py
--rw-r--r--  2.0 unx      678 b- defN 23-Oct-16 09:59 odoo/addons/connector_importer/data/ir_cron.xml
--rw-r--r--  2.0 unx      827 b- defN 23-Oct-16 09:59 odoo/addons/connector_importer/data/queue_job_function_data.xml
--rw-r--r--  2.0 unx    31893 b- defN 23-Oct-16 09:59 odoo/addons/connector_importer/i18n/connector_importer.pot
--rw-r--r--  2.0 unx      187 b- defN 23-Oct-16 09:59 odoo/addons/connector_importer/models/__init__.py
--rw-r--r--  2.0 unx     5054 b- defN 23-Oct-16 09:59 odoo/addons/connector_importer/models/backend.py
--rw-r--r--  2.0 unx     2499 b- defN 23-Oct-16 09:59 odoo/addons/connector_importer/models/cron_mixin.py
--rw-r--r--  2.0 unx     4377 b- defN 23-Oct-16 09:59 odoo/addons/connector_importer/models/import_type.py
--rw-r--r--  2.0 unx      903 b- defN 23-Oct-16 09:59 odoo/addons/connector_importer/models/job_mixin.py
--rw-r--r--  2.0 unx     4438 b- defN 23-Oct-16 09:59 odoo/addons/connector_importer/models/record.py
--rw-r--r--  2.0 unx    14029 b- defN 23-Oct-16 09:59 odoo/addons/connector_importer/models/recordset.py
--rw-r--r--  2.0 unx     8955 b- defN 23-Oct-16 09:59 odoo/addons/connector_importer/models/reporter.py
--rw-r--r--  2.0 unx       88 b- defN 23-Oct-16 09:59 odoo/addons/connector_importer/models/sources/__init__.py
--rw-r--r--  2.0 unx     2409 b- defN 23-Oct-16 09:59 odoo/addons/connector_importer/models/sources/source_consumer_mixin.py
--rw-r--r--  2.0 unx     4005 b- defN 23-Oct-16 09:59 odoo/addons/connector_importer/models/sources/source_csv.py
--rw-r--r--  2.0 unx     4192 b- defN 23-Oct-16 09:59 odoo/addons/connector_importer/models/sources/source_mixin.py
--rw-r--r--  2.0 unx      184 b- defN 23-Oct-16 09:59 odoo/addons/connector_importer/readme/CONTRIBUTORS.rst
--rw-r--r--  2.0 unx      118 b- defN 23-Oct-16 09:59 odoo/addons/connector_importer/readme/DESCRIPTION.rst
--rw-r--r--  2.0 unx     1027 b- defN 23-Oct-16 09:59 odoo/addons/connector_importer/readme/ROADMAP.rst
--rw-r--r--  2.0 unx     1402 b- defN 23-Oct-16 09:59 odoo/addons/connector_importer/security/ir.model.access.csv
--rw-r--r--  2.0 unx      647 b- defN 23-Oct-16 09:59 odoo/addons/connector_importer/security/security.xml
--rw-r--r--  2.0 unx     7981 b- defN 23-Oct-16 09:59 odoo/addons/connector_importer/static/description/icon.png
--rw-r--r--  2.0 unx     3946 b- defN 23-Oct-16 09:59 odoo/addons/connector_importer/static/description/icon.svg
--rw-r--r--  2.0 unx    14046 b- defN 23-Oct-16 09:59 odoo/addons/connector_importer/static/description/index.html
--rw-r--r--  2.0 unx      379 b- defN 23-Oct-16 09:59 odoo/addons/connector_importer/tests/__init__.py
--rw-r--r--  2.0 unx     3341 b- defN 23-Oct-16 09:59 odoo/addons/connector_importer/tests/common.py
--rw-r--r--  2.0 unx     1995 b- defN 23-Oct-16 09:59 odoo/addons/connector_importer/tests/fake_components.py
--rw-r--r--  2.0 unx     1181 b- defN 23-Oct-16 09:59 odoo/addons/connector_importer/tests/fake_models.py
--rw-r--r--  2.0 unx     1545 b- defN 23-Oct-16 09:59 odoo/addons/connector_importer/tests/test_backend.py
--rw-r--r--  2.0 unx     1507 b- defN 23-Oct-16 09:59 odoo/addons/connector_importer/tests/test_cron.py
--rw-r--r--  2.0 unx     7335 b- defN 23-Oct-16 09:59 odoo/addons/connector_importer/tests/test_event_listeners.py
--rw-r--r--  2.0 unx     4047 b- defN 23-Oct-16 09:59 odoo/addons/connector_importer/tests/test_import_type.py
--rw-r--r--  2.0 unx     6766 b- defN 23-Oct-16 09:59 odoo/addons/connector_importer/tests/test_mapper.py
--rw-r--r--  2.0 unx     2734 b- defN 23-Oct-16 09:59 odoo/addons/connector_importer/tests/test_record_handler.py
--rw-r--r--  2.0 unx     4793 b- defN 23-Oct-16 09:59 odoo/addons/connector_importer/tests/test_record_importer.py
--rw-r--r--  2.0 unx     4825 b- defN 23-Oct-16 09:59 odoo/addons/connector_importer/tests/test_record_importer_basic.py
--rw-r--r--  2.0 unx     1994 b- defN 23-Oct-16 09:59 odoo/addons/connector_importer/tests/test_record_importer_xmlid.py
--rw-r--r--  2.0 unx     3762 b- defN 23-Oct-16 09:59 odoo/addons/connector_importer/tests/test_recordset.py
--rw-r--r--  2.0 unx     3498 b- defN 23-Oct-16 09:59 odoo/addons/connector_importer/tests/test_recordset_importer.py
--rw-r--r--  2.0 unx     2920 b- defN 23-Oct-16 09:59 odoo/addons/connector_importer/tests/test_source.py
--rw-r--r--  2.0 unx     2997 b- defN 23-Oct-16 09:59 odoo/addons/connector_importer/tests/test_source_csv.py
--rw-r--r--  2.0 unx       85 b- defN 23-Oct-16 09:59 odoo/addons/connector_importer/tests/fixtures/csv_source_test1.csv
--rw-r--r--  2.0 unx        0 b- defN 23-Oct-16 09:59 odoo/addons/connector_importer/utils/__init__.py
--rw-r--r--  2.0 unx     4114 b- defN 23-Oct-16 09:59 odoo/addons/connector_importer/utils/import_utils.py
--rw-r--r--  2.0 unx    11401 b- defN 23-Oct-16 09:59 odoo/addons/connector_importer/utils/mapper_utils.py
--rw-r--r--  2.0 unx     1982 b- defN 23-Oct-16 09:59 odoo/addons/connector_importer/utils/misc.py
--rw-r--r--  2.0 unx     4254 b- defN 23-Oct-16 09:59 odoo/addons/connector_importer/utils/report_html.py
--rw-r--r--  2.0 unx     6214 b- defN 23-Oct-16 09:59 odoo/addons/connector_importer/views/backend_views.xml
--rw-r--r--  2.0 unx     9503 b- defN 23-Oct-16 09:59 odoo/addons/connector_importer/views/docs_template.xml
--rw-r--r--  2.0 unx     1637 b- defN 23-Oct-16 09:59 odoo/addons/connector_importer/views/import_type_views.xml
--rw-r--r--  2.0 unx     7329 b- defN 23-Oct-16 09:59 odoo/addons/connector_importer/views/recordset_views.xml
--rw-r--r--  2.0 unx     2099 b- defN 23-Oct-16 09:59 odoo/addons/connector_importer/views/report_template.xml
--rw-r--r--  2.0 unx      576 b- defN 23-Oct-16 09:59 odoo/addons/connector_importer/views/source_config_template.xml
--rw-r--r--  2.0 unx     2616 b- defN 23-Oct-16 09:59 odoo/addons/connector_importer/views/source_views.xml
--rw-r--r--  2.0 unx     5165 b- defN 23-Oct-16 09:59 odoo_addon_connector_importer-16.0.1.1.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Oct-16 09:59 odoo_addon_connector_importer-16.0.1.1.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        5 b- defN 23-Oct-16 09:59 odoo_addon_connector_importer-16.0.1.1.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     8349 b- defN 23-Oct-16 09:59 odoo_addon_connector_importer-16.0.1.1.0.dist-info/RECORD
-76 files, 297489 bytes uncompressed, 90997 bytes compressed:  69.4%
+Zip file size: 109097 bytes, number of entries: 77
+-rw-r--r--  2.0 unx     4426 b- defN 24-May-07 03:23 odoo/addons/connector_importer/README.rst
+-rw-r--r--  2.0 unx       72 b- defN 24-May-07 03:23 odoo/addons/connector_importer/__init__.py
+-rw-r--r--  2.0 unx     1033 b- defN 24-May-07 03:23 odoo/addons/connector_importer/__manifest__.py
+-rw-r--r--  2.0 unx      985 b- defN 24-May-07 03:23 odoo/addons/connector_importer/events.py
+-rw-r--r--  2.0 unx      757 b- defN 24-May-07 03:23 odoo/addons/connector_importer/log.py
+-rw-r--r--  2.0 unx     1059 b- defN 24-May-07 03:23 odoo/addons/connector_importer/menuitems.xml
+-rw-r--r--  2.0 unx      251 b- defN 24-May-07 03:23 odoo/addons/connector_importer/components/__init__.py
+-rw-r--r--  2.0 unx      566 b- defN 24-May-07 03:23 odoo/addons/connector_importer/components/automapper.py
+-rw-r--r--  2.0 unx      332 b- defN 24-May-07 03:23 odoo/addons/connector_importer/components/base.py
+-rw-r--r--  2.0 unx     7078 b- defN 24-May-07 03:23 odoo/addons/connector_importer/components/dynamicmapper.py
+-rw-r--r--  2.0 unx    15898 b- defN 24-May-07 03:23 odoo/addons/connector_importer/components/importer.py
+-rw-r--r--  2.0 unx     6589 b- defN 24-May-07 03:23 odoo/addons/connector_importer/components/importer_csv_std.py
+-rw-r--r--  2.0 unx     3356 b- defN 24-May-07 03:23 odoo/addons/connector_importer/components/listeners.py
+-rw-r--r--  2.0 unx     4380 b- defN 24-May-07 03:23 odoo/addons/connector_importer/components/mapper.py
+-rw-r--r--  2.0 unx     9335 b- defN 24-May-07 03:23 odoo/addons/connector_importer/components/odoorecord.py
+-rw-r--r--  2.0 unx     1436 b- defN 24-May-07 03:23 odoo/addons/connector_importer/components/odoorecord_csv_std.py
+-rw-r--r--  2.0 unx     4204 b- defN 24-May-07 03:23 odoo/addons/connector_importer/components/tracker.py
+-rw-r--r--  2.0 unx       19 b- defN 24-May-07 03:23 odoo/addons/connector_importer/controllers/__init__.py
+-rw-r--r--  2.0 unx      788 b- defN 24-May-07 03:23 odoo/addons/connector_importer/controllers/main.py
+-rw-r--r--  2.0 unx      678 b- defN 24-May-07 03:23 odoo/addons/connector_importer/data/ir_cron.xml
+-rw-r--r--  2.0 unx      827 b- defN 24-May-07 03:23 odoo/addons/connector_importer/data/queue_job_function_data.xml
+-rw-r--r--  2.0 unx    31893 b- defN 24-May-07 03:23 odoo/addons/connector_importer/i18n/connector_importer.pot
+-rw-r--r--  2.0 unx    31963 b- defN 24-May-07 03:23 odoo/addons/connector_importer/i18n/it.po
+-rw-r--r--  2.0 unx      187 b- defN 24-May-07 03:23 odoo/addons/connector_importer/models/__init__.py
+-rw-r--r--  2.0 unx     5054 b- defN 24-May-07 03:23 odoo/addons/connector_importer/models/backend.py
+-rw-r--r--  2.0 unx     2499 b- defN 24-May-07 03:23 odoo/addons/connector_importer/models/cron_mixin.py
+-rw-r--r--  2.0 unx     4377 b- defN 24-May-07 03:23 odoo/addons/connector_importer/models/import_type.py
+-rw-r--r--  2.0 unx      903 b- defN 24-May-07 03:23 odoo/addons/connector_importer/models/job_mixin.py
+-rw-r--r--  2.0 unx     4438 b- defN 24-May-07 03:23 odoo/addons/connector_importer/models/record.py
+-rw-r--r--  2.0 unx    14029 b- defN 24-May-07 03:23 odoo/addons/connector_importer/models/recordset.py
+-rw-r--r--  2.0 unx     8955 b- defN 24-May-07 03:23 odoo/addons/connector_importer/models/reporter.py
+-rw-r--r--  2.0 unx       88 b- defN 24-May-07 03:23 odoo/addons/connector_importer/models/sources/__init__.py
+-rw-r--r--  2.0 unx     2409 b- defN 24-May-07 03:23 odoo/addons/connector_importer/models/sources/source_consumer_mixin.py
+-rw-r--r--  2.0 unx     4005 b- defN 24-May-07 03:23 odoo/addons/connector_importer/models/sources/source_csv.py
+-rw-r--r--  2.0 unx     4192 b- defN 24-May-07 03:23 odoo/addons/connector_importer/models/sources/source_mixin.py
+-rw-r--r--  2.0 unx      184 b- defN 24-May-07 03:23 odoo/addons/connector_importer/readme/CONTRIBUTORS.rst
+-rw-r--r--  2.0 unx      118 b- defN 24-May-07 03:23 odoo/addons/connector_importer/readme/DESCRIPTION.rst
+-rw-r--r--  2.0 unx     1027 b- defN 24-May-07 03:23 odoo/addons/connector_importer/readme/ROADMAP.rst
+-rw-r--r--  2.0 unx     1402 b- defN 24-May-07 03:23 odoo/addons/connector_importer/security/ir.model.access.csv
+-rw-r--r--  2.0 unx      647 b- defN 24-May-07 03:23 odoo/addons/connector_importer/security/security.xml
+-rw-r--r--  2.0 unx     7981 b- defN 24-May-07 03:23 odoo/addons/connector_importer/static/description/icon.png
+-rw-r--r--  2.0 unx     3946 b- defN 24-May-07 03:23 odoo/addons/connector_importer/static/description/icon.svg
+-rw-r--r--  2.0 unx    14046 b- defN 24-May-07 03:23 odoo/addons/connector_importer/static/description/index.html
+-rw-r--r--  2.0 unx      379 b- defN 24-May-07 03:23 odoo/addons/connector_importer/tests/__init__.py
+-rw-r--r--  2.0 unx     3341 b- defN 24-May-07 03:23 odoo/addons/connector_importer/tests/common.py
+-rw-r--r--  2.0 unx     1995 b- defN 24-May-07 03:23 odoo/addons/connector_importer/tests/fake_components.py
+-rw-r--r--  2.0 unx     1181 b- defN 24-May-07 03:23 odoo/addons/connector_importer/tests/fake_models.py
+-rw-r--r--  2.0 unx     1545 b- defN 24-May-07 03:23 odoo/addons/connector_importer/tests/test_backend.py
+-rw-r--r--  2.0 unx     1507 b- defN 24-May-07 03:23 odoo/addons/connector_importer/tests/test_cron.py
+-rw-r--r--  2.0 unx     7335 b- defN 24-May-07 03:23 odoo/addons/connector_importer/tests/test_event_listeners.py
+-rw-r--r--  2.0 unx     4047 b- defN 24-May-07 03:23 odoo/addons/connector_importer/tests/test_import_type.py
+-rw-r--r--  2.0 unx     6766 b- defN 24-May-07 03:23 odoo/addons/connector_importer/tests/test_mapper.py
+-rw-r--r--  2.0 unx     2734 b- defN 24-May-07 03:23 odoo/addons/connector_importer/tests/test_record_handler.py
+-rw-r--r--  2.0 unx     4793 b- defN 24-May-07 03:23 odoo/addons/connector_importer/tests/test_record_importer.py
+-rw-r--r--  2.0 unx     4825 b- defN 24-May-07 03:23 odoo/addons/connector_importer/tests/test_record_importer_basic.py
+-rw-r--r--  2.0 unx     1994 b- defN 24-May-07 03:23 odoo/addons/connector_importer/tests/test_record_importer_xmlid.py
+-rw-r--r--  2.0 unx     3762 b- defN 24-May-07 03:23 odoo/addons/connector_importer/tests/test_recordset.py
+-rw-r--r--  2.0 unx     3498 b- defN 24-May-07 03:23 odoo/addons/connector_importer/tests/test_recordset_importer.py
+-rw-r--r--  2.0 unx     2920 b- defN 24-May-07 03:23 odoo/addons/connector_importer/tests/test_source.py
+-rw-r--r--  2.0 unx     2997 b- defN 24-May-07 03:23 odoo/addons/connector_importer/tests/test_source_csv.py
+-rw-r--r--  2.0 unx       85 b- defN 24-May-07 03:23 odoo/addons/connector_importer/tests/fixtures/csv_source_test1.csv
+-rw-r--r--  2.0 unx        0 b- defN 24-May-07 03:23 odoo/addons/connector_importer/utils/__init__.py
+-rw-r--r--  2.0 unx     4114 b- defN 24-May-07 03:23 odoo/addons/connector_importer/utils/import_utils.py
+-rw-r--r--  2.0 unx    11401 b- defN 24-May-07 03:23 odoo/addons/connector_importer/utils/mapper_utils.py
+-rw-r--r--  2.0 unx     1982 b- defN 24-May-07 03:23 odoo/addons/connector_importer/utils/misc.py
+-rw-r--r--  2.0 unx     4254 b- defN 24-May-07 03:23 odoo/addons/connector_importer/utils/report_html.py
+-rw-r--r--  2.0 unx     6214 b- defN 24-May-07 03:23 odoo/addons/connector_importer/views/backend_views.xml
+-rw-r--r--  2.0 unx     9503 b- defN 24-May-07 03:23 odoo/addons/connector_importer/views/docs_template.xml
+-rw-r--r--  2.0 unx     1637 b- defN 24-May-07 03:23 odoo/addons/connector_importer/views/import_type_views.xml
+-rw-r--r--  2.0 unx     7329 b- defN 24-May-07 03:23 odoo/addons/connector_importer/views/recordset_views.xml
+-rw-r--r--  2.0 unx     2099 b- defN 24-May-07 03:23 odoo/addons/connector_importer/views/report_template.xml
+-rw-r--r--  2.0 unx      576 b- defN 24-May-07 03:23 odoo/addons/connector_importer/views/source_config_template.xml
+-rw-r--r--  2.0 unx     2616 b- defN 24-May-07 03:23 odoo/addons/connector_importer/views/source_views.xml
+-rw-r--r--  2.0 unx     5167 b- defN 24-May-07 03:24 odoo_addon_connector_importer-16.0.1.1.0.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-07 03:24 odoo_addon_connector_importer-16.0.1.1.0.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx        5 b- defN 24-May-07 03:24 odoo_addon_connector_importer-16.0.1.1.0.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     8456 b- defN 24-May-07 03:24 odoo_addon_connector_importer-16.0.1.1.0.1.dist-info/RECORD
+77 files, 329561 bytes uncompressed, 94931 bytes compressed:  71.2%
```

## zipnote {}

```diff
@@ -60,14 +60,17 @@
 
 Filename: odoo/addons/connector_importer/data/queue_job_function_data.xml
 Comment: 
 
 Filename: odoo/addons/connector_importer/i18n/connector_importer.pot
 Comment: 
 
+Filename: odoo/addons/connector_importer/i18n/it.po
+Comment: 
+
 Filename: odoo/addons/connector_importer/models/__init__.py
 Comment: 
 
 Filename: odoo/addons/connector_importer/models/backend.py
 Comment: 
 
 Filename: odoo/addons/connector_importer/models/cron_mixin.py
@@ -210,20 +213,20 @@
 
 Filename: odoo/addons/connector_importer/views/source_config_template.xml
 Comment: 
 
 Filename: odoo/addons/connector_importer/views/source_views.xml
 Comment: 
 
-Filename: odoo_addon_connector_importer-16.0.1.1.0.dist-info/METADATA
+Filename: odoo_addon_connector_importer-16.0.1.1.0.1.dist-info/METADATA
 Comment: 
 
-Filename: odoo_addon_connector_importer-16.0.1.1.0.dist-info/WHEEL
+Filename: odoo_addon_connector_importer-16.0.1.1.0.1.dist-info/WHEEL
 Comment: 
 
-Filename: odoo_addon_connector_importer-16.0.1.1.0.dist-info/top_level.txt
+Filename: odoo_addon_connector_importer-16.0.1.1.0.1.dist-info/top_level.txt
 Comment: 
 
-Filename: odoo_addon_connector_importer-16.0.1.1.0.dist-info/RECORD
+Filename: odoo_addon_connector_importer-16.0.1.1.0.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `odoo_addon_connector_importer-16.0.1.1.0.dist-info/METADATA` & `odoo_addon_connector_importer-16.0.1.1.0.1.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odoo-addon-connector-importer
-Version: 16.0.1.1.0
+Version: 16.0.1.1.0.1
 Summary: This module takes care of import sessions.
 Home-page: https://github.com/OCA/connector-interfaces
 Author: Camptocamp, Odoo Community Association (OCA)
 Author-email: support@odoo-community.org
 License: AGPL-3
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
```

## Comparing `odoo_addon_connector_importer-16.0.1.1.0.dist-info/RECORD` & `odoo_addon_connector_importer-16.0.1.1.0.1.dist-info/RECORD`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 odoo/addons/connector_importer/components/odoorecord_csv_std.py,sha256=2a6suU7GEcbfJNYqpmwB0ABJVj0pTiuATAKQP0M02Cs,1436
 odoo/addons/connector_importer/components/tracker.py,sha256=LVATxle9Cme4mcs37Y0pdJqExRFnK-QrzeFjws1I2zU,4204
 odoo/addons/connector_importer/controllers/__init__.py,sha256=4KFqEP2QHFbPN66eQJMdGsmNz2v7ywWv_FR1pW_kkLk,19
 odoo/addons/connector_importer/controllers/main.py,sha256=nhoRxonfXSGRgiU4b3ZG_-VnOXx40fZbpgZucdvVilU,788
 odoo/addons/connector_importer/data/ir_cron.xml,sha256=rOMNu38Eyf6oP_wZ_RrGaLYAw2ppps1LeVAn3MRCvdY,678
 odoo/addons/connector_importer/data/queue_job_function_data.xml,sha256=2NLyI0tIRNqHCK6LzLR2HxqlJbP_IkXhdSWBRckEcrA,827
 odoo/addons/connector_importer/i18n/connector_importer.pot,sha256=6mrySa_6kcG24QEG0kRnsVxApckSEX9xzsse3JUQ0yw,31893
+odoo/addons/connector_importer/i18n/it.po,sha256=hSoiE3oW-C0n3zvJjgQFFWCWn-0XxzpVzBZmGDIgXFI,31963
 odoo/addons/connector_importer/models/__init__.py,sha256=orxP9e6AoeA-14goPFDfkc7-HVbytsRaqtOHoCa0Na0,187
 odoo/addons/connector_importer/models/backend.py,sha256=GgtrK3ZogOVHZO6SBVPVoTXpZAafUh_faoi1YVNXYAE,5054
 odoo/addons/connector_importer/models/cron_mixin.py,sha256=q6WFTHSxazjyaiNmP3ykgz_MN-BiWSZ34FdsMTxb7pc,2499
 odoo/addons/connector_importer/models/import_type.py,sha256=nZ4DhJt4kD8kUz0AvazW_ZNwzi49-JByx0ZTbZOX8Gk,4377
 odoo/addons/connector_importer/models/job_mixin.py,sha256=hthk1PLNsUoazxqivzYGrSZ5fT8EqK3Ekj8zUNFftE0,903
 odoo/addons/connector_importer/models/record.py,sha256=CP9AYPwTf6f3ZXaZUzqU-Gbdxh0__QsRHFtR2ogah5k,4438
 odoo/addons/connector_importer/models/recordset.py,sha256=94_feDhDVmh3BZtrFVYR-FfELPMpMv4hOlvPd6u4t6o,14029
@@ -66,11 +67,11 @@
 odoo/addons/connector_importer/views/backend_views.xml,sha256=JbR2TZlFSYPJFeVI9Fo96NUBrRChYnypDmT2pGzfXWw,6214
 odoo/addons/connector_importer/views/docs_template.xml,sha256=QHQgJtlEBqulmLzpulpHiAGSnHmkEYds-hGsf55AOmw,9503
 odoo/addons/connector_importer/views/import_type_views.xml,sha256=hklf5eaJ0NVGJDr3-tDr-ZXJy3I4IbTHoUKOsahdeHU,1637
 odoo/addons/connector_importer/views/recordset_views.xml,sha256=00qugBSK24DTjKTLMiaHLanDxcBv8nmw45o9_L_zIC4,7329
 odoo/addons/connector_importer/views/report_template.xml,sha256=DLYJgdxWw2FoH-1IFaKqQ5Vpl_J7wEzryPonpTGUzxc,2099
 odoo/addons/connector_importer/views/source_config_template.xml,sha256=LzIiidOvDNBRQV_5byrSQK6gyVDxcbVr4rlnxLTkKgw,576
 odoo/addons/connector_importer/views/source_views.xml,sha256=-8V2OP0V2Ier1ulc8L9mhY7mp104HkbVHGJj64e7Kkc,2616
-odoo_addon_connector_importer-16.0.1.1.0.dist-info/METADATA,sha256=kg8c6gM9hbymE0UxqPfT6woHwkE-JXhAOKhfaDXBrGY,5165
-odoo_addon_connector_importer-16.0.1.1.0.dist-info/WHEEL,sha256=yQN5g4mg4AybRjkgi-9yy4iQEFibGQmlz78Pik5Or-A,92
-odoo_addon_connector_importer-16.0.1.1.0.dist-info/top_level.txt,sha256=qBj40grFkGOfDZ2WDSw3y1RnDlgG0u8rP8pvGNdbz4w,5
-odoo_addon_connector_importer-16.0.1.1.0.dist-info/RECORD,,
+odoo_addon_connector_importer-16.0.1.1.0.1.dist-info/METADATA,sha256=Q73nhyRt91N_w9t0yPAE_rSTAqlRDxeXhLeYXjGM9YM,5167
+odoo_addon_connector_importer-16.0.1.1.0.1.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+odoo_addon_connector_importer-16.0.1.1.0.1.dist-info/top_level.txt,sha256=qBj40grFkGOfDZ2WDSw3y1RnDlgG0u8rP8pvGNdbz4w,5
+odoo_addon_connector_importer-16.0.1.1.0.1.dist-info/RECORD,,
```

