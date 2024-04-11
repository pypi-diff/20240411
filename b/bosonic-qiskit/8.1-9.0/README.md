# Comparing `tmp/bosonic-qiskit-8.1.tar.gz` & `tmp/bosonic-qiskit-9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bosonic-qiskit-8.1.tar", last modified: Thu Apr 20 20:03:55 2023, max compression
+gzip compressed data, was "bosonic-qiskit-9.0.tar", last modified: Wed Aug  9 14:18:37 2023, max compression
```

## Comparing `bosonic-qiskit-8.1.tar` & `bosonic-qiskit-9.0.tar`

### file list

```diff
@@ -1,35 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 20:03:55.482550 bosonic-qiskit-8.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-04-20 20:03:39.000000 bosonic-qiskit-8.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-04-20 20:03:55.482550 bosonic-qiskit-8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-04-20 20:03:39.000000 bosonic-qiskit-8.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 20:03:55.478551 bosonic-qiskit-8.1/bosonic_qiskit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-04-20 20:03:55.000000 bosonic-qiskit-8.1/bosonic_qiskit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-04-20 20:03:55.000000 bosonic-qiskit-8.1/bosonic_qiskit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 20:03:55.000000 bosonic-qiskit-8.1/bosonic_qiskit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-20 20:03:55.000000 bosonic-qiskit-8.1/bosonic_qiskit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-20 20:03:55.000000 bosonic-qiskit-8.1/bosonic_qiskit.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 20:03:55.482550 bosonic-qiskit-8.1/c2qa/
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-04-20 20:03:39.000000 bosonic-qiskit-8.1/c2qa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15116 2023-04-20 20:03:39.000000 bosonic-qiskit-8.1/c2qa/animate.py
--rw-r--r--   0 runner    (1001) docker     (123)    27351 2023-04-20 20:03:39.000000 bosonic-qiskit-8.1/c2qa/circuit.py
--rw-r--r--   0 runner    (1001) docker     (123)     7824 2023-04-20 20:03:39.000000 bosonic-qiskit-8.1/c2qa/kraus.py
--rw-r--r--   0 runner    (1001) docker     (123)    12160 2023-04-20 20:03:39.000000 bosonic-qiskit-8.1/c2qa/operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     5626 2023-04-20 20:03:39.000000 bosonic-qiskit-8.1/c2qa/parameterized_unitary_gate.py
--rw-r--r--   0 runner    (1001) docker     (123)     3149 2023-04-20 20:03:39.000000 bosonic-qiskit-8.1/c2qa/qumoderegister.py
--rw-r--r--   0 runner    (1001) docker     (123)    17533 2023-04-20 20:03:39.000000 bosonic-qiskit-8.1/c2qa/util.py
--rw-r--r--   0 runner    (1001) docker     (123)    12720 2023-04-20 20:03:39.000000 bosonic-qiskit-8.1/c2qa/wigner.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 20:03:55.482550 bosonic-qiskit-8.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-04-20 20:03:39.000000 bosonic-qiskit-8.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 20:03:55.482550 bosonic-qiskit-8.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-20 20:03:39.000000 bosonic-qiskit-8.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6761 2023-04-20 20:03:39.000000 bosonic-qiskit-8.1/tests/test_animate.py
--rw-r--r--   0 runner    (1001) docker     (123)     4299 2023-04-20 20:03:39.000000 bosonic-qiskit-8.1/tests/test_circuit.py
--rw-r--r--   0 runner    (1001) docker     (123)    10010 2023-04-20 20:03:39.000000 bosonic-qiskit-8.1/tests/test_gates.py
--rw-r--r--   0 runner    (1001) docker     (123)     2849 2023-04-20 20:03:39.000000 bosonic-qiskit-8.1/tests/test_inconsistent_statevectors.py
--rw-r--r--   0 runner    (1001) docker     (123)    21472 2023-04-20 20:03:39.000000 bosonic-qiskit-8.1/tests/test_noise_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3691 2023-04-20 20:03:39.000000 bosonic-qiskit-8.1/tests/test_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     2765 2023-04-20 20:03:39.000000 bosonic-qiskit-8.1/tests/test_parameterized.py
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-20 20:03:39.000000 bosonic-qiskit-8.1/tests/test_qiskit.py
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-04-20 20:03:39.000000 bosonic-qiskit-8.1/tests/test_qumoderegister.py
--rw-r--r--   0 runner    (1001) docker     (123)     4688 2023-04-20 20:03:39.000000 bosonic-qiskit-8.1/tests/test_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     5605 2023-04-20 20:03:39.000000 bosonic-qiskit-8.1/tests/test_wigner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 14:18:37.365499 bosonic-qiskit-9.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-08-09 14:18:23.000000 bosonic-qiskit-9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-08-09 14:18:37.365499 bosonic-qiskit-9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-08-09 14:18:23.000000 bosonic-qiskit-9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 14:18:37.353500 bosonic-qiskit-9.0/bosonic_qiskit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-08-09 14:18:37.000000 bosonic-qiskit-9.0/bosonic_qiskit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-08-09 14:18:37.000000 bosonic-qiskit-9.0/bosonic_qiskit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-09 14:18:37.000000 bosonic-qiskit-9.0/bosonic_qiskit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-08-09 14:18:37.000000 bosonic-qiskit-9.0/bosonic_qiskit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-08-09 14:18:37.000000 bosonic-qiskit-9.0/bosonic_qiskit.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 14:18:37.357499 bosonic-qiskit-9.0/c2qa/
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-08-09 14:18:23.000000 bosonic-qiskit-9.0/c2qa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10598 2023-08-09 14:18:23.000000 bosonic-qiskit-9.0/c2qa/animate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33194 2023-08-09 14:18:23.000000 bosonic-qiskit-9.0/c2qa/circuit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12334 2023-08-09 14:18:23.000000 bosonic-qiskit-9.0/c2qa/discretize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8118 2023-08-09 14:18:23.000000 bosonic-qiskit-9.0/c2qa/kraus.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14004 2023-08-09 14:18:23.000000 bosonic-qiskit-9.0/c2qa/operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6531 2023-08-09 14:18:23.000000 bosonic-qiskit-9.0/c2qa/parameterized_unitary_gate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3345 2023-08-09 14:18:23.000000 bosonic-qiskit-9.0/c2qa/qumoderegister.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29707 2023-08-09 14:18:23.000000 bosonic-qiskit-9.0/c2qa/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13775 2023-08-09 14:18:23.000000 bosonic-qiskit-9.0/c2qa/wigner.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-09 14:18:37.365499 bosonic-qiskit-9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-08-09 14:18:23.000000 bosonic-qiskit-9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-09 14:18:37.365499 bosonic-qiskit-9.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-08-09 14:18:23.000000 bosonic-qiskit-9.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6761 2023-08-09 14:18:23.000000 bosonic-qiskit-9.0/tests/test_animate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8691 2023-08-09 14:18:23.000000 bosonic-qiskit-9.0/tests/test_circuit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8342 2023-08-09 14:18:23.000000 bosonic-qiskit-9.0/tests/test_discretize.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10456 2023-08-09 14:18:23.000000 bosonic-qiskit-9.0/tests/test_gates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2849 2023-08-09 14:18:23.000000 bosonic-qiskit-9.0/tests/test_inconsistent_statevectors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22539 2023-08-09 14:18:23.000000 bosonic-qiskit-9.0/tests/test_noise_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3691 2023-08-09 14:18:23.000000 bosonic-qiskit-9.0/tests/test_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2778 2023-08-09 14:18:23.000000 bosonic-qiskit-9.0/tests/test_parameterized.py
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-08-09 14:18:23.000000 bosonic-qiskit-9.0/tests/test_qiskit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-08-09 14:18:23.000000 bosonic-qiskit-9.0/tests/test_qumoderegister.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11294 2023-08-09 14:18:23.000000 bosonic-qiskit-9.0/tests/test_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5683 2023-08-09 14:18:23.000000 bosonic-qiskit-9.0/tests/test_wigner.py
```

### Comparing `bosonic-qiskit-8.1/LICENSE` & `bosonic-qiskit-9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bosonic-qiskit-8.1/README.md` & `bosonic-qiskit-9.0/README.md`

 * *Files identical despite different names*

### Comparing `bosonic-qiskit-8.1/bosonic_qiskit.egg-info/SOURCES.txt` & `bosonic-qiskit-9.0/bosonic_qiskit.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -5,23 +5,25 @@
 bosonic_qiskit.egg-info/SOURCES.txt
 bosonic_qiskit.egg-info/dependency_links.txt
 bosonic_qiskit.egg-info/requires.txt
 bosonic_qiskit.egg-info/top_level.txt
 c2qa/__init__.py
 c2qa/animate.py
 c2qa/circuit.py
+c2qa/discretize.py
 c2qa/kraus.py
 c2qa/operators.py
 c2qa/parameterized_unitary_gate.py
 c2qa/qumoderegister.py
 c2qa/util.py
 c2qa/wigner.py
 tests/__init__.py
 tests/test_animate.py
 tests/test_circuit.py
+tests/test_discretize.py
 tests/test_gates.py
 tests/test_inconsistent_statevectors.py
 tests/test_noise_model.py
 tests/test_operators.py
 tests/test_parameterized.py
 tests/test_qiskit.py
 tests/test_qumoderegister.py
```

### Comparing `bosonic-qiskit-8.1/c2qa/circuit.py` & `bosonic-qiskit-9.0/c2qa/circuit.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import copy
 import warnings
 
 import numpy as np
 from qiskit import QuantumCircuit, QuantumRegister
 from qiskit.circuit.parametertable import ParameterTable
+from qiskit.quantum_info.operators.predicates import is_unitary_matrix
 import qiskit.providers.aer.library.save_instructions as save
 
 from c2qa.operators import CVOperators
 from c2qa.parameterized_unitary_gate import ParameterizedUnitaryGate
 from c2qa.qumoderegister import QumodeRegister
 
 
@@ -105,14 +106,18 @@
         self._calibrations = copy.deepcopy(circuit._calibrations)
         self._metadata = copy.deepcopy(circuit._metadata)
 
     @property
     def cutoff(self):
         """Integer cutoff size."""
         return self.qmregs[-1].cutoff
+    
+    def qumode_cutoff(self, qumode_index:int):
+        """Return the qumode cutoff at the given index"""
+        return self.qmregs[qumode_index].cutoff
 
     @property
     def num_qubits_per_qumode(self):
         """Integer number of qubits to represent a qumode."""
         return self.qmregs[-1].num_qubits_per_qumode
 
     @property
@@ -131,14 +136,40 @@
 
         for index, qubit in enumerate(self.qubits):
             if qubit in qmodes:
                 indices.append(index)
 
         return indices
 
+    @property
+    def qumode_qubits_indices_grouped(self):
+        """Same as qumode_qubit_indices but it groups qubits representing the same qumode together. Returns a nested list."""
+        grouped_indices = []
+    
+        # Iterate through all qmregs
+        for _, qmreg in enumerate(self.qmregs):
+            num_qumodes_in_reg = qmreg.num_qumodes
+            num_qubits_per_qumode = qmreg.num_qubits_per_qumode
+
+            qmreg_qubit_indices = []
+
+            # For every qubit in circuit, append index of qubit to list if qubit is in qmreg
+            for qubit_index, qubit in enumerate(self.qubits): 
+                if qubit in qmreg[:]:
+                    qmreg_qubit_indices.append(qubit_index)
+
+            # Split list according to no. of qumodes in qmreg
+            qmreg_qubit_indices = [qmreg_qubit_indices[i * num_qubits_per_qumode: (i + 1) * num_qubits_per_qumode] for i in range(num_qumodes_in_reg)]
+
+            # Extend final list
+            grouped_indices.extend(qmreg_qubit_indices) 
+
+        return(grouped_indices)        
+         
+
     def get_qubit_index(self, qubit):
         """Return the index of the given Qubit"""
         for i, q in enumerate(self.qubits):
             if q == qubit:
                 return i
         return None
 
@@ -152,14 +183,21 @@
                 flat_list += [el]
        
         indices = []
         for i, q in enumerate(self.qubits):
             if q in flat_list:
                 indices.append(i)
         return indices
+    
+    def get_qubit_qumode_index(self, qubit):
+        """Return the qumode index for the given qubit. If not found, return -1."""
+        for index, qmr in enumerate(self.qmregs):
+            if qubit in qmr:
+                return index
+        raise ValueError(f"Bit {qubit} not found in circuit.")
 
     @property
     def cv_gate_labels(self):
         """
         All the CV gate names on the current circuit. These will either be
         instances of ParameterizedUnitaryGate or be instances of super
         Intstruction and flagged with 'cv_conditional' if a conditional gate.
@@ -208,29 +246,33 @@
         # Qumodes are already represented as arrays of qubits,
         # but if this is an array of arrays, then we are initializing multiple qumodes.
         modes = qumodes
         if not isinstance(qumodes[0], list):
             modes = [qumodes]
 
         if isinstance(params, int):
-            if params >= self.qmregs[-1].cutoff:
-                raise ValueError("The given Fock state is greater than the cutoff.")
-
             for qumode in modes:
-                value = np.zeros((self.qmregs[-1].cutoff,), dtype=np.complex_)
+                qumode_index = self.get_qubit_qumode_index(qumode[0])
+
+                if params >= self.qumode_cutoff(qumode_index):
+                    raise ValueError("The given Fock state is greater than the cutoff.")
+
+                value = np.zeros((self.qumode_cutoff(qumode_index),), dtype=np.complex_)
                 value[params] = 1 + 0j
 
                 super().initialize(value, qumode)
         else:
-            if len(params) > self.qmregs[-1].cutoff:
-                raise ValueError("len(params) exceeds the cutoff.")
-
             for qumode in modes:
+                qumode_index = self.get_qubit_qumode_index(qumode[0])
+
+                if len(params) > self.qumode_cutoff(qumode_index):
+                    raise ValueError("len(params) exceeds the cutoff.")
+
                 params = np.array(params) / np.linalg.norm(np.array(params))
-                amplitudes = np.zeros((self.qmregs[-1].cutoff,), dtype=np.complex_)
+                amplitudes = np.zeros((self.qumode_cutoff(qumode_index),), dtype=np.complex_)
                 for ind in range(len(params)):
                     amplitudes[ind] = complex(params[ind])
 
                 super().initialize(amplitudes, qumode)
 
     @staticmethod
     def cv_conditional(
@@ -508,15 +550,15 @@
                 duration=duration,
                 unit=unit
             ),
             qargs=qumode_a + qumode_b + [qubit],
         )
 
     def cv_c_schwinger(self, params, qumode_a, qumode_b, qubit, duration=100, unit="ns"):
-        """General form of a controlled Schwinger gate, containing both the controlled phase beamsplitter
+        """General form of a controlled 'Schwinger' gate, containing both the controlled phase beamsplitter
         and pairs of controlled phase space rotations as special cases.
 
         It has the form exp(-i*beta*(n1_hat.sigma)(n2_hat.S)),
         where ni_hat = sin(theta_i)*cos(phi_i) + sin(theta_i)*sin(phi_i) + cos(theta_i).
         sigma = [sigmax, sigmay, sigmaz] is the vector of Pauli operators, and
         S = [Sx, Sy, Sz] is a vector of Schwinger boson operators,
 
@@ -538,68 +580,97 @@
         self.append(
             ParameterizedUnitaryGate(
                 self.ops.cschwinger,
                 params,
                 num_qubits=len(qumode_a) + len(qumode_b) + 1,
                 label="cSchw",
                 duration=duration,
-                unit=unit
+                unit=unit,
+                discretized_param_indices=[0]
             ),
             qargs=qumode_a + qumode_b + [qubit],
         )
 
     def cv_snap(self, theta, n, qumode, qubit=None, duration=100, unit="ns"):
-        """SNAP (Selective Number-dependent Arbitrary Phase) gate.
-        TODO: Add second snap implementation that includes sigma_z qubit
+        """SNAP (Selective Number-dependent Arbitrary Phase) gate. If no qubit is passed,
+        then phases are applied to each qumode Fock state specified in theta and n (without
+        explicit rotation of the qubit). If a qubit is passed, the phase will be multiplied by
+        sigma_z-dependent geometric phase (akin to the implementation of the SNAP gate
+        as described in Heeres et al, PRL (2015).
 
         Args:
-            theta (real): phase
-            n (integer): Fock state in which the mode should acquire the phase
+            theta (real or list[real]): phase
+            n (integer or list[integer]): Fock state in which the mode should acquire the phase
             qumode (list): list of qubits representing qumode
             qubit (Qubit): control qubit. If no qubit is passed, the gate will implement for sigma^z = +1.
 
         Returns:
             Instruction: QisKit instruction
         """
-        if qubit is None:
-            self.append(
-                ParameterizedUnitaryGate(
-                    self.ops.snap, [theta, n], num_qubits=len(qumode), label="SNAP", duration=duration, unit=unit
-                ),
-                qargs=qumode,
-            )
+        if isinstance(n,int):
+            if n > self.cutoff:
+                ValueError("Fock state specified by n exceeds the cutoff.")
+            if qubit is None:
+                self.append(
+                    ParameterizedUnitaryGate(
+                        self.ops.snap, [theta, n], num_qubits=len(qumode), label="SNAP", duration=duration, unit=unit
+                    ),
+                    qargs=qumode,
+                )
+            else:
+                self.append(
+                    ParameterizedUnitaryGate(
+                        self.ops.csnap, [theta, n], num_qubits=len(qumode) + 1, label="cSNAP", duration=duration, unit=unit
+                    ),
+                    qargs=qumode + [qubit],
+                )
+        elif isinstance(n,list) and isinstance(theta,list):
+            if qubit is None:
+                self.append(
+                    ParameterizedUnitaryGate(
+                        self.ops.multisnap, theta + n, num_qubits=len(qumode), label="SNAP", duration=duration, unit=unit
+                    ),
+                    qargs=qumode,
+                )
+            else:
+                self.append(
+                    ParameterizedUnitaryGate(
+                        self.ops.multicsnap, theta + n, num_qubits=len(qumode) + 1, label="cSNAP", duration=duration, unit=unit
+                    ),
+                    qargs=qumode + [qubit],
+                )
         else:
-            self.append(
-                ParameterizedUnitaryGate(
-                    self.ops.csnap, [theta, n], num_qubits=len(qumode) + 1, label="cSNAP", duration=duration, unit=unit
-                ),
-                qargs=qumode + [qubit],
-            )
+            raise ValueError("if theta is passed as a list, then n must also be a list of equal length (and vice versa).")
+
+
+    # def cv_c_sqr(self, theta, n, qumode, qubit, duration=100, unit="ns"):
+    #     """TODO"""
+
             
-    def cv_multisnap(self, thetas, ns, qumode, duration=1, unit="us"):
-        params = thetas + ns
-        self.append(
-            ParameterizedUnitaryGate(
-                self.ops.multisnap, params, num_qubits=len(qumode), label="mSNAP", duration=duration, unit=unit
-            ),
-            qargs=qumode,
-        )
+    # def cv_multisnap(self, thetas, ns, qumode, duration=1, unit="us"):
+    #     params = thetas + ns
+    #     self.append(
+    #         ParameterizedUnitaryGate(
+    #             self.ops.multisnap, params, num_qubits=len(qumode), label="mSNAP", duration=duration, unit=unit
+    #         ),
+    #         qargs=qumode,
+    #     )
             
-    def cv_c_multiboson_sampling(self, max, qumode, qubit=None, duration=1, unit="us"):
-        """SNAP (Selective Number-dependent Arbitrary Phase) gates for multiboson sampling.
+    def cv_c_pnr(self, max, qumode, qubit, duration=100, unit="ns"):
+        """ PNR (Photon number readout) TODO: Needs comments/explanation/citation!
         Args:
             max (int): the period of the mapping
             qumode (list): list of qubits representing qumode
             qubit (Qubit): control qubit.
         Returns:
             Instruction: QisKit instruction
         """
         self.append(
             ParameterizedUnitaryGate(
-                self.ops.c_multiboson_sampling, [max], num_qubits=len(qumode) + 1, label="c_multiboson_sampling", duration=duration, unit=unit
+                self.ops.pnr, [max], num_qubits=len(qumode) + 1, label="c_pnr", duration=duration, unit=unit
             ),
             qargs=qumode + [qubit],
         )
 
     def cv_eswap(self, theta, qumode_a, qumode_b, duration=100, unit="ns"):
         """Exponential SWAP gate.
 
@@ -719,19 +790,14 @@
                 If len(cbit_list) is greater than the required number of
                 classical bits, excess will be ignored. If len(cbit_list) is
                 insufficient, an error will be thrown.
 
         Returns:
             Instruction: QisKit measure instruction
         """
-        if not self.probe_measure:
-            warnings.warn(
-                "Probe qubits not in use, set probe_measure to True for measure support.",
-                UserWarning,
-            )
 
         # Flattens the list (if necessary)
         flat_list = []
         for el in qubit_qumode_list:
             if isinstance(el, list):
                 flat_list += el
             else:
@@ -742,14 +808,32 @@
         # This piece is useful so that the user doesn't need to think about
         # how many bits are needed to read out a list of qumodes, qubits, etc.
         if len(flat_list) < len(cbit_list):
             self.measure(flat_list, cbit_list[0:len(flat_list)])
         else:
             self.measure(flat_list, cbit_list)
 
+    def cv_delay(self, duration, qumode, unit="ns"):
+        """CV_delay. Implements an identity gate of the specified duration. 
+        This is particularly useful for the implementation of a noise pass.
+
+        Args:
+            duration (real): duration of delay gate
+            qumode (list): list of qubits representing qumode
+
+        Returns:
+            Instruction: QisKit instruction
+        """
+        return self.append(
+            ParameterizedUnitaryGate(
+                self.ops.id, [], num_qubits=len(qumode), label="delay(" + str(duration) + " " + unit +")", duration=duration, unit=unit
+            ),
+            qargs=qumode,
+        )
+
     def cv_c_multiboson_sampling(self, max, qumode, qubit, duration=1, unit="us"):
         """SNAP (Selective Number-dependent Arbitrary Phase) gates for multiboson sampling.
         Args:
             max (int): the period of the mapping
             qumode (list): list of qubits representing qumode
             qubit (Qubit): control qubit.
         Returns:
@@ -757,7 +841,58 @@
         """
         self.append(
             ParameterizedUnitaryGate(
                 self.ops.c_multiboson_sampling, [max], num_qubits=len(qumode) + 1, label="c_multiboson_sampling", duration=duration, unit=unit
             ),
             qargs=qumode + [qubit],
         )
+
+    def cv_gate_from_matrix(self, matrix, qumodes=[], qubits=[], duration=100, unit="ns"):
+        """Converts matrix to gate. Note that if you choose to input some complex gate that would typically be physically 
+        implemented by multiple successive gate operations, PhotonLossNoisePass, simulate(discretize=True), and animate may 
+        not be applied in a way that is physical.
+
+        Args:
+            matrix (np.array/nested list): Matrix for conversion into gate
+            qumodes (QumodeRegister/list): Qumodes initialized by QumodeRegister
+            qubits (QuantumRegister/list): Qubits initialized by QuantumRegister
+
+        Returns:
+            Instruction: QisKit instruction
+        """     
+        # If multiple qubits are given, slice to get list of qubits. Otherwise, encase QuantumRegister for single qubit in list.
+        try: 
+            qubits = qubits[:]
+        except: 
+            qubits = [qubits]
+
+        # Slice QumodeRegister to get list of qumodes
+        if isinstance(qumodes, QumodeRegister):    
+            qumodes = qumodes[:]
+
+        # Convert matrix to np.ndarray so that we can compute error flags easier
+        matrix = np.array(matrix)
+        
+        ## Error flags
+        # Matrix needs to be square
+        n, m = matrix.shape
+        if n != m:
+            raise ValueError("Matrix given is not square")
+        
+        # Determine if input matrix is same dimension as input qumodes+qubits
+        if n != 2 ** (len(qumodes) + len(qubits)):
+            raise ValueError("Matrix is of different dimension from qumodes + qubits")
+
+        # Checks if input matrix is unitary
+        if not is_unitary_matrix(matrix):
+            raise ValueError("The mapping provided is not unitary!")
+
+        # Make sure that np.ndarray doesn't get fed into PUG
+        if isinstance(matrix, np.ndarray):
+            matrix = matrix.tolist()
+
+        return self.append(
+            ParameterizedUnitaryGate(
+                self.ops.gate_from_matrix, [matrix], num_qubits=len(qumodes) + len(qubits), label="gate_from_matrix", duration=duration, unit=unit
+            ),
+            qargs=qumodes + qubits,
+        )
```

### Comparing `bosonic-qiskit-8.1/c2qa/kraus.py` & `bosonic-qiskit-9.0/c2qa/kraus.py`

 * *Files 6% similar despite different names*

```diff
@@ -150,51 +150,57 @@
 
         # Test that we have the correct number of photon loss rates
         if len(self._photon_loss_rates) != self._num_qumodes:
             raise Exception("List of photon loss rates must have same length as number of qumodes! (i.e., one rate per qumode)")
 
         # Convert photon loss rate to photons per second
         if self._time_unit == "dt":
-            self._photon_loss_rates_sec = [rate * self._dt for rate in self._photon_loss_rates] 
+            self.photon_loss_rates_sec = [rate * self._dt for rate in self._photon_loss_rates] 
         else:
             conversion = 1.0 / apply_prefix(1.0, self._time_unit)
-            self._photon_loss_rates_sec = [rate * conversion for rate in self._photon_loss_rates] 
+            self.photon_loss_rates_sec = [rate * conversion for rate in self._photon_loss_rates] 
 
         super().__init__(self._photon_loss_error)
 
     def _photon_loss_error(self, op: Instruction, qubits: Sequence[int]):
         """Return photon loss error on each operand qubit"""
         error = None
         
-        if (self._instructions is None or op.name in self._instructions) and (self._qumode_indices is None or any(x in qubits for x in self._qumode_indices)):
+        if self.applies_to_instruction(op, qubits):
             if not op.duration:
                 if op.duration is None:
                     warnings.warn(
                         "PhotonLossNoisePass ignores instructions without duration,"
                         " you may need to schedule circuit in advance.",
                         UserWarning,
                     )
                 return None
 
             # Qiskit `delay` gates are always for one qubit, see https://qiskit.org/documentation/stubs/qiskit.circuit.QuantumCircuit.delay.html            
             if op.name == "delay":
                 warnings.warn("Qiskit applies delays as single qubit gates. Qumode PhotonLossNoisePass will not be applied")
                 return None
 
-            # Convert op duration to seconds
-            if op.unit == "dt":
-                if self._dt is None:
-                    raise NoiseError(
-                        "PhotonLossNoisePass cannot apply noise to a 'dt' unit duration"
-                        " without a dt time set."
-                    )
-                duration = op.duration * self._dt
-            else:
-                duration = apply_prefix(op.duration, op.unit)
+            duration = self.duration_to_sec(op)
 
             kraus_operators = calculate_kraus(
-                self._photon_loss_rates_sec, duration, self._circuit, qubits, self._qumode_indices
+                self.photon_loss_rates_sec, duration, self._circuit, qubits, self._qumode_indices
             )
 
             error = kraus_error(kraus_operators)
 
         return error
+
+    def applies_to_instruction(self, op: Instruction, qubits: Sequence[int]):
+        """Test if this PhotonLossNoisePass applies to the given instruction based on its name and qumodes (qubits)"""
+        return (self._instructions is None or op.name in self._instructions) and (self._qumode_indices is None or any(x in qubits for x in self._qumode_indices))
+
+    def duration_to_sec(self, op: Instruction):
+        """Return the given Instruction's duration in seconds"""
+        if op.unit == "dt":
+            if self._dt is None:
+                raise NoiseError("PhotonLossNoisePass cannot apply noise to a 'dt' unit duration without a dt time set.")
+            duration = op.duration * self._dt
+        else:
+            duration = apply_prefix(op.duration, op.unit)
+
+        return duration
```

### Comparing `bosonic-qiskit-8.1/c2qa/operators.py` & `bosonic-qiskit-9.0/c2qa/operators.py`

 * *Files 9% similar despite different names*

```diff
@@ -34,63 +34,75 @@
         # self.N = scipy.sparse.matmul(self.a_dag, self.a)
         self.N = self.a_dag * self.a
 
         self.eye = scipy.sparse.eye(cutoff)
 
         self.cutoff_value = cutoff
 
+    def id(self):
+        """Identity gate (used by cv_delay)
+
+        Args:
+            None
+
+        Returns:
+            dia_matrix: operator matrix
+        """
+
+        return self.eye
+
     def r(self, theta):
         """Phase space rotation operator
 
         Args:
             theta (real): rotation
 
         Returns:
-            ndarray: operator matrix
+            csc_matrix: operator matrix
         """
         arg = 1j * theta * self.N
 
         return scipy.sparse.linalg.expm(arg)
 
     def d(self, alpha):
         """Displacement operator
 
         Args:
             alpha (real): displacement
 
         Returns:
-            ndarray: operator matrix
+            csc_matrix: operator matrix
         """
         arg = (alpha * self.a_dag) - (numpy.conjugate(alpha) * self.a)
 
         return scipy.sparse.linalg.expm(arg)
 
     def s(self, theta):
         """Single-mode squeezing operator
 
         Args:
             theta (real): squeeze
 
         Returns:
-            ndarray: operator matrix
+            csc_matrix: operator matrix
         """
         a_sqr = self.a * self.a
         a_dag_sqr = self.a_dag * self.a_dag
         arg = 0.5 * ((numpy.conjugate(theta) * a_sqr) - (theta * a_dag_sqr))
 
         return scipy.sparse.linalg.expm(arg)
 
     def s2(self, theta):
         """Two-mode squeezing operator
 
         Args:
             g (real): multiplied by 1j to yield imaginary phase
 
         Returns:
-            ndarray: operator matrix
+            csc_matrix: operator matrix
         """
 
         self.a1 = scipy.sparse.kron(self.a, self.eye).tocsc()
         self.a2 = scipy.sparse.kron(self.eye, self.a).tocsc()
         self.a1_dag = self.a1.conjugate().transpose().tocsc()
         self.a2_dag = self.a2.conjugate().transpose().tocsc()
 
@@ -104,15 +116,15 @@
     def bs(self, theta):
         """Two-mode beam splitter operator
 
         Args:
             theta: phase
 
         Returns:
-            ndarray: operator matrix
+            csc_matrix: operator matrix
         """
 
         self.a1 = scipy.sparse.kron(self.a, self.eye).tocsc()
         self.a2 = scipy.sparse.kron(self.eye, self.a).tocsc()
         self.a1_dag = self.a1.conjugate().transpose().tocsc()
         self.a2_dag = self.a2.conjugate().transpose().tocsc()
 
@@ -126,55 +138,55 @@
     def cr(self, theta):
         """Controlled phase space rotation operator
 
         Args:
             theta (real): phase
 
         Returns:
-            ndarray: operator matrix
+            csc_matrix: operator matrix
         """
         arg = theta * 1j * scipy.sparse.kron(zQB, self.N).tocsc()
 
         return scipy.sparse.linalg.expm(arg)
 
     def crx(self, theta):
         """Controlled phase space rotation operator around sigma^x
 
         Args:
             theta (real): phase
 
         Returns:
-            ndarray: operator matrix
+            csc_matrix: operator matrix
         """
         arg = theta * 1j * scipy.sparse.kron(xQB, self.N).tocsc()
 
         return scipy.sparse.linalg.expm(arg)
 
     def cry(self, theta):
         """Controlled phase space rotation operator around sigma^x
 
         Args:
             theta (real): phase
 
         Returns:
-            ndarray: operator matrix
+            csc_matrix: operator matrix
         """
         arg = theta * 1j * scipy.sparse.kron(yQB, self.N).tocsc()
 
         return scipy.sparse.linalg.expm(arg)
 
     def cd(self, theta, beta=None):
         """Controlled displacement operator
 
         Args:
             theta (real): displacement for qubit state 0
             beta (real): displacement for qubit state 1. If None, use -alpha.
 
         Returns:
-            ndarray: operator matrix
+            bsr_matrix: operator matrix
         """
         displace0 = (theta * self.a_dag) - (numpy.conjugate(theta) * self.a)
         if beta is None:
             beta = -theta
         displace1 = (beta * self.a_dag) - (numpy.conjugate(beta) * self.a)
 
         return scipy.sparse.kron(
@@ -184,29 +196,29 @@
     def ecd(self, theta):
         """Echoed controlled displacement operator
 
         Args:
             theta (real): displacement
 
         Returns:
-            ndarray: operator matrix
+            csr_matrix: operator matrix
         """
         argm = (theta * self.a_dag) - (numpy.conjugate(theta) * self.a)
         arg = scipy.sparse.kron(zQB, argm)
 
         return scipy.sparse.linalg.expm(arg)
 
     def cbs(self, theta):
         """Controlled phase two-mode beam splitter operator
 
         Args:
             theta (real): real phase
 
         Returns:
-            ndarray: operator matrix
+            csc_matrix: operator matrix
         """
         self.a1 = scipy.sparse.kron(self.a, self.eye).tocsc()
         self.a2 = scipy.sparse.kron(self.eye, self.a).tocsc()
         self.a1_dag = self.a1.conjugate().transpose().tocsc()
         self.a2_dag = self.a2.conjugate().transpose().tocsc()
 
         a12dag = self.a1 * self.a2_dag
@@ -220,15 +232,15 @@
     def cschwinger(self, beta, theta_1, phi_1, theta_2, phi_2):
         """General form of a controlled Schwinger gate
 
         Args:
             params (real): [beta, theta_1, phi_1, theta_2, phi_2]
 
         Returns:
-            ndarray: operator matrix
+            csc_matrix: operator matrix
         """
         self.a1 = scipy.sparse.kron(self.a, self.eye).tocsc()
         self.a2 = scipy.sparse.kron(self.eye, self.a).tocsc()
         self.a1dag = self.a1.conjugate().transpose().tocsc()
         self.a2dag = self.a2.conjugate().transpose().tocsc()
 
         a12dag = self.a1 * self.a2dag
@@ -248,15 +260,15 @@
         """SNAP (Selective Number-dependent Arbitrary Phase) operator
 
         Args:
             theta (real): phase
             n (integer): Fock state in which the mode should acquire the phase
 
         Returns:
-            ndarray: operator matrix
+            csc_matrix: operator matrix
         """
 
         ket_n = numpy.zeros(self.cutoff_value)
         ket_n[n] = 1
         projector = numpy.outer(ket_n, ket_n)
         sparse_projector = scipy.sparse.csr_matrix(projector)
         arg = theta * 1j * sparse_projector.tocsc()
@@ -268,61 +280,87 @@
         fock-number selective qubit rotations.
 
         Args:
             theta (real): phase
             n (integer): Fock state in which the mode should acquire the phase
 
         Returns:
-            ndarray: operator matrix
+            csc_matrix: operator matrix
         """
 
         ket_n = numpy.zeros(self.cutoff_value)
         ket_n[n] = 1
         projector = numpy.outer(ket_n, ket_n)
         # sparse_projector = scipy.sparse.csc_matrix(projector)
         arg = theta * 1j * scipy.sparse.kron(zQB, projector).tocsc()
         return scipy.sparse.linalg.expm(arg)
-    
+        
     def multisnap(self, *args):
-        """multi-SNAP (Selective Number-dependent Arbitrary Phase) operator,
-        with explicit sigma_z in exponential. Can be used to generate
-        fock-number selective qubit rotations.
+        """SNAP (Selective Number-dependent Arbitrary Phase) operator for multiple Fock states.
+        Generates an arbitrary number of fock-number selective qubit rotations.
+        
         Args:
-            theta (real): phase
-            n (integer): Fock state in which the mode should acquire the phase
+            args (List[reals, integers]): [List of phases, List of Fock states in which the mode should acquire the associated phase]
+        
+        Returns:
+            csr_matrix: operator matrix
+        """
+        # Divide list in two because thetas and ns must be sent in as a single list
+        thetas = args[:len(args) // 2] # arguments
+        ns = args[len(args) // 2:] # Fock states on which they are applied
+        if len(thetas)!=len(ns): # one theta per Fock state to apply it to
+            raise Exception("len(theta) must be equal to len(n)")
+
+        id = numpy.eye(self.cutoff_value)
+        gate = scipy.sparse.csr_matrix(id)
+        for i in range(len(ns)):
+            ket_n = numpy.zeros(self.cutoff_value)
+            ket_n[ns[i]] = 1
+            projector = numpy.outer(ket_n, ket_n)
+            coeff = numpy.exp(1j * thetas[i]) - 1
+            mat = scipy.sparse.csr_matrix(coeff * projector)
+            gate = numpy.add(gate, mat)
+        return scipy.sparse.csr_matrix(gate)
+
+    def multicsnap(self, *args):
+        """SNAP (Selective Number-dependent Arbitrary Phase) operator for multiple Fock states.
+        Generates an arbitrary number of fock-number selective qubit rotations, with the qubit that accrues the geometric phase explicit.
+        
+        Args:
+            args (List[reals, integers]): [List of phases, List of Fock states in which the mode should acquire the associated phase]
+        
         Returns:
-            ndarray: operator matrix
+            csr_matrix: operator matrix
         """
         # Divide list in two because thetas and ns must be sent in as a single list
         thetas = args[:len(args) // 2] # arguments
         ns = args[len(args) // 2:] # Fock states on which they are applied
         if len(thetas)!=len(ns): # one theta per Fock state to apply it to
-            raise Exception("len(thetas) must be equal to len(ns)")
+            raise Exception("len(theta) must be equal to len(n)")
 
         id = numpy.eye(self.cutoff_value)
-        ket_0 = numpy.zeros(self.cutoff_value)
-        ket_0[0] = 1
-        projector = numpy.outer(ket_0, ket_0)
-        coeff = numpy.exp(- 1j * 0) - 1
-        gate = scipy.sparse.csr_matrix(id + coeff * projector)
+        gate = scipy.sparse.csr_matrix(scipy.sparse.kron(idQB,id))
         for i in range(len(ns)):
             ket_n = numpy.zeros(self.cutoff_value)
             ket_n[ns[i]] = 1
             projector = numpy.outer(ket_n, ket_n)
-            coeff = numpy.exp(- 1j * thetas[i]) - 1
-            mat = scipy.sparse.csr_matrix(id + (coeff * projector))
-            gate = gate @ mat
+            coeff = scipy.sparse.linalg.expm(1j * thetas[i] * zQB) - idQB
+            mat = scipy.sparse.kron(coeff,projector).tocsr()
+            gate = numpy.add(gate, mat)
         return scipy.sparse.csr_matrix(gate)
+
     
-    def c_multiboson_sampling(self, max):
-        """SNAP gate creation for multiboson sampling purposes.
+    def pnr(self, max):
+        """Support gate for photon number readout (see Curtis et al., PRA (2021) and Wang et al., PRX (2020))
+        
         Args:
             max (int): the period of the mapping
+        
         Returns:
-            ndarray: operator matrix
+            csc_matrix: operator matrix
         """
         ket_n = numpy.zeros(self.cutoff_value)
         projector = numpy.outer(ket_n, ket_n)
         # binary search
         for j in range(int(max / 2)):
             for i in range(j, self.cutoff_value, max):
                 ket_n = numpy.zeros(self.cutoff_value)
@@ -337,15 +375,15 @@
     def eswap(self, theta):
         """Exponential SWAP operator
 
         Args:
             theta (real): rotation
 
         Returns:
-            ndarray: operator matrix
+            csc_matrix: operator matrix
         """
 
         self.mat = numpy.zeros([self.cutoff_value * self.cutoff_value, self.cutoff_value * self.cutoff_value])
         for j in range(self.cutoff_value):
             for i in range(self.cutoff_value):
                 self.mat[i + (j * self.cutoff_value)][i * self.cutoff_value + j] = 1
         self.sparse_mat = scipy.sparse.csr_matrix(self.mat).tocsc()
@@ -358,15 +396,15 @@
     def csq(self, theta):
         """Single-mode squeezing operator
 
         Args:
             theta (real): squeeze
 
         Returns:
-            ndarray: operator matrix
+            csc_matrix: operator matrix
         """
         a_sqr = self.a * self.a
         a_dag_sqr = self.a_dag * self.a_dag
         arg = scipy.sparse.kron(zQB, 0.5 * ((numpy.conjugate(theta) * a_sqr) - (theta * a_dag_sqr))).tocsc()
 
         return scipy.sparse.linalg.expm(arg)
 
@@ -374,15 +412,26 @@
     def testqubitorderf(self, phi):
 
         arg = 1j * phi * scipy.sparse.kron(xQB, idQB)
         return scipy.sparse.linalg.expm(arg)
 
     def c_multiboson_sampling(self, max):
         """SNAP gate creation for multiboson sampling purposes.
+        
         Args:
             max (int): the period of the mapping
+        
         Returns:
-            ndarray: operator matrix
+            dia_matrix: operator matrix
         """
         print(max)
 
         return self.eye
+
+    def gate_from_matrix(self, matrix):
+        """Converts matrix into gate. Called using ParameterizedUnitaryGate.
+        Args:
+            matrix (list): the (unitary) matrix that you wish to convert into a gate
+        Returns:
+            csc_matrix: operator matrix
+        """ 
+        return scipy.sparse.csc_matrix(matrix)
```

### Comparing `bosonic-qiskit-8.1/c2qa/parameterized_unitary_gate.py` & `bosonic-qiskit-9.0/c2qa/parameterized_unitary_gate.py`

 * *Files 22% similar despite different names*

```diff
@@ -8,40 +8,42 @@
 from qiskit.extensions.unitary import UnitaryGate
 
 
 class ParameterizedUnitaryGate(Gate):
     """UnitaryGate sublcass that stores the operator matrix for later reference by animation utility."""
 
     def __init__(
-        self, op_func, params, num_qubits, label=None, duration=100, unit="ns"
+        self, op_func, params, num_qubits, label=None, duration=100, unit="ns", discretized_param_indices: list = []
     ):
         """Initialize ParameterizedUnitaryGate
 
         Args:
             op_func (function): function to build operator matrix
             params (List): List of parameters to pass to op_func to build
                 operator matrix (supports instances of Qiskit Parameter to be
                 bound later)
             num_qubits (int): Number of qubits in the operator -- this would
                 likely equate to (num_qubits_per_qumode * num_qumodes + num_ancilla).
             label (string, optional): Gate name. Defaults to None.
             duration (int, optional): Duration of gate used for noise modeling. Defaults to 100.
             unit (string, optional): Unit of duration (only supports those allowed by Qiskit).
+            discretized_param_indices (list): list of int indices into self.params for parameters to be discretized. An empty list will discretize all params.
         """
         super().__init__(name=label, num_qubits=num_qubits, params=params, label=label)
 
         self.op_func = op_func
 
         self._parameterized = any(
             isinstance(param, ParameterExpression) and param.parameters
             for param in params
         )
 
         self.duration = duration
         self.unit = unit
+        self.discretized_param_indices = discretized_param_indices
 
     def __array__(self, dtype=None):
         """Call the operator function to build the array using the bound parameter values."""
         # return self.op_func(*map(complex, self.params)).toarray()
         values = []
         for param in self.params:
             if isinstance(param, ParameterExpression):
@@ -99,45 +101,58 @@
             ndarray: operator matrix
         """
         if self.is_parameterized():
             raise NotImplementedError(
                 "Unable to calculate incremental operator matrices for parameterized gate"
             )
 
-        values = self.calculate_frame_params(current_step, total_steps, keep_state)
+        values = self.calculate_segment_params(current_step, total_steps, keep_state)
 
         # if self.inverse:
         #     result = scipy.sparse.linalg.inv(self.op_func(*values))
         # else:
         #     result = self.op_func(*values)
         result = self.op_func(*values)
 
         if hasattr(result, "toarray"):
             result = result.toarray()
 
         return result
 
 
-def __calculate_frame_params(
+def __calculate_segment_params(
     self, current_step: int = 1, total_steps: int = 1, keep_state: bool = False
 ):
-    """Calculate the parameters at the current step. Return a tuples of the values."""
+    """
+    Calculate the parameters at the current step. Return a tuples of the values.
+    
+     Args:
+        current_step (int): 0-based current step index of the discretization
+        total_steps (int): total number of discretization steps
+        keep_state (bool): true if the state should be kept between discretization steps (i.e., if the discretization value should be 1/total_steps vs current_step/total_steps)
+        
+    Returns:
+        discretized parameter values as tuple
+    """
     if keep_state:
         param_fraction = 1 / total_steps
     else:
         param_fraction = current_step / total_steps
 
     values = []
-    for param in self.params:
-        values.append(param * param_fraction)
+    for index, param in enumerate(self.params):
+        if not hasattr(self, "discretized_param_indices") or len(self.discretized_param_indices) == 0 or index in self.discretized_param_indices:
+            values.append(param * param_fraction)
+        else:
+            values.append(param)
 
     return tuple(values)
 
 
-def __calculate_frame_duration(
+def __calculate_segment_duration(
     self, current_step: int = 1, total_steps: int = 1, keep_state: bool = False
 ):
     """Calculate the duration at the current step. Return a tuple of the (duration, unit)."""
     frame_duration = None
 
     if self.duration:
         if keep_state:
@@ -147,9 +162,9 @@
 
         frame_duration = self.duration * fraction
     
     return frame_duration, self.unit
 
 
 # Monkey patch Qiskit Instruction to support animating base Qiskit Instruction
-qiskit.circuit.instruction.Instruction.calculate_frame_params = __calculate_frame_params
-qiskit.circuit.instruction.Instruction.calculate_frame_duration = __calculate_frame_duration
+qiskit.circuit.instruction.Instruction.calculate_segment_params = __calculate_segment_params
+qiskit.circuit.instruction.Instruction.calculate_segment_duration = __calculate_segment_duration
```

### Comparing `bosonic-qiskit-8.1/c2qa/qumoderegister.py` & `bosonic-qiskit-9.0/c2qa/qumoderegister.py`

 * *Files 6% similar despite different names*

```diff
@@ -63,14 +63,18 @@
             raise ValueError("Must provide slice or int.")
 
         return self.qreg[start:stop:step]
 
     def __len__(self):
         """The length of a QumodeRegister is the number of qumodes (not the num_qumodes * num_qubits_per_qumode)"""
         return self.num_qumodes
+    
+    def __contains__(self, qubit):
+        """Return true if this QumodeRegister contains the given qubit. This allows callers to use `in` python syntax."""
+        return qubit in self.qreg
 
 
 class QumodeIterator:
     """Iterate over the list of lists representing the qubits for each qumode in the register"""
 
     def __init__(self, register: QumodeRegister):
         self._index = 0
```

### Comparing `bosonic-qiskit-8.1/c2qa/wigner.py` & `bosonic-qiskit-9.0/c2qa/wigner.py`

 * *Files 14% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     xvec: np.ndarray,
     shots: int,
     noise_passes=None,
     conditional: bool = True,
     trace: bool = False,
 ):
     """Simulate the circuit, optionally partial trace the results, and calculate the Wigner function."""
-    states, _ = simulate(
+    states, _, _ = simulate(
         circuit,
         shots=shots,
         noise_passes=noise_passes,
         conditional_state_vector=conditional,
     )
 
     if states:
@@ -50,14 +50,48 @@
         )
         wigner_result = None
         state = None
 
     return wigner_result, state
 
 
+def simulate_wigner_multiple_statevectors(
+    circuit: CVCircuit,
+    xvec: np.ndarray,
+    shots: int,
+    statevector_label: str,
+    num_statevectors:int,
+    noise_passes=None,
+    trace: bool = False,
+):
+    """Simulate the circuit, optionally partial trace the results, and calculate the Wigner function on each statevector starting with the given label."""
+    state, result, _ = simulate(
+        circuit,
+        shots=shots,
+        noise_passes=noise_passes
+    )
+
+    if len(result.results):
+        wigner_results = []
+        for num in range(num_statevectors):
+            state = result.data()[f"{statevector_label}{num}"]
+            if trace:
+                density_matrix = trace_out_qubits(circuit, state)
+            else:
+                density_matrix = state
+
+            wigner_results.append(_wigner(density_matrix, xvec))
+    else:
+        print(
+            "WARN: No state vector returned by simulation -- unable to calculate Wigner function!"
+        )
+        wigner_results = None
+
+    return wigner_results
+
 def wigner(
     state,
     axes_min: int = -6,
     axes_max: int = 6,
     axes_steps: int = 200,
 ):
     """
@@ -272,20 +306,20 @@
     Args:
         circuit (CVCircuit): circuit to simulate and plot
         qubit (Qubit): qubit to measure
         file (str, optional): File path to save file, if None return plot. Defaults to None.
         draw_grid (bool, optional): True if gridlines should be drawn on plots. Defaults to False.
     """
     # Get unaltered state vector and partial trace
-    x, _ = simulate(circuit)
+    x, _, _ = simulate(circuit)
     xT = x.data.conjugate().transpose()
 
     # Project onto 0 and 1 using Pauli Z
     circuit.z(qubit)
-    y, _ = simulate(circuit)
+    y, _, _ = simulate(circuit)
     yT = y.data.conjugate().transpose()
 
     x_xT = x.data * xT
     x_yT = x.data * yT
     y_xT = y.data * xT
     y_yT = y.data * yT
 
@@ -298,15 +332,15 @@
     projection_one = (trace_x_xT - trace_x_yT - trace_y_xT + trace_y_yT) / 4
 
     # Clean up by popping off the Pauli Z
     circuit.data.pop()
 
     # Project onto + and - using Pauli X
     circuit.x(qubit)
-    y, _ = simulate(circuit)
+    y, _, _ = simulate(circuit)
     yT = y.data.conjugate().transpose()
 
     x_xT = x.data * xT
     x_yT = x.data * yT
     y_xT = y.data * xT
     y_yT = y.data * yT
```

### Comparing `bosonic-qiskit-8.1/setup.py` & `bosonic-qiskit-9.0/setup.py`

 * *Files identical despite different names*

### Comparing `bosonic-qiskit-8.1/tests/test_animate.py` & `bosonic-qiskit-9.0/tests/test_animate.py`

 * *Files identical despite different names*

### Comparing `bosonic-qiskit-8.1/tests/test_gates.py` & `bosonic-qiskit-9.0/tests/test_gates.py`

 * *Files 7% similar despite different names*

```diff
@@ -54,39 +54,39 @@
 
     # TODO - better understand what the state vector results should be
     assert count_nonzero(state) == 1
 
 
 def test_no_gates():
     circuit, qmr = create_unconditional()
-    state, result = c2qa.util.simulate(circuit)
+    state, result, fock_counts = c2qa.util.simulate(circuit)
     assert_unchanged(state, result)
 
 
 def test_beamsplitter_once():
     circuit, qmr = create_unconditional()
 
     phi = random.random()
     circuit.cv_bs(phi, qmr[0], qmr[1])
 
-    state, result = c2qa.util.simulate(circuit)
+    state, result, fock_counts = c2qa.util.simulate(circuit)
 
     # TODO - Beam splitter gate does not change state vector
     #        Both Strawberry Fields & FockWits are the same, too.
     # assert_changed(state, result)
     assert_unchanged(state, result)
 
 
 def test_conditional_beamsplitter():
     circuit, qmr, qr = create_conditional()
 
     theta = random.random()
     circuit.cv_c_bs(theta, qmr[0], qmr[1], qr[0])
 
-    state, result = c2qa.util.simulate(circuit)
+    state, result, fock_counts = c2qa.util.simulate(circuit)
 
     # TODO - Beam splitter gate does not change state vector
     #        Both Strawberry Fields & FockWits are the same, too.
     # assert_changed(state, result)
     assert_unchanged(state, result)
 
 def test_conditional_schwinger():
@@ -95,78 +95,85 @@
     beta = random.random()
     theta_1 = random.random()
     phi_1 = random.random()
     theta_2 = random.random()
     phi_2 = random.random()
     circuit.cv_c_schwinger([beta, theta_1, phi_1, theta_2, phi_2], qmr[0], qmr[1], qr[0])
 
-    state, result = c2qa.util.simulate(circuit)
+    state, result, fock_counts = c2qa.util.simulate(circuit)
 
     assert_unchanged(state, result)
 
 
 def test_beamsplitter_twice():
     circuit, qmr = create_unconditional()
 
     phi = random.random()
     circuit.cv_bs(phi, qmr[0], qmr[1])
     circuit.cv_bs(-phi, qmr[0], qmr[1])
 
-    state, result = c2qa.util.simulate(circuit)
+    state, result, fock_counts = c2qa.util.simulate(circuit)
     assert_unchanged(state, result)
 
 
 def test_conditonal_displacement():
     circuit, qmr, qr = create_conditional()
 
     alpha = random.random()
     circuit.cv_c_d(alpha, qmr[0], qr[0])
     circuit.cv_c_d(-alpha, qmr[0], qr[0])
 
     circuit.cv_c_d(-alpha, qmr[0], qr[1])
     circuit.cv_c_d(alpha, qmr[0], qr[1])
 
-    state, result = c2qa.util.simulate(circuit)
+    state, result, fock_counts = c2qa.util.simulate(circuit)
     assert_unchanged(state, result)
 
 
 def test_conditonal_squeezing():
     circuit, qmr, qr = create_conditional()
 
     alpha = random.random()
     circuit.cv_c_sq(alpha, qmr[0], qr[0])
     circuit.cv_c_sq(-alpha, qmr[0], qr[0])
 
     circuit.cv_c_sq(-alpha, qmr[0], qr[1])
     circuit.cv_c_sq(alpha, qmr[0], qr[1])
 
-    state, result = c2qa.util.simulate(circuit)
+    state, result, fock_counts = c2qa.util.simulate(circuit)
     assert_unchanged(state, result)
 
 
 def test_displacement_once(capsys):
     with capsys.disabled():
         circuit, qmr = create_unconditional()
 
         # alpha = random.random()
         alpha = 1
         circuit.cv_d(alpha, qmr[0])
 
-        state, result = c2qa.util.simulate(circuit)
+        state, result, fock_counts = c2qa.util.simulate(circuit)
         assert_changed(state, result)
 
+def test_cv_delay():
+    circuit, qmr = create_unconditional()
+
+    circuit.cv_delay(100,qmr[0])
+
+    state, result, fock_counts = c2qa.util.simulate(circuit)
+
 
 def test_displacement_twice():
     circuit, qmr = create_unconditional()
 
     alpha = random.random()
     circuit.cv_d(alpha, qmr[0])
     circuit.cv_d(-alpha, qmr[0])
 
-    state, result = c2qa.util.simulate(circuit)
+    state, result, fock_counts = c2qa.util.simulate(circuit)
     assert_unchanged(state, result)
 
 
 def test_cond_displacement_gate_vs_two_separate():
     from qiskit.extensions import UnitaryGate
 
     alpha = numpy.sqrt(numpy.pi)
@@ -174,15 +181,15 @@
     # Circuit using cnd_d
     qmr = c2qa.QumodeRegister(1, 2)
     qr = qiskit.QuantumRegister(1)
     cr = qiskit.ClassicalRegister(1)
     circuit = c2qa.CVCircuit(qmr, qr, cr)
     circuit.cv_initialize(0, qmr[0])  # qr[0] and cr[0] will init to zero
     circuit.cv_c_d(alpha, qmr[0], qr[0])
-    state, result = c2qa.util.simulate(circuit)
+    state, result, fock_counts = c2qa.util.simulate(circuit)
     assert result.success
     state_cnd = result.get_statevector(circuit)
 
     # Circuit using two controlled unitaries
     qmr = c2qa.QumodeRegister(1, 2)
     qr = qiskit.QuantumRegister(1)
     cr = qiskit.ClassicalRegister(1)
@@ -196,15 +203,15 @@
     )
     circuit.append(
         UnitaryGate(circuit.ops.d(-alpha).toarray()).control(
             num_ctrl_qubits=1, ctrl_state=1
         ),
         [qr[0]] + qmr[0],
     )
-    state, result = c2qa.util.simulate(circuit)
+    state, result, fock_counts = c2qa.util.simulate(circuit)
     assert result.success
     state_unitary = result.get_statevector(circuit)
 
     assert numpy.allclose(state_cnd, state_unitary)
 
 
 def test_displacement_calibration(capsys):
@@ -223,15 +230,15 @@
         circuit.cv_c_d(alpha, qmr[0], qr[0])
         circuit.cv_d(1j * alpha, qmr[0])
         circuit.cv_c_d(-alpha, qmr[0], qr[0])
         circuit.cv_d(-1j * alpha, qmr[0])
         circuit.h(qr[0])
         circuit.measure(qr[0], cr[0])
 
-        state, result = c2qa.util.simulate(circuit)
+        state, result, fock_counts = c2qa.util.simulate(circuit)
         assert result.success
 
         state = result.get_statevector(circuit)
         counts = result.get_counts(circuit)
 
         assert state.dim > 0
         assert counts
@@ -244,72 +251,72 @@
 
 def test_rotation_once():
     circuit, qmr = create_unconditional()
 
     theta = random.random()
     circuit.cv_r(theta, qmr[0])
 
-    state, result = c2qa.util.simulate(circuit)
+    state, result, fock_counts = c2qa.util.simulate(circuit)
 
     # TODO - Rotation gate does not change state vector.
     #        Both Strawberry Fields & FockWits are the same, too.
     # assert_changed(state, result)
     assert_unchanged(state, result)
 
 
 def test_rotation_twice():
     circuit, qmr = create_unconditional()
 
     theta = random.random()
     circuit.cv_r(theta, qmr[0])
     circuit.cv_r(-theta, qmr[0])
 
-    state, result = c2qa.util.simulate(circuit)
+    state, result, fock_counts = c2qa.util.simulate(circuit)
     assert_unchanged(state, result)
 
 
 def test_squeezing_once():
     circuit, qmr = create_unconditional()
 
     z = random.random()
     circuit.cv_sq(z, qmr[0])
 
-    state, result = c2qa.util.simulate(circuit)
+    state, result, fock_counts = c2qa.util.simulate(circuit)
     assert_changed(state, result)
 
 
 def test_squeezing_twice():
     circuit, qmr = create_unconditional()
 
     z = random.random()
     circuit.cv_sq(z, qmr[0])
     circuit.cv_sq(-z, qmr[0])
 
-    state, result = c2qa.util.simulate(circuit)
+    state, result, fock_counts = c2qa.util.simulate(circuit)
     assert_unchanged(state, result)
 
 
 def test_two_mode_squeezing_once():
     circuit, qmr = create_unconditional()
 
     z = random.random()
     circuit.cv_sq2(z, qmr[0], qmr[1])
 
-    state, result = c2qa.util.simulate(circuit)
+    state, result, fock_counts = c2qa.util.simulate(circuit)
     assert_changed(state, result)
 
 
 def test_two_mode_squeezing_twice():
     circuit, qmr = create_unconditional()
 
     z = random.random()
     circuit.cv_sq2(z, qmr[0], qmr[1])
     circuit.cv_sq2(-z, qmr[0], qmr[1])
 
-    state, result = c2qa.util.simulate(circuit)
+    state, result, fock_counts = c2qa.util.simulate(circuit)
     assert_unchanged(state, result)
 
 
 def test_gates():
     """Verify that we can use the gates, not that they are actually working."""
 
     # ===== Constants =====
@@ -328,43 +335,43 @@
 
     # Hybrid qubit-cavity gates
     circuit.cv_c_d(alpha, qmr[0], qr[0])
     circuit.cv_c_d(alpha, qmr[1], qr[0])
     circuit.cv_c_sq(z, qmr[0], qr[0])
     circuit.cv_c_sq(z, qmr[1], qr[0])
 
-    state, result = c2qa.util.simulate(circuit)
+    state, result, fock_counts = c2qa.util.simulate(circuit)
 
     assert result.success
 
 
 def test_snap():
     circuit, qmr = create_unconditional()
 
     phi = random.random()
     n = 1
     circuit.cv_snap(phi, n, qmr[0])
 
-    state, result = c2qa.util.simulate(circuit)
+    state, result, fock_counts = c2qa.util.simulate(circuit)
 
 
 def test_eswap():
     circuit, qmr = create_unconditional()
 
     phi = random.random()
     circuit.cv_eswap(phi, qmr[0], qmr[1])
 
-    state, result = c2qa.util.simulate(circuit)
+    state, result, fock_counts = c2qa.util.simulate(circuit)
 
 def test_multiboson_sampling(capsys):
     with capsys.disabled():
         num_qubits=1
         num_qumodes=2
         num_qubits_per_qumode=2
         qmrA = c2qa.QumodeRegister(num_qumodes = num_qumodes, num_qubits_per_qumode = num_qubits_per_qumode,name="qmrA_initial")
         qmrB = c2qa.QumodeRegister(num_qumodes = num_qumodes, num_qubits_per_qumode = num_qubits_per_qumode,name="qmrB_initial")
         qbr = qiskit.QuantumRegister(size=num_qubits,name='qbr_initial')
         circuit = c2qa.CVCircuit(qmrA, qmrB, qbr)
         circuit.cv_c_multiboson_sampling([0,1,2,3], qmrA[0], qbr[0])
 
-        state, result = c2qa.util.simulate(circuit)
+        state, result, fock_counts = c2qa.util.simulate(circuit)
         assert result.success
```

### Comparing `bosonic-qiskit-8.1/tests/test_inconsistent_statevectors.py` & `bosonic-qiskit-9.0/tests/test_inconsistent_statevectors.py`

 * *Files identical despite different names*

### Comparing `bosonic-qiskit-8.1/tests/test_noise_model.py` & `bosonic-qiskit-9.0/tests/test_noise_model.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import math
 from pathlib import Path
 import pytest
 import random
 
 
 import c2qa
 import numpy as np
@@ -44,15 +45,15 @@
             op_qubits=[0, 1, 2],
             qumode_indices=[0, 1]
         )
 
         print("kraus")
         print(kraus_operators)
 
-        state, result = c2qa.util.simulate(circuit)
+        state, result, fock_counts = c2qa.util.simulate(circuit)
 
 
 def test_kraus_operators(capsys):
     with capsys.disabled():
         num_qumodes = 1
         num_qubits_per_qumode = 2
         qmr = c2qa.QumodeRegister(num_qumodes, num_qubits_per_qumode)
@@ -196,15 +197,15 @@
         qmr = c2qa.QumodeRegister(num_qumodes=num_qumodes, num_qubits_per_qumode=qubits_per_mode)
         init_circuit = c2qa.CVCircuit(qmr)
         init_circuit.cv_initialize(2, qmr[0])
         init_circuit.cv_bs(1, qmr[1], qmr[0], duration=100, unit="ns")
         photon_loss_rate = 0.01
         time_unit = "ns"
         noise_pass = c2qa.kraus.PhotonLossNoisePass(photon_loss_rates=photon_loss_rate, circuit=init_circuit, time_unit=time_unit)
-        state, result = c2qa.util.simulate(init_circuit, noise_passes=noise_pass)
+        state, result, fock_counts = c2qa.util.simulate(init_circuit, noise_passes=noise_pass)
 
 
 def test_noise_with_cnd_beamsplitter(capsys):
     with capsys.disabled():
         num_qumodes = 2
         qubits_per_mode = 2
         num_qubits = 1
@@ -213,15 +214,15 @@
         qbr = qiskit.QuantumRegister(size=num_qubits)
         init_circuit = c2qa.CVCircuit(qmr, qbr)
         init_circuit.cv_initialize(2, qmr[0])
         init_circuit.cv_c_bs(1, qmr[1], qmr[0], qbr[0], duration=100, unit="ns")
         photon_loss_rate = 0.01
         time_unit = "ns"
         noise_pass = c2qa.kraus.PhotonLossNoisePass(photon_loss_rates=photon_loss_rate, circuit=init_circuit, time_unit=time_unit)
-        state, result = c2qa.util.simulate(init_circuit, noise_passes=noise_pass)
+        state, result, fock_counts = c2qa.util.simulate(init_circuit, noise_passes=noise_pass)
 
 
 def test_photon_loss_pass_with_conditional(capsys):
     with capsys.disabled():
         num_qumodes = 1
         qubits_per_mode = 2
         num_qubits = 1
@@ -230,15 +231,15 @@
         qbr = qiskit.QuantumRegister(size=num_qubits)
         init_circuit = c2qa.CVCircuit(qmr, qbr)
         init_circuit.cv_initialize(2, qmr[0])
         init_circuit.cv_c_d(1, qmr[0], qbr[0], duration=100, unit="ns")
         photon_loss_rate = 0.01
         time_unit = "ns"
         noise_pass = c2qa.kraus.PhotonLossNoisePass(photon_loss_rates=photon_loss_rate, circuit=init_circuit, time_unit=time_unit)
-        state, result = c2qa.util.simulate(init_circuit, noise_passes=noise_pass)
+        state, result, fock_counts = c2qa.util.simulate(init_circuit, noise_passes=noise_pass)
 
 
 def test_photon_loss_pass_delay_without_unit(capsys):
     with capsys.disabled():
         num_qumodes = 1
         qubits_per_mode = 2
         num_qubits = 1
@@ -249,15 +250,15 @@
         fail_circuit = c2qa.CVCircuit(qmr, qbr)
         fail_circuit.cv_initialize(2, qmr[0])
         fail_circuit.delay(duration=100) #, unit="ns")
         fail_circuit.cv_c_d(1, qmr[0], qbr[0], duration=100, unit="ns")
         photon_loss_rate = 0.01
         time_unit = "ns"
         noise_pass = c2qa.kraus.PhotonLossNoisePass(photon_loss_rates=photon_loss_rate, circuit=fail_circuit, time_unit=time_unit)
-        state, result = c2qa.util.simulate(fail_circuit, noise_passes=noise_pass)
+        state, result, fock_counts = c2qa.util.simulate(fail_circuit, noise_passes=noise_pass)
         assert result.success
 
 
 def test_photon_loss_pass_delay_with_unit(capsys):
     with capsys.disabled():
         num_qumodes = 1
         qubits_per_mode = 2
@@ -269,15 +270,15 @@
         pass_circuit = c2qa.CVCircuit(qmr, qbr)
         pass_circuit.cv_initialize(2, qmr[0])
         pass_circuit.delay(duration=100, unit="ns")
         pass_circuit.cv_c_d(1, qmr[0], qbr[0], duration=100, unit="ns")
         photon_loss_rate = 0.01
         time_unit = "ns"
         noise_pass = c2qa.kraus.PhotonLossNoisePass(photon_loss_rates=photon_loss_rate, circuit=pass_circuit, time_unit=time_unit)
-        state, result = c2qa.util.simulate(pass_circuit, noise_passes=noise_pass)
+        state, result, fock_counts = c2qa.util.simulate(pass_circuit, noise_passes=noise_pass)
         assert result.success
 
 
 def test_animate_photon_loss_pass(capsys):
     with capsys.disabled():
         num_qumodes = 1
         num_qubits_per_qumode = 4
@@ -298,14 +299,39 @@
             animation_segments=10,
             file=wigner_filename,
             noise_passes=noise_pass,
         )
         assert Path(wigner_filename).is_file()
 
 
+def test_animate_photon_loss_pas_with_epsilon(capsys):
+    with capsys.disabled():
+        num_qumodes = 1
+        num_qubits_per_qumode = 4
+        qmr = c2qa.QumodeRegister(num_qumodes, num_qubits_per_qumode)
+        circuit = c2qa.CVCircuit(qmr)
+
+        circuit.cv_initialize(3, qmr[0])
+
+        circuit.cv_d(0, qmr[0], duration=100, unit="ns")
+
+        photon_loss_rate = 0.01
+        time_unit = "ns"
+        noise_pass = c2qa.kraus.PhotonLossNoisePass(photon_loss_rates=photon_loss_rate, circuit=circuit, time_unit=time_unit)
+
+        wigner_filename = "tests/test_animate_photon_loss_pas_with_epsilon.gif"
+        c2qa.animate.animate_wigner(
+            circuit,
+            discretize_epsilon=0.1,
+            file=wigner_filename,
+            noise_passes=noise_pass,
+        )
+        assert Path(wigner_filename).is_file()
+
+
 @pytest.mark.skip(reason="GitHub actions build environments do not have ffmpeg")
 def test_photon_loss_pass_no_displacement(capsys):
     with capsys.disabled():
         num_qumodes = 1
         num_qubits_per_qumode = 4
         qmr = c2qa.QumodeRegister(num_qumodes, num_qubits_per_qumode)
         circuit = c2qa.CVCircuit(qmr)
@@ -314,15 +340,15 @@
 
         circuit.cv_d(0, qmr[0], duration=100, unit="ns")
 
         photon_loss_rate = 0.01
         time_unit = "ns"
         noise_pass = c2qa.kraus.PhotonLossNoisePass(photon_loss_rates=photon_loss_rate, circuit=circuit, time_unit=time_unit)
 
-        # state, result = c2qa.util.simulate(circuit, noise_passes=noise_pass)
+        # state, result, fock_counts = c2qa.util.simulate(circuit, noise_passes=noise_pass)
 
         wigner_filename = "tests/test_photon_loss_pass_no_displacement.mp4"
         c2qa.animate.animate_wigner(
             circuit,
             animation_segments=200,
             file=wigner_filename,
             noise_passes=noise_pass,
@@ -341,15 +367,15 @@
 
         circuit.cv_d(1.5, qmr[0], duration=100, unit="ns")
 
         photon_loss_rate = 0.02
         time_unit = "ns"
         noise_pass = c2qa.kraus.PhotonLossNoisePass(photon_loss_rates=photon_loss_rate, circuit=circuit, time_unit=time_unit)
 
-        # state, result = c2qa.util.simulate(circuit, noise_passes=noise_pass)
+        # state, result, fock_counts = c2qa.util.simulate(circuit, noise_passes=noise_pass)
 
         wigner_filename = "tests/test_photon_loss_pass_slow_displacement.mp4"
         c2qa.animate.animate_wigner(
             circuit,
             animation_segments=200,
             file=wigner_filename,
             noise_passes=noise_pass,
@@ -372,15 +398,15 @@
 
         circuit.cv_c_d(1, qmr[0], qbr[0], duration=100, unit="ns")
 
         photon_loss_rate = 0.02
         time_unit = "ns"
         noise_pass = c2qa.kraus.PhotonLossNoisePass(photon_loss_rates=photon_loss_rate, circuit=circuit, time_unit=time_unit)
 
-        # state, result = c2qa.util.simulate(circuit, noise_passes=noise_pass)
+        # state, result, fock_counts = c2qa.util.simulate(circuit, noise_passes=noise_pass)
 
         wigner_filename = "tests/test_photon_loss_pass_slow_conditional_displacement.mp4"
         c2qa.animate.animate_wigner(
             circuit,
             animation_segments=200,
             file=wigner_filename,
             noise_passes=noise_pass,
@@ -403,15 +429,15 @@
         circuit.cv_d(1, qmr[0], duration=100, unit="ns")
         circuit.cv_c_d(1, qmr[1], qbr[0], duration=100, unit="ns")
 
         photon_loss_rate = 0.02
         time_unit = "ns"
         noise_pass = c2qa.kraus.PhotonLossNoisePass(photon_loss_rates=photon_loss_rate, circuit=circuit, time_unit=time_unit, instructions=["cD"])
 
-        state, result = c2qa.util.simulate(circuit, noise_passes=noise_pass)
+        state, result, fock_counts = c2qa.util.simulate(circuit, noise_passes=noise_pass)
         assert result.success
 
 
 def test_photon_loss_qumode(capsys):
     with capsys.disabled():
         num_qumodes = 2
         num_qubits_per_qumode = 2
@@ -426,15 +452,15 @@
         circuit.cv_d(1, qmr[0], duration=100, unit="ns")
         circuit.cv_c_d(1, qmr[1], qbr[0], duration=100, unit="ns")
 
         photon_loss_rate = 0.02
         time_unit = "ns"
         noise_pass = c2qa.kraus.PhotonLossNoisePass(photon_loss_rates=photon_loss_rate, circuit=circuit, time_unit=time_unit, qumodes=qmr[1])
 
-        state, result = c2qa.util.simulate(circuit, noise_passes=noise_pass)
+        state, result, fock_counts = c2qa.util.simulate(circuit, noise_passes=noise_pass)
         assert result.success
 
 
 def test_photon_loss_instruction_qumode(capsys):
     with capsys.disabled():
         num_qumodes = 2
         num_qubits_per_qumode = 2
@@ -449,25 +475,25 @@
         circuit.cv_d(1, qmr[0], duration=100, unit="ns")
         circuit.cv_c_d(1, qmr[1], qbr[0], duration=100, unit="ns")
 
         photon_loss_rate = 0.02
         time_unit = "ns"
         noise_pass = c2qa.kraus.PhotonLossNoisePass(photon_loss_rates=photon_loss_rate, circuit=circuit, time_unit=time_unit, instructions=["cD"], qumodes=qmr[0])
 
-        state, result = c2qa.util.simulate(circuit, noise_passes=noise_pass)
+        state, result, fock_counts = c2qa.util.simulate(circuit, noise_passes=noise_pass)
         assert result.success
 
 
 def test_photon_loss_and_phase_damping(capsys):
     with capsys.disabled():
-        state_a, result_a = _build_photon_loss_and_amp_damping_circuit(0.0)
+        state_a, result_a, fock_counts = _build_photon_loss_and_amp_damping_circuit(0.0)
         print(state_a)
         assert result_a.success
 
-        state_b, result_b = _build_photon_loss_and_amp_damping_circuit(1.0)
+        state_b, result_b, fock_counts = _build_photon_loss_and_amp_damping_circuit(1.0)
         print(state_b)
         assert result_b.success
 
         assert not allclose(state_a, state_b)
     
 
 def _build_photon_loss_and_amp_damping_circuit(amp_damp = 0.3, photon_loss_rate = 0.01):
@@ -578,27 +604,27 @@
         circuit.cv_initialize(1, qmr[1])
         circuit.cv_bs(np.pi/4, qmr[0], qmr[1], duration=100, unit="ns")
         circuit.cv_bs(-np.pi/4, qmr[0], qmr[1], duration=100, unit="ns")
 
         photon_loss_rate = 10000000
         noise_pass = c2qa.kraus.PhotonLossNoisePass(photon_loss_rate, circuit)
 
-        fity_fifty = False
+        fifty_fifty = False
         print()
         for i in range(20):
             print("----------------------")
             print(f"Iteration {i}")
-            state_vector, result = c2qa.util.simulate(circuit, noise_passes=noise_pass)
+            state_vector, result, fock_counts = c2qa.util.simulate(circuit, noise_passes=noise_pass)
             # plot_histogram(result.get_counts(circuit), filename=f"tests/test_manual_validate_beamsplitter-{i}.png")
             occupation, fock_states = c2qa.util.stateread(state_vector, 0, num_qumodes, 2**num_qubits_per_qumode,verbose=True)
 
             for qumode_state, qubit_state, amplitude in fock_states:
                 # print(f"{qumode_state} {qubit_state} {amplitude}")
                 qumode1 = qumode_state[0]
                 qumode2 = qumode_state[1]
                 probability = amplitude**2
 
-                if (qumode1 == 1 and qumode2 == 0) or (qumode1 == 0 and qumode1 == 1) and probability == 0.5:
-                    fity_fifty = True
+                if (qumode1 == 1 and qumode2 == 0) or (qumode1 == 0 and qumode1 == 1) and math.isclose(probability, 0.5, 0.025):
+                    fifty_fifty = True
             
-        assert fity_fifty
+        assert fifty_fifty
```

### Comparing `bosonic-qiskit-8.1/tests/test_operators.py` & `bosonic-qiskit-9.0/tests/test_operators.py`

 * *Files identical despite different names*

### Comparing `bosonic-qiskit-8.1/tests/test_parameterized.py` & `bosonic-qiskit-9.0/tests/test_parameterized.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,15 +44,15 @@
         circuit, qmr, qr = create_conditional()
 
         alpha = qiskit.circuit.Parameter("alpha")
         circuit.cv_d(alpha, qmr[0])
 
         bound_circuit = circuit.bind_parameters({alpha: 3.14})
 
-        state, result = c2qa.util.simulate(bound_circuit)
+        state, result, fock_counts = c2qa.util.simulate(bound_circuit)
         assert_changed(state, result)
 
 
 def test_complex_literals(capsys):
     with capsys.disabled():
         # a = qiskit.circuit.Parameter('𝛼')
```

### Comparing `bosonic-qiskit-8.1/tests/test_qiskit.py` & `bosonic-qiskit-9.0/tests/test_qiskit.py`

 * *Files identical despite different names*

### Comparing `bosonic-qiskit-8.1/tests/test_wigner.py` & `bosonic-qiskit-9.0/tests/test_wigner.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,30 +17,30 @@
 
         # qr[0] will init to zero
         circuit.cv_initialize(0, qmr[0])
 
         circuit.h(qr[0])
         circuit.cv_c_d(dist, qmr[0], qr[0])
 
-        state, _ = c2qa.util.simulate(circuit)
+        state, result, fock_counts = c2qa.util.simulate(circuit)
         trace = c2qa.util.trace_out_qubits(circuit, state)
         c2qa.wigner.plot_wigner(circuit, trace, file="tests/zero.png", trace=False)
 
 
 def test_plot_one(capsys):
     with capsys.disabled():
         qmr = c2qa.QumodeRegister(num_qumodes=1, num_qubits_per_qumode=2)
         qr = qiskit.QuantumRegister(size=1)
         cr = qiskit.ClassicalRegister(size=1)
         circuit = c2qa.CVCircuit(qmr, qr, cr)
 
         # qr[0] and cr[0] will init to zero
         circuit.cv_initialize(1, qmr[0])
 
-        state, _ = c2qa.util.simulate(circuit)
+        state, result, fock_counts = c2qa.util.simulate(circuit)
         # print("Qumode initialized to one:")
         # print(state)
         c2qa.wigner.plot_wigner(circuit, state, file="tests/one.png")
 
 
 def test_plot_wigner_projection(capsys):
     with capsys.disabled():
@@ -77,15 +77,15 @@
 
         circuit.h(qr[0])
         circuit.cv_c_d(dist, qmr[0], qr[0])
         circuit.h(qr[0])
         circuit.measure(qr[0], cr[0])
 
         # conditional_state_vector=True will return two state vectors, one for 0 and 1 classical register value
-        state, _ = c2qa.util.simulate(circuit, conditional_state_vector=True)
+        state, result, fock_counts = c2qa.util.simulate(circuit, conditional_state_vector=True)
         even_state = state["0x0"]
         odd_state = state["0x1"]
 
         wigner_filename = "tests/cat_wigner_even.png"
         c2qa.wigner.plot_wigner(
             circuit,
             even_state,
@@ -134,16 +134,16 @@
         circuit.initialize([1, 0], qr[0])
         circuit.cv_initialize(0, qmr[0])
 
         circuit.h(qr[0])
         circuit.cv_c_d(dist, qmr[0], qr[0])
         circuit.h(qr[0])
 
-        states, result = c2qa.util.simulate(circuit, per_shot_state_vector=True)
-        wigner = c2qa.wigner.wigner_mle(states)
+        state, result, fock_counts = c2qa.util.simulate(circuit, per_shot_state_vector=True)
+        wigner = c2qa.wigner.wigner_mle(state)
         assert wigner is not None
         print(wigner)
 
 
 def test_plot_wigner_snapshot(capsys):
     with capsys.disabled():
         num_qubits_per_qumode = 4
@@ -168,15 +168,15 @@
 
         circuit.cv_snapshot()
 
         circuit.h(qr[0])
 
         circuit.cv_snapshot()
 
-        state, result = c2qa.util.simulate(circuit)
+        state, result, fock_counts = c2qa.util.simulate(circuit)
 
         c2qa.wigner.plot_wigner_snapshot(circuit, result, "tests")
 
 
 def test_plot_zero_contour(capsys):
     with capsys.disabled():
         data = numpy.zeros((200, 200)).tolist()
```

