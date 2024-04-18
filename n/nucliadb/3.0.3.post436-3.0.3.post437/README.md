# Comparing `tmp/nucliadb-3.0.3.post436-py3-none-any.whl.zip` & `tmp/nucliadb-3.0.3.post437-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,453 +1,455 @@
-Zip file size: 746800 bytes, number of entries: 451
--rw-r--r--  2.0 unx     1135 b- defN 24-Apr-18 07:57 migrations/0001_bootstrap.py
--rw-r--r--  2.0 unx     1177 b- defN 24-Apr-18 07:57 migrations/0002_rollover_shards.py
--rw-r--r--  2.0 unx     2436 b- defN 24-Apr-18 07:57 migrations/0003_allfields_key.py
--rw-r--r--  2.0 unx     1177 b- defN 24-Apr-18 07:57 migrations/0004_rollover_shards.py
--rw-r--r--  2.0 unx     1177 b- defN 24-Apr-18 07:57 migrations/0005_rollover_shards.py
--rw-r--r--  2.0 unx     1024 b- defN 24-Apr-18 07:57 migrations/0006_rollover_shards.py
--rw-r--r--  2.0 unx     1301 b- defN 24-Apr-18 07:57 migrations/0008_cleanup_leftover_rollover_metadata.py
--rw-r--r--  2.0 unx     1378 b- defN 24-Apr-18 07:57 migrations/0009_upgrade_relations_and_texts_to_v2.py
--rw-r--r--  2.0 unx     1610 b- defN 24-Apr-18 07:57 migrations/0010_fix_corrupt_indexes.py
--rw-r--r--  2.0 unx     1843 b- defN 24-Apr-18 07:57 migrations/0011_materialize_labelset_ids.py
--rw-r--r--  2.0 unx     1443 b- defN 24-Apr-18 07:57 migrations/0012_rollover_shards.py
--rw-r--r--  2.0 unx     1024 b- defN 24-Apr-18 07:57 migrations/0013_rollover_shards.py
--rw-r--r--  2.0 unx     1382 b- defN 24-Apr-18 07:57 migrations/0014_rollover_shards.py
--rw-r--r--  2.0 unx     1462 b- defN 24-Apr-18 07:57 migrations/0015_targeted_rollover.py
--rw-r--r--  2.0 unx     2506 b- defN 24-Apr-18 07:57 migrations/0016_upgrade_to_paragraphs_v2.py
--rw-r--r--  2.0 unx     2100 b- defN 24-Apr-18 07:57 migrations/0017_multiple_writable_shards.py
--rw-r--r--  2.0 unx      835 b- defN 24-Apr-18 07:57 migrations/__init__.py
--rw-r--r--  2.0 unx      891 b- defN 24-Apr-18 07:57 nucliadb/__init__.py
--rw-r--r--  2.0 unx     3733 b- defN 24-Apr-18 07:57 nucliadb/health.py
--rw-r--r--  2.0 unx    10590 b- defN 24-Apr-18 07:57 nucliadb/learning_proxy.py
--rw-r--r--  2.0 unx     4806 b- defN 24-Apr-18 07:57 nucliadb/metrics_exporter.py
--rw-r--r--  2.0 unx     2272 b- defN 24-Apr-18 07:57 nucliadb/openapi.py
--rw-r--r--  2.0 unx        0 b- defN 24-Apr-18 07:57 nucliadb/py.typed
--rw-r--r--  2.0 unx      835 b- defN 24-Apr-18 07:57 nucliadb/common/__init__.py
--rw-r--r--  2.0 unx     4905 b- defN 24-Apr-18 07:57 nucliadb/common/locking.py
--rw-r--r--  2.0 unx      835 b- defN 24-Apr-18 07:57 nucliadb/common/cluster/__init__.py
--rw-r--r--  2.0 unx     4983 b- defN 24-Apr-18 07:57 nucliadb/common/cluster/base.py
--rw-r--r--  2.0 unx     1495 b- defN 24-Apr-18 07:57 nucliadb/common/cluster/exceptions.py
--rw-r--r--  2.0 unx     3658 b- defN 24-Apr-18 07:57 nucliadb/common/cluster/grpc_node_dummy.py
--rw-r--r--  2.0 unx     3429 b- defN 24-Apr-18 07:57 nucliadb/common/cluster/index_node.py
--rw-r--r--  2.0 unx    21095 b- defN 24-Apr-18 07:57 nucliadb/common/cluster/manager.py
--rw-r--r--  2.0 unx     8490 b- defN 24-Apr-18 07:57 nucliadb/common/cluster/rebalance.py
--rw-r--r--  2.0 unx    19449 b- defN 24-Apr-18 07:57 nucliadb/common/cluster/rollover.py
--rw-r--r--  2.0 unx     2713 b- defN 24-Apr-18 07:57 nucliadb/common/cluster/settings.py
--rw-r--r--  2.0 unx     5494 b- defN 24-Apr-18 07:57 nucliadb/common/cluster/utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-Apr-18 07:57 nucliadb/common/cluster/discovery/__init__.py
--rw-r--r--  2.0 unx     6553 b- defN 24-Apr-18 07:57 nucliadb/common/cluster/discovery/base.py
--rw-r--r--  2.0 unx    12518 b- defN 24-Apr-18 07:57 nucliadb/common/cluster/discovery/k8s.py
--rw-r--r--  2.0 unx     1957 b- defN 24-Apr-18 07:57 nucliadb/common/cluster/discovery/manual.py
--rw-r--r--  2.0 unx     1737 b- defN 24-Apr-18 07:57 nucliadb/common/cluster/discovery/single.py
--rw-r--r--  2.0 unx     1139 b- defN 24-Apr-18 07:57 nucliadb/common/cluster/discovery/types.py
--rw-r--r--  2.0 unx     2548 b- defN 24-Apr-18 07:57 nucliadb/common/cluster/discovery/utils.py
--rw-r--r--  2.0 unx      833 b- defN 24-Apr-18 07:57 nucliadb/common/cluster/standalone/__init__.py
--rw-r--r--  2.0 unx    13705 b- defN 24-Apr-18 07:57 nucliadb/common/cluster/standalone/grpc_node_binding.py
--rw-r--r--  2.0 unx     4683 b- defN 24-Apr-18 07:57 nucliadb/common/cluster/standalone/index_node.py
--rw-r--r--  2.0 unx     3444 b- defN 24-Apr-18 07:57 nucliadb/common/cluster/standalone/service.py
--rw-r--r--  2.0 unx     3386 b- defN 24-Apr-18 07:57 nucliadb/common/cluster/standalone/utils.py
--rw-r--r--  2.0 unx     3498 b- defN 24-Apr-18 07:57 nucliadb/common/context/__init__.py
--rw-r--r--  2.0 unx     1628 b- defN 24-Apr-18 07:57 nucliadb/common/context/fastapi.py
--rw-r--r--  2.0 unx     1813 b- defN 24-Apr-18 07:57 nucliadb/common/datamanagers/__init__.py
--rw-r--r--  2.0 unx     1451 b- defN 24-Apr-18 07:57 nucliadb/common/datamanagers/cluster.py
--rw-r--r--  2.0 unx     5383 b- defN 24-Apr-18 07:57 nucliadb/common/datamanagers/entities.py
--rw-r--r--  2.0 unx      883 b- defN 24-Apr-18 07:57 nucliadb/common/datamanagers/exceptions.py
--rw-r--r--  2.0 unx     2940 b- defN 24-Apr-18 07:57 nucliadb/common/datamanagers/kb.py
--rw-r--r--  2.0 unx     5389 b- defN 24-Apr-18 07:57 nucliadb/common/datamanagers/labels.py
--rw-r--r--  2.0 unx     1599 b- defN 24-Apr-18 07:57 nucliadb/common/datamanagers/processing.py
--rw-r--r--  2.0 unx     7637 b- defN 24-Apr-18 07:57 nucliadb/common/datamanagers/resources.py
--rw-r--r--  2.0 unx     5633 b- defN 24-Apr-18 07:57 nucliadb/common/datamanagers/rollover.py
--rw-r--r--  2.0 unx     1681 b- defN 24-Apr-18 07:57 nucliadb/common/datamanagers/utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-Apr-18 07:57 nucliadb/common/http_clients/__init__.py
--rw-r--r--  2.0 unx     2146 b- defN 24-Apr-18 07:57 nucliadb/common/http_clients/auth.py
--rw-r--r--  2.0 unx     1100 b- defN 24-Apr-18 07:57 nucliadb/common/http_clients/exceptions.py
--rw-r--r--  2.0 unx     7155 b- defN 24-Apr-18 07:57 nucliadb/common/http_clients/processing.py
--rw-r--r--  2.0 unx     1540 b- defN 24-Apr-18 07:57 nucliadb/common/http_clients/pypi.py
--rw-r--r--  2.0 unx     1551 b- defN 24-Apr-18 07:57 nucliadb/common/http_clients/utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-Apr-18 07:57 nucliadb/common/maindb/__init__.py
--rw-r--r--  2.0 unx     3449 b- defN 24-Apr-18 07:57 nucliadb/common/maindb/driver.py
--rw-r--r--  2.0 unx      946 b- defN 24-Apr-18 07:57 nucliadb/common/maindb/exceptions.py
--rw-r--r--  2.0 unx     6769 b- defN 24-Apr-18 07:57 nucliadb/common/maindb/local.py
--rw-r--r--  2.0 unx     8391 b- defN 24-Apr-18 07:57 nucliadb/common/maindb/pg.py
--rw-r--r--  2.0 unx     6053 b- defN 24-Apr-18 07:57 nucliadb/common/maindb/redis.py
--rw-r--r--  2.0 unx    14502 b- defN 24-Apr-18 07:57 nucliadb/common/maindb/tikv.py
--rw-r--r--  2.0 unx     4109 b- defN 24-Apr-18 07:57 nucliadb/common/maindb/utils.py
--rw-r--r--  2.0 unx      932 b- defN 24-Apr-18 07:57 nucliadb/export_import/__init__.py
--rw-r--r--  2.0 unx     6171 b- defN 24-Apr-18 07:57 nucliadb/export_import/datamanager.py
--rw-r--r--  2.0 unx     1949 b- defN 24-Apr-18 07:57 nucliadb/export_import/exceptions.py
--rw-r--r--  2.0 unx     7116 b- defN 24-Apr-18 07:57 nucliadb/export_import/exporter.py
--rw-r--r--  2.0 unx     4258 b- defN 24-Apr-18 07:57 nucliadb/export_import/importer.py
--rw-r--r--  2.0 unx     2063 b- defN 24-Apr-18 07:57 nucliadb/export_import/models.py
--rw-r--r--  2.0 unx     2571 b- defN 24-Apr-18 07:57 nucliadb/export_import/tasks.py
--rw-r--r--  2.0 unx    19270 b- defN 24-Apr-18 07:57 nucliadb/export_import/utils.py
--rw-r--r--  2.0 unx     1011 b- defN 24-Apr-18 07:57 nucliadb/ingest/__init__.py
--rw-r--r--  2.0 unx     7277 b- defN 24-Apr-18 07:57 nucliadb/ingest/app.py
--rw-r--r--  2.0 unx     1005 b- defN 24-Apr-18 07:57 nucliadb/ingest/cache.py
--rw-r--r--  2.0 unx     2484 b- defN 24-Apr-18 07:57 nucliadb/ingest/partitions.py
--rw-r--r--  2.0 unx    19541 b- defN 24-Apr-18 07:57 nucliadb/ingest/processing.py
--rw-r--r--  2.0 unx    20277 b- defN 24-Apr-18 07:57 nucliadb/ingest/serialize.py
--rw-r--r--  2.0 unx     3183 b- defN 24-Apr-18 07:57 nucliadb/ingest/settings.py
--rw-r--r--  2.0 unx     2314 b- defN 24-Apr-18 07:57 nucliadb/ingest/utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-Apr-18 07:57 nucliadb/ingest/consumer/__init__.py
--rw-r--r--  2.0 unx    11563 b- defN 24-Apr-18 07:57 nucliadb/ingest/consumer/auditing.py
--rw-r--r--  2.0 unx    12159 b- defN 24-Apr-18 07:57 nucliadb/ingest/consumer/consumer.py
--rw-r--r--  2.0 unx     3788 b- defN 24-Apr-18 07:57 nucliadb/ingest/consumer/materializer.py
--rw-r--r--  2.0 unx     1075 b- defN 24-Apr-18 07:57 nucliadb/ingest/consumer/metrics.py
--rw-r--r--  2.0 unx     9543 b- defN 24-Apr-18 07:57 nucliadb/ingest/consumer/pull.py
--rw-r--r--  2.0 unx     6935 b- defN 24-Apr-18 07:57 nucliadb/ingest/consumer/service.py
--rw-r--r--  2.0 unx     4331 b- defN 24-Apr-18 07:57 nucliadb/ingest/consumer/shard_creator.py
--rw-r--r--  2.0 unx     2656 b- defN 24-Apr-18 07:57 nucliadb/ingest/consumer/utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-Apr-18 07:57 nucliadb/ingest/fields/__init__.py
--rw-r--r--  2.0 unx    18433 b- defN 24-Apr-18 07:57 nucliadb/ingest/fields/base.py
--rw-r--r--  2.0 unx     6516 b- defN 24-Apr-18 07:57 nucliadb/ingest/fields/conversation.py
--rw-r--r--  2.0 unx     1223 b- defN 24-Apr-18 07:57 nucliadb/ingest/fields/date.py
--rw-r--r--  2.0 unx     1205 b- defN 24-Apr-18 07:57 nucliadb/ingest/fields/exceptions.py
--rw-r--r--  2.0 unx     5159 b- defN 24-Apr-18 07:57 nucliadb/ingest/fields/file.py
--rw-r--r--  2.0 unx     1547 b- defN 24-Apr-18 07:57 nucliadb/ingest/fields/generic.py
--rw-r--r--  2.0 unx     1235 b- defN 24-Apr-18 07:57 nucliadb/ingest/fields/keywordset.py
--rw-r--r--  2.0 unx     2250 b- defN 24-Apr-18 07:57 nucliadb/ingest/fields/layout.py
--rw-r--r--  2.0 unx     4084 b- defN 24-Apr-18 07:57 nucliadb/ingest/fields/link.py
--rw-r--r--  2.0 unx     1319 b- defN 24-Apr-18 07:57 nucliadb/ingest/fields/text.py
--rw-r--r--  2.0 unx      835 b- defN 24-Apr-18 07:57 nucliadb/ingest/orm/__init__.py
--rw-r--r--  2.0 unx    27582 b- defN 24-Apr-18 07:57 nucliadb/ingest/orm/brain.py
--rw-r--r--  2.0 unx    15758 b- defN 24-Apr-18 07:57 nucliadb/ingest/orm/entities.py
--rw-r--r--  2.0 unx     1279 b- defN 24-Apr-18 07:57 nucliadb/ingest/orm/exceptions.py
--rw-r--r--  2.0 unx    18865 b- defN 24-Apr-18 07:57 nucliadb/ingest/orm/knowledgebox.py
--rw-r--r--  2.0 unx     1096 b- defN 24-Apr-18 07:57 nucliadb/ingest/orm/metrics.py
--rw-r--r--  2.0 unx    60085 b- defN 24-Apr-18 07:57 nucliadb/ingest/orm/resource.py
--rw-r--r--  2.0 unx     1739 b- defN 24-Apr-18 07:57 nucliadb/ingest/orm/synonyms.py
--rw-r--r--  2.0 unx     3074 b- defN 24-Apr-18 07:57 nucliadb/ingest/orm/utils.py
--rw-r--r--  2.0 unx    26460 b- defN 24-Apr-18 07:57 nucliadb/ingest/orm/processor/__init__.py
--rw-r--r--  2.0 unx     1690 b- defN 24-Apr-18 07:57 nucliadb/ingest/orm/processor/sequence_manager.py
--rw-r--r--  2.0 unx     2057 b- defN 24-Apr-18 07:57 nucliadb/ingest/service/__init__.py
--rw-r--r--  2.0 unx      835 b- defN 24-Apr-18 07:57 nucliadb/ingest/service/exceptions.py
--rw-r--r--  2.0 unx    36594 b- defN 24-Apr-18 07:57 nucliadb/ingest/service/writer.py
--rw-r--r--  2.0 unx      835 b- defN 24-Apr-18 07:57 nucliadb/ingest/tests/__init__.py
--rw-r--r--  2.0 unx     1157 b- defN 24-Apr-18 07:57 nucliadb/ingest/tests/conftest.py
--rw-r--r--  2.0 unx    24068 b- defN 24-Apr-18 07:57 nucliadb/ingest/tests/fixtures.py
--rw-r--r--  2.0 unx    62843 b- defN 24-Apr-18 07:57 nucliadb/ingest/tests/vectors.py
--rw-r--r--  2.0 unx      835 b- defN 24-Apr-18 07:57 nucliadb/ingest/tests/integration/__init__.py
--rw-r--r--  2.0 unx      833 b- defN 24-Apr-18 07:57 nucliadb/ingest/tests/integration/consumer/__init__.py
--rw-r--r--  2.0 unx     2549 b- defN 24-Apr-18 07:57 nucliadb/ingest/tests/integration/consumer/test_auditing.py
--rw-r--r--  2.0 unx     2591 b- defN 24-Apr-18 07:57 nucliadb/ingest/tests/integration/consumer/test_materializer.py
--rw-r--r--  2.0 unx     4465 b- defN 24-Apr-18 07:57 nucliadb/ingest/tests/integration/consumer/test_pull.py
--rw-r--r--  2.0 unx     2763 b- defN 24-Apr-18 07:57 nucliadb/ingest/tests/integration/consumer/test_service.py
--rw-r--r--  2.0 unx     2019 b- defN 24-Apr-18 07:57 nucliadb/ingest/tests/integration/consumer/test_shard_creator.py
--rw-r--r--  2.0 unx      835 b- defN 24-Apr-18 07:57 nucliadb/ingest/tests/integration/ingest/__init__.py
--rw-r--r--  2.0 unx    27334 b- defN 24-Apr-18 07:57 nucliadb/ingest/tests/integration/ingest/test_ingest.py
--rw-r--r--  2.0 unx     3040 b- defN 24-Apr-18 07:57 nucliadb/ingest/tests/integration/ingest/test_processing_engine.py
--rw-r--r--  2.0 unx     8586 b- defN 24-Apr-18 07:57 nucliadb/ingest/tests/integration/ingest/test_relations.py
--rw-r--r--  2.0 unx      835 b- defN 24-Apr-18 07:57 nucliadb/ingest/tests/unit/__init__.py
--rw-r--r--  2.0 unx     1189 b- defN 24-Apr-18 07:57 nucliadb/ingest/tests/unit/test_cache.py
--rw-r--r--  2.0 unx     1432 b- defN 24-Apr-18 07:57 nucliadb/ingest/tests/unit/test_partitions.py
--rw-r--r--  2.0 unx     5807 b- defN 24-Apr-18 07:57 nucliadb/ingest/tests/unit/test_processing.py
--rw-r--r--  2.0 unx      978 b- defN 24-Apr-18 07:57 nucliadb/ingest/tests/unit/test_settings.py
--rw-r--r--  2.0 unx      833 b- defN 24-Apr-18 07:57 nucliadb/ingest/tests/unit/consumer/__init__.py
--rw-r--r--  2.0 unx     3981 b- defN 24-Apr-18 07:57 nucliadb/ingest/tests/unit/consumer/test_auditing.py
--rw-r--r--  2.0 unx     2472 b- defN 24-Apr-18 07:57 nucliadb/ingest/tests/unit/consumer/test_consumer.py
--rw-r--r--  2.0 unx     2063 b- defN 24-Apr-18 07:57 nucliadb/ingest/tests/unit/consumer/test_pull.py
--rw-r--r--  2.0 unx     4075 b- defN 24-Apr-18 07:57 nucliadb/ingest/tests/unit/consumer/test_shard_creator.py
--rw-r--r--  2.0 unx     1934 b- defN 24-Apr-18 07:57 nucliadb/ingest/tests/unit/consumer/test_utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-Apr-18 07:57 nucliadb/ingest/tests/unit/orm/__init__.py
--rw-r--r--  2.0 unx     9876 b- defN 24-Apr-18 07:57 nucliadb/ingest/tests/unit/orm/test_brain.py
--rw-r--r--  2.0 unx     4045 b- defN 24-Apr-18 07:57 nucliadb/ingest/tests/unit/orm/test_processor.py
--rw-r--r--  2.0 unx     8965 b- defN 24-Apr-18 07:57 nucliadb/ingest/tests/unit/orm/test_resource.py
--rw-r--r--  2.0 unx     2216 b- defN 24-Apr-18 07:57 nucliadb/middleware/__init__.py
--rw-r--r--  2.0 unx     3912 b- defN 24-Apr-18 07:57 nucliadb/middleware/transaction.py
--rw-r--r--  2.0 unx      835 b- defN 24-Apr-18 07:57 nucliadb/migrator/__init__.py
--rw-r--r--  2.0 unx     2119 b- defN 24-Apr-18 07:57 nucliadb/migrator/command.py
--rw-r--r--  2.0 unx     1334 b- defN 24-Apr-18 07:57 nucliadb/migrator/context.py
--rw-r--r--  2.0 unx     5104 b- defN 24-Apr-18 07:57 nucliadb/migrator/datamanager.py
--rw-r--r--  2.0 unx      889 b- defN 24-Apr-18 07:57 nucliadb/migrator/exceptions.py
--rw-r--r--  2.0 unx     9237 b- defN 24-Apr-18 07:57 nucliadb/migrator/migrator.py
--rw-r--r--  2.0 unx     1145 b- defN 24-Apr-18 07:57 nucliadb/migrator/models.py
--rw-r--r--  2.0 unx     1110 b- defN 24-Apr-18 07:57 nucliadb/migrator/settings.py
--rw-r--r--  2.0 unx     2346 b- defN 24-Apr-18 07:57 nucliadb/migrator/utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-Apr-18 07:57 nucliadb/models/__init__.py
--rw-r--r--  2.0 unx     1599 b- defN 24-Apr-18 07:57 nucliadb/models/responses.py
--rw-r--r--  2.0 unx     6041 b- defN 24-Apr-18 07:57 nucliadb/purge/__init__.py
--rw-r--r--  2.0 unx     9364 b- defN 24-Apr-18 07:57 nucliadb/purge/orphan_shards.py
--rw-r--r--  2.0 unx     1328 b- defN 24-Apr-18 07:57 nucliadb/reader/__init__.py
--rw-r--r--  2.0 unx     3709 b- defN 24-Apr-18 07:57 nucliadb/reader/app.py
--rw-r--r--  2.0 unx     1366 b- defN 24-Apr-18 07:57 nucliadb/reader/lifecycle.py
--rw-r--r--  2.0 unx     1031 b- defN 24-Apr-18 07:57 nucliadb/reader/openapi.py
--rw-r--r--  2.0 unx     1447 b- defN 24-Apr-18 07:57 nucliadb/reader/run.py
--rw-r--r--  2.0 unx      872 b- defN 24-Apr-18 07:57 nucliadb/reader/api/__init__.py
--rw-r--r--  2.0 unx     2434 b- defN 24-Apr-18 07:57 nucliadb/reader/api/models.py
--rw-r--r--  2.0 unx     1110 b- defN 24-Apr-18 07:57 nucliadb/reader/api/v1/__init__.py
--rw-r--r--  2.0 unx    12368 b- defN 24-Apr-18 07:57 nucliadb/reader/api/v1/download.py
--rw-r--r--  2.0 unx     6450 b- defN 24-Apr-18 07:57 nucliadb/reader/api/v1/export_import.py
--rw-r--r--  2.0 unx     3632 b- defN 24-Apr-18 07:57 nucliadb/reader/api/v1/knowledgebox.py
--rw-r--r--  2.0 unx     2093 b- defN 24-Apr-18 07:57 nucliadb/reader/api/v1/learning_collector.py
--rw-r--r--  2.0 unx     4454 b- defN 24-Apr-18 07:57 nucliadb/reader/api/v1/learning_config.py
--rw-r--r--  2.0 unx    13928 b- defN 24-Apr-18 07:57 nucliadb/reader/api/v1/resource.py
--rw-r--r--  2.0 unx     1011 b- defN 24-Apr-18 07:57 nucliadb/reader/api/v1/router.py
--rw-r--r--  2.0 unx    13882 b- defN 24-Apr-18 07:57 nucliadb/reader/api/v1/services.py
--rw-r--r--  2.0 unx      835 b- defN 24-Apr-18 07:57 nucliadb/reader/reader/__init__.py
--rw-r--r--  2.0 unx     8155 b- defN 24-Apr-18 07:57 nucliadb/reader/reader/notifications.py
--rw-r--r--  2.0 unx      835 b- defN 24-Apr-18 07:57 nucliadb/reader/tests/__init__.py
--rw-r--r--  2.0 unx     1224 b- defN 24-Apr-18 07:57 nucliadb/reader/tests/conftest.py
--rw-r--r--  2.0 unx     4345 b- defN 24-Apr-18 07:57 nucliadb/reader/tests/fixtures.py
--rw-r--r--  2.0 unx     2748 b- defN 24-Apr-18 07:57 nucliadb/reader/tests/test_list_resources.py
--rw-r--r--  2.0 unx    10199 b- defN 24-Apr-18 07:57 nucliadb/reader/tests/test_reader_file_download.py
--rw-r--r--  2.0 unx    10586 b- defN 24-Apr-18 07:57 nucliadb/reader/tests/test_reader_resource.py
--rw-r--r--  2.0 unx     6535 b- defN 24-Apr-18 07:57 nucliadb/reader/tests/test_reader_resource_field.py
--rw-r--r--  2.0 unx     1535 b- defN 24-Apr-18 07:57 nucliadb/search/__init__.py
--rw-r--r--  2.0 unx     4905 b- defN 24-Apr-18 07:57 nucliadb/search/app.py
--rw-r--r--  2.0 unx     1956 b- defN 24-Apr-18 07:57 nucliadb/search/lifecycle.py
--rw-r--r--  2.0 unx     1016 b- defN 24-Apr-18 07:57 nucliadb/search/openapi.py
--rw-r--r--  2.0 unx    19798 b- defN 24-Apr-18 07:57 nucliadb/search/predict.py
--rw-r--r--  2.0 unx     1402 b- defN 24-Apr-18 07:57 nucliadb/search/run.py
--rw-r--r--  2.0 unx     1193 b- defN 24-Apr-18 07:57 nucliadb/search/settings.py
--rw-r--r--  2.0 unx     1037 b- defN 24-Apr-18 07:57 nucliadb/search/utilities.py
--rw-r--r--  2.0 unx      835 b- defN 24-Apr-18 07:57 nucliadb/search/api/__init__.py
--rw-r--r--  2.0 unx     1272 b- defN 24-Apr-18 07:57 nucliadb/search/api/v1/__init__.py
--rw-r--r--  2.0 unx     9913 b- defN 24-Apr-18 07:57 nucliadb/search/api/v1/chat.py
--rw-r--r--  2.0 unx     2665 b- defN 24-Apr-18 07:57 nucliadb/search/api/v1/feedback.py
--rw-r--r--  2.0 unx     8804 b- defN 24-Apr-18 07:57 nucliadb/search/api/v1/find.py
--rw-r--r--  2.0 unx     7026 b- defN 24-Apr-18 07:57 nucliadb/search/api/v1/knowledgebox.py
--rw-r--r--  2.0 unx     3041 b- defN 24-Apr-18 07:57 nucliadb/search/api/v1/predict_proxy.py
--rw-r--r--  2.0 unx      988 b- defN 24-Apr-18 07:57 nucliadb/search/api/v1/router.py
--rw-r--r--  2.0 unx    18359 b- defN 24-Apr-18 07:57 nucliadb/search/api/v1/search.py
--rw-r--r--  2.0 unx     5928 b- defN 24-Apr-18 07:57 nucliadb/search/api/v1/suggest.py
--rw-r--r--  2.0 unx     2536 b- defN 24-Apr-18 07:57 nucliadb/search/api/v1/summarize.py
--rw-r--r--  2.0 unx     1412 b- defN 24-Apr-18 07:57 nucliadb/search/api/v1/utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-Apr-18 07:57 nucliadb/search/api/v1/resource/__init__.py
--rw-r--r--  2.0 unx     6095 b- defN 24-Apr-18 07:57 nucliadb/search/api/v1/resource/ask.py
--rw-r--r--  2.0 unx     5887 b- defN 24-Apr-18 07:57 nucliadb/search/api/v1/resource/chat.py
--rw-r--r--  2.0 unx     5293 b- defN 24-Apr-18 07:57 nucliadb/search/api/v1/resource/search.py
--rw-r--r--  2.0 unx      833 b- defN 24-Apr-18 07:57 nucliadb/search/requesters/__init__.py
--rw-r--r--  2.0 unx     9070 b- defN 24-Apr-18 07:57 nucliadb/search/requesters/utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-Apr-18 07:57 nucliadb/search/search/__init__.py
--rw-r--r--  2.0 unx     2746 b- defN 24-Apr-18 07:57 nucliadb/search/search/cache.py
--rw-r--r--  2.0 unx     1154 b- defN 24-Apr-18 07:57 nucliadb/search/search/exceptions.py
--rw-r--r--  2.0 unx     5465 b- defN 24-Apr-18 07:57 nucliadb/search/search/fetch.py
--rw-r--r--  2.0 unx     6513 b- defN 24-Apr-18 07:57 nucliadb/search/search/filters.py
--rw-r--r--  2.0 unx     4646 b- defN 24-Apr-18 07:57 nucliadb/search/search/find.py
--rw-r--r--  2.0 unx    17152 b- defN 24-Apr-18 07:57 nucliadb/search/search/find_merge.py
--rw-r--r--  2.0 unx    21118 b- defN 24-Apr-18 07:57 nucliadb/search/search/merge.py
--rw-r--r--  2.0 unx     1130 b- defN 24-Apr-18 07:57 nucliadb/search/search/metrics.py
--rw-r--r--  2.0 unx     8698 b- defN 24-Apr-18 07:57 nucliadb/search/search/paragraphs.py
--rw-r--r--  2.0 unx     3026 b- defN 24-Apr-18 07:57 nucliadb/search/search/predict_proxy.py
--rw-r--r--  2.0 unx    32297 b- defN 24-Apr-18 07:57 nucliadb/search/search/query.py
--rw-r--r--  2.0 unx     3149 b- defN 24-Apr-18 07:57 nucliadb/search/search/shards.py
--rw-r--r--  2.0 unx     5101 b- defN 24-Apr-18 07:57 nucliadb/search/search/summarize.py
--rw-r--r--  2.0 unx     2438 b- defN 24-Apr-18 07:57 nucliadb/search/search/utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-Apr-18 07:57 nucliadb/search/search/chat/__init__.py
--rw-r--r--  2.0 unx     2058 b- defN 24-Apr-18 07:57 nucliadb/search/search/chat/images.py
--rw-r--r--  2.0 unx    20793 b- defN 24-Apr-18 07:57 nucliadb/search/search/chat/prompt.py
--rw-r--r--  2.0 unx    15347 b- defN 24-Apr-18 07:57 nucliadb/search/search/chat/query.py
--rw-r--r--  2.0 unx      835 b- defN 24-Apr-18 07:57 nucliadb/search/tests/__init__.py
--rw-r--r--  2.0 unx     1295 b- defN 24-Apr-18 07:57 nucliadb/search/tests/conftest.py
--rw-r--r--  2.0 unx     6578 b- defN 24-Apr-18 07:57 nucliadb/search/tests/fixtures.py
--rw-r--r--  2.0 unx    15529 b- defN 24-Apr-18 07:57 nucliadb/search/tests/node.py
--rw-r--r--  2.0 unx      833 b- defN 24-Apr-18 07:57 nucliadb/search/tests/unit/__init__.py
--rw-r--r--  2.0 unx     2649 b- defN 24-Apr-18 07:57 nucliadb/search/tests/unit/test_app.py
--rw-r--r--  2.0 unx     3374 b- defN 24-Apr-18 07:57 nucliadb/search/tests/unit/test_find_merge.py
--rw-r--r--  2.0 unx     1400 b- defN 24-Apr-18 07:57 nucliadb/search/tests/unit/test_merge.py
--rw-r--r--  2.0 unx    17080 b- defN 24-Apr-18 07:57 nucliadb/search/tests/unit/test_predict.py
--rw-r--r--  2.0 unx     1317 b- defN 24-Apr-18 07:57 nucliadb/search/tests/unit/test_run.py
--rw-r--r--  2.0 unx      835 b- defN 24-Apr-18 07:57 nucliadb/search/tests/unit/api/__init__.py
--rw-r--r--  2.0 unx      835 b- defN 24-Apr-18 07:57 nucliadb/search/tests/unit/api/v1/__init__.py
--rw-r--r--  2.0 unx     2966 b- defN 24-Apr-18 07:57 nucliadb/search/tests/unit/api/v1/test_chat.py
--rw-r--r--  2.0 unx     2865 b- defN 24-Apr-18 07:57 nucliadb/search/tests/unit/api/v1/test_predict_proxy.py
--rw-r--r--  2.0 unx     2901 b- defN 24-Apr-18 07:57 nucliadb/search/tests/unit/api/v1/test_summarize.py
--rw-r--r--  2.0 unx      835 b- defN 24-Apr-18 07:57 nucliadb/search/tests/unit/api/v1/resource/__init__.py
--rw-r--r--  2.0 unx     2411 b- defN 24-Apr-18 07:57 nucliadb/search/tests/unit/api/v1/resource/test_ask.py
--rw-r--r--  2.0 unx     3040 b- defN 24-Apr-18 07:57 nucliadb/search/tests/unit/api/v1/resource/test_chat.py
--rw-r--r--  2.0 unx      833 b- defN 24-Apr-18 07:57 nucliadb/search/tests/unit/search/__init__.py
--rw-r--r--  2.0 unx     8567 b- defN 24-Apr-18 07:57 nucliadb/search/tests/unit/search/test_chat_prompt.py
--rw-r--r--  2.0 unx     3736 b- defN 24-Apr-18 07:57 nucliadb/search/tests/unit/search/test_fetch.py
--rw-r--r--  2.0 unx     4306 b- defN 24-Apr-18 07:57 nucliadb/search/tests/unit/search/test_filters.py
--rw-r--r--  2.0 unx     4492 b- defN 24-Apr-18 07:57 nucliadb/search/tests/unit/search/test_paragraphs.py
--rw-r--r--  2.0 unx     3496 b- defN 24-Apr-18 07:57 nucliadb/search/tests/unit/search/test_predict_proxy.py
--rw-r--r--  2.0 unx     7001 b- defN 24-Apr-18 07:57 nucliadb/search/tests/unit/search/test_query.py
--rw-r--r--  2.0 unx      833 b- defN 24-Apr-18 07:57 nucliadb/search/tests/unit/search/requesters/__init__.py
--rw-r--r--  2.0 unx     6455 b- defN 24-Apr-18 07:57 nucliadb/search/tests/unit/search/requesters/test_utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-Apr-18 07:57 nucliadb/search/tests/unit/search/search/__init__.py
--rw-r--r--  2.0 unx     1759 b- defN 24-Apr-18 07:57 nucliadb/search/tests/unit/search/search/test_shards.py
--rw-r--r--  2.0 unx     2511 b- defN 24-Apr-18 07:57 nucliadb/search/tests/unit/search/search/test_utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-Apr-18 07:57 nucliadb/standalone/__init__.py
--rw-r--r--  2.0 unx     6746 b- defN 24-Apr-18 07:57 nucliadb/standalone/api_router.py
--rw-r--r--  2.0 unx     5763 b- defN 24-Apr-18 07:57 nucliadb/standalone/app.py
--rw-r--r--  2.0 unx     7800 b- defN 24-Apr-18 07:57 nucliadb/standalone/auth.py
--rw-r--r--  2.0 unx     5309 b- defN 24-Apr-18 07:57 nucliadb/standalone/config.py
--rw-r--r--  2.0 unx     6930 b- defN 24-Apr-18 07:57 nucliadb/standalone/introspect.py
--rw-r--r--  2.0 unx     2488 b- defN 24-Apr-18 07:57 nucliadb/standalone/lifecycle.py
--rw-r--r--  2.0 unx     1317 b- defN 24-Apr-18 07:57 nucliadb/standalone/purge.py
--rw-r--r--  2.0 unx     5336 b- defN 24-Apr-18 07:57 nucliadb/standalone/run.py
--rw-r--r--  2.0 unx     5781 b- defN 24-Apr-18 07:57 nucliadb/standalone/settings.py
--rw-r--r--  2.0 unx     3132 b- defN 24-Apr-18 07:57 nucliadb/standalone/versions.py
--rw-r--r--  2.0 unx     2285 b- defN 24-Apr-18 07:57 nucliadb/standalone/static/favicon.ico
--rw-r--r--  2.0 unx     3833 b- defN 24-Apr-18 07:57 nucliadb/standalone/static/index.html
--rw-r--r--  2.0 unx     2639 b- defN 24-Apr-18 07:57 nucliadb/standalone/static/logo.svg
--rw-r--r--  2.0 unx      835 b- defN 24-Apr-18 07:57 nucliadb/standalone/tests/__init__.py
--rw-r--r--  2.0 unx     1294 b- defN 24-Apr-18 07:57 nucliadb/standalone/tests/conftest.py
--rw-r--r--  2.0 unx     1319 b- defN 24-Apr-18 07:57 nucliadb/standalone/tests/fixtures.py
--rw-r--r--  2.0 unx      833 b- defN 24-Apr-18 07:57 nucliadb/standalone/tests/unit/__init__.py
--rw-r--r--  2.0 unx     1722 b- defN 24-Apr-18 07:57 nucliadb/standalone/tests/unit/test_api_router.py
--rw-r--r--  2.0 unx     5509 b- defN 24-Apr-18 07:57 nucliadb/standalone/tests/unit/test_auth.py
--rw-r--r--  2.0 unx     1334 b- defN 24-Apr-18 07:57 nucliadb/standalone/tests/unit/test_introspect.py
--rw-r--r--  2.0 unx     1472 b- defN 24-Apr-18 07:57 nucliadb/standalone/tests/unit/test_run.py
--rw-r--r--  2.0 unx     1972 b- defN 24-Apr-18 07:57 nucliadb/standalone/tests/unit/test_versions.py
--rw-r--r--  2.0 unx     1037 b- defN 24-Apr-18 07:57 nucliadb/tasks/__init__.py
--rw-r--r--  2.0 unx     7655 b- defN 24-Apr-18 07:57 nucliadb/tasks/consumer.py
--rw-r--r--  2.0 unx      924 b- defN 24-Apr-18 07:57 nucliadb/tasks/logger.py
--rw-r--r--  2.0 unx     1378 b- defN 24-Apr-18 07:57 nucliadb/tasks/models.py
--rw-r--r--  2.0 unx     3457 b- defN 24-Apr-18 07:57 nucliadb/tasks/producer.py
--rw-r--r--  2.0 unx     1753 b- defN 24-Apr-18 07:57 nucliadb/tasks/registry.py
--rw-r--r--  2.0 unx     1360 b- defN 24-Apr-18 07:57 nucliadb/tasks/utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-Apr-18 07:57 nucliadb/tests/__init__.py
--rw-r--r--  2.0 unx     1229 b- defN 24-Apr-18 07:57 nucliadb/tests/conftest.py
--rw-r--r--  2.0 unx    22365 b- defN 24-Apr-18 07:57 nucliadb/tests/fixtures.py
--rw-r--r--  2.0 unx     7549 b- defN 24-Apr-18 07:57 nucliadb/tests/tikv.py
--rw-r--r--  2.0 unx      835 b- defN 24-Apr-18 07:57 nucliadb/tests/benchmarks/__init__.py
--rw-r--r--  2.0 unx     3032 b- defN 24-Apr-18 07:57 nucliadb/tests/benchmarks/test_search.py
--rw-r--r--  2.0 unx      919 b- defN 24-Apr-18 07:57 nucliadb/tests/knowledgeboxes/__init__.py
--rw-r--r--  2.0 unx     7002 b- defN 24-Apr-18 07:57 nucliadb/tests/knowledgeboxes/philosophy_books.py
--rw-r--r--  2.0 unx     3037 b- defN 24-Apr-18 07:57 nucliadb/tests/knowledgeboxes/ten_dummy_resources.py
--rw-r--r--  2.0 unx      835 b- defN 24-Apr-18 07:57 nucliadb/tests/migrations/__init__.py
--rw-r--r--  2.0 unx     2878 b- defN 24-Apr-18 07:57 nucliadb/tests/migrations/test_migration_0017.py
--rw-r--r--  2.0 unx      835 b- defN 24-Apr-18 07:57 nucliadb/tests/unit/__init__.py
--rw-r--r--  2.0 unx     1487 b- defN 24-Apr-18 07:57 nucliadb/tests/unit/test_field_ids.py
--rw-r--r--  2.0 unx     2758 b- defN 24-Apr-18 07:57 nucliadb/tests/unit/test_health.py
--rw-r--r--  2.0 unx     1543 b- defN 24-Apr-18 07:57 nucliadb/tests/unit/test_kb_slugs.py
--rw-r--r--  2.0 unx     7892 b- defN 24-Apr-18 07:57 nucliadb/tests/unit/test_learning_proxy.py
--rw-r--r--  2.0 unx     2642 b- defN 24-Apr-18 07:57 nucliadb/tests/unit/test_metrics_exporter.py
--rw-r--r--  2.0 unx     1341 b- defN 24-Apr-18 07:57 nucliadb/tests/unit/test_openapi.py
--rw-r--r--  2.0 unx     3656 b- defN 24-Apr-18 07:57 nucliadb/tests/unit/test_purge.py
--rw-r--r--  2.0 unx      835 b- defN 24-Apr-18 07:57 nucliadb/tests/unit/common/__init__.py
--rw-r--r--  2.0 unx     1268 b- defN 24-Apr-18 07:57 nucliadb/tests/unit/common/test_context.py
--rw-r--r--  2.0 unx      835 b- defN 24-Apr-18 07:57 nucliadb/tests/unit/common/cluster/__init__.py
--rw-r--r--  2.0 unx    11955 b- defN 24-Apr-18 07:57 nucliadb/tests/unit/common/cluster/test_cluster.py
--rw-r--r--  2.0 unx     5387 b- defN 24-Apr-18 07:57 nucliadb/tests/unit/common/cluster/test_kb_shard_manager.py
--rw-r--r--  2.0 unx     9470 b- defN 24-Apr-18 07:57 nucliadb/tests/unit/common/cluster/test_rollover.py
--rw-r--r--  2.0 unx      835 b- defN 24-Apr-18 07:57 nucliadb/tests/unit/common/cluster/discovery/__init__.py
--rw-r--r--  2.0 unx     5584 b- defN 24-Apr-18 07:57 nucliadb/tests/unit/common/cluster/discovery/test_k8s.py
--rw-r--r--  2.0 unx      833 b- defN 24-Apr-18 07:57 nucliadb/tests/unit/common/cluster/standalone/__init__.py
--rw-r--r--  2.0 unx     3750 b- defN 24-Apr-18 07:57 nucliadb/tests/unit/common/cluster/standalone/test_service.py
--rw-r--r--  2.0 unx     2114 b- defN 24-Apr-18 07:57 nucliadb/tests/unit/common/cluster/standalone/test_utils.py
--rw-r--r--  2.0 unx      833 b- defN 24-Apr-18 07:57 nucliadb/tests/unit/common/maindb/__init__.py
--rw-r--r--  2.0 unx     3579 b- defN 24-Apr-18 07:57 nucliadb/tests/unit/common/maindb/test_driver.py
--rw-r--r--  2.0 unx     1869 b- defN 24-Apr-18 07:57 nucliadb/tests/unit/common/maindb/test_tikv.py
--rw-r--r--  2.0 unx     2998 b- defN 24-Apr-18 07:57 nucliadb/tests/unit/common/maindb/test_utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-Apr-18 07:57 nucliadb/tests/unit/export_import/__init__.py
--rw-r--r--  2.0 unx     1435 b- defN 24-Apr-18 07:57 nucliadb/tests/unit/export_import/test_datamanager.py
--rw-r--r--  2.0 unx     9706 b- defN 24-Apr-18 07:57 nucliadb/tests/unit/export_import/test_utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-Apr-18 07:57 nucliadb/tests/unit/migrator/__init__.py
--rw-r--r--  2.0 unx     3233 b- defN 24-Apr-18 07:57 nucliadb/tests/unit/migrator/test_migrator.py
--rw-r--r--  2.0 unx      835 b- defN 24-Apr-18 07:57 nucliadb/tests/unit/tasks/__init__.py
--rw-r--r--  2.0 unx     1375 b- defN 24-Apr-18 07:57 nucliadb/tests/unit/tasks/conftest.py
--rw-r--r--  2.0 unx     2714 b- defN 24-Apr-18 07:57 nucliadb/tests/unit/tasks/test_consumer.py
--rw-r--r--  2.0 unx     3189 b- defN 24-Apr-18 07:57 nucliadb/tests/unit/tasks/test_producer.py
--rw-r--r--  2.0 unx     1827 b- defN 24-Apr-18 07:57 nucliadb/tests/unit/tasks/test_tasks.py
--rw-r--r--  2.0 unx     2507 b- defN 24-Apr-18 07:57 nucliadb/tests/utils/__init__.py
--rw-r--r--  2.0 unx     1797 b- defN 24-Apr-18 07:57 nucliadb/tests/utils/aiohttp_session.py
--rw-r--r--  2.0 unx     2533 b- defN 24-Apr-18 07:57 nucliadb/tests/utils/entities.py
--rw-r--r--  2.0 unx     6145 b- defN 24-Apr-18 07:57 nucliadb/tests/utils/broker_messages/__init__.py
--rw-r--r--  2.0 unx     6795 b- defN 24-Apr-18 07:57 nucliadb/tests/utils/broker_messages/fields.py
--rw-r--r--  2.0 unx     1196 b- defN 24-Apr-18 07:57 nucliadb/tests/utils/broker_messages/helpers.py
--rw-r--r--  2.0 unx     1325 b- defN 24-Apr-18 07:57 nucliadb/train/__init__.py
--rw-r--r--  2.0 unx     3530 b- defN 24-Apr-18 07:57 nucliadb/train/app.py
--rw-r--r--  2.0 unx     3800 b- defN 24-Apr-18 07:57 nucliadb/train/generator.py
--rw-r--r--  2.0 unx     1698 b- defN 24-Apr-18 07:57 nucliadb/train/lifecycle.py
--rw-r--r--  2.0 unx     1198 b- defN 24-Apr-18 07:57 nucliadb/train/models.py
--rw-r--r--  2.0 unx     5706 b- defN 24-Apr-18 07:57 nucliadb/train/nodes.py
--rw-r--r--  2.0 unx     1400 b- defN 24-Apr-18 07:57 nucliadb/train/run.py
--rw-r--r--  2.0 unx     5926 b- defN 24-Apr-18 07:57 nucliadb/train/servicer.py
--rw-r--r--  2.0 unx     1415 b- defN 24-Apr-18 07:57 nucliadb/train/settings.py
--rw-r--r--  2.0 unx     1496 b- defN 24-Apr-18 07:57 nucliadb/train/types.py
--rw-r--r--  2.0 unx     3265 b- defN 24-Apr-18 07:57 nucliadb/train/upload.py
--rw-r--r--  2.0 unx     6420 b- defN 24-Apr-18 07:57 nucliadb/train/uploader.py
--rw-r--r--  2.0 unx     3179 b- defN 24-Apr-18 07:57 nucliadb/train/utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-Apr-18 07:57 nucliadb/train/api/__init__.py
--rw-r--r--  2.0 unx     1479 b- defN 24-Apr-18 07:57 nucliadb/train/api/utils.py
--rw-r--r--  2.0 unx      928 b- defN 24-Apr-18 07:57 nucliadb/train/api/v1/__init__.py
--rw-r--r--  2.0 unx     2065 b- defN 24-Apr-18 07:57 nucliadb/train/api/v1/check.py
--rw-r--r--  2.0 unx      910 b- defN 24-Apr-18 07:57 nucliadb/train/api/v1/router.py
--rw-r--r--  2.0 unx     1905 b- defN 24-Apr-18 07:57 nucliadb/train/api/v1/shards.py
--rw-r--r--  2.0 unx     2129 b- defN 24-Apr-18 07:57 nucliadb/train/api/v1/trainset.py
--rw-r--r--  2.0 unx      835 b- defN 24-Apr-18 07:57 nucliadb/train/generators/__init__.py
--rw-r--r--  2.0 unx     3723 b- defN 24-Apr-18 07:57 nucliadb/train/generators/field_classifier.py
--rw-r--r--  2.0 unx     6712 b- defN 24-Apr-18 07:57 nucliadb/train/generators/image_classifier.py
--rw-r--r--  2.0 unx     2789 b- defN 24-Apr-18 07:57 nucliadb/train/generators/paragraph_classifier.py
--rw-r--r--  2.0 unx     3590 b- defN 24-Apr-18 07:57 nucliadb/train/generators/paragraph_streaming.py
--rw-r--r--  2.0 unx     5372 b- defN 24-Apr-18 07:57 nucliadb/train/generators/question_answer_streaming.py
--rw-r--r--  2.0 unx     5160 b- defN 24-Apr-18 07:57 nucliadb/train/generators/sentence_classifier.py
--rw-r--r--  2.0 unx    10446 b- defN 24-Apr-18 07:57 nucliadb/train/generators/token_classifier.py
--rw-r--r--  2.0 unx     3877 b- defN 24-Apr-18 07:57 nucliadb/train/generators/utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-Apr-18 07:57 nucliadb/train/tests/__init__.py
--rw-r--r--  2.0 unx     1125 b- defN 24-Apr-18 07:57 nucliadb/train/tests/conftest.py
--rw-r--r--  2.0 unx    11053 b- defN 24-Apr-18 07:57 nucliadb/train/tests/fixtures.py
--rw-r--r--  2.0 unx     4598 b- defN 24-Apr-18 07:57 nucliadb/train/tests/test_field_classification.py
--rw-r--r--  2.0 unx     2729 b- defN 24-Apr-18 07:57 nucliadb/train/tests/test_get_entities.py
--rw-r--r--  2.0 unx     1876 b- defN 24-Apr-18 07:57 nucliadb/train/tests/test_get_info.py
--rw-r--r--  2.0 unx     1382 b- defN 24-Apr-18 07:57 nucliadb/train/tests/test_get_ontology.py
--rw-r--r--  2.0 unx     2417 b- defN 24-Apr-18 07:57 nucliadb/train/tests/test_get_ontology_count.py
--rw-r--r--  2.0 unx     7669 b- defN 24-Apr-18 07:57 nucliadb/train/tests/test_image_classification.py
--rw-r--r--  2.0 unx     1416 b- defN 24-Apr-18 07:57 nucliadb/train/tests/test_list_fields.py
--rw-r--r--  2.0 unx     2944 b- defN 24-Apr-18 07:57 nucliadb/train/tests/test_list_paragraphs.py
--rw-r--r--  2.0 unx     1423 b- defN 24-Apr-18 07:57 nucliadb/train/tests/test_list_resources.py
--rw-r--r--  2.0 unx     2947 b- defN 24-Apr-18 07:57 nucliadb/train/tests/test_list_sentences.py
--rw-r--r--  2.0 unx     4645 b- defN 24-Apr-18 07:57 nucliadb/train/tests/test_paragraph_classification.py
--rw-r--r--  2.0 unx     4320 b- defN 24-Apr-18 07:57 nucliadb/train/tests/test_paragraph_streaming.py
--rw-r--r--  2.0 unx     8751 b- defN 24-Apr-18 07:57 nucliadb/train/tests/test_question_answer_streaming.py
--rw-r--r--  2.0 unx     5051 b- defN 24-Apr-18 07:57 nucliadb/train/tests/test_sentence_classification.py
--rw-r--r--  2.0 unx     5583 b- defN 24-Apr-18 07:57 nucliadb/train/tests/test_token_classification.py
--rw-r--r--  2.0 unx     3324 b- defN 24-Apr-18 07:57 nucliadb/train/tests/utils.py
--rw-r--r--  2.0 unx     1328 b- defN 24-Apr-18 07:57 nucliadb/writer/__init__.py
--rw-r--r--  2.0 unx     4268 b- defN 24-Apr-18 07:57 nucliadb/writer/app.py
--rw-r--r--  2.0 unx    19435 b- defN 24-Apr-18 07:57 nucliadb/writer/back_pressure.py
--rw-r--r--  2.0 unx      972 b- defN 24-Apr-18 07:57 nucliadb/writer/exceptions.py
--rw-r--r--  2.0 unx     1953 b- defN 24-Apr-18 07:57 nucliadb/writer/lifecycle.py
--rw-r--r--  2.0 unx     1032 b- defN 24-Apr-18 07:57 nucliadb/writer/openapi.py
--rw-r--r--  2.0 unx     1448 b- defN 24-Apr-18 07:57 nucliadb/writer/run.py
--rw-r--r--  2.0 unx     3074 b- defN 24-Apr-18 07:57 nucliadb/writer/settings.py
--rw-r--r--  2.0 unx     1036 b- defN 24-Apr-18 07:57 nucliadb/writer/utilities.py
--rw-r--r--  2.0 unx     1948 b- defN 24-Apr-18 07:57 nucliadb/writer/vectors.py
--rw-r--r--  2.0 unx      835 b- defN 24-Apr-18 07:57 nucliadb/writer/api/__init__.py
--rw-r--r--  2.0 unx     1429 b- defN 24-Apr-18 07:57 nucliadb/writer/api/constants.py
--rw-r--r--  2.0 unx     1095 b- defN 24-Apr-18 07:57 nucliadb/writer/api/v1/__init__.py
--rw-r--r--  2.0 unx     6565 b- defN 24-Apr-18 07:57 nucliadb/writer/api/v1/export_import.py
--rw-r--r--  2.0 unx    28320 b- defN 24-Apr-18 07:57 nucliadb/writer/api/v1/field.py
--rw-r--r--  2.0 unx     5239 b- defN 24-Apr-18 07:57 nucliadb/writer/api/v1/knowledgebox.py
--rw-r--r--  2.0 unx     2052 b- defN 24-Apr-18 07:57 nucliadb/writer/api/v1/learning_config.py
--rw-r--r--  2.0 unx    19940 b- defN 24-Apr-18 07:57 nucliadb/writer/api/v1/resource.py
--rw-r--r--  2.0 unx     1034 b- defN 24-Apr-18 07:57 nucliadb/writer/api/v1/router.py
--rw-r--r--  2.0 unx    12733 b- defN 24-Apr-18 07:57 nucliadb/writer/api/v1/services.py
--rw-r--r--  2.0 unx    31464 b- defN 24-Apr-18 07:57 nucliadb/writer/api/v1/upload.py
--rw-r--r--  2.0 unx     1612 b- defN 24-Apr-18 07:57 nucliadb/writer/layouts/__init__.py
--rw-r--r--  2.0 unx     2115 b- defN 24-Apr-18 07:57 nucliadb/writer/layouts/v1.py
--rw-r--r--  2.0 unx      835 b- defN 24-Apr-18 07:57 nucliadb/writer/resource/__init__.py
--rw-r--r--  2.0 unx     1425 b- defN 24-Apr-18 07:57 nucliadb/writer/resource/audit.py
--rw-r--r--  2.0 unx    10968 b- defN 24-Apr-18 07:57 nucliadb/writer/resource/basic.py
--rw-r--r--  2.0 unx    16319 b- defN 24-Apr-18 07:57 nucliadb/writer/resource/field.py
--rw-r--r--  2.0 unx     2022 b- defN 24-Apr-18 07:57 nucliadb/writer/resource/origin.py
--rw-r--r--  2.0 unx     1152 b- defN 24-Apr-18 07:57 nucliadb/writer/resource/slug.py
--rw-r--r--  2.0 unx      835 b- defN 24-Apr-18 07:57 nucliadb/writer/tests/__init__.py
--rw-r--r--  2.0 unx     1200 b- defN 24-Apr-18 07:57 nucliadb/writer/tests/conftest.py
--rw-r--r--  2.0 unx     5971 b- defN 24-Apr-18 07:57 nucliadb/writer/tests/fixtures.py
--rw-r--r--  2.0 unx    15472 b- defN 24-Apr-18 07:57 nucliadb/writer/tests/test_fields.py
--rw-r--r--  2.0 unx    25913 b- defN 24-Apr-18 07:57 nucliadb/writer/tests/test_files.py
--rw-r--r--  2.0 unx     1729 b- defN 24-Apr-18 07:57 nucliadb/writer/tests/test_knowledgebox.py
--rw-r--r--  2.0 unx     4569 b- defN 24-Apr-18 07:57 nucliadb/writer/tests/test_reprocess_file_field.py
--rw-r--r--  2.0 unx    17449 b- defN 24-Apr-18 07:57 nucliadb/writer/tests/test_resources.py
--rw-r--r--  2.0 unx     5120 b- defN 24-Apr-18 07:57 nucliadb/writer/tests/test_service.py
--rw-r--r--  2.0 unx     6054 b- defN 24-Apr-18 07:57 nucliadb/writer/tests/test_tus.py
--rw-r--r--  2.0 unx     1287 b- defN 24-Apr-18 07:57 nucliadb/writer/tests/utils.py
--rw-r--r--  2.0 unx     5226 b- defN 24-Apr-18 07:57 nucliadb/writer/tus/__init__.py
--rw-r--r--  2.0 unx     5082 b- defN 24-Apr-18 07:57 nucliadb/writer/tus/dm.py
--rw-r--r--  2.0 unx     2186 b- defN 24-Apr-18 07:57 nucliadb/writer/tus/exceptions.py
--rw-r--r--  2.0 unx    14527 b- defN 24-Apr-18 07:57 nucliadb/writer/tus/gcs.py
--rw-r--r--  2.0 unx     5849 b- defN 24-Apr-18 07:57 nucliadb/writer/tus/local.py
--rw-r--r--  2.0 unx     4367 b- defN 24-Apr-18 07:57 nucliadb/writer/tus/pg.py
--rw-r--r--  2.0 unx     9069 b- defN 24-Apr-18 07:57 nucliadb/writer/tus/s3.py
--rw-r--r--  2.0 unx     4734 b- defN 24-Apr-18 07:57 nucliadb/writer/tus/storage.py
--rw-r--r--  2.0 unx     2556 b- defN 24-Apr-18 07:57 nucliadb/writer/tus/utils.py
--rw-r--r--  2.0 unx     4348 b- defN 24-Apr-18 07:58 nucliadb-3.0.3.post436.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-18 07:58 nucliadb-3.0.3.post436.dist-info/WHEEL
--rw-r--r--  2.0 unx     1268 b- defN 24-Apr-18 07:58 nucliadb-3.0.3.post436.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       20 b- defN 24-Apr-18 07:58 nucliadb-3.0.3.post436.dist-info/top_level.txt
--rw-r--r--  2.0 unx        1 b- defN 24-Apr-18 07:58 nucliadb-3.0.3.post436.dist-info/zip-safe
--rw-rw-r--  2.0 unx    42245 b- defN 24-Apr-18 07:58 nucliadb-3.0.3.post436.dist-info/RECORD
-451 files, 2226110 bytes uncompressed, 679260 bytes compressed:  69.5%
+Zip file size: 749659 bytes, number of entries: 453
+-rw-r--r--  2.0 unx     1135 b- defN 24-Apr-18 08:02 migrations/0001_bootstrap.py
+-rw-r--r--  2.0 unx     1177 b- defN 24-Apr-18 08:02 migrations/0002_rollover_shards.py
+-rw-r--r--  2.0 unx     2436 b- defN 24-Apr-18 08:02 migrations/0003_allfields_key.py
+-rw-r--r--  2.0 unx     1177 b- defN 24-Apr-18 08:02 migrations/0004_rollover_shards.py
+-rw-r--r--  2.0 unx     1177 b- defN 24-Apr-18 08:02 migrations/0005_rollover_shards.py
+-rw-r--r--  2.0 unx     1024 b- defN 24-Apr-18 08:02 migrations/0006_rollover_shards.py
+-rw-r--r--  2.0 unx     1301 b- defN 24-Apr-18 08:02 migrations/0008_cleanup_leftover_rollover_metadata.py
+-rw-r--r--  2.0 unx     1378 b- defN 24-Apr-18 08:02 migrations/0009_upgrade_relations_and_texts_to_v2.py
+-rw-r--r--  2.0 unx     1610 b- defN 24-Apr-18 08:02 migrations/0010_fix_corrupt_indexes.py
+-rw-r--r--  2.0 unx     1843 b- defN 24-Apr-18 08:02 migrations/0011_materialize_labelset_ids.py
+-rw-r--r--  2.0 unx     1443 b- defN 24-Apr-18 08:02 migrations/0012_rollover_shards.py
+-rw-r--r--  2.0 unx     1024 b- defN 24-Apr-18 08:02 migrations/0013_rollover_shards.py
+-rw-r--r--  2.0 unx     1382 b- defN 24-Apr-18 08:02 migrations/0014_rollover_shards.py
+-rw-r--r--  2.0 unx     1462 b- defN 24-Apr-18 08:02 migrations/0015_targeted_rollover.py
+-rw-r--r--  2.0 unx     2506 b- defN 24-Apr-18 08:02 migrations/0016_upgrade_to_paragraphs_v2.py
+-rw-r--r--  2.0 unx     2100 b- defN 24-Apr-18 08:02 migrations/0017_multiple_writable_shards.py
+-rw-r--r--  2.0 unx     2264 b- defN 24-Apr-18 08:02 migrations/0018_purge_orphan_kbslugs.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Apr-18 08:02 migrations/__init__.py
+-rw-r--r--  2.0 unx      891 b- defN 24-Apr-18 08:02 nucliadb/__init__.py
+-rw-r--r--  2.0 unx     3733 b- defN 24-Apr-18 08:02 nucliadb/health.py
+-rw-r--r--  2.0 unx    10590 b- defN 24-Apr-18 08:02 nucliadb/learning_proxy.py
+-rw-r--r--  2.0 unx     4806 b- defN 24-Apr-18 08:02 nucliadb/metrics_exporter.py
+-rw-r--r--  2.0 unx     2272 b- defN 24-Apr-18 08:02 nucliadb/openapi.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-18 08:02 nucliadb/py.typed
+-rw-r--r--  2.0 unx      835 b- defN 24-Apr-18 08:02 nucliadb/common/__init__.py
+-rw-r--r--  2.0 unx     4905 b- defN 24-Apr-18 08:02 nucliadb/common/locking.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Apr-18 08:02 nucliadb/common/cluster/__init__.py
+-rw-r--r--  2.0 unx     4983 b- defN 24-Apr-18 08:02 nucliadb/common/cluster/base.py
+-rw-r--r--  2.0 unx     1495 b- defN 24-Apr-18 08:02 nucliadb/common/cluster/exceptions.py
+-rw-r--r--  2.0 unx     3658 b- defN 24-Apr-18 08:02 nucliadb/common/cluster/grpc_node_dummy.py
+-rw-r--r--  2.0 unx     3429 b- defN 24-Apr-18 08:02 nucliadb/common/cluster/index_node.py
+-rw-r--r--  2.0 unx    21095 b- defN 24-Apr-18 08:02 nucliadb/common/cluster/manager.py
+-rw-r--r--  2.0 unx     8490 b- defN 24-Apr-18 08:02 nucliadb/common/cluster/rebalance.py
+-rw-r--r--  2.0 unx    19449 b- defN 24-Apr-18 08:02 nucliadb/common/cluster/rollover.py
+-rw-r--r--  2.0 unx     2713 b- defN 24-Apr-18 08:02 nucliadb/common/cluster/settings.py
+-rw-r--r--  2.0 unx     5494 b- defN 24-Apr-18 08:02 nucliadb/common/cluster/utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Apr-18 08:02 nucliadb/common/cluster/discovery/__init__.py
+-rw-r--r--  2.0 unx     6553 b- defN 24-Apr-18 08:02 nucliadb/common/cluster/discovery/base.py
+-rw-r--r--  2.0 unx    12518 b- defN 24-Apr-18 08:02 nucliadb/common/cluster/discovery/k8s.py
+-rw-r--r--  2.0 unx     1957 b- defN 24-Apr-18 08:02 nucliadb/common/cluster/discovery/manual.py
+-rw-r--r--  2.0 unx     1737 b- defN 24-Apr-18 08:02 nucliadb/common/cluster/discovery/single.py
+-rw-r--r--  2.0 unx     1139 b- defN 24-Apr-18 08:02 nucliadb/common/cluster/discovery/types.py
+-rw-r--r--  2.0 unx     2548 b- defN 24-Apr-18 08:02 nucliadb/common/cluster/discovery/utils.py
+-rw-r--r--  2.0 unx      833 b- defN 24-Apr-18 08:02 nucliadb/common/cluster/standalone/__init__.py
+-rw-r--r--  2.0 unx    13705 b- defN 24-Apr-18 08:02 nucliadb/common/cluster/standalone/grpc_node_binding.py
+-rw-r--r--  2.0 unx     4683 b- defN 24-Apr-18 08:02 nucliadb/common/cluster/standalone/index_node.py
+-rw-r--r--  2.0 unx     3444 b- defN 24-Apr-18 08:02 nucliadb/common/cluster/standalone/service.py
+-rw-r--r--  2.0 unx     3386 b- defN 24-Apr-18 08:02 nucliadb/common/cluster/standalone/utils.py
+-rw-r--r--  2.0 unx     3498 b- defN 24-Apr-18 08:02 nucliadb/common/context/__init__.py
+-rw-r--r--  2.0 unx     1628 b- defN 24-Apr-18 08:02 nucliadb/common/context/fastapi.py
+-rw-r--r--  2.0 unx     1813 b- defN 24-Apr-18 08:02 nucliadb/common/datamanagers/__init__.py
+-rw-r--r--  2.0 unx     1451 b- defN 24-Apr-18 08:02 nucliadb/common/datamanagers/cluster.py
+-rw-r--r--  2.0 unx     5383 b- defN 24-Apr-18 08:02 nucliadb/common/datamanagers/entities.py
+-rw-r--r--  2.0 unx      883 b- defN 24-Apr-18 08:02 nucliadb/common/datamanagers/exceptions.py
+-rw-r--r--  2.0 unx     2940 b- defN 24-Apr-18 08:02 nucliadb/common/datamanagers/kb.py
+-rw-r--r--  2.0 unx     5389 b- defN 24-Apr-18 08:02 nucliadb/common/datamanagers/labels.py
+-rw-r--r--  2.0 unx     1599 b- defN 24-Apr-18 08:02 nucliadb/common/datamanagers/processing.py
+-rw-r--r--  2.0 unx     7637 b- defN 24-Apr-18 08:02 nucliadb/common/datamanagers/resources.py
+-rw-r--r--  2.0 unx     5633 b- defN 24-Apr-18 08:02 nucliadb/common/datamanagers/rollover.py
+-rw-r--r--  2.0 unx     1681 b- defN 24-Apr-18 08:02 nucliadb/common/datamanagers/utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Apr-18 08:02 nucliadb/common/http_clients/__init__.py
+-rw-r--r--  2.0 unx     2146 b- defN 24-Apr-18 08:02 nucliadb/common/http_clients/auth.py
+-rw-r--r--  2.0 unx     1100 b- defN 24-Apr-18 08:02 nucliadb/common/http_clients/exceptions.py
+-rw-r--r--  2.0 unx     7155 b- defN 24-Apr-18 08:02 nucliadb/common/http_clients/processing.py
+-rw-r--r--  2.0 unx     1540 b- defN 24-Apr-18 08:02 nucliadb/common/http_clients/pypi.py
+-rw-r--r--  2.0 unx     1551 b- defN 24-Apr-18 08:02 nucliadb/common/http_clients/utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Apr-18 08:02 nucliadb/common/maindb/__init__.py
+-rw-r--r--  2.0 unx     3449 b- defN 24-Apr-18 08:02 nucliadb/common/maindb/driver.py
+-rw-r--r--  2.0 unx      946 b- defN 24-Apr-18 08:02 nucliadb/common/maindb/exceptions.py
+-rw-r--r--  2.0 unx     6769 b- defN 24-Apr-18 08:02 nucliadb/common/maindb/local.py
+-rw-r--r--  2.0 unx     8391 b- defN 24-Apr-18 08:02 nucliadb/common/maindb/pg.py
+-rw-r--r--  2.0 unx     6053 b- defN 24-Apr-18 08:02 nucliadb/common/maindb/redis.py
+-rw-r--r--  2.0 unx    14502 b- defN 24-Apr-18 08:02 nucliadb/common/maindb/tikv.py
+-rw-r--r--  2.0 unx     4109 b- defN 24-Apr-18 08:02 nucliadb/common/maindb/utils.py
+-rw-r--r--  2.0 unx      932 b- defN 24-Apr-18 08:02 nucliadb/export_import/__init__.py
+-rw-r--r--  2.0 unx     6171 b- defN 24-Apr-18 08:02 nucliadb/export_import/datamanager.py
+-rw-r--r--  2.0 unx     1949 b- defN 24-Apr-18 08:02 nucliadb/export_import/exceptions.py
+-rw-r--r--  2.0 unx     7116 b- defN 24-Apr-18 08:02 nucliadb/export_import/exporter.py
+-rw-r--r--  2.0 unx     4258 b- defN 24-Apr-18 08:02 nucliadb/export_import/importer.py
+-rw-r--r--  2.0 unx     2063 b- defN 24-Apr-18 08:02 nucliadb/export_import/models.py
+-rw-r--r--  2.0 unx     2571 b- defN 24-Apr-18 08:02 nucliadb/export_import/tasks.py
+-rw-r--r--  2.0 unx    19270 b- defN 24-Apr-18 08:02 nucliadb/export_import/utils.py
+-rw-r--r--  2.0 unx     1011 b- defN 24-Apr-18 08:02 nucliadb/ingest/__init__.py
+-rw-r--r--  2.0 unx     7277 b- defN 24-Apr-18 08:02 nucliadb/ingest/app.py
+-rw-r--r--  2.0 unx     1005 b- defN 24-Apr-18 08:02 nucliadb/ingest/cache.py
+-rw-r--r--  2.0 unx     2484 b- defN 24-Apr-18 08:02 nucliadb/ingest/partitions.py
+-rw-r--r--  2.0 unx    19541 b- defN 24-Apr-18 08:02 nucliadb/ingest/processing.py
+-rw-r--r--  2.0 unx    20277 b- defN 24-Apr-18 08:02 nucliadb/ingest/serialize.py
+-rw-r--r--  2.0 unx     3183 b- defN 24-Apr-18 08:02 nucliadb/ingest/settings.py
+-rw-r--r--  2.0 unx     2314 b- defN 24-Apr-18 08:02 nucliadb/ingest/utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Apr-18 08:02 nucliadb/ingest/consumer/__init__.py
+-rw-r--r--  2.0 unx    11563 b- defN 24-Apr-18 08:02 nucliadb/ingest/consumer/auditing.py
+-rw-r--r--  2.0 unx    12159 b- defN 24-Apr-18 08:02 nucliadb/ingest/consumer/consumer.py
+-rw-r--r--  2.0 unx     3788 b- defN 24-Apr-18 08:02 nucliadb/ingest/consumer/materializer.py
+-rw-r--r--  2.0 unx     1075 b- defN 24-Apr-18 08:02 nucliadb/ingest/consumer/metrics.py
+-rw-r--r--  2.0 unx     9543 b- defN 24-Apr-18 08:02 nucliadb/ingest/consumer/pull.py
+-rw-r--r--  2.0 unx     6935 b- defN 24-Apr-18 08:02 nucliadb/ingest/consumer/service.py
+-rw-r--r--  2.0 unx     4331 b- defN 24-Apr-18 08:02 nucliadb/ingest/consumer/shard_creator.py
+-rw-r--r--  2.0 unx     2656 b- defN 24-Apr-18 08:02 nucliadb/ingest/consumer/utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Apr-18 08:02 nucliadb/ingest/fields/__init__.py
+-rw-r--r--  2.0 unx    18433 b- defN 24-Apr-18 08:02 nucliadb/ingest/fields/base.py
+-rw-r--r--  2.0 unx     6516 b- defN 24-Apr-18 08:02 nucliadb/ingest/fields/conversation.py
+-rw-r--r--  2.0 unx     1223 b- defN 24-Apr-18 08:02 nucliadb/ingest/fields/date.py
+-rw-r--r--  2.0 unx     1205 b- defN 24-Apr-18 08:02 nucliadb/ingest/fields/exceptions.py
+-rw-r--r--  2.0 unx     5159 b- defN 24-Apr-18 08:02 nucliadb/ingest/fields/file.py
+-rw-r--r--  2.0 unx     1547 b- defN 24-Apr-18 08:02 nucliadb/ingest/fields/generic.py
+-rw-r--r--  2.0 unx     1235 b- defN 24-Apr-18 08:02 nucliadb/ingest/fields/keywordset.py
+-rw-r--r--  2.0 unx     2250 b- defN 24-Apr-18 08:02 nucliadb/ingest/fields/layout.py
+-rw-r--r--  2.0 unx     4084 b- defN 24-Apr-18 08:02 nucliadb/ingest/fields/link.py
+-rw-r--r--  2.0 unx     1319 b- defN 24-Apr-18 08:02 nucliadb/ingest/fields/text.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Apr-18 08:02 nucliadb/ingest/orm/__init__.py
+-rw-r--r--  2.0 unx    27582 b- defN 24-Apr-18 08:02 nucliadb/ingest/orm/brain.py
+-rw-r--r--  2.0 unx    15758 b- defN 24-Apr-18 08:02 nucliadb/ingest/orm/entities.py
+-rw-r--r--  2.0 unx     1279 b- defN 24-Apr-18 08:02 nucliadb/ingest/orm/exceptions.py
+-rw-r--r--  2.0 unx    18747 b- defN 24-Apr-18 08:02 nucliadb/ingest/orm/knowledgebox.py
+-rw-r--r--  2.0 unx     1096 b- defN 24-Apr-18 08:02 nucliadb/ingest/orm/metrics.py
+-rw-r--r--  2.0 unx    60085 b- defN 24-Apr-18 08:02 nucliadb/ingest/orm/resource.py
+-rw-r--r--  2.0 unx     1739 b- defN 24-Apr-18 08:02 nucliadb/ingest/orm/synonyms.py
+-rw-r--r--  2.0 unx     3074 b- defN 24-Apr-18 08:02 nucliadb/ingest/orm/utils.py
+-rw-r--r--  2.0 unx    26460 b- defN 24-Apr-18 08:02 nucliadb/ingest/orm/processor/__init__.py
+-rw-r--r--  2.0 unx     1690 b- defN 24-Apr-18 08:02 nucliadb/ingest/orm/processor/sequence_manager.py
+-rw-r--r--  2.0 unx     2057 b- defN 24-Apr-18 08:02 nucliadb/ingest/service/__init__.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Apr-18 08:02 nucliadb/ingest/service/exceptions.py
+-rw-r--r--  2.0 unx    36594 b- defN 24-Apr-18 08:02 nucliadb/ingest/service/writer.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Apr-18 08:02 nucliadb/ingest/tests/__init__.py
+-rw-r--r--  2.0 unx     1157 b- defN 24-Apr-18 08:02 nucliadb/ingest/tests/conftest.py
+-rw-r--r--  2.0 unx    24068 b- defN 24-Apr-18 08:02 nucliadb/ingest/tests/fixtures.py
+-rw-r--r--  2.0 unx    62843 b- defN 24-Apr-18 08:02 nucliadb/ingest/tests/vectors.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Apr-18 08:02 nucliadb/ingest/tests/integration/__init__.py
+-rw-r--r--  2.0 unx      833 b- defN 24-Apr-18 08:02 nucliadb/ingest/tests/integration/consumer/__init__.py
+-rw-r--r--  2.0 unx     2549 b- defN 24-Apr-18 08:02 nucliadb/ingest/tests/integration/consumer/test_auditing.py
+-rw-r--r--  2.0 unx     2591 b- defN 24-Apr-18 08:02 nucliadb/ingest/tests/integration/consumer/test_materializer.py
+-rw-r--r--  2.0 unx     4465 b- defN 24-Apr-18 08:02 nucliadb/ingest/tests/integration/consumer/test_pull.py
+-rw-r--r--  2.0 unx     2763 b- defN 24-Apr-18 08:02 nucliadb/ingest/tests/integration/consumer/test_service.py
+-rw-r--r--  2.0 unx     2019 b- defN 24-Apr-18 08:02 nucliadb/ingest/tests/integration/consumer/test_shard_creator.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Apr-18 08:02 nucliadb/ingest/tests/integration/ingest/__init__.py
+-rw-r--r--  2.0 unx    27334 b- defN 24-Apr-18 08:02 nucliadb/ingest/tests/integration/ingest/test_ingest.py
+-rw-r--r--  2.0 unx     3040 b- defN 24-Apr-18 08:02 nucliadb/ingest/tests/integration/ingest/test_processing_engine.py
+-rw-r--r--  2.0 unx     8586 b- defN 24-Apr-18 08:02 nucliadb/ingest/tests/integration/ingest/test_relations.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Apr-18 08:02 nucliadb/ingest/tests/unit/__init__.py
+-rw-r--r--  2.0 unx     1189 b- defN 24-Apr-18 08:02 nucliadb/ingest/tests/unit/test_cache.py
+-rw-r--r--  2.0 unx     1432 b- defN 24-Apr-18 08:02 nucliadb/ingest/tests/unit/test_partitions.py
+-rw-r--r--  2.0 unx     5807 b- defN 24-Apr-18 08:02 nucliadb/ingest/tests/unit/test_processing.py
+-rw-r--r--  2.0 unx      978 b- defN 24-Apr-18 08:02 nucliadb/ingest/tests/unit/test_settings.py
+-rw-r--r--  2.0 unx      833 b- defN 24-Apr-18 08:02 nucliadb/ingest/tests/unit/consumer/__init__.py
+-rw-r--r--  2.0 unx     3981 b- defN 24-Apr-18 08:02 nucliadb/ingest/tests/unit/consumer/test_auditing.py
+-rw-r--r--  2.0 unx     2472 b- defN 24-Apr-18 08:02 nucliadb/ingest/tests/unit/consumer/test_consumer.py
+-rw-r--r--  2.0 unx     2063 b- defN 24-Apr-18 08:02 nucliadb/ingest/tests/unit/consumer/test_pull.py
+-rw-r--r--  2.0 unx     4075 b- defN 24-Apr-18 08:02 nucliadb/ingest/tests/unit/consumer/test_shard_creator.py
+-rw-r--r--  2.0 unx     1934 b- defN 24-Apr-18 08:02 nucliadb/ingest/tests/unit/consumer/test_utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Apr-18 08:02 nucliadb/ingest/tests/unit/orm/__init__.py
+-rw-r--r--  2.0 unx     9876 b- defN 24-Apr-18 08:02 nucliadb/ingest/tests/unit/orm/test_brain.py
+-rw-r--r--  2.0 unx     4045 b- defN 24-Apr-18 08:02 nucliadb/ingest/tests/unit/orm/test_processor.py
+-rw-r--r--  2.0 unx     8965 b- defN 24-Apr-18 08:02 nucliadb/ingest/tests/unit/orm/test_resource.py
+-rw-r--r--  2.0 unx     2216 b- defN 24-Apr-18 08:02 nucliadb/middleware/__init__.py
+-rw-r--r--  2.0 unx     3912 b- defN 24-Apr-18 08:02 nucliadb/middleware/transaction.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Apr-18 08:02 nucliadb/migrator/__init__.py
+-rw-r--r--  2.0 unx     2119 b- defN 24-Apr-18 08:02 nucliadb/migrator/command.py
+-rw-r--r--  2.0 unx     1334 b- defN 24-Apr-18 08:02 nucliadb/migrator/context.py
+-rw-r--r--  2.0 unx     5104 b- defN 24-Apr-18 08:02 nucliadb/migrator/datamanager.py
+-rw-r--r--  2.0 unx      889 b- defN 24-Apr-18 08:02 nucliadb/migrator/exceptions.py
+-rw-r--r--  2.0 unx     9237 b- defN 24-Apr-18 08:02 nucliadb/migrator/migrator.py
+-rw-r--r--  2.0 unx     1145 b- defN 24-Apr-18 08:02 nucliadb/migrator/models.py
+-rw-r--r--  2.0 unx     1110 b- defN 24-Apr-18 08:02 nucliadb/migrator/settings.py
+-rw-r--r--  2.0 unx     2346 b- defN 24-Apr-18 08:02 nucliadb/migrator/utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Apr-18 08:02 nucliadb/models/__init__.py
+-rw-r--r--  2.0 unx     1599 b- defN 24-Apr-18 08:02 nucliadb/models/responses.py
+-rw-r--r--  2.0 unx     6041 b- defN 24-Apr-18 08:02 nucliadb/purge/__init__.py
+-rw-r--r--  2.0 unx     9364 b- defN 24-Apr-18 08:02 nucliadb/purge/orphan_shards.py
+-rw-r--r--  2.0 unx     1328 b- defN 24-Apr-18 08:02 nucliadb/reader/__init__.py
+-rw-r--r--  2.0 unx     3709 b- defN 24-Apr-18 08:02 nucliadb/reader/app.py
+-rw-r--r--  2.0 unx     1366 b- defN 24-Apr-18 08:02 nucliadb/reader/lifecycle.py
+-rw-r--r--  2.0 unx     1031 b- defN 24-Apr-18 08:02 nucliadb/reader/openapi.py
+-rw-r--r--  2.0 unx     1447 b- defN 24-Apr-18 08:02 nucliadb/reader/run.py
+-rw-r--r--  2.0 unx      872 b- defN 24-Apr-18 08:02 nucliadb/reader/api/__init__.py
+-rw-r--r--  2.0 unx     2434 b- defN 24-Apr-18 08:02 nucliadb/reader/api/models.py
+-rw-r--r--  2.0 unx     1110 b- defN 24-Apr-18 08:02 nucliadb/reader/api/v1/__init__.py
+-rw-r--r--  2.0 unx    12368 b- defN 24-Apr-18 08:02 nucliadb/reader/api/v1/download.py
+-rw-r--r--  2.0 unx     6450 b- defN 24-Apr-18 08:02 nucliadb/reader/api/v1/export_import.py
+-rw-r--r--  2.0 unx     3632 b- defN 24-Apr-18 08:02 nucliadb/reader/api/v1/knowledgebox.py
+-rw-r--r--  2.0 unx     2093 b- defN 24-Apr-18 08:02 nucliadb/reader/api/v1/learning_collector.py
+-rw-r--r--  2.0 unx     4454 b- defN 24-Apr-18 08:02 nucliadb/reader/api/v1/learning_config.py
+-rw-r--r--  2.0 unx    13928 b- defN 24-Apr-18 08:02 nucliadb/reader/api/v1/resource.py
+-rw-r--r--  2.0 unx     1011 b- defN 24-Apr-18 08:02 nucliadb/reader/api/v1/router.py
+-rw-r--r--  2.0 unx    13882 b- defN 24-Apr-18 08:02 nucliadb/reader/api/v1/services.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Apr-18 08:02 nucliadb/reader/reader/__init__.py
+-rw-r--r--  2.0 unx     8155 b- defN 24-Apr-18 08:02 nucliadb/reader/reader/notifications.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Apr-18 08:02 nucliadb/reader/tests/__init__.py
+-rw-r--r--  2.0 unx     1224 b- defN 24-Apr-18 08:02 nucliadb/reader/tests/conftest.py
+-rw-r--r--  2.0 unx     4345 b- defN 24-Apr-18 08:02 nucliadb/reader/tests/fixtures.py
+-rw-r--r--  2.0 unx     2748 b- defN 24-Apr-18 08:02 nucliadb/reader/tests/test_list_resources.py
+-rw-r--r--  2.0 unx    10199 b- defN 24-Apr-18 08:02 nucliadb/reader/tests/test_reader_file_download.py
+-rw-r--r--  2.0 unx    10586 b- defN 24-Apr-18 08:02 nucliadb/reader/tests/test_reader_resource.py
+-rw-r--r--  2.0 unx     6535 b- defN 24-Apr-18 08:02 nucliadb/reader/tests/test_reader_resource_field.py
+-rw-r--r--  2.0 unx     1535 b- defN 24-Apr-18 08:02 nucliadb/search/__init__.py
+-rw-r--r--  2.0 unx     4905 b- defN 24-Apr-18 08:02 nucliadb/search/app.py
+-rw-r--r--  2.0 unx     1956 b- defN 24-Apr-18 08:02 nucliadb/search/lifecycle.py
+-rw-r--r--  2.0 unx     1016 b- defN 24-Apr-18 08:02 nucliadb/search/openapi.py
+-rw-r--r--  2.0 unx    19798 b- defN 24-Apr-18 08:02 nucliadb/search/predict.py
+-rw-r--r--  2.0 unx     1402 b- defN 24-Apr-18 08:02 nucliadb/search/run.py
+-rw-r--r--  2.0 unx     1193 b- defN 24-Apr-18 08:02 nucliadb/search/settings.py
+-rw-r--r--  2.0 unx     1037 b- defN 24-Apr-18 08:02 nucliadb/search/utilities.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Apr-18 08:02 nucliadb/search/api/__init__.py
+-rw-r--r--  2.0 unx     1272 b- defN 24-Apr-18 08:02 nucliadb/search/api/v1/__init__.py
+-rw-r--r--  2.0 unx     9913 b- defN 24-Apr-18 08:02 nucliadb/search/api/v1/chat.py
+-rw-r--r--  2.0 unx     2665 b- defN 24-Apr-18 08:02 nucliadb/search/api/v1/feedback.py
+-rw-r--r--  2.0 unx     8804 b- defN 24-Apr-18 08:02 nucliadb/search/api/v1/find.py
+-rw-r--r--  2.0 unx     7026 b- defN 24-Apr-18 08:02 nucliadb/search/api/v1/knowledgebox.py
+-rw-r--r--  2.0 unx     3041 b- defN 24-Apr-18 08:02 nucliadb/search/api/v1/predict_proxy.py
+-rw-r--r--  2.0 unx      988 b- defN 24-Apr-18 08:02 nucliadb/search/api/v1/router.py
+-rw-r--r--  2.0 unx    18359 b- defN 24-Apr-18 08:02 nucliadb/search/api/v1/search.py
+-rw-r--r--  2.0 unx     5928 b- defN 24-Apr-18 08:02 nucliadb/search/api/v1/suggest.py
+-rw-r--r--  2.0 unx     2536 b- defN 24-Apr-18 08:02 nucliadb/search/api/v1/summarize.py
+-rw-r--r--  2.0 unx     1412 b- defN 24-Apr-18 08:02 nucliadb/search/api/v1/utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Apr-18 08:02 nucliadb/search/api/v1/resource/__init__.py
+-rw-r--r--  2.0 unx     6095 b- defN 24-Apr-18 08:02 nucliadb/search/api/v1/resource/ask.py
+-rw-r--r--  2.0 unx     5887 b- defN 24-Apr-18 08:02 nucliadb/search/api/v1/resource/chat.py
+-rw-r--r--  2.0 unx     5293 b- defN 24-Apr-18 08:02 nucliadb/search/api/v1/resource/search.py
+-rw-r--r--  2.0 unx      833 b- defN 24-Apr-18 08:02 nucliadb/search/requesters/__init__.py
+-rw-r--r--  2.0 unx     9070 b- defN 24-Apr-18 08:02 nucliadb/search/requesters/utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Apr-18 08:02 nucliadb/search/search/__init__.py
+-rw-r--r--  2.0 unx     2746 b- defN 24-Apr-18 08:02 nucliadb/search/search/cache.py
+-rw-r--r--  2.0 unx     1154 b- defN 24-Apr-18 08:02 nucliadb/search/search/exceptions.py
+-rw-r--r--  2.0 unx     5465 b- defN 24-Apr-18 08:02 nucliadb/search/search/fetch.py
+-rw-r--r--  2.0 unx     6513 b- defN 24-Apr-18 08:02 nucliadb/search/search/filters.py
+-rw-r--r--  2.0 unx     4646 b- defN 24-Apr-18 08:02 nucliadb/search/search/find.py
+-rw-r--r--  2.0 unx    17152 b- defN 24-Apr-18 08:02 nucliadb/search/search/find_merge.py
+-rw-r--r--  2.0 unx    21118 b- defN 24-Apr-18 08:02 nucliadb/search/search/merge.py
+-rw-r--r--  2.0 unx     1130 b- defN 24-Apr-18 08:02 nucliadb/search/search/metrics.py
+-rw-r--r--  2.0 unx     8698 b- defN 24-Apr-18 08:02 nucliadb/search/search/paragraphs.py
+-rw-r--r--  2.0 unx     3026 b- defN 24-Apr-18 08:02 nucliadb/search/search/predict_proxy.py
+-rw-r--r--  2.0 unx    32297 b- defN 24-Apr-18 08:02 nucliadb/search/search/query.py
+-rw-r--r--  2.0 unx     3149 b- defN 24-Apr-18 08:02 nucliadb/search/search/shards.py
+-rw-r--r--  2.0 unx     5101 b- defN 24-Apr-18 08:02 nucliadb/search/search/summarize.py
+-rw-r--r--  2.0 unx     2438 b- defN 24-Apr-18 08:02 nucliadb/search/search/utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Apr-18 08:02 nucliadb/search/search/chat/__init__.py
+-rw-r--r--  2.0 unx     2058 b- defN 24-Apr-18 08:02 nucliadb/search/search/chat/images.py
+-rw-r--r--  2.0 unx    20793 b- defN 24-Apr-18 08:02 nucliadb/search/search/chat/prompt.py
+-rw-r--r--  2.0 unx    15347 b- defN 24-Apr-18 08:02 nucliadb/search/search/chat/query.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Apr-18 08:02 nucliadb/search/tests/__init__.py
+-rw-r--r--  2.0 unx     1295 b- defN 24-Apr-18 08:02 nucliadb/search/tests/conftest.py
+-rw-r--r--  2.0 unx     6578 b- defN 24-Apr-18 08:02 nucliadb/search/tests/fixtures.py
+-rw-r--r--  2.0 unx    15529 b- defN 24-Apr-18 08:02 nucliadb/search/tests/node.py
+-rw-r--r--  2.0 unx      833 b- defN 24-Apr-18 08:02 nucliadb/search/tests/unit/__init__.py
+-rw-r--r--  2.0 unx     2649 b- defN 24-Apr-18 08:02 nucliadb/search/tests/unit/test_app.py
+-rw-r--r--  2.0 unx     3374 b- defN 24-Apr-18 08:02 nucliadb/search/tests/unit/test_find_merge.py
+-rw-r--r--  2.0 unx     1400 b- defN 24-Apr-18 08:02 nucliadb/search/tests/unit/test_merge.py
+-rw-r--r--  2.0 unx    17080 b- defN 24-Apr-18 08:02 nucliadb/search/tests/unit/test_predict.py
+-rw-r--r--  2.0 unx     1317 b- defN 24-Apr-18 08:02 nucliadb/search/tests/unit/test_run.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Apr-18 08:02 nucliadb/search/tests/unit/api/__init__.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Apr-18 08:02 nucliadb/search/tests/unit/api/v1/__init__.py
+-rw-r--r--  2.0 unx     2966 b- defN 24-Apr-18 08:02 nucliadb/search/tests/unit/api/v1/test_chat.py
+-rw-r--r--  2.0 unx     2865 b- defN 24-Apr-18 08:02 nucliadb/search/tests/unit/api/v1/test_predict_proxy.py
+-rw-r--r--  2.0 unx     2901 b- defN 24-Apr-18 08:02 nucliadb/search/tests/unit/api/v1/test_summarize.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Apr-18 08:02 nucliadb/search/tests/unit/api/v1/resource/__init__.py
+-rw-r--r--  2.0 unx     2411 b- defN 24-Apr-18 08:02 nucliadb/search/tests/unit/api/v1/resource/test_ask.py
+-rw-r--r--  2.0 unx     3040 b- defN 24-Apr-18 08:02 nucliadb/search/tests/unit/api/v1/resource/test_chat.py
+-rw-r--r--  2.0 unx      833 b- defN 24-Apr-18 08:02 nucliadb/search/tests/unit/search/__init__.py
+-rw-r--r--  2.0 unx     8567 b- defN 24-Apr-18 08:02 nucliadb/search/tests/unit/search/test_chat_prompt.py
+-rw-r--r--  2.0 unx     3736 b- defN 24-Apr-18 08:02 nucliadb/search/tests/unit/search/test_fetch.py
+-rw-r--r--  2.0 unx     4306 b- defN 24-Apr-18 08:02 nucliadb/search/tests/unit/search/test_filters.py
+-rw-r--r--  2.0 unx     4492 b- defN 24-Apr-18 08:02 nucliadb/search/tests/unit/search/test_paragraphs.py
+-rw-r--r--  2.0 unx     3496 b- defN 24-Apr-18 08:02 nucliadb/search/tests/unit/search/test_predict_proxy.py
+-rw-r--r--  2.0 unx     7001 b- defN 24-Apr-18 08:02 nucliadb/search/tests/unit/search/test_query.py
+-rw-r--r--  2.0 unx      833 b- defN 24-Apr-18 08:02 nucliadb/search/tests/unit/search/requesters/__init__.py
+-rw-r--r--  2.0 unx     6455 b- defN 24-Apr-18 08:02 nucliadb/search/tests/unit/search/requesters/test_utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Apr-18 08:02 nucliadb/search/tests/unit/search/search/__init__.py
+-rw-r--r--  2.0 unx     1759 b- defN 24-Apr-18 08:02 nucliadb/search/tests/unit/search/search/test_shards.py
+-rw-r--r--  2.0 unx     2511 b- defN 24-Apr-18 08:02 nucliadb/search/tests/unit/search/search/test_utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Apr-18 08:02 nucliadb/standalone/__init__.py
+-rw-r--r--  2.0 unx     6746 b- defN 24-Apr-18 08:02 nucliadb/standalone/api_router.py
+-rw-r--r--  2.0 unx     5763 b- defN 24-Apr-18 08:02 nucliadb/standalone/app.py
+-rw-r--r--  2.0 unx     7800 b- defN 24-Apr-18 08:02 nucliadb/standalone/auth.py
+-rw-r--r--  2.0 unx     5309 b- defN 24-Apr-18 08:02 nucliadb/standalone/config.py
+-rw-r--r--  2.0 unx     6930 b- defN 24-Apr-18 08:02 nucliadb/standalone/introspect.py
+-rw-r--r--  2.0 unx     2488 b- defN 24-Apr-18 08:02 nucliadb/standalone/lifecycle.py
+-rw-r--r--  2.0 unx     1317 b- defN 24-Apr-18 08:02 nucliadb/standalone/purge.py
+-rw-r--r--  2.0 unx     5336 b- defN 24-Apr-18 08:02 nucliadb/standalone/run.py
+-rw-r--r--  2.0 unx     5781 b- defN 24-Apr-18 08:02 nucliadb/standalone/settings.py
+-rw-r--r--  2.0 unx     3132 b- defN 24-Apr-18 08:02 nucliadb/standalone/versions.py
+-rw-r--r--  2.0 unx     2285 b- defN 24-Apr-18 08:02 nucliadb/standalone/static/favicon.ico
+-rw-r--r--  2.0 unx     3833 b- defN 24-Apr-18 08:02 nucliadb/standalone/static/index.html
+-rw-r--r--  2.0 unx     2639 b- defN 24-Apr-18 08:02 nucliadb/standalone/static/logo.svg
+-rw-r--r--  2.0 unx      835 b- defN 24-Apr-18 08:02 nucliadb/standalone/tests/__init__.py
+-rw-r--r--  2.0 unx     1294 b- defN 24-Apr-18 08:02 nucliadb/standalone/tests/conftest.py
+-rw-r--r--  2.0 unx     1319 b- defN 24-Apr-18 08:02 nucliadb/standalone/tests/fixtures.py
+-rw-r--r--  2.0 unx      833 b- defN 24-Apr-18 08:02 nucliadb/standalone/tests/unit/__init__.py
+-rw-r--r--  2.0 unx     1722 b- defN 24-Apr-18 08:02 nucliadb/standalone/tests/unit/test_api_router.py
+-rw-r--r--  2.0 unx     5509 b- defN 24-Apr-18 08:02 nucliadb/standalone/tests/unit/test_auth.py
+-rw-r--r--  2.0 unx     1334 b- defN 24-Apr-18 08:02 nucliadb/standalone/tests/unit/test_introspect.py
+-rw-r--r--  2.0 unx     1472 b- defN 24-Apr-18 08:02 nucliadb/standalone/tests/unit/test_run.py
+-rw-r--r--  2.0 unx     1972 b- defN 24-Apr-18 08:02 nucliadb/standalone/tests/unit/test_versions.py
+-rw-r--r--  2.0 unx     1037 b- defN 24-Apr-18 08:02 nucliadb/tasks/__init__.py
+-rw-r--r--  2.0 unx     7655 b- defN 24-Apr-18 08:02 nucliadb/tasks/consumer.py
+-rw-r--r--  2.0 unx      924 b- defN 24-Apr-18 08:02 nucliadb/tasks/logger.py
+-rw-r--r--  2.0 unx     1378 b- defN 24-Apr-18 08:02 nucliadb/tasks/models.py
+-rw-r--r--  2.0 unx     3457 b- defN 24-Apr-18 08:02 nucliadb/tasks/producer.py
+-rw-r--r--  2.0 unx     1753 b- defN 24-Apr-18 08:02 nucliadb/tasks/registry.py
+-rw-r--r--  2.0 unx     1360 b- defN 24-Apr-18 08:02 nucliadb/tasks/utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Apr-18 08:02 nucliadb/tests/__init__.py
+-rw-r--r--  2.0 unx     1229 b- defN 24-Apr-18 08:02 nucliadb/tests/conftest.py
+-rw-r--r--  2.0 unx    22365 b- defN 24-Apr-18 08:02 nucliadb/tests/fixtures.py
+-rw-r--r--  2.0 unx     7549 b- defN 24-Apr-18 08:02 nucliadb/tests/tikv.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Apr-18 08:02 nucliadb/tests/benchmarks/__init__.py
+-rw-r--r--  2.0 unx     3032 b- defN 24-Apr-18 08:02 nucliadb/tests/benchmarks/test_search.py
+-rw-r--r--  2.0 unx      919 b- defN 24-Apr-18 08:02 nucliadb/tests/knowledgeboxes/__init__.py
+-rw-r--r--  2.0 unx     7002 b- defN 24-Apr-18 08:02 nucliadb/tests/knowledgeboxes/philosophy_books.py
+-rw-r--r--  2.0 unx     3037 b- defN 24-Apr-18 08:02 nucliadb/tests/knowledgeboxes/ten_dummy_resources.py
+-rw-r--r--  2.0 unx     1148 b- defN 24-Apr-18 08:02 nucliadb/tests/migrations/__init__.py
+-rw-r--r--  2.0 unx     2726 b- defN 24-Apr-18 08:02 nucliadb/tests/migrations/test_migration_0017.py
+-rw-r--r--  2.0 unx     3625 b- defN 24-Apr-18 08:02 nucliadb/tests/migrations/test_migration_0018.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Apr-18 08:02 nucliadb/tests/unit/__init__.py
+-rw-r--r--  2.0 unx     1487 b- defN 24-Apr-18 08:02 nucliadb/tests/unit/test_field_ids.py
+-rw-r--r--  2.0 unx     2758 b- defN 24-Apr-18 08:02 nucliadb/tests/unit/test_health.py
+-rw-r--r--  2.0 unx     1543 b- defN 24-Apr-18 08:02 nucliadb/tests/unit/test_kb_slugs.py
+-rw-r--r--  2.0 unx     7892 b- defN 24-Apr-18 08:02 nucliadb/tests/unit/test_learning_proxy.py
+-rw-r--r--  2.0 unx     2642 b- defN 24-Apr-18 08:02 nucliadb/tests/unit/test_metrics_exporter.py
+-rw-r--r--  2.0 unx     1341 b- defN 24-Apr-18 08:02 nucliadb/tests/unit/test_openapi.py
+-rw-r--r--  2.0 unx     3656 b- defN 24-Apr-18 08:02 nucliadb/tests/unit/test_purge.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Apr-18 08:02 nucliadb/tests/unit/common/__init__.py
+-rw-r--r--  2.0 unx     1268 b- defN 24-Apr-18 08:02 nucliadb/tests/unit/common/test_context.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Apr-18 08:02 nucliadb/tests/unit/common/cluster/__init__.py
+-rw-r--r--  2.0 unx    11955 b- defN 24-Apr-18 08:02 nucliadb/tests/unit/common/cluster/test_cluster.py
+-rw-r--r--  2.0 unx     5387 b- defN 24-Apr-18 08:02 nucliadb/tests/unit/common/cluster/test_kb_shard_manager.py
+-rw-r--r--  2.0 unx     9470 b- defN 24-Apr-18 08:02 nucliadb/tests/unit/common/cluster/test_rollover.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Apr-18 08:02 nucliadb/tests/unit/common/cluster/discovery/__init__.py
+-rw-r--r--  2.0 unx     5584 b- defN 24-Apr-18 08:02 nucliadb/tests/unit/common/cluster/discovery/test_k8s.py
+-rw-r--r--  2.0 unx      833 b- defN 24-Apr-18 08:02 nucliadb/tests/unit/common/cluster/standalone/__init__.py
+-rw-r--r--  2.0 unx     3750 b- defN 24-Apr-18 08:02 nucliadb/tests/unit/common/cluster/standalone/test_service.py
+-rw-r--r--  2.0 unx     2114 b- defN 24-Apr-18 08:02 nucliadb/tests/unit/common/cluster/standalone/test_utils.py
+-rw-r--r--  2.0 unx      833 b- defN 24-Apr-18 08:02 nucliadb/tests/unit/common/maindb/__init__.py
+-rw-r--r--  2.0 unx     3579 b- defN 24-Apr-18 08:02 nucliadb/tests/unit/common/maindb/test_driver.py
+-rw-r--r--  2.0 unx     1869 b- defN 24-Apr-18 08:02 nucliadb/tests/unit/common/maindb/test_tikv.py
+-rw-r--r--  2.0 unx     2998 b- defN 24-Apr-18 08:02 nucliadb/tests/unit/common/maindb/test_utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Apr-18 08:02 nucliadb/tests/unit/export_import/__init__.py
+-rw-r--r--  2.0 unx     1435 b- defN 24-Apr-18 08:02 nucliadb/tests/unit/export_import/test_datamanager.py
+-rw-r--r--  2.0 unx     9706 b- defN 24-Apr-18 08:02 nucliadb/tests/unit/export_import/test_utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Apr-18 08:02 nucliadb/tests/unit/migrator/__init__.py
+-rw-r--r--  2.0 unx     3233 b- defN 24-Apr-18 08:02 nucliadb/tests/unit/migrator/test_migrator.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Apr-18 08:02 nucliadb/tests/unit/tasks/__init__.py
+-rw-r--r--  2.0 unx     1375 b- defN 24-Apr-18 08:02 nucliadb/tests/unit/tasks/conftest.py
+-rw-r--r--  2.0 unx     2714 b- defN 24-Apr-18 08:02 nucliadb/tests/unit/tasks/test_consumer.py
+-rw-r--r--  2.0 unx     3189 b- defN 24-Apr-18 08:02 nucliadb/tests/unit/tasks/test_producer.py
+-rw-r--r--  2.0 unx     1827 b- defN 24-Apr-18 08:02 nucliadb/tests/unit/tasks/test_tasks.py
+-rw-r--r--  2.0 unx     2507 b- defN 24-Apr-18 08:02 nucliadb/tests/utils/__init__.py
+-rw-r--r--  2.0 unx     1797 b- defN 24-Apr-18 08:02 nucliadb/tests/utils/aiohttp_session.py
+-rw-r--r--  2.0 unx     2533 b- defN 24-Apr-18 08:02 nucliadb/tests/utils/entities.py
+-rw-r--r--  2.0 unx     6145 b- defN 24-Apr-18 08:02 nucliadb/tests/utils/broker_messages/__init__.py
+-rw-r--r--  2.0 unx     6795 b- defN 24-Apr-18 08:02 nucliadb/tests/utils/broker_messages/fields.py
+-rw-r--r--  2.0 unx     1196 b- defN 24-Apr-18 08:02 nucliadb/tests/utils/broker_messages/helpers.py
+-rw-r--r--  2.0 unx     1325 b- defN 24-Apr-18 08:02 nucliadb/train/__init__.py
+-rw-r--r--  2.0 unx     3530 b- defN 24-Apr-18 08:02 nucliadb/train/app.py
+-rw-r--r--  2.0 unx     3800 b- defN 24-Apr-18 08:02 nucliadb/train/generator.py
+-rw-r--r--  2.0 unx     1698 b- defN 24-Apr-18 08:02 nucliadb/train/lifecycle.py
+-rw-r--r--  2.0 unx     1198 b- defN 24-Apr-18 08:02 nucliadb/train/models.py
+-rw-r--r--  2.0 unx     5706 b- defN 24-Apr-18 08:02 nucliadb/train/nodes.py
+-rw-r--r--  2.0 unx     1400 b- defN 24-Apr-18 08:02 nucliadb/train/run.py
+-rw-r--r--  2.0 unx     5926 b- defN 24-Apr-18 08:02 nucliadb/train/servicer.py
+-rw-r--r--  2.0 unx     1415 b- defN 24-Apr-18 08:02 nucliadb/train/settings.py
+-rw-r--r--  2.0 unx     1496 b- defN 24-Apr-18 08:02 nucliadb/train/types.py
+-rw-r--r--  2.0 unx     3265 b- defN 24-Apr-18 08:02 nucliadb/train/upload.py
+-rw-r--r--  2.0 unx     6420 b- defN 24-Apr-18 08:02 nucliadb/train/uploader.py
+-rw-r--r--  2.0 unx     3179 b- defN 24-Apr-18 08:02 nucliadb/train/utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Apr-18 08:02 nucliadb/train/api/__init__.py
+-rw-r--r--  2.0 unx     1479 b- defN 24-Apr-18 08:02 nucliadb/train/api/utils.py
+-rw-r--r--  2.0 unx      928 b- defN 24-Apr-18 08:02 nucliadb/train/api/v1/__init__.py
+-rw-r--r--  2.0 unx     2065 b- defN 24-Apr-18 08:02 nucliadb/train/api/v1/check.py
+-rw-r--r--  2.0 unx      910 b- defN 24-Apr-18 08:02 nucliadb/train/api/v1/router.py
+-rw-r--r--  2.0 unx     1905 b- defN 24-Apr-18 08:02 nucliadb/train/api/v1/shards.py
+-rw-r--r--  2.0 unx     2129 b- defN 24-Apr-18 08:02 nucliadb/train/api/v1/trainset.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Apr-18 08:02 nucliadb/train/generators/__init__.py
+-rw-r--r--  2.0 unx     3723 b- defN 24-Apr-18 08:02 nucliadb/train/generators/field_classifier.py
+-rw-r--r--  2.0 unx     6712 b- defN 24-Apr-18 08:02 nucliadb/train/generators/image_classifier.py
+-rw-r--r--  2.0 unx     2789 b- defN 24-Apr-18 08:02 nucliadb/train/generators/paragraph_classifier.py
+-rw-r--r--  2.0 unx     3590 b- defN 24-Apr-18 08:02 nucliadb/train/generators/paragraph_streaming.py
+-rw-r--r--  2.0 unx     5372 b- defN 24-Apr-18 08:02 nucliadb/train/generators/question_answer_streaming.py
+-rw-r--r--  2.0 unx     5160 b- defN 24-Apr-18 08:02 nucliadb/train/generators/sentence_classifier.py
+-rw-r--r--  2.0 unx    10446 b- defN 24-Apr-18 08:02 nucliadb/train/generators/token_classifier.py
+-rw-r--r--  2.0 unx     3877 b- defN 24-Apr-18 08:02 nucliadb/train/generators/utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Apr-18 08:02 nucliadb/train/tests/__init__.py
+-rw-r--r--  2.0 unx     1125 b- defN 24-Apr-18 08:02 nucliadb/train/tests/conftest.py
+-rw-r--r--  2.0 unx    11053 b- defN 24-Apr-18 08:02 nucliadb/train/tests/fixtures.py
+-rw-r--r--  2.0 unx     4598 b- defN 24-Apr-18 08:02 nucliadb/train/tests/test_field_classification.py
+-rw-r--r--  2.0 unx     2729 b- defN 24-Apr-18 08:02 nucliadb/train/tests/test_get_entities.py
+-rw-r--r--  2.0 unx     1876 b- defN 24-Apr-18 08:02 nucliadb/train/tests/test_get_info.py
+-rw-r--r--  2.0 unx     1382 b- defN 24-Apr-18 08:02 nucliadb/train/tests/test_get_ontology.py
+-rw-r--r--  2.0 unx     2417 b- defN 24-Apr-18 08:02 nucliadb/train/tests/test_get_ontology_count.py
+-rw-r--r--  2.0 unx     7669 b- defN 24-Apr-18 08:02 nucliadb/train/tests/test_image_classification.py
+-rw-r--r--  2.0 unx     1416 b- defN 24-Apr-18 08:02 nucliadb/train/tests/test_list_fields.py
+-rw-r--r--  2.0 unx     2944 b- defN 24-Apr-18 08:02 nucliadb/train/tests/test_list_paragraphs.py
+-rw-r--r--  2.0 unx     1423 b- defN 24-Apr-18 08:02 nucliadb/train/tests/test_list_resources.py
+-rw-r--r--  2.0 unx     2947 b- defN 24-Apr-18 08:02 nucliadb/train/tests/test_list_sentences.py
+-rw-r--r--  2.0 unx     4645 b- defN 24-Apr-18 08:02 nucliadb/train/tests/test_paragraph_classification.py
+-rw-r--r--  2.0 unx     4320 b- defN 24-Apr-18 08:02 nucliadb/train/tests/test_paragraph_streaming.py
+-rw-r--r--  2.0 unx     8751 b- defN 24-Apr-18 08:02 nucliadb/train/tests/test_question_answer_streaming.py
+-rw-r--r--  2.0 unx     5051 b- defN 24-Apr-18 08:02 nucliadb/train/tests/test_sentence_classification.py
+-rw-r--r--  2.0 unx     5583 b- defN 24-Apr-18 08:02 nucliadb/train/tests/test_token_classification.py
+-rw-r--r--  2.0 unx     3324 b- defN 24-Apr-18 08:02 nucliadb/train/tests/utils.py
+-rw-r--r--  2.0 unx     1328 b- defN 24-Apr-18 08:02 nucliadb/writer/__init__.py
+-rw-r--r--  2.0 unx     4268 b- defN 24-Apr-18 08:02 nucliadb/writer/app.py
+-rw-r--r--  2.0 unx    19435 b- defN 24-Apr-18 08:02 nucliadb/writer/back_pressure.py
+-rw-r--r--  2.0 unx      972 b- defN 24-Apr-18 08:02 nucliadb/writer/exceptions.py
+-rw-r--r--  2.0 unx     1953 b- defN 24-Apr-18 08:02 nucliadb/writer/lifecycle.py
+-rw-r--r--  2.0 unx     1032 b- defN 24-Apr-18 08:02 nucliadb/writer/openapi.py
+-rw-r--r--  2.0 unx     1448 b- defN 24-Apr-18 08:02 nucliadb/writer/run.py
+-rw-r--r--  2.0 unx     3074 b- defN 24-Apr-18 08:02 nucliadb/writer/settings.py
+-rw-r--r--  2.0 unx     1036 b- defN 24-Apr-18 08:02 nucliadb/writer/utilities.py
+-rw-r--r--  2.0 unx     1948 b- defN 24-Apr-18 08:02 nucliadb/writer/vectors.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Apr-18 08:02 nucliadb/writer/api/__init__.py
+-rw-r--r--  2.0 unx     1429 b- defN 24-Apr-18 08:02 nucliadb/writer/api/constants.py
+-rw-r--r--  2.0 unx     1095 b- defN 24-Apr-18 08:02 nucliadb/writer/api/v1/__init__.py
+-rw-r--r--  2.0 unx     6565 b- defN 24-Apr-18 08:02 nucliadb/writer/api/v1/export_import.py
+-rw-r--r--  2.0 unx    28320 b- defN 24-Apr-18 08:02 nucliadb/writer/api/v1/field.py
+-rw-r--r--  2.0 unx     5239 b- defN 24-Apr-18 08:02 nucliadb/writer/api/v1/knowledgebox.py
+-rw-r--r--  2.0 unx     2052 b- defN 24-Apr-18 08:02 nucliadb/writer/api/v1/learning_config.py
+-rw-r--r--  2.0 unx    19940 b- defN 24-Apr-18 08:02 nucliadb/writer/api/v1/resource.py
+-rw-r--r--  2.0 unx     1034 b- defN 24-Apr-18 08:02 nucliadb/writer/api/v1/router.py
+-rw-r--r--  2.0 unx    12733 b- defN 24-Apr-18 08:02 nucliadb/writer/api/v1/services.py
+-rw-r--r--  2.0 unx    31464 b- defN 24-Apr-18 08:02 nucliadb/writer/api/v1/upload.py
+-rw-r--r--  2.0 unx     1612 b- defN 24-Apr-18 08:02 nucliadb/writer/layouts/__init__.py
+-rw-r--r--  2.0 unx     2115 b- defN 24-Apr-18 08:02 nucliadb/writer/layouts/v1.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Apr-18 08:02 nucliadb/writer/resource/__init__.py
+-rw-r--r--  2.0 unx     1425 b- defN 24-Apr-18 08:02 nucliadb/writer/resource/audit.py
+-rw-r--r--  2.0 unx    10968 b- defN 24-Apr-18 08:02 nucliadb/writer/resource/basic.py
+-rw-r--r--  2.0 unx    16319 b- defN 24-Apr-18 08:02 nucliadb/writer/resource/field.py
+-rw-r--r--  2.0 unx     2022 b- defN 24-Apr-18 08:02 nucliadb/writer/resource/origin.py
+-rw-r--r--  2.0 unx     1152 b- defN 24-Apr-18 08:02 nucliadb/writer/resource/slug.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Apr-18 08:02 nucliadb/writer/tests/__init__.py
+-rw-r--r--  2.0 unx     1200 b- defN 24-Apr-18 08:02 nucliadb/writer/tests/conftest.py
+-rw-r--r--  2.0 unx     5971 b- defN 24-Apr-18 08:02 nucliadb/writer/tests/fixtures.py
+-rw-r--r--  2.0 unx    15472 b- defN 24-Apr-18 08:02 nucliadb/writer/tests/test_fields.py
+-rw-r--r--  2.0 unx    25913 b- defN 24-Apr-18 08:02 nucliadb/writer/tests/test_files.py
+-rw-r--r--  2.0 unx     1729 b- defN 24-Apr-18 08:02 nucliadb/writer/tests/test_knowledgebox.py
+-rw-r--r--  2.0 unx     4569 b- defN 24-Apr-18 08:02 nucliadb/writer/tests/test_reprocess_file_field.py
+-rw-r--r--  2.0 unx    17449 b- defN 24-Apr-18 08:02 nucliadb/writer/tests/test_resources.py
+-rw-r--r--  2.0 unx     5120 b- defN 24-Apr-18 08:02 nucliadb/writer/tests/test_service.py
+-rw-r--r--  2.0 unx     6054 b- defN 24-Apr-18 08:02 nucliadb/writer/tests/test_tus.py
+-rw-r--r--  2.0 unx     1287 b- defN 24-Apr-18 08:02 nucliadb/writer/tests/utils.py
+-rw-r--r--  2.0 unx     5226 b- defN 24-Apr-18 08:02 nucliadb/writer/tus/__init__.py
+-rw-r--r--  2.0 unx     5082 b- defN 24-Apr-18 08:02 nucliadb/writer/tus/dm.py
+-rw-r--r--  2.0 unx     2186 b- defN 24-Apr-18 08:02 nucliadb/writer/tus/exceptions.py
+-rw-r--r--  2.0 unx    14527 b- defN 24-Apr-18 08:02 nucliadb/writer/tus/gcs.py
+-rw-r--r--  2.0 unx     5849 b- defN 24-Apr-18 08:02 nucliadb/writer/tus/local.py
+-rw-r--r--  2.0 unx     4367 b- defN 24-Apr-18 08:02 nucliadb/writer/tus/pg.py
+-rw-r--r--  2.0 unx     9069 b- defN 24-Apr-18 08:02 nucliadb/writer/tus/s3.py
+-rw-r--r--  2.0 unx     4734 b- defN 24-Apr-18 08:02 nucliadb/writer/tus/storage.py
+-rw-r--r--  2.0 unx     2556 b- defN 24-Apr-18 08:02 nucliadb/writer/tus/utils.py
+-rw-r--r--  2.0 unx     4348 b- defN 24-Apr-18 08:03 nucliadb-3.0.3.post437.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-18 08:03 nucliadb-3.0.3.post437.dist-info/WHEEL
+-rw-r--r--  2.0 unx     1268 b- defN 24-Apr-18 08:03 nucliadb-3.0.3.post437.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       20 b- defN 24-Apr-18 08:03 nucliadb-3.0.3.post437.dist-info/top_level.txt
+-rw-r--r--  2.0 unx        1 b- defN 24-Apr-18 08:03 nucliadb-3.0.3.post437.dist-info/zip-safe
+-rw-rw-r--  2.0 unx    42447 b- defN 24-Apr-18 08:03 nucliadb-3.0.3.post437.dist-info/RECORD
+453 files, 2232244 bytes uncompressed, 681793 bytes compressed:  69.5%
```

## zipnote {}

```diff
@@ -42,14 +42,17 @@
 
 Filename: migrations/0016_upgrade_to_paragraphs_v2.py
 Comment: 
 
 Filename: migrations/0017_multiple_writable_shards.py
 Comment: 
 
+Filename: migrations/0018_purge_orphan_kbslugs.py
+Comment: 
+
 Filename: migrations/__init__.py
 Comment: 
 
 Filename: nucliadb/__init__.py
 Comment: 
 
 Filename: nucliadb/health.py
@@ -921,14 +924,17 @@
 
 Filename: nucliadb/tests/migrations/__init__.py
 Comment: 
 
 Filename: nucliadb/tests/migrations/test_migration_0017.py
 Comment: 
 
+Filename: nucliadb/tests/migrations/test_migration_0018.py
+Comment: 
+
 Filename: nucliadb/tests/unit/__init__.py
 Comment: 
 
 Filename: nucliadb/tests/unit/test_field_ids.py
 Comment: 
 
 Filename: nucliadb/tests/unit/test_health.py
@@ -1329,26 +1335,26 @@
 
 Filename: nucliadb/writer/tus/storage.py
 Comment: 
 
 Filename: nucliadb/writer/tus/utils.py
 Comment: 
 
-Filename: nucliadb-3.0.3.post436.dist-info/METADATA
+Filename: nucliadb-3.0.3.post437.dist-info/METADATA
 Comment: 
 
-Filename: nucliadb-3.0.3.post436.dist-info/WHEEL
+Filename: nucliadb-3.0.3.post437.dist-info/WHEEL
 Comment: 
 
-Filename: nucliadb-3.0.3.post436.dist-info/entry_points.txt
+Filename: nucliadb-3.0.3.post437.dist-info/entry_points.txt
 Comment: 
 
-Filename: nucliadb-3.0.3.post436.dist-info/top_level.txt
+Filename: nucliadb-3.0.3.post437.dist-info/top_level.txt
 Comment: 
 
-Filename: nucliadb-3.0.3.post436.dist-info/zip-safe
+Filename: nucliadb-3.0.3.post437.dist-info/zip-safe
 Comment: 
 
-Filename: nucliadb-3.0.3.post436.dist-info/RECORD
+Filename: nucliadb-3.0.3.post437.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## nucliadb/ingest/orm/knowledgebox.py

```diff
@@ -88,15 +88,14 @@
         else:
             return self._config
 
     @classmethod
     async def delete_kb(cls, txn: Transaction, slug: str = "", kbid: str = ""):
         # Mark storage to be deleted
         # Mark keys to be deleted
-        logger.info(f"Deleting KB kbid={kbid} slug={slug}")
         if not kbid and not slug:
             raise AttributeError()
 
         if slug and not kbid:
             kbid_bytes = await txn.get(datamanagers.kb.KB_SLUGS.format(slug=slug))
             if kbid_bytes is None:
                 raise datamanagers.exceptions.KnowledgeBoxNotFound()
@@ -109,15 +108,14 @@
             pbconfig = KnowledgeBoxConfig()
             pbconfig.ParseFromString(kbconfig_bytes)
             slug = pbconfig.slug
 
         # Delete main anchor
         async with txn.driver.transaction() as subtxn:
             key_match = datamanagers.kb.KB_SLUGS.format(slug=slug)
-            logger.info(f"Deleting KB with slug: {slug}")
             await subtxn.delete(key_match)
 
             when = datetime.now().isoformat()
             await subtxn.set(KB_TO_DELETE.format(kbid=kbid), when.encode())
             await subtxn.commit()
 
         audit_util = get_audit()
```

## nucliadb/tests/migrations/__init__.py

```diff
@@ -13,7 +13,18 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU Affero General Public License for more details.
 #
 # You should have received a copy of the GNU Affero General Public License
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
 #
+
+from nucliadb.migrator.models import Migration
+from nucliadb.migrator.utils import get_migrations
+
+
+def get_migration(version: int) -> Migration:
+    migration: Migration = get_migrations(from_version=version - 1, to_version=version)[
+        0
+    ]
+    assert migration.version == version
+    return migration
```

## nucliadb/tests/migrations/test_migration_0017.py

```diff
@@ -20,22 +20,18 @@
 from unittest.mock import Mock
 
 import pytest
 
 from nucliadb.common import datamanagers
 from nucliadb.common.maindb.driver import Driver
 from nucliadb.migrator.models import Migration
-from nucliadb.migrator.utils import get_migrations
+from nucliadb.tests.migrations import get_migration
 from nucliadb_protos import writer_pb2
 
-MIGRATION_UNDER_TEST = 17
-migration: Migration = get_migrations(
-    from_version=MIGRATION_UNDER_TEST - 1, to_version=MIGRATION_UNDER_TEST
-)[0]
-assert migration.version == MIGRATION_UNDER_TEST
+migration: Migration = get_migration(17)
 
 
 @pytest.mark.asyncio
 async def test_migration_0017_kb(maindb_driver: Driver):
     execution_context = Mock()
     execution_context.kv_driver = maindb_driver
```

## Comparing `nucliadb-3.0.3.post436.dist-info/METADATA` & `nucliadb-3.0.3.post437.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nucliadb
-Version: 3.0.3.post436
+Version: 3.0.3.post437
 Home-page: https://docs.nuclia.dev/docs/guides/nucliadb/intro
 Author: NucliaDB Community
 Author-email: nucliadb@nuclia.com
 License: BSD
 Project-URL: Nuclia, https://nuclia.com
 Project-URL: Github, https://github.com/nuclia/nucliadb
 Project-URL: Discord, https://discord.gg/8EvQwmsbzf
@@ -17,18 +17,18 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.9, <4
 Description-Content-Type: text/markdown
-Requires-Dist: nucliadb-telemetry[all] >=3.0.3.post436
-Requires-Dist: nucliadb-utils[cache,fastapi,storages] >=3.0.3.post436
-Requires-Dist: nucliadb-protos >=3.0.3.post436
-Requires-Dist: nucliadb-models >=3.0.3.post436
+Requires-Dist: nucliadb-telemetry[all] >=3.0.3.post437
+Requires-Dist: nucliadb-utils[cache,fastapi,storages] >=3.0.3.post437
+Requires-Dist: nucliadb-protos >=3.0.3.post437
+Requires-Dist: nucliadb-models >=3.0.3.post437
 Requires-Dist: nucliadb-admin-assets >=1.0.0.post1224
 Requires-Dist: nucliadb-node-binding >=2.26.0
 Requires-Dist: uvicorn <0.19.0
 Requires-Dist: pydantic-argparse
 Requires-Dist: aiohttp >=3.9.3
 Requires-Dist: lru-dict >=1.1.7
 Requires-Dist: backoff
```

## Comparing `nucliadb-3.0.3.post436.dist-info/entry_points.txt` & `nucliadb-3.0.3.post437.dist-info/entry_points.txt`

 * *Files identical despite different names*

## Comparing `nucliadb-3.0.3.post436.dist-info/RECORD` & `nucliadb-3.0.3.post437.dist-info/RECORD`

 * *Files 1% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 migrations/0011_materialize_labelset_ids.py,sha256=nu9mzkwwVD3mw-_jE6YJZAV8r2gXfigL-wUzIaR8iiw,1843
 migrations/0012_rollover_shards.py,sha256=3ShFPB11vFEYvso5vc8NZwYhXwuA0R4inA16k15GAkI,1443
 migrations/0013_rollover_shards.py,sha256=c3IU8zinlWeVRN8T6o5eLpvGzkQOHX_Yz5xuFVRUy5U,1024
 migrations/0014_rollover_shards.py,sha256=24yLtXAwlVvCwtHLx9Tz-VWCzeMuy-0o3M6QNESi_Iw,1382
 migrations/0015_targeted_rollover.py,sha256=7C9XM8wg-bpkNyFh0xJuaGzOcE2WqU1BfqtInKAjTkw,1462
 migrations/0016_upgrade_to_paragraphs_v2.py,sha256=pOZUwTDfGoLjcSSKiWaN6FUvMDN95XNCBoux3u0dsmQ,2506
 migrations/0017_multiple_writable_shards.py,sha256=NY38wFVxSDXglkZE6DRnuN1DG_1kyZXr2j37C8VhyA0,2100
+migrations/0018_purge_orphan_kbslugs.py,sha256=3x5OsMb-JnP9y8_-ztYugk1RiXbOuthTFB-8I1XX3bk,2264
 migrations/__init__.py,sha256=cp15ZcFnHvpcu_5-aK2A4uUyvuZVV_MJn4bIXMa20ks,835
 nucliadb/__init__.py,sha256=_abCmDJ_0ku483Os4UAjPX7Nywm39cQgAV_DiyjsKeQ,891
 nucliadb/health.py,sha256=zPwd3CAFJf9owhbadtyGLvHekOjX9ykvxLYWYxnD5eo,3733
 nucliadb/learning_proxy.py,sha256=RVuBDsI2zbU53x2fnl965aZF8FV3GhI5J7b8TfX6mN4,10590
 nucliadb/metrics_exporter.py,sha256=PummIqtRLdpcONPIpRKBj_jGYnX7B9XZ2IO048bu2pM,4806
 nucliadb/openapi.py,sha256=wDiw0dVEvTpJvbatkJ0JZLkKm9RItZT5PWRHjqRfqTA,2272
 nucliadb/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
@@ -107,15 +108,15 @@
 nucliadb/ingest/fields/layout.py,sha256=clgBVGWArtkAEawDqCAu_hB9gVu5c6UT1Cf_5yrw47s,2250
 nucliadb/ingest/fields/link.py,sha256=6D1jlwX1ImU3RL1dVawXm2ChoB_s1_h5DOVGyW4q37M,4084
 nucliadb/ingest/fields/text.py,sha256=qMMH76gN--Ag1fPZ1I5G9ZPAi4U0i9jbqlrpYc3cMxg,1319
 nucliadb/ingest/orm/__init__.py,sha256=cp15ZcFnHvpcu_5-aK2A4uUyvuZVV_MJn4bIXMa20ks,835
 nucliadb/ingest/orm/brain.py,sha256=Ox5IxnQsJcJzi5B8Q35zmyT2W-htFSUjX5C1PaKZH4E,27582
 nucliadb/ingest/orm/entities.py,sha256=q027LfocE-KIqRNC1ZOSrrvt6x9NGrB25TZsOe0SyVk,15758
 nucliadb/ingest/orm/exceptions.py,sha256=GKr20V5xLv-WHBBHhr8lBChpW5oa9k18Xuiw-dIF9DM,1279
-nucliadb/ingest/orm/knowledgebox.py,sha256=TrDagvZ88vNFJVZIyySNuSEt0s7b4nttwgRG6r-hvKM,18865
+nucliadb/ingest/orm/knowledgebox.py,sha256=XJPAUNiV1lai20RQ4CF9JEIcuPuuSCUADSijNNeHs1o,18747
 nucliadb/ingest/orm/metrics.py,sha256=OkwMSPKLZcKba0ZTwtTiIxwBgaLMX5ydhGieKvi2y7E,1096
 nucliadb/ingest/orm/resource.py,sha256=AwWlzVrXYxZMnvn9ECA9KFMI5etFoEoFCIjkHaNpH58,60085
 nucliadb/ingest/orm/synonyms.py,sha256=tyOEGPfuJwhM5iYm4uNPjc2E8oWPk70DzZeuxVZ5alQ,1739
 nucliadb/ingest/orm/utils.py,sha256=VMLhujH4kihWiSvCPCiGAvGxqTZBh8RGn_9CZUUIELI,3074
 nucliadb/ingest/orm/processor/__init__.py,sha256=rdd6Eec4C3yhQYcrHLgwngLk3amMpih5h3N_8hYjqNk,26460
 nucliadb/ingest/orm/processor/sequence_manager.py,sha256=Mc9SA_NfzxTwovD5yGiAcdmen4pa-QNdsYcONIWeZPc,1690
 nucliadb/ingest/service/__init__.py,sha256=C_lkkjoHm0hDT2fZjEN4mpwXtU4bWthB-vM5-28-MBM,2057
@@ -301,16 +302,17 @@
 nucliadb/tests/fixtures.py,sha256=XS9go2JZbTXz3hAdgSuCC8ya2htqdK3O73w_mU6yY68,22365
 nucliadb/tests/tikv.py,sha256=MGwBL9ezcOOR8JwttouQ8Qj6534d742i2A3TAumdrM4,7549
 nucliadb/tests/benchmarks/__init__.py,sha256=cp15ZcFnHvpcu_5-aK2A4uUyvuZVV_MJn4bIXMa20ks,835
 nucliadb/tests/benchmarks/test_search.py,sha256=1Icz4bXwLJtzZGnc8xY4bXmVmgWJGXmv0Zq0NlZHIuk,3032
 nucliadb/tests/knowledgeboxes/__init__.py,sha256=u4paaCDL4YOUPUW5iZOzP72yMkdqTA_dMr6hRQEnf5k,919
 nucliadb/tests/knowledgeboxes/philosophy_books.py,sha256=CFPR5ARHpaWJm8KA5gPmSmrUyZBHCaFfuhkQFpmZKbM,7002
 nucliadb/tests/knowledgeboxes/ten_dummy_resources.py,sha256=8yvWnAcYrlHTvfEntN9309LHFqchLd1BTIGKimFQab0,3037
-nucliadb/tests/migrations/__init__.py,sha256=cp15ZcFnHvpcu_5-aK2A4uUyvuZVV_MJn4bIXMa20ks,835
-nucliadb/tests/migrations/test_migration_0017.py,sha256=dHcomKzvCUP1m7VN4dblWmiEIeho_aPSu4mEi4oZQUg,2878
+nucliadb/tests/migrations/__init__.py,sha256=1alcOjjpC6F2MmwnUGz3O4DQ0AbuMKtkkDsVbRyQec8,1148
+nucliadb/tests/migrations/test_migration_0017.py,sha256=U0Fy7bjwn61hfUZ-K9SYty6_dwS55V3E1r18UjFuNdM,2726
+nucliadb/tests/migrations/test_migration_0018.py,sha256=GrfCyTNfEE7E2Jy9sfjUBJ3Gs87XZdgf_rjQkdn13Ck,3625
 nucliadb/tests/unit/__init__.py,sha256=cp15ZcFnHvpcu_5-aK2A4uUyvuZVV_MJn4bIXMa20ks,835
 nucliadb/tests/unit/test_field_ids.py,sha256=pwtHELSrfGtmKI3n4HBtsiRZFHlps6z2Nlb4kc7p5p4,1487
 nucliadb/tests/unit/test_health.py,sha256=wkGz2C5zENNMK63Esb439cNhaUhsYV3i4hY3ExugEQc,2758
 nucliadb/tests/unit/test_kb_slugs.py,sha256=XlifR2gz0e1WmqjMiCah0D7YXoceF1Sn8WGXqxGEeD8,1543
 nucliadb/tests/unit/test_learning_proxy.py,sha256=e3-wL_gsv0nQoChfvHR6NfDqSBzesnoq5MeGaHjzyNM,7892
 nucliadb/tests/unit/test_metrics_exporter.py,sha256=t__hVxV0Fo0duKtnJQl7BjyOXtP7QcD0pzHD9936z4o,2642
 nucliadb/tests/unit/test_openapi.py,sha256=ivwIs7UcTDfGyWD85VtzcmurPyU-ez9hvEmSCfFexrs,1341
@@ -439,13 +441,13 @@
 nucliadb/writer/tus/exceptions.py,sha256=CmxYKnHXpXug25DYV4SpVAU47SGD-NVBd7pNTRbWHyk,2186
 nucliadb/writer/tus/gcs.py,sha256=WykJZicWKRYkVB5_Fkb_1cVLovAk86IVkEn1VgEDufc,14527
 nucliadb/writer/tus/local.py,sha256=lIOoGaylnsxPBYGskcmKSHv7MsvwIYFS4soDLey_KSs,5849
 nucliadb/writer/tus/pg.py,sha256=JUK_xKsyNcKAvWOch8gUMTc_e1evI_3aC6-Y5gMk2jw,4367
 nucliadb/writer/tus/s3.py,sha256=a9mfPtjBW3QaTYY2r6P7u_Y13V6mBefZjWgV4juZzgE,9069
 nucliadb/writer/tus/storage.py,sha256=8iBOjWIcY6PawQq_rmSiBKi0Gl6J6Q5ad6L-9nLCcJ4,4734
 nucliadb/writer/tus/utils.py,sha256=MSdVbRsRSZVdkaum69_0wku7X3p5wlZf4nr6E0GMKbw,2556
-nucliadb-3.0.3.post436.dist-info/METADATA,sha256=lJVzByZQqy8hd95xw4PRuEJ2SPqFq7MofoExU5bb50U,4348
-nucliadb-3.0.3.post436.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-nucliadb-3.0.3.post436.dist-info/entry_points.txt,sha256=XqGfgFDuY3zXQc8ewXM2TRVjTModIq851zOsgrmaXx4,1268
-nucliadb-3.0.3.post436.dist-info/top_level.txt,sha256=hwYhTVnX7jkQ9gJCkVrbqEG1M4lT2F_iPQND1fCzF80,20
-nucliadb-3.0.3.post436.dist-info/zip-safe,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
-nucliadb-3.0.3.post436.dist-info/RECORD,,
+nucliadb-3.0.3.post437.dist-info/METADATA,sha256=YXcSvvI4iPzl7MMfIzDoeqPUnrFJYkv_wNdrOn1eyhs,4348
+nucliadb-3.0.3.post437.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+nucliadb-3.0.3.post437.dist-info/entry_points.txt,sha256=XqGfgFDuY3zXQc8ewXM2TRVjTModIq851zOsgrmaXx4,1268
+nucliadb-3.0.3.post437.dist-info/top_level.txt,sha256=hwYhTVnX7jkQ9gJCkVrbqEG1M4lT2F_iPQND1fCzF80,20
+nucliadb-3.0.3.post437.dist-info/zip-safe,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
+nucliadb-3.0.3.post437.dist-info/RECORD,,
```

