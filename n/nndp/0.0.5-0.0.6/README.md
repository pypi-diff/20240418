# Comparing `tmp/nndp-0.0.5.tar.gz` & `tmp/nndp-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nndp-0.0.5.tar", last modified: Thu Mar  2 13:51:38 2023, max compression
+gzip compressed data, was "nndp-0.0.6.tar", last modified: Thu Apr 18 16:46:10 2024, max compression
```

## Comparing `nndp-0.0.5.tar` & `nndp-0.0.6.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-03-02 13:51:37.453376 nndp-0.0.5/
--rw-rw-rw-   0        0        0       59 2023-02-26 23:27:51.000000 nndp-0.0.5/.gitignore
--rw-rw-rw-   0        0        0     1098 2023-02-26 23:27:51.000000 nndp-0.0.5/LICENSE
--rw-rw-rw-   0        0        0     2888 2023-03-02 13:51:38.248381 nndp-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     2519 2023-02-26 23:46:27.000000 nndp-0.0.5/README.md
-drwxrwxrwx   0        0        0        0 2023-03-02 13:51:37.305375 nndp-0.0.5/examples/
-drwxrwxrwx   0        0        0        0 2023-03-02 13:51:37.673376 nndp-0.0.5/examples/income_fluctuations/
--rw-rw-rw-   0        0        0    38881 2023-03-02 13:50:21.000000 nndp-0.0.5/examples/income_fluctuations/main.ipynb
--rw-rw-rw-   0        0        0     2586 2023-02-26 23:27:51.000000 nndp-0.0.5/examples/income_fluctuations/model.py
--rw-rw-rw-   0        0        0    50248 2023-02-26 23:27:51.000000 nndp-0.0.5/examples/income_fluctuations/simulation_results.csv
--rw-rw-rw-   0        0        0       42 2023-03-02 13:51:38.267379 nndp-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0      785 2023-03-02 13:51:30.000000 nndp-0.0.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-02 13:51:37.350375 nndp-0.0.5/src/
-drwxrwxrwx   0        0        0        0 2023-03-02 13:51:37.874377 nndp-0.0.5/src/nndp/
--rw-rw-rw-   0        0        0       23 2023-02-26 23:57:13.000000 nndp-0.0.5/src/nndp/__init__.py
--rw-rw-rw-   0        0        0     7486 2023-02-27 00:30:28.000000 nndp-0.0.5/src/nndp/core.py
--rw-rw-rw-   0        0        0     5123 2023-03-02 13:50:21.000000 nndp-0.0.5/src/nndp/policy_function.py
-drwxrwxrwx   0        0        0        0 2023-03-02 13:51:37.350375 nndp-0.0.5/src/nndp.egg-info/
--rw-rw-rw-   0        0        0     2888 2023-03-02 13:51:35.000000 nndp-0.0.5/src/nndp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      392 2023-03-02 13:51:36.000000 nndp-0.0.5/src/nndp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-02 13:51:35.000000 nndp-0.0.5/src/nndp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       91 2023-03-02 13:51:35.000000 nndp-0.0.5/src/nndp.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-03-02 13:51:35.000000 nndp-0.0.5/src/nndp.egg-info/top_level.txt
+drwxr-xr-x   0 mbarrera (10656) users      (100)        0 2024-04-18 16:46:10.602706 nndp-0.0.6/
+-rwxr-xr-x   0 mbarrera (10656) users      (100)     1098 2023-02-26 23:27:51.000000 nndp-0.0.6/LICENSE
+-rw-r--r--   0 mbarrera (10656) users      (100)     4408 2024-04-18 16:46:10.600709 nndp-0.0.6/PKG-INFO
+-rw-r--r--   0 mbarrera (10656) users      (100)     2702 2024-04-17 12:06:41.000000 nndp-0.0.6/README.md
+-rw-r--r--   0 mbarrera (10656) users      (100)      607 2024-04-18 16:45:27.000000 nndp-0.0.6/pyproject.toml
+-rw-r--r--   0 mbarrera (10656) users      (100)       38 2024-04-18 16:46:10.602713 nndp-0.0.6/setup.cfg
+drwxr-xr-x   0 mbarrera (10656) users      (100)        0 2024-04-18 16:46:10.552712 nndp-0.0.6/src/
+drwxr-xr-x   0 mbarrera (10656) users      (100)        0 2024-04-18 16:46:10.566706 nndp-0.0.6/src/nndp/
+-rwxr-xr-x   0 mbarrera (10656) users      (100)       23 2023-02-26 23:57:13.000000 nndp-0.0.6/src/nndp/__init__.py
+drwxr-xr-x   0 mbarrera (10656) users      (100)        0 2024-04-18 16:46:10.593708 nndp-0.0.6/src/nndp/agnostic/
+-rw-r--r--   0 mbarrera (10656) users      (100)      126 2024-04-13 14:51:09.000000 nndp-0.0.6/src/nndp/agnostic/__init__.py
+-rwxr-xr-x   0 mbarrera (10656) users      (100)      370 2024-04-13 13:34:40.000000 nndp-0.0.6/src/nndp/agnostic/analysis.py
+-rwxr-xr-x   0 mbarrera (10656) users      (100)      266 2024-04-12 18:32:39.000000 nndp-0.0.6/src/nndp/agnostic/model.py
+-rwxr-xr-x   0 mbarrera (10656) users      (100)      949 2024-04-12 18:32:37.000000 nndp-0.0.6/src/nndp/agnostic/policy.py
+-rwxr-xr-x   0 mbarrera (10656) users      (100)     1821 2024-04-13 13:34:41.000000 nndp-0.0.6/src/nndp/agnostic/samplers.py
+-rwxr-xr-x   0 mbarrera (10656) users      (100)     6346 2024-04-13 13:34:39.000000 nndp-0.0.6/src/nndp/agnostic/train.py
+-rwxr-xr-x   0 mbarrera (10656) users      (100)     7486 2024-04-17 11:23:33.000000 nndp-0.0.6/src/nndp/core.py
+-rwxr-xr-x   0 mbarrera (10656) users      (100)     5123 2023-04-28 21:16:17.000000 nndp-0.0.6/src/nndp/policy_function.py
+drwxr-xr-x   0 mbarrera (10656) users      (100)        0 2024-04-18 16:46:10.596712 nndp-0.0.6/src/nndp.egg-info/
+-rw-r--r--   0 mbarrera (10656) users      (100)     4408 2024-04-18 16:46:10.000000 nndp-0.0.6/src/nndp.egg-info/PKG-INFO
+-rw-r--r--   0 mbarrera (10656) users      (100)      429 2024-04-18 16:46:10.000000 nndp-0.0.6/src/nndp.egg-info/SOURCES.txt
+-rw-r--r--   0 mbarrera (10656) users      (100)        1 2024-04-18 16:46:10.000000 nndp-0.0.6/src/nndp.egg-info/dependency_links.txt
+-rw-r--r--   0 mbarrera (10656) users      (100)      108 2024-04-18 16:46:10.000000 nndp-0.0.6/src/nndp.egg-info/requires.txt
+-rw-r--r--   0 mbarrera (10656) users      (100)        5 2024-04-18 16:46:10.000000 nndp-0.0.6/src/nndp.egg-info/top_level.txt
```

### Comparing `nndp-0.0.5/LICENSE` & `nndp-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `nndp-0.0.5/PKG-INFO` & `nndp-0.0.6/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,45 +1,39 @@
-Metadata-Version: 2.1
-Name: nndp
-Version: 0.0.5
-Summary: Dynamic Programming with Neural Networks
-Home-page: https://github.com/marcdelabarrera/nndp
-Author: Marc de la Barrera i Bardalet
-Author-email: mbarrera@mit.edu
-Classifier: Programming Language :: Python :: 3.10
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-License-File: LICENSE
-
-# Dynamic Programming with Neural Networks `(nndp)`
-
-Marc de la Barrera i Bardalet, Tim de Silva
-
-`nndp` provides a framework for solving finite horizon dynamic programming problems using neural networks that is implemented using the [JAX](https://github.com/google/jax) functional programming paradigm and [Haiku](https://github.com/deepmind/dm-haiku). This solution technique, introduced and described in detail by [Duarte, Fonesca, Goodman, and Parker (2021)](https://0f2486b1-f568-477b-8307-dd98a6c77afd.filesusr.com/ugd/f9db9d_972da014adb2453b8a4dab0239909062.pdf), applies to problems of the following form: 
-
-$$V(s_0)=\max_{a_t\in\Gamma(s_t)} E_0\left[\sum_{t=0}^T u(s_t,a_t)\right],$$
-
-$$s_{t+1}=m(s_{t},a_{t},\epsilon_t), $$
-
-$$s_0 \sim F(\cdot).$$
-
-The state vector is denoted by $s_t=(k_t, x_t)$, where $k_t$ are exogenous states and $x_t$ are endogenous states. We adopt the convention that the first exogenous state in $k_t$ is $t$. The goal is to find a policy function $\pi(s_t)$ that satisfies:
-
-$$\hat V(s_0,\pi)=E_0\left[\sum_{t=0}^T u(s_t,\pi(s_t))\right],$$
-
-$$s_{t+1}=m(s_{t},\pi(s_{t}),\epsilon_t),$$
-
-$$V(s_0)=\hat V(s_0,\pi)\quad \forall s_0.$$
-
-We parametrize $\pi(s_t)=\tilde\pi(s_t,\theta)$ as a fully connected feedforward neural network and update the networksâ€™ parameters, $\theta$, using stochastic gradient descent. To use this framework, the user only needs to write the following functions that are defined by the dynamic programming problem of interest:
-
-1. `u(state, action)`: reward function for $s_t$ = `state` and $a_t$ = `action`
-2. `m(key, state, action)`: state evolution equation for $s_{t+1}$ if $s_t$ = `state` and $a_t$ = `action`. `key` is a JAX RNG key used to simulate any shocks present in the model.
-3. `Gamma(state)`: defines the set of possible actions, $a_t$, at $s_t$ = `state`
-4. `F(key, N)`: samples `N` observations from the distribution of $s_0$. `key` is a JAX RNG key used to simulate any shocks present in the model.
-5. `nn_to_action(state, params, nn)`: defines how the output of a Haiku Neural Network, `nn`, with parameters, `params`, is mapped into an action at $s_t$ = `state`
-
-We provide an example application to the income fluctations problem in `examples/income_fluctuations/main.ipynb` to illustrate how this framework can be used.
-
-# References
-Duarte, Victor, Julia Fonseca, Jonathan A. Parker, and Aaron Goodman (2021), Simple Allocation Rules and Optimal Portfolio Choice Over the Lifecycle, Working Paper.
-
+# Dynamic Programming with Neural Networks `(nndp)`
+
+By: Marc de la Barrera i Bardalet, Tim de Silva
+
+## Overview
+
+`nndp` provides a framework for solving finite horizon dynamic programming problems using neural networks that is implemented using the [JAX](https://github.com/google/jax) functional programming paradigm and [Haiku](https://github.com/deepmind/dm-haiku). This solution technique, introduced and described in detail by [Duarte, Fonesca, Goodman, and Parker (2021)](https://0f2486b1-f568-477b-8307-dd98a6c77afd.filesusr.com/ugd/f9db9d_972da014adb2453b8a4dab0239909062.pdf), applies to problems of the following form: 
+
+$$V(s_0)=\max_{a_t\in\Gamma(s_t)} E_0\left[\sum_{t=0}^T u(s_t,a_t)\right],$$
+
+$$s_{t+1}=m(s_{t},a_{t},\epsilon_t), $$
+
+$$s_0 \sim F(\cdot).$$
+
+The state vector is denoted by $s_t=(k_t, x_t)$, where $k_t$ are exogenous states and $x_t$ are endogenous states. We adopt the convention that the first exogenous state in $k_t$ is $t$. The goal is to find a policy function $\pi(s_t)$ that satisfies:
+
+$$\hat V(s_0,\pi)=E_0\left[\sum_{t=0}^T u(s_t,\pi(s_t))\right],$$
+
+$$s_{t+1}=m(s_{t},\pi(s_{t}),\epsilon_t),$$
+
+$$V(s_0)=\hat V(s_0,\pi)\quad \forall s_0.$$
+
+We parametrize $\pi(s_t)=\tilde\pi(s_t,\theta)$ as a fully connected feedforward neural network and update the networks’ parameters, $\theta$, using stochastic gradient descent. To use this framework, the user only needs to write the following functions that are defined by the dynamic programming problem of interest:
+
+1. `u(state, action)`: reward function for $s_t$ = `state` and $a_t$ = `action`
+2. `m(key, state, action)`: state evolution equation for $s_{t+1}$ if $s_t$ = `state` and $a_t$ = `action`. `key` is a JAX RNG key used to simulate any shocks present in the model.
+3. `Gamma(state)`: defines the set of possible actions, $a_t$, at $s_t$ = `state`
+4. `F(key, N)`: samples `N` observations from the distribution of $s_0$. `key` is a JAX RNG key used to simulate any shocks present in the model.
+5. `nn_to_action(state, params, nn)`: defines how the output of a Haiku Neural Network, `nn`, with parameters, `params`, is mapped into an action at $s_t$ = `state`
+
+We provide an example application to the income fluctations problem in `docs/source/notebooks/income_fluctuations/main.ipynb` to illustrate how this framework can be used.
+
+## Installation
+
+`nndp` requires [JAX](https://github.com/google/jax) and [Haiku](https://github.com/deepmind/dm-haiku) to be installed. To install with `pip`, run `pip install nndp`.
+
+## References
+Duarte, Victor, Julia Fonseca, Jonathan A. Parker, and Aaron Goodman (2021), Simple Allocation Rules and Optimal Portfolio Choice Over the Lifecycle, Working Paper.
+
```

### Comparing `nndp-0.0.5/src/nndp/core.py` & `nndp-0.0.6/src/nndp/core.py`

 * *Files identical despite different names*

### Comparing `nndp-0.0.5/src/nndp/policy_function.py` & `nndp-0.0.6/src/nndp/policy_function.py`

 * *Files identical despite different names*

