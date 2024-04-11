# Comparing `tmp/qadence-1.5.0.tar.gz` & `tmp/qadence-1.5.1.tar.gz`

## Comparing `qadence-1.5.0.tar` & `qadence-1.5.1.tar`

### file list

```diff
@@ -1,154 +1,154 @@
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 qadence-1.5.0/.coveragerc
--rw-r--r--   0        0        0      763 2020-02-02 00:00:00.000000 qadence-1.5.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 qadence-1.5.0/MANIFEST.in
--rw-r--r--   0        0        0     4793 2020-02-02 00:00:00.000000 qadence-1.5.0/mkdocs.yml
--rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 qadence-1.5.0/renovate.json
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 qadence-1.5.0/setup.py
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 qadence-1.5.0/.github/dependabot.yml
--rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 qadence-1.5.0/.github/workflows/build_docs.yml
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 qadence-1.5.0/.github/workflows/dependabot.yml
--rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 qadence-1.5.0/.github/workflows/lint.yml
--rw-r--r--   0        0        0     1410 2020-02-02 00:00:00.000000 qadence-1.5.0/.github/workflows/test_all.yml
--rw-r--r--   0        0        0      676 2020-02-02 00:00:00.000000 qadence-1.5.0/.github/workflows/test_examples.yml
--rw-r--r--   0        0        0     3063 2020-02-02 00:00:00.000000 qadence-1.5.0/.github/workflows/test_fast.yml
--rw-r--r--   0        0        0     1708 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/__init__.py
--rw-r--r--   0        0        0    15493 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/backend.py
--rw-r--r--   0        0        0     6892 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/circuit.py
--rw-r--r--   0        0        0     5230 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/decompose.py
--rw-r--r--   0        0        0     1832 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/divergences.py
--rw-r--r--   0        0        0     9287 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/execution.py
--rw-r--r--   0        0        0     4582 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/extensions.py
--rw-r--r--   0        0        0     1592 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/finitediff.py
--rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/libs.py
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/logger.py
--rw-r--r--   0        0        0    17294 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/overlap.py
--rw-r--r--   0        0        0    12334 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/parameters.py
--rw-r--r--   0        0        0      442 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/protocols.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/py.typed
--rw-r--r--   0        0        0     2120 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/qubit_support.py
--rw-r--r--   0        0        0    10276 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/register.py
--rw-r--r--   0        0        0    11702 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/serialization.py
--rw-r--r--   0        0        0    14341 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/states.py
--rw-r--r--   0        0        0     9699 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/types.py
--rw-r--r--   0        0        0     8829 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/utils.py
--rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/analog/__init__.py
--rw-r--r--   0        0        0     6435 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/analog/addressing.py
--rw-r--r--   0        0        0     1243 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/analog/constants.py
--rw-r--r--   0        0        0     2412 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/analog/device.py
--rw-r--r--   0        0        0     3421 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/analog/hamiltonian_terms.py
--rw-r--r--   0        0        0     4223 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/analog/parse_analog.py
--rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/backends/__init__.py
--rw-r--r--   0        0        0     6831 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/backends/adjoint.py
--rw-r--r--   0        0        0     3224 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/backends/api.py
--rw-r--r--   0        0        0     4341 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/backends/gpsr.py
--rw-r--r--   0        0        0     5038 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/backends/jax_utils.py
--rw-r--r--   0        0        0     6490 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/backends/utils.py
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/backends/braket/__init__.py
--rw-r--r--   0        0        0     8730 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/backends/braket/backend.py
--rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/backends/braket/config.py
--rw-r--r--   0        0        0     3417 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/backends/braket/convert_ops.py
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/backends/horqrux/__init__.py
--rw-r--r--   0        0        0     9330 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/backends/horqrux/backend.py
--rw-r--r--   0        0        0      901 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/backends/horqrux/config.py
--rw-r--r--   0        0        0     8564 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/backends/horqrux/convert_ops.py
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/backends/pulser/__init__.py
--rw-r--r--   0        0        0    13868 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/backends/pulser/backend.py
--rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/backends/pulser/channels.py
--rw-r--r--   0        0        0     2057 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/backends/pulser/cloud.py
--rw-r--r--   0        0        0     3122 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/backends/pulser/config.py
--rw-r--r--   0        0        0     1227 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/backends/pulser/convert_ops.py
--rw-r--r--   0        0        0     2448 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/backends/pulser/devices.py
--rw-r--r--   0        0        0    11893 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/backends/pulser/pulses.py
--rw-r--r--   0        0        0     2227 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/backends/pulser/waveforms.py
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/backends/pyqtorch/__init__.py
--rw-r--r--   0        0        0     9763 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/backends/pyqtorch/backend.py
--rw-r--r--   0        0        0     1907 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/backends/pyqtorch/config.py
--rw-r--r--   0        0        0    17512 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/backends/pyqtorch/convert_ops.py
--rw-r--r--   0        0        0      960 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/blocks/__init__.py
--rw-r--r--   0        0        0    11796 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/blocks/abstract.py
--rw-r--r--   0        0        0    10812 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/blocks/analog.py
--rw-r--r--   0        0        0    17415 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/blocks/block_to_tensor.py
--rw-r--r--   0        0        0     8897 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/blocks/composite.py
--rw-r--r--   0        0        0     6513 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/blocks/embedding.py
--rw-r--r--   0        0        0     2387 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/blocks/manipulate.py
--rw-r--r--   0        0        0     3785 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/blocks/matrix.py
--rw-r--r--   0        0        0    16631 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/blocks/primitive.py
--rw-r--r--   0        0        0    16358 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/blocks/utils.py
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/constructors/__init__.py
--rw-r--r--   0        0        0    12170 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/constructors/ansatze.py
--rw-r--r--   0        0        0    11566 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/constructors/feature_maps.py
--rw-r--r--   0        0        0     8860 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/constructors/hamiltonians.py
--rw-r--r--   0        0        0     7001 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/constructors/iia.py
--rw-r--r--   0        0        0     7688 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/constructors/qft.py
--rw-r--r--   0        0        0     4848 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/constructors/rydberg_feature_maps.py
--rw-r--r--   0        0        0     8372 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/constructors/rydberg_hea.py
--rw-r--r--   0        0        0     3080 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/constructors/utils.py
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/constructors/daqc/__init__.py
--rw-r--r--   0        0        0     9922 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/constructors/daqc/daqc.py
--rw-r--r--   0        0        0     3821 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/constructors/daqc/gen_parser.py
--rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/constructors/daqc/utils.py
--rw-r--r--   0        0        0     2319 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/draw/__init__.py
--rw-r--r--   0        0        0     5533 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/draw/themes.py
--rw-r--r--   0        0        0    12108 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/draw/utils.py
--rw-r--r--   0        0        0    14997 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/draw/vizbackend.py
--rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/draw/assets/dark/measurement.png
--rw-r--r--   0        0        0     7282 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/draw/assets/dark/measurement.svg
--rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/draw/assets/light/measurement.png
--rw-r--r--   0        0        0     7282 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/draw/assets/light/measurement.svg
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/engines/__init__.py
--rw-r--r--   0        0        0     5875 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/engines/differentiable_backend.py
--rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/engines/jax/__init__.py
--rw-r--r--   0        0        0     3062 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/engines/jax/differentiable_backend.py
--rw-r--r--   0        0        0     3677 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/engines/jax/differentiable_expectation.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/engines/torch/__init__.py
--rw-r--r--   0        0        0     3553 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/engines/torch/differentiable_backend.py
--rw-r--r--   0        0        0     9161 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/engines/torch/differentiable_expectation.py
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/exceptions/__init__.py
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/exceptions/exceptions.py
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/measurements/__init__.py
--rw-r--r--   0        0        0     1161 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/measurements/protocols.py
--rw-r--r--   0        0        0     1200 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/measurements/samples.py
--rw-r--r--   0        0        0    12550 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/measurements/shadow.py
--rw-r--r--   0        0        0     2665 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/measurements/tomography.py
--rw-r--r--   0        0        0     6534 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/measurements/utils.py
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/mitigations/__init__.py
--rw-r--r--   0        0        0     7768 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/mitigations/analog_zne.py
--rw-r--r--   0        0        0     1608 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/mitigations/protocols.py
--rw-r--r--   0        0        0     6262 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/mitigations/readout.py
--rw-r--r--   0        0        0      786 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/ml_tools/__init__.py
--rw-r--r--   0        0        0     2356 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/ml_tools/config.py
--rw-r--r--   0        0        0     4283 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/ml_tools/data.py
--rw-r--r--   0        0        0    11736 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/ml_tools/models.py
--rw-r--r--   0        0        0     1800 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/ml_tools/optimize_step.py
--rw-r--r--   0        0        0     1301 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/ml_tools/parameters.py
--rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/ml_tools/printing.py
--rw-r--r--   0        0        0     4663 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/ml_tools/saveload.py
--rw-r--r--   0        0        0     1337 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/ml_tools/tensors.py
--rw-r--r--   0        0        0     7399 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/ml_tools/train_grad.py
--rw-r--r--   0        0        0     4714 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/ml_tools/train_no_grad.py
--rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/ml_tools/utils.py
--rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/models/__init__.py
--rw-r--r--   0        0        0    10397 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/models/qnn.py
--rw-r--r--   0        0        0    14107 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/models/quantum_model.py
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/noise/__init__.py
--rw-r--r--   0        0        0     1653 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/noise/protocols.py
--rw-r--r--   0        0        0     6736 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/noise/readout.py
--rw-r--r--   0        0        0     1944 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/operations/__init__.py
--rw-r--r--   0        0        0     7782 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/operations/analog.py
--rw-r--r--   0        0        0     9492 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/operations/control_ops.py
--rw-r--r--   0        0        0     7400 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/operations/ham_evo.py
--rw-r--r--   0        0        0     4919 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/operations/parametric.py
--rw-r--r--   0        0        0     9011 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/operations/primitive.py
--rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/transpile/__init__.py
--rw-r--r--   0        0        0     1336 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/transpile/apply_fn.py
--rw-r--r--   0        0        0    11591 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/transpile/block.py
--rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/transpile/circuit.py
--rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/transpile/digitalize.py
--rw-r--r--   0        0        0     3427 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/transpile/flatten.py
--rw-r--r--   0        0        0     4867 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/transpile/invert.py
--rw-r--r--   0        0        0     2721 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/transpile/transpile.py
--rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 qadence-1.5.0/.gitignore
--rw-r--r--   0        0        0    11358 2020-02-02 00:00:00.000000 qadence-1.5.0/LICENSE
--rw-r--r--   0        0        0     6536 2020-02-02 00:00:00.000000 qadence-1.5.0/README.md
--rw-r--r--   0        0        0     5503 2020-02-02 00:00:00.000000 qadence-1.5.0/pyproject.toml
--rw-r--r--   0        0        0     8997 2020-02-02 00:00:00.000000 qadence-1.5.0/PKG-INFO
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 qadence-1.5.1/.coveragerc
+-rw-r--r--   0        0        0      763 2020-02-02 00:00:00.000000 qadence-1.5.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 qadence-1.5.1/MANIFEST.in
+-rw-r--r--   0        0        0     4793 2020-02-02 00:00:00.000000 qadence-1.5.1/mkdocs.yml
+-rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 qadence-1.5.1/renovate.json
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 qadence-1.5.1/setup.py
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 qadence-1.5.1/.github/dependabot.yml
+-rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 qadence-1.5.1/.github/workflows/build_docs.yml
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 qadence-1.5.1/.github/workflows/dependabot.yml
+-rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 qadence-1.5.1/.github/workflows/lint.yml
+-rw-r--r--   0        0        0     1410 2020-02-02 00:00:00.000000 qadence-1.5.1/.github/workflows/test_all.yml
+-rw-r--r--   0        0        0      676 2020-02-02 00:00:00.000000 qadence-1.5.1/.github/workflows/test_examples.yml
+-rw-r--r--   0        0        0     3063 2020-02-02 00:00:00.000000 qadence-1.5.1/.github/workflows/test_fast.yml
+-rw-r--r--   0        0        0     1708 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/__init__.py
+-rw-r--r--   0        0        0    14410 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/backend.py
+-rw-r--r--   0        0        0     6892 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/circuit.py
+-rw-r--r--   0        0        0     5230 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/decompose.py
+-rw-r--r--   0        0        0     1832 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/divergences.py
+-rw-r--r--   0        0        0     9287 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/execution.py
+-rw-r--r--   0        0        0     4582 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/extensions.py
+-rw-r--r--   0        0        0     1592 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/finitediff.py
+-rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/libs.py
+-rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/logger.py
+-rw-r--r--   0        0        0    17294 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/overlap.py
+-rw-r--r--   0        0        0    12334 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/parameters.py
+-rw-r--r--   0        0        0      442 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/protocols.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/py.typed
+-rw-r--r--   0        0        0     2120 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/qubit_support.py
+-rw-r--r--   0        0        0    10276 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/register.py
+-rw-r--r--   0        0        0    11702 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/serialization.py
+-rw-r--r--   0        0        0    14341 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/states.py
+-rw-r--r--   0        0        0     9699 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/types.py
+-rw-r--r--   0        0        0     8829 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/utils.py
+-rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/analog/__init__.py
+-rw-r--r--   0        0        0     6435 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/analog/addressing.py
+-rw-r--r--   0        0        0     1243 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/analog/constants.py
+-rw-r--r--   0        0        0     2412 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/analog/device.py
+-rw-r--r--   0        0        0     3421 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/analog/hamiltonian_terms.py
+-rw-r--r--   0        0        0     4223 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/analog/parse_analog.py
+-rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/backends/__init__.py
+-rw-r--r--   0        0        0     6831 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/backends/adjoint.py
+-rw-r--r--   0        0        0     3224 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/backends/api.py
+-rw-r--r--   0        0        0     4341 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/backends/gpsr.py
+-rw-r--r--   0        0        0     5038 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/backends/jax_utils.py
+-rw-r--r--   0        0        0     6490 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/backends/utils.py
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/backends/braket/__init__.py
+-rw-r--r--   0        0        0     8729 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/backends/braket/backend.py
+-rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/backends/braket/config.py
+-rw-r--r--   0        0        0     3417 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/backends/braket/convert_ops.py
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/backends/horqrux/__init__.py
+-rw-r--r--   0        0        0     9329 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/backends/horqrux/backend.py
+-rw-r--r--   0        0        0      901 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/backends/horqrux/config.py
+-rw-r--r--   0        0        0     8564 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/backends/horqrux/convert_ops.py
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/backends/pulser/__init__.py
+-rw-r--r--   0        0        0    13867 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/backends/pulser/backend.py
+-rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/backends/pulser/channels.py
+-rw-r--r--   0        0        0     2057 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/backends/pulser/cloud.py
+-rw-r--r--   0        0        0     3122 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/backends/pulser/config.py
+-rw-r--r--   0        0        0     1227 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/backends/pulser/convert_ops.py
+-rw-r--r--   0        0        0     2448 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/backends/pulser/devices.py
+-rw-r--r--   0        0        0    11893 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/backends/pulser/pulses.py
+-rw-r--r--   0        0        0     2227 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/backends/pulser/waveforms.py
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/backends/pyqtorch/__init__.py
+-rw-r--r--   0        0        0     9762 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/backends/pyqtorch/backend.py
+-rw-r--r--   0        0        0     1907 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/backends/pyqtorch/config.py
+-rw-r--r--   0        0        0    17512 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/backends/pyqtorch/convert_ops.py
+-rw-r--r--   0        0        0      960 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/blocks/__init__.py
+-rw-r--r--   0        0        0    11796 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/blocks/abstract.py
+-rw-r--r--   0        0        0    10812 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/blocks/analog.py
+-rw-r--r--   0        0        0    17415 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/blocks/block_to_tensor.py
+-rw-r--r--   0        0        0     8897 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/blocks/composite.py
+-rw-r--r--   0        0        0     6513 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/blocks/embedding.py
+-rw-r--r--   0        0        0     2387 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/blocks/manipulate.py
+-rw-r--r--   0        0        0     3785 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/blocks/matrix.py
+-rw-r--r--   0        0        0    16631 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/blocks/primitive.py
+-rw-r--r--   0        0        0    16358 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/blocks/utils.py
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/constructors/__init__.py
+-rw-r--r--   0        0        0    12170 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/constructors/ansatze.py
+-rw-r--r--   0        0        0    11566 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/constructors/feature_maps.py
+-rw-r--r--   0        0        0     8860 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/constructors/hamiltonians.py
+-rw-r--r--   0        0        0     7001 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/constructors/iia.py
+-rw-r--r--   0        0        0     7688 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/constructors/qft.py
+-rw-r--r--   0        0        0     4848 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/constructors/rydberg_feature_maps.py
+-rw-r--r--   0        0        0     8372 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/constructors/rydberg_hea.py
+-rw-r--r--   0        0        0     3080 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/constructors/utils.py
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/constructors/daqc/__init__.py
+-rw-r--r--   0        0        0     9922 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/constructors/daqc/daqc.py
+-rw-r--r--   0        0        0     3821 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/constructors/daqc/gen_parser.py
+-rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/constructors/daqc/utils.py
+-rw-r--r--   0        0        0     2319 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/draw/__init__.py
+-rw-r--r--   0        0        0     5533 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/draw/themes.py
+-rw-r--r--   0        0        0    12108 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/draw/utils.py
+-rw-r--r--   0        0        0    14997 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/draw/vizbackend.py
+-rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/draw/assets/dark/measurement.png
+-rw-r--r--   0        0        0     7282 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/draw/assets/dark/measurement.svg
+-rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/draw/assets/light/measurement.png
+-rw-r--r--   0        0        0     7282 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/draw/assets/light/measurement.svg
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/engines/__init__.py
+-rw-r--r--   0        0        0     5875 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/engines/differentiable_backend.py
+-rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/engines/jax/__init__.py
+-rw-r--r--   0        0        0     3062 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/engines/jax/differentiable_backend.py
+-rw-r--r--   0        0        0     3677 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/engines/jax/differentiable_expectation.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/engines/torch/__init__.py
+-rw-r--r--   0        0        0     3553 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/engines/torch/differentiable_backend.py
+-rw-r--r--   0        0        0     9161 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/engines/torch/differentiable_expectation.py
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/exceptions/__init__.py
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/exceptions/exceptions.py
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/measurements/__init__.py
+-rw-r--r--   0        0        0     1161 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/measurements/protocols.py
+-rw-r--r--   0        0        0     1200 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/measurements/samples.py
+-rw-r--r--   0        0        0    12550 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/measurements/shadow.py
+-rw-r--r--   0        0        0     2665 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/measurements/tomography.py
+-rw-r--r--   0        0        0     6534 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/measurements/utils.py
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/mitigations/__init__.py
+-rw-r--r--   0        0        0     7768 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/mitigations/analog_zne.py
+-rw-r--r--   0        0        0     1608 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/mitigations/protocols.py
+-rw-r--r--   0        0        0     6262 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/mitigations/readout.py
+-rw-r--r--   0        0        0      786 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/ml_tools/__init__.py
+-rw-r--r--   0        0        0     2356 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/ml_tools/config.py
+-rw-r--r--   0        0        0     4283 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/ml_tools/data.py
+-rw-r--r--   0        0        0    12476 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/ml_tools/models.py
+-rw-r--r--   0        0        0     1800 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/ml_tools/optimize_step.py
+-rw-r--r--   0        0        0     1301 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/ml_tools/parameters.py
+-rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/ml_tools/printing.py
+-rw-r--r--   0        0        0     4663 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/ml_tools/saveload.py
+-rw-r--r--   0        0        0     1337 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/ml_tools/tensors.py
+-rw-r--r--   0        0        0     7727 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/ml_tools/train_grad.py
+-rw-r--r--   0        0        0     4714 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/ml_tools/train_no_grad.py
+-rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/ml_tools/utils.py
+-rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/models/__init__.py
+-rw-r--r--   0        0        0    10397 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/models/qnn.py
+-rw-r--r--   0        0        0    14186 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/models/quantum_model.py
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/noise/__init__.py
+-rw-r--r--   0        0        0     1653 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/noise/protocols.py
+-rw-r--r--   0        0        0     6736 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/noise/readout.py
+-rw-r--r--   0        0        0     1944 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/operations/__init__.py
+-rw-r--r--   0        0        0     7782 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/operations/analog.py
+-rw-r--r--   0        0        0     9492 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/operations/control_ops.py
+-rw-r--r--   0        0        0     7400 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/operations/ham_evo.py
+-rw-r--r--   0        0        0     4919 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/operations/parametric.py
+-rw-r--r--   0        0        0     9011 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/operations/primitive.py
+-rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/transpile/__init__.py
+-rw-r--r--   0        0        0     1336 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/transpile/apply_fn.py
+-rw-r--r--   0        0        0    11591 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/transpile/block.py
+-rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/transpile/circuit.py
+-rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/transpile/digitalize.py
+-rw-r--r--   0        0        0     3427 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/transpile/flatten.py
+-rw-r--r--   0        0        0     4867 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/transpile/invert.py
+-rw-r--r--   0        0        0     2721 2020-02-02 00:00:00.000000 qadence-1.5.1/qadence/transpile/transpile.py
+-rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 qadence-1.5.1/.gitignore
+-rw-r--r--   0        0        0    11358 2020-02-02 00:00:00.000000 qadence-1.5.1/LICENSE
+-rw-r--r--   0        0        0     6536 2020-02-02 00:00:00.000000 qadence-1.5.1/README.md
+-rw-r--r--   0        0        0     5503 2020-02-02 00:00:00.000000 qadence-1.5.1/pyproject.toml
+-rw-r--r--   0        0        0     8997 2020-02-02 00:00:00.000000 qadence-1.5.1/PKG-INFO
```

### Comparing `qadence-1.5.0/.pre-commit-config.yaml` & `qadence-1.5.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `qadence-1.5.0/mkdocs.yml` & `qadence-1.5.1/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `qadence-1.5.0/.github/workflows/build_docs.yml` & `qadence-1.5.1/.github/workflows/build_docs.yml`

 * *Files identical despite different names*

### Comparing `qadence-1.5.0/.github/workflows/test_all.yml` & `qadence-1.5.1/.github/workflows/test_all.yml`

 * *Files identical despite different names*

### Comparing `qadence-1.5.0/.github/workflows/test_examples.yml` & `qadence-1.5.1/.github/workflows/test_examples.yml`

 * *Files identical despite different names*

### Comparing `qadence-1.5.0/.github/workflows/test_fast.yml` & `qadence-1.5.1/.github/workflows/test_fast.yml`

 * *Files identical despite different names*

### Comparing `qadence-1.5.0/qadence/__init__.py` & `qadence-1.5.1/qadence/__init__.py`

 * *Files identical despite different names*

### Comparing `qadence-1.5.0/qadence/backend.py` & `qadence-1.5.1/qadence/backend.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,15 +22,14 @@
 from qadence.circuit import QuantumCircuit
 from qadence.logger import get_logger
 from qadence.measurements import Measurements
 from qadence.mitigations import Mitigations
 from qadence.noise import Noise
 from qadence.parameters import stringify
 from qadence.types import ArrayLike, BackendName, DiffMode, Endianness, Engine, ParamDictType
-from qadence.utils import validate_values_and_state
 
 logger = get_logger(__file__)
 
 
 @dataclass
 class BackendConfiguration:
     _use_gate_params: bool = True
@@ -255,37 +254,14 @@
             state: Initial state.
             noise: A noise model to use.
             mitigation: An error mitigation protocol to apply.
             endianness: Endianness of the resulting bit strings.
         """
         raise NotImplementedError
 
-    @abstractmethod
-    def _run(
-        self,
-        circuit: ConvertedCircuit,
-        param_values: dict[str, ArrayLike] = {},
-        state: ArrayLike | None = None,
-        endianness: Endianness = Endianness.BIG,
-    ) -> ArrayLike:
-        """Run a circuit and return the resulting wave function.
-
-        Arguments:
-            circuit: A converted circuit as returned by `backend.circuit`.
-            param_values: _**Already embedded**_ parameters of the circuit. See
-                [`embedding`][qadence.blocks.embedding.embedding] for more info.
-            state: Initial state.
-            endianness: Endianness of the resulting wavefunction.
-
-        Returns:
-            A list of Counter objects where each key represents a bitstring
-            and its value the number of times it has been sampled from the given wave function.
-        """
-        raise NotImplementedError
-
     def run(
         self,
         circuit: ConvertedCircuit,
         param_values: dict[str, ArrayLike] = {},
         state: Tensor | None = None,
         endianness: Endianness = Endianness.BIG,
         *args: Any,
@@ -300,16 +276,15 @@
             state: Initial state.
             endianness: Endianness of the resulting wavefunction.
 
         Returns:
             A list of Counter objects where each key represents a bitstring
             and its value the number of times it has been sampled from the given wave function.
         """
-        validate_values_and_state(state, circuit.abstract.n_qubits, param_values)
-        return self._run(circuit, param_values, state, endianness, *args, **kwargs)
+        raise NotImplementedError
 
     @abstractmethod
     def run_dm(
         self,
         circuit: ConvertedCircuit,
         noise: Noise,
         param_values: dict[str, ArrayLike] = {},
```

### Comparing `qadence-1.5.0/qadence/circuit.py` & `qadence-1.5.1/qadence/circuit.py`

 * *Files identical despite different names*

### Comparing `qadence-1.5.0/qadence/decompose.py` & `qadence-1.5.1/qadence/decompose.py`

 * *Files identical despite different names*

### Comparing `qadence-1.5.0/qadence/divergences.py` & `qadence-1.5.1/qadence/divergences.py`

 * *Files identical despite different names*

### Comparing `qadence-1.5.0/qadence/execution.py` & `qadence-1.5.1/qadence/execution.py`

 * *Files identical despite different names*

### Comparing `qadence-1.5.0/qadence/extensions.py` & `qadence-1.5.1/qadence/extensions.py`

 * *Files identical despite different names*

### Comparing `qadence-1.5.0/qadence/finitediff.py` & `qadence-1.5.1/qadence/finitediff.py`

 * *Files identical despite different names*

### Comparing `qadence-1.5.0/qadence/logger.py` & `qadence-1.5.1/qadence/logger.py`

 * *Files identical despite different names*

### Comparing `qadence-1.5.0/qadence/overlap.py` & `qadence-1.5.1/qadence/overlap.py`

 * *Files identical despite different names*

### Comparing `qadence-1.5.0/qadence/parameters.py` & `qadence-1.5.1/qadence/parameters.py`

 * *Files identical despite different names*

### Comparing `qadence-1.5.0/qadence/qubit_support.py` & `qadence-1.5.1/qadence/qubit_support.py`

 * *Files identical despite different names*

### Comparing `qadence-1.5.0/qadence/register.py` & `qadence-1.5.1/qadence/register.py`

 * *Files identical despite different names*

### Comparing `qadence-1.5.0/qadence/serialization.py` & `qadence-1.5.1/qadence/serialization.py`

 * *Files identical despite different names*

### Comparing `qadence-1.5.0/qadence/states.py` & `qadence-1.5.1/qadence/states.py`

 * *Files identical despite different names*

### Comparing `qadence-1.5.0/qadence/types.py` & `qadence-1.5.1/qadence/types.py`

 * *Files identical despite different names*

### Comparing `qadence-1.5.0/qadence/utils.py` & `qadence-1.5.1/qadence/utils.py`

 * *Files identical despite different names*

### Comparing `qadence-1.5.0/qadence/analog/addressing.py` & `qadence-1.5.1/qadence/analog/addressing.py`

 * *Files identical despite different names*

### Comparing `qadence-1.5.0/qadence/analog/constants.py` & `qadence-1.5.1/qadence/analog/constants.py`

 * *Files identical despite different names*

### Comparing `qadence-1.5.0/qadence/analog/device.py` & `qadence-1.5.1/qadence/analog/device.py`

 * *Files identical despite different names*

### Comparing `qadence-1.5.0/qadence/analog/hamiltonian_terms.py` & `qadence-1.5.1/qadence/analog/hamiltonian_terms.py`

 * *Files identical despite different names*

### Comparing `qadence-1.5.0/qadence/analog/parse_analog.py` & `qadence-1.5.1/qadence/analog/parse_analog.py`

 * *Files identical despite different names*

### Comparing `qadence-1.5.0/qadence/backends/adjoint.py` & `qadence-1.5.1/qadence/backends/adjoint.py`

 * *Files identical despite different names*

### Comparing `qadence-1.5.0/qadence/backends/api.py` & `qadence-1.5.1/qadence/backends/api.py`

 * *Files identical despite different names*

### Comparing `qadence-1.5.0/qadence/backends/gpsr.py` & `qadence-1.5.1/qadence/backends/gpsr.py`

 * *Files identical despite different names*

### Comparing `qadence-1.5.0/qadence/backends/jax_utils.py` & `qadence-1.5.1/qadence/backends/jax_utils.py`

 * *Files identical despite different names*

### Comparing `qadence-1.5.0/qadence/backends/utils.py` & `qadence-1.5.1/qadence/backends/utils.py`

 * *Files identical despite different names*

### Comparing `qadence-1.5.0/qadence/backends/braket/backend.py` & `qadence-1.5.1/qadence/backends/braket/backend.py`

 * *Files 0% similar despite different names*

```diff
@@ -84,15 +84,15 @@
             block=obs,
             values={},
             qubit_support=tuple([i for i in range(n_qubits)]),
             endianness=Endianness.BIG,
         ).squeeze(0)
         return ConvertedObservable(native=native, abstract=obs, original=obs)
 
-    def _run(
+    def run(
         self,
         circuit: ConvertedCircuit,
         param_values: dict[str, Tensor] = {},
         state: Tensor | None = None,
         endianness: Endianness = Endianness.BIG,
     ) -> Tensor:
         """
```

### Comparing `qadence-1.5.0/qadence/backends/braket/config.py` & `qadence-1.5.1/qadence/backends/braket/config.py`

 * *Files identical despite different names*

### Comparing `qadence-1.5.0/qadence/backends/braket/convert_ops.py` & `qadence-1.5.1/qadence/backends/braket/convert_ops.py`

 * *Files identical despite different names*

### Comparing `qadence-1.5.0/qadence/backends/horqrux/backend.py` & `qadence-1.5.1/qadence/backends/horqrux/backend.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,15 +62,15 @@
             flatten,
             scale_primitive_blocks_only,
         ]
         block = transpile(*transpilations)(observable)  # type: ignore[call-overload]
         hq_obs = convert_observable(block, n_qubits=n_qubits, config=self.config)
         return ConvertedObservable(native=hq_obs, abstract=block, original=observable)
 
-    def _run(
+    def run(
         self,
         circuit: ConvertedCircuit,
         param_values: ParamDictType = {},
         state: ArrayLike | None = None,
         endianness: Endianness = Endianness.BIG,
         horqify_state: bool = True,
         unhorqify_state: bool = True,
```

### Comparing `qadence-1.5.0/qadence/backends/horqrux/config.py` & `qadence-1.5.1/qadence/backends/horqrux/config.py`

 * *Files identical despite different names*

### Comparing `qadence-1.5.0/qadence/backends/horqrux/convert_ops.py` & `qadence-1.5.1/qadence/backends/horqrux/convert_ops.py`

 * *Files identical despite different names*

### Comparing `qadence-1.5.0/qadence/backends/pulser/backend.py` & `qadence-1.5.1/qadence/backends/pulser/backend.py`

 * *Files 1% similar despite different names*

```diff
@@ -196,15 +196,15 @@
             k: v.detach().cpu().numpy()
             for (k, v) in param_values.items()
             if k in circuit.native.declared_variables
         }
 
         return circuit.native.build(**numpy_param_values)
 
-    def _run(
+    def run(
         self,
         circuit: ConvertedCircuit,
         param_values: dict[str, Tensor] = {},
         state: Tensor | None = None,
         endianness: Endianness = Endianness.BIG,
     ) -> Tensor:
         vals = to_list_of_dicts(param_values)
```

### Comparing `qadence-1.5.0/qadence/backends/pulser/cloud.py` & `qadence-1.5.1/qadence/backends/pulser/cloud.py`

 * *Files identical despite different names*

### Comparing `qadence-1.5.0/qadence/backends/pulser/config.py` & `qadence-1.5.1/qadence/backends/pulser/config.py`

 * *Files identical despite different names*

### Comparing `qadence-1.5.0/qadence/backends/pulser/convert_ops.py` & `qadence-1.5.1/qadence/backends/pulser/convert_ops.py`

 * *Files identical despite different names*

### Comparing `qadence-1.5.0/qadence/backends/pulser/devices.py` & `qadence-1.5.1/qadence/backends/pulser/devices.py`

 * *Files identical despite different names*

### Comparing `qadence-1.5.0/qadence/backends/pulser/pulses.py` & `qadence-1.5.1/qadence/backends/pulser/pulses.py`

 * *Files identical despite different names*

### Comparing `qadence-1.5.0/qadence/backends/pulser/waveforms.py` & `qadence-1.5.1/qadence/backends/pulser/waveforms.py`

 * *Files identical despite different names*

### Comparing `qadence-1.5.0/qadence/backends/pyqtorch/backend.py` & `qadence-1.5.1/qadence/backends/pyqtorch/backend.py`

 * *Files 0% similar despite different names*

```diff
@@ -76,15 +76,15 @@
             scale_primitive_blocks_only,
         ]
         block = transpile(*transpilations)(observable)  # type: ignore[call-overload]
 
         (native,) = convert_observable(block, n_qubits=n_qubits, config=self.config)
         return ConvertedObservable(native=native, abstract=block, original=observable)
 
-    def _run(
+    def run(
         self,
         circuit: ConvertedCircuit,
         param_values: dict[str, Tensor] = {},
         state: Tensor | None = None,
         endianness: Endianness = Endianness.BIG,
         pyqify_state: bool = True,
         unpyqify_state: bool = True,
```

### Comparing `qadence-1.5.0/qadence/backends/pyqtorch/config.py` & `qadence-1.5.1/qadence/backends/pyqtorch/config.py`

 * *Files identical despite different names*

### Comparing `qadence-1.5.0/qadence/backends/pyqtorch/convert_ops.py` & `qadence-1.5.1/qadence/backends/pyqtorch/convert_ops.py`

 * *Files identical despite different names*

### Comparing `qadence-1.5.0/qadence/blocks/__init__.py` & `qadence-1.5.1/qadence/blocks/__init__.py`

 * *Files identical despite different names*

### Comparing `qadence-1.5.0/qadence/blocks/abstract.py` & `qadence-1.5.1/qadence/blocks/abstract.py`

 * *Files identical despite different names*

### Comparing `qadence-1.5.0/qadence/blocks/analog.py` & `qadence-1.5.1/qadence/blocks/analog.py`

 * *Files identical despite different names*

### Comparing `qadence-1.5.0/qadence/blocks/block_to_tensor.py` & `qadence-1.5.1/qadence/blocks/block_to_tensor.py`

 * *Files identical despite different names*

### Comparing `qadence-1.5.0/qadence/blocks/composite.py` & `qadence-1.5.1/qadence/blocks/composite.py`

 * *Files identical despite different names*

### Comparing `qadence-1.5.0/qadence/blocks/embedding.py` & `qadence-1.5.1/qadence/blocks/embedding.py`

 * *Files identical despite different names*

### Comparing `qadence-1.5.0/qadence/blocks/manipulate.py` & `qadence-1.5.1/qadence/blocks/manipulate.py`

 * *Files identical despite different names*

### Comparing `qadence-1.5.0/qadence/blocks/matrix.py` & `qadence-1.5.1/qadence/blocks/matrix.py`

 * *Files identical despite different names*

### Comparing `qadence-1.5.0/qadence/blocks/primitive.py` & `qadence-1.5.1/qadence/blocks/primitive.py`

 * *Files identical despite different names*

### Comparing `qadence-1.5.0/qadence/blocks/utils.py` & `qadence-1.5.1/qadence/blocks/utils.py`

 * *Files identical despite different names*

### Comparing `qadence-1.5.0/qadence/constructors/__init__.py` & `qadence-1.5.1/qadence/constructors/__init__.py`

 * *Files identical despite different names*

### Comparing `qadence-1.5.0/qadence/constructors/ansatze.py` & `qadence-1.5.1/qadence/constructors/ansatze.py`

 * *Files identical despite different names*

### Comparing `qadence-1.5.0/qadence/constructors/feature_maps.py` & `qadence-1.5.1/qadence/constructors/feature_maps.py`

 * *Files identical despite different names*

### Comparing `qadence-1.5.0/qadence/constructors/hamiltonians.py` & `qadence-1.5.1/qadence/constructors/hamiltonians.py`

 * *Files identical despite different names*

### Comparing `qadence-1.5.0/qadence/constructors/iia.py` & `qadence-1.5.1/qadence/constructors/iia.py`

 * *Files identical despite different names*

### Comparing `qadence-1.5.0/qadence/constructors/qft.py` & `qadence-1.5.1/qadence/constructors/qft.py`

 * *Files identical despite different names*

### Comparing `qadence-1.5.0/qadence/constructors/rydberg_feature_maps.py` & `qadence-1.5.1/qadence/constructors/rydberg_feature_maps.py`

 * *Files identical despite different names*

### Comparing `qadence-1.5.0/qadence/constructors/rydberg_hea.py` & `qadence-1.5.1/qadence/constructors/rydberg_hea.py`

 * *Files identical despite different names*

### Comparing `qadence-1.5.0/qadence/constructors/utils.py` & `qadence-1.5.1/qadence/constructors/utils.py`

 * *Files identical despite different names*

### Comparing `qadence-1.5.0/qadence/constructors/daqc/daqc.py` & `qadence-1.5.1/qadence/constructors/daqc/daqc.py`

 * *Files identical despite different names*

### Comparing `qadence-1.5.0/qadence/constructors/daqc/gen_parser.py` & `qadence-1.5.1/qadence/constructors/daqc/gen_parser.py`

 * *Files identical despite different names*

### Comparing `qadence-1.5.0/qadence/constructors/daqc/utils.py` & `qadence-1.5.1/qadence/constructors/daqc/utils.py`

 * *Files identical despite different names*

### Comparing `qadence-1.5.0/qadence/draw/__init__.py` & `qadence-1.5.1/qadence/draw/__init__.py`

 * *Files identical despite different names*

### Comparing `qadence-1.5.0/qadence/draw/themes.py` & `qadence-1.5.1/qadence/draw/themes.py`

 * *Files identical despite different names*

### Comparing `qadence-1.5.0/qadence/draw/utils.py` & `qadence-1.5.1/qadence/draw/utils.py`

 * *Files identical despite different names*

### Comparing `qadence-1.5.0/qadence/draw/vizbackend.py` & `qadence-1.5.1/qadence/draw/vizbackend.py`

 * *Files identical despite different names*

### Comparing `qadence-1.5.0/qadence/draw/assets/dark/measurement.svg` & `qadence-1.5.1/qadence/draw/assets/dark/measurement.svg`

 * *Files identical despite different names*

### Comparing `qadence-1.5.0/qadence/draw/assets/light/measurement.svg` & `qadence-1.5.1/qadence/draw/assets/light/measurement.svg`

 * *Files identical despite different names*

### Comparing `qadence-1.5.0/qadence/engines/differentiable_backend.py` & `qadence-1.5.1/qadence/engines/differentiable_backend.py`

 * *Files identical despite different names*

### Comparing `qadence-1.5.0/qadence/engines/jax/differentiable_backend.py` & `qadence-1.5.1/qadence/engines/jax/differentiable_backend.py`

 * *Files identical despite different names*

### Comparing `qadence-1.5.0/qadence/engines/jax/differentiable_expectation.py` & `qadence-1.5.1/qadence/engines/jax/differentiable_expectation.py`

 * *Files identical despite different names*

### Comparing `qadence-1.5.0/qadence/engines/torch/differentiable_backend.py` & `qadence-1.5.1/qadence/engines/torch/differentiable_backend.py`

 * *Files identical despite different names*

### Comparing `qadence-1.5.0/qadence/engines/torch/differentiable_expectation.py` & `qadence-1.5.1/qadence/engines/torch/differentiable_expectation.py`

 * *Files identical despite different names*

### Comparing `qadence-1.5.0/qadence/measurements/protocols.py` & `qadence-1.5.1/qadence/measurements/protocols.py`

 * *Files identical despite different names*

### Comparing `qadence-1.5.0/qadence/measurements/samples.py` & `qadence-1.5.1/qadence/measurements/samples.py`

 * *Files identical despite different names*

### Comparing `qadence-1.5.0/qadence/measurements/shadow.py` & `qadence-1.5.1/qadence/measurements/shadow.py`

 * *Files identical despite different names*

### Comparing `qadence-1.5.0/qadence/measurements/tomography.py` & `qadence-1.5.1/qadence/measurements/tomography.py`

 * *Files identical despite different names*

### Comparing `qadence-1.5.0/qadence/measurements/utils.py` & `qadence-1.5.1/qadence/measurements/utils.py`

 * *Files identical despite different names*

### Comparing `qadence-1.5.0/qadence/mitigations/analog_zne.py` & `qadence-1.5.1/qadence/mitigations/analog_zne.py`

 * *Files identical despite different names*

### Comparing `qadence-1.5.0/qadence/mitigations/protocols.py` & `qadence-1.5.1/qadence/mitigations/protocols.py`

 * *Files identical despite different names*

### Comparing `qadence-1.5.0/qadence/mitigations/readout.py` & `qadence-1.5.1/qadence/mitigations/readout.py`

 * *Files identical despite different names*

### Comparing `qadence-1.5.0/qadence/ml_tools/__init__.py` & `qadence-1.5.1/qadence/ml_tools/__init__.py`

 * *Files identical despite different names*

### Comparing `qadence-1.5.0/qadence/ml_tools/config.py` & `qadence-1.5.1/qadence/ml_tools/config.py`

 * *Files identical despite different names*

### Comparing `qadence-1.5.0/qadence/ml_tools/data.py` & `qadence-1.5.1/qadence/ml_tools/data.py`

 * *Files identical despite different names*

### Comparing `qadence-1.5.0/qadence/ml_tools/models.py` & `qadence-1.5.1/qadence/ml_tools/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -285,16 +285,28 @@
             input_shifting=torch.tensor(d["_input_shifting"]),
             output_shifting=torch.tensor(d["_output_shifting"]),
         )
 
     def to(self, *args: Any, **kwargs: Any) -> TransformedModule:
         try:
             self.model = self.model.to(*args, **kwargs)
-            self._input_scaling = self._input_scaling.to(*args, **kwargs)
-            self._input_shifting = self._input_shifting.to(*args, **kwargs)
-            self._output_scaling = self._output_scaling.to(*args, **kwargs)
-            self._output_shifting = self._output_shifting.to(*args, **kwargs)
+            if isinstance(self.model, QuantumModel):
+                device = self.model._circuit.native.device
+                dtype = (
+                    torch.float64
+                    if self.model._circuit.native.dtype == torch.cdouble
+                    else torch.float32
+                )
 
+                self._input_scaling = self._input_scaling.to(device=device, dtype=dtype)
+                self._input_shifting = self._input_shifting.to(device=device, dtype=dtype)
+                self._output_scaling = self._output_scaling.to(device=device, dtype=dtype)
+                self._output_shifting = self._output_shifting.to(device=device, dtype=dtype)
+            elif isinstance(self.model, torch.nn.Module):
+                self._input_scaling = self._input_scaling.to(*args, **kwargs)
+                self._input_shifting = self._input_shifting.to(*args, **kwargs)
+                self._output_scaling = self._output_scaling.to(*args, **kwargs)
+                self._output_shifting = self._output_shifting.to(*args, **kwargs)
             logger.debug(f"Moved {self} to {args}, {kwargs}.")
         except Exception as e:
             logger.warning(f"Unable to move {self} to {args}, {kwargs} due to {e}.")
         return self
```

### Comparing `qadence-1.5.0/qadence/ml_tools/optimize_step.py` & `qadence-1.5.1/qadence/ml_tools/optimize_step.py`

 * *Files identical despite different names*

### Comparing `qadence-1.5.0/qadence/ml_tools/parameters.py` & `qadence-1.5.1/qadence/ml_tools/parameters.py`

 * *Files identical despite different names*

### Comparing `qadence-1.5.0/qadence/ml_tools/printing.py` & `qadence-1.5.1/qadence/ml_tools/printing.py`

 * *Files identical despite different names*

### Comparing `qadence-1.5.0/qadence/ml_tools/saveload.py` & `qadence-1.5.1/qadence/ml_tools/saveload.py`

 * *Files identical despite different names*

### Comparing `qadence-1.5.0/qadence/ml_tools/tensors.py` & `qadence-1.5.1/qadence/ml_tools/tensors.py`

 * *Files identical despite different names*

### Comparing `qadence-1.5.0/qadence/ml_tools/train_grad.py` & `qadence-1.5.1/qadence/ml_tools/train_grad.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from __future__ import annotations
 
 from typing import Callable, Union
 
 from rich.progress import BarColumn, Progress, TaskProgressColumn, TextColumn, TimeRemainingColumn
+from torch import complex128, float32, float64
 from torch import device as torch_device
 from torch import dtype as torch_dtype
 from torch.nn import DataParallel, Module
 from torch.optim import Optimizer
 from torch.utils.data import DataLoader
 from torch.utils.tensorboard import SummaryWriter
 
@@ -106,58 +107,66 @@
     )
     x = torch.linspace(0, 1, batch_size).reshape(-1, 1)
     y = torch.sin(x)
     data = to_dataloader(x, y, batch_size=batch_size, infinite=True)
     train_with_grad(model, data, optimizer, config, loss_fn=loss_fn)
     ```
     """
+    # load available checkpoint
+    init_iter = 0
+    if config.folder:
+        model, optimizer, init_iter = load_checkpoint(config.folder, model, optimizer)
+        logger.debug(f"Loaded model and optimizer from {config.folder}")
 
     # Move model to device before optimizer is loaded
     if isinstance(model, DataParallel):
         model = model.module.to(device=device, dtype=dtype)
     else:
         model = model.to(device=device, dtype=dtype)
-    # load available checkpoint
-    init_iter = 0
-    if config.folder:
-        model, optimizer, init_iter = load_checkpoint(config.folder, model, optimizer)
-        logger.debug(f"Loaded model and optimizer from {config.folder}")
     # initialize tensorboard
     writer = SummaryWriter(config.folder, purge_step=init_iter)
 
     ## Training
     progress = Progress(
         TextColumn("[progress.description]{task.description}"),
         BarColumn(),
         TaskProgressColumn(),
         TimeRemainingColumn(elapsed_when_finished=True),
     )
-
+    data_dtype = None
+    if dtype:
+        data_dtype = float64 if dtype == complex128 else float32
     with progress:
         dl_iter = iter(dataloader) if dataloader is not None else None
 
         # outer epoch loop
         for iteration in progress.track(range(init_iter, init_iter + config.max_iter)):
             try:
                 # in case there is not data needed by the model
                 # this is the case, for example, of quantum models
                 # which do not have classical input data (e.g. chemistry)
                 if dataloader is None:
                     loss, metrics = optimize_step(
-                        model=model, optimizer=optimizer, loss_fn=loss_fn, xs=None, device=device
+                        model=model,
+                        optimizer=optimizer,
+                        loss_fn=loss_fn,
+                        xs=None,
+                        device=device,
+                        dtype=data_dtype,
                     )
                     loss = loss.item()
 
                 elif isinstance(dataloader, (DictDataLoader, DataLoader)):
                     loss, metrics = optimize_step(
                         model=model,
                         optimizer=optimizer,
                         loss_fn=loss_fn,
                         xs=next(dl_iter),  # type: ignore[arg-type]
                         device=device,
+                        dtype=data_dtype,
                     )
 
                 else:
                     raise NotImplementedError(
                         f"Unsupported dataloader type: {type(dataloader)}. "
                         "You can use e.g. `qadence.ml_tools.to_dataloader` to build a dataloader."
                     )
```

### Comparing `qadence-1.5.0/qadence/ml_tools/train_no_grad.py` & `qadence-1.5.1/qadence/ml_tools/train_no_grad.py`

 * *Files identical despite different names*

### Comparing `qadence-1.5.0/qadence/ml_tools/utils.py` & `qadence-1.5.1/qadence/ml_tools/utils.py`

 * *Files identical despite different names*

### Comparing `qadence-1.5.0/qadence/models/qnn.py` & `qadence-1.5.1/qadence/models/qnn.py`

 * *Files identical despite different names*

### Comparing `qadence-1.5.0/qadence/models/quantum_model.py` & `qadence-1.5.1/qadence/models/quantum_model.py`

 * *Files 8% similar despite different names*

```diff
@@ -338,27 +338,30 @@
 
     def assign_parameters(self, values: dict[str, Tensor]) -> Any:
         """Return the final, assigned circuit that is used in e.g. `backend.run`."""
         params = self.embedding_fn(self._params, values)
         return self.backend.assign_parameters(self._circuit, params)
 
     def to(self, *args: Any, **kwargs: Any) -> QuantumModel:
+        from pyqtorch import QuantumCircuit as PyQCircuit
+
         try:
-            if isinstance(self._circuit.native, torch.nn.Module):
-                # Backends which are not torch-based cannot be moved to 'device'
+            if isinstance(self._circuit.native, PyQCircuit):
                 self._circuit.native = self._circuit.native.to(*args, **kwargs)
                 if self._observable is not None:
                     if isinstance(self._observable, ConvertedObservable):
                         self._observable.native = self._observable.native.to(*args, **kwargs)
                     elif isinstance(self._observable, list):
                         for obs in self._observable:
                             obs.native = obs.native.to(*args, **kwargs)
                 self._params = self._params.to(
                     device=self._circuit.native.device,
                     dtype=torch.float64
                     if self._circuit.native.dtype == torch.cdouble
                     else torch.float32,
                 )
                 logger.debug(f"Moved {self} to {args}, {kwargs}.")
+            else:
+                logger.debug("QuantumModel.to only supports pyqtorch.QuantumCircuits.")
         except Exception as e:
             logger.warning(f"Unable to move {self} to {args}, {kwargs} due to {e}.")
         return self
```

### Comparing `qadence-1.5.0/qadence/noise/protocols.py` & `qadence-1.5.1/qadence/noise/protocols.py`

 * *Files identical despite different names*

### Comparing `qadence-1.5.0/qadence/noise/readout.py` & `qadence-1.5.1/qadence/noise/readout.py`

 * *Files identical despite different names*

### Comparing `qadence-1.5.0/qadence/operations/__init__.py` & `qadence-1.5.1/qadence/operations/__init__.py`

 * *Files identical despite different names*

### Comparing `qadence-1.5.0/qadence/operations/analog.py` & `qadence-1.5.1/qadence/operations/analog.py`

 * *Files identical despite different names*

### Comparing `qadence-1.5.0/qadence/operations/control_ops.py` & `qadence-1.5.1/qadence/operations/control_ops.py`

 * *Files identical despite different names*

### Comparing `qadence-1.5.0/qadence/operations/ham_evo.py` & `qadence-1.5.1/qadence/operations/ham_evo.py`

 * *Files identical despite different names*

### Comparing `qadence-1.5.0/qadence/operations/parametric.py` & `qadence-1.5.1/qadence/operations/parametric.py`

 * *Files identical despite different names*

### Comparing `qadence-1.5.0/qadence/operations/primitive.py` & `qadence-1.5.1/qadence/operations/primitive.py`

 * *Files identical despite different names*

### Comparing `qadence-1.5.0/qadence/transpile/apply_fn.py` & `qadence-1.5.1/qadence/transpile/apply_fn.py`

 * *Files identical despite different names*

### Comparing `qadence-1.5.0/qadence/transpile/block.py` & `qadence-1.5.1/qadence/transpile/block.py`

 * *Files identical despite different names*

### Comparing `qadence-1.5.0/qadence/transpile/digitalize.py` & `qadence-1.5.1/qadence/transpile/digitalize.py`

 * *Files identical despite different names*

### Comparing `qadence-1.5.0/qadence/transpile/flatten.py` & `qadence-1.5.1/qadence/transpile/flatten.py`

 * *Files identical despite different names*

### Comparing `qadence-1.5.0/qadence/transpile/invert.py` & `qadence-1.5.1/qadence/transpile/invert.py`

 * *Files identical despite different names*

### Comparing `qadence-1.5.0/qadence/transpile/transpile.py` & `qadence-1.5.1/qadence/transpile/transpile.py`

 * *Files identical despite different names*

### Comparing `qadence-1.5.0/.gitignore` & `qadence-1.5.1/.gitignore`

 * *Files identical despite different names*

### Comparing `qadence-1.5.0/LICENSE` & `qadence-1.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `qadence-1.5.0/README.md` & `qadence-1.5.1/README.md`

 * *Files identical despite different names*

### Comparing `qadence-1.5.0/pyproject.toml` & `qadence-1.5.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     { name = "Roland Guichard", email = "roland.guichard@pasqal.com" },
     { name = "Joao P. Moutinho", email = "joao.moutinho@pasqal.com"},
     { name = "Vytautas Abramavicius", email = "vytautas.abramavicius@pasqal.com" },
     { name = "Gergana Velikova", email = "gergana.velikova@pasqal.com" },
 ]
 requires-python = ">=3.9,<3.13"
 license = {text = "Apache 2.0"}
-version = "1.5.0"
+version = "1.5.1"
 classifiers=[
     "License :: OSI Approved :: Apache Software License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
```

### Comparing `qadence-1.5.0/PKG-INFO` & `qadence-1.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: qadence
-Version: 1.5.0
+Version: 1.5.1
 Summary: Pasqal interface for circuit-based quantum computing SDKs
 Author-email: Aleksander Wennersteen <aleksander.wennersteen@pasqal.com>, Gert-Jan Both <gert-jan.both@pasqal.com>, Niklas Heim <niklas.heim@pasqal.com>, Mario Dagrada <mario.dagrada@pasqal.com>, Vincent Elfving <vincent.elfving@pasqal.com>, Dominik Seitz <dominik.seitz@pasqal.com>, Roland Guichard <roland.guichard@pasqal.com>, "Joao P. Moutinho" <joao.moutinho@pasqal.com>, Vytautas Abramavicius <vytautas.abramavicius@pasqal.com>, Gergana Velikova <gergana.velikova@pasqal.com>
 License: Apache 2.0
 License-File: LICENSE
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

