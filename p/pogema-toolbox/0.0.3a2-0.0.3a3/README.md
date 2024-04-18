# Comparing `tmp/pogema-toolbox-0.0.3a2.tar.gz` & `tmp/pogema_toolbox-0.0.3a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pogema-toolbox-0.0.3a2.tar", last modified: Fri Apr 12 16:28:45 2024, max compression
+gzip compressed data, was "pogema_toolbox-0.0.3a3.tar", last modified: Thu Apr 18 12:54:41 2024, max compression
```

## Comparing `pogema-toolbox-0.0.3a2.tar` & `pogema_toolbox-0.0.3a3.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 skrynnik   (503) staff       (20)        0 2024-04-12 16:28:45.699344 pogema-toolbox-0.0.3a2/
--rw-r--r--   0 skrynnik   (503) staff       (20)    11345 2024-04-03 20:32:18.000000 pogema-toolbox-0.0.3a2/LICENSE
--rw-r--r--   0 skrynnik   (503) staff       (20)      720 2024-04-12 16:28:45.697795 pogema-toolbox-0.0.3a2/PKG-INFO
--rw-r--r--   0 skrynnik   (503) staff       (20)       16 2024-03-22 09:25:51.000000 pogema-toolbox-0.0.3a2/README.md
-drwxr-xr-x   0 skrynnik   (503) staff       (20)        0 2024-04-12 16:28:45.676026 pogema-toolbox-0.0.3a2/pogema_toolbox/
--rw-r--r--   0 skrynnik   (503) staff       (20)       25 2024-04-12 16:28:25.000000 pogema-toolbox-0.0.3a2/pogema_toolbox/__init__.py
--rw-r--r--   0 skrynnik   (503) staff       (20)      370 2024-04-03 05:14:34.000000 pogema-toolbox-0.0.3a2/pogema_toolbox/algorithm_config.py
--rw-r--r--   0 skrynnik   (503) staff       (20)     2759 2024-03-22 09:02:48.000000 pogema-toolbox-0.0.3a2/pogema_toolbox/config_variant_generator.py
--rw-r--r--   0 skrynnik   (503) staff       (20)     2301 2024-04-12 16:28:25.000000 pogema-toolbox-0.0.3a2/pogema_toolbox/create_env.py
--rw-r--r--   0 skrynnik   (503) staff       (20)     1358 2024-03-22 09:02:48.000000 pogema-toolbox-0.0.3a2/pogema_toolbox/eval_utils.py
--rw-r--r--   0 skrynnik   (503) staff       (20)    11780 2024-04-12 16:13:34.000000 pogema-toolbox-0.0.3a2/pogema_toolbox/evaluator.py
--rw-r--r--   0 skrynnik   (503) staff       (20)      133 2024-04-03 14:41:24.000000 pogema-toolbox-0.0.3a2/pogema_toolbox/fix_num_threads_issue.py
-drwxr-xr-x   0 skrynnik   (503) staff       (20)        0 2024-04-12 16:28:45.685358 pogema-toolbox-0.0.3a2/pogema_toolbox/maps/
--rw-r--r--   0 skrynnik   (503) staff       (20)      870 2024-04-12 09:29:53.000000 pogema-toolbox-0.0.3a2/pogema_toolbox/maps/default-maps.yaml
--rw-r--r--   0 skrynnik   (503) staff       (20)     4362 2024-04-03 20:32:18.000000 pogema-toolbox-0.0.3a2/pogema_toolbox/registry.py
--rw-r--r--   0 skrynnik   (503) staff       (20)      393 2024-03-22 13:32:25.000000 pogema-toolbox-0.0.3a2/pogema_toolbox/results_holder.py
-drwxr-xr-x   0 skrynnik   (503) staff       (20)        0 2024-04-12 16:28:45.694389 pogema-toolbox-0.0.3a2/pogema_toolbox/views/
--rw-r--r--   0 skrynnik   (503) staff       (20)        0 2024-04-03 05:14:34.000000 pogema-toolbox-0.0.3a2/pogema_toolbox/views/__init__.py
--rw-r--r--   0 skrynnik   (503) staff       (20)     3137 2024-04-04 10:45:37.000000 pogema-toolbox-0.0.3a2/pogema_toolbox/views/view_multi_plot.py
--rw-r--r--   0 skrynnik   (503) staff       (20)     3946 2024-04-03 20:32:18.000000 pogema-toolbox-0.0.3a2/pogema_toolbox/views/view_plot.py
--rw-r--r--   0 skrynnik   (503) staff       (20)     3612 2024-04-03 20:32:18.000000 pogema-toolbox-0.0.3a2/pogema_toolbox/views/view_tabular.py
--rw-r--r--   0 skrynnik   (503) staff       (20)     4424 2024-04-03 20:32:18.000000 pogema-toolbox-0.0.3a2/pogema_toolbox/views/view_utils.py
-drwxr-xr-x   0 skrynnik   (503) staff       (20)        0 2024-04-12 16:28:45.696742 pogema-toolbox-0.0.3a2/pogema_toolbox.egg-info/
--rw-r--r--   0 skrynnik   (503) staff       (20)      720 2024-04-12 16:28:45.000000 pogema-toolbox-0.0.3a2/pogema_toolbox.egg-info/PKG-INFO
--rw-r--r--   0 skrynnik   (503) staff       (20)      763 2024-04-12 16:28:45.000000 pogema-toolbox-0.0.3a2/pogema_toolbox.egg-info/SOURCES.txt
--rw-r--r--   0 skrynnik   (503) staff       (20)        1 2024-04-12 16:28:45.000000 pogema-toolbox-0.0.3a2/pogema_toolbox.egg-info/dependency_links.txt
--rw-r--r--   0 skrynnik   (503) staff       (20)      219 2024-04-12 16:28:45.000000 pogema-toolbox-0.0.3a2/pogema_toolbox.egg-info/requires.txt
--rw-r--r--   0 skrynnik   (503) staff       (20)       15 2024-04-12 16:28:45.000000 pogema-toolbox-0.0.3a2/pogema_toolbox.egg-info/top_level.txt
--rw-r--r--   0 skrynnik   (503) staff       (20)       38 2024-04-12 16:28:45.699490 pogema-toolbox-0.0.3a2/setup.cfg
--rw-r--r--   0 skrynnik   (503) staff       (20)     1756 2024-04-12 09:35:22.000000 pogema-toolbox-0.0.3a2/setup.py
+drwxr-xr-x   0 skrynnik   (503) staff       (20)        0 2024-04-18 12:54:41.663657 pogema_toolbox-0.0.3a3/
+-rw-r--r--   0 skrynnik   (503) staff       (20)    11345 2024-04-03 20:32:18.000000 pogema_toolbox-0.0.3a3/LICENSE
+-rw-r--r--   0 skrynnik   (503) staff       (20)      720 2024-04-18 12:54:41.662527 pogema_toolbox-0.0.3a3/PKG-INFO
+-rw-r--r--   0 skrynnik   (503) staff       (20)       16 2024-03-22 09:25:51.000000 pogema_toolbox-0.0.3a3/README.md
+drwxr-xr-x   0 skrynnik   (503) staff       (20)        0 2024-04-18 12:54:41.647186 pogema_toolbox-0.0.3a3/pogema_toolbox/
+-rw-r--r--   0 skrynnik   (503) staff       (20)       25 2024-04-18 12:52:07.000000 pogema_toolbox-0.0.3a3/pogema_toolbox/__init__.py
+-rw-r--r--   0 skrynnik   (503) staff       (20)      370 2024-04-03 05:14:34.000000 pogema_toolbox-0.0.3a3/pogema_toolbox/algorithm_config.py
+-rw-r--r--   0 skrynnik   (503) staff       (20)     2759 2024-03-22 09:02:48.000000 pogema_toolbox-0.0.3a3/pogema_toolbox/config_variant_generator.py
+-rw-r--r--   0 skrynnik   (503) staff       (20)     2247 2024-04-18 12:48:29.000000 pogema_toolbox-0.0.3a3/pogema_toolbox/create_env.py
+-rw-r--r--   0 skrynnik   (503) staff       (20)     1358 2024-03-22 09:02:48.000000 pogema_toolbox-0.0.3a3/pogema_toolbox/eval_utils.py
+-rw-r--r--   0 skrynnik   (503) staff       (20)    11792 2024-04-18 12:52:14.000000 pogema_toolbox-0.0.3a3/pogema_toolbox/evaluator.py
+-rw-r--r--   0 skrynnik   (503) staff       (20)      133 2024-04-03 14:41:24.000000 pogema_toolbox-0.0.3a3/pogema_toolbox/fix_num_threads_issue.py
+drwxr-xr-x   0 skrynnik   (503) staff       (20)        0 2024-04-18 12:54:41.653595 pogema_toolbox-0.0.3a3/pogema_toolbox/maps/
+-rw-r--r--   0 skrynnik   (503) staff       (20)     2501 2024-04-15 14:00:58.000000 pogema_toolbox-0.0.3a3/pogema_toolbox/maps/default-maps.yaml
+-rw-r--r--   0 skrynnik   (503) staff       (20)     4362 2024-04-03 20:32:18.000000 pogema_toolbox-0.0.3a3/pogema_toolbox/registry.py
+-rw-r--r--   0 skrynnik   (503) staff       (20)      393 2024-03-22 13:32:25.000000 pogema_toolbox-0.0.3a3/pogema_toolbox/results_holder.py
+drwxr-xr-x   0 skrynnik   (503) staff       (20)        0 2024-04-18 12:54:41.660562 pogema_toolbox-0.0.3a3/pogema_toolbox/views/
+-rw-r--r--   0 skrynnik   (503) staff       (20)        0 2024-04-03 05:14:34.000000 pogema_toolbox-0.0.3a3/pogema_toolbox/views/__init__.py
+-rw-r--r--   0 skrynnik   (503) staff       (20)     3137 2024-04-04 10:45:37.000000 pogema_toolbox-0.0.3a3/pogema_toolbox/views/view_multi_plot.py
+-rw-r--r--   0 skrynnik   (503) staff       (20)     3946 2024-04-03 20:32:18.000000 pogema_toolbox-0.0.3a3/pogema_toolbox/views/view_plot.py
+-rw-r--r--   0 skrynnik   (503) staff       (20)     3612 2024-04-03 20:32:18.000000 pogema_toolbox-0.0.3a3/pogema_toolbox/views/view_tabular.py
+-rw-r--r--   0 skrynnik   (503) staff       (20)     4424 2024-04-03 20:32:18.000000 pogema_toolbox-0.0.3a3/pogema_toolbox/views/view_utils.py
+drwxr-xr-x   0 skrynnik   (503) staff       (20)        0 2024-04-18 12:54:41.661795 pogema_toolbox-0.0.3a3/pogema_toolbox.egg-info/
+-rw-r--r--   0 skrynnik   (503) staff       (20)      720 2024-04-18 12:54:41.000000 pogema_toolbox-0.0.3a3/pogema_toolbox.egg-info/PKG-INFO
+-rw-r--r--   0 skrynnik   (503) staff       (20)      763 2024-04-18 12:54:41.000000 pogema_toolbox-0.0.3a3/pogema_toolbox.egg-info/SOURCES.txt
+-rw-r--r--   0 skrynnik   (503) staff       (20)        1 2024-04-18 12:54:41.000000 pogema_toolbox-0.0.3a3/pogema_toolbox.egg-info/dependency_links.txt
+-rw-r--r--   0 skrynnik   (503) staff       (20)      219 2024-04-18 12:54:41.000000 pogema_toolbox-0.0.3a3/pogema_toolbox.egg-info/requires.txt
+-rw-r--r--   0 skrynnik   (503) staff       (20)       15 2024-04-18 12:54:41.000000 pogema_toolbox-0.0.3a3/pogema_toolbox.egg-info/top_level.txt
+-rw-r--r--   0 skrynnik   (503) staff       (20)       38 2024-04-18 12:54:41.663765 pogema_toolbox-0.0.3a3/setup.cfg
+-rw-r--r--   0 skrynnik   (503) staff       (20)     1756 2024-04-12 09:35:22.000000 pogema_toolbox-0.0.3a3/setup.py
```

### Comparing `pogema-toolbox-0.0.3a2/LICENSE` & `pogema_toolbox-0.0.3a3/LICENSE`

 * *Files identical despite different names*

### Comparing `pogema-toolbox-0.0.3a2/PKG-INFO` & `pogema_toolbox-0.0.3a3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pogema-toolbox
-Version: 0.0.3a2
+Version: 0.0.3a3
 Summary: Evaluation toolbox for Pogema environment
 Home-page: https://github.com/Tviskaron/pogema-toolbox
 Author: Alexey Skrynnik
 License: Apache License 2.0
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `pogema-toolbox-0.0.3a2/pogema_toolbox/config_variant_generator.py` & `pogema_toolbox-0.0.3a3/pogema_toolbox/config_variant_generator.py`

 * *Files identical despite different names*

### Comparing `pogema-toolbox-0.0.3a2/pogema_toolbox/create_env.py` & `pogema_toolbox-0.0.3a3/pogema_toolbox/create_env.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,16 +7,15 @@
 from pogema.animation import AnimationMonitor, AnimationConfig
 from gymnasium import Wrapper
 from pydantic import BaseModel
 
 from pogema_toolbox.registry import ToolboxRegistry
 
 
-class Environment(BaseModel, ):
-    grid_config: GridConfig = GridConfig()
+class Environment(GridConfig, ):
     with_animation: bool = False
     use_maps: bool = True
 
 
 class ProvideGlobalObstacles(Wrapper):
     def get_global_obstacles(self):
         return self.grid.get_obstacles().astype(int).tolist()
@@ -56,15 +55,15 @@
             cfg = deepcopy(self._configs[map_idx])
             self.env.unwrapped.grid_config = cfg
             self.env.unwrapped.grid_config.seed = seed
         return self.env.reset(seed=seed, **kwargs)
 
 
 def create_env_base(config: Environment):
-    env = pogema_v0(grid_config=config.grid_config)
+    env = pogema_v0(grid_config=config)
     env = ProvideGlobalObstacles(env)
     if config.use_maps:
         env = MultiMapWrapper(env)
     if config.with_animation:
         env = AnimationMonitor(env, AnimationConfig(directory='experiments/renders', save_every_idx_episode=None))
 
     return env
```

### Comparing `pogema-toolbox-0.0.3a2/pogema_toolbox/eval_utils.py` & `pogema_toolbox-0.0.3a3/pogema_toolbox/eval_utils.py`

 * *Files identical despite different names*

### Comparing `pogema-toolbox-0.0.3a2/pogema_toolbox/evaluator.py` & `pogema_toolbox-0.0.3a3/pogema_toolbox/evaluator.py`

 * *Files 0% similar despite different names*

```diff
@@ -97,15 +97,15 @@
     offset = int(1.0 * size / num_chunks + 0.5)
     for i in range(0, num_chunks - 1):
         yield i * offset, i * offset + offset
     yield num_chunks * offset - offset, size
 
 
 def get_env_config_cost(raw_config):
-    gc = Environment(**raw_config).grid_config
+    gc = Environment(**raw_config)
     return gc.num_agents * gc.max_episode_steps
 
 
 def get_balanced_buckets_indexes(env_configs, num_buckets):
     """
     Distributes environment indexes into balanced buckets based on their costs.
 
@@ -160,15 +160,15 @@
 
     num_process = min(initialized_algo_config.num_process, get_num_of_available_cpus())
     cluster = dd.LocalCluster(n_workers=num_process, threads_per_worker=1, nthreads=1, )
     client = dd.Client(cluster, timeout="120s")  # Connect the client to the cluster
 
     futures = []
     for left, right in split_on_chunks(len(env_configs), initialized_algo_config.num_process):
-        future = client.submit(sequential_backend, algo_config, env_configs[left:right], full_algo_name)
+        future = client.submit(sequential_backend, algo_config, env_configs[left:right], full_algo_name, pure=False)
         futures.append(future)
 
     results = client.gather(futures)  # Gather the results from the distributed tasks
     client.close()  # Close the Dask client and cluster
     cluster.close()
     results = np.concatenate(results).tolist()
     return results
@@ -201,15 +201,15 @@
 
     # Getting maps to initialize registry (if not) and  avoid multiple loading
     ToolboxRegistry.get_maps()
     registry_state = ToolboxRegistry.get_state()
 
     for bucket in balanced_buckets:
         bucket_configs = [env_configs[idx] for idx in bucket]
-        future = client.submit(sequential_backend, algo_config, bucket_configs, full_algo_name, registry_state)
+        future = client.submit(sequential_backend, algo_config, bucket_configs, full_algo_name, registry_state, pure=False)
         futures.append(future)
 
     results = client.gather(futures)
     client.close()
     cluster.close()
 
     # Reorder the results according to the original order of env_configs
```

### Comparing `pogema-toolbox-0.0.3a2/pogema_toolbox/registry.py` & `pogema_toolbox-0.0.3a3/pogema_toolbox/registry.py`

 * *Files identical despite different names*

### Comparing `pogema-toolbox-0.0.3a2/pogema_toolbox/views/view_multi_plot.py` & `pogema_toolbox-0.0.3a3/pogema_toolbox/views/view_multi_plot.py`

 * *Files identical despite different names*

### Comparing `pogema-toolbox-0.0.3a2/pogema_toolbox/views/view_plot.py` & `pogema_toolbox-0.0.3a3/pogema_toolbox/views/view_plot.py`

 * *Files identical despite different names*

### Comparing `pogema-toolbox-0.0.3a2/pogema_toolbox/views/view_tabular.py` & `pogema_toolbox-0.0.3a3/pogema_toolbox/views/view_tabular.py`

 * *Files identical despite different names*

### Comparing `pogema-toolbox-0.0.3a2/pogema_toolbox/views/view_utils.py` & `pogema_toolbox-0.0.3a3/pogema_toolbox/views/view_utils.py`

 * *Files identical despite different names*

### Comparing `pogema-toolbox-0.0.3a2/pogema_toolbox.egg-info/PKG-INFO` & `pogema_toolbox-0.0.3a3/pogema_toolbox.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pogema-toolbox
-Version: 0.0.3a2
+Version: 0.0.3a3
 Summary: Evaluation toolbox for Pogema environment
 Home-page: https://github.com/Tviskaron/pogema-toolbox
 Author: Alexey Skrynnik
 License: Apache License 2.0
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `pogema-toolbox-0.0.3a2/pogema_toolbox.egg-info/SOURCES.txt` & `pogema_toolbox-0.0.3a3/pogema_toolbox.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pogema-toolbox-0.0.3a2/setup.py` & `pogema_toolbox-0.0.3a3/setup.py`

 * *Files identical despite different names*

