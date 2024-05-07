# Comparing `tmp/qiskit_braket_provider-0.2.0.tar.gz` & `tmp/qiskit_braket_provider-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qiskit_braket_provider-0.2.0.tar", last modified: Wed Mar  6 22:25:38 2024, max compression
+gzip compressed data, was "qiskit_braket_provider-0.3.1.tar", last modified: Tue May  7 20:16:20 2024, max compression
```

## Comparing `qiskit_braket_provider-0.2.0.tar` & `qiskit_braket_provider-0.3.1.tar`

### file list

```diff
@@ -1,31 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 22:25:38.987719 qiskit_braket_provider-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11416 2024-03-06 22:25:31.000000 qiskit_braket_provider-0.2.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3380 2024-03-06 22:25:38.987719 qiskit_braket_provider-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2466 2024-03-06 22:25:31.000000 qiskit_braket_provider-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 22:25:38.987719 qiskit_braket_provider-0.2.0/qiskit_braket_provider/
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-03-06 22:25:31.000000 qiskit_braket_provider-0.2.0/qiskit_braket_provider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-03-06 22:25:32.000000 qiskit_braket_provider-0.2.0/qiskit_braket_provider/exception.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 22:25:38.987719 qiskit_braket_provider-0.2.0/qiskit_braket_provider/providers/
--rw-r--r--   0 runner    (1001) docker     (127)      778 2024-03-06 22:25:32.000000 qiskit_braket_provider-0.2.0/qiskit_braket_provider/providers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22656 2024-03-06 22:25:32.000000 qiskit_braket_provider-0.2.0/qiskit_braket_provider/providers/adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)    13453 2024-03-06 22:25:32.000000 qiskit_braket_provider-0.2.0/qiskit_braket_provider/providers/braket_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)     7676 2024-03-06 22:25:32.000000 qiskit_braket_provider-0.2.0/qiskit_braket_provider/providers/braket_job.py
--rw-r--r--   0 runner    (1001) docker     (127)     2722 2024-03-06 22:25:32.000000 qiskit_braket_provider-0.2.0/qiskit_braket_provider/providers/braket_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-03-06 22:25:32.000000 qiskit_braket_provider-0.2.0/qiskit_braket_provider/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 22:25:38.987719 qiskit_braket_provider-0.2.0/qiskit_braket_provider.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3380 2024-03-06 22:25:38.000000 qiskit_braket_provider-0.2.0/qiskit_braket_provider.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      830 2024-03-06 22:25:38.000000 qiskit_braket_provider-0.2.0/qiskit_braket_provider.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-06 22:25:38.000000 qiskit_braket_provider-0.2.0/qiskit_braket_provider.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-03-06 22:25:38.000000 qiskit_braket_provider-0.2.0/qiskit_braket_provider.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-03-06 22:25:38.000000 qiskit_braket_provider-0.2.0/qiskit_braket_provider.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-03-06 22:25:38.991719 qiskit_braket_provider-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-03-06 22:25:32.000000 qiskit_braket_provider-0.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 22:25:38.987719 qiskit_braket_provider-0.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-06 22:25:32.000000 qiskit_braket_provider-0.2.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 22:25:38.987719 qiskit_braket_provider-0.2.0/tests/providers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-06 22:25:32.000000 qiskit_braket_provider-0.2.0/tests/providers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4922 2024-03-06 22:25:32.000000 qiskit_braket_provider-0.2.0/tests/providers/mocks.py
--rw-r--r--   0 runner    (1001) docker     (127)    22120 2024-03-06 22:25:32.000000 qiskit_braket_provider-0.2.0/tests/providers/test_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)    12065 2024-03-06 22:25:32.000000 qiskit_braket_provider-0.2.0/tests/providers/test_braket_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)     4368 2024-03-06 22:25:32.000000 qiskit_braket_provider-0.2.0/tests/providers/test_braket_job.py
--rw-r--r--   0 runner    (1001) docker     (127)     7076 2024-03-06 22:25:32.000000 qiskit_braket_provider-0.2.0/tests/providers/test_braket_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:16:20.148283 qiskit_braket_provider-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11416 2024-05-07 20:16:14.000000 qiskit_braket_provider-0.3.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3380 2024-05-07 20:16:20.152283 qiskit_braket_provider-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2466 2024-05-07 20:16:14.000000 qiskit_braket_provider-0.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:16:20.148283 qiskit_braket_provider-0.3.1/qiskit_braket_provider/
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-05-07 20:16:14.000000 qiskit_braket_provider-0.3.1/qiskit_braket_provider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-07 20:16:14.000000 qiskit_braket_provider-0.3.1/qiskit_braket_provider/exception.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:16:20.148283 qiskit_braket_provider-0.3.1/qiskit_braket_provider/providers/
+-rw-r--r--   0 runner    (1001) docker     (127)      829 2024-05-07 20:16:14.000000 qiskit_braket_provider-0.3.1/qiskit_braket_provider/providers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23041 2024-05-07 20:16:14.000000 qiskit_braket_provider-0.3.1/qiskit_braket_provider/providers/adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13449 2024-05-07 20:16:14.000000 qiskit_braket_provider-0.3.1/qiskit_braket_provider/providers/braket_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1907 2024-05-07 20:16:14.000000 qiskit_braket_provider-0.3.1/qiskit_braket_provider/providers/braket_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2690 2024-05-07 20:16:14.000000 qiskit_braket_provider-0.3.1/qiskit_braket_provider/providers/braket_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6873 2024-05-07 20:16:14.000000 qiskit_braket_provider-0.3.1/qiskit_braket_provider/providers/braket_quantum_task.py
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-07 20:16:14.000000 qiskit_braket_provider-0.3.1/qiskit_braket_provider/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:16:20.148283 qiskit_braket_provider-0.3.1/qiskit_braket_provider.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3380 2024-05-07 20:16:20.000000 qiskit_braket_provider-0.3.1/qiskit_braket_provider.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      895 2024-05-07 20:16:20.000000 qiskit_braket_provider-0.3.1/qiskit_braket_provider.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 20:16:20.000000 qiskit_braket_provider-0.3.1/qiskit_braket_provider.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-07 20:16:20.000000 qiskit_braket_provider-0.3.1/qiskit_braket_provider.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-07 20:16:20.000000 qiskit_braket_provider-0.3.1/qiskit_braket_provider.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-07 20:16:20.152283 qiskit_braket_provider-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1565 2024-05-07 20:16:14.000000 qiskit_braket_provider-0.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:16:20.148283 qiskit_braket_provider-0.3.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 20:16:14.000000 qiskit_braket_provider-0.3.1/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:16:20.148283 qiskit_braket_provider-0.3.1/tests/providers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 20:16:14.000000 qiskit_braket_provider-0.3.1/tests/providers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4922 2024-05-07 20:16:14.000000 qiskit_braket_provider-0.3.1/tests/providers/mocks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25457 2024-05-07 20:16:14.000000 qiskit_braket_provider-0.3.1/tests/providers/test_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12065 2024-05-07 20:16:14.000000 qiskit_braket_provider-0.3.1/tests/providers/test_braket_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7076 2024-05-07 20:16:14.000000 qiskit_braket_provider-0.3.1/tests/providers/test_braket_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5451 2024-05-07 20:16:14.000000 qiskit_braket_provider-0.3.1/tests/providers/test_braket_quantum_task.py
```

### Comparing `qiskit_braket_provider-0.2.0/LICENSE.txt` & `qiskit_braket_provider-0.3.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `qiskit_braket_provider-0.2.0/PKG-INFO` & `qiskit_braket_provider-0.3.1/qiskit_braket_provider.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: qiskit_braket_provider
-Version: 0.2.0
+Name: qiskit-braket-provider
+Version: 0.3.1
 Summary: Qiskit-Braket provider to execute Qiskit programs on AWS quantum computing hardware devices through Amazon Braket.
 Home-page: UNKNOWN
 License: UNKNOWN
 Keywords: qiskit braket sdk quantum
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
```

### Comparing `qiskit_braket_provider-0.2.0/README.md` & `qiskit_braket_provider-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `qiskit_braket_provider-0.2.0/qiskit_braket_provider/providers/__init__.py` & `qiskit_braket_provider-0.3.1/qiskit_braket_provider/providers/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -20,7 +20,8 @@
     AmazonBraketTask
 """
 
 from .adapter import to_braket, to_qiskit
 from .braket_backend import AWSBraketBackend, BraketAwsBackend, BraketLocalBackend
 from .braket_job import AmazonBraketTask, AWSBraketJob
 from .braket_provider import AWSBraketProvider, BraketProvider
+from .braket_quantum_task import BraketQuantumTask
```

### Comparing `qiskit_braket_provider-0.2.0/qiskit_braket_provider/providers/adapter.py` & `qiskit_braket_provider-0.3.1/qiskit_braket_provider/providers/adapter.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import qiskit.circuit.library as qiskit_gates
 from braket.aws import AwsDevice
 from braket.circuits import (
     Circuit,
     FreeParameter,
     FreeParameterExpression,
     Instruction,
-    observables,
+    measure,
 )
 from braket.device_schema import DeviceActionType, OpenQASMDeviceActionProperties
 from braket.device_schema.ionq import IonqDeviceCapabilities
 from braket.device_schema.oqc import OqcDeviceCapabilities
 from braket.device_schema.rigetti import RigettiDeviceCapabilities
 from braket.device_schema.simulators import GateModelSimulatorDeviceCapabilities
 from braket.devices import LocalSimulator
@@ -58,14 +58,15 @@
     "h": "h",
     "cy": "cy",
     "cz": "cz",
     "ccnot": "ccx",
     "cswap": "cswap",
     "cphaseshift": "cp",
     "ecr": "ecr",
+    "prx": "r",
     "gpi": "gpi",
     "gpi2": "gpi2",
     "ms": "ms",
     "gphase": _GPHASE_GATE_NAME,
 }
 
 _CONTROLLED_GATES_BY_QUBIT_COUNT = {
@@ -115,14 +116,15 @@
     "cz": lambda: [braket_gates.CZ()],
     "ccx": lambda: [braket_gates.CCNot()],
     "cswap": lambda: [braket_gates.CSwap()],
     "rxx": lambda angle: [braket_gates.XX(angle)],
     "ryy": lambda angle: [braket_gates.YY(angle)],
     "ecr": lambda: [braket_gates.ECR()],
     "iswap": lambda: [braket_gates.ISwap()],
+    "r": lambda angle_1, angle_2: [braket_gates.PRx(angle_1, angle_2)],
     # IonQ gates
     "gpi": lambda turns: [braket_gates.GPi(2 * pi * turns)],
     "gpi2": lambda turns: [braket_gates.GPi2(2 * pi * turns)],
     "ms": lambda turns_1, turns_2, turns_3: [
         braket_gates.MS(2 * pi * turns_1, 2 * pi * turns_2, 2 * pi * turns_3)
     ],
     "zz": lambda angle: [braket_gates.ZZ(2 * pi * angle)],
@@ -169,23 +171,25 @@
     "x": qiskit_gates.XGate(),
     "xx": qiskit_gates.RXXGate(Parameter("theta")),
     "y": qiskit_gates.YGate(),
     "yy": qiskit_gates.RYYGate(Parameter("theta")),
     "z": qiskit_gates.ZGate(),
     "zz": qiskit_gates.RZZGate(Parameter("theta")),
     "ecr": qiskit_gates.ECRGate(),
+    "prx": qiskit_gates.RGate(Parameter("theta"), Parameter("phi")),
     "iswap": qiskit_gates.iSwapGate(),
     "gpi": ionq_gates.GPIGate(Parameter("phi") / (2 * pi)),
     "gpi2": ionq_gates.GPI2Gate(Parameter("phi") / (2 * pi)),
     "ms": ionq_gates.MSGate(
         Parameter("phi0") / (2 * pi),
         Parameter("phi1") / (2 * pi),
         Parameter("theta") / (2 * pi),
     ),
     "gphase": qiskit_gates.GlobalPhaseGate(Parameter("theta")),
+    "measure": qiskit_gates.Measure(),
 }
 
 
 def gateset_from_properties(properties: OpenQASMDeviceActionProperties) -> set[str]:
     """Returns the gateset supported by a Braket device with the given properties
 
     Args:
@@ -428,20 +432,15 @@
         gate_name = operation.name
 
         qubits = circuit_instruction.qubits
 
         if gate_name == "measure":
             qubit = qubits[0]  # qubit count = 1 for measure
             qubit_index = circuit.find_bit(qubit).index
-            braket_circuit.sample(
-                observable=observables.Z(),
-                target=[
-                    qubit_index,
-                ],
-            )
+            braket_circuit.measure(qubit_index)
         elif gate_name == "barrier":
             warnings.warn(
                 "The Qiskit circuit contains barrier instructions that are ignored."
             )
         elif gate_name == "reset":
             raise NotImplementedError(
                 "reset operation not supported by qiskit to braket adapter"
@@ -527,22 +526,25 @@
 
     Returns:
         QuantumCircuit: Qiskit quantum circuit
     """
     if not isinstance(circuit, Circuit):
         raise TypeError(f"Expected a Circuit, got {type(circuit)} instead.")
 
-    qiskit_circuit = QuantumCircuit(circuit.qubit_count)
+    num_measurements = sum(
+        isinstance(instr.operator, measure.Measure) for instr in circuit.instructions
+    )
+    qiskit_circuit = QuantumCircuit(circuit.qubit_count, num_measurements)
     qubit_map = {
         int(qubit): index for index, qubit in enumerate(sorted(circuit.qubits))
     }
     dict_param = {}
+    cbit = 0
     for instruction in circuit.instructions:
         gate_name = instruction.operator.name.lower()
-
         gate_params = []
         if hasattr(instruction.operator, "parameters"):
             for value in instruction.operator.parameters:
                 if isinstance(value, FreeParameter):
                     if value.name not in dict_param:
                         dict_param[value.name] = Parameter(value.name)
                     gate_params.append(dict_param[value.name])
@@ -556,16 +558,21 @@
         if control_qubits := instruction.control:
             ctrl_state = instruction.control_state.as_string[::-1]
             gate = gate.control(len(control_qubits), ctrl_state=ctrl_state)
 
         target = [qiskit_circuit.qubits[qubit_map[i]] for i in control_qubits]
         target += [qiskit_circuit.qubits[qubit_map[i]] for i in instruction.target]
 
-        qiskit_circuit.append(gate, target)
-    qiskit_circuit.measure_all()
+        if gate_name == "measure":
+            qiskit_circuit.append(gate, target, [cbit])
+            cbit += 1
+        else:
+            qiskit_circuit.append(gate, target)
+    if num_measurements == 0:
+        qiskit_circuit.measure_all()
     return qiskit_circuit
 
 
 def _create_qiskit_gate(
     gate_name: str, gate_params: list[Union[float, Parameter]]
 ) -> Instruction:
     gate_instance = _GATE_NAME_TO_QISKIT_GATE.get(gate_name, None)
```

### Comparing `qiskit_braket_provider-0.2.0/qiskit_braket_provider/providers/braket_backend.py` & `qiskit_braket_provider-0.3.1/qiskit_braket_provider/providers/braket_backend.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 from ..exception import QiskitBraketException
 from .adapter import (
     aws_device_to_target,
     gateset_from_properties,
     local_simulator_to_target,
     to_braket,
 )
-from .braket_job import AmazonBraketTask
+from .braket_quantum_task import BraketQuantumTask
 
 logger = logging.getLogger(__name__)
 
 
 _TASK_ID_DIVIDER = ";"
 
 
@@ -57,22 +57,22 @@
         return gateset_from_properties(action) if action else None
 
 
 class BraketLocalBackend(BraketBackend):
     """BraketLocalBackend."""
 
     def __init__(self, name: str = "default", **fields):
-        """BraketLocalBackend for local execution of circuits.
+        """BraketLocalBackend for executing circuits locally.
 
         Example:
-            >>> device = LocalSimulator()                         #Local State Vector Simulator
-            >>> device = LocalSimulator("default")                #Local State Vector Simulator
-            >>> device = LocalSimulator(name="default")        #Local State Vector Simulator
-            >>> device = LocalSimulator(name="braket_sv")      #Local State Vector Simulator
-            >>> device = LocalSimulator(name="braket_dm")      #Local Density Matrix Simulator
+            >>> device = LocalSimulator()                    #Local State Vector Simulator
+            >>> device = LocalSimulator("default")           #Local State Vector Simulator
+            >>> device = LocalSimulator(name="default")      #Local State Vector Simulator
+            >>> device = LocalSimulator(name="braket_sv")    #Local State Vector Simulator
+            >>> device = LocalSimulator(name="braket_dm")    #Local Density Matrix Simulator
 
         Args:
             name: name of backend
             **fields: extra fields
         """
         super().__init__(name=name, **fields)
         self.backend_name = name
@@ -121,15 +121,15 @@
         raise NotImplementedError(f"Acquire channel is not supported by {self.name}.")
 
     def control_channel(self, qubits: Iterable[int]):
         raise NotImplementedError(f"Control channel is not supported by {self.name}.")
 
     def run(
         self, run_input: Union[QuantumCircuit, list[QuantumCircuit]], **options
-    ) -> AmazonBraketTask:
+    ) -> BraketQuantumTask:
         convert_input = (
             [run_input] if isinstance(run_input, QuantumCircuit) else list(run_input)
         )
         verbatim = options.pop("verbatim", False)
         gateset = self._get_gateset() if not verbatim else None
         circuits: list[Circuit] = [
             to_braket(circ, gateset, verbatim) for circ in convert_input
@@ -156,15 +156,15 @@
                 logger.error("Attempt to cancel %s...", task.id)
                 task.cancel()
                 logger.error("State of %s: %s.", task.id, task.state())
             raise ex
 
         task_id = _TASK_ID_DIVIDER.join(task.id for task in tasks)
 
-        return AmazonBraketTask(
+        return BraketQuantumTask(
             task_id=task_id,
             tasks=tasks,
             backend=self,
             shots=shots,
         )
 
 
@@ -179,15 +179,15 @@
         description: str = None,
         online_date: datetime.datetime = None,
         backend_version: str = None,
         *,
         device: Optional[AwsDevice] = None,
         **fields,
     ):
-        """BraketAwsBackend for execution circuits against AWS Braket devices.
+        """BraketAwsBackend for executing circuits on Amazon Braket devices.
 
         Example:
             >>> provider = BraketProvider()
             >>> backend = provider.get_backend("SV1")
             >>> transpiled_circuit = transpile(circuit, backend=backend)
             >>> backend.run(transpiled_circuit, shots=10).result().get_counts()
             {"100": 10, "001": 10}
@@ -216,26 +216,26 @@
         )
         self._aws_device = AwsDevice(arn) if arn else device
         self._aws_device.aws_session.add_braket_user_agent(
             f"QiskitBraketProvider/{version.__version__}"
         )
         self._target = aws_device_to_target(device=device)
 
-    def retrieve_job(self, task_id: str) -> AmazonBraketTask:
+    def retrieve_job(self, task_id: str) -> BraketQuantumTask:
         """Return a single job submitted to AWS backend.
 
         Args:
             task_id: ID of the task to retrieve.
 
         Returns:
             The job with the given ID.
         """
         task_ids = task_id.split(_TASK_ID_DIVIDER)
 
-        return AmazonBraketTask(
+        return BraketQuantumTask(
             task_id=task_id,
             backend=self,
             tasks=[AwsQuantumTask(arn=task_id) for task_id in task_ids],
         )
 
     @property
     def target(self):
@@ -332,15 +332,15 @@
 
         batch_task: AwsQuantumTaskBatch = self._device.run_batch(
             braket_circuits, **options
         )
         tasks: list[AwsQuantumTask] = batch_task.tasks
         task_id = _TASK_ID_DIVIDER.join(task.id for task in tasks)
 
-        return AmazonBraketTask(
+        return BraketQuantumTask(
             task_id=task_id, tasks=tasks, backend=self, shots=options.get("shots")
         )
 
 
 class AWSBraketBackend(BraketAwsBackend):
     """AWSBraketBackend."""
```

### Comparing `qiskit_braket_provider-0.2.0/qiskit_braket_provider/providers/braket_job.py` & `qiskit_braket_provider-0.3.1/qiskit_braket_provider/providers/braket_quantum_task.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,11 @@
-"""AWS Braket job."""
+"""Amazon Braket task."""
 
 from datetime import datetime
 from typing import List, Optional, Union
-from warnings import warn
 
 from braket.aws import AwsQuantumTask, AwsQuantumTaskBatch
 from braket.aws.queue_information import QuantumTaskQueueInfo
 from braket.tasks.local_quantum_task import LocalQuantumTask
 from qiskit.providers import BackendV2, JobStatus, JobV1
 from qiskit.quantum_info import Statevector
 from qiskit.result import Result
@@ -14,15 +13,15 @@
 
 
 def retry_if_result_none(result):
     """Retry on result function."""
     return result is None
 
 
-def _get_result_from_aws_tasks(
+def _get_result_from_tasks(
     tasks: Union[List[LocalQuantumTask], List[AwsQuantumTask]],
 ) -> Optional[List[ExperimentResult]]:
     """Returns experiment results of AWS tasks.
 
     Args:
         tasks: AWS Quantum tasks
         shots: number of shots
@@ -62,41 +61,43 @@
                     for shot_result in result.measurements
                 ],
             )
 
         experiment_result = ExperimentResult(
             shots=result.task_metadata.shots,
             success=True,
-            status=task.state()
-            if isinstance(task, LocalQuantumTask)
-            else result.task_metadata.status,
+            status=(
+                task.state()
+                if isinstance(task, LocalQuantumTask)
+                else result.task_metadata.status
+            ),
             data=data,
         )
         experiment_results.append(experiment_result)
 
     return experiment_results
 
 
-class AmazonBraketTask(JobV1):
-    """AmazonBraketTask."""
+class BraketQuantumTask(JobV1):
+    """BraketQuantumTask."""
 
     def __init__(
         self,
         task_id: str,
         backend: BackendV2,
         tasks: Union[List[LocalQuantumTask], List[AwsQuantumTask]],
         **metadata: Optional[dict],
     ):
-        """AmazonBraketTask for local execution of circuits.
+        """BraketQuantumTask for execution of circuits on Amazon Braket or locally.
 
         Args:
-            task_id: id of the task
-            backend: Local simulator
+            task_id: Semicolon-separated IDs of the underlying tasks
+            backend: BraketBackend that ran the circuit
             tasks: Executed tasks
-            **metadata:
+            **metadata: Additional metadata
         """
         super().__init__(backend=backend, job_id=task_id, metadata=metadata)
         self._task_id = task_id
         self._backend = backend
         self._metadata = metadata
         self._tasks = tasks
         self._date_of_creation = datetime.now()
@@ -154,15 +155,15 @@
             return AwsQuantumTask(self.task_id()).queue_position()
 
     def task_id(self) -> str:
         """Return a unique id identifying the task."""
         return self._task_id
 
     def result(self) -> Result:
-        experiment_results = _get_result_from_aws_tasks(tasks=self._tasks)
+        experiment_results = _get_result_from_tasks(tasks=self._tasks)
         status = self.status(use_cached_value=True)
 
         return Result(
             backend_name=self._backend,
             backend_version=self._backend.version,
             job_id=self._task_id,
             qobj_id=0,
@@ -173,17 +174,19 @@
 
     def cancel(self):
         for task in self._tasks:
             task.cancel()
 
     def status(self, use_cached_value: bool = False):
         braket_tasks_states = [
-            task.state()
-            if isinstance(task, LocalQuantumTask)
-            else task.state(use_cached_value=use_cached_value)
+            (
+                task.state()
+                if isinstance(task, LocalQuantumTask)
+                else task.state(use_cached_value=use_cached_value)
+            )
             for task in self._tasks
         ]
 
         if "FAILED" in braket_tasks_states:
             status = JobStatus.ERROR
         elif "CANCELLED" in braket_tasks_states:
             status = JobStatus.CANCELLED
@@ -191,36 +194,7 @@
             status = JobStatus.DONE
         elif all(state == "RUNNING" for state in braket_tasks_states):
             status = JobStatus.RUNNING
         else:
             status = JobStatus.QUEUED
 
         return status
-
-
-class AWSBraketJob(AmazonBraketTask):
-    """AWSBraketJob."""
-
-    def __init_subclass__(cls, **kwargs):
-        """This throws a deprecation warning on subclassing."""
-        warn(f"{cls.__name__} is deprecated.", DeprecationWarning, stacklevel=2)
-        super().__init_subclass__(**kwargs)
-
-    def __init__(
-        self,
-        job_id: str,
-        backend: BackendV2,
-        tasks: Union[List[LocalQuantumTask], List[AwsQuantumTask]],
-        **metadata: Optional[dict],
-    ):
-        """This throws a deprecation warning on initialization."""
-        warn(
-            f"{self.__class__.__name__} is deprecated.",
-            DeprecationWarning,
-            stacklevel=2,
-        )
-        super().__init__(task_id=job_id, backend=backend, tasks=tasks, **metadata)
-        self._job_id = job_id
-        self._backend = backend
-        self._metadata = metadata
-        self._tasks = tasks
-        self._date_of_creation = datetime.now()
```

### Comparing `qiskit_braket_provider-0.2.0/qiskit_braket_provider/providers/braket_provider.py` & `qiskit_braket_provider-0.3.1/qiskit_braket_provider/providers/braket_provider.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,33 +1,32 @@
-"""AWS Braket provider."""
+"""Amazon Braket provider."""
 
 import warnings
 
 from braket.aws import AwsDevice
 from braket.device_schema.dwave import DwaveDeviceCapabilities
 from braket.device_schema.quera import QueraDeviceCapabilities
 from braket.device_schema.xanadu import XanaduDeviceCapabilities
 from qiskit.providers import ProviderV1
 
 from .braket_backend import BraketAwsBackend, BraketLocalBackend
 
 
 class BraketProvider(ProviderV1):
-    """BraketProvider class for accessing AWS Braket backends.
+    """BraketProvider class for accessing Amazon Braket backends.
 
     Example:
         >>> provider = BraketProvider()
         >>> backends = provider.backends()
         >>> backends
-        [BraketBackend[Aspen-10],
-         BraketBackend[Aspen-11],
-         BraketBackend[Aspen-8],
-         BraketBackend[Aspen-9],
-         BraketBackend[Aspen-M-1],
-         BraketBackend[IonQ Device],
+        [BraketBackend[Aria 1],
+         BraketBackend[Aria 2],
+         BraketBackend[Aspen-M-3],
+         BraketBackend[Forte 1],
+         BraketBackend[Harmony],
          BraketBackend[Lucy],
          BraketBackend[SV1],
          BraketBackend[TN1],
          BraketBackend[dm1]]
     """
 
     def backends(self, name=None, **kwargs):
@@ -62,15 +61,15 @@
                 backend_version="2",
             )
             for device in supported_devices
         ]
 
 
 class AWSBraketProvider(BraketProvider):
-    """AWSBraketProvider class for accessing AWS Braket backends."""
+    """AWSBraketProvider class for accessing Amazon Braket backends."""
 
     def __init_subclass__(cls, **kwargs):
         """This throws a deprecation warning on subclassing."""
         warnings.warn(
             f"{cls.__name__} is deprecated.", DeprecationWarning, stacklevel=2
         )
         super().__init_subclass__(**kwargs)
```

### Comparing `qiskit_braket_provider-0.2.0/qiskit_braket_provider.egg-info/PKG-INFO` & `qiskit_braket_provider-0.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: qiskit-braket-provider
-Version: 0.2.0
+Name: qiskit_braket_provider
+Version: 0.3.1
 Summary: Qiskit-Braket provider to execute Qiskit programs on AWS quantum computing hardware devices through Amazon Braket.
 Home-page: UNKNOWN
 License: UNKNOWN
 Keywords: qiskit braket sdk quantum
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
```

### Comparing `qiskit_braket_provider-0.2.0/qiskit_braket_provider.egg-info/SOURCES.txt` & `qiskit_braket_provider-0.3.1/qiskit_braket_provider.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 qiskit_braket_provider.egg-info/requires.txt
 qiskit_braket_provider.egg-info/top_level.txt
 qiskit_braket_provider/providers/__init__.py
 qiskit_braket_provider/providers/adapter.py
 qiskit_braket_provider/providers/braket_backend.py
 qiskit_braket_provider/providers/braket_job.py
 qiskit_braket_provider/providers/braket_provider.py
+qiskit_braket_provider/providers/braket_quantum_task.py
 tests/__init__.py
 tests/providers/__init__.py
 tests/providers/mocks.py
 tests/providers/test_adapter.py
 tests/providers/test_braket_backend.py
-tests/providers/test_braket_job.py
-tests/providers/test_braket_provider.py
+tests/providers/test_braket_provider.py
+tests/providers/test_braket_quantum_task.py
```

### Comparing `qiskit_braket_provider-0.2.0/setup.py` & `qiskit_braket_provider-0.3.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Setup file for Qiskit-Braket provider."""
+
 import os
 from typing import Any, Dict, Optional
 
 import setuptools
 
 with open("README.md", encoding="utf-8") as f:
     long_description = f.read()
```

### Comparing `qiskit_braket_provider-0.2.0/tests/providers/mocks.py` & `qiskit_braket_provider-0.3.1/tests/providers/mocks.py`

 * *Files identical despite different names*

### Comparing `qiskit_braket_provider-0.2.0/tests/providers/test_adapter.py` & `qiskit_braket_provider-0.3.1/tests/providers/test_adapter.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """Tests for Qiskit to Braket adapter."""
 
 from unittest import TestCase
 from unittest.mock import Mock, patch
 
 import numpy as np
 import pytest
-from braket.circuits import Circuit, FreeParameter, Gate, Instruction, observables
-from braket.circuits.angled_gate import AngledGate, TripleAngledGate
+from braket.circuits import Circuit, FreeParameter, Gate, Instruction
+from braket.circuits.angled_gate import AngledGate, DoubleAngledGate, TripleAngledGate
 from qiskit import ClassicalRegister, QuantumCircuit, QuantumRegister
 from qiskit.circuit import Parameter, ParameterVector
 from qiskit.circuit.library import GlobalPhaseGate, PauliEvolutionGate
 from qiskit.circuit.library import standard_gates as qiskit_gates
 from qiskit.quantum_info import Operator, SparsePauliOp
 from qiskit_ionq import ionq_gates
 
@@ -218,14 +218,15 @@
             "sdg": "si",
             "sx": "v",
             "sxdg": "vi",
             "rzz": "zz",
             "id": "i",
             "ccx": "ccnot",
             "cp": "cphaseshift",
+            "r": "prx",
             "rxx": "xx",
             "ryy": "yy",
             "zz": "zz",
             "global_phase": "gphase",
         }
 
         qiskit_to_braket_gate_names |= {
@@ -252,21 +253,26 @@
                 "ecr",
                 "gpi",
                 "gpi2",
                 "ms",
             ]
         }
 
+        braket_to_qiskit_gate_names = {
+            **qiskit_to_braket_gate_names,
+            **{"measure": "measure"},
+        }
+
         self.assertEqual(
             set(qiskit_to_braket_gate_names.keys()),
             set(_GATE_NAME_TO_BRAKET_GATE.keys()),
         )
 
         self.assertEqual(
-            set(qiskit_to_braket_gate_names.values()),
+            set(braket_to_qiskit_gate_names.values()),
             set(_GATE_NAME_TO_QISKIT_GATE.keys()),
         )
 
     def test_type_error_on_bad_input(self):
         """Test raising TypeError if adapter does not receive a Qiskit QuantumCircuit."""
         circuit = Mock()
 
@@ -305,33 +311,30 @@
         with pytest.warns(UserWarning, match="contains barrier instructions"):
             braket_circuit = to_braket(qiskit_circuit)
 
         expected_braket_circuit = Circuit().x(0).x(1)
 
         self.assertEqual(braket_circuit, expected_braket_circuit)
 
-    def test_sample_result_type(self):
-        """Tests sample result type with observables Z"""
+    def test_measure(self):
+        """Tests the translation of a measure instruction"""
 
         qiskit_circuit = QuantumCircuit(2, 2)
         qiskit_circuit.h(0)
         qiskit_circuit.cx(0, 1)
         qiskit_circuit.measure(0, 0)
         braket_circuit = to_braket(qiskit_circuit)
 
         expected_braket_circuit = (
-            Circuit()  # pylint: disable=no-member
-            .h(0)
-            .cnot(0, 1)
-            .sample(observable=observables.Z(), target=0)
+            Circuit().h(0).cnot(0, 1).measure(0)  # pylint: disable=no-member
         )
 
         self.assertEqual(braket_circuit, expected_braket_circuit)
 
-    def test_sample_result_type_different_indices(self):
+    def test_measure_different_indices(self):
         """
         Tests the translation of a measure instruction.
 
         We test that the issue #132 has been fixed. The qubit index
         can be different from the classical bit index. The classical bit
         is ignored during the translation.
         """
@@ -339,18 +342,69 @@
         qiskit_circuit = QuantumCircuit(2, 2)
         qiskit_circuit.h(0)
         qiskit_circuit.cx(0, 1)
         qiskit_circuit.measure(0, 1)
         braket_circuit = to_braket(qiskit_circuit)
 
         expected_braket_circuit = (
+            Circuit().h(0).cnot(0, 1).measure(0)  # pylint: disable=no-member
+        )
+
+        self.assertEqual(braket_circuit, expected_braket_circuit)
+
+    def test_measure_subset_indices(self):
+        """
+        Tests the translation of a measure instruction on
+        a subset of qubits.
+        """
+
+        qiskit_circuit = QuantumCircuit(4, 2)
+        qiskit_circuit.h(0)
+        qiskit_circuit.cx(0, 1)
+        qiskit_circuit.cx(1, 2)
+        qiskit_circuit.cx(2, 3)
+        qiskit_circuit.measure(0, 0)
+        qiskit_circuit.measure(2, 1)
+        braket_circuit = to_braket(qiskit_circuit)
+
+        expected_braket_circuit = (
             Circuit()  # pylint: disable=no-member
             .h(0)
             .cnot(0, 1)
-            .sample(observable=observables.Z(), target=0)
+            .cnot(1, 2)
+            .cnot(2, 3)
+            .measure(0)
+            .measure(2)
+        )
+
+        self.assertEqual(braket_circuit, expected_braket_circuit)
+
+    def test_measure_all(self):
+        """
+        Tests the translation of a measure_all instruction
+        """
+
+        qiskit_circuit = QuantumCircuit(4, 2)
+        qiskit_circuit.h(0)
+        qiskit_circuit.cx(0, 1)
+        qiskit_circuit.cx(1, 2)
+        qiskit_circuit.cx(2, 3)
+        qiskit_circuit.measure_all()
+        braket_circuit = to_braket(qiskit_circuit)
+
+        expected_braket_circuit = (
+            Circuit()  # pylint: disable=no-member
+            .h(0)
+            .cnot(0, 1)
+            .cnot(1, 2)
+            .cnot(2, 3)
+            .measure(0)
+            .measure(1)
+            .measure(2)
+            .measure(3)
         )
 
         self.assertEqual(braket_circuit, expected_braket_circuit)
 
     def test_multiple_registers(self):
         """
         Tests the use of multiple registers.
@@ -369,16 +423,16 @@
         braket_circuit = to_braket(qiskit_circuit)
 
         expected_braket_circuit = (
             Circuit()  # pylint: disable=no-member
             .h(0)
             .cnot(0, 2)
             .x(1)
-            .sample(observable=observables.Z(), target=0)
-            .sample(observable=observables.Z(), target=2)
+            .measure(0)
+            .measure(2)
         )
         self.assertEqual(braket_circuit, expected_braket_circuit)
 
     def test_verbatim(self):
         """Tests that transpilation is skipped for verbatim circuits."""
         qiskit_circuit = QuantumCircuit(2)
         qiskit_circuit.h(0)
@@ -489,30 +543,34 @@
         ]
 
         for gate_name in gate_set:
             for params_braket in param_sets:
                 gate = getattr(Gate, gate_name)
                 if issubclass(gate, AngledGate):
                     op = gate(params_braket[0])
+                elif issubclass(gate, DoubleAngledGate):
+                    op = gate(params_braket[0], params_braket[1])
                 elif issubclass(gate, TripleAngledGate):
                     op = gate(*params_braket)
                 else:
                     op = gate()
                 target = range(op.qubit_count)
                 instr = Instruction(op, target)
 
                 braket_circuit = Circuit().add_instruction(instr)
                 qiskit_circuit = to_qiskit(braket_circuit)
                 param_uuids = {
                     param.name: param._uuid for param in qiskit_circuit.parameters
                 }
                 params_qiskit = [
-                    Parameter(param.name, uuid=param_uuids.get(param.name))
-                    if isinstance(param, FreeParameter)
-                    else param
+                    (
+                        Parameter(param.name, uuid=param_uuids.get(param.name))
+                        if isinstance(param, FreeParameter)
+                        else param
+                    )
                     for param in params_braket
                 ]
 
                 expected_qiskit_circuit = QuantumCircuit(op.qubit_count)
                 qiskit_gate = _GATE_NAME_TO_QISKIT_GATE.get(gate_name.lower())
                 expected_qiskit_circuit.append(qiskit_gate, target)
                 expected_qiskit_circuit.measure_all()
@@ -594,7 +652,53 @@
 
         expected_qiskit_circuit = QuantumCircuit(1)
         sx = qiskit_gates.XGate().power(0.5)
         expected_qiskit_circuit.append(sx, [0])
         expected_qiskit_circuit.measure_all()
 
         self.assertEqual(qiskit_circuit, expected_qiskit_circuit)
+
+    def test_measure_subset(self):
+        """Tests the measure instruction conversion from braket to qiskit"""
+        braket_circuit = Circuit().h(0).cnot(0, 1).measure(0)
+        qiskit_circuit = to_qiskit(braket_circuit)
+
+        expected_qiskit_circuit = QuantumCircuit(2, 1)
+        expected_qiskit_circuit.h(0)
+        expected_qiskit_circuit.cx(0, 1)
+        expected_qiskit_circuit.measure(0, 0)
+
+        self.assertEqual(qiskit_circuit, expected_qiskit_circuit)
+
+    def test_measure_multiple_indices(self):
+        """
+        Tests the measure instruction conversion with multiple
+        indices in the braket measure target.
+        """
+        braket_circuit = Circuit().h(0).cnot(0, 1).cnot(1, 2).measure([0, 1, 2])
+        qiskit_circuit = to_qiskit(braket_circuit)
+
+        expected_qiskit_circuit = QuantumCircuit(3, 3)
+        expected_qiskit_circuit.h(0)
+        expected_qiskit_circuit.cx(0, 1)
+        expected_qiskit_circuit.cx(1, 2)
+        expected_qiskit_circuit.measure(0, 0)
+        expected_qiskit_circuit.measure(1, 1)
+        expected_qiskit_circuit.measure(2, 2)
+
+        self.assertEqual(qiskit_circuit, expected_qiskit_circuit)
+
+    def test_measure_different_indices(self):
+        """
+        Tests the measure instruction conversion from with
+        the ordering of the targets unsorted.
+        """
+        braket_circuit = Circuit().h(0).cnot(0, 1).measure([1, 0])
+        qiskit_circuit = to_qiskit(braket_circuit)
+
+        expected_qiskit_circuit = QuantumCircuit(2, 2)
+        expected_qiskit_circuit.h(0)
+        expected_qiskit_circuit.cx(0, 1)
+        expected_qiskit_circuit.measure(1, 0)
+        expected_qiskit_circuit.measure(0, 1)
+
+        self.assertEqual(qiskit_circuit, expected_qiskit_circuit)
```

### Comparing `qiskit_braket_provider-0.2.0/tests/providers/test_braket_backend.py` & `qiskit_braket_provider-0.3.1/tests/providers/test_braket_backend.py`

 * *Files identical despite different names*

### Comparing `qiskit_braket_provider-0.2.0/tests/providers/test_braket_job.py` & `qiskit_braket_provider-0.3.1/tests/providers/test_braket_quantum_task.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,18 +7,63 @@
 from braket.aws.aws_quantum_task import AwsQuantumTask
 from qiskit.providers import JobStatus
 
 from qiskit_braket_provider.providers import (
     AmazonBraketTask,
     AWSBraketJob,
     BraketLocalBackend,
+    BraketQuantumTask,
 )
 from tests.providers.mocks import MOCK_LOCAL_QUANTUM_TASK
 
 
+class TestBraketTask(TestCase):
+    """Tests BraketTask."""
+
+    def _get_task(self):
+        return BraketQuantumTask(
+            backend=BraketLocalBackend(name="default"),
+            task_id="AwesomeId",
+            tasks=[MOCK_LOCAL_QUANTUM_TASK],
+            shots=10,
+        )
+
+    def test_task(self):
+        """Tests task."""
+        task = self._get_task()
+
+        self.assertTrue(isinstance(task, BraketQuantumTask))
+        self.assertEqual(task.shots, 10)
+
+        self.assertEqual(task.status(), JobStatus.DONE)
+
+    def test_result(self):
+        """Tests result."""
+        task = self._get_task()
+
+        self.assertEqual(task.result().job_id, "AwesomeId")
+        self.assertEqual(task.result().results[0].data.counts, {"01": 1, "10": 2})
+        self.assertEqual(task.result().results[0].data.memory, ["10", "10", "01"])
+        self.assertEqual(task.result().results[0].status, "COMPLETED")
+        self.assertEqual(task.result().results[0].shots, 3)
+        self.assertEqual(task.result().get_memory(), ["10", "10", "01"])
+
+    def test_queue_position_for_local_quantum_task(self):
+        """Tests job status when multiple task status is present."""
+        task = BraketQuantumTask(
+            backend=BraketLocalBackend(name="default"),
+            task_id="MockId",
+            tasks=[MOCK_LOCAL_QUANTUM_TASK],
+            shots=100,
+        )
+        message = "We don't provide queue information for the LocalQuantumTask."
+        with pytest.raises(NotImplementedError, match=message):
+            task.queue_position()
+
+
 class TestAmazonBraketTask(TestCase):
     """Tests AmazonBraketTask."""
 
     def _get_task(self):
         return AmazonBraketTask(
             backend=BraketLocalBackend(name="default"),
             task_id="AwesomeId",
@@ -75,26 +120,14 @@
         self.assertEqual(job.result().job_id, "AwesomeId")
         self.assertEqual(job.result().results[0].data.counts, {"01": 1, "10": 2})
         self.assertEqual(job.result().results[0].data.memory, ["10", "10", "01"])
         self.assertEqual(job.result().results[0].status, "COMPLETED")
         self.assertEqual(job.result().results[0].shots, 3)
         self.assertEqual(job.result().get_memory(), ["10", "10", "01"])
 
-    def test_queue_position_for_local_quantum_task(self):
-        """Tests job status when multiple task status is present."""
-        job = AWSBraketJob(
-            backend=BraketLocalBackend(name="default"),
-            job_id="MockId",
-            tasks=[MOCK_LOCAL_QUANTUM_TASK],
-            shots=100,
-        )
-        message = "We don't provide queue information for the LocalQuantumTask."
-        with pytest.raises(NotImplementedError, match=message):
-            job.queue_position()
-
 
 class TestBraketJobStatus:
     """Tests for Amazon Braket job status."""
 
     def _get_mock_aws_quantum_task(self, status: str) -> AwsQuantumTask:
         """
         Creates a mock AwsQuantumTask with the given status.
@@ -119,11 +152,11 @@
         """Tests job status when multiple task status is present."""
         job = AWSBraketJob(
             backend=BraketLocalBackend(name="default"),
             job_id="MockId",
             tasks=[MOCK_LOCAL_QUANTUM_TASK],
             shots=100,
         )
-        job._tasks = Mock(spec=AmazonBraketTask)
+        job._tasks = Mock(spec=BraketQuantumTask)
         job._tasks = [self._get_mock_aws_quantum_task(state) for state in task_states]
 
         assert job.status() == expected_status
```

### Comparing `qiskit_braket_provider-0.2.0/tests/providers/test_braket_provider.py` & `qiskit_braket_provider-0.3.1/tests/providers/test_braket_provider.py`

 * *Files identical despite different names*

