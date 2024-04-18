# Comparing `tmp/anjana-0.0.1.post1.tar.gz` & `tmp/anjana-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anjana-0.0.1.post1.tar", max compression
+gzip compressed data, was "anjana-0.0.2.tar", max compression
```

## Comparing `anjana-0.0.1.post1.tar` & `anjana-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0    11353 2024-03-19 16:17:26.810719 anjana-0.0.1.post1/LICENSE
--rw-r--r--   0        0        0     4711 2024-04-11 07:00:56.429436 anjana-0.0.1.post1/README.md
--rw-r--r--   0        0        0      749 2024-04-11 07:42:52.316264 anjana-0.0.1.post1/anjana/__init__.py
--rw-r--r--   0        0        0     1277 2024-04-10 10:21:10.035760 anjana-0.0.1.post1/anjana/anonymity/__init__.py
--rw-r--r--   0        0        0     6416 2024-04-10 10:21:10.035760 anjana-0.0.1.post1/anjana/anonymity/_beta_likeness.py
--rw-r--r--   0        0        0     3629 2024-04-10 10:21:10.035760 anjana-0.0.1.post1/anjana/anonymity/_delta_disclosure.py
--rw-r--r--   0        0        0    10095 2024-04-10 10:21:10.035760 anjana-0.0.1.post1/anjana/anonymity/_k_anonymity.py
--rw-r--r--   0        0        0    13419 2024-04-10 10:21:10.035760 anjana-0.0.1.post1/anjana/anonymity/_l_diversity.py
--rw-r--r--   0        0        0     3501 2024-04-10 10:21:10.035760 anjana-0.0.1.post1/anjana/anonymity/_t_closeness.py
--rw-r--r--   0        0        0      784 2024-03-20 08:17:01.773369 anjana-0.0.1.post1/anjana/anonymity/utils/__init__.py
--rw-r--r--   0        0        0     3552 2024-04-10 10:40:59.006301 anjana-0.0.1.post1/anjana/anonymity/utils/utils.py
--rw-r--r--   0        0        0     2054 2024-04-11 08:17:33.117704 anjana-0.0.1.post1/pyproject.toml
--rw-r--r--   0        0        0     6206 1970-01-01 00:00:00.000000 anjana-0.0.1.post1/PKG-INFO
+-rw-r--r--   0        0        0    11353 2024-03-19 16:17:26.810719 anjana-0.0.2/LICENSE
+-rw-r--r--   0        0        0     8178 2024-04-17 15:18:31.376020 anjana-0.0.2/README.md
+-rw-r--r--   0        0        0      743 2024-04-18 11:34:03.385593 anjana-0.0.2/anjana/__init__.py
+-rw-r--r--   0        0        0     1277 2024-04-10 10:21:10.035760 anjana-0.0.2/anjana/anonymity/__init__.py
+-rw-r--r--   0        0        0     6416 2024-04-10 10:21:10.035760 anjana-0.0.2/anjana/anonymity/_beta_likeness.py
+-rw-r--r--   0        0        0     3629 2024-04-10 10:21:10.035760 anjana-0.0.2/anjana/anonymity/_delta_disclosure.py
+-rw-r--r--   0        0        0    10095 2024-04-10 10:21:10.035760 anjana-0.0.2/anjana/anonymity/_k_anonymity.py
+-rw-r--r--   0        0        0    13419 2024-04-10 10:21:10.035760 anjana-0.0.2/anjana/anonymity/_l_diversity.py
+-rw-r--r--   0        0        0     3501 2024-04-10 10:21:10.035760 anjana-0.0.2/anjana/anonymity/_t_closeness.py
+-rw-r--r--   0        0        0      940 2024-04-18 11:15:39.469543 anjana-0.0.2/anjana/anonymity/utils/__init__.py
+-rw-r--r--   0        0        0     4806 2024-04-18 11:34:03.385593 anjana-0.0.2/anjana/anonymity/utils/utils.py
+-rw-r--r--   0        0        0     2048 2024-04-18 11:34:03.385593 anjana-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     9667 1970-01-01 00:00:00.000000 anjana-0.0.2/PKG-INFO
```

### Comparing `anjana-0.0.1.post1/LICENSE` & `anjana-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `anjana-0.0.1.post1/anjana/__init__.py` & `anjana-0.0.2/anjana/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -12,8 +12,8 @@
 # distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 # License for the specific language governing permissions and limitations
 # under the License.
 
 """ANJANA is an open source framework for anonymizing data with different techniques."""
 
-__version__ = "0.0.1.post1"
+__version__ = "0.0.2"
```

### Comparing `anjana-0.0.1.post1/anjana/anonymity/__init__.py` & `anjana-0.0.2/anjana/anonymity/__init__.py`

 * *Files identical despite different names*

### Comparing `anjana-0.0.1.post1/anjana/anonymity/_beta_likeness.py` & `anjana-0.0.2/anjana/anonymity/_beta_likeness.py`

 * *Files identical despite different names*

### Comparing `anjana-0.0.1.post1/anjana/anonymity/_delta_disclosure.py` & `anjana-0.0.2/anjana/anonymity/_delta_disclosure.py`

 * *Files identical despite different names*

### Comparing `anjana-0.0.1.post1/anjana/anonymity/_k_anonymity.py` & `anjana-0.0.2/anjana/anonymity/_k_anonymity.py`

 * *Files identical despite different names*

### Comparing `anjana-0.0.1.post1/anjana/anonymity/_l_diversity.py` & `anjana-0.0.2/anjana/anonymity/_l_diversity.py`

 * *Files identical despite different names*

### Comparing `anjana-0.0.1.post1/anjana/anonymity/_t_closeness.py` & `anjana-0.0.2/anjana/anonymity/_t_closeness.py`

 * *Files identical despite different names*

### Comparing `anjana-0.0.1.post1/anjana/anonymity/utils/utils.py` & `anjana-0.0.2/anjana/anonymity/utils/utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -99,13 +99,53 @@
         with the hierarchies and the levels
 
     :return: level of generalization applied to each QI.
     :rtype: dict
     """
     gen_level = {}
     for qi in quasi_ident:
-        for level in hierarchies[qi].keys():
-            hierarchy_level = set(hierarchies[qi][level])
-            if set(data[qi].values).issubset(hierarchy_level):
-                gen_level[qi] = level
+        if qi in hierarchies.keys():
+            for level in hierarchies[qi].keys():
+                hierarchy_level = set(hierarchies[qi][level])
+                if set(data[qi].values).issubset(hierarchy_level):
+                    gen_level[qi] = level
 
     return gen_level
+
+
+@beartype()
+def get_transformation(
+    data_anon: pd.DataFrame,
+    quasi_ident: typing.Union[typing.List, np.ndarray],
+    hierarchies: dict,
+) -> list:
+    """Get the transformation applied for anonymizing the data.
+
+    Example: a transformation (0,1,2,0) means:
+    - Level 0 of generalization for th 1st QI
+    - Level 1 of generalization for th 2nd QI
+    - Level 2 of generalization for th 3rd QI
+    - Level 0 of generalization for the 4th QI
+
+    :param data_anon: data under study.
+    :type data_anon: pandas dataframe
+
+    :param quasi_ident: list with the name of the columns of the dataframe
+        that are quasi-identifiers.
+    :type quasi_ident: list of strings
+
+    :param hierarchies: hierarchies for generalizing the QI.
+    :type hierarchies: dictionary containing one dictionary for QI
+        with the hierarchies and the levels
+
+    :return: transformation applied
+    :rtype: list
+    """
+    gen_level = check_gen_level(data_anon, quasi_ident, hierarchies)
+    transformation = []
+    for qi in quasi_ident:
+        if qi in gen_level.keys():
+            transformation.append(gen_level[qi])
+        else:
+            transformation.append(0)
+
+    return transformation
```

### Comparing `anjana-0.0.1.post1/pyproject.toml` & `anjana-0.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "anjana"
-version = "0.0.1.post1"
+version = "0.0.2"
 description = "ANJANA is an open source framework for applying different anonymity techniques."
 authors = [
     "Judith Sáinz-Pardo Díaz <sainzpardo@ifca.unican.es>",
     "Álvaro López García <aloga@ifca.unican.es>"
 ]
 maintainers = ["Judith Sáinz-Pardo Díaz <sainzpardo@ifca.unican.es>"]
 license = "Apache License 2.0"
```

### Comparing `anjana-0.0.1.post1/PKG-INFO` & `anjana-0.0.2/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anjana
-Version: 0.0.1.post1
+Version: 0.0.2
 Summary: ANJANA is an open source framework for applying different anonymity techniques.
 Home-page: https://gitlab.ifca.es/privacy-security/anjana
 License: Apache-2.0
 Keywords: anonymity,privacy
 Author: Judith Sáinz-Pardo Díaz
 Author-email: sainzpardo@ifca.unican.es
 Maintainer: Judith Sáinz-Pardo Díaz
@@ -32,35 +32,57 @@
 Requires-Dist: tabulate (==0.9.0)
 Requires-Dist: typing_extensions (==4.9.0)
 Project-URL: Repository, https://gitlab.ifca.es/privacy-security/anjana
 Description-Content-Type: text/markdown
 
 # ANJANA
 [![License: Apache 2.0](https://img.shields.io/badge/License-Apache_2.0-green.svg)](https://gitlab.ifca.es/privacy-security/anjana/-/blob/main/LICENSE)
-[![Pipeline Status](https://gitlab.ifca.es/privacy-security/anjana/badges/main/pipeline.svg)](https://gitlab.ifca.es/privacy-security/anjana/-/pipelines)
+[![codecov](https://codecov.io/gh/IFCA-Advanced-Computing/anjana/graph/badge.svg?token=AVI53GZ7YD)](https://codecov.io/gh/IFCA-Advanced-Computing/anjana)
 
 ![Python version](https://img.shields.io/badge/python-3.9|3.10|3.11|3.12-blue)
 
 
-**Anonymity as major assurance of personal data privacy**
+**Anonymity as major assurance of personal data privacy:**
 
 ANJANA is a Python library for anonymizing sensitive data.
 
 The following anonymity techniques are implemented, based on the Python library _[pyCANON](https://github.com/IFCA-Advanced-Computing/pycanon)_:
 * _k-anonymity_.
 * _(α,k)-anonymity_.
 * _ℓ-diversity_.
 * _Entropy ℓ-diversity_.
 * _Recursive (c,ℓ)-diversity_.
 * _t-closeness_.
 * _Basic β-likeness_.
 * _Enhanced β-likeness_.
 * _δ-disclosure privacy_.
 
-## Getting started
+## :bulb: Installation
+First, we strongly recommend the use of a virtual environment. In linux: 
+```bash
+virtualenv .venv -p python3
+source .venv/bin/activate
+```
+
+**Using [pip](https://pypi.org/project/anjana/)**:
+
+Install anjana (linux and windows):
+```bash
+pip install anjana
+```
+
+**Using git**:
+
+Install the most updated version of anjana (linux and windows):
+
+```bash
+pip install git+https://github.com/IFCA-Advanced-Computing/anjana.git
+```
+
+## :rocket: Getting started
 
 For anonymizing your data you need to introduce:
 * The **pandas dataframe** with the data to be anonymized. Each column can contain: indentifiers, quasi-indentifiers or sensitive attributes.
 * The **list with the names of the identifiers** in the dataframe, in order to suppress them.
 * The **list with the names of the quasi-identifiers** in the dataframe.
 * The **sentive attribute** (only one) in case of applying other techniques than _k-anonymity_.
 * The **level of anonymity to be applied**, e.g. _k_ (for _k-anonymity_), _ℓ_ (for _ℓ-diversity_), _t_ (for _t-closeness_), _β_ (for _basic or enhanced β-likeness_), etc.
@@ -125,18 +147,63 @@
 data_anon = t_closeness(
     data_anon, ident, quasi_ident, sens_att, k, t, supp_level, hierarchies
 )
 ```
 
 The previous code can be executed in less than 4 seconds for the more than 30,000 records of the original dataset.
 
-## License
+### Define your own hierarchies
+
+All the anonymity functions available in ANJANA receive a dictionary with the hierarchies to be applied to the quasi-identifiers. In particular, this dictionary has as key the names of the columns that are quasi-identifiers to which a hierarchy is to be applied (it may happen that you do not want to generalize some QIs and therefore no hierarchy is to be applied to them, just do not include them in this dictionary). The value for each key (QI) is formed by a dictionary in such a way that the value 0 has as value the raw column (as it is in the original dataset), the value 1 corresponds to the first level of transformation to be applied, in relation to the values of the original column, and so on with as many keys as levels of hierarchies have been established. 
+
+For a better understanding, let's look at the following example. Supose that we have the following simulated dataset (extracted from the [_hospital_extended.csv_](https://github.com/IFCA-Advanced-Computing/anjana/blob/main/examples/data/hospital_extended.csv) dataset used for testing purposes) with _age_, _gender_ and _city_ as quasi-identifiers, _name_ as identifier and _disease_ as sensitive attribute. Regarding the QI, we want to apply the following hierarquies: interval of 5 years (first level) and 10 years (second level) for the _age_. Suppression as first level for both _gender_ and _city_.
+
+| name      | age | gender | city       | disease        |
+|-----------|-----|--------|------------|----------------|
+| Ramsha    | 29  | Female | Tamil Nadu | Cancer         |
+| Yadu      | 24  | Female | Kerala     | Viralinfection |
+| Salima    | 28  | Female | Tamil Nadu | TB             |
+| Sunny     | 27  | Male   | Karnataka  | No illness     |
+| Joan      | 24  | Female | Kerala     | Heart-related  |
+| Bahuksana | 23  | Male   | Karnataka  | TB             |
+| Rambha    | 19  | Male   | Kerala     | Cancer         |
+| Kishor    | 29  | Male   | Karnataka  | Heart-related  |
+| Johnson   | 17  | Male   | Kerala     | Heart-related  |
+| John      | 19  | Male   | Kerala     | Viralinfection |
+
+Then, in order to create the hierarquies we can define the following dictionary:
+
+```python
+age = data['age'].values
+# Values: [29 24 28 27 24 23 19 29 17 19] (note that the following can be automatized)
+age_5years = ['[25, 30)', '[20, 25)', '[25, 30)',
+              '[25, 30)', '[20, 25)', '[20, 25)',
+              '[15, 20)', '[25, 30)', '[15, 20)', '[15, 20)']
+
+age_10years = ['[20, 30)', '[20, 30)', '[20, 30)',
+               '[20, 30)', '[20, 30)', '[20, 30)',
+               '[10, 20)', '[20, 30)', '[10, 20)', '[10, 20)']
+
+hierarchies = {
+    "age": {0: age,
+            1: age_5years,
+            2: age_10years},
+    "gender": {
+        0: data["gender"].values,
+        1: np.array(["*"] * len(data["gender"].values)) # Suppression
+    },
+    "city": {0: data["city"].values,
+             1: np.array(["*"] * len(data["city"].values))} # Suppression
+}
+```
+
+## :scroll: License
 This project is licensed under the [Apache 2.0 license](https://gitlab.ifca.es/privacy-security/anjana/-/blob/main/LICENSE?ref_type=heads).
 
-## Project status
+## :warning: Project status
 This project is under active development.
 
 ## Funding and acknowledgments
 This work is funded by European Union through the SIESTA project (Horizon Europe) under Grant number 101131957.
 <p>
 <img align="center" width="250" src="https://ec.europa.eu/regional_policy/images/information-sources/logo-download-center/eu_funded_en.jpg">
 <img align="center" width="250" src="https://eosc.eu/wp-content/uploads/2024/01/SIESTA-Logo-1.png">
```

