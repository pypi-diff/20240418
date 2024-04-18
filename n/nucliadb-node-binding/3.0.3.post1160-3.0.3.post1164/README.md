# Comparing `tmp/nucliadb_node_binding-3.0.3.post1160.tar.gz` & `tmp/nucliadb_node_binding-3.0.3.post1164.tar.gz`

## Comparing `nucliadb_node_binding-3.0.3.post1160.tar` & `nucliadb_node_binding-3.0.3.post1164.tar`

### file list

```diff
@@ -1,306 +1,308 @@
--rw-r--r--   0        0        0      501 1970-01-01 00:00:00.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_protos/Cargo.toml
--rw-r--r--   0     1001      127     2155 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_protos/build.rs
--rw-r--r--   0     1001      127    27030 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_protos/src/fdbwriter.rs
--rw-r--r--   0     1001      127        0 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_protos/src/google.protobuf.rs
--rw-r--r--   0     1001      127     9170 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_protos/src/knowledgebox.rs
--rw-r--r--   0     1001      127     1256 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_protos/src/lib.rs
--rw-r--r--   0     1001      127    77192 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_protos/src/nodereader.rs
--rw-r--r--   0     1001      127    10215 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_protos/src/noderesources.rs
--rw-r--r--   0     1001      127    43211 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_protos/src/nodewriter.rs
--rw-r--r--   0     1001      127    18949 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_protos/src/replication.rs
--rw-r--r--   0     1001      127    32797 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_protos/src/resources.rs
--rw-r--r--   0     1001      127     5528 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_protos/src/utils.rs
--rw-r--r--   0        0        0      399 1970-01-01 00:00:00.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_texts2/Cargo.toml
--rw-r--r--   0     1001      127      931 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_texts2/src/lib.rs
--rw-r--r--   0     1001      127     2755 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_texts2/src/query_io.rs
--rw-r--r--   0     1001      127    22604 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_texts2/src/reader.rs
--rw-r--r--   0     1001      127     3105 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_texts2/src/schema.rs
--rw-r--r--   0     1001      127     8682 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_texts2/src/search_query.rs
--rw-r--r--   0     1001      127    10377 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_texts2/src/writer.rs
--rw-r--r--   0     1001      127     3391 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_texts2/tests/common/mod.rs
--rw-r--r--   0     1001      127     2046 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_texts2/tests/test_reader.rs
--rw-r--r--   0     1001      127     8881 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_texts2/tests/test_search.rs
--rw-r--r--   0     1001      127     1249 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_texts2/tests/test_streaming.rs
--rw-r--r--   0     1001      127     3460 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_texts2/tests/test_writer.rs
--rw-r--r--   0        0        0      398 1970-01-01 00:00:00.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_texts/Cargo.toml
--rw-r--r--   0     1001      127      931 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_texts/src/lib.rs
--rw-r--r--   0     1001      127     2755 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_texts/src/query_io.rs
--rw-r--r--   0     1001      127    21119 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_texts/src/reader.rs
--rw-r--r--   0     1001      127     2761 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_texts/src/schema.rs
--rw-r--r--   0     1001      127     8676 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_texts/src/search_query.rs
--rw-r--r--   0     1001      127     9257 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_texts/src/writer.rs
--rw-r--r--   0     1001      127     3389 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_texts/tests/common/mod.rs
--rw-r--r--   0     1001      127     2044 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_texts/tests/test_reader.rs
--rw-r--r--   0     1001      127     8063 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_texts/tests/test_search.rs
--rw-r--r--   0     1001      127     1249 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_texts/tests/test_streaming.rs
--rw-r--r--   0     1001      127     3458 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_texts/tests/test_writer.rs
--rw-r--r--   0        0        0      628 1970-01-01 00:00:00.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_paragraphs/Cargo.toml
--rw-r--r--   0     1001      127     7796 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_paragraphs/src/fuzzy_query.rs
--rw-r--r--   0     1001      127     1009 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_paragraphs/src/lib.rs
--rw-r--r--   0     1001      127     2780 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_paragraphs/src/query_io.rs
--rw-r--r--   0     1001      127    43068 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_paragraphs/src/reader.rs
--rw-r--r--   0     1001      127     4221 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_paragraphs/src/schema.rs
--rw-r--r--   0     1001      127    21255 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_paragraphs/src/search_query.rs
--rw-r--r--   0     1001      127    11380 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_paragraphs/src/search_response.rs
--rw-r--r--   0     1001      127     4090 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_paragraphs/src/stop_words.rs
--rw-r--r--   0     1001      127    17196 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_paragraphs/src/writer.rs
--rw-r--r--   0     1001      127       88 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_paragraphs/stop_words/README.md
--rw-r--r--   0     1001      127    19791 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_paragraphs/stop_words/ar.json
--rw-r--r--   0     1001      127     1923 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_paragraphs/stop_words/az.json
--rw-r--r--   0     1001      127    11684 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_paragraphs/stop_words/bn.json
--rw-r--r--   0     1001      127     2513 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_paragraphs/stop_words/ca.json
--rw-r--r--   0     1001      127    12802 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_paragraphs/stop_words/ch.json
--rw-r--r--   0     1001      127      730 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_paragraphs/stop_words/da.json
--rw-r--r--   0     1001      127     2090 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_paragraphs/stop_words/de.json
--rw-r--r--   0     1001      127     6284 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_paragraphs/stop_words/el.json
--rw-r--r--   0     1001      127     1473 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_paragraphs/stop_words/en.json
--rw-r--r--   0     1001      127     3451 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_paragraphs/stop_words/es.json
--rw-r--r--   0     1001      127     3182 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_paragraphs/stop_words/eu.json
--rw-r--r--   0     1001      127     2126 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_paragraphs/stop_words/extract.py
--rw-r--r--   0     1001      127     2748 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_paragraphs/stop_words/fi.json
--rw-r--r--   0     1001      127     1388 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_paragraphs/stop_words/fr.json
--rw-r--r--   0     1001      127     5716 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_paragraphs/stop_words/he.json
--rw-r--r--   0     1001      127     2108 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_paragraphs/stop_words/hu.json
--rw-r--r--   0     1001      127     8721 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_paragraphs/stop_words/id.json
--rw-r--r--   0     1001      127     2535 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_paragraphs/stop_words/it.json
--rw-r--r--   0     1001      127    11737 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_paragraphs/stop_words/kk.json
--rw-r--r--   0     1001      127     7730 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_paragraphs/stop_words/ne.json
--rw-r--r--   0     1001      127      756 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_paragraphs/stop_words/nl.json
--rw-r--r--   0     1001      127     1447 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_paragraphs/stop_words/no.json
--rw-r--r--   0     1001      127     2055 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_paragraphs/stop_words/pt.json
--rw-r--r--   0     1001      127     3327 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_paragraphs/stop_words/ro.json
--rw-r--r--   0     1001      127     3856 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_paragraphs/stop_words/ru.json
--rw-r--r--   0     1001      127    23032 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_paragraphs/stop_words/sl.json
--rw-r--r--   0     1001      127      993 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_paragraphs/stop_words/sv.json
--rw-r--r--   0     1001      127     5424 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_paragraphs/stop_words/tg.json
--rw-r--r--   0     1001      127      491 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_paragraphs/stop_words/tr.json
--rw-r--r--   0        0        0      708 1970-01-01 00:00:00.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_relations2/Cargo.toml
--rw-r--r--   0     1001      127     3593 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_relations2/src/io_maps.rs
--rw-r--r--   0     1001      127      916 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_relations2/src/lib.rs
--rw-r--r--   0     1001      127    17053 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_relations2/src/reader.rs
--rw-r--r--   0     1001      127     7123 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_relations2/src/schema.rs
--rw-r--r--   0     1001      127     8279 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_relations2/src/writer.rs
--rw-r--r--   0     1001      127     1802 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_relations2/tests/common/mod.rs
--rw-r--r--   0     1001      127     9435 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_relations2/tests/test_reader.rs
--rw-r--r--   0     1001      127     3296 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_relations2/tests/test_writer.rs
--rw-r--r--   0        0        0      629 1970-01-01 00:00:00.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_paragraphs2/Cargo.toml
--rw-r--r--   0     1001      127     7796 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_paragraphs2/src/fuzzy_query.rs
--rw-r--r--   0     1001      127     1009 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_paragraphs2/src/lib.rs
--rw-r--r--   0     1001      127     2780 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_paragraphs2/src/query_io.rs
--rw-r--r--   0     1001      127    42935 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_paragraphs2/src/reader.rs
--rw-r--r--   0     1001      127     4808 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_paragraphs2/src/schema.rs
--rw-r--r--   0     1001      127    22494 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_paragraphs2/src/search_query.rs
--rw-r--r--   0     1001      127    11392 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_paragraphs2/src/search_response.rs
--rw-r--r--   0     1001      127     4090 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_paragraphs2/src/stop_words.rs
--rw-r--r--   0     1001      127    18507 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_paragraphs2/src/writer.rs
--rw-r--r--   0     1001      127       88 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_paragraphs2/stop_words/README.md
--rw-r--r--   0     1001      127    19791 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_paragraphs2/stop_words/ar.json
--rw-r--r--   0     1001      127     1923 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_paragraphs2/stop_words/az.json
--rw-r--r--   0     1001      127    11684 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_paragraphs2/stop_words/bn.json
--rw-r--r--   0     1001      127     2513 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_paragraphs2/stop_words/ca.json
--rw-r--r--   0     1001      127    12802 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_paragraphs2/stop_words/ch.json
--rw-r--r--   0     1001      127      730 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_paragraphs2/stop_words/da.json
--rw-r--r--   0     1001      127     2090 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_paragraphs2/stop_words/de.json
--rw-r--r--   0     1001      127     6284 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_paragraphs2/stop_words/el.json
--rw-r--r--   0     1001      127     1473 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_paragraphs2/stop_words/en.json
--rw-r--r--   0     1001      127     3451 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_paragraphs2/stop_words/es.json
--rw-r--r--   0     1001      127     3182 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_paragraphs2/stop_words/eu.json
--rw-r--r--   0     1001      127     2126 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_paragraphs2/stop_words/extract.py
--rw-r--r--   0     1001      127     2748 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_paragraphs2/stop_words/fi.json
--rw-r--r--   0     1001      127     1388 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_paragraphs2/stop_words/fr.json
--rw-r--r--   0     1001      127     5716 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_paragraphs2/stop_words/he.json
--rw-r--r--   0     1001      127     2108 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_paragraphs2/stop_words/hu.json
--rw-r--r--   0     1001      127     8721 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_paragraphs2/stop_words/id.json
--rw-r--r--   0     1001      127     2535 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_paragraphs2/stop_words/it.json
--rw-r--r--   0     1001      127    11737 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_paragraphs2/stop_words/kk.json
--rw-r--r--   0     1001      127     7730 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_paragraphs2/stop_words/ne.json
--rw-r--r--   0     1001      127      756 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_paragraphs2/stop_words/nl.json
--rw-r--r--   0     1001      127     1447 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_paragraphs2/stop_words/no.json
--rw-r--r--   0     1001      127     2055 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_paragraphs2/stop_words/pt.json
--rw-r--r--   0     1001      127     3327 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_paragraphs2/stop_words/ro.json
--rw-r--r--   0     1001      127     3856 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_paragraphs2/stop_words/ru.json
--rw-r--r--   0     1001      127    23032 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_paragraphs2/stop_words/sl.json
--rw-r--r--   0     1001      127      993 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_paragraphs2/stop_words/sv.json
--rw-r--r--   0     1001      127     5424 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_paragraphs2/stop_words/tg.json
--rw-r--r--   0     1001      127      491 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_paragraphs2/stop_words/tr.json
--rw-r--r--   0        0        0     3314 1970-01-01 00:00:00.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_node/Cargo.toml
--rw-r--r--   0     1001      127     1045 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_node/.rustc_info.json
--rw-r--r--   0     1001      127      877 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_node/Makefile
--rw-r--r--   0     1001      127     1500 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_node/README.md
--rw-r--r--   0     1001      127     1757 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_node/nucliadb_node/__init__.py
--rw-r--r--   0     1001      127     3957 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_node/nucliadb_node/app.py
--rw-r--r--   0     1001      127    17752 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_node/nucliadb_node/indexer.py
--rw-r--r--   0     1001      127      890 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_node/nucliadb_node/listeners/__init__.py
--rw-r--r--   0     1001      127     2424 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_node/nucliadb_node/listeners/indexed_publisher.py
--rw-r--r--   0     1001      127     4015 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_node/nucliadb_node/pull.py
--rw-r--r--   0     1001      127     1535 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_node/nucliadb_node/service.py
--rw-r--r--   0     1001      127     1487 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_node/nucliadb_node/settings.py
--rw-r--r--   0     1001      127     1133 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_node/nucliadb_node/signals.py
--rw-r--r--   0     1001      127      835 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_node/nucliadb_node/tests/__init__.py
--rw-r--r--   0     1001      127     1092 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_node/nucliadb_node/tests/conftest.py
--rw-r--r--   0     1001      127    10810 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_node/nucliadb_node/tests/fixtures.py
--rw-r--r--   0     1001      127    13788 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_node/nucliadb_node/tests/integration/test_indexing.py
--rw-r--r--   0     1001      127     2289 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_node/nucliadb_node/tests/unit/test_app.py
--rw-r--r--   0     1001      127     2361 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_node/nucliadb_node/tests/unit/test_indexed_publisher.py
--rw-r--r--   0     1001      127    12553 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_node/nucliadb_node/tests/unit/test_indexer.py
--rw-r--r--   0     1001      127     3379 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_node/nucliadb_node/tests/unit/test_pull.py
--rw-r--r--   0     1001      127     2323 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_node/nucliadb_node/writer.py
--rw-r--r--   0     1001      127      101 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_node/requirements-sources.txt
--rw-r--r--   0     1001      127      276 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_node/requirements.txt
--rw-r--r--   0     1001      127      249 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_node/setup.cfg
--rw-r--r--   0     1001      127     1405 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_node/setup.py
--rw-r--r--   0     1001      127     2518 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_node/src/analytics/blocking.rs
--rw-r--r--   0     1001      127     1219 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_node/src/analytics/mod.rs
--rw-r--r--   0     1001      127     4931 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_node/src/analytics/payload.rs
--rw-r--r--   0     1001      127    12828 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_node/src/analytics/sender.rs
--rw-r--r--   0     1001      127     3085 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_node/src/analytics/sink.rs
--rw-r--r--   0     1001      127     1900 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_node/src/analytics/sync.rs
--rw-r--r--   0     1001      127     5045 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_node/src/bin/reader.rs
--rw-r--r--   0     1001      127     8050 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_node/src/bin/writer.rs
--rw-r--r--   0     1001      127     1345 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_node/src/cache/mod.rs
--rw-r--r--   0     1001      127     3043 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_node/src/cache/reader_cache.rs
--rw-r--r--   0     1001      127    14199 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_node/src/cache/resource_cache.rs
--rw-r--r--   0     1001      127    10999 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_node/src/cache/writer_cache.rs
--rw-r--r--   0     1001      127     1771 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_node/src/disk_structure.rs
--rw-r--r--   0     1001      127     2656 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_node/src/grpc/collect_garbage.rs
--rw-r--r--   0     1001      127    18821 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_node/src/grpc/grpc_reader.rs
--rw-r--r--   0     1001      127    13691 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_node/src/grpc/grpc_writer.rs
--rw-r--r--   0     1001      127     3186 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_node/src/grpc/middleware/debug.rs
--rw-r--r--   0     1001      127     3440 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_node/src/grpc/middleware/metrics.rs
--rw-r--r--   0     1001      127     1009 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_node/src/grpc/middleware/mod.rs
--rw-r--r--   0     1001      127     4158 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_node/src/grpc/middleware/telemetry.rs
--rw-r--r--   0     1001      127     1283 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_node/src/grpc/mod.rs
--rw-r--r--   0     1001      127     2581 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_node/src/grpc/update.rs
--rw-r--r--   0     1001      127     1173 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_node/src/http_server/metrics_service.rs
--rw-r--r--   0     1001      127     1465 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_node/src/http_server/mod.rs
--rw-r--r--   0     1001      127     1943 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_node/src/http_server/traces_service.rs
--rw-r--r--   0     1001      127     1488 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_node/src/lib.rs
--rw-r--r--   0     1001      127     2757 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_node/src/lifecycle.rs
--rw-r--r--   0     1001      127     1778 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_node/src/merge/global.rs
--rw-r--r--   0     1001      127     1089 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_node/src/merge/mod.rs
--rw-r--r--   0     1001      127    13672 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_node/src/merge/scheduler.rs
--rw-r--r--   0     1001      127     3677 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_node/src/merge/work.rs
--rw-r--r--   0     1001      127     1935 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_node/src/node_metadata.rs
--rw-r--r--   0     1001      127     2417 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_node/src/replication/health.rs
--rw-r--r--   0     1001      127     1070 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_node/src/replication/mod.rs
--rw-r--r--   0     1001      127    14052 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_node/src/replication/replicator.rs
--rw-r--r--   0     1001      127    11682 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_node/src/replication/service.rs
--rw-r--r--   0     1001      127    11615 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_node/src/settings.rs
--rw-r--r--   0     1001      127     1111 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_node/src/shards/errors.rs
--rw-r--r--   0     1001      127    10834 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_node/src/shards/metadata.rs
--rw-r--r--   0     1001      127     1122 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_node/src/shards/mod.rs
--rw-r--r--   0     1001      127    24292 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_node/src/shards/shard_reader.rs
--rw-r--r--   0     1001      127    19507 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_node/src/shards/shard_writer.rs
--rw-r--r--   0     1001      127    10251 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_node/src/shards/versions.rs
--rw-r--r--   0     1001      127    10170 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_node/src/telemetry.rs
--rw-r--r--   0     1001      127     6396 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_node/src/utils.rs
--rw-r--r--   0     1001      127       42 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_node/test.sh
--rw-r--r--   0     1001      127     1115 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_node/tests/common/mod.rs
--rw-r--r--   0     1001      127    12731 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_node/tests/common/node_services.rs
--rw-r--r--   0     1001      127     7823 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_node/tests/common/resources.rs
--rw-r--r--   0     1001      127     8173 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_node/tests/test_date_range_search.rs
--rw-r--r--   0     1001      127     4089 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_node/tests/test_download.rs
--rw-r--r--   0     1001      127     1684 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_node/tests/test_merge.rs
--rw-r--r--   0     1001      127     6003 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_node/tests/test_replication.rs
--rw-r--r--   0     1001      127    22494 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_node/tests/test_search_relations.rs
--rw-r--r--   0     1001      127     6958 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_node/tests/test_search_sorting.rs
--rw-r--r--   0     1001      127     7044 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_node/tests/test_security_search.rs
--rw-r--r--   0     1001      127     6862 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_node/tests/test_shards.rs
--rw-r--r--   0     1001      127    10698 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_node/tests/test_suggest.rs
--rw-r--r--   0        0        0      838 1970-01-01 00:00:00.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_relations/Cargo.toml
--rw-r--r--   0     1001      127     9354 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_relations/src/bfs_engine.rs
--rw-r--r--   0     1001      127     1761 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_relations/src/errors.rs
--rw-r--r--   0     1001      127    21119 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_relations/src/graph_db.rs
--rw-r--r--   0     1001      127     1784 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_relations/src/graph_test_utils.rs
--rw-r--r--   0     1001      127    10531 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_relations/src/index.rs
--rw-r--r--   0     1001      127     1003 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_relations/src/lib.rs
--rw-r--r--   0     1001      127     5550 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_relations/src/node_dictionary.rs
--rw-r--r--   0     1001      127     5249 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_relations/src/relations_io.rs
--rw-r--r--   0     1001      127     2658 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_relations/src/service/bfs.rs
--rw-r--r--   0     1001      127      970 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_relations/src/service/mod.rs
--rw-r--r--   0     1001      127     9828 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_relations/src/service/reader.rs
--rw-r--r--   0     1001      127    10781 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_relations/src/service/tests.rs
--rw-r--r--   0     1001      127     3071 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_relations/src/service/utils.rs
--rw-r--r--   0     1001      127     7110 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_relations/src/service/writer.rs
--rw-r--r--   0        0        0      931 1970-01-01 00:00:00.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_core/Cargo.toml
--rw-r--r--   0     1001      127     5872 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_core/src/fs_state.rs
--rw-r--r--   0     1001      127     2681 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_core/src/lib.rs
--rw-r--r--   0     1001      127     2295 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_core/src/merge.rs
--rw-r--r--   0     1001      127      906 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_core/src/metrics/meters/mod.rs
--rw-r--r--   0     1001      127     4869 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_core/src/metrics/meters/prometheus.rs
--rw-r--r--   0     1001      127     1702 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_core/src/metrics/metric/grpc_ops.rs
--rw-r--r--   0     1001      127     1442 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_core/src/metrics/metric/mod.rs
--rw-r--r--   0     1001      127     1950 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_core/src/metrics/metric/replication.rs
--rw-r--r--   0     1001      127     2626 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_core/src/metrics/metric/request_time.rs
--rw-r--r--   0     1001      127     1644 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_core/src/metrics/metric/shard_cache.rs
--rw-r--r--   0     1001      127    21641 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_core/src/metrics/metric/tokio_runtime.rs
--rw-r--r--   0     1001      127    16736 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_core/src/metrics/metric/tokio_tasks.rs
--rw-r--r--   0     1001      127     3415 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_core/src/metrics/metric/vectors.rs
--rw-r--r--   0     1001      127     1324 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_core/src/metrics/mod.rs
--rw-r--r--   0     1001      127     3074 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_core/src/metrics/task_monitor.rs
--rw-r--r--   0     1001      127     3920 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_core/src/metrics/tests.rs
--rw-r--r--   0     1001      127     2990 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_core/src/paragraphs.rs
--rw-r--r--   0     1001      127    17305 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_core/src/query_language/mod.rs
--rw-r--r--   0     1001      127    15365 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_core/src/query_planner.rs
--rw-r--r--   0     1001      127     2069 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_core/src/relations.rs
--rw-r--r--   0     1001      127     8399 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_core/src/tantivy_replica.rs
--rw-r--r--   0     1001      127     2603 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_core/src/texts.rs
--rw-r--r--   0     1001      127     3526 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_core/src/vectors.rs
--rw-r--r--   0        0        0      742 1970-01-01 00:00:00.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_vectors/Cargo.toml
--rw-r--r--   0     1001      127       69 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_vectors/README.md
--rw-r--r--   0     1001      127       43 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_vectors/docs/README.md
--rw-r--r--   0     1001      127    25718 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_vectors/docs/labels.drawio.svg
--rw-r--r--   0     1001      127    12340 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_vectors/src/data_point/disk_hnsw.rs
--rw-r--r--   0     1001      127    24470 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_vectors/src/data_point/mod.rs
--rw-r--r--   0     1001      127    11214 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_vectors/src/data_point/node.rs
--rw-r--r--   0     1001      127    14639 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_vectors/src/data_point/ops_hnsw.rs
--rw-r--r--   0     1001      127     1642 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_vectors/src/data_point/params.rs
--rw-r--r--   0     1001      127     3952 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_vectors/src/data_point/ram_hnsw.rs
--rw-r--r--   0     1001      127    14176 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_vectors/src/data_point/tests.rs
--rw-r--r--   0     1001      127     5798 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_vectors/src/data_point_provider/garbage_collector.rs
--rw-r--r--   0     1001      127     2722 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_vectors/src/data_point_provider/mod.rs
--rw-r--r--   0     1001      127    10394 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_vectors/src/data_point_provider/reader.rs
--rw-r--r--   0     1001      127     2304 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_vectors/src/data_point_provider/replication.rs
--rw-r--r--   0     1001      127     5288 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_vectors/src/data_point_provider/state.rs
--rw-r--r--   0     1001      127    20587 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_vectors/src/data_point_provider/writer.rs
--rw-r--r--   0     1001      127    23710 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_vectors/src/data_types/data_store.rs
--rw-r--r--   0     1001      127     6916 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_vectors/src/data_types/dtrie_ram.rs
--rw-r--r--   0     1001      127     1959 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_vectors/src/data_types/mod.rs
--rw-r--r--   0     1001      127     6143 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_vectors/src/data_types/trie.rs
--rw-r--r--   0     1001      127     2904 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_vectors/src/data_types/trie_ram.rs
--rw-r--r--   0     1001      127     4433 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_vectors/src/data_types/vector.rs
--rw-r--r--   0     1001      127     8116 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_vectors/src/formula/mod.rs
--rw-r--r--   0     1001      127     2154 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_vectors/src/lib.rs
--rw-r--r--   0     1001      127     1278 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_vectors/src/service/mod.rs
--rw-r--r--   0     1001      127     1897 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_vectors/src/service/query_io.rs
--rw-r--r--   0     1001      127    17122 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_vectors/src/service/reader.rs
--rw-r--r--   0     1001      127    15456 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_vectors/src/service/writer.rs
--rw-r--r--   0     1001      127     2884 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_vectors/tests/test_merge.rs
--rw-r--r--   0        0        0      361 1970-01-01 00:00:00.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_procs/Cargo.toml
--rw-r--r--   0     1001      127     3409 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_procs/src/lib.rs
--rw-r--r--   0     1001      127     2885 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_procs/src/measure.rs
--rw-r--r--   0     1001      127     1081 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_procs/tests/dont_compile/actor_defined_twice.rs
--rw-r--r--   0     1001      127      222 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_procs/tests/dont_compile/actor_defined_twice.stderr
--rw-r--r--   0     1001      127     1038 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_procs/tests/dont_compile/actor_not_defined.rs
--rw-r--r--   0     1001      127      327 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_procs/tests/dont_compile/actor_not_defined.stderr
--rw-r--r--   0     1001      127     1086 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_procs/tests/dont_compile/metric_defined_twice.rs
--rw-r--r--   0     1001      127      249 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_procs/tests/dont_compile/metric_defined_twice.stderr
--rw-r--r--   0     1001      127     1046 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_procs/tests/dont_compile/wrong_actor.rs
--rw-r--r--   0     1001      127     1303 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_procs/tests/dont_compile/wrong_actor.stderr
--rw-r--r--   0     1001      127     1408 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_procs/tests/test_measure.rs
--rw-r--r--   0        0        0      943 1970-01-01 00:00:00.000000 nucliadb_node_binding-3.0.3.post1160/Cargo.toml
--rw-r--r--   0     1001      127     1553 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/CHANGELOG.md
--rw-r--r--   0     1001      127      895 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/Makefile
--rw-r--r--   0     1001      127       52 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/README.md
--rwxr-xr-x   0     1001      127      978 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/cov.sh
--rw-r--r--   0     1001      127     1309 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/pyproject.toml
--rw-r--r--   0     1001      127     2195 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/src/collect_garbage.rs
--rw-r--r--   0     1001      127     1212 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/src/errors.rs
--rw-r--r--   0     1001      127     2337 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/src/lib.rs
--rw-r--r--   0     1001      127     9405 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/src/reader.rs
--rw-r--r--   0     1001      127     2154 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/src/update.rs
--rw-r--r--   0     1001      127     9123 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/src/writer.rs
--rw-r--r--   0     1001      127      835 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/tests/__init__.py
--rw-r--r--   0     1001      127      892 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/tests/conftest.py
--rw-r--r--   0     1001      127     3903 2024-04-17 14:31:59.000000 nucliadb_node_binding-3.0.3.post1160/tests/integration/test_indexing.py
--rw-r--r--   0        0        0      401 1970-01-01 00:00:00.000000 nucliadb_node_binding-3.0.3.post1160/PKG-INFO
+-rw-r--r--   0        0        0      501 1970-01-01 00:00:00.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_protos/Cargo.toml
+-rw-r--r--   0     1001      127     2155 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_protos/build.rs
+-rw-r--r--   0     1001      127    27030 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_protos/src/fdbwriter.rs
+-rw-r--r--   0     1001      127        0 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_protos/src/google.protobuf.rs
+-rw-r--r--   0     1001      127     9795 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_protos/src/knowledgebox.rs
+-rw-r--r--   0     1001      127     1256 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_protos/src/lib.rs
+-rw-r--r--   0     1001      127    77192 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_protos/src/nodereader.rs
+-rw-r--r--   0     1001      127    10215 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_protos/src/noderesources.rs
+-rw-r--r--   0     1001      127    43352 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_protos/src/nodewriter.rs
+-rw-r--r--   0     1001      127    19010 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_protos/src/replication.rs
+-rw-r--r--   0     1001      127    32797 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_protos/src/resources.rs
+-rw-r--r--   0     1001      127     5528 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_protos/src/utils.rs
+-rw-r--r--   0        0        0      708 1970-01-01 00:00:00.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_relations2/Cargo.toml
+-rw-r--r--   0     1001      127     3593 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_relations2/src/io_maps.rs
+-rw-r--r--   0     1001      127      916 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_relations2/src/lib.rs
+-rw-r--r--   0     1001      127    17053 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_relations2/src/reader.rs
+-rw-r--r--   0     1001      127     7123 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_relations2/src/schema.rs
+-rw-r--r--   0     1001      127     8279 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_relations2/src/writer.rs
+-rw-r--r--   0     1001      127     1802 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_relations2/tests/common/mod.rs
+-rw-r--r--   0     1001      127     9435 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_relations2/tests/test_reader.rs
+-rw-r--r--   0     1001      127     3296 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_relations2/tests/test_writer.rs
+-rw-r--r--   0        0        0      629 1970-01-01 00:00:00.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_paragraphs2/Cargo.toml
+-rw-r--r--   0     1001      127     7796 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_paragraphs2/src/fuzzy_query.rs
+-rw-r--r--   0     1001      127     1009 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_paragraphs2/src/lib.rs
+-rw-r--r--   0     1001      127     2780 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_paragraphs2/src/query_io.rs
+-rw-r--r--   0     1001      127    42935 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_paragraphs2/src/reader.rs
+-rw-r--r--   0     1001      127     4808 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_paragraphs2/src/schema.rs
+-rw-r--r--   0     1001      127    22494 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_paragraphs2/src/search_query.rs
+-rw-r--r--   0     1001      127    11392 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_paragraphs2/src/search_response.rs
+-rw-r--r--   0     1001      127     4090 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_paragraphs2/src/stop_words.rs
+-rw-r--r--   0     1001      127    18507 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_paragraphs2/src/writer.rs
+-rw-r--r--   0     1001      127       88 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_paragraphs2/stop_words/README.md
+-rw-r--r--   0     1001      127    19791 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_paragraphs2/stop_words/ar.json
+-rw-r--r--   0     1001      127     1923 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_paragraphs2/stop_words/az.json
+-rw-r--r--   0     1001      127    11684 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_paragraphs2/stop_words/bn.json
+-rw-r--r--   0     1001      127     2513 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_paragraphs2/stop_words/ca.json
+-rw-r--r--   0     1001      127    12802 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_paragraphs2/stop_words/ch.json
+-rw-r--r--   0     1001      127      730 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_paragraphs2/stop_words/da.json
+-rw-r--r--   0     1001      127     2090 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_paragraphs2/stop_words/de.json
+-rw-r--r--   0     1001      127     6284 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_paragraphs2/stop_words/el.json
+-rw-r--r--   0     1001      127     1473 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_paragraphs2/stop_words/en.json
+-rw-r--r--   0     1001      127     3451 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_paragraphs2/stop_words/es.json
+-rw-r--r--   0     1001      127     3182 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_paragraphs2/stop_words/eu.json
+-rw-r--r--   0     1001      127     2126 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_paragraphs2/stop_words/extract.py
+-rw-r--r--   0     1001      127     2748 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_paragraphs2/stop_words/fi.json
+-rw-r--r--   0     1001      127     1388 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_paragraphs2/stop_words/fr.json
+-rw-r--r--   0     1001      127     5716 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_paragraphs2/stop_words/he.json
+-rw-r--r--   0     1001      127     2108 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_paragraphs2/stop_words/hu.json
+-rw-r--r--   0     1001      127     8721 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_paragraphs2/stop_words/id.json
+-rw-r--r--   0     1001      127     2535 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_paragraphs2/stop_words/it.json
+-rw-r--r--   0     1001      127    11737 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_paragraphs2/stop_words/kk.json
+-rw-r--r--   0     1001      127     7730 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_paragraphs2/stop_words/ne.json
+-rw-r--r--   0     1001      127      756 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_paragraphs2/stop_words/nl.json
+-rw-r--r--   0     1001      127     1447 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_paragraphs2/stop_words/no.json
+-rw-r--r--   0     1001      127     2055 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_paragraphs2/stop_words/pt.json
+-rw-r--r--   0     1001      127     3327 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_paragraphs2/stop_words/ro.json
+-rw-r--r--   0     1001      127     3856 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_paragraphs2/stop_words/ru.json
+-rw-r--r--   0     1001      127    23032 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_paragraphs2/stop_words/sl.json
+-rw-r--r--   0     1001      127      993 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_paragraphs2/stop_words/sv.json
+-rw-r--r--   0     1001      127     5424 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_paragraphs2/stop_words/tg.json
+-rw-r--r--   0     1001      127      491 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_paragraphs2/stop_words/tr.json
+-rw-r--r--   0        0        0     3314 1970-01-01 00:00:00.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_node/Cargo.toml
+-rw-r--r--   0     1001      127     1045 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_node/.rustc_info.json
+-rw-r--r--   0     1001      127      877 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_node/Makefile
+-rw-r--r--   0     1001      127     1500 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_node/README.md
+-rw-r--r--   0     1001      127     1757 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_node/nucliadb_node/__init__.py
+-rw-r--r--   0     1001      127     3957 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_node/nucliadb_node/app.py
+-rw-r--r--   0     1001      127    17752 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_node/nucliadb_node/indexer.py
+-rw-r--r--   0     1001      127      890 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_node/nucliadb_node/listeners/__init__.py
+-rw-r--r--   0     1001      127     2424 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_node/nucliadb_node/listeners/indexed_publisher.py
+-rw-r--r--   0     1001      127     4015 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_node/nucliadb_node/pull.py
+-rw-r--r--   0     1001      127     1535 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_node/nucliadb_node/service.py
+-rw-r--r--   0     1001      127     1487 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_node/nucliadb_node/settings.py
+-rw-r--r--   0     1001      127     1133 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_node/nucliadb_node/signals.py
+-rw-r--r--   0     1001      127      835 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_node/nucliadb_node/tests/__init__.py
+-rw-r--r--   0     1001      127     1092 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_node/nucliadb_node/tests/conftest.py
+-rw-r--r--   0     1001      127    10810 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_node/nucliadb_node/tests/fixtures.py
+-rw-r--r--   0     1001      127    13788 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_node/nucliadb_node/tests/integration/test_indexing.py
+-rw-r--r--   0     1001      127     2289 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_node/nucliadb_node/tests/unit/test_app.py
+-rw-r--r--   0     1001      127     2361 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_node/nucliadb_node/tests/unit/test_indexed_publisher.py
+-rw-r--r--   0     1001      127    12553 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_node/nucliadb_node/tests/unit/test_indexer.py
+-rw-r--r--   0     1001      127     3379 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_node/nucliadb_node/tests/unit/test_pull.py
+-rw-r--r--   0     1001      127     2323 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_node/nucliadb_node/writer.py
+-rw-r--r--   0     1001      127      101 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_node/requirements-sources.txt
+-rw-r--r--   0     1001      127      276 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_node/requirements.txt
+-rw-r--r--   0     1001      127      249 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_node/setup.cfg
+-rw-r--r--   0     1001      127     1405 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_node/setup.py
+-rw-r--r--   0     1001      127     2518 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_node/src/analytics/blocking.rs
+-rw-r--r--   0     1001      127     1219 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_node/src/analytics/mod.rs
+-rw-r--r--   0     1001      127     4931 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_node/src/analytics/payload.rs
+-rw-r--r--   0     1001      127    12828 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_node/src/analytics/sender.rs
+-rw-r--r--   0     1001      127     3085 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_node/src/analytics/sink.rs
+-rw-r--r--   0     1001      127     1900 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_node/src/analytics/sync.rs
+-rw-r--r--   0     1001      127     5045 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_node/src/bin/reader.rs
+-rw-r--r--   0     1001      127     8050 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_node/src/bin/writer.rs
+-rw-r--r--   0     1001      127     1345 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_node/src/cache/mod.rs
+-rw-r--r--   0     1001      127     3043 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_node/src/cache/reader_cache.rs
+-rw-r--r--   0     1001      127    14199 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_node/src/cache/resource_cache.rs
+-rw-r--r--   0     1001      127    11037 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_node/src/cache/writer_cache.rs
+-rw-r--r--   0     1001      127     1771 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_node/src/disk_structure.rs
+-rw-r--r--   0     1001      127     2656 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_node/src/grpc/collect_garbage.rs
+-rw-r--r--   0     1001      127    18821 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_node/src/grpc/grpc_reader.rs
+-rw-r--r--   0     1001      127    13730 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_node/src/grpc/grpc_writer.rs
+-rw-r--r--   0     1001      127     3186 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_node/src/grpc/middleware/debug.rs
+-rw-r--r--   0     1001      127     3440 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_node/src/grpc/middleware/metrics.rs
+-rw-r--r--   0     1001      127     1009 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_node/src/grpc/middleware/mod.rs
+-rw-r--r--   0     1001      127     4158 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_node/src/grpc/middleware/telemetry.rs
+-rw-r--r--   0     1001      127     1283 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_node/src/grpc/mod.rs
+-rw-r--r--   0     1001      127     2581 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_node/src/grpc/update.rs
+-rw-r--r--   0     1001      127     1173 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_node/src/http_server/metrics_service.rs
+-rw-r--r--   0     1001      127     1465 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_node/src/http_server/mod.rs
+-rw-r--r--   0     1001      127     1943 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_node/src/http_server/traces_service.rs
+-rw-r--r--   0     1001      127     1488 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_node/src/lib.rs
+-rw-r--r--   0     1001      127     2757 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_node/src/lifecycle.rs
+-rw-r--r--   0     1001      127     1778 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_node/src/merge/global.rs
+-rw-r--r--   0     1001      127     1089 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_node/src/merge/mod.rs
+-rw-r--r--   0     1001      127    13672 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_node/src/merge/scheduler.rs
+-rw-r--r--   0     1001      127     3677 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_node/src/merge/work.rs
+-rw-r--r--   0     1001      127     1935 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_node/src/node_metadata.rs
+-rw-r--r--   0     1001      127     2417 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_node/src/replication/health.rs
+-rw-r--r--   0     1001      127     1070 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_node/src/replication/mod.rs
+-rw-r--r--   0     1001      127    14103 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_node/src/replication/replicator.rs
+-rw-r--r--   0     1001      127    11755 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_node/src/replication/service.rs
+-rw-r--r--   0     1001      127    11615 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_node/src/settings.rs
+-rw-r--r--   0     1001      127     1111 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_node/src/shards/errors.rs
+-rw-r--r--   0     1001      127    11409 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_node/src/shards/metadata.rs
+-rw-r--r--   0     1001      127     1122 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_node/src/shards/mod.rs
+-rw-r--r--   0     1001      127    24353 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_node/src/shards/shard_reader.rs
+-rw-r--r--   0     1001      127    19629 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_node/src/shards/shard_writer.rs
+-rw-r--r--   0     1001      127    10251 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_node/src/shards/versions.rs
+-rw-r--r--   0     1001      127    10170 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_node/src/telemetry.rs
+-rw-r--r--   0     1001      127     6396 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_node/src/utils.rs
+-rw-r--r--   0     1001      127       42 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_node/test.sh
+-rw-r--r--   0     1001      127     1115 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_node/tests/common/mod.rs
+-rw-r--r--   0     1001      127    12731 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_node/tests/common/node_services.rs
+-rw-r--r--   0     1001      127     7823 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_node/tests/common/resources.rs
+-rw-r--r--   0     1001      127     8173 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_node/tests/test_date_range_search.rs
+-rw-r--r--   0     1001      127     4089 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_node/tests/test_download.rs
+-rw-r--r--   0     1001      127     1684 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_node/tests/test_merge.rs
+-rw-r--r--   0     1001      127     6003 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_node/tests/test_replication.rs
+-rw-r--r--   0     1001      127    22494 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_node/tests/test_search_relations.rs
+-rw-r--r--   0     1001      127     6958 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_node/tests/test_search_sorting.rs
+-rw-r--r--   0     1001      127     7044 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_node/tests/test_security_search.rs
+-rw-r--r--   0     1001      127     6862 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_node/tests/test_shards.rs
+-rw-r--r--   0     1001      127    10698 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_node/tests/test_suggest.rs
+-rw-r--r--   0     1001      127     5438 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_node/tests/test_vector_normalization.rs
+-rw-r--r--   0        0        0      361 1970-01-01 00:00:00.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_procs/Cargo.toml
+-rw-r--r--   0     1001      127     3409 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_procs/src/lib.rs
+-rw-r--r--   0     1001      127     2885 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_procs/src/measure.rs
+-rw-r--r--   0     1001      127     1081 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_procs/tests/dont_compile/actor_defined_twice.rs
+-rw-r--r--   0     1001      127      222 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_procs/tests/dont_compile/actor_defined_twice.stderr
+-rw-r--r--   0     1001      127     1038 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_procs/tests/dont_compile/actor_not_defined.rs
+-rw-r--r--   0     1001      127      327 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_procs/tests/dont_compile/actor_not_defined.stderr
+-rw-r--r--   0     1001      127     1086 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_procs/tests/dont_compile/metric_defined_twice.rs
+-rw-r--r--   0     1001      127      249 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_procs/tests/dont_compile/metric_defined_twice.stderr
+-rw-r--r--   0     1001      127     1046 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_procs/tests/dont_compile/wrong_actor.rs
+-rw-r--r--   0     1001      127     1303 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_procs/tests/dont_compile/wrong_actor.stderr
+-rw-r--r--   0     1001      127     1408 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_procs/tests/test_measure.rs
+-rw-r--r--   0        0        0      628 1970-01-01 00:00:00.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_paragraphs/Cargo.toml
+-rw-r--r--   0     1001      127     7796 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_paragraphs/src/fuzzy_query.rs
+-rw-r--r--   0     1001      127     1009 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_paragraphs/src/lib.rs
+-rw-r--r--   0     1001      127     2780 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_paragraphs/src/query_io.rs
+-rw-r--r--   0     1001      127    43068 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_paragraphs/src/reader.rs
+-rw-r--r--   0     1001      127     4221 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_paragraphs/src/schema.rs
+-rw-r--r--   0     1001      127    21255 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_paragraphs/src/search_query.rs
+-rw-r--r--   0     1001      127    11380 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_paragraphs/src/search_response.rs
+-rw-r--r--   0     1001      127     4090 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_paragraphs/src/stop_words.rs
+-rw-r--r--   0     1001      127    17196 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_paragraphs/src/writer.rs
+-rw-r--r--   0     1001      127       88 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_paragraphs/stop_words/README.md
+-rw-r--r--   0     1001      127    19791 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_paragraphs/stop_words/ar.json
+-rw-r--r--   0     1001      127     1923 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_paragraphs/stop_words/az.json
+-rw-r--r--   0     1001      127    11684 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_paragraphs/stop_words/bn.json
+-rw-r--r--   0     1001      127     2513 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_paragraphs/stop_words/ca.json
+-rw-r--r--   0     1001      127    12802 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_paragraphs/stop_words/ch.json
+-rw-r--r--   0     1001      127      730 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_paragraphs/stop_words/da.json
+-rw-r--r--   0     1001      127     2090 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_paragraphs/stop_words/de.json
+-rw-r--r--   0     1001      127     6284 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_paragraphs/stop_words/el.json
+-rw-r--r--   0     1001      127     1473 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_paragraphs/stop_words/en.json
+-rw-r--r--   0     1001      127     3451 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_paragraphs/stop_words/es.json
+-rw-r--r--   0     1001      127     3182 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_paragraphs/stop_words/eu.json
+-rw-r--r--   0     1001      127     2126 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_paragraphs/stop_words/extract.py
+-rw-r--r--   0     1001      127     2748 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_paragraphs/stop_words/fi.json
+-rw-r--r--   0     1001      127     1388 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_paragraphs/stop_words/fr.json
+-rw-r--r--   0     1001      127     5716 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_paragraphs/stop_words/he.json
+-rw-r--r--   0     1001      127     2108 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_paragraphs/stop_words/hu.json
+-rw-r--r--   0     1001      127     8721 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_paragraphs/stop_words/id.json
+-rw-r--r--   0     1001      127     2535 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_paragraphs/stop_words/it.json
+-rw-r--r--   0     1001      127    11737 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_paragraphs/stop_words/kk.json
+-rw-r--r--   0     1001      127     7730 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_paragraphs/stop_words/ne.json
+-rw-r--r--   0     1001      127      756 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_paragraphs/stop_words/nl.json
+-rw-r--r--   0     1001      127     1447 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_paragraphs/stop_words/no.json
+-rw-r--r--   0     1001      127     2055 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_paragraphs/stop_words/pt.json
+-rw-r--r--   0     1001      127     3327 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_paragraphs/stop_words/ro.json
+-rw-r--r--   0     1001      127     3856 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_paragraphs/stop_words/ru.json
+-rw-r--r--   0     1001      127    23032 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_paragraphs/stop_words/sl.json
+-rw-r--r--   0     1001      127      993 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_paragraphs/stop_words/sv.json
+-rw-r--r--   0     1001      127     5424 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_paragraphs/stop_words/tg.json
+-rw-r--r--   0     1001      127      491 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_paragraphs/stop_words/tr.json
+-rw-r--r--   0        0        0      838 1970-01-01 00:00:00.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_relations/Cargo.toml
+-rw-r--r--   0     1001      127     9354 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_relations/src/bfs_engine.rs
+-rw-r--r--   0     1001      127     1761 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_relations/src/errors.rs
+-rw-r--r--   0     1001      127    21119 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_relations/src/graph_db.rs
+-rw-r--r--   0     1001      127     1784 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_relations/src/graph_test_utils.rs
+-rw-r--r--   0     1001      127    10531 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_relations/src/index.rs
+-rw-r--r--   0     1001      127     1003 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_relations/src/lib.rs
+-rw-r--r--   0     1001      127     5550 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_relations/src/node_dictionary.rs
+-rw-r--r--   0     1001      127     5249 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_relations/src/relations_io.rs
+-rw-r--r--   0     1001      127     2658 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_relations/src/service/bfs.rs
+-rw-r--r--   0     1001      127      970 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_relations/src/service/mod.rs
+-rw-r--r--   0     1001      127     9828 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_relations/src/service/reader.rs
+-rw-r--r--   0     1001      127    10781 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_relations/src/service/tests.rs
+-rw-r--r--   0     1001      127     3071 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_relations/src/service/utils.rs
+-rw-r--r--   0     1001      127     7110 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_relations/src/service/writer.rs
+-rw-r--r--   0        0        0      931 1970-01-01 00:00:00.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_core/Cargo.toml
+-rw-r--r--   0     1001      127     5872 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_core/src/fs_state.rs
+-rw-r--r--   0     1001      127     2681 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_core/src/lib.rs
+-rw-r--r--   0     1001      127     2295 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_core/src/merge.rs
+-rw-r--r--   0     1001      127      906 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_core/src/metrics/meters/mod.rs
+-rw-r--r--   0     1001      127     4869 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_core/src/metrics/meters/prometheus.rs
+-rw-r--r--   0     1001      127     1702 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_core/src/metrics/metric/grpc_ops.rs
+-rw-r--r--   0     1001      127     1442 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_core/src/metrics/metric/mod.rs
+-rw-r--r--   0     1001      127     1950 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_core/src/metrics/metric/replication.rs
+-rw-r--r--   0     1001      127     2626 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_core/src/metrics/metric/request_time.rs
+-rw-r--r--   0     1001      127     1644 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_core/src/metrics/metric/shard_cache.rs
+-rw-r--r--   0     1001      127    21641 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_core/src/metrics/metric/tokio_runtime.rs
+-rw-r--r--   0     1001      127    16736 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_core/src/metrics/metric/tokio_tasks.rs
+-rw-r--r--   0     1001      127     3415 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_core/src/metrics/metric/vectors.rs
+-rw-r--r--   0     1001      127     1324 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_core/src/metrics/mod.rs
+-rw-r--r--   0     1001      127     3074 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_core/src/metrics/task_monitor.rs
+-rw-r--r--   0     1001      127     3920 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_core/src/metrics/tests.rs
+-rw-r--r--   0     1001      127     2990 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_core/src/paragraphs.rs
+-rw-r--r--   0     1001      127    17305 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_core/src/query_language/mod.rs
+-rw-r--r--   0     1001      127    15365 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_core/src/query_planner.rs
+-rw-r--r--   0     1001      127     2069 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_core/src/relations.rs
+-rw-r--r--   0     1001      127     8399 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_core/src/tantivy_replica.rs
+-rw-r--r--   0     1001      127     2603 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_core/src/texts.rs
+-rw-r--r--   0     1001      127     3559 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_core/src/vectors.rs
+-rw-r--r--   0        0        0      398 1970-01-01 00:00:00.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_texts/Cargo.toml
+-rw-r--r--   0     1001      127      931 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_texts/src/lib.rs
+-rw-r--r--   0     1001      127     2755 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_texts/src/query_io.rs
+-rw-r--r--   0     1001      127    21119 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_texts/src/reader.rs
+-rw-r--r--   0     1001      127     2761 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_texts/src/schema.rs
+-rw-r--r--   0     1001      127     8676 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_texts/src/search_query.rs
+-rw-r--r--   0     1001      127     9257 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_texts/src/writer.rs
+-rw-r--r--   0     1001      127     3389 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_texts/tests/common/mod.rs
+-rw-r--r--   0     1001      127     2044 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_texts/tests/test_reader.rs
+-rw-r--r--   0     1001      127     8063 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_texts/tests/test_search.rs
+-rw-r--r--   0     1001      127     1249 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_texts/tests/test_streaming.rs
+-rw-r--r--   0     1001      127     3458 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_texts/tests/test_writer.rs
+-rw-r--r--   0        0        0      399 1970-01-01 00:00:00.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_texts2/Cargo.toml
+-rw-r--r--   0     1001      127      931 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_texts2/src/lib.rs
+-rw-r--r--   0     1001      127     2755 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_texts2/src/query_io.rs
+-rw-r--r--   0     1001      127    22604 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_texts2/src/reader.rs
+-rw-r--r--   0     1001      127     3105 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_texts2/src/schema.rs
+-rw-r--r--   0     1001      127     8682 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_texts2/src/search_query.rs
+-rw-r--r--   0     1001      127    10377 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_texts2/src/writer.rs
+-rw-r--r--   0     1001      127     3391 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_texts2/tests/common/mod.rs
+-rw-r--r--   0     1001      127     2046 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_texts2/tests/test_reader.rs
+-rw-r--r--   0     1001      127     8881 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_texts2/tests/test_search.rs
+-rw-r--r--   0     1001      127     1249 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_texts2/tests/test_streaming.rs
+-rw-r--r--   0     1001      127     3460 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_texts2/tests/test_writer.rs
+-rw-r--r--   0        0        0      742 1970-01-01 00:00:00.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_vectors/Cargo.toml
+-rw-r--r--   0     1001      127       69 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_vectors/README.md
+-rw-r--r--   0     1001      127       43 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_vectors/docs/README.md
+-rw-r--r--   0     1001      127    25718 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_vectors/docs/labels.drawio.svg
+-rw-r--r--   0     1001      127    12340 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_vectors/src/data_point/disk_hnsw.rs
+-rw-r--r--   0     1001      127    24470 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_vectors/src/data_point/mod.rs
+-rw-r--r--   0     1001      127    11214 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_vectors/src/data_point/node.rs
+-rw-r--r--   0     1001      127    14639 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_vectors/src/data_point/ops_hnsw.rs
+-rw-r--r--   0     1001      127     1642 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_vectors/src/data_point/params.rs
+-rw-r--r--   0     1001      127     3952 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_vectors/src/data_point/ram_hnsw.rs
+-rw-r--r--   0     1001      127    14176 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_vectors/src/data_point/tests.rs
+-rw-r--r--   0     1001      127     5798 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_vectors/src/data_point_provider/garbage_collector.rs
+-rw-r--r--   0     1001      127     2777 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_vectors/src/data_point_provider/mod.rs
+-rw-r--r--   0     1001      127    10613 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_vectors/src/data_point_provider/reader.rs
+-rw-r--r--   0     1001      127     2304 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_vectors/src/data_point_provider/replication.rs
+-rw-r--r--   0     1001      127     5288 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_vectors/src/data_point_provider/state.rs
+-rw-r--r--   0     1001      127    20587 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_vectors/src/data_point_provider/writer.rs
+-rw-r--r--   0     1001      127    23710 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_vectors/src/data_types/data_store.rs
+-rw-r--r--   0     1001      127     6916 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_vectors/src/data_types/dtrie_ram.rs
+-rw-r--r--   0     1001      127     1959 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_vectors/src/data_types/mod.rs
+-rw-r--r--   0     1001      127     6143 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_vectors/src/data_types/trie.rs
+-rw-r--r--   0     1001      127     2904 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_vectors/src/data_types/trie_ram.rs
+-rw-r--r--   0     1001      127     4433 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_vectors/src/data_types/vector.rs
+-rw-r--r--   0     1001      127     8116 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_vectors/src/formula/mod.rs
+-rw-r--r--   0     1001      127     2165 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_vectors/src/lib.rs
+-rw-r--r--   0     1001      127     1278 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_vectors/src/service/mod.rs
+-rw-r--r--   0     1001      127     1897 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_vectors/src/service/query_io.rs
+-rw-r--r--   0     1001      127    17236 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_vectors/src/service/reader.rs
+-rw-r--r--   0     1001      127    15869 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_vectors/src/service/writer.rs
+-rw-r--r--   0     1001      127     1668 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_vectors/src/utils.rs
+-rw-r--r--   0     1001      127     2884 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_vectors/tests/test_merge.rs
+-rw-r--r--   0        0        0      943 1970-01-01 00:00:00.000000 nucliadb_node_binding-3.0.3.post1164/Cargo.toml
+-rw-r--r--   0     1001      127     1553 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/CHANGELOG.md
+-rw-r--r--   0     1001      127      895 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/Makefile
+-rw-r--r--   0     1001      127       52 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/README.md
+-rwxr-xr-x   0     1001      127      978 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/cov.sh
+-rw-r--r--   0     1001      127     1309 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/pyproject.toml
+-rw-r--r--   0     1001      127     2195 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/src/collect_garbage.rs
+-rw-r--r--   0     1001      127     1212 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/src/errors.rs
+-rw-r--r--   0     1001      127     2337 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/src/lib.rs
+-rw-r--r--   0     1001      127     9405 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/src/reader.rs
+-rw-r--r--   0     1001      127     2154 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/src/update.rs
+-rw-r--r--   0     1001      127     9162 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/src/writer.rs
+-rw-r--r--   0     1001      127      835 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/tests/__init__.py
+-rw-r--r--   0     1001      127      892 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/tests/conftest.py
+-rw-r--r--   0     1001      127     3903 2024-04-18 09:18:41.000000 nucliadb_node_binding-3.0.3.post1164/tests/integration/test_indexing.py
+-rw-r--r--   0        0        0      401 1970-01-01 00:00:00.000000 nucliadb_node_binding-3.0.3.post1164/PKG-INFO
```

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_protos/build.rs` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_protos/build.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_protos/src/fdbwriter.rs` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_protos/src/fdbwriter.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_protos/src/knowledgebox.rs` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_protos/src/knowledgebox.rs`

 * *Files 3% similar despite different names*

```diff
@@ -37,26 +37,33 @@
 
 #[derive(Clone, PartialEq, ::prost::Message)]
 pub struct KnowledgeBoxNew {
     #[prost(string, tag="1")]
     pub slug: ::prost::alloc::string::String,
     #[prost(message, optional, tag="2")]
     pub config: ::core::option::Option<KnowledgeBoxConfig>,
+    /// this fields are only set by backend when creating hosted KBs
     #[prost(string, tag="3")]
     pub forceuuid: ::prost::alloc::string::String,
     #[prost(enumeration="super::utils::VectorSimilarity", tag="4")]
     pub similarity: i32,
     #[prost(int32, optional, tag="5")]
     pub vector_dimension: ::core::option::Option<i32>,
     #[prost(float, optional, tag="6")]
     pub default_min_score: ::core::option::Option<f32>,
-    #[prost(enumeration="super::utils::ReleaseChannel", tag="7")]
-    pub release_channel: i32,
+    #[prost(uint32, repeated, tag="9")]
+    pub matryoshka_dimensions: ::prost::alloc::vec::Vec<u32>,
+    /// this field are only used by NucliaDB Writer API when creating a KB. Used
+    /// in onprem scenarios
     #[prost(string, tag="8")]
     pub learning_config: ::prost::alloc::string::String,
+    /// release channel, although not used when backend creates hosted KBs, it's
+    /// recomputed and changed depending on the environment
+    #[prost(enumeration="super::utils::ReleaseChannel", tag="7")]
+    pub release_channel: i32,
 }
 #[derive(Clone, PartialEq, ::prost::Message)]
 pub struct NewKnowledgeBoxResponse {
     #[prost(enumeration="KnowledgeBoxResponseStatus", tag="1")]
     pub status: i32,
     #[prost(string, tag="2")]
     pub uuid: ::prost::alloc::string::String,
@@ -230,14 +237,18 @@
 pub struct SemanticModelMetadata {
     #[prost(enumeration="super::utils::VectorSimilarity", tag="1")]
     pub similarity_function: i32,
     #[prost(int32, optional, tag="2")]
     pub vector_dimension: ::core::option::Option<i32>,
     #[prost(float, optional, tag="3")]
     pub default_min_score: ::core::option::Option<f32>,
+    /// list of possible subdivisions of the matryoshka embeddings (if the model
+    /// supports it)
+    #[prost(uint32, repeated, tag="4")]
+    pub matryoshka_dimensions: ::prost::alloc::vec::Vec<u32>,
 }
 // Do not update this model without confirmation of internal Learning Config API
 
 /// Deprecated
 #[derive(Clone, PartialEq, ::prost::Message)]
 pub struct KbConfiguration {
     #[prost(string, tag="2")]
```

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_protos/src/lib.rs` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_protos/src/lib.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_protos/src/nodereader.rs` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_protos/src/nodereader.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_protos/src/noderesources.rs` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_protos/src/noderesources.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_protos/src/nodewriter.rs` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_protos/src/nodewriter.rs`

 * *Files 1% similar despite different names*

```diff
@@ -65,14 +65,17 @@
 pub struct NewShardRequest {
     #[prost(enumeration="super::utils::VectorSimilarity", tag="1")]
     pub similarity: i32,
     #[prost(string, tag="2")]
     pub kbid: ::prost::alloc::string::String,
     #[prost(enumeration="super::utils::ReleaseChannel", tag="3")]
     pub release_channel: i32,
+    /// indicates whether the shard should normalize vectors on indexing or not
+    #[prost(bool, tag="4")]
+    pub normalize_vectors: bool,
 }
 #[derive(Clone, PartialEq, ::prost::Message)]
 pub struct NewVectorSetRequest {
     #[prost(message, optional, tag="1")]
     pub id: ::core::option::Option<super::noderesources::VectorSetId>,
     #[prost(enumeration="super::utils::VectorSimilarity", tag="2")]
     pub similarity: i32,
```

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_protos/src/replication.rs` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_protos/src/replication.rs`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,16 @@
     /// if there is a new version of the shard available to download
     #[prost(string, tag="2")]
     pub generation_id: ::prost::alloc::string::String,
     #[prost(string, tag="3")]
     pub kbid: ::prost::alloc::string::String,
     #[prost(string, tag="4")]
     pub similarity: ::prost::alloc::string::String,
+    #[prost(bool, tag="5")]
+    pub normalize_vectors: bool,
 }
 #[derive(Clone, PartialEq, ::prost::Message)]
 pub struct SecondaryShardReplicationState {
     #[prost(string, tag="1")]
     pub shard_id: ::prost::alloc::string::String,
     /// ID to identify the generation of the shard to know
     /// if there is a new version of the shard available to download
```

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_protos/src/resources.rs` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_protos/src/resources.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_protos/src/utils.rs` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_protos/src/utils.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_texts2/src/lib.rs` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_texts/src/lib.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_texts2/src/query_io.rs` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_texts/src/query_io.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_texts2/src/reader.rs` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_texts2/src/reader.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_texts2/src/schema.rs` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_texts2/src/schema.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_texts2/src/search_query.rs` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_texts2/src/search_query.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_texts2/src/writer.rs` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_texts2/src/writer.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_texts2/tests/common/mod.rs` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_texts2/tests/common/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_texts2/tests/test_reader.rs` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_texts2/tests/test_reader.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_texts2/tests/test_search.rs` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_texts2/tests/test_search.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_texts2/tests/test_streaming.rs` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_texts/tests/test_streaming.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_texts2/tests/test_writer.rs` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_texts2/tests/test_writer.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_texts/src/lib.rs` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_texts2/src/lib.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_texts/src/query_io.rs` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_texts2/src/query_io.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_texts/src/reader.rs` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_texts/src/reader.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_texts/src/schema.rs` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_texts/src/schema.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_texts/src/search_query.rs` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_texts/src/search_query.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_texts/src/writer.rs` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_texts/src/writer.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_texts/tests/common/mod.rs` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_texts/tests/common/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_texts/tests/test_reader.rs` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_texts/tests/test_reader.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_texts/tests/test_search.rs` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_texts/tests/test_search.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_texts/tests/test_streaming.rs` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_texts2/tests/test_streaming.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_texts/tests/test_writer.rs` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_texts/tests/test_writer.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_paragraphs/Cargo.toml` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_paragraphs/Cargo.toml`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_paragraphs/src/fuzzy_query.rs` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_paragraphs2/src/fuzzy_query.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_paragraphs/src/lib.rs` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_paragraphs2/src/lib.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_paragraphs/src/query_io.rs` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_paragraphs2/src/query_io.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_paragraphs/src/reader.rs` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_paragraphs/src/reader.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_paragraphs/src/schema.rs` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_paragraphs/src/schema.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_paragraphs/src/search_query.rs` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_paragraphs/src/search_query.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_paragraphs/src/search_response.rs` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_paragraphs/src/search_response.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_paragraphs/src/stop_words.rs` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_paragraphs2/src/stop_words.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_paragraphs/src/writer.rs` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_paragraphs/src/writer.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_paragraphs/stop_words/ar.json` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_paragraphs2/stop_words/ar.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_paragraphs/stop_words/az.json` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_paragraphs2/stop_words/az.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_paragraphs/stop_words/bn.json` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_paragraphs2/stop_words/bn.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_paragraphs/stop_words/ca.json` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_paragraphs2/stop_words/ca.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_paragraphs/stop_words/ch.json` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_paragraphs2/stop_words/ch.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_paragraphs/stop_words/da.json` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_paragraphs2/stop_words/da.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_paragraphs/stop_words/de.json` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_paragraphs2/stop_words/de.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_paragraphs/stop_words/el.json` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_paragraphs2/stop_words/el.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_paragraphs/stop_words/en.json` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_paragraphs2/stop_words/en.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_paragraphs/stop_words/es.json` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_paragraphs2/stop_words/es.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_paragraphs/stop_words/eu.json` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_paragraphs2/stop_words/eu.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_paragraphs/stop_words/extract.py` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_paragraphs2/stop_words/extract.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_paragraphs/stop_words/fi.json` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_paragraphs2/stop_words/fi.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_paragraphs/stop_words/fr.json` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_paragraphs2/stop_words/fr.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_paragraphs/stop_words/he.json` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_paragraphs2/stop_words/he.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_paragraphs/stop_words/hu.json` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_paragraphs2/stop_words/hu.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_paragraphs/stop_words/id.json` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_paragraphs2/stop_words/id.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_paragraphs/stop_words/it.json` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_paragraphs2/stop_words/it.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_paragraphs/stop_words/kk.json` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_paragraphs2/stop_words/kk.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_paragraphs/stop_words/ne.json` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_paragraphs2/stop_words/ne.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_paragraphs/stop_words/nl.json` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_paragraphs2/stop_words/nl.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_paragraphs/stop_words/no.json` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_paragraphs2/stop_words/no.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_paragraphs/stop_words/pt.json` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_paragraphs2/stop_words/pt.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_paragraphs/stop_words/ro.json` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_paragraphs2/stop_words/ro.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_paragraphs/stop_words/ru.json` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_paragraphs2/stop_words/ru.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_paragraphs/stop_words/sl.json` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_paragraphs2/stop_words/sl.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_paragraphs/stop_words/sv.json` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_paragraphs2/stop_words/sv.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_paragraphs/stop_words/tg.json` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_paragraphs2/stop_words/tg.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_relations2/Cargo.toml` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_relations2/Cargo.toml`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_relations2/src/io_maps.rs` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_relations2/src/io_maps.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_relations2/src/lib.rs` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_relations2/src/lib.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_relations2/src/reader.rs` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_relations2/src/reader.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_relations2/src/schema.rs` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_relations2/src/schema.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_relations2/src/writer.rs` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_relations2/src/writer.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_relations2/tests/common/mod.rs` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_relations2/tests/common/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_relations2/tests/test_reader.rs` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_relations2/tests/test_reader.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_relations2/tests/test_writer.rs` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_relations2/tests/test_writer.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_paragraphs2/Cargo.toml` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_paragraphs2/Cargo.toml`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_paragraphs2/src/fuzzy_query.rs` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_paragraphs/src/fuzzy_query.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_paragraphs2/src/lib.rs` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_paragraphs/src/lib.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_paragraphs2/src/query_io.rs` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_paragraphs/src/query_io.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_paragraphs2/src/reader.rs` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_paragraphs2/src/reader.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_paragraphs2/src/schema.rs` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_paragraphs2/src/schema.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_paragraphs2/src/search_query.rs` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_paragraphs2/src/search_query.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_paragraphs2/src/search_response.rs` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_paragraphs2/src/search_response.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_paragraphs2/src/stop_words.rs` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_paragraphs/src/stop_words.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_paragraphs2/src/writer.rs` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_paragraphs2/src/writer.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_paragraphs2/stop_words/ar.json` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_paragraphs/stop_words/ar.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_paragraphs2/stop_words/az.json` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_paragraphs/stop_words/az.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_paragraphs2/stop_words/bn.json` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_paragraphs/stop_words/bn.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_paragraphs2/stop_words/ca.json` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_paragraphs/stop_words/ca.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_paragraphs2/stop_words/ch.json` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_paragraphs/stop_words/ch.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_paragraphs2/stop_words/da.json` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_paragraphs/stop_words/da.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_paragraphs2/stop_words/de.json` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_paragraphs/stop_words/de.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_paragraphs2/stop_words/el.json` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_paragraphs/stop_words/el.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_paragraphs2/stop_words/en.json` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_paragraphs/stop_words/en.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_paragraphs2/stop_words/es.json` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_paragraphs/stop_words/es.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_paragraphs2/stop_words/eu.json` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_paragraphs/stop_words/eu.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_paragraphs2/stop_words/extract.py` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_paragraphs/stop_words/extract.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_paragraphs2/stop_words/fi.json` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_paragraphs/stop_words/fi.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_paragraphs2/stop_words/fr.json` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_paragraphs/stop_words/fr.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_paragraphs2/stop_words/he.json` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_paragraphs/stop_words/he.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_paragraphs2/stop_words/hu.json` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_paragraphs/stop_words/hu.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_paragraphs2/stop_words/id.json` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_paragraphs/stop_words/id.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_paragraphs2/stop_words/it.json` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_paragraphs/stop_words/it.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_paragraphs2/stop_words/kk.json` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_paragraphs/stop_words/kk.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_paragraphs2/stop_words/ne.json` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_paragraphs/stop_words/ne.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_paragraphs2/stop_words/nl.json` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_paragraphs/stop_words/nl.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_paragraphs2/stop_words/no.json` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_paragraphs/stop_words/no.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_paragraphs2/stop_words/pt.json` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_paragraphs/stop_words/pt.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_paragraphs2/stop_words/ro.json` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_paragraphs/stop_words/ro.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_paragraphs2/stop_words/ru.json` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_paragraphs/stop_words/ru.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_paragraphs2/stop_words/sl.json` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_paragraphs/stop_words/sl.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_paragraphs2/stop_words/sv.json` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_paragraphs/stop_words/sv.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_paragraphs2/stop_words/tg.json` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_paragraphs/stop_words/tg.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_node/Cargo.toml` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_node/Cargo.toml`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_node/.rustc_info.json` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_node/.rustc_info.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_node/Makefile` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_node/Makefile`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_node/README.md` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_node/README.md`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_node/nucliadb_node/__init__.py` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_node/nucliadb_node/__init__.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_node/nucliadb_node/app.py` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_node/nucliadb_node/app.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_node/nucliadb_node/indexer.py` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_node/nucliadb_node/indexer.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_node/nucliadb_node/listeners/__init__.py` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_node/nucliadb_node/listeners/__init__.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_node/nucliadb_node/listeners/indexed_publisher.py` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_node/nucliadb_node/listeners/indexed_publisher.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_node/nucliadb_node/pull.py` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_node/nucliadb_node/pull.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_node/nucliadb_node/service.py` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_node/nucliadb_node/service.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_node/nucliadb_node/settings.py` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_node/nucliadb_node/settings.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_node/nucliadb_node/signals.py` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_node/nucliadb_node/signals.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_node/nucliadb_node/tests/__init__.py` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_node/nucliadb_node/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_node/nucliadb_node/tests/conftest.py` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_node/nucliadb_node/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_node/nucliadb_node/tests/fixtures.py` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_node/nucliadb_node/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_node/nucliadb_node/tests/integration/test_indexing.py` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_node/nucliadb_node/tests/integration/test_indexing.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_node/nucliadb_node/tests/unit/test_app.py` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_node/nucliadb_node/tests/unit/test_app.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_node/nucliadb_node/tests/unit/test_indexed_publisher.py` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_node/nucliadb_node/tests/unit/test_indexed_publisher.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_node/nucliadb_node/tests/unit/test_indexer.py` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_node/nucliadb_node/tests/unit/test_indexer.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_node/nucliadb_node/tests/unit/test_pull.py` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_node/nucliadb_node/tests/unit/test_pull.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_node/nucliadb_node/writer.py` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_node/nucliadb_node/writer.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_node/setup.py` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_node/setup.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_node/src/analytics/blocking.rs` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_node/src/analytics/blocking.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_node/src/analytics/mod.rs` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_node/src/analytics/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_node/src/analytics/payload.rs` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_node/src/analytics/payload.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_node/src/analytics/sender.rs` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_node/src/analytics/sender.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_node/src/analytics/sink.rs` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_node/src/analytics/sink.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_node/src/analytics/sync.rs` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_node/src/analytics/sync.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_node/src/bin/reader.rs` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_node/src/bin/reader.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_node/src/bin/writer.rs` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_node/src/bin/writer.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_node/src/cache/mod.rs` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_node/src/cache/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_node/src/cache/reader_cache.rs` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_node/src/cache/reader_cache.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_node/src/cache/resource_cache.rs` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_node/src/cache/resource_cache.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_node/src/cache/writer_cache.rs` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_node/src/cache/writer_cache.rs`

 * *Files 1% similar despite different names*

```diff
@@ -252,15 +252,16 @@
         .into();
         let cache = Arc::new(ShardWriterCache::new(settings.clone()));
 
         let shard_id_0 = ShardId::from("shard_id_0");
         let shard_0_path = settings.shards_path().join(shard_id_0.clone());
         fs::create_dir(settings.shards_path()).unwrap();
 
-        let shard_meta = ShardMetadata::new(shard_0_path.clone(), shard_id_0.clone(), None, Similarity::Cosine, None);
+        let shard_meta =
+            ShardMetadata::new(shard_0_path.clone(), shard_id_0.clone(), None, Similarity::Cosine, None, false);
         cache.create(shard_meta).unwrap();
 
         let shard_0 = cache.get(&shard_id_0).unwrap();
 
         scope(|scope| {
             let cache_clone = cache.clone();
             let shard_id_0_clone = shard_id_0.clone();
@@ -292,13 +293,14 @@
         })
         .unwrap();
 
         // Shard is deleted, getting it should fail to load
         assert!(cache.get(&shard_id_0).is_err());
 
         // Recreating the shard should work (i.e: it's not stuck in the deletion state)
-        let shard_meta = ShardMetadata::new(shard_0_path.clone(), shard_id_0.clone(), None, Similarity::Cosine, None);
+        let shard_meta =
+            ShardMetadata::new(shard_0_path.clone(), shard_id_0.clone(), None, Similarity::Cosine, None, false);
         cache.create(shard_meta).unwrap();
 
         assert!(cache.get(&shard_id_0).is_ok());
     }
 }
```

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_node/src/disk_structure.rs` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_node/src/disk_structure.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_node/src/grpc/collect_garbage.rs` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_node/src/grpc/collect_garbage.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_node/src/grpc/grpc_reader.rs` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_node/src/grpc/grpc_reader.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_node/src/grpc/grpc_writer.rs` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_node/src/grpc/grpc_writer.rs`

 * *Files 1% similar despite different names*

```diff
@@ -119,14 +119,15 @@
         let shard_id = uuid::Uuid::new_v4().to_string();
         let metadata = ShardMetadata::new(
             self.shards.shards_path.join(shard_id.clone()),
             shard_id,
             Some(kbid),
             request.similarity().into(),
             Some(Channel::from(request.release_channel)),
+            request.normalize_vectors,
         );
 
         let shards = Arc::clone(&self.shards);
         let new_shard = tokio::task::spawn_blocking(move || shards.create(metadata))
             .await
             .map_err(|error| tonic::Status::internal(format!("Error creating shard: {error:?}")))?;
```

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_node/src/grpc/middleware/debug.rs` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_node/src/grpc/middleware/debug.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_node/src/grpc/middleware/metrics.rs` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_node/src/grpc/middleware/metrics.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_node/src/grpc/middleware/mod.rs` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_node/src/grpc/middleware/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_node/src/grpc/middleware/telemetry.rs` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_node/src/grpc/middleware/telemetry.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_node/src/grpc/mod.rs` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_node/src/grpc/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_node/src/grpc/update.rs` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_node/src/grpc/update.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_node/src/http_server/metrics_service.rs` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_node/src/http_server/metrics_service.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_node/src/http_server/mod.rs` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_node/src/http_server/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_node/src/http_server/traces_service.rs` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_node/src/http_server/traces_service.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_node/src/lib.rs` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_node/src/lib.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_node/src/lifecycle.rs` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_node/src/lifecycle.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_node/src/merge/global.rs` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_node/src/merge/global.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_node/src/merge/mod.rs` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_node/src/merge/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_node/src/merge/scheduler.rs` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_node/src/merge/scheduler.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_node/src/merge/work.rs` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_node/src/merge/work.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_node/src/node_metadata.rs` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_node/src/node_metadata.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_node/src/replication/health.rs` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_node/src/replication/health.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_node/src/replication/mod.rs` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_node/src/replication/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_node/src/replication/replicator.rs` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_node/src/replication/replicator.rs`

 * *Files 1% similar despite different names*

```diff
@@ -263,14 +263,15 @@
             } else {
                 let metadata = ShardMetadata::new(
                     shards_path.join(shard_id.clone()),
                     shard_state.shard_id.clone(),
                     Some(shard_state.kbid.clone()),
                     shard_state.similarity.clone().into(),
                     None,
+                    shard_state.normalize_vectors,
                 );
                 let shard_cache_clone = Arc::clone(&shard_cache);
 
                 warn!("Creating shard to replicate: {shard_id}");
                 let shard_create = tokio::task::spawn_blocking(move || shard_cache_clone.create(metadata)).await?;
                 if shard_create.is_err() {
                     warn!("Failed to create shard: {:?}", shard_create);
```

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_node/src/replication/service.rs` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_node/src/replication/service.rs`

 * *Files 1% similar despite different names*

```diff
@@ -225,14 +225,15 @@
                     let similarity: Similarity = metadata.similarity().into();
 
                     resp_shard_states.push(replication::PrimaryShardReplicationState {
                         shard_id,
                         generation_id: gen_id,
                         kbid: metadata.kbid().unwrap_or_default(),
                         similarity: similarity.to_string(),
+                        normalize_vectors: metadata.normalize_vectors(),
                     });
                 }
             } else {
                 warn!("Shard {} metadata not found", shard_id);
             }
         }
```

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_node/src/settings.rs` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_node/src/settings.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_node/src/shards/errors.rs` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_node/src/shards/errors.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_node/src/shards/metadata.rs` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_node/src/shards/metadata.rs`

 * *Files 5% similar despite different names*

```diff
@@ -72,23 +72,25 @@
 #[derive(Serialize, Deserialize, Default, Clone, Debug)]
 pub struct ShardMetadataFile {
     pub kbid: Option<String>,
     pub similarity: Option<Similarity>,
     pub id: Option<String>,
     #[serde(default)]
     pub channel: Option<Channel>,
+    pub normalize_vectors: Option<bool>,
 }
 
 #[derive(Default, Debug)]
 pub struct ShardMetadata {
     shard_path: PathBuf,
     id: String,
     kbid: Option<String>,
     similarity: Option<Similarity>,
     channel: Option<Channel>,
+    normalize_vectors: bool,
     // A generation id is a way to track if a shard has changed.
     // A new id means that something in the shard has changed.
     // This is used by replication to track which shards have changed
     // and to efficiently replicate them.
     generation_id: RwLock<Option<String>>,
 }
 
@@ -104,71 +106,87 @@
         let metadata: ShardMetadataFile = serde_json::from_reader(&mut reader)?;
         Ok(ShardMetadata {
             shard_path,
             kbid: metadata.kbid,
             similarity: metadata.similarity,
             id: metadata.id.unwrap_or(requested_shard_id),
             channel: metadata.channel,
+            normalize_vectors: metadata.normalize_vectors.unwrap_or(false),
             generation_id: RwLock::new(None),
         })
     }
+
     pub fn new(
         shard_path: PathBuf,
         id: String,
         kbid: Option<String>,
         similarity: Similarity,
         channel: Option<Channel>,
+        normalize_vectors: bool,
     ) -> ShardMetadata {
         ShardMetadata {
             shard_path,
             kbid,
             similarity: Some(similarity),
             id,
             channel,
+            normalize_vectors,
             generation_id: RwLock::new(None),
         }
     }
+
     pub fn exists(shard_path: &Path) -> bool {
         let metadata_path = shard_path.join(disk_structure::METADATA_FILE);
         metadata_path.exists()
     }
+
     pub fn serialize_metadata(&self) -> NodeResult<()> {
         let metadata_path = self.shard_path.join(disk_structure::METADATA_FILE);
         let temp_metadata_path = metadata_path.with_extension("tmp");
 
         let mut writer = BufWriter::new(File::create(temp_metadata_path.clone())?);
         serde_json::to_writer(
             &mut writer,
             &ShardMetadataFile {
                 kbid: self.kbid.clone(),
                 similarity: self.similarity,
                 id: Some(self.id.clone()),
                 channel: self.channel,
+                normalize_vectors: Some(self.normalize_vectors),
             },
         )?;
         writer.flush()?;
 
         std::fs::rename(temp_metadata_path, metadata_path)?;
 
         self.new_generation_id();
 
         Ok(())
     }
+
     pub fn shard_path(&self) -> PathBuf {
         self.shard_path.clone()
     }
+
     pub fn kbid(&self) -> Option<String> {
         self.kbid.clone()
     }
+
     pub fn similarity(&self) -> protos::VectorSimilarity {
         self.similarity.unwrap_or(Similarity::Cosine).into()
     }
+
     pub fn channel(&self) -> Channel {
         self.channel.unwrap_or_default()
     }
+
+    pub fn normalize_vectors(&self) -> bool {
+        self.normalize_vectors
+    }
+
     pub fn id(&self) -> String {
         self.id.clone()
     }
 
     pub fn get_generation_id(&self) -> Option<String> {
         if let Ok(gen_id_read) = self.generation_id.read() {
             match &*gen_id_read {
@@ -257,20 +275,25 @@
         let dir = TempDir::new().unwrap();
         let meta = ShardMetadata::new(
             dir.path().to_path_buf(),
             "ID".to_string(),
             Some("KB".to_string()),
             Similarity::Cosine,
             Some(Channel::EXPERIMENTAL),
+            false,
         );
         meta.serialize_metadata().unwrap();
         let meta_disk = ShardMetadata::open(dir.path().to_path_buf()).unwrap();
         assert_eq!(meta.kbid, meta_disk.kbid);
         assert_eq!(meta.similarity, meta_disk.similarity);
+        assert_eq!(meta.id, meta_disk.id);
+        assert_eq!(meta.channel, meta_disk.channel);
+        assert_eq!(meta.normalize_vectors, meta_disk.normalize_vectors);
     }
+
     #[test]
     fn open_empty() {
         let dir = TempDir::new().unwrap();
         assert!(!ShardMetadata::exists(dir.path()));
         let meta = ShardMetadata::open(dir.path().to_path_buf());
         assert!(meta.is_err());
     }
@@ -294,14 +317,15 @@
         let dir = TempDir::new().unwrap();
         let meta = ShardMetadata::new(
             dir.path().to_path_buf(),
             "ID".to_string(),
             Some("KB".to_string()),
             Similarity::Cosine,
             Some(Channel::EXPERIMENTAL),
+            false,
         );
         let gen_id = meta.get_generation_id();
         assert_eq!(gen_id, meta.get_generation_id());
         // assert!(meta.generation_id.read().unwrap().is_none());
         // let gen_id = meta.get_generation_id();
         // assert_eq!(
         //     *meta.generation_id.read().unwrap().as_ref().unwrap(),
```

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_node/src/shards/mod.rs` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_node/src/shards/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_node/src/shards/shard_reader.rs` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_node/src/shards/shard_reader.rs`

 * *Files 0% similar despite different names*

```diff
@@ -234,14 +234,15 @@
         let channel = metadata.channel();
 
         let vsc = VectorConfig {
             similarity: None,
             path: shard_path.join(VECTORS_DIR),
             channel,
             shard_id: id.clone(),
+            normalize_vectors: metadata.normalize_vectors(),
         };
         let rsc = RelationConfig {
             path: shard_path.join(RELATIONS_DIR),
             channel,
         };
         let versions = Versions::load(&shard_path.join(VERSION_FILE))?;
         let text_task = || Some(versions.get_texts_reader(&tsc));
```

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_node/src/shards/shard_writer.rs` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_node/src/shards/shard_writer.rs`

 * *Files 2% similar despite different names*

```diff
@@ -187,14 +187,15 @@
         let channel = metadata.channel();
 
         let vsc = VectorConfig {
             similarity: Some(metadata.similarity()),
             path: path.join(VECTORS_DIR),
             channel,
             shard_id: metadata.id(),
+            normalize_vectors: metadata.normalize_vectors(),
         };
         let rsc = RelationConfig {
             path: path.join(RELATIONS_DIR),
             channel,
         };
 
         std::fs::create_dir(path)?;
@@ -218,14 +219,15 @@
         let channel = metadata.channel();
 
         let vsc = VectorConfig {
             similarity: None,
             path: path.join(VECTORS_DIR),
             channel,
             shard_id: metadata.id(),
+            normalize_vectors: metadata.normalize_vectors(),
         };
         let rsc = RelationConfig {
             path: path.join(RELATIONS_DIR),
             channel,
         };
 
         ShardWriter::initialize(metadata, tsc, psc, vsc, rsc)
```

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_node/src/shards/versions.rs` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_node/src/shards/versions.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_node/src/telemetry.rs` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_node/src/telemetry.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_node/src/utils.rs` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_node/src/utils.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_node/tests/common/mod.rs` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_node/tests/common/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_node/tests/common/node_services.rs` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_node/tests/common/node_services.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_node/tests/common/resources.rs` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_node/tests/common/resources.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_node/tests/test_date_range_search.rs` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_node/tests/test_date_range_search.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_node/tests/test_download.rs` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_node/tests/test_download.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_node/tests/test_merge.rs` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_node/tests/test_merge.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_node/tests/test_replication.rs` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_node/tests/test_replication.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_node/tests/test_search_relations.rs` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_node/tests/test_search_relations.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_node/tests/test_search_sorting.rs` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_node/tests/test_search_sorting.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_node/tests/test_security_search.rs` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_node/tests/test_security_search.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_node/tests/test_shards.rs` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_node/tests/test_shards.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_node/tests/test_suggest.rs` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_node/tests/test_suggest.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_relations/Cargo.toml` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_relations/Cargo.toml`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_relations/src/bfs_engine.rs` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_relations/src/bfs_engine.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_relations/src/errors.rs` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_relations/src/errors.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_relations/src/graph_db.rs` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_relations/src/graph_db.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_relations/src/graph_test_utils.rs` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_relations/src/graph_test_utils.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_relations/src/index.rs` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_relations/src/index.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_relations/src/lib.rs` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_relations/src/lib.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_relations/src/node_dictionary.rs` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_relations/src/node_dictionary.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_relations/src/relations_io.rs` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_relations/src/relations_io.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_relations/src/service/bfs.rs` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_relations/src/service/bfs.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_relations/src/service/mod.rs` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_relations/src/service/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_relations/src/service/reader.rs` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_relations/src/service/reader.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_relations/src/service/tests.rs` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_relations/src/service/tests.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_relations/src/service/utils.rs` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_relations/src/service/utils.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_relations/src/service/writer.rs` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_relations/src/service/writer.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_core/Cargo.toml` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_core/Cargo.toml`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_core/src/fs_state.rs` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_core/src/fs_state.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_core/src/lib.rs` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_core/src/lib.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_core/src/merge.rs` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_core/src/merge.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_core/src/metrics/meters/mod.rs` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_core/src/metrics/meters/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_core/src/metrics/meters/prometheus.rs` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_core/src/metrics/meters/prometheus.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_core/src/metrics/metric/grpc_ops.rs` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_core/src/metrics/metric/grpc_ops.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_core/src/metrics/metric/mod.rs` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_core/src/metrics/metric/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_core/src/metrics/metric/replication.rs` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_core/src/metrics/metric/replication.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_core/src/metrics/metric/request_time.rs` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_core/src/metrics/metric/request_time.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_core/src/metrics/metric/shard_cache.rs` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_core/src/metrics/metric/shard_cache.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_core/src/metrics/metric/tokio_runtime.rs` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_core/src/metrics/metric/tokio_runtime.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_core/src/metrics/metric/tokio_tasks.rs` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_core/src/metrics/metric/tokio_tasks.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_core/src/metrics/metric/vectors.rs` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_core/src/metrics/metric/vectors.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_core/src/metrics/mod.rs` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_core/src/metrics/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_core/src/metrics/task_monitor.rs` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_core/src/metrics/task_monitor.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_core/src/metrics/tests.rs` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_core/src/metrics/tests.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_core/src/paragraphs.rs` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_core/src/paragraphs.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_core/src/query_language/mod.rs` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_core/src/query_language/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_core/src/query_planner.rs` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_core/src/query_planner.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_core/src/relations.rs` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_core/src/relations.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_core/src/tantivy_replica.rs` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_core/src/tantivy_replica.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_core/src/texts.rs` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_core/src/texts.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_core/src/vectors.rs` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_core/src/vectors.rs`

 * *Files 4% similar despite different names*

```diff
@@ -49,14 +49,15 @@
 
 #[derive(Clone)]
 pub struct VectorConfig {
     pub similarity: Option<VectorSimilarity>,
     pub path: PathBuf,
     pub channel: Channel,
     pub shard_id: String,
+    pub normalize_vectors: bool,
 }
 
 // In an ideal world this should be part of the actual request, but since
 // we use protos all the way down the stack here we are. Once the protos use
 // is restricted to only the upper layer, this type won't be needed anymore.
 #[derive(Clone, Default)]
 pub struct VectorsContext {
```

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_vectors/Cargo.toml` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_vectors/Cargo.toml`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_vectors/docs/labels.drawio.svg` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_vectors/docs/labels.drawio.svg`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_vectors/src/data_point/disk_hnsw.rs` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_vectors/src/data_point/disk_hnsw.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_vectors/src/data_point/mod.rs` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_vectors/src/data_point/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_vectors/src/data_point/node.rs` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_vectors/src/data_point/node.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_vectors/src/data_point/ops_hnsw.rs` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_vectors/src/data_point/ops_hnsw.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_vectors/src/data_point/params.rs` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_vectors/src/data_point/params.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_vectors/src/data_point/ram_hnsw.rs` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_vectors/src/data_point/ram_hnsw.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_vectors/src/data_point/tests.rs` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_vectors/src/data_point/tests.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_vectors/src/data_point_provider/garbage_collector.rs` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_vectors/src/data_point_provider/garbage_collector.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_vectors/src/data_point_provider/mod.rs` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_vectors/src/data_point_provider/mod.rs`

 * *Files 6% similar despite different names*

```diff
@@ -66,14 +66,16 @@
 
 #[derive(Debug, Default, Serialize, Deserialize)]
 pub struct IndexMetadata {
     #[serde(default)]
     pub similarity: Similarity,
     #[serde(default)]
     pub channel: Channel,
+    #[serde(default)]
+    pub normalize_vectors: bool,
 }
 impl IndexMetadata {
     pub fn write(&self, path: &Path) -> VectorR<()> {
         let mut writer = BufWriter::new(File::create(path.join(METADATA))?);
         serde_json::to_writer(&mut writer, self)?;
         Ok(writer.flush()?)
     }
```

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_vectors/src/data_point_provider/reader.rs` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_vectors/src/data_point_provider/reader.rs`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 
 use crate::data_point::{self, DataPointPin, OpenDataPoint, SearchParams};
 pub use crate::data_point::{DpId, Neighbour};
 use crate::data_point_provider::state::read_state;
 use crate::data_point_provider::{IndexMetadata, SearchRequest, OPENING_FLAG, STATE};
 use crate::data_types::dtrie_ram::DTrie;
 use crate::data_types::DeleteLog;
+use crate::utils;
 use crate::{VectorErr, VectorR};
 use fs2::FileExt;
 use fxhash::{FxHashMap, FxHashSet};
 use std::cmp::Ordering;
 use std::collections::{HashMap, HashSet};
 use std::fs::File;
 use std::io;
@@ -225,20 +226,28 @@
         Ok(())
     }
 
     pub fn search(&self, request: &dyn SearchRequest) -> VectorR<Vec<Neighbour>> {
         let Some(dimension) = self.dimension else {
             return Ok(Vec::with_capacity(0));
         };
-        if dimension != request.get_query().len() as u64 {
+
+        let normalized_query;
+        let query = if self.metadata.normalize_vectors {
+            normalized_query = utils::normalize_vector(request.get_query());
+            &normalized_query
+        } else {
+            request.get_query()
+        };
+
+        if dimension != query.len() as u64 {
             return Err(VectorErr::InconsistentDimensions);
         }
 
         let similarity = self.metadata.similarity;
-        let query = request.get_query();
         let filter = request.get_filter();
         let with_duplicates = request.with_duplicates();
         let no_results = request.no_results();
         let min_score = request.min_score();
         let mut ffsv = Fssc::new(request.no_results(), with_duplicates);
 
         for open_data_point in self.open_data_points.values() {
```

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_vectors/src/data_point_provider/replication.rs` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_vectors/src/data_point_provider/replication.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_vectors/src/data_point_provider/state.rs` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_vectors/src/data_point_provider/state.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_vectors/src/data_point_provider/writer.rs` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_vectors/src/data_point_provider/writer.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_vectors/src/data_types/data_store.rs` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_vectors/src/data_types/data_store.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_vectors/src/data_types/dtrie_ram.rs` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_vectors/src/data_types/dtrie_ram.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_vectors/src/data_types/mod.rs` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_vectors/src/data_types/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_vectors/src/data_types/trie.rs` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_vectors/src/data_types/trie.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_vectors/src/data_types/trie_ram.rs` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_vectors/src/data_types/trie_ram.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_vectors/src/data_types/vector.rs` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_vectors/src/data_types/vector.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_vectors/src/formula/mod.rs` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_vectors/src/formula/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_vectors/src/lib.rs` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_vectors/src/lib.rs`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 //
 
 pub mod data_point;
 pub mod data_point_provider;
 mod data_types;
 pub mod formula;
 pub mod service;
+mod utils;
 
 use thiserror::Error;
 #[derive(Debug, Error)]
 pub enum VectorErr {
     #[error("Error using bincode: {0}")]
     BincodeError(#[from] bincode::Error),
     #[error("Error using fst: {0}")]
```

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_vectors/src/service/mod.rs` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_vectors/src/service/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_vectors/src/service/query_io.rs` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_vectors/src/service/query_io.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_vectors/src/service/reader.rs` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_vectors/src/service/reader.rs`

 * *Files 3% similar despite different names*

```diff
@@ -199,14 +199,15 @@
     fn test_key_prefix_search() {
         let dir = TempDir::new().unwrap();
         let vsc = VectorConfig {
             similarity: Some(VectorSimilarity::Cosine),
             path: dir.path().join("vectors"),
             channel: Channel::EXPERIMENTAL,
             shard_id: "abc".into(),
+            normalize_vectors: false,
         };
         let raw_sentences = [
             ("DOC/KEY/1/1".to_string(), vec![1.0, 3.0, 4.0]),
             ("DOC/KEY/1/2".to_string(), vec![2.0, 4.0, 5.0]),
             ("DOC/KEY/1/3".to_string(), vec![3.0, 5.0, 6.0]),
             ("DOC/KEY/1/4".to_string(), vec![3.0, 5.0, 6.0]),
         ];
@@ -281,14 +282,15 @@
     fn test_new_vector_reader() {
         let dir = TempDir::new().unwrap();
         let vsc = VectorConfig {
             similarity: Some(VectorSimilarity::Cosine),
             path: dir.path().join("vectors"),
             channel: Channel::EXPERIMENTAL,
             shard_id: "abc".into(),
+            normalize_vectors: false,
         };
         let raw_sentences = [
             ("DOC/KEY/1/1".to_string(), vec![1.0, 3.0, 4.0]),
             ("DOC/KEY/1/2".to_string(), vec![2.0, 4.0, 5.0]),
             ("DOC/KEY/1/3".to_string(), vec![3.0, 5.0, 6.0]),
             ("DOC/KEY/1/4".to_string(), vec![3.0, 5.0, 6.0]),
         ];
@@ -402,14 +404,15 @@
     fn test_vectors_deduplication() {
         let dir = TempDir::new().unwrap();
         let vsc = VectorConfig {
             similarity: Some(VectorSimilarity::Cosine),
             path: dir.path().join("vectors"),
             channel: Channel::EXPERIMENTAL,
             shard_id: "abc".into(),
+            normalize_vectors: false,
         };
         let raw_sentences =
             [("DOC/KEY/1/1".to_string(), vec![1.0, 2.0, 3.0]), ("DOC/KEY/1/2".to_string(), vec![1.0, 2.0, 3.0])];
         let resource_id = ResourceId {
             shard_id: "DOC".to_string(),
             uuid: "DOC/KEY".to_string(),
         };
```

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_vectors/src/service/writer.rs` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_vectors/src/service/writer.rs`

 * *Files 4% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 // You should have received a copy of the GNU Affero General Public License
 // along with this program. If not, see <http://www.gnu.org/licenses/>.
 
 use crate::data_point::{self, DataPointPin, Elem, LabelDictionary};
 use crate::data_point_provider::garbage_collector;
 use crate::data_point_provider::writer::Writer;
 use crate::data_point_provider::*;
+use crate::utils;
 use nucliadb_core::metrics;
 use nucliadb_core::metrics::request_time;
 use nucliadb_core::metrics::vectors::MergeSource;
 use nucliadb_core::prelude::*;
 use nucliadb_core::protos::prost::Message;
 use nucliadb_core::protos::resource::ResourceStatus;
 use nucliadb_core::protos::{Resource, ResourceId};
@@ -108,29 +109,34 @@
         debug!("{id:?} - Updating main index");
         let v = time.elapsed().as_millis();
         debug!("{id:?} - Creating elements for the main index: starts {v} ms");
 
         let temporal_mark = SystemTime::now();
         let mut lengths: HashMap<usize, Vec<_>> = HashMap::new();
         let mut elems = Vec::new();
+        let normalize_vectors = self.index.metadata().normalize_vectors;
         if resource.status != ResourceStatus::Delete as i32 {
-            for (paragraph_field, paragraph) in resource.paragraphs.iter() {
-                for index in paragraph.paragraphs.values() {
-                    let mut inner_labels = index.labels.clone();
-                    inner_labels.push(paragraph_field.clone());
+            for (field_id, field_paragraphs) in resource.paragraphs.iter() {
+                for paragraph in field_paragraphs.paragraphs.values() {
+                    let mut inner_labels = paragraph.labels.clone();
+                    inner_labels.push(field_id.clone());
                     let labels = LabelDictionary::new(inner_labels);
 
-                    for (key, sentence) in index.sentences.iter().clone() {
+                    for (key, sentence) in paragraph.sentences.iter().clone() {
                         let key = key.to_string();
                         let labels = labels.clone();
-                        let vector = sentence.vector.clone();
+                        let vector = if normalize_vectors {
+                            utils::normalize_vector(&sentence.vector)
+                        } else {
+                            sentence.vector.clone()
+                        };
                         let metadata = sentence.metadata.as_ref().map(|m| m.encode_to_vec());
                         let bucket = lengths.entry(vector.len()).or_default();
                         elems.push(Elem::new(key, vector, labels, metadata));
-                        bucket.push(paragraph_field);
+                        bucket.push(field_id);
                     }
                 }
             }
         }
         let v = time.elapsed().as_millis();
         debug!("{id:?} - Creating elements for the main index: ends {v} ms");
 
@@ -234,14 +240,15 @@
         } else {
             let Some(similarity) = config.similarity.map(|i| i.into()) else {
                 return Err(node_error!("A similarity must be specified, {:?}", config.similarity));
             };
             let index_metadata = IndexMetadata {
                 similarity,
                 channel: config.channel,
+                normalize_vectors: config.normalize_vectors,
             };
             Ok(VectorWriterService {
                 index: Writer::new(path, index_metadata, config.shard_id.clone())?,
                 config: config.clone(),
             })
         }
     }
@@ -276,14 +283,15 @@
     fn test_new_vector_writer() {
         let dir = TempDir::new().unwrap();
         let vsc = VectorConfig {
             similarity: Some(VectorSimilarity::Cosine),
             path: dir.path().join("vectors"),
             channel: Channel::EXPERIMENTAL,
             shard_id: "abc".into(),
+            normalize_vectors: false,
         };
         let raw_sentences = [
             ("DOC/KEY/1/1".to_string(), vec![1.0, 3.0, 4.0]),
             ("DOC/KEY/1/2".to_string(), vec![2.0, 4.0, 5.0]),
             ("DOC/KEY/1/3".to_string(), vec![3.0, 5.0, 6.0]),
         ];
         let resource_id = ResourceId {
@@ -342,14 +350,15 @@
     fn test_get_segments() {
         let dir = TempDir::new().unwrap();
         let vsc = VectorConfig {
             similarity: Some(VectorSimilarity::Cosine),
             path: dir.path().join("vectors"),
             channel: Channel::EXPERIMENTAL,
             shard_id: "abc".into(),
+            normalize_vectors: false,
         };
         let resource_id = ResourceId {
             shard_id: "DOC".to_string(),
             uuid: "DOC/KEY".to_string(),
         };
 
         let mut sentences = HashMap::new();
```

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_vectors/tests/test_merge.rs` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_vectors/tests/test_merge.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_procs/src/lib.rs` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_procs/src/lib.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_procs/src/measure.rs` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_procs/src/measure.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_procs/tests/dont_compile/actor_defined_twice.rs` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_procs/tests/dont_compile/actor_defined_twice.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_procs/tests/dont_compile/actor_not_defined.rs` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_procs/tests/dont_compile/actor_not_defined.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_procs/tests/dont_compile/metric_defined_twice.rs` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_procs/tests/dont_compile/metric_defined_twice.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_procs/tests/dont_compile/wrong_actor.rs` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_procs/tests/dont_compile/wrong_actor.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_procs/tests/dont_compile/wrong_actor.stderr` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_procs/tests/dont_compile/wrong_actor.stderr`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/local_dependencies/nucliadb_procs/tests/test_measure.rs` & `nucliadb_node_binding-3.0.3.post1164/local_dependencies/nucliadb_procs/tests/test_measure.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/Cargo.toml` & `nucliadb_node_binding-3.0.3.post1164/Cargo.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "nucliadb_node_binding"
-version = "3.0.3-post1160"
+version = "3.0.3-post1164"
 edition = "2021"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 [lib]
 name = "nucliadb_node_binding"
 crate-type = ["cdylib"]
```

### Comparing `nucliadb_node_binding-3.0.3.post1160/CHANGELOG.md` & `nucliadb_node_binding-3.0.3.post1164/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/Makefile` & `nucliadb_node_binding-3.0.3.post1164/Makefile`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/cov.sh` & `nucliadb_node_binding-3.0.3.post1164/cov.sh`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/pyproject.toml` & `nucliadb_node_binding-3.0.3.post1164/pyproject.toml`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/src/collect_garbage.rs` & `nucliadb_node_binding-3.0.3.post1164/src/collect_garbage.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/src/errors.rs` & `nucliadb_node_binding-3.0.3.post1164/src/errors.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/src/lib.rs` & `nucliadb_node_binding-3.0.3.post1164/src/lib.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/src/reader.rs` & `nucliadb_node_binding-3.0.3.post1164/src/reader.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/src/update.rs` & `nucliadb_node_binding-3.0.3.post1164/src/update.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/src/writer.rs` & `nucliadb_node_binding-3.0.3.post1164/src/writer.rs`

 * *Files 1% similar despite different names*

```diff
@@ -99,14 +99,15 @@
         let similarity = VectorSimilarity::from_i32(request.similarity).unwrap();
         let metadata = ShardMetadata::new(
             self.shards_path.join(shard_id.clone()),
             shard_id,
             Some(request.kbid),
             similarity.into(),
             Some(Channel::from(request.release_channel)),
+            request.normalize_vectors,
         );
         let new_shard = self.shards.create(metadata);
         match new_shard {
             Ok(new_shard) => Ok(PyList::new(
                 py,
                 ShardCreated {
                     document_service: new_shard.document_version() as i32,
```

### Comparing `nucliadb_node_binding-3.0.3.post1160/tests/__init__.py` & `nucliadb_node_binding-3.0.3.post1164/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/tests/conftest.py` & `nucliadb_node_binding-3.0.3.post1164/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1160/tests/integration/test_indexing.py` & `nucliadb_node_binding-3.0.3.post1164/tests/integration/test_indexing.py`

 * *Files identical despite different names*

