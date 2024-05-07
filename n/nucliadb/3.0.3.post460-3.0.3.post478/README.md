# Comparing `tmp/nucliadb-3.0.3.post460-py3-none-any.whl.zip` & `tmp/nucliadb-3.0.3.post478-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,457 +1,455 @@
-Zip file size: 752092 bytes, number of entries: 455
--rw-r--r--  2.0 unx     1135 b- defN 24-Apr-29 09:40 migrations/0001_bootstrap.py
--rw-r--r--  2.0 unx     1177 b- defN 24-Apr-29 09:40 migrations/0002_rollover_shards.py
--rw-r--r--  2.0 unx     2436 b- defN 24-Apr-29 09:40 migrations/0003_allfields_key.py
--rw-r--r--  2.0 unx     1177 b- defN 24-Apr-29 09:40 migrations/0004_rollover_shards.py
--rw-r--r--  2.0 unx     1177 b- defN 24-Apr-29 09:40 migrations/0005_rollover_shards.py
--rw-r--r--  2.0 unx     1024 b- defN 24-Apr-29 09:40 migrations/0006_rollover_shards.py
--rw-r--r--  2.0 unx     1301 b- defN 24-Apr-29 09:40 migrations/0008_cleanup_leftover_rollover_metadata.py
--rw-r--r--  2.0 unx     1378 b- defN 24-Apr-29 09:40 migrations/0009_upgrade_relations_and_texts_to_v2.py
--rw-r--r--  2.0 unx     1610 b- defN 24-Apr-29 09:40 migrations/0010_fix_corrupt_indexes.py
--rw-r--r--  2.0 unx     1843 b- defN 24-Apr-29 09:40 migrations/0011_materialize_labelset_ids.py
--rw-r--r--  2.0 unx     1443 b- defN 24-Apr-29 09:40 migrations/0012_rollover_shards.py
--rw-r--r--  2.0 unx     1024 b- defN 24-Apr-29 09:40 migrations/0013_rollover_shards.py
--rw-r--r--  2.0 unx     1382 b- defN 24-Apr-29 09:40 migrations/0014_rollover_shards.py
--rw-r--r--  2.0 unx     1462 b- defN 24-Apr-29 09:40 migrations/0015_targeted_rollover.py
--rw-r--r--  2.0 unx     2506 b- defN 24-Apr-29 09:40 migrations/0016_upgrade_to_paragraphs_v2.py
--rw-r--r--  2.0 unx     2100 b- defN 24-Apr-29 09:40 migrations/0017_multiple_writable_shards.py
--rw-r--r--  2.0 unx     2264 b- defN 24-Apr-29 09:40 migrations/0018_purge_orphan_kbslugs.py
--rw-r--r--  2.0 unx     2506 b- defN 24-Apr-29 09:40 migrations/0019_upgrade_to_paragraphs_v3.py
--rw-r--r--  2.0 unx      835 b- defN 24-Apr-29 09:40 migrations/__init__.py
--rw-r--r--  2.0 unx      891 b- defN 24-Apr-29 09:40 nucliadb/__init__.py
--rw-r--r--  2.0 unx     3733 b- defN 24-Apr-29 09:40 nucliadb/health.py
--rw-r--r--  2.0 unx    11626 b- defN 24-Apr-29 09:40 nucliadb/learning_proxy.py
--rw-r--r--  2.0 unx     4806 b- defN 24-Apr-29 09:40 nucliadb/metrics_exporter.py
--rw-r--r--  2.0 unx     2272 b- defN 24-Apr-29 09:40 nucliadb/openapi.py
--rw-r--r--  2.0 unx        0 b- defN 24-Apr-29 09:40 nucliadb/py.typed
--rw-r--r--  2.0 unx      835 b- defN 24-Apr-29 09:40 nucliadb/common/__init__.py
--rw-r--r--  2.0 unx     4905 b- defN 24-Apr-29 09:40 nucliadb/common/locking.py
--rw-r--r--  2.0 unx      835 b- defN 24-Apr-29 09:40 nucliadb/common/cluster/__init__.py
--rw-r--r--  2.0 unx     4971 b- defN 24-Apr-29 09:40 nucliadb/common/cluster/base.py
--rw-r--r--  2.0 unx     1495 b- defN 24-Apr-29 09:40 nucliadb/common/cluster/exceptions.py
--rw-r--r--  2.0 unx     3658 b- defN 24-Apr-29 09:40 nucliadb/common/cluster/grpc_node_dummy.py
--rw-r--r--  2.0 unx     3429 b- defN 24-Apr-29 09:40 nucliadb/common/cluster/index_node.py
--rw-r--r--  2.0 unx    21231 b- defN 24-Apr-29 09:40 nucliadb/common/cluster/manager.py
--rw-r--r--  2.0 unx     8490 b- defN 24-Apr-29 09:40 nucliadb/common/cluster/rebalance.py
--rw-r--r--  2.0 unx    19593 b- defN 24-Apr-29 09:40 nucliadb/common/cluster/rollover.py
--rw-r--r--  2.0 unx     2713 b- defN 24-Apr-29 09:40 nucliadb/common/cluster/settings.py
--rw-r--r--  2.0 unx     5494 b- defN 24-Apr-29 09:40 nucliadb/common/cluster/utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-Apr-29 09:40 nucliadb/common/cluster/discovery/__init__.py
--rw-r--r--  2.0 unx     6553 b- defN 24-Apr-29 09:40 nucliadb/common/cluster/discovery/base.py
--rw-r--r--  2.0 unx    12518 b- defN 24-Apr-29 09:40 nucliadb/common/cluster/discovery/k8s.py
--rw-r--r--  2.0 unx     1957 b- defN 24-Apr-29 09:40 nucliadb/common/cluster/discovery/manual.py
--rw-r--r--  2.0 unx     1737 b- defN 24-Apr-29 09:40 nucliadb/common/cluster/discovery/single.py
--rw-r--r--  2.0 unx     1139 b- defN 24-Apr-29 09:40 nucliadb/common/cluster/discovery/types.py
--rw-r--r--  2.0 unx     2548 b- defN 24-Apr-29 09:40 nucliadb/common/cluster/discovery/utils.py
--rw-r--r--  2.0 unx      833 b- defN 24-Apr-29 09:40 nucliadb/common/cluster/standalone/__init__.py
--rw-r--r--  2.0 unx    13707 b- defN 24-Apr-29 09:40 nucliadb/common/cluster/standalone/grpc_node_binding.py
--rw-r--r--  2.0 unx     4683 b- defN 24-Apr-29 09:40 nucliadb/common/cluster/standalone/index_node.py
--rw-r--r--  2.0 unx     3444 b- defN 24-Apr-29 09:40 nucliadb/common/cluster/standalone/service.py
--rw-r--r--  2.0 unx     3386 b- defN 24-Apr-29 09:40 nucliadb/common/cluster/standalone/utils.py
--rw-r--r--  2.0 unx     3498 b- defN 24-Apr-29 09:40 nucliadb/common/context/__init__.py
--rw-r--r--  2.0 unx     1628 b- defN 24-Apr-29 09:40 nucliadb/common/context/fastapi.py
--rw-r--r--  2.0 unx     1813 b- defN 24-Apr-29 09:40 nucliadb/common/datamanagers/__init__.py
--rw-r--r--  2.0 unx     1451 b- defN 24-Apr-29 09:40 nucliadb/common/datamanagers/cluster.py
--rw-r--r--  2.0 unx     5383 b- defN 24-Apr-29 09:40 nucliadb/common/datamanagers/entities.py
--rw-r--r--  2.0 unx      883 b- defN 24-Apr-29 09:40 nucliadb/common/datamanagers/exceptions.py
--rw-r--r--  2.0 unx     3994 b- defN 24-Apr-29 09:40 nucliadb/common/datamanagers/kb.py
--rw-r--r--  2.0 unx     5389 b- defN 24-Apr-29 09:40 nucliadb/common/datamanagers/labels.py
--rw-r--r--  2.0 unx     1599 b- defN 24-Apr-29 09:40 nucliadb/common/datamanagers/processing.py
--rw-r--r--  2.0 unx     8719 b- defN 24-Apr-29 09:40 nucliadb/common/datamanagers/resources.py
--rw-r--r--  2.0 unx     5633 b- defN 24-Apr-29 09:40 nucliadb/common/datamanagers/rollover.py
--rw-r--r--  2.0 unx     1631 b- defN 24-Apr-29 09:40 nucliadb/common/datamanagers/utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-Apr-29 09:40 nucliadb/common/http_clients/__init__.py
--rw-r--r--  2.0 unx     2146 b- defN 24-Apr-29 09:40 nucliadb/common/http_clients/auth.py
--rw-r--r--  2.0 unx     1100 b- defN 24-Apr-29 09:40 nucliadb/common/http_clients/exceptions.py
--rw-r--r--  2.0 unx     7155 b- defN 24-Apr-29 09:40 nucliadb/common/http_clients/processing.py
--rw-r--r--  2.0 unx     1540 b- defN 24-Apr-29 09:40 nucliadb/common/http_clients/pypi.py
--rw-r--r--  2.0 unx     1551 b- defN 24-Apr-29 09:40 nucliadb/common/http_clients/utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-Apr-29 09:40 nucliadb/common/maindb/__init__.py
--rw-r--r--  2.0 unx     3449 b- defN 24-Apr-29 09:40 nucliadb/common/maindb/driver.py
--rw-r--r--  2.0 unx      946 b- defN 24-Apr-29 09:40 nucliadb/common/maindb/exceptions.py
--rw-r--r--  2.0 unx     6769 b- defN 24-Apr-29 09:40 nucliadb/common/maindb/local.py
--rw-r--r--  2.0 unx     8391 b- defN 24-Apr-29 09:40 nucliadb/common/maindb/pg.py
--rw-r--r--  2.0 unx     6053 b- defN 24-Apr-29 09:40 nucliadb/common/maindb/redis.py
--rw-r--r--  2.0 unx    14502 b- defN 24-Apr-29 09:40 nucliadb/common/maindb/tikv.py
--rw-r--r--  2.0 unx     4109 b- defN 24-Apr-29 09:40 nucliadb/common/maindb/utils.py
--rw-r--r--  2.0 unx      932 b- defN 24-Apr-29 09:40 nucliadb/export_import/__init__.py
--rw-r--r--  2.0 unx     6171 b- defN 24-Apr-29 09:40 nucliadb/export_import/datamanager.py
--rw-r--r--  2.0 unx     1949 b- defN 24-Apr-29 09:40 nucliadb/export_import/exceptions.py
--rw-r--r--  2.0 unx     7116 b- defN 24-Apr-29 09:40 nucliadb/export_import/exporter.py
--rw-r--r--  2.0 unx     4258 b- defN 24-Apr-29 09:40 nucliadb/export_import/importer.py
--rw-r--r--  2.0 unx     2063 b- defN 24-Apr-29 09:40 nucliadb/export_import/models.py
--rw-r--r--  2.0 unx     2571 b- defN 24-Apr-29 09:40 nucliadb/export_import/tasks.py
--rw-r--r--  2.0 unx    19270 b- defN 24-Apr-29 09:40 nucliadb/export_import/utils.py
--rw-r--r--  2.0 unx     1011 b- defN 24-Apr-29 09:40 nucliadb/ingest/__init__.py
--rw-r--r--  2.0 unx     7277 b- defN 24-Apr-29 09:40 nucliadb/ingest/app.py
--rw-r--r--  2.0 unx     1005 b- defN 24-Apr-29 09:40 nucliadb/ingest/cache.py
--rw-r--r--  2.0 unx     2484 b- defN 24-Apr-29 09:40 nucliadb/ingest/partitions.py
--rw-r--r--  2.0 unx    19541 b- defN 24-Apr-29 09:40 nucliadb/ingest/processing.py
--rw-r--r--  2.0 unx    20277 b- defN 24-Apr-29 09:40 nucliadb/ingest/serialize.py
--rw-r--r--  2.0 unx     3183 b- defN 24-Apr-29 09:40 nucliadb/ingest/settings.py
--rw-r--r--  2.0 unx     2314 b- defN 24-Apr-29 09:40 nucliadb/ingest/utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-Apr-29 09:40 nucliadb/ingest/consumer/__init__.py
--rw-r--r--  2.0 unx    11563 b- defN 24-Apr-29 09:40 nucliadb/ingest/consumer/auditing.py
--rw-r--r--  2.0 unx    12159 b- defN 24-Apr-29 09:40 nucliadb/ingest/consumer/consumer.py
--rw-r--r--  2.0 unx     3788 b- defN 24-Apr-29 09:40 nucliadb/ingest/consumer/materializer.py
--rw-r--r--  2.0 unx     1075 b- defN 24-Apr-29 09:40 nucliadb/ingest/consumer/metrics.py
--rw-r--r--  2.0 unx     9543 b- defN 24-Apr-29 09:40 nucliadb/ingest/consumer/pull.py
--rw-r--r--  2.0 unx     6935 b- defN 24-Apr-29 09:40 nucliadb/ingest/consumer/service.py
--rw-r--r--  2.0 unx     4331 b- defN 24-Apr-29 09:40 nucliadb/ingest/consumer/shard_creator.py
--rw-r--r--  2.0 unx     2656 b- defN 24-Apr-29 09:40 nucliadb/ingest/consumer/utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-Apr-29 09:40 nucliadb/ingest/fields/__init__.py
--rw-r--r--  2.0 unx    18433 b- defN 24-Apr-29 09:40 nucliadb/ingest/fields/base.py
--rw-r--r--  2.0 unx     6516 b- defN 24-Apr-29 09:40 nucliadb/ingest/fields/conversation.py
--rw-r--r--  2.0 unx     1223 b- defN 24-Apr-29 09:40 nucliadb/ingest/fields/date.py
--rw-r--r--  2.0 unx     1205 b- defN 24-Apr-29 09:40 nucliadb/ingest/fields/exceptions.py
--rw-r--r--  2.0 unx     5159 b- defN 24-Apr-29 09:40 nucliadb/ingest/fields/file.py
--rw-r--r--  2.0 unx     1547 b- defN 24-Apr-29 09:40 nucliadb/ingest/fields/generic.py
--rw-r--r--  2.0 unx     1235 b- defN 24-Apr-29 09:40 nucliadb/ingest/fields/keywordset.py
--rw-r--r--  2.0 unx     2250 b- defN 24-Apr-29 09:40 nucliadb/ingest/fields/layout.py
--rw-r--r--  2.0 unx     4084 b- defN 24-Apr-29 09:40 nucliadb/ingest/fields/link.py
--rw-r--r--  2.0 unx     1319 b- defN 24-Apr-29 09:40 nucliadb/ingest/fields/text.py
--rw-r--r--  2.0 unx      835 b- defN 24-Apr-29 09:40 nucliadb/ingest/orm/__init__.py
--rw-r--r--  2.0 unx    28367 b- defN 24-Apr-29 09:40 nucliadb/ingest/orm/brain.py
--rw-r--r--  2.0 unx    15758 b- defN 24-Apr-29 09:40 nucliadb/ingest/orm/entities.py
--rw-r--r--  2.0 unx     1279 b- defN 24-Apr-29 09:40 nucliadb/ingest/orm/exceptions.py
--rw-r--r--  2.0 unx    17167 b- defN 24-Apr-29 09:40 nucliadb/ingest/orm/knowledgebox.py
--rw-r--r--  2.0 unx     1096 b- defN 24-Apr-29 09:40 nucliadb/ingest/orm/metrics.py
--rw-r--r--  2.0 unx    60444 b- defN 24-Apr-29 09:40 nucliadb/ingest/orm/resource.py
--rw-r--r--  2.0 unx     1739 b- defN 24-Apr-29 09:40 nucliadb/ingest/orm/synonyms.py
--rw-r--r--  2.0 unx     3683 b- defN 24-Apr-29 09:40 nucliadb/ingest/orm/utils.py
--rw-r--r--  2.0 unx    26423 b- defN 24-Apr-29 09:40 nucliadb/ingest/orm/processor/__init__.py
--rw-r--r--  2.0 unx     1690 b- defN 24-Apr-29 09:40 nucliadb/ingest/orm/processor/sequence_manager.py
--rw-r--r--  2.0 unx     2057 b- defN 24-Apr-29 09:40 nucliadb/ingest/service/__init__.py
--rw-r--r--  2.0 unx      835 b- defN 24-Apr-29 09:40 nucliadb/ingest/service/exceptions.py
--rw-r--r--  2.0 unx    33536 b- defN 24-Apr-29 09:40 nucliadb/ingest/service/writer.py
--rw-r--r--  2.0 unx      835 b- defN 24-Apr-29 09:40 nucliadb/ingest/tests/__init__.py
--rw-r--r--  2.0 unx     1157 b- defN 24-Apr-29 09:40 nucliadb/ingest/tests/conftest.py
--rw-r--r--  2.0 unx    24060 b- defN 24-Apr-29 09:40 nucliadb/ingest/tests/fixtures.py
--rw-r--r--  2.0 unx    62843 b- defN 24-Apr-29 09:40 nucliadb/ingest/tests/vectors.py
--rw-r--r--  2.0 unx      835 b- defN 24-Apr-29 09:40 nucliadb/ingest/tests/integration/__init__.py
--rw-r--r--  2.0 unx      833 b- defN 24-Apr-29 09:40 nucliadb/ingest/tests/integration/consumer/__init__.py
--rw-r--r--  2.0 unx     2549 b- defN 24-Apr-29 09:40 nucliadb/ingest/tests/integration/consumer/test_auditing.py
--rw-r--r--  2.0 unx     2591 b- defN 24-Apr-29 09:40 nucliadb/ingest/tests/integration/consumer/test_materializer.py
--rw-r--r--  2.0 unx     4465 b- defN 24-Apr-29 09:40 nucliadb/ingest/tests/integration/consumer/test_pull.py
--rw-r--r--  2.0 unx     2763 b- defN 24-Apr-29 09:40 nucliadb/ingest/tests/integration/consumer/test_service.py
--rw-r--r--  2.0 unx     2019 b- defN 24-Apr-29 09:40 nucliadb/ingest/tests/integration/consumer/test_shard_creator.py
--rw-r--r--  2.0 unx      835 b- defN 24-Apr-29 09:40 nucliadb/ingest/tests/integration/ingest/__init__.py
--rw-r--r--  2.0 unx    27325 b- defN 24-Apr-29 09:40 nucliadb/ingest/tests/integration/ingest/test_ingest.py
--rw-r--r--  2.0 unx     3040 b- defN 24-Apr-29 09:40 nucliadb/ingest/tests/integration/ingest/test_processing_engine.py
--rw-r--r--  2.0 unx     8586 b- defN 24-Apr-29 09:40 nucliadb/ingest/tests/integration/ingest/test_relations.py
--rw-r--r--  2.0 unx      835 b- defN 24-Apr-29 09:40 nucliadb/ingest/tests/unit/__init__.py
--rw-r--r--  2.0 unx     1189 b- defN 24-Apr-29 09:40 nucliadb/ingest/tests/unit/test_cache.py
--rw-r--r--  2.0 unx     1432 b- defN 24-Apr-29 09:40 nucliadb/ingest/tests/unit/test_partitions.py
--rw-r--r--  2.0 unx     5807 b- defN 24-Apr-29 09:40 nucliadb/ingest/tests/unit/test_processing.py
--rw-r--r--  2.0 unx      978 b- defN 24-Apr-29 09:40 nucliadb/ingest/tests/unit/test_settings.py
--rw-r--r--  2.0 unx      833 b- defN 24-Apr-29 09:40 nucliadb/ingest/tests/unit/consumer/__init__.py
--rw-r--r--  2.0 unx     3981 b- defN 24-Apr-29 09:40 nucliadb/ingest/tests/unit/consumer/test_auditing.py
--rw-r--r--  2.0 unx     2472 b- defN 24-Apr-29 09:40 nucliadb/ingest/tests/unit/consumer/test_consumer.py
--rw-r--r--  2.0 unx     2063 b- defN 24-Apr-29 09:40 nucliadb/ingest/tests/unit/consumer/test_pull.py
--rw-r--r--  2.0 unx     4075 b- defN 24-Apr-29 09:40 nucliadb/ingest/tests/unit/consumer/test_shard_creator.py
--rw-r--r--  2.0 unx     1934 b- defN 24-Apr-29 09:40 nucliadb/ingest/tests/unit/consumer/test_utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-Apr-29 09:40 nucliadb/ingest/tests/unit/orm/__init__.py
--rw-r--r--  2.0 unx     9876 b- defN 24-Apr-29 09:40 nucliadb/ingest/tests/unit/orm/test_brain.py
--rw-r--r--  2.0 unx     2435 b- defN 24-Apr-29 09:40 nucliadb/ingest/tests/unit/orm/test_brain_vectors.py
--rw-r--r--  2.0 unx     1174 b- defN 24-Apr-29 09:40 nucliadb/ingest/tests/unit/orm/test_orm_utils.py
--rw-r--r--  2.0 unx     4045 b- defN 24-Apr-29 09:40 nucliadb/ingest/tests/unit/orm/test_processor.py
--rw-r--r--  2.0 unx    11033 b- defN 24-Apr-29 09:40 nucliadb/ingest/tests/unit/orm/test_resource.py
--rw-r--r--  2.0 unx     2216 b- defN 24-Apr-29 09:40 nucliadb/middleware/__init__.py
--rw-r--r--  2.0 unx     3912 b- defN 24-Apr-29 09:40 nucliadb/middleware/transaction.py
--rw-r--r--  2.0 unx      835 b- defN 24-Apr-29 09:40 nucliadb/migrator/__init__.py
--rw-r--r--  2.0 unx     2119 b- defN 24-Apr-29 09:40 nucliadb/migrator/command.py
--rw-r--r--  2.0 unx     1334 b- defN 24-Apr-29 09:40 nucliadb/migrator/context.py
--rw-r--r--  2.0 unx     5104 b- defN 24-Apr-29 09:40 nucliadb/migrator/datamanager.py
--rw-r--r--  2.0 unx      889 b- defN 24-Apr-29 09:40 nucliadb/migrator/exceptions.py
--rw-r--r--  2.0 unx     9237 b- defN 24-Apr-29 09:40 nucliadb/migrator/migrator.py
--rw-r--r--  2.0 unx     1145 b- defN 24-Apr-29 09:40 nucliadb/migrator/models.py
--rw-r--r--  2.0 unx     1110 b- defN 24-Apr-29 09:40 nucliadb/migrator/settings.py
--rw-r--r--  2.0 unx     2346 b- defN 24-Apr-29 09:40 nucliadb/migrator/utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-Apr-29 09:40 nucliadb/models/__init__.py
--rw-r--r--  2.0 unx     1599 b- defN 24-Apr-29 09:40 nucliadb/models/responses.py
--rw-r--r--  2.0 unx     6041 b- defN 24-Apr-29 09:40 nucliadb/purge/__init__.py
--rw-r--r--  2.0 unx     9364 b- defN 24-Apr-29 09:40 nucliadb/purge/orphan_shards.py
--rw-r--r--  2.0 unx     1328 b- defN 24-Apr-29 09:40 nucliadb/reader/__init__.py
--rw-r--r--  2.0 unx     3709 b- defN 24-Apr-29 09:40 nucliadb/reader/app.py
--rw-r--r--  2.0 unx     1366 b- defN 24-Apr-29 09:40 nucliadb/reader/lifecycle.py
--rw-r--r--  2.0 unx     1031 b- defN 24-Apr-29 09:40 nucliadb/reader/openapi.py
--rw-r--r--  2.0 unx     1447 b- defN 24-Apr-29 09:40 nucliadb/reader/run.py
--rw-r--r--  2.0 unx      872 b- defN 24-Apr-29 09:40 nucliadb/reader/api/__init__.py
--rw-r--r--  2.0 unx     2434 b- defN 24-Apr-29 09:40 nucliadb/reader/api/models.py
--rw-r--r--  2.0 unx     1110 b- defN 24-Apr-29 09:40 nucliadb/reader/api/v1/__init__.py
--rw-r--r--  2.0 unx    12368 b- defN 24-Apr-29 09:40 nucliadb/reader/api/v1/download.py
--rw-r--r--  2.0 unx     6450 b- defN 24-Apr-29 09:40 nucliadb/reader/api/v1/export_import.py
--rw-r--r--  2.0 unx     3632 b- defN 24-Apr-29 09:40 nucliadb/reader/api/v1/knowledgebox.py
--rw-r--r--  2.0 unx     2093 b- defN 24-Apr-29 09:40 nucliadb/reader/api/v1/learning_collector.py
--rw-r--r--  2.0 unx     4454 b- defN 24-Apr-29 09:40 nucliadb/reader/api/v1/learning_config.py
--rw-r--r--  2.0 unx    13928 b- defN 24-Apr-29 09:40 nucliadb/reader/api/v1/resource.py
--rw-r--r--  2.0 unx     1011 b- defN 24-Apr-29 09:40 nucliadb/reader/api/v1/router.py
--rw-r--r--  2.0 unx    12378 b- defN 24-Apr-29 09:40 nucliadb/reader/api/v1/services.py
--rw-r--r--  2.0 unx      835 b- defN 24-Apr-29 09:40 nucliadb/reader/reader/__init__.py
--rw-r--r--  2.0 unx     8155 b- defN 24-Apr-29 09:40 nucliadb/reader/reader/notifications.py
--rw-r--r--  2.0 unx      835 b- defN 24-Apr-29 09:40 nucliadb/reader/tests/__init__.py
--rw-r--r--  2.0 unx     1224 b- defN 24-Apr-29 09:40 nucliadb/reader/tests/conftest.py
--rw-r--r--  2.0 unx     4345 b- defN 24-Apr-29 09:40 nucliadb/reader/tests/fixtures.py
--rw-r--r--  2.0 unx     2748 b- defN 24-Apr-29 09:40 nucliadb/reader/tests/test_list_resources.py
--rw-r--r--  2.0 unx    10199 b- defN 24-Apr-29 09:40 nucliadb/reader/tests/test_reader_file_download.py
--rw-r--r--  2.0 unx    10586 b- defN 24-Apr-29 09:40 nucliadb/reader/tests/test_reader_resource.py
--rw-r--r--  2.0 unx     6535 b- defN 24-Apr-29 09:40 nucliadb/reader/tests/test_reader_resource_field.py
--rw-r--r--  2.0 unx     1535 b- defN 24-Apr-29 09:40 nucliadb/search/__init__.py
--rw-r--r--  2.0 unx     4905 b- defN 24-Apr-29 09:40 nucliadb/search/app.py
--rw-r--r--  2.0 unx     1956 b- defN 24-Apr-29 09:40 nucliadb/search/lifecycle.py
--rw-r--r--  2.0 unx     1016 b- defN 24-Apr-29 09:40 nucliadb/search/openapi.py
--rw-r--r--  2.0 unx    18535 b- defN 24-Apr-29 09:40 nucliadb/search/predict.py
--rw-r--r--  2.0 unx     1402 b- defN 24-Apr-29 09:40 nucliadb/search/run.py
--rw-r--r--  2.0 unx     1193 b- defN 24-Apr-29 09:40 nucliadb/search/settings.py
--rw-r--r--  2.0 unx     1037 b- defN 24-Apr-29 09:40 nucliadb/search/utilities.py
--rw-r--r--  2.0 unx      835 b- defN 24-Apr-29 09:40 nucliadb/search/api/__init__.py
--rw-r--r--  2.0 unx     1272 b- defN 24-Apr-29 09:40 nucliadb/search/api/v1/__init__.py
--rw-r--r--  2.0 unx     9913 b- defN 24-Apr-29 09:40 nucliadb/search/api/v1/chat.py
--rw-r--r--  2.0 unx     2665 b- defN 24-Apr-29 09:40 nucliadb/search/api/v1/feedback.py
--rw-r--r--  2.0 unx     8804 b- defN 24-Apr-29 09:40 nucliadb/search/api/v1/find.py
--rw-r--r--  2.0 unx     6938 b- defN 24-Apr-29 09:40 nucliadb/search/api/v1/knowledgebox.py
--rw-r--r--  2.0 unx     3041 b- defN 24-Apr-29 09:40 nucliadb/search/api/v1/predict_proxy.py
--rw-r--r--  2.0 unx      988 b- defN 24-Apr-29 09:40 nucliadb/search/api/v1/router.py
--rw-r--r--  2.0 unx    18325 b- defN 24-Apr-29 09:40 nucliadb/search/api/v1/search.py
--rw-r--r--  2.0 unx     5928 b- defN 24-Apr-29 09:40 nucliadb/search/api/v1/suggest.py
--rw-r--r--  2.0 unx     2536 b- defN 24-Apr-29 09:40 nucliadb/search/api/v1/summarize.py
--rw-r--r--  2.0 unx     1412 b- defN 24-Apr-29 09:40 nucliadb/search/api/v1/utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-Apr-29 09:40 nucliadb/search/api/v1/resource/__init__.py
--rw-r--r--  2.0 unx     6095 b- defN 24-Apr-29 09:40 nucliadb/search/api/v1/resource/ask.py
--rw-r--r--  2.0 unx     5887 b- defN 24-Apr-29 09:40 nucliadb/search/api/v1/resource/chat.py
--rw-r--r--  2.0 unx     5293 b- defN 24-Apr-29 09:40 nucliadb/search/api/v1/resource/search.py
--rw-r--r--  2.0 unx      833 b- defN 24-Apr-29 09:40 nucliadb/search/requesters/__init__.py
--rw-r--r--  2.0 unx     9070 b- defN 24-Apr-29 09:40 nucliadb/search/requesters/utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-Apr-29 09:40 nucliadb/search/search/__init__.py
--rw-r--r--  2.0 unx     2746 b- defN 24-Apr-29 09:40 nucliadb/search/search/cache.py
--rw-r--r--  2.0 unx     1154 b- defN 24-Apr-29 09:40 nucliadb/search/search/exceptions.py
--rw-r--r--  2.0 unx     5465 b- defN 24-Apr-29 09:40 nucliadb/search/search/fetch.py
--rw-r--r--  2.0 unx     6513 b- defN 24-Apr-29 09:40 nucliadb/search/search/filters.py
--rw-r--r--  2.0 unx     4612 b- defN 24-Apr-29 09:40 nucliadb/search/search/find.py
--rw-r--r--  2.0 unx    17152 b- defN 24-Apr-29 09:40 nucliadb/search/search/find_merge.py
--rw-r--r--  2.0 unx    21282 b- defN 24-Apr-29 09:40 nucliadb/search/search/merge.py
--rw-r--r--  2.0 unx     1130 b- defN 24-Apr-29 09:40 nucliadb/search/search/metrics.py
--rw-r--r--  2.0 unx     8698 b- defN 24-Apr-29 09:40 nucliadb/search/search/paragraphs.py
--rw-r--r--  2.0 unx     3026 b- defN 24-Apr-29 09:40 nucliadb/search/search/predict_proxy.py
--rw-r--r--  2.0 unx    31084 b- defN 24-Apr-29 09:40 nucliadb/search/search/query.py
--rw-r--r--  2.0 unx     3018 b- defN 24-Apr-29 09:40 nucliadb/search/search/shards.py
--rw-r--r--  2.0 unx     5101 b- defN 24-Apr-29 09:40 nucliadb/search/search/summarize.py
--rw-r--r--  2.0 unx     2438 b- defN 24-Apr-29 09:40 nucliadb/search/search/utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-Apr-29 09:40 nucliadb/search/search/chat/__init__.py
--rw-r--r--  2.0 unx     2058 b- defN 24-Apr-29 09:40 nucliadb/search/search/chat/images.py
--rw-r--r--  2.0 unx    20793 b- defN 24-Apr-29 09:40 nucliadb/search/search/chat/prompt.py
--rw-r--r--  2.0 unx    15347 b- defN 24-Apr-29 09:40 nucliadb/search/search/chat/query.py
--rw-r--r--  2.0 unx      835 b- defN 24-Apr-29 09:40 nucliadb/search/tests/__init__.py
--rw-r--r--  2.0 unx     1295 b- defN 24-Apr-29 09:40 nucliadb/search/tests/conftest.py
--rw-r--r--  2.0 unx     6578 b- defN 24-Apr-29 09:40 nucliadb/search/tests/fixtures.py
--rw-r--r--  2.0 unx    15529 b- defN 24-Apr-29 09:40 nucliadb/search/tests/node.py
--rw-r--r--  2.0 unx      833 b- defN 24-Apr-29 09:40 nucliadb/search/tests/unit/__init__.py
--rw-r--r--  2.0 unx     2649 b- defN 24-Apr-29 09:40 nucliadb/search/tests/unit/test_app.py
--rw-r--r--  2.0 unx     3374 b- defN 24-Apr-29 09:40 nucliadb/search/tests/unit/test_find_merge.py
--rw-r--r--  2.0 unx     1400 b- defN 24-Apr-29 09:40 nucliadb/search/tests/unit/test_merge.py
--rw-r--r--  2.0 unx    14729 b- defN 24-Apr-29 09:40 nucliadb/search/tests/unit/test_predict.py
--rw-r--r--  2.0 unx     1317 b- defN 24-Apr-29 09:40 nucliadb/search/tests/unit/test_run.py
--rw-r--r--  2.0 unx      835 b- defN 24-Apr-29 09:40 nucliadb/search/tests/unit/api/__init__.py
--rw-r--r--  2.0 unx      835 b- defN 24-Apr-29 09:40 nucliadb/search/tests/unit/api/v1/__init__.py
--rw-r--r--  2.0 unx     2966 b- defN 24-Apr-29 09:40 nucliadb/search/tests/unit/api/v1/test_chat.py
--rw-r--r--  2.0 unx     2865 b- defN 24-Apr-29 09:40 nucliadb/search/tests/unit/api/v1/test_predict_proxy.py
--rw-r--r--  2.0 unx     2901 b- defN 24-Apr-29 09:40 nucliadb/search/tests/unit/api/v1/test_summarize.py
--rw-r--r--  2.0 unx      835 b- defN 24-Apr-29 09:40 nucliadb/search/tests/unit/api/v1/resource/__init__.py
--rw-r--r--  2.0 unx     2411 b- defN 24-Apr-29 09:40 nucliadb/search/tests/unit/api/v1/resource/test_ask.py
--rw-r--r--  2.0 unx     3040 b- defN 24-Apr-29 09:40 nucliadb/search/tests/unit/api/v1/resource/test_chat.py
--rw-r--r--  2.0 unx      833 b- defN 24-Apr-29 09:40 nucliadb/search/tests/unit/search/__init__.py
--rw-r--r--  2.0 unx     8567 b- defN 24-Apr-29 09:40 nucliadb/search/tests/unit/search/test_chat_prompt.py
--rw-r--r--  2.0 unx     3736 b- defN 24-Apr-29 09:40 nucliadb/search/tests/unit/search/test_fetch.py
--rw-r--r--  2.0 unx     4306 b- defN 24-Apr-29 09:40 nucliadb/search/tests/unit/search/test_filters.py
--rw-r--r--  2.0 unx     4492 b- defN 24-Apr-29 09:40 nucliadb/search/tests/unit/search/test_paragraphs.py
--rw-r--r--  2.0 unx     3496 b- defN 24-Apr-29 09:40 nucliadb/search/tests/unit/search/test_predict_proxy.py
--rw-r--r--  2.0 unx     7001 b- defN 24-Apr-29 09:40 nucliadb/search/tests/unit/search/test_query.py
--rw-r--r--  2.0 unx      833 b- defN 24-Apr-29 09:40 nucliadb/search/tests/unit/search/requesters/__init__.py
--rw-r--r--  2.0 unx     6455 b- defN 24-Apr-29 09:40 nucliadb/search/tests/unit/search/requesters/test_utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-Apr-29 09:40 nucliadb/search/tests/unit/search/search/__init__.py
--rw-r--r--  2.0 unx     1759 b- defN 24-Apr-29 09:40 nucliadb/search/tests/unit/search/search/test_shards.py
--rw-r--r--  2.0 unx     2511 b- defN 24-Apr-29 09:40 nucliadb/search/tests/unit/search/search/test_utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-Apr-29 09:40 nucliadb/standalone/__init__.py
--rw-r--r--  2.0 unx     6746 b- defN 24-Apr-29 09:40 nucliadb/standalone/api_router.py
--rw-r--r--  2.0 unx     5763 b- defN 24-Apr-29 09:40 nucliadb/standalone/app.py
--rw-r--r--  2.0 unx     7800 b- defN 24-Apr-29 09:40 nucliadb/standalone/auth.py
--rw-r--r--  2.0 unx     5309 b- defN 24-Apr-29 09:40 nucliadb/standalone/config.py
--rw-r--r--  2.0 unx     6930 b- defN 24-Apr-29 09:40 nucliadb/standalone/introspect.py
--rw-r--r--  2.0 unx     2488 b- defN 24-Apr-29 09:40 nucliadb/standalone/lifecycle.py
--rw-r--r--  2.0 unx     1317 b- defN 24-Apr-29 09:40 nucliadb/standalone/purge.py
--rw-r--r--  2.0 unx     5336 b- defN 24-Apr-29 09:40 nucliadb/standalone/run.py
--rw-r--r--  2.0 unx     5781 b- defN 24-Apr-29 09:40 nucliadb/standalone/settings.py
--rw-r--r--  2.0 unx     3132 b- defN 24-Apr-29 09:40 nucliadb/standalone/versions.py
--rw-r--r--  2.0 unx     2285 b- defN 24-Apr-29 09:40 nucliadb/standalone/static/favicon.ico
--rw-r--r--  2.0 unx     3833 b- defN 24-Apr-29 09:40 nucliadb/standalone/static/index.html
--rw-r--r--  2.0 unx     2639 b- defN 24-Apr-29 09:40 nucliadb/standalone/static/logo.svg
--rw-r--r--  2.0 unx      835 b- defN 24-Apr-29 09:40 nucliadb/standalone/tests/__init__.py
--rw-r--r--  2.0 unx     1294 b- defN 24-Apr-29 09:40 nucliadb/standalone/tests/conftest.py
--rw-r--r--  2.0 unx     1319 b- defN 24-Apr-29 09:40 nucliadb/standalone/tests/fixtures.py
--rw-r--r--  2.0 unx      833 b- defN 24-Apr-29 09:40 nucliadb/standalone/tests/unit/__init__.py
--rw-r--r--  2.0 unx     1722 b- defN 24-Apr-29 09:40 nucliadb/standalone/tests/unit/test_api_router.py
--rw-r--r--  2.0 unx     5509 b- defN 24-Apr-29 09:40 nucliadb/standalone/tests/unit/test_auth.py
--rw-r--r--  2.0 unx     1334 b- defN 24-Apr-29 09:40 nucliadb/standalone/tests/unit/test_introspect.py
--rw-r--r--  2.0 unx     1472 b- defN 24-Apr-29 09:40 nucliadb/standalone/tests/unit/test_run.py
--rw-r--r--  2.0 unx     1972 b- defN 24-Apr-29 09:40 nucliadb/standalone/tests/unit/test_versions.py
--rw-r--r--  2.0 unx     1037 b- defN 24-Apr-29 09:40 nucliadb/tasks/__init__.py
--rw-r--r--  2.0 unx     7655 b- defN 24-Apr-29 09:40 nucliadb/tasks/consumer.py
--rw-r--r--  2.0 unx      924 b- defN 24-Apr-29 09:40 nucliadb/tasks/logger.py
--rw-r--r--  2.0 unx     1378 b- defN 24-Apr-29 09:40 nucliadb/tasks/models.py
--rw-r--r--  2.0 unx     3457 b- defN 24-Apr-29 09:40 nucliadb/tasks/producer.py
--rw-r--r--  2.0 unx     1753 b- defN 24-Apr-29 09:40 nucliadb/tasks/registry.py
--rw-r--r--  2.0 unx     1360 b- defN 24-Apr-29 09:40 nucliadb/tasks/utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-Apr-29 09:40 nucliadb/tests/__init__.py
--rw-r--r--  2.0 unx     1229 b- defN 24-Apr-29 09:40 nucliadb/tests/conftest.py
--rw-r--r--  2.0 unx    22365 b- defN 24-Apr-29 09:40 nucliadb/tests/fixtures.py
--rw-r--r--  2.0 unx     7549 b- defN 24-Apr-29 09:40 nucliadb/tests/tikv.py
--rw-r--r--  2.0 unx      835 b- defN 24-Apr-29 09:40 nucliadb/tests/benchmarks/__init__.py
--rw-r--r--  2.0 unx     3032 b- defN 24-Apr-29 09:40 nucliadb/tests/benchmarks/test_search.py
--rw-r--r--  2.0 unx      919 b- defN 24-Apr-29 09:40 nucliadb/tests/knowledgeboxes/__init__.py
--rw-r--r--  2.0 unx     7002 b- defN 24-Apr-29 09:40 nucliadb/tests/knowledgeboxes/philosophy_books.py
--rw-r--r--  2.0 unx     3037 b- defN 24-Apr-29 09:40 nucliadb/tests/knowledgeboxes/ten_dummy_resources.py
--rw-r--r--  2.0 unx     1148 b- defN 24-Apr-29 09:40 nucliadb/tests/migrations/__init__.py
--rw-r--r--  2.0 unx     2726 b- defN 24-Apr-29 09:40 nucliadb/tests/migrations/test_migration_0017.py
--rw-r--r--  2.0 unx     3625 b- defN 24-Apr-29 09:40 nucliadb/tests/migrations/test_migration_0018.py
--rw-r--r--  2.0 unx      835 b- defN 24-Apr-29 09:40 nucliadb/tests/unit/__init__.py
--rw-r--r--  2.0 unx     1487 b- defN 24-Apr-29 09:40 nucliadb/tests/unit/test_field_ids.py
--rw-r--r--  2.0 unx     2758 b- defN 24-Apr-29 09:40 nucliadb/tests/unit/test_health.py
--rw-r--r--  2.0 unx     1543 b- defN 24-Apr-29 09:40 nucliadb/tests/unit/test_kb_slugs.py
--rw-r--r--  2.0 unx     7892 b- defN 24-Apr-29 09:40 nucliadb/tests/unit/test_learning_proxy.py
--rw-r--r--  2.0 unx     2642 b- defN 24-Apr-29 09:40 nucliadb/tests/unit/test_metrics_exporter.py
--rw-r--r--  2.0 unx     1341 b- defN 24-Apr-29 09:40 nucliadb/tests/unit/test_openapi.py
--rw-r--r--  2.0 unx     3656 b- defN 24-Apr-29 09:40 nucliadb/tests/unit/test_purge.py
--rw-r--r--  2.0 unx      835 b- defN 24-Apr-29 09:40 nucliadb/tests/unit/common/__init__.py
--rw-r--r--  2.0 unx     1268 b- defN 24-Apr-29 09:40 nucliadb/tests/unit/common/test_context.py
--rw-r--r--  2.0 unx      835 b- defN 24-Apr-29 09:40 nucliadb/tests/unit/common/cluster/__init__.py
--rw-r--r--  2.0 unx    11955 b- defN 24-Apr-29 09:40 nucliadb/tests/unit/common/cluster/test_cluster.py
--rw-r--r--  2.0 unx     5387 b- defN 24-Apr-29 09:40 nucliadb/tests/unit/common/cluster/test_kb_shard_manager.py
--rw-r--r--  2.0 unx     9470 b- defN 24-Apr-29 09:40 nucliadb/tests/unit/common/cluster/test_rollover.py
--rw-r--r--  2.0 unx      835 b- defN 24-Apr-29 09:40 nucliadb/tests/unit/common/cluster/discovery/__init__.py
--rw-r--r--  2.0 unx     5584 b- defN 24-Apr-29 09:40 nucliadb/tests/unit/common/cluster/discovery/test_k8s.py
--rw-r--r--  2.0 unx      833 b- defN 24-Apr-29 09:40 nucliadb/tests/unit/common/cluster/standalone/__init__.py
--rw-r--r--  2.0 unx     3750 b- defN 24-Apr-29 09:40 nucliadb/tests/unit/common/cluster/standalone/test_service.py
--rw-r--r--  2.0 unx     2114 b- defN 24-Apr-29 09:40 nucliadb/tests/unit/common/cluster/standalone/test_utils.py
--rw-r--r--  2.0 unx      833 b- defN 24-Apr-29 09:40 nucliadb/tests/unit/common/maindb/__init__.py
--rw-r--r--  2.0 unx     3579 b- defN 24-Apr-29 09:40 nucliadb/tests/unit/common/maindb/test_driver.py
--rw-r--r--  2.0 unx     1869 b- defN 24-Apr-29 09:40 nucliadb/tests/unit/common/maindb/test_tikv.py
--rw-r--r--  2.0 unx     2998 b- defN 24-Apr-29 09:40 nucliadb/tests/unit/common/maindb/test_utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-Apr-29 09:40 nucliadb/tests/unit/export_import/__init__.py
--rw-r--r--  2.0 unx     1435 b- defN 24-Apr-29 09:40 nucliadb/tests/unit/export_import/test_datamanager.py
--rw-r--r--  2.0 unx     9706 b- defN 24-Apr-29 09:40 nucliadb/tests/unit/export_import/test_utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-Apr-29 09:40 nucliadb/tests/unit/migrator/__init__.py
--rw-r--r--  2.0 unx     3233 b- defN 24-Apr-29 09:40 nucliadb/tests/unit/migrator/test_migrator.py
--rw-r--r--  2.0 unx      835 b- defN 24-Apr-29 09:40 nucliadb/tests/unit/tasks/__init__.py
--rw-r--r--  2.0 unx     1375 b- defN 24-Apr-29 09:40 nucliadb/tests/unit/tasks/conftest.py
--rw-r--r--  2.0 unx     2714 b- defN 24-Apr-29 09:40 nucliadb/tests/unit/tasks/test_consumer.py
--rw-r--r--  2.0 unx     3189 b- defN 24-Apr-29 09:40 nucliadb/tests/unit/tasks/test_producer.py
--rw-r--r--  2.0 unx     1827 b- defN 24-Apr-29 09:40 nucliadb/tests/unit/tasks/test_tasks.py
--rw-r--r--  2.0 unx     2507 b- defN 24-Apr-29 09:40 nucliadb/tests/utils/__init__.py
--rw-r--r--  2.0 unx     1797 b- defN 24-Apr-29 09:40 nucliadb/tests/utils/aiohttp_session.py
--rw-r--r--  2.0 unx     2533 b- defN 24-Apr-29 09:40 nucliadb/tests/utils/entities.py
--rw-r--r--  2.0 unx     6327 b- defN 24-Apr-29 09:40 nucliadb/tests/utils/broker_messages/__init__.py
--rw-r--r--  2.0 unx     7557 b- defN 24-Apr-29 09:40 nucliadb/tests/utils/broker_messages/fields.py
--rw-r--r--  2.0 unx     1196 b- defN 24-Apr-29 09:40 nucliadb/tests/utils/broker_messages/helpers.py
--rw-r--r--  2.0 unx     1325 b- defN 24-Apr-29 09:40 nucliadb/train/__init__.py
--rw-r--r--  2.0 unx     3530 b- defN 24-Apr-29 09:40 nucliadb/train/app.py
--rw-r--r--  2.0 unx     3800 b- defN 24-Apr-29 09:40 nucliadb/train/generator.py
--rw-r--r--  2.0 unx     1698 b- defN 24-Apr-29 09:40 nucliadb/train/lifecycle.py
--rw-r--r--  2.0 unx     1198 b- defN 24-Apr-29 09:40 nucliadb/train/models.py
--rw-r--r--  2.0 unx     5706 b- defN 24-Apr-29 09:40 nucliadb/train/nodes.py
--rw-r--r--  2.0 unx     1400 b- defN 24-Apr-29 09:40 nucliadb/train/run.py
--rw-r--r--  2.0 unx     5926 b- defN 24-Apr-29 09:40 nucliadb/train/servicer.py
--rw-r--r--  2.0 unx     1415 b- defN 24-Apr-29 09:40 nucliadb/train/settings.py
--rw-r--r--  2.0 unx     1496 b- defN 24-Apr-29 09:40 nucliadb/train/types.py
--rw-r--r--  2.0 unx     3265 b- defN 24-Apr-29 09:40 nucliadb/train/upload.py
--rw-r--r--  2.0 unx     6420 b- defN 24-Apr-29 09:40 nucliadb/train/uploader.py
--rw-r--r--  2.0 unx     3179 b- defN 24-Apr-29 09:40 nucliadb/train/utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-Apr-29 09:40 nucliadb/train/api/__init__.py
--rw-r--r--  2.0 unx     1479 b- defN 24-Apr-29 09:40 nucliadb/train/api/utils.py
--rw-r--r--  2.0 unx      928 b- defN 24-Apr-29 09:40 nucliadb/train/api/v1/__init__.py
--rw-r--r--  2.0 unx     2065 b- defN 24-Apr-29 09:40 nucliadb/train/api/v1/check.py
--rw-r--r--  2.0 unx      910 b- defN 24-Apr-29 09:40 nucliadb/train/api/v1/router.py
--rw-r--r--  2.0 unx     1905 b- defN 24-Apr-29 09:40 nucliadb/train/api/v1/shards.py
--rw-r--r--  2.0 unx     2129 b- defN 24-Apr-29 09:40 nucliadb/train/api/v1/trainset.py
--rw-r--r--  2.0 unx      835 b- defN 24-Apr-29 09:40 nucliadb/train/generators/__init__.py
--rw-r--r--  2.0 unx     3723 b- defN 24-Apr-29 09:40 nucliadb/train/generators/field_classifier.py
--rw-r--r--  2.0 unx     6712 b- defN 24-Apr-29 09:40 nucliadb/train/generators/image_classifier.py
--rw-r--r--  2.0 unx     2789 b- defN 24-Apr-29 09:40 nucliadb/train/generators/paragraph_classifier.py
--rw-r--r--  2.0 unx     3590 b- defN 24-Apr-29 09:40 nucliadb/train/generators/paragraph_streaming.py
--rw-r--r--  2.0 unx     5372 b- defN 24-Apr-29 09:40 nucliadb/train/generators/question_answer_streaming.py
--rw-r--r--  2.0 unx     5160 b- defN 24-Apr-29 09:40 nucliadb/train/generators/sentence_classifier.py
--rw-r--r--  2.0 unx    10446 b- defN 24-Apr-29 09:40 nucliadb/train/generators/token_classifier.py
--rw-r--r--  2.0 unx     3877 b- defN 24-Apr-29 09:40 nucliadb/train/generators/utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-Apr-29 09:40 nucliadb/train/tests/__init__.py
--rw-r--r--  2.0 unx     1125 b- defN 24-Apr-29 09:40 nucliadb/train/tests/conftest.py
--rw-r--r--  2.0 unx    11053 b- defN 24-Apr-29 09:40 nucliadb/train/tests/fixtures.py
--rw-r--r--  2.0 unx     4598 b- defN 24-Apr-29 09:40 nucliadb/train/tests/test_field_classification.py
--rw-r--r--  2.0 unx     2729 b- defN 24-Apr-29 09:40 nucliadb/train/tests/test_get_entities.py
--rw-r--r--  2.0 unx     1876 b- defN 24-Apr-29 09:40 nucliadb/train/tests/test_get_info.py
--rw-r--r--  2.0 unx     1382 b- defN 24-Apr-29 09:40 nucliadb/train/tests/test_get_ontology.py
--rw-r--r--  2.0 unx     2417 b- defN 24-Apr-29 09:40 nucliadb/train/tests/test_get_ontology_count.py
--rw-r--r--  2.0 unx     7669 b- defN 24-Apr-29 09:40 nucliadb/train/tests/test_image_classification.py
--rw-r--r--  2.0 unx     1416 b- defN 24-Apr-29 09:40 nucliadb/train/tests/test_list_fields.py
--rw-r--r--  2.0 unx     2944 b- defN 24-Apr-29 09:40 nucliadb/train/tests/test_list_paragraphs.py
--rw-r--r--  2.0 unx     1423 b- defN 24-Apr-29 09:40 nucliadb/train/tests/test_list_resources.py
--rw-r--r--  2.0 unx     2947 b- defN 24-Apr-29 09:40 nucliadb/train/tests/test_list_sentences.py
--rw-r--r--  2.0 unx     4645 b- defN 24-Apr-29 09:40 nucliadb/train/tests/test_paragraph_classification.py
--rw-r--r--  2.0 unx     4320 b- defN 24-Apr-29 09:40 nucliadb/train/tests/test_paragraph_streaming.py
--rw-r--r--  2.0 unx     8751 b- defN 24-Apr-29 09:40 nucliadb/train/tests/test_question_answer_streaming.py
--rw-r--r--  2.0 unx     5051 b- defN 24-Apr-29 09:40 nucliadb/train/tests/test_sentence_classification.py
--rw-r--r--  2.0 unx     5583 b- defN 24-Apr-29 09:40 nucliadb/train/tests/test_token_classification.py
--rw-r--r--  2.0 unx     3324 b- defN 24-Apr-29 09:40 nucliadb/train/tests/utils.py
--rw-r--r--  2.0 unx     1328 b- defN 24-Apr-29 09:40 nucliadb/writer/__init__.py
--rw-r--r--  2.0 unx     4268 b- defN 24-Apr-29 09:40 nucliadb/writer/app.py
--rw-r--r--  2.0 unx    19495 b- defN 24-Apr-29 09:40 nucliadb/writer/back_pressure.py
--rw-r--r--  2.0 unx      972 b- defN 24-Apr-29 09:40 nucliadb/writer/exceptions.py
--rw-r--r--  2.0 unx     1953 b- defN 24-Apr-29 09:40 nucliadb/writer/lifecycle.py
--rw-r--r--  2.0 unx     1032 b- defN 24-Apr-29 09:40 nucliadb/writer/openapi.py
--rw-r--r--  2.0 unx     1448 b- defN 24-Apr-29 09:40 nucliadb/writer/run.py
--rw-r--r--  2.0 unx     3074 b- defN 24-Apr-29 09:40 nucliadb/writer/settings.py
--rw-r--r--  2.0 unx     1036 b- defN 24-Apr-29 09:40 nucliadb/writer/utilities.py
--rw-r--r--  2.0 unx      835 b- defN 24-Apr-29 09:40 nucliadb/writer/api/__init__.py
--rw-r--r--  2.0 unx     1429 b- defN 24-Apr-29 09:40 nucliadb/writer/api/constants.py
--rw-r--r--  2.0 unx     1095 b- defN 24-Apr-29 09:40 nucliadb/writer/api/v1/__init__.py
--rw-r--r--  2.0 unx     6565 b- defN 24-Apr-29 09:40 nucliadb/writer/api/v1/export_import.py
--rw-r--r--  2.0 unx    24419 b- defN 24-Apr-29 09:40 nucliadb/writer/api/v1/field.py
--rw-r--r--  2.0 unx     5239 b- defN 24-Apr-29 09:40 nucliadb/writer/api/v1/knowledgebox.py
--rw-r--r--  2.0 unx     2052 b- defN 24-Apr-29 09:40 nucliadb/writer/api/v1/learning_config.py
--rw-r--r--  2.0 unx    18869 b- defN 24-Apr-29 09:40 nucliadb/writer/api/v1/resource.py
--rw-r--r--  2.0 unx     1034 b- defN 24-Apr-29 09:40 nucliadb/writer/api/v1/router.py
--rw-r--r--  2.0 unx    10726 b- defN 24-Apr-29 09:40 nucliadb/writer/api/v1/services.py
--rw-r--r--  2.0 unx    30722 b- defN 24-Apr-29 09:40 nucliadb/writer/api/v1/upload.py
--rw-r--r--  2.0 unx     1612 b- defN 24-Apr-29 09:40 nucliadb/writer/layouts/__init__.py
--rw-r--r--  2.0 unx     2115 b- defN 24-Apr-29 09:40 nucliadb/writer/layouts/v1.py
--rw-r--r--  2.0 unx      835 b- defN 24-Apr-29 09:40 nucliadb/writer/resource/__init__.py
--rw-r--r--  2.0 unx     1425 b- defN 24-Apr-29 09:40 nucliadb/writer/resource/audit.py
--rw-r--r--  2.0 unx    10968 b- defN 24-Apr-29 09:40 nucliadb/writer/resource/basic.py
--rw-r--r--  2.0 unx    16319 b- defN 24-Apr-29 09:40 nucliadb/writer/resource/field.py
--rw-r--r--  2.0 unx     2022 b- defN 24-Apr-29 09:40 nucliadb/writer/resource/origin.py
--rw-r--r--  2.0 unx     1152 b- defN 24-Apr-29 09:40 nucliadb/writer/resource/slug.py
--rw-r--r--  2.0 unx      835 b- defN 24-Apr-29 09:40 nucliadb/writer/tests/__init__.py
--rw-r--r--  2.0 unx     1200 b- defN 24-Apr-29 09:40 nucliadb/writer/tests/conftest.py
--rw-r--r--  2.0 unx     5971 b- defN 24-Apr-29 09:40 nucliadb/writer/tests/fixtures.py
--rw-r--r--  2.0 unx    15472 b- defN 24-Apr-29 09:40 nucliadb/writer/tests/test_fields.py
--rw-r--r--  2.0 unx    25999 b- defN 24-Apr-29 09:40 nucliadb/writer/tests/test_files.py
--rw-r--r--  2.0 unx     1729 b- defN 24-Apr-29 09:40 nucliadb/writer/tests/test_knowledgebox.py
--rw-r--r--  2.0 unx     4358 b- defN 24-Apr-29 09:40 nucliadb/writer/tests/test_reprocess_file_field.py
--rw-r--r--  2.0 unx    16694 b- defN 24-Apr-29 09:40 nucliadb/writer/tests/test_resources.py
--rw-r--r--  2.0 unx     5120 b- defN 24-Apr-29 09:40 nucliadb/writer/tests/test_service.py
--rw-r--r--  2.0 unx     6054 b- defN 24-Apr-29 09:40 nucliadb/writer/tests/test_tus.py
--rw-r--r--  2.0 unx     1287 b- defN 24-Apr-29 09:40 nucliadb/writer/tests/utils.py
--rw-r--r--  2.0 unx     5226 b- defN 24-Apr-29 09:40 nucliadb/writer/tus/__init__.py
--rw-r--r--  2.0 unx     5082 b- defN 24-Apr-29 09:40 nucliadb/writer/tus/dm.py
--rw-r--r--  2.0 unx     2186 b- defN 24-Apr-29 09:40 nucliadb/writer/tus/exceptions.py
--rw-r--r--  2.0 unx    14527 b- defN 24-Apr-29 09:40 nucliadb/writer/tus/gcs.py
--rw-r--r--  2.0 unx     5849 b- defN 24-Apr-29 09:40 nucliadb/writer/tus/local.py
--rw-r--r--  2.0 unx     4367 b- defN 24-Apr-29 09:40 nucliadb/writer/tus/pg.py
--rw-r--r--  2.0 unx     9069 b- defN 24-Apr-29 09:40 nucliadb/writer/tus/s3.py
--rw-r--r--  2.0 unx     4734 b- defN 24-Apr-29 09:40 nucliadb/writer/tus/storage.py
--rw-r--r--  2.0 unx     2556 b- defN 24-Apr-29 09:40 nucliadb/writer/tus/utils.py
--rw-r--r--  2.0 unx     4343 b- defN 24-Apr-29 09:41 nucliadb-3.0.3.post460.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-29 09:41 nucliadb-3.0.3.post460.dist-info/WHEEL
--rw-r--r--  2.0 unx     1268 b- defN 24-Apr-29 09:41 nucliadb-3.0.3.post460.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       20 b- defN 24-Apr-29 09:41 nucliadb-3.0.3.post460.dist-info/top_level.txt
--rw-r--r--  2.0 unx        1 b- defN 24-Apr-29 09:41 nucliadb-3.0.3.post460.dist-info/zip-safe
--rw-rw-r--  2.0 unx    42679 b- defN 24-Apr-29 09:41 nucliadb-3.0.3.post460.dist-info/RECORD
-455 files, 2225108 bytes uncompressed, 683840 bytes compressed:  69.3%
+Zip file size: 748588 bytes, number of entries: 453
+-rw-r--r--  2.0 unx     1135 b- defN 24-May-07 11:35 migrations/0001_bootstrap.py
+-rw-r--r--  2.0 unx     1177 b- defN 24-May-07 11:35 migrations/0002_rollover_shards.py
+-rw-r--r--  2.0 unx     2436 b- defN 24-May-07 11:35 migrations/0003_allfields_key.py
+-rw-r--r--  2.0 unx     1177 b- defN 24-May-07 11:35 migrations/0004_rollover_shards.py
+-rw-r--r--  2.0 unx     1177 b- defN 24-May-07 11:35 migrations/0005_rollover_shards.py
+-rw-r--r--  2.0 unx     1024 b- defN 24-May-07 11:35 migrations/0006_rollover_shards.py
+-rw-r--r--  2.0 unx     1301 b- defN 24-May-07 11:35 migrations/0008_cleanup_leftover_rollover_metadata.py
+-rw-r--r--  2.0 unx     1378 b- defN 24-May-07 11:35 migrations/0009_upgrade_relations_and_texts_to_v2.py
+-rw-r--r--  2.0 unx     1610 b- defN 24-May-07 11:35 migrations/0010_fix_corrupt_indexes.py
+-rw-r--r--  2.0 unx     1843 b- defN 24-May-07 11:35 migrations/0011_materialize_labelset_ids.py
+-rw-r--r--  2.0 unx     1443 b- defN 24-May-07 11:35 migrations/0012_rollover_shards.py
+-rw-r--r--  2.0 unx     1024 b- defN 24-May-07 11:35 migrations/0013_rollover_shards.py
+-rw-r--r--  2.0 unx     1382 b- defN 24-May-07 11:35 migrations/0014_rollover_shards.py
+-rw-r--r--  2.0 unx     1462 b- defN 24-May-07 11:35 migrations/0015_targeted_rollover.py
+-rw-r--r--  2.0 unx     2506 b- defN 24-May-07 11:35 migrations/0016_upgrade_to_paragraphs_v2.py
+-rw-r--r--  2.0 unx     2100 b- defN 24-May-07 11:35 migrations/0017_multiple_writable_shards.py
+-rw-r--r--  2.0 unx     2264 b- defN 24-May-07 11:35 migrations/0018_purge_orphan_kbslugs.py
+-rw-r--r--  2.0 unx     2506 b- defN 24-May-07 11:35 migrations/0019_upgrade_to_paragraphs_v3.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-07 11:35 migrations/__init__.py
+-rw-r--r--  2.0 unx      891 b- defN 24-May-07 11:35 nucliadb/__init__.py
+-rw-r--r--  2.0 unx     3733 b- defN 24-May-07 11:35 nucliadb/health.py
+-rw-r--r--  2.0 unx    11626 b- defN 24-May-07 11:35 nucliadb/learning_proxy.py
+-rw-r--r--  2.0 unx     4806 b- defN 24-May-07 11:35 nucliadb/metrics_exporter.py
+-rw-r--r--  2.0 unx     2272 b- defN 24-May-07 11:35 nucliadb/openapi.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-07 11:35 nucliadb/py.typed
+-rw-r--r--  2.0 unx      835 b- defN 24-May-07 11:35 nucliadb/common/__init__.py
+-rw-r--r--  2.0 unx     4905 b- defN 24-May-07 11:35 nucliadb/common/locking.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-07 11:35 nucliadb/common/cluster/__init__.py
+-rw-r--r--  2.0 unx     4971 b- defN 24-May-07 11:35 nucliadb/common/cluster/base.py
+-rw-r--r--  2.0 unx     1495 b- defN 24-May-07 11:35 nucliadb/common/cluster/exceptions.py
+-rw-r--r--  2.0 unx     3790 b- defN 24-May-07 11:35 nucliadb/common/cluster/grpc_node_dummy.py
+-rw-r--r--  2.0 unx     3429 b- defN 24-May-07 11:35 nucliadb/common/cluster/index_node.py
+-rw-r--r--  2.0 unx    21584 b- defN 24-May-07 11:35 nucliadb/common/cluster/manager.py
+-rw-r--r--  2.0 unx     8490 b- defN 24-May-07 11:35 nucliadb/common/cluster/rebalance.py
+-rw-r--r--  2.0 unx    19549 b- defN 24-May-07 11:35 nucliadb/common/cluster/rollover.py
+-rw-r--r--  2.0 unx     2713 b- defN 24-May-07 11:35 nucliadb/common/cluster/settings.py
+-rw-r--r--  2.0 unx     5494 b- defN 24-May-07 11:35 nucliadb/common/cluster/utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-07 11:35 nucliadb/common/cluster/discovery/__init__.py
+-rw-r--r--  2.0 unx     6553 b- defN 24-May-07 11:35 nucliadb/common/cluster/discovery/base.py
+-rw-r--r--  2.0 unx    12518 b- defN 24-May-07 11:35 nucliadb/common/cluster/discovery/k8s.py
+-rw-r--r--  2.0 unx     1957 b- defN 24-May-07 11:35 nucliadb/common/cluster/discovery/manual.py
+-rw-r--r--  2.0 unx     1737 b- defN 24-May-07 11:35 nucliadb/common/cluster/discovery/single.py
+-rw-r--r--  2.0 unx     1139 b- defN 24-May-07 11:35 nucliadb/common/cluster/discovery/types.py
+-rw-r--r--  2.0 unx     2548 b- defN 24-May-07 11:35 nucliadb/common/cluster/discovery/utils.py
+-rw-r--r--  2.0 unx      833 b- defN 24-May-07 11:35 nucliadb/common/cluster/standalone/__init__.py
+-rw-r--r--  2.0 unx    13707 b- defN 24-May-07 11:35 nucliadb/common/cluster/standalone/grpc_node_binding.py
+-rw-r--r--  2.0 unx     4683 b- defN 24-May-07 11:35 nucliadb/common/cluster/standalone/index_node.py
+-rw-r--r--  2.0 unx     3444 b- defN 24-May-07 11:35 nucliadb/common/cluster/standalone/service.py
+-rw-r--r--  2.0 unx     3386 b- defN 24-May-07 11:35 nucliadb/common/cluster/standalone/utils.py
+-rw-r--r--  2.0 unx     3498 b- defN 24-May-07 11:35 nucliadb/common/context/__init__.py
+-rw-r--r--  2.0 unx     1628 b- defN 24-May-07 11:35 nucliadb/common/context/fastapi.py
+-rw-r--r--  2.0 unx     1813 b- defN 24-May-07 11:35 nucliadb/common/datamanagers/__init__.py
+-rw-r--r--  2.0 unx     1451 b- defN 24-May-07 11:35 nucliadb/common/datamanagers/cluster.py
+-rw-r--r--  2.0 unx     5383 b- defN 24-May-07 11:35 nucliadb/common/datamanagers/entities.py
+-rw-r--r--  2.0 unx      883 b- defN 24-May-07 11:35 nucliadb/common/datamanagers/exceptions.py
+-rw-r--r--  2.0 unx     3994 b- defN 24-May-07 11:35 nucliadb/common/datamanagers/kb.py
+-rw-r--r--  2.0 unx     5389 b- defN 24-May-07 11:35 nucliadb/common/datamanagers/labels.py
+-rw-r--r--  2.0 unx     1599 b- defN 24-May-07 11:35 nucliadb/common/datamanagers/processing.py
+-rw-r--r--  2.0 unx     8719 b- defN 24-May-07 11:35 nucliadb/common/datamanagers/resources.py
+-rw-r--r--  2.0 unx     5633 b- defN 24-May-07 11:35 nucliadb/common/datamanagers/rollover.py
+-rw-r--r--  2.0 unx     1631 b- defN 24-May-07 11:35 nucliadb/common/datamanagers/utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-07 11:35 nucliadb/common/http_clients/__init__.py
+-rw-r--r--  2.0 unx     2146 b- defN 24-May-07 11:35 nucliadb/common/http_clients/auth.py
+-rw-r--r--  2.0 unx     1100 b- defN 24-May-07 11:35 nucliadb/common/http_clients/exceptions.py
+-rw-r--r--  2.0 unx     7155 b- defN 24-May-07 11:35 nucliadb/common/http_clients/processing.py
+-rw-r--r--  2.0 unx     1540 b- defN 24-May-07 11:35 nucliadb/common/http_clients/pypi.py
+-rw-r--r--  2.0 unx     1551 b- defN 24-May-07 11:35 nucliadb/common/http_clients/utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-07 11:35 nucliadb/common/maindb/__init__.py
+-rw-r--r--  2.0 unx     3449 b- defN 24-May-07 11:35 nucliadb/common/maindb/driver.py
+-rw-r--r--  2.0 unx      946 b- defN 24-May-07 11:35 nucliadb/common/maindb/exceptions.py
+-rw-r--r--  2.0 unx     6769 b- defN 24-May-07 11:35 nucliadb/common/maindb/local.py
+-rw-r--r--  2.0 unx     8391 b- defN 24-May-07 11:35 nucliadb/common/maindb/pg.py
+-rw-r--r--  2.0 unx     6053 b- defN 24-May-07 11:35 nucliadb/common/maindb/redis.py
+-rw-r--r--  2.0 unx    14502 b- defN 24-May-07 11:35 nucliadb/common/maindb/tikv.py
+-rw-r--r--  2.0 unx     4109 b- defN 24-May-07 11:35 nucliadb/common/maindb/utils.py
+-rw-r--r--  2.0 unx      932 b- defN 24-May-07 11:35 nucliadb/export_import/__init__.py
+-rw-r--r--  2.0 unx     6171 b- defN 24-May-07 11:35 nucliadb/export_import/datamanager.py
+-rw-r--r--  2.0 unx     1949 b- defN 24-May-07 11:35 nucliadb/export_import/exceptions.py
+-rw-r--r--  2.0 unx     7116 b- defN 24-May-07 11:35 nucliadb/export_import/exporter.py
+-rw-r--r--  2.0 unx     4258 b- defN 24-May-07 11:35 nucliadb/export_import/importer.py
+-rw-r--r--  2.0 unx     2063 b- defN 24-May-07 11:35 nucliadb/export_import/models.py
+-rw-r--r--  2.0 unx     2571 b- defN 24-May-07 11:35 nucliadb/export_import/tasks.py
+-rw-r--r--  2.0 unx    19270 b- defN 24-May-07 11:35 nucliadb/export_import/utils.py
+-rw-r--r--  2.0 unx     1011 b- defN 24-May-07 11:35 nucliadb/ingest/__init__.py
+-rw-r--r--  2.0 unx     7277 b- defN 24-May-07 11:35 nucliadb/ingest/app.py
+-rw-r--r--  2.0 unx     1005 b- defN 24-May-07 11:35 nucliadb/ingest/cache.py
+-rw-r--r--  2.0 unx     2484 b- defN 24-May-07 11:35 nucliadb/ingest/partitions.py
+-rw-r--r--  2.0 unx    19541 b- defN 24-May-07 11:35 nucliadb/ingest/processing.py
+-rw-r--r--  2.0 unx    20277 b- defN 24-May-07 11:35 nucliadb/ingest/serialize.py
+-rw-r--r--  2.0 unx     3183 b- defN 24-May-07 11:35 nucliadb/ingest/settings.py
+-rw-r--r--  2.0 unx     2314 b- defN 24-May-07 11:35 nucliadb/ingest/utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-07 11:35 nucliadb/ingest/consumer/__init__.py
+-rw-r--r--  2.0 unx    11563 b- defN 24-May-07 11:35 nucliadb/ingest/consumer/auditing.py
+-rw-r--r--  2.0 unx    12159 b- defN 24-May-07 11:35 nucliadb/ingest/consumer/consumer.py
+-rw-r--r--  2.0 unx     3788 b- defN 24-May-07 11:35 nucliadb/ingest/consumer/materializer.py
+-rw-r--r--  2.0 unx     1075 b- defN 24-May-07 11:35 nucliadb/ingest/consumer/metrics.py
+-rw-r--r--  2.0 unx     9543 b- defN 24-May-07 11:35 nucliadb/ingest/consumer/pull.py
+-rw-r--r--  2.0 unx     6935 b- defN 24-May-07 11:35 nucliadb/ingest/consumer/service.py
+-rw-r--r--  2.0 unx     4331 b- defN 24-May-07 11:35 nucliadb/ingest/consumer/shard_creator.py
+-rw-r--r--  2.0 unx     2656 b- defN 24-May-07 11:35 nucliadb/ingest/consumer/utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-07 11:35 nucliadb/ingest/fields/__init__.py
+-rw-r--r--  2.0 unx    18433 b- defN 24-May-07 11:35 nucliadb/ingest/fields/base.py
+-rw-r--r--  2.0 unx     6516 b- defN 24-May-07 11:35 nucliadb/ingest/fields/conversation.py
+-rw-r--r--  2.0 unx     1223 b- defN 24-May-07 11:35 nucliadb/ingest/fields/date.py
+-rw-r--r--  2.0 unx     1205 b- defN 24-May-07 11:35 nucliadb/ingest/fields/exceptions.py
+-rw-r--r--  2.0 unx     5159 b- defN 24-May-07 11:35 nucliadb/ingest/fields/file.py
+-rw-r--r--  2.0 unx     1547 b- defN 24-May-07 11:35 nucliadb/ingest/fields/generic.py
+-rw-r--r--  2.0 unx     1235 b- defN 24-May-07 11:35 nucliadb/ingest/fields/keywordset.py
+-rw-r--r--  2.0 unx     2250 b- defN 24-May-07 11:35 nucliadb/ingest/fields/layout.py
+-rw-r--r--  2.0 unx     4084 b- defN 24-May-07 11:35 nucliadb/ingest/fields/link.py
+-rw-r--r--  2.0 unx     1319 b- defN 24-May-07 11:35 nucliadb/ingest/fields/text.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-07 11:35 nucliadb/ingest/orm/__init__.py
+-rw-r--r--  2.0 unx    28367 b- defN 24-May-07 11:35 nucliadb/ingest/orm/brain.py
+-rw-r--r--  2.0 unx    15758 b- defN 24-May-07 11:35 nucliadb/ingest/orm/entities.py
+-rw-r--r--  2.0 unx     1279 b- defN 24-May-07 11:35 nucliadb/ingest/orm/exceptions.py
+-rw-r--r--  2.0 unx    17167 b- defN 24-May-07 11:35 nucliadb/ingest/orm/knowledgebox.py
+-rw-r--r--  2.0 unx     1096 b- defN 24-May-07 11:35 nucliadb/ingest/orm/metrics.py
+-rw-r--r--  2.0 unx    60444 b- defN 24-May-07 11:35 nucliadb/ingest/orm/resource.py
+-rw-r--r--  2.0 unx     1739 b- defN 24-May-07 11:35 nucliadb/ingest/orm/synonyms.py
+-rw-r--r--  2.0 unx     3683 b- defN 24-May-07 11:35 nucliadb/ingest/orm/utils.py
+-rw-r--r--  2.0 unx    26423 b- defN 24-May-07 11:35 nucliadb/ingest/orm/processor/__init__.py
+-rw-r--r--  2.0 unx     1690 b- defN 24-May-07 11:35 nucliadb/ingest/orm/processor/sequence_manager.py
+-rw-r--r--  2.0 unx     2057 b- defN 24-May-07 11:35 nucliadb/ingest/service/__init__.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-07 11:35 nucliadb/ingest/service/exceptions.py
+-rw-r--r--  2.0 unx    33536 b- defN 24-May-07 11:35 nucliadb/ingest/service/writer.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-07 11:35 nucliadb/ingest/tests/__init__.py
+-rw-r--r--  2.0 unx     1157 b- defN 24-May-07 11:35 nucliadb/ingest/tests/conftest.py
+-rw-r--r--  2.0 unx    24060 b- defN 24-May-07 11:35 nucliadb/ingest/tests/fixtures.py
+-rw-r--r--  2.0 unx    62843 b- defN 24-May-07 11:35 nucliadb/ingest/tests/vectors.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-07 11:35 nucliadb/ingest/tests/integration/__init__.py
+-rw-r--r--  2.0 unx      833 b- defN 24-May-07 11:35 nucliadb/ingest/tests/integration/consumer/__init__.py
+-rw-r--r--  2.0 unx     2549 b- defN 24-May-07 11:35 nucliadb/ingest/tests/integration/consumer/test_auditing.py
+-rw-r--r--  2.0 unx     2591 b- defN 24-May-07 11:35 nucliadb/ingest/tests/integration/consumer/test_materializer.py
+-rw-r--r--  2.0 unx     4465 b- defN 24-May-07 11:35 nucliadb/ingest/tests/integration/consumer/test_pull.py
+-rw-r--r--  2.0 unx     2763 b- defN 24-May-07 11:35 nucliadb/ingest/tests/integration/consumer/test_service.py
+-rw-r--r--  2.0 unx     2019 b- defN 24-May-07 11:35 nucliadb/ingest/tests/integration/consumer/test_shard_creator.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-07 11:35 nucliadb/ingest/tests/integration/ingest/__init__.py
+-rw-r--r--  2.0 unx    27325 b- defN 24-May-07 11:35 nucliadb/ingest/tests/integration/ingest/test_ingest.py
+-rw-r--r--  2.0 unx     3040 b- defN 24-May-07 11:35 nucliadb/ingest/tests/integration/ingest/test_processing_engine.py
+-rw-r--r--  2.0 unx     8586 b- defN 24-May-07 11:35 nucliadb/ingest/tests/integration/ingest/test_relations.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-07 11:35 nucliadb/ingest/tests/unit/__init__.py
+-rw-r--r--  2.0 unx     1189 b- defN 24-May-07 11:35 nucliadb/ingest/tests/unit/test_cache.py
+-rw-r--r--  2.0 unx     1432 b- defN 24-May-07 11:35 nucliadb/ingest/tests/unit/test_partitions.py
+-rw-r--r--  2.0 unx     5807 b- defN 24-May-07 11:35 nucliadb/ingest/tests/unit/test_processing.py
+-rw-r--r--  2.0 unx      978 b- defN 24-May-07 11:35 nucliadb/ingest/tests/unit/test_settings.py
+-rw-r--r--  2.0 unx      833 b- defN 24-May-07 11:35 nucliadb/ingest/tests/unit/consumer/__init__.py
+-rw-r--r--  2.0 unx     3981 b- defN 24-May-07 11:35 nucliadb/ingest/tests/unit/consumer/test_auditing.py
+-rw-r--r--  2.0 unx     2472 b- defN 24-May-07 11:35 nucliadb/ingest/tests/unit/consumer/test_consumer.py
+-rw-r--r--  2.0 unx     2063 b- defN 24-May-07 11:35 nucliadb/ingest/tests/unit/consumer/test_pull.py
+-rw-r--r--  2.0 unx     4075 b- defN 24-May-07 11:35 nucliadb/ingest/tests/unit/consumer/test_shard_creator.py
+-rw-r--r--  2.0 unx     1934 b- defN 24-May-07 11:35 nucliadb/ingest/tests/unit/consumer/test_utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-07 11:35 nucliadb/ingest/tests/unit/orm/__init__.py
+-rw-r--r--  2.0 unx     9876 b- defN 24-May-07 11:35 nucliadb/ingest/tests/unit/orm/test_brain.py
+-rw-r--r--  2.0 unx     2435 b- defN 24-May-07 11:35 nucliadb/ingest/tests/unit/orm/test_brain_vectors.py
+-rw-r--r--  2.0 unx     1174 b- defN 24-May-07 11:35 nucliadb/ingest/tests/unit/orm/test_orm_utils.py
+-rw-r--r--  2.0 unx     4045 b- defN 24-May-07 11:35 nucliadb/ingest/tests/unit/orm/test_processor.py
+-rw-r--r--  2.0 unx    11033 b- defN 24-May-07 11:35 nucliadb/ingest/tests/unit/orm/test_resource.py
+-rw-r--r--  2.0 unx     2216 b- defN 24-May-07 11:35 nucliadb/middleware/__init__.py
+-rw-r--r--  2.0 unx     3912 b- defN 24-May-07 11:35 nucliadb/middleware/transaction.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-07 11:35 nucliadb/migrator/__init__.py
+-rw-r--r--  2.0 unx     2119 b- defN 24-May-07 11:35 nucliadb/migrator/command.py
+-rw-r--r--  2.0 unx     1334 b- defN 24-May-07 11:35 nucliadb/migrator/context.py
+-rw-r--r--  2.0 unx     5104 b- defN 24-May-07 11:35 nucliadb/migrator/datamanager.py
+-rw-r--r--  2.0 unx      889 b- defN 24-May-07 11:35 nucliadb/migrator/exceptions.py
+-rw-r--r--  2.0 unx     9237 b- defN 24-May-07 11:35 nucliadb/migrator/migrator.py
+-rw-r--r--  2.0 unx     1145 b- defN 24-May-07 11:35 nucliadb/migrator/models.py
+-rw-r--r--  2.0 unx     1110 b- defN 24-May-07 11:35 nucliadb/migrator/settings.py
+-rw-r--r--  2.0 unx     2346 b- defN 24-May-07 11:35 nucliadb/migrator/utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-07 11:35 nucliadb/models/__init__.py
+-rw-r--r--  2.0 unx     1599 b- defN 24-May-07 11:35 nucliadb/models/responses.py
+-rw-r--r--  2.0 unx     6041 b- defN 24-May-07 11:35 nucliadb/purge/__init__.py
+-rw-r--r--  2.0 unx     9364 b- defN 24-May-07 11:35 nucliadb/purge/orphan_shards.py
+-rw-r--r--  2.0 unx     1328 b- defN 24-May-07 11:35 nucliadb/reader/__init__.py
+-rw-r--r--  2.0 unx     3709 b- defN 24-May-07 11:35 nucliadb/reader/app.py
+-rw-r--r--  2.0 unx     1366 b- defN 24-May-07 11:35 nucliadb/reader/lifecycle.py
+-rw-r--r--  2.0 unx     1031 b- defN 24-May-07 11:35 nucliadb/reader/openapi.py
+-rw-r--r--  2.0 unx     1447 b- defN 24-May-07 11:35 nucliadb/reader/run.py
+-rw-r--r--  2.0 unx      872 b- defN 24-May-07 11:35 nucliadb/reader/api/__init__.py
+-rw-r--r--  2.0 unx     2434 b- defN 24-May-07 11:35 nucliadb/reader/api/models.py
+-rw-r--r--  2.0 unx     1110 b- defN 24-May-07 11:35 nucliadb/reader/api/v1/__init__.py
+-rw-r--r--  2.0 unx    12368 b- defN 24-May-07 11:35 nucliadb/reader/api/v1/download.py
+-rw-r--r--  2.0 unx     6450 b- defN 24-May-07 11:35 nucliadb/reader/api/v1/export_import.py
+-rw-r--r--  2.0 unx     3632 b- defN 24-May-07 11:35 nucliadb/reader/api/v1/knowledgebox.py
+-rw-r--r--  2.0 unx     2093 b- defN 24-May-07 11:35 nucliadb/reader/api/v1/learning_collector.py
+-rw-r--r--  2.0 unx     4454 b- defN 24-May-07 11:35 nucliadb/reader/api/v1/learning_config.py
+-rw-r--r--  2.0 unx    13928 b- defN 24-May-07 11:35 nucliadb/reader/api/v1/resource.py
+-rw-r--r--  2.0 unx     1011 b- defN 24-May-07 11:35 nucliadb/reader/api/v1/router.py
+-rw-r--r--  2.0 unx    12378 b- defN 24-May-07 11:35 nucliadb/reader/api/v1/services.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-07 11:35 nucliadb/reader/reader/__init__.py
+-rw-r--r--  2.0 unx     8155 b- defN 24-May-07 11:35 nucliadb/reader/reader/notifications.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-07 11:35 nucliadb/reader/tests/__init__.py
+-rw-r--r--  2.0 unx     1224 b- defN 24-May-07 11:35 nucliadb/reader/tests/conftest.py
+-rw-r--r--  2.0 unx     4345 b- defN 24-May-07 11:35 nucliadb/reader/tests/fixtures.py
+-rw-r--r--  2.0 unx     2748 b- defN 24-May-07 11:35 nucliadb/reader/tests/test_list_resources.py
+-rw-r--r--  2.0 unx    10199 b- defN 24-May-07 11:35 nucliadb/reader/tests/test_reader_file_download.py
+-rw-r--r--  2.0 unx    10586 b- defN 24-May-07 11:35 nucliadb/reader/tests/test_reader_resource.py
+-rw-r--r--  2.0 unx     6535 b- defN 24-May-07 11:35 nucliadb/reader/tests/test_reader_resource_field.py
+-rw-r--r--  2.0 unx     1535 b- defN 24-May-07 11:35 nucliadb/search/__init__.py
+-rw-r--r--  2.0 unx     4905 b- defN 24-May-07 11:35 nucliadb/search/app.py
+-rw-r--r--  2.0 unx     1956 b- defN 24-May-07 11:35 nucliadb/search/lifecycle.py
+-rw-r--r--  2.0 unx     1016 b- defN 24-May-07 11:35 nucliadb/search/openapi.py
+-rw-r--r--  2.0 unx    17332 b- defN 24-May-07 11:35 nucliadb/search/predict.py
+-rw-r--r--  2.0 unx     1402 b- defN 24-May-07 11:35 nucliadb/search/run.py
+-rw-r--r--  2.0 unx     1193 b- defN 24-May-07 11:35 nucliadb/search/settings.py
+-rw-r--r--  2.0 unx     1037 b- defN 24-May-07 11:35 nucliadb/search/utilities.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-07 11:35 nucliadb/search/api/__init__.py
+-rw-r--r--  2.0 unx     1222 b- defN 24-May-07 11:35 nucliadb/search/api/v1/__init__.py
+-rw-r--r--  2.0 unx     9913 b- defN 24-May-07 11:35 nucliadb/search/api/v1/chat.py
+-rw-r--r--  2.0 unx     2665 b- defN 24-May-07 11:35 nucliadb/search/api/v1/feedback.py
+-rw-r--r--  2.0 unx     8804 b- defN 24-May-07 11:35 nucliadb/search/api/v1/find.py
+-rw-r--r--  2.0 unx     6938 b- defN 24-May-07 11:35 nucliadb/search/api/v1/knowledgebox.py
+-rw-r--r--  2.0 unx     3041 b- defN 24-May-07 11:35 nucliadb/search/api/v1/predict_proxy.py
+-rw-r--r--  2.0 unx      988 b- defN 24-May-07 11:35 nucliadb/search/api/v1/router.py
+-rw-r--r--  2.0 unx    18325 b- defN 24-May-07 11:35 nucliadb/search/api/v1/search.py
+-rw-r--r--  2.0 unx     5928 b- defN 24-May-07 11:35 nucliadb/search/api/v1/suggest.py
+-rw-r--r--  2.0 unx     2536 b- defN 24-May-07 11:35 nucliadb/search/api/v1/summarize.py
+-rw-r--r--  2.0 unx     1433 b- defN 24-May-07 11:35 nucliadb/search/api/v1/utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-07 11:35 nucliadb/search/api/v1/resource/__init__.py
+-rw-r--r--  2.0 unx     5887 b- defN 24-May-07 11:35 nucliadb/search/api/v1/resource/chat.py
+-rw-r--r--  2.0 unx     5293 b- defN 24-May-07 11:35 nucliadb/search/api/v1/resource/search.py
+-rw-r--r--  2.0 unx      833 b- defN 24-May-07 11:35 nucliadb/search/requesters/__init__.py
+-rw-r--r--  2.0 unx     9070 b- defN 24-May-07 11:35 nucliadb/search/requesters/utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-07 11:35 nucliadb/search/search/__init__.py
+-rw-r--r--  2.0 unx     2746 b- defN 24-May-07 11:35 nucliadb/search/search/cache.py
+-rw-r--r--  2.0 unx     1154 b- defN 24-May-07 11:35 nucliadb/search/search/exceptions.py
+-rw-r--r--  2.0 unx     5465 b- defN 24-May-07 11:35 nucliadb/search/search/fetch.py
+-rw-r--r--  2.0 unx     6513 b- defN 24-May-07 11:35 nucliadb/search/search/filters.py
+-rw-r--r--  2.0 unx     4612 b- defN 24-May-07 11:35 nucliadb/search/search/find.py
+-rw-r--r--  2.0 unx    17152 b- defN 24-May-07 11:35 nucliadb/search/search/find_merge.py
+-rw-r--r--  2.0 unx    21282 b- defN 24-May-07 11:35 nucliadb/search/search/merge.py
+-rw-r--r--  2.0 unx     1130 b- defN 24-May-07 11:35 nucliadb/search/search/metrics.py
+-rw-r--r--  2.0 unx     8698 b- defN 24-May-07 11:35 nucliadb/search/search/paragraphs.py
+-rw-r--r--  2.0 unx     3026 b- defN 24-May-07 11:35 nucliadb/search/search/predict_proxy.py
+-rw-r--r--  2.0 unx    31567 b- defN 24-May-07 11:35 nucliadb/search/search/query.py
+-rw-r--r--  2.0 unx     3018 b- defN 24-May-07 11:35 nucliadb/search/search/shards.py
+-rw-r--r--  2.0 unx     5101 b- defN 24-May-07 11:35 nucliadb/search/search/summarize.py
+-rw-r--r--  2.0 unx     2438 b- defN 24-May-07 11:35 nucliadb/search/search/utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-07 11:35 nucliadb/search/search/chat/__init__.py
+-rw-r--r--  2.0 unx     2058 b- defN 24-May-07 11:35 nucliadb/search/search/chat/images.py
+-rw-r--r--  2.0 unx    20793 b- defN 24-May-07 11:35 nucliadb/search/search/chat/prompt.py
+-rw-r--r--  2.0 unx    15347 b- defN 24-May-07 11:35 nucliadb/search/search/chat/query.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-07 11:35 nucliadb/search/tests/__init__.py
+-rw-r--r--  2.0 unx     1295 b- defN 24-May-07 11:35 nucliadb/search/tests/conftest.py
+-rw-r--r--  2.0 unx     6578 b- defN 24-May-07 11:35 nucliadb/search/tests/fixtures.py
+-rw-r--r--  2.0 unx    15480 b- defN 24-May-07 11:35 nucliadb/search/tests/node.py
+-rw-r--r--  2.0 unx      833 b- defN 24-May-07 11:35 nucliadb/search/tests/unit/__init__.py
+-rw-r--r--  2.0 unx     2649 b- defN 24-May-07 11:35 nucliadb/search/tests/unit/test_app.py
+-rw-r--r--  2.0 unx     3374 b- defN 24-May-07 11:35 nucliadb/search/tests/unit/test_find_merge.py
+-rw-r--r--  2.0 unx     1400 b- defN 24-May-07 11:35 nucliadb/search/tests/unit/test_merge.py
+-rw-r--r--  2.0 unx    13101 b- defN 24-May-07 11:35 nucliadb/search/tests/unit/test_predict.py
+-rw-r--r--  2.0 unx     1317 b- defN 24-May-07 11:35 nucliadb/search/tests/unit/test_run.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-07 11:35 nucliadb/search/tests/unit/api/__init__.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-07 11:35 nucliadb/search/tests/unit/api/v1/__init__.py
+-rw-r--r--  2.0 unx     2966 b- defN 24-May-07 11:35 nucliadb/search/tests/unit/api/v1/test_chat.py
+-rw-r--r--  2.0 unx     2865 b- defN 24-May-07 11:35 nucliadb/search/tests/unit/api/v1/test_predict_proxy.py
+-rw-r--r--  2.0 unx     2901 b- defN 24-May-07 11:35 nucliadb/search/tests/unit/api/v1/test_summarize.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-07 11:35 nucliadb/search/tests/unit/api/v1/resource/__init__.py
+-rw-r--r--  2.0 unx     3040 b- defN 24-May-07 11:35 nucliadb/search/tests/unit/api/v1/resource/test_chat.py
+-rw-r--r--  2.0 unx      833 b- defN 24-May-07 11:35 nucliadb/search/tests/unit/search/__init__.py
+-rw-r--r--  2.0 unx     8567 b- defN 24-May-07 11:35 nucliadb/search/tests/unit/search/test_chat_prompt.py
+-rw-r--r--  2.0 unx     3736 b- defN 24-May-07 11:35 nucliadb/search/tests/unit/search/test_fetch.py
+-rw-r--r--  2.0 unx     4306 b- defN 24-May-07 11:35 nucliadb/search/tests/unit/search/test_filters.py
+-rw-r--r--  2.0 unx     4492 b- defN 24-May-07 11:35 nucliadb/search/tests/unit/search/test_paragraphs.py
+-rw-r--r--  2.0 unx     3496 b- defN 24-May-07 11:35 nucliadb/search/tests/unit/search/test_predict_proxy.py
+-rw-r--r--  2.0 unx     7001 b- defN 24-May-07 11:35 nucliadb/search/tests/unit/search/test_query.py
+-rw-r--r--  2.0 unx      833 b- defN 24-May-07 11:35 nucliadb/search/tests/unit/search/requesters/__init__.py
+-rw-r--r--  2.0 unx     6455 b- defN 24-May-07 11:35 nucliadb/search/tests/unit/search/requesters/test_utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-07 11:35 nucliadb/search/tests/unit/search/search/__init__.py
+-rw-r--r--  2.0 unx     1759 b- defN 24-May-07 11:35 nucliadb/search/tests/unit/search/search/test_shards.py
+-rw-r--r--  2.0 unx     2511 b- defN 24-May-07 11:35 nucliadb/search/tests/unit/search/search/test_utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-07 11:35 nucliadb/standalone/__init__.py
+-rw-r--r--  2.0 unx     6746 b- defN 24-May-07 11:35 nucliadb/standalone/api_router.py
+-rw-r--r--  2.0 unx     5763 b- defN 24-May-07 11:35 nucliadb/standalone/app.py
+-rw-r--r--  2.0 unx     7800 b- defN 24-May-07 11:35 nucliadb/standalone/auth.py
+-rw-r--r--  2.0 unx     5309 b- defN 24-May-07 11:35 nucliadb/standalone/config.py
+-rw-r--r--  2.0 unx     6930 b- defN 24-May-07 11:35 nucliadb/standalone/introspect.py
+-rw-r--r--  2.0 unx     2488 b- defN 24-May-07 11:35 nucliadb/standalone/lifecycle.py
+-rw-r--r--  2.0 unx     1317 b- defN 24-May-07 11:35 nucliadb/standalone/purge.py
+-rw-r--r--  2.0 unx     5336 b- defN 24-May-07 11:35 nucliadb/standalone/run.py
+-rw-r--r--  2.0 unx     5781 b- defN 24-May-07 11:35 nucliadb/standalone/settings.py
+-rw-r--r--  2.0 unx     3132 b- defN 24-May-07 11:35 nucliadb/standalone/versions.py
+-rw-r--r--  2.0 unx     2285 b- defN 24-May-07 11:35 nucliadb/standalone/static/favicon.ico
+-rw-r--r--  2.0 unx     3833 b- defN 24-May-07 11:35 nucliadb/standalone/static/index.html
+-rw-r--r--  2.0 unx     2639 b- defN 24-May-07 11:35 nucliadb/standalone/static/logo.svg
+-rw-r--r--  2.0 unx      835 b- defN 24-May-07 11:35 nucliadb/standalone/tests/__init__.py
+-rw-r--r--  2.0 unx     1294 b- defN 24-May-07 11:35 nucliadb/standalone/tests/conftest.py
+-rw-r--r--  2.0 unx     1319 b- defN 24-May-07 11:35 nucliadb/standalone/tests/fixtures.py
+-rw-r--r--  2.0 unx      833 b- defN 24-May-07 11:35 nucliadb/standalone/tests/unit/__init__.py
+-rw-r--r--  2.0 unx     1722 b- defN 24-May-07 11:35 nucliadb/standalone/tests/unit/test_api_router.py
+-rw-r--r--  2.0 unx     5509 b- defN 24-May-07 11:35 nucliadb/standalone/tests/unit/test_auth.py
+-rw-r--r--  2.0 unx     1334 b- defN 24-May-07 11:35 nucliadb/standalone/tests/unit/test_introspect.py
+-rw-r--r--  2.0 unx     1472 b- defN 24-May-07 11:35 nucliadb/standalone/tests/unit/test_run.py
+-rw-r--r--  2.0 unx     1972 b- defN 24-May-07 11:35 nucliadb/standalone/tests/unit/test_versions.py
+-rw-r--r--  2.0 unx     1037 b- defN 24-May-07 11:35 nucliadb/tasks/__init__.py
+-rw-r--r--  2.0 unx     7655 b- defN 24-May-07 11:35 nucliadb/tasks/consumer.py
+-rw-r--r--  2.0 unx      924 b- defN 24-May-07 11:35 nucliadb/tasks/logger.py
+-rw-r--r--  2.0 unx     1378 b- defN 24-May-07 11:35 nucliadb/tasks/models.py
+-rw-r--r--  2.0 unx     3457 b- defN 24-May-07 11:35 nucliadb/tasks/producer.py
+-rw-r--r--  2.0 unx     1753 b- defN 24-May-07 11:35 nucliadb/tasks/registry.py
+-rw-r--r--  2.0 unx     1360 b- defN 24-May-07 11:35 nucliadb/tasks/utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-07 11:35 nucliadb/tests/__init__.py
+-rw-r--r--  2.0 unx     1229 b- defN 24-May-07 11:35 nucliadb/tests/conftest.py
+-rw-r--r--  2.0 unx    22365 b- defN 24-May-07 11:35 nucliadb/tests/fixtures.py
+-rw-r--r--  2.0 unx     7549 b- defN 24-May-07 11:35 nucliadb/tests/tikv.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-07 11:35 nucliadb/tests/benchmarks/__init__.py
+-rw-r--r--  2.0 unx     3032 b- defN 24-May-07 11:35 nucliadb/tests/benchmarks/test_search.py
+-rw-r--r--  2.0 unx      919 b- defN 24-May-07 11:35 nucliadb/tests/knowledgeboxes/__init__.py
+-rw-r--r--  2.0 unx     7002 b- defN 24-May-07 11:35 nucliadb/tests/knowledgeboxes/philosophy_books.py
+-rw-r--r--  2.0 unx     3037 b- defN 24-May-07 11:35 nucliadb/tests/knowledgeboxes/ten_dummy_resources.py
+-rw-r--r--  2.0 unx     1148 b- defN 24-May-07 11:35 nucliadb/tests/migrations/__init__.py
+-rw-r--r--  2.0 unx     2726 b- defN 24-May-07 11:35 nucliadb/tests/migrations/test_migration_0017.py
+-rw-r--r--  2.0 unx     3625 b- defN 24-May-07 11:35 nucliadb/tests/migrations/test_migration_0018.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-07 11:35 nucliadb/tests/unit/__init__.py
+-rw-r--r--  2.0 unx     1487 b- defN 24-May-07 11:35 nucliadb/tests/unit/test_field_ids.py
+-rw-r--r--  2.0 unx     2758 b- defN 24-May-07 11:35 nucliadb/tests/unit/test_health.py
+-rw-r--r--  2.0 unx     1543 b- defN 24-May-07 11:35 nucliadb/tests/unit/test_kb_slugs.py
+-rw-r--r--  2.0 unx     7892 b- defN 24-May-07 11:35 nucliadb/tests/unit/test_learning_proxy.py
+-rw-r--r--  2.0 unx     2642 b- defN 24-May-07 11:35 nucliadb/tests/unit/test_metrics_exporter.py
+-rw-r--r--  2.0 unx     1341 b- defN 24-May-07 11:35 nucliadb/tests/unit/test_openapi.py
+-rw-r--r--  2.0 unx     3656 b- defN 24-May-07 11:35 nucliadb/tests/unit/test_purge.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-07 11:35 nucliadb/tests/unit/common/__init__.py
+-rw-r--r--  2.0 unx     1268 b- defN 24-May-07 11:35 nucliadb/tests/unit/common/test_context.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-07 11:35 nucliadb/tests/unit/common/cluster/__init__.py
+-rw-r--r--  2.0 unx    11955 b- defN 24-May-07 11:35 nucliadb/tests/unit/common/cluster/test_cluster.py
+-rw-r--r--  2.0 unx     5387 b- defN 24-May-07 11:35 nucliadb/tests/unit/common/cluster/test_kb_shard_manager.py
+-rw-r--r--  2.0 unx     9470 b- defN 24-May-07 11:35 nucliadb/tests/unit/common/cluster/test_rollover.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-07 11:35 nucliadb/tests/unit/common/cluster/discovery/__init__.py
+-rw-r--r--  2.0 unx     5584 b- defN 24-May-07 11:35 nucliadb/tests/unit/common/cluster/discovery/test_k8s.py
+-rw-r--r--  2.0 unx      833 b- defN 24-May-07 11:35 nucliadb/tests/unit/common/cluster/standalone/__init__.py
+-rw-r--r--  2.0 unx     3750 b- defN 24-May-07 11:35 nucliadb/tests/unit/common/cluster/standalone/test_service.py
+-rw-r--r--  2.0 unx     2114 b- defN 24-May-07 11:35 nucliadb/tests/unit/common/cluster/standalone/test_utils.py
+-rw-r--r--  2.0 unx      833 b- defN 24-May-07 11:35 nucliadb/tests/unit/common/maindb/__init__.py
+-rw-r--r--  2.0 unx     3579 b- defN 24-May-07 11:35 nucliadb/tests/unit/common/maindb/test_driver.py
+-rw-r--r--  2.0 unx     1869 b- defN 24-May-07 11:35 nucliadb/tests/unit/common/maindb/test_tikv.py
+-rw-r--r--  2.0 unx     2998 b- defN 24-May-07 11:35 nucliadb/tests/unit/common/maindb/test_utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-07 11:35 nucliadb/tests/unit/export_import/__init__.py
+-rw-r--r--  2.0 unx     1435 b- defN 24-May-07 11:35 nucliadb/tests/unit/export_import/test_datamanager.py
+-rw-r--r--  2.0 unx     9706 b- defN 24-May-07 11:35 nucliadb/tests/unit/export_import/test_utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-07 11:35 nucliadb/tests/unit/migrator/__init__.py
+-rw-r--r--  2.0 unx     3233 b- defN 24-May-07 11:35 nucliadb/tests/unit/migrator/test_migrator.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-07 11:35 nucliadb/tests/unit/tasks/__init__.py
+-rw-r--r--  2.0 unx     1375 b- defN 24-May-07 11:35 nucliadb/tests/unit/tasks/conftest.py
+-rw-r--r--  2.0 unx     2714 b- defN 24-May-07 11:35 nucliadb/tests/unit/tasks/test_consumer.py
+-rw-r--r--  2.0 unx     3189 b- defN 24-May-07 11:35 nucliadb/tests/unit/tasks/test_producer.py
+-rw-r--r--  2.0 unx     1827 b- defN 24-May-07 11:35 nucliadb/tests/unit/tasks/test_tasks.py
+-rw-r--r--  2.0 unx     2507 b- defN 24-May-07 11:35 nucliadb/tests/utils/__init__.py
+-rw-r--r--  2.0 unx     1797 b- defN 24-May-07 11:35 nucliadb/tests/utils/aiohttp_session.py
+-rw-r--r--  2.0 unx     2533 b- defN 24-May-07 11:35 nucliadb/tests/utils/entities.py
+-rw-r--r--  2.0 unx     6327 b- defN 24-May-07 11:35 nucliadb/tests/utils/broker_messages/__init__.py
+-rw-r--r--  2.0 unx     7557 b- defN 24-May-07 11:35 nucliadb/tests/utils/broker_messages/fields.py
+-rw-r--r--  2.0 unx     1196 b- defN 24-May-07 11:35 nucliadb/tests/utils/broker_messages/helpers.py
+-rw-r--r--  2.0 unx     1325 b- defN 24-May-07 11:35 nucliadb/train/__init__.py
+-rw-r--r--  2.0 unx     3530 b- defN 24-May-07 11:35 nucliadb/train/app.py
+-rw-r--r--  2.0 unx     3800 b- defN 24-May-07 11:35 nucliadb/train/generator.py
+-rw-r--r--  2.0 unx     1698 b- defN 24-May-07 11:35 nucliadb/train/lifecycle.py
+-rw-r--r--  2.0 unx     1198 b- defN 24-May-07 11:35 nucliadb/train/models.py
+-rw-r--r--  2.0 unx     5706 b- defN 24-May-07 11:35 nucliadb/train/nodes.py
+-rw-r--r--  2.0 unx     1400 b- defN 24-May-07 11:35 nucliadb/train/run.py
+-rw-r--r--  2.0 unx     5926 b- defN 24-May-07 11:35 nucliadb/train/servicer.py
+-rw-r--r--  2.0 unx     1415 b- defN 24-May-07 11:35 nucliadb/train/settings.py
+-rw-r--r--  2.0 unx     1496 b- defN 24-May-07 11:35 nucliadb/train/types.py
+-rw-r--r--  2.0 unx     3265 b- defN 24-May-07 11:35 nucliadb/train/upload.py
+-rw-r--r--  2.0 unx     6420 b- defN 24-May-07 11:35 nucliadb/train/uploader.py
+-rw-r--r--  2.0 unx     3179 b- defN 24-May-07 11:35 nucliadb/train/utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-07 11:35 nucliadb/train/api/__init__.py
+-rw-r--r--  2.0 unx     1479 b- defN 24-May-07 11:35 nucliadb/train/api/utils.py
+-rw-r--r--  2.0 unx      928 b- defN 24-May-07 11:35 nucliadb/train/api/v1/__init__.py
+-rw-r--r--  2.0 unx     2065 b- defN 24-May-07 11:35 nucliadb/train/api/v1/check.py
+-rw-r--r--  2.0 unx      910 b- defN 24-May-07 11:35 nucliadb/train/api/v1/router.py
+-rw-r--r--  2.0 unx     1905 b- defN 24-May-07 11:35 nucliadb/train/api/v1/shards.py
+-rw-r--r--  2.0 unx     2129 b- defN 24-May-07 11:35 nucliadb/train/api/v1/trainset.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-07 11:35 nucliadb/train/generators/__init__.py
+-rw-r--r--  2.0 unx     3723 b- defN 24-May-07 11:35 nucliadb/train/generators/field_classifier.py
+-rw-r--r--  2.0 unx     6712 b- defN 24-May-07 11:35 nucliadb/train/generators/image_classifier.py
+-rw-r--r--  2.0 unx     2789 b- defN 24-May-07 11:35 nucliadb/train/generators/paragraph_classifier.py
+-rw-r--r--  2.0 unx     3590 b- defN 24-May-07 11:35 nucliadb/train/generators/paragraph_streaming.py
+-rw-r--r--  2.0 unx     5372 b- defN 24-May-07 11:35 nucliadb/train/generators/question_answer_streaming.py
+-rw-r--r--  2.0 unx     5160 b- defN 24-May-07 11:35 nucliadb/train/generators/sentence_classifier.py
+-rw-r--r--  2.0 unx    10446 b- defN 24-May-07 11:35 nucliadb/train/generators/token_classifier.py
+-rw-r--r--  2.0 unx     3877 b- defN 24-May-07 11:35 nucliadb/train/generators/utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-07 11:35 nucliadb/train/tests/__init__.py
+-rw-r--r--  2.0 unx     1125 b- defN 24-May-07 11:35 nucliadb/train/tests/conftest.py
+-rw-r--r--  2.0 unx    11053 b- defN 24-May-07 11:35 nucliadb/train/tests/fixtures.py
+-rw-r--r--  2.0 unx     4598 b- defN 24-May-07 11:35 nucliadb/train/tests/test_field_classification.py
+-rw-r--r--  2.0 unx     2729 b- defN 24-May-07 11:35 nucliadb/train/tests/test_get_entities.py
+-rw-r--r--  2.0 unx     1876 b- defN 24-May-07 11:35 nucliadb/train/tests/test_get_info.py
+-rw-r--r--  2.0 unx     1382 b- defN 24-May-07 11:35 nucliadb/train/tests/test_get_ontology.py
+-rw-r--r--  2.0 unx     2417 b- defN 24-May-07 11:35 nucliadb/train/tests/test_get_ontology_count.py
+-rw-r--r--  2.0 unx     7669 b- defN 24-May-07 11:35 nucliadb/train/tests/test_image_classification.py
+-rw-r--r--  2.0 unx     1416 b- defN 24-May-07 11:35 nucliadb/train/tests/test_list_fields.py
+-rw-r--r--  2.0 unx     2944 b- defN 24-May-07 11:35 nucliadb/train/tests/test_list_paragraphs.py
+-rw-r--r--  2.0 unx     1423 b- defN 24-May-07 11:35 nucliadb/train/tests/test_list_resources.py
+-rw-r--r--  2.0 unx     2947 b- defN 24-May-07 11:35 nucliadb/train/tests/test_list_sentences.py
+-rw-r--r--  2.0 unx     4645 b- defN 24-May-07 11:35 nucliadb/train/tests/test_paragraph_classification.py
+-rw-r--r--  2.0 unx     4320 b- defN 24-May-07 11:35 nucliadb/train/tests/test_paragraph_streaming.py
+-rw-r--r--  2.0 unx     8751 b- defN 24-May-07 11:35 nucliadb/train/tests/test_question_answer_streaming.py
+-rw-r--r--  2.0 unx     5051 b- defN 24-May-07 11:35 nucliadb/train/tests/test_sentence_classification.py
+-rw-r--r--  2.0 unx     5583 b- defN 24-May-07 11:35 nucliadb/train/tests/test_token_classification.py
+-rw-r--r--  2.0 unx     3324 b- defN 24-May-07 11:35 nucliadb/train/tests/utils.py
+-rw-r--r--  2.0 unx     1328 b- defN 24-May-07 11:35 nucliadb/writer/__init__.py
+-rw-r--r--  2.0 unx     4268 b- defN 24-May-07 11:35 nucliadb/writer/app.py
+-rw-r--r--  2.0 unx    19495 b- defN 24-May-07 11:35 nucliadb/writer/back_pressure.py
+-rw-r--r--  2.0 unx      972 b- defN 24-May-07 11:35 nucliadb/writer/exceptions.py
+-rw-r--r--  2.0 unx     1953 b- defN 24-May-07 11:35 nucliadb/writer/lifecycle.py
+-rw-r--r--  2.0 unx     1032 b- defN 24-May-07 11:35 nucliadb/writer/openapi.py
+-rw-r--r--  2.0 unx     1448 b- defN 24-May-07 11:35 nucliadb/writer/run.py
+-rw-r--r--  2.0 unx     3074 b- defN 24-May-07 11:35 nucliadb/writer/settings.py
+-rw-r--r--  2.0 unx     1036 b- defN 24-May-07 11:35 nucliadb/writer/utilities.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-07 11:35 nucliadb/writer/api/__init__.py
+-rw-r--r--  2.0 unx     1429 b- defN 24-May-07 11:35 nucliadb/writer/api/constants.py
+-rw-r--r--  2.0 unx     1095 b- defN 24-May-07 11:35 nucliadb/writer/api/v1/__init__.py
+-rw-r--r--  2.0 unx     6565 b- defN 24-May-07 11:35 nucliadb/writer/api/v1/export_import.py
+-rw-r--r--  2.0 unx    24419 b- defN 24-May-07 11:35 nucliadb/writer/api/v1/field.py
+-rw-r--r--  2.0 unx     5239 b- defN 24-May-07 11:35 nucliadb/writer/api/v1/knowledgebox.py
+-rw-r--r--  2.0 unx     2052 b- defN 24-May-07 11:35 nucliadb/writer/api/v1/learning_config.py
+-rw-r--r--  2.0 unx    18869 b- defN 24-May-07 11:35 nucliadb/writer/api/v1/resource.py
+-rw-r--r--  2.0 unx     1034 b- defN 24-May-07 11:35 nucliadb/writer/api/v1/router.py
+-rw-r--r--  2.0 unx    10726 b- defN 24-May-07 11:35 nucliadb/writer/api/v1/services.py
+-rw-r--r--  2.0 unx    30722 b- defN 24-May-07 11:35 nucliadb/writer/api/v1/upload.py
+-rw-r--r--  2.0 unx     1612 b- defN 24-May-07 11:35 nucliadb/writer/layouts/__init__.py
+-rw-r--r--  2.0 unx     2115 b- defN 24-May-07 11:35 nucliadb/writer/layouts/v1.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-07 11:35 nucliadb/writer/resource/__init__.py
+-rw-r--r--  2.0 unx     1425 b- defN 24-May-07 11:35 nucliadb/writer/resource/audit.py
+-rw-r--r--  2.0 unx    10968 b- defN 24-May-07 11:35 nucliadb/writer/resource/basic.py
+-rw-r--r--  2.0 unx    16319 b- defN 24-May-07 11:35 nucliadb/writer/resource/field.py
+-rw-r--r--  2.0 unx     2022 b- defN 24-May-07 11:35 nucliadb/writer/resource/origin.py
+-rw-r--r--  2.0 unx     1152 b- defN 24-May-07 11:35 nucliadb/writer/resource/slug.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-07 11:35 nucliadb/writer/tests/__init__.py
+-rw-r--r--  2.0 unx     1200 b- defN 24-May-07 11:35 nucliadb/writer/tests/conftest.py
+-rw-r--r--  2.0 unx     5971 b- defN 24-May-07 11:35 nucliadb/writer/tests/fixtures.py
+-rw-r--r--  2.0 unx    15472 b- defN 24-May-07 11:35 nucliadb/writer/tests/test_fields.py
+-rw-r--r--  2.0 unx    25999 b- defN 24-May-07 11:35 nucliadb/writer/tests/test_files.py
+-rw-r--r--  2.0 unx     1729 b- defN 24-May-07 11:35 nucliadb/writer/tests/test_knowledgebox.py
+-rw-r--r--  2.0 unx     4358 b- defN 24-May-07 11:35 nucliadb/writer/tests/test_reprocess_file_field.py
+-rw-r--r--  2.0 unx    16694 b- defN 24-May-07 11:35 nucliadb/writer/tests/test_resources.py
+-rw-r--r--  2.0 unx     5120 b- defN 24-May-07 11:35 nucliadb/writer/tests/test_service.py
+-rw-r--r--  2.0 unx     6054 b- defN 24-May-07 11:35 nucliadb/writer/tests/test_tus.py
+-rw-r--r--  2.0 unx     1287 b- defN 24-May-07 11:35 nucliadb/writer/tests/utils.py
+-rw-r--r--  2.0 unx     5226 b- defN 24-May-07 11:35 nucliadb/writer/tus/__init__.py
+-rw-r--r--  2.0 unx     5082 b- defN 24-May-07 11:35 nucliadb/writer/tus/dm.py
+-rw-r--r--  2.0 unx     2186 b- defN 24-May-07 11:35 nucliadb/writer/tus/exceptions.py
+-rw-r--r--  2.0 unx    14527 b- defN 24-May-07 11:35 nucliadb/writer/tus/gcs.py
+-rw-r--r--  2.0 unx     5849 b- defN 24-May-07 11:35 nucliadb/writer/tus/local.py
+-rw-r--r--  2.0 unx     4367 b- defN 24-May-07 11:35 nucliadb/writer/tus/pg.py
+-rw-r--r--  2.0 unx     9069 b- defN 24-May-07 11:35 nucliadb/writer/tus/s3.py
+-rw-r--r--  2.0 unx     4734 b- defN 24-May-07 11:35 nucliadb/writer/tus/storage.py
+-rw-r--r--  2.0 unx     2556 b- defN 24-May-07 11:35 nucliadb/writer/tus/utils.py
+-rw-r--r--  2.0 unx     4399 b- defN 24-May-07 11:36 nucliadb-3.0.3.post478.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-07 11:36 nucliadb-3.0.3.post478.dist-info/WHEEL
+-rw-r--r--  2.0 unx     1268 b- defN 24-May-07 11:36 nucliadb-3.0.3.post478.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       20 b- defN 24-May-07 11:36 nucliadb-3.0.3.post478.dist-info/top_level.txt
+-rw-r--r--  2.0 unx        1 b- defN 24-May-07 11:36 nucliadb-3.0.3.post478.dist-info/zip-safe
+-rw-rw-r--  2.0 unx    42473 b- defN 24-May-07 11:36 nucliadb-3.0.3.post478.dist-info/RECORD
+453 files, 2214467 bytes uncompressed, 680672 bytes compressed:  69.3%
```

## zipnote {}

```diff
@@ -648,17 +648,14 @@
 
 Filename: nucliadb/search/api/v1/utils.py
 Comment: 
 
 Filename: nucliadb/search/api/v1/resource/__init__.py
 Comment: 
 
-Filename: nucliadb/search/api/v1/resource/ask.py
-Comment: 
-
 Filename: nucliadb/search/api/v1/resource/chat.py
 Comment: 
 
 Filename: nucliadb/search/api/v1/resource/search.py
 Comment: 
 
 Filename: nucliadb/search/requesters/__init__.py
@@ -768,17 +765,14 @@
 
 Filename: nucliadb/search/tests/unit/api/v1/test_summarize.py
 Comment: 
 
 Filename: nucliadb/search/tests/unit/api/v1/resource/__init__.py
 Comment: 
 
-Filename: nucliadb/search/tests/unit/api/v1/resource/test_ask.py
-Comment: 
-
 Filename: nucliadb/search/tests/unit/api/v1/resource/test_chat.py
 Comment: 
 
 Filename: nucliadb/search/tests/unit/search/__init__.py
 Comment: 
 
 Filename: nucliadb/search/tests/unit/search/test_chat_prompt.py
@@ -1341,26 +1335,26 @@
 
 Filename: nucliadb/writer/tus/storage.py
 Comment: 
 
 Filename: nucliadb/writer/tus/utils.py
 Comment: 
 
-Filename: nucliadb-3.0.3.post460.dist-info/METADATA
+Filename: nucliadb-3.0.3.post478.dist-info/METADATA
 Comment: 
 
-Filename: nucliadb-3.0.3.post460.dist-info/WHEEL
+Filename: nucliadb-3.0.3.post478.dist-info/WHEEL
 Comment: 
 
-Filename: nucliadb-3.0.3.post460.dist-info/entry_points.txt
+Filename: nucliadb-3.0.3.post478.dist-info/entry_points.txt
 Comment: 
 
-Filename: nucliadb-3.0.3.post460.dist-info/top_level.txt
+Filename: nucliadb-3.0.3.post478.dist-info/top_level.txt
 Comment: 
 
-Filename: nucliadb-3.0.3.post460.dist-info/zip-safe
+Filename: nucliadb-3.0.3.post478.dist-info/zip-safe
 Comment: 
 
-Filename: nucliadb-3.0.3.post460.dist-info/RECORD
+Filename: nucliadb-3.0.3.post478.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## nucliadb/common/cluster/grpc_node_dummy.py

```diff
@@ -54,21 +54,24 @@
         shards.append(ShardId(shard_id="shard"))
         shards.append(ShardId(shard_id="shard2"))
         return shards
 
     async def SetResource(self, data):  # pragma: no cover
         self.calls.setdefault("SetResource", []).append(data)
         result = OpStatus()
-        result.field_count = 1
+        return result
+
+    async def SetResourceFromStorage(self, data):  # pragma: no cover
+        self.calls.setdefault("SetResourceFromStorage", []).append(data)
+        result = OpStatus()
         return result
 
     async def AddVectorSet(self, data):  # pragma: no cover
         self.calls.setdefault("AddVectorSet", []).append(data)
         result = OpStatus()
-        result.field_count = 1
         return result
 
     async def ListVectorSet(self, data: ShardId):  # pragma: no cover
         self.calls.setdefault("ListVectorSet", []).append(data)
         result = VectorSetList()
         result.shard.id = data.id
         result.vectorset.append("base")
```

## nucliadb/common/cluster/manager.py

```diff
@@ -317,14 +317,17 @@
         resource: noderesources_pb2.Resource,
         txid: int,
         partition: str,
         kb: str,
         reindex_id: Optional[str] = None,
         source: IndexMessageSource.ValueType = IndexMessageSource.PROCESSOR,
     ) -> None:
+        """
+        Stores the Resource object in the object storage and sends an IndexMessage to the indexing Nats stream.
+        """
         if txid == -1 and reindex_id is None:
             # This means we are injecting a complete resource via ingest gRPC
             # outside of a transaction. We need to treat this as a reindex operation.
             reindex_id = uuid.uuid4().hex
 
         storage = await get_storage()
         indexing = get_indexing()
@@ -441,14 +444,18 @@
         resource: noderesources_pb2.Resource,
         txid: int,
         partition: str,
         kb: str,
         reindex_id: Optional[str] = None,
         source: IndexMessageSource.ValueType = IndexMessageSource.PROCESSOR,
     ) -> None:
+        """
+        Calls the node writer's SetResource method directly to store the resource in the node.
+        There is no queuing for standalone nodes at the moment -- indexing is done synchronously.
+        """
         index_node = None
         for shardreplica in shard.replicas:
             resource.shard_id = resource.resource.shard_id = shardreplica.shard.id
             index_node = get_index_node(shardreplica.node)
             if index_node is None:  # pragma: no cover
                 raise NodesUnsync(
                     f"Node {shardreplica.node} is not found or not available"
```

## nucliadb/common/cluster/rollover.py

```diff
@@ -407,27 +407,27 @@
                 kbid=kbid,
                 resource_id=resource_id,
                 shard_id=shard_id,
                 modification_time=-1,
             )
             await txn.commit()
 
-        # any left overs should be deleted
-        async for resource_id, (
-            shard_id,
-            last_indexed,
-        ) in datamanagers.rollover.iterate_indexed_data(kbid=kbid):
-            if last_indexed == -1:
-                continue
+    # any left overs should be deleted
+    async for resource_id, (
+        shard_id,
+        last_indexed,
+    ) in datamanagers.rollover.iterate_indexed_data(kbid=kbid):
+        if last_indexed == -1:
+            continue
 
-            shard = _get_shard(rolled_over_shards, shard_id)
-            if shard is None:
-                raise UnexpectedRolloverError("Shard not found. This should not happen")
+        shard = _get_shard(rolled_over_shards, shard_id)
+        if shard is None:
+            raise UnexpectedRolloverError("Shard not found. This should not happen")
 
-            await delete_resource_from_shard(app_context, kbid, resource_id, shard)
+        await delete_resource_from_shard(app_context, kbid, resource_id, shard)
 
     _set_rollover_status(rolled_over_shards, RolloverStatus.RESOURCES_VALIDATED)
     async with datamanagers.with_transaction() as txn:
         await datamanagers.cluster.update_kb_shards(
             txn, kbid=kbid, shards=rolled_over_shards
         )
```

## nucliadb/search/predict.py

```diff
@@ -26,15 +26,14 @@
 import aiohttp
 import backoff
 from nucliadb_protos.utils_pb2 import RelationNode
 
 from nucliadb.ingest.tests.vectors import Q, Qm2023
 from nucliadb.search import logger
 from nucliadb_models.search import (
-    AskDocumentModel,
     ChatModel,
     FeedbackRequest,
     Ner,
     QueryInfo,
     RephraseModel,
     SentenceSearch,
     SummarizedResource,
@@ -86,15 +85,14 @@
 PRIVATE_PREDICT = "/api/internal/predict"
 VERSIONED_PRIVATE_PREDICT = "/api/v1/internal/predict"
 SENTENCE = "/sentence"
 TOKENS = "/tokens"
 QUERY = "/query"
 SUMMARIZE = "/summarize"
 CHAT = "/chat"
-ASK_DOCUMENT = "/ask_document"
 REPHRASE = "/rephrase"
 FEEDBACK = "/feedback"
 
 NUCLIA_LEARNING_ID_HEADER = "NUCLIA-LEARNING-ID"
 
 
 predict_observer = metrics.Observer(
@@ -302,36 +300,14 @@
             headers=self.get_predict_headers(kbid),
             timeout=None,
         )
         await self.check_response(resp, expected_status=200)
         ident = resp.headers.get(NUCLIA_LEARNING_ID_HEADER)
         return ident, get_answer_generator(resp)
 
-    @predict_observer.wrap({"type": "ask_document"})
-    async def ask_document(
-        self, kbid: str, question: str, blocks: list[list[str]], user_id: str
-    ) -> str:
-        try:
-            self.check_nua_key_is_configured_for_onprem()
-        except NUAKeyMissingError:
-            error = "Nuclia Service account is not defined so could not ask document"
-            logger.warning(error)
-            raise SendToPredictError(error)
-
-        item = AskDocumentModel(question=question, blocks=blocks, user_id=user_id)
-        resp = await self.make_request(
-            "POST",
-            url=self.get_predict_url(ASK_DOCUMENT, kbid),
-            json=item.dict(),
-            headers=self.get_predict_headers(kbid),
-            timeout=None,
-        )
-        await self.check_response(resp, expected_status=200)
-        return await resp.text()
-
     @predict_observer.wrap({"type": "query"})
     async def query(
         self,
         kbid: str,
         sentence: str,
         generative_model: Optional[str] = None,
         rephrase: Optional[bool] = False,
@@ -453,21 +429,14 @@
 
         async def generate():
             for i in self.generated_answer:
                 yield i
 
         return (DUMMY_LEARNING_ID, generate())
 
-    async def ask_document(
-        self, kbid: str, query: str, blocks: list[list[str]], user_id: str
-    ) -> str:
-        self.calls.append(("ask_document", (query, blocks, user_id)))
-        answer = os.environ.get("TEST_ASK_DOCUMENT") or "Answer to your question"
-        return answer
-
     async def query(
         self,
         kbid: str,
         sentence: str,
         generative_model: Optional[str] = None,
         rephrase: Optional[bool] = False,
     ) -> QueryInfo:
```

## nucliadb/search/api/v1/__init__.py

```diff
@@ -21,11 +21,10 @@
 from . import feedback  # noqa
 from . import find  # noqa
 from . import knowledgebox  # noqa
 from . import predict_proxy  # noqa
 from . import search  # noqa
 from . import suggest  # noqa
 from . import summarize  # noqa
-from .resource import ask as ask_resource  # noqa
 from .resource import chat as chat_resource  # noqa
 from .resource import search as search_resource  # noqa
 from .router import api  # noqa
```

## nucliadb/search/api/v1/utils.py

```diff
@@ -32,11 +32,12 @@
         default_value = param.default
     else:
         default_value = default
     return Query(
         default=default_value,
         title=param.title,
         description=param.description,
+        le=param.le,
         gt=param.gt,
         max_length=param.max_items,
         **kw
     )
```

## nucliadb/search/search/query.py

```diff
@@ -64,14 +64,16 @@
 from .exceptions import InvalidQueryError
 
 INDEX_SORTABLE_FIELDS = [
     SortField.CREATED,
     SortField.MODIFIED,
 ]
 
+MAX_VECTOR_RESULTS_ALLOWED = 2000
+
 
 class QueryParser:
     """
     Queries are getting more and more complex and different phases of the query
     depending on different data.
 
     This class is an encapsulation of the different phases of the query and allow
@@ -142,14 +144,22 @@
         self.rephrase = rephrase
         self.query_endpoint_used = False
         if len(self.filters) > 0:
             self.filters = translate_label_filters(self.filters)
             self.flat_filter_labels = flat_filter_labels(self.filters)
         self.max_tokens = max_tokens
 
+    @property
+    def has_vector_search(self) -> bool:
+        return SearchOptions.VECTOR in self.features
+
+    @property
+    def has_relations_search(self) -> bool:
+        return SearchOptions.RELATIONS in self.features
+
     def _get_default_semantic_min_score(self) -> Awaitable[float]:
         if self._min_score_task is None:  # pragma: no cover
             self._min_score_task = asyncio.create_task(
                 get_default_semantic_min_score(self.kbid)
             )
         return self._min_score_task
 
@@ -212,22 +222,20 @@
         if len(self.filters) > 0 and has_classification_label_filters(
             self.flat_filter_labels
         ):
             asyncio.ensure_future(self._get_classification_labels())
         if self.min_score.semantic is None:
             asyncio.ensure_future(self._get_default_semantic_min_score())
 
-        if SearchOptions.VECTOR in self.features and self.user_vector is None:
+        if self.has_vector_search and self.user_vector is None:
             self.query_endpoint_used = True
             asyncio.ensure_future(self._get_query_information())
             asyncio.ensure_future(self._get_matryoshka_dimension())
 
-        if (SearchOptions.RELATIONS in self.features or self.autofilter) and len(
-            self.query
-        ) > 0:
+        if (self.has_relations_search or self.autofilter) and len(self.query) > 0:
             if not self.query_endpoint_used:
                 # If we only need to detect entities, we don't need the query endpoint
                 asyncio.ensure_future(self._get_detected_entities())
             asyncio.ensure_future(self._get_entities_meta_cache())
             asyncio.ensure_future(self._get_deleted_entity_groups())
         if self.with_synonyms and self.query:
             asyncio.ensure_future(self._get_synomyns())
@@ -240,24 +248,25 @@
                 - incomplete: If the query is incomplete (missing vectors)
                 - autofilters: The autofilters that were applied
         """
         request = nodereader_pb2.SearchRequest()
         request.body = self.query
         request.with_duplicates = self.with_duplicates
 
+        self.parse_sorting(request)
+
         await self._schedule_dependency_tasks()
 
         await self.parse_filters(request)
         self.parse_document_search(request)
         self.parse_paragraph_search(request)
         incomplete = await self.parse_vector_search(request)
         autofilters = await self.parse_relation_search(request)
         await self.parse_synonyms(request)
 
-        self.parse_sorting(request)
         await self.parse_min_score(request)
 
         return request, incomplete, autofilters
 
     async def parse_filters(self, request: nodereader_pb2.SearchRequest) -> None:
         if len(self.filters) > 0:
             field_labels = self.flat_filter_labels
@@ -343,14 +352,23 @@
             request.result_per_page = self.page_number * self.page_size + self.page_size
 
         sort_field = SortFieldMap[self.sort.field] if self.sort else None
         if sort_field is not None:
             request.order.sort_by = sort_field
             request.order.type = SortOrderMap[self.sort.order]  # type: ignore
 
+        if (
+            self.has_vector_search
+            and request.result_per_page > MAX_VECTOR_RESULTS_ALLOWED
+        ):
+            raise InvalidQueryError(
+                "page_size",
+                f"Pagination of semantic results limit reached: {MAX_VECTOR_RESULTS_ALLOWED}. If you want to paginate through all results, please disable the vector search feature.",  # noqa: E501
+            )
+
     async def parse_min_score(self, request: nodereader_pb2.SearchRequest) -> None:
         if self.min_score.semantic is None:
             self.min_score.semantic = await self._get_default_semantic_min_score()
         request.min_score_semantic = self.min_score.semantic
         request.min_score_bm25 = self.min_score.bm25
 
     def parse_document_search(self, request: nodereader_pb2.SearchRequest) -> None:
@@ -360,15 +378,15 @@
 
     def parse_paragraph_search(self, request: nodereader_pb2.SearchRequest) -> None:
         if SearchOptions.PARAGRAPH in self.features:
             request.paragraph = True
             node_features.inc({"type": "paragraphs"})
 
     async def parse_vector_search(self, request: nodereader_pb2.SearchRequest) -> bool:
-        if SearchOptions.VECTOR not in self.features:
+        if not self.has_vector_search:
             return False
 
         node_features.inc({"type": "vectors"})
 
         incomplete = False
         query_vector = None
         if self.user_vector is None:
@@ -393,29 +411,28 @@
             request.vector.extend(query_vector)
         return incomplete
 
     async def parse_relation_search(
         self, request: nodereader_pb2.SearchRequest
     ) -> list[str]:
         autofilters = []
-        relations_search = SearchOptions.RELATIONS in self.features
-        if relations_search or self.autofilter:
+        if self.has_relations_search or self.autofilter:
             if not self.query_endpoint_used:
                 detected_entities = await self._get_detected_entities()
             else:
                 query_info_result = await self._get_query_information()
                 if query_info_result.entities:
                     detected_entities = convert_relations(
                         query_info_result.entities.dict()
                     )
                 else:
                     detected_entities = []
             meta_cache = await self._get_entities_meta_cache()
             detected_entities = expand_entities(meta_cache, detected_entities)
-            if relations_search:
+            if self.has_relations_search:
                 request.relation_subgraph.entry_points.extend(detected_entities)
                 request.relation_subgraph.depth = 1
                 request.relation_subgraph.deleted_groups.extend(
                     await self._get_deleted_entity_groups()
                 )
                 for group_id, deleted_entities in meta_cache.deleted_entities.items():
                     request.relation_subgraph.deleted_entities.append(
@@ -431,18 +448,15 @@
                 )
         return autofilters
 
     async def parse_synonyms(self, request: nodereader_pb2.SearchRequest) -> None:
         if not self.with_synonyms:
             return
 
-        if (
-            SearchOptions.VECTOR in self.features
-            or SearchOptions.RELATIONS in self.features
-        ):
+        if self.has_vector_search or self.has_relations_search:
             raise InvalidQueryError(
                 "synonyms",
                 "Search with custom synonyms is only supported on paragraph and document search",
             )
 
         if not self.query:
             # Nothing to do
```

## nucliadb/search/tests/node.py

```diff
@@ -40,14 +40,15 @@
 
 logger = logging.getLogger(__name__)
 
 images.settings["nucliadb_node_reader"] = {
     "image": "europe-west4-docker.pkg.dev/nuclia-internal/nuclia/node",
     "version": "latest",
     "env": {
+        "FILE_BACKEND": "unset",
         "HOST_KEY_PATH": "/data/node.key",
         "DATA_PATH": "/data",
         "READER_LISTEN_ADDRESS": "0.0.0.0:4445",
         "NUCLIADB_DISABLE_ANALYTICS": "True",
         "RUST_BACKTRACE": "full",
         "RUST_LOG": "nucliadb_*=DEBUG",
     },
@@ -62,14 +63,15 @@
     },
 }
 
 images.settings["nucliadb_node_writer"] = {
     "image": "europe-west4-docker.pkg.dev/nuclia-internal/nuclia/node",
     "version": "latest",
     "env": {
+        "FILE_BACKEND": "unset",
         "HOST_KEY_PATH": "/data/node.key",
         "DATA_PATH": "/data",
         "WRITER_LISTEN_ADDRESS": "0.0.0.0:4446",
         "NUCLIADB_DISABLE_ANALYTICS": "True",
         "RUST_BACKTRACE": "full",
         "RUST_LOG": "nucliadb_*=DEBUG",
     },
@@ -318,28 +320,27 @@
                     "port": sidecar2_port,
                 },
             }
         )
         return self.data
 
     def stop(self):
-        container_ids = [
-            nucliadb_node_1_reader.container_obj.id,
-            nucliadb_node_1_writer.container_obj.id,
-            nucliadb_node_1_sidecar.container_obj.id,
-            nucliadb_node_2_writer.container_obj.id,
-            nucliadb_node_2_reader.container_obj.id,
-            nucliadb_node_2_sidecar.container_obj.id,
-        ]
-        nucliadb_node_1_reader.stop()
-        nucliadb_node_1_writer.stop()
-        nucliadb_node_1_sidecar.stop()
-        nucliadb_node_2_writer.stop()
-        nucliadb_node_2_reader.stop()
-        nucliadb_node_2_sidecar.stop()
+        container_ids = []
+        for component in [
+            nucliadb_node_1_reader,
+            nucliadb_node_1_writer,
+            nucliadb_node_1_sidecar,
+            nucliadb_node_2_writer,
+            nucliadb_node_2_reader,
+            nucliadb_node_2_sidecar,
+        ]:
+            container_obj = getattr(component, "container_obj", None)
+            if container_obj:
+                container_ids.append(container_obj.id)
+                component.stop()
 
         for container_id in container_ids:
             for _ in range(5):
                 try:
                     self.docker_client.containers.get(container_id)  # type: ignore
                 except docker.errors.NotFound:
                     break
```

## nucliadb/search/tests/unit/test_predict.py

```diff
@@ -32,15 +32,14 @@
     RephraseMissingContextError,
     SendToPredictError,
     _parse_rephrase_response,
     get_answer_generator,
 )
 from nucliadb.tests.utils.aiohttp_session import get_mocked_session
 from nucliadb_models.search import (
-    AskDocumentModel,
     ChatModel,
     FeedbackRequest,
     FeedbackTasks,
     RephraseModel,
     SummarizedResource,
     SummarizedResponse,
     SummarizeModel,
@@ -54,15 +53,14 @@
     pe = DummyPredictEngine()
     await pe.initialize()
     await pe.finalize()
     await pe.send_feedback("kbid", Mock(), "", "", "")
     assert await pe.rephrase_query("kbid", Mock())
     assert await pe.chat_query("kbid", Mock())
     assert await pe.detect_entities("kbid", "some sentence")
-    assert await pe.ask_document("kbid", "query", [["footext"]], "userid")
     assert await pe.summarize("kbid", Mock(resources={}))
 
 
 @pytest.mark.asyncio
 @pytest.mark.parametrize(
     "onprem,expected_url,expected_header,expected_header_value",
     [
@@ -153,15 +151,14 @@
                 FeedbackRequest(ident="foo", good=True, task=FeedbackTasks.CHAT),
                 "",
                 "",
                 "",
             ],
         ),
         ("rephrase_query", ["kbid", RephraseModel(question="foo", user_id="bar")]),
-        ("ask_document", ["kbid", "query", [["footext"]], "userid"]),
     ],
 )
 async def test_predict_engine_handles_limits_exceeded_error(
     session_limits_exceeded, method, args
 ):
     pe = PredictEngine(
         "cluster",
@@ -177,15 +174,14 @@
 @pytest.mark.parametrize(
     "method,args,exception,output",
     [
         ("chat_query", ["kbid", Mock()], True, None),
         ("rephrase_query", ["kbid", Mock()], True, None),
         ("send_feedback", ["kbid", MagicMock(), "", "", ""], False, None),
         ("detect_entities", ["kbid", "sentence"], False, []),
-        ("ask_document", ["kbid", "query", [["footext"]], "userid"], True, None),
         ("summarize", ["kbid", Mock(resources={})], True, None),
     ],
 )
 async def test_onprem_nuclia_service_account_not_configured(
     method, args, exception, output
 ):
     pe = PredictEngine(
@@ -197,65 +193,14 @@
     if exception:
         with pytest.raises(SendToPredictError):
             await getattr(pe, method)(*args)
     else:
         assert await getattr(pe, method)(*args) == output
 
 
-async def test_ask_document_onprem():
-    pe = PredictEngine(
-        "cluster",
-        "public-{zone}",
-        nuclia_service_account="foo",
-        zone="europe1",
-        onprem=True,
-    )
-    pe.session = get_mocked_session(
-        "POST", 200, text="The answer", context_manager=False
-    )
-
-    assert (
-        await pe.ask_document("kbid", "query", [["footext"]], "userid") == "The answer"
-    )
-
-    pe.session.post.assert_awaited_once_with(
-        url="public-europe1/api/v1/predict/ask_document/kbid",
-        json=AskDocumentModel(
-            question="query", blocks=[["footext"]], user_id="userid"
-        ).dict(),
-        headers={"X-STF-NUAKEY": "Bearer foo"},
-        timeout=None,
-    )
-
-
-async def test_ask_document_cloud():
-    pe = PredictEngine(
-        "cluster",
-        "public-{zone}",
-        zone="europe1",
-        onprem=False,
-    )
-    pe.session = get_mocked_session(
-        "POST", 200, text="The answer", context_manager=False
-    )
-
-    assert (
-        await pe.ask_document("kbid", "query", [["footext"]], "userid") == "The answer"
-    )
-
-    pe.session.post.assert_awaited_once_with(
-        url="cluster/api/v1/internal/predict/ask_document",
-        json=AskDocumentModel(
-            question="query", blocks=[["footext"]], user_id="userid"
-        ).dict(),
-        headers={"X-STF-KBID": "kbid"},
-        timeout=None,
-    )
-
-
 async def test_rephrase():
     pe = PredictEngine(
         "cluster",
         "public-{zone}",
         zone="europe1",
         onprem=False,
     )
```

## Comparing `nucliadb-3.0.3.post460.dist-info/METADATA` & `nucliadb-3.0.3.post478.dist-info/METADATA`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nucliadb
-Version: 3.0.3.post460
+Version: 3.0.3.post478
 Home-page: https://docs.nuclia.dev/docs/guides/nucliadb/intro
 Author: NucliaDB Community
 Author-email: nucliadb@nuclia.com
 License: BSD
 Project-URL: Nuclia, https://nuclia.com
 Project-URL: Github, https://github.com/nuclia/nucliadb
 Project-URL: Discord, https://discord.gg/8EvQwmsbzf
@@ -17,38 +17,38 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.9, <4
 Description-Content-Type: text/markdown
-Requires-Dist: nucliadb-telemetry[all] >=3.0.3.post460
-Requires-Dist: nucliadb-utils[cache,fastapi,storages] >=3.0.3.post460
-Requires-Dist: nucliadb-protos >=3.0.3.post460
-Requires-Dist: nucliadb-models >=3.0.3.post460
+Requires-Dist: nucliadb-telemetry[all] >=3.0.3.post478
+Requires-Dist: nucliadb-utils[cache,fastapi,storages] >=3.0.3.post478
+Requires-Dist: nucliadb-protos >=3.0.3.post478
+Requires-Dist: nucliadb-models >=3.0.3.post478
 Requires-Dist: nucliadb-admin-assets >=1.0.0.post1224
 Requires-Dist: nucliadb-node-binding >=2.26.0
 Requires-Dist: uvicorn <0.19.0
 Requires-Dist: pydantic-argparse
 Requires-Dist: aiohttp >=3.9.4
 Requires-Dist: lru-dict >=1.1.7
 Requires-Dist: backoff
 Requires-Dist: aiofiles >=0.8.0
 Requires-Dist: psutil >=5.9.7
 Requires-Dist: types-psutil >=5.9.5.17
 Requires-Dist: types-aiofiles >=0.8.3
 Requires-Dist: protobuf >=4.22.3
 Requires-Dist: types-protobuf <5,>=4.24
-Requires-Dist: grpcio >=1.44.0
-Requires-Dist: grpcio-health-checking >=1.44.0
-Requires-Dist: grpcio-channelz >=1.44.0
-Requires-Dist: grpcio-status >=1.44.0
-Requires-Dist: grpcio-tools >=1.44.0
-Requires-Dist: grpcio-testing >=1.44.0
-Requires-Dist: grpcio-reflection >=1.44.0
+Requires-Dist: grpcio <1.63.0,>=1.44.0
+Requires-Dist: grpcio-health-checking <1.63.0,>=1.44.0
+Requires-Dist: grpcio-channelz <1.63.0,>=1.44.0
+Requires-Dist: grpcio-status <1.63.0,>=1.44.0
+Requires-Dist: grpcio-tools <1.63.0,>=1.44.0
+Requires-Dist: grpcio-testing <1.63.0,>=1.44.0
+Requires-Dist: grpcio-reflection <1.63.0,>=1.44.0
 Requires-Dist: orjson >=3.6.7
 Requires-Dist: types-setuptools
 Requires-Dist: pydantic <2.0,>=1.9.0
 Requires-Dist: aiobotocore >=2.9.0
 Requires-Dist: botocore >=1.34.0
 Requires-Dist: google-cloud-storage
 Requires-Dist: gcloud
```

## Comparing `nucliadb-3.0.3.post460.dist-info/entry_points.txt` & `nucliadb-3.0.3.post478.dist-info/entry_points.txt`

 * *Files identical despite different names*

## Comparing `nucliadb-3.0.3.post460.dist-info/RECORD` & `nucliadb-3.0.3.post478.dist-info/RECORD`

 * *Files 1% similar despite different names*

```diff
@@ -24,19 +24,19 @@
 nucliadb/openapi.py,sha256=wDiw0dVEvTpJvbatkJ0JZLkKm9RItZT5PWRHjqRfqTA,2272
 nucliadb/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 nucliadb/common/__init__.py,sha256=cp15ZcFnHvpcu_5-aK2A4uUyvuZVV_MJn4bIXMa20ks,835
 nucliadb/common/locking.py,sha256=_168BClwNyXVentC7mk4_on0qof5G2y5VgTpOWvzJGk,4905
 nucliadb/common/cluster/__init__.py,sha256=cp15ZcFnHvpcu_5-aK2A4uUyvuZVV_MJn4bIXMa20ks,835
 nucliadb/common/cluster/base.py,sha256=z_JD-xNVPB6-6O_u8YMpyOPP3fRmimwq7LbA3EGqDnE,4971
 nucliadb/common/cluster/exceptions.py,sha256=V3c_fgH00GyJ-a5CaGLhwTuhwhUNR9YAGvS5jaRuc_Y,1495
-nucliadb/common/cluster/grpc_node_dummy.py,sha256=pBO675j-BptC5U_8Wi6uB19QSQTixgJP2MTzr8v6_Wk,3658
+nucliadb/common/cluster/grpc_node_dummy.py,sha256=10OWSt-k2198cvaQtm12gjdsjyfjEY0laXcVcaz7gyc,3790
 nucliadb/common/cluster/index_node.py,sha256=WafWLzU1l7EHj1VyG0w6qi2BW_Izc8rFze6ZWbYvT9g,3429
-nucliadb/common/cluster/manager.py,sha256=JIb5jpfmBSjFPXxe4YQqWrQW3TD8iY-0a2HrqIGbThw,21231
+nucliadb/common/cluster/manager.py,sha256=rs2nujx6_avXC4y_6zGlHw2g22NLO6MJzU9-9T6rHl0,21584
 nucliadb/common/cluster/rebalance.py,sha256=RC5Q9Uic0__QHeukd2ANlWyd6AYKBzRm3FXhvwcwxCo,8490
-nucliadb/common/cluster/rollover.py,sha256=pvQbL-xGtEcSlLGsQnMDFj1Jr7_g7IMkj6ZQkH2a4Vo,19593
+nucliadb/common/cluster/rollover.py,sha256=93enMmV9drrokAt0233KtOBOCHQZt2p1Gp2NyYZu1QE,19549
 nucliadb/common/cluster/settings.py,sha256=snENrNo9voc1TZ6uyBnuSHGoS2Ocga_Kn-W33nOlO-c,2713
 nucliadb/common/cluster/utils.py,sha256=Hqhm3OwZ14GWaF3UiAGDXgfxjjpgtQz1xoSBxC2Bd3Q,5494
 nucliadb/common/cluster/discovery/__init__.py,sha256=cp15ZcFnHvpcu_5-aK2A4uUyvuZVV_MJn4bIXMa20ks,835
 nucliadb/common/cluster/discovery/base.py,sha256=P0JwzRYqOKxOzV_K_glwPizDGFGBY-l8G7TeTId9LIA,6553
 nucliadb/common/cluster/discovery/k8s.py,sha256=pvuyIYuWWDpRz7Bv8D_LOKFMz0w8sucpJvDshmRNpe0,12518
 nucliadb/common/cluster/discovery/manual.py,sha256=7wdcyfrR8oii2hP3AzOTAaUAGwkQu7eOj9Xl7Q49IUQ,1957
 nucliadb/common/cluster/discovery/single.py,sha256=2BhcencPKQQIfVitmTPJZm3TkBHyY9ZMcr-Clh8k2tM,1737
@@ -195,32 +195,31 @@
 nucliadb/reader/tests/test_reader_file_download.py,sha256=V_wLTRmSlYemSPLOBo3A_jhMBluro2sJiQwSsGGBx6I,10199
 nucliadb/reader/tests/test_reader_resource.py,sha256=A7XzHngspJxPqxzyMZ2Zg2Kp8SuDTi78Fo2rG1roLyo,10586
 nucliadb/reader/tests/test_reader_resource_field.py,sha256=YQ-U2mEGhs_rPGxcWPZmWLSEoCxBo3AVDtLZCtZrGb8,6535
 nucliadb/search/__init__.py,sha256=fwzdF6p7p9uDCtE38gTUxrRVIdbEDVQTAXWUMVKgSBM,1535
 nucliadb/search/app.py,sha256=azMj8BiaFr03pYQKcWSr2YqjB0FopJDeVKE2wwuj6pU,4905
 nucliadb/search/lifecycle.py,sha256=s6If2a78dcv4_71d-Q_uA6b9TaJCQOASUhqa2HcxfIw,1956
 nucliadb/search/openapi.py,sha256=t3Wo_4baTrfPftg2BHsyLWNZ1MYn7ZRdW7ht-wFOgRs,1016
-nucliadb/search/predict.py,sha256=u_49fIHNlduVDxd7kbZJO5UYmgSyPSH-PVpu7OG9UOU,18535
+nucliadb/search/predict.py,sha256=SOzMErnplx-jDTdKya1hr4LKbQt956THyzN_vVc1iiY,17332
 nucliadb/search/run.py,sha256=aFb-CXRi_C8YMpP_ivNj8KW1BYhADj88y8K9Lr_nUPI,1402
 nucliadb/search/settings.py,sha256=Nm4BkdNNdYfU1wGvvWMvlazRSlRGoae99GEdm48-bXI,1193
 nucliadb/search/utilities.py,sha256=9SsRDw0rJVXVoLBfF7rBb6q080h-thZc7u8uRcTiBeY,1037
 nucliadb/search/api/__init__.py,sha256=cp15ZcFnHvpcu_5-aK2A4uUyvuZVV_MJn4bIXMa20ks,835
-nucliadb/search/api/v1/__init__.py,sha256=JH9NGhhyRzirOYY5_pDx5zGZVvpU3317lygSbEb0MFk,1272
+nucliadb/search/api/v1/__init__.py,sha256=tusthakDVkeiAgU-eNjLsO183KXs8Js3fdPAF3JTXP0,1222
 nucliadb/search/api/v1/chat.py,sha256=dNaU4Cfkbta9-buRsPb98s1gsfvvzVCQIoYp2yvICmk,9913
 nucliadb/search/api/v1/feedback.py,sha256=j0PGSGDSbwwS5clRDbU_iCxuISFOtf2DN9Ey-fVGpso,2665
 nucliadb/search/api/v1/find.py,sha256=TvfV-KBUT52gpAgrWTtDOEkNTcKm69qma8mKl0p9mCQ,8804
 nucliadb/search/api/v1/knowledgebox.py,sha256=hQ0wdBlHJVTwiRZgVCeNVwW_6f2bay88Hs9JMHgnx9M,6938
 nucliadb/search/api/v1/predict_proxy.py,sha256=2RME4enSpVXbNzboYQT1XhFFSgakDBgg3Wxj26mQglY,3041
 nucliadb/search/api/v1/router.py,sha256=mtT07rBZcVfpa49doaw9b1tj3sdi3qLH0gn9Io6NYM0,988
 nucliadb/search/api/v1/search.py,sha256=M3NQ7xZDeWsEWpfZyNnivHj7NNk11K4rbbziqhj8Ihs,18325
 nucliadb/search/api/v1/suggest.py,sha256=zGNB-vFgwYUjp9vxBYr5KB2ucJhhhZJqK85tOUO6z0w,5928
 nucliadb/search/api/v1/summarize.py,sha256=-hzveoztY3Qy68V5bCbX07McG5TKFzCerA27rYOQW7o,2536
-nucliadb/search/api/v1/utils.py,sha256=zvZNUSYNjF28NnKdmBTwLbFF0kjzFUNIWaP3qCs3P9Q,1412
+nucliadb/search/api/v1/utils.py,sha256=yEAuvuPXjyhCQ-rOqGajCRDp0Y6UDH8uG6QWtK-tVuc,1433
 nucliadb/search/api/v1/resource/__init__.py,sha256=cp15ZcFnHvpcu_5-aK2A4uUyvuZVV_MJn4bIXMa20ks,835
-nucliadb/search/api/v1/resource/ask.py,sha256=9DXycgB0zXGjmZ9A51VVnJRkxI_tfL5LlT61-ADG6Es,6095
 nucliadb/search/api/v1/resource/chat.py,sha256=y3SIyr92oMQBrc5UKWsRLDFUCK3cgAKjxM0PBsNnu5Q,5887
 nucliadb/search/api/v1/resource/search.py,sha256=xIl_w70MpvC8Aqu89h4tXWNCZYaN9hxUUV04J1wK95w,5293
 nucliadb/search/requesters/__init__.py,sha256=itSI7dtTwFP55YMX4iK7JzdMHS5CQVUiB1XzQu4UBh8,833
 nucliadb/search/requesters/utils.py,sha256=UbWLBSIuZETkG0OoDDkL4XjC2Zmc5wWfofdJPufXmdw,9070
 nucliadb/search/search/__init__.py,sha256=cp15ZcFnHvpcu_5-aK2A4uUyvuZVV_MJn4bIXMa20ks,835
 nucliadb/search/search/cache.py,sha256=86WwnknDYI00bd-kFf5MhN8TVFS2tfHzgobUHv_fAIA,2746
 nucliadb/search/search/exceptions.py,sha256=mbToQ-ghrv8ukLEv8S_-EZrgweWaIZZ5SIpoeuGDk6s,1154
@@ -228,39 +227,38 @@
 nucliadb/search/search/filters.py,sha256=HpTpaDjKmUZWkp5xFFqKHz3TYdKEVBk4jWb2ssIYa5g,6513
 nucliadb/search/search/find.py,sha256=_cGdIfSqpaxm01SqTbcQCQJtadeiL71HB4zEIBj1dM4,4612
 nucliadb/search/search/find_merge.py,sha256=vhq14MFE7N9-9SNlg66LNUr6YAhR9cW22oDpmjvQhL0,17152
 nucliadb/search/search/merge.py,sha256=-srmB1gZEuMa9c2_hLTD1ihjJwDhdB6wnp9b7ljxuIM,21282
 nucliadb/search/search/metrics.py,sha256=4xQm4Q0_-R1bgMtnrbm-YaClEFR8HE6wDk9lunCrhjo,1130
 nucliadb/search/search/paragraphs.py,sha256=8TTii45JvQ7SXsV9Z9ipt5QpYk7ux6PnlOkjKPfYz4A,8698
 nucliadb/search/search/predict_proxy.py,sha256=aOq1AzXkUdHtEmXsec07ffuMKGjlMu-NaUxb_IKme6U,3026
-nucliadb/search/search/query.py,sha256=K7Q_lgeTRVsUT-vNCUGmbk_wOhSg2q1v9d8XYD6FJIE,31084
+nucliadb/search/search/query.py,sha256=bVfTxBQPp86CK_d12K3hS8SMa7eZkXU1w8r1O2jIoDM,31567
 nucliadb/search/search/shards.py,sha256=0p_BWLEVrK87htqhavZ2ixA2l253FPQnre3RpThtZco,3018
 nucliadb/search/search/summarize.py,sha256=bjncFFBv1R9g4OyhQSlGHFq5cJ8UvR8KrMgeKc-1AMU,5101
 nucliadb/search/search/utils.py,sha256=Gzjr9rFdwRfOgyDzX1Slz8DbcXLvavo0124S8II9omw,2438
 nucliadb/search/search/chat/__init__.py,sha256=cp15ZcFnHvpcu_5-aK2A4uUyvuZVV_MJn4bIXMa20ks,835
 nucliadb/search/search/chat/images.py,sha256=AjPgCJaCzu19ruUJcEVaG_bEUmqzB65EH0mduMbkzAE,2058
 nucliadb/search/search/chat/prompt.py,sha256=W98mZrhrscjkxVJ02OM7veAQ1fjMrNDSZ1CUSaECCCk,20793
 nucliadb/search/search/chat/query.py,sha256=4wV6nwzNVA4skiUVM0ggBgdRR7BjYHZ801b87WAuIgI,15347
 nucliadb/search/tests/__init__.py,sha256=cp15ZcFnHvpcu_5-aK2A4uUyvuZVV_MJn4bIXMa20ks,835
 nucliadb/search/tests/conftest.py,sha256=BhVEPbrIm7GKDHtnS7tc7WqCRReIL4MzzTjLQUWrLJY,1295
 nucliadb/search/tests/fixtures.py,sha256=a0q-mh15uvr97ebGTStcdONWx4AQ8rdkH772azMwMMg,6578
-nucliadb/search/tests/node.py,sha256=S1JT1Rq7K2w_4c-bjSUkazr7bDN_OvjTTuYv1Ut_j64,15529
+nucliadb/search/tests/node.py,sha256=QInxf97DUUi-afzBPZDboCH8D-E02A3R-XFwFpUrvCc,15480
 nucliadb/search/tests/unit/__init__.py,sha256=itSI7dtTwFP55YMX4iK7JzdMHS5CQVUiB1XzQu4UBh8,833
 nucliadb/search/tests/unit/test_app.py,sha256=3wr6_DTLdwhpk7Sske7EEqmGbaJSG4OH9Olw_KVszPw,2649
 nucliadb/search/tests/unit/test_find_merge.py,sha256=z_qLcXG8qdUegGkaEloG7wXXwoZyppeOnzUCcHAVq3w,3374
 nucliadb/search/tests/unit/test_merge.py,sha256=1uCdn3MZbUWs2WKFGJSJZgpm4xTtn5nvgurbo37l5B8,1400
-nucliadb/search/tests/unit/test_predict.py,sha256=TUEk2zGwAss0CpdoEtM3C3mxbn_tn9x3hg9SsDzJgrQ,14729
+nucliadb/search/tests/unit/test_predict.py,sha256=QRM2KhJtsaWUOzXv36LQ5hazuN9ViFsmvrgwdGZI3_I,13101
 nucliadb/search/tests/unit/test_run.py,sha256=7fDXkaEOSd8f3Cd7w5QWYeB4uGXA59M22MojR1auv0Y,1317
 nucliadb/search/tests/unit/api/__init__.py,sha256=cp15ZcFnHvpcu_5-aK2A4uUyvuZVV_MJn4bIXMa20ks,835
 nucliadb/search/tests/unit/api/v1/__init__.py,sha256=cp15ZcFnHvpcu_5-aK2A4uUyvuZVV_MJn4bIXMa20ks,835
 nucliadb/search/tests/unit/api/v1/test_chat.py,sha256=Ud6MDM7gLUV6PZQeCDA5vBcJ40Sf4fqNeWBwYWUOi-E,2966
 nucliadb/search/tests/unit/api/v1/test_predict_proxy.py,sha256=CuouBrldS3mpBZe3FlpkaW3R_cI8Db8o6bSFPW0ifmA,2865
 nucliadb/search/tests/unit/api/v1/test_summarize.py,sha256=4VQm-fegHLeBNBoNuoKbKM5FiqAML9m9QT7XNY3n2n4,2901
 nucliadb/search/tests/unit/api/v1/resource/__init__.py,sha256=cp15ZcFnHvpcu_5-aK2A4uUyvuZVV_MJn4bIXMa20ks,835
-nucliadb/search/tests/unit/api/v1/resource/test_ask.py,sha256=U2IY8NfBTUj1Phc8poTMSDegB5_OLMT6vJ7NIo1EI5c,2411
 nucliadb/search/tests/unit/api/v1/resource/test_chat.py,sha256=p91CJTfjmPfVpMt6B1Rzee2yK1Dy4vNQeXgqxTXRWCk,3040
 nucliadb/search/tests/unit/search/__init__.py,sha256=itSI7dtTwFP55YMX4iK7JzdMHS5CQVUiB1XzQu4UBh8,833
 nucliadb/search/tests/unit/search/test_chat_prompt.py,sha256=cSHYWqCOUMIuCECFrXB6bWopWw9aTMC8aa5hwX1K-gA,8567
 nucliadb/search/tests/unit/search/test_fetch.py,sha256=YKEhS3yUcirzZXAwauhKeOo5v7pvAh6dzuiSMIRx9xg,3736
 nucliadb/search/tests/unit/search/test_filters.py,sha256=oOn7C8egKDnVsflfQLFNkeNZsXoqDV7S3Yl2qb0MtSs,4306
 nucliadb/search/tests/unit/search/test_paragraphs.py,sha256=cyyCzyOBzUyhwqx5w3M9wp96qrWsg2vHksMyoqs5kYg,4492
 nucliadb/search/tests/unit/search/test_predict_proxy.py,sha256=8fSUbNaMEv3pKBcGW-7e7xOwX6qfn7K1m9UfMpwu1TI,3496
@@ -443,13 +441,13 @@
 nucliadb/writer/tus/exceptions.py,sha256=CmxYKnHXpXug25DYV4SpVAU47SGD-NVBd7pNTRbWHyk,2186
 nucliadb/writer/tus/gcs.py,sha256=WykJZicWKRYkVB5_Fkb_1cVLovAk86IVkEn1VgEDufc,14527
 nucliadb/writer/tus/local.py,sha256=lIOoGaylnsxPBYGskcmKSHv7MsvwIYFS4soDLey_KSs,5849
 nucliadb/writer/tus/pg.py,sha256=JUK_xKsyNcKAvWOch8gUMTc_e1evI_3aC6-Y5gMk2jw,4367
 nucliadb/writer/tus/s3.py,sha256=a9mfPtjBW3QaTYY2r6P7u_Y13V6mBefZjWgV4juZzgE,9069
 nucliadb/writer/tus/storage.py,sha256=8iBOjWIcY6PawQq_rmSiBKi0Gl6J6Q5ad6L-9nLCcJ4,4734
 nucliadb/writer/tus/utils.py,sha256=MSdVbRsRSZVdkaum69_0wku7X3p5wlZf4nr6E0GMKbw,2556
-nucliadb-3.0.3.post460.dist-info/METADATA,sha256=AtTXtJ6DjnwwaVRDPMtoq9nZ4pi2LsbROPXK1bCOqYs,4343
-nucliadb-3.0.3.post460.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-nucliadb-3.0.3.post460.dist-info/entry_points.txt,sha256=XqGfgFDuY3zXQc8ewXM2TRVjTModIq851zOsgrmaXx4,1268
-nucliadb-3.0.3.post460.dist-info/top_level.txt,sha256=hwYhTVnX7jkQ9gJCkVrbqEG1M4lT2F_iPQND1fCzF80,20
-nucliadb-3.0.3.post460.dist-info/zip-safe,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
-nucliadb-3.0.3.post460.dist-info/RECORD,,
+nucliadb-3.0.3.post478.dist-info/METADATA,sha256=DiXKWtANY3AkFT8S83WkG1zbdO6o69BoR2HcyWc8wj8,4399
+nucliadb-3.0.3.post478.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+nucliadb-3.0.3.post478.dist-info/entry_points.txt,sha256=XqGfgFDuY3zXQc8ewXM2TRVjTModIq851zOsgrmaXx4,1268
+nucliadb-3.0.3.post478.dist-info/top_level.txt,sha256=hwYhTVnX7jkQ9gJCkVrbqEG1M4lT2F_iPQND1fCzF80,20
+nucliadb-3.0.3.post478.dist-info/zip-safe,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
+nucliadb-3.0.3.post478.dist-info/RECORD,,
```

