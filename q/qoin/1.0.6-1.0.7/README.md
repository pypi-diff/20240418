# Comparing `tmp/qoin-1.0.6.tar.gz` & `tmp/qoin-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qoin-1.0.6.tar", last modified: Fri Mar 29 15:47:32 2024, max compression
+gzip compressed data, was "qoin-1.0.7.tar", last modified: Thu Apr 18 11:10:35 2024, max compression
```

## Comparing `qoin-1.0.6.tar` & `qoin-1.0.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-03-29 15:47:32.390392 qoin-1.0.6/
--rw-rw-rw-   0        0        0    35823 2024-03-27 19:02:44.000000 qoin-1.0.6/LICENSE
--rw-rw-rw-   0        0        0    42866 2024-03-29 15:47:32.388119 qoin-1.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     1052 2024-03-28 14:48:01.000000 qoin-1.0.6/README.md
--rw-rw-rw-   0        0        0      838 2024-03-29 15:47:03.000000 qoin-1.0.6/pyproject.toml
-drwxrwxrwx   0        0        0        0 2024-03-29 15:47:32.292460 qoin-1.0.6/qoin/
--rw-rw-rw-   0        0        0      812 2024-03-27 19:18:59.000000 qoin-1.0.6/qoin/__init__.py
--rw-rw-rw-   0        0        0    18784 2024-03-29 15:17:22.000000 qoin-1.0.6/qoin/qrng.py
-drwxrwxrwx   0        0        0        0 2024-03-29 15:47:32.381019 qoin-1.0.6/qoin.egg-info/
--rw-rw-rw-   0        0        0    42866 2024-03-29 15:47:32.000000 qoin-1.0.6/qoin.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      210 2024-03-29 15:47:32.000000 qoin-1.0.6/qoin.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-29 15:47:32.000000 qoin-1.0.6/qoin.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       57 2024-03-29 15:47:32.000000 qoin-1.0.6/qoin.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2024-03-29 15:47:32.000000 qoin-1.0.6/qoin.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-03-29 15:47:32.390962 qoin-1.0.6/setup.cfg
--rw-rw-rw-   0        0        0     1971 2024-03-29 15:46:43.000000 qoin-1.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-18 11:10:35.440680 qoin-1.0.7/
+-rw-rw-rw-   0        0        0    35823 2024-03-27 19:02:44.000000 qoin-1.0.7/LICENSE
+-rw-rw-rw-   0        0        0    42866 2024-04-18 11:10:35.437663 qoin-1.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     1052 2024-03-28 14:48:01.000000 qoin-1.0.7/README.md
+-rw-rw-rw-   0        0        0      838 2024-04-18 11:01:42.000000 qoin-1.0.7/pyproject.toml
+drwxrwxrwx   0        0        0        0 2024-04-18 11:10:35.315759 qoin-1.0.7/qoin/
+-rw-rw-rw-   0        0        0      812 2024-03-27 19:18:59.000000 qoin-1.0.7/qoin/__init__.py
+-rw-rw-rw-   0        0        0    18760 2024-04-18 10:58:20.000000 qoin-1.0.7/qoin/qrng.py
+drwxrwxrwx   0        0        0        0 2024-04-18 11:10:35.427526 qoin-1.0.7/qoin.egg-info/
+-rw-rw-rw-   0        0        0    42866 2024-04-18 11:10:34.000000 qoin-1.0.7/qoin.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      210 2024-04-18 11:10:35.000000 qoin-1.0.7/qoin.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-18 11:10:34.000000 qoin-1.0.7/qoin.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       57 2024-04-18 11:10:34.000000 qoin-1.0.7/qoin.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2024-04-18 11:10:34.000000 qoin-1.0.7/qoin.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-18 11:10:35.442772 qoin-1.0.7/setup.cfg
+-rw-rw-rw-   0        0        0     1986 2024-04-17 15:57:04.000000 qoin-1.0.7/setup.py
```

### Comparing `qoin-1.0.6/LICENSE` & `qoin-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `qoin-1.0.6/PKG-INFO` & `qoin-1.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qoin
-Version: 1.0.6
+Version: 1.0.7
 Summary: Quantum Random Number Generator.
 Author: Amir Ali Malekani Nezhad
 Author-email: Amir Ali Malekani Nezhad <amiralimlk07@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
```

### Comparing `qoin-1.0.6/README.md` & `qoin-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `qoin-1.0.6/pyproject.toml` & `qoin-1.0.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "qoin"
-version = "1.0.6"
+version = "1.0.7"
 description = "Quantum Random Number Generator."
 readme = "README.md"
 authors = [{ name = "Amir Ali Malekani Nezhad", email = "amiralimlk07@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Programming Language :: Python",
```

### Comparing `qoin-1.0.6/qoin/__init__.py` & `qoin-1.0.7/qoin/__init__.py`

 * *Files identical despite different names*

### Comparing `qoin-1.0.6/qoin/qrng.py` & `qoin-1.0.7/qoin/qrng.py`

 * *Files 3% similar despite different names*

```diff
@@ -34,58 +34,59 @@
     def __init__(self) -> None:
         """ Initialize a `QRNG` instance.
         """
         self._backend = BackendSampler(AerSimulator())
 
     def randint(self,
                 lowerbound: int,
-                upperbound: int,) -> int:
+                upperbound: int) -> int:
         """ Generate a random integer from [lowerbound, upperbound).
 
         Parameters
         ----------
-        `lowerbound` (int):
+        `lowerbound` : int
             The lowerbound of the selection.
-        `upperbound` (int):
+        `upperbound` : int
             The upperbound of the selection.
 
         Returns
         -------
-        `random_int` (int): The random number generated from the selection.
+        `return_int` : int
+            The random number generated from the selection.
 
         Raises
         ------
-        TypeError:
+        TypeError
             If the lowerbound and upperbound are not integers.
-        ValueError:
+        ValueError
             If the upperbound is less than the lowerbound.
 
         Notes
         -----
         The random integer is generated using the quantum circuit. The quantum
         circuit generates a uniform distribution over all possible integers
         between the lowerbound and upperbound. The distribution is then
         measured to extract the random integer.
 
         The random integer is generated using the following steps:
+
         1. Calculate the difference between the upperbound and lowerbound.
         2. Scale the difference to the closest power of 2.
         3. Calculate the number of qubits needed to represent the selection.
         4. Create a uniform distribution over all possible integers.
         5. Apply measurement to the distribution.
         6. Extract the quasi-probability distribution from the result.
         7. Convert the quasi-probability distribution to counts.
         8. Postprocess the measurement result.
         9. Scale the integer back.
-        10. Shift the random integer's range from [0;upperbound-lowerbound-1]
-            to [lowerbound;upperbound-1].
+        10. Shift range from [0;upperbound-lowerbound-1] to [lowerbound;upperbound-1].
         11. Return the random integer.
 
-        Examples
-        --------
+        Usage
+        -----
         >>> random_integer = qrng.randint(0, 10)
         >>> type_checker = isinstance(random_integer, int)
         >>> bound_checker = random_integer < 10 and random_integer >= 0
         >>> type_checker and bound_checker
         True
         >>> qrng.randint(5.5, 10)
         Traceback (most recent call last):
@@ -150,23 +151,25 @@
         return random_int
 
     def randbin(self) -> bool:
         """ Generate a random boolean.
 
         Returns
         -------
-        `random_bin` (bool): The random boolean.
+        `random_bin` : bool
+            The random boolean.
 
         Notes
         -----
         The random boolean is generated using the quantum circuit. The quantum
         circuit generates a uniform distribution over all possible booleans.
         The distribution is then measured to extract the random boolean.
 
         The random boolean is generated using the following steps:
+
         1. Create a uniform distribution over all possible booleans.
         2. Apply measurement to the distribution.
         3. Extract the quasi-probability distribution from the result.
         4. Convert the quasi-probability distribution to counts.
         5. Postprocess the measurement result.
         6. Return the random boolean.
 
@@ -177,41 +180,43 @@
         >>> bound_checker = random_bool == True or random_bool == False
         >>> type_checker and bound_checker
         True
         """
         return bool(self.randint(0, 2))
 
     def random(self,
-               num_digits: int,) -> float:
+               num_digits: int) -> float:
         """ Generate a random float between 0 and 1.
 
         Parameters
         ----------
-        `num_digits` (int):
+        `num_digits` : int
             The number of bits used to represent the angle divider.
 
         Returns
         -------
-        `random_float`(float): The random generated float.
+        `random_float` : float
+            The random generated float.
 
         Raises
         ------
-        TypeError:
+        TypeError
             If the number of digits is not an integer.
-        ValueError:
+        ValueError
             If the number of digits is less than or equal to 0.
 
         Notes
         -----
         The random float is generated using the quantum circuit. The quantum
         circuit generates a uniform distribution over all possible floats
         between 0 and 1. The distribution is then measured to extract the
         random float.
 
         The random float is generated using the following steps:
+
         1. Calculate the number of bits used to represent the angle divider.
         2. Create a uniform distribution over all possible floats.
         3. Apply measurement to the distribution.
         4. Extract the quasi-probability distribution from the result.
         5. Convert the quasi-probability distribution to counts.
         6. Postprocess the measurement result.
         7. Return the random float.
@@ -248,39 +253,41 @@
             # Generate a random integer between 0 and 9
             random_float += str(self.randint(0, 9))
 
         # Return the random float
         return float(random_float)
 
     def choice(self,
-               items: MutableSequence[Any],) -> Any:
+               items: MutableSequence[Any]) -> Any:
         """ Choose a random element from the list of items.
 
         Parameters
         ----------
-        `items` (MutableSequence[Any]):
+        `items` : MutableSequence[Any]
             The list of items.
 
         Returns
         -------
-        (Any): The item selected.
+        Any
+            The item selected.
 
         Raises
         ------
-        TypeError:
+        TypeError
             If the items are not an instance of MutableSequence.
 
         Notes
         -----
         The random element is selected using the quantum circuit. The quantum
         circuit generates a uniform distribution over all possible elements in
         the list. The distribution is then measured to extract the random
         element.
 
         The random element is selected using the following steps:
+
         1. Create a uniform distribution over all possible elements.
         2. Apply measurement to the distribution.
         3. Extract the quasi-probability distribution from the result.
         4. Convert the quasi-probability distribution to counts.
         5. Postprocess the measurement result.
         6. Return the random element.
 
@@ -288,53 +295,55 @@
         --------
         >>> random_choice = qrng.choice([1, 2, 3, 4, 5])
         >>> random_choice in [1, 2, 3, 4, 5]
         True
         >>> qrng.choice(1)
         Traceback (most recent call last):
             ...
-        TypeError: Population must be a MutableSequence or set.
+        TypeError: Population must be a MutableSequence.
         """
         # Ensure that the items are MutableSequence
         if not isinstance(items, MutableSequence):
             raise TypeError("Population must be a MutableSequence.")
 
         return items[self.randint(0, len(items))]
 
     def choices(self,
                 items: MutableSequence[Any],
-                num_selections: int,) -> Any | list[Any]:
+                num_selections: int) -> Any | list[Any]:
         """ Choose random element(s) from the list of items.
 
         Parameters
         ----------
-        `items` (MutableSequence[Any]):
+        `items` : MutableSequence[Any]
             The list of items.
-        `num_selections` (int):
+        `num_selections` : int
             The number of selections.
 
         Returns
         -------
-        (Any | list[Any]): The item(s) selected.
+        Any | list[Any]
+            The item(s) selected.
 
         Raises
         ------
-        TypeError:
+        TypeError
             If the items are not MutableSequence.
-        ValueError:
+        ValueError
             If the number of selections is less than or equal to 0.
 
         Notes
         -----
         The random element(s) are selected using the quantum circuit. The
         quantum circuit generates a uniform distribution over all possible
         elements in the list. The distribution is then measured to extract the
         random element(s).
 
         The random element(s) are selected using the following steps:
+
         1. Calculate the number of selections.
         2. Create a uniform distribution over all possible elements.
         3. Apply measurement to the distribution.
         4. Extract the quasi-probability distribution from the result.
         5. Convert the quasi-probability distribution to counts.
         6. Postprocess the measurement result.
         7. Return the random element(s).
@@ -343,23 +352,23 @@
         --------
         >>> random_choices = qrng.choices([1, 2, 3, 4, 5], 3)
         >>> all(random_choice in [1, 2, 3, 4, 5] for random_choice in random_choices)
         True
         >>> qrng.choices(1, 3)
         Traceback (most recent call last):
             ...
-        TypeError: Population must be a MutableSequence or set.
+        TypeError: Population must be a MutableSequence.
         >>> qrng.choices([1, 2, 3, 4, 5], 0)
         Traceback (most recent call last):
             ...
         ValueError: Sample larger than population or is negative.
         """
         # Ensure that the items are MutableSequence
         if not isinstance(items, MutableSequence):
-            raise TypeError("Population must be a MutableSequence or set.")
+            raise TypeError("Population must be a MutableSequence.")
 
         # Ensure that the number of selections is valid
         if num_selections <= 0:
             raise ValueError("Sample larger than population or is negative.")
 
         # Define indices list
         indices = []
@@ -372,70 +381,72 @@
         indices = [self.randint(0, len(items)) for _ in range(num_selections)]
 
         # Return the selections
         return [items[i] for i in indices]
 
     def sample(self,
                items: MutableSequence[Any],
-               num_selections: int,) -> Any | list[Any]:
+               num_selections: int) -> Any | list[Any]:
         """ Choose random element(s) from the list of items.
 
         Parameters
         ----------
-        `items` (MutableSequence[Any]):
+        `items` : MutableSequence[Any]
             The list of items.
-        `num_selections` (int):
+        `num_selections` : int
             The number of selections.
 
         Returns
         -------
-        (Any | list[Any]): The item(s) selected.
+        Any | list[Any]
+            The item(s) selected.
 
         Raises
         ------
-        TypeError:
+        TypeError
             If the items are not MutableSequence.
-        ValueError:
+        ValueError
             If the number of selections is less than or equal to 0.
 
         Notes
         -----
         The random element(s) are selected using the quantum circuit. The
         quantum circuit generates a uniform distribution over all possible
         elements in the list. The distribution is then measured to extract the
         random element(s).
 
         The random element(s) are selected using the following steps:
+
         1. Calculate the number of selections.
         2. Create a uniform distribution over all possible elements.
         3. Apply measurement to the distribution.
         4. Extract the quasi-probability distribution from the result.
         5. Convert the quasi-probability distribution to counts.
         6. Postprocess the measurement result.
         7. Return the random element(s).
 
         Examples
         --------
         >>> random_samples = qrng.sample([1, 2, 3, 4, 5], 3)
-        >>> bound_checker = all(random_sample in [1, 2, 3, 4, 5]\
-            for random_sample in random_samples)
+        >>> bound_checker = all(random_sample in [1, 2, 3, 4, 5]
+        ... for random_sample in random_samples)
         >>> unique_checker = len(set(random_samples)) == 3
         >>> bound_checker and unique_checker
         True
         >>> qrng.sample(1, 3)
         Traceback (most recent call last):
             ...
-        TypeError: Population must be a MutableSequence or set.
+        TypeError: Population must be a MutableSequence.
         >>> qrng.sample([1, 2, 3, 4, 5], 6)
         Traceback (most recent call last):
             ...
         ValueError: Sample larger than population or is negative.
         """
         if not isinstance(items, MutableSequence):
-            raise TypeError("Population must be a MutableSequence or set.")
+            raise TypeError("Population must be a MutableSequence.")
 
         # Ensure that the number of selections is valid
         if not (num_selections > 0 and num_selections <= len(items)):
             raise ValueError("Sample larger than population or is negative.")
 
         # Define indices list
         indices: list[Any] = []
@@ -456,39 +467,41 @@
             if random_index not in indices:
                 indices.append(random_index)
 
         # Return the selections
         return [items[i] for i in indices]
 
     def shuffle(self,
-                items: MutableSequence[Any],) -> list[Any]:
+                items: MutableSequence[Any]) -> list[Any]:
         """ Shuffle the list of items.
 
         Parameters
         ----------
-        `items` (list[Any]):
+        `items` : list[Any]
             The list of items to shuffle.
 
         Returns
         -------
-        (list[Any]): The shuffled list of items.
+        list[Any]
+            The shuffled list of items.
 
         Raises
         ------
-        TypeError:
+        TypeError
             If the items are not a list.
 
         Notes
         -----
         The list of items is shuffled using the quantum circuit. The quantum
         circuit generates a uniform distribution over all possible permutations
         of the list. The distribution is then measured to extract the random
         permutation.
 
         The list of items is shuffled using the following steps:
+
         1. Create a uniform distribution over all possible permutations.
         2. Apply measurement to the distribution.
         3. Extract the quasi-probability distribution from the result.
         4. Convert the quasi-probability distribution to counts.
         5. Postprocess the measurement result.
         6. Return the shuffled list of items.
 
@@ -496,18 +509,18 @@
         --------
         >>> shuffled = qrng.shuffle([1, 2, 3, 4, 5])
         >>> len(set(shuffled)) == 5
         True
         >>> qrng.shuffle(1)
         Traceback (most recent call last):
             ...
-        TypeError: Population must be a MutableSequence or set.
+        TypeError: Population must be a MutableSequence.
         """
         # Ensure that the items are a list
         if not isinstance(items, list):
-            raise TypeError("Population must be a MutableSequence or set.")
+            raise TypeError("Population must be a MutableSequence.")
 
         return self.sample(items, len(items))
 
 if __name__ == '__main__':
     import doctest
     doctest.testmod(extraglobs={'qrng': QRNG()})
```

### Comparing `qoin-1.0.6/qoin.egg-info/PKG-INFO` & `qoin-1.0.7/qoin.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qoin
-Version: 1.0.6
+Version: 1.0.7
 Summary: Quantum Random Number Generator.
 Author: Amir Ali Malekani Nezhad
 Author-email: Amir Ali Malekani Nezhad <amiralimlk07@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
```

### Comparing `qoin-1.0.6/setup.py` & `qoin-1.0.7/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,23 +12,23 @@
 # GNU General Public License for more details.
 
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
 import codecs
 import os
-from setuptools import setup, find_packages
+from setuptools import setup, find_packages # type: ignore
 
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '1.0.6'
+VERSION = '1.0.7'
 DESCRIPTION = 'Quantum Random Number Generator.'
 LONG_DESCRIPTION = '`qoin` is the analogue of `random` package implemented through \
 gate-based quantum computing.'
 
 # Setting up
 setup(
     name="qoin",
```

