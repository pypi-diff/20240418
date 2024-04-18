# Comparing `tmp/text_lloom-0.6.tar.gz` & `tmp/text_lloom-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "text_lloom-0.6.tar", max compression
+gzip compressed data, was "text_lloom-0.6.1.tar", max compression
```

## Comparing `text_lloom-0.6.tar` & `text_lloom-0.6.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0       39 2024-02-02 13:27:07.282735 text_lloom-0.6/README.md
--rw-r--r--   0        0        0      570 2024-04-18 02:02:51.796866 text_lloom-0.6/pyproject.toml
--rw-r--r--   0        0        0     2019 2024-04-16 10:45:54.173463 text_lloom-0.6/src/text_lloom/__init__.py
--rw-r--r--   0        0        0      738 2024-02-28 09:09:42.891236 text_lloom-0.6/src/text_lloom/concept.py
--rw-r--r--   0        0        0    57603 2024-04-18 02:00:30.123241 text_lloom-0.6/src/text_lloom/concept_induction.py
--rw-r--r--   0        0        0    12290 2024-03-08 09:30:26.443347 text_lloom-0.6/src/text_lloom/llm.py
--rw-r--r--   0        0        0     8416 2024-04-13 23:28:08.093682 text_lloom-0.6/src/text_lloom/prompts.py
--rw-r--r--   0        0        0     1263 2024-04-15 01:19:42.816858 text_lloom-0.6/src/text_lloom/static/index.css
--rw-r--r--   0        0        0   455935 2024-04-15 01:19:42.816860 text_lloom-0.6/src/text_lloom/static/index.js
--rw-r--r--   0        0        0      707 2024-04-15 01:19:38.799003 text_lloom-0.6/src/text_lloom/static/index_select.css
--rw-r--r--   0        0        0    11241 2024-04-15 01:19:38.799013 text_lloom-0.6/src/text_lloom/static/index_select.js
--rw-r--r--   0        0        0    27460 2024-04-18 01:46:01.866537 text_lloom-0.6/src/text_lloom/workbench.py
--rw-r--r--   0        0        0     1023 1970-01-01 00:00:00.000000 text_lloom-0.6/PKG-INFO
+-rw-r--r--   0        0        0       39 2024-02-02 13:27:07.282735 text_lloom-0.6.1/README.md
+-rw-r--r--   0        0        0      572 2024-04-18 02:43:32.859020 text_lloom-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0     2019 2024-04-16 10:45:54.173463 text_lloom-0.6.1/src/text_lloom/__init__.py
+-rw-r--r--   0        0        0      738 2024-02-28 09:09:42.891236 text_lloom-0.6.1/src/text_lloom/concept.py
+-rw-r--r--   0        0        0    57603 2024-04-18 02:00:30.123241 text_lloom-0.6.1/src/text_lloom/concept_induction.py
+-rw-r--r--   0        0        0    12290 2024-03-08 09:30:26.443347 text_lloom-0.6.1/src/text_lloom/llm.py
+-rw-r--r--   0        0        0     8416 2024-04-13 23:28:08.093682 text_lloom-0.6.1/src/text_lloom/prompts.py
+-rw-r--r--   0        0        0     1263 2024-04-15 01:19:42.816858 text_lloom-0.6.1/src/text_lloom/static/index.css
+-rw-r--r--   0        0        0   455935 2024-04-15 01:19:42.816860 text_lloom-0.6.1/src/text_lloom/static/index.js
+-rw-r--r--   0        0        0      707 2024-04-15 01:19:38.799003 text_lloom-0.6.1/src/text_lloom/static/index_select.css
+-rw-r--r--   0        0        0    11241 2024-04-15 01:19:38.799013 text_lloom-0.6.1/src/text_lloom/static/index_select.js
+-rw-r--r--   0        0        0    27400 2024-04-18 02:39:31.834969 text_lloom-0.6.1/src/text_lloom/workbench.py
+-rw-r--r--   0        0        0     1025 1970-01-01 00:00:00.000000 text_lloom-0.6.1/PKG-INFO
```

### Comparing `text_lloom-0.6/pyproject.toml` & `text_lloom-0.6.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "text_lloom"
-version = "0.6"
+version = "0.6.1"
 description = "Concept Induction to analyze unstructured text"
 authors = ["Michelle Lam <mlam4@cs.stanford.edu>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 bertopic = "^0.16.0"
```

### Comparing `text_lloom-0.6/src/text_lloom/__init__.py` & `text_lloom-0.6.1/src/text_lloom/__init__.py`

 * *Files identical despite different names*

### Comparing `text_lloom-0.6/src/text_lloom/concept.py` & `text_lloom-0.6.1/src/text_lloom/concept.py`

 * *Files identical despite different names*

### Comparing `text_lloom-0.6/src/text_lloom/concept_induction.py` & `text_lloom-0.6.1/src/text_lloom/concept_induction.py`

 * *Files identical despite different names*

### Comparing `text_lloom-0.6/src/text_lloom/llm.py` & `text_lloom-0.6.1/src/text_lloom/llm.py`

 * *Files identical despite different names*

### Comparing `text_lloom-0.6/src/text_lloom/prompts.py` & `text_lloom-0.6.1/src/text_lloom/prompts.py`

 * *Files identical despite different names*

### Comparing `text_lloom-0.6/src/text_lloom/static/index.css` & `text_lloom-0.6.1/src/text_lloom/static/index.css`

 * *Files identical despite different names*

### Comparing `text_lloom-0.6/src/text_lloom/static/index.js` & `text_lloom-0.6.1/src/text_lloom/static/index.js`

 * *Files identical despite different names*

### Comparing `text_lloom-0.6/src/text_lloom/static/index_select.css` & `text_lloom-0.6.1/src/text_lloom/static/index_select.css`

 * *Files identical despite different names*

### Comparing `text_lloom-0.6/src/text_lloom/static/index_select.js` & `text_lloom-0.6.1/src/text_lloom/static/index_select.js`

 * *Files identical despite different names*

### Comparing `text_lloom-0.6/src/text_lloom/workbench.py` & `text_lloom-0.6.1/src/text_lloom/workbench.py`

 * *Files 0% similar despite different names*

```diff
@@ -307,17 +307,17 @@
                     n_quotes=params["filter_n_quotes"],
                     seed=seed,
                     sess=self,
                 )
                 self.df_to_score = df_filtered  # Change to use filtered df for concept scoring
                 self.df_filtered = df_filtered
                 spinner.ok("✅")
-                if debug:
-                    self.print_timing(step_name)
-                    display(df_filtered)
+            if debug:
+                self.print_timing(step_name)
+                display(df_filtered)
         else:
             # Just use original df to generate bullets
             self.df_filtered = self.in_df
         
         step_name = "Distill-summarize"
         with self.spinner_wrapper(step_name) as spinner:
             df_bullets = await distill_summarize(
@@ -327,17 +327,17 @@
                 model_name=self.model_name,
                 n_bullets=params["summ_n_bullets"],
                 seed=seed,
                 sess=self,
             )
             self.df_bullets = df_bullets
             spinner.ok("✅")
-            if debug:
-                self.print_timing(step_name)
-                display(df_bullets)
+        if debug:
+            self.print_timing(step_name)
+            display(df_bullets)
         
         df_cluster_in = df_bullets
         synth_doc_col = self.doc_col
         synth_n_concepts = params["synth_n_concepts"]
         concept_col_prefix = "concept"
         # Perform synthesize step n_synth times
         for i in range(n_synth):
@@ -349,17 +349,17 @@
                     text_df=df_cluster_in, 
                     doc_col=synth_doc_col,
                     doc_id_col=self.doc_id_col,
                     embed_model_name=self.embed_model_name,
                     sess=self,
                 )
                 spinner.ok("✅")
-                if debug:
-                    self.print_timing(step_name)
-                    display(df_cluster)
+            if debug:
+                self.print_timing(step_name)
+                display(df_cluster)
             
             step_name = "Synthesize"
             with self.spinner_wrapper(step_name) as spinner:
                 df_concepts, synth_logs = await synthesize(
                     cluster_df=df_cluster, 
                     doc_col=synth_doc_col,
                     doc_id_col=self.doc_id_col,
@@ -368,34 +368,34 @@
                     n_concepts=synth_n_concepts,
                     pattern_phrase="unique topic",
                     seed=seed,
                     sess=self,
                     return_logs=True,
                 )
                 spinner.ok("✅")
-                if debug:
-                    print(synth_logs)
-                    self.print_timing(step_name)
+            if debug:
+                print(synth_logs)
+                self.print_timing(step_name)
 
                 # Review current concepts (remove low-quality, merge similar)
                 if auto_review:
                     step_name = "Review"
                     with self.spinner_wrapper(step_name) as spinner:
                         _, df_concepts, review_logs = await review(
                             concepts=self.concepts, 
                             concept_df=df_concepts, 
                             concept_col_prefix=concept_col_prefix, 
                             model_name=self.synth_model_name, 
                             sess=self,
                             return_logs=True,
                         )
                         spinner.ok("✅")
-                        if debug:
-                            print(review_logs)
-                            self.print_timing(step_name)
+                    if debug:
+                        print(review_logs)
+                        self.print_timing(step_name)
 
                 self.concept_history[i] = self.concepts
                 if debug:
                     # Print results
                     print(f"\n\n{self.highlight_txt('Synthesize', color='blue')} {i + 1}: (n={len(self.concepts)} concepts)")
                     for k, c in self.concepts.items():
                         print(f'- Concept {k}:\n\t{c.name}\n\t- Prompt: {c.prompt}')
```

### Comparing `text_lloom-0.6/PKG-INFO` & `text_lloom-0.6.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: text_lloom
-Version: 0.6
+Version: 0.6.1
 Summary: Concept Induction to analyze unstructured text
 Author: Michelle Lam
 Author-email: mlam4@cs.stanford.edu
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

