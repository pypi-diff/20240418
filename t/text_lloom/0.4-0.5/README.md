# Comparing `tmp/text_lloom-0.4.tar.gz` & `tmp/text_lloom-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "text_lloom-0.4.tar", max compression
+gzip compressed data, was "text_lloom-0.5.tar", max compression
```

## Comparing `text_lloom-0.4.tar` & `text_lloom-0.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0       39 2024-02-02 13:27:07.282735 text_lloom-0.4/README.md
--rw-r--r--   0        0        0      552 2024-04-16 09:41:54.316560 text_lloom-0.4/pyproject.toml
--rw-r--r--   0        0        0     2019 2024-04-16 07:43:43.539102 text_lloom-0.4/src/text_lloom/__init__.py
--rw-r--r--   0        0        0      738 2024-02-28 09:09:42.891236 text_lloom-0.4/src/text_lloom/concept.py
--rw-r--r--   0        0        0    57291 2024-04-15 00:44:18.318856 text_lloom-0.4/src/text_lloom/concept_induction.py
--rw-r--r--   0        0        0    12290 2024-03-08 09:30:26.443347 text_lloom-0.4/src/text_lloom/llm.py
--rw-r--r--   0        0        0     8416 2024-04-13 23:28:08.093682 text_lloom-0.4/src/text_lloom/prompts.py
--rw-r--r--   0        0        0     1263 2024-04-15 01:19:42.816858 text_lloom-0.4/src/text_lloom/static/index.css
--rw-r--r--   0        0        0   455935 2024-04-15 01:19:42.816860 text_lloom-0.4/src/text_lloom/static/index.js
--rw-r--r--   0        0        0      707 2024-04-15 01:19:38.799003 text_lloom-0.4/src/text_lloom/static/index_select.css
--rw-r--r--   0        0        0    11241 2024-04-15 01:19:38.799013 text_lloom-0.4/src/text_lloom/static/index_select.js
--rw-r--r--   0        0        0    24594 2024-04-12 08:12:52.865258 text_lloom-0.4/src/text_lloom/workbench.py
--rw-r--r--   0        0        0      984 1970-01-01 00:00:00.000000 text_lloom-0.4/PKG-INFO
+-rw-r--r--   0        0        0       39 2024-02-02 13:27:07.282735 text_lloom-0.5/README.md
+-rw-r--r--   0        0        0      570 2024-04-17 21:07:25.391477 text_lloom-0.5/pyproject.toml
+-rw-r--r--   0        0        0     2019 2024-04-16 10:45:54.173463 text_lloom-0.5/src/text_lloom/__init__.py
+-rw-r--r--   0        0        0      738 2024-02-28 09:09:42.891236 text_lloom-0.5/src/text_lloom/concept.py
+-rw-r--r--   0        0        0    57328 2024-04-17 20:37:28.168461 text_lloom-0.5/src/text_lloom/concept_induction.py
+-rw-r--r--   0        0        0    12290 2024-03-08 09:30:26.443347 text_lloom-0.5/src/text_lloom/llm.py
+-rw-r--r--   0        0        0     8416 2024-04-13 23:28:08.093682 text_lloom-0.5/src/text_lloom/prompts.py
+-rw-r--r--   0        0        0     1263 2024-04-15 01:19:42.816858 text_lloom-0.5/src/text_lloom/static/index.css
+-rw-r--r--   0        0        0   455935 2024-04-15 01:19:42.816860 text_lloom-0.5/src/text_lloom/static/index.js
+-rw-r--r--   0        0        0      707 2024-04-15 01:19:38.799003 text_lloom-0.5/src/text_lloom/static/index_select.css
+-rw-r--r--   0        0        0    11241 2024-04-15 01:19:38.799013 text_lloom-0.5/src/text_lloom/static/index_select.js
+-rw-r--r--   0        0        0    27004 2024-04-17 20:51:33.880540 text_lloom-0.5/src/text_lloom/workbench.py
+-rw-r--r--   0        0        0     1023 1970-01-01 00:00:00.000000 text_lloom-0.5/PKG-INFO
```

### Comparing `text_lloom-0.4/pyproject.toml` & `text_lloom-0.5/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "text_lloom"
-version = "0.4"
+version = "0.5"
 description = "Concept Induction to analyze unstructured text"
 authors = ["Michelle Lam <mlam4@cs.stanford.edu>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 bertopic = "^0.16.0"
@@ -14,11 +14,12 @@
 langchain = "0.0.271"
 anywidget = "^0.9.7"
 pathos = "^0.3.2"
 ipywidgets = "^8.1.2"
 tiktoken = "^0.6.0"
 nltk = "^3.8.1"
 jupyterlab_widgets = "^3.0.10"
+yaspin = "^3.0.2"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `text_lloom-0.4/src/text_lloom/__init__.py` & `text_lloom-0.5/src/text_lloom/__init__.py`

 * *Files identical despite different names*

### Comparing `text_lloom-0.4/src/text_lloom/concept.py` & `text_lloom-0.5/src/text_lloom/concept.py`

 * *Files identical despite different names*

### Comparing `text_lloom-0.4/src/text_lloom/concept_induction.py` & `text_lloom-0.5/src/text_lloom/concept_induction.py`

 * *Files 0% similar despite different names*

```diff
@@ -92,38 +92,38 @@
     clusters, probs = topic_model.fit_transform(text_vals)
     rows = list(zip(id_vals, text_vals, clusters)) # id_col, text_col, cluster_id_col
     cluster_df = pd.DataFrame(rows, columns=[doc_id_col, doc_col, cluster_id_col])
     cluster_df = cluster_df.sort_values(by=[cluster_id_col])
     
     return cluster_df
 
-def save_progress(sess, df, step_name, start, res, model_name, debug=True):
+def save_progress(sess, df, step_name, start, res, model_name, debug=False):
     # Save df to session
     if (sess is not None) and (df is not None):
         k = sess.get_save_key(step_name)
         sess.saved_dfs[k] = df
 
     # Gets timing
     get_timing(start, step_name, sess, debug=debug)
 
     # Gets cost
     calc_cost(res, model_name, step_name, sess, debug=debug)
 
-def get_timing(start, step_name, sess, debug=True):
+def get_timing(start, step_name, sess, debug=False):
     if start is None:
         return
     elapsed = time.time() - start
     if debug:
         print(f"Total time: {elapsed:0.2f} sec")
     if sess is not None:
         # Save to session if provided
         k = sess.get_save_key(step_name)
         sess.time[k] = elapsed
 
-def calc_cost(results, model_name, step_name, sess, debug=True):
+def calc_cost(results, model_name, step_name, sess, debug=False):
     # Calculate cost with API results and model name
     if results is None:
         return
     # Cost estimation
     in_tokens = np.sum([res.llm_output["token_usage"]["prompt_tokens"] for res in results])
     out_tokens = np.sum([res.llm_output["token_usage"]["completion_tokens"] for res in results])
     in_token_cost, out_token_cost = calc_cost_by_tokens(model_name, in_tokens, out_tokens)
@@ -411,14 +411,15 @@
 # - concept_df: DataFrame (columns: doc_id, text, concept_id, concept_name, concept_prompt)
 async def review(concepts, concept_df, concept_col_prefix, model_name, debug=True, sess=None):
     # Model is asked to review the provided set of concepts
     concepts_out, concept_df_out, removed = await review_remove(concepts, concept_df, concept_col_prefix, model_name=model_name, sess=sess)
     concepts_out, concept_df_out, merged = await review_merge(concepts_out, concept_df_out, concept_col_prefix, model_name=model_name, sess=sess)
 
     if debug:
+        print(f"\n\nAuto-review")
         print(f"Removed ({len(removed)}):\n{removed}")
         print(f"Merged ({len(merged)}):")
         pretty_print_merge_results(merged)
 
     # TODO: ask model to filter to the "best" N concepts
     if sess is not None:
         sess.concepts = concepts_out
```

### Comparing `text_lloom-0.4/src/text_lloom/llm.py` & `text_lloom-0.5/src/text_lloom/llm.py`

 * *Files identical despite different names*

### Comparing `text_lloom-0.4/src/text_lloom/prompts.py` & `text_lloom-0.5/src/text_lloom/prompts.py`

 * *Files identical despite different names*

### Comparing `text_lloom-0.4/src/text_lloom/static/index.css` & `text_lloom-0.5/src/text_lloom/static/index.css`

 * *Files identical despite different names*

### Comparing `text_lloom-0.4/src/text_lloom/static/index.js` & `text_lloom-0.5/src/text_lloom/static/index.js`

 * *Files identical despite different names*

### Comparing `text_lloom-0.4/src/text_lloom/static/index_select.css` & `text_lloom-0.5/src/text_lloom/static/index_select.css`

 * *Files identical despite different names*

### Comparing `text_lloom-0.4/src/text_lloom/static/index_select.js` & `text_lloom-0.5/src/text_lloom/static/index_select.js`

 * *Files identical despite different names*

### Comparing `text_lloom-0.4/src/text_lloom/workbench.py` & `text_lloom-0.5/src/text_lloom/workbench.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import time
 import pandas as pd
 import ipywidgets as widgets
 import random
 from nltk.tokenize import sent_tokenize
 import os
 import openai
+from yaspin import yaspin
 
 
 # Local imports
 if __package__ is None or __package__ == '':
     # uses current directory visibility
     from concept_induction import *
     from concept import Concept
@@ -106,14 +107,40 @@
         self.select_widget = select_widget  # Restore widget after saving
 
     def get_save_key(self, step_name):
         t = time.strftime('%Y-%m-%d-%H-%M-%S', time.localtime())
         k = (step_name, t)  # Key of step name and current time
         return k
 
+    # Printed text formatting
+    def bold_txt(self, s):
+        return f"\033[1m{s}\033[0m"
+
+    def highlight_txt(self, s, color="yellow"):
+        if color == "yellow":
+            return f"\x1b[48;5;228m{s}\x1b[m"
+        elif color == "blue":
+            return f"\x1b[48;5;117m{s}\x1b[m"
+
+    def bold_highlight_txt(self, s):
+        return self.bold_txt(self.highlight_txt(s))
+    
+    def spinner_wrapper(self, step_name):
+        format_step_name = f"{self.highlight_txt(step_name, color='blue')}"
+        return yaspin(text=format_step_name, color="yellow")
+
+    def print_timing(self, step_name):
+        # Print elapsed time for the provided step
+        key_matches = [k for k in self.time.keys() if k[0] == step_name]
+        if len(key_matches) == 0:
+            return  # No matches
+        step_key = key_matches[:-1] # Get the last key
+        elapsed = self.time[step_key]
+        print(f"Total time: {elapsed:0.2f} sec")
+
     # Estimate cost of generation for the given params
     def estimate_gen_cost(self, params=None, verbose=False):
         if params is None:
             params = self.auto_suggest_parameters()
             print(f"No parameters provided, so using auto-suggested parameters: {params}")
         # Conservative estimates based on empirical data
         # TODO: change to gather estimates from test cases programmatically
@@ -151,15 +178,15 @@
 
         # Review: pass all names and prompts
         rev_in_tokens = synth_out_tokens * 2  # For both review_remove and review_merge
         rev_out_tokens = rev_in_tokens * 0.5  # Conservatively assume half size
         est_cost["review"] = calc_cost_by_tokens(self.synth_model_name, rev_in_tokens, rev_out_tokens)
         
         total_cost = np.sum([c[0] + c[1] for c in est_cost.values()])
-        print(f"\n\nEstimated cost: {np.round(total_cost, 2)}")
+        print(f"\n\n{self.bold_txt('Estimated cost')}: ${np.round(total_cost, 2)}")
         print("**Please note that this is only an approximate cost estimate**")
 
         if verbose:
             print(f"\nEstimated cost breakdown:")
             for step_name, cost in est_cost.items():
                 total_cost = np.sum(cost)
                 print(f"\t{step_name}: {total_cost:0.4f}")
@@ -183,15 +210,15 @@
         all_doc_tokens = np.sum([get_token_estimate(doc, self.score_model_name) for doc in self.df_to_score[self.doc_col].tolist()])  # Tokens to encode all documents
         score_in_tokens = all_doc_tokens + (n_batches * (score_prompt_tokens + est_concept_tokens))
         score_out_tokens = est_score_json_tokens * n_concepts * len(self.in_df)
         est_cost = calc_cost_by_tokens(self.score_model_name, score_in_tokens, score_out_tokens)
 
         total_cost = np.sum(est_cost)
         print(f"\n\nScoring {n_concepts} concepts for {len(self.in_df)} documents")
-        print(f"Estimated cost: {np.round(total_cost, 2)}")
+        print(f"{self.bold_txt('Estimated cost')}: ${np.round(total_cost, 2)}")
         print("**Please note that this is only an approximate cost estimate**")
 
         if verbose:
             print(f"\nEstimated cost breakdown:")
             for step_name, cost in zip(["Input", "Output"], est_cost):
                 print(f"\t{step_name}: {cost:0.4f}")
 
@@ -222,135 +249,155 @@
             "synth_n_concepts": synth_n_concepts,
         }
         return params
     
     def summary(self, verbose=True):
         # Time
         total_time = np.sum(list(self.time.values()))
-        print(f"Total time: {total_time:0.2f} sec ({(total_time/60):0.2f} min)")
+        print(f"{self.bold_txt('Total time')}: {total_time:0.2f} sec ({(total_time/60):0.2f} min)")
         if verbose:
             for step_name, time in self.time.items():
                 print(f"\t{step_name}: {time:0.2f} sec")
 
         # Cost
         total_cost = np.sum(list(self.cost.values()))
-        print(f"\n\nTotal cost: {total_cost:0.2f}")
+        print(f"\n\n{self.bold_txt('Total cost')}: ${total_cost:0.2f}")
         if verbose:
             for step_name, cost in self.cost.items():
-                print(f"\t{step_name}: {cost:0.3f}")
+                print(f"\t{step_name}: ${cost:0.3f}")
 
         # Tokens
         in_tokens = np.sum(self.tokens["in_tokens"])
         out_tokens = np.sum(self.tokens["out_tokens"])
         total_tokens =  in_tokens + out_tokens
-        print(f"\n\nTokens: total={total_tokens}, in={in_tokens}, out={out_tokens}")
+        print(f"\n\n{self.bold_txt('Tokens')}: total={total_tokens}, in={in_tokens}, out={out_tokens}")
 
     def show_selected(self):
         active_concepts = self.__get_active_concepts()
-        print(f"\n\nActive concepts (n={len(active_concepts)}):")
+        print(f"\n\n{self.bold_txt('Active concepts')} (n={len(active_concepts)}):")
         for c_id, c in active_concepts.items():
-            print(f"- {c.name}: {c.prompt}")
+            print(f"- {self.bold_txt(c.name)}: {c.prompt}")
 
     # HELPER FUNCTIONS ================================
     async def gen(self, seed=None, params=None, n_synth=1, auto_review=True, debug=True):
         if params is None:
             params = self.auto_suggest_parameters(debug=debug)
             if debug:
-                print(f"Auto-suggested parameters: {params}")
+                print(f"{self.bold_txt('Auto-suggested parameters')}: {params}")
         
         # Run cost estimation
         self.estimate_gen_cost(params)
         
         # Confirm to proceed
-        user_input = input("\nProceed with generation? (y/n): ")
+        print(f"\n\n{self.bold_highlight_txt('Action required')}")
+        user_input = input("Proceed with generation? (y/n): ")
         if user_input.lower() != "y":
             print("Cancelled generation")
             return
 
         # Run concept generation
         filter_n_quotes = params["filter_n_quotes"]
         if filter_n_quotes > 1:
-            df_filtered = await distill_filter(
-                text_df=self.in_df, 
+            step_name = "Distill-filter"
+            with self.spinner_wrapper(step_name) as spinner:
+                df_filtered = await distill_filter(
+                    text_df=self.in_df, 
+                    doc_col=self.doc_col,
+                    doc_id_col=self.doc_id_col,
+                    model_name=self.model_name,
+                    n_quotes=params["filter_n_quotes"],
+                    seed=seed,
+                    sess=self,
+                )
+                self.df_to_score = df_filtered  # Change to use filtered df for concept scoring
+                self.df_filtered = df_filtered
+                spinner.ok("✅")
+                if debug:
+                    self.print_timing(step_name)
+                    display(df_filtered)
+        else:
+            # Just use original df to generate bullets
+            self.df_filtered = self.in_df
+        
+        step_name = "Distill-summarize"
+        with self.spinner_wrapper(step_name) as spinner:
+            df_bullets = await distill_summarize(
+                text_df=self.df_filtered, 
                 doc_col=self.doc_col,
                 doc_id_col=self.doc_id_col,
                 model_name=self.model_name,
-                n_quotes=params["filter_n_quotes"],
+                n_bullets=params["summ_n_bullets"],
                 seed=seed,
                 sess=self,
             )
-            self.df_to_score = df_filtered  # Change to use filtered df for concept scoring
-            self.df_filtered = df_filtered
+            self.df_bullets = df_bullets
+            spinner.ok("✅")
             if debug:
-                print("df_filtered")
-                display(df_filtered)
-        else:
-            # Just use original df to generate bullets
-            self.df_filtered = self.in_df
-        
-        df_bullets = await distill_summarize(
-            text_df=self.df_filtered, 
-            doc_col=self.doc_col,
-            doc_id_col=self.doc_id_col,
-            model_name=self.model_name,
-            n_bullets=params["summ_n_bullets"],
-            seed=seed,
-            sess=self,
-        )
-        self.df_bullets = df_bullets
-        if debug:
-            print("df_bullets")
-            display(df_bullets)
+                self.print_timing(step_name)
+                display(df_bullets)
         
         df_cluster_in = df_bullets
         synth_doc_col = self.doc_col
         synth_n_concepts = params["synth_n_concepts"]
         concept_col_prefix = "concept"
         # Perform synthesize step n_synth times
         for i in range(n_synth):
             self.concepts = {}
-            df_cluster = await cluster(
-                text_df=df_cluster_in, 
-                doc_col=synth_doc_col,
-                doc_id_col=self.doc_id_col,
-                embed_model_name=self.embed_model_name,
-                sess=self,
-            )
-            if debug:
-                print("df_cluster")
-                display(df_cluster)
-            
-            df_concepts = await synthesize(
-                cluster_df=df_cluster, 
-                doc_col=synth_doc_col,
-                doc_id_col=self.doc_id_col,
-                model_name=self.synth_model_name,
-                concept_col_prefix=concept_col_prefix,
-                n_concepts=synth_n_concepts,
-                pattern_phrase="unique topic",
-                seed=seed,
-                sess=self,
-            )
 
-            # Review current concepts (remove low-quality, merge similar)
-            if auto_review:
-                _, df_concepts = await review(concepts=self.concepts, concept_df=df_concepts, concept_col_prefix=concept_col_prefix, model_name=self.synth_model_name, sess=self)
-
-            self.concept_history[i] = self.concepts
-            if debug:
-                # Print results
-                print(f"synthesize {i + 1}: (n={len(self.concepts)})")
-                for k, c in self.concepts.items():
-                    print(f'- Concept {k}:\n\t{c.name}\n\t- Prompt: {c.prompt}')
+            step_name = "Cluster"
+            with self.spinner_wrapper(step_name) as spinner:
+                df_cluster = await cluster(
+                    text_df=df_cluster_in, 
+                    doc_col=synth_doc_col,
+                    doc_id_col=self.doc_id_col,
+                    embed_model_name=self.embed_model_name,
+                    sess=self,
+                )
+                spinner.ok("✅")
+                if debug:
+                    self.print_timing(step_name)
+                    display(df_cluster)
+            
+            step_name = "Synthesize"
+            with self.spinner_wrapper(step_name) as spinner:
+                df_concepts = await synthesize(
+                    cluster_df=df_cluster, 
+                    doc_col=synth_doc_col,
+                    doc_id_col=self.doc_id_col,
+                    model_name=self.synth_model_name,
+                    concept_col_prefix=concept_col_prefix,
+                    n_concepts=synth_n_concepts,
+                    pattern_phrase="unique topic",
+                    seed=seed,
+                    sess=self,
+                )
+                spinner.ok("✅")
+                if debug:
+                    self.print_timing(step_name)
+
+                # Review current concepts (remove low-quality, merge similar)
+                if auto_review:
+                    step_name = "Review"
+                    with self.spinner_wrapper(step_name) as spinner:
+                        _, df_concepts = await review(concepts=self.concepts, concept_df=df_concepts, concept_col_prefix=concept_col_prefix, model_name=self.synth_model_name, sess=self)
+                        spinner.ok("✅")
+
+                self.concept_history[i] = self.concepts
+                if debug:
+                    # Print results
+                    print(f"\n\n{self.highlight_txt('Synthesize', color='blue')} {i + 1}: (n={len(self.concepts)} concepts)")
+                    for k, c in self.concepts.items():
+                        print(f'- Concept {k}:\n\t{c.name}\n\t- Prompt: {c.prompt}')
             
             # Update synthesize params for next iteration
             df_concepts["synth_doc_col"] = df_concepts[f"{concept_col_prefix}_name"] + ": " + df_concepts[f"{concept_col_prefix}_prompt"]
             df_cluster_in = df_concepts
             synth_doc_col = "synth_doc_col"
             synth_n_concepts = math.floor(synth_n_concepts * 0.75)
+        print("✅ Done with concept generation!")
 
     def __concepts_to_json(self):
         concept_dict = {c_id: c.to_dict() for c_id, c in self.concepts.items()}
         # Get examples from example IDs
         for c_id, c in concept_dict.items():
             ex_ids = c["example_ids"]
             in_df = self.df_filtered.copy()
@@ -407,15 +454,16 @@
         if ignore_existing:
             concepts = {c_id: c for c_id, c in concepts.items() if c_id not in self.results}
         
         # Run cost estimation
         self.estimate_score_cost(n_concepts=len(concepts), batch_size=batch_size, get_highlights=get_highlights)
 
         # Confirm to proceed
-        user_input = input("\nProceed with scoring? (y/n): ")
+        print(f"\n\n{self.bold_highlight_txt('Action required')}")
+        user_input = input("Proceed with scoring? (y/n): ")
         if user_input.lower() != "y":
             print("Cancelled scoring")
             return
 
         # Run usual scoring; results are stored to self.results within the function
         score_df = await score_concepts(
             text_df=self.df_to_score, 
@@ -425,14 +473,15 @@
             model_name=self.score_model_name,
             batch_size=batch_size,
             get_highlights=get_highlights,
             sess=self,
             threshold=1.0,
         )
 
+        print("✅ Done with concept scoring!")
         return score_df
 
     def __get_concept_from_name(self, name):
         if name == "Outlier":
             return Concept(name="Outlier", prompt=OUTLIER_CRITERIA, example_ids=[], active=True)
         for c_id, c in self.concepts.items():
             if c.name == name:
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `text_lloom-0.4/PKG-INFO` & `text_lloom-0.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: text_lloom
-Version: 0.4
+Version: 0.5
 Summary: Concept Induction to analyze unstructured text
 Author: Michelle Lam
 Author-email: mlam4@cs.stanford.edu
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -17,11 +17,12 @@
 Requires-Dist: ipywidgets (>=8.1.2,<9.0.0)
 Requires-Dist: jupyterlab_widgets (>=3.0.10,<4.0.0)
 Requires-Dist: langchain (==0.0.271)
 Requires-Dist: nltk (>=3.8.1,<4.0.0)
 Requires-Dist: openai (==0.28)
 Requires-Dist: pathos (>=0.3.2,<0.4.0)
 Requires-Dist: tiktoken (>=0.6.0,<0.7.0)
+Requires-Dist: yaspin (>=3.0.2,<4.0.0)
 Description-Content-Type: text/markdown
 
 Directory for the LLooM python package
```

