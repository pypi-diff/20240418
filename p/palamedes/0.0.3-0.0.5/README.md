# Comparing `tmp/palamedes-0.0.3.tar.gz` & `tmp/palamedes-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "palamedes-0.0.3.tar", last modified: Wed Mar 27 19:22:34 2024, max compression
+gzip compressed data, was "palamedes-0.0.5.tar", last modified: Thu Apr 18 18:25:47 2024, max compression
```

## Comparing `palamedes-0.0.3.tar` & `palamedes-0.0.5.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 19:22:34.120012 palamedes-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-03-27 19:22:29.000000 palamedes-0.0.3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4943 2024-03-27 19:22:34.120012 palamedes-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4378 2024-03-27 19:22:29.000000 palamedes-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 19:22:34.116012 palamedes-0.0.3/palamedes/
--rw-r--r--   0 runner    (1001) docker     (127)     3816 2024-03-27 19:22:29.000000 palamedes-0.0.3/palamedes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2621 2024-03-27 19:22:29.000000 palamedes-0.0.3/palamedes/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10300 2024-03-27 19:22:29.000000 palamedes-0.0.3/palamedes/align.py
--rw-r--r--   0 runner    (1001) docker     (127)      940 2024-03-27 19:22:29.000000 palamedes-0.0.3/palamedes/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 19:22:34.120012 palamedes-0.0.3/palamedes/hgvs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 19:22:29.000000 palamedes-0.0.3/palamedes/hgvs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11965 2024-03-27 19:22:29.000000 palamedes-0.0.3/palamedes/hgvs/builders.py
--rw-r--r--   0 runner    (1001) docker     (127)     2973 2024-03-27 19:22:29.000000 palamedes-0.0.3/palamedes/hgvs/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2047 2024-03-27 19:22:29.000000 palamedes-0.0.3/palamedes/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     3416 2024-03-27 19:22:29.000000 palamedes-0.0.3/palamedes/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 19:22:34.120012 palamedes-0.0.3/palamedes.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4943 2024-03-27 19:22:34.000000 palamedes-0.0.3/palamedes.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      599 2024-03-27 19:22:34.000000 palamedes-0.0.3/palamedes.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-27 19:22:34.000000 palamedes-0.0.3/palamedes.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-03-27 19:22:34.000000 palamedes-0.0.3/palamedes.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-03-27 19:22:34.000000 palamedes-0.0.3/palamedes.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-03-27 19:22:34.000000 palamedes-0.0.3/palamedes.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-27 19:22:34.120012 palamedes-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      889 2024-03-27 19:22:29.000000 palamedes-0.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 19:22:34.120012 palamedes-0.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 19:22:29.000000 palamedes-0.0.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-03-27 19:22:29.000000 palamedes-0.0.3/tests/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 19:22:34.120012 palamedes-0.0.3/tests/hgvs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 19:22:29.000000 palamedes-0.0.3/tests/hgvs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10431 2024-03-27 19:22:29.000000 palamedes-0.0.3/tests/hgvs/test_builders.py
--rw-r--r--   0 runner    (1001) docker     (127)     9293 2024-03-27 19:22:29.000000 palamedes-0.0.3/tests/hgvs/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    11257 2024-03-27 19:22:29.000000 palamedes-0.0.3/tests/test_align.py
--rw-r--r--   0 runner    (1001) docker     (127)     1915 2024-03-27 19:22:29.000000 palamedes-0.0.3/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     3650 2024-03-27 19:22:29.000000 palamedes-0.0.3/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:25:47.610363 palamedes-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-18 18:25:35.000000 palamedes-0.0.5/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5269 2024-04-18 18:25:47.610363 palamedes-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4704 2024-04-18 18:25:35.000000 palamedes-0.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:25:47.606363 palamedes-0.0.5/palamedes/
+-rw-r--r--   0 runner    (1001) docker     (127)     3816 2024-04-18 18:25:35.000000 palamedes-0.0.5/palamedes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2621 2024-04-18 18:25:35.000000 palamedes-0.0.5/palamedes/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11495 2024-04-18 18:25:35.000000 palamedes-0.0.5/palamedes/align.py
+-rw-r--r--   0 runner    (1001) docker     (127)      940 2024-04-18 18:25:35.000000 palamedes-0.0.5/palamedes/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:25:47.606363 palamedes-0.0.5/palamedes/hgvs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 18:25:35.000000 palamedes-0.0.5/palamedes/hgvs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11965 2024-04-18 18:25:35.000000 palamedes-0.0.5/palamedes/hgvs/builders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2973 2024-04-18 18:25:35.000000 palamedes-0.0.5/palamedes/hgvs/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2047 2024-04-18 18:25:35.000000 palamedes-0.0.5/palamedes/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3416 2024-04-18 18:25:35.000000 palamedes-0.0.5/palamedes/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:25:47.610363 palamedes-0.0.5/palamedes.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5269 2024-04-18 18:25:47.000000 palamedes-0.0.5/palamedes.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      599 2024-04-18 18:25:47.000000 palamedes-0.0.5/palamedes.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 18:25:47.000000 palamedes-0.0.5/palamedes.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-18 18:25:47.000000 palamedes-0.0.5/palamedes.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-18 18:25:47.000000 palamedes-0.0.5/palamedes.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-18 18:25:47.000000 palamedes-0.0.5/palamedes.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 18:25:47.610363 palamedes-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      889 2024-04-18 18:25:35.000000 palamedes-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:25:47.606363 palamedes-0.0.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 18:25:35.000000 palamedes-0.0.5/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-04-18 18:25:35.000000 palamedes-0.0.5/tests/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:25:47.610363 palamedes-0.0.5/tests/hgvs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 18:25:35.000000 palamedes-0.0.5/tests/hgvs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10431 2024-04-18 18:25:35.000000 palamedes-0.0.5/tests/hgvs/test_builders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9293 2024-04-18 18:25:35.000000 palamedes-0.0.5/tests/hgvs/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12977 2024-04-18 18:25:35.000000 palamedes-0.0.5/tests/test_align.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1915 2024-04-18 18:25:35.000000 palamedes-0.0.5/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3650 2024-04-18 18:25:35.000000 palamedes-0.0.5/tests/test_utils.py
```

### Comparing `palamedes-0.0.3/LICENSE.txt` & `palamedes-0.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `palamedes-0.0.3/PKG-INFO` & `palamedes-0.0.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: palamedes
-Version: 0.0.3
+Version: 0.0.5
 Summary: Palamedes: HGVS variants from a sequence alignment
 Home-page: https://github.com/mammothbio-os/palamedes
 Author-email: open-source@mammothbiosci.com
 Keywords: bioinformatics,alignment,hgvs,variant,amino acid
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.11
@@ -23,15 +23,17 @@
 
 ## Documentation
 
 Documentation for the project can be found [here](https://mammothbio-os-palamedes.readthedocs.io/en/stable/)
 
 ## Installing
 
-Palamedes is packaged in PyPI, to install simply run: `pip install palamedes`
+Palamedes uses the [hgvs](https://github.com/biocommons/hgvs) package as a dependency. At this time, `hgvs` requires `postgresql` system dependencies to be installed before use. Please see the [README](https://github.com/biocommons/hgvs/blob/main/README.md#installing-hgvs-locally) for install instructions if needed.
+
+Palamedes itself is packaged in PyPI, to install simply run: `pip install palamedes`
 
 ## Usage - CLI
 
 Palamedes includes a CLI entrypoint, which is mostly useful for debugging and exploration. Once installed, simply run `palamedes` and provide a reference and alternate sequence:
 ```shell
 palamedes PFKISIHL TPFKISIH
 [2024-03-25 11:40:59,904] {cli.py:39} INFO - Running with args: Namespace(ref='PFKISIHL', alt='TPFKISIH', molecule_type='protein')
```

### Comparing `palamedes-0.0.3/README.md` & `palamedes-0.0.5/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,17 @@
 
 ## Documentation
 
 Documentation for the project can be found [here](https://mammothbio-os-palamedes.readthedocs.io/en/stable/)
 
 ## Installing
 
-Palamedes is packaged in PyPI, to install simply run: `pip install palamedes`
+Palamedes uses the [hgvs](https://github.com/biocommons/hgvs) package as a dependency. At this time, `hgvs` requires `postgresql` system dependencies to be installed before use. Please see the [README](https://github.com/biocommons/hgvs/blob/main/README.md#installing-hgvs-locally) for install instructions if needed.
+
+Palamedes itself is packaged in PyPI, to install simply run: `pip install palamedes`
 
 ## Usage - CLI
 
 Palamedes includes a CLI entrypoint, which is mostly useful for debugging and exploration. Once installed, simply run `palamedes` and provide a reference and alternate sequence:
 ```shell
 palamedes PFKISIHL TPFKISIH
 [2024-03-25 11:40:59,904] {cli.py:39} INFO - Running with args: Namespace(ref='PFKISIHL', alt='TPFKISIH', molecule_type='protein')
```

### Comparing `palamedes-0.0.3/palamedes/__init__.py` & `palamedes-0.0.5/palamedes/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 from palamedes.config import MOLECULE_TYPE_PROTEIN, ALT_SEQUENCE_ID, REF_SEQUENCE_ID
 from palamedes.align import generate_seq_record, generate_alignment, generate_variant_blocks
 from palamedes.hgvs.utils import categorize_variant_block
 from palamedes.hgvs.builders import BUILDER_CONFIG
 
 
-__version__ = "0.0.3"
+__version__ = "0.0.5"
 
 
 def generate_hgvs_variants(
     reference_sequence: str | SeqRecord,
     alternate_sequence: str | SeqRecord,
     molecule_type: str = MOLECULE_TYPE_PROTEIN,
     aligner: PairwiseAligner | None = None,
```

### Comparing `palamedes-0.0.3/palamedes/__main__.py` & `palamedes-0.0.5/palamedes/__main__.py`

 * *Files identical despite different names*

### Comparing `palamedes-0.0.3/palamedes/align.py` & `palamedes-0.0.5/palamedes/align.py`

 * *Files 10% similar despite different names*

```diff
@@ -32,14 +32,32 @@
     return SeqRecord(
         Seq(sequence),
         id=seq_id,
         annotations={MOLECULE_TYPE_ANNOTATION_KEY: molecule_type},
     )
 
 
+def reverse_seq_record(seq_record: SeqRecord) -> SeqRecord:
+    """
+    Helper function to copy a SeqRecord into a new one, with the sequence reversed. This is a best effort copy,
+    which is only used internally to the alignment logic to more easily access the 3' end most representation of
+    the best alignment.
+    """
+    return SeqRecord(
+        Seq(seq_record.seq[::-1]),
+        id=seq_record.id,
+        name=seq_record.name,
+        description=seq_record.description,
+        dbxrefs=seq_record.dbxrefs[:],
+        features=seq_record.features[:],
+        annotations=seq_record.annotations.copy(),
+        letter_annotations=seq_record.letter_annotations.copy(),
+    )
+
+
 def make_variant_base(ref_base: str, alt_base: str) -> str:
     """Helper function to generate the correct variant base given the ref and alt alignment bases"""
     if ref_base == alt_base:
         return VARIANT_BASE_MATCH
 
     if ref_base == ALIGNMENT_GAP_CHAR:
         return VARIANT_BASE_INSERTION
@@ -165,27 +183,38 @@
 
     if (alt_molecule_type := alternate_seq_record.annotations.get("molecule_type")) != molecule_type:
         raise ValueError(
             "Cannot generate alignment, alternate_seq_record is a SeqRecord an invalid molecule_type annotation "
             f"got: {alt_molecule_type}, expected: {molecule_type}!"
         )
 
-    alignments = aligner.align(reference_seq_record, alternate_seq_record)
-    best_alignment = next(alignments)
-    best_alignment_score = best_alignment.score
-
-    other_alignments_with_best = [alignment for alignment in alignments if alignment.score == best_alignment_score]
-    if len(other_alignments_with_best) > 0:
-        LOGGER.debug(
-            "Found %s alignments with max score, returning last in the list (3' end rule)",
-            len(other_alignments_with_best) + 1,
-        )
-        best_alignment = other_alignments_with_best[-1]
+    # reverse the sequences and then align the reversed, keeping the first best alignment
+    reversed_ref_seq_record = reverse_seq_record(reference_seq_record)
+    reversed_alt_seq_record = reverse_seq_record(alternate_seq_record)
+    reversed_alignments = aligner.align(reversed_ref_seq_record, reversed_alt_seq_record)
+    reversed_alignment = reversed_alignments[0]
+
+    # undo the reversal, to recover the "last" highest scoring alignment for the forward
+    # which should correspond to the 3' end most alignment and follow HGSV spec
+    # note 'infer_coordinates' will soon be deprecated, update to 'parse_printed_alignment' once its live
+    forward_coordinates = Alignment.infer_coordinates(
+        [
+            reversed_alignment[0][::-1],
+            reversed_alignment[1][::-1],
+        ]
+    )
+    forward_alignment = Alignment(
+        [reference_seq_record, alternate_seq_record],
+        forward_coordinates,
+    )
+
+    # score is not technically an attribute on the class
+    setattr(forward_alignment, "score", reversed_alignment.score)
 
-    return best_alignment
+    return forward_alignment
 
 
 def generate_variant_blocks(alignment: Alignment) -> list[VariantBlock]:
     """
     Given a BioPython.Alignment object, parse the alignment to generate a list of VariantBlock objects.
     A VariantBlock is an internal object which represents a contiguous run of positions within the alignment
     which are not matches (mismatch, del or ins). These blocks will be categorized and converted into HGVS
```

### Comparing `palamedes-0.0.3/palamedes/config.py` & `palamedes-0.0.5/palamedes/config.py`

 * *Files identical despite different names*

### Comparing `palamedes-0.0.3/palamedes/hgvs/builders.py` & `palamedes-0.0.5/palamedes/hgvs/builders.py`

 * *Files identical despite different names*

### Comparing `palamedes-0.0.3/palamedes/hgvs/utils.py` & `palamedes-0.0.5/palamedes/hgvs/utils.py`

 * *Files identical despite different names*

### Comparing `palamedes-0.0.3/palamedes/models.py` & `palamedes-0.0.5/palamedes/models.py`

 * *Files identical despite different names*

### Comparing `palamedes-0.0.3/palamedes/utils.py` & `palamedes-0.0.5/palamedes/utils.py`

 * *Files identical despite different names*

### Comparing `palamedes-0.0.3/palamedes.egg-info/PKG-INFO` & `palamedes-0.0.5/palamedes.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: palamedes
-Version: 0.0.3
+Version: 0.0.5
 Summary: Palamedes: HGVS variants from a sequence alignment
 Home-page: https://github.com/mammothbio-os/palamedes
 Author-email: open-source@mammothbiosci.com
 Keywords: bioinformatics,alignment,hgvs,variant,amino acid
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.11
@@ -23,15 +23,17 @@
 
 ## Documentation
 
 Documentation for the project can be found [here](https://mammothbio-os-palamedes.readthedocs.io/en/stable/)
 
 ## Installing
 
-Palamedes is packaged in PyPI, to install simply run: `pip install palamedes`
+Palamedes uses the [hgvs](https://github.com/biocommons/hgvs) package as a dependency. At this time, `hgvs` requires `postgresql` system dependencies to be installed before use. Please see the [README](https://github.com/biocommons/hgvs/blob/main/README.md#installing-hgvs-locally) for install instructions if needed.
+
+Palamedes itself is packaged in PyPI, to install simply run: `pip install palamedes`
 
 ## Usage - CLI
 
 Palamedes includes a CLI entrypoint, which is mostly useful for debugging and exploration. Once installed, simply run `palamedes` and provide a reference and alternate sequence:
 ```shell
 palamedes PFKISIHL TPFKISIH
 [2024-03-25 11:40:59,904] {cli.py:39} INFO - Running with args: Namespace(ref='PFKISIHL', alt='TPFKISIH', molecule_type='protein')
```

### Comparing `palamedes-0.0.3/palamedes.egg-info/SOURCES.txt` & `palamedes-0.0.5/palamedes.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `palamedes-0.0.3/setup.py` & `palamedes-0.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import find_packages, setup
 
-version = "0.0.3"
+version = "0.0.5"
 
 setup(
     name="palamedes",
     version=version,
     url="https://github.com/mammothbio-os/palamedes",
     python_requires=">=3.11",
     description="Palamedes: HGVS variants from a sequence alignment",
```

### Comparing `palamedes-0.0.3/tests/base.py` & `palamedes-0.0.5/tests/base.py`

 * *Files identical despite different names*

### Comparing `palamedes-0.0.3/tests/hgvs/test_builders.py` & `palamedes-0.0.5/tests/hgvs/test_builders.py`

 * *Files identical despite different names*

### Comparing `palamedes-0.0.3/tests/hgvs/test_utils.py` & `palamedes-0.0.5/tests/hgvs/test_utils.py`

 * *Files identical despite different names*

### Comparing `palamedes-0.0.3/tests/test_align.py` & `palamedes-0.0.5/tests/test_align.py`

 * *Files 19% similar despite different names*

```diff
@@ -193,14 +193,65 @@
 
         custom_match_score = 10_000
         custom_aligner = PairwiseAligner(mode=GLOBAL_ALIGN_MODE, match_score=custom_match_score)
 
         alignment = generate_alignment(ref, alt, aligner=custom_aligner)
         self.assertTrue(alignment.score, custom_match_score)
 
+    def test_generate_alignment_three_prime_end_most_del(self):
+        ref, alt = self.make_seq_records(
+            "T" + "A" * 10 + "G",
+            "T" + "A" * 9 + "G",
+        )
+
+        alignment = generate_alignment(ref, alt)
+
+        # ensure we get the ref unchanged
+        # and the last A deleted, not any others
+        self.assertEqual(alignment[0], ref.seq)
+        self.assertEqual(alignment[1], "T" + "A" * 9 + "-G")
+
+    def test_generate_alignment_three_prime_end_most_double_del(self):
+        ref, alt = self.make_seq_records(
+            "ATTGCCA",
+            "ATGCA",
+        )
+
+        alignment = generate_alignment(ref, alt)
+
+        # ensure we get the ref unchanged
+        # and the second of each paired based deleted
+        self.assertEqual(alignment[0], ref.seq)
+        self.assertEqual(alignment[1], "AT-GC-A")
+
+    def test_generate_alignment_three_prime_end_most_ins(self):
+        ref, alt = self.make_seq_records(
+            "T" + "A" * 9 + "G",
+            "T" + "A" * 10 + "G",
+        )
+
+        alignment = generate_alignment(ref, alt)
+
+        # ensure we get the alt unchanged
+        # and the insertion happens after the last A in the ref
+        self.assertEqual(alignment[0], "T" + "A" * 9 + "-G")
+        self.assertEqual(alignment[1], alt.seq)
+
+    def test_generate_alignment_three_prime_end_most_double_ins(self):
+        ref, alt = self.make_seq_records(
+            "ATGCA",
+            "ATTGCCA",
+        )
+        alignment = generate_alignment(ref, alt)
+
+        # ensure we get the alt unchanged
+        # and the insertion happens after the last A in the ref
+        self.assertEqual(alignment[0], "AT-GC-A")
+        self.assertEqual(alignment[1], alt.seq)
+
 
 class GenerateVariantBlocksTestCase(PalamedesBaseCase):
     def test_generate_variant_blocks_all_matches(self):
         alignment = self.make_alignment("A" * 5, "A" * 5)
         self.assertEqual(generate_variant_blocks(alignment), [])
 
     def test_generate_variant_blocks_all_matches_single_mismatch(self):
```

### Comparing `palamedes-0.0.3/tests/test_models.py` & `palamedes-0.0.5/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `palamedes-0.0.3/tests/test_utils.py` & `palamedes-0.0.5/tests/test_utils.py`

 * *Files identical despite different names*

