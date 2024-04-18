# Comparing `tmp/ptcr-0.1.7.tar.gz` & `tmp/ptcr-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ptcr-0.1.7.tar", last modified: Wed Apr 17 02:55:56 2024, max compression
+gzip compressed data, was "ptcr-0.1.8.tar", last modified: Thu Apr 18 19:48:32 2024, max compression
```

## Comparing `ptcr-0.1.7.tar` & `ptcr-0.1.8.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2024-04-17 02:55:56.323605 ptcr-0.1.7/
--rw-rw-rw-   0        0        0     1069 2024-04-16 23:53:12.000000 ptcr-0.1.7/LICENSE
--rw-rw-rw-   0        0        0    11205 2024-04-17 02:55:56.322605 ptcr-0.1.7/PKG-INFO
--rw-rw-rw-   0        0        0    10639 2024-04-17 02:44:06.000000 ptcr-0.1.7/README.md
-drwxrwxrwx   0        0        0        0 2024-04-17 02:55:56.311313 ptcr-0.1.7/ptcr.egg-info/
--rw-rw-rw-   0        0        0    11205 2024-04-17 02:55:56.000000 ptcr-0.1.7/ptcr.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      343 2024-04-17 02:55:56.000000 ptcr-0.1.7/ptcr.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-17 02:55:56.000000 ptcr-0.1.7/ptcr.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      180 2024-04-17 02:55:56.000000 ptcr-0.1.7/ptcr.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-04-17 02:55:56.000000 ptcr-0.1.7/ptcr.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-17 02:55:56.320606 ptcr-0.1.7/ptcr2/
--rw-rw-rw-   0        0        0        0 2024-02-23 22:22:15.000000 ptcr-0.1.7/ptcr2/__init__.py
--rw-rw-rw-   0        0        0     7664 2024-03-06 16:01:26.000000 ptcr-0.1.7/ptcr2/automata_utility.py
--rw-rw-rw-   0        0        0     3681 2024-04-16 13:50:12.000000 ptcr-0.1.7/ptcr2/base_model.py
--rw-rw-rw-   0        0        0     3364 2024-04-07 16:47:54.000000 ptcr-0.1.7/ptcr2/belief_tree.py
--rw-rw-rw-   0        0        0    27773 2024-04-16 23:22:39.000000 ptcr-0.1.7/ptcr2/event_predictor.py
--rw-rw-rw-   0        0        0    10168 2024-04-07 21:33:36.000000 ptcr-0.1.7/ptcr2/fom.py
--rw-rw-rw-   0        0        0     9897 2024-04-07 16:36:30.000000 ptcr-0.1.7/ptcr2/markov_chain.py
--rw-rw-rw-   0        0        0    75894 2024-04-07 21:39:01.000000 ptcr-0.1.7/ptcr2/markov_decision_process.py
--rw-rw-rw-   0        0        0       42 2024-04-17 02:55:56.323605 ptcr-0.1.7/setup.cfg
--rw-rw-rw-   0        0        0     1047 2024-04-17 02:55:52.000000 ptcr-0.1.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-18 19:48:32.378819 ptcr-0.1.8/
+-rw-rw-rw-   0        0        0     1069 2024-04-16 23:53:12.000000 ptcr-0.1.8/LICENSE
+-rw-rw-rw-   0        0        0    12865 2024-04-18 19:48:32.377812 ptcr-0.1.8/PKG-INFO
+-rw-rw-rw-   0        0        0    12299 2024-04-18 19:47:24.000000 ptcr-0.1.8/README.md
+drwxrwxrwx   0        0        0        0 2024-04-18 19:48:32.283226 ptcr-0.1.8/ptcr.egg-info/
+-rw-rw-rw-   0        0        0    12865 2024-04-18 19:48:32.000000 ptcr-0.1.8/ptcr.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      343 2024-04-18 19:48:32.000000 ptcr-0.1.8/ptcr.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-18 19:48:32.000000 ptcr-0.1.8/ptcr.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      180 2024-04-18 19:48:32.000000 ptcr-0.1.8/ptcr.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-04-18 19:48:32.000000 ptcr-0.1.8/ptcr.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-18 19:48:32.375836 ptcr-0.1.8/ptcr2/
+-rw-rw-rw-   0        0        0        0 2024-02-23 22:22:15.000000 ptcr-0.1.8/ptcr2/__init__.py
+-rw-rw-rw-   0        0        0     7664 2024-03-06 16:01:26.000000 ptcr-0.1.8/ptcr2/automata_utility.py
+-rw-rw-rw-   0        0        0     3681 2024-04-16 13:50:12.000000 ptcr-0.1.8/ptcr2/base_model.py
+-rw-rw-rw-   0        0        0     3364 2024-04-07 16:47:54.000000 ptcr-0.1.8/ptcr2/belief_tree.py
+-rw-rw-rw-   0        0        0    27773 2024-04-16 23:22:39.000000 ptcr-0.1.8/ptcr2/event_predictor.py
+-rw-rw-rw-   0        0        0    10168 2024-04-07 21:33:36.000000 ptcr-0.1.8/ptcr2/fom.py
+-rw-rw-rw-   0        0        0     9897 2024-04-07 16:36:30.000000 ptcr-0.1.8/ptcr2/markov_chain.py
+-rw-rw-rw-   0        0        0    75894 2024-04-07 21:39:01.000000 ptcr-0.1.8/ptcr2/markov_decision_process.py
+-rw-rw-rw-   0        0        0       42 2024-04-18 19:48:32.378819 ptcr-0.1.8/setup.cfg
+-rw-rw-rw-   0        0        0     1047 2024-04-18 19:40:14.000000 ptcr-0.1.8/setup.py
```

### Comparing `ptcr-0.1.7/LICENSE` & `ptcr-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `ptcr-0.1.7/PKG-INFO` & `ptcr-0.1.8/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ptcr
-Version: 0.1.7
+Version: 0.1.8
 Summary: Constructs and simulates PTCR models.
 Home-page: https://github.com/T-Lind/ptcr
 Author: Tiernan Lindauer
 Author-email: tiernanlind@tamu.edu
 License: MIT
 Keywords: PTCR,FOM,simulation,optimization,decision making,models
 Classifier: Programming Language :: Python :: 3
@@ -16,17 +16,23 @@
 
 # Exploring Alternative Cost Mechanisms for Probabilistic Planning
 
 ### Author: T-Lind
 
 
 ## Overview
+This work implements and extends the work of Dylan A. Shell and Hazhar Rahmani in their paper ["Planning to chronicle: Optimal policies for narrative observation of unpredictable events"](https://journals.sagepub.com/doi/pdf/10.1177/02783649211069154).
+An excerpt from the paper is as follows:
+
 "An important class of applications entails a robot monitoring, scrutinizing, or recording the evolution of an uncertain
 time-extended process. This sort of situation leads to an interesting family
-of planning problems in which the robot is limited in what it sees and must, thus, choose what to pay attention to. The distinguishing characteristic of this setting is that the robot has influence over what it  captures via its sensors, but exercises no causal authority over the evolving process. As such, the robotâ€™s objective is to observe the underlying process and to produce a â€˜chronicleâ€™ of occurrent events, subject to a
+of planning problems in which the robot is limited in what it sees and must, thus, choose what to pay attention to.
+The distinguishing characteristic of this setting is that the robot has influence over what it  captures via its sensors,
+but exercises no causal authority over the evolving process. As such, the robotâ€™s objective is to observe the underlying
+process and to produce a â€˜chronicleâ€™ of current events, subject to a
 goal specification of the sorts of event sequences that may be of interest.
 This paper examines variants of such problems when the robot aims to
 collect sets of observations to meet a rich specification of their sequential structure. We study this class of problems by modeling a stochastic
 process via a variant of a hidden Markov model, and specify the event
 sequences of interest as a regular language, developing a vocabulary of
 â€˜mutatorsâ€™ that enable sophisticated requirements to be expressed. Under different suppositions about the information gleaned about the event
 model, we formulate and solve different planning problems. The core underlying idea is the construction of a product between the event model
@@ -70,15 +76,31 @@
 transform DFAs, enabling easy expression of sophisticated requirements, we distinguish when mutators preserve representational independence too."
 
 Additionally, a cost-based optimization approach has been implemented, such that the optimal policy becomes the one that
 reduces the most amount of cost, while still satisfying the constraints of the problem. This could mean minimizing the
 distance a robot travels, reducing its wear and improving its efficiency, minimizing the amount of time it takes to
 complete a certain task.
 
+This "cost" is implemented in a matrix, so that the transition from state to state in the model incurs a certain cost.
+This is then paired with an optimization algorithm that factors in the state-state optimization, such that the robot
+can minimize the cost it incurs while still satisfying the constraints of the problem. This could be described as a 
+"navigation" cost.
+
+
+
 ## Example Usage
+In the example usage below, the state names must be specified as strings inside of a list, like seen below.
+The transition matrix then must be square of the size of the state names; the row is "from" and the column is "to".
+This represents probabilities in the model, so each row should sum up to 1.0. The cost matrix is also square, and
+represents the cost of transitioning from one state to another as described above. Note that the costs could be from any
+range, but should be consistent across the matrix. The initial distribution is the probability of starting in each state,
+and should sum up to 1.0. The state events are the events that can occur in each state, and should be specified as a list
+of lists of strings. The single initial states are the states that the robot can start in, and should be specified as a
+list of lists of lists, where the innermost list is the state and the outermost list is the initial state. The alphabet is
+the list of all possible events that can occur in the model.
 ```json
 {
   "state_names": ["I", "E", "B", "C", "D", "S"],
   "transition_matrix": [
     [0.0, 0.1, 0.3, 0.1, 0.2, 0.3],
     [0.0, 0.1, 0.2, 0.1, 0.3, 0.3],
     [0.0, 0.2, 0.1, 0.1, 0.3, 0.3],
@@ -103,18 +125,14 @@
     ],
   "single_initial_states": [
     [[["d1", "d2"], "d12"]],
     [[["d2", "d3"], "d23"]]
   ],
 
   "alphabet": ["e1", "b1", "c1", "d1", "s1", "e2", "b2", "c2", "d2", "s2", "d12", "e3", "b3", "c3", "d3", "s3", "d23"],
-
-  "plot": true,
-  "log": true
-}
 ```
 
 Demonstrate capabilities:
 ```python
 import json
 from timeit import default_timer as timer
```

### Comparing `ptcr-0.1.7/README.md` & `ptcr-0.1.8/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,16 +1,22 @@
 # Exploring Alternative Cost Mechanisms for Probabilistic Planning
 
 ### Author: T-Lind
 
 
 ## Overview
+This work implements and extends the work of Dylan A. Shell and Hazhar Rahmani in their paper ["Planning to chronicle: Optimal policies for narrative observation of unpredictable events"](https://journals.sagepub.com/doi/pdf/10.1177/02783649211069154).
+An excerpt from the paper is as follows:
+
 "An important class of applications entails a robot monitoring, scrutinizing, or recording the evolution of an uncertain
 time-extended process. This sort of situation leads to an interesting family
-of planning problems in which the robot is limited in what it sees and must, thus, choose what to pay attention to. The distinguishing characteristic of this setting is that the robot has influence over what it  captures via its sensors, but exercises no causal authority over the evolving process. As such, the robot’s objective is to observe the underlying process and to produce a ‘chronicle’ of occurrent events, subject to a
+of planning problems in which the robot is limited in what it sees and must, thus, choose what to pay attention to.
+The distinguishing characteristic of this setting is that the robot has influence over what it  captures via its sensors,
+but exercises no causal authority over the evolving process. As such, the robot’s objective is to observe the underlying
+process and to produce a ‘chronicle’ of current events, subject to a
 goal specification of the sorts of event sequences that may be of interest.
 This paper examines variants of such problems when the robot aims to
 collect sets of observations to meet a rich specification of their sequential structure. We study this class of problems by modeling a stochastic
 process via a variant of a hidden Markov model, and specify the event
 sequences of interest as a regular language, developing a vocabulary of
 ‘mutators’ that enable sophisticated requirements to be expressed. Under different suppositions about the information gleaned about the event
 model, we formulate and solve different planning problems. The core underlying idea is the construction of a product between the event model
@@ -54,15 +60,31 @@
 transform DFAs, enabling easy expression of sophisticated requirements, we distinguish when mutators preserve representational independence too."
 
 Additionally, a cost-based optimization approach has been implemented, such that the optimal policy becomes the one that
 reduces the most amount of cost, while still satisfying the constraints of the problem. This could mean minimizing the
 distance a robot travels, reducing its wear and improving its efficiency, minimizing the amount of time it takes to
 complete a certain task.
 
+This "cost" is implemented in a matrix, so that the transition from state to state in the model incurs a certain cost.
+This is then paired with an optimization algorithm that factors in the state-state optimization, such that the robot
+can minimize the cost it incurs while still satisfying the constraints of the problem. This could be described as a 
+"navigation" cost.
+
+
+
 ## Example Usage
+In the example usage below, the state names must be specified as strings inside of a list, like seen below.
+The transition matrix then must be square of the size of the state names; the row is "from" and the column is "to".
+This represents probabilities in the model, so each row should sum up to 1.0. The cost matrix is also square, and
+represents the cost of transitioning from one state to another as described above. Note that the costs could be from any
+range, but should be consistent across the matrix. The initial distribution is the probability of starting in each state,
+and should sum up to 1.0. The state events are the events that can occur in each state, and should be specified as a list
+of lists of strings. The single initial states are the states that the robot can start in, and should be specified as a
+list of lists of lists, where the innermost list is the state and the outermost list is the initial state. The alphabet is
+the list of all possible events that can occur in the model.
 ```json
 {
   "state_names": ["I", "E", "B", "C", "D", "S"],
   "transition_matrix": [
     [0.0, 0.1, 0.3, 0.1, 0.2, 0.3],
     [0.0, 0.1, 0.2, 0.1, 0.3, 0.3],
     [0.0, 0.2, 0.1, 0.1, 0.3, 0.3],
@@ -87,18 +109,14 @@
     ],
   "single_initial_states": [
     [[["d1", "d2"], "d12"]],
     [[["d2", "d3"], "d23"]]
   ],
 
   "alphabet": ["e1", "b1", "c1", "d1", "s1", "e2", "b2", "c2", "d2", "s2", "d12", "e3", "b3", "c3", "d3", "s3", "d23"],
-
-  "plot": true,
-  "log": true
-}
 ```
 
 Demonstrate capabilities:
 ```python
 import json
 from timeit import default_timer as timer
```

### Comparing `ptcr-0.1.7/ptcr.egg-info/PKG-INFO` & `ptcr-0.1.8/ptcr.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ptcr
-Version: 0.1.7
+Version: 0.1.8
 Summary: Constructs and simulates PTCR models.
 Home-page: https://github.com/T-Lind/ptcr
 Author: Tiernan Lindauer
 Author-email: tiernanlind@tamu.edu
 License: MIT
 Keywords: PTCR,FOM,simulation,optimization,decision making,models
 Classifier: Programming Language :: Python :: 3
@@ -16,17 +16,23 @@
 
 # Exploring Alternative Cost Mechanisms for Probabilistic Planning
 
 ### Author: T-Lind
 
 
 ## Overview
+This work implements and extends the work of Dylan A. Shell and Hazhar Rahmani in their paper ["Planning to chronicle: Optimal policies for narrative observation of unpredictable events"](https://journals.sagepub.com/doi/pdf/10.1177/02783649211069154).
+An excerpt from the paper is as follows:
+
 "An important class of applications entails a robot monitoring, scrutinizing, or recording the evolution of an uncertain
 time-extended process. This sort of situation leads to an interesting family
-of planning problems in which the robot is limited in what it sees and must, thus, choose what to pay attention to. The distinguishing characteristic of this setting is that the robot has influence over what it  captures via its sensors, but exercises no causal authority over the evolving process. As such, the robotâ€™s objective is to observe the underlying process and to produce a â€˜chronicleâ€™ of occurrent events, subject to a
+of planning problems in which the robot is limited in what it sees and must, thus, choose what to pay attention to.
+The distinguishing characteristic of this setting is that the robot has influence over what it  captures via its sensors,
+but exercises no causal authority over the evolving process. As such, the robotâ€™s objective is to observe the underlying
+process and to produce a â€˜chronicleâ€™ of current events, subject to a
 goal specification of the sorts of event sequences that may be of interest.
 This paper examines variants of such problems when the robot aims to
 collect sets of observations to meet a rich specification of their sequential structure. We study this class of problems by modeling a stochastic
 process via a variant of a hidden Markov model, and specify the event
 sequences of interest as a regular language, developing a vocabulary of
 â€˜mutatorsâ€™ that enable sophisticated requirements to be expressed. Under different suppositions about the information gleaned about the event
 model, we formulate and solve different planning problems. The core underlying idea is the construction of a product between the event model
@@ -70,15 +76,31 @@
 transform DFAs, enabling easy expression of sophisticated requirements, we distinguish when mutators preserve representational independence too."
 
 Additionally, a cost-based optimization approach has been implemented, such that the optimal policy becomes the one that
 reduces the most amount of cost, while still satisfying the constraints of the problem. This could mean minimizing the
 distance a robot travels, reducing its wear and improving its efficiency, minimizing the amount of time it takes to
 complete a certain task.
 
+This "cost" is implemented in a matrix, so that the transition from state to state in the model incurs a certain cost.
+This is then paired with an optimization algorithm that factors in the state-state optimization, such that the robot
+can minimize the cost it incurs while still satisfying the constraints of the problem. This could be described as a 
+"navigation" cost.
+
+
+
 ## Example Usage
+In the example usage below, the state names must be specified as strings inside of a list, like seen below.
+The transition matrix then must be square of the size of the state names; the row is "from" and the column is "to".
+This represents probabilities in the model, so each row should sum up to 1.0. The cost matrix is also square, and
+represents the cost of transitioning from one state to another as described above. Note that the costs could be from any
+range, but should be consistent across the matrix. The initial distribution is the probability of starting in each state,
+and should sum up to 1.0. The state events are the events that can occur in each state, and should be specified as a list
+of lists of strings. The single initial states are the states that the robot can start in, and should be specified as a
+list of lists of lists, where the innermost list is the state and the outermost list is the initial state. The alphabet is
+the list of all possible events that can occur in the model.
 ```json
 {
   "state_names": ["I", "E", "B", "C", "D", "S"],
   "transition_matrix": [
     [0.0, 0.1, 0.3, 0.1, 0.2, 0.3],
     [0.0, 0.1, 0.2, 0.1, 0.3, 0.3],
     [0.0, 0.2, 0.1, 0.1, 0.3, 0.3],
@@ -103,18 +125,14 @@
     ],
   "single_initial_states": [
     [[["d1", "d2"], "d12"]],
     [[["d2", "d3"], "d23"]]
   ],
 
   "alphabet": ["e1", "b1", "c1", "d1", "s1", "e2", "b2", "c2", "d2", "s2", "d12", "e3", "b3", "c3", "d3", "s3", "d23"],
-
-  "plot": true,
-  "log": true
-}
 ```
 
 Demonstrate capabilities:
 ```python
 import json
 from timeit import default_timer as timer
```

### Comparing `ptcr-0.1.7/ptcr2/automata_utility.py` & `ptcr-0.1.8/ptcr2/automata_utility.py`

 * *Files identical despite different names*

### Comparing `ptcr-0.1.7/ptcr2/base_model.py` & `ptcr-0.1.8/ptcr2/base_model.py`

 * *Files identical despite different names*

### Comparing `ptcr-0.1.7/ptcr2/belief_tree.py` & `ptcr-0.1.8/ptcr2/belief_tree.py`

 * *Files identical despite different names*

### Comparing `ptcr-0.1.7/ptcr2/event_predictor.py` & `ptcr-0.1.8/ptcr2/event_predictor.py`

 * *Files identical despite different names*

### Comparing `ptcr-0.1.7/ptcr2/fom.py` & `ptcr-0.1.8/ptcr2/fom.py`

 * *Files identical despite different names*

### Comparing `ptcr-0.1.7/ptcr2/markov_chain.py` & `ptcr-0.1.8/ptcr2/markov_chain.py`

 * *Files identical despite different names*

### Comparing `ptcr-0.1.7/ptcr2/markov_decision_process.py` & `ptcr-0.1.8/ptcr2/markov_decision_process.py`

 * *Files identical despite different names*

### Comparing `ptcr-0.1.7/setup.py` & `ptcr-0.1.8/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='ptcr',
-    version='0.1.7',
+    version='0.1.8',
     author='Tiernan Lindauer',
     author_email='tiernanlind@tamu.edu',
     description='Constructs and simulates PTCR models.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     packages=find_packages(),
     classifiers=[
```

