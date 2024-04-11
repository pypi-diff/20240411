# Comparing `tmp/nucliadb_node_binding-2.46.1.post1112.tar.gz` & `tmp/nucliadb_node_binding-3.0.0.post1133.tar.gz`

## Comparing `nucliadb_node_binding-2.46.1.post1112.tar` & `nucliadb_node_binding-3.0.0.post1133.tar`

### file list

```diff
@@ -1,310 +1,306 @@
--rw-r--r--   0        0        0      628 1970-01-01 00:00:00.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_paragraphs/Cargo.toml
--rw-r--r--   0     1001      127     7796 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_paragraphs/src/fuzzy_query.rs
--rw-r--r--   0     1001      127     1009 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_paragraphs/src/lib.rs
--rw-r--r--   0     1001      127     2780 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_paragraphs/src/query_io.rs
--rw-r--r--   0     1001      127    43068 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_paragraphs/src/reader.rs
--rw-r--r--   0     1001      127     4221 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_paragraphs/src/schema.rs
--rw-r--r--   0     1001      127    21255 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_paragraphs/src/search_query.rs
--rw-r--r--   0     1001      127    11380 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_paragraphs/src/search_response.rs
--rw-r--r--   0     1001      127     4090 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_paragraphs/src/stop_words.rs
--rw-r--r--   0     1001      127    17196 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_paragraphs/src/writer.rs
--rw-r--r--   0     1001      127       88 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_paragraphs/stop_words/README.md
--rw-r--r--   0     1001      127    19791 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_paragraphs/stop_words/ar.json
--rw-r--r--   0     1001      127     1923 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_paragraphs/stop_words/az.json
--rw-r--r--   0     1001      127    11684 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_paragraphs/stop_words/bn.json
--rw-r--r--   0     1001      127     2513 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_paragraphs/stop_words/ca.json
--rw-r--r--   0     1001      127    12802 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_paragraphs/stop_words/ch.json
--rw-r--r--   0     1001      127      730 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_paragraphs/stop_words/da.json
--rw-r--r--   0     1001      127     2090 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_paragraphs/stop_words/de.json
--rw-r--r--   0     1001      127     6284 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_paragraphs/stop_words/el.json
--rw-r--r--   0     1001      127     1473 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_paragraphs/stop_words/en.json
--rw-r--r--   0     1001      127     3451 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_paragraphs/stop_words/es.json
--rw-r--r--   0     1001      127     3182 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_paragraphs/stop_words/eu.json
--rw-r--r--   0     1001      127     2126 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_paragraphs/stop_words/extract.py
--rw-r--r--   0     1001      127     2748 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_paragraphs/stop_words/fi.json
--rw-r--r--   0     1001      127     1388 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_paragraphs/stop_words/fr.json
--rw-r--r--   0     1001      127     5716 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_paragraphs/stop_words/he.json
--rw-r--r--   0     1001      127     2108 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_paragraphs/stop_words/hu.json
--rw-r--r--   0     1001      127     8721 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_paragraphs/stop_words/id.json
--rw-r--r--   0     1001      127     2535 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_paragraphs/stop_words/it.json
--rw-r--r--   0     1001      127    11737 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_paragraphs/stop_words/kk.json
--rw-r--r--   0     1001      127     7730 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_paragraphs/stop_words/ne.json
--rw-r--r--   0     1001      127      756 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_paragraphs/stop_words/nl.json
--rw-r--r--   0     1001      127     1447 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_paragraphs/stop_words/no.json
--rw-r--r--   0     1001      127     2055 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_paragraphs/stop_words/pt.json
--rw-r--r--   0     1001      127     3327 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_paragraphs/stop_words/ro.json
--rw-r--r--   0     1001      127     3856 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_paragraphs/stop_words/ru.json
--rw-r--r--   0     1001      127    23032 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_paragraphs/stop_words/sl.json
--rw-r--r--   0     1001      127      993 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_paragraphs/stop_words/sv.json
--rw-r--r--   0     1001      127     5424 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_paragraphs/stop_words/tg.json
--rw-r--r--   0     1001      127      491 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_paragraphs/stop_words/tr.json
--rw-r--r--   0        0        0      501 1970-01-01 00:00:00.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_protos/Cargo.toml
--rw-r--r--   0     1001      127     2155 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_protos/build.rs
--rw-r--r--   0     1001      127    27030 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_protos/src/fdbwriter.rs
--rw-r--r--   0     1001      127        0 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_protos/src/google.protobuf.rs
--rw-r--r--   0     1001      127     9078 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_protos/src/knowledgebox.rs
--rw-r--r--   0     1001      127     1256 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_protos/src/lib.rs
--rw-r--r--   0     1001      127    77192 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_protos/src/nodereader.rs
--rw-r--r--   0     1001      127    10215 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_protos/src/noderesources.rs
--rw-r--r--   0     1001      127    43211 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_protos/src/nodewriter.rs
--rw-r--r--   0     1001      127    18949 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_protos/src/replication.rs
--rw-r--r--   0     1001      127    32797 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_protos/src/resources.rs
--rw-r--r--   0     1001      127     5528 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_protos/src/utils.rs
--rw-r--r--   0        0        0      838 1970-01-01 00:00:00.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_relations/Cargo.toml
--rw-r--r--   0     1001      127     9354 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_relations/src/bfs_engine.rs
--rw-r--r--   0     1001      127     1761 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_relations/src/errors.rs
--rw-r--r--   0     1001      127    21119 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_relations/src/graph_db.rs
--rw-r--r--   0     1001      127     1784 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_relations/src/graph_test_utils.rs
--rw-r--r--   0     1001      127    10531 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_relations/src/index.rs
--rw-r--r--   0     1001      127     1003 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_relations/src/lib.rs
--rw-r--r--   0     1001      127     5550 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_relations/src/node_dictionary.rs
--rw-r--r--   0     1001      127     5249 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_relations/src/relations_io.rs
--rw-r--r--   0     1001      127     2658 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_relations/src/service/bfs.rs
--rw-r--r--   0     1001      127      970 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_relations/src/service/mod.rs
--rw-r--r--   0     1001      127     9828 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_relations/src/service/reader.rs
--rw-r--r--   0     1001      127    10781 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_relations/src/service/tests.rs
--rw-r--r--   0     1001      127     3071 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_relations/src/service/utils.rs
--rw-r--r--   0     1001      127     7110 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_relations/src/service/writer.rs
--rw-r--r--   0        0        0      361 1970-01-01 00:00:00.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_procs/Cargo.toml
--rw-r--r--   0     1001      127     3409 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_procs/src/lib.rs
--rw-r--r--   0     1001      127     2885 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_procs/src/measure.rs
--rw-r--r--   0     1001      127     1081 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_procs/tests/dont_compile/actor_defined_twice.rs
--rw-r--r--   0     1001      127      222 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_procs/tests/dont_compile/actor_defined_twice.stderr
--rw-r--r--   0     1001      127     1038 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_procs/tests/dont_compile/actor_not_defined.rs
--rw-r--r--   0     1001      127      327 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_procs/tests/dont_compile/actor_not_defined.stderr
--rw-r--r--   0     1001      127     1086 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_procs/tests/dont_compile/metric_defined_twice.rs
--rw-r--r--   0     1001      127      249 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_procs/tests/dont_compile/metric_defined_twice.stderr
--rw-r--r--   0     1001      127     1046 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_procs/tests/dont_compile/wrong_actor.rs
--rw-r--r--   0     1001      127     1303 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_procs/tests/dont_compile/wrong_actor.stderr
--rw-r--r--   0     1001      127     1408 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_procs/tests/test_measure.rs
--rw-r--r--   0        0        0      629 1970-01-01 00:00:00.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_paragraphs2/Cargo.toml
--rw-r--r--   0     1001      127     7796 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_paragraphs2/src/fuzzy_query.rs
--rw-r--r--   0     1001      127     1009 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_paragraphs2/src/lib.rs
--rw-r--r--   0     1001      127     2780 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_paragraphs2/src/query_io.rs
--rw-r--r--   0     1001      127    43068 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_paragraphs2/src/reader.rs
--rw-r--r--   0     1001      127     4808 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_paragraphs2/src/schema.rs
--rw-r--r--   0     1001      127    22494 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_paragraphs2/src/search_query.rs
--rw-r--r--   0     1001      127    11380 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_paragraphs2/src/search_response.rs
--rw-r--r--   0     1001      127     4090 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_paragraphs2/src/stop_words.rs
--rw-r--r--   0     1001      127    18507 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_paragraphs2/src/writer.rs
--rw-r--r--   0     1001      127       88 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_paragraphs2/stop_words/README.md
--rw-r--r--   0     1001      127    19791 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_paragraphs2/stop_words/ar.json
--rw-r--r--   0     1001      127     1923 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_paragraphs2/stop_words/az.json
--rw-r--r--   0     1001      127    11684 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_paragraphs2/stop_words/bn.json
--rw-r--r--   0     1001      127     2513 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_paragraphs2/stop_words/ca.json
--rw-r--r--   0     1001      127    12802 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_paragraphs2/stop_words/ch.json
--rw-r--r--   0     1001      127      730 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_paragraphs2/stop_words/da.json
--rw-r--r--   0     1001      127     2090 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_paragraphs2/stop_words/de.json
--rw-r--r--   0     1001      127     6284 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_paragraphs2/stop_words/el.json
--rw-r--r--   0     1001      127     1473 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_paragraphs2/stop_words/en.json
--rw-r--r--   0     1001      127     3451 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_paragraphs2/stop_words/es.json
--rw-r--r--   0     1001      127     3182 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_paragraphs2/stop_words/eu.json
--rw-r--r--   0     1001      127     2126 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_paragraphs2/stop_words/extract.py
--rw-r--r--   0     1001      127     2748 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_paragraphs2/stop_words/fi.json
--rw-r--r--   0     1001      127     1388 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_paragraphs2/stop_words/fr.json
--rw-r--r--   0     1001      127     5716 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_paragraphs2/stop_words/he.json
--rw-r--r--   0     1001      127     2108 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_paragraphs2/stop_words/hu.json
--rw-r--r--   0     1001      127     8721 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_paragraphs2/stop_words/id.json
--rw-r--r--   0     1001      127     2535 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_paragraphs2/stop_words/it.json
--rw-r--r--   0     1001      127    11737 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_paragraphs2/stop_words/kk.json
--rw-r--r--   0     1001      127     7730 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_paragraphs2/stop_words/ne.json
--rw-r--r--   0     1001      127      756 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_paragraphs2/stop_words/nl.json
--rw-r--r--   0     1001      127     1447 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_paragraphs2/stop_words/no.json
--rw-r--r--   0     1001      127     2055 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_paragraphs2/stop_words/pt.json
--rw-r--r--   0     1001      127     3327 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_paragraphs2/stop_words/ro.json
--rw-r--r--   0     1001      127     3856 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_paragraphs2/stop_words/ru.json
--rw-r--r--   0     1001      127    23032 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_paragraphs2/stop_words/sl.json
--rw-r--r--   0     1001      127      993 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_paragraphs2/stop_words/sv.json
--rw-r--r--   0     1001      127     5424 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_paragraphs2/stop_words/tg.json
--rw-r--r--   0     1001      127      491 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_paragraphs2/stop_words/tr.json
--rw-r--r--   0        0        0      708 1970-01-01 00:00:00.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_relations2/Cargo.toml
--rw-r--r--   0     1001      127     3593 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_relations2/src/io_maps.rs
--rw-r--r--   0     1001      127      916 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_relations2/src/lib.rs
--rw-r--r--   0     1001      127    17053 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_relations2/src/reader.rs
--rw-r--r--   0     1001      127     7123 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_relations2/src/schema.rs
--rw-r--r--   0     1001      127     8279 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_relations2/src/writer.rs
--rw-r--r--   0     1001      127     1802 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_relations2/tests/common/mod.rs
--rw-r--r--   0     1001      127     9435 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_relations2/tests/test_reader.rs
--rw-r--r--   0     1001      127     3296 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_relations2/tests/test_writer.rs
--rw-r--r--   0        0        0      931 1970-01-01 00:00:00.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_core/Cargo.toml
--rw-r--r--   0     1001      127     5872 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_core/src/fs_state.rs
--rw-r--r--   0     1001      127     2681 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_core/src/lib.rs
--rw-r--r--   0     1001      127     2295 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_core/src/merge.rs
--rw-r--r--   0     1001      127      906 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_core/src/metrics/meters/mod.rs
--rw-r--r--   0     1001      127     4869 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_core/src/metrics/meters/prometheus.rs
--rw-r--r--   0     1001      127     1702 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_core/src/metrics/metric/grpc_ops.rs
--rw-r--r--   0     1001      127     1442 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_core/src/metrics/metric/mod.rs
--rw-r--r--   0     1001      127     1950 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_core/src/metrics/metric/replication.rs
--rw-r--r--   0     1001      127     2626 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_core/src/metrics/metric/request_time.rs
--rw-r--r--   0     1001      127     1644 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_core/src/metrics/metric/shard_cache.rs
--rw-r--r--   0     1001      127    21641 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_core/src/metrics/metric/tokio_runtime.rs
--rw-r--r--   0     1001      127    16736 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_core/src/metrics/metric/tokio_tasks.rs
--rw-r--r--   0     1001      127     3415 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_core/src/metrics/metric/vectors.rs
--rw-r--r--   0     1001      127     1324 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_core/src/metrics/mod.rs
--rw-r--r--   0     1001      127     3074 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_core/src/metrics/task_monitor.rs
--rw-r--r--   0     1001      127     3920 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_core/src/metrics/tests.rs
--rw-r--r--   0     1001      127     2990 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_core/src/paragraphs.rs
--rw-r--r--   0     1001      127    17305 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_core/src/query_language/mod.rs
--rw-r--r--   0     1001      127    15365 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_core/src/query_planner.rs
--rw-r--r--   0     1001      127     2069 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_core/src/relations.rs
--rw-r--r--   0     1001      127     8399 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_core/src/tantivy_replica.rs
--rw-r--r--   0     1001      127     2603 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_core/src/texts.rs
--rw-r--r--   0     1001      127     3806 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_core/src/vectors.rs
--rw-r--r--   0        0        0      398 1970-01-01 00:00:00.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_texts/Cargo.toml
--rw-r--r--   0     1001      127      931 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_texts/src/lib.rs
--rw-r--r--   0     1001      127     2755 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_texts/src/query_io.rs
--rw-r--r--   0     1001      127    21119 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_texts/src/reader.rs
--rw-r--r--   0     1001      127     2761 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_texts/src/schema.rs
--rw-r--r--   0     1001      127     8676 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_texts/src/search_query.rs
--rw-r--r--   0     1001      127     9257 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_texts/src/writer.rs
--rw-r--r--   0     1001      127     3389 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_texts/tests/common/mod.rs
--rw-r--r--   0     1001      127     2044 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_texts/tests/test_reader.rs
--rw-r--r--   0     1001      127     8063 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_texts/tests/test_search.rs
--rw-r--r--   0     1001      127     1249 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_texts/tests/test_streaming.rs
--rw-r--r--   0     1001      127     3458 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_texts/tests/test_writer.rs
--rw-r--r--   0        0        0      703 1970-01-01 00:00:00.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_vectors/Cargo.toml
--rw-r--r--   0     1001      127       69 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_vectors/README.md
--rw-r--r--   0     1001      127       43 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_vectors/docs/README.md
--rw-r--r--   0     1001      127    25718 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_vectors/docs/labels.drawio.svg
--rw-r--r--   0     1001      127    12250 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_vectors/src/data_point/disk_hnsw.rs
--rw-r--r--   0     1001      127    19361 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_vectors/src/data_point/mod.rs
--rw-r--r--   0     1001      127    11214 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_vectors/src/data_point/node.rs
--rw-r--r--   0     1001      127    12611 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_vectors/src/data_point/ops_hnsw.rs
--rw-r--r--   0     1001      127     1405 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_vectors/src/data_point/params.rs
--rw-r--r--   0     1001      127     3952 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_vectors/src/data_point/ram_hnsw.rs
--rw-r--r--   0     1001      127    11778 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_vectors/src/data_point/tests.rs
--rw-r--r--   0     1001      127     5798 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_vectors/src/data_point_provider/garbage_collector.rs
--rw-r--r--   0     1001      127     2722 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_vectors/src/data_point_provider/mod.rs
--rw-r--r--   0     1001      127    10271 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_vectors/src/data_point_provider/reader.rs
--rw-r--r--   0     1001      127     2304 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_vectors/src/data_point_provider/replication.rs
--rw-r--r--   0     1001      127     5288 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_vectors/src/data_point_provider/state.rs
--rw-r--r--   0     1001      127    20587 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_vectors/src/data_point_provider/writer.rs
--rw-r--r--   0     1001      127    22479 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_vectors/src/data_types/data_store.rs
--rw-r--r--   0     1001      127     6916 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_vectors/src/data_types/dtrie_ram.rs
--rw-r--r--   0     1001      127     1959 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_vectors/src/data_types/mod.rs
--rw-r--r--   0     1001      127     6143 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_vectors/src/data_types/trie.rs
--rw-r--r--   0     1001      127     2904 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_vectors/src/data_types/trie_ram.rs
--rw-r--r--   0     1001      127     4433 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_vectors/src/data_types/vector.rs
--rw-r--r--   0     1001      127     8043 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_vectors/src/formula/mod.rs
--rw-r--r--   0     1001      127     4762 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_vectors/src/indexset/mod.rs
--rw-r--r--   0     1001      127     1087 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_vectors/src/indexset/state.rs
--rw-r--r--   0     1001      127     2172 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_vectors/src/lib.rs
--rw-r--r--   0     1001      127     1278 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_vectors/src/service/mod.rs
--rw-r--r--   0     1001      127     1897 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_vectors/src/service/query_io.rs
--rw-r--r--   0     1001      127    18388 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_vectors/src/service/reader.rs
--rw-r--r--   0     1001      127    24262 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_vectors/src/service/writer.rs
--rw-r--r--   0     1001      127     2884 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_vectors/tests/test_merge.rs
--rw-r--r--   0        0        0     3314 1970-01-01 00:00:00.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_node/Cargo.toml
--rw-r--r--   0     1001      127     1045 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_node/.rustc_info.json
--rw-r--r--   0     1001      127      877 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_node/Makefile
--rw-r--r--   0     1001      127     1500 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_node/README.md
--rw-r--r--   0     1001      127     1757 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_node/nucliadb_node/__init__.py
--rw-r--r--   0     1001      127     4192 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_node/nucliadb_node/app.py
--rw-r--r--   0     1001      127    17752 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_node/nucliadb_node/indexer.py
--rw-r--r--   0     1001      127      941 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_node/nucliadb_node/listeners/__init__.py
--rw-r--r--   0     1001      127     6724 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_node/nucliadb_node/listeners/gc_scheduler.py
--rw-r--r--   0     1001      127     2424 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_node/nucliadb_node/listeners/indexed_publisher.py
--rw-r--r--   0     1001      127     4015 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_node/nucliadb_node/pull.py
--rw-r--r--   0     1001      127     1535 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_node/nucliadb_node/service.py
--rw-r--r--   0     1001      127     1487 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_node/nucliadb_node/settings.py
--rw-r--r--   0     1001      127     1133 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_node/nucliadb_node/signals.py
--rw-r--r--   0     1001      127      835 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_node/nucliadb_node/tests/__init__.py
--rw-r--r--   0     1001      127     1092 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_node/nucliadb_node/tests/conftest.py
--rw-r--r--   0     1001      127    10810 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_node/nucliadb_node/tests/fixtures.py
--rw-r--r--   0     1001      127    13788 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_node/nucliadb_node/tests/integration/test_indexing.py
--rw-r--r--   0     1001      127     2461 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_node/nucliadb_node/tests/unit/test_app.py
--rw-r--r--   0     1001      127     4963 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_node/nucliadb_node/tests/unit/test_gc_scheduler.py
--rw-r--r--   0     1001      127     2361 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_node/nucliadb_node/tests/unit/test_indexed_publisher.py
--rw-r--r--   0     1001      127    12553 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_node/nucliadb_node/tests/unit/test_indexer.py
--rw-r--r--   0     1001      127     4989 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_node/nucliadb_node/tests/unit/test_pull.py
--rw-r--r--   0     1001      127     2323 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_node/nucliadb_node/writer.py
--rw-r--r--   0     1001      127      101 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_node/requirements-sources.txt
--rw-r--r--   0     1001      127      276 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_node/requirements.txt
--rw-r--r--   0     1001      127      249 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_node/setup.cfg
--rw-r--r--   0     1001      127     1405 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_node/setup.py
--rw-r--r--   0     1001      127     2518 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_node/src/analytics/blocking.rs
--rw-r--r--   0     1001      127     1219 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_node/src/analytics/mod.rs
--rw-r--r--   0     1001      127     4931 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_node/src/analytics/payload.rs
--rw-r--r--   0     1001      127    12828 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_node/src/analytics/sender.rs
--rw-r--r--   0     1001      127     3085 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_node/src/analytics/sink.rs
--rw-r--r--   0     1001      127     1900 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_node/src/analytics/sync.rs
--rw-r--r--   0     1001      127     4935 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_node/src/bin/reader.rs
--rw-r--r--   0     1001      127     8050 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_node/src/bin/writer.rs
--rw-r--r--   0     1001      127     1345 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_node/src/cache/mod.rs
--rw-r--r--   0     1001      127     3043 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_node/src/cache/reader_cache.rs
--rw-r--r--   0     1001      127    14199 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_node/src/cache/resource_cache.rs
--rw-r--r--   0     1001      127    10999 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_node/src/cache/writer_cache.rs
--rw-r--r--   0     1001      127     1816 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_node/src/disk_structure.rs
--rw-r--r--   0     1001      127     2558 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_node/src/grpc/collect_garbage.rs
--rw-r--r--   0     1001      127    18829 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_node/src/grpc/grpc_reader.rs
--rw-r--r--   0     1001      127    17029 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_node/src/grpc/grpc_writer.rs
--rw-r--r--   0     1001      127     3186 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_node/src/grpc/middleware/debug.rs
--rw-r--r--   0     1001      127     3440 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_node/src/grpc/middleware/metrics.rs
--rw-r--r--   0     1001      127     1009 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_node/src/grpc/middleware/mod.rs
--rw-r--r--   0     1001      127     4158 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_node/src/grpc/middleware/telemetry.rs
--rw-r--r--   0     1001      127     1283 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_node/src/grpc/mod.rs
--rw-r--r--   0     1001      127     2482 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_node/src/grpc/update.rs
--rw-r--r--   0     1001      127     1173 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_node/src/http_server/metrics_service.rs
--rw-r--r--   0     1001      127     1465 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_node/src/http_server/mod.rs
--rw-r--r--   0     1001      127     1943 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_node/src/http_server/traces_service.rs
--rw-r--r--   0     1001      127     1488 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_node/src/lib.rs
--rw-r--r--   0     1001      127     2757 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_node/src/lifecycle.rs
--rw-r--r--   0     1001      127     1778 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_node/src/merge/global.rs
--rw-r--r--   0     1001      127     1089 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_node/src/merge/mod.rs
--rw-r--r--   0     1001      127    13672 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_node/src/merge/scheduler.rs
--rw-r--r--   0     1001      127     3677 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_node/src/merge/work.rs
--rw-r--r--   0     1001      127     1935 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_node/src/node_metadata.rs
--rw-r--r--   0     1001      127     2417 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_node/src/replication/health.rs
--rw-r--r--   0     1001      127     1070 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_node/src/replication/mod.rs
--rw-r--r--   0     1001      127    14052 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_node/src/replication/replicator.rs
--rw-r--r--   0     1001      127    11682 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_node/src/replication/service.rs
--rw-r--r--   0     1001      127    11231 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_node/src/settings.rs
--rw-r--r--   0     1001      127     1111 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_node/src/shards/errors.rs
--rw-r--r--   0     1001      127    10834 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_node/src/shards/metadata.rs
--rw-r--r--   0     1001      127     1122 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_node/src/shards/mod.rs
--rw-r--r--   0     1001      127    24437 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_node/src/shards/shard_reader.rs
--rw-r--r--   0     1001      127    20462 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_node/src/shards/shard_writer.rs
--rw-r--r--   0     1001      127    10251 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_node/src/shards/versions.rs
--rw-r--r--   0     1001      127    10170 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_node/src/telemetry.rs
--rw-r--r--   0     1001      127     6396 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_node/src/utils.rs
--rw-r--r--   0     1001      127       42 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_node/test.sh
--rw-r--r--   0     1001      127     1115 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_node/tests/common/mod.rs
--rw-r--r--   0     1001      127    12731 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_node/tests/common/node_services.rs
--rw-r--r--   0     1001      127     7823 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_node/tests/common/resources.rs
--rw-r--r--   0     1001      127     8173 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_node/tests/test_date_range_search.rs
--rw-r--r--   0     1001      127     4089 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_node/tests/test_download.rs
--rw-r--r--   0     1001      127     1684 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_node/tests/test_merge.rs
--rw-r--r--   0     1001      127     7024 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_node/tests/test_replication.rs
--rw-r--r--   0     1001      127    22494 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_node/tests/test_search_relations.rs
--rw-r--r--   0     1001      127     6958 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_node/tests/test_search_sorting.rs
--rw-r--r--   0     1001      127     7044 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_node/tests/test_security_search.rs
--rw-r--r--   0     1001      127     6862 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_node/tests/test_shards.rs
--rw-r--r--   0     1001      127    10698 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_node/tests/test_suggest.rs
--rw-r--r--   0        0        0      399 1970-01-01 00:00:00.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_texts2/Cargo.toml
--rw-r--r--   0     1001      127      931 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_texts2/src/lib.rs
--rw-r--r--   0     1001      127     2755 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_texts2/src/query_io.rs
--rw-r--r--   0     1001      127    22604 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_texts2/src/reader.rs
--rw-r--r--   0     1001      127     3105 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_texts2/src/schema.rs
--rw-r--r--   0     1001      127     8682 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_texts2/src/search_query.rs
--rw-r--r--   0     1001      127    10377 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_texts2/src/writer.rs
--rw-r--r--   0     1001      127     3391 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_texts2/tests/common/mod.rs
--rw-r--r--   0     1001      127     2046 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_texts2/tests/test_reader.rs
--rw-r--r--   0     1001      127     8881 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_texts2/tests/test_search.rs
--rw-r--r--   0     1001      127     1249 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_texts2/tests/test_streaming.rs
--rw-r--r--   0     1001      127     3460 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_texts2/tests/test_writer.rs
--rw-r--r--   0        0        0      944 1970-01-01 00:00:00.000000 nucliadb_node_binding-2.46.1.post1112/Cargo.toml
--rw-r--r--   0     1001      127     1553 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/CHANGELOG.md
--rw-r--r--   0     1001      127      895 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/Makefile
--rw-r--r--   0     1001      127       52 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/README.md
--rwxr-xr-x   0     1001      127      978 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/cov.sh
--rw-r--r--   0     1001      127     1309 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/pyproject.toml
--rw-r--r--   0     1001      127     2195 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/src/collect_garbage.rs
--rw-r--r--   0     1001      127     1212 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/src/errors.rs
--rw-r--r--   0     1001      127     2337 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/src/lib.rs
--rw-r--r--   0     1001      127     9413 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/src/reader.rs
--rw-r--r--   0     1001      127     2154 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/src/update.rs
--rw-r--r--   0     1001      127    11920 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/src/writer.rs
--rw-r--r--   0     1001      127      835 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/tests/__init__.py
--rw-r--r--   0     1001      127      892 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/tests/conftest.py
--rw-r--r--   0     1001      127     3903 2024-04-08 09:53:14.000000 nucliadb_node_binding-2.46.1.post1112/tests/integration/test_indexing.py
--rw-r--r--   0        0        0      402 1970-01-01 00:00:00.000000 nucliadb_node_binding-2.46.1.post1112/PKG-INFO
+-rw-r--r--   0        0        0      501 1970-01-01 00:00:00.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_protos/Cargo.toml
+-rw-r--r--   0     1001      127     2155 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_protos/build.rs
+-rw-r--r--   0     1001      127    27030 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_protos/src/fdbwriter.rs
+-rw-r--r--   0     1001      127        0 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_protos/src/google.protobuf.rs
+-rw-r--r--   0     1001      127     9078 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_protos/src/knowledgebox.rs
+-rw-r--r--   0     1001      127     1256 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_protos/src/lib.rs
+-rw-r--r--   0     1001      127    77192 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_protos/src/nodereader.rs
+-rw-r--r--   0     1001      127    10215 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_protos/src/noderesources.rs
+-rw-r--r--   0     1001      127    43211 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_protos/src/nodewriter.rs
+-rw-r--r--   0     1001      127    18949 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_protos/src/replication.rs
+-rw-r--r--   0     1001      127    32797 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_protos/src/resources.rs
+-rw-r--r--   0     1001      127     5528 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_protos/src/utils.rs
+-rw-r--r--   0        0        0      931 1970-01-01 00:00:00.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_core/Cargo.toml
+-rw-r--r--   0     1001      127     5872 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_core/src/fs_state.rs
+-rw-r--r--   0     1001      127     2681 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_core/src/lib.rs
+-rw-r--r--   0     1001      127     2295 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_core/src/merge.rs
+-rw-r--r--   0     1001      127      906 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_core/src/metrics/meters/mod.rs
+-rw-r--r--   0     1001      127     4869 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_core/src/metrics/meters/prometheus.rs
+-rw-r--r--   0     1001      127     1702 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_core/src/metrics/metric/grpc_ops.rs
+-rw-r--r--   0     1001      127     1442 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_core/src/metrics/metric/mod.rs
+-rw-r--r--   0     1001      127     1950 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_core/src/metrics/metric/replication.rs
+-rw-r--r--   0     1001      127     2626 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_core/src/metrics/metric/request_time.rs
+-rw-r--r--   0     1001      127     1644 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_core/src/metrics/metric/shard_cache.rs
+-rw-r--r--   0     1001      127    21641 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_core/src/metrics/metric/tokio_runtime.rs
+-rw-r--r--   0     1001      127    16736 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_core/src/metrics/metric/tokio_tasks.rs
+-rw-r--r--   0     1001      127     3415 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_core/src/metrics/metric/vectors.rs
+-rw-r--r--   0     1001      127     1324 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_core/src/metrics/mod.rs
+-rw-r--r--   0     1001      127     3074 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_core/src/metrics/task_monitor.rs
+-rw-r--r--   0     1001      127     3920 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_core/src/metrics/tests.rs
+-rw-r--r--   0     1001      127     2990 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_core/src/paragraphs.rs
+-rw-r--r--   0     1001      127    17305 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_core/src/query_language/mod.rs
+-rw-r--r--   0     1001      127    15365 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_core/src/query_planner.rs
+-rw-r--r--   0     1001      127     2069 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_core/src/relations.rs
+-rw-r--r--   0     1001      127     8399 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_core/src/tantivy_replica.rs
+-rw-r--r--   0     1001      127     2603 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_core/src/texts.rs
+-rw-r--r--   0     1001      127     3526 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_core/src/vectors.rs
+-rw-r--r--   0        0        0      708 1970-01-01 00:00:00.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_relations2/Cargo.toml
+-rw-r--r--   0     1001      127     3593 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_relations2/src/io_maps.rs
+-rw-r--r--   0     1001      127      916 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_relations2/src/lib.rs
+-rw-r--r--   0     1001      127    17053 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_relations2/src/reader.rs
+-rw-r--r--   0     1001      127     7123 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_relations2/src/schema.rs
+-rw-r--r--   0     1001      127     8279 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_relations2/src/writer.rs
+-rw-r--r--   0     1001      127     1802 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_relations2/tests/common/mod.rs
+-rw-r--r--   0     1001      127     9435 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_relations2/tests/test_reader.rs
+-rw-r--r--   0     1001      127     3296 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_relations2/tests/test_writer.rs
+-rw-r--r--   0        0        0      398 1970-01-01 00:00:00.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_texts/Cargo.toml
+-rw-r--r--   0     1001      127      931 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_texts/src/lib.rs
+-rw-r--r--   0     1001      127     2755 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_texts/src/query_io.rs
+-rw-r--r--   0     1001      127    21119 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_texts/src/reader.rs
+-rw-r--r--   0     1001      127     2761 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_texts/src/schema.rs
+-rw-r--r--   0     1001      127     8676 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_texts/src/search_query.rs
+-rw-r--r--   0     1001      127     9257 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_texts/src/writer.rs
+-rw-r--r--   0     1001      127     3389 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_texts/tests/common/mod.rs
+-rw-r--r--   0     1001      127     2044 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_texts/tests/test_reader.rs
+-rw-r--r--   0     1001      127     8063 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_texts/tests/test_search.rs
+-rw-r--r--   0     1001      127     1249 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_texts/tests/test_streaming.rs
+-rw-r--r--   0     1001      127     3458 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_texts/tests/test_writer.rs
+-rw-r--r--   0        0        0      629 1970-01-01 00:00:00.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_paragraphs2/Cargo.toml
+-rw-r--r--   0     1001      127     7796 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_paragraphs2/src/fuzzy_query.rs
+-rw-r--r--   0     1001      127     1009 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_paragraphs2/src/lib.rs
+-rw-r--r--   0     1001      127     2780 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_paragraphs2/src/query_io.rs
+-rw-r--r--   0     1001      127    43068 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_paragraphs2/src/reader.rs
+-rw-r--r--   0     1001      127     4808 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_paragraphs2/src/schema.rs
+-rw-r--r--   0     1001      127    22494 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_paragraphs2/src/search_query.rs
+-rw-r--r--   0     1001      127    11380 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_paragraphs2/src/search_response.rs
+-rw-r--r--   0     1001      127     4090 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_paragraphs2/src/stop_words.rs
+-rw-r--r--   0     1001      127    18507 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_paragraphs2/src/writer.rs
+-rw-r--r--   0     1001      127       88 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_paragraphs2/stop_words/README.md
+-rw-r--r--   0     1001      127    19791 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_paragraphs2/stop_words/ar.json
+-rw-r--r--   0     1001      127     1923 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_paragraphs2/stop_words/az.json
+-rw-r--r--   0     1001      127    11684 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_paragraphs2/stop_words/bn.json
+-rw-r--r--   0     1001      127     2513 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_paragraphs2/stop_words/ca.json
+-rw-r--r--   0     1001      127    12802 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_paragraphs2/stop_words/ch.json
+-rw-r--r--   0     1001      127      730 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_paragraphs2/stop_words/da.json
+-rw-r--r--   0     1001      127     2090 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_paragraphs2/stop_words/de.json
+-rw-r--r--   0     1001      127     6284 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_paragraphs2/stop_words/el.json
+-rw-r--r--   0     1001      127     1473 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_paragraphs2/stop_words/en.json
+-rw-r--r--   0     1001      127     3451 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_paragraphs2/stop_words/es.json
+-rw-r--r--   0     1001      127     3182 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_paragraphs2/stop_words/eu.json
+-rw-r--r--   0     1001      127     2126 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_paragraphs2/stop_words/extract.py
+-rw-r--r--   0     1001      127     2748 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_paragraphs2/stop_words/fi.json
+-rw-r--r--   0     1001      127     1388 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_paragraphs2/stop_words/fr.json
+-rw-r--r--   0     1001      127     5716 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_paragraphs2/stop_words/he.json
+-rw-r--r--   0     1001      127     2108 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_paragraphs2/stop_words/hu.json
+-rw-r--r--   0     1001      127     8721 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_paragraphs2/stop_words/id.json
+-rw-r--r--   0     1001      127     2535 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_paragraphs2/stop_words/it.json
+-rw-r--r--   0     1001      127    11737 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_paragraphs2/stop_words/kk.json
+-rw-r--r--   0     1001      127     7730 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_paragraphs2/stop_words/ne.json
+-rw-r--r--   0     1001      127      756 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_paragraphs2/stop_words/nl.json
+-rw-r--r--   0     1001      127     1447 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_paragraphs2/stop_words/no.json
+-rw-r--r--   0     1001      127     2055 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_paragraphs2/stop_words/pt.json
+-rw-r--r--   0     1001      127     3327 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_paragraphs2/stop_words/ro.json
+-rw-r--r--   0     1001      127     3856 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_paragraphs2/stop_words/ru.json
+-rw-r--r--   0     1001      127    23032 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_paragraphs2/stop_words/sl.json
+-rw-r--r--   0     1001      127      993 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_paragraphs2/stop_words/sv.json
+-rw-r--r--   0     1001      127     5424 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_paragraphs2/stop_words/tg.json
+-rw-r--r--   0     1001      127      491 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_paragraphs2/stop_words/tr.json
+-rw-r--r--   0        0        0      361 1970-01-01 00:00:00.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_procs/Cargo.toml
+-rw-r--r--   0     1001      127     3409 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_procs/src/lib.rs
+-rw-r--r--   0     1001      127     2885 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_procs/src/measure.rs
+-rw-r--r--   0     1001      127     1081 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_procs/tests/dont_compile/actor_defined_twice.rs
+-rw-r--r--   0     1001      127      222 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_procs/tests/dont_compile/actor_defined_twice.stderr
+-rw-r--r--   0     1001      127     1038 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_procs/tests/dont_compile/actor_not_defined.rs
+-rw-r--r--   0     1001      127      327 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_procs/tests/dont_compile/actor_not_defined.stderr
+-rw-r--r--   0     1001      127     1086 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_procs/tests/dont_compile/metric_defined_twice.rs
+-rw-r--r--   0     1001      127      249 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_procs/tests/dont_compile/metric_defined_twice.stderr
+-rw-r--r--   0     1001      127     1046 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_procs/tests/dont_compile/wrong_actor.rs
+-rw-r--r--   0     1001      127     1303 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_procs/tests/dont_compile/wrong_actor.stderr
+-rw-r--r--   0     1001      127     1408 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_procs/tests/test_measure.rs
+-rw-r--r--   0        0        0      628 1970-01-01 00:00:00.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_paragraphs/Cargo.toml
+-rw-r--r--   0     1001      127     7796 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_paragraphs/src/fuzzy_query.rs
+-rw-r--r--   0     1001      127     1009 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_paragraphs/src/lib.rs
+-rw-r--r--   0     1001      127     2780 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_paragraphs/src/query_io.rs
+-rw-r--r--   0     1001      127    43068 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_paragraphs/src/reader.rs
+-rw-r--r--   0     1001      127     4221 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_paragraphs/src/schema.rs
+-rw-r--r--   0     1001      127    21255 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_paragraphs/src/search_query.rs
+-rw-r--r--   0     1001      127    11380 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_paragraphs/src/search_response.rs
+-rw-r--r--   0     1001      127     4090 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_paragraphs/src/stop_words.rs
+-rw-r--r--   0     1001      127    17196 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_paragraphs/src/writer.rs
+-rw-r--r--   0     1001      127       88 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_paragraphs/stop_words/README.md
+-rw-r--r--   0     1001      127    19791 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_paragraphs/stop_words/ar.json
+-rw-r--r--   0     1001      127     1923 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_paragraphs/stop_words/az.json
+-rw-r--r--   0     1001      127    11684 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_paragraphs/stop_words/bn.json
+-rw-r--r--   0     1001      127     2513 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_paragraphs/stop_words/ca.json
+-rw-r--r--   0     1001      127    12802 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_paragraphs/stop_words/ch.json
+-rw-r--r--   0     1001      127      730 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_paragraphs/stop_words/da.json
+-rw-r--r--   0     1001      127     2090 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_paragraphs/stop_words/de.json
+-rw-r--r--   0     1001      127     6284 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_paragraphs/stop_words/el.json
+-rw-r--r--   0     1001      127     1473 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_paragraphs/stop_words/en.json
+-rw-r--r--   0     1001      127     3451 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_paragraphs/stop_words/es.json
+-rw-r--r--   0     1001      127     3182 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_paragraphs/stop_words/eu.json
+-rw-r--r--   0     1001      127     2126 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_paragraphs/stop_words/extract.py
+-rw-r--r--   0     1001      127     2748 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_paragraphs/stop_words/fi.json
+-rw-r--r--   0     1001      127     1388 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_paragraphs/stop_words/fr.json
+-rw-r--r--   0     1001      127     5716 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_paragraphs/stop_words/he.json
+-rw-r--r--   0     1001      127     2108 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_paragraphs/stop_words/hu.json
+-rw-r--r--   0     1001      127     8721 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_paragraphs/stop_words/id.json
+-rw-r--r--   0     1001      127     2535 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_paragraphs/stop_words/it.json
+-rw-r--r--   0     1001      127    11737 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_paragraphs/stop_words/kk.json
+-rw-r--r--   0     1001      127     7730 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_paragraphs/stop_words/ne.json
+-rw-r--r--   0     1001      127      756 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_paragraphs/stop_words/nl.json
+-rw-r--r--   0     1001      127     1447 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_paragraphs/stop_words/no.json
+-rw-r--r--   0     1001      127     2055 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_paragraphs/stop_words/pt.json
+-rw-r--r--   0     1001      127     3327 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_paragraphs/stop_words/ro.json
+-rw-r--r--   0     1001      127     3856 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_paragraphs/stop_words/ru.json
+-rw-r--r--   0     1001      127    23032 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_paragraphs/stop_words/sl.json
+-rw-r--r--   0     1001      127      993 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_paragraphs/stop_words/sv.json
+-rw-r--r--   0     1001      127     5424 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_paragraphs/stop_words/tg.json
+-rw-r--r--   0     1001      127      491 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_paragraphs/stop_words/tr.json
+-rw-r--r--   0        0        0      838 1970-01-01 00:00:00.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_relations/Cargo.toml
+-rw-r--r--   0     1001      127     9354 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_relations/src/bfs_engine.rs
+-rw-r--r--   0     1001      127     1761 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_relations/src/errors.rs
+-rw-r--r--   0     1001      127    21119 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_relations/src/graph_db.rs
+-rw-r--r--   0     1001      127     1784 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_relations/src/graph_test_utils.rs
+-rw-r--r--   0     1001      127    10531 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_relations/src/index.rs
+-rw-r--r--   0     1001      127     1003 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_relations/src/lib.rs
+-rw-r--r--   0     1001      127     5550 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_relations/src/node_dictionary.rs
+-rw-r--r--   0     1001      127     5249 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_relations/src/relations_io.rs
+-rw-r--r--   0     1001      127     2658 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_relations/src/service/bfs.rs
+-rw-r--r--   0     1001      127      970 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_relations/src/service/mod.rs
+-rw-r--r--   0     1001      127     9828 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_relations/src/service/reader.rs
+-rw-r--r--   0     1001      127    10781 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_relations/src/service/tests.rs
+-rw-r--r--   0     1001      127     3071 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_relations/src/service/utils.rs
+-rw-r--r--   0     1001      127     7110 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_relations/src/service/writer.rs
+-rw-r--r--   0        0        0      399 1970-01-01 00:00:00.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_texts2/Cargo.toml
+-rw-r--r--   0     1001      127      931 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_texts2/src/lib.rs
+-rw-r--r--   0     1001      127     2755 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_texts2/src/query_io.rs
+-rw-r--r--   0     1001      127    22604 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_texts2/src/reader.rs
+-rw-r--r--   0     1001      127     3105 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_texts2/src/schema.rs
+-rw-r--r--   0     1001      127     8682 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_texts2/src/search_query.rs
+-rw-r--r--   0     1001      127    10377 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_texts2/src/writer.rs
+-rw-r--r--   0     1001      127     3391 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_texts2/tests/common/mod.rs
+-rw-r--r--   0     1001      127     2046 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_texts2/tests/test_reader.rs
+-rw-r--r--   0     1001      127     8881 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_texts2/tests/test_search.rs
+-rw-r--r--   0     1001      127     1249 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_texts2/tests/test_streaming.rs
+-rw-r--r--   0     1001      127     3460 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_texts2/tests/test_writer.rs
+-rw-r--r--   0        0        0      703 1970-01-01 00:00:00.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_vectors/Cargo.toml
+-rw-r--r--   0     1001      127       69 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_vectors/README.md
+-rw-r--r--   0     1001      127       43 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_vectors/docs/README.md
+-rw-r--r--   0     1001      127    25718 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_vectors/docs/labels.drawio.svg
+-rw-r--r--   0     1001      127    12250 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_vectors/src/data_point/disk_hnsw.rs
+-rw-r--r--   0     1001      127    19361 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_vectors/src/data_point/mod.rs
+-rw-r--r--   0     1001      127    11214 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_vectors/src/data_point/node.rs
+-rw-r--r--   0     1001      127    12611 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_vectors/src/data_point/ops_hnsw.rs
+-rw-r--r--   0     1001      127     1405 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_vectors/src/data_point/params.rs
+-rw-r--r--   0     1001      127     3952 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_vectors/src/data_point/ram_hnsw.rs
+-rw-r--r--   0     1001      127    11778 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_vectors/src/data_point/tests.rs
+-rw-r--r--   0     1001      127     5798 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_vectors/src/data_point_provider/garbage_collector.rs
+-rw-r--r--   0     1001      127     2722 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_vectors/src/data_point_provider/mod.rs
+-rw-r--r--   0     1001      127    10271 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_vectors/src/data_point_provider/reader.rs
+-rw-r--r--   0     1001      127     2304 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_vectors/src/data_point_provider/replication.rs
+-rw-r--r--   0     1001      127     5288 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_vectors/src/data_point_provider/state.rs
+-rw-r--r--   0     1001      127    20587 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_vectors/src/data_point_provider/writer.rs
+-rw-r--r--   0     1001      127    22479 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_vectors/src/data_types/data_store.rs
+-rw-r--r--   0     1001      127     6916 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_vectors/src/data_types/dtrie_ram.rs
+-rw-r--r--   0     1001      127     1959 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_vectors/src/data_types/mod.rs
+-rw-r--r--   0     1001      127     6143 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_vectors/src/data_types/trie.rs
+-rw-r--r--   0     1001      127     2904 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_vectors/src/data_types/trie_ram.rs
+-rw-r--r--   0     1001      127     4433 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_vectors/src/data_types/vector.rs
+-rw-r--r--   0     1001      127     8043 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_vectors/src/formula/mod.rs
+-rw-r--r--   0     1001      127     2154 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_vectors/src/lib.rs
+-rw-r--r--   0     1001      127     1278 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_vectors/src/service/mod.rs
+-rw-r--r--   0     1001      127     1897 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_vectors/src/service/query_io.rs
+-rw-r--r--   0     1001      127    17122 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_vectors/src/service/reader.rs
+-rw-r--r--   0     1001      127    15456 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_vectors/src/service/writer.rs
+-rw-r--r--   0     1001      127     2884 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_vectors/tests/test_merge.rs
+-rw-r--r--   0        0        0     3314 1970-01-01 00:00:00.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_node/Cargo.toml
+-rw-r--r--   0     1001      127     1045 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_node/.rustc_info.json
+-rw-r--r--   0     1001      127      877 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_node/Makefile
+-rw-r--r--   0     1001      127     1500 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_node/README.md
+-rw-r--r--   0     1001      127     1757 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_node/nucliadb_node/__init__.py
+-rw-r--r--   0     1001      127     3957 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_node/nucliadb_node/app.py
+-rw-r--r--   0     1001      127    17752 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_node/nucliadb_node/indexer.py
+-rw-r--r--   0     1001      127      890 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_node/nucliadb_node/listeners/__init__.py
+-rw-r--r--   0     1001      127     2424 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_node/nucliadb_node/listeners/indexed_publisher.py
+-rw-r--r--   0     1001      127     4015 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_node/nucliadb_node/pull.py
+-rw-r--r--   0     1001      127     1535 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_node/nucliadb_node/service.py
+-rw-r--r--   0     1001      127     1487 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_node/nucliadb_node/settings.py
+-rw-r--r--   0     1001      127     1133 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_node/nucliadb_node/signals.py
+-rw-r--r--   0     1001      127      835 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_node/nucliadb_node/tests/__init__.py
+-rw-r--r--   0     1001      127     1092 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_node/nucliadb_node/tests/conftest.py
+-rw-r--r--   0     1001      127    10810 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_node/nucliadb_node/tests/fixtures.py
+-rw-r--r--   0     1001      127    13788 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_node/nucliadb_node/tests/integration/test_indexing.py
+-rw-r--r--   0     1001      127     2289 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_node/nucliadb_node/tests/unit/test_app.py
+-rw-r--r--   0     1001      127     2361 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_node/nucliadb_node/tests/unit/test_indexed_publisher.py
+-rw-r--r--   0     1001      127    12553 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_node/nucliadb_node/tests/unit/test_indexer.py
+-rw-r--r--   0     1001      127     3379 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_node/nucliadb_node/tests/unit/test_pull.py
+-rw-r--r--   0     1001      127     2323 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_node/nucliadb_node/writer.py
+-rw-r--r--   0     1001      127      101 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_node/requirements-sources.txt
+-rw-r--r--   0     1001      127      276 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_node/requirements.txt
+-rw-r--r--   0     1001      127      249 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_node/setup.cfg
+-rw-r--r--   0     1001      127     1405 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_node/setup.py
+-rw-r--r--   0     1001      127     2518 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_node/src/analytics/blocking.rs
+-rw-r--r--   0     1001      127     1219 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_node/src/analytics/mod.rs
+-rw-r--r--   0     1001      127     4931 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_node/src/analytics/payload.rs
+-rw-r--r--   0     1001      127    12828 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_node/src/analytics/sender.rs
+-rw-r--r--   0     1001      127     3085 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_node/src/analytics/sink.rs
+-rw-r--r--   0     1001      127     1900 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_node/src/analytics/sync.rs
+-rw-r--r--   0     1001      127     4935 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_node/src/bin/reader.rs
+-rw-r--r--   0     1001      127     8050 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_node/src/bin/writer.rs
+-rw-r--r--   0     1001      127     1345 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_node/src/cache/mod.rs
+-rw-r--r--   0     1001      127     3043 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_node/src/cache/reader_cache.rs
+-rw-r--r--   0     1001      127    14199 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_node/src/cache/resource_cache.rs
+-rw-r--r--   0     1001      127    10999 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_node/src/cache/writer_cache.rs
+-rw-r--r--   0     1001      127     1771 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_node/src/disk_structure.rs
+-rw-r--r--   0     1001      127     2558 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_node/src/grpc/collect_garbage.rs
+-rw-r--r--   0     1001      127    18821 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_node/src/grpc/grpc_reader.rs
+-rw-r--r--   0     1001      127    13691 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_node/src/grpc/grpc_writer.rs
+-rw-r--r--   0     1001      127     3186 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_node/src/grpc/middleware/debug.rs
+-rw-r--r--   0     1001      127     3440 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_node/src/grpc/middleware/metrics.rs
+-rw-r--r--   0     1001      127     1009 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_node/src/grpc/middleware/mod.rs
+-rw-r--r--   0     1001      127     4158 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_node/src/grpc/middleware/telemetry.rs
+-rw-r--r--   0     1001      127     1283 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_node/src/grpc/mod.rs
+-rw-r--r--   0     1001      127     2482 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_node/src/grpc/update.rs
+-rw-r--r--   0     1001      127     1173 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_node/src/http_server/metrics_service.rs
+-rw-r--r--   0     1001      127     1465 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_node/src/http_server/mod.rs
+-rw-r--r--   0     1001      127     1943 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_node/src/http_server/traces_service.rs
+-rw-r--r--   0     1001      127     1488 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_node/src/lib.rs
+-rw-r--r--   0     1001      127     2757 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_node/src/lifecycle.rs
+-rw-r--r--   0     1001      127     1778 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_node/src/merge/global.rs
+-rw-r--r--   0     1001      127     1089 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_node/src/merge/mod.rs
+-rw-r--r--   0     1001      127    13672 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_node/src/merge/scheduler.rs
+-rw-r--r--   0     1001      127     3677 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_node/src/merge/work.rs
+-rw-r--r--   0     1001      127     1935 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_node/src/node_metadata.rs
+-rw-r--r--   0     1001      127     2417 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_node/src/replication/health.rs
+-rw-r--r--   0     1001      127     1070 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_node/src/replication/mod.rs
+-rw-r--r--   0     1001      127    14052 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_node/src/replication/replicator.rs
+-rw-r--r--   0     1001      127    11682 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_node/src/replication/service.rs
+-rw-r--r--   0     1001      127    11231 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_node/src/settings.rs
+-rw-r--r--   0     1001      127     1111 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_node/src/shards/errors.rs
+-rw-r--r--   0     1001      127    10834 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_node/src/shards/metadata.rs
+-rw-r--r--   0     1001      127     1122 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_node/src/shards/mod.rs
+-rw-r--r--   0     1001      127    24292 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_node/src/shards/shard_reader.rs
+-rw-r--r--   0     1001      127    19507 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_node/src/shards/shard_writer.rs
+-rw-r--r--   0     1001      127    10251 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_node/src/shards/versions.rs
+-rw-r--r--   0     1001      127    10170 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_node/src/telemetry.rs
+-rw-r--r--   0     1001      127     6396 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_node/src/utils.rs
+-rw-r--r--   0     1001      127       42 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_node/test.sh
+-rw-r--r--   0     1001      127     1115 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_node/tests/common/mod.rs
+-rw-r--r--   0     1001      127    12731 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_node/tests/common/node_services.rs
+-rw-r--r--   0     1001      127     7823 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_node/tests/common/resources.rs
+-rw-r--r--   0     1001      127     8173 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_node/tests/test_date_range_search.rs
+-rw-r--r--   0     1001      127     4089 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_node/tests/test_download.rs
+-rw-r--r--   0     1001      127     1684 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_node/tests/test_merge.rs
+-rw-r--r--   0     1001      127     6003 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_node/tests/test_replication.rs
+-rw-r--r--   0     1001      127    22494 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_node/tests/test_search_relations.rs
+-rw-r--r--   0     1001      127     6958 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_node/tests/test_search_sorting.rs
+-rw-r--r--   0     1001      127     7044 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_node/tests/test_security_search.rs
+-rw-r--r--   0     1001      127     6862 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_node/tests/test_shards.rs
+-rw-r--r--   0     1001      127    10698 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_node/tests/test_suggest.rs
+-rw-r--r--   0        0        0      943 1970-01-01 00:00:00.000000 nucliadb_node_binding-3.0.0.post1133/Cargo.toml
+-rw-r--r--   0     1001      127     1553 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/CHANGELOG.md
+-rw-r--r--   0     1001      127      895 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/Makefile
+-rw-r--r--   0     1001      127       52 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/README.md
+-rwxr-xr-x   0     1001      127      978 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/cov.sh
+-rw-r--r--   0     1001      127     1309 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/pyproject.toml
+-rw-r--r--   0     1001      127     2195 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/src/collect_garbage.rs
+-rw-r--r--   0     1001      127     1212 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/src/errors.rs
+-rw-r--r--   0     1001      127     2337 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/src/lib.rs
+-rw-r--r--   0     1001      127     9405 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/src/reader.rs
+-rw-r--r--   0     1001      127     2154 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/src/update.rs
+-rw-r--r--   0     1001      127     9123 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/src/writer.rs
+-rw-r--r--   0     1001      127      835 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/tests/__init__.py
+-rw-r--r--   0     1001      127      892 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/tests/conftest.py
+-rw-r--r--   0     1001      127     3903 2024-04-10 13:42:48.000000 nucliadb_node_binding-3.0.0.post1133/tests/integration/test_indexing.py
+-rw-r--r--   0        0        0      401 1970-01-01 00:00:00.000000 nucliadb_node_binding-3.0.0.post1133/PKG-INFO
```

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_paragraphs/Cargo.toml` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_paragraphs/Cargo.toml`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_paragraphs/src/fuzzy_query.rs` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_paragraphs2/src/fuzzy_query.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_paragraphs/src/lib.rs` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_paragraphs2/src/lib.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_paragraphs/src/query_io.rs` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_paragraphs2/src/query_io.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_paragraphs/src/reader.rs` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_paragraphs2/src/reader.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_paragraphs/src/schema.rs` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_paragraphs/src/schema.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_paragraphs/src/search_query.rs` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_paragraphs/src/search_query.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_paragraphs/src/search_response.rs` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_paragraphs2/src/search_response.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_paragraphs/src/stop_words.rs` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_paragraphs2/src/stop_words.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_paragraphs/src/writer.rs` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_paragraphs/src/writer.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_paragraphs/stop_words/ar.json` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_paragraphs2/stop_words/ar.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_paragraphs/stop_words/az.json` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_paragraphs2/stop_words/az.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_paragraphs/stop_words/bn.json` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_paragraphs2/stop_words/bn.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_paragraphs/stop_words/ca.json` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_paragraphs2/stop_words/ca.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_paragraphs/stop_words/ch.json` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_paragraphs2/stop_words/ch.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_paragraphs/stop_words/da.json` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_paragraphs2/stop_words/da.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_paragraphs/stop_words/de.json` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_paragraphs2/stop_words/de.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_paragraphs/stop_words/el.json` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_paragraphs2/stop_words/el.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_paragraphs/stop_words/en.json` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_paragraphs2/stop_words/en.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_paragraphs/stop_words/es.json` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_paragraphs2/stop_words/es.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_paragraphs/stop_words/eu.json` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_paragraphs2/stop_words/eu.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_paragraphs/stop_words/extract.py` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_paragraphs2/stop_words/extract.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_paragraphs/stop_words/fi.json` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_paragraphs2/stop_words/fi.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_paragraphs/stop_words/fr.json` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_paragraphs2/stop_words/fr.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_paragraphs/stop_words/he.json` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_paragraphs2/stop_words/he.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_paragraphs/stop_words/hu.json` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_paragraphs2/stop_words/hu.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_paragraphs/stop_words/id.json` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_paragraphs2/stop_words/id.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_paragraphs/stop_words/it.json` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_paragraphs2/stop_words/it.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_paragraphs/stop_words/kk.json` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_paragraphs2/stop_words/kk.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_paragraphs/stop_words/ne.json` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_paragraphs2/stop_words/ne.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_paragraphs/stop_words/nl.json` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_paragraphs2/stop_words/nl.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_paragraphs/stop_words/no.json` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_paragraphs2/stop_words/no.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_paragraphs/stop_words/pt.json` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_paragraphs2/stop_words/pt.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_paragraphs/stop_words/ro.json` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_paragraphs2/stop_words/ro.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_paragraphs/stop_words/ru.json` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_paragraphs2/stop_words/ru.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_paragraphs/stop_words/sl.json` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_paragraphs2/stop_words/sl.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_paragraphs/stop_words/sv.json` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_paragraphs2/stop_words/sv.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_paragraphs/stop_words/tg.json` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_paragraphs2/stop_words/tg.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_protos/build.rs` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_protos/build.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_protos/src/fdbwriter.rs` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_protos/src/fdbwriter.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_protos/src/knowledgebox.rs` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_protos/src/knowledgebox.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_protos/src/lib.rs` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_protos/src/lib.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_protos/src/nodereader.rs` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_protos/src/nodereader.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_protos/src/noderesources.rs` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_protos/src/noderesources.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_protos/src/nodewriter.rs` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_protos/src/nodewriter.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_protos/src/replication.rs` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_protos/src/replication.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_protos/src/resources.rs` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_protos/src/resources.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_protos/src/utils.rs` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_protos/src/utils.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_relations/Cargo.toml` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_relations/Cargo.toml`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_relations/src/bfs_engine.rs` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_relations/src/bfs_engine.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_relations/src/errors.rs` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_relations/src/errors.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_relations/src/graph_db.rs` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_relations/src/graph_db.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_relations/src/graph_test_utils.rs` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_relations/src/graph_test_utils.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_relations/src/index.rs` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_relations/src/index.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_relations/src/lib.rs` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_relations/src/lib.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_relations/src/node_dictionary.rs` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_relations/src/node_dictionary.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_relations/src/relations_io.rs` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_relations/src/relations_io.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_relations/src/service/bfs.rs` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_relations/src/service/bfs.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_relations/src/service/mod.rs` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_relations/src/service/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_relations/src/service/reader.rs` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_relations/src/service/reader.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_relations/src/service/tests.rs` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_relations/src/service/tests.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_relations/src/service/utils.rs` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_relations/src/service/utils.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_relations/src/service/writer.rs` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_relations/src/service/writer.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_procs/src/lib.rs` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_procs/src/lib.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_procs/src/measure.rs` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_procs/src/measure.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_procs/tests/dont_compile/actor_defined_twice.rs` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_procs/tests/dont_compile/actor_defined_twice.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_procs/tests/dont_compile/actor_not_defined.rs` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_procs/tests/dont_compile/actor_not_defined.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_procs/tests/dont_compile/metric_defined_twice.rs` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_procs/tests/dont_compile/metric_defined_twice.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_procs/tests/dont_compile/wrong_actor.rs` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_procs/tests/dont_compile/wrong_actor.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_procs/tests/dont_compile/wrong_actor.stderr` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_procs/tests/dont_compile/wrong_actor.stderr`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_procs/tests/test_measure.rs` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_procs/tests/test_measure.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_paragraphs2/Cargo.toml` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_paragraphs2/Cargo.toml`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_paragraphs2/src/fuzzy_query.rs` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_paragraphs/src/fuzzy_query.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_paragraphs2/src/lib.rs` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_paragraphs/src/lib.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_paragraphs2/src/query_io.rs` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_paragraphs/src/query_io.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_paragraphs2/src/reader.rs` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_paragraphs/src/reader.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_paragraphs2/src/schema.rs` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_paragraphs2/src/schema.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_paragraphs2/src/search_query.rs` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_paragraphs2/src/search_query.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_paragraphs2/src/search_response.rs` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_paragraphs/src/search_response.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_paragraphs2/src/stop_words.rs` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_paragraphs/src/stop_words.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_paragraphs2/src/writer.rs` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_paragraphs2/src/writer.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_paragraphs2/stop_words/ar.json` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_paragraphs/stop_words/ar.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_paragraphs2/stop_words/az.json` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_paragraphs/stop_words/az.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_paragraphs2/stop_words/bn.json` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_paragraphs/stop_words/bn.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_paragraphs2/stop_words/ca.json` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_paragraphs/stop_words/ca.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_paragraphs2/stop_words/ch.json` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_paragraphs/stop_words/ch.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_paragraphs2/stop_words/da.json` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_paragraphs/stop_words/da.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_paragraphs2/stop_words/de.json` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_paragraphs/stop_words/de.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_paragraphs2/stop_words/el.json` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_paragraphs/stop_words/el.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_paragraphs2/stop_words/en.json` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_paragraphs/stop_words/en.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_paragraphs2/stop_words/es.json` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_paragraphs/stop_words/es.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_paragraphs2/stop_words/eu.json` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_paragraphs/stop_words/eu.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_paragraphs2/stop_words/extract.py` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_paragraphs/stop_words/extract.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_paragraphs2/stop_words/fi.json` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_paragraphs/stop_words/fi.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_paragraphs2/stop_words/fr.json` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_paragraphs/stop_words/fr.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_paragraphs2/stop_words/he.json` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_paragraphs/stop_words/he.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_paragraphs2/stop_words/hu.json` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_paragraphs/stop_words/hu.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_paragraphs2/stop_words/id.json` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_paragraphs/stop_words/id.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_paragraphs2/stop_words/it.json` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_paragraphs/stop_words/it.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_paragraphs2/stop_words/kk.json` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_paragraphs/stop_words/kk.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_paragraphs2/stop_words/ne.json` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_paragraphs/stop_words/ne.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_paragraphs2/stop_words/nl.json` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_paragraphs/stop_words/nl.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_paragraphs2/stop_words/no.json` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_paragraphs/stop_words/no.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_paragraphs2/stop_words/pt.json` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_paragraphs/stop_words/pt.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_paragraphs2/stop_words/ro.json` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_paragraphs/stop_words/ro.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_paragraphs2/stop_words/ru.json` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_paragraphs/stop_words/ru.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_paragraphs2/stop_words/sl.json` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_paragraphs/stop_words/sl.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_paragraphs2/stop_words/sv.json` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_paragraphs/stop_words/sv.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_paragraphs2/stop_words/tg.json` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_paragraphs/stop_words/tg.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_relations2/Cargo.toml` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_relations2/Cargo.toml`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_relations2/src/io_maps.rs` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_relations2/src/io_maps.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_relations2/src/lib.rs` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_relations2/src/lib.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_relations2/src/reader.rs` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_relations2/src/reader.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_relations2/src/schema.rs` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_relations2/src/schema.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_relations2/src/writer.rs` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_relations2/src/writer.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_relations2/tests/common/mod.rs` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_relations2/tests/common/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_relations2/tests/test_reader.rs` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_relations2/tests/test_reader.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_relations2/tests/test_writer.rs` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_relations2/tests/test_writer.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_core/Cargo.toml` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_core/Cargo.toml`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_core/src/fs_state.rs` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_core/src/fs_state.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_core/src/lib.rs` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_core/src/lib.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_core/src/merge.rs` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_core/src/merge.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_core/src/metrics/meters/mod.rs` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_core/src/metrics/meters/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_core/src/metrics/meters/prometheus.rs` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_core/src/metrics/meters/prometheus.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_core/src/metrics/metric/grpc_ops.rs` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_core/src/metrics/metric/grpc_ops.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_core/src/metrics/metric/mod.rs` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_core/src/metrics/metric/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_core/src/metrics/metric/replication.rs` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_core/src/metrics/metric/replication.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_core/src/metrics/metric/request_time.rs` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_core/src/metrics/metric/request_time.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_core/src/metrics/metric/shard_cache.rs` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_core/src/metrics/metric/shard_cache.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_core/src/metrics/metric/tokio_runtime.rs` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_core/src/metrics/metric/tokio_runtime.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_core/src/metrics/metric/tokio_tasks.rs` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_core/src/metrics/metric/tokio_tasks.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_core/src/metrics/metric/vectors.rs` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_core/src/metrics/metric/vectors.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_core/src/metrics/mod.rs` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_core/src/metrics/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_core/src/metrics/task_monitor.rs` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_core/src/metrics/task_monitor.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_core/src/metrics/tests.rs` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_core/src/metrics/tests.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_core/src/paragraphs.rs` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_core/src/paragraphs.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_core/src/query_language/mod.rs` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_core/src/query_language/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_core/src/query_planner.rs` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_core/src/query_planner.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_core/src/relations.rs` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_core/src/relations.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_core/src/tantivy_replica.rs` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_core/src/tantivy_replica.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_core/src/texts.rs` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_core/src/texts.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_core/src/vectors.rs` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_core/src/vectors.rs`

 * *Files 14% similar despite different names*

```diff
@@ -47,15 +47,14 @@
     pub source: MergeSource,
 }
 
 #[derive(Clone)]
 pub struct VectorConfig {
     pub similarity: Option<VectorSimilarity>,
     pub path: PathBuf,
-    pub vectorset: PathBuf,
     pub channel: Channel,
     pub shard_id: String,
 }
 
 // In an ideal world this should be part of the actual request, but since
 // we use protos all the way down the stack here we are. Once the protos use
 // is restricted to only the upper layer, this type won't be needed anymore.
@@ -79,28 +78,25 @@
 pub trait MergeRunner {
     fn run(&mut self) -> NodeResult<Box<dyn MergeResults>>;
 }
 
 pub trait VectorReader: std::fmt::Debug + Send + Sync {
     fn search(&self, request: &ProtosRequest, context: &VectorsContext) -> NodeResult<ProtosResponse>;
     fn stored_ids(&self) -> NodeResult<Vec<String>>;
-    fn count(&self, vectorset: &str) -> NodeResult<usize>;
+    fn count(&self) -> NodeResult<usize>;
 
     fn update(&mut self) -> NodeResult<()>;
 }
 
 pub trait VectorWriter: std::fmt::Debug + Send + Sync {
     fn count(&self) -> NodeResult<usize>;
     fn get_segment_ids(&self) -> NodeResult<Vec<String>>;
     fn get_index_files(&self, ignored_segment_ids: &[String]) -> NodeResult<IndexFiles>;
-    fn list_vectorsets(&self) -> NodeResult<Vec<String>>;
 
     fn prepare_merge(&self, parameters: MergeParameters) -> NodeResult<Option<Box<dyn MergeRunner>>>;
     fn record_merge(&mut self, merge_result: Box<dyn MergeResults>, source: MergeSource) -> NodeResult<MergeMetrics>;
     fn set_resource(&mut self, resource: &Resource) -> NodeResult<()>;
     fn delete_resource(&mut self, resource_id: &ResourceId) -> NodeResult<()>;
     fn garbage_collection(&mut self) -> NodeResult<()>;
     fn force_garbage_collection(&mut self) -> NodeResult<()>;
-    fn remove_vectorset(&mut self, setid: &VectorSetId) -> NodeResult<()>;
-    fn add_vectorset(&mut self, setid: &VectorSetId, similarity: VectorSimilarity) -> NodeResult<()>;
     fn reload(&mut self) -> NodeResult<()>;
 }
```

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_texts/src/lib.rs` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_texts/src/lib.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_texts/src/query_io.rs` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_texts/src/query_io.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_texts/src/reader.rs` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_texts/src/reader.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_texts/src/schema.rs` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_texts/src/schema.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_texts/src/search_query.rs` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_texts/src/search_query.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_texts/src/writer.rs` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_texts/src/writer.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_texts/tests/common/mod.rs` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_texts/tests/common/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_texts/tests/test_reader.rs` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_texts/tests/test_reader.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_texts/tests/test_search.rs` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_texts/tests/test_search.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_texts/tests/test_streaming.rs` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_texts/tests/test_streaming.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_texts/tests/test_writer.rs` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_texts/tests/test_writer.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_vectors/Cargo.toml` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_vectors/Cargo.toml`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_vectors/docs/labels.drawio.svg` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_vectors/docs/labels.drawio.svg`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_vectors/src/data_point/disk_hnsw.rs` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_vectors/src/data_point/disk_hnsw.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_vectors/src/data_point/mod.rs` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_vectors/src/data_point/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_vectors/src/data_point/node.rs` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_vectors/src/data_point/node.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_vectors/src/data_point/ops_hnsw.rs` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_vectors/src/data_point/ops_hnsw.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_vectors/src/data_point/params.rs` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_vectors/src/data_point/params.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_vectors/src/data_point/ram_hnsw.rs` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_vectors/src/data_point/ram_hnsw.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_vectors/src/data_point/tests.rs` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_vectors/src/data_point/tests.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_vectors/src/data_point_provider/garbage_collector.rs` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_vectors/src/data_point_provider/garbage_collector.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_vectors/src/data_point_provider/mod.rs` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_vectors/src/data_point_provider/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_vectors/src/data_point_provider/reader.rs` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_vectors/src/data_point_provider/reader.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_vectors/src/data_point_provider/replication.rs` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_vectors/src/data_point_provider/replication.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_vectors/src/data_point_provider/state.rs` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_vectors/src/data_point_provider/state.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_vectors/src/data_point_provider/writer.rs` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_vectors/src/data_point_provider/writer.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_vectors/src/data_types/data_store.rs` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_vectors/src/data_types/data_store.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_vectors/src/data_types/dtrie_ram.rs` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_vectors/src/data_types/dtrie_ram.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_vectors/src/data_types/mod.rs` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_vectors/src/data_types/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_vectors/src/data_types/trie.rs` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_vectors/src/data_types/trie.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_vectors/src/data_types/trie_ram.rs` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_vectors/src/data_types/trie_ram.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_vectors/src/data_types/vector.rs` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_vectors/src/data_types/vector.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_vectors/src/formula/mod.rs` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_vectors/src/formula/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_vectors/src/indexset/state.rs` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_node/tests/common/mod.rs`

 * *Files 18% similar despite different names*

```diff
@@ -12,18 +12,17 @@
 // This program is distributed in the hope that it will be useful,
 // but WITHOUT ANY WARRANTY; without even the implied warranty of
 // MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 // GNU Affero General Public License for more details.
 //
 // You should have received a copy of the GNU Affero General Public License
 // along with this program. If not, see <http://www.gnu.org/licenses/>.
+//
+
+/// Utilities to test NucliaDB node
 
-use serde::{Deserialize, Serialize};
-use std::collections::HashSet;
-use std::path::PathBuf;
+#[allow(dead_code)] // clippy don't detect it's used in our integration tests]
+mod node_services;
+#[allow(dead_code)] // clippy don't detect it's used in our integration tests]
+pub mod resources;
 
-#[derive(Serialize, Deserialize, Default)]
-pub struct State {
-    #[allow(unused)]
-    location: PathBuf,
-    pub indexes: HashSet<String>,
-}
+pub use node_services::*;
```

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_vectors/src/lib.rs` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_vectors/src/lib.rs`

 * *Files 4% similar despite different names*

```diff
@@ -18,15 +18,14 @@
 // along with this program. If not, see <http://www.gnu.org/licenses/>.
 //
 
 pub mod data_point;
 pub mod data_point_provider;
 mod data_types;
 pub mod formula;
-pub mod indexset;
 pub mod service;
 
 use thiserror::Error;
 #[derive(Debug, Error)]
 pub enum VectorErr {
     #[error("Error using bincode: {0}")]
     BincodeError(#[from] bincode::Error),
```

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_vectors/src/service/mod.rs` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_vectors/src/service/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_vectors/src/service/query_io.rs` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_vectors/src/service/query_io.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_vectors/src/service/reader.rs` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_vectors/src/service/reader.rs`

 * *Files 4% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 //
 // You should have received a copy of the GNU Affero General Public License
 // along with this program. If not, see <http://www.gnu.org/licenses/>.
 
 use crate::data_point_provider::reader::Reader;
 use crate::data_point_provider::*;
 use crate::formula::{AtomClause, BooleanOperator, Clause, CompoundClause, Formula};
-use crate::indexset::ReaderSet;
 use crate::service::query_io;
 use nucliadb_core::prelude::*;
 use nucliadb_core::protos::prost::Message;
 use nucliadb_core::protos::{
     DocumentScored, DocumentVectorIdentifier, SentenceMetadata, VectorSearchRequest, VectorSearchResponse,
 };
 use nucliadb_core::tracing::{self, *};
@@ -49,41 +48,31 @@
     fn min_score(&self) -> f32 {
         self.1.min_score
     }
 }
 
 pub struct VectorReaderService {
     index: Reader,
-    indexset: ReaderSet,
 }
 impl Debug for VectorReaderService {
     fn fmt(&self, f: &mut std::fmt::Formatter<'_>) -> std::fmt::Result {
         f.debug_struct("VectorReaderService").finish()
     }
 }
 
 impl VectorReader for VectorReaderService {
     fn update(&mut self) -> NodeResult<()> {
         self.index.update()?;
-        self.indexset.update()?;
         Ok(())
     }
 
     #[tracing::instrument(skip_all)]
-    fn count(&self, vectorset: &str) -> NodeResult<usize> {
-        if vectorset.is_empty() {
-            debug!("Id for the vectorset is empty");
-            Ok(self.index.size())
-        } else if let Some(index) = self.indexset.get(vectorset)? {
-            debug!("Counting nodes for {vectorset}");
-            Ok(index.size())
-        } else {
-            debug!("There was not a set called {vectorset}");
-            Ok(0)
-        }
+    fn count(&self) -> NodeResult<usize> {
+        debug!("Id for the vectorset is empty");
+        Ok(self.index.size())
     }
 
     #[measure(actor = "vectors", metric = "search")]
     #[tracing::instrument(skip_all)]
     fn search(&self, request: &ProtosRequest, context: &VectorsContext) -> NodeResult<ProtosResponse> {
         let time = Instant::now();
 
@@ -114,24 +103,16 @@
             formula.extend(clause);
         }
 
         let search_request = (total_to_get, request, formula);
         let v = time.elapsed().as_millis();
         debug!("{id:?} - Searching: starts at {v} ms");
 
-        let result = if request.vector_set.is_empty() {
-            debug!("{id:?} - No vectorset specified, searching in the main index");
-            self.index.search(&search_request)?
-        } else if let Some(index) = self.indexset.get(&request.vector_set)? {
-            debug!("{id:?} - vectorset specified and found, searching on {}", request.vector_set);
-            index.search(&search_request)?
-        } else {
-            debug!("{id:?} - A was vectorset specified, but not found. {} is not a vectorset", request.vector_set);
-            vec![]
-        };
+        let result = self.index.search(&search_request)?;
+
         let v = time.elapsed().as_millis();
         debug!("{id:?} - Searching: ends at {v} ms");
         debug!("{id:?} - Creating results: starts at {v} ms");
 
         let documents = result
             .into_iter()
             .enumerate()
@@ -190,20 +171,16 @@
 
 impl VectorReaderService {
     #[tracing::instrument(skip_all)]
     pub fn start(config: &VectorConfig) -> NodeResult<Self> {
         if !config.path.exists() {
             return Err(node_error!("Invalid path {:?}", config.path));
         }
-        if !config.vectorset.exists() {
-            return Err(node_error!("Invalid path {:?}", config.vectorset));
-        }
         Ok(VectorReaderService {
             index: Reader::open(&config.path)?,
-            indexset: ReaderSet::new(&config.vectorset)?,
         })
     }
 }
 
 #[cfg(test)]
 mod tests {
     use std::collections::HashMap;
@@ -220,15 +197,14 @@
 
     #[test]
     fn test_key_prefix_search() {
         let dir = TempDir::new().unwrap();
         let vsc = VectorConfig {
             similarity: Some(VectorSimilarity::Cosine),
             path: dir.path().join("vectors"),
-            vectorset: dir.path().join("vectorset"),
             channel: Channel::EXPERIMENTAL,
             shard_id: "abc".into(),
         };
         let raw_sentences = [
             ("DOC/KEY/1/1".to_string(), vec![1.0, 3.0, 4.0]),
             ("DOC/KEY/1/2".to_string(), vec![2.0, 4.0, 5.0]),
             ("DOC/KEY/1/3".to_string(), vec![3.0, 5.0, 6.0]),
@@ -303,15 +279,14 @@
 
     #[test]
     fn test_new_vector_reader() {
         let dir = TempDir::new().unwrap();
         let vsc = VectorConfig {
             similarity: Some(VectorSimilarity::Cosine),
             path: dir.path().join("vectors"),
-            vectorset: dir.path().join("vectorset"),
             channel: Channel::EXPERIMENTAL,
             shard_id: "abc".into(),
         };
         let raw_sentences = [
             ("DOC/KEY/1/1".to_string(), vec![1.0, 3.0, 4.0]),
             ("DOC/KEY/1/2".to_string(), vec![2.0, 4.0, 5.0]),
             ("DOC/KEY/1/3".to_string(), vec![3.0, 5.0, 6.0]),
@@ -385,15 +360,15 @@
             field_labels: vec!["1".to_string()],
             page_number: 0,
             result_per_page: 20,
             with_duplicates: false,
             ..Default::default()
         };
         let result = reader.search(&request, &context).unwrap();
-        let no_nodes = reader.count("").unwrap();
+        let no_nodes = reader.count().unwrap();
         assert_eq!(no_nodes, 4);
         assert_eq!(result.documents.len(), 3);
 
         // Check that min_score works
         let request = VectorSearchRequest {
             id: "".to_string(),
             vector_set: "".to_string(),
@@ -402,15 +377,15 @@
             page_number: 0,
             result_per_page: 20,
             with_duplicates: false,
             min_score: 900.0,
             ..Default::default()
         };
         let result = reader.search(&request, &context).unwrap();
-        let no_nodes = reader.count("").unwrap();
+        let no_nodes = reader.count().unwrap();
         assert_eq!(no_nodes, 4);
         assert_eq!(result.documents.len(), 0);
 
         let bad_request = VectorSearchRequest {
             id: "".to_string(),
             vector_set: "".to_string(),
             vector: vec![4.0, 6.0],
@@ -425,15 +400,14 @@
 
     #[test]
     fn test_vectors_deduplication() {
         let dir = TempDir::new().unwrap();
         let vsc = VectorConfig {
             similarity: Some(VectorSimilarity::Cosine),
             path: dir.path().join("vectors"),
-            vectorset: dir.path().join("vectorset"),
             channel: Channel::EXPERIMENTAL,
             shard_id: "abc".into(),
         };
         let raw_sentences =
             [("DOC/KEY/1/1".to_string(), vec![1.0, 2.0, 3.0]), ("DOC/KEY/1/2".to_string(), vec![1.0, 2.0, 3.0])];
         let resource_id = ResourceId {
             shard_id: "DOC".to_string(),
```

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_vectors/tests/test_merge.rs` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_vectors/tests/test_merge.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_node/Cargo.toml` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_node/Cargo.toml`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_node/.rustc_info.json` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_node/.rustc_info.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_node/Makefile` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_node/Makefile`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_node/README.md` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_node/README.md`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_node/nucliadb_node/__init__.py` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_node/nucliadb_node/__init__.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_node/nucliadb_node/app.py` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_node/nucliadb_node/app.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 import asyncio
 import uuid
 from typing import Optional
 
 import pkg_resources
 
 from nucliadb_node import SERVICE_NAME, logger
-from nucliadb_node.listeners import IndexedPublisher, ShardGcScheduler
+from nucliadb_node.listeners import IndexedPublisher
 from nucliadb_node.pull import Worker
 from nucliadb_node.service import start_grpc
 from nucliadb_node.settings import indexing_settings, settings
 from nucliadb_node.writer import Writer
 from nucliadb_telemetry import errors
 from nucliadb_telemetry.logs import setup_logging
 from nucliadb_telemetry.utils import setup_telemetry
@@ -38,30 +38,23 @@
 from nucliadb_utils.run import run_until_exit
 from nucliadb_utils.utilities import get_storage, start_nats_manager, stop_nats_manager
 
 
 async def start_listeners(writer: Writer):
     return [
         await start_indexed_publisher(),
-        await start_shard_gc_scheduler(writer),
     ]
 
 
 async def start_indexed_publisher() -> IndexedPublisher:
     publisher = IndexedPublisher()
     await publisher.initialize()
     return publisher
 
 
-async def start_shard_gc_scheduler(writer: Writer) -> ShardGcScheduler:
-    scheduler = ShardGcScheduler(writer)
-    await scheduler.initialize()
-    return scheduler
-
-
 async def start_worker(
     writer: Writer, nats_connection_manager: NatsConnectionManager
 ) -> Worker:
     node = await get_node_id()
     if node is None:  # pragma: nocover
         raise Exception("No Key defined")
```

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_node/nucliadb_node/indexer.py` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_node/nucliadb_node/indexer.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_node/nucliadb_node/listeners/__init__.py` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_node/nucliadb_node/tests/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,10 +12,8 @@
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU Affero General Public License for more details.
 #
 # You should have received a copy of the GNU Affero General Public License
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
-
-from .gc_scheduler import ShardGcScheduler  # noqa
-from .indexed_publisher import IndexedPublisher  # noqa
+#
```

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_node/nucliadb_node/listeners/indexed_publisher.py` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_node/nucliadb_node/listeners/indexed_publisher.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_node/nucliadb_node/pull.py` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_node/nucliadb_node/pull.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_node/nucliadb_node/service.py` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_node/nucliadb_node/service.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_node/nucliadb_node/settings.py` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_node/nucliadb_node/settings.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_node/nucliadb_node/signals.py` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_node/nucliadb_node/signals.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_node/nucliadb_node/tests/__init__.py` & `nucliadb_node_binding-3.0.0.post1133/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_node/nucliadb_node/tests/conftest.py` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_node/nucliadb_node/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_node/nucliadb_node/tests/fixtures.py` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_node/nucliadb_node/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_node/nucliadb_node/tests/integration/test_indexing.py` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_node/nucliadb_node/tests/integration/test_indexing.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_node/nucliadb_node/tests/unit/test_app.py` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_node/nucliadb_node/tests/unit/test_app.py`

 * *Files 12% similar despite different names*

```diff
@@ -32,16 +32,14 @@
     ) as start_worker, patch(
         "nucliadb_node.app.start_nats_manager", AsyncMock()
     ) as _, patch(
         "nucliadb_node.app.stop_nats_manager", AsyncMock()
     ) as stop_nats_manager, patch(
         "nucliadb_node.app.start_indexed_publisher", AsyncMock()
     ) as start_indexed_publisher, patch(
-        "nucliadb_node.app.start_shard_gc_scheduler", AsyncMock()
-    ) as start_shard_gc_scheduler, patch(
         "nucliadb_node.app.start_grpc", AsyncMock()
     ) as start_grpc, patch(
         "nucliadb_node.app.serve_metrics", AsyncMock()
     ) as serve_metrics, patch(
         "nucliadb_node.app.run_until_exit", AsyncMock()
     ) as run_until_exit, patch(
         "nucliadb_node.app.Writer", MagicMock()
@@ -52,14 +50,13 @@
         await app.main()
 
         run_until_exit.assert_awaited_once_with(
             [
                 start_grpc.return_value,
                 start_worker.return_value.finalize,
                 start_indexed_publisher.return_value.finalize,
-                start_shard_gc_scheduler.return_value.finalize,
                 serve_metrics.return_value.shutdown,
                 writer.return_value.close,
                 stop_nats_manager,
                 storage.return_value.finalize,
             ]
         )
```

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_node/nucliadb_node/tests/unit/test_indexed_publisher.py` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_node/nucliadb_node/tests/unit/test_indexed_publisher.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 import pytest
 from nucliadb_protos.nodewriter_pb2 import IndexMessage
 
 from nucliadb_node.listeners import IndexedPublisher
 from nucliadb_node.signals import SuccessfulIndexingPayload, successful_indexing
 
 
-class TestShardGcScheduler:
+class TestIndexedPublisher:
     @pytest.fixture
     @pytest.mark.asyncio
     async def indexed_publisher(self):
         ip = IndexedPublisher()
         await ip.initialize()
         yield ip
         await ip.finalize()
```

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_node/nucliadb_node/tests/unit/test_indexer.py` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_node/nucliadb_node/tests/unit/test_indexer.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_node/nucliadb_node/writer.py` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_node/nucliadb_node/writer.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_node/setup.py` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_node/setup.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_node/src/analytics/blocking.rs` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_node/src/analytics/blocking.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_node/src/analytics/mod.rs` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_node/src/analytics/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_node/src/analytics/payload.rs` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_node/src/analytics/payload.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_node/src/analytics/sender.rs` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_node/src/analytics/sender.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_node/src/analytics/sink.rs` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_node/src/analytics/sink.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_node/src/analytics/sync.rs` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_node/src/analytics/sync.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_node/src/bin/reader.rs` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_node/src/bin/reader.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_node/src/bin/writer.rs` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_node/src/bin/writer.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_node/src/cache/mod.rs` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_node/src/cache/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_node/src/cache/reader_cache.rs` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_node/src/cache/reader_cache.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_node/src/cache/resource_cache.rs` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_node/src/cache/resource_cache.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_node/src/cache/writer_cache.rs` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_node/src/cache/writer_cache.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_node/src/disk_structure.rs` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_node/src/disk_structure.rs`

 * *Files 2% similar despite different names*

```diff
@@ -39,14 +39,13 @@
 pub const GENERATION_FILE: &str = "generation";
 
 pub const SHARDS_DIR: &str = "shards";
 
 pub const PARAGRAPHS_DIR: &str = "paragraph";
 pub const RELATIONS_DIR: &str = "relations";
 pub const TEXTS_DIR: &str = "text";
-pub const VECTORSET_DIR: &str = "vectorset";
 pub const VECTORS_DIR: &str = "vectors";
 
 /// Path where shard `id` is stored
 pub fn shard_path_by_id(shards_path: &Path, id: &str) -> PathBuf {
     shards_path.join(id)
 }
```

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_node/src/grpc/collect_garbage.rs` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_node/src/grpc/collect_garbage.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_node/src/grpc/grpc_reader.rs` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_node/src/grpc/grpc_reader.rs`

 * *Files 0% similar despite different names*

```diff
@@ -171,15 +171,15 @@
             Some(ref shard_id) => shard_id.id.clone(),
             None => return Err(tonic::Status::invalid_argument("Shard ID must be provided")),
         };
         let info = info_span!(parent: &span, "get shard");
         let shards = Arc::clone(&self.shards);
         let task = move || {
             let shard = obtain_shard(shards, shard_id)?;
-            run_with_telemetry(info, move || shard.get_info(&request))
+            run_with_telemetry(info, move || shard.get_info())
         };
         let shard_info = tokio::task::spawn_blocking(task)
             .await
             .map_err(|error| tonic::Status::internal(format!("Blocking task panicked: {error:?}")))?;
         match shard_info {
             Ok(shard) => Ok(tonic::Response::new(shard)),
             Err(error) => Err(tonic::Status::internal(error.to_string())),
```

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_node/src/grpc/grpc_writer.rs` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_node/src/grpc/grpc_writer.rs`

 * *Files 11% similar despite different names*

```diff
@@ -250,100 +250,24 @@
                     ..Default::default()
                 };
                 Ok(tonic::Response::new(status))
             }
         }
     }
 
-    async fn add_vector_set(&self, request: Request<NewVectorSetRequest>) -> Result<Response<OpStatus>, Status> {
-        let span = Span::current();
-        let request = request.into_inner();
-        let vectorset_id = match request.id {
-            Some(ref vectorset_id) => vectorset_id.clone(),
-            None => return Err(tonic::Status::invalid_argument("Vectorset ID must be provided")),
-        };
-        let shard_id = match vectorset_id.shard {
-            Some(ref shard_id) => &shard_id.id,
-            None => return Err(tonic::Status::invalid_argument("Shard ID must be provided")),
-        };
-
-        let shards = Arc::clone(&self.shards);
-        let shard_id_clone = shard_id.clone();
-        let info = info_span!(parent: &span, "add vector set");
-        let task = || {
-            run_with_telemetry(info, move || {
-                let shard = obtain_shard(shards, shard_id_clone)?;
-                shard.add_vectorset(&vectorset_id, request.similarity()).and_then(|()| shard.get_opstatus())
-            })
-        };
-        let status = tokio::task::spawn_blocking(task)
-            .await
-            .map_err(|error| tonic::Status::internal(format!("Blocking task panicked: {error:?}")))?;
-        match status {
-            Ok(mut status) => {
-                status.status = 0;
-                status.detail = "Success!".to_string();
-                Ok(tonic::Response::new(status))
-            }
-            Err(error) => Err(tonic::Status::internal(error.to_string())),
-        }
+    async fn add_vector_set(&self, _: Request<NewVectorSetRequest>) -> Result<Response<OpStatus>, Status> {
+        Err(tonic::Status::internal("Coming soon.."))
     }
 
-    async fn remove_vector_set(&self, request: Request<VectorSetId>) -> Result<Response<OpStatus>, Status> {
-        let span = Span::current();
-        let request = request.into_inner();
-        let shard_id = match request.shard {
-            Some(ref shard_id) => &shard_id.id,
-            None => return Err(tonic::Status::invalid_argument("Shard ID must be provided")),
-        };
-        let shards = Arc::clone(&self.shards);
-        let shard_id_clone = shard_id.clone();
-        let info = info_span!(parent: &span, "remove vector set");
-        let task = || {
-            run_with_telemetry(info, move || {
-                let shard = obtain_shard(shards, shard_id_clone)?;
-                shard.remove_vectorset(&request).and_then(|()| shard.get_opstatus())
-            })
-        };
-        let status = tokio::task::spawn_blocking(task)
-            .await
-            .map_err(|error| tonic::Status::internal(format!("Blocking task panicked: {error:?}")))?;
-        match status {
-            Ok(mut status) => {
-                status.status = 0;
-                status.detail = "Success!".to_string();
-                Ok(tonic::Response::new(status))
-            }
-            Err(error) => Err(tonic::Status::internal(error.to_string())),
-        }
+    async fn remove_vector_set(&self, _: Request<VectorSetId>) -> Result<Response<OpStatus>, Status> {
+        Err(tonic::Status::internal("Coming soon.."))
     }
 
-    async fn list_vector_sets(&self, request: Request<ShardId>) -> Result<Response<VectorSetList>, Status> {
-        let span = Span::current();
-        let shard_id = request.into_inner();
-        let shards = Arc::clone(&self.shards);
-        let shard_id_clone = shard_id.id.clone();
-        let info = info_span!(parent: &span, "list vector sets");
-        let task = || {
-            let shard = obtain_shard(shards, shard_id_clone)?;
-            run_with_telemetry(info, move || shard.list_vectorsets())
-        };
-        let status = tokio::task::spawn_blocking(task)
-            .await
-            .map_err(|error| tonic::Status::internal(format!("Blocking task panicked: {error:?}")))?;
-        match status {
-            Ok(vectorset) => {
-                let list = VectorSetList {
-                    vectorset,
-                    shard: Some(shard_id),
-                };
-                Ok(tonic::Response::new(list))
-            }
-            Err(error) => Err(tonic::Status::internal(error.to_string())),
-        }
+    async fn list_vector_sets(&self, _: Request<ShardId>) -> Result<Response<VectorSetList>, Status> {
+        Err(tonic::Status::internal("Coming soon.."))
     }
 
     async fn get_metadata(&self, _request: Request<EmptyQuery>) -> Result<Response<NodeMetadata>, Status> {
         let settings = &self.settings;
         let mut total_disk = 0;
         let mut available_disk = 0;
```

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_node/src/grpc/middleware/debug.rs` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_node/src/grpc/middleware/debug.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_node/src/grpc/middleware/metrics.rs` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_node/src/grpc/middleware/metrics.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_node/src/grpc/middleware/mod.rs` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_node/src/grpc/middleware/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_node/src/grpc/middleware/telemetry.rs` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_node/src/grpc/middleware/telemetry.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_node/src/grpc/mod.rs` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_node/src/grpc/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_node/src/grpc/update.rs` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_node/src/grpc/update.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_node/src/http_server/metrics_service.rs` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_node/src/http_server/metrics_service.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_node/src/http_server/mod.rs` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_node/src/http_server/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_node/src/http_server/traces_service.rs` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_node/src/http_server/traces_service.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_node/src/lib.rs` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_node/src/lib.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_node/src/lifecycle.rs` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_node/src/lifecycle.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_node/src/merge/global.rs` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_node/src/merge/global.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_node/src/merge/mod.rs` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_node/src/merge/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_node/src/merge/scheduler.rs` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_node/src/merge/scheduler.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_node/src/merge/work.rs` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_node/src/merge/work.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_node/src/node_metadata.rs` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_node/src/node_metadata.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_node/src/replication/health.rs` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_node/src/replication/health.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_node/src/replication/mod.rs` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_node/src/replication/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_node/src/replication/replicator.rs` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_node/src/replication/replicator.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_node/src/replication/service.rs` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_node/src/replication/service.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_node/src/settings.rs` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_node/src/settings.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_node/src/shards/errors.rs` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_node/src/shards/errors.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_node/src/shards/metadata.rs` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_node/src/shards/metadata.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_node/src/shards/mod.rs` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_node/src/shards/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_node/src/shards/shard_reader.rs` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_node/src/shards/shard_reader.rs`

 * *Files 1% similar despite different names*

```diff
@@ -22,18 +22,18 @@
 use crate::telemetry::run_with_telemetry;
 use crossbeam_utils::thread as crossbeam_thread;
 use nucliadb_core::paragraphs::*;
 use nucliadb_core::prelude::*;
 use nucliadb_core::protos;
 use nucliadb_core::protos::shard_created::{DocumentService, ParagraphService, RelationService, VectorService};
 use nucliadb_core::protos::{
-    DocumentSearchRequest, DocumentSearchResponse, EdgeList, GetShardRequest, ParagraphSearchRequest,
-    ParagraphSearchResponse, RelationPrefixSearchRequest, RelationSearchRequest, RelationSearchResponse, SearchRequest,
-    SearchResponse, Shard, ShardFile, ShardFileChunk, ShardFileList, StreamRequest, SuggestFeatures, SuggestRequest,
-    SuggestResponse, VectorSearchRequest, VectorSearchResponse,
+    DocumentSearchRequest, DocumentSearchResponse, EdgeList, ParagraphSearchRequest, ParagraphSearchResponse,
+    RelationPrefixSearchRequest, RelationSearchRequest, RelationSearchResponse, SearchRequest, SearchResponse, Shard,
+    ShardFile, ShardFileChunk, ShardFileList, StreamRequest, SuggestFeatures, SuggestRequest, SuggestResponse,
+    VectorSearchRequest, VectorSearchResponse,
 };
 use nucliadb_core::query_planner;
 use nucliadb_core::relations::*;
 use nucliadb_core::texts::*;
 use nucliadb_core::thread::*;
 use nucliadb_core::tracing::{self, *};
 use nucliadb_core::vectors::*;
@@ -150,27 +150,27 @@
             2 => RelationService::RelationV2,
             i => panic!("Unknown relation version {i}"),
         }
     }
 
     #[measure(actor = "shard", metric = "get_info")]
     #[tracing::instrument(skip_all)]
-    pub fn get_info(&self, request: &GetShardRequest) -> NodeResult<Shard> {
+    pub fn get_info(&self) -> NodeResult<Shard> {
         let span = tracing::Span::current();
 
         let paragraphs = self.paragraph_reader.clone();
         let vectors = self.vector_reader.clone();
         let texts = self.text_reader.clone();
 
         let info = info_span!(parent: &span, "text count");
         let text_task = || run_with_telemetry(info, move || read_rw_lock(&texts).count());
         let info = info_span!(parent: &span, "paragraph count");
         let paragraph_task = || run_with_telemetry(info, move || read_rw_lock(&paragraphs).count());
         let info = info_span!(parent: &span, "vector count");
-        let vector_task = || run_with_telemetry(info, move || read_rw_lock(&vectors).count(&request.vectorset));
+        let vector_task = || run_with_telemetry(info, move || read_rw_lock(&vectors).count());
 
         let mut text_result = Ok(0);
         let mut paragraph_result = Ok(0);
         let mut vector_result = Ok(0);
         crossbeam_thread::scope(|s| {
             s.spawn(|_| text_result = text_task());
             s.spawn(|_| paragraph_result = paragraph_task());
@@ -232,15 +232,14 @@
         };
 
         let channel = metadata.channel();
 
         let vsc = VectorConfig {
             similarity: None,
             path: shard_path.join(VECTORS_DIR),
-            vectorset: shard_path.join(VECTORSET_DIR),
             channel,
             shard_id: id.clone(),
         };
         let rsc = RelationConfig {
             path: shard_path.join(RELATIONS_DIR),
             channel,
         };
@@ -585,16 +584,16 @@
 
     #[tracing::instrument(skip_all)]
     pub fn paragraph_count(&self) -> NodeResult<usize> {
         read_rw_lock(&self.paragraph_reader).count()
     }
 
     #[tracing::instrument(skip_all)]
-    pub fn vector_count(&self, vector_set: &str) -> NodeResult<usize> {
-        read_rw_lock(&self.vector_reader).count(vector_set)
+    pub fn vector_count(&self) -> NodeResult<usize> {
+        read_rw_lock(&self.vector_reader).count()
     }
 
     #[tracing::instrument(skip_all)]
     pub fn text_count(&self) -> NodeResult<usize> {
         read_rw_lock(&self.text_reader).count()
     }
```

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_node/src/shards/shard_writer.rs` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_node/src/shards/shard_writer.rs`

 * *Files 5% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 use std::collections::HashMap;
 use std::path::PathBuf;
 use std::sync::{Arc, Mutex, MutexGuard};
 
 use nucliadb_core::paragraphs::*;
 use nucliadb_core::prelude::*;
 use nucliadb_core::protos::shard_created::{DocumentService, ParagraphService, RelationService, VectorService};
-use nucliadb_core::protos::{OpStatus, Resource, ResourceId, VectorSetId, VectorSimilarity};
+use nucliadb_core::protos::{OpStatus, Resource, ResourceId};
 use nucliadb_core::relations::*;
 use nucliadb_core::texts::*;
 use nucliadb_core::tracing::{self, *};
 use nucliadb_core::vectors::*;
 use nucliadb_core::{thread, IndexFiles};
 use nucliadb_procs::measure;
 use nucliadb_vectors::VectorErr;
@@ -185,15 +185,14 @@
         };
 
         let channel = metadata.channel();
 
         let vsc = VectorConfig {
             similarity: Some(metadata.similarity()),
             path: path.join(VECTORS_DIR),
-            vectorset: path.join(VECTORSET_DIR),
             channel,
             shard_id: metadata.id(),
         };
         let rsc = RelationConfig {
             path: path.join(RELATIONS_DIR),
             channel,
         };
@@ -217,15 +216,14 @@
         };
 
         let channel = metadata.channel();
 
         let vsc = VectorConfig {
             similarity: None,
             path: path.join(VECTORS_DIR),
-            vectorset: path.join(VECTORSET_DIR),
             channel,
             shard_id: metadata.id(),
         };
         let rsc = RelationConfig {
             path: path.join(RELATIONS_DIR),
             channel,
         };
@@ -395,41 +393,14 @@
             paragraph_count: paragraph_count? as u64,
             sentence_count: vector_count? as u64,
             ..Default::default()
         })
     }
 
     #[tracing::instrument(skip_all)]
-    pub fn list_vectorsets(&self) -> NodeResult<Vec<String>> {
-        let reader = read_rw_lock(&self.vector_writer);
-        let keys = reader.list_vectorsets()?;
-        Ok(keys)
-    }
-
-    #[tracing::instrument(skip_all)]
-    pub fn add_vectorset(&self, setid: &VectorSetId, similarity: VectorSimilarity) -> NodeResult<()> {
-        let mut writer = write_rw_lock(&self.vector_writer);
-        writer.add_vectorset(setid, similarity)?;
-
-        self.metadata.new_generation_id();
-
-        Ok(())
-    }
-
-    #[tracing::instrument(skip_all)]
-    pub fn remove_vectorset(&self, setid: &VectorSetId) -> NodeResult<()> {
-        let mut writer = write_rw_lock(&self.vector_writer);
-        writer.remove_vectorset(setid)?;
-
-        self.metadata.new_generation_id();
-
-        Ok(())
-    }
-
-    #[tracing::instrument(skip_all)]
     pub fn paragraph_count(&self) -> NodeResult<usize> {
         read_rw_lock(&self.paragraph_writer).count()
     }
 
     #[tracing::instrument(skip_all)]
     pub fn vector_count(&self) -> NodeResult<usize> {
         read_rw_lock(&self.vector_writer).count()
```

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_node/src/shards/versions.rs` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_node/src/shards/versions.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_node/src/telemetry.rs` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_node/src/telemetry.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_node/src/utils.rs` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_node/src/utils.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_node/tests/common/mod.rs` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_node/nucliadb_node/listeners/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,28 +1,20 @@
-// Copyright (C) 2021 Bosutech XXI S.L.
-//
-// nucliadb is offered under the AGPL v3.0 and as commercial software.
-// For commercial licensing, contact us at info@nuclia.com.
-//
-// AGPL:
-// This program is free software: you can redistribute it and/or modify
-// it under the terms of the GNU Affero General Public License as
-// published by the Free Software Foundation, either version 3 of the
-// License, or (at your option) any later version.
-//
-// This program is distributed in the hope that it will be useful,
-// but WITHOUT ANY WARRANTY; without even the implied warranty of
-// MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
-// GNU Affero General Public License for more details.
-//
-// You should have received a copy of the GNU Affero General Public License
-// along with this program. If not, see <http://www.gnu.org/licenses/>.
-//
+# Copyright (C) 2021 Bosutech XXI S.L.
+#
+# nucliadb is offered under the AGPL v3.0 and as commercial software.
+# For commercial licensing, contact us at info@nuclia.com.
+#
+# AGPL:
+# This program is free software: you can redistribute it and/or modify
+# it under the terms of the GNU Affero General Public License as
+# published by the Free Software Foundation, either version 3 of the
+# License, or (at your option) any later version.
+#
+# This program is distributed in the hope that it will be useful,
+# but WITHOUT ANY WARRANTY; without even the implied warranty of
+# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
+# GNU Affero General Public License for more details.
+#
+# You should have received a copy of the GNU Affero General Public License
+# along with this program. If not, see <http://www.gnu.org/licenses/>.
 
-/// Utilities to test NucliaDB node
-
-#[allow(dead_code)] // clippy don't detect it's used in our integration tests]
-mod node_services;
-#[allow(dead_code)] // clippy don't detect it's used in our integration tests]
-pub mod resources;
-
-pub use node_services::*;
+from .indexed_publisher import IndexedPublisher  # noqa
```

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_node/tests/common/node_services.rs` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_node/tests/common/node_services.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_node/tests/common/resources.rs` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_node/tests/common/resources.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_node/tests/test_date_range_search.rs` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_node/tests/test_date_range_search.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_node/tests/test_download.rs` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_node/tests/test_download.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_node/tests/test_merge.rs` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_node/tests/test_merge.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_node/tests/test_replication.rs` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_node/tests/test_replication.rs`

 * *Files 18% similar despite different names*

```diff
@@ -20,18 +20,15 @@
 
 mod common;
 
 use std::collections::HashMap;
 use std::sync::Arc;
 
 use common::{resources, NodeFixture, TestNodeReader, TestNodeWriter};
-use nucliadb_core::protos::{
-    op_status, NewShardRequest, NewVectorSetRequest, ReleaseChannel, SearchRequest, SearchResponse, ShardId,
-    UserVector, UserVectors, VectorSetId, VectorSimilarity,
-};
+use nucliadb_core::protos::{op_status, NewShardRequest, ReleaseChannel, SearchRequest, SearchResponse, ShardId};
 use nucliadb_node::replication::health::ReplicationHealthManager;
 use rstest::*;
 use tonic::Request;
 
 #[rstest]
 #[tokio::test]
 async fn test_search_replicated_data(
@@ -69,15 +66,14 @@
     assert!(response.vector.is_some());
     assert!(response.document.is_some());
     assert!(response.paragraph.is_some());
     assert_eq!(response.document.unwrap().results.len(), 2);
     assert_eq!(response.paragraph.unwrap().results.len(), 2);
     assert_eq!(response.vector.unwrap().documents.len(), 1);
 
-    query.vectorset = "test_vector_set".to_string();
     query.vector = vec![1.0, 2.0, 3.0];
     let response = run_search(&mut secondary_reader, query.clone()).await;
     assert!(response.vector.is_some());
     assert_eq!(response.vector.unwrap().documents.len(), 1);
 
     // Validate generation id is the same
     let primary_shard = Arc::downgrade(&fixture.primary_shard_cache().get(&shard.id)?);
@@ -94,15 +90,16 @@
     // wait for the shard to be deleted
     tokio::time::sleep(std::time::Duration::from_secs(2)).await;
 
     assert!(primary_shard.upgrade().is_none());
     assert!(secondary_shard.upgrade().is_none());
 
     let err_search_result = secondary_reader.search(query).await;
-    assert!(err_search_result.is_err());
+
+    let _err = err_search_result;
 
     Ok(())
 }
 
 struct ShardDetails {
     id: String,
 }
@@ -110,27 +107,14 @@
 async fn create_shard(writer: &mut TestNodeWriter, release_channel: ReleaseChannel) -> ShardDetails {
     let request = Request::new(NewShardRequest {
         release_channel: release_channel.into(),
         ..Default::default()
     });
     let new_shard_response = writer.new_shard(request).await.expect("Unable to create new shard");
     let shard_id = &new_shard_response.get_ref().id;
-
-    writer
-        .add_vector_set(NewVectorSetRequest {
-            id: Some(VectorSetId {
-                shard: Some(ShardId {
-                    id: shard_id.clone(),
-                }),
-                vectorset: "test_vector_set".to_string(),
-            }),
-            similarity: VectorSimilarity::Cosine as i32,
-        })
-        .await
-        .expect("Unable to create vector set");
     create_test_resources(writer, shard_id.clone()).await;
     ShardDetails {
         id: shard_id.to_owned(),
     }
 }
 
 async fn delete_shard(writer: &mut TestNodeWriter, shard_id: String) {
@@ -143,34 +127,16 @@
 async fn create_test_resources(writer: &mut TestNodeWriter, shard_id: String) -> HashMap<&str, String> {
     let resources = [
         ("little prince", resources::little_prince(&shard_id)),
         ("zarathustra", resources::thus_spoke_zarathustra(&shard_id)),
         ("pap", resources::people_and_places(&shard_id)),
     ];
     let mut resource_uuids = HashMap::new();
-
-    let mut user_vectors = HashMap::new();
-    user_vectors.insert(
-        "test_vector".to_string(),
-        UserVector {
-            vector: vec![1.0, 2.0, 3.0],
-            labels: vec!["label1".to_string(), "label2".to_string()],
-            start: 0,
-            end: 3,
-        },
-    );
-
-    for (name, mut resource) in resources.into_iter() {
+    for (name, resource) in resources.into_iter() {
         resource_uuids.insert(name, resource.resource.as_ref().unwrap().uuid.clone());
-        resource.vectors.insert(
-            "test_vector_set".to_string(),
-            UserVectors {
-                vectors: user_vectors.clone(),
-            },
-        );
         let response = writer.set_resource(resource).await.unwrap();
         assert_eq!(response.get_ref().status, op_status::Status::Ok as i32);
     }
 
     resource_uuids
 }
```

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_node/tests/test_search_relations.rs` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_node/tests/test_search_relations.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_node/tests/test_search_sorting.rs` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_node/tests/test_search_sorting.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_node/tests/test_security_search.rs` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_node/tests/test_security_search.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_node/tests/test_shards.rs` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_node/tests/test_shards.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_node/tests/test_suggest.rs` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_node/tests/test_suggest.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_texts2/src/lib.rs` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_texts2/src/lib.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_texts2/src/query_io.rs` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_texts2/src/query_io.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_texts2/src/reader.rs` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_texts2/src/reader.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_texts2/src/schema.rs` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_texts2/src/schema.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_texts2/src/search_query.rs` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_texts2/src/search_query.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_texts2/src/writer.rs` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_texts2/src/writer.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_texts2/tests/common/mod.rs` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_texts2/tests/common/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_texts2/tests/test_reader.rs` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_texts2/tests/test_reader.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_texts2/tests/test_search.rs` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_texts2/tests/test_search.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_texts2/tests/test_streaming.rs` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_texts2/tests/test_streaming.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/local_dependencies/nucliadb_texts2/tests/test_writer.rs` & `nucliadb_node_binding-3.0.0.post1133/local_dependencies/nucliadb_texts2/tests/test_writer.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/Cargo.toml` & `nucliadb_node_binding-3.0.0.post1133/Cargo.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "nucliadb_node_binding"
-version = "2.46.1-post1112"
+version = "3.0.0-post1133"
 edition = "2021"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 [lib]
 name = "nucliadb_node_binding"
 crate-type = ["cdylib"]
```

### Comparing `nucliadb_node_binding-2.46.1.post1112/CHANGELOG.md` & `nucliadb_node_binding-3.0.0.post1133/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/Makefile` & `nucliadb_node_binding-3.0.0.post1133/Makefile`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/cov.sh` & `nucliadb_node_binding-3.0.0.post1133/cov.sh`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/pyproject.toml` & `nucliadb_node_binding-3.0.0.post1133/pyproject.toml`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/src/collect_garbage.rs` & `nucliadb_node_binding-3.0.0.post1133/src/collect_garbage.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/src/errors.rs` & `nucliadb_node_binding-3.0.0.post1133/src/errors.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/src/lib.rs` & `nucliadb_node_binding-3.0.0.post1133/src/lib.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/src/reader.rs` & `nucliadb_node_binding-3.0.0.post1133/src/reader.rs`

 * *Files 0% similar despite different names*

```diff
@@ -135,15 +135,15 @@
 
     pub fn get_shard<'p>(&mut self, shard_id: RawProtos, py: Python<'p>) -> PyResult<&'p PyAny> {
         let request = GetShardRequest::decode(&mut Cursor::new(shard_id)).expect("Error decoding arguments");
         let Some(shard_id) = request.shard_id.clone() else {
             return Err(PyValueError::new_err("Missing shard_id field"));
         };
         let shard = self.obtain_shard(shard_id.id)?;
-        match shard.get_info(&request) {
+        match shard.get_info() {
             Ok(shard) => Ok(PyList::new(py, shard.encode_to_vec())),
             Err(error) => Err(IndexNodeException::new_err(error.to_string())),
         }
     }
 
     pub fn search<'p>(&mut self, request: RawProtos, py: Python<'p>) -> PyResult<&'p PyAny> {
         let search_request = SearchRequest::decode(&mut Cursor::new(request)).expect("Error decoding arguments");
```

### Comparing `nucliadb_node_binding-2.46.1.post1112/src/update.rs` & `nucliadb_node_binding-3.0.0.post1133/src/update.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1112/src/writer.rs` & `nucliadb_node_binding-3.0.0.post1133/src/writer.rs`

 * *Files 14% similar despite different names*

```diff
@@ -32,15 +32,14 @@
 use nucliadb_node::analytics::payload::AnalyticsEvent;
 use nucliadb_node::cache::ShardWriterCache;
 use nucliadb_node::lifecycle;
 use nucliadb_node::settings::load_settings;
 use nucliadb_node::shards::metadata::ShardMetadata;
 use nucliadb_node::shards::writer::ShardWriter;
 use prost::Message;
-use pyo3::exceptions::PyValueError;
 use pyo3::prelude::*;
 use pyo3::types::PyList;
 use std::thread::JoinHandle;
 use std::time::Duration;
 
 const GC_LOOP_INTERVAL: Duration = Duration::from_secs(60);
 
@@ -199,88 +198,26 @@
                 };
                 Ok(PyList::new(py, status.encode_to_vec()))
             }
         }
     }
 
     // TODO: rename to list_vectorsets
-    pub fn get_vectorset<'p>(&mut self, request: RawProtos, py: Python<'p>) -> PyResult<&'p PyAny> {
-        let shard_id = ShardId::decode(&mut Cursor::new(request)).expect("Error decoding arguments");
-        let shard = self.obtain_shard(shard_id.id.clone())?;
-        let vector_sets = shard.list_vectorsets();
-        match vector_sets {
-            Ok(vector_sets) => {
-                let response = VectorSetList {
-                    shard: Some(shard_id),
-                    vectorset: vector_sets,
-                };
-                Ok(PyList::new(py, response.encode_to_vec()))
-            }
-            Err(error) => {
-                let message = format!("Error listing vectorsets: {}", error);
-                Err(IndexNodeException::new_err(message))
-            }
-        }
+    pub fn get_vectorset<'p>(&mut self, _request: RawProtos, _py: Python<'p>) -> PyResult<&'p PyAny> {
+        Err(IndexNodeException::new_err("Coming soon.."))
     }
 
     // TODO
-    pub fn set_vectorset<'p>(&mut self, request: RawProtos, py: Python<'p>) -> PyResult<&'p PyAny> {
-        let request = NewVectorSetRequest::decode(&mut Cursor::new(request)).expect("Error decoding arguments");
-        let Some(ref vectorset_id) = request.id else {
-            return Err(PyValueError::new_err("Missing vectorset id field"));
-        };
-        let Some(ref shard_id) = vectorset_id.shard else {
-            return Err(PyValueError::new_err("Missing shard id field"));
-        };
-        let shard = self.obtain_shard(shard_id.id.clone())?;
-        let status = shard.add_vectorset(vectorset_id, request.similarity()).and_then(|()| shard.get_opstatus());
-        match status {
-            Ok(mut status) => {
-                status.status = 0;
-                status.detail = "Success!".to_string();
-                Ok(PyList::new(py, status.encode_to_vec()))
-            }
-            Err(error) => {
-                let op_status = OpStatus {
-                    status: op_status::Status::Error as i32,
-                    detail: error.to_string(),
-                    field_count: 0_u64,
-                    shard_id: shard_id.id.clone(),
-                    ..Default::default()
-                };
-                Ok(PyList::new(py, op_status.encode_to_vec()))
-            }
-        }
+    pub fn set_vectorset<'p>(&mut self, _request: RawProtos, _py: Python<'p>) -> PyResult<&'p PyAny> {
+        Err(IndexNodeException::new_err("Coming soon.."))
     }
 
     // TODO
-    pub fn del_vectorset<'p>(&mut self, request: RawProtos, py: Python<'p>) -> PyResult<&'p PyAny> {
-        let vectorset = VectorSetId::decode(&mut Cursor::new(request)).expect("Error decoding arguments");
-        let Some(ref shard_id) = vectorset.shard else {
-            return Err(PyValueError::new_err("Missing shard id field"));
-        };
-        let shard = self.obtain_shard(shard_id.id.clone())?;
-        let status = shard.remove_vectorset(&vectorset).and_then(|()| shard.get_opstatus());
-        match status {
-            Ok(mut status) => {
-                status.status = 0;
-                status.detail = "Success!".to_string();
-                Ok(PyList::new(py, status.encode_to_vec()))
-            }
-            Err(error) => {
-                let op_status = OpStatus {
-                    status: op_status::Status::Error as i32,
-                    detail: error.to_string(),
-                    field_count: 0_u64,
-                    shard_id: shard_id.id.clone(),
-                    ..Default::default()
-                };
-                Ok(PyList::new(py, op_status.encode_to_vec()))
-            }
-        }
+    pub fn del_vectorset<'p>(&mut self, _request: RawProtos, _py: Python<'p>) -> PyResult<&'p PyAny> {
+        Err(IndexNodeException::new_err("Coming soon.."))
     }
 
     pub fn gc<'p>(&mut self, request: RawProtos, py: Python<'p>) -> PyResult<&'p PyAny> {
         send_analytics_event(AnalyticsEvent::GarbageCollect);
         let shard_id = ShardId::decode(&mut Cursor::new(request)).expect("Error decoding arguments");
         let shard = self.obtain_shard(shard_id.id)?;
         let result = shard.force_garbage_collection();
```

### Comparing `nucliadb_node_binding-2.46.1.post1112/tests/__init__.py` & `nucliadb_node_binding-3.0.0.post1133/tests/conftest.py`

 * *Files 19% similar despite different names*

```diff
@@ -13,7 +13,10 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU Affero General Public License for more details.
 #
 # You should have received a copy of the GNU Affero General Public License
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
 #
+pytest_plugins = [
+    "nucliadb_node.tests.fixtures",
+]
```

### Comparing `nucliadb_node_binding-2.46.1.post1112/tests/integration/test_indexing.py` & `nucliadb_node_binding-3.0.0.post1133/tests/integration/test_indexing.py`

 * *Files identical despite different names*

