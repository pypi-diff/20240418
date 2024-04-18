# Comparing `tmp/qoqo_qiskit-0.3.0.tar.gz` & `tmp/qoqo_qiskit-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qoqo_qiskit-0.3.0.tar", last modified: Thu Feb 29 15:10:21 2024, max compression
+gzip compressed data, was "qoqo_qiskit-0.4.0.tar", last modified: Thu Apr 18 12:29:18 2024, max compression
```

## Comparing `qoqo_qiskit-0.3.0.tar` & `qoqo_qiskit-0.4.0.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 15:10:21.468870 qoqo_qiskit-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-02-29 15:10:07.000000 qoqo_qiskit-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    15354 2024-02-29 15:10:21.468870 qoqo_qiskit-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-02-29 15:10:07.000000 qoqo_qiskit-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 15:10:21.460870 qoqo_qiskit-0.3.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      612 2024-02-29 15:10:07.000000 qoqo_qiskit-0.3.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     5837 2024-02-29 15:10:07.000000 qoqo_qiskit-0.3.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      367 2024-02-29 15:10:07.000000 qoqo_qiskit-0.3.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3569 2024-02-29 15:10:07.000000 qoqo_qiskit-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-29 15:10:21.468870 qoqo_qiskit-0.3.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 15:10:21.460870 qoqo_qiskit-0.3.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 15:10:21.460870 qoqo_qiskit-0.3.0/src/qoqo_qiskit/
--rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-02-29 15:10:07.000000 qoqo_qiskit-0.3.0/src/qoqo_qiskit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 15:10:21.464870 qoqo_qiskit-0.3.0/src/qoqo_qiskit/backend/
--rw-r--r--   0 runner    (1001) docker     (127)      885 2024-02-29 15:10:07.000000 qoqo_qiskit-0.3.0/src/qoqo_qiskit/backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14250 2024-02-29 15:10:07.000000 qoqo_qiskit-0.3.0/src/qoqo_qiskit/backend/backend.py
--rw-r--r--   0 runner    (1001) docker     (127)     3774 2024-02-29 15:10:07.000000 qoqo_qiskit-0.3.0/src/qoqo_qiskit/backend/post_processing.py
--rw-r--r--   0 runner    (1001) docker     (127)    11221 2024-02-29 15:10:07.000000 qoqo_qiskit-0.3.0/src/qoqo_qiskit/backend/queued_results.py
--rw-r--r--   0 runner    (1001) docker     (127)     1515 2024-02-29 15:10:07.000000 qoqo_qiskit-0.3.0/src/qoqo_qiskit/backend/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 15:10:21.464870 qoqo_qiskit-0.3.0/src/qoqo_qiskit/interface/
--rw-r--r--   0 runner    (1001) docker     (127)      731 2024-02-29 15:10:07.000000 qoqo_qiskit-0.3.0/src/qoqo_qiskit/interface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5938 2024-02-29 15:10:07.000000 qoqo_qiskit-0.3.0/src/qoqo_qiskit/interface/interface.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 15:10:21.464870 qoqo_qiskit-0.3.0/src/qoqo_qiskit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    15354 2024-02-29 15:10:21.000000 qoqo_qiskit-0.3.0/src/qoqo_qiskit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      735 2024-02-29 15:10:21.000000 qoqo_qiskit-0.3.0/src/qoqo_qiskit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-29 15:10:21.000000 qoqo_qiskit-0.3.0/src/qoqo_qiskit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-02-29 15:10:21.000000 qoqo_qiskit-0.3.0/src/qoqo_qiskit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-02-29 15:10:21.000000 qoqo_qiskit-0.3.0/src/qoqo_qiskit.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 15:10:21.464870 qoqo_qiskit-0.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      731 2024-02-29 15:10:07.000000 qoqo_qiskit-0.3.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 15:10:21.464870 qoqo_qiskit-0.3.0/tests/backend/
--rw-r--r--   0 runner    (1001) docker     (127)      704 2024-02-29 15:10:07.000000 qoqo_qiskit-0.3.0/tests/backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13529 2024-02-29 15:10:07.000000 qoqo_qiskit-0.3.0/tests/backend/test_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)     5414 2024-02-29 15:10:07.000000 qoqo_qiskit-0.3.0/tests/backend/test_queued_results.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 15:10:21.464870 qoqo_qiskit-0.3.0/tests/interface/
--rw-r--r--   0 runner    (1001) docker     (127)      689 2024-02-29 15:10:07.000000 qoqo_qiskit-0.3.0/tests/interface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5352 2024-02-29 15:10:07.000000 qoqo_qiskit-0.3.0/tests/interface/test_interface.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:29:18.117527 qoqo_qiskit-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-18 12:29:06.000000 qoqo_qiskit-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    15354 2024-04-18 12:29:18.117527 qoqo_qiskit-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-18 12:29:06.000000 qoqo_qiskit-0.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:29:18.109527 qoqo_qiskit-0.4.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      612 2024-04-18 12:29:06.000000 qoqo_qiskit-0.4.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     5837 2024-04-18 12:29:06.000000 qoqo_qiskit-0.4.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      367 2024-04-18 12:29:06.000000 qoqo_qiskit-0.4.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3569 2024-04-18 12:29:06.000000 qoqo_qiskit-0.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 12:29:18.117527 qoqo_qiskit-0.4.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:29:18.109527 qoqo_qiskit-0.4.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:29:18.109527 qoqo_qiskit-0.4.0/src/qoqo_qiskit/
+-rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-04-18 12:29:06.000000 qoqo_qiskit-0.4.0/src/qoqo_qiskit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:29:18.113527 qoqo_qiskit-0.4.0/src/qoqo_qiskit/backend/
+-rw-r--r--   0 runner    (1001) docker     (127)      885 2024-04-18 12:29:06.000000 qoqo_qiskit-0.4.0/src/qoqo_qiskit/backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18370 2024-04-18 12:29:06.000000 qoqo_qiskit-0.4.0/src/qoqo_qiskit/backend/backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3774 2024-04-18 12:29:06.000000 qoqo_qiskit-0.4.0/src/qoqo_qiskit/backend/post_processing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11221 2024-04-18 12:29:06.000000 qoqo_qiskit-0.4.0/src/qoqo_qiskit/backend/queued_results.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1515 2024-04-18 12:29:06.000000 qoqo_qiskit-0.4.0/src/qoqo_qiskit/backend/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:29:18.113527 qoqo_qiskit-0.4.0/src/qoqo_qiskit/interface/
+-rw-r--r--   0 runner    (1001) docker     (127)      731 2024-04-18 12:29:06.000000 qoqo_qiskit-0.4.0/src/qoqo_qiskit/interface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5938 2024-04-18 12:29:06.000000 qoqo_qiskit-0.4.0/src/qoqo_qiskit/interface/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:29:18.113527 qoqo_qiskit-0.4.0/src/qoqo_qiskit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    15354 2024-04-18 12:29:18.000000 qoqo_qiskit-0.4.0/src/qoqo_qiskit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      735 2024-04-18 12:29:18.000000 qoqo_qiskit-0.4.0/src/qoqo_qiskit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 12:29:18.000000 qoqo_qiskit-0.4.0/src/qoqo_qiskit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-04-18 12:29:18.000000 qoqo_qiskit-0.4.0/src/qoqo_qiskit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-18 12:29:18.000000 qoqo_qiskit-0.4.0/src/qoqo_qiskit.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:29:18.113527 qoqo_qiskit-0.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      731 2024-04-18 12:29:06.000000 qoqo_qiskit-0.4.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:29:18.113527 qoqo_qiskit-0.4.0/tests/backend/
+-rw-r--r--   0 runner    (1001) docker     (127)      704 2024-04-18 12:29:06.000000 qoqo_qiskit-0.4.0/tests/backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17620 2024-04-18 12:29:06.000000 qoqo_qiskit-0.4.0/tests/backend/test_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5414 2024-04-18 12:29:06.000000 qoqo_qiskit-0.4.0/tests/backend/test_queued_results.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:29:18.113527 qoqo_qiskit-0.4.0/tests/interface/
+-rw-r--r--   0 runner    (1001) docker     (127)      689 2024-04-18 12:29:06.000000 qoqo_qiskit-0.4.0/tests/interface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5352 2024-04-18 12:29:06.000000 qoqo_qiskit-0.4.0/tests/interface/test_interface.py
```

### Comparing `qoqo_qiskit-0.3.0/LICENSE` & `qoqo_qiskit-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `qoqo_qiskit-0.3.0/PKG-INFO` & `qoqo_qiskit-0.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qoqo_qiskit
-Version: 0.3.0
+Version: 0.4.0
 Author-email: HQS Quantum Simulation GmbH <info@quantumsimulations.de>
 Maintainer-email: Matteo Lodi <matteo.lodi@quantumsimulations.de>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `qoqo_qiskit-0.3.0/README.md` & `qoqo_qiskit-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `qoqo_qiskit-0.3.0/docs/Makefile` & `qoqo_qiskit-0.4.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `qoqo_qiskit-0.3.0/docs/conf.py` & `qoqo_qiskit-0.4.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `qoqo_qiskit-0.3.0/pyproject.toml` & `qoqo_qiskit-0.4.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "qoqo_qiskit"
-version = "0.3.0"
+version = "0.4.0"
 license = { file = "LICENSE" }
 authors = [
     { name = "HQS Quantum Simulation GmbH", email = "info@quantumsimulations.de" },
 ]
 maintainers = [
     { name = "Matteo Lodi", email = "matteo.lodi@quantumsimulations.de" },
 ]
```

### Comparing `qoqo_qiskit-0.3.0/src/qoqo_qiskit/__init__.py` & `qoqo_qiskit-0.4.0/src/qoqo_qiskit/__init__.py`

 * *Files identical despite different names*

### Comparing `qoqo_qiskit-0.3.0/src/qoqo_qiskit/backend/__init__.py` & `qoqo_qiskit-0.4.0/src/qoqo_qiskit/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `qoqo_qiskit-0.3.0/src/qoqo_qiskit/backend/backend.py` & `qoqo_qiskit-0.4.0/src/qoqo_qiskit/backend/backend.py`

 * *Files 23% similar despite different names*

```diff
@@ -7,21 +7,22 @@
 #
 # Unless required by applicable law or agreed to in writing, software distributed under the License
 # is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express
 # or implied. See the License for the specific language governing permissions and limitations under
 # the License.
 """Qoqo-qiskit backend for simulation purposes."""
 
-from typing import Any, Dict, List, Optional, Tuple, cast
+from typing import Any, Dict, List, Optional, Tuple, Union, cast
 
 from qiskit import QuantumCircuit, execute
 from qiskit.providers import Backend
 from qiskit.providers.job import Job
 from qiskit_aer import AerSimulator
-from qoqo import Circuit
+from qoqo import Circuit, QuantumProgram
+from qoqo.measurements import ClassicalRegister  # type:ignore
 
 from qoqo_qiskit.backend.queued_results import QueuedCircuitRun, QueuedProgramRun
 from qoqo_qiskit.interface import to_qiskit_circuit
 
 from .post_processing import _transform_job_result
 
 
@@ -368,14 +369,71 @@
 
         return measurement.evaluate(
             output_bit_register_dict,
             output_float_register_dict,
             output_complex_register_dict,
         )
 
+    def run_program(self, program: QuantumProgram, params_values: List[List[float]]) -> Optional[
+        List[
+            Union[
+                Tuple[
+                    Dict[str, List[List[bool]]],
+                    Dict[str, List[List[float]]],
+                    Dict[str, List[List[complex]]],
+                ],
+                Dict[str, float],
+            ]
+        ]
+    ]:
+        """Run a qoqo quantum program on an IBM backend multiple times.
+
+        It can handle QuantumProgram instances containing any kind of measurement. The list of
+        lists of parameters will be used to call `program.run(self, params)` or
+        `program.run_registers(self, params)` as many times as the number of sublists.
+        The return type will change accordingly.
+
+        If no parameters values are provided, a normal call `program.run(self, [])` call
+        will be executed.
+
+        Args:
+            program (QuantumProgram): the qoqo quantum program to run.
+            params_values (List[List[float]]): the parameters values to pass to the quantum
+                program.
+
+        Returns:
+            Optional[
+                List[
+                    Union[
+                        Tuple[
+                            Dict[str, List[List[bool]]],
+                            Dict[str, List[List[float]]],
+                            Dict[str, List[List[complex]]],
+                        ],
+                        Dict[str, float],
+                    ]
+                ]
+            ]: list of dictionaries (or tuples of dictionaries) containing the
+                run results.
+        """
+        returned_results = []
+
+        if isinstance(program.measurement(), ClassicalRegister):
+            if not params_values:
+                returned_results.append(program.run_registers(self, []))
+            for params in params_values:
+                returned_results.append(program.run_registers(self, params))
+        else:
+            if not params_values:
+                returned_results.append(program.run(self, []))
+            for params in params_values:
+                returned_results.append(program.run(self, params))
+
+        return returned_results
+
     def run_measurement_queued(self, measurement: Any) -> QueuedProgramRun:
         """Run a qoqo measurement on a Qiskit backend and return a queued Job Result.
 
         The default number of shots for the simulation is 200.
         Any kind of Measurement, Statevector or DensityMatrix instruction only works as intended if
         they are the last instructions in the Circuit.
         Currently only one simulation is performed, meaning different measurements on different
@@ -393,7 +451,51 @@
             if constant_circuit is None:
                 run_circuit = circuit
             else:
                 run_circuit = constant_circuit + circuit
 
             queued_circuits.append(self.run_circuit_queued(run_circuit))
         return QueuedProgramRun(measurement, queued_circuits)
+
+    def run_program_queued(
+        self, program: QuantumProgram, params_values: List[List[float]]
+    ) -> List[QueuedProgramRun]:
+        """Run a qoqo quantum program on a AWS backend multiple times return a list of queued Jobs.
+
+        This effectively performs the same operations as `run_program` but returns
+        queued results.
+
+
+        Args:
+            program (QuantumProgram): the qoqo quantum program to run.
+            params_values (List[List[float]]): the parameters values to pass to the quantum
+                program.
+
+        Raises:
+            ValueError: incorrect length of params_values compared to program's input
+                parameter names.
+
+        Returns:
+            List[QueuedProgramRun]]
+        """
+        queued_runs: List[QueuedProgramRun] = []
+        input_parameter_names = program.input_parameter_names()
+
+        if not params_values:
+            if input_parameter_names:
+                raise ValueError(
+                    "Wrong parameters value: no parameters values provided but"
+                    f" input QuantumProgram has {len(input_parameter_names)}"
+                    " input parameter names."
+                )
+            queued_runs.append(self.run_measurement_queued(program.measurement()))
+        for params in params_values:
+            if len(params) != len(input_parameter_names):
+                raise ValueError(
+                    f"Wrong number of parameters {len(input_parameter_names)} parameters"
+                    f" expected {len(params)} parameters given."
+                )
+            substituted_parameters = dict(zip(input_parameter_names, params))
+            measurement = program.measurement().substitute_parameters(substituted_parameters)
+            queued_runs.append(self.run_measurement_queued(measurement))
+
+        return queued_runs
```

### Comparing `qoqo_qiskit-0.3.0/src/qoqo_qiskit/backend/post_processing.py` & `qoqo_qiskit-0.4.0/src/qoqo_qiskit/backend/post_processing.py`

 * *Files identical despite different names*

### Comparing `qoqo_qiskit-0.3.0/src/qoqo_qiskit/backend/queued_results.py` & `qoqo_qiskit-0.4.0/src/qoqo_qiskit/backend/queued_results.py`

 * *Files identical despite different names*

### Comparing `qoqo_qiskit-0.3.0/src/qoqo_qiskit/backend/utils.py` & `qoqo_qiskit-0.4.0/src/qoqo_qiskit/backend/utils.py`

 * *Files identical despite different names*

### Comparing `qoqo_qiskit-0.3.0/src/qoqo_qiskit/interface/__init__.py` & `qoqo_qiskit-0.4.0/src/qoqo_qiskit/interface/__init__.py`

 * *Files identical despite different names*

### Comparing `qoqo_qiskit-0.3.0/src/qoqo_qiskit/interface/interface.py` & `qoqo_qiskit-0.4.0/src/qoqo_qiskit/interface/interface.py`

 * *Files identical despite different names*

### Comparing `qoqo_qiskit-0.3.0/src/qoqo_qiskit.egg-info/PKG-INFO` & `qoqo_qiskit-0.4.0/src/qoqo_qiskit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qoqo_qiskit
-Version: 0.3.0
+Version: 0.4.0
 Author-email: HQS Quantum Simulation GmbH <info@quantumsimulations.de>
 Maintainer-email: Matteo Lodi <matteo.lodi@quantumsimulations.de>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `qoqo_qiskit-0.3.0/src/qoqo_qiskit.egg-info/SOURCES.txt` & `qoqo_qiskit-0.4.0/src/qoqo_qiskit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `qoqo_qiskit-0.3.0/tests/__init__.py` & `qoqo_qiskit-0.4.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `qoqo_qiskit-0.3.0/tests/backend/__init__.py` & `qoqo_qiskit-0.4.0/tests/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `qoqo_qiskit-0.3.0/tests/backend/test_queued_results.py` & `qoqo_qiskit-0.4.0/tests/backend/test_queued_results.py`

 * *Files identical despite different names*

### Comparing `qoqo_qiskit-0.3.0/tests/interface/__init__.py` & `qoqo_qiskit-0.4.0/tests/interface/__init__.py`

 * *Files identical despite different names*

### Comparing `qoqo_qiskit-0.3.0/tests/interface/test_interface.py` & `qoqo_qiskit-0.4.0/tests/interface/test_interface.py`

 * *Files identical despite different names*

