# Comparing `tmp/pypz-kafka-io-0.9.0b9.tar.gz` & `tmp/pypz_kafka_io-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypz-kafka-io-0.9.0b9.tar", last modified: Tue Feb 13 09:32:46 2024, max compression
+gzip compressed data, was "pypz_kafka_io-0.9.1.tar", last modified: Thu Apr 18 05:48:43 2024, max compression
```

## Comparing `pypz-kafka-io-0.9.0b9.tar` & `pypz_kafka_io-0.9.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:32:46.498227 pypz-kafka-io-0.9.0b9/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-02-13 09:32:32.000000 pypz-kafka-io-0.9.0b9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2401 2024-02-13 09:32:46.498227 pypz-kafka-io-0.9.0b9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-02-13 09:32:32.000000 pypz-kafka-io-0.9.0b9/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      757 2024-02-13 09:32:32.000000 pypz-kafka-io-0.9.0b9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-13 09:32:46.498227 pypz-kafka-io-0.9.0b9/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:32:46.494227 pypz-kafka-io-0.9.0b9/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:32:46.494227 pypz-kafka-io-0.9.0b9/src/pypz/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:32:46.494227 pypz-kafka-io-0.9.0b9/src/pypz/plugins/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:32:46.494227 pypz-kafka-io-0.9.0b9/src/pypz/plugins/kafka_io/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 09:32:32.000000 pypz-kafka-io-0.9.0b9/src/pypz/plugins/kafka_io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    28881 2024-02-13 09:32:32.000000 pypz-kafka-io-0.9.0b9/src/pypz/plugins/kafka_io/channels.py
--rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-02-13 09:32:32.000000 pypz-kafka-io-0.9.0b9/src/pypz/plugins/kafka_io/ports.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 09:32:46.498227 pypz-kafka-io-0.9.0b9/src/pypz_kafka_io.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2401 2024-02-13 09:32:46.000000 pypz-kafka-io-0.9.0b9/src/pypz_kafka_io.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-02-13 09:32:46.000000 pypz-kafka-io-0.9.0b9/src/pypz_kafka_io.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-13 09:32:46.000000 pypz-kafka-io-0.9.0b9/src/pypz_kafka_io.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-02-13 09:32:46.000000 pypz-kafka-io-0.9.0b9/src/pypz_kafka_io.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-02-13 09:32:46.000000 pypz-kafka-io-0.9.0b9/src/pypz_kafka_io.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 05:48:43.531407 pypz_kafka_io-0.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-18 05:48:37.000000 pypz_kafka_io-0.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2619 2024-04-18 05:48:43.531407 pypz_kafka_io-0.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-04-18 05:48:37.000000 pypz_kafka_io-0.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      897 2024-04-18 05:48:37.000000 pypz_kafka_io-0.9.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 05:48:43.531407 pypz_kafka_io-0.9.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 05:48:43.527408 pypz_kafka_io-0.9.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 05:48:43.527408 pypz_kafka_io-0.9.1/src/pypz/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 05:48:43.527408 pypz_kafka_io-0.9.1/src/pypz/plugins/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 05:48:43.527408 pypz_kafka_io-0.9.1/src/pypz/plugins/kafka_io/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 05:48:37.000000 pypz_kafka_io-0.9.1/src/pypz/plugins/kafka_io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28905 2024-04-18 05:48:37.000000 pypz_kafka_io-0.9.1/src/pypz/plugins/kafka_io/channels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-04-18 05:48:37.000000 pypz_kafka_io-0.9.1/src/pypz/plugins/kafka_io/ports.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 05:48:43.531407 pypz_kafka_io-0.9.1/src/pypz_kafka_io.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2619 2024-04-18 05:48:43.000000 pypz_kafka_io-0.9.1/src/pypz_kafka_io.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-04-18 05:48:43.000000 pypz_kafka_io-0.9.1/src/pypz_kafka_io.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 05:48:43.000000 pypz_kafka_io-0.9.1/src/pypz_kafka_io.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-18 05:48:43.000000 pypz_kafka_io-0.9.1/src/pypz_kafka_io.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-18 05:48:43.000000 pypz_kafka_io-0.9.1/src/pypz_kafka_io.egg-info/top_level.txt
```

### Comparing `pypz-kafka-io-0.9.0b9/LICENSE` & `pypz_kafka_io-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pypz-kafka-io-0.9.0b9/PKG-INFO` & `pypz_kafka_io-0.9.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,29 @@
 Metadata-Version: 2.1
 Name: pypz-kafka-io
-Version: 0.9.0b9
+Version: 0.9.1
 Summary: Provides a Kafka implementation of the ChannelInput/OutputPort in pypz.
 Author-email: Laszlo Anka <laszlo.anka@gmail.com>
 License: Apache-2.0
 Keywords: pypz,plugin,kafka
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pypz-core
 Requires-Dist: avro==1.10.1
 Requires-Dist: kafka-python==2.0.2
 Requires-Dist: avro-validator==1.2.1
+Provides-Extra: static
+Requires-Dist: flake8~=7.0.0; extra == "static"
+Requires-Dist: flake8-html~=0.4.3; extra == "static"
+Requires-Dist: mypy~=1.8.0; extra == "static"
+Requires-Dist: coverage~=7.4.1; extra == "static"
 
 # Description
 
 This package contains the Kafka implementation of the Input-/OutputPortPlugin 
 interface of *pypz*. It enables the operators to send and receive data records
 in a real streaming fashion.
```

### Comparing `pypz-kafka-io-0.9.0b9/README.md` & `pypz_kafka_io-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `pypz-kafka-io-0.9.0b9/pyproject.toml` & `pypz_kafka_io-0.9.1/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=68.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pypz-kafka-io"
-version = "0.9.0b9"
+version = "0.9.1"
 authors = [
     { name = "Laszlo Anka", email = "laszlo.anka@gmail.com" }
 ]
 description = "Provides a Kafka implementation of the ChannelInput/OutputPort in pypz."
 readme = "README.md"
 license = { text = "Apache-2.0" }
 requires-python = ">=3.11"
@@ -25,10 +25,18 @@
 dependencies = [
     "pypz-core",
     "avro==1.10.1",
     "kafka-python==2.0.2",
     "avro-validator==1.2.1"
 ]
 
+[project.optional-dependencies]
+static = [
+    "flake8 ~= 7.0.0",
+    "flake8-html ~= 0.4.3",
+    "mypy ~= 1.8.0",
+    "coverage ~= 7.4.1"
+]
+
 [tool.setuptools.packages.find]
 where = ["src"]
 namespaces = true
```

### Comparing `pypz-kafka-io-0.9.0b9/src/pypz/plugins/kafka_io/channels.py` & `pypz_kafka_io-0.9.1/src/pypz/plugins/kafka_io/channels.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 
     # ======================= Static fields =======================
 
     # ======================= ctor =======================
 
     def __init__(self, channel_name: str,
                  context: 'OutputPortPlugin',
-                 executor: concurrent.futures.ThreadPoolExecutor = None,
+                 executor: Optional[concurrent.futures.ThreadPoolExecutor] = None,
                  **kwargs):
         super().__init__(channel_name, context, executor, **kwargs)
 
         self._data_producer: Optional[KafkaProducer] = None
         """
         Data producer, responsible to produce data received by the plugin
         """
@@ -110,16 +110,16 @@
         self._admin_client: Optional[KafkaAdminClient] = None
         """
         Kafka admin client. Necessary to create/delete topics.
         """
 
         self._round_robin_partition_idx: int = 0
         """
-        This index ensures that we produce in a true round robin fashion. It is necessary,
-        since Kafka's round robin considers batches of records instead of simple records
+        This index ensures that we produce in a true round-robin fashion. It is necessary,
+        since Kafka's round-robin considers batches of records instead of simple records
         """
 
         self._target_partition_count: int = 1
         """
         The number of partitions of the topic that is created by the channel reader. This
         value will be read from the Kafka directly.
         """
@@ -311,15 +311,15 @@
 
     DataConsumerTimeoutInMs = 5000
 
     StatusConsumerTimeoutInMs = 1000
 
     def __init__(self, channel_name: str,
                  context: 'InputPortPlugin',
-                 executor: concurrent.futures.ThreadPoolExecutor = None,
+                 executor: Optional[concurrent.futures.ThreadPoolExecutor] = None,
                  **kwargs):
         super().__init__(channel_name, context, executor, **kwargs)
 
         self._data_consumer: Optional[KafkaConsumer] = None
         """
         This is a kafka consumer to poll data from the specified data topic.
         """
@@ -381,15 +381,15 @@
         The topic partition that this channel will read
         """
 
         self._partition_count: int = 1 if self._context.is_in_group_mode() else self._context.get_group_size()
         """
         The number of partitions to be created for the data channel. If group mode,
         then it shall be 1, since all the channel readers in the group will read all
-        the records sent to the channel. Otherwise it is the size of the group.
+        the records sent to the channel. Otherwise, it is the size of the group.
         """
 
         self._admin_client: Optional[KafkaAdminClient] = None
         """
         Kafka admin client. Necessary to check, whether topic is existing on retrieving 0 records on poll.
         """
 
@@ -667,11 +667,11 @@
             self._logger.warn(e)
             return False
 
     def get_consumer_lag(self) -> int:
         end_offsets = self._data_consumer.end_offsets([self._target_partition])
 
         overall_lag = 0
-        for topicPartition in end_offsets.keys():
-            overall_lag += (end_offsets[topicPartition] - self._data_consumer.position(topicPartition))
+        for topic_partition in end_offsets.keys():
+            overall_lag += (end_offsets[topic_partition] - self._data_consumer.position(topic_partition))
 
         return overall_lag
```

### Comparing `pypz-kafka-io-0.9.0b9/src/pypz/plugins/kafka_io/ports.py` & `pypz_kafka_io-0.9.1/src/pypz/plugins/kafka_io/ports.py`

 * *Files identical despite different names*

### Comparing `pypz-kafka-io-0.9.0b9/src/pypz_kafka_io.egg-info/PKG-INFO` & `pypz_kafka_io-0.9.1/src/pypz_kafka_io.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,29 @@
 Metadata-Version: 2.1
 Name: pypz-kafka-io
-Version: 0.9.0b9
+Version: 0.9.1
 Summary: Provides a Kafka implementation of the ChannelInput/OutputPort in pypz.
 Author-email: Laszlo Anka <laszlo.anka@gmail.com>
 License: Apache-2.0
 Keywords: pypz,plugin,kafka
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pypz-core
 Requires-Dist: avro==1.10.1
 Requires-Dist: kafka-python==2.0.2
 Requires-Dist: avro-validator==1.2.1
+Provides-Extra: static
+Requires-Dist: flake8~=7.0.0; extra == "static"
+Requires-Dist: flake8-html~=0.4.3; extra == "static"
+Requires-Dist: mypy~=1.8.0; extra == "static"
+Requires-Dist: coverage~=7.4.1; extra == "static"
 
 # Description
 
 This package contains the Kafka implementation of the Input-/OutputPortPlugin 
 interface of *pypz*. It enables the operators to send and receive data records
 in a real streaming fashion.
```

