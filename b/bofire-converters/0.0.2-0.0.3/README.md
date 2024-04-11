# Comparing `tmp/bofire_converters-0.0.2.tar.gz` & `tmp/bofire_converters-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bofire_converters-0.0.2.tar", last modified: Tue Jul  4 13:08:19 2023, max compression
+gzip compressed data, was "bofire_converters-0.0.3.tar", last modified: Thu Apr 11 13:54:25 2024, max compression
```

## Comparing `bofire_converters-0.0.2.tar` & `bofire_converters-0.0.3.tar`

### file list

```diff
@@ -1,20 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-07-04 13:08:19.626971 bofire_converters-0.0.2/
--rw-rw-rw-   0        0        0      390 2023-06-21 18:09:51.000000 bofire_converters-0.0.2/.pre-commit-config.yaml
--rw-rw-rw-   0        0        0     1534 2023-04-24 08:46:39.000000 bofire_converters-0.0.2/LICENSE
--rw-rw-rw-   0        0        0     3284 2023-07-04 13:08:19.626971 bofire_converters-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      960 2023-07-04 13:06:43.000000 bofire_converters-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-07-04 13:08:19.580090 bofire_converters-0.0.2/bofire_converters/
--rw-rw-rw-   0        0        0        0 2023-04-27 13:01:22.000000 bofire_converters-0.0.2/bofire_converters/__init__.py
--rw-rw-rw-   0        0        0     8790 2023-07-04 10:22:09.000000 bofire_converters-0.0.2/bofire_converters/opti_to_domain.py
--rw-rw-rw-   0        0        0      215 2023-07-04 13:08:19.000000 bofire_converters-0.0.2/bofire_converters/version.py
-drwxrwxrwx   0        0        0        0 2023-07-04 13:08:19.611348 bofire_converters-0.0.2/bofire_converters.egg-info/
--rw-rw-rw-   0        0        0     3284 2023-07-04 13:08:19.000000 bofire_converters-0.0.2/bofire_converters.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      400 2023-07-04 13:08:19.000000 bofire_converters-0.0.2/bofire_converters.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-04 13:08:19.000000 bofire_converters-0.0.2/bofire_converters.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2023-07-04 13:08:19.000000 bofire_converters-0.0.2/bofire_converters.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-07-04 13:08:19.000000 bofire_converters-0.0.2/bofire_converters.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1197 2023-07-04 13:07:43.000000 bofire_converters-0.0.2/pyproject.toml
--rw-rw-rw-   0        0        0      119 2023-04-27 12:57:50.000000 bofire_converters-0.0.2/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-07-04 13:08:19.626971 bofire_converters-0.0.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-04 13:08:19.626971 bofire_converters-0.0.2/test/
--rw-rw-rw-   0        0        0     4322 2023-04-28 16:04:59.000000 bofire_converters-0.0.2/test/test_opti_to_domain.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:54:25.679065 bofire_converters-0.0.3/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:54:25.675065 bofire_converters-0.0.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:54:25.675065 bofire_converters-0.0.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      830 2024-04-11 13:54:17.000000 bofire_converters-0.0.3/.github/workflows/lint.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      755 2024-04-11 13:54:17.000000 bofire_converters-0.0.3/.github/workflows/publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      553 2024-04-11 13:54:17.000000 bofire_converters-0.0.3/.github/workflows/test.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-11 13:54:17.000000 bofire_converters-0.0.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-11 13:54:17.000000 bofire_converters-0.0.3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-04-11 13:54:17.000000 bofire_converters-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3326 2024-04-11 13:54:25.679065 bofire_converters-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      940 2024-04-11 13:54:17.000000 bofire_converters-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:54:25.675065 bofire_converters-0.0.3/bofire_converters/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 13:54:17.000000 bofire_converters-0.0.3/bofire_converters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9739 2024-04-11 13:54:17.000000 bofire_converters-0.0.3/bofire_converters/opti_to_domain.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-11 13:54:25.000000 bofire_converters-0.0.3/bofire_converters/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:54:25.675065 bofire_converters-0.0.3/bofire_converters.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3326 2024-04-11 13:54:25.000000 bofire_converters-0.0.3/bofire_converters.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      525 2024-04-11 13:54:25.000000 bofire_converters-0.0.3/bofire_converters.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 13:54:25.000000 bofire_converters-0.0.3/bofire_converters.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-11 13:54:25.000000 bofire_converters-0.0.3/bofire_converters.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-11 13:54:25.000000 bofire_converters-0.0.3/bofire_converters.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-04-11 13:54:17.000000 bofire_converters-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-11 13:54:17.000000 bofire_converters-0.0.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 13:54:25.679065 bofire_converters-0.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:54:25.675065 bofire_converters-0.0.3/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     4251 2024-04-11 13:54:17.000000 bofire_converters-0.0.3/test/test_opti_to_domain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-04-11 13:54:17.000000 bofire_converters-0.0.3/test/test_pyprojecttoml.py
```

### Comparing `bofire_converters-0.0.2/LICENSE` & `bofire_converters-0.0.3/LICENSE`

 * *Ordering differences only*

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,28 @@
-BSD 3-Clause License
-
-Copyright (c) 2023, experimental-design
-
-Redistribution and use in source and binary forms, with or without
-modification, are permitted provided that the following conditions are met:
-
-1. Redistributions of source code must retain the above copyright notice, this
-   list of conditions and the following disclaimer.
-
-2. Redistributions in binary form must reproduce the above copyright notice,
-   this list of conditions and the following disclaimer in the documentation
-   and/or other materials provided with the distribution.
-
-3. Neither the name of the copyright holder nor the names of its
-   contributors may be used to endorse or promote products derived from
-   this software without specific prior written permission.
-
-THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
-AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
-IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
-DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
-FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
-DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
-SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
-CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
-OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
-OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+BSD 3-Clause License
+
+Copyright (c) 2023, experimental-design
+
+Redistribution and use in source and binary forms, with or without
+modification, are permitted provided that the following conditions are met:
+
+1. Redistributions of source code must retain the above copyright notice, this
+   list of conditions and the following disclaimer.
+
+2. Redistributions in binary form must reproduce the above copyright notice,
+   this list of conditions and the following disclaimer in the documentation
+   and/or other materials provided with the distribution.
+
+3. Neither the name of the copyright holder nor the names of its
+   contributors may be used to endorse or promote products derived from
+   this software without specific prior written permission.
+
+THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
+DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
+FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
+DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
+SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
+CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
+OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
+OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
```

### Comparing `bofire_converters-0.0.2/PKG-INFO` & `bofire_converters-0.0.3/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,64 +1,67 @@
-Metadata-Version: 2.1
-Name: bofire_converters
-Version: 0.0.2
-License: BSD 3-Clause License
-        
-        Copyright (c) 2023, experimental-design
-        
-        Redistribution and use in source and binary forms, with or without
-        modification, are permitted provided that the following conditions are met:
-        
-        1. Redistributions of source code must retain the above copyright notice, this
-           list of conditions and the following disclaimer.
-        
-        2. Redistributions in binary form must reproduce the above copyright notice,
-           this list of conditions and the following disclaimer in the documentation
-           and/or other materials provided with the distribution.
-        
-        3. Neither the name of the copyright holder nor the names of its
-           contributors may be used to endorse or promote products derived from
-           this software without specific prior written permission.
-        
-        THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
-        AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
-        IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
-        DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
-        FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
-        DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
-        SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
-        CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
-        OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
-        OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
-        
-Project-URL: Homepage, https://github.com/experimental-design/bofire-converters
-Classifier: Development Status :: 1 - Planning
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Topic :: Scientific/Engineering
-Classifier: Intended Audience :: Science/Research
-Classifier: Intended Audience :: Developers
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-Provides-Extra: test
-License-File: LICENSE
-
-# Mopti Problem to Bofire Domain Converter
-
-These tools are to help with migration of legacy applications from [Mopti](https://github.com/basf/mopti) to [BoFire](https://github.com/experimental-design/bofire). Mopti is for defining optimization problems (inputs, outputs, constraints, ...) and has some sampling utilities. If you have a _problem_ defined in the Mopti format, `bofire_converters` can help you to create the corresponding BoFire object, which is called a _domain_.
-
-## Quick start
-
-Install via pip
-
-`pip install bofire-converters`
-
-Here is an example of converting a `Problem` object from [Mopti](https://github.com/basf/mopti) to a BoFire `Domain`.
-
-```python
-from bofire_converters.opti_to_domain import convert_problem
-from opti.problems.multi import Daechert1
-
-# Use one of the opti built-in problems as an example
-my_opti_problem = Daechert1()                    
-my_bofire_domain = convert_problem(my_opti_problem)
-```
+Metadata-Version: 2.1
+Name: bofire_converters
+Version: 0.0.3
+License: BSD 3-Clause License
+        
+        Copyright (c) 2023, experimental-design
+        
+        Redistribution and use in source and binary forms, with or without
+        modification, are permitted provided that the following conditions are met:
+        
+        1. Redistributions of source code must retain the above copyright notice, this
+           list of conditions and the following disclaimer.
+        
+        2. Redistributions in binary form must reproduce the above copyright notice,
+           this list of conditions and the following disclaimer in the documentation
+           and/or other materials provided with the distribution.
+        
+        3. Neither the name of the copyright holder nor the names of its
+           contributors may be used to endorse or promote products derived from
+           this software without specific prior written permission.
+        
+        THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+        AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+        IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
+        DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
+        FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
+        DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
+        SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
+        CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
+        OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
+        OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+        
+Project-URL: Homepage, https://github.com/experimental-design/bofire-converters
+Classifier: Development Status :: 1 - Planning
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Topic :: Scientific/Engineering
+Classifier: Intended Audience :: Science/Research
+Classifier: Intended Audience :: Developers
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: mopti>=0.10.10
+Requires-Dist: bofire>=0.0.12
+Provides-Extra: test
+Requires-Dist: pytest>=8.1.1; extra == "test"
+
+# Mopti Problem to Bofire Domain Converter
+
+These tools are to help with migration of legacy applications from [Mopti](https://github.com/basf/mopti) to [BoFire](https://github.com/experimental-design/bofire). Mopti is for defining optimization problems (inputs, outputs, constraints, ...) and has some sampling utilities. If you have a _problem_ defined in the Mopti format, `bofire_converters` can help you to create the corresponding BoFire object, which is called a _domain_.
+
+## Quick start
+
+Install via pip
+
+`pip install bofire-converters`
+
+Here is an example of converting a `Problem` object from [Mopti](https://github.com/basf/mopti) to a BoFire `Domain`.
+
+```python
+from bofire_converters.opti_to_domain import convert_problem
+from opti.problems.multi import Daechert1
+
+# Use one of the opti built-in problems as an example
+my_opti_problem = Daechert1()                    
+my_bofire_domain = convert_problem(my_opti_problem)
+```
```

### Comparing `bofire_converters-0.0.2/bofire_converters/opti_to_domain.py` & `bofire_converters-0.0.3/bofire_converters/opti_to_domain.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,250 +1,268 @@
-from typing import List, Optional
-from warnings import warn
-
-from bofire.data_models.constraints.api import (
-    Constraint,
-    LinearEqualityConstraint,
-    LinearInequalityConstraint,
-    NChooseKConstraint,
-    NonlinearEqualityConstraint,
-    NonlinearInequalityConstraint,
-)
-from bofire.data_models.domain.api import Domain
-from bofire.data_models.features.api import (
-    CategoricalInput,
-    CategoricalOutput,
-    ContinuousInput,
-    ContinuousOutput,
-    DiscreteInput,
-    Output,
-)
-from bofire.data_models.objectives.api import (
-    CloseToTargetObjective,
-    MaximizeObjective,
-    MinimizeObjective,
-)
-from opti import (
-    CloseToTarget,
-    Maximize,
-    Minimize,
-    Objectives,
-    Parameters,
-    Problem,
-)
-from opti.constraint import (
-    Constraints,
-    LinearEquality,
-    LinearInequality,
-    NChooseK,
-    NonlinearEquality,
-    NonlinearInequality,
-)
-
-
-def convert_inputs(inputs: Parameters) -> List:
-    """Make the Bofire equivalent to an inputs objects from (m)opti
-
-    Parameters:
-        inputs: The inputs from an opti problem generated using
-        Parameters
-
-    Returns:
-        List of BoFire parameters, eg, ContinuousInput
-
-    Examples:
-        # Parameters, Discrete, Continuous and Categorical are from mopti
-        inputs = Parameters(
-            [
-                Discrete("x1", domain=[0.0, 1.0, 2.0, 3.0]),
-                Continuous("x2", domain=[-2.0, 2.0]),
-                Continuous("x3", domain=[-2.0, 2.0]),
-                Continuous("x4", domain=[-2.0, 2.0]),
-                Categorical("x5", domain=["cat", "dog", "monkey"]),
-            ]
-        )
-        convert_inputs(inputs)
-    """
-    convert_types = {
-        "discrete": {"type": DiscreteInput, "domain": "values"},
-        "continuous": {"type": ContinuousInput, "domain": "bounds"},
-        "categorical": {"type": CategoricalInput, "domain": "categories"},
-    }
-
-    d_inputs = []
-    for key, value in inputs.parameters.items():
-        kwargs = {"key": key, convert_types[value.type]["domain"]: value.domain}
-        d_type = convert_types[value.type]["type"](**kwargs)
-        d_inputs.append(d_type)
-    return d_inputs
-
-
-def convert_outputs_and_objectives(
-    outputs: Parameters,
-    objectives: Objectives,
-    output_constraints: Optional[Objectives] = None,
-) -> List[Output]:
-    """Make BoFire outputs from opti outputs and objectives
-
-    opti specifies experimental outputs, which are quantities to be observed
-    and (at least) predicted, and also objectives, which refer by name to the
-    outputs. Bofire does it differently; objectives are specified within
-    outputs so that a list of bofire outputs contains the same information as both
-    outputs and objectives from opti. Furthermore, opti allows output constraints,
-    which in this function are converted to objectives.
-
-    Questions about parameters and tolerances:
-    https://github.com/experimental-design/bofire/issues/77#issuecomment-1521418422
-
-    Parameters:
-        outputs: outputs from opti. These are quantities that get modelled and are
-            usually generated using the Parameters function from opti.
-        objectives: objectives from opti. These refer to the names of the
-            outputs to determine what is to be optimized
-
-    Returns:
-        List of BoFire outputs
-    """
-    # Treat output constraints from opti problems like objectives
-    if output_constraints is not None:
-        objectives = Objectives(objectives.objectives + output_constraints.objectives)
-
-    # create a dict where each key is an output and the values are the objectives in which
-    # that output appears
-    outs_and_objs = {
-        opti_out.name: [obj for obj in objectives if obj.name == opti_out.name]
-        for opti_out in outputs
-    }
-
-    output_list = []
-    for out, objs in outs_and_objs.items():
-        objs = [None] if len(objs) == 0 else objs
-        for idx, obj in enumerate(objs):
-            bof_obj = None
-            if isinstance(obj, CloseToTarget):
-                bof_obj = CloseToTargetObjective(
-                    target_value=obj.target, exponent=obj.exponent
-                )
-            elif isinstance(obj, Maximize):
-                bof_obj = MaximizeObjective()
-            elif isinstance(obj, Minimize):
-                bof_obj = MinimizeObjective()
-            elif obj is not None:
-                raise Exception("Unhandled objective type: {type(obj)}")
-
-            # if there are multiple objectives associated with a single input,
-            # give the resulting outputs in the bofire domain different names
-            if len(objs) > 1:
-                suffix = f"_{idx}"
-            else:
-                suffix = ""
-
-            if outputs[out].type == "continuous":
-                bof_out = ContinuousOutput(key=f"{out}{suffix}", objective=bof_obj)
-            elif outputs[out].type == "discrete":
-                warn(f"{out} has been converted to a continuous output.")
-                bof_out = ContinuousOutput(key=f"{out}{suffix}", objective=bof_obj)
-            elif outputs[out].type == "categorical":
-                bof_out = CategoricalOutput(
-                    key=f"{out}{suffix}",
-                    type="CategoricalOutput",
-                    categories=outputs[out].domain,
-                    objective=[
-                        1.0 / len(outputs[out].domain) for _ in outputs[out].domain
-                    ],
-                )
-            else:
-                raise Exception(f"Unhandled output type: {outputs[out].type}")
-
-            output_list.append(bof_out)
-
-    return output_list
-
-
-def convert_constraints(opti_constraints: Constraints) -> List[Constraint]:
-    """opti constraints to bofire constraints
-
-    Parameters:
-        opti_constraints: The constraints to be converted
-
-    Returns:
-        List of bofire constraints
-    """
-    domain_constraints = []
-    for cnstr in opti_constraints.get(types=LinearEquality):
-        domain_constraints.append(
-            LinearEqualityConstraint(
-                features=cnstr.names, coefficients=cnstr.lhs.tolist(), rhs=cnstr.rhs
-            )
-        )
-    for cnstr in opti_constraints.get(types=LinearInequality):
-        domain_constraints.append(
-            LinearInequalityConstraint(
-                features=cnstr.names, coefficients=cnstr.lhs.tolist(), rhs=cnstr.rhs
-            )
-        )
-    for cnstr in opti_constraints.get(types=NonlinearEquality):
-        domain_constraints.append(
-            NonlinearEqualityConstraint(expression=cnstr.expression)
-        )
-    for cnstr in opti_constraints.get(types=NonlinearInequality):
-        domain_constraints.append(
-            NonlinearInequalityConstraint(expression=cnstr.expression)
-        )
-    for cnstr in opti_constraints.get(types=NChooseK):
-        domain_constraints.append(
-            NChooseKConstraint(
-                features=cnstr.names,
-                min_count=0,
-                max_count=cnstr.max_active,
-                none_also_valid=True,
-            )
-        )
-
-    return domain_constraints
-
-
-def convert_problem(opti_problem: Problem) -> Domain:
-    """Turn an opti problem into the equivalent bofire domain
-
-    Parameters:
-        opti_problem: Problem object from opti for conversion
-
-    Returns:
-        Domain, able to be used as a problem definition by bofire.
-
-    Examples:
-    myproblem = Problem(
-                    inputs=Parameters(
-                        [Continuous('x1', domain=[78.0, 102.0]),
-                         Continuous('x2', domain=[33.0, 45.0])]
-                    ),
-                    outputs=Parameters(
-                        [Continuous('y0')]
-                    ),
-                    objectives=Objectives(
-                    [Minimize('y0')]
-                    ),
-                    constraints=Constraints(
-                        [NonlinearInequality('(85.334407 + 0.0056858 * x2 * x1 ) - 92.0')]
-                    ),
-                )
-    mydomain = convert_problem(myproblem)
-    """
-
-    domain_inputs = convert_inputs(opti_problem.inputs)
-    if opti_problem.constraints is not None:
-        domain_constraints = convert_constraints(opti_problem.constraints)
-    else:
-        domain_constraints = None
-
-    domain_outputs = convert_outputs_and_objectives(
-        opti_problem.outputs, opti_problem.objectives, opti_problem.output_constraints
-    )
-
-    bofire_domain = Domain.from_lists(
-        inputs=domain_inputs,
-        outputs=domain_outputs,
-        constraints=domain_constraints,
-    )
-
-    return bofire_domain
+from typing import Dict, List, Optional, cast
+from warnings import warn
+
+import opti
+import opti.objective as opti_o
+import opti.parameter as opti_p
+from bofire.data_models.constraints.api import (
+    AnyConstraint,
+    LinearEqualityConstraint,
+    LinearInequalityConstraint,
+    NChooseKConstraint,
+    NonlinearEqualityConstraint,
+    NonlinearInequalityConstraint,
+)
+from bofire.data_models.domain.api import Domain
+from bofire.data_models.features.api import (
+    AnyOutput,
+    CategoricalInput,
+    CategoricalOutput,
+    ContinuousInput,
+    ContinuousOutput,
+    DiscreteInput,
+)
+from bofire.data_models.objectives.api import (
+    AnyCategoricalObjective,
+    AnyObjective,
+    CloseToTargetObjective,
+    ConstrainedCategoricalObjective,
+    MaximizeObjective,
+    MinimizeObjective,
+)
+
+
+def convert_inputs(inputs: opti.Parameters) -> List:
+    """Make the Bofire equivalent to an inputs objects from (m)opti
+
+    Parameters:
+        inputs: The inputs from an opti problem generated using
+        Parameters
+
+    Returns:
+        List of BoFire parameters, eg, ContinuousInput
+
+    Examples:
+        # Parameters, Discrete, Continuous and Categorical are from mopti
+        inputs = Parameters(
+            [
+                Discrete("x1", domain=[0.0, 1.0, 2.0, 3.0]),
+                Continuous("x2", domain=[-2.0, 2.0]),
+                Continuous("x3", domain=[-2.0, 2.0]),
+                Continuous("x4", domain=[-2.0, 2.0]),
+                Categorical("x5", domain=["cat", "dog", "monkey"]),
+            ]
+        )
+        convert_inputs(inputs)
+    """
+    convert_types = {
+        "discrete": {"type": DiscreteInput, "domain": "values"},
+        "continuous": {"type": ContinuousInput, "domain": "bounds"},
+        "categorical": {"type": CategoricalInput, "domain": "categories"},
+    }
+
+    d_inputs = []
+    for key, value in inputs.parameters.items():
+        kwargs = {"key": key, convert_types[value.type]["domain"]: value.domain}
+        d_type = convert_types[value.type]["type"](**kwargs)
+        d_inputs.append(d_type)
+    return d_inputs
+
+
+def _convert_obj_cont_disc(obj: opti_o.Objective) -> AnyObjective:
+    if isinstance(obj, opti.CloseToTarget):
+        return CloseToTargetObjective(target_value=obj.target, exponent=obj.exponent)
+    elif isinstance(obj, opti.Maximize):
+        return MaximizeObjective()
+    elif isinstance(obj, opti.Minimize):
+        return MinimizeObjective()
+    elif isinstance(obj, opti.CloseToTarget):
+        return CloseToTargetObjective(target_value=obj.target, exponent=obj.exponent)
+    elif obj is not None:
+        raise Exception("Unhandled objective type: {type(obj)}")
+
+
+def _convert_obj_cat(
+    parameter_domain: List[str], obj: opti_o.Objective
+) -> AnyCategoricalObjective:
+    if isinstance(obj, opti.CloseToTarget):
+        domain = cast(List[str], parameter_domain)
+        return ConstrainedCategoricalObjective(
+            categories=domain, desirability=[d == obj.target for d in domain]
+        )
+    elif isinstance(obj, opti.Maximize):
+        raise ValueError("cannot maximize categorical output")
+    elif isinstance(obj, opti.Minimize):
+        raise ValueError("cannot minimize categorical output")
+    elif obj is not None:
+        raise Exception("Unhandled objective type: {type(obj)}")
+
+
+def convert_outputs_and_objectives(
+    outputs: opti.Parameters,
+    objectives: opti.Objectives,
+    output_constraints: Optional[opti.Objectives] = None,
+) -> List[AnyOutput]:
+    """Make BoFire outputs from opti outputs and objectives
+
+    opti specifies experimental outputs, which are quantities to be observed
+    and (at least) predicted, and also objectives, which refer by name to the
+    outputs. Bofire does it differently; objectives are specified within
+    outputs so that a list of bofire outputs contains the same information as both
+    outputs and objectives from opti. Furthermore, opti allows output constraints,
+    which in this function are converted to objectives.
+
+    Questions about parameters and tolerances:
+    https://github.com/experimental-design/bofire/issues/77#issuecomment-1521418422
+
+    Parameters:
+        outputs: outputs from opti. These are quantities that get modelled and are
+            usually generated using the Parameters function from opti.
+        objectives: objectives from opti. These refer to the names of the
+            outputs to determine what is to be optimized
+
+    Returns:
+        List of BoFire outputs
+    """
+    # Treat output constraints from opti problems like objectives
+    if output_constraints is not None:
+        objectives = opti.Objectives(
+            objectives.objectives + output_constraints.objectives
+        )
+
+    # create a dict where each key is an output and the values are the objectives in which
+    # that output appears
+    outs_and_objs: Dict[str, List[opti_o.Objective]] = {
+        opti_out.name: [obj for obj in objectives if obj.name == opti_out.name]
+        for opti_out in outputs
+    }
+
+    output_list = []
+    for out_name, objs in outs_and_objs.items():
+        objs = [None] if len(objs) == 0 else objs
+        for idx, obj in enumerate(objs):
+            # if there are multiple objectives associated with a single input,
+            # give the resulting outputs in the bofire domain different names
+            if len(objs) > 1:
+                suffix = f"_{idx}"
+            else:
+                suffix = ""
+
+            output: opti_p.Parameter = outputs[out_name]
+
+            if output.type == "continuous":
+                bof_obj = obj and _convert_obj_cont_disc(obj)
+                bof_out = ContinuousOutput(key=f"{out_name}{suffix}", objective=bof_obj)
+            elif output.type == "discrete":
+                warn(f"{out_name} has been converted to a continuous output.")
+                bof_obj = obj and _convert_obj_cont_disc(obj)
+                bof_out = ContinuousOutput(key=f"{out_name}{suffix}", objective=bof_obj)
+            elif output.type == "categorical":
+                domain = cast(List[str], output.domain)
+                if obj is None:
+                    bof_obj = ConstrainedCategoricalObjective(
+                        categories=domain, desirability=[True] * len(domain)
+                    )
+                else:
+                    bof_obj = _convert_obj_cat(domain, obj)
+                bof_out = CategoricalOutput(
+                    key=f"{out_name}{suffix}",
+                    type="CategoricalOutput",
+                    categories=domain,
+                    objective=bof_obj,
+                )
+            else:
+                raise Exception(f"Unhandled output type: {outputs[out_name].type}")
+
+            output_list.append(bof_out)
+
+    return output_list
+
+
+def convert_constraints(opti_constraints: opti.Constraints) -> List[AnyConstraint]:
+    """opti constraints to bofire constraints
+
+    Parameters:
+        opti_constraints: The constraints to be converted
+
+    Returns:
+        List of bofire constraints
+    """
+    domain_constraints = []
+    for cnstr in opti_constraints.get(types=opti.LinearEquality):
+        domain_constraints.append(
+            LinearEqualityConstraint(
+                features=cnstr.names, coefficients=cnstr.lhs.tolist(), rhs=cnstr.rhs
+            )
+        )
+    for cnstr in opti_constraints.get(types=opti.LinearInequality):
+        domain_constraints.append(
+            LinearInequalityConstraint(
+                features=cnstr.names, coefficients=cnstr.lhs.tolist(), rhs=cnstr.rhs
+            )
+        )
+    for cnstr in opti_constraints.get(types=opti.NonlinearEquality):
+        domain_constraints.append(
+            NonlinearEqualityConstraint(expression=cnstr.expression)
+        )
+    for cnstr in opti_constraints.get(types=opti.NonlinearInequality):
+        domain_constraints.append(
+            NonlinearInequalityConstraint(expression=cnstr.expression)
+        )
+    for cnstr in opti_constraints.get(types=opti.NChooseK):
+        domain_constraints.append(
+            NChooseKConstraint(
+                features=cnstr.names,
+                min_count=0,
+                max_count=cnstr.max_active,
+                none_also_valid=True,
+            )
+        )
+
+    return domain_constraints
+
+
+def convert_problem(opti_problem: opti.Problem) -> Domain:
+    """Turn an opti problem into the equivalent bofire domain
+
+    Parameters:
+        opti_problem: Problem object from opti for conversion
+
+    Returns:
+        Domain, able to be used as a problem definition by bofire.
+
+    Examples:
+    myproblem = Problem(
+                    inputs=Parameters(
+                        [Continuous('x1', domain=[78.0, 102.0]),
+                         Continuous('x2', domain=[33.0, 45.0])]
+                    ),
+                    outputs=Parameters(
+                        [Continuous('y0')]
+                    ),
+                    objectives=Objectives(
+                    [Minimize('y0')]
+                    ),
+                    constraints=Constraints(
+                        [NonlinearInequality('(85.334407 + 0.0056858 * x2 * x1 ) - 92.0')]
+                    ),
+                )
+    mydomain = convert_problem(myproblem)
+    """
+
+    domain_inputs = convert_inputs(opti_problem.inputs)
+    if opti_problem.constraints is not None:
+        domain_constraints = convert_constraints(opti_problem.constraints)
+    else:
+        domain_constraints = None
+
+    domain_outputs = convert_outputs_and_objectives(
+        opti_problem.outputs, opti_problem.objectives, opti_problem.output_constraints
+    )
+
+    bofire_domain = Domain.from_lists(
+        inputs=domain_inputs,
+        outputs=list(domain_outputs),
+        constraints=domain_constraints and list(domain_constraints),
+    )
+
+    return bofire_domain
```

### Comparing `bofire_converters-0.0.2/bofire_converters.egg-info/PKG-INFO` & `bofire_converters-0.0.3/bofire_converters.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,64 +1,67 @@
-Metadata-Version: 2.1
-Name: bofire-converters
-Version: 0.0.2
-License: BSD 3-Clause License
-        
-        Copyright (c) 2023, experimental-design
-        
-        Redistribution and use in source and binary forms, with or without
-        modification, are permitted provided that the following conditions are met:
-        
-        1. Redistributions of source code must retain the above copyright notice, this
-           list of conditions and the following disclaimer.
-        
-        2. Redistributions in binary form must reproduce the above copyright notice,
-           this list of conditions and the following disclaimer in the documentation
-           and/or other materials provided with the distribution.
-        
-        3. Neither the name of the copyright holder nor the names of its
-           contributors may be used to endorse or promote products derived from
-           this software without specific prior written permission.
-        
-        THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
-        AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
-        IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
-        DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
-        FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
-        DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
-        SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
-        CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
-        OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
-        OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
-        
-Project-URL: Homepage, https://github.com/experimental-design/bofire-converters
-Classifier: Development Status :: 1 - Planning
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Topic :: Scientific/Engineering
-Classifier: Intended Audience :: Science/Research
-Classifier: Intended Audience :: Developers
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-Provides-Extra: test
-License-File: LICENSE
-
-# Mopti Problem to Bofire Domain Converter
-
-These tools are to help with migration of legacy applications from [Mopti](https://github.com/basf/mopti) to [BoFire](https://github.com/experimental-design/bofire). Mopti is for defining optimization problems (inputs, outputs, constraints, ...) and has some sampling utilities. If you have a _problem_ defined in the Mopti format, `bofire_converters` can help you to create the corresponding BoFire object, which is called a _domain_.
-
-## Quick start
-
-Install via pip
-
-`pip install bofire-converters`
-
-Here is an example of converting a `Problem` object from [Mopti](https://github.com/basf/mopti) to a BoFire `Domain`.
-
-```python
-from bofire_converters.opti_to_domain import convert_problem
-from opti.problems.multi import Daechert1
-
-# Use one of the opti built-in problems as an example
-my_opti_problem = Daechert1()                    
-my_bofire_domain = convert_problem(my_opti_problem)
-```
+Metadata-Version: 2.1
+Name: bofire_converters
+Version: 0.0.3
+License: BSD 3-Clause License
+        
+        Copyright (c) 2023, experimental-design
+        
+        Redistribution and use in source and binary forms, with or without
+        modification, are permitted provided that the following conditions are met:
+        
+        1. Redistributions of source code must retain the above copyright notice, this
+           list of conditions and the following disclaimer.
+        
+        2. Redistributions in binary form must reproduce the above copyright notice,
+           this list of conditions and the following disclaimer in the documentation
+           and/or other materials provided with the distribution.
+        
+        3. Neither the name of the copyright holder nor the names of its
+           contributors may be used to endorse or promote products derived from
+           this software without specific prior written permission.
+        
+        THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+        AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+        IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
+        DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
+        FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
+        DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
+        SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
+        CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
+        OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
+        OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+        
+Project-URL: Homepage, https://github.com/experimental-design/bofire-converters
+Classifier: Development Status :: 1 - Planning
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Topic :: Scientific/Engineering
+Classifier: Intended Audience :: Science/Research
+Classifier: Intended Audience :: Developers
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: mopti>=0.10.10
+Requires-Dist: bofire>=0.0.12
+Provides-Extra: test
+Requires-Dist: pytest>=8.1.1; extra == "test"
+
+# Mopti Problem to Bofire Domain Converter
+
+These tools are to help with migration of legacy applications from [Mopti](https://github.com/basf/mopti) to [BoFire](https://github.com/experimental-design/bofire). Mopti is for defining optimization problems (inputs, outputs, constraints, ...) and has some sampling utilities. If you have a _problem_ defined in the Mopti format, `bofire_converters` can help you to create the corresponding BoFire object, which is called a _domain_.
+
+## Quick start
+
+Install via pip
+
+`pip install bofire-converters`
+
+Here is an example of converting a `Problem` object from [Mopti](https://github.com/basf/mopti) to a BoFire `Domain`.
+
+```python
+from bofire_converters.opti_to_domain import convert_problem
+from opti.problems.multi import Daechert1
+
+# Use one of the opti built-in problems as an example
+my_opti_problem = Daechert1()                    
+my_bofire_domain = convert_problem(my_opti_problem)
+```
```

### Comparing `bofire_converters-0.0.2/pyproject.toml` & `bofire_converters-0.0.3/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,47 +1,48 @@
-[build-system]
-requires = ["setuptools", "setuptools_scm[toml]", "wheel"]
-build-backend = "setuptools.build_meta"
-
-[tool.setuptools_scm]
-local_scheme = "node-and-date"
-write_to = "./bofire_converters/version.py"
-
-[tool.ruff]
-ignore = [
-    "E501",  # don't enforce for comments and docstrings
-    "B017",  # required for tests
-    "B027",  # required for optional _tell method
-    "B028",
-    "B904",
-    "B905"
-]
-line-length = 88
-select = ["B", "C", "E", "F", "W", "I"]
-
-[tool.ruff.mccabe]
-max-complexity = 18
-
-[project]
-name = "bofire_converters"
-version = "0.0.2"
-license = { file = "LICENSE" }
-readme = "README.md"
-requires-python = ">=3.7"
-classifiers = ["Development Status :: 1 - Planning",
-        "Programming Language :: Python :: 3 :: Only",
-        "License :: OSI Approved :: BSD License",
-        "Topic :: Scientific/Engineering",
-        "Intended Audience :: Science/Research",
-        "Intended Audience :: Developers"]
-dependencies = [
-    "mopti==0.10.10",
-    "bofire>=0.0.4",
-]
-
-[project.urls]
-Homepage = "https://github.com/experimental-design/bofire-converters"
-
-[project.optional-dependencies]
-test = [
-    "pytest ~=7.3.2",
+[build-system]
+requires = ["setuptools", "setuptools_scm[toml]", "wheel"]
+build-backend = "setuptools.build_meta"
+
+[tool.setuptools_scm]
+local_scheme = "node-and-date"
+write_to = "./bofire_converters/version.py"
+
+[tool.ruff]
+ignore = [
+    "E501",  # don't enforce for comments and docstrings
+    "B017",  # required for tests
+    "B027",  # required for optional _tell method
+    "B028",
+    "B904",
+    "B905"
+]
+line-length = 88
+select = ["B", "C", "E", "F", "W", "I"]
+
+[tool.ruff.mccabe]
+max-complexity = 18
+
+[project]
+name = "bofire_converters"
+license = { file = "LICENSE" }
+readme = "README.md"
+requires-python = ">=3.7"
+classifiers = ["Development Status :: 1 - Planning",
+        "Programming Language :: Python :: 3 :: Only",
+        "License :: OSI Approved :: BSD License",
+        "Topic :: Scientific/Engineering",
+        "Intended Audience :: Science/Research",
+        "Intended Audience :: Developers"]
+dependencies = [
+    "mopti>=0.10.10",
+    "bofire>=0.0.12",
+]
+dynamic = [
+  "version",
+]
+[project.urls]
+Homepage = "https://github.com/experimental-design/bofire-converters"
+
+[project.optional-dependencies]
+test = [
+    "pytest>=8.1.1",
 ]
```

### Comparing `bofire_converters-0.0.2/test/test_opti_to_domain.py` & `bofire_converters-0.0.3/test/test_opti_to_domain.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,162 +1,165 @@
-import pytest
-from bofire.data_models.domain.api import Domain
-from opti import (
-    Categorical,
-    CloseToTarget,
-    Continuous,
-    Discrete,
-    Maximize,
-    Minimize,
-    Objectives,
-    Parameters,
-)
-from opti.constraint import (
-    Constraints,
-    LinearEquality,
-    LinearInequality,
-    NChooseK,
-    NonlinearEquality,
-    NonlinearInequality,
-)
-from opti.problems.cbo_benchmarks import (
-    G4,
-    G6,
-    G7,
-    G8,
-    G10,
-    Gardner,
-    Gramacy,
-    PressureVessel,
-    Sasena,
-    SpeedReducer,
-    TensionCompression,
-    WeldedBeam1,
-)
-from opti.problems.detergent import (
-    Detergent,
-    Detergent_NChooseKConstraint,
-    Detergent_OutputConstraint,
-    Detergent_TwoOutputConstraints,
-)
-from opti.problems.mixed import DiscreteFuelInjector, DiscreteVLMOP2
-from opti.problems.multi import (
-    Daechert1,
-    Daechert2,
-    Daechert3,
-    Hyperellipsoid,
-    OmniTest,
-    Poloni,
-    Qapi1,
-    WeldedBeam,
-)
-
-from domainconverters.opti_to_domain import (
-    convert_constraints,
-    convert_inputs,
-    convert_outputs_and_objectives,
-    convert_problem,
-)
-
-test_problems = [
-    G4(),
-    G6(),
-    G7(),
-    G8(),
-    G10(),
-    Gardner(),
-    Gramacy(),
-    PressureVessel(),
-    Sasena(),
-    SpeedReducer(),
-    TensionCompression(),
-    WeldedBeam1(),
-    DiscreteFuelInjector(),
-    DiscreteVLMOP2(),
-    Daechert1(),
-    Daechert2(),
-    Daechert3(),
-    Poloni(),
-    Qapi1(),
-    WeldedBeam(),
-    Hyperellipsoid(),
-    OmniTest(),
-    Detergent(),
-    Detergent_NChooseKConstraint(),
-    Detergent_OutputConstraint(discrete=True),
-    Detergent_OutputConstraint(discrete=False),
-    Detergent_TwoOutputConstraints(),
-]
-
-
-@pytest.mark.parametrize("test_problem", test_problems)
-def test_convert_benchmarks(test_problem):
-    if not all(
-        [otype == "continuous" for otype in [o.type for o in test_problem.outputs]]
-    ):
-        with pytest.warns(UserWarning):
-            bofire_domain = convert_problem(test_problem)
-    else:
-        bofire_domain = convert_problem(test_problem)
-    assert isinstance(bofire_domain, Domain)
-    assert len(test_problem.inputs) == len(bofire_domain.inputs)
-    if test_problem.constraints is not None:
-        assert len(test_problem.constraints) == len(bofire_domain.constraints)
-
-
-def test_convert_constraints():
-    cnstrs = Constraints(
-        [
-            LinearEquality(["x1", "x2", "x3"], lhs=[1, 1, 1], rhs=1),
-            LinearInequality(["x1", "x2"], lhs=[1, 1], rhs=0.5),
-            NonlinearEquality("x1 + x2 + x3 - 1"),
-            NonlinearInequality("x1**2 + x3**2 - 1"),
-            NChooseK(["x1", "x2"], max_active=2),
-        ]
-    )
-    bofire_constraints = convert_constraints(cnstrs)
-    print(bofire_constraints)
-    assert isinstance(bofire_constraints, list)
-    assert len(bofire_constraints) == 5
-
-
-def test_convert_inputs():
-    inputs = Parameters(
-        [
-            Discrete("x1", domain=[0.0, 1.0, 2.0, 3.0]),
-            Continuous("x2", domain=[-2.0, 2.0]),
-            Continuous("x3", domain=[-2.0, 2.0]),
-            Continuous("x4", domain=[-2.0, 2.0]),
-            Categorical("x5", domain=["cat", "dog", "monkey"]),
-        ]
-    )
-
-    bofire_inputs = convert_inputs(inputs)
-    assert isinstance(bofire_inputs, list)
-    assert len(bofire_inputs) == 5
-
-
-def test_convert_outputs_and_objectives():
-    outputs = Parameters(
-        [
-            Discrete("meetings", domain=[0.0, 1.0, 2.0, 3.0]),
-            Continuous("coffee", domain=[0, 20.0]),
-            Continuous("seriousness", domain=[0, 10.0]),
-            Categorical("animal", domain=["cat", "dog", "monkey"]),
-        ]
-    )
-
-    objectives = Objectives(
-        [
-            Minimize("meetings", target=2),
-            Maximize("coffee", target=4),
-            CloseToTarget("seriousness", target=5, exponent=2, tolerance=1.1),
-        ]
-    )
-
-    with pytest.warns(UserWarning):
-        out_list = convert_outputs_and_objectives(outputs, objectives)
-
-    assert len(out_list) == 4
-    # we used to check these but now all outputs are converted to continuous
-    # assert out_list[0].type == "discrete"
-    # assert out_list[-1].type == "categorical"
+import pytest
+from bofire.data_models.domain.api import Domain
+from opti import (
+    Categorical,
+    CloseToTarget,
+    Continuous,
+    Discrete,
+    Maximize,
+    Minimize,
+    Objectives,
+    Parameters,
+)
+from opti.constraint import (
+    Constraints,
+    LinearEquality,
+    LinearInequality,
+    NChooseK,
+    NonlinearEquality,
+    NonlinearInequality,
+)
+from opti.problems.cbo_benchmarks import (
+    G4,
+    G6,
+    G7,
+    G8,
+    G10,
+    Gardner,
+    Gramacy,
+    PressureVessel,
+    Sasena,
+    SpeedReducer,
+    TensionCompression,
+    WeldedBeam1,
+)
+from opti.problems.detergent import (
+    Detergent,
+    Detergent_NChooseKConstraint,
+    Detergent_OutputConstraint,
+    Detergent_TwoOutputConstraints,
+)
+from opti.problems.mixed import DiscreteFuelInjector, DiscreteVLMOP2
+from opti.problems.multi import (
+    Daechert1,
+    Daechert2,
+    Daechert3,
+    Hyperellipsoid,
+    OmniTest,
+    Poloni,
+    Qapi1,
+    WeldedBeam,
+)
+
+from bofire_converters.opti_to_domain import (
+    convert_constraints,
+    convert_inputs,
+    convert_outputs_and_objectives,
+    convert_problem,
+)
+
+test_problems = [
+    G4(),
+    G6(),
+    G7(),
+    G8(),
+    G10(),
+    Gardner(),
+    Gramacy(),
+    PressureVessel(),
+    Sasena(),
+    SpeedReducer(),
+    TensionCompression(),
+    WeldedBeam1(),
+    DiscreteFuelInjector(),
+    DiscreteVLMOP2(),
+    Daechert1(),
+    Daechert2(),
+    Daechert3(),
+    Poloni(),
+    Qapi1(),
+    WeldedBeam(),
+    Hyperellipsoid(),
+    OmniTest(),
+    Detergent(),
+    Detergent_NChooseKConstraint(),
+    Detergent_OutputConstraint(discrete=True),
+    Detergent_OutputConstraint(discrete=False),
+    Detergent_TwoOutputConstraints(),
+]
+
+
+@pytest.mark.parametrize("test_problem", test_problems)
+def test_convert_benchmarks(test_problem):
+    if not all(
+        otype == "continuous" for otype in [o.type for o in test_problem.outputs]
+    ):
+        with pytest.warns(UserWarning):
+            bofire_domain = convert_problem(test_problem)
+    else:
+        bofire_domain = convert_problem(test_problem)
+    assert isinstance(bofire_domain, Domain)
+    assert len(test_problem.inputs) == len(bofire_domain.inputs)
+    if test_problem.constraints is not None:
+        assert len(test_problem.constraints) == len(bofire_domain.constraints)
+
+
+def test_convert_constraints():
+    cnstrs = Constraints(
+        [
+            LinearEquality(["x1", "x2", "x3"], lhs=[1, 1, 1], rhs=1),
+            LinearInequality(["x1", "x2"], lhs=[1, 1], rhs=0.5),
+            NonlinearEquality("x1 + x2 + x3 - 1"),
+            NonlinearInequality("x1**2 + x3**2 - 1"),
+            NChooseK(["x1", "x2"], max_active=2),
+        ]
+    )
+    bofire_constraints = convert_constraints(cnstrs)
+    print(bofire_constraints)
+    assert isinstance(bofire_constraints, list)
+    assert len(bofire_constraints) == 5
+
+
+def test_convert_inputs():
+    inputs = Parameters(
+        [
+            Discrete("x1", domain=[0.0, 1.0, 2.0, 3.0]),
+            Continuous("x2", domain=[-2.0, 2.0]),
+            Continuous("x3", domain=[-2.0, 2.0]),
+            Continuous("x4", domain=[-2.0, 2.0]),
+            Categorical("x5", domain=["cat", "dog", "monkey"]),
+        ]
+    )
+
+    bofire_inputs = convert_inputs(inputs)
+    assert isinstance(bofire_inputs, list)
+    assert len(bofire_inputs) == 5
+
+
+def test_convert_outputs_and_objectives():
+    outputs = Parameters(
+        [
+            Discrete("meetings", domain=[0.0, 1.0, 2.0, 3.0]),
+            Continuous("coffee", domain=[0, 20.0]),
+            Continuous("seriousness", domain=[0, 10.0]),
+            Categorical("animal", domain=["cat", "dog", "monkey"]),
+        ]
+    )
+
+    objectives = Objectives(
+        [
+            Minimize("meetings", target=2),
+            Maximize("coffee", target=4),
+            CloseToTarget("seriousness", target=5, exponent=2, tolerance=1.1),
+        ]
+    )
+
+    with pytest.warns(UserWarning):
+        out_list = convert_outputs_and_objectives(outputs, objectives)
+
+    assert len(out_list) == 4
+    assert (
+        out_list[0].type == "ContinuousOutput"
+    )  # discrete will be converted to continuous
+    assert out_list[1].type == "ContinuousOutput"
+    assert out_list[2].type == "ContinuousOutput"
+    assert out_list[3].type == "CategoricalOutput"
```

