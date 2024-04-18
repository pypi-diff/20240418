# Comparing `tmp/ptcr-0.1.8.tar.gz` & `tmp/ptcr-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ptcr-0.1.8.tar", last modified: Thu Apr 18 19:48:32 2024, max compression
+gzip compressed data, was "ptcr-0.1.9.tar", last modified: Thu Apr 18 19:58:14 2024, max compression
```

## Comparing `ptcr-0.1.8.tar` & `ptcr-0.1.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2024-04-18 19:48:32.378819 ptcr-0.1.8/
--rw-rw-rw-   0        0        0     1069 2024-04-16 23:53:12.000000 ptcr-0.1.8/LICENSE
--rw-rw-rw-   0        0        0    12865 2024-04-18 19:48:32.377812 ptcr-0.1.8/PKG-INFO
--rw-rw-rw-   0        0        0    12299 2024-04-18 19:47:24.000000 ptcr-0.1.8/README.md
-drwxrwxrwx   0        0        0        0 2024-04-18 19:48:32.283226 ptcr-0.1.8/ptcr.egg-info/
--rw-rw-rw-   0        0        0    12865 2024-04-18 19:48:32.000000 ptcr-0.1.8/ptcr.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      343 2024-04-18 19:48:32.000000 ptcr-0.1.8/ptcr.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-18 19:48:32.000000 ptcr-0.1.8/ptcr.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      180 2024-04-18 19:48:32.000000 ptcr-0.1.8/ptcr.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-04-18 19:48:32.000000 ptcr-0.1.8/ptcr.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-18 19:48:32.375836 ptcr-0.1.8/ptcr2/
--rw-rw-rw-   0        0        0        0 2024-02-23 22:22:15.000000 ptcr-0.1.8/ptcr2/__init__.py
--rw-rw-rw-   0        0        0     7664 2024-03-06 16:01:26.000000 ptcr-0.1.8/ptcr2/automata_utility.py
--rw-rw-rw-   0        0        0     3681 2024-04-16 13:50:12.000000 ptcr-0.1.8/ptcr2/base_model.py
--rw-rw-rw-   0        0        0     3364 2024-04-07 16:47:54.000000 ptcr-0.1.8/ptcr2/belief_tree.py
--rw-rw-rw-   0        0        0    27773 2024-04-16 23:22:39.000000 ptcr-0.1.8/ptcr2/event_predictor.py
--rw-rw-rw-   0        0        0    10168 2024-04-07 21:33:36.000000 ptcr-0.1.8/ptcr2/fom.py
--rw-rw-rw-   0        0        0     9897 2024-04-07 16:36:30.000000 ptcr-0.1.8/ptcr2/markov_chain.py
--rw-rw-rw-   0        0        0    75894 2024-04-07 21:39:01.000000 ptcr-0.1.8/ptcr2/markov_decision_process.py
--rw-rw-rw-   0        0        0       42 2024-04-18 19:48:32.378819 ptcr-0.1.8/setup.cfg
--rw-rw-rw-   0        0        0     1047 2024-04-18 19:40:14.000000 ptcr-0.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-18 19:58:14.737403 ptcr-0.1.9/
+-rw-rw-rw-   0        0        0     1069 2024-04-16 23:53:12.000000 ptcr-0.1.9/LICENSE
+-rw-rw-rw-   0        0        0    12804 2024-04-18 19:58:14.737403 ptcr-0.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0    12280 2024-04-18 19:57:39.000000 ptcr-0.1.9/README.md
+drwxrwxrwx   0        0        0        0 2024-04-18 19:58:14.725662 ptcr-0.1.9/ptcr.egg-info/
+-rw-rw-rw-   0        0        0    12804 2024-04-18 19:58:14.000000 ptcr-0.1.9/ptcr.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      343 2024-04-18 19:58:14.000000 ptcr-0.1.9/ptcr.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-18 19:58:14.000000 ptcr-0.1.9/ptcr.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      180 2024-04-18 19:58:14.000000 ptcr-0.1.9/ptcr.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-04-18 19:58:14.000000 ptcr-0.1.9/ptcr.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-18 19:58:14.735658 ptcr-0.1.9/ptcr2/
+-rw-rw-rw-   0        0        0        0 2024-02-23 22:22:15.000000 ptcr-0.1.9/ptcr2/__init__.py
+-rw-rw-rw-   0        0        0     7664 2024-03-06 16:01:26.000000 ptcr-0.1.9/ptcr2/automata_utility.py
+-rw-rw-rw-   0        0        0     3681 2024-04-16 13:50:12.000000 ptcr-0.1.9/ptcr2/base_model.py
+-rw-rw-rw-   0        0        0     3364 2024-04-07 16:47:54.000000 ptcr-0.1.9/ptcr2/belief_tree.py
+-rw-rw-rw-   0        0        0    27773 2024-04-16 23:22:39.000000 ptcr-0.1.9/ptcr2/event_predictor.py
+-rw-rw-rw-   0        0        0    10168 2024-04-07 21:33:36.000000 ptcr-0.1.9/ptcr2/fom.py
+-rw-rw-rw-   0        0        0     9897 2024-04-07 16:36:30.000000 ptcr-0.1.9/ptcr2/markov_chain.py
+-rw-rw-rw-   0        0        0    75894 2024-04-07 21:39:01.000000 ptcr-0.1.9/ptcr2/markov_decision_process.py
+-rw-rw-rw-   0        0        0       42 2024-04-18 19:58:14.737403 ptcr-0.1.9/setup.cfg
+-rw-rw-rw-   0        0        0     1047 2024-04-18 19:58:07.000000 ptcr-0.1.9/setup.py
```

### Comparing `ptcr-0.1.8/LICENSE` & `ptcr-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ptcr-0.1.8/PKG-INFO` & `ptcr-0.1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ptcr
-Version: 0.1.8
+Version: 0.1.9
 Summary: Constructs and simulates PTCR models.
 Home-page: https://github.com/T-Lind/ptcr
 Author: Tiernan Lindauer
 Author-email: tiernanlind@tamu.edu
 License: MIT
 Keywords: PTCR,FOM,simulation,optimization,decision making,models
 Classifier: Programming Language :: Python :: 3
@@ -23,36 +23,36 @@
 This work implements and extends the work of Dylan A. Shell and Hazhar Rahmani in their paper ["Planning to chronicle: Optimal policies for narrative observation of unpredictable events"](https://journals.sagepub.com/doi/pdf/10.1177/02783649211069154).
 An excerpt from the paper is as follows:
 
 "An important class of applications entails a robot monitoring, scrutinizing, or recording the evolution of an uncertain
 time-extended process. This sort of situation leads to an interesting family
 of planning problems in which the robot is limited in what it sees and must, thus, choose what to pay attention to.
 The distinguishing characteristic of this setting is that the robot has influence over what it  captures via its sensors,
-but exercises no causal authority over the evolving process. As such, the robotâ€™s objective is to observe the underlying
-process and to produce a â€˜chronicleâ€™ of current events, subject to a
+but exercises no causal authority over the evolving process. As such, the robot's objective is to observe the underlying
+process and to produce a 'chronicle' of current events, subject to a
 goal specification of the sorts of event sequences that may be of interest.
 This paper examines variants of such problems when the robot aims to
 collect sets of observations to meet a rich specification of their sequential structure. We study this class of problems by modeling a stochastic
 process via a variant of a hidden Markov model, and specify the event
-sequences of interest as a regular language, developing a vocabulary of
-â€˜mutatorsâ€™ that enable sophisticated requirements to be expressed. Under different suppositions about the information gleaned about the event
+sequences of interest as a regular language, developing a vocabulary of 'mutators'
+that enable sophisticated requirements to be expressed. Under different suppositions about the information gleaned about the event
 model, we formulate and solve different planning problems. The core underlying idea is the construction of a product between the event model
 and a specification automaton.
 
 "A concrete motivation for this sort of setting, consider the
 proliferation of home videos. These videos are, with remarkably few exceptions,
 crummy specimens of the cinematic arts. They fail, generally, to establish and
 then bracket a scene; they often founder in emphasizing the importance of key
 subjects within the developing action, and are usually unsuccessful in attempts
 to trace an evolving narrative arc. And the current generation of autonomous
-personal robots and video drones, in their roles as costly and glorified â€˜selfie
-sticks,â€™ are set to follow suit. The trouble is that capturing footage to tell a story
+personal robots and video drones, in their roles as costly and glorified 'selfie sticks'
+are set to follow suit. The trouble is that capturing footage to tell a story
 is challenging. A camera can only record what you point it toward, so part of
-the difficulty stems from the fact that you canâ€™t know exactly how the scene will
-unfold before it actually does. Moreover, what constitutes structure isnâ€™t easily
+the difficulty stems from the fact that you can't know exactly how the scene will
+unfold before it actually does. Moreover, what constitutes structure isn't easily
 summed up with a few trite quantities. Another part of the challenge, of course,
 is that one has only limited time to capture video footage.
 Setting aside pure vanity as a motivator, many applications can be cast as
 the problem of producing a finite-length sensor-based recording of the evolution
 of some process. As the video example emphasizes, one might be interested
 in recordings that meet rich specifications of the event sequences that are of
 interest. When the evolution of the event-generating process is uncertain/nondeterministic and sensing is local (necessitating its active direction), then one
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `ptcr-0.1.8/README.md` & `ptcr-0.1.9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -7,36 +7,36 @@
 This work implements and extends the work of Dylan A. Shell and Hazhar Rahmani in their paper ["Planning to chronicle: Optimal policies for narrative observation of unpredictable events"](https://journals.sagepub.com/doi/pdf/10.1177/02783649211069154).
 An excerpt from the paper is as follows:
 
 "An important class of applications entails a robot monitoring, scrutinizing, or recording the evolution of an uncertain
 time-extended process. This sort of situation leads to an interesting family
 of planning problems in which the robot is limited in what it sees and must, thus, choose what to pay attention to.
 The distinguishing characteristic of this setting is that the robot has influence over what it  captures via its sensors,
-but exercises no causal authority over the evolving process. As such, the robot’s objective is to observe the underlying
-process and to produce a ‘chronicle’ of current events, subject to a
+but exercises no causal authority over the evolving process. As such, the robot's objective is to observe the underlying
+process and to produce a 'chronicle' of current events, subject to a
 goal specification of the sorts of event sequences that may be of interest.
 This paper examines variants of such problems when the robot aims to
 collect sets of observations to meet a rich specification of their sequential structure. We study this class of problems by modeling a stochastic
 process via a variant of a hidden Markov model, and specify the event
-sequences of interest as a regular language, developing a vocabulary of
-‘mutators’ that enable sophisticated requirements to be expressed. Under different suppositions about the information gleaned about the event
+sequences of interest as a regular language, developing a vocabulary of 'mutators'
+that enable sophisticated requirements to be expressed. Under different suppositions about the information gleaned about the event
 model, we formulate and solve different planning problems. The core underlying idea is the construction of a product between the event model
 and a specification automaton.
 
 "A concrete motivation for this sort of setting, consider the
 proliferation of home videos. These videos are, with remarkably few exceptions,
 crummy specimens of the cinematic arts. They fail, generally, to establish and
 then bracket a scene; they often founder in emphasizing the importance of key
 subjects within the developing action, and are usually unsuccessful in attempts
 to trace an evolving narrative arc. And the current generation of autonomous
-personal robots and video drones, in their roles as costly and glorified ‘selfie
-sticks,’ are set to follow suit. The trouble is that capturing footage to tell a story
+personal robots and video drones, in their roles as costly and glorified 'selfie sticks'
+are set to follow suit. The trouble is that capturing footage to tell a story
 is challenging. A camera can only record what you point it toward, so part of
-the difficulty stems from the fact that you can’t know exactly how the scene will
-unfold before it actually does. Moreover, what constitutes structure isn’t easily
+the difficulty stems from the fact that you can't know exactly how the scene will
+unfold before it actually does. Moreover, what constitutes structure isn't easily
 summed up with a few trite quantities. Another part of the challenge, of course,
 is that one has only limited time to capture video footage.
 Setting aside pure vanity as a motivator, many applications can be cast as
 the problem of producing a finite-length sensor-based recording of the evolution
 of some process. As the video example emphasizes, one might be interested
 in recordings that meet rich specifications of the event sequences that are of
 interest. When the evolution of the event-generating process is uncertain/nondeterministic and sensing is local (necessitating its active direction), then one
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `ptcr-0.1.8/ptcr.egg-info/PKG-INFO` & `ptcr-0.1.9/ptcr.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ptcr
-Version: 0.1.8
+Version: 0.1.9
 Summary: Constructs and simulates PTCR models.
 Home-page: https://github.com/T-Lind/ptcr
 Author: Tiernan Lindauer
 Author-email: tiernanlind@tamu.edu
 License: MIT
 Keywords: PTCR,FOM,simulation,optimization,decision making,models
 Classifier: Programming Language :: Python :: 3
@@ -23,36 +23,36 @@
 This work implements and extends the work of Dylan A. Shell and Hazhar Rahmani in their paper ["Planning to chronicle: Optimal policies for narrative observation of unpredictable events"](https://journals.sagepub.com/doi/pdf/10.1177/02783649211069154).
 An excerpt from the paper is as follows:
 
 "An important class of applications entails a robot monitoring, scrutinizing, or recording the evolution of an uncertain
 time-extended process. This sort of situation leads to an interesting family
 of planning problems in which the robot is limited in what it sees and must, thus, choose what to pay attention to.
 The distinguishing characteristic of this setting is that the robot has influence over what it  captures via its sensors,
-but exercises no causal authority over the evolving process. As such, the robotâ€™s objective is to observe the underlying
-process and to produce a â€˜chronicleâ€™ of current events, subject to a
+but exercises no causal authority over the evolving process. As such, the robot's objective is to observe the underlying
+process and to produce a 'chronicle' of current events, subject to a
 goal specification of the sorts of event sequences that may be of interest.
 This paper examines variants of such problems when the robot aims to
 collect sets of observations to meet a rich specification of their sequential structure. We study this class of problems by modeling a stochastic
 process via a variant of a hidden Markov model, and specify the event
-sequences of interest as a regular language, developing a vocabulary of
-â€˜mutatorsâ€™ that enable sophisticated requirements to be expressed. Under different suppositions about the information gleaned about the event
+sequences of interest as a regular language, developing a vocabulary of 'mutators'
+that enable sophisticated requirements to be expressed. Under different suppositions about the information gleaned about the event
 model, we formulate and solve different planning problems. The core underlying idea is the construction of a product between the event model
 and a specification automaton.
 
 "A concrete motivation for this sort of setting, consider the
 proliferation of home videos. These videos are, with remarkably few exceptions,
 crummy specimens of the cinematic arts. They fail, generally, to establish and
 then bracket a scene; they often founder in emphasizing the importance of key
 subjects within the developing action, and are usually unsuccessful in attempts
 to trace an evolving narrative arc. And the current generation of autonomous
-personal robots and video drones, in their roles as costly and glorified â€˜selfie
-sticks,â€™ are set to follow suit. The trouble is that capturing footage to tell a story
+personal robots and video drones, in their roles as costly and glorified 'selfie sticks'
+are set to follow suit. The trouble is that capturing footage to tell a story
 is challenging. A camera can only record what you point it toward, so part of
-the difficulty stems from the fact that you canâ€™t know exactly how the scene will
-unfold before it actually does. Moreover, what constitutes structure isnâ€™t easily
+the difficulty stems from the fact that you can't know exactly how the scene will
+unfold before it actually does. Moreover, what constitutes structure isn't easily
 summed up with a few trite quantities. Another part of the challenge, of course,
 is that one has only limited time to capture video footage.
 Setting aside pure vanity as a motivator, many applications can be cast as
 the problem of producing a finite-length sensor-based recording of the evolution
 of some process. As the video example emphasizes, one might be interested
 in recordings that meet rich specifications of the event sequences that are of
 interest. When the evolution of the event-generating process is uncertain/nondeterministic and sensing is local (necessitating its active direction), then one
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `ptcr-0.1.8/ptcr2/automata_utility.py` & `ptcr-0.1.9/ptcr2/automata_utility.py`

 * *Files identical despite different names*

### Comparing `ptcr-0.1.8/ptcr2/base_model.py` & `ptcr-0.1.9/ptcr2/base_model.py`

 * *Files identical despite different names*

### Comparing `ptcr-0.1.8/ptcr2/belief_tree.py` & `ptcr-0.1.9/ptcr2/belief_tree.py`

 * *Files identical despite different names*

### Comparing `ptcr-0.1.8/ptcr2/event_predictor.py` & `ptcr-0.1.9/ptcr2/event_predictor.py`

 * *Files identical despite different names*

### Comparing `ptcr-0.1.8/ptcr2/fom.py` & `ptcr-0.1.9/ptcr2/fom.py`

 * *Files identical despite different names*

### Comparing `ptcr-0.1.8/ptcr2/markov_chain.py` & `ptcr-0.1.9/ptcr2/markov_chain.py`

 * *Files identical despite different names*

### Comparing `ptcr-0.1.8/ptcr2/markov_decision_process.py` & `ptcr-0.1.9/ptcr2/markov_decision_process.py`

 * *Files identical despite different names*

### Comparing `ptcr-0.1.8/setup.py` & `ptcr-0.1.9/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='ptcr',
-    version='0.1.8',
+    version='0.1.9',
     author='Tiernan Lindauer',
     author_email='tiernanlind@tamu.edu',
     description='Constructs and simulates PTCR models.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     packages=find_packages(),
     classifiers=[
```

