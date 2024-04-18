# Comparing `tmp/sqlgym-0.1.0-py3-none-any.whl.zip` & `tmp/sqlgym-0.1.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 5137 bytes, number of entries: 9
--rw-r--r--  2.0 unx      194 b- defN 24-Apr-07 12:34 sqlgym/__init__.py
--rw-r--r--  2.0 unx     1898 b- defN 24-Apr-07 12:34 sqlgym/sqlgym.py
--rw-r--r--  2.0 unx       41 b- defN 24-Apr-07 12:34 sqlgym/datasets/__init__.py
--rw-r--r--  2.0 unx     5467 b- defN 24-Apr-07 12:34 sqlgym/datasets/bird.py
--rw-r--r--  2.0 unx     1067 b- defN 24-Apr-07 12:34 sqlgym/datasets/utils.py
--rw-r--r--  2.0 unx     1379 b- defN 24-Apr-07 12:34 sqlgym-0.1.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-07 12:34 sqlgym-0.1.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        7 b- defN 24-Apr-07 12:34 sqlgym-0.1.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      683 b- defN 24-Apr-07 12:34 sqlgym-0.1.0.dist-info/RECORD
-9 files, 10828 bytes uncompressed, 3967 bytes compressed:  63.4%
+Zip file size: 5753 bytes, number of entries: 9
+-rw-r--r--  2.0 unx      194 b- defN 24-Apr-18 12:08 sqlgym/__init__.py
+-rw-r--r--  2.0 unx     2176 b- defN 24-Apr-18 12:08 sqlgym/sqlgym.py
+-rw-r--r--  2.0 unx       41 b- defN 24-Apr-18 12:08 sqlgym/datasets/__init__.py
+-rw-r--r--  2.0 unx     5525 b- defN 24-Apr-18 12:08 sqlgym/datasets/bird.py
+-rw-r--r--  2.0 unx     1032 b- defN 24-Apr-18 12:08 sqlgym/datasets/utils.py
+-rw-r--r--  2.0 unx     2996 b- defN 24-Apr-18 12:08 sqlgym-0.1.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-18 12:08 sqlgym-0.1.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx        7 b- defN 24-Apr-18 12:08 sqlgym-0.1.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      683 b- defN 24-Apr-18 12:08 sqlgym-0.1.1.dist-info/RECORD
+9 files, 12746 bytes uncompressed, 4583 bytes compressed:  64.0%
```

## zipnote {}

```diff
@@ -9,20 +9,20 @@
 
 Filename: sqlgym/datasets/bird.py
 Comment: 
 
 Filename: sqlgym/datasets/utils.py
 Comment: 
 
-Filename: sqlgym-0.1.0.dist-info/METADATA
+Filename: sqlgym-0.1.1.dist-info/METADATA
 Comment: 
 
-Filename: sqlgym-0.1.0.dist-info/WHEEL
+Filename: sqlgym-0.1.1.dist-info/WHEEL
 Comment: 
 
-Filename: sqlgym-0.1.0.dist-info/top_level.txt
+Filename: sqlgym-0.1.1.dist-info/top_level.txt
 Comment: 
 
-Filename: sqlgym-0.1.0.dist-info/RECORD
+Filename: sqlgym-0.1.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## sqlgym/__init__.py

```diff
@@ -1,12 +1,12 @@
 from gymnasium.envs.registration import register
 
 from .sqlgym import SqlGymEnv
 
-__version__ = "0.1.0"
+__version__ = "0.1.1"
 
 
 register(
     id="SQLGymEnv-v0",
     entry_point=SqlGymEnv,
     max_episode_steps=300,
 )
```

## sqlgym/sqlgym.py

```diff
@@ -15,22 +15,26 @@
         self,
         idx,
         seed=None,
         options=None,
     ) -> str:
         super().reset(seed=seed, options=options)
         self.idx = idx
-        self.conn = sqlite3.connect(self.dataset[idx].path)
+        path = self.dataset[idx].path
+        self.conn = sqlite3.connect(path, uri=path.startswith("file:"))
         return self.dataset[idx].query
 
     def _get_ground_truth(self) -> str:
         cursor = self.conn.cursor()
-        cursor.execute(self.dataset[self.idx].gt)
-        gt = cursor.fetchall()
-        return gt
+        try:
+            cursor.execute(self.dataset[self.idx].gt)
+            gt = cursor.fetchall()
+            return gt
+        except Exception as e:
+            return str(e)
 
     def _get_reward(self, execution_result: list | Exception) -> float:
         if isinstance(execution_result, Exception):
             return 0.0
         gt = self._get_ground_truth()
         if set(execution_result) == set(gt):
             return 1.0
@@ -48,17 +52,19 @@
 
     def step(self, action: str) -> tuple:
         """
         Action is a string of a SQL query.
         """
         execution_result = self._exec_sql(action)
         reward = self._get_reward(execution_result)
+        if isinstance(execution_result, Exception):
+            execution_result = str(execution_result)
         if self.dataset.sql_gym_env_mode == SqlGymEnvModeEnum.SINGLE:
             terminated = True
-            info = {}
+            info = {"ground_truth": self.dataset[self.idx].gt}
         else:
             raise NotImplementedError
         return execution_result, reward, terminated, info, terminated
 
     def render(self) -> None:
         """make gymnasium.Env happy."""
         return super().render()
```

## sqlgym/datasets/bird.py

```diff
@@ -105,20 +105,22 @@
             db_foreign_keys=self.tables[self._data[idx]["db_id"]]["foreign_keys"],
         )
 
         return f"{database_desciption}\n\n{self._data[idx]['question']}"
 
     def __getitem__(self, idx: int) -> DbDatasetItem:
         return DbDatasetItem(
-            path=self.bird_path.joinpath(
+            path="file:"
+            + self.bird_path.joinpath(
                 self.mode,
                 f"{self.mode}_databases",
                 self._data[idx]["db_id"],
                 f'{self._data[idx]["db_id"]}.sqlite',
-            ),
+            ).as_posix()
+            + "?mode=ro",
             gt=self._data[idx]["SQL"],
             query=self._format_instruction(idx),
             info={
                 "evidence": self._data[idx]["evidence"],
                 "difficulty": (
                     self._data[idx]["difficulty"]
                     if "difficulty" in self._data[idx]
```

## sqlgym/datasets/utils.py

```diff
@@ -27,24 +27,21 @@
     def __getitem__(self, idx: int) -> DbDatasetItem:
         raise NotImplementedError
 
     @abstractmethod
     def __len__(self) -> int:
         raise NotImplementedError
 
-    @abstractmethod
-    def format_instruction(self, idx: int) -> str:
-        raise NotImplementedError
-
 
 def make_sft_dataset(dataset: DbDataset, save_path: Path):
     with open(save_path, "w", encoding="utf8") as f:
-        for data in tqdm(dataset):
+        for idx, data in tqdm(enumerate(dataset), total=len(dataset)):
             f.write(
                 json.dumps(
                     {
+                        "id": idx,
                         "input": data.query,
                         "output": data.gt,
                     }
                 )
                 + "\n"
             )
```

