# Comparing `tmp/cryojax-0.2.3rc1.tar.gz` & `tmp/cryojax-0.3.0a0.tar.gz`

## Comparing `cryojax-0.2.3rc1.tar` & `cryojax-0.3.0a0.tar`

### file list

```diff
@@ -1,119 +1,130 @@
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 cryojax-0.2.3rc1/.gitattributes
--rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 cryojax-0.2.3rc1/.pre-commit-config.yaml
--rw-r--r--   0        0        0     2084 2020-02-02 00:00:00.000000 cryojax-0.2.3rc1/CONTRIBUTING.md
--rw-r--r--   0        0        0     2147 2020-02-02 00:00:00.000000 cryojax-0.2.3rc1/mkdocs.yml
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 cryojax-0.2.3rc1/.github/dependabot.yml
--rw-r--r--   0        0        0     1110 2020-02-02 00:00:00.000000 cryojax-0.2.3rc1/.github/workflows/build_docs.yml
--rw-r--r--   0        0        0      784 2020-02-02 00:00:00.000000 cryojax-0.2.3rc1/.github/workflows/release.yml
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 cryojax-0.2.3rc1/.github/workflows/ruff.yml
--rw-r--r--   0        0        0     1000 2020-02-02 00:00:00.000000 cryojax-0.2.3rc1/.github/workflows/testing.yml
--rw-r--r--   0        0        0     6088 2020-02-02 00:00:00.000000 cryojax-0.2.3rc1/docs/index.md
--rw-r--r--   0        0        0     3108 2020-02-02 00:00:00.000000 cryojax-0.2.3rc1/docs/_static/custom_css.css
--rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 cryojax-0.2.3rc1/docs/_static/mathjax.js
--rw-r--r--   0        0        0     2713 2020-02-02 00:00:00.000000 cryojax-0.2.3rc1/docs/api/simulator/scattering_potential.md
--rw-r--r--   0        0        0   511451 2020-02-02 00:00:00.000000 cryojax-0.2.3rc1/docs/examples/read-dataset.ipynb
--rw-r--r--   0        0        0     7539 2020-02-02 00:00:00.000000 cryojax-0.2.3rc1/docs/examples/simulate-helix.ipynb
--rw-r--r--   0        0        0   230839 2020-02-02 00:00:00.000000 cryojax-0.2.3rc1/docs/examples/simulate-image.ipynb
--rw-r--r--   0        0        0   137948 2020-02-02 00:00:00.000000 cryojax-0.2.3rc1/docs/examples/simulate-micrograph.ipynb
--rw-r--r--   0        0        0    13153 2020-02-02 00:00:00.000000 cryojax-0.2.3rc1/docs/examples/test-multiatom.ipynb
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cryojax-0.2.3rc1/docs/examples/data/.gitkeep
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 cryojax-0.2.3rc1/docs/examples/data/ribosome_4ug0_micrograph.mrc
--rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 cryojax-0.2.3rc1/docs/examples/data/ribosome_4ug0_micrograph.mrcs
--rw-r--r--   0        0        0     2019 2020-02-02 00:00:00.000000 cryojax-0.2.3rc1/docs/examples/data/ribosome_4ug0_particles.star
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 cryojax-0.2.3rc1/docs/examples/data/ribosome_4ug0_scattering_potential_from_cistem.mrc
--rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 cryojax-0.2.3rc1/src/cryojax/__init__.py
--rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 cryojax-0.2.3rc1/src/cryojax/cryojax_version.py
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 cryojax-0.2.3rc1/src/cryojax/constants/__init__.py
--rw-r--r--   0        0        0     1653 2020-02-02 00:00:00.000000 cryojax-0.2.3rc1/src/cryojax/constants/_load_atoms.py
--rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 cryojax-0.2.3rc1/src/cryojax/constants/_unit_conversions.py
--rw-r--r--   0        0        0     8048 2020-02-02 00:00:00.000000 cryojax-0.2.3rc1/src/cryojax/constants/element_params.npy
--rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 cryojax-0.2.3rc1/src/cryojax/coordinates/__init__.py
--rw-r--r--   0        0        0     8613 2020-02-02 00:00:00.000000 cryojax-0.2.3rc1/src/cryojax/coordinates/_coordinates.py
--rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 cryojax-0.2.3rc1/src/cryojax/core/__init__.py
--rw-r--r--   0        0        0      902 2020-02-02 00:00:00.000000 cryojax-0.2.3rc1/src/cryojax/core/_errors.py
--rw-r--r--   0        0        0      779 2020-02-02 00:00:00.000000 cryojax-0.2.3rc1/src/cryojax/core/_filter_specs.py
--rw-r--r--   0        0        0     3459 2020-02-02 00:00:00.000000 cryojax-0.2.3rc1/src/cryojax/core/_filtered_transformations.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cryojax-0.2.3rc1/src/cryojax/core/_serialization.py
--rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 cryojax-0.2.3rc1/src/cryojax/data/__init__.py
--rw-r--r--   0        0        0     2861 2020-02-02 00:00:00.000000 cryojax-0.2.3rc1/src/cryojax/data/_dataset.py
--rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 cryojax-0.2.3rc1/src/cryojax/data/_particle_stack.py
--rw-r--r--   0        0        0    17841 2020-02-02 00:00:00.000000 cryojax-0.2.3rc1/src/cryojax/data/_relion.py
--rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 cryojax-0.2.3rc1/src/cryojax/image/__init__.py
--rw-r--r--   0        0        0     3530 2020-02-02 00:00:00.000000 cryojax-0.2.3rc1/src/cryojax/image/_average.py
--rw-r--r--   0        0        0     6259 2020-02-02 00:00:00.000000 cryojax-0.2.3rc1/src/cryojax/image/_edges.py
--rw-r--r--   0        0        0     4644 2020-02-02 00:00:00.000000 cryojax-0.2.3rc1/src/cryojax/image/_fft.py
--rw-r--r--   0        0        0     8242 2020-02-02 00:00:00.000000 cryojax-0.2.3rc1/src/cryojax/image/_map_coordinates.py
--rw-r--r--   0        0        0     3659 2020-02-02 00:00:00.000000 cryojax-0.2.3rc1/src/cryojax/image/_normalize.py
--rw-r--r--   0        0        0     1853 2020-02-02 00:00:00.000000 cryojax-0.2.3rc1/src/cryojax/image/_rescale_pixel_size.py
--rw-r--r--   0        0        0     4549 2020-02-02 00:00:00.000000 cryojax-0.2.3rc1/src/cryojax/image/_spectrum.py
--rw-r--r--   0        0        0     1162 2020-02-02 00:00:00.000000 cryojax-0.2.3rc1/src/cryojax/image/operators/__init__.py
--rw-r--r--   0        0        0     7058 2020-02-02 00:00:00.000000 cryojax-0.2.3rc1/src/cryojax/image/operators/_filters.py
--rw-r--r--   0        0        0     6598 2020-02-02 00:00:00.000000 cryojax-0.2.3rc1/src/cryojax/image/operators/_fourier_operator.py
--rw-r--r--   0        0        0     3687 2020-02-02 00:00:00.000000 cryojax-0.2.3rc1/src/cryojax/image/operators/_masks.py
--rw-r--r--   0        0        0     6563 2020-02-02 00:00:00.000000 cryojax-0.2.3rc1/src/cryojax/image/operators/_operator.py
--rw-r--r--   0        0        0     2533 2020-02-02 00:00:00.000000 cryojax-0.2.3rc1/src/cryojax/image/operators/_real_operator.py
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 cryojax-0.2.3rc1/src/cryojax/inference/__init__.py
--rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 cryojax-0.2.3rc1/src/cryojax/inference/distributions/__init__.py
--rw-r--r--   0        0        0     1673 2020-02-02 00:00:00.000000 cryojax-0.2.3rc1/src/cryojax/inference/distributions/_distribution.py
--rw-r--r--   0        0        0     4534 2020-02-02 00:00:00.000000 cryojax-0.2.3rc1/src/cryojax/inference/distributions/_gaussian_distributions.py
--rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 cryojax-0.2.3rc1/src/cryojax/inference/transforms/__init__.py
--rw-r--r--   0        0        0     4109 2020-02-02 00:00:00.000000 cryojax-0.2.3rc1/src/cryojax/inference/transforms/_lie_group_transforms.py
--rw-r--r--   0        0        0     7634 2020-02-02 00:00:00.000000 cryojax-0.2.3rc1/src/cryojax/inference/transforms/_transforms.py
--rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 cryojax-0.2.3rc1/src/cryojax/io/__init__.py
--rw-r--r--   0        0        0     1584 2020-02-02 00:00:00.000000 cryojax-0.2.3rc1/src/cryojax/io/_cif.py
--rw-r--r--   0        0        0     3056 2020-02-02 00:00:00.000000 cryojax-0.2.3rc1/src/cryojax/io/_gemmi.py
--rw-r--r--   0        0        0     1008 2020-02-02 00:00:00.000000 cryojax-0.2.3rc1/src/cryojax/io/_mdtraj.py
--rw-r--r--   0        0        0     8248 2020-02-02 00:00:00.000000 cryojax-0.2.3rc1/src/cryojax/io/_mrc.py
--rw-r--r--   0        0        0     1861 2020-02-02 00:00:00.000000 cryojax-0.2.3rc1/src/cryojax/io/_pdb.py
--rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 cryojax-0.2.3rc1/src/cryojax/io/_starfile.py
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 cryojax-0.2.3rc1/src/cryojax/rotations/__init__.py
--rw-r--r--   0        0        0    16095 2020-02-02 00:00:00.000000 cryojax-0.2.3rc1/src/cryojax/rotations/_lie_group.py
--rw-r--r--   0        0        0     1934 2020-02-02 00:00:00.000000 cryojax-0.2.3rc1/src/cryojax/rotations/_rotation.py
--rw-r--r--   0        0        0     2445 2020-02-02 00:00:00.000000 cryojax-0.2.3rc1/src/cryojax/simulator/__init__.py
--rw-r--r--   0        0        0     7374 2020-02-02 00:00:00.000000 cryojax-0.2.3rc1/src/cryojax/simulator/_config.py
--rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 cryojax-0.2.3rc1/src/cryojax/simulator/_conformation.py
--rw-r--r--   0        0        0     5580 2020-02-02 00:00:00.000000 cryojax-0.2.3rc1/src/cryojax/simulator/_detector.py
--rw-r--r--   0        0        0      460 2020-02-02 00:00:00.000000 cryojax-0.2.3rc1/src/cryojax/simulator/_dose.py
--rw-r--r--   0        0        0     2644 2020-02-02 00:00:00.000000 cryojax-0.2.3rc1/src/cryojax/simulator/_ice.py
--rw-r--r--   0        0        0     6172 2020-02-02 00:00:00.000000 cryojax-0.2.3rc1/src/cryojax/simulator/_instrument.py
--rw-r--r--   0        0        0     7413 2020-02-02 00:00:00.000000 cryojax-0.2.3rc1/src/cryojax/simulator/_optics.py
--rw-r--r--   0        0        0    22542 2020-02-02 00:00:00.000000 cryojax-0.2.3rc1/src/cryojax/simulator/_pipeline.py
--rw-r--r--   0        0        0    12243 2020-02-02 00:00:00.000000 cryojax-0.2.3rc1/src/cryojax/simulator/_pose.py
--rw-r--r--   0        0        0     5615 2020-02-02 00:00:00.000000 cryojax-0.2.3rc1/src/cryojax/simulator/_specimen.py
--rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 cryojax-0.2.3rc1/src/cryojax/simulator/_assembly/__init__.py
--rw-r--r--   0        0        0     4110 2020-02-02 00:00:00.000000 cryojax-0.2.3rc1/src/cryojax/simulator/_assembly/_assembly.py
--rw-r--r--   0        0        0    10346 2020-02-02 00:00:00.000000 cryojax-0.2.3rc1/src/cryojax/simulator/_assembly/_helix.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 cryojax-0.2.3rc1/src/cryojax/simulator/_integrators/__init__.py
--rw-r--r--   0        0        0     6769 2020-02-02 00:00:00.000000 cryojax-0.2.3rc1/src/cryojax/simulator/_integrators/_fourier_slice_extract.py
--rw-r--r--   0        0        0     4874 2020-02-02 00:00:00.000000 cryojax-0.2.3rc1/src/cryojax/simulator/_integrators/_gaussian_mixture.py
--rw-r--r--   0        0        0     3723 2020-02-02 00:00:00.000000 cryojax-0.2.3rc1/src/cryojax/simulator/_integrators/_nufft_project.py
--rw-r--r--   0        0        0     1237 2020-02-02 00:00:00.000000 cryojax-0.2.3rc1/src/cryojax/simulator/_integrators/_potential_integrator.py
--rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 cryojax-0.2.3rc1/src/cryojax/simulator/_potential/__init__.py
--rw-r--r--   0        0        0     1250 2020-02-02 00:00:00.000000 cryojax-0.2.3rc1/src/cryojax/simulator/_potential/_atom_potential.py
--rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 cryojax-0.2.3rc1/src/cryojax/simulator/_potential/_scattering_potential.py
--rw-r--r--   0        0        0    23788 2020-02-02 00:00:00.000000 cryojax-0.2.3rc1/src/cryojax/simulator/_potential/_voxel_potential.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cryojax-0.2.3rc1/tests/__init__.py
--rw-r--r--   0        0        0     4168 2020-02-02 00:00:00.000000 cryojax-0.2.3rc1/tests/conftest.py
--rw-r--r--   0        0        0     5945 2020-02-02 00:00:00.000000 cryojax-0.2.3rc1/tests/test_agree_with_cistem.py
--rw-r--r--   0        0        0     3678 2020-02-02 00:00:00.000000 cryojax-0.2.3rc1/tests/test_atom_routines.py
--rw-r--r--   0        0        0     1786 2020-02-02 00:00:00.000000 cryojax-0.2.3rc1/tests/test_detector.py
--rw-r--r--   0        0        0     1514 2020-02-02 00:00:00.000000 cryojax-0.2.3rc1/tests/test_ensemble.py
--rw-r--r--   0        0        0     1285 2020-02-02 00:00:00.000000 cryojax-0.2.3rc1/tests/test_fft.py
--rw-r--r--   0        0        0     1572 2020-02-02 00:00:00.000000 cryojax-0.2.3rc1/tests/test_filters_and_masks.py
--rw-r--r--   0        0        0     5952 2020-02-02 00:00:00.000000 cryojax-0.2.3rc1/tests/test_helix.py
--rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 cryojax-0.2.3rc1/tests/test_jit.py
--rw-r--r--   0        0        0      971 2020-02-02 00:00:00.000000 cryojax-0.2.3rc1/tests/test_normalize.py
--rw-r--r--   0        0        0     2927 2020-02-02 00:00:00.000000 cryojax-0.2.3rc1/tests/test_pose_agreement.py
--rw-r--r--   0        0        0     4044 2020-02-02 00:00:00.000000 cryojax-0.2.3rc1/tests/test_potential.py
--rw-r--r--   0        0        0     1233 2020-02-02 00:00:00.000000 cryojax-0.2.3rc1/tests/test_projection_agreement.py
--rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 cryojax-0.2.3rc1/tests/test_shape.py
--rw-r--r--   0        0        0     4450 2020-02-02 00:00:00.000000 cryojax-0.2.3rc1/tests/test_voxels_from_atoms.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cryojax-0.2.3rc1/tests/data/.gitkeep
--rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 cryojax-0.2.3rc1/tests/data/1uao.pdb
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 cryojax-0.2.3rc1/tests/data/3j9g_potential_ps4_4.mrc
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 cryojax-0.2.3rc1/tests/data/3j9g_subunit_potential_ps4_4.mrc
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 cryojax-0.2.3rc1/.gitignore
--rw-r--r--   0        0        0    26526 2020-02-02 00:00:00.000000 cryojax-0.2.3rc1/LICENSE
--rw-r--r--   0        0        0     7066 2020-02-02 00:00:00.000000 cryojax-0.2.3rc1/README.md
--rw-r--r--   0        0        0     1723 2020-02-02 00:00:00.000000 cryojax-0.2.3rc1/pyproject.toml
--rw-r--r--   0        0        0    38731 2020-02-02 00:00:00.000000 cryojax-0.2.3rc1/PKG-INFO
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 cryojax-0.3.0a0/.gitattributes
+-rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 cryojax-0.3.0a0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     2084 2020-02-02 00:00:00.000000 cryojax-0.3.0a0/CONTRIBUTING.md
+-rw-r--r--   0        0        0     2235 2020-02-02 00:00:00.000000 cryojax-0.3.0a0/mkdocs.yml
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 cryojax-0.3.0a0/.github/dependabot.yml
+-rw-r--r--   0        0        0     1110 2020-02-02 00:00:00.000000 cryojax-0.3.0a0/.github/workflows/build_docs.yml
+-rw-r--r--   0        0        0      784 2020-02-02 00:00:00.000000 cryojax-0.3.0a0/.github/workflows/release.yml
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 cryojax-0.3.0a0/.github/workflows/ruff.yml
+-rw-r--r--   0        0        0     1000 2020-02-02 00:00:00.000000 cryojax-0.3.0a0/.github/workflows/testing.yml
+-rw-r--r--   0        0        0     6678 2020-02-02 00:00:00.000000 cryojax-0.3.0a0/docs/index.md
+-rw-r--r--   0        0        0     3108 2020-02-02 00:00:00.000000 cryojax-0.3.0a0/docs/_static/custom_css.css
+-rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 cryojax-0.3.0a0/docs/_static/mathjax.js
+-rw-r--r--   0        0        0     2738 2020-02-02 00:00:00.000000 cryojax-0.3.0a0/docs/api/simulator/scattering_potential.md
+-rw-r--r--   0        0        0  1155917 2020-02-02 00:00:00.000000 cryojax-0.3.0a0/docs/examples/cross-correlation-search.ipynb
+-rw-r--r--   0        0        0   511326 2020-02-02 00:00:00.000000 cryojax-0.3.0a0/docs/examples/read-dataset.ipynb
+-rw-r--r--   0        0        0     7539 2020-02-02 00:00:00.000000 cryojax-0.3.0a0/docs/examples/simulate-helix.ipynb
+-rw-r--r--   0        0        0   269240 2020-02-02 00:00:00.000000 cryojax-0.3.0a0/docs/examples/simulate-image.ipynb
+-rw-r--r--   0        0        0   137942 2020-02-02 00:00:00.000000 cryojax-0.3.0a0/docs/examples/simulate-micrograph.ipynb
+-rw-r--r--   0        0        0    13153 2020-02-02 00:00:00.000000 cryojax-0.3.0a0/docs/examples/test-multiatom.ipynb
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cryojax-0.3.0a0/docs/examples/data/.gitkeep
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 cryojax-0.3.0a0/docs/examples/data/ribosome_4ug0_micrograph.mrc
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 cryojax-0.3.0a0/docs/examples/data/ribosome_4ug0_micrograph.mrcs
+-rw-r--r--   0        0        0     2019 2020-02-02 00:00:00.000000 cryojax-0.3.0a0/docs/examples/data/ribosome_4ug0_particles.star
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 cryojax-0.3.0a0/docs/examples/data/ribosome_4ug0_scattering_potential_from_cistem.mrc
+-rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 cryojax-0.3.0a0/src/cryojax/__init__.py
+-rw-r--r--   0        0        0      901 2020-02-02 00:00:00.000000 cryojax-0.3.0a0/src/cryojax/_errors.py
+-rw-r--r--   0        0        0     1731 2020-02-02 00:00:00.000000 cryojax-0.3.0a0/src/cryojax/_filter_specs.py
+-rw-r--r--   0        0        0     3772 2020-02-02 00:00:00.000000 cryojax-0.3.0a0/src/cryojax/_filtered_transformations.py
+-rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 cryojax-0.3.0a0/src/cryojax/cryojax_version.py
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 cryojax-0.3.0a0/src/cryojax/constants/__init__.py
+-rw-r--r--   0        0        0     1653 2020-02-02 00:00:00.000000 cryojax-0.3.0a0/src/cryojax/constants/_load_atoms.py
+-rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 cryojax-0.3.0a0/src/cryojax/constants/_unit_conversions.py
+-rw-r--r--   0        0        0     8048 2020-02-02 00:00:00.000000 cryojax-0.3.0a0/src/cryojax/constants/element_params.npy
+-rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 cryojax-0.3.0a0/src/cryojax/coordinates/__init__.py
+-rw-r--r--   0        0        0     4457 2020-02-02 00:00:00.000000 cryojax-0.3.0a0/src/cryojax/coordinates/_coordinate_functions.py
+-rw-r--r--   0        0        0     4343 2020-02-02 00:00:00.000000 cryojax-0.3.0a0/src/cryojax/coordinates/_coordinate_wrappers.py
+-rw-r--r--   0        0        0     1110 2020-02-02 00:00:00.000000 cryojax-0.3.0a0/src/cryojax/data/__init__.py
+-rw-r--r--   0        0        0     2861 2020-02-02 00:00:00.000000 cryojax-0.3.0a0/src/cryojax/data/_dataset.py
+-rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 cryojax-0.3.0a0/src/cryojax/data/_particle_stack.py
+-rw-r--r--   0        0        0    18332 2020-02-02 00:00:00.000000 cryojax-0.3.0a0/src/cryojax/data/_relion.py
+-rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 cryojax-0.3.0a0/src/cryojax/data/_io/__init__.py
+-rw-r--r--   0        0        0     1583 2020-02-02 00:00:00.000000 cryojax-0.3.0a0/src/cryojax/data/_io/cif.py
+-rw-r--r--   0        0        0     3056 2020-02-02 00:00:00.000000 cryojax-0.3.0a0/src/cryojax/data/_io/gemmi.py
+-rw-r--r--   0        0        0     1008 2020-02-02 00:00:00.000000 cryojax-0.3.0a0/src/cryojax/data/_io/mdtraj.py
+-rw-r--r--   0        0        0     8248 2020-02-02 00:00:00.000000 cryojax-0.3.0a0/src/cryojax/data/_io/mrc.py
+-rw-r--r--   0        0        0     1860 2020-02-02 00:00:00.000000 cryojax-0.3.0a0/src/cryojax/data/_io/pdb.py
+-rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 cryojax-0.3.0a0/src/cryojax/data/_io/starfile.py
+-rw-r--r--   0        0        0     1005 2020-02-02 00:00:00.000000 cryojax-0.3.0a0/src/cryojax/image/__init__.py
+-rw-r--r--   0        0        0     3500 2020-02-02 00:00:00.000000 cryojax-0.3.0a0/src/cryojax/image/_average.py
+-rw-r--r--   0        0        0     6227 2020-02-02 00:00:00.000000 cryojax-0.3.0a0/src/cryojax/image/_edges.py
+-rw-r--r--   0        0        0     4636 2020-02-02 00:00:00.000000 cryojax-0.3.0a0/src/cryojax/image/_fft.py
+-rw-r--r--   0        0        0     8242 2020-02-02 00:00:00.000000 cryojax-0.3.0a0/src/cryojax/image/_map_coordinates.py
+-rw-r--r--   0        0        0     3664 2020-02-02 00:00:00.000000 cryojax-0.3.0a0/src/cryojax/image/_normalize.py
+-rw-r--r--   0        0        0     3474 2020-02-02 00:00:00.000000 cryojax-0.3.0a0/src/cryojax/image/_rescale_pixel_size.py
+-rw-r--r--   0        0        0     4535 2020-02-02 00:00:00.000000 cryojax-0.3.0a0/src/cryojax/image/_spectrum.py
+-rw-r--r--   0        0        0     1162 2020-02-02 00:00:00.000000 cryojax-0.3.0a0/src/cryojax/image/operators/__init__.py
+-rw-r--r--   0        0        0     7058 2020-02-02 00:00:00.000000 cryojax-0.3.0a0/src/cryojax/image/operators/_filters.py
+-rw-r--r--   0        0        0     6601 2020-02-02 00:00:00.000000 cryojax-0.3.0a0/src/cryojax/image/operators/_fourier_operator.py
+-rw-r--r--   0        0        0     3687 2020-02-02 00:00:00.000000 cryojax-0.3.0a0/src/cryojax/image/operators/_masks.py
+-rw-r--r--   0        0        0     6563 2020-02-02 00:00:00.000000 cryojax-0.3.0a0/src/cryojax/image/operators/_operator.py
+-rw-r--r--   0        0        0     2536 2020-02-02 00:00:00.000000 cryojax-0.3.0a0/src/cryojax/image/operators/_real_operator.py
+-rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 cryojax-0.3.0a0/src/cryojax/inference/__init__.py
+-rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 cryojax-0.3.0a0/src/cryojax/inference/_grid_search/__init__.py
+-rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 cryojax-0.3.0a0/src/cryojax/inference/_grid_search/custom_types.py
+-rw-r--r--   0        0        0     7276 2020-02-02 00:00:00.000000 cryojax-0.3.0a0/src/cryojax/inference/_grid_search/pytree_manipulation.py
+-rw-r--r--   0        0        0     9545 2020-02-02 00:00:00.000000 cryojax-0.3.0a0/src/cryojax/inference/_grid_search/search_loop.py
+-rw-r--r--   0        0        0    10168 2020-02-02 00:00:00.000000 cryojax-0.3.0a0/src/cryojax/inference/_grid_search/search_method.py
+-rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 cryojax-0.3.0a0/src/cryojax/inference/_transforms/__init__.py
+-rw-r--r--   0        0        0     4084 2020-02-02 00:00:00.000000 cryojax-0.3.0a0/src/cryojax/inference/_transforms/lie_group_transforms.py
+-rw-r--r--   0        0        0     5077 2020-02-02 00:00:00.000000 cryojax-0.3.0a0/src/cryojax/inference/_transforms/transforms.py
+-rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 cryojax-0.3.0a0/src/cryojax/inference/distributions/__init__.py
+-rw-r--r--   0        0        0     1614 2020-02-02 00:00:00.000000 cryojax-0.3.0a0/src/cryojax/inference/distributions/_base_distribution.py
+-rw-r--r--   0        0        0     6537 2020-02-02 00:00:00.000000 cryojax-0.3.0a0/src/cryojax/inference/distributions/_gaussian_distributions.py
+-rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 cryojax-0.3.0a0/src/cryojax/rotations/__init__.py
+-rw-r--r--   0        0        0    16051 2020-02-02 00:00:00.000000 cryojax-0.3.0a0/src/cryojax/rotations/_lie_group.py
+-rw-r--r--   0        0        0     1934 2020-02-02 00:00:00.000000 cryojax-0.3.0a0/src/cryojax/rotations/_rotation.py
+-rw-r--r--   0        0        0     2502 2020-02-02 00:00:00.000000 cryojax-0.3.0a0/src/cryojax/rotations/_utils.py
+-rw-r--r--   0        0        0     3301 2020-02-02 00:00:00.000000 cryojax-0.3.0a0/src/cryojax/simulator/__init__.py
+-rw-r--r--   0        0        0     7998 2020-02-02 00:00:00.000000 cryojax-0.3.0a0/src/cryojax/simulator/_detector.py
+-rw-r--r--   0        0        0    13585 2020-02-02 00:00:00.000000 cryojax-0.3.0a0/src/cryojax/simulator/_imaging_pipeline.py
+-rw-r--r--   0        0        0     6379 2020-02-02 00:00:00.000000 cryojax-0.3.0a0/src/cryojax/simulator/_instrument_config.py
+-rw-r--r--   0        0        0     9790 2020-02-02 00:00:00.000000 cryojax-0.3.0a0/src/cryojax/simulator/_pose.py
+-rw-r--r--   0        0        0     3025 2020-02-02 00:00:00.000000 cryojax-0.3.0a0/src/cryojax/simulator/_solvent.py
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 cryojax-0.3.0a0/src/cryojax/simulator/_assembly/__init__.py
+-rw-r--r--   0        0        0     4254 2020-02-02 00:00:00.000000 cryojax-0.3.0a0/src/cryojax/simulator/_assembly/assembly.py
+-rw-r--r--   0        0        0    10344 2020-02-02 00:00:00.000000 cryojax-0.3.0a0/src/cryojax/simulator/_assembly/helix.py
+-rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 cryojax-0.3.0a0/src/cryojax/simulator/_potential_integrator/__init__.py
+-rw-r--r--   0        0        0     2695 2020-02-02 00:00:00.000000 cryojax-0.3.0a0/src/cryojax/simulator/_potential_integrator/base_potential_integrator.py
+-rw-r--r--   0        0        0     8274 2020-02-02 00:00:00.000000 cryojax-0.3.0a0/src/cryojax/simulator/_potential_integrator/fourier_voxel_extract.py
+-rw-r--r--   0        0        0     4874 2020-02-02 00:00:00.000000 cryojax-0.3.0a0/src/cryojax/simulator/_potential_integrator/gaussian_mixture.py
+-rw-r--r--   0        0        0     4085 2020-02-02 00:00:00.000000 cryojax-0.3.0a0/src/cryojax/simulator/_potential_integrator/nufft_project.py
+-rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 cryojax-0.3.0a0/src/cryojax/simulator/_potential_representation/__init__.py
+-rw-r--r--   0        0        0     1201 2020-02-02 00:00:00.000000 cryojax-0.3.0a0/src/cryojax/simulator/_potential_representation/atom_potential.py
+-rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 cryojax-0.3.0a0/src/cryojax/simulator/_potential_representation/base_potential.py
+-rw-r--r--   0        0        0    23744 2020-02-02 00:00:00.000000 cryojax-0.3.0a0/src/cryojax/simulator/_potential_representation/voxel_potential.py
+-rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 cryojax-0.3.0a0/src/cryojax/simulator/_scattering_theory/__init__.py
+-rw-r--r--   0        0        0      955 2020-02-02 00:00:00.000000 cryojax-0.3.0a0/src/cryojax/simulator/_scattering_theory/base_scattering_theory.py
+-rw-r--r--   0        0        0    10833 2020-02-02 00:00:00.000000 cryojax-0.3.0a0/src/cryojax/simulator/_scattering_theory/linear_scattering_theory.py
+-rw-r--r--   0        0        0      531 2020-02-02 00:00:00.000000 cryojax-0.3.0a0/src/cryojax/simulator/_structural_ensemble/__init__.py
+-rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 cryojax-0.3.0a0/src/cryojax/simulator/_structural_ensemble/base_conformation.py
+-rw-r--r--   0        0        0     2114 2020-02-02 00:00:00.000000 cryojax-0.3.0a0/src/cryojax/simulator/_structural_ensemble/base_ensemble.py
+-rw-r--r--   0        0        0     2123 2020-02-02 00:00:00.000000 cryojax-0.3.0a0/src/cryojax/simulator/_structural_ensemble/discrete_ensemble.py
+-rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 cryojax-0.3.0a0/src/cryojax/simulator/_structural_ensemble/ensemble_batcher.py
+-rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 cryojax-0.3.0a0/src/cryojax/simulator/_transfer_theory/__init__.py
+-rw-r--r--   0        0        0     1730 2020-02-02 00:00:00.000000 cryojax-0.3.0a0/src/cryojax/simulator/_transfer_theory/base_transfer_theory.py
+-rw-r--r--   0        0        0     2224 2020-02-02 00:00:00.000000 cryojax-0.3.0a0/src/cryojax/simulator/_transfer_theory/common_functions.py
+-rw-r--r--   0        0        0     6725 2020-02-02 00:00:00.000000 cryojax-0.3.0a0/src/cryojax/simulator/_transfer_theory/contrast_transfer_theory.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cryojax-0.3.0a0/tests/__init__.py
+-rw-r--r--   0        0        0     3918 2020-02-02 00:00:00.000000 cryojax-0.3.0a0/tests/conftest.py
+-rw-r--r--   0        0        0     5957 2020-02-02 00:00:00.000000 cryojax-0.3.0a0/tests/test_agree_with_cistem.py
+-rw-r--r--   0        0        0     3678 2020-02-02 00:00:00.000000 cryojax-0.3.0a0/tests/test_atom_routines.py
+-rw-r--r--   0        0        0     1769 2020-02-02 00:00:00.000000 cryojax-0.3.0a0/tests/test_detector.py
+-rw-r--r--   0        0        0     1714 2020-02-02 00:00:00.000000 cryojax-0.3.0a0/tests/test_ensemble.py
+-rw-r--r--   0        0        0     1271 2020-02-02 00:00:00.000000 cryojax-0.3.0a0/tests/test_fft.py
+-rw-r--r--   0        0        0     3283 2020-02-02 00:00:00.000000 cryojax-0.3.0a0/tests/test_grid_search.py
+-rw-r--r--   0        0        0     7512 2020-02-02 00:00:00.000000 cryojax-0.3.0a0/tests/test_helix.py
+-rw-r--r--   0        0        0      789 2020-02-02 00:00:00.000000 cryojax-0.3.0a0/tests/test_normalize.py
+-rw-r--r--   0        0        0     2985 2020-02-02 00:00:00.000000 cryojax-0.3.0a0/tests/test_pose_agreement.py
+-rw-r--r--   0        0        0     1455 2020-02-02 00:00:00.000000 cryojax-0.3.0a0/tests/test_potential.py
+-rw-r--r--   0        0        0     2406 2020-02-02 00:00:00.000000 cryojax-0.3.0a0/tests/test_shape.py
+-rw-r--r--   0        0        0     4452 2020-02-02 00:00:00.000000 cryojax-0.3.0a0/tests/test_voxels_from_atoms.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cryojax-0.3.0a0/tests/data/.gitkeep
+-rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 cryojax-0.3.0a0/tests/data/1uao.pdb
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 cryojax-0.3.0a0/tests/data/3j9g_potential_ps4_4.mrc
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 cryojax-0.3.0a0/tests/data/3j9g_subunit_potential_ps4_4.mrc
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 cryojax-0.3.0a0/.gitignore
+-rw-r--r--   0        0        0    26526 2020-02-02 00:00:00.000000 cryojax-0.3.0a0/LICENSE
+-rw-r--r--   0        0        0     7681 2020-02-02 00:00:00.000000 cryojax-0.3.0a0/README.md
+-rw-r--r--   0        0        0     1783 2020-02-02 00:00:00.000000 cryojax-0.3.0a0/pyproject.toml
+-rw-r--r--   0        0        0    39365 2020-02-02 00:00:00.000000 cryojax-0.3.0a0/PKG-INFO
```

### Comparing `cryojax-0.2.3rc1/.pre-commit-config.yaml` & `cryojax-0.3.0a0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `cryojax-0.2.3rc1/CONTRIBUTING.md` & `cryojax-0.3.0a0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `cryojax-0.2.3rc1/mkdocs.yml` & `cryojax-0.3.0a0/mkdocs.yml`

 * *Files 4% similar despite different names*

```diff
@@ -60,9 +60,10 @@
     - 'index.md'
     - Examples:
         - Introductory:
             - Simulate an image: 'examples/simulate-image.ipynb'
             - Read a particle stack: 'examples/read-dataset.ipynb'
         - Intermediate:
             - Simulate a batch of images: 'examples/simulate-micrograph.ipynb'
+            - Run a cross-correlation search: 'examples/cross-correlation-search.ipynb'
     - Simulator API:
         - 'api/simulator/scattering_potential.md'
```

### Comparing `cryojax-0.2.3rc1/.github/workflows/build_docs.yml` & `cryojax-0.3.0a0/.github/workflows/build_docs.yml`

 * *Files identical despite different names*

### Comparing `cryojax-0.2.3rc1/.github/workflows/release.yml` & `cryojax-0.3.0a0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `cryojax-0.2.3rc1/.github/workflows/testing.yml` & `cryojax-0.3.0a0/.github/workflows/testing.yml`

 * *Files identical despite different names*

### Comparing `cryojax-0.2.3rc1/docs/index.md` & `cryojax-0.3.0a0/docs/index.md`

 * *Files 13% similar despite different names*

```diff
@@ -38,74 +38,70 @@
 
 The [`jax-finufft`](https://github.com/dfm/jax-finufft) package is an optional dependency used for non-uniform fast fourier transforms. These are included as an option for computing image projections of real-space voxel-based scattering potential representations. In this case, we recommend first following the `jax_finufft` installation instructions and then installing `cryojax`.
 
 ## Quick example
 
 The following is a basic workflow to simulate an image.
 
-First, instantiate the scattering potential representation and its respective method for computing image projections.
+First, instantiate the spatial potential energy distribution representation and its respective method for computing image projections.
 
 ```python
 import jax
 import jax.numpy as jnp
-import cryojax.simulator as cs
-from cryojax.io import read_array_with_spacing_from_mrc
+import cryojax.simulator as cxs
+from cryojax.data import read_array_with_spacing_from_mrc
 
-# Instantiate the scattering potential.
+# Instantiate the scattering potential
 filename = "example_scattering_potential.mrc"
 real_voxel_grid, voxel_size = read_array_with_spacing_from_mrc(filename)
-potential = cs.FourierVoxelGridPotential.from_real_voxel_grid(real_voxel_grid, voxel_size)
-# ... now instantiate fourier slice extraction
-integrator = cs.FourierSliceExtract(interpolation_order=1)
-```
-
-Here, the 3D scattering potential array is read from `filename`. Then, the abstraction of the scattering potential is then loaded in fourier-space into a `FourierVoxelGridPotential`, and the fourier-slice projection theorem is initialized with `FourierSliceExtract`. The scattering potential can be generated with an external program, such as the [cisTEM](https://github.com/timothygrant80/cisTEM) simulate tool.
-
-We can now instantiate the representation of a biological specimen, which also includes a pose.
-
-```python
-# First instantiate the pose. Angles are given in degrees
-pose = cs.EulerAnglePose(
+potential = cxs.FourierVoxelGridPotential.from_real_voxel_grid(real_voxel_grid, voxel_size)
+# ... now, instantiate the pose. Angles are given in degrees
+pose = cxs.EulerAnglePose(
     offset_x_in_angstroms=5.0,
     offset_y_in_angstroms=-3.0,
     view_phi=20.0,
     view_theta=80.0,
     view_psi=-10.0,
 )
-# ... now, build the biological specimen
-specimen = cs.Specimen(potential, integrator, pose)
+# ... now, build the ensemble. In this case, the ensemble is just a single structure
+structural_ensemble = cxs.SingleStructureEnsemble(potential, pose)
 ```
 
-Next, build the model for the electron microscope. Here, we simply include a model for the CTF in the weak-phase approximation (linear image formation theory).
+Here, the 3D scattering potential array is read from `filename`. Then, the abstraction of the scattering potential is then loaded in fourier-space into a `FourierVoxelGridPotential`. The scattering potential can be generated with an external program, such as the [cisTEM](https://github.com/timothygrant80/cisTEM) simulate tool. Then, the representation of a biological specimen is instantiated, which also includes a pose and conformational heterogeneity. Here, the `SingleStructureEnsemble` class takes a pose but has no heterogeneity.
+
+Next, build the *scattering theory*. The simplest `scattering_theory` is the `LinearScatteringTheory`. This represents the usual image formation pipeline in cryo-EM, which forms images by computing projections of the potential and convolving the result with a contrast transfer function.
 
 ```python
 from cryojax.image import operators as op
 
-# First, initialize the CTF and its optics model
-ctf = cs.CTF(
-    defocus_u_in_angstroms=10000.0,
-    defocus_v_in_angstroms=9800.0,
+# Initialize the scattering theory. First, instantiate fourier slice extraction
+potential_integrator = cxs.FourierSliceExtraction(interpolation_order=1)
+# ... next, the contrast transfer theory
+ctf = cxs.ContrastTransferFunction(
+    defocus_in_angstroms=9800.0,
+    astigmatism_in_angstroms=200.0,
     astigmatism_angle=10.0,
-    amplitude_contrast_ratio=0.1)
-optics = cs.WeakPhaseOptics(ctf, envelope=op.FourierGaussian(b_factor=5.0))  # b_factor is given in Angstroms^2
-# ... these are stored in the Instrument
-voltage_in_kilovolts = 300.0
-instrument = cs.Instrument(voltage_in_kilovolts, optics)
+    amplitude_contrast_ratio=0.1
+)
+transfer_theory = cxs.ContrastTransferTheory(ctf, envelope=op.FourierGaussian(b_factor=5.0))
+# ... now for the scattering theory
+scattering_theory = cxs.LinearScatteringTheory(structural_ensemble, potential_integrator, transfer_theory)
 ```
 
-The `CTF` has all parameters used in CTFFIND4, which take their default values if not
-explicitly configured here. Finally, we can instantiate the `ImagePipeline` and simulate an image.
+The `ContrastTransferFunction` has parameters used in CTFFIND4, which take their default values if not
+explicitly configured here. Finally, we can instantiate the `imaging_pipeline`--the highest level of imaging abstraction in `cryojax`--and simulate an image. Here, we choose a `ContrastImagingPipeline`, which simulates image contrast from a linear scattering theory.
 
 ```python
-# Instantiate the image configuration
-config = cs.ImageConfig(shape=(320, 320), pixel_size=voxel_size)
-# Build the image formation model
-pipeline = cs.ImagePipeline(config, specimen, instrument)
-# ... simulate an image and return a normalized image in real-space
-image = pipeline.render(get_real=True, normalize=True)
+# Finally, build the image formation model
+# ... first instantiate the instrument configuration
+instrument_config = cxs.InstrumentConfig(shape=(320, 320), pixel_size=voxel_size, voltage_in_kilovolts=300.0)
+# ... now the imaging pipeline
+imaging_pipeline = cxs.ContrastImagingPipeline(instrument_config, scattering_theory)
+# ... finally, simulate an image and return in real-space!
+image_without_noise = imaging_pipeline.render(get_real=True)
 ```
 
 ## Next steps
 
 There are many modeling features in `cryojax` to learn about. To learn more, see the Examples section of the documentation.
 
 ## Acknowledgements
```

### Comparing `cryojax-0.2.3rc1/docs/_static/custom_css.css` & `cryojax-0.3.0a0/docs/_static/custom_css.css`

 * *Files identical despite different names*

### Comparing `cryojax-0.2.3rc1/docs/api/simulator/scattering_potential.md` & `cryojax-0.3.0a0/docs/api/simulator/scattering_potential.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Scattering potential representations
 
-`cryojax` provides different options for how to represent scattering potentials in cryo-EM.
+`cryojax` provides different options for how to represent spatial potential energy distributions in cryo-EM.
 
-???+ abstract "`cryojax.simulator.AbstractScatteringPotential`"
-    ::: cryojax.simulator.AbstractScatteringPotential
+???+ abstract "`cryojax.simulator.AbstractPotentialRepresentation`"
+    ::: cryojax.simulator.AbstractPotentialRepresentation
         options:
             members:
                 - rotate_to_pose
 
 ## Voxel-based scattering potentials
 
 ???+ abstract "`cryojax.simulator.AbstractVoxelPotential`"
```

### Comparing `cryojax-0.2.3rc1/docs/examples/read-dataset.ipynb` & `cryojax-0.3.0a0/docs/examples/read-dataset.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9972968431637163%*

 * *Differences: {"'cells'": "{4: {'source': {insert: [(8, '    stores a `cryojax` models for the contrast transfer "*

 * *            'function (the `ContrastTransferFunction` class) and the pose (the `EulerAnglePose` '*

 * *            "class).\\n')], delete: [8]}}, 5: {'outputs': {0: {'text': {insert: [(2, '  "*

 * *            "instrument_config=InstrumentConfig(\\n'), (5, '    voltage_in_kilovolts=f32[],\\n'), "*

 * *            '(6, \'    electrons_per_angstrom_squared=f32[],\\n\'), (8, "    '*

 * *            'pad_mode=\'constant\'\\n"), (18 […]*

```diff
@@ -59,15 +59,15 @@
                 "\n",
                 "!!! info \"What is a `RelionDataset`?\"\n",
                 "\n",
                 "    CryoJAX implements an abstraction an a dataset in RELION, called a `RelionDataset`. This object takes in a\n",
                 "    RELION STAR file for a particle stack. Upon accessing an image in the particle stack, a `RelionParticleStack`\n",
                 "    is returned. Specifically, the `RelionParticleStack` stores the image(s) in the image stack, as well as the metadata\n",
                 "    in the STAR file. The metadata is used to instantiate compatible `cryojax` objects. For example, the `RelionParticleStack`\n",
-                "    stores a `cryojax` models for the contrast transfer function (the `CTF` class) and the pose (the `EulerAnglePose` class).\n",
+                "    stores a `cryojax` models for the contrast transfer function (the `ContrastTransferFunction` class) and the pose (the `EulerAnglePose` class).\n",
                 "\n",
                 "    More generally, a `RelionDataset` is an `AbstractDataset`, which is complemented by the abstraction of a particle stack: the `AbstractParticleStack`.\n",
                 "    These abstract interfaces are part of the `cryojax` public API!  "
             ]
         },
         {
             "cell_type": "code",
@@ -76,38 +76,35 @@
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "RelionParticleStack(\n",
                         "  image_stack=f32[100,100],\n",
-                        "  config=ImageConfig(\n",
+                        "  instrument_config=InstrumentConfig(\n",
                         "    shape=(100, 100),\n",
                         "    pixel_size=f32[],\n",
+                        "    voltage_in_kilovolts=f32[],\n",
+                        "    electrons_per_angstrom_squared=f32[],\n",
                         "    padded_shape=(100, 100),\n",
-                        "    pad_mode='constant',\n",
-                        "    rescale_method='bicubic',\n",
-                        "    wrapped_frequency_grid=FrequencyGrid(array=f32[100,51,2]),\n",
-                        "    wrapped_padded_frequency_grid=FrequencyGrid(array=f32[100,51,2]),\n",
-                        "    wrapped_coordinate_grid=CoordinateGrid(array=f32[100,100,2]),\n",
-                        "    wrapped_padded_coordinate_grid=CoordinateGrid(array=f32[100,100,2])\n",
+                        "    pad_mode='constant'\n",
                         "  ),\n",
                         "  pose=EulerAnglePose(\n",
                         "    offset_x_in_angstroms=f32[],\n",
                         "    offset_y_in_angstroms=f32[],\n",
                         "    offset_z_in_angstroms=f32[],\n",
                         "    view_phi=f32[],\n",
                         "    view_theta=f32[],\n",
                         "    view_psi=f32[]\n",
                         "  ),\n",
-                        "  ctf=CTF(\n",
-                        "    defocus_u_in_angstroms=f32[],\n",
-                        "    defocus_v_in_angstroms=f32[],\n",
+                        "  ctf=ContrastTransferFunction(\n",
+                        "    defocus_in_angstroms=f32[],\n",
+                        "    astigmatism_in_angstroms=f32[],\n",
                         "    astigmatism_angle=f32[],\n",
-                        "    voltage_in_kilovolts=f32[],\n",
+                        "    voltage_in_kilovolts=300.0,\n",
                         "    spherical_aberration_in_mm=f32[],\n",
                         "    amplitude_contrast_ratio=f32[],\n",
                         "    phase_shift=f32[]\n",
                         "  )\n",
                         ")\n"
                     ]
                 }
@@ -197,31 +194,31 @@
                 "print(relion_particles.image_stack.shape)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "Now, we see that the `image_stack` attribute has a leading dimension for each image. We can also inspect the metadata read from the STAR file by printing the `CTF`."
+                "Now, we see that the `image_stack` attribute has a leading dimension for each image. We can also inspect the metadata read from the STAR file by printing the `ContrastTransferFunction`."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 7,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "CTF(\n",
-                        "  defocus_u_in_angstroms=Array([10050.97, 10050.97, 10050.97], dtype=float32),\n",
-                        "  defocus_v_in_angstroms=Array([9999.999, 9999.999, 9999.999], dtype=float32),\n",
+                        "ContrastTransferFunction(\n",
+                        "  defocus_in_angstroms=Array([10050.97, 10050.97, 10050.97], dtype=float32),\n",
+                        "  astigmatism_in_angstroms=Array([-50.970703, -50.970703, -50.970703], dtype=float32),\n",
                         "  astigmatism_angle=Array([-54.58706, -54.58706, -54.58706], dtype=float32),\n",
-                        "  voltage_in_kilovolts=Array(300., dtype=float32),\n",
+                        "  voltage_in_kilovolts=300.0,\n",
                         "  spherical_aberration_in_mm=Array(2.7, dtype=float32),\n",
                         "  amplitude_contrast_ratio=Array(0.1, dtype=float32),\n",
                         "  phase_shift=Array([0., 0., 0.], dtype=float32)\n",
                         ")\n"
                     ]
                 }
             ],
@@ -230,15 +227,15 @@
                 "eqx.tree_pprint(relion_particles.ctf, short_arrays=False)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "Notice that not all attributes of the `CTF` have a leading dimension. For those familiar with RELION STAR format, only the `CTF` parameters stored on a per-particle basis have a leading dimension! Parameters stored in the opticsGroup do not have a leading dimension."
+                "Notice that not all attributes of the `ContrastTransferFunction` have a leading dimension. For those familiar with RELION STAR format, only the `ContrastTransferFunction` parameters stored on a per-particle basis have a leading dimension! Parameters stored in the opticsGroup do not have a leading dimension."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 8,
             "metadata": {},
             "outputs": [
@@ -290,22 +287,20 @@
                 "\n",
                 "\n",
                 "# Get the particle\n",
                 "relion_particle = dataset[0]\n",
                 "# ... and the image in fourier space\n",
                 "fourier_image = rfftn(relion_particle.image_stack)\n",
                 "# ... and the cartesian coordinate system\n",
-                "pixel_size = relion_particle.config.pixel_size\n",
+                "pixel_size = relion_particle.instrument_config.pixel_size\n",
                 "frequency_grid_in_angstroms = (\n",
-                "    relion_particle.config.wrapped_frequency_grid_in_angstroms.get()\n",
+                "    relion_particle.instrument_config.wrapped_frequency_grid_in_angstroms.get()\n",
                 ")\n",
                 "# ... now, compute a radial coordinate system\n",
-                "radial_frequency_grid_in_angstroms = jnp.linalg.norm(\n",
-                "    frequency_grid_in_angstroms, axis=-1\n",
-                ")\n",
+                "radial_frequency_grid_in_angstroms = jnp.linalg.norm(frequency_grid_in_angstroms, axis=-1)\n",
                 "# ... plot the image in fourier space and the radial frequency grid\n",
                 "fig, axes = plt.subplots(figsize=(5, 4), ncols=2)\n",
                 "plot_image(\n",
                 "    jnp.log(jnp.abs(jnp.fft.fftshift(fourier_image, axes=(0,))) ** 2),\n",
                 "    fig,\n",
                 "    axes[0],\n",
                 "    label=\"Image log power spectrum\",\n",
@@ -357,15 +352,15 @@
             "source": [
                 "import math\n",
                 "\n",
                 "from cryojax.image import powerspectrum\n",
                 "\n",
                 "\n",
                 "fig, ax = plt.subplots(figsize=(4, 4))\n",
-                "N_pixels = math.prod(relion_particle.config.shape)\n",
+                "N_pixels = math.prod(relion_particle.instrument_config.shape)\n",
                 "spectrum, wavenumbers = powerspectrum(\n",
                 "    fourier_image,\n",
                 "    radial_frequency_grid_in_angstroms,\n",
                 "    pixel_size,\n",
                 "    k_max=1 / (2 * pixel_size),\n",
                 ")\n",
                 "ax.plot(wavenumbers, spectrum / N_pixels, color=\"k\")\n",
```

### Comparing `cryojax-0.2.3rc1/docs/examples/simulate-helix.ipynb` & `cryojax-0.3.0a0/docs/examples/simulate-helix.ipynb`

 * *Files identical despite different names*

### Comparing `cryojax-0.2.3rc1/docs/examples/simulate-micrograph.ipynb` & `cryojax-0.3.0a0/docs/examples/simulate-micrograph.ipynb`

 * *Files 27% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9924334641815111%*

 * *Differences: {"'cells'": '{0: {\'source\': {insert: [(2, "The goal of this tutorial is to learn how to vmap in '*

 * *            "`cryojax`'s recommended pattern. This uses the lightweight wrappers around `equinox` "*

 * *            'in `cryojax`.")], delete: [2]}}, 3: {\'source\': {insert: [(1, \'from jaxtyping '*

 * *            "import install_import_hook\\n'), (2, '\\n'), (3, '\\n'), (4, 'with "*

 * *            'install_import_hook("cryojax", "typeguard.typechecked"):\\n\'), (5, \'    import '*

 * *            "cryojax.simulator as cxs\\ […]*

```diff
@@ -2,15 +2,15 @@
     "cells": [
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "In this tutorial, we will simulate a naive model of a micrograph. In particular, we will simulate a batch of images of the same particle at random poses, then sum over them.\n",
                 "\n",
-                "The goal of this tutorial is to learn how to vmap in `cryojax`'s recommended pattern. Namely, we will demonstrate this pattern using utilities in `cryojax.core`. These utilities are lightweight wrappers around `equinox`."
+                "The goal of this tutorial is to learn how to vmap in `cryojax`'s recommended pattern. This uses the lightweight wrappers around `equinox` in `cryojax`."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 1,
             "metadata": {},
             "outputs": [],
@@ -45,17 +45,21 @@
         {
             "cell_type": "code",
             "execution_count": 3,
             "metadata": {},
             "outputs": [],
             "source": [
                 "# CryoJAX imports\n",
-                "import cryojax.simulator as cs\n",
-                "from cryojax.io import read_array_with_spacing_from_mrc\n",
-                "from cryojax.rotations import SO3"
+                "from jaxtyping import install_import_hook\n",
+                "\n",
+                "\n",
+                "with install_import_hook(\"cryojax\", \"typeguard.typechecked\"):\n",
+                "    import cryojax.simulator as cxs\n",
+                "    from cryojax.data import read_array_with_spacing_from_mrc\n",
+                "    from cryojax.rotations import SO3"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "First, we will build the image formation modeling components that we do not want to vmap over."
@@ -66,41 +70,41 @@
             "execution_count": 4,
             "metadata": {},
             "outputs": [],
             "source": [
                 "# First, load the scattering potential and projection method\n",
                 "filename = \"./data/ribosome_4ug0_scattering_potential_from_cistem.mrc\"\n",
                 "real_voxel_grid, voxel_size = read_array_with_spacing_from_mrc(filename)\n",
-                "potential = cs.FourierVoxelGridPotential.from_real_voxel_grid(\n",
+                "potential = cxs.FourierVoxelGridPotential.from_real_voxel_grid(\n",
                 "    real_voxel_grid, voxel_size, pad_scale=2\n",
                 ")\n",
-                "integrator = cs.FourierSliceExtract(interpolation_order=1)\n",
-                "\n",
-                "# ... and build the instrument\n",
-                "voltage_in_kilovolts = 300.0\n",
-                "optics = cs.WeakPhaseOptics(\n",
-                "    ctf=cs.CTF(\n",
-                "        defocus_u_in_angstroms=10000.0,\n",
-                "        defocus_v_in_angstroms=10000.0,\n",
+                "# ... now the projection method\n",
+                "potential_integrator = cxs.FourierSliceExtraction(interpolation_order=1)\n",
+                "# ... and the contrast transfer theory\n",
+                "transfer_theory = cxs.ContrastTransferTheory(\n",
+                "    ctf=cxs.ContrastTransferFunction(\n",
+                "        defocus_in_angstroms=10000.0,\n",
+                "        astigmatism_in_angstroms=0.0,\n",
                 "    )\n",
                 ")\n",
-                "instrument = cs.Instrument(voltage_in_kilovolts, optics=optics)\n",
-                "\n",
-                "# ... and finally the config\n",
+                "# ... finally, the instrument_config\n",
                 "shape = (400, 600)\n",
                 "pixel_size = potential.voxel_size  # Angstroms\n",
-                "image_size = np.asarray(shape) * pixel_size\n",
-                "config = cs.ImageConfig(shape, pixel_size, pad_scale=1.1)"
+                "voltage_in_kilovolts = 300.0\n",
+                "instrument_config = cxs.InstrumentConfig(\n",
+                "    shape, pixel_size, voltage_in_kilovolts, pad_scale=1.1\n",
+                ")\n",
+                "image_size = np.asarray(shape) * pixel_size"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "Now we will construct an `ImagePipeline` by batching over a set of random number generator keys."
+                "Now we will construct a `ContrastImagingPipeline` by batching over a set of random number generator keys."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 5,
             "metadata": {},
             "outputs": [],
@@ -109,118 +113,123 @@
                 "\n",
                 "import equinox as eqx\n",
                 "import equinox.internal as eqxi\n",
                 "from jaxtyping import PRNGKeyArray, PyTree\n",
                 "\n",
                 "\n",
                 "@partial(eqx.filter_vmap, in_axes=(0, None), out_axes=eqxi.if_mapped(axis=0))\n",
-                "def make_pipeline(key: PRNGKeyArray, no_vmap: tuple[PyTree, ...]) -> cs.ImagePipeline:\n",
-                "    config, potential, integrator, instrument = no_vmap\n",
+                "def make_imaging_pipeline(\n",
+                "    key: PRNGKeyArray, no_vmap: tuple[PyTree, ...]\n",
+                ") -> cxs.ContrastImagingPipeline:\n",
+                "    config, potential, potential_integrator = no_vmap\n",
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
                 "    # ... build the pose\n",
-                "    pose = cs.QuaternionPose.from_rotation_and_translation(\n",
-                "        rotation, offset_in_angstroms\n",
+                "    pose = cxs.QuaternionPose.from_rotation_and_translation(rotation, offset_in_angstroms)\n",
+                "    # ... build the ensemble\n",
+                "    structural_ensemble = cxs.SingleStructureEnsemble(potential, pose)\n",
+                "    # ... and finally the scattering theory and return\n",
+                "    theory = cxs.LinearScatteringTheory(\n",
+                "        structural_ensemble, potential_integrator, transfer_theory\n",
                 "    )\n",
-                "    # ... build the Specimen and ImagePipeline as usual and return\n",
-                "    specimen = cs.Specimen(potential, integrator, pose)\n",
-                "    return cs.ImagePipeline(config, specimen, instrument)"
+                "    return cxs.ContrastImagingPipeline(config, theory)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "!!! info \"What's with the `out_axes=eqxi.if_mapped(axis=0)`?\"\n",
                 "    \n",
                 "    When we create a pytree with `eqx.filter_vmap` (or `jax.vmap`), `out_axes` should have the same structure as the output pytree. If `out_axes` is set to `None` at a particular leaf, this\n",
                 "    says that we do not want to broadcast that leaf (of course, this only works for unmapped leaves). By default `jax.vmap` sets `out_axes=0`, so all unmapped leaves get broadcasted. `equinox` allows us to pass `out_axes=eqxi.if_mapped(axes=0)`, which specifies *not* to broadcast pytree leaves unless the leaves are directly mapped.\n",
                 "\n",
-                "    When building an `ImagePipeline`, it is very important that we do not broadcast arbitrary leaves! For example, an `ImageConfig` stores the coordinate systems for our image. Without the `out_axes=eqxi.if_mapped(axes=0)` specification, the `make_pipeline` would output an `ImagePipeline.config` whose coordinate systems have a batch dimension. This takes up unecessary memory."
+                "    When building a `ContrastImagingPipeline`, it is very important that we do not broadcast arbitrary leaves! For example, an `InstrumentConfig` stores the coordinate systems for our image. Without the `out_axes=eqxi.if_mapped(axes=0)` specification, the `make_imaging_pipeline` would output an `ContrastImagingPipeline.instrument_config` whose coordinate systems have a batch dimension. This takes up unecessary memory."
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
-                "# ... instantiate the pipeline\n",
-                "pipeline = make_pipeline(keys, (config, potential, integrator, instrument))"
+                "# ... instantiate the instrument_pipeline\n",
+                "imaging_pipeline = make_imaging_pipeline(\n",
+                "    keys, (instrument_config, potential, potential_integrator)\n",
+                ")"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "This may be a little odd at first. We have contructed a pipeline, where if we were to directly call its `render` method, it would not work. Think of it this way: because we created our `pipeline`s with a `vmap`, functions can now only be called after crossing `vmap` boundaries. There is very good reason for this! To learn more, read the section of the equinox documentation on [model ensembling](https://docs.kidger.site/equinox/tricks/#ensembling).\n",
+                "This may be a little odd at first. We have contructed an `imaging_pipeline`, where if we were to directly call its `render` method, it would not work. Think of it this way: because we created our `imaging_pipeline`s with a `vmap`, functions can now only be called after crossing `vmap` boundaries. There is very good reason for this! To learn more, read the section of the equinox documentation on [model ensembling](https://docs.kidger.site/equinox/tricks/#ensembling).\n",
                 "\n",
-                "Now that we have an `ImagePipeline` with a batched set of poses, we need some way of telling our `vmap` exactly what pytree leaves have batch dimensions. One way `equinox` does this is by using pointers to particular pytree leaves to create what is called a `filter_spec`."
+                "Now that we have a `ContrastImagingPipeline` with a batched set of poses, we need some way of telling our `vmap` exactly what pytree leaves have batch dimensions. One way `equinox` does this is by using pointers to particular pytree leaves to create what is called a `filter_spec`."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 7,
             "metadata": {},
             "outputs": [],
             "source": [
-                "import cryojax.core as cjc\n",
+                "import cryojax as cx\n",
                 "\n",
                 "\n",
                 "# ... specify which leaves we would like to vmap over\n",
-                "where = lambda pipeline: pipeline.specimen.pose\n",
+                "where = lambda p: p.scattering_theory.structural_ensemble.pose\n",
                 "# ... use a cryojax wrapper to return a filter_spec\n",
-                "filter_spec = cjc.get_filter_spec(pipeline, where)"
+                "filter_spec = cx.get_filter_spec(imaging_pipeline, where)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "Here, `filter_spec` is a pytree of booleans of the same structure as `pipeline`. The values are `True` at leaves that we do want to `vmap` over and `False` where we don't. Filtered transformations are a cornerstone to `equinox` and it is highly recommended to learn about them. See [here](https://docs.kidger.site/equinox/examples/frozen_layer/) in the equinox documentation for reading.\n",
+                "Here, `filter_spec` is a pytree of booleans of the same structure as `imaging_pipeline`. The values are `True` at leaves that we do want to `vmap` over and `False` where we don't. Filtered transformations are a cornerstone to `equinox` and it is highly recommended to learn about them. See [here](https://docs.kidger.site/equinox/examples/frozen_layer/) in the equinox documentation for reading.\n",
                 "\n",
-                "Above we have used a `cryojax` utility routine for creating a `filter_spec`, called `cryojax.core.get_filter_spec`. Next, we will finally define functions to batch and sum over images! To do this, we will again use a `cryojax` wrapper to `equinox` called `filter_vmap_with_spec`. This batches over a pytree, only at leaves specified by `filter_spec`. "
+                "Above we have used a `cryojax` utility routine for creating a `filter_spec`, called `cryojax.get_filter_spec`. Next, we will finally define functions to batch and sum over images! To do this, we will again use a `cryojax` wrapper to `equinox` called `filter_vmap_with_spec`. This batches over a pytree, only at leaves specified by `filter_spec`. "
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 8,
             "metadata": {},
             "outputs": [],
             "source": [
                 "import equinox as eqx\n",
                 "\n",
                 "\n",
-                "@partial(cjc.filter_vmap_with_spec, filter_spec=filter_spec)\n",
-                "def compute_image_stack(pipeline):\n",
+                "@partial(cx.filter_vmap_with_spec, filter_spec=filter_spec)\n",
+                "def compute_image_stack(imaging_pipeline):\n",
                 "    \"\"\"Compute a batch of images at different poses,\n",
                 "    specified by the `filter_spec`.\n",
                 "    \"\"\"\n",
-                "    image = pipeline.render()\n",
-                "    return image - image.mean()\n",
+                "    return imaging_pipeline.render()\n",
                 "\n",
                 "\n",
                 "@eqx.filter_jit\n",
-                "def compute_micrograph(pipeline):\n",
+                "def compute_micrograph(imaging_pipeline):\n",
                 "    \"\"\"Sum together the image stack.\"\"\"\n",
-                "    return jnp.sum(compute_image_stack(pipeline), axis=0)"
+                "    return jnp.sum(compute_image_stack(imaging_pipeline), axis=0)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 9,
             "metadata": {},
             "outputs": [
@@ -233,27 +242,27 @@
                     },
                     "execution_count": 9,
                     "metadata": {},
                     "output_type": "execute_result"
                 },
                 {
                     "data": {
-                        "image/png": "iVBORw0KGgoAAAANSUhEUgAAAhYAAAFNCAYAAABc5iZ6AAAAOXRFWHRTb2Z0d2FyZQBNYXRwbG90bGliIHZlcnNpb24zLjguMywgaHR0cHM6Ly9tYXRwbG90bGliLm9yZy/H5lhTAAAACXBIWXMAAA9hAAAPYQGoP6dpAAEAAElEQVR4nOy9eZRdZZU2/txz53kea0gllcoEgfgFhDiBgEZNoywVAb9PkFZpaVAR5acgyqTipy2ggqLt2CpLPxywW5GxBbsbFGQUQkKGmqtu3Xme7zm/P2rtzbkn5966laoklXCftVihzj3je97zvvvd+9nP1kiSJKGHHnrooYceeuhhGSAc6RvooYceeuihhx6OHfQMix566KGHHnroYdnQMyx66KGHHnrooYdlQ8+w6KGHHnrooYcelg09w6KHHnrooYceelg29AyLHnrooYceeuhh2dAzLHrooYceeuihh2VDz7DooYceeuihhx6WDT3Dooceeuihhx56WDb0DIseeugCTz75JF73utfBarVCo9Hg2WefPdK39KpAoVDAhz/8YYRCIWg0GlxxxRVH+pY64vrrr4dGoznSt9FDD0cUPcOiDX784x9Do9Hgb3/725G+lWMOjz32GK6//npkMpkjcv2ZmRlcf/31XRsH9Xod5557LlKpFG699Vb89Kc/xapVqw7tTfYAAPjyl7+MH//4x7j00kvx05/+FB/4wAeO9C310EMPC0B3pG+gh1cfHnvsMdxwww344Ac/CJfLddivPzMzgxtuuAFDQ0PYsmXLgvvv27cP4+Pj+Nd//Vd8+MMfPvQ32APjP//zP3HqqafiuuuuO9K30kMPPXSJnseihxUNURRRqVSO6D3EYjEAWFYjqFgsLtu5jmXEYrGDbveV0Hd66OHViJ5hsQh88IMfhM1mw8TEBP7hH/4BNpsNfX19uOOOOwAAf//733HGGWfAarVi1apVuOuuu1qOT6VS+PSnP43NmzfDZrPB4XDg7W9/O5577rkDrjU+Po53vvOdsFqtCAQC+OQnP4n7778fGo0GjzzySMu+f/3rX/G2t70NTqcTFosFp512Gv7nf/6nq2eqVCq4/vrrsW7dOphMJoTDYbz73e/Gvn37eJ9isYhPfepTGBgYgNFoxPr16/Ev//IvUBbG1Wg0uPzyy3HPPffg+OOPh9FoxHHHHYf77ruP97n++utx1VVXAQBWr14NjUYDjUaDsbGxlnP8/Oc/x3HHHQej0cjH/8u//Ate97rXwev1wmw2Y+vWrfjVr351wDM9+OCDeMMb3gCXywWbzYb169fjmmuuAQA88sgjOPnkkwEAF198MV//xz/+sWr7fPCDH8Rpp50GADj33HOh0Whw+umn8+//+Z//iTe+8Y2wWq1wuVx417vehZdeeqnlHBR337lzJ97//vfD7XbjDW94Q9t3sph+ooZOzw+8EuajNic88sgjB/Sv008/Hccffzyef/55nHbaabBYLFi7di23+6OPPopTTjkFZrMZ69evx0MPPdTVPcZiMXzoQx9CMBiEyWTCiSeeiJ/85CcH3Mvo6Cj+8Ic/HNBP1LAcfaebPkz47//+b5x88skwmUwYHh7Gd7/7XdX7ajQauOmmmzA8PAyj0YihoSFcc801qFarLfsNDQ3hH/7hH/DII4/gpJNOgtlsxubNm/l9/OY3v8HmzZthMpmwdetWPPPMMws1M7/rP//5z/inf/oneL1eOBwOXHjhhUin0wfs/+1vf5vbLhKJ4LLLLjsgZLlnzx685z3vQSgUgslkQn9/P84//3xks9mW/X72s59h69atMJvN8Hg8OP/88zE5OXlQ5+rhKIPUgyp+9KMfSQCkJ598krdddNFFkslkkjZt2iR99KMfle644w7pda97nQRA+tGPfiRFIhHpqquukr71rW9Jxx13nKTVaqX9+/fz8U8++aQ0PDwsffazn5W++93vSjfeeKPU19cnOZ1OaXp6mvcrFArSmjVrJLPZLH32s5+VbrvtNum1r32tdOKJJ0oApD/96U+878MPPywZDAZp27Zt0te//nXp1ltvlU444QTJYDBIf/3rXzs+Y6PRkM4880wJgHT++edLt99+u3TzzTdLZ5xxhnTPPfdIkiRJoihKZ5xxhqTRaKQPf/jD0u233y6dffbZEgDpiiuuaDkfAOnEE0+UwuGwdNNNN0m33XabtGbNGslisUiJREKSJEl67rnnpAsuuEACIN16663ST3/6U+mnP/2pVCgU+BwbN26U/H6/dMMNN0h33HGH9Mwzz0iSJEn9/f3SP//zP0u33367dMstt0ivfe1rJQDS73//e76HF154QTIYDNJJJ50kfeMb35DuvPNO6dOf/rT0pje9SZIkSYpGo9KNN94oAZAuueQSvv6+fftU2+ixxx6TrrnmGgmA9PGPf1z66U9/Kj3wwAOSJEnSgw8+KOl0OmndunXSV7/6VemGG26QfD6f5Ha7pdHRUT7HddddJwGQNm3aJL3rXe+Svv3tb0t33HFH2/fSbT9Rw0LPL0mv9G35PUqSJP3pT386oH+ddtppUiQSkQYGBrhvb9q0SdJqtdIvfvELKRQKSddff71022238T3mcrmO91gqlaSNGzdKer1e+uQnPyl985vflN74xjdKAKTbbrtNkqT59/TTn/5U8vl80pYtWw7oJ2pYat+hcyzUhyVJkp5//nnJbDZLg4OD0s033yzddNNNUjAYlE444QRJOaxedNFFEgDpve99r3THHXdIF154oQRAOuecc1r2W7VqlbR+/XopHA5L119/vXTrrbdKfX19ks1mk372s59Jg4OD0le+8hXpK1/5iuR0OqW1a9dKzWazY1vTu968ebP0xje+UfrmN78pXXbZZZIgCNKb3vQmSRRF3pf66VlnnSV961vfki6//HJJq9VKJ598slSr1SRJkqRqtSqtXr1aikQi0he/+EXp+9//vnTDDTdIJ598sjQ2Nsbn+uIXvyhpNBrpvPPOk7797W/ztzE0NCSl0+lFnauHow89w6IN2hkWAKQvf/nLvC2dTktms1nSaDTSL37xC96+a9cuCYB03XXX8bZKpXLAQDA6OioZjUbpxhtv5G1f//rXJQA8uUuSJJXLZWnDhg0tA78oitLIyIi0ffv2lgGiVCpJq1evlt7ylrd0fMYf/vCHEgDplltuOeA3Ot8999wjAZC++MUvtvz+3ve+V9JoNNLevXt5GwDJYDC0bHvuueckANK3vvUt3va1r31NdWKjcwiCIL344osH/FYqlVr+rtVq0vHHHy+dccYZvO3WW2+VAEjxeLztcz/55JNsDHYDmnDvvvvulu1btmyRAoGAlEwmedtzzz0nCYIgXXjhhbyNBuwLLrigq+t120/U0M3zL9awACDdddddvI36tiAI0l/+8hfefv/993fVrrfddpsEQPrZz37G22q1mrRt2zbJZrO1GCarVq2SduzY0fF8hKX2HTpHN334nHPOkUwmkzQ+Ps7bdu7cKWm12hbD4tlnn5UASB/+8IdbrvPpT39aAiD953/+Z8uzApAee+wx3kZtajabW6713e9+94B3pQZ611u3bmXjQJIk6atf/aoEQPrd734nSZIkxWIxyWAwSG9961tb+t7tt98uAZB++MMfSpIkSc8884zqtyDH2NiYpNVqpS996Ust2//+979LOp2Ot3dzrh6OTvRCIQcBOYHP5XJh/fr1sFqteN/73sfb169fD5fLhf379/M2o9EIQZhv8maziWQyya7qp59+mve777770NfXh3e+8528zWQy4SMf+UjLfTz77LPYs2cP3v/+9yOZTCKRSCCRSKBYLOLMM8/En//8Z4ii2PY5fv3rX8Pn8+FjH/vYAb9Ryty9994LrVaLj3/84y2/f+pTn4IkSfjjH//Ysv2ss87C8PAw/33CCSfA4XC0tMNCOO2007Bp06YDtpvNZv7/dDqNbDaLN77xjS1tR/H43/3udx2ffamYnZ3Fs88+iw9+8IPweDy8/YQTTsBb3vIW3HvvvQcc89GPfrSrc3fbT9RwKJ7fZrPh/PPP57+pb2/cuBGnnHIKb6f/X+hd33vvvQiFQrjgggt4m16vx8c//nEUCgU8+uijB32vS+k7hIX6cLPZxP33349zzjkHg4ODvN/GjRuxffv2A54VAK688sqW7Z/61KcAAH/4wx9atm/atAnbtm3jv6lNzzjjjJZrddvWhEsuuQR6vZ7/vvTSS6HT6fj+HnroIdRqNVxxxRXc9wDgIx/5CBwOB9+n0+kEANx///0olUqq1/rNb34DURTxvve9j8ekRCKBUCiEkZER/OlPf+r6XD0cnegZFouEyWSC3+9v2eZ0OtHf339A/rrT6WyJY4qiiFtvvRUjIyMwGo3w+Xzw+/14/vnnW2KK4+PjGB4ePuB8a9eubfl7z549AICLLroIfr+/5b/vf//7qFarHWOV+/btw/r166HTtU8OGh8fRyQSgd1ub9m+ceNG/l0O+eBHcLvdqvHcdli9erXq9t///vc49dRTYTKZ4PF44Pf78Z3vfKflGc877zy8/vWvx4c//GEEg0Gcf/75+H//7/8tu5FBz71+/foDftu4cSMbeHK0ey4luu0najgUz9+ubw8MDBywDcCC73p8fBwjIyMtExjQvk8tBkvpO4SF+nA8Hke5XMbIyMgB+yn7w/j4OARBOODbDYVCcLlcC34/1KYH29YE5b3abDaEw2HmrLTrzwaDAWvWrOHfV69ejSuvvBLf//734fP5sH37dtxxxx0t7bhnzx5IkoSRkZEDxqWXXnqJydDdnKuHoxO9dNNFQqvVLmq7JCM4fvnLX8bnP/95/OM//iNuuukmeDweCIKAK6644qAGfjrma1/7Wtu0SZvNtujzLgXdtMNCkK8uCf/1X/+Fd77znXjTm96Eb3/72wiHw9Dr9fjRj37UQpI1m83485//jD/96U/4wx/+gPvuuw+//OUvccYZZ+CBBx5oe3+HA2rPpYal9JNunr+dgFOz2VTdvpQ+f7ixlL5DOBTP1a1o1tHQ1l//+tfxwQ9+EL/73e/wwAMP4OMf/zhuvvlm/OUvf0F/fz9EUYRGo8Ef//hH1fuWj0kLnauHoxM9w+Iw4le/+hXe/OY34wc/+EHL9kwmA5/Px3+vWrUKO3fuhCRJLQPS3r17W44jd63D4cBZZ5216PsZHh7GX//6V9Tr9RY3qRyrVq3CQw89hHw+3+K12LVrF/++WByMMuGvf/1rmEwm3H///TAajbz9Rz/60QH7CoKAM888E2eeeSZuueUWfPnLX8bnPvc5/OlPf8JZZ521LMqI9Ny7d+8+4Lddu3bB5/PBarUe1Lm77SftsNDzu91uPp8cS/EULAarVq3C888/D1EUW7wWS+lTnbCYvtMN/H4/zGYzewzlUPaHVatWQRRF7Nmzhz0yADA3N4dMJnPYhNb27NmDN7/5zfx3oVDA7Ows3vGOd/B9AvP3v2bNGt6vVqthdHT0gPFl8+bN2Lx5M6699lo89thjeP3rX48777wTX/ziFzE8PAxJkrB69WqsW7duwXvrdK4ejk70QiGHEVqt9oAVxt13343p6emWbdu3b8f09DT+/d//nbdVKhX867/+a8t+W7duxfDwMP7lX/4FhULhgOvF4/GO9/Oe97wHiUQCt99++wG/0X2+4x3vQLPZPGCfW2+9FRqNBm9/+9s7XkMNNOEuRnmTVtryVfXY2Bjuueeelv1SqdQBx5I3h9L7Dub6SoTDYWzZsgU/+clPWs7zwgsv4IEHHuAB+2DQbT9RQzfPTwbpn//8Z96n2Wzie9/73sHe8qLwjne8A9FoFL/85S95W6PRwLe+9S3YbDZO710udNt3FnO+7du345577sHExARvf+mll3D//fe37Ev94LbbbmvZfssttwAAduzYcVD3sFh873vfQ71e57+/853voNFo8Pd71llnwWAw4Jvf/GZL3/vBD36AbDbL95nL5dBoNFrOvXnzZgiCwP3r3e9+N7RaLW644YYD+rEkSUgmk12fq4ejEz2PxWHEP/zDP+DGG2/ExRdfjNe97nX4+9//jp///OctKwQA+Kd/+ifcfvvtuOCCC/CJT3wC4XAYP//5z2EymQC8suIXBAHf//738fa3vx3HHXccLr74YvT19WF6ehp/+tOf4HA48B//8R9t7+fCCy/Ev/3bv+HKK6/EE088gTe+8Y0oFot46KGH8M///M9417vehbPPPhtvfvOb8bnPfQ5jY2M48cQT8cADD+B3v/sdrrjiihaSW7fYunUrAOBzn/sczj//fOj1epx99tkdV/g7duzALbfcgre97W14//vfj1gshjvuuANr167F888/z/vdeOON+POf/4wdO3Zg1apViMVi+Pa3v43+/n7WjhgeHobL5cKdd94Ju90Oq9WKU045pWsOBOFrX/sa3v72t2Pbtm340Ic+hHK5jG9961twOp24/vrrF90uhG77iRq6ef7jjjsOp556Kq6++mqkUil4PB784he/OGCQP1S45JJL8N3vfhcf/OAH8dRTT2FoaAi/+tWv8D//8z+47bbbDuDzLBXd9p3F4IYbbsB9992HN77xjfjnf/5nNoyOO+64lnOeeOKJuOiii/C9730PmUwGp512Gp544gn85Cc/wTnnnNPiRTiUqNVqOPPMM/G+970Pu3fvxre//W284Q1vYIK43+/H1VdfjRtuuAFve9vb8M53vpP3O/nkk/F//s//ATCv23L55Zfj3HPPxbp169BoNPDTn/4UWq0W73nPewDMf19f/OIXcfXVV2NsbAznnHMO7HY7RkdH8dvf/haXXHIJPv3pT3d1rh6OUhyBTJSjAu3STa1W6wH7nnbaadJxxx13wHZlqlylUpE+9alPSeFwWDKbzdLrX/966fHHH5dOO+006bTTTms5dv/+/dKOHTsks9ks+f1+6VOf+pT061//WgLQkuInSfNpW+9+97slr9crGY1GadWqVdL73vc+6eGHH17wOUulkvS5z31OWr16taTX66VQKCS9973vbdF1yOfz0ic/+UkpEolIer1eGhkZkb72ta+1pLhK0nyq3mWXXabaDhdddFHLtptuuknq6+uTBEFoSX1sdw5JkqQf/OAH0sjIiGQ0GqUNGzZIP/rRjziVk/Dwww9L73rXu6RIJCIZDAYpEolIF1xwgfTyyy+3nOt3v/udtGnT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",
+                        "image/png": "iVBORw0KGgoAAAANSUhEUgAAAhYAAAFNCAYAAABc5iZ6AAAAOXRFWHRTb2Z0d2FyZQBNYXRwbG90bGliIHZlcnNpb24zLjguMywgaHR0cHM6Ly9tYXRwbG90bGliLm9yZy/H5lhTAAAACXBIWXMAAA9hAAAPYQGoP6dpAAEAAElEQVR4nOy9eZRcZbU2/tSpeZ7HHpNOZ4JA/AJCnHBAoyLKcgL8PhmuwpULKqL+FMTLpOLSq6CCotfxqiz9cMD7KTIKeO8FBZEAEhIy9NxdXfM81zm/P3rtzamTU9XV6U7SCfWsldWpU6fO8J73vO9+9372szWSJEnooYceeuihhx56WAEIR/sCeuihhx566KGH4wc9w6KHHnrooYceelgx9AyLHnrooYceeuhhxdAzLHrooYceeuihhxVDz7DooYceeuihhx5WDD3Dooceeuihhx56WDH0DIseeuihhx566GHF0DMseuihhx566KGHFUPPsOihhx566KGHHlYMPcOihx66wJNPPolXvepVsFqt0Gg02Llz59G+pJcFCoUCPvzhDyMUCkGj0eDKK6882pfUEddffz00Gs3Rvoweejiq6BkWbfDjH/8YGo0Gf/vb3472pRx3eOyxx3D99dcjk8kclfPPzs7i+uuv79o4qNfreN/73odUKoVbbrkFP/3pTzE0NHR4L7IHAMCXvvQl/PjHP8Zll12Gn/70p/jgBz94tC+phx56WAS6o30BPbz88Nhjj+GGG27ARRddBJfLdcTPPzs7ixtuuAHDw8PYunXrovvv378fExMT+Pd//3d8+MMfPvwX2APjT3/6E04//XRcd911R/tSeuihhy7R81j0sKohiiIqlcpRvYZYLAYAK2oEFYvFFTvW8YxYLHbI7b4a+k4PPbwc0TMsloCLLroINpsNk5OTeMc73gGbzYa+vj7cfvvtAIDnnnsOb3zjG2G1WjE0NIQ777yz5fepVAqf+tSnsGXLFthsNjgcDrztbW/DM888c9C5JiYm8M53vhNWqxWBQACf+MQncN9990Gj0eCRRx5p2fevf/0r3vrWt8LpdMJiseCMM87A//zP/3R1T5VKBddffz3Wr18Pk8mEcDiMd7/73di/fz/vUywW8clPfhIDAwMwGo3YsGED/u3f/g3KwrgajQZXXHEF7r77bpx44okwGo044YQTcO+99/I+119/PT796U8DANasWQONRgONRoPx8fGWY/z85z/HCSecAKPRyL//t3/7N7zqVa+C1+uF2WzGtm3b8Ktf/eqge3rggQfwmte8Bi6XCzabDRs2bMA111wDAHjkkUdw6qmnAgAuvvhiPv+Pf/xj1fa56KKLcMYZZwAA3ve+90Gj0eD1r389f/+nP/0Jr33ta2G1WuFyufCud70LL7zwQssxKO6+a9cufOADH4Db7cZrXvOats9kKf1EDZ3uH3gpzEdtTnjkkUcO6l+vf/3rceKJJ+LZZ5/FGWecAYvFgnXr1nG7P/roozjttNNgNpuxYcMGPPjgg11dYywWw4c+9CEEg0GYTCacfPLJ+MlPfnLQtYyNjeEPf/jDQf1EDSvRd7rpw4T//u//xqmnngqTyYSRkRF897vfVb2uRqOBm266CSMjIzAajRgeHsY111yDarXast/w8DDe8Y534JFHHsEpp5wCs9mMLVu28PP4zW9+gy1btsBkMmHbtm14+umnF2tmftZ//vOf8c///M/wer1wOBy44IILkE6nD9r/29/+NrddJBLB5ZdfflDIcu/evXjPe96DUCgEk8mE/v5+nHfeechmsy37/exnP8O2bdtgNpvh8Xhw3nnnYWpq6pCO1cMxBqkHVfzoRz+SAEhPPvkkb7vwwgslk8kkbd68WfrIRz4i3X777dKrXvUqCYD0ox/9SIpEItKnP/1p6Vvf+pZ0wgknSFqtVjpw4AD//sknn5RGRkakz372s9J3v/td6cYbb5T6+vokp9MpzczM8H6FQkFau3atZDabpc9+9rPSrbfeKr3yla+UTj75ZAmA9PDDD/O+Dz30kGQwGKTt27dLX/va16RbbrlFOumkkySDwSD99a9/7XiPjUZDetOb3iQBkM477zzptttuk26++WbpjW98o3T33XdLkiRJoihKb3zjGyWNRiN9+MMflm677Tbp7LPPlgBIV155ZcvxAEgnn3yyFA6HpZtuukm69dZbpbVr10oWi0VKJBKSJEnSM888I51//vkSAOmWW26RfvrTn0o//elPpUKhwMfYtGmT5Pf7pRtuuEG6/fbbpaefflqSJEnq7++X/uVf/kW67bbbpK9//evSK1/5SgmA9Pvf/56v4R//+IdkMBikU045RfrGN74h3XHHHdKnPvUp6XWve50kSZIUjUalG2+8UQIgXXrppXz+/fv3q7bRY489Jl1zzTUSAOljH/uY9NOf/lS6//77JUmSpAceeEDS6XTS+vXrpa985SvSDTfcIPl8PsntdktjY2N8jOuuu04CIG3evFl617veJX3729+Wbr/99rbPpdt+oobF7l+SXurb8muUJEl6+OGHD+pfZ5xxhhSJRKSBgQHu25s3b5a0Wq30i1/8QgqFQtL1118v3XrrrXyNuVyu4zWWSiVp06ZNkl6vlz7xiU9I3/zmN6XXvva1EgDp1ltvlSRp4Tn99Kc/lXw+n7R169aD+okaltt36BiL9WFJkqRnn31WMpvN0uDgoHTzzTdLN910kxQMBqWTTjpJUg6rF154oQRAeu973yvdfvvt0gUXXCABkM4555yW/YaGhqQNGzZI4XBYuv7666VbbrlF6uvrk2w2m/Szn/1MGhwclL785S9LX/7ylyWn0ymtW7dOajabHduanvWWLVuk1772tdI3v/lN6fLLL5cEQZBe97rXSaIo8r7UT88880zpW9/6lnTFFVdIWq1WOvXUU6VarSZJkiRVq1VpzZo1UiQSkb7whS9I3//+96UbbrhBOvXUU6Xx8XE+1he+8AVJo9FI5557rvTtb3+b343h4WEpnU4v6Vg9HHvoGRZt0M6wACB96Utf4m3pdFoym82SRqORfvGLX/D23bt3SwCk6667jrdVKpWDBoKxsTHJaDRKN954I2/72te+JgHgyV2SJKlcLksbN25sGfhFUZRGR0elHTt2tAwQpVJJWrNmjfTmN7+54z3+8Ic/lABIX//61w/6jo539913SwCkL3zhCy3fv/e975U0Go20b98+3gZAMhgMLdueeeYZCYD0rW99i7d99atfVZ3Y6BiCIEjPP//8Qd+VSqWWz7VaTTrxxBOlN77xjbztlltukQBI8Xi87X0/+eSTbAx2A5pw77rrrpbtW7dulQKBgJRMJnnbM888IwmCIF1wwQW8jQbs888/v6vzddtP1NDN/S/VsAAg3XnnnbyN+rYgCNJf/vIX3n7fffd11a633nqrBED62c9+xttqtZq0fft2yWaztRgmQ0ND0llnndXxeITl9h06Rjd9+JxzzpFMJpM0MTHB23bt2iVptdoWw2Lnzp0SAOnDH/5wy3k+9alPSQCkP/3pTy33CkB67LHHeBu1qdlsbjnXd7/73YOelRroWW/bto2NA0mSpK985SsSAOl3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vxtarRY33HDDQf1YkiQkk8muj9XDsYmex+II4h3veAduvPFGXHzxxXjVq16F5557Dj//+c9bVggA8M///M+47bbbcP755+PjH/84wuEwfv7zn8NkMgF4acUvCAK+//3v421vextOOOEEXHzxxejr68PMzAwefvhhOBwO/L//9//aXs8FF1yA//iP/8BVV12FJ554Aq997WtRLBbx4IMP4l/+5V/wrne9C2effTbe8IY34HOf+xzGx8dx8skn4/7778fvfvc7XHnllS0kt26xbds2AMDnPvc5nHfeedDr9Tj77LM7rvDPOussfP3rX8db3/pWfOADH0AsFsPtt9+OdevW4dlnn+X9brzxRvz5z3/GWWedhaGhIcRiMXz7299Gf38/a0eMjIzA5XLhjjvugN1uh9VqxWmnndY1B4Lw1a9+FW9729uwfft2fOhDH0K5XMa3vvUtOJ1OXH/99UtuF0K3/UQN3dz/CSecgNNPPx1XX301UqkUPB4PfvGLXxw0yB8uXHrppfjud7+Liy66CE899RSGh4fxq1/9Cv/zP/+DW2+99SA+z3LRbd9ZCm644Qbce++9eO1rX4t/+Zd/YcPohBNOaDnmySefjAsvvBDf+973kMlkcMYZZ+CJJ57AT37yE5xzzjktXoTDiVqthje96U14//vfjz179uDb3/42XvOa1zBB3O/34+qrr8YNN9yAt771rXjnO9/J+5166qn4P//n/wBY0G254oor8L73vQ/r169Ho9HAT3/6U2i1WrznPe8BsPB+feELX8DVV1+N8fFxnHPOObDb7RgbG8Nvf/tbXHrppfjUpz7V1bF6OEZxFDJRjgm0Sze1Wq0H7XvGGWdIJ5xwwkHblalylUpF+uQnPymFw2HJbDZLr371q6XHH39cOuOMM6Qzzjij5bcHDhyQzjrrLMlsNkt+v1/65Cc/Kf3617+WALSk+EnSQtrWu9/9bsnr9UpGo1EaGhqS3v/+90sPPfTQovdZKpWkz33uc9KaNWskvV4vhUIh6b3vfW+LrkM+n5c+8YlPSJFIRNLr9dLo6Kj01a9+tSXFVZIWUvUuv/xy1Xa48MILW7bddNNNUl9fnyQIQkvqY7tjSJIk/eAHP5BGR0clo9Eobdy4UfrRj37EqZyEhx56SHrXu94lRSIRyWAwSJFIRDr//POlF198seVYv/vd76TNmzdL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",
                         "text/plain": [
                             "<Figure size 550x550 with 2 Axes>"
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
                 }
             ],
             "source": [
                 "# Compute the image and plot\n",
                 "fig, ax = plt.subplots(figsize=(5.5, 5.5))\n",
-                "micrograph = compute_micrograph(pipeline)\n",
+                "micrograph = compute_micrograph(imaging_pipeline)\n",
                 "plot_image(\n",
                 "    micrograph,\n",
                 "    fig,\n",
                 "    ax,\n",
                 "    label=\"Image contrast for a sum of random poses\",\n",
                 "    interpolation=None,\n",
                 ")"
```

### Comparing `cryojax-0.2.3rc1/docs/examples/test-multiatom.ipynb` & `cryojax-0.3.0a0/docs/examples/test-multiatom.ipynb`

 * *Files identical despite different names*

### Comparing `cryojax-0.2.3rc1/docs/examples/data/ribosome_4ug0_particles.star` & `cryojax-0.3.0a0/docs/examples/data/ribosome_4ug0_particles.star`

 * *Files identical despite different names*

### Comparing `cryojax-0.2.3rc1/src/cryojax/constants/_load_atoms.py` & `cryojax-0.3.0a0/src/cryojax/constants/_load_atoms.py`

 * *Files identical despite different names*

### Comparing `cryojax-0.2.3rc1/src/cryojax/constants/element_params.npy` & `cryojax-0.3.0a0/src/cryojax/constants/element_params.npy`

 * *Files identical despite different names*

### Comparing `cryojax-0.2.3rc1/src/cryojax/core/_errors.py` & `cryojax-0.3.0a0/src/cryojax/_errors.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Utilities for runtime errors, wrapping `equinox.error_if`. 
+Utilities for runtime errors, wrapping `equinox.error_if`.
 """
 
 import equinox as eqx
 import jax.numpy as jnp
 from jaxtyping import Array, ArrayLike
```

### Comparing `cryojax-0.2.3rc1/src/cryojax/core/_filtered_transformations.py` & `cryojax-0.3.0a0/src/cryojax/_filtered_transformations.py`

 * *Files 22% similar despite different names*

```diff
@@ -14,14 +14,18 @@
 def filter_grad_with_spec(
     func: Callable,
     filter_spec: PyTree[Union[bool, Callable[[Any], bool]]],
     is_leaf: Optional[Callable[[Any], bool]] = None,
     *,
     has_aux: bool = False,
 ) -> Callable:
+    """A lightweight wrapper around `equinox.filter_grad` that accepts a
+    `filter_spec`.
+    """
+
     @wraps(func)
     def partition_and_recombine_fn(pytree: PyTree, *args: Any, **kwargs: Any):
         @partial(
             eqx.filter_grad,
             has_aux=has_aux,
         )
         def recombine_fn(
@@ -41,14 +45,18 @@
 def filter_value_and_grad_with_spec(
     func: Callable,
     filter_spec: PyTree[Union[bool, Callable[[Any], bool]]],
     is_leaf: Optional[Callable[[Any], bool]] = None,
     *,
     has_aux: bool = False,
 ) -> Callable:
+    """A lightweight wrapper around `equinox.filter_value_and_grad` that
+    accepts a `filter_spec`.
+    """
+
     @wraps(func)
     def partition_and_recombine_fn(pytree: PyTree, *args: Any, **kwargs: Any):
         @partial(
             eqx.filter_value_and_grad,
             has_aux=has_aux,
         )
         def recombine_fn(
@@ -75,14 +83,18 @@
     ),
     out_axes: PyTree[Union[int, None, Callable[[Any], Optional[int]]]] = eqx.if_array(
         axis=0
     ),
     axis_name: Hashable = None,
     axis_size: Optional[int] = None,
 ) -> Callable:
+    """A lightweight wrapper around `equinox.filter_vmap` that accepts a
+    `filter_spec`.
+    """
+
     @wraps(func)
     def partition_and_recombine_fn(pytree: PyTree, *args: Any):
         @partial(
             eqx.filter_vmap,
             in_axes=(in_axes, None),
             out_axes=out_axes,
             axis_name=axis_name,
```

### Comparing `cryojax-0.2.3rc1/src/cryojax/data/_dataset.py` & `cryojax-0.3.0a0/src/cryojax/data/_dataset.py`

 * *Files identical despite different names*

### Comparing `cryojax-0.2.3rc1/src/cryojax/data/_relion.py` & `cryojax-0.3.0a0/src/cryojax/data/_relion.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,17 +7,17 @@
 import equinox as eqx
 import jax.numpy as jnp
 import mrcfile
 import numpy as np
 import pandas as pd
 from jaxtyping import Array, Float, Int
 
-from ..io import read_and_validate_starfile
-from ..simulator import CTF, EulerAnglePose, ImageConfig
+from ..simulator import ContrastTransferFunction, EulerAnglePose, InstrumentConfig
 from ._dataset import AbstractDataset
+from ._io import read_and_validate_starfile
 from ._particle_stack import AbstractParticleStack
 
 
 RELION_REQUIRED_OPTICS_KEYS = [
     "rlnImageSize",
     "rlnVoltage",
     "rlnImagePixelSize",
@@ -35,100 +35,101 @@
 
 class RelionParticleStack(AbstractParticleStack):
     """A particle stack with information imported from
     [RELION](https://relion.readthedocs.io/en/release-5.0/).
     """
 
     image_stack: Float[Array, "... y_dim x_dim"]
-    config: ImageConfig
+    instrument_config: InstrumentConfig
     pose: EulerAnglePose
-    ctf: CTF
+    ctf: ContrastTransferFunction
 
     def __init__(
         self,
         image_stack: Float[Array, "... y_dim x_dim"],
-        config: ImageConfig,
+        instrument_config: InstrumentConfig,
         pose: EulerAnglePose,
-        ctf: CTF,
+        ctf: ContrastTransferFunction,
     ):
         # Set image stack and config as is
         self.image_stack = jnp.asarray(image_stack)
-        self.config = config
+        self.instrument_config = instrument_config
         # Set CTF using the defocus offset in the EulerAnglePose
         self.ctf = eqx.tree_at(
-            lambda ctf: (ctf.defocus_u_in_angstroms, ctf.defocus_v_in_angstroms),
+            lambda tf: tf.defocus_in_angstroms,
             ctf,
-            (
-                ctf.defocus_u_in_angstroms + pose.offset_z_in_angstroms,
-                ctf.defocus_v_in_angstroms + pose.offset_z_in_angstroms,
-            ),
+            ctf.defocus_in_angstroms + pose.offset_z_in_angstroms,
         )
         # Set defocus offset to zero
         self.pose = eqx.tree_at(
             lambda pose: pose.offset_z_in_angstroms, pose, jnp.asarray(0.0)
         )
 
 
 RelionParticleStack.__init__.__doc__ = """**Arguments:**
 
 - `image_stack`: The stack of images. The shape of this array
                  is a leading batch dimension followed by the shape
                  of an image in the stack.
-- `config`: The image configuration. Any subset of pytree leaves may
+- `instrument_config`: The instrument configuration. Any subset of pytree leaves may
             have a batch dimension.
 - `pose`: The pose, represented by euler angles. Any subset of pytree leaves may
           have a batch dimension. Upon instantiation, `pose.offset_z_in_angstroms`
           is set to zero.
 - `ctf`: The contrast transfer function. Any subset of pytree leaves may
-         have a batch dimension. Upon instantiation, `ctf.defocus_u_in_angstroms`
-         is set to `ctf.defocus_u_in_angstroms + pose.offset_z_in_angstroms` (and
-         also for `ctf.defocus_v_in_angstroms`).
-"""
+                       have a batch dimension. Upon instantiation,
+                       `ctf.defocus_in_angstroms` is set to
+                       `ctf.defocus_in_angstroms + pose.offset_z_in_angstroms`.
+"""  # noqa: E501
 
 
-def default_relion_make_config(
-    shape: tuple[int, int], pixel_size: float | Float[np.ndarray, "..."], **kwargs: Any
+def _default_make_instrument_config_fn(
+    shape: tuple[int, int],
+    pixel_size: Float[Array, ""],
+    voltage_in_kilovolts: Float[Array, ""],
+    **kwargs: Any,
 ):
-    return ImageConfig(shape, jnp.asarray(pixel_size), **kwargs)
+    return InstrumentConfig(shape, pixel_size, voltage_in_kilovolts, **kwargs)
 
 
 @dataclasses.dataclass(frozen=True)
 class RelionDataset(AbstractDataset):
     """A dataset that wraps a Relion particle stack in
     [STAR](https://relion.readthedocs.io/en/latest/Reference/Conventions.html) format.
     """
 
     path_to_relion_project: pathlib.Path
     data_blocks: dict[str, pd.DataFrame]
 
-    make_config: Callable[
-        [tuple[int, int], float | Float[np.ndarray, "..."]], ImageConfig
+    make_instrument_config_fn: Callable[
+        [tuple[int, int], Float[Array, "..."], Float[Array, "..."]], InstrumentConfig
     ]
 
     @final
     def __init__(
         self,
         path_to_starfile: str | pathlib.Path,
         path_to_relion_project: str | pathlib.Path,
-        make_config: Callable[
-            [tuple[int, int], float | Float[np.ndarray, "..."]], ImageConfig
-        ] = default_relion_make_config,
+        make_instrument_config_fn: Callable[
+            [tuple[int, int], Float[Array, "..."], Float[Array, "..."]],
+            InstrumentConfig,
+        ] = _default_make_instrument_config_fn,
     ):
         """**Arguments:**
 
         - `path_to_starfile`: The path to the Relion STAR file.
         - `path_to_relion_project`: The path to the Relion project directory.
         """
         data_blocks = read_and_validate_starfile(path_to_starfile)
         _validate_relion_data_blocks(data_blocks)
         object.__setattr__(self, "data_blocks", data_blocks)
         object.__setattr__(
             self, "path_to_relion_project", pathlib.Path(path_to_relion_project)
         )
-        object.__setattr__(self, "make_config", make_config)
+        object.__setattr__(self, "make_instrument_config_fn", make_instrument_config_fn)
 
     @final
     def __getitem__(
         self, index: int | slice | Int[np.ndarray, ""] | Int[np.ndarray, " N"]
     ) -> RelionParticleStack:
         # Load particle data and optics group
         n_rows = self.data_blocks["particles"].shape[0]
@@ -138,15 +139,15 @@
             f"access the index {idx}."
         )
         # pandas has bad error messages for its indexing
         if isinstance(index, (int, Int[np.ndarray, ""])):
             if index > n_rows - 1:
                 raise IndexError(index_error_msg(index))
         elif isinstance(index, slice):
-            if index.start > n_rows - 1:
+            if index.start is not None and index.start > n_rows - 1:
                 raise IndexError(index_error_msg(index.start))
         elif isinstance(index, np.ndarray):
             pass  # catch exceptions later
         else:
             raise IndexError(
                 f"Indexing with the type {type(index)} is not supported by "
                 "`RelionDataset`. Indexing by integers is supported, one-dimensional "
@@ -207,46 +208,50 @@
                 )
             # ... create full path to the image stack
             path_to_image_stack = pathlib.Path(
                 self.path_to_relion_project,
                 np.asarray(image_stack_filename, dtype=object)[0],
             )
             # ... relion convention starts indexing at 1, not 0
-            particle_index = (
-                np.asarray(relion_particle_index.astype(int), dtype=int) - 1
-            )
+            particle_index = np.asarray(relion_particle_index.astype(int), dtype=int) - 1
         else:
             raise IOError(
                 "Could not read `rlnImageName` in STAR file for `RelionDataset` "
                 f"index equal to {index}."
             )
         with mrcfile.mmap(path_to_image_stack, mode="r", permissive=True) as mrc:
             image_stack = np.asarray(mrc.data[particle_index])  # type: ignore
         # Read metadata into a RelionParticleStack
         # ... particle data
-        defocus_u_in_angstroms = np.asarray(particle_blocks["rlnDefocusU"])
-        defocus_v_in_angstroms = np.asarray(particle_blocks["rlnDefocusV"])
-        astigmatism_angle = np.asarray(particle_blocks["rlnDefocusAngle"])
-        phase_shift = np.asarray(particle_blocks["rlnPhaseShift"])
+        defocus_in_angstroms = jnp.asarray(particle_blocks["rlnDefocusU"])
+        astigmatism_in_angstroms = jnp.asarray(
+            particle_blocks["rlnDefocusV"]
+        ) - jnp.asarray(particle_blocks["rlnDefocusU"])
+        astigmatism_angle = jnp.asarray(particle_blocks["rlnDefocusAngle"])
+        phase_shift = jnp.asarray(particle_blocks["rlnPhaseShift"])
         # ... optics group data
-        image_size = np.asarray(optics_group["rlnImageSize"])
-        pixel_size = np.asarray(optics_group["rlnImagePixelSize"])
-        voltage_in_kilovolts = np.asarray(optics_group["rlnVoltage"])
-        spherical_aberration_in_mm = np.asarray(optics_group["rlnSphericalAberration"])
-        amplitude_contrast_ratio = np.asarray(optics_group["rlnAmplitudeContrast"])
+        image_size = jnp.asarray(optics_group["rlnImageSize"])
+        pixel_size = jnp.asarray(optics_group["rlnImagePixelSize"])
+        voltage_in_kilovolts = float(optics_group["rlnVoltage"])
+        spherical_aberration_in_mm = jnp.asarray(optics_group["rlnSphericalAberration"])
+        amplitude_contrast_ratio = jnp.asarray(optics_group["rlnAmplitudeContrast"])
         # ... create cryojax objects
-        config = self.make_config((int(image_size), int(image_size)), pixel_size)
-        ctf = CTF(
-            defocus_u_in_angstroms,
-            defocus_v_in_angstroms,
-            astigmatism_angle,
-            voltage_in_kilovolts,
-            spherical_aberration_in_mm,
-            amplitude_contrast_ratio,
-            phase_shift,
+        instrument_config = self.make_instrument_config_fn(
+            (int(image_size), int(image_size)),
+            pixel_size,
+            jnp.asarray(voltage_in_kilovolts),
+        )
+        ctf = ContrastTransferFunction(
+            defocus_in_angstroms=defocus_in_angstroms,
+            astigmatism_in_angstroms=astigmatism_in_angstroms,
+            astigmatism_angle=astigmatism_angle,
+            voltage_in_kilovolts=voltage_in_kilovolts,
+            spherical_aberration_in_mm=spherical_aberration_in_mm,
+            amplitude_contrast_ratio=amplitude_contrast_ratio,
+            phase_shift=phase_shift,
         )
         pose = EulerAnglePose()
         # ... values for the pose are optional, so look to see if
         # each key is present
         particle_keys = particle_blocks.keys()
         pose_parameter_names_and_values = []
         if "rlnOriginXAngst" in particle_keys:
@@ -289,17 +294,15 @@
                 # ... if the column is just equal to a float, then
                 # directly check if it is equal to -999.0
                 particle_blocks_for_psi = (
                     0.0
                     if particle_blocks["rlnAnglePsi"] == -999.0
                     else particle_blocks["rlnAnglePsi"]
                 )
-            pose_parameter_names_and_values.append(
-                ("view_psi", particle_blocks_for_psi)
-            )
+            pose_parameter_names_and_values.append(("view_psi", particle_blocks_for_psi))
         elif "rlnAnglePsiPrior" in particle_keys:  # support for helices
             pose_parameter_names_and_values.append(
                 ("view_psi", particle_blocks["rlnAnglePsiPrior"])
             )
         pose_parameter_names, pose_parameter_values = tuple(
             zip(*pose_parameter_names_and_values)
         )
@@ -308,15 +311,15 @@
         # instantiation
         pose = eqx.tree_at(
             lambda p: tuple([getattr(p, name) for name in pose_parameter_names]),
             pose,
             tuple([jnp.asarray(value) for value in pose_parameter_values]),
         )
 
-        return RelionParticleStack(jnp.asarray(image_stack), config, pose, ctf)
+        return RelionParticleStack(jnp.asarray(image_stack), instrument_config, pose, ctf)
 
     @final
     def __len__(self) -> int:
         return len(self.data_blocks["particles"])
 
 
 @dataclasses.dataclass(frozen=True)
```

### Comparing `cryojax-0.2.3rc1/src/cryojax/image/__init__.py` & `cryojax-0.3.0a0/src/cryojax/image/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -18,9 +18,12 @@
     map_coordinates_with_cubic_spline as map_coordinates_with_cubic_spline,
 )
 from ._normalize import (
     compute_mean_and_std_from_fourier_image as compute_mean_and_std_from_fourier_image,
     normalize_image as normalize_image,
     rescale_image as rescale_image,
 )
-from ._rescale_pixel_size import rescale_pixel_size as rescale_pixel_size
+from ._rescale_pixel_size import (
+    maybe_rescale_pixel_size as maybe_rescale_pixel_size,
+    rescale_pixel_size as rescale_pixel_size,
+)
 from ._spectrum import powerspectrum as powerspectrum
```

### Comparing `cryojax-0.2.3rc1/src/cryojax/image/_average.py` & `cryojax-0.3.0a0/src/cryojax/image/_average.py`

 * *Files 4% similar despite different names*

```diff
@@ -109,13 +109,11 @@
         elif interpolation_mode == "linear":
             average_as_grid = jnp.interp(
                 radial_grid.ravel(),
                 bins,
                 average_as_profile,
             ).reshape(radial_grid.shape)
         else:
-            raise ValueError(
-                f"interpolation_mode = {interpolation_mode} not supported."
-            )
+            raise ValueError(f"interpolation_mode = {interpolation_mode} not supported.")
         return average_as_profile, average_as_grid
     else:
         return average_as_profile
```

### Comparing `cryojax-0.2.3rc1/src/cryojax/image/_edges.py` & `cryojax-0.3.0a0/src/cryojax/image/_edges.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,17 +20,15 @@
 def crop_to_shape(
     image_or_volume: Inexact[Array, "z_dim y_dim x_dim"],
     shape: tuple[int, int, int],
 ) -> Inexact[Array, " {shape[0]} {shape[1]} {shape[2]}"]: ...
 
 
 def crop_to_shape(
-    image_or_volume: (
-        Inexact[Array, "y_dim x_dim"] | Inexact[Array, "z_dim y_dim x_dim"]
-    ),
+    image_or_volume: Inexact[Array, "y_dim x_dim"] | Inexact[Array, "z_dim y_dim x_dim"],
     shape: tuple[int, int] | tuple[int, int, int],
 ) -> (
     Inexact[Array, " {shape[0]} {shape[1]}"]
     | Inexact[Array, " {shape[0]} {shape[1]} {shape[2]}"]
 ):
     """Crop an image or volume to a new shape around its
     center.
@@ -120,17 +118,15 @@
     image_or_volume: Inexact[Array, "z_dim y_dim x_dim"],
     shape: tuple[int, int, int],
     **kwargs: Any,
 ) -> Inexact[Array, " {shape[0]} {shape[1]} {shape[2]}"]: ...
 
 
 def pad_to_shape(
-    image_or_volume: (
-        Inexact[Array, "y_dim x_dim"] | Inexact[Array, "z_dim y_dim x_dim"]
-    ),
+    image_or_volume: Inexact[Array, "y_dim x_dim"] | Inexact[Array, "z_dim y_dim x_dim"],
     shape: tuple[int, int] | tuple[int, int, int],
     **kwargs: Any,
 ) -> (
     Inexact[Array, " {shape[0]} {shape[1]}"]
     | Inexact[Array, " {shape[0]} {shape[1]} {shape[2]}"]
 ):
     """Pad an image or volume to a new shape."""
```

### Comparing `cryojax-0.2.3rc1/src/cryojax/image/_fft.py` & `cryojax-0.3.0a0/src/cryojax/image/_fft.py`

 * *Files 1% similar despite different names*

```diff
@@ -117,17 +117,15 @@
 
 def irfftn(
     ft: Complex[Array, "y_dim x_dim//2+1"] | Complex[Array, "z_dim y_dim x_dim//2+1"],
     s: Optional[tuple[int, ...]] = None,
     axes: Optional[tuple[int, ...]] = None,
     **kwargs: Any,
 ) -> (
-    Float[Array, "y_dim x_dim"]
-    | Float[Array, "z_dim y_dim x_dim"]
-    | Float[Array, " *s"]
+    Float[Array, "y_dim x_dim"] | Float[Array, "z_dim y_dim x_dim"] | Float[Array, " *s"]
 ):
     """
     Helper routine to compute the inverse fourier transform
     from real input.
 
     Arguments
     ---------
```

### Comparing `cryojax-0.2.3rc1/src/cryojax/image/_map_coordinates.py` & `cryojax-0.3.0a0/src/cryojax/image/_map_coordinates.py`

 * *Files identical despite different names*

### Comparing `cryojax-0.2.3rc1/src/cryojax/image/_normalize.py` & `cryojax-0.3.0a0/src/cryojax/image/_normalize.py`

 * *Files 2% similar despite different names*

```diff
@@ -100,15 +100,15 @@
             N1 * (2 * N2 - 1)
             if shape_in_real_space is None
             else shape_in_real_space[0] * shape_in_real_space[1]
         )
     else:
         N_modes = N1 * N2
     # The mean is just the zero mode divided by the number of modes
-    mean = fourier_image[0, 0] / N_modes
+    mean = fourier_image[0, 0].real / N_modes
     # The standard deviation is square root norm squared of the zero mean image
     std = (
         jnp.sqrt(
             jnp.sum(jnp.abs(fourier_image[:, 0]) ** 2)
             - jnp.abs(fourier_image[0, 0]) ** 2
             + 2 * jnp.sum(jnp.abs(fourier_image[:, 1:]) ** 2)
         )
```

### Comparing `cryojax-0.2.3rc1/src/cryojax/image/_spectrum.py` & `cryojax-0.3.0a0/src/cryojax/image/_spectrum.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,17 +40,15 @@
     *,
     to_grid: bool = False,
     interpolation_mode: str = "nearest",
     k_min: Optional[Float[Array, ""] | float] = None,
     k_max: Optional[Float[Array, ""] | float] = None,
 ) -> (
     tuple[Float[Array, " n_bins"], Float[Array, " n_bins"]]
-    | tuple[
-        Float[Array, " n_bins"], Float[Array, "y_dim x_dim"], Float[Array, " n_bins"]
-    ]
+    | tuple[Float[Array, " n_bins"], Float[Array, "y_dim x_dim"], Float[Array, " n_bins"]]
 ): ...
 
 
 @overload
 def powerspectrum(
     fourier_image: Complex[Array, "z_dim y_dim x_dim"],
     radial_frequency_grid: Float[Array, "z_dim y_dim x_dim"],
```

### Comparing `cryojax-0.2.3rc1/src/cryojax/image/operators/__init__.py` & `cryojax-0.3.0a0/src/cryojax/image/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `cryojax-0.2.3rc1/src/cryojax/image/operators/_filters.py` & `cryojax-0.3.0a0/src/cryojax/image/operators/_filters.py`

 * *Files identical despite different names*

### Comparing `cryojax-0.2.3rc1/src/cryojax/image/operators/_fourier_operator.py` & `cryojax-0.3.0a0/src/cryojax/image/operators/_fourier_operator.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from typing import overload
 from typing_extensions import override
 
 import jax.numpy as jnp
 from equinox import field
 from jaxtyping import Array, Float, Inexact
 
-from ...core import error_if_not_positive
+from ..._errors import error_if_not_positive
 from ._operator import AbstractImageOperator
 
 
 class AbstractFourierOperator(AbstractImageOperator, strict=True):
     """
     The base class for all fourier-based operators.
```

### Comparing `cryojax-0.2.3rc1/src/cryojax/image/operators/_masks.py` & `cryojax-0.3.0a0/src/cryojax/image/operators/_masks.py`

 * *Files identical despite different names*

### Comparing `cryojax-0.2.3rc1/src/cryojax/image/operators/_operator.py` & `cryojax-0.3.0a0/src/cryojax/image/operators/_operator.py`

 * *Files identical despite different names*

### Comparing `cryojax-0.2.3rc1/src/cryojax/image/operators/_real_operator.py` & `cryojax-0.3.0a0/src/cryojax/image/operators/_real_operator.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from typing import overload
 from typing_extensions import override
 
 import jax.numpy as jnp
 from equinox import field
 from jaxtyping import Array, Float
 
-from ...core import error_if_not_positive
+from ..._errors import error_if_not_positive
 from ._operator import AbstractImageOperator
 
 
 class AbstractRealOperator(AbstractImageOperator, strict=True):
     """
     The base class for all real operators.
```

### Comparing `cryojax-0.2.3rc1/src/cryojax/inference/distributions/_distribution.py` & `cryojax-0.3.0a0/src/cryojax/inference/distributions/_base_distribution.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,55 +1,51 @@
 """
 Base class for a cryojax distribution.
 """
 
 from abc import abstractmethod
 
-from equinox import AbstractVar, Module
+from equinox import Module
 from jaxtyping import Array, Float, Inexact, PRNGKeyArray
 
 
 class AbstractDistribution(Module, strict=True):
     """An image formation model equipped with a probabilistic model."""
 
     @abstractmethod
-    def log_likelihood(
-        self, observed: Inexact[Array, "y_dim x_dim"]
-    ) -> Float[Array, ""]:
+    def log_likelihood(self, observed: Inexact[Array, "y_dim x_dim"]) -> Float[Array, ""]:
         """Evaluate the log likelihood.
 
         **Arguments:**
 
         - `observed` : The observed data in real or fourier space.
         """
         raise NotImplementedError
 
     @abstractmethod
     def sample(
-        self, key: PRNGKeyArray, *, get_real: bool = True
+        self, rng_key: PRNGKeyArray, *, get_real: bool = True
     ) -> Inexact[Array, "y_dim x_dim"]:
         """Sample from the distribution.
 
         **Arguments:**
 
-        - `key` : The RNG key or key(s). See `AbstractPipeline.sample` for
+        - `rng_key` : The RNG key or key(s). See `AbstractPipeline.sample` for
                   more documentation.
         """
         raise NotImplementedError
 
     @abstractmethod
-    def render(self, *, get_real: bool = True) -> Inexact[Array, "y_dim x_dim"]:
+    def compute_signal(self, *, get_real: bool = True) -> Inexact[Array, "y_dim x_dim"]:
         """Render the image formation model."""
         raise NotImplementedError
 
 
 class AbstractMarginalDistribution(AbstractDistribution, strict=True):
-    """An image formation model equipped with a probabilistic model."""
-
-    distribution: AbstractVar[AbstractDistribution]
+    """An `AbstractDistribution` equipped with a marginalized likelihood."""
 
     @abstractmethod
     def marginal_log_likelihood(
         self, observed: Inexact[Array, "y_dim x_dim"]
     ) -> Float[Array, ""]:
         """Evaluate the marginalized log likelihood.
```

### Comparing `cryojax-0.2.3rc1/src/cryojax/inference/transforms/_lie_group_transforms.py` & `cryojax-0.3.0a0/src/cryojax/inference/_transforms/lie_group_transforms.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 import jax.numpy as jnp
 import jax.tree_util as jtu
 from equinox import AbstractVar
 from jaxtyping import Array, Float, PyTree
 
 from ...rotations import AbstractMatrixLieGroup, SE3, SO3
 from ...simulator import QuaternionPose
-from ._transforms import AbstractParameterTransform
+from .transforms import AbstractParameterTransform
 
 
 def _apply_update_with_lie_transform(u, p):
     if u is None:
         return p
     elif isinstance(u, AbstractLieGroupTransform):
         lie_group = type(u.group_element)
@@ -64,15 +64,14 @@
     tangent space of the corresponding SO3 element.
 
     This class is based on the implementation in `jaxlie.manifold`.
 
     **Attributes:**
 
     - `transformed_parameter`: The local tangent vector.
-
     - `group_element`: The element of SO3.
     """
 
     transformed_parameter: Float[Array, "3"]
     group_element: SO3
 
     def __init__(self, wxyz: Float[Array, "4"]):
@@ -96,15 +95,14 @@
     tangent space of the corresponding SE3 element.
 
     This class is based on the implementation in `jaxlie.manifold`.
 
     **Attributes:**
 
     - `transformed_parameter`: The local tangent vector.
-
     - `group_element`: The element of SE3.
     """
 
     transformed_parameter: Float[Array, "6"]
     group_element: SE3
 
     def __init__(self, quaternion_pose: QuaternionPose):
@@ -119,13 +117,11 @@
             rotation=quaternion_pose.rotation,
             xyz=quaternion_pose.offset_in_angstroms,
         )
 
     def get(self) -> Float[Array, "6"]:
         """An implementation of the `jaxlie.manifold.rplus`."""
         local_tangent = self.transformed_parameter
-        group_element = jax.lax.stop_gradient(self.group_element) @ SE3.exp(
-            local_tangent
-        )
+        group_element = jax.lax.stop_gradient(self.group_element) @ SE3.exp(local_tangent)
         return QuaternionPose.from_rotation_and_translation(
             group_element.rotation, group_element.xyz
         )
```

### Comparing `cryojax-0.2.3rc1/src/cryojax/io/__init__.py` & `cryojax-0.3.0a0/src/cryojax/data/_io/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-from ._cif import read_atoms_from_cif as read_atoms_from_cif
-from ._gemmi import (
+from .cif import read_atoms_from_cif as read_atoms_from_cif
+from .gemmi import (
     clean_gemmi_structure as clean_gemmi_structure,
     extract_atom_positions_and_names as extract_atom_positions_and_names,
     extract_gemmi_atoms as extract_gemmi_atoms,
     get_atom_info_from_gemmi_model as get_atom_info_from_gemmi_model,
 )
-from ._mdtraj import (
+from .mdtraj import (
     get_atom_info_from_mdtraj as get_atom_info_from_mdtraj,
     mdtraj_load_from_file as mdtraj_load_from_file,
 )
-from ._mrc import (
+from .mrc import (
     read_array_from_mrc as read_array_from_mrc,
     read_array_with_spacing_from_mrc as read_array_with_spacing_from_mrc,
     write_image_stack_to_mrc as write_image_stack_to_mrc,
     write_image_to_mrc as write_image_to_mrc,
     write_volume_to_mrc as write_volume_to_mrc,
 )
-from ._pdb import read_atoms_from_pdb as read_atoms_from_pdb
-from ._starfile import read_and_validate_starfile as read_and_validate_starfile
+from .pdb import read_atoms_from_pdb as read_atoms_from_pdb
+from .starfile import read_and_validate_starfile as read_and_validate_starfile
```

### Comparing `cryojax-0.2.3rc1/src/cryojax/io/_cif.py` & `cryojax-0.3.0a0/src/cryojax/data/_io/cif.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import numpy as np
 from jaxtyping import Float, Int
 
-from ._gemmi import (
+from .gemmi import (
     clean_gemmi_structure,
     extract_atom_positions_and_names,
     extract_gemmi_atoms,
 )
 
 
 def read_atoms_from_cif(
```

### Comparing `cryojax-0.2.3rc1/src/cryojax/io/_gemmi.py` & `cryojax-0.3.0a0/src/cryojax/data/_io/gemmi.py`

 * *Files identical despite different names*

### Comparing `cryojax-0.2.3rc1/src/cryojax/io/_mdtraj.py` & `cryojax-0.3.0a0/src/cryojax/data/_io/mdtraj.py`

 * *Files identical despite different names*

### Comparing `cryojax-0.2.3rc1/src/cryojax/io/_mrc.py` & `cryojax-0.3.0a0/src/cryojax/data/_io/mrc.py`

 * *Files identical despite different names*

### Comparing `cryojax-0.2.3rc1/src/cryojax/io/_pdb.py` & `cryojax-0.3.0a0/src/cryojax/data/_io/pdb.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 Read and write atomic models in various formats.
 Large amounts of the code are adapted from the ioSPI package
 """
 
 import numpy as np
 from jaxtyping import Float, Int
 
-from ._gemmi import (
+from .gemmi import (
     clean_gemmi_structure,
     extract_atom_positions_and_names,
     extract_gemmi_atoms,
 )
 
 
 def read_atoms_from_pdb(
```

### Comparing `cryojax-0.2.3rc1/src/cryojax/io/_starfile.py` & `cryojax-0.3.0a0/src/cryojax/data/_io/starfile.py`

 * *Files identical despite different names*

### Comparing `cryojax-0.2.3rc1/src/cryojax/rotations/_lie_group.py` & `cryojax-0.3.0a0/src/cryojax/rotations/_lie_group.py`

 * *Files 2% similar despite different names*

```diff
@@ -102,17 +102,15 @@
                     x0 * y1 - y0 * x1 + z0 * w1 + w0 * z1,
                 ]
             )
         )
 
     def inverse(self) -> Self:
         # Negate complex terms.
-        return eqx.tree_at(
-            lambda R: R.wxyz, self, self.wxyz * jnp.array([1, -1, -1, -1])
-        )
+        return eqx.tree_at(lambda R: R.wxyz, self, self.wxyz * jnp.array([1, -1, -1, -1]))
 
     @classmethod
     def from_x_radians(cls, angle: Float[Array, ""]) -> Self:
         """Generates a x-axis rotation."""
         return cls.exp(jnp.asarray([angle, 0.0, 0.0]))
 
     @classmethod
@@ -302,17 +300,15 @@
         """Computes the adjoint, which transforms tangent vectors
         between tangent spaces.
         """
         return self.as_matrix()
 
     @override
     def normalize(self) -> Self:
-        return eqx.tree_at(
-            lambda R: R.wxyz, self, self.wxyz / jnp.linalg.norm(self.wxyz)
-        )
+        return eqx.tree_at(lambda R: R.wxyz, self, self.wxyz / jnp.linalg.norm(self.wxyz))
 
     @classmethod
     def sample_uniform(cls, key: PRNGKeyArray) -> Self:
         # Uniformly sample over S^3.
         # > Reference: http://planning.cs.uiuc.edu/node198.html
         u1, u2, u3 = jax.random.uniform(
             key=key,
```

### Comparing `cryojax-0.2.3rc1/src/cryojax/rotations/_rotation.py` & `cryojax-0.3.0a0/src/cryojax/rotations/_rotation.py`

 * *Files identical despite different names*

### Comparing `cryojax-0.2.3rc1/src/cryojax/simulator/__init__.py` & `cryojax-0.3.0a0/src/cryojax/simulator/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,66 +1,72 @@
 from ._assembly import (
     AbstractAssembly as AbstractAssembly,
     compute_helical_lattice_positions as compute_helical_lattice_positions,
     compute_helical_lattice_rotations as compute_helical_lattice_rotations,
-    Helix as Helix,
-)
-from ._config import ImageConfig as ImageConfig
-from ._conformation import (
-    AbstractConformation as AbstractConformation,
-    DiscreteConformation as DiscreteConformation,
+    HelicalAssembly as HelicalAssembly,
 )
 from ._detector import (
     AbstractDetector as AbstractDetector,
     AbstractDQE as AbstractDQE,
     GaussianDetector as GaussianDetector,
+    IdealCountingDQE as IdealCountingDQE,
     IdealDQE as IdealDQE,
     PoissonDetector as PoissonDetector,
 )
-from ._dose import ElectronDose as ElectronDose
-from ._ice import (
-    AbstractIce as AbstractIce,
-    GaussianIce as GaussianIce,
-)
-from ._instrument import Instrument as Instrument
-from ._integrators import (
-    AbstractPotentialIntegrator as AbstractPotentialIntegrator,
-    extract_slice as extract_slice,
-    extract_slice_with_cubic_spline as extract_slice_with_cubic_spline,
-    FourierSliceExtract as FourierSliceExtract,
-    NufftProject as NufftProject,
-    project_with_nufft as project_with_nufft,
-)
-from ._optics import (
-    AbstractOptics as AbstractOptics,
-    CTF as CTF,
-    WeakPhaseOptics as WeakPhaseOptics,
-)
-from ._pipeline import (
-    AbstractPipeline as AbstractPipeline,
-    AssemblyPipeline as AssemblyPipeline,
-    ImagePipeline as ImagePipeline,
+from ._imaging_pipeline import (
+    AbstractImagingPipeline as AbstractImagingPipeline,
+    ContrastImagingPipeline as ContrastImagingPipeline,
+    ElectronCountingImagingPipeline as ElectronCountingImagingPipeline,
+    IntensityImagingPipeline as IntensityImagingPipeline,
 )
+from ._instrument_config import InstrumentConfig as InstrumentConfig
 from ._pose import (
     AbstractPose as AbstractPose,
     AxisAnglePose as AxisAnglePose,
     EulerAnglePose as EulerAnglePose,
     QuaternionPose as QuaternionPose,
 )
-from ._potential import (
+from ._potential_integrator import (
+    AbstractFourierVoxelExtraction as AbstractFourierVoxelExtraction,
+    AbstractPotentialIntegrator as AbstractPotentialIntegrator,
+    AbstractVoxelPotentialIntegrator as AbstractVoxelPotentialIntegrator,
+    FourierSliceExtraction as FourierSliceExtraction,
+    NufftProjection as NufftProjection,
+)
+from ._potential_representation import (
     AbstractFourierVoxelGridPotential as AbstractFourierVoxelGridPotential,
-    AbstractScatteringPotential as AbstractScatteringPotential,
+    AbstractPotentialRepresentation as AbstractPotentialRepresentation,
     AbstractVoxelPotential as AbstractVoxelPotential,
     build_real_space_voxels_from_atoms as build_real_space_voxels_from_atoms,
     evaluate_3d_atom_potential as evaluate_3d_atom_potential,
     evaluate_3d_real_space_gaussian as evaluate_3d_real_space_gaussian,
     FourierVoxelGridPotential as FourierVoxelGridPotential,
     FourierVoxelGridPotentialInterpolator as FourierVoxelGridPotentialInterpolator,
     RealVoxelCloudPotential as RealVoxelCloudPotential,
     RealVoxelGridPotential as RealVoxelGridPotential,
 )
-from ._specimen import (
-    AbstractEnsemble as AbstractEnsemble,
-    AbstractSpecimen as AbstractSpecimen,
-    DiscreteEnsemble as DiscreteEnsemble,
-    Specimen as Specimen,
+from ._scattering_theory import (
+    AbstractLinearScatteringTheory as AbstractLinearScatteringTheory,
+    AbstractScatteringTheory as AbstractScatteringTheory,
+    LinearScatteringTheory as LinearScatteringTheory,
+    LinearSuperpositionScatteringTheory as LinearSuperpositionScatteringTheory,
+)
+from ._solvent import (
+    AbstractIce as AbstractIce,
+    GaussianIce as GaussianIce,
+)
+from ._structural_ensemble import (
+    AbstractConformationalVariable as AbstractConformationalVariable,
+    AbstractStructuralEnsemble as AbstractStructuralEnsemble,
+    AbstractStructuralEnsembleBatcher as AbstractStructuralEnsembleBatcher,
+    DiscreteConformationalVariable as DiscreteConformationalVariable,
+    DiscreteStructuralEnsemble as DiscreteStructuralEnsemble,
+    SingleStructureEnsemble as SingleStructureEnsemble,
+)
+from ._transfer_theory import (
+    AbstractContrastTransferFunction as AbstractContrastTransferFunction,
+    AbstractTransferFunction as AbstractTransferFunction,
+    AbstractTransferTheory as AbstractTransferTheory,
+    ContrastTransferFunction as ContrastTransferFunction,
+    ContrastTransferTheory as ContrastTransferTheory,
+    IdealContrastTransferFunction as IdealContrastTransferFunction,
 )
```

### Comparing `cryojax-0.2.3rc1/src/cryojax/simulator/_detector.py` & `cryojax-0.3.0a0/src/cryojax/simulator/_detector.py`

 * *Files 22% similar despite different names*

```diff
@@ -8,18 +8,18 @@
 
 import jax.numpy as jnp
 import jax.random as jr
 import numpy as np
 from equinox import AbstractVar, field, Module
 from jaxtyping import Array, Complex, Float, PRNGKeyArray
 
-from ..core import error_if_not_fractional
+from .._errors import error_if_not_fractional
 from ..image import irfftn, rfftn
 from ..image.operators import AbstractFourierOperator
-from ._config import ImageConfig
+from ._instrument_config import InstrumentConfig
 
 
 class AbstractDQE(AbstractFourierOperator, strict=True):
     r"""Base class for a detector DQE."""
 
     fraction_detected_electrons: AbstractVar[Float[Array, ""]]
 
@@ -38,16 +38,16 @@
                                                    in angstroms, `pixel_size`
                                                    must be passed
         - `pixel_size`: The pixel size of `frequency_grid_in_angstroms_or_pixels`.
         """
         raise NotImplementedError
 
 
-class IdealDQE(AbstractDQE, strict=True):
-    r"""The model for an ideal DQE.
+class IdealCountingDQE(AbstractDQE, strict=True):
+    r"""A perfect DQE for a detector at a discrete pixel size.
 
     See Ruskin et. al. "Quantitative characterization of electron detectors for
     transmission electron microscopy." (2013) for details.
     """
 
     fraction_detected_electrons: Float[Array, ""] = field(
         default=1.0, converter=error_if_not_fractional
@@ -57,57 +57,121 @@
     def __call__(
         self,
         frequency_grid_in_angstroms_or_pixels: Float[Array, "y_dim x_dim 2"],
         *,
         pixel_size: Optional[Float[Array, ""]] = None,
     ) -> Float[Array, "y_dim x_dim"]:
         if pixel_size is None:
-            frequency_grid_in_nyquist_units = (
-                frequency_grid_in_angstroms_or_pixels / 0.5
-            )
+            frequency_grid_in_nyquist_units = frequency_grid_in_angstroms_or_pixels / 0.5
         else:
             frequency_grid_in_nyquist_units = (
                 frequency_grid_in_angstroms_or_pixels * pixel_size
             ) / 0.5
         return (
             self.fraction_detected_electrons**2
             * jnp.sinc(frequency_grid_in_nyquist_units[..., 0] / 2) ** 2
             * jnp.sinc(frequency_grid_in_nyquist_units[..., 1] / 2) ** 2
         )
 
 
+class IdealDQE(AbstractDQE, strict=True):
+    r"""A DQE that is perfect across all spatial frequencies."""
+
+    fraction_detected_electrons: Float[Array, ""] = field(
+        default=1.0, converter=error_if_not_fractional
+    )
+
+    @override
+    def __call__(
+        self,
+        frequency_grid_in_angstroms_or_pixels: Float[Array, "y_dim x_dim 2"],
+        *,
+        pixel_size: Optional[Float[Array, ""]] = None,
+    ) -> Float[Array, "y_dim x_dim"]:
+        return jnp.full(
+            frequency_grid_in_angstroms_or_pixels.shape[0:2],
+            self.fraction_detected_electrons,
+        )
+
+
 class AbstractDetector(Module, strict=True):
     """Base class for an electron detector."""
 
     dqe: AbstractDQE
 
     def __init__(self, dqe: AbstractDQE):
         self.dqe = dqe
 
     @abstractmethod
-    def sample(
+    def sample_readout_from_expected_events(
         self, key: PRNGKeyArray, expected_electron_events: Float[Array, "y_dim x_dim"]
     ) -> Float[Array, "y_dim x_dim"]:
         """Sample a realization from the detector noise model."""
         raise NotImplementedError
 
-    def __call__(
+    def compute_expected_electron_events(
+        self,
+        fourier_squared_wavefunction_at_detector_plane: Complex[
+            Array,
+            "{instrument_config.padded_y_dim} {instrument_config.padded_x_dim//2+1}",
+        ],
+        instrument_config: InstrumentConfig,
+    ) -> Complex[
+        Array, "{instrument_config.padded_y_dim} {instrument_config.padded_x_dim//2+1}"
+    ]:
+        """Compute the expected electron events from the detector."""
+        fourier_expected_electron_events = (
+            self._compute_expected_events_or_detector_readout(
+                fourier_squared_wavefunction_at_detector_plane,
+                instrument_config,
+                key=None,
+            )
+        )
+
+        return fourier_expected_electron_events
+
+    def compute_detector_readout(
         self,
+        key: PRNGKeyArray,
         fourier_squared_wavefunction_at_detector_plane: Complex[
-            Array, "{config.padded_y_dim} {config.padded_x_dim//2+1}"
+            Array,
+            "{instrument_config.padded_y_dim} {instrument_config.padded_x_dim//2+1}",
         ],
-        config: ImageConfig,
-        electrons_per_angstrom_squared: Float[Array, ""],
+        instrument_config: InstrumentConfig,
+    ) -> Complex[
+        Array, "{instrument_config.padded_y_dim} {instrument_config.padded_x_dim//2+1}"
+    ]:
+        """Measure the readout from the detector."""
+        fourier_detector_readout = self._compute_expected_events_or_detector_readout(
+            fourier_squared_wavefunction_at_detector_plane,
+            instrument_config,
+            key,
+        )
+
+        return fourier_detector_readout
+
+    def _compute_expected_events_or_detector_readout(
+        self,
+        fourier_squared_wavefunction_at_detector_plane: Complex[
+            Array,
+            "{instrument_config.padded_y_dim} {instrument_config.padded_x_dim//2+1}",
+        ],
+        instrument_config: InstrumentConfig,
         key: Optional[PRNGKeyArray] = None,
-    ) -> Complex[Array, "{config.padded_y_dim} {config.padded_x_dim//2+1}"]:
+    ) -> Complex[
+        Array, "{instrument_config.padded_y_dim} {instrument_config.padded_x_dim//2+1}"
+    ]:
         """Pass the image through the detector model."""
-        N_pix = np.prod(config.padded_shape)
-        frequency_grid = config.wrapped_padded_frequency_grid_in_pixels.get()
+        N_pix = np.prod(instrument_config.padded_shape)
+        frequency_grid = instrument_config.wrapped_padded_frequency_grid_in_pixels.get()
         # Compute the time-integrated electron flux in pixels
-        electrons_per_pixel = electrons_per_angstrom_squared * config.pixel_size**2
+        electrons_per_pixel = (
+            instrument_config.electrons_per_angstrom_squared
+            * instrument_config.pixel_size**2
+        )
         # ... now the total number of electrons over the entire image
         electrons_per_image = N_pix * electrons_per_pixel
         # Normalize the squared wavefunction to a set of probabilities
         fourier_squared_wavefunction_at_detector_plane /= (
             fourier_squared_wavefunction_at_detector_plane[0, 0]
         )
         # Compute the noiseless signal by applying the DQE to the squared wavefunction
@@ -119,34 +183,36 @@
         if key is None:
             # If there is no key given, return
             return fourier_expected_electron_events
         else:
             # ... otherwise, go to real space, sample, go back to fourier,
             # and return.
             expected_electron_events = irfftn(
-                fourier_expected_electron_events, s=config.padded_shape
+                fourier_expected_electron_events, s=instrument_config.padded_shape
+            )
+            return rfftn(
+                self.sample_readout_from_expected_events(key, expected_electron_events)
             )
-            return rfftn(self.sample(key, expected_electron_events))
 
 
 class GaussianDetector(AbstractDetector, strict=True):
     """A detector with a gaussian noise model. This is the gaussian limit
     of `PoissonDetector`.
     """
 
     @override
-    def sample(
+    def sample_readout_from_expected_events(
         self, key: PRNGKeyArray, expected_electron_events: Float[Array, "y_dim x_dim"]
     ) -> Float[Array, "y_dim x_dim"]:
-        return expected_electron_events + jnp.sqrt(
-            expected_electron_events
-        ) * jr.normal(key, expected_electron_events.shape)
+        return expected_electron_events + jnp.sqrt(expected_electron_events) * jr.normal(
+            key, expected_electron_events.shape
+        )
 
 
 class PoissonDetector(AbstractDetector, strict=True):
     """A detector with a poisson noise model."""
 
     @override
-    def sample(
+    def sample_readout_from_expected_events(
         self, key: PRNGKeyArray, expected_electron_events: Float[Array, "y_dim x_dim"]
     ) -> Float[Array, "y_dim x_dim"]:
         return jr.poisson(key, expected_electron_events).astype(float)
```

### Comparing `cryojax-0.2.3rc1/src/cryojax/simulator/_optics.py` & `cryojax-0.3.0a0/src/cryojax/simulator/_transfer_theory/contrast_transfer_theory.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,41 +1,49 @@
-"""
-Models of instrument optics.
-"""
-
 from abc import abstractmethod
-from typing import ClassVar, Optional
+from typing import Optional
 from typing_extensions import override
 
 import jax.numpy as jnp
-from equinox import AbstractClassVar, AbstractVar, field, Module
+from equinox import field
 from jaxtyping import Array, Complex, Float
 
-from ..constants import convert_keV_to_angstroms
-from ..coordinates import cartesian_to_polar
-from ..core import error_if_negative, error_if_not_fractional, error_if_not_positive
-from ..image.operators import (
-    AbstractFourierOperator,
+from ..._errors import error_if_negative, error_if_not_fractional, error_if_not_positive
+from ...constants import convert_keV_to_angstroms
+from ...image.operators import (
     Constant,
     FourierOperatorLike,
 )
-from ._config import ImageConfig
+from .._instrument_config import InstrumentConfig
+from .base_transfer_theory import AbstractTransferFunction, AbstractTransferTheory
+from .common_functions import compute_phase_shifts_with_amplitude_contrast_ratio
 
 
-class CTF(AbstractFourierOperator, strict=True):
-    """Compute the Contrast Transfer Function (CTF) in for a weakly
-    scattering specimen.
+class AbstractContrastTransferFunction(AbstractTransferFunction, strict=True):
+    """An abstract base class for a transfer function."""
+
+    @abstractmethod
+    def __call__(
+        self,
+        frequency_grid_in_angstroms: Float[Array, "y_dim x_dim 2"],
+        *,
+        wavelength_in_angstroms: Optional[Float[Array, ""] | float] = None,
+        defocus_offset: Float[Array, ""] | float = 0.0,
+    ) -> Float[Array, "y_dim x_dim"]:
+        raise NotImplementedError
+
+
+class ContrastTransferFunction(AbstractContrastTransferFunction, strict=True):
+    """Compute an astigmatic Contrast Transfer Function (CTF) with a
+    spherical aberration correction and amplitude contrast ratio.
     """
 
-    defocus_u_in_angstroms: Float[Array, ""] = field(
-        default=10000.0, converter=error_if_not_positive
-    )
-    defocus_v_in_angstroms: Float[Array, ""] = field(
+    defocus_in_angstroms: Float[Array, ""] = field(
         default=10000.0, converter=error_if_not_positive
     )
+    astigmatism_in_angstroms: Float[Array, ""] = field(default=0.0, converter=jnp.asarray)
     astigmatism_angle: Float[Array, ""] = field(default=0.0, converter=jnp.asarray)
     voltage_in_kilovolts: Float[Array, ""] | float = field(
         default=300.0, static=True
     )  # Mark `static=True` so that the voltage is not part of the model pytree
     # It is treated as part of the pytree upstream, in the Instrument!
     spherical_aberration_in_mm: Float[Array, ""] = field(
         default=2.7, converter=error_if_negative
@@ -61,147 +69,107 @@
         # CTF
         if wavelength_in_angstroms is None:
             wavelength_in_angstroms = convert_keV_to_angstroms(
                 jnp.asarray(self.voltage_in_kilovolts)
             )
         else:
             wavelength_in_angstroms = jnp.asarray(wavelength_in_angstroms)
+        defocus_axis_1_in_angstroms = self.defocus_in_angstroms + jnp.asarray(
+            defocus_offset
+        )
+        defocus_axis_2_in_angstroms = (
+            self.defocus_in_angstroms
+            + self.astigmatism_in_angstroms
+            + jnp.asarray(defocus_offset)
+        )
         # Compute phase shifts for CTF
-        phase_shifts = _compute_phase_shifts(
+        phase_shifts = compute_phase_shifts_with_amplitude_contrast_ratio(
             frequency_grid_in_angstroms,
-            self.defocus_u_in_angstroms + jnp.asarray(defocus_offset),
-            self.defocus_v_in_angstroms + jnp.asarray(defocus_offset),
+            defocus_axis_1_in_angstroms,
+            defocus_axis_2_in_angstroms,
             astigmatism_angle,
             wavelength_in_angstroms,
             spherical_aberration_in_angstroms,
-            self.amplitude_contrast_ratio,
             phase_shift,
+            self.amplitude_contrast_ratio,
         )
         # Compute the CTF
         return jnp.sin(phase_shifts).at[0, 0].set(0.0)
 
 
-CTF.__init__.__doc__ = """**Arguments:**
+ContrastTransferFunction.__init__.__doc__ = """**Arguments:**
 
 - `defocus_u_in_angstroms`: The major axis defocus in Angstroms.
 - `defocus_v_in_angstroms`: The minor axis defocus in Angstroms.
 - `astigmatism_angle`: The defocus angle.
 - `voltage_in_kilovolts`: The accelerating voltage in kV.
 - `spherical_aberration_in_mm`: The spherical aberration coefficient in mm.
 - `amplitude_contrast_ratio`: The amplitude contrast ratio.
 - `phase_shift`: The additional phase shift.
 """
 
 
-class AbstractOptics(Module, strict=True):
-    """Base class for an optics model."""
-
-    ctf: AbstractVar[CTF]
-    envelope: AbstractVar[FourierOperatorLike]
-
-    is_linear: AbstractClassVar[bool]
-
-    @property
-    def wavelength_in_angstroms(self) -> Float[Array, ""]:
-        return self.ctf.wavelength_in_angstroms
+class IdealContrastTransferFunction(AbstractContrastTransferFunction, strict=True):
+    """Compute a perfect CTF, where frequency content is delivered equally
+    over all frequencies.
+    """
 
-    @abstractmethod
     def __call__(
         self,
-        fourier_phase_in_exit_plane: Complex[
-            Array, "{config.padded_y_dim} {config.padded_x_dim//2+1}"
-        ],
-        config: ImageConfig,
-        wavelength_in_angstroms: Float[Array, ""] | float,
+        frequency_grid_in_angstroms: Float[Array, "y_dim x_dim 2"],
+        *,
+        wavelength_in_angstroms: Optional[Float[Array, ""] | float] = None,
         defocus_offset: Float[Array, ""] | float = 0.0,
-    ) -> (
-        Complex[Array, "{config.padded_y_dim} {config.padded_x_dim//2+1}"]
-        | Complex[Array, "{config.padded_y_dim} {config.padded_x_dim}"]
-    ):
-        """Pass an image through the optics model."""
-        raise NotImplementedError
+    ) -> Float[Array, "y_dim x_dim"]:
+        return jnp.ones(frequency_grid_in_angstroms.shape[0:2])
 
 
-class WeakPhaseOptics(AbstractOptics, strict=True):
+class ContrastTransferTheory(AbstractTransferTheory, strict=True):
     """An optics model in the weak-phase approximation. Here, compute the image
     contrast by applying the CTF directly to the exit plane phase shifts.
     """
 
-    ctf: CTF
+    ctf: AbstractContrastTransferFunction
     envelope: FourierOperatorLike
 
-    is_linear: ClassVar[bool] = True
-
     def __init__(
         self,
-        ctf: CTF,
+        ctf: AbstractContrastTransferFunction,
         envelope: Optional[FourierOperatorLike] = None,
     ):
         self.ctf = ctf
         self.envelope = envelope or Constant(1.0)
 
     @override
     def __call__(
         self,
-        fourier_phase_in_exit_plane: Complex[
-            Array, "{config.padded_y_dim} {config.padded_x_dim//2+1}"
+        fourier_phase_at_exit_plane: Complex[
+            Array,
+            "{instrument_config.padded_y_dim} {instrument_config.padded_x_dim//2+1}",
         ],
-        config: ImageConfig,
-        wavelength_in_angstroms: Float[Array, ""] | float,
+        instrument_config: InstrumentConfig,
         defocus_offset: Float[Array, ""] | float = 0.0,
-    ) -> Complex[Array, "{config.padded_y_dim} {config.padded_x_dim//2+1}"]:
+    ) -> Complex[
+        Array, "{instrument_config.padded_y_dim} {instrument_config.padded_x_dim//2+1}"
+    ]:
         """Apply the CTF directly to the phase shifts in the exit plane."""
-        frequency_grid = config.wrapped_padded_frequency_grid_in_angstroms.get()
+        frequency_grid = (
+            instrument_config.wrapped_padded_frequency_grid_in_angstroms.get()
+        )
         # Compute the CTF
-        ctf = self.envelope(frequency_grid) * self.ctf(
+        ctf_array = self.envelope(frequency_grid) * self.ctf(
             frequency_grid,
-            wavelength_in_angstroms=wavelength_in_angstroms,
+            wavelength_in_angstroms=instrument_config.wavelength_in_angstroms,
             defocus_offset=defocus_offset,
         )
         # ... compute the contrast as the CTF multiplied by the exit plane
         # phase shifts
-        fourier_contrast_in_detector_plane = ctf * fourier_phase_in_exit_plane
+        fourier_contrast_at_detector_plane = ctf_array * fourier_phase_at_exit_plane
 
-        return fourier_contrast_in_detector_plane
+        return fourier_contrast_at_detector_plane
 
 
-WeakPhaseOptics.__init__.__doc__ = """**Arguments:**
+ContrastTransferTheory.__init__.__doc__ = """**Arguments:**
 
 - `ctf`: The contrast transfer function model.
 - `envelope`: The envelope function of the optics model.
 """
-
-
-def _compute_phase_shifts(
-    frequency_grid_in_angstroms: Float[Array, "y_dim x_dim 2"],
-    defocus_u_in_angstroms: Float[Array, ""],
-    defocus_v_in_angstroms: Float[Array, ""],
-    astigmatism_angle: Float[Array, ""],
-    wavelength_in_angstroms: Float[Array, ""],
-    spherical_aberration_in_angstroms: Float[Array, ""],
-    amplitude_contrast_ratio: Float[Array, ""],
-    phase_shift: Float[Array, ""],
-) -> Float[Array, "y_dim x_dim"]:
-    k_sqr, azimuth = cartesian_to_polar(frequency_grid_in_angstroms, square=True)
-    defocus = 0.5 * (
-        defocus_u_in_angstroms
-        + defocus_v_in_angstroms
-        + (defocus_u_in_angstroms - defocus_v_in_angstroms)
-        * jnp.cos(2.0 * (azimuth - astigmatism_angle))
-    )
-    amplitude_contrast_phase_shifts = jnp.arctan(
-        amplitude_contrast_ratio / jnp.sqrt(1.0 - amplitude_contrast_ratio**2)
-    )
-    defocus_phase_shifts = -0.5 * defocus * wavelength_in_angstroms * k_sqr
-    aberration_phase_shifts = (
-        0.25
-        * spherical_aberration_in_angstroms
-        * (wavelength_in_angstroms**3)
-        * (k_sqr**2)
-    )
-    phase_shifts = (
-        (2 * jnp.pi) * (defocus_phase_shifts + aberration_phase_shifts)
-        - phase_shift
-        - amplitude_contrast_phase_shifts
-    )
-
-    return phase_shifts
```

### Comparing `cryojax-0.2.3rc1/src/cryojax/simulator/_pose.py` & `cryojax-0.3.0a0/src/cryojax/simulator/_pose.py`

 * *Files 20% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 import equinox as eqx
 import jax
 import jax.numpy as jnp
 from equinox import AbstractVar, field, Module
 from jaxtyping import Array, Complex, Float
 
-from ..rotations import SO3
+from ..rotations import convert_quaternion_to_euler_angles, SO3
 
 
 class AbstractPose(Module, strict=True):
     """Base class for the image pose.
 
     Subclasses should choose a viewing convention,
     such as with Euler angles or Quaternions. In particular,
@@ -43,17 +43,15 @@
     @overload
     def rotate_coordinates(
         self, volume_coordinates: Float[Array, "size 3"], inverse: bool = False
     ) -> Float[Array, "size 3"]: ...
 
     def rotate_coordinates(
         self,
-        volume_coordinates: (
-            Float[Array, "z_dim y_dim x_dim 3"] | Float[Array, "size 3"]
-        ),
+        volume_coordinates: Float[Array, "z_dim y_dim x_dim 3"] | Float[Array, "size 3"],
         inverse: bool = False,
     ) -> Float[Array, "z_dim y_dim x_dim 3"] | Float[Array, "size 3"]:
         """Rotate coordinates from a particular convention."""
         rotation = self.rotation.inverse() if inverse else self.rotation
         if isinstance(volume_coordinates, Float[Array, "size 3"]):  # type: ignore
             rotated_volume_coordinates = jax.vmap(rotation.apply)(volume_coordinates)
         elif isinstance(volume_coordinates, Float[Array, "z_dim y_dim x_dim 3"]):  # type: ignore
@@ -71,17 +69,15 @@
     def compute_shifts(
         self, frequency_grid_in_angstroms: Float[Array, "y_dim x_dim 2"]
     ) -> Complex[Array, "y_dim x_dim"]:
         """Compute the phase shifts from the in-plane translation,
         given a frequency grid coordinate system.
         """
         xy = self.offset_in_angstroms[0:2]
-        return jnp.exp(
-            -1.0j * (2 * jnp.pi * jnp.matmul(frequency_grid_in_angstroms, xy))
-        )
+        return jnp.exp(-1.0j * (2 * jnp.pi * jnp.matmul(frequency_grid_in_angstroms, xy)))
 
     @cached_property
     def offset_in_angstroms(self) -> Float[Array, "3"]:
         """The translation vector, relative to the center of the in-plane
         (x, y) coordinates and relative to the configured defocus in the
         out-of-plane z coordinate.
         """
@@ -159,15 +155,15 @@
             SO3.from_z_radians(psi),
         )
         return R3 @ R2 @ R1
 
     @override
     @classmethod
     def from_rotation(cls, rotation: SO3):
-        view_phi, view_theta, view_psi = _convert_quaternion_to_euler_angles(
+        view_phi, view_theta, view_psi = convert_quaternion_to_euler_angles(
             rotation.wxyz,
             "zyz",
         )
         return cls(view_phi=view_phi, view_theta=view_theta, view_psi=view_psi)
 
 
 EulerAnglePose.__init__.__doc__ = """**Arguments:**
@@ -261,66 +257,7 @@
 - `offset_y_in_angstroms` : In-plane translation in y direction.
 - `offset_z_in_angstroms` : Out-of-plane translation in the z
                             direction. The translation is measured
                             relative to the configured defocus.
 - `euler_vector`: The axis-angle parameterization, represented as a
                   vector $\boldsymbol{\omega} = (\omega_x, \omega_y, \omega_z)$.
 """
-
-
-def _convert_quaternion_to_euler_angles(
-    wxyz: jax.Array, convention: str = "zyz"
-) -> jax.Array:
-    """Convert a quaternion to a sequence of euler angles about an extrinsic
-    coordinate system.
-
-    Adapted from https://github.com/chrisflesher/jax-scipy-spatial/.
-    """
-    if len(convention) != 3 or not all(
-        [axis in ["x", "y", "z"] for axis in convention]
-    ):
-        raise ValueError(
-            f"`convention` should be a string of three characters, each "
-            f"of which is 'x', 'y', or 'z'. Instead, got '{convention}'"
-        )
-    if convention[0] == convention[1] or convention[1] == convention[2]:
-        raise ValueError(
-            f"`convention` cannot have axes repeating in a row. For example, "
-            f"'xxy' or 'zzz' are not allowed. Got '{convention}'."
-        )
-    xyz_axis_to_array_axis = {"x": 0, "y": 1, "z": 2}
-    axes = [xyz_axis_to_array_axis[axis] for axis in convention]
-    xyzw = jnp.roll(wxyz, shift=-1)
-    angle_first = 0
-    angle_third = 2
-    i = axes[0]
-    j = axes[1]
-    k = axes[2]
-    symmetric = i == k
-    k = jnp.where(symmetric, 3 - i - j, k)
-    sign = jnp.array((i - j) * (j - k) * (k - i) // 2, dtype=xyzw.dtype)
-    eps = 1e-7
-    a = jnp.where(symmetric, xyzw[3], xyzw[3] - xyzw[j])
-    b = jnp.where(symmetric, xyzw[i], xyzw[i] + xyzw[k] * sign)
-    c = jnp.where(symmetric, xyzw[j], xyzw[j] + xyzw[3])
-    d = jnp.where(symmetric, xyzw[k] * sign, xyzw[k] * sign - xyzw[i])
-    angles = jnp.empty(3, dtype=xyzw.dtype)
-    angles = angles.at[1].set(2 * jnp.arctan2(jnp.hypot(c, d), jnp.hypot(a, b)))
-    case = jnp.where(jnp.abs(angles[1] - jnp.pi) <= eps, 2, 0)
-    case = jnp.where(jnp.abs(angles[1]) <= eps, 1, case)
-    half_sum = jnp.arctan2(b, a)
-    half_diff = jnp.arctan2(d, c)
-    angles = angles.at[0].set(
-        jnp.where(case == 1, 2 * half_sum, 2 * half_diff * -1)
-    )  # any degenerate case
-    angles = angles.at[angle_first].set(
-        jnp.where(case == 0, half_sum - half_diff, angles[angle_first])
-    )
-    angles = angles.at[angle_third].set(
-        jnp.where(case == 0, half_sum + half_diff, angles[angle_third])
-    )
-    angles = angles.at[angle_third].set(
-        jnp.where(symmetric, angles[angle_third], angles[angle_third] * sign)
-    )
-    angles = angles.at[1].set(jnp.where(symmetric, angles[1], angles[1] - jnp.pi / 2))
-    angles = (angles + jnp.pi) % (2 * jnp.pi) - jnp.pi
-    return -jnp.rad2deg(angles)
```

### Comparing `cryojax-0.2.3rc1/src/cryojax/simulator/_assembly/_assembly.py` & `cryojax-0.3.0a0/src/cryojax/simulator/_assembly/assembly.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,57 +1,55 @@
 """
 Abstraction of a biological assembly. This assembles a structure
-by computing an Ensemble of subunits, parameterized by
-some geometry.
+by computing a batch of subunits, parameterized by some geometry.
 """
 
 from abc import abstractmethod
 from functools import cached_property
 from typing import Optional
+from typing_extensions import override
 
 import equinox as eqx
 import jax
 from equinox import AbstractVar
 from jaxtyping import Array, Float
 
 from ...rotations import SO3
-from .._conformation import AbstractConformation
 from .._pose import AbstractPose
-from .._specimen import AbstractEnsemble, AbstractSpecimen
+from .._structural_ensemble import (
+    AbstractConformationalVariable,
+    AbstractStructuralEnsemble,
+    AbstractStructuralEnsembleBatcher,
+)
 
 
-class AbstractAssembly(eqx.Module, strict=True):
+class AbstractAssembly(AbstractStructuralEnsembleBatcher, strict=True):
     """Abstraction of a biological assembly.
 
-    This class acts just like an ``AbstractSpecimen``, however
-    it creates an assembly from a subunit.
-
     To subclass an `AbstractAssembly`,
         1) Overwrite the `AbstractAssembly.n_subunits`
            property
         2) Overwrite the `AbstractAssembly.positions`
            and `AbstractAssembly.rotations` properties.
     """
 
-    subunit: AbstractVar[AbstractSpecimen]
+    subunit: AbstractVar[AbstractStructuralEnsemble]
     pose: AbstractVar[AbstractPose]
-    conformation: AbstractVar[Optional[AbstractConformation]]
+    conformation: AbstractVar[Optional[AbstractConformationalVariable]]
 
     n_subunits: AbstractVar[int]
 
     def __check_init__(self):
-        if self.conformation is not None and not isinstance(
-            self.subunit, AbstractEnsemble
-        ):
+        if self.conformation is not None and self.subunit.conformation is None:
             # Make sure that if conformation is set, subunit is an AbstractEnsemble
             raise AttributeError(
-                f"If {type(self)}.conformation is set, {type(self)}.subunit must be an "
-                "AbstractEnsemble."
+                f"If {type(self)}.conformation is set, "
+                "{type(self)}.subunit.conformation cannot be `None`."
             )
-        if self.conformation is not None and isinstance(self.subunit, AbstractEnsemble):
+        if self.conformation is not None and self.subunit.conformation is not None:
             # ... if it is an AbstractEnsemble, the AbstractConformation must be the
             #  right type
             if not isinstance(self.conformation, type(self.subunit.conformation)):
                 raise AttributeError(
                     f"{type(self)}.conformation must be type "
                     f" {type(self.subunit.conformation)} if {type(self)}.subunit is "
                     f"type {type(self.subunit)}."
@@ -71,37 +69,41 @@
 
     @cached_property
     def poses(self) -> AbstractPose:
         """
         Draw the poses of the subunits in the lab frame, measured
         from the rotation relative to the first subunit.
         """
-        # Transform the subunit positions by pose of the helix
+        # Transform the subunit positions by the center of mass pose of the assembly.
         transformed_positions = (
             self.pose.rotate_coordinates(self.offsets_in_angstroms, inverse=False)
             + self.pose.offset_in_angstroms
         )
-        # Transform the subunit rotations by the pose of the helix. This operation
-        # left multiplies by the pose of the helix, taking care that first subunits
-        # are rotated to the center of mass frame, then the lab frame.
+        # Transform the subunit rotations by the center of mass pose of the assembly.
+        # This operation left multiplies by the pose rotation matrix, taking care that
+        # first subunits are rotated to the center of mass frame, then the lab frame.
         transformed_rotations = jax.vmap(
             lambda com_rotation, subunit_rotation: com_rotation @ subunit_rotation,
             in_axes=[None, 0],
         )(self.pose.rotation, self.rotations)
-        # Function to construct AbstractPoses
+        # Construct the batch of `AbstractPose`s
         cls = type(self.pose)
         make_assembly_poses = jax.vmap(
             lambda rot, pos: cls.from_rotation_and_translation(rot, pos)
         )
 
         return make_assembly_poses(transformed_rotations, transformed_positions)
 
     @cached_property
-    def subunits(self) -> AbstractSpecimen:
+    def subunits(self) -> AbstractStructuralEnsemble:
         """Draw a realization of all of the subunits in the lab frame."""
         # Compute a list of subunits, configured at the correct conformations
-        if isinstance(self.subunit, AbstractEnsemble):
+        if self.subunit.conformation is not None:
             where = lambda s: (s.conformation, s.pose)
             return eqx.tree_at(where, self.subunit, (self.conformation, self.poses))
         else:
             where = lambda s: s.pose
             return eqx.tree_at(where, self.subunit, self.poses)
+
+    @override
+    def get_batched_structural_ensemble(self) -> AbstractStructuralEnsemble:
+        return self.subunits
```

### Comparing `cryojax-0.2.3rc1/src/cryojax/simulator/_assembly/_helix.py` & `cryojax-0.3.0a0/src/cryojax/simulator/_assembly/helix.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,52 +3,53 @@
 """
 
 from functools import cached_property
 from typing import Optional
 
 import jax
 import jax.numpy as jnp
-from equinox import field
 from jaxtyping import Array, Float
 
 from ...rotations import SO3
-from .._conformation import AbstractConformation
 from .._pose import AbstractPose, EulerAnglePose
-from .._specimen import AbstractSpecimen
-from ._assembly import AbstractAssembly
+from .._structural_ensemble import (
+    AbstractConformationalVariable,
+    AbstractStructuralEnsemble,
+)
+from .assembly import AbstractAssembly
 
 
-class Helix(AbstractAssembly, strict=True):
+class HelicalAssembly(AbstractAssembly, strict=True):
     """
     Abstraction of a helical polymer.
 
     This class assembles a helix from a subunit.
     See the ``AbstractAssembly`` base class for more information.
 
     The screw axis is taken to be in the center of the
     image, pointing out-of-plane (i.e. along the z direction).
     """
 
-    subunit: AbstractSpecimen
+    subunit: AbstractStructuralEnsemble
     rise: Float[Array, ""]
     twist: Float[Array, ""]
 
     pose: AbstractPose
-    conformation: Optional[AbstractConformation]
+    conformation: Optional[AbstractConformationalVariable]
 
-    n_subunits: int = field(static=True)
-    n_start: int = field(static=True)
+    n_subunits: int
+    n_start: int
 
     def __init__(
         self,
-        subunit: AbstractSpecimen,
+        subunit: AbstractStructuralEnsemble,
         rise: Float[Array, ""] | float,
         twist: Float[Array, ""] | float,
         pose: Optional[AbstractPose] = None,
-        conformation: Optional[AbstractConformation] = None,
+        conformation: Optional[AbstractConformationalVariable] = None,
         n_start: int = 1,
         n_subunits: int = 1,
     ):
         """**Arguments:**
         - `subunit`:
             The helical subunit. It is important to set the the initial pose
             of the initial subunit here. This is in the center of mass frame
```

### Comparing `cryojax-0.2.3rc1/src/cryojax/simulator/_integrators/_gaussian_mixture.py` & `cryojax-0.3.0a0/src/cryojax/simulator/_potential_integrator/gaussian_mixture.py`

 * *Files identical despite different names*

### Comparing `cryojax-0.2.3rc1/src/cryojax/simulator/_integrators/_nufft_project.py` & `cryojax-0.3.0a0/src/cryojax/simulator/_potential_integrator/nufft_project.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,94 +1,101 @@
 """
 Using non-uniform FFTs for computing volume projections.
 """
 
 import math
+from typing_extensions import override
 
 import jax.numpy as jnp
-from equinox import field
 from jaxtyping import Array, Complex, Float
 
-from .._config import ImageConfig
-from .._potential import RealVoxelCloudPotential, RealVoxelGridPotential
-from ._potential_integrator import AbstractPotentialIntegrator
+from .._instrument_config import InstrumentConfig
+from .._potential_representation import RealVoxelCloudPotential, RealVoxelGridPotential
+from .base_potential_integrator import AbstractVoxelPotentialIntegrator
 
 
-class NufftProject(AbstractPotentialIntegrator, strict=True):
+class NufftProjection(
+    AbstractVoxelPotentialIntegrator[RealVoxelGridPotential | RealVoxelCloudPotential],
+    strict=True,
+):
     """Integrate points onto the exit plane using
     non-uniform FFTs.
-
-    Attributes
-    ----------
-    eps : `float`
-        See ``jax-finufft`` for documentation.
     """
 
-    eps: float = field(static=True, default=1e-6)
+    pixel_rescaling_method: str = "bicubic"
+    eps: float = 1e-6
+
+    def project_voxel_cloud_with_nufft(
+        self,
+        weights: Float[Array, " size"],
+        coordinate_list: Float[Array, "size 2"] | Float[Array, "size 3"],
+        shape: tuple[int, int],
+    ) -> Complex[Array, "{shape[0]} {shape[1]}"]:
+        """Project and interpolate 3D volume point cloud
+        onto imaging plane using a non-uniform FFT.
+
+        **Arguments:**
+
+        - `weights`:
+            Density point cloud.
+        - `coordinates`:
+            Coordinate system of point cloud.
+        - `shape`:
+            Shape of the imaging plane in pixels.
+            ``width, height = shape[0], shape[1]``
+            is the size of the desired imaging plane.
+
+        **Returns:**
+
+        The output image in fourier space.
+        """
+        return _project_with_nufft(weights, coordinate_list, shape, self.eps)
 
-    def __call__(
+    @override
+    def compute_raw_fourier_image(
         self,
         potential: RealVoxelGridPotential | RealVoxelCloudPotential,
-        wavelength_in_angstroms: Float[Array, ""],
-        config: ImageConfig,
-    ) -> Complex[Array, "{config.padded_y_dim} {config.padded_x_dim//2+1}"]:
+        instrument_config: InstrumentConfig,
+    ) -> Complex[
+        Array, "{instrument_config.padded_y_dim} {instrument_config.padded_x_dim//2+1}"
+    ]:
         """Rasterize image with non-uniform FFTs."""
         if isinstance(potential, RealVoxelGridPotential):
             shape = potential.shape
-            fourier_projection = project_with_nufft(
+            fourier_projection = self.project_voxel_cloud_with_nufft(
                 potential.real_voxel_grid.ravel(),
                 potential.wrapped_coordinate_grid_in_pixels.get().reshape(
                     (math.prod(shape), 3)
                 ),
-                config.padded_shape,
-                eps=self.eps,
+                instrument_config.padded_shape,
             )
         elif isinstance(potential, RealVoxelCloudPotential):
-            fourier_projection = project_with_nufft(
+            fourier_projection = self.project_voxel_cloud_with_nufft(
                 potential.voxel_weights,
                 potential.wrapped_coordinate_list_in_pixels.get(),
-                config.padded_shape,
-                eps=self.eps,
+                instrument_config.padded_shape,
             )
         else:
             raise ValueError(
                 "Supported density representations are RealVoxelGrid and VoxelCloud."
             )
-        # Rescale the voxel size to the ImageConfig.pixel_size
-        return config.rescale_to_pixel_size(
-            fourier_projection, potential.voxel_size, is_real=False
-        )
+        return fourier_projection
 
 
-def project_with_nufft(
-    weights: Float[Array, " size"],
-    coordinate_list: Float[Array, "size 2"] | Float[Array, "size 3"],
-    shape: tuple[int, int],
-    eps: float = 1e-6,
-) -> Complex[Array, "{shape[0]} {shape[1]}"]:
-    """
-    Project and interpolate 3D volume point cloud
-    onto imaging plane using a non-uniform FFT.
+NufftProjection.__init__.__doc__ = """**Arguments:**
 
-    Arguments
-    ---------
-    weights : shape `(N,)`
-        Density point cloud.
-    coordinates : shape `(N, 2)` or shape `(N, 3)`
-        Coordinate system of point cloud.
-    shape :
-        Shape of the imaging plane in pixels.
-        ``width, height = shape[0], shape[1]``
-        is the size of the desired imaging plane.
-
-    Returns
-    -------
-    projection :
-        The output image in fourier space.
-    """
+- `pixel_rescaling_method`:
+    Method for interpolating the final image to the `InstrumentConfig`
+    pixel size. See `cryojax.image._rescale_pixel_size` for documentation.
+- `eps` : `float`
+    See ``jax-finufft`` for documentation.
+"""
+
+
+def _project_with_nufft(weights, coordinate_list, shape, eps=1e-6):
     from jax_finufft import nufft1
 
     weights, coordinate_list = (
         jnp.asarray(weights).astype(complex),
         jnp.asarray(coordinate_list),
     )
     # Get x and y coordinates
```

### Comparing `cryojax-0.2.3rc1/src/cryojax/simulator/_potential/__init__.py` & `cryojax-0.3.0a0/src/cryojax/simulator/_potential_representation/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-from ._scattering_potential import (
-    AbstractScatteringPotential as AbstractScatteringPotential,
+from .base_potential import (
+    AbstractPotentialRepresentation as AbstractPotentialRepresentation,
 )
-from ._voxel_potential import (
+from .voxel_potential import (
     AbstractFourierVoxelGridPotential as AbstractFourierVoxelGridPotential,
     AbstractVoxelPotential as AbstractVoxelPotential,
     build_real_space_voxels_from_atoms as build_real_space_voxels_from_atoms,
     evaluate_3d_atom_potential as evaluate_3d_atom_potential,
     evaluate_3d_real_space_gaussian as evaluate_3d_real_space_gaussian,
     FourierVoxelGridPotential as FourierVoxelGridPotential,
     FourierVoxelGridPotentialInterpolator as FourierVoxelGridPotentialInterpolator,
```

### Comparing `cryojax-0.2.3rc1/src/cryojax/simulator/_potential/_atom_potential.py` & `cryojax-0.3.0a0/src/cryojax/simulator/_potential_representation/atom_potential.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,23 @@
 """
-Atomic-based electron density representations.
-"""
-
 from typing import Any, ClassVar, Type
 
 import equinox as eqx
 import jax.numpy as jnp
 from equinox import field
 from jaxtyping import Array
 
 from .._pose import AbstractPose
-from ._scattering_potential import AbstractScatteringPotential
+from .scattering_potential import AbstractScatteringPotential
 
 
 class AtomCloud(AbstractScatteringPotential):
-    """
+    '''
     Abstraction of a point cloud of atoms.
-    """
+    '''
 
     weights: Array = field(converter=jnp.asarray)
     coordinate_list: Array = field(converter=jnp.asarray)
     variances: Array = field(converter=jnp.asarray)
     identity: Array = field(converter=jnp.asarray)
 
     is_real: ClassVar[bool] = True
@@ -34,15 +31,16 @@
 
     @classmethod
     def from_file(
         cls: Type["AtomCloud"],
         filename: str,
         **kwargs: Any,
     ) -> "AtomCloud":
-        """
+        '''
         Load an Atom Cloud
 
         TODO: What is the file format appropriate here? Q. for Michael...
-        """
+        '''
 
         raise NotImplementedError
         # return cls.from_mrc(filename, config=config, **kwargs)
+"""
```

### Comparing `cryojax-0.2.3rc1/src/cryojax/simulator/_potential/_voxel_potential.py` & `cryojax-0.3.0a0/src/cryojax/simulator/_potential_representation/voxel_potential.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,40 +5,39 @@
 from abc import abstractmethod
 from functools import cached_property
 from typing import (
     Any,
     cast,
     ClassVar,
     Optional,
-    overload,
 )
 from typing_extensions import override, Self
 
 import equinox as eqx
 import jax
 import jax.numpy as jnp
 import numpy as np
 from equinox import AbstractClassVar, AbstractVar, field
 from jaxtyping import Array, Complex, Float, Int
 
+from ..._errors import error_if_not_positive
 from ...constants import get_form_factor_params
 from ...coordinates import CoordinateGrid, CoordinateList, FrequencySlice
-from ...core import error_if_not_positive
 from ...image import (
     compute_spline_coefficients,
     crop_to_shape,
     fftn,
     pad_to_shape,
 )
 from ...image.operators import AbstractFilter
 from .._pose import AbstractPose
-from ._scattering_potential import AbstractScatteringPotential
+from .base_potential import AbstractPotentialRepresentation
 
 
-class AbstractVoxelPotential(AbstractScatteringPotential, strict=True):
+class AbstractVoxelPotential(AbstractPotentialRepresentation, strict=True):
     """Abstract interface for a voxel-based scattering potential representation."""
 
     voxel_size: AbstractVar[Float[Array, ""]]
     is_real: AbstractClassVar[bool]
 
     @property
     @abstractmethod
@@ -49,15 +48,15 @@
     @classmethod
     @abstractmethod
     def from_real_voxel_grid(
         cls,
         real_voxel_grid: Float[Array, "dim dim dim"] | Float[np.ndarray, "dim dim dim"],
         voxel_size: Float[Array, ""] | Float[np.ndarray, ""] | float,
     ) -> Self:
-        """Load an `AbstractVoxels` from real-valued 3D electron
+        """Load an `AbstractVoxelPotential` from real-valued 3D electron
         scattering potential.
         """
         raise NotImplementedError
 
     @classmethod
     @abstractmethod
     def from_atoms(
@@ -68,15 +67,15 @@
         coordinate_grid_in_angstroms: CoordinateGrid,
         form_factors: Optional[
             Float[Array, "n_atoms n_form_factors"]
             | Float[np.ndarray, "n_atoms n_form_factors"]
         ] = None,
         **kwargs: Any,
     ) -> Self:
-        """Load an `AbstractVoxels` from atom positions and identities."""
+        """Load an `AbstractVoxelPotential` from atom positions and identities."""
         raise NotImplementedError
 
 
 class AbstractFourierVoxelGridPotential(AbstractVoxelPotential, strict=True):
     """Abstract interface of a 3D scattering potential voxel grid
     in fourier-space.
     """
@@ -180,17 +179,15 @@
         """Load an `AbstractFourierVoxelGridPotential` from atom positions and
         identities.
 
         **Arguments:**
 
         - `**kwargs`: Passed to `AbstractFourierVoxelGridPotential.from_real_voxel_grid`
         """
-        form_factors = (
-            form_factors if form_factors is None else jnp.asarray(form_factors)
-        )
+        form_factors = form_factors if form_factors is None else jnp.asarray(form_factors)
         a_vals, b_vals = get_form_factor_params(
             jnp.asarray(atom_identities), form_factors
         )
 
         potential = build_real_space_voxels_from_atoms(
             jnp.asarray(atom_positions),
             a_vals,
@@ -277,17 +274,15 @@
         """
         self.coefficients = compute_spline_coefficients(jnp.asarray(fourier_voxel_grid))
         self.wrapped_frequency_slice_in_pixels = wrapped_frequency_slice_in_pixels
         self.voxel_size = jnp.asarray(voxel_size)
 
     @property
     def shape(self) -> tuple[int, int, int]:
-        return cast(
-            tuple[int, int, int], tuple([s - 2 for s in self.coefficients.shape])
-        )
+        return cast(tuple[int, int, int], tuple([s - 2 for s in self.coefficients.shape]))
 
 
 class RealVoxelGridPotential(AbstractVoxelPotential, strict=True):
     """Abstraction of a 3D scattering potential voxel grid in real-space."""
 
     real_voxel_grid: Float[Array, "dim dim dim"]
     wrapped_coordinate_grid_in_pixels: CoordinateGrid
@@ -326,34 +321,14 @@
             lambda d: d.wrapped_coordinate_grid_in_pixels.array,
             self,
             pose.rotate_coordinates(
                 self.wrapped_coordinate_grid_in_pixels.get(), inverse=False
             ),
         )
 
-    @overload
-    @classmethod
-    def from_real_voxel_grid(
-        cls,
-        real_voxel_grid: Float[Array, "dim dim dim"] | Float[np.ndarray, "dim dim dim"],
-        voxel_size: Float[Array, ""] | Float[np.ndarray, ""] | float,
-        *,
-        coordinate_grid: Optional[CoordinateGrid] = None,
-    ) -> Self: ...
-
-    @overload
-    @classmethod
-    def from_real_voxel_grid(
-        cls,
-        real_voxel_grid: Float[Array, "dim dim dim"] | Float[np.ndarray, "dim dim dim"],
-        voxel_size: Float[Array, ""] | Float[np.ndarray, ""] | float,
-        *,
-        crop_scale: Optional[float] = None,
-    ) -> Self: ...
-
     @classmethod
     def from_real_voxel_grid(
         cls,
         real_voxel_grid: Float[Array, "dim dim dim"] | Float[np.ndarray, "dim dim dim"],
         voxel_size: Float[Array, ""] | Float[np.ndarray, ""] | float,
         *,
         coordinate_grid_in_pixels: Optional[CoordinateGrid] = None,
@@ -404,17 +379,15 @@
     ) -> Self:
         """Load a `RealVoxelGridPotential` from atom positions and identities.
 
         **Arguments:**
 
         - `**kwargs`: Passed to `RealVoxelGridPotential.from_real_voxel_grid`
         """
-        form_factors = (
-            form_factors if form_factors is None else jnp.asarray(form_factors)
-        )
+        form_factors = form_factors if form_factors is None else jnp.asarray(form_factors)
         a_vals, b_vals = get_form_factor_params(
             jnp.asarray(atom_identities), form_factors
         )
 
         real_voxel_grid = build_real_space_voxels_from_atoms(
             jnp.asarray(atom_positions),
             a_vals,
@@ -434,15 +407,16 @@
     """Abstraction of a 3D electron scattering potential voxel point cloud.
 
     !!! info
         This object is similar to the `RealVoxelGridPotential`. Instead
         of storing the whole voxel grid, a `RealVoxelCloudPotential` need
         only store points of non-zero scattering potential. Therefore,
         a `RealVoxelCloudPotential` stores a point cloud of scattering potential
-        voxel values.
+        voxel values. Instantiating with the `from_real_voxel_grid` constructor
+        will automatically mask points of zero scattering potential.
     """
 
     voxel_weights: Float[Array, " size"]
     wrapped_coordinate_list_in_pixels: CoordinateList
     voxel_size: Float[Array, ""] = field(converter=error_if_not_positive)
 
     is_real: ClassVar[bool] = True
@@ -461,16 +435,16 @@
         - `voxel_size`: The voxel size.
         """
         self.voxel_weights = jnp.asarray(voxel_weights)
         self.wrapped_coordinate_list_in_pixels = wrapped_coordinate_list_in_pixels
         self.voxel_size = jnp.asarray(voxel_size)
 
     @property
-    def shape(self) -> tuple[int, int]:
-        return cast(tuple[int, int], self.voxel_weights.shape)
+    def shape(self) -> tuple[int]:
+        return cast(tuple[int], self.voxel_weights.shape)
 
     @cached_property
     def wrapped_coordinate_list_in_angstroms(self) -> CoordinateList:
         """The `coordinate_list` in angstroms."""
         return self.voxel_size * self.wrapped_coordinate_list_in_pixels  # type: ignore
 
     def rotate_to_pose(self, pose: AbstractPose) -> Self:
@@ -487,38 +461,49 @@
         cls,
         real_voxel_grid: Float[Array, "dim dim dim"] | Float[np.ndarray, "dim dim dim"],
         voxel_size: Float[Array, ""] | Float[np.ndarray, ""] | float,
         *,
         coordinate_grid_in_pixels: Optional[CoordinateGrid] = None,
         rtol: float = 1e-05,
         atol: float = 1e-08,
+        size: Optional[int] = None,
+        fill_value: Optional[float] = None,
     ) -> Self:
         """Load an `RealVoxelCloudPotential` from a real-valued 3D electron
         scattering potential voxel grid.
 
         **Arguments:**
 
         - `real_voxel_grid`: An electron scattering potential voxel grid in real space.
         - `voxel_size`: The voxel size of `real_voxel_grid`.
-        - `rtol`: Argument passed to `jnp.isclose`, used for removing
-                points of zero scattering potential.
-        - `atol`: Argument passed to `jnp.isclose`, used for removing
-                points of zero scattering potential.
+        - `rtol`: Argument passed to `jnp.isclose`, used for masking
+                  voxels of zero scattering potential.
+        - `atol`: Argument passed to `jnp.isclose`, used for masking
+                  voxels of zero scattering potential.
+        - `size`: Argument passed to `jnp.where`, used for fixing the size
+                  of the masked scattering potential. This argument is required
+                  for using this function with a JAX transformation.
+        - `fill_value`: Argument passed to `jnp.where`, used if `size` is specified and
+                        the mask has fewer than the indicated number of elements.
         """
         # Cast to jax array
         real_voxel_grid, voxel_size = (
             jnp.asarray(real_voxel_grid),
             jnp.asarray(voxel_size),
         )
         # Make coordinates if not given
         if coordinate_grid_in_pixels is None:
             coordinate_grid_in_pixels = CoordinateGrid(real_voxel_grid.shape)
         # ... mask zeros to store smaller arrays. This
         # option is not jittable.
-        nonzero = jnp.where(~jnp.isclose(real_voxel_grid, 0.0, rtol=rtol, atol=atol))
+        nonzero = jnp.where(
+            ~jnp.isclose(real_voxel_grid, 0.0, rtol=rtol, atol=atol),
+            size=size,
+            fill_value=fill_value,
+        )
         flat_potential = real_voxel_grid[nonzero]
         coordinate_list = CoordinateList(coordinate_grid_in_pixels.get()[nonzero])
 
         return cls(flat_potential, coordinate_list, voxel_size)
 
     @classmethod
     def from_atoms(
@@ -535,17 +520,15 @@
     ) -> Self:
         """Load a `RealVoxelCloudPotential` from atom positions and identities.
 
         **Arguments:**
 
         - `**kwargs`: Passed to `RealVoxelCloudPotential.from_real_voxel_grid`
         """
-        form_factors = (
-            form_factors if form_factors is None else jnp.asarray(form_factors)
-        )
+        form_factors = form_factors if form_factors is None else jnp.asarray(form_factors)
         a_vals, b_vals = get_form_factor_params(
             jnp.asarray(atom_identities), form_factors
         )
 
         real_voxel_grid = build_real_space_voxels_from_atoms(
             jnp.asarray(atom_positions),
             a_vals,
```

### Comparing `cryojax-0.2.3rc1/tests/conftest.py` & `cryojax-0.3.0a0/tests/conftest.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 import os
 
-import equinox as eqx
 import jax
 import jax.numpy as jnp
 import jax.random as jr
 import pytest
 from jaxtyping import install_import_hook
 
 
 with install_import_hook("cryojax", "typeguard.typechecked"):
     import cryojax as cryojax
     import cryojax.simulator as cs
+    from cryojax.data import read_array_with_spacing_from_mrc
     from cryojax.image import operators as op, rfftn
-    from cryojax.io import read_array_with_spacing_from_mrc
 
 
 # jax.config.update("jax_numpy_dtype_promotion", "strict")
 # jax.config.update("jax_numpy_rank_promotion", "raise")
 jax.config.update("jax_enable_x64", True)
 
 
@@ -69,21 +68,26 @@
 
 @pytest.fixture
 def pixel_size():
     return 4.4
 
 
 @pytest.fixture
-def config(pixel_size):
-    return cs.ImageConfig((65, 66), pixel_size, pad_scale=1.1)
+def voltage_in_kilovolts():
+    return 300.0
 
 
 @pytest.fixture
-def integrator():
-    return cs.FourierSliceExtract(interpolation_order=1)
+def config(pixel_size, voltage_in_kilovolts):
+    return cs.InstrumentConfig((65, 66), pixel_size, voltage_in_kilovolts, pad_scale=1.1)
+
+
+@pytest.fixture
+def projection_method():
+    return cs.FourierSliceExtraction(interpolation_order=1)
 
 
 @pytest.fixture
 def potential(sample_mrc_path):
     real_voxel_grid, voxel_size = read_array_with_spacing_from_mrc(sample_mrc_path)
     return cs.FourierVoxelGridPotential.from_real_voxel_grid(
         real_voxel_grid, voxel_size, pad_scale=1.3
@@ -100,81 +104,69 @@
     return op.CircularMask(
         config.wrapped_padded_coordinate_grid_in_angstroms.get(),
         radius=20 * float(config.pixel_size),
     )
 
 
 @pytest.fixture
-def instrument():
-    voltage_in_kilovolts = 300.0
-    return cs.Instrument(
-        voltage_in_kilovolts,
-        optics=cs.WeakPhaseOptics(cs.CTF()),
-        dose=cs.ElectronDose(electrons_per_angstrom_squared=1000.0),
-        detector=cs.GaussianDetector(cs.IdealDQE(fraction_detected_electrons=1.0)),
-    )
+def transfer_theory():
+    return cs.ContrastTransferTheory(ctf=cs.ContrastTransferFunction())
+
+
+@pytest.fixture
+def detector():
+    return cs.PoissonDetector(cs.IdealDQE())
 
 
 @pytest.fixture
 def pose():
     return cs.EulerAnglePose(
         view_phi=30.0,
         view_theta=100.0,
         view_psi=-10.0,
         offset_x_in_angstroms=10.0,
         offset_y_in_angstroms=-5.0,
     )
 
 
 @pytest.fixture
-def specimen(potential, integrator, pose):
-    return cs.Specimen(potential, integrator, pose)
+def specimen(potential, pose):
+    return cs.SingleStructureEnsemble(potential, pose)
 
 
 @pytest.fixture
 def solvent():
     return cs.GaussianIce(op.Constant(0.001**2))
 
 
 @pytest.fixture
-def noiseless_model(config, specimen, instrument):
-    instrument = eqx.tree_at(lambda ins: ins.detector, instrument, None)
-    return cs.ImagePipeline(config=config, specimen=specimen, instrument=instrument)
+def theory(specimen, projection_method, transfer_theory, solvent):
+    return cs.LinearScatteringTheory(
+        specimen, projection_method, transfer_theory, solvent
+    )
 
 
 @pytest.fixture
-def noisy_model(config, specimen, instrument, solvent):
-    return cs.ImagePipeline(
-        config=config,
-        specimen=specimen,
-        instrument=instrument,
-        solvent=solvent,
+def theory_with_solvent(specimen, projection_method, transfer_theory, solvent):
+    return cs.LinearScatteringTheory(
+        specimen, projection_method, transfer_theory, solvent
     )
 
 
 @pytest.fixture
-def filtered_model(config, specimen, instrument, solvent, filters):
-    return cs.ImagePipeline(
-        config=config,
-        specimen=specimen,
-        instrument=instrument,
-        solvent=solvent,
-        filter=filters,
-    )
+def noiseless_model(config, theory):
+    return cs.IntensityImagingPipeline(instrument_config=config, scattering_theory=theory)
 
 
 @pytest.fixture
-def filtered_and_masked_model(config, specimen, instrument, solvent, filters, masks):
-    return cs.ImagePipeline(
-        config=config,
-        specimen=specimen,
-        instrument=instrument,
-        solvent=solvent,
-        filter=filters,
-        mask=masks,
+def noisy_model(config, theory_with_solvent, detector):
+    return cs.ElectronCountingImagingPipeline(
+        instrument_config=config,
+        scattering_theory=theory_with_solvent,
+        detector=detector,
     )
 
 
 @pytest.fixture
 def test_image(noisy_model):
-    image = noisy_model.sample(jr.PRNGKey(1234))
+    image = noisy_model.render(jr.PRNGKey(1234))
     return rfftn(image)
```

### Comparing `cryojax-0.2.3rc1/tests/test_agree_with_cistem.py` & `cryojax-0.3.0a0/tests/test_agree_with_cistem.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import jax
 import jax.numpy as jnp
 import numpy as np
 import pytest
-from pycistem.core import AnglesAndShifts, CTF as cisCTF, Image
+from pycistem.core import AnglesAndShifts, CTF as cisCTF, Image  # pyright: ignore
 
 import cryojax.simulator as cs
 from cryojax.coordinates import cartesian_to_polar, make_frequencies
+from cryojax.data import read_array_with_spacing_from_mrc
 from cryojax.image import irfftn, powerspectrum
-from cryojax.io import read_array_with_spacing_from_mrc
-from cryojax.simulator import CTF, EulerAnglePose
+from cryojax.simulator import ContrastTransferFunction, EulerAnglePose
 
 
 jax.config.update("jax_enable_x64", True)
 
 
 @pytest.mark.parametrize(
     "defocus1,defocus2,asti_angle,kV,cs,ac,pixel_size",
@@ -32,36 +32,36 @@
     """Test CTF model against cisTEM.
 
     Modified from https://github.com/jojoelfe/contrasttransferfunction"""
     shape = (512, 512)
     freqs = make_frequencies(shape, pixel_size)
     k_sqr, theta = cartesian_to_polar(freqs, square=True)
     # Compute cryojax CTF
-    optics = CTF(
-        defocus_u_in_angstroms=defocus1,
-        defocus_v_in_angstroms=defocus2,
+    optics = ContrastTransferFunction(
+        defocus_in_angstroms=defocus1,
+        astigmatism_in_angstroms=defocus2 - defocus1,
         astigmatism_angle=asti_angle,
         voltage_in_kilovolts=kV,
         spherical_aberration_in_mm=cs,
         amplitude_contrast_ratio=ac,
     )
-    ctf = np.array(optics(freqs))
+    ctf = jnp.array(optics(freqs))
     # Compute cisTEM CTF
     cisTEM_optics = cisCTF(
         kV=kV,
         cs=cs,
         ac=ac,
         defocus1=defocus1,
         defocus2=defocus2,
         astig_angle=asti_angle,
         pixel_size=pixel_size,
     )
-    cisTEM_ctf = np.vectorize(
-        lambda k_sqr, theta: cisTEM_optics.Evaluate(k_sqr, theta)
-    )(k_sqr.ravel() * pixel_size**2, theta.ravel()).reshape(freqs.shape[0:2])
+    cisTEM_ctf = np.vectorize(lambda k_sqr, theta: cisTEM_optics.Evaluate(k_sqr, theta))(
+        k_sqr.ravel() * pixel_size**2, theta.ravel()
+    ).reshape(freqs.shape[0:2])
     cisTEM_ctf[0, 0] = 0.0
 
     # Compute cryojax and cisTEM power spectrum
     radial_freqs = jnp.linalg.norm(freqs, axis=-1)
     spectrum1D, _ = powerspectrum(
         ctf, radial_freqs, pixel_size, k_max=1 / (2 * pixel_size)
     )
@@ -118,22 +118,23 @@
 ):
     # cryojax
     real_voxel_grid, voxel_size = read_array_with_spacing_from_mrc(sample_mrc_path)
     potential = cs.FourierVoxelGridPotential.from_real_voxel_grid(
         real_voxel_grid, voxel_size
     )
     pose = cs.EulerAnglePose(view_phi=phi, view_theta=theta, view_psi=psi)
-    integrator = cs.FourierSliceExtract()
-    specimen = cs.Specimen(potential, integrator, pose)
+    projection_method = cs.FourierSliceExtraction()
     box_size = potential.shape[0]
-    config = cs.ImageConfig((box_size, box_size), pixel_size)
-    instrument = cs.Instrument(voltage_in_kilovolts=300.0)
-    pipeline = cs.ImagePipeline(config, specimen, instrument)
+    config = cs.InstrumentConfig((box_size, box_size), pixel_size, 300.0)
     cryojax_projection = irfftn(
-        pipeline.render(get_real=False).at[0, 0].set(0.0 + 0.0j)
+        projection_method.compute_raw_fourier_image(
+            potential.rotate_to_pose(pose), config
+        )
+        .at[0, 0]
+        .set(0.0 + 0.0j)
         / np.sqrt(np.prod(config.shape)),
         s=config.padded_shape,
     )
     # pycistem
     pycistem_volume = _load_pycistem_template(sample_mrc_path, box_size)
     pycistem_angles = AnglesAndShifts()
     pycistem_angles.Init(phi, theta, psi, 0.0, 0.0)
```

### Comparing `cryojax-0.2.3rc1/tests/test_atom_routines.py` & `cryojax-0.3.0a0/tests/test_atom_routines.py`

 * *Files identical despite different names*

### Comparing `cryojax-0.2.3rc1/tests/test_detector.py` & `cryojax-0.3.0a0/tests/test_detector.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,41 +4,41 @@
 
 import cryojax.simulator as cs
 from cryojax.image import irfftn, rfftn
 
 
 def test_gaussian_limit():
     # Pick a large integrated electron flux to test
-    electrons_per_angstrom_squared = 10000.0
-    # Create ImageConfig
-    config = cs.ImageConfig((25, 25), 1.0)
+    # Create InstrumentConfig, picking a large electron flux to test
+    config = cs.InstrumentConfig(
+        (25, 25),
+        1.0,
+        voltage_in_kilovolts=300.0,
+        electrons_per_angstrom_squared=10000.0,
+    )
     N_pix = np.prod(config.padded_shape)
-    electrons_per_pixel = electrons_per_angstrom_squared * config.pixel_size**2
+    electrons_per_pixel = config.electrons_per_angstrom_squared * config.pixel_size**2
     # Create squared wavefunction of just vacuum, i.e. 1 everywhere
     vacuum_squared_wavefunction = jnp.ones(config.shape, dtype=float)
     fourier_vacuum_squared_wavefunction = rfftn(vacuum_squared_wavefunction)
-    # Instantiate the electron dose
-    dose = cs.ElectronDose(electrons_per_angstrom_squared)
     # Create detector models
     key = jax.random.PRNGKey(1234)
     dqe = cs.IdealDQE()
     gaussian_detector = cs.GaussianDetector(dqe)
     poisson_detector = cs.PoissonDetector(dqe)
     # Compute detector readout
-    fourier_gaussian_detector_readout = gaussian_detector(
+    fourier_gaussian_detector_readout = gaussian_detector.compute_detector_readout(
+        key,
         fourier_vacuum_squared_wavefunction,
         config,
-        dose.electrons_per_angstrom_squared,
-        key,
     )
-    fourier_poisson_detector_readout = poisson_detector(
+    fourier_poisson_detector_readout = poisson_detector.compute_detector_readout(
+        key,
         fourier_vacuum_squared_wavefunction,
         config,
-        dose.electrons_per_angstrom_squared,
-        key,
     )
     # Compare to see if the autocorrelation has converged
     np.testing.assert_allclose(
         irfftn(
             jnp.abs(fourier_gaussian_detector_readout) ** 2
             / (N_pix * electrons_per_pixel**2),
             s=config.padded_shape,
```

### Comparing `cryojax-0.2.3rc1/tests/test_fft.py` & `cryojax-0.3.0a0/tests/test_fft.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,13 +25,11 @@
         ifftn(fftn(random)).real, jnp.fft.ifftn(jnp.fft.fftn(random)).real
     )
     np.testing.assert_allclose(random, ifftn(fftn(random)).real)
     np.testing.assert_allclose(fftn(random), fftn(ifftn(fftn(random))))
     # Run tests with an image
     np.testing.assert_allclose(image, ifftn(fftn(image)).real)
     # ... test zero mode separately
-    np.testing.assert_allclose(
-        fftn(image)[1:, 1:], fftn(ifftn(fftn(image)).real)[1:, 1:]
-    )
+    np.testing.assert_allclose(fftn(image)[1:, 1:], fftn(ifftn(fftn(image)).real)[1:, 1:])
     np.testing.assert_allclose(
         fftn(image)[0, 0], fftn(ifftn(fftn(image)).real)[0, 0], atol=1e-12
     )
```

### Comparing `cryojax-0.2.3rc1/tests/test_pose_agreement.py` & `cryojax-0.3.0a0/tests/test_pose_agreement.py`

 * *Files 9% similar despite different names*

```diff
@@ -17,38 +17,38 @@
 
 
 def test_translation_agreement():
     rotation = SO3(jnp.asarray((1.0, 0.0, 0.0, 0.0)))
     offset = jnp.asarray((0.0, -1.4, 4.5))
     quat = cs.QuaternionPose.from_rotation_and_translation(rotation, offset)
     axis_angle = cs.AxisAnglePose.from_rotation_and_translation(rotation, offset)
-    np.testing.assert_allclose(
-        quat.rotation.as_matrix(), axis_angle.rotation.as_matrix()
-    )
+    np.testing.assert_allclose(quat.rotation.as_matrix(), axis_angle.rotation.as_matrix())
     np.testing.assert_allclose(quat.offset_in_angstroms, axis_angle.offset_in_angstroms)
 
 
 def test_pose_conversion():
     wxyz = jnp.asarray((1.0, 2.0, 3.0, 0.5))
     rotation = SO3(wxyz).normalize()
     quat = cs.QuaternionPose.from_rotation(rotation)
     euler = cs.EulerAnglePose.from_rotation(rotation)
     axis_angle = cs.AxisAnglePose.from_rotation(rotation)
     np.testing.assert_allclose(quat.rotation.as_matrix(), euler.rotation.as_matrix())
-    np.testing.assert_allclose(
-        quat.rotation.as_matrix(), axis_angle.rotation.as_matrix()
-    )
+    np.testing.assert_allclose(quat.rotation.as_matrix(), axis_angle.rotation.as_matrix())
 
 
 def test_default_pose_images(noiseless_model):
     euler = cs.EulerAnglePose()
     quat = cs.QuaternionPose()
 
-    model_euler = eqx.tree_at(lambda m: m.specimen.pose, noiseless_model, euler)
-    model_quat = eqx.tree_at(lambda m: m.specimen.pose, noiseless_model, quat)
+    model_euler = eqx.tree_at(
+        lambda m: m.scattering_theory.structural_ensemble.pose, noiseless_model, euler
+    )
+    model_quat = eqx.tree_at(
+        lambda m: m.scattering_theory.structural_ensemble.pose, noiseless_model, quat
+    )
     np.testing.assert_allclose(model_euler.render(), model_quat.render())
 
 
 def test_axis_angle_euler_agreement():
     angle = 2.0
     angle_in_radians = jnp.deg2rad(angle)
     rotation_x = SO3.from_x_radians(angle_in_radians)
```

### Comparing `cryojax-0.2.3rc1/tests/test_voxels_from_atoms.py` & `cryojax-0.3.0a0/tests/test_voxels_from_atoms.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import jax
 import jax.numpy as jnp
 import numpy as np
 import pytest
 from jax import config
 
 from cryojax.coordinates import CoordinateGrid
+from cryojax.data import read_atoms_from_pdb
 from cryojax.image import ifftn
-from cryojax.io import read_atoms_from_pdb
 from cryojax.simulator import (
     build_real_space_voxels_from_atoms,
     FourierVoxelGridPotential,
     RealVoxelGridPotential,
 )
```

### Comparing `cryojax-0.2.3rc1/LICENSE` & `cryojax-0.3.0a0/LICENSE`

 * *Files identical despite different names*

### Comparing `cryojax-0.2.3rc1/README.md` & `cryojax-0.3.0a0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -45,85 +45,82 @@
 
 The [`jax-finufft`](https://github.com/dfm/jax-finufft) package is an optional dependency used for non-uniform fast fourier transforms. These are included as an option for computing image projections of real-space voxel-based scattering potential representations. In this case, we recommend first following the `jax_finufft` installation instructions and then installing `cryojax`.
 
 ## Simulating an image
 
 The following is a basic workflow to simulate an image.
 
-First, instantiate the scattering potential representation and its respective method for computing image projections.
+First, instantiate the spatial potential energy distribution representation and its respective method for computing image projections.
 
 ```python
 import jax
 import jax.numpy as jnp
-import cryojax.simulator as cs
-from cryojax.io import read_array_with_spacing_from_mrc
+import cryojax.simulator as cxs
+from cryojax.data import read_array_with_spacing_from_mrc
 
-# Instantiate the scattering potential.
+# Instantiate the scattering potential
 filename = "example_scattering_potential.mrc"
 real_voxel_grid, voxel_size = read_array_with_spacing_from_mrc(filename)
-potential = cs.FourierVoxelGridPotential.from_real_voxel_grid(real_voxel_grid, voxel_size)
-# ... now instantiate fourier slice extraction
-integrator = cs.FourierSliceExtract(interpolation_order=1)
-```
-
-Here, the 3D scattering potential array is read from `filename`. Then, the abstraction of the scattering potential is then loaded in fourier-space into a `FourierVoxelGridPotential`, and the fourier-slice projection theorem is initialized with `FourierSliceExtract`. The scattering potential can be generated with an external program, such as the [cisTEM](https://github.com/timothygrant80/cisTEM) simulate tool.
-
-We can now instantiate the representation of a biological specimen, which also includes a pose.
-
-```python
-# First instantiate the pose. Here, angles are given in degrees
-pose = cs.EulerAnglePose(
+potential = cxs.FourierVoxelGridPotential.from_real_voxel_grid(real_voxel_grid, voxel_size)
+# ... now, instantiate the pose. Angles are given in degrees
+pose = cxs.EulerAnglePose(
     offset_x_in_angstroms=5.0,
     offset_y_in_angstroms=-3.0,
     view_phi=20.0,
     view_theta=80.0,
     view_psi=-10.0,
 )
-# ... now, build the biological specimen
-specimen = cs.Specimen(potential, integrator, pose)
+# ... now, build the ensemble. In this case, the ensemble is just a single structure
+structural_ensemble = cxs.SingleStructureEnsemble(potential, pose)
 ```
 
-Next, build the model for the electron microscope. Here, we simply include a model for the CTF in the weak-phase approximation (linear image formation theory).
+Here, the 3D scattering potential array is read from `filename`. Then, the abstraction of the scattering potential is then loaded in fourier-space into a `FourierVoxelGridPotential`. The scattering potential can be generated with an external program, such as the [cisTEM](https://github.com/timothygrant80/cisTEM) simulate tool. Then, the representation of a biological specimen is instantiated, which also includes a pose and conformational heterogeneity. Here, the `SingleStructureEnsemble` class takes a pose but has no heterogeneity.
+
+Next, build the *scattering theory*. The simplest `scattering_theory` is the `LinearScatteringTheory`. This represents the usual image formation pipeline in cryo-EM, which forms images by computing projections of the potential and convolving the result with a contrast transfer function.
 
 ```python
 from cryojax.image import operators as op
 
-# First, initialize the CTF and its optics model
-ctf = cs.CTF(
-    defocus_u_in_angstroms=10000.0,
-    defocus_v_in_angstroms=9800.0,
+# Initialize the scattering theory. First, instantiate fourier slice extraction
+potential_integrator = cxs.FourierSliceExtraction(interpolation_order=1)
+# ... next, the contrast transfer theory
+ctf = cxs.ContrastTransferFunction(
+    defocus_in_angstroms=9800.0,
+    astigmatism_in_angstroms=200.0,
     astigmatism_angle=10.0,
-    amplitude_contrast_ratio=0.1)
-optics = cs.WeakPhaseOptics(ctf, envelope=op.FourierGaussian(b_factor=5.0))  # b_factor is given in Angstroms^2
-# ... these are stored in the Instrument
-voltage_in_kilovolts = 300.0,
-instrument = cs.Instrument(voltage_in_kilovolts, optics)
+    amplitude_contrast_ratio=0.1
+)
+transfer_theory = cxs.ContrastTransferTheory(ctf, envelope=op.FourierGaussian(b_factor=5.0))
+# ... now for the scattering theory
+scattering_theory = cxs.LinearScatteringTheory(structural_ensemble, potential_integrator, transfer_theory)
 ```
 
-The `CTF` has parameters used in CTFFIND4, which take their default values if not
-explicitly configured here. Finally, we can instantiate the `ImagePipeline` and simulate an image.
+The `ContrastTransferFunction` has parameters used in CTFFIND4, which take their default values if not
+explicitly configured here. Finally, we can instantiate the `imaging_pipeline`--the highest level of imaging abstraction in `cryojax`--and simulate an image. Here, we choose a `ContrastImagingPipeline`, which simulates image contrast from a linear scattering theory.
 
 ```python
-# Instantiate the image configuration
-config = cs.ImageConfig(shape=(320, 320), pixel_size=voxel_size)
-# Build the image formation model
-pipeline = cs.ImagePipeline(config, specimen, instrument)
-# ... simulate an image and return in real-space.
-image_without_noise = pipeline.render(get_real=True)
+# Finally, build the image formation model
+# ... first instantiate the instrument configuration
+instrument_config = cxs.InstrumentConfig(shape=(320, 320), pixel_size=voxel_size, voltage_in_kilovolts=300.0)
+# ... now the imaging pipeline
+imaging_pipeline = cxs.ContrastImagingPipeline(instrument_config, scattering_theory)
+# ... finally, simulate an image and return in real-space!
+image_without_noise = imaging_pipeline.render(get_real=True)
 ```
 
-`cryojax` also defines a library of distributions from which to sample the data. These distributions define the stochastic model from which images are drawn. For example, instantiate an `IndependentFourierGaussian` distribution and either sample from it or compute its log-likelihood.
+`cryojax` also defines a library of distributions from which to sample the data. These distributions define the stochastic model from which images are drawn. For example, instantiate an `IndependentGaussianFourierModes` distribution and either sample from it or compute its log-likelihood.
 
 ```python
-from cryojax.image import rfftn
+from cryojax.image import rfftn, operators as op
 from cryojax.inference import distributions as dist
-from cryojax.image import operators as op
 
 # Passing the ImagePipeline and a variance function, instantiate the distribution
-distribution = dist.IndependentFourierGaussian(pipeline, variance=op.Constant(1.0))
+distribution = dist.IndependentGaussianFourierModes(
+    imaging_pipeline, variance_function=op.Constant(1.0)
+)
 # ... then, either simulate an image from this distribution
 key = jax.random.PRNGKey(seed=0)
 image_with_noise = distribution.sample(key)
 # ... or compute the likelihood
 observed = rfftn(...)  # for this example, read in observed data and take FFT
 log_likelihood = distribution.log_likelihood(observed)
 ```
```

### Comparing `cryojax-0.2.3rc1/pyproject.toml` & `cryojax-0.3.0a0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -23,14 +23,15 @@
     "equinox>=0.11.0",
     "jaxtyping>=0.2.23",
     "lineax",
     "mrcfile",
     "starfile",
     "pandas",
     "typing_extensions>=4.5.0",
+    "tqdm",
 ]
 
 [project.optional-dependencies]
 test = ["pytest", "pycistem", "gemmi"]
 
 [build-system]
 requires = ["hatchling", "hatch-vcs"]
@@ -41,22 +42,26 @@
 
 [tool.hatch.build.hooks.vcs]
 version-file = "src/cryojax/cryojax_version.py"
 
 [tool.ruff]
 extend-include = ["*.ipynb"]
 lint.fixable = ["I001", "F401"]
+line-length = 90
 lint.ignore = ["E402", "E721", "E731", "E741", "F722"]
 lint.ignore-init-module-imports = true
 lint.select = ["E", "F", "I001"]
 src = ["src"]
 
 [tool.ruff.lint.isort]
 combine-as-imports = true
 extra-standard-library = ["typing_extensions"]
 lines-after-imports = 2
 order-by-type = false
 
+[tool.black]
+line-length = 90
+
 [tool.pyright]
 reportIncompatibleMethodOverride = true
 reportIncompatibleVariableOverride = false  # Incompatible with eqx.AbstractVar
 include = ["cryojax", "tests"]
```

### Comparing `cryojax-0.2.3rc1/PKG-INFO` & `cryojax-0.3.0a0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: cryojax
-Version: 0.2.3rc1
+Version: 0.3.0a0
 Summary: Cryo-EM image simulation and analysis powered by JAX
 Project-URL: repository, https://github.com/mjo22/cryojax
 Author-email: Michael O'Brien <michaelobrien@g.harvard.edu>
 License:                   GNU LESSER GENERAL PUBLIC LICENSE
                                Version 2.1, February 1999
         
          Copyright (C) 1991, 1999 Free Software Foundation, Inc.
@@ -522,14 +522,15 @@
 Requires-Dist: jax
 Requires-Dist: jaxlib
 Requires-Dist: jaxtyping>=0.2.23
 Requires-Dist: lineax
 Requires-Dist: mrcfile
 Requires-Dist: pandas
 Requires-Dist: starfile
+Requires-Dist: tqdm
 Requires-Dist: typing-extensions>=4.5.0
 Provides-Extra: test
 Requires-Dist: gemmi; extra == 'test'
 Requires-Dist: pycistem; extra == 'test'
 Requires-Dist: pytest; extra == 'test'
 Description-Content-Type: text/markdown
 
@@ -580,85 +581,82 @@
 
 The [`jax-finufft`](https://github.com/dfm/jax-finufft) package is an optional dependency used for non-uniform fast fourier transforms. These are included as an option for computing image projections of real-space voxel-based scattering potential representations. In this case, we recommend first following the `jax_finufft` installation instructions and then installing `cryojax`.
 
 ## Simulating an image
 
 The following is a basic workflow to simulate an image.
 
-First, instantiate the scattering potential representation and its respective method for computing image projections.
+First, instantiate the spatial potential energy distribution representation and its respective method for computing image projections.
 
 ```python
 import jax
 import jax.numpy as jnp
-import cryojax.simulator as cs
-from cryojax.io import read_array_with_spacing_from_mrc
+import cryojax.simulator as cxs
+from cryojax.data import read_array_with_spacing_from_mrc
 
-# Instantiate the scattering potential.
+# Instantiate the scattering potential
 filename = "example_scattering_potential.mrc"
 real_voxel_grid, voxel_size = read_array_with_spacing_from_mrc(filename)
-potential = cs.FourierVoxelGridPotential.from_real_voxel_grid(real_voxel_grid, voxel_size)
-# ... now instantiate fourier slice extraction
-integrator = cs.FourierSliceExtract(interpolation_order=1)
-```
-
-Here, the 3D scattering potential array is read from `filename`. Then, the abstraction of the scattering potential is then loaded in fourier-space into a `FourierVoxelGridPotential`, and the fourier-slice projection theorem is initialized with `FourierSliceExtract`. The scattering potential can be generated with an external program, such as the [cisTEM](https://github.com/timothygrant80/cisTEM) simulate tool.
-
-We can now instantiate the representation of a biological specimen, which also includes a pose.
-
-```python
-# First instantiate the pose. Here, angles are given in degrees
-pose = cs.EulerAnglePose(
+potential = cxs.FourierVoxelGridPotential.from_real_voxel_grid(real_voxel_grid, voxel_size)
+# ... now, instantiate the pose. Angles are given in degrees
+pose = cxs.EulerAnglePose(
     offset_x_in_angstroms=5.0,
     offset_y_in_angstroms=-3.0,
     view_phi=20.0,
     view_theta=80.0,
     view_psi=-10.0,
 )
-# ... now, build the biological specimen
-specimen = cs.Specimen(potential, integrator, pose)
+# ... now, build the ensemble. In this case, the ensemble is just a single structure
+structural_ensemble = cxs.SingleStructureEnsemble(potential, pose)
 ```
 
-Next, build the model for the electron microscope. Here, we simply include a model for the CTF in the weak-phase approximation (linear image formation theory).
+Here, the 3D scattering potential array is read from `filename`. Then, the abstraction of the scattering potential is then loaded in fourier-space into a `FourierVoxelGridPotential`. The scattering potential can be generated with an external program, such as the [cisTEM](https://github.com/timothygrant80/cisTEM) simulate tool. Then, the representation of a biological specimen is instantiated, which also includes a pose and conformational heterogeneity. Here, the `SingleStructureEnsemble` class takes a pose but has no heterogeneity.
+
+Next, build the *scattering theory*. The simplest `scattering_theory` is the `LinearScatteringTheory`. This represents the usual image formation pipeline in cryo-EM, which forms images by computing projections of the potential and convolving the result with a contrast transfer function.
 
 ```python
 from cryojax.image import operators as op
 
-# First, initialize the CTF and its optics model
-ctf = cs.CTF(
-    defocus_u_in_angstroms=10000.0,
-    defocus_v_in_angstroms=9800.0,
+# Initialize the scattering theory. First, instantiate fourier slice extraction
+potential_integrator = cxs.FourierSliceExtraction(interpolation_order=1)
+# ... next, the contrast transfer theory
+ctf = cxs.ContrastTransferFunction(
+    defocus_in_angstroms=9800.0,
+    astigmatism_in_angstroms=200.0,
     astigmatism_angle=10.0,
-    amplitude_contrast_ratio=0.1)
-optics = cs.WeakPhaseOptics(ctf, envelope=op.FourierGaussian(b_factor=5.0))  # b_factor is given in Angstroms^2
-# ... these are stored in the Instrument
-voltage_in_kilovolts = 300.0,
-instrument = cs.Instrument(voltage_in_kilovolts, optics)
+    amplitude_contrast_ratio=0.1
+)
+transfer_theory = cxs.ContrastTransferTheory(ctf, envelope=op.FourierGaussian(b_factor=5.0))
+# ... now for the scattering theory
+scattering_theory = cxs.LinearScatteringTheory(structural_ensemble, potential_integrator, transfer_theory)
 ```
 
-The `CTF` has parameters used in CTFFIND4, which take their default values if not
-explicitly configured here. Finally, we can instantiate the `ImagePipeline` and simulate an image.
+The `ContrastTransferFunction` has parameters used in CTFFIND4, which take their default values if not
+explicitly configured here. Finally, we can instantiate the `imaging_pipeline`--the highest level of imaging abstraction in `cryojax`--and simulate an image. Here, we choose a `ContrastImagingPipeline`, which simulates image contrast from a linear scattering theory.
 
 ```python
-# Instantiate the image configuration
-config = cs.ImageConfig(shape=(320, 320), pixel_size=voxel_size)
-# Build the image formation model
-pipeline = cs.ImagePipeline(config, specimen, instrument)
-# ... simulate an image and return in real-space.
-image_without_noise = pipeline.render(get_real=True)
+# Finally, build the image formation model
+# ... first instantiate the instrument configuration
+instrument_config = cxs.InstrumentConfig(shape=(320, 320), pixel_size=voxel_size, voltage_in_kilovolts=300.0)
+# ... now the imaging pipeline
+imaging_pipeline = cxs.ContrastImagingPipeline(instrument_config, scattering_theory)
+# ... finally, simulate an image and return in real-space!
+image_without_noise = imaging_pipeline.render(get_real=True)
 ```
 
-`cryojax` also defines a library of distributions from which to sample the data. These distributions define the stochastic model from which images are drawn. For example, instantiate an `IndependentFourierGaussian` distribution and either sample from it or compute its log-likelihood.
+`cryojax` also defines a library of distributions from which to sample the data. These distributions define the stochastic model from which images are drawn. For example, instantiate an `IndependentGaussianFourierModes` distribution and either sample from it or compute its log-likelihood.
 
 ```python
-from cryojax.image import rfftn
+from cryojax.image import rfftn, operators as op
 from cryojax.inference import distributions as dist
-from cryojax.image import operators as op
 
 # Passing the ImagePipeline and a variance function, instantiate the distribution
-distribution = dist.IndependentFourierGaussian(pipeline, variance=op.Constant(1.0))
+distribution = dist.IndependentGaussianFourierModes(
+    imaging_pipeline, variance_function=op.Constant(1.0)
+)
 # ... then, either simulate an image from this distribution
 key = jax.random.PRNGKey(seed=0)
 image_with_noise = distribution.sample(key)
 # ... or compute the likelihood
 observed = rfftn(...)  # for this example, read in observed data and take FFT
 log_likelihood = distribution.log_likelihood(observed)
 ```
```

