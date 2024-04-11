# Comparing `tmp/cryojax-0.2.2rc1.tar.gz` & `tmp/cryojax-0.2.3rc1.tar.gz`

## Comparing `cryojax-0.2.2rc1.tar` & `cryojax-0.2.3rc1.tar`

### file list

```diff
@@ -1,120 +1,119 @@
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 cryojax-0.2.2rc1/.gitattributes
--rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 cryojax-0.2.2rc1/.pre-commit-config.yaml
--rw-r--r--   0        0        0     2084 2020-02-02 00:00:00.000000 cryojax-0.2.2rc1/CONTRIBUTING.md
--rw-r--r--   0        0        0     2147 2020-02-02 00:00:00.000000 cryojax-0.2.2rc1/mkdocs.yml
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 cryojax-0.2.2rc1/.github/dependabot.yml
--rw-r--r--   0        0        0     1110 2020-02-02 00:00:00.000000 cryojax-0.2.2rc1/.github/workflows/build_docs.yml
--rw-r--r--   0        0        0      784 2020-02-02 00:00:00.000000 cryojax-0.2.2rc1/.github/workflows/release.yml
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 cryojax-0.2.2rc1/.github/workflows/ruff.yml
--rw-r--r--   0        0        0     1000 2020-02-02 00:00:00.000000 cryojax-0.2.2rc1/.github/workflows/testing.yml
--rw-r--r--   0        0        0     6069 2020-02-02 00:00:00.000000 cryojax-0.2.2rc1/docs/index.md
--rw-r--r--   0        0        0     3108 2020-02-02 00:00:00.000000 cryojax-0.2.2rc1/docs/_static/custom_css.css
--rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 cryojax-0.2.2rc1/docs/_static/mathjax.js
--rw-r--r--   0        0        0     2713 2020-02-02 00:00:00.000000 cryojax-0.2.2rc1/docs/api/simulator/scattering_potential.md
--rw-r--r--   0        0        0   511451 2020-02-02 00:00:00.000000 cryojax-0.2.2rc1/docs/examples/read-dataset.ipynb
--rw-r--r--   0        0        0     7539 2020-02-02 00:00:00.000000 cryojax-0.2.2rc1/docs/examples/simulate-helix.ipynb
--rw-r--r--   0        0        0   230609 2020-02-02 00:00:00.000000 cryojax-0.2.2rc1/docs/examples/simulate-image.ipynb
--rw-r--r--   0        0        0   136594 2020-02-02 00:00:00.000000 cryojax-0.2.2rc1/docs/examples/simulate-micrograph.ipynb
--rw-r--r--   0        0        0    13153 2020-02-02 00:00:00.000000 cryojax-0.2.2rc1/docs/examples/test-multiatom.ipynb
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cryojax-0.2.2rc1/docs/examples/data/.gitkeep
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 cryojax-0.2.2rc1/docs/examples/data/ribosome_4ug0_micrograph.mrc
--rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 cryojax-0.2.2rc1/docs/examples/data/ribosome_4ug0_micrograph.mrcs
--rw-r--r--   0        0        0     2019 2020-02-02 00:00:00.000000 cryojax-0.2.2rc1/docs/examples/data/ribosome_4ug0_particles.star
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 cryojax-0.2.2rc1/docs/examples/data/ribosome_4ug0_scattering_potential_from_cistem.mrc
--rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 cryojax-0.2.2rc1/src/cryojax/__init__.py
--rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 cryojax-0.2.2rc1/src/cryojax/cryojax_version.py
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 cryojax-0.2.2rc1/src/cryojax/constants/__init__.py
--rw-r--r--   0        0        0     1686 2020-02-02 00:00:00.000000 cryojax-0.2.2rc1/src/cryojax/constants/_load_atoms.py
--rw-r--r--   0        0        0     8048 2020-02-02 00:00:00.000000 cryojax-0.2.2rc1/src/cryojax/constants/element_params.npy
--rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 cryojax-0.2.2rc1/src/cryojax/coordinates/__init__.py
--rw-r--r--   0        0        0     8168 2020-02-02 00:00:00.000000 cryojax-0.2.2rc1/src/cryojax/coordinates/_coordinates.py
--rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 cryojax-0.2.2rc1/src/cryojax/core/__init__.py
--rw-r--r--   0        0        0      902 2020-02-02 00:00:00.000000 cryojax-0.2.2rc1/src/cryojax/core/_errors.py
--rw-r--r--   0        0        0      779 2020-02-02 00:00:00.000000 cryojax-0.2.2rc1/src/cryojax/core/_filter_specs.py
--rw-r--r--   0        0        0     3459 2020-02-02 00:00:00.000000 cryojax-0.2.2rc1/src/cryojax/core/_filtered_transformations.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cryojax-0.2.2rc1/src/cryojax/core/_serialization.py
--rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 cryojax-0.2.2rc1/src/cryojax/data/__init__.py
--rw-r--r--   0        0        0     2861 2020-02-02 00:00:00.000000 cryojax-0.2.2rc1/src/cryojax/data/_dataset.py
--rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 cryojax-0.2.2rc1/src/cryojax/data/_particle_stack.py
--rw-r--r--   0        0        0    17879 2020-02-02 00:00:00.000000 cryojax-0.2.2rc1/src/cryojax/data/_relion.py
--rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 cryojax-0.2.2rc1/src/cryojax/image/__init__.py
--rw-r--r--   0        0        0     3070 2020-02-02 00:00:00.000000 cryojax-0.2.2rc1/src/cryojax/image/_average.py
--rw-r--r--   0        0        0     5547 2020-02-02 00:00:00.000000 cryojax-0.2.2rc1/src/cryojax/image/_edges.py
--rw-r--r--   0        0        0     2779 2020-02-02 00:00:00.000000 cryojax-0.2.2rc1/src/cryojax/image/_fft.py
--rw-r--r--   0        0        0     8242 2020-02-02 00:00:00.000000 cryojax-0.2.2rc1/src/cryojax/image/_map_coordinates.py
--rw-r--r--   0        0        0     3523 2020-02-02 00:00:00.000000 cryojax-0.2.2rc1/src/cryojax/image/_normalize.py
--rw-r--r--   0        0        0     1814 2020-02-02 00:00:00.000000 cryojax-0.2.2rc1/src/cryojax/image/_rescale_pixel_size.py
--rw-r--r--   0        0        0     3946 2020-02-02 00:00:00.000000 cryojax-0.2.2rc1/src/cryojax/image/_spectrum.py
--rw-r--r--   0        0        0     1162 2020-02-02 00:00:00.000000 cryojax-0.2.2rc1/src/cryojax/image/operators/__init__.py
--rw-r--r--   0        0        0     6337 2020-02-02 00:00:00.000000 cryojax-0.2.2rc1/src/cryojax/image/operators/_filters.py
--rw-r--r--   0        0        0     6091 2020-02-02 00:00:00.000000 cryojax-0.2.2rc1/src/cryojax/image/operators/_fourier_operator.py
--rw-r--r--   0        0        0     3156 2020-02-02 00:00:00.000000 cryojax-0.2.2rc1/src/cryojax/image/operators/_masks.py
--rw-r--r--   0        0        0     6155 2020-02-02 00:00:00.000000 cryojax-0.2.2rc1/src/cryojax/image/operators/_operator.py
--rw-r--r--   0        0        0     2439 2020-02-02 00:00:00.000000 cryojax-0.2.2rc1/src/cryojax/image/operators/_real_operator.py
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 cryojax-0.2.2rc1/src/cryojax/inference/__init__.py
--rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 cryojax-0.2.2rc1/src/cryojax/inference/distributions/__init__.py
--rw-r--r--   0        0        0     1541 2020-02-02 00:00:00.000000 cryojax-0.2.2rc1/src/cryojax/inference/distributions/_distribution.py
--rw-r--r--   0        0        0     4084 2020-02-02 00:00:00.000000 cryojax-0.2.2rc1/src/cryojax/inference/distributions/_gaussian_distributions.py
--rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 cryojax-0.2.2rc1/src/cryojax/inference/transforms/__init__.py
--rw-r--r--   0        0        0     4109 2020-02-02 00:00:00.000000 cryojax-0.2.2rc1/src/cryojax/inference/transforms/_lie_group_transforms.py
--rw-r--r--   0        0        0     7636 2020-02-02 00:00:00.000000 cryojax-0.2.2rc1/src/cryojax/inference/transforms/_transforms.py
--rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 cryojax-0.2.2rc1/src/cryojax/io/__init__.py
--rw-r--r--   0        0        0     1584 2020-02-02 00:00:00.000000 cryojax-0.2.2rc1/src/cryojax/io/_cif.py
--rw-r--r--   0        0        0     3056 2020-02-02 00:00:00.000000 cryojax-0.2.2rc1/src/cryojax/io/_gemmi.py
--rw-r--r--   0        0        0     1008 2020-02-02 00:00:00.000000 cryojax-0.2.2rc1/src/cryojax/io/_mdtraj.py
--rw-r--r--   0        0        0     8227 2020-02-02 00:00:00.000000 cryojax-0.2.2rc1/src/cryojax/io/_mrc.py
--rw-r--r--   0        0        0     1861 2020-02-02 00:00:00.000000 cryojax-0.2.2rc1/src/cryojax/io/_pdb.py
--rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 cryojax-0.2.2rc1/src/cryojax/io/_starfile.py
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 cryojax-0.2.2rc1/src/cryojax/rotations/__init__.py
--rw-r--r--   0        0        0    16267 2020-02-02 00:00:00.000000 cryojax-0.2.2rc1/src/cryojax/rotations/_lie_group.py
--rw-r--r--   0        0        0     1934 2020-02-02 00:00:00.000000 cryojax-0.2.2rc1/src/cryojax/rotations/_rotation.py
--rw-r--r--   0        0        0     2557 2020-02-02 00:00:00.000000 cryojax-0.2.2rc1/src/cryojax/simulator/__init__.py
--rw-r--r--   0        0        0     6234 2020-02-02 00:00:00.000000 cryojax-0.2.2rc1/src/cryojax/simulator/_config.py
--rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 cryojax-0.2.2rc1/src/cryojax/simulator/_conformation.py
--rw-r--r--   0        0        0     6022 2020-02-02 00:00:00.000000 cryojax-0.2.2rc1/src/cryojax/simulator/_detector.py
--rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 cryojax-0.2.2rc1/src/cryojax/simulator/_dose.py
--rw-r--r--   0        0        0     2973 2020-02-02 00:00:00.000000 cryojax-0.2.2rc1/src/cryojax/simulator/_ice.py
--rw-r--r--   0        0        0     4959 2020-02-02 00:00:00.000000 cryojax-0.2.2rc1/src/cryojax/simulator/_instrument.py
--rw-r--r--   0        0        0     7463 2020-02-02 00:00:00.000000 cryojax-0.2.2rc1/src/cryojax/simulator/_optics.py
--rw-r--r--   0        0        0    16862 2020-02-02 00:00:00.000000 cryojax-0.2.2rc1/src/cryojax/simulator/_pipeline.py
--rw-r--r--   0        0        0    12418 2020-02-02 00:00:00.000000 cryojax-0.2.2rc1/src/cryojax/simulator/_pose.py
--rw-r--r--   0        0        0     5371 2020-02-02 00:00:00.000000 cryojax-0.2.2rc1/src/cryojax/simulator/_specimen.py
--rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 cryojax-0.2.2rc1/src/cryojax/simulator/_assembly/__init__.py
--rw-r--r--   0        0        0     4162 2020-02-02 00:00:00.000000 cryojax-0.2.2rc1/src/cryojax/simulator/_assembly/_assembly.py
--rw-r--r--   0        0        0    10414 2020-02-02 00:00:00.000000 cryojax-0.2.2rc1/src/cryojax/simulator/_assembly/_helix.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 cryojax-0.2.2rc1/src/cryojax/simulator/_integrators/__init__.py
--rw-r--r--   0        0        0     6600 2020-02-02 00:00:00.000000 cryojax-0.2.2rc1/src/cryojax/simulator/_integrators/_fourier_slice_extract.py
--rw-r--r--   0        0        0     4967 2020-02-02 00:00:00.000000 cryojax-0.2.2rc1/src/cryojax/simulator/_integrators/_gaussian_mixture.py
--rw-r--r--   0        0        0     3617 2020-02-02 00:00:00.000000 cryojax-0.2.2rc1/src/cryojax/simulator/_integrators/_nufft_project.py
--rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 cryojax-0.2.2rc1/src/cryojax/simulator/_integrators/_potential_integrator.py
--rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 cryojax-0.2.2rc1/src/cryojax/simulator/_potential/__init__.py
--rw-r--r--   0        0        0     1250 2020-02-02 00:00:00.000000 cryojax-0.2.2rc1/src/cryojax/simulator/_potential/_atom_potential.py
--rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 cryojax-0.2.2rc1/src/cryojax/simulator/_potential/_scattering_potential.py
--rw-r--r--   0        0        0    22372 2020-02-02 00:00:00.000000 cryojax-0.2.2rc1/src/cryojax/simulator/_potential/_voxel_potential.py
--rw-r--r--   0        0        0     2289 2020-02-02 00:00:00.000000 cryojax-0.2.2rc1/src/cryojax/typing/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cryojax-0.2.2rc1/tests/__init__.py
--rw-r--r--   0        0        0     3809 2020-02-02 00:00:00.000000 cryojax-0.2.2rc1/tests/conftest.py
--rw-r--r--   0        0        0     5826 2020-02-02 00:00:00.000000 cryojax-0.2.2rc1/tests/test_agree_with_cistem.py
--rw-r--r--   0        0        0     3678 2020-02-02 00:00:00.000000 cryojax-0.2.2rc1/tests/test_atom_routines.py
--rw-r--r--   0        0        0     1673 2020-02-02 00:00:00.000000 cryojax-0.2.2rc1/tests/test_detector.py
--rw-r--r--   0        0        0     1279 2020-02-02 00:00:00.000000 cryojax-0.2.2rc1/tests/test_distribution.py
--rw-r--r--   0        0        0     1351 2020-02-02 00:00:00.000000 cryojax-0.2.2rc1/tests/test_ensemble.py
--rw-r--r--   0        0        0     1285 2020-02-02 00:00:00.000000 cryojax-0.2.2rc1/tests/test_fft.py
--rw-r--r--   0        0        0     1572 2020-02-02 00:00:00.000000 cryojax-0.2.2rc1/tests/test_filters_and_masks.py
--rw-r--r--   0        0        0     5439 2020-02-02 00:00:00.000000 cryojax-0.2.2rc1/tests/test_helix.py
--rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 cryojax-0.2.2rc1/tests/test_jit.py
--rw-r--r--   0        0        0      971 2020-02-02 00:00:00.000000 cryojax-0.2.2rc1/tests/test_normalize.py
--rw-r--r--   0        0        0     2927 2020-02-02 00:00:00.000000 cryojax-0.2.2rc1/tests/test_pose_agreement.py
--rw-r--r--   0        0        0     3728 2020-02-02 00:00:00.000000 cryojax-0.2.2rc1/tests/test_potential.py
--rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 cryojax-0.2.2rc1/tests/test_projection_agreement.py
--rw-r--r--   0        0        0      920 2020-02-02 00:00:00.000000 cryojax-0.2.2rc1/tests/test_shape.py
--rw-r--r--   0        0        0     4436 2020-02-02 00:00:00.000000 cryojax-0.2.2rc1/tests/test_voxels_from_atoms.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cryojax-0.2.2rc1/tests/data/.gitkeep
--rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 cryojax-0.2.2rc1/tests/data/1uao.pdb
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 cryojax-0.2.2rc1/tests/data/3j9g_potential_ps4_4.mrc
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 cryojax-0.2.2rc1/tests/data/3j9g_subunit_potential_ps4_4.mrc
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 cryojax-0.2.2rc1/.gitignore
--rw-r--r--   0        0        0    26526 2020-02-02 00:00:00.000000 cryojax-0.2.2rc1/LICENSE
--rw-r--r--   0        0        0     7046 2020-02-02 00:00:00.000000 cryojax-0.2.2rc1/README.md
--rw-r--r--   0        0        0     1723 2020-02-02 00:00:00.000000 cryojax-0.2.2rc1/pyproject.toml
--rw-r--r--   0        0        0    38711 2020-02-02 00:00:00.000000 cryojax-0.2.2rc1/PKG-INFO
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 cryojax-0.2.3rc1/.gitattributes
+-rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 cryojax-0.2.3rc1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     2084 2020-02-02 00:00:00.000000 cryojax-0.2.3rc1/CONTRIBUTING.md
+-rw-r--r--   0        0        0     2147 2020-02-02 00:00:00.000000 cryojax-0.2.3rc1/mkdocs.yml
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 cryojax-0.2.3rc1/.github/dependabot.yml
+-rw-r--r--   0        0        0     1110 2020-02-02 00:00:00.000000 cryojax-0.2.3rc1/.github/workflows/build_docs.yml
+-rw-r--r--   0        0        0      784 2020-02-02 00:00:00.000000 cryojax-0.2.3rc1/.github/workflows/release.yml
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 cryojax-0.2.3rc1/.github/workflows/ruff.yml
+-rw-r--r--   0        0        0     1000 2020-02-02 00:00:00.000000 cryojax-0.2.3rc1/.github/workflows/testing.yml
+-rw-r--r--   0        0        0     6088 2020-02-02 00:00:00.000000 cryojax-0.2.3rc1/docs/index.md
+-rw-r--r--   0        0        0     3108 2020-02-02 00:00:00.000000 cryojax-0.2.3rc1/docs/_static/custom_css.css
+-rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 cryojax-0.2.3rc1/docs/_static/mathjax.js
+-rw-r--r--   0        0        0     2713 2020-02-02 00:00:00.000000 cryojax-0.2.3rc1/docs/api/simulator/scattering_potential.md
+-rw-r--r--   0        0        0   511451 2020-02-02 00:00:00.000000 cryojax-0.2.3rc1/docs/examples/read-dataset.ipynb
+-rw-r--r--   0        0        0     7539 2020-02-02 00:00:00.000000 cryojax-0.2.3rc1/docs/examples/simulate-helix.ipynb
+-rw-r--r--   0        0        0   230839 2020-02-02 00:00:00.000000 cryojax-0.2.3rc1/docs/examples/simulate-image.ipynb
+-rw-r--r--   0        0        0   137948 2020-02-02 00:00:00.000000 cryojax-0.2.3rc1/docs/examples/simulate-micrograph.ipynb
+-rw-r--r--   0        0        0    13153 2020-02-02 00:00:00.000000 cryojax-0.2.3rc1/docs/examples/test-multiatom.ipynb
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cryojax-0.2.3rc1/docs/examples/data/.gitkeep
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 cryojax-0.2.3rc1/docs/examples/data/ribosome_4ug0_micrograph.mrc
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 cryojax-0.2.3rc1/docs/examples/data/ribosome_4ug0_micrograph.mrcs
+-rw-r--r--   0        0        0     2019 2020-02-02 00:00:00.000000 cryojax-0.2.3rc1/docs/examples/data/ribosome_4ug0_particles.star
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 cryojax-0.2.3rc1/docs/examples/data/ribosome_4ug0_scattering_potential_from_cistem.mrc
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 cryojax-0.2.3rc1/src/cryojax/__init__.py
+-rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 cryojax-0.2.3rc1/src/cryojax/cryojax_version.py
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 cryojax-0.2.3rc1/src/cryojax/constants/__init__.py
+-rw-r--r--   0        0        0     1653 2020-02-02 00:00:00.000000 cryojax-0.2.3rc1/src/cryojax/constants/_load_atoms.py
+-rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 cryojax-0.2.3rc1/src/cryojax/constants/_unit_conversions.py
+-rw-r--r--   0        0        0     8048 2020-02-02 00:00:00.000000 cryojax-0.2.3rc1/src/cryojax/constants/element_params.npy
+-rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 cryojax-0.2.3rc1/src/cryojax/coordinates/__init__.py
+-rw-r--r--   0        0        0     8613 2020-02-02 00:00:00.000000 cryojax-0.2.3rc1/src/cryojax/coordinates/_coordinates.py
+-rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 cryojax-0.2.3rc1/src/cryojax/core/__init__.py
+-rw-r--r--   0        0        0      902 2020-02-02 00:00:00.000000 cryojax-0.2.3rc1/src/cryojax/core/_errors.py
+-rw-r--r--   0        0        0      779 2020-02-02 00:00:00.000000 cryojax-0.2.3rc1/src/cryojax/core/_filter_specs.py
+-rw-r--r--   0        0        0     3459 2020-02-02 00:00:00.000000 cryojax-0.2.3rc1/src/cryojax/core/_filtered_transformations.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cryojax-0.2.3rc1/src/cryojax/core/_serialization.py
+-rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 cryojax-0.2.3rc1/src/cryojax/data/__init__.py
+-rw-r--r--   0        0        0     2861 2020-02-02 00:00:00.000000 cryojax-0.2.3rc1/src/cryojax/data/_dataset.py
+-rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 cryojax-0.2.3rc1/src/cryojax/data/_particle_stack.py
+-rw-r--r--   0        0        0    17841 2020-02-02 00:00:00.000000 cryojax-0.2.3rc1/src/cryojax/data/_relion.py
+-rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 cryojax-0.2.3rc1/src/cryojax/image/__init__.py
+-rw-r--r--   0        0        0     3530 2020-02-02 00:00:00.000000 cryojax-0.2.3rc1/src/cryojax/image/_average.py
+-rw-r--r--   0        0        0     6259 2020-02-02 00:00:00.000000 cryojax-0.2.3rc1/src/cryojax/image/_edges.py
+-rw-r--r--   0        0        0     4644 2020-02-02 00:00:00.000000 cryojax-0.2.3rc1/src/cryojax/image/_fft.py
+-rw-r--r--   0        0        0     8242 2020-02-02 00:00:00.000000 cryojax-0.2.3rc1/src/cryojax/image/_map_coordinates.py
+-rw-r--r--   0        0        0     3659 2020-02-02 00:00:00.000000 cryojax-0.2.3rc1/src/cryojax/image/_normalize.py
+-rw-r--r--   0        0        0     1853 2020-02-02 00:00:00.000000 cryojax-0.2.3rc1/src/cryojax/image/_rescale_pixel_size.py
+-rw-r--r--   0        0        0     4549 2020-02-02 00:00:00.000000 cryojax-0.2.3rc1/src/cryojax/image/_spectrum.py
+-rw-r--r--   0        0        0     1162 2020-02-02 00:00:00.000000 cryojax-0.2.3rc1/src/cryojax/image/operators/__init__.py
+-rw-r--r--   0        0        0     7058 2020-02-02 00:00:00.000000 cryojax-0.2.3rc1/src/cryojax/image/operators/_filters.py
+-rw-r--r--   0        0        0     6598 2020-02-02 00:00:00.000000 cryojax-0.2.3rc1/src/cryojax/image/operators/_fourier_operator.py
+-rw-r--r--   0        0        0     3687 2020-02-02 00:00:00.000000 cryojax-0.2.3rc1/src/cryojax/image/operators/_masks.py
+-rw-r--r--   0        0        0     6563 2020-02-02 00:00:00.000000 cryojax-0.2.3rc1/src/cryojax/image/operators/_operator.py
+-rw-r--r--   0        0        0     2533 2020-02-02 00:00:00.000000 cryojax-0.2.3rc1/src/cryojax/image/operators/_real_operator.py
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 cryojax-0.2.3rc1/src/cryojax/inference/__init__.py
+-rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 cryojax-0.2.3rc1/src/cryojax/inference/distributions/__init__.py
+-rw-r--r--   0        0        0     1673 2020-02-02 00:00:00.000000 cryojax-0.2.3rc1/src/cryojax/inference/distributions/_distribution.py
+-rw-r--r--   0        0        0     4534 2020-02-02 00:00:00.000000 cryojax-0.2.3rc1/src/cryojax/inference/distributions/_gaussian_distributions.py
+-rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 cryojax-0.2.3rc1/src/cryojax/inference/transforms/__init__.py
+-rw-r--r--   0        0        0     4109 2020-02-02 00:00:00.000000 cryojax-0.2.3rc1/src/cryojax/inference/transforms/_lie_group_transforms.py
+-rw-r--r--   0        0        0     7634 2020-02-02 00:00:00.000000 cryojax-0.2.3rc1/src/cryojax/inference/transforms/_transforms.py
+-rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 cryojax-0.2.3rc1/src/cryojax/io/__init__.py
+-rw-r--r--   0        0        0     1584 2020-02-02 00:00:00.000000 cryojax-0.2.3rc1/src/cryojax/io/_cif.py
+-rw-r--r--   0        0        0     3056 2020-02-02 00:00:00.000000 cryojax-0.2.3rc1/src/cryojax/io/_gemmi.py
+-rw-r--r--   0        0        0     1008 2020-02-02 00:00:00.000000 cryojax-0.2.3rc1/src/cryojax/io/_mdtraj.py
+-rw-r--r--   0        0        0     8248 2020-02-02 00:00:00.000000 cryojax-0.2.3rc1/src/cryojax/io/_mrc.py
+-rw-r--r--   0        0        0     1861 2020-02-02 00:00:00.000000 cryojax-0.2.3rc1/src/cryojax/io/_pdb.py
+-rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 cryojax-0.2.3rc1/src/cryojax/io/_starfile.py
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 cryojax-0.2.3rc1/src/cryojax/rotations/__init__.py
+-rw-r--r--   0        0        0    16095 2020-02-02 00:00:00.000000 cryojax-0.2.3rc1/src/cryojax/rotations/_lie_group.py
+-rw-r--r--   0        0        0     1934 2020-02-02 00:00:00.000000 cryojax-0.2.3rc1/src/cryojax/rotations/_rotation.py
+-rw-r--r--   0        0        0     2445 2020-02-02 00:00:00.000000 cryojax-0.2.3rc1/src/cryojax/simulator/__init__.py
+-rw-r--r--   0        0        0     7374 2020-02-02 00:00:00.000000 cryojax-0.2.3rc1/src/cryojax/simulator/_config.py
+-rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 cryojax-0.2.3rc1/src/cryojax/simulator/_conformation.py
+-rw-r--r--   0        0        0     5580 2020-02-02 00:00:00.000000 cryojax-0.2.3rc1/src/cryojax/simulator/_detector.py
+-rw-r--r--   0        0        0      460 2020-02-02 00:00:00.000000 cryojax-0.2.3rc1/src/cryojax/simulator/_dose.py
+-rw-r--r--   0        0        0     2644 2020-02-02 00:00:00.000000 cryojax-0.2.3rc1/src/cryojax/simulator/_ice.py
+-rw-r--r--   0        0        0     6172 2020-02-02 00:00:00.000000 cryojax-0.2.3rc1/src/cryojax/simulator/_instrument.py
+-rw-r--r--   0        0        0     7413 2020-02-02 00:00:00.000000 cryojax-0.2.3rc1/src/cryojax/simulator/_optics.py
+-rw-r--r--   0        0        0    22542 2020-02-02 00:00:00.000000 cryojax-0.2.3rc1/src/cryojax/simulator/_pipeline.py
+-rw-r--r--   0        0        0    12243 2020-02-02 00:00:00.000000 cryojax-0.2.3rc1/src/cryojax/simulator/_pose.py
+-rw-r--r--   0        0        0     5615 2020-02-02 00:00:00.000000 cryojax-0.2.3rc1/src/cryojax/simulator/_specimen.py
+-rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 cryojax-0.2.3rc1/src/cryojax/simulator/_assembly/__init__.py
+-rw-r--r--   0        0        0     4110 2020-02-02 00:00:00.000000 cryojax-0.2.3rc1/src/cryojax/simulator/_assembly/_assembly.py
+-rw-r--r--   0        0        0    10346 2020-02-02 00:00:00.000000 cryojax-0.2.3rc1/src/cryojax/simulator/_assembly/_helix.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 cryojax-0.2.3rc1/src/cryojax/simulator/_integrators/__init__.py
+-rw-r--r--   0        0        0     6769 2020-02-02 00:00:00.000000 cryojax-0.2.3rc1/src/cryojax/simulator/_integrators/_fourier_slice_extract.py
+-rw-r--r--   0        0        0     4874 2020-02-02 00:00:00.000000 cryojax-0.2.3rc1/src/cryojax/simulator/_integrators/_gaussian_mixture.py
+-rw-r--r--   0        0        0     3723 2020-02-02 00:00:00.000000 cryojax-0.2.3rc1/src/cryojax/simulator/_integrators/_nufft_project.py
+-rw-r--r--   0        0        0     1237 2020-02-02 00:00:00.000000 cryojax-0.2.3rc1/src/cryojax/simulator/_integrators/_potential_integrator.py
+-rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 cryojax-0.2.3rc1/src/cryojax/simulator/_potential/__init__.py
+-rw-r--r--   0        0        0     1250 2020-02-02 00:00:00.000000 cryojax-0.2.3rc1/src/cryojax/simulator/_potential/_atom_potential.py
+-rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 cryojax-0.2.3rc1/src/cryojax/simulator/_potential/_scattering_potential.py
+-rw-r--r--   0        0        0    23788 2020-02-02 00:00:00.000000 cryojax-0.2.3rc1/src/cryojax/simulator/_potential/_voxel_potential.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cryojax-0.2.3rc1/tests/__init__.py
+-rw-r--r--   0        0        0     4168 2020-02-02 00:00:00.000000 cryojax-0.2.3rc1/tests/conftest.py
+-rw-r--r--   0        0        0     5945 2020-02-02 00:00:00.000000 cryojax-0.2.3rc1/tests/test_agree_with_cistem.py
+-rw-r--r--   0        0        0     3678 2020-02-02 00:00:00.000000 cryojax-0.2.3rc1/tests/test_atom_routines.py
+-rw-r--r--   0        0        0     1786 2020-02-02 00:00:00.000000 cryojax-0.2.3rc1/tests/test_detector.py
+-rw-r--r--   0        0        0     1514 2020-02-02 00:00:00.000000 cryojax-0.2.3rc1/tests/test_ensemble.py
+-rw-r--r--   0        0        0     1285 2020-02-02 00:00:00.000000 cryojax-0.2.3rc1/tests/test_fft.py
+-rw-r--r--   0        0        0     1572 2020-02-02 00:00:00.000000 cryojax-0.2.3rc1/tests/test_filters_and_masks.py
+-rw-r--r--   0        0        0     5952 2020-02-02 00:00:00.000000 cryojax-0.2.3rc1/tests/test_helix.py
+-rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 cryojax-0.2.3rc1/tests/test_jit.py
+-rw-r--r--   0        0        0      971 2020-02-02 00:00:00.000000 cryojax-0.2.3rc1/tests/test_normalize.py
+-rw-r--r--   0        0        0     2927 2020-02-02 00:00:00.000000 cryojax-0.2.3rc1/tests/test_pose_agreement.py
+-rw-r--r--   0        0        0     4044 2020-02-02 00:00:00.000000 cryojax-0.2.3rc1/tests/test_potential.py
+-rw-r--r--   0        0        0     1233 2020-02-02 00:00:00.000000 cryojax-0.2.3rc1/tests/test_projection_agreement.py
+-rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 cryojax-0.2.3rc1/tests/test_shape.py
+-rw-r--r--   0        0        0     4450 2020-02-02 00:00:00.000000 cryojax-0.2.3rc1/tests/test_voxels_from_atoms.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cryojax-0.2.3rc1/tests/data/.gitkeep
+-rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 cryojax-0.2.3rc1/tests/data/1uao.pdb
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 cryojax-0.2.3rc1/tests/data/3j9g_potential_ps4_4.mrc
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 cryojax-0.2.3rc1/tests/data/3j9g_subunit_potential_ps4_4.mrc
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 cryojax-0.2.3rc1/.gitignore
+-rw-r--r--   0        0        0    26526 2020-02-02 00:00:00.000000 cryojax-0.2.3rc1/LICENSE
+-rw-r--r--   0        0        0     7066 2020-02-02 00:00:00.000000 cryojax-0.2.3rc1/README.md
+-rw-r--r--   0        0        0     1723 2020-02-02 00:00:00.000000 cryojax-0.2.3rc1/pyproject.toml
+-rw-r--r--   0        0        0    38731 2020-02-02 00:00:00.000000 cryojax-0.2.3rc1/PKG-INFO
```

### Comparing `cryojax-0.2.2rc1/.pre-commit-config.yaml` & `cryojax-0.2.3rc1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `cryojax-0.2.2rc1/CONTRIBUTING.md` & `cryojax-0.2.3rc1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `cryojax-0.2.2rc1/mkdocs.yml` & `cryojax-0.2.3rc1/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `cryojax-0.2.2rc1/.github/workflows/build_docs.yml` & `cryojax-0.2.3rc1/.github/workflows/build_docs.yml`

 * *Files identical despite different names*

### Comparing `cryojax-0.2.2rc1/.github/workflows/release.yml` & `cryojax-0.2.3rc1/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `cryojax-0.2.2rc1/.github/workflows/testing.yml` & `cryojax-0.2.3rc1/.github/workflows/testing.yml`

 * *Files identical despite different names*

### Comparing `cryojax-0.2.2rc1/docs/index.md` & `cryojax-0.2.3rc1/docs/index.md`

 * *Files 2% similar despite different names*

```diff
@@ -81,19 +81,19 @@
 from cryojax.image import operators as op
 
 # First, initialize the CTF and its optics model
 ctf = cs.CTF(
     defocus_u_in_angstroms=10000.0,
     defocus_v_in_angstroms=9800.0,
     astigmatism_angle=10.0,
-    voltage_in_kilovolts=300.0,
     amplitude_contrast_ratio=0.1)
 optics = cs.WeakPhaseOptics(ctf, envelope=op.FourierGaussian(b_factor=5.0))  # b_factor is given in Angstroms^2
 # ... these are stored in the Instrument
-instrument = cs.Instrument(optics)
+voltage_in_kilovolts = 300.0
+instrument = cs.Instrument(voltage_in_kilovolts, optics)
 ```
 
 The `CTF` has all parameters used in CTFFIND4, which take their default values if not
 explicitly configured here. Finally, we can instantiate the `ImagePipeline` and simulate an image.
 
 ```python
 # Instantiate the image configuration
```

### Comparing `cryojax-0.2.2rc1/docs/_static/custom_css.css` & `cryojax-0.2.3rc1/docs/_static/custom_css.css`

 * *Files identical despite different names*

### Comparing `cryojax-0.2.2rc1/docs/api/simulator/scattering_potential.md` & `cryojax-0.2.3rc1/docs/api/simulator/scattering_potential.md`

 * *Files identical despite different names*

### Comparing `cryojax-0.2.2rc1/docs/examples/read-dataset.ipynb` & `cryojax-0.2.3rc1/docs/examples/read-dataset.ipynb`

 * *Files identical despite different names*

### Comparing `cryojax-0.2.2rc1/docs/examples/simulate-helix.ipynb` & `cryojax-0.2.3rc1/docs/examples/simulate-helix.ipynb`

 * *Files identical despite different names*

### Comparing `cryojax-0.2.2rc1/docs/examples/simulate-image.ipynb` & `cryojax-0.2.3rc1/docs/examples/simulate-image.ipynb`

 * *Files 14% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9978908648786469%*

 * *Differences: {"'cells'": "{10: {'source': {insert: [(1, 'voltage_in_kilovolts = 300.0\\n'), (12, "*

 * *            "'instrument_with_dose = cs.Instrument(voltage_in_kilovolts, dose=dose)\\n'), (13, "*

 * *            "'instrument_with_optics = cs.Instrument(voltage_in_kilovolts, dose=dose, "*

 * *            "optics=optics)\\n'), (14, 'instrument_with_detector = cs.Instrument(\\n'), (15, '    "*

 * *            "voltage_in_kilovolts, dose=dose, optics=optics, detector=detector\\n'), (16, ')')], "*

 * *            "delete: [12, 11]}}, 12: {'sou […]*

```diff
@@ -117,26 +117,30 @@
         {
             "cell_type": "code",
             "execution_count": 7,
             "metadata": {},
             "outputs": [],
             "source": [
                 "# Initialize the instrument\n",
+                "voltage_in_kilovolts = 300.0\n",
                 "dose = cs.ElectronDose(electrons_per_angstrom_squared=100.0)\n",
                 "optics = cs.WeakPhaseOptics(\n",
                 "    ctf=cs.CTF(\n",
                 "        defocus_u_in_angstroms=10000.0,\n",
                 "        defocus_v_in_angstroms=9000.0,\n",
                 "        astigmatism_angle=20.0,\n",
                 "        amplitude_contrast_ratio=0.07,\n",
                 "    )\n",
                 ")\n",
                 "detector = cs.PoissonDetector(dqe=cs.IdealDQE(fraction_detected_electrons=1.0))\n",
-                "instrument_with_optics = cs.Instrument(optics)\n",
-                "instrument_with_optics_and_detector = cs.Instrument(optics, dose, detector)"
+                "instrument_with_dose = cs.Instrument(voltage_in_kilovolts, dose=dose)\n",
+                "instrument_with_optics = cs.Instrument(voltage_in_kilovolts, dose=dose, optics=optics)\n",
+                "instrument_with_detector = cs.Instrument(\n",
+                "    voltage_in_kilovolts, dose=dose, optics=optics, detector=detector\n",
+                ")"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "Optionally, we can choose a model for the solvent. Here, we model the ice as gaussian colored noise with `GaussianIce` and choose an analytical model for the power spectrum taken from the `cryojax.image.operators` module. Here, we choose the `Lorenzian`, whose abstract base class is an `AbstractFourierOperator`."
@@ -144,59 +148,59 @@
         },
         {
             "cell_type": "code",
             "execution_count": 8,
             "metadata": {},
             "outputs": [],
             "source": [
-                "# Then, choose a model for the solvent scattering potential. The amplitude is the\n",
-                "# (squared) characteristic phase shift from the scattering potential, and the scale is\n",
-                "# the characteristic length scale of the potential.\n",
+                "# Then, choose a model for the solvent. The amplitude is the\n",
+                "# (squared) characteristic phase shift of the ice phase shifts, and the length_scale is\n",
+                "# their characteristic length scale.\n",
                 "solvent = cs.GaussianIce(\n",
                 "    variance=op.Lorenzian(amplitude=0.005**2, length_scale=2.0 * potential.voxel_size)\n",
                 ")"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "Finally, we create an `ImageConfig` and initialize our `ImagePipeline`. In this example, we would like to simulate images at each stage of the image formation process. This is controlled by the modeling complexity in the `Instrument`, which here has three levels.\n",
                 "\n",
-                "**1. If there is no `Instrument`:** In this case, the returned \"image\" is the scattering potential in the exit plane.\n",
+                "**1. If the `Instrument` just has an accelerating voltage and a dose:** In this case, the returned \"image\" is the phase shifts in the exit plane.\n",
                 "\n",
-                "**2. If the `Instrument` just has an optics model:** The returned \"image\" here is the squared wavefunction in the detector plane.\n",
+                "**2. If the `Instrument` also has an optics model:** The returned \"image\" here is the squared wavefunction in the detector plane.\n",
                 "\n",
-                "**3. If the `Instrument` has optics, dose, and detector models:** Last, the returned \"image\" is the detector readout."
+                "**3. If the `Instrument` also has a detector model:** Last, the returned \"image\" is the detector readout."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 9,
             "metadata": {},
             "outputs": [],
             "source": [
                 "# Create the image configuration\n",
                 "config = cs.ImageConfig(\n",
                 "    shape=(80, 80), pixel_size=potential.voxel_size, padded_shape=potential.shape[:2]\n",
                 ")\n",
                 "# ... now, build the image formation models\n",
                 "scattering_pipeline = cs.ImagePipeline(\n",
-                "    config=config, specimen=specimen, solvent=solvent\n",
+                "    config=config, specimen=specimen, instrument=instrument_with_dose, solvent=solvent\n",
                 ")\n",
                 "optics_pipeline = cs.ImagePipeline(\n",
                 "    config=config,\n",
                 "    specimen=specimen,\n",
                 "    instrument=instrument_with_optics,\n",
                 "    solvent=solvent,\n",
                 ")\n",
                 "detector_pipeline = cs.ImagePipeline(\n",
                 "    config=config,\n",
                 "    specimen=specimen,\n",
-                "    instrument=instrument_with_optics_and_detector,\n",
+                "    instrument=instrument_with_detector,\n",
                 "    solvent=solvent,\n",
                 ")"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
@@ -240,15 +244,15 @@
         {
             "cell_type": "code",
             "execution_count": 11,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
-                        "image/png": "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VKgQHn74YWTNmhWffPIJ2rdvj4kTJ+L66693ytWnTx9ceeWVeOKJJ7Bz504MHz4cvXv3xvjx4wEAw4cPR58+fZAtWzY8+uijAIB8+fJFvM8JEybgxIkT6NmzJ3LlyoXly5fj1VdfxU8//YQJEyYku75Scr27774be/fuxaxZszB27NhkXXfs2LHo0qUL4uPj8dxzz+HEiRN44403UK9ePaxZswbFihVDkyZNcO+992Lo0KFo3749qlatin379qFPnz5o1qwZ7rnnnkSv3aBBA/Tt2xevvPIKHnnkEZQrVw4A/P8jce7cObRs2RLXXnstnn/+eUyfPh1PPPEEzp49iyFDhkT83IoVK7B48WJ06tQJV111FXbu3Ik33ngDjRo1wqZNm8J+cUqqzZNbP0bqkBJbfdddd+GDDz7Arbfeijp16mDu3Llo06bNRX3/G2+8gQoVKuC6665D+vTpMXnyZNx7771ISEhAr169nHO3bNmCW265BXfffTe6d++OMmXK4MSJE2jYsCH27NmDu+++G0WKFMHixYsxYMAA7Nu3z1/S7nke/vWvf2HRokW45557UK5cOXz++efo0qVLkmW84oorULFiRSxYsAB9+/YFcN62R0VF4ddff8WmTZtQoUIFAMDChQt9HwMkz8bcdNNNePDBB/HJJ5/ggQcecL77k08+QYsWLfzQu+T4q7vvvhuFChXCM888g759+6JGjRqBdjWIcePG4ffff8fdd9+NqKgoPP/887jhhhvwww8/IEOGDACAdevWoX79+siQIQN69OiBYsWKYfv27Zg8eTKefvpp3HDDDdi6dSs++ugjDBs2DLlz5waAiD7uwIEDqFOnDk6cOIG+ffsiV65cGDNmDK677jp8+umnYX7m2WefRXR0NP773//iyJEjeP7559G5c2csW7Ys8N6SY9suxN7OnDkTHTp0QPny5TF06FD88ssv6Nq1K6666qqwc++++26MHj0aXbt2Rd++fbFjxw689tprWLNmDb755htkyJAh0E8mt/8DwJ133onRo0ejVatWuOuuu3D27FksXLgQS5cuRfXq1TF27FjcddddqFmzJnr06AEAKFGiBIDzvr9+/fqIjY3Fgw8+iAwZMuDNN99Eo0aN8PXXX6NWrVrOfd17773IkycPBg4ciOPHjwe2A3B+xWZUVBQeeughHDx4EMOHD0ezZs2wdu3awFUQL7/8Mq677jp07twZp0+fxscff4yOHTviq6++CrNNyZmPHThwANdeey2ioqLQu3dv5MmTB9OmTcOdd96Jo0ePol+/fknei2GkNrfddhseeeQRzJw5E927dweQvPl6UvYtuXO1i/UBd911F8aMGYMbb7wR//nPf7Bs2TIMHToUmzdvxueff+7ca2LzgCB++eUXtGrVCp06dcK///1v5MuXDwkJCbjuuuuwaNEi9OjRA+XKlcP69esxbNgwbN261QlhTu4cZeDAgXjqqafQunVrtG7dGqtXr0aLFi1w+vRppzwp9W9JEenZ1zAuKZf7rdjFMHPmTC9dunReunTpvNq1a3sPPvigN2PGDO/06dPOedu2bfOio6O966+/PuxXPf71WVfCeJ7n3X333V6WLFmct9pt2rRJ9A3xihUrEv01PCEhwStVqpQXHx8f9n1xcXFe8+bN/b+F3vTfcsstYdePtFIqJibG+/777/2/ffvttx4A79VXX/X/1q5dOy9Llizenj17/L9t27bNS58+fbJXSgHw/ve///l/O3XqlFelShUvb968fp0PHz7cA+B98MEH/nmnT5/2ateu7WXLls07evSo53nnVwBAVj6EaNq0qVepUiWnzhMSErw6dep4pUqV8v8WesPfrFkzp17vv/9+L126dN7hw4f9v1WoUCHRX+4TWymVWD8YOnSoFxUV5e3atcv/W3JXSiX3er169UrW9TzP837//Xfviiuu8Lp37+78ff/+/V6OHDmcvx8/ftwrWbKkV6FCBe+PP/7w2rRp48XGxjrf7XnhKwkmTJiQrF/rQ4RWTvTp08f/W0JCgtemTRsvJibGO3TokP93bfvE6mjJkiUeAO/999/3/5bcNk9J/Rh/Psm11WvXrvUAePfee6/z91tvvfWiVkol1r/i4+O94sWLO38LrRaZPn268/cnn3zSy5o1q7d161bn7w8//LCXLl06f7XFpEmTPADe888/759z9uxZr379+kmulPK88zaAV0D179/fa9CggZc3b15/Veovv/ziRUVFOSuqkmtjateu7VWrVs05b/ny5c44S4m/CtlPXTWS0pVSuXLlclbtfPHFFx4Ab/Lkyf7fGjRo4GXPnj3MbnEZQ6vB9Fdfzwu3b/369fMAeAsXLvT/9vvvv3txcXFesWLF/LlC6B7LlSvnnTp1yj/35Zdf9gB469evD/suJrm2LaX2tkqVKl6BAgUcPzdz5sywX7AXLlzoAfA+/PBD5/PTp08P+3skP5nc/j937lwPgNe3b9+wa3A7Zc2aNexXfc/zvPbt23sxMTHe9u3b/b/t3bvXy549u9egQQP/byE/UK9ePWcleyRCbVioUCF/DuJ5nvfJJ594AJyxlJhd0TY8ffq0V7FiRa9JkybO35M7H7vzzju9AgUKeD///LPz+U6dOnk5cuRItM8Yxp9NUiulPM/zcuTI4V1zzTV+Ornz9Uj2LSVztYvxAaG5xV133eX8/b///a8HwJs7d67/t0jzgEiEno9Gjhzp/H3s2LFedHS042M8z/NGjhzpAfC++eYb/2/JmaMcPHjQi4mJ8dq0aePc8yOPPBK24jS5/i25K6U8L/Kzr2FcKv7SQufNmzfHkiVLcN111+Hbb7/F888/j/j4eBQqVAhffvmlf96kSZOQkJCAgQMHIjraveWoqCj/mH8p+/333/Hzzz+jfv36OHHiBL777rsLLufatWuxbds23Hrrrfjll1/w888/4+eff8bx48fRtGlTLFiwAAkJCc5nIq1gSYxmzZr5vzQC51ccxcbG4ocffgBwfvXK7Nmz0b59exQsWNA/r2TJkmjVqlWyvyd9+vS4++67/XRMTAzuvvtuHDx4EKtWrQJwXqw7f/78uOWWW/zzMmTIgL59++LYsWP4+uuvA7/j119/xdy5c3HTTTf5bfDzzz/jl19+QXx8PLZt24Y9e/Y4n+nRo4fTjvXr18e5c+ewa9euZN8bw/3g+PHj+Pnnn1GnTh14noc1a9Zc9usBwKxZs3D48GHccsstfh39/PPPSJcuHWrVqoV58+b552bJkgWjR4/G5s2b0aBBA0yZMgXDhg1DkSJFLui7k6J3797+ceiX4NOnT2P27NkRP8N1dObMGfzyyy8oWbIkrrjiCqxevTrs/KTaPCX1Y/z5JNdWT506FQD8lUIhLnblAPevI0eO4Oeff0bDhg3xww8/4MiRI865cXFxiI+Pd/42YcIE1K9fH1deeaXTn5o1a4Zz585hwYIFfvnTp0+Pnj17+p9Nly6dLxabFPXr18eBAwewZcsWAOdXRDVo0AD169fHwoULAZxfieF5nrNSKrk25uabb8aqVauwfft2/2/jx49HxowZ8a9//QvAhfmri+Xmm292BNJD9xbyYYcOHcKCBQvQrVu3MLvFdiAlTJ06FTVr1kS9evX8v2XLlg09evTAzp07sWnTJuf8rl27IiYmJmIZI5FS25Yc9u3bh7Vr16JLly7IkSOH//fmzZujfPnyzrkTJkxAjhw50Lx5c6fvVqtWDdmyZUuWLUxu/584cSKioqLwxBNPhF0jqXY6d+4cZs6cifbt26N48eL+3wsUKIBbb70VixYtwtGjR53PdO/eHenSpUuy/CFuv/12ZM+e3U/feOONKFCggG93IsFt+Ntvv+HIkSOoX79+ou2X1HzM8zxMnDgR7dq1g+d5Tn3Gx8fjyJEjF9wvDOPPJlu2bP4ufBcyX1eSO1e7WB8QGuP9+/d3/v6f//wHADBlyhTn74nNA4LImDEjunbt6vxtwoQJKFeuHMqWLevcW5MmTQDAsb3JmaPMnj0bp0+fRp8+fZx7Tmx+lFL/Zhhpgb90+B4A1KhRA5999hlOnz6Nb7/9Fp9//jmGDRuGG2+8EWvXrkX58uWxfft2REdHh03WlI0bN+Kxxx7D3LlzwyY/+uCSErZt2wYAgSEcR44ccSblcXFxyb5+Yi8XrrzySvz2228AzovRnjx5EiVLlgw7L7G/RaJgwYJhQqKlS5cGAOzcuRPXXnstdu3ahVKlSoW9/Ast003qRdH3338Pz/Pw+OOP4/HHH0/0nIMHD6JQoUJ+Wu8/VI+h+08pu3fvxsCBA/Hll1+GXeNC+sGlvh7w/30q5NyU2NhYJ123bl307NkTI0aMQHx8vB9ueamJjo52HigAt49E4uTJkxg6dChGjRqFPXv2OCGridVRUm2e0vox/nySY6t37dqF6Oho56EOQJJL55Pim2++wRNPPIElS5bgxIkTTt6RI0ecB/vEbO+2bduwbt26iKFgIcHvXbt2oUCBAmHL2pNb/tCLjoULF+Kqq67CmjVr8NRTTyFPnjx48cUX/bzY2FhUrlzZ/1xybUzHjh3Rv39/jB8/Ho888gg8z8OECRPQqlUrf0xciL+6WJIaz6EH+qRCP1PCrl27wsLBANdX8fddqJ9JqW1LbtkBoFSpUmF5ZcqUcV5qbNu2DUeOHEHevHkTvVZyNhpIbv/fvn07ChYsiJw5cyZ5TeXQoUM4ceJEomOlXLlySEhIwI8//uiHsAIpmycB4fUVFRWFkiVLJrkj2FdffYWnnnoKa9euxalTp5zPK0nNxw4dOoTDhw/jrbfewltvvZXo96XlzR+MfzbHjh3zbcmFzNeV5M7VLtYHhOYW+syTP39+XHHFFWHPJim1LYUKFXJ+tADO39vmzZuTtJtA8uYokex+njx5wvxxSv2bYaQF/vIvpULExMSgRo0aqFGjBkqXLo2uXbtiwoQJif5ilxiHDx9Gw4YNERsbiyFDhqBEiRLIlCkTVq9ejYceeuiifhkOffaFF15AlSpVEj1HH2JSsstDpF8KefL7VyFUV//9738j/kqhTuVS3v+5c+fQvHlz/Prrr3jooYdQtmxZZM2aFXv27MEdd9yR4n5wqa8XIvS5sWPHIn/+/GH5ukvjqVOnMH/+fADnHxzS2s4gffr0wahRo9CvXz/Url0bOXLkQFRUFDp16pRoHSXV5imtHyP1uFhbHSLSr6Pnzp1z0tu3b0fTpk1RtmxZvPTSSyhcuDBiYmIwdepUDBs2LKx/JWZ7ExIS0Lx5czz44IOJfmfoxevFUrBgQcTFxWHBggUoVqwYPM9D7dq1kSdPHtx3333YtWsXFi5ciDp16vgv/lNiYwoWLIj69evjk08+wSOPPIKlS5di9+7deO6555x7BVLmr5SoqKhE7a+2TYi/gg+70DKm1LZdahISEpA3b158+OGHieYnR1cytfp/SkmNHcAWLlyI6667Dg0aNMDrr7+OAgUKIEOGDBg1ahTGjRsXdn5yfdO///3viC9+Q/qahpGW+Omnn3DkyBF/Dn4h83UltedqyV1Zm1LbEmneUKlSJbz00kuJfqZw4cIAUj5HuZQkdx5lGKnB3/LJLLSV6b59+wCcF9FMSEjApk2bIk6y58+fj19++QWfffYZGjRo4P99x44dYedGGsSR/h761T82NhbNmjVL9n1cKvLmzYtMmTLh+++/D8tL7G+R2Lt3b9i2y1u3bgUAX4iwaNGiWLduHRISEpzVUqHwx6JFiwKIXFehVTYZMmS4pHWVXEe0fv16bN26FWPGjMHtt9/u/33WrFkX9L0puV5KwlBCfSpv3rzJqqcnnngCmzdvxosvvoiHHnoIDz/8MF555ZXAz1xIWExCQgJ++OEH5yFF+0hifPrpp+jSpQv+97//+X/7448/cPjw4RSXAUh5/RiXB7XVRYsWRUJCArZv3+6smAiFszFXXnllov1Df/GcPHkyTp06hS+//NJZxZCSEM4SJUrg2LFjSfalokWLYs6cOTh27Jjz4iax8keifv36WLBgAeLi4lClShVkz54dlStXRo4cOTB9+nSsXr0agwcP9s9Pqc26+eabce+992LLli0YP348smTJgnbt2jn3Clycv7ryyisTDWu70JDqkF/YsGFD4HkpsVlFixZNtF3UV10sybVtKS078P+rDBi9pxIlSmD27NmoW7dukg9aQXOY5PT/EiVKYMaMGfj1118DV0sl9j158uRBlixZIrZJdHS0/xB3oWh9eZ6H77//PvAl0MSJE5EpUybMmDEDGTNm9P8+atSoCypDnjx5kD17dpw7d858k/GXIrQJT+gFVErm60k9HyU1V7tYHxCaW2zbts3ZQOLAgQM4fPjwJbP3TIkSJfDtt9+iadOmgfY9uXMUtvsckXDo0KGwFbvJ9W+hFVbqjxLz1RcaKm8YyeUvrSk1b968RH+lDMUOhx5q2rdvj+joaAwZMiTsjXPo86Fft/h6p0+fxuuvvx52/axZsya67D70skYHd7Vq1VCiRAm8+OKLOHbsWNjnDh06FPEeLwXp0qVDs2bNMGnSJOzdu9f/+/fff49p06Yl+zpnz57Fm2++6adPnz6NN998E3ny5EG1atUAAK1bt8b+/fudXdDOnj2LV199FdmyZUPDhg0BwF+lo3WVN29eNGrUCG+++ab/oMpcaF1lzZo1WS84EusHnufh5ZdfvqDvTcn1IvWfxIiPj0dsbCyeeeYZnDlzJiyf62nZsmV48cUX0a9fP/znP//BAw88gNdeey1Jfa+UlId57bXX/GPP8/Daa68hQ4YMaNq0acTPpEuXLmwsv/rqqxf8a01K6sf480murQ5p3OkLU97dK0SJEiVw5MgRrFu3zv/bvn37wnbRSWwMHjlyJEUPlTfddBOWLFmCGTNmhOUdPnwYZ8+eBXDe/p09exZvvPGGn3/u3Dm8+uqryf6u+vXrY+fOnRg/frwfzhcdHY06dergpZdewpkzZxw9qZTarA4dOiBdunT46KOPMGHCBLRt29b5oeFS+KsSJUrgu+++c8799ttv8c033yT52cTIkycPGjRogPfeew+7d+928vi+U2KzWrdujeXLl2PJkiX+344fP4633noLxYoVSzLcP7kk17alpOwFChRAlSpVMGbMGGcuMmvWrDCtkJtuugnnzp3Dk08+GXads2fPOt8XyU8mt/936NABnuc5L01DaDvp96RLlw4tWrTAF1984YTTHThwAOPGjUO9evUuOuz6/fff9/VwgPMvDPft2xeorZkuXTpERUU57bVz505n56yUkC5dOnTo0AETJ05M9AHbfJORFpk7dy6efPJJxMXFoXPnzgBSNl+PZN+SO1e7WB/QunVrAOFzidAqpovd4TcxbrrpJuzZswdvv/12WN7Jkyf9HUOTO0dp1qwZMmTIgFdffdU5N7H5UXL9W+ilYEgXEDg/Z0kstDjSs69hXCr+0iul+vTpgxMnTuD6669H2bJlcfr0aSxevBjjx49HsWLFfNG5kiVL4tFHH8WTTz6J+vXr44YbbkDGjBmxYsUKFCxYEEOHDkWdOnVw5ZVXokuXLujbty+ioqIwduzYRB+kqlWrhvHjx6N///6oUaMGsmXLhnbt2qFEiRK44oorMHLkSGTPnh1Zs2ZFrVq1EBcXh3feeQetWrVChQoV0LVrVxQqVAh79uzBvHnzEBsbi8mTJ/+pdTVo0CDMnDnT1xY6d+4cXnvtNVSsWBFr165N1jUKFiyI5557Djt37kTp0qUxfvx4rF27Fm+99Za/bXePHj3w5ptv4o477sCqVatQrFgxfPrpp/jmm28wfPhwX2Q0c+bMKF++PMaPH4/SpUsjZ86cqFixIipWrIgRI0agXr16qFSpErp3747ixYvjwIEDWLJkCX766Sd8++23Kb7/atWq4Y033sBTTz2FkiVLIm/evInGsJctWxYlSpTAf//7X+zZswexsbGYOHHiBetTpeR6oRd7ffv2RXx8PNKlS4dOnTolet3Y2Fi88cYbuO2221C1alV06tQJefLkwe7duzFlyhTUrVsXr732Gv744w906dIFpUqVwtNPPw0AGDx4MCZPnoyuXbti/fr1YTphIapUqYJ06dLhueeew5EjR5AxY0Y0adIkojYJAGTKlAnTp09Hly5dUKtWLUybNg1TpkzBI488Ehgm0rZtW4wdOxY5cuRA+fLlsWTJEsyePdvfQjulJLd+jNQhuba6SpUquOWWW/D666/jyJEjqFOnDubMmZPois5OnTrhoYcewvXXX4++ffv620iXLl3a0dRp0aIFYmJi0K5dO9x99904duwY3n77beTNmzfRiXRiPPDAA/jyyy/Rtm1b3HHHHahWrRqOHz+O9evX49NPP8XOnTuRO3dutGvXDnXr1sXDDz+MnTt3onz58vjss89SNJELvXDasmULnnnmGf/vDRo0wLRp05AxY0bUqFHD/3tKbVbevHnRuHFjvPTSS/j9999x8803O/nR0dEX7a+6deuGl156CfHx8bjzzjtx8OBBjBw5EhUqVAjTa0wur7zyCurVq4eqVauiR48eiIuLw86dOzFlyhTfh4Vs6KOPPopOnTohQ4YMaNeuXaI27uGHH8ZHH32EVq1aoW/fvsiZMyfGjBmDHTt2YOLEiWG6iBdKcm1bSu3t0KFD0aZNG9SrVw/dunXDr7/+ildffRUVKlRwXiY2bNgQd999N4YOHYq1a9eiRYsWyJAhA7Zt24YJEybg5Zdfxo033ujXX2J+Mrn9v3HjxrjtttvwyiuvYNu2bWjZsiUSEhKwcOFCNG7c2N8Eo1q1apg9ezZeeuklP2S1Vq1aeOqppzBr1izUq1cP9957L9KnT48333wTp06dwvPPP3/RbZEzZ07Uq1cPXbt2xYEDBzB8+HCULFnS394+Mdq0aYOXXnoJLVu2xK233oqDBw9ixIgRKFmypPNCPCU8++yzmDdvHmrVqoXu3bujfPny+PXXX7F69WrMnj0bv/7664XeomFcNNOmTcN3332Hs2fP4sCBA5g7dy5mzZqFokWL4ssvv0SmTJn8c5M7Xw+yb8mdq12MD6hcuTK6dOmCt956y5drWb58OcaMGYP27dujcePGl7web7vtNnzyySe45557MG/ePNStWxfnzp3Dd999h08++QQzZsxA9erVkz1HyZMnD/773/9i6NChaNu2LVq3bo01a9Zg2rRpyJ07t/PdyfVvFSpUwLXXXosBAwb4K1w//vhj/4cGJtKzr2FcMv60ff1SgWnTpnndunXzypYt62XLls2LiYnxSpYs6fXp08c7cOBA2Pnvvfeed80113gZM2b0rrzySq9hw4berFmz/PxvvvnGu/baa73MmTN7BQsW9Lcth2yLeezYMe/WW2/1rrjiirDtl7/44guvfPnyXvr06cO2AF+zZo13ww03eLly5fIyZszoFS1a1Lvpppu8OXPm+OeEtjM/dOhQWPkT2+ocgNerV6+wc3X7a8/zvDlz5njXXHONFxMT45UoUcJ75513vP/85z9epkyZIlWxT8OGDb0KFSp4K1eu9GrXru1lypTJK1q0qPfaa6+FnXvgwAGva9euXu7cub2YmBivUqVKiW6FvnjxYq9atWpeTExM2Hbv27dv926//XYvf/78XoYMGbxChQp5bdu29T799FP/nEjb1ya2len+/fu9Nm3aeNmzZ/cA+NteJ3bupk2bvGbNmnnZsmXzcufO7XXv3t3f1pnvI7H2SIzkXu/s2bNenz59vDx58nhRUVHJuva8efO8+Ph4L0eOHF6mTJm8EiVKeHfccYe3cuVKz/M87/777/fSpUvnLVu2zPncypUrvfTp03s9e/b0/5ZYn3n77be94sWLe+nSpUtyu/IuXbp4WbNm9bZv3+61aNHCy5Ili5cvXz7viSee8LefDaHt/dtvv/l9Jlu2bF58fLz33XffhZUpJW2enPoxUoeU2OqTJ096ffv29XLlyuVlzZrVa9eunffjjz+G9RnP87yZM2d6FStW9GJiYrwyZcp4H3zwQaLj8ssvv/SuvvpqL1OmTF6xYsW85557znvvvffCtkIuWrSo16ZNm0Tv4ffff/cGDBjglSxZ0ouJifFy587t1alTx3vxxRe906dP++f98ssv3m233ebFxsZ6OXLk8G677TZvzZo1YeM9iLx583oAnLpZtGiRB8CrX79+2PnJtTEh3n77bQ+Alz17du/kyZOJliE5/io07iZMmBD2+Q8++MArXry4FxMT41WpUsWbMWOG16VLF8df7tixwwPgvfDCC2GfT6y9N2zY4F1//fXeFVdc4WXKlMkrU6aM9/jjjzvnPPnkk16hQoW86Ohop30Ts2/bt2/3brzxRv96NWvW9L766ivnnEj3GCp7Um2aXNvmeSmzt57neRMnTvTKlSvnZcyY0Stfvrz32WefhdVxiLfeesurVq2alzlzZi979uxepUqVvAcffNDbu3evf04kP+l5ye//Z8+e9V544QWvbNmyXkxMjJcnTx6vVatW3qpVq/xzvvvuO69BgwZe5syZw7YyX716tRcfH+9ly5bNy5Ili9e4cWNv8eLFzr0kZ+t6JtSGH330kTdgwAAvb968XubMmb02bdqEbS+fWP29++67XqlSpbyMGTN6ZcuW9UaNGnXR87EDBw54vXr18goXLuxlyJDBy58/v9e0aVPvrbfeStY9GcalJjSuQv9iYmK8/Pnze82bN/defvll7+jRo4l+Ljnzdc8Ltm/JnatdjA84c+aMN3jwYC8uLs7LkCGDV7hwYW/AgAHeH3/84Xw+aB6QGKHn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fEpq+onY2NgwO58YPLYA1+5pv1ZYN0M1pYI0mvSXevY3OgbUFrCd07Jrefm6QToegKs/peNbv4frVbeuVjvHW4err+JzGzZs6OTpvUydOtU/VhvIehaAu7W55um20jt27PCPmzdv7uTlzp3bSfMWz6qFoeeyTphqoageFeerDgX7FNVx0Qfz9evX+8ebNm1y8lQ3irUydCvroO3pVZ9P24l9ivYFLh8ALFiwwD/Wbbm1/KyNo76Jx5OOF9YsBIC1a9dGPFf1OHnljc4vVXeL6zekF3Ipt/v+Oz9sMKnpIxjub61atXLyVJ+GtYFCIYQhWJAdcOeWanMrV67sH6vdV1vJ2jW8cgxwdZcA1xfp3Ee/h3WNVJ907ty5TprtjfqTli1bOml+ttC6Vm1T9hE8HwHcebJep1+/fk56xIgR/rHqu6qdYq0inc/pPP7LL7/0jwcOHIggWI9Kx2yjRo0ifi4poX72Y+or+flLnyu0DKyHps8H+kzK9lD9JvsERZ/N1J+wXbzpppucvJkzZzppLj/ragHhmoqsVaVzFn5hrfMbHZdcPu0LOibY36l2FuuWAe7cLfQd6iMZ05RySdFKqQIFCoQJ6pUrV84fICGjro78wIEDYQY/RMaMGREbG+v8MwzDSMuk1q8b48ePR//+/fHEE09g9erVqFy5MuLj48MelkMsXrwYt9xyC+68806sWbMG7du3R/v27R1x5P79+2P69On44IMPsHnzZvTr1w+9e/d2JmUXg/kJwzAMWykVCfMRhmEYtlJKSdFLqbp164a9tdy6dav/djUuLg758+d3dqI4evQoli1bFqZubxiG8VcltRzJSy+9hO7du6Nr164oX748Ro4ciSxZsuC9995L9PyXX34ZLVu2xAMPPIBy5crhySefRNWqVfHaa6/55yxevBhdunRBo0aNUKxYMfTo0QOVK1fG8uXLL7g+GPMThmEY9lIqEuYjDMMw7KWUkqKXUvfffz+WLl2KZ555Bt9//z3GjRuHt956C7169QJwftlav3798NRTT+HLL7/E+vXrcfvtt6NgwYJo3779n1F+wzCMVCc1HMnp06exatUqR+w1OjoazZo1iyj2umTJkrCtmePj453z69Spgy+//BJ79uyB53mYN28etm7dGrbN8IVifsIwDMNeSkXCfIRhGIa9lFJSpClVo0YNfP755xgwYACG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tZVJ+oVqK1kTR+vD2lTAVr+eIsnXAPFaSdfxqpPI5ao/1bZt2yjPdkDvrV+/flGebf/f//73qKxTp04hrXbq+OOPz3gdtQOsIaX1ZW07ADj33HOjPOv9anvqGoHtobbnJ598EuVZd0ttpWpX8bqkRYsWURlrds2dOzcqUz/Vp0+fkGbtMSB9zLGt1PtW7Sdea6gO5qWXXhrl2eeqzpY+k/KaWO2p6lHxvepaevny5SGtazVto5dffjmkde1Tq1atjPVTbeUXXnghyqf+IAz8127o3GBK4lliW3jjjTdw0EEH4YADDkCXLl1w22234cADD4w+c/vtt+PWW29FzZo1cc455+Cqq64Kz06zZ89Gp06dIluTk5OD4cOH47vvvkvr80w4fM8YY4rJjmy5rVGjBipWrBj+DRs2rNDf+Oabb7Bly5a0h9kqVapkfNm5evXqIj8/fPhwlC1bFldcccWONIExxpgEslF3cPPmzbjllltQp04dVKhQAc2aNYteXgJbX0reeOONqF27Nvbee2/UqVMHt956q1+aGWPMTqQkniWKonv37njssceQm5uL4cOHY9q0aejRo0f0x6krrrgC48ePx+uvv47f//73+Mtf/oKrr746lGd69kiVbStZu1PKGGN2Rz777LPor/fb+5eN7SEvLw+jRo3CwoUL03YWGmOM+XWR0h0cM2YM2rVrh5EjRyInJwfLli1LOz0LAG644QY88cQTePDBB9GgQQO88sor6N27N2bNmhV2ZwwfPhz33XcfHn30URxxxBFYsGABLrzwQlSsWNF/zDDGmCxgZz1L8KmPTZo0QdOmTVGnTh288cYb4VRSjsBo2rQpypUrh9///vcYNmzYTn2G8U4pY4wpJjvy1439998/+pfJoFeuXBllypRJO3p3zZo1GeO6q1atmvj5GTNm4KuvvkLNmjVRtmxZlC1bFp9++in+8Ic/pG1ZNsYYs/2UxE4p1h1s1KgRxowZg3322QcPPfRQoZ9//PHHcf3116Nnz5447LDDcOmll6Jnz5648847w2dmzZqFU045BSeccAJq1aqF0047Dd26dSvy5FdjjDHbTkk8SxSXww47DJUrV04LN2XatWuHn3/+OYSrZnr2SJVtK1m7Uyp15CCA6HQoje3VmGKNsWRUL4BjTlVDgTVmNAZXO561D1QrRPNffPFFSKvWgcbSsn6B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BAwePBhjxoxBu3btMHLkSOTk5GDZsmVp+iwAMGvWLJx99tkYNmwYTjzxRIwbNw69evXCwoUL0bhxY/zwww9YuHAhbrzxRjRr1gzfffcdrrzySpx88slYsGBBseu3q5k/f37oS9ZK0HGu9pFtoo4bteGsPaFjgsd99erVozLVDOT+1+vouGctDNXAad68eZRnPaKDDz44KnvvvfeiPN+rzkPV+eA2U7umek+s5aC+ijWH1N689tprUb5fv34hXadOnahMbf/cuXNDWv2E6lCw7p7aKm171r1i3RYg1rwCYn0W1axQjRXWz1LdR14Arlq1KirT+27VqlVIqwaI3hv7QPWzqkXIfq0ofSy+lq5jtD2PPPLIjJ/VecC6hYceemjG+qqWlupP8XXV1mter8XouobXaClNqSTdNmtK7Xo++uij0Oesa6S6QTpfTz/99JDW9aKuLXk+zJw5Mypju6DzSu0zjze1EfqbkydPDmkNtdHrsk3p0aNHVMY6VkCsG6RzRf0o6xuylg4AfPDBB1H+mGOOCWnVx2I7pjaN+wyINadUz07X2Owbte5qp7jf9JlJNRV5zutnWaMJiLUaVYtMdcy43/R5i+2Uton6Y7aHeXl5GX8DiHUx1ebqHyv5vtV2qx3k8aA6Ue+++26UP/7440Na+79FixZRfs6cOSGtz8G8vmncuHFUpmtCXu+89dZbUZn6BNZ3U1+juls811JryZ2pO5j6DpDun8qXL582Z7eVN954AwcddBAOOOAAdOnSBbfddlto39mzZ+O3v/1tNJa7du2K0qVLY+7cuejduzdmz56NTp06RfMsJycHw4cPx3fffZfoZ5li7ZQaNmwY2rRpg/322w8HHXQQevXqhWXLlkWf+emnnzBgwAAceOCB2HfffdGnT5+0FxTGGPNrpqTC90aMGIGLLroIF154IRo1aoQxY8Zgn332wUMPPVTo50eNGoXu3bvjT3/6Exo2bIhbb70VLVu2xL333gtg6wJqypQpOOOMM1C/fn0ceeSRuPfee5GXl5f2wLi92E8YY4zD9zJhH2GMMTv2LFGjRg1UrFgx/Bs2bNh21aF79+547LHHkJubi+HDh2PatGno0aNHePG4evXqtD+Cly1bFpUqVQovEVevXp12eEAqry8akyjWS6lp06ZhwIABmDNnDqZMmYLNmzejW7du0UlGV111FZ5/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",
+                        "image/png": "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XlRUlJcrVy5nDN19991e/vz5/XRKbMzzzz/vAfB27NgR9t0PPfSQlylTJu/XX3/1/5acv0rKZoXsasOGDf1jRtss5Auef/5574033vCKFy/uxcTEeNWrV/eWLVsW9vlNmzZ5HTt29PLkyeNlzpzZK126tPfwww97nvf/7a7/QjaE7VuIbdu2eTfccIN3+eWXe1myZPFq1arlffnll845IR8xfvx478knn/SuuOIKLzY21mvSpIm3devWsDIqKbFt52NvPc/z/X5sbKxXoUIF79NPP01yXJw9e9YbNmyYV758eS82NtbLly+f16NHD6e9g/yk56W8/589e9YbPny4V7FiRS82NtbLkyePl5CQ4C1fvtzzPC/J++R2WbVqldeyZUsvR44cXrZs2bwmTZp4S5Yscb4jVF/z58/3evbs6eXNm9e77LLLItZTqA0/+ugjb8CAAV7+/Pm9rFmzeu3atfN27drlnJtU/T3//PNe7dq1vVy5cnmZM2f2qlat6k2YMCHse1IzH/vpp5+8rl27evny5fPPe+eddyLeg2H82YTGVWisKk8//bQHwHvzzTedvyc3X0+JfUvpXO1CfMDp06e9IUOG+H6maNGi3oABA7w//vjD+Y6geUBS8PNR/fr1vSxZsnj33nuv53nn5jMDBw70SpQo4fvm+++/P+w7UzpHSUxM9J544gnviiuu8LJkyeI1atTIW79+/Xn7t1Db6Fxbn40iPfsaxsXkL73spmjRoliyZAnWr1+PihUrBp47ePBgDBo0CHXq1MGQIUMQExODb775BnPnzkWLFi0AnIunzp49O/r374/s2bNj7ty5GDhwII4cOYLnn38eAPDII4/g8OHD+OmnnzBs2DAAQPbs2VGuXDkMGTIEAwcORI8ePVC/fn0AQJ06dQAAc+fORatWrVCtWjU8/vjjiI6OxqhRo9CkSRMsXLgQNWvWdMrbsWNHlCpVCk8//TQ8zwu8t0WLFuHTTz/FPffcgxw5cuDll19Ghw4dsGvXLuTOnRsAsHr1arRs2RIFCxbE4MGDcfbsWQwZMgR58+ZNcX3/9ttvaN26NW688UbcfPPN+Pjjj9GzZ0/ExMSgW7duAIATJ06gUaNG+P7779G7d2/Ex8djwoQJuP3223Ho0CHce++9yJs3L15//XX07NkT1113Ha6//noAwFVXXQUA2LBhA+rWrYsrrrgCDz30ELJly4aPP/4Y7du3x8SJE3Hdddc55erTpw8uv/xyPP7449ixYweGDx+O3r17Y/z48QCA4cOHo0+fPsiePTseeeQRAED+/Pkj3ueECRNw/Phx9OzZE7lz58ayZcvwyiuv4KeffsKECRNSXF+pud5dd92FPXv2YNasWRg7dmyKrjt27Fh06dIFCQkJePbZZ3H8+HG8/vrrqFevHlavXo1ixYqhSZMmuOeeezB06FC0b98eVatWxd69e9GnTx80a9YMd999d5LXbtCgAfr27YuXX34ZDz/8MMqVKwcA/v+ROHv2LFq2bIlrrrkGzz33HKZPn47HH38cZ86cwZAhQyJ+bvny5Vi8eDE6deqEK6+8Ejt27MDrr7+ORo0aYePGjWG/OCXX5imtHyNtSI2tvvPOO/H+++/jlltuQZ06dTB37ly0adPmgr7/9ddfR4UKFXDttdciY8aMmDx5Mu655x4kJiaiV69ezrmbN2/GzTffjLvuugvdu3dHmTJlcPz4cTRs2BC7d+/GXXfdhSJFimDx4sUYMGAA9u7d6y9p9zwP//rXv7Bo0SLcfffdKFeuHD777DN06dIl2TJedtllqFixIhYsWIC+ffsCOGfbo6Ki8Ouvv2Ljxo2oUKECAGDhwoW+jwFSZmNuvPFGPPDAA/j4449x//33O9/98ccfo0WLFn7oXUr81V133YUrrrgCTz/9NPr27YsaNWoE2tUgxo0bh99//x133XUXoqKi8Nxzz+H666/HDz/8gEyZMgEA1q5di/r16yNTpkzo0aMHihUrhm3btmHy5Ml46qmncP3112PLli348MMPMWzYMOTJkwcAIvq4/fv3o06dOjh+/Dj69u2L3LlzY8yYMbj22mvxySefhPmZZ555BtHR0fjvf/+Lw4cP47nnnkPnzp3xzTffBN5bSmzb+djbmTNnokOHDihfvjyGDh2KX375BV27dsWVV14Zdu5dd92F0aNHo2vXrujbty+2b9+OV199FatXr8bXX3+NTJkyBfrJlPZ/ALjjjjswevRotGrVCnfeeSfOnDmDhQsXYunSpahevTrGjh2LO++8EzVr1kSPHj0AACVKlABwzvfXr18fcXFxeOCBB5ApUya88cYbaNSoEb766ivUqlXLua977rkHefPmxcCBA3Hs2LHAdgDOrdiMiorCgw8+iAMHDmD48OFo1qwZ1qxZE7gK4qWXXsK1116Lzp0749SpU/joo4/QsWNHfPnll2G2KSXzsf379+Oaa65BVFQUevfujbx582LatGm44447cOTIEfTr1y/ZezGMtObWW2/Fww8/jJkzZ6J79+4AUjZfT86+pXSudqE+4M4778SYMWNwww034D//+Q+++eYbDB06FJs2bcJnn33m3GtS84AgfvnlF7Rq1QqdOnXCv//9b+TPnx+JiYm49tprsWjRIvTo0QPlypXDunXrMGzYMGzZssUJYU7pHGXgwIF48skn0bp1a7Ru3RqrVq1CixYtcOrUKac8qfVvyRHp2dcwLiqX+q3YhTBz5kwvQ4YMXoYMGbzatWt7DzzwgDdjxgzv1KlTznlbt271oqOjveuuuy7sVz3+9VlXwnie5911111e1qxZnbfabdq0SfIN8fLly5P8NTwxMdErVaqUl5CQEPZ98fHxXvPmzf2/hd7033zzzWHXj7RSKiYmxvv+++/9v3377bceAO+VV17x/9auXTsva9as3u7du/2/bd261cuYMWOKV0oB8P73v//5fzt58qRXpUoVL1++fH6dDx8+3APgvf/++/55p06d8mrXru1lz57dO3LkiOd551YAQFY+hGjatKlXqVIlp84TExO9OnXqeKVKlfL/FnrD36xZM6de77vvPi9DhgzeoUOH/L9VqFAhyV/uk1oplVQ/GDp0qBcVFeXt3LnT/1tKV0ql9Hq9evVK0fU8z/N+//1377LLLvO6d+/u/H3fvn1ezpw5nb8fO3bMK1mypFehQgXvjz/+8Nq0aePFxcU53+154SsJJkyYkKJf60OEVk706dPH/1tiYqLXpk0bLyYmxjt48KD/d237pOpoyZIlHgDvvffe8/+W0jZPTf0Yfz4ptdVr1qzxAHj33HOP8/dbbrnlglZKJdW/EhISvOLFizt/C60WmT59uvP3J554wsuWLZu3ZcsW5+8PPfSQlyFDBn+1xaRJkzwA3nPPPeefc+bMGa9+/frJrpTyvHM2gFdA9e/f32vQoIGXL18+f1XqL7/84kVFRTkrqlJqY2rXru1Vq1bNOW/ZsmXOOEuNvwrZT101ktqVUrlz53ZW7Xz++eceAG/y5Mn+3xo0aODlyJEjzG5xGUOrwfRXX88Lt2/9+vXzAHgLFy70//b777978fHxXrFixfy5Qugey5Ur5508edI/96WX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IezYsQPly5fHp59+mqqJXOiF0+bNm/H000/7f2/QoAGmTZuG2NhY1KhRw/97am1Wvnz50LhxY7z44ov4/fffcdNNNzn50dHRF+yvunXrhhdffBEJCQm44447cODAAYwcORIVKlQI02tMKS+//DLq1auHqlWrokePHoiPj8eOHTswZcoU34eFbOgjjzyCTp06IVOmTGjXrl2SNu6hhx7Chx9+iFatWqFv377IlSsXxowZg+3bt2PixIlhuojnS0ptW2rt7dChQ9GmTRvUq1cP3bp1w6+//opXXnkFFSpUcF4mNmzYEHfddReGDh2KNWvWoEWLFsiUKRO2bt2KCRMm4KWXXsINN9zg119SfjKl/b9x48a49dZb8fLLL2Pr1q1o2bIlEhMTsXDhQjRu3NjfBKNatWqYPXs2XnzxRT9ktVatWnjyyScxa9Ys1KtXD/fccw8yZsyIN954AydPnsRzzz13wW2RK1cu1KtXD127dsX+/fsxfPhwlCxZ0t/ePinatGmDF198ES1btsQtt9yCAwcOYMSIEShZsqTzQjw1PPPMM5g3bx5q1aqF7t27o3z58vj111+xatUqzJ49G7/++uv53qJhXDDTpk3Dd999hzNnzmD//v2YO3cuZs2ahaJFi+KLL75A5syZ/XNTOl8Psm8pnatdiA+oXLkyunTpgjfffNOXa1m2bBnGjBmD9u3bo3Hjxhe9Hm+99VZ8/PHHuPvuuzFv3jzUrVsXZ8+exXfffYePP/4YM2bMQPXq1VM8R8mbNy/++9//YujQoWjbti1at26N1atXY9q0aciTJ4/z3Sn1bxUqVMA111yDAQMG+CtcP/roI/+HBibSs69hXDT+tH390oBp06Z53bp188qWLetlz57di4mJ8UqWLOn16dPH279/f9j57777rnf11Vd7sbGx3uWXX+41bNjQmzVrlp//9ddfe9dcc42XJUsWr1ChQv625ZBtMY8ePerdcsst3mWXXRa2/fLnn3/ulS9f3suYMWPYFuCrV6/2rr/+ei937txebGysV7RoUe/GG2/05syZ458T2s784MGDYeVPaqtzAF6vXr3CztXtrz3P8+bMmeNdffXVXkxMjFeiRAnv7bff9v7zn/94mTNnjlTFPg0bNvQqVKjgrVixwqtdu7aXOXNmr2jRot6rr74adu7+/fu9rl27enny5PFiYmK8SpUqJbkV+uLFi71q1ap5MTExYdu9b9u2zbvtttu8AgUKeJkyZfKuuOIKr23btt4nn3zinxNp+9qktjLdt2+f16ZNGy9HjhweAH/b66TO3bhxo9esWTMve/bsXp48ebzu3bv72zrzfSTVHkmR0uudOXPG69Onj5c3b14vKioqRdeeN2+el5CQ4OXMmdPLnDmzV6JECe/222/3VqxY4Xme5913331ehgwZvG+++cb53IoVK7yMGTN6PXv29P+WVJ956623vOLFi3sZMmRIdrvyLl26eNmyZfO2bdvmtWjRwsuaNauXP39+7/HHH/e3nw2h7f3bb7/5fSZ79uxeQkKC991334WVKTVtnpL6MdKG1NjqEydOeH379vVy587tZcuWzWvXrp33448/hvUZz/O8mTNnehUrVvRiYmK8MmXKeO+//36S4/KLL77wrrrqKi9z5sxesWLFvGeffdZ79913w7ZCLlq0qNemTZsk7+H333/3BgwY4JUsWdKLiYnx8uTJ49WpU8d74YUXvFOnTvnn/fLLL96tt97qxcXFeTlz5vRuvfVWb/Xq1WHjPYh8+fJ5AJy6WbRokQfAq1+/ftj5KbUxId566y0PgJcjRw7vxIkTSZYhJf4qNO4mTJgQ9vn333/fK168uBcTE+NVqVLFmzFjhtelSxfHX27fvt0D4D3//PNhn0+qvdevX+9dd9113mWXXeZlzpzZK1OmjPfYY4855zzxxBPeFVdc4UVHRzvtm5R927Ztm3fDDTf416tZs6b35ZdfOudEusdQ2ZNr05TaNs9Lnb31PM+bOHGiV65cOS82NtYrX7689+mnn4bVcYg333zTq1atmpclSxYvR44cXqVKlbwHHnjA27Nnj39OJD/peSnv/2fOnPGef/55r2zZsl5MTIyXN29er1WrVt7KlSv9c7777juvQYMGXpYsWcK2Ml+1apWXkJDgZc+e3cuaNavXuHFjb/Hixc69pGTreibUhh9++KE3YMAAL1++fF6WLFm8Nm3ahG0vn1T9vfPOO16pUqW82NhYr2zZst6oUaMueD62f/9+r1evXl7hwoW9TJkyeQUKFPCaNm3qvfnmmym6J8O42ITGVehfTEyMV6BAAa958+beSy+95B05ciTJz6Vkvu55wfYtpXO1C/EBp0+f9gYPHuzFx8d7mTJl8goXLuwNGDDA++OPP5zPB80DkiL0fJQUp06d8p599lmvQoUK/rNntWrVvMGDB3uHDx/2z0vpHOXs2bPe4MGDvYIFC3pZsmTxGjVq5K1fv/68/VvovGbNmnmxsbFe/vz5vYcfftibNWtWqp59DeNiEOV56UhJ1Ehz2rdvjw0bNiSpTcE0atQIP//8c7Lx3MY/l9tvvx2ffPJJkiE/hnGhhLaaHzRo0KUuimEYfyHmz5+Pxo0bY8KECf6qMMMwDMMw0g9/aU0pI3WcOHHCSW/duhVTp05Fo0aNLk2BDMMwDMMwDMMwDMP4x/KX1pQyUkfx4sVx++23o3jx4ti5cydef/11xMTERNzm2TAMwzAMwzAMwzAM48/CXkr9g2jZsiU+/PBD7Nu3D7GxsahduzaefvpplCpV6lIXzTAMwzAMwzAMwzCMfximKWUYhmEYhmEYhmEYhmGkOaYpZRiGYRiGYRiGYRiGYaQ59lLKMAzDMAzDMAzDMAzDSHPSnaZUYmIi9uzZgxw5ciAqKupSF8cwjH8onufh999/R6FChRAd/f/v7//44w+cOnXqvK4ZExODzJkzX6wi/mMxP2EYRnrgYvsJ8xEXB/MRhmGkB+xZIuWku5dSe/bsQeHChS91MQzDMAAAP/74I6688koA55xIfHw89u3bd17XKlCgALZv3/63dCZpifkJwzDSExfLT5iPuDiYjzAMIz1hzxLJk+5eSuXIkQMAnDeK/GYxW7ZszvnHjh1z0hkyZIh47ZMnT0Y8Vxv2zJkzEa/5yy+/OOkTJ074x5dddpmTFxMTE/HcLFmyOHl6L3zf2bNnd/J+++03Jx0XF+cfq3b92bNnnTTnZ8zodgEtL5+r9Xf48GFEIleuXBGvo79a8X0Cbh1pebhd9FqxsbFO3h9//OGkufzapqF+FyJTpkz+sbY31zXg1oOWL2/evBHztE35Ovz9SX32yJEjEc/V+uR60T6mbcFlSkxMdPK0v54+fTriudpX+NcA/c7LL7/cP/79998RBPcH7Rval48fP+4f//zzz06e1j3XYai+EhMTsWPHDqdvnDp1Cvv27cOuXbvC+kFyHDlyBEWKFMGpU6f+do4krQm1yQMPPOC3V4kSJfx8tiFAuN9Q+8loX2ayZs3qpNm25suXz8n79ddfnTSPPR47QLjNzpkzZ5LHQPjY4ns7evRoxLIDwObNm/3jcuXKOXlaJk6rLdV62L59u3+su7nyeNd613HI5yZn14J8tPoCtuFan9re3G46xvPnz++kt2zZ4h+rPyxYsGDE8qvt4r6h96n9iO2Rlk9/dWU/fOjQISfvp59+ctJsP3ksAcCBAwecNPs1nVRrX+YyqX3XOuJ203Pz5MnjH2s/V79WoEAB/3jHjh2B38mfVT+r1+WXHKFzT5w4gXvvvfei+AnzERePUHv06dPH71fcp3Q8qA2pXLmyf6z2ZOHChU6ax4v22/j4eP9469atTh7bTQC4+uqr/WMdV1WrVnXShQoV8o/VJ2i/ZTvVrl07J2/evHlOulixYv6x2hOdu/F40TpSu8W2XuuIv1Pn4t99952TZlteqVIlJ0/9FJ+rY1vnBDwPVZuxf/9+Jx16sQCE26J169Y56datW/vHa9eudfLYpgFAyZIl/WOto3HjxvnHt912m5On9rlevXr+sfaxxYsXO+ncuXP7x+oLg54P9+zZ4+RxnQCu/+YxAIT7Hh4/c+fOdfK0b/O9aR2tXLnSP1Y/37ZtWyf99ddf+8dcBwDw7bffOukmTZr4x1999ZWTpy++77nnHv/4wQcfBHBuHL377rv2LJEC0t1LqZDRi46OTvKllDoOncBpOqXn6nV5cGqeGmZOJ1ceTl/IuUEvdnRSGJTW6wbVQ3JliFQe/c7kXkqlpo7+rLrnekjNdfXe+Dpq8IP6clrdd3JtEVRefdmZ0jIE1VHQ92u+lieoPi+kzyXVz+Pi4lLtSIyLR6hNYmNjfaesL0oYzdPJKxP0UkpfzPIY0Emuvhjj6+pkL+gFsJZd+znnB5UdcH980evqS6mgF8laD0HX5c9qvet1+Fx9cXMhL6X4BbWWT+uM203P1Tbm8uvkWe+Ny6/lC/KzOulMTd/g8uoDpl6X+6ReV++F8zVP5xt8P9rH9LNcL/oQyd+pvkfbkM/V+wxqf/1O/R7+rN6L+Yn0BfuIUL/iMaD2RccO9xvtQ/rCnPutjjPu4/qdQdfRc4PGYNC8Xa+rPwQEjY/knn14vOh11P9x+XXs8HcG2Vj9Hh3LajvZ7idne4JshtprzleboW3K3xN0HS2DXjfIPut1uI31XO1X/Fm1d3ovQT8KB42R5PwJt7nWkRJUR1wmvU5Qv9fy6L3xdybXhmzv9VzzEcmT7l5KJYX+osFop+S0vinVyRL/mqCDTw0qE2QA9NfyoBUu2mH1FwI+Vx2dGm5eCaKrlHSA8YOBPiSoUQqaUPLbZf1lRh+6+BdyvY7WPd9b0IowwHWaWtf6K4T+csOw8wLc+k7ugVbbggl6eaRv+bkO9T713rhva90HOZLkfvkKmqDraiO+n6AHJ8Dt2zoOuT71c1oG/lVK20zbhX99036tY0/vDQh+wPc8L+w+kiO15xvJU7BgQb/P8K+Z3PYA8MMPPzhp7g9qL3Vcsp378ccfnbyghwgdhzxOr7jiCidPV2Pu3LnTP2Y/kBRcPu1jaoevuuoq/1jtkZaX61NXCB08eNBJV6lSJcnyAO4v/urj1G5wHekv0Fo+/mxyK0A5X3/hVVvL/lx/Idf65PbX+1Ybw78Oly5d2snjOlK7o/6F+5m2A7cvAGzcuNE/1rlJmTJlnDTb0/Xr1zt5+lmekxUtWtTJ41+rAffXf71vfZHH/Vd9FY89rVv10dx3dFwGrTwL6mOar/OYpEitnzAfcfG56qqr/P7BK0W5XwLhKz14VZPOD2644QYnzStVdMUkz2F0zNWtWzdiuRs2bOikN23a5KS5j2/YsMHJ01VVbEN0JYr2cZ5H6bhXW/nxxx/7x2obGzdu7KQ5imTNmjVOHs9np06d6uTdfffdTnr16tX+8fTp0508nef179/fP3722WedPF05w88aalebNm3qpFesWOEfs+8Dwm0Ir7rZvXu3k6e2nW0cr0YFgOeff94/Vh+mK/eKFy/uH+v8QVdyXX/99f6x+k0dE8uWLfOPeSUhEO6v+dmM6wsIf0HEcy6e+wDuyigAGDNmjH+sK7B49aCOLbX7tWrV8o95JSEQHvG0bds2/1j7tc4XeWVfaB4a9COoPUu4/CVeShmGYaQnzJEYhmEYQdhLKcMwDCMS9izhYi+lDMMwUok5EsMwDCMIeyllGIZhRMKeJVzS7Usp1pTipdrJhTLwMm5dRhsUZ62w6F2QaDPgLv/WZZ/6nbwcVu8lKMxOl3lqp+RlwRp6qKEhvFRWl2vqMkO+V71vXr6uS3c17IrrSEPygmKe9b512Sej963LKrkMydU9X0u/U++Nl6nqsk9ejqshRRp+FiS+rO3CfTdI2wkIDkXUJbd8rSDtJwBhon2MjgOuQ13ezOMrSGsFcEMydXzrMvSgcA8dP0mFolr4XvonPj7etxG8xFqFP1XcmPuOjtkgfScNP+Nl9Nqv9TvZ9mvoj4bSsT1SuxEkIKu2icNVtIzJ6TMWKVLEP1Yboz6RbZcK9LKIqYrWqj1iO6L3ovWwa9cu/1jbLEi7SssepH+odaRhguxLVWZA66F8+fL+sYbHcRmChOwBt+9ouLOWgetQ+7mWgW0gz3+AcP/OfVnDLTQclttUz9XxxO0YZH81NF/rjH2X1p/KOrAouvqx5cuXO+mk5jz63Yy9lLr07N271x8nt956q//3iRMnOufpfILbQsOtJ02a5KRvuukm/7hixYpOHtsBDj0DwsPheExqH9dwLh7bQXqAgDvX5BCnpM5lG62+RoXFOUxM7bOGifE40bkah+G1atXKyXvmmWecNIdzqY3QkEwOBWzWrJmTt3Tp0ojXVduoYvDs01atWuXkaWhijx49/GMNu1ObHCSXwu39/fffO3l6b9x3de7L5QHcPqmblMyaNctJ16lTxz9WnzB//nwnzb5dx4/eG4eBakiePkvUr1/fP9Z+xJu3TJ48OfA7uS9rfd55551OmsP7NPy1bNmyTppDKUPzLx1jjD1LuKTbl1KGYRjpFXMkhmEYRhD2UsowDMOIhD1LuNhLKcMwjFRijsQwDMMIwl5KGYZhGJGwZwkXeyllGIaRSsyRGIZhGEHYSynDMAwjEvYs4ZJuX0qdOXPGj69lzQzVwFHdG44xVa0I3d6Z9QxUU4j1iFT3QmNp+bp6neS26GaCdJiC8rS8qisRpNuh2huqn8TaS0Fbx+rnVN+JY7+1DlSLJUhLS3WYuL61L2j7c1r7kZaJY721DbU+WW9FdQm4fLwlOBCuvcE6HlonWr9cR9rnNE5dtbUYrTNuN71v1RnhMgRpegCuNovWEZ+r8e/aj1jTRetP+z3r3OjWxvo9XL7QfQUZfnMk6YN169b5eiGFCxf2/666MRrTz1szB+nJAa6t1S2SWa9P9YYUPld1/lijQtFtpNX+sG1lnSUgXCNi7969/rHet9YRX0ttipb3hx9+8I+vuuoqJ0+3U2dUY6NGjRr+sWpAaP3ymFbbqnXEtkJ1UvR7WHNF7YT6H+4bqu+k5eX6VL0YtoGqM6PtxNu/q46LznHYr6luhtpLLh/rXwHh44ltK2tRAeFzCrateq6Wgcurvp/rQbW+tHysCVOzZs2I3wG4/oj7MRA+3pPSlArSdLSXUpeew4cP+/OTadOm+X9XnaCqVas6aZ5zb9++3ckbOHCgk3733Xf9Y+3/pUuX9o9Z+zWp67L2jmoT6VhRO8ao3WL7p/NitWmq6cOwbiMAJCQk+Meqw1S3bl0nzeNs7dq1Th7bXPUJtWvXdtLs79QvqV/lMmzcuNHJU9/I+nE67rUMrDGkZdA25nmz+kJNsx9TW7lkyRL/uGjRok6ezvHZP2s/0e+sVq2af/zmm286eay3B7j1q3N89ftXX321f6wan6oFxrZetXV5Xge4flXHGreFPiNXqVLFSfO8qkWLFk7eihUrnDT7VdatAsJ9Ofej//znPwDOtQ/bCMaeJVyikz/FMAzDMAzDMAzDMAzDMC4u6XallGEYRnrFft0wDMMwgrCVUoZhGEYk7FnCxV5KGYZhpBJzJIZhGEYQ9lLKMAzDiIQ9S7ik25dS0dHRfuwza10kp4PBceAaV60aBRxbrZpNnMe6SkC43g9rLalegca8cry0alBoPDTrCOl1NSaX48I1xlnP5XtVPQ29V45r1jri+tQ8/U5uN9VH0nho1otQXY4gTS5F65PLoBoUqgvB9aJ5qq3F+Rqvz+2vOida19xuqnmlcPm1TvS+uW207+r38L3p+NF24zhr1ZvScclx11p/HEOuda3l5fvWvqvl5fGl19E6Y02s0OcSExPD9K9CmCNJHxw/fty3NWwrtC+odgePNR2HqlfDfUDHC2t1qH9RfZ/8+fMn+f0AULBgQSfN36N9MOh7dPyoPgN/r96nak2wZpPqUmj9VqxY0T/esWOHk8fjUD+ndpjHod4363gArm6G2hQda6wTphoQatd27tzpH/N9AeFtyvZdNV+0PlmfI2/evE4et3dy9py1PDRPbSL3OfVNem7x4sX9Y/XJ+llG63P16tVOWv1e0HW5r+i9sZaHjgHVAGH9rCJFijh52u+5DMnpgnG/CvUbnevo+fZS6tLSokULv61YU4/7OwDUr1/fSX/11Vf+sdqIDz/80Ek3adLEP1ZNQtauUf0mtav//ve//WP1S6zRo+iY++677yJ+VvU/tQysWVenTh0nT23aokWL/OMKFSo4eUHPFiVLlkQkVq5c6aRVW4vrSLVCVX+I21vHtmo1sk3R+1y6dKmTZs09tWH8nQDw2Wef+ceq+Vi2bFknzfWybt06J4/1vFinDAifb48dO9Y/1jri9gXce+3YsaOTp32FbafeN+uCAa6/Xrx4sZPHOlaAO//ROtIxs2nTJv+4ZcuWTh5rAmr7qtYX+2D9Tq17rpetW7ciCL63kG6d2gTGniVc0u1LKcMwjPSKORLDMAwjCHspZRiGYUTCniVc7KWUYRhGKjFHYhiGYQRhL6UMwzCMSNizhEu6fSmVLVs2f6kgL/vUxtAloryUWpfc6hL/oO28eZmifqcuW+Rln7pNpsJhRLrsW5c/8n3rdXVZJS+31+WOuqSVlyrqMvigcDndqpXDEbSO9LpcPg1z0HbitIY/ajqovnW5Lrd/ctfhdtLr6PJ/vncNY+TwHl1iq2Ea3N4a8qB1xuEeujxX4RCOoHAewO3b2j81nILrU/uc1if3OS1vUPiDhvdwCKbWtY5vDinUNtTy8fLa0HdczLCM0GeMi8uxY8f8fsBLtzVMTMcs26OgEFHAHRM8lgB3TGt/1DHLvkq/88cff3TS3Ffi4uKcPO27fK7aeu3DbN81T7fBZhukWzrreOJ83tYaAIoVK+Yfq1/QMcuhJOoPtU25ftWmqH0PCjtQSQAOWdH71lA1Xuav4UBaXrb32v5cPu7HQHi/4v6ZnP/mEEgNGQwK52O/BQTbQu3n6ue4jLzlPRAeohQUys3zDx0D6sd4y3QNp9H5Rs2aNf1jDfPlMEC9VsOGDQGE2xbGXkpdembNmuXbmapVq/p/163dNeSNw8SmTJni5HHoMABs3rzZP9bQL+6r+p2a5u+pVKmSk7dw4UInzTaOw8mA8JBVDp9iSY6k4DGpdkrLxONl1apVTp76E54D1qhRw8njkKx69eo5eepr2N5oiLeORbbtGgbYs2dPJ831q/NknY+zbY+Pj3fyVMpi3759SX4OCA8p4+8NCi9VP/T222876Xbt2iV5Tb0O4PrZGTNmOHn8jAe49at1Mn/+fCddt25d/1jHi9pvbhsNGdVwOR7D+vzP41B9oYbes39p0aKFk6fjh+vok08+cfLYfwBu24T6nz4fMfYs4ZJuX0oZhmGkV8yRGIZhGEHYSynDMAwjEvYs4RJZvdIwDMMwDMMwDMMwDMMw/iRspZRhGEYqsV83DMMwjCBspZRhGIYRCXuWcEm3L6UyZszox69yHK5uVaxaAhyrqtt3a5q1GVQHgWNnNf5Vz+Xyaeyo6iJwZ9Lrqg5Gjhw5/GPVH1KNB46t1Vhf1Z9ijRLdDlY1KljPQvO4HrQdDh486KRZv0L1P1Qzg+9N44I1Hp7rTDUzgra+1XbhutYyqPaGXpfLoPHkQdo1qmXC9aD9SNuf+45ufapx67zFuerlaAw+13fQ1tmKjkvVwWEdDx0/3F/1O3XMch/U79R2YS2CIP0uwG2LUBmC9MrMkaQPcubM6euFcN/Q8ay2i/UvVD9Ht+/lfqD9iHXWVANJ7dyOHTsi5ul1efyorVINH7ZVqdHKU+0T7Z/8Wd2OXP0Gj1PVidKxxqgtYPuuGoZ6XbZzqjui9cBlUD0O9aW89bb6UrWfXCbVBdPtvrlNdVtu9p/a/1RbhO2e2kCtI/YpfF+Aq/UFBM95WPMFcLWhVLNJdUh47Kk/13kCl1f9GPdXbV+df/BY1PbVOcT69ev9Yx0DqinG2j2h62idM/ZS6tJz+PBhv7+wHZg6dapzXvXq1Z30pEmT/GMdk2rrFyxY4B83bdrUyWOdntAW8SFUY401plSbTzWvWMtGx8OKFSucNGv66HVKly7tpHlM6vxr2rRpTprH1vXXX+/kcZ0AwPLly/3jIBv81VdfOXnqn3m86VhWn1GqVClEQu+F57esSQeE+2duG7YfQLhOGGtKqZZWwYIFnfSyZcv8Y7WrS5cu9Y9Vx0r7LpdfbazOhbhd9BmKyw64mmKq0aV+iv1htWrVnDzV6uN5iWqR6bkTJkzwj++++24nj/ur1pE+f3Xs2NE/1rmQjqdFixb5x3qf2k78LBHSUdPrMfYs4ZJuX0oZhmGkZ/7OjsEwDMO4cMxPGIZhGJEwH/H/2EspwzCMVGK/bhiGYRhB2EopwzAMIxL2LOFiL6UMwzBSiTkSwzAMIwh7KWUYhmFEwp4lXNLtS6ljx475Mb6sFaOxvRqrGXRukDYUazIBbgy5av9oTC5rfmjcqpaBdRI0Tl11hPheVKNHtRlYx0G1f7Zv3+6kgzR8tLys8aDx25ynuiGq6cKojojqgfC1VCtC24LrTOtT64G/hzWOgPD65M+qJoXGuHMcu/ZHbhetW9Ug4fbWOtH+yX1Qz1VtJW5vvY7WZ9B9K3xdrfsgnbCgdtG+oeXje1PDrGOP81UbRPsVj6+QRlfQ/ZsjSR/kzp3b7z/cxr/99ptznvaNIkWK+Meq0aT9M3/+/P6xtiFrVujY0nGoeg2M2n62R1oe/R7WJQlpGITQccn9XvU2VOeItUZUq0Nh39q4cWMnjzUh1AerZgnbT/VNhw8fdtI8PtX/aHtzWjVAgjTuSpYs6eSpfh9rgmhda1twGVU3g8uneiZ6bzzfKFy4sJOnfmz//v0Rz1XbyvpofAyEzz+4H+n8Qr+H9TqqVq0aeF3uZ9qGfN/aF9QnB2l46HjifqbjsE6dOk6afXZIS0Q/w9hLqUvPFVdc4esQse3s1KmTc57q/LFfUPs3d+5cJ81aovPnz3fy2H+wDhQQrvczZ84c//iaa65x8nT+zTo9W7ZscfLUR7AOk2pI6djh665bt87JUy1B1pFSrSr1q//5z3/8Y7XtPK4efvhhJ081pvheVfNPNV353urXrx9YPp6fq+1Rux+kfadagtxuapeWLFnipNmWaDtxnan90/ks22TVuFKfy3pJqh2pmlKsYcj6epoHAG+//bZ/3L59eydP/SrXp+oXqv9r27atf6xzrAYNGvjH+nyl2lTvv/++f6zjReuB/dTGjRudvNatWzvpcePG+ceh52AtJ2PPEi7p9qWUYRhGesUciWEYhhGEvZQyDMMwImHPEi6Rt9MyDMMwLjkjRoxAsWLFkDlzZtSqVcvZoUXZsGEDOnTogGLFiiEqKgrDhw+/4GsahmEYhmEYhmH8WfwlVkrxW0FdVqlLETlsTJeI6tJJXg6u4Wa8jFK3/NWleMltHc9w+TXsKiikTEMDtLxcJr1PXabP5dWtWbU++Xt1uSuXX7ct161OuXwcUqDlAdzQNC27LuXk8gdtGa7fo3WkoXXcdzSMS8vEy7O1nbjO9Du1vLz8VfuuLlPm8Ar+fiA4lFKXqWof5CWvupxdP8tLubW8Wvdchxrap3XPaGgN15EuZ9d74TrSMBHtc7yMPjT2g36NSKtfN8aPH4/+/ftj5MiRqFWrFoYPH46EhARs3rw5rH2Ac2UvXrw4OnbsiPvuu++iXDM9kyFDBr/v8VJ9XW6v9pLthraL9g0ew+p/uI/p+NA091e1IRpCsXPnTkRCw494jGjYlY4RLv+OHTsCz2Vbpv1C65dDttQ/8thLbmk+2wId+xqGsHXrVv9Yw0q0vbmNOaQaCA9RYL+rNlpD0zi8JSh8GHDrUP0jhwRoaJ+GagRtG69+gutBwwK1nbi+tQzqA3meUKZMGSdP5xS8Zbb2OZVC4PLrGOBwFu2rWkfcbuqLdPzw+NZ+o3MyDpUN+SL1+YytlLr0/Pjjj34f4B9fNDxKbdHChQv94969ezt5b7zxhpPmsFQdV3Xr1vWPZ8yY4eStWLHCSXNIoZanUaNGTprD1bUP6lyIx5XOtzZv3uykeWwVL17cydPwW/YDhQoVcvJ0nsfPVGrbOe+TTz5x8jTsnUP0dGxraBXnq50vVqyYk+a+ofNFDaXkkGQtw5dffumk9VqM2j8uo/o09lsaIqih4jyP1/vUeuB203vRMDu2+zpnUdv+7LPP+scapqj9np+NNGS0du3aTpp9ntprbv+KFSs6edqXOeQxZ86cTp62Ifv9q666ysn7/PPPnTS3aaifa39nbKWUi62UMgzDSCUhR5Laf6nlxRdfRPfu3dG1a1eUL18eI0eORNasWfHuu+8meX6NGjXw/PPPo1OnTmETjPO9pmEYhpF60sJHGIZhGH9N0upZ4q9Cql5KhUJC9F+vXr0AnHvb2atXL+TOnRvZs2dHhw4dwlbFGIZh/NW5EEdy5MgR518kEcRTp05h5cqVaNasmf+36OhoNGvWLOyXp5TyZ1xTMT9hGIZhL6UiYT7CMAzDXkopqXoptXz5cuzdu9f/N2vWLABAx44dAQD33XcfJk+ejAkTJuCrr77Cnj17nN0ZDMMw/g5ciCMpXLgwcubM6f8bOnRokt/x888/4+zZs2Hhmfnz5w9bgp1S/oxrKuYnDMMw7KVUJMxHGIZh2EspJVWaUhrb+8wzz6BEiRJo2LAhDh8+jHfeeQfjxo1DkyZNAACjRo1CuXLlsHTp0rCY3OQ4fvy4H/vPcf2qeaRaNqw5o+Erul0yx6PqagW+rsaDahxw0Jb2QduOJrcVOZ+rMa/JbZfNaOwv36vGfat2RFAdcf2q9obWNceMqx6EwvHFGv+uW74yuiWpthPreOh2obqFPMdvq16WxjGXKFHCP9atg7k/6NbZql3D44tj1oFwzQDuK7oltWqbcF/Rsmu/Ya0b7Z+qV8Jtrvo52l/5V84gfSytkyBtBO2raqjZbmj9qV4D95VQe549exYbNmxAUlxIHPiPP/7o6AxECrP7q5KWfiJTpkxh+kxAuAZSUFvpdsraV1TbgeH+qPZHxyGPU7UT+p1sl9UvqD1nG6M6Clp2tq06vrUe2O5pH9V74+uqPeIxrbpGet9cL+ondLyzvo/aVtXv43bizwHh98af/eKLL5w81YKqUqWKf6zbsgfpSCxevNhJV69e3T9W364+j224arxoGbivzJ4928nT+mXtJ/1OPZftl97n6tWrnTTbcJ1DqG4Ut0WQr09Ov4v7kZ6r45T1QrgOgPB743EZ6tfq+7RcqfETf+eHDSYtfUTGjBn9eWToekD4/FC3jK9WrZp/PG/ePCdPddTYpqjtYd2lhIQEJ081AHnep3pmOg9lrSDN0/k335t+J98nAMyfP98/ZvsGhPsMnvvquNK5E79UfOqpp5y8+vXr+8c6N2PtLCD8XpnQS82kPtuyZUsnb9KkSU6abZzOH7RMbL+bNm3q5On8tkiRIv6x6nepJmCQ/itr9WkdbNu2zUmzfpJuYtO4cWMnzX1Fy646UWzL1YfpZ9nvq13VH0W5DDfddJOT9+qrrzrpWrVq+cf6nMF1rXWr/oR9e+fOnZ08vReeV02bNs3J02dfrvuQ7qXOXZgLeZZIKQsWLMDzzz+PlStXYu/evfjss8/Qvn17Pz+SLvZzzz2H+++/H8C5uWSfPn0wefJkREdHo0OHDnjppZccO7V27Vr06tULy5cvR968edGnTx888MADqSrreWtKnTp1Cu+//z66deuGqKgorFy5EqdPn3bCQsqWLYsiRYpctLAQwzCM9MCF/LoRFxfn/Iv0UipPnjzIkCFDWNjC/v37w8SaU8qfcc0gzE8YhvFPxX4BTx7zEYZh/FNJi5VSx44dQ+XKlTFixIgk83nV6t69e/Huu+8iKioKHTp08M/p3LkzNmzYgFmzZuHLL7/EggUL0KNHDz//yJEjaNGiBYoWLYqVK1fi+eefx6BBg/Dmm2+mqqznvfvepEmTcOjQIdx+++0Azin6x8TEhP3amlxYyMmTJ51fz/SNtGEYRnojLX7diImJQbVq1TBnzhz/V43ExETMmTMnbDegS3nNIMxPGIbxT8VWSiWP+QjDMP6ppMWzRKtWrdCqVauI+fqD9Oeff47GjRv7q742bdqE6dOnY/ny5f6q7ldeeQWtW7fGCy+8gEKFCuGDDz7AqVOn8O677yImJgYVKlTAmjVr8OKLLzovr5LjvFdKvfPOO2jVqlXYNqCpZejQoY6+im65bBiGkd5Iqzjw/v3746233sKYMWOwadMm9OzZE8eOHUPXrl0BALfddhsGDBjgn3/q1CmsWbMGa9aswalTp7B7926sWbPGWb6f3DUvJuYnDMP4p2IrpZLHfIRhGP9ULuRZIqWbJqWG/fv3Y8qUKbjjjjv8vy1ZsgSXXXaZIzPQrFkzREdH45tvvvHPadCggSOnkZCQgM2bN4fJ4wRxXiuldu7cidmzZ+PTTz/1/1agQAGcOnUKhw4dcn7hSC4sZMCAAejfv7+fPnLkCAoXLoyYmBhfS4N1pFRjSGMh+deR5LQZOBZUtao43lwbWn/B4VhqjX9WLQaOndWYYY1NZTQOXGNpuSNoeVWXh+ORVdMjqK1UX4HTGjOr7cTfqTH3el3Wq9A6Uf0YbrcgnRMAzq9sGjMcHx8f8XtUpyModlrLy21cvnx5J0/biWPwVe9AtWF4wqVtqP2cy6v6NNpfuQ417lu/hw2NtotqGvCYUR0zLpNqXincr7TfqKYBX1dtgdoN7p8hGxIUB55W3HTTTTh48CAGDhyIffv2oUqVKpg+fbrfNrt27XLuc8+ePbj66qv99AsvvIAXXngBDRs29LUikrvmxSIt/ESWLFl8+8b6NKr9o/aIx5P2R7XL3HeCdNa0j6kmCNtw7avqU9gG6i/+rC0BuLoPajdUw4l1FvQ6+lDIY/jbb7918ho0aOCkly5d6h+rfSxdurR/rHZCNStYL0bvW23KwYMH/WPWNgHCbWuQ5pVqY7BOk2oeXXnllU6a7ZW2oep8cBn0XL4XrT+1c+yP1N+oVg+H6Wr7qu3n7+H+B4RrgnDIsdpsHcfLly/3j1kHBwgfe9w/9Lrcbmq/dbxz+dR36ndyv7rqqqucvI0bNzpp1SPTchmpIy18xL/+9S/fLn7wwQd+PtslIHy+s3DhQv+4cuXKYeVmSpUq5R9rf+D5t+osNWzYMOK5qs2mekQ8Z1V7wuUBXNujfXzt2rVOmse+ah/qw2XZsmX9Y13FdsMNNzjpQYMG+ceq2cRzS7V/Ol7ZTuncXNuQx68+Q5UrV85Js+387LPPnDydN7NtUjuv53LdlyxZ0snTeQCvZvn444+dPPZT2t4VKlSIeG5oBWKI9957D5FQ+6xzBK4jtbmq0/vDDz/4x8npQ3J96hxLddh4nqVzBC4Da08B4TpcrKmk47JTp05Oes6cOf5x8+bNI+YBbv8N2R2df14s9MX7448/7oyz82HMmDHIkSOHowG3b9++sDGbMWNG5MqVyx/3+/btC3uODo3Hffv2BWpEOtc9n0KPGjUK+fLlQ5s2bfy/VatWDZkyZcKcOXP8OMTNmzdj165dqF27dsRrxcbG/u2Efg3D+HuTFktuQ/Tu3TtiaB2LkgLnJhUp+Z6ga14szE8YhvFPxsL3gjEfYRjGP5n0tmnSu+++i86dOwcukvkzSfVLqcTERIwaNQpdunQJ2x3ujjvuQP/+/ZErVy7ExcWhT58+qF27dqp3yzAMw0jPpOVLqb8i5icMw/inYy+lImM+wjCMfzoX8iwR2izpYrFw4UJs3rwZ48ePd/5eoECBsJXVZ86cwa+//uqvXi1QoECSGyiF8lJKql9KzZ49G7t27UK3bt3C8oYNG+ZvFXjy5EkkJCTgtddeS+1XADh3M6El2ry0T5dta8gWN5Auo9UldLycU8Ph+Lq6hFXDOzhMI7nKDwo3047J36NLDzU0jd+Q6hJ+PVeXjDJav7xkT5fR8nV06e7hw4edNC/11OvoUlRut6Cl0IBb93qfei+81FHPVfh7tXxBoYq6RJHDaXRZqoaj8HJyXQqr4Sm8RFjfjmsf5OXOWp/aV3hprNaRhsTw92ie3hu3k5aBx7eO0aB+rnnar3g7dM3T0BD+Xj03KeylVDBp5Se4HXhpvI41XVKvIQKM2hh2tBp+xjZG7Q0vXwfcrYLVBmvf4HM1VERDzXmJvYYq6blJbWkfQpew16lTxz/WUMTQVsdJfa/6R7ZlGv6kD5m7du3yj3W5uIav8LbsHP4GhNto3tp87ty5gWXgtqlRo4aTp8vlebm62mHtYzNmzPCP1b63aNHCP9Y2VN/P/kj9jYavcHhkUBg/4I4fzdPrcn1zm2n5ALd+1U/oZ3kepr/Usi/VkBntV+x/2A8A4f2er6t1pPNCnguG8jSsnbGXUpFJKx+xZMkSvy9xWI7OUdRHrFmzxj++7bbbnDwdvx9++KF/HCR7oGGw+kDJ/UttjfYznlOrvdOHQ2bdunVOWueWPBfSe9Hxy3Wk8zH1J40aNfKPNZR4+/bt/jGHTwPA7t27nTSHpulYVpvL4YX6UK31yfZbwxQ1DJ59Y3Kh7XyvOicoUqSIk/7oo49SVF79DrW5FStW9I+1r6qMCH9W20x9ET8zq63UOQ0/W6h91n7Pcwa9b40G4FBate08ZjS0U/0z93N9DlLbwONA52P6fqBmzZr+cWhMBGk9padniXfeeQfVqlULC1euXbs2Dh06hJUrV6JatWoAzs2jEhMT/TDJ2rVr45FHHsHp06f9dxuzZs1CmTJlUhy6B5zHS6kWLVpErJDMmTNjxIgREbcdNAzD+DuQnhxJesT8hGEY/3TspVRkzEcYhvFPJy2eJY4ePepsdrR9+3asWbMGuXLl8l+MHjlyBBMmTMD//ve/sM+XK1cOLVu2RPfu3TFy5EicPn0avXv3RqdOnfyXrrfccgsGDx6MO+64Aw8++CDWr1+Pl156CcOGDUtVWf8c9S3DMIy/MfZSyjAMwwjCXkoZhmEYkUiLZ4kVK1agcePGfjq0IUSXLl0wevRoAOdW6Xmeh5tvvjnJa3zwwQfo3bs3mjZt6q9iffnll/38nDlzYubMmejVqxeqVauGPHnyYODAgejRo0eqymovpQzDMM4De4AwDMMwgjA/YRiGYUTiz/YRjRo1SvY7evToEfgCKVeuXBg3blzgNa666ipn19LzId2+lLryyiv9GG+ON9XYaU2zZoZuZ6laMawloNobjOqIqF4Jx0uqnoZqM7COlObpvbCOh56r2jt8rt6LxkdzLLDqNmgdcX5q6khjnLleNH5X44s5NlljmjVWPkivQnVGGI0n13vj+tb60zh7jj/We+Hyq5aSxnYH6bJovD6ndSt63Wadr6U6Ztr+nK/tpH2DY791K3ptC25T1engulbDqduh83W0z+m9cLto+2p5eTzpdZPCVkqlD06cOOHrSnBfUU0AhfVD1O6qtghrMuhW22zn9HM6Lvl7VAtB7eWqVav8Y70X1osA3LGmY1RtF2tuqDaCaovwWFP7w1tt6/eqfgT3e61rte98r6wdApybE0S6rto11Z9iW6XjW31BUls6h1B7xN+jbaiaMLxF+oIFC5w8toGqpaXwvWp7a1/hLb5Vq0O1B1WfhVHbyloyWn+qNXL11Vf7x6pFpluZc19W/RUuv2qcqb9krS/VD1Ttk6DvVI2an3/+2T8O6WEF6VPaSqlLz5EjR/w2Hj58uP933hIecHWCAHcc6sOY6h4FaUHxnFXbV+0f+wX1H2q3eB6lmq46Hti2d+7c2ckL7XAYgvWK1N7pcwc/Y+mcT+0Nl3Hy5MlOHuvZqfaPjl+2eTqWp0+f7qTZxqld1fplfbuEhAQn75tvvnHSIR2dpMqnumHLli1L8jsA4MYbb3TS1atX94/Z1gCuz1WNHtUJY7ulcw2eWwCuXprqT+nzDNeZlk/bgucBrLmWVJlYQ1P9/B133OGkWfdK5yH8zKK+kdsBcPtG3bp1nTy9lyVLlvjHOl6OHDnipFlPOeSndH7C2LOES3TypxiGYRiGYRiGYRiGYRjGxSXdrpQyDMNIr9ivG4ZhGEYQtlLKMAzDiIQ9S7ik25dSp0+f9sMhOPRGl/3p0nFO69JrXSqbO3du/1iXcnJaw430ulw+XT6vnYfDATQ0QOEl/XquLk3kJfP6nRo2xktwdXmuhjxy+Id+J4eraOiHLsHlz+pSRg2HC6p7DTHgpdEaGqLhFBzOp/fN2+sCbptq6IIuo+al0kFhYtzfgPBlv9x3dctcDRHgvqyhnQqXSe9b4a1vdbwEbeup7RK0XJWXt+p1td/offNntR00fIrTuhxXwz84JDd0L9qfGHMk6YOoqCi/vXi7Yh0/utSc7aWGG2lf5mXoat95fKud1fHOtjQoRBBw+7b2c15KDrjL3dWW6hjm0IIyZco4eerX+Hs1lFe3DNawJ4ZDANSGaAghh4VpCMp3333npHl8avvq93BabaCGW7Av4z4FhIdfBNlsrU+uIw3BrF27tn88Z84cJ0/nPByGoH1VQ4e472r/1Dbk0Dq1jxr6EuR31QfydbVdNByIv0fLy9+j8yH1geyzdUt59ec8FvU79V44zCTUP/UzjL2UuvSULVvWH4s8tnX+9f777ztpHr8aBj1lyhQnXalSJf/422+/dfJYpkF9jdrn0qVL+8fqa9QGc5nU9qh0xddff+0fr1y50skLbfEegudcy5cvd/KqVKnipNm2awihhnGzzbjrrrucvKlTp/rHOuY4NBIAOnbs6B+/++67Tp7WZ40aNfxjDSfUEEIOM+bwXyD8vrdt2+Yfs00A3PAyALjpppv8Y9XbUb+1du1a/7hVq1ZOHrcLfz8Q7n+5P2oIns5LPv30U/9Y7bPaTg4v1O9Uf8LzFH2u1LnH3Llz/eN69eo5eSqZ0Lt3b//46aefdvLYH6uPaNKkiZPmfqThufr8wu0/bdo0J0/7Obdp6FlW53uMPUu4WPieYRhGKgk5ktT+MwzDMP4ZpIWPWLBgAdq1a4dChQohKioKkyZNSvYz8+fPR9WqVREbG4uSJUv6OzCFGDp0KGrUqIEcOXIgX758aN++fZhOm2EYhnFh2LOEi72UMgzDSCXmSAzDMIwg0sJHHDt2DJUrV8aIESNSdP727dvRpk0bNG7cGGvWrEG/fv1w5513YsaMGf45X331FXr16oWlS5di1qxZOH36NFq0aJHsBhKGYRhGyrFnCZd0G75nGIaRXrElt4ZhGEYQaRG+16pVq7BQnyBGjhyJ+Ph4/O9//wMAlCtXDosWLcKwYcP8Xcd0F7PRo0cjX758WLlypbM7m2EYhnH+2LOES7p9KZUzZ04/HpNjjFVfQ7ch5ThS1ToI0i7SOOYgHR6NC+fv0fLpudyZVMdKdRFYP0fjyVV7R2PeGY2PZR0H1b3QOFzW9VAtBi6/xi1ru3B5NZ54x44dTpp1pDT+mbV/tHxaB3ovXAatE42lZm0l/U5Nc7tpPXCdqT6S6nZwbPqWLVucPO0r/FndklR1uDjOWrVrtM5Ye0nLp4aQ+7bWp+qP8b1rP2ftL437D9LLUp0o1YjgOtP21c9yPwvViWlKpX+WLl3q29xy5cr5f1f7U6RIESfNY0Z1E1SfgzVjVN+H9QNUwy5IH037lvoJ1gb66aefnLwgXR49V7UMuJ8np3HHWyar9pPamHbt2vnHah+XLl3qHwf5F8D1DeqT1XYtXrzYP77mmmucvKC61y2nVZeJy6TX1fKy5ormlS1b1knz3EDt7urVq/1jtedcf4DrY1RDivVrAFffRG20hmNdddVV/rHqJKmuC7e/2mytT9bhSq7PsU6J+jwe0zq+VdNS8xkdEzzP0uuo5gu3Tcg3qa4pc74vpbQPxMbGhvXp82XJkiVo1qyZ87eEhAT069cv4mdCdaT276/Ajh07/HkY2/aJEyc657Vs2dJJ86qwkiVLOnn6TMBts27dOiePx6RqPdWsWdNJjx07NuJ3qs/gsa3tyfNXwLXf+hyk8zy2N6y7o98JuHN3HVeqm8faQPoMMGHCBP9Y9ev0uitWrPCP1RfqSj7WaFKbtmnTJifN9lp9eZD+r85R1Q9wP1N/or6SNbFUm4z9sfZdte1BemP6jMp6T1pHem88/rVd9Pnmlltu8Y9ffPFFJ0/rlzUV9b61Pr/55pskyw64GpCqQdm2bVsn/frrr/vHam+Vxo0b+8dadp0/cl8J+XW9B8aeJVwsfM8wDCOV2JJbwzAMI4jz9RGFCxdGzpw5/X9Dhw69aGXat29f2IuJ/Pnz48iRI0m+YEtMTES/fv1Qt27dsBcNhmEYxvljzxIu6XallGEYhmEYhmH8k/jxxx+dFXEXa5XU+dCrVy+sX78eixYtumRlMAzDMP7+2EspwzCMVGJLbg3DMIwgzjd8Ly4uLkwK4GJRoEAB7N+/3/nb/v37ERcXFxZG3Lt3b3z55ZdYsGBBWNirYRiGcWHYs4RLun0pdfjwYT9mlWNgVQtG46xZy0Y1kFRngD+rscl8Hf2c6uXwZzVGWM/VNKPxvPzrmOapNgPHUmscsNYRx8Nr51aNKZ6kaOw512+Q9g/g3rfGHgd9p5ZdY385nZzeAWuv6ORLy8TL2zlOOany8gSPdW0AN9ZbdVg0HprR+2bdC8CNu9+2bZuTF9QHNR5a73v79u3+scaiq1YI9wdtf9WDYd0RrT/W7dD7DNJ10v6oegI8fjRPtUy4DUNjIsjwmyNJH9SuXdvvT2ynVYNPtTy4f+q5qsvEtkK1JTjchfUggHCtPNYI0X6tKyHYz2neFVdc4aR5/LAuHRBuu/jcffv2OXnqA1mPQzWlgh6Y1UdXqlTJP161alXgdVjXQ8e3+uHvv//eP65QoYKTp1pAbJ9US0RhfQt9eNc2XrNmjX+sdm3jxo1Omv2T9iNuC9aX0jzA1ZFSOzZ//nwnzf5RNUA0zf1c7WWxYsWcNNen6mNpm7Lmhvoq1XorWLCgf6z9nv2Y+gn1YzwOtD+qHhBfS3W2uDyA61tD84mL6SfSwkfUrl0bU6dOdf42a9Ysp997noc+ffrgs88+w/z58xEfH/+nl+vPoly5cv7YHD58uP/35s2bO+exZg/gzndmz57t5LHGDODaep2Hss3QscH6SIBrr3X+pRp17AdYiy2p8vHY4Xmw5gHA1Vdf7R8vW7bMyWNdKMC1Pzqf/eKLL5w0j2cdkyzUn9x3sm2qXLmyk7d+/XonzeNXday0vDwP+Prrr5087f/si3TOr9qHH3zwgX+sek46T+bnDg2xZTuqGmILFy500tyvNCRX65Ovq+2icyEeE3fffbeTpyspOa3zrylTpjjpefPm+cd33nmnk6fjiW393r17nTz2SzoGlixZ4qTZR5QuXdrJ0/HEO5PeeOONTp5qSvFzccOGDQGcawPVAQthzxIu6fallGEYRnrFHIlhGIYRRFq8lDp69Kjzgnb79u1Ys2YNcuXKhSJFimDAgAHYvXs33nvvPQDnHiZfffVVPPDAA+jWrRvmzp2Ljz/+2HlQ7NWrF8aNG4fPP/8cOXLk8F+M5syZM+wHPcMwDOP8sGcJF3spZRiGkUrMkRiGYRhBpMVLqRUrVjirAvr37w8A6NKlC0aPHo29e/c6OyDGx8djypQpuO+++/DSSy/hyiuvxNtvv42EhAT/nNDOVI0aNXK+a9SoUbj99ttTXUbDMAwjHHuWcEm3L6Vy5MjhbwnMy9d1m2ANKeIQBA0p0mWrvHRStzXmZakaBqjX5eXfuiRel8YGhdnpkn4OBwja4hhwl/RriIEuGeX70e/U8vMSYS0vL8fVdtFlqRxGoCERujyT20nz9Lrc/rr8WreW5RAUDa3RpbLcTnpvCi/9VGPBISga3qHl462E+ZdPIDzch5fgalighidwfWobaigQL43V+9Z+xNuc6nU17IH7SlCon44X/VWW61fvM6h8Wh4NT+F+FqrrxMTEiFvFmiNJH0RHR/s2i0Mjtm7d6pynoWAchqN9TG1B0Fb0HNak/VptDC/rVzvL9htwwzj0XA2XYrun/VrD2ILOVTvC+brkX8MbeLm7hvpx2ESJEiWcPB3vfG+6zbWGW9xwww3+MS//B8LDwridtF00PI7tiNpADRPjkA/1Pxp+w/kaQsjl5xBqAKhSpYqTZrvG4YOAG3oIAG3atPGPx4wZ4+RpKDeHrqnf1T7HZVA/piEV7Lu0TqpXr+6k2d4GjUttB+1z3HeCwroBOFpJWnYNxWEbE/KrQSHmafFSqlGjRoGfGz16dJKf0TDRCy1HemXEiBF+W911113+36dNm+acp88HLJGh9aEhZmwHWrZs6eTx2OHt7AGgXr16Trp+/fr+sdoTDc3lMDud8wc9z6gP4zBtwA17uvbaa508DWN76aWX/GOVGAnyaRoWxnNjHYNqg7lMaivVprEt1zYrWrRoxHPVby5dutRJc/ic2mD1W4MGDfKP9d5Up61GjRr+8eTJk508DlEfO3ask6c2mK+r9ffdd9856Tp16vjH2i4amsg+QsPhNESP/RbfFxA+1vilufYjDXldsGCBf6zzEp7n6xyFxxbg1oPKHOh4atGihX88adIkJ099Loct3nfffQDOhUWGfixQ7FnCJd2+lDIMw0ivmCMxDMMwgkiPmlKGYRhG+sCeJVzspZRhGEYqMUdiGIZhBGEvpQzDMIxI2LOEi72UMgzDSCXmSAzDMIwg7KWUYRiGEQl7lnBJty+lfv31V19LQ2N0GdXp4XhU1avQOFZuWM1jnQDVrVKtA9a20TyN31ZtE0bLy9+reiWqr8H5HAuv5QPcuGvVV6hVq5aT3rJlS5KfA1wNEq0j1ffhmGfdgl11orhN9+zZEzEvuetqLDX3I40nV20lvlfV3VJdAP5ePZfR2GjW5QBczQxtb41x5jbV62p7cx9ULQ6tz6Btt1WXicuk40dj51krRLeo5X4UpMGm+cn1OS6TbnWraS5DaExoGxjpj6NHj/rtxO2tOoDaP1lzSDVh1Gazn9C+y/1cbWnQLlV6ro5v1kBi/SsgXJeJ9RhU30L7MOuU6PhRXR62y2qHVRuI9fB0bK1atco/Zm0TIFwLg+tBtQfVT/CYVZunbcq2jLU5gHBbxW2jui6qNcJl4DoAwrVl2B+pHgdrYWofU80r1rBQ/TPdNp51M1SbSm0/t5v2Xe2v7EdUo0u/h+cQJUuWdPK0frnN1Sez7odqXmm/4q3h1T+qj+a+oxpXPLYAd/tvLZ+RPrn22mv9/sy2Xe3Ahg0bnDSPX51LqhYQz5tV347nmsuXL3fy1O6zr9F+Wr58eSfNmmBqM9Susq7fBx984ORVrFjRSfN4UE011ssBgJo1a/rHap9ZfwhwbcjKlSudPPZxamuaN2/upFmPT22P6hF9++23/vGtt97q5Km/Y9vO9QWEP1N99dVX/nHdunUjXgcAxo8fH/Fc1ejiOazWJ/crvY4+D7Id1T6mNm7hwoX+sfrNypUrO2m2+3qf11xzTcQy6TOT+rS2bdv6x6r9xLuCAkCDBg38Y9XF4+/s0KGDkzdz5kwnzXWvdaTPZkFauzqP4vET0rXSfmlEJt2+lDIMw0iv2K8bhmEYRhC2UsowDMOIhD1LuNhLKcMwjPPg7+wYDMMwjAvH/IRhGIYRCfMR/4+9lDIMw0gl9uuGYRiGEYStlDIMwzAiYc8SLun2pVSmTJl8TSmO2VStENXMCH0GSF4rhHUcVLeDz1WtGo035e/U2G4tA3+nEhR3qtoL+j0c88z6PUC4PgSXV2NpNdabY+e1HjimWNtBNR9Y+0I1PFSfhGOpWT8DADZu3OikWftJ8zQGnzWRVFtJtS5++ukn/1gNQOHChZ30wYMHEQluF+0LrPcBuBoVeq7WJ9ehnst6NFo+jQPX+H3WXmG9FP1OwNU80DrSPsj6JaqrxuXXfq3jhetT70XblO2Gjn3VGOKxF/qc1itjjiR9kDdvXr9vsXaN6jGoBgj3c/Upqs/AY0SvyxpnqgGi2gPcl1U7TfU3+LNqv1X7hMeE+ibVDWJNEy2fjvcDBw5ELK/WJ+umqC4h60fofar+FNtdtcl6LuvNaZ2o7tZnn33mH6uNUc0htiuq2bR169aI52r9/fbbb06aNZGqVavm5G3bts0/Vn0k1Yli/Q21Kax1Arj1qfp8VatWddJ8LdXFUZ0o7suszwaE23fWJdH+yRpNALB9+3b/WPscl0/1DtU/cp/T+gzSD/3hhx+cPB3TPHcK+TjtT1pmeyl1admzZ49vw4sXL+7/vVGjRs55PAYB1z6qxhDr5AFun9L+zzp/mqdzQH4OUX1AHa+sibNixQonb/To0U6a71tto44dHpOsyQSc0+di2B7qfKxp06ZOmv0o2yUA+Pzzz/1jHZ86fj/66CP/+LHHHouYB7hzfrWNQX5q6dKlCILHvJZX9Q253bS9mzRp4qTZZ+gzKT/rsC8Bwv0Uz4VbtWrl5Gnf5evqM2ilSpWcNOt5qX1W/bG5c+f6x6qvqBpTPC5U71fnP9xX6tSp4+SxTpjO38uVK+ekefzoeNG5Bz/P6BjWucfVV1/tH4e0OC+mjwh95u9Kun0pZRiGkV4xR2IYhmEEYS+lDMMwjEjYs4RLdPKnuOzevRv//ve/kTt3bmTJkgWVKlVy3tJ7noeBAweiYMGCyJIlC5o1axb266JhGMZfmZAjSe2/fwrmJwzD+KdjPiIy5iMMw/inY88SLqlaKfXbb7+hbt26aNy4MaZNm4a8efNi69atzlLu5557Di+//DLGjBmD+Ph4PPbYY0hISMDGjRvDwiSCiI6O9pdK8/LI5MLjOLyClyWGrsnwUkUNE+KlqLrkXMMeeBmjfofeMy/t1BAnDT/iZYL6nbwcF3CXc2bKlMnJ0+X/vERUtzrVUDReyqv1yXWvy9x1m0wO/dNwPW1Trk9dGqtb3XJ5tQxa9xx+pu2kW5Ryfet1g0LgNMSRl9VqyIG2Ny/t5WXHQPjWt3nz5vWPdcmtLvvlfqb9SI0b15nWkY4Rbrfktt3mEA8NI+H71hAY7XO87FvLo+EyPNY0jEnbic8N9WsL3zs/0tJP7Nu3z1/ezfZSl3zrUnMOleUwNSB8G3juOzzuFP2c2lYelzoG1M5xuKnaR92Knm2/hpnw1tCAO/7VFugYZtulfkFDmNlHqn1v0aKFf/zee+85eVr3fK9advUpXH4NM9CxxttM67bs6t85reHsei7bCG1DtWUcWsChpoB739ouGvK4fv16/1hDjrRfsR9Rn6L1y/5Jtw3X8BAeoxoCrmOP61vD/DXNdlglCzg8RP2L9iPun+pnNZSb61tD3xUuX8iHBMku2EqppElLH5ElSxb/fLblOnY0ZIfH75w5c5w8DV/mfLX77BeaNWvm5Kl8BvdFDU3SsDAOgVKpCp1r8vjQOZXeC7eBzrd1TsRzar23UOhSCK4XtcG33nprxLK/9tprTprz2aYC4WOb7f78+fOdPA7pBoCaNWv6xxzaBYT7P24LvU8NE+S5ZteuXZ28L7/80klXrFjRP9awRfYD7FOB8DBoDnVXn6AvdvnZh+sAAGbNmuWkObxZpVW0TTnkW+3znXfe6aSnT5/uH99///1Onvp9HqfqI9inqY/4/vvvnTT7CL0X/U5ufw37XLx4sZPmMoU+p/MGxp4lXFL1UurZZ59F4cKFMWrUKP9vPHg9z8Pw4cPx6KOP4l//+heAc5PQ/PnzY9KkSejUqdNFKrZhGIaRHjE/YRiGYUTCfIRhGIahpCp874svvkD16tXRsWNH5MuXD1dffTXeeustP3/79u3Yt2+f88Y8Z86cqFWrFpYsWZLkNU+ePIkjR444/wzDMNIztuQ2MuYnDMMwLHwvEuYjDMMw7FlCSdVLqR9++AGvv/46SpUqhRkzZqBnz57o27cvxowZA+D/lwHqUu/8+fOHhUeFGDp0KHLmzOn/07AAwzCM9IY5ksiYnzAMw7CXUpEwH2EYhmHPEkqqwvcSExNRvXp1PP300wDObX24fv16jBw5El26dDmvAgwYMAD9+/f300eOHEHhwoVx5swZX9OG9RZUL0ljnFkHR3VkdEtp1gJQ3QG+jsaIa2w3dxC9jsZv82c1Ll7TrFGR3PabfK+qtaNaF3xv+p16rxy/rfHajN636pMExfrqlrR8bxr3r7G+rCOjsfE6cFmLZe3atU6e6njwZEjbWzVT+H60HlRnhtH7Zj001eW46qqrnDT3+4ULFzp5QVvRq06UxqJzHLvqHQRpzpQqVcrJ0zh2blONlWe0/yk8/jVOW9uf49hVu0TrgeszdN30oik1YsQIPP/889i3bx8qV66MV155JSz2n5kwYQIee+wx7NixA6VKlcKzzz6L1q1b+/lHjx7FQw89hEmTJuGXX35BfHw8+vbti7vvvvu8yqekpZ+Ii4sLs/NJwWMLcO2e9muFdTNUUypIo0l/qWd/o2NAbQHbOS27lpevG6TjAbj6Uzq+9Xu4XnXrarVzvHW4+io+t2HDhk6e3svUqVP9Y7WBrGcBuFuba55uK719+3b/uHnz5k5enjx5nDRv8axaGHou64SpForqUXG+6lCwT1EdF30wX7dunX+8ceNGJ091o1grQ7eyDtqeXvX5tJ3Yp2hf4PIBwIIFC/xj3ZZby8/aOOqbeDzpeGHNQgBYs2ZNxHNVj5NX3uj8UnW3uH5DeiEXc7vvv/PDBpOWPoLh/taqVSsnT/VpWBsoFEIYggXZAXduqTa3cuXK/rHafbWVrF3DK8cAV3cJcH2Rzn30e1jXSPVJ586d66TZ3qg/admypZPmZwuta9U2ZR/B8xHAnSfrdfr16+ekR4wY4R+rvqvaKdYq0vmczuO/+OIL/3jgwIEIgvWodMw2atQo4ueSE+pnP6a+kp+/9LlCy8B6aPp8oM+kbA/Vb7JPUPTZTP0J28Ubb7zRyZs5c6aT5vKzrhYQrqnIWlU6Z+EX1jq/0XHJ5dO+oGOC/Z1qZ7FuGeDO3ULfoT6SMU0pl1StlCpYsGCYoF65cuX8ARIy6urI9+/fH2bwQ8TGxiIuLs75ZxiGkZ5Jq183xo8fj/79++Pxxx/HqlWrULlyZSQkJIQ9LIdYvHgxbr75Ztxxxx1YvXo12rdvj/bt2zviyP3798f06dPx/vvvY9OmTejXrx969+7tTMouBPMThmEYtlIqEuYjDMMwbKWUkqqXUnXr1g17a7llyxb/7Wp8fDwKFCjg7ERx5MgRfPPNN2Hq9oZhGH9V0sqRvPjii+jevTu6du2K8uXLY+TIkciaNSvefffdJM9/6aWX0LJlS9x///0oV64cnnjiCVStWhWvvvqqf87ixYvRpUsXNGrUCMWKFUOPHj1QuXJlLFu27LzrgzE/YRiGYS+lImE+wjAMw15KKal6KXXfffdh6dKlePrpp/H9999j3LhxePPNN9GrVy8A55at9evXD08++SS++OILrFu3DrfddhsKFSqE9u3b/xnlNwzDSHPSwpGcOnUKK1eudMReo6Oj0axZs4hir0uWLAnbmjkhIcE5v06dOvjiiy+we/dueJ6HefPmYcuWLWHbDJ8v5icMwzDspVQkzEcYhmHYSyklVZpSNWrUwGeffYYBAwZgyJAhiI+Px/Dhw9G5c2f/nAceeADHjh1Djx49cOjQIdSrVw/Tp08P0y5KDo7/Za0O1s8AwvV+OJZW4001fpvjrGNjYyOWRb8zSFciSE9D09qxVK+Ez9UyaNy1auYwGvvL56ouT8mSJZ00x9qq3gKHEGmdqI4Vx0OrppRqcXBcs2pnaT2wNpBquKjWDLeT6nRoTD7ryKiWFvcxwI0h1nO5D+p36r1wf9S61n7EsenadzV2nttY+5x+D48n1mwBwjVzuM6CvhNw60x1ABgdP7p8n8ugda0aJKwlorZAP8vlD7Wn6pcx5+MYQudrP42NjU3S/vz88884e/ZskmKvkWL99+3bl6w47CuvvIIePXrgyiuvRMaMGREdHY233noLDRo0SNX9RCIt/cQvv/zijyO2OWqPVGODNRm0n2/ZssVJ8xjR8bJz507/WPu8ajew5oLqJen44XGo9kbtJ9uN5MY3h7Tofaod5vGjWhg6NoK0J7juVcdFtYtYB0J1HjTch8ew6jBpebgedM6gukase6S6HtoWIWFmIFxHT/1uvXr1/GPWoAGAVatW+ceqgaR1VKFCBf9YfYjCujjaH1U/JD4+PmKe+mHW6OL+BwDff/+9k+Z2076rIVbc/qp9w9odOr/QOmP9ENUSVaFsnifo+Amq31AdBZ2TWj/xd37YYNLSR9SqVcvvdzxGJ0yY4JynPoP1lLT/axm4r2rf5LTqLKk2UNWqVf1j1ar5+uuvnTTbR53PaPlYwyc5XSuuI9bD0usAwE033eQfz5gxI7AMfO9a1/yjmdrGTZs2OWm2z2qndG5Vp04d//ijjz5y8lQvi3XDVPNP/R2XsVKlSk6e2heuT/1Ote2lS5eOmMdzX34+Adx+o9/z7LPPOnn6o2XHjh39Y9VB1HZi/6crFlkPDTg37kJov9G5B/eN5DQVub/y/Eu/U5+ZtN/zc7D6av1OfjZnXw3AkcYAXH3d0HfqPIy5kGeJlLJgwQI8//zzWLlyJfbu3YvPPvss7OX+pk2b8OCDD+Krr77CmTNnUL58eUycONHXa2zUqJEznwCAu+66CyNHjvTTu3btQs+ePTFv3jxkz54dXbp0wdChQ8NsYhCpeikFAG3btkXbtm0j5kdFRWHIkCEYMmRIai9tGIbxt0dfKD/++OMYNGhQmn3/K6+8gqVLl+KLL75A0aJFsWDBAvTq1QuFChUKm7CcL+YnDMMwjEiYjzAMw/jzOXbsGCpXroxu3brh+uuvD8vftm0b6tWrhzvuuAODBw9GXFwcNmzYEPZiuXv37o495h90zp49izZt2qBAgQJYvHgx9u7di9tuuw2ZMmXyN7RICal+KWUYhvFP50J+3fjxxx+dFQKRVmnmyZMHGTJkSJXYa4ECBQLPP3HiBB5++GF89tlnaNOmDYBzOzuuWbMGL7zwwkV7KWUYhvFPx1ZKGYZhGJFIi5VSrVq1ClulzjzyyCNo3bo1nnvuOf9vGkEAnHsJFenZY+bMmdi4cSNmz56N/Pnzo0qVKnjiiSfw4IMPYtCgQWErqiORbl9KZciQwQ/N4tAGfXOnYRC8ZE+XjGn4ES+p0y3ieTmsLm/VJaL8WV2erqECnNZG0i0s+d50u01drsvX1U6jSwc5rcsWFV4Gr+GFfB19ENYwB24XrU8tL4cFFitWzMnT7+F60WWzvP054Na3lkFDV/gNsC7l1GW1QaGTvOxbty3Xbay5v+pyce3nvHxYw0aCtqbXkAgNG+LxldyScK4HHWtBdaKhklx+DYXQEExuJw390H7O52qdaCgLhxSGyq51w1yII0npzkAxMTGoVq0a5syZ4y+1TUxMxJw5c9C7d+8kP1O7dm3MmTPH2UZ51qxZ/lLr06dP4/Tp02H2LkOGDIH3m14pUqSI30fYNmg/52XxgLssXbd017HGS/fVvvMYUfuoLxs5jEjDAXTpO7ePluenn35y0jxmkgtrYmrWrOmka9So4aR5WbqGVCxYsMBJc5jbrFmznDwe3xp2oOEXbO81HPeqq65y0t98841/zMv2gfD2L1iwoH+stlXbib9XQwg/+eQTJ80hm1dffbWTpyEVHPKm5eW6Vt+kbcjfec0110S8DgCsWbPGP9YVmurzOHSf6xYAmjdv7qSrV6/uH6tgdVAot9p3nSewz9atwTnEQ8eP+kC+V50HaMgHzyGC5jiA6wND92Lhe+mbuXPn+mOc5x4crgqE24HQjzZAuC1SO9ukSRP/WG3auHHj/GPt0wkJCU6a+yqLvAPBzzrqE9Tf9e/f3z9W+6zl5bmQ2n2tIx53OlefPXu2k+Z8taN8L+vWrXPy1FZyaJq2y3333eekP/zwQ/9YV+Wp3+c5me5urOey71T7p+HCbIM11E9t8tKlS/3jV155xcljO7VhwwYnT+uBv+fjjz928vQZip+bdN6u9cD+Zt68eU6e9u0VK1b4xzrfZH8MuP1K5+Ya8sq+qXXr1k7ewoUL/WP1m3ov7K815FzbkJ/V1G/qMzSHCYaebS+mjwh9Bki5FEgQiYmJmDJlCh544AEkJCRg9erViI+Px4ABA8JC/D744AO8//77KFCgANq1a4fHHnvMn38vWbIElSpVcp6XExIS0LNnT2zYsCFsfhSJVAmdG4ZhGGknTti/f3+89dZbGDNmDDZt2oSePXvi2LFj6Nq1KwDgtttuw4ABA/zz7733XkyfPh3/+9//8N1332HQoEFYsWKF/xIrLi4ODRs2xP3334/58+dj+/btGD16NN577z1cd911F6dyDMMwDBOwNQzDMCJyIc8ShQsXRs6cOf1/Q4cOTfX3HzhwAEePHsUzzzyDli1bYubMmbjuuutw/fXXOxpSt9xyC95//33MmzcPAwYMwNixY/Hvf//bz4+kZxvKSynpdqWUYRhGeiUtltwC54REDx48iIEDB2Lfvn2oUqUKpk+f7hv7Xbt2Ob9C1alTB+PGjcOjjz6Khx9+GKVKlcKkSZOcX7E++ugjDBgwAJ07d8avv/6KokWL4qmnnsLdd9+d6vIZhmEYSWMrpQzDMIxIpIUUSBChlc3/+te//JWGVapUweLFizFy5Eh/FXyPHj38z1SqVAkFCxZE06ZNsW3btiRD/c4XeyllGIaRStLqpRQA9O7dO2K43vz588P+1rFjR2dHFaVAgQIYNWrUeZXFMAzDSBn2UsowDMOIRFpIgQSRJ08eZMyYMWx343LlymHRokURPxcKq/3+++9RokQJFChQAMuWLXPOCYWKRtKhSop0+1IqOjraXwHA27lrjLPG+nKMc3L6Tqwzo9oBHKupbx91S3sugy5f0xhdjqXV66jGlG5hyahuA6dVM0G1gDjW9vLLL3fyNDad9S1U64LRWGmNA+b4fdWR0G1xOeZZY/d5O1j9Ho3P1lhvbgvVGOI+Brh1pjHYqovC5xYvXtzJC+pH2r5r165NsqxAuOgcD3Id8BqTz3WoW7wG6aNpGVTficeajkONGeeYbO0bXCbV3dIxy31HddZUZ4S1B3S8aMw4j72QvkFyjsIeIC4927Zt87U2WLtGtxXWMRyUp/aSfYNu6Rw0DlW7iPX51NbreNm6dat/rP1MdYO4b6v/UXvO2xWrFoLqWvG5Ova1ftk38H0Crm3QbZonT57spNmmqK369ttvnTTbT9UN0jTXg9pd3Xqd7fDYsWOdPLUbrHei+k66ZJ3tk/YNruuNGzc6eepbuT9qu+g8hutQy65twZpXrC8FhPsC9pe6RXaVKlWcNM9ztM+pz+YxrNuTs46VjhfV4+QxoWNNJ/Hs87TutZ+zdktoXKrvU8xPXFoOHjzo9wHWWtL+r88WU6ZM8Y91Xqe6mKyvyVo6AFC5cmX/mG0LED6uuH+ppqfOH3msq37T3LlznTRrXumcSsfHjTfe6B+zNiUQrht15513+sevvfaak8f6PgDQuXNn/zhoTGjdql5SkC6v/kjHD8l16tRx8nSss/3W9tYx/t133/nH+gylabYhqouoc2Hug6rbyM9JqtHUrl07J83zaNUzUi1bLoM+F6kt52eL5HS3+DlJ61NfdrAIt44frSPWN+R2ANyxpvqAOm/iOQuvAgKAwYMHO2n2o6oVqc+O3K9Cem3p2UfExMSgRo0aYc/LW7ZsCdObY0JaaSFfXLt2bTz11FM4cOCA3+dnzZqFuLi4sBdeQaTbl1KGYRjplbRcKWUYhmH89bCVUoZhGEYk0uJZ4ujRo46Y+/bt27FmzRrkypULRYoUwf3334+bbroJDRo0QOPGjTF9+nRMnjzZf8m7bds2jBs3Dq1bt0bu3Lmxdu1a3HfffWjQoIH/orVFixYoX748br31Vjz33HPYt28fHn30UfTq1StVYYX2UsowDCOV2EspwzAMIwh7KWUYhmFEIi2eJVasWIHGjRv76dBunF26dMHo0aNx3XXXYeTIkRg6dCj69u2LMmXKYOLEiahXrx6Ac6upZs+ejeHDh+PYsWMoXLgwOnTogEcffdS/ZoYMGfDll1+iZ8+eqF27NrJly4YuXbpgyJAhqSqrvZQyDMMwDMMwDMMwDMP4m9CoUaNkX2R169YN3bp1SzKvcOHCzk58kShatCimTp16XmUMkW5fSv3xxx9+3CxrfKgugsZqckysakdw3Dfgau1oHus/qDaV6hxxbLeeq9flOHbVVlKNKY5j1fvUNJdB49T1XK7PIE0HwK1v1VLiWGnWAgFc3SrAvVeNcdb75lhgjX9XnQ6ON1Z9DY1j5mvpdVU74vDhw/6xxohr+/O9ajw8azapVo1qdHEbamy36r3wuaqJo9pK3B+0fKrhxGXSWG4dT2XKlPGPWY8EAC677DInzW2+fPnyiOVVjauQXlBS19H71CWiXIeapzH5TKg9ExMTw8ZvCFsplT44efKk3w9YT0Dj/HX8sK6MapPx2Adc7QTVo+H+qeNZbSKPH43f177Mdll9io5D1s9Rm6f6gvw9ao927NjhpFk/q0aNGk6elumbb77xj1kfSb9HfYi2C/sbHbNqd1nPSdtww4YNTpo1nFR3i5e1A6491/vUfsV2jzWPAODLL7900mx71ffPmTPHP1ZdKLVBnK91pFpafK/qZ9W+a7sxQZpsqiGmbcFl1Hth7TTA9bXaN7jOtC9oG7J913PVn/OcR+te51Lcl0N5eg5jK6UuPWXKlPHbjW20zhfV7rNOGfsW4JzeCsPaKyGtlRD8nWpzdf7NuoSFChVy8kaOHOmkedw988wzTp5q4bHdCtJlBeA8VLZu3drJ0/7J56puTM+ePZ3022+/7R+rP+E5P/sSIHzOynWvensffvihk+Yt63Wuqz533rx5/rH2jdAOZCFYN0jtlGoUsj6fzhHef/99J83+m8sOuPMQtaOqv8d+X7UZ1f5xP1OtQ64TAOjatat/rPeicxpuU63PBg0aOGnWfNRnfO2D3I7apjfddJN/zD4VCO9HrGep7aBaWlw+HfuqM8r6WKF2Uv06xp4lXNLtSynDMIz0ijkSwzAMIwh7KWUYhmFEwp4lXOyllGEYRioxR2IYhmEEYS+lDMMwjEjYs4RLun0pxQ3FYTgaiqZhWLpUkdElhLw8V5d4czooRBBwQ5V0a2L9LId/6BJMDXnjZbVaPg0N4fAz3cZRQ/J4GaOGrekyQ64zLR+ndQmrhm/xkn4NMdB24QGn4Vy6BSwvjdW+oFuWapkYXdLK6L3pdtRch3ovmzZt8o91y2ENveBl1RpepmEjHE6h9al9jpdK69JYXSLOfS65EEfeqldDGDScj8uvbcphJbrEVvsjLxnWLZP13KAwUB1PXKbQd3BYlGKOJH0QHx/vjzluY7V5Oka4v+pYU7vMIRYaTspjTW2/jm8Ot9CwMN3amO279nNdNs8hDNpn1R+yjdHr6lbMbGs1PErHadOmTf1jrQf2E7NmzXLydNtmXgqv4TQdOnRw0rw9ubaZtj9v960hhLp9Om8br2ioGod7vfnmm06e+huu79GjRzt5HEqiISm6jTz7H92iXW00b4Ot25FrX+FzeetvINx38feov5kwYYKTLlGihH+s/Uivy/ej9cBjVttbtznnUBINldR5gfZBRv0l+/eQLQiy6/ZS6tITExPj2zIOw1Hb+O233zrpRo0a+ce7du1y8nQ+wf1E/QmHxep3Llq0yEnfcsstEctz7733Omm2peo/tE+zndL+r2Fs1apV8481VFznwhzyrWNQr8v2R+uI7bWGE2roHIdFN2nSxMl74IEHnDTPQ3UOreHWHKqmc8kZM2Y46bJly/rHep8a6sx+VMPhevXq5aR5/KuGD8teaHiZ+iW2uRpOqmXgZwANwWO/Drj2W8PY1Bdx39E5v/pG9j3ad/k5A3Cf1bQNuXzcRkC4H2VbcN111zl5Gv7P4YY6P9BzeX4W6udBciH2LOGSbl9KGYZhpFfMkRiGYRhB2EspwzAMIxL2LOFiL6UMwzBSiTkSwzAMIwh7KWUYhmFEwp4lXOyllGEYRioxR2IYhmEEYS+lDMMwjEjYs4RLun0plSFDhiTjMPVvuv0wa8VoDLHGCfNn9bocg626Agrnq7aOapCwHlVyukG8faxu1am6RqyboNvOqhYUf4+eq1onrB2i97Zv3z7/WHVONA6YdSdUD0sJ2kJctZ84bllj5RW+lmpvaHw0a6+o7pJuGx3pOwBXM0PjqPXcIEOjceusTaDb1Gs/CorX1/h37ita16oVw+NHNZq4bwCuFoHqgnG9aOy51jVrehw/ftzJ0/HN+aoxo5/l8aN6EUb65dChQ75WD/dBbW/VF+B81ZvSsZY/f37/WPVz+LNq89SWsi/Q/qf2nPWo9DtVc4G3Edfxo5o9X3/9tX+sNk+vy2VUPYZVq1Y5aa5f9QVsU6pWrerk6b2x9pNqqqh95PGuuhmqP8XwNuYAcPXVVztptq3q89QPL1261D9W7SLWWwFcO612jfuualaqbQ3qc6oLxjofqr+ydetWJ80aXqp9wxolgNverAmYVPnZ37MGJODqtQGuLo2Wga+r7aBaKKw1ou2gWm88f9Oxr+OU+0PIF6k2m5G+KFCggN9W5cuX9/++c+dO57z4+HgnzX2sePHiTp76F9Z00rkl28PKlSs7eWqvP/vsM/9Y9Ul163m+ltpufWZh26njU8dO0DOK2n2uF9WLU/1AHs9qy9nHqp3SeR3rMKkml2pesY6Vzr+1fKwbtG3bNidPP8vz6Dp16jh5OvdlzUJt/+nTpztpnhuzXwfcOYL2m5UrVzpp9qtaPrW5TO/evZ30E0884aRZn7ZevXpOnrY/93vtN2pXuf217suUKeOk2V8vXrzYyeP+qv1a54CtWrXyj6dNm+bkqZ4hz0X0Oah169ZOmrWqQjbGfETKSbcvpQzDMNIr9uuGYRiGEYStlDIMwzAiYc8SLvZSyjAMI5WYIzEMwzCCsJdShmEYRiTsWcLFXkoZhmGkEnMkhmEYRhD2UsowDMOIhD1LuPwlXkpxnKjqdATpF2jcqsZds4aC6sjwdVW3SmOGWfNBNQlYkwkI1p/SGGLueBoPqzGqHCes5VPdKK5PPVf1NVizQu+NUT0NjQNn7SJtl9y5c0csL8cwJ3Vd1k/Sgap6Klx+1VJSTRfVDGC432h5VQeD21vLrnW2a9cu/1j1nDSmnetQr6taBNzeWteq78X9gfU9NE+vqzoyqvnBZdL6Y40P7WP6nUlpeoRQbS0eIzqGVeuN6zB03cTERETCHEn6IHPmzH5bcqy/6vBov58/f75/rHaXdSgAdwyrv2EtBO1/an/Y5ui4Uz/BOkyqEac6QpyvOlFapvXr1/vHqheivpU/q3p9Wn4e02oLWP+iYsWKTp7aXa5ftQXLli1z0qwbpPp8Wg+MjmttJ27/DRs2OHlapsaNG/vHWn9Llixx0qxDUrNmTSeP65p1bwBXr0avq/oW6uv5uu+9956TpzpRbJ9UH0S1v1j7pEqVKk6e+lauM9Uz0TT7Ne2f8+bN849VB07HN+t6qJ9V/8P9U/U3Vf+QfWKoH+l8hrGXUpeeokWL+v5/06ZN/t+1D6mt/O233/xj1WpTnRsedzp3Y9vE9hcIt5WMjiPVquJnFrUROl/kfqvaVGpvuF6++uorJ++mm25y0uw71SeobWI/xfpNgDuG9FlMbSWP140bNzp56qfYz6vd1/vm79W6Z/0hwPVb6nv02YHrSPVpVY+P61B1jh588EH/eMqUKU6e2nL2W9o31OZyGVRvj7V1AVe7Ub9T51zcxrVq1XLydF4/adIk/7hRo0ZOns7zuf1V14rHk7aDaiiybVdfo+3C96bl4+c2wK3D0HO7+k/GniVc/hIvpQzDMNIT5kgMwzCMIOyllGEYhhEJe5ZwsZdShmEYqcQciWEYhhGEvZQyDMMwImHPEi7p9qVUhgwZ/CV1HHqjW53qsjteIqrLtoOWyuqSW16Oqx1At4flpX661FC3fuYlgzly5HDydPkjl0HDHDRki8uoS3c1TJCvpUvPdeks14sux+VQNQ5NSOo7edmqthmHwOhntY60DTWchtEy8b0lF/bA52roly5/5nxd0sohZBo2oP2Tw1F0WbK2KfcVXYauS0U5rUvUtc9x3Wvf0DJs377dP9b+qPXJ9a3jicM7dPm1Xoe/R/M0zIn7jm6hq2EZXA+h+rLwvfTPb7/95vcJtg3adhqGxUvYkwsZ5XbTbYY5JFxDfzRcnPunjsOg62o/1zCOpUuX+sfazzUcm9Gxr3aNw7I0LLlYsWJOmpfKq91gm7h27Vonb/ny5U6al/mXLFnSyVu9erWT5jA29SnqdzmEQf23hu+xnVabF/Q92ufq1q3rpNmn6DyG8z744AMnT9uQwws5xAgIr08uk/oF7edsE7V9ta9wKIR+p86B2Eerz+OttgG3n2koCaNbdmvoUHx8vH+soTh6Lof+aRvydQC3vkO+Sn0fYy+lLj1LlizxbSj3P51baqha/fr1/WO1GepPeH6rc1+2oxoOpd/J5y5cuNDJU1vEPkNDukuXLu2kuc9r+dQW8feUKlXKyfvhhx+ctIZEMWq/+V5Xrlzp5PG4V9/41FNPOWn2f5UrV3by1B5ySPXcuXOdPLXP/LzAc3EA+Pzzz500yz+ojdBnFPbfGlK2bds2J83++4EHHnDy2E9p+OjXX3/tpP/1r3/5xx999JGTN3XqVCfdvn17/5jD6IDwOuKwbq1rtfscfqhzrJkzZzppDuvXebz2Qa4zteXsazScXmUa2Ocm14Z83RkzZjh56tMqVKjgH4fmcRczxDv0mb8r0cmfYhiGYRiGYRiGYRiGYRgXl1S9lBo0aBCioqKcfyzA/ccff6BXr17InTs3smfPjg4dOoT9SmUYhvFXJ/TrRmr//RMwP2EYhnF+fuKfgPkIwzAMe5ZQUr1SqkKFCti7d6//b9GiRX7efffdh8mTJ2PChAn46quvsGfPHlx//fUXtcCGYRiXGnMkwZifMAzjn475iMiYjzAM45+OPUu4pFpTKmPGjGGxmcA5HYZ33nkH48aNQ5MmTQAAo0aNQrly5bB06VJcc801qfqezJkz+/oNHLOvMf+qocE6BKqDoJ/lczUulOOLVdtAY2n5s6r9pLG0rOug5dMYWI55V10R1TniTqrXUR0M1gLSeF09l8ur8dAcm65bMmusL8fv6rlaXo5N1thevW/+rMYiq4YG6xXptu+qC8H6Kqqzpe3PMfCsIQW4scSqCaDncl/RPqf1yfWi56pWApdP60THJWuvqFaV1hHH1asmm+qVMFp/PA50u1rV4eIxrLpgqiPDWgl63zqe+NxQferYVf7OjuFCSSs/kSNHDr8fsq6G6lmobgZrUaguhvoUtiuqCcJjQvv14sWLnTTbAtWfUk0Q7q+qIaXbinM//Omnn5w81XlgW6G6QTrWWO9HNRFUh+nHH3/0j1UDietTbalup802UW2e6lqxvoWO727dujlp9hvq83bu3OmkWT9Cy6v2ietFtVqCNLFU75B1KbU8uu01+ybVnalRo4aT5r6jflb1Ydj2qx6azms4rX5N64z7Bh8DQOPGjZ009+UdO3Y4eTz/0PbWeQuPRfWHCtenzjfUR3MZQvWp362Yn0iatPIRMTExvt3juaeO1yD9JP1Otclsz3WezPMvfvEGuDYMcMe6aispbNs7d+7s5PEcH3DHy9ixY528J554wkmz3o/6TX0xyBpEal/Ux1155ZX+sfqwhx9+2D9etmyZk6d6XuynvvnmGyePtYk0X+tE65e/V31NkSJFnHRCQoJ/rHpT6iuDbLBqV7Hd1eu88sor/rHOdQcOHOikWb9L57Hql3gez9poALBixQonzfWrOlaspaSf1fq75ZZbnDTPlbTPtWrVyknznOvTTz918ooWLeofq25Z1apVnXTNmjX94y1btjh52o/4eVHbUPsVz8FC9xKkOwiYj2BSvVJq69atKFSoEIoXL47OnTtj165dAM51gNOnT6NZs2b+uWXLlkWRIkUcQVLDMIy/OvbrRjDmJwzD+KdjPiIy5iMMw/inY88SLqlaKVWrVi2MHj0aZcqUwd69ezF48GDUr18f69evx759+xATExP2q1n+/PkDV02cPHnS+TVKf6U2DMNIb5yPY/g7OxLG/IRhGIbtvhcJ8xGGYRj2LKGkaqVUq1at0LFjR1x11VVISEjA1KlTcejQIXz88cfnXYChQ4ciZ86c/j9dHm8YhpHesF83ImN+wjAMI21WSi1YsADt2rVDoUKFEBUVFbate1LMnz8fVatWRWxsLEqWLInRo0eHnTNixAgUK1YMmTNnRq1atcLCqi4E8xGGYRj2LKGkWlOKueyyy1C6dGl8//33aN68OU6dOoVDhw45v3Ds378/ybjxEAMGDED//v399JEjR1C4cGEcP37cj9Xn2F+NN82fP7+TDvp1RDWHOG5YdXlYV0LjizUWnWN2Y2JinDzVromPj/ePVYdHOxrr52hMqv6KxPem96Kx3dweWiesbQG4cetB+graxqq9wvH5XLdJlTfSdwDhmlJcRxqDredyGbU+tR9xPmtOAOFaLKxDoedyvLZqtmhf5ThxrWvVIOHrasy4XpfLpLHorLMFuBoveq7q03B/VW0YHSPcjqoVE6QDp2mG6wAIrzPOVx0z1T3hOPHQGNZ7YOzXjZTzZ/qJY8eO+TaAtSe0b+h4552cdPyolo3aMoZ1eNSeq8bCpk2b/ONVq1Y5eWrP161b5x+3b9/eydN7Ye230qVLO3mqu8bjQHWsVGePdUi0vOqHuW+rfV+6dGmS1wTg7LgFuPWZnA4D67xs3LjRyfviiy+cdJkyZfzjgwcPOnmqI8QakVpHqkPC7daxY0cnT7+HdTPU7laqVMk/Vn+tWmVc1zfccENg+dg/qp/t1auXk/7www/9Y/Wlel32ZeoXdByzHdVxqfMlnn/od/L4Ur02LQO3t/ZV9d88JnQM85gF3PlcqJ20rpi0WCl17NgxVK5cGd26dUuRGPj27dvRpk0b3H333fjggw8wZ84c3HnnnShYsKCvlTN+/Hj0798fI0eORK1atTB8+HAkJCRg8+bNYXpKF4M/00fkzJnT73dsD3VOpW3P41BXaKldYG037Yv8Mk/7ns5vWGNKr6Of/eijj/xjnd9s3rzZSbNt13HPWneAq/2kunNaD+zjdL6k2nis6aP6vqxfqD5Cdbfatm3rH2tf1JeabE9q1arl5OnLW/Yn+uwwY8YMJ81lVB+rfotths4J9PnwjTfe8I+bNm3q5LEWlOrk6fx77dq1/rHqN6nNZf+sWkqqHcm+qE6dOk6e6gWyP1RNqZEjRzppDtXl/ge4+liA28/atWvn5E2dOtU/vvnmm5081ZjiOYKWXXW32N8ltwso66WF2vBi+ojQZ/6upFpTijl69Ci2bduGggULolq1asiUKRPmzJnj52/evBm7du1C7dq1I14jNjYWcXFxzj/DMAzj74H5CcMwjD+HVq1a4cknn8R1112XovNHjhyJ+Ph4/O9//0O5cuXQu3dv3HDDDRg2bJh/zosvvoju3buja9euKF++PEaOHImsWbPi3Xff/VPuwXyEYRiGkaqVUv/973/Rrl07FC1aFHv27MHjjz+ODBky4Oabb0bOnDlxxx13oH///siVKxfi4uLQp08f1K5dO9W7ZRiGYaRn7NeNyJifMAzDOP+VUkntKh20ojw1LFmyxFmZAJzbTaxfv34Azq0iXrlyJQYMGODnR0dHo1mzZhdNaNx8hGEYhj1LKKl6KfXTTz/h5ptvxi+//IK8efOiXr16WLp0qb+N5bBhwxAdHY0OHTrg5MmTSEhIwGuvvXZeBePlnRxqo0sPNVyKHbcuq9SlsrwkT5fI8xJ+XWqqy3x5uaYu09PtI3n5sZ6rS9s5tC4oHApwO6nep3ZgrjNdPqqhA7x8U8NauF50+aMus+Z7Cwr9ANyQCF1iraE2HHrB24EmBS+71HYJ7fwSgpfH6lJeLS9PILVv8K91Gs6h4Wa8Nb2GwGjf4O1W9RdBbX/uO7o0WkPpuC/rWNP+ysuztT9qOCQv+9br8jL15EIwuV60PrXO+N70O/Vcvu9Qn9Jxz5gjiUxa+4lQO7EN1/7I9hxw+46ey9tyh74jhNo5thNVqlRx8jisDnDHcHJ+jO2Thg6oneOxVrduXSdPQx/YnmoIK4fOAa5vUP+jtou3U9dzeZtrHXda92wLtE6uvvrqiOXVUGO1a7xtt4agtGnTJuJ1OYwSCN82nu9t4sSJTp76GPZr6ktZ/yYkWxBCw77ZB+oW3ho6wuWbPHmyk6ef5VUo7IuAcL+2bdu2iOUNCvVTG6gvWvhcDUli36V1q23K962+U8M1GfUpGg7L3xMKkQoKMz3fl1Kqh/T4449j0KBBKb5OEPv27Qvzz/nz58eRI0dw4sQJ/Pbbbzh79myS56iNOF/S0kds2rTJ72fcF3TOr+FS8+bN8481/KhGjRpOmutK577cPzSsTudj3P80RGv+/PlOmvuIzpsKFizopHmMBo0VAJg1a5Z/rGHlulKuUaNG/rE+SygcClutWjUnj9uicuXKTt6WLVuc9OzZsyN+R+PGjZ30tGnT/GOtT50TsG/U0D6toylTpvjHGjqu7c+fVdujL5/5pavaXPZx6gu1L3Oo4jfffOPkBc0f1HePHz/eSXN/aNKkiZOnz1BsozVEVH0P9zmWuAHC/QuXX5/xue9oiPxPP/3kpLk/6ApMDhEF3HmUtmFQSH8o9FDnS4w9S7ik6qUUxzAnRebMmTFixAiMGDHiggplGIaRnjFHEhnzE4ZhGOf/UurHH390HnYu1iqp9IL5CMMwDHuWUC5I6NwwDOOfiDkSwzAMI4jzfSn1Z2oiFShQIEysd//+/YiLi0OWLFmQIUMGZMiQIclzgoTGDcMwjNRhzxIuFyR0bhiG8U/EtnE1DMMwgkiPPqJ27dqOiDhwLnwmFMISExODatWqOeckJiZizpw5gULjhmEYRuqwZwmXdLtSKlOmTH4sKceGajysxgVzvKdqwrBGE+DGzwbFQ2u8ruoZ8Hdq3LLqYnDcsupr6K9QHG+sMbj6PbyNpn6nwrodql2g+hUc867nsiaJxiKrngpv3ao6DarJwDHE+p06GLktdAtajbNnfSzN037EW8lqnWiMMy+t1xhxLpPqYWl/5P6gv5Kq/gvHqWsdsd4H4Nav6muoRgr/Oqqx8nny5HHSXPeqxaE6AFx+1SlgjTHVglGNM64j3TJZP8vtonlaD6zDFerLpimV/ilcuLDfD3isaXurjgbrM/D28UD4lr+8PbDqFLAd1u3jdWyxnghv0Q0Ea4uofdS+y2OEteaAcC2UBQsW+Me6nbZq/bGd1q2hVetv+/bt/rFqTfC24qpJo3XNtkz15PRBukSJEv6x6jxo/bJOhZZB7Sf7BtWOUT/M56puhOqGlS1b1j9WX8DtzVunA+G+gO2a3veGDRucNPcdbRfVLOFt2bVvqE/hute5k/pSbkcdh+pTeItvFdXmOqtUqZKTp+3N8xHVgVP/zajd0Prl9g5pyF3M7b7Px0ccPXrU0TzZvn071qxZg1y5cqFIkSIYMGAAdu/ejffeew8AcPfdd+PVV1/FAw88gG7dumHu3Ln4+OOPHZ2c/v37o0uXLqhevTpq1qyJ4cOH49ixY+jatWuqy3epKVasmG8zee7BczwgfM7CW97rXE218HgM6DyUNQp1zKk+EttK9R/abytWrOgfq1YVaz0BwIQJE/zj7t27O3lLly510sWLF/ePVZOwd+/eTpp9D/sAILzO2GbofbOukWr/qH1R/UBG55YtWrTwj1WTjW0N4M7zd+/e7eSxRhMALFy40D9WvSm1TaxzpPWp31OzZk3/ePr06U4e20rtR9xvALeOtE7UrrJvV9ut99a8eXP/WJ8PVAuKyz9w4EAnb9GiRU66fPny/rFq2a1cudJJd+7c2T/+8MMPnTyes7/11ltO3kMPPeSkFy9e7B9rOyxfvtxJsx/g+SAQPu9j/xwas0E+x54lXNLtSynDMIz0ijkSwzAMI4i0eCm1YsUKR+C5f//+AIAuXbpg9OjR2Lt3ryNCHB8fjylTpuC+++7DSy+9hCuvvBJvv/02EhIS/HNuuukmHDx4EAMHDsS+fftQpUoVTJ8+PeyB0TAMwzh/7FnCxcL3DMMwUklaLrkdMWIEihUrhsyZM6NWrVpYtmxZ4PkTJkxA2bJlkTlzZlSqVAlTp04NO2fTpk249tprkTNnTmTLlg01atQI2z3FMAzDOH/Swkc0atQoyeuMHj0aADB69OiwndsaNWqE1atX4+TJk9i2bRtuv/32sOv27t0bO3fuxMmTJ/HNN9+ErRYxDMMwLgwL33NJtyuleBkeL1vUXUh0S0heMq8hERoCxQ2rS+R5GaOGpmnIAS+P1PJoiBGHAupyR106zp/V62qYGIcGaIijlp/rQetTQwh5CS6HOAHufesSWw054XvRutZQBg4N0TyFl60mV/e8bFVDK3SLVV7+yqGR+p2AWy9B4T3JhXdwu2nIqC6j5e2yNZRTlwhzmJ2Gw2nf4H6vv4rqcmxekqptqt/Dn9Wl79wfdYzqd3KYi9afhtVyOJKG4mlbcEhUqD2DwvfSivHjx6N///4YOXIkatWqheHDhyMhIQGbN28OC7EBzi1JvvnmmzF06FC0bdsW48aNQ/v27bFq1Sp/uf+2bdtQr1493HHHHRg8eDDi4uKwYcOGZLd0To9kypTJ7we8pF1DtLQv8zjVcAA9d8eOHf6xLt3m/qkhrBrGwTZG+66Ob/YFHE4BhIcT8/hXexm0xF7vRcNXeHzrsn71rbx1tNYDf891113n5HHImJZfQ1LUX3IomIbZ6dhlLZxrr73WyVN73qlTJ/947ty5Tp6GqLAfVp9cv359J81hXnoul5f7GxDux7iddMxqv+e61xCCdevWOWn2nyoBsHfvXifN/l3nG2rfOfRB/YS+YOf5iIZVcp/TsmvIDNenfieHEQHuGFa/q7aA6zDkZ3UsGOmLEydO+HN97os6j9eQKO6bKrWh8we2TXfffbeTx2FCfAyE2+By5cpFPFdfCvIY0NBcvTfOHzNmjJOn9oWfiwoWLOjkrV+/3knzD1k6/9J5KdtODanlZzz9DpX74LBFDe1Sn8HPEt26dXPyNEyQwyz5O4BwW8Qhb9dcc42T9+qrrzrpWbNm+cdqV3keDwAzZ870j9W2c1/R66h/5pAyDo0DwufYHF6tdaIh9Bziq8+DWt5bb73VP9Z20vvmOYOGQ7dt29ZJr1692j9WyQH2PTq29FmnWLFi/rHOkzTMnOtbXwhpSD9L14T6kfmIlGMrpQzDMFJJWv268eKLL6J79+7o2rUrypcvj5EjRyJr1qx49913kzz/pZdeQsuWLXH//fejXLlyeOKJJ1C1alVnovTII4+gdevWeO6553D11VejRIkSuPbaa5N8yWUYhmGcH/YLuGEYhhGJtHiWWLBgAdq1a4dChQohKioKkyZNCjsnueiJP/74A7169ULu3LmRPXt2dOjQIezl965du9CmTRtkzZoV+fLlw/333x+my5gc9lLKMAwjlaSFIzl16hRWrlyJZs2a+X+Ljo5Gs2bNwsQqQyxZssQ5HwASEhL88xMTEzFlyhSULl0aCQkJyJcvH2rVqpWkkzIMwzDOH3spZRiGYUQiLZ4ljh07hsqVK2PEiBFJ5oeiJ8qWLYv58+dj7dq1eOyxx5zVb/fddx8mT56MCRMm4KuvvsKePXtw/fXX+/lnz55FmzZtcOrUKSxevBhjxozB6NGjw0TukyPdhu8ZhmGkV87HMYTO19Cd2NjYsDBa4NzuQGfPng0LIcmfP39YmE6Iffv2JXl+aDnygQMHcPToUTzzzDN48skn8eyzz2L69Om4/vrrMW/ePDRs2DBV92QYhmEkTWr9hL2UMgzD+OdwIc8SKaVVq1Zo1apVxHyOngjBYe6HDx/GO++8g3HjxvmhwKNGjUK5cuWwdOlSXHPNNZg5cyY2btyI2bNnI3/+/KhSpQqeeOIJPPjggxg0aFCYZEUk0u1LqRMnTvj6Ehzrrdu4aswrP/Bpw+lW2qwfoBoUvEWk6uOo/gd/VrfKVrhMGg+rMdkct67blqv+FH+vxsNqzHiQTpM+HPP3ah7HJqsWg24hzvHHWh6te36oXrt2rZOnW3eyDobqWKmWBPcdjicGwnWYWCdDrxsUS633zXmqtaLtxLodqnuhnw3qR3rfPH5UV0SXX3I7qm6C9hvWutEy6HVZX0B1oriOtK6DxoiOAY2V53P1vrXP8feGjGeQptSFOBLVJ3j88cfDtiv+swjd07/+9S/cd999AM5tbb548WKMHDnyL/dSKnPmzH7/YZ0otdG6hJjTqm+h9p7H09atW528IN0l1gcB3L6sY0v18IoUKZLkdwDhY4TtmtoJ1UlhvSLV0lKbyDt6zZkzx8nTF5884VHBfNZjueqqq5w8HUOsJ8H6FUB4fbL+odoC1bfg+lWNDdW3UN2ooDzWsFB7oZpiXN9B/lupXr26k2Zbqt+pKyjZ1laoUMHJU50orge1parVwv1Ky6BzAZ6TqZ9VLTCuIx0TXEeqsxY0t1NtG9VOY1uhcxPV9+I6Ct2XjkfGXkpdenLnzu33D+7z+pCmdovHet26dZ28adOmOemqVav6xzq/Yc061R9SPTYeH9oXdS7E84i3337bydM+zxpJ+syk87qFCxf6xz169HDydM760EMP+cdqr9XHsaaizpNZ5+qBBx5w8lijR79H7YlqInH9ql4u+1jA1Y5VnUHdKKB3797+sT5s63MSaxlVqVLFydN64H61fPlyJ491me69914nb8KECU6afa5qKQXNhdq1a+fkDRs2zEnzOND+qfMo1ovU71QdJvY3rFUMhPsetvU6Z2FNrvbt2zt5qg/JZVD9Ke1HXH6dw+izDveH0Heov2fS4gfuIELREw888AASEhKwevVqxMfHY8CAAX4drly5EqdPn3aiMMqWLYsiRYpgyZIluOaaa7BkyRJUqlTJmRsmJCSgZ8+e2LBhQ5hucyQsfM8wDCOVXMiS2x9//BGHDx/2/w0YMCDJ78iTJw8yZMgQ5vT2798fNsEKUaBAgcDz8+TJg4wZM4Y9mJcrV8523zMMw7iIWPieYRiGEYkLeZYoXLgwcubM6f8bOnRoqr+foydatmyJmTNn4rrrrsP111+Pr776CsC5l9ExMTFhLww5CiNSlEYoL6Wk25VShmEY6ZnzfYCIi4sLW82WFDExMahWrRrmzJnj/2KRmJiIOXPmOL/UMbVr18acOXPQr18//2+zZs3ydx+LiYlBjRo1wn592rJlS9ivtoZhGMaFYS+aDMMwjEicr4/48ccfnWeJ1K6SAtJf9IS9lDIMw0glaREHDgD9+/dHly5dUL16ddSsWRPDhw/HsWPH0LVrVwDAbbfdhiuuuML/heTee+9Fw4YN8b///Q9t2rTBRx99hBUrVuDNN9/0r3n//ffjpptuQoMGDdC4cWNMnz4dkydPDluibhiGYZw/Fr5nGIZhROJCniVS+gN3EEHRE4sWLQJwLgLj1KlTOHTokLNaiqMwChQogGXLljnXCEVtRIrsSIp0+1IqKirK19LgmGKO+wXC42WD9JK04fmtosa8sm6QahuophBrKmj5NN6Y9UpUK0TjQzlmVzUe9L4ZjifW8gFuPei5GuPM2g2snwG4cbKqZaKhQHny5PGPq1Wr5uSpTgcPMo0Z1uWB/FmtI/5OwI0h176guhDcN/TeVNeMY5xVy4TrSI2HnsvtpDHIOqi53VT3QpdKnjhxwj9W/RQ9l8uo/Vx1T1j/RbVrtF+tW7cuYhm47rV9NRSN20V/FdBzedyqfo6Wj9swlBekKZVW3HTTTTh48CAGDhyIffv2oUqVKpg+fbpfT7t27XLsSJ06dTBu3Dg8+uijePjhh1GqVClMmjTJ0ZS47rrrMHLkSAwdOhR9+/ZFmTJlMHHiRNSrVy/N7+9COXz4sG+XWNNJbavq57C+jmpIabvztXgsAa7f0DGq4501QbT/7dmzx0mz/dQl02rX+HtVa0dtA49T9ZWqEfHZZ5/5x+rXVq1a5aS5DlULg/2a2lnV/mIBf9VAUjtcunRp/1jtmGrycZuGJlohtM5YU0XrKD4+3klz/Wqbqr3k/CBdF9XO0jkE2yrVVNHy8urHfPnyOXmq6xFaTQkAH330UeC5lStX9o+1TlasWOGkue5VF0fbomDBgv6x6kRxnfF5ALBhw4aI5dOxpdpv3Cd1DGt96vg30j9nzpzx7TTbEJ1jqS3icTdv3jwnT+3hJ5984h+zlg5wzieH0Dn+jBkznDTPU7SPq84Rl1/HZ9++fZ0066hp/9cHydtuu80/Vn04LcOHH37oH+t8UZ8lNm3a5B8vXbrUyWNbr89iqgHHdiE5fR/2A/qcoXafy6Q2TB/Y+Vy+LyB87sH6XqVKlXLyFi9e7KTZP996661OHteD/oBYqVIlJ83+mPsmEF6/rPWzZs2aiHmAq+mrK2hUb5P9Xf369Z087jeA25f1Ojov4Wc3fY7r2LGjf6y+Ru+N+5HaAr0u6zrq/FCfUfm+Q2NCx0Z6IiXRE9WqVUOmTJkwZ84cdOjQAcA5ra9du3b584batWvjqaeewoEDB/y5xqxZsxAXFxc2foJIvzVlGIaRTkmrlVLAOVHNSOF6Sa1u6tixo+Ock6Jbt27o1q3beZXHMAzDSB5bKWUYhmFEIi2eJY4ePer8gLV9+3asWbMGuXLlQpEiRZKNnsiZMyfuuOMO9O/fH7ly5UJcXBz69OmD2rVr+5s3tGjRAuXLl8ett96K5557Dvv27cOjjz6KXr16pSqs0F5KGYZhpJK0fCllGIZh/PWwl1KGYRhGJNLiWWLFihXObsr9+/cHAHTp0gWjR49OUfTEsGHDEB0djQ4dOuDkyZNISEjAa6+95udnyJABX375JXr27InatWsjW7Zs6NKlC4YMGZKqsqbbl1I5cuQIWwYJhIdhaOgFh5jp5zXNy+x0G1de6s5hSkldh5eV69I+DeHg5bm6vF9D8vizeq4uaeS0hhFoHWma0c/ycli9F17eHLQkHnC3r9Ul8Bqewm2o98nXAdz61m1wtS24DjUUREPpeHtTNQAqCM3LYbWvcOipbm2r1+Ul2FqfGtbGy6i133BYC+AuTQ3arl3LpOGa2k5cnxqOovDyTd0qncMug8YW4C4n1zbT9ue+o+NH742vFToOCpG1l1LpAw7NYDRcU0OieLtq7Y/ar7gPapgEh1isXr3aydMl2zzWtm3bFngu21YdzxqOxLZK+6yGfvHWx3qujhG+Vw1ZVj/M21Xrdfk6ah81DIbbjUP5AKBMmTJO+ptvvvGPNVxP/QaHbmh4oYZscXix+htNc1/RMui28XyvGm7GYR3aVzUEk33y9OnTnTz9LNe3ho5wSDUAfPHFF/6x9hsOhwPcfq92TUPe2KZrSI+GXfK8IUiygNseCG9Drl8NLdewDkbHlvZzDmcJlS8opM9eSl16Nm/e7P9Sz7ZIw8J0Tti0aVP/WP3JnDlznHRI4xFww54B1y906tTJyVuyZImTLlu2rH+sYWEazsdoaJruwsU+onPnzk7etdde66RnzpzpH9esWdPJ0/kil1Ft+dSpU500h0fWqlXLyeP5LpcVAOrWreuk2a6q39RQYvazGmZ14MABJ83l17BADX3mMDadS2od8Wp2DX/UOmNpEw27Y1uu96mhp6Fd0wDX5wPhPozrm0NNgfBQOra7avc03J7rSPu5zqP42UjHpYYxjhkzxj/u2bOnk8eSHTof6969u5PmOY32I53DcDinhjTqvIl9WpUqVZK8HpMWzxKNGjVK9jPJRU9kzpwZI0aMwIgRIyKeU7Ro0bBxn1rS7UspwzCM9Iq9lDIMwzCCsJdShmEYRiTsWcLFXkoZhmGkEnMkhmEYRhD2UsowDMOIhD1LuNhLKcMwjFRijsQwDMMIwl5KGYZhGJGwZwmXdPtS6siRI742AetDBOnaAO522aprpGm+lmpdcGyqailpLC3rSmhsqn4nf49qHqkOBsfZcqwxEL6FJccxa+y5xjzzZ3mreCA89jXo3nhgqOaRaqbw9puqFRIUKx+k/wC4ehXaF7TduO5Vh+ann35y0ocPH/aPWWMECNcuYn0a/hzg6n/o51S3g7VtVP9D9Q54a2HdBld3OuA21O3kuZ8Dro6Hbges7c+x6XpuUD/S8vF40nsJMr5qC1SfJCmtoRDaFtw3Qu2p41PLZY7k0pM7d25ky5YNgNveqrGhNobHj+YF2WzV4+PvqVq1qpO3fv16J83aVGrrtd+zhoWOUR3DnJ4wYULE6wCujkJI7yCEaphwGVXrjQUwAWDUqFH+sfomLoNq/6xdu9ZJs6aP6smp9hdr+6n9Vr0k1uBQu6s6QlzfWr4uXbo46ebNm/vHqoGk/odtoLYLa+4lpwvGekmqD6L+kq/19ddfO3mqQ8Lfo/5b2437io4f1VThcal6baqBxWKsq1atcvJYG0p1HfVcHt/aH7Vf8dxEfYr6kG+//dY/DvkHtReMvZS69Pz6669+3+a+qRpwqpu2YMEC/1j7gWrisC1lzRvA1eVRLbnQzlUheM6vc5TixYtHPFfnqKqjxlpuEydOdPJUs4f7sz7r6G6/fN+qJadaRjzOJk2a5OSxXmCjRo2cPK17noeq5pWWl8c+tycQrl3VpEkT/1jnqGpf2E6oLVcNSJ4XqHax+jT+3vbt2zt53N6qeaUae/wspPq0bMMAVy9t4cKFgeVjzal58+Y5eVr37BfUF27evNlJt27d2j/WeTc/XwFAq1at/GNtU/ajWkc6J7jnnnv8Y60/bX9Oq76cPvvyHCv0HBf0HGvPEi7hSuKGYRiGYRiGYRiGYRiG8SeTbldKGYZhpFfs1w3DMAwjCFspZRiGYUTCniVc7KWUYRhGKjFHYhiGYQRhL6UMwzCMSNizhEu6fSmVmJgYFqMMhOsrhPREQnAMscb6a5w152vcMut0aIyraijwdVUPQsvAOg4aZxqkXRSkWwC4mj6q6aB6EJyvelOsxaDnqg4KxxtrzLCeu3v3bv9YY49Vi4N1MrRdNJ6X61Pjn1VLgttGtSxUU4x1JzRPdWW4jjRmnOtB21BjkTkGX7WpgmLPtTyqmbFjxw7/WLVh9N64zooUKeLkaV8J0mzSNt61a5d/rOOJ49+17KpjxXH1HLsNhNsCth/ab/Re2MiHrpOYmBim5cXnmyO59Hz33Xe+VgXbYdavAML7PetzbNmyxckL0ohQXR4e36rJxH0VcO2Ejm/Vw2Obrf1c742/9+qrr3by9F54XH7//fdOnvpb1txQv6b3xpqH6n/Yr40ePdrJu/baa520agUxNWrUcNJsK1RTSv0Y35v6XdXDY3taqVIlJ0/nHzNnzvSPtY7UdnEZGzZs6ORxO6nfUtvP/lF19Jo1a+akWStD7Y/6bNYaUW0l1SXZu3evf6z+W30r9+WlS5c6efpZ1vBS/6N9jtG5E9+b2nrV0uL213NVW4TbNKRTpj6UsZdSl57ExER/zsGaODwvAoAvv/zSSVeoUME/1r6nukHvvfeef6x2ittUNeCGDBnipG+55Rb/WOeHquHTrl07//jDDz908lTziu2N9v8DBw44adZASk4nim2a2jstA/setausoap6dqwTpOdq2fU72abpc5DqOPL8Qe2dXpfnDDr/njNnjpNmPS8tr85LWHNM/UmtWrX8Y9VH0mfS66+/3j9WG7Z69WonzXpOb7/9tpOn98b6i6qhqbacfZPaNe67gOuvdQ6gaZ6TB83V5s6d6+SpnuErr7yS5DWBcP+8YsUK/1h9rN4bX+uRRx4BEO5X9PP2LPH/pNuXUoZhGOkVcySGYRhGEPZSyjAMw4iEPUu4XJDQ+TPPPIOoqCj069fP/9sff/yBXr16IXfu3MiePTs6dOgQ9kbaMAzjr0zIkaT23z8N8xGGYfxTMR+RMsxPGIbxT8SeJVzOe6XU8uXL8cYbb4Rtu3jfffdhypQpmDBhAnLmzInevXvj+uuvDwt7SI6YmBh/aSMv09cQKG0cDm3QpacaUsTn6lJJDp3T6+jyf14WqMs+tXy83bQuq9Rl+7ycVMuuS3A5dCm5LZB56b1uh63n8tJ0rSNeRqtbZ/MWr4C7dFa3ONd74xA4/U4OAwPcJf663F/P5VAb/U4NN9SlyIyGe3Aoji5h5WWbunxUw99WrlzpH2s4j4aecntrOI8uFeUlw8mFWUYKVwPCQyQ4lIX7FBAensTLlLX+uI9peIzWJ9ehji1Ncx3qWNNl09zvQ0uJNcxQv8t+3Qjmz/YRwLm+H+r/3Fe0rr/77jsnzUvC1Z7r2Ofrar+58sor/WPd5lj7Lts9DSfl6wBu6IbaDbWffG8adqX9nv2n2hRNs99L7ly2/7p1OdsnvW+1gbxMXkNmNISCQxY0xFHrLKltmkOozeH+oOXVkEe2n1peDQvl79W+wWEb27dvd/L0XrhM2m90O3Wue+3Xug02+wataw2N5hDNUBhbCL1vDgPVEBr1G9wfNBSey6ehV3pv7Ks0tFNR/8no/IPHV8jPXszQjH+ajwD+fD+RJ08e3w5ySE9QmCkAVKlSxT/+4YcfnDwdOzwe9BmF5xHPPPOMk/foo486af4eDYPu0KGDk16wYIF/fM011zh5+vJu1qxZ/rE+O2iY4Pr16/1jDssGgJo1a0a8rt63jl/+HrXBJ0+e9I853A1wfQLg2lkNs9q4caOTZvuszwcagslhdxpm2aJFCyfN88UpU6Y4efzsCLi2VOcPQXME9d18b2o32cbqdTjsDwh/RuUQ9OrVqzt5+nzA38OhpgAwadIkJ83+mfsJEB4WyM8L2nc1fJ3rXp8zuQzqR1u2bOmkeRyw/wXc/ggAnTp18o+1XZYvX+6kOT8kT3D8+HFMnDgRSWHPEi7ntVLq6NGj6Ny5M9566y1ncnr48GG88847ePHFF9GkSRNUq1YNo0aNwuLFi8O0BAzDMP6q2K8bwZiPMAzjn475iGDMTxiG8U/GniVczuulVK9evdCmTZswwa+VK1fi9OnTzt/Lli2LIkWKYMmSJUle6+TJkzhy5IjzzzAMIz1jjiSYi+kjAPMThmH89TAfEYw9SxiG8U/GniVcUh2+99FHH2HVqlVhS9aAc2r7MTExYSEE+fPnD9slJsTQoUMxePDg1BbDMAzDSIdcbB8BmJ8wDMP4O2HPEoZhGAaTqpdSP/74I+69917MmjUrTOfgfBkwYAD69+/vp48cOYLChQsjOjraj7/luH6NwdW4a0bjdzXNmhkaB8xvIvU7NN6UNSlUk0fjT1lvQ52r6iKwNpReR+O1WaencuXKTp7+YsSx86ohpWVgvR/dfpNjfcuWLevk6WSCt3nVsufJk8dJcwy5apdo3D9fV9tQ24lRHRmNs+b+rWVQ7RDVGYl0HdWe0K2k+d6S007jMaH6U1q//Fn9Tu3bXIfaF1R/jGPGNQY/qM60DFz3qjelGlg8vrQNtS/zeA/SnlPUTiSFxYEnzZ/hI4DIfiImJsa3jTy+gvTvAKBYsWL+seoGqe1iP6E6BWzDVZtI7W69evX8Y9YDAcJtF2v46LhT/STeXlu18tRms//U71TfyuNAt+VWjRXeap3rFoATbqPaRIsXL3bS3GdUW0S1i1gHQm2V+tY1a9b4x6qLotdlDRh9YNYtvbm8et2gfqQ+L0gDSb+T20LrWrVG2I+orpr6Mdal0b6hY4THmmqpqQ1nvbGKFSs6eaojxGNItW9Yq0p1PtW3cnvrd6jtZ9+l26WrriB/b8h3qq9mTFMqadLyWeL06dO+LeNt7HX+oH6f5ynaF7UPsY3WeSfrMiUkJDh5QXo0qtOq+nHt2rXzjz/88EMnT/WyWBtI7Yn6Ex5nOpZVE2vhwoX+cUg/J8T48eOdNGsF6Rz17rvv9o9Z9wsI93+s0aS2sm3btk563LhxEc/V+uQ21jz9LNtD9Y1bt2510qzvpLqsqo3H/lE1r7iddK6htr1Nmzb+sT6TVqhQwUlzf9i0aZOTp8913G4fffSRk7dq1Sonfc899/jHOjdnHSvAna81bdrUyRs+fLiTHjJkiH+s+nJ8nc6dOzt53FcBd26kz9c8nwFc3bAaNWo4eWo3eN63bNkyAMHPovYs4ZKql1IrV67EgQMHHMN+9uxZLFiwAK+++ipmzJiBU6dO4dChQ86EbP/+/WEvE0LExsaGdQjDMIz0zt/ZMZwvf4aPAMxPGIbx18T8RDj2LGEYhnEO8xH/T6peSjVt2hTr1q1z/ta1a1eULVsWDz74IAoXLoxMmTJhzpw5/k4Rmzdvxq5du1C7du2LV2rDMIxLiP26kTTmIwzDMM5hK6WSxvyEYRiGPUsoqXoplSNHjrDl19myZUPu3Ln9v99xxx3o378/cuXKhbi4OPTp0we1a9cO27LUMAzjr4o5kqQxH2EYhnEOeymVNOYnDMMw7FlCSbXQeXIMGzYM0dHR6NChA06ePImEhAS89tprqb7OmTNn/FhN1snQOHBdrssaAKorovo0rAXwf+2de7yOVf7+L4dQU5lkIiJCDjkfQ1GSjU6k84H6+tVUVDIznb5FpxmZvonKpJrpzDAd6Ky0lUPOW5IUHZRSVFNoVMjevz+8njXXup793NtG2xPX+/Xyaq3W89zPutfh81n3vdfnWhojztoBqtmjcLlqeuh1Od5YdTBUg4JjillfCth6ZC6jMe+Mxm9zfCvHOwPpWkDcRvobHB+t2iWqdcEx2HovSXHWqjeg9eO4f/2s/g7H+mrbax04flt1UBTuN21rru+qVauiMr3uzz//XOj3gHSNFB5Xei+6vZ3rpMaM4/yB+F6qVKkSlenvcF7bWvVKOG5d5zCPDW4DrTsQa2DpfNb5w3NRNcMUnsOp31DdEsaOZPvZWT4C2DpeUnoyrFugfkE1Inh8qq6DPiyxvWRtDiCe0zqf69evH+V5zrIuBpA+zpN0zdQ2sGbEZ599FpXp73AddKeC6gjxPNW5oH6N9QXVTuTl5YU0ayoC6XpEbI9at24dlaluHWtBqS6K9hP7XfWdahtYR0V1rdQHsq6VrhNq1qyZsU6qQ8g2W/VgVBOE/Zzed/PmzaO8akwxqoHF7a1rJ9aZAeLxqXoZ2p6dOnUKadWHUZ946KGHhrT6FPYTqkuoedaQU1ug98J10nmoui6sYZlaa+qaj/FLqe1nZ/mJHj16BNvM9lHtidot1n1T7btTTz01yrNGoI4htrO6RlU7z+sk1UFUzT/WN1QdWdXP4Wvp2kxtcJ06dUJatXVGjx4d5VlXdOzYsVGZai1xnVhfEYg1e7R+up7l+ar2RO3zgAEDQvr555+PyvR32Oa99NJLUZn6LR4bqg+ofcx+VW2j+gjuC9Vt5DGnmpRqr9muqp6T2lxe5+tzkI6N3r17Z6zfrbfeGuUnTZoU0jp21bafcsopIc1jAUgfR1xfXe+wv1a/pOOI/bWu1e6+++4oz88ddevWjcp0bcl9k+oX1Txk/CwRs8Mvpd54440oX6FCBYwePTrNeBljzO6CHcm2Yx9hjNkT8Uupbcd+whizp+FniZidvlPKGGN2d+xIjDHGJOGXUsYYYzLhZ4mYrH0pVapUqRAywFvfdIutbtPnrflJRzUC8XZwPdaXr6vHIeu2QN4GqNsfdVslh17olj79Hd6aqkeA6pZ03tKoW9m1TtxGuqVR68shErxVF4i3YOok0S3tXH+tDx/frJ/VrbBJIWS6LVVDV3gbq4am6VZeDnvQY+B1izDXV8cGb8fWMt16mhTeo6EhHOamY0FD/bgNNVxTwyw5BEm32Gp4HLenHoOrIXo85vReuH4aQqTjkceZ3rdum+fPJoUBAnEoYMpO7M6Gf3ehXLlyYRzwWFF7uWTJkijPW+51e7jaYR4bGi7F80VDT9VOcBiWHjWvtoFDjDR0Tj+bdLSxhuhx/fVoaD2enMs1DGzp0qVRnttI5ze3r4ZbqE959tlnQ1pDG9QXcBtpCIWG6PF31f/ouoBDtDSUU/3lypUrQ1pDHTREhe9dQz25PTUsWW0p20gOmwTSQyi47Tn0Quuj9Vd/OGfOnCjftGnTjPVTeKxrn2ooHftlHfec17WTtifPET0uXX0r2wr9TQ2dZBuTSquPMtnF1KlTg13kNYyuk6dOnRrlORQoJycnKvv73/8e5VNi7ADwz3/+Myp77733QlrDa9nWAPFY1JAitddPPPFESP/P//xPVHb22WdH+c8//zyk1fd07NgxY50WL14clWn4Gc+XNm3aRGU6z1q0aBHSDzzwQFTGNk3XZhpez2u5/v37R2UcMgbENk3XxQr3t/qabt26RXkOVSyqPbn/9RmlZ8+eUZ79ia5Zub+1H/g5DUiXU2F052GXLl1CWtue7TwALFiwIKT1uWjhwoVRntfPOhbOP//8KM/2Wseu+lX2W7pW45Dc8ePHR2XqVznsTsMLNWyb+0KfbXXdd8EFF4R0qj9//PFHvPzyyzBFk7UvpYwxJlvxXzeMMcYk4Z1SxhhjMuFniRi/lDLGmGJiR2KMMSYJv5QyxhiTCT9LxPillDHGFBM7EmOMMUn4pZQxxphM+FkiJmtfSpUuXTpoQrHWjmqFsGYPEGsSaLypakcwet0knYCk4x1Vk0A1cjhmV4/V1jhm1v9Q7R/9Lg9SPaJStbVY10F1grSN+ChUjbvl7+ox5RoPzfG8WqZtxPeiukuqX6H9xmgcM8fV63V0kvO96pGq2vasoaLaJtyeqnuh7cmodgnXHQAqVaoU0nyEOZCulcD6aFoHHXNcnqSdBsQx+nodjXlnfSquOxDr1ei803htzqvmlcb2c7/pnNX68r2l7jvJ8NuRZAfLly8PeiGsf6B+QbWWWENQx6PqEbGtUFvA+gJqx3Qesm/Qeah6Bzzf1bYeeuihUZ61HdTWq64Rt4vOCdWTYNurmhWqz8G2Ys2aNVEZ/87MmTOjMj3KnDUCX3vttahM/Tm3t2oEqg9kHQrV+lI7zLp7qkekui5NmjQJadULUb1Ltl26TmBfpToejzzySJRnn6e6UHp0+dtvv53xN9Wec/smaZIAcbvoONIxyONV9Ti0/xs2bBjSqvPJfk61tNTX8xzW+aO6lKyhw78PpGsw8jxN+Tid54xfSu16PvnkkzC2TzvttPD/33rrrehzunZjLZtZs2ZFZWoHJkyYENKqk8c6UqrNd84550R5tlvPPfdc2n0wPXr0COmHHnooKtP1Dc9JXX/37ds3yvOaVTWv1J8krS1fffXVKM92Qu0L2wW1S+qXeD4/+uijUZmuH9kvnXjiiVGZ2k5eI6iv0XZo3bp1SJ9wwglRGesuAbFvUp+gbcZ5XZew3pSuF3TNwj5CtZ9OPvnkjNdN8h9A3PYdOnSIyu6+++4oX6dOnZDW+9T1A9vkuXPnRmXqM9hfq21nTcpjjjkmKtN+Yc02nZfqe7i9te1VT5fnXmpNoM9SjJ8lYrL2pZQxxmQrdiTGGGOS8EspY4wxmfCzRIxfShljTDGxIzHGGJOEX0oZY4zJhJ8lYvxSyhhjiokdiTHGmCT8UsoYY0wm/CwRk7UvpcqWLRvioDmmWPUfVHuH45Y1LlRj/zmGWLVrOMZUNRJUk4Djd1WTKUlHSPWQVBuINSA0rlpjp3mQahtpbDLrMWh8udaJ70evw7HfqtGkukusk1GUlsm///3vkFbNK43n5c/qfWssMmuJsF4AkN6erA/CmgBAenw595v2N7eZ1kfjjHmc6b2oRgqPV9VCULi9GzVqFJV9/fXXUZ7vRftQ6899o0ZS5xPPGdWCStLk0OvwvWiZ6v3wdXmcAMCBBx4Y5VlDIDUH8vPz02L1TXax7777hhh+tueq3cD6fEBsW9V21ahRI8qznVN7xHOYNQoKg8egjlXVN+HPqk1Zvnx5lGebrbpBem9s97QOhx9+eJRnzY2RI0dGZR07dozy48ePD2nVn2Ifff7550dl6gu4/mofWccDiG2kalSobhTrKC5ZsiQqUxuY5Eu1Tmwj9b7VznGd1J6zfpfqeKjOR5IGX5JOis6JDz/8MMrzeNDrap7totZP75t9iq4v1A/zeNB1V926dQutK5Duq1jXR/tMNX9Y30Z9iq5NuO1Tflf1Z0x20aVLlzA+WN/n6KOPjj6nzwuLFi0KadWuWbp0aZTv3r17SE+fPj0qY9ujvkXtFn9XnwfUv7DP0Lnds2fPKD9lypSQVv0cfQZIum+dH+xX+T6B9LUm63Lpuuqyyy4L6X/9619RmeqTtmnTJqQfe+yxqEz9CddJ7arq9Go7MKpz9eabb4a0ahXpuOI6qRaeamux/pP6nmOPPTakZ8yYEZWpneJ7Vb+k98nl+oyn2mnsK6tXrx6VaX+zXdT5ousoXuPo83WvXr2iPLfLCy+8EJWxjpWO3UGDBkV5HsuqQaqwn1K/qe8gWCcx1UYbNmzAXXfdlfgbZitZ+1LKGGOyFf91wxhjTBLeKWWMMSYTfpaI8UspY4wpJnYkxhhjkvBLKWOMMZnws0RM1r6UKlOmTNi+zVtcdSunblvkLbh6RLx+l7d86/ZM3h6u23p1iygPED0WnLflA/H2Qt32raFpHHqh22b1d/gYbt2ey9vegfjISt3Kqds3eXuuhkTwFkw+VhRID/X65z//GdLaZ7r1mEM49L41NIDbXrdRasiBtm/SdTl0QEMitP7cjzpWeLurbkvVtubf4SPhC6s737eORz0OmPtCjzjXI695rvFx50DykeJ635rncaRjjuepGlvdwpwU0qohetwvGuKoY4Ovm6pfkuG3I8kOqlevHuwHb8FWe66+gMOaNLxHQyp4G7iGVLCd0DAwHY+HHnpoSHN4MJC+xZ7rxLZd6651ULuhcy0p7EptONscPfa6ZcuWUV7DIxm2BY0bN47KNJyhXbt2Ia3zW0Md2G/o8eMaHse2QO9TQ0kaNGgQ0nzsOpAefsP9pqFoHOIBxKFD8+fPj8p4fKo/1Pvm8aDhcLre4Pv++OOPozINeeO+UX+o8PpIQzzU93OIjYZ46Pjk+aVtzWNMwz90TnD91O/qfOJ71fWGthHbgtRvqi9h/FJq1/PVV1+FNRGH9KsdOO6446I8h4mdeOKJUdnf/va3KD9t2rSQ1jC2d955J6R1zZ/0DKBh22qvX3/99ZBWO6VznUOf+b6AdBvSsGHDkFb7rNft3LlzSOfm5kZl6kd5Tqp/fvzxx0Naw9/0N9lWcqgUkB5SxqF1bNcLY+bMmSHdtWvXqEztFP8Oh24C6f3P4Yh9+/aNym677bYof9ZZZ4W0PsctXrw4pDt06BCV6Tqe17PvvvtuVKZyGRzOzDIrQLrvYXuodlT99VFHHRXS2ofqK/mz+jyj85R9RJcuXTKW6fx54IEHovzJJ58c0vq8ou3J/c1+vLDfefDBB0O6Xr16ANJ9IuNniZjSRX/EGGMMk3Ikxf23PYwePRq1atVChQoV0K5dO8ybNy/x808++SQaNGiAChUqoEmTJnjppZcyfvaSSy5BqVKl0jSDjDHG7Bgl5SOMMcb8+iiJZ4np06fjpJNOQrVq1VCqVClMmjQpKr/gggtQqlSp6J++bK1Vq1baZ26//fboM4sXL8bRRx+NChUqoEaNGvjrX/9a7PbwSyljjCkmJfVSasKECRg8eDCGDh2KhQsXolmzZsjJyckozDhr1iycffbZ6N+/P9566y306tULvXr1ShN3BoCJEydizpw5qFatWrHrZYwxJhm/lDLGGJOJkniW2LBhA5o1a4bRo0dn/Ez37t3x5Zdfhn8c3ZTilltuiT5z+eWXh7L169ejW7duOPTQQ5GXl4c77rgDN910U9oOtaLI2vA9Y4zJZkriAWLEiBG46KKLcOGFFwIAxowZgxdffBEPPfQQrr322rTPjxo1Ct27d8ef/vQnAMCtt96KKVOm4N5778WYMWPC51atWoXLL78cr7zySlpoljHGmJ2DXzQZY4zJxC/tI3r06JEW4quUL18+TQJH2W+//TJ+ZuzYsdi0aRMeeughlCtXDkcccQQWLVqEESNG4OKLL97mumbtSymOG+b4WNUGUZ0bjvnX2FSNG+U4T43t5u/q91Tfh/UMNK5W47VZf0Bje7UOHEOuZaxPUtjvMno0JutOqGaPXocnCx8VC8Sx57oTQ7UYuA21z1RbieOYNV6Xj0wF4jhxva7qQ/C96HVV/4V1PbSf9Khq1ivSeGONq2fWr18f5bnNtEzrwDoZatBUI4dj0TXmXmP7WTdMj3FVHTNuIx1HSTpXGl/N7an3rfOH20HLVEuL20jL9L75s6n5nZ+fn/a5FDsSB673WL58+TRNFGBrm+bl5eG6664L/6906dLo2rUrZs+eXehvzJ49G4MHD47+X05OTrRdNz8/H+effz7+9Kc/penB/Nr44YcfQruqzWHUZvN8V00h1fR57733QlptFetk6NxSG8P6HOpTUtoDKQ4//PCQVk0IHXdcrtppai95fi9cuDAqY90RIG7P5s2bR2Wq6cNtpna3ffv2If3RRx9FZaobxMc/T5gwISrjI9CB2E9omWoXsUaE1l3XFNyG6mdV34LHg9pHHQ/qG5j7778/pHv37h2VqbYf97/aXdVYmTx5ckirL9LFJWs2qU6S6rywNqEeka26VtwOaod5bGiddM3Dc0avo/3Cn9W5r/owvD5SP6tjg3U+U+xMvRC/wPpl4XGiNkLtAvtY1okB0o+Q53GjtjJJv1BtJWviaH1YmwrY6tdTJPkaIF4r6TpedRK5XPWn2rZtG+XZDui99evXL8qz7f/73/8elXXq1Cmk1U4df/zxGa+jdoA1pLS+rG0HAOeee26UZ71fbU9dI7A91Pb85JNPojzrbqmtVO0qXpe0aNEiKmPNrrlz50Zl6qf69OkT0qw9BqSPObaVet+q/cRrDdXBvPTSS6M8+1zV2dJnUl4Tqz1VPSq+V11LL1++PKR1raZt9PLLL4e0rn1q1aqVsX6qrfzCCy9E+dQfhIH/2g2dG0xJPEtsC2+88QYOOuggHHDAAejSpQtuu+02HHjggdFnbr/9dtx6662oWbMmzjnnHFx11VXh2Wn27Nno1KlTZGtycnIwfPhwfPfdd2l9ngmH7xljTDHZkS23NWrUQMWKFcO/YcOGFfob33zzDbZs2ZL2MFulSpWMLztXr15d5OeHDx+OsmXL4oorrtiRJjDGGJNANuoObt68Gbfccgvq1KmDChUqoFmzZtHLS2DrS8kbb7wRtWvXxt577406derg1ltv9UszY4zZiZTEs0RRdO/eHY899hhyc3MxfPhwTJs2DT169Ij+OHXFFVdg/PjxeP311/H73/8ef/nLX3D11VeH8kzPHqmybSVrd0oZY8zuyGeffRb99X57/7KxPeTl5WHUqFFYuHBh2s5CY4wxvy5SuoNjxoxBu3btMHLkSOTk5GDZsmVpp2cBwA033IAnnngCDz74IBo0aIBXXnkFvXv3xqxZs8LujOHDh+O+++7Do48+iiOOOAILFizAhRdeiIoVK/qPGcYYkwXsrGcJPvWxSZMmaNq0KerUqYM33ngjnErKERhNmzZFuXLl8Pvf/x7Dhg3bqc8w3illjDHFZEf+urH//vtH/zIZ9MqVK6NMmTJpR++uWbMmY1x31apVEz8/Y8YMfPXVV6hZsybKli2LsmXL4tNPP8Uf/vCHtC3Lxhhjtp+S2CnFuoONGjXCmDFjsM8+++Chhx4q9POPP/44rr/+evTs2ROHHXYYLr30UvTs2RN33nln+MysWbNwyimn4IQTTkCtWrVw2mmnoVu3bkWe/GqMMWbbKYlnieJy2GGHoXLlymnhpky7du3w888/h3DVTM8eqbJtJWt3SqWOHAQQnQ6lsb0aU6wxlozqBXDMqWoosMaMxuBqx7P2gWqFaP6LL74IadU60Fha1i9QrRDVW+A4V9XB0a1zX3/9dUirPpIuilh/QbfmcVtr2+qJXhxnyr8PpOtBsJbWhg0bojKN5ef6V6xYMSrTfuJ+LEr7i6+bpD8EIIq7Vb0Kbk+9DsfjA3Efavyt3guPDe0z7VMeZ9p+GkPO41N/U+vP41X7VMcy96OOFdaj0bbV3Tzcb6ohpPNU+yLTdYDCda2SHhB2JA58WylXrhxatWqF3NzcoLWTn5+P3NxcDBw4sNDvtG/fHrm5uRg0aFD4f1OmTAnaLeeff36ajkFOTg7OP//8IKb+a+LAAw8M44dtoo6bVatWRXnW4lGtAZ0/PF51zPH80d9gfQMg1p/S+nEZsPWhMIXq2qh2EeshqNaYajnwfavmgr6U5AdQtUdq3w855JCQVn1BtlWs2wHEuoRA3A5qf1TfgLVQ9D7VFnTp0iWk1aeoPgf/7rhx4zLWD4jtlY4bhbVQVC/mlFNOCWn19QcffHCU535T3672nX1248aNozLtC25PXQ9pm7EG2ueffx6VqU4YrxP0vuvWrRvleT2nOhw8v9RvqU/h8ai+SOcwz0XVk1PNLu7j1HzRtmF+aU2p7dEd3LhxY9q6ee+998bMmTNDvkOHDnjggQewfPlyHH744Xj77bcxc+ZMjBgxolj1ywZOP/30YDOnTZsW/j9r3gDptpPXNEVpt/EYeuKJJzLWRddJard4rqvm1WuvvRblVQeVYa1VIPYnRWnkDh06NKSff/75qEz1k3iNpbvy1DZNnz49pFkPC4htXocOHaIy1RTidtA2Ur0f1rc7+eSTozK1GWzTeB0MINLkBIC+ffuGtNo/9Y1sk3XeJWkN/e1vf4vy7JfatWsXlakf5ZcDqiupWoennnpqSBelVcW6ZuqP33777SjPdlefy9VX8vzRe9Nxzn6MdRCBeE5rfbSNeI7k5eVFZdov9evXD2k9lU7H1V133RXS3bp1A5A+1piSeJYoLp9//jn+/e9/p609mEWLFqF06dJh3rdv3x7/+7//i82bN4e1+JQpU1C/fv1t1pMCsvillDHGZCsl5UgGDx6Mfv36oXXr1mjbti1GjhyJDRs2hBdIffv2RfXq1UMs+ZVXXonOnTvjzjvvxAknnIDx48djwYIF4VjWAw88MG0xsddee6Fq1aqR4zXGGLNjbO9LqW0VsE3SHdQ/eqXIycnBiBEj0KlTJ9SpUwe5ubl45plnoheR1157LdavX48GDRqgTJky2LJlC/785z+niUMbY4zZfkriWeI///lPtOtpxYoVWLRoESpVqoRKlSrh5ptvRp8+fVC1alV89NFHuPrqq1G3bt3w8nj27NmYO3cujj32WOy3336YPXs2rrrqKpx33nnhhdM555yDm2++Gf3798c111yDJUuWYNSoUdFLum3BL6WMMaaYlNRLqTPPPBNff/01hgwZgtWrV6N58+aYPHlyeAhZuXJl9FenDh06YNy4cbjhhhtw/fXXo169epg0aVLaLgljjDG/LNv7Ukp3mw0dOhQ33XTTTqnTqFGjcNFFF6FBgwYoVaoU6tSpgwsvvDAK9/vXv/6FsWPHYty4ceFo70GDBqFatWppp6oZY4zZPkriWWLBggU49thjQz6lD9WvXz/cd999WLx4MR599FGsXbsW1apVQ7du3XDrrbeGP4SUL18e48ePx0033YSNGzeidu3auOqqqyKdqYoVK+LVV1/FgAED0KpVK1SuXBlDhgzBxRdfXKy6lirIsuM01q9fj4oVK+Kggw4KD1v8Fxz9a5GG6HC5bvHWbasc7qHhPLzdTo8B1uvylm/d3q/bfjkUQ+MsNfyMtxDqttSkUDUNgdLP8n3rdn99eOVtd3rf/Jt8bDqQ3tbaLoxuJ+XwFP1rn4b6cb/xMepAeqgAb/U84ogjojLdXsmhDHq8ro453pKr7clbeTW8R3+Twwp0WmoID4853RKuddi8eXOhdQXSwxZ5y7Vuv9YxyNfVv+zqlmYOOdF74fGqoRAaasHf1RBWbQf+rs4JHZ88zlNbgPPz8/HNN99g3bp1YYt7yj5dcMEFaW1XFJs2bcIjjzwSXc9sH6l+uO2228KY5u3Z2t96tDHPHx1jOr95Duu28w8++CCkdbeCzh/+TQ0T0pA8nls6VjXkg+2whlvoNnSeMxziBKTbAva7aqM11O+2224rtD5AbHP0exri2LNnz5CeOnVqVKY2hX3rGWecEZWp7WffxX0GxMdcA/FW/RkzZkRlGhbDfVNUGOjChQtDmsNKgPhocG0jtZcaWsfovfAaQ8MCtX7sozUsQrffs0/U62roJK8/1E9oaB2HcWiIKx+1fuSRR0Zl6vMY9aUatspzTcN2dByxz069OPrhhx9wzjnn7BQ/kfIRhQnYFrZTatOmTdhnn33w1FNPhRBvYOvDxtq1a/Hss89m/K2ffvoJ//73v1GtWjVce+21eOGFF8L4qVGjBq699loMGDAgfP62227DE088kXEHVraR6oMbb7wx2CBe1+lc1rU695s+A2hfcNiTji9G7b7KkXCI79lnnx2V6Xpn6dKlIa024vTTT4/yc+bMCWl94fmvf/0rynM7qE9LQm0Ey3AA8dzS0GHexaFtrffNdapdu3ZUpqdIsv/j8Dxgq6Azw/ZQr6Ohiey3eEwBsWg0ENsmtY1qy/m6+nzYuXPnkFZtN/WjrVq1CmkNU9X1DbevPismSd6o7dYwO24zff5T38NjTp/FNc9jXX1P0jMJ+w8gDpXV9Y36Z87rMxS/7NH6ptYHGzZsQO/evf0ssQ1Y6NwYY4rJjogTGmOM2f35pQVsWXcwRUp3MKUjmIkKFSqgevXq+Pnnn/H0009HumY//PBD2oNjmTJl0l5+GGOM2X78LBFTrJdS9913H5o2bRocZfv27fHyyy+H8p9++gkDBgzAgQceiH333Rd9+vRJU2M3xphfO3YkmbGfMMaYkjl9b/DgwXjwwQfx6KOP4r333sOll16apjvIQuhz587FM888g48//hgzZsxA9+7dkZ+fj6uvvjp85qSTTsKf//xnvPjii/jkk08wceJEjBgxAr17997xRoF9hDHGAH6WUIr1UuqQQw7B7bffjry8PCxYsABdunTBKaecErb8XnXVVXj++efx5JNPYtq0afjiiy8iZX9jjDG7N/YTxhhTMpx55pn4v//7PwwZMgTNmzfHokWL0nQHv/zyy/D5n376CTfccAMaNWqE3r17o3r16pg5c2YUqnjPPffgtNNOw2WXXYaGDRvij3/8I37/+9/j1ltv3Sl1to8wxhijFEvo/KSTToryf/7zn3Hfffdhzpw5OOSQQ/CPf/wD48aNC8cvP/zww2jYsCHmzJmTpgFQFJs3bw6aAhyHq/HFGvPPca6qT6Mxphz7qXHgrGegcbYa/5mk/6FvNFk7RE/BUg0Frp/ep9YpSRdBt2FzXLvet8bVszbL2rVrozJua43tTaqDtpFqhfC96meTYm9VR0ZjslkHQ6+r2+NZU0P7SePAWaMkSe9DY661vvw7Wh89Fpf1k7R/k7TTtH4cyw/EfaxtrX+p5Pml9dU4Z57Det8cEqAaOBq/zb+pGlcKzz39TdUR0nFfFNl4jGu2UJJ+omzZsqFvWU+nqDh71jtQW6osXrw4pFUThK+jv6lHQ7PuiB5lrRoG7Ce0fmpHeOyqVkfdunWjPOtc6W+qv2Sdpn/84x9RmWotcbvodVm7Qf236hTyseFNmzaNyvSo8DfffDOk1RaoRgTbMvV5atf4KGm1l2oTWddFtaCaN2+e8bs6znmsqH6J6gJxH7/66qtRmeqksM6LHg2ubc/3qvowTz/9dJTnUC9ta9Xs4vbVtm/Tpk2U5yPnVVuG9WO07mq/kzRK9LPsL1VvRzVgWE8pNV/U3zLbK3ReXAYOHIiBAwcWWvbGG29E+c6dO0fjtjD2228/jBw5EiNHjtyu+hRFSfqIJUuWBLvDenyql6N6qs8991xIq31hO6Xlavd5HaraZ0cddVSU1znK6Jqa56jWj20YEI95XW+rdtWsWbMK/Q0gXZcndToXELcXkO4jrrzyypBW7UOeo6eddlpUxv4XAB588MGQvvbaa6MyXfMvWbKk0N8A0tts7NixIc3PU0C6/iK3g55arP6P9XZbtGgRlWn7sv1T+N7Ur+szAPex3qfq/7KOo/pC9UU8tlUnitsPiNcEuv7W+rJPU60qtdc897QOzZo1C+kkzV6tn/p1DVPmOujzoK7HWLMr9Zy2M31E6ju7K9utKbVlyxaMHz8eGzZsQPv27ZGXl4fNmzdHgp0NGjRAzZo1MXv27IzX2bhxI9avXx/9M8aYbMZbbrcN+wljzJ6KfUTR2EcYY/ZU/CwRU+yXUu+88w723XdflC9fHpdccgkmTpyIRo0aYfXq1ShXrlzajp4qVaqknULEDBs2DBUrVgz/9C9VxhiTbdiRJGM/YYzZ07GPyIx9hDFmT8fPEjHFfilVv359LFq0CHPnzsWll16Kfv36FbkVOInrrrsO69atC/9066MxxmQbdiTJ2E8YY/Z07CMyYx9hjNnT8bNETLE0pYCtsZepeNZWrVph/vz5GDVqFM4880xs2rQJa9eujf7CsWbNmrQ4X6Z8+fKFHne73377hbjTTMfhAum6Axxjum7duqhM9UA4r9oBrO+k39N4Y/4sa/0A6fGnrJGjTlM1pTj+XeOhVf+D20j/wqT159hajTdetWpVlGddDP0rFcf+apnGInNMrbaJxlFzG+nY0VhfbrPvvvsuKvvoo4+iPI8NvU+NN+Zrqe7SYYcdFuW5DTUmm+OaNX5cdbh4DOqY1zzrf3AMM5Aer81tVNQJNmzsdE7oXGOtG+0XjaFmvR29LudVl0c1Xfg3NU6ddXiAeM5o/+rWfp4zqbml85FxHHgyJeUnypcvH+wFz0P9rMb9s71SW6pjmTWR1L7z3NN5p5oGbDeWL1+e8TpA7GNYpBhI9xuqI8WwjhUQ25zWrVtHZaoFxBohqkOh2m88n7i9gFg/q1+/flHZpEmTojzrgun8VtvFfk01XljzCABef/31kFZtRLUxbLvUl2p7sr3S+a36MDzOVPuJ/Y3+xrhx46I8+2S1YzqW2Yap9pO2A485Hbuqj8X2VMenwtfSsbFw4cIoz1qOag+S5ix/D4i1T3QdqOsE/ixrRgHp/c9rspQ+lrYVU1w/YR+x833EH//4x7D2mzp1avj/3377bfQ5tS9nnXVWSE+ZMiUqO++88zJ+V9chPGb0pZtqNLVr1y6kdV2sayq25fPmzYvK1LYzast1XXfMMceEtGo/sWYPAMyfPz+kdX2r2lAzZ84MaZ2DJ598ckir5pWuCTmsU7WAtI34GSUl/J9iwoQJUZ6fWdT36HUXLFgQ0vo8wL4GiDWndO2r7XDZZZeFtPb//fffH9L67KB+gH2azhkdn/wspGNBr8s+V7UudWcil+t961zjMaf9PXHixCjPfurEE09EJlSPVtcarEuofab6cmzjVRdMtd54/Zham+1MH5H6zu7KdmtKpcjPz8fGjRvRqlUr7LXXXsjNzQ1ly5Ytw8qVK9G+ffsd/RljjMka/NeN4mE/YYzZ07CP2HbsI4wxexp+logp1k6p6667Dj169EDNmjXx/fffY9y4cXjjjTfwyiuvoGLFiujfvz8GDx6MSpUqYf/998fll1+O9u3bF/u0DGOMyWb8143M2E8YY4x3SmXCPsIYY/wsoRTrpdRXX32Fvn374ssvv0TFihXRtGlTvPLKKzj++OMBAHfddRdKly6NPn36YOPGjcjJycHf/va37apY+fLlQ/gNb53UbZUKbz/UsDUNx+EtjvpZ3vapWyz1yErekq7X0frydkjdpqghRhyWoeFmGnbHg1S3qeo2S24j3Vaon+Vtlnl5eVEZb6NMChEE4u31Goqo4TJcf91qqqEW/DsaAqPhE9xP2vbaDnx0dcuWLaMyDb3hrak6Nri+GnKg22p5fGrI4McffxzlOQRS20+39nK7FDV/eMurhuhon/K81PvWbcAc2qRtzVuwtUzDJ7jfNJRKtwjz+NRjZXUccX1TYy4/Pz/tN0zRlKSf2G+//YLtYRupIdYausT9quHEOp/YXul2dp4TGiakx0jzHNGjjDUMgbf8r1y5Mirjre5AHNak41VDmGvXrh3Suu1cw7Dq1asX0tp+Gp7NoWB9+vSJynhOc7gHgLTTtDp06BDSSccoA3HYhPqme++9N8pz2IyGtqiN4fbV48i1n9hfqo3h8AAgtqdJ4fgaaqrHxnPYUZcuXaIyvRe2/TqukyQANBxOjyDna6lfUD/M5ToeObQJiH2g2nP2IXovuh7isaNzTdc4bCu0TP0a1yFVVtQ4NemUpI+YM2dOGIO85tIxpKGkbEt1LfTaa69FeV6n6rqT/ZLaUbUnHLqrn23QoEGUf+aZZ0K6Vq1aURmHXgOxvT788MOjMrVxHD6n61C1TQ0bNgxptT3qi9i/9OzZMypjW64hjRrOx2FiL730UlR29tlnR3leLy5btiwqY/8GxP12xBFHRGVvv/12lOe+OPbYY6OypHAzfU5q2rRpxjroWoP7UJ8dtK05VFKfezmcHojbWyUIZsyYEeU5fFNtd9u2baM8+0Oda+zngViS4J133onKTjjhhCjP40jbiH3uW2+9FZXxMx0Qr/l1zaJzmMeKlqn/43VVqq72EdtOsV5K/eMf/0gsr1ChAkaPHo3Ro0fvUKWMMSab8V83MmM/YYwx3imVCfsIY4zxs4RSbKFzY4wxu7djMMYYs+PYTxhjjMmEfcR/8UspY4wpJv7rhjHGmCS8U8oYY0wm/CwRk7Uvpb755psQC6v6C4zqNnCMtmo8JGnO6HX22muvjL+ZpBulmj2aZy0bjbPVIyw5Tli1DZIGperl6PGbrH2iceD6O3xEt7YfxzirjoTGMXOMtmqZ6L2wnoXqXmj9OE5Y21Pjrjn+WGOROTZef0fvTduB+03HKveF6mPp0e58rxojrn3Kcfba1vpd1nvR8ahtz5/V66iODGt1qIaPxm9zubZD0jzUOcFjQ9tE86wPorpwOq7YVqSukzTH7Eiyg59//jmMH9aG0jmhmiA8T1U3QzWmeFyp5gzr8OgcUC0b5quvvoryOie4vqoBolpVPE9ZNw9IP6ab53+S7hsQzzWtQ9JR3DqH+bhy1fFQ/RDWx+rdu3dUpv3C+liKXpevpbZfj7LmflQ9Lz1GnseRanKpzeE+Vn0THle6vtC2Zxut65TOnTtH+U8//TSk9Sh4HrtAvBbQOmifsn1X7Q7WwgTi+aO6a6q1Ua1atYxlSb5e5w+3kc59nXusD6O+Xf0Ej8FUe+lnGL+U2vU0bNgwjN/JkyeH/6/aOmrbWadMbc2iRYuifPPmzUNa5+Rxxx0X0qqXo88orGf39NNPR2WqP8QaPjpfde7wfGCbAKTrJzVp0iSkWZsISF/X8fOB2gjVwHr//fczXkfnM/PBBx9E+UMPPTSkdd7rmpXn+llnnRWVsSYXEPtOtRFKq1atQlr9iep78fOO+k1tX+4L1RFmbcFXXnklKmvcuHGUZ79flG4w94WuYbp37x7l+VlS10367MP9pusQ1cjltYfOyxdeeCHKDxo0KKTHjx8flfF4UF+tz1vsn7W/eT4DsX7WrFmzojJdc3EbpuyGPrcyfpaIydqXUsYYk63YkRhjjEnCL6WMMcZkws8SMX4pZYwxxcSOxBhjTBJ+KWWMMSYTfpaIydqXUhUqVAhb+nj7oW6v1pCdypUrR9dgdJslb6nTrfZ8lKj+hm7F423wOliSwgB1y6pu7eTth1rGW1iBeKuntpEeWcmhLUnHtgLxtlDdpsjtUlR4B2/71C38GlbAWzC1PTWEQ4+LZXSrNLc3hwkUdl3ecquhIBoOwNv3ta15W6iOPw0L5HHF262B5PBSHbsalsFhRLp1W+Hvah9q6B+Htmhon25L57mo84l/R/tb24y3COuWdW0Hnj86D3Us83b31PbbpC3ldiTZQcWKFcM44LFSpUqV6HO6lZtD1/g4aiDdPiWF4XEondoi3d7OY0x/Q20M23C1BTqWn3/++ZDmI5uB9PDs5cuXZ6yvhh3wdzXcQkMz+N4mTZoUlXFIns59DkkAYv+jn9U5y8d0s78urH5cfw3r1v7lsEVFt/lz36i9PPXUU6M8b/vXEDe2jzpW1ddzGI/aZPUpPD451AZIHxscrqThFXpvS5cuDWntF10f8THyWj8Ni+J5qW3NazuVJNC1HttaDeXV9mQ7r2U6T/leUt/T8Bith19K7VoeeOCBYDMvu+yy8P9nz54dfU7tDa8ndHzpepHRedahQ4eQVjul67rXXnstpDUET0MGOdRPr6uh2XPnzg3pli1bRmVPPfVUlOd1nc5ttY28Vq9evXpUpiFmHJo2Z86cqIxDq44//vioTEO+ef2t9oR9DRD70XvuuScqO++886L8ihUrkAkO3wLi56Jx48ZFZTqH2b/k5eVFZccee2yU5zGp4XscZs4hlkD6up5DO5944omorFevXlGen1/YBwDA/PnzozyHQGp4qfYbj0G23UD6/GEbrH2o4YbXXnttSGu/8JpLfayu8/iZReehjnPuC33G07Umr8FSazN9ZmT8LBFTuuiPGGOMMcYYY4wxxhizc8nanVLGGJOt+K8bxhhjkvBOKWOMMZnws0SMX0oZY0wxsSMxxhiThF9KGWOMyYSfJWKy9qXU5s2bg6YUx3PrsZOqF8B6BvpZPfKaY0OT9GlUc0L1iFjXQbUXNP6UNQr0OFOtA5drvLvqMLGugWpFaDx80rHg+lluT60f63RoTLvGOLOWiWoe6RHnfJSo9qHG+nKf6nU0z/XX+HHVn2JdDz3yWeODWZslSVtLj7ZVbZgk/THVCeNxrwZK5wTH3Wt7ap+yFpT2k943979qb+i4Z30EvU8eu/obet8cm651V30V1h3RNtFxz/eduq41pbIf7ge2ezp2VeOMx6Dq6qnmEF+X9TaA2I6w3gyQrrPG81+1G1RzgY8V1vmiY5ePHFd9G9Ul4XvRo5fVhnMd1Ae+9dZbUZ5tAWs9AbEew8svvxyVaVuzRoTOP7UFrBmhvl01K1hTZfHixVGZapZ89NFHIa3HsGubcZ+rPz/yyCOjPM9//g0gvletj/ox7mMdG2qHWd9G1xC6juE6qJaM2i6eXzrXVBOL66jjSK/Lvlb1YnisqM5IEjqOVKeQ9dx0POpR5uw/U/olOscYv5Ta9Zx88snBp/O6Wdt65syZad9LoZoz6jPY/qnNYH02XZvrOonXP6qLp/OM57ZeR+cHH3Gvmj1nnHFGlJ86dWpId+3aNSrTuc06eaecckpUpr/D2jv6fMDaco8//nhUpjaXtatOPPHEqExtO9vnbt26RWUNGzaM8s8++2xIF6UbNHr06JBmzTAg/dmCx87pp58elaneE98b62wBcf9r/fQZhbUOL7nkkqhMNcS4/gsWLIjK1Fbm5uaGNOtLAelrD9bl1XWTrnd4rOs41+cmHsvt27ePygYPHhzS3bt3j8p0fcbjs3Xr1lGZPg+yX1DtNNV64/Gamoc700ekvrO7krUvpYwxJluxIzHGGJOEX0oZY4zJhJ8lYvxSyhhjiokdiTHGmCT8UsoYY0wm/CwR45dSxhhTTOxIjDHGJOGXUsYYYzLhZ4mYrH0ptWXLlqAFwPGYqh2hmgqsiaQxrqpBw9fV2FnWVChKm4rzql2isegce67X+fLLL6N8UgyxxrSzng7HEwPp7XDYYYdlrJ/CGhA1atSIyliLQeOoVZuK25N1qgqjZcuWIa1tr5pDjOoGqRYHxxRre/K9APF4UJ0ObV8eV6ydBcT1V40MjZ1O0uhSXQweuxqfrbHT3P865lRnhNE20vnDceyqYaBGk/VgVBuG20h/Q/ufr6vjiDVwgHjsapnqv/C8TbWRNaWyn6+//jqMU9ZwYj0xIH2usZ6O6h2oHeY5ouORbUFROg+sYaF296uvvorybCtUR0/hOqkGjmoX1a9fP6RVRyFJj0Ovo23EOg9qh9lWnXnmmVGZ6sCxHVm2bFlUpraBbXatWrWiMtaxAmKtKtWAUA0sbiPVBVP/zn3KGldArEup5Vo/1qxQ3Ra172zDWSursO+ydpnaevWlbJ+0fqqFw5/V31Qfw3ZYx1GS9uBRRx0VlfGYUz0s9QWst6NrEdUoYT0bXSupP2/SpElaHZLWM34ptetZuXJlGAPsB7Rvzz777CjPY3P+/PlRWefOnaM860apXiD7Iv1NXRPyOkXnoK5DedyyriAAzJkzJ8rz/F24cGFUpnaKbVFKNy2Frn3Z3zz66KMZy4DY/vAaHwAeeuihkNa5rfOVdaTUz6uP4Lyu8ceOHRvlWSvo/fffj8r0+eboo48OaZ3/+mzWs2fPkH7xxRejst69e0f5adOmhbQ+b3Gfqmai2i32d//3f/8XlakOE49X1c6aPn16xu/q+NT1Dq+f2W4C6ZpirGOm/kPbgefBfffdF5U98sgjIa39q7pOST5M5yXXQeehPku8+eabIZ1aCyU9t/pZIiZrX0oZY0y2YkdijDEmCb+UMsYYkwk/S8SULvojxhhjjDHGGGOMMcbsXLJ2p1SFChXCNj7efq3herr1lLeIamiAhl7wNlXd2vf555+HtIaB6VY8DlfQ7a1aX94SXK5cuahM68vb1TVsQLc4cp30swqHJ2j9NMyFw0r03jhkQkNM9Drcvhouo3XgUD/dlqpviLnNdNuvhmxx2+u96JZMHkdaBw315KNbDz300Iz10/AJHXO8vVjDJbQ9uf91Duh2Yg6X09/UccRbcDUMR8PZeJxpiIRuYea5p+OTt79q22r9eDu29q/Ob75vPepbQxx5DKbaOim00X/dyA7Wr18fxhP3t84fHSu8PVtD6b7//vsozzZQQ6nYhuu41tAktjk6P3Su8ZzQOaDX5dARtT9t27aN8hx2kOQ7Nc8h30D6fGcbqEdt83c5rABIt7v8XQ2D0SPbeb6rzdO+YF+l4cP6WQ790q35Gt7A9lTDGTR8hUME2rVrF5VxW+tY0Dbisau+U4+r5mvpveiR7byGaNGiRVSmv/Pee++FtM4tnU/cLtom2sdJ8gvc32pLNXSEw0DV5+mc4HvTNZiOFV4XptZR2l+Md0rten766afQrroOYDQkuXHjxiGtYbw6LjjcS58XOnbsGNIcngUAHTp0iPIcUn333XdHZZ06dYryHM6l4Xoaote9e/eQ5vU/kB5a9cUXX4T08ccfH5VxeBQQz1f1PdpGPCc1HPKII44IaQ3J4/A3IPZbRx55ZFT297//Pcrzveo8nTVrVpTn9tWQMV1bchjblClTorI+ffpEef7dY445JirTEHW2wWor+blJ/XGXLl2i/MSJE0Nax436KQ6d41BrADj88MOjPPepPr+qhAf7LW17lSfhNY7et65/2NerBMFf//rXkL7sssuisnnz5kV5trXqE3gNoHn1J/rcyfeWClNMeib3s0RM1r6UMsaYbMWOxBhjTBJ+KWWMMSYTfpaI8UspY4wpJnYkxhhjkvBLKWOMMZnws0SMX0oZY0wxsSMxxhiThF9KGWOMyYSfJWKy9qVU6dKlQywpx6NqPKfG+laqVCmkNaZZtUJY14O/B8Sx56pzo7oSrPGgZarTwXXSuFq9F9bw0XvRPOs6aPyuaj6wVoPGAat2BNdRj0nl62q/JOX1N/QYV+4XjSfW+2ZUV0Rj07l9VU9FdcL4vjXOWg1Ckl4Sjx2NwdbPsl6Nal7pfXMsvx5nqp/l+mq8tmqBcXvrfWp9uY30N7XNuM9VI4VR7SzVQeE21N9UDRKeP6wLBKTPCc6n2lY1tBg7kuygWrVqwX6wfddxrTpMrEFTr169qEz1qHguql1jP6E6Hqq7xPNbx58e8cz3ojo3rN8ExDpR6uPUpzA6X1SfgY+DfuONN6Iy1bTgeao+hefp22+/HZWxlggQ6+qpDVQ9Km7fJUuWRGXqz1kLSMvUx5xyyikhrf5btWX4upwG0v0a+2X1P2yfVKNC68C/o/Zcx4qOQUbbgftQNfc++uijKM9aI2qj9bM8F7X9dJ6y31DdNbbHelS5asAwOp+T9AS1z1RDjv15Si9EbQLjl1K7nsMOOyzYf9bfU20l1TdjbSU9Il7HOK9b2rRpE5W98847Ia32WPOs2VS7du2oTDWvmjVrFtKqa3TBBRdE+aR1vNrVBg0ahLTaNC4D4jU33ycQtzUQ6/qpz+XnJv2eagH9z//8T0jff//9UZlqA82YMSOkVTtLn9XY9ixatCgqY58AALNnzw5p9R9qg9k+qD3WdfKpp54a0pMmTYrKeFypn9f+ZzurulDquxcvXhzSqjPYtGnTKN+oUaOQVlul6wmeM9r2qjvI6yH1jUlzRtuTf+fhhx+OyrQdeH4vX748KlM/wH7qtNNOi8pGjx4d5Vu2bBnSKc24DRs24J///CcKw88SMT59zxhjtoOUM9nWf8YYY/Ys7COMMcZk4pd+lpg+fTpOOukkVKtWDaVKlUp74XnBBRegVKlS0T8+HAHYuvnh3HPPxf7774/f/va36N+/f9rL+sWLF+Poo49GhQoVUKNGjUh4flvxSyljjCkmxXUifugwxpg9C/sIY4wxmSiJZ4kNGzagWbNmabu6mO7du+PLL78M/3Rn17nnnot3330XU6ZMwQsvvIDp06fj4osvDuXr169Ht27dcOihhyIvLw933HEHbrrpJjzwwAPFqqtfShljTBYzevRo1KpVCxUqVEC7du3StrMrTz75JBo0aIAKFSqgSZMmeOmll0LZ5s2bcc0116BJkyb4zW9+g2rVqqFv377RVmZjjDHGGGPMr5sePXrgtttuQ+/evTN+pnz58qhatWr4x9IA7733HiZPnoy///3vaNeuHY466ijcc889GD9+fHh2GDt2LDZt2oSHHnoIRxxxBM466yxcccUVGDFiRLHqmrWaUvvuu2+IHWVNBY31VL0F1iFQDR/9LKNvHpM0PZL0c5K0f4A4vnjlypVRmeoi8NY41eFRDRK9V0Y1PlhTQfWyVGeCtVi07JBDDsl4HdVz4ode1Q3S+GjuJ/4NIF1vg3VHVDdG45Y5Jr9u3bpRmW5D5DZSDSzVg+Gxo/oSrCOSpJ8BxG2o+lg6PrW+SdflGGy9rrYZk6RHAsRjXdtINbp4/Ooc5rzWXeP1+b61fhrTzuNI57COQdYdSd1LUfaiJOLAJ0yYgMGDB2PMmDFo164dRo4ciZycHCxbtixNnwUAZs2ahbPPPhvDhg3DiSeeiHHjxqFXr15YuHAhGjdujB9++AELFy7EjTfeiGbNmuG7777DlVdeiZNPPhkLFiwodv12NfPnzw99yVoJOs7VPrJN1HGjNpy1J3RM8LivXr16VKaagdz/eh0d96yFoRo4zZs3j/KsR3TwwQdHZe+9916U53vVeag6H9xmatdU74m1HNRXseaQ2pvXXnstyvfr1y+k69SpE5Wp7Z87d25Iq59QHQrW3VNbpW3Pules2wLEmldArM+imhWqscL6War7yAvAVatWRWV6361atQpp1QDRe2MfqH5WtQjZrxWlj8XX0nWMtueRRx6Z8bM6D1i38NBDD81YX9XSUv0pvq7aes3rtRhd1/AaLaUplaTbZk2pXc9HH30U+px1jVQ3SOfr6aefHtK6XtS1Jc+HmTNnRmVsF3ReqX3m8aY2Qn9z8uTJIa2hNnpdtik9evSIyljHCoh1g3SuqB9lfUPW0gGADz74IMofc8wxIa36WGzH1KZxnwGx5pTq2ekam32j1l3tFPebPjOppiLPef0sazQBsVajapGpjhn3mz5vsZ3SNlF/zPYwLy8v428AsS6m2lz9YyXft9putYM8HlQn6t13343yxx9/fEhr/7do0SLKz5kzJ6T1OZjXN40bN47KdE3I65233norKlOfwPpu6mtUd4vnWmotuTN1B1PfAdL9U/ny5dPm7Lbyxhtv4KCDDsIBBxyALl264LbbbgvtO3v2bPz2t7+NxnLXrl1RunRpzJ07F71798bs2bPRqVOnaJ7l5ORg+PDh+O677xL9LFOsnVLDhg1DmzZtsN9+++Gggw5Cr169sGzZsugzP/30EwYMGIADDzwQ++67L/r06ZP2gsIYY37NlFT43ogRI3DRRRfhwgsvRKNGjTBmzBjss88+eOihhwr9/KhRo9C9e3f86U9/QsOGDXHrrbeiZcuWuPfeewFsXUBNmTIFZ5xxBurXr48jjzwS9957L/Ly8tIeGLcX+wljjHH4XibsI4wxZseeJWrUqIGKFSuGf8OGDduuOnTv3h2PPfYYcnNzMXz4cEybNg09evQILx5Xr16d9kfwsmXLolKlSuEl4urVq9MOD0jl9UVjEsV6KTVt2jQMGDAAc+bMwZQpU7B582Z069YtOsnoqquuwvPPP48nn3wS06ZNwxdffBGdKGCMMb92dsSRrF+/Pvqnu8pSbNq0CXl5eejatWv4f6VLl0bXrl2j01+Y2bNnR58Htv61ItPnga07W0qVKpV2StX2Yj9hjDF+KZUJ+whjjNmxZ4nPPvsM69atC/+uu+667arDWWedhZNPPhlNmjRBr1698MILL2D+/PlpOwRLgmKF7/F2UWDrts+DDjoIeXl56NSpE9atW4d//OMfGDduHLp06QJg67GMDRs2xJw5c6Jt3EVWrGzZsB2Qt2RqaIWGSHB4gG7XU/iI4aRjPDWESMO3eLua/mbSEc26nV5DsnjLo2411ZAO3hqn4RNafz7mWLfla3gFb9HU7ZpLly4NaQ091DemjN6nbjfkLZi6LVXbgbeb6hZR3drLaD9pnn9Xx5xuA04KneSQA21bDT/j8aBtomOOx67CIRBA3P/6PR2f3L7antpvHCrE26SB9PrzvSaFtGrddZHO23V166puaeb6avvx4lfLU9vmk9p4R7bc6lwZOnQobrrpprTPf/PNN9iyZUuhf33QY51TZPprRaa/VPz000+45pprcPbZZ6fZ0u2lJP1EmzZtgg1Lsvc6R3l+a39oaAHPH/0Ntolqq9S+c+iGHsOtOwB4W79u8Vd7xDZcxyxvzQdie1RU6AP/ZUxDR9SWcaiJ+hQOWdD24+3gAJCbmxvSujU/yU/oVn31VRyyoCGO2vYcdqL3onaDyz/88MOoTNuej51W28E+WW2gHpHO/a9tpPOcx26SvwFie6p14PoBcXi2bsvXsCMNi2J0zLEN0nBiDtHUOavhEdxGGqbIoRhAvJbSPtM243wqpEvDfxmH7xVOSfqIffbZJ/Qb29ITTjgh+pw+gPF8VfunYU3t2rULaa3bs88+W+g1AeDSSy+N8o899lhIcxgdALzwwgtRnv/4pLZc7RSHgul81JAttgtFSTiwnVX7p7adfd78+fOjMg6B0zmoef5N9SdqKzn0S9tI10lsU9T2aCgdo+tktWnsk9UvcfgjEN+rhoPzvalNS1rz6/qhQ4cOUX7ixIkZ685hdQAwZcqUkFY/+vrrr0d5HmcdO3aMynRscOikrtV1XPG6vmHDhlEZh/TrPNTnYg6z03vR+c3+RdcLul7kNnv11VcBpPcPsyPPEvvvv/9OYmjIXQAAUIVJREFUW7czhx12GCpXrowPP/wQxx13HKpWrZr2jPfzzz/j22+/DWO2atWqaW2TyuscTmKHhM5TnZyasHl5edi8eXNkLBs0aICaNWsm/qXeGGN+TWTDXzd2lM2bN+OMM85AQUEB7rvvvl/sd+wnjDF7It4ptW3YRxhj9kRKSgqkOHz++ef497//HV7WtW/fHmvXro30yaZOnYr8/PzwQr59+/aYPn169FJxypQpqF+//jbrSQE7IHSen5+PQYMGoWPHjuGvlKtXr0a5cuXSwkCS/lK/cePG6K9uuvvBGGOyjZL460blypVRpkyZQv/6kOkvD5n+WqGfT72Q+vTTTzF16tRf5K8tgP2EMWbPxTulisY+whizp7IjzxLbyn/+859ox9mKFSuwaNEiVKpUCZUqVcLNN9+MPn36oGrVqvjoo49w9dVXo27dusjJyQGwdUda9+7dcdFFF2HMmDHYvHkzBg4ciLPOOiscxHLOOefg5ptvRv/+/XHNNddgyZIlGDVqFO66665i1XW7d0oNGDAAS5Yswfjx47f3EgC2Ch6yUJduyzbGmGyjJP66Ua5cObRq1SoKacrPz0dubi7at29f6Hfat28ffR7Y+tcK/nzqhdQHH3yA1157LS0EaGdiP2GM2VPJtr+AZyP2EcaYPZWSeJZYsGABWrRoEcJZBw8ejBYtWmDIkCEoU6YMFi9ejJNPPhmHH344+vfvj1atWmHGjBmRZMLYsWPRoEEDHHfccejZsyeOOuooPPDAA6G8YsWKePXVV7FixQq0atUKf/jDHzBkyBBcfPHFxarrdu2UGjhwIF544QVMnz49ivOvWrUqNm3ahLVr10Z/4Uj6y/51112HwYMHh/z69etRo0YNrFu3LsTFsm6DdobGn3Lst8ZxqiYOHzmtxzwmxVJrHDPHb6vmkWodcF41cPS4adV8YFQXgdtXY3D1OryVLknzCohjl/UvT9zWGous983l2kaa537SGGy9F85rm+hY4XGkOlt6b3wEsOp3qbYJ11f1Xjivf/XTHS16tCyjYth8LR2POu5Z40PbU7V2OD5aP6ttlqR5plosHFevMfiZPgekj0fuJz3+XDV9+Fqqc6L3wuUpjZAkTamSYvDgwejXrx9at26Ntm3bYuTIkdiwYQMuvPBCAEDfvn1RvXr1cOrGlVdeic6dO+POO+/ECSecgPHjx2PBggXBeWzevBmnnXYaFi5ciBdeeAFbtmwJf3muVKlSoj5acSkJP7H33nsHfSO2Bam/3qTQOczHF+vR1c2aNYvyb7/9dkirDgXrPNSvX7/QuqdgW6t+S+0l6zmpno/aES7X4591HrLOg9ZB7Q8fdXz00UdHZbpbgee0ajdwW6ud1XnIddAt37qbj+tQ1LHX/FnVHVF9LH5JO3369MQ68Ge1jZYsWRLl2Z7qEfM8dovSvOI6aJ/pC2bWsCmqv9kG6lhWDZPq1atnLNM+5c+qTVW7zKhP4fmzYsWKqExfQPAY1PmjR5dzHXTtpPN92rRpIZ3SyClKu9RkpiR8RO3atYMdZPuj4zSlXZWCdYV4DAPp9o/XZxMmTIjKeA3Tq1evqEzHW5MmTUJa50q/fv2iPNsBfpYB0te+rGvVoEGDqEztCz/PqI5Mt27dkIlFixZF+c6dO0d5lim48847ozKeV0OGDInKLr/88ijPvl3X26oxxLph2i/ah2xTWP8RSF/zs71RrSr1uay927Nnz6iM9RaBuM+feeaZqEzbk1FtKl1PMHPmzInyrPWltlxDZXmNrfd92WWXRXluX31u02eUTz/9NKS1/VTP7fTTTw/pRx55JCpjv7p48eKoTHXWWEtN1xo6f3hdrGND9bF4LZTq7x9++CHSiytpjjnmmMQXWa+88kqR16hUqRLGjRuX+JmmTZtixowZxa4fU6yXUgUFBbj88ssxceJEvPHGG2kvAVq1aoW99toLubm56NOnDwBg2bJlWLlyZca/7JcvXz5twhtjTDZTEltuAeDMM8/E119/jSFDhmD16tVo3rw5Jk+eHB6WVq5cGS2uO3TogHHjxuGGG27A9ddfj3r16mHSpEkhLGLVqlV47rnnAADNmzePfuv111/HMcccU+w6KvYTxhjj8L1M2EcYY0zJPUv8WijWS6kBAwZg3LhxePbZZ7HffvuFN6EVK1bE3nvvjYoVK6J///4YPHgwKlWqhP333x+XX3452rdvX6zTMowxJpspSUcycOBADBw4sNCywo5sPf3006O/JjG1atX6xR2a/YQxxvilVCbsI4wxxi+llGK9lEqd0KR/TX/44YdxwQUXAADuuusulC5dGn369MHGjRuRk5ODv/3tbzulssYYkw3YkWTGfsIYY/xSKhP2EcYY42cJpdjhe0VRoUIFjB49GqNHj97uSgFbY79Tsf4cr60x/grH5Kr+g+oXsO6Axm9z/KlqL2g7cMy4xspq/DvHLbNWif4mkK4dwiSdLKL1Vd0ovm/V/1BdniTtCL5XjWFWDReug2oV6Xe5fVUj47DDDovyrOekdVcNDdYOUT0BjU1P6QoB6bpGK1eujPKs/6JtxPHROv5UM4P7X/tMtX6437R+uoWd20HbROvL8yB1PHMKbV9uM+1T/R0u1/HJ9dc4f9WN4n7R9tQ5we2gc0nnO7dvavwlaUrZkWSmJP1EmTJlgkYM62roHC3KFzCqRcDjQPUOWN9CdRPUpvA417mlujSse6N6EWoT2daqXg7rWSiqo6h1ev/990NafRPPQyBuF9VfYbuhoTfqJzJdE0j3E6yFofZH/S7bAtauAdJ1Pbi+qk2mfuPwww8PabXRqlPBeR0bSTqKarvYRmqbJGnCaYiU2mgeO3qfel2eXzq3WrZsGeVZa0bHp+o98ZjUOcpaHqqLo2OX21D9lvY3a4uozVcd0lQYNPDfOat9yfilVOGUpI+YPXt2mP8dOnQI/1916Lp27RrlWQeVNW8AoEePHlGeyxs1ahSVsV9QfRwdm/xZXQM++uijUf5///d/Q/qJJ56IytRmdOzYMaQnTZoUlelc4nWU+povvvgiyrN91LWb6vodccQRIc3ahkBsk//4xz9GZa+++mqU535SPSzVlEpJFQDxPAfS9bxYQ5HrCqQ/d/C9svYYAJx00klRnv2oasPWq1cvyrOf1bUva/WoHdV+Yr+ktGnTJsovXLgwpNXeqR/t1KlTSOt656233orybK/VzutY4ftR/6x51jVSCQpeRyVpbwKxP9a66zMVjw29LpcBwOTJk0N65syZANLfCzB+lojZLqFzY4zZk7EjMcYYk4RfShljjMmEnyVi/FLKGGOKiR2JMcaYJPxSyhhjTCb8LBGTtS+lypcvH7aQ89Z73SqtoUCffPJJSOt2PQ054G3nSUdAJoUFAXEolZZpGAlvU9TQOT1ik7ct6jZ93V7I39VtldoO/Lu6hV/DSLj+upWTQy805ECvw+EAGpahR2fz72jYAG+p1s9y3wPp/c1hMHovGoLA7Ttv3jxsK9qe3BfaRtoOSaFpmuf21PvUsczbgPX4cw0x4fpqH+p2cq6/zstVq1ZFed62rnXgsa1blvW6PB40pEiPUud70e2zmuff1dCVwrAjyQ6++OKLMJ54K7xuZ1+2bFmU5/mkIRU6JzjEQu0P29IWLVpEZRpawFvjdaxqKDfXX4/7VjvCdk1tv4ao8JHjRc1ZDvlQ26q/w1vaf/e730VlScdnczg7ELe9hrbofbNvUruh98K2Srfb6zHt3GYa3qx14hAV9fV6rxzqotfhz3I4OJAevslh32qTNSSTx7b6ED66GojbSMND9Bhsvhf1Y3rkOI8z/ayGcfCaQuchh+Zo3TW8itdOOtf42HAgvjf1TRrOx74h5evV5zN+KbXradiwYejX3Nzc8P85FAlIn0u8RtC1us4lnr+6Zv3qq69CWu2Srs15rmjYUv/+/aP8m2++GdIacn7JJZdEefY9OqbVvvC80+crDT/T8GZG12fsT3T9zeFTajePPvrojPmkEHkgtrMaKq7rW557Og+1fdmuajic2gP2h2r3dVzxGOzcuXNUxj5Y/Z32Kdtvtbm6FmLU32loJ/u7L7/8Mirr1q1blOcwO+1TleHhe9Prargch1JyaDgQh2hqiKhe57zzzgtp9W/K1KlTQ1rDfDUclt8XNGvWDMDWZ5wJEyYUem0/S8Rk7UspY4zJVuxIjDHGJOGXUsYYYzLhZ4mYorcEGGOMMcYYY4wxxhizk/FOKWOMKSb+64YxxpgkvFPKGGNMJvwsEZO1L6X23nvvEL/PMdka46xHWHJMscZ2a2wtxyNrTC7nNW5Z42M59lx/U7U3WLNA70V1HDg2VXVPFNaS0NhZPQKZ66D3rd9lfQvV/2CND9ViYN0LIG5DPb5Z25cnnGpHaCw1xx9rnL+2GbevXlf1BPi6qjGkBoG1RPRe+Loaa65jl8eOtpHqRvHv6LjRMci/q2WqEcDl+lmNwee8tj3ryGj9Vc+J54HOF21PvpeijldOOuJ8Zxj13dkx/FrYd999g12fNWtW+P+qWaC2n8t1XCdpxNSqVSvK83dVL0RtCs8n1WjS67IOjtoq9od6XbW7Xbp0ifJcrvpD1atXj/I8Z7RMfSD7Kj0KnL+rc1/9ButAqD6jznfOa9urDhcfy612go/EBuJ7S9IdAWIbo9pF2kacV41I1vLQ48e1Dvybavt1TcFjQzWvVNeFtR31SPTatWtnrK+uL/S6POZ0faF2meep9vdLL70U0tpG2g4891SLTOcea9+oFp1qrLAGUOo39beVkvATo0ePxh133IHVq1ejWbNmuOeee9C2bdtCP7t582YMGzYMjz76KFatWoX69etj+PDh6N69e/S5VatW4ZprrsHLL7+MH374AXXr1sXDDz+M1q1b/+L3szM58sgjwxjkvtc1lmoOsfYYa9UAwMSJE6M86wapFhBrDqk20QcffBDleZ5NmzYtKtM5yfNV15Jz586N8kcddVRIN27cOGPdgVifTX2E2m9+ftD2ZA04/axqAbHPqFmzZlSm45j9n35W9X9Zl0u17lTPi+e6+iVd37Kd1XGj6wf2C9p+auNY70n9FK+p1Y5qP3Fenx10LcT2SXXMdBx16NAhpLWNXn755SjPfkDXLKqbyGNONZu0j5cuXRrS2oc8v/U+1T9zW6uN1nZ49913Q1rXJfpZHq+p+9I+UPws8V8cvmeMMcUk9deN4v4zxhizZ1ASPmLChAkYPHgwhg4dioULF6JZs2bIyclJexBMccMNN+D+++/HPffcg6VLl+KSSy5B7969I7Hp7777Dh07dsRee+2Fl19+GUuXLsWdd96ZJj5vjDFm+/GzRIxfShljTDGxIzHGGJNESfiIESNG4KKLLsKFF16IRo0aYcyYMdhnn33w0EMPFfr5xx9/HNdffz169uyJww47DJdeeil69uyJO++8M3xm+PDhqFGjBh5++GG0bdsWtWvXRrdu3dJ2IBpjjNl+/CwR45dSxhhTTOxIjDHGJLG9PmL9+vXRPw2zT7Fp0ybk5eVFIS+lS5dG165dMXv27EK/s3HjxkjmAtgaijNz5syQf+6559C6dWucfvrpOOigg9CiRQs8+OCDO9ocxhhjCD9LxGStptR//vOfoDfA8aeq06GaMxyjq45c9TY4zlPjY1nHQfVJVq9eHeU5vli1IjT+lDVz9t9//6hM46FZg0J1ET777LMoz+UaX6zaQGvWrAlpvTeNY+bFi04Ebl+N39UYd46V15hrrQNrVOh9c5w/EMdor1u3LirT3+G+0LZWbS2Oh1bdi48//jjKsx6M6nZw+2mbKKyXpfVL0kTSeHfVuOA6qD6Nzh/tR0bnE49frZ/GzrPegI4jrQOjc5bj/rVM5wTH4H/zzTdRmdaBx0qqH7Rd9fvFdQy7syPZVRxwwAFhzPJ4ULur2gOsQaR6TqpPxL5BdfX4N1X7R30K23Odozp/2Jap7oRqNvHvqp6P6nywL1Dbqnp9PF7ffvvtqEzvjTUh1J7Xq1cvpNUG8veA2Cdr/XQ+slaL1l3tebVq1UJabaBel33V8uXLEz/7xRdfhLSuTdSXcv+rRhP3i64vVAsjScdMP8vjSNcBqpfE9pLvC0jvC7b9qvmhcH11baJtxmNO/Sxr1CT5OP0d7TNdo/G11McdfvjhUZ79ss6Bwiiun0h9VjUZhw4diptuuint89988w22bNmSNueqVKkS6agxOTk5GDFiBDp16oQ6deogNzcXzzzzTNTHH3/8Me677z4MHjwY119/PebPn48rrrgC5cqVQ79+/bb5frKBZ599NowP1sNSLTm1nbwuOf3006My1Ytju6bzntezqjelekRch6L0h3hs6nX13qZMmRLSquejfov1c3Ru63f5eYZ1WIH0dmBtwaeffjoqa968ecb66HV5/mobNWnSJMqzxpBq/+gam8NX2V8AQLNmzaL8U089FdInn3xyVDZv3rwoz2uPBQsWRGXap6wVpX6gV69eIT1ixIioTPW72B6oz1Vbwdpkuk5ivT0AmDFjRkg3aNAgKlPdNV6PN23aNCrTPmbNM9XL0v7nvNpJXu+oLde2Zl0zXT/oGou1BnUtpD6Y/WrK7qjPYfwsEZO1L6WMMSZbsSMxxhiTxPa+lPrss8+iF3/6kn1HGDVqFC666CI0aNAApUqVQp06dXDhhRdG4X75+flo3bo1/vKXvwAAWrRogSVLlmDMmDG/updSxhiTrfhZIsbhe8YYY4wxxmQB+++/f/Qv00upypUro0yZMtHud2Drbnjd+ZPid7/7HSZNmoQNGzbg008/xfvvv4999903OtHw4IMPRqNGjaLvNWzYMG0nuDHGGLOzyNqdUnvvvXcIaeDQmqSwGyAOg9Ay3erJ27p1aztv3dVj6jUkgq+jIUUaNsTbI3VrpG4H5y1/GuKkWxz5u5lOXSnsWrp9WLepcrvowohDBbSNdOsk34v+pm6V5Xv7/PPPozLtfw690XBI7SfeTqr9rVuNuY30OE/9LNdJr8v3rXXX7aTcLhpyoGF1vN1UQ1UU7ouk4+6BeP7odXVs83W1TfTe+Lq6bZrvTX9Dt9VyqIXOLT3amLcta3iHjlfu7235q7T/upEdfP/99yHshMeYzlkNG2LbpTZGxz2PHbXR/DCoD4G6VZ/Hsto8DQtkO6KhXhrCzHZPj7vXrfs8/3WcH3300Rmvq9vPP/zwwyjP7aChLRwCp/NZ+4VD69QGqs/jLfbaZxwOop/VB3i1rdOnTw9pDWPjUEQgtjnaRmpz2L6rf+TrcPgMEIe9AHEIja4LtB14vaH3rbaWx5zab/0sh91paJ+GR/KY0/pqGAf/DssiAPH8Vlv/zjvvRHlex+gY0/HJ19XQFm0znhPqQwpje3dKbSvlypVDq1atkJubG8J78vPzkZubi4EDByZ+t0KFCqhevTo2b96Mp59+GmeccUYo69ixY3RkOrB1HmuIzq+Bpk2bhjm+ePHi8P/VBietbx555JGoTNuBx7WGTXII3PPPPx+V6Vr4xBNPzFg/9VNsF7SvdBzzfFC7qr6nRYsWIV1UCCG/yFRfo/Ns/vz5IX3HHXdEZVwnbSMOswKADh06hPSbb74ZlWn4HtsQDW3W+ct1UFuu4fXcT7rW0BC4uXPnhjSHgRVG48aNQ1p9GN9rq1atojJdI/AYfOONN6Iy/S7/TibtuhQ8JvUkTvVbPCd43gHJ4dZq93VdwuF72i9JYbQaKs7hkccff3zGugNxKHlS6C4QhyqmDobQZ33GzxIxWftSyhhjshU7EmOMMUn80i+lAGDw4MHo168fWrdujbZt22LkyJHYsGEDLrzwQgBA3759Ub16dQwbNgzA1ofkVatWoXnz5li1ahVuuukm5Ofn4+qrrw7XvOqqq9ChQwf85S9/wRlnnIF58+bhgQcewAMPPFDs+hljjCkcP0vE+KWUMcYUEzsSY4wxSZTES6kzzzwTX3/9NYYMGYLVq1ejefPmmDx5ctgts3LlymhHwU8//YQbbrgBH3/8Mfbdd1/07NkTjz/+eLQTsU2bNpg4cSKuu+463HLLLahduzZGjhyJc889t9j1M8YYUzh+lojxSyljjCkmdiTGGGOSKImXUgAwcODAjOF6Gr7TuXNnLF26tMhrnnjiiVGYkjHGmJ2LnyVisval1Nq1a0OML8d6q2aCHg3MscCq/6Hxpxw/q9fluFaNRdU8xxQXFZPLn9W4WtX44DhUjYfW73Ics2r2aJ14QGvsrMbHcpy1ajaxPoj+hrY934t+Vo9+5t/R+9ZjUlnHhY+/LqwOHA+vcfUaO89tqJoUqhvF96btyXobqomiceusk6F6Sap7wuNI6666LVwH1QTQccTX0s8mHWtaVKw8t4u2A6Nx4Dq/+d60H5K0tfS6OpbVNhSFHUl2sHbt2mBP2Fbo3Fcbw3oSrIsBpGts8NjW439Z10NtkwoFsz4Ra+EB6ZoLbNfUpqifYJutQsRq57hddM6++OKLUf7MM88MaZ2HOvf4aOZPP/00KuOjy1XvUNuBr5OXlxeVqZ4Ttz3rlQDpWlDcN6qBNGvWrCjP7asaJWonuJw1C4F07QnWglIfzbojeuy6/iaPT7XfqovDdk71kdReFme9weOMjxQH0nUp+Sh29WtaB87r2GX/o3owOo74XtX2q94O+zz1cbqm4Hb46KOPCv0OU1IvpUxmqlevHuYF22+1ueoHeC6x1g+QriPE80XHNOvvqR6gas2wdtWpp54alek4Zjum2lSq1cbf1TmotohfRKrNUO22+vXrh/RTTz2VWF+ed08//XRUdsQRR4S06iOldHlSzJs3L6TZXwD/nZMp+FlN2yRJh0v9/GuvvRbl/9//+38hreNI9cb4WVJ1J9VvsW5U//79o7KpU6dmvA6XAbGdatmyZVSmzwe8NlI9LNZv0uuyTiOQ7nu437Rf2rVrF+VZd5LTQPrzV8OGDUNanyV4vOo413ZgbS1dN2n78vjUcZPkp/75z38CSH9GY/wsEZO1L6WMMSZbsSMxxhiThF9KGWOMyYSfJWL8UsoYY4qJHYkxxpgk/FLKGGNMJvwsEVO8mBVjjDHGGGOMMcYYY3YCWbtTaq+99gqxmqxfofGwqk9UHL0a/qxeh/Oq6aHx5Bxnq1obqsuzefPmkFZtKtXbqFatWkirppDeC7eLxrjqW1Wur95bkiaW1oH1ForqB46zVU0P1atg/RJuLyCO7QXiuGHVWlFtE+4b1aRQ3Q6OTdaYe42d5nh+1RNgTQ+9F20zHg+qiaPx8NyG2n7ap/y7qqWk1+Wxo/XTscz3quNR61CpUqWQ1rbnzxal7cRtr3ofOs65PXVeap7vNZVO0qjyXzeyg7333jvMFR7nqifA4w+Ix3JRehw8XnWusc1Wu6B2uHnz5iGtc4v1kYBYy0H1fbS+bGu1THWjWBOEtX4AoEGDBlH+2WefDWm9N9VI4PtRO5ykWaGwHpH+ptpP/h29F9UE0X5jtH1ZT0LHjdoE9g2qSaP+kn9HNUp69eoV0qpZofaS/aOuIVSjhj/L2iZAuh/+9ttvQ1p1kpJ0zFgLEUjXIeH662e17Vl/R/ub21NtqdaX10OqO6N+g+fp559/HpWpz+P2TdUnyWd5p9SuZ8WKFaGvuD91jaLrRS5v06ZNVKbrHdaw02cUXsvpeFe7z/ZZdfFU75Xto+oY6b1xnXieA+nPHXfffXdIq0/Q+fDwww+HtIrn9+zZM8qzrXz33Xejsvbt24e0avxpG/Xo0SOkb7rppqjs2muvjfKzZ88OafXrHTt2jPKsYahjoW/fvlGe9QO1TVgfEIj1yLSttX2POuqokH7ppZeiMn72Ua3DMWPGRHn2J/r88t1330V5fp7VcaMHHUyfPj2k1ebqvXzyySchzfqUAPDMM89Eefa52t/3339/lOe+0HXIAQccENLqa9Tf8ZxQX60apJxXbSpts5kzZ4Z0Sh9tZ+oOpr6zu5K1L6WMMSZbsSMxxhiThF9KGWOMyYSfJWL8UsoYY4qJHYkxxpgk/FLKGGNMJvwsEZO1L6V+97vfha3nvEVPt2BqnjtLt7brFj3eiq/b8pOOnld4K69usdWjtPlIWN1GqyEGHBKh4Vy6JZO3k+qRx0nf5e2OhdWft+1rGfeLbmHX47G5TjqhdCs095v2oX6WQxK0/bSN+Fq6xVqPtU7qcz36na+VdNyuhk9om3E/aRvp+OSxoduHFd7mraGn2g5cJw1d0e9y/2t4h/Ybf1aPSud+0z7T7bkcPqHtqSFRPPe0rbU9+V5T89Lhe9nPN998E8YPb2/Xrdo6nzk8V8eYhg1xOJKGSfB2fB0vWgfeTn7QQQdFZTo2OMxNQ/A0NI3nTK1ataIytVV8XT32WLeY8zxVu6Z2mK+rYXc893RbvG595/mtIXl6PPmECRNCWo8R1zDBevXqhXRSmC8Qt+GKFSuiskaNGkV5Dk3T62g/cUiIjiPuJx2PGg7H7anh7NrffK9FHZ/O9lTtsI5B9hs6bnSs8LpBw/o5ZEZ/V8MkeK5pSKP6QO4Lnc86T3m86pzVEFwO70u1p65BGb+U2vUsXbo0+AgOoeZQYSB93HKYp44DtS/8XQ1j6969e0i///77UZnaAQ7vU9ujv8k2T8PhdK3GtlRDfNXO8njmEG4gDp0D4nZRW6RzieeOrt24rTmEDYhDegFg+fLlIa0hgnpvHOam/oPDrACgU6dOIa22/OWXX874WfW5l1xySZQfPXp0SBcln8Ghf2qn+NlRQ7xbtGgR5efMmRPSOs5feeWVKH/RRReFtNp9vW/uf72O2i4eV+r3O3ToEOWffPLJkOb5AqSHVPO6ZNGiRVEZ+zQOmwSASZMmRfn+/fuH9LRp06IynZfsXzRMUeF5mWoTnY+MnyVisvallDHGZCt2JMYYY5LwSyljjDGZ8LNETLFP35s+fTpOOukkVKtWDaVKlUp7+1hQUIAhQ4bg4IMPxt57742uXbvigw8+2Fn1NcaYrCDlTLb1356CfYQxxmzFPqJw7CeMMcbPEkyxX0pt2LABzZo1i7YkMn/9619x9913Y8yYMZg7dy5+85vfICcnJ1F93hhjfk0U14nsCc4khX2EMcZsn5/YU7CfMMbs6fhZIqbY4Xs9evRIiytOUVBQgJEjR+KGG27AKaecAgB47LHHUKVKFUyaNAlnnXXWNv9O6dKlg3aCahkxqmWTpIugugP83SRdEdUjUW0q/q5qL6gD5bzWR3Vv+L71eFgdlKyxoNfRPMdLa4yzHlnKuhiqP8VaQHqf+pvcRvpZ1QKqVq1aSCcdX6rf1X5SfQ2OTdbYc40h12NJGf0dHmca9//1118X+rnCfpN1WjQeX3UxuO21THWiNM/o8disa6UaCxrjzn2sY1k1Z5J0zHiMadvqdbm+OmdVv43HmfaL6rQUpltnTanto6R8BLC1X1NjlrUndGyobgbPbz42GkjXiOC5pvOFdaJUy081hZh///vfUV7nMNs11Z3Qccm2X3WDdK6xpo9q8E2dOjXKcxuprdJ75Tqof2R7rtdRvQi+b7XRel3WfXjvvfeissWLF0f5888/P6TVrqnd0D5m1C5zG6qui/of1vbQOrDWjd5306ZNo3ySxqb2C9scbSPVdWENm3bt2kVlui5gDT7VrNSxzbZX21rXH3Xq1AlpnRN83/Xr14/KdBzxd7U/dU7wmNQ20fHKujmp9ZmudRiH72WmpPzEt99+G9b68+bNC/9ftS2POeaYKP/GG2+EtO7QUr0z1itS/8F+QMetakwtWLAgpM8444yoTOfV9OnTM5Ydd9xxUf7pp58OadXz0fHLOn9aX17PArFN1rGr7cD+Wa/L81U1uXQOsv6r6g9xnwGxf9a1pD5XTpkyJaQ7d+4clWl933777ZBWu6/6SWz/itJp5T7V8chrVl2z6Hjksa32OScnJ8qzzdP2U60q3s2o2pFqV1977bWQVv1KnXtHH310SOta/fTTT4/y8+fPD2kdy/zd1q1bR2XqG3nOqI5ZmzZtojzrj+k6RJ9Z+Fk99eyV9CLdzxIxxd4plcSKFSuwevVqdO3aNfy/ihUrol27dmmTKMXGjRuxfv366J8xxpjdj+3xEYD9hDHG7Cn4WcIYY3YORYVKM5dccglKlSqFkSNHRv+/Vq1aKFWqVPTv9ttvjz6zePFiHH300ahQoQJq1KiBv/71r8Wu6059KZX6y6C+kaxSpUraXw1TDBs2DBUrVgz/9C+9xhiTbXjL7faxPT4CsJ8wxvz6sI/YPvwsYYzZEyiJZ4miQqVTTJw4EXPmzIl2tzO33HILvvzyy/Dv8ssvD2Xr169Ht27dcOihhyIvLw933HEHbrrpJjzwwAPFqutOfSm1PVx33XVYt25d+PfZZ5/t6ioZY0wifilVsthPGGN+bdhHlBz2EcaYXxsl8SzRo0cP3Hbbbejdu3fGz6xatQqXX345xo4dm1HyZb/99kPVqlXDPw6JHTt2LDZt2oSHHnoIRxxxBM466yxcccUVGDFiRLHqWmxNqSRScaNr1qzBwQcfHP7/mjVrIs0Epnz58mm6UMDWuOZUw3McrmrVaDwnx3ZrDLFqF3FMKWtiALE2B8dYA+mxtFw/jRHWz3LstOpBqL4CX1c/q3UqVapUSKueimpUcCy16jbwdfR39LOsD8Gx20B6nDq3b5LGkaJjQ+vAv6OLEI1x/vbbb0Na9VS0zVh/Q2PPNeaZ20H7ieuvbav1Y+0LbT/9ro57RuvLbabtqcaN55f2qf4mjw1tP20HjltXXQK+jraJwu2gsfIK11djunVecn1TczjJ8JdkHPjo0aNxxx13YPXq1WjWrBnuuecetG3bNuPnn3zySdx444345JNPUK9ePQwfPhw9e/aM6jF06FA8+OCDWLt2LTp27Ij77rsP9erV2676FYft8RFAsp9IjR/ub9UsSNIxU70I9RNsr3ScH3TQQSGtmj36F322P1o/tUc8VnTssi4UEM9Z9QsNGjSI8qxlpHNUtSZYu+Hwww+PylTrj+el2gn+TQ2pURvDY3DRokVRmfpWbjP19Ty2tA563+r7WatK22/lypUZ66B+TbUn2E+odlHSukVtFWuz6JzQ3+Tr6nV0fLIepo4jrROPSb2Orje4XXTcJ63JtI14XKmv1zHH2l+1a9eOylRPkMek6rVpnu87NV+SNE+tKbV97MxniVSoCRDPZ53348ePj/L8O6y3BqRr1jFqG9neqI9Q+3fqqaeGNPsLIN0G83xVu6QaPn369Alp1bN76623onyrVq1CWrVV9buM+g/1uawbpDpMbBv1GU/twDXXXBPSuvMjpT+WgtfUqstbs2bNKM+/+8knn0RlunOE+0LbT/X42Mapvp36l44dO4a0jhW2yaqzpFpQrKGpfabPUGy/ue+B9L7gPtV1CesBAsCrr74a0suWLYvK2rdvH+VZR0zHfZMmTTJ+Vn+T57+uH1SbjNtI5/OTTz4Z5QcMGBDSr7/+elSmmo/8fJjS1dJ1I7MjzxK6nspkA4siPz8f559/Pv70pz9FuonK7bffjltvvRU1a9bEOeecg6uuuiq06+zZs9GpU6fIF+fk5GD48OH47rvviny2S7FTd0rVrl0bVatWRW5ubvh/69evx9y5c9MGoTHG/FopqZ1SEyZMwODBgzF06FAsXLgQzZo1Q05OTprwcIpZs2bh7LPPRv/+/fHWW2+hV69e6NWrVyQOuitPNbKPMMbsKXin1PZhP2GM2RPYkWeJGjVqRCHLw4YN2646DB8+HGXLlsUVV1yR8TNXXHEFxo8fj9dffx2///3v8Ze//AVXX311KF+9enWh4dapsm2l2Dul/vOf/0R/qVuxYgUWLVqESpUqoWbNmhg0aBBuu+021KtXD7Vr18aNN96IatWqoVevXsX9KWOMyUpKaqfUiBEjcNFFF+HCCy8EAIwZMwYvvvgiHnroIVx77bVpnx81ahS6d++OP/3pTwCAW2+9FVOmTMG9996LMWPGoKBg555+Vxj2EcYY451SSdhPGGP2dHbkWeKzzz6LIqy2Z5dUXl4eRo0ahYULF6ZF5DCDBw8O6aZNm6JcuXL4/e9/j2HDhm3X72ai2C+lFixYgGOPPTbkUxXt168fHnnkEVx99dXYsGEDLr74YqxduxZHHXUUJk+enBaeUBQbN24MIUy8hVq3lWvIG/+1X7cp6vY93s6u4VK8hTApbEmvo2jIAW+D1y19el2uvx5FrSEIvEVe66P3xlv89ShZ/S63p2535vAp3Rqr1+G21/vUUAve6qlhAzppuF10q71uPeXP6k4THSt83zputN94C6VuNeZ20bAb7UPO69HZus2b21A/q3ON+1+Nn7Yvh4zqdbR9+e23viFPCvfQOctzRH9Dwzv4vjVcRuca97eOOQ394/qm5kd+fn4U5sWUxEupTZs2IS8vD9ddd134f6VLl0bXrl0znkA0e/bsyHkAW7fQpk7bKOpUo53xUqqkfASwNVQiNW/YMSb5BSAeZ7q9Xecah+fodXVOM2o32O7qNn6dLzy2dYs2h5cBcTiSzgm1c3y0uW47V3vEIey81R1In08cIqVzlsMQdGs47+ADYjusv6nw8e5qv/WIZ7bZ6kMaNWoU5dkGaqix9im3mdZB+5T7Qn0phwqpndAjxvm66ts1rI3tnI45bV8eZzpfdG5yH2vIYN26daM8j0/1ydpm/F2dWzwP1X5rv/DLDg5zApKlBoryKXzfqX7RzzB+KZWZkvIT9erVC+OF+0rH4gknnBDlOQxPQ1J1vPF1dXwtX748pDW8TMNZH3vssZDWeaRhTTyu1Z7ozgT2cXovumbl0D8OwQLS12etW7cO6U8//TQq+/zzz6M8rxF1Dc0h9A0bNozKxo4dG+XHjRsX0iqlob5yxowZIa0hmPrcwSF5al+SZGM0xHHatGlRnseDrh/Uv7At0utwaJ8+t+nYZZ+R9HwKxL78/fffj8o0dG7q1KkhffPNN0dlU6ZMifIsbaDtqf6F/fXjjz8elWl4dOoPtADw6KOPRmV9+/YNaQ7zA7a+fGHYlteqVSsq02eq5557LqTVr2v/87ok9Vm1F8yOPEvsv//+aWOquMyYMQNfffVVFM66ZcsW/OEPf8DIkSPTQllTtGvXDj///DM++eQT1K9fH1WrVo3kAoD/ygdoOHESxX4pdcwxxyQ2YKlSpXDLLbfglltuKe6ljTHmV0FJxIF/88032LJlS6FbYnXxkCLTFtrUInV7T78rDvYRxhjjl1JJ2E8YY/Z0SlKftjDOP//86I/UwNY/ZJ9//vnRC0Bl0aJFKF26dHj52L59e/zv//4vNm/eHP64M2XKFNSvX3+b9aSAnSx0bowxJhk9qnro0KG46aabdk1ljDHGGGOMMbsdRYVK627ivfbaC1WrVg07GGfPno25c+fi2GOPxX777YfZs2fjqquuwnnnnRdeOJ1zzjm4+eab0b9/f1xzzTVYsmQJRo0ahbvuuqtYdfVLKWOMKSYlEQdeuXJllClTptAtsZm2w2baQpv6/PaefmeMMaZ4eKeUMcaYTJTETqmiQqWLonz58hg/fjxuuukmbNy4EbVr18ZVV10VSYVUrFgRr776KgYMGIBWrVqhcuXKGDJkCC6++OJi1TVrX0rxMa4c85wUyw3EMbmqHaGaGRw3qg+GHAOrA0BjOPk6GtutMdhcX62f1kHry2g8NP+u6jRo/DaX670kaZ1oLD9fV3UltM34NzXGWX+T70X1vDRe/6OPPsr4WdXh4vYu6thZHkfap9q+rEOhcf+s26FjVfuFP6sx46rhwvVnDRQgve35XvQ6+lkec9rfWn9+MaL11b5I0lLj2HMt0zpwW6s2gsZ687hK0uQC4j5Oxbvr3GVKIg68XLlyaNWqFXJzc4O4a35+PnJzczFw4MBCv9O+fXvk5uZi0KBB4f9NmTIlnFjEpxqlXkKlTjW69NJLi3U/2UB+fn7oJ/YNOjZUu4E1kHT+qJYNa+Ik6TmpboLqFPB40fGn84V1ClRTiG2eonZYdT54jujLS9V7Yjut2lQ6T1l/RecFH9usGiq6a5A58sgjo7xqlLBen/qUww47LGP99L7Vl86ZMyekddu5amxwHdq0aROV8dgAYt+gv8njQe9TNbrYr+nYVZ/Hdlk/q7Cf0P7Wsc12WP2C+kfuCx03OtdYf0eP++Y5rP5a24zXUjq3VHeL20g1uvQvyHzdlH9JWqf5pdSuZ8uWLWFe8BjSucxaRUDs/1V/T8ctzw9dW55xxhkhreN/7ty5Uf7MM88MaZ33bMMA4O233w5p1RRSu89rSx3jqgfLGjI5OTlRma5vuY6qrTNhwoQoz+2ic5LvhbWdgHSNKV7L6fxU3Sgu1/UhrzuBWE9Jw5lU2oDtY7Vq1aKyxYsXR3n2J/qArm3GPkN9OY+5WbNmRWWq0cTll112WVQ2fvz4KM9rUdYVAoBnn302yvN4eOWVV6IyHXO8dtexrH3K7XvSSSdFZQsWLIjyr7/+ekhr+7H9VH1AHcvsM3Tto5qtvG5p2bJlVKZrTb7X1NhIOtm6JF5KFRUqraiOVMuWLaNxnImmTZtGOm7bQ9a+lDLGmGylpOLABw8ejH79+qF169Zo27YtRo4ciQ0bNoRY7759+6J69erhKNgrr7wSnTt3xp133okTTjgB48ePx4IFC/DAAw8A2Ppi1qcaGWPML49fShljjMnErtaUyjb8UsoYY4pJSTmSM888E19//TWGDBmC1atXo3nz5pg8eXIQKl+5cmX0l88OHTpg3LhxuOGGG3D99dejXr16mDRpEho3bhw+szNPvzPGGFM4filljDEmE34pFVOqIMvubv369ahYsSLq1q0bwuKStkfrSVa8xVG/p6F/vM1cQ+l465+WaegFb8nVbYq6ZZ6Pt0w6Mly/q9tHdfs//65eV48853J9ENXQBt6WrCFHvJVXNW50CzNvX9QQDg0N4PbVttatxxw6oFs5FW573X6dFC6n40i3YnKIh27l5G3Kei9639yHeiSpjituQw1/1PAJ3qasdU+aExoKoluu+XeLeqGRFBbI80u3WOuc0LGcBPe3jrkkUvdVUFCA77//HuvWrQtjP2WfKleunDYWiyI/Px/ffPNNdD2zfaT64Z577gnziENrNPRS3RzPRZ0v2jc89zSUl8PG9Dc1pIzthP6mhiFwiNGqVauiMvVH/F0NN1O7sXLlykLTQPoc4W3qeh2172yvNJyBfVdRYXY8v9UWJB2fraEYarvY5mi4itp+DpPREAAN32QbrqEtamu5z7W+7DfUnmuoGod46JHoei/chmq/te3feeedkC5qDcHzSf2Y+mHucx0b7733XpTntZSGOrEPUZ/M4bhaPw1F1BAVHtvafjqneTyk2vbHH3/EJZdcslP8hH3EziPVB4MGDQq+gW1e27Zto89rP7E/0XWI+gEOd9HxlgqdB9JDXfX5hcP3eD4CwJNPPhnlOby1Y8eOUVlubm6Ub9WqVUir7dY1K495na+6Lp06dWpIa/iytkODBg1CWn0a11/DnhcuXBjl+VlD7YD2Ifeb3rf6u9atW4e06uyozWCfpmNDfUSLFi0yXldlJVjXU8M1OYxN1wtaB14/nHLKKVGZ+n32Nxoyr1IBjRo1CmkNmdbP8vjU/tb1GI85fQbVccX111Ok+brqs3Q9weM+yScA8RhU7VVtB/5s7969AWyd9xdccIGfJbYB75Qyxphi4r9uGGOMScI7pYwxxmTCzxIxfilljDHFxI7EGGNMEn4pZYwxJhN+logp3p4xY4wxxhhjjDHGGGN2Alm7U2rDhg0hzpJjuzXWU7WBOLZW47c1/pivq7HSrKmgZaozwfokqpejuggcx6y6DZrnuGWN+9b4XdZx0NhpfavK2hJFaQyxrpXG0XMcbFFaDBw7rTHD2p6soaFxwdr/3N6q2aRtxvfGekNA+ljhco1FVg2NJB0mvo5+T7VD+F5Un0S1WLjftM90zHH9dCzzHNDvapm2Gd+rjjEdV9zHGgPN/ab9q+MoKfZaNQJ47Kp2Q9Ix66nxl5+fnzbmU/ivG9nBhg0bQt/xuNJj33XssoaAzgkdK7Vq1QrppHGu+huqXcRjuahj6tk26FjV44vZr6nukvoCthWs8QGk6xZyHXQeqi1j2/XBBx9EZTy3tB9U14iPBlf7re3L93rsscdmLANiG6g2RPuUNbtUH0nvjW2X2mHW1ADiPlb7zu2rOiNJGmI6dnU9xG2mv6lHeLOP0f7Ve+O5pvNFfSCvDfQ6Wn/uC9XdWrp0aUirzpbe91tvvRXSqjui84l/U32ejk+eE6k5rGsHvbZ3Su1aPv/887D+0P5l9Plg3rx5Ia0aPjo/eA6w7g4QayCpPpKu1VhzqEOHDlHZgAEDovwTTzwR0itWrIjKjj/++Cj/7rvvhvTRRx8dlY0fPz7Ksy7hK6+8EpXpd9nu6/pLbT37LdWbYhun9lnXkjzXVQvozTffjPKsG6ZrOdWumjlzZkirbpD6F9bs0rGh9uX9998PafUJH374YZRnv8VaVADw6quvhrS2idpKHjtPP/10VHb44YdHefYRbDeB9PUDr6lVS0l1hdl/63V4TQXEvlHn4axZs6I8+wxdIyQ9v+gcSXo203tjra3p06dnrA8Qa3Gm1lRJuth+lojJ2pdSxhiTzezOjsEYY8yOYz9hjDEmE/YR/8UvpYwxpphsjxOx4zHGmD0H/wXcGGNMJvwsEeOXUsYYU0zsSIwxxiThl1LGGGMy4WeJmKx9KbVp06YQW8x6C0maMkAcY6pxohrjzLHAGtvNMc4aI6yf5bjqpOtoudZPv8vaDBq3qpokHM+t2kqqR5Skr6GwhoLqOOi9MaodwdepXLlyVHbwwQdH+e+++67QugLpehXc9vy9wurA19L4cs1zm2nMuMbD8+9oW3Ofar9o+3GcuPYva6UBcey56mnoffOcUH0sbTPVe2K037jN9F60/hxTrvXjsqQ20fKiNMQ4plzbT+caz4OUvVEdHcaOJDsoXbp0sI3c/6pvoPA4UpuiGjQ831U/huePjhedLzxedTyqLg/rPrC2CQAsW7Ysyh9yyCEhrfeten2rVq0KadU/VM0m9jlJ2nNA7COTbAxrUgCx3kZhdWCWLFkS5Vn3Y/ny5VGZtn2SrpXqRLHehfof9cOsNaH6h+oneHzoGGONSG1r7SfWfEmyY0Bsc3Ts6hhke65zQvNsl1VLRm0263Po2FDfz75A113t2rULaZ0DavubNm2asUz7lOuraxzW4gHi+aU+rjD8UmrX06dPn7SxDqSvNbSvWcNJy+bPnx/l2RapzeXxpfVQLUHWEdK5/dRTT0V5Xmvq/FQtqCZNmoS02lz9Hb7vF198MSp7/fXXozzbynfeeScqY78EAIsWLQppnTuPPfZYSKt+U5s2baI86w7qXFY9PtaEmzt3blSm/c+aijVq1IjKXnjhhSjP9vvjjz+Oytg+67V0fmsbffLJJyGt2kWtW7cO6WbNmkVl+vzC6wf1Q9r206ZNC+nOnTtHZfp8wGNZ/fFll10W5dknaz/xWADidcExxxwTlenaiOeM+gi+LrcXAFx11VVR/sEHHwxpfW5r3759lM/Lywtp9aPnnntulGett7PPPhtAug9i/CwRk7UvpYwxJluxIzHGGJOEX0oZY4zJhJ8lYvxSyhhjiokdiTHGmCT8UsoYY0wm/CwRk7UvpcqWLRu2onO4j25T1aMWeXu4bqfXbeb8XQ0F4tA6DTfSOvB2ew3h0G2LvHVStyXq1l6ur15HtwjztveirsvbdfW6GlLI2yO1jTisQEMitB04r+EJfGQ0EB/VqqFzutWYr6X9onVKCsnUscHbLXWbrxoE/l1tI66fjlUdV9xGGrKh98L9pH2mbc8hJzo2dCsvhwVqmyhJoX7aDjxek+ashn7oVlne7qx9qHm+lpZpmAvXL5V2+F7207BhwzB+kmygbkNnu6LzW7/LW+PVp/C2cx27euQ0b/nXsA0djzz/NeRpzZo1UZ7nodrAxo0bR3m2BTzXtX5APGf0N/WzPE/1umxH1OZpmB3bOQ6nAJKPYde21zBBDi3hkA4gPjYciMMv1AboNv8kG6NjpW7duiG9cuXKqIz9RFGyA1y/6tWrR2UciqHfVb+rtp/DwPU39chxDgPVPlS/wOsPPWpbxwrbYZ0THIaiv6E+he9Vr6N14PbUNlLbwPM2NZd07DF+KbXr+eyzz8Kc4rA7DpUD0uf6xIkTQ1rH0PXXXx/ln3322UK/BwA333xzSHPoGQAcddRRUZ5tmoaB6dqX506rVq2isjfffDPK8zH13377bVSmY55tiK6/tR04zyGChcHhXurTDj300JDWOachtezn+/XrF5W9/PLLUZ79oYa2q/3jUGINz9SxwrZd16haX7ZpS5cujco0XJ1tk7Ynf5bDyYD08PW+ffuGtK7j33vvvSjfsWPHkNYxps9m7PdPO+20xOtyX6jESO3ataM823P1abqOYls/e/bsqOyUU04Jae0zbTMe2zondJ6yD9PQPg1jPOGEE0I6FSqr/onxs0RMsqCQMcYYY4wxxhhjjDG/AFm7U8oYY7IV/3XDGGNMEt4pZYwxJhN+lojxSyljjCkmdiTGGGOS8EspY4wxmfCzREzWvpQqVapUiC1mrQbVEtB4Xo4/Vf0H1dvg2GU96pnROGqNwWZUCyhJW0m1nvS7rPekMamq2cNaHRoXrPpTSfet8dysb6HaCVpfRvU1uM00RljrwBNOj9JM0irSuGBtM45r1rqvW7cuynN7qu6WjiPuU9UD4e/qMbMcG6/XUbQ9k/pF25Nj53W+6Fjmsa6fVe0QLletGK0v95OWcV/oWNV74bGTpBEHxBouql2ifci2IjXG9DOMHUl28OGHH4a5wO1blMYQ6z6oLdDjlVk/QnU+2B+pv2HdHSC2T6xfASRr+2nd1X6yDolqZ6lN/PTTT0Na549qafF817GrWiOMthHPYZ3PK1asiPJsq9Sm1KlTJ8qz7VJfqu3AfaN1Vw0QPpZb7ZGuBdiG62+q7haPK9VU+eKLL0JadTy0vqxHpX5LfQzbWrXn2qesI6V6JjxugFjbb9myZRl/E4jHmc5LbV/27+r7WVNF52j9+vWjPPeF+lXWrwHi9k7SQ9Nrpfp+Z2oP2kfsfH7++edgX7l/VW9P9Wl4but8HTt2bMbf0yPt2U6phtTHH38c5dkPqE7QSSedFOXZdqrtbt26dZTn+at2VfWo5syZE9Kqv6dac+wj1DbqWpg1nXQtybpGTz31VFSmdpXtwFtvvRWV6Zr6ww8/DGltI9UcYjt23HHHZbyOXku1D9u0aZPxu9ovqnPFtkQ1Cfk62oe81gWAJ554IqR1zOkzNNucefPmRWWdOnWK8rwmnjt3blTWq1evKM/179KlS1Smmk3cbw8++GBUprphPHaaN28elXEf6ppAdTzZtqtv1H7i7xalZcvaWqm23Zm6g9v7nV8LWftSyhhjshU7EmOMMUn4pZQxxphM+Fkixi+ljDGmmNiRGGOMScIvpYwxxmTCzxIxfilljDHFxI7EGGNMEn4pZYwxJhN+lojJ2pdSpUuXTotRBtL1kjQ+ljUKNI5TtSO4XLUuWItDdQ80/pQ1NLTOqkvD9VV9JNU24fpprLTqdnBsssYia/15QGs8rOo4sE5Pkp6Xlqk2Ff+OaqRonDrH72t/q8YD35vGsOvvcHurlpLmuR20jZK0lVTXiOukhkT1QPjedCwk9aFqWui44ryOT70ua7ronNCYfI7Z5u8VVn/uY60D97FeR8dVks6T9vdXX30V0jqukzTFUvXZmVoh2/sdk8yBBx4YxiFrAam2js5L1hZRW6pjhfVzZs2aFZWdcMIJIa3zQ6/DNlq1lFR/iLUR1N/UrFkzyvM8VK0dtQWso6HjUW3t559/HtJqz1UDi+epzhuuE89JIL3t2QZq/VRbhNtByzTP9l3trupusd1TX6prCtbyKMoH8nU/+OCDqIx1UlQLQzXEknS31GZzn2r/6r3x+kg1VPR3+LuqeaXtsGbNmkJ/A0j32dxPSXpOOm4WL16c8bNKcfTRWL8LAKpXrx7SBx10EIB025L0W0VhH7HzmTdvXljncF9Pnjw5+pzqRp1//vkhvXTp0qhM14tTp04NafYXWqb6TWqvuf9VW06fAXgNo/NTdY1Y33DGjBmJn2WtrUWLFkVlZ599dpRnG6d2inXyAOB3v/tdSKfmTor3338/pNleAOnrOta5WrhwYVSmWo3cvqeeempU9uabb0Z5tu2qraTrCf4d1ajTNQLXX9cISbpbqlXF/k51/NQesq6ZPq+oreQ6dO/ePSrTMXfttdeG9I033hiVPf7441Ge+/vvf/97VHbsscdGeR6/uhZSX8njl9dfQNxG2g+1atWK8qwxrOsx1oUC4ucObU9tI/bfKc0z9b2MnyVi0t/67CRGjx6NWrVqoUKFCmjXrl3aJDfGGLPnYh9hjDEmCfsJY4zZM/hFXkpNmDABgwcPxtChQ7Fw4UI0a9YMOTk5aX8lNcaYXyMFBQXb9c9sxT7CGLO7Yx+xY9hPGGN2Z/wsEVOq4Be4u3bt2qFNmza49957AWzdSl2jRg1cfvnl0fa/wli/fj0qVqyIWrVqhTAf3tqn2x91y23S9lfdVs5hRLoFj39Tt5zrdm3eyqvhR7qtltFQJL0uf1e3eepnecughsMldbGGMWn7ch011IvrpGEN+pv8WW1r3QqtISeMbunn39GQEg3T4C23et8a7pHU9rog4j7X0DS+blKYgP6mhpTocfMcnqBlStJxpNrfvK1a70XHFaPjPmnMJY177UO9Ny7XcZMUyqLzJSkMMEV+fj6+/PJLrFu3LtiOlH0qXbp0WnhOURQUFCA/Pz+63p7KjvgI4L/98OCDDxYavqdzTcN5eKxomfoUthX6WfYNeuSwHvfMISAakqA2kW2tzlEd97x1X+uu3+Xr6pzQcEPefq9zX+0nz3+dW+ybOGxSy7R+iv4m96HaZK0vh6hoP2noA4ed6JHtGgLA39Xf1C37Scen82c51AZI71Mu12PNNWSmdu3aIc0hMkB623OIivpDDWHnsBi9Fw2/4O+qb+ej6rUOWj+uU1Fh3ezHNDQjyZ/r+kL9GodZptaXP/74Iy677LKd4ifsI2J2xrPEsGHDgu3gkK0ePXpEn08Kl9I1VJKMhNp2nnfvvvtuVNa0adMoz7ZJr8OhwkAcLjd37tyobNCgQVGefaN+VsP37rrrrpDW0DR9FmIfweFQQHqYE899tXHs09S/tWzZMsq/8sorIX344YdHZRqaxqHv6o+T1s0aMtaoUaMoz/2oNlh9GI8rndNqrzk8WNuPbaXuFjzppJOiPI/zjh07RmX6XMzjQX1h27Ztozy3p64t9JmF7fU555wTlb399ttRntceHJ4JpMsV8NjR8cjhnBoiqvDzoM7nf/zjH1FefRGj475OnTohnWqvH3/8EX/4wx/8LLEN7PSdUps2bUJeXh66du363x8pXRpdu3bF7Nmz0z6/ceNGrF+/PvpnjDHZjP+6sf0U10cA9hPGmF8f9hHbj58ljDG7O36WiNnpL6W++eYbbNmyJe2vZVWqVEn7SwQADBs2DBUrVgz/VFDOGGOyDTuS7ae4PgKwnzDG/Pqwj9h+/CxhjNnd8bNEzC4/fe+6667D4MGDQ37dunWoWbNmFCbBW7M1fELz3FnaccU5kYU/W9RvZqorkH4CD6OfLc519bNJbVScUKqkOhSnbGe1p5L0O0XVge91Z7b9to6rpM9peVFjN6l+SddNqp9eqzjzpzhjLuleinPfOzJuiuoL/kyme9mdHUO2kclPcAgah1hoaFpxwvc0HClpzPF19Df11Lyk+ml4CM/DokKj+Vrqb/R3OISiqDpkatvC6pBkW5N+Q+ubFLpdnLbX3+HwgKTwey3XsLWk72qZhu/xeEgK39O662e5TjrGksZgUW2fdIqstgNfS+undeJ70/5Nat+ksawhMjrmku5F4XvREPBtuW7qv/YTu5ZMPoL7l8P/d8T+6SmXPB6T7InahKR5pr+ZNNf1uhpKzN/VOafX5Tmq102yA0X5v231aWrnNaycv6u/ofVLak/tw6TrJNn2JB+rv6t2K+l3ktYPKnORZHOL8hFJJ7TqZ5PmhN4LXyvpVHe9ltZXv8vlaq+TxqPC103yx4X9DpPUh6l0ql72EUWz019KVa5cGWXKlEk71nPNmjVpMb3AVgPORjy15VaP4t0ZbO92XtVXMLsO1SQpDrt6O3eSJlNRlNQYzLaxng31+f7770Pserly5VC1atWMO3qKomrVqmk6JXsaxfURQGY/ccUVV/xyFTXGmG1kZ/kJ+4it7KxniZtvvrnQ6z/77LM7sbbZxeOPP76rq2BKkKeeeipj2YMPPliCNSmchx56aFdXISvws0TR7PSXUuXKlUOrVq2Qm5uLXr16Adj65js3NxcDBw4s8vvVqlXDZ599hoKCAtSsWROfffbZbifktbNYv349atSo4TZKwG2UjNsnMwUFBfj+++8jcdsKFSpgxYoVaX9J2VbKlSuXJti8p7GjPgKwn9hWPL+Lxm1UNG6jzOxsP2EfsRU/S5Qcnt9F4zYqGrdR4fhZYtv5RcL3Bg8ejH79+qF169Zo27YtRo4ciQ0bNuDCCy8s8rulS5fGIYccEv7Ksf/++3twF4HbqGjcRsm4fQpHT/cAtjqT3dEZlCQ74iMA+4ni4vYpGrdR0biNCsd+4pfBzxIli9uoaNxGReM2Ssc+Ytv4RV5KnXnmmfj6668xZMgQrF69Gs2bN8fkyZPTBAuNMcbsedhHGGOMScJ+whhj9hx+MaHzgQMHbnMohjHGmD0L+whjjDFJ2E8YY8yeQemiP7JrKF++PIYOHZp2koX5L26jonEbJeP2Mb9mPH6TcfsUjduoaNxG5teKx27RuI2Kxm1UNG4js6OUKvBZhMYYY4wxxhhjjDGmhMnanVLGGGOMMcYYY4wxZvfFL6WMMcYYY4wxxhhjTInjl1LGGGOMMcYYY4wxpsTxSyljjDHGGGOMMcYYU+Jk7Uup0aNHo1atWqhQoQLatWuHefPm7eoq7RKGDRuGNm3aYL/99sNBBx2EXr16YdmyZdFnfvrpJwwYMAAHHngg9t13X/Tp0wdr1qzZRTXe9dx+++0oVaoUBg0aFP6f2whYtWoVzjvvPBx44IHYe++90aRJEyxYsCCUFxQUYMiQITj44IOx9957o2vXrvjggw92YY2NyYx9xH+xnyge9hGFYx9hdjfsJ7ZiH1F87CcKx37C/FJk5UupCRMmYPDgwRg6dCgWLlyIZs2aIScnB1999dWurlqJM23aNAwYMABz5szBlClTsHnzZnTr1g0bNmwIn7nqqqvw/PPP48knn8S0adPwxRdf4NRTT92Ftd51zJ8/H/fffz+aNm0a/f89vY2+++47dOzYEXvttRdefvllLF26FHfeeScOOOCA8Jm//vWvuPvuuzFmzBjMnTsXv/nNb5CTk4OffvppF9bcmHTsI2LsJ7Yd+4jCsY8wuxv2E//FPqJ42E8Ujv2E+UUpyELatm1bMGDAgJDfsmVLQbVq1QqGDRu2C2uVHXz11VcFAAqmTZtWUFBQULB27dqCvfbaq+DJJ58Mn3nvvfcKABTMnj17V1Vzl/D9998X1KtXr2DKlCkFnTt3LrjyyisLCgrcRgUFBQXXXHNNwVFHHZWxPD8/v6Bq1aoFd9xxR/h/a9euLShfvnzBP//5z5KoojHbjH1EMvYThWMfkRn7CLO7YT+RGfuIzNhPZMZ+wvySZN1OqU2bNiEvLw9du3YN/6906dLo2rUrZs+evQtrlh2sW7cOAFCpUiUAQF5eHjZv3hy1V4MGDVCzZs09rr0GDBiAE044IWoLwG0EAM899xxat26N008/HQcddBBatGiBBx98MJSvWLECq1evjtqoYsWKaNeu3R7TRubXgX1E0dhPFI59RGbsI8zuhP1EMvYRmbGfyIz9hPklybqXUt988w22bNmCKlWqRP+/SpUqWL169S6qVXaQn5+PQYMGoWPHjmjcuDEAYPXq1ShXrhx++9vfRp/d09pr/PjxWLhwIYYNG5ZW5jYCPv74Y9x3332oV68eXnnlFVx66aW44oor8OijjwJAaAfPO5Pt2EckYz9ROPYRydhHmN0J+4nM2Edkxn4iGfsJ80tSdldXwGw7AwYMwJIlSzBz5sxdXZWs4rPPPsOVV16JKVOmoEKFCru6OllJfn4+Wrdujb/85S8AgBYtWmDJkiUYM2YM+vXrt4trZ4zZWdhPpGMfUTT2EcbsGdhHFI79RNHYT5hfkqzbKVW5cmWUKVMm7TSDNWvWoGrVqruoVruegQMH4oUXXsDrr7+OQw45JPz/qlWrYtOmTVi7dm30+T2pvfLy8vDVV1+hZcuWKFu2LMqWLYtp06bh7rvvRtmyZVGlSpU9vo0OPvhgNGrUKPp/DRs2xMqVKwEgtIPnncl27CMyYz9ROPYRRWMfYXYn7CcKxz4iM/YTRWM/YX5Jsu6lVLly5dCqVSvk5uaG/5efn4/c3Fy0b99+F9Zs11BQUICBAwdi4sSJmDp1KmrXrh2Vt2rVCnvttVfUXsuWLcPKlSv3mPY67rjj8M4772DRokXhX+vWrXHuueeG9J7eRh07dkw7/nf58uU49NBDAQC1a9dG1apVozZav3495s6du8e0kfl1YB+Rjv1EMvYRRWMfYXYn7Cdi7COKxn6iaOwnzC/KLhZaL5Tx48cXlC9fvuCRRx4pWLp0acHFF19c8Nvf/rZg9erVu7pqJc6ll15aULFixYI33nij4Msvvwz/fvjhh/CZSy65pKBmzZoFU6dOLViwYEFB+/btC9q3b78La73r4RMzCgrcRvPmzSsoW7ZswZ///OeCDz74oGDs2LEF++yzT8ETTzwRPnP77bcX/Pa3vy149tlnCxYvXlxwyimnFNSuXbvgxx9/3IU1NyYd+4gY+4niYx8RYx9hdjfsJ/6LfcT2YT8RYz9hfkmy8qVUQUFBwT333FNQs2bNgnLlyhW0bdu2YM6cObu6SrsEAIX+e/jhh8Nnfvzxx4LLLrus4IADDijYZ599Cnr37l3w5Zdf7rpKZwHqSNxGBQXPP/98QePGjQvKly9f0KBBg4IHHnggKs/Pzy+48cYbC6pUqVJQvnz5guOOO65g2bJlu6i2xiRjH/Ff7CeKj31EOvYRZnfDfmIr9hHbh/1EOvYT5peiVEFBQUFJ784yxhhjjDHGGGOMMXs2WacpZYwxxhhjjDHGGGN2f/xSyhhjjDHGGGOMMcaUOH4pZYwxxhhjjDHGGGNKHL+UMsYYY4wxxhhjjDEljl9KGWOMMcYYY4wxxpgSxy+ljDHGGGOMMcYYY0yJ45dSxhhjjDHGGGOMMabE8UspY4wxxhhjjDHGGFPi+KWUMcYYY4wxxhhjjClx/FLKGGOMMcYYY4wxxpQ4filljDHGGGOMMcYYY0ocv5QyxhhjjDHGGGOMMSXO/wcBW4iaLHvcaQAAAABJRU5ErkJggg==",
                         "text/plain": [
                             "<Figure size 1200x600 with 6 Axes>"
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
                 }
@@ -258,15 +262,15 @@
                 "key = jax.random.PRNGKey(0)\n",
                 "fig, axes = plt.subplots(ncols=3, figsize=(12, 6))\n",
                 "ax1, ax2, ax3 = axes\n",
                 "im1 = plot_image(\n",
                 "    compute_noisy_image(scattering_pipeline, key),\n",
                 "    fig,\n",
                 "    ax1,\n",
-                "    label=\"Scattering potential at exit plane\",\n",
+                "    label=\"Phase shifts at exit plane\",\n",
                 ")\n",
                 "im2 = plot_image(\n",
                 "    compute_noisy_image(optics_pipeline, key),\n",
                 "    fig,\n",
                 "    ax2,\n",
                 "    label=\"Squared wavefunction at detector plane\",\n",
                 ")\n",
@@ -278,29 +282,29 @@
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "What if we did not want to include noise in the simulation? In this case, the three outputs are\n",
                 "\n",
-                "**1. If there is no `Instrument`:** The returned \"image\" is the scattering potential in the exit plane including stochasticity, which here we use in the `solvent` model.\n",
+                "**1. If there the `Instrument` just has an accelerating voltage and a dose:** The returned \"image\" is the phase shifts in the exit plane including stochasticity, which here we use in the `solvent` model.\n",
                 "\n",
-                "**2. If the `Instrument` just has an optics model:** Again, the returned \"image\" is the squared wavefunction in the detector plane.\n",
+                "**2. If the `Instrument` also has an optics model:** Again, the returned \"image\" is the squared wavefunction in the detector plane.\n",
                 "\n",
-                "**3. If the `Instrument` has optics, dose, and detector models:** Now, the returned \"image\" is the expected number of electron counts for each pixel. This is nothing but the poisson rate."
+                "**3. If the `Instrument` also has a detector model:** Now, the returned \"image\" is the expected number of electron counts for each pixel. This is nothing but the poisson rate."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 12,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
-                        "image/png": "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ZsyYgc6dOxvpevjhh1G4cGEMGzYMu3btwvjx49G/f39MmzYNADB+/Hg8/PDDKFCggDuAKVGiRND3nD59Ok6fPo2+ffuiaNGi+OmnnzBhwgT8+uuvmD59etj55eV+DzzwAPbv34/58+fjgw8+COu+H3zwAbp3746UlBQ8//zzOH36NN544w00a9YMq1evRvny5XH99dfjoYcewpgxY9CpUydcc801OHDgAB5++GG0adMGDz74YMB7t2jRAgMGDMCrr76KJ554AtWrVwcA9/9gXLx4Ee3atcO1116LsWPHYs6cORg2bBguXLiAkSNHBr3u559/xrJly3DXXXehTJky2LVrF9544w20atUKGzZsQL58+YzzQ5V5uPmjZA1ebPV9992HDz/8EPfccw+aNm2KRYsWoUOHDhl6/htvvIGaNWvilltuQa5cuTBr1iw89NBDSEtLQ79+/YxzN2/ejLvvvhsPPPAA7r//flStWhWnT59Gy5YtsW/fPjzwwAMoV64cli1bhiFDhuDAgQNuOLfjOLj11lvx3Xff4cEHH0T16tXx2WefoXv37iHTWKhQIdSqVQtLly7FgAEDAFyy7REREfj999+xYcMG1KxZE8Clj1A+HwOEZ2PuuOMOPProo/j444/djp+Pjz/+GG3btnVD78LxVw888ABKly6N0aNHY8CAAWjUqJHVrtqYOnUq/vzzTzzwwAOIiIjA2LFj0aVLF+zYsQO5c+cGAPzyyy9o3rw5cufOjT59+qB8+fLYvn07Zs2ahWeffRZdunTBli1b8N///hfjxo1DsWLFACCojzt06BCaNm2K06dPY8CAAShatCjef/993HLLLfjkk0/8/Mxzzz2HyMhI/Pvf/8bx48cxduxY/OMf/8CPP/5ofbdwbFt67O28efPQtWtX1KhRA2PGjMHRo0fRs2fPgB9nHnjgAUyZMgU9e/bEgAEDsHPnTrz22mtYvXo1vv/+e+TOndvqJ8Ot/wDQu3dvTJkyBe3bt8d9992HCxcu4Ntvv8UPP/yAhg0b4oMPPsB9992Hxo0bo0+fPgCAihUrArjk+5s3b47Y2Fg8+uijyJ07N9588020atUKS5YsQZMmTYz3euihh1C8eHEMHToUp06dspYDcGnGZkREBB577DEcPnwY48ePR5s2bZCammqdDfnKK6/glltuwT/+8Q+cO3cOH330EW6//XZ8+eWXfrYpnP7YoUOHcO2117oDteLFi+Prr79G7969ceLECQwcODDkuyh/L44fP44jR44Yf4uIiHDrzFNPPYVZs2ahd+/eWLt2LQoWLIi5c+fi7bffxqhRo1C3bl3j2nDqerjjkv3796Nx48Y4duwY+vTpg2rVqmHfvn345JNPcPr06ZD2K9y+mBebFoiM9PmeffZZPP3007jjjjtw33334bfffsOECRPQokULrF692v1Bbf78+bj55ptRsmRJ/Otf/0JCQgI2btyIL7/8Ev/617/C6stPnjwZf/31F/r06YOYmBgUKVIECxYsQPv27VGhQgUMHz4cZ86cwYQJE3Dddddh1apVfmm/4447kJSUhDFjxmDVqlV45513EB8fj+eff96aR6HSD8BzWsIllG20+fD169fj5ptvRp06dTBy5EjExMRg27ZtAT+gKjkYJwczb948JyoqyomKinKSk5OdRx991Jk7d65z7tw547ytW7c6kZGRTufOnZ2LFy8ax9LS0tzt06dP+z3jgQcecPLly+f89ddf7t86dOjgJCYm+p37888/OwCcyZMn+z2jcuXKTkpKit/zkpKSnBtvvNH927BhwxwAzt133+13f98xCQAnOjra2bZtm/u3NWvWOACcCRMmuH/r2LGjky9fPmffvn3u37Zu3erkypXL756BaNmypQPAeemll9y/nT171qlXr54THx/v5vn48eMdAM6HH37onnfu3DknOTnZKVCggHPixAnHcRznt99+cwA4w4YN83vWDTfc4NSuXdvI87S0NKdp06ZO5cqV3b9NnjzZAeC0adPGyNdBgwY5UVFRzrFjx9y/1axZ02nZsqXfs7755hsHgPPNN9+4fwtUD8aMGeNEREQ4u3fvdv8WqDwCEe79+vXrF9b9HMdx/vzzT6dQoULO/fffb/z94MGDTlxcnPH3U6dOOZUqVXJq1qzp/PXXX06HDh2c2NhY49mO4ziJiYlO9+7d3f3p06f75Y2N7t27OwCchx9+2P1bWlqa06FDByc6Otr57bff3L9z2QfKo+XLlzsAnP/85z/u38Itcy/5o1x+wrXVqampDgDnoYceMv5+zz33+NWZ7t27B7TDgdploPqVkpLiVKhQwfhbYmKiA8CZM2eO8fdRo0Y5+fPnd7Zs2WL8/fHHH3eioqKcPXv2OI7jODNnznQAOGPHjnXPuXDhgtO8efOAvoHp16+fU6JECXd/8ODBTosWLZz4+HjnjTfecBzHcY4ePepEREQ4r7zyivX9AtmY5ORkp0GDBsZ5P/30k9HOvPgrn/2cPn26cc+WLVsGtLdcZjt37nQAOEWLFnV+//139++ff/65A8CZNWuW+7cWLVo4BQsW9LNbMo0vvPCCA8DZuXOn37PZvg0cONAB4Hz77bfu3/78808nKSnJKV++vNtX8L1j9erVnbNnz7rnvvLKKw4AZ+3atX7PkoRr27za23r16jklS5Y0/Ny8efMcAEYef/vttw4A5//+7/+M6+fMmeP392B+Mtz6v2jRIgeAM2DAAL97yHLKnz+/URY+OnXq5ERHRzvbt293/7Z//36nYMGCTosWLdy/+fxAs2bNnAsXLvjdh/GVYenSpd0+iOM4zscff+wAMNpSILvCZXju3DmnVq1azvXXX2/8Pdz+WO/evZ2SJUs6R44cMa6/6667nLi4uIB1Rvl74qvLgf7FxMQY565du9aJjo527rvvPuePP/5wSpcu7TRs2NA5f/68e064dd2Lne/WrZsTGRnp/Pzzz37p910bzH556YuFa9MC4eU53EfYtWuXExUV5Tz77LPGtWvXrnVy5crl/v3ChQtOUlKSk5iY6Pzxxx8B88Fxgvflff4uNjbWOXz4sHHMN5Y6evSo+7c1a9Y4kZGRTrdu3fzS3qtXL+P6zp07O0WLFg2YNz7CTX+4afHSBwvXNgbz4ePGjXMAGOMI5e9Hjg7fu/HGG7F8+XLccsstWLNmDcaOHYuUlBSULl3aCPWaOXMm0tLSMHToUERGmq8spxjKX8r+/PNPHDlyBM2bN8fp06exadOmdKczNTUVW7duxT333IOjR4/iyJEjOHLkCE6dOoUbbrgBS5cu9ZsCH2wGSyDatGnj/tIIXJpxFBsbix07dgC4NHtlwYIF6NSpE0qVKuWeV6lSJbRv3z7s5+TKlQsPPPCAux8dHY0HHngAhw8fxsqVKwFcEvhLSEjA3Xff7Z6XO3duDBgwACdPnsSSJUusz/j999+xaNEi3HHHHW4ZHDlyBEePHkVKSgq2bt2Kffv2Gdf06dPHKMfmzZvj4sWLAcNUwkHWg1OnTuHIkSNo2rQpHMfB6tWrr/j9gEu/dhw7dgx33323m0dHjhxBVFQUmjRpgm+++cY9N1++fJgyZQo2btyIFi1aYPbs2Rg3bhzKlSuXrmeHon///u6275fgc+fOYcGCBUGvkXl0/vx5HD16FJUqVUKhQoWwatUqv/NDlbmX/FEuP+Ha6q+++goA3JlCPjI6c0DWL98v0i1btsSOHTtw/Phx49ykpCSkpKQYf5s+fTqaN2+OwoULG/WpTZs2uHjxIpYuXeqmP1euXOjbt697bVRUFB5++OGw0tm8eXMcOnQImzdvBnBpRlSLFi3QvHlzfPvttwAu/droOI4xUypcG3PnnXdi5cqV2L59u/u3adOmISYmBrfeeiuA9PmrjHLnnXcaAum+d/P5sN9++w1Lly5Fr169/OxWepf2/uqrr9C4cWM3PB64NOu5T58+2LVrlxtS4aNnz56G7genMRhebVs4HDhwAKmpqejevTvi4uLcv994442oUaOGce706dMRFxeHG2+80ai7DRo0QIECBcKyheHW/xkzZiAiIgLDhg3zu0eocrp48SLmzZuHTp06oUKFCu7fS5YsiXvuuQffffcdTpw4YVxz//33IyoqKmT6fXTr1g0FCxZ092+77TaULFnStTvBkGX4xx9/4Pjx42jevHnA8gvVH3McBzNmzEDHjh3hOI6RnykpKTh+/Hi664WSc5k4cSLmz59v/Pv666+Nc2rVqoURI0bgnXfeQUpKCo4cOYL3338/oNZsqLoerp1PS0vDzJkz0bFjx4CaV6Hadbh9MS82LSPPCcSnn36KtLQ03HHHHca1CQkJqFy5snvt6tWrsXPnTgwcONBPisCLH+ratasxg9f37j169ECRIkXcv9epUwc33nhjQPvEY8TmzZvj6NGjfjZSEk7605OWcAllG2340vv5559nev9DyT7k6PA9AGjUqBE+/fRTnDt3DmvWrMFnn32GcePG4bbbbkNqaipq1KiB7du3IzIyMqRhW79+PZ566iksWrTIr2HzwMULW7duBQBrCMfx48eNTnlSUlLY9w/0caFw4cKuXsThw4dx5syZgKt4eFnZo1SpUn5ColWqVAFwKVb62muvxe7du1G5cmW/j3++abyhPhRt27YNjuPg6aefxtNPPx3wnMOHD6N06dLuPr+/Lx+lXoYX9uzZg6FDh+KLL77wu0d66kFm3w/4X526/vrrAx6PjY019q+77jr07dsXEydOREpKihtumdlERkYaAwrArCPBOHPmDMaMGYPJkydj3759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84f1gSNQPXAcx2+51HDxcr9g9ScQKSkpiI2NxejRo3H+/Hm/4zKffvzxR7z44osYOHAg/t//+3945JFH8Nprr4XU9/KSHslrr73mbjuOg9deew25c+fGDTfcEPSaqKgov7Y8YcKEoL+4hMJL/iiXn3BttU/jjj+YytW9fFSsWBHHjx/HL7/84v7twIEDfktIB2qDx48f9zSovOOOO7B8+XLMnTvX79ixY8dw4cIFAJfs34ULF/DGG2+4xy9evIgJEyaE/azmzZtj165dmDZtmhvOFxkZiaZNm+Lll1/G+fPnDT0przara9euiIqKwn//+19Mnz4dN998s9HhzQx/VbFiRWzatMk4d82aNeleKad48eJo0aIF3nvvPezZs8c4Jt/bi8266aab8NNPP2H58uXu306dOoW33noL5cuXD0vHJBzCtW1e0l6yZEnUq1cP77//vtEXmT9/vp8W1h133IGLFy9i1KhRfve5cOGC8bxgfjLc+t+1a1c4jmN8NPXB5cTPiYqKQtu2bfH5558b4XSHDh3C1KlT0axZswyHXf/nP//Bn3/+6e5/8sknOHDggFVbMyoqChEREUZ57dq1CzNnzkxXGqKiotC1a1fMmDEj4EBffZMSjJdffhnLli3DW2+9hVGjRqFp06bo27ev36p9QOi6Hq6dj4yMRKdOnTBr1iysWLHC7zxfuw5mv8Lti3mxaYHISJ+vS5cuiIqKwogRI/xsteM4OHr0KADgmmuuQVJSEsaPH+/3nun1Q4D57vKadevWYd68ebjpppvCuk8owkm/l7SE2wfzQrC8CzRjzzfJRIZUKzmbHD1T6uGHH8bp06fRuXNnVKtWDefOncOyZcswbdo0lC9fHj179gRwKdzrySefxKhRo9C8eXN06dIFMTEx+Pnnn1GqVCmMGTMGTZs2ReHChdG9e3cMGDAAERER+OCDDwIOpBo0aIBp06Zh8ODBaNSoEQoUKICOHTuiYsWKKFSoECZNmoSCBQsif/78aNKkCZKSkvDOO++gffv2qFmzJnr27InSpUtj3759+OabbxAbG4tZs2Zd1rwaPnw45s2b52oLXbx4Ea+99hpq1aqF1NTUsO5RqlQpPP/889i1axeqVKmCadOmITU1FW+99ZYbc92nTx+8+eab6NGjB1auXIny5cvjk08+wffff4/x48e7wot58+ZFjRo1MG3aNFSpUgVFihRBrVq1UKtWLUycOBHNmjVD7dq1cf/996NChQo4dOgQli9fjl9//RVr1qzx/P4NGjTAG2+8gWeeeQaVKlVCfHx8wNjzatWqoWLFivj3v/+Nffv2ITY2FjNmzEi3PpWX+/k+7A0YMAApKSmIiorCXXfdFfC+sbGxeOONN3DvvffimmuuwV133YXixYtjz549mD17Nq677jq89tpr+Ouvv9C9e3dUrlwZzz77LABgxIgRmDVrFnr27Im1a9cG/QWmXr16iIqKwvPPP4/jx48jJiYG119/fVBtEgDIkycP5syZg+7du6NJkyb4+uuvMXv2bDzxxBPWMJGbb74ZH3zwAeLi4lCjRg0sX74cCxYscJdD9kq4+aNkDeHa6nr16uHuu+/G66+/juPHj6Np06ZYuHBhwBmdd911Fx577DF07twZAwYMcJd/rlKliqE/0bZtW0RHR6Njx4544IEHcPLkSbz99tuIj48P+OE7EI888gi++OIL3HzzzejRowcaNGiAU6dOYe3atfjkk0+wa9cuFCtWDB07dsR1112Hxx9/HLt27UKNGjXw6aefetIO8n1w2rx5M0aPHu3+vUWLFvj6668RExODRo0auX/3arPi4+PRunVrvPzyy/jzzz9x5513GscjIyMz7K969eqFl19+GSkpKejduzcOHz6MSZMmoWbNmlYhVhuvvvoqmjVrhmuuuQZ9+vRBUlISdu3ahdmzZ7s+zGdDn3zySdx1113InTs3OnbsGNDGPf744/jvf/+L9u3bY8CAAShSpAjef/997Ny5EzNmzMg0nYpwbZtXeztmzBh06NABzZo1Q69evfD7779jwoQJqFmzpjHIbNmyJR544AGMGTMGqampaNu2LXLnzo2tW7di+vTpeOWVV3Dbbbe5+RfIT4Zb/1u3bo17770Xr776KrZu3Yp27dohLS0N3377LVq3bu0ugtGgQQMsWLAAL7/8shuy2qRJEzzzzDOYP38+mjVrhoceegi5cuXCm2++ibNnz2Ls2LEZLosiRYqgWbNm6NmzJw4dOoTx48ejUqVKuP/++4Ne06FDB7z88sto164d7rnnHhw+fBgTJ05EpUqVjMGYF5577jl88803aNKkCe6//37UqFEDv//+O1atWoUFCxZkOGRKyXl8/fXXARdUatq0KSpUqICNGzfi6aefRo8ePdyZrVOmTEG9evXw0EMP4eOPPzauC1XXvdj50aNHY968eWjZsiX69OmD6tWr48CBA5g+fTq+++47FCpUyGq/wu2LhWvTApGRPl/FihXxzDPPYMiQIdi1axc6deqEggULYufOnfjss8/Qp08f/Pvf/0ZkZCTeeOMNdOzYEfXq1UPPnj1RsmRJbNq0CevXr3c/2nvpy/t44YUX0L59eyQnJ6N37944c+YMJkyYgLi4OAwfPtx6bbiEm/5w0xJuH8wLwXz4yJEjsXTpUnTo0AGJiYk4fPgwXn/9dZQpU8ZYrETJ4VyGFf2yjK+//trp1auXU61aNadAgQJOdHS0U6lSJefhhx92Dh065Hf+e++959SvX9+JiYlxChcu7LRs2dKZP3++e/z77793rr32Widv3rxOqVKl3GXLQcucnjx50rnnnnucQoUK+S1V+vnnnzs1atRwcuXK5bcE+OrVq50uXbo4RYsWdWJiYpzExETnjjvucBYuXOie41tKM9Cyl8GW2ezXr5/fubz8teM4zsKFC5369es70dHRTsWKFZ133nnH+X//7/85efLkCZbFLi1btnRq1qzprFixwklOTnby5MnjJCYmOq+99prfuYcOHXJ69uzpFCtWzImOjnZq164dcCn0ZcuWOQ0aNHCio6P9lnvfvn27061bNychIcHJnTu3U7p0aefmm292PvnkE/cc31K6vEytb0lcWWYHDx50OnTo4BQsWNAB4C57HejcDRs2OG3atHEKFCjgFCtWzLn//vvdpUvlewQqj0CEe78LFy44Dz/8sFO8eHEnIiIirHt/8803TkpKihMXF+fkyZPHqVixotOjRw9nxYoVjuM4zqBBg5yoqCjnxx9/NK5bsWKFkytXLqdv377u3wLVmbffftupUKGCExUVFXK58u7duzv58+d3tm/f7rRt29bJly+fU6JECWfYsGHu8uo+uLz/+OMPt84UKFDASUlJcTZt2uSXJi9lHk7+KFmDF1t95swZZ8CAAU7RokWd/PnzOx07dnT27t3rV2cc59Jy0bVq1XKio6OdqlWrOh9++GHAdvnFF184derUcfLkyeOUL1/eef7555333nvPb+nhxMREp0OHDgHf4c8//3SGDBniVKpUyYmOjnaKFSvmNG3a1HnxxRedc+fOuecdPXrUuffee53Y2FgnLi7Ouffee53Vq1f7tXcb8fHxDgAj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9NJL6NChAz766COsWLECb731lnvPRx55BHfeeSdatGiB1q1bY86cOZg1a5afMLOiKIqS9fAHiZiYmIAf+2y6g5s2bQp475SUFLz88sto0aIFKlasiIULF+LTTz91B14FCxZEcnIyRo0aherVq6NEiRL473//i+XLl/t9BFUURVGUzELD9xRFUTySVVNu77zzTrz44osYOnQo6tWrh9TUVMyZM8cdhOzZs8f4Fapp06aYOnUq3nrrLdStWxeffPIJZs6ciVq1arnndO7cGZMmTcLYsWNRu3ZtvPPOO5gxY4bfii6KoihK+smOuoOvvPIKKleujGrVqiE6Ohr9+/dHz549jV/4P/jgAziOg9KlSyMmJgavvvoq7r777ss2U1lRFOVqRMP3TNTDKIqieCQrHUn//v2xe/dunD17Fj/++KOx7PvixYsxZcoU4/zbb78dmzdvxtmzZ7Fu3TrcdNNNfvfs1asXtm7dijNnziA1NRW33nprutKmKIqiBCY76g4WL14cM2fOxKlTp7B7925s2rQJBQoUQIUKFdxzKlasiCVLluDkyZPYu3cvfvrpJ5w/f944R1EURckYWTGWWLp0KTp27IhSpUohIiICM2fONI736NEDERERxj8OQ92yZQtuvfVWFCtWDLGxsWjWrBm++eYb45w9e/agQ4cOyJcvH+Lj4/HII4/4hdaHIseF73FhcOyvjN3kX3U4plTGtdp0g0I9U8L3YQ0SqSN06tQp4xjrOMi4Vn4XjqWWOj2cXu5ISK0AjkXm9EqdGU6vjPXmuGWeai5j57mScofKprXFccsyhpjjlvk+smzkwB7w1yCR53IMtozXBszYahnvDpjvynHpnL7y5csHfSZrr8i6y3HpXFdk7DzrRHCbkBoqSUlJ1nPle/O7cfrlvozl5vty7DXHrXOcuITbpU2Xjp/jRWvCd2+NA7/yBCuHULZfljefy/tSt4A1QGR74jrP6ZJtljUVpDYHYNoy1upg/an169e722wfbfqCbPvZZkudOG6zfG716tXdbfaBkqlTpxr7FStWNPavvfZad5vDj+RsP8C0VfXr1zeOsa+SdpjzfuXKlUHTxJqL7HeXLFnibrO+BdcjWT/q1KljHJPvxmlnDT6Z96ztxdqT8plcN0qVKmXsb9myxd3mMC3WP5TaMtwmWEtLpunbb781jvG1Eq4b0mZzm2CN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",
+                        "image/png": "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ZsyYgc6dOxvpevjhh1G4cGEMGzYMu3btwvjx49G/f39MmzYNADB+/Hg8/PDDKFCggDuAKVGiRND3nD59Ok6fPo2+ffuiaNGi+OmnnzBhwgT8+uuvmD59etj55eV+DzzwAPbv34/58+fjgw8+COu+H3zwAbp3746UlBQ8//zzOH36NN544w00a9YMq1evRvny5XH99dfjoYcewpgxY9CpUydcc801OHDgAB5++GG0adMGDz74YMB7t2jRAgMGDMCrr76KJ554AtWrVwcA9/9gXLx4Ee3atcO1116LsWPHYs6cORg2bBguXLiAkSNHBr3u559/xrJly3DXXXehTJky2LVrF9544w20atUKGzZsQL58+YzzQ5V5uPmjZA1ebPV9992HDz/8EPfccw+aNm2KRYsWoUOHDhl6/htvvIGaNWvilltuQa5cuTBr1iw89NBDSEtLQ79+/YxzN2/ejLvvvhsPPPAA7r//flStWhWnT59Gy5YtsW/fPjzwwAMoV64cli1bhiFDhuDAgQNuOLfjOLj11lvx3Xff4cEHH0T16tXx2WefoXv37iHTWKhQIdSqVQtLly7FgAEDAFyy7REREfj999+xYcMG1KxZE8Clj1A+HwOEZ2PuuOMOPProo/j444/djp+Pjz/+GG3btnVD78LxVw888ABKly6N0aNHY8CAAWjUqJHVrtqYOnUq/vzzTzzwwAOIiIjA2LFj0aVLF+zYsQO5c+cGAPzyyy9o3rw5cufOjT59+qB8+fLYvn07Zs2ahWeffRZdunTBli1b8N///hfjxo1DsWLFACCojzt06BCaNm2K06dPY8CAAShatCjef/993HLLLfjkk0/8/Mxzzz2HyMhI/Pvf/8bx48cxduxY/OMf/8CPP/5ofbdwbFt67O28efPQtWtX1KhRA2PGjMHRo0fRs2fPgB9nHnjgAUyZMgU9e/bEgAEDsHPnTrz22mtYvXo1vv/+e+TOndvqJ8Ot/wDQu3dvTJkyBe3bt8d9992HCxcu4Ntvv8UPP/yAhg0b4oMPPsB9992Hxo0bo0+fPgCAihUrArjk+5s3b47Y2Fg8+uijyJ07N9588020atUKS5YsQZMmTYz3euihh1C8eHEMHToUp06dspYDcGnGZkREBB577DEcPnwY48ePR5s2bZCammqdDfnKK6/glltuwT/+8Q+cO3cOH330EW6//XZ8+eWXfrYpnP7YoUOHcO2117oDteLFi+Prr79G7969ceLECQwcODDkuyh/L44fP44jR44Yf4uIiHDrzFNPPYVZs2ahd+/eWLt2LQoWLIi5c+fi7bffxqhRo1C3bl3j2nDqerjjkv3796Nx48Y4duwY+vTpg2rVqmHfvn345JNPcPr06ZD2K9y+mBebFoiM9PmeffZZPP3007jjjjtw33334bfffsOECRPQokULrF692v1Bbf78+bj55ptRsmRJ/Otf/0JCQgI2btyIL7/8Ev/617/C6stPnjwZf/31F/r06YOYmBgUKVIECxYsQPv27VGhQgUMHz4cZ86cwYQJE3Dddddh1apVfmm/4447kJSUhDFjxmDVqlV45513EB8fj+eff96aR6HSD8BzWsIllG20+fD169fj5ptvRp06dTBy5EjExMRg27ZtAT+gKjkYJwczb948JyoqyomKinKSk5OdRx991Jk7d65z7tw547ytW7c6kZGRTufOnZ2LFy8ax9LS0tzt06dP+z3jgQcecPLly+f89ddf7t86dOjgJCYm+p37888/OwCcyZMn+z2jcuXKTkpKit/zkpKSnBtvvNH927BhwxwAzt133+13f98xCQAnOjra2bZtm/u3NWvWOACcCRMmuH/r2LGjky9fPmffvn3u37Zu3erkypXL756BaNmypQPAeemll9y/nT171qlXr54THx/v5vn48eMdAM6HH37onnfu3DknOTnZKVCggHPixAnHcRznt99+cwA4w4YN83vWDTfc4NSuXdvI87S0NKdp06ZO5cqV3b9NnjzZAeC0adPGyNdBgwY5UVFRzrFjx9y/1axZ02nZsqXfs7755hsHgPPNN9+4fwtUD8aMGeNEREQ4u3fvdv8WqDwCEe79+vXrF9b9HMdx/vzzT6dQoULO/fffb/z94MGDTlxcnPH3U6dOOZUqVXJq1qzp/PXXX06HDh2c2NhY49mO4ziJiYlO9+7d3f3p06f75Y2N7t27OwCchx9+2P1bWlqa06FDByc6Otr57bff3L9z2QfKo+XLlzsAnP/85z/u38Itcy/5o1x+wrXVqampDgDnoYceMv5+zz33+NWZ7t27B7TDgdploPqVkpLiVKhQwfhbYmKiA8CZM2eO8fdRo0Y5+fPnd7Zs2WL8/fHHH3eioqKcPXv2OI7jODNnznQAOGPHjnXPuXDhgtO8efOAvoHp16+fU6JECXd/8ODBTosWLZz4+HjnjTfecBzHcY4ePepEREQ4r7zyivX9AtmY5ORkp0GDBsZ5P/30k9HOvPgrn/2cPn26cc+WLVsGtLdcZjt37nQAOEWLFnV+//139++ff/65A8CZNWuW+7cWLVo4BQsW9LNbMo0vvPCCA8DZuXOn37PZvg0cONAB4Hz77bfu3/78808nKSnJKV++vNtX8L1j9erVnbNnz7rnvvLKKw4AZ+3atX7PkoRr27za23r16jklS5Y0/Ny8efMcAEYef/vttw4A5//+7/+M6+fMmeP392B+Mtz6v2jRIgeAM2DAAL97yHLKnz+/URY+OnXq5ERHRzvbt293/7Z//36nYMGCTosWLdy/+fxAs2bNnAsXLvjdh/GVYenSpd0+iOM4zscff+wAMNpSILvCZXju3DmnVq1azvXXX2/8Pdz+WO/evZ2SJUs6R44cMa6/6667nLi4uIB1Rvl74qvLgf7FxMQY565du9aJjo527rvvPuePP/5wSpcu7TRs2NA5f/68e064dd2Lne/WrZsTGRnp/Pzzz37p910bzH556YuFa9MC4eU53EfYtWuXExUV5Tz77LPGtWvXrnVy5crl/v3ChQtOUlKSk5iY6Pzxxx8B88Fxgvflff4uNjbWOXz4sHHMN5Y6evSo+7c1a9Y4kZGRTrdu3fzS3qtXL+P6zp07O0WLFg2YNz7CTX+4afHSBwvXNgbz4ePGjXMAGOMI5e9Hjg7fu/HGG7F8+XLccsstWLNmDcaOHYuUlBSULl3aCPWaOXMm0tLSMHToUERGmq8spxjKX8r+/PNPHDlyBM2bN8fp06exadOmdKczNTUVW7duxT333IOjR4/iyJEjOHLkCE6dOoUbbrgBS5cu9ZsCH2wGSyDatGnj/tIIXJpxFBsbix07dgC4NHtlwYIF6NSpE0qVKuWeV6lSJbRv3z7s5+TKlQsPPPCAux8dHY0HHngAhw8fxsqVKwFcEvhLSEjA3Xff7Z6XO3duDBgwACdPnsSSJUusz/j999+xaNEi3HHHHW4ZHDlyBEePHkVKSgq2bt2Kffv2Gdf06dPHKMfmzZvj4sWLAcNUwkHWg1OnTuHIkSNo2rQpHMfB6tWrr/j9gEu/dhw7dgx33323m0dHjhxBVFQUmjRpgm+++cY9N1++fJgyZQo2btyIFi1aYPbs2Rg3bhzKlSuXrmeHon///u6275fgc+fOYcGCBUGvkXl0/vx5HD16FJUqVUKhQoWwatUqv/NDlbmX/FEuP+Ha6q+++goA3JlCPjI6c0DWL98v0i1btsSOHTtw/Phx49ykpCSkpKQYf5s+fTqaN2+OwoULG/WpTZs2uHjxIpYuXeqmP1euXOjbt697bVRUFB5++OGw0tm8eXMcOnQImzdvBnBpRlSLFi3QvHlzfPvttwAu/droOI4xUypcG3PnnXdi5cqV2L59u/u3adOmISYmBrfeeiuA9PmrjHLnnXcaAum+d/P5sN9++w1Lly5Fr169/OxWepf2/uqrr9C4cWM3PB64NOu5T58+2LVrlxtS4aNnz56G7genMRhebVs4HDhwAKmpqejevTvi4uLcv994442oUaOGce706dMRFxeHG2+80ai7DRo0QIECBcKyheHW/xkzZiAiIgLDhg3zu0eocrp48SLmzZuHTp06oUKFCu7fS5YsiXvuuQffffcdTpw4YVxz//33IyoqKmT6fXTr1g0FCxZ092+77TaULFnStTvBkGX4xx9/4Pjx42jevHnA8gvVH3McBzNmzEDHjh3hOI6RnykpKTh+/Hi664WSc5k4cSLmz59v/Pv666+Nc2rVqoURI0bgnXfeQUpKCo4cOYL3338/oNZsqLoerp1PS0vDzJkz0bFjx4CaV6Hadbh9MS82LSPPCcSnn36KtLQ03HHHHca1CQkJqFy5snvt6tWrsXPnTgwcONBPisCLH+ratasxg9f37j169ECRIkXcv9epUwc33nhjQPvEY8TmzZvj6NGjfjZSEk7605OWcAllG2340vv5559nev9DyT7k6PA9AGjUqBE+/fRTnDt3DmvWrMFnn32GcePG4bbbbkNqaipq1KiB7du3IzIyMqRhW79+PZ566iksWrTIr2HzwMULW7duBQBrCMfx48eNTnlSUlLY9w/0caFw4cKuXsThw4dx5syZgKt4eFnZo1SpUn5ColWqVAFwKVb62muvxe7du1G5cmW/j3++abyhPhRt27YNjuPg6aefxtNPPx3wnMOHD6N06dLuPr+/Lx+lXoYX9uzZg6FDh+KLL77wu0d66kFm3w/4X526/vrrAx6PjY019q+77jr07dsXEydOREpKihtumdlERkYaAwrArCPBOHPmDMaMGYPJkydj3759RshqoDwKVeZe80e5/IRjq3fv3o3IyEij4wIAVatWzdCzv//+ewwbNgzLly/30104fvy40QkOZHu3bt2KX375JWgomE/we/fu3ShZsiQKFCiQrvT7PnR8++23KFOmDFavXo1nnnkGxYsXx4svvugei42NNcI1wrUxt99+OwYPHuzqjTiOg+nTp7saPr53Bbz5q4wSqj37Oq2hQj+9sHv3br9wMMD0VfJ56fUzXm1buGkHgMqVK/sdq1q1qvFRY+vWrTh+/HhAnU0gvIUGwq3/27dvR6lSpYzBTLj89ttvOH36dMC2Ur16daSlpWHv3r1uCCvgrZ8E+OdXREQEKlWqFHLFsC+//BLPPPMMUlNTcfbsWeN6JlR/7LfffsOxY8fw1ltv4a233gr4vOy8+INyeWjcuHFYQuePPPIIPvroI/z0008YPXp00HFNqLoerp0/d+4cTpw4kW7bG25fzItNy8hzgl3rOE7AZwNwQ8h9P+Zk1A+x3fK9ezDbN3fuXL+FHGz+KNi7hpP+9KQlXELZRht33nkn3nnnHdx33314/PHHccMNN6BLly647bbb/MabSs4lx3+U8hEdHY1GjRqhUaNGqFKlCnr27Inp06cH/MUuEMeOHUPLli0RGxuLkSNHomLFisiTJw9WrVqFxx57LENfZn3XvvDCC6hXr17Ac3gQ42W1p2C/FMrOb07Bl1f//ve//WYr+OAPaZn5/hcvXsSNN96I33//HY899hiqVauG/PnzY9++fejRo4fnepDZ9/Phu+6DDz4wBI998C9nZ8+edUUnt2/fjtOnT/vpNF1JHn74YUyePBkDBw5EcnIy4uLiEBERgbvuuitgHoUqc6/5o2QdGbXVPoL9MikXpgAu1fcbbrgB1apVw8svv4yyZcsiOjoaX331FcaNG+dXvwLZ3rS0NNx444149NFHAz7T9+E1o5QqVQpJSUlYunQpypcvD8dxkJycjOLFi+Nf//oXdu/ejW+//RZNmzZ1O2JebEypUqXQvHlzfPzxx3jiiSfwww8/YM+ePYYORXr8FRMRERHQ/nLZ+MgJPiy9afRq2zKbtLQ0xMfH4//+7/8CHg9HVzKr6r9XsmJVzG+//Ra33HILWrRogddffx0lS5ZE7ty5MXnyZEydOtXv/HB90z//+c+gHwR8+pqKwuzYscP9ALN27dp03ydcO//777+n+xnyOZe7L5aR56SlpSEiIgJff/11wPYbyt95JTPsVnbwmeH2wXxkJM158+bF0qVL8c0332D27NmYM2cOpk2bhuuvvx7z5s3zNGNWyb78LUdmvl8bDhw4AOCSiGZaWho2bNgQ1PguXrwYR48exaeffooWLVq4f9+5c6ffucEaYrC/+371j42NRZs2bcJ+j8wiPj4eefLkCbhSUDirB/nYv3+/3xfyLVu2AIArfJeYmIhffvkFaWlpxtdrX/hjYmIigOB55Ztlkzt37kzNq3Cn1q5duxZbtmzB+++/j27durl/nz9/frqe6+V+Xqb/+upUfHx8WPk0bNgwbNy4ES+++CIee+wxPP7448YqX4FIT1hMWloaduzYYQxSuI4E4pNPPkH37t3x0ksvuX/766+/wlq1LBBe80e5MrCtTkxMRFpaGrZv3278UucLZ5MULlw4YP3g2ZizZs3C2bNn8cUXXxi/1HkJ4axYsSJOnjwZsi4lJiZi4cKFOHnypNGRDZT+YDRv3hxLly5FUlIS6tWrh4IFC6Ju3bqIi4vDnDlzsGrVKowYMcI936vNuvPOO/HQQw9h8+bNmDZtGvLly4eOHTsa7wpkzF8VLlw44JT89IZU+/zCunXrrOd5sVmJiYkBy4V9VUYJ17Z5TTvwv9kBEn6nihUrYsGCBbjuuutCDoZsfZhw6n/FihUxd+5c/P7779bZUoGeU7x4ceTLly9omURGRqJs2bLW54eC88txHGzbts36EWjGjBnIkycP5s6di5iYGPfvkydPTlcafKuKXrx4UX2T4om0tDT06NEDsbGxGDhwIEaPHo3bbrvNXSxIEqquh2vnixcvjtjY2HTb3nD7Yl5sWkaeE+xax3GQlJRk/cDue8a6deusz/Dad/a9ezDbV6xYsXTNTGLCSb+XtITbB/OCLe8iIyNxww034IYbbsDLL7+M0aNH48knn8Q333yjtvRvQo6e8/bNN98E/MLqi3n1DWo6deqEyMhIjBw50u+XSd/1vq+s8n7nzp3D66+/7nf//PnzB5x272uo3EgbNGiAihUr4sUXX8TJkyf9rgu0lH1mEhUVhTZt2mDmzJnYv3+/+/dt27b5xazbuHDhgrs8OnApf958800UL14cDRo0AADcdNNNOHjwoLEK2oULFzBhwgQUKFDAXULcN0uH8yo+Ph6tWrXCm2++6Q5UJenNq/z584f1gSNQPXAcx2+51HDxcr9g9ScQKSkpiI2NxejRo3H+/Hm/4zKffvzxR7z44osYOHAg/t//+3945JFH8Nprr4XU9/KSHslrr73mbjuOg9deew25c+fGDTfcEPSaqKgov7Y8YcKEoL+4hMJL/iiXn3BttU/jjj+YytW9fFSsWBHHjx/HL7/84v7twIEDfktIB2qDx48f9zSovOOOO7B8+XLMnTvX79ixY8dw4cIFAJfs34ULF/DGG2+4xy9evIgJEyaE/azmzZtj165dmDZtmhvOFxkZiaZNm+Lll1/G+fPnDT0przara9euiIqKwn//+19Mnz4dN998s9HhzQx/VbFiRWzatMk4d82aNeleKad48eJo0aIF3nvvPezZs8c4Jt/bi8266aab8NNPP2H58uXu306dOoW33noL5cuXD0vHJBzCtW1e0l6yZEnUq1cP77//vtEXmT9/vp8W1h133IGLFy9i1KhRfve5cOGC8bxgfjLc+t+1a1c4jmN8NPXB5cTPiYqKQtu2bfH5558b4XSHDh3C1KlT0axZswyHXf/nP//Bn3/+6e5/8sknOHDggFVbMyoqChEREUZ57dq1CzNnzkxXGqKiotC1a1fMmDEj4EBffZMSjJdffhnLli3DW2+9hVGjRqFp06bo27ev36p9QOi6Hq6dj4yMRKdOnTBr1iysWLHC7zxfuw5mv8Lti3mxaYHISJ+vS5cuiIqKwogRI/xsteM4OHr0KADgmmuuQVJSEsaPH+/3nun1Q4D57vKadevWYd68ebjpppvCuk8owkm/l7SE2wfzQrC8CzRjzzfJRIZUKzmbHD1T6uGHH8bp06fRuXNnVKtWDefOncOyZcswbdo0lC9fHj179gRwKdzrySefxKhRo9C8eXN06dIFMTEx+Pnnn1GqVCmMGTMGTZs2ReHChdG9e3cMGDAAERER+OCDDwIOpBo0aIBp06Zh8ODBaNSoEQoUKICOHTuiYsWKKFSoECZNmoSCBQsif/78aNKkCZKSkvDOO++gffv2qFmzJnr27InSpUtj3759+OabbxAbG4tZs2Zd1rwaPnw45s2b52oLXbx4Ea+99hpq1aqF1NTUsO5RqlQpPP/889i1axeqVKmCadOmITU1FW+99ZYbc92nTx+8+eab6NGjB1auXIny5cvjk08+wffff4/x48e7wot58+ZFjRo1MG3aNFSpUgVFihRBrVq1UKtWLUycOBHNmjVD7dq1cf/996NChQo4dOgQli9fjl9//RVr1qzx/P4NGjTAG2+8gWeeeQaVKlVCfHx8wNjzatWqoWLFivj3v/+Nffv2ITY2FjNmzEi3PpWX+/k+7A0YMAApKSmIiorCXXfdFfC+sbGxeOONN3DvvffimmuuwV133YXixYtjz549mD17Nq677jq89tpr+Ouvv9C9e3dUrlwZzz77LABgxIgRmDVrFnr27Im1a9cG/QWmXr16iIqKwvPPP4/jx48jJiYG119/fVBtEgDIkycP5syZg+7du6NJkyb4+uuvMXv2bDzxxBPWMJGbb74ZH3zwAeLi4lCjRg0sX74cCxYscJdD9kq4+aNkDeHa6nr16uHuu+/G66+/juPHj6Np06ZYuHBhwBmdd911Fx577DF07twZAwYMcJd/rlKliqE/0bZtW0RHR6Njx4544IEHcPLkSbz99tuIj48P+OE7EI888gi++OIL3HzzzejRowcaNGiAU6dOYe3atfjkk0+wa9cuFCtWDB07dsR1112Hxx9/HLt27UKNGjXw6aefetIO8n1w2rx5M0aPHu3+vUWLFvj6668RExODRo0auX/3arPi4+PRunVrvPzyy/jzzz9x5513GscjIyMz7K969eqFl19+GSkpKejduzcOHz6MSZMmoWbNmlYhVhuvvvoqmjVrhmuuuQZ9+vRBUlISdu3ahdmzZ7s+zGdDn3zySdx1113InTs3OnbsGNDGPf744/jvf/+L9u3bY8CAAShSpAjef/997Ny5EzNmzMg0nYpwbZtXeztmzBh06NABzZo1Q69evfD7779jwoQJqFmzpjHIbNmyJR544AGMGTMGqampaNu2LXLnzo2tW7di+vTpeOWVV3Dbbbe5+RfIT4Zb/1u3bo17770Xr776KrZu3Yp27dohLS0N3377LVq3bu0ugtGgQQMsWLAAL7/8shuy2qRJEzzzzDOYP38+mjVrhoceegi5cuXCm2++ibNnz2Ls2LEZLosiRYqgWbNm6NmzJw4dOoTx48ejUqVKuP/++4Ne06FDB7z88sto164d7rnnHhw+fBgTJ05EpUqVjMGYF5577jl88803aNKkCe6//37UqFEDv//+O1atWoUFCxZkOGRKyXl8/fXXARdUatq0KSpUqICNGzfi6aefRo8ePdyZrVOmTEG9evXw0EMP4eOPPzauC1XXvdj50aNHY968eWjZsiX69OmD6tWr48CBA5g+fTq+++47FCpUyGq/wu2LhWvTApGRPl/FihXxzDPPYMiQIdi1axc6deqEggULYufOnfjss8/Qp08f/Pvf/0ZkZCTeeOMNdOzYEfXq1UPPnj1RsmRJbNq0CevXr3c/2nvpy/t44YUX0L59eyQnJ6N37944c+YMJkyYgLi4OAwfPtx6bbiEm/5w0xJuH8wLwXz4yJEjsXTpUnTo0AGJiYk4fPgwXn/9dZQpU8ZYrETJ4VyGFf2yjK+//trp1auXU61aNadAgQJOdHS0U6lSJefhhx92Dh065Hf+e++959SvX9+JiYlxChcu7LRs2dKZP3++e/z77793rr32Widv3rxOqVKl3GXLQcucnjx50rnnnnucQoUK+S1V+vnnnzs1atRwcuXK5bcE+OrVq50uXbo4RYsWdWJiYpzExETnjjvucBYuXOie41tKM9Cyl8GW2ezXr5/fubz8teM4zsKFC5369es70dHRTsWKFZ133nnH+X//7/85efLkCZbFLi1btnRq1qzprFixwklOTnby5MnjJCYmOq+99prfuYcOHXJ69uzpFCtWzImOjnZq164dcCn0ZcuWOQ0aNHCio6P9lnvfvn27061bNychIcHJnTu3U7p0aefmm292PvnkE/cc31K6vEytb0lcWWYHDx50OnTo4BQsWNAB4C57HejcDRs2OG3atHEKFCjgFCtWzLn//vvdpUvlewQqj0CEe78LFy44Dz/8sFO8eHEnIiIirHt/8803TkpKihMXF+fkyZPHqVixotOjRw9nxYoVjuM4zqBBg5yoqCjnxx9/NK5bsWKFkytXLqdv377u3wLVmbffftupUKGCExUVFXK58u7duzv58+d3tm/f7rRt29bJly+fU6JECWfYsGHu8uo+uLz/+OMPt84UKFDASUlJcTZt2uSXJi9lHk7+KFmDF1t95swZZ8CAAU7RokWd/PnzOx07dnT27t3rV2cc59Jy0bVq1XKio6OdqlWrOh9++GHAdvnFF184derUcfLkyeOUL1/eef7555333nvPb+nhxMREp0OHDgHf4c8//3SGDBniVKpUyYmOjnaKFSvmNG3a1HnxxRedc+fOuecdPXrUuffee53Y2FgnLi7Ouffee53Vq1f7tXcb8fHxDgAj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2RIvvfQSOnTogI8++ggrVqzAW2+95d7zkUcewZ133okWLVqgdevWmDNnDmbNmuUnzKwoiqJkPfxBIiYmJuDHPpvu4KZNmwLeOyUlBS+//DJatGiBihUrYuHChfj000/dgVfBggWRnJyMUaNGoXr16ihRogT++9//Yvny5X4fQRVFURQls9DwPUVRFI9k1ZTbO++8Ey+++CKGDh2KevXqITU1FXPmzHEHIXv27DF+hWratCmmTp2Kt956C3Xr1sUnn3yCmTNnolatWu45nTt3xqRJkzB27FjUrl0b77zzDmbMmOG3oouiKIqSfrKj7uArr7yCypUro1q1aoiOjkb//v3Rs2dP4xf+Dz74AI7joHTp0oiJicGrr76Ku++++7LNVFYURbka0fA9E/UwiqIoHslKR9K/f3/s3r0bZ8+exY8//mgs+7548WJMmTLFOP/222/H5s2bcfbsWaxbtw433XST3z179eqFrVu34syZM0hNTcWtt96arrQpiqIogcmOuoPFixfHzJkzcerUKezevRubNm1CgQIFUKFCBfecihUrYsmSJTh58iT27t2Ln376CefPnzfOURRFUTJGVowlli5dio4dO6JUqVKIiIjAzJkzjeM9evRARESE8Y/DULds2YJbb70VxYoVQ2xsLJo1a4ZvvvnGOGfPnj3o0KED8uXLh/j4eDzyyCN+ofWhyHHhe1wYHPsrYzf5Vx2OKZVxrTbdoFDPlPB9WINE6gidOnXKOMY6DjKuld+FY6mlTg+nlzsSUiuAY5E5vVJnhtMrY705bpmnmsvYea6k3KGyaW1x3LKMIea4Zb6PLBs5sAf8NUjkuRyDLeO1ATO2Wsa7A+a7clw6p698+fJBn8naK7Luclw61xUZO886EdwmpIZKUlKS9Vz53vxunH65L2O5+b4ce81x6xwnLuF2adOl4+d40Zrw3VvjwK88wcohlO2X5c3n8r7ULWANENmeuM5zumSbZU0Fqc0BmLaMtTpYf2r9+vXuNttHm74g23622VInjtssn1u9enV3m32gZOrUqcZ+xYoVjf1rr73W3ebwIznbDzBtVf369Y1j7KukHea8X7lyZdA0seYi+90lS5a426xvwfVI1o86deoYx+S7cdpZg0/mPWt7sfakfCbXjVKlShn7W7Zscbc5TIv1D6W2DLcJ1tKSafr222+NY3ythOuGtNnc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",
                         "text/plain": [
                             "<Figure size 1200x600 with 6 Axes>"
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
                 }
@@ -310,15 +314,15 @@
                 "key = jax.random.PRNGKey(0)\n",
                 "fig, axes = plt.subplots(ncols=3, figsize=(12, 6))\n",
                 "ax1, ax2, ax3 = axes\n",
                 "im1 = plot_image(\n",
                 "    compute_image(scattering_pipeline),\n",
                 "    fig,\n",
                 "    ax1,\n",
-                "    label=\"Scattering potential at exit plane\",\n",
+                "    label=\"Phase shifts at exit plane\",\n",
                 ")\n",
                 "im2 = plot_image(\n",
                 "    compute_image(optics_pipeline),\n",
                 "    fig,\n",
                 "    ax2,\n",
                 "    label=\"Squared wavefunction at detector plane\",\n",
                 ")\n",
```

### Comparing `cryojax-0.2.2rc1/docs/examples/simulate-micrograph.ipynb` & `cryojax-0.2.3rc1/docs/examples/simulate-micrograph.ipynb`

 * *Files 27% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9900519805372807%*

 * *Differences: {"'cells'": "{5: {'source': {insert: [(9, 'voltage_in_kilovolts = 300.0\\n'), (16, 'instrument = "*

 * *            "cs.Instrument(voltage_in_kilovolts, optics=optics)\\n')], delete: [16, 13]}}, 7: "*

 * *            "{'source': {insert: [(2, 'import equinox as eqx\\n'), (3, 'import equinox.internal as "*

 * *            "eqxi\\n'), (4, 'from jaxtyping import PRNGKeyArray, PyTree\\n'), (7, "*

 * *            "'@partial(eqx.filter_vmap, in_axes=(0, None), out_axes=eqxi.if_mapped(axis=0))\\n'), "*

 * *            "(8, 'def make_pipel […]*

```diff
@@ -72,22 +72,22 @@
                 "real_voxel_grid, voxel_size = read_array_with_spacing_from_mrc(filename)\n",
                 "potential = cs.FourierVoxelGridPotential.from_real_voxel_grid(\n",
                 "    real_voxel_grid, voxel_size, pad_scale=2\n",
                 ")\n",
                 "integrator = cs.FourierSliceExtract(interpolation_order=1)\n",
                 "\n",
                 "# ... and build the instrument\n",
+                "voltage_in_kilovolts = 300.0\n",
                 "optics = cs.WeakPhaseOptics(\n",
                 "    ctf=cs.CTF(\n",
                 "        defocus_u_in_angstroms=10000.0,\n",
                 "        defocus_v_in_angstroms=10000.0,\n",
-                "        voltage_in_kilovolts=300.0,\n",
                 "    )\n",
                 ")\n",
-                "instrument = cs.Instrument(optics)\n",
+                "instrument = cs.Instrument(voltage_in_kilovolts, optics=optics)\n",
                 "\n",
                 "# ... and finally the config\n",
                 "shape = (400, 600)\n",
                 "pixel_size = potential.voxel_size  # Angstroms\n",
                 "image_size = np.asarray(shape) * pixel_size\n",
                 "config = cs.ImageConfig(shape, pixel_size, pad_scale=1.1)"
             ]
@@ -103,65 +103,76 @@
             "cell_type": "code",
             "execution_count": 5,
             "metadata": {},
             "outputs": [],
             "source": [
                 "from functools import partial\n",
                 "\n",
-                "from jaxtyping import PRNGKeyArray\n",
+                "import equinox as eqx\n",
+                "import equinox.internal as eqxi\n",
+                "from jaxtyping import PRNGKeyArray, PyTree\n",
                 "\n",
                 "\n",
-                "@partial(jax.vmap, in_axes=[0, None])\n",
-                "def make_poses(\n",
-                "    key: PRNGKeyArray,\n",
-                "    config: cs.ImageConfig,\n",
-                "):\n",
+                "@partial(eqx.filter_vmap, in_axes=(0, None), out_axes=eqxi.if_mapped(axis=0))\n",
+                "def make_pipeline(key: PRNGKeyArray, no_vmap: tuple[PyTree, ...]) -> cs.ImagePipeline:\n",
+                "    config, potential, integrator, instrument = no_vmap\n",
                 "    # ... instantiate rotations\n",
                 "    rotation = SO3.sample_uniform(key)\n",
                 "    # ... now in-plane translation\n",
                 "    ny, nx = config.shape\n",
                 "    in_plane_offset_in_angstroms = (\n",
                 "        jax.random.uniform(key, (2,), minval=-0.45, maxval=0.45)\n",
                 "        * jnp.asarray((nx, ny))\n",
                 "        * config.pixel_size\n",
                 "    )\n",
                 "    # ... convert 2D in-plane translation to 3D, setting the out-of-plane translation to\n",
                 "    # zero\n",
                 "    offset_in_angstroms = jnp.pad(in_plane_offset_in_angstroms, ((0, 1),))\n",
-                "    # Build the pose and return\n",
-                "    return cs.QuaternionPose.from_rotation_and_translation(\n",
+                "    # ... build the pose\n",
+                "    pose = cs.QuaternionPose.from_rotation_and_translation(\n",
                 "        rotation, offset_in_angstroms\n",
-                "    )"
+                "    )\n",
+                "    # ... build the Specimen and ImagePipeline as usual and return\n",
+                "    specimen = cs.Specimen(potential, integrator, pose)\n",
+                "    return cs.ImagePipeline(config, specimen, instrument)"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "!!! info \"What's with the `out_axes=eqxi.if_mapped(axis=0)`?\"\n",
+                "    \n",
+                "    When we create a pytree with `eqx.filter_vmap` (or `jax.vmap`), `out_axes` should have the same structure as the output pytree. If `out_axes` is set to `None` at a particular leaf, this\n",
+                "    says that we do not want to broadcast that leaf (of course, this only works for unmapped leaves). By default `jax.vmap` sets `out_axes=0`, so all unmapped leaves get broadcasted. `equinox` allows us to pass `out_axes=eqxi.if_mapped(axes=0)`, which specifies *not* to broadcast pytree leaves unless the leaves are directly mapped.\n",
+                "\n",
+                "    When building an `ImagePipeline`, it is very important that we do not broadcast arbitrary leaves! For example, an `ImageConfig` stores the coordinate systems for our image. Without the `out_axes=eqxi.if_mapped(axes=0)` specification, the `make_pipeline` would output an `ImagePipeline.config` whose coordinate systems have a batch dimension. This takes up unecessary memory."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 6,
             "metadata": {},
             "outputs": [],
             "source": [
                 "# Generate RNG keys\n",
                 "number_of_poses = 20\n",
                 "keys = jax.random.split(jax.random.PRNGKey(12345), number_of_poses)\n",
                 "\n",
-                "# ... instantiate the poses\n",
-                "poses = make_poses(keys, config)\n",
-                "\n",
-                "# ... build the Specimen and ImagePipeline as usual\n",
-                "specimen = cs.Specimen(potential, integrator, poses)\n",
-                "pipeline = cs.ImagePipeline(config, specimen, instrument)"
+                "# ... instantiate the pipeline\n",
+                "pipeline = make_pipeline(keys, (config, potential, integrator, instrument))"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "This may be a little odd at first. We have contructed a pipeline, where if we were to directly call its `render` method, it would not work. Think of it this way: because we created our `pose`s with a `vmap`, functions can now only be called after crossing `vmap` boundaries. There is very good reason for this! To learn more, read the section of the equinox documentation on [model ensembling](https://docs.kidger.site/equinox/tricks/#ensembling).\n",
+                "This may be a little odd at first. We have contructed a pipeline, where if we were to directly call its `render` method, it would not work. Think of it this way: because we created our `pipeline`s with a `vmap`, functions can now only be called after crossing `vmap` boundaries. There is very good reason for this! To learn more, read the section of the equinox documentation on [model ensembling](https://docs.kidger.site/equinox/tricks/#ensembling).\n",
                 "\n",
-                "Now that we have an `ImagePipeline` with a batched set of poses, we need some way of telling our `vmap` exactly what pytree leaves are batched. One way `equinox` does this is by using pointers to particular pytree leaves to create what is called a `filter_spec`."
+                "Now that we have an `ImagePipeline` with a batched set of poses, we need some way of telling our `vmap` exactly what pytree leaves have batch dimensions. One way `equinox` does this is by using pointers to particular pytree leaves to create what is called a `filter_spec`."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 7,
             "metadata": {},
             "outputs": [],
@@ -222,15 +233,15 @@
                     },
                     "execution_count": 9,
                     "metadata": {},
                     "output_type": "execute_result"
                 },
                 {
                     "data": {
-                        "image/png": "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baNHHnlEuuqqqyQA0sc//nHppz/9qXTfffdJkiRJ999/v6TT6aT169dLX/3qV6XrrrtO8vl8ktvtlsbGxvgc11xzjQRA2rx5s3T22WdL3/nOd6Rbb7217Xvptp+oYbHnl6SX+rb8HiVJkv70pz8d1L9OP/10KRKJSAMDA9y3N2/eLGm1WukXv/iFFAqFpGuvvVa6+eab+R5zuVzHeyyVStKmTZskvV4vffKTn5S+9a1vSa973eskANLNN98sSdLCe/rpT38q+Xw+aevWrQf1EzUst+/QORbrw5IkSc8++6xkNpulwcFB6cYbb5RuuOEGKRgMSieddJKkHFYvuOACCYD07ne/W7r11lul888/XwIgnXPOOS37DQ0NSRs2bJDC4bB07bXXSjfddJPU19cn2Ww26Wc/+5k0ODgofeUrX5G+8pWvSE6nU1q3bp3UbDY7tjW96y1btkive93rpG9961vSJZdcIgmCIL3+9a+XRFHkfamfnnnmmdK3v/1t6dJLL5W0Wq10yimnSLVaTZIkSapWq9KaNWukSCQiffGLX5S+//3vS9ddd510yimnSOPj43yuL37xi5JGo5HOPfdc6Tvf+Q5/G8PDw1I6nV7SuXo49tAjFm3QjlgAkL785S/ztnQ6LZnNZkmj0Ui/+MUvePvu3bslANI111zD2yqVykEDwdjYmGQ0GqXrr7+et33961+XAPDkLkmSVC6XpY0bN7YM/KIoSqOjo9KOHTtaBohSqSStWbNGevOb39zxGX/4wx9KAKRvfOMbB/1G57vrrrskANIXv/jFlt/f/e53SxqNRtq3bx9vAyAZDIaWbc8884wEQPr2t7/N2772ta+pTmx0DkEQpOeff/6g30qlUsvftVpNOvHEE6UzzjiDt910000SACkej7d97scff5zJYDegCffOO+9s2b5161YpEAhIyWSStz3zzDOSIAjS+eefz9towD7vvPO6ul63/UQN3Tz/UokFAOmOO+7gbdS3BUGQ/vKXv/D2e++9t6t2vfnmmyUA0s9+9jPeVqvVpO3bt0s2m62FmAwNDUk7d+7seD7CcvsOnaObPnzOOedIJpNJmpiY4G27du2StFptC7F4+umnJQDShz/84ZbrfPrTn5YASP/5n//Z8qwApEceeYS3UZuazeaWa333u9896F2pgd71tm3bmBxIkiR99atflQBIv/vd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3/lOaLVaXHfddQf1Y0mSkEwmuz5XD8cmehaLI4h/+Id/wPXXX48LL7wQr371q/H3v/8dP//5z1tWCADwT//0T7jllltw3nnn4ROf+ATC4TB+/vOfw2QyAXhpxS8IAr7//e/jbW97G0444QRceOGF6Ovrw8zMDP70pz/B4XDgP/7jP9rez/nnn49/+7d/w+WXX47HHnsMr3vd61AsFvHAAw/gn//5n3H22WfjrLPOwhvf+EZ87nOfw/j4OE4++WTcd999+N3vfofLLrusReTWLbZt2wYA+NznPof3ve990Ov1OOusszqu8Hfu3IlvfOMbeOtb34r3v//9iMViuPXWW7Fu3To8++yzvN/111+PP//5z9i5cyeGhoYQi8Xwne98B/39/Zw7YmRkBC6XC7fffjvsdjusVitOPfXUrjUQhK997Wt429vehu3bt+NDH/oQyuUyvv3tb8PpdOLaa69dcrsQuu0naujm+U844QScdtppuPLKK5FKpeDxePCLX/zioEH+cOGiiy7Cd7/7XXzwgx/EE088geHhYfzqV7/C//zP/+Dmm28+SM+zXHTbd5aC6667Dvfccw9e97rX4Z//+Z+ZGJ1wwgkt5zz55JNxwQUX4Hvf+x4ymQxOP/10PPbYY/jJT36Cc845p8WKcDhRq9Xwpje9Ce9973uxZ88efOc738FrX/taFoj7/X5ceeWVuO666/DWt74V73jHO3i/U045Bf/n//wfAAt5Wy699FK85z3vwfr169FoNPDTn/4UWq0W73rXuwAsfF9f/OIXceWVV2J8fBznnHMO7HY7xsbG8Nvf/hYXXXQRPv3pT3d1rh6OURyFSJRjAu3CTa1W60H7nn766dIJJ5xw0HZlqFylUpE+9alPSeFwWDKbzdJrXvMa6dFHH5VOP/106fTTT2859sCBA9LOnTsls9ks+f1+6VOf+pT061//WgLQEuInSQthW+985zslr9crGY1GaWhoSHrve98rPfjgg4s+Z6lUkj73uc9Ja9askfR6vRQKhaR3v/vdLXkd8vm89MlPflKKRCKSXq+XRkdHpa997WstIa6StBCqd8kll6i2wwUXXNCy7YYbbpD6+vokQRBaQh/bnUOSJOkHP/iBNDo6KhmNRmnjxo3Sj370Iw7lJDz44IPS2WefLUUiEclgMEiRSEQ677zzpBdffLHlXL/73e+kzZs3SzqdbtEQyXbhppIkSQ888ID0mte8RjKbzZLD4ZDOOussadeuXS370D12CgGVYyn9RIlun3///v3SmWeeKRmNRikYDEpXXXWVdP/996uGm3bTtwmd3p8c8/Pz0oUXXij5fD7JYDBIW7ZsUX0HSw03XU7f6XQOtT788MMPS9u2bZMMBoO0du1a6fbbb1c9Z71el6677jr+xgYGBqQrr7xSqlQqXT2r2j2NjY1JAKSvfe1rbdtDkl4axx5++GHpoosuktxut2Sz2aT//b//d0uYNOGWW26RNm7cKOn1eikYDEoXX3wx552QpIVx6R//8R+lkZERyWQySR6PR3rjG98oPfDAAwed69e//rX02te+VrJarZLVapU2btwoXXLJJdKePXuWfK4eji1oJOkoKq16WBJuvvlmfPKTn8T09DT6+vqO9u300EMPqxw//vGPceGFF+Lxxx/HK1/5yqN9Oz28TNDTWKxSlMvllr8rlQq++93vYnR0tEcqeuihhx56WLXoaSxWKd75zndicHAQW7duRTabxc9+9jPs3r0bP//5z4/2rfXQQw899NBDW/SIxSrFjh078P3vfx8///nP0Ww2sXnzZvziF7/Aueeee7RvrYceeuihhx7aoqex6KGHHnrooYceVgw9jUUPPfTQQw899LBi6BGLHnrooYceeuhhxXBMaixEUcTs7CzsdvuKpGfuoYceeujh5QNJkpDP5xGJRFrSylcqFdRqtRW7jsFg4MSGLycck8Ridnb2oGp/PfTQQw899LAUTE1NcbGzSqWCNWvWIBqNrtj5Q6EQxsbGXnbk4pgkFpTy91vf+lbXFSOPF0iywmSku+1ZbQ4/VrqtJUWBuW6v205rrdFoDvqt23ulY+l4QRC4iupi11VeS62d6FnbtaH8+hqN5qC/5edZ7LrKbcp2Wclvp9M51L5TtX3l55DfazfPrtVqIYpi1+9mJdDufpdzPrq/lThftyiXy/j4xz/ekj6+VqshGo1icnISDodj2dfI5XIYHBxErVbrEYtjAdQRzWYzLBbLUb6bw4sj+bH10B400crNpp327bSfvPR5N+drd33lNvl1F7sHOaiPyc+ndu5OUO4nP0e7vztdXw30TGrn6bSt0/N020aLoV17t3tm5bO0a2flPvT/er2+ZUJuNBpcZE15zEqOIfLnPB7GJjXSZbfbV6RezbHeNsvB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",
+                        "image/png": "iVBORw0KGgoAAAANSUhEUgAAAhYAAAFNCAYAAABc5iZ6AAAAOXRFWHRTb2Z0d2FyZQBNYXRwbG90bGliIHZlcnNpb24zLjguMywgaHR0cHM6Ly9tYXRwbG90bGliLm9yZy/H5lhTAAAACXBIWXMAAA9hAAAPYQGoP6dpAAEAAElEQVR4nOy9eZRdZZU2/txz53kea0gllcoEgfgFhDiBgEZNoywVAb9PkFZpaVAR5acgyqTipy2ggqLt2CpLPxywW5GxBbsbFGQUQkKGmqtu3Xme7zm/P2rtzbkn5966laoklXCftVihzj3je97zvvvd+9nP1kiSJKGHHnrooYceeuhhGSAc6RvooYceeuihhx6OHfQMix566KGHHnroYdnQMyx66KGHHnrooYdlQ8+w6KGHHnrooYcelg09w6KHHnrooYceelg29AyLHnrooYceeuhh2dAzLHrooYceeuihh2VDz7DooYceeuihhx6WDT3Dooceeuihhx56WDb0DIseeugCTz75JF73utfBarVCo9Hg2WefPdK39KpAoVDAhz/8YYRCIWg0GlxxxRVH+pY64vrrr4dGoznSt9FDD0cUPcOiDX784x9Do9Hgb3/725G+lWMOjz32GK6//npkMpkjcv2ZmRlcf/31XRsH9Xod5557LlKpFG699Vb89Kc/xapVqw7tTfYAAPjyl7+MH//4x7j00kvx05/+FB/4wAeO9C310EMPC0B3pG+gh1cfHnvsMdxwww344Ac/CJfLddivPzMzgxtuuAFDQ0PYsmXLgvvv27cP4+Pj+Nd//Vd8+MMfPvQ32APjP//zP3HqqafiuuuuO9K30kMPPXSJnseihxUNURRRqVSO6D3EYjEAWFYjqFgsLtu5jmXEYrGDbveV0Hd66OHViJ5hsQh88IMfhM1mw8TEBP7hH/4BNpsNfX19uOOOOwAAf//733HGGWfAarVi1apVuOuuu1qOT6VS+PSnP43NmzfDZrPB4XDg7W9/O5577rkDrjU+Po53vvOdsFqtCAQC+OQnP4n7778fGo0GjzzySMu+f/3rX/G2t70NTqcTFosFp512Gv7nf/6nq2eqVCq4/vrrsW7dOphMJoTDYbz73e/Gvn37eJ9isYhPfepTGBgYgNFoxPr16/Ev//IvUBbG1Wg0uPzyy3HPPffg+OOPh9FoxHHHHYf77ruP97n++utx1VVXAQBWr14NjUYDjUaDsbGxlnP8/Oc/x3HHHQej0cjH/8u//Ate97rXwev1wmw2Y+vWrfjVr351wDM9+OCDeMMb3gCXywWbzYb169fjmmuuAQA88sgjOPnkkwEAF198MV//xz/+sWr7fPCDH8Rpp50GADj33HOh0Whw+umn8+//+Z//iTe+8Y2wWq1wuVx417vehZdeeqnlHBR337lzJ97//vfD7XbjDW94Q9t3sph+ooZOzw+8EuajNic88sgjB/Sv008/Hccffzyef/55nHbaabBYLFi7di23+6OPPopTTjkFZrMZ69evx0MPPdTVPcZiMXzoQx9CMBiEyWTCiSeeiJ/85CcH3Mvo6Cj+8Ic/HNBP1LAcfaebPkz47//+b5x88skwmUwYHh7Gd7/7XdX7ajQauOmmmzA8PAyj0YihoSFcc801qFarLfsNDQ3hH/7hH/DII4/gpJNOgtlsxubNm/l9/OY3v8HmzZthMpmwdetWPPPMMws1M7/rP//5z/inf/oneL1eOBwOXHjhhUin0wfs/+1vf5vbLhKJ4LLLLjsgZLlnzx685z3vQSgUgslkQn9/P84//3xks9mW/X72s59h69atMJvN8Hg8OP/88zE5OXlQ5+rhKIPUgyp+9KMfSQCkJ598krdddNFFkslkkjZt2iR99KMfle644w7pda97nQRA+tGPfiRFIhHpqquukr71rW9Jxx13nKTVaqX9+/fz8U8++aQ0PDwsffazn5W++93vSjfeeKPU19cnOZ1OaXp6mvcrFArSmjVrJLPZLH32s5+VbrvtNum1r32tdOKJJ0oApD/96U+878MPPywZDAZp27Zt0te//nXp1ltvlU444QTJYDBIf/3rXzs+Y6PRkM4880wJgHT++edLt99+u3TzzTdLZ5xxhnTPPfdIkiRJoihKZ5xxhqTRaKQPf/jD0u233y6dffbZEgDpiiuuaDkfAOnEE0+UwuGwdNNNN0m33XabtGbNGslisUiJREKSJEl67rnnpAsuuEACIN16663ST3/6U+mnP/2pVCgU+BwbN26U/H6/dMMNN0h33HGH9Mwzz0iSJEn9/f3SP//zP0u33367dMstt0ivfe1rJQDS73//e76HF154QTIYDNJJJ50kfeMb35DuvPNO6dOf/rT0pje9SZIkSYpGo9KNN94oAZAuueQSvv6+fftU2+ixxx6TrrnmGgmA9PGPf1z66U9/Kj3wwAOSJEnSgw8+KOl0OmndunXSV7/6VemGG26QfD6f5Ha7pdHRUT7HddddJwGQNm3aJL3rXe+Svv3tb0t33HFH2/fSbT9Rw0LPL0mv9G35PUqSJP3pT386oH+ddtppUiQSkQYGBrhvb9q0SdJqtdIvfvELKRQKSddff71022238T3mcrmO91gqlaSNGzdKer1e+uQnPyl985vflN74xjdKAKTbbrtNkqT59/TTn/5U8vl80pYtWw7oJ2pYat+hcyzUhyVJkp5//nnJbDZLg4OD0s033yzddNNNUjAYlE444QRJOaxedNFFEgDpve99r3THHXdIF154oQRAOuecc1r2W7VqlbR+/XopHA5L119/vXTrrbdKfX19ks1mk372s59Jg4OD0le+8hXpK1/5iuR0OqW1a9dKzWazY1vTu968ebP0xje+UfrmN78pXXbZZZIgCNKb3vQmSRRF3pf66VlnnSV961vfki6//HJJq9VKJ598slSr1SRJkqRqtSqtXr1aikQi0he/+EXp+9//vnTDDTdIJ598sjQ2Nsbn+uIXvyhpNBrpvPPOk7797W/ztzE0NCSl0+lFnauHow89w6IN2hkWAKQvf/nLvC2dTktms1nSaDTSL37xC96+a9cuCYB03XXX8bZKpXLAQDA6OioZjUbpxhtv5G1f//rXJQA8uUuSJJXLZWnDhg0tA78oitLIyIi0ffv2lgGiVCpJq1evlt7ylrd0fMYf/vCHEgDplltuOeA3Ot8999wjAZC++MUvtvz+3ve+V9JoNNLevXt5GwDJYDC0bHvuueckANK3vvUt3va1r31NdWKjcwiCIL344osH/FYqlVr+rtVq0vHHHy+dccYZvO3WW2+VAEjxeLztcz/55JNsDHYDmnDvvvvulu1btmyRAoGAlEwmedtzzz0nCYIgXXjhhbyNBuwLLrigq+t120/U0M3zL9awACDdddddvI36tiAI0l/+8hfefv/993fVrrfddpsEQPrZz37G22q1mrRt2zbJZrO1GCarVq2SduzY0fF8hKX2HTpHN334nHPOkUwmkzQ+Ps7bdu7cKWm12hbD4tlnn5UASB/+8IdbrvPpT39aAiD953/+Z8uzApAee+wx3kZtajabW6713e9+94B3pQZ611u3bmXjQJIk6atf/aoEQPrd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3e9+N7RaLW644YYD+rEkSUgmk12fq4ejEz2PxWHEP/zDP+DGG2/ExRdfjNe97nX4+9//jp///OctKwQA+Kd/+ifcfvvtuOCCC/CJT3wC4XAYP//5z2EymQC8suIXBAHf//738fa3vx3HHXccLr74YvT19WF6ehp/+tOf4HA48B//8R9t7+fCCy/Ev/3bv+HKK6/EE088gTe+8Y0oFot46KGH8M///M9417vehbPPPhtvfvOb8bnPfQ5jY2M48cQT8cADD+B3v/sdrrjiihaSW7fYunUrAOBzn/sczj//fOj1epx99tkdV/g7duzALbfcgre97W14//vfj1gshjvuuANr167F888/z/vdeOON+POf/4wdO3Zg1apViMVi+Pa3v43+/n7WjhgeHobL5cKdd94Ju90Oq9WKU045pWsOBOFrX/sa3v72t2Pbtm340Ic+hHK5jG9961twOp24/vrrF90uhG77iRq6ef7jjjsOp556Kq6++mqkUil4PB784he/OGCQP1S45JJL8N3vfhcf/OAH8dRTT2FoaAi/+tWv8D//8z+47bbbDuDzLBXd9p3F4IYbbsB9992HN77xjfjnf/5nNoyOO+64lnOeeOKJuOiii/C9730PmUwGp512Gp544gn85Cc/wTnnnNPiRTiUqNVqOPPMM/G+970Pu3fvxre//W284Q1vYIK43+/H1VdfjRtuuAFve9vb8M53vpP3O/nkk/F//s//ATCv23L55Zfj3HPPxbp169BoNPDTn/4UWq0W73nPewDMf19f/OIXcfXVV2NsbAznnHMO7HY7RkdH8dvf/haXXHIJPv3pT3d1rh6OUhyBTJSjAu3STa1W6wH7nnbaadJxxx13wHZlqlylUpE+9alPSeFwWDKbzdLrX/966fHHH5dOO+006bTTTms5dv/+/dKOHTsks9ks+f1+6VOf+pT061//WgLQkuInSfNpW+9+97slr9crGY1GadWqVdL73vc+6eGHH17wOUulkvS5z31OWr16taTX66VQKCS9973vbdF1yOfz0ic/+UkpEolIer1eGhkZkb72ta+1pLhK0nyq3mWXXabaDhdddFHLtptuuknq6+uTBEFoSX1sdw5JkqQf/OAH0sjIiGQ0GqUNGzZIP/rRjziVk/Dwww9L73rXu6RIJCIZDAYpEolIF1xwgfTyyy+3nOt3v/udtGnT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",
                         "text/plain": [
                             "<Figure size 550x550 with 2 Axes>"
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
                 }
```

### Comparing `cryojax-0.2.2rc1/docs/examples/test-multiatom.ipynb` & `cryojax-0.2.3rc1/docs/examples/test-multiatom.ipynb`

 * *Files identical despite different names*

### Comparing `cryojax-0.2.2rc1/docs/examples/data/ribosome_4ug0_particles.star` & `cryojax-0.2.3rc1/docs/examples/data/ribosome_4ug0_particles.star`

 * *Files identical despite different names*

### Comparing `cryojax-0.2.2rc1/src/cryojax/constants/element_params.npy` & `cryojax-0.2.3rc1/src/cryojax/constants/element_params.npy`

 * *Files identical despite different names*

### Comparing `cryojax-0.2.2rc1/src/cryojax/coordinates/_coordinates.py` & `cryojax-0.2.3rc1/src/cryojax/coordinates/_coordinates.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,127 +3,136 @@
 """
 
 from abc import abstractmethod
 from typing import Any, Optional
 from typing_extensions import Self
 
 import equinox as eqx
-import jax
 import jax.numpy as jnp
+import numpy as np
 from equinox import AbstractVar
-from jaxtyping import Array, ArrayLike, Float
-
-from ..typing import (
-    Image,
-    ImageCoords,
-    PointCloudCoords2D,
-    PointCloudCoords3D,
-    VolumeCoords,
-    VolumeSliceCoords,
-)
+from jaxtyping import Array, Float, Inexact
 
 
 class AbstractCoordinates(eqx.Module, strict=True):
     """
     A base class that wraps a coordinate array.
     """
 
     array: AbstractVar[Any]
 
     @abstractmethod
     def get(self) -> Any:
         """Get the coordinates."""
         raise NotImplementedError
 
-    def __mul__(self, arr: ArrayLike) -> Self:
+    def __mul__(
+        self, real_number: float | Float[np.ndarray, ""] | Float[Array, ""]
+    ) -> Self:
         # The following line seems to be required for differentiability with
         # respect to arr
         rescaled_array = jnp.where(
-            self.array != 0.0, self.array * jnp.asarray(arr), 0.0
+            self.array != 0.0, self.array * jnp.asarray(real_number), 0.0
         )
         return eqx.tree_at(lambda x: x.array, self, rescaled_array)
 
-    def __rmul__(self, arr: ArrayLike) -> Self:
+    def __rmul__(
+        self, real_number: float | Float[np.ndarray, ""] | Float[Array, ""]
+    ) -> Self:
         rescaled_array = jnp.where(
-            self.array != 0.0, jnp.asarray(arr) * self.array, 0.0
+            self.array != 0.0, jnp.asarray(real_number) * self.array, 0.0
         )
         return eqx.tree_at(lambda x: x.array, self, rescaled_array)
 
-    def __truediv__(self, arr: ArrayLike) -> Self:
+    def __truediv__(
+        self, real_number: float | Float[np.ndarray, ""] | Float[Array, ""]
+    ) -> Self:
         rescaled_array = jnp.where(
-            self.array != 0.0, self.array / jnp.asarray(arr), 0.0
+            self.array != 0.0, self.array / jnp.asarray(real_number), 0.0
         )
         return eqx.tree_at(lambda x: x.array, self, rescaled_array)
 
 
 class CoordinateList(AbstractCoordinates, strict=True):
     """
     A Pytree that wraps a coordinate list.
     """
 
-    array: PointCloudCoords3D | PointCloudCoords2D = eqx.field(converter=jnp.asarray)
+    array: Float[Array, "size 3"] | Float[Array, "size 2"] = eqx.field(
+        converter=jnp.asarray
+    )
 
-    def __init__(self, coordinate_list: PointCloudCoords2D | PointCloudCoords3D):
+    def __init__(
+        self, coordinate_list: Float[Array, "size 2"] | Float[Array, "size 3"]
+    ):
         self.array = coordinate_list
 
-    def get(self) -> PointCloudCoords3D | PointCloudCoords2D:
+    def get(self) -> Float[Array, "size 3"] | Float[Array, "size 2"]:
         return self.array
 
 
 class CoordinateGrid(AbstractCoordinates, strict=True):
     """
     A Pytree that wraps a coordinate grid.
     """
 
-    array: ImageCoords | VolumeCoords = eqx.field(converter=jnp.asarray)
+    array: Float[Array, "y_dim x_dim 2"] | Float[Array, "z_dim y_dim x_dim 3"] = (
+        eqx.field(converter=jnp.asarray)
+    )
 
     def __init__(
         self,
         shape: tuple[int, ...],
-        grid_spacing: float | ArrayLike = 1.0,
+        grid_spacing: float | Float[np.ndarray, ""] = 1.0,
     ):
         self.array = make_coordinates(shape, grid_spacing)
 
-    def get(self) -> ImageCoords | VolumeCoords:
-        return jax.lax.stop_gradient(self.array)
+    def get(
+        self,
+    ) -> Float[Array, "y_dim x_dim 2"] | Float[Array, "z_dim y_dim x_dim 3"]:
+        return self.array
 
 
 class FrequencyGrid(AbstractCoordinates, strict=True):
     """
     A Pytree that wraps a frequency grid.
     """
 
-    array: ImageCoords | VolumeCoords = eqx.field(converter=jnp.asarray)
+    array: Float[Array, "y_dim x_dim 2"] | Float[Array, "z_dim y_dim x_dim 3"] = (
+        eqx.field(converter=jnp.asarray)
+    )
 
     def __init__(
         self,
         shape: tuple[int, ...],
-        grid_spacing: float | ArrayLike = 1.0,
+        grid_spacing: float | Float[np.ndarray, ""] = 1.0,
         half_space: bool = True,
     ):
         self.array = make_frequencies(shape, grid_spacing, half_space=half_space)
 
-    def get(self) -> ImageCoords | VolumeCoords:
-        return jax.lax.stop_gradient(self.array)
+    def get(
+        self,
+    ) -> Float[Array, "y_dim x_dim 2"] | Float[Array, "z_dim y_dim x_dim 3"]:
+        return self.array
 
 
 class FrequencySlice(AbstractCoordinates, strict=True):
     """
     A Pytree that wraps a frequency slice.
 
     Unlike a `FrequencyGrid`, a `FrequencySlice` has the zero frequency
     component in the center.
     """
 
-    array: VolumeSliceCoords = eqx.field(converter=jnp.asarray)
+    array: Float[Array, "1 y_dim x_dim 3"] = eqx.field(converter=jnp.asarray)
 
     def __init__(
         self,
         shape: tuple[int, int],
-        grid_spacing: float | ArrayLike = 1.0,
+        grid_spacing: float | Float[np.ndarray, ""] = 1.0,
         half_space: bool = True,
     ):
         frequency_slice = make_frequencies(shape, grid_spacing, half_space=half_space)
         if half_space:
             frequency_slice = jnp.fft.fftshift(frequency_slice, axes=(0,))
         else:
             frequency_slice = jnp.fft.fftshift(frequency_slice, axes=(0, 1))
@@ -134,21 +143,21 @@
                 mode="constant",
                 constant_values=0.0,
             ),
             axis=0,
         )
         self.array = frequency_slice
 
-    def get(self) -> VolumeSliceCoords:
-        return jax.lax.stop_gradient(self.array)
+    def get(self) -> Float[Array, "1 y_dim x_dim 3"]:
+        return self.array
 
 
 def make_coordinates(
-    shape: tuple[int, ...], grid_spacing: float | ArrayLike = 1.0
-) -> Float[Array, "*shape len(shape)"]:
+    shape: tuple[int, ...], grid_spacing: float | Float[np.ndarray, ""] = 1.0
+) -> Float[Array, "*shape ndim"]:
     """
     Create a real-space cartesian coordinate system on a grid.
 
     Arguments
     ---------
     shape :
         Shape of the voxel grid, with
@@ -165,17 +174,17 @@
         shape, grid_spacing=grid_spacing, real_space=True
     )
     return coordinate_grid
 
 
 def make_frequencies(
     shape: tuple[int, ...],
-    grid_spacing: float | ArrayLike = 1.0,
+    grid_spacing: float | Float[np.ndarray, ""] = 1.0,
     half_space: bool = True,
-) -> Float[Array, "*shape len(shape)"]:
+) -> Float[Array, "*shape ndim"]:
     """
     Create a fourier-space cartesian coordinate system on a grid.
     The zero-frequency component is in the beginning.
 
     Arguments
     ---------
     shape :
@@ -198,15 +207,17 @@
         grid_spacing=grid_spacing,
         real_space=False,
         half_space=half_space,
     )
     return frequency_grid
 
 
-def cartesian_to_polar(freqs: ImageCoords, square: bool = False) -> tuple[Image, Image]:
+def cartesian_to_polar(
+    freqs: Float[Array, "y_dim x_dim 2"], square: bool = False
+) -> tuple[Inexact[Array, "y_dim x_dim"], Inexact[Array, "y_dim x_dim"]]:
     """
     Convert from cartesian to polar coordinates.
 
     Arguments
     ---------
     freqs :
         The cartesian coordinate system.
@@ -222,18 +233,18 @@
     else:
         kr = jnp.sqrt(k_sqr)
         return kr, theta
 
 
 def _make_coordinates_or_frequencies(
     shape: tuple[int, ...],
-    grid_spacing: float | ArrayLike = 1.0,
+    grid_spacing: float | Float[np.ndarray, ""] = 1.0,
     real_space: bool = False,
     half_space: bool = True,
-) -> Float[Array, "*shape len(shape)"]:
+) -> Float[Array, "*shape ndim"]:
     ndim = len(shape)
     coords1D = []
     for idx in range(ndim):
         if real_space:
             c1D = _make_coordinates_or_frequencies_1d(
                 shape[idx], grid_spacing, real_space
             )
@@ -264,15 +275,15 @@
         )
 
     return coords
 
 
 def _make_coordinates_or_frequencies_1d(
     size: int,
-    grid_spacing: float | ArrayLike,
+    grid_spacing: float | Float[np.ndarray, ""],
     real_space: bool = False,
     rfftfreq: Optional[bool] = None,
 ) -> Float[Array, " size"]:
     """One-dimensional coordinates in real or fourier space"""
     if real_space:
         make_1d = (
             lambda size, dx: jnp.fft.fftshift(jnp.fft.fftfreq(size, 1 / dx)) * size
```

### Comparing `cryojax-0.2.2rc1/src/cryojax/core/_errors.py` & `cryojax-0.2.3rc1/src/cryojax/core/_errors.py`

 * *Files identical despite different names*

### Comparing `cryojax-0.2.2rc1/src/cryojax/core/_filter_specs.py` & `cryojax-0.2.3rc1/src/cryojax/core/_filter_specs.py`

 * *Files identical despite different names*

### Comparing `cryojax-0.2.2rc1/src/cryojax/core/_filtered_transformations.py` & `cryojax-0.2.3rc1/src/cryojax/core/_filtered_transformations.py`

 * *Files identical despite different names*

### Comparing `cryojax-0.2.2rc1/src/cryojax/data/_dataset.py` & `cryojax-0.2.3rc1/src/cryojax/data/_dataset.py`

 * *Files identical despite different names*

### Comparing `cryojax-0.2.2rc1/src/cryojax/data/_relion.py` & `cryojax-0.2.3rc1/src/cryojax/data/_relion.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,19 +5,18 @@
 from typing import Any, Callable, final
 
 import equinox as eqx
 import jax.numpy as jnp
 import mrcfile
 import numpy as np
 import pandas as pd
-from jaxtyping import Float, Int, Shaped
+from jaxtyping import Array, Float, Int
 
 from ..io import read_and_validate_starfile
 from ..simulator import CTF, EulerAnglePose, ImageConfig
-from ..typing import RealImage
 from ._dataset import AbstractDataset
 from ._particle_stack import AbstractParticleStack
 
 
 RELION_REQUIRED_OPTICS_KEYS = [
     "rlnImageSize",
     "rlnVoltage",
@@ -35,22 +34,22 @@
 
 
 class RelionParticleStack(AbstractParticleStack):
     """A particle stack with information imported from
     [RELION](https://relion.readthedocs.io/en/release-5.0/).
     """
 
-    image_stack: Shaped[RealImage, "..."]
+    image_stack: Float[Array, "... y_dim x_dim"]
     config: ImageConfig
     pose: EulerAnglePose
     ctf: CTF
 
     def __init__(
         self,
-        image_stack: Shaped[RealImage, "..."] | Float[np.ndarray, "... Ny Nx"],
+        image_stack: Float[Array, "... y_dim x_dim"],
         config: ImageConfig,
         pose: EulerAnglePose,
         ctf: CTF,
     ):
         # Set image stack and config as is
         self.image_stack = jnp.asarray(image_stack)
         self.config = config
@@ -309,15 +308,15 @@
         # instantiation
         pose = eqx.tree_at(
             lambda p: tuple([getattr(p, name) for name in pose_parameter_names]),
             pose,
             tuple([jnp.asarray(value) for value in pose_parameter_values]),
         )
 
-        return RelionParticleStack(image_stack, config, pose, ctf)
+        return RelionParticleStack(jnp.asarray(image_stack), config, pose, ctf)
 
     @final
     def __len__(self) -> int:
         return len(self.data_blocks["particles"])
 
 
 @dataclasses.dataclass(frozen=True)
```

### Comparing `cryojax-0.2.2rc1/src/cryojax/image/__init__.py` & `cryojax-0.2.3rc1/src/cryojax/image/__init__.py`

 * *Files identical despite different names*

### Comparing `cryojax-0.2.2rc1/src/cryojax/image/_average.py` & `cryojax-0.2.3rc1/src/cryojax/image/_average.py`

 * *Files 27% similar despite different names*

```diff
@@ -5,73 +5,68 @@
 from functools import partial
 from typing import overload
 
 import jax
 import jax.numpy as jnp
 from jaxtyping import Array, Float, Inexact
 
-from ..typing import (
-    Image,
-    RealImage,
-    RealVolume,
-    Volume,
-)
-
-
-Vector = Inexact[Array, "N"]
-RealVector = Float[Array, "N"]
-
 
 @overload
 def radial_average(
-    image: Image,
-    radial_grid: RealImage,
-    bins: RealVector,
-) -> Vector: ...
+    image: Inexact[Array, "y_dim x_dim"],
+    radial_grid: Float[Array, "y_dim x_dim"],
+    bins: Float[Array, " n_bins"],
+) -> Inexact[Array, " n_bins"]: ...
 
 
 @overload
 def radial_average(
-    image: Volume,
-    radial_grid: RealVolume,
-    bins: RealVector,
-) -> Vector: ...
+    image: Inexact[Array, "z_dim y_dim x_dim"],
+    radial_grid: Float[Array, "z_dim y_dim x_dim"],
+    bins: Float[Array, " n_bins"],
+) -> Inexact[Array, " n_bins"]: ...
 
 
 @overload
 def radial_average(
-    image: Image,
-    radial_grid: RealImage,
-    bins: RealVector,
+    image: Inexact[Array, "y_dim x_dim"],
+    radial_grid: Float[Array, "y_dim x_dim"],
+    bins: Float[Array, " n_bins"],
     *,
     to_grid: bool = False,
     interpolation_mode: str = "nearest",
-) -> tuple[Vector, Image]: ...
+) -> tuple[Inexact[Array, " n_bins"], Inexact[Array, "y_dim x_dim"]]: ...
 
 
 @overload
 def radial_average(
-    image: Volume,
-    radial_grid: RealVolume,
-    bins: RealVector,
+    image: Inexact[Array, "z_dim y_dim x_dim"],
+    radial_grid: Float[Array, "z_dim y_dim x_dim"],
+    bins: Float[Array, " n_bins"],
     *,
     to_grid: bool = False,
     interpolation_mode: str = "nearest",
-) -> tuple[Vector, Volume]: ...
+) -> tuple[Inexact[Array, " n_bins"], Inexact[Array, "z_dim y_dim x_dim"]]: ...
 
 
 @partial(jax.jit, static_argnames=["to_grid", "interpolation_mode"])
 def radial_average(
-    image: Image | Volume,
-    radial_grid: RealImage | RealVolume,
-    bins: RealVector,
+    image: Inexact[Array, "y_dim x_dim"] | Inexact[Array, "z_dim y_dim x_dim"],
+    radial_grid: Float[Array, "y_dim x_dim"] | Float[Array, "z_dim y_dim x_dim"],
+    bins: Float[Array, " n_bins"],
     *,
     to_grid: bool = False,
     interpolation_mode: str = "nearest",
-) -> Vector | tuple[Vector, Image | Volume]:
+) -> (
+    Inexact[Array, " n_bins"]
+    | tuple[
+        Inexact[Array, " n_bins"],
+        Inexact[Array, "y_dim x_dim"] | Inexact[Array, "z_dim y_dim x_dim"],
+    ]
+):
     """
     Radially average vectors r with a given magnitude
     coordinate system |r|.
 
     Arguments
     ---------
     image :
```

### Comparing `cryojax-0.2.2rc1/src/cryojax/image/_map_coordinates.py` & `cryojax-0.2.3rc1/src/cryojax/image/_map_coordinates.py`

 * *Files identical despite different names*

### Comparing `cryojax-0.2.2rc1/src/cryojax/image/_rescale_pixel_size.py` & `cryojax-0.2.3rc1/src/cryojax/image/_rescale_pixel_size.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 """
 Routines for rescaling image pixel size.
 """
 
 import jax
 import jax.numpy as jnp
 from jax.image import scale_and_translate
-
-from ..typing import RealImage, RealNumber
+from jaxtyping import Array, Float
 
 
 def rescale_pixel_size(
-    image: RealImage,
-    current_pixel_size: RealNumber,
-    new_pixel_size: RealNumber,
+    image: Float[Array, "y_dim x_dim"],
+    current_pixel_size: Float[Array, ""],
+    new_pixel_size: Float[Array, ""],
     method: str = "bicubic",
     antialias: bool = False,
-) -> RealImage:
+) -> Float[Array, "y_dim x_dim"]:
     """
     Measure an image at a given pixel size using interpolation.
 
     For more detail, see ``cryojax.utils.interpolation.scale``.
 
     Parameters
     ----------
```

### Comparing `cryojax-0.2.2rc1/src/cryojax/image/operators/__init__.py` & `cryojax-0.2.3rc1/src/cryojax/image/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `cryojax-0.2.2rc1/src/cryojax/image/operators/_operator.py` & `cryojax-0.2.3rc1/src/cryojax/image/operators/_operator.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,17 +5,15 @@
 from abc import abstractmethod
 from typing import Any, Callable
 from typing_extensions import override
 
 import jax
 import jax.numpy as jnp
 from equinox import AbstractVar, field, Module, Partial
-from jaxtyping import Array, Shaped
-
-from ...typing import Image, RealNumber, Volume
+from jaxtyping import Array, Float, Inexact
 
 
 class AbstractImageOperator(Module, strict=True):
     """
     The base class for image operators that contain
     model parameters and compute an ``Array`` at runtime.
     """
@@ -62,83 +60,95 @@
     Attributes
     ----------
     operator :
         The operator. Note that this is automatically
         computed upon instantiation.
     """
 
-    buffer: AbstractVar[Image | Volume]
-
-    def __call__(self, image: Image | Volume) -> Image | Volume:
+    buffer: AbstractVar[
+        Inexact[Array, "y_dim x_dim"] | Inexact[Array, "z_dim y_dim x_dim"]
+    ]
+
+    def __call__(
+        self, image: Inexact[Array, "y_dim x_dim"] | Inexact[Array, "z_dim y_dim x_dim"]
+    ) -> Inexact[Array, "y_dim x_dim"] | Inexact[Array, "z_dim y_dim x_dim"]:
         return image * jax.lax.stop_gradient(self.buffer)
 
     def __mul__(self, other) -> "AbstractImageMultiplier":
         return ProductImageMultiplier(operator1=self, operator2=other)
 
     def __rmul__(self, other) -> "AbstractImageMultiplier":
         return ProductImageMultiplier(operator1=other, operator2=self)
 
 
 class Constant(AbstractImageOperator, strict=True):
     """An operator that is a constant."""
 
-    value: Shaped[RealNumber, "..."] = field(default=1.0, converter=jnp.asarray)
+    value: Float[Array, "..."] = field(default=1.0, converter=jnp.asarray)
 
     @override
-    def __call__(self, *args: Any, **kwargs: Any) -> RealNumber:
+    def __call__(self, *args: Any, **kwargs: Any) -> Float[Array, ""]:
         return self.value
 
 
 Constant.__init__.__doc__ = """**Arguments:**
 
 - `value`: The value of the constant
 """
 
 
 class Lambda(AbstractImageOperator, strict=True):
     """An operator that calls a custom function."""
 
-    fn: Callable[[Array], Image | Volume] = field(static=True)
+    fn: Callable[
+        [Array], Inexact[Array, "y_dim x_dim"] | Inexact[Array, "z_dim y_dim x_dim"]
+    ] = field(static=True)
 
     @override
-    def __call__(self, *args: Any, **kwargs: Any) -> Image | Volume:
+    def __call__(
+        self, *args: Any, **kwargs: Any
+    ) -> Inexact[Array, "y_dim x_dim"] | Inexact[Array, "z_dim y_dim x_dim"]:
         return self.fn(*args, **kwargs)
 
 
 Lambda.__init__.__doc__ = """**Arguments:**
 
 - `fn`: The `Callable` wrapped into a `AbstractImageOperator`.
 """
 
 
 class Empirical(AbstractImageOperator, strict=True):
     """This operator stores and returns an array, rather than
     computing one from a model.
     """
 
-    array: Shaped[Image, "..."] | Shaped[Volume, "..."] | Shaped[RealNumber, "..."]
-    amplitude: Shaped[RealNumber, "..."] = field(default=1.0, converter=jnp.asarray)
+    array: (
+        Inexact[Array, "... y_dim x_dim"]
+        | Inexact[Array, "... z_dim y_dim x_dim"]
+        | Float[Array, "..."]
+    )
+    amplitude: Float[Array, "..."] = field(default=1.0, converter=jnp.asarray)
 
     @override
-    def __call__(self, *args: Any, **kwargs: Any) -> Image:
+    def __call__(self, *args: Any, **kwargs: Any) -> Inexact[Array, "y_dim x_dim"]:
         """Return the scaled and offset measurement."""
         return self.amplitude * jax.lax.stop_gradient(self.array)
 
 
 Empirical.__init__.__doc__ = """**Arguments:**
 
 - `array`: The array to be returned upon calling `Empirical`.
 - `amplitude`: An amplitude scaling for `array`.
 """
 
 
 class ProductImageMultiplier(AbstractImageMultiplier, strict=True):
     """A helper to represent the product of two operators."""
 
-    buffer: Image | Volume
+    buffer: Inexact[Array, "y_dim x_dim"] | Inexact[Array, "z_dim y_dim x_dim"]
 
     operator1: AbstractImageMultiplier
     operator2: AbstractImageMultiplier
 
     def __init__(
         self,
         operator1: AbstractImageMultiplier,
```

### Comparing `cryojax-0.2.2rc1/src/cryojax/inference/distributions/_gaussian_distributions.py` & `cryojax-0.2.3rc1/src/cryojax/inference/distributions/_gaussian_distributions.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,39 +5,38 @@
 from typing import Optional
 from typing_extensions import override
 
 import jax.numpy as jnp
 import jax.random as jr
 import numpy as np
 from equinox import field
-from jaxtyping import PRNGKeyArray, Shaped
+from jaxtyping import Array, Complex, Float, PRNGKeyArray
 
 from ...core import error_if_not_positive
 from ...image.operators import Constant, FourierOperatorLike
 from ...simulator import AbstractPipeline
-from ...typing import ComplexImage, Image, RealNumber
 from ._distribution import AbstractDistribution
 
 
 class IndependentFourierGaussian(AbstractDistribution, strict=True):
     r"""A gaussian noise model, where each fourier mode is independent.
 
     This computes the likelihood in Fourier space,
     so that the variance to be an arbitrary noise power spectrum.
     """
 
     pipeline: AbstractPipeline
     variance: FourierOperatorLike
-    contrast_scale: Shaped[RealNumber, "..."] = field(converter=error_if_not_positive)
+    contrast_scale: Float[Array, ""] = field(converter=error_if_not_positive)
 
     def __init__(
         self,
         pipeline: AbstractPipeline,
         variance: Optional[FourierOperatorLike] = None,
-        contrast_scale: float | RealNumber = 1.0,
+        contrast_scale: float | Float[Array, ""] = 1.0,
     ):
         """**Arguments:**
 
         - `pipeline`: The image formation model.
         - `variance`: The variance of each fourier mode. By default,
                       `cryojax.image.operators.Constant(1.0)`.
         - `contrast_scale`: The standard deviation of an image simulated
@@ -45,37 +44,53 @@
                             `1.0`.
         """
         self.pipeline = pipeline
         self.variance = variance or Constant(1.0)
         self.contrast_scale = jnp.asarray(contrast_scale)
 
     @override
-    def render(self, *, get_real: bool = True) -> Image:
+    def render(
+        self, *, get_real: bool = True
+    ) -> (
+        Float[Array, "{self.pipeline.config.y_dim} {self.pipeline.config.x_dim}"]
+        | Complex[Array, "{self.pipeline.config.y_dim} {self.config.x_dim//2+1}"]
+    ):
         """Render the image formation model."""
         return self.contrast_scale * self.pipeline.render(
             normalize=True, get_real=get_real
         )
 
     @override
-    def sample(self, key: PRNGKeyArray, *, get_real: bool = True) -> Image:
+    def sample(
+        self, key: PRNGKeyArray, *, get_real: bool = True
+    ) -> (
+        Float[Array, "{self.pipeline.config.y_dim} {self.pipeline.config.x_dim}"]
+        | Complex[Array, "{self.pipeline.config.y_dim} {self.config.x_dim//2+1}"]
+    ):
         """Sample from the gaussian noise model."""
         N_pix = np.prod(self.pipeline.config.padded_shape)
         freqs = self.pipeline.config.wrapped_padded_frequency_grid_in_angstroms.get()
         # Compute the zero mean variance and scale up to be independent of the number of
         # pixels
         std = jnp.sqrt(N_pix * self.variance(freqs))
         noise = self.pipeline.crop_and_apply_operators(
             std * jr.normal(key, shape=freqs.shape[0:-1]).at[0, 0].set(0.0),
             get_real=get_real,
         )
         image = self.render(get_real=get_real)
         return image + noise
 
     @override
-    def log_likelihood(self, observed: ComplexImage) -> RealNumber:
+    def log_likelihood(
+        self,
+        observed: Complex[
+            Array,
+            "{self.pipeline.config.y_dim} {self.pipeline.config.x_dim//2+1}",
+        ],
+    ) -> Float[Array, ""]:
         """Evaluate the log-likelihood of the gaussian noise model.
 
         **Arguments:**
 
         - `observed` : The observed data in fourier space.
         """
         N_pix = np.prod(self.pipeline.config.shape)
```

### Comparing `cryojax-0.2.2rc1/src/cryojax/inference/transforms/__init__.py` & `cryojax-0.2.3rc1/src/cryojax/inference/transforms/__init__.py`

 * *Files identical despite different names*

### Comparing `cryojax-0.2.2rc1/src/cryojax/inference/transforms/_lie_group_transforms.py` & `cryojax-0.2.3rc1/src/cryojax/inference/transforms/_lie_group_transforms.py`

 * *Files identical despite different names*

### Comparing `cryojax-0.2.2rc1/src/cryojax/inference/transforms/_transforms.py` & `cryojax-0.2.3rc1/src/cryojax/inference/transforms/_transforms.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,18 +7,17 @@
 from typing_extensions import overload
 
 import equinox as eqx
 import jax
 import jax.numpy as jnp
 import jax.tree_util as jtu
 from equinox import AbstractVar, field, Module
-from jaxtyping import Array, PyTree
+from jaxtyping import Array, Float, PyTree
 
 from ...core import error_if_not_positive, error_if_zero
-from ...typing import RealNumber
 
 
 def _is_transformed(x: Any) -> bool:
     return isinstance(x, AbstractParameterTransform)
 
 
 def _resolve_transform(x: Any) -> Any:
@@ -158,22 +157,22 @@
 
     **Attributes:**
 
     - `transformed_parameter`: The rescaled parameter.
     """
 
     transformed_parameter: Array
-    scaling: RealNumber = field(converter=error_if_zero)
-    shift: RealNumber
+    scaling: Float[Array, ""] = field(converter=error_if_zero)
+    shift: Float[Array, ""]
 
     def __init__(
         self,
         parameter: Array,
-        scaling: RealNumber | float,
-        shift: RealNumber | float = 0.0,
+        scaling: Float[Array, ""] | float,
+        shift: Float[Array, ""] | float = 0.0,
     ):
         """**Arguments:**
 
         - `parameter`: The parameter to be rescaled.
 
         - `scaling`: The scale factor.
```

### Comparing `cryojax-0.2.2rc1/src/cryojax/io/__init__.py` & `cryojax-0.2.3rc1/src/cryojax/io/__init__.py`

 * *Files identical despite different names*

### Comparing `cryojax-0.2.2rc1/src/cryojax/io/_cif.py` & `cryojax-0.2.3rc1/src/cryojax/io/_cif.py`

 * *Files identical despite different names*

### Comparing `cryojax-0.2.2rc1/src/cryojax/io/_gemmi.py` & `cryojax-0.2.3rc1/src/cryojax/io/_gemmi.py`

 * *Files identical despite different names*

### Comparing `cryojax-0.2.2rc1/src/cryojax/io/_mdtraj.py` & `cryojax-0.2.3rc1/src/cryojax/io/_mdtraj.py`

 * *Files identical despite different names*

### Comparing `cryojax-0.2.2rc1/src/cryojax/io/_mrc.py` & `cryojax-0.2.3rc1/src/cryojax/io/_mrc.py`

 * *Files 4% similar despite different names*

```diff
@@ -60,15 +60,15 @@
         filename, get_spacing=True, mmap=mmap, permissive=permissive
     )
 
     return array, grid_spacing
 
 
 def write_image_to_mrc(
-    image: Float[Array, "N1 N2"],
+    image: Float[Array, "y_dim x_dim"],
     pixel_size: Float[Array, ""] | Float[np.ndarray, ""] | float,
     filename: str | pathlib.Path,
     overwrite: bool = False,
     compression: Optional[str] = None,
 ):
     """Write an image stack to an MRC file.
 
@@ -95,15 +95,15 @@
     # Create new file and write
     with mrcfile.new(filename, compression=compression, overwrite=overwrite) as mrc:
         mrc.set_data(image_as_numpy)
         mrc.voxel_size = pixel_size_as_numpy
 
 
 def write_image_stack_to_mrc(
-    image_stack: Float[Array, "M N1 N2"],
+    image_stack: Float[Array, "M y_dim x_dim"],
     pixel_size: Float[Array, ""] | Float[np.ndarray, ""] | float,
     filename: str | pathlib.Path,
     overwrite: bool = False,
     compression: Optional[str] = None,
 ):
     """Write an image stack to an MRC file.
 
@@ -131,15 +131,15 @@
     with mrcfile.new(filename, compression=compression, overwrite=overwrite) as mrc:
         mrc.set_data(image_stack_as_numpy)
         mrc.set_image_stack()
         mrc.voxel_size = (1.0, pixel_size_as_numpy, pixel_size_as_numpy)
 
 
 def write_volume_to_mrc(
-    voxel_grid: Float[Array, "N1 N2 N3"],
+    voxel_grid: Float[Array, "z_dim y_dim x_dim"],
     voxel_size: Float[Array, ""] | Float[np.ndarray, ""] | float,
     filename: str | pathlib.Path,
     overwrite: bool = False,
     compression: Optional[str] = None,
 ):
     """Write a voxel grid to an MRC file.
```

### Comparing `cryojax-0.2.2rc1/src/cryojax/io/_pdb.py` & `cryojax-0.2.3rc1/src/cryojax/io/_pdb.py`

 * *Files identical despite different names*

### Comparing `cryojax-0.2.2rc1/src/cryojax/io/_starfile.py` & `cryojax-0.2.3rc1/src/cryojax/io/_starfile.py`

 * *Files identical despite different names*

### Comparing `cryojax-0.2.2rc1/src/cryojax/rotations/_lie_group.py` & `cryojax-0.2.3rc1/src/cryojax/rotations/_lie_group.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 """
 Abstraction of rotations represented by matrix lie groups.
 """
 
 from abc import abstractmethod
-from typing import cast, ClassVar, Type
+from typing import cast, ClassVar
 from typing_extensions import override, Self
 
 import equinox as eqx
 import jax
 import jax.numpy as jnp
 from equinox import AbstractClassVar, field
 from jaxtyping import Array, Float, PRNGKeyArray
 
-from ..typing import RealNumber
 from ._rotation import AbstractRotation
 
 
 class AbstractMatrixLieGroup(AbstractRotation, strict=True):
     """Base class for a rotation that is represented by
     a matrix lie group.
 
@@ -28,28 +27,28 @@
 
     parameter_dimension: AbstractClassVar[int]
     tangent_dimension: AbstractClassVar[int]
     matrix_dimension: AbstractClassVar[int]
 
     @classmethod
     @abstractmethod
-    def exp(cls: Type[Self], tangent: Array) -> Self:
+    def exp(cls, tangent: Array) -> Self:
         """Computes the exponential map of an element of the
         lie algebra.
         """
         raise NotImplementedError
 
     @abstractmethod
     def log(self) -> Array:
         """Computes the logarithmic map of the lie group element."""
         raise NotImplementedError
 
     @classmethod
     @abstractmethod
-    def from_matrix(cls: Type[Self], matrix: Array) -> Self:
+    def from_matrix(cls, matrix: Array) -> Self:
         """Computes the group element from a rotation matrix."""
         raise NotImplementedError
 
     @abstractmethod
     def as_matrix(self) -> Array:
         """Represent the group element as a rotation matrix."""
         raise NotImplementedError
@@ -78,20 +77,20 @@
     """
 
     space_dimension: ClassVar[int] = 3
     parameter_dimension: ClassVar[int] = 4
     tangent_dimension: ClassVar[int] = 3
     matrix_dimension: ClassVar[int] = 3
 
-    wxyz: Float[Array, "... 4"] = field(converter=jnp.asarray)
+    wxyz: Float[Array, "4"] = field(converter=jnp.asarray)
 
     @override
-    def apply(self, vector: Float[Array, "3"]) -> Float[Array, "3"]:
+    def apply(self, target: Float[Array, "3"]) -> Float[Array, "3"]:
         # Compute using quaternion multiplys.
-        padded_target = jnp.concatenate([jnp.zeros(1), vector])
+        padded_target = jnp.concatenate([jnp.zeros(1), target])
         return (self @ SO3(wxyz=padded_target) @ self.inverse()).wxyz[1:]
 
     @override
     def compose(self, other: Self) -> Self:
         w0, x0, y0, z0 = self.wxyz
         w1, x1, y1, z1 = other.wxyz
         return type(self)(
@@ -108,36 +107,36 @@
     def inverse(self) -> Self:
         # Negate complex terms.
         return eqx.tree_at(
             lambda R: R.wxyz, self, self.wxyz * jnp.array([1, -1, -1, -1])
         )
 
     @classmethod
-    def from_x_radians(cls: Type[Self], angle: RealNumber) -> Self:
+    def from_x_radians(cls, angle: Float[Array, ""]) -> Self:
         """Generates a x-axis rotation."""
         return cls.exp(jnp.asarray([angle, 0.0, 0.0]))
 
     @classmethod
-    def from_y_radians(cls: Type[Self], angle: RealNumber) -> Self:
+    def from_y_radians(cls, angle: Float[Array, ""]) -> Self:
         """Generates a x-axis rotation."""
         return cls.exp(jnp.asarray([0.0, angle, 0.0]))
 
     @classmethod
-    def from_z_radians(cls: Type[Self], angle: RealNumber) -> Self:
+    def from_z_radians(cls, angle: Float[Array, ""]) -> Self:
         """Generates a x-axis rotation."""
         return cls.exp(jnp.asarray([0.0, 0.0, angle]))
 
     @override
     @classmethod
     def identity(cls) -> Self:
         return cls(jnp.asarray([1.0, 0.0, 0.0, 0.0]))
 
     @override
     @classmethod
-    def from_matrix(cls: Type[Self], matrix: Float[Array, "3 3"]) -> Self:
+    def from_matrix(cls, matrix: Float[Array, "3 3"]) -> Self:
         # Modified from:
         # > "Converting a Rotation Matrix to a Quaternion" from Mike Day
         # > https://d3cw3dd2w32x2b.cloudfront.net/wp-content/uploads/2015/01/matrix-to-quat.pdf
 
         def case0(m):
             t = 1 + m[0, 0] - m[1, 1] - m[2, 2]
             q = jnp.array(
@@ -220,15 +219,15 @@
                 [1.0 - q[2, 2] - q[3, 3], q[1, 2] - q[3, 0], q[1, 3] + q[2, 0]],
                 [q[1, 2] + q[3, 0], 1.0 - q[1, 1] - q[3, 3], q[2, 3] - q[1, 0]],
                 [q[1, 3] - q[2, 0], q[2, 3] + q[1, 0], 1.0 - q[1, 1] - q[2, 2]],
             ]
         )
 
     @classmethod
-    def exp(cls: Type[Self], tangent: Float[Array, "3"]) -> Self:
+    def exp(cls, tangent: Float[Array, "3"]) -> Self:
         # Reference:
         # > https://github.com/strasdat/Sophus/blob/a0fe89a323e20c42d3cecb590937eb7a06b8343a/sophus/so3.hpp#L583
         theta_squared = tangent @ tangent
         theta_pow_4 = theta_squared * theta_squared
         use_taylor = theta_squared < _get_epsilon(tangent.dtype)
 
         # Shim to avoid NaNs in jnp.where branches, which cause failures for
@@ -308,15 +307,15 @@
     @override
     def normalize(self) -> Self:
         return eqx.tree_at(
             lambda R: R.wxyz, self, self.wxyz / jnp.linalg.norm(self.wxyz)
         )
 
     @classmethod
-    def sample_uniform(cls: Type[Self], key: PRNGKeyArray) -> Self:
+    def sample_uniform(cls, key: PRNGKeyArray) -> Self:
         # Uniformly sample over S^3.
         # > Reference: http://planning.cs.uiuc.edu/node198.html
         u1, u2, u3 = jax.random.uniform(
             key=key,
             shape=(3,),
             minval=jnp.zeros(3),
             maxval=jnp.array([1.0, 2.0 * jnp.pi, 2.0 * jnp.pi]),
@@ -356,15 +355,15 @@
 
     space_dimension: ClassVar[int] = 3
     parameter_dimension: ClassVar[int] = 7
     tangent_dimension: ClassVar[int] = 6
     matrix_dimension: ClassVar[int] = 4
 
     rotation: SO3
-    xyz: Float[Array, "... 3"]
+    xyz: Float[Array, "3"]
 
     @override
     def apply(self, target: Float[Array, "3"]) -> Float[Array, "3"]:
         return self.rotation @ target + self.xyz
 
     @override
     def compose(self, other: Self) -> Self:
@@ -372,35 +371,35 @@
         return cls(
             rotation=self.rotation @ other.rotation,
             xyz=(self.rotation @ other.xyz) + self.xyz,
         )
 
     @override
     @classmethod
-    def identity(cls: Type[Self]) -> Self:
+    def identity(cls) -> Self:
         return cls(rotation=SO3.identity(), xyz=jnp.zeros(3, dtype=float))
 
     @override
     @classmethod
-    def from_matrix(cls: Type[Self], matrix: Float[Array, "4 4"]) -> Self:
+    def from_matrix(cls, matrix: Float[Array, "4 4"]) -> Self:
         # Currently assumes bottom row is [0, 0, 0, 1].
         return cls(
             rotation=SO3.from_matrix(matrix[:3, :3]),
             xyz=matrix[:3, 3],
         )
 
     @override
     def as_matrix(self) -> Float[Array, "4 4"]:
         return (
             jnp.eye(4).at[:3, :3].set(self.rotation.as_matrix()).at[:3, 3].set(self.xyz)
         )
 
     @override
     @classmethod
-    def exp(cls: Type[Self], tangent: Float[Array, "6"]) -> Self:
+    def exp(cls, tangent: Float[Array, "6"]) -> Self:
         # Reference:
         # > https://github.com/strasdat/Sophus/blob/a0fe89a323e20c42d3cecb590937eb7a06b8343a/sophus/se3.hpp#L761
         # assumes tangent is ordered as (x, y, z, w_x, w_y, w_z)
         rotation = SO3.exp(tangent[3:])
         theta_squared = tangent[3:] @ tangent[3:]
         use_taylor = theta_squared < _get_epsilon(theta_squared.dtype)
         # Shim to avoid NaNs in jnp.where branches, which cause failures for
@@ -488,15 +487,15 @@
     def inverse(self) -> Self:
         cls = type(self)
         inverse_rotation = self.rotation.inverse()
         return cls(rotation=inverse_rotation, xyz=-(inverse_rotation @ self.xyz))
 
     @override
     @classmethod
-    def sample_uniform(cls: Type[Self], key: PRNGKeyArray) -> Self:
+    def sample_uniform(cls, key: PRNGKeyArray) -> Self:
         key0, key1 = jax.random.split(key)
         return cls(
             rotation=SO3.sample_uniform(key0),
             xyz=jax.random.uniform(key=key1, shape=(3,), minval=-1.0, maxval=1.0),
         )
```

### Comparing `cryojax-0.2.2rc1/src/cryojax/rotations/_rotation.py` & `cryojax-0.2.3rc1/src/cryojax/rotations/_rotation.py`

 * *Files identical despite different names*

### Comparing `cryojax-0.2.2rc1/src/cryojax/simulator/__init__.py` & `cryojax-0.2.3rc1/src/cryojax/simulator/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,37 +10,33 @@
     DiscreteConformation as DiscreteConformation,
 )
 from ._detector import (
     AbstractDetector as AbstractDetector,
     AbstractDQE as AbstractDQE,
     GaussianDetector as GaussianDetector,
     IdealDQE as IdealDQE,
-    NullDetector as NullDetector,
-    NullDQE as NullDQE,
     PoissonDetector as PoissonDetector,
 )
 from ._dose import ElectronDose as ElectronDose
 from ._ice import (
     AbstractIce as AbstractIce,
     GaussianIce as GaussianIce,
-    NullIce as NullIce,
 )
 from ._instrument import Instrument as Instrument
 from ._integrators import (
     AbstractPotentialIntegrator as AbstractPotentialIntegrator,
     extract_slice as extract_slice,
     extract_slice_with_cubic_spline as extract_slice_with_cubic_spline,
     FourierSliceExtract as FourierSliceExtract,
     NufftProject as NufftProject,
     project_with_nufft as project_with_nufft,
 )
 from ._optics import (
     AbstractOptics as AbstractOptics,
     CTF as CTF,
-    NullOptics as NullOptics,
     WeakPhaseOptics as WeakPhaseOptics,
 )
 from ._pipeline import (
     AbstractPipeline as AbstractPipeline,
     AssemblyPipeline as AssemblyPipeline,
     ImagePipeline as ImagePipeline,
 )
```

### Comparing `cryojax-0.2.2rc1/src/cryojax/simulator/_config.py` & `cryojax-0.2.3rc1/src/cryojax/simulator/_config.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 """
 The image configuration and utility manager.
 """
 
+import math
 from functools import cached_property
 from typing import Any, Callable, Optional, Union
 
 import jax
 import jax.numpy as jnp
 from equinox import field, Module
-from jaxtyping import Shaped
+from jaxtyping import Array, Complex, Float
 
 from ..coordinates import CoordinateGrid, FrequencyGrid
 from ..core import error_if_not_positive
 from ..image import (
     crop_to_shape,
     irfftn,
     pad_to_shape,
     rescale_pixel_size,
     resize_with_crop_or_pad,
     rfftn,
 )
-from ..typing import Image, RealImage, RealNumber
 
 
 class ImageConfig(Module, strict=True):
     """Configuration and utilities for an electron microscopy image.
 
     **Attributes:**
 
@@ -39,46 +39,46 @@
         set with the `pad_scale` variable during initialization.
     - `pad_mode`:
         The method of image padding. By default, ``"constant"``.
         For all options, see ``jax.numpy.pad``.
     - `rescale_method`:
         The interpolation method for pixel size rescaling. See
         ``jax.image.scale_and_translate`` for options.
-    - `wrapped_frequency_grid`:
+    - `wrapped_frequency_grid_in_pixels`:
         The fourier wavevectors in the imaging plane, wrapped in
         a `FrequencyGrid` object.
-    - `wrapped_padded_frequency_grid`:
+    - `wrapped_padded_frequency_grid_in_pixels`:
         The fourier wavevectors in the imaging plane
         in the padded coordinate system, wrapped in
         a `FrequencyGrid` object.
-    - `wrapped_coordinate_grid`:
+    - `wrapped_coordinate_grid_in_pixels`:
         The coordinates in the imaging plane, wrapped
         in a `CoordinateGrid` object.
-    - `wrapped_padded_coordinate_grid`:
+    - `wrapped_padded_coordinate_grid_in_pixels`:
         The coordinates in the imaging plane
         in the padded coordinate system, wrapped in a
         `CoordinateGrid` object.
     """
 
     shape: tuple[int, int] = field(static=True)
-    pixel_size: Shaped[RealNumber, "..."] = field(converter=error_if_not_positive)
+    pixel_size: Float[Array, ""] = field(converter=error_if_not_positive)
 
     padded_shape: tuple[int, int] = field(static=True)
     pad_mode: Union[str, Callable] = field(static=True)
     rescale_method: str = field(static=True)
 
-    wrapped_frequency_grid: FrequencyGrid
-    wrapped_padded_frequency_grid: FrequencyGrid
-    wrapped_coordinate_grid: CoordinateGrid
-    wrapped_padded_coordinate_grid: CoordinateGrid
+    wrapped_frequency_grid_in_pixels: FrequencyGrid
+    wrapped_padded_frequency_grid_in_pixels: FrequencyGrid
+    wrapped_coordinate_grid_in_pixels: CoordinateGrid
+    wrapped_padded_coordinate_grid_in_pixels: CoordinateGrid
 
     def __init__(
         self,
         shape: tuple[int, int],
-        pixel_size: float | Shaped[RealNumber, "..."],
+        pixel_size: float | Float[Array, ""],
         padded_shape: Optional[tuple[int, int]] = None,
         *,
         pad_scale: float = 1.0,
         pad_mode: Union[str, Callable] = "constant",
         rescale_method: str = "bicubic",
     ):
         """**Arguments:**
@@ -94,45 +94,55 @@
         self.rescale_method = rescale_method
         # Set shape after padding
         if padded_shape is None:
             self.padded_shape = (int(pad_scale * shape[0]), int(pad_scale * shape[1]))
         else:
             self.padded_shape = padded_shape
         # Set coordinates
-        self.wrapped_frequency_grid = FrequencyGrid(shape=self.shape)
-        self.wrapped_padded_frequency_grid = FrequencyGrid(shape=self.padded_shape)
-        self.wrapped_coordinate_grid = CoordinateGrid(shape=self.shape)
-        self.wrapped_padded_coordinate_grid = CoordinateGrid(shape=self.padded_shape)
+        self.wrapped_frequency_grid_in_pixels = FrequencyGrid(shape=self.shape)
+        self.wrapped_padded_frequency_grid_in_pixels = FrequencyGrid(
+            shape=self.padded_shape
+        )
+        self.wrapped_coordinate_grid_in_pixels = CoordinateGrid(shape=self.shape)
+        self.wrapped_padded_coordinate_grid_in_pixels = CoordinateGrid(
+            shape=self.padded_shape
+        )
 
     def __check_init__(self):
         if self.padded_shape[0] < self.shape[0] or self.padded_shape[1] < self.shape[1]:
             raise AttributeError(
                 "ImageConfig.padded_shape is less than ImageConfig.shape in one or "
                 "more dimensions."
             )
 
     @cached_property
     def wrapped_coordinate_grid_in_angstroms(self) -> CoordinateGrid:
-        return self.pixel_size * self.wrapped_coordinate_grid  # type: ignore
+        return self.pixel_size * self.wrapped_coordinate_grid_in_pixels  # type: ignore
 
     @cached_property
     def wrapped_frequency_grid_in_angstroms(self) -> FrequencyGrid:
-        return self.wrapped_frequency_grid / self.pixel_size
+        return self.wrapped_frequency_grid_in_pixels / self.pixel_size
 
     @cached_property
     def wrapped_padded_coordinate_grid_in_angstroms(self) -> CoordinateGrid:
-        return self.pixel_size * self.wrapped_padded_coordinate_grid  # type: ignore
+        return self.pixel_size * self.wrapped_padded_coordinate_grid_in_pixels  # type: ignore
 
     @cached_property
     def wrapped_padded_frequency_grid_in_angstroms(self) -> FrequencyGrid:
-        return self.wrapped_padded_frequency_grid / self.pixel_size
+        return self.wrapped_padded_frequency_grid_in_pixels / self.pixel_size
 
     def rescale_to_pixel_size(
-        self, image: Image, current_pixel_size: RealNumber, is_real: bool = True
-    ) -> RealImage:
+        self,
+        real_or_fourier_image: (
+            Float[Array, "{self.padded_y_dim} {self.padded_x_dim}"]
+            | Complex[Array, "{self.padded_y_dim} {self.padded_x_dim//2+1}"]
+        ),
+        current_pixel_size: Float[Array, ""],
+        is_real: bool = True,
+    ) -> Complex[Array, "{self.padded_y_dim} {self.padded_x_dim//2+1}"]:
         """Rescale the image pixel size using real-space interpolation. Only
         interpolate if the `pixel_size` is not the `current_pixel_size`."""
         if is_real:
             rescale_fn = lambda im: rescale_pixel_size(
                 im, current_pixel_size, self.pixel_size, method=self.rescale_method
             )
         else:
@@ -145,23 +155,53 @@
                 )
             )
         null_fn = lambda im: im
         return jax.lax.cond(
             jnp.isclose(current_pixel_size, self.pixel_size),
             null_fn,
             rescale_fn,
-            image,
+            real_or_fourier_image,
         )
 
-    def crop_to_shape(self, image: RealImage) -> RealImage:
+    def crop_to_shape(
+        self, image: Float[Array, "y_dim x_dim"]
+    ) -> Float[Array, "{self.y_dim} {self.x_dim}"]:
         """Crop an image."""
         return crop_to_shape(image, self.shape)
 
-    def pad_to_padded_shape(self, image: RealImage, **kwargs: Any) -> RealImage:
+    def pad_to_padded_shape(
+        self, image: Float[Array, "y_dim x_dim"], **kwargs: Any
+    ) -> Float[Array, "{self.padded_y_dim} {self.padded_x_dim}"]:
         """Pad an image."""
         return pad_to_shape(image, self.padded_shape, mode=self.pad_mode, **kwargs)
 
-    def crop_or_pad_to_padded_shape(self, image: RealImage, **kwargs: Any) -> RealImage:
+    def crop_or_pad_to_padded_shape(
+        self, image: Float[Array, "y_dim x_dim"], **kwargs: Any
+    ) -> Float[Array, "{self.padded_y_dim} {self.padded_x_dim}"]:
         """Reshape an image using cropping or padding."""
         return resize_with_crop_or_pad(
             image, self.padded_shape, mode=self.pad_mode, **kwargs
         )
+
+    @property
+    def n_pix(self) -> int:
+        return math.prod(self.shape)
+
+    @property
+    def y_dim(self) -> int:
+        return self.shape[0]
+
+    @property
+    def x_dim(self) -> int:
+        return self.shape[1]
+
+    @property
+    def padded_y_dim(self) -> int:
+        return self.padded_shape[0]
+
+    @property
+    def padded_x_dim(self) -> int:
+        return self.padded_shape[1]
+
+    @property
+    def padded_n_pix(self) -> int:
+        return math.prod(self.padded_shape)
```

### Comparing `cryojax-0.2.2rc1/src/cryojax/simulator/_detector.py` & `cryojax-0.2.3rc1/src/cryojax/simulator/_detector.py`

 * *Files 27% similar despite different names*

```diff
@@ -6,85 +6,71 @@
 from typing import Optional
 from typing_extensions import override
 
 import jax.numpy as jnp
 import jax.random as jr
 import numpy as np
 from equinox import AbstractVar, field, Module
-from jaxtyping import PRNGKeyArray, Shaped
+from jaxtyping import Array, Complex, Float, PRNGKeyArray
 
 from ..core import error_if_not_fractional
 from ..image import irfftn, rfftn
 from ..image.operators import AbstractFourierOperator
-from ..typing import ComplexImage, ImageCoords, RealImage, RealNumber
 from ._config import ImageConfig
-from ._dose import ElectronDose
 
 
 class AbstractDQE(AbstractFourierOperator, strict=True):
     r"""Base class for a detector DQE."""
 
-    fraction_detected_electrons: AbstractVar[Shaped[RealNumber, "..."]]
+    fraction_detected_electrons: AbstractVar[Float[Array, ""]]
 
     @abstractmethod
     def __call__(
         self,
-        frequency_grid_maybe_in_angstroms: ImageCoords,
+        frequency_grid_in_angstroms_or_pixels: Float[Array, "y_dim x_dim 2"],
         *,
-        pixel_size: Optional[RealNumber] = None,
-    ) -> RealImage | RealNumber:
+        pixel_size: Optional[Float[Array, ""]] = None,
+    ) -> Float[Array, "y_dim x_dim"]:
         """**Arguments:**
 
-        - `frequency_grid_maybe_in_angstroms`: A frequency grid given in units of
-                                               nyquist.
+        - `frequency_grid_in_angstroms_or_pixels`: A frequency grid
+                                                   given in angstroms
+                                                   or pixels. If given
+                                                   in angstroms, `pixel_size`
+                                                   must be passed
+        - `pixel_size`: The pixel size of `frequency_grid_in_angstroms_or_pixels`.
         """
         raise NotImplementedError
 
 
-class NullDQE(AbstractDQE, strict=True):
-    r"""A model for a null DQE."""
-
-    fraction_detected_electrons: Shaped[RealNumber, "..."]
-
-    def __init__(self):
-        self.fraction_detected_electrons = jnp.asarray(1.0)
-
-    @override
-    def __call__(
-        self,
-        frequency_grid_maybe_in_angstroms: ImageCoords,
-        *,
-        pixel_size: Optional[RealNumber] = None,
-    ) -> RealNumber:
-        return jnp.asarray(1.0)
-
-
 class IdealDQE(AbstractDQE, strict=True):
     r"""The model for an ideal DQE.
 
     See Ruskin et. al. "Quantitative characterization of electron detectors for
     transmission electron microscopy." (2013) for details.
     """
 
-    fraction_detected_electrons: Shaped[RealNumber, "..."] = field(
+    fraction_detected_electrons: Float[Array, ""] = field(
         default=1.0, converter=error_if_not_fractional
     )
 
     @override
     def __call__(
         self,
-        frequency_grid_maybe_in_angstroms: ImageCoords,
+        frequency_grid_in_angstroms_or_pixels: Float[Array, "y_dim x_dim 2"],
         *,
-        pixel_size: Optional[RealNumber] = None,
-    ) -> RealImage:
+        pixel_size: Optional[Float[Array, ""]] = None,
+    ) -> Float[Array, "y_dim x_dim"]:
         if pixel_size is None:
-            frequency_grid_in_nyquist_units = frequency_grid_maybe_in_angstroms / 0.5
+            frequency_grid_in_nyquist_units = (
+                frequency_grid_in_angstroms_or_pixels / 0.5
+            )
         else:
             frequency_grid_in_nyquist_units = (
-                frequency_grid_maybe_in_angstroms * pixel_size
+                frequency_grid_in_angstroms_or_pixels * pixel_size
             ) / 0.5
         return (
             self.fraction_detected_electrons**2
             * jnp.sinc(frequency_grid_in_nyquist_units[..., 0] / 2) ** 2
             * jnp.sinc(frequency_grid_in_nyquist_units[..., 1] / 2) ** 2
         )
 
@@ -95,94 +81,72 @@
     dqe: AbstractDQE
 
     def __init__(self, dqe: AbstractDQE):
         self.dqe = dqe
 
     @abstractmethod
     def sample(
-        self, key: PRNGKeyArray, expected_electron_events: RealImage
-    ) -> RealImage:
+        self, key: PRNGKeyArray, expected_electron_events: Float[Array, "y_dim x_dim"]
+    ) -> Float[Array, "y_dim x_dim"]:
         """Sample a realization from the detector noise model."""
         raise NotImplementedError
 
     def __call__(
         self,
-        fourier_squared_wavefunction_at_detector_plane: ComplexImage,
-        dose: ElectronDose,
+        fourier_squared_wavefunction_at_detector_plane: Complex[
+            Array, "{config.padded_y_dim} {config.padded_x_dim//2+1}"
+        ],
         config: ImageConfig,
+        electrons_per_angstrom_squared: Float[Array, ""],
         key: Optional[PRNGKeyArray] = None,
-    ) -> ComplexImage:
+    ) -> Complex[Array, "{config.padded_y_dim} {config.padded_x_dim//2+1}"]:
         """Pass the image through the detector model."""
         N_pix = np.prod(config.padded_shape)
-        frequency_grid = config.wrapped_padded_frequency_grid.get()
+        frequency_grid = config.wrapped_padded_frequency_grid_in_pixels.get()
         # Compute the time-integrated electron flux in pixels
-        electrons_per_pixel = dose.electrons_per_angstrom_squared * config.pixel_size**2
+        electrons_per_pixel = electrons_per_angstrom_squared * config.pixel_size**2
         # ... now the total number of electrons over the entire image
         electrons_per_image = N_pix * electrons_per_pixel
         # Normalize the squared wavefunction to a set of probabilities
         fourier_squared_wavefunction_at_detector_plane /= (
             fourier_squared_wavefunction_at_detector_plane[0, 0]
         )
         # Compute the noiseless signal by applying the DQE to the squared wavefunction
         fourier_signal = fourier_squared_wavefunction_at_detector_plane * jnp.sqrt(
             self.dqe(frequency_grid)
         )
-        # Apply the dose
+        # Apply the integrated dose rate
         fourier_expected_electron_events = electrons_per_image * fourier_signal
         if key is None:
             # If there is no key given, return
             return fourier_expected_electron_events
         else:
             # ... otherwise, go to real space, sample, go back to fourier,
             # and return.
             expected_electron_events = irfftn(
                 fourier_expected_electron_events, s=config.padded_shape
             )
             return rfftn(self.sample(key, expected_electron_events))
 
 
-class NullDetector(AbstractDetector):
-    """A null detector model."""
-
-    @override
-    def __init__(self):
-        self.dqe = NullDQE()
-
-    @override
-    def sample(
-        self, key: PRNGKeyArray, expected_electron_events: RealImage
-    ) -> RealImage:
-        return expected_electron_events
-
-    @override
-    def __call__(
-        self,
-        fourier_squared_wavefunction_at_detector_plane: ComplexImage,
-        dose: ElectronDose,
-        config: ImageConfig,
-        key: Optional[PRNGKeyArray] = None,
-    ) -> ComplexImage:
-        return fourier_squared_wavefunction_at_detector_plane
-
-
 class GaussianDetector(AbstractDetector, strict=True):
     """A detector with a gaussian noise model. This is the gaussian limit
     of `PoissonDetector`.
     """
 
     @override
     def sample(
-        self, key: PRNGKeyArray, expected_electron_events: RealImage
-    ) -> RealImage:
+        self, key: PRNGKeyArray, expected_electron_events: Float[Array, "y_dim x_dim"]
+    ) -> Float[Array, "y_dim x_dim"]:
         return expected_electron_events + jnp.sqrt(
             expected_electron_events
         ) * jr.normal(key, expected_electron_events.shape)
 
 
 class PoissonDetector(AbstractDetector, strict=True):
     """A detector with a poisson noise model."""
 
     @override
     def sample(
-        self, key: PRNGKeyArray, expected_electron_events: RealImage
-    ) -> RealImage:
+        self, key: PRNGKeyArray, expected_electron_events: Float[Array, "y_dim x_dim"]
+    ) -> Float[Array, "y_dim x_dim"]:
         return jr.poisson(key, expected_electron_events).astype(float)
```

### Comparing `cryojax-0.2.2rc1/src/cryojax/simulator/_ice.py` & `cryojax-0.2.3rc1/src/cryojax/simulator/_ice.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,62 +5,44 @@
 from abc import abstractmethod
 from typing_extensions import override
 
 import jax.numpy as jnp
 import jax.random as jr
 import numpy as np
 from equinox import Module
-from jaxtyping import PRNGKeyArray
+from jaxtyping import Array, Complex, PRNGKeyArray
 
 from ..image.operators import FourierOperatorLike
-from ..typing import ComplexImage, Image
 from ._config import ImageConfig
 
 
 class AbstractIce(Module, strict=True):
     """Base class for an ice model."""
 
     @abstractmethod
-    def sample(self, key: PRNGKeyArray, config: ImageConfig) -> Image:
-        """Sample a stochastic realization of the potential due to the ice
+    def sample(
+        self, key: PRNGKeyArray, config: ImageConfig
+    ) -> Complex[Array, "{config.padded_y_dim} {config.padded_x_dim//2+1}"]:
+        """Sample a stochastic realization of the phase shifts due to the ice
         at the exit plane."""
         raise NotImplementedError
 
     def __call__(
         self,
         key: PRNGKeyArray,
-        fourier_potential_at_exit_plane: ComplexImage,
+        fourier_phase_at_exit_plane: Complex[
+            Array, "{config.padded_y_dim} {config.padded_x_dim//2+1}"
+        ],
         config: ImageConfig,
-    ) -> ComplexImage:
-        """Compute the combined potential of the ice and the specimen."""
-        # Sample the realization of the potential due to the ice.
-        fourier_ice_potential_at_exit_plane = self.sample(key, config)
+    ) -> Complex[Array, "{config.padded_y_dim} {config.padded_x_dim//2+1}"]:
+        """Compute the combined phase of the ice and the specimen."""
+        # Sample the realization of the phase due to the ice.
+        fourier_ice_phase_at_exit_plane = self.sample(key, config)
 
-        return fourier_potential_at_exit_plane + fourier_ice_potential_at_exit_plane
-
-
-class NullIce(AbstractIce):
-    """A "null" ice model."""
-
-    @override
-    def sample(self, key: PRNGKeyArray, config: ImageConfig) -> Image:
-        return jnp.zeros(
-            config.wrapped_padded_frequency_grid_in_angstroms.get().shape[0:-1]
-        )
-
-    @override
-    def __call__(
-        self,
-        key: PRNGKeyArray,
-        potential_at_exit_plane: ComplexImage,
-        config: ImageConfig,
-    ) -> ComplexImage:
-        return jnp.zeros(
-            config.wrapped_padded_frequency_grid_in_angstroms.get().shape[0:-1]
-        )
+        return fourier_phase_at_exit_plane + fourier_ice_phase_at_exit_plane
 
 
 class GaussianIce(AbstractIce, strict=True):
     r"""Ice modeled as gaussian noise.
 
     **Attributes:**
 
@@ -72,23 +54,25 @@
 
     variance: FourierOperatorLike
 
     def __init__(self, variance: FourierOperatorLike):
         self.variance = variance
 
     @override
-    def sample(self, key: PRNGKeyArray, config: ImageConfig) -> ComplexImage:
-        """Sample a realization of the ice potential as colored gaussian noise."""
+    def sample(
+        self, key: PRNGKeyArray, config: ImageConfig
+    ) -> Complex[Array, "{config.padded_y_dim} {config.padded_x_dim//2+1}"]:
+        """Sample a realization of the ice phase shifts as colored gaussian noise."""
         N_pix = np.prod(config.padded_shape)
         frequency_grid_in_angstroms = (
             config.wrapped_padded_frequency_grid_in_angstroms.get()
         )
         # Compute standard deviation, scaling up by the variance by the number
         # of pixels to make the realization independent pixel-independent in real-space.
         std = jnp.sqrt(N_pix * self.variance(frequency_grid_in_angstroms))
-        ice_potential_at_exit_plane = std * jr.normal(
+        ice_phase_at_exit_plane = std * jr.normal(
             key,
             shape=frequency_grid_in_angstroms.shape[0:-1],
             dtype=complex,
         ).at[0, 0].set(0.0)
 
-        return ice_potential_at_exit_plane
+        return ice_phase_at_exit_plane
```

### Comparing `cryojax-0.2.2rc1/src/cryojax/simulator/_optics.py` & `cryojax-0.2.3rc1/src/cryojax/simulator/_optics.py`

 * *Files 24% similar despite different names*

```diff
@@ -4,85 +4,83 @@
 
 from abc import abstractmethod
 from typing import ClassVar, Optional
 from typing_extensions import override
 
 import jax.numpy as jnp
 from equinox import AbstractClassVar, AbstractVar, field, Module
-from jaxtyping import Shaped
+from jaxtyping import Array, Complex, Float
 
+from ..constants import convert_keV_to_angstroms
 from ..coordinates import cartesian_to_polar
 from ..core import error_if_negative, error_if_not_fractional, error_if_not_positive
 from ..image.operators import (
     AbstractFourierOperator,
     Constant,
     FourierOperatorLike,
 )
-from ..typing import (
-    ComplexImage,
-    Image,
-    ImageCoords,
-    RealImage,
-    RealNumber,
-)
 from ._config import ImageConfig
 
 
 class CTF(AbstractFourierOperator, strict=True):
     """Compute the Contrast Transfer Function (CTF) in for a weakly
     scattering specimen.
     """
 
-    defocus_u_in_angstroms: Shaped[RealNumber, "..."] = field(
+    defocus_u_in_angstroms: Float[Array, ""] = field(
         default=10000.0, converter=error_if_not_positive
     )
-    defocus_v_in_angstroms: Shaped[RealNumber, "..."] = field(
+    defocus_v_in_angstroms: Float[Array, ""] = field(
         default=10000.0, converter=error_if_not_positive
     )
-    astigmatism_angle: Shaped[RealNumber, "..."] = field(
-        default=0.0, converter=jnp.asarray
-    )
-    voltage_in_kilovolts: Shaped[RealNumber, "..."] = field(
-        default=300.0, converter=error_if_not_positive
-    )
-    spherical_aberration_in_mm: Shaped[RealNumber, "..."] = field(
+    astigmatism_angle: Float[Array, ""] = field(default=0.0, converter=jnp.asarray)
+    voltage_in_kilovolts: Float[Array, ""] | float = field(
+        default=300.0, static=True
+    )  # Mark `static=True` so that the voltage is not part of the model pytree
+    # It is treated as part of the pytree upstream, in the Instrument!
+    spherical_aberration_in_mm: Float[Array, ""] = field(
         default=2.7, converter=error_if_negative
     )
-    amplitude_contrast_ratio: Shaped[RealNumber, "..."] = field(
+    amplitude_contrast_ratio: Float[Array, ""] = field(
         default=0.1, converter=error_if_not_fractional
     )
-    phase_shift: Shaped[RealNumber, "..."] = field(default=0.0, converter=jnp.asarray)
-
-    @property
-    def wavelength_in_angstroms(self):
-        voltage_in_volts = 1000.0 * self.voltage_in_kilovolts  # kV to V
-        return 12.2643 / (voltage_in_volts + 0.97845e-6 * voltage_in_volts**2) ** 0.5
+    phase_shift: Float[Array, ""] = field(default=0.0, converter=jnp.asarray)
 
     def __call__(
         self,
-        frequency_grid_in_angstroms: ImageCoords,
+        frequency_grid_in_angstroms: Float[Array, "y_dim x_dim 2"],
         *,
-        defocus_offset: RealNumber | float = 0.0,
-    ) -> RealImage:
+        wavelength_in_angstroms: Optional[Float[Array, ""] | float] = None,
+        defocus_offset: Float[Array, ""] | float = 0.0,
+    ) -> Float[Array, "y_dim x_dim"]:
         # Convert degrees to radians
         phase_shift = jnp.deg2rad(self.phase_shift)
         astigmatism_angle = jnp.deg2rad(self.astigmatism_angle)
         # Convert spherical abberation coefficient to angstroms
         spherical_aberration_in_angstroms = self.spherical_aberration_in_mm * 1e7
+        # Get the wavelength. It can either be passed from upstream or stored in the
+        # CTF
+        if wavelength_in_angstroms is None:
+            wavelength_in_angstroms = convert_keV_to_angstroms(
+                jnp.asarray(self.voltage_in_kilovolts)
+            )
+        else:
+            wavelength_in_angstroms = jnp.asarray(wavelength_in_angstroms)
         # Compute phase shifts for CTF
         phase_shifts = _compute_phase_shifts(
             frequency_grid_in_angstroms,
             self.defocus_u_in_angstroms + jnp.asarray(defocus_offset),
             self.defocus_v_in_angstroms + jnp.asarray(defocus_offset),
             astigmatism_angle,
-            self.wavelength_in_angstroms,
+            wavelength_in_angstroms,
             spherical_aberration_in_angstroms,
             self.amplitude_contrast_ratio,
             phase_shift,
         )
+        # Compute the CTF
         return jnp.sin(phase_shifts).at[0, 0].set(0.0)
 
 
 CTF.__init__.__doc__ = """**Arguments:**
 
 - `defocus_u_in_angstroms`: The major axis defocus in Angstroms.
 - `defocus_v_in_angstroms`: The minor axis defocus in Angstroms.
@@ -99,63 +97,37 @@
 
     ctf: AbstractVar[CTF]
     envelope: AbstractVar[FourierOperatorLike]
 
     is_linear: AbstractClassVar[bool]
 
     @property
-    def wavelength_in_angstroms(self) -> RealNumber:
+    def wavelength_in_angstroms(self) -> Float[Array, ""]:
         return self.ctf.wavelength_in_angstroms
 
     @abstractmethod
     def __call__(
         self,
-        fourier_potential_in_exit_plane: ComplexImage,
+        fourier_phase_in_exit_plane: Complex[
+            Array, "{config.padded_y_dim} {config.padded_x_dim//2+1}"
+        ],
         config: ImageConfig,
-        defocus_offset: RealNumber | float = 0.0,
-    ) -> Image:
+        wavelength_in_angstroms: Float[Array, ""] | float,
+        defocus_offset: Float[Array, ""] | float = 0.0,
+    ) -> (
+        Complex[Array, "{config.padded_y_dim} {config.padded_x_dim//2+1}"]
+        | Complex[Array, "{config.padded_y_dim} {config.padded_x_dim}"]
+    ):
         """Pass an image through the optics model."""
         raise NotImplementedError
 
 
-class NullOptics(AbstractOptics):
-    """A null optics model."""
-
-    ctf: CTF
-    envelope: FourierOperatorLike
-
-    is_linear: ClassVar[bool] = True
-
-    def __init__(self):
-        self.ctf = CTF()
-        self.envelope = Constant(1.0)
-
-    @override
-    def __call__(
-        self,
-        fourier_potential_in_exit_plane: ComplexImage,
-        config: ImageConfig,
-        defocus_offset: RealNumber | float = 0.0,
-    ) -> Image:
-        return fourier_potential_in_exit_plane
-
-
-NullOptics.__init__.__doc__ = """**Arguments:**
-
-- `ctf`: The contrast transfer function model.
-- `envelope`: The envelope function of the optics model.
-- `is_linear`: If `True`, the optics model directly computes
-               the image contrast from the potential. If `False`,
-               the optics model computes the wavefunction.
-"""
-
-
 class WeakPhaseOptics(AbstractOptics, strict=True):
     """An optics model in the weak-phase approximation. Here, compute the image
-    contrast by applying the CTF directly to the scattering potential.
+    contrast by applying the CTF directly to the exit plane phase shifts.
     """
 
     ctf: CTF
     envelope: FourierOperatorLike
 
     is_linear: ClassVar[bool] = True
 
@@ -166,50 +138,53 @@
     ):
         self.ctf = ctf
         self.envelope = envelope or Constant(1.0)
 
     @override
     def __call__(
         self,
-        fourier_potential_in_exit_plane: ComplexImage,
+        fourier_phase_in_exit_plane: Complex[
+            Array, "{config.padded_y_dim} {config.padded_x_dim//2+1}"
+        ],
         config: ImageConfig,
-        defocus_offset: RealNumber | float = 0.0,
-    ) -> ComplexImage:
-        """Apply the CTF directly to the scattering potential."""
+        wavelength_in_angstroms: Float[Array, ""] | float,
+        defocus_offset: Float[Array, ""] | float = 0.0,
+    ) -> Complex[Array, "{config.padded_y_dim} {config.padded_x_dim//2+1}"]:
+        """Apply the CTF directly to the phase shifts in the exit plane."""
         frequency_grid = config.wrapped_padded_frequency_grid_in_angstroms.get()
         # Compute the CTF
         ctf = self.envelope(frequency_grid) * self.ctf(
-            frequency_grid, defocus_offset=defocus_offset
+            frequency_grid,
+            wavelength_in_angstroms=wavelength_in_angstroms,
+            defocus_offset=defocus_offset,
         )
-        # ... compute the contrast as the CTF multiplied by the scattering potential
-        fourier_contrast_in_detector_plane = ctf * fourier_potential_in_exit_plane
+        # ... compute the contrast as the CTF multiplied by the exit plane
+        # phase shifts
+        fourier_contrast_in_detector_plane = ctf * fourier_phase_in_exit_plane
 
         return fourier_contrast_in_detector_plane
 
 
 WeakPhaseOptics.__init__.__doc__ = """**Arguments:**
 
 - `ctf`: The contrast transfer function model.
 - `envelope`: The envelope function of the optics model.
-- `is_linear`: If `True`, the optics model directly computes
-               the image contrast from the potential. If `False`,
-               the optics model computes the wavefunction.
 """
 
 
 def _compute_phase_shifts(
-    frequency_grid_in_angstroms: ImageCoords,
-    defocus_u_in_angstroms: RealNumber,
-    defocus_v_in_angstroms: RealNumber,
-    astigmatism_angle: RealNumber,
-    wavelength_in_angstroms: RealNumber,
-    spherical_aberration_in_angstroms: RealNumber,
-    amplitude_contrast_ratio: RealNumber,
-    phase_shift: RealNumber,
-) -> RealImage:
+    frequency_grid_in_angstroms: Float[Array, "y_dim x_dim 2"],
+    defocus_u_in_angstroms: Float[Array, ""],
+    defocus_v_in_angstroms: Float[Array, ""],
+    astigmatism_angle: Float[Array, ""],
+    wavelength_in_angstroms: Float[Array, ""],
+    spherical_aberration_in_angstroms: Float[Array, ""],
+    amplitude_contrast_ratio: Float[Array, ""],
+    phase_shift: Float[Array, ""],
+) -> Float[Array, "y_dim x_dim"]:
     k_sqr, azimuth = cartesian_to_polar(frequency_grid_in_angstroms, square=True)
     defocus = 0.5 * (
         defocus_u_in_angstroms
         + defocus_v_in_angstroms
         + (defocus_u_in_angstroms - defocus_v_in_angstroms)
         * jnp.cos(2.0 * (azimuth - astigmatism_angle))
     )
```

### Comparing `cryojax-0.2.2rc1/src/cryojax/simulator/_pose.py` & `cryojax-0.2.3rc1/src/cryojax/simulator/_pose.py`

 * *Files 17% similar despite different names*

```diff
@@ -7,24 +7,17 @@
 from typing import overload
 from typing_extensions import override
 
 import equinox as eqx
 import jax
 import jax.numpy as jnp
 from equinox import AbstractVar, field, Module
-from jaxtyping import Array, Float, Shaped
+from jaxtyping import Array, Complex, Float
 
 from ..rotations import SO3
-from ..typing import (
-    ComplexImage,
-    ImageCoords,
-    PointCloudCoords3D,
-    RealNumber,
-    VolumeCoords,
-)
 
 
 class AbstractPose(Module, strict=True):
     """Base class for the image pose.
 
     Subclasses should choose a viewing convention,
     such as with Euler angles or Quaternions. In particular,
@@ -32,50 +25,56 @@
         1. Define angular coordinates as dataclass fields, along
            with other dataclass fields.
 
         2. Overwrite the `AbstractPose.rotation` property and
            `AbstractPose.from_rotation` class method.
     """
 
-    offset_x_in_angstroms: AbstractVar[Shaped[RealNumber, "..."]]
-    offset_y_in_angstroms: AbstractVar[Shaped[RealNumber, "..."]]
-    offset_z_in_angstroms: AbstractVar[Shaped[RealNumber, "..."]]
+    offset_x_in_angstroms: AbstractVar[Float[Array, ""]]
+    offset_y_in_angstroms: AbstractVar[Float[Array, ""]]
+    offset_z_in_angstroms: AbstractVar[Float[Array, ""]]
 
     @overload
     def rotate_coordinates(
-        self, volume_coordinates: VolumeCoords, inverse: bool = False
-    ) -> VolumeCoords: ...
+        self,
+        volume_coordinates: Float[Array, "z_dim y_dim x_dim 3"],
+        inverse: bool = False,
+    ) -> Float[Array, "z_dim y_dim x_dim 3"]: ...
 
     @overload
     def rotate_coordinates(
-        self, volume_coordinates: PointCloudCoords3D, inverse: bool = False
-    ) -> PointCloudCoords3D: ...
+        self, volume_coordinates: Float[Array, "size 3"], inverse: bool = False
+    ) -> Float[Array, "size 3"]: ...
 
     def rotate_coordinates(
         self,
-        volume_coordinates: VolumeCoords | PointCloudCoords3D,
+        volume_coordinates: (
+            Float[Array, "z_dim y_dim x_dim 3"] | Float[Array, "size 3"]
+        ),
         inverse: bool = False,
-    ) -> VolumeCoords | PointCloudCoords3D:
+    ) -> Float[Array, "z_dim y_dim x_dim 3"] | Float[Array, "size 3"]:
         """Rotate coordinates from a particular convention."""
         rotation = self.rotation.inverse() if inverse else self.rotation
-        if isinstance(volume_coordinates, PointCloudCoords3D):  # type: ignore
+        if isinstance(volume_coordinates, Float[Array, "size 3"]):  # type: ignore
             rotated_volume_coordinates = jax.vmap(rotation.apply)(volume_coordinates)
-        elif isinstance(volume_coordinates, VolumeCoords):  # type: ignore
+        elif isinstance(volume_coordinates, Float[Array, "z_dim y_dim x_dim 3"]):  # type: ignore
             rotated_volume_coordinates = jax.vmap(jax.vmap(jax.vmap(rotation.apply)))(
                 volume_coordinates
             )
         else:
             raise ValueError(
                 "Coordinates must be a JAX array either of shape (N, 3) or "
                 f"(N1, N2, N3, 3). Instead, got {volume_coordinates.shape} and type "
                 f"{type(volume_coordinates)}."
             )
         return rotated_volume_coordinates
 
-    def compute_shifts(self, frequency_grid_in_angstroms: ImageCoords) -> ComplexImage:
+    def compute_shifts(
+        self, frequency_grid_in_angstroms: Float[Array, "y_dim x_dim 2"]
+    ) -> Complex[Array, "y_dim x_dim"]:
         """Compute the phase shifts from the in-plane translation,
         given a frequency grid coordinate system.
         """
         xy = self.offset_in_angstroms[0:2]
         return jnp.exp(
             -1.0j * (2 * jnp.pi * jnp.matmul(frequency_grid_in_angstroms, xy))
         )
@@ -132,27 +131,21 @@
 
 class EulerAnglePose(AbstractPose, strict=True):
     r"""An `AbstractPose` represented by Euler angles.
     Angles are given in degrees, and the sequence of rotations is
     given by a zyz extrinsic rotations.
     """
 
-    offset_x_in_angstroms: Shaped[RealNumber, "..."] = field(
-        default=0.0, converter=jnp.asarray
-    )
-    offset_y_in_angstroms: Shaped[RealNumber, "..."] = field(
-        default=0.0, converter=jnp.asarray
-    )
-    offset_z_in_angstroms: Shaped[RealNumber, "..."] = field(
-        default=0.0, converter=jnp.asarray
-    )
-
-    view_phi: Shaped[RealNumber, "..."] = field(default=0.0, converter=jnp.asarray)
-    view_theta: Shaped[RealNumber, "..."] = field(default=0.0, converter=jnp.asarray)
-    view_psi: Shaped[RealNumber, "..."] = field(default=0.0, converter=jnp.asarray)
+    offset_x_in_angstroms: Float[Array, ""] = field(default=0.0, converter=jnp.asarray)
+    offset_y_in_angstroms: Float[Array, ""] = field(default=0.0, converter=jnp.asarray)
+    offset_z_in_angstroms: Float[Array, ""] = field(default=0.0, converter=jnp.asarray)
+
+    view_phi: Float[Array, ""] = field(default=0.0, converter=jnp.asarray)
+    view_theta: Float[Array, ""] = field(default=0.0, converter=jnp.asarray)
+    view_psi: Float[Array, ""] = field(default=0.0, converter=jnp.asarray)
 
     @cached_property
     @override
     def rotation(self) -> SO3:
         """Generate a `SO3` object from a set of Euler angles."""
         phi, theta, psi = self.view_phi, self.view_theta, self.view_psi
         # Convert to radians.
@@ -189,27 +182,19 @@
 - `view_psi`: Angle to rotate about third rotation axis, which is the z axis.
 """
 
 
 class QuaternionPose(AbstractPose, strict=True):
     """An `AbstractPose` represented by unit quaternions."""
 
-    offset_x_in_angstroms: Shaped[RealNumber, "..."] = field(
-        default=0.0, converter=jnp.asarray
-    )
-    offset_y_in_angstroms: Shaped[RealNumber, "..."] = field(
-        default=0.0, converter=jnp.asarray
-    )
-    offset_z_in_angstroms: Shaped[RealNumber, "..."] = field(
-        default=0.0, converter=jnp.asarray
-    )
+    offset_x_in_angstroms: Float[Array, ""] = field(default=0.0, converter=jnp.asarray)
+    offset_y_in_angstroms: Float[Array, ""] = field(default=0.0, converter=jnp.asarray)
+    offset_z_in_angstroms: Float[Array, ""] = field(default=0.0, converter=jnp.asarray)
 
-    wxyz: Float[Array, "... 4"] = field(
-        default=(1.0, 0.0, 0.0, 0.0), converter=jnp.asarray
-    )
+    wxyz: Float[Array, "4"] = field(default=(1.0, 0.0, 0.0, 0.0), converter=jnp.asarray)
 
     @cached_property
     @override
     def rotation(self) -> SO3:
         """Generate rotation from the unit quaternion."""
         # Generate SO3 object from unit quaternion
         R = SO3(wxyz=self.wxyz).normalize()
@@ -239,25 +224,19 @@
     which are skew-symmetric matrices, with the euler vector. The magnitude
     of this vector is the angle, and the unit vector is the axis.
 
     In a `SO3` object, the euler vector is mapped to SO3 group elements using
     the matrix exponential.
     """
 
-    offset_x_in_angstroms: Shaped[RealNumber, "..."] = field(
-        default=0.0, converter=jnp.asarray
-    )
-    offset_y_in_angstroms: Shaped[RealNumber, "..."] = field(
-        default=0.0, converter=jnp.asarray
-    )
-    offset_z_in_angstroms: Shaped[RealNumber, "..."] = field(
-        default=0.0, converter=jnp.asarray
-    )
+    offset_x_in_angstroms: Float[Array, ""] = field(default=0.0, converter=jnp.asarray)
+    offset_y_in_angstroms: Float[Array, ""] = field(default=0.0, converter=jnp.asarray)
+    offset_z_in_angstroms: Float[Array, ""] = field(default=0.0, converter=jnp.asarray)
 
-    euler_vector: Float[Array, "... 3"] = field(
+    euler_vector: Float[Array, "3"] = field(
         default=(0.0, 0.0, 0.0), converter=jnp.asarray
     )
 
     @cached_property
     @override
     def rotation(self) -> SO3:
         """Generate rotation from an euler vector using the exponential map."""
```

### Comparing `cryojax-0.2.2rc1/src/cryojax/simulator/_specimen.py` & `cryojax-0.2.3rc1/src/cryojax/simulator/_specimen.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,20 +5,20 @@
 from abc import abstractmethod
 from functools import cached_property
 from typing import Any, Optional
 from typing_extensions import override
 
 import jax
 from equinox import AbstractVar, Module
-from jaxtyping import PRNGKeyArray
+from jaxtyping import Array, Complex, PRNGKeyArray
 
-from ..typing import ComplexImage
 from ._config import ImageConfig
 from ._conformation import AbstractConformation, DiscreteConformation
 from ._ice import AbstractIce
+from ._instrument import Instrument
 from ._integrators import AbstractPotentialIntegrator
 from ._pose import AbstractPose, EulerAnglePose
 from ._potential import AbstractScatteringPotential
 
 
 class AbstractSpecimen(Module, strict=True):
     """
@@ -44,43 +44,50 @@
         raise NotImplementedError
 
     @cached_property
     def potential_in_lab_frame(self) -> AbstractScatteringPotential:
         """Get the scattering potential in the lab frame."""
         return self.potential_in_com_frame.rotate_to_pose(self.pose)
 
-    def scatter_to_exit_plane(self, config: ImageConfig) -> ComplexImage:
+    def scatter_to_exit_plane(
+        self,
+        instrument: Instrument,
+        config: ImageConfig,
+    ) -> Complex[Array, "{config.padded_y_dim} {config.padded_x_dim//2+1}"]:
         """Scatter the specimen potential to the exit plane."""
         # Get potential in the lab frame
         potential = self.potential_in_lab_frame
         # Compute the scattering potential in fourier space
-        fourier_potential_at_exit_plane = self.integrator(potential, config)
+        fourier_phase_at_exit_plane = self.integrator(
+            potential, instrument.wavelength_in_angstroms, config
+        )
         # Apply translation through phase shifts
-        fourier_potential_at_exit_plane *= self.pose.compute_shifts(
+        fourier_phase_at_exit_plane *= self.pose.compute_shifts(
             config.wrapped_padded_frequency_grid_in_angstroms.get()
         )
 
-        return fourier_potential_at_exit_plane
+        return fourier_phase_at_exit_plane
 
     def scatter_to_exit_plane_with_solvent(
         self,
         key: PRNGKeyArray,
+        instrument: Instrument,
         solvent: AbstractIce,
         config: ImageConfig,
-    ) -> ComplexImage:
+    ) -> Complex[Array, "{config.padded_y_dim} {config.padded_x_dim//2+1}"]:
         """Scatter the specimen potential to the exit plane, including
-        the potential due to the solvent."""
-        # Compute the scattering potential in fourier space
-        fourier_potential_at_exit_plane = self.scatter_to_exit_plane(config)
+        the phase shifts due to the solvent."""
+        # Compute the phase  in fourier space
+        fourier_phase_at_exit_plane = self.scatter_to_exit_plane(instrument, config)
         # Get the potential of the specimen plus the ice
-        fourier_potential_at_exit_plane_with_solvent = solvent(
-            key, fourier_potential_at_exit_plane, config
+        fourier_phase_at_exit_plane_with_solvent = solvent(
+            key, fourier_phase_at_exit_plane, config
         )
 
-        return fourier_potential_at_exit_plane_with_solvent
+        return fourier_phase_at_exit_plane_with_solvent
 
 
 class Specimen(AbstractSpecimen, strict=True):
     """
     Abstraction of a of biological specimen.
 
     **Attributes:**
```

### Comparing `cryojax-0.2.2rc1/src/cryojax/simulator/_assembly/_assembly.py` & `cryojax-0.2.3rc1/src/cryojax/simulator/_assembly/_assembly.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from abc import abstractmethod
 from functools import cached_property
 from typing import Optional
 
 import equinox as eqx
 import jax
 from equinox import AbstractVar
-from jaxtyping import Array, Float, Shaped
+from jaxtyping import Array, Float
 
 from ...rotations import SO3
 from .._conformation import AbstractConformation
 from .._pose import AbstractPose
 from .._specimen import AbstractEnsemble, AbstractSpecimen
 
 
@@ -55,26 +55,26 @@
                     f"{type(self)}.conformation must be type "
                     f" {type(self.subunit.conformation)} if {type(self)}.subunit is "
                     f"type {type(self.subunit)}."
                 )
 
     @cached_property
     @abstractmethod
-    def offsets_in_angstroms(self) -> Float[Array, "n_subunits 3"]:
+    def offsets_in_angstroms(self) -> Float[Array, "{n_subunits} 3"]:
         """The positions of each subunit."""
         raise NotImplementedError
 
     @cached_property
     @abstractmethod
-    def rotations(self) -> Shaped[SO3, " n_subunits"]:
+    def rotations(self) -> SO3:
         """The relative rotations between subunits."""
         raise NotImplementedError
 
     @cached_property
-    def poses(self) -> Shaped[AbstractPose, " n_subunits"]:
+    def poses(self) -> AbstractPose:
         """
         Draw the poses of the subunits in the lab frame, measured
         from the rotation relative to the first subunit.
         """
         # Transform the subunit positions by pose of the helix
         transformed_positions = (
             self.pose.rotate_coordinates(self.offsets_in_angstroms, inverse=False)
```

### Comparing `cryojax-0.2.2rc1/src/cryojax/simulator/_assembly/_helix.py` & `cryojax-0.2.3rc1/src/cryojax/simulator/_assembly/_helix.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,18 +4,17 @@
 
 from functools import cached_property
 from typing import Optional
 
 import jax
 import jax.numpy as jnp
 from equinox import field
-from jaxtyping import Array, Float, Shaped
+from jaxtyping import Array, Float
 
 from ...rotations import SO3
-from ...typing import RealNumber
 from .._conformation import AbstractConformation
 from .._pose import AbstractPose, EulerAnglePose
 from .._specimen import AbstractSpecimen
 from ._assembly import AbstractAssembly
 
 
 class Helix(AbstractAssembly, strict=True):
@@ -26,28 +25,28 @@
     See the ``AbstractAssembly`` base class for more information.
 
     The screw axis is taken to be in the center of the
     image, pointing out-of-plane (i.e. along the z direction).
     """
 
     subunit: AbstractSpecimen
-    rise: Shaped[RealNumber, "..."]
-    twist: Shaped[RealNumber, "..."]
+    rise: Float[Array, ""]
+    twist: Float[Array, ""]
 
     pose: AbstractPose
     conformation: Optional[AbstractConformation]
 
     n_subunits: int = field(static=True)
     n_start: int = field(static=True)
 
     def __init__(
         self,
         subunit: AbstractSpecimen,
-        rise: Shaped[RealNumber, "..."] | float,
-        twist: Shaped[RealNumber, "..."] | float,
+        rise: Float[Array, ""] | float,
+        twist: Float[Array, ""] | float,
         pose: Optional[AbstractPose] = None,
         conformation: Optional[AbstractConformation] = None,
         n_start: int = 1,
         n_subunits: int = 1,
     ):
         """**Arguments:**
         - `subunit`:
@@ -83,26 +82,26 @@
     def __check_init__(self):
         if self.n_subunits % self.n_start != 0:
             raise AttributeError(
                 "The number of subunits must be a multiple of the helical start number."
             )
 
     @cached_property
-    def offsets_in_angstroms(self) -> Float[Array, "n_subunits 3"]:
+    def offsets_in_angstroms(self) -> Float[Array, "{self.n_subunits} 3"]:
         """Get the helical lattice positions in the center of mass frame."""
         return compute_helical_lattice_positions(
             self.rise,
             self.twist,
             n_subunits_per_start=self.n_subunits // self.n_start,
             initial_displacement=self.subunit.pose.offset_in_angstroms,
             n_start=self.n_start,
         )
 
     @cached_property
-    def rotations(self) -> Shaped[SO3, "n_subunits"]:
+    def rotations(self) -> SO3:
         """Get the helical lattice rotations in the center of mass frame.
 
         These are rotations of the initial subunit.
         """
         transformed_rotation_matrices = compute_helical_lattice_rotations(
             self.twist,
             n_subunits_per_start=self.n_subunits // self.n_start,
@@ -113,20 +112,20 @@
         transformed_rotations = jax.vmap(lambda mat: SO3.from_matrix(mat))(
             transformed_rotation_matrices
         )
         return transformed_rotations
 
 
 def compute_helical_lattice_positions(
-    rise: RealNumber,
-    twist: RealNumber,
+    rise: Float[Array, ""],
+    twist: Float[Array, ""],
     n_subunits_per_start: int,
     initial_displacement: Float[Array, "3"],
     n_start: int = 1,
-) -> Float[Array, "n_start*n_subunits_per_start 3"]:
+) -> Float[Array, "{n_start*n_subunits_per_start} 3"]:
     """
     Compute the lattice points of a helix for a given
     rise, twist, radius, and start number.
 
     Arguments
     ---------
     rise : `Real_` or `RealVector`, shape `(n_subunits,)`
@@ -200,19 +199,19 @@
         symmetry_angles, subunit_positions_in_subhelix
     ).reshape((n_start * n_subunits_per_start, 3))
 
     return subunit_positions
 
 
 def compute_helical_lattice_rotations(
-    twist: RealNumber,
+    twist: Float[Array, ""],
     n_subunits_per_start: int,
     initial_rotation: Float[Array, "3 3"] = jnp.eye(3),
     n_start: int = 1,
-) -> Float[Array, "n_start*n_subunits_per_start 3"]:
+) -> Float[Array, "{n_start*n_subunits_per_start} 3 3"]:
     """
     Compute the relative rotations of subunits on a
     helical lattice, parameterized by the
     rise, twist, start number, and an initial rotation.
 
     Arguments
     ---------
```

### Comparing `cryojax-0.2.2rc1/src/cryojax/simulator/_integrators/_fourier_slice_extract.py` & `cryojax-0.2.3rc1/src/cryojax/simulator/_integrators/_fourier_slice_extract.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,22 +2,22 @@
 Using the fourier slice theorem for computing volume projections.
 """
 
 from typing import Any
 
 import jax.numpy as jnp
 from equinox import field
+from jaxtyping import Array, Complex, Float
 
 from ...image import (
     irfftn,
     map_coordinates,
     map_coordinates_with_cubic_spline,
     rfftn,
 )
-from ...typing import ComplexCubicVolume, ComplexImage, VolumeSliceCoords
 from .._config import ImageConfig
 from .._potential import (
     FourierVoxelGridPotential,
     FourierVoxelGridPotentialInterpolator,
 )
 from ._potential_integrator import AbstractPotentialIntegrator
 
@@ -46,20 +46,21 @@
     interpolation_order: int = field(static=True, default=1)
     interpolation_mode: str = field(static=True, default="fill")
     interpolation_cval: complex = field(static=True, default=0.0 + 0.0j)
 
     def __call__(
         self,
         potential: FourierVoxelGridPotential | FourierVoxelGridPotentialInterpolator,
+        wavelength_in_angstroms: Float[Array, ""],
         config: ImageConfig,
-    ) -> ComplexImage:
+    ) -> Complex[Array, "{config.padded_y_dim} {config.padded_x_dim//2+1}"]:
         """Compute a projection of the real-space potential by extracting
         a central slice in fourier space.
         """
-        frequency_slice = potential.wrapped_frequency_slice.get()
+        frequency_slice = potential.wrapped_frequency_slice_in_pixels.get()
         N = frequency_slice.shape[1]
         if potential.shape != (N, N, N):
             raise AttributeError(
                 "Only cubic boxes are supported for fourier slice extraction."
             )
         # Compute the fourier projection
         if isinstance(potential, FourierVoxelGridPotentialInterpolator):
@@ -91,19 +92,19 @@
         # Rescale the voxel size to the ImageConfig.pixel_size
         return config.rescale_to_pixel_size(
             fourier_projection, potential.voxel_size, is_real=False
         )
 
 
 def extract_slice(
-    fourier_voxel_grid: ComplexCubicVolume,
-    frequency_slice: VolumeSliceCoords,
+    fourier_voxel_grid: Complex[Array, "dim dim dim"],
+    frequency_slice: Float[Array, "1 dim dim 3"],
     interpolation_order: int = 1,
     **kwargs: Any,
-) -> ComplexImage:
+) -> Complex[Array, "dim dim//2+1"]:
     """
     Project and interpolate 3D volume point cloud
     onto imaging plane using the fourier slice theorem.
 
     Arguments
     ---------
     fourier_voxel_grid : shape `(N, N, N)`
@@ -136,18 +137,18 @@
     # Set last line of frequencies to zero if image dimension is even
     if N % 2 == 0:
         projection = projection.at[:, -1].set(0.0 + 0.0j).at[N // 2, :].set(0.0 + 0.0j)
     return projection
 
 
 def extract_slice_with_cubic_spline(
-    spline_coefficients: ComplexCubicVolume,
-    frequency_slice: VolumeSliceCoords,
+    spline_coefficients: Complex[Array, "dim+2 dim+2 dim+2"],
+    frequency_slice: Float[Array, "1 dim dim 3"],
     **kwargs: Any,
-) -> ComplexImage:
+) -> Complex[Array, "dim dim//2+1"]:
     """
     Project and interpolate 3D volume point cloud
     onto imaging plane using the fourier slice theorem, using cubic
     spline coefficients as input.
 
     Arguments
     ---------
```

### Comparing `cryojax-0.2.2rc1/src/cryojax/simulator/_integrators/_gaussian_mixture.py` & `cryojax-0.2.3rc1/src/cryojax/simulator/_integrators/_gaussian_mixture.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,14 @@
 """
 Scattering methods for the gaussian mixtures of atoms.
 """
 
+'''
 import jax.numpy as jnp
 
-from ...typing import (
-    ComplexImage,
-    ImageCoords,
-    PointCloudCoords2D,
-    RealNumber,
-)
 from .._potential._atom_potential import AtomCloud
 from ._potential_integrator import AbstractPotentialIntegrator
 
 
 class IndependentAtomScattering(AbstractPotentialIntegrator):
     """
     Projects a pointcloud of atoms onto the imaging plane.
@@ -114,7 +109,8 @@
         tuple: two arrays containing the x, y coordinates of each pixel, respectively.
     """
     grid_1d = jnp.linspace(
         -npixels_per_side / 2, npixels_per_side / 2, npixels_per_side + 1
     )[:-1]
     grid_1d *= pixel_size
     return jnp.expand_dims(grid_1d, axis=(0, -1))
+'''
```

### Comparing `cryojax-0.2.2rc1/src/cryojax/simulator/_integrators/_nufft_project.py` & `cryojax-0.2.3rc1/src/cryojax/simulator/_integrators/_nufft_project.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,17 @@
 """
 Using non-uniform FFTs for computing volume projections.
 """
 
 import math
-from typing import Union
 
 import jax.numpy as jnp
 from equinox import field
+from jaxtyping import Array, Complex, Float
 
-from ...typing import (
-    ComplexImage,
-    PointCloudCoords2D,
-    PointCloudCoords3D,
-    RealPointCloud,
-)
 from .._config import ImageConfig
 from .._potential import RealVoxelCloudPotential, RealVoxelGridPotential
 from ._potential_integrator import AbstractPotentialIntegrator
 
 
 class NufftProject(AbstractPotentialIntegrator, strict=True):
     """Integrate points onto the exit plane using
@@ -30,48 +24,51 @@
     """
 
     eps: float = field(static=True, default=1e-6)
 
     def __call__(
         self,
         potential: RealVoxelGridPotential | RealVoxelCloudPotential,
+        wavelength_in_angstroms: Float[Array, ""],
         config: ImageConfig,
-    ) -> ComplexImage:
+    ) -> Complex[Array, "{config.padded_y_dim} {config.padded_x_dim//2+1}"]:
         """Rasterize image with non-uniform FFTs."""
         if isinstance(potential, RealVoxelGridPotential):
             shape = potential.shape
             fourier_projection = project_with_nufft(
                 potential.real_voxel_grid.ravel(),
-                potential.wrapped_coordinate_grid.get().reshape((math.prod(shape), 3)),
+                potential.wrapped_coordinate_grid_in_pixels.get().reshape(
+                    (math.prod(shape), 3)
+                ),
                 config.padded_shape,
                 eps=self.eps,
             )
         elif isinstance(potential, RealVoxelCloudPotential):
             fourier_projection = project_with_nufft(
                 potential.voxel_weights,
-                potential.wrapped_coordinate_list.get(),
+                potential.wrapped_coordinate_list_in_pixels.get(),
                 config.padded_shape,
                 eps=self.eps,
             )
         else:
             raise ValueError(
                 "Supported density representations are RealVoxelGrid and VoxelCloud."
             )
         # Rescale the voxel size to the ImageConfig.pixel_size
         return config.rescale_to_pixel_size(
             fourier_projection, potential.voxel_size, is_real=False
         )
 
 
 def project_with_nufft(
-    weights: RealPointCloud,
-    coordinate_list: Union[PointCloudCoords2D, PointCloudCoords3D],
+    weights: Float[Array, " size"],
+    coordinate_list: Float[Array, "size 2"] | Float[Array, "size 3"],
     shape: tuple[int, int],
     eps: float = 1e-6,
-) -> ComplexImage:
+) -> Complex[Array, "{shape[0]} {shape[1]}"]:
     """
     Project and interpolate 3D volume point cloud
     onto imaging plane using a non-uniform FFT.
 
     Arguments
     ---------
     weights : shape `(N,)`
```

### Comparing `cryojax-0.2.2rc1/src/cryojax/simulator/_integrators/_potential_integrator.py` & `cryojax-0.2.3rc1/src/cryojax/simulator/_integrators/_potential_integrator.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,36 +2,39 @@
 Methods for integrating the scattering potential onto the exit plane.
 """
 
 from abc import abstractmethod
 from typing import Generic, TypeVar
 
 from equinox import Module
+from jaxtyping import Array, Complex, Float
 
-from ...typing import ComplexImage
 from .._config import ImageConfig
 from .._potential import AbstractScatteringPotential
 
 
 ScatteringPotentialT = TypeVar(
     "ScatteringPotentialT", bound="AbstractScatteringPotential"
 )
 
 
 class AbstractPotentialIntegrator(Module, Generic[ScatteringPotentialT], strict=True):
     """Base class for a method of integrating the scattering
-    potential onto the exit plane."""
+    potential to a set of phase shifts the exit plane."""
 
     @abstractmethod
     def __call__(
-        self, potential: ScatteringPotentialT, config: ImageConfig
-    ) -> ComplexImage:
+        self,
+        potential: ScatteringPotentialT,
+        wavelength_in_angstroms: Float[Array, ""],
+        config: ImageConfig,
+    ) -> Complex[Array, "{config.padded_y_dim} {config.padded_x_dim//2+1}"]:
         """Compute the scattering potential in the exit plane at
         the `ImageConfig` settings.
 
         **Arguments:**
 
         - `potential`: The scattering potential representation.
-
+        - `wavelength_in_angstroms`: The wavelength of the electron beam.
         - `config`: The configuration of the resulting image.
         """
         raise NotImplementedError
```

### Comparing `cryojax-0.2.2rc1/src/cryojax/simulator/_potential/__init__.py` & `cryojax-0.2.3rc1/src/cryojax/simulator/_potential/__init__.py`

 * *Files identical despite different names*

### Comparing `cryojax-0.2.2rc1/src/cryojax/simulator/_potential/_atom_potential.py` & `cryojax-0.2.3rc1/src/cryojax/simulator/_potential/_atom_potential.py`

 * *Files identical despite different names*

### Comparing `cryojax-0.2.2rc1/src/cryojax/simulator/_potential/_scattering_potential.py` & `cryojax-0.2.3rc1/src/cryojax/simulator/_potential/_scattering_potential.py`

 * *Files identical despite different names*

### Comparing `cryojax-0.2.2rc1/src/cryojax/simulator/_potential/_voxel_potential.py` & `cryojax-0.2.3rc1/src/cryojax/simulator/_potential/_voxel_potential.py`

 * *Files 15% similar despite different names*

```diff
@@ -6,116 +6,114 @@
 from functools import cached_property
 from typing import (
     Any,
     cast,
     ClassVar,
     Optional,
     overload,
-    Type,
 )
 from typing_extensions import override, Self
 
 import equinox as eqx
 import jax
 import jax.numpy as jnp
 import numpy as np
 from equinox import AbstractClassVar, AbstractVar, field
-from jaxtyping import Array, Float, Int, Shaped
+from jaxtyping import Array, Complex, Float, Int
 
 from ...constants import get_form_factor_params
 from ...coordinates import CoordinateGrid, CoordinateList, FrequencySlice
 from ...core import error_if_not_positive
 from ...image import (
     compute_spline_coefficients,
     crop_to_shape,
     fftn,
     pad_to_shape,
 )
 from ...image.operators import AbstractFilter
-from ...typing import (
-    ComplexCubicVolume,
-    RealCubicVolume,
-    RealNumber,
-    RealPointCloud,
-)
 from .._pose import AbstractPose
 from ._scattering_potential import AbstractScatteringPotential
 
 
 class AbstractVoxelPotential(AbstractScatteringPotential, strict=True):
     """Abstract interface for a voxel-based scattering potential representation."""
 
-    voxel_size: AbstractVar[Shaped[RealNumber, "..."]]
+    voxel_size: AbstractVar[Float[Array, ""]]
     is_real: AbstractClassVar[bool]
 
     @property
     @abstractmethod
     def shape(self) -> tuple[int, ...]:
         """The shape of the voxel array."""
         raise NotImplementedError
 
     @classmethod
     @abstractmethod
     def from_real_voxel_grid(
-        cls: Type[Self],
-        real_voxel_grid: Float[Array, "N N N"] | Float[np.ndarray, "N N N"],
+        cls,
+        real_voxel_grid: Float[Array, "dim dim dim"] | Float[np.ndarray, "dim dim dim"],
         voxel_size: Float[Array, ""] | Float[np.ndarray, ""] | float,
     ) -> Self:
         """Load an `AbstractVoxels` from real-valued 3D electron
         scattering potential.
         """
         raise NotImplementedError
 
     @classmethod
     @abstractmethod
     def from_atoms(
-        cls: Type[Self],
-        atom_positions: Float[Array, "N 3"],
-        atom_identities: Int[Array, " N"],
+        cls,
+        atom_positions: Float[Array, "n_atoms 3"] | Float[np.ndarray, "n_atoms 3"],
+        atom_identities: Int[Array, " n_atoms"] | Int[np.ndarray, " n_atoms"],
         voxel_size: Float[Array, ""] | Float[np.ndarray, ""] | float,
         coordinate_grid_in_angstroms: CoordinateGrid,
-        form_factors: Optional[Float[Array, "N 5"]] = None,
+        form_factors: Optional[
+            Float[Array, "n_atoms n_form_factors"]
+            | Float[np.ndarray, "n_atoms n_form_factors"]
+        ] = None,
         **kwargs: Any,
     ) -> Self:
         """Load an `AbstractVoxels` from atom positions and identities."""
         raise NotImplementedError
 
 
 class AbstractFourierVoxelGridPotential(AbstractVoxelPotential, strict=True):
     """Abstract interface of a 3D scattering potential voxel grid
     in fourier-space.
     """
 
-    wrapped_frequency_slice: AbstractVar[FrequencySlice]
+    wrapped_frequency_slice_in_pixels: AbstractVar[FrequencySlice]
 
     @abstractmethod
     def __init__(
         self,
-        fourier_voxel_grid: Shaped[ComplexCubicVolume, "..."],
-        wrapped_frequency_slice: FrequencySlice,
-        voxel_size: Shaped[RealNumber, "..."] | float,
+        fourier_voxel_grid: Complex[Array, "dim dim dim"],
+        wrapped_frequency_slice_in_pixels: FrequencySlice,
+        voxel_size: Float[Array, ""] | float,
     ):
         raise NotImplementedError
 
     @cached_property
     def wrapped_frequency_slice_in_angstroms(self) -> FrequencySlice:
         """The `wrapped_frequency_slice` in angstroms."""
-        return self.wrapped_frequency_slice / self.voxel_size
+        return self.wrapped_frequency_slice_in_pixels / self.voxel_size
 
     def rotate_to_pose(self, pose: AbstractPose) -> Self:
         return eqx.tree_at(
-            lambda d: d.wrapped_frequency_slice.array,
+            lambda d: d.wrapped_frequency_slice_in_pixels.array,
             self,
-            pose.rotate_coordinates(self.wrapped_frequency_slice.get(), inverse=True),
+            pose.rotate_coordinates(
+                self.wrapped_frequency_slice_in_pixels.get(), inverse=True
+            ),
         )
 
     @classmethod
     def from_real_voxel_grid(
-        cls: Type[Self],
-        real_voxel_grid: Float[Array, "N N N"] | Float[np.ndarray, "N N N"],
+        cls,
+        real_voxel_grid: Float[Array, "dim dim dim"] | Float[np.ndarray, "dim dim dim"],
         voxel_size: Float[Array, ""] | Float[np.ndarray, ""] | float,
         *,
         pad_scale: float = 1.0,
         pad_mode: str = "constant",
         filter: Optional[AbstractFilter] = None,
     ) -> Self:
         """Load an `AbstractFourierVoxelGridPotential` from real-valued 3D electron
@@ -164,90 +162,101 @@
             cast(tuple[int, int], padded_real_voxel_grid.shape[:-1]), half_space=False
         )
 
         return cls(fourier_voxel_grid, frequency_slice, voxel_size)
 
     @classmethod
     def from_atoms(
-        cls: Type[Self],
-        atom_positions: Float[Array, "N 3"],
-        atom_identities: Int[Array, " N"],
+        cls,
+        atom_positions: Float[Array, "n_atoms 3"] | Float[np.ndarray, "n_atoms 3"],
+        atom_identities: Int[Array, " n_atoms"] | Int[np.ndarray, " n_atoms"],
         voxel_size: Float[Array, ""] | Float[np.ndarray, ""] | float,
         coordinate_grid_in_angstroms: CoordinateGrid,
-        form_factors: Optional[Float[Array, "N 5"]] = None,
+        form_factors: Optional[
+            Float[Array, "n_atoms n_form_factors"]
+            | Float[np.ndarray, "n_atoms n_form_factors"]
+        ] = None,
         **kwargs: Any,
     ) -> Self:
         """Load an `AbstractFourierVoxelGridPotential` from atom positions and
         identities.
 
         **Arguments:**
 
         - `**kwargs`: Passed to `AbstractFourierVoxelGridPotential.from_real_voxel_grid`
         """
-        a_vals, b_vals = get_form_factor_params(atom_identities, form_factors)
+        form_factors = (
+            form_factors if form_factors is None else jnp.asarray(form_factors)
+        )
+        a_vals, b_vals = get_form_factor_params(
+            jnp.asarray(atom_identities), form_factors
+        )
 
         potential = build_real_space_voxels_from_atoms(
-            atom_positions, a_vals, b_vals, coordinate_grid_in_angstroms.get()
+            jnp.asarray(atom_positions),
+            a_vals,
+            b_vals,
+            coordinate_grid_in_angstroms.get(),
         )
 
         return cls.from_real_voxel_grid(
             potential,
             voxel_size,
             **kwargs,
         )
 
 
 class FourierVoxelGridPotential(AbstractFourierVoxelGridPotential):
     """A 3D scattering potential voxel grid in fourier-space."""
 
-    fourier_voxel_grid: Shaped[ComplexCubicVolume, "..."]
-    wrapped_frequency_slice: FrequencySlice
-    voxel_size: Shaped[RealNumber, "..."] = field(converter=error_if_not_positive)
+    fourier_voxel_grid: Complex[Array, "dim dim dim"]
+    wrapped_frequency_slice_in_pixels: FrequencySlice
+    voxel_size: Float[Array, ""] = field(converter=error_if_not_positive)
 
     is_real: ClassVar[bool] = False
 
     @override
     def __init__(
         self,
-        fourier_voxel_grid: Shaped[ComplexCubicVolume, "..."],
-        wrapped_frequency_slice: FrequencySlice,
-        voxel_size: Shaped[RealNumber, "..."] | float,
+        fourier_voxel_grid: Complex[Array, "dim dim dim"],
+        wrapped_frequency_slice_in_pixels: FrequencySlice,
+        voxel_size: Float[Array, ""] | float,
     ):
         """**Arguments:**
 
         - `fourier_voxel_grid`: The cubic voxel grid in fourier space.
-        - `wrapped_frequency_slice`: Frequency slice coordinate system,
-                                     wrapped in a `FrequencySlice` object.
+        - `wrapped_frequency_slice_in_pixels`: Frequency slice coordinate system,
+                                               wrapped in a `FrequencySlice` object.
         - `voxel_size`: The voxel size.
         """
         self.fourier_voxel_grid = jnp.asarray(fourier_voxel_grid)
-        self.wrapped_frequency_slice = wrapped_frequency_slice
+        self.wrapped_frequency_slice_in_pixels = wrapped_frequency_slice_in_pixels
         self.voxel_size = jnp.asarray(voxel_size)
 
     @property
     def shape(self) -> tuple[int, int, int]:
         return cast(tuple[int, int, int], self.fourier_voxel_grid.shape)
 
 
 class FourierVoxelGridPotentialInterpolator(AbstractFourierVoxelGridPotential):
     """A 3D scattering potential voxel grid in fourier-space, represented
     by spline coefficients.
     """
 
-    coefficients: Shaped[ComplexCubicVolume, "..."]
-    wrapped_frequency_slice: FrequencySlice
-    voxel_size: Shaped[RealNumber, "..."] = field(converter=error_if_not_positive)
+    coefficients: Float[Array, "coeff_dim coeff_dim coeff_dim"]
+    wrapped_frequency_slice_in_pixels: FrequencySlice
+    voxel_size: Float[Array, ""] = field(converter=error_if_not_positive)
 
     is_real: ClassVar[bool] = False
 
     def __init__(
         self,
-        fourier_voxel_grid: Shaped[ComplexCubicVolume, "..."],
-        wrapped_frequency_slice: FrequencySlice,
-        voxel_size: Shaped[RealNumber, "..."] | float,
+        fourier_voxel_grid: Float[Array, "dim dim dim"],
+        wrapped_frequency_slice_in_pixels: FrequencySlice,
+        voxel_size: Float[Array, ""] | float,
     ):
         """
         !!! note
             The argument `fourier_voxel_grid` is used to set
             `FourierVoxelGridPotentialInterpolator.coefficients` in the `__init__`,
             but it is not stored in the class. For example,
 
@@ -258,104 +267,100 @@
             assert hasattr(voxels, "fourier_voxel_grid")  # This will return an error
             assert hasattr(voxels, "coefficients")  # Instead, store spline coefficients
             ```
 
         **Arguments:**
 
         - `fourier_voxel_grid`: The cubic voxel grid in fourier space.
-        - `wrapped_frequency_slice`: Frequency slice coordinate system,
-                                     wrapped in a `FrequencySlice` object.
+        - `wrapped_frequency_slice_in_pixels`: Frequency slice coordinate system,
+                                               wrapped in a `FrequencySlice` object.
         - `voxel_size`: The voxel size.
         """
-        n_batch_dims = fourier_voxel_grid.ndim - 3
-        compute_spline_coefficients_3d = compute_spline_coefficients
-        for _ in range(n_batch_dims):
-            compute_spline_coefficients_3d = jax.vmap(compute_spline_coefficients_3d)
-        self.coefficients = compute_spline_coefficients_3d(
-            jnp.asarray(fourier_voxel_grid)
-        )
-        self.wrapped_frequency_slice = wrapped_frequency_slice
+        self.coefficients = compute_spline_coefficients(jnp.asarray(fourier_voxel_grid))
+        self.wrapped_frequency_slice_in_pixels = wrapped_frequency_slice_in_pixels
         self.voxel_size = jnp.asarray(voxel_size)
 
     @property
     def shape(self) -> tuple[int, int, int]:
         return cast(
             tuple[int, int, int], tuple([s - 2 for s in self.coefficients.shape])
         )
 
 
 class RealVoxelGridPotential(AbstractVoxelPotential, strict=True):
     """Abstraction of a 3D scattering potential voxel grid in real-space."""
 
-    real_voxel_grid: Shaped[RealCubicVolume, "..."]
-    wrapped_coordinate_grid: CoordinateGrid
-    voxel_size: Shaped[RealNumber, "..."] = field(converter=error_if_not_positive)
+    real_voxel_grid: Float[Array, "dim dim dim"]
+    wrapped_coordinate_grid_in_pixels: CoordinateGrid
+    voxel_size: Float[Array, ""] = field(converter=error_if_not_positive)
 
     is_real: ClassVar[bool] = True
 
     def __init__(
         self,
-        real_voxel_grid: Shaped[RealCubicVolume, "..."],
-        wrapped_coordinate_grid: CoordinateGrid,
-        voxel_size: Shaped[RealNumber, "..."] | float,
+        real_voxel_grid: Float[Array, "dim dim dim"],
+        wrapped_coordinate_grid_in_pixels: CoordinateGrid,
+        voxel_size: Float[Array, ""] | float,
     ):
         """**Arguments:**
 
         - `real_voxel_grid`: The voxel grid in fourier space.
-        - `wrapped_coordinate_grid`: A coordinate grid, wrapped into a
-                                     `CoordinateGrid` object.
+        - `wrapped_coordinate_grid_in_pixels`: A coordinate grid, wrapped into a
+                                               `CoordinateGrid` object.
         - `voxel_size`: The voxel size.
         """
         self.real_voxel_grid = jnp.asarray(real_voxel_grid)
-        self.wrapped_coordinate_grid = wrapped_coordinate_grid
+        self.wrapped_coordinate_grid_in_pixels = wrapped_coordinate_grid_in_pixels
         self.voxel_size = jnp.asarray(voxel_size)
 
     @property
     def shape(self) -> tuple[int, int, int]:
         return cast(tuple[int, int, int], self.real_voxel_grid.shape)
 
     @cached_property
     def wrapped_coordinate_grid_in_angstroms(self) -> CoordinateGrid:
         """The `coordinate_grid` in angstroms."""
-        return self.voxel_size * self.wrapped_coordinate_grid  # type: ignore
+        return self.voxel_size * self.wrapped_coordinate_grid_in_pixels  # type: ignore
 
     def rotate_to_pose(self, pose: AbstractPose) -> Self:
         return eqx.tree_at(
-            lambda d: d.wrapped_coordinate_grid.array,
+            lambda d: d.wrapped_coordinate_grid_in_pixels.array,
             self,
-            pose.rotate_coordinates(self.wrapped_coordinate_grid.get(), inverse=False),
+            pose.rotate_coordinates(
+                self.wrapped_coordinate_grid_in_pixels.get(), inverse=False
+            ),
         )
 
     @overload
     @classmethod
     def from_real_voxel_grid(
-        cls: Type[Self],
-        real_voxel_grid: Float[Array, "N N N"] | Float[np.ndarray, "N N N"],
+        cls,
+        real_voxel_grid: Float[Array, "dim dim dim"] | Float[np.ndarray, "dim dim dim"],
         voxel_size: Float[Array, ""] | Float[np.ndarray, ""] | float,
         *,
         coordinate_grid: Optional[CoordinateGrid] = None,
     ) -> Self: ...
 
     @overload
     @classmethod
     def from_real_voxel_grid(
-        cls: Type[Self],
-        real_voxel_grid: Float[Array, "N N N"] | Float[np.ndarray, "N N N"],
+        cls,
+        real_voxel_grid: Float[Array, "dim dim dim"] | Float[np.ndarray, "dim dim dim"],
         voxel_size: Float[Array, ""] | Float[np.ndarray, ""] | float,
         *,
         crop_scale: Optional[float] = None,
     ) -> Self: ...
 
     @classmethod
     def from_real_voxel_grid(
-        cls: Type[Self],
-        real_voxel_grid: Float[Array, "N N N"] | Float[np.ndarray, "N N N"],
+        cls,
+        real_voxel_grid: Float[Array, "dim dim dim"] | Float[np.ndarray, "dim dim dim"],
         voxel_size: Float[Array, ""] | Float[np.ndarray, ""] | float,
         *,
-        coordinate_grid: Optional[CoordinateGrid] = None,
+        coordinate_grid_in_pixels: Optional[CoordinateGrid] = None,
         crop_scale: Optional[float] = None,
     ) -> Self:
         """Load a `RealVoxelGridPotential` from a real-valued 3D electron
         scattering potential voxel grid.
 
         **Arguments:**
 
@@ -366,54 +371,65 @@
         """
         # Cast to jax array
         real_voxel_grid, voxel_size = (
             jnp.asarray(real_voxel_grid),
             jnp.asarray(voxel_size),
         )
         # Make coordinates if not given
-        if coordinate_grid is None:
+        if coordinate_grid_in_pixels is None:
             # Option for cropping template
             if crop_scale is not None:
                 if crop_scale > 1.0:
                     raise ValueError("crop_scale must be less than 1.0")
                 cropped_shape = cast(
                     tuple[int, int, int],
                     tuple([int(s * crop_scale) for s in real_voxel_grid.shape[-3:]]),
                 )
                 real_voxel_grid = crop_to_shape(real_voxel_grid, cropped_shape)
-            coordinate_grid = CoordinateGrid(real_voxel_grid.shape[-3:])
+            coordinate_grid_in_pixels = CoordinateGrid(real_voxel_grid.shape[-3:])
 
-        return cls(real_voxel_grid, coordinate_grid, voxel_size)
+        return cls(real_voxel_grid, coordinate_grid_in_pixels, voxel_size)
 
     @classmethod
     def from_atoms(
-        cls: Type[Self],
-        atom_positions: Float[Array, "N 3"],
-        atom_identities: Int[Array, " N"],
+        cls,
+        atom_positions: Float[Array, "n_atoms 3"] | Float[np.ndarray, "n_atoms 3"],
+        atom_identities: Int[Array, " n_atoms"] | Int[np.ndarray, " n_atoms"],
         voxel_size: Float[Array, ""] | Float[np.ndarray, ""] | float,
         coordinate_grid_in_angstroms: CoordinateGrid,
-        form_factors: Optional[Float[Array, "N 5"]] = None,
+        form_factors: Optional[
+            Float[Array, "n_atoms n_form_factors"]
+            | Float[np.ndarray, "n_atoms n_form_factors"]
+        ] = None,
         **kwargs: Any,
     ) -> Self:
         """Load a `RealVoxelGridPotential` from atom positions and identities.
 
         **Arguments:**
 
         - `**kwargs`: Passed to `RealVoxelGridPotential.from_real_voxel_grid`
         """
-        a_vals, b_vals = get_form_factor_params(atom_identities, form_factors)
+        form_factors = (
+            form_factors if form_factors is None else jnp.asarray(form_factors)
+        )
+        a_vals, b_vals = get_form_factor_params(
+            jnp.asarray(atom_identities), form_factors
+        )
 
         real_voxel_grid = build_real_space_voxels_from_atoms(
-            atom_positions, a_vals, b_vals, coordinate_grid_in_angstroms.get()
+            jnp.asarray(atom_positions),
+            a_vals,
+            b_vals,
+            coordinate_grid_in_angstroms.get(),
         )
 
         return cls.from_real_voxel_grid(
             real_voxel_grid,
             voxel_size,
-            coordinate_grid=coordinate_grid_in_angstroms / voxel_size,
+            coordinate_grid_in_pixels=coordinate_grid_in_angstroms / voxel_size,
             **kwargs,
         )
 
 
 class RealVoxelCloudPotential(AbstractVoxelPotential, strict=True):
     """Abstraction of a 3D electron scattering potential voxel point cloud.
 
@@ -421,60 +437,62 @@
         This object is similar to the `RealVoxelGridPotential`. Instead
         of storing the whole voxel grid, a `RealVoxelCloudPotential` need
         only store points of non-zero scattering potential. Therefore,
         a `RealVoxelCloudPotential` stores a point cloud of scattering potential
         voxel values.
     """
 
-    voxel_weights: Shaped[RealPointCloud, "..."]
-    wrapped_coordinate_list: CoordinateList
-    voxel_size: Shaped[RealNumber, "..."] = field(converter=error_if_not_positive)
+    voxel_weights: Float[Array, " size"]
+    wrapped_coordinate_list_in_pixels: CoordinateList
+    voxel_size: Float[Array, ""] = field(converter=error_if_not_positive)
 
     is_real: ClassVar[bool] = True
 
     def __init__(
         self,
-        voxel_weights: Shaped[RealPointCloud, "..."],
-        wrapped_coordinate_list: CoordinateList,
-        voxel_size: Shaped[RealNumber, "..."] | float,
+        voxel_weights: Float[Array, " size"],
+        wrapped_coordinate_list_in_pixels: CoordinateList,
+        voxel_size: Float[Array, ""] | float,
     ):
         """**Arguments:**
 
         - `voxel_weights`: A point-cloud of voxel scattering potential values.
-        - `wrapped_coordinate_list`: Coordinate list for the `voxel_weights`, wrapped
-                                     in a `CoordinateList` object.
+        - `wrapped_coordinate_list_in_pixels`: Coordinate list for the `voxel_weights`,
+                                               wrapped in a `CoordinateList` object.
         - `voxel_size`: The voxel size.
         """
         self.voxel_weights = jnp.asarray(voxel_weights)
-        self.wrapped_coordinate_list = wrapped_coordinate_list
+        self.wrapped_coordinate_list_in_pixels = wrapped_coordinate_list_in_pixels
         self.voxel_size = jnp.asarray(voxel_size)
 
     @property
     def shape(self) -> tuple[int, int]:
         return cast(tuple[int, int], self.voxel_weights.shape)
 
     @cached_property
-    def coordinate_list_in_angstroms(self) -> CoordinateList:
+    def wrapped_coordinate_list_in_angstroms(self) -> CoordinateList:
         """The `coordinate_list` in angstroms."""
-        return self.voxel_size * self.wrapped_coordinate_list  # type: ignore
+        return self.voxel_size * self.wrapped_coordinate_list_in_pixels  # type: ignore
 
     def rotate_to_pose(self, pose: AbstractPose) -> Self:
         return eqx.tree_at(
-            lambda d: d.wrapped_coordinate_list.array,
+            lambda d: d.wrapped_coordinate_list_in_pixels.array,
             self,
-            pose.rotate_coordinates(self.wrapped_coordinate_list.get(), inverse=False),
+            pose.rotate_coordinates(
+                self.wrapped_coordinate_list_in_pixels.get(), inverse=False
+            ),
         )
 
     @classmethod
     def from_real_voxel_grid(
-        cls: Type[Self],
-        real_voxel_grid: Float[Array, "N N N"] | Float[np.ndarray, "N N N"],
+        cls,
+        real_voxel_grid: Float[Array, "dim dim dim"] | Float[np.ndarray, "dim dim dim"],
         voxel_size: Float[Array, ""] | Float[np.ndarray, ""] | float,
         *,
-        coordinate_grid: Optional[CoordinateGrid] = None,
+        coordinate_grid_in_pixels: Optional[CoordinateGrid] = None,
         rtol: float = 1e-05,
         atol: float = 1e-08,
     ) -> Self:
         """Load an `RealVoxelCloudPotential` from a real-valued 3D electron
         scattering potential voxel grid.
 
         **Arguments:**
@@ -488,60 +506,71 @@
         """
         # Cast to jax array
         real_voxel_grid, voxel_size = (
             jnp.asarray(real_voxel_grid),
             jnp.asarray(voxel_size),
         )
         # Make coordinates if not given
-        if coordinate_grid is None:
-            coordinate_grid = CoordinateGrid(real_voxel_grid.shape)
+        if coordinate_grid_in_pixels is None:
+            coordinate_grid_in_pixels = CoordinateGrid(real_voxel_grid.shape)
         # ... mask zeros to store smaller arrays. This
         # option is not jittable.
         nonzero = jnp.where(~jnp.isclose(real_voxel_grid, 0.0, rtol=rtol, atol=atol))
         flat_potential = real_voxel_grid[nonzero]
-        coordinate_list = CoordinateList(coordinate_grid.get()[nonzero])
+        coordinate_list = CoordinateList(coordinate_grid_in_pixels.get()[nonzero])
 
         return cls(flat_potential, coordinate_list, voxel_size)
 
     @classmethod
     def from_atoms(
-        cls: Type[Self],
-        atom_positions: Float[Array, "N 3"],
-        atom_identities: Int[Array, " N"],
+        cls,
+        atom_positions: Float[Array, "n_atoms 3"] | Float[np.ndarray, "n_atoms 3"],
+        atom_identities: Int[Array, " n_atoms"] | Int[np.ndarray, " n_atoms"],
         voxel_size: Float[Array, ""] | Float[np.ndarray, ""] | float,
         coordinate_grid_in_angstroms: CoordinateGrid,
-        form_factors: Optional[Float[Array, "N 5"]] = None,
+        form_factors: Optional[
+            Float[Array, "n_atoms n_form_factors"]
+            | Float[np.ndarray, "n_atoms n_form_factors"]
+        ] = None,
         **kwargs: Any,
     ) -> Self:
         """Load a `RealVoxelCloudPotential` from atom positions and identities.
 
         **Arguments:**
 
         - `**kwargs`: Passed to `RealVoxelCloudPotential.from_real_voxel_grid`
         """
-        a_vals, b_vals = get_form_factor_params(atom_identities, form_factors)
+        form_factors = (
+            form_factors if form_factors is None else jnp.asarray(form_factors)
+        )
+        a_vals, b_vals = get_form_factor_params(
+            jnp.asarray(atom_identities), form_factors
+        )
 
         real_voxel_grid = build_real_space_voxels_from_atoms(
-            atom_positions, a_vals, b_vals, coordinate_grid_in_angstroms.get()
+            jnp.asarray(atom_positions),
+            a_vals,
+            b_vals,
+            coordinate_grid_in_angstroms.get(),
         )
 
         return cls.from_real_voxel_grid(
             real_voxel_grid,
             voxel_size,
-            coordinate_grid=coordinate_grid_in_angstroms / voxel_size,
+            coordinate_grid_in_pixels=coordinate_grid_in_angstroms / voxel_size,
             **kwargs,
         )
 
 
 def evaluate_3d_real_space_gaussian(
-    coordinate_grid_in_angstroms: Float[Array, "N1 N2 N3 3"],
+    coordinate_grid_in_angstroms: Float[Array, "z_dim y_dim x_dim 3"],
     atom_position: Float[Array, "3"],
     a: Float[Array, ""],
     b: Float[Array, ""],
-) -> Float[Array, "N1 N2 N3"]:
+) -> Float[Array, "z_dim y_dim x_dim"]:
     """Evaluate a gaussian on a 3D grid.
     The naming convention for parameters follows "Robust
     Parameterization of Elastic and Absorptive Electron Atomic Scattering
     Factors" by Peng et al.
 
     **Arguments:**
 
@@ -558,19 +587,19 @@
     sq_distances = jnp.sum(
         b_inverse * (coordinate_grid_in_angstroms - atom_position) ** 2, axis=-1
     )
     return jnp.exp(-jnp.pi * sq_distances) * a * b_inverse ** (3.0 / 2.0)
 
 
 def evaluate_3d_atom_potential(
-    coordinate_grid_in_angstroms: Float[Array, "N1 N2 N3 3"],
+    coordinate_grid_in_angstroms: Float[Array, "z_dim y_dim x_dim 3"],
     atom_position: Float[Array, "3"],
-    atomic_as: Float[Array, "5"],
-    atomic_bs: Float[Array, "5"],
-) -> Float[Array, "N1 N2 N3"]:
+    atomic_as: Float[Array, " n_form_factors"],
+    atomic_bs: Float[Array, " n_form_factors"],
+) -> Float[Array, "z_dim y_dim x_dim"]:
     """Evaluates the electron potential of a single atom on a 3D grid.
 
     **Arguments:**
 
     - `coordinate_grid_in_angstroms`: The coordinate system of the grid.
     - `atom_position`: The location of the atom.
     - `atomic_as`: The intensity values for each gaussian in the atom.
@@ -585,19 +614,19 @@
         eval_fxn(coordinate_grid_in_angstroms, atom_position, atomic_as, atomic_bs),
         axis=0,
     )
 
 
 @jax.jit
 def build_real_space_voxels_from_atoms(
-    atom_positions: Float[Array, "N 3"],
-    ff_a: Float[Array, "N 5"],
-    ff_b: Float[Array, "N 5"],
-    coordinate_grid_in_angstroms: Float[Array, "N1 N2 N3 3"],
-) -> RealCubicVolume:
+    atom_positions: Float[Array, "n_atoms 3"],
+    ff_a: Float[Array, "n_atoms n_form_factors"],
+    ff_b: Float[Array, "n_atoms n_form_factors"],
+    coordinate_grid_in_angstroms: Float[Array, "dim dim dim 3"],
+) -> Float[Array, "dim dim dim"]:
     """
     Build a voxel representation of an atomic model.
 
     **Arguments**
 
     - `atom_coords`: The coordinates of the atoms.
     - `ff_a`: Intensity values for each Gaussian in the atom
```

### Comparing `cryojax-0.2.2rc1/tests/conftest.py` & `cryojax-0.2.3rc1/tests/conftest.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,26 @@
 import os
 
 import equinox as eqx
 import jax
+import jax.numpy as jnp
 import jax.random as jr
-import numpy as np
 import pytest
+from jaxtyping import install_import_hook
 
-import cryojax.simulator as cs
-from cryojax.image import operators as op, rfftn
-from cryojax.io import read_array_with_spacing_from_mrc
 
+with install_import_hook("cryojax", "typeguard.typechecked"):
+    import cryojax as cryojax
+    import cryojax.simulator as cs
+    from cryojax.image import operators as op, rfftn
+    from cryojax.io import read_array_with_spacing_from_mrc
 
+
+# jax.config.update("jax_numpy_dtype_promotion", "strict")
+# jax.config.update("jax_numpy_rank_promotion", "raise")
 jax.config.update("jax_enable_x64", True)
 
 
 @pytest.fixture
 def sample_mrc_path():
     return os.path.join(os.path.dirname(__file__), "data", "3j9g_potential_ps4_4.mrc")
 
@@ -29,31 +35,31 @@
 @pytest.fixture
 def sample_pdb_path():
     return os.path.join(os.path.dirname(__file__), "data", "1uao.pdb")
 
 
 @pytest.fixture
 def toy_gaussian_cloud():
-    atom_positions = np.array(
+    atom_positions = jnp.array(
         [
             [0.0, 0.0, 0.0],
             [0.0, 0.0, 1.0],
             [1.0, 0.0, 0.0],
             [0.0, 1.0, 0.0],
         ]
     )
     num_atoms = atom_positions.shape[0]
-    ff_a = np.array(
+    ff_a = jnp.array(
         num_atoms
         * [
             [1.0, 0.5],
         ]
     )
 
-    ff_b = np.array(
+    ff_b = jnp.array(
         num_atoms
         * [
             [0.3, 0.2],
         ]
     )
 
     n_voxels_per_side = (128, 128, 128)
@@ -82,31 +88,33 @@
     return cs.FourierVoxelGridPotential.from_real_voxel_grid(
         real_voxel_grid, voxel_size, pad_scale=1.3
     )
 
 
 @pytest.fixture
 def filters(config):
-    return op.LowpassFilter(config.wrapped_padded_frequency_grid.get())
+    return op.LowpassFilter(config.wrapped_padded_frequency_grid_in_pixels.get())
 
 
 @pytest.fixture
 def masks(config):
     return op.CircularMask(
         config.wrapped_padded_coordinate_grid_in_angstroms.get(),
-        radius=20 * config.pixel_size,
+        radius=20 * float(config.pixel_size),
     )
 
 
 @pytest.fixture
 def instrument():
+    voltage_in_kilovolts = 300.0
     return cs.Instrument(
-        cs.WeakPhaseOptics(cs.CTF()),
-        cs.ElectronDose(electrons_per_angstrom_squared=1000.0),
-        cs.GaussianDetector(cs.IdealDQE(fraction_detected_electrons=1.0)),
+        voltage_in_kilovolts,
+        optics=cs.WeakPhaseOptics(cs.CTF()),
+        dose=cs.ElectronDose(electrons_per_angstrom_squared=1000.0),
+        detector=cs.GaussianDetector(cs.IdealDQE(fraction_detected_electrons=1.0)),
     )
 
 
 @pytest.fixture
 def pose():
     return cs.EulerAnglePose(
         view_phi=30.0,
@@ -125,15 +133,15 @@
 @pytest.fixture
 def solvent():
     return cs.GaussianIce(op.Constant(0.001**2))
 
 
 @pytest.fixture
 def noiseless_model(config, specimen, instrument):
-    instrument = eqx.tree_at(lambda ins: ins.detector, instrument, cs.NullDetector())
+    instrument = eqx.tree_at(lambda ins: ins.detector, instrument, None)
     return cs.ImagePipeline(config=config, specimen=specimen, instrument=instrument)
 
 
 @pytest.fixture
 def noisy_model(config, specimen, instrument, solvent):
     return cs.ImagePipeline(
         config=config,
```

### Comparing `cryojax-0.2.2rc1/tests/test_agree_with_cistem.py` & `cryojax-0.2.3rc1/tests/test_agree_with_cistem.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,23 +13,23 @@
 
 jax.config.update("jax_enable_x64", True)
 
 
 @pytest.mark.parametrize(
     "defocus1,defocus2,asti_angle,kV,cs,ac,pixel_size",
     [
-        (12000, 12000, 0.0, 300.0, 2.7, 0.07, 1.0),
-        (12000, 12000, 0.0, 200.0, 0.01, 0.12, 1.3),
-        (1200, 1200, 0.0, 300.0, 2.7, 0.07, 1.5),
-        (24000, 12000, 30.0, 300.0, 2.7, 0.07, 0.9),
-        (24000, 24000, 0.0, 300.0, 2.7, 0.07, 2.0),
-        (9000, 7000, 180.0, 300.0, 2.7, 0.07, 1.0),
-        (12000, 9000, 0.0, 200.0, 2.7, 0.07, 0.9),
-        (12000, 12000, 60.0, 200.0, 2.7, 0.02, 0.75),
-        (12000, 3895, 45.0, 200.0, 2.7, 0.07, 2.2),
+        (12000.0, 12000.0, 0.0, 300.0, 2.7, 0.07, 1.0),
+        (12000.0, 12000.0, 0.0, 200.0, 0.01, 0.12, 1.3),
+        (1200.0, 1200.0, 0.0, 300.0, 2.7, 0.07, 1.5),
+        (24000.0, 12000.0, 30.0, 300.0, 2.7, 0.07, 0.9),
+        (24000.0, 24000.0, 0.0, 300.0, 2.7, 0.07, 2.0),
+        (9000.0, 7000.0, 180.0, 300.0, 2.7, 0.07, 1.0),
+        (12000.0, 9000.0, 0.0, 200.0, 2.7, 0.07, 0.9),
+        (12000.0, 12000.0, 60.0, 200.0, 2.7, 0.02, 0.75),
+        (12000.0, 3895.0, 45.0, 200.0, 2.7, 0.07, 2.2),
     ],
 )
 def test_ctf_with_cistem(defocus1, defocus2, asti_angle, kV, cs, ac, pixel_size):
     """Test CTF model against cisTEM.
 
     Modified from https://github.com/jojoelfe/contrasttransferfunction"""
     shape = (512, 512)
@@ -71,15 +71,15 @@
 
     np.testing.assert_allclose(ctf, cisTEM_ctf, atol=5e-2)
     np.testing.assert_allclose(spectrum1D, cisTEM_spectrum1D, atol=5e-3)
 
 
 @pytest.mark.parametrize(
     "phi, theta, psi",
-    [(10, 90, 170)],
+    [(10.0, 90.0, 170.0)],
     # [(10, 80, -20), (1.2, -90.5, 67), (-50, 62, -21)],
 )
 def test_euler_matrix_with_cistem(phi, theta, psi):
     """Test zyz rotation matrix"""
     # Hard code zyz rotation matrix from cisTEM convention
     phi_in_rad, theta_in_rad, psi_in_rad = [
         np.deg2rad(angle) for angle in [phi, theta, psi]
@@ -103,15 +103,15 @@
     # Generate rotation that matches this rotation matrix
     pose = EulerAnglePose(view_phi=phi, view_theta=theta, view_psi=psi)
     np.testing.assert_allclose(pose.rotation.as_matrix(), matrix.T, atol=1e-12)
 
 
 @pytest.mark.parametrize(
     "phi, theta, psi",
-    [(10, 90, 170)],
+    [(10.0, 90.0, 170.0)],
 )
 def test_compute_projection_with_cistem(
     phi,
     theta,
     psi,
     sample_mrc_path,
     pixel_size,
@@ -122,15 +122,16 @@
         real_voxel_grid, voxel_size
     )
     pose = cs.EulerAnglePose(view_phi=phi, view_theta=theta, view_psi=psi)
     integrator = cs.FourierSliceExtract()
     specimen = cs.Specimen(potential, integrator, pose)
     box_size = potential.shape[0]
     config = cs.ImageConfig((box_size, box_size), pixel_size)
-    pipeline = cs.ImagePipeline(config, specimen)
+    instrument = cs.Instrument(voltage_in_kilovolts=300.0)
+    pipeline = cs.ImagePipeline(config, specimen, instrument)
     cryojax_projection = irfftn(
         pipeline.render(get_real=False).at[0, 0].set(0.0 + 0.0j)
         / np.sqrt(np.prod(config.shape)),
         s=config.padded_shape,
     )
     # pycistem
     pycistem_volume = _load_pycistem_template(sample_mrc_path, box_size)
```

### Comparing `cryojax-0.2.2rc1/tests/test_atom_routines.py` & `cryojax-0.2.3rc1/tests/test_atom_routines.py`

 * *Files identical despite different names*

### Comparing `cryojax-0.2.2rc1/tests/test_detector.py` & `cryojax-0.2.3rc1/tests/test_detector.py`

 * *Files 11% similar despite different names*

```diff
@@ -16,23 +16,29 @@
     # Create squared wavefunction of just vacuum, i.e. 1 everywhere
     vacuum_squared_wavefunction = jnp.ones(config.shape, dtype=float)
     fourier_vacuum_squared_wavefunction = rfftn(vacuum_squared_wavefunction)
     # Instantiate the electron dose
     dose = cs.ElectronDose(electrons_per_angstrom_squared)
     # Create detector models
     key = jax.random.PRNGKey(1234)
-    dqe = cs.NullDQE()
+    dqe = cs.IdealDQE()
     gaussian_detector = cs.GaussianDetector(dqe)
     poisson_detector = cs.PoissonDetector(dqe)
     # Compute detector readout
     fourier_gaussian_detector_readout = gaussian_detector(
-        fourier_vacuum_squared_wavefunction, dose, config, key
+        fourier_vacuum_squared_wavefunction,
+        config,
+        dose.electrons_per_angstrom_squared,
+        key,
     )
     fourier_poisson_detector_readout = poisson_detector(
-        fourier_vacuum_squared_wavefunction, dose, config, key
+        fourier_vacuum_squared_wavefunction,
+        config,
+        dose.electrons_per_angstrom_squared,
+        key,
     )
     # Compare to see if the autocorrelation has converged
     np.testing.assert_allclose(
         irfftn(
             jnp.abs(fourier_gaussian_detector_readout) ** 2
             / (N_pix * electrons_per_pixel**2),
             s=config.padded_shape,
```

### Comparing `cryojax-0.2.2rc1/tests/test_ensemble.py` & `cryojax-0.2.3rc1/tests/test_ensemble.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,40 +1,44 @@
 from functools import partial
 
 import equinox as eqx
 import jax
 import jax.numpy as jnp
 import jax.tree_util as jtu
 
-from cryojax.simulator import DiscreteConformation, DiscreteEnsemble
+from cryojax.simulator import DiscreteConformation, DiscreteEnsemble, Instrument
 
 
 def test_conformation(potential, pose, integrator, config):
     potential = tuple([potential for _ in range(3)])
     ensemble = DiscreteEnsemble(
         potential, integrator, pose, conformation=DiscreteConformation(0)
     )
-    _ = ensemble.scatter_to_exit_plane(config)
+    instrument = Instrument(300.0)
+    _ = ensemble.scatter_to_exit_plane(instrument, config)
 
 
 def test_conformation_vmap(potential, pose, integrator, config):
     # Build Ensemble
     stacked_potential = tuple([potential for _ in range(3)])
     ensemble = DiscreteEnsemble(
         stacked_potential,
         integrator,
         pose,
-        conformation=DiscreteConformation(jnp.asarray((0, 1, 2, 1, 0))),
+        conformation=jax.vmap(lambda value: DiscreteConformation(value))(
+            jnp.asarray((0, 1, 2, 1, 0))
+        ),
     )
     # Setup vmap
     is_vmap = lambda x: isinstance(x, DiscreteConformation)
     to_vmap = jtu.tree_map(is_vmap, ensemble, is_leaf=is_vmap)
     vmap, novmap = eqx.partition(ensemble, to_vmap)
 
     @partial(jax.vmap, in_axes=[0, None, None])
     def compute_conformation_stack(vmap, novmap, config):
         ensemble = eqx.combine(vmap, novmap)
-        return ensemble.scatter_to_exit_plane(config)
+        instrument = Instrument(300.0)
+        return ensemble.scatter_to_exit_plane(instrument, config)
 
     # Vmap over conformations
     image_stack = compute_conformation_stack(vmap, novmap, config)
     assert image_stack.shape[0] == ensemble.conformation.value.shape[0]
```

### Comparing `cryojax-0.2.2rc1/tests/test_fft.py` & `cryojax-0.2.3rc1/tests/test_fft.py`

 * *Files identical despite different names*

### Comparing `cryojax-0.2.2rc1/tests/test_filters_and_masks.py` & `cryojax-0.2.3rc1/tests/test_filters_and_masks.py`

 * *Files identical despite different names*

### Comparing `cryojax-0.2.2rc1/tests/test_helix.py` & `cryojax-0.2.3rc1/tests/test_helix.py`

 * *Files 16% similar despite different names*

```diff
@@ -45,37 +45,41 @@
     integrator = cs.FourierSliceExtract()
     subunit = cs.DiscreteEnsemble(
         subunit_density,
         integrator,
         subunit_pose,
         conformation=cs.DiscreteConformation(0),
     )
-    conformation = cs.DiscreteConformation(
+    conformation = jax.vmap(lambda value: cs.DiscreteConformation(value))(
         np.random.choice(2, n_start * n_subunits_per_start)
     )
     return cs.Helix(
         subunit,
         conformation=conformation,
         rise=21.8,
         twist=29.4,
         n_start=n_start,
         n_subunits=n_subunits_per_start * 6,
     )
 
 
 def test_superposition_pipeline_without_conformation(sample_subunit_mrc_path, config):
     helix = build_helix(sample_subunit_mrc_path, 1)
-    pipeline = cs.AssemblyPipeline(config=config, assembly=helix)
+    pipeline = cs.AssemblyPipeline(
+        config=config, assembly=helix, instrument=cs.Instrument(300.0)
+    )
     _ = pipeline.render()
     _ = pipeline.sample(jax.random.PRNGKey(0))
 
 
 def test_superposition_pipeline_with_conformation(sample_subunit_mrc_path, config):
     helix = build_helix_with_conformation(sample_subunit_mrc_path, 2)
-    pipeline = cs.AssemblyPipeline(config=config, assembly=helix)
+    pipeline = cs.AssemblyPipeline(
+        config=config, instrument=cs.Instrument(300.0), assembly=helix
+    )
     _ = pipeline.render()
     _ = pipeline.sample(jax.random.PRNGKey(0))
 
 
 @pytest.mark.parametrize(
     "rotation_angle, n_subunits_per_start",
     [(360.0 / 6, 1), (2 * 360.0 / 6, 1), (360.0 / 6, 2)],
@@ -84,15 +88,17 @@
     sample_subunit_mrc_path, config, rotation_angle, n_subunits_per_start
 ):
     helix = build_helix(sample_subunit_mrc_path, n_subunits_per_start)
 
     @jax.jit
     def compute_rotated_image(config, helix, pose):
         helix = eqx.tree_at(lambda m: m.pose, helix, pose)
-        pipeline = cs.AssemblyPipeline(config=config, assembly=helix)
+        pipeline = cs.AssemblyPipeline(
+            config=config, instrument=cs.Instrument(300.0), assembly=helix
+        )
         return pipeline.render(normalize=True)
 
     np.testing.assert_allclose(
         compute_rotated_image(config, helix, cs.EulerAnglePose()),
         compute_rotated_image(
             config, helix, cs.EulerAnglePose(view_phi=rotation_angle)
         ),
@@ -105,48 +111,59 @@
         ((0.0, 0.0), (60.0, 100.0, -40.0)),
         ((1.0, -3.0), (10.0, 50.0, 100.0)),
     ],
 )
 def test_agree_with_3j9g_assembly(
     sample_subunit_mrc_path, potential, config, translation, euler_angles
 ):
+    instrument = cs.Instrument(voltage_in_kilovolts=300.0)
     helix = build_helix(sample_subunit_mrc_path, 2)
     specimen_39jg = cs.Specimen(potential, helix.subunit.integrator)
+    pipeline_for_assembly = cs.AssemblyPipeline(
+        config=config, instrument=instrument, assembly=helix
+    )
+    pipeline_for_3j9g = cs.ImagePipeline(
+        config=config, instrument=instrument, specimen=specimen_39jg
+    )
 
-    @jax.jit
-    def compute_rotated_image_with_helix(helix, config, pose):
-        helix = eqx.tree_at(lambda m: m.pose, helix, pose)
-        pipeline = cs.AssemblyPipeline(config=config, assembly=helix)
+    @eqx.filter_jit
+    def compute_rotated_image_with_helix(
+        pipeline: cs.AssemblyPipeline, pose: cs.AbstractPose
+    ):
+        pipeline = eqx.tree_at(lambda m: m.assembly.pose, pipeline, pose)
         return pipeline.render(normalize=True)
 
-    @jax.jit
-    def compute_rotated_image_with_3j9g(specimen, config, pose):
-        specimen = eqx.tree_at(lambda m: m.pose, specimen, pose)
-        pipeline = cs.ImagePipeline(config=config, specimen=specimen)
+    @eqx.filter_jit
+    def compute_rotated_image_with_3j9g(
+        pipeline: cs.ImagePipeline, pose: cs.AbstractPose
+    ):
+        pipeline = eqx.tree_at(lambda m: m.specimen.pose, pipeline, pose)
         return pipeline.render(normalize=True)
 
     pose = cs.EulerAnglePose(*translation, 0.0, *euler_angles)
     reference_image = compute_rotated_image_with_3j9g(
-        specimen_39jg, config, cs.EulerAnglePose()
+        pipeline_for_3j9g, cs.EulerAnglePose()
     )
-    assembled_image = compute_rotated_image_with_helix(helix, config, pose)
-    test_image = compute_rotated_image_with_3j9g(specimen_39jg, config, pose)
+    assembled_image = compute_rotated_image_with_helix(pipeline_for_assembly, pose)
+    test_image = compute_rotated_image_with_3j9g(pipeline_for_3j9g, pose)
     assert np.std(assembled_image - test_image) < 10 * np.std(
         assembled_image - reference_image
     )
 
 
 def test_transform_by_rise_and_twist(sample_subunit_mrc_path, pixel_size):
     helix = build_helix(sample_subunit_mrc_path, 12)
     config = cs.ImageConfig((50, 20), pixel_size, pad_scale=6)
 
     @jax.jit
     def compute_rotated_image(config, helix, pose):
         helix = eqx.tree_at(lambda m: m.pose, helix, pose)
-        pipeline = cs.AssemblyPipeline(config=config, assembly=helix)
+        pipeline = cs.AssemblyPipeline(
+            config=config, instrument=cs.Instrument(300.0), assembly=helix
+        )
         return pipeline.render(normalize=True)
 
     np.testing.assert_allclose(
         compute_rotated_image(
             config,
             helix,
             cs.EulerAnglePose(view_phi=0.0, view_theta=90.0, view_psi=0.0),
```

### Comparing `cryojax-0.2.2rc1/tests/test_normalize.py` & `cryojax-0.2.3rc1/tests/test_normalize.py`

 * *Files identical despite different names*

### Comparing `cryojax-0.2.2rc1/tests/test_pose_agreement.py` & `cryojax-0.2.3rc1/tests/test_pose_agreement.py`

 * *Files identical despite different names*

### Comparing `cryojax-0.2.2rc1/tests/test_potential.py` & `cryojax-0.2.3rc1/tests/test_potential.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 from functools import partial
 
 import equinox as eqx
 import jax
 import jax.numpy as jnp
 import jax.tree_util as jtu
+from jaxtyping import Array, Float
 
 import cryojax.simulator as cs
+from cryojax.constants import convert_keV_to_angstroms
 from cryojax.coordinates import (
     AbstractCoordinates,
     CoordinateGrid,
     CoordinateList,
     FrequencySlice,
 )
-from cryojax.typing import PointCloudCoords3D, VolumeCoords, VolumeSliceCoords
 
 
 def test_voxel_electron_potential_loaders():
     real_voxel_grid = jnp.zeros((10, 10, 10), dtype=float)
     voxel_size = 1.1
     fourier_potential = cs.FourierVoxelGridPotential.from_real_voxel_grid(
         real_voxel_grid, voxel_size=voxel_size
@@ -26,22 +27,29 @@
     )
     cloud_potential = cs.RealVoxelCloudPotential.from_real_voxel_grid(
         real_voxel_grid, voxel_size=voxel_size
     )
     for potential in [real_potential, fourier_potential, cloud_potential]:
         assert potential.voxel_size == jnp.asarray(voxel_size)
 
-    assert isinstance(fourier_potential.wrapped_frequency_slice, FrequencySlice)
     assert isinstance(
-        fourier_potential.wrapped_frequency_slice.get(), VolumeSliceCoords
+        fourier_potential.wrapped_frequency_slice_in_pixels, FrequencySlice
+    )
+    assert isinstance(
+        fourier_potential.wrapped_frequency_slice_in_pixels.get(),
+        Float[Array, "1 _ _ 3"],
+    )
+    assert isinstance(real_potential.wrapped_coordinate_grid_in_pixels, CoordinateGrid)
+    assert isinstance(
+        real_potential.wrapped_coordinate_grid_in_pixels.get(), Float[Array, "_ _ _ 3"]
+    )
+    assert isinstance(cloud_potential.wrapped_coordinate_list_in_pixels, CoordinateList)
+    assert isinstance(
+        cloud_potential.wrapped_coordinate_list_in_pixels.get(), Float[Array, "_ 3"]
     )
-    assert isinstance(real_potential.wrapped_coordinate_grid, CoordinateGrid)
-    assert isinstance(real_potential.wrapped_coordinate_grid.get(), VolumeCoords)
-    assert isinstance(cloud_potential.wrapped_coordinate_list, CoordinateList)
-    assert isinstance(cloud_potential.wrapped_coordinate_list.get(), PointCloudCoords3D)
 
 
 def test_electron_potential_vmap(potential, integrator, config):
     filter_spec = jtu.tree_map(
         lambda x: not isinstance(x, AbstractCoordinates),
         potential,
         is_leaf=lambda x: isinstance(x, AbstractCoordinates),
@@ -53,24 +61,28 @@
         potential,
         is_leaf=lambda x: isinstance(x, AbstractCoordinates),
     )
     vmap, novmap = eqx.partition(potential, filter_spec)
 
     @partial(jax.vmap, in_axes=[0, None, None, None])
     def compute_image_stack(vmap, novmap, integrator, config):
+        wavelength_in_angstroms = convert_keV_to_angstroms(300.0)
         potential = eqx.combine(vmap, novmap)
-        return integrator(potential, config)
+        return integrator(potential, wavelength_in_angstroms, config)
 
     # vmap over first axis
     image_stack = compute_image_stack(vmap, novmap, integrator, config)
     assert image_stack.shape[:1] == (1,)
 
 
 def test_electron_potential_vmap_with_pipeline(potential, pose, integrator, config):
-    pipeline = cs.ImagePipeline(config, cs.Specimen(potential, integrator, pose))
+    instrument = cs.Instrument(voltage_in_kilovolts=300.0)
+    pipeline = cs.ImagePipeline(
+        config, cs.Specimen(potential, integrator, pose), instrument
+    )
 
     def is_potential_leaves_without_coordinates(element):
         if isinstance(element, cs.AbstractScatteringPotential):
             return jtu.tree_map(
                 lambda x: not isinstance(x, AbstractCoordinates),
                 potential,
                 is_leaf=lambda x: isinstance(x, AbstractCoordinates),
```

### Comparing `cryojax-0.2.2rc1/tests/test_projection_agreement.py` & `cryojax-0.2.3rc1/tests/test_projection_agreement.py`

 * *Files 14% similar despite different names*

```diff
@@ -19,14 +19,15 @@
     )
     assert control_shape == potential.fourier_voxel_grid.shape[0:2]
     pose = cs.EulerAnglePose()
     integrator = cs.FourierSliceExtract()
     specimen = cs.Specimen(potential, integrator, pose)
     config_control = cs.ImageConfig(control_shape, pixel_size)
     config_test = cs.ImageConfig(shape, pixel_size)
-    pipeline_control = cs.ImagePipeline(config_control, specimen)
-    pipeline_test = cs.ImagePipeline(config_test, specimen)
+    instrument = cs.Instrument(voltage_in_kilovolts=300.0)
+    pipeline_control = cs.ImagePipeline(config_control, specimen, instrument)
+    pipeline_test = cs.ImagePipeline(config_test, specimen, instrument)
 
     np.testing.assert_allclose(
         crop_to_shape(pipeline_test.render(), control_shape),
         pipeline_control.render(),
     )
```

### Comparing `cryojax-0.2.2rc1/tests/test_shape.py` & `cryojax-0.2.3rc1/tests/test_shape.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import pytest
 
 
 @pytest.mark.parametrize("model", ["noisy_model", "filtered_and_masked_model"])
 def test_real_shape(model, request):
     """Make sure shapes are as expected in real space."""
     model = request.getfixturevalue(model)
-    image = model()
-    padded_image = model(view_cropped=False)
+    image = model.render()
+    padded_image = model.render(view_cropped=False)
     assert image.shape == model.config.shape
     assert padded_image.shape == model.config.padded_shape
 
 
 @pytest.mark.parametrize("model", ["noisy_model", "filtered_and_masked_model"])
 def test_fourier_shape(model, request):
     """Make sure shapes are as expected in fourier space."""
     model = request.getfixturevalue(model)
-    image = model(get_real=False)
-    padded_image = model(view_cropped=False, get_real=False)
-    assert image.shape == model.config.wrapped_frequency_grid.get().shape[0:2]
+    image = model.render(get_real=False)
+    padded_image = model.render(view_cropped=False, get_real=False)
+    assert image.shape == model.config.wrapped_frequency_grid_in_pixels.get().shape[0:2]
     assert (
         padded_image.shape
-        == model.config.wrapped_padded_frequency_grid.get().shape[0:2]
+        == model.config.wrapped_padded_frequency_grid_in_pixels.get().shape[0:2]
     )
```

### Comparing `cryojax-0.2.2rc1/tests/test_voxels_from_atoms.py` & `cryojax-0.2.3rc1/tests/test_voxels_from_atoms.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,15 +57,15 @@
         (
             atom_positions,
             ff_a,
             ff_b,
             n_voxels_per_side,
             voxel_size,
         ) = toy_gaussian_cloud
-        ff_a[largest_atom] += 1.0
+        ff_a = ff_a.at[largest_atom].add(1.0)
         coordinate_grid = CoordinateGrid(n_voxels_per_side, voxel_size)
 
         # Build the potential
         real_voxel_grid = build_real_space_voxels_from_atoms(
             atom_positions, ff_a, ff_b, coordinate_grid.get()
         )
 
@@ -104,20 +104,20 @@
             atom_positions,
             ff_a,
             ff_b,
             n_voxels_per_side,
             voxel_size,
         ) = toy_gaussian_cloud
         second_set_of_positions = atom_positions + 1.0
-        traj = np.stack([atom_positions, second_set_of_positions], axis=0)
+        traj = jnp.stack([atom_positions, second_set_of_positions], axis=0)
 
         coordinate_grid = CoordinateGrid(n_voxels_per_side, voxel_size)
 
         # Build the trajectory $density
-        elements = np.array([1, 1, 2, 6])
+        elements = jnp.array([1, 1, 2, 6])
 
         make_voxel_grid_ensemble = jax.vmap(
             RealVoxelGridPotential.from_atoms, in_axes=[0, None, None, None]
         )
         traj_voxels = make_voxel_grid_ensemble(
             traj, elements, voxel_size, coordinate_grid
         )
```

### Comparing `cryojax-0.2.2rc1/LICENSE` & `cryojax-0.2.3rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `cryojax-0.2.2rc1/README.md` & `cryojax-0.2.3rc1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -88,19 +88,19 @@
 from cryojax.image import operators as op
 
 # First, initialize the CTF and its optics model
 ctf = cs.CTF(
     defocus_u_in_angstroms=10000.0,
     defocus_v_in_angstroms=9800.0,
     astigmatism_angle=10.0,
-    voltage_in_kilovolts=300.0,
     amplitude_contrast_ratio=0.1)
 optics = cs.WeakPhaseOptics(ctf, envelope=op.FourierGaussian(b_factor=5.0))  # b_factor is given in Angstroms^2
 # ... these are stored in the Instrument
-instrument = cs.Instrument(optics)
+voltage_in_kilovolts = 300.0,
+instrument = cs.Instrument(voltage_in_kilovolts, optics)
 ```
 
 The `CTF` has parameters used in CTFFIND4, which take their default values if not
 explicitly configured here. Finally, we can instantiate the `ImagePipeline` and simulate an image.
 
 ```python
 # Instantiate the image configuration
```

### Comparing `cryojax-0.2.2rc1/pyproject.toml` & `cryojax-0.2.3rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `cryojax-0.2.2rc1/PKG-INFO` & `cryojax-0.2.3rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: cryojax
-Version: 0.2.2rc1
+Version: 0.2.3rc1
 Summary: Cryo-EM image simulation and analysis powered by JAX
 Project-URL: repository, https://github.com/mjo22/cryojax
 Author-email: Michael O'Brien <michaelobrien@g.harvard.edu>
 License:                   GNU LESSER GENERAL PUBLIC LICENSE
                                Version 2.1, February 1999
         
          Copyright (C) 1991, 1999 Free Software Foundation, Inc.
@@ -623,19 +623,19 @@
 from cryojax.image import operators as op
 
 # First, initialize the CTF and its optics model
 ctf = cs.CTF(
     defocus_u_in_angstroms=10000.0,
     defocus_v_in_angstroms=9800.0,
     astigmatism_angle=10.0,
-    voltage_in_kilovolts=300.0,
     amplitude_contrast_ratio=0.1)
 optics = cs.WeakPhaseOptics(ctf, envelope=op.FourierGaussian(b_factor=5.0))  # b_factor is given in Angstroms^2
 # ... these are stored in the Instrument
-instrument = cs.Instrument(optics)
+voltage_in_kilovolts = 300.0,
+instrument = cs.Instrument(voltage_in_kilovolts, optics)
 ```
 
 The `CTF` has parameters used in CTFFIND4, which take their default values if not
 explicitly configured here. Finally, we can instantiate the `ImagePipeline` and simulate an image.
 
 ```python
 # Instantiate the image configuration
```

