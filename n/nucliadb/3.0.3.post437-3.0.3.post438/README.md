# Comparing `tmp/nucliadb-3.0.3.post437-py3-none-any.whl.zip` & `tmp/nucliadb-3.0.3.post438-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,455 +1,458 @@
-Zip file size: 749659 bytes, number of entries: 453
--rw-r--r--  2.0 unx     1135 b- defN 24-Apr-18 08:02 migrations/0001_bootstrap.py
--rw-r--r--  2.0 unx     1177 b- defN 24-Apr-18 08:02 migrations/0002_rollover_shards.py
--rw-r--r--  2.0 unx     2436 b- defN 24-Apr-18 08:02 migrations/0003_allfields_key.py
--rw-r--r--  2.0 unx     1177 b- defN 24-Apr-18 08:02 migrations/0004_rollover_shards.py
--rw-r--r--  2.0 unx     1177 b- defN 24-Apr-18 08:02 migrations/0005_rollover_shards.py
--rw-r--r--  2.0 unx     1024 b- defN 24-Apr-18 08:02 migrations/0006_rollover_shards.py
--rw-r--r--  2.0 unx     1301 b- defN 24-Apr-18 08:02 migrations/0008_cleanup_leftover_rollover_metadata.py
--rw-r--r--  2.0 unx     1378 b- defN 24-Apr-18 08:02 migrations/0009_upgrade_relations_and_texts_to_v2.py
--rw-r--r--  2.0 unx     1610 b- defN 24-Apr-18 08:02 migrations/0010_fix_corrupt_indexes.py
--rw-r--r--  2.0 unx     1843 b- defN 24-Apr-18 08:02 migrations/0011_materialize_labelset_ids.py
--rw-r--r--  2.0 unx     1443 b- defN 24-Apr-18 08:02 migrations/0012_rollover_shards.py
--rw-r--r--  2.0 unx     1024 b- defN 24-Apr-18 08:02 migrations/0013_rollover_shards.py
--rw-r--r--  2.0 unx     1382 b- defN 24-Apr-18 08:02 migrations/0014_rollover_shards.py
--rw-r--r--  2.0 unx     1462 b- defN 24-Apr-18 08:02 migrations/0015_targeted_rollover.py
--rw-r--r--  2.0 unx     2506 b- defN 24-Apr-18 08:02 migrations/0016_upgrade_to_paragraphs_v2.py
--rw-r--r--  2.0 unx     2100 b- defN 24-Apr-18 08:02 migrations/0017_multiple_writable_shards.py
--rw-r--r--  2.0 unx     2264 b- defN 24-Apr-18 08:02 migrations/0018_purge_orphan_kbslugs.py
--rw-r--r--  2.0 unx      835 b- defN 24-Apr-18 08:02 migrations/__init__.py
--rw-r--r--  2.0 unx      891 b- defN 24-Apr-18 08:02 nucliadb/__init__.py
--rw-r--r--  2.0 unx     3733 b- defN 24-Apr-18 08:02 nucliadb/health.py
--rw-r--r--  2.0 unx    10590 b- defN 24-Apr-18 08:02 nucliadb/learning_proxy.py
--rw-r--r--  2.0 unx     4806 b- defN 24-Apr-18 08:02 nucliadb/metrics_exporter.py
--rw-r--r--  2.0 unx     2272 b- defN 24-Apr-18 08:02 nucliadb/openapi.py
--rw-r--r--  2.0 unx        0 b- defN 24-Apr-18 08:02 nucliadb/py.typed
--rw-r--r--  2.0 unx      835 b- defN 24-Apr-18 08:02 nucliadb/common/__init__.py
--rw-r--r--  2.0 unx     4905 b- defN 24-Apr-18 08:02 nucliadb/common/locking.py
--rw-r--r--  2.0 unx      835 b- defN 24-Apr-18 08:02 nucliadb/common/cluster/__init__.py
--rw-r--r--  2.0 unx     4983 b- defN 24-Apr-18 08:02 nucliadb/common/cluster/base.py
--rw-r--r--  2.0 unx     1495 b- defN 24-Apr-18 08:02 nucliadb/common/cluster/exceptions.py
--rw-r--r--  2.0 unx     3658 b- defN 24-Apr-18 08:02 nucliadb/common/cluster/grpc_node_dummy.py
--rw-r--r--  2.0 unx     3429 b- defN 24-Apr-18 08:02 nucliadb/common/cluster/index_node.py
--rw-r--r--  2.0 unx    21095 b- defN 24-Apr-18 08:02 nucliadb/common/cluster/manager.py
--rw-r--r--  2.0 unx     8490 b- defN 24-Apr-18 08:02 nucliadb/common/cluster/rebalance.py
--rw-r--r--  2.0 unx    19449 b- defN 24-Apr-18 08:02 nucliadb/common/cluster/rollover.py
--rw-r--r--  2.0 unx     2713 b- defN 24-Apr-18 08:02 nucliadb/common/cluster/settings.py
--rw-r--r--  2.0 unx     5494 b- defN 24-Apr-18 08:02 nucliadb/common/cluster/utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-Apr-18 08:02 nucliadb/common/cluster/discovery/__init__.py
--rw-r--r--  2.0 unx     6553 b- defN 24-Apr-18 08:02 nucliadb/common/cluster/discovery/base.py
--rw-r--r--  2.0 unx    12518 b- defN 24-Apr-18 08:02 nucliadb/common/cluster/discovery/k8s.py
--rw-r--r--  2.0 unx     1957 b- defN 24-Apr-18 08:02 nucliadb/common/cluster/discovery/manual.py
--rw-r--r--  2.0 unx     1737 b- defN 24-Apr-18 08:02 nucliadb/common/cluster/discovery/single.py
--rw-r--r--  2.0 unx     1139 b- defN 24-Apr-18 08:02 nucliadb/common/cluster/discovery/types.py
--rw-r--r--  2.0 unx     2548 b- defN 24-Apr-18 08:02 nucliadb/common/cluster/discovery/utils.py
--rw-r--r--  2.0 unx      833 b- defN 24-Apr-18 08:02 nucliadb/common/cluster/standalone/__init__.py
--rw-r--r--  2.0 unx    13705 b- defN 24-Apr-18 08:02 nucliadb/common/cluster/standalone/grpc_node_binding.py
--rw-r--r--  2.0 unx     4683 b- defN 24-Apr-18 08:02 nucliadb/common/cluster/standalone/index_node.py
--rw-r--r--  2.0 unx     3444 b- defN 24-Apr-18 08:02 nucliadb/common/cluster/standalone/service.py
--rw-r--r--  2.0 unx     3386 b- defN 24-Apr-18 08:02 nucliadb/common/cluster/standalone/utils.py
--rw-r--r--  2.0 unx     3498 b- defN 24-Apr-18 08:02 nucliadb/common/context/__init__.py
--rw-r--r--  2.0 unx     1628 b- defN 24-Apr-18 08:02 nucliadb/common/context/fastapi.py
--rw-r--r--  2.0 unx     1813 b- defN 24-Apr-18 08:02 nucliadb/common/datamanagers/__init__.py
--rw-r--r--  2.0 unx     1451 b- defN 24-Apr-18 08:02 nucliadb/common/datamanagers/cluster.py
--rw-r--r--  2.0 unx     5383 b- defN 24-Apr-18 08:02 nucliadb/common/datamanagers/entities.py
--rw-r--r--  2.0 unx      883 b- defN 24-Apr-18 08:02 nucliadb/common/datamanagers/exceptions.py
--rw-r--r--  2.0 unx     2940 b- defN 24-Apr-18 08:02 nucliadb/common/datamanagers/kb.py
--rw-r--r--  2.0 unx     5389 b- defN 24-Apr-18 08:02 nucliadb/common/datamanagers/labels.py
--rw-r--r--  2.0 unx     1599 b- defN 24-Apr-18 08:02 nucliadb/common/datamanagers/processing.py
--rw-r--r--  2.0 unx     7637 b- defN 24-Apr-18 08:02 nucliadb/common/datamanagers/resources.py
--rw-r--r--  2.0 unx     5633 b- defN 24-Apr-18 08:02 nucliadb/common/datamanagers/rollover.py
--rw-r--r--  2.0 unx     1681 b- defN 24-Apr-18 08:02 nucliadb/common/datamanagers/utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-Apr-18 08:02 nucliadb/common/http_clients/__init__.py
--rw-r--r--  2.0 unx     2146 b- defN 24-Apr-18 08:02 nucliadb/common/http_clients/auth.py
--rw-r--r--  2.0 unx     1100 b- defN 24-Apr-18 08:02 nucliadb/common/http_clients/exceptions.py
--rw-r--r--  2.0 unx     7155 b- defN 24-Apr-18 08:02 nucliadb/common/http_clients/processing.py
--rw-r--r--  2.0 unx     1540 b- defN 24-Apr-18 08:02 nucliadb/common/http_clients/pypi.py
--rw-r--r--  2.0 unx     1551 b- defN 24-Apr-18 08:02 nucliadb/common/http_clients/utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-Apr-18 08:02 nucliadb/common/maindb/__init__.py
--rw-r--r--  2.0 unx     3449 b- defN 24-Apr-18 08:02 nucliadb/common/maindb/driver.py
--rw-r--r--  2.0 unx      946 b- defN 24-Apr-18 08:02 nucliadb/common/maindb/exceptions.py
--rw-r--r--  2.0 unx     6769 b- defN 24-Apr-18 08:02 nucliadb/common/maindb/local.py
--rw-r--r--  2.0 unx     8391 b- defN 24-Apr-18 08:02 nucliadb/common/maindb/pg.py
--rw-r--r--  2.0 unx     6053 b- defN 24-Apr-18 08:02 nucliadb/common/maindb/redis.py
--rw-r--r--  2.0 unx    14502 b- defN 24-Apr-18 08:02 nucliadb/common/maindb/tikv.py
--rw-r--r--  2.0 unx     4109 b- defN 24-Apr-18 08:02 nucliadb/common/maindb/utils.py
--rw-r--r--  2.0 unx      932 b- defN 24-Apr-18 08:02 nucliadb/export_import/__init__.py
--rw-r--r--  2.0 unx     6171 b- defN 24-Apr-18 08:02 nucliadb/export_import/datamanager.py
--rw-r--r--  2.0 unx     1949 b- defN 24-Apr-18 08:02 nucliadb/export_import/exceptions.py
--rw-r--r--  2.0 unx     7116 b- defN 24-Apr-18 08:02 nucliadb/export_import/exporter.py
--rw-r--r--  2.0 unx     4258 b- defN 24-Apr-18 08:02 nucliadb/export_import/importer.py
--rw-r--r--  2.0 unx     2063 b- defN 24-Apr-18 08:02 nucliadb/export_import/models.py
--rw-r--r--  2.0 unx     2571 b- defN 24-Apr-18 08:02 nucliadb/export_import/tasks.py
--rw-r--r--  2.0 unx    19270 b- defN 24-Apr-18 08:02 nucliadb/export_import/utils.py
--rw-r--r--  2.0 unx     1011 b- defN 24-Apr-18 08:02 nucliadb/ingest/__init__.py
--rw-r--r--  2.0 unx     7277 b- defN 24-Apr-18 08:02 nucliadb/ingest/app.py
--rw-r--r--  2.0 unx     1005 b- defN 24-Apr-18 08:02 nucliadb/ingest/cache.py
--rw-r--r--  2.0 unx     2484 b- defN 24-Apr-18 08:02 nucliadb/ingest/partitions.py
--rw-r--r--  2.0 unx    19541 b- defN 24-Apr-18 08:02 nucliadb/ingest/processing.py
--rw-r--r--  2.0 unx    20277 b- defN 24-Apr-18 08:02 nucliadb/ingest/serialize.py
--rw-r--r--  2.0 unx     3183 b- defN 24-Apr-18 08:02 nucliadb/ingest/settings.py
--rw-r--r--  2.0 unx     2314 b- defN 24-Apr-18 08:02 nucliadb/ingest/utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-Apr-18 08:02 nucliadb/ingest/consumer/__init__.py
--rw-r--r--  2.0 unx    11563 b- defN 24-Apr-18 08:02 nucliadb/ingest/consumer/auditing.py
--rw-r--r--  2.0 unx    12159 b- defN 24-Apr-18 08:02 nucliadb/ingest/consumer/consumer.py
--rw-r--r--  2.0 unx     3788 b- defN 24-Apr-18 08:02 nucliadb/ingest/consumer/materializer.py
--rw-r--r--  2.0 unx     1075 b- defN 24-Apr-18 08:02 nucliadb/ingest/consumer/metrics.py
--rw-r--r--  2.0 unx     9543 b- defN 24-Apr-18 08:02 nucliadb/ingest/consumer/pull.py
--rw-r--r--  2.0 unx     6935 b- defN 24-Apr-18 08:02 nucliadb/ingest/consumer/service.py
--rw-r--r--  2.0 unx     4331 b- defN 24-Apr-18 08:02 nucliadb/ingest/consumer/shard_creator.py
--rw-r--r--  2.0 unx     2656 b- defN 24-Apr-18 08:02 nucliadb/ingest/consumer/utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-Apr-18 08:02 nucliadb/ingest/fields/__init__.py
--rw-r--r--  2.0 unx    18433 b- defN 24-Apr-18 08:02 nucliadb/ingest/fields/base.py
--rw-r--r--  2.0 unx     6516 b- defN 24-Apr-18 08:02 nucliadb/ingest/fields/conversation.py
--rw-r--r--  2.0 unx     1223 b- defN 24-Apr-18 08:02 nucliadb/ingest/fields/date.py
--rw-r--r--  2.0 unx     1205 b- defN 24-Apr-18 08:02 nucliadb/ingest/fields/exceptions.py
--rw-r--r--  2.0 unx     5159 b- defN 24-Apr-18 08:02 nucliadb/ingest/fields/file.py
--rw-r--r--  2.0 unx     1547 b- defN 24-Apr-18 08:02 nucliadb/ingest/fields/generic.py
--rw-r--r--  2.0 unx     1235 b- defN 24-Apr-18 08:02 nucliadb/ingest/fields/keywordset.py
--rw-r--r--  2.0 unx     2250 b- defN 24-Apr-18 08:02 nucliadb/ingest/fields/layout.py
--rw-r--r--  2.0 unx     4084 b- defN 24-Apr-18 08:02 nucliadb/ingest/fields/link.py
--rw-r--r--  2.0 unx     1319 b- defN 24-Apr-18 08:02 nucliadb/ingest/fields/text.py
--rw-r--r--  2.0 unx      835 b- defN 24-Apr-18 08:02 nucliadb/ingest/orm/__init__.py
--rw-r--r--  2.0 unx    27582 b- defN 24-Apr-18 08:02 nucliadb/ingest/orm/brain.py
--rw-r--r--  2.0 unx    15758 b- defN 24-Apr-18 08:02 nucliadb/ingest/orm/entities.py
--rw-r--r--  2.0 unx     1279 b- defN 24-Apr-18 08:02 nucliadb/ingest/orm/exceptions.py
--rw-r--r--  2.0 unx    18747 b- defN 24-Apr-18 08:02 nucliadb/ingest/orm/knowledgebox.py
--rw-r--r--  2.0 unx     1096 b- defN 24-Apr-18 08:02 nucliadb/ingest/orm/metrics.py
--rw-r--r--  2.0 unx    60085 b- defN 24-Apr-18 08:02 nucliadb/ingest/orm/resource.py
--rw-r--r--  2.0 unx     1739 b- defN 24-Apr-18 08:02 nucliadb/ingest/orm/synonyms.py
--rw-r--r--  2.0 unx     3074 b- defN 24-Apr-18 08:02 nucliadb/ingest/orm/utils.py
--rw-r--r--  2.0 unx    26460 b- defN 24-Apr-18 08:02 nucliadb/ingest/orm/processor/__init__.py
--rw-r--r--  2.0 unx     1690 b- defN 24-Apr-18 08:02 nucliadb/ingest/orm/processor/sequence_manager.py
--rw-r--r--  2.0 unx     2057 b- defN 24-Apr-18 08:02 nucliadb/ingest/service/__init__.py
--rw-r--r--  2.0 unx      835 b- defN 24-Apr-18 08:02 nucliadb/ingest/service/exceptions.py
--rw-r--r--  2.0 unx    36594 b- defN 24-Apr-18 08:02 nucliadb/ingest/service/writer.py
--rw-r--r--  2.0 unx      835 b- defN 24-Apr-18 08:02 nucliadb/ingest/tests/__init__.py
--rw-r--r--  2.0 unx     1157 b- defN 24-Apr-18 08:02 nucliadb/ingest/tests/conftest.py
--rw-r--r--  2.0 unx    24068 b- defN 24-Apr-18 08:02 nucliadb/ingest/tests/fixtures.py
--rw-r--r--  2.0 unx    62843 b- defN 24-Apr-18 08:02 nucliadb/ingest/tests/vectors.py
--rw-r--r--  2.0 unx      835 b- defN 24-Apr-18 08:02 nucliadb/ingest/tests/integration/__init__.py
--rw-r--r--  2.0 unx      833 b- defN 24-Apr-18 08:02 nucliadb/ingest/tests/integration/consumer/__init__.py
--rw-r--r--  2.0 unx     2549 b- defN 24-Apr-18 08:02 nucliadb/ingest/tests/integration/consumer/test_auditing.py
--rw-r--r--  2.0 unx     2591 b- defN 24-Apr-18 08:02 nucliadb/ingest/tests/integration/consumer/test_materializer.py
--rw-r--r--  2.0 unx     4465 b- defN 24-Apr-18 08:02 nucliadb/ingest/tests/integration/consumer/test_pull.py
--rw-r--r--  2.0 unx     2763 b- defN 24-Apr-18 08:02 nucliadb/ingest/tests/integration/consumer/test_service.py
--rw-r--r--  2.0 unx     2019 b- defN 24-Apr-18 08:02 nucliadb/ingest/tests/integration/consumer/test_shard_creator.py
--rw-r--r--  2.0 unx      835 b- defN 24-Apr-18 08:02 nucliadb/ingest/tests/integration/ingest/__init__.py
--rw-r--r--  2.0 unx    27334 b- defN 24-Apr-18 08:02 nucliadb/ingest/tests/integration/ingest/test_ingest.py
--rw-r--r--  2.0 unx     3040 b- defN 24-Apr-18 08:02 nucliadb/ingest/tests/integration/ingest/test_processing_engine.py
--rw-r--r--  2.0 unx     8586 b- defN 24-Apr-18 08:02 nucliadb/ingest/tests/integration/ingest/test_relations.py
--rw-r--r--  2.0 unx      835 b- defN 24-Apr-18 08:02 nucliadb/ingest/tests/unit/__init__.py
--rw-r--r--  2.0 unx     1189 b- defN 24-Apr-18 08:02 nucliadb/ingest/tests/unit/test_cache.py
--rw-r--r--  2.0 unx     1432 b- defN 24-Apr-18 08:02 nucliadb/ingest/tests/unit/test_partitions.py
--rw-r--r--  2.0 unx     5807 b- defN 24-Apr-18 08:02 nucliadb/ingest/tests/unit/test_processing.py
--rw-r--r--  2.0 unx      978 b- defN 24-Apr-18 08:02 nucliadb/ingest/tests/unit/test_settings.py
--rw-r--r--  2.0 unx      833 b- defN 24-Apr-18 08:02 nucliadb/ingest/tests/unit/consumer/__init__.py
--rw-r--r--  2.0 unx     3981 b- defN 24-Apr-18 08:02 nucliadb/ingest/tests/unit/consumer/test_auditing.py
--rw-r--r--  2.0 unx     2472 b- defN 24-Apr-18 08:02 nucliadb/ingest/tests/unit/consumer/test_consumer.py
--rw-r--r--  2.0 unx     2063 b- defN 24-Apr-18 08:02 nucliadb/ingest/tests/unit/consumer/test_pull.py
--rw-r--r--  2.0 unx     4075 b- defN 24-Apr-18 08:02 nucliadb/ingest/tests/unit/consumer/test_shard_creator.py
--rw-r--r--  2.0 unx     1934 b- defN 24-Apr-18 08:02 nucliadb/ingest/tests/unit/consumer/test_utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-Apr-18 08:02 nucliadb/ingest/tests/unit/orm/__init__.py
--rw-r--r--  2.0 unx     9876 b- defN 24-Apr-18 08:02 nucliadb/ingest/tests/unit/orm/test_brain.py
--rw-r--r--  2.0 unx     4045 b- defN 24-Apr-18 08:02 nucliadb/ingest/tests/unit/orm/test_processor.py
--rw-r--r--  2.0 unx     8965 b- defN 24-Apr-18 08:02 nucliadb/ingest/tests/unit/orm/test_resource.py
--rw-r--r--  2.0 unx     2216 b- defN 24-Apr-18 08:02 nucliadb/middleware/__init__.py
--rw-r--r--  2.0 unx     3912 b- defN 24-Apr-18 08:02 nucliadb/middleware/transaction.py
--rw-r--r--  2.0 unx      835 b- defN 24-Apr-18 08:02 nucliadb/migrator/__init__.py
--rw-r--r--  2.0 unx     2119 b- defN 24-Apr-18 08:02 nucliadb/migrator/command.py
--rw-r--r--  2.0 unx     1334 b- defN 24-Apr-18 08:02 nucliadb/migrator/context.py
--rw-r--r--  2.0 unx     5104 b- defN 24-Apr-18 08:02 nucliadb/migrator/datamanager.py
--rw-r--r--  2.0 unx      889 b- defN 24-Apr-18 08:02 nucliadb/migrator/exceptions.py
--rw-r--r--  2.0 unx     9237 b- defN 24-Apr-18 08:02 nucliadb/migrator/migrator.py
--rw-r--r--  2.0 unx     1145 b- defN 24-Apr-18 08:02 nucliadb/migrator/models.py
--rw-r--r--  2.0 unx     1110 b- defN 24-Apr-18 08:02 nucliadb/migrator/settings.py
--rw-r--r--  2.0 unx     2346 b- defN 24-Apr-18 08:02 nucliadb/migrator/utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-Apr-18 08:02 nucliadb/models/__init__.py
--rw-r--r--  2.0 unx     1599 b- defN 24-Apr-18 08:02 nucliadb/models/responses.py
--rw-r--r--  2.0 unx     6041 b- defN 24-Apr-18 08:02 nucliadb/purge/__init__.py
--rw-r--r--  2.0 unx     9364 b- defN 24-Apr-18 08:02 nucliadb/purge/orphan_shards.py
--rw-r--r--  2.0 unx     1328 b- defN 24-Apr-18 08:02 nucliadb/reader/__init__.py
--rw-r--r--  2.0 unx     3709 b- defN 24-Apr-18 08:02 nucliadb/reader/app.py
--rw-r--r--  2.0 unx     1366 b- defN 24-Apr-18 08:02 nucliadb/reader/lifecycle.py
--rw-r--r--  2.0 unx     1031 b- defN 24-Apr-18 08:02 nucliadb/reader/openapi.py
--rw-r--r--  2.0 unx     1447 b- defN 24-Apr-18 08:02 nucliadb/reader/run.py
--rw-r--r--  2.0 unx      872 b- defN 24-Apr-18 08:02 nucliadb/reader/api/__init__.py
--rw-r--r--  2.0 unx     2434 b- defN 24-Apr-18 08:02 nucliadb/reader/api/models.py
--rw-r--r--  2.0 unx     1110 b- defN 24-Apr-18 08:02 nucliadb/reader/api/v1/__init__.py
--rw-r--r--  2.0 unx    12368 b- defN 24-Apr-18 08:02 nucliadb/reader/api/v1/download.py
--rw-r--r--  2.0 unx     6450 b- defN 24-Apr-18 08:02 nucliadb/reader/api/v1/export_import.py
--rw-r--r--  2.0 unx     3632 b- defN 24-Apr-18 08:02 nucliadb/reader/api/v1/knowledgebox.py
--rw-r--r--  2.0 unx     2093 b- defN 24-Apr-18 08:02 nucliadb/reader/api/v1/learning_collector.py
--rw-r--r--  2.0 unx     4454 b- defN 24-Apr-18 08:02 nucliadb/reader/api/v1/learning_config.py
--rw-r--r--  2.0 unx    13928 b- defN 24-Apr-18 08:02 nucliadb/reader/api/v1/resource.py
--rw-r--r--  2.0 unx     1011 b- defN 24-Apr-18 08:02 nucliadb/reader/api/v1/router.py
--rw-r--r--  2.0 unx    13882 b- defN 24-Apr-18 08:02 nucliadb/reader/api/v1/services.py
--rw-r--r--  2.0 unx      835 b- defN 24-Apr-18 08:02 nucliadb/reader/reader/__init__.py
--rw-r--r--  2.0 unx     8155 b- defN 24-Apr-18 08:02 nucliadb/reader/reader/notifications.py
--rw-r--r--  2.0 unx      835 b- defN 24-Apr-18 08:02 nucliadb/reader/tests/__init__.py
--rw-r--r--  2.0 unx     1224 b- defN 24-Apr-18 08:02 nucliadb/reader/tests/conftest.py
--rw-r--r--  2.0 unx     4345 b- defN 24-Apr-18 08:02 nucliadb/reader/tests/fixtures.py
--rw-r--r--  2.0 unx     2748 b- defN 24-Apr-18 08:02 nucliadb/reader/tests/test_list_resources.py
--rw-r--r--  2.0 unx    10199 b- defN 24-Apr-18 08:02 nucliadb/reader/tests/test_reader_file_download.py
--rw-r--r--  2.0 unx    10586 b- defN 24-Apr-18 08:02 nucliadb/reader/tests/test_reader_resource.py
--rw-r--r--  2.0 unx     6535 b- defN 24-Apr-18 08:02 nucliadb/reader/tests/test_reader_resource_field.py
--rw-r--r--  2.0 unx     1535 b- defN 24-Apr-18 08:02 nucliadb/search/__init__.py
--rw-r--r--  2.0 unx     4905 b- defN 24-Apr-18 08:02 nucliadb/search/app.py
--rw-r--r--  2.0 unx     1956 b- defN 24-Apr-18 08:02 nucliadb/search/lifecycle.py
--rw-r--r--  2.0 unx     1016 b- defN 24-Apr-18 08:02 nucliadb/search/openapi.py
--rw-r--r--  2.0 unx    19798 b- defN 24-Apr-18 08:02 nucliadb/search/predict.py
--rw-r--r--  2.0 unx     1402 b- defN 24-Apr-18 08:02 nucliadb/search/run.py
--rw-r--r--  2.0 unx     1193 b- defN 24-Apr-18 08:02 nucliadb/search/settings.py
--rw-r--r--  2.0 unx     1037 b- defN 24-Apr-18 08:02 nucliadb/search/utilities.py
--rw-r--r--  2.0 unx      835 b- defN 24-Apr-18 08:02 nucliadb/search/api/__init__.py
--rw-r--r--  2.0 unx     1272 b- defN 24-Apr-18 08:02 nucliadb/search/api/v1/__init__.py
--rw-r--r--  2.0 unx     9913 b- defN 24-Apr-18 08:02 nucliadb/search/api/v1/chat.py
--rw-r--r--  2.0 unx     2665 b- defN 24-Apr-18 08:02 nucliadb/search/api/v1/feedback.py
--rw-r--r--  2.0 unx     8804 b- defN 24-Apr-18 08:02 nucliadb/search/api/v1/find.py
--rw-r--r--  2.0 unx     7026 b- defN 24-Apr-18 08:02 nucliadb/search/api/v1/knowledgebox.py
--rw-r--r--  2.0 unx     3041 b- defN 24-Apr-18 08:02 nucliadb/search/api/v1/predict_proxy.py
--rw-r--r--  2.0 unx      988 b- defN 24-Apr-18 08:02 nucliadb/search/api/v1/router.py
--rw-r--r--  2.0 unx    18359 b- defN 24-Apr-18 08:02 nucliadb/search/api/v1/search.py
--rw-r--r--  2.0 unx     5928 b- defN 24-Apr-18 08:02 nucliadb/search/api/v1/suggest.py
--rw-r--r--  2.0 unx     2536 b- defN 24-Apr-18 08:02 nucliadb/search/api/v1/summarize.py
--rw-r--r--  2.0 unx     1412 b- defN 24-Apr-18 08:02 nucliadb/search/api/v1/utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-Apr-18 08:02 nucliadb/search/api/v1/resource/__init__.py
--rw-r--r--  2.0 unx     6095 b- defN 24-Apr-18 08:02 nucliadb/search/api/v1/resource/ask.py
--rw-r--r--  2.0 unx     5887 b- defN 24-Apr-18 08:02 nucliadb/search/api/v1/resource/chat.py
--rw-r--r--  2.0 unx     5293 b- defN 24-Apr-18 08:02 nucliadb/search/api/v1/resource/search.py
--rw-r--r--  2.0 unx      833 b- defN 24-Apr-18 08:02 nucliadb/search/requesters/__init__.py
--rw-r--r--  2.0 unx     9070 b- defN 24-Apr-18 08:02 nucliadb/search/requesters/utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-Apr-18 08:02 nucliadb/search/search/__init__.py
--rw-r--r--  2.0 unx     2746 b- defN 24-Apr-18 08:02 nucliadb/search/search/cache.py
--rw-r--r--  2.0 unx     1154 b- defN 24-Apr-18 08:02 nucliadb/search/search/exceptions.py
--rw-r--r--  2.0 unx     5465 b- defN 24-Apr-18 08:02 nucliadb/search/search/fetch.py
--rw-r--r--  2.0 unx     6513 b- defN 24-Apr-18 08:02 nucliadb/search/search/filters.py
--rw-r--r--  2.0 unx     4646 b- defN 24-Apr-18 08:02 nucliadb/search/search/find.py
--rw-r--r--  2.0 unx    17152 b- defN 24-Apr-18 08:02 nucliadb/search/search/find_merge.py
--rw-r--r--  2.0 unx    21118 b- defN 24-Apr-18 08:02 nucliadb/search/search/merge.py
--rw-r--r--  2.0 unx     1130 b- defN 24-Apr-18 08:02 nucliadb/search/search/metrics.py
--rw-r--r--  2.0 unx     8698 b- defN 24-Apr-18 08:02 nucliadb/search/search/paragraphs.py
--rw-r--r--  2.0 unx     3026 b- defN 24-Apr-18 08:02 nucliadb/search/search/predict_proxy.py
--rw-r--r--  2.0 unx    32297 b- defN 24-Apr-18 08:02 nucliadb/search/search/query.py
--rw-r--r--  2.0 unx     3149 b- defN 24-Apr-18 08:02 nucliadb/search/search/shards.py
--rw-r--r--  2.0 unx     5101 b- defN 24-Apr-18 08:02 nucliadb/search/search/summarize.py
--rw-r--r--  2.0 unx     2438 b- defN 24-Apr-18 08:02 nucliadb/search/search/utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-Apr-18 08:02 nucliadb/search/search/chat/__init__.py
--rw-r--r--  2.0 unx     2058 b- defN 24-Apr-18 08:02 nucliadb/search/search/chat/images.py
--rw-r--r--  2.0 unx    20793 b- defN 24-Apr-18 08:02 nucliadb/search/search/chat/prompt.py
--rw-r--r--  2.0 unx    15347 b- defN 24-Apr-18 08:02 nucliadb/search/search/chat/query.py
--rw-r--r--  2.0 unx      835 b- defN 24-Apr-18 08:02 nucliadb/search/tests/__init__.py
--rw-r--r--  2.0 unx     1295 b- defN 24-Apr-18 08:02 nucliadb/search/tests/conftest.py
--rw-r--r--  2.0 unx     6578 b- defN 24-Apr-18 08:02 nucliadb/search/tests/fixtures.py
--rw-r--r--  2.0 unx    15529 b- defN 24-Apr-18 08:02 nucliadb/search/tests/node.py
--rw-r--r--  2.0 unx      833 b- defN 24-Apr-18 08:02 nucliadb/search/tests/unit/__init__.py
--rw-r--r--  2.0 unx     2649 b- defN 24-Apr-18 08:02 nucliadb/search/tests/unit/test_app.py
--rw-r--r--  2.0 unx     3374 b- defN 24-Apr-18 08:02 nucliadb/search/tests/unit/test_find_merge.py
--rw-r--r--  2.0 unx     1400 b- defN 24-Apr-18 08:02 nucliadb/search/tests/unit/test_merge.py
--rw-r--r--  2.0 unx    17080 b- defN 24-Apr-18 08:02 nucliadb/search/tests/unit/test_predict.py
--rw-r--r--  2.0 unx     1317 b- defN 24-Apr-18 08:02 nucliadb/search/tests/unit/test_run.py
--rw-r--r--  2.0 unx      835 b- defN 24-Apr-18 08:02 nucliadb/search/tests/unit/api/__init__.py
--rw-r--r--  2.0 unx      835 b- defN 24-Apr-18 08:02 nucliadb/search/tests/unit/api/v1/__init__.py
--rw-r--r--  2.0 unx     2966 b- defN 24-Apr-18 08:02 nucliadb/search/tests/unit/api/v1/test_chat.py
--rw-r--r--  2.0 unx     2865 b- defN 24-Apr-18 08:02 nucliadb/search/tests/unit/api/v1/test_predict_proxy.py
--rw-r--r--  2.0 unx     2901 b- defN 24-Apr-18 08:02 nucliadb/search/tests/unit/api/v1/test_summarize.py
--rw-r--r--  2.0 unx      835 b- defN 24-Apr-18 08:02 nucliadb/search/tests/unit/api/v1/resource/__init__.py
--rw-r--r--  2.0 unx     2411 b- defN 24-Apr-18 08:02 nucliadb/search/tests/unit/api/v1/resource/test_ask.py
--rw-r--r--  2.0 unx     3040 b- defN 24-Apr-18 08:02 nucliadb/search/tests/unit/api/v1/resource/test_chat.py
--rw-r--r--  2.0 unx      833 b- defN 24-Apr-18 08:02 nucliadb/search/tests/unit/search/__init__.py
--rw-r--r--  2.0 unx     8567 b- defN 24-Apr-18 08:02 nucliadb/search/tests/unit/search/test_chat_prompt.py
--rw-r--r--  2.0 unx     3736 b- defN 24-Apr-18 08:02 nucliadb/search/tests/unit/search/test_fetch.py
--rw-r--r--  2.0 unx     4306 b- defN 24-Apr-18 08:02 nucliadb/search/tests/unit/search/test_filters.py
--rw-r--r--  2.0 unx     4492 b- defN 24-Apr-18 08:02 nucliadb/search/tests/unit/search/test_paragraphs.py
--rw-r--r--  2.0 unx     3496 b- defN 24-Apr-18 08:02 nucliadb/search/tests/unit/search/test_predict_proxy.py
--rw-r--r--  2.0 unx     7001 b- defN 24-Apr-18 08:02 nucliadb/search/tests/unit/search/test_query.py
--rw-r--r--  2.0 unx      833 b- defN 24-Apr-18 08:02 nucliadb/search/tests/unit/search/requesters/__init__.py
--rw-r--r--  2.0 unx     6455 b- defN 24-Apr-18 08:02 nucliadb/search/tests/unit/search/requesters/test_utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-Apr-18 08:02 nucliadb/search/tests/unit/search/search/__init__.py
--rw-r--r--  2.0 unx     1759 b- defN 24-Apr-18 08:02 nucliadb/search/tests/unit/search/search/test_shards.py
--rw-r--r--  2.0 unx     2511 b- defN 24-Apr-18 08:02 nucliadb/search/tests/unit/search/search/test_utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-Apr-18 08:02 nucliadb/standalone/__init__.py
--rw-r--r--  2.0 unx     6746 b- defN 24-Apr-18 08:02 nucliadb/standalone/api_router.py
--rw-r--r--  2.0 unx     5763 b- defN 24-Apr-18 08:02 nucliadb/standalone/app.py
--rw-r--r--  2.0 unx     7800 b- defN 24-Apr-18 08:02 nucliadb/standalone/auth.py
--rw-r--r--  2.0 unx     5309 b- defN 24-Apr-18 08:02 nucliadb/standalone/config.py
--rw-r--r--  2.0 unx     6930 b- defN 24-Apr-18 08:02 nucliadb/standalone/introspect.py
--rw-r--r--  2.0 unx     2488 b- defN 24-Apr-18 08:02 nucliadb/standalone/lifecycle.py
--rw-r--r--  2.0 unx     1317 b- defN 24-Apr-18 08:02 nucliadb/standalone/purge.py
--rw-r--r--  2.0 unx     5336 b- defN 24-Apr-18 08:02 nucliadb/standalone/run.py
--rw-r--r--  2.0 unx     5781 b- defN 24-Apr-18 08:02 nucliadb/standalone/settings.py
--rw-r--r--  2.0 unx     3132 b- defN 24-Apr-18 08:02 nucliadb/standalone/versions.py
--rw-r--r--  2.0 unx     2285 b- defN 24-Apr-18 08:02 nucliadb/standalone/static/favicon.ico
--rw-r--r--  2.0 unx     3833 b- defN 24-Apr-18 08:02 nucliadb/standalone/static/index.html
--rw-r--r--  2.0 unx     2639 b- defN 24-Apr-18 08:02 nucliadb/standalone/static/logo.svg
--rw-r--r--  2.0 unx      835 b- defN 24-Apr-18 08:02 nucliadb/standalone/tests/__init__.py
--rw-r--r--  2.0 unx     1294 b- defN 24-Apr-18 08:02 nucliadb/standalone/tests/conftest.py
--rw-r--r--  2.0 unx     1319 b- defN 24-Apr-18 08:02 nucliadb/standalone/tests/fixtures.py
--rw-r--r--  2.0 unx      833 b- defN 24-Apr-18 08:02 nucliadb/standalone/tests/unit/__init__.py
--rw-r--r--  2.0 unx     1722 b- defN 24-Apr-18 08:02 nucliadb/standalone/tests/unit/test_api_router.py
--rw-r--r--  2.0 unx     5509 b- defN 24-Apr-18 08:02 nucliadb/standalone/tests/unit/test_auth.py
--rw-r--r--  2.0 unx     1334 b- defN 24-Apr-18 08:02 nucliadb/standalone/tests/unit/test_introspect.py
--rw-r--r--  2.0 unx     1472 b- defN 24-Apr-18 08:02 nucliadb/standalone/tests/unit/test_run.py
--rw-r--r--  2.0 unx     1972 b- defN 24-Apr-18 08:02 nucliadb/standalone/tests/unit/test_versions.py
--rw-r--r--  2.0 unx     1037 b- defN 24-Apr-18 08:02 nucliadb/tasks/__init__.py
--rw-r--r--  2.0 unx     7655 b- defN 24-Apr-18 08:02 nucliadb/tasks/consumer.py
--rw-r--r--  2.0 unx      924 b- defN 24-Apr-18 08:02 nucliadb/tasks/logger.py
--rw-r--r--  2.0 unx     1378 b- defN 24-Apr-18 08:02 nucliadb/tasks/models.py
--rw-r--r--  2.0 unx     3457 b- defN 24-Apr-18 08:02 nucliadb/tasks/producer.py
--rw-r--r--  2.0 unx     1753 b- defN 24-Apr-18 08:02 nucliadb/tasks/registry.py
--rw-r--r--  2.0 unx     1360 b- defN 24-Apr-18 08:02 nucliadb/tasks/utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-Apr-18 08:02 nucliadb/tests/__init__.py
--rw-r--r--  2.0 unx     1229 b- defN 24-Apr-18 08:02 nucliadb/tests/conftest.py
--rw-r--r--  2.0 unx    22365 b- defN 24-Apr-18 08:02 nucliadb/tests/fixtures.py
--rw-r--r--  2.0 unx     7549 b- defN 24-Apr-18 08:02 nucliadb/tests/tikv.py
--rw-r--r--  2.0 unx      835 b- defN 24-Apr-18 08:02 nucliadb/tests/benchmarks/__init__.py
--rw-r--r--  2.0 unx     3032 b- defN 24-Apr-18 08:02 nucliadb/tests/benchmarks/test_search.py
--rw-r--r--  2.0 unx      919 b- defN 24-Apr-18 08:02 nucliadb/tests/knowledgeboxes/__init__.py
--rw-r--r--  2.0 unx     7002 b- defN 24-Apr-18 08:02 nucliadb/tests/knowledgeboxes/philosophy_books.py
--rw-r--r--  2.0 unx     3037 b- defN 24-Apr-18 08:02 nucliadb/tests/knowledgeboxes/ten_dummy_resources.py
--rw-r--r--  2.0 unx     1148 b- defN 24-Apr-18 08:02 nucliadb/tests/migrations/__init__.py
--rw-r--r--  2.0 unx     2726 b- defN 24-Apr-18 08:02 nucliadb/tests/migrations/test_migration_0017.py
--rw-r--r--  2.0 unx     3625 b- defN 24-Apr-18 08:02 nucliadb/tests/migrations/test_migration_0018.py
--rw-r--r--  2.0 unx      835 b- defN 24-Apr-18 08:02 nucliadb/tests/unit/__init__.py
--rw-r--r--  2.0 unx     1487 b- defN 24-Apr-18 08:02 nucliadb/tests/unit/test_field_ids.py
--rw-r--r--  2.0 unx     2758 b- defN 24-Apr-18 08:02 nucliadb/tests/unit/test_health.py
--rw-r--r--  2.0 unx     1543 b- defN 24-Apr-18 08:02 nucliadb/tests/unit/test_kb_slugs.py
--rw-r--r--  2.0 unx     7892 b- defN 24-Apr-18 08:02 nucliadb/tests/unit/test_learning_proxy.py
--rw-r--r--  2.0 unx     2642 b- defN 24-Apr-18 08:02 nucliadb/tests/unit/test_metrics_exporter.py
--rw-r--r--  2.0 unx     1341 b- defN 24-Apr-18 08:02 nucliadb/tests/unit/test_openapi.py
--rw-r--r--  2.0 unx     3656 b- defN 24-Apr-18 08:02 nucliadb/tests/unit/test_purge.py
--rw-r--r--  2.0 unx      835 b- defN 24-Apr-18 08:02 nucliadb/tests/unit/common/__init__.py
--rw-r--r--  2.0 unx     1268 b- defN 24-Apr-18 08:02 nucliadb/tests/unit/common/test_context.py
--rw-r--r--  2.0 unx      835 b- defN 24-Apr-18 08:02 nucliadb/tests/unit/common/cluster/__init__.py
--rw-r--r--  2.0 unx    11955 b- defN 24-Apr-18 08:02 nucliadb/tests/unit/common/cluster/test_cluster.py
--rw-r--r--  2.0 unx     5387 b- defN 24-Apr-18 08:02 nucliadb/tests/unit/common/cluster/test_kb_shard_manager.py
--rw-r--r--  2.0 unx     9470 b- defN 24-Apr-18 08:02 nucliadb/tests/unit/common/cluster/test_rollover.py
--rw-r--r--  2.0 unx      835 b- defN 24-Apr-18 08:02 nucliadb/tests/unit/common/cluster/discovery/__init__.py
--rw-r--r--  2.0 unx     5584 b- defN 24-Apr-18 08:02 nucliadb/tests/unit/common/cluster/discovery/test_k8s.py
--rw-r--r--  2.0 unx      833 b- defN 24-Apr-18 08:02 nucliadb/tests/unit/common/cluster/standalone/__init__.py
--rw-r--r--  2.0 unx     3750 b- defN 24-Apr-18 08:02 nucliadb/tests/unit/common/cluster/standalone/test_service.py
--rw-r--r--  2.0 unx     2114 b- defN 24-Apr-18 08:02 nucliadb/tests/unit/common/cluster/standalone/test_utils.py
--rw-r--r--  2.0 unx      833 b- defN 24-Apr-18 08:02 nucliadb/tests/unit/common/maindb/__init__.py
--rw-r--r--  2.0 unx     3579 b- defN 24-Apr-18 08:02 nucliadb/tests/unit/common/maindb/test_driver.py
--rw-r--r--  2.0 unx     1869 b- defN 24-Apr-18 08:02 nucliadb/tests/unit/common/maindb/test_tikv.py
--rw-r--r--  2.0 unx     2998 b- defN 24-Apr-18 08:02 nucliadb/tests/unit/common/maindb/test_utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-Apr-18 08:02 nucliadb/tests/unit/export_import/__init__.py
--rw-r--r--  2.0 unx     1435 b- defN 24-Apr-18 08:02 nucliadb/tests/unit/export_import/test_datamanager.py
--rw-r--r--  2.0 unx     9706 b- defN 24-Apr-18 08:02 nucliadb/tests/unit/export_import/test_utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-Apr-18 08:02 nucliadb/tests/unit/migrator/__init__.py
--rw-r--r--  2.0 unx     3233 b- defN 24-Apr-18 08:02 nucliadb/tests/unit/migrator/test_migrator.py
--rw-r--r--  2.0 unx      835 b- defN 24-Apr-18 08:02 nucliadb/tests/unit/tasks/__init__.py
--rw-r--r--  2.0 unx     1375 b- defN 24-Apr-18 08:02 nucliadb/tests/unit/tasks/conftest.py
--rw-r--r--  2.0 unx     2714 b- defN 24-Apr-18 08:02 nucliadb/tests/unit/tasks/test_consumer.py
--rw-r--r--  2.0 unx     3189 b- defN 24-Apr-18 08:02 nucliadb/tests/unit/tasks/test_producer.py
--rw-r--r--  2.0 unx     1827 b- defN 24-Apr-18 08:02 nucliadb/tests/unit/tasks/test_tasks.py
--rw-r--r--  2.0 unx     2507 b- defN 24-Apr-18 08:02 nucliadb/tests/utils/__init__.py
--rw-r--r--  2.0 unx     1797 b- defN 24-Apr-18 08:02 nucliadb/tests/utils/aiohttp_session.py
--rw-r--r--  2.0 unx     2533 b- defN 24-Apr-18 08:02 nucliadb/tests/utils/entities.py
--rw-r--r--  2.0 unx     6145 b- defN 24-Apr-18 08:02 nucliadb/tests/utils/broker_messages/__init__.py
--rw-r--r--  2.0 unx     6795 b- defN 24-Apr-18 08:02 nucliadb/tests/utils/broker_messages/fields.py
--rw-r--r--  2.0 unx     1196 b- defN 24-Apr-18 08:02 nucliadb/tests/utils/broker_messages/helpers.py
--rw-r--r--  2.0 unx     1325 b- defN 24-Apr-18 08:02 nucliadb/train/__init__.py
--rw-r--r--  2.0 unx     3530 b- defN 24-Apr-18 08:02 nucliadb/train/app.py
--rw-r--r--  2.0 unx     3800 b- defN 24-Apr-18 08:02 nucliadb/train/generator.py
--rw-r--r--  2.0 unx     1698 b- defN 24-Apr-18 08:02 nucliadb/train/lifecycle.py
--rw-r--r--  2.0 unx     1198 b- defN 24-Apr-18 08:02 nucliadb/train/models.py
--rw-r--r--  2.0 unx     5706 b- defN 24-Apr-18 08:02 nucliadb/train/nodes.py
--rw-r--r--  2.0 unx     1400 b- defN 24-Apr-18 08:02 nucliadb/train/run.py
--rw-r--r--  2.0 unx     5926 b- defN 24-Apr-18 08:02 nucliadb/train/servicer.py
--rw-r--r--  2.0 unx     1415 b- defN 24-Apr-18 08:02 nucliadb/train/settings.py
--rw-r--r--  2.0 unx     1496 b- defN 24-Apr-18 08:02 nucliadb/train/types.py
--rw-r--r--  2.0 unx     3265 b- defN 24-Apr-18 08:02 nucliadb/train/upload.py
--rw-r--r--  2.0 unx     6420 b- defN 24-Apr-18 08:02 nucliadb/train/uploader.py
--rw-r--r--  2.0 unx     3179 b- defN 24-Apr-18 08:02 nucliadb/train/utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-Apr-18 08:02 nucliadb/train/api/__init__.py
--rw-r--r--  2.0 unx     1479 b- defN 24-Apr-18 08:02 nucliadb/train/api/utils.py
--rw-r--r--  2.0 unx      928 b- defN 24-Apr-18 08:02 nucliadb/train/api/v1/__init__.py
--rw-r--r--  2.0 unx     2065 b- defN 24-Apr-18 08:02 nucliadb/train/api/v1/check.py
--rw-r--r--  2.0 unx      910 b- defN 24-Apr-18 08:02 nucliadb/train/api/v1/router.py
--rw-r--r--  2.0 unx     1905 b- defN 24-Apr-18 08:02 nucliadb/train/api/v1/shards.py
--rw-r--r--  2.0 unx     2129 b- defN 24-Apr-18 08:02 nucliadb/train/api/v1/trainset.py
--rw-r--r--  2.0 unx      835 b- defN 24-Apr-18 08:02 nucliadb/train/generators/__init__.py
--rw-r--r--  2.0 unx     3723 b- defN 24-Apr-18 08:02 nucliadb/train/generators/field_classifier.py
--rw-r--r--  2.0 unx     6712 b- defN 24-Apr-18 08:02 nucliadb/train/generators/image_classifier.py
--rw-r--r--  2.0 unx     2789 b- defN 24-Apr-18 08:02 nucliadb/train/generators/paragraph_classifier.py
--rw-r--r--  2.0 unx     3590 b- defN 24-Apr-18 08:02 nucliadb/train/generators/paragraph_streaming.py
--rw-r--r--  2.0 unx     5372 b- defN 24-Apr-18 08:02 nucliadb/train/generators/question_answer_streaming.py
--rw-r--r--  2.0 unx     5160 b- defN 24-Apr-18 08:02 nucliadb/train/generators/sentence_classifier.py
--rw-r--r--  2.0 unx    10446 b- defN 24-Apr-18 08:02 nucliadb/train/generators/token_classifier.py
--rw-r--r--  2.0 unx     3877 b- defN 24-Apr-18 08:02 nucliadb/train/generators/utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-Apr-18 08:02 nucliadb/train/tests/__init__.py
--rw-r--r--  2.0 unx     1125 b- defN 24-Apr-18 08:02 nucliadb/train/tests/conftest.py
--rw-r--r--  2.0 unx    11053 b- defN 24-Apr-18 08:02 nucliadb/train/tests/fixtures.py
--rw-r--r--  2.0 unx     4598 b- defN 24-Apr-18 08:02 nucliadb/train/tests/test_field_classification.py
--rw-r--r--  2.0 unx     2729 b- defN 24-Apr-18 08:02 nucliadb/train/tests/test_get_entities.py
--rw-r--r--  2.0 unx     1876 b- defN 24-Apr-18 08:02 nucliadb/train/tests/test_get_info.py
--rw-r--r--  2.0 unx     1382 b- defN 24-Apr-18 08:02 nucliadb/train/tests/test_get_ontology.py
--rw-r--r--  2.0 unx     2417 b- defN 24-Apr-18 08:02 nucliadb/train/tests/test_get_ontology_count.py
--rw-r--r--  2.0 unx     7669 b- defN 24-Apr-18 08:02 nucliadb/train/tests/test_image_classification.py
--rw-r--r--  2.0 unx     1416 b- defN 24-Apr-18 08:02 nucliadb/train/tests/test_list_fields.py
--rw-r--r--  2.0 unx     2944 b- defN 24-Apr-18 08:02 nucliadb/train/tests/test_list_paragraphs.py
--rw-r--r--  2.0 unx     1423 b- defN 24-Apr-18 08:02 nucliadb/train/tests/test_list_resources.py
--rw-r--r--  2.0 unx     2947 b- defN 24-Apr-18 08:02 nucliadb/train/tests/test_list_sentences.py
--rw-r--r--  2.0 unx     4645 b- defN 24-Apr-18 08:02 nucliadb/train/tests/test_paragraph_classification.py
--rw-r--r--  2.0 unx     4320 b- defN 24-Apr-18 08:02 nucliadb/train/tests/test_paragraph_streaming.py
--rw-r--r--  2.0 unx     8751 b- defN 24-Apr-18 08:02 nucliadb/train/tests/test_question_answer_streaming.py
--rw-r--r--  2.0 unx     5051 b- defN 24-Apr-18 08:02 nucliadb/train/tests/test_sentence_classification.py
--rw-r--r--  2.0 unx     5583 b- defN 24-Apr-18 08:02 nucliadb/train/tests/test_token_classification.py
--rw-r--r--  2.0 unx     3324 b- defN 24-Apr-18 08:02 nucliadb/train/tests/utils.py
--rw-r--r--  2.0 unx     1328 b- defN 24-Apr-18 08:02 nucliadb/writer/__init__.py
--rw-r--r--  2.0 unx     4268 b- defN 24-Apr-18 08:02 nucliadb/writer/app.py
--rw-r--r--  2.0 unx    19435 b- defN 24-Apr-18 08:02 nucliadb/writer/back_pressure.py
--rw-r--r--  2.0 unx      972 b- defN 24-Apr-18 08:02 nucliadb/writer/exceptions.py
--rw-r--r--  2.0 unx     1953 b- defN 24-Apr-18 08:02 nucliadb/writer/lifecycle.py
--rw-r--r--  2.0 unx     1032 b- defN 24-Apr-18 08:02 nucliadb/writer/openapi.py
--rw-r--r--  2.0 unx     1448 b- defN 24-Apr-18 08:02 nucliadb/writer/run.py
--rw-r--r--  2.0 unx     3074 b- defN 24-Apr-18 08:02 nucliadb/writer/settings.py
--rw-r--r--  2.0 unx     1036 b- defN 24-Apr-18 08:02 nucliadb/writer/utilities.py
--rw-r--r--  2.0 unx     1948 b- defN 24-Apr-18 08:02 nucliadb/writer/vectors.py
--rw-r--r--  2.0 unx      835 b- defN 24-Apr-18 08:02 nucliadb/writer/api/__init__.py
--rw-r--r--  2.0 unx     1429 b- defN 24-Apr-18 08:02 nucliadb/writer/api/constants.py
--rw-r--r--  2.0 unx     1095 b- defN 24-Apr-18 08:02 nucliadb/writer/api/v1/__init__.py
--rw-r--r--  2.0 unx     6565 b- defN 24-Apr-18 08:02 nucliadb/writer/api/v1/export_import.py
--rw-r--r--  2.0 unx    28320 b- defN 24-Apr-18 08:02 nucliadb/writer/api/v1/field.py
--rw-r--r--  2.0 unx     5239 b- defN 24-Apr-18 08:02 nucliadb/writer/api/v1/knowledgebox.py
--rw-r--r--  2.0 unx     2052 b- defN 24-Apr-18 08:02 nucliadb/writer/api/v1/learning_config.py
--rw-r--r--  2.0 unx    19940 b- defN 24-Apr-18 08:02 nucliadb/writer/api/v1/resource.py
--rw-r--r--  2.0 unx     1034 b- defN 24-Apr-18 08:02 nucliadb/writer/api/v1/router.py
--rw-r--r--  2.0 unx    12733 b- defN 24-Apr-18 08:02 nucliadb/writer/api/v1/services.py
--rw-r--r--  2.0 unx    31464 b- defN 24-Apr-18 08:02 nucliadb/writer/api/v1/upload.py
--rw-r--r--  2.0 unx     1612 b- defN 24-Apr-18 08:02 nucliadb/writer/layouts/__init__.py
--rw-r--r--  2.0 unx     2115 b- defN 24-Apr-18 08:02 nucliadb/writer/layouts/v1.py
--rw-r--r--  2.0 unx      835 b- defN 24-Apr-18 08:02 nucliadb/writer/resource/__init__.py
--rw-r--r--  2.0 unx     1425 b- defN 24-Apr-18 08:02 nucliadb/writer/resource/audit.py
--rw-r--r--  2.0 unx    10968 b- defN 24-Apr-18 08:02 nucliadb/writer/resource/basic.py
--rw-r--r--  2.0 unx    16319 b- defN 24-Apr-18 08:02 nucliadb/writer/resource/field.py
--rw-r--r--  2.0 unx     2022 b- defN 24-Apr-18 08:02 nucliadb/writer/resource/origin.py
--rw-r--r--  2.0 unx     1152 b- defN 24-Apr-18 08:02 nucliadb/writer/resource/slug.py
--rw-r--r--  2.0 unx      835 b- defN 24-Apr-18 08:02 nucliadb/writer/tests/__init__.py
--rw-r--r--  2.0 unx     1200 b- defN 24-Apr-18 08:02 nucliadb/writer/tests/conftest.py
--rw-r--r--  2.0 unx     5971 b- defN 24-Apr-18 08:02 nucliadb/writer/tests/fixtures.py
--rw-r--r--  2.0 unx    15472 b- defN 24-Apr-18 08:02 nucliadb/writer/tests/test_fields.py
--rw-r--r--  2.0 unx    25913 b- defN 24-Apr-18 08:02 nucliadb/writer/tests/test_files.py
--rw-r--r--  2.0 unx     1729 b- defN 24-Apr-18 08:02 nucliadb/writer/tests/test_knowledgebox.py
--rw-r--r--  2.0 unx     4569 b- defN 24-Apr-18 08:02 nucliadb/writer/tests/test_reprocess_file_field.py
--rw-r--r--  2.0 unx    17449 b- defN 24-Apr-18 08:02 nucliadb/writer/tests/test_resources.py
--rw-r--r--  2.0 unx     5120 b- defN 24-Apr-18 08:02 nucliadb/writer/tests/test_service.py
--rw-r--r--  2.0 unx     6054 b- defN 24-Apr-18 08:02 nucliadb/writer/tests/test_tus.py
--rw-r--r--  2.0 unx     1287 b- defN 24-Apr-18 08:02 nucliadb/writer/tests/utils.py
--rw-r--r--  2.0 unx     5226 b- defN 24-Apr-18 08:02 nucliadb/writer/tus/__init__.py
--rw-r--r--  2.0 unx     5082 b- defN 24-Apr-18 08:02 nucliadb/writer/tus/dm.py
--rw-r--r--  2.0 unx     2186 b- defN 24-Apr-18 08:02 nucliadb/writer/tus/exceptions.py
--rw-r--r--  2.0 unx    14527 b- defN 24-Apr-18 08:02 nucliadb/writer/tus/gcs.py
--rw-r--r--  2.0 unx     5849 b- defN 24-Apr-18 08:02 nucliadb/writer/tus/local.py
--rw-r--r--  2.0 unx     4367 b- defN 24-Apr-18 08:02 nucliadb/writer/tus/pg.py
--rw-r--r--  2.0 unx     9069 b- defN 24-Apr-18 08:02 nucliadb/writer/tus/s3.py
--rw-r--r--  2.0 unx     4734 b- defN 24-Apr-18 08:02 nucliadb/writer/tus/storage.py
--rw-r--r--  2.0 unx     2556 b- defN 24-Apr-18 08:02 nucliadb/writer/tus/utils.py
--rw-r--r--  2.0 unx     4348 b- defN 24-Apr-18 08:03 nucliadb-3.0.3.post437.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-18 08:03 nucliadb-3.0.3.post437.dist-info/WHEEL
--rw-r--r--  2.0 unx     1268 b- defN 24-Apr-18 08:03 nucliadb-3.0.3.post437.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       20 b- defN 24-Apr-18 08:03 nucliadb-3.0.3.post437.dist-info/top_level.txt
--rw-r--r--  2.0 unx        1 b- defN 24-Apr-18 08:03 nucliadb-3.0.3.post437.dist-info/zip-safe
--rw-rw-r--  2.0 unx    42447 b- defN 24-Apr-18 08:03 nucliadb-3.0.3.post437.dist-info/RECORD
-453 files, 2232244 bytes uncompressed, 681793 bytes compressed:  69.5%
+Zip file size: 754961 bytes, number of entries: 456
+-rw-r--r--  2.0 unx     1135 b- defN 24-Apr-18 09:18 migrations/0001_bootstrap.py
+-rw-r--r--  2.0 unx     1177 b- defN 24-Apr-18 09:18 migrations/0002_rollover_shards.py
+-rw-r--r--  2.0 unx     2436 b- defN 24-Apr-18 09:18 migrations/0003_allfields_key.py
+-rw-r--r--  2.0 unx     1177 b- defN 24-Apr-18 09:18 migrations/0004_rollover_shards.py
+-rw-r--r--  2.0 unx     1177 b- defN 24-Apr-18 09:18 migrations/0005_rollover_shards.py
+-rw-r--r--  2.0 unx     1024 b- defN 24-Apr-18 09:18 migrations/0006_rollover_shards.py
+-rw-r--r--  2.0 unx     1301 b- defN 24-Apr-18 09:18 migrations/0008_cleanup_leftover_rollover_metadata.py
+-rw-r--r--  2.0 unx     1378 b- defN 24-Apr-18 09:18 migrations/0009_upgrade_relations_and_texts_to_v2.py
+-rw-r--r--  2.0 unx     1610 b- defN 24-Apr-18 09:18 migrations/0010_fix_corrupt_indexes.py
+-rw-r--r--  2.0 unx     1843 b- defN 24-Apr-18 09:18 migrations/0011_materialize_labelset_ids.py
+-rw-r--r--  2.0 unx     1443 b- defN 24-Apr-18 09:18 migrations/0012_rollover_shards.py
+-rw-r--r--  2.0 unx     1024 b- defN 24-Apr-18 09:18 migrations/0013_rollover_shards.py
+-rw-r--r--  2.0 unx     1382 b- defN 24-Apr-18 09:18 migrations/0014_rollover_shards.py
+-rw-r--r--  2.0 unx     1462 b- defN 24-Apr-18 09:18 migrations/0015_targeted_rollover.py
+-rw-r--r--  2.0 unx     2506 b- defN 24-Apr-18 09:18 migrations/0016_upgrade_to_paragraphs_v2.py
+-rw-r--r--  2.0 unx     2100 b- defN 24-Apr-18 09:18 migrations/0017_multiple_writable_shards.py
+-rw-r--r--  2.0 unx     2264 b- defN 24-Apr-18 09:18 migrations/0018_purge_orphan_kbslugs.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Apr-18 09:18 migrations/__init__.py
+-rw-r--r--  2.0 unx      891 b- defN 24-Apr-18 09:18 nucliadb/__init__.py
+-rw-r--r--  2.0 unx     3733 b- defN 24-Apr-18 09:18 nucliadb/health.py
+-rw-r--r--  2.0 unx    11626 b- defN 24-Apr-18 09:18 nucliadb/learning_proxy.py
+-rw-r--r--  2.0 unx     4806 b- defN 24-Apr-18 09:18 nucliadb/metrics_exporter.py
+-rw-r--r--  2.0 unx     2272 b- defN 24-Apr-18 09:18 nucliadb/openapi.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-18 09:18 nucliadb/py.typed
+-rw-r--r--  2.0 unx      835 b- defN 24-Apr-18 09:18 nucliadb/common/__init__.py
+-rw-r--r--  2.0 unx     4905 b- defN 24-Apr-18 09:18 nucliadb/common/locking.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Apr-18 09:18 nucliadb/common/cluster/__init__.py
+-rw-r--r--  2.0 unx     5090 b- defN 24-Apr-18 09:18 nucliadb/common/cluster/base.py
+-rw-r--r--  2.0 unx     1495 b- defN 24-Apr-18 09:18 nucliadb/common/cluster/exceptions.py
+-rw-r--r--  2.0 unx     3658 b- defN 24-Apr-18 09:18 nucliadb/common/cluster/grpc_node_dummy.py
+-rw-r--r--  2.0 unx     3429 b- defN 24-Apr-18 09:18 nucliadb/common/cluster/index_node.py
+-rw-r--r--  2.0 unx    21231 b- defN 24-Apr-18 09:18 nucliadb/common/cluster/manager.py
+-rw-r--r--  2.0 unx     8490 b- defN 24-Apr-18 09:18 nucliadb/common/cluster/rebalance.py
+-rw-r--r--  2.0 unx    19593 b- defN 24-Apr-18 09:18 nucliadb/common/cluster/rollover.py
+-rw-r--r--  2.0 unx     2713 b- defN 24-Apr-18 09:18 nucliadb/common/cluster/settings.py
+-rw-r--r--  2.0 unx     5494 b- defN 24-Apr-18 09:18 nucliadb/common/cluster/utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Apr-18 09:18 nucliadb/common/cluster/discovery/__init__.py
+-rw-r--r--  2.0 unx     6553 b- defN 24-Apr-18 09:18 nucliadb/common/cluster/discovery/base.py
+-rw-r--r--  2.0 unx    12518 b- defN 24-Apr-18 09:18 nucliadb/common/cluster/discovery/k8s.py
+-rw-r--r--  2.0 unx     1957 b- defN 24-Apr-18 09:18 nucliadb/common/cluster/discovery/manual.py
+-rw-r--r--  2.0 unx     1737 b- defN 24-Apr-18 09:18 nucliadb/common/cluster/discovery/single.py
+-rw-r--r--  2.0 unx     1139 b- defN 24-Apr-18 09:18 nucliadb/common/cluster/discovery/types.py
+-rw-r--r--  2.0 unx     2548 b- defN 24-Apr-18 09:18 nucliadb/common/cluster/discovery/utils.py
+-rw-r--r--  2.0 unx      833 b- defN 24-Apr-18 09:18 nucliadb/common/cluster/standalone/__init__.py
+-rw-r--r--  2.0 unx    13707 b- defN 24-Apr-18 09:18 nucliadb/common/cluster/standalone/grpc_node_binding.py
+-rw-r--r--  2.0 unx     4683 b- defN 24-Apr-18 09:18 nucliadb/common/cluster/standalone/index_node.py
+-rw-r--r--  2.0 unx     3444 b- defN 24-Apr-18 09:18 nucliadb/common/cluster/standalone/service.py
+-rw-r--r--  2.0 unx     3386 b- defN 24-Apr-18 09:18 nucliadb/common/cluster/standalone/utils.py
+-rw-r--r--  2.0 unx     3498 b- defN 24-Apr-18 09:18 nucliadb/common/context/__init__.py
+-rw-r--r--  2.0 unx     1628 b- defN 24-Apr-18 09:18 nucliadb/common/context/fastapi.py
+-rw-r--r--  2.0 unx     1813 b- defN 24-Apr-18 09:18 nucliadb/common/datamanagers/__init__.py
+-rw-r--r--  2.0 unx     1451 b- defN 24-Apr-18 09:18 nucliadb/common/datamanagers/cluster.py
+-rw-r--r--  2.0 unx     5383 b- defN 24-Apr-18 09:18 nucliadb/common/datamanagers/entities.py
+-rw-r--r--  2.0 unx      883 b- defN 24-Apr-18 09:18 nucliadb/common/datamanagers/exceptions.py
+-rw-r--r--  2.0 unx     3994 b- defN 24-Apr-18 09:18 nucliadb/common/datamanagers/kb.py
+-rw-r--r--  2.0 unx     5389 b- defN 24-Apr-18 09:18 nucliadb/common/datamanagers/labels.py
+-rw-r--r--  2.0 unx     1599 b- defN 24-Apr-18 09:18 nucliadb/common/datamanagers/processing.py
+-rw-r--r--  2.0 unx     7637 b- defN 24-Apr-18 09:18 nucliadb/common/datamanagers/resources.py
+-rw-r--r--  2.0 unx     5633 b- defN 24-Apr-18 09:18 nucliadb/common/datamanagers/rollover.py
+-rw-r--r--  2.0 unx     1681 b- defN 24-Apr-18 09:18 nucliadb/common/datamanagers/utils.py
+-rw-r--r--  2.0 unx     2055 b- defN 24-Apr-18 09:18 nucliadb/common/datamanagers/vectorsets.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Apr-18 09:18 nucliadb/common/http_clients/__init__.py
+-rw-r--r--  2.0 unx     2146 b- defN 24-Apr-18 09:18 nucliadb/common/http_clients/auth.py
+-rw-r--r--  2.0 unx     1100 b- defN 24-Apr-18 09:18 nucliadb/common/http_clients/exceptions.py
+-rw-r--r--  2.0 unx     7155 b- defN 24-Apr-18 09:18 nucliadb/common/http_clients/processing.py
+-rw-r--r--  2.0 unx     1540 b- defN 24-Apr-18 09:18 nucliadb/common/http_clients/pypi.py
+-rw-r--r--  2.0 unx     1551 b- defN 24-Apr-18 09:18 nucliadb/common/http_clients/utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Apr-18 09:18 nucliadb/common/maindb/__init__.py
+-rw-r--r--  2.0 unx     3449 b- defN 24-Apr-18 09:18 nucliadb/common/maindb/driver.py
+-rw-r--r--  2.0 unx      946 b- defN 24-Apr-18 09:18 nucliadb/common/maindb/exceptions.py
+-rw-r--r--  2.0 unx     6769 b- defN 24-Apr-18 09:18 nucliadb/common/maindb/local.py
+-rw-r--r--  2.0 unx     8391 b- defN 24-Apr-18 09:18 nucliadb/common/maindb/pg.py
+-rw-r--r--  2.0 unx     6053 b- defN 24-Apr-18 09:18 nucliadb/common/maindb/redis.py
+-rw-r--r--  2.0 unx    14502 b- defN 24-Apr-18 09:18 nucliadb/common/maindb/tikv.py
+-rw-r--r--  2.0 unx     4109 b- defN 24-Apr-18 09:18 nucliadb/common/maindb/utils.py
+-rw-r--r--  2.0 unx      932 b- defN 24-Apr-18 09:18 nucliadb/export_import/__init__.py
+-rw-r--r--  2.0 unx     6171 b- defN 24-Apr-18 09:18 nucliadb/export_import/datamanager.py
+-rw-r--r--  2.0 unx     1949 b- defN 24-Apr-18 09:18 nucliadb/export_import/exceptions.py
+-rw-r--r--  2.0 unx     7116 b- defN 24-Apr-18 09:18 nucliadb/export_import/exporter.py
+-rw-r--r--  2.0 unx     4258 b- defN 24-Apr-18 09:18 nucliadb/export_import/importer.py
+-rw-r--r--  2.0 unx     2063 b- defN 24-Apr-18 09:18 nucliadb/export_import/models.py
+-rw-r--r--  2.0 unx     2571 b- defN 24-Apr-18 09:18 nucliadb/export_import/tasks.py
+-rw-r--r--  2.0 unx    19270 b- defN 24-Apr-18 09:18 nucliadb/export_import/utils.py
+-rw-r--r--  2.0 unx     1011 b- defN 24-Apr-18 09:18 nucliadb/ingest/__init__.py
+-rw-r--r--  2.0 unx     7277 b- defN 24-Apr-18 09:18 nucliadb/ingest/app.py
+-rw-r--r--  2.0 unx     1005 b- defN 24-Apr-18 09:18 nucliadb/ingest/cache.py
+-rw-r--r--  2.0 unx     2484 b- defN 24-Apr-18 09:18 nucliadb/ingest/partitions.py
+-rw-r--r--  2.0 unx    19541 b- defN 24-Apr-18 09:18 nucliadb/ingest/processing.py
+-rw-r--r--  2.0 unx    20277 b- defN 24-Apr-18 09:18 nucliadb/ingest/serialize.py
+-rw-r--r--  2.0 unx     3183 b- defN 24-Apr-18 09:18 nucliadb/ingest/settings.py
+-rw-r--r--  2.0 unx     2314 b- defN 24-Apr-18 09:18 nucliadb/ingest/utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Apr-18 09:18 nucliadb/ingest/consumer/__init__.py
+-rw-r--r--  2.0 unx    11563 b- defN 24-Apr-18 09:18 nucliadb/ingest/consumer/auditing.py
+-rw-r--r--  2.0 unx    12159 b- defN 24-Apr-18 09:18 nucliadb/ingest/consumer/consumer.py
+-rw-r--r--  2.0 unx     3788 b- defN 24-Apr-18 09:18 nucliadb/ingest/consumer/materializer.py
+-rw-r--r--  2.0 unx     1075 b- defN 24-Apr-18 09:18 nucliadb/ingest/consumer/metrics.py
+-rw-r--r--  2.0 unx     9543 b- defN 24-Apr-18 09:18 nucliadb/ingest/consumer/pull.py
+-rw-r--r--  2.0 unx     6935 b- defN 24-Apr-18 09:18 nucliadb/ingest/consumer/service.py
+-rw-r--r--  2.0 unx     4331 b- defN 24-Apr-18 09:18 nucliadb/ingest/consumer/shard_creator.py
+-rw-r--r--  2.0 unx     2656 b- defN 24-Apr-18 09:18 nucliadb/ingest/consumer/utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Apr-18 09:18 nucliadb/ingest/fields/__init__.py
+-rw-r--r--  2.0 unx    18433 b- defN 24-Apr-18 09:18 nucliadb/ingest/fields/base.py
+-rw-r--r--  2.0 unx     6516 b- defN 24-Apr-18 09:18 nucliadb/ingest/fields/conversation.py
+-rw-r--r--  2.0 unx     1223 b- defN 24-Apr-18 09:18 nucliadb/ingest/fields/date.py
+-rw-r--r--  2.0 unx     1205 b- defN 24-Apr-18 09:18 nucliadb/ingest/fields/exceptions.py
+-rw-r--r--  2.0 unx     5159 b- defN 24-Apr-18 09:18 nucliadb/ingest/fields/file.py
+-rw-r--r--  2.0 unx     1547 b- defN 24-Apr-18 09:18 nucliadb/ingest/fields/generic.py
+-rw-r--r--  2.0 unx     1235 b- defN 24-Apr-18 09:18 nucliadb/ingest/fields/keywordset.py
+-rw-r--r--  2.0 unx     2250 b- defN 24-Apr-18 09:18 nucliadb/ingest/fields/layout.py
+-rw-r--r--  2.0 unx     4084 b- defN 24-Apr-18 09:18 nucliadb/ingest/fields/link.py
+-rw-r--r--  2.0 unx     1319 b- defN 24-Apr-18 09:18 nucliadb/ingest/fields/text.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Apr-18 09:18 nucliadb/ingest/orm/__init__.py
+-rw-r--r--  2.0 unx    28367 b- defN 24-Apr-18 09:18 nucliadb/ingest/orm/brain.py
+-rw-r--r--  2.0 unx    15758 b- defN 24-Apr-18 09:18 nucliadb/ingest/orm/entities.py
+-rw-r--r--  2.0 unx     1279 b- defN 24-Apr-18 09:18 nucliadb/ingest/orm/exceptions.py
+-rw-r--r--  2.0 unx    18731 b- defN 24-Apr-18 09:18 nucliadb/ingest/orm/knowledgebox.py
+-rw-r--r--  2.0 unx     1096 b- defN 24-Apr-18 09:18 nucliadb/ingest/orm/metrics.py
+-rw-r--r--  2.0 unx    60647 b- defN 24-Apr-18 09:18 nucliadb/ingest/orm/resource.py
+-rw-r--r--  2.0 unx     1739 b- defN 24-Apr-18 09:18 nucliadb/ingest/orm/synonyms.py
+-rw-r--r--  2.0 unx     3683 b- defN 24-Apr-18 09:18 nucliadb/ingest/orm/utils.py
+-rw-r--r--  2.0 unx    26460 b- defN 24-Apr-18 09:18 nucliadb/ingest/orm/processor/__init__.py
+-rw-r--r--  2.0 unx     1690 b- defN 24-Apr-18 09:18 nucliadb/ingest/orm/processor/sequence_manager.py
+-rw-r--r--  2.0 unx     2057 b- defN 24-Apr-18 09:18 nucliadb/ingest/service/__init__.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Apr-18 09:18 nucliadb/ingest/service/exceptions.py
+-rw-r--r--  2.0 unx    37355 b- defN 24-Apr-18 09:18 nucliadb/ingest/service/writer.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Apr-18 09:18 nucliadb/ingest/tests/__init__.py
+-rw-r--r--  2.0 unx     1157 b- defN 24-Apr-18 09:18 nucliadb/ingest/tests/conftest.py
+-rw-r--r--  2.0 unx    24068 b- defN 24-Apr-18 09:18 nucliadb/ingest/tests/fixtures.py
+-rw-r--r--  2.0 unx    62843 b- defN 24-Apr-18 09:18 nucliadb/ingest/tests/vectors.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Apr-18 09:18 nucliadb/ingest/tests/integration/__init__.py
+-rw-r--r--  2.0 unx      833 b- defN 24-Apr-18 09:18 nucliadb/ingest/tests/integration/consumer/__init__.py
+-rw-r--r--  2.0 unx     2549 b- defN 24-Apr-18 09:18 nucliadb/ingest/tests/integration/consumer/test_auditing.py
+-rw-r--r--  2.0 unx     2591 b- defN 24-Apr-18 09:18 nucliadb/ingest/tests/integration/consumer/test_materializer.py
+-rw-r--r--  2.0 unx     4465 b- defN 24-Apr-18 09:18 nucliadb/ingest/tests/integration/consumer/test_pull.py
+-rw-r--r--  2.0 unx     2763 b- defN 24-Apr-18 09:18 nucliadb/ingest/tests/integration/consumer/test_service.py
+-rw-r--r--  2.0 unx     2019 b- defN 24-Apr-18 09:18 nucliadb/ingest/tests/integration/consumer/test_shard_creator.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Apr-18 09:18 nucliadb/ingest/tests/integration/ingest/__init__.py
+-rw-r--r--  2.0 unx    27334 b- defN 24-Apr-18 09:18 nucliadb/ingest/tests/integration/ingest/test_ingest.py
+-rw-r--r--  2.0 unx     3040 b- defN 24-Apr-18 09:18 nucliadb/ingest/tests/integration/ingest/test_processing_engine.py
+-rw-r--r--  2.0 unx     8586 b- defN 24-Apr-18 09:18 nucliadb/ingest/tests/integration/ingest/test_relations.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Apr-18 09:18 nucliadb/ingest/tests/unit/__init__.py
+-rw-r--r--  2.0 unx     1189 b- defN 24-Apr-18 09:18 nucliadb/ingest/tests/unit/test_cache.py
+-rw-r--r--  2.0 unx     1432 b- defN 24-Apr-18 09:18 nucliadb/ingest/tests/unit/test_partitions.py
+-rw-r--r--  2.0 unx     5807 b- defN 24-Apr-18 09:18 nucliadb/ingest/tests/unit/test_processing.py
+-rw-r--r--  2.0 unx      978 b- defN 24-Apr-18 09:18 nucliadb/ingest/tests/unit/test_settings.py
+-rw-r--r--  2.0 unx      833 b- defN 24-Apr-18 09:18 nucliadb/ingest/tests/unit/consumer/__init__.py
+-rw-r--r--  2.0 unx     3981 b- defN 24-Apr-18 09:18 nucliadb/ingest/tests/unit/consumer/test_auditing.py
+-rw-r--r--  2.0 unx     2472 b- defN 24-Apr-18 09:18 nucliadb/ingest/tests/unit/consumer/test_consumer.py
+-rw-r--r--  2.0 unx     2063 b- defN 24-Apr-18 09:18 nucliadb/ingest/tests/unit/consumer/test_pull.py
+-rw-r--r--  2.0 unx     4075 b- defN 24-Apr-18 09:18 nucliadb/ingest/tests/unit/consumer/test_shard_creator.py
+-rw-r--r--  2.0 unx     1934 b- defN 24-Apr-18 09:18 nucliadb/ingest/tests/unit/consumer/test_utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Apr-18 09:18 nucliadb/ingest/tests/unit/orm/__init__.py
+-rw-r--r--  2.0 unx     9876 b- defN 24-Apr-18 09:18 nucliadb/ingest/tests/unit/orm/test_brain.py
+-rw-r--r--  2.0 unx     2435 b- defN 24-Apr-18 09:18 nucliadb/ingest/tests/unit/orm/test_brain_vectors.py
+-rw-r--r--  2.0 unx     1174 b- defN 24-Apr-18 09:18 nucliadb/ingest/tests/unit/orm/test_orm_utils.py
+-rw-r--r--  2.0 unx     4045 b- defN 24-Apr-18 09:18 nucliadb/ingest/tests/unit/orm/test_processor.py
+-rw-r--r--  2.0 unx    11005 b- defN 24-Apr-18 09:18 nucliadb/ingest/tests/unit/orm/test_resource.py
+-rw-r--r--  2.0 unx     2216 b- defN 24-Apr-18 09:18 nucliadb/middleware/__init__.py
+-rw-r--r--  2.0 unx     3912 b- defN 24-Apr-18 09:18 nucliadb/middleware/transaction.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Apr-18 09:18 nucliadb/migrator/__init__.py
+-rw-r--r--  2.0 unx     2119 b- defN 24-Apr-18 09:18 nucliadb/migrator/command.py
+-rw-r--r--  2.0 unx     1334 b- defN 24-Apr-18 09:18 nucliadb/migrator/context.py
+-rw-r--r--  2.0 unx     5104 b- defN 24-Apr-18 09:18 nucliadb/migrator/datamanager.py
+-rw-r--r--  2.0 unx      889 b- defN 24-Apr-18 09:18 nucliadb/migrator/exceptions.py
+-rw-r--r--  2.0 unx     9237 b- defN 24-Apr-18 09:18 nucliadb/migrator/migrator.py
+-rw-r--r--  2.0 unx     1145 b- defN 24-Apr-18 09:18 nucliadb/migrator/models.py
+-rw-r--r--  2.0 unx     1110 b- defN 24-Apr-18 09:18 nucliadb/migrator/settings.py
+-rw-r--r--  2.0 unx     2346 b- defN 24-Apr-18 09:18 nucliadb/migrator/utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Apr-18 09:18 nucliadb/models/__init__.py
+-rw-r--r--  2.0 unx     1599 b- defN 24-Apr-18 09:18 nucliadb/models/responses.py
+-rw-r--r--  2.0 unx     6041 b- defN 24-Apr-18 09:18 nucliadb/purge/__init__.py
+-rw-r--r--  2.0 unx     9364 b- defN 24-Apr-18 09:18 nucliadb/purge/orphan_shards.py
+-rw-r--r--  2.0 unx     1328 b- defN 24-Apr-18 09:18 nucliadb/reader/__init__.py
+-rw-r--r--  2.0 unx     3709 b- defN 24-Apr-18 09:18 nucliadb/reader/app.py
+-rw-r--r--  2.0 unx     1366 b- defN 24-Apr-18 09:18 nucliadb/reader/lifecycle.py
+-rw-r--r--  2.0 unx     1031 b- defN 24-Apr-18 09:18 nucliadb/reader/openapi.py
+-rw-r--r--  2.0 unx     1447 b- defN 24-Apr-18 09:18 nucliadb/reader/run.py
+-rw-r--r--  2.0 unx      872 b- defN 24-Apr-18 09:18 nucliadb/reader/api/__init__.py
+-rw-r--r--  2.0 unx     2434 b- defN 24-Apr-18 09:18 nucliadb/reader/api/models.py
+-rw-r--r--  2.0 unx     1110 b- defN 24-Apr-18 09:18 nucliadb/reader/api/v1/__init__.py
+-rw-r--r--  2.0 unx    12368 b- defN 24-Apr-18 09:18 nucliadb/reader/api/v1/download.py
+-rw-r--r--  2.0 unx     6450 b- defN 24-Apr-18 09:18 nucliadb/reader/api/v1/export_import.py
+-rw-r--r--  2.0 unx     3632 b- defN 24-Apr-18 09:18 nucliadb/reader/api/v1/knowledgebox.py
+-rw-r--r--  2.0 unx     2093 b- defN 24-Apr-18 09:18 nucliadb/reader/api/v1/learning_collector.py
+-rw-r--r--  2.0 unx     4454 b- defN 24-Apr-18 09:18 nucliadb/reader/api/v1/learning_config.py
+-rw-r--r--  2.0 unx    13928 b- defN 24-Apr-18 09:18 nucliadb/reader/api/v1/resource.py
+-rw-r--r--  2.0 unx     1011 b- defN 24-Apr-18 09:18 nucliadb/reader/api/v1/router.py
+-rw-r--r--  2.0 unx    13882 b- defN 24-Apr-18 09:18 nucliadb/reader/api/v1/services.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Apr-18 09:18 nucliadb/reader/reader/__init__.py
+-rw-r--r--  2.0 unx     8155 b- defN 24-Apr-18 09:18 nucliadb/reader/reader/notifications.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Apr-18 09:18 nucliadb/reader/tests/__init__.py
+-rw-r--r--  2.0 unx     1224 b- defN 24-Apr-18 09:18 nucliadb/reader/tests/conftest.py
+-rw-r--r--  2.0 unx     4345 b- defN 24-Apr-18 09:18 nucliadb/reader/tests/fixtures.py
+-rw-r--r--  2.0 unx     2748 b- defN 24-Apr-18 09:18 nucliadb/reader/tests/test_list_resources.py
+-rw-r--r--  2.0 unx    10199 b- defN 24-Apr-18 09:18 nucliadb/reader/tests/test_reader_file_download.py
+-rw-r--r--  2.0 unx    10586 b- defN 24-Apr-18 09:18 nucliadb/reader/tests/test_reader_resource.py
+-rw-r--r--  2.0 unx     6535 b- defN 24-Apr-18 09:18 nucliadb/reader/tests/test_reader_resource_field.py
+-rw-r--r--  2.0 unx     1535 b- defN 24-Apr-18 09:18 nucliadb/search/__init__.py
+-rw-r--r--  2.0 unx     4905 b- defN 24-Apr-18 09:18 nucliadb/search/app.py
+-rw-r--r--  2.0 unx     1956 b- defN 24-Apr-18 09:18 nucliadb/search/lifecycle.py
+-rw-r--r--  2.0 unx     1016 b- defN 24-Apr-18 09:18 nucliadb/search/openapi.py
+-rw-r--r--  2.0 unx    19798 b- defN 24-Apr-18 09:18 nucliadb/search/predict.py
+-rw-r--r--  2.0 unx     1402 b- defN 24-Apr-18 09:18 nucliadb/search/run.py
+-rw-r--r--  2.0 unx     1193 b- defN 24-Apr-18 09:18 nucliadb/search/settings.py
+-rw-r--r--  2.0 unx     1037 b- defN 24-Apr-18 09:18 nucliadb/search/utilities.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Apr-18 09:18 nucliadb/search/api/__init__.py
+-rw-r--r--  2.0 unx     1272 b- defN 24-Apr-18 09:18 nucliadb/search/api/v1/__init__.py
+-rw-r--r--  2.0 unx     9913 b- defN 24-Apr-18 09:18 nucliadb/search/api/v1/chat.py
+-rw-r--r--  2.0 unx     2665 b- defN 24-Apr-18 09:18 nucliadb/search/api/v1/feedback.py
+-rw-r--r--  2.0 unx     8804 b- defN 24-Apr-18 09:18 nucliadb/search/api/v1/find.py
+-rw-r--r--  2.0 unx     7026 b- defN 24-Apr-18 09:18 nucliadb/search/api/v1/knowledgebox.py
+-rw-r--r--  2.0 unx     3041 b- defN 24-Apr-18 09:18 nucliadb/search/api/v1/predict_proxy.py
+-rw-r--r--  2.0 unx      988 b- defN 24-Apr-18 09:18 nucliadb/search/api/v1/router.py
+-rw-r--r--  2.0 unx    18359 b- defN 24-Apr-18 09:18 nucliadb/search/api/v1/search.py
+-rw-r--r--  2.0 unx     5928 b- defN 24-Apr-18 09:18 nucliadb/search/api/v1/suggest.py
+-rw-r--r--  2.0 unx     2536 b- defN 24-Apr-18 09:18 nucliadb/search/api/v1/summarize.py
+-rw-r--r--  2.0 unx     1412 b- defN 24-Apr-18 09:18 nucliadb/search/api/v1/utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Apr-18 09:18 nucliadb/search/api/v1/resource/__init__.py
+-rw-r--r--  2.0 unx     6095 b- defN 24-Apr-18 09:18 nucliadb/search/api/v1/resource/ask.py
+-rw-r--r--  2.0 unx     5887 b- defN 24-Apr-18 09:18 nucliadb/search/api/v1/resource/chat.py
+-rw-r--r--  2.0 unx     5293 b- defN 24-Apr-18 09:18 nucliadb/search/api/v1/resource/search.py
+-rw-r--r--  2.0 unx      833 b- defN 24-Apr-18 09:18 nucliadb/search/requesters/__init__.py
+-rw-r--r--  2.0 unx     9070 b- defN 24-Apr-18 09:18 nucliadb/search/requesters/utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Apr-18 09:18 nucliadb/search/search/__init__.py
+-rw-r--r--  2.0 unx     2746 b- defN 24-Apr-18 09:18 nucliadb/search/search/cache.py
+-rw-r--r--  2.0 unx     1154 b- defN 24-Apr-18 09:18 nucliadb/search/search/exceptions.py
+-rw-r--r--  2.0 unx     5465 b- defN 24-Apr-18 09:18 nucliadb/search/search/fetch.py
+-rw-r--r--  2.0 unx     6513 b- defN 24-Apr-18 09:18 nucliadb/search/search/filters.py
+-rw-r--r--  2.0 unx     4646 b- defN 24-Apr-18 09:18 nucliadb/search/search/find.py
+-rw-r--r--  2.0 unx    17152 b- defN 24-Apr-18 09:18 nucliadb/search/search/find_merge.py
+-rw-r--r--  2.0 unx    21118 b- defN 24-Apr-18 09:18 nucliadb/search/search/merge.py
+-rw-r--r--  2.0 unx     1130 b- defN 24-Apr-18 09:18 nucliadb/search/search/metrics.py
+-rw-r--r--  2.0 unx     8698 b- defN 24-Apr-18 09:18 nucliadb/search/search/paragraphs.py
+-rw-r--r--  2.0 unx     3026 b- defN 24-Apr-18 09:18 nucliadb/search/search/predict_proxy.py
+-rw-r--r--  2.0 unx    32831 b- defN 24-Apr-18 09:18 nucliadb/search/search/query.py
+-rw-r--r--  2.0 unx     3149 b- defN 24-Apr-18 09:18 nucliadb/search/search/shards.py
+-rw-r--r--  2.0 unx     5101 b- defN 24-Apr-18 09:18 nucliadb/search/search/summarize.py
+-rw-r--r--  2.0 unx     2438 b- defN 24-Apr-18 09:18 nucliadb/search/search/utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Apr-18 09:18 nucliadb/search/search/chat/__init__.py
+-rw-r--r--  2.0 unx     2058 b- defN 24-Apr-18 09:18 nucliadb/search/search/chat/images.py
+-rw-r--r--  2.0 unx    20793 b- defN 24-Apr-18 09:18 nucliadb/search/search/chat/prompt.py
+-rw-r--r--  2.0 unx    15347 b- defN 24-Apr-18 09:18 nucliadb/search/search/chat/query.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Apr-18 09:18 nucliadb/search/tests/__init__.py
+-rw-r--r--  2.0 unx     1295 b- defN 24-Apr-18 09:18 nucliadb/search/tests/conftest.py
+-rw-r--r--  2.0 unx     6578 b- defN 24-Apr-18 09:18 nucliadb/search/tests/fixtures.py
+-rw-r--r--  2.0 unx    15529 b- defN 24-Apr-18 09:18 nucliadb/search/tests/node.py
+-rw-r--r--  2.0 unx      833 b- defN 24-Apr-18 09:18 nucliadb/search/tests/unit/__init__.py
+-rw-r--r--  2.0 unx     2649 b- defN 24-Apr-18 09:18 nucliadb/search/tests/unit/test_app.py
+-rw-r--r--  2.0 unx     3374 b- defN 24-Apr-18 09:18 nucliadb/search/tests/unit/test_find_merge.py
+-rw-r--r--  2.0 unx     1400 b- defN 24-Apr-18 09:18 nucliadb/search/tests/unit/test_merge.py
+-rw-r--r--  2.0 unx    17080 b- defN 24-Apr-18 09:18 nucliadb/search/tests/unit/test_predict.py
+-rw-r--r--  2.0 unx     1317 b- defN 24-Apr-18 09:18 nucliadb/search/tests/unit/test_run.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Apr-18 09:18 nucliadb/search/tests/unit/api/__init__.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Apr-18 09:18 nucliadb/search/tests/unit/api/v1/__init__.py
+-rw-r--r--  2.0 unx     2966 b- defN 24-Apr-18 09:18 nucliadb/search/tests/unit/api/v1/test_chat.py
+-rw-r--r--  2.0 unx     2865 b- defN 24-Apr-18 09:18 nucliadb/search/tests/unit/api/v1/test_predict_proxy.py
+-rw-r--r--  2.0 unx     2901 b- defN 24-Apr-18 09:18 nucliadb/search/tests/unit/api/v1/test_summarize.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Apr-18 09:18 nucliadb/search/tests/unit/api/v1/resource/__init__.py
+-rw-r--r--  2.0 unx     2411 b- defN 24-Apr-18 09:18 nucliadb/search/tests/unit/api/v1/resource/test_ask.py
+-rw-r--r--  2.0 unx     3040 b- defN 24-Apr-18 09:18 nucliadb/search/tests/unit/api/v1/resource/test_chat.py
+-rw-r--r--  2.0 unx      833 b- defN 24-Apr-18 09:18 nucliadb/search/tests/unit/search/__init__.py
+-rw-r--r--  2.0 unx     8567 b- defN 24-Apr-18 09:18 nucliadb/search/tests/unit/search/test_chat_prompt.py
+-rw-r--r--  2.0 unx     3736 b- defN 24-Apr-18 09:18 nucliadb/search/tests/unit/search/test_fetch.py
+-rw-r--r--  2.0 unx     4306 b- defN 24-Apr-18 09:18 nucliadb/search/tests/unit/search/test_filters.py
+-rw-r--r--  2.0 unx     4492 b- defN 24-Apr-18 09:18 nucliadb/search/tests/unit/search/test_paragraphs.py
+-rw-r--r--  2.0 unx     3496 b- defN 24-Apr-18 09:18 nucliadb/search/tests/unit/search/test_predict_proxy.py
+-rw-r--r--  2.0 unx     7001 b- defN 24-Apr-18 09:18 nucliadb/search/tests/unit/search/test_query.py
+-rw-r--r--  2.0 unx      833 b- defN 24-Apr-18 09:18 nucliadb/search/tests/unit/search/requesters/__init__.py
+-rw-r--r--  2.0 unx     6455 b- defN 24-Apr-18 09:18 nucliadb/search/tests/unit/search/requesters/test_utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Apr-18 09:18 nucliadb/search/tests/unit/search/search/__init__.py
+-rw-r--r--  2.0 unx     1759 b- defN 24-Apr-18 09:18 nucliadb/search/tests/unit/search/search/test_shards.py
+-rw-r--r--  2.0 unx     2511 b- defN 24-Apr-18 09:18 nucliadb/search/tests/unit/search/search/test_utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Apr-18 09:18 nucliadb/standalone/__init__.py
+-rw-r--r--  2.0 unx     6746 b- defN 24-Apr-18 09:18 nucliadb/standalone/api_router.py
+-rw-r--r--  2.0 unx     5763 b- defN 24-Apr-18 09:18 nucliadb/standalone/app.py
+-rw-r--r--  2.0 unx     7800 b- defN 24-Apr-18 09:18 nucliadb/standalone/auth.py
+-rw-r--r--  2.0 unx     5309 b- defN 24-Apr-18 09:18 nucliadb/standalone/config.py
+-rw-r--r--  2.0 unx     6930 b- defN 24-Apr-18 09:18 nucliadb/standalone/introspect.py
+-rw-r--r--  2.0 unx     2488 b- defN 24-Apr-18 09:18 nucliadb/standalone/lifecycle.py
+-rw-r--r--  2.0 unx     1317 b- defN 24-Apr-18 09:18 nucliadb/standalone/purge.py
+-rw-r--r--  2.0 unx     5336 b- defN 24-Apr-18 09:18 nucliadb/standalone/run.py
+-rw-r--r--  2.0 unx     5781 b- defN 24-Apr-18 09:18 nucliadb/standalone/settings.py
+-rw-r--r--  2.0 unx     3132 b- defN 24-Apr-18 09:18 nucliadb/standalone/versions.py
+-rw-r--r--  2.0 unx     2285 b- defN 24-Apr-18 09:18 nucliadb/standalone/static/favicon.ico
+-rw-r--r--  2.0 unx     3833 b- defN 24-Apr-18 09:18 nucliadb/standalone/static/index.html
+-rw-r--r--  2.0 unx     2639 b- defN 24-Apr-18 09:18 nucliadb/standalone/static/logo.svg
+-rw-r--r--  2.0 unx      835 b- defN 24-Apr-18 09:18 nucliadb/standalone/tests/__init__.py
+-rw-r--r--  2.0 unx     1294 b- defN 24-Apr-18 09:18 nucliadb/standalone/tests/conftest.py
+-rw-r--r--  2.0 unx     1319 b- defN 24-Apr-18 09:18 nucliadb/standalone/tests/fixtures.py
+-rw-r--r--  2.0 unx      833 b- defN 24-Apr-18 09:18 nucliadb/standalone/tests/unit/__init__.py
+-rw-r--r--  2.0 unx     1722 b- defN 24-Apr-18 09:18 nucliadb/standalone/tests/unit/test_api_router.py
+-rw-r--r--  2.0 unx     5509 b- defN 24-Apr-18 09:18 nucliadb/standalone/tests/unit/test_auth.py
+-rw-r--r--  2.0 unx     1334 b- defN 24-Apr-18 09:18 nucliadb/standalone/tests/unit/test_introspect.py
+-rw-r--r--  2.0 unx     1472 b- defN 24-Apr-18 09:18 nucliadb/standalone/tests/unit/test_run.py
+-rw-r--r--  2.0 unx     1972 b- defN 24-Apr-18 09:18 nucliadb/standalone/tests/unit/test_versions.py
+-rw-r--r--  2.0 unx     1037 b- defN 24-Apr-18 09:18 nucliadb/tasks/__init__.py
+-rw-r--r--  2.0 unx     7655 b- defN 24-Apr-18 09:18 nucliadb/tasks/consumer.py
+-rw-r--r--  2.0 unx      924 b- defN 24-Apr-18 09:18 nucliadb/tasks/logger.py
+-rw-r--r--  2.0 unx     1378 b- defN 24-Apr-18 09:18 nucliadb/tasks/models.py
+-rw-r--r--  2.0 unx     3457 b- defN 24-Apr-18 09:18 nucliadb/tasks/producer.py
+-rw-r--r--  2.0 unx     1753 b- defN 24-Apr-18 09:18 nucliadb/tasks/registry.py
+-rw-r--r--  2.0 unx     1360 b- defN 24-Apr-18 09:18 nucliadb/tasks/utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Apr-18 09:18 nucliadb/tests/__init__.py
+-rw-r--r--  2.0 unx     1229 b- defN 24-Apr-18 09:18 nucliadb/tests/conftest.py
+-rw-r--r--  2.0 unx    22365 b- defN 24-Apr-18 09:18 nucliadb/tests/fixtures.py
+-rw-r--r--  2.0 unx     7549 b- defN 24-Apr-18 09:18 nucliadb/tests/tikv.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Apr-18 09:18 nucliadb/tests/benchmarks/__init__.py
+-rw-r--r--  2.0 unx     3032 b- defN 24-Apr-18 09:18 nucliadb/tests/benchmarks/test_search.py
+-rw-r--r--  2.0 unx      919 b- defN 24-Apr-18 09:18 nucliadb/tests/knowledgeboxes/__init__.py
+-rw-r--r--  2.0 unx     7002 b- defN 24-Apr-18 09:18 nucliadb/tests/knowledgeboxes/philosophy_books.py
+-rw-r--r--  2.0 unx     3037 b- defN 24-Apr-18 09:18 nucliadb/tests/knowledgeboxes/ten_dummy_resources.py
+-rw-r--r--  2.0 unx     1148 b- defN 24-Apr-18 09:18 nucliadb/tests/migrations/__init__.py
+-rw-r--r--  2.0 unx     2726 b- defN 24-Apr-18 09:18 nucliadb/tests/migrations/test_migration_0017.py
+-rw-r--r--  2.0 unx     3625 b- defN 24-Apr-18 09:18 nucliadb/tests/migrations/test_migration_0018.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Apr-18 09:18 nucliadb/tests/unit/__init__.py
+-rw-r--r--  2.0 unx     1487 b- defN 24-Apr-18 09:18 nucliadb/tests/unit/test_field_ids.py
+-rw-r--r--  2.0 unx     2758 b- defN 24-Apr-18 09:18 nucliadb/tests/unit/test_health.py
+-rw-r--r--  2.0 unx     1543 b- defN 24-Apr-18 09:18 nucliadb/tests/unit/test_kb_slugs.py
+-rw-r--r--  2.0 unx     7892 b- defN 24-Apr-18 09:18 nucliadb/tests/unit/test_learning_proxy.py
+-rw-r--r--  2.0 unx     2642 b- defN 24-Apr-18 09:18 nucliadb/tests/unit/test_metrics_exporter.py
+-rw-r--r--  2.0 unx     1341 b- defN 24-Apr-18 09:18 nucliadb/tests/unit/test_openapi.py
+-rw-r--r--  2.0 unx     3656 b- defN 24-Apr-18 09:18 nucliadb/tests/unit/test_purge.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Apr-18 09:18 nucliadb/tests/unit/common/__init__.py
+-rw-r--r--  2.0 unx     1268 b- defN 24-Apr-18 09:18 nucliadb/tests/unit/common/test_context.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Apr-18 09:18 nucliadb/tests/unit/common/cluster/__init__.py
+-rw-r--r--  2.0 unx    11955 b- defN 24-Apr-18 09:18 nucliadb/tests/unit/common/cluster/test_cluster.py
+-rw-r--r--  2.0 unx     5387 b- defN 24-Apr-18 09:18 nucliadb/tests/unit/common/cluster/test_kb_shard_manager.py
+-rw-r--r--  2.0 unx     9470 b- defN 24-Apr-18 09:18 nucliadb/tests/unit/common/cluster/test_rollover.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Apr-18 09:18 nucliadb/tests/unit/common/cluster/discovery/__init__.py
+-rw-r--r--  2.0 unx     5584 b- defN 24-Apr-18 09:18 nucliadb/tests/unit/common/cluster/discovery/test_k8s.py
+-rw-r--r--  2.0 unx      833 b- defN 24-Apr-18 09:18 nucliadb/tests/unit/common/cluster/standalone/__init__.py
+-rw-r--r--  2.0 unx     3750 b- defN 24-Apr-18 09:18 nucliadb/tests/unit/common/cluster/standalone/test_service.py
+-rw-r--r--  2.0 unx     2114 b- defN 24-Apr-18 09:18 nucliadb/tests/unit/common/cluster/standalone/test_utils.py
+-rw-r--r--  2.0 unx      833 b- defN 24-Apr-18 09:18 nucliadb/tests/unit/common/maindb/__init__.py
+-rw-r--r--  2.0 unx     3579 b- defN 24-Apr-18 09:18 nucliadb/tests/unit/common/maindb/test_driver.py
+-rw-r--r--  2.0 unx     1869 b- defN 24-Apr-18 09:18 nucliadb/tests/unit/common/maindb/test_tikv.py
+-rw-r--r--  2.0 unx     2998 b- defN 24-Apr-18 09:18 nucliadb/tests/unit/common/maindb/test_utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Apr-18 09:18 nucliadb/tests/unit/export_import/__init__.py
+-rw-r--r--  2.0 unx     1435 b- defN 24-Apr-18 09:18 nucliadb/tests/unit/export_import/test_datamanager.py
+-rw-r--r--  2.0 unx     9706 b- defN 24-Apr-18 09:18 nucliadb/tests/unit/export_import/test_utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Apr-18 09:18 nucliadb/tests/unit/migrator/__init__.py
+-rw-r--r--  2.0 unx     3233 b- defN 24-Apr-18 09:18 nucliadb/tests/unit/migrator/test_migrator.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Apr-18 09:18 nucliadb/tests/unit/tasks/__init__.py
+-rw-r--r--  2.0 unx     1375 b- defN 24-Apr-18 09:18 nucliadb/tests/unit/tasks/conftest.py
+-rw-r--r--  2.0 unx     2714 b- defN 24-Apr-18 09:18 nucliadb/tests/unit/tasks/test_consumer.py
+-rw-r--r--  2.0 unx     3189 b- defN 24-Apr-18 09:18 nucliadb/tests/unit/tasks/test_producer.py
+-rw-r--r--  2.0 unx     1827 b- defN 24-Apr-18 09:18 nucliadb/tests/unit/tasks/test_tasks.py
+-rw-r--r--  2.0 unx     2507 b- defN 24-Apr-18 09:18 nucliadb/tests/utils/__init__.py
+-rw-r--r--  2.0 unx     1797 b- defN 24-Apr-18 09:18 nucliadb/tests/utils/aiohttp_session.py
+-rw-r--r--  2.0 unx     2533 b- defN 24-Apr-18 09:18 nucliadb/tests/utils/entities.py
+-rw-r--r--  2.0 unx     6327 b- defN 24-Apr-18 09:18 nucliadb/tests/utils/broker_messages/__init__.py
+-rw-r--r--  2.0 unx     7557 b- defN 24-Apr-18 09:18 nucliadb/tests/utils/broker_messages/fields.py
+-rw-r--r--  2.0 unx     1196 b- defN 24-Apr-18 09:18 nucliadb/tests/utils/broker_messages/helpers.py
+-rw-r--r--  2.0 unx     1325 b- defN 24-Apr-18 09:18 nucliadb/train/__init__.py
+-rw-r--r--  2.0 unx     3530 b- defN 24-Apr-18 09:18 nucliadb/train/app.py
+-rw-r--r--  2.0 unx     3800 b- defN 24-Apr-18 09:18 nucliadb/train/generator.py
+-rw-r--r--  2.0 unx     1698 b- defN 24-Apr-18 09:18 nucliadb/train/lifecycle.py
+-rw-r--r--  2.0 unx     1198 b- defN 24-Apr-18 09:18 nucliadb/train/models.py
+-rw-r--r--  2.0 unx     5706 b- defN 24-Apr-18 09:18 nucliadb/train/nodes.py
+-rw-r--r--  2.0 unx     1400 b- defN 24-Apr-18 09:18 nucliadb/train/run.py
+-rw-r--r--  2.0 unx     5926 b- defN 24-Apr-18 09:18 nucliadb/train/servicer.py
+-rw-r--r--  2.0 unx     1415 b- defN 24-Apr-18 09:18 nucliadb/train/settings.py
+-rw-r--r--  2.0 unx     1496 b- defN 24-Apr-18 09:18 nucliadb/train/types.py
+-rw-r--r--  2.0 unx     3265 b- defN 24-Apr-18 09:18 nucliadb/train/upload.py
+-rw-r--r--  2.0 unx     6420 b- defN 24-Apr-18 09:18 nucliadb/train/uploader.py
+-rw-r--r--  2.0 unx     3179 b- defN 24-Apr-18 09:18 nucliadb/train/utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Apr-18 09:18 nucliadb/train/api/__init__.py
+-rw-r--r--  2.0 unx     1479 b- defN 24-Apr-18 09:18 nucliadb/train/api/utils.py
+-rw-r--r--  2.0 unx      928 b- defN 24-Apr-18 09:18 nucliadb/train/api/v1/__init__.py
+-rw-r--r--  2.0 unx     2065 b- defN 24-Apr-18 09:18 nucliadb/train/api/v1/check.py
+-rw-r--r--  2.0 unx      910 b- defN 24-Apr-18 09:18 nucliadb/train/api/v1/router.py
+-rw-r--r--  2.0 unx     1905 b- defN 24-Apr-18 09:18 nucliadb/train/api/v1/shards.py
+-rw-r--r--  2.0 unx     2129 b- defN 24-Apr-18 09:18 nucliadb/train/api/v1/trainset.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Apr-18 09:18 nucliadb/train/generators/__init__.py
+-rw-r--r--  2.0 unx     3723 b- defN 24-Apr-18 09:18 nucliadb/train/generators/field_classifier.py
+-rw-r--r--  2.0 unx     6712 b- defN 24-Apr-18 09:18 nucliadb/train/generators/image_classifier.py
+-rw-r--r--  2.0 unx     2789 b- defN 24-Apr-18 09:18 nucliadb/train/generators/paragraph_classifier.py
+-rw-r--r--  2.0 unx     3590 b- defN 24-Apr-18 09:18 nucliadb/train/generators/paragraph_streaming.py
+-rw-r--r--  2.0 unx     5372 b- defN 24-Apr-18 09:18 nucliadb/train/generators/question_answer_streaming.py
+-rw-r--r--  2.0 unx     5160 b- defN 24-Apr-18 09:18 nucliadb/train/generators/sentence_classifier.py
+-rw-r--r--  2.0 unx    10446 b- defN 24-Apr-18 09:18 nucliadb/train/generators/token_classifier.py
+-rw-r--r--  2.0 unx     3877 b- defN 24-Apr-18 09:18 nucliadb/train/generators/utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Apr-18 09:18 nucliadb/train/tests/__init__.py
+-rw-r--r--  2.0 unx     1125 b- defN 24-Apr-18 09:18 nucliadb/train/tests/conftest.py
+-rw-r--r--  2.0 unx    11053 b- defN 24-Apr-18 09:18 nucliadb/train/tests/fixtures.py
+-rw-r--r--  2.0 unx     4598 b- defN 24-Apr-18 09:18 nucliadb/train/tests/test_field_classification.py
+-rw-r--r--  2.0 unx     2729 b- defN 24-Apr-18 09:18 nucliadb/train/tests/test_get_entities.py
+-rw-r--r--  2.0 unx     1876 b- defN 24-Apr-18 09:18 nucliadb/train/tests/test_get_info.py
+-rw-r--r--  2.0 unx     1382 b- defN 24-Apr-18 09:18 nucliadb/train/tests/test_get_ontology.py
+-rw-r--r--  2.0 unx     2417 b- defN 24-Apr-18 09:18 nucliadb/train/tests/test_get_ontology_count.py
+-rw-r--r--  2.0 unx     7669 b- defN 24-Apr-18 09:18 nucliadb/train/tests/test_image_classification.py
+-rw-r--r--  2.0 unx     1416 b- defN 24-Apr-18 09:18 nucliadb/train/tests/test_list_fields.py
+-rw-r--r--  2.0 unx     2944 b- defN 24-Apr-18 09:18 nucliadb/train/tests/test_list_paragraphs.py
+-rw-r--r--  2.0 unx     1423 b- defN 24-Apr-18 09:18 nucliadb/train/tests/test_list_resources.py
+-rw-r--r--  2.0 unx     2947 b- defN 24-Apr-18 09:18 nucliadb/train/tests/test_list_sentences.py
+-rw-r--r--  2.0 unx     4645 b- defN 24-Apr-18 09:18 nucliadb/train/tests/test_paragraph_classification.py
+-rw-r--r--  2.0 unx     4320 b- defN 24-Apr-18 09:18 nucliadb/train/tests/test_paragraph_streaming.py
+-rw-r--r--  2.0 unx     8751 b- defN 24-Apr-18 09:18 nucliadb/train/tests/test_question_answer_streaming.py
+-rw-r--r--  2.0 unx     5051 b- defN 24-Apr-18 09:18 nucliadb/train/tests/test_sentence_classification.py
+-rw-r--r--  2.0 unx     5583 b- defN 24-Apr-18 09:18 nucliadb/train/tests/test_token_classification.py
+-rw-r--r--  2.0 unx     3324 b- defN 24-Apr-18 09:18 nucliadb/train/tests/utils.py
+-rw-r--r--  2.0 unx     1328 b- defN 24-Apr-18 09:18 nucliadb/writer/__init__.py
+-rw-r--r--  2.0 unx     4268 b- defN 24-Apr-18 09:18 nucliadb/writer/app.py
+-rw-r--r--  2.0 unx    19435 b- defN 24-Apr-18 09:18 nucliadb/writer/back_pressure.py
+-rw-r--r--  2.0 unx      972 b- defN 24-Apr-18 09:18 nucliadb/writer/exceptions.py
+-rw-r--r--  2.0 unx     1953 b- defN 24-Apr-18 09:18 nucliadb/writer/lifecycle.py
+-rw-r--r--  2.0 unx     1032 b- defN 24-Apr-18 09:18 nucliadb/writer/openapi.py
+-rw-r--r--  2.0 unx     1448 b- defN 24-Apr-18 09:18 nucliadb/writer/run.py
+-rw-r--r--  2.0 unx     3074 b- defN 24-Apr-18 09:18 nucliadb/writer/settings.py
+-rw-r--r--  2.0 unx     1036 b- defN 24-Apr-18 09:18 nucliadb/writer/utilities.py
+-rw-r--r--  2.0 unx     1948 b- defN 24-Apr-18 09:18 nucliadb/writer/vectors.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Apr-18 09:18 nucliadb/writer/api/__init__.py
+-rw-r--r--  2.0 unx     1429 b- defN 24-Apr-18 09:18 nucliadb/writer/api/constants.py
+-rw-r--r--  2.0 unx     1095 b- defN 24-Apr-18 09:18 nucliadb/writer/api/v1/__init__.py
+-rw-r--r--  2.0 unx     6565 b- defN 24-Apr-18 09:18 nucliadb/writer/api/v1/export_import.py
+-rw-r--r--  2.0 unx    28320 b- defN 24-Apr-18 09:18 nucliadb/writer/api/v1/field.py
+-rw-r--r--  2.0 unx     5239 b- defN 24-Apr-18 09:18 nucliadb/writer/api/v1/knowledgebox.py
+-rw-r--r--  2.0 unx     2052 b- defN 24-Apr-18 09:18 nucliadb/writer/api/v1/learning_config.py
+-rw-r--r--  2.0 unx    19940 b- defN 24-Apr-18 09:18 nucliadb/writer/api/v1/resource.py
+-rw-r--r--  2.0 unx     1034 b- defN 24-Apr-18 09:18 nucliadb/writer/api/v1/router.py
+-rw-r--r--  2.0 unx    12733 b- defN 24-Apr-18 09:18 nucliadb/writer/api/v1/services.py
+-rw-r--r--  2.0 unx    31464 b- defN 24-Apr-18 09:18 nucliadb/writer/api/v1/upload.py
+-rw-r--r--  2.0 unx     1612 b- defN 24-Apr-18 09:18 nucliadb/writer/layouts/__init__.py
+-rw-r--r--  2.0 unx     2115 b- defN 24-Apr-18 09:18 nucliadb/writer/layouts/v1.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Apr-18 09:18 nucliadb/writer/resource/__init__.py
+-rw-r--r--  2.0 unx     1425 b- defN 24-Apr-18 09:18 nucliadb/writer/resource/audit.py
+-rw-r--r--  2.0 unx    10968 b- defN 24-Apr-18 09:18 nucliadb/writer/resource/basic.py
+-rw-r--r--  2.0 unx    16319 b- defN 24-Apr-18 09:18 nucliadb/writer/resource/field.py
+-rw-r--r--  2.0 unx     2022 b- defN 24-Apr-18 09:18 nucliadb/writer/resource/origin.py
+-rw-r--r--  2.0 unx     1152 b- defN 24-Apr-18 09:18 nucliadb/writer/resource/slug.py
+-rw-r--r--  2.0 unx      835 b- defN 24-Apr-18 09:18 nucliadb/writer/tests/__init__.py
+-rw-r--r--  2.0 unx     1200 b- defN 24-Apr-18 09:18 nucliadb/writer/tests/conftest.py
+-rw-r--r--  2.0 unx     5971 b- defN 24-Apr-18 09:18 nucliadb/writer/tests/fixtures.py
+-rw-r--r--  2.0 unx    15472 b- defN 24-Apr-18 09:18 nucliadb/writer/tests/test_fields.py
+-rw-r--r--  2.0 unx    25913 b- defN 24-Apr-18 09:18 nucliadb/writer/tests/test_files.py
+-rw-r--r--  2.0 unx     1729 b- defN 24-Apr-18 09:18 nucliadb/writer/tests/test_knowledgebox.py
+-rw-r--r--  2.0 unx     4569 b- defN 24-Apr-18 09:18 nucliadb/writer/tests/test_reprocess_file_field.py
+-rw-r--r--  2.0 unx    17449 b- defN 24-Apr-18 09:18 nucliadb/writer/tests/test_resources.py
+-rw-r--r--  2.0 unx     5120 b- defN 24-Apr-18 09:18 nucliadb/writer/tests/test_service.py
+-rw-r--r--  2.0 unx     6054 b- defN 24-Apr-18 09:18 nucliadb/writer/tests/test_tus.py
+-rw-r--r--  2.0 unx     1287 b- defN 24-Apr-18 09:18 nucliadb/writer/tests/utils.py
+-rw-r--r--  2.0 unx     5226 b- defN 24-Apr-18 09:18 nucliadb/writer/tus/__init__.py
+-rw-r--r--  2.0 unx     5082 b- defN 24-Apr-18 09:18 nucliadb/writer/tus/dm.py
+-rw-r--r--  2.0 unx     2186 b- defN 24-Apr-18 09:18 nucliadb/writer/tus/exceptions.py
+-rw-r--r--  2.0 unx    14527 b- defN 24-Apr-18 09:18 nucliadb/writer/tus/gcs.py
+-rw-r--r--  2.0 unx     5849 b- defN 24-Apr-18 09:18 nucliadb/writer/tus/local.py
+-rw-r--r--  2.0 unx     4367 b- defN 24-Apr-18 09:18 nucliadb/writer/tus/pg.py
+-rw-r--r--  2.0 unx     9069 b- defN 24-Apr-18 09:18 nucliadb/writer/tus/s3.py
+-rw-r--r--  2.0 unx     4734 b- defN 24-Apr-18 09:18 nucliadb/writer/tus/storage.py
+-rw-r--r--  2.0 unx     2556 b- defN 24-Apr-18 09:18 nucliadb/writer/tus/utils.py
+-rw-r--r--  2.0 unx     4348 b- defN 24-Apr-18 09:19 nucliadb-3.0.3.post438.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-18 09:19 nucliadb-3.0.3.post438.dist-info/WHEEL
+-rw-r--r--  2.0 unx     1268 b- defN 24-Apr-18 09:19 nucliadb-3.0.3.post438.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       20 b- defN 24-Apr-18 09:19 nucliadb-3.0.3.post438.dist-info/top_level.txt
+-rw-r--r--  2.0 unx        1 b- defN 24-Apr-18 09:19 nucliadb-3.0.3.post438.dist-info/zip-safe
+-rw-rw-r--  2.0 unx    42761 b- defN 24-Apr-18 09:19 nucliadb-3.0.3.post438.dist-info/RECORD
+456 files, 2246920 bytes uncompressed, 686583 bytes compressed:  69.5%
```

## zipnote {}

```diff
@@ -174,14 +174,17 @@
 
 Filename: nucliadb/common/datamanagers/rollover.py
 Comment: 
 
 Filename: nucliadb/common/datamanagers/utils.py
 Comment: 
 
+Filename: nucliadb/common/datamanagers/vectorsets.py
+Comment: 
+
 Filename: nucliadb/common/http_clients/__init__.py
 Comment: 
 
 Filename: nucliadb/common/http_clients/auth.py
 Comment: 
 
 Filename: nucliadb/common/http_clients/exceptions.py
@@ -450,14 +453,20 @@
 
 Filename: nucliadb/ingest/tests/unit/orm/__init__.py
 Comment: 
 
 Filename: nucliadb/ingest/tests/unit/orm/test_brain.py
 Comment: 
 
+Filename: nucliadb/ingest/tests/unit/orm/test_brain_vectors.py
+Comment: 
+
+Filename: nucliadb/ingest/tests/unit/orm/test_orm_utils.py
+Comment: 
+
 Filename: nucliadb/ingest/tests/unit/orm/test_processor.py
 Comment: 
 
 Filename: nucliadb/ingest/tests/unit/orm/test_resource.py
 Comment: 
 
 Filename: nucliadb/middleware/__init__.py
@@ -1335,26 +1344,26 @@
 
 Filename: nucliadb/writer/tus/storage.py
 Comment: 
 
 Filename: nucliadb/writer/tus/utils.py
 Comment: 
 
-Filename: nucliadb-3.0.3.post437.dist-info/METADATA
+Filename: nucliadb-3.0.3.post438.dist-info/METADATA
 Comment: 
 
-Filename: nucliadb-3.0.3.post437.dist-info/WHEEL
+Filename: nucliadb-3.0.3.post438.dist-info/WHEEL
 Comment: 
 
-Filename: nucliadb-3.0.3.post437.dist-info/entry_points.txt
+Filename: nucliadb-3.0.3.post438.dist-info/entry_points.txt
 Comment: 
 
-Filename: nucliadb-3.0.3.post437.dist-info/top_level.txt
+Filename: nucliadb-3.0.3.post438.dist-info/top_level.txt
 Comment: 
 
-Filename: nucliadb-3.0.3.post437.dist-info/zip-safe
+Filename: nucliadb-3.0.3.post438.dist-info/zip-safe
 Comment: 
 
-Filename: nucliadb-3.0.3.post437.dist-info/RECORD
+Filename: nucliadb-3.0.3.post438.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## nucliadb/learning_proxy.py

```diff
@@ -24,15 +24,15 @@
 from enum import Enum
 from typing import Any, Optional, Union
 
 import backoff
 import httpx
 from fastapi import Request, Response
 from fastapi.responses import StreamingResponse
-from pydantic import BaseModel
+from pydantic import BaseModel, Field, root_validator
 
 from nucliadb_telemetry import errors
 from nucliadb_utils.settings import is_onprem_nucliadb, nuclia_settings
 
 SERVICE_NAME = "nucliadb.learning_proxy"
 logger = logging.getLogger(SERVICE_NAME)
 
@@ -49,19 +49,43 @@
 
 
 class LearningService(str, Enum):
     CONFIG = "config"
     COLLECTOR = "collector-api"
 
 
+# Subset of learning configuration of nucliadb's interest. Look at
+# learning_config models for more fields
 class LearningConfiguration(BaseModel):
     semantic_model: str
+    # aka similarity function
     semantic_vector_similarity: str
+    # aka vector_dimension
     semantic_vector_size: Optional[int]
+    # aka min_score
     semantic_threshold: Optional[float]
+    # List of possible subdivisions of the matryoshka embeddings (if the model
+    # supports it)
+    semantic_matryoshka_dimensions: Optional[list[int]] = Field(
+        default=None, alias="semantic_matryoshka_dims"
+    )
+
+    @root_validator(pre=False)
+    def validate_matryoshka_and_vector_dimension_consistency(cls, values):
+        vector_size = values.get("semantic_vector_size")
+        matryoshka_dimensions = values.get("semantic_matryoshka_dimensions", []) or []
+        if (
+            len(matryoshka_dimensions) > 0
+            and vector_size is not None
+            and vector_size not in matryoshka_dimensions
+        ):
+            raise ValueError(
+                "Semantic vector size is inconsistent with matryoshka dimensions"
+            )
+        return values
 
 
 async def get_configuration(
     kbid: str,
 ) -> Optional[LearningConfiguration]:
     async with learning_config_client() as client:
         resp = await client.get(f"config/{kbid}")
@@ -300,14 +324,15 @@
 
     def get_config(self, *args: Any, **kwargs: Any):
         lconfig = LearningConfiguration(
             semantic_model="multilingual",
             semantic_vector_similarity="cosine",
             semantic_vector_size=None,
             semantic_threshold=None,
+            semantic_matryoshka_dims=[],
         )
         return self._response(content=lconfig.dict())
 
     async def request(  # type: ignore
         self,
         method: str,
         url: str,
```

## nucliadb/common/cluster/base.py

```diff
@@ -95,17 +95,21 @@
         return await self.reader.GetShard(req)  # type: ignore
 
     async def new_shard(
         self,
         kbid: str,
         similarity: utils_pb2.VectorSimilarity.ValueType,
         release_channel: utils_pb2.ReleaseChannel.ValueType,
+        normalize_vectors: bool,
     ) -> noderesources_pb2.ShardCreated:
         req = NewShardRequest(
-            kbid=kbid, similarity=similarity, release_channel=release_channel
+            kbid=kbid,
+            similarity=similarity,
+            release_channel=release_channel,
+            normalize_vectors=normalize_vectors,
         )
 
         resp = await self.writer.NewShard(req)  # type: ignore
         return resp
 
     async def list_shards(self) -> list[str]:
         shards = await self.writer.ListShards(noderesources_pb2.EmptyQuery())  # type: ignore
```

## nucliadb/common/cluster/manager.py

```diff
@@ -216,19 +216,21 @@
                     # available/responsive to create the required replicas
                     raise ExhaustedNodesError()
 
                 node = get_index_node(node_id)
                 if node is None:
                     logger.error(f"Node {node_id} is not found or not available")
                     continue
+                is_matryoshka = len(kb_shards.model.matryoshka_dimensions) > 0
                 try:
                     shard_created = await node.new_shard(
                         kbid,
                         similarity=kb_shards.similarity,
                         release_channel=kb_shards.release_channel,
+                        normalize_vectors=is_matryoshka,
                     )
                 except Exception as e:
                     errors.capture_exception(e)
                     logger.exception(f"Error creating new shard at {node}: {e}")
                     continue
 
                 replica = writer_pb2.ShardReplica(node=str(node_id))
```

## nucliadb/common/cluster/rollover.py

```diff
@@ -97,19 +97,21 @@
                         nodes = cluster_manager.sorted_primary_nodes()
                     node_id = nodes.pop(0)
 
                     node = get_index_node(node_id)
                     if node is None:
                         logger.error(f"Node {node_id} is not found or not available")
                         continue
+                    is_matryoshka = len(kb_shards.model.matryoshka_dimensions) > 0
                     try:
                         shard_created = await node.new_shard(
                             kbid,
                             similarity=kb_shards.similarity,
                             release_channel=kb_shards.release_channel,
+                            normalize_vectors=is_matryoshka,
                         )
                     except Exception as e:
                         errors.capture_exception(e)
                         logger.exception(f"Error creating new shard at {node}")
                         continue
 
                     replica = writer_pb2.ShardReplica(node=str(node_id))
```

## nucliadb/common/cluster/standalone/grpc_node_binding.py

```diff
@@ -48,19 +48,18 @@
     ResourceID,
 )
 from nucliadb_protos.noderesources_pb2 import Shard as NodeResourcesShard
 from nucliadb_protos.noderesources_pb2 import (
     ShardCreated,
     ShardId,
     ShardIds,
-    ShardMetadata,
     VectorSetID,
     VectorSetList,
 )
-from nucliadb_protos.nodewriter_pb2 import OpStatus
+from nucliadb_protos.nodewriter_pb2 import NewShardRequest, OpStatus
 
 from ..settings import settings
 
 logger = logging.getLogger(__name__)
 
 try:
     from nucliadb_node_binding import IndexNodeException  # type: ignore
@@ -283,15 +282,15 @@
         if NodeWriter is None:
             raise ImportError(
                 "NucliaDB index node bindings are not installed (writer not found)"
             )
         self.writer = NodeWriter()
         self.executor = ThreadPoolExecutor(settings.local_writer_threads)
 
-    async def NewShard(self, request: ShardMetadata) -> ShardCreated:
+    async def NewShard(self, request: NewShardRequest) -> ShardCreated:
         loop = asyncio.get_running_loop()
         resp = await loop.run_in_executor(
             self.executor, self.writer.new_shard, request.SerializeToString()
         )
         pb_bytes = bytes(resp)
         shard_created = ShardCreated()
         shard_created.ParseFromString(pb_bytes)
@@ -385,15 +384,15 @@
     "ParagraphSearch": (ParagraphSearchRequest, ParagraphSearchResponse),
     "RelationSearch": (RelationSearchRequest, RelationSearchResponse),
     "GetShard": (GetShardRequest, NodeResourcesShard),
     "Suggest": (SuggestRequest, SuggestResponse),
     "RelationEdges": (ShardId, EdgeList),
 }
 WRITER_METHODS = {
-    "NewShard": (ShardMetadata, ShardCreated),
+    "NewShard": (NewShardRequest, ShardCreated),
     "DeleteShard": (ShardId, ShardId),
     "ListShards": (EmptyQuery, ShardIds),
     "RemoveVectorSet": (VectorSetID, OpStatus),
     "AddVectorSet": (VectorSetID, OpStatus),
     "ListVectorSets": (ShardId, VectorSetList),
     "SetResource": (Resource, OpStatus),
     "RemoveResource": (ResourceID, OpStatus),
```

## nucliadb/common/datamanagers/kb.py

```diff
@@ -29,30 +29,57 @@
 KB_UUID = "/kbs/{kbid}/config"
 KB_SLUGS_BASE = "/kbslugs/"
 KB_SLUGS = KB_SLUGS_BASE + "{slug}"
 
 logger = logging.getLogger(__name__)
 
 
+async def get_kbs(
+    txn: Transaction, *, prefix: str = ""
+) -> AsyncIterator[tuple[str, str]]:
+    async for key in txn.keys(KB_SLUGS.format(slug=prefix), count=-1):
+        slug = key.replace(KB_SLUGS_BASE, "")
+        uuid = await get_kb_uuid(txn, slug=slug)
+        if uuid is None:
+            logger.error(f"KB with slug ({slug}) but without uuid?")
+            continue
+        yield (uuid, slug)
+
+
 async def exists_kb(txn: Transaction, *, kbid: str) -> bool:
     return await get_config(txn, kbid=kbid) is not None
 
 
+async def get_kb_uuid(txn: Transaction, *, slug: str) -> Optional[str]:
+    uuid = await txn.get(KB_SLUGS.format(slug=slug))
+    if uuid is not None:
+        return uuid.decode()
+    else:
+        return None
+
+
 async def get_config(
     txn: Transaction, *, kbid: str
 ) -> Optional[knowledgebox_pb2.KnowledgeBoxConfig]:
     key = KB_UUID.format(kbid=kbid)
     payload = await txn.get(key)
     if payload is None:
         return None
     response = knowledgebox_pb2.KnowledgeBoxConfig()
     response.ParseFromString(payload)
     return response
 
 
+async def set_config(
+    txn: Transaction, *, kbid: str, config: knowledgebox_pb2.KnowledgeBoxConfig
+):
+    key = KB_UUID.format(kbid=kbid)
+    await txn.set(key, config.SerializeToString())
+
+
 async def get_model_metadata(
     txn: Transaction, *, kbid: str
 ) -> knowledgebox_pb2.SemanticModelMetadata:
     shards_obj = await cluster.get_kb_shards(txn, kbid=kbid)
     if shards_obj is None:
         raise KnowledgeBoxNotFound(kbid)
     if shards_obj.HasField("model"):
@@ -61,25 +88,29 @@
         # B/c code for old KBs that do not have the `model` attribute set in the Shards object.
         # Cleanup this code after a migration is done unifying all fields under `model` (on-prem and cloud).
         return knowledgebox_pb2.SemanticModelMetadata(
             similarity_function=shards_obj.similarity
         )
 
 
-async def get_kb_uuid(txn: Transaction, *, slug: str) -> Optional[str]:
-    uuid = await txn.get(KB_SLUGS.format(slug=slug))
-    if uuid is not None:
-        return uuid.decode()
-    else:
-        return None
-
-
-async def get_kbs(
-    txn: Transaction, *, prefix: str = ""
-) -> AsyncIterator[tuple[str, str]]:
-    async for key in txn.keys(KB_SLUGS.format(slug=prefix), count=-1):
-        slug = key.replace(KB_SLUGS_BASE, "")
-        uuid = await get_kb_uuid(txn, slug=slug)
-        if uuid is None:
-            logger.error(f"KB with slug ({slug}) but without uuid?")
-            continue
-        yield (uuid, slug)
+async def get_matryoshka_vector_dimension(
+    txn: Transaction, *, kbid: str
+) -> Optional[int]:
+    """Return vector dimension for matryoshka models"""
+    model_metadata = await get_model_metadata(txn, kbid=kbid)
+    dimension = None
+    if (
+        len(model_metadata.matryoshka_dimensions) > 0
+        and model_metadata.vector_dimension
+    ):
+        if model_metadata.vector_dimension in model_metadata.matryoshka_dimensions:
+            dimension = model_metadata.vector_dimension
+        else:
+            logger.error(
+                "KB has an invalid matryoshka dimension!",
+                extra={
+                    "kbid": kbid,
+                    "vector_dimension": model_metadata.vector_dimension,
+                    "matryoshka_dimensions": model_metadata.matryoshka_dimensions,
+                },
+            )
+    return dimension
```

## nucliadb/ingest/orm/brain.py

```diff
@@ -51,14 +51,22 @@
 if TYPE_CHECKING:  # pragma: no cover
     StatusValue = Union[Metadata.Status.V, int]
 else:
     StatusValue = int
 
 FilePagePositions = dict[int, tuple[int, int]]
 
+FIELD_PARAGRAPH_ID = "{rid}/{field_id}/{paragraph_start}-{paragraph_end}"
+SPLIT_FIELD_PARAGRAPH_ID = (
+    "{rid}/{field_id}/{subfield_id}/{paragraph_start}-{paragraph_end}"
+)
+FIELD_VECTOR_ID = "{rid}/{field_id}/{index}/{vector_start}-{vector_end}"
+SPLIT_FIELD_VECTOR_ID = (
+    "{rid}/{field_id}/{subfield_id}/{index}/{vector_start}-{vector_end}"
+)
 
 METADATA_STATUS_PB_TYPE_TO_NAME_MAP = {
     Metadata.Status.ERROR: ResourceProcessingStatus.ERROR.name,
     Metadata.Status.PROCESSED: ResourceProcessingStatus.PROCESSED.name,
     Metadata.Status.PENDING: ResourceProcessingStatus.PENDING.name,
     Metadata.Status.BLOCKED: ResourceProcessingStatus.BLOCKED.name,
     Metadata.Status.EXPIRED: ResourceProcessingStatus.EXPIRED.name,
@@ -256,92 +264,119 @@
         for paragraph in metadata.metadata.paragraphs:
             self.brain.sentences_to_delete.append(
                 f"{self.rid}/{field_key}/{paragraph.start}-{paragraph.end}"
             )
 
     def apply_field_vectors(
         self,
-        field_key: str,
-        vo: VectorObject,
-        replace_field: bool,
-        replace_splits: list[str],
+        field_id: str,
+        vo: utils_pb2.VectorObject,
+        *,
+        replace_field: bool = False,
+        replace_splits: Optional[list[str]] = None,
+        matryoshka_vector_dimension: Optional[int] = None,
     ):
+        replace_splits = replace_splits or []
+
         for subfield, vectors in vo.split_vectors.items():
             # For each split of this field
-
             for index, vector in enumerate(vectors.vectors):
-                sparagraph = self.brain.paragraphs[field_key].paragraphs[
-                    f"{self.rid}/{field_key}/{subfield}/{vector.start_paragraph}-{vector.end_paragraph}"
-                ]
-                ssentence = sparagraph.sentences[
-                    f"{self.rid}/{field_key}/{subfield}/{index}/{vector.start}-{vector.end}"
-                ]
-
-                ssentence.ClearField("vector")  # clear first to prevent duplicates
-                ssentence.vector.extend(vector.vector)
-
-                # we only care about start/stop position of the paragraph for a given sentence here
-                # the key has the sentence position
-                ssentence.metadata.position.start = vector.start_paragraph
-                ssentence.metadata.position.end = vector.end_paragraph
-
-                ssentence.metadata.position.page_number = (
-                    sparagraph.metadata.position.page_number
-                )
-                ssentence.metadata.position.in_page = (
-                    sparagraph.metadata.position.in_page
-                )
-                ssentence.metadata.page_with_visual = (
-                    sparagraph.metadata.page_with_visual
-                )
-
-                ssentence.metadata.representation.file = (
-                    sparagraph.metadata.representation.file
+                paragraph_key = SPLIT_FIELD_PARAGRAPH_ID.format(
+                    rid=self.rid,
+                    field_id=field_id,
+                    subfield_id=subfield,
+                    paragraph_start=vector.start_paragraph,
+                    paragraph_end=vector.end_paragraph,
+                )
+                sentence_key = SPLIT_FIELD_VECTOR_ID.format(
+                    rid=self.rid,
+                    field_id=field_id,
+                    subfield_id=subfield,
+                    index=index,
+                    vector_start=vector.start,
+                    vector_end=vector.end,
                 )
-                ssentence.metadata.representation.is_a_table = (
-                    sparagraph.metadata.representation.is_a_table
+                self._apply_field_vector(
+                    field_id,
+                    paragraph_key,
+                    sentence_key,
+                    vector,
+                    matryoshka_vector_dimension=matryoshka_vector_dimension,
                 )
-                ssentence.metadata.position.index = sparagraph.metadata.position.index
 
         for index, vector in enumerate(vo.vectors.vectors):
-            para_key = f"{self.rid}/{field_key}/{vector.start_paragraph}-{vector.end_paragraph}"
-            paragraph = self.brain.paragraphs[field_key].paragraphs[para_key]
-            sent_key = f"{self.rid}/{field_key}/{index}/{vector.start}-{vector.end}"
-            sentence = paragraph.sentences[sent_key]
-
-            sentence.ClearField("vector")  # clear first to prevent duplicates
-            sentence.vector.extend(vector.vector)
-
-            # we only care about start/stop position of the paragraph for a given sentence here
-            # the key has the sentence position
-            sentence.metadata.position.start = vector.start_paragraph
-            sentence.metadata.position.end = vector.end_paragraph
-
-            # does it make sense to copy forward paragraph values here?
-            sentence.metadata.position.page_number = (
-                paragraph.metadata.position.page_number
+            paragraph_key = FIELD_PARAGRAPH_ID.format(
+                rid=self.rid,
+                field_id=field_id,
+                paragraph_start=vector.start_paragraph,
+                paragraph_end=vector.end_paragraph,
             )
-            sentence.metadata.position.in_page = paragraph.metadata.position.in_page
-
-            sentence.metadata.page_with_visual = paragraph.metadata.page_with_visual
-
-            sentence.metadata.representation.file = (
-                paragraph.metadata.representation.file
+            sentence_key = FIELD_VECTOR_ID.format(
+                rid=self.rid,
+                field_id=field_id,
+                index=index,
+                vector_start=vector.start,
+                vector_end=vector.end,
             )
-            sentence.metadata.representation.is_a_table = (
-                paragraph.metadata.representation.is_a_table
+            self._apply_field_vector(
+                field_id,
+                paragraph_key,
+                sentence_key,
+                vector,
+                matryoshka_vector_dimension=matryoshka_vector_dimension,
             )
 
-            sentence.metadata.position.index = paragraph.metadata.position.index
-
         for split in replace_splits:
-            self.brain.sentences_to_delete.append(f"{self.rid}/{field_key}/{split}")
+            self.brain.sentences_to_delete.append(f"{self.rid}/{field_id}/{split}")
 
         if replace_field:
-            self.brain.sentences_to_delete.append(f"{self.rid}/{field_key}")
+            self.brain.sentences_to_delete.append(f"{self.rid}/{field_id}")
+
+    def _apply_field_vector(
+        self,
+        field_id: str,
+        paragraph_key: str,
+        sentence_key: str,
+        vector: utils_pb2.Vector,
+        *,
+        matryoshka_vector_dimension: Optional[int] = None,
+    ):
+        paragraph_pb = self.brain.paragraphs[field_id].paragraphs[paragraph_key]
+        sentence_pb = paragraph_pb.sentences[sentence_key]
+
+        sentence_pb.ClearField("vector")  # clear first to prevent duplicates
+
+        # cut vectors if a specific dimension is specified
+        if matryoshka_vector_dimension is not None:
+            sentence_pb.vector.extend(vector.vector[:matryoshka_vector_dimension])
+        else:
+            sentence_pb.vector.extend(vector.vector)
+
+        # we only care about start/stop position of the paragraph for a given sentence here
+        # the key has the sentence position
+        sentence_pb.metadata.position.start = vector.start_paragraph
+        sentence_pb.metadata.position.end = vector.end_paragraph
+
+        # does it make sense to copy forward paragraph values here?
+        sentence_pb.metadata.position.page_number = (
+            paragraph_pb.metadata.position.page_number
+        )
+        sentence_pb.metadata.position.in_page = paragraph_pb.metadata.position.in_page
+
+        sentence_pb.metadata.page_with_visual = paragraph_pb.metadata.page_with_visual
+
+        sentence_pb.metadata.representation.file = (
+            paragraph_pb.metadata.representation.file
+        )
+
+        sentence_pb.metadata.representation.is_a_table = (
+            paragraph_pb.metadata.representation.is_a_table
+        )
+
+        sentence_pb.metadata.position.index = paragraph_pb.metadata.position.index
 
     def delete_vectors(self, field_key: str, vo: VectorObject):
         for subfield, vectors in vo.split_vectors.items():
             for vector in vectors.vectors:
                 self.brain.sentences_to_delete.append(
                     f"{self.rid}/{field_key}/{subfield}/{vector.start}-{vector.end}"
                 )
```

## nucliadb/ingest/orm/knowledgebox.py

```diff
@@ -26,15 +26,15 @@
 from nucliadb_protos.knowledgebox_pb2 import (
     KnowledgeBoxConfig,
     Labels,
     LabelSet,
     SemanticModelMetadata,
 )
 from nucliadb_protos.knowledgebox_pb2 import Synonyms as PBSynonyms
-from nucliadb_protos.knowledgebox_pb2 import VectorSet, VectorSets
+from nucliadb_protos.knowledgebox_pb2 import VectorSet
 from nucliadb_protos.resources_pb2 import Basic
 from nucliadb_protos.utils_pb2 import ReleaseChannel
 
 from nucliadb.common import datamanagers
 from nucliadb.common.cluster.base import AbstractIndexNode
 from nucliadb.common.cluster.exceptions import ShardNotFound, ShardsNotFound
 from nucliadb.common.cluster.manager import get_index_node
@@ -44,27 +44,30 @@
 from nucliadb.ingest.orm.exceptions import KnowledgeBoxConflict
 from nucliadb.ingest.orm.resource import (
     KB_RESOURCE_SLUG,
     KB_RESOURCE_SLUG_BASE,
     Resource,
 )
 from nucliadb.ingest.orm.synonyms import Synonyms
-from nucliadb.ingest.orm.utils import compute_paragraph_key, get_basic, set_basic
+from nucliadb.ingest.orm.utils import (
+    choose_matryoshka_dimension,
+    compute_paragraph_key,
+    get_basic,
+    set_basic,
+)
 from nucliadb.migrator.utils import get_latest_version
 from nucliadb_protos import writer_pb2
 from nucliadb_utils.storages.storage import Storage
 from nucliadb_utils.utilities import get_audit, get_storage
 
 # XXX Eventually all these keys should be moved to datamanagers.kb
 KB_RESOURCE = "/kbs/{kbid}/r/{uuid}"
 
 KB_KEYS = "/kbs/{kbid}/"
 
-KB_VECTORSET = "/kbs/{kbid}/vectorsets"
-
 KB_TO_DELETE_BASE = "/kbtodelete/"
 KB_TO_DELETE_STORAGE_BASE = "/storagetodelete/"
 
 KB_TO_DELETE = f"{KB_TO_DELETE_BASE}{{kbid}}"
 KB_TO_DELETE_STORAGE = f"{KB_TO_DELETE_STORAGE_BASE}{{kbid}}"
 
 
@@ -167,21 +170,32 @@
         if failed is False:
             kb_shards = writer_pb2.Shards()
             kb_shards.kbid = uuid
             # B/c with Shards.actual
             kb_shards.actual = -1
             # B/c with `Shards.similarity`, replaced by `model`
             kb_shards.similarity = semantic_model.similarity_function
+
+            # if this KB uses a matryoshka model, we can choose a different
+            # dimension
+            if len(semantic_model.matryoshka_dimensions) > 0:
+                semantic_model.vector_dimension = choose_matryoshka_dimension(
+                    semantic_model.matryoshka_dimensions  # type: ignore
+                )
             kb_shards.model.CopyFrom(semantic_model)
+
             kb_shards.release_channel = release_channel
 
             await datamanagers.cluster.update_kb_shards(
                 txn, kbid=uuid, shards=kb_shards
             )
 
+            # shard creation will alter this value on maindb, make sure nobody
+            # uses this variable anymore
+            del kb_shards
             shard_manager = get_shard_manager()
             try:
                 await shard_manager.create_shard_by_kbid(txn, uuid)
             except Exception as e:
                 await storage.delete_kb(uuid)
                 raise e
 
@@ -212,18 +226,15 @@
                 config.slug = slug
             else:
                 exist.slug = slug
 
         if config and exist != config:
             exist.MergeFrom(config)
 
-        await txn.set(
-            datamanagers.kb.KB_UUID.format(kbid=uuid),
-            exist.SerializeToString(),
-        )
+        await datamanagers.kb.set_config(txn, kbid=uuid, config=exist)
 
         return uuid
 
     async def iterate_kb_nodes(self) -> AsyncIterator[tuple[AbstractIndexNode, str]]:
         async with datamanagers.with_transaction() as txn:
             shards_obj = await datamanagers.cluster.get_kb_shards(txn, kbid=self.kbid)
             if shards_obj is None:
@@ -233,44 +244,37 @@
             for replica in shard.replicas:
                 node = get_index_node(replica.node)
                 if node is not None:
                     yield node, replica.shard.id
 
     # Vectorset
     async def get_vectorsets(self, response: writer_pb2.GetVectorSetsResponse):
-        vectorset_key = KB_VECTORSET.format(kbid=self.kbid)
-        payload = await self.txn.get(vectorset_key)
-        if payload is not None:
-            response.vectorsets.ParseFromString(payload)
-
-    async def del_vectorset(self, id: str):
-        vectorset_key = KB_VECTORSET.format(kbid=self.kbid)
-        payload = await self.txn.get(vectorset_key)
-        vts = VectorSets()
-        if payload is not None:
-            vts.ParseFromString(payload)
-        del vts.vectorsets[id]
-        # For each Node on the KB delete the vectorset
-        async for node, shard in self.iterate_kb_nodes():
-            await node.del_vectorset(shard, id)
-        payload = vts.SerializeToString()
-        await self.txn.set(vectorset_key, payload)
+        vectorsets = await datamanagers.vectorsets.get_vectorsets(
+            self.txn, kbid=self.kbid
+        )
+        if vectorsets is not None:
+            response.vectorsets.CopyFrom(vectorsets)
 
     async def set_vectorset(self, id: str, vs: VectorSet):
-        vectorset_key = KB_VECTORSET.format(kbid=self.kbid)
-        payload = await self.txn.get(vectorset_key)
-        vts = VectorSets()
-        if payload is not None:
-            vts.ParseFromString(payload)
-        vts.vectorsets[id].CopyFrom(vs)
         # For each Node on the KB add the vectorset
         async for node, shard in self.iterate_kb_nodes():
             await node.set_vectorset(shard, id, similarity=vs.similarity)
-        payload = vts.SerializeToString()
-        await self.txn.set(vectorset_key, payload)
+
+        await datamanagers.vectorsets.set_vectorset(
+            self.txn, kbid=self.kbid, vectorset_id=id, vs=vs
+        )
+
+    async def del_vectorset(self, id: str):
+        await datamanagers.vectorsets.del_vectorset(
+            self.txn, kbid=self.kbid, vectorset_id=id
+        )
+
+        # For each Node on the KB delete the vectorset
+        async for node, shard in self.iterate_kb_nodes():
+            await node.del_vectorset(shard, id)
 
     # Labels
     async def set_labelset(self, id: str, labelset: LabelSet):
         await datamanagers.labels.set_labelset(
             self.txn, kbid=self.kbid, labelset_id=id, labelset=labelset
         )
```

## nucliadb/ingest/orm/resource.py

```diff
@@ -58,14 +58,15 @@
     TrainParagraph,
     TrainResource,
     TrainSentence,
 )
 from nucliadb_protos.utils_pb2 import Relation as PBRelation
 from nucliadb_protos.writer_pb2 import BrokerMessage
 
+from nucliadb.common import datamanagers
 from nucliadb.common.maindb.driver import Transaction
 from nucliadb.ingest.fields.base import Field
 from nucliadb.ingest.fields.conversation import Conversation
 from nucliadb.ingest.fields.date import Datetime
 from nucliadb.ingest.fields.file import File
 from nucliadb.ingest.fields.generic import VALID_GENERIC_FIELDS, Generic
 from nucliadb.ingest.fields.keywordset import Keywordset
@@ -416,15 +417,22 @@
                     extracted_text=await field.get_extracted_text(),
                     basic_user_field_metadata=user_field_metadata,
                 )
 
             if self.disable_vectors is False:
                 vo = await field.get_vectors()
                 if vo is not None:
-                    brain.apply_field_vectors(field_key, vo, False, [])
+                    dimension = await datamanagers.kb.get_matryoshka_vector_dimension(
+                        self.txn, kbid=self.kb.kbid
+                    )
+                    brain.apply_field_vectors(
+                        field_key,
+                        vo,
+                        matryoshka_vector_dimension=dimension,
+                    )
         return brain
 
     async def generate_field_vectors(
         self,
         bm: BrokerMessage,
         type_id: FieldType.ValueType,
         field_id: str,
@@ -1008,23 +1016,27 @@
         (
             vo,
             replace_field_sentences,
             replace_splits_sentences,
         ) = await field_obj.set_vectors(field_vectors)
         field_key = self.generate_field_id(field_vectors.field)
         if vo is not None:
-            apply_field_vectors = partial(
+            dimension = await datamanagers.kb.get_matryoshka_vector_dimension(
+                self.txn, kbid=self.kb.kbid
+            )
+            apply_field_vectors_partial = partial(
                 self.indexer.apply_field_vectors,
                 field_key,
                 vo,
-                replace_field_sentences,
-                replace_splits_sentences,
+                replace_field=replace_field_sentences,
+                replace_splits=replace_splits_sentences,
+                matryoshka_vector_dimension=dimension,
             )
             loop = asyncio.get_running_loop()
-            await loop.run_in_executor(_executor, apply_field_vectors)
+            await loop.run_in_executor(_executor, apply_field_vectors_partial)
         else:
             raise AttributeError("VO not found on set")
 
     async def _apply_field_large_metadata(
         self, field_large_metadata: LargeComputedMetadataWrapper
     ):
         field_obj = await self.get_field(
```

## nucliadb/ingest/orm/utils.py

```diff
@@ -78,7 +78,29 @@
     writer.basic.metadata.status = Metadata.Status.PENDING
 
     toprocess.genericfield["title"] = Text(body=title, format=PushTextFormat.PLAIN)
 
 
 def compute_paragraph_key(rid: str, paragraph_key: str) -> str:
     return paragraph_key.replace("N_RID", rid)
+
+
+def choose_matryoshka_dimension(dimensions: list[int]) -> int:
+    """Given a list of matryoshka embedding available dimensions, choose one to
+    set the vector dimension.
+    """
+    if len(dimensions) == 0:
+        raise ValueError("Can't choose matryoshka dimension from an empty list")
+
+    threshold = 2000
+    previous = None
+    for dimension in sorted(dimensions):
+        if dimension > threshold:
+            break
+        previous = dimension
+
+    if dimension > threshold:
+        if previous is None:
+            return dimension
+        else:
+            return previous
+    return dimension
```

## nucliadb/ingest/service/writer.py

```diff
@@ -197,14 +197,16 @@
             else:
                 # We set an empty configuration so that learning chooses the default values.
                 config = {}
                 logger.warning(
                     "No learning configuration provided. Default will be used.",
                     extra={"kbid": kbid},
                 )
+            # NOTE: we rely on learning to return an updated configuration with
+            # matryoshka settings if they're available
             lconfig = await learning_proxy.set_configuration(kbid, config=config)
             lconfig_created = True
         else:
             logger.info("Learning configuration already exists", extra={"kbid": kbid})
         try:
             await self.proc.create_kb(
                 request.slug,
@@ -870,14 +872,16 @@
         model.vector_dimension = lconfig.semantic_vector_size
     else:
         logger.warning("Vector dimension not set!")
     if lconfig.semantic_threshold is not None:
         model.default_min_score = lconfig.semantic_threshold
     else:
         logger.warning("Default min score not set!")
+    if lconfig.semantic_matryoshka_dimensions is not None:
+        model.matryoshka_dimensions.extend(lconfig.semantic_matryoshka_dimensions)
     return model
 
 
 def parse_model_metadata_from_request(
     request: KnowledgeBoxNew,
 ) -> SemanticModelMetadata:
     model = SemanticModelMetadata()
@@ -888,14 +892,27 @@
         logger.warning(
             "Vector dimension not set. Will be detected automatically on the first vector set."
         )
     if request.HasField("default_min_score"):
         model.default_min_score = request.default_min_score
     else:
         logger.warning("Default min score not set!")
+
+    if len(request.matryoshka_dimensions) > 0:
+        if model.vector_dimension not in request.matryoshka_dimensions:
+            logger.warning(
+                "Vector dimensions is inconsistent with matryoshka dimensions! Ignoring them",
+                extra={
+                    "kbid": request.forceuuid,
+                    "kbslug": request.slug,
+                },
+            )
+        else:
+            model.matryoshka_dimensions.extend(request.matryoshka_dimensions)
+
     return model
 
 
 def get_release_channel(request: KnowledgeBoxNew) -> utils_pb2.ReleaseChannel.ValueType:
     """
     Set channel to Experimental if specified in the grpc request or if the requested
     slug has the experimental_kb feature enabled in stage environment.
```

## nucliadb/ingest/tests/unit/orm/test_resource.py

```diff
@@ -13,15 +13,15 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU Affero General Public License for more details.
 #
 # You should have received a copy of the GNU Affero General Public License
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
 #
-from unittest.mock import AsyncMock, MagicMock
+from unittest.mock import AsyncMock, MagicMock, Mock, patch
 
 import pytest
 from nucliadb_protos.resources_pb2 import (
     AllFieldIDs,
     Basic,
     CloudFile,
     FieldID,
@@ -37,14 +37,15 @@
     get_file_page_positions,
     get_text_field_mimetype,
     maybe_update_basic_icon,
     maybe_update_basic_summary,
     maybe_update_basic_thumbnail,
     update_basic_languages,
 )
+from nucliadb_protos import utils_pb2, writer_pb2
 
 
 @pytest.mark.asyncio
 async def test_get_file_page_positions():
     extracted_data = FileExtractedData()
     extracted_data.file_pages_previews.positions.extend(
         [PagePositions(start=0, end=10), PagePositions(start=11, end=20)]
@@ -269,7 +270,61 @@
         FieldID(field_type=FieldType.LINK, field="link"),
         FieldID(field_type=FieldType.FILE, field="file"),
         FieldID(field_type=FieldType.CONVERSATION, field="conversation"),
     ]
     resource.update_all_field_ids.call_args[1]["deleted"] == [
         FieldID(field_type=FieldType.LAYOUT, field="to_delete"),
     ]
+
+
+async def test_apply_extracted_vectors_matryoshka_embeddings(txn, storage, kb):
+    STORED_VECTOR_DIMENSION = 100
+    MATRYOSHKA_DIMENSION = 10
+
+    mock_field = AsyncMock()
+    vectors = utils_pb2.VectorObject(
+        vectors=utils_pb2.Vectors(
+            vectors=[
+                utils_pb2.Vector(
+                    start=0,
+                    end=10,
+                    start_paragraph=0,
+                    end_paragraph=10,
+                    vector=[1.0] * STORED_VECTOR_DIMENSION,
+                )
+            ]
+        )
+    )
+    mock_field.set_vectors.return_value = (vectors, False, [])
+
+    resource = Resource(txn, storage, kb, "matryoshka-rid")
+    with (
+        patch.object(resource, "has_field", Mock(return_value=True)),
+        patch.object(resource, "get_field", AsyncMock(return_value=mock_field)),
+        patch.object(resource, "generate_field_id", Mock(return_value="field_id")),
+        patch("nucliadb.ingest.orm.resource.datamanagers") as mock_datamanagers,
+        patch.object(
+            resource.indexer, "apply_field_vectors", AsyncMock()
+        ) as apply_field_vectors,
+    ):
+        mock_datamanagers.kb.get_matryoshka_vector_dimension = AsyncMock(
+            return_value=None
+        )
+        await resource._apply_extracted_vectors(
+            writer_pb2.ExtractedVectorsWrapper(vectors=vectors)
+        )
+        assert apply_field_vectors.call_count == 1
+        assert (
+            apply_field_vectors.call_args.kwargs["matryoshka_vector_dimension"] is None
+        )
+
+        mock_datamanagers.kb.get_matryoshka_vector_dimension = AsyncMock(
+            return_value=MATRYOSHKA_DIMENSION
+        )
+        await resource._apply_extracted_vectors(
+            writer_pb2.ExtractedVectorsWrapper(vectors=vectors)
+        )
+        assert apply_field_vectors.call_count == 2
+        assert (
+            apply_field_vectors.call_args.kwargs["matryoshka_vector_dimension"]
+            == MATRYOSHKA_DIMENSION
+        )
```

## nucliadb/search/search/query.py

```diff
@@ -401,43 +401,57 @@
         node_features.inc({"type": "vectors"})
 
         incomplete = False
         if self.vectorset is not None:
             request.vectorset = self.vectorset
             node_features.inc({"type": "vectorset"})
 
+        query_vector = None
         if self.user_vector is None:
             if self.query_endpoint_enabled:
                 try:
                     query_info = await self._get_query_information()
-                    if query_info and query_info.sentence:
-                        request.vector.extend(query_info.sentence.data)
-                    else:
-                        incomplete = True
                 except SendToPredictError as err:
                     logger.warning(
                         f"Errors on predict api trying to embedd query: {err}"
                     )
                     incomplete = True
                 except PredictVectorMissing:
                     logger.warning("Predict api returned an empty vector")
                     incomplete = True
+                else:
+                    if query_info and query_info.sentence:
+                        query_vector = query_info.sentence.data
+                    else:
+                        incomplete = True
             else:
                 try:
-                    request.vector.extend(await self._get_converted_vectors())
+                    query_vector = await self._get_converted_vectors()
                 except SendToPredictError as err:
                     logger.warning(
                         f"Errors on predict api trying to embedd query: {err}"
                     )
                     incomplete = True
                 except PredictVectorMissing:
                     logger.warning("Predict api returned an empty vector")
                     incomplete = True
         else:
-            request.vector.extend(self.user_vector)
+            query_vector = self.user_vector
+
+        if query_vector is not None:
+            async with datamanagers.with_transaction(read_only=True) as txn:
+                dimension = await datamanagers.kb.get_matryoshka_vector_dimension(
+                    txn, kbid=self.kbid
+                )
+            if dimension is not None:
+                # KB using a matryoshka embeddings model, cut the query vector
+                # accordingly
+                query_vector = query_vector[:dimension]
+            request.vector.extend(query_vector)
+
         return incomplete
 
     async def parse_relation_search(
         self, request: nodereader_pb2.SearchRequest
     ) -> list[str]:
         autofilters = []
         relations_search = SearchOptions.RELATIONS in self.features
```

## nucliadb/tests/utils/broker_messages/__init__.py

```diff
@@ -157,11 +157,15 @@
                 replace_if_exists(
                     self.bm.field_metadata, field.id, field.extracted.metadata
                 )
             if field.extracted.text is not None:
                 replace_if_exists(
                     self.bm.extracted_text, field.id, field.extracted.text
                 )
+            if field.extracted.vectors is not None:
+                replace_if_exists(
+                    self.bm.field_vectors, field.id, field.extracted.vectors
+                )
             if field.extracted.question_answers is not None:
                 replace_if_exists(
                     self.bm.question_answers, field.id, field.extracted.question_answers
                 )
```

## nucliadb/tests/utils/broker_messages/fields.py

```diff
@@ -19,27 +19,29 @@
 #
 
 import dataclasses
 from datetime import datetime
 from typing import Optional
 
 from nucliadb_protos import resources_pb2 as rpb
+from nucliadb_protos import utils_pb2
 
 from .helpers import labels_to_classifications
 
 
 @dataclasses.dataclass
 class FieldUser:
     metadata: Optional[rpb.UserFieldMetadata] = None
 
 
 @dataclasses.dataclass
 class FieldExtracted:
     metadata: Optional[rpb.FieldComputedMetadataWrapper] = None
     text: Optional[rpb.ExtractedTextWrapper] = None
+    vectors: Optional[rpb.ExtractedVectorsWrapper] = None
     question_answers: Optional[rpb.FieldQuestionAnswerWrapper] = None
 
 
 @dataclasses.dataclass
 class Field:
     id: rpb.FieldID
     user: FieldUser = dataclasses.field(default_factory=FieldUser)
@@ -47,14 +49,15 @@
 
 
 class FieldBuilder:
     def __init__(self, field: str, field_type: rpb.FieldType.ValueType):
         self._field_id = rpb.FieldID(field=field, field_type=field_type)
         self.__extracted_metadata: Optional[rpb.FieldComputedMetadataWrapper] = None
         self.__extracted_text: Optional[rpb.ExtractedTextWrapper] = None
+        self.__extracted_vectors: Optional[rpb.ExtractedVectorsWrapper] = None
         self.__user_metadata: Optional[rpb.UserFieldMetadata] = None
         self.__question_answers: Optional[rpb.FieldQuestionAnswerWrapper] = None
 
     @property
     def id(self) -> rpb.FieldID:
         return self._field_id
 
@@ -77,14 +80,20 @@
     @property
     def _extracted_text(self) -> rpb.ExtractedTextWrapper:
         if self.__extracted_text is None:
             self.__extracted_text = rpb.ExtractedTextWrapper(field=self._field_id)
         return self.__extracted_text
 
     @property
+    def _extracted_vectors(self) -> rpb.ExtractedVectorsWrapper:
+        if self.__extracted_vectors is None:
+            self.__extracted_vectors = rpb.ExtractedVectorsWrapper(field=self._field_id)
+        return self.__extracted_vectors
+
+    @property
     def _question_answers(self) -> rpb.FieldQuestionAnswerWrapper:
         if self.__question_answers is None:
             self.__question_answers = rpb.FieldQuestionAnswerWrapper(
                 field=self._field_id
             )
         return self.__question_answers
 
@@ -101,14 +110,18 @@
             field.extracted.metadata = rpb.FieldComputedMetadataWrapper()
             field.extracted.metadata.CopyFrom(self.__extracted_metadata)
 
         if self.__extracted_text is not None:
             field.extracted.text = rpb.ExtractedTextWrapper()
             field.extracted.text.CopyFrom(self.__extracted_text)
 
+        if self.__extracted_vectors is not None:
+            field.extracted.vectors = rpb.ExtractedVectorsWrapper()
+            field.extracted.vectors.CopyFrom(self.__extracted_vectors)
+
         if self.__question_answers is not None:
             field.extracted.question_answers = rpb.FieldQuestionAnswerWrapper()
             field.extracted.question_answers.CopyFrom(self.__question_answers)
 
         if self.__user_metadata is not None:
             field.user.metadata = rpb.UserFieldMetadata()
             field.user.metadata.CopyFrom(self.__user_metadata)
@@ -120,14 +133,17 @@
         self._extracted_metadata.metadata.metadata.classifications.extend(
             classifications
         )
 
     def with_extracted_text(self, text: str):
         self._extracted_text.body.text = text
 
+    def with_extracted_vectors(self, vectors: list[utils_pb2.Vector]):
+        self._extracted_vectors.vectors.vectors.vectors.extend(vectors)
+
     def with_extracted_paragraph_metadata(self, paragraph: rpb.Paragraph):
         self._extracted_metadata.metadata.metadata.paragraphs.append(paragraph)
 
     def with_user_entity(self, klass: str, name: str, *, start: int, end: int):
         entity = rpb.TokenSplit(
             klass=klass,
             token=name,
```

## Comparing `nucliadb-3.0.3.post437.dist-info/METADATA` & `nucliadb-3.0.3.post438.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nucliadb
-Version: 3.0.3.post437
+Version: 3.0.3.post438
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
-Requires-Dist: nucliadb-telemetry[all] >=3.0.3.post437
-Requires-Dist: nucliadb-utils[cache,fastapi,storages] >=3.0.3.post437
-Requires-Dist: nucliadb-protos >=3.0.3.post437
-Requires-Dist: nucliadb-models >=3.0.3.post437
+Requires-Dist: nucliadb-telemetry[all] >=3.0.3.post438
+Requires-Dist: nucliadb-utils[cache,fastapi,storages] >=3.0.3.post438
+Requires-Dist: nucliadb-protos >=3.0.3.post438
+Requires-Dist: nucliadb-models >=3.0.3.post438
 Requires-Dist: nucliadb-admin-assets >=1.0.0.post1224
 Requires-Dist: nucliadb-node-binding >=2.26.0
 Requires-Dist: uvicorn <0.19.0
 Requires-Dist: pydantic-argparse
 Requires-Dist: aiohttp >=3.9.3
 Requires-Dist: lru-dict >=1.1.7
 Requires-Dist: backoff
```

## Comparing `nucliadb-3.0.3.post437.dist-info/entry_points.txt` & `nucliadb-3.0.3.post438.dist-info/entry_points.txt`

 * *Files identical despite different names*

## Comparing `nucliadb-3.0.3.post437.dist-info/RECORD` & `nucliadb-3.0.3.post438.dist-info/RECORD`

 * *Files 1% similar despite different names*

```diff
@@ -14,54 +14,55 @@
 migrations/0015_targeted_rollover.py,sha256=7C9XM8wg-bpkNyFh0xJuaGzOcE2WqU1BfqtInKAjTkw,1462
 migrations/0016_upgrade_to_paragraphs_v2.py,sha256=pOZUwTDfGoLjcSSKiWaN6FUvMDN95XNCBoux3u0dsmQ,2506
 migrations/0017_multiple_writable_shards.py,sha256=NY38wFVxSDXglkZE6DRnuN1DG_1kyZXr2j37C8VhyA0,2100
 migrations/0018_purge_orphan_kbslugs.py,sha256=3x5OsMb-JnP9y8_-ztYugk1RiXbOuthTFB-8I1XX3bk,2264
 migrations/__init__.py,sha256=cp15ZcFnHvpcu_5-aK2A4uUyvuZVV_MJn4bIXMa20ks,835
 nucliadb/__init__.py,sha256=_abCmDJ_0ku483Os4UAjPX7Nywm39cQgAV_DiyjsKeQ,891
 nucliadb/health.py,sha256=zPwd3CAFJf9owhbadtyGLvHekOjX9ykvxLYWYxnD5eo,3733
-nucliadb/learning_proxy.py,sha256=RVuBDsI2zbU53x2fnl965aZF8FV3GhI5J7b8TfX6mN4,10590
+nucliadb/learning_proxy.py,sha256=6r_fFgE662yEFgNpgGNxc3KTfFiR78yiEN95Qir6ctI,11626
 nucliadb/metrics_exporter.py,sha256=PummIqtRLdpcONPIpRKBj_jGYnX7B9XZ2IO048bu2pM,4806
 nucliadb/openapi.py,sha256=wDiw0dVEvTpJvbatkJ0JZLkKm9RItZT5PWRHjqRfqTA,2272
 nucliadb/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 nucliadb/common/__init__.py,sha256=cp15ZcFnHvpcu_5-aK2A4uUyvuZVV_MJn4bIXMa20ks,835
 nucliadb/common/locking.py,sha256=_168BClwNyXVentC7mk4_on0qof5G2y5VgTpOWvzJGk,4905
 nucliadb/common/cluster/__init__.py,sha256=cp15ZcFnHvpcu_5-aK2A4uUyvuZVV_MJn4bIXMa20ks,835
-nucliadb/common/cluster/base.py,sha256=cmo1kDig2u3k-h5EBYNtuw-xusPgYgMoznO0DEoj5tg,4983
+nucliadb/common/cluster/base.py,sha256=JNb-NhRBd7eLMpaiPsypxk0x1YUo2GIyfubhnjDuD6Y,5090
 nucliadb/common/cluster/exceptions.py,sha256=V3c_fgH00GyJ-a5CaGLhwTuhwhUNR9YAGvS5jaRuc_Y,1495
 nucliadb/common/cluster/grpc_node_dummy.py,sha256=pBO675j-BptC5U_8Wi6uB19QSQTixgJP2MTzr8v6_Wk,3658
 nucliadb/common/cluster/index_node.py,sha256=WafWLzU1l7EHj1VyG0w6qi2BW_Izc8rFze6ZWbYvT9g,3429
-nucliadb/common/cluster/manager.py,sha256=zBbA-d763fl0VAAqi0lDWYEV6r3HIpY4UcCT5HWM2cU,21095
+nucliadb/common/cluster/manager.py,sha256=JIb5jpfmBSjFPXxe4YQqWrQW3TD8iY-0a2HrqIGbThw,21231
 nucliadb/common/cluster/rebalance.py,sha256=RC5Q9Uic0__QHeukd2ANlWyd6AYKBzRm3FXhvwcwxCo,8490
-nucliadb/common/cluster/rollover.py,sha256=ybPdme4ofaHKQuGW4D_p_TyVJgnFy_HhI5bq78gubjA,19449
+nucliadb/common/cluster/rollover.py,sha256=pvQbL-xGtEcSlLGsQnMDFj1Jr7_g7IMkj6ZQkH2a4Vo,19593
 nucliadb/common/cluster/settings.py,sha256=snENrNo9voc1TZ6uyBnuSHGoS2Ocga_Kn-W33nOlO-c,2713
 nucliadb/common/cluster/utils.py,sha256=Hqhm3OwZ14GWaF3UiAGDXgfxjjpgtQz1xoSBxC2Bd3Q,5494
 nucliadb/common/cluster/discovery/__init__.py,sha256=cp15ZcFnHvpcu_5-aK2A4uUyvuZVV_MJn4bIXMa20ks,835
 nucliadb/common/cluster/discovery/base.py,sha256=P0JwzRYqOKxOzV_K_glwPizDGFGBY-l8G7TeTId9LIA,6553
 nucliadb/common/cluster/discovery/k8s.py,sha256=pvuyIYuWWDpRz7Bv8D_LOKFMz0w8sucpJvDshmRNpe0,12518
 nucliadb/common/cluster/discovery/manual.py,sha256=7wdcyfrR8oii2hP3AzOTAaUAGwkQu7eOj9Xl7Q49IUQ,1957
 nucliadb/common/cluster/discovery/single.py,sha256=2BhcencPKQQIfVitmTPJZm3TkBHyY9ZMcr-Clh8k2tM,1737
 nucliadb/common/cluster/discovery/types.py,sha256=vs-K790rofjZ4FWYaMkgjkZZqMvIvd_0eSw3shuiLwA,1139
 nucliadb/common/cluster/discovery/utils.py,sha256=A3DhpM3ExTSxtIo0Wh8ZIFARq2GW2OM1GPX967gyRbk,2548
 nucliadb/common/cluster/standalone/__init__.py,sha256=itSI7dtTwFP55YMX4iK7JzdMHS5CQVUiB1XzQu4UBh8,833
-nucliadb/common/cluster/standalone/grpc_node_binding.py,sha256=LwbL1VwBzv_r3TqtKN5EHetpIUN59BguXJw2BBSqN7E,13705
+nucliadb/common/cluster/standalone/grpc_node_binding.py,sha256=52U0TCREO4CcCOC9ctrxmx6xno2M8t01QbI8MIcw3Qc,13707
 nucliadb/common/cluster/standalone/index_node.py,sha256=aKpkAEosp9qbd-77fYgE1AAnDc-6ER05cA_HJtkeBT0,4683
 nucliadb/common/cluster/standalone/service.py,sha256=tJI5Gc-cu4uprC84bcLQr4CMW0hBS9T2YX_Ex6zeyuI,3444
 nucliadb/common/cluster/standalone/utils.py,sha256=S5aSK18CVLCd7YR4CImEK9Skz7d_xSH63eQkHOYdHK8,3386
 nucliadb/common/context/__init__.py,sha256=DaiW_oYiAprzYWaabIJdQ3kh-b99fleHKC7Xg8CaqD0,3498
 nucliadb/common/context/fastapi.py,sha256=qsxQ8s5dl67uCATrwdJCXA9JDfVn3DqxgsiWf6MUJhE,1628
 nucliadb/common/datamanagers/__init__.py,sha256=nr-HLFp_3u3SZeVYMvi5ew_VGGLYNO1cQWWAXfB9b1Y,1813
 nucliadb/common/datamanagers/cluster.py,sha256=Rc_gWufL-Fx3zQ7WlgCFYBPQD9fPjUvHkyW0QK6hBSg,1451
 nucliadb/common/datamanagers/entities.py,sha256=vQe_xdyqqsII0wmqKWp1yxVTFmB67Tc6bnVxezRUVK0,5383
 nucliadb/common/datamanagers/exceptions.py,sha256=Atz_PP_GGq4jgJaWcAkcRbHBoBaGcC9yJvFteylKtTE,883
-nucliadb/common/datamanagers/kb.py,sha256=gFSQ5WSLm6mCy0rDLvUJbSmDd8Vei2OZqyH-C4PbBRE,2940
+nucliadb/common/datamanagers/kb.py,sha256=zkG3lVbGFFLtjcTlJvJDtTY6S55xdty1nSlwI4xDEQ4,3994
 nucliadb/common/datamanagers/labels.py,sha256=2pN8RrFNTXLitDo44CS3AApjCjbv-2ALkqjwHVR_Mb0,5389
 nucliadb/common/datamanagers/processing.py,sha256=gdCHGzF2LiHOapsg4oaYFYNxACwaCbN1z3kw7iHTuNc,1599
 nucliadb/common/datamanagers/resources.py,sha256=HapnkdZznvxzZMUVLpMhY0sM8578hOq1WbrjVSNuNHg,7637
 nucliadb/common/datamanagers/rollover.py,sha256=gyF5EJ_-R3lunnXfj4JD7rdhh1l8lEWgwgRxeZHMpsw,5633
 nucliadb/common/datamanagers/utils.py,sha256=_Yp_s3zCeWCqtqSSO_PY7xgk2Vo0W9mVqQst2Mj2eFU,1681
+nucliadb/common/datamanagers/vectorsets.py,sha256=4CZkeQ0s0ITcneBSCGtGojdjqqaGu9ykPisYmEYv8IM,2055
 nucliadb/common/http_clients/__init__.py,sha256=cp15ZcFnHvpcu_5-aK2A4uUyvuZVV_MJn4bIXMa20ks,835
 nucliadb/common/http_clients/auth.py,sha256=9A1k-H121W3lAFRl_XxGizcxUw_qw1STDZqJOC2Kpyw,2146
 nucliadb/common/http_clients/exceptions.py,sha256=47Y8OjkaGV_F18G07FpJhOzgWKUIexhlILyuVtICz8s,1100
 nucliadb/common/http_clients/processing.py,sha256=-J5Lxmlk4coboOWvYQ4gc88AIrvHzSV9bzVsedmslCQ,7155
 nucliadb/common/http_clients/pypi.py,sha256=VHIUjwJEJVntVUo_FRoXIo8sLmluy7sa9-iXSITcrMY,1540
 nucliadb/common/http_clients/utils.py,sha256=b7FCaOSf21UVE9OqDhBpWetxP2nguV_gKwBBb9dYifI,1551
 nucliadb/common/maindb/__init__.py,sha256=cp15ZcFnHvpcu_5-aK2A4uUyvuZVV_MJn4bIXMa20ks,835
@@ -105,27 +106,27 @@
 nucliadb/ingest/fields/file.py,sha256=RtLlnDuT3bueO7V0gnm_i_P1lUCG9l6CZFky0fFCCgg,5159
 nucliadb/ingest/fields/generic.py,sha256=elgtqv15aJUq3zY7X_g0bli_2BpcwPArVvzhe54Y4Ig,1547
 nucliadb/ingest/fields/keywordset.py,sha256=mLpitqGiSH3IilHCEo2ZGg3laTOMoZ5qc_DVbV3UECA,1235
 nucliadb/ingest/fields/layout.py,sha256=clgBVGWArtkAEawDqCAu_hB9gVu5c6UT1Cf_5yrw47s,2250
 nucliadb/ingest/fields/link.py,sha256=6D1jlwX1ImU3RL1dVawXm2ChoB_s1_h5DOVGyW4q37M,4084
 nucliadb/ingest/fields/text.py,sha256=qMMH76gN--Ag1fPZ1I5G9ZPAi4U0i9jbqlrpYc3cMxg,1319
 nucliadb/ingest/orm/__init__.py,sha256=cp15ZcFnHvpcu_5-aK2A4uUyvuZVV_MJn4bIXMa20ks,835
-nucliadb/ingest/orm/brain.py,sha256=Ox5IxnQsJcJzi5B8Q35zmyT2W-htFSUjX5C1PaKZH4E,27582
+nucliadb/ingest/orm/brain.py,sha256=Hq8c0TpHlJ2rT5oig3QX3xmSQZiB8YFURws5xj3-iuk,28367
 nucliadb/ingest/orm/entities.py,sha256=q027LfocE-KIqRNC1ZOSrrvt6x9NGrB25TZsOe0SyVk,15758
 nucliadb/ingest/orm/exceptions.py,sha256=GKr20V5xLv-WHBBHhr8lBChpW5oa9k18Xuiw-dIF9DM,1279
-nucliadb/ingest/orm/knowledgebox.py,sha256=XJPAUNiV1lai20RQ4CF9JEIcuPuuSCUADSijNNeHs1o,18747
+nucliadb/ingest/orm/knowledgebox.py,sha256=28LLX4rhMVL7mqIAxSmRhTGSN_6rZSJu_Ct42Ut7gEY,18731
 nucliadb/ingest/orm/metrics.py,sha256=OkwMSPKLZcKba0ZTwtTiIxwBgaLMX5ydhGieKvi2y7E,1096
-nucliadb/ingest/orm/resource.py,sha256=AwWlzVrXYxZMnvn9ECA9KFMI5etFoEoFCIjkHaNpH58,60085
+nucliadb/ingest/orm/resource.py,sha256=TWjYAqRRaZamT1ssWDGrQMmrxvu5R2X07zL13i7XxqY,60647
 nucliadb/ingest/orm/synonyms.py,sha256=tyOEGPfuJwhM5iYm4uNPjc2E8oWPk70DzZeuxVZ5alQ,1739
-nucliadb/ingest/orm/utils.py,sha256=VMLhujH4kihWiSvCPCiGAvGxqTZBh8RGn_9CZUUIELI,3074
+nucliadb/ingest/orm/utils.py,sha256=0GwmyP0CqskAUqKbp0LAInYE64kt8locVqZ0HB04zlw,3683
 nucliadb/ingest/orm/processor/__init__.py,sha256=rdd6Eec4C3yhQYcrHLgwngLk3amMpih5h3N_8hYjqNk,26460
 nucliadb/ingest/orm/processor/sequence_manager.py,sha256=Mc9SA_NfzxTwovD5yGiAcdmen4pa-QNdsYcONIWeZPc,1690
 nucliadb/ingest/service/__init__.py,sha256=C_lkkjoHm0hDT2fZjEN4mpwXtU4bWthB-vM5-28-MBM,2057
 nucliadb/ingest/service/exceptions.py,sha256=cp15ZcFnHvpcu_5-aK2A4uUyvuZVV_MJn4bIXMa20ks,835
-nucliadb/ingest/service/writer.py,sha256=jHWygnQaNqg_IbagM_ZAgsoEfaaI9jEBXh39AWuaknY,36594
+nucliadb/ingest/service/writer.py,sha256=xGsk2noVqKYnD8p_LYpzzand1tBiQKe13EJhfoMRHKc,37355
 nucliadb/ingest/tests/__init__.py,sha256=cp15ZcFnHvpcu_5-aK2A4uUyvuZVV_MJn4bIXMa20ks,835
 nucliadb/ingest/tests/conftest.py,sha256=yTepuxodMXl5vEMTzFfgos9wdRnYfxPffZQDYm3Ej-E,1157
 nucliadb/ingest/tests/fixtures.py,sha256=CeVkscwCn14PqPdfbjfR9u3FYgDKe_6kZG8nL75qjCU,24068
 nucliadb/ingest/tests/vectors.py,sha256=CcNKx-E8LPpyvRyljbmb-Tn_wST9Juw2CBoogWrKiTk,62843
 nucliadb/ingest/tests/integration/__init__.py,sha256=cp15ZcFnHvpcu_5-aK2A4uUyvuZVV_MJn4bIXMa20ks,835
 nucliadb/ingest/tests/integration/consumer/__init__.py,sha256=itSI7dtTwFP55YMX4iK7JzdMHS5CQVUiB1XzQu4UBh8,833
 nucliadb/ingest/tests/integration/consumer/test_auditing.py,sha256=5VYFGUeaxd18mLtUfHCUPu9c1iAShNHNM5X_CSkIFSs,2549
@@ -146,16 +147,18 @@
 nucliadb/ingest/tests/unit/consumer/test_auditing.py,sha256=9bFYLwx-LBfFjfOreILffkyyizH42rh8J_9Mn3J8dvo,3981
 nucliadb/ingest/tests/unit/consumer/test_consumer.py,sha256=UWdQXCDoUpayaVg8IJISGYyU4xG1Di8vhS7V2agFlms,2472
 nucliadb/ingest/tests/unit/consumer/test_pull.py,sha256=j0VQLhdmJsJxqvzU25zYwKvfIJbi7vuafzeYQGQxOAY,2063
 nucliadb/ingest/tests/unit/consumer/test_shard_creator.py,sha256=jvHiNHrKU0vPs06B2894kwKF92CBNh22jsUUux9J7lw,4075
 nucliadb/ingest/tests/unit/consumer/test_utils.py,sha256=sanGAv21LfsnmqqjbprnAY22n-MSvm-n34bzj0Hj4h0,1934
 nucliadb/ingest/tests/unit/orm/__init__.py,sha256=cp15ZcFnHvpcu_5-aK2A4uUyvuZVV_MJn4bIXMa20ks,835
 nucliadb/ingest/tests/unit/orm/test_brain.py,sha256=MSSG0OdWaYeYhBpvKlqGHGdTiV5xLaXwniFdqC9OWDc,9876
+nucliadb/ingest/tests/unit/orm/test_brain_vectors.py,sha256=HNi332BgnFQ_wx5Mw3AYv9mhSsRmj9F04VNZb6Nu3lE,2435
+nucliadb/ingest/tests/unit/orm/test_orm_utils.py,sha256=wpQ3KX2pt0uIM_eLjlBKWO5900h-jc7i7JR4HNGrmRE,1174
 nucliadb/ingest/tests/unit/orm/test_processor.py,sha256=OHTsPGlficyRxQf8QT_8N5mX3JfgSHpyo8S-VfvZcTI,4045
-nucliadb/ingest/tests/unit/orm/test_resource.py,sha256=a3DBgYyV_mpfm2XAZhV9HkTG0z4wG_lm3ZTtrXpJHNY,8965
+nucliadb/ingest/tests/unit/orm/test_resource.py,sha256=TR6-TPFy_TM-IqxJ6vl4qi35VP8cFlZgFn1NAPWrTlA,11005
 nucliadb/middleware/__init__.py,sha256=knHBrVD30vfAWxn1RdRYEloSpIqakY3Ch9-NQzqKxk4,2216
 nucliadb/middleware/transaction.py,sha256=BjLGePAUnGAtpYIfv9lXKRFI1fB6lrseVeYzY-ckiFY,3912
 nucliadb/migrator/__init__.py,sha256=cp15ZcFnHvpcu_5-aK2A4uUyvuZVV_MJn4bIXMa20ks,835
 nucliadb/migrator/command.py,sha256=MgDruKOYpLuUMoO8aAE86vPflfOt7pAbW8QZQSZTFQQ,2119
 nucliadb/migrator/context.py,sha256=3h6M_AG2HFjTYtQC2XDmKps7wywdUduT1RM3C30S_S0,1334
 nucliadb/migrator/datamanager.py,sha256=5CLt1_fA3hXCBwUr1ltfmN3o69AzbweyiP42FkOqqV0,5104
 nucliadb/migrator/exceptions.py,sha256=jTj3YhKmFwUyjjgoKUNoCAiGrpEbB64X1Um212nSNQ8,889
@@ -225,15 +228,15 @@
 nucliadb/search/search/filters.py,sha256=HpTpaDjKmUZWkp5xFFqKHz3TYdKEVBk4jWb2ssIYa5g,6513
 nucliadb/search/search/find.py,sha256=cnWh2yC6Zq0XNG0c0ciycFr1APobbCF1Fye4fatxSIc,4646
 nucliadb/search/search/find_merge.py,sha256=vhq14MFE7N9-9SNlg66LNUr6YAhR9cW22oDpmjvQhL0,17152
 nucliadb/search/search/merge.py,sha256=afHYOJhBvqmiLbpayLw08ODDk4Upkq8jssqocJvYx3E,21118
 nucliadb/search/search/metrics.py,sha256=4xQm4Q0_-R1bgMtnrbm-YaClEFR8HE6wDk9lunCrhjo,1130
 nucliadb/search/search/paragraphs.py,sha256=8TTii45JvQ7SXsV9Z9ipt5QpYk7ux6PnlOkjKPfYz4A,8698
 nucliadb/search/search/predict_proxy.py,sha256=aOq1AzXkUdHtEmXsec07ffuMKGjlMu-NaUxb_IKme6U,3026
-nucliadb/search/search/query.py,sha256=NHQvCeAh7hdhaBWUfl2AVu0IFCKdsXSUpZhKJF5dB3U,32297
+nucliadb/search/search/query.py,sha256=HR5q_LbbXUKW6gtBPtjDYHBaNe6otRzKAP1ndGDcnlw,32831
 nucliadb/search/search/shards.py,sha256=CiQHBPR-_IjtfaC_897adddH4sRSxgfTEURuFpoMLQs,3149
 nucliadb/search/search/summarize.py,sha256=bjncFFBv1R9g4OyhQSlGHFq5cJ8UvR8KrMgeKc-1AMU,5101
 nucliadb/search/search/utils.py,sha256=Gzjr9rFdwRfOgyDzX1Slz8DbcXLvavo0124S8II9omw,2438
 nucliadb/search/search/chat/__init__.py,sha256=cp15ZcFnHvpcu_5-aK2A4uUyvuZVV_MJn4bIXMa20ks,835
 nucliadb/search/search/chat/images.py,sha256=AjPgCJaCzu19ruUJcEVaG_bEUmqzB65EH0mduMbkzAE,2058
 nucliadb/search/search/chat/prompt.py,sha256=W98mZrhrscjkxVJ02OM7veAQ1fjMrNDSZ1CUSaECCCk,20793
 nucliadb/search/search/chat/query.py,sha256=4wV6nwzNVA4skiUVM0ggBgdRR7BjYHZ801b87WAuIgI,15347
@@ -341,16 +344,16 @@
 nucliadb/tests/unit/tasks/conftest.py,sha256=txsUKEZ9_T8T2t1mdpQU91FRBrm5XA1PQfyii8jrdXo,1375
 nucliadb/tests/unit/tasks/test_consumer.py,sha256=iYAEIcyjRE4RMA2882K73RkBjDY_nhkJPaibyzgeWH8,2714
 nucliadb/tests/unit/tasks/test_producer.py,sha256=7HzGtZ4kzkL9JPnS7q-BVX2JelamG-ryKZkTjYCYNO0,3189
 nucliadb/tests/unit/tasks/test_tasks.py,sha256=l1iVwmGb_gJ25sT-97Awg1w976Jrp72C85CeSPF2xdU,1827
 nucliadb/tests/utils/__init__.py,sha256=9PJi9kuj_ABbacVFXEUlZe0n5BtjaWXZmKEv1LRo3-8,2507
 nucliadb/tests/utils/aiohttp_session.py,sha256=iU6_EhebdcJ1GGcHHX-r7lFh-uSXGCTkFkWwyb6zNaY,1797
 nucliadb/tests/utils/entities.py,sha256=IPTHEsYY6tryoxZhpz3dpkklw0AQm4_shk0Osj8Bnwk,2533
-nucliadb/tests/utils/broker_messages/__init__.py,sha256=0aPIe5_fb9dX-RkHu5xE5athJ2W-8NXxaAkGoEK1YUY,6145
-nucliadb/tests/utils/broker_messages/fields.py,sha256=v8WxIdCJleCOba_QgGZYZm1C2RArQbkXhR431OlrZ8M,6795
+nucliadb/tests/utils/broker_messages/__init__.py,sha256=O9swTEVkn4PKu0rJyPZkYnHYLVlL6UczSgMMFk4jSGM,6327
+nucliadb/tests/utils/broker_messages/fields.py,sha256=2eK3AMb0ahynILRAEVmNy_7aLEoxC5bGuE7gpJir4lY,7557
 nucliadb/tests/utils/broker_messages/helpers.py,sha256=RGJ2YZ34ZU7ENsCUPVpFDkNEpxv9v45FYIvPVePML7o,1196
 nucliadb/train/__init__.py,sha256=qdZ6DeuwED8iIl32NVyDYWTy544FyHCZUQnQGnms604,1325
 nucliadb/train/app.py,sha256=3AucXVUiDFueskmw85nO22fu9YjRyZIU1yhGlh0jVOE,3530
 nucliadb/train/generator.py,sha256=zmoffpYvc6u3gk6cPXKcKPf0KKpMibu6xWnwDs143bQ,3800
 nucliadb/train/lifecycle.py,sha256=ZLqCl_IjFimon9pl3OJyF2UM4Jky_xsHuqilnrJj1as,1698
 nucliadb/train/models.py,sha256=BmgmMjDsu_1Ih5JDAqo6whhume90q0ASJcDP9dkMQm8,1198
 nucliadb/train/nodes.py,sha256=IIO0ub7yn47pAooVGpTBvk_bxdF0Rn9G21ZnbwR_bww,5706
@@ -441,13 +444,13 @@
 nucliadb/writer/tus/exceptions.py,sha256=CmxYKnHXpXug25DYV4SpVAU47SGD-NVBd7pNTRbWHyk,2186
 nucliadb/writer/tus/gcs.py,sha256=WykJZicWKRYkVB5_Fkb_1cVLovAk86IVkEn1VgEDufc,14527
 nucliadb/writer/tus/local.py,sha256=lIOoGaylnsxPBYGskcmKSHv7MsvwIYFS4soDLey_KSs,5849
 nucliadb/writer/tus/pg.py,sha256=JUK_xKsyNcKAvWOch8gUMTc_e1evI_3aC6-Y5gMk2jw,4367
 nucliadb/writer/tus/s3.py,sha256=a9mfPtjBW3QaTYY2r6P7u_Y13V6mBefZjWgV4juZzgE,9069
 nucliadb/writer/tus/storage.py,sha256=8iBOjWIcY6PawQq_rmSiBKi0Gl6J6Q5ad6L-9nLCcJ4,4734
 nucliadb/writer/tus/utils.py,sha256=MSdVbRsRSZVdkaum69_0wku7X3p5wlZf4nr6E0GMKbw,2556
-nucliadb-3.0.3.post437.dist-info/METADATA,sha256=YXcSvvI4iPzl7MMfIzDoeqPUnrFJYkv_wNdrOn1eyhs,4348
-nucliadb-3.0.3.post437.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-nucliadb-3.0.3.post437.dist-info/entry_points.txt,sha256=XqGfgFDuY3zXQc8ewXM2TRVjTModIq851zOsgrmaXx4,1268
-nucliadb-3.0.3.post437.dist-info/top_level.txt,sha256=hwYhTVnX7jkQ9gJCkVrbqEG1M4lT2F_iPQND1fCzF80,20
-nucliadb-3.0.3.post437.dist-info/zip-safe,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
-nucliadb-3.0.3.post437.dist-info/RECORD,,
+nucliadb-3.0.3.post438.dist-info/METADATA,sha256=ahFZf6v3gG2ORDLr4fh-5w-lTLgkFYHj9tXjS-45YkM,4348
+nucliadb-3.0.3.post438.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+nucliadb-3.0.3.post438.dist-info/entry_points.txt,sha256=XqGfgFDuY3zXQc8ewXM2TRVjTModIq851zOsgrmaXx4,1268
+nucliadb-3.0.3.post438.dist-info/top_level.txt,sha256=hwYhTVnX7jkQ9gJCkVrbqEG1M4lT2F_iPQND1fCzF80,20
+nucliadb-3.0.3.post438.dist-info/zip-safe,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
+nucliadb-3.0.3.post438.dist-info/RECORD,,
```

