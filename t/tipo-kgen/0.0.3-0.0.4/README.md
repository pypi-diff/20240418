# Comparing `tmp/tipo-kgen-0.0.3.tar.gz` & `tmp/tipo-kgen-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tipo-kgen-0.0.3.tar", last modified: Wed Apr 17 18:15:22 2024, max compression
+gzip compressed data, was "tipo-kgen-0.0.4.tar", last modified: Thu Apr 18 15:59:00 2024, max compression
```

## Comparing `tipo-kgen-0.0.3.tar` & `tipo-kgen-0.0.4.tar`

### file list

```diff
@@ -1,25 +1,26 @@
-drwxrwxrwx   0        0        0        0 2024-04-17 18:15:22.945565 tipo-kgen-0.0.3/
--rw-rw-rw-   0        0        0      386 2024-04-17 18:15:22.945565 tipo-kgen-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0      144 2024-04-17 17:13:19.000000 tipo-kgen-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2024-04-17 18:15:22.927545 tipo-kgen-0.0.3/kgen/
--rw-rw-rw-   0        0        0        0 2024-04-17 15:02:12.000000 tipo-kgen-0.0.3/kgen/__init__.py
--rw-rw-rw-   0        0        0     4111 2024-04-17 18:14:56.000000 tipo-kgen-0.0.3/kgen/formatter.py
--rw-rw-rw-   0        0        0     4379 2024-04-17 17:13:55.000000 tipo-kgen-0.0.3/kgen/generate.py
--rw-rw-rw-   0        0        0     1153 2024-04-17 17:47:41.000000 tipo-kgen-0.0.3/kgen/logging.py
--rw-rw-rw-   0        0        0      876 2024-04-17 15:02:12.000000 tipo-kgen-0.0.3/kgen/metainfo.py
--rw-rw-rw-   0        0        0     2484 2024-04-17 15:02:12.000000 tipo-kgen-0.0.3/kgen/models.py
-drwxrwxrwx   0        0        0        0 2024-04-17 18:15:22.935050 tipo-kgen-0.0.3/kgen/tag-list/
--rw-rw-rw-   0        0        0        0 2024-04-17 16:47:26.000000 tipo-kgen-0.0.3/kgen/tag-list/__init__.py
--rw-rw-rw-   0        0        0  4459440 2024-04-17 15:02:11.000000 tipo-kgen-0.0.3/kgen/tag-list/artist.txt
--rw-rw-rw-   0        0        0  4079093 2024-04-17 15:02:11.000000 tipo-kgen-0.0.3/kgen/tag-list/characters.txt
--rw-rw-rw-   0        0        0   823337 2024-04-17 15:02:11.000000 tipo-kgen-0.0.3/kgen/tag-list/copyrights.txt
--rw-rw-rw-   0        0        0     8830 2024-04-17 15:02:11.000000 tipo-kgen-0.0.3/kgen/tag-list/meta.txt
--rw-rw-rw-   0        0        0       42 2024-04-17 18:15:22.946564 tipo-kgen-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      603 2024-04-17 18:15:00.000000 tipo-kgen-0.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-17 18:15:22.945565 tipo-kgen-0.0.3/tipo_kgen.egg-info/
--rw-rw-rw-   0        0        0      386 2024-04-17 18:15:22.000000 tipo-kgen-0.0.3/tipo_kgen.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      446 2024-04-17 18:15:22.000000 tipo-kgen-0.0.3/tipo_kgen.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-17 18:15:22.000000 tipo-kgen-0.0.3/tipo_kgen.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-04-17 17:29:04.000000 tipo-kgen-0.0.3/tipo_kgen.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       35 2024-04-17 18:15:22.000000 tipo-kgen-0.0.3/tipo_kgen.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2024-04-17 18:15:22.000000 tipo-kgen-0.0.3/tipo_kgen.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-18 15:59:00.423552 tipo-kgen-0.0.4/
+-rw-rw-rw-   0        0        0    11540 2024-03-23 06:06:25.000000 tipo-kgen-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0      409 2024-04-18 15:59:00.422549 tipo-kgen-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     2352 2024-04-18 03:16:31.000000 tipo-kgen-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2024-04-18 15:59:00.392022 tipo-kgen-0.0.4/kgen/
+-rw-rw-rw-   0        0        0        0 2024-04-17 15:02:12.000000 tipo-kgen-0.0.4/kgen/__init__.py
+-rw-rw-rw-   0        0        0     4111 2024-04-17 18:14:56.000000 tipo-kgen-0.0.4/kgen/formatter.py
+-rw-rw-rw-   0        0        0     4328 2024-04-18 15:58:06.000000 tipo-kgen-0.0.4/kgen/generate.py
+-rw-rw-rw-   0        0        0     1153 2024-04-17 17:47:41.000000 tipo-kgen-0.0.4/kgen/logging.py
+-rw-rw-rw-   0        0        0     1072 2024-04-18 15:58:40.000000 tipo-kgen-0.0.4/kgen/metainfo.py
+-rw-rw-rw-   0        0        0     2484 2024-04-17 15:02:12.000000 tipo-kgen-0.0.4/kgen/models.py
+drwxrwxrwx   0        0        0        0 2024-04-18 15:59:00.404539 tipo-kgen-0.0.4/kgen/tag-list/
+-rw-rw-rw-   0        0        0        0 2024-04-17 16:47:26.000000 tipo-kgen-0.0.4/kgen/tag-list/__init__.py
+-rw-rw-rw-   0        0        0  4459440 2024-04-17 15:02:11.000000 tipo-kgen-0.0.4/kgen/tag-list/artist.txt
+-rw-rw-rw-   0        0        0  4079093 2024-04-17 15:02:11.000000 tipo-kgen-0.0.4/kgen/tag-list/characters.txt
+-rw-rw-rw-   0        0        0   823337 2024-04-17 15:02:11.000000 tipo-kgen-0.0.4/kgen/tag-list/copyrights.txt
+-rw-rw-rw-   0        0        0     8830 2024-04-17 15:02:11.000000 tipo-kgen-0.0.4/kgen/tag-list/meta.txt
+-rw-rw-rw-   0        0        0       42 2024-04-18 15:59:00.423552 tipo-kgen-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      603 2024-04-18 15:58:55.000000 tipo-kgen-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-18 15:59:00.422549 tipo-kgen-0.0.4/tipo_kgen.egg-info/
+-rw-rw-rw-   0        0        0      409 2024-04-18 15:59:00.000000 tipo-kgen-0.0.4/tipo_kgen.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      454 2024-04-18 15:59:00.000000 tipo-kgen-0.0.4/tipo_kgen.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-18 15:59:00.000000 tipo-kgen-0.0.4/tipo_kgen.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-04-17 17:29:04.000000 tipo-kgen-0.0.4/tipo_kgen.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       35 2024-04-18 15:59:00.000000 tipo-kgen-0.0.4/tipo_kgen.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2024-04-18 15:59:00.000000 tipo-kgen-0.0.4/tipo_kgen.egg-info/top_level.txt
```

### Comparing `tipo-kgen-0.0.3/kgen/formatter.py` & `tipo-kgen-0.0.4/kgen/formatter.py`

 * *Files identical despite different names*

### Comparing `tipo-kgen-0.0.3/kgen/generate.py` & `tipo-kgen-0.0.4/kgen/generate.py`

 * *Files 3% similar despite different names*

```diff
@@ -122,34 +122,35 @@
             eos_token_id=getattr(tokenizer, "eos_token_id", None),
             seed=seed + iter_count,
         )
         iter_count += 1
         llm_gen = llm_gen.replace("</s>", "").replace("<s>", "")
         orig_prompt = llm_gen.split("<|input_end|>")[0]
         extra = llm_gen.split("<|input_end|>")[-1].strip().strip(",")
-        extra_tokens = list(
-            [
-                tok.strip()
-                for tok in extra.split(",")
-                if not black_list_match(tok.strip(), black_list)
-            ]
+        extra_tokens = sorted(
+            set(
+                [
+                    tok.strip()
+                    for tok in extra.split(",")
+                    if not black_list_match(tok.strip(), black_list)
+                ]
+            )
         )
         llm_gen = llm_gen.replace(extra, ", ".join(extra_tokens))
 
         yield llm_gen, extra_tokens, iter_count
 
         if set(extra_tokens) == prev_output:
             same_output_count += 1
             retry += 1
         else:
             same_output_count = 0
             prev_output = set(extra_tokens)
 
         if len(prompt_tags) + len(extra_tokens) < len_target:
-            # print(f"retry: {retry}, same_output_count: {same_output_count}, len: {len(extra_tokens)}")
             retry -= 1
             shuffle(extra_tokens)
             llm_gen = f"{orig_prompt}<|input_end|>{', '.join(extra_tokens)}"
             prompt = llm_gen.strip().replace("  <|", " <|")
         else:
             break
     yield llm_gen, extra_tokens, iter_count
```

### Comparing `tipo-kgen-0.0.3/kgen/logging.py` & `tipo-kgen-0.0.4/kgen/logging.py`

 * *Files identical despite different names*

### Comparing `tipo-kgen-0.0.3/kgen/metainfo.py` & `tipo-kgen-0.0.4/kgen/metainfo.py`

 * *Files 20% similar despite different names*

```diff
@@ -35,14 +35,24 @@
     "displeasing",
     "very displeasing",
     "newest",
     "recent",
     "mid",
     "early",
     "old",
+    "score_9",
+    "score_8_up",
+    "score_7_up",
+    "score_6_up",
+    "score_5_up",
+    "score_4_up",
+    "source_anime",
+    "source_cartoon",
+    "source_furry",
+    "source_pony",
 ]
 RATING_TAGS = ["safe", "general", "sfw", "sensitive", "nsfw", "explicit"]
 TARGET = {
     "very_short": 8,
     "short": 16,
     "long": 30,
     "very_long": 45,
```

### Comparing `tipo-kgen-0.0.3/kgen/models.py` & `tipo-kgen-0.0.4/kgen/models.py`

 * *Files identical despite different names*

### Comparing `tipo-kgen-0.0.3/kgen/tag-list/artist.txt` & `tipo-kgen-0.0.4/kgen/tag-list/artist.txt`

 * *Files identical despite different names*

### Comparing `tipo-kgen-0.0.3/kgen/tag-list/characters.txt` & `tipo-kgen-0.0.4/kgen/tag-list/characters.txt`

 * *Files identical despite different names*

### Comparing `tipo-kgen-0.0.3/kgen/tag-list/copyrights.txt` & `tipo-kgen-0.0.4/kgen/tag-list/copyrights.txt`

 * *Files identical despite different names*

### Comparing `tipo-kgen-0.0.3/kgen/tag-list/meta.txt` & `tipo-kgen-0.0.4/kgen/tag-list/meta.txt`

 * *Files identical despite different names*

### Comparing `tipo-kgen-0.0.3/setup.py` & `tipo-kgen-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 
 setup(
     name="tipo-kgen",
     packages=find_packages(),
-    version="0.0.3",
+    version="0.0.4",
     license="Apache 2.0",
     url="https://github.com/KohakuBlueleaf/KGen",
     description=(
         "TIPO: Text to Image genration through "
         "text Presampling with LLMs for Optimal prompting"
     ),
     author="Shih-Ying Yeh(KohakuBlueLeaf)",
```

