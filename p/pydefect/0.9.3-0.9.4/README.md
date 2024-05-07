# Comparing `tmp/pydefect-0.9.3.tar.gz` & `tmp/pydefect-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pydefect-0.9.3.tar", last modified: Sun Mar 31 01:55:42 2024, max compression
+gzip compressed data, was "dist/pydefect-0.9.4.tar", last modified: Tue May  7 00:39:22 2024, max compression
```

## Comparing `pydefect-0.9.3.tar` & `pydefect-0.9.4.tar`

### file list

```diff
@@ -1,287 +1,229 @@
-drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2024-03-31 01:55:42.190449 pydefect-0.9.3/
--rw-r--r--   0 kumagai    (501) staff       (20)       54 2021-03-12 02:40:59.000000 pydefect-0.9.3/MANIFEST.in
--rw-r--r--   0 kumagai    (501) staff       (20)      397 2024-03-31 01:55:42.189967 pydefect-0.9.3/PKG-INFO
--rw-r--r--   0 kumagai    (501) staff       (20)     4571 2023-11-29 21:52:31.000000 pydefect-0.9.3/README.md
-drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2024-03-31 01:55:41.947057 pydefect-0.9.3/pydefect/
--rw-r--r--   0 kumagai    (501) staff       (20)       21 2024-03-31 01:55:11.000000 pydefect-0.9.3/pydefect/__init__.py
-drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2024-03-31 01:55:41.970824 pydefect-0.9.3/pydefect/analyzer/
--rw-r--r--   0 kumagai    (501) staff       (20)       95 2020-05-18 00:09:10.000000 pydefect-0.9.3/pydefect/analyzer/__init__.py
--rw-r--r--   0 kumagai    (501) staff       (20)     2840 2021-04-02 01:38:50.000000 pydefect-0.9.3/pydefect/analyzer/_defect_charge_distribution.py
--rw-r--r--   0 kumagai    (501) staff       (20)    12239 2023-11-09 01:03:42.000000 pydefect-0.9.3/pydefect/analyzer/band_edge_states.py
--rw-r--r--   0 kumagai    (501) staff       (20)     1334 2021-05-01 01:17:09.000000 pydefect-0.9.3/pydefect/analyzer/calc_results.py
--rw-r--r--   0 kumagai    (501) staff       (20)     2426 2021-05-26 07:04:12.000000 pydefect-0.9.3/pydefect/analyzer/calc_summary.py
-drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2024-03-31 01:55:41.976354 pydefect-0.9.3/pydefect/analyzer/concentration/
--rw-r--r--   0 kumagai    (501) staff       (20)       61 2023-01-30 01:05:15.000000 pydefect-0.9.3/pydefect/analyzer/concentration/__init__.py
--rw-r--r--   0 kumagai    (501) staff       (20)     5631 2023-02-08 05:36:42.000000 pydefect-0.9.3/pydefect/analyzer/concentration/concentration.py
--rw-r--r--   0 kumagai    (501) staff       (20)     2973 2023-02-01 00:50:27.000000 pydefect-0.9.3/pydefect/analyzer/concentration/degeneracy.py
--rw-r--r--   0 kumagai    (501) staff       (20)      385 2023-01-30 01:10:12.000000 pydefect-0.9.3/pydefect/analyzer/concentration/distribution_function.py
--rw-r--r--   0 kumagai    (501) staff       (20)     7772 2023-02-08 07:02:02.000000 pydefect-0.9.3/pydefect/analyzer/concentration/make_concentration.py
--rw-r--r--   0 kumagai    (501) staff       (20)     2462 2023-03-09 04:26:39.000000 pydefect-0.9.3/pydefect/analyzer/concentration/plot_concentration.py
--rw-r--r--   0 kumagai    (501) staff       (20)     4716 2021-08-06 10:14:07.000000 pydefect-0.9.3/pydefect/analyzer/defect_charge_info.py
--rw-r--r--   0 kumagai    (501) staff       (20)    13088 2023-06-29 09:23:18.000000 pydefect-0.9.3/pydefect/analyzer/defect_energy.py
--rw-r--r--   0 kumagai    (501) staff       (20)     7810 2024-01-26 05:08:28.000000 pydefect-0.9.3/pydefect/analyzer/defect_energy_plotter.py
--rw-r--r--   0 kumagai    (501) staff       (20)     1280 2022-11-15 04:48:53.000000 pydefect-0.9.3/pydefect/analyzer/defect_energy_util.py
--rw-r--r--   0 kumagai    (501) staff       (20)     7741 2022-09-30 05:43:38.000000 pydefect-0.9.3/pydefect/analyzer/defect_structure_comparator.py
--rw-r--r--   0 kumagai    (501) staff       (20)     6536 2023-01-28 01:55:02.000000 pydefect-0.9.3/pydefect/analyzer/defect_structure_info.py
--rw-r--r--   0 kumagai    (501) staff       (20)     6463 2023-11-29 23:55:37.000000 pydefect-0.9.3/pydefect/analyzer/eigenvalue_plotter.py
--rw-r--r--   0 kumagai    (501) staff       (20)     2420 2021-08-06 10:11:01.000000 pydefect-0.9.3/pydefect/analyzer/grids.py
--rw-r--r--   0 kumagai    (501) staff       (20)     7225 2022-11-22 05:43:00.000000 pydefect-0.9.3/pydefect/analyzer/make_band_edge_states.py
--rw-r--r--   0 kumagai    (501) staff       (20)     1571 2021-05-26 07:04:53.000000 pydefect-0.9.3/pydefect/analyzer/make_calc_summary.py
--rw-r--r--   0 kumagai    (501) staff       (20)     2390 2023-12-01 04:56:00.000000 pydefect-0.9.3/pydefect/analyzer/make_defect_energy_info.py
--rw-r--r--   0 kumagai    (501) staff       (20)     1716 2023-02-11 23:51:37.000000 pydefect-0.9.3/pydefect/analyzer/make_defect_energy_summary.py
--rw-r--r--   0 kumagai    (501) staff       (20)     6480 2022-11-19 06:15:43.000000 pydefect-0.9.3/pydefect/analyzer/make_defect_structure_info.py
--rw-r--r--   0 kumagai    (501) staff       (20)      787 2022-12-08 07:12:16.000000 pydefect-0.9.3/pydefect/analyzer/pinning_levels.py
--rw-r--r--   0 kumagai    (501) staff       (20)     1575 2021-04-27 05:43:07.000000 pydefect-0.9.3/pydefect/analyzer/refine_defect_structure.py
--rw-r--r--   0 kumagai    (501) staff       (20)     2279 2022-11-16 04:21:58.000000 pydefect-0.9.3/pydefect/analyzer/transition_levels.py
--rw-r--r--   0 kumagai    (501) staff       (20)     2006 2022-11-16 04:21:59.000000 pydefect-0.9.3/pydefect/analyzer/transition_levels_plotter.py
--rw-r--r--   0 kumagai    (501) staff       (20)     2128 2023-03-26 01:17:24.000000 pydefect-0.9.3/pydefect/analyzer/unitcell.py
-drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2024-03-31 01:55:41.979216 pydefect-0.9.3/pydefect/chem_pot_diag/
--rw-r--r--   0 kumagai    (501) staff       (20)       95 2020-05-18 00:09:10.000000 pydefect-0.9.3/pydefect/chem_pot_diag/__init__.py
--rw-r--r--   0 kumagai    (501) staff       (20)    15678 2023-01-04 05:04:29.000000 pydefect-0.9.3/pydefect/chem_pot_diag/chem_pot_diag.py
--rw-r--r--   0 kumagai    (501) staff       (20)     5575 2023-11-30 04:00:39.000000 pydefect-0.9.3/pydefect/chem_pot_diag/cpd_plotter.py
-drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2024-03-31 01:55:41.987382 pydefect-0.9.3/pydefect/cli/
--rw-r--r--   0 kumagai    (501) staff       (20)       95 2020-05-18 00:09:10.000000 pydefect-0.9.3/pydefect/cli/__init__.py
--rw-r--r--   0 kumagai    (501) staff       (20)    15952 2023-11-08 22:35:02.000000 pydefect-0.9.3/pydefect/cli/main.py
--rw-r--r--   0 kumagai    (501) staff       (20)    10978 2023-11-30 00:31:21.000000 pydefect-0.9.3/pydefect/cli/main_functions.py
--rw-r--r--   0 kumagai    (501) staff       (20)      497 2023-09-05 22:31:29.000000 pydefect-0.9.3/pydefect/cli/main_print_json.py
--rw-r--r--   0 kumagai    (501) staff       (20)     2248 2023-09-23 22:34:14.000000 pydefect-0.9.3/pydefect/cli/main_tools.py
--rw-r--r--   0 kumagai    (501) staff       (20)     9985 2023-09-20 06:33:01.000000 pydefect-0.9.3/pydefect/cli/main_util.py
--rw-r--r--   0 kumagai    (501) staff       (20)     6846 2023-08-25 03:46:50.000000 pydefect-0.9.3/pydefect/cli/main_util_functions.py
--rw-r--r--   0 kumagai    (501) staff       (20)     4923 2021-05-02 06:20:14.000000 pydefect-0.9.3/pydefect/cli/make_defect_vesta_file.py
-drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2024-03-31 01:55:42.007005 pydefect-0.9.3/pydefect/cli/vasp/
--rw-r--r--   0 kumagai    (501) staff       (20)        0 2020-05-26 08:41:03.000000 pydefect-0.9.3/pydefect/cli/vasp/__init__.py
--rwxr-xr-x   0 kumagai    (501) staff       (20)     1017 2021-04-29 04:10:12.000000 pydefect-0.9.3/pydefect/cli/vasp/get_defect_charge_state.py
--rw-r--r--   0 kumagai    (501) staff       (20)     9144 2022-11-22 04:59:04.000000 pydefect-0.9.3/pydefect/cli/vasp/main_vasp.py
--rw-r--r--   0 kumagai    (501) staff       (20)     7734 2023-11-09 01:06:37.000000 pydefect-0.9.3/pydefect/cli/vasp/main_vasp_functions.py
--rw-r--r--   0 kumagai    (501) staff       (20)     5798 2023-05-28 21:33:53.000000 pydefect-0.9.3/pydefect/cli/vasp/main_vasp_util.py
--rw-r--r--   0 kumagai    (501) staff       (20)     4378 2023-11-11 01:31:20.000000 pydefect-0.9.3/pydefect/cli/vasp/main_vasp_util_functions.py
--rw-r--r--   0 kumagai    (501) staff       (20)     4865 2023-11-09 01:05:53.000000 pydefect-0.9.3/pydefect/cli/vasp/make_band_edge_orbital_infos.py
--rw-r--r--   0 kumagai    (501) staff       (20)      690 2021-04-13 03:41:39.000000 pydefect-0.9.3/pydefect/cli/vasp/make_calc_results.py
--rw-r--r--   0 kumagai    (501) staff       (20)     2209 2024-03-31 01:52:37.000000 pydefect-0.9.3/pydefect/cli/vasp/make_composition_energies_from_mp.py
--rw-r--r--   0 kumagai    (501) staff       (20)     2754 2021-05-24 05:42:28.000000 pydefect-0.9.3/pydefect/cli/vasp/make_defect_charge_info.py
--rw-r--r--   0 kumagai    (501) staff       (20)     4546 2023-11-08 22:33:43.000000 pydefect-0.9.3/pydefect/cli/vasp/make_efnv_correction.py
--rw-r--r--   0 kumagai    (501) staff       (20)     2647 2023-09-20 06:28:25.000000 pydefect-0.9.3/pydefect/cli/vasp/make_gkfo_correction.py
--rw-r--r--   0 kumagai    (501) staff       (20)    18753 2023-11-30 03:58:28.000000 pydefect-0.9.3/pydefect/cli/vasp/make_local_extrema.py
--rw-r--r--   0 kumagai    (501) staff       (20)     1349 2021-08-06 10:14:07.000000 pydefect-0.9.3/pydefect/cli/vasp/make_perfect_band_edge_state.py
--rw-r--r--   0 kumagai    (501) staff       (20)     2433 2023-12-04 03:00:30.000000 pydefect-0.9.3/pydefect/cli/vasp/make_poscars_from_query.py
--rw-r--r--   0 kumagai    (501) staff       (20)     1156 2021-04-25 05:20:51.000000 pydefect-0.9.3/pydefect/cli/vasp/make_unitcell.py
-drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2024-03-31 01:55:42.009545 pydefect-0.9.3/pydefect/cli/vasp/molecules/
-drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2024-03-31 01:55:42.011198 pydefect-0.9.3/pydefect/cli/vasp/molecules/H2/
--rw-r--r--   0 kumagai    (501) staff       (20)      501 2020-12-04 01:34:20.000000 pydefect-0.9.3/pydefect/cli/vasp/molecules/H2/POSCAR
--rw-r--r--   0 kumagai    (501) staff       (20)       17 2020-05-15 22:52:05.000000 pydefect-0.9.3/pydefect/cli/vasp/molecules/H2/prior_info.yaml
-drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2024-03-31 01:55:42.012976 pydefect-0.9.3/pydefect/cli/vasp/molecules/H2O/
--rw-r--r--   0 kumagai    (501) staff       (20)      618 2020-05-15 22:52:05.000000 pydefect-0.9.3/pydefect/cli/vasp/molecules/H2O/POSCAR
--rw-r--r--   0 kumagai    (501) staff       (20)       17 2020-05-15 22:52:05.000000 pydefect-0.9.3/pydefect/cli/vasp/molecules/H2O/prior_info.yaml
-drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2024-03-31 01:55:42.014814 pydefect-0.9.3/pydefect/cli/vasp/molecules/N2/
--rw-r--r--   0 kumagai    (501) staff       (20)      501 2020-05-15 22:52:05.000000 pydefect-0.9.3/pydefect/cli/vasp/molecules/N2/POSCAR
--rw-r--r--   0 kumagai    (501) staff       (20)       17 2020-05-15 22:52:05.000000 pydefect-0.9.3/pydefect/cli/vasp/molecules/N2/prior_info.yaml
-drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2024-03-31 01:55:42.017032 pydefect-0.9.3/pydefect/cli/vasp/molecules/NH3/
--rw-r--r--   0 kumagai    (501) staff       (20)      733 2020-05-15 22:52:05.000000 pydefect-0.9.3/pydefect/cli/vasp/molecules/NH3/POSCAR
--rw-r--r--   0 kumagai    (501) staff       (20)       17 2020-05-15 22:52:05.000000 pydefect-0.9.3/pydefect/cli/vasp/molecules/NH3/prior_info.yaml
-drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2024-03-31 01:55:42.019322 pydefect-0.9.3/pydefect/cli/vasp/molecules/NO2/
--rw-r--r--   0 kumagai    (501) staff       (20)      623 2020-05-15 22:52:05.000000 pydefect-0.9.3/pydefect/cli/vasp/molecules/NO2/POSCAR
--rw-r--r--   0 kumagai    (501) staff       (20)       17 2020-05-15 22:52:05.000000 pydefect-0.9.3/pydefect/cli/vasp/molecules/NO2/prior_info.yaml
-drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2024-03-31 01:55:42.021852 pydefect-0.9.3/pydefect/cli/vasp/molecules/O2/
--rw-r--r--   0 kumagai    (501) staff       (20)      501 2020-05-15 22:52:05.000000 pydefect-0.9.3/pydefect/cli/vasp/molecules/O2/POSCAR
--rw-r--r--   0 kumagai    (501) staff       (20)       49 2020-05-15 22:52:05.000000 pydefect-0.9.3/pydefect/cli/vasp/molecules/O2/prior_info.yaml
--rw-r--r--   0 kumagai    (501) staff       (20)       95 2020-05-26 08:59:11.000000 pydefect-0.9.3/pydefect/cli/vasp/molecules/__init__.py
--rw-r--r--   0 kumagai    (501) staff       (20)      729 2020-05-15 22:52:05.000000 pydefect-0.9.3/pydefect/cli/vasp/molecules/molecule_data.yaml
--rw-r--r--   0 kumagai    (501) staff       (20)      417 2020-05-26 08:59:40.000000 pydefect-0.9.3/pydefect/cli/vasp/molecules/molecules.py
-drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2024-03-31 01:55:42.029497 pydefect-0.9.3/pydefect/corrections/
--rw-r--r--   0 kumagai    (501) staff       (20)       95 2020-05-18 00:09:10.000000 pydefect-0.9.3/pydefect/corrections/__init__.py
--rw-r--r--   0 kumagai    (501) staff       (20)      728 2023-08-21 23:57:40.000000 pydefect-0.9.3/pydefect/corrections/abstract_correction.py
--rw-r--r--   0 kumagai    (501) staff       (20)     2042 2023-09-20 06:21:53.000000 pydefect-0.9.3/pydefect/corrections/efnv_correction.py
--rw-r--r--   0 kumagai    (501) staff       (20)     4802 2020-06-06 00:50:29.000000 pydefect-0.9.3/pydefect/corrections/ewald.py
--rw-r--r--   0 kumagai    (501) staff       (20)     2875 2020-11-26 00:07:11.000000 pydefect-0.9.3/pydefect/corrections/gkfo_correction.py
--rw-r--r--   0 kumagai    (501) staff       (20)      306 2023-06-28 00:22:41.000000 pydefect-0.9.3/pydefect/corrections/no_correction.py
--rw-r--r--   0 kumagai    (501) staff       (20)     6967 2023-11-30 00:15:21.000000 pydefect-0.9.3/pydefect/corrections/site_potential_plotter.py
-drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2024-03-31 01:55:42.035433 pydefect-0.9.3/pydefect/database/
--rw-r--r--   0 kumagai    (501) staff       (20)       95 2020-05-18 00:09:10.000000 pydefect-0.9.3/pydefect/database/__init__.py
--rw-r--r--   0 kumagai    (501) staff       (20)      808 2021-04-28 23:15:40.000000 pydefect-0.9.3/pydefect/database/database.py
--rw-r--r--   0 kumagai    (501) staff       (20)      985 2020-05-15 01:50:57.000000 pydefect-0.9.3/pydefect/database/electronegativity.yaml
--rw-r--r--   0 kumagai    (501) staff       (20)      467 2021-05-08 04:43:11.000000 pydefect-0.9.3/pydefect/database/oxidation_state.yaml
--rw-r--r--   0 kumagai    (501) staff       (20)     1073 2020-05-15 01:46:44.000000 pydefect-0.9.3/pydefect/database/rcore.yaml
--rw-r--r--   0 kumagai    (501) staff       (20)     2982 2021-06-10 06:38:20.000000 pydefect-0.9.3/pydefect/defaults.py
--rw-r--r--   0 kumagai    (501) staff       (20)      138 2020-05-13 06:54:40.000000 pydefect-0.9.3/pydefect/error.py
-drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2024-03-31 01:55:42.048712 pydefect-0.9.3/pydefect/input_maker/
--rw-r--r--   0 kumagai    (501) staff       (20)        0 2020-05-14 10:45:24.000000 pydefect-0.9.3/pydefect/input_maker/__init__.py
--rw-r--r--   0 kumagai    (501) staff       (20)     2252 2022-11-04 06:49:00.000000 pydefect-0.9.3/pydefect/input_maker/append_interstitial.py
--rw-r--r--   0 kumagai    (501) staff       (20)     2011 2023-03-13 01:10:20.000000 pydefect-0.9.3/pydefect/input_maker/complex_defect_entries_make.py
--rw-r--r--   0 kumagai    (501) staff       (20)     1178 2023-03-12 23:38:44.000000 pydefect-0.9.3/pydefect/input_maker/complex_defect_set.py
--rw-r--r--   0 kumagai    (501) staff       (20)     1509 2022-09-30 06:02:01.000000 pydefect-0.9.3/pydefect/input_maker/defect.py
--rw-r--r--   0 kumagai    (501) staff       (20)     5794 2022-09-30 06:04:45.000000 pydefect-0.9.3/pydefect/input_maker/defect_entries_maker.py
--rw-r--r--   0 kumagai    (501) staff       (20)     4655 2022-09-30 06:27:37.000000 pydefect-0.9.3/pydefect/input_maker/defect_entry.py
--rw-r--r--   0 kumagai    (501) staff       (20)     1464 2022-07-01 01:20:02.000000 pydefect-0.9.3/pydefect/input_maker/defect_set.py
--rw-r--r--   0 kumagai    (501) staff       (20)     3918 2020-11-23 04:55:46.000000 pydefect-0.9.3/pydefect/input_maker/defect_set_maker.py
--rw-r--r--   0 kumagai    (501) staff       (20)     2305 2021-08-06 10:14:07.000000 pydefect-0.9.3/pydefect/input_maker/local_extrema.py
--rw-r--r--   0 kumagai    (501) staff       (20)     3149 2023-01-28 01:22:10.000000 pydefect-0.9.3/pydefect/input_maker/manual_supercell_maker.py
--rw-r--r--   0 kumagai    (501) staff       (20)     3938 2023-01-28 00:19:05.000000 pydefect-0.9.3/pydefect/input_maker/supercell.py
--rw-r--r--   0 kumagai    (501) staff       (20)     4242 2023-01-28 01:11:46.000000 pydefect-0.9.3/pydefect/input_maker/supercell_info.py
--rw-r--r--   0 kumagai    (501) staff       (20)     4772 2024-01-22 23:36:45.000000 pydefect-0.9.3/pydefect/input_maker/supercell_maker.py
-drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2024-03-31 01:55:42.050947 pydefect-0.9.3/pydefect/tests/
--rw-r--r--   0 kumagai    (501) staff       (20)        0 2020-05-14 10:39:18.000000 pydefect-0.9.3/pydefect/tests/__init__.py
-drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2024-03-31 01:55:42.073831 pydefect-0.9.3/pydefect/tests/analyzer/
--rw-r--r--   0 kumagai    (501) staff       (20)     1983 2022-09-30 04:57:26.000000 pydefect-0.9.3/pydefect/tests/analyzer/POSCAR
--rw-r--r--   0 kumagai    (501) staff       (20)       61 2020-08-03 11:12:30.000000 pydefect-0.9.3/pydefect/tests/analyzer/__init__.py
-drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2024-03-31 01:55:42.079501 pydefect-0.9.3/pydefect/tests/analyzer/concentration/
--rw-r--r--   0 kumagai    (501) staff       (20)       61 2023-01-30 01:05:35.000000 pydefect-0.9.3/pydefect/tests/analyzer/concentration/__init__.py
--rw-r--r--   0 kumagai    (501) staff       (20)     3177 2023-02-02 23:17:57.000000 pydefect-0.9.3/pydefect/tests/analyzer/concentration/test_concentration.py
--rw-r--r--   0 kumagai    (501) staff       (20)     1723 2023-02-01 00:50:07.000000 pydefect-0.9.3/pydefect/tests/analyzer/concentration/test_degeneracy.py
--rw-r--r--   0 kumagai    (501) staff       (20)      469 2023-01-30 01:09:25.000000 pydefect-0.9.3/pydefect/tests/analyzer/concentration/test_distribution_function.py
--rw-r--r--   0 kumagai    (501) staff       (20)     3239 2023-03-05 02:07:50.000000 pydefect-0.9.3/pydefect/tests/analyzer/concentration/test_make_concentration.py
--rw-r--r--   0 kumagai    (501) staff       (20)      975 2023-02-08 06:50:25.000000 pydefect-0.9.3/pydefect/tests/analyzer/concentration/test_plot_concentration.py
--rw-r--r--   0 kumagai    (501) staff       (20)     7574 2023-11-09 00:41:22.000000 pydefect-0.9.3/pydefect/tests/analyzer/test_band_edge_states.py
--rw-r--r--   0 kumagai    (501) staff       (20)     1022 2021-08-06 10:14:07.000000 pydefect-0.9.3/pydefect/tests/analyzer/test_calc_results.py
--rw-r--r--   0 kumagai    (501) staff       (20)     2402 2021-05-26 07:04:12.000000 pydefect-0.9.3/pydefect/tests/analyzer/test_calc_summary.py
--rw-r--r--   0 kumagai    (501) staff       (20)     2915 2021-05-03 01:56:28.000000 pydefect-0.9.3/pydefect/tests/analyzer/test_defect_charge_info.py
--rw-r--r--   0 kumagai    (501) staff       (20)     8261 2023-06-29 09:24:13.000000 pydefect-0.9.3/pydefect/tests/analyzer/test_defect_energy.py
--rw-r--r--   0 kumagai    (501) staff       (20)     2027 2023-11-30 04:00:24.000000 pydefect-0.9.3/pydefect/tests/analyzer/test_defect_energy_plotter.py
--rw-r--r--   0 kumagai    (501) staff       (20)     1540 2022-11-15 04:49:34.000000 pydefect-0.9.3/pydefect/tests/analyzer/test_defect_energy_util.py
--rw-r--r--   0 kumagai    (501) staff       (20)     7391 2022-09-30 04:57:30.000000 pydefect-0.9.3/pydefect/tests/analyzer/test_defect_structure_comparator.py
--rw-r--r--   0 kumagai    (501) staff       (20)     4373 2023-01-29 23:13:01.000000 pydefect-0.9.3/pydefect/tests/analyzer/test_defect_structure_info.py
--rw-r--r--   0 kumagai    (501) staff       (20)     2267 2023-11-30 00:13:23.000000 pydefect-0.9.3/pydefect/tests/analyzer/test_eigenvalue_plotter.py
--rw-r--r--   0 kumagai    (501) staff       (20)     2648 2021-08-06 10:14:07.000000 pydefect-0.9.3/pydefect/tests/analyzer/test_grids.py
--rw-r--r--   0 kumagai    (501) staff       (20)     7215 2022-11-22 05:40:58.000000 pydefect-0.9.3/pydefect/tests/analyzer/test_make_band_edge_states.py
--rw-r--r--   0 kumagai    (501) staff       (20)     1786 2021-08-06 10:14:07.000000 pydefect-0.9.3/pydefect/tests/analyzer/test_make_calc_summary.py
--rw-r--r--   0 kumagai    (501) staff       (20)     2067 2021-08-06 10:14:07.000000 pydefect-0.9.3/pydefect/tests/analyzer/test_make_defect_energy_info.py
--rw-r--r--   0 kumagai    (501) staff       (20)     1609 2023-06-29 09:17:41.000000 pydefect-0.9.3/pydefect/tests/analyzer/test_make_defect_energy_summary.py
--rw-r--r--   0 kumagai    (501) staff       (20)     1665 2022-09-30 05:50:49.000000 pydefect-0.9.3/pydefect/tests/analyzer/test_make_defect_structure_info.py
--rw-r--r--   0 kumagai    (501) staff       (20)     1465 2022-12-08 07:12:16.000000 pydefect-0.9.3/pydefect/tests/analyzer/test_pinning_levels.py
--rw-r--r--   0 kumagai    (501) staff       (20)     4262 2022-05-20 02:54:43.000000 pydefect-0.9.3/pydefect/tests/analyzer/test_refine_defect_structure.py
--rw-r--r--   0 kumagai    (501) staff       (20)     1796 2022-11-16 04:14:17.000000 pydefect-0.9.3/pydefect/tests/analyzer/test_transition_levels.py
--rw-r--r--   0 kumagai    (501) staff       (20)     1539 2022-11-16 04:16:01.000000 pydefect-0.9.3/pydefect/tests/analyzer/test_transition_levels_plotter.py
--rw-r--r--   0 kumagai    (501) staff       (20)     2014 2023-05-10 06:40:55.000000 pydefect-0.9.3/pydefect/tests/analyzer/test_unitcell.py
-drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2024-03-31 01:55:42.080400 pydefect-0.9.3/pydefect/tests/chem_pot_diag/
--rw-r--r--   0 kumagai    (501) staff       (20)      169 2020-11-30 07:08:52.000000 pydefect-0.9.3/pydefect/tests/chem_pot_diag/cpd.yaml
-drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2024-03-31 01:55:42.088524 pydefect-0.9.3/pydefect/tests/cli/
--rw-r--r--   0 kumagai    (501) staff       (20)       95 2020-05-18 00:09:10.000000 pydefect-0.9.3/pydefect/tests/cli/__init__.py
--rw-r--r--   0 kumagai    (501) staff       (20)    10359 2023-11-08 22:17:17.000000 pydefect-0.9.3/pydefect/tests/cli/test_main.py
--rw-r--r--   0 kumagai    (501) staff       (20)    11282 2023-11-08 22:16:01.000000 pydefect-0.9.3/pydefect/tests/cli/test_main_functions.py
--rw-r--r--   0 kumagai    (501) staff       (20)     1980 2022-10-10 09:24:54.000000 pydefect-0.9.3/pydefect/tests/cli/test_main_tools.py
--rw-r--r--   0 kumagai    (501) staff       (20)     5032 2023-11-09 01:04:55.000000 pydefect-0.9.3/pydefect/tests/cli/test_main_util.py
--rw-r--r--   0 kumagai    (501) staff       (20)     5312 2023-09-20 06:33:01.000000 pydefect-0.9.3/pydefect/tests/cli/test_main_util_functions.py
--rw-r--r--   0 kumagai    (501) staff       (20)     3011 2021-05-15 12:24:21.000000 pydefect-0.9.3/pydefect/tests/cli/test_make_defect_vesta_file.py
-drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2024-03-31 01:55:42.106142 pydefect-0.9.3/pydefect/tests/cli/vasp/
--rw-r--r--   0 kumagai    (501) staff       (20)       95 2020-05-18 00:09:10.000000 pydefect-0.9.3/pydefect/tests/cli/vasp/__init__.py
--rwxr-xr-x   0 kumagai    (501) staff       (20)     1671 2021-08-06 10:14:07.000000 pydefect-0.9.3/pydefect/tests/cli/vasp/test_get_defect_charge_state.py
--rw-r--r--   0 kumagai    (501) staff       (20)     4907 2022-11-22 04:59:59.000000 pydefect-0.9.3/pydefect/tests/cli/vasp/test_main_vasp.py
--rw-r--r--   0 kumagai    (501) staff       (20)    10434 2023-11-09 01:02:43.000000 pydefect-0.9.3/pydefect/tests/cli/vasp/test_main_vasp_functions.py
--rw-r--r--   0 kumagai    (501) staff       (20)     2779 2023-05-28 21:34:46.000000 pydefect-0.9.3/pydefect/tests/cli/vasp/test_main_vasp_util.py
--rw-r--r--   0 kumagai    (501) staff       (20)     5041 2023-05-28 21:34:15.000000 pydefect-0.9.3/pydefect/tests/cli/vasp/test_main_vasp_util_functions.py
--rw-r--r--   0 kumagai    (501) staff       (20)     7433 2023-11-09 00:30:18.000000 pydefect-0.9.3/pydefect/tests/cli/vasp/test_make_band_edge_orbital_infos.py
--rw-r--r--   0 kumagai    (501) staff       (20)      873 2023-03-26 01:11:16.000000 pydefect-0.9.3/pydefect/tests/cli/vasp/test_make_calc_results.py
--rw-r--r--   0 kumagai    (501) staff       (20)     2700 2024-03-31 01:49:22.000000 pydefect-0.9.3/pydefect/tests/cli/vasp/test_make_composition_energies_from_mp.py
--rw-r--r--   0 kumagai    (501) staff       (20)     2164 2021-08-06 10:10:20.000000 pydefect-0.9.3/pydefect/tests/cli/vasp/test_make_defect_charge_info.py
--rw-r--r--   0 kumagai    (501) staff       (20)     2385 2021-03-05 09:52:57.000000 pydefect-0.9.3/pydefect/tests/cli/vasp/test_make_efnv_correction.py
--rw-r--r--   0 kumagai    (501) staff       (20)     1619 2021-04-12 08:07:10.000000 pydefect-0.9.3/pydefect/tests/cli/vasp/test_make_gkfo_correction.py
--rw-r--r--   0 kumagai    (501) staff       (20)     2178 2021-04-29 04:12:46.000000 pydefect-0.9.3/pydefect/tests/cli/vasp/test_make_local_extrema.py
--rw-r--r--   0 kumagai    (501) staff       (20)     1429 2023-03-26 01:11:16.000000 pydefect-0.9.3/pydefect/tests/cli/vasp/test_make_perfect_band_edge_state.py
--rw-r--r--   0 kumagai    (501) staff       (20)     1557 2022-05-20 02:54:43.000000 pydefect-0.9.3/pydefect/tests/cli/vasp/test_make_poscars_from_query.py
--rw-r--r--   0 kumagai    (501) staff       (20)     1538 2023-03-26 01:11:16.000000 pydefect-0.9.3/pydefect/tests/cli/vasp/test_make_unitcell.py
--rw-r--r--   0 kumagai    (501) staff       (20)      216 2021-04-23 05:16:53.000000 pydefect-0.9.3/pydefect/tests/cli/vasp/unitcell.yaml
-drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2024-03-31 01:55:41.936121 pydefect-0.9.3/pydefect/tests/cli/vasp/vasp_files/
-drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2024-03-31 01:55:42.107426 pydefect-0.9.3/pydefect/tests/cli/vasp/vasp_files/KInO2_Va_O_2/
--rw-r--r--   0 kumagai    (501) staff       (20)       18 2020-05-31 08:54:40.000000 pydefect-0.9.3/pydefect/tests/cli/vasp/vasp_files/KInO2_Va_O_2/pydefect.yaml
--rw-r--r--   0 kumagai    (501) staff       (20)    14382 2023-05-10 00:54:37.000000 pydefect-0.9.3/pydefect/tests/conftest.py
-drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2024-03-31 01:55:42.114251 pydefect-0.9.3/pydefect/tests/corrections/
--rw-r--r--   0 kumagai    (501) staff       (20)       61 2020-06-14 07:43:24.000000 pydefect-0.9.3/pydefect/tests/corrections/__init__.py
--rw-r--r--   0 kumagai    (501) staff       (20)     1723 2021-04-26 01:56:50.000000 pydefect-0.9.3/pydefect/tests/corrections/test_efnv_correction.py
--rw-r--r--   0 kumagai    (501) staff       (20)      963 2020-06-05 00:53:04.000000 pydefect-0.9.3/pydefect/tests/corrections/test_efnv_performance.py
--rw-r--r--   0 kumagai    (501) staff       (20)     3613 2021-03-02 02:40:28.000000 pydefect-0.9.3/pydefect/tests/corrections/test_ewald.py
--rw-r--r--   0 kumagai    (501) staff       (20)     2549 2020-11-25 07:07:18.000000 pydefect-0.9.3/pydefect/tests/corrections/test_gkfo_correction.py
--rw-r--r--   0 kumagai    (501) staff       (20)     2053 2023-11-30 00:17:18.000000 pydefect-0.9.3/pydefect/tests/corrections/test_site_potential_plotter.py
-drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2024-03-31 01:55:42.115094 pydefect-0.9.3/pydefect/tests/helpers/
--rw-r--r--   0 kumagai    (501) staff       (20)        0 2020-05-14 10:39:18.000000 pydefect-0.9.3/pydefect/tests/helpers/__init__.py
-drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2024-03-31 01:55:42.130614 pydefect-0.9.3/pydefect/tests/input_maker/
--rw-r--r--   0 kumagai    (501) staff       (20)      347 2020-08-05 23:35:58.000000 pydefect-0.9.3/pydefect/tests/input_maker/POSCAR
--rw-r--r--   0 kumagai    (501) staff       (20)        0 2020-05-14 10:46:18.000000 pydefect-0.9.3/pydefect/tests/input_maker/__init__.py
--rw-r--r--   0 kumagai    (501) staff       (20)     2704 2021-04-28 11:25:22.000000 pydefect-0.9.3/pydefect/tests/input_maker/test_append_interstitial.py
--rw-r--r--   0 kumagai    (501) staff       (20)     1923 2023-03-13 01:10:15.000000 pydefect-0.9.3/pydefect/tests/input_maker/test_complex_defect_entries_make.py
--rw-r--r--   0 kumagai    (501) staff       (20)      810 2023-03-13 00:52:36.000000 pydefect-0.9.3/pydefect/tests/input_maker/test_complex_defect_set.py
--rw-r--r--   0 kumagai    (501) staff       (20)     1230 2022-09-30 06:02:25.000000 pydefect-0.9.3/pydefect/tests/input_maker/test_defect.py
--rw-r--r--   0 kumagai    (501) staff       (20)     5834 2021-08-06 10:14:07.000000 pydefect-0.9.3/pydefect/tests/input_maker/test_defect_entries_maker.py
--rw-r--r--   0 kumagai    (501) staff       (20)     4367 2022-09-30 06:12:21.000000 pydefect-0.9.3/pydefect/tests/input_maker/test_defect_entry.py
--rw-r--r--   0 kumagai    (501) staff       (20)     1551 2022-07-01 01:20:10.000000 pydefect-0.9.3/pydefect/tests/input_maker/test_defect_set.py
--rw-r--r--   0 kumagai    (501) staff       (20)     2139 2020-12-23 03:22:55.000000 pydefect-0.9.3/pydefect/tests/input_maker/test_defect_set_maker.py
--rw-r--r--   0 kumagai    (501) staff       (20)     4174 2021-08-06 10:11:01.000000 pydefect-0.9.3/pydefect/tests/input_maker/test_local_extrema.py
--rw-r--r--   0 kumagai    (501) staff       (20)     2368 2023-01-28 01:19:23.000000 pydefect-0.9.3/pydefect/tests/input_maker/test_manual_supercell_maker.py
--rw-r--r--   0 kumagai    (501) staff       (20)     3571 2021-03-05 09:52:57.000000 pydefect-0.9.3/pydefect/tests/input_maker/test_supercell.py
--rw-r--r--   0 kumagai    (501) staff       (20)     4443 2023-01-27 05:27:59.000000 pydefect-0.9.3/pydefect/tests/input_maker/test_supercell_info.py
--rw-r--r--   0 kumagai    (501) staff       (20)     5393 2023-05-19 23:41:13.000000 pydefect-0.9.3/pydefect/tests/input_maker/test_supercell_maker.py
-drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2024-03-31 01:55:41.937066 pydefect-0.9.3/pydefect/tests/test_data_files/
-drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2024-03-31 01:55:42.131802 pydefect-0.9.3/pydefect/tests/test_data_files/Na3AgO2/
--rw-r--r--   0 kumagai    (501) staff       (20)     3145 2023-01-31 23:38:38.000000 pydefect-0.9.3/pydefect/tests/test_data_files/Na3AgO2/degeneracies.yaml
-drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2024-03-31 01:55:42.138312 pydefect-0.9.3/pydefect/util/
--rw-r--r--   0 kumagai    (501) staff       (20)       95 2020-05-26 03:04:22.000000 pydefect-0.9.3/pydefect/util/__init__.py
--rw-r--r--   0 kumagai    (501) staff       (20)      245 2021-04-06 09:47:19.000000 pydefect-0.9.3/pydefect/util/coords.py
--rw-r--r--   0 kumagai    (501) staff       (20)      351 2023-11-08 22:28:42.000000 pydefect-0.9.3/pydefect/util/error_classes.py
--rw-r--r--   0 kumagai    (501) staff       (20)     1368 2024-03-28 22:12:26.000000 pydefect-0.9.3/pydefect/util/mp_tools.py
--rw-r--r--   0 kumagai    (501) staff       (20)     2457 2023-11-30 00:19:15.000000 pydefect-0.9.3/pydefect/util/prepare_names.py
--rw-r--r--   0 kumagai    (501) staff       (20)     2727 2021-04-26 23:23:36.000000 pydefect-0.9.3/pydefect/util/structure_tools.py
-drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2024-03-31 01:55:41.950535 pydefect-0.9.3/pydefect.egg-info/
--rw-r--r--   0 kumagai    (501) staff       (20)      397 2024-03-31 01:55:36.000000 pydefect-0.9.3/pydefect.egg-info/PKG-INFO
--rw-r--r--   0 kumagai    (501) staff       (20)    10832 2024-03-31 01:55:41.000000 pydefect-0.9.3/pydefect.egg-info/SOURCES.txt
--rw-r--r--   0 kumagai    (501) staff       (20)        1 2024-03-31 01:55:36.000000 pydefect-0.9.3/pydefect.egg-info/dependency_links.txt
--rw-r--r--   0 kumagai    (501) staff       (20)      256 2024-03-31 01:55:36.000000 pydefect-0.9.3/pydefect.egg-info/entry_points.txt
--rw-r--r--   0 kumagai    (501) staff       (20)       69 2024-03-31 01:55:36.000000 pydefect-0.9.3/pydefect.egg-info/requires.txt
--rw-r--r--   0 kumagai    (501) staff       (20)        9 2024-03-31 01:55:36.000000 pydefect-0.9.3/pydefect.egg-info/top_level.txt
--rw-r--r--   0 kumagai    (501) staff       (20)       38 2024-03-31 01:55:42.190625 pydefect-0.9.3/setup.cfg
--rw-r--r--   0 kumagai    (501) staff       (20)     1335 2021-08-06 00:13:51.000000 pydefect-0.9.3/setup.py
-drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2024-03-31 01:55:41.937780 pydefect-0.9.3/venv/
-drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2024-03-31 01:55:41.938100 pydefect-0.9.3/venv/lib/
-drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2024-03-31 01:55:41.938440 pydefect-0.9.3/venv/lib/python3.10/
-drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2024-03-31 01:55:41.940450 pydefect-0.9.3/venv/lib/python3.10/site-packages/
-drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2024-03-31 01:55:41.939056 pydefect-0.9.3/venv/lib/python3.10/site-packages/emmet/
-drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2024-03-31 01:55:41.939232 pydefect-0.9.3/venv/lib/python3.10/site-packages/emmet/core/
-drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2024-03-31 01:55:41.939448 pydefect-0.9.3/venv/lib/python3.10/site-packages/emmet/core/vasp/
-drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2024-03-31 01:55:42.139578 pydefect-0.9.3/venv/lib/python3.10/site-packages/emmet/core/vasp/calc_types/
--rw-r--r--   0 kumagai    (501) staff       (20)     1733 2023-11-30 07:24:35.000000 pydefect-0.9.3/venv/lib/python3.10/site-packages/emmet/core/vasp/calc_types/run_types.yaml
-drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2024-03-31 01:55:41.940024 pydefect-0.9.3/venv/lib/python3.10/site-packages/maggma/
-drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2024-03-31 01:55:42.140584 pydefect-0.9.3/venv/lib/python3.10/site-packages/maggma/api/
--rw-r--r--   0 kumagai    (501) staff       (20)     1562 2023-11-30 07:24:35.000000 pydefect-0.9.3/venv/lib/python3.10/site-packages/maggma/api/default_responses.yaml
-drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2024-03-31 01:55:41.943340 pydefect-0.9.3/venv/lib/python3.10/site-packages/pymatgen/
-drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2024-03-31 01:55:42.147120 pydefect-0.9.3/venv/lib/python3.10/site-packages/pymatgen/analysis/
--rw-r--r--   0 kumagai    (501) staff       (20)     1241 2023-11-30 03:51:15.000000 pydefect-0.9.3/venv/lib/python3.10/site-packages/pymatgen/analysis/bonds_jmol_ob.yaml
--rw-r--r--   0 kumagai    (501) staff       (20)     1770 2023-11-30 03:51:15.000000 pydefect-0.9.3/venv/lib/python3.10/site-packages/pymatgen/analysis/bvparam_1991.yaml
--rw-r--r--   0 kumagai    (501) staff       (20)     1443 2023-11-30 03:51:15.000000 pydefect-0.9.3/venv/lib/python3.10/site-packages/pymatgen/analysis/cn_opt_params.yaml
--rw-r--r--   0 kumagai    (501) staff       (20)    34095 2023-11-30 03:51:15.000000 pydefect-0.9.3/venv/lib/python3.10/site-packages/pymatgen/analysis/icsd_bv.yaml
-drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2024-03-31 01:55:42.148370 pydefect-0.9.3/venv/lib/python3.10/site-packages/pymatgen/analysis/magnetism/
--rw-r--r--   0 kumagai    (501) staff       (20)      473 2023-11-30 03:51:15.000000 pydefect-0.9.3/venv/lib/python3.10/site-packages/pymatgen/analysis/magnetism/default_magmoms.yaml
--rw-r--r--   0 kumagai    (501) staff       (20)     3096 2023-11-30 03:51:15.000000 pydefect-0.9.3/venv/lib/python3.10/site-packages/pymatgen/analysis/op_params.yaml
-drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2024-03-31 01:55:42.149347 pydefect-0.9.3/venv/lib/python3.10/site-packages/pymatgen/analysis/structure_prediction/
--rw-r--r--   0 kumagai    (501) staff       (20)     3586 2023-11-30 03:51:15.000000 pydefect-0.9.3/venv/lib/python3.10/site-packages/pymatgen/analysis/structure_prediction/DLS_bond_params.yaml
--rw-r--r--   0 kumagai    (501) staff       (20)    15599 2023-11-30 03:51:15.000000 pydefect-0.9.3/venv/lib/python3.10/site-packages/pymatgen/analysis/vesta_cutoffs.yaml
-drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2024-03-31 01:55:42.152571 pydefect-0.9.3/venv/lib/python3.10/site-packages/pymatgen/entries/
--rw-r--r--   0 kumagai    (501) staff       (20)     2000 2023-11-30 03:51:15.000000 pydefect-0.9.3/venv/lib/python3.10/site-packages/pymatgen/entries/MITCompatibility.yaml
--rw-r--r--   0 kumagai    (501) staff       (20)     1555 2023-11-30 03:51:15.000000 pydefect-0.9.3/venv/lib/python3.10/site-packages/pymatgen/entries/MP2020Compatibility.yaml
--rw-r--r--   0 kumagai    (501) staff       (20)     2206 2023-11-30 03:51:15.000000 pydefect-0.9.3/venv/lib/python3.10/site-packages/pymatgen/entries/MPCompatibility.yaml
-drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2024-03-31 01:55:41.942895 pydefect-0.9.3/venv/lib/python3.10/site-packages/pymatgen/io/
-drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2024-03-31 01:55:42.156372 pydefect-0.9.3/venv/lib/python3.10/site-packages/pymatgen/io/feff/
--rw-r--r--   0 kumagai    (501) staff       (20)      405 2023-11-30 03:51:15.000000 pydefect-0.9.3/venv/lib/python3.10/site-packages/pymatgen/io/feff/MPELNESSet.yaml
--rw-r--r--   0 kumagai    (501) staff       (20)      112 2023-11-30 03:51:15.000000 pydefect-0.9.3/venv/lib/python3.10/site-packages/pymatgen/io/feff/MPEXAFSSet.yaml
--rw-r--r--   0 kumagai    (501) staff       (20)      362 2023-11-30 03:51:15.000000 pydefect-0.9.3/venv/lib/python3.10/site-packages/pymatgen/io/feff/MPEXELFSSet.yaml
--rw-r--r--   0 kumagai    (501) staff       (20)      161 2023-11-30 03:51:15.000000 pydefect-0.9.3/venv/lib/python3.10/site-packages/pymatgen/io/feff/MPXANESSet.yaml
-drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2024-03-31 01:55:42.157703 pydefect-0.9.3/venv/lib/python3.10/site-packages/pymatgen/io/lammps/
--rw-r--r--   0 kumagai    (501) staff       (20)     9910 2023-11-30 03:51:15.000000 pydefect-0.9.3/venv/lib/python3.10/site-packages/pymatgen/io/lammps/CoeffsDataType.yaml
-drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2024-03-31 01:55:41.942627 pydefect-0.9.3/venv/lib/python3.10/site-packages/pymatgen/io/lobster/
-drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2024-03-31 01:55:42.171530 pydefect-0.9.3/venv/lib/python3.10/site-packages/pymatgen/io/lobster/lobster_basis/
--rw-r--r--   0 kumagai    (501) staff       (20)     3863 2023-11-30 03:51:15.000000 pydefect-0.9.3/venv/lib/python3.10/site-packages/pymatgen/io/lobster/lobster_basis/BASIS_PBE_54_max.yaml
--rw-r--r--   0 kumagai    (501) staff       (20)     3734 2023-11-30 03:51:15.000000 pydefect-0.9.3/venv/lib/python3.10/site-packages/pymatgen/io/lobster/lobster_basis/BASIS_PBE_54_min.yaml
--rw-r--r--   0 kumagai    (501) staff       (20)     3863 2023-11-30 03:51:15.000000 pydefect-0.9.3/venv/lib/python3.10/site-packages/pymatgen/io/lobster/lobster_basis/BASIS_PBE_54_standard.yaml
-drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2024-03-31 01:55:42.181990 pydefect-0.9.3/venv/lib/python3.10/site-packages/pymatgen/io/vasp/
--rw-r--r--   0 kumagai    (501) staff       (20)     7576 2023-11-30 03:51:15.000000 pydefect-0.9.3/venv/lib/python3.10/site-packages/pymatgen/io/vasp/MITRelaxSet.yaml
--rw-r--r--   0 kumagai    (501) staff       (20)     1772 2023-11-30 03:51:15.000000 pydefect-0.9.3/venv/lib/python3.10/site-packages/pymatgen/io/vasp/MPAbsorptionSet.yaml
--rw-r--r--   0 kumagai    (501) staff       (20)     1508 2023-11-30 03:51:15.000000 pydefect-0.9.3/venv/lib/python3.10/site-packages/pymatgen/io/vasp/MPHSERelaxSet.yaml
--rw-r--r--   0 kumagai    (501) staff       (20)     2375 2023-11-30 03:51:15.000000 pydefect-0.9.3/venv/lib/python3.10/site-packages/pymatgen/io/vasp/MPRelaxSet.yaml
--rw-r--r--   0 kumagai    (501) staff       (20)     1785 2023-11-30 03:51:15.000000 pydefect-0.9.3/venv/lib/python3.10/site-packages/pymatgen/io/vasp/MPSCANRelaxSet.yaml
--rw-r--r--   0 kumagai    (501) staff       (20)     1683 2023-11-30 03:51:15.000000 pydefect-0.9.3/venv/lib/python3.10/site-packages/pymatgen/io/vasp/MVLGWSet.yaml
--rw-r--r--   0 kumagai    (501) staff       (20)     2465 2023-11-30 03:51:15.000000 pydefect-0.9.3/venv/lib/python3.10/site-packages/pymatgen/io/vasp/MVLRelax52Set.yaml
--rw-r--r--   0 kumagai    (501) staff       (20)     1511 2023-11-30 03:51:15.000000 pydefect-0.9.3/venv/lib/python3.10/site-packages/pymatgen/io/vasp/MatPESStaticSet.yaml
--rw-r--r--   0 kumagai    (501) staff       (20)     1217 2023-11-30 03:51:15.000000 pydefect-0.9.3/venv/lib/python3.10/site-packages/pymatgen/io/vasp/PBE54Base.yaml
--rw-r--r--   0 kumagai    (501) staff       (20)      364 2023-11-30 03:51:15.000000 pydefect-0.9.3/venv/lib/python3.10/site-packages/pymatgen/io/vasp/VASPIncarBase.yaml
--rw-r--r--   0 kumagai    (501) staff       (20)      614 2023-11-30 03:51:15.000000 pydefect-0.9.3/venv/lib/python3.10/site-packages/pymatgen/io/vasp/vdW_parameters.yaml
-drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2024-03-31 01:55:42.185063 pydefect-0.9.3/venv/lib/python3.10/site-packages/pymatgen/symmetry/
--rw-r--r--   0 kumagai    (501) staff       (20)    48801 2023-11-30 03:51:15.000000 pydefect-0.9.3/venv/lib/python3.10/site-packages/pymatgen/symmetry/symm_data.yaml
--rw-r--r--   0 kumagai    (501) staff       (20)   443430 2023-11-30 03:51:15.000000 pydefect-0.9.3/venv/lib/python3.10/site-packages/pymatgen/symmetry/symm_ops.yaml
-drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2024-03-31 01:55:42.188546 pydefect-0.9.3/venv/lib/python3.10/site-packages/pymatgen/vis/
--rw-r--r--   0 kumagai    (501) staff       (20)     4494 2023-11-30 03:51:15.000000 pydefect-0.9.3/venv/lib/python3.10/site-packages/pymatgen/vis/ElementColorSchemes.yaml
+drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2024-05-07 00:39:22.157368 pydefect-0.9.4/
+-rw-r--r--   0 kumagai    (501) staff       (20)       54 2021-03-12 02:40:59.000000 pydefect-0.9.4/MANIFEST.in
+-rw-r--r--   0 kumagai    (501) staff       (20)      397 2024-05-07 00:39:22.156921 pydefect-0.9.4/PKG-INFO
+-rw-r--r--   0 kumagai    (501) staff       (20)     4571 2023-11-29 21:52:31.000000 pydefect-0.9.4/README.md
+drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2024-05-07 00:39:21.978999 pydefect-0.9.4/pydefect/
+-rw-r--r--   0 kumagai    (501) staff       (20)       21 2024-05-07 00:38:47.000000 pydefect-0.9.4/pydefect/__init__.py
+drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2024-05-07 00:39:22.002027 pydefect-0.9.4/pydefect/analyzer/
+-rw-r--r--   0 kumagai    (501) staff       (20)       95 2020-05-18 00:09:10.000000 pydefect-0.9.4/pydefect/analyzer/__init__.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     2840 2021-04-02 01:38:50.000000 pydefect-0.9.4/pydefect/analyzer/_defect_charge_distribution.py
+-rw-r--r--   0 kumagai    (501) staff       (20)    12239 2023-11-09 01:03:42.000000 pydefect-0.9.4/pydefect/analyzer/band_edge_states.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     1334 2021-05-01 01:17:09.000000 pydefect-0.9.4/pydefect/analyzer/calc_results.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     2426 2021-05-26 07:04:12.000000 pydefect-0.9.4/pydefect/analyzer/calc_summary.py
+drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2024-05-07 00:39:22.007908 pydefect-0.9.4/pydefect/analyzer/concentration/
+-rw-r--r--   0 kumagai    (501) staff       (20)       61 2023-01-30 01:05:15.000000 pydefect-0.9.4/pydefect/analyzer/concentration/__init__.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     5631 2023-02-08 05:36:42.000000 pydefect-0.9.4/pydefect/analyzer/concentration/concentration.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     2973 2023-02-01 00:50:27.000000 pydefect-0.9.4/pydefect/analyzer/concentration/degeneracy.py
+-rw-r--r--   0 kumagai    (501) staff       (20)      385 2023-01-30 01:10:12.000000 pydefect-0.9.4/pydefect/analyzer/concentration/distribution_function.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     7772 2023-02-08 07:02:02.000000 pydefect-0.9.4/pydefect/analyzer/concentration/make_concentration.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     2462 2023-03-09 04:26:39.000000 pydefect-0.9.4/pydefect/analyzer/concentration/plot_concentration.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     4716 2021-08-06 10:14:07.000000 pydefect-0.9.4/pydefect/analyzer/defect_charge_info.py
+-rw-r--r--   0 kumagai    (501) staff       (20)    13088 2023-06-29 09:23:18.000000 pydefect-0.9.4/pydefect/analyzer/defect_energy.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     7810 2024-01-26 05:08:28.000000 pydefect-0.9.4/pydefect/analyzer/defect_energy_plotter.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     1280 2022-11-15 04:48:53.000000 pydefect-0.9.4/pydefect/analyzer/defect_energy_util.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     7741 2022-09-30 05:43:38.000000 pydefect-0.9.4/pydefect/analyzer/defect_structure_comparator.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     6536 2023-01-28 01:55:02.000000 pydefect-0.9.4/pydefect/analyzer/defect_structure_info.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     6463 2023-11-29 23:55:37.000000 pydefect-0.9.4/pydefect/analyzer/eigenvalue_plotter.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     2420 2021-08-06 10:11:01.000000 pydefect-0.9.4/pydefect/analyzer/grids.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     7225 2022-11-22 05:43:00.000000 pydefect-0.9.4/pydefect/analyzer/make_band_edge_states.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     1571 2021-05-26 07:04:53.000000 pydefect-0.9.4/pydefect/analyzer/make_calc_summary.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     2390 2023-12-01 04:56:00.000000 pydefect-0.9.4/pydefect/analyzer/make_defect_energy_info.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     1716 2023-02-11 23:51:37.000000 pydefect-0.9.4/pydefect/analyzer/make_defect_energy_summary.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     6480 2022-11-19 06:15:43.000000 pydefect-0.9.4/pydefect/analyzer/make_defect_structure_info.py
+-rw-r--r--   0 kumagai    (501) staff       (20)      787 2022-12-08 07:12:16.000000 pydefect-0.9.4/pydefect/analyzer/pinning_levels.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     1575 2021-04-27 05:43:07.000000 pydefect-0.9.4/pydefect/analyzer/refine_defect_structure.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     2279 2022-11-16 04:21:58.000000 pydefect-0.9.4/pydefect/analyzer/transition_levels.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     2006 2022-11-16 04:21:59.000000 pydefect-0.9.4/pydefect/analyzer/transition_levels_plotter.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     2128 2023-03-26 01:17:24.000000 pydefect-0.9.4/pydefect/analyzer/unitcell.py
+drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2024-05-07 00:39:22.010775 pydefect-0.9.4/pydefect/chem_pot_diag/
+-rw-r--r--   0 kumagai    (501) staff       (20)       95 2020-05-18 00:09:10.000000 pydefect-0.9.4/pydefect/chem_pot_diag/__init__.py
+-rw-r--r--   0 kumagai    (501) staff       (20)    15678 2023-01-04 05:04:29.000000 pydefect-0.9.4/pydefect/chem_pot_diag/chem_pot_diag.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     5575 2024-05-07 00:36:05.000000 pydefect-0.9.4/pydefect/chem_pot_diag/cpd_plotter.py
+drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2024-05-07 00:39:22.018366 pydefect-0.9.4/pydefect/cli/
+-rw-r--r--   0 kumagai    (501) staff       (20)       95 2020-05-18 00:09:10.000000 pydefect-0.9.4/pydefect/cli/__init__.py
+-rw-r--r--   0 kumagai    (501) staff       (20)    15952 2023-11-08 22:35:02.000000 pydefect-0.9.4/pydefect/cli/main.py
+-rw-r--r--   0 kumagai    (501) staff       (20)    10978 2023-11-30 00:31:21.000000 pydefect-0.9.4/pydefect/cli/main_functions.py
+-rw-r--r--   0 kumagai    (501) staff       (20)      497 2023-09-05 22:31:29.000000 pydefect-0.9.4/pydefect/cli/main_print_json.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     2248 2024-05-05 23:26:13.000000 pydefect-0.9.4/pydefect/cli/main_tools.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     9985 2023-09-20 06:33:01.000000 pydefect-0.9.4/pydefect/cli/main_util.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     6846 2024-05-05 23:26:17.000000 pydefect-0.9.4/pydefect/cli/main_util_functions.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     4923 2021-05-02 06:20:14.000000 pydefect-0.9.4/pydefect/cli/make_defect_vesta_file.py
+drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2024-05-07 00:39:22.034882 pydefect-0.9.4/pydefect/cli/vasp/
+-rw-r--r--   0 kumagai    (501) staff       (20)        0 2020-05-26 08:41:03.000000 pydefect-0.9.4/pydefect/cli/vasp/__init__.py
+-rwxr-xr-x   0 kumagai    (501) staff       (20)     1017 2021-04-29 04:10:12.000000 pydefect-0.9.4/pydefect/cli/vasp/get_defect_charge_state.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     9144 2022-11-22 04:59:04.000000 pydefect-0.9.4/pydefect/cli/vasp/main_vasp.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     7734 2023-11-09 01:06:37.000000 pydefect-0.9.4/pydefect/cli/vasp/main_vasp_functions.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     5798 2023-05-28 21:33:53.000000 pydefect-0.9.4/pydefect/cli/vasp/main_vasp_util.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     4378 2023-11-11 01:31:20.000000 pydefect-0.9.4/pydefect/cli/vasp/main_vasp_util_functions.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     4865 2023-11-09 01:05:53.000000 pydefect-0.9.4/pydefect/cli/vasp/make_band_edge_orbital_infos.py
+-rw-r--r--   0 kumagai    (501) staff       (20)      690 2021-04-13 03:41:39.000000 pydefect-0.9.4/pydefect/cli/vasp/make_calc_results.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     2209 2024-03-31 01:52:37.000000 pydefect-0.9.4/pydefect/cli/vasp/make_composition_energies_from_mp.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     2754 2021-05-24 05:42:28.000000 pydefect-0.9.4/pydefect/cli/vasp/make_defect_charge_info.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     4484 2024-05-05 22:01:53.000000 pydefect-0.9.4/pydefect/cli/vasp/make_efnv_correction.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     2647 2023-09-20 06:28:25.000000 pydefect-0.9.4/pydefect/cli/vasp/make_gkfo_correction.py
+-rw-r--r--   0 kumagai    (501) staff       (20)    18735 2024-05-07 00:36:42.000000 pydefect-0.9.4/pydefect/cli/vasp/make_local_extrema.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     1349 2021-08-06 10:14:07.000000 pydefect-0.9.4/pydefect/cli/vasp/make_perfect_band_edge_state.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     2433 2023-12-04 03:00:30.000000 pydefect-0.9.4/pydefect/cli/vasp/make_poscars_from_query.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     1156 2021-04-25 05:20:51.000000 pydefect-0.9.4/pydefect/cli/vasp/make_unitcell.py
+drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2024-05-07 00:39:22.037254 pydefect-0.9.4/pydefect/cli/vasp/molecules/
+drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2024-05-07 00:39:22.038951 pydefect-0.9.4/pydefect/cli/vasp/molecules/H2/
+-rw-r--r--   0 kumagai    (501) staff       (20)      501 2020-12-04 01:34:20.000000 pydefect-0.9.4/pydefect/cli/vasp/molecules/H2/POSCAR
+-rw-r--r--   0 kumagai    (501) staff       (20)       17 2020-05-15 22:52:05.000000 pydefect-0.9.4/pydefect/cli/vasp/molecules/H2/prior_info.yaml
+drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2024-05-07 00:39:22.040484 pydefect-0.9.4/pydefect/cli/vasp/molecules/H2O/
+-rw-r--r--   0 kumagai    (501) staff       (20)      618 2020-05-15 22:52:05.000000 pydefect-0.9.4/pydefect/cli/vasp/molecules/H2O/POSCAR
+-rw-r--r--   0 kumagai    (501) staff       (20)       17 2020-05-15 22:52:05.000000 pydefect-0.9.4/pydefect/cli/vasp/molecules/H2O/prior_info.yaml
+drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2024-05-07 00:39:22.041950 pydefect-0.9.4/pydefect/cli/vasp/molecules/N2/
+-rw-r--r--   0 kumagai    (501) staff       (20)      501 2020-05-15 22:52:05.000000 pydefect-0.9.4/pydefect/cli/vasp/molecules/N2/POSCAR
+-rw-r--r--   0 kumagai    (501) staff       (20)       17 2020-05-15 22:52:05.000000 pydefect-0.9.4/pydefect/cli/vasp/molecules/N2/prior_info.yaml
+drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2024-05-07 00:39:22.043557 pydefect-0.9.4/pydefect/cli/vasp/molecules/NH3/
+-rw-r--r--   0 kumagai    (501) staff       (20)      733 2020-05-15 22:52:05.000000 pydefect-0.9.4/pydefect/cli/vasp/molecules/NH3/POSCAR
+-rw-r--r--   0 kumagai    (501) staff       (20)       17 2020-05-15 22:52:05.000000 pydefect-0.9.4/pydefect/cli/vasp/molecules/NH3/prior_info.yaml
+drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2024-05-07 00:39:22.044961 pydefect-0.9.4/pydefect/cli/vasp/molecules/NO2/
+-rw-r--r--   0 kumagai    (501) staff       (20)      623 2020-05-15 22:52:05.000000 pydefect-0.9.4/pydefect/cli/vasp/molecules/NO2/POSCAR
+-rw-r--r--   0 kumagai    (501) staff       (20)       17 2020-05-15 22:52:05.000000 pydefect-0.9.4/pydefect/cli/vasp/molecules/NO2/prior_info.yaml
+drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2024-05-07 00:39:22.046315 pydefect-0.9.4/pydefect/cli/vasp/molecules/O2/
+-rw-r--r--   0 kumagai    (501) staff       (20)      501 2020-05-15 22:52:05.000000 pydefect-0.9.4/pydefect/cli/vasp/molecules/O2/POSCAR
+-rw-r--r--   0 kumagai    (501) staff       (20)       49 2020-05-15 22:52:05.000000 pydefect-0.9.4/pydefect/cli/vasp/molecules/O2/prior_info.yaml
+-rw-r--r--   0 kumagai    (501) staff       (20)       95 2020-05-26 08:59:11.000000 pydefect-0.9.4/pydefect/cli/vasp/molecules/__init__.py
+-rw-r--r--   0 kumagai    (501) staff       (20)      729 2020-05-15 22:52:05.000000 pydefect-0.9.4/pydefect/cli/vasp/molecules/molecule_data.yaml
+-rw-r--r--   0 kumagai    (501) staff       (20)      417 2020-05-26 08:59:40.000000 pydefect-0.9.4/pydefect/cli/vasp/molecules/molecules.py
+drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2024-05-07 00:39:22.053323 pydefect-0.9.4/pydefect/corrections/
+-rw-r--r--   0 kumagai    (501) staff       (20)       95 2020-05-18 00:09:10.000000 pydefect-0.9.4/pydefect/corrections/__init__.py
+-rw-r--r--   0 kumagai    (501) staff       (20)      728 2023-08-21 23:57:40.000000 pydefect-0.9.4/pydefect/corrections/abstract_correction.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     2042 2023-09-20 06:21:53.000000 pydefect-0.9.4/pydefect/corrections/efnv_correction.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     4802 2020-06-06 00:50:29.000000 pydefect-0.9.4/pydefect/corrections/ewald.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     2875 2020-11-26 00:07:11.000000 pydefect-0.9.4/pydefect/corrections/gkfo_correction.py
+-rw-r--r--   0 kumagai    (501) staff       (20)      306 2023-06-28 00:22:41.000000 pydefect-0.9.4/pydefect/corrections/no_correction.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     6967 2023-11-30 00:15:21.000000 pydefect-0.9.4/pydefect/corrections/site_potential_plotter.py
+drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2024-05-07 00:39:22.057512 pydefect-0.9.4/pydefect/database/
+-rw-r--r--   0 kumagai    (501) staff       (20)       95 2020-05-18 00:09:10.000000 pydefect-0.9.4/pydefect/database/__init__.py
+-rw-r--r--   0 kumagai    (501) staff       (20)      808 2021-04-28 23:15:40.000000 pydefect-0.9.4/pydefect/database/database.py
+-rw-r--r--   0 kumagai    (501) staff       (20)      985 2020-05-15 01:50:57.000000 pydefect-0.9.4/pydefect/database/electronegativity.yaml
+-rw-r--r--   0 kumagai    (501) staff       (20)      467 2021-05-08 04:43:11.000000 pydefect-0.9.4/pydefect/database/oxidation_state.yaml
+-rw-r--r--   0 kumagai    (501) staff       (20)     1073 2020-05-15 01:46:44.000000 pydefect-0.9.4/pydefect/database/rcore.yaml
+-rw-r--r--   0 kumagai    (501) staff       (20)     2982 2024-05-05 23:23:52.000000 pydefect-0.9.4/pydefect/defaults.py
+-rw-r--r--   0 kumagai    (501) staff       (20)      138 2020-05-13 06:54:40.000000 pydefect-0.9.4/pydefect/error.py
+drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2024-05-07 00:39:22.070366 pydefect-0.9.4/pydefect/input_maker/
+-rw-r--r--   0 kumagai    (501) staff       (20)        0 2020-05-14 10:45:24.000000 pydefect-0.9.4/pydefect/input_maker/__init__.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     2252 2022-11-04 06:49:00.000000 pydefect-0.9.4/pydefect/input_maker/append_interstitial.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     2011 2023-03-13 01:10:20.000000 pydefect-0.9.4/pydefect/input_maker/complex_defect_entries_make.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     1249 2024-05-06 23:57:00.000000 pydefect-0.9.4/pydefect/input_maker/complex_defect_set.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     1509 2022-09-30 06:02:01.000000 pydefect-0.9.4/pydefect/input_maker/defect.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     5794 2022-09-30 06:04:45.000000 pydefect-0.9.4/pydefect/input_maker/defect_entries_maker.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     4655 2022-09-30 06:27:37.000000 pydefect-0.9.4/pydefect/input_maker/defect_entry.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     1464 2022-07-01 01:20:02.000000 pydefect-0.9.4/pydefect/input_maker/defect_set.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     3918 2020-11-23 04:55:46.000000 pydefect-0.9.4/pydefect/input_maker/defect_set_maker.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     2305 2021-08-06 10:14:07.000000 pydefect-0.9.4/pydefect/input_maker/local_extrema.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     3149 2023-01-28 01:22:10.000000 pydefect-0.9.4/pydefect/input_maker/manual_supercell_maker.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     3938 2023-01-28 00:19:05.000000 pydefect-0.9.4/pydefect/input_maker/supercell.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     4242 2023-01-28 01:11:46.000000 pydefect-0.9.4/pydefect/input_maker/supercell_info.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     4772 2024-01-22 23:36:45.000000 pydefect-0.9.4/pydefect/input_maker/supercell_maker.py
+drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2024-05-07 00:39:22.071992 pydefect-0.9.4/pydefect/tests/
+-rw-r--r--   0 kumagai    (501) staff       (20)        0 2020-05-14 10:39:18.000000 pydefect-0.9.4/pydefect/tests/__init__.py
+drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2024-05-07 00:39:22.093489 pydefect-0.9.4/pydefect/tests/analyzer/
+-rw-r--r--   0 kumagai    (501) staff       (20)     1983 2022-09-30 04:57:26.000000 pydefect-0.9.4/pydefect/tests/analyzer/POSCAR
+-rw-r--r--   0 kumagai    (501) staff       (20)       61 2020-08-03 11:12:30.000000 pydefect-0.9.4/pydefect/tests/analyzer/__init__.py
+drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2024-05-07 00:39:22.099245 pydefect-0.9.4/pydefect/tests/analyzer/concentration/
+-rw-r--r--   0 kumagai    (501) staff       (20)       61 2023-01-30 01:05:35.000000 pydefect-0.9.4/pydefect/tests/analyzer/concentration/__init__.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     3177 2023-02-02 23:17:57.000000 pydefect-0.9.4/pydefect/tests/analyzer/concentration/test_concentration.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     1723 2023-02-01 00:50:07.000000 pydefect-0.9.4/pydefect/tests/analyzer/concentration/test_degeneracy.py
+-rw-r--r--   0 kumagai    (501) staff       (20)      469 2023-01-30 01:09:25.000000 pydefect-0.9.4/pydefect/tests/analyzer/concentration/test_distribution_function.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     3239 2023-03-05 02:07:50.000000 pydefect-0.9.4/pydefect/tests/analyzer/concentration/test_make_concentration.py
+-rw-r--r--   0 kumagai    (501) staff       (20)      975 2023-02-08 06:50:25.000000 pydefect-0.9.4/pydefect/tests/analyzer/concentration/test_plot_concentration.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     7574 2023-11-09 00:41:22.000000 pydefect-0.9.4/pydefect/tests/analyzer/test_band_edge_states.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     1022 2021-08-06 10:14:07.000000 pydefect-0.9.4/pydefect/tests/analyzer/test_calc_results.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     2402 2021-05-26 07:04:12.000000 pydefect-0.9.4/pydefect/tests/analyzer/test_calc_summary.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     2915 2021-05-03 01:56:28.000000 pydefect-0.9.4/pydefect/tests/analyzer/test_defect_charge_info.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     8261 2023-06-29 09:24:13.000000 pydefect-0.9.4/pydefect/tests/analyzer/test_defect_energy.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     2027 2023-11-30 04:00:24.000000 pydefect-0.9.4/pydefect/tests/analyzer/test_defect_energy_plotter.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     1540 2022-11-15 04:49:34.000000 pydefect-0.9.4/pydefect/tests/analyzer/test_defect_energy_util.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     7391 2022-09-30 04:57:30.000000 pydefect-0.9.4/pydefect/tests/analyzer/test_defect_structure_comparator.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     4373 2023-01-29 23:13:01.000000 pydefect-0.9.4/pydefect/tests/analyzer/test_defect_structure_info.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     2267 2023-11-30 00:13:23.000000 pydefect-0.9.4/pydefect/tests/analyzer/test_eigenvalue_plotter.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     2648 2021-08-06 10:14:07.000000 pydefect-0.9.4/pydefect/tests/analyzer/test_grids.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     7215 2022-11-22 05:40:58.000000 pydefect-0.9.4/pydefect/tests/analyzer/test_make_band_edge_states.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     1786 2021-08-06 10:14:07.000000 pydefect-0.9.4/pydefect/tests/analyzer/test_make_calc_summary.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     2067 2021-08-06 10:14:07.000000 pydefect-0.9.4/pydefect/tests/analyzer/test_make_defect_energy_info.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     1609 2023-06-29 09:17:41.000000 pydefect-0.9.4/pydefect/tests/analyzer/test_make_defect_energy_summary.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     1665 2022-09-30 05:50:49.000000 pydefect-0.9.4/pydefect/tests/analyzer/test_make_defect_structure_info.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     1465 2022-12-08 07:12:16.000000 pydefect-0.9.4/pydefect/tests/analyzer/test_pinning_levels.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     4262 2022-05-20 02:54:43.000000 pydefect-0.9.4/pydefect/tests/analyzer/test_refine_defect_structure.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     1796 2022-11-16 04:14:17.000000 pydefect-0.9.4/pydefect/tests/analyzer/test_transition_levels.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     1539 2022-11-16 04:16:01.000000 pydefect-0.9.4/pydefect/tests/analyzer/test_transition_levels_plotter.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     2014 2023-05-10 06:40:55.000000 pydefect-0.9.4/pydefect/tests/analyzer/test_unitcell.py
+drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2024-05-07 00:39:22.100146 pydefect-0.9.4/pydefect/tests/chem_pot_diag/
+-rw-r--r--   0 kumagai    (501) staff       (20)      169 2020-11-30 07:08:52.000000 pydefect-0.9.4/pydefect/tests/chem_pot_diag/cpd.yaml
+drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2024-05-07 00:39:22.108182 pydefect-0.9.4/pydefect/tests/cli/
+-rw-r--r--   0 kumagai    (501) staff       (20)       95 2020-05-18 00:09:10.000000 pydefect-0.9.4/pydefect/tests/cli/__init__.py
+-rw-r--r--   0 kumagai    (501) staff       (20)    10359 2023-11-08 22:17:17.000000 pydefect-0.9.4/pydefect/tests/cli/test_main.py
+-rw-r--r--   0 kumagai    (501) staff       (20)    11282 2023-11-08 22:16:01.000000 pydefect-0.9.4/pydefect/tests/cli/test_main_functions.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     1980 2022-10-10 09:24:54.000000 pydefect-0.9.4/pydefect/tests/cli/test_main_tools.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     5032 2023-11-09 01:04:55.000000 pydefect-0.9.4/pydefect/tests/cli/test_main_util.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     5312 2023-09-20 06:33:01.000000 pydefect-0.9.4/pydefect/tests/cli/test_main_util_functions.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     3011 2021-05-15 12:24:21.000000 pydefect-0.9.4/pydefect/tests/cli/test_make_defect_vesta_file.py
+drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2024-05-07 00:39:22.124189 pydefect-0.9.4/pydefect/tests/cli/vasp/
+-rw-r--r--   0 kumagai    (501) staff       (20)       95 2020-05-18 00:09:10.000000 pydefect-0.9.4/pydefect/tests/cli/vasp/__init__.py
+-rwxr-xr-x   0 kumagai    (501) staff       (20)     1009 2024-05-06 23:55:16.000000 pydefect-0.9.4/pydefect/tests/cli/vasp/test_get_defect_charge_state.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     4907 2022-11-22 04:59:59.000000 pydefect-0.9.4/pydefect/tests/cli/vasp/test_main_vasp.py
+-rw-r--r--   0 kumagai    (501) staff       (20)    10434 2023-11-09 01:02:43.000000 pydefect-0.9.4/pydefect/tests/cli/vasp/test_main_vasp_functions.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     2779 2023-05-28 21:34:46.000000 pydefect-0.9.4/pydefect/tests/cli/vasp/test_main_vasp_util.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     5041 2023-05-28 21:34:15.000000 pydefect-0.9.4/pydefect/tests/cli/vasp/test_main_vasp_util_functions.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     7433 2023-11-09 00:30:18.000000 pydefect-0.9.4/pydefect/tests/cli/vasp/test_make_band_edge_orbital_infos.py
+-rw-r--r--   0 kumagai    (501) staff       (20)      873 2023-03-26 01:11:16.000000 pydefect-0.9.4/pydefect/tests/cli/vasp/test_make_calc_results.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     2700 2024-03-31 01:49:22.000000 pydefect-0.9.4/pydefect/tests/cli/vasp/test_make_composition_energies_from_mp.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     2164 2021-08-06 10:10:20.000000 pydefect-0.9.4/pydefect/tests/cli/vasp/test_make_defect_charge_info.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     2385 2021-03-05 09:52:57.000000 pydefect-0.9.4/pydefect/tests/cli/vasp/test_make_efnv_correction.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     1619 2021-04-12 08:07:10.000000 pydefect-0.9.4/pydefect/tests/cli/vasp/test_make_gkfo_correction.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     2178 2021-04-29 04:12:46.000000 pydefect-0.9.4/pydefect/tests/cli/vasp/test_make_local_extrema.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     1429 2023-03-26 01:11:16.000000 pydefect-0.9.4/pydefect/tests/cli/vasp/test_make_perfect_band_edge_state.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     1557 2022-05-20 02:54:43.000000 pydefect-0.9.4/pydefect/tests/cli/vasp/test_make_poscars_from_query.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     1538 2023-03-26 01:11:16.000000 pydefect-0.9.4/pydefect/tests/cli/vasp/test_make_unitcell.py
+-rw-r--r--   0 kumagai    (501) staff       (20)      216 2021-04-23 05:16:53.000000 pydefect-0.9.4/pydefect/tests/cli/vasp/unitcell.yaml
+drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2024-05-07 00:39:21.973435 pydefect-0.9.4/pydefect/tests/cli/vasp/vasp_files/
+drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2024-05-07 00:39:22.125294 pydefect-0.9.4/pydefect/tests/cli/vasp/vasp_files/KInO2_Va_O_2/
+-rw-r--r--   0 kumagai    (501) staff       (20)       18 2020-05-31 08:54:40.000000 pydefect-0.9.4/pydefect/tests/cli/vasp/vasp_files/KInO2_Va_O_2/pydefect.yaml
+-rw-r--r--   0 kumagai    (501) staff       (20)    14382 2023-05-10 00:54:37.000000 pydefect-0.9.4/pydefect/tests/conftest.py
+drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2024-05-07 00:39:22.131951 pydefect-0.9.4/pydefect/tests/corrections/
+-rw-r--r--   0 kumagai    (501) staff       (20)       61 2020-06-14 07:43:24.000000 pydefect-0.9.4/pydefect/tests/corrections/__init__.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     1723 2021-04-26 01:56:50.000000 pydefect-0.9.4/pydefect/tests/corrections/test_efnv_correction.py
+-rw-r--r--   0 kumagai    (501) staff       (20)      963 2020-06-05 00:53:04.000000 pydefect-0.9.4/pydefect/tests/corrections/test_efnv_performance.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     3613 2021-03-02 02:40:28.000000 pydefect-0.9.4/pydefect/tests/corrections/test_ewald.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     2549 2020-11-25 07:07:18.000000 pydefect-0.9.4/pydefect/tests/corrections/test_gkfo_correction.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     2053 2023-11-30 00:17:18.000000 pydefect-0.9.4/pydefect/tests/corrections/test_site_potential_plotter.py
+drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2024-05-07 00:39:22.133139 pydefect-0.9.4/pydefect/tests/helpers/
+-rw-r--r--   0 kumagai    (501) staff       (20)        0 2020-05-14 10:39:18.000000 pydefect-0.9.4/pydefect/tests/helpers/__init__.py
+drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2024-05-07 00:39:22.148668 pydefect-0.9.4/pydefect/tests/input_maker/
+-rw-r--r--   0 kumagai    (501) staff       (20)      347 2020-08-05 23:35:58.000000 pydefect-0.9.4/pydefect/tests/input_maker/POSCAR
+-rw-r--r--   0 kumagai    (501) staff       (20)        0 2020-05-14 10:46:18.000000 pydefect-0.9.4/pydefect/tests/input_maker/__init__.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     2704 2021-04-28 11:25:22.000000 pydefect-0.9.4/pydefect/tests/input_maker/test_append_interstitial.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     1923 2023-03-13 01:10:15.000000 pydefect-0.9.4/pydefect/tests/input_maker/test_complex_defect_entries_make.py
+-rw-r--r--   0 kumagai    (501) staff       (20)      810 2023-03-13 00:52:36.000000 pydefect-0.9.4/pydefect/tests/input_maker/test_complex_defect_set.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     1230 2022-09-30 06:02:25.000000 pydefect-0.9.4/pydefect/tests/input_maker/test_defect.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     5834 2021-08-06 10:14:07.000000 pydefect-0.9.4/pydefect/tests/input_maker/test_defect_entries_maker.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     4367 2022-09-30 06:12:21.000000 pydefect-0.9.4/pydefect/tests/input_maker/test_defect_entry.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     1551 2022-07-01 01:20:10.000000 pydefect-0.9.4/pydefect/tests/input_maker/test_defect_set.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     2139 2020-12-23 03:22:55.000000 pydefect-0.9.4/pydefect/tests/input_maker/test_defect_set_maker.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     4174 2021-08-06 10:11:01.000000 pydefect-0.9.4/pydefect/tests/input_maker/test_local_extrema.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     2368 2023-01-28 01:19:23.000000 pydefect-0.9.4/pydefect/tests/input_maker/test_manual_supercell_maker.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     3571 2021-03-05 09:52:57.000000 pydefect-0.9.4/pydefect/tests/input_maker/test_supercell.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     4443 2023-01-27 05:27:59.000000 pydefect-0.9.4/pydefect/tests/input_maker/test_supercell_info.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     5411 2024-05-06 23:59:02.000000 pydefect-0.9.4/pydefect/tests/input_maker/test_supercell_maker.py
+drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2024-05-07 00:39:21.974866 pydefect-0.9.4/pydefect/tests/test_data_files/
+drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2024-05-07 00:39:22.149716 pydefect-0.9.4/pydefect/tests/test_data_files/Na3AgO2/
+-rw-r--r--   0 kumagai    (501) staff       (20)     3145 2023-01-31 23:38:38.000000 pydefect-0.9.4/pydefect/tests/test_data_files/Na3AgO2/degeneracies.yaml
+drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2024-05-07 00:39:22.156084 pydefect-0.9.4/pydefect/util/
+-rw-r--r--   0 kumagai    (501) staff       (20)       95 2020-05-26 03:04:22.000000 pydefect-0.9.4/pydefect/util/__init__.py
+-rw-r--r--   0 kumagai    (501) staff       (20)      245 2021-04-06 09:47:19.000000 pydefect-0.9.4/pydefect/util/coords.py
+-rw-r--r--   0 kumagai    (501) staff       (20)      351 2023-11-08 22:28:42.000000 pydefect-0.9.4/pydefect/util/error_classes.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     1315 2024-04-12 20:25:44.000000 pydefect-0.9.4/pydefect/util/mp_tools.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     2457 2023-11-30 00:19:15.000000 pydefect-0.9.4/pydefect/util/prepare_names.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     2727 2021-04-26 23:23:36.000000 pydefect-0.9.4/pydefect/util/structure_tools.py
+drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2024-05-07 00:39:21.982533 pydefect-0.9.4/pydefect.egg-info/
+-rw-r--r--   0 kumagai    (501) staff       (20)      397 2024-05-07 00:39:21.000000 pydefect-0.9.4/pydefect.egg-info/PKG-INFO
+-rw-r--r--   0 kumagai    (501) staff       (20)     8291 2024-05-07 00:39:21.000000 pydefect-0.9.4/pydefect.egg-info/SOURCES.txt
+-rw-r--r--   0 kumagai    (501) staff       (20)        1 2024-05-07 00:39:21.000000 pydefect-0.9.4/pydefect.egg-info/dependency_links.txt
+-rw-r--r--   0 kumagai    (501) staff       (20)      256 2024-05-07 00:39:21.000000 pydefect-0.9.4/pydefect.egg-info/entry_points.txt
+-rw-r--r--   0 kumagai    (501) staff       (20)       69 2024-05-07 00:39:21.000000 pydefect-0.9.4/pydefect.egg-info/requires.txt
+-rw-r--r--   0 kumagai    (501) staff       (20)        9 2024-05-07 00:39:21.000000 pydefect-0.9.4/pydefect.egg-info/top_level.txt
+-rw-r--r--   0 kumagai    (501) staff       (20)       38 2024-05-07 00:39:22.157564 pydefect-0.9.4/setup.cfg
+-rw-r--r--   0 kumagai    (501) staff       (20)     1335 2021-08-06 00:13:51.000000 pydefect-0.9.4/setup.py
```

### Comparing `pydefect-0.9.3/README.md` & `pydefect-0.9.4/README.md`

 * *Files identical despite different names*

### Comparing `pydefect-0.9.3/pydefect/analyzer/_defect_charge_distribution.py` & `pydefect-0.9.4/pydefect/analyzer/_defect_charge_distribution.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.9.3/pydefect/analyzer/band_edge_states.py` & `pydefect-0.9.4/pydefect/analyzer/band_edge_states.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.9.3/pydefect/analyzer/calc_results.py` & `pydefect-0.9.4/pydefect/analyzer/calc_results.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.9.3/pydefect/analyzer/calc_summary.py` & `pydefect-0.9.4/pydefect/analyzer/calc_summary.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.9.3/pydefect/analyzer/concentration/concentration.py` & `pydefect-0.9.4/pydefect/analyzer/concentration/concentration.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.9.3/pydefect/analyzer/concentration/degeneracy.py` & `pydefect-0.9.4/pydefect/analyzer/concentration/degeneracy.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.9.3/pydefect/analyzer/concentration/make_concentration.py` & `pydefect-0.9.4/pydefect/analyzer/concentration/make_concentration.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.9.3/pydefect/analyzer/concentration/plot_concentration.py` & `pydefect-0.9.4/pydefect/analyzer/concentration/plot_concentration.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.9.3/pydefect/analyzer/defect_charge_info.py` & `pydefect-0.9.4/pydefect/analyzer/defect_charge_info.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.9.3/pydefect/analyzer/defect_energy.py` & `pydefect-0.9.4/pydefect/analyzer/defect_energy.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.9.3/pydefect/analyzer/defect_energy_plotter.py` & `pydefect-0.9.4/pydefect/analyzer/defect_energy_plotter.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.9.3/pydefect/analyzer/defect_energy_util.py` & `pydefect-0.9.4/pydefect/analyzer/defect_energy_util.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.9.3/pydefect/analyzer/defect_structure_comparator.py` & `pydefect-0.9.4/pydefect/analyzer/defect_structure_comparator.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.9.3/pydefect/analyzer/defect_structure_info.py` & `pydefect-0.9.4/pydefect/analyzer/defect_structure_info.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.9.3/pydefect/analyzer/eigenvalue_plotter.py` & `pydefect-0.9.4/pydefect/analyzer/eigenvalue_plotter.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.9.3/pydefect/analyzer/grids.py` & `pydefect-0.9.4/pydefect/analyzer/grids.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.9.3/pydefect/analyzer/make_band_edge_states.py` & `pydefect-0.9.4/pydefect/analyzer/make_band_edge_states.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.9.3/pydefect/analyzer/make_calc_summary.py` & `pydefect-0.9.4/pydefect/analyzer/make_calc_summary.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.9.3/pydefect/analyzer/make_defect_energy_info.py` & `pydefect-0.9.4/pydefect/analyzer/make_defect_energy_info.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.9.3/pydefect/analyzer/make_defect_energy_summary.py` & `pydefect-0.9.4/pydefect/analyzer/make_defect_energy_summary.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.9.3/pydefect/analyzer/make_defect_structure_info.py` & `pydefect-0.9.4/pydefect/analyzer/make_defect_structure_info.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.9.3/pydefect/analyzer/pinning_levels.py` & `pydefect-0.9.4/pydefect/analyzer/pinning_levels.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.9.3/pydefect/analyzer/refine_defect_structure.py` & `pydefect-0.9.4/pydefect/analyzer/refine_defect_structure.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.9.3/pydefect/analyzer/transition_levels.py` & `pydefect-0.9.4/pydefect/analyzer/transition_levels.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.9.3/pydefect/analyzer/transition_levels_plotter.py` & `pydefect-0.9.4/pydefect/analyzer/transition_levels_plotter.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.9.3/pydefect/analyzer/unitcell.py` & `pydefect-0.9.4/pydefect/analyzer/unitcell.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.9.3/pydefect/chem_pot_diag/chem_pot_diag.py` & `pydefect-0.9.4/pydefect/chem_pot_diag/chem_pot_diag.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.9.3/pydefect/chem_pot_diag/cpd_plotter.py` & `pydefect-0.9.4/pydefect/chem_pot_diag/cpd_plotter.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.9.3/pydefect/cli/main.py` & `pydefect-0.9.4/pydefect/cli/main.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.9.3/pydefect/cli/main_functions.py` & `pydefect-0.9.4/pydefect/cli/main_functions.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.9.3/pydefect/cli/main_tools.py` & `pydefect-0.9.4/pydefect/cli/main_tools.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.9.3/pydefect/cli/main_util.py` & `pydefect-0.9.4/pydefect/cli/main_util.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.9.3/pydefect/cli/main_util_functions.py` & `pydefect-0.9.4/pydefect/cli/main_util_functions.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.9.3/pydefect/cli/make_defect_vesta_file.py` & `pydefect-0.9.4/pydefect/cli/make_defect_vesta_file.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.9.3/pydefect/cli/vasp/get_defect_charge_state.py` & `pydefect-0.9.4/pydefect/cli/vasp/get_defect_charge_state.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.9.3/pydefect/cli/vasp/main_vasp.py` & `pydefect-0.9.4/pydefect/cli/vasp/main_vasp.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.9.3/pydefect/cli/vasp/main_vasp_functions.py` & `pydefect-0.9.4/pydefect/cli/vasp/main_vasp_functions.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.9.3/pydefect/cli/vasp/main_vasp_util.py` & `pydefect-0.9.4/pydefect/cli/vasp/main_vasp_util.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.9.3/pydefect/cli/vasp/main_vasp_util_functions.py` & `pydefect-0.9.4/pydefect/cli/vasp/main_vasp_util_functions.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.9.3/pydefect/cli/vasp/make_band_edge_orbital_infos.py` & `pydefect-0.9.4/pydefect/cli/vasp/make_band_edge_orbital_infos.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.9.3/pydefect/cli/vasp/make_calc_results.py` & `pydefect-0.9.4/pydefect/cli/vasp/make_calc_results.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.9.3/pydefect/cli/vasp/make_composition_energies_from_mp.py` & `pydefect-0.9.4/pydefect/cli/vasp/make_composition_energies_from_mp.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.9.3/pydefect/cli/vasp/make_defect_charge_info.py` & `pydefect-0.9.4/pydefect/cli/vasp/make_defect_charge_info.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.9.3/pydefect/cli/vasp/make_efnv_correction.py` & `pydefect-0.9.4/pydefect/cli/vasp/make_efnv_correction.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 # -*- coding: utf-8 -*-
 #  Copyright (c) 2020. Distributed under the terms of the MIT License.
-from typing import Optional
+from typing import Optional, Tuple
 
 import numpy as np
 from numpy import dot, cross
 from numpy.linalg import norm
 
 from pydefect.analyzer.calc_results import CalcResults
 from pydefect.analyzer.defect_structure_comparator import \
     DefectStructureComparator
 from pydefect.corrections.efnv_correction import \
     ExtendedFnvCorrection, PotentialSite
 from pydefect.corrections.ewald import Ewald
 from pydefect.defaults import defaults
 from pydefect.util.error_classes import SupercellError, \
     NoCalculatedPotentialSiteError
-from vise.util.logger import get_logger
-from vise.util.typing import Coords
 
-logger = get_logger(__name__)
+
+Coords = Tuple[float, float, float]
 
 
 def make_efnv_correction(charge: float,
                          calc_results: CalcResults,
                          perfect_calc_results: CalcResults,
                          dielectric_tensor: np.array,
                          defect_coords: Optional[Coords] = None,
```

### Comparing `pydefect-0.9.3/pydefect/cli/vasp/make_gkfo_correction.py` & `pydefect-0.9.4/pydefect/cli/vasp/make_gkfo_correction.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.9.3/pydefect/cli/vasp/make_local_extrema.py` & `pydefect-0.9.4/pydefect/cli/vasp/make_local_extrema.py`

 * *Files 1% similar despite different names*

```diff
@@ -426,16 +426,16 @@
     def _dist_mat(self, pos_frac):
         # return a matrix that contains the distances
         aa = np.linspace(0, 1, len(self.chgcar.get_axis_grid(0)), endpoint=False)
         bb = np.linspace(0, 1, len(self.chgcar.get_axis_grid(1)), endpoint=False)
         cc = np.linspace(0, 1, len(self.chgcar.get_axis_grid(2)), endpoint=False)
         AA, BB, CC = np.meshgrid(aa, bb, cc, indexing="ij")
         dist_from_pos = self.chgcar.structure.lattice.get_all_distances(
-            fcoords1=np.vstack([AA.flatten(), BB.flatten(), CC.flatten()]).T,
-            fcoords2=pos_frac,
+            np.vstack([AA.flatten(), BB.flatten(), CC.flatten()]).T,
+            pos_frac,
         )
         return dist_from_pos.reshape(AA.shape)
 
 
 def extrema_coords(volumetric_data: VolumetricData,
                    find_min: bool,
                    params: VolumetricDataAnalyzeParams) -> DataFrame:
```

### Comparing `pydefect-0.9.3/pydefect/cli/vasp/make_perfect_band_edge_state.py` & `pydefect-0.9.4/pydefect/cli/vasp/make_perfect_band_edge_state.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.9.3/pydefect/cli/vasp/make_poscars_from_query.py` & `pydefect-0.9.4/pydefect/cli/vasp/make_poscars_from_query.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.9.3/pydefect/cli/vasp/make_unitcell.py` & `pydefect-0.9.4/pydefect/cli/vasp/make_unitcell.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.9.3/pydefect/cli/vasp/molecules/H2O/POSCAR` & `pydefect-0.9.4/pydefect/cli/vasp/molecules/H2O/POSCAR`

 * *Files identical despite different names*

### Comparing `pydefect-0.9.3/pydefect/cli/vasp/molecules/NH3/POSCAR` & `pydefect-0.9.4/pydefect/cli/vasp/molecules/NH3/POSCAR`

 * *Files identical despite different names*

### Comparing `pydefect-0.9.3/pydefect/cli/vasp/molecules/NO2/POSCAR` & `pydefect-0.9.4/pydefect/cli/vasp/molecules/NO2/POSCAR`

 * *Files identical despite different names*

### Comparing `pydefect-0.9.3/pydefect/cli/vasp/molecules/molecule_data.yaml` & `pydefect-0.9.4/pydefect/cli/vasp/molecules/molecule_data.yaml`

 * *Files identical despite different names*

### Comparing `pydefect-0.9.3/pydefect/corrections/abstract_correction.py` & `pydefect-0.9.4/pydefect/corrections/abstract_correction.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.9.3/pydefect/corrections/efnv_correction.py` & `pydefect-0.9.4/pydefect/corrections/efnv_correction.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.9.3/pydefect/corrections/ewald.py` & `pydefect-0.9.4/pydefect/corrections/ewald.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.9.3/pydefect/corrections/gkfo_correction.py` & `pydefect-0.9.4/pydefect/corrections/gkfo_correction.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.9.3/pydefect/corrections/site_potential_plotter.py` & `pydefect-0.9.4/pydefect/corrections/site_potential_plotter.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.9.3/pydefect/database/database.py` & `pydefect-0.9.4/pydefect/database/database.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.9.3/pydefect/database/electronegativity.yaml` & `pydefect-0.9.4/pydefect/database/electronegativity.yaml`

 * *Files identical despite different names*

### Comparing `pydefect-0.9.3/pydefect/database/rcore.yaml` & `pydefect-0.9.4/pydefect/database/rcore.yaml`

 * *Files identical despite different names*

### Comparing `pydefect-0.9.3/pydefect/defaults.py` & `pydefect-0.9.4/pydefect/defaults.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.9.3/pydefect/input_maker/append_interstitial.py` & `pydefect-0.9.4/pydefect/input_maker/append_interstitial.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.9.3/pydefect/input_maker/complex_defect_entries_make.py` & `pydefect-0.9.4/pydefect/input_maker/complex_defect_entries_make.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.9.3/pydefect/input_maker/complex_defect_set.py` & `pydefect-0.9.4/pydefect/input_maker/complex_defect_set.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 # -*- coding: utf-8 -*-
 #  Copyright (c) 2023 Kumagai group.
-from collections import Iterable
+try:
+    from collections import Iterable
+except ImportError:
+    from collections.abc import Iterable
+
 from dataclasses import dataclass
 from typing import List, Dict, Optional, Iterator
 
 from monty.serialization import loadfn
 
 
 @dataclass
```

### Comparing `pydefect-0.9.3/pydefect/input_maker/defect.py` & `pydefect-0.9.4/pydefect/input_maker/defect.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.9.3/pydefect/input_maker/defect_entries_maker.py` & `pydefect-0.9.4/pydefect/input_maker/defect_entries_maker.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.9.3/pydefect/input_maker/defect_entry.py` & `pydefect-0.9.4/pydefect/input_maker/defect_entry.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.9.3/pydefect/input_maker/defect_set.py` & `pydefect-0.9.4/pydefect/input_maker/defect_set.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.9.3/pydefect/input_maker/defect_set_maker.py` & `pydefect-0.9.4/pydefect/input_maker/defect_set_maker.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.9.3/pydefect/input_maker/local_extrema.py` & `pydefect-0.9.4/pydefect/input_maker/local_extrema.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.9.3/pydefect/input_maker/manual_supercell_maker.py` & `pydefect-0.9.4/pydefect/input_maker/manual_supercell_maker.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.9.3/pydefect/input_maker/supercell.py` & `pydefect-0.9.4/pydefect/input_maker/supercell.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.9.3/pydefect/input_maker/supercell_info.py` & `pydefect-0.9.4/pydefect/input_maker/supercell_info.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.9.3/pydefect/input_maker/supercell_maker.py` & `pydefect-0.9.4/pydefect/input_maker/supercell_maker.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.9.3/pydefect/tests/analyzer/POSCAR` & `pydefect-0.9.4/pydefect/tests/analyzer/POSCAR`

 * *Files identical despite different names*

### Comparing `pydefect-0.9.3/pydefect/tests/analyzer/concentration/test_concentration.py` & `pydefect-0.9.4/pydefect/tests/analyzer/concentration/test_concentration.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.9.3/pydefect/tests/analyzer/concentration/test_degeneracy.py` & `pydefect-0.9.4/pydefect/tests/analyzer/concentration/test_degeneracy.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.9.3/pydefect/tests/analyzer/concentration/test_make_concentration.py` & `pydefect-0.9.4/pydefect/tests/analyzer/concentration/test_make_concentration.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.9.3/pydefect/tests/analyzer/concentration/test_plot_concentration.py` & `pydefect-0.9.4/pydefect/tests/analyzer/concentration/test_plot_concentration.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.9.3/pydefect/tests/analyzer/test_band_edge_states.py` & `pydefect-0.9.4/pydefect/tests/analyzer/test_band_edge_states.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.9.3/pydefect/tests/analyzer/test_calc_results.py` & `pydefect-0.9.4/pydefect/tests/analyzer/test_calc_results.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.9.3/pydefect/tests/analyzer/test_calc_summary.py` & `pydefect-0.9.4/pydefect/tests/analyzer/test_calc_summary.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.9.3/pydefect/tests/analyzer/test_defect_charge_info.py` & `pydefect-0.9.4/pydefect/tests/analyzer/test_defect_charge_info.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.9.3/pydefect/tests/analyzer/test_defect_energy.py` & `pydefect-0.9.4/pydefect/tests/analyzer/test_defect_energy.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.9.3/pydefect/tests/analyzer/test_defect_energy_plotter.py` & `pydefect-0.9.4/pydefect/tests/analyzer/test_defect_energy_plotter.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.9.3/pydefect/tests/analyzer/test_defect_energy_util.py` & `pydefect-0.9.4/pydefect/tests/analyzer/test_defect_energy_util.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.9.3/pydefect/tests/analyzer/test_defect_structure_comparator.py` & `pydefect-0.9.4/pydefect/tests/analyzer/test_defect_structure_comparator.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.9.3/pydefect/tests/analyzer/test_defect_structure_info.py` & `pydefect-0.9.4/pydefect/tests/analyzer/test_defect_structure_info.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.9.3/pydefect/tests/analyzer/test_eigenvalue_plotter.py` & `pydefect-0.9.4/pydefect/tests/analyzer/test_eigenvalue_plotter.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.9.3/pydefect/tests/analyzer/test_grids.py` & `pydefect-0.9.4/pydefect/tests/analyzer/test_grids.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.9.3/pydefect/tests/analyzer/test_make_band_edge_states.py` & `pydefect-0.9.4/pydefect/tests/analyzer/test_make_band_edge_states.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.9.3/pydefect/tests/analyzer/test_make_calc_summary.py` & `pydefect-0.9.4/pydefect/tests/analyzer/test_make_calc_summary.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.9.3/pydefect/tests/analyzer/test_make_defect_energy_info.py` & `pydefect-0.9.4/pydefect/tests/analyzer/test_make_defect_energy_info.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.9.3/pydefect/tests/analyzer/test_make_defect_energy_summary.py` & `pydefect-0.9.4/pydefect/tests/analyzer/test_make_defect_energy_summary.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.9.3/pydefect/tests/analyzer/test_make_defect_structure_info.py` & `pydefect-0.9.4/pydefect/tests/analyzer/test_make_defect_structure_info.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.9.3/pydefect/tests/analyzer/test_pinning_levels.py` & `pydefect-0.9.4/pydefect/tests/analyzer/test_pinning_levels.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.9.3/pydefect/tests/analyzer/test_refine_defect_structure.py` & `pydefect-0.9.4/pydefect/tests/analyzer/test_refine_defect_structure.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.9.3/pydefect/tests/analyzer/test_transition_levels.py` & `pydefect-0.9.4/pydefect/tests/analyzer/test_transition_levels.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.9.3/pydefect/tests/analyzer/test_transition_levels_plotter.py` & `pydefect-0.9.4/pydefect/tests/analyzer/test_transition_levels_plotter.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.9.3/pydefect/tests/analyzer/test_unitcell.py` & `pydefect-0.9.4/pydefect/tests/analyzer/test_unitcell.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.9.3/pydefect/tests/cli/test_main.py` & `pydefect-0.9.4/pydefect/tests/cli/test_main.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.9.3/pydefect/tests/cli/test_main_functions.py` & `pydefect-0.9.4/pydefect/tests/cli/test_main_functions.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.9.3/pydefect/tests/cli/test_main_tools.py` & `pydefect-0.9.4/pydefect/tests/cli/test_main_tools.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.9.3/pydefect/tests/cli/test_main_util.py` & `pydefect-0.9.4/pydefect/tests/cli/test_main_util.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.9.3/pydefect/tests/cli/test_main_util_functions.py` & `pydefect-0.9.4/pydefect/tests/cli/test_main_util_functions.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.9.3/pydefect/tests/cli/test_make_defect_vesta_file.py` & `pydefect-0.9.4/pydefect/tests/cli/test_make_defect_vesta_file.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.9.3/pydefect/tests/cli/vasp/test_main_vasp.py` & `pydefect-0.9.4/pydefect/tests/cli/vasp/test_main_vasp.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.9.3/pydefect/tests/cli/vasp/test_main_vasp_functions.py` & `pydefect-0.9.4/pydefect/tests/cli/vasp/test_main_vasp_functions.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.9.3/pydefect/tests/cli/vasp/test_main_vasp_util.py` & `pydefect-0.9.4/pydefect/tests/cli/vasp/test_main_vasp_util.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.9.3/pydefect/tests/cli/vasp/test_main_vasp_util_functions.py` & `pydefect-0.9.4/pydefect/tests/cli/vasp/test_main_vasp_util_functions.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.9.3/pydefect/tests/cli/vasp/test_make_band_edge_orbital_infos.py` & `pydefect-0.9.4/pydefect/tests/cli/vasp/test_make_band_edge_orbital_infos.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.9.3/pydefect/tests/cli/vasp/test_make_calc_results.py` & `pydefect-0.9.4/pydefect/tests/cli/vasp/test_make_calc_results.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.9.3/pydefect/tests/cli/vasp/test_make_composition_energies_from_mp.py` & `pydefect-0.9.4/pydefect/tests/cli/vasp/test_make_composition_energies_from_mp.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.9.3/pydefect/tests/cli/vasp/test_make_defect_charge_info.py` & `pydefect-0.9.4/pydefect/tests/cli/vasp/test_make_defect_charge_info.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.9.3/pydefect/tests/cli/vasp/test_make_efnv_correction.py` & `pydefect-0.9.4/pydefect/tests/cli/vasp/test_make_efnv_correction.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.9.3/pydefect/tests/cli/vasp/test_make_gkfo_correction.py` & `pydefect-0.9.4/pydefect/tests/cli/vasp/test_make_gkfo_correction.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.9.3/pydefect/tests/cli/vasp/test_make_local_extrema.py` & `pydefect-0.9.4/pydefect/tests/cli/vasp/test_make_local_extrema.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.9.3/pydefect/tests/cli/vasp/test_make_perfect_band_edge_state.py` & `pydefect-0.9.4/pydefect/tests/cli/vasp/test_make_perfect_band_edge_state.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.9.3/pydefect/tests/cli/vasp/test_make_poscars_from_query.py` & `pydefect-0.9.4/pydefect/tests/cli/vasp/test_make_poscars_from_query.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.9.3/pydefect/tests/cli/vasp/test_make_unitcell.py` & `pydefect-0.9.4/pydefect/tests/cli/vasp/test_make_unitcell.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.9.3/pydefect/tests/conftest.py` & `pydefect-0.9.4/pydefect/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.9.3/pydefect/tests/corrections/test_efnv_correction.py` & `pydefect-0.9.4/pydefect/tests/corrections/test_efnv_correction.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.9.3/pydefect/tests/corrections/test_efnv_performance.py` & `pydefect-0.9.4/pydefect/tests/corrections/test_efnv_performance.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.9.3/pydefect/tests/corrections/test_ewald.py` & `pydefect-0.9.4/pydefect/tests/corrections/test_ewald.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.9.3/pydefect/tests/corrections/test_gkfo_correction.py` & `pydefect-0.9.4/pydefect/tests/corrections/test_gkfo_correction.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.9.3/pydefect/tests/corrections/test_site_potential_plotter.py` & `pydefect-0.9.4/pydefect/tests/corrections/test_site_potential_plotter.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.9.3/pydefect/tests/input_maker/test_append_interstitial.py` & `pydefect-0.9.4/pydefect/tests/input_maker/test_append_interstitial.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.9.3/pydefect/tests/input_maker/test_complex_defect_entries_make.py` & `pydefect-0.9.4/pydefect/tests/input_maker/test_complex_defect_entries_make.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.9.3/pydefect/tests/input_maker/test_complex_defect_set.py` & `pydefect-0.9.4/pydefect/tests/input_maker/test_complex_defect_set.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.9.3/pydefect/tests/input_maker/test_defect.py` & `pydefect-0.9.4/pydefect/tests/input_maker/test_defect.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.9.3/pydefect/tests/input_maker/test_defect_entries_maker.py` & `pydefect-0.9.4/pydefect/tests/input_maker/test_defect_entries_maker.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.9.3/pydefect/tests/input_maker/test_defect_entry.py` & `pydefect-0.9.4/pydefect/tests/input_maker/test_defect_entry.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.9.3/pydefect/tests/input_maker/test_defect_set.py` & `pydefect-0.9.4/pydefect/tests/input_maker/test_defect_set.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.9.3/pydefect/tests/input_maker/test_defect_set_maker.py` & `pydefect-0.9.4/pydefect/tests/input_maker/test_defect_set_maker.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.9.3/pydefect/tests/input_maker/test_local_extrema.py` & `pydefect-0.9.4/pydefect/tests/input_maker/test_local_extrema.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.9.3/pydefect/tests/input_maker/test_manual_supercell_maker.py` & `pydefect-0.9.4/pydefect/tests/input_maker/test_manual_supercell_maker.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.9.3/pydefect/tests/input_maker/test_supercell.py` & `pydefect-0.9.4/pydefect/tests/input_maker/test_supercell.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.9.3/pydefect/tests/input_maker/test_supercell_info.py` & `pydefect-0.9.4/pydefect/tests/input_maker/test_supercell_info.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.9.3/pydefect/tests/input_maker/test_supercell_maker.py` & `pydefect-0.9.4/pydefect/tests/input_maker/test_supercell_maker.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
                [0,  2,  0],
                [0,  0,  1]]
     np.testing.assert_array_equal(actual, expected)
 
 
 def test_create_supercell_raise_not_primitive_error(bcc):
     with pytest.raises(NotPrimitiveError):
-        SupercellMaker(primitive_structure=bcc)
+        SupercellMaker(primitive_structure=bcc, raise_error=True)
 
 
 def test_create_supercell_matrix(a_centered_orthorhombic):
     matrix = [[2, 0, 0], [0, 1, 0], [0, 0, 1]]
     cs = SupercellMaker(a_centered_orthorhombic, matrix=matrix)
     actual = cs.supercell.matrix
     np.testing.assert_array_equal(actual, matrix)
```

### Comparing `pydefect-0.9.3/pydefect/tests/test_data_files/Na3AgO2/degeneracies.yaml` & `pydefect-0.9.4/pydefect/tests/test_data_files/Na3AgO2/degeneracies.yaml`

 * *Files identical despite different names*

### Comparing `pydefect-0.9.3/pydefect/util/mp_tools.py` & `pydefect-0.9.4/pydefect/util/mp_tools.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,15 +22,14 @@
             logger.info("Note that you're using the newer MPRester.")
             default_fields = ["material_id", "formula_pretty", "structure",
                               "symmetry", "band_gap", "total_magnetization",
                               "types_of_magnetic_species"]
             properties = properties or default_fields
             self.materials = m.materials.summary.search(
                 chemsys=chemsys(element_list),
-                num_elements=(1, len(element_list)),
                 energy_above_hull=(-1e-5, e_above_hull),
                 fields=properties)
 
 
 def chemsys(element_list: list):
     result = []
     for i in range(1, len(element_list)+1):
```

### Comparing `pydefect-0.9.3/pydefect/util/prepare_names.py` & `pydefect-0.9.4/pydefect/util/prepare_names.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.9.3/pydefect/util/structure_tools.py` & `pydefect-0.9.4/pydefect/util/structure_tools.py`

 * *Files identical despite different names*

### Comparing `pydefect-0.9.3/setup.py` & `pydefect-0.9.4/setup.py`

 * *Files identical despite different names*

