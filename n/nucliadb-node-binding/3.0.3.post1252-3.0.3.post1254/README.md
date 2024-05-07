# Comparing `tmp/nucliadb_node_binding-3.0.3.post1252.tar.gz` & `tmp/nucliadb_node_binding-3.0.3.post1254.tar.gz`

## Comparing `nucliadb_node_binding-3.0.3.post1252.tar` & `nucliadb_node_binding-3.0.3.post1254.tar`

### file list

```diff
@@ -1,285 +1,285 @@
--rw-r--r--   0        0        0      931 1970-01-01 00:00:00.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_core/Cargo.toml
--rw-r--r--   0     1001      127     5872 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_core/src/fs_state.rs
--rw-r--r--   0     1001      127     2969 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_core/src/lib.rs
--rw-r--r--   0     1001      127     2295 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_core/src/merge.rs
--rw-r--r--   0     1001      127      906 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_core/src/metrics/meters/mod.rs
--rw-r--r--   0     1001      127     5462 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_core/src/metrics/meters/prometheus.rs
--rw-r--r--   0     1001      127     1702 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_core/src/metrics/metric/grpc_ops.rs
--rw-r--r--   0     1001      127     1442 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_core/src/metrics/metric/mod.rs
--rw-r--r--   0     1001      127     1950 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_core/src/metrics/metric/replication.rs
--rw-r--r--   0     1001      127     2626 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_core/src/metrics/metric/request_time.rs
--rw-r--r--   0     1001      127     1644 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_core/src/metrics/metric/shard_cache.rs
--rw-r--r--   0     1001      127    21641 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_core/src/metrics/metric/tokio_runtime.rs
--rw-r--r--   0     1001      127    16736 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_core/src/metrics/metric/tokio_tasks.rs
--rw-r--r--   0     1001      127     3415 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_core/src/metrics/metric/vectors.rs
--rw-r--r--   0     1001      127     1324 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_core/src/metrics/mod.rs
--rw-r--r--   0     1001      127     3074 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_core/src/metrics/task_monitor.rs
--rw-r--r--   0     1001      127     3920 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_core/src/metrics/tests.rs
--rw-r--r--   0     1001      127     2990 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_core/src/paragraphs.rs
--rw-r--r--   0     1001      127    17305 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_core/src/query_language/mod.rs
--rw-r--r--   0     1001      127    15367 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_core/src/query_planner.rs
--rw-r--r--   0     1001      127     2069 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_core/src/relations.rs
--rw-r--r--   0     1001      127     8250 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_core/src/tantivy_replica.rs
--rw-r--r--   0     1001      127     2603 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_core/src/texts.rs
--rw-r--r--   0     1001      127     3551 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_core/src/vectors.rs
--rw-r--r--   0        0        0      708 1970-01-01 00:00:00.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_relations2/Cargo.toml
--rw-r--r--   0     1001      127     3593 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_relations2/src/io_maps.rs
--rw-r--r--   0     1001      127      916 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_relations2/src/lib.rs
--rw-r--r--   0     1001      127    17039 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_relations2/src/reader.rs
--rw-r--r--   0     1001      127     7123 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_relations2/src/schema.rs
--rw-r--r--   0     1001      127     8007 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_relations2/src/writer.rs
--rw-r--r--   0     1001      127     1802 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_relations2/tests/common/mod.rs
--rw-r--r--   0     1001      127     9445 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_relations2/tests/test_reader.rs
--rw-r--r--   0     1001      127     3297 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_relations2/tests/test_writer.rs
--rw-r--r--   0        0        0      501 1970-01-01 00:00:00.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_protos/Cargo.toml
--rw-r--r--   0     1001      127     2155 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_protos/build.rs
--rw-r--r--   0     1001      127    26110 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_protos/src/fdbwriter.rs
--rw-r--r--   0     1001      127        0 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_protos/src/google.protobuf.rs
--rw-r--r--   0     1001      127     9795 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_protos/src/knowledgebox.rs
--rw-r--r--   0     1001      127     1256 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_protos/src/lib.rs
--rw-r--r--   0     1001      127    77311 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_protos/src/nodereader.rs
--rw-r--r--   0     1001      127    10240 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_protos/src/noderesources.rs
--rw-r--r--   0     1001      127    46404 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_protos/src/nodewriter.rs
--rw-r--r--   0     1001      127    19106 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_protos/src/replication.rs
--rw-r--r--   0     1001      127    33352 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_protos/src/resources.rs
--rw-r--r--   0     1001      127     5528 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_protos/src/utils.rs
--rw-r--r--   0        0        0      629 1970-01-01 00:00:00.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_paragraphs3/Cargo.toml
--rw-r--r--   0     1001      127     7796 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_paragraphs3/src/fuzzy_query.rs
--rw-r--r--   0     1001      127     1024 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_paragraphs3/src/lib.rs
--rw-r--r--   0     1001      127     2780 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_paragraphs3/src/query_io.rs
--rw-r--r--   0     1001      127    42885 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_paragraphs3/src/reader.rs
--rw-r--r--   0     1001      127     4407 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_paragraphs3/src/schema.rs
--rw-r--r--   0     1001      127    21349 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_paragraphs3/src/search_query.rs
--rw-r--r--   0     1001      127    11723 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_paragraphs3/src/search_response.rs
--rw-r--r--   0     1001      127     2846 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_paragraphs3/src/set_query.rs
--rw-r--r--   0     1001      127     4090 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_paragraphs3/src/stop_words.rs
--rw-r--r--   0     1001      127    17057 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_paragraphs3/src/writer.rs
--rw-r--r--   0     1001      127       88 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_paragraphs3/stop_words/README.md
--rw-r--r--   0     1001      127    19791 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_paragraphs3/stop_words/ar.json
--rw-r--r--   0     1001      127     1923 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_paragraphs3/stop_words/az.json
--rw-r--r--   0     1001      127    11684 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_paragraphs3/stop_words/bn.json
--rw-r--r--   0     1001      127     2513 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_paragraphs3/stop_words/ca.json
--rw-r--r--   0     1001      127    12802 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_paragraphs3/stop_words/ch.json
--rw-r--r--   0     1001      127      730 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_paragraphs3/stop_words/da.json
--rw-r--r--   0     1001      127     2090 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_paragraphs3/stop_words/de.json
--rw-r--r--   0     1001      127     6284 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_paragraphs3/stop_words/el.json
--rw-r--r--   0     1001      127     1473 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_paragraphs3/stop_words/en.json
--rw-r--r--   0     1001      127     3451 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_paragraphs3/stop_words/es.json
--rw-r--r--   0     1001      127     3182 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_paragraphs3/stop_words/eu.json
--rw-r--r--   0     1001      127     2126 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_paragraphs3/stop_words/extract.py
--rw-r--r--   0     1001      127     2748 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_paragraphs3/stop_words/fi.json
--rw-r--r--   0     1001      127     1388 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_paragraphs3/stop_words/fr.json
--rw-r--r--   0     1001      127     5716 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_paragraphs3/stop_words/he.json
--rw-r--r--   0     1001      127     2108 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_paragraphs3/stop_words/hu.json
--rw-r--r--   0     1001      127     8721 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_paragraphs3/stop_words/id.json
--rw-r--r--   0     1001      127     2535 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_paragraphs3/stop_words/it.json
--rw-r--r--   0     1001      127    11737 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_paragraphs3/stop_words/kk.json
--rw-r--r--   0     1001      127     7730 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_paragraphs3/stop_words/ne.json
--rw-r--r--   0     1001      127      756 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_paragraphs3/stop_words/nl.json
--rw-r--r--   0     1001      127     1447 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_paragraphs3/stop_words/no.json
--rw-r--r--   0     1001      127     2055 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_paragraphs3/stop_words/pt.json
--rw-r--r--   0     1001      127     3327 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_paragraphs3/stop_words/ro.json
--rw-r--r--   0     1001      127     3856 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_paragraphs3/stop_words/ru.json
--rw-r--r--   0     1001      127    23032 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_paragraphs3/stop_words/sl.json
--rw-r--r--   0     1001      127      993 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_paragraphs3/stop_words/sv.json
--rw-r--r--   0     1001      127     5424 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_paragraphs3/stop_words/tg.json
--rw-r--r--   0     1001      127      491 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_paragraphs3/stop_words/tr.json
--rw-r--r--   0        0        0     3294 1970-01-01 00:00:00.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_node/Cargo.toml
--rw-r--r--   0     1001      127     1045 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_node/.rustc_info.json
--rw-r--r--   0     1001      127      877 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_node/Makefile
--rw-r--r--   0     1001      127     1500 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_node/README.md
--rw-r--r--   0     1001      127     1757 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_node/nucliadb_node/__init__.py
--rw-r--r--   0     1001      127     3957 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_node/nucliadb_node/app.py
--rw-r--r--   0     1001      127    19055 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_node/nucliadb_node/indexer.py
--rw-r--r--   0     1001      127      890 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_node/nucliadb_node/listeners/__init__.py
--rw-r--r--   0     1001      127     2424 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_node/nucliadb_node/listeners/indexed_publisher.py
--rw-r--r--   0     1001      127     4015 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_node/nucliadb_node/pull.py
--rw-r--r--   0     1001      127     1535 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_node/nucliadb_node/service.py
--rw-r--r--   0     1001      127     1487 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_node/nucliadb_node/settings.py
--rw-r--r--   0     1001      127     1133 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_node/nucliadb_node/signals.py
--rw-r--r--   0     1001      127      835 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_node/nucliadb_node/tests/__init__.py
--rw-r--r--   0     1001      127     1092 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_node/nucliadb_node/tests/conftest.py
--rw-r--r--   0     1001      127    11293 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_node/nucliadb_node/tests/fixtures.py
--rw-r--r--   0     1001      127    13795 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_node/nucliadb_node/tests/integration/test_indexing.py
--rw-r--r--   0     1001      127     2289 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_node/nucliadb_node/tests/unit/test_app.py
--rw-r--r--   0     1001      127     2361 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_node/nucliadb_node/tests/unit/test_indexed_publisher.py
--rw-r--r--   0     1001      127    12984 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_node/nucliadb_node/tests/unit/test_indexer.py
--rw-r--r--   0     1001      127     3379 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_node/nucliadb_node/tests/unit/test_pull.py
--rw-r--r--   0     1001      127     2489 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_node/nucliadb_node/writer.py
--rw-r--r--   0     1001      127      101 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_node/requirements-sources.txt
--rw-r--r--   0     1001      127      276 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_node/requirements.txt
--rw-r--r--   0     1001      127      249 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_node/setup.cfg
--rw-r--r--   0     1001      127     1405 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_node/setup.py
--rw-r--r--   0     1001      127     2518 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_node/src/analytics/blocking.rs
--rw-r--r--   0     1001      127     1219 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_node/src/analytics/mod.rs
--rw-r--r--   0     1001      127     4931 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_node/src/analytics/payload.rs
--rw-r--r--   0     1001      127    12828 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_node/src/analytics/sender.rs
--rw-r--r--   0     1001      127     3085 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_node/src/analytics/sink.rs
--rw-r--r--   0     1001      127     1900 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_node/src/analytics/sync.rs
--rw-r--r--   0     1001      127     5045 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_node/src/bin/reader.rs
--rw-r--r--   0     1001      127     8050 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_node/src/bin/writer.rs
--rw-r--r--   0     1001      127     1345 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_node/src/cache/mod.rs
--rw-r--r--   0     1001      127     3035 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_node/src/cache/reader_cache.rs
--rw-r--r--   0     1001      127    14199 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_node/src/cache/resource_cache.rs
--rw-r--r--   0     1001      127    11265 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_node/src/cache/writer_cache.rs
--rw-r--r--   0     1001      127     1771 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_node/src/disk_structure.rs
--rw-r--r--   0     1001      127     1111 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_node/src/errors.rs
--rw-r--r--   0     1001      127     2656 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_node/src/grpc/collect_garbage.rs
--rw-r--r--   0     1001      127    18813 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_node/src/grpc/grpc_reader.rs
--rw-r--r--   0     1001      127    15003 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_node/src/grpc/grpc_writer.rs
--rw-r--r--   0     1001      127     3186 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_node/src/grpc/middleware/debug.rs
--rw-r--r--   0     1001      127     3440 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_node/src/grpc/middleware/metrics.rs
--rw-r--r--   0     1001      127     1009 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_node/src/grpc/middleware/mod.rs
--rw-r--r--   0     1001      127     4158 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_node/src/grpc/middleware/telemetry.rs
--rw-r--r--   0     1001      127     1283 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_node/src/grpc/mod.rs
--rw-r--r--   0     1001      127     2581 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_node/src/grpc/update.rs
--rw-r--r--   0     1001      127     1173 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_node/src/http_server/metrics_service.rs
--rw-r--r--   0     1001      127     1465 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_node/src/http_server/mod.rs
--rw-r--r--   0     1001      127     1943 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_node/src/http_server/traces_service.rs
--rw-r--r--   0     1001      127     1504 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_node/src/lib.rs
--rw-r--r--   0     1001      127     2757 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_node/src/lifecycle.rs
--rw-r--r--   0     1001      127     1778 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_node/src/merge/global.rs
--rw-r--r--   0     1001      127     1089 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_node/src/merge/mod.rs
--rw-r--r--   0     1001      127    13672 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_node/src/merge/scheduler.rs
--rw-r--r--   0     1001      127     3677 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_node/src/merge/work.rs
--rw-r--r--   0     1001      127     1935 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_node/src/node_metadata.rs
--rw-r--r--   0     1001      127     2417 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_node/src/replication/health.rs
--rw-r--r--   0     1001      127     1070 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_node/src/replication/mod.rs
--rw-r--r--   0     1001      127    14144 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_node/src/replication/replicator.rs
--rw-r--r--   0     1001      127    11803 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_node/src/replication/service.rs
--rw-r--r--   0     1001      127    15251 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_node/src/settings.rs
--rw-r--r--   0     1001      127     1111 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_node/src/shards/errors.rs
--rw-r--r--   0     1001      127     9990 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_node/src/shards/indexes.rs
--rw-r--r--   0     1001      127    11085 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_node/src/shards/metadata.rs
--rw-r--r--   0     1001      127     1140 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_node/src/shards/mod.rs
--rw-r--r--   0     1001      127    26968 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_node/src/shards/shard_reader.rs
--rw-r--r--   0     1001      127    21473 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_node/src/shards/shard_writer.rs
--rw-r--r--   0     1001      127     1890 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_node/src/shards/versioning.rs
--rw-r--r--   0     1001      127    10170 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_node/src/telemetry.rs
--rw-r--r--   0     1001      127     6396 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_node/src/utils.rs
--rw-r--r--   0     1001      127       42 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_node/test.sh
--rw-r--r--   0     1001      127     1115 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_node/tests/common/mod.rs
--rw-r--r--   0     1001      127    12731 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_node/tests/common/node_services.rs
--rw-r--r--   0     1001      127     7823 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_node/tests/common/resources.rs
--rw-r--r--   0     1001      127     8173 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_node/tests/test_date_range_search.rs
--rw-r--r--   0     1001      127     4089 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_node/tests/test_download.rs
--rw-r--r--   0     1001      127     1684 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_node/tests/test_merge.rs
--rw-r--r--   0     1001      127     6003 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_node/tests/test_replication.rs
--rw-r--r--   0     1001      127    22494 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_node/tests/test_search_relations.rs
--rw-r--r--   0     1001      127     6958 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_node/tests/test_search_sorting.rs
--rw-r--r--   0     1001      127     7044 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_node/tests/test_security_search.rs
--rw-r--r--   0     1001      127     2508 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_node/tests/test_set_resource_from_storage.rs
--rw-r--r--   0     1001      127     6862 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_node/tests/test_shards.rs
--rw-r--r--   0     1001      127    10698 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_node/tests/test_suggest.rs
--rw-r--r--   0     1001      127     5438 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_node/tests/test_vector_normalization.rs
--rw-r--r--   0        0        0      399 1970-01-01 00:00:00.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_texts2/Cargo.toml
--rw-r--r--   0     1001      127      931 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_texts2/src/lib.rs
--rw-r--r--   0     1001      127     2755 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_texts2/src/query_io.rs
--rw-r--r--   0     1001      127    22721 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_texts2/src/reader.rs
--rw-r--r--   0     1001      127     3105 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_texts2/src/schema.rs
--rw-r--r--   0     1001      127     8682 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_texts2/src/search_query.rs
--rw-r--r--   0     1001      127    10109 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_texts2/src/writer.rs
--rw-r--r--   0     1001      127     3396 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_texts2/tests/common/mod.rs
--rw-r--r--   0     1001      127     2068 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_texts2/tests/test_reader.rs
--rw-r--r--   0     1001      127     9567 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_texts2/tests/test_search.rs
--rw-r--r--   0     1001      127     1249 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_texts2/tests/test_streaming.rs
--rw-r--r--   0     1001      127     3469 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_texts2/tests/test_writer.rs
--rw-r--r--   0        0        0      742 1970-01-01 00:00:00.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_vectors/Cargo.toml
--rw-r--r--   0     1001      127       69 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_vectors/README.md
--rw-r--r--   0     1001      127       43 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_vectors/docs/README.md
--rw-r--r--   0     1001      127    25718 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_vectors/docs/labels.drawio.svg
--rw-r--r--   0     1001      127    12340 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_vectors/src/data_point/disk_hnsw.rs
--rw-r--r--   0     1001      127    24470 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_vectors/src/data_point/mod.rs
--rw-r--r--   0     1001      127    11214 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_vectors/src/data_point/node.rs
--rw-r--r--   0     1001      127    15068 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_vectors/src/data_point/ops_hnsw.rs
--rw-r--r--   0     1001      127     1741 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_vectors/src/data_point/params.rs
--rw-r--r--   0     1001      127     3952 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_vectors/src/data_point/ram_hnsw.rs
--rw-r--r--   0     1001      127    14175 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_vectors/src/data_point/tests.rs
--rw-r--r--   0     1001      127     5798 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_vectors/src/data_point_provider/garbage_collector.rs
--rw-r--r--   0     1001      127     2777 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_vectors/src/data_point_provider/mod.rs
--rw-r--r--   0     1001      127    10613 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_vectors/src/data_point_provider/reader.rs
--rw-r--r--   0     1001      127     2304 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_vectors/src/data_point_provider/replication.rs
--rw-r--r--   0     1001      127     5288 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_vectors/src/data_point_provider/state.rs
--rw-r--r--   0     1001      127    20587 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_vectors/src/data_point_provider/writer.rs
--rw-r--r--   0     1001      127    23710 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_vectors/src/data_types/data_store.rs
--rw-r--r--   0     1001      127     6916 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_vectors/src/data_types/dtrie_ram.rs
--rw-r--r--   0     1001      127     1959 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_vectors/src/data_types/mod.rs
--rw-r--r--   0     1001      127     6143 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_vectors/src/data_types/trie.rs
--rw-r--r--   0     1001      127     2904 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_vectors/src/data_types/trie_ram.rs
--rw-r--r--   0     1001      127     4433 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_vectors/src/data_types/vector.rs
--rw-r--r--   0     1001      127    10472 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_vectors/src/formula/mod.rs
--rw-r--r--   0     1001      127     2165 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_vectors/src/lib.rs
--rw-r--r--   0     1001      127     1278 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_vectors/src/service/mod.rs
--rw-r--r--   0     1001      127     1897 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_vectors/src/service/query_io.rs
--rw-r--r--   0     1001      127    17174 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_vectors/src/service/reader.rs
--rw-r--r--   0     1001      127    15115 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_vectors/src/service/writer.rs
--rw-r--r--   0     1001      127     1668 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_vectors/src/utils.rs
--rw-r--r--   0     1001      127     2884 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_vectors/tests/test_merge.rs
--rw-r--r--   0        0        0      361 1970-01-01 00:00:00.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_procs/Cargo.toml
--rw-r--r--   0     1001      127     3409 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_procs/src/lib.rs
--rw-r--r--   0     1001      127     2885 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_procs/src/measure.rs
--rw-r--r--   0     1001      127     1081 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_procs/tests/dont_compile/actor_defined_twice.rs
--rw-r--r--   0     1001      127      222 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_procs/tests/dont_compile/actor_defined_twice.stderr
--rw-r--r--   0     1001      127     1038 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_procs/tests/dont_compile/actor_not_defined.rs
--rw-r--r--   0     1001      127      327 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_procs/tests/dont_compile/actor_not_defined.stderr
--rw-r--r--   0     1001      127     1086 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_procs/tests/dont_compile/metric_defined_twice.rs
--rw-r--r--   0     1001      127      249 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_procs/tests/dont_compile/metric_defined_twice.stderr
--rw-r--r--   0     1001      127     1046 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_procs/tests/dont_compile/wrong_actor.rs
--rw-r--r--   0     1001      127     1303 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_procs/tests/dont_compile/wrong_actor.stderr
--rw-r--r--   0     1001      127     1408 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_procs/tests/test_measure.rs
--rw-r--r--   0        0        0      629 1970-01-01 00:00:00.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_paragraphs2/Cargo.toml
--rw-r--r--   0     1001      127     7796 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_paragraphs2/src/fuzzy_query.rs
--rw-r--r--   0     1001      127     1009 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_paragraphs2/src/lib.rs
--rw-r--r--   0     1001      127     2780 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_paragraphs2/src/query_io.rs
--rw-r--r--   0     1001      127    42940 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_paragraphs2/src/reader.rs
--rw-r--r--   0     1001      127     4808 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_paragraphs2/src/schema.rs
--rw-r--r--   0     1001      127    22494 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_paragraphs2/src/search_query.rs
--rw-r--r--   0     1001      127    11391 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_paragraphs2/src/search_response.rs
--rw-r--r--   0     1001      127     4090 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_paragraphs2/src/stop_words.rs
--rw-r--r--   0     1001      127    17965 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_paragraphs2/src/writer.rs
--rw-r--r--   0     1001      127       88 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_paragraphs2/stop_words/README.md
--rw-r--r--   0     1001      127    19791 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_paragraphs2/stop_words/ar.json
--rw-r--r--   0     1001      127     1923 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_paragraphs2/stop_words/az.json
--rw-r--r--   0     1001      127    11684 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_paragraphs2/stop_words/bn.json
--rw-r--r--   0     1001      127     2513 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_paragraphs2/stop_words/ca.json
--rw-r--r--   0     1001      127    12802 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_paragraphs2/stop_words/ch.json
--rw-r--r--   0     1001      127      730 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_paragraphs2/stop_words/da.json
--rw-r--r--   0     1001      127     2090 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_paragraphs2/stop_words/de.json
--rw-r--r--   0     1001      127     6284 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_paragraphs2/stop_words/el.json
--rw-r--r--   0     1001      127     1473 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_paragraphs2/stop_words/en.json
--rw-r--r--   0     1001      127     3451 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_paragraphs2/stop_words/es.json
--rw-r--r--   0     1001      127     3182 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_paragraphs2/stop_words/eu.json
--rw-r--r--   0     1001      127     2126 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_paragraphs2/stop_words/extract.py
--rw-r--r--   0     1001      127     2748 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_paragraphs2/stop_words/fi.json
--rw-r--r--   0     1001      127     1388 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_paragraphs2/stop_words/fr.json
--rw-r--r--   0     1001      127     5716 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_paragraphs2/stop_words/he.json
--rw-r--r--   0     1001      127     2108 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_paragraphs2/stop_words/hu.json
--rw-r--r--   0     1001      127     8721 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_paragraphs2/stop_words/id.json
--rw-r--r--   0     1001      127     2535 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_paragraphs2/stop_words/it.json
--rw-r--r--   0     1001      127    11737 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_paragraphs2/stop_words/kk.json
--rw-r--r--   0     1001      127     7730 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_paragraphs2/stop_words/ne.json
--rw-r--r--   0     1001      127      756 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_paragraphs2/stop_words/nl.json
--rw-r--r--   0     1001      127     1447 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_paragraphs2/stop_words/no.json
--rw-r--r--   0     1001      127     2055 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_paragraphs2/stop_words/pt.json
--rw-r--r--   0     1001      127     3327 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_paragraphs2/stop_words/ro.json
--rw-r--r--   0     1001      127     3856 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_paragraphs2/stop_words/ru.json
--rw-r--r--   0     1001      127    23032 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_paragraphs2/stop_words/sl.json
--rw-r--r--   0     1001      127      993 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_paragraphs2/stop_words/sv.json
--rw-r--r--   0     1001      127     5424 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_paragraphs2/stop_words/tg.json
--rw-r--r--   0     1001      127      491 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_paragraphs2/stop_words/tr.json
--rw-r--r--   0        0        0      943 1970-01-01 00:00:00.000000 nucliadb_node_binding-3.0.3.post1252/Cargo.toml
--rw-r--r--   0     1001      127     1553 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/CHANGELOG.md
--rw-r--r--   0     1001      127      895 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/Makefile
--rw-r--r--   0     1001      127       52 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/README.md
--rwxr-xr-x   0     1001      127      978 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/cov.sh
--rw-r--r--   0     1001      127     1309 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/pyproject.toml
--rw-r--r--   0     1001      127     2195 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/src/collect_garbage.rs
--rw-r--r--   0     1001      127     1212 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/src/errors.rs
--rw-r--r--   0     1001      127     2337 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/src/lib.rs
--rw-r--r--   0     1001      127     9405 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/src/reader.rs
--rw-r--r--   0     1001      127     2154 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/src/update.rs
--rw-r--r--   0     1001      127     8996 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/src/writer.rs
--rw-r--r--   0     1001      127      835 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/tests/__init__.py
--rw-r--r--   0     1001      127      892 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/tests/conftest.py
--rw-r--r--   0     1001      127     3903 2024-05-06 14:12:26.000000 nucliadb_node_binding-3.0.3.post1252/tests/integration/test_indexing.py
--rw-r--r--   0        0        0      401 1970-01-01 00:00:00.000000 nucliadb_node_binding-3.0.3.post1252/PKG-INFO
+-rw-r--r--   0        0        0     3294 1970-01-01 00:00:00.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_node/Cargo.toml
+-rw-r--r--   0     1001      127     1045 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_node/.rustc_info.json
+-rw-r--r--   0     1001      127      877 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_node/Makefile
+-rw-r--r--   0     1001      127     1500 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_node/README.md
+-rw-r--r--   0     1001      127     1757 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_node/nucliadb_node/__init__.py
+-rw-r--r--   0     1001      127     3957 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_node/nucliadb_node/app.py
+-rw-r--r--   0     1001      127    19055 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_node/nucliadb_node/indexer.py
+-rw-r--r--   0     1001      127      890 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_node/nucliadb_node/listeners/__init__.py
+-rw-r--r--   0     1001      127     2424 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_node/nucliadb_node/listeners/indexed_publisher.py
+-rw-r--r--   0     1001      127     4015 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_node/nucliadb_node/pull.py
+-rw-r--r--   0     1001      127     1535 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_node/nucliadb_node/service.py
+-rw-r--r--   0     1001      127     1487 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_node/nucliadb_node/settings.py
+-rw-r--r--   0     1001      127     1133 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_node/nucliadb_node/signals.py
+-rw-r--r--   0     1001      127      835 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_node/nucliadb_node/tests/__init__.py
+-rw-r--r--   0     1001      127     1092 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_node/nucliadb_node/tests/conftest.py
+-rw-r--r--   0     1001      127    11293 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_node/nucliadb_node/tests/fixtures.py
+-rw-r--r--   0     1001      127    13795 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_node/nucliadb_node/tests/integration/test_indexing.py
+-rw-r--r--   0     1001      127     2289 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_node/nucliadb_node/tests/unit/test_app.py
+-rw-r--r--   0     1001      127     2361 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_node/nucliadb_node/tests/unit/test_indexed_publisher.py
+-rw-r--r--   0     1001      127    12984 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_node/nucliadb_node/tests/unit/test_indexer.py
+-rw-r--r--   0     1001      127     3379 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_node/nucliadb_node/tests/unit/test_pull.py
+-rw-r--r--   0     1001      127     2489 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_node/nucliadb_node/writer.py
+-rw-r--r--   0     1001      127      101 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_node/requirements-sources.txt
+-rw-r--r--   0     1001      127      276 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_node/requirements.txt
+-rw-r--r--   0     1001      127      249 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_node/setup.cfg
+-rw-r--r--   0     1001      127     1405 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_node/setup.py
+-rw-r--r--   0     1001      127     2518 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_node/src/analytics/blocking.rs
+-rw-r--r--   0     1001      127     1219 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_node/src/analytics/mod.rs
+-rw-r--r--   0     1001      127     4931 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_node/src/analytics/payload.rs
+-rw-r--r--   0     1001      127    12828 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_node/src/analytics/sender.rs
+-rw-r--r--   0     1001      127     3085 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_node/src/analytics/sink.rs
+-rw-r--r--   0     1001      127     1900 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_node/src/analytics/sync.rs
+-rw-r--r--   0     1001      127     5045 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_node/src/bin/reader.rs
+-rw-r--r--   0     1001      127     8050 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_node/src/bin/writer.rs
+-rw-r--r--   0     1001      127     1345 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_node/src/cache/mod.rs
+-rw-r--r--   0     1001      127     3035 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_node/src/cache/reader_cache.rs
+-rw-r--r--   0     1001      127    14199 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_node/src/cache/resource_cache.rs
+-rw-r--r--   0     1001      127    11265 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_node/src/cache/writer_cache.rs
+-rw-r--r--   0     1001      127     1771 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_node/src/disk_structure.rs
+-rw-r--r--   0     1001      127     1111 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_node/src/errors.rs
+-rw-r--r--   0     1001      127     2656 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_node/src/grpc/collect_garbage.rs
+-rw-r--r--   0     1001      127    18813 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_node/src/grpc/grpc_reader.rs
+-rw-r--r--   0     1001      127    15003 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_node/src/grpc/grpc_writer.rs
+-rw-r--r--   0     1001      127     3186 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_node/src/grpc/middleware/debug.rs
+-rw-r--r--   0     1001      127     3440 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_node/src/grpc/middleware/metrics.rs
+-rw-r--r--   0     1001      127     1009 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_node/src/grpc/middleware/mod.rs
+-rw-r--r--   0     1001      127     4158 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_node/src/grpc/middleware/telemetry.rs
+-rw-r--r--   0     1001      127     1283 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_node/src/grpc/mod.rs
+-rw-r--r--   0     1001      127     2581 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_node/src/grpc/update.rs
+-rw-r--r--   0     1001      127     1173 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_node/src/http_server/metrics_service.rs
+-rw-r--r--   0     1001      127     1465 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_node/src/http_server/mod.rs
+-rw-r--r--   0     1001      127     1943 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_node/src/http_server/traces_service.rs
+-rw-r--r--   0     1001      127     1504 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_node/src/lib.rs
+-rw-r--r--   0     1001      127     2757 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_node/src/lifecycle.rs
+-rw-r--r--   0     1001      127     1778 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_node/src/merge/global.rs
+-rw-r--r--   0     1001      127     1089 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_node/src/merge/mod.rs
+-rw-r--r--   0     1001      127    13672 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_node/src/merge/scheduler.rs
+-rw-r--r--   0     1001      127     3677 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_node/src/merge/work.rs
+-rw-r--r--   0     1001      127     1935 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_node/src/node_metadata.rs
+-rw-r--r--   0     1001      127     2417 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_node/src/replication/health.rs
+-rw-r--r--   0     1001      127     1070 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_node/src/replication/mod.rs
+-rw-r--r--   0     1001      127    14144 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_node/src/replication/replicator.rs
+-rw-r--r--   0     1001      127    11803 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_node/src/replication/service.rs
+-rw-r--r--   0     1001      127    15251 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_node/src/settings.rs
+-rw-r--r--   0     1001      127     1111 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_node/src/shards/errors.rs
+-rw-r--r--   0     1001      127     9990 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_node/src/shards/indexes.rs
+-rw-r--r--   0     1001      127    11085 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_node/src/shards/metadata.rs
+-rw-r--r--   0     1001      127     1140 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_node/src/shards/mod.rs
+-rw-r--r--   0     1001      127    26968 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_node/src/shards/shard_reader.rs
+-rw-r--r--   0     1001      127    21469 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_node/src/shards/shard_writer.rs
+-rw-r--r--   0     1001      127     1890 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_node/src/shards/versioning.rs
+-rw-r--r--   0     1001      127    10170 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_node/src/telemetry.rs
+-rw-r--r--   0     1001      127     6396 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_node/src/utils.rs
+-rw-r--r--   0     1001      127       42 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_node/test.sh
+-rw-r--r--   0     1001      127     1115 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_node/tests/common/mod.rs
+-rw-r--r--   0     1001      127    12731 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_node/tests/common/node_services.rs
+-rw-r--r--   0     1001      127     7823 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_node/tests/common/resources.rs
+-rw-r--r--   0     1001      127     8173 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_node/tests/test_date_range_search.rs
+-rw-r--r--   0     1001      127     4089 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_node/tests/test_download.rs
+-rw-r--r--   0     1001      127     1684 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_node/tests/test_merge.rs
+-rw-r--r--   0     1001      127     6003 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_node/tests/test_replication.rs
+-rw-r--r--   0     1001      127    22494 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_node/tests/test_search_relations.rs
+-rw-r--r--   0     1001      127     6958 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_node/tests/test_search_sorting.rs
+-rw-r--r--   0     1001      127     7044 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_node/tests/test_security_search.rs
+-rw-r--r--   0     1001      127     2508 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_node/tests/test_set_resource_from_storage.rs
+-rw-r--r--   0     1001      127     6862 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_node/tests/test_shards.rs
+-rw-r--r--   0     1001      127    10698 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_node/tests/test_suggest.rs
+-rw-r--r--   0     1001      127     5438 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_node/tests/test_vector_normalization.rs
+-rw-r--r--   0        0        0      931 1970-01-01 00:00:00.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_core/Cargo.toml
+-rw-r--r--   0     1001      127     5872 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_core/src/fs_state.rs
+-rw-r--r--   0     1001      127     2969 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_core/src/lib.rs
+-rw-r--r--   0     1001      127     2295 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_core/src/merge.rs
+-rw-r--r--   0     1001      127      906 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_core/src/metrics/meters/mod.rs
+-rw-r--r--   0     1001      127     5462 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_core/src/metrics/meters/prometheus.rs
+-rw-r--r--   0     1001      127     1702 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_core/src/metrics/metric/grpc_ops.rs
+-rw-r--r--   0     1001      127     1442 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_core/src/metrics/metric/mod.rs
+-rw-r--r--   0     1001      127     1950 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_core/src/metrics/metric/replication.rs
+-rw-r--r--   0     1001      127     2626 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_core/src/metrics/metric/request_time.rs
+-rw-r--r--   0     1001      127     1644 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_core/src/metrics/metric/shard_cache.rs
+-rw-r--r--   0     1001      127    21641 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_core/src/metrics/metric/tokio_runtime.rs
+-rw-r--r--   0     1001      127    16736 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_core/src/metrics/metric/tokio_tasks.rs
+-rw-r--r--   0     1001      127     3415 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_core/src/metrics/metric/vectors.rs
+-rw-r--r--   0     1001      127     1324 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_core/src/metrics/mod.rs
+-rw-r--r--   0     1001      127     3074 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_core/src/metrics/task_monitor.rs
+-rw-r--r--   0     1001      127     3920 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_core/src/metrics/tests.rs
+-rw-r--r--   0     1001      127     2990 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_core/src/paragraphs.rs
+-rw-r--r--   0     1001      127    17305 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_core/src/query_language/mod.rs
+-rw-r--r--   0     1001      127    15367 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_core/src/query_planner.rs
+-rw-r--r--   0     1001      127     2069 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_core/src/relations.rs
+-rw-r--r--   0     1001      127     8250 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_core/src/tantivy_replica.rs
+-rw-r--r--   0     1001      127     2603 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_core/src/texts.rs
+-rw-r--r--   0     1001      127     3551 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_core/src/vectors.rs
+-rw-r--r--   0        0        0      629 1970-01-01 00:00:00.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_paragraphs3/Cargo.toml
+-rw-r--r--   0     1001      127     7796 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_paragraphs3/src/fuzzy_query.rs
+-rw-r--r--   0     1001      127     1024 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_paragraphs3/src/lib.rs
+-rw-r--r--   0     1001      127     2780 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_paragraphs3/src/query_io.rs
+-rw-r--r--   0     1001      127    43069 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_paragraphs3/src/reader.rs
+-rw-r--r--   0     1001      127     4407 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_paragraphs3/src/schema.rs
+-rw-r--r--   0     1001      127    21349 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_paragraphs3/src/search_query.rs
+-rw-r--r--   0     1001      127    11723 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_paragraphs3/src/search_response.rs
+-rw-r--r--   0     1001      127     2846 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_paragraphs3/src/set_query.rs
+-rw-r--r--   0     1001      127     4090 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_paragraphs3/src/stop_words.rs
+-rw-r--r--   0     1001      127    17039 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_paragraphs3/src/writer.rs
+-rw-r--r--   0     1001      127       88 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_paragraphs3/stop_words/README.md
+-rw-r--r--   0     1001      127    19791 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_paragraphs3/stop_words/ar.json
+-rw-r--r--   0     1001      127     1923 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_paragraphs3/stop_words/az.json
+-rw-r--r--   0     1001      127    11684 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_paragraphs3/stop_words/bn.json
+-rw-r--r--   0     1001      127     2513 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_paragraphs3/stop_words/ca.json
+-rw-r--r--   0     1001      127    12802 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_paragraphs3/stop_words/ch.json
+-rw-r--r--   0     1001      127      730 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_paragraphs3/stop_words/da.json
+-rw-r--r--   0     1001      127     2090 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_paragraphs3/stop_words/de.json
+-rw-r--r--   0     1001      127     6284 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_paragraphs3/stop_words/el.json
+-rw-r--r--   0     1001      127     1473 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_paragraphs3/stop_words/en.json
+-rw-r--r--   0     1001      127     3451 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_paragraphs3/stop_words/es.json
+-rw-r--r--   0     1001      127     3182 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_paragraphs3/stop_words/eu.json
+-rw-r--r--   0     1001      127     2126 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_paragraphs3/stop_words/extract.py
+-rw-r--r--   0     1001      127     2748 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_paragraphs3/stop_words/fi.json
+-rw-r--r--   0     1001      127     1388 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_paragraphs3/stop_words/fr.json
+-rw-r--r--   0     1001      127     5716 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_paragraphs3/stop_words/he.json
+-rw-r--r--   0     1001      127     2108 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_paragraphs3/stop_words/hu.json
+-rw-r--r--   0     1001      127     8721 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_paragraphs3/stop_words/id.json
+-rw-r--r--   0     1001      127     2535 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_paragraphs3/stop_words/it.json
+-rw-r--r--   0     1001      127    11737 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_paragraphs3/stop_words/kk.json
+-rw-r--r--   0     1001      127     7730 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_paragraphs3/stop_words/ne.json
+-rw-r--r--   0     1001      127      756 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_paragraphs3/stop_words/nl.json
+-rw-r--r--   0     1001      127     1447 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_paragraphs3/stop_words/no.json
+-rw-r--r--   0     1001      127     2055 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_paragraphs3/stop_words/pt.json
+-rw-r--r--   0     1001      127     3327 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_paragraphs3/stop_words/ro.json
+-rw-r--r--   0     1001      127     3856 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_paragraphs3/stop_words/ru.json
+-rw-r--r--   0     1001      127    23032 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_paragraphs3/stop_words/sl.json
+-rw-r--r--   0     1001      127      993 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_paragraphs3/stop_words/sv.json
+-rw-r--r--   0     1001      127     5424 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_paragraphs3/stop_words/tg.json
+-rw-r--r--   0     1001      127      491 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_paragraphs3/stop_words/tr.json
+-rw-r--r--   0        0        0      742 1970-01-01 00:00:00.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_vectors/Cargo.toml
+-rw-r--r--   0     1001      127       69 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_vectors/README.md
+-rw-r--r--   0     1001      127       43 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_vectors/docs/README.md
+-rw-r--r--   0     1001      127    25718 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_vectors/docs/labels.drawio.svg
+-rw-r--r--   0     1001      127    12340 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_vectors/src/data_point/disk_hnsw.rs
+-rw-r--r--   0     1001      127    24470 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_vectors/src/data_point/mod.rs
+-rw-r--r--   0     1001      127    11214 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_vectors/src/data_point/node.rs
+-rw-r--r--   0     1001      127    15068 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_vectors/src/data_point/ops_hnsw.rs
+-rw-r--r--   0     1001      127     1741 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_vectors/src/data_point/params.rs
+-rw-r--r--   0     1001      127     3952 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_vectors/src/data_point/ram_hnsw.rs
+-rw-r--r--   0     1001      127    14175 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_vectors/src/data_point/tests.rs
+-rw-r--r--   0     1001      127     5798 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_vectors/src/data_point_provider/garbage_collector.rs
+-rw-r--r--   0     1001      127     2777 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_vectors/src/data_point_provider/mod.rs
+-rw-r--r--   0     1001      127    10613 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_vectors/src/data_point_provider/reader.rs
+-rw-r--r--   0     1001      127     2304 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_vectors/src/data_point_provider/replication.rs
+-rw-r--r--   0     1001      127     5288 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_vectors/src/data_point_provider/state.rs
+-rw-r--r--   0     1001      127    20587 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_vectors/src/data_point_provider/writer.rs
+-rw-r--r--   0     1001      127    23710 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_vectors/src/data_types/data_store.rs
+-rw-r--r--   0     1001      127     6916 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_vectors/src/data_types/dtrie_ram.rs
+-rw-r--r--   0     1001      127     1959 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_vectors/src/data_types/mod.rs
+-rw-r--r--   0     1001      127     6143 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_vectors/src/data_types/trie.rs
+-rw-r--r--   0     1001      127     2904 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_vectors/src/data_types/trie_ram.rs
+-rw-r--r--   0     1001      127     4433 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_vectors/src/data_types/vector.rs
+-rw-r--r--   0     1001      127    10472 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_vectors/src/formula/mod.rs
+-rw-r--r--   0     1001      127     2165 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_vectors/src/lib.rs
+-rw-r--r--   0     1001      127     1278 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_vectors/src/service/mod.rs
+-rw-r--r--   0     1001      127     1897 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_vectors/src/service/query_io.rs
+-rw-r--r--   0     1001      127    17312 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_vectors/src/service/reader.rs
+-rw-r--r--   0     1001      127    15104 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_vectors/src/service/writer.rs
+-rw-r--r--   0     1001      127     1668 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_vectors/src/utils.rs
+-rw-r--r--   0     1001      127     2884 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_vectors/tests/test_merge.rs
+-rw-r--r--   0        0        0      708 1970-01-01 00:00:00.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_relations2/Cargo.toml
+-rw-r--r--   0     1001      127     3593 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_relations2/src/io_maps.rs
+-rw-r--r--   0     1001      127      916 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_relations2/src/lib.rs
+-rw-r--r--   0     1001      127    17039 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_relations2/src/reader.rs
+-rw-r--r--   0     1001      127     7123 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_relations2/src/schema.rs
+-rw-r--r--   0     1001      127     7990 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_relations2/src/writer.rs
+-rw-r--r--   0     1001      127     1802 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_relations2/tests/common/mod.rs
+-rw-r--r--   0     1001      127     9523 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_relations2/tests/test_reader.rs
+-rw-r--r--   0     1001      127     3296 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_relations2/tests/test_writer.rs
+-rw-r--r--   0        0        0      361 1970-01-01 00:00:00.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_procs/Cargo.toml
+-rw-r--r--   0     1001      127     3409 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_procs/src/lib.rs
+-rw-r--r--   0     1001      127     2885 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_procs/src/measure.rs
+-rw-r--r--   0     1001      127     1081 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_procs/tests/dont_compile/actor_defined_twice.rs
+-rw-r--r--   0     1001      127      222 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_procs/tests/dont_compile/actor_defined_twice.stderr
+-rw-r--r--   0     1001      127     1038 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_procs/tests/dont_compile/actor_not_defined.rs
+-rw-r--r--   0     1001      127      327 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_procs/tests/dont_compile/actor_not_defined.stderr
+-rw-r--r--   0     1001      127     1086 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_procs/tests/dont_compile/metric_defined_twice.rs
+-rw-r--r--   0     1001      127      249 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_procs/tests/dont_compile/metric_defined_twice.stderr
+-rw-r--r--   0     1001      127     1046 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_procs/tests/dont_compile/wrong_actor.rs
+-rw-r--r--   0     1001      127     1303 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_procs/tests/dont_compile/wrong_actor.stderr
+-rw-r--r--   0     1001      127     1408 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_procs/tests/test_measure.rs
+-rw-r--r--   0        0        0      501 1970-01-01 00:00:00.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_protos/Cargo.toml
+-rw-r--r--   0     1001      127     2155 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_protos/build.rs
+-rw-r--r--   0     1001      127    26110 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_protos/src/fdbwriter.rs
+-rw-r--r--   0     1001      127        0 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_protos/src/google.protobuf.rs
+-rw-r--r--   0     1001      127     9795 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_protos/src/knowledgebox.rs
+-rw-r--r--   0     1001      127     1256 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_protos/src/lib.rs
+-rw-r--r--   0     1001      127    77311 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_protos/src/nodereader.rs
+-rw-r--r--   0     1001      127    10240 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_protos/src/noderesources.rs
+-rw-r--r--   0     1001      127    46404 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_protos/src/nodewriter.rs
+-rw-r--r--   0     1001      127    19106 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_protos/src/replication.rs
+-rw-r--r--   0     1001      127    33352 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_protos/src/resources.rs
+-rw-r--r--   0     1001      127     5528 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_protos/src/utils.rs
+-rw-r--r--   0        0        0      399 1970-01-01 00:00:00.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_texts2/Cargo.toml
+-rw-r--r--   0     1001      127      931 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_texts2/src/lib.rs
+-rw-r--r--   0     1001      127     2755 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_texts2/src/query_io.rs
+-rw-r--r--   0     1001      127    22721 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_texts2/src/reader.rs
+-rw-r--r--   0     1001      127     3105 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_texts2/src/schema.rs
+-rw-r--r--   0     1001      127     8682 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_texts2/src/search_query.rs
+-rw-r--r--   0     1001      127    10092 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_texts2/src/writer.rs
+-rw-r--r--   0     1001      127     3435 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_texts2/tests/common/mod.rs
+-rw-r--r--   0     1001      127     2152 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_texts2/tests/test_reader.rs
+-rw-r--r--   0     1001      127     9567 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_texts2/tests/test_search.rs
+-rw-r--r--   0     1001      127     1249 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_texts2/tests/test_streaming.rs
+-rw-r--r--   0     1001      127     3523 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_texts2/tests/test_writer.rs
+-rw-r--r--   0        0        0      629 1970-01-01 00:00:00.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_paragraphs2/Cargo.toml
+-rw-r--r--   0     1001      127     7796 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_paragraphs2/src/fuzzy_query.rs
+-rw-r--r--   0     1001      127     1009 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_paragraphs2/src/lib.rs
+-rw-r--r--   0     1001      127     2780 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_paragraphs2/src/query_io.rs
+-rw-r--r--   0     1001      127    43124 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_paragraphs2/src/reader.rs
+-rw-r--r--   0     1001      127     4808 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_paragraphs2/src/schema.rs
+-rw-r--r--   0     1001      127    22494 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_paragraphs2/src/search_query.rs
+-rw-r--r--   0     1001      127    11391 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_paragraphs2/src/search_response.rs
+-rw-r--r--   0     1001      127     4090 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_paragraphs2/src/stop_words.rs
+-rw-r--r--   0     1001      127    17947 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_paragraphs2/src/writer.rs
+-rw-r--r--   0     1001      127       88 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_paragraphs2/stop_words/README.md
+-rw-r--r--   0     1001      127    19791 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_paragraphs2/stop_words/ar.json
+-rw-r--r--   0     1001      127     1923 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_paragraphs2/stop_words/az.json
+-rw-r--r--   0     1001      127    11684 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_paragraphs2/stop_words/bn.json
+-rw-r--r--   0     1001      127     2513 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_paragraphs2/stop_words/ca.json
+-rw-r--r--   0     1001      127    12802 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_paragraphs2/stop_words/ch.json
+-rw-r--r--   0     1001      127      730 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_paragraphs2/stop_words/da.json
+-rw-r--r--   0     1001      127     2090 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_paragraphs2/stop_words/de.json
+-rw-r--r--   0     1001      127     6284 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_paragraphs2/stop_words/el.json
+-rw-r--r--   0     1001      127     1473 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_paragraphs2/stop_words/en.json
+-rw-r--r--   0     1001      127     3451 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_paragraphs2/stop_words/es.json
+-rw-r--r--   0     1001      127     3182 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_paragraphs2/stop_words/eu.json
+-rw-r--r--   0     1001      127     2126 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_paragraphs2/stop_words/extract.py
+-rw-r--r--   0     1001      127     2748 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_paragraphs2/stop_words/fi.json
+-rw-r--r--   0     1001      127     1388 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_paragraphs2/stop_words/fr.json
+-rw-r--r--   0     1001      127     5716 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_paragraphs2/stop_words/he.json
+-rw-r--r--   0     1001      127     2108 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_paragraphs2/stop_words/hu.json
+-rw-r--r--   0     1001      127     8721 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_paragraphs2/stop_words/id.json
+-rw-r--r--   0     1001      127     2535 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_paragraphs2/stop_words/it.json
+-rw-r--r--   0     1001      127    11737 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_paragraphs2/stop_words/kk.json
+-rw-r--r--   0     1001      127     7730 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_paragraphs2/stop_words/ne.json
+-rw-r--r--   0     1001      127      756 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_paragraphs2/stop_words/nl.json
+-rw-r--r--   0     1001      127     1447 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_paragraphs2/stop_words/no.json
+-rw-r--r--   0     1001      127     2055 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_paragraphs2/stop_words/pt.json
+-rw-r--r--   0     1001      127     3327 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_paragraphs2/stop_words/ro.json
+-rw-r--r--   0     1001      127     3856 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_paragraphs2/stop_words/ru.json
+-rw-r--r--   0     1001      127    23032 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_paragraphs2/stop_words/sl.json
+-rw-r--r--   0     1001      127      993 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_paragraphs2/stop_words/sv.json
+-rw-r--r--   0     1001      127     5424 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_paragraphs2/stop_words/tg.json
+-rw-r--r--   0     1001      127      491 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_paragraphs2/stop_words/tr.json
+-rw-r--r--   0        0        0      943 1970-01-01 00:00:00.000000 nucliadb_node_binding-3.0.3.post1254/Cargo.toml
+-rw-r--r--   0     1001      127     1553 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/CHANGELOG.md
+-rw-r--r--   0     1001      127      895 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/Makefile
+-rw-r--r--   0     1001      127       52 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/README.md
+-rwxr-xr-x   0     1001      127      978 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/cov.sh
+-rw-r--r--   0     1001      127     1309 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/pyproject.toml
+-rw-r--r--   0     1001      127     2195 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/src/collect_garbage.rs
+-rw-r--r--   0     1001      127     1212 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/src/errors.rs
+-rw-r--r--   0     1001      127     2337 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/src/lib.rs
+-rw-r--r--   0     1001      127     9405 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/src/reader.rs
+-rw-r--r--   0     1001      127     2154 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/src/update.rs
+-rw-r--r--   0     1001      127     8996 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/src/writer.rs
+-rw-r--r--   0     1001      127      835 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/tests/__init__.py
+-rw-r--r--   0     1001      127      892 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/tests/conftest.py
+-rw-r--r--   0     1001      127     3903 2024-05-06 15:22:06.000000 nucliadb_node_binding-3.0.3.post1254/tests/integration/test_indexing.py
+-rw-r--r--   0        0        0      401 1970-01-01 00:00:00.000000 nucliadb_node_binding-3.0.3.post1254/PKG-INFO
```

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_core/Cargo.toml` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_core/Cargo.toml`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_core/src/fs_state.rs` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_core/src/fs_state.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_core/src/lib.rs` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_core/src/lib.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_core/src/merge.rs` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_core/src/merge.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_core/src/metrics/meters/mod.rs` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_core/src/metrics/meters/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_core/src/metrics/meters/prometheus.rs` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_core/src/metrics/meters/prometheus.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_core/src/metrics/metric/grpc_ops.rs` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_core/src/metrics/metric/grpc_ops.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_core/src/metrics/metric/mod.rs` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_core/src/metrics/metric/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_core/src/metrics/metric/replication.rs` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_core/src/metrics/metric/replication.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_core/src/metrics/metric/request_time.rs` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_core/src/metrics/metric/request_time.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_core/src/metrics/metric/shard_cache.rs` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_core/src/metrics/metric/shard_cache.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_core/src/metrics/metric/tokio_runtime.rs` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_core/src/metrics/metric/tokio_runtime.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_core/src/metrics/metric/tokio_tasks.rs` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_core/src/metrics/metric/tokio_tasks.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_core/src/metrics/metric/vectors.rs` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_core/src/metrics/metric/vectors.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_core/src/metrics/mod.rs` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_core/src/metrics/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_core/src/metrics/task_monitor.rs` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_core/src/metrics/task_monitor.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_core/src/metrics/tests.rs` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_core/src/metrics/tests.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_core/src/paragraphs.rs` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_core/src/paragraphs.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_core/src/query_language/mod.rs` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_core/src/query_language/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_core/src/query_planner.rs` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_core/src/query_planner.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_core/src/relations.rs` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_core/src/relations.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_core/src/tantivy_replica.rs` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_core/src/tantivy_replica.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_core/src/texts.rs` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_core/src/texts.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_core/src/vectors.rs` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_core/src/vectors.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_relations2/Cargo.toml` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_relations2/Cargo.toml`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_relations2/src/io_maps.rs` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_relations2/src/io_maps.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_relations2/src/lib.rs` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_relations2/src/lib.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_relations2/src/reader.rs` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_relations2/src/reader.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_relations2/src/schema.rs` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_relations2/src/schema.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_relations2/src/writer.rs` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_relations2/src/writer.rs`

 * *Files 1% similar despite different names*

```diff
@@ -120,15 +120,15 @@
             writer,
             schema: field_schema,
             config: config.clone(),
         })
     }
 
     #[tracing::instrument(skip_all)]
-    pub fn create(config: &RelationConfig) -> NodeResult<Self> {
+    pub fn create(config: RelationConfig) -> NodeResult<Self> {
         Self::try_create_index_dir(&config.path)?;
 
         let settings = IndexSettings {
             ..Default::default()
         };
         let field_schema = Schema::new();
         let mut index_builder = Index::builder().schema(field_schema.schema.clone());
@@ -136,15 +136,15 @@
         let index = index_builder.create_in_dir(&config.path).expect("Index directory should exist");
         let writer = index.writer_with_num_threads(1, TANTIVY_INDEX_ARENA_MEMORY).unwrap();
 
         Ok(RelationsWriterService {
             index,
             writer,
             schema: field_schema,
-            config: config.clone(),
+            config,
         })
     }
 
     fn try_create_index_dir(path: &Path) -> NodeResult<()> {
         let result = fs::create_dir(path);
         if let Err(error) = result {
             if path.exists() {
```

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_relations2/tests/common/mod.rs` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_relations2/tests/common/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_relations2/tests/test_reader.rs` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_relations2/tests/test_reader.rs`

 * *Files 2% similar despite different names*

```diff
@@ -31,21 +31,22 @@
 use nucliadb_core::Channel;
 use nucliadb_relations2::reader::RelationsReaderService;
 use nucliadb_relations2::writer::RelationsWriterService;
 use tempfile::TempDir;
 
 fn create_reader() -> NodeResult<RelationsReaderService> {
     let dir = TempDir::new().unwrap();
+    let shard_path = dir.path().join("relations");
     let config = RelationConfig {
-        path: dir.path().join("relations"),
+        path: shard_path.clone(),
         channel: Channel::EXPERIMENTAL,
     };
 
-    let mut writer = RelationsWriterService::create(&config)?;
-    let reader = RelationsReaderService::open(&config.path)?;
+    let mut writer = RelationsWriterService::create(config)?;
+    let reader = RelationsReaderService::open(&shard_path)?;
 
     writer.set_resource(&Resource {
         resource: Some(ResourceId {
             uuid: "uuid".to_string(),
             shard_id: "shard_id".to_string(),
         }),
         relations: vec![
@@ -120,21 +121,22 @@
 
     Ok(reader)
 }
 
 #[test]
 fn test_start_new_reader_after_a_writer() -> NodeResult<()> {
     let dir = TempDir::new()?;
+    let shard_path = dir.path().join("relations");
     let config = RelationConfig {
-        path: dir.path().join("relations"),
+        path: shard_path.clone(),
         channel: Channel::EXPERIMENTAL,
     };
 
-    let _writer = RelationsWriterService::create(&config)?;
-    let reader: Result<RelationsReaderService, nucliadb_core::Error> = RelationsReaderService::open(&config.path);
+    let _writer = RelationsWriterService::create(config)?;
+    let reader: Result<RelationsReaderService, nucliadb_core::Error> = RelationsReaderService::open(&shard_path);
     assert!(reader.is_ok());
 
     Ok(())
 }
 
 #[test]
 fn test_stored_ids() -> NodeResult<()> {
```

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_relations2/tests/test_writer.rs` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_relations2/tests/test_writer.rs`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 fn test_index_docs() -> NodeResult<()> {
     let dir = TempDir::new().unwrap();
     let config = RelationConfig {
         path: dir.path().join("relations"),
         channel: Channel::EXPERIMENTAL,
     };
 
-    let mut writer = RelationsWriterService::create(&config).unwrap();
+    let mut writer = RelationsWriterService::create(config).unwrap();
 
     writer.set_resource(&Resource {
         resource: Some(ResourceId {
             uuid: "uuid".to_string(),
             shard_id: "shard_id".to_string(),
         }),
         relations: vec![
```

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_protos/build.rs` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_protos/build.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_protos/src/fdbwriter.rs` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_protos/src/fdbwriter.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_protos/src/knowledgebox.rs` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_protos/src/knowledgebox.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_protos/src/lib.rs` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_protos/src/lib.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_protos/src/nodereader.rs` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_protos/src/nodereader.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_protos/src/noderesources.rs` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_protos/src/noderesources.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_protos/src/nodewriter.rs` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_protos/src/nodewriter.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_protos/src/replication.rs` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_protos/src/replication.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_protos/src/resources.rs` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_protos/src/resources.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_protos/src/utils.rs` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_protos/src/utils.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_paragraphs3/Cargo.toml` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_paragraphs3/Cargo.toml`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_paragraphs3/src/fuzzy_query.rs` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_paragraphs3/src/fuzzy_query.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_paragraphs3/src/lib.rs` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_paragraphs3/src/lib.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_paragraphs3/src/query_io.rs` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_paragraphs3/src/query_io.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_paragraphs3/src/reader.rs` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_paragraphs2/src/reader.rs`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,16 @@
 use tantivy::query::{AllQuery, Query, QueryParser};
 use tantivy::schema::*;
 use tantivy::{DocAddress, Index, IndexReader, LeasedItem, ReloadPolicy};
 
 use super::schema::ParagraphSchema;
 use crate::search_query;
 use crate::search_query::SharedTermC;
-use crate::search_response::{extract_labels, SearchBm25Response, SearchFacetsResponse, SearchIntResponse};
+use crate::search_response::extract_labels;
+use crate::search_response::{SearchBm25Response, SearchFacetsResponse, SearchIntResponse};
 
 const FUZZY_DISTANCE: u8 = 1;
 const NUMBER_OF_RESULTS_SUGGEST: usize = 10;
 
 pub struct ParagraphReaderService {
     index: Index,
     pub schema: ParagraphSchema,
@@ -138,15 +139,14 @@
 
         let v = time.elapsed().as_millis();
         debug!("{id:?} - Creating query: starts at {v} ms");
 
         let parser = QueryParser::for_index(&self.index, vec![self.schema.text]);
         let results = request.result_per_page as usize;
         let offset = results * request.page_number as usize;
-
         let facets: Vec<_> = request
             .faceted
             .as_ref()
             .iter()
             .flat_map(|v| v.labels.iter())
             .filter(|s| ParagraphReaderService::is_valid_facet(s))
             .cloned()
@@ -596,27 +596,28 @@
             ..Default::default()
         }
     }
     #[test]
     fn test_total_number_of_results() -> NodeResult<()> {
         const UUID: &str = "f56c58ac-b4f9-4d61-a077-ffccaadd0001";
         let dir = TempDir::new().unwrap();
+        let shard_path = dir.path().join("paragraphs");
         let psc = ParagraphConfig {
-            path: dir.path().join("paragraphs"),
+            path: shard_path.clone(),
         };
         let seconds = SystemTime::now().duration_since(SystemTime::UNIX_EPOCH).map(|t| t.as_secs() as i64).unwrap();
         let timestamp = Timestamp {
             seconds,
             nanos: 0,
         };
 
-        let mut paragraph_writer_service = ParagraphWriterService::create(&psc).unwrap();
+        let mut paragraph_writer_service = ParagraphWriterService::create(psc).unwrap();
         let resource1 = create_resource("shard1".to_string(), timestamp);
-        paragraph_writer_service.set_resource(&resource1)?;
-        let paragraph_reader_service = ParagraphReaderService::open(&psc.path).unwrap();
+        let _ = paragraph_writer_service.set_resource(&resource1);
+        let paragraph_reader_service = ParagraphReaderService::open(&shard_path).unwrap();
         let context = ParagraphsContext::default();
 
         // Search on all paragraphs faceted
         let search = ProtosRequest {
             id: "shard1".to_string(),
             uuid: UUID.to_string(),
             body: "".to_string(),
@@ -657,28 +658,29 @@
         Ok(())
     }
 
     #[test]
     fn test_filtered_search() -> NodeResult<()> {
         const UUID: &str = "f56c58ac-b4f9-4d61-a077-ffccaadd0001";
         let dir = TempDir::new().unwrap();
+        let shard_path = dir.path().join("paragraphs");
         let psc = ParagraphConfig {
-            path: dir.path().join("paragraphs"),
+            path: shard_path.clone(),
         };
         let seconds = SystemTime::now().duration_since(SystemTime::UNIX_EPOCH).map(|t| t.as_secs() as i64).unwrap();
         let timestamp = Timestamp {
             seconds,
             nanos: 0,
         };
 
-        let mut paragraph_writer_service = ParagraphWriterService::create(&psc).unwrap();
+        let mut paragraph_writer_service = ParagraphWriterService::create(psc).unwrap();
         let resource1 = create_resource("shard1".to_string(), timestamp);
-        paragraph_writer_service.set_resource(&resource1)?;
+        let _ = paragraph_writer_service.set_resource(&resource1);
 
-        let paragraph_reader_service = ParagraphReaderService::open(&psc.path).unwrap();
+        let paragraph_reader_service = ParagraphReaderService::open(&shard_path).unwrap();
 
         let reader = paragraph_writer_service.index.reader()?;
         let searcher = reader.searcher();
         let mut context = ParagraphsContext::default();
         let (_top_docs, count) = searcher.search(&AllQuery, &(TopDocs::with_limit(10), Count))?;
         assert_eq!(count, 4);
 
@@ -729,26 +731,27 @@
         Ok(())
     }
 
     #[test]
     fn test_new_paragraph() -> NodeResult<()> {
         const UUID: &str = "f56c58ac-b4f9-4d61-a077-ffccaadd0001";
         let dir = TempDir::new().unwrap();
+        let shard_path = dir.path().join("paragraphs");
         let psc = ParagraphConfig {
-            path: dir.path().join("paragraphs"),
+            path: shard_path.clone(),
         };
         let seconds = SystemTime::now().duration_since(SystemTime::UNIX_EPOCH).map(|t| t.as_secs() as i64).unwrap();
         let timestamp = Timestamp {
             seconds,
             nanos: 0,
         };
-        let mut paragraph_writer_service = ParagraphWriterService::create(&psc).unwrap();
+        let mut paragraph_writer_service = ParagraphWriterService::create(psc).unwrap();
         let resource1 = create_resource("shard1".to_string(), timestamp);
-        paragraph_writer_service.set_resource(&resource1)?;
-        let paragraph_reader_service = ParagraphReaderService::open(&psc.path).unwrap();
+        let _ = paragraph_writer_service.set_resource(&resource1);
+        let paragraph_reader_service = ParagraphReaderService::open(&shard_path).unwrap();
         let reader = paragraph_writer_service.index.reader()?;
         let searcher = reader.searcher();
         let empty_context = ParagraphsContext::default();
         let (_top_docs, count) = searcher.search(&AllQuery, &(TopDocs::with_limit(10), Count))?;
         assert_eq!(count, 4);
 
         let faceted = Faceted {
@@ -983,28 +986,29 @@
         assert_eq!(count, 4);
         Ok(())
     }
 
     #[test]
     fn test_search_paragraph_with_timestamps() -> NodeResult<()> {
         let dir = TempDir::new().unwrap();
+        let shard_path = dir.path().join("paragraphs");
         let psc = ParagraphConfig {
-            path: dir.path().join("paragraphs"),
+            path: shard_path.clone(),
         };
         let time_baseline = Timestamp {
             seconds: 2,
             nanos: 0,
         };
 
-        let mut paragraph_writer_service = ParagraphWriterService::create(&psc).unwrap();
+        let mut paragraph_writer_service = ParagraphWriterService::create(psc).unwrap();
         let resource1 = create_resource("shard1".to_string(), time_baseline.clone());
 
-        paragraph_writer_service.set_resource(&resource1)?;
+        let _ = paragraph_writer_service.set_resource(&resource1);
 
-        let paragraph_reader_service = ParagraphReaderService::open(&psc.path).unwrap();
+        let paragraph_reader_service = ParagraphReaderService::open(&shard_path).unwrap();
 
         let reader = paragraph_writer_service.index.reader()?;
         let searcher = reader.searcher();
         let (_top_docs, count) = searcher.search(&AllQuery, &(TopDocs::with_limit(10), Count))?;
         assert_eq!(count, 4);
 
         fn do_search(paragraph_reader_service: &ParagraphReaderService, timestamps: Timestamps) -> i32 {
```

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_paragraphs3/src/schema.rs` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_paragraphs3/src/schema.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_paragraphs3/src/search_query.rs` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_paragraphs3/src/search_query.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_paragraphs3/src/search_response.rs` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_paragraphs3/src/search_response.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_paragraphs3/src/set_query.rs` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_paragraphs3/src/set_query.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_paragraphs3/src/stop_words.rs` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_paragraphs3/src/stop_words.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_paragraphs3/src/writer.rs` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_paragraphs3/src/writer.rs`

 * *Files 0% similar despite different names*

```diff
@@ -153,15 +153,15 @@
         let safe_state = tantivy_replica::compute_safe_replica_state(params, &self.index)?;
         Ok(IndexFiles::Tantivy(safe_state))
     }
 }
 
 impl ParagraphWriterService {
     #[tracing::instrument(skip_all)]
-    pub fn create(config: &ParagraphConfig) -> NodeResult<ParagraphWriterService> {
+    pub fn create(config: ParagraphConfig) -> NodeResult<ParagraphWriterService> {
         let paragraph_schema = ParagraphSchema::default();
 
         fs::create_dir(&config.path)?;
 
         let mut index_builder = Index::builder().schema(paragraph_schema.schema.clone());
         let settings = IndexSettings {
             sort_by_field: Some(IndexSortByField {
@@ -176,15 +176,15 @@
 
         let writer = index.writer_with_num_threads(1, 6_000_000)?;
 
         Ok(ParagraphWriterService {
             index,
             writer,
             schema: paragraph_schema,
-            config: config.clone(),
+            config,
         })
     }
     #[tracing::instrument(skip_all)]
     pub fn open(config: &ParagraphConfig) -> NodeResult<ParagraphWriterService> {
         let paragraph_schema = ParagraphSchema::default();
 
         let index = Index::open_in_dir(&config.path)?;
@@ -430,15 +430,15 @@
     #[test]
     fn test_new_writer() -> NodeResult<()> {
         let dir = TempDir::new().unwrap();
         let psc = ParagraphConfig {
             path: dir.path().join("paragraphs"),
         };
 
-        let mut paragraph_writer_service = ParagraphWriterService::create(&psc).unwrap();
+        let mut paragraph_writer_service = ParagraphWriterService::create(psc).unwrap();
         let resource1 = create_resource("shard1".to_string());
         let _ = paragraph_writer_service.set_resource(&resource1);
         let _ = paragraph_writer_service.set_resource(&resource1);
 
         let reader = paragraph_writer_service.index.reader()?;
         let searcher = reader.searcher();
```

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_paragraphs3/stop_words/ar.json` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_paragraphs3/stop_words/ar.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_paragraphs3/stop_words/az.json` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_paragraphs3/stop_words/az.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_paragraphs3/stop_words/bn.json` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_paragraphs3/stop_words/bn.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_paragraphs3/stop_words/ca.json` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_paragraphs3/stop_words/ca.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_paragraphs3/stop_words/ch.json` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_paragraphs3/stop_words/ch.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_paragraphs3/stop_words/da.json` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_paragraphs3/stop_words/da.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_paragraphs3/stop_words/de.json` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_paragraphs3/stop_words/de.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_paragraphs3/stop_words/el.json` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_paragraphs3/stop_words/el.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_paragraphs3/stop_words/en.json` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_paragraphs3/stop_words/en.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_paragraphs3/stop_words/es.json` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_paragraphs3/stop_words/es.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_paragraphs3/stop_words/eu.json` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_paragraphs3/stop_words/eu.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_paragraphs3/stop_words/extract.py` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_paragraphs3/stop_words/extract.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_paragraphs3/stop_words/fi.json` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_paragraphs3/stop_words/fi.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_paragraphs3/stop_words/fr.json` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_paragraphs3/stop_words/fr.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_paragraphs3/stop_words/he.json` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_paragraphs3/stop_words/he.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_paragraphs3/stop_words/hu.json` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_paragraphs3/stop_words/hu.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_paragraphs3/stop_words/id.json` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_paragraphs3/stop_words/id.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_paragraphs3/stop_words/it.json` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_paragraphs3/stop_words/it.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_paragraphs3/stop_words/kk.json` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_paragraphs3/stop_words/kk.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_paragraphs3/stop_words/ne.json` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_paragraphs3/stop_words/ne.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_paragraphs3/stop_words/nl.json` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_paragraphs3/stop_words/nl.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_paragraphs3/stop_words/no.json` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_paragraphs3/stop_words/no.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_paragraphs3/stop_words/pt.json` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_paragraphs3/stop_words/pt.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_paragraphs3/stop_words/ro.json` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_paragraphs3/stop_words/ro.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_paragraphs3/stop_words/ru.json` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_paragraphs3/stop_words/ru.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_paragraphs3/stop_words/sl.json` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_paragraphs3/stop_words/sl.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_paragraphs3/stop_words/sv.json` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_paragraphs3/stop_words/sv.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_paragraphs3/stop_words/tg.json` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_paragraphs3/stop_words/tg.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_node/Cargo.toml` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_node/Cargo.toml`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_node/.rustc_info.json` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_node/.rustc_info.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_node/Makefile` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_node/Makefile`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_node/README.md` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_node/README.md`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_node/nucliadb_node/__init__.py` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_node/nucliadb_node/__init__.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_node/nucliadb_node/app.py` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_node/nucliadb_node/app.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_node/nucliadb_node/indexer.py` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_node/nucliadb_node/indexer.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_node/nucliadb_node/listeners/__init__.py` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_node/nucliadb_node/listeners/__init__.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_node/nucliadb_node/listeners/indexed_publisher.py` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_node/nucliadb_node/listeners/indexed_publisher.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_node/nucliadb_node/pull.py` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_node/nucliadb_node/pull.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_node/nucliadb_node/service.py` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_node/nucliadb_node/service.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_node/nucliadb_node/settings.py` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_node/nucliadb_node/settings.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_node/nucliadb_node/signals.py` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_node/nucliadb_node/signals.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_node/nucliadb_node/tests/__init__.py` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_node/nucliadb_node/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_node/nucliadb_node/tests/conftest.py` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_node/nucliadb_node/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_node/nucliadb_node/tests/fixtures.py` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_node/nucliadb_node/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_node/nucliadb_node/tests/integration/test_indexing.py` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_node/nucliadb_node/tests/integration/test_indexing.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_node/nucliadb_node/tests/unit/test_app.py` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_node/nucliadb_node/tests/unit/test_app.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_node/nucliadb_node/tests/unit/test_indexed_publisher.py` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_node/nucliadb_node/tests/unit/test_indexed_publisher.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_node/nucliadb_node/tests/unit/test_indexer.py` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_node/nucliadb_node/tests/unit/test_indexer.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_node/nucliadb_node/tests/unit/test_pull.py` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_node/nucliadb_node/tests/unit/test_pull.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_node/nucliadb_node/writer.py` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_node/nucliadb_node/writer.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_node/setup.py` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_node/setup.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_node/src/analytics/blocking.rs` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_node/src/analytics/blocking.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_node/src/analytics/mod.rs` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_node/src/analytics/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_node/src/analytics/payload.rs` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_node/src/analytics/payload.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_node/src/analytics/sender.rs` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_node/src/analytics/sender.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_node/src/analytics/sink.rs` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_node/src/analytics/sink.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_node/src/analytics/sync.rs` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_node/src/analytics/sync.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_node/src/bin/reader.rs` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_node/src/bin/reader.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_node/src/bin/writer.rs` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_node/src/bin/writer.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_node/src/cache/mod.rs` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_node/src/cache/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_node/src/cache/reader_cache.rs` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_node/src/cache/reader_cache.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_node/src/cache/resource_cache.rs` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_node/src/cache/resource_cache.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_node/src/cache/writer_cache.rs` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_node/src/cache/writer_cache.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_node/src/disk_structure.rs` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_node/src/disk_structure.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_node/src/errors.rs` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_node/src/errors.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_node/src/grpc/collect_garbage.rs` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_node/src/grpc/collect_garbage.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_node/src/grpc/grpc_reader.rs` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_node/src/grpc/grpc_reader.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_node/src/grpc/grpc_writer.rs` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_node/src/grpc/grpc_writer.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_node/src/grpc/middleware/debug.rs` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_node/src/grpc/middleware/debug.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_node/src/grpc/middleware/metrics.rs` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_node/src/grpc/middleware/metrics.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_node/src/grpc/middleware/mod.rs` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_node/src/grpc/middleware/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_node/src/grpc/middleware/telemetry.rs` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_node/src/grpc/middleware/telemetry.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_node/src/grpc/mod.rs` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_node/src/grpc/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_node/src/grpc/update.rs` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_node/src/grpc/update.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_node/src/http_server/metrics_service.rs` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_node/src/http_server/metrics_service.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_node/src/http_server/mod.rs` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_node/src/http_server/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_node/src/http_server/traces_service.rs` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_node/src/http_server/traces_service.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_node/src/lib.rs` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_node/src/lib.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_node/src/lifecycle.rs` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_node/src/lifecycle.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_node/src/merge/global.rs` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_node/src/merge/global.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_node/src/merge/mod.rs` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_node/src/merge/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_node/src/merge/scheduler.rs` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_node/src/merge/scheduler.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_node/src/merge/work.rs` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_node/src/merge/work.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_node/src/node_metadata.rs` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_node/src/node_metadata.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_node/src/replication/health.rs` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_node/src/replication/health.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_node/src/replication/mod.rs` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_node/src/replication/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_node/src/replication/replicator.rs` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_node/src/replication/replicator.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_node/src/replication/service.rs` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_node/src/replication/service.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_node/src/settings.rs` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_node/src/settings.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_node/src/shards/errors.rs` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_node/src/shards/errors.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_node/src/shards/indexes.rs` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_node/src/shards/indexes.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_node/src/shards/metadata.rs` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_node/src/shards/metadata.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_node/src/shards/mod.rs` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_node/src/shards/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_node/src/shards/shard_reader.rs` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_node/src/shards/shard_reader.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_node/src/shards/shard_writer.rs` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_node/src/shards/shard_writer.rs`

 * *Files 1% similar despite different names*

```diff
@@ -180,18 +180,18 @@
             vectors: versioning::VECTORS_VERSION,
             texts: versioning::TEXTS_VERSION,
             relations: versioning::RELATIONS_VERSION,
         };
         let versions_path = metadata.shard_path().join(VERSION_FILE);
         Versions::create(&versions_path, versions)?;
 
-        let text_task = || Some(nucliadb_texts2::writer::TextWriterService::create(&tsc));
-        let paragraph_task = || Some(nucliadb_paragraphs3::writer::ParagraphWriterService::create(&psc));
-        let vector_task = || Some(nucliadb_vectors::service::VectorWriterService::create(&vsc));
-        let relation_task = || Some(nucliadb_relations2::writer::RelationsWriterService::create(&rsc));
+        let text_task = || Some(nucliadb_texts2::writer::TextWriterService::create(tsc));
+        let paragraph_task = || Some(nucliadb_paragraphs3::writer::ParagraphWriterService::create(psc));
+        let vector_task = || Some(nucliadb_vectors::service::VectorWriterService::create(vsc));
+        let relation_task = || Some(nucliadb_relations2::writer::RelationsWriterService::create(rsc));
 
         let span = tracing::Span::current();
         let info = info_span!(parent: &span, "text start");
         let text_task = || run_with_telemetry(info, text_task);
         let info = info_span!(parent: &span, "paragraph start");
         let paragraph_task = || run_with_telemetry(info, paragraph_task);
         let info = info_span!(parent: &span, "vector start");
```

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_node/src/shards/versioning.rs` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_node/src/shards/versioning.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_node/src/telemetry.rs` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_node/src/telemetry.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_node/src/utils.rs` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_node/src/utils.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_node/tests/common/mod.rs` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_node/tests/common/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_node/tests/common/node_services.rs` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_node/tests/common/node_services.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_node/tests/common/resources.rs` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_node/tests/common/resources.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_node/tests/test_date_range_search.rs` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_node/tests/test_date_range_search.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_node/tests/test_download.rs` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_node/tests/test_download.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_node/tests/test_merge.rs` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_node/tests/test_merge.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_node/tests/test_replication.rs` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_node/tests/test_replication.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_node/tests/test_search_relations.rs` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_node/tests/test_search_relations.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_node/tests/test_search_sorting.rs` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_node/tests/test_search_sorting.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_node/tests/test_security_search.rs` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_node/tests/test_security_search.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_node/tests/test_set_resource_from_storage.rs` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_node/tests/test_set_resource_from_storage.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_node/tests/test_shards.rs` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_node/tests/test_shards.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_node/tests/test_suggest.rs` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_node/tests/test_suggest.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_node/tests/test_vector_normalization.rs` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_node/tests/test_vector_normalization.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_texts2/src/lib.rs` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_texts2/src/lib.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_texts2/src/query_io.rs` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_texts2/src/query_io.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_texts2/src/reader.rs` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_texts2/src/reader.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_texts2/src/schema.rs` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_texts2/src/schema.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_texts2/src/search_query.rs` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_texts2/src/search_query.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_texts2/src/writer.rs` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_texts2/src/writer.rs`

 * *Files 1% similar despite different names*

```diff
@@ -166,15 +166,15 @@
             writer,
             schema: field_schema,
             config: config.clone(),
         })
     }
 
     #[tracing::instrument(skip_all)]
-    pub fn create(config: &TextConfig) -> NodeResult<Self> {
+    pub fn create(config: TextConfig) -> NodeResult<Self> {
         Self::try_create_index_dir(&config.path)?;
 
         let settings = IndexSettings {
             sort_by_field: Some(IndexSortByField {
                 field: "created".to_string(),
                 order: Order::Desc,
             }),
@@ -186,15 +186,15 @@
         let index = index_builder.create_in_dir(&config.path).expect("Index directory should exist");
         let writer = index.writer_with_num_threads(1, TANTIVY_INDEX_ARENA_MEMORY).unwrap();
 
         Ok(TextWriterService {
             index,
             writer,
             schema: field_schema,
-            config: config.clone(),
+            config,
         })
     }
 
     fn try_create_index_dir(path: &Path) -> NodeResult<()> {
         let result = fs::create_dir(path);
         if let Err(error) = result {
             if path.exists() {
```

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_texts2/tests/common/mod.rs` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_texts2/tests/common/mod.rs`

 * *Files 2% similar despite different names*

```diff
@@ -30,23 +30,24 @@
 use nucliadb_core::texts::*;
 use nucliadb_texts2::reader::TextReaderService;
 use nucliadb_texts2::writer::TextWriterService;
 use tempfile::TempDir;
 
 pub fn test_reader() -> TextReaderService {
     let dir = TempDir::new().unwrap();
+    let shard_path = dir.path().join("texts");
     let config = TextConfig {
-        path: dir.path().join("texts"),
+        path: shard_path.clone(),
     };
 
-    let mut writer = TextWriterService::create(&config).unwrap();
+    let mut writer = TextWriterService::create(config).unwrap();
     let resource = create_resource("shard".to_string());
     writer.set_resource(&resource).unwrap();
 
-    TextReaderService::open(&config.path).unwrap()
+    TextReaderService::open(&shard_path).unwrap()
 }
 
 pub fn create_resource(shard_id: String) -> Resource {
     let resource_id = ResourceId {
         shard_id: shard_id.to_string(),
         uuid: "f56c58ac-b4f9-4d61-a077-ffccaadd0001".to_string(),
     };
```

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_texts2/tests/test_reader.rs` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_texts2/tests/test_reader.rs`

 * *Files 14% similar despite different names*

```diff
@@ -22,34 +22,36 @@
 use nucliadb_texts2::reader::TextReaderService;
 use nucliadb_texts2::writer::TextWriterService;
 use tempfile::TempDir;
 
 #[test]
 fn test_start_new_reader_after_a_writer() {
     let dir = TempDir::new().unwrap();
+    let shard_path = dir.path().join("texts");
     let config = TextConfig {
-        path: dir.path().join("texts"),
+        path: shard_path.clone(),
     };
 
-    let _writer = TextWriterService::create(&config).unwrap();
-    let reader = TextReaderService::open(&config.path);
+    let _writer = TextWriterService::create(config).unwrap();
+    let reader = TextReaderService::open(&shard_path);
     assert!(reader.is_ok());
 }
 
 #[test]
 fn test_open_multiple_readers() {
     let dir = TempDir::new().unwrap();
+    let shard_path = dir.path().join("texts");
     let config = TextConfig {
-        path: dir.path().join("texts"),
+        path: shard_path.clone(),
     };
 
-    let _writer = TextWriterService::create(&config).unwrap();
-    let reader1 = TextReaderService::open(&config.path);
-    let reader2 = TextReaderService::open(&config.path);
-    let reader3 = TextReaderService::open(&config.path);
+    let _writer = TextWriterService::create(config.clone()).unwrap();
+    let reader1 = TextReaderService::open(&shard_path);
+    let reader2 = TextReaderService::open(&shard_path);
+    let reader3 = TextReaderService::open(&shard_path);
     assert!(reader1.is_ok());
     assert!(reader2.is_ok());
     assert!(reader3.is_ok());
 }
 
 #[test]
 fn test_start_new_reader_before_a_writer() {
```

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_texts2/tests/test_search.rs` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_texts2/tests/test_search.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_texts2/tests/test_streaming.rs` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_texts2/tests/test_streaming.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_texts2/tests/test_writer.rs` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_texts2/tests/test_writer.rs`

 * *Files 10% similar despite different names*

```diff
@@ -32,26 +32,26 @@
 #[test]
 fn test_start_new_writer() {
     let dir = TempDir::new().unwrap();
     let config = TextConfig {
         path: dir.path().join("texts"),
     };
 
-    let writer = TextWriterService::create(&config);
+    let writer = TextWriterService::create(config);
     assert!(writer.is_ok());
 }
 
 #[test]
 fn test_open_writer_for_existent_index() {
     let dir = TempDir::new().unwrap();
     let config = TextConfig {
         path: dir.path().join("texts"),
     };
 
-    let writer = TextWriterService::create(&config).unwrap();
+    let writer = TextWriterService::create(config.clone()).unwrap();
     std::mem::drop(writer);
 
     let another_writer = TextWriterService::open(&config);
 
     assert!(another_writer.is_ok());
 }
 
@@ -59,46 +59,47 @@
 #[should_panic]
 fn test_two_simultaneous_writers() {
     let dir = TempDir::new().unwrap();
     let config = TextConfig {
         path: dir.path().join("texts"),
     };
 
-    let _writer = TextWriterService::create(&config).unwrap();
+    let _writer = TextWriterService::create(config.clone()).unwrap();
     let _another_writer = TextWriterService::open(&config);
 }
 
 #[test]
 fn test_set_resource() {
     let dir = TempDir::new().unwrap();
     let config = TextConfig {
         path: dir.path().join("texts"),
     };
 
-    let mut writer = TextWriterService::create(&config).unwrap();
+    let mut writer = TextWriterService::create(config).unwrap();
     let resource = common::create_resource("shard1".to_string());
     let result = writer.set_resource(&resource);
 
     assert!(result.is_ok());
 }
 
 // TODO: move to another test file and refactor
 #[test]
 fn test_old_writer_test() -> NodeResult<()> {
     let dir = TempDir::new().unwrap();
+    let shard_path = dir.path().join("texts");
     let fsc = TextConfig {
-        path: dir.path().join("texts"),
+        path: shard_path.clone(),
     };
 
-    let mut field_writer_service = TextWriterService::create(&fsc).unwrap();
+    let mut field_writer_service = TextWriterService::create(fsc).unwrap();
     let resource1 = common::create_resource("shard1".to_string());
     let _ = field_writer_service.set_resource(&resource1);
     let _ = field_writer_service.set_resource(&resource1);
 
-    let field_reader_service = TextReaderService::open(&fsc.path).unwrap();
+    let field_reader_service = TextReaderService::open(&shard_path).unwrap();
 
     let reader = field_reader_service;
     let searcher = reader.reader.searcher();
 
     let query =
         TermQuery::new(Term::from_field_text(field_writer_service.schema.text, "document"), IndexRecordOption::Basic);
```

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_vectors/Cargo.toml` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_vectors/Cargo.toml`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_vectors/docs/labels.drawio.svg` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_vectors/docs/labels.drawio.svg`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_vectors/src/data_point/disk_hnsw.rs` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_vectors/src/data_point/disk_hnsw.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_vectors/src/data_point/mod.rs` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_vectors/src/data_point/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_vectors/src/data_point/node.rs` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_vectors/src/data_point/node.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_vectors/src/data_point/ops_hnsw.rs` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_vectors/src/data_point/ops_hnsw.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_vectors/src/data_point/params.rs` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_vectors/src/data_point/params.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_vectors/src/data_point/ram_hnsw.rs` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_vectors/src/data_point/ram_hnsw.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_vectors/src/data_point/tests.rs` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_vectors/src/data_point/tests.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_vectors/src/data_point_provider/garbage_collector.rs` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_vectors/src/data_point_provider/garbage_collector.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_vectors/src/data_point_provider/mod.rs` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_vectors/src/data_point_provider/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_vectors/src/data_point_provider/reader.rs` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_vectors/src/data_point_provider/reader.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_vectors/src/data_point_provider/replication.rs` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_vectors/src/data_point_provider/replication.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_vectors/src/data_point_provider/state.rs` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_vectors/src/data_point_provider/state.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_vectors/src/data_point_provider/writer.rs` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_vectors/src/data_point_provider/writer.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_vectors/src/data_types/data_store.rs` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_vectors/src/data_types/data_store.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_vectors/src/data_types/dtrie_ram.rs` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_vectors/src/data_types/dtrie_ram.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_vectors/src/data_types/mod.rs` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_vectors/src/data_types/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_vectors/src/data_types/trie.rs` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_vectors/src/data_types/trie.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_vectors/src/data_types/trie_ram.rs` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_vectors/src/data_types/trie_ram.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_vectors/src/data_types/vector.rs` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_vectors/src/data_types/vector.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_vectors/src/formula/mod.rs` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_vectors/src/formula/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_vectors/src/lib.rs` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_vectors/src/lib.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_vectors/src/service/mod.rs` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_vectors/src/service/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_vectors/src/service/query_io.rs` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_vectors/src/service/query_io.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_vectors/src/service/reader.rs` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_vectors/src/service/reader.rs`

 * *Files 2% similar despite different names*

```diff
@@ -194,17 +194,18 @@
 
     use super::*;
     use crate::service::writer::VectorWriterService;
 
     #[test]
     fn test_key_prefix_search() {
         let dir = TempDir::new().unwrap();
+        let shard_path = dir.path().join("vectors");
         let vsc = VectorConfig {
             similarity: VectorSimilarity::Cosine,
-            path: dir.path().join("vectors"),
+            path: shard_path.clone(),
             channel: Channel::EXPERIMENTAL,
             shard_id: "abc".into(),
             normalize_vectors: false,
         };
         let raw_sentences = [
             ("DOC/KEY/1/1".to_string(), vec![1.0, 3.0, 4.0]),
             ("DOC/KEY/1/2".to_string(), vec![2.0, 4.0, 5.0]),
@@ -250,18 +251,18 @@
             relations: vec![],
             vectors: HashMap::default(),
             vectors_to_delete: HashMap::default(),
             shard_id: "DOC".to_string(),
             ..Default::default()
         };
         // insert - delete - insert sequence
-        let mut writer = VectorWriterService::create(&vsc).unwrap();
+        let mut writer = VectorWriterService::create(vsc).unwrap();
         writer.set_resource(&resource).unwrap();
 
-        let reader = VectorReaderService::open(&vsc.path).unwrap();
+        let reader = VectorReaderService::open(&shard_path).unwrap();
         let mut request = VectorSearchRequest {
             id: "".to_string(),
             vector_set: "".to_string(),
             vector: vec![4.0, 6.0, 7.0],
             field_labels: vec!["1".to_string()],
             key_filters: vec!["DOC/KEY/1".to_string()],
             page_number: 0,
@@ -277,17 +278,18 @@
         let result = reader.search(&request, &context).unwrap();
         assert_eq!(result.documents.len(), 0);
     }
 
     #[test]
     fn test_new_vector_reader() {
         let dir = TempDir::new().unwrap();
+        let shard_path = dir.path().join("vectors");
         let vsc = VectorConfig {
             similarity: VectorSimilarity::Cosine,
-            path: dir.path().join("vectors"),
+            path: shard_path.clone(),
             channel: Channel::EXPERIMENTAL,
             shard_id: "abc".into(),
             normalize_vectors: false,
         };
         let raw_sentences = [
             ("DOC/KEY/1/1".to_string(), vec![1.0, 3.0, 4.0]),
             ("DOC/KEY/1/2".to_string(), vec![2.0, 4.0, 5.0]),
@@ -333,18 +335,18 @@
             relations: vec![],
             vectors: HashMap::default(),
             vectors_to_delete: HashMap::default(),
             shard_id: "DOC".to_string(),
             ..Default::default()
         };
         // insert - delete - insert sequence
-        let mut writer = VectorWriterService::create(&vsc).unwrap();
+        let mut writer = VectorWriterService::create(vsc).unwrap();
         let res = writer.set_resource(&resource);
         assert!(res.is_ok());
-        let reader = VectorReaderService::open(&vsc.path).unwrap();
+        let reader = VectorReaderService::open(&shard_path).unwrap();
         let request = VectorSearchRequest {
             id: "".to_string(),
             vector_set: "".to_string(),
             vector: vec![4.0, 6.0, 7.0],
             field_labels: vec!["1".to_string()],
             page_number: 0,
             result_per_page: 20,
@@ -399,17 +401,18 @@
         };
         assert!(reader.search(&bad_request, &context).is_err());
     }
 
     #[test]
     fn test_vectors_deduplication() {
         let dir = TempDir::new().unwrap();
+        let shard_path = dir.path().join("vectors");
         let vsc = VectorConfig {
             similarity: VectorSimilarity::Cosine,
-            path: dir.path().join("vectors"),
+            path: shard_path.clone(),
             channel: Channel::EXPERIMENTAL,
             shard_id: "abc".into(),
             normalize_vectors: false,
         };
         let raw_sentences =
             [("DOC/KEY/1/1".to_string(), vec![1.0, 2.0, 3.0]), ("DOC/KEY/1/2".to_string(), vec![1.0, 2.0, 3.0])];
         let resource_id = ResourceId {
@@ -450,18 +453,18 @@
             sentences_to_delete: vec![],
             relations: vec![],
             vectors: HashMap::default(),
             vectors_to_delete: HashMap::default(),
             shard_id: "DOC".to_string(),
             ..Default::default()
         };
-        let mut writer = VectorWriterService::create(&vsc).unwrap();
+        let mut writer = VectorWriterService::create(vsc).unwrap();
         let res = writer.set_resource(&resource);
         assert!(res.is_ok());
-        let reader = VectorReaderService::open(&vsc.path).unwrap();
+        let reader = VectorReaderService::open(&shard_path).unwrap();
         let request = VectorSearchRequest {
             id: "".to_string(),
             vector_set: "".to_string(),
             vector: vec![4.0, 6.0, 7.0],
             field_labels: vec!["1".to_string()],
             page_number: 0,
             result_per_page: 20,
```

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_vectors/src/service/writer.rs` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_vectors/src/service/writer.rs`

 * *Files 0% similar despite different names*

```diff
@@ -213,26 +213,26 @@
             report.push_str(&partial);
         }
         report.pop();
         report
     }
 
     #[tracing::instrument(skip_all)]
-    pub fn create(config: &VectorConfig) -> NodeResult<Self> {
+    pub fn create(config: VectorConfig) -> NodeResult<Self> {
         let path = std::path::Path::new(&config.path);
         if path.exists() {
             Err(node_error!("Shard does exist".to_string()))
         } else {
             let index_metadata = IndexMetadata {
                 similarity: config.similarity.into(),
                 channel: config.channel,
                 normalize_vectors: config.normalize_vectors,
             };
             Ok(VectorWriterService {
-                index: Writer::new(path, index_metadata, config.shard_id.clone())?,
+                index: Writer::new(path, index_metadata, config.shard_id)?,
                 path: path.to_path_buf(),
             })
         }
     }
 
     #[tracing::instrument(skip_all)]
     pub fn open(path: &Path, shard_id: String) -> NodeResult<Self> {
@@ -313,15 +313,15 @@
             relations: vec![],
             vectors: HashMap::default(),
             vectors_to_delete: HashMap::default(),
             shard_id: "DOC".to_string(),
             ..Default::default()
         };
         // insert - delete - insert sequence
-        let mut writer = VectorWriterService::create(&vsc).unwrap();
+        let mut writer = VectorWriterService::create(vsc).unwrap();
         let res = writer.set_resource(&resource);
         assert!(res.is_ok());
         let res = writer.delete_resource(&resource_id);
         assert!(res.is_ok());
         let res = writer.set_resource(&resource);
         assert!(res.is_ok());
     }
@@ -376,15 +376,15 @@
             relations: vec![],
             vectors: HashMap::default(),
             vectors_to_delete: HashMap::default(),
             shard_id: "DOC".to_string(),
             ..Default::default()
         };
         // insert - delete - insert sequence
-        let mut writer = VectorWriterService::create(&vsc).unwrap();
+        let mut writer = VectorWriterService::create(vsc).unwrap();
         let res = writer.set_resource(&resource);
         assert!(res.is_ok());
         let res = writer.delete_resource(&resource_id);
         assert!(res.is_ok());
         let res = writer.set_resource(&resource);
         assert!(res.is_ok());
```

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_vectors/src/utils.rs` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_vectors/src/utils.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_vectors/tests/test_merge.rs` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_vectors/tests/test_merge.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_procs/src/lib.rs` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_procs/src/lib.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_procs/src/measure.rs` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_procs/src/measure.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_procs/tests/dont_compile/actor_defined_twice.rs` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_procs/tests/dont_compile/actor_defined_twice.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_procs/tests/dont_compile/actor_not_defined.rs` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_procs/tests/dont_compile/actor_not_defined.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_procs/tests/dont_compile/metric_defined_twice.rs` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_procs/tests/dont_compile/metric_defined_twice.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_procs/tests/dont_compile/wrong_actor.rs` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_procs/tests/dont_compile/wrong_actor.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_procs/tests/dont_compile/wrong_actor.stderr` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_procs/tests/dont_compile/wrong_actor.stderr`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_procs/tests/test_measure.rs` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_procs/tests/test_measure.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_paragraphs2/Cargo.toml` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_paragraphs2/Cargo.toml`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_paragraphs2/src/fuzzy_query.rs` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_paragraphs2/src/fuzzy_query.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_paragraphs2/src/lib.rs` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_paragraphs2/src/lib.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_paragraphs2/src/query_io.rs` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_paragraphs2/src/query_io.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_paragraphs2/src/reader.rs` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_paragraphs3/src/reader.rs`

 * *Files 2% similar despite different names*

```diff
@@ -33,16 +33,15 @@
 use tantivy::query::{AllQuery, Query, QueryParser};
 use tantivy::schema::*;
 use tantivy::{DocAddress, Index, IndexReader, LeasedItem, ReloadPolicy};
 
 use super::schema::ParagraphSchema;
 use crate::search_query;
 use crate::search_query::SharedTermC;
-use crate::search_response::extract_labels;
-use crate::search_response::{SearchBm25Response, SearchFacetsResponse, SearchIntResponse};
+use crate::search_response::{extract_labels, SearchBm25Response, SearchFacetsResponse, SearchIntResponse};
 
 const FUZZY_DISTANCE: u8 = 1;
 const NUMBER_OF_RESULTS_SUGGEST: usize = 10;
 
 pub struct ParagraphReaderService {
     index: Index,
     pub schema: ParagraphSchema,
@@ -139,14 +138,15 @@
 
         let v = time.elapsed().as_millis();
         debug!("{id:?} - Creating query: starts at {v} ms");
 
         let parser = QueryParser::for_index(&self.index, vec![self.schema.text]);
         let results = request.result_per_page as usize;
         let offset = results * request.page_number as usize;
+
         let facets: Vec<_> = request
             .faceted
             .as_ref()
             .iter()
             .flat_map(|v| v.labels.iter())
             .filter(|s| ParagraphReaderService::is_valid_facet(s))
             .cloned()
@@ -596,27 +596,28 @@
             ..Default::default()
         }
     }
     #[test]
     fn test_total_number_of_results() -> NodeResult<()> {
         const UUID: &str = "f56c58ac-b4f9-4d61-a077-ffccaadd0001";
         let dir = TempDir::new().unwrap();
+        let shard_path = dir.path().join("paragraphs");
         let psc = ParagraphConfig {
-            path: dir.path().join("paragraphs"),
+            path: shard_path.clone(),
         };
         let seconds = SystemTime::now().duration_since(SystemTime::UNIX_EPOCH).map(|t| t.as_secs() as i64).unwrap();
         let timestamp = Timestamp {
             seconds,
             nanos: 0,
         };
 
-        let mut paragraph_writer_service = ParagraphWriterService::create(&psc).unwrap();
+        let mut paragraph_writer_service = ParagraphWriterService::create(psc).unwrap();
         let resource1 = create_resource("shard1".to_string(), timestamp);
-        let _ = paragraph_writer_service.set_resource(&resource1);
-        let paragraph_reader_service = ParagraphReaderService::open(&psc.path).unwrap();
+        paragraph_writer_service.set_resource(&resource1)?;
+        let paragraph_reader_service = ParagraphReaderService::open(&shard_path).unwrap();
         let context = ParagraphsContext::default();
 
         // Search on all paragraphs faceted
         let search = ProtosRequest {
             id: "shard1".to_string(),
             uuid: UUID.to_string(),
             body: "".to_string(),
@@ -657,28 +658,29 @@
         Ok(())
     }
 
     #[test]
     fn test_filtered_search() -> NodeResult<()> {
         const UUID: &str = "f56c58ac-b4f9-4d61-a077-ffccaadd0001";
         let dir = TempDir::new().unwrap();
+        let shard_path = dir.path().join("paragraphs");
         let psc = ParagraphConfig {
-            path: dir.path().join("paragraphs"),
+            path: shard_path.clone(),
         };
         let seconds = SystemTime::now().duration_since(SystemTime::UNIX_EPOCH).map(|t| t.as_secs() as i64).unwrap();
         let timestamp = Timestamp {
             seconds,
             nanos: 0,
         };
 
-        let mut paragraph_writer_service = ParagraphWriterService::create(&psc).unwrap();
+        let mut paragraph_writer_service = ParagraphWriterService::create(psc).unwrap();
         let resource1 = create_resource("shard1".to_string(), timestamp);
-        let _ = paragraph_writer_service.set_resource(&resource1);
+        paragraph_writer_service.set_resource(&resource1)?;
 
-        let paragraph_reader_service = ParagraphReaderService::open(&psc.path).unwrap();
+        let paragraph_reader_service = ParagraphReaderService::open(&shard_path).unwrap();
 
         let reader = paragraph_writer_service.index.reader()?;
         let searcher = reader.searcher();
         let mut context = ParagraphsContext::default();
         let (_top_docs, count) = searcher.search(&AllQuery, &(TopDocs::with_limit(10), Count))?;
         assert_eq!(count, 4);
 
@@ -729,26 +731,27 @@
         Ok(())
     }
 
     #[test]
     fn test_new_paragraph() -> NodeResult<()> {
         const UUID: &str = "f56c58ac-b4f9-4d61-a077-ffccaadd0001";
         let dir = TempDir::new().unwrap();
+        let shard_path = dir.path().join("paragraphs");
         let psc = ParagraphConfig {
-            path: dir.path().join("paragraphs"),
+            path: shard_path.clone(),
         };
         let seconds = SystemTime::now().duration_since(SystemTime::UNIX_EPOCH).map(|t| t.as_secs() as i64).unwrap();
         let timestamp = Timestamp {
             seconds,
             nanos: 0,
         };
-        let mut paragraph_writer_service = ParagraphWriterService::create(&psc).unwrap();
+        let mut paragraph_writer_service = ParagraphWriterService::create(psc).unwrap();
         let resource1 = create_resource("shard1".to_string(), timestamp);
-        let _ = paragraph_writer_service.set_resource(&resource1);
-        let paragraph_reader_service = ParagraphReaderService::open(&psc.path).unwrap();
+        paragraph_writer_service.set_resource(&resource1)?;
+        let paragraph_reader_service = ParagraphReaderService::open(&shard_path).unwrap();
         let reader = paragraph_writer_service.index.reader()?;
         let searcher = reader.searcher();
         let empty_context = ParagraphsContext::default();
         let (_top_docs, count) = searcher.search(&AllQuery, &(TopDocs::with_limit(10), Count))?;
         assert_eq!(count, 4);
 
         let faceted = Faceted {
@@ -983,28 +986,29 @@
         assert_eq!(count, 4);
         Ok(())
     }
 
     #[test]
     fn test_search_paragraph_with_timestamps() -> NodeResult<()> {
         let dir = TempDir::new().unwrap();
+        let shard_path = dir.path().join("paragraphs");
         let psc = ParagraphConfig {
-            path: dir.path().join("paragraphs"),
+            path: shard_path.clone(),
         };
         let time_baseline = Timestamp {
             seconds: 2,
             nanos: 0,
         };
 
-        let mut paragraph_writer_service = ParagraphWriterService::create(&psc).unwrap();
+        let mut paragraph_writer_service = ParagraphWriterService::create(psc).unwrap();
         let resource1 = create_resource("shard1".to_string(), time_baseline.clone());
 
-        let _ = paragraph_writer_service.set_resource(&resource1);
+        paragraph_writer_service.set_resource(&resource1)?;
 
-        let paragraph_reader_service = ParagraphReaderService::open(&psc.path).unwrap();
+        let paragraph_reader_service = ParagraphReaderService::open(&shard_path).unwrap();
 
         let reader = paragraph_writer_service.index.reader()?;
         let searcher = reader.searcher();
         let (_top_docs, count) = searcher.search(&AllQuery, &(TopDocs::with_limit(10), Count))?;
         assert_eq!(count, 4);
 
         fn do_search(paragraph_reader_service: &ParagraphReaderService, timestamps: Timestamps) -> i32 {
```

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_paragraphs2/src/schema.rs` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_paragraphs2/src/schema.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_paragraphs2/src/search_query.rs` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_paragraphs2/src/search_query.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_paragraphs2/src/search_response.rs` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_paragraphs2/src/search_response.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_paragraphs2/src/stop_words.rs` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_paragraphs2/src/stop_words.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_paragraphs2/src/writer.rs` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_paragraphs2/src/writer.rs`

 * *Files 0% similar despite different names*

```diff
@@ -151,15 +151,15 @@
         let safe_state = tantivy_replica::compute_safe_replica_state(params, &self.index)?;
         Ok(IndexFiles::Tantivy(safe_state))
     }
 }
 
 impl ParagraphWriterService {
     #[tracing::instrument(skip_all)]
-    pub fn create(config: &ParagraphConfig) -> NodeResult<ParagraphWriterService> {
+    pub fn create(config: ParagraphConfig) -> NodeResult<ParagraphWriterService> {
         let paragraph_schema = ParagraphSchema::default();
 
         fs::create_dir(&config.path)?;
 
         let mut index_builder = Index::builder().schema(paragraph_schema.schema.clone());
         let settings = IndexSettings {
             sort_by_field: Some(IndexSortByField {
@@ -174,15 +174,15 @@
 
         let writer = index.writer_with_num_threads(1, 6_000_000)?;
 
         Ok(ParagraphWriterService {
             index,
             writer,
             schema: paragraph_schema,
-            config: config.clone(),
+            config,
         })
     }
     #[tracing::instrument(skip_all)]
     pub fn open(config: &ParagraphConfig) -> NodeResult<ParagraphWriterService> {
         let paragraph_schema = ParagraphSchema::default();
 
         let index = Index::open_in_dir(&config.path)?;
@@ -450,15 +450,15 @@
     #[test]
     fn test_new_writer() -> NodeResult<()> {
         let dir = TempDir::new().unwrap();
         let psc = ParagraphConfig {
             path: dir.path().join("paragraphs"),
         };
 
-        let mut paragraph_writer_service = ParagraphWriterService::create(&psc).unwrap();
+        let mut paragraph_writer_service = ParagraphWriterService::create(psc).unwrap();
         let resource1 = create_resource("shard1".to_string());
         let _ = paragraph_writer_service.set_resource(&resource1);
         let _ = paragraph_writer_service.set_resource(&resource1);
 
         let reader = paragraph_writer_service.index.reader()?;
         let searcher = reader.searcher();
```

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_paragraphs2/stop_words/ar.json` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_paragraphs2/stop_words/ar.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_paragraphs2/stop_words/az.json` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_paragraphs2/stop_words/az.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_paragraphs2/stop_words/bn.json` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_paragraphs2/stop_words/bn.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_paragraphs2/stop_words/ca.json` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_paragraphs2/stop_words/ca.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_paragraphs2/stop_words/ch.json` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_paragraphs2/stop_words/ch.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_paragraphs2/stop_words/da.json` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_paragraphs2/stop_words/da.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_paragraphs2/stop_words/de.json` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_paragraphs2/stop_words/de.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_paragraphs2/stop_words/el.json` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_paragraphs2/stop_words/el.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_paragraphs2/stop_words/en.json` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_paragraphs2/stop_words/en.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_paragraphs2/stop_words/es.json` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_paragraphs2/stop_words/es.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_paragraphs2/stop_words/eu.json` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_paragraphs2/stop_words/eu.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_paragraphs2/stop_words/extract.py` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_paragraphs2/stop_words/extract.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_paragraphs2/stop_words/fi.json` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_paragraphs2/stop_words/fi.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_paragraphs2/stop_words/fr.json` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_paragraphs2/stop_words/fr.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_paragraphs2/stop_words/he.json` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_paragraphs2/stop_words/he.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_paragraphs2/stop_words/hu.json` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_paragraphs2/stop_words/hu.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_paragraphs2/stop_words/id.json` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_paragraphs2/stop_words/id.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_paragraphs2/stop_words/it.json` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_paragraphs2/stop_words/it.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_paragraphs2/stop_words/kk.json` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_paragraphs2/stop_words/kk.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_paragraphs2/stop_words/ne.json` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_paragraphs2/stop_words/ne.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_paragraphs2/stop_words/nl.json` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_paragraphs2/stop_words/nl.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_paragraphs2/stop_words/no.json` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_paragraphs2/stop_words/no.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_paragraphs2/stop_words/pt.json` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_paragraphs2/stop_words/pt.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_paragraphs2/stop_words/ro.json` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_paragraphs2/stop_words/ro.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_paragraphs2/stop_words/ru.json` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_paragraphs2/stop_words/ru.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_paragraphs2/stop_words/sl.json` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_paragraphs2/stop_words/sl.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_paragraphs2/stop_words/sv.json` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_paragraphs2/stop_words/sv.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/local_dependencies/nucliadb_paragraphs2/stop_words/tg.json` & `nucliadb_node_binding-3.0.3.post1254/local_dependencies/nucliadb_paragraphs2/stop_words/tg.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/Cargo.toml` & `nucliadb_node_binding-3.0.3.post1254/Cargo.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "nucliadb_node_binding"
-version = "3.0.3-post1252"
+version = "3.0.3-post1254"
 edition = "2021"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 [lib]
 name = "nucliadb_node_binding"
 crate-type = ["cdylib"]
```

### Comparing `nucliadb_node_binding-3.0.3.post1252/CHANGELOG.md` & `nucliadb_node_binding-3.0.3.post1254/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/Makefile` & `nucliadb_node_binding-3.0.3.post1254/Makefile`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/cov.sh` & `nucliadb_node_binding-3.0.3.post1254/cov.sh`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/pyproject.toml` & `nucliadb_node_binding-3.0.3.post1254/pyproject.toml`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/src/collect_garbage.rs` & `nucliadb_node_binding-3.0.3.post1254/src/collect_garbage.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/src/errors.rs` & `nucliadb_node_binding-3.0.3.post1254/src/errors.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/src/lib.rs` & `nucliadb_node_binding-3.0.3.post1254/src/lib.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/src/reader.rs` & `nucliadb_node_binding-3.0.3.post1254/src/reader.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/src/update.rs` & `nucliadb_node_binding-3.0.3.post1254/src/update.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/src/writer.rs` & `nucliadb_node_binding-3.0.3.post1254/src/writer.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/tests/__init__.py` & `nucliadb_node_binding-3.0.3.post1254/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/tests/conftest.py` & `nucliadb_node_binding-3.0.3.post1254/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1252/tests/integration/test_indexing.py` & `nucliadb_node_binding-3.0.3.post1254/tests/integration/test_indexing.py`

 * *Files identical despite different names*

