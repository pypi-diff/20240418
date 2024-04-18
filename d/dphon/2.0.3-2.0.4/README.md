# Comparing `tmp/dphon-2.0.3.tar.gz` & `tmp/dphon-2.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dphon-2.0.3.tar", last modified: Mon Feb  5 18:13:25 2024, max compression
+gzip compressed data, was "dphon-2.0.4.tar", last modified: Thu Apr 18 04:15:17 2024, max compression
```

## Comparing `dphon-2.0.3.tar` & `dphon-2.0.4.tar`

### file list

```diff
@@ -1,40 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 18:13:25.609511 dphon-2.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-02-05 18:12:59.000000 dphon-2.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-02-05 18:12:59.000000 dphon-2.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    11418 2024-02-05 18:13:25.609511 dphon-2.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8964 2024-02-05 18:12:59.000000 dphon-2.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 18:13:25.609511 dphon-2.0.3/dphon/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-02-05 18:12:59.000000 dphon-2.0.3/dphon/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4547 2024-02-05 18:12:59.000000 dphon-2.0.3/dphon/align.py
--rw-r--r--   0 runner    (1001) docker     (127)     8817 2024-02-05 18:12:59.000000 dphon-2.0.3/dphon/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     4938 2024-02-05 18:12:59.000000 dphon-2.0.3/dphon/console.py
--rw-r--r--   0 runner    (1001) docker     (127)     6842 2024-02-05 18:12:59.000000 dphon-2.0.3/dphon/corpus.py
--rw-r--r--   0 runner    (1001) docker     (127)     7403 2024-02-05 18:12:59.000000 dphon-2.0.3/dphon/extend.py
--rw-r--r--   0 runner    (1001) docker     (127)     7328 2024-02-05 18:12:59.000000 dphon-2.0.3/dphon/g2p.py
--rw-r--r--   0 runner    (1001) docker     (127)     6057 2024-02-05 18:12:59.000000 dphon-2.0.3/dphon/index.py
--rw-r--r--   0 runner    (1001) docker     (127)     2479 2024-02-05 18:12:59.000000 dphon-2.0.3/dphon/match.py
--rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-02-05 18:12:59.000000 dphon-2.0.3/dphon/ngrams.py
--rw-r--r--   0 runner    (1001) docker     (127)     4478 2024-02-05 18:12:59.000000 dphon-2.0.3/dphon/reuse.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 18:13:25.609511 dphon-2.0.3/dphon.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11418 2024-02-05 18:13:25.000000 dphon-2.0.3/dphon.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      673 2024-02-05 18:13:25.000000 dphon-2.0.3/dphon.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-05 18:13:25.000000 dphon-2.0.3/dphon.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      211 2024-02-05 18:13:25.000000 dphon-2.0.3/dphon.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-02-05 18:13:25.000000 dphon-2.0.3/dphon.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-02-05 18:13:25.000000 dphon-2.0.3/dphon.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-02-05 18:12:59.000000 dphon-2.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-02-05 18:13:25.609511 dphon-2.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2039 2024-02-05 18:12:59.000000 dphon-2.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 18:13:25.609511 dphon-2.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-05 18:12:59.000000 dphon-2.0.3/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 18:13:25.609511 dphon-2.0.3/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-05 18:12:59.000000 dphon-2.0.3/tests/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5013 2024-02-05 18:12:59.000000 dphon-2.0.3/tests/unit/test_align.py
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-02-05 18:12:59.000000 dphon-2.0.3/tests/unit/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     2460 2024-02-05 18:12:59.000000 dphon-2.0.3/tests/unit/test_corpus.py
--rw-r--r--   0 runner    (1001) docker     (127)    12543 2024-02-05 18:12:59.000000 dphon-2.0.3/tests/unit/test_extend.py
--rw-r--r--   0 runner    (1001) docker     (127)     4710 2024-02-05 18:12:59.000000 dphon-2.0.3/tests/unit/test_g2p.py
--rw-r--r--   0 runner    (1001) docker     (127)     3233 2024-02-05 18:12:59.000000 dphon-2.0.3/tests/unit/test_index.py
--rw-r--r--   0 runner    (1001) docker     (127)     1926 2024-02-05 18:12:59.000000 dphon-2.0.3/tests/unit/test_match.py
--rw-r--r--   0 runner    (1001) docker     (127)     2599 2024-02-05 18:12:59.000000 dphon-2.0.3/tests/unit/test_ngrams.py
--rw-r--r--   0 runner    (1001) docker     (127)     3001 2024-02-05 18:12:59.000000 dphon-2.0.3/tests/unit/test_reuse.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 04:15:17.765501 dphon-2.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-18 04:14:41.000000 dphon-2.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-18 04:14:41.000000 dphon-2.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    11702 2024-04-18 04:15:17.765501 dphon-2.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8973 2024-04-18 04:14:41.000000 dphon-2.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 04:15:17.761501 dphon-2.0.4/dphon/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-18 04:14:41.000000 dphon-2.0.4/dphon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4547 2024-04-18 04:14:41.000000 dphon-2.0.4/dphon/align.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8817 2024-04-18 04:14:41.000000 dphon-2.0.4/dphon/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4938 2024-04-18 04:14:41.000000 dphon-2.0.4/dphon/console.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6842 2024-04-18 04:14:41.000000 dphon-2.0.4/dphon/corpus.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 04:15:17.761501 dphon-2.0.4/dphon/data/
+-rw-r--r--   0 runner    (1001) docker     (127)     2322 2024-04-18 04:14:41.000000 dphon-2.0.4/dphon/data/oc-consonants.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-18 04:14:41.000000 dphon-2.0.4/dphon/data/oc-vowels.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   354021 2024-04-18 04:14:41.000000 dphon-2.0.4/dphon/data/sound_table_v1.json
+-rw-r--r--   0 runner    (1001) docker     (127)   814074 2024-04-18 04:14:41.000000 dphon-2.0.4/dphon/data/sound_table_v2.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7403 2024-04-18 04:14:41.000000 dphon-2.0.4/dphon/extend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7328 2024-04-18 04:14:41.000000 dphon-2.0.4/dphon/g2p.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6057 2024-04-18 04:14:41.000000 dphon-2.0.4/dphon/index.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2479 2024-04-18 04:14:41.000000 dphon-2.0.4/dphon/match.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-04-18 04:14:41.000000 dphon-2.0.4/dphon/ngrams.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4478 2024-04-18 04:14:41.000000 dphon-2.0.4/dphon/reuse.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 04:15:17.765501 dphon-2.0.4/dphon.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11702 2024-04-18 04:15:17.000000 dphon-2.0.4/dphon.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      505 2024-04-18 04:15:17.000000 dphon-2.0.4/dphon.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 04:15:17.000000 dphon-2.0.4/dphon.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-04-18 04:15:17.000000 dphon-2.0.4/dphon.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-18 04:15:17.000000 dphon-2.0.4/dphon.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-18 04:15:17.000000 dphon-2.0.4/dphon.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1779 2024-04-18 04:14:41.000000 dphon-2.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 04:15:17.765501 dphon-2.0.4/setup.cfg
```

### Comparing `dphon-2.0.3/LICENSE` & `dphon-2.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `dphon-2.0.3/README.md` & `dphon-2.0.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 # dphon
+
 [![ci](https://github.com/direct-phonology/dphon/workflows/ci/badge.svg)](https://github.com/direct-phonology/dphon/actions?query=workflow%3Aci)
 [![codecov](https://codecov.io/gh/direct-phonology/dphon/branch/main/graph/badge.svg?token=uGbgB5UFtk)](https://codecov.io/gh/direct-phonology/dphon)
 ![pyversions](https://img.shields.io/pypi/pyversions/dphon.svg?style=flat)
 [![zenodo](https://zenodo.org/badge/DOI/10.5281/zenodo.4641277.svg)](https://zenodo.org/record/4641277)
 [![spaCy](https://img.shields.io/static/v1?label=made%20with%20%E2%9D%A4%20and&message=spaCy&color=09a3d5)](https://spacy.io)
 [![code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
@@ -15,14 +16,15 @@
 ```
 
 if you're on windows and are seeing incorrectly formatted output in your terminal, have a look at this [stackoverflow answer](https://stackoverflow.com/questions/49476326/displaying-unicode-in-powershell/49481797#49481797).
 
 ## usage
 
 ### basics
+
 the main function of `dphon` is to look for instances of text reuse in a corpus of old chinese texts. instead of relying purely on graphemes, it does this by performing grapheme-to-phoneme conversion, and determining possible reuse based on whether passages are likely to have _sounded_ similar (or rhymed) when spoken aloud.
 
 you will need to have files stored locally as utf-8 encoded plain-text (`.txt`) or json-lines (`.jsonl`) format. for the former, one file is assumed to represent one document. for the latter, one file can contain any number of lines, each of which is a document, with required keys `id` (a unique identifier) and `text` (text content) and any number of optional keys. you can obtain a representative corpus of old chinese sourced from the kanseki repository via [`direct-phonology/ect-krp`](https://github.com/direct-phonology/ect-krp).
 
 a simple invocation of `dphon` might look like:
 
 ```sh
@@ -38,33 +40,36 @@
 2.  text_b (3340–3348)：
     不可弗爲以爲可　故爲之爲之繇其道物
     *ləʔ ɢʷraj kʰˤajʔ kˤaʔs ɢʷraj tə ɢʷraj tə pit
 ```
 
 the numbers next to the identifiers are _token indices_, and may vary depending on how the text is tokenized – `dphon` currently uses character-based tokenization. whitespace will be removed, and the output will be aligned to make it easier to spot differences between the two sequences. by default, insertions are highlighted in green, and mismatches (differences between the two sequences) are highlighted in red. additional (non-matching) context added to either side of match sequences is displayed using a dimmed color (see "advanced usage" below for more information on colorization).
 
-matches are sorted by the ratio of their phomenic similarity to their graphic similarity – in other words, matches between texts that sound highly similar but were written very differently will be at the top of the list. 
+matches are sorted by the ratio of their phomenic similarity to their graphic similarity – in other words, matches between texts that sound highly similar but were written very differently will be at the top of the list.
 
 by default, `dphon` only returns matches that display at least one instance of _graphic variation_ – a case where two different graphemes are used in the same place to represent the same sound. these cases are highlighted in blue. if you're interested in all instances of reuse, regardless of graphic variation, you can use the `--all` flag:
 
 ```sh
 $ dphon --all text_a.txt text_b.txt
 ```
 
 you can view the full list of command options with:
+
 ```sh
 $ dphon --help
 ```
 
 this tool is under active development, and results may vary. to find the version you are running:
+
 ```sh
 $ dphon --version
 ```
 
 ### advanced usage
+
 by default, `dphon` uses your system's `$PAGER` to display output, since the results can be quite long. on MacOS and Linux, this will likely be `less`, which supports additional options like searching through the output once it's displayed. for more information, see the man page:
 
 ```sh
 $ man less
 ```
 
 `dphon` can colorize output for nicer display in the terminal if your pager supports it. to enable this behavior on MacOS and Linux, set `LESS=R`:
@@ -96,15 +101,15 @@
 ...
 ```
 
 if two characters have the same phonemes, they're treated as a match. for characters with multiple readings, `dphon` currently chooses the first available reading for comparison. more work is planned for version 3.0 to address this shortcoming.
 
 in version 1.0, `dphon`'s default reconstruction was based on Schuessler 2007[<sup>1</sup>](#note1), but used a single "dummy" character to represent all the lexemes in a rhyming group. [the dictionary](dphon/data/sound_table_v1.json) was compiled by John O'Leary ([@valgrinderror](https://github.com/valgrinderror)) and Gian Duri Rominger ([@GDRom](https://github.com/GDRom)). since version 2.0, `dphon` uses [a dictionary](dphon/data/sound_table_v2.json) based on the Baxter-Sagart 2014 reconstruction[<sup>2</sup>](#note2), with additional work by Rominger.
 
-the matching algorithm is based on Paul Vierthaler's [`chinesetextreuse`](https://github.com/vierth/chinesetextreuse) project[<sup>3</sup>](#note3), with some modifications. it uses a [BLAST](https://en.wikipedia.org/wiki/BLAST_(biotechnology))-like strategy to identify initial match candidates, and then extend them via phonetic [edit distance](https://en.wikipedia.org/wiki/Edit_distance) comparison. finally, the results are aligned using a version of the [Smith-Waterman algorithm](https://en.wikipedia.org/wiki/Smith%E2%80%93Waterman_algorithm) that operates on phonemes, powered by the `lingpy` library[<sup>4</sup>](#note4).
+the matching algorithm is based on Paul Vierthaler's [`chinesetextreuse`](https://github.com/vierth/chinesetextreuse) project[<sup>3</sup>](#note3), with some modifications. it uses a [BLAST](<https://en.wikipedia.org/wiki/BLAST_(biotechnology)>)-like strategy to identify initial match candidates, and then extend them via phonetic [edit distance](https://en.wikipedia.org/wiki/Edit_distance) comparison. finally, the results are aligned using a version of the [Smith-Waterman algorithm](https://en.wikipedia.org/wiki/Smith%E2%80%93Waterman_algorithm) that operates on phonemes, powered by the `lingpy` library[<sup>4</sup>](#note4).
 
 ## development setup
 
 first, clone the repository:
 
 ```sh
 $ git clone https://github.com/direct-phonology/dphon.git
@@ -129,30 +134,33 @@
 ```sh
 $ pip install -e .
 ```
 
 now your changes will be automatically picked up when you run `dphon`.
 
 pull requests can be made against `main`.
+
 ## code documentation
+
 code documentation is [available on github pages](https://direct-phonology.github.io/dphon) and is generated with `pdoc3`.
 
 to build the docs:
+
 ```sh
 $ pdoc --html --output-dir docs dphon
 ```
 
 ## tests
+
 unit tests are written with `unittest`. you can run them with:
 
 ```sh
 $ python -m unittest
 ```
 
-
 ## releases
 
 the package is built and published to pyPI automatically using `twine` when using GitHub's release functionality.
 
 **make sure the version number in `dphon/__init__.py` is correct!**
 
 <hr/>
```

### Comparing `dphon-2.0.3/dphon/align.py` & `dphon-2.0.4/dphon/align.py`

 * *Files identical despite different names*

### Comparing `dphon-2.0.3/dphon/cli.py` & `dphon-2.0.4/dphon/cli.py`

 * *Files identical despite different names*

### Comparing `dphon-2.0.3/dphon/console.py` & `dphon-2.0.4/dphon/console.py`

 * *Files identical despite different names*

### Comparing `dphon-2.0.3/dphon/corpus.py` & `dphon-2.0.4/dphon/corpus.py`

 * *Files identical despite different names*

### Comparing `dphon-2.0.3/dphon/extend.py` & `dphon-2.0.4/dphon/extend.py`

 * *Files identical despite different names*

### Comparing `dphon-2.0.3/dphon/g2p.py` & `dphon-2.0.4/dphon/g2p.py`

 * *Files identical despite different names*

### Comparing `dphon-2.0.3/dphon/index.py` & `dphon-2.0.4/dphon/index.py`

 * *Files identical despite different names*

### Comparing `dphon-2.0.3/dphon/match.py` & `dphon-2.0.4/dphon/match.py`

 * *Files identical despite different names*

### Comparing `dphon-2.0.3/dphon/ngrams.py` & `dphon-2.0.4/dphon/ngrams.py`

 * *Files identical despite different names*

### Comparing `dphon-2.0.3/dphon/reuse.py` & `dphon-2.0.4/dphon/reuse.py`

 * *Files identical despite different names*

