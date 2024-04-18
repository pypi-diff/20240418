# Comparing `tmp/faststream-0.5.1.tar.gz` & `tmp/faststream-0.5.2.tar.gz`

## Comparing `faststream-0.5.1.tar` & `faststream-0.5.2.tar`

### file list

```diff
@@ -1,322 +1,322 @@
--rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 faststream-0.5.1/.codespell-whitelist.txt
--rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 faststream-0.5.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0     3860 2020-02-02 00:00:00.000000 faststream-0.5.1/.secrets.baseline
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 faststream-0.5.1/.semgrepignore
--rw-r--r--   0        0        0     2681 2020-02-02 00:00:00.000000 faststream-0.5.1/CITATION.cff
--rw-r--r--   0        0        0     5480 2020-02-02 00:00:00.000000 faststream-0.5.1/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     2630 2020-02-02 00:00:00.000000 faststream-0.5.1/CONTRIBUTING.md
--rw-r--r--   0        0        0     1420 2020-02-02 00:00:00.000000 faststream-0.5.1/SECURITY.md
--rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 faststream-0.5.1/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0        0        0      630 2020-02-02 00:00:00.000000 faststream-0.5.1/.github/dependabot.yml
--rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 faststream-0.5.1/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 faststream-0.5.1/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0        0        0      975 2020-02-02 00:00:00.000000 faststream-0.5.1/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 faststream-0.5.1/.github/workflows/check-broken-links-in-docs.yaml
--rw-r--r--   0        0        0     3520 2020-02-02 00:00:00.000000 faststream-0.5.1/.github/workflows/codeql.yml
--rw-r--r--   0        0        0      934 2020-02-02 00:00:00.000000 faststream-0.5.1/.github/workflows/dependency-review.yaml
--rw-r--r--   0        0        0     1436 2020-02-02 00:00:00.000000 faststream-0.5.1/.github/workflows/deploy-docs.yaml
--rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 faststream-0.5.1/.github/workflows/publish_coverage.yml
--rw-r--r--   0        0        0     1207 2020-02-02 00:00:00.000000 faststream-0.5.1/.github/workflows/publish_pypi.yml
--rw-r--r--   0        0        0    16399 2020-02-02 00:00:00.000000 faststream-0.5.1/.github/workflows/test.yaml
--rw-r--r--   0        0        0     1999 2020-02-02 00:00:00.000000 faststream-0.5.1/.github/workflows/update_release_notes.yaml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.1/examples/__init__.py
--rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 faststream-0.5.1/examples/e01_basic_consume.py
--rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 faststream-0.5.1/examples/e02_1_basic_publisher.py
--rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 faststream-0.5.1/examples/e02_2_basic_publisher.py
--rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 faststream-0.5.1/examples/e02_3_basic_publisher.py
--rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 faststream-0.5.1/examples/e03_miltiple_pubsub.py
--rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 faststream-0.5.1/examples/e04_msg_filter.py
--rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 faststream-0.5.1/examples/e05_rpc_request.py
--rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 faststream-0.5.1/examples/e06_manual_ack.py
--rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 faststream-0.5.1/examples/e07_ack_immediately.py
--rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 faststream-0.5.1/examples/e08_testing.py
--rw-r--r--   0        0        0      787 2020-02-02 00:00:00.000000 faststream-0.5.1/examples/e09_testing_mocks.py
--rw-r--r--   0        0        0     1364 2020-02-02 00:00:00.000000 faststream-0.5.1/examples/e10_middlewares.py
--rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 faststream-0.5.1/examples/e11_settings.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.1/examples/fastapi_integration/__init__.py
--rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 faststream-0.5.1/examples/fastapi_integration/app.py
--rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 faststream-0.5.1/examples/fastapi_integration/testing.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.1/examples/howto/__init__.py
--rw-r--r--   0        0        0     1188 2020-02-02 00:00:00.000000 faststream-0.5.1/examples/howto/structlogs.py
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 faststream-0.5.1/examples/kafka/__init__.py
--rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 faststream-0.5.1/examples/kafka/ack_after_process.py
--rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 faststream-0.5.1/examples/kafka/batch_consume.py
--rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 faststream-0.5.1/examples/kafka/batch_publish_1.py
--rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 faststream-0.5.1/examples/kafka/batch_publish_2.py
--rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 faststream-0.5.1/examples/kafka/batch_publish_3.py
--rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 faststream-0.5.1/examples/kafka/testing.py
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 faststream-0.5.1/examples/nats/__init__.py
--rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 faststream-0.5.1/examples/nats/e01_basic.py
--rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 faststream-0.5.1/examples/nats/e02_basic_rpc.py
--rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 faststream-0.5.1/examples/nats/e03_publisher.py
--rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 faststream-0.5.1/examples/nats/e04_js_basic.py
--rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 faststream-0.5.1/examples/nats/e05_basic_and_js.py
--rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 faststream-0.5.1/examples/nats/e06_key_value.py
--rw-r--r--   0        0        0      873 2020-02-02 00:00:00.000000 faststream-0.5.1/examples/nats/e07_object_storage.py
--rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 faststream-0.5.1/examples/nats/e08_wildcards.py
--rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 faststream-0.5.1/examples/nats/e09_pull_sub.py
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 faststream-0.5.1/examples/rabbit/__init__.py
--rw-r--r--   0        0        0     1012 2020-02-02 00:00:00.000000 faststream-0.5.1/examples/rabbit/direct.py
--rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 faststream-0.5.1/examples/rabbit/fanout.py
--rw-r--r--   0        0        0     1620 2020-02-02 00:00:00.000000 faststream-0.5.1/examples/rabbit/header.py
--rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 faststream-0.5.1/examples/rabbit/stream.py
--rw-r--r--   0        0        0     1133 2020-02-02 00:00:00.000000 faststream-0.5.1/examples/rabbit/topic.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.1/examples/redis/__init__.py
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 faststream-0.5.1/examples/redis/channel_sub.py
--rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 faststream-0.5.1/examples/redis/channel_sub_pattern.py
--rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 faststream-0.5.1/examples/redis/list_sub.py
--rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 faststream-0.5.1/examples/redis/list_sub_batch.py
--rw-r--r--   0        0        0      974 2020-02-02 00:00:00.000000 faststream-0.5.1/examples/redis/rpc.py
--rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 faststream-0.5.1/examples/redis/stream_sub.py
--rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 faststream-0.5.1/examples/redis/stream_sub_batch.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.1/examples/router/__init__.py
--rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 faststream-0.5.1/examples/router/basic_consume.py
--rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 faststream-0.5.1/examples/router/basic_publish.py
--rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 faststream-0.5.1/examples/router/delay_registration.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.1/examples/serialization/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.1/examples/serialization/avro/__init__.py
--rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 faststream-0.5.1/examples/serialization/avro/avro.py
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 faststream-0.5.1/examples/serialization/avro/person.avsc
--rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 faststream-0.5.1/examples/serialization/avro/requirements.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.1/examples/serialization/msgpack/__init__.py
--rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 faststream-0.5.1/examples/serialization/msgpack/pack.py
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 faststream-0.5.1/examples/serialization/msgpack/requirements.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.1/examples/serialization/protobuf/__init__.py
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 faststream-0.5.1/examples/serialization/protobuf/message.proto
--rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 faststream-0.5.1/examples/serialization/protobuf/protobuf.py
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 faststream-0.5.1/examples/serialization/protobuf/requirements.txt
--rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/__about__.py
--rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/__init__.py
--rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/__main__.py
--rw-r--r--   0        0        0     5562 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/_compat.py
--rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/annotations.py
--rw-r--r--   0        0        0     7313 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/app.py
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/constants.py
--rw-r--r--   0        0        0     1825 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/exceptions.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/py.typed
--rw-r--r--   0        0        0     4511 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/security.py
--rw-r--r--   0        0        0     2356 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/types.py
--rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/asyncapi/__init__.py
--rw-r--r--   0        0        0     1382 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/asyncapi/abc.py
--rw-r--r--   0        0        0     5963 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/asyncapi/generate.py
--rw-r--r--   0        0        0     3384 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/asyncapi/message.py
--rw-r--r--   0        0        0     1029 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/asyncapi/proto.py
--rw-r--r--   0        0        0     4739 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/asyncapi/site.py
--rw-r--r--   0        0        0     1177 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/asyncapi/utils.py
--rw-r--r--   0        0        0     1339 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/asyncapi/schema/__init__.py
--rw-r--r--   0        0        0     1334 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/asyncapi/schema/channels.py
--rw-r--r--   0        0        0     5067 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/asyncapi/schema/info.py
--rw-r--r--   0        0        0     3438 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/asyncapi/schema/main.py
--rw-r--r--   0        0        0     2027 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/asyncapi/schema/message.py
--rw-r--r--   0        0        0     1425 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/asyncapi/schema/operations.py
--rw-r--r--   0        0        0     3032 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/asyncapi/schema/security.py
--rw-r--r--   0        0        0     2350 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/asyncapi/schema/servers.py
--rw-r--r--   0        0        0     2032 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/asyncapi/schema/utils.py
--rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/asyncapi/schema/bindings/__init__.py
--rw-r--r--   0        0        0     2556 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/asyncapi/schema/bindings/amqp.py
--rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/asyncapi/schema/bindings/kafka.py
--rw-r--r--   0        0        0     2726 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/asyncapi/schema/bindings/main.py
--rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/asyncapi/schema/bindings/nats.py
--rw-r--r--   0        0        0     1147 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/asyncapi/schema/bindings/redis.py
--rw-r--r--   0        0        0     1012 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/asyncapi/schema/bindings/sqs.py
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/broker/__init__.py
--rw-r--r--   0        0        0     6047 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/broker/acknowledgement_watcher.py
--rw-r--r--   0        0        0     2630 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/broker/message.py
--rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/broker/proto.py
--rw-r--r--   0        0        0     2103 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/broker/router.py
--rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/broker/schemas.py
--rw-r--r--   0        0        0     1857 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/broker/types.py
--rw-r--r--   0        0        0     3196 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/broker/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/broker/core/__init__.py
--rw-r--r--   0        0        0     4246 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/broker/core/abc.py
--rw-r--r--   0        0        0     2643 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/broker/core/logging.py
--rw-r--r--   0        0        0    10503 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/broker/core/usecase.py
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/broker/fastapi/__init__.py
--rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/broker/fastapi/context.py
--rw-r--r--   0        0        0     4309 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/broker/fastapi/get_dependant.py
--rw-r--r--   0        0        0     9644 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/broker/fastapi/route.py
--rw-r--r--   0        0        0    18036 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/broker/fastapi/router.py
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/broker/middlewares/__init__.py
--rw-r--r--   0        0        0     3139 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/broker/middlewares/base.py
--rw-r--r--   0        0        0     2219 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/broker/middlewares/logging.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/broker/publisher/__init__.py
--rw-r--r--   0        0        0     1386 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/broker/publisher/fake.py
--rw-r--r--   0        0        0     1934 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/broker/publisher/proto.py
--rw-r--r--   0        0        0     5012 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/broker/publisher/usecase.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/broker/subscriber/__init__.py
--rw-r--r--   0        0        0     5197 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/broker/subscriber/call_item.py
--rw-r--r--   0        0        0     2743 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/broker/subscriber/proto.py
--rw-r--r--   0        0        0    13087 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/broker/subscriber/usecase.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/broker/wrapper/__init__.py
--rw-r--r--   0        0        0     6048 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/broker/wrapper/call.py
--rw-r--r--   0        0        0     2361 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/broker/wrapper/proto.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/cli/__init__.py
--rw-r--r--   0        0        0     7018 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/cli/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/cli/docs/__init__.py
--rw-r--r--   0        0        0     4814 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/cli/docs/app.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/cli/supervisors/__init__.py
--rw-r--r--   0        0        0     2052 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/cli/supervisors/basereload.py
--rw-r--r--   0        0        0     1161 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/cli/supervisors/multiprocess.py
--rw-r--r--   0        0        0     1857 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/cli/supervisors/utils.py
--rw-r--r--   0        0        0     2368 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/cli/supervisors/watchfiles.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/cli/utils/__init__.py
--rw-r--r--   0        0        0     3079 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/cli/utils/imports.py
--rw-r--r--   0        0        0     1758 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/cli/utils/logs.py
--rw-r--r--   0        0        0     2006 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/cli/utils/parser.py
--rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/confluent/__init__.py
--rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/confluent/annotations.py
--rw-r--r--   0        0        0    14880 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/confluent/client.py
--rw-r--r--   0        0        0     1213 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/confluent/message.py
--rw-r--r--   0        0        0     3390 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/confluent/parser.py
--rw-r--r--   0        0        0    20008 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/confluent/router.py
--rw-r--r--   0        0        0     2253 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/confluent/security.py
--rw-r--r--   0        0        0     7212 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/confluent/testing.py
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/confluent/broker/__init__.py
--rw-r--r--   0        0        0    18827 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/confluent/broker/broker.py
--rw-r--r--   0        0        0     2276 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/confluent/broker/logging.py
--rw-r--r--   0        0        0    64951 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/confluent/broker/registrator.py
--rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/confluent/fastapi/__init__.py
--rw-r--r--   0        0        0    99735 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/confluent/fastapi/fastapi.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/confluent/publisher/__init__.py
--rw-r--r--   0        0        0     5524 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/confluent/publisher/asyncapi.py
--rw-r--r--   0        0        0     3274 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/confluent/publisher/producer.py
--rw-r--r--   0        0        0     5840 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/confluent/publisher/usecase.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/confluent/schemas/__init__.py
--rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/confluent/schemas/params.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/confluent/subscriber/__init__.py
--rw-r--r--   0        0        0     6124 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/confluent/subscriber/asyncapi.py
--rw-r--r--   0        0        0    10532 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/confluent/subscriber/usecase.py
--rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/kafka/__init__.py
--rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/kafka/annotations.py
--rw-r--r--   0        0        0     1224 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/kafka/message.py
--rw-r--r--   0        0        0     2752 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/kafka/parser.py
--rw-r--r--   0        0        0    20346 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/kafka/router.py
--rw-r--r--   0        0        0     2253 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/kafka/security.py
--rw-r--r--   0        0        0     5923 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/kafka/testing.py
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/kafka/broker/__init__.py
--rw-r--r--   0        0        0    28966 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/kafka/broker/broker.py
--rw-r--r--   0        0        0     2261 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/kafka/broker/logging.py
--rw-r--r--   0        0        0    71638 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/kafka/broker/registrator.py
--rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/kafka/fastapi/__init__.py
--rw-r--r--   0        0        0   117854 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/kafka/fastapi/fastapi.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/kafka/publisher/__init__.py
--rw-r--r--   0        0        0     5520 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/kafka/publisher/asyncapi.py
--rw-r--r--   0        0        0     3242 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/kafka/publisher/producer.py
--rw-r--r--   0        0        0     8807 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/kafka/publisher/usecase.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/kafka/schemas/__init__.py
--rw-r--r--   0        0        0     2105 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/kafka/schemas/params.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/kafka/subscriber/__init__.py
--rw-r--r--   0        0        0     6594 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/kafka/subscriber/asyncapi.py
--rw-r--r--   0        0        0    10959 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/kafka/subscriber/usecase.py
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/log/__init__.py
--rw-r--r--   0        0        0     2424 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/log/formatter.py
--rw-r--r--   0        0        0     1975 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/log/logging.py
--rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/nats/__init__.py
--rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/nats/annotations.py
--rw-r--r--   0        0        0      827 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/nats/helpers.py
--rw-r--r--   0        0        0     1953 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/nats/message.py
--rw-r--r--   0        0        0     3512 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/nats/parser.py
--rw-r--r--   0        0        0    12274 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/nats/router.py
--rw-r--r--   0        0        0      884 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/nats/security.py
--rw-r--r--   0        0        0     4297 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/nats/testing.py
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/nats/broker/__init__.py
--rw-r--r--   0        0        0    27053 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/nats/broker/broker.py
--rw-r--r--   0        0        0     2540 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/nats/broker/logging.py
--rw-r--r--   0        0        0    11868 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/nats/broker/registrator.py
--rw-r--r--   0        0        0     1018 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/nats/fastapi/__init__.py
--rw-r--r--   0        0        0    36228 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/nats/fastapi/fastapi.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/nats/publisher/__init__.py
--rw-r--r--   0        0        0     2736 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/nats/publisher/asyncapi.py
--rw-r--r--   0        0        0     5595 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/nats/publisher/producer.py
--rw-r--r--   0        0        0     5125 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/nats/publisher/usecase.py
--rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/nats/schemas/__init__.py
--rw-r--r--   0        0        0     9645 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/nats/schemas/js_stream.py
--rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/nats/schemas/pull_sub.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/nats/subscriber/__init__.py
--rw-r--r--   0        0        0     6406 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/nats/subscriber/asyncapi.py
--rw-r--r--   0        0        0    14807 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/nats/subscriber/usecase.py
--rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/rabbit/__init__.py
--rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/rabbit/annotations.py
--rw-r--r--   0        0        0     1787 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/rabbit/message.py
--rw-r--r--   0        0        0     3247 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/rabbit/parser.py
--rw-r--r--   0        0        0    11497 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/rabbit/router.py
--rw-r--r--   0        0        0     1028 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/rabbit/security.py
--rw-r--r--   0        0        0    10071 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/rabbit/testing.py
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/rabbit/types.py
--rw-r--r--   0        0        0     4125 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/rabbit/utils.py
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/rabbit/broker/__init__.py
--rw-r--r--   0        0        0    19596 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/rabbit/broker/broker.py
--rw-r--r--   0        0        0     2085 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/rabbit/broker/logging.py
--rw-r--r--   0        0        0    10794 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/rabbit/broker/registrator.py
--rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/rabbit/fastapi/__init__.py
--rw-r--r--   0        0        0    30283 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/rabbit/fastapi/router.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/rabbit/publisher/__init__.py
--rw-r--r--   0        0        0     5063 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/rabbit/publisher/asyncapi.py
--rw-r--r--   0        0        0     7466 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/rabbit/publisher/producer.py
--rw-r--r--   0        0        0     8209 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/rabbit/publisher/usecase.py
--rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/rabbit/schemas/__init__.py
--rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/rabbit/schemas/constants.py
--rw-r--r--   0        0        0     3919 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/rabbit/schemas/exchange.py
--rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/rabbit/schemas/proto.py
--rw-r--r--   0        0        0     3284 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/rabbit/schemas/queue.py
--rw-r--r--   0        0        0     1297 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/rabbit/schemas/reply.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/rabbit/subscriber/__init__.py
--rw-r--r--   0        0        0     4383 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/rabbit/subscriber/asyncapi.py
--rw-r--r--   0        0        0     7172 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/rabbit/subscriber/usecase.py
--rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/redis/__init__.py
--rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/redis/annotations.py
--rw-r--r--   0        0        0     3017 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/redis/message.py
--rw-r--r--   0        0        0     5463 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/redis/parser.py
--rw-r--r--   0        0        0     8211 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/redis/router.py
--rw-r--r--   0        0        0     1494 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/redis/security.py
--rw-r--r--   0        0        0     6635 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/redis/testing.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/redis/broker/__init__.py
--rw-r--r--   0        0        0    15909 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/redis/broker/broker.py
--rw-r--r--   0        0        0     1845 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/redis/broker/logging.py
--rw-r--r--   0        0        0     7576 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/redis/broker/registrator.py
--rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/redis/fastapi/__init__.py
--rw-r--r--   0        0        0    27558 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/redis/fastapi/fastapi.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/redis/publisher/__init__.py
--rw-r--r--   0        0        0     6019 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/redis/publisher/asyncapi.py
--rw-r--r--   0        0        0     4143 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/redis/publisher/producer.py
--rw-r--r--   0        0        0    14932 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/redis/publisher/usecase.py
--rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/redis/schemas/__init__.py
--rw-r--r--   0        0        0      828 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/redis/schemas/list_sub.py
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/redis/schemas/proto.py
--rw-r--r--   0        0        0      862 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/redis/schemas/pub_sub.py
--rw-r--r--   0        0        0     1603 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/redis/schemas/stream_sub.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/redis/subscriber/__init__.py
--rw-r--r--   0        0        0     7044 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/redis/subscriber/asyncapi.py
--rw-r--r--   0        0        0    21352 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/redis/subscriber/usecase.py
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/testing/__init__.py
--rw-r--r--   0        0        0     2244 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/testing/app.py
--rw-r--r--   0        0        0     6746 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/testing/broker.py
--rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/utils/__init__.py
--rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/utils/ast.py
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/utils/classes.py
--rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/utils/data.py
--rw-r--r--   0        0        0     1932 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/utils/functions.py
--rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/utils/no_cast.py
--rw-r--r--   0        0        0     1317 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/utils/path.py
--rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/utils/context/__init__.py
--rw-r--r--   0        0        0      966 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/utils/context/builders.py
--rw-r--r--   0        0        0     5117 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/utils/context/repository.py
--rw-r--r--   0        0        0     2536 2020-02-02 00:00:00.000000 faststream-0.5.1/faststream/utils/context/types.py
--rwxr-xr-x   0        0        0      915 2020-02-02 00:00:00.000000 faststream-0.5.1/scripts/build-docs-pre-commit.sh
--rwxr-xr-x   0        0        0       66 2020-02-02 00:00:00.000000 faststream-0.5.1/scripts/build-docs.sh
--rwxr-xr-x   0        0        0      909 2020-02-02 00:00:00.000000 faststream-0.5.1/scripts/lint-pre-commit.sh
--rwxr-xr-x   0        0        0      247 2020-02-02 00:00:00.000000 faststream-0.5.1/scripts/lint.sh
--rwxr-xr-x   0        0        0       51 2020-02-02 00:00:00.000000 faststream-0.5.1/scripts/publish.sh
--rwxr-xr-x   0        0        0       70 2020-02-02 00:00:00.000000 faststream-0.5.1/scripts/serve-docs.sh
--rwxr-xr-x   0        0        0      522 2020-02-02 00:00:00.000000 faststream-0.5.1/scripts/set_variables.sh
--rwxr-xr-x   0        0        0      147 2020-02-02 00:00:00.000000 faststream-0.5.1/scripts/start_test_env.sh
--rwxr-xr-x   0        0        0      175 2020-02-02 00:00:00.000000 faststream-0.5.1/scripts/static-analysis.sh
--rwxr-xr-x   0        0        0      926 2020-02-02 00:00:00.000000 faststream-0.5.1/scripts/static-pre-commit.sh
--rwxr-xr-x   0        0        0      132 2020-02-02 00:00:00.000000 faststream-0.5.1/scripts/stop_test_env.sh
--rwxr-xr-x   0        0        0      154 2020-02-02 00:00:00.000000 faststream-0.5.1/scripts/test-cov.sh
--rwxr-xr-x   0        0        0      131 2020-02-02 00:00:00.000000 faststream-0.5.1/scripts/test.sh
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 faststream-0.5.1/.gitignore
--rw-r--r--   0        0        0    11363 2020-02-02 00:00:00.000000 faststream-0.5.1/LICENSE
--rw-r--r--   0        0        0    14865 2020-02-02 00:00:00.000000 faststream-0.5.1/README.md
--rw-r--r--   0        0        0    10330 2020-02-02 00:00:00.000000 faststream-0.5.1/pyproject.toml
--rw-r--r--   0        0        0    22988 2020-02-02 00:00:00.000000 faststream-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 faststream-0.5.2/.codespell-whitelist.txt
+-rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 faststream-0.5.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     3860 2020-02-02 00:00:00.000000 faststream-0.5.2/.secrets.baseline
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 faststream-0.5.2/.semgrepignore
+-rw-r--r--   0        0        0     2681 2020-02-02 00:00:00.000000 faststream-0.5.2/CITATION.cff
+-rw-r--r--   0        0        0     5480 2020-02-02 00:00:00.000000 faststream-0.5.2/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     2630 2020-02-02 00:00:00.000000 faststream-0.5.2/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1420 2020-02-02 00:00:00.000000 faststream-0.5.2/SECURITY.md
+-rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 faststream-0.5.2/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0        0        0      630 2020-02-02 00:00:00.000000 faststream-0.5.2/.github/dependabot.yml
+-rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 faststream-0.5.2/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 faststream-0.5.2/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0        0        0      975 2020-02-02 00:00:00.000000 faststream-0.5.2/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 faststream-0.5.2/.github/workflows/check-broken-links-in-docs.yaml
+-rw-r--r--   0        0        0     3520 2020-02-02 00:00:00.000000 faststream-0.5.2/.github/workflows/codeql.yml
+-rw-r--r--   0        0        0      934 2020-02-02 00:00:00.000000 faststream-0.5.2/.github/workflows/dependency-review.yaml
+-rw-r--r--   0        0        0     1436 2020-02-02 00:00:00.000000 faststream-0.5.2/.github/workflows/deploy-docs.yaml
+-rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 faststream-0.5.2/.github/workflows/publish_coverage.yml
+-rw-r--r--   0        0        0     1207 2020-02-02 00:00:00.000000 faststream-0.5.2/.github/workflows/publish_pypi.yml
+-rw-r--r--   0        0        0    16399 2020-02-02 00:00:00.000000 faststream-0.5.2/.github/workflows/test.yaml
+-rw-r--r--   0        0        0     1999 2020-02-02 00:00:00.000000 faststream-0.5.2/.github/workflows/update_release_notes.yaml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.2/examples/__init__.py
+-rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 faststream-0.5.2/examples/e01_basic_consume.py
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 faststream-0.5.2/examples/e02_1_basic_publisher.py
+-rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 faststream-0.5.2/examples/e02_2_basic_publisher.py
+-rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 faststream-0.5.2/examples/e02_3_basic_publisher.py
+-rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 faststream-0.5.2/examples/e03_miltiple_pubsub.py
+-rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 faststream-0.5.2/examples/e04_msg_filter.py
+-rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 faststream-0.5.2/examples/e05_rpc_request.py
+-rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 faststream-0.5.2/examples/e06_manual_ack.py
+-rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 faststream-0.5.2/examples/e07_ack_immediately.py
+-rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 faststream-0.5.2/examples/e08_testing.py
+-rw-r--r--   0        0        0      787 2020-02-02 00:00:00.000000 faststream-0.5.2/examples/e09_testing_mocks.py
+-rw-r--r--   0        0        0     1364 2020-02-02 00:00:00.000000 faststream-0.5.2/examples/e10_middlewares.py
+-rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 faststream-0.5.2/examples/e11_settings.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.2/examples/fastapi_integration/__init__.py
+-rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 faststream-0.5.2/examples/fastapi_integration/app.py
+-rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 faststream-0.5.2/examples/fastapi_integration/testing.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.2/examples/howto/__init__.py
+-rw-r--r--   0        0        0     1188 2020-02-02 00:00:00.000000 faststream-0.5.2/examples/howto/structlogs.py
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 faststream-0.5.2/examples/kafka/__init__.py
+-rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 faststream-0.5.2/examples/kafka/ack_after_process.py
+-rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 faststream-0.5.2/examples/kafka/batch_consume.py
+-rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 faststream-0.5.2/examples/kafka/batch_publish_1.py
+-rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 faststream-0.5.2/examples/kafka/batch_publish_2.py
+-rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 faststream-0.5.2/examples/kafka/batch_publish_3.py
+-rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 faststream-0.5.2/examples/kafka/testing.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 faststream-0.5.2/examples/nats/__init__.py
+-rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 faststream-0.5.2/examples/nats/e01_basic.py
+-rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 faststream-0.5.2/examples/nats/e02_basic_rpc.py
+-rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 faststream-0.5.2/examples/nats/e03_publisher.py
+-rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 faststream-0.5.2/examples/nats/e04_js_basic.py
+-rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 faststream-0.5.2/examples/nats/e05_basic_and_js.py
+-rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 faststream-0.5.2/examples/nats/e06_key_value.py
+-rw-r--r--   0        0        0      873 2020-02-02 00:00:00.000000 faststream-0.5.2/examples/nats/e07_object_storage.py
+-rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 faststream-0.5.2/examples/nats/e08_wildcards.py
+-rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 faststream-0.5.2/examples/nats/e09_pull_sub.py
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 faststream-0.5.2/examples/rabbit/__init__.py
+-rw-r--r--   0        0        0     1012 2020-02-02 00:00:00.000000 faststream-0.5.2/examples/rabbit/direct.py
+-rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 faststream-0.5.2/examples/rabbit/fanout.py
+-rw-r--r--   0        0        0     1620 2020-02-02 00:00:00.000000 faststream-0.5.2/examples/rabbit/header.py
+-rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 faststream-0.5.2/examples/rabbit/stream.py
+-rw-r--r--   0        0        0     1133 2020-02-02 00:00:00.000000 faststream-0.5.2/examples/rabbit/topic.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.2/examples/redis/__init__.py
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 faststream-0.5.2/examples/redis/channel_sub.py
+-rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 faststream-0.5.2/examples/redis/channel_sub_pattern.py
+-rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 faststream-0.5.2/examples/redis/list_sub.py
+-rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 faststream-0.5.2/examples/redis/list_sub_batch.py
+-rw-r--r--   0        0        0      974 2020-02-02 00:00:00.000000 faststream-0.5.2/examples/redis/rpc.py
+-rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 faststream-0.5.2/examples/redis/stream_sub.py
+-rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 faststream-0.5.2/examples/redis/stream_sub_batch.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.2/examples/router/__init__.py
+-rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 faststream-0.5.2/examples/router/basic_consume.py
+-rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 faststream-0.5.2/examples/router/basic_publish.py
+-rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 faststream-0.5.2/examples/router/delay_registration.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.2/examples/serialization/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.2/examples/serialization/avro/__init__.py
+-rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 faststream-0.5.2/examples/serialization/avro/avro.py
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 faststream-0.5.2/examples/serialization/avro/person.avsc
+-rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 faststream-0.5.2/examples/serialization/avro/requirements.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.2/examples/serialization/msgpack/__init__.py
+-rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 faststream-0.5.2/examples/serialization/msgpack/pack.py
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 faststream-0.5.2/examples/serialization/msgpack/requirements.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.2/examples/serialization/protobuf/__init__.py
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 faststream-0.5.2/examples/serialization/protobuf/message.proto
+-rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 faststream-0.5.2/examples/serialization/protobuf/protobuf.py
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 faststream-0.5.2/examples/serialization/protobuf/requirements.txt
+-rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 faststream-0.5.2/faststream/__about__.py
+-rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 faststream-0.5.2/faststream/__init__.py
+-rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 faststream-0.5.2/faststream/__main__.py
+-rw-r--r--   0        0        0     5562 2020-02-02 00:00:00.000000 faststream-0.5.2/faststream/_compat.py
+-rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 faststream-0.5.2/faststream/annotations.py
+-rw-r--r--   0        0        0     7313 2020-02-02 00:00:00.000000 faststream-0.5.2/faststream/app.py
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 faststream-0.5.2/faststream/constants.py
+-rw-r--r--   0        0        0     1825 2020-02-02 00:00:00.000000 faststream-0.5.2/faststream/exceptions.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.2/faststream/py.typed
+-rw-r--r--   0        0        0     4511 2020-02-02 00:00:00.000000 faststream-0.5.2/faststream/security.py
+-rw-r--r--   0        0        0     2356 2020-02-02 00:00:00.000000 faststream-0.5.2/faststream/types.py
+-rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 faststream-0.5.2/faststream/asyncapi/__init__.py
+-rw-r--r--   0        0        0     1382 2020-02-02 00:00:00.000000 faststream-0.5.2/faststream/asyncapi/abc.py
+-rw-r--r--   0        0        0     5963 2020-02-02 00:00:00.000000 faststream-0.5.2/faststream/asyncapi/generate.py
+-rw-r--r--   0        0        0     3384 2020-02-02 00:00:00.000000 faststream-0.5.2/faststream/asyncapi/message.py
+-rw-r--r--   0        0        0     1029 2020-02-02 00:00:00.000000 faststream-0.5.2/faststream/asyncapi/proto.py
+-rw-r--r--   0        0        0     4739 2020-02-02 00:00:00.000000 faststream-0.5.2/faststream/asyncapi/site.py
+-rw-r--r--   0        0        0     1177 2020-02-02 00:00:00.000000 faststream-0.5.2/faststream/asyncapi/utils.py
+-rw-r--r--   0        0        0     1339 2020-02-02 00:00:00.000000 faststream-0.5.2/faststream/asyncapi/schema/__init__.py
+-rw-r--r--   0        0        0     1334 2020-02-02 00:00:00.000000 faststream-0.5.2/faststream/asyncapi/schema/channels.py
+-rw-r--r--   0        0        0     5067 2020-02-02 00:00:00.000000 faststream-0.5.2/faststream/asyncapi/schema/info.py
+-rw-r--r--   0        0        0     3438 2020-02-02 00:00:00.000000 faststream-0.5.2/faststream/asyncapi/schema/main.py
+-rw-r--r--   0        0        0     2027 2020-02-02 00:00:00.000000 faststream-0.5.2/faststream/asyncapi/schema/message.py
+-rw-r--r--   0        0        0     1425 2020-02-02 00:00:00.000000 faststream-0.5.2/faststream/asyncapi/schema/operations.py
+-rw-r--r--   0        0        0     3032 2020-02-02 00:00:00.000000 faststream-0.5.2/faststream/asyncapi/schema/security.py
+-rw-r--r--   0        0        0     2350 2020-02-02 00:00:00.000000 faststream-0.5.2/faststream/asyncapi/schema/servers.py
+-rw-r--r--   0        0        0     2032 2020-02-02 00:00:00.000000 faststream-0.5.2/faststream/asyncapi/schema/utils.py
+-rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 faststream-0.5.2/faststream/asyncapi/schema/bindings/__init__.py
+-rw-r--r--   0        0        0     2556 2020-02-02 00:00:00.000000 faststream-0.5.2/faststream/asyncapi/schema/bindings/amqp.py
+-rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 faststream-0.5.2/faststream/asyncapi/schema/bindings/kafka.py
+-rw-r--r--   0        0        0     2726 2020-02-02 00:00:00.000000 faststream-0.5.2/faststream/asyncapi/schema/bindings/main.py
+-rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 faststream-0.5.2/faststream/asyncapi/schema/bindings/nats.py
+-rw-r--r--   0        0        0     1147 2020-02-02 00:00:00.000000 faststream-0.5.2/faststream/asyncapi/schema/bindings/redis.py
+-rw-r--r--   0        0        0     1012 2020-02-02 00:00:00.000000 faststream-0.5.2/faststream/asyncapi/schema/bindings/sqs.py
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 faststream-0.5.2/faststream/broker/__init__.py
+-rw-r--r--   0        0        0     6047 2020-02-02 00:00:00.000000 faststream-0.5.2/faststream/broker/acknowledgement_watcher.py
+-rw-r--r--   0        0        0     2630 2020-02-02 00:00:00.000000 faststream-0.5.2/faststream/broker/message.py
+-rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 faststream-0.5.2/faststream/broker/proto.py
+-rw-r--r--   0        0        0     2103 2020-02-02 00:00:00.000000 faststream-0.5.2/faststream/broker/router.py
+-rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 faststream-0.5.2/faststream/broker/schemas.py
+-rw-r--r--   0        0        0     1857 2020-02-02 00:00:00.000000 faststream-0.5.2/faststream/broker/types.py
+-rw-r--r--   0        0        0     3196 2020-02-02 00:00:00.000000 faststream-0.5.2/faststream/broker/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.2/faststream/broker/core/__init__.py
+-rw-r--r--   0        0        0     4246 2020-02-02 00:00:00.000000 faststream-0.5.2/faststream/broker/core/abc.py
+-rw-r--r--   0        0        0     2643 2020-02-02 00:00:00.000000 faststream-0.5.2/faststream/broker/core/logging.py
+-rw-r--r--   0        0        0    10503 2020-02-02 00:00:00.000000 faststream-0.5.2/faststream/broker/core/usecase.py
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 faststream-0.5.2/faststream/broker/fastapi/__init__.py
+-rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 faststream-0.5.2/faststream/broker/fastapi/context.py
+-rw-r--r--   0        0        0     4309 2020-02-02 00:00:00.000000 faststream-0.5.2/faststream/broker/fastapi/get_dependant.py
+-rw-r--r--   0        0        0     9644 2020-02-02 00:00:00.000000 faststream-0.5.2/faststream/broker/fastapi/route.py
+-rw-r--r--   0        0        0    18036 2020-02-02 00:00:00.000000 faststream-0.5.2/faststream/broker/fastapi/router.py
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 faststream-0.5.2/faststream/broker/middlewares/__init__.py
+-rw-r--r--   0        0        0     3123 2020-02-02 00:00:00.000000 faststream-0.5.2/faststream/broker/middlewares/base.py
+-rw-r--r--   0        0        0     2219 2020-02-02 00:00:00.000000 faststream-0.5.2/faststream/broker/middlewares/logging.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.2/faststream/broker/publisher/__init__.py
+-rw-r--r--   0        0        0     1386 2020-02-02 00:00:00.000000 faststream-0.5.2/faststream/broker/publisher/fake.py
+-rw-r--r--   0        0        0     1934 2020-02-02 00:00:00.000000 faststream-0.5.2/faststream/broker/publisher/proto.py
+-rw-r--r--   0        0        0     5012 2020-02-02 00:00:00.000000 faststream-0.5.2/faststream/broker/publisher/usecase.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.2/faststream/broker/subscriber/__init__.py
+-rw-r--r--   0        0        0     5197 2020-02-02 00:00:00.000000 faststream-0.5.2/faststream/broker/subscriber/call_item.py
+-rw-r--r--   0        0        0     2743 2020-02-02 00:00:00.000000 faststream-0.5.2/faststream/broker/subscriber/proto.py
+-rw-r--r--   0        0        0    13087 2020-02-02 00:00:00.000000 faststream-0.5.2/faststream/broker/subscriber/usecase.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.2/faststream/broker/wrapper/__init__.py
+-rw-r--r--   0        0        0     6048 2020-02-02 00:00:00.000000 faststream-0.5.2/faststream/broker/wrapper/call.py
+-rw-r--r--   0        0        0     2361 2020-02-02 00:00:00.000000 faststream-0.5.2/faststream/broker/wrapper/proto.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.2/faststream/cli/__init__.py
+-rw-r--r--   0        0        0     7018 2020-02-02 00:00:00.000000 faststream-0.5.2/faststream/cli/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.2/faststream/cli/docs/__init__.py
+-rw-r--r--   0        0        0     4814 2020-02-02 00:00:00.000000 faststream-0.5.2/faststream/cli/docs/app.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.2/faststream/cli/supervisors/__init__.py
+-rw-r--r--   0        0        0     2052 2020-02-02 00:00:00.000000 faststream-0.5.2/faststream/cli/supervisors/basereload.py
+-rw-r--r--   0        0        0     1161 2020-02-02 00:00:00.000000 faststream-0.5.2/faststream/cli/supervisors/multiprocess.py
+-rw-r--r--   0        0        0     1857 2020-02-02 00:00:00.000000 faststream-0.5.2/faststream/cli/supervisors/utils.py
+-rw-r--r--   0        0        0     2368 2020-02-02 00:00:00.000000 faststream-0.5.2/faststream/cli/supervisors/watchfiles.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.2/faststream/cli/utils/__init__.py
+-rw-r--r--   0        0        0     3079 2020-02-02 00:00:00.000000 faststream-0.5.2/faststream/cli/utils/imports.py
+-rw-r--r--   0        0        0     1758 2020-02-02 00:00:00.000000 faststream-0.5.2/faststream/cli/utils/logs.py
+-rw-r--r--   0        0        0     2006 2020-02-02 00:00:00.000000 faststream-0.5.2/faststream/cli/utils/parser.py
+-rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 faststream-0.5.2/faststream/confluent/__init__.py
+-rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 faststream-0.5.2/faststream/confluent/annotations.py
+-rw-r--r--   0        0        0    14880 2020-02-02 00:00:00.000000 faststream-0.5.2/faststream/confluent/client.py
+-rw-r--r--   0        0        0     1213 2020-02-02 00:00:00.000000 faststream-0.5.2/faststream/confluent/message.py
+-rw-r--r--   0        0        0     3390 2020-02-02 00:00:00.000000 faststream-0.5.2/faststream/confluent/parser.py
+-rw-r--r--   0        0        0    20008 2020-02-02 00:00:00.000000 faststream-0.5.2/faststream/confluent/router.py
+-rw-r--r--   0        0        0     2253 2020-02-02 00:00:00.000000 faststream-0.5.2/faststream/confluent/security.py
+-rw-r--r--   0        0        0     7212 2020-02-02 00:00:00.000000 faststream-0.5.2/faststream/confluent/testing.py
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 faststream-0.5.2/faststream/confluent/broker/__init__.py
+-rw-r--r--   0        0        0    18827 2020-02-02 00:00:00.000000 faststream-0.5.2/faststream/confluent/broker/broker.py
+-rw-r--r--   0        0        0     2276 2020-02-02 00:00:00.000000 faststream-0.5.2/faststream/confluent/broker/logging.py
+-rw-r--r--   0        0        0    64951 2020-02-02 00:00:00.000000 faststream-0.5.2/faststream/confluent/broker/registrator.py
+-rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 faststream-0.5.2/faststream/confluent/fastapi/__init__.py
+-rw-r--r--   0        0        0    99735 2020-02-02 00:00:00.000000 faststream-0.5.2/faststream/confluent/fastapi/fastapi.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.2/faststream/confluent/publisher/__init__.py
+-rw-r--r--   0        0        0     5524 2020-02-02 00:00:00.000000 faststream-0.5.2/faststream/confluent/publisher/asyncapi.py
+-rw-r--r--   0        0        0     3274 2020-02-02 00:00:00.000000 faststream-0.5.2/faststream/confluent/publisher/producer.py
+-rw-r--r--   0        0        0     5840 2020-02-02 00:00:00.000000 faststream-0.5.2/faststream/confluent/publisher/usecase.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.2/faststream/confluent/schemas/__init__.py
+-rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 faststream-0.5.2/faststream/confluent/schemas/params.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.2/faststream/confluent/subscriber/__init__.py
+-rw-r--r--   0        0        0     6124 2020-02-02 00:00:00.000000 faststream-0.5.2/faststream/confluent/subscriber/asyncapi.py
+-rw-r--r--   0        0        0    10532 2020-02-02 00:00:00.000000 faststream-0.5.2/faststream/confluent/subscriber/usecase.py
+-rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 faststream-0.5.2/faststream/kafka/__init__.py
+-rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 faststream-0.5.2/faststream/kafka/annotations.py
+-rw-r--r--   0        0        0     1224 2020-02-02 00:00:00.000000 faststream-0.5.2/faststream/kafka/message.py
+-rw-r--r--   0        0        0     2752 2020-02-02 00:00:00.000000 faststream-0.5.2/faststream/kafka/parser.py
+-rw-r--r--   0        0        0    20346 2020-02-02 00:00:00.000000 faststream-0.5.2/faststream/kafka/router.py
+-rw-r--r--   0        0        0     2253 2020-02-02 00:00:00.000000 faststream-0.5.2/faststream/kafka/security.py
+-rw-r--r--   0        0        0     5923 2020-02-02 00:00:00.000000 faststream-0.5.2/faststream/kafka/testing.py
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 faststream-0.5.2/faststream/kafka/broker/__init__.py
+-rw-r--r--   0        0        0    28966 2020-02-02 00:00:00.000000 faststream-0.5.2/faststream/kafka/broker/broker.py
+-rw-r--r--   0        0        0     2261 2020-02-02 00:00:00.000000 faststream-0.5.2/faststream/kafka/broker/logging.py
+-rw-r--r--   0        0        0    71638 2020-02-02 00:00:00.000000 faststream-0.5.2/faststream/kafka/broker/registrator.py
+-rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 faststream-0.5.2/faststream/kafka/fastapi/__init__.py
+-rw-r--r--   0        0        0   117854 2020-02-02 00:00:00.000000 faststream-0.5.2/faststream/kafka/fastapi/fastapi.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.2/faststream/kafka/publisher/__init__.py
+-rw-r--r--   0        0        0     5520 2020-02-02 00:00:00.000000 faststream-0.5.2/faststream/kafka/publisher/asyncapi.py
+-rw-r--r--   0        0        0     3242 2020-02-02 00:00:00.000000 faststream-0.5.2/faststream/kafka/publisher/producer.py
+-rw-r--r--   0        0        0     8807 2020-02-02 00:00:00.000000 faststream-0.5.2/faststream/kafka/publisher/usecase.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.2/faststream/kafka/schemas/__init__.py
+-rw-r--r--   0        0        0     2105 2020-02-02 00:00:00.000000 faststream-0.5.2/faststream/kafka/schemas/params.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.2/faststream/kafka/subscriber/__init__.py
+-rw-r--r--   0        0        0     6594 2020-02-02 00:00:00.000000 faststream-0.5.2/faststream/kafka/subscriber/asyncapi.py
+-rw-r--r--   0        0        0    10959 2020-02-02 00:00:00.000000 faststream-0.5.2/faststream/kafka/subscriber/usecase.py
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 faststream-0.5.2/faststream/log/__init__.py
+-rw-r--r--   0        0        0     2424 2020-02-02 00:00:00.000000 faststream-0.5.2/faststream/log/formatter.py
+-rw-r--r--   0        0        0     1975 2020-02-02 00:00:00.000000 faststream-0.5.2/faststream/log/logging.py
+-rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 faststream-0.5.2/faststream/nats/__init__.py
+-rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 faststream-0.5.2/faststream/nats/annotations.py
+-rw-r--r--   0        0        0      827 2020-02-02 00:00:00.000000 faststream-0.5.2/faststream/nats/helpers.py
+-rw-r--r--   0        0        0     1953 2020-02-02 00:00:00.000000 faststream-0.5.2/faststream/nats/message.py
+-rw-r--r--   0        0        0     3512 2020-02-02 00:00:00.000000 faststream-0.5.2/faststream/nats/parser.py
+-rw-r--r--   0        0        0    12274 2020-02-02 00:00:00.000000 faststream-0.5.2/faststream/nats/router.py
+-rw-r--r--   0        0        0      884 2020-02-02 00:00:00.000000 faststream-0.5.2/faststream/nats/security.py
+-rw-r--r--   0        0        0     4297 2020-02-02 00:00:00.000000 faststream-0.5.2/faststream/nats/testing.py
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 faststream-0.5.2/faststream/nats/broker/__init__.py
+-rw-r--r--   0        0        0    27053 2020-02-02 00:00:00.000000 faststream-0.5.2/faststream/nats/broker/broker.py
+-rw-r--r--   0        0        0     2540 2020-02-02 00:00:00.000000 faststream-0.5.2/faststream/nats/broker/logging.py
+-rw-r--r--   0        0        0    11868 2020-02-02 00:00:00.000000 faststream-0.5.2/faststream/nats/broker/registrator.py
+-rw-r--r--   0        0        0     1018 2020-02-02 00:00:00.000000 faststream-0.5.2/faststream/nats/fastapi/__init__.py
+-rw-r--r--   0        0        0    36228 2020-02-02 00:00:00.000000 faststream-0.5.2/faststream/nats/fastapi/fastapi.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.2/faststream/nats/publisher/__init__.py
+-rw-r--r--   0        0        0     2736 2020-02-02 00:00:00.000000 faststream-0.5.2/faststream/nats/publisher/asyncapi.py
+-rw-r--r--   0        0        0     5595 2020-02-02 00:00:00.000000 faststream-0.5.2/faststream/nats/publisher/producer.py
+-rw-r--r--   0        0        0     5125 2020-02-02 00:00:00.000000 faststream-0.5.2/faststream/nats/publisher/usecase.py
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 faststream-0.5.2/faststream/nats/schemas/__init__.py
+-rw-r--r--   0        0        0     9645 2020-02-02 00:00:00.000000 faststream-0.5.2/faststream/nats/schemas/js_stream.py
+-rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 faststream-0.5.2/faststream/nats/schemas/pull_sub.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.2/faststream/nats/subscriber/__init__.py
+-rw-r--r--   0        0        0     6406 2020-02-02 00:00:00.000000 faststream-0.5.2/faststream/nats/subscriber/asyncapi.py
+-rw-r--r--   0        0        0    14807 2020-02-02 00:00:00.000000 faststream-0.5.2/faststream/nats/subscriber/usecase.py
+-rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 faststream-0.5.2/faststream/rabbit/__init__.py
+-rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 faststream-0.5.2/faststream/rabbit/annotations.py
+-rw-r--r--   0        0        0     1787 2020-02-02 00:00:00.000000 faststream-0.5.2/faststream/rabbit/message.py
+-rw-r--r--   0        0        0     3247 2020-02-02 00:00:00.000000 faststream-0.5.2/faststream/rabbit/parser.py
+-rw-r--r--   0        0        0    11497 2020-02-02 00:00:00.000000 faststream-0.5.2/faststream/rabbit/router.py
+-rw-r--r--   0        0        0     1028 2020-02-02 00:00:00.000000 faststream-0.5.2/faststream/rabbit/security.py
+-rw-r--r--   0        0        0    10071 2020-02-02 00:00:00.000000 faststream-0.5.2/faststream/rabbit/testing.py
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 faststream-0.5.2/faststream/rabbit/types.py
+-rw-r--r--   0        0        0     4125 2020-02-02 00:00:00.000000 faststream-0.5.2/faststream/rabbit/utils.py
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 faststream-0.5.2/faststream/rabbit/broker/__init__.py
+-rw-r--r--   0        0        0    19596 2020-02-02 00:00:00.000000 faststream-0.5.2/faststream/rabbit/broker/broker.py
+-rw-r--r--   0        0        0     2085 2020-02-02 00:00:00.000000 faststream-0.5.2/faststream/rabbit/broker/logging.py
+-rw-r--r--   0        0        0    10794 2020-02-02 00:00:00.000000 faststream-0.5.2/faststream/rabbit/broker/registrator.py
+-rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 faststream-0.5.2/faststream/rabbit/fastapi/__init__.py
+-rw-r--r--   0        0        0    30283 2020-02-02 00:00:00.000000 faststream-0.5.2/faststream/rabbit/fastapi/router.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.2/faststream/rabbit/publisher/__init__.py
+-rw-r--r--   0        0        0     5063 2020-02-02 00:00:00.000000 faststream-0.5.2/faststream/rabbit/publisher/asyncapi.py
+-rw-r--r--   0        0        0     7466 2020-02-02 00:00:00.000000 faststream-0.5.2/faststream/rabbit/publisher/producer.py
+-rw-r--r--   0        0        0     8209 2020-02-02 00:00:00.000000 faststream-0.5.2/faststream/rabbit/publisher/usecase.py
+-rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 faststream-0.5.2/faststream/rabbit/schemas/__init__.py
+-rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 faststream-0.5.2/faststream/rabbit/schemas/constants.py
+-rw-r--r--   0        0        0     3919 2020-02-02 00:00:00.000000 faststream-0.5.2/faststream/rabbit/schemas/exchange.py
+-rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 faststream-0.5.2/faststream/rabbit/schemas/proto.py
+-rw-r--r--   0        0        0     3284 2020-02-02 00:00:00.000000 faststream-0.5.2/faststream/rabbit/schemas/queue.py
+-rw-r--r--   0        0        0     1297 2020-02-02 00:00:00.000000 faststream-0.5.2/faststream/rabbit/schemas/reply.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.2/faststream/rabbit/subscriber/__init__.py
+-rw-r--r--   0        0        0     4383 2020-02-02 00:00:00.000000 faststream-0.5.2/faststream/rabbit/subscriber/asyncapi.py
+-rw-r--r--   0        0        0     7172 2020-02-02 00:00:00.000000 faststream-0.5.2/faststream/rabbit/subscriber/usecase.py
+-rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 faststream-0.5.2/faststream/redis/__init__.py
+-rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 faststream-0.5.2/faststream/redis/annotations.py
+-rw-r--r--   0        0        0     3017 2020-02-02 00:00:00.000000 faststream-0.5.2/faststream/redis/message.py
+-rw-r--r--   0        0        0     5463 2020-02-02 00:00:00.000000 faststream-0.5.2/faststream/redis/parser.py
+-rw-r--r--   0        0        0     8211 2020-02-02 00:00:00.000000 faststream-0.5.2/faststream/redis/router.py
+-rw-r--r--   0        0        0     1494 2020-02-02 00:00:00.000000 faststream-0.5.2/faststream/redis/security.py
+-rw-r--r--   0        0        0     6635 2020-02-02 00:00:00.000000 faststream-0.5.2/faststream/redis/testing.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.2/faststream/redis/broker/__init__.py
+-rw-r--r--   0        0        0    15909 2020-02-02 00:00:00.000000 faststream-0.5.2/faststream/redis/broker/broker.py
+-rw-r--r--   0        0        0     1845 2020-02-02 00:00:00.000000 faststream-0.5.2/faststream/redis/broker/logging.py
+-rw-r--r--   0        0        0     7576 2020-02-02 00:00:00.000000 faststream-0.5.2/faststream/redis/broker/registrator.py
+-rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 faststream-0.5.2/faststream/redis/fastapi/__init__.py
+-rw-r--r--   0        0        0    27638 2020-02-02 00:00:00.000000 faststream-0.5.2/faststream/redis/fastapi/fastapi.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.2/faststream/redis/publisher/__init__.py
+-rw-r--r--   0        0        0     6019 2020-02-02 00:00:00.000000 faststream-0.5.2/faststream/redis/publisher/asyncapi.py
+-rw-r--r--   0        0        0     4143 2020-02-02 00:00:00.000000 faststream-0.5.2/faststream/redis/publisher/producer.py
+-rw-r--r--   0        0        0    14932 2020-02-02 00:00:00.000000 faststream-0.5.2/faststream/redis/publisher/usecase.py
+-rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 faststream-0.5.2/faststream/redis/schemas/__init__.py
+-rw-r--r--   0        0        0      828 2020-02-02 00:00:00.000000 faststream-0.5.2/faststream/redis/schemas/list_sub.py
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 faststream-0.5.2/faststream/redis/schemas/proto.py
+-rw-r--r--   0        0        0      862 2020-02-02 00:00:00.000000 faststream-0.5.2/faststream/redis/schemas/pub_sub.py
+-rw-r--r--   0        0        0     1603 2020-02-02 00:00:00.000000 faststream-0.5.2/faststream/redis/schemas/stream_sub.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.2/faststream/redis/subscriber/__init__.py
+-rw-r--r--   0        0        0     7044 2020-02-02 00:00:00.000000 faststream-0.5.2/faststream/redis/subscriber/asyncapi.py
+-rw-r--r--   0        0        0    21352 2020-02-02 00:00:00.000000 faststream-0.5.2/faststream/redis/subscriber/usecase.py
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 faststream-0.5.2/faststream/testing/__init__.py
+-rw-r--r--   0        0        0     2244 2020-02-02 00:00:00.000000 faststream-0.5.2/faststream/testing/app.py
+-rw-r--r--   0        0        0     6746 2020-02-02 00:00:00.000000 faststream-0.5.2/faststream/testing/broker.py
+-rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 faststream-0.5.2/faststream/utils/__init__.py
+-rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 faststream-0.5.2/faststream/utils/ast.py
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 faststream-0.5.2/faststream/utils/classes.py
+-rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 faststream-0.5.2/faststream/utils/data.py
+-rw-r--r--   0        0        0     1932 2020-02-02 00:00:00.000000 faststream-0.5.2/faststream/utils/functions.py
+-rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 faststream-0.5.2/faststream/utils/no_cast.py
+-rw-r--r--   0        0        0     1317 2020-02-02 00:00:00.000000 faststream-0.5.2/faststream/utils/path.py
+-rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 faststream-0.5.2/faststream/utils/context/__init__.py
+-rw-r--r--   0        0        0      966 2020-02-02 00:00:00.000000 faststream-0.5.2/faststream/utils/context/builders.py
+-rw-r--r--   0        0        0     5117 2020-02-02 00:00:00.000000 faststream-0.5.2/faststream/utils/context/repository.py
+-rw-r--r--   0        0        0     2536 2020-02-02 00:00:00.000000 faststream-0.5.2/faststream/utils/context/types.py
+-rwxr-xr-x   0        0        0      915 2020-02-02 00:00:00.000000 faststream-0.5.2/scripts/build-docs-pre-commit.sh
+-rwxr-xr-x   0        0        0       66 2020-02-02 00:00:00.000000 faststream-0.5.2/scripts/build-docs.sh
+-rwxr-xr-x   0        0        0      909 2020-02-02 00:00:00.000000 faststream-0.5.2/scripts/lint-pre-commit.sh
+-rwxr-xr-x   0        0        0      247 2020-02-02 00:00:00.000000 faststream-0.5.2/scripts/lint.sh
+-rwxr-xr-x   0        0        0       51 2020-02-02 00:00:00.000000 faststream-0.5.2/scripts/publish.sh
+-rwxr-xr-x   0        0        0       70 2020-02-02 00:00:00.000000 faststream-0.5.2/scripts/serve-docs.sh
+-rwxr-xr-x   0        0        0      522 2020-02-02 00:00:00.000000 faststream-0.5.2/scripts/set_variables.sh
+-rwxr-xr-x   0        0        0      147 2020-02-02 00:00:00.000000 faststream-0.5.2/scripts/start_test_env.sh
+-rwxr-xr-x   0        0        0      175 2020-02-02 00:00:00.000000 faststream-0.5.2/scripts/static-analysis.sh
+-rwxr-xr-x   0        0        0      926 2020-02-02 00:00:00.000000 faststream-0.5.2/scripts/static-pre-commit.sh
+-rwxr-xr-x   0        0        0      132 2020-02-02 00:00:00.000000 faststream-0.5.2/scripts/stop_test_env.sh
+-rwxr-xr-x   0        0        0      154 2020-02-02 00:00:00.000000 faststream-0.5.2/scripts/test-cov.sh
+-rwxr-xr-x   0        0        0      131 2020-02-02 00:00:00.000000 faststream-0.5.2/scripts/test.sh
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 faststream-0.5.2/.gitignore
+-rw-r--r--   0        0        0    11363 2020-02-02 00:00:00.000000 faststream-0.5.2/LICENSE
+-rw-r--r--   0        0        0    14865 2020-02-02 00:00:00.000000 faststream-0.5.2/README.md
+-rw-r--r--   0        0        0    10330 2020-02-02 00:00:00.000000 faststream-0.5.2/pyproject.toml
+-rw-r--r--   0        0        0    22988 2020-02-02 00:00:00.000000 faststream-0.5.2/PKG-INFO
```

### Comparing `faststream-0.5.1/.pre-commit-config.yaml` & `faststream-0.5.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `faststream-0.5.1/.secrets.baseline` & `faststream-0.5.2/.secrets.baseline`

 * *Files identical despite different names*

### Comparing `faststream-0.5.1/CITATION.cff` & `faststream-0.5.2/CITATION.cff`

 * *Files identical despite different names*

### Comparing `faststream-0.5.1/CODE_OF_CONDUCT.md` & `faststream-0.5.2/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `faststream-0.5.1/CONTRIBUTING.md` & `faststream-0.5.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `faststream-0.5.1/SECURITY.md` & `faststream-0.5.2/SECURITY.md`

 * *Files identical despite different names*

### Comparing `faststream-0.5.1/.github/PULL_REQUEST_TEMPLATE.md` & `faststream-0.5.2/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `faststream-0.5.1/.github/dependabot.yml` & `faststream-0.5.2/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `faststream-0.5.1/.github/ISSUE_TEMPLATE/bug_report.md` & `faststream-0.5.2/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `faststream-0.5.1/.github/ISSUE_TEMPLATE/feature_request.md` & `faststream-0.5.2/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `faststream-0.5.1/.github/workflows/check-broken-links-in-docs.yaml` & `faststream-0.5.2/.github/workflows/check-broken-links-in-docs.yaml`

 * *Files identical despite different names*

### Comparing `faststream-0.5.1/.github/workflows/codeql.yml` & `faststream-0.5.2/.github/workflows/codeql.yml`

 * *Files identical despite different names*

### Comparing `faststream-0.5.1/.github/workflows/dependency-review.yaml` & `faststream-0.5.2/.github/workflows/dependency-review.yaml`

 * *Files identical despite different names*

### Comparing `faststream-0.5.1/.github/workflows/deploy-docs.yaml` & `faststream-0.5.2/.github/workflows/deploy-docs.yaml`

 * *Files identical despite different names*

### Comparing `faststream-0.5.1/.github/workflows/publish_coverage.yml` & `faststream-0.5.2/.github/workflows/publish_coverage.yml`

 * *Files identical despite different names*

### Comparing `faststream-0.5.1/.github/workflows/publish_pypi.yml` & `faststream-0.5.2/.github/workflows/publish_pypi.yml`

 * *Files identical despite different names*

### Comparing `faststream-0.5.1/.github/workflows/test.yaml` & `faststream-0.5.2/.github/workflows/test.yaml`

 * *Files identical despite different names*

### Comparing `faststream-0.5.1/.github/workflows/update_release_notes.yaml` & `faststream-0.5.2/.github/workflows/update_release_notes.yaml`

 * *Files identical despite different names*

### Comparing `faststream-0.5.1/examples/e02_1_basic_publisher.py` & `faststream-0.5.2/examples/e02_1_basic_publisher.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.1/examples/e02_2_basic_publisher.py` & `faststream-0.5.2/examples/e02_2_basic_publisher.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.1/examples/e02_3_basic_publisher.py` & `faststream-0.5.2/examples/e02_3_basic_publisher.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.1/examples/e03_miltiple_pubsub.py` & `faststream-0.5.2/examples/e03_miltiple_pubsub.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.1/examples/e04_msg_filter.py` & `faststream-0.5.2/examples/e04_msg_filter.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.1/examples/e07_ack_immediately.py` & `faststream-0.5.2/examples/e07_ack_immediately.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.1/examples/e09_testing_mocks.py` & `faststream-0.5.2/examples/e09_testing_mocks.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.1/examples/e10_middlewares.py` & `faststream-0.5.2/examples/e10_middlewares.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.1/examples/e11_settings.py` & `faststream-0.5.2/examples/e11_settings.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.1/examples/fastapi_integration/testing.py` & `faststream-0.5.2/examples/fastapi_integration/testing.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.1/examples/howto/structlogs.py` & `faststream-0.5.2/examples/howto/structlogs.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.1/examples/kafka/testing.py` & `faststream-0.5.2/examples/kafka/testing.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.1/examples/nats/e03_publisher.py` & `faststream-0.5.2/examples/nats/e03_publisher.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.1/examples/nats/e04_js_basic.py` & `faststream-0.5.2/examples/nats/e04_js_basic.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.1/examples/nats/e05_basic_and_js.py` & `faststream-0.5.2/examples/nats/e05_basic_and_js.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.1/examples/nats/e06_key_value.py` & `faststream-0.5.2/examples/nats/e06_key_value.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.1/examples/nats/e07_object_storage.py` & `faststream-0.5.2/examples/nats/e07_object_storage.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.1/examples/rabbit/direct.py` & `faststream-0.5.2/examples/rabbit/direct.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.1/examples/rabbit/fanout.py` & `faststream-0.5.2/examples/rabbit/fanout.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.1/examples/rabbit/header.py` & `faststream-0.5.2/examples/rabbit/header.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.1/examples/rabbit/topic.py` & `faststream-0.5.2/examples/rabbit/topic.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.1/examples/redis/channel_sub_pattern.py` & `faststream-0.5.2/examples/redis/channel_sub_pattern.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.1/examples/redis/rpc.py` & `faststream-0.5.2/examples/redis/rpc.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.1/examples/router/basic_publish.py` & `faststream-0.5.2/examples/router/basic_publish.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.1/examples/serialization/avro/avro.py` & `faststream-0.5.2/examples/serialization/avro/avro.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.1/examples/serialization/msgpack/pack.py` & `faststream-0.5.2/examples/serialization/msgpack/pack.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.1/examples/serialization/protobuf/protobuf.py` & `faststream-0.5.2/examples/serialization/protobuf/protobuf.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.1/faststream/__init__.py` & `faststream-0.5.2/faststream/__init__.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.1/faststream/_compat.py` & `faststream-0.5.2/faststream/_compat.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.1/faststream/app.py` & `faststream-0.5.2/faststream/app.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.1/faststream/exceptions.py` & `faststream-0.5.2/faststream/exceptions.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.1/faststream/security.py` & `faststream-0.5.2/faststream/security.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.1/faststream/types.py` & `faststream-0.5.2/faststream/types.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.1/faststream/asyncapi/abc.py` & `faststream-0.5.2/faststream/asyncapi/abc.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.1/faststream/asyncapi/generate.py` & `faststream-0.5.2/faststream/asyncapi/generate.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.1/faststream/asyncapi/message.py` & `faststream-0.5.2/faststream/asyncapi/message.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.1/faststream/asyncapi/proto.py` & `faststream-0.5.2/faststream/asyncapi/proto.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.1/faststream/asyncapi/site.py` & `faststream-0.5.2/faststream/asyncapi/site.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.1/faststream/asyncapi/utils.py` & `faststream-0.5.2/faststream/asyncapi/utils.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.1/faststream/asyncapi/schema/__init__.py` & `faststream-0.5.2/faststream/asyncapi/schema/__init__.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.1/faststream/asyncapi/schema/channels.py` & `faststream-0.5.2/faststream/asyncapi/schema/channels.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.1/faststream/asyncapi/schema/info.py` & `faststream-0.5.2/faststream/asyncapi/schema/info.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.1/faststream/asyncapi/schema/main.py` & `faststream-0.5.2/faststream/asyncapi/schema/main.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.1/faststream/asyncapi/schema/message.py` & `faststream-0.5.2/faststream/asyncapi/schema/message.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.1/faststream/asyncapi/schema/operations.py` & `faststream-0.5.2/faststream/asyncapi/schema/operations.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.1/faststream/asyncapi/schema/security.py` & `faststream-0.5.2/faststream/asyncapi/schema/security.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.1/faststream/asyncapi/schema/servers.py` & `faststream-0.5.2/faststream/asyncapi/schema/servers.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.1/faststream/asyncapi/schema/utils.py` & `faststream-0.5.2/faststream/asyncapi/schema/utils.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.1/faststream/asyncapi/schema/bindings/amqp.py` & `faststream-0.5.2/faststream/asyncapi/schema/bindings/amqp.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.1/faststream/asyncapi/schema/bindings/kafka.py` & `faststream-0.5.2/faststream/asyncapi/schema/bindings/kafka.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.1/faststream/asyncapi/schema/bindings/main.py` & `faststream-0.5.2/faststream/asyncapi/schema/bindings/main.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.1/faststream/asyncapi/schema/bindings/nats.py` & `faststream-0.5.2/faststream/asyncapi/schema/bindings/nats.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.1/faststream/asyncapi/schema/bindings/redis.py` & `faststream-0.5.2/faststream/asyncapi/schema/bindings/redis.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.1/faststream/asyncapi/schema/bindings/sqs.py` & `faststream-0.5.2/faststream/asyncapi/schema/bindings/sqs.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.1/faststream/broker/acknowledgement_watcher.py` & `faststream-0.5.2/faststream/broker/acknowledgement_watcher.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.1/faststream/broker/message.py` & `faststream-0.5.2/faststream/broker/message.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.1/faststream/broker/router.py` & `faststream-0.5.2/faststream/broker/router.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.1/faststream/broker/schemas.py` & `faststream-0.5.2/faststream/broker/schemas.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.1/faststream/broker/types.py` & `faststream-0.5.2/faststream/broker/types.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.1/faststream/broker/utils.py` & `faststream-0.5.2/faststream/broker/utils.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.1/faststream/broker/core/abc.py` & `faststream-0.5.2/faststream/broker/core/abc.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.1/faststream/broker/core/logging.py` & `faststream-0.5.2/faststream/broker/core/logging.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.1/faststream/broker/core/usecase.py` & `faststream-0.5.2/faststream/broker/core/usecase.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.1/faststream/broker/fastapi/context.py` & `faststream-0.5.2/faststream/broker/fastapi/context.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.1/faststream/broker/fastapi/get_dependant.py` & `faststream-0.5.2/faststream/broker/fastapi/get_dependant.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.1/faststream/broker/fastapi/route.py` & `faststream-0.5.2/faststream/broker/fastapi/route.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.1/faststream/broker/fastapi/router.py` & `faststream-0.5.2/faststream/broker/fastapi/router.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.1/faststream/broker/middlewares/base.py` & `faststream-0.5.2/faststream/broker/middlewares/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,23 +55,22 @@
 
     async def consume_scope(
         self,
         call_next: "AsyncFuncAny",
         msg: "StreamMessage[Any]",
     ) -> Any:
         """Asynchronously consumes a message and returns an asynchronous iterator of decoded messages."""
-        err: Optional[Exception]
+        err: Optional[Exception] = None
         try:
             result = await call_next(await self.on_consume(msg))
 
         except Exception as e:
             err = e
 
         else:
-            err = None
             return result
 
         finally:
             await self.after_consume(err)
 
     async def on_publish(
         self,
```

### Comparing `faststream-0.5.1/faststream/broker/middlewares/logging.py` & `faststream-0.5.2/faststream/broker/middlewares/logging.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.1/faststream/broker/publisher/fake.py` & `faststream-0.5.2/faststream/broker/publisher/fake.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.1/faststream/broker/publisher/proto.py` & `faststream-0.5.2/faststream/broker/publisher/proto.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.1/faststream/broker/publisher/usecase.py` & `faststream-0.5.2/faststream/broker/publisher/usecase.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.1/faststream/broker/subscriber/call_item.py` & `faststream-0.5.2/faststream/broker/subscriber/call_item.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.1/faststream/broker/subscriber/proto.py` & `faststream-0.5.2/faststream/broker/subscriber/proto.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.1/faststream/broker/subscriber/usecase.py` & `faststream-0.5.2/faststream/broker/subscriber/usecase.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.1/faststream/broker/wrapper/call.py` & `faststream-0.5.2/faststream/broker/wrapper/call.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.1/faststream/broker/wrapper/proto.py` & `faststream-0.5.2/faststream/broker/wrapper/proto.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.1/faststream/cli/main.py` & `faststream-0.5.2/faststream/cli/main.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.1/faststream/cli/docs/app.py` & `faststream-0.5.2/faststream/cli/docs/app.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.1/faststream/cli/supervisors/basereload.py` & `faststream-0.5.2/faststream/cli/supervisors/basereload.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.1/faststream/cli/supervisors/multiprocess.py` & `faststream-0.5.2/faststream/cli/supervisors/multiprocess.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.1/faststream/cli/supervisors/utils.py` & `faststream-0.5.2/faststream/cli/supervisors/utils.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.1/faststream/cli/supervisors/watchfiles.py` & `faststream-0.5.2/faststream/cli/supervisors/watchfiles.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.1/faststream/cli/utils/imports.py` & `faststream-0.5.2/faststream/cli/utils/imports.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.1/faststream/cli/utils/logs.py` & `faststream-0.5.2/faststream/cli/utils/logs.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.1/faststream/cli/utils/parser.py` & `faststream-0.5.2/faststream/cli/utils/parser.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.1/faststream/confluent/annotations.py` & `faststream-0.5.2/faststream/confluent/annotations.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.1/faststream/confluent/client.py` & `faststream-0.5.2/faststream/confluent/client.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.1/faststream/confluent/message.py` & `faststream-0.5.2/faststream/confluent/message.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.1/faststream/confluent/parser.py` & `faststream-0.5.2/faststream/confluent/parser.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.1/faststream/confluent/router.py` & `faststream-0.5.2/faststream/confluent/router.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.1/faststream/confluent/security.py` & `faststream-0.5.2/faststream/confluent/security.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.1/faststream/confluent/testing.py` & `faststream-0.5.2/faststream/confluent/testing.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.1/faststream/confluent/broker/broker.py` & `faststream-0.5.2/faststream/confluent/broker/broker.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.1/faststream/confluent/broker/logging.py` & `faststream-0.5.2/faststream/confluent/broker/logging.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.1/faststream/confluent/broker/registrator.py` & `faststream-0.5.2/faststream/confluent/broker/registrator.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.1/faststream/confluent/fastapi/__init__.py` & `faststream-0.5.2/faststream/confluent/fastapi/__init__.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.1/faststream/confluent/fastapi/fastapi.py` & `faststream-0.5.2/faststream/confluent/fastapi/fastapi.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.1/faststream/confluent/publisher/asyncapi.py` & `faststream-0.5.2/faststream/confluent/publisher/asyncapi.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.1/faststream/confluent/publisher/producer.py` & `faststream-0.5.2/faststream/confluent/publisher/producer.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.1/faststream/confluent/publisher/usecase.py` & `faststream-0.5.2/faststream/confluent/publisher/usecase.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.1/faststream/confluent/schemas/params.py` & `faststream-0.5.2/faststream/confluent/schemas/params.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.1/faststream/confluent/subscriber/asyncapi.py` & `faststream-0.5.2/faststream/confluent/subscriber/asyncapi.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.1/faststream/confluent/subscriber/usecase.py` & `faststream-0.5.2/faststream/confluent/subscriber/usecase.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.1/faststream/kafka/annotations.py` & `faststream-0.5.2/faststream/kafka/annotations.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.1/faststream/kafka/message.py` & `faststream-0.5.2/faststream/kafka/message.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.1/faststream/kafka/parser.py` & `faststream-0.5.2/faststream/kafka/parser.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.1/faststream/kafka/router.py` & `faststream-0.5.2/faststream/kafka/router.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.1/faststream/kafka/security.py` & `faststream-0.5.2/faststream/kafka/security.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.1/faststream/kafka/testing.py` & `faststream-0.5.2/faststream/kafka/testing.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.1/faststream/kafka/broker/broker.py` & `faststream-0.5.2/faststream/kafka/broker/broker.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.1/faststream/kafka/broker/logging.py` & `faststream-0.5.2/faststream/kafka/broker/logging.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.1/faststream/kafka/broker/registrator.py` & `faststream-0.5.2/faststream/kafka/broker/registrator.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.1/faststream/kafka/fastapi/__init__.py` & `faststream-0.5.2/faststream/kafka/fastapi/__init__.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.1/faststream/kafka/fastapi/fastapi.py` & `faststream-0.5.2/faststream/kafka/fastapi/fastapi.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.1/faststream/kafka/publisher/asyncapi.py` & `faststream-0.5.2/faststream/kafka/publisher/asyncapi.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.1/faststream/kafka/publisher/producer.py` & `faststream-0.5.2/faststream/kafka/publisher/producer.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.1/faststream/kafka/publisher/usecase.py` & `faststream-0.5.2/faststream/kafka/publisher/usecase.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.1/faststream/kafka/schemas/params.py` & `faststream-0.5.2/faststream/kafka/schemas/params.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.1/faststream/kafka/subscriber/asyncapi.py` & `faststream-0.5.2/faststream/kafka/subscriber/asyncapi.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.1/faststream/kafka/subscriber/usecase.py` & `faststream-0.5.2/faststream/kafka/subscriber/usecase.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.1/faststream/log/formatter.py` & `faststream-0.5.2/faststream/log/formatter.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.1/faststream/log/logging.py` & `faststream-0.5.2/faststream/log/logging.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.1/faststream/nats/__init__.py` & `faststream-0.5.2/faststream/nats/__init__.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.1/faststream/nats/annotations.py` & `faststream-0.5.2/faststream/nats/annotations.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.1/faststream/nats/helpers.py` & `faststream-0.5.2/faststream/nats/helpers.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.1/faststream/nats/message.py` & `faststream-0.5.2/faststream/nats/message.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.1/faststream/nats/parser.py` & `faststream-0.5.2/faststream/nats/parser.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.1/faststream/nats/router.py` & `faststream-0.5.2/faststream/nats/router.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.1/faststream/nats/security.py` & `faststream-0.5.2/faststream/nats/security.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.1/faststream/nats/testing.py` & `faststream-0.5.2/faststream/nats/testing.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.1/faststream/nats/broker/broker.py` & `faststream-0.5.2/faststream/nats/broker/broker.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.1/faststream/nats/broker/logging.py` & `faststream-0.5.2/faststream/nats/broker/logging.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.1/faststream/nats/broker/registrator.py` & `faststream-0.5.2/faststream/nats/broker/registrator.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.1/faststream/nats/fastapi/__init__.py` & `faststream-0.5.2/faststream/nats/fastapi/__init__.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.1/faststream/nats/fastapi/fastapi.py` & `faststream-0.5.2/faststream/nats/fastapi/fastapi.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.1/faststream/nats/publisher/asyncapi.py` & `faststream-0.5.2/faststream/nats/publisher/asyncapi.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.1/faststream/nats/publisher/producer.py` & `faststream-0.5.2/faststream/nats/publisher/producer.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.1/faststream/nats/publisher/usecase.py` & `faststream-0.5.2/faststream/nats/publisher/usecase.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.1/faststream/nats/schemas/js_stream.py` & `faststream-0.5.2/faststream/nats/schemas/js_stream.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.1/faststream/nats/schemas/pull_sub.py` & `faststream-0.5.2/faststream/nats/schemas/pull_sub.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.1/faststream/nats/subscriber/asyncapi.py` & `faststream-0.5.2/faststream/nats/subscriber/asyncapi.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.1/faststream/nats/subscriber/usecase.py` & `faststream-0.5.2/faststream/nats/subscriber/usecase.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.1/faststream/rabbit/__init__.py` & `faststream-0.5.2/faststream/rabbit/__init__.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.1/faststream/rabbit/annotations.py` & `faststream-0.5.2/faststream/rabbit/annotations.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.1/faststream/rabbit/message.py` & `faststream-0.5.2/faststream/rabbit/message.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.1/faststream/rabbit/parser.py` & `faststream-0.5.2/faststream/rabbit/parser.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.1/faststream/rabbit/router.py` & `faststream-0.5.2/faststream/rabbit/router.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.1/faststream/rabbit/security.py` & `faststream-0.5.2/faststream/rabbit/security.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.1/faststream/rabbit/testing.py` & `faststream-0.5.2/faststream/rabbit/testing.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.1/faststream/rabbit/utils.py` & `faststream-0.5.2/faststream/rabbit/utils.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.1/faststream/rabbit/broker/broker.py` & `faststream-0.5.2/faststream/rabbit/broker/broker.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.1/faststream/rabbit/broker/logging.py` & `faststream-0.5.2/faststream/rabbit/broker/logging.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.1/faststream/rabbit/broker/registrator.py` & `faststream-0.5.2/faststream/rabbit/broker/registrator.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.1/faststream/rabbit/fastapi/__init__.py` & `faststream-0.5.2/faststream/rabbit/fastapi/__init__.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.1/faststream/rabbit/fastapi/router.py` & `faststream-0.5.2/faststream/rabbit/fastapi/router.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.1/faststream/rabbit/publisher/asyncapi.py` & `faststream-0.5.2/faststream/rabbit/publisher/asyncapi.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.1/faststream/rabbit/publisher/producer.py` & `faststream-0.5.2/faststream/rabbit/publisher/producer.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.1/faststream/rabbit/publisher/usecase.py` & `faststream-0.5.2/faststream/rabbit/publisher/usecase.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.1/faststream/rabbit/schemas/constants.py` & `faststream-0.5.2/faststream/rabbit/schemas/constants.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.1/faststream/rabbit/schemas/exchange.py` & `faststream-0.5.2/faststream/rabbit/schemas/exchange.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.1/faststream/rabbit/schemas/queue.py` & `faststream-0.5.2/faststream/rabbit/schemas/queue.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.1/faststream/rabbit/schemas/reply.py` & `faststream-0.5.2/faststream/rabbit/schemas/reply.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.1/faststream/rabbit/subscriber/asyncapi.py` & `faststream-0.5.2/faststream/rabbit/subscriber/asyncapi.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.1/faststream/rabbit/subscriber/usecase.py` & `faststream-0.5.2/faststream/rabbit/subscriber/usecase.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.1/faststream/redis/__init__.py` & `faststream-0.5.2/faststream/redis/__init__.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.1/faststream/redis/annotations.py` & `faststream-0.5.2/faststream/redis/annotations.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.1/faststream/redis/message.py` & `faststream-0.5.2/faststream/redis/message.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.1/faststream/redis/parser.py` & `faststream-0.5.2/faststream/redis/parser.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.1/faststream/redis/router.py` & `faststream-0.5.2/faststream/redis/router.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.1/faststream/redis/security.py` & `faststream-0.5.2/faststream/redis/security.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.1/faststream/redis/testing.py` & `faststream-0.5.2/faststream/redis/testing.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.1/faststream/redis/broker/broker.py` & `faststream-0.5.2/faststream/redis/broker/broker.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.1/faststream/redis/broker/logging.py` & `faststream-0.5.2/faststream/redis/broker/logging.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.1/faststream/redis/broker/registrator.py` & `faststream-0.5.2/faststream/redis/broker/registrator.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.1/faststream/redis/fastapi/__init__.py` & `faststream-0.5.2/faststream/redis/fastapi/__init__.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.1/faststream/redis/fastapi/fastapi.py` & `faststream-0.5.2/faststream/redis/fastapi/fastapi.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,32 +65,32 @@
     broker: RB
 
     def __init__(
         self,
         url: str = "redis://localhost:6379",
         polling_interval: Optional[float] = None,
         *,
-        host: str = "localhost",
-        port: Union[str, int] = 6379,
-        db: Union[str, int] = 0,
+        host: Union[str, object] = Parameter.empty,
+        port: Union[str, int, object] = Parameter.empty,
+        db: Union[str, int, object] = Parameter.empty,
+        connection_class: Union[Type["Connection"], object] = Parameter.empty,
         client_name: Optional[str] = SERVICE_NAME,
         health_check_interval: float = 0,
         max_connections: Optional[int] = None,
         socket_timeout: Optional[float] = None,
         socket_connect_timeout: Optional[float] = None,
         socket_read_size: int = 65536,
         socket_keepalive: bool = False,
         socket_keepalive_options: Optional[Mapping[int, Union[int, bytes]]] = None,
         socket_type: int = 0,
         retry_on_timeout: bool = False,
         encoding: str = "utf-8",
         encoding_errors: str = "strict",
         decode_responses: bool = False,
         parser_class: Type["BaseParser"] = DefaultParser,
-        connection_class: Type["Connection"] = Connection,
         encoder_class: Type["Encoder"] = Encoder,
         # broker base args
         graceful_timeout: Annotated[
             Optional[float],
             Doc(
                 "Graceful shutdown timeout. Broker waits for all running subscribers completion before shut down."
             ),
```

### Comparing `faststream-0.5.1/faststream/redis/publisher/asyncapi.py` & `faststream-0.5.2/faststream/redis/publisher/asyncapi.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.1/faststream/redis/publisher/producer.py` & `faststream-0.5.2/faststream/redis/publisher/producer.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.1/faststream/redis/publisher/usecase.py` & `faststream-0.5.2/faststream/redis/publisher/usecase.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.1/faststream/redis/schemas/list_sub.py` & `faststream-0.5.2/faststream/redis/schemas/list_sub.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.1/faststream/redis/schemas/proto.py` & `faststream-0.5.2/faststream/redis/schemas/proto.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.1/faststream/redis/schemas/pub_sub.py` & `faststream-0.5.2/faststream/redis/schemas/pub_sub.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.1/faststream/redis/schemas/stream_sub.py` & `faststream-0.5.2/faststream/redis/schemas/stream_sub.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.1/faststream/redis/subscriber/asyncapi.py` & `faststream-0.5.2/faststream/redis/subscriber/asyncapi.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.1/faststream/redis/subscriber/usecase.py` & `faststream-0.5.2/faststream/redis/subscriber/usecase.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.1/faststream/testing/app.py` & `faststream-0.5.2/faststream/testing/app.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.1/faststream/testing/broker.py` & `faststream-0.5.2/faststream/testing/broker.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.1/faststream/utils/ast.py` & `faststream-0.5.2/faststream/utils/ast.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.1/faststream/utils/classes.py` & `faststream-0.5.2/faststream/utils/classes.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.1/faststream/utils/data.py` & `faststream-0.5.2/faststream/utils/data.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.1/faststream/utils/functions.py` & `faststream-0.5.2/faststream/utils/functions.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.1/faststream/utils/no_cast.py` & `faststream-0.5.2/faststream/utils/no_cast.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.1/faststream/utils/path.py` & `faststream-0.5.2/faststream/utils/path.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.1/faststream/utils/context/builders.py` & `faststream-0.5.2/faststream/utils/context/builders.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.1/faststream/utils/context/repository.py` & `faststream-0.5.2/faststream/utils/context/repository.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.1/faststream/utils/context/types.py` & `faststream-0.5.2/faststream/utils/context/types.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.1/scripts/build-docs-pre-commit.sh` & `faststream-0.5.2/scripts/build-docs-pre-commit.sh`

 * *Files identical despite different names*

### Comparing `faststream-0.5.1/scripts/lint-pre-commit.sh` & `faststream-0.5.2/scripts/lint-pre-commit.sh`

 * *Files identical despite different names*

### Comparing `faststream-0.5.1/scripts/set_variables.sh` & `faststream-0.5.2/scripts/set_variables.sh`

 * *Files identical despite different names*

### Comparing `faststream-0.5.1/scripts/static-pre-commit.sh` & `faststream-0.5.2/scripts/static-pre-commit.sh`

 * *Files identical despite different names*

### Comparing `faststream-0.5.1/LICENSE` & `faststream-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `faststream-0.5.1/README.md` & `faststream-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `faststream-0.5.1/pyproject.toml` & `faststream-0.5.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `faststream-0.5.1/PKG-INFO` & `faststream-0.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: faststream
-Version: 0.5.1
+Version: 0.5.2
 Summary: FastStream: the simplest way to work with a messaging queues
 Project-URL: Homepage, https://faststream.airt.ai/latest/
 Project-URL: Documentation, https://faststream.airt.ai/latest/getting-started/
 Project-URL: Tracker, https://github.com/airtai/FastStream/issues
 Project-URL: Source, https://github.com/airtai/FastStream
 Project-URL: Discord, https://discord.gg/qFm6aSqq59
 Author-email: airt <info@airt.ai>, Nikita Pastukhov <nikita@pastukhov-dev.ru>
```

