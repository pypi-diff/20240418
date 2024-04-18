# Comparing `tmp/text_lloom-0.5.tar.gz` & `tmp/text_lloom-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "text_lloom-0.5.tar", max compression
+gzip compressed data, was "text_lloom-0.6.tar", max compression
```

## Comparing `text_lloom-0.5.tar` & `text_lloom-0.6.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0       39 2024-02-02 13:27:07.282735 text_lloom-0.5/README.md
--rw-r--r--   0        0        0      570 2024-04-17 21:07:25.391477 text_lloom-0.5/pyproject.toml
--rw-r--r--   0        0        0     2019 2024-04-16 10:45:54.173463 text_lloom-0.5/src/text_lloom/__init__.py
--rw-r--r--   0        0        0      738 2024-02-28 09:09:42.891236 text_lloom-0.5/src/text_lloom/concept.py
--rw-r--r--   0        0        0    57328 2024-04-17 20:37:28.168461 text_lloom-0.5/src/text_lloom/concept_induction.py
--rw-r--r--   0        0        0    12290 2024-03-08 09:30:26.443347 text_lloom-0.5/src/text_lloom/llm.py
--rw-r--r--   0        0        0     8416 2024-04-13 23:28:08.093682 text_lloom-0.5/src/text_lloom/prompts.py
--rw-r--r--   0        0        0     1263 2024-04-15 01:19:42.816858 text_lloom-0.5/src/text_lloom/static/index.css
--rw-r--r--   0        0        0   455935 2024-04-15 01:19:42.816860 text_lloom-0.5/src/text_lloom/static/index.js
--rw-r--r--   0        0        0      707 2024-04-15 01:19:38.799003 text_lloom-0.5/src/text_lloom/static/index_select.css
--rw-r--r--   0        0        0    11241 2024-04-15 01:19:38.799013 text_lloom-0.5/src/text_lloom/static/index_select.js
--rw-r--r--   0        0        0    27004 2024-04-17 20:51:33.880540 text_lloom-0.5/src/text_lloom/workbench.py
--rw-r--r--   0        0        0     1023 1970-01-01 00:00:00.000000 text_lloom-0.5/PKG-INFO
+-rw-r--r--   0        0        0       39 2024-02-02 13:27:07.282735 text_lloom-0.6/README.md
+-rw-r--r--   0        0        0      570 2024-04-18 02:02:51.796866 text_lloom-0.6/pyproject.toml
+-rw-r--r--   0        0        0     2019 2024-04-16 10:45:54.173463 text_lloom-0.6/src/text_lloom/__init__.py
+-rw-r--r--   0        0        0      738 2024-02-28 09:09:42.891236 text_lloom-0.6/src/text_lloom/concept.py
+-rw-r--r--   0        0        0    57603 2024-04-18 02:00:30.123241 text_lloom-0.6/src/text_lloom/concept_induction.py
+-rw-r--r--   0        0        0    12290 2024-03-08 09:30:26.443347 text_lloom-0.6/src/text_lloom/llm.py
+-rw-r--r--   0        0        0     8416 2024-04-13 23:28:08.093682 text_lloom-0.6/src/text_lloom/prompts.py
+-rw-r--r--   0        0        0     1263 2024-04-15 01:19:42.816858 text_lloom-0.6/src/text_lloom/static/index.css
+-rw-r--r--   0        0        0   455935 2024-04-15 01:19:42.816860 text_lloom-0.6/src/text_lloom/static/index.js
+-rw-r--r--   0        0        0      707 2024-04-15 01:19:38.799003 text_lloom-0.6/src/text_lloom/static/index_select.css
+-rw-r--r--   0        0        0    11241 2024-04-15 01:19:38.799013 text_lloom-0.6/src/text_lloom/static/index_select.js
+-rw-r--r--   0        0        0    27460 2024-04-18 01:46:01.866537 text_lloom-0.6/src/text_lloom/workbench.py
+-rw-r--r--   0        0        0     1023 1970-01-01 00:00:00.000000 text_lloom-0.6/PKG-INFO
```

### Comparing `text_lloom-0.5/pyproject.toml` & `text_lloom-0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "text_lloom"
-version = "0.5"
+version = "0.6"
 description = "Concept Induction to analyze unstructured text"
 authors = ["Michelle Lam <mlam4@cs.stanford.edu>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 bertopic = "^0.16.0"
```

### Comparing `text_lloom-0.5/src/text_lloom/__init__.py` & `text_lloom-0.6/src/text_lloom/__init__.py`

 * *Files identical despite different names*

### Comparing `text_lloom-0.5/src/text_lloom/concept.py` & `text_lloom-0.6/src/text_lloom/concept.py`

 * *Files identical despite different names*

### Comparing `text_lloom-0.5/src/text_lloom/concept_induction.py` & `text_lloom-0.6/src/text_lloom/concept_induction.py`

 * *Files 1% similar despite different names*

```diff
@@ -286,15 +286,15 @@
     return examples_json
 
 # Input: cluster_df (columns: doc_id, doc, cluster_id)
 # Parameters: n_concepts
 # Output: 
 # - concepts: dict (concept_id -> concept dict)
 # - concept_df: DataFrame (columns: doc_id, doc, concept_id, concept_name, concept_prompt)
-async def synthesize(cluster_df, doc_col, doc_id_col, model_name, cluster_id_col="cluster_id", concept_col_prefix="concept", n_concepts=None, batch_size=None, verbose=True, pattern_phrase="unifying pattern", dedupe=True, seed=None, sess=None):
+async def synthesize(cluster_df, doc_col, doc_id_col, model_name, cluster_id_col="cluster_id", concept_col_prefix="concept", n_concepts=None, batch_size=None, verbose=False, pattern_phrase="unifying pattern", dedupe=True, seed=None, sess=None, return_logs=False):
     # Synthesis operates on "doc" column for each cluster_id
     # Concept object is created for each concept
     start = time.time()
     
     # Filter to non-empty rows
     cluster_df = filter_empty_rows(cluster_df, doc_col)
 
@@ -350,20 +350,18 @@
     # Run prompts
     prompt_template = synthesize_prompt
     res_text, res_full = await multi_query_gpt_wrapper(prompt_template, arg_dicts, model_name)
 
     # Process results
     concepts = {}
     rows = []
+    logs = ""
     for cur_cluster_id, res in zip(cluster_ids, res_text):
         cur_concepts = json_load(res, top_level_key="patterns")
         if cur_concepts is not None:
-            # concepts.extend(cur_concepts)
-            # cur_examples_dict = {ex_to_id[cur_ex]: cur_ex for cur_ex in cur_examples}
-            
             for concept_dict in cur_concepts:
                 ex_ids = concept_dict["example_ids"]
                 ex_ids = set(ex_ids) # remove duplicates
                 concept = Concept(
                     name=concept_dict["name"],
                     prompt=concept_dict["prompt"],
                     example_ids=ex_ids,
@@ -373,60 +371,80 @@
                 
                 for ex_id in ex_ids:
                     # doc_id, text, concept_id, concept_name, concept_prompt
                     cur_key = (ex_id, cur_cluster_id)
                     if cur_key in ex_id_to_ex:
                         row = [ex_id, ex_id_to_ex[cur_key], concept.id, concept.name, concept.prompt]
                         rows.append(row)
+            # Print intermediate results
+            examples = cluster_dfs[cur_cluster_id][doc_col].tolist()
+            concepts_formatted = pretty_print_dict_list(cur_concepts)
+            cur_log = f"\n\nInput examples: {examples}\nOutput concepts: {concepts_formatted}"
+            logs += cur_log
             if verbose:
-                examples = cluster_dfs[cur_cluster_id][doc_col].tolist()
-                concepts_formatted = pretty_print_dict_list(cur_concepts)
-                print(f"\n\nInput examples: {examples}\nOutput concepts: {concepts_formatted}")
+                print(cur_log)
     # doc_id, text, concept_id, concept_name, concept_prompt
     concept_df = pd.DataFrame(rows, columns=[doc_id_col, doc_col, concept_col_prefix, f"{concept_col_prefix}_name", f"{concept_col_prefix}_prompt"])
 
     concept_df[f"{concept_col_prefix}_namePrompt"] = concept_df[f"{concept_col_prefix}_name"] + ": " + concept_df[f"{concept_col_prefix}_prompt"]
     if dedupe:
         concept_df = dedupe_concepts(concept_df, concept_col=f"{concept_col_prefix}_namePrompt")
 
     save_progress(sess, concept_df, step_name="synthesize", start=start, res=res_full, model_name=model_name)
     # Save to session if provided
     if sess is not None:
         for c_id, c in concepts.items():
             sess.concepts[c_id] = c
+    
+    if return_logs:
+        return concept_df, logs
     return concept_df
 
 def dedupe_concepts(df, concept_col):
     # Remove duplicate concept rows
     return df.drop_duplicates(subset=[concept_col])
 
-def pretty_print_merge_results(merged):
+def get_merge_results(merged):
+    out = ""
     for m in merged:
         orig_concepts = m["original_themes"]
-        print(f"[{orig_concepts}] --> {m['merged_theme_name']}: {m['merged_theme_prompt']}")
+        cur_out = f"\t{orig_concepts} --> {m['merged_theme_name']}: {m['merged_theme_prompt']}"
+        out += cur_out + "\n"
+    return out
 
 # Input: concept_df (columns: doc_id, text, concept_id, concept_name, concept_prompt)
 # Parameters: n_concepts
 # Output: 
 # - concepts: dict (concept_id -> Concept)
 # - concept_df: DataFrame (columns: doc_id, text, concept_id, concept_name, concept_prompt)
-async def review(concepts, concept_df, concept_col_prefix, model_name, debug=True, sess=None):
+async def review(concepts, concept_df, concept_col_prefix, model_name, debug=False, sess=None, return_logs=False):
     # Model is asked to review the provided set of concepts
     concepts_out, concept_df_out, removed = await review_remove(concepts, concept_df, concept_col_prefix, model_name=model_name, sess=sess)
     concepts_out, concept_df_out, merged = await review_merge(concepts_out, concept_df_out, concept_col_prefix, model_name=model_name, sess=sess)
 
+    merge_results = get_merge_results(merged)
+    logs = f"""
+    Auto-review:
+    Removed ({len(removed)}):
+        {removed}
+    Merged ({len(merged)}): 
+    {merge_results}
+    """
     if debug:
         print(f"\n\nAuto-review")
-        print(f"Removed ({len(removed)}):\n{removed}")
-        print(f"Merged ({len(merged)}):")
-        pretty_print_merge_results(merged)
+        print(f"")
+        print(f"")
+        
 
     # TODO: ask model to filter to the "best" N concepts
     if sess is not None:
         sess.concepts = concepts_out
+    
+    if return_logs:
+        return concepts_out, concept_df_out, logs
     return concepts_out, concept_df_out
 
 
 # Model removes concepts that are too specific or too general
 # Input: concept_df (columns: doc_id, text, concept_id, concept_name, concept_prompt)
 # Parameters: n_concepts
 # Output:
```

### Comparing `text_lloom-0.5/src/text_lloom/llm.py` & `text_lloom-0.6/src/text_lloom/llm.py`

 * *Files identical despite different names*

### Comparing `text_lloom-0.5/src/text_lloom/prompts.py` & `text_lloom-0.6/src/text_lloom/prompts.py`

 * *Files identical despite different names*

### Comparing `text_lloom-0.5/src/text_lloom/static/index.css` & `text_lloom-0.6/src/text_lloom/static/index.css`

 * *Files identical despite different names*

### Comparing `text_lloom-0.5/src/text_lloom/static/index.js` & `text_lloom-0.6/src/text_lloom/static/index.js`

 * *Files identical despite different names*

### Comparing `text_lloom-0.5/src/text_lloom/static/index_select.css` & `text_lloom-0.6/src/text_lloom/static/index_select.css`

 * *Files identical despite different names*

### Comparing `text_lloom-0.5/src/text_lloom/static/index_select.js` & `text_lloom-0.6/src/text_lloom/static/index_select.js`

 * *Files identical despite different names*

### Comparing `text_lloom-0.5/src/text_lloom/workbench.py` & `text_lloom-0.6/src/text_lloom/workbench.py`

 * *Files 1% similar despite different names*

```diff
@@ -355,35 +355,47 @@
                 spinner.ok("✅")
                 if debug:
                     self.print_timing(step_name)
                     display(df_cluster)
             
             step_name = "Synthesize"
             with self.spinner_wrapper(step_name) as spinner:
-                df_concepts = await synthesize(
+                df_concepts, synth_logs = await synthesize(
                     cluster_df=df_cluster, 
                     doc_col=synth_doc_col,
                     doc_id_col=self.doc_id_col,
                     model_name=self.synth_model_name,
                     concept_col_prefix=concept_col_prefix,
                     n_concepts=synth_n_concepts,
                     pattern_phrase="unique topic",
                     seed=seed,
                     sess=self,
+                    return_logs=True,
                 )
                 spinner.ok("✅")
                 if debug:
+                    print(synth_logs)
                     self.print_timing(step_name)
 
                 # Review current concepts (remove low-quality, merge similar)
                 if auto_review:
                     step_name = "Review"
                     with self.spinner_wrapper(step_name) as spinner:
-                        _, df_concepts = await review(concepts=self.concepts, concept_df=df_concepts, concept_col_prefix=concept_col_prefix, model_name=self.synth_model_name, sess=self)
+                        _, df_concepts, review_logs = await review(
+                            concepts=self.concepts, 
+                            concept_df=df_concepts, 
+                            concept_col_prefix=concept_col_prefix, 
+                            model_name=self.synth_model_name, 
+                            sess=self,
+                            return_logs=True,
+                        )
                         spinner.ok("✅")
+                        if debug:
+                            print(review_logs)
+                            self.print_timing(step_name)
 
                 self.concept_history[i] = self.concepts
                 if debug:
                     # Print results
                     print(f"\n\n{self.highlight_txt('Synthesize', color='blue')} {i + 1}: (n={len(self.concepts)} concepts)")
                     for k, c in self.concepts.items():
                         print(f'- Concept {k}:\n\t{c.name}\n\t- Prompt: {c.prompt}')
```

### Comparing `text_lloom-0.5/PKG-INFO` & `text_lloom-0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: text_lloom
-Version: 0.5
+Version: 0.6
 Summary: Concept Induction to analyze unstructured text
 Author: Michelle Lam
 Author-email: mlam4@cs.stanford.edu
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

