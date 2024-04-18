# Comparing `tmp/padawan-0.8.1.tar.gz` & `tmp/padawan-0.9.tar.gz`

## Comparing `padawan-0.8.1.tar` & `padawan-0.9.tar`

### file list

```diff
@@ -1,52 +1,52 @@
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 padawan-0.8.1/.readthedocs.yml
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 padawan-0.8.1/docs/Makefile
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 padawan-0.8.1/docs/api.rst
--rw-r--r--   0        0        0     1041 2020-02-02 00:00:00.000000 padawan-0.8.1/docs/conf.py
--rw-r--r--   0        0        0     3428 2020-02-02 00:00:00.000000 padawan-0.8.1/docs/index.rst
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 padawan-0.8.1/docs/make.bat
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 padawan-0.8.1/docs/requirements.txt
--rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 padawan-0.8.1/src/padawan/__init__.py
--rw-r--r--   0        0        0     3000 2020-02-02 00:00:00.000000 padawan-0.8.1/src/padawan/collated_dataset.py
--rw-r--r--   0        0        0     3197 2020-02-02 00:00:00.000000 padawan-0.8.1/src/padawan/concatenated_dataset.py
--rw-r--r--   0        0        0    16594 2020-02-02 00:00:00.000000 padawan-0.8.1/src/padawan/dataset.py
--rw-r--r--   0        0        0     1518 2020-02-02 00:00:00.000000 padawan-0.8.1/src/padawan/in_memory_dataset.py
--rw-r--r--   0        0        0     3053 2020-02-02 00:00:00.000000 padawan-0.8.1/src/padawan/joined_dataset.py
--rw-r--r--   0        0        0     1459 2020-02-02 00:00:00.000000 padawan-0.8.1/src/padawan/json_io.py
--rw-r--r--   0        0        0     5256 2020-02-02 00:00:00.000000 padawan-0.8.1/src/padawan/mapped_dataset.py
--rw-r--r--   0        0        0      886 2020-02-02 00:00:00.000000 padawan-0.8.1/src/padawan/metadata.py
--rw-r--r--   0        0        0     2239 2020-02-02 00:00:00.000000 padawan-0.8.1/src/padawan/ordering.py
--rw-r--r--   0        0        0     3250 2020-02-02 00:00:00.000000 padawan-0.8.1/src/padawan/parallelize.py
--rw-r--r--   0        0        0     2417 2020-02-02 00:00:00.000000 padawan-0.8.1/src/padawan/persisted_dataset.py
--rw-r--r--   0        0        0     5163 2020-02-02 00:00:00.000000 padawan-0.8.1/src/padawan/reindexed_dataset.py
--rw-r--r--   0        0        0     1361 2020-02-02 00:00:00.000000 padawan-0.8.1/src/padawan/renamed_dataset.py
--rw-r--r--   0        0        0     8375 2020-02-02 00:00:00.000000 padawan-0.8.1/src/padawan/repartitioned_dataset.py
--rw-r--r--   0        0        0     5834 2020-02-02 00:00:00.000000 padawan-0.8.1/src/padawan/sliced_dataset.py
--rw-r--r--   0        0        0     3583 2020-02-02 00:00:00.000000 padawan-0.8.1/tests/fixtures.py
--rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 padawan-0.8.1/tests/scratch.py
--rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 padawan-0.8.1/tests/test_collate.py
--rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 padawan-0.8.1/tests/test_concat.py
--rw-r--r--   0        0        0     1189 2020-02-02 00:00:00.000000 padawan-0.8.1/tests/test_from_polars.py
--rw-r--r--   0        0        0     7636 2020-02-02 00:00:00.000000 padawan-0.8.1/tests/test_io.py
--rw-r--r--   0        0        0     1490 2020-02-02 00:00:00.000000 padawan-0.8.1/tests/test_join.py
--rw-r--r--   0        0        0     3956 2020-02-02 00:00:00.000000 padawan-0.8.1/tests/test_map.py
--rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 padawan-0.8.1/tests/test_rename.py
--rw-r--r--   0        0        0     4184 2020-02-02 00:00:00.000000 padawan-0.8.1/tests/test_repartition.py
--rw-r--r--   0        0        0     5711 2020-02-02 00:00:00.000000 padawan-0.8.1/tests/test_slice.py
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 padawan-0.8.1/tests/utils.py
--rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 padawan-0.8.1/tests/tests/data/date_sample.parquet/part0.parquet
--rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 padawan-0.8.1/tests/tests/data/date_sample.parquet/part1.parquet
--rw-r--r--   0        0        0     1447 2020-02-02 00:00:00.000000 padawan-0.8.1/tests/tests/data/datetime_sample.parquet/part0.parquet
--rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 padawan-0.8.1/tests/tests/data/datetime_sample.parquet/part1.parquet
--rw-r--r--   0        0        0     1400 2020-02-02 00:00:00.000000 padawan-0.8.1/tests/tests/data/datetime_sample.parquet/part2.parquet
--rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 padawan-0.8.1/tests/tests/data/datetime_sample.parquet/part3.parquet
--rw-r--r--   0        0        0     1402 2020-02-02 00:00:00.000000 padawan-0.8.1/tests/tests/data/datetime_sample.parquet/part4.parquet
--rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 padawan-0.8.1/tests/tests/data/datetime_sample.parquet/part5.parquet
--rw-r--r--   0        0        0     1402 2020-02-02 00:00:00.000000 padawan-0.8.1/tests/tests/data/datetime_sample.parquet/part6.parquet
--rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 padawan-0.8.1/tests/tests/data/datetime_sample.parquet/part7.parquet
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 padawan-0.8.1/tests/tests/data/result.parquet/_padawan_metadata.json
--rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 padawan-0.8.1/tests/tests/data/result.parquet/_padawan_schema
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 padawan-0.8.1/.gitignore
--rwxr-xr-x   0        0        0     1074 2020-02-02 00:00:00.000000 padawan-0.8.1/LICENSE
--rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 padawan-0.8.1/README.md
--rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 padawan-0.8.1/pyproject.toml
--rw-r--r--   0        0        0     1192 2020-02-02 00:00:00.000000 padawan-0.8.1/PKG-INFO
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 padawan-0.9/.readthedocs.yml
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 padawan-0.9/docs/Makefile
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 padawan-0.9/docs/api.rst
+-rw-r--r--   0        0        0     1041 2020-02-02 00:00:00.000000 padawan-0.9/docs/conf.py
+-rw-r--r--   0        0        0     3428 2020-02-02 00:00:00.000000 padawan-0.9/docs/index.rst
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 padawan-0.9/docs/make.bat
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 padawan-0.9/docs/requirements.txt
+-rw-r--r--   0        0        0      602 2020-02-02 00:00:00.000000 padawan-0.9/src/padawan/__init__.py
+-rw-r--r--   0        0        0     3000 2020-02-02 00:00:00.000000 padawan-0.9/src/padawan/collated_dataset.py
+-rw-r--r--   0        0        0     3197 2020-02-02 00:00:00.000000 padawan-0.9/src/padawan/concatenated_dataset.py
+-rw-r--r--   0        0        0    16594 2020-02-02 00:00:00.000000 padawan-0.9/src/padawan/dataset.py
+-rw-r--r--   0        0        0     1518 2020-02-02 00:00:00.000000 padawan-0.9/src/padawan/in_memory_dataset.py
+-rw-r--r--   0        0        0     3053 2020-02-02 00:00:00.000000 padawan-0.9/src/padawan/joined_dataset.py
+-rw-r--r--   0        0        0     1459 2020-02-02 00:00:00.000000 padawan-0.9/src/padawan/json_io.py
+-rw-r--r--   0        0        0     5256 2020-02-02 00:00:00.000000 padawan-0.9/src/padawan/mapped_dataset.py
+-rw-r--r--   0        0        0      886 2020-02-02 00:00:00.000000 padawan-0.9/src/padawan/metadata.py
+-rw-r--r--   0        0        0     2239 2020-02-02 00:00:00.000000 padawan-0.9/src/padawan/ordering.py
+-rw-r--r--   0        0        0     3250 2020-02-02 00:00:00.000000 padawan-0.9/src/padawan/parallelize.py
+-rw-r--r--   0        0        0     2417 2020-02-02 00:00:00.000000 padawan-0.9/src/padawan/persisted_dataset.py
+-rw-r--r--   0        0        0     5163 2020-02-02 00:00:00.000000 padawan-0.9/src/padawan/reindexed_dataset.py
+-rw-r--r--   0        0        0     1361 2020-02-02 00:00:00.000000 padawan-0.9/src/padawan/renamed_dataset.py
+-rw-r--r--   0        0        0     8157 2020-02-02 00:00:00.000000 padawan-0.9/src/padawan/repartitioned_dataset.py
+-rw-r--r--   0        0        0     5834 2020-02-02 00:00:00.000000 padawan-0.9/src/padawan/sliced_dataset.py
+-rw-r--r--   0        0        0     3593 2020-02-02 00:00:00.000000 padawan-0.9/tests/fixtures.py
+-rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 padawan-0.9/tests/scratch.py
+-rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 padawan-0.9/tests/test_collate.py
+-rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 padawan-0.9/tests/test_concat.py
+-rw-r--r--   0        0        0     1189 2020-02-02 00:00:00.000000 padawan-0.9/tests/test_from_polars.py
+-rw-r--r--   0        0        0     7636 2020-02-02 00:00:00.000000 padawan-0.9/tests/test_io.py
+-rw-r--r--   0        0        0     1490 2020-02-02 00:00:00.000000 padawan-0.9/tests/test_join.py
+-rw-r--r--   0        0        0     3956 2020-02-02 00:00:00.000000 padawan-0.9/tests/test_map.py
+-rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 padawan-0.9/tests/test_rename.py
+-rw-r--r--   0        0        0     4184 2020-02-02 00:00:00.000000 padawan-0.9/tests/test_repartition.py
+-rw-r--r--   0        0        0     5711 2020-02-02 00:00:00.000000 padawan-0.9/tests/test_slice.py
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 padawan-0.9/tests/utils.py
+-rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 padawan-0.9/tests/tests/data/date_sample.parquet/part0.parquet
+-rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 padawan-0.9/tests/tests/data/date_sample.parquet/part1.parquet
+-rw-r--r--   0        0        0     1447 2020-02-02 00:00:00.000000 padawan-0.9/tests/tests/data/datetime_sample.parquet/part0.parquet
+-rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 padawan-0.9/tests/tests/data/datetime_sample.parquet/part1.parquet
+-rw-r--r--   0        0        0     1400 2020-02-02 00:00:00.000000 padawan-0.9/tests/tests/data/datetime_sample.parquet/part2.parquet
+-rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 padawan-0.9/tests/tests/data/datetime_sample.parquet/part3.parquet
+-rw-r--r--   0        0        0     1402 2020-02-02 00:00:00.000000 padawan-0.9/tests/tests/data/datetime_sample.parquet/part4.parquet
+-rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 padawan-0.9/tests/tests/data/datetime_sample.parquet/part5.parquet
+-rw-r--r--   0        0        0     1402 2020-02-02 00:00:00.000000 padawan-0.9/tests/tests/data/datetime_sample.parquet/part6.parquet
+-rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 padawan-0.9/tests/tests/data/datetime_sample.parquet/part7.parquet
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 padawan-0.9/tests/tests/data/result.parquet/_padawan_metadata.json
+-rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 padawan-0.9/tests/tests/data/result.parquet/_padawan_schema
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 padawan-0.9/.gitignore
+-rwxr-xr-x   0        0        0     1074 2020-02-02 00:00:00.000000 padawan-0.9/LICENSE
+-rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 padawan-0.9/README.md
+-rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 padawan-0.9/pyproject.toml
+-rw-r--r--   0        0        0     1191 2020-02-02 00:00:00.000000 padawan-0.9/PKG-INFO
```

### Comparing `padawan-0.8.1/docs/Makefile` & `padawan-0.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `padawan-0.8.1/docs/conf.py` & `padawan-0.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `padawan-0.8.1/docs/index.rst` & `padawan-0.9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `padawan-0.8.1/docs/make.bat` & `padawan-0.9/docs/make.bat`

 * *Files identical despite different names*

### Comparing `padawan-0.8.1/src/padawan/__init__.py` & `padawan-0.9/src/padawan/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = '0.8.1'
+__version__ = '0.9'
 
 __all__ = [
     'scan_parquet',
     'from_polars',
     'concat',
 ]
```

### Comparing `padawan-0.8.1/src/padawan/collated_dataset.py` & `padawan-0.9/src/padawan/collated_dataset.py`

 * *Files identical despite different names*

### Comparing `padawan-0.8.1/src/padawan/concatenated_dataset.py` & `padawan-0.9/src/padawan/concatenated_dataset.py`

 * *Files identical despite different names*

### Comparing `padawan-0.8.1/src/padawan/dataset.py` & `padawan-0.9/src/padawan/dataset.py`

 * *Files identical despite different names*

### Comparing `padawan-0.8.1/src/padawan/in_memory_dataset.py` & `padawan-0.9/src/padawan/in_memory_dataset.py`

 * *Files identical despite different names*

### Comparing `padawan-0.8.1/src/padawan/joined_dataset.py` & `padawan-0.9/src/padawan/joined_dataset.py`

 * *Files identical despite different names*

### Comparing `padawan-0.8.1/src/padawan/json_io.py` & `padawan-0.9/src/padawan/json_io.py`

 * *Files identical despite different names*

### Comparing `padawan-0.8.1/src/padawan/mapped_dataset.py` & `padawan-0.9/src/padawan/mapped_dataset.py`

 * *Files identical despite different names*

### Comparing `padawan-0.8.1/src/padawan/metadata.py` & `padawan-0.9/src/padawan/metadata.py`

 * *Files identical despite different names*

### Comparing `padawan-0.8.1/src/padawan/ordering.py` & `padawan-0.9/src/padawan/ordering.py`

 * *Files identical despite different names*

### Comparing `padawan-0.8.1/src/padawan/parallelize.py` & `padawan-0.9/src/padawan/parallelize.py`

 * *Files identical despite different names*

### Comparing `padawan-0.8.1/src/padawan/persisted_dataset.py` & `padawan-0.9/src/padawan/persisted_dataset.py`

 * *Files identical despite different names*

### Comparing `padawan-0.8.1/src/padawan/reindexed_dataset.py` & `padawan-0.9/src/padawan/reindexed_dataset.py`

 * *Files identical despite different names*

### Comparing `padawan-0.8.1/src/padawan/renamed_dataset.py` & `padawan-0.9/src/padawan/renamed_dataset.py`

 * *Files identical despite different names*

### Comparing `padawan-0.8.1/src/padawan/repartitioned_dataset.py` & `padawan-0.9/src/padawan/repartitioned_dataset.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,61 +1,65 @@
 import polars as pl
 
 from .dataset import Dataset
 
 
 def get_row_divisions(partition_sizes, rows_per_partition):
-        partition_indices = []
-        row_indices = []
-        src_partition = 0
-        src_row_index = 0
-        dest_row_index = 0
-        num_src_partitions = len(partition_sizes)
-        while (src_partition, src_row_index) < (num_src_partitions, 0):
-            rem_src_rows = partition_sizes[src_partition] - src_row_index
-            rem_dest_rows = rows_per_partition - dest_row_index
-            if rem_src_rows < rem_dest_rows:
-                # add remainder of source partition
-                dest_row_index += rem_src_rows
-                src_partition += 1
-                src_row_index = 0
-            elif rem_src_rows == rem_dest_rows:
-                # add remainder of source partition and create split
-                dest_row_index += rem_src_rows
-                src_partition += 1
-                src_row_index = 0
-                dest_row_index = 0
-                if src_partition < num_src_partitions:
-                    partition_indices.append(src_partition)
-                    row_indices.append(src_row_index)
-            else:
-                # add part of source partition and create split
-                src_row_index += rem_dest_rows
-                dest_row_index = 0
-                if src_partition < num_src_partitions:
-                    partition_indices.append(src_partition)
-                    row_indices.append(src_row_index)
-
-        divisions = list(zip(partition_indices, row_indices))
-        sizes = [rows_per_partition]*len(divisions) + \
-            [sum(partition_sizes)-rows_per_partition*len(divisions)]
-        lower_bounds = [()]*len(sizes)
-        upper_bounds = [()]*len(sizes)
-        return divisions, sizes, lower_bounds, upper_bounds
+    num_rows = sum(partition_sizes)
+    df_old = (
+        pl.DataFrame(pl.Series('row', [0] + list(partition_sizes)[:-1], pl.UInt32))
+        .with_row_count('part_index')
+        .with_columns(
+            row=pl.col('row').cum_sum(),
+            is_new_div=pl.lit(False, pl.Boolean),
+        )
+        .select(
+            'row',
+            'part_index',
+            pl.col('row').alias('part_base'),
+            'is_new_div',
+        )
+    )
+    df_new = (
+        pl.DataFrame(pl.int_range(0, num_rows, rows_per_partition, dtype=pl.UInt32, eager=True).alias('row'))
+        .with_columns(
+            part_index=pl.lit(None, pl.UInt32),
+            part_base=pl.lit(None, pl.UInt32),
+            is_new_div=pl.lit(True, pl.Boolean),
+        )
+    )
+    divisions = list(
+        pl.concat([df_old, df_new])
+        .sort('row', 'is_new_div')
+        .with_columns(
+            part_index=pl.col('part_index').fill_null(strategy='forward'),
+            part_base=pl.col('part_base').fill_null(strategy='forward'),
+        )
+        .with_columns(offset=pl.col('row') - pl.col('part_base'))
+        .filter(pl.col('is_new_div') & (pl.col('row') > 0))
+        .select('part_index', 'offset')
+        .rows()
+    )
+
+    sizes = [rows_per_partition]*len(divisions) + \
+        [sum(partition_sizes)-rows_per_partition*len(divisions)]
+    lower_bounds = [()]*len(sizes)
+    upper_bounds = [()]*len(sizes)
+    return divisions, sizes, lower_bounds, upper_bounds
 
 
 def _sample_partition(part, seed, index_columns, frac):
     sample = part.select(index_columns)
     if frac < 1.0:
         sample = sample.collect()
         nrows = max(int(frac*len(sample)), 1)
         sample = sample.sample(nrows, seed=seed).lazy()
     sample = (
         sample
-        .groupby(index_columns)
+        .group_by(index_columns)
         .agg(pl.count().alias('__size'))
     )
     return sample
 
 
 def get_index_divisions(
         ds,
@@ -78,42 +82,47 @@
         .map(
             _sample_partition,
             extra_args=extra_args,
             shared_args=shared_args,
         )
         .collect(parallel=parallel, progress=progress)
         .lazy()
-        .groupby(index_columns)
+        .group_by(index_columns)
         .agg(pl.col('__size').sum())
         .sort(index_columns)
-        .with_columns(pl.col('__size').cumsum())
+        .with_columns(__part=pl.col('__size').cum_sum()//rows_per_partition)
         .collect()
     )
-
-    lower_bounds = []
-    upper_bounds = []
-    sizes = []
-    current_size = 0
-    while len(sample) > 0:
-        head = sample.filter(
-            pl.col('__size') <= current_size + samples_per_partition)
-        if len(head) == 0:
-            head = sample[:1, :]
-            sample = sample[1:, :]
-        else:
-            sample = sample.filter(
-                pl.col('__size') > current_size + samples_per_partition)
-        lower_bounds.append(head.row(0)[:-1])
-        upper_bounds.append(head.row(-1)[:-1])
-        sizes.append(head[-1, '__size'] - current_size)
-        current_size = head[-1, '__size']
-
+    lower_bounds = list(
+        sample
+        .group_by('__part')
+        .head(1)
+        .sort('__part')
+        .select(index_columns)
+        .rows()
+    )
     divisions = lower_bounds[1:]
-
-    if samples_per_partition != rows_per_partition:
+    if samples_per_partition == rows_per_partition:
+        upper_bounds = list(
+            sample
+            .group_by('__part')
+            .tail(1)
+            .sort('__part')
+            .select(index_columns)
+            .rows()
+        )
+        sizes = (
+            sample
+            .group_by('__part')
+            .agg(pl.col('__size').sum())
+            .sort('__part')
+            .get_column('__size')
+            .to_list()
+        )
+    else:
         lower_bounds = None
         upper_bounds = None
         sizes = None
 
     return divisions, sizes, lower_bounds, upper_bounds
 
 
@@ -226,14 +235,16 @@
       seed_increment (int, optional): For every subsequent partition the
         random seed in incremented by `seed_increment`. Defaults to 10.
 
     Returns:
       padawan.Dataset: The repartitioned dataset.
 
     """
+    if len(self) == 0:
+        return self
     return RepartitionedDataset(
         self,
         rows_per_partition,
         sample_fraction=sample_fraction,
         parallel=parallel,
         progress=progress,
         base_seed=base_seed,
```

### Comparing `padawan-0.8.1/src/padawan/sliced_dataset.py` & `padawan-0.9/src/padawan/sliced_dataset.py`

 * *Files identical despite different names*

### Comparing `padawan-0.8.1/tests/fixtures.py` & `padawan-0.9/tests/fixtures.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 
 @pytest.fixture
 def datetime_sample():
     t0 = datetime(2022, 1, 1)
     t1 = datetime(2022, 1, 5)
     dt = timedelta(hours=1)
-    t = pl.date_range(t0, t1, dt, name='t', closed='left', eager=True)
+    t = pl.datetime_range(t0, t1, dt, closed='left', eager=True).alias('t')
     day = t.dt.truncate('1d').cast(pl.Date).alias('date')
     hour = (t - day).alias('hour')
     a = pl.Series('a', np.arange(len(t)))
     df = pl.DataFrame([t, day, hour, a])
 
     null_df = pl.DataFrame([
         pl.Series('t', [None, None], pl.Datetime),
@@ -77,15 +77,15 @@
 
 
 @pytest.fixture
 def date_sample():
     t0 = datetime(2022, 1, 2)
     t1 = datetime(2022, 1, 6)
     dt = timedelta(days=1)
-    t = pl.date_range(t0, t1, dt, name='t', closed='left', eager=True)
+    t = pl.datetime_range(t0, t1, dt, closed='left', eager=True).alias('t')
     day = t.dt.truncate('1d').cast(pl.Date).alias('date')
     x = pl.Series('x', np.arange(len(day)))
     df = pl.DataFrame([day, x])
 
 
     divisions = [0, 2, 4]
```

### Comparing `padawan-0.8.1/tests/test_collate.py` & `padawan-0.9/tests/test_collate.py`

 * *Files identical despite different names*

### Comparing `padawan-0.8.1/tests/test_concat.py` & `padawan-0.9/tests/test_concat.py`

 * *Files identical despite different names*

### Comparing `padawan-0.8.1/tests/test_from_polars.py` & `padawan-0.9/tests/test_from_polars.py`

 * *Files identical despite different names*

### Comparing `padawan-0.8.1/tests/test_io.py` & `padawan-0.9/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `padawan-0.8.1/tests/test_join.py` & `padawan-0.9/tests/test_join.py`

 * *Files identical despite different names*

### Comparing `padawan-0.8.1/tests/test_map.py` & `padawan-0.9/tests/test_map.py`

 * *Files identical despite different names*

### Comparing `padawan-0.8.1/tests/test_rename.py` & `padawan-0.9/tests/test_rename.py`

 * *Files identical despite different names*

### Comparing `padawan-0.8.1/tests/test_repartition.py` & `padawan-0.9/tests/test_repartition.py`

 * *Files identical despite different names*

### Comparing `padawan-0.8.1/tests/test_slice.py` & `padawan-0.9/tests/test_slice.py`

 * *Files identical despite different names*

### Comparing `padawan-0.8.1/tests/tests/data/date_sample.parquet/part0.parquet` & `padawan-0.9/tests/tests/data/date_sample.parquet/part0.parquet`

 * *Files identical despite different names*

### Comparing `padawan-0.8.1/tests/tests/data/date_sample.parquet/part1.parquet` & `padawan-0.9/tests/tests/data/date_sample.parquet/part1.parquet`

 * *Files identical despite different names*

### Comparing `padawan-0.8.1/tests/tests/data/datetime_sample.parquet/part0.parquet` & `padawan-0.9/tests/tests/data/datetime_sample.parquet/part0.parquet`

 * *Files identical despite different names*

### Comparing `padawan-0.8.1/tests/tests/data/datetime_sample.parquet/part1.parquet` & `padawan-0.9/tests/tests/data/datetime_sample.parquet/part1.parquet`

 * *Files identical despite different names*

### Comparing `padawan-0.8.1/tests/tests/data/datetime_sample.parquet/part2.parquet` & `padawan-0.9/tests/tests/data/datetime_sample.parquet/part2.parquet`

 * *Files identical despite different names*

### Comparing `padawan-0.8.1/tests/tests/data/datetime_sample.parquet/part3.parquet` & `padawan-0.9/tests/tests/data/datetime_sample.parquet/part3.parquet`

 * *Files identical despite different names*

### Comparing `padawan-0.8.1/tests/tests/data/datetime_sample.parquet/part4.parquet` & `padawan-0.9/tests/tests/data/datetime_sample.parquet/part4.parquet`

 * *Files identical despite different names*

### Comparing `padawan-0.8.1/tests/tests/data/datetime_sample.parquet/part5.parquet` & `padawan-0.9/tests/tests/data/datetime_sample.parquet/part5.parquet`

 * *Files identical despite different names*

### Comparing `padawan-0.8.1/tests/tests/data/datetime_sample.parquet/part6.parquet` & `padawan-0.9/tests/tests/data/datetime_sample.parquet/part6.parquet`

 * *Files identical despite different names*

### Comparing `padawan-0.8.1/tests/tests/data/datetime_sample.parquet/part7.parquet` & `padawan-0.9/tests/tests/data/datetime_sample.parquet/part7.parquet`

 * *Files identical despite different names*

### Comparing `padawan-0.8.1/LICENSE` & `padawan-0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `padawan-0.8.1/README.md` & `padawan-0.9/README.md`

 * *Files identical despite different names*

### Comparing `padawan-0.8.1/PKG-INFO` & `padawan-0.9/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: padawan
-Version: 0.8.1
+Version: 0.9
 Summary: Wrangle partitioned data with polars.
 Project-URL: Homepage, https://github.com/mwiebusch78/padawan
 Project-URL: Bug Tracker, https://github.com/mwiebusch78/padawan/issues
 Project-URL: Documentation, https://padawan.readthedocs.io/en/latest/
 Author: Martin Wiebusch
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Requires-Dist: cloudpickle
-Requires-Dist: polars>=0.15.9
+Requires-Dist: polars>=0.19.19
 Description-Content-Type: text/markdown
 
 # padawan
 
 Wrangle partitioned data with polars.
 
 ## Installation
```

